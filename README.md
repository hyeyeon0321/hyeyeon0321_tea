# hyeyeon0321_tea
def recommend_tea(health_condition):
    tea_recommendations = {
        "스트레스": [("카모마일 차", 2), ("라벤더 차", 2)],
        "불면증": [("카모마일 차", 2), ("발레리안 차", 2)],
        "소화불량": [("페퍼민트 차", 3), ("생강 차", 3)],
        "면역력 강화": [("그린 티", 2), ("에키네시아 차", 2)],
        "피로 회복": [("레몬 티", 3), ("홍차", 2)]
    }

    if health_condition in tea_recommendations:
        recommendations = tea_recommendations[health_condition]
        print(f"{health_condition}에 권장되는 차:")
        for tea, cups in recommendations:
            print(f" - {tea}: 하루에 {cups}잔")
    else:
        print("알려지지 않은 건강 상태입니다. 다른 상태를 입력해 주세요.")

# 사용 예시
health_condition = input("건강 상태를 입력하세요 (예: 스트레스, 불면증, 소화불량, 면역력 강화, 피로 회복): ")
recommend_tea(health_condition)
