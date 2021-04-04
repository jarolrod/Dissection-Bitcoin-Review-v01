# Dissecting Bitcoin Core v0.21

Proposal: Review and update of the book "Dissection of Bitcoin"



* [Adresses](2_1_bitcoin_address.asciidoc)
* [Transactions](2_2_transactions.asciidoc)
* [Serialization](3_0_serialization.asciidoc)
  * [Original Implementation](3_0_serialization.asciidoc#original-implementation)
  * [Relevant Changes](3_0_serialization.asciidoc#relevant-changes)
    * [PR #352 - secure_allocator and zero_after_free_allocator](3_0_serialization.asciidoc#pr-352---secure_allocator-and-zero_after_free_allocator)
    * [PR #1567 - CHashWriter](3_0_serialization.asciidoc#pr-1567---chashwriter)
    * [PR #2409 - CSerializeData](3_0_serialization.asciidoc#pr-2409---cserializedata)
    * [PR #4508 - CSizeComputer](3_0_serialization.asciidoc#pr-4508---csizecomputer)
    * [PR #5510 - Big endian support](3_0_serialization.asciidoc#pr-5510---big-endian-support)
    * [PR #6914 - prevector](3_0_serialization.asciidoc#pr-6914---prevector)
  * [Transactions Serialization - Current Implementation (BIP 144)](3_0_serialization.asciidoc#transactions-serialization---current-implementation)
    * [VarInt](3_0_serialization.asciidoc#varint)
    * [SerializeTransaction()](https://github.com/leonardojobim/Dissection-Bitcoin-Test/blob/main/3_0_serialization.asciidoc#serializetransaction)
    * [UnserializeTransaction()](3_0_serialization.asciidoc#unserializetransaction)
    * [Serializing a transaction - Process](3_0_serialization.asciidoc#serializing-a-transaction---process)
      * [Sending Requested Transaction](3_0_serialization.asciidoc#sending-requested-transaction)