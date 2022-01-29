# OpenSea 관련 구현 방법
- OpenSea의 이더리움 메인넷을 사용하면 현금이 지불되므로, 다른 네트워크 사용 
> 예. Polygon, Kalytn 또는 OpenSea 테스트 넷(이더리움 넷은 Rinkeby로 제한되있음) (근데 OpenSea에서 ethereum network API만 지원하는것으로 보임)
- 만약 나중에 web3 API를 다룰 수 있게 된다면 NFT를 ERC20코인 기반으로 거래 할 수 도 있음 (물론 수수료는 ether)

## Java
- [web3j](https://github.com/web3j/web3j)의 API로 ethereum network 접근 가능
- [OpenSea의 Java API](https://docs.opensea.io/reference/api-overview)는 검색이 한계
- 나중에 OpenSea가 사용하는 contract를 분석해서 web3j로 커스텀 contract를 만들어서 다루면 근본적으로 모든 작업 가능 (Java web framework 사용해서 가능)
- 프로그램 관리, 기능 추가 용이 / 버그, 에러에 강함 / 확실함

## Javascript
- [web3.js](https://web3js.readthedocs.io/en/v1.7.0/)의 API로 ethereum network 접근 가능
- OpenSea의 Javascript API는 검색도 되고, [opensea-js](https://github.com/ProjectOpenSea/opensea-js)를 이용하면 OpenSea에서의 대부분 작업(경매, 전달, 민팅, 판매 등)을 API로 가능 (하지만 OpenSea가 사용하는 API(사용하는 contract)에 종속되는 단점)
- 나중에 OpenSea가 사용하는 contract를 분석해서 web3.js로 커스텀 contract를 만들어서 다루면 근본적으로 모든 작업 가능
- 뛰어난 접근성



# NFT 저장 방식
- 만약 OpenSea API를 쓴다면 OpenSea가 관리해 주므로 걱정할 필요 없음
- 만약 자체 마켓 구현시, 생각해볼 수 있는 방법
> NFT등록시 새로운 ERC721 token제작 후 network에 등록 (metadata로 NFT리소스의 hash value 저장)
> NFT저장방식은 중앙서버 or IPFS (NFT식별은 hash valuefh)



# 참고
- [OpenSea Clone Project Blog](https://mybc.tistory.com/99) ([Github](https://github.com/Parkstelth/Project01_Opensea))
- [ERC721](https://eips.ethereum.org/EIPS/eip-721)
- [opensea-js 예제 프로젝트?](https://codesandbox.io/examples/package/opensea-js)