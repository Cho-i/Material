<template>
	<div id="content">
		<template>
			<h2>Material Design</h2>
			<h3>머티리얼 디자인 (Material Design) 이란?</h3>
			<p>
				구글이 처음 모바일 디바이스를 만들때는 사용하기에 그다지 편리한 환경은 아니었습니다. <br>
				하지만, 모바일 디바이스는 빠르게 진화했습니다. 성능은 훨씬 더 강력해졌고, 속도는 빨라졌고, 보다 직관적으로 사용할 수 있도록 발전하였습니다.<br>이러한 변화에 발맞추어, 구글은 모바일과 데스크탑 그리고 그 외 다양한 디바이스들을 아우르는 하나의 일관된 디자인 가이드라인을 공개하였습니다.<br>바로 머티리얼 디자인 (material design) 입니다. <br>머티리얼 디자인은 질감이 느껴지는 표면 (tactile surfaces) 과 대담하고 선명한 그래픽 디자인 (bold graphic design), 그리고 아름답고 직관적인 사용자 경험을 위한 자연스러운 애니메이션을 특징으로 합니다.<br><br>
				머티리얼 디자인에서 표면과 그림자는 물리적인 구조를 형성하여, 사용자들이 화면 상의 어떤 부분을 터치할 수 있고 움직일 수 있는지 쉽게 이해할 수 있도록 돕습니다. <br>현대적인 출판물 디자인 원칙이 반영되어 다른 부가 요소보다 컨텐츠 자체가 강조됩니다. <br>모든 움직임에는 의미가 있으며, 화면 요소들 간의 관계를 명확히 하고 세세한 디테일을 통해 사용자에게 이러한 관계를 알려 쥡니다.
			</p>
			<iframe width="100%" height="500" src="https://www.youtube.com/embed/Q8TXgCzxEnw" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
			<p>
				구글은 작은 시계부터 커다란 TV까지 다양한 종류의 디바이스와 화면 크기를 아우를 수 있는 디자인이 필요했습니다. <br>때문에, 다양한 플랫폼에 일관되게 적용될 수 있는 통일된 디자인 가이드라인을 만들었고, 그 결과, 머티리얼 디자인은 안드로이드 웨어 (Android Wear) 와 안드로이드 TV (Android TV) 그리고 안드로이드 오토 (Android Auto) 에 모두 적용되었습니다. <br>구글 디자인 사이트를 방문하시면 자세한 내용을 확인해보실 수 있습니다.<br><br>
			<strong>안드로이드에서 머리티얼 디자인 적용하기</strong><br>
				안드로이드 L 개발자 프리뷰 버전의 주요 내용 중 하나는 바로 머티리얼 디자인입니다. <br>여러분의 앱에 새로운 스타일을 적용할 수 있도록 머티리얼 테마가 추가되었고, 이를 활용해 손쉽게 여러분의 고유한 브랜드 색상을 자연스럽게 앱에 녹여낼 수 있습니다. <br>또한 새로운 위젯들과 엑티비티 전환 애니매이션을 위한 프레임워크, 움직이는 터치 피드백 기능등도 함께 추가되었습니다. <br>또한, 각 뷰의 깊이 값 (Elevation) 을 설정할 수 있도록 추가되었는데, 이를 통해 UI 요소들을 화면 상에 띄우고 동적으로 적절한 그림자를 표현할 수 있습니다.<br><br>
				<strong>웹에서 머티리얼 디자인 적용하기</strong><br>
				작년 I/O 에서 구글은 다음 세대의 웹을 위한 UI 툴킷을 노리는 야심찬 폴리머 (Polymer) 프로젝트를 공개했습니다. <br>개발자 여러분은 폴리머를 이용해 웹상에서도 만질 수 있을 것 같은 디자인 요소들, 과감하고 선명한 그래픽 디자인, 부드러운 애니매이션 효과 등 머티리얼 디자인의 핵심 요소들을 손쉽게 활용하실 수 있습니다.<br>머티리얼 디자인에 관해 더 궁금한점이 있는 분들은 구글의 머티리얼 디자인 가이드라인을 살펴보시기 바랍니다.
			</p>
			<p>
				<strong>*Polymer</strong><br>
				Material Design을 기반으로 한 Polymer는 웹 컴포넌트 기반 어플리케이션을 쉽고 빠르게 만들게 해주는 라이브러리입니다. <br>구글이 웹 컴포넌트 스팩에 따라 구현한 것이 Polymer 입니다. <br>Polymer를 이해하기 위해선 웹 컴포넌트에 대한 개념이 필요합니다. 웹 컴포넌트는 웹 다큐먼트의 표현을 위젯이나 컴포넌트로 빌딩하는 개념으로 W3C에서 나왔습니다.<br>
				Polymer는 DOM을 템플릿화 하여 재활용함을 목적으로 하고있습니다.<br><br>
				<strong>웹 컴포넌트 4가지 구성요소</strong><br>
				<strong>1. Custom Elements</strong><br>
				HTML에 새로운 HTML/DOM 요소를 정의하는 것입니다.<br><br>
				<strong>2. Templates</strong><br>
				컴포넌트의 골격이 사용되기 전까지 비활성화된 상태로 관리되도록 합니다.<br><br>
				<strong>3. Shadow DOM</strong><br>
				DOM과 스타일을 캡슐화 하여 처리할 수 있도록 해줍니다.<br><br>
				<strong>4. HTML Imports</strong><br>
				위의 요소들을 포함한 Resource를 로딩할 수 있도록 합니다.
			</p>
			<a v-bind:href="link1" target="_blank">Material Design 소개</a>
			<a v-bind:href="link2" target="_blank">Material Design 살펴보기</a>
			<a v-bind:href="link5" target="_blank">Polymer 정리</a>
			<a v-bind:href="link6" target="_blank">Polymer Catalog</a>
			<br>
			<h2>Material UI</h2>
			<a v-bind:href="link3" target="_blank">https://material.io</a>
			<a v-bind:href="link4" target="_blank">https://vuematerial.io/</a>
		</template>

	</div>
</template>

<script>
	export default {
		name: 'content',
		data: () => ({
			link1:'https://developers-kr.googleblog.com/2014/07/this-is-material-design.html',
			link2:'https://www.slideshare.net/watchncompass/3-material-design',
			link3:'https://material.io',
			link4:'https://vuematerial.io/',
			link5:'https://www.slideshare.net/cwdoh/polymer-web-components-web-animations',
			link6:'https://elements.polymer-project.org/',
		})
	}
</script>

<style>
a{display:block;padding:5px;color:#000 !important;}

</style>
