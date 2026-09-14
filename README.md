from typing import Any


class Wonu:
    name = '양원우'
    role = 'Backend Developer'

    introduction = (
        '팀원들이 여러 걱정을 하지 않도록 고민하며, '
        '유지보수하기 쉬운 소프트웨어를 개발하는 백엔드 개발자입니다.'
    )

    education = {
        'school': '경북소프트웨어마이스터고등학교',
        'status': '재학 중',
        'focus': ['Backend Development', 'AI/ML', 'Web Development'],
    }

    skills = [
        'Python',
        'FastAPI',
        'Node.js',
        'Express',
        'React',
        'TypeScript',
        'OpenAI API',
        'OCR',
        'JWT Authentication',
        'MariaDB',
        'Chrome Extension',
        'REST API',
    ]

    projects = [
        {
            'name': 'Reply',
            'description': '유튜브 댓글 AI 필터링 크롬 확장 프로그램',
            'role': 'Backend Developer',
            'technologies': [
                'Python',
                'FastAPI',
                'Node.js',
                'OpenAI API',
                'Chrome Extension',
            ],
            'contributions': [
                '유튜브 댓글 데이터를 AI 서버로 전달하는 백엔드 로직 구현',
                'AI 분석 결과를 반환하는 REST API 개발',
                '프론트엔드와 통신하기 위한 JSON 스키마 설계',
                '욕설 강도에 따른 댓글 숨김 및 순화 처리 구조 구현',
            ],
        },
        {
            'name': 'Folio',
            'description': 'AI 기반 포트폴리오 분석 및 커리어 컨설팅 서비스',
            'role': 'Backend & AI Developer',
            'technologies': [
                'FastAPI',
                'Node.js',
                'Express',
                'React',
                'TypeScript',
                'OpenAI API',
            ],
            'contributions': [
                '회원가입·로그인 및 JWT 인증 API 구현',
                '프로필 조회·수정 API 설계 및 구현',
                'PDF와 이미지 파일을 처리하는 OCR 엔진 구현',
                'OCR 결과를 줄과 블록 단위로 재구성하는 Layout 엔진 개발',
                'OpenAI API를 활용한 포트폴리오 분석 및 커리어 컨설팅 구현',
                '프론트엔드와 통신하기 위한 REST API 및 JSON 스키마 설계',
            ],
            'links': {
                'service': 'https://www.hellogsm.kr/',
                'github': 'https://github.com/yoosion030/hello-gsm-front',
            },
        },
    ]

    activities = [
        {
            'name': '웹 개발 동아리 WINE',
            'period': '2025.03.19 ~',
            'role': 'Backend Developer',
        },
        {
            'name': '교내 체육 학생부',
            'period': '2025.03.19 ~',
            'role': '학생부 활동',
        },
        {
            'name': 'IT 코딩 발명 아이디어 및 에세이 경진대회',
            'achievement': '장려상',
        },
        {
            'name': '2025 SOFT WAVE 출품',
            'project': 'Reply',
        },
        {
            'name': '2026 AI EXPO 출품',
            'project': 'Folio',
        },
    ]

    certifications = [
        'ITQ PowerPoint',
        'SQLD 결과 대기 중',
    ]

    contacts = {
        'email': 'anyaswint@gmail.com',
        'github': 'https://github.com/wonu1016',
        'tech_blog': 'https://velog.io/@anyaswint/posts',
        'linktree': 'https://linktr.ee/anyaswint',
        'portfolio': (
            'https://wonu-portfolio.notion.site/'
            '0a97ea1e118183969d1781d77d7c3dce'
        ),
    }

    def introduce(self) -> dict[str, Any]:
        return {
            'name': self.name,
            'role': self.role,
            'introduction': self.introduction,
            'education': self.education,
            'skills': self.skills,
            'projects': self.projects,
            'activities': self.activities,
            'certifications': self.certifications,
            'contacts': self.contacts,
        }


me = Wonu()
print(me.introduce())
