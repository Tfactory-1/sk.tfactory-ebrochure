import React, { useState, useEffect } from "react";
import { motion, AnimatePresence, useScroll, useSpring } from "motion/react";
import { ArrowLeft, ArrowRight } from "lucide-react";
// @ts-ignore
import coverImage from "./cover-1.jpg";
// @ts-ignore
import phoneImage from "./phone_atelier.jpg";
// @ts-ignore
import firstFloorImage from "./1st_floor.jpg";
// @ts-ignore
import skTelecomLogo from "./SK_Telecom_logo.png";
// @ts-ignore
import tFactoryHeaderLogo from "./T Factory_logo.png"; 
// @ts-ignore
import tFactoryFooterLogo from "./T Factory_logo_footer.png";
// @ts-ignore
import mainHall1 from "./main_hall_1.jpg";
// @ts-ignore
import mainHall2 from "./main_hall_2.jpg";

const FLOORS_DATA = [
  {
    id: "garden",
    name: "Garden",
    shortName: "GD",
    label: "T Garden",
    spec: "120m² / 36py / Height 4.2M",
    hotspots: [
      { id: "g1", name: "Glass Greenhouse", x: 30, y: 25, w: 20, h: 22 },
      { id: "g2", name: "Botanical Path", x: 55, y: 40, w: 25, h: 18 },
      { id: "g3", name: "Pavilion", x: 42, y: 15, w: 12, h: 12 }
    ],
    spaces: [
      {
        id: "space-g-1",
        name: "Garden Zone",
        category: "Outdoor",
        description: "도심 속 자연을 느낄 수 있는 정원입니다. 계절의 변화를 담아내는 식물들과 함께 편안한 휴식을 취해보세요.",
        image: "https://images.unsplash.com/photo-1558904541-efa843a96f0f?q=80&w=1920&auto=format&fit=crop"
      }
    ]
  },
  {
    id: "basement",
    name: "Basement",
    shortName: "B1",
    label: "T Factory Vault",
    spec: "250m² / 75py / Height 3.5M",
    hotspots: [
      { id: "b1", name: "Digital Arcade", x: 25, y: 30, w: 18, h: 24 },
      { id: "b2", name: "VR Pod Experience", x: 48, y: 20, w: 22, h: 16 },
      { id: "b3", name: "Sound Cave", x: 62, y: 42, w: 16, h: 20 }
    ],
    spaces: [
      {
        id: "space-b-1",
        name: "Digital Arcade",
        category: "Play",
        description: "다양한 디지털 엔터테인먼트를 즐길 수 있는 B1 공간입니다. 몰입감 넘치는 사운드 룸과 VR 체험이 준비되어 있습니다.",
        image: "https://images.unsplash.com/photo-1511512578047-dfb367046420?q=80&w=1920&auto=format&fit=crop"
      }
    ]
  },
  {
    id: "first_floor",
    name: "First Floor",
    shortName: "1F",
    label: "Main Hall",
    spec: "330m²/100py/height3.9M",
    hotspots: [
      { id: "f1", name: "Photo both", x: 58, y: 48.5, w: 10.5, h: 12.5 },
      { id: "f2", name: "Media Wall", x: 60.5, y: 25.5, w: 10, h: 11.5 },
      { id: "f3", name: "Experience Zone", x: 39.5, y: 41.5, w: 3.2, h: 4.2 },
      { id: "f4", name: "T-Factory Bar", x: 39.5, y: 31.3, w: 5.8, h: 3.2 },
      { id: "f5", name: "Access Gateway", x: 34.1, y: 29.1, w: 3.2, h: 14.8 },
      { id: "f6", name: "Consulting Pod", x: 51.8, y: 20.8, w: 3.2, h: 4.2 }
    ],
    spaces: [
      {
        id: "space-1f-1",
        name: "Main Hall",
        category: "Lounge",
        description: "메인홀은 고정된 틀에 갇히지 않고, 시대의 트렌드와 다채로운 크리에이티브를 유연하게 담아내는 복합 문화 공간입니다. 시즌마다 완전히 새로운 콘셉트의 프로그램과 팝업을 선보이며 방문객들에게 늘 신선한 영감을 선사하고 있습니다. 메인홀은 열린 플랫폼으로서 새로운 시도를 원하는 모든 파트너와의 협업에 언제나 열려 있습니다.",
        image: mainHall1,
        extraInfo: {
          category: "Program",
          description: "현재 메인홀에서는 미래의 기술과 영감을 담은 'BACK TO THE_' 데이터센터 프로그램이 운영 중입니다."
        }
      },
      {
        id: "space-1f-2",
        name: "Experience Zone",
        category: "Experience",
        description: "곳곳에 배치된 체험존과 미디어 디스플레이를 통해 SK텔레콤의 혁신적인 기술과 서비스를 직접 만져보고 경험할 수 있도록 설계되었습니다.",
        image: mainHall2,
      }
    ]
  },
  {
    id: "second_floor",
    name: "Second Floor",
    shortName: "2F",
    label: "Lounge",
    spec: "280m² / 85py / Height 3.8M",
    hotspots: [
      { id: "s1", name: "Phone Atelier", x: 30, y: 25, w: 20, h: 18 },
      { id: "s2", name: "Fortune Photo Zone", x: 60, y: 45, w: 22, h: 18 },
      { id: "s3", name: "Coffee Bar", x: 45, y: 12, w: 18, h: 14 }
    ],
    spaces: [
      {
        id: "space-2f-1",
        name: "Lounge",
        category: "Phone Atelier",
        description: "2층 라운지는 SKT 고객을 위한 고유의 브랜드 경험과 휴식이 결합된 복합 문화 공간입니다. 편안하게 머무를 수 있는 휴식 공간을 중심으로, 브랜드의 위트가 담긴 포춘포토, 고객 맞춤형 큐레이션을 제공하는 폰 아틀리에 존, 그리고 공간의 밀도를 더해주는 커피 바를 유기적으로 구성했습니다. 방문객들에게 단순한 대기를 넘어 가치 있는 브랜드 체류 시간을 선사합니다.",
        image: phoneImage,
      }
    ]
  },
  {
    id: "rooftop",
    name: "Rooftop",
    shortName: "RF",
    label: "Sky Forest",
    spec: "180m² / 54py / Height 4.0M",
    hotspots: [
      { id: "r1", name: "Observatory Deck", x: 35, y: 28, w: 24, h: 22 },
      { id: "r2", name: "Open-Air Garden", x: 62, y: 38, w: 18, h: 18 }
    ],
    spaces: [
      {
        id: "space-r-1",
        name: "Sky Forest",
        category: "Outdoor",
        description: "성수동의 하늘을 한눈에 담을 수 있는 루프탑입니다. 뻥 뚫린 개방감 속에서 브랜드의 또 다른 모습을 발견해 보세요.",
        image: "https://images.unsplash.com/photo-1533104816154-1b151ab17058?q=80&w=1920&auto=format&fit=crop"
      }
    ]
  }
];

