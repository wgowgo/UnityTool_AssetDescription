# 📘 Unity Asset Description System
## 🇰🇷 에셋 설명 시스템 · 🇺🇸 Asset Description System

### Unity 에셋 및 GameObject에 설명을 추가하여 Inspector / SceneView Overlay / Console에서 확인할 수 있게 해주는 에디터 확장 도구입니다.
### This Unity Editor extension allows adding descriptions to any asset or GameObject, visible in the Inspector, SceneView overlay, and Console.

## ✨ 주요 기능 Features
### 🇰🇷 한국어

모든 에셋 및 씬 오브젝트에 설명 추가

인스펙터에서 직접 생성/편집/삭제 가능

씬뷰 오버레이로 실시간 표시

선택 변경 시 콘솔에 1회 출력

에셋 삭제 시 설명 파일 자동 삭제

Prefab 인스턴스는 Prefab 원본 설명 사용

텍스트 길이에 맞춰 오버레이 자동 리사이즈

### 🇺🇸 English

Add descriptions to any asset or scene GameObject

Create/edit/delete descriptions directly in the Inspector

Real-time SceneView overlay display

Console prints description once per selection

Automatically removes description file when asset is deleted

Prefab instances inherit description from their prefab

Overlay auto-resizes based on text length

## 📂 폴더 구조 · Folder Structure
Assets/
└── Editor/
    └── AssetDescription/
        ├── AssetDescription.cs
        ├── AssetDescriptionTool.cs
        ├── AssetInspectorDescription.cs
        ├── AssetDescriptionOverlay.cs
        ├── AssetDescriptionAutoCleaner.cs
        └── Description/      ← 설명 파일 자동 저장

## 🚀 사용 방법 · How to Use
### 🇰🇷 한국어
1) 설명 생성/편집

에셋 또는 씬 오브젝트 클릭

Inspector 상단의 "Create Description" 버튼 클릭

즉시 수정 가능하며 SceneView 오버레이 즉시 갱신

2) 오버레이 보기

설명이 존재하는 오브젝트를 선택하면
씬뷰 왼쪽 상단에 설명 박스 표시

3) 전역 설정

Tools > 에셋 설명 에디터

콘솔 출력 ON/OFF

오버레이 ON/OFF

4) 설명 삭제

Inspector 버튼으로 삭제 가능
원본 에셋 삭제 시 자동 삭제됨

### 🇺🇸 English
1) Create / Edit Descriptions

Select any asset or GameObject

Click "Create Description" on the Inspector

Changes update instantly in the SceneView overlay

2) Overlay Display

When selecting an object with a description,
the overlay appears in the top-left of the SceneView

3) Global Settings

Tools > Asset Description Editor

Toggle console output

Toggle overlay visibility

4) Delete Description

Remove via Inspector button
Description auto-deletes if the source asset is removed

## ⚠ 주의 사항 · Notes
### 🇰🇷 한국어

프로젝트 에셋은 GUID 기반으로 설명 저장

씬 오브젝트는 GlobalObjectID 기반

Prefab 인스턴스는 Prefab 설명을 표시

Description 파일은 Git 버전관리에 포함하는 것을 권장

### 🇺🇸 English

Project assets use GUID-based description mapping

Scene objects use GlobalObjectID

Prefab instances display their prefab’s description

Description folder is recommended to be included in version control
