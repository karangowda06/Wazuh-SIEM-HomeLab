Architecture Overview

Endpoints with Wazuh agents forward logs to the Wazuh Manager.
The manager processes events using decoders and rules, then forwards
alerts to the Wazuh Indexer for storage and visualization in the Dashboard.

Data Flow

Agent → Manager → Indexer → Dashboard