const ARCHIVE_DATA = [
  { id: "hero", type: "hero" as const, image: coverImage },
  { id: "floorplan", type: "floorplan" as const },
  { id: "details", type: "details" as const }
];

export default function App() {
  const { scrollYProgress } = useScroll();
  const scaleX = useSpring(scrollYProgress, {
    stiffness: 100,
    damping: 30,
    restDelta: 0.001
  });

  const [activeFloorId, setActiveFloorId] = useState("first_floor");
  const [showHeader, setShowHeader] = useState(false);

  const activeFloor = FLOORS_DATA.find((f) => f.id === activeFloorId) || FLOORS_DATA[2];

  useEffect(() => {
    const handleScroll = () => {
      if (window.scrollY > window.innerHeight * 0.7) {
        setShowHeader(true);
      } else {
        setShowHeader(false);
      }
    };

    window.addEventListener("scroll", handleScroll);
    return () => window.removeEventListener("scroll", handleScroll);
  }, []);

  return (
    <main className="bg-white selection:bg-black selection:text-white relative">
      <motion.div className="fixed top-0 left-0 right-0 h-1 bg-white mix-blend-difference origin-left z-[110]" style={{ scaleX }} />

      <header className={`fixed top-0 left-0 w-full px-4 md:px-8 pt-10 flex justify-between items-center z-[100] mix-blend-difference text-white pointer-events-none transition-opacity duration-500 ${showHeader ? "opacity-100" : "opacity-0"}`}>
        <div className="flex items-center">
         <img src={skTelecomLogo} alt="SK telecom" className="h-2.5 md:h-3 w-auto object-contain" />
        </div>
        <div className="text-[13px] font-medium tracking-tight">
          T Factory 성수
        </div>
        <div className="text-[14px] font-bold font-sans">
          {activeFloor.shortName}
        </div>
      </header>

      {/* 💡 표지 섹션 시작: 모바일 전용 390*844 비율과 데스크톱 1440*1024 비율을 각각 적용했습니다. */}
      <section className="relative w-full aspect-[390/844] md:aspect-[1440/1024] overflow-hidden bg-black selection:bg-black/80 selection:text-white">
        {/* 배경 이미지: 화면을 꽉 채우도록 object-cover 유지 */}
        <img 
          src={ARCHIVE_DATA[0].image} 
          alt="Architectural Facade" 
          className="absolute inset-0 w-full h-full object-cover opacity-70 scale-105"
        />
        
        {/* 💡 T Factory 로고: 
            모바일 시안과 동일하게 왼쪽 하단에 배치하고, 
            데스크톱보다 모바일에서 상대적으로 로고가 더 잘 보이도록 크기(h-14)를 키웠습니다. */}
        <motion.img
          src={tFactoryHeaderLogo}
          alt="T Factory Logo"
          initial={{ opacity: 0, y: 30 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 1.5, ease: [0.22, 1, 0.36, 1] }}
          className="absolute left-8 bottom-12 md:left-12 md:bottom-12 h-14 md:h-16 w-auto object-contain z-20"
        />
      </section>
      {/* 표지 섹션 끝 */}

      <div className="flex flex-col gap-0">
        {ARCHIVE_DATA.slice(1).map((section) => {
          if (section.type === "floorplan") {
            return (
              <FloorPlanSection 
                key={section.id} 
                activeFloorId={activeFloorId} 
                setActiveFloorId={setActiveFloorId} 
              />
            );
          }
          if (section.type === "details") {
            return (
              <SpaceDetailSection 
                key={section.id} 
                activeFloorId={activeFloorId} 
              />
            );
          }
          return null;
        })}
      </div>

      {/* 하단 푸터 섹션 (mt-24 md:mt-36 마진 탑 배치 완료) */}
      <footer className="mt-24 md:mt-36 bg-[#EFEFEF] py-16 px-6 md:px-12 text-black font-sans w-full text-left">
        <div className="w-full flex flex-col gap-12">
          <div>
            <img src={tFactoryFooterLogo} alt="T Factory Seongsu" className="h-14 md:h-16 w-auto object-contain" />
          </div>
          <div className="flex flex-col gap-4 text-[14px] md:text-[15px] font-normal leading-relaxed md:leading-tight text-[#1a1a1a]">
            <div className="flex flex-col gap-1.5">
              <p>T Factory 성수는 여백 없는 성수에서 여유로운 휴식과 즐거운 경험을 채우는 SK텔레콤의 브랜드 체험 공간입니다.</p>
              <p>잠시 쉬어가고 싶을 때, 새로운 재미가 필요할 때 언제든 T Factory 성수에 들러 주세요.</p>
            </div>
            <div className="flex flex-col gap-1.5 mt-2">
              <p>T Factory Seongsu is a brand experience space by SK Telecom where you can find relaxing comfort and enjoyable experiences in the heart of crowded Seongsu.</p>
              <p>Whether you're looking for a place to rest for a while or seeking something fresh and fun, T Factory Seongsu is always open for you.</p>
            </div>
          </div>
          <div className="text-[14px] md:text-[15px] font-normal text-[#1a1a1a] -mt-6">
            <span>오시는 길</span>
            <span className="mx-2 md:mx-3 text-[#1a1a1a]/30">|</span>
            <span>서울특별시 성수동 연무장1길 7-1 T 팩토리 성수</span>
          </div>
          <div className="flex flex-col gap-2 pt-8 text-[12px] md:text-[13px] text-[#888888]">
            <div className="font-medium">
              Copyright @ SK TELECOM., LTD
            </div>
            <div className="text-[#888888] font-normal flex flex-wrap gap-x-2 gap-y-1 items-center">
              <span>상호 에스케이텔레콤(주)</span>
              <span className="text-black/15">|</span>
              <span>대표이사 정재헌</span>
              <span className="text-black/15">|</span>
              <span>사업자등록번호 104-81-37225</span>
              <span className="text-black/15">|</span>
              <span>판매허가번호 2004-서울중구-2923</span>
              <span className="text-black/15">|</span>
              <span>주소 서울특별시 중구 을지로 65</span>
            </div>
          </div>
        </div>
      </footer>
    </main>
  );
}

