# 1. 제한사항
- String user, List<List<String>> friends, List<String> visitors 가 주어진다.
- user는 길이가 1이상 30이하인 문자열이다
- friends는 길이가 1 이상 10,000 이하이다.
- friends의 아이디의 길이는 1이상 30 이하이다.
- visitors는 길이가 0 이상 10,000 이하이다.
- 사용자 아이디는 알파벳 소문자로만 이루어져 있다.
- 동일한 친구 관계가 중복해서 주어지지 않는다.
- 추천할 친구가 없는 경우는 주어지지 않는다.
- 점수가 가장 높은 친구를 기준으로, 점수가 같다면 이름 순으로 정렬해 최대 5명을 추천한다.
- List <String> 형태로 반환한다.
# 2. 기능목록
- 친구 관계가 주어지면 그 관계를 저장한다.
- 특정 친구에게 더할 점수의 액수가 주어지면 값을 계산하여 저장한다.
- 사용자의 친구의 친구가 존재하면 그 친구에게 점수를 더한다.
- 방문자가 존재하면 그 친구에게 점수를 더한다.
- 이미 사용자의 친구이면 추천 친구로부터 배재시킨다.
- 구한 친구의 점수를 점수를 기준으로 내림차순으로 정렬하고 점수가 같다면 이름을 기준으로 오름차순 정렬한다.
- 점수와 이름을 기준으로 정렬한 map을 최종적으로 최대 5명을 추천할 친구의 명단을 list로 만들어 반환한다.