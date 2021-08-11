<h1> Deploy your first subgraph with TheGraph Studio </h1>

<h3> Zora contract address: 0xabEFBc9fD2F806065b4f3C237d4b59D9A97Bcac7 </h3>

- npm install -g @graphprotocol/graph-cli

- graph init --contract-name Token --index-events --product subgraph-studio --from-contract 0xabEFBc9fD2F806065b4f3C237d4b59D9A97Bcac7

  Paste the info in the below step.

  Subgraph name: zora <br/>
  Directory to create the subgraph in: zora <br/>
  Ethereum network: minnet <br/>
  Contract address: 0xabEFBc9fD2F806065b4f3C237d4b59D9A97Bcac7 <br/>
  Contract Name: Token <br/>

- Edit `schema.graphql` file

- Edit `subgraph.yaml` file <br/>
  You can optionally specify startBlock in "dataSoruces/source"

- graph codegen <br/>
  You will see newly created `Token` folder in `generated` folder

- Edit `mapping.ts` file

- graph auth --studio <br/>
  Deploy key: \*\*\*\*Paste your studio deploy key here\*\*\*\*

- graph deploy --studio zora