function FloorPlanSection({ activeFloorId, setActiveFloorId }: any) {
  const [hoveredHotspotId, setHoveredHotspotId] = useState<string | null>(null);
  const activeFloor = FLOORS_DATA.find((f) => f.id === activeFloorId) || FLOORS_DATA[2];

  const getFilterStyle = (id: string) => {
    switch (id) {
      case "garden": return "brightness-[1.02] contrast-[1.0] hue-rotate-[10deg] saturate-[1.1]";
      case "basement": return "brightness-[0.98] contrast-[1.1] saturate-[0.8]";
      case "second_floor": return "rotate-[0.2deg] brightness-[1.0] contrast-[1.02]";
      case "rooftop": return "brightness-[1.03] opacity-[0.95] contrast-[0.95]";
      default: return "";
    }
  };

  return (
    // 💡 모바일에서는 aspect 비율을 해제하여(h-auto) 콘텐츠가 세로로 넉넉히 들어갈 공간을 확보합니다.
    <section className="relative w-full h-auto md:aspect-[1440/1024] bg-white flex flex-col pt-12 md:pt-24 pb-12 md:pb-12 px-6 md:px-8 font-sans overflow-hidden">
      
      {/* 💡 모바일(기본)에서는 flex-col로 위아래로 떨어뜨리고, 데스크톱(md:)에서만 기존의 12컬럼 그리드로 바꿉니다. */}
      <div className="flex flex-col md:grid md:grid-cols-12 gap-8 md:gap-4 items-center w-full h-full relative">
        
        {/* [1. 층수 메뉴] 
            💡 모바일(기본)에서는 flex-col로 세로 나열하고 items-center로 중앙 정렬합니다.
            💡 데스크톱(md:) 환경에서는 기존처럼 왼쪽 정렬(md:items-start)로 유연하게 바뀝니다. */}
        <div className="w-full md:w-auto md:col-span-1 flex flex-col md:flex-col items-center md:items-start justify-center md:justify-start gap-3 md:gap-5 text-[13px] md:text-[15px] select-none relative z-20 pl-0 md:pl-2 whitespace-nowrap">
          {FLOORS_DATA.map((fl) => {
            const isActive = fl.id === activeFloorId;
            return (
              <div key={fl.id} className="relative w-fit">
                <span 
                  onClick={() => {
                    setActiveFloorId(fl.id);
                    setHoveredHotspotId(null);
                  }}
                  className={`transition-colors duration-300 cursor-pointer text-sm md:text-base tracking-tight py-0.5 block ${
                    isActive 
                      ? "text-black font-bold" 
                      : "text-gray-300 font-semibold hover:text-black"
                  }`}
                >
                  {fl.name}
                </span>
              </div>
            );
          })}
        </div>

        {/* [2. 중앙 도면 이미지] 모바일에서도 가로 폭을 꽉 채우고 고유 비율 유지 */}
        <div className="w-full aspect-[4/3] md:aspect-auto md:h-full md:col-span-10 flex flex-col items-center justify-center py-2 md:py-6 relative z-10">
          <div className="relative w-full h-full max-w-[1550px] overflow-hidden select-none bg-white">
            <motion.img 
              key={activeFloorId}
              src={firstFloorImage} 
              alt={`${activeFloor.name} Plan`} 
              className={`w-full h-full object-contain transition-all duration-700 ${getFilterStyle(activeFloorId)}`}
              initial={{ opacity: 0.8, scale: 0.99 }}
              animate={{ opacity: 1, scale: 1 }}
              transition={{ duration: 0.5 }}
            />

            {activeFloor.hotspots.map((spot) => {
              const isHovered = hoveredHotspotId === spot.id;
              return (
                <div
                  key={spot.id}
                  className="absolute cursor-pointer"
                  style={{ left: `${spot.x}%`, top: `${spot.y}%`, width: `${spot.w}%`, height: `${spot.h}%` }}
                  onMouseEnter={() => setHoveredHotspotId(spot.id)}
                  onMouseLeave={() => setHoveredHotspotId(null)}
                >
                  <div className={`w-full h-full flex items-center justify-center transition-all duration-300 border ${
                      isHovered ? "bg-gray-200/80 border-black/10 shadow-sm" : "bg-transparent border-transparent"
                    }`}>
                    <span className={`text-[10px] md:text-[11px] font-bold text-black tracking-tight text-center px-1 transition-opacity duration-300 select-none ${
                        isHovered ? "opacity-100" : "opacity-0"
                      }`}>
                      {spot.name}
                    </span>
                  </div>
                </div>
              );
            })}
          </div>
        </div>

        {/* [3. 우측 공간명 라벨] 모바일에서는 맨 아래 중앙 / 데스크톱에서는 우측 끝 정렬 */}
        <div className="w-full md:col-span-1 flex justify-center md:justify-end select-none relative z-20 whitespace-nowrap pr-0 md:pr-2 pt-2 md:pt-0">
          <motion.h2 
            key={activeFloorId}
            initial={{ opacity: 0, y: 10 }}
            animate={{ opacity: 1, y: 0 }}
            transition={{ duration: 0.6, ease: [0.22, 1, 0.36, 1] }}
            className="text-sm md:text-base font-bold tracking-tight text-black text-center md:text-right"
          >
            {activeFloor.label}
          </motion.h2>
        </div>

      </div>
    </section>
  );
}

