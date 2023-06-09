정규 표현식(Regylar Expression)
정규표현식(Regular Expression)은 문자열의 패턴을 표현하는데 사용되는 형식 언어입니다. 정규표현식은 특정한 규칙에 맞는 문자열을 찾거나 변형하는 작업에 주로 사용됩니다. 다양한 프로그래밍 언어와 텍스트 편집기에서 지원되며, 문자열 처리와 검색 작업을 보다 효율적이고 유연하게 수행할 수 있도록 도와줍니다.
정규표현식은 여러가지 기능이 있는데 대표적으로 4가지가 있습니다.
1. 패턴 매칭(Matching): 주어진 텍스트에서 특정 패턴을 찾는 작업을 수행합니다. 예를 들어, 이메일 주소, 전화번호, URL 등과 같은 특정 형식의 문자열을 찾을 수 있습니다.
2. 검색 및 대체(Search and Replace): 텍스트에서 특정 패턴을 찾아 다른 문자열로 대체할 수 있습니다. 이를 통해 문자열 내에서 특정 부분을 수정하거나 치환할 수 있습니다.
3. 분리(Splitting): 주어진 텍스트를 특정 패턴을 기준으로 분리할 수 있습니다. 예를 들어, 쉼표로 구분된 문자열을 분리하여 각각의 항목을 추출할 수 있습니다.
4. 유효성 검사(Validation): 주어진 문자열이 특정한 규칙에 부합하는지 확인할 수 있습니다. 예를 들어, 이메일 주소가 유효한 형식인지 검증할 수 있습니다.



정규표현식은 간단한 패턴부터 복잡한 패턴까지 다양한 규칙을 표현할 수 있습니다. 
1. 파이썬에서 정규 표현식을 사용하기 위해서는 'import re'를 사용하여 모듈을 가져옵니다.

        import re

2. 'search'함수를 사용하여 정규 표현식 패턴과 일치하는 첫 번째 문자열을 검색합니다. group() 메서드를 호출하여 일치하는 문자열을 가져올 수 있습니다.

        match = pattern.search('검색 대상 문자열')
        if match:
        print(match.group())

3. 'match()' 함수를 사용하여 문자열의 시작부터 정규 표현식 패턴과 일치하는지 확인할 수 있습니다.

        match = pattern.match('대상 문자열')
        if match:
        print('일치합니다.')

4. 'sub()' 함수를 사용하여 정규 표현식 패턴과 일치하는 문자열을 다른 문자열로 치환할 수 있습니다.

        new_string = pattern.sub('치환할 문자열', '대상 문자열')
        print(new_string)

5. 'split()' 함수를 사용하여 정규 표현식 패턴을 기준으로 문자열을 분할할 수 있습니다.

        result = pattern.split('분할할 문자열')
        print(result)

