---
date: '2023-09-08T21:09:33+01:00'
draft: false
tags: [Java, Apache-PDFBox, Document-Automation]
categories: [blog]
title:  "Contract Generator"
---
## Purpose

Created an internal tool for a human resources company to automatically generate employment contracts from Excel data and a PDF template.

## Key Features

The script reads candidate and contract details from spreadsheets, fills PDF form fields, and exports one finalized contract per employee.

## Challenges

Several libraries seemed suitable, but they all had problems processing Chinese characters. Ultimately, the issue was successfully solved using a Java PDF library(Apache PDFBox)

## Implementation

Designed PDF form fields to match Excel column headers. Used Apache POI to read spreadsheet data and Apache PDFBox to populate PDF form fields and generate output files.