---
description: 에버월렛은 매우 편리한 시드키, 키 및 계정관리 구조를 가지고 있습니다. 이것은 에버월렛 내에서 매우 간단하게 사용 가능합니다.
---

# 아키텍쳐(Architecture)

## [시드키](seed-phrase-management/)

아키텍처의 선두에는 **시드키**가 있습니다. 시드키는 해당 지갑에 담긴 가상자산에 대한 접근을 제공하는 일련의 단어 모음입니다. 지갑을 가상자산의 암호관리자로 생각하고 시드키를 마스터 암호로 생각하시면 이해하기 편합니다. 시드키가 있는 한 지갑을 삭제하거나 행여 분실하더라도 해당 시드키를 입력함으로서 귀하의 자산에 여전히 접근할 수 있습니다.&#x20;

반대로 시드키를 분실하면 토큰에 대한 접근권한을 잃게 되므로 절대 시드키를 분실하지 않도록 주의하십시오.

## [공개키](keys-management/)

공개키는 계정의 저장소입니다. 각 공개키는 [유형별](../getting-started/install-and-singing-in/types-of-wallet.md)로 하나의 계정과 연결될 수 있습니다. 공개키는 [다중서명(멀티시그) 지갑](../multisig/)을 만들 때 필요합니다. [배포](../multisig/creating-a-multisig-account.md) 중 관리인으로 입력되는 주소이기도 하며 거래확인 요청이 그곳으로 전송됩니다.

The public key is the repository of your accounts.\
Each public key can be associated with one account of [each type](../getting-started/install-and-singing-in/types-of-wallet.md).\
The public key is needed when creating a [Multisig wallet](../multisig/) - it is its address that is entered as a custodian during its [deployment ](../multisig/creating-a-multisig-account.md)and a request to confirm the transaction will be sent to it.

## [계정](account-management/)

계정은 아키텍쳐에서 기본이 되는 요소입니다. 계정은 귀하가 자신의 토큰을 [전송(송금)](../manage-assets/sending-and-receiving-tokens.md#sending)하도록 해주며 보관 및 [수신(입금)](../manage-assets/sending-and-receiving-tokens.md#receiving)받을 수 있도록 해줍니다. 귀하가 다른 사람에게 [토큰을 전송](../manage-assets/sending-and-receiving-tokens.md#sending)하거나 [받을 때](../manage-assets/sending-and-receiving-tokens.md#receiving) 사용하는 것이 바로 이 계정주소입니다.&#x20;

