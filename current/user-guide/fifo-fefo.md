---
sidebar_position: 6
---

# FIFO/FEFO/FMFO queues

Here you can find description of FIFO/FEFO/FMFO queues based on Batches, Serial Numbers and for Items managed neither by Batches, nor Serial Numbers.

## Batch managed Items

- The queue type is chosen based on ProcessForce:

        - if it is installed: the queue type is taken from ProcessForce settings,
        - if it is not installed: you can choose the type in Custom Configuration → Manager → Enable Batch Management Manager → Set Default Settings
- FEFO – the queue is based on 'ExpDate' and (if ProcessForce is installed) U_ExpiryTime.
- FMFO – the queue is based on 'MnfDate'
- FIFO – "First In" is based on 'InDate'

## Serial Numbers managed Items, Items managed neither by Batches, nor Serial Numbers

It is always FIFO – uses ProcessForce implementation: takes a document creation date in ILM. It means that if after receipt to a Warehouse an Items is transferred, the date of the transfer will be taken under consideration (because it is the latest).

:::warning
    If with the FEFO queue there is no 'ExpDate' set for a Batch, during location search with this queue this will be recognized as the earliest date.
:::
