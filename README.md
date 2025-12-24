# 📘 Unity Asset Description System
## 🇰🇷 에셋 설명 시스템 · 🇺🇸 Asset Description System

### Unity 에셋 및 GameObject에 설명을 추가하여 **Inspector / SceneView Overlay / Console**에서 <br/> 확인할 수 있게 해주는 에디터 확장 도구입니다.  
### This Unity Editor extension allows adding descriptions to **any asset or GameObject**, visible in the Inspector, SceneView overlay, and Console.


---

# 주요 기능 · Features

## 🇰🇷 한국어
- 모든 에셋 및 씬 오브젝트에 설명 추가  
- 인스펙터에서 직접 생성/편집/삭제 가능  
- 씬뷰 오버레이로 실시간 표시  
- 선택 변경 시 콘솔에 1회 출력  
- 에셋 삭제 시 설명 파일 자동 삭제  
- Prefab 인스턴스는 Prefab 원본 설명 사용  
- 텍스트 길이에 맞춰 오버레이 자동 리사이즈  

## 🇺🇸 English
- Add descriptions to any asset or scene GameObject  
- Create/edit/delete descriptions directly in the Inspector  
- Real-time SceneView overlay display  
- Console prints description once per selection  
- Automatically removes description file when the referenced asset is deleted  
- Prefab instances inherit their prefab’s description  
- Overlay auto-resizes based on text length  

---

#폴더 구조 · Folder Structure

'''
Assets/<br/>
└── Editor//<br/>
    └── AssetDescription//<br/>
        ├── AssetDescription.cs                  ← ScriptableObject 데이터 구조/<br/>
        ├── AssetDescriptionTool.cs              ← 에셋 설명 에디터 윈도우/<br/>
        ├── AssetInspectorDescription.cs         ← Inspector UI 확장/<br/>
        ├── AssetDescriptionOverlay.cs           ← SceneView 오버레이/<br/>
        ├── AssetDescriptionAutoCleaner.cs       ← 에셋 삭제 시 설명 자동 삭제/<br/>
        ├── icon.png                             ← (선택) 에디터 아이콘/<br/>
        └── Description/                         ← 설명 파일 자동 저장 폴더 (자동 생성됨)
'''

---

# 사용 방법 · How to Use

## 🇰🇷 한국어

### 1) 설명 생성/편집
- 에셋 또는 씬 오브젝트 클릭  
- Inspector 상단의 **"Create Description"** 버튼 클릭  
- 설명 즉시 수정 가능, SceneView 오버레이도 즉시 갱신됨  

### 2) 오버레이 보기
- 설명이 존재하는 오브젝트 선택 시  
  SceneView 왼쪽 상단에 설명 박스 표시  

### 3) 전역 설정
**Tools > 에셋 설명 에디터**
- 콘솔 출력 ON/OFF  
- 오버레이 ON/OFF  

### 4) 설명 삭제
- Inspector의 **Delete Description** 버튼으로 삭제 가능  
- 원본 에셋 삭제 시 설명 파일도 자동 삭제됨  

---

## 🇺🇸 English

### 1) Create / Edit Descriptions
- Select any asset or GameObject  
- Click **"Create Description"** in the Inspector  
- Changes update instantly in the SceneView overlay  

### 2) Overlay Display
- When selecting an object with a description,  
  the overlay appears in the top-left of the SceneView  

### 3) Global Settings
**Tools > Asset Description Editor**
- Toggle console output  
- Toggle overlay visibility  

### 4) Delete Description
- Remove via Inspector button  
- Description file auto-deletes when the original asset is removed  

---

# ⚠ 주의 사항 · Notes

## 🇰🇷 한국어
- 프로젝트 에셋은 **GUID 기반**으로 설명 저장  
- 씬 오브젝트는 **GlobalObjectID 기반**  
- Prefab 인스턴스는 Prefab 원본 설명을 표시  
- Description 폴더를 Git 버전관리 대상에 포함하는 것을 권장  

## 🇺🇸 English
- Project assets use a **GUID-based** description mapping  
- Scene objects use **GlobalObjectID**  
- Prefab instances display their prefab’s description  
- It is recommended to include the Description folder in version control  

---
<img width="1097" height="506" alt="image" src="https://github.com/user-attachments/assets/adee5d74-02d5-4807-956e-ba756e0a06d3" />
<br/>
<img width="452" height="201" alt="image" src="https://github.com/user-attachments/assets/65ac6535-4a37-48d9-88e8-9de3e934dcaf" />
<br/>
<img width="451" height="320" alt="image" src="https://github.com/user-attachments/assets/5da180d4-5d9a-4478-ab2b-3316e8f7f2c6" />

