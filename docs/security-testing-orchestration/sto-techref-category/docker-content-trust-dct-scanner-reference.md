---
title: Docker Content Trust (DCT) scanner reference for STO
description: Image scans with Docker Content Trust
sidebar_label: Docker Content Trust (DCT) scanner reference
sidebar_position: 150
---

You can run Docker Content Trust (DCT) scans on your container images using a Security step: create a CI Build or Security Tests stage, add a Security step, and then add the `setting:value` pairs as specified below.

## Important notes for running Docker Content Trust scans in STO


### Docker-in-Docker requirements


import StoDinDRequirements from '/docs/security-testing-orchestration/sto-techref-category/shared/dind-bg-step.md';


<StoDinDRequirements />

### Root access requirements


import StoRootRequirements from '/docs/security-testing-orchestration/sto-techref-category/shared/root-access-requirements.md';


<StoRootRequirements />

### For more information


import StoMoreInfo from '/docs/security-testing-orchestration/sto-techref-category/shared/_more-information.md';


<StoMoreInfo />

## Security step settings for Docker Content Trust scans in STO

### Target and variant


import StoLegacyTargetAndVariant  from './shared/legacy/_sto-ref-legacy-target-and-variant.md';


<StoLegacyTargetAndVariant />

### Docker Content Trust (DCT) scan settings

* `product_name` = `docker-content-trust`
* [`scan_type`](/docs/security-testing-orchestration/sto-techref-category/security-step-settings-reference#scanner-categories) = `containerImage`
* [`policy_type`](/docs/security-testing-orchestration/sto-techref-category/security-step-settings-reference#data-ingestion-methods) = `orchestratedScan` or `ingestionOnly`
* `product_config_name` =`default`
* `fail_on_severity` - See [Fail on Severity](#fail-on-severity).

### Container image scan settings


import StoLegacyContainer from './shared/legacy/_sto-ref-legacy-container.md';


<StoLegacyContainer />

### Ingestion file


import StoLegacyIngest from './shared/legacy/_sto-ref-legacy-ingest.md';


<StoLegacyIngest />

### Fail on Severity


import StoSettingFailOnSeverity from './shared/step_palette/_sto-ref-ui-fail-on-severity.md';

<StoSettingFailOnSeverity />


<!-- CONTAINERS --------------------------------------------------------------------------- -->



