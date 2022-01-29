# 설명
- nft거래소
- 자체 계정을 운영하지 않고, 다른 wallet으로 이용 가능
- 오픈소스로 운영
- [OpenSea js API Github](https://github.com/ProjectOpenSea/opensea-js)
- [부가기능 자체 Contracts](https://github.com/ProjectOpenSea/opensea-creatures)
- 위의 `opensea-creatures`에서 나중에 web3 API로 직접 NFT 거래소를 제작할 때, 민팅/구매/전달/경매 등의 contracts의 구현 방법 참고 가능



# NFT 데이터 저장방식
1. centralized server
2. decentralized storage system `or` other blockchain
3. same blockchain as the NFT
- (추측) OpenSea는 기본적으로 1번방식으로 리소스를 저장하고, frozen을 사용하면 2번의 방식을 사용 (IPFS) (Filecoin같은 것)해서 저장해주는것으로 보임 ([filecoin with OpenSea](https://filecoin.io/blog/posts/opensea-decentralizes-and-persists-nft-storage-with-ipfs-and-filecoin/))




# Metadata 분산
- [article](https://opensea.io/blog/announcements/decentralizing-nft-metadata-on-opensea/)



# 참고
- [OpenSea API](https://docs.opensea.io/reference/api-overview)
- [OpenSea Testnet(rinkeby) API](https://docs.opensea.io/reference/rinkeby-api-overview)