function SpaceDetailSection({ activeFloorId }: any) {
  const activeFloor = FLOORS_DATA.find((f) => f.id === activeFloorId) || FLOORS_DATA[2];
  const spaces = activeFloor.spaces || [];

  const [index, setIndex] = useState(0);

  useEffect(() => {
    setIndex(0);
  }, [activeFloorId]);

  if (spaces.length === 0) return null;
  const current = spaces[index] || spaces[0];

  const goPrev = () => setIndex((prev: number) => (prev > 0 ? prev - 1 : spaces.length - 1));
  const goNext = () => setIndex((prev: number) => (prev + 1) % spaces.length);

  return (
    <section className="py-0 flex flex-col items-center bg-white">
      <div className="w-full flex flex-col gap-0">
        <div className="relative aspect-[1440/1024] overflow-hidden group">
          <AnimatePresence mode="wait">
            <motion.img
              key={current.id}
              id={current.id}
              src={current.image}
              alt={current.name}
              initial={{ opacity: 0, scale: 1.02 }}
              animate={{ opacity: 1, scale: 1 }}
              exit={{ opacity: 0, scale: 0.98 }}
              transition={{ duration: 0.5, ease: [0.22, 1, 0.36, 1] }}
              className="w-full h-full object-cover"
            />
          </AnimatePresence>
          
          {spaces.length > 1 && (
            <div className="absolute inset-x-12 top-1/2 -translate-y-1/2 flex justify-between pointer-events-none opacity-0 group-hover:opacity-100 transition-opacity duration-500">
              <button onClick={(e) => { e.stopPropagation(); goPrev(); }} className="w-16 h-16 bg-black/40 backdrop-blur-md rounded-full flex items-center justify-center text-white pointer-events-auto hover:bg-black/60 transition-all scale-90 hover:scale-100 shadow-xl">
                <ArrowLeft strokeWidth={1} />
              </button>
              <button onClick={(e) => { e.stopPropagation(); goNext(); }} className="w-16 h-16 bg-black/40 backdrop-blur-md rounded-full flex items-center justify-center text-white pointer-events-auto hover:bg-black/60 transition-all scale-90 hover:scale-100 shadow-xl">
                <ArrowRight strokeWidth={1} />
              </button>
            </div>
          )}
        </div>

        {/* 💡 텍스트 가로 그리드 및 모바일 세로 1줄 레이아웃 짝 맞춤 완료 구역 */}
        <div className="px-6 md:px-12 pt-8 md:pt-12 pb-16 md:pb-20 w-full overflow-hidden">
          <AnimatePresence mode="wait">
             <motion.div 
               key={current.id}
               initial={{ opacity: 0, y: 15 }}
               animate={{ opacity: 1, y: 0 }}
               exit={{ opacity: 0, y: -15 }}
               transition={{ duration: 0.3, ease: [0.22, 1, 0.36, 1] }}
               className="flex flex-col md:grid md:grid-cols-12 gap-6 md:gap-8 items-start"
             >
              <div className="w-full md:col-span-3">
                <h3 className="text-lg md:text-xl font-bold tracking-tight text-black">
                  {current.name}
                </h3>
              </div>

              <div className="w-full md:col-span-9 flex flex-col gap-5 md:gap-6">
                {/* 첫 번째 줄 (카테고리 및 본문) */}
                <div className="flex flex-col md:grid md:grid-cols-3 gap-2 md:gap-8 items-start">
                  <span className="text-sm md:text-base font-medium text-gray-400 md:-ml-16">
                    {current.category}
                  </span>
                  <div className="md:col-span-2 md:col-start-2">
                    <p className="text-xs md:text-sm font-normal text-black leading-relaxed tracking-wide whitespace-pre-line">
                      {current.description}
                    </p>
                  </div>
                </div>

                {/* 두 번째 줄 (추가 정보 및 칼정렬 회색 선) */}
                {current.extraInfo && (
                  <>
                    <div className="grid grid-cols-1 md:grid-cols-3 gap-8 my-2">
                      <div className="md:col-span-3 md:-ml-16">
                        <div className="w-full h-px bg-gray-200" />
                      </div>
                    </div>
                    
                    <div className="flex flex-col md:grid md:grid-cols-3 gap-2 md:gap-8 items-start">
                      <span className="text-sm md:text-base font-medium text-gray-400 md:-ml-16">
                        {current.extraInfo.category}
                      </span>
                      <div className="md:col-span-2 md:col-start-2">
                        <p className="text-xs md:text-sm font-normal text-black leading-relaxed tracking-wide whitespace-pre-line">
                          {current.extraInfo.description}
                        </p>
                      </div>
                    </div>
                  </>
                )}
              </div>
            </motion.div>
          </AnimatePresence>
        </div>
      </div>
    </section>
  );
}
