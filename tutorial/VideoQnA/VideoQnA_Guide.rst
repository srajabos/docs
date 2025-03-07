.. _VideoQnA_Guide:

VideoQnA
#################

.. note:: This guide is in its early development and is a work-in-progress with
   placeholder content.

Overview
********

VideoQnA is a framework that retrieves video based on provided user prompt. It uses only the video embeddings to perform vector similarity search in Intel's VDMS vector database and performs all operations on Intel Xeon CPU. The pipeline supports long form videos and time-based search.

Purpose
*******

How It Works
************

It utilizes the `GenAIComps <https://github.com/opea-project/GenAIComps>`_ microservice pipeline on Intel Xeon server. The steps include Docker image creation, container deployment via Docker Compose, and service execution to integrate microservices such as embedding, retriever, rerank, and lvm.
