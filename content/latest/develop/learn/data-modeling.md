---
title: 2. Data Modelling
linkTitle: 2. Data Modelling
description: Data Modelling
aliases:
  - /develop/learn/data-modelling/
menu:
  latest:
    identifier: data-modelling
    parent: learn
    weight: 562
---

Data modeling is a process that involves identifying the entities (items to be stored) and the relationships between entities. To create your data model, identify the patterns used to access data and the types of queries to be performed. These two ideas inform the organization and structure of the data, and the design and creation of the database's tables.

<ul class="nav nav-tabs nav-tabs-yb">
  <li class="active">
    <a href="#cassandra">
      <i class="icon-cassandra" aria-hidden="true"></i>
      Cassandra
    </a>
  </li>
</ul>

<div class="tab-content">
  <div id="cassandra" class="tab-pane fade in active">
    {{% includeMarkdown "cassandra/data-modeling.md" /%}}
  </div>
</div>