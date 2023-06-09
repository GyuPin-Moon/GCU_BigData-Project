# Twitch 인터넷 방송 플랫폼을 이용한 대회형 마케팅 성과 분석

- 수업 : 빅데이터분석개론 (이영호 교수님, 화 A,B)
- 학과 : 컴퓨터공학과
- 학년 : 4학년
- 학번 : 201735949
- 이름 : 문규빈

# 서론

## 요약

 최근 방송 서비스는 사용자 편의성에 맞춰 개인화되고 있다. 이에 따라 마케팅의 영역 역시 IPTV를 넘어 OTT와 개인 방송의 영역으로 확장되었다. 그 중 개인 방송 플랫폼을 통해 대회를 주최하여 마케팅을 진행하는 전략이 존제한다. 이에 본 보고서에서는 대회형 마케팅의 성과를 분석하기 위해, 2022년 Twitch 개인 방송 플랫폼에서 진행된 대회를 **유입성**과 **잔존성**을 중심으로 데이터 분석하였다. 분석 결과, 대회 진행 기간 마케팅 대상의 뷰어십은 최대 6271% 증가하였지만, 대회 이후 2개월간 데이터가 대회 이전과 비교시 최대 19% 만큼 방송 시간이 감소한 것을 확인할 수 있었다.

## 배경

 최근 방송 서비스가 개인회되면서 개인 방송의 규모가 점차 증가하고 있다. 이에 따라 마케팅의 영역이 방송사에서 개인 방송인으로 확장되고 있다. 개인 방송은 기존 방송과 다르게 _[게임 방송, 메이크업 방송(뷰티), 먹는 방송(먹방), 요리 방송(쿡방)]_ 등 개인이 보여줄 수 있는 콘텐츠를 중심으로 진행된다. 이에 따라 개인 방송의 시청자들은 자신이 관심있는 콘텐츠를 진행하는 방송을 선택하여 시청할 수 있어, 인터넷 방송의 시청자들은 **해당 콘텐츠에 관심을 보이는 시청자**들로 구성되게 된다. 따라서, 국내 게임사는 게임 방송을 대상으로 마케팅을 진행하여 게임에 관심있는 시청자들을 대상으로만 홍보를 진행할 수 있다.
 
### 게임 마케팅

 개인 방송을 대상으로한 게임 마케팅은 크게 두 가지로 볼 수 있다.
 - **개인 방송의 일일 콘텐츠로 광고 대상이 되는 게임을 진행하는 직접적 방법.**
 - **대회 주최 혹은 후원을 통해 광고 대상이 되는 게임을 홍보하는 간접적 방법.**
 
  첫 번째 방식의 경우 절차가 간단하고 비용이 적게 소모되지만, 평소 진행하던 콘텐츠와 다른 콘텐츠를 진행한다는 시청자들의 거부감과 홍보의 규모가 대상 개인 방송으로 국한된다는 단점을 가지고 있다.
  두 번째 방식의 경우 절차가 복잡하고 비용이 크게 소모되지만, 여러 개인 방송인이 복합적으로 상호작용하며 콘텐츠로서 진행하게 되고 사용자들 역시 대회로서 콘텐츠를 받아들이기 때문에 폭넓은 시청자들을 대상으로 문화로서 접근할 수 있다.
  이번 보고서에서는 대회형 마케팅의 실제 성과를 파악하기 위해, 2022년 Twitch에서 진행된 대회를 대상으로 **뷰어십을 통한 유입성 분석**과 **지속되는 방송 수를 통한 잔존성 분석**을 진행한다.

### 2022년 대회형 마케팅

 Twitch는 글로벌 개인 방송 플랫폼으로 [2021년 10월 기준으로 246만8천911명의 MAU](https://www.yna.co.kr/view/AKR20220129048800017)를 기록하여 국내 1위의 점유율을 보이고 있다. 이에 따라 다수의 대회형 마케팅이 Twitch를 대상으로 진행되었다. 2022년에 Twitch에서 FPS 장르 게임을 대상으로 진행된 대회는 다음과 같다.
- **[2022 블리자드 철인 3종 하계 대회](https://news.blizzard.com/ko-kr/blizzard/23813564/2022%EB%85%84-%EB%B8%94%EB%A6%AC%EC%9E%90%EB%93%9C-%E2%80%98%EC%B2%A0%EC%9D%B8-3%EC%A2%85-%EA%B2%BD%EA%B8%B0%E2%80%99-%ED%95%98%EA%B3%84-%EB%8C%80%ED%9A%8C%EA%B0%80-%EC%8B%9C%EC%9E%91%EB%90%A9%EB%8B%88%EB%8B%A4-7-14-7-17)** *(2022.07.05 ~ 2022.07.17)*
- **[2022 자낳대: 서든어택 시즌 2](https://www.enchantenter.team/sajnd1)** *(2022.08.05 ~ 2022.08.14)*
- **[2022 자낳대: 발로란트](https://www.enchantenter.co.kr/content/jndvalorant)** *(2022.09.22 ~ 2022.10.02)*
- **[2022 블리자드 철인 3종 동계 대회](https://news.blizzard.com/ko-kr/blizzard/23882530/2022%EB%85%84-%EB%B8%94%EB%A6%AC%EC%9E%90%EB%93%9C-%E2%80%98%EC%B2%A0%EC%9D%B8-3%EC%A2%85-%EA%B2%BD%EA%B8%B0%E2%80%99-%EB%8F%99%EA%B3%84-%EB%8C%80%ED%9A%8C%EA%B0%80-%EC%8B%9C%EC%9E%91%EB%90%A9%EB%8B%88%EB%8B%A4-12-12-12-15)** *(2022.12.02 ~ 2022.12.15)*

 대회는 **각 게임 개발사가 주최**하고 '인첸트 엔터테인먼트'에서 주관하여 하여 진행되었다. 

 [[그림 1. 2023년 5월 21일 게임 순위]](http://www.gametrics.com/rank/Rank02.aspx)
 
 ![test](https://lh3.googleusercontent.com/fife/APg5EOYm0-jo1zCuxoYvDDP8nQCVCP7bEqecRkD6JP7Q7AMui_1etpUp7n6Uk3nV-dlJ7SbQiC1HeeWbZcDRmd8CvFAh0y1GjlPcOWPEBVn1U6vSI5KXwNVOPvbwXUaLvM957C-r7e4OWMl_l4jrdRX9BHC62AYpX9AV5rHycRUTbHfxnZWCWoG7p6TzHSO7uCKZsjnw18WF-cFSFc3kuaBu6yqSL28flPdx2OXDbbvIWm8CqvSgTHdwIkLivxzgMPmyp0quuxe0Wpvln5UF6_qV2H80jbJyR7uMRzPpe9paN4LdzAzBaZ1Y4zGpdZ5dTsmcwWZhK8_ba_6cwgnDHontphSWJxQvuNG9psvbSgiInGA2Dpkwugimch7JMJx2TgVfFyJcYVuOBx_aT3q3JPEdJdBcnGEFZfnVcrQ6oFEXeDm3Ej8Czm0EMjMUizkXcMJnlBvapoZUiLz-agAlsXibqi8LqPHjvEirk5rJCN9MxZ2E1cfhg0rLDwik7yQIJbr0za1wE97SZ3YDSZc0y-BKPsmHbUUMFIRiljbL3TL4S3TJ8KkZu-L9aRipVBNPEtrNU0efGgBocguWLUOU0nFKQ9D2tYZQFxxMioE6rGN1XUrwQMZ3r7V0YEJeRTciNN02XMcKU_-MYdcYZVaP7VUxAx7ftqdIoEXBvjag68i5UxCbdg4zzAagx04q74xHNJXzYEehoU5_eGpuUtsCUmsMgJm6qy1z7Saa0I2_vrRo-zkHq0Moe9QcrCAgrGoPs-OovqLWcMaYceI7iRZYYXtlzS3b8NHT7zBZQGeXq3AsoEZnpCZrqwMm7G8dggugg8PN9sovcNtfDLll-7ByH3p7kRKpYV6GOHjJOkbyRilEOyJng3FTRdoT6oih_9b4IzR0EP1J8Yy9S508h2TToJhTl7es51YB53qQRqbzBtY0Mg_7VPA01RVGlTwStusDzOMQ7dclKgcrml-KDzFsPzR58n_Y7228UQ72Rv33Y0jOmkRVO2G369V6a4x_A4OhMTJcRjeNdGbIH1QCzjI7U5dL4S9V8TB07sed0hOPoRxGdgO9eE4AILQJxcjPnSs9dQ-UanxAmXJyg3hCD5A8o-TLZZsTwJLB18NJgX6P2XUy1a-6DyA3Kpc3bcNEsILLZAP-BMdoRaV3P5jw848o4cUu6Bn94rkw9NVzVRvZ5rzCfN2SfDukBriRThMyMIPr5weritav11PTV8tH7znG7yk_O-EsWzwTK0NN9aUFIwMACgFQ1XufHt3yIRFfb1OrK7GRSYinq-P_uMe548Yp-T3M86YzqoTBfJ_kdJHBynZos2Xk6k1eqD-2voIbcqYHjVM8CYkW-yCPn3W34QACIWfu71XGIFV67tgkQ8I7j-_VfFhK8Tsncev5zEh1l8FCYqSwk0wWiIkEuMJF_iEr1gQAu6Co7ckluSuUKNV3ZItnD98htaxqrECoAGQZfVJeuqzxfyhq8KpFaDRFBnHEJHIyEblGsQ=w1920-h972)

 해당 대회들로 진행한 게임은 국내 FPS 장르 게임 시장에서 2023년 5월 2일 기준으로 다음과 같은 점유율을 보인다. 그림 1에 따르면 'VALORANT', '서든어택', 'Overwatch' 순으로 사용시간을 점유하고 있는 것을 확인할 수 있다. 따라서 이번 데이터 분석은 대회 진행 전후 3개월의 데이터를 분석하기 위해 **2022년 4월부터 2023년 3월**까지의 데이터를 데이터를 기준으로, **'VALORANT', '서든어택', 'Overwatch'** 를 대상으로 하여 진행한다.

# 본론

## 1. 오픈 데이터 설명

### 데이터 소스

 Twitch는 개발자 친화 정책으로 Twitch Developors 콘솔을 지원한다. 인증 토큰을 발급받은 개발자는 Twitch Developer를 통해 지원되는 API를 사용해 Twitch 데이터에 접근할 수 있다. 이번 분석에서는 제공되는 여러 데이터 중 Game Developer Analytics 데이터를 사용한다. 다음과 같은 과정을 통해 데이터를 수집할 수 있다.
 
#### 1. Twitch Developers 콘솔에 응용 프로그램 등록

Twitch Developers 콘솔에 로그인 한 후, 다음과 같이 응용 프로그램을 등록한다.

![twitch-developer1](https://lh3.googleusercontent.com/fife/APg5EObko_9GS0t-4NqHzu8VAtVlKsJyBk5bU2F_JU_k_xd0FgWQaUTpwjSxCRJ3PatvDPYbOoez3lRIzyU4c-QDABo_-TES5xymfWEtuqgaLgu7qDCGIW_HTcuRRyq0K1kTqgTXT1GC-MTGqWMc1VgNGkRqgHBtU7PrFvIq849hDDBp_Sl9bVz5pHNJ7PoUgqBcxco9ZV-lDiaBitO8WAAwSDqMlzSt4nvlPRGT2mZn9-NR5eyf-MuRZgUGC9TCP2VBKAVFvghWCO-t9VqkwZYuK8B3R0GVQ0LxtNbYazqa5Ys_5zUwTqUi3xSgS3ta4WVC7510e-utEPbrPzf4mKHjqaDF6vgUyFdBij_A1f_LLeiWFD3m7jgWA-jjuKK_-JnZcrNMfYJuua0wKyCIJonhW_njpHgLCN5d8PqNeAQJXLOmOoLCo-f6aU7B2bzWD84008DkZPacw7bZxnjXq4gsqGlcwD83tRLmBfgrwqv4RJ0cBODuYSrRYgbQYZvil9HY1tfnXjEdtu0CTyXuTeVqgu3RJ2-0OF5Y5ZMGeLc4l-qcRzZAhb1bj3GctYVq_M_UKCY1Z1D-X-9Qdv1zMoDOt18VAZhUG4uKYg3OABDQgcvTtWLuEv7DZYP7f619LR0qWgvNjZjfW4n3GuomrSwxFmB38ZuFv17lOJ5r8NbpUSSvyy35K3TxOYKR3osjAIF2uaqMVKTlJbz0ZeMdPMQfvV_2RFjCJW0c80oKLpnpLxyclPXDndV9vGE_2Ra1VSugMxmf9kZu2-PiirxD97W0kJoIk-GLaLG-Q5-Lp4dfRygtrXsmUizLTVM-cBc2YzMU57F2Yt_wzmHtAA7i1-xNEk-I593m1ELQ2_V2hvaKp1klEiYMKw-rY0C-Fw-lY5Kt942VPoOoo-j05kXA5CmWmr8ki-lFTW2VRrLognWKhW8ZLKdI9HClm5X9S9qx1jXforsDbqm51MfFCKiMHcG5c8tNMUZ0BPYYmYSUn5CpxGPG6x_IRZxrCS68HXVoWqLI-KyDaRGg5b9x93pm339iqjNWMHo7vX1augykhyCwiyuesSJNcVdQw2UAHYiQzhN5qczi1boLDI-39R30BPSACSxIThMa_30a2UAvxOmugXWV2D_FlUTwH-W1GFDqzimNu92zSWk_MvKvk42d0gVEW2GKl42nIiEEBwdh06QjV7GpulqWSIZZNKY52Apqaw4MKJyegjiSDcIqBhIhtlZPOQNtrRv7cS-bUdgAKcdqzuoBGYFcH7F-rtsov9thfN9WAZJFdxcAWG27V-Kwf881PLmryHMo0zsBo5ruAjL6muvxw6mGDuIFkDHuOWod0Lx9P1fDPu26JwIaOsffzUtiHGAHvqMjneGy0rleMf8zhbLMsS-2Q198JnyXjmUVVEnn2t4h0AI75tvemdZZDewN9dx0Nn0QkL3iKmJHNFmuqUMXu3alaKisVBAHqREnHDe28p0JIcFqBliCyvBoyKlJGEzfMg=w1920-h886)

등록한 프로그램을 통해 client id와 client secret을 발급받는다.

![twitch-developer2](https://lh3.googleusercontent.com/fife/APg5EOb1R5bcDLdXMBgsRJoZWOipvR1rYHqj22b8PfMg87YHDJBt-kVHMI858MKKeZwf2m_kGpYTdYvwEOqaIhS3bGjXCAZcn04f3ROPUW8NfjjcgYYnLaFDWAa8E4WXtkwx_-WepJp0waRUaPyNG8jr0JvCLUSpdzWkT3EZudsb3MHAUI-SSw6hHrKDCLSgEX6AAEdE-WYoAb6SxaRDdytldAwAtr6YRE4C7lmI12DUtu6bbMIv3vUSHlB70nYPIZHfGqpvIC79w6n61UQqRVBmeGop62QmeBHtd9ykrrxzWwM5MdmeFoitT7kv79l0mDHKDDjbtCYMaqrvJmMzO-3F32xpTrv_D9OeMZi0kdywe102xByWe50GC0__aKjHk8yl-lRczlxeD0o-dDiC2-Ls981nbzO9Jsv9VCX46AbJdJUW7Qv5Dkv-mEQ6RCsuviEb-jqJPj4I29GibmLsesufmlOsTM0IeTC3nRmn-ULFaIM9vpn3DMJa8P6wcRNfwrAnm7GjBAwqdJ_v4ys8OuTXZCodtQDxH0SHv17-sxFB8lW_GisdTeOZP58JFYFdwqZJqlZezs9nfBcUM2GndRc4G4m-WGtiuTT-Ri-VlyMHqt0xPXVK4sE_0-Cx6xstWarkbNTVvVRgjnq61GRK9GNWYB9iQ4i7Eu5N5iaJjNtHodkXaZmJJNX1nXvsA6J_AehX_ap_CxecLzn6C9cafDUZ41-83AOwvFoGl_ZUrOt5X9JENuvAFxKZX7a6cefRZWR3WN-ttDxbmg-X4_HLCrAA643KqID__8doOKrHKExxGjDOmMCG2N5IPBDBxByS2-YuEyZonr9SMzS84xtxb14fPK01448gdyIO9JZ0-2WVnFrd27tHlNRWAKfYfoIej6vqlL8QOrjqnnPTrtHuQn-4xA62UNUjP_47255SDdHLre9lW7htQMcFlQtMQQVfubbVVeNPn1aDK9YGQZszunwvnmBxkAdRURjVSKWvyiWVYKYtevMei2yw3sF8vZdeHTQ0PzjnXoK-2IyWTz_76efCbDuhkmyLI_fpSkkW24-gU-zrYeTh3dfxBLzPr3P-WBMVOJSbA9kcir0jkl--rejW1vXiwsWvM3ibD_buVe6cmv2Z9KGVF9cV8tZsuydjAbudFXCrobh_TaWTd9NmPgiiijJkgBH_ws1lMDJzdHEkUEcel4PQr_G06oy4Y9vW4O5v2VvIHm-jmu2ok4Nd-KXjDun01IPTZMs7wbW9qdlD87MnMoosczw9ad41K3mb2N98IVB_qS0oprTy79P2AFY-RaGPXkkBnvil6EyMDbM-4r54bZfyDciAYooDrv4q2wM20EL2oASJXE1I1i_Lpf6YKtpc1K75Wa0OCOe8K3OYDajGiOc0Cc-qJkMh1088kjcmNJ_nKdQ6EteyM92JqiQaPga1Ey2FWNWQOsF75_DbCZN5-HAEVmrXIbbBv63WYi1z_m9I6tHbx3rzFll933yQimkvgg=w1920-h886)


#### 2. User Access Token 발급

requests 패키지를 통해 API POST 요청을 보낸다.


```python
import requests

client_id = "s5uk18mah8k2wzxbjvrhrwy6j7l6nt"
client_secret = "92okr33mpcbpdrx4y06kyfdxea3zeh"

auth_response = requests.post("https://id.twitch.tv/oauth2/token?client_id=s5uk18mah8k2wzxbjvrhrwy6j7l6nt&client_secret=92okr33mpcbpdrx4y06kyfdxea3zeh&grant_type=client_credentials")
print(auth_response.json())
```

    {'access_token': 'r12b0m7zrnwvmg6rm6uvnfh37tlsd2', 'expires_in': 5523972, 'token_type': 'bearer'}


#### 3. Game Developers Analytics 데이터 요청


```python
client_auth = "rovsoh74e7620ky7j3yzu8ba9gxpdy"

VALORANT_id = "516575"
SuddenAttack_id = "29068"
Overwatch_id = "488552"
Overwatch2_id = "515025"

headers = {
    'Authorization': 'Bearer rovsoh74e7620ky7j3yzu8ba9gxpdy',
    'Client-Id': 's5uk18mah8k2wzxbjvrhrwy6j7l6nt'
}

valorant_response = requests.get('https://api.twitch.tv/helix/analytics/games?game_id=516575&started_at=2022-04-01T00:00:00Z&ended_at=2023-03-31T00:00:00Z', headers=headers)
print(valorant_response.json())

suddenattack_response = requests.get('https://api.twitch.tv/helix/analytics/games?game_id=29068&started_at=2022-04-01T00:00:00Z&ended_at=2023-03-31T00:00:00Z', headers=headers)
print(suddenattack_response.json())

overwatch_response = requests.get('https://api.twitch.tv/helix/analytics/games?game_id=488552&started_at=2022-04-01T00:00:00Z&ended_at=2023-03-31T00:00:00Z', headers=headers)
print(overwatch_response.json())

overwatch2_response = requests.get('https://api.twitch.tv/helix/analytics/games?game_id=515025&started_at=2022-04-01T00:00:00Z&ended_at=2023-03-31T00:00:00Z', headers=headers)
print(overwatch2_response.json())

```

    {'error': 'Unauthorized', 'status': 401, 'message': 'Invalid OAuth token'}
    {'error': 'Unauthorized', 'status': 401, 'message': 'Invalid OAuth token'}
    {'error': 'Unauthorized', 'status': 401, 'message': 'Invalid OAuth token'}
    {'error': 'Unauthorized', 'status': 401, 'message': 'Invalid OAuth token'}


일반적으로 이 방법을 통해 데이터를 수집할 수 있지만, 이는 **게임 개발자 조직으로 등록한 사용자에게만 제공되는 데이터**라 조직에 속하지 않은 학생 입장에서 기간 내에 획득할 수 없었다. 따라서 비공식 웹사이트를 통해 데이터를 수집하는 방법으로 전환하였다.

![twitch-developer3](https://lh3.googleusercontent.com/fife/APg5EOZ-JNwffb0ugw9PYzm2T6Xt0GzfC3bKALfXiKDO7EW2Dr-7R7uRgtH6OaI-ojuJMRfXMPtgNuyWelP1e_idtL9PCFzV1RSH5Si2aGaLZ8zW5d7KwbNRYiX6S2KaBrBmUVftawgalLb_be-Jz9l4aeFbcazfxhkut6V2LKFbQRgUVqpQzakMBfLVOD8VrdbTnFFxTLKv4FPicMmYX1x1pNfgWODX09G5J6xfuEaGukmdCpZ9d7FNUDUSvV6iqOoTDF9WL9CNeZ74_kbVF4LqI3BhNttfcOZRs3NpXyazn2y348ErQvFblDQ9OGN5oVrq0Dh1FrzS6B0e84pUNdtCrnMUw8gjU7ryYPrCFL52eJfuZmEYpwHzJANY6FDuot2TJMdTts56XjjyZ2vpGACorde4M5lISx_gN3-OFpigAtXdao_1LuzDZ-EzkwFaXvWxEU7f56wAQHzqs0p6g78LaKfP_tYM_7L-5Piq1pkPVIj980O7h7zDoTFX6Jbkf72sHl66CXxIx-gvNcXfgdSrcNmf4y7wi1vad3bou-5NryS-SsLBoqX9NbZVHFk3nX54e5n6BxrLlSoO7UetG4aNlqMg6IqT64_OdQPoONBLaV6spx74yvQEzzjg4ENrMsvea9TKOpXoIdgLT-8zq8-yNXY-2OG5vRcoLS_beJFHARjf5c4bj4Ht0w8pA9sCnW7q7q5HFzYi4-Bxs1turH7PgFdDk2YVwJZa1_AKMH1GwsAxB6IAooCJ3IX8lzZp047jpeZhejI8J4yAxhUWW_r8zBvhqPo0PTtZTv34Ku9ccIl6JxHAfbWpXcfdWX3pvUQMgv7Sok79eQ8f5SACGL_MiX3C_6nKeZJO4UdUkLV5TPwtz6LZQDDtGbKi8m1WMFXDYvU-jarJR1VaILYpzvd-1nwfkmFG2NP58-W8eCg4pktAWSfQZnel5eDhy1Mje4zY8OnTULM99M1_zHWMg32la_HLMIf4YNPWwujs-D_yVcbny1ycbtZ50ZrOAW93YZ7LXS-j305d3Tr2AtFea0UZ-4hFOYLUCRNJz3GuZ2AMK5jkfeb-EVx4OvqgH0CrA381GBmbfm9QBxoPoxoU1bnWRlM-0wejWKJL8V7U9ihg0fKeoxgetPQ5Ocd5G3Tc7P3knAQt0H9lvJBfjM2EK6Rz4II5ik5BToZsCJ81xGw_67PUTp8tkAFeKLnpr9RtGFWTIGGDuW0ngy-qARgdyCbOh4JOElBsjobAidhaJdKw-PDxjPGvSpQmxbkPuwCR354Y29eISCpEUDNiZLh0QCFZUn3DXPMNslH9SS_b1qSoyC6Pq6op96Pb_o7TzJtcDBB0LHOL-TKSTZL8SPdLoVT8__JHmyXJpmIP2GGJxTwvRUu8egHfsnpdM7kMfWV699a7XiETi9JTpMt1_uK6tCgccysc9_hFH4dJs7quY-pNK-Uv-nnR9fZhf-tp7isBPTAui2Hff8xQswcKvhq4iSOhN_tE9g=w1920-h886)

#### [4. sullygnome.com](https://sullygnome.com/)

개인이 운영하는 트위치 통계 및 분석 사이트로, Twitch API를 사용하여 5분마다 데이터가 갱신된다. Twitch 공식 지원 웹사이트는 아니지만 이번 분석에 필요한 데이터를 얻기에는 충분하다.

![sullygnome](https://lh3.googleusercontent.com/fife/APg5EOZzllaw4fQJIz9R9te13rdrC1qXlvw-P1osohmaqnyofw3GqNgwEJmVV7VAM4Yx23RW9Popt7z-1iHQ2c75zj1hw1zbAD-ZEaKmeW3dZBzhmJxAqTofyl9mefjTNVZSf36XVjqrEXgRPIYI0BD_b31yuh4hL6cdcvU8oVGYLc-6HSp3n8XJU03U2hnaqPlyKE7yRoNjrcQfDJK81sabmhI-HSHvA8dU8iQcq3vlUyAU7IFf2a6S0qA9Vs56tnZDpcXg972V-XHA2j7lyveaBID6-n8viGvSEIc5arWg-aTOu-kZmnnqEQ6jlBt8gJ4j-NT1UKR6xsQPoVgJkjYFDcAzd41wli9r-fUaobmyu3uwZ_AY4lIbb-paobFTg-nfwMwC7yTneaiArS8i4XDE0akZXywIE_Nlyb58feyFZFDR7u1Wm79bTHTcK1lXy84r3byPsbpdbVqhTJeEXwFlECzGL13iuRcYbsubiZDAro0BOwU5B2NiRMmdVKRabNxinB-cS5Ch1lcRBeTCf3d3OjBXp0p_LV-394ruU92Mc5_wDp_w4d0ZjFpVlSRBrPE-my8JXGrnsYCuHlZcxoWrmNqEzLkldAMjepUdUVZ7BiyNqvtasbcqHsaSSEw8XHUeNq4fYvrZS6dPwM2ugUf1vnMqhRBdXbWvzKsMsJ32pAylAJsZ0JIX8YEMM382ujTHSx5SO5N-OK06sO-YQSZmWVTE0aKyWeoqkJrskcRImYL7mj1KhDCtfbatjL_gnt0oh0aarOUEVtfFkslmUsl7yk5f-zB4V8ZVfEUY6LEz03G2CAq6S-eZTe3cNInmztsit5jtvmvtGPZFenPWO103--Ke5SEIyeAhUccGXi17DzkF1FtVerIQKDs0_26pSkrVJlf2ommNe4qjYcZfZnN4oAzfI2S16qeq46FAuWyQZ5UbID9-ttieScDMZe8LXaPeHN_X1cLHqelqaefFWco9YWp82gn_i4xaCzo9uIdiXcz289aJg4Hi78cA-7whrdgx1Ckan-Pqo8cb2uXkjCiHMQ5GM55h8Wy6pSrPWgdXnGH0fO5-zEz6drzE2-3vqtfqkAXRaWymqcFM_Qqceo0dnZmjEWNwOTqXIm4A6WnWnaOvSQ7LYxw_g4_ou2BuaathJy7uEtchzLeUc_IlYlsGfSrejgv2vIo97N6rwJSwd-9UDSmS9z-RKkxh1t1FPJfc8Zw43g-YIuc0H825IVlijz6scNYGvYFI3vgcKx-mUZUq4vcC4U4f3eTI673jjM2vqlrHpB2Ui2lsvK6qjreEtLA2Ohg_jHiLXEDWKe0S666x13kb7grxBKZJxBfTKgBvJV--qGTNzRp8yJ9CRjmm8dIAdWgHXi0gvoGapkx0Il8nR0sk5-srpflKPgdeTalh3xi_8lRX870AT788c-HkULCQF9-2OCtcvzKAkw5bDD1vShfr2_GeeiVK7EVOL6gZutvI_N0hFMTzOhba46JHrHtCew=w1920-h886)

sullygnome를 통해 분석하고자 하는 **2022년 4월부터 2023년 3월**까지의 **'VALORANT', '서든어택', 'Overwatch'** 의 상위 100개의 개인 방송에 관한 데이터를 '게임명-년도-월' 이름을 가지는 CSV 타입의 파일로 수집할 수 있었다.

### 데이터 준비

디렉터리에서 준비한 CSV 파일들을 읽는다.
게임 기준으로 디렉터리 계층을 구성하였으며, concat 함수를 통해 디렉터리 내 월 단위로 분산된 파일을 병합하였다.


```python
import os
import pandas as pd

os.chdir('/home/moon/bigdata')
main_dir = os.getcwd()
os.chdir(main_dir)

valorant_data_list = os.listdir(main_dir+'/twitch_data/VALORANT')
sudden_data_list = os.listdir(main_dir+'/twitch_data/Sudden_Attack')
overwatch_data_list = os.listdir(main_dir+'/twitch_data/Overwatch')
overwatch2_data_list = os.listdir(main_dir+'/twitch_data/Overwatch2')

os.chdir(main_dir+'/twitch_data/VALORANT')
valorant_data = pd.DataFrame()

for datas in valorant_data_list:
    df = pd.read_csv(datas)
    valorant_data = pd.concat([valorant_data, df])
    
os.chdir(main_dir+'/twitch_data/Sudden_Attack')
sudden_data = pd.DataFrame()

for datas in sudden_data_list:
    df = pd.read_csv(datas)
    sudden_data = pd.concat([sudden_data, df])

os.chdir(main_dir+'/twitch_data/Overwatch')
overwatch_data = pd.DataFrame()

for datas in overwatch_data_list:
    df = pd.read_csv(datas)
    overwatch_data = pd.concat([overwatch_data, df])

os.chdir(main_dir+'/twitch_data/Overwatch2')
overwatch2_data = pd.DataFrame()

for datas in overwatch2_data_list:
    df = pd.read_csv(datas)
    overwatch2_data = pd.concat([overwatch2_data, df])

```

### 데이터 백업

1) #### 병합 데이터 CSV 파일 백업

twitch_raw_data에 일차적으로 병합한 데이터를 저장하여 백업한다. 이후 데이터 처리는 월 단위로 분산된 데이터가 아닌, 병합한 데이터를 기준으로 하여 사용한다.


```python
os.chdir(main_dir+'/twitch_backup_data')

valorant_data.to_csv("valorant_2022-04_2023-03.csv")
sudden_data.to_csv("sudden_2022-04_2023-03.csv")
overwatch_data.to_csv("overwatch_2022-04_2023-03.csv")
overwatch2_data.to_csv("overwatch2_2022-04_2023-03.csv")

print(os.listdir())
```

    ['overwatch2_2022-04_2023-03.csv', 'overwatch_2022-04_2023-03.csv', 'sudden_2022-04_2023-03.csv', 'valorant_2022-04_2023-03.csv']


#### 2) 작업 디렉터리를 git 리포지토리로 등록

버전 관리를 위해 작업 디렉터리를 git으로 관리한다.

![git-repo](https://lh3.googleusercontent.com/fife/APg5EOaEs0BjnNUrH6SPE1KRZYbo3hrtOC1wiUghp2nqoa_XyebWlT7sQuKtFMoMEEZy3TkmRLI_XXs5W32sp-14EyrOceEjuhWK2VJs7wssEfl7SCYp-wi4hsYYj_y_QbcmwfCbCX5hhsz3jlEJUGHQEV1nmfVzTsKHIh_LTPk_cAw2emhuK6k-fKCfbgQU2bl0GIaRxn6Th9A-IZXBnUeiv59n7p7QDT0gRBLNQTFjJNRI0olGtG6nyNcsaN-NuMzOBo0Kn-ZgYSo-T4oSAQjbS1zLbc_oPPqckpNQM49bLFi2fSdw5chplFh6n_jTR74L7lfa7sj55LKTVdcjs28zZwXMedDdX-jyfoOHCylbPkDUUqrcKZdu4nAz41_-OWcNMVO1lNqm-8eAzetM0Q2_nUR3bJK9LY6rXXSqH3M2XVVW7zM5I-QxwGAnrY6bPyhJkaRpLGXwXKelRkCWgE_fJlMRn1zXdUvtzrJuG9cuVmsaOxW43WXpGWbTT_Aafu2rVjWqRIBXmCqVT8KHLk0GjjSsQ6tdEeEfjDacV-I4p6bV7RPPc1rGEMt3r7wMmA5X977ohWd3I-pleNrfZXyvCp8IHd0AfMgMJL9q4ToB-7lRuMq4bRnrYhz3xSCH3helOoFKKTab44BHCk0w6bZFNa0TaSnoxDcPao2uJcXXGRb1pcH80s-1i2wbreFMslhM4BsJzcG3IrDp9mZ7TZHgVd8OZJNEckdVNa1O8L4wMd3p2Yr2j9kvslQ1Kdk3-gTwvd7hRlpFCZ5_gYThDPoTpavAhcx9unr4ce6-0ruEgSkoamgL8OM5dmgk3O0t4yTj1ZKF-Pg8OLLXCtOjzszZDlMdJ0qBui-Dhrgmzx9HCe8Myun80-eSNY9JZadIx37Dz41nIoLSLUFfe5o811ltHkD0JiWNXbdm8GUVU3ZKlCC7wCcDw5n3qOMRt7eXwEgKobvdQqGszX3MeWcnuM1ytXP4-PTOa17jxtSpVDQDd8-sVnk6D17fAVZdYTWifjLEWqpicS67VtzVL69L-HEIeA7M-Dqq-PNWZmJtTeE-YnmiP_xGt_uoNZAwBGSIn22J1f5tyGvMrJoRSiK9GKg7imb74vsWBjf8wBTn2XyMHQ_HrfLPRavI3oDN0OdjLtmID5EUlS44Mt_aKcCwB0N07z7C6QIrwjtfunuSLel0eMQDfT7luBQA-y2NEjb6HzlAksGzeFR_PYc4Yds2CsdMGMjoNejbP762jYjF8RPyT5I088AHkfT8ni0voz3tL3LPWhCPLRzlYHmZIXMawuCHBeO9tM7Pxnb6Hd47jcunRP9QelDg_iDanusdI9xKOHcLc0_ggH07avez_gl7oJ7f5WFSicHsKcvAum-PaMgODYbR9A8bX78Kbf2NvW45U66JQR8aap1nOM-11iTMXRbbnyCyU8U3ttQGwkdenL10cZcQzQrpRsJyaAYmL8Ee-MUcAs_enn6veFUOpr7VDCo5CX6Y0g=w1920-h886)

![git-commit1](https://lh3.googleusercontent.com/fife/APg5EOaQTjyNgQawML6tQkmzwON_8UkjBRAQIZfyrwO3-YSO5ndNfjT46-nfnilOLsECV3g7rouY9tnWBg9HdWV4jvFCXE5g7BmWsX6B8aWMLpbE9knKMKaffujUGiI5HW9bAgqwUvfxcvE2jjR6fErmTcxacfH4xLjyoIZxsMtDcqvkeW3wf0o0Tkef3xf9QhTiXSQiuexl2mjdnYr1z-WE1diqsjeLvOcbGYekrs9Tc_-SkfvTdp0nNfZgRXIoudLOuUXYFhEZB21uqdbolV52WUKgC_dyXkvoaCQqlX5jyhYzDqYMbgby08hWVavZAV-hgMx-8nxeBnrDH2CCNU1cOSMz11ou3bD-9V1UMGPcBd7nJbxx17T18a3yXrFP6I8aRdqelQvaFWjdG2dWyvjK7pDjcXEuM1L6N4Mjolf7kZD6XbpP-zxCTaHR_99avWbLU9jgq45QkJ_bjM-hNR8opu0tZlvAPFmvMP1Gb3KQqtDTI1xP0tUaX801PGJbjjY7_KAzIIsqDkA0hn3sTYQvrG_v-fYUqzZKRR52UBtKoBmdIoNYMY6wN0siG1ssZZqlfdfFfAZXpEVAzFG2uX7GKLFKL65FqSqnO6koK3yqx1Tx5wq4vP_j41FzFyunNw_-EG1744t0IWP1GHF6u4_N_TWEOvEMILFj-GWuJEk-Tb5ywMCaaatFxLKzdcdXM_GLFXljgOp0I2on1B-NSRyri8P9gNzApCWZbqB-ktQE5dYGV6VyMDFXiemNmIzjWg2iU2epwoDMhe17cYAutiffcNDX3PR8Kn0myyK_1fRzTMe2OqmpEfogK19dsmApxYNo6-dhzGIQ4m3ke5BYivrPFcoDjPs1lIAl4XXI0oWOIb1ZjXwl6cJiiI3qBh_UDR0_mVyzU4ewHbhTGSd_7hznVXz4mHYhmQ1dTK6uyu-6zFxIWBBvZzMN_tfMY-p7DeO-W9BqdbEYHgJFBPRjL1KidcITiyq8xRxAoGH7Qbd8r6AkavS-fOV67bOYlnfq8PiMEkd5Ov3KQrcVFK_Di5L8g0iIBrLuoq4i-LGnfDQuBv-4DcSPIbTAdq6JPp-VhLEOrEdPgpV27YH3gBdOPdmWiAeEsu7e0RREJ_RZLGhf7IoAqJQhzMiHGitcs3SZx2L6t-xnx3D9QD9aBkBRY7ncIp-NjLGYIXkLCj73PoLgjkda9NF1dw5TtKePORKQUL3sPvGFYUu6j7PHVnTVAiuTKuQw_26i7pEwB_TMJkNZieuK1Lyfqf0JnTaZXn51YrmCvKVY6QKAh-TUG-xi22M8m2qKDMFxDMNNi3pFcuUgfNj9IaaOwj41V7fHYxi1vmvxjseYQa-DfaAICSDOnvVJyRFaXqT4Rv_dJZswCfBODMoUF-J2rFk-460O2hSRlyy3WVmwNXpkDATLiPmZeHyuMAnmIevgT7VYqAfOJJpEDg6WJE4PXjJu_CxmfM2QMd6xqcDWARU80xgrcQ2prX183linFw=w1920-h886)

_상단 이미지는 초기 작업 버전 당시의 이미지임으로 보고서와 명칭이나 내용이 다를 수 있다._

## 2. 데이터 보기

### 데이터 필드

우선 데이터 필드 정보를 알아보기 위해 info() 함수를 사용해보면 아래와 같은 정보를 알 수 있다.


```python
print(valorant_data.info())
```

    <class 'pandas.core.frame.DataFrame'>
    Int64Index: 1200 entries, 0 to 99
    Data columns (total 7 columns):
     #   Column              Non-Null Count  Dtype    
    ---  ------              --------------  -----    
     0   Watch time (mins)   1200 non-null   int64    
     1   Stream time (mins)  1200 non-null   int64    
     2   Peak viewers        1200 non-null   int64    
     3   Average viewers     1200 non-null   int64    
     4   Followers           1200 non-null   int64    
     5   Game                1200 non-null   object   
     6   Date                1200 non-null   period[M]
    dtypes: int64(5), object(1), period[M](1)
    memory usage: 75.0+ KB
    None


즉, CSV 파일에서 인덱스 역할을 하는 0번 컬럼을 제외한 컬럼은 다음과 같다.
1. Logo : 개인 방송의 로고의 주소다.
2. Channel : 개인 방송 채널명이다.
3. Watch time (mins) : 총 시청 시간으로, 한 달간 해당 게임으로 진행한 개인 방송에 대한 모든 시청자들의 시청 시간의 합이다.
4. Stream time (mins) : 총 방송 시간으로, 한 달간 해당 게임으로 진행한 개인 방송에 대한 모든 방송 시간의 합이다.
5. Peak viewers : 최대 시청자 수로, 한 달간 해당 게임으로 진행한 개인 방송의 모든 시청자 수 중 최대값이다.
6. Average viewers : 평균 시청자 수로, 한 달간 해당 게임으로 진행한 개인 방송의 모든 시청자 수의 평균이다.
7. Followers : 팔로우 수로, 해당 개인 방송을 진행하는 방송인을 팔로우 해둔 모든 사용자 수의 합이다.
8. Partnered : Twitch 파트너 여부를 bool 타입으로 나타낸다.
9. Mature : 성인 방송 설정 여부를 bool 타입으로 나타낸다.
10. Language : 사용 언어다. 데이터를 수집할 때 Korean 데이터만 수집하도록 설정하였다.

### 데이터 재구조화

데이터 분석을 위해 사용할 데이터만 남기고, 필요한 데이터는 추가하는 형태로 데이터를 재구조화시킨다.

#### 1) 데이터 조작

어느 기간의 어떤 게임을 나타내는지에 대한 ('Game', 'Date') 컬럼이 추가로 필요하며, ('Logo', 'Channel', 'Partnered', 'Mauture', 'Language') 데이터는 필요하지 않다.


```python
# Remove Columns

valorant_data = valorant_data[['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers']]
sudden_data = sudden_data[['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers']]
overwatch_data = overwatch_data[['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers']]
overwatch2_data = overwatch2_data[['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers']]

valorant_data.head(5)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Watch time (mins)</th>
      <th>Stream time (mins)</th>
      <th>Peak viewers</th>
      <th>Average viewers</th>
      <th>Followers</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>8397960</td>
      <td>600</td>
      <td>20792</td>
      <td>13997</td>
      <td>833289</td>
    </tr>
    <tr>
      <th>1</th>
      <td>3403695</td>
      <td>1155</td>
      <td>17294</td>
      <td>2947</td>
      <td>182596</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2950830</td>
      <td>585</td>
      <td>9459</td>
      <td>5044</td>
      <td>128763</td>
    </tr>
    <tr>
      <th>3</th>
      <td>15646065</td>
      <td>4905</td>
      <td>8548</td>
      <td>3190</td>
      <td>72451</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2990625</td>
      <td>585</td>
      <td>8325</td>
      <td>5112</td>
      <td>130369</td>
    </tr>
  </tbody>
</table>
</div>




```python
# Add new Columns

valorant_data['Game'] = "VALORANT"
sudden_data['Game'] = "Sudden Attack"
overwatch_data['Game'] = "Overwatch"
overwatch2_data['Game'] = "Overwatch2"

# SettingWithCopyWarning but OK
time_table = pd.date_range(start='2022-04-01', end=None, periods=12, freq='MS')
valorant_data['Date'] = time_table[0]
for i in range(1,12):
    valorant_data['Date'][i*100:(i+1)*100] = time_table[i]
    
sudden_data['Date'] = time_table[0]
for i in range(1,12):
    sudden_data['Date'][i*100:(i+1)*100] = time_table[i]
    
overwatch_data['Date'] = time_table[0]
for i in range(1,12):
    overwatch_data['Date'][i*100:(i+1)*100] = time_table[i]
    
overwatch2_data['Date'] = time_table[0]
for i in range(1,12):
    overwatch2_data['Date'][i*100:(i+1)*100] = time_table[i]
```

    /tmp/ipykernel_397/2818933428.py:12: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame
    
    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      valorant_data['Date'][i*100:(i+1)*100] = time_table[i]
    /tmp/ipykernel_397/2818933428.py:16: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame
    
    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      sudden_data['Date'][i*100:(i+1)*100] = time_table[i]
    /tmp/ipykernel_397/2818933428.py:20: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame
    
    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      overwatch_data['Date'][i*100:(i+1)*100] = time_table[i]
    /tmp/ipykernel_397/2818933428.py:24: SettingWithCopyWarning: 
    A value is trying to be set on a copy of a slice from a DataFrame
    
    See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
      overwatch2_data['Date'][i*100:(i+1)*100] = time_table[i]


#### 2) 병합과 연결

게임별로 분산되어 있는 데이터프레임을 하나의 데이터프레임으로 연결한다.


```python
fps_data = pd.DataFrame()
fps_data = pd.concat([fps_data, valorant_data, sudden_data, overwatch_data, overwatch2_data])

fps_data.info()
```

    <class 'pandas.core.frame.DataFrame'>
    Int64Index: 4800 entries, 0 to 99
    Data columns (total 7 columns):
     #   Column              Non-Null Count  Dtype         
    ---  ------              --------------  -----         
     0   Watch time (mins)   4224 non-null   float64       
     1   Stream time (mins)  4224 non-null   float64       
     2   Peak viewers        4224 non-null   float64       
     3   Average viewers     4224 non-null   float64       
     4   Followers           4224 non-null   float64       
     5   Game                4800 non-null   object        
     6   Date                4800 non-null   datetime64[ns]
    dtypes: datetime64[ns](1), float64(5), object(1)
    memory usage: 300.0+ KB


#### 3) 인덱스 설정

reset_index() 함수를 통해 연결한 데이터의 인덱스를 새로 설정하였다.


```python
fps_data.reset_index(drop=True, inplace=True)
fps_data
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Watch time (mins)</th>
      <th>Stream time (mins)</th>
      <th>Peak viewers</th>
      <th>Average viewers</th>
      <th>Followers</th>
      <th>Game</th>
      <th>Date</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>8397960.0</td>
      <td>600.0</td>
      <td>20792.0</td>
      <td>13997.0</td>
      <td>833289.0</td>
      <td>VALORANT</td>
      <td>2022-04-01</td>
    </tr>
    <tr>
      <th>1</th>
      <td>3403695.0</td>
      <td>1155.0</td>
      <td>17294.0</td>
      <td>2947.0</td>
      <td>182596.0</td>
      <td>VALORANT</td>
      <td>2022-04-01</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2950830.0</td>
      <td>585.0</td>
      <td>9459.0</td>
      <td>5044.0</td>
      <td>128763.0</td>
      <td>VALORANT</td>
      <td>2022-04-01</td>
    </tr>
    <tr>
      <th>3</th>
      <td>15646065.0</td>
      <td>4905.0</td>
      <td>8548.0</td>
      <td>3190.0</td>
      <td>72451.0</td>
      <td>VALORANT</td>
      <td>2022-04-01</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2990625.0</td>
      <td>585.0</td>
      <td>8325.0</td>
      <td>5112.0</td>
      <td>130369.0</td>
      <td>VALORANT</td>
      <td>2022-04-01</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>4795</th>
      <td>23775.0</td>
      <td>360.0</td>
      <td>130.0</td>
      <td>66.0</td>
      <td>617.0</td>
      <td>Overwatch2</td>
      <td>2023-03-01</td>
    </tr>
    <tr>
      <th>4796</th>
      <td>3825.0</td>
      <td>30.0</td>
      <td>128.0</td>
      <td>128.0</td>
      <td>26774.0</td>
      <td>Overwatch2</td>
      <td>2023-03-01</td>
    </tr>
    <tr>
      <th>4797</th>
      <td>71295.0</td>
      <td>1275.0</td>
      <td>126.0</td>
      <td>56.0</td>
      <td>3642.0</td>
      <td>Overwatch2</td>
      <td>2023-03-01</td>
    </tr>
    <tr>
      <th>4798</th>
      <td>234465.0</td>
      <td>6180.0</td>
      <td>126.0</td>
      <td>38.0</td>
      <td>1667.0</td>
      <td>Overwatch2</td>
      <td>2023-03-01</td>
    </tr>
    <tr>
      <th>4799</th>
      <td>70095.0</td>
      <td>960.0</td>
      <td>124.0</td>
      <td>73.0</td>
      <td>2354.0</td>
      <td>Overwatch2</td>
      <td>2023-03-01</td>
    </tr>
  </tbody>
</table>
<p>4800 rows × 7 columns</p>
</div>



### 데이터 백업 2

연결하여 새로 만들어진 데이터프레임을 백업해준다.


```python
os.chdir(main_dir+'/twitch_backup_data')

fps_data.to_csv("fps_data_2022-04_2023-03.csv")
print(os.listdir())
```

    ['fps_data_2022-04_2023-03.csv', 'overwatch2_2022-04_2023-03.csv', 'overwatch_2022-04_2023-03.csv', 'sudden_2022-04_2023-03.csv', 'valorant_2022-04_2023-03.csv']


## 3. 데이터 클린징


### 결측값

#### 1) 결측값 확인하기

isna() 함수와 sum() 함수를 통해 결측값의 개수를 파악할 수 있다.


```python
print(fps_data.isna().sum())
```

    Watch time (mins)     576
    Stream time (mins)    576
    Peak viewers          576
    Average viewers       576
    Followers             576
    Game                    0
    Date                    0
    dtype: int64


#### 2) 결측값 처리

이 결측값들은 데이터 수집 과정에서 각 월별 상위 100개의 데이터를 가져오는 과정에서, 100개보다 부족한 경우 발생한다.
따라서 아예 존제하지 않는 데이터이기에 결측값 처리를 제거를 통해 진행한다.


```python
fps_data = fps_data.dropna()
```

#### 3) 결측값 처리 확인

제거 처리가 제대로 되었는지 확인한다.


```python
print(fps_data.isna().sum())
```

    Watch time (mins)     0
    Stream time (mins)    0
    Peak viewers          0
    Average viewers       0
    Followers             0
    Game                  0
    Date                  0
    dtype: int64


#### 4. 인덱스 초기화

제거로 인해 인덱스가 틀어졌음으로, 초기화 후 새로 부여해준다.


```python
print(fps_data.shape)
fps_data.reset_index(drop=True, inplace=True)
```

    (4224, 7)


### 이상값

#### 1) 논리적 이상값 확인 - Overwatch

 수집 대상이 되는 게임 중 Overwatch와 Overwatch2에는 특이 사항이 있다. 먼저 Overwatch는 게임 서비스가 2022년 10월 4일 종료되었다. 즉 2022년 10월부터 2023년 03월까지의 데이터는 기입 오류로 발생한 이상값이다. 단, 이 데이터에서는 10월달 전체의 데이터 기준이라 2022년 10월 4일에 서비스가 종료되었지만 2022년 10월 01일부터의 모든 데이터를 처리 대상으로 한다.


```python
service_end = pd.to_datetime('2022-10-01')

fps_data[(fps_data['Date']>=service_end) & (fps_data['Game']=="Overwatch")]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Watch time (mins)</th>
      <th>Stream time (mins)</th>
      <th>Peak viewers</th>
      <th>Average viewers</th>
      <th>Followers</th>
      <th>Game</th>
      <th>Date</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2996</th>
      <td>8355.0</td>
      <td>90.0</td>
      <td>106.0</td>
      <td>93.0</td>
      <td>5578.0</td>
      <td>Overwatch</td>
      <td>2022-10-01</td>
    </tr>
    <tr>
      <th>2997</th>
      <td>2250.0</td>
      <td>45.0</td>
      <td>76.0</td>
      <td>50.0</td>
      <td>4332.0</td>
      <td>Overwatch</td>
      <td>2022-10-01</td>
    </tr>
    <tr>
      <th>2998</th>
      <td>1035.0</td>
      <td>15.0</td>
      <td>69.0</td>
      <td>69.0</td>
      <td>1555.0</td>
      <td>Overwatch</td>
      <td>2022-10-01</td>
    </tr>
    <tr>
      <th>2999</th>
      <td>795.0</td>
      <td>15.0</td>
      <td>53.0</td>
      <td>53.0</td>
      <td>9524.0</td>
      <td>Overwatch</td>
      <td>2022-10-01</td>
    </tr>
    <tr>
      <th>3000</th>
      <td>9150.0</td>
      <td>255.0</td>
      <td>46.0</td>
      <td>36.0</td>
      <td>841.0</td>
      <td>Overwatch</td>
      <td>2022-10-01</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>3110</th>
      <td>3045.0</td>
      <td>1575.0</td>
      <td>5.0</td>
      <td>2.0</td>
      <td>393.0</td>
      <td>Overwatch</td>
      <td>2023-03-01</td>
    </tr>
    <tr>
      <th>3111</th>
      <td>75.0</td>
      <td>15.0</td>
      <td>5.0</td>
      <td>5.0</td>
      <td>629.0</td>
      <td>Overwatch</td>
      <td>2023-03-01</td>
    </tr>
    <tr>
      <th>3112</th>
      <td>315.0</td>
      <td>180.0</td>
      <td>3.0</td>
      <td>2.0</td>
      <td>40.0</td>
      <td>Overwatch</td>
      <td>2023-03-01</td>
    </tr>
    <tr>
      <th>3113</th>
      <td>45.0</td>
      <td>15.0</td>
      <td>3.0</td>
      <td>3.0</td>
      <td>5447.0</td>
      <td>Overwatch</td>
      <td>2023-03-01</td>
    </tr>
    <tr>
      <th>3114</th>
      <td>45.0</td>
      <td>30.0</td>
      <td>2.0</td>
      <td>2.0</td>
      <td>51.0</td>
      <td>Overwatch</td>
      <td>2023-03-01</td>
    </tr>
  </tbody>
</table>
<p>119 rows × 7 columns</p>
</div>



총 119개의 데이터가 있는 것을 확인할 수 있다.

#### 2) 논리적 이상값 처리 - Overwatch

이 기입 오류는 Overwatch2 게임을 진행한 방송이지만, Overwatch 게임을 진행했다고 개인 방송인이 잘못 기입한 것에 기인한다. 따라서 해당 데이터들은 Overwatch2 게임에 관한 데이터라 볼 수 있다. 이를 기반으로 이상값 처리를 컬럼값을 바꾸는 것을 통해 처리한다.


```python
fps_data.loc[(fps_data['Date']>=service_end) & (fps_data['Game']=="Overwatch"), 'Game'] = "Overwatch2"
```

#### 3) 논리적 이상값 처리 확인 - Overwatch

처리가 제대로 되었는지 확인한다.


```python
fps_data[(fps_data['Date']>=service_end) & (fps_data['Game']=="Overwatch")]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Watch time (mins)</th>
      <th>Stream time (mins)</th>
      <th>Peak viewers</th>
      <th>Average viewers</th>
      <th>Followers</th>
      <th>Game</th>
      <th>Date</th>
    </tr>
  </thead>
  <tbody>
  </tbody>
</table>
</div>



#### 4) 논리적 이상값 확인 - Overwatch2

Overwatch2는 특이하게 2022년 10월 5일, 즉 Overwatch가 서비스 종료한 바로 다음 날 부터 얼리 액세스를 통한 출시를 하였다. 이 전에는 클로즈 베타 테스트를 통해 플레이할 수 있었는데, 1차 클로즈 베타 서비스는 2022년 4월 27일부터 2022년 5월 18일까지 진행되었고, 2차 클로즈 베타 서비스는 2022년 06월 29일부터 2022년 07월 30일까지 진행되었다. 따라서 2022년 8월과 9월에 해당하는 데이터는 개인 방송인이 잘못 기입한 데이터이다.


```python
fps_data[((fps_data['Date']=='2022-08-01') | (fps_data['Date']=='2022-09-01')) & (fps_data['Game']=="Overwatch2")]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Watch time (mins)</th>
      <th>Stream time (mins)</th>
      <th>Peak viewers</th>
      <th>Average viewers</th>
      <th>Followers</th>
      <th>Game</th>
      <th>Date</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>3515</th>
      <td>390.0</td>
      <td>15.0</td>
      <td>26.0</td>
      <td>26.0</td>
      <td>1127.0</td>
      <td>Overwatch2</td>
      <td>2022-08-01</td>
    </tr>
    <tr>
      <th>3516</th>
      <td>705.0</td>
      <td>90.0</td>
      <td>10.0</td>
      <td>8.0</td>
      <td>51.0</td>
      <td>Overwatch2</td>
      <td>2022-08-01</td>
    </tr>
    <tr>
      <th>3517</th>
      <td>270.0</td>
      <td>75.0</td>
      <td>6.0</td>
      <td>4.0</td>
      <td>18.0</td>
      <td>Overwatch2</td>
      <td>2022-08-01</td>
    </tr>
    <tr>
      <th>3518</th>
      <td>135.0</td>
      <td>30.0</td>
      <td>5.0</td>
      <td>5.0</td>
      <td>154.0</td>
      <td>Overwatch2</td>
      <td>2022-08-01</td>
    </tr>
    <tr>
      <th>3519</th>
      <td>75.0</td>
      <td>15.0</td>
      <td>5.0</td>
      <td>5.0</td>
      <td>297.0</td>
      <td>Overwatch2</td>
      <td>2022-08-01</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>3619</th>
      <td>4980.0</td>
      <td>255.0</td>
      <td>29.0</td>
      <td>20.0</td>
      <td>968.0</td>
      <td>Overwatch2</td>
      <td>2022-09-01</td>
    </tr>
    <tr>
      <th>3620</th>
      <td>4155.0</td>
      <td>180.0</td>
      <td>29.0</td>
      <td>23.0</td>
      <td>1439.0</td>
      <td>Overwatch2</td>
      <td>2022-09-01</td>
    </tr>
    <tr>
      <th>3621</th>
      <td>2865.0</td>
      <td>165.0</td>
      <td>29.0</td>
      <td>17.0</td>
      <td>852.0</td>
      <td>Overwatch2</td>
      <td>2022-09-01</td>
    </tr>
    <tr>
      <th>3622</th>
      <td>1635.0</td>
      <td>75.0</td>
      <td>28.0</td>
      <td>22.0</td>
      <td>5732.0</td>
      <td>Overwatch2</td>
      <td>2022-09-01</td>
    </tr>
    <tr>
      <th>3623</th>
      <td>2100.0</td>
      <td>135.0</td>
      <td>28.0</td>
      <td>16.0</td>
      <td>6648.0</td>
      <td>Overwatch2</td>
      <td>2022-09-01</td>
    </tr>
  </tbody>
</table>
<p>109 rows × 7 columns</p>
</div>



총 109개의 이상값 데이터가 있는 것을 확인할 수 있다.

#### 5) 논리적 이상값 처리 - Overwatch2

마찬가지로, 이 당시 진행한 게임은 Overwatch이지만 Overwatch2로 잘못 기입한 경우임으로 컬럼값 변경을 통해 처리한다.


```python
fps_data.loc[((fps_data['Date']=='2022-08-01') | (fps_data['Date']=='2022-09-01')) & (fps_data['Game']=="Overwatch2"), 'Game'] = "Overwatch"
```

#### 6) 논리적 이상값 처리 확인 - Overwatch2

처리가 제대로 되었는지 확인한다.


```python
fps_data[((fps_data['Date']=='2022-08-01') | (fps_data['Date']=='2022-09-01')) & (fps_data['Game']=="Overwatch2")]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Watch time (mins)</th>
      <th>Stream time (mins)</th>
      <th>Peak viewers</th>
      <th>Average viewers</th>
      <th>Followers</th>
      <th>Game</th>
      <th>Date</th>
    </tr>
  </thead>
  <tbody>
  </tbody>
</table>
</div>



#### 7) 데이터 정렬 후 인덱스 초기화

이상값 처리로 인해 틀어진 데이터를 정렬 후 인덱스 번호를 재지정한다.


```python
fps_data = fps_data.sort_values('Game')
fps_data.reset_index(drop=True, inplace=True)
fps_data
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Watch time (mins)</th>
      <th>Stream time (mins)</th>
      <th>Peak viewers</th>
      <th>Average viewers</th>
      <th>Followers</th>
      <th>Game</th>
      <th>Date</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>8397960.0</td>
      <td>600.0</td>
      <td>20792.0</td>
      <td>13997.0</td>
      <td>833289.0</td>
      <td>VALORANT</td>
      <td>2022-04-01</td>
    </tr>
    <tr>
      <th>1</th>
      <td>3403695.0</td>
      <td>1155.0</td>
      <td>17294.0</td>
      <td>2947.0</td>
      <td>182596.0</td>
      <td>VALORANT</td>
      <td>2022-04-01</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2950830.0</td>
      <td>585.0</td>
      <td>9459.0</td>
      <td>5044.0</td>
      <td>128763.0</td>
      <td>VALORANT</td>
      <td>2022-04-01</td>
    </tr>
    <tr>
      <th>3</th>
      <td>15646065.0</td>
      <td>4905.0</td>
      <td>8548.0</td>
      <td>3190.0</td>
      <td>72451.0</td>
      <td>VALORANT</td>
      <td>2022-04-01</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2990625.0</td>
      <td>585.0</td>
      <td>8325.0</td>
      <td>5112.0</td>
      <td>130369.0</td>
      <td>VALORANT</td>
      <td>2022-04-01</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>4219</th>
      <td>23775.0</td>
      <td>360.0</td>
      <td>130.0</td>
      <td>66.0</td>
      <td>617.0</td>
      <td>Overwatch2</td>
      <td>2023-03-01</td>
    </tr>
    <tr>
      <th>4220</th>
      <td>3825.0</td>
      <td>30.0</td>
      <td>128.0</td>
      <td>128.0</td>
      <td>26774.0</td>
      <td>Overwatch2</td>
      <td>2023-03-01</td>
    </tr>
    <tr>
      <th>4221</th>
      <td>71295.0</td>
      <td>1275.0</td>
      <td>126.0</td>
      <td>56.0</td>
      <td>3642.0</td>
      <td>Overwatch2</td>
      <td>2023-03-01</td>
    </tr>
    <tr>
      <th>4222</th>
      <td>234465.0</td>
      <td>6180.0</td>
      <td>126.0</td>
      <td>38.0</td>
      <td>1667.0</td>
      <td>Overwatch2</td>
      <td>2023-03-01</td>
    </tr>
    <tr>
      <th>4223</th>
      <td>70095.0</td>
      <td>960.0</td>
      <td>124.0</td>
      <td>73.0</td>
      <td>2354.0</td>
      <td>Overwatch2</td>
      <td>2023-03-01</td>
    </tr>
  </tbody>
</table>
<p>4224 rows × 7 columns</p>
</div>



#### 8) BoxPlot을 통한 이상값 확인


```python
import matplotlib.pyplot as plt
import seaborn as sns

sns.boxplot(x="Game", y='Watch time (mins)', data=fps_data)
plt.yscale('log')
```


    
![png](output_55_0.png)
    



```python
sns.boxplot(x="Game", y="Stream time (mins)", data=fps_data)
```




    <AxesSubplot: xlabel='Game', ylabel='Stream time (mins)'>




    
![png](output_56_1.png)
    



```python
sns.boxplot(x="Game", y="Peak viewers", data=fps_data)
```




    <AxesSubplot: xlabel='Game', ylabel='Peak viewers'>




    
![png](output_57_1.png)
    



```python
sns.boxplot(x="Game", y="Average viewers", data=fps_data)
```




    <AxesSubplot: xlabel='Game', ylabel='Average viewers'>




    
![png](output_58_1.png)
    


다음과 같은 박스플롯을 확인할 수 있지만, **Twitch 개인 방송 데이터는 박스 플롯을 활용하여 이상값을 판단하기 부적절하다.** 개인 방송은 소수의 방송이 다수의 시청자들을 이끌고, 그 외 다수의 방송은 소수의 시청자들만 이끌기 때문에, 평균과 사분위수를 나타내는 박스 자체가 낮게 나타나게 된다. 고로 클러스터링 되어 있지 않은 소수의 데이터만 실제로 이상값인지 확인하는 절차를 걸쳤다.

유의깊게 살펴본 데이터로는 Stream time (mins)가 있다. 이는 해당 게임을 진행한 방송 시간을 의미하는데, 방송을 켜놓기만 한 경우나 자면서 틀어놓는 경우가 있어 이를 검증할 필요가 있었다. 놀랍게도 실제로 한달 동안 25035분간의 게임 방송을 진행한 것을 확인할 수 있었다. 따라서 수치적 이상값은 존제하지 않았다.

### 중복값

duplicated() 함수를 통해 중복값이 있는지 파악한다.


```python
fps_data.duplicated().sum()
```




    0



중복값은 존제하지 않는다.

### 클린징 완료된 데이터 백업

클린징이 완료된 데이터프레임 역시 백업을 진행한다.


```python
fps_data.to_csv("fps_data_clean_2022-04_2023-03.csv")
print(os.listdir())
```

    ['fps_data_2022-04_2023-03.csv', 'fps_data_clean_2022-04_2023-03.csv', 'overwatch2_2022-04_2023-03.csv', 'overwatch_2022-04_2023-03.csv', 'sudden_2022-04_2023-03.csv', 'valorant_2022-04_2023-03.csv']


연결한 데이터 및 클린징을 진행한 데이터에 대한 commit을 진행하여 데이터에 대한 스냅샷을 남겨둔다.

![commit3](https://lh3.googleusercontent.com/fife/APg5EOYOk0Say__AI0O3dtS1e0fgfLZhRgxEZNLgiffp4U4ZNlHzek3S6O75JJeZjN_VQVXn14FT90mA5YH63k_d3ZU10qi2JjqXMIOCOPDS7mEIKE5sQX7hAZJzjxYtq_WtQWl_N9pvohnzsofScM9nb3YMIbKdfK-rtVe2cONMTErQwt-2MHWBTPxDJWQOPXctNr5plBS-z73lxYrZigvyEFAgeINWAZqFSxERzDjwEMfJsaYguuLB-RXx593g_FjF6HdMbZkceAr4z8wmayUr061Ynlo_B3wS02Ka7dV945b8QAHEo8daxL5UTzStjzs10_yxQFzNH04j9phrsC3l-foga5cy1QSTAn3R3ECTKioUUhejPpHB6_N_r1b8ebDLcOojfsUMDJO180g-3cI9s89L-ioD4zo0d00G-_oGZu0XqL38n1sroEXApKj2rfKsIatl-_AxkHlzytzVUKKhV3sOeSWNNF16fpnbWo5kp8sJMofamHGhFQuU0ZPzRW9bXvCt-A0B8Zr6Mv2ObZv7CTOgM3MkAx5agEZ8TIJ6xaYlg9J3H9fEBkxIOjGFX2loxPHDf396mOO6YVpyqKJOxNbIVA93ptBv9NjGosTh-CSS4xlQ-DcQ7yZS9BqpmFI8nYGlyEmTMs5v3G-FhqrE_95DXmIJwGEVUiRZu1U4cypDhaDN--ccSwAYW5UCADDKFJvU7ryhk_7f2oDChQaWAz4v4g7IkFvpwFqJTT3NvT40ybe_2Kk5DSwPSWKnYDnR3HTrek7TJvXD3VorXUzzIh9qCSJoRgswCPUl6YA775mpxiqRXWEGtmpOtQ5YLsB0pcKCwu7rP0EdNKKh_zPXJB9O5vWxdK6GxTaKezcze-z_tnp3-dDvFnjHeABzTKCljOJ6TNHtWHr6RssygNMboRSZrLl1F1dULtWauiVPoe7-6nOBH1iCtBMBzM3uIHAI8nNbM149PskrX0iDIqsB6weVm7BHTg_5keSu8tRk5EDuNPZLE9JAghn05Gh3gTFOGf4gXkUTa54o8QP7fHJ01AoKMuBMzp0CwgkX6bn6oOf4EGchVV_Rl4k_4FRS4hWBXtStx9Oo5ScSufJTWQjex8zbJ7wn8gwZ9ZCEL6QlfG-EGVRG4ryRV6h98-oM3JXB9zQtkrQw4ZRBv-F6ioI7QBPGtxjbmBkWiP2ONQaEBohfcImIi89naobkgdxU3u7IRB7sLk8p_7jTJsf8Shk9FEwP6ejWCM8XEP85ePuw2RGaFXpp5HIgfvAjrooPubrSyWeWguVadur17vyTrVBmyudBXkzEa9SNyhN1EKQGKL4IloW2puTKQb0d3CfHMPNGC2JGp07_7cj7yBxPeVPZijX92-PM5j75aK8Id4hbl1EvU17jbk0SQIPl3XC90TLylp0KhSrsvK8KsWHApgLcnbIlZhl21-kWCHwUqBx0wtdQLFHXj0YvgLns_pxs0E0uOh9EBEi8y_fto3RwBeqNyWHwSA=w1920-h886)

## 데이터 분석 : 유입성

**게임 마케팅의 핵심은 최대한 많은 사람에게 광고를 노출시켜 유입을 늘리는 것이다. 따라서 방송의 뷰어십을 분석하여 얼마나 광고가 많은 사람에게 노출되었는지 알아보고자 한다.**

### 4. 데이터 탐색

#### 1) Overwatch와 Overwatch2 데이터 통합

Overwatch 서비스 종료 직후 Overwatch2가 시작된 것이며 이용자 풀도 계승되었기에, 두 데이터를 통합하여 한 그룹으로서 바라볼 수 있다.


```python
import os
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

fps_clean_data = pd.read_csv('/home/moon/bigdata/twitch_backup_data/fps_data_clean_2022-04_2023-03.csv')
fps_clean_data.loc[fps_clean_data['Game']=="Overwatch2", 'Game'] = "Overwatch"
```

#### 2) 통합된 데이터로부터 월별 상위 100개 데이터만 남기기

이상값 처리 및 데이터 통합에 따라 게임별 데이터 수가 불균형해졌다. Overwatch를 Game 값으로 가지는 데이터에 대해 Watch time (mins) 순으로 정렬해 월별 상위 100개의 데이터만 남기는 것으로 신뢰성을 보장해준다.


```python
fps_clean_data = fps_clean_data.sort_values(by=['Game', 'Date', 'Watch time (mins)'], ascending=[False, True, False]).groupby(['Game','Date']).head(100)

print(len(fps_clean_data.loc[(fps_clean_data['Date'] == '2022-04-01') & (fps_clean_data['Game'] == "Overwatch")]))
fps_clean_data.shape
```

    100





    (3596, 8)



데이터가 3600개가 아니라 3596개인 이유는, Sudden Attack의 데이터 중 월별 데이터 개수가 100개가 아닌 96개인 데이터가 있기 때문에, 결측값 처리 과정에서 발생하였다.

#### 3) 'Game'과 'Date' 그룹으로 묶기

게임별, 월별 데이터가 필요함으로 'Game'과 'Date'를 기준으로 묶는다.


```python
fps_gd_group = fps_clean_data.groupby(['Game', 'Date'])
```

#### 4) 시청 시간, 방송 시간, 팔로워 수에 대한 합계 정보

시청 시간의 합을 통해 게임별 월별 총 시청 시간을 알 수 있다. 방송 시간과 팔로워 수에 관해서도 마찬가지로 진행한다.


```python
fps_gd_max_group = fps_gd_group[['Watch time (mins)', 'Stream time (mins)', 'Followers']].sum()
fps_gd_max_group
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th></th>
      <th>Watch time (mins)</th>
      <th>Stream time (mins)</th>
      <th>Followers</th>
    </tr>
    <tr>
      <th>Game</th>
      <th>Date</th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th rowspan="12" valign="top">Overwatch</th>
      <th>2022-04-01</th>
      <td>106321980.0</td>
      <td>242580.0</td>
      <td>15781426.0</td>
    </tr>
    <tr>
      <th>2022-05-01</th>
      <td>40445025.0</td>
      <td>302055.0</td>
      <td>6839828.0</td>
    </tr>
    <tr>
      <th>2022-06-01</th>
      <td>41010240.0</td>
      <td>270090.0</td>
      <td>4933096.0</td>
    </tr>
    <tr>
      <th>2022-07-01</th>
      <td>118954095.0</td>
      <td>266955.0</td>
      <td>10453041.0</td>
    </tr>
    <tr>
      <th>2022-08-01</th>
      <td>33854580.0</td>
      <td>245685.0</td>
      <td>6679357.0</td>
    </tr>
    <tr>
      <th>2022-09-01</th>
      <td>26425125.0</td>
      <td>219975.0</td>
      <td>3834804.0</td>
    </tr>
    <tr>
      <th>2022-10-01</th>
      <td>349336965.0</td>
      <td>224985.0</td>
      <td>23410968.0</td>
    </tr>
    <tr>
      <th>2022-11-01</th>
      <td>67673235.0</td>
      <td>231960.0</td>
      <td>7309118.0</td>
    </tr>
    <tr>
      <th>2022-12-01</th>
      <td>123719055.0</td>
      <td>315180.0</td>
      <td>10803766.0</td>
    </tr>
    <tr>
      <th>2023-01-01</th>
      <td>49924605.0</td>
      <td>371970.0</td>
      <td>5001556.0</td>
    </tr>
    <tr>
      <th>2023-02-01</th>
      <td>49711860.0</td>
      <td>295290.0</td>
      <td>6866584.0</td>
    </tr>
    <tr>
      <th>2023-03-01</th>
      <td>44049195.0</td>
      <td>232905.0</td>
      <td>6237515.0</td>
    </tr>
    <tr>
      <th rowspan="12" valign="top">Sudden Attack</th>
      <th>2022-04-01</th>
      <td>1465140.0</td>
      <td>77460.0</td>
      <td>1132780.0</td>
    </tr>
    <tr>
      <th>2022-05-01</th>
      <td>305385.0</td>
      <td>63405.0</td>
      <td>152351.0</td>
    </tr>
    <tr>
      <th>2022-06-01</th>
      <td>545160.0</td>
      <td>62700.0</td>
      <td>857681.0</td>
    </tr>
    <tr>
      <th>2022-07-01</th>
      <td>1042155.0</td>
      <td>64140.0</td>
      <td>1733149.0</td>
    </tr>
    <tr>
      <th>2022-08-01</th>
      <td>30591210.0</td>
      <td>69585.0</td>
      <td>6449430.0</td>
    </tr>
    <tr>
      <th>2022-09-01</th>
      <td>264210.0</td>
      <td>58935.0</td>
      <td>437217.0</td>
    </tr>
    <tr>
      <th>2022-10-01</th>
      <td>191115.0</td>
      <td>53625.0</td>
      <td>323997.0</td>
    </tr>
    <tr>
      <th>2022-11-01</th>
      <td>145470.0</td>
      <td>38820.0</td>
      <td>26122.0</td>
    </tr>
    <tr>
      <th>2022-12-01</th>
      <td>183945.0</td>
      <td>45075.0</td>
      <td>57781.0</td>
    </tr>
    <tr>
      <th>2023-01-01</th>
      <td>228090.0</td>
      <td>50415.0</td>
      <td>58710.0</td>
    </tr>
    <tr>
      <th>2023-02-01</th>
      <td>183630.0</td>
      <td>38355.0</td>
      <td>290956.0</td>
    </tr>
    <tr>
      <th>2023-03-01</th>
      <td>145590.0</td>
      <td>44745.0</td>
      <td>47572.0</td>
    </tr>
    <tr>
      <th rowspan="12" valign="top">VALORANT</th>
      <th>2022-04-01</th>
      <td>149503380.0</td>
      <td>204105.0</td>
      <td>12566944.0</td>
    </tr>
    <tr>
      <th>2022-05-01</th>
      <td>70078710.0</td>
      <td>185115.0</td>
      <td>11423350.0</td>
    </tr>
    <tr>
      <th>2022-06-01</th>
      <td>96332400.0</td>
      <td>168720.0</td>
      <td>12875971.0</td>
    </tr>
    <tr>
      <th>2022-07-01</th>
      <td>315103395.0</td>
      <td>190575.0</td>
      <td>18056574.0</td>
    </tr>
    <tr>
      <th>2022-08-01</th>
      <td>196668240.0</td>
      <td>194160.0</td>
      <td>16758347.0</td>
    </tr>
    <tr>
      <th>2022-09-01</th>
      <td>469484325.0</td>
      <td>284310.0</td>
      <td>16429243.0</td>
    </tr>
    <tr>
      <th>2022-10-01</th>
      <td>248151960.0</td>
      <td>190860.0</td>
      <td>16291599.0</td>
    </tr>
    <tr>
      <th>2022-11-01</th>
      <td>117101790.0</td>
      <td>155550.0</td>
      <td>14587779.0</td>
    </tr>
    <tr>
      <th>2022-12-01</th>
      <td>90827205.0</td>
      <td>175065.0</td>
      <td>11376024.0</td>
    </tr>
    <tr>
      <th>2023-01-01</th>
      <td>88647735.0</td>
      <td>179670.0</td>
      <td>11543168.0</td>
    </tr>
    <tr>
      <th>2023-02-01</th>
      <td>131511075.0</td>
      <td>205965.0</td>
      <td>12742004.0</td>
    </tr>
    <tr>
      <th>2023-03-01</th>
      <td>141763995.0</td>
      <td>201405.0</td>
      <td>12961412.0</td>
    </tr>
  </tbody>
</table>
</div>



#### 5) 최대 시청자, 평균 시청자에 대한 평균 정보

게임별 월별 최대 시청자 및 평균 시청자에 대한 평균 정보를 구한다.


```python
fps_gd_mean_group = fps_gd_group[['Peak viewers', 'Average viewers']].mean()
fps_gd_mean_group
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th></th>
      <th>Peak viewers</th>
      <th>Average viewers</th>
    </tr>
    <tr>
      <th>Game</th>
      <th>Date</th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th rowspan="12" valign="top">Overwatch</th>
      <th>2022-04-01</th>
      <td>2167.5600</td>
      <td>1355.470000</td>
    </tr>
    <tr>
      <th>2022-05-01</th>
      <td>455.7500</td>
      <td>286.460000</td>
    </tr>
    <tr>
      <th>2022-06-01</th>
      <td>399.5600</td>
      <td>241.280000</td>
    </tr>
    <tr>
      <th>2022-07-01</th>
      <td>1599.8500</td>
      <td>803.730000</td>
    </tr>
    <tr>
      <th>2022-08-01</th>
      <td>566.0500</td>
      <td>430.260000</td>
    </tr>
    <tr>
      <th>2022-09-01</th>
      <td>254.8100</td>
      <td>154.860000</td>
    </tr>
    <tr>
      <th>2022-10-01</th>
      <td>4422.0900</td>
      <td>2458.350000</td>
    </tr>
    <tr>
      <th>2022-11-01</th>
      <td>910.6700</td>
      <td>570.090000</td>
    </tr>
    <tr>
      <th>2022-12-01</th>
      <td>1640.7400</td>
      <td>817.760000</td>
    </tr>
    <tr>
      <th>2023-01-01</th>
      <td>369.0200</td>
      <td>207.900000</td>
    </tr>
    <tr>
      <th>2023-02-01</th>
      <td>703.8400</td>
      <td>483.540000</td>
    </tr>
    <tr>
      <th>2023-03-01</th>
      <td>523.4700</td>
      <td>317.340000</td>
    </tr>
    <tr>
      <th rowspan="12" valign="top">Sudden Attack</th>
      <th>2022-04-01</th>
      <td>109.7600</td>
      <td>91.100000</td>
    </tr>
    <tr>
      <th>2022-05-01</th>
      <td>20.0800</td>
      <td>16.300000</td>
    </tr>
    <tr>
      <th>2022-06-01</th>
      <td>44.2700</td>
      <td>30.460000</td>
    </tr>
    <tr>
      <th>2022-07-01</th>
      <td>91.9100</td>
      <td>80.610000</td>
    </tr>
    <tr>
      <th>2022-08-01</th>
      <td>558.7400</td>
      <td>279.380000</td>
    </tr>
    <tr>
      <th>2022-09-01</th>
      <td>18.7800</td>
      <td>15.820000</td>
    </tr>
    <tr>
      <th>2022-10-01</th>
      <td>10.7200</td>
      <td>8.280000</td>
    </tr>
    <tr>
      <th>2022-11-01</th>
      <td>6.4375</td>
      <td>4.510417</td>
    </tr>
    <tr>
      <th>2022-12-01</th>
      <td>7.8000</td>
      <td>5.760000</td>
    </tr>
    <tr>
      <th>2023-01-01</th>
      <td>13.4600</td>
      <td>10.740000</td>
    </tr>
    <tr>
      <th>2023-02-01</th>
      <td>13.0500</td>
      <td>10.640000</td>
    </tr>
    <tr>
      <th>2023-03-01</th>
      <td>7.5200</td>
      <td>5.290000</td>
    </tr>
    <tr>
      <th rowspan="12" valign="top">VALORANT</th>
      <th>2022-04-01</th>
      <td>1882.9400</td>
      <td>977.980000</td>
    </tr>
    <tr>
      <th>2022-05-01</th>
      <td>1342.9000</td>
      <td>836.160000</td>
    </tr>
    <tr>
      <th>2022-06-01</th>
      <td>1477.3900</td>
      <td>884.630000</td>
    </tr>
    <tr>
      <th>2022-07-01</th>
      <td>2866.6500</td>
      <td>1542.160000</td>
    </tr>
    <tr>
      <th>2022-08-01</th>
      <td>2328.0700</td>
      <td>1335.650000</td>
    </tr>
    <tr>
      <th>2022-09-01</th>
      <td>3714.0500</td>
      <td>1753.260000</td>
    </tr>
    <tr>
      <th>2022-10-01</th>
      <td>3336.1900</td>
      <td>1641.290000</td>
    </tr>
    <tr>
      <th>2022-11-01</th>
      <td>1757.3400</td>
      <td>1047.750000</td>
    </tr>
    <tr>
      <th>2022-12-01</th>
      <td>1258.0400</td>
      <td>772.930000</td>
    </tr>
    <tr>
      <th>2023-01-01</th>
      <td>1781.4800</td>
      <td>1049.300000</td>
    </tr>
    <tr>
      <th>2023-02-01</th>
      <td>1479.6800</td>
      <td>803.170000</td>
    </tr>
    <tr>
      <th>2023-03-01</th>
      <td>1469.2500</td>
      <td>836.360000</td>
    </tr>
  </tbody>
</table>
</div>



#### 6) 대회 기간을 제외한 달의 평균 데이터

대회 기간과 대회 기간 이후의 차이를 구하기 위해 계산한다. 단 Overwatch 데이터는 2022년 10월 5일에 Overwatch2 얼리액세스 개시라는 특이 케이스가 있음으로, 이를 추가로 제외한다.


```python
overwatch_no_conf = fps_clean_data.loc[(fps_clean_data['Game'] == 'Overwatch') & ((fps_clean_data['Date'] != '2022-07-01') & (fps_clean_data['Date'] != '2022-10-01') & (fps_clean_data['Date'] != '2022-12-01'))]
overwatch_no_conf_group = overwatch_no_conf.groupby(['Game'])['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers'].mean()
overwatch_no_conf_group
```

    /tmp/ipykernel_25/2672062703.py:2: FutureWarning: Indexing with multiple keys (implicitly converted to a tuple of keys) will be deprecated, use a list instead.
      overwatch_no_conf_group = overwatch_no_conf.groupby(['Game'])['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers'].mean()





<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Watch time (mins)</th>
      <th>Stream time (mins)</th>
      <th>Peak viewers</th>
      <th>Average viewers</th>
      <th>Followers</th>
    </tr>
    <tr>
      <th>Game</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Overwatch</th>
      <td>510462.05</td>
      <td>2680.566667</td>
      <td>705.636667</td>
      <td>449.688889</td>
      <td>70536.982222</td>
    </tr>
  </tbody>
</table>
</div>



Overwatch 말고도 Sudden Attack 과 VALORANT에도 같은 처리를 해준댜.


```python
sudden_no_conf = fps_clean_data.loc[(fps_clean_data['Game'] == 'Sudden Attack') & (fps_clean_data['Date'] != '2022-08-01')]
sudden_no_conf_group = sudden_no_conf.groupby(['Game'])['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers'].mean()
valorant_no_conf = fps_clean_data.loc[(fps_clean_data['Game'] == 'VALORANT') & (fps_clean_data['Date'] != '2022-09-01')]
valorant_no_conf_group = valorant_no_conf.groupby(['Game'])['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers'].mean()
```

    /tmp/ipykernel_25/1828670829.py:2: FutureWarning: Indexing with multiple keys (implicitly converted to a tuple of keys) will be deprecated, use a list instead.
      sudden_no_conf_group = sudden_no_conf.groupby(['Game'])['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers'].mean()
    /tmp/ipykernel_25/1828670829.py:4: FutureWarning: Indexing with multiple keys (implicitly converted to a tuple of keys) will be deprecated, use a list instead.
      valorant_no_conf_group = valorant_no_conf.groupby(['Game'])['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers'].mean()


#### 7) 방송 시간당 시청 시간 계산

단순히 방송 시간이 많아 그에 따라 시청 시간이 불어났을 수 있기 때문에, Watch time (mins) / Stream time (mins) 를 통해 방송 시간당 시청 시간 **Watch per Stream 파생변수**를 만들어 데이터의 신뢰성을 높인다.


```python
overwatch_no_conf_group['Watch per Stream'] = overwatch_no_conf_group['Watch time (mins)'] / overwatch_no_conf_group['Stream time (mins)']
sudden_no_conf_group['Watch per Stream'] = sudden_no_conf_group['Watch time (mins)'] / sudden_no_conf_group['Stream time (mins)']
valorant_no_conf_group['Watch per Stream'] = valorant_no_conf_group['Watch time (mins)'] / valorant_no_conf_group['Stream time (mins)']
```

#### 8) 대회 기간 아닌 데이터에 대한 데이터프레임 연결


```python
no_conf_group = pd.DataFrame()
no_conf_group = pd.concat([no_conf_group, overwatch_no_conf_group, sudden_no_conf_group, valorant_no_conf_group])
no_conf_group = no_conf_group[['Watch per Stream', 'Peak viewers', 'Average viewers', 'Followers']]
no_conf_group
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Watch per Stream</th>
      <th>Peak viewers</th>
      <th>Average viewers</th>
      <th>Followers</th>
    </tr>
    <tr>
      <th>Game</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Overwatch</th>
      <td>190.430649</td>
      <td>705.636667</td>
      <td>449.688889</td>
      <td>70536.982222</td>
    </tr>
    <tr>
      <th>Sudden Attack</th>
      <td>7.863622</td>
      <td>31.343978</td>
      <td>25.486314</td>
      <td>4669.996350</td>
    </tr>
    <tr>
      <th>VALORANT</th>
      <td>802.309823</td>
      <td>1907.266364</td>
      <td>1066.125455</td>
      <td>137439.247273</td>
    </tr>
  </tbody>
</table>
</div>



#### 9) 대회 기간 데이터 탐색

(6) ~ (8) 까지의 과정을 대회 기간으로 적용한다.


```python
overwatch_conf = fps_clean_data.loc[(fps_clean_data['Game'] == 'Overwatch') & ((fps_clean_data['Date'] == '2022-07-01') | (fps_clean_data['Date'] == '2022-12-01'))]
overwatch_conf_group = overwatch_conf.groupby(['Game'])['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers'].mean()
sudden_conf = fps_clean_data.loc[(fps_clean_data['Game'] == 'Sudden Attack') & (fps_clean_data['Date'] == '2022-08-01')]
sudden_conf_group = sudden_conf.groupby(['Game'])['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers'].mean()
valorant_conf = fps_clean_data.loc[(fps_clean_data['Game'] == 'VALORANT') & (fps_clean_data['Date'] == '2022-09-01')]
valorant_conf_group = valorant_conf.groupby(['Game'])['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers'].mean()

overwatch_conf_group['Watch per Stream'] = overwatch_conf_group['Watch time (mins)'] / overwatch_conf_group['Stream time (mins)']
sudden_conf_group['Watch per Stream'] = sudden_conf_group['Watch time (mins)'] / sudden_conf_group['Stream time (mins)']
valorant_conf_group['Watch per Stream'] = valorant_conf_group['Watch time (mins)'] / valorant_conf_group['Stream time (mins)']

conf_group = pd.DataFrame()
conf_group = pd.concat([conf_group, overwatch_conf_group, sudden_conf_group, valorant_conf_group])
conf_group = conf_group[['Watch per Stream', 'Peak viewers', 'Average viewers', 'Followers']]
conf_group
```

    /tmp/ipykernel_25/3124496987.py:2: FutureWarning: Indexing with multiple keys (implicitly converted to a tuple of keys) will be deprecated, use a list instead.
      overwatch_conf_group = overwatch_conf.groupby(['Game'])['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers'].mean()
    /tmp/ipykernel_25/3124496987.py:4: FutureWarning: Indexing with multiple keys (implicitly converted to a tuple of keys) will be deprecated, use a list instead.
      sudden_conf_group = sudden_conf.groupby(['Game'])['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers'].mean()
    /tmp/ipykernel_25/3124496987.py:6: FutureWarning: Indexing with multiple keys (implicitly converted to a tuple of keys) will be deprecated, use a list instead.
      valorant_conf_group = valorant_conf.groupby(['Game'])['Watch time (mins)', 'Stream time (mins)', 'Peak viewers', 'Average viewers', 'Followers'].mean()





<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Watch per Stream</th>
      <th>Peak viewers</th>
      <th>Average viewers</th>
      <th>Followers</th>
    </tr>
    <tr>
      <th>Game</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Overwatch</th>
      <td>416.867479</td>
      <td>1620.295</td>
      <td>810.745</td>
      <td>106284.035</td>
    </tr>
    <tr>
      <th>Sudden Attack</th>
      <td>439.623626</td>
      <td>558.740</td>
      <td>279.380</td>
      <td>64494.300</td>
    </tr>
    <tr>
      <th>VALORANT</th>
      <td>1651.311333</td>
      <td>3714.050</td>
      <td>1753.260</td>
      <td>164292.430</td>
    </tr>
  </tbody>
</table>
</div>



### 5. 데이터 시각화

날짜별 변화를 효과적으로 파악하기 위해 바 플롯 형태를 사용하였다.


```python
sns.catplot(x="Game", y="Watch time (mins)", hue="Date", data=fps_gd_max_group.reset_index(), kind="bar")
```




    <seaborn.axisgrid.FacetGrid at 0x7fbd37e78af0>




    
![png](output_88_1.png)
    


### 6. 데이터 분석

우선 시각화 데이터 통해 특이 케이스로 분류할 수 있는 Overwatch의 10월달 데이터를 제외하면 각 대회 기간마다 시청 시간이 급격하게 증가하는 것을 확인할 수 있다. 이 외에도 전반적으로 VALORANT가 시청 시간이 많고, Overwatch가 그 다음이며, Sudden Attack은 매우 적다는 것을 볼 수 있다.

다음으로 데이터 탐색 결과를 보면, 대회 기간을 제외한 게임들의 Watch Per Stream의 평균값은 각각 190, 7, 802이지만, 대회 기간 동안의 Watch Per Stream의 평균값은 416, 439, 1651로 증가한 것을 확인할 수 있다. 가장 높은 증가율을 보여준 게임은 Sudden Attack으로 6271%의 방송 시간당 시청 시간이 증가하였다. 가장 낮은 증가율은 VALORANT로 205%만큼 증가한 것을 확인할 수 있다.

평균 시청자 수 Average viewers의 변화를 보면, 대회 기간을 제외한 값은 449, 25, 1066 이지만, 대회 기간의 평균 시청자 수는 810, 279, 1753으로 각각 180%, 1116%, 164% 증가하였다.

다음 결과로부터 도출할 수 있는 결론은 **대회를 통해 최대 6271%의 뷰어십 증가 효과를 볼 수 있다**는 것이다. 특히 기존 시청자 풀을 크게 확보하고 있던 게임보다, **기존 시청자 풀을 적게 확보하고 있던 게임의 경우 효과가 더욱 크게 나타났다.** 따라서 신규 게임을 대상으로 대회형 마케팅을 시도할 경우 더욱 극적인 효과를 볼 수 있을 것으로 예상된다.

## 데이터 분석 : 유지성

**대회를 통해 시청자들을 많이 끌어모을 수 있지만, 대회가 끝난 이후 얼마나 끌어모은 시청자들이 유지되는가에 대한 분석이다.**

### 4. 데이터 탐색

#### 1) 대회 전 후 구분을 위한 컬럼 생성

데이터 분류를 위해 대회 이전은 0으로, 대회 기간은 1로, 대회 이후는 2로 지정한 컬럼을 생성한다.
Overwatch의 경우 하계와 동계 두 번의 대회가 있었는데, 이중 동계 대회의 경우 이전 2개월 중 얼리 액세스 개시라는 특이 케이스 데이터가 포함되어 있어 제대로 된 분석을 진행할 수 없음으로 하계 대회에 대한 데이터만 진행을 한다.


```python
fps_clean_data['Conference'] = 0
fps_clean_data.loc[(fps_clean_data['Game']=='Overwatch') & (fps_clean_data['Date'] == '2022-07-01'), 'Conference'] = 1
fps_clean_data.loc[(fps_clean_data['Game']=='Overwatch') & (fps_clean_data['Date'] > '2022-07-01'), 'Conference'] = 2
fps_clean_data.loc[(fps_clean_data['Game']=='Sudden Attack') & (fps_clean_data['Date'] == '2022-08-01'), 'Conference'] = 1
fps_clean_data.loc[(fps_clean_data['Game']=='Sudden Attack') & (fps_clean_data['Date'] > '2022-08-01'), 'Conference'] = 2
fps_clean_data.loc[(fps_clean_data['Game']=='VALORANT') & (fps_clean_data['Date'] == '2022-09-01'), 'Conference'] = 1
fps_clean_data.loc[(fps_clean_data['Game']=='VALORANT') & (fps_clean_data['Date'] > '2022-09-01'), 'Conference'] = 2

fps_clean_data['Conference']
```




    14      0
    3       0
    19      0
    0       0
    18      0
           ..
    4148    2
    4203    2
    4202    2
    4171    2
    4220    2
    Name: Conference, Length: 3596, dtype: int64



#### 2) 게임별 대회 전 2개월 데이터의 평균값 탐색


```python
before_conference = fps_clean_data[fps_clean_data['Conference']==0].groupby(['Game', 'Date']).mean()
del before_conference['Unnamed: 0']
before_conference = before_conference.groupby('Game').tail(2)
before_conference = before_conference.groupby('Game').mean()
before_conference
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Watch time (mins)</th>
      <th>Stream time (mins)</th>
      <th>Peak viewers</th>
      <th>Average viewers</th>
      <th>Followers</th>
      <th>Conference</th>
    </tr>
    <tr>
      <th>Game</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Overwatch</th>
      <td>407276.325</td>
      <td>2860.725</td>
      <td>427.655</td>
      <td>263.870</td>
      <td>58864.620</td>
      <td>0.0</td>
    </tr>
    <tr>
      <th>Sudden Attack</th>
      <td>7936.575</td>
      <td>634.200</td>
      <td>68.090</td>
      <td>55.535</td>
      <td>12954.150</td>
      <td>0.0</td>
    </tr>
    <tr>
      <th>VALORANT</th>
      <td>2558858.175</td>
      <td>1923.675</td>
      <td>2597.360</td>
      <td>1438.905</td>
      <td>174074.605</td>
      <td>0.0</td>
    </tr>
  </tbody>
</table>
</div>



#### 3) 게임별 대회 후 2개월 데이터의 평균값 탐색


```python
after_conference = fps_clean_data[fps_clean_data['Conference']==2].groupby(['Game', 'Date']).mean()
del after_conference['Unnamed: 0']
after_conference = after_conference.groupby('Game').head(2)
after_conference = after_conference.groupby('Game').mean()
after_conference
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Watch time (mins)</th>
      <th>Stream time (mins)</th>
      <th>Peak viewers</th>
      <th>Average viewers</th>
      <th>Followers</th>
      <th>Conference</th>
    </tr>
    <tr>
      <th>Game</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Overwatch</th>
      <td>301398.525</td>
      <td>2328.30</td>
      <td>410.430</td>
      <td>292.56</td>
      <td>52570.805</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>Sudden Attack</th>
      <td>2276.625</td>
      <td>562.80</td>
      <td>14.750</td>
      <td>12.05</td>
      <td>3806.070</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>VALORANT</th>
      <td>1826268.750</td>
      <td>1732.05</td>
      <td>2546.765</td>
      <td>1344.52</td>
      <td>154396.890</td>
      <td>2.0</td>
    </tr>
  </tbody>
</table>
</div>



#### 4) 데이터프레임 연결

원활한 데이터 비교를 위해 데이터프레임을 연결시켜주었다.


```python
conference_data = pd.DataFrame()
conference_data = pd.concat([conference_data, before_conference, after_conference])
conference_data = conference_data.sort_index()
conference_data
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Watch time (mins)</th>
      <th>Stream time (mins)</th>
      <th>Peak viewers</th>
      <th>Average viewers</th>
      <th>Followers</th>
      <th>Conference</th>
    </tr>
    <tr>
      <th>Game</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Overwatch</th>
      <td>407276.325</td>
      <td>2860.725</td>
      <td>427.655</td>
      <td>263.870</td>
      <td>58864.620</td>
      <td>0.0</td>
    </tr>
    <tr>
      <th>Overwatch</th>
      <td>301398.525</td>
      <td>2328.300</td>
      <td>410.430</td>
      <td>292.560</td>
      <td>52570.805</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>Sudden Attack</th>
      <td>7936.575</td>
      <td>634.200</td>
      <td>68.090</td>
      <td>55.535</td>
      <td>12954.150</td>
      <td>0.0</td>
    </tr>
    <tr>
      <th>Sudden Attack</th>
      <td>2276.625</td>
      <td>562.800</td>
      <td>14.750</td>
      <td>12.050</td>
      <td>3806.070</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>VALORANT</th>
      <td>2558858.175</td>
      <td>1923.675</td>
      <td>2597.360</td>
      <td>1438.905</td>
      <td>174074.605</td>
      <td>0.0</td>
    </tr>
    <tr>
      <th>VALORANT</th>
      <td>1826268.750</td>
      <td>1732.050</td>
      <td>2546.765</td>
      <td>1344.520</td>
      <td>154396.890</td>
      <td>2.0</td>
    </tr>
  </tbody>
</table>
</div>



### 5. 데이터 시각화

탐색 과정을 통해 도출한 대회 이전 2개월간의 평균 방송 시간과, 대회 이후 2개월간의 평균 방송 시간을 시각화하였다.
여러 데이터가 있지만, 그 중 방송 시간 Stream time (mins)가 게임에 관심을 지속해서 가지고 개인 방송의 콘텐츠로서 진행하는 방송인의 수를 의미함으로 방송 시간을 기준으로 시각화하였다.


```python
sns.catplot(x="Game", y="Stream time (mins)", hue="Conference", data=conference_data.reset_index(), kind="bar")
plt.yscale('log')
```


    
![png](output_99_0.png)
    


### 6. 데이터 분석

특이하게도 대회 이후 방송 시간이 각각 2860, 634, 1923 에서 2328, 562, 1732 로 19%, 11%, 10% 만큼 **감소**하였다. 방송 시간을 이외의 데이터 역시 전반적으로 수치가 감소한 것을 확인할 수 있다. 이에 대한 원인으로는 다음 4가지를 들 수 있다.
1. 한 대회가 끝나고 이어서 다음 대회가 시작하기에, 시청자와 개인 방송인들이 대회가 진행중인 게임을 진행하러가 수치가 감소하였다.
2. 대회가 끝나면 개인 방송인은 대회 기간 동안 집중적으로 해당 게임을 진행하였기에 일종의 번아웃으로서 대회를 진행한 게임에 거부감을 가진다.
3. 대회 시작 전에는 시청자들은 대회에 대한 기대감을 가진다.
4. 대회 시작 전에는 개인 방송인들은 대회에 대비하기 위해 연습 시간을 가진다.

다음 결과로부터 도출할 수 있는 결론은 여러 요인들로 인한 **대회형 마케팅의 부작용으로서 유지성이 감소**한다는 것을 확인할 수 있다.

# 결론

 대회형 마케팅을 통해 유입성을 크게 높일 수 있지만 그에 대한 유지성이 떨어지는 것을 넘어 오히려 대회 이전보다 감소한다는 사실을 알 수 있다. 단 이 데이터는 Twitch 플랫폼의 개인 방송에 대한 데이터로서 실제 게임 사용자의 데이터와는 다르다는 것을 염두에 두어야 한다. 따라서 **많은 사람들에게 게임을 홍보하는 목적으로서의 마케팅이라면 대회형 마케팅이 적합**할 수 있으나, 지속적으로 게임을 플레이하는 사용자를 원하는, 즉 **게임 사용자 풀을 염두에 둔 마케팅이라면 대회형 마케팅은 부적절할 수 있다.**

## 7. 데이터 분석 차별화 포인트

데이터를 그대로 사용하는 것이 아닌 파생 변수 활용, 그룹 분석 및 데이터 재구조화를 적극적으로 사용하였다는 점과, 실제 기업에서 사용하는 데이터를 대상으로 명확한 목표를 가지고 데이터를 분석하여 의미 있는 결과를 도출하였다는 점이 가장 차별화될 수 있는 포인트라 생각한다.


## 8. 데이터분석 수업을 마감하며

수업적 내용으로 말하면 3학년 수업이면서 개론 수업이라 이상할 수 있지만, 개론에 걸맞는 데이터를 다루는 꼭 알아야 하는 내용에 대해 집중적으로 진행하는 것이 좋았다. 빅데이터라는게 이제는 '빅데이터'라는 하나의 과목에서 멈춘 것이 아니라 머신러닝, 데이터베이스, 웹, 심지어 시스템 프로그램에서도 활용할 수 있는 내용이라 사실 선택이 아닌 필수적인 과목이라 생각된다.


수업 외적 내용으로 말하면, 학생들을 밖으로 내몰아 세상 경험을 하게 해주며 정말 대학교 신입생때 알았으면 좋았을 정보를 강력하게 피력해서 알려주셔서 좋았다. 이미 4학년이라 늦었다고 생각될지 몰라도 지금부터라도 열심히 외부 경험을 할 수 있으면 더 좋은 결과가 있을 것이라 기대한다.


