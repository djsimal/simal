#include "imgui/imgui.h"
//#include <KittyMemory/Kitty.h>
#include "imgui/backends/imgui_impl_android.h"
#include "imgui/backends/imgui_impl_opengl3.h"
#include <Helper/define.h>
#include "Helper/Iconcpp.h"
#include "Helper/ImguiPP.h"
#include "Helper/Menu.h"
#include "Helper/Font.h"
#include "Helper/Icon.h"
#include "Helper/fake_dlfcn.h"
#include "Helper/Includes.h"
#include "Helper/plthook.h"
#include "Helper/json.hpp"
#include "Helper/StrEnc.h"
#include <android/keycodes.h>
#include <android/native_activity.h>

// first include font
#include "font3.h"
ImFont* flamee;
float FONT_SIZE_FACTOR = 15.0f;
static float isRed = 0.0f, isGreen = 0.01f, isBlue = 0.0f;
#include "Helper/Spoof.h"
#include "Helper/Tools.h"
#include "Helper/obfuscate.h"
#include "Helper/Dobby/dobby.h"
#include "Helper/font/segue_font.h"
#include "Helper/font/ico_font.h"
#include "Helper/font/LoginFont.h"
#include "Helper/font/LoginIcon.h"
#include "Helper/font/iicon.h"
#include "Helper/font/Ske.h"
#include "Helper/font/Oont.h"
#include "Helper/Item.h"
#include "Helper/Items.h"
#include "Helper/Itemsmg.h"
#include "Helper/ItemSni.h"
#include "Helper/Itemsammo.h"
#include "Helper/Itemsmag.h"
#include "Helper/Itemscope.h"
#include "Helper/Heal.h"
#include "Helper/Vector3.hpp"
#include "Helper/ElfImg.h"
#include "KittyMemory/MemoryPatch.h"
#include "foxcheats/include/ScanEngine.hpp"
#include "MemoryTools.h"
#include "Substrate/SubstrateHook.h"
#include "base64/base64.h"
#include "SDK.hpp"
#include "Rect.h"
#include "HOOK.h"
#include "Includes/Logger.h"
//#include "Includes/Utils.h"
//#include "Includes/Macros.h"
#include "Iteem.h"
//#include "Geometry.h"
#include "imgui/XMAS.h"
#include "imgui/gradient.h"
#include "imgui/stb_image.h"
#include "imgui/imgui_headers.h"
#include "imgui/imgui_internal.h"
#include "Image/Loader.h"
#include "Android_App.h"
#include <vector>
#include <random>
#include <math.h>
std::vector<ImVec2> circles_pos;
std::vector<ImVec2> circles_dir;
std::vector<int> circles_radius;
using namespace SPra;
#include <cstring>
#include <string.h>
bool Logo = true;
float accent_color[4] = { 0.300f, 0.220f, 0.750f, 1.000f };
#include <curl/curl.h>
#include <openssl/rsa.h>
#include <openssl/pem.h>
using namespace SDK;
using json = nlohmann::json;
int gScreenWidth;
int gScreenHeight;
#define STB_IMAGE_IMPLEMENTATION
//float inttouchx = 30, inttouchy = 60;
// ======================================================================== //
#include <curl/curl.h>
#include <openssl/evp.h>
#include <openssl/pem.h>
#include <openssl/rsa.h>
#include <openssl/err.h>
#include <openssl/md5.h>

#include <hook/hook.h>
#define targetLibName OBFUSCATE("libanort.so")
static bool WantTextInputLast = false;

inline bool FileExist(const std::string& name) {
    if (FILE* file = fopen(name.c_str(), "r")) {
        fclose(file);
        return true;
    }
    else {
        return false;
    }
}

DWORD libue4header = 0x0;
DWORD libanogsheader = 0x0;
DWORD libgcloudheader = 0x0;

//ProcMap g_Handle;

struct  MemTrap_t {
    uintptr_t baseAddr;
    uintptr_t endAddr;
};

std::vector<MemTrap_t> MemTraps = std::vector<MemTrap_t>();

bool IsObjectInvalid(UObject* pObject) {
    if (pObject == 0)
        return true;

    for (auto& i : MemTraps) {
        if ((uintptr_t)pObject >= i.baseAddr && (uintptr_t)pObject <= i.endAddr) {
            return true;
        }
    }
    return false;
}
float AimSpeed = 15.0f; // Daha yavaş bir nişan alma hızı
float SpeedAim = 15.0f; // Daha yavaş bir nişan alma hızı
extern long libbase;
extern long GWorld;
extern long GNames;
static float tm = 127 / 255.f;
#define targetLibName OBFUSCATE("libanort.so")
ImFont* ico = nullptr;
ImFont* ico_combo = nullptr;
ImFont* ico_button = nullptr;
ImFont* ico_grande = nullptr;
ImFont* segu = nullptr;
ImFont* default_segu = nullptr;
ImFont* bold_segu = nullptr;
ImFont* logoicon = nullptr;
ImFont* logoicon2 = nullptr;
ImFont* bold = nullptr;
ImFont* bankai = nullptr;
ImFont* ico_default = nullptr;
ImFont* basic = nullptr;
bool initImGui = false;
static int xsuit = 0;
static int skinm4 = 0;
static int skinakm = 0;
static int skinscar = 0;
static int skinm7 = 0;
static int skinuzi = 0;
static int skinump45 = 0;
static int skinvector = 0;
static int skinbizon = 0;
static int skingroza = 0;
static int skinkar = 0;
static int skinm24 = 0;
static int skinawm = 0;
static int skindp28 = 0;
static int skinqbz = 0;
static int skinm16a4 = 0;
static int skinm249 = 0;
static int skinmini14 = 0;
static int skinslr = 0;
static int skinsks = 0;
static int skinpan = 0;
static int skins1897 = 0;
static int skinvss = 0;
static int skins12k = 0;
static int skinaug = 0;
static int skinmk14 = 0;
//=============//
static int Hair11 = 0;
static int skinsace32 = 0;
static int skinxsuit = 0;
static int modm4 = 0;
static int modakm = 0;
static int modscar = 0;
static int modm7 = 0;
static int moduzi = 0;
static int modump45 = 0;
static int modvector = 0;
static int modbizon = 0;
static int modgroza = 0;
static int modkar = 0;
static int modm24 = 0;
static int modawm = 0;
static int moddp28 = 0;
static int modqbz = 0;
static int modm16a4 = 0;
static int modm249 = 0;
static int modmini14 = 0;
static int modslr = 0;
static int modsks = 0;
static int modpan = 0;
static int mods1897 = 0;
static int modvss = 0;
static int mods12k = 0;
static int modaug = 0;
static int modmk14 = 0;
static int skinbg = 0;
static int skinhmm = 0;
static int skinmyth = 0;
static int skinfool = 0;
//=================//
static int Efm4 = 0;
static int Efscar = 0;
static int Efaug = 0;
static int Efakm = 0;
static int Efface = 0;
static int EfHair = 0;
int screenWidth = -1, glWidth, screenHeight = -1, glHeight;
float density = -1;
json items_data;
json items_data_r;
json items_data_sm;
json items_data_sn;
json items_data_h;
json items_data_ammo;
json items_data_mag;
json items_data_scop;
time_t rng = 0;
std::string expiretime = "";
std::string g_Token, g_Auth;
bool bValid = false;
bool KEROB = true;
#define SLEEP_TIME 1000LL / 120LL
uintptr_t tersafe;
static char s[64];
char extra[32];
bool down;
//std::vector<Snowflake::Snowflake> Snow;
// ======================================================================== //
#define DefineHook(RET, NAME, ARGS) \
	RET(*Orig_##NAME)               \
	ARGS;                           \
	RET Hook_##NAME ARGS
bool WriteAddr(void* addr, void* buffer, size_t length) {
    unsigned long page_size = sysconf(_SC_PAGESIZE);
    unsigned long size = page_size * sizeof(uintptr_t);
    return mprotect((void*)((uintptr_t)addr - ((uintptr_t)addr % page_size) - page_size), (size_t)size, PROT_EXEC | PROT_READ | PROT_WRITE) == 0 && memcpy(addr, buffer, length) != 0;
}

enum EAim {
    Distance = 0,
    Croshhair = 1
};

enum EAimTarget {
    Auto = 0,
    Chest = 2
};

//enum EAimTrigger {
//    Any = 0,
//    Shooting = 1,
//    Scoping = 2,
//    Both = 3,
//    None = 4
//};

enum EAimTrigger {
    Shooting,
    None,
    Scoping,
    Both,
    Any
};
enum Em416 {
    nom4 = 0,
    m4gc = 1,
    m4fool = 2,
    m4lizard = 3,

};

struct sConfig {

    bool Antiban2;
    bool Logo;

    //Functions
    bool Line = true;
    bool Box = true;
    bool P_Weapon = true;
    bool Hp = true;
    bool Name = true;
    bool Bone = true;
    bool HitCount = true;
    bool Vehicle = true;
    bool V_Hp = true;
    bool V_3d = true;
    bool V_Fuel = true;
    bool Alert360 = true;
    bool Hide_Bot = true;
    bool Distance = true;
    bool Team = true;
    bool Grenade = true;
    bool Bypass;
    bool GameInfo = true;
    bool LootItem = true;
    bool Loot = true;
    bool AirDrop = true;
    bool Fight = true;


    struct sAimMenu {
        bool Enable;
        bool AimBot;
        int Cross;
        float Recc;
        EAim By;
        EAimTarget Target;
        EAimTrigger Trigger;
        bool Pred;
        bool ReCo;
        bool IgnoreKnocked;
        bool VisCheck;
        bool IgnoreBots;
        bool TargetLine;
    };
    sAimMenu SilentAim{ 0 };
    sAimMenu AimBot{ 0 };
    struct sColorsESP
    {
        float* PVLine;
        float* Text;
        float* Menucolour;
        float* Line;
        float* Box;
        float* Boxbot;
        float* Name;
        float* Distance;
        float* Skeleton;
        float* Skeletonbot;
        float* Linebot;
        float* Count;
        float* Vehicle;
        float* Cross2;
        float* PVILine;
        float* BVLine;
        float* BVILine;
        float* PVBox;
        float* PVIBox;
        float* BVBox;
        float* BVIBox;
        float* PVSkeleton;
        float* PVISkeleton;
        float* BVSkeleton;
        float* BVISkeleton;
        float* TeamID;
        float* SkeletonVisible;
        float* Items;
        float* Fov;
    };
    sColorsESP ColorsESP{ 0 };
    struct sPlayerESP {
		  bool wide_view{ false };
         float set_field_of_view{ 70.f };
        bool WEAPON;
        bool ActiveEsp = true;
        bool DBox = true;
        bool KERO;
        bool Line1 = true;
        bool Box = true;
        bool Line2 = true;
        //	bool Box;
        bool 准心射线;
        bool Health = true;
        bool Skeleton = true;
        bool Name = true;
        bool Distance = true;
        bool TeamID = true;
        float Kiss;
        bool Vehicle = true;
        bool NoBot;
        bool RadarDraw;
        bool RadarDraw2;
        bool Radar1;
        bool Radar2;
        bool Radar3;
        bool Radar4;
        bool LootBox = true;
        bool Grenade = true;
        bool VehicleHP = true;
        bool VehicleFuel = true;
        bool Warning = true;
        bool WzCs;
        //	EEsp By;

    };
    // kero_200
    sPlayerESP PlayerESP{ 0 };
    int Skill1;
    int Skill3;
    int Skill4;
    int RadarY;
    int RadarX;
    bool Radar;
    bool TargetLine;
    int LootSizeitems;
    int LootSize;
    //size edit
    int L_size;
    int S_size;
    int Grenade_d;
    int Maters;
    int Materrs;
    struct MemoryHack {
        bool Xkill;
        bool killmessage;
        bool mc;
        bool xk;
        bool fs;
        bool ms;
        bool m416;
        bool m4sel;
        bool akm;
        bool carteleport;
        bool cartrack;
    };
    MemoryHack MemoryHacks{ 0 };
    //Colors
    float* B_non;
    float* B_vis;
    float* P_non;
    float* P_vis;
    float* VehicleS;
    float* VehicleColor;
    float* Fov;
};
sConfig Config{ 0 };

bool ShowMenu = true;
void processKeyEvent(AInputEvent* event) {
    int32_t keyCode = AKeyEvent_getKeyCode(event);
    switch (keyCode) {
    case AKEYCODE_INSERT:
        ShowMenu = !ShowMenu;
        break;
        // Handle other key codes as needed
    }
}
void AddTextName(const ImFont* font, float font_size, const ImVec2& pos, ImColor col, const char* text_begin, bool bCenter, bool bOutLine)
{
    ImVec2 TextSize = font->CalcTextSizeA(font_size, FLT_MAX, 0.0f, text_begin);
    if (bOutLine)
    {
        ImGui::GetForegroundDrawList()->AddText(font, font_size, ImVec2((bCenter ? pos.x - TextSize.x / 2.0f : pos.x) + 1.0f, pos.y + 1.0f), IM_COL32(0, 0, 0, 255), text_begin);
    }
    ImGui::GetForegroundDrawList()->AddText(font, font_size, ImVec2(bCenter ? pos.x - TextSize.x / 2.0f : pos.x, pos.y), col, text_begin);
}


std::map<int, bool> Items;
std::map<int, float*> ItemColors;

// ======================================================================== //
#define CREATE_COLOR(r, g, b, a) new float[4] {(float)r, (float)g, (float)b, (float)a};

//-------------------------------------------------------------------------------------------------------------------------------------//
uint32_t Colors[] = { 0x53BB0C, 0x530826, 0x0FC3F4, 0xDC2855, 0x0A31DE, 0xBAA7FD, 0xCEDB3F, 0x286A45, 0x58F014, 0x45CAE6, 0x773702, 0xB0CEF0, 0x3C5F51, 0x453CD7, 0x364024, 0x439997, 0x4CB612, 0xC6B564, 0x17F250, 0xE41BC0, 0xAF8E27, 0x8E382E, 0x47A101, 0x9DAC33, 0x66F4CF, 0x59A9F0, 0x798D1A, 0x2EBB59, 0xBF66C3, 0x4BD8FB, 0xBBFA54, 0x6B9881, 0x144967, 0xBAA3AE, 0xE80B9D, 0x7BA552, 0x96A456, 0x17D7B4, 0x130C39, 0x3C06A8, 0x62737E, 0xA87E89, 0xB6D3E4, 0x66B77D, 0x66E304, 0x1B80E1, 0x7A06BC, 0xBFFB1B, 0x618506, 0x7E4D34 };

long Random1(int index) {
    srand(index);

    int a = 255;
    int r = ((Colors[rand() % sizeof(Colors)] & 0xFF0000) >> 17);
    int g = ((Colors[rand() % sizeof(Colors)] & 0x00FF00) >> 9);
    int b = (Colors[rand() % sizeof(Colors)] & 0x0000FF);

    return IM_COL32(r, g, b, a);
}
long Random2(int index) {
    srand(index);

    int a = 130;
    int r = ((Colors[rand() % sizeof(Colors)] & 0xFF0000) >> 17);
    int g = ((Colors[rand() % sizeof(Colors)] & 0x00FF00) >> 9);
    int b = (Colors[rand() % sizeof(Colors)] & 0x0000FF);

    return IM_COL32(r, g, b, a);
}

// ======================================================================== //
uintptr_t anogs;
uintptr_t UE4;

uintptr_t g_cloud;


uintptr_t AimBullet_Offset;
uintptr_t GWorld_Offset, GUObjectArray_Offset, SilentAim_Offset;

android_app* g_App = 0;
ASTExtraPlayerCharacter* g_LocalPlayer = 0;
ASTExtraPlayerController* g_LocalController = 0;

// ======================================================================== //
//#define GNames_Offset 0x41b6030
//#define GEngine_Offset 0x8cf6cd8 //UEngine
//#define GEngine_Offset 0x93e3590 //UlocalPlayer
//#define GUObject_Offset 0x9582594
//#define GetActorArray 0x6072410
//#define Canvas_Map_Offset 0x93ed500
//#define ProcessEvent_Offset 0x566f134
//#define GNativeAndroidApp_Offset 0x8c5dbe8
//#define Actors_Offset 0x70


#define GNames_Offset  0x43a2070
#define GUObject_Offset 0x8e358f8
#define ProcessEvent_Offset 0x5a40edc
#define GNativeAndroidApp_Offset 0x8c5dbe8
#define GetActorArray 0x5EA6144

#define Actors_Offset : 0x70
// ======================================================================== //

//-------------------------------------------------------------------------------------------------------------------------------------//
void DrawBoxEnemy(ImDrawList* draw, ImVec2 X, ImVec2 Y, float thicc, int color) {
    draw->AddLine({ X.x, X.y }, { Y.x, Y.y }, color, thicc);
}
void DrawBoxEnemy(ImDrawList* draw, ImVec2 X, ImVec2 Y, float thicc, float rounding, int color) {
    draw->AddLine({ X.x, X.y }, { Y.x, Y.y }, color, thicc);
}
void DrawImage(int x, int y, int w, int h, ImTextureID Texture);

void DrawImage(int x, int y, int w, int h, ImTextureID Texture) {
    ImGui::GetBackgroundDrawList()->AddImage(Texture, ImVec2(x, y), ImVec2(x + w, y + h));
}

struct sRegion {
    uintptr_t start, end;
};

std::vector<sRegion> trapRegions;

bool isObjectInvalid(UObject* obj) {
    if (!Tools::IsPtrValid(obj)) {
        return true;
    }

    if (!Tools::IsPtrValid(obj->ClassPrivate)) {
        return true;
    }

    if (obj->InternalIndex <= 0) {
        return true;
    }

    if (obj->NamePrivate.ComparisonIndex <= 0) {
        return true;
    }

    if ((uintptr_t)(obj) % sizeof(uintptr_t) != 0x0 && (uintptr_t)(obj) % sizeof(uintptr_t) != 0x4) {
        return true;
    }

    if (std::any_of(trapRegions.begin(), trapRegions.end(), [obj](sRegion region) { return ((uintptr_t)obj) >= region.start && ((uintptr_t)obj) <= region.end; }) ||
        std::any_of(trapRegions.begin(), trapRegions.end(), [obj](sRegion region) { return ((uintptr_t)obj->ClassPrivate) >= region.start && ((uintptr_t)obj->ClassPrivate) <= region.end; })) {
        return true;
    }

    return false;
}


// ======================================================================== //
std::string getObjectPath(UObject* Object) {
    std::string s;
    for (auto super = Object->ClassPrivate; super; super = (UClass*)super->SuperStruct) {
        if (!s.empty())
            s += ".";
        s += super->NamePrivate.GetName();
    }
    return s;
}


// ======================================================================== //
static UFont* tslFont = 0, * robotoTinyFont = 0;

// ======================================================================== //
static UEngine* GEngine = 0;
UWorld* GetWorld() {
    while (!GEngine) {
        GEngine = UObject::FindObject<UEngine>("UAEGameEngine Transient.UAEGameEngine_1"); // Auto 
        sleep(1);
    }
    if (GEngine) {
        auto ViewPort = GEngine->GameViewport;

        if (ViewPort) {
            //return {};
            return ViewPort->World;
        }
    }
    return 0;
}
TNameEntryArray* GetGNames()
{
    return ((TNameEntryArray * (*)()) (UE4 + GNames_Offset))();
}

std::vector<AActor*> getActors() {
    auto World = GetWorld();
    if (!World)
        return std::vector<AActor*>();

    auto PersistentLevel = World->PersistentLevel;
    if (!PersistentLevel)
        return std::vector<AActor*>();

    struct GovnoArray {
        uintptr_t base;
        int32_t count;
        int32_t max;
    };
    static thread_local GovnoArray Actors{};

    Actors = *(((GovnoArray * (*)(uintptr_t))(UE4 + GetActorArray))(reinterpret_cast<uintptr_t>(PersistentLevel)));

    if (Actors.count <= 0) {
        return {};
    }

    std::vector<AActor*> actors;
    for (int i = 0; i < Actors.count; i++) {
        auto Actor = *(uintptr_t*)(Actors.base + (i * sizeof(uintptr_t)));
        if (Actor) {
            actors.push_back(reinterpret_cast<AActor* const>(Actor));
        }
    }
    return actors;
}
template<typename T>
void Write(uintptr_t addr, T value) {
    WriteAddr((void*)addr, &value, sizeof(T));
}
// ======================================================================== //
long GetRandomColorByIndex(int index) {
    srand(index);

    int a = 135;
    int r = ((Colors[rand() % sizeof(Colors)] & 0xFF0000) >> 16);
    int g = ((Colors[rand() % sizeof(Colors)] & 0x00FF00) >> 8);
    int b = (Colors[rand() % sizeof(Colors)] & 0x0000FF);

    return IM_COL32(r, g, b, a);
}

// ======================================================================== //

int32_t ToColor(float* col) {
    return ImGui::ColorConvertFloat4ToU32(*(ImVec4*)(col));
}
//==//
FRotator ToRotator(FVector local, FVector target) {
    FVector rotation = UKismetMathLibrary::Subtract_VectorVector(local, target);
    float hyp = sqrt(rotation.X * rotation.X + rotation.Y * rotation.Y);
    FRotator newViewAngle = { 0 };
    newViewAngle.Pitch = -atan(rotation.Z / hyp) * (180.f / (float)3.14159265358979323846);
    newViewAngle.Yaw = atan(rotation.Y / rotation.X) * (180.f / (float)3.14159265358979323846);
    newViewAngle.Roll = (float)0.f;
    if (rotation.X >= 0.f)
        newViewAngle.Yaw += 180.0f;
    return newViewAngle;
}

#define IM_PI                   3.14159265358979323846f
#define RAD2DEG( x )  ( (float)(x) * (float)(180.f / IM_PI) )
#define DEG2RAD( x ) ( (float)(x) * (float)(IM_PI / 180.f) )

FVector WorldToRadar(float Yaw, FVector Origin, FVector LocalOrigin, float PosX, float PosY, Vector3 Size, bool& outbuff) {
    bool flag = false;
    double num = (double)Yaw;
    double num2 = num * 0.017453292519943295;
    float num3 = (float)std::cos(num2);
    float num4 = (float)std::sin(num2);
    float num5 = Origin.X - LocalOrigin.X;
    float num6 = Origin.Y - LocalOrigin.Y;
    struct FVector Xector;
    Xector.X = (num6 * num3 - num5 * num4) / 150.f;
    Xector.Y = (num5 * num3 + num6 * num4) / 150.f;
    struct FVector Xector2;
    Xector2.X = Xector.X + PosX + Size.X / 2.f;
    Xector2.Y = -Xector.Y + PosY + Size.Y / 2.f;
    bool flag2 = Xector2.X > PosX + Size.X;
    if (flag2) {
        Xector2.X = PosX + Size.X;
    }
    else {
        bool flag3 = Xector2.X < PosX;
        if (flag3) {
            Xector2.X = PosX;
        }
    }
    bool flag4 = Xector2.Y > PosY + Size.Y;
    if (flag4) {
        Xector2.Y = PosY + Size.Y;
    }
    else {
        bool flag5 = Xector2.Y < PosY;
        if (flag5) {
            Xector2.Y = PosY;
        }
    }
    bool flag6 = Xector2.Y == PosY || Xector2.X == PosX;
    if (flag6) {
        flag = true;
    }
    outbuff = flag;
    return Xector2;
}
void VectorAnglesRadar(Vector3& forward, FVector& angles) {
    if (forward.X == 0.f && forward.Y == 0.f) {
        angles.X = forward.Z > 0.f ? -90.f : 90.f;
        angles.Y = 0.f;
    }
    else {
        angles.X = RAD2DEG(atan2(-forward.Z, forward.Magnitude(forward)));
        angles.Y = RAD2DEG(atan2(forward.Y, forward.X));
    }
    angles.Z = 0.f;
}

void RotateTriangle(std::array<Vector3, 3>& points, float rotation) {
    const auto points_center = (points.at(0) + points.at(1) + points.at(2)) / 3;
    for (auto& point : points) {
        point = point - points_center;
        const auto temp_x = point.X;
        const auto temp_y = point.Y;
        const auto theta = DEG2RAD(rotation);
        const auto c = cosf(theta);
        const auto s = sinf(theta);
        point.X = temp_x * c - temp_y * s;
        point.Y = temp_x * s + temp_y * c;
        point = point + points_center;
    }
}

#define W2S(w, s) UGameplayStatics::ProjectWorldToScreen(localController, w, true, s)
//=====Aiming======//
bool isInsideFOV(int x, int y) {
    if (!Config.SilentAim.Cross)
        return true;
    int circle_x = glWidth / 2;
    int circle_y = glHeight / 2;
    int rad = Config.SilentAim.Cross * 0.5f;
    return (x - circle_x) * (x - circle_x) + (y - circle_y) * (y - circle_y) <= rad * rad;
}
auto GetTargetByCrossDist() {
    ASTExtraPlayerCharacter* result = 0;
    float max = std::numeric_limits<float>::infinity();

    auto Actors = getActors();

    auto localPlayer = g_LocalPlayer;
    auto localController = g_LocalController;
    FVector ViewPosY{ 0, 0, 0 };
    if (localPlayer) {
        ViewPosY = localPlayer->GetBonePos("Head", {});
        ViewPosY.Z += 10.f;
    }
    if (localPlayer) {
        for (int i = 0; i < Actors.size(); i++) {
            auto Actor = Actors[i];
            if (isObjectInvalid(Actor))
                continue;

            if (Actor->IsA(ASTExtraPlayerCharacter::StaticClass())) {
                auto Player = (ASTExtraPlayerCharacter*)Actor;
                auto Target = (ASTExtraPlayerCharacter*)Actor;
                float dist = localPlayer->GetDistanceTo(Target) / 150.0f;
                if (dist > Config.Maters)
                    continue;

                if (Player->PlayerKey == localPlayer->PlayerKey)
                    continue;

                if (Player->TeamID == localPlayer->TeamID)
                    continue;

                if (Player->bDead)
                    continue;

                if (Config.SilentAim.IgnoreKnocked) {
                    if (Player->Health == 0.0f)
                        continue;
                }

                if (Config.SilentAim.VisCheck) {
                    if (!localController->LineOfSightTo(Player, ViewPosY, true))
                        continue;
                }
                if (Config.SilentAim.IgnoreBots) {
                    if (Player->bEnsure)
                        continue;
                }

                auto Root = Player->GetBonePos("Root", {});
                auto Head = Player->GetBonePos("Head", {});

                FVector2D RootSc, HeadSc;
                if (W2S(Root, &RootSc) && W2S(Head, &HeadSc)) {
                    float height = abs(HeadSc.Y - RootSc.Y);
                    float width = height * 0.65f;

                    FVector middlePoint = { HeadSc.X + (width / 2), HeadSc.Y + (height / 2), 0 };
                    if ((middlePoint.X >= 0 && middlePoint.X <= glWidth) && (middlePoint.Y >= 0 && middlePoint.Y <= glHeight)) {
                        FVector2D v2Middle = FVector2D((float)(glWidth / 2), (float)(glHeight / 2));
                        FVector2D v2Loc = FVector2D(middlePoint.X, middlePoint.Y);
                        if (isInsideFOV((int)middlePoint.X, (int)middlePoint.Y)) {
                            float dist = FVector2D::Distance(v2Middle, v2Loc);

                            if (dist < max) {
                                max = dist;
                                result = Player;
                            }
                        }
                    }
                }
            }
        }
    }

    return result;
}
auto GetTargetForAiming() {
    ASTExtraPlayerCharacter* result = 0;
    float max = std::numeric_limits<float>::infinity();

    auto Actors = getActors();

    auto localPlayer = g_LocalPlayer;
    auto localController = g_LocalController;
    FVector ViewPosY{ 0, 0, 0 };
    if (localPlayer) {
        ViewPosY = localPlayer->GetBonePos("Head", {});
        ViewPosY.Z += 10.f;
    }
    if (localPlayer) {
        for (int i = 0; i < Actors.size(); i++) {
            auto Actor = Actors[i];
            if (isObjectInvalid(Actor))
                continue;
            if (Actor->IsA(ASTExtraPlayerCharacter::StaticClass())) {
                auto Player = (ASTExtraPlayerCharacter*)Actor;
                auto Target = (ASTExtraPlayerCharacter*)Actor;

                float dist = localPlayer->GetDistanceTo(Target) / 150.0f;
                if (dist > Config.Materrs)
                    continue;
                if (Player->PlayerKey == localPlayer->PlayerKey)
                    continue;
                if (Player->TeamID == localPlayer->TeamID)
                    continue;
                if (Player->bDead)
                    continue;

                if (Config.SilentAim.IgnoreKnocked) {
                    if (Player->Health == 0.0f)
                        continue;
                }

                if (Config.SilentAim.VisCheck) {
                    if (!localController->LineOfSightTo(Player, ViewPosY, true))
                        continue;
                }

                if (Config.SilentAim.IgnoreBots) {
                    if (Player->bEnsure)
                        continue;
                }
                auto Root = Player->GetBonePos("Root", {});
                auto Head = Player->GetBonePos("Head", {});
                FVector2D RootSc, HeadSc;
                if (W2S(Root, &RootSc) && W2S(Head, &HeadSc)) {
                    float height = abs(HeadSc.Y - RootSc.Y);
                    float width = height * 0.65f;
                    FVector middlePoint = { HeadSc.X + (width / 2), HeadSc.Y + (height / 2), 0 };
                    if ((middlePoint.X >= 0 && middlePoint.X <= glWidth) && (middlePoint.Y >= 0 && middlePoint.Y <= glHeight)) {
                        FVector2D v2Middle = FVector2D((float)(glWidth / 2), (float)(glHeight / 2));
                        FVector2D v2Loc = FVector2D(middlePoint.X, middlePoint.Y);
                        if (isInsideFOV((int)middlePoint.X, (int)middlePoint.Y)) {
                            float dist = FVector2D::Distance(v2Middle, v2Loc);
                            if (dist < max) {
                                max = dist;
                                result = Player;
                            }
                        }
                    }
                }
            }
        }
    }

    return result;
}

// ======================================================================== //
bool deadbox1;

static int skinThompson = 0;
void* (*oProcessEvent)(UObject* pObj, UFunction* pFunc, void* pArgs);
void* hkProcessEvent(UObject* pObj, UFunction* pFunc, void* pArgs) {
    //LOGI("CALLED {%s} FUN {%s} ",pObj->GetFullName().c_str(),pFunc->GetFullName().c_str());
    auto LocalPlayer = g_LocalPlayer;







    if (deadbox1)
    {
        if (strstr((const char*)pFunc->GetFullName().c_str(), "BackpackBlueprintUtils_BP.BackpackBlueprintUtils_BP_C.CreateBattleItemHandle") || strstr((const char*)pFunc->GetFullName().c_str(), "CreateWeaponAndChangeSkin") || strstr((char*)pFunc->GetFullName().c_str(), "BackpackBlueprintUtils_BP.BackpackBlueprintUtils_BP_C.GetWeaponSkinMappingID") || strstr((char*)pFunc->GetFullName().c_str(), "BackpackBlueprintUtils_BP.BackpackBlueprintUtils_BP_C.ModifySetting")) {
            ULobbyWeaponManagerComponent_CreateWeaponAndChangeSkin_Params* PARAMS = (ULobbyWeaponManagerComponent_CreateWeaponAndChangeSkin_Params*)pArgs;
            auto GWorld = GetWorld();
            ASTExtraPlayerController* localController = (ASTExtraPlayerController*)GWorld->NetDriver->ServerConnection->PlayerController;
            ASTExtraPlayerCharacter* localPlayer = (ASTExtraPlayerCharacter*)localController->AcknowledgedPawn;
            std::string strWeaponId = std::to_string((int)PARAMS->WeaponSkinID);
            if (strstr(strWeaponId.c_str(), "101004")) {

                if (skinm4 == 1)

                    PARAMS->WeaponSkinID = 1101004046; //Glacier - M416 
                if (skinm4 == 2)
                    PARAMS->WeaponSkinID = 1101004062; //Glacier - M416 
                if (skinm4 == 3)
                    PARAMS->WeaponSkinID = 1101004086; //Glacier - M416 
                if (skinm4 == 4)
                    PARAMS->WeaponSkinID = 1101004078; //Glacier - M416 
                if (skinm4 == 5)
                    PARAMS->WeaponSkinID = 1101004098; //Glacier - M416 
                if (skinm4 == 9)
                    PARAMS->WeaponSkinID = 1101004218; //Glacier - M416 
                if (skinm4 == 6)
                    PARAMS->WeaponSkinID = 1101004163; //Glacier - M416 
                if (skinm4 == 7)
                    PARAMS->WeaponSkinID = 1101004201; //Glacier - M416 
                if (skinm4 == 8)
                    PARAMS->WeaponSkinID = 1101004138; //Glacier - M416 
                if (skinm4 == 10)
                    PARAMS->WeaponSkinID = 1101004209; //Glacier - M416 
            }

            if (strstr(strWeaponId.c_str(), "205002"))// Config.M416_Tactical_stock
            {
                if (skinm4 == 1)
                    PARAMS->WeaponSkinID = 1010040443; //Glacier - M416 
                else if (skinm4 == 2)
                    PARAMS->WeaponSkinID = 1010040623; //The Fool - M416
                else if (skinm4 == 3)
                    PARAMS->WeaponSkinID = 1010040863; //Lizard Roar - M416
                else if (skinm4 == 4)
                    PARAMS->WeaponSkinID = 1010040783; //Wanderer - M416
                else if (skinm4 == 5)
                    PARAMS->WeaponSkinID = 1010040983; //Call of the Wild - M416
                else if (skinm4 == 6)
                    PARAMS->WeaponSkinID = 1010041633; //Imperial Splendor - M416
                else if (skinm4 == 7)
                    PARAMS->WeaponSkinID = 1010042013; //Silver Guru - M416
                else if (skinm4 == 8)
                    PARAMS->WeaponSkinID = 1010041383; //TechnoCore - M416
                else if (skinm4 == 9)
                    PARAMS->WeaponSkinID = 1010042093; //Tidal Embrace - M416
                else if (skinm4 == 10)
                    PARAMS->WeaponSkinID = 1010042183; //Shinobi Kami - M416

            }

            if (strstr(strWeaponId.c_str(), "205005"))// M416_default_stock
            {
                if (skinm4 == 1)
                    PARAMS->WeaponSkinID = 1010040443; //Glacier - M416 
                else if (skinm4 == 2)
                    PARAMS->WeaponSkinID = 1010040623; //The Fool - M416
                else if (skinm4 == 3)
                    PARAMS->WeaponSkinID = 1010040863; //Lizard Roar - M416
                else if (skinm4 == 4)
                    PARAMS->WeaponSkinID = 1010040783; //Wanderer - M416
                else if (skinm4 == 5)
                    PARAMS->WeaponSkinID = 1010040983; //Call of the Wild - M416
                else if (skinm4 == 6)
                    PARAMS->WeaponSkinID = 1010041633; //Imperial Splendor - M416
                else if (skinm4 == 7)
                    PARAMS->WeaponSkinID = 1010042013; //Silver Guru - M416
                else if (skinm4 == 8)
                    PARAMS->WeaponSkinID = 1010041383; //TechnoCore - M416
                else if (skinm4 == 9)
                    PARAMS->WeaponSkinID = 1010042093; //Tidal Embrace - M416
                else if (skinm4 == 10)
                    PARAMS->WeaponSkinID = 1010042183; //Shinobi Kami - M416

            }

            if (strstr(strWeaponId.c_str(), "203008"))// M416_Mechanical_Sights
            {
                if (skinm4 == 1)
                    PARAMS->WeaponSkinID = 1010040442; //Glacier - M416 
                else if (skinm4 == 2)
                    PARAMS->WeaponSkinID = 1010040622; //The Fool - M416
                else if (skinm4 == 3)
                    PARAMS->WeaponSkinID = 1010040862; //Lizard Roar - M416
                else if (skinm4 == 4)
                    PARAMS->WeaponSkinID = 1010040782; //Wanderer - M416
                else if (skinm4 == 5)
                    PARAMS->WeaponSkinID = 1010040982; //Call of the Wild - M416
                else if (skinm4 == 6)
                    PARAMS->WeaponSkinID = 1010041632; //Imperial Splendor - M416
                else if (skinm4 == 7)
                    PARAMS->WeaponSkinID = 1010042012; //Silver Guru - M416
                else if (skinm4 == 8)
                    PARAMS->WeaponSkinID = 1010041382; //TechnoCore - M416
                else if (skinm4 == 9)
                    PARAMS->WeaponSkinID = 1010042092; //Tidal Embrace - M416
                else if (skinm4 == 10)
                    PARAMS->WeaponSkinID = 1010042182; //Shinobi Kami - M416                         
            }

            if (strstr(strWeaponId.c_str(), "291004"))// M416_default_Magazine
            {
                if (skinm4 == 1)
                    PARAMS->WeaponSkinID = 1010040441; //Glacier - M416 
                else if (skinm4 == 2)
                    PARAMS->WeaponSkinID = 1010040621; //The Fool - M416
                else if (skinm4 == 3)
                    PARAMS->WeaponSkinID = 1010040861; //Lizard Roar - M416
                else if (skinm4 == 4)
                    PARAMS->WeaponSkinID = 1010040781; //Wanderer - M416
                else if (skinm4 == 5)
                    PARAMS->WeaponSkinID = 1010040981; //Call of the Wild - M416
                else if (skinm4 == 6)
                    PARAMS->WeaponSkinID = 1010041631; //Imperial Splendor - M416
                else if (skinm4 == 7)
                    PARAMS->WeaponSkinID = 1010042011; //Silver Guru - M416
                else if (skinm4 == 8)
                    PARAMS->WeaponSkinID = 1010041381; //TechnoCore - M416
                else if (skinm4 == 9)
                    PARAMS->WeaponSkinID = 1010042091; //Tidal Embrace - M416
                else if (skinm4 == 10)
                    PARAMS->WeaponSkinID = 1010042181; //Shinobi Kami - M416

            }

            if (strstr(strWeaponId.c_str(), "101001")) {
                if (skinakm == 1)
                    PARAMS->WeaponSkinID = 1101001037; //Sculpture - AKM
                if (skinakm == 2)
                    PARAMS->WeaponSkinID = 1101001057; //The Seven Seas - AKM
                if (skinakm == 3)
                    PARAMS->WeaponSkinID = 1101001065; //Roaring Tiger - AKM
                if (skinakm == 4)
                    PARAMS->WeaponSkinID = 1101001089; //Glacier - AKM
                if (skinakm == 5)
                    PARAMS->WeaponSkinID = 1101001103; //Desert Fossil - AKM
                if (skinakm == 6)
                    PARAMS->WeaponSkinID = 1101001116; //Jack-o'-lantern - AKM
                if (skinakm == 7)
                    PARAMS->WeaponSkinID = 1101001128; //Ghillie Dragon - AKM 
                if (skinakm == 8)
                    PARAMS->WeaponSkinID = 1101001143; //Gold Pirate - AKM
                if (skinakm == 9)
                    PARAMS->WeaponSkinID = 1101001174; //Wandering Tyrant - AKM
                if (skinakm == 10)
                    PARAMS->WeaponSkinID = 1101001213; //Star Admiral - AKM
                if (skinakm == 11)
                    PARAMS->WeaponSkinID = 1101001023; //Hellfire - AKM
            }
            if (strstr(strWeaponId.c_str(), "101003")) {
                if (skinscar == 1)
                    PARAMS->WeaponSkinID = 1101003057; //Water Blaster - SCAR-L
                if (skinscar == 2)
                    PARAMS->WeaponSkinID = 1101003070; //Enchanted Pumpkin - SCAR-L
                if (skinscar == 3)
                    PARAMS->WeaponSkinID = 1101003079; //Operation Tomorrow - SCAR-L
                if (skinscar == 4)
                    PARAMS->WeaponSkinID = 1101003099; //Drop the Bass - SCAR-L 
                if (skinscar == 5)
                    PARAMS->WeaponSkinID = 1101003119; //Hextech Crystal - SCAR-L 
                if (skinscar == 6)
                    PARAMS->WeaponSkinID = 1101003146; //THORN OF MALICE - SCAR-L 
                if (skinscar == 7)
                    PARAMS->WeaponSkinID = 1101003181; //THORN OF MALICE - SCAR-L 
            }
            if (strstr(strWeaponId.c_str(), "101008")) {
                if (skinm7 == 1)
                    PARAMS->WeaponSkinID = 1101008026; //8-bit Unicorn - M762
                else if (skinm7 == 2)
                    PARAMS->WeaponSkinID = 1101008070; //GACKT MOONSAGA-M762
                else if (skinm7 == 3)
                    PARAMS->WeaponSkinID = 1101008036; //Lotus Fury - M762
                else if (skinm7 == 4)
                    PARAMS->WeaponSkinID = 1101008116; //Messi Football Icon M762
                else if (skinm7 == 5)
                    PARAMS->WeaponSkinID = 1101008051; //Concerto of Love - M762
                else if (skinm7 == 6)
                    PARAMS->WeaponSkinID = 1101008104; //StarCore-M762
                else if (skinm7 == 7)
                    PARAMS->WeaponSkinID = 1101008081; //Stray Rebellion - M762
            }
            if (strstr(strWeaponId.c_str(), "102001")) {
                if (skinuzi == 1)
                    PARAMS->WeaponSkinID = 1102001024; //Savagery - UZI
                if (skinuzi == 2)
                    PARAMS->WeaponSkinID = 1102001036; //Ethereal Emblem - UZI
                if (skinuzi == 3)
                    PARAMS->WeaponSkinID = 1102001058; //Romantic Moments - UZI
                if (skinuzi == 4)
                    PARAMS->WeaponSkinID = 1102001069; //Shimmer Power - UZI
            }
            if (strstr(strWeaponId.c_str(), "102002")) {
                if (skinump45 == 1)
                    PARAMS->WeaponSkinID = 1102002043;
                if (skinump45 == 2)
                    PARAMS->WeaponSkinID = 1102002053;
                if (skinump45 == 3)
                    PARAMS->WeaponSkinID = 1102002061;
                if (skinump45 == 4)
                    PARAMS->WeaponSkinID = 1102002070;
                if (skinump45 == 5)
                    PARAMS->WeaponSkinID = 1102002030;
                if (skinump45 == 6)
                    PARAMS->WeaponSkinID = 1102002090;
                if (skinump45 == 7)
                    PARAMS->WeaponSkinID = 1102002136;
            }
            if (strstr(strWeaponId.c_str(), "102003")) {
                if (skinvector == 1)
                    PARAMS->WeaponSkinID = 1102003020;
                if (skinvector == 2)
                    PARAMS->WeaponSkinID = 1102003031;
                if (skinvector == 3)
                    PARAMS->WeaponSkinID = 1102003039;
                if (skinvector == 4)
                    PARAMS->WeaponSkinID = 1102003072;
                if (skinvector == 5)
                    PARAMS->WeaponSkinID = 1102003060;
            }
            if (strstr(strWeaponId.c_str(), "102004")) {
                if (skinThompson == 1)
                    PARAMS->WeaponSkinID = 1102003060;  //candy cane
            }
            if (strstr(strWeaponId.c_str(), "102005")) {
                if (skinbizon == 1)
                    PARAMS->WeaponSkinID = 1102005007;
                if (skinbizon == 2)
                    PARAMS->WeaponSkinID = 1102005020;
            }
            if (strstr(strWeaponId.c_str(), "103001")) {
                if (skinkar == 1)
                    PARAMS->WeaponSkinID = 1103001060;
                if (skinkar == 2)
                    PARAMS->WeaponSkinID = 1103001079;
                if (skinkar == 3)
                    PARAMS->WeaponSkinID = 1103001085;
                if (skinkar == 4)
                    PARAMS->WeaponSkinID = 1103001101;
            }
            if (strstr(strWeaponId.c_str(), "103002")) {
                if (skinm24 == 1)
                    PARAMS->WeaponSkinID = 1103002018;
                if (skinm24 == 2)
                    PARAMS->WeaponSkinID = 1103002030;
                if (skinm24 == 3)
                    PARAMS->WeaponSkinID = 1103002049;
                if (skinm24 == 4)
                    PARAMS->WeaponSkinID = 1103002047;
                if (skinm24 == 5)
                    PARAMS->WeaponSkinID = 1103002059;
            }
            if (strstr(strWeaponId.c_str(), "103003")) {
                if (skinawm == 1)
                    PARAMS->WeaponSkinID = 1103003022;
                if (skinawm == 2)
                    PARAMS->WeaponSkinID = 1103003030;
                if (skinawm == 3)
                    PARAMS->WeaponSkinID = 1103003042;
                if (skinawm == 4)
                    PARAMS->WeaponSkinID = 1103003062;
            }
            if (strstr(strWeaponId.c_str(), "105002")) {
                if (skindp28 == 1)
                    PARAMS->WeaponSkinID = 1105002018;
                if (skindp28 == 2)
                    PARAMS->WeaponSkinID = 1105002035;
            }
            if (strstr(strWeaponId.c_str(), "101002")) {
                if (skinm16a4 == 1)
                    PARAMS->WeaponSkinID = 1101002029;
                if (skinm16a4 == 2)
                    PARAMS->WeaponSkinID = 1101002056;
                if (skinm16a4 == 3)
                    PARAMS->WeaponSkinID = 1101002068;
                if (skinm16a4 == 4)
                    PARAMS->WeaponSkinID = 1101002081;
            }
            if (strstr(strWeaponId.c_str(), "105001")) {
                if (skinm249 == 1)
                    PARAMS->WeaponSkinID = 1105001034;
                if (skinm249 == 2)
                    PARAMS->WeaponSkinID = 1105001020;
                if (skinm249 == 3)
                    PARAMS->WeaponSkinID = 1105001048;
            }
            if (strstr(strWeaponId.c_str(), "101005")) {
                if (skingroza == 1)
                    PARAMS->WeaponSkinID = 1101005019;
                if (skingroza == 2)
                    PARAMS->WeaponSkinID = 1101005052;
                if (skingroza == 3)
                    PARAMS->WeaponSkinID = 1101005025;
                if (skingroza == 4)
                    PARAMS->WeaponSkinID = 1101005038;
            }
            if (strstr(strWeaponId.c_str(), "103005")) {
                if (skinvss == 1)
                    PARAMS->WeaponSkinID = 1103005024;
            }
            if (strstr(strWeaponId.c_str(), "103007")) {
                if (skinmk14 == 1)
                    PARAMS->WeaponSkinID = 1103007020;
                if (skinmk14 == 2)
                    PARAMS->WeaponSkinID = 1103007028;
            }
            if (strstr(strWeaponId.c_str(), "104002")) {
                if (skins1897 == 1)
                    PARAMS->WeaponSkinID = 1104002022;
            }


            if (strstr(strWeaponId.c_str(), "101006")) {
                if (skinaug == 1)
                    PARAMS->WeaponSkinID = 1101006033;
                if (skinaug == 2)
                    PARAMS->WeaponSkinID = 1101006044;
                if (skinaug == 3)
                    PARAMS->WeaponSkinID = 1101006062;
            }
            if (strstr(strWeaponId.c_str(), "101006")) {
                if (skins12k == 1)
                    PARAMS->WeaponSkinID = 1104003026;
            }



        }

    }




    if (deadbox1)
    {
        if (strstr((const char*)pFunc->GetFullName().c_str(), "BackpackBlueprintUtils_BP.BackpackBlueprintUtils_BP_C.CreateBattleItemHandle") || strstr((const char*)pFunc->GetFullName().c_str(), "CreateWeaponAndChangeSkin") || strstr((char*)pFunc->GetFullName().c_str(), "BackpackBlueprintUtils_BP.BackpackBlueprintUtils_BP_C.GetWeaponSkinMappingID") || strstr((char*)pFunc->GetFullName().c_str(), "BackpackBlueprintUtils_BP.BackpackBlueprintUtils_BP_C.ModifySetting")) {
            UBackpackUtils_CreateBattleItemHandle_Params* PARAMS = (UBackpackUtils_CreateBattleItemHandle_Params*)pArgs;
            auto GWorld = GetWorld();
            ASTExtraPlayerController* localController = (ASTExtraPlayerController*)GWorld->NetDriver->ServerConnection->PlayerController;
            ASTExtraPlayerCharacter* localPlayer = (ASTExtraPlayerCharacter*)localController->AcknowledgedPawn;
            std::string strWeaponId = std::to_string((int)PARAMS->DefineID.TypeSpecificID);

            if (strstr(strWeaponId.c_str(), "1400129"))// TSHIRT
            {

                if (skinxsuit == 1)
                    PARAMS->DefineID.TypeSpecificID = 1405870;
                else if (skinxsuit == 2)
                    PARAMS->DefineID.TypeSpecificID = 1405628;
                else if (skinxsuit == 3)
                    PARAMS->DefineID.TypeSpecificID = 1406152;
                else if (skinxsuit == 4)
                    PARAMS->DefineID.TypeSpecificID = 1406475;
                else if (skinxsuit == 5)
                    PARAMS->DefineID.TypeSpecificID = 1405983;
                else if (skinxsuit == 6)
                    PARAMS->DefineID.TypeSpecificID = 1406638;
                else if (skinxsuit == 7)
                    PARAMS->DefineID.TypeSpecificID = 1406311;
                if (skinmyth == 1)
                    PARAMS->DefineID.TypeSpecificID = 1405623;
                else if (skinmyth == 2)
                    PARAMS->DefineID.TypeSpecificID = 1400687;
                else if (skinmyth == 3)
                    PARAMS->DefineID.TypeSpecificID = 1405102;
                else if (skinmyth == 4)
                    PARAMS->DefineID.TypeSpecificID = 1405145;
                else if (skinmyth == 5)
                    PARAMS->DefineID.TypeSpecificID = 1400782;
                else if (skinmyth == 6)
                    PARAMS->DefineID.TypeSpecificID = 1400119;
                else if (skinmyth == 7)
                    PARAMS->DefineID.TypeSpecificID = 1400117;
                else if (skinmyth == 8)
                    // SKIN 2
                    PARAMS->DefineID.TypeSpecificID = 1400693;                        if (skinfool == 1)
                    PARAMS->DefineID.TypeSpecificID = 1405092;
                    else if (skinfool == 2)
                    PARAMS->DefineID.TypeSpecificID = 1405090;
                    else if (skinfool == 3)
                    PARAMS->DefineID.TypeSpecificID = 1405482;
                    else if (skinfool == 4)
                    PARAMS->DefineID.TypeSpecificID = 1405583;
                    else if (skinfool == 5)
                    PARAMS->DefineID.TypeSpecificID = 1405593;
                    else if (skinfool == 6)
                    PARAMS->DefineID.TypeSpecificID = 1405629;
                    else if (skinfool == 7)
                    PARAMS->DefineID.TypeSpecificID = 1405582;
            }


            if (strstr(strWeaponId.c_str(), "40601001"))
            {
                if (Hair11 == 1)
                    PARAMS->DefineID.TypeSpecificID = 40601011;
                else if (Hair11 == 2)
                    PARAMS->DefineID.TypeSpecificID = 40601012;
            }

            if (strstr(strWeaponId.c_str(), "501001"))
            {
                if (skinbg == 1)
                    PARAMS->DefineID.TypeSpecificID = 1501001220;
                else if (skinbg == 2)
                    PARAMS->DefineID.TypeSpecificID = 1501001174;
                else if (skinbg == 3)
                    PARAMS->DefineID.TypeSpecificID = 1501001265;
                else if (skinbg == 4)
                    PARAMS->DefineID.TypeSpecificID = 1501001303;
                else if (skinbg == 5)
                    PARAMS->DefineID.TypeSpecificID = 1501001331;
                else if (skinbg == 6)
                    PARAMS->DefineID.TypeSpecificID = 1501001009;
                else if (skinbg == 7)
                    PARAMS->DefineID.TypeSpecificID = 1501001061;
            }

            if (strstr(strWeaponId.c_str(), "501004"))
            {
                if (skinbg == 1)
                    PARAMS->DefineID.TypeSpecificID = 1501001220;
                else if (skinbg == 2)
                    PARAMS->DefineID.TypeSpecificID = 1501001174;
                else if (skinbg == 3)
                    PARAMS->DefineID.TypeSpecificID = 1501001265;
                else if (skinbg == 4)
                    PARAMS->DefineID.TypeSpecificID = 1501001303;
                else if (skinbg == 5)
                    PARAMS->DefineID.TypeSpecificID = 1501001331;
                else if (skinbg == 6)
                    PARAMS->DefineID.TypeSpecificID = 1501001009;
                else if (skinbg == 7)
                    PARAMS->DefineID.TypeSpecificID = 1501001061;
            }


            if (strstr(strWeaponId.c_str(), "501002"))
            {
                if (skinbg == 1)
                    PARAMS->DefineID.TypeSpecificID = 1501002220;
                else if (skinbg == 2)
                    PARAMS->DefineID.TypeSpecificID = 1501002174;
                else if (skinbg == 3)
                    PARAMS->DefineID.TypeSpecificID = 1501002265;
                else if (skinbg == 4)
                    PARAMS->DefineID.TypeSpecificID = 1501002303;
                else if (skinbg == 5)
                    PARAMS->DefineID.TypeSpecificID = 1501002331;
                else if (skinbg == 6)
                    PARAMS->DefineID.TypeSpecificID = 1501002009;
                else if (skinbg == 7)
                    PARAMS->DefineID.TypeSpecificID = 1501002061;
            }

            if (strstr(strWeaponId.c_str(), "501005"))
            {
                if (skinbg == 1)
                    PARAMS->DefineID.TypeSpecificID = 1501002220;
                else if (skinbg == 2)
                    PARAMS->DefineID.TypeSpecificID = 1501002174;
                else if (skinbg == 3)
                    PARAMS->DefineID.TypeSpecificID = 1501002265;
                else if (skinbg == 4)
                    PARAMS->DefineID.TypeSpecificID = 1501002303;
                else if (skinbg == 5)
                    PARAMS->DefineID.TypeSpecificID = 1501002331;
                else if (skinbg == 6)
                    PARAMS->DefineID.TypeSpecificID = 1501002009;
                else if (skinbg == 7)
                    PARAMS->DefineID.TypeSpecificID = 1501002061;
            }

            if (strstr(strWeaponId.c_str(), "501003"))
            {
                if (skinbg == 1)
                    PARAMS->DefineID.TypeSpecificID = 1501003220;
                else if (skinbg == 2)
                    PARAMS->DefineID.TypeSpecificID = 1501003174;
                else if (skinbg == 3)
                    PARAMS->DefineID.TypeSpecificID = 1501003265;
                else if (skinbg == 4)
                    PARAMS->DefineID.TypeSpecificID = 1501003303;
                else if (skinbg == 5)
                    PARAMS->DefineID.TypeSpecificID = 1501003331;
                else if (skinbg == 6)
                    PARAMS->DefineID.TypeSpecificID = 1501003009;
                else if (skinbg == 7)
                    PARAMS->DefineID.TypeSpecificID = 1501003061;
            }

            if (strstr(strWeaponId.c_str(), "501006"))
            {
                if (skinbg == 1)
                    PARAMS->DefineID.TypeSpecificID = 1501003220;
                else if (skinbg == 2)
                    PARAMS->DefineID.TypeSpecificID = 1501003174;
                else if (skinbg == 3)
                    PARAMS->DefineID.TypeSpecificID = 1501003265;
                else if (skinbg == 4)
                    PARAMS->DefineID.TypeSpecificID = 1501003303;
                else if (skinbg == 5)
                    PARAMS->DefineID.TypeSpecificID = 1501003331;
                else if (skinbg == 6)
                    PARAMS->DefineID.TypeSpecificID = 1501003009;
                else if (skinbg == 7)
                    PARAMS->DefineID.TypeSpecificID = 1501003061;
            }



            if (strstr(strWeaponId.c_str(), "502001"))
            {
                if (skinhmm == 1)
                    PARAMS->DefineID.TypeSpecificID = 1502001014;
                else if (skinhmm == 2)
                    PARAMS->DefineID.TypeSpecificID = 1502001023;
                else if (skinhmm == 3)
                    PARAMS->DefineID.TypeSpecificID = 1502001183;
                else if (skinhmm == 4)
                    PARAMS->DefineID.TypeSpecificID = 1502001128;
                else if (skinhmm == 5)
                    PARAMS->DefineID.TypeSpecificID = 1502001069;
                else if (skinhmm == 6)
                    PARAMS->DefineID.TypeSpecificID = 1502001009;
                else if (skinhmm == 7)
                    PARAMS->DefineID.TypeSpecificID = 1502001101;
            }

            if (strstr(strWeaponId.c_str(), "502004"))
            {
                if (skinhmm == 1)
                    PARAMS->DefineID.TypeSpecificID = 1502001014;
                else if (skinhmm == 2)
                    PARAMS->DefineID.TypeSpecificID = 1502001023;
                else if (skinhmm == 3)
                    PARAMS->DefineID.TypeSpecificID = 1502001183;
                else if (skinhmm == 4)
                    PARAMS->DefineID.TypeSpecificID = 1502001128;
                else if (skinhmm == 5)
                    PARAMS->DefineID.TypeSpecificID = 1502001069;
                else if (skinhmm == 6)
                    PARAMS->DefineID.TypeSpecificID = 1502001009;
                else if (skinhmm == 7)
                    PARAMS->DefineID.TypeSpecificID = 1502001101;
            }



            if (strstr(strWeaponId.c_str(), "502002"))
            {
                if (skinhmm == 1)
                    PARAMS->DefineID.TypeSpecificID = 1502002014;

                else if (skinhmm == 2)
                    PARAMS->DefineID.TypeSpecificID = 1502002023;
                else if (skinhmm == 3)
                    PARAMS->DefineID.TypeSpecificID = 1502002183;
                else if (skinhmm == 4)
                    PARAMS->DefineID.TypeSpecificID = 1502002128;
                else if (skinhmm == 5)
                    PARAMS->DefineID.TypeSpecificID = 1502002069;
                else if (skinhmm == 6)
                    PARAMS->DefineID.TypeSpecificID = 1502002009;
                else if (skinhmm == 7)
                    PARAMS->DefineID.TypeSpecificID = 1502002101;
            }

            if (strstr(strWeaponId.c_str(), "502005"))
            {
                if (skinhmm == 1)
                    PARAMS->DefineID.TypeSpecificID = 1502002014;
                else if (skinhmm == 2)
                    PARAMS->DefineID.TypeSpecificID = 1502002023;
                else if (skinhmm == 3)
                    PARAMS->DefineID.TypeSpecificID = 1502002183;
                else if (skinhmm == 4)
                    PARAMS->DefineID.TypeSpecificID = 1502002128;
                else if (skinhmm == 5)
                    PARAMS->DefineID.TypeSpecificID = 1502002069;
                else if (skinhmm == 6)
                    PARAMS->DefineID.TypeSpecificID = 1502002009;
                else if (skinhmm == 7)
                    PARAMS->DefineID.TypeSpecificID = 1502002101;
            }

            if (strstr(strWeaponId.c_str(), "502003"))
            {
                if (skinhmm == 1)
                    PARAMS->DefineID.TypeSpecificID = 1502003014;
                else if (skinhmm == 2)
                    PARAMS->DefineID.TypeSpecificID = 1502003023;
                else if (skinhmm == 3)
                    PARAMS->DefineID.TypeSpecificID = 1502003183;
                else if (skinhmm == 4)
                    PARAMS->DefineID.TypeSpecificID = 1502003128;
                else if (skinhmm == 5)
                    PARAMS->DefineID.TypeSpecificID = 1502003069;
                else if (skinhmm == 6)
                    PARAMS->DefineID.TypeSpecificID = 1502003009;
                else if (skinhmm == 7)
                    PARAMS->DefineID.TypeSpecificID = 1502003101;
            }
            if (strstr(strWeaponId.c_str(), "502006"))
            {
                if (skinhmm == 1)
                    PARAMS->DefineID.TypeSpecificID = 1502003014;
                else if (skinhmm == 2)
                    PARAMS->DefineID.TypeSpecificID = 1502003023;
                else if (skinhmm == 3)
                    PARAMS->DefineID.TypeSpecificID = 1502003183;
                else if (skinhmm == 4)
                    PARAMS->DefineID.TypeSpecificID = 1502003128;
                else if (skinhmm == 5)
                    PARAMS->DefineID.TypeSpecificID = 1502003069;
                else if (skinhmm == 6)
                    PARAMS->DefineID.TypeSpecificID = 1502003009;
                else if (skinhmm == 7)
                    PARAMS->DefineID.TypeSpecificID = 1502003101;
            }

            if (strstr(strWeaponId.c_str(), "101004")) {

                if (skinm4 == 1)

                    PARAMS->DefineID.TypeSpecificID = 1101004046; //Glacier - M416 
                if (skinm4 == 2)
                    PARAMS->DefineID.TypeSpecificID = 1101004062; //Glacier - M416 
                if (skinm4 == 3)
                    PARAMS->DefineID.TypeSpecificID = 1101004086; //Glacier - M416 
                if (skinm4 == 4)
                    PARAMS->DefineID.TypeSpecificID = 1101004078; //Glacier - M416 
                if (skinm4 == 5)
                    PARAMS->DefineID.TypeSpecificID = 1101004098; //Glacier - M416 
                if (skinm4 == 9)
                    PARAMS->DefineID.TypeSpecificID = 1101004218; //Glacier - M416 
                if (skinm4 == 6)
                    PARAMS->DefineID.TypeSpecificID = 1101004163; //Glacier - M416 
                if (skinm4 == 7)
                    PARAMS->DefineID.TypeSpecificID = 1101004201; //Glacier - M416 
                if (skinm4 == 8)
                    PARAMS->DefineID.TypeSpecificID = 1101004138; //Glacier - M416 
                if (skinm4 == 10)
                    PARAMS->DefineID.TypeSpecificID = 1101004209; //Glacier - M416 
            }

            if (strstr(strWeaponId.c_str(), "205002"))// Config.M416_Tactical_stock
            {
                if (skinm4 == 1)
                    PARAMS->DefineID.TypeSpecificID = 1010040443; //Glacier - M416 
                else if (skinm4 == 2)
                    PARAMS->DefineID.TypeSpecificID = 1010040623; //The Fool - M416
                else if (skinm4 == 3)
                    PARAMS->DefineID.TypeSpecificID = 1010040863; //Lizard Roar - M416
                else if (skinm4 == 4)
                    PARAMS->DefineID.TypeSpecificID = 1010040783; //Wanderer - M416
                else if (skinm4 == 5)
                    PARAMS->DefineID.TypeSpecificID = 1010040983; //Call of the Wild - M416
                else if (skinm4 == 6)
                    PARAMS->DefineID.TypeSpecificID = 1010041633; //Imperial Splendor - M416
                else if (skinm4 == 7)
                    PARAMS->DefineID.TypeSpecificID = 1010042013; //Silver Guru - M416
                else if (skinm4 == 8)
                    PARAMS->DefineID.TypeSpecificID = 1010041383; //TechnoCore - M416
                else if (skinm4 == 9)
                    PARAMS->DefineID.TypeSpecificID = 1010042093; //Tidal Embrace - M416
                else if (skinm4 == 10)
                    PARAMS->DefineID.TypeSpecificID = 1010042183; //Shinobi Kami - M416

            }

            if (strstr(strWeaponId.c_str(), "205005"))// M416_default_stock
            {
                if (skinm4 == 1)
                    PARAMS->DefineID.TypeSpecificID = 1010040443; //Glacier - M416 
                else if (skinm4 == 2)
                    PARAMS->DefineID.TypeSpecificID = 1010040623; //The Fool - M416
                else if (skinm4 == 3)
                    PARAMS->DefineID.TypeSpecificID = 1010040863; //Lizard Roar - M416
                else if (skinm4 == 4)
                    PARAMS->DefineID.TypeSpecificID = 1010040783; //Wanderer - M416
                else if (skinm4 == 5)
                    PARAMS->DefineID.TypeSpecificID = 1010040983; //Call of the Wild - M416
                else if (skinm4 == 6)
                    PARAMS->DefineID.TypeSpecificID = 1010041633; //Imperial Splendor - M416
                else if (skinm4 == 7)
                    PARAMS->DefineID.TypeSpecificID = 1010042013; //Silver Guru - M416
                else if (skinm4 == 8)
                    PARAMS->DefineID.TypeSpecificID = 1010041383; //TechnoCore - M416
                else if (skinm4 == 9)
                    PARAMS->DefineID.TypeSpecificID = 1010042093; //Tidal Embrace - M416
                else if (skinm4 == 10)
                    PARAMS->DefineID.TypeSpecificID = 1010042183; //Shinobi Kami - M416

            }

            if (strstr(strWeaponId.c_str(), "203008"))// M416_Mechanical_Sights
            {
                if (skinm4 == 1)
                    PARAMS->DefineID.TypeSpecificID = 1010040442; //Glacier - M416 
                else if (skinm4 == 2)
                    PARAMS->DefineID.TypeSpecificID = 1010040622; //The Fool - M416
                else if (skinm4 == 3)
                    PARAMS->DefineID.TypeSpecificID = 1010040862; //Lizard Roar - M416
                else if (skinm4 == 4)
                    PARAMS->DefineID.TypeSpecificID = 1010040782; //Wanderer - M416
                else if (skinm4 == 5)
                    PARAMS->DefineID.TypeSpecificID = 1010040982; //Call of the Wild - M416
                else if (skinm4 == 6)
                    PARAMS->DefineID.TypeSpecificID = 1010041632; //Imperial Splendor - M416
                else if (skinm4 == 7)
                    PARAMS->DefineID.TypeSpecificID = 1010042012; //Silver Guru - M416
                else if (skinm4 == 8)
                    PARAMS->DefineID.TypeSpecificID = 1010041382; //TechnoCore - M416
                else if (skinm4 == 9)
                    PARAMS->DefineID.TypeSpecificID = 1010042092; //Tidal Embrace - M416
                else if (skinm4 == 10)
                    PARAMS->DefineID.TypeSpecificID = 1010042182; //Shinobi Kami - M416                         
            }

            if (strstr(strWeaponId.c_str(), "291004"))// M416_default_Magazine
            {
                if (skinm4 == 1)
                    PARAMS->DefineID.TypeSpecificID = 1010040441; //Glacier - M416 
                else if (skinm4 == 2)
                    PARAMS->DefineID.TypeSpecificID = 1010040621; //The Fool - M416
                else if (skinm4 == 3)
                    PARAMS->DefineID.TypeSpecificID = 1010040861; //Lizard Roar - M416
                else if (skinm4 == 4)
                    PARAMS->DefineID.TypeSpecificID = 1010040781; //Wanderer - M416
                else if (skinm4 == 5)
                    PARAMS->DefineID.TypeSpecificID = 1010040981; //Call of the Wild - M416
                else if (skinm4 == 6)
                    PARAMS->DefineID.TypeSpecificID = 1010041631; //Imperial Splendor - M416
                else if (skinm4 == 7)
                    PARAMS->DefineID.TypeSpecificID = 1010042011; //Silver Guru - M416
                else if (skinm4 == 8)
                    PARAMS->DefineID.TypeSpecificID = 1010041381; //TechnoCore - M416
                else if (skinm4 == 9)
                    PARAMS->DefineID.TypeSpecificID = 1010042091; //Tidal Embrace - M416
                else if (skinm4 == 10)
                    PARAMS->DefineID.TypeSpecificID = 1010042181; //Shinobi Kami - M416

            }

            if (strstr(strWeaponId.c_str(), "101001")) {
                if (skinakm == 1)
                    PARAMS->DefineID.TypeSpecificID = 1101001037; //Sculpture - AKM
                if (skinakm == 2)
                    PARAMS->DefineID.TypeSpecificID = 1101001057; //The Seven Seas - AKM
                if (skinakm == 3)
                    PARAMS->DefineID.TypeSpecificID = 1101001065; //Roaring Tiger - AKM
                if (skinakm == 4)
                    PARAMS->DefineID.TypeSpecificID = 1101001089; //Glacier - AKM
                if (skinakm == 5)
                    PARAMS->DefineID.TypeSpecificID = 1101001103; //Desert Fossil - AKM
                if (skinakm == 6)
                    PARAMS->DefineID.TypeSpecificID = 1101001116; //Jack-o'-lantern - AKM
                if (skinakm == 7)
                    PARAMS->DefineID.TypeSpecificID = 1101001128; //Ghillie Dragon - AKM 
                if (skinakm == 8)
                    PARAMS->DefineID.TypeSpecificID = 1101001143; //Gold Pirate - AKM
                if (skinakm == 9)
                    PARAMS->DefineID.TypeSpecificID = 1101001174; //Wandering Tyrant - AKM
                if (skinakm == 10)
                    PARAMS->DefineID.TypeSpecificID = 1101001213; //Star Admiral - AKM
                if (skinakm == 11)
                    PARAMS->DefineID.TypeSpecificID = 1101001023; //Hellfire - AKM
            }
            if (strstr(strWeaponId.c_str(), "101003")) {
                if (skinscar == 1)
                    PARAMS->DefineID.TypeSpecificID = 1101003057; //Water Blaster - SCAR-L
                if (skinscar == 2)
                    PARAMS->DefineID.TypeSpecificID = 1101003070; //Enchanted Pumpkin - SCAR-L
                if (skinscar == 3)
                    PARAMS->DefineID.TypeSpecificID = 1101003079; //Operation Tomorrow - SCAR-L
                if (skinscar == 4)
                    PARAMS->DefineID.TypeSpecificID = 1101003099; //Drop the Bass - SCAR-L 
                if (skinscar == 5)
                    PARAMS->DefineID.TypeSpecificID = 1101003119; //Hextech Crystal - SCAR-L 
                if (skinscar == 6)
                    PARAMS->DefineID.TypeSpecificID = 1101003146; //THORN OF MALICE - SCAR-L 
                if (skinscar == 7)
                    PARAMS->DefineID.TypeSpecificID = 1101003181; //THORN OF MALICE - SCAR-L 
            }
            if (strstr(strWeaponId.c_str(), "101008")) {
                if (skinm7 == 1)
                    PARAMS->DefineID.TypeSpecificID = 1101008026; //8-bit Unicorn - M762
                else if (skinm7 == 2)
                    PARAMS->DefineID.TypeSpecificID = 1101008070; //GACKT MOONSAGA-M762
                else if (skinm7 == 3)
                    PARAMS->DefineID.TypeSpecificID = 1101008036; //Lotus Fury - M762
                else if (skinm7 == 4)
                    PARAMS->DefineID.TypeSpecificID = 1101008116; //Messi Football Icon M762
                else if (skinm7 == 5)
                    PARAMS->DefineID.TypeSpecificID = 1101008051; //Concerto of Love - M762
                else if (skinm7 == 6)
                    PARAMS->DefineID.TypeSpecificID = 1101008104; //StarCore-M762
                else if (skinm7 == 7)
                    PARAMS->DefineID.TypeSpecificID = 1101008081; //Stray Rebellion - M762
            }
            if (strstr(strWeaponId.c_str(), "102001")) {
                if (skinuzi == 1)
                    PARAMS->DefineID.TypeSpecificID = 1102001024; //Savagery - UZI
                if (skinuzi == 2)
                    PARAMS->DefineID.TypeSpecificID = 1102001036; //Ethereal Emblem - UZI
                if (skinuzi == 3)
                    PARAMS->DefineID.TypeSpecificID = 1102001058; //Romantic Moments - UZI
                if (skinuzi == 4)
                    PARAMS->DefineID.TypeSpecificID = 1102001069; //Shimmer Power - UZI
            }
            if (strstr(strWeaponId.c_str(), "102002")) {
                if (skinump45 == 1)
                    PARAMS->DefineID.TypeSpecificID = 1102002043;
                if (skinump45 == 2)
                    PARAMS->DefineID.TypeSpecificID = 1102002053;
                if (skinump45 == 3)
                    PARAMS->DefineID.TypeSpecificID = 1102002061;
                if (skinump45 == 4)
                    PARAMS->DefineID.TypeSpecificID = 1102002070;
                if (skinump45 == 5)
                    PARAMS->DefineID.TypeSpecificID = 1102002030;
                if (skinump45 == 6)
                    PARAMS->DefineID.TypeSpecificID = 1102002090;
                if (skinump45 == 7)
                    PARAMS->DefineID.TypeSpecificID = 1102002136;
            }
            if (strstr(strWeaponId.c_str(), "102003")) {
                if (skinvector == 1)
                    PARAMS->DefineID.TypeSpecificID = 1102003020;
                if (skinvector == 2)
                    PARAMS->DefineID.TypeSpecificID = 1102003031;
                if (skinvector == 3)
                    PARAMS->DefineID.TypeSpecificID = 1102003039;
                if (skinvector == 4)
                    PARAMS->DefineID.TypeSpecificID = 1102003072;
                if (skinvector == 5)
                    PARAMS->DefineID.TypeSpecificID = 1102003060;
            }
            if (strstr(strWeaponId.c_str(), "102004")) {
                if (skinThompson == 1)
                    PARAMS->DefineID.TypeSpecificID = 1102003060;  //candy cane
            }
            if (strstr(strWeaponId.c_str(), "102005")) {
                if (skinbizon == 1)
                    PARAMS->DefineID.TypeSpecificID = 1102005007;
                if (skinbizon == 2)
                    PARAMS->DefineID.TypeSpecificID = 1102005020;
            }
            if (strstr(strWeaponId.c_str(), "103001")) {
                if (skinkar == 1)
                    PARAMS->DefineID.TypeSpecificID = 1103001060;
                if (skinkar == 2)
                    PARAMS->DefineID.TypeSpecificID = 1103001079;
                if (skinkar == 3)
                    PARAMS->DefineID.TypeSpecificID = 1103001085;
                if (skinkar == 4)
                    PARAMS->DefineID.TypeSpecificID = 1103001101;
            }
            if (strstr(strWeaponId.c_str(), "103002")) {
                if (skinm24 == 1)
                    PARAMS->DefineID.TypeSpecificID = 1103002018;
                if (skinm24 == 2)
                    PARAMS->DefineID.TypeSpecificID = 1103002030;
                if (skinm24 == 3)
                    PARAMS->DefineID.TypeSpecificID = 1103002049;
                if (skinm24 == 4)
                    PARAMS->DefineID.TypeSpecificID = 1103002047;
                if (skinm24 == 5)
                    PARAMS->DefineID.TypeSpecificID = 1103002059;
            }
            if (strstr(strWeaponId.c_str(), "103003")) {
                if (skinawm == 1)
                    PARAMS->DefineID.TypeSpecificID = 1103003022;
                if (skinawm == 2)
                    PARAMS->DefineID.TypeSpecificID = 1103003030;
                if (skinawm == 3)
                    PARAMS->DefineID.TypeSpecificID = 1103003042;
                if (skinawm == 4)
                    PARAMS->DefineID.TypeSpecificID = 1103003062;
            }
            if (strstr(strWeaponId.c_str(), "105002")) {
                if (skindp28 == 1)
                    PARAMS->DefineID.TypeSpecificID = 1105002018;
                if (skindp28 == 2)
                    PARAMS->DefineID.TypeSpecificID = 1105002035;
            }
            if (strstr(strWeaponId.c_str(), "101002")) {
                if (skinm16a4 == 1)
                    PARAMS->DefineID.TypeSpecificID = 1101002029;
                if (skinm16a4 == 2)
                    PARAMS->DefineID.TypeSpecificID = 1101002056;
                if (skinm16a4 == 3)
                    PARAMS->DefineID.TypeSpecificID = 1101002068;
                if (skinm16a4 == 4)
                    PARAMS->DefineID.TypeSpecificID = 1101002081;
            }
            if (strstr(strWeaponId.c_str(), "105001")) {
                if (skinm249 == 1)
                    PARAMS->DefineID.TypeSpecificID = 1105001034;
                if (skinm249 == 2)
                    PARAMS->DefineID.TypeSpecificID = 1105001020;
                if (skinm249 == 3)
                    PARAMS->DefineID.TypeSpecificID = 1105001048;
            }
            if (strstr(strWeaponId.c_str(), "101005")) {
                if (skingroza == 1)
                    PARAMS->DefineID.TypeSpecificID = 1101005019;
                if (skingroza == 2)
                    PARAMS->DefineID.TypeSpecificID = 1101005052;
                if (skingroza == 3)
                    PARAMS->DefineID.TypeSpecificID = 1101005025;
                if (skingroza == 4)
                    PARAMS->DefineID.TypeSpecificID = 1101005038;
            }
            if (strstr(strWeaponId.c_str(), "103005")) {
                if (skinvss == 1)
                    PARAMS->DefineID.TypeSpecificID = 1103005024;
            }
            if (strstr(strWeaponId.c_str(), "103007")) {
                if (skinmk14 == 1)
                    PARAMS->DefineID.TypeSpecificID = 1103007020;
                if (skinmk14 == 2)
                    PARAMS->DefineID.TypeSpecificID = 1103007028;
            }
            if (strstr(strWeaponId.c_str(), "104002")) {
                if (skins1897 == 1)
                    PARAMS->DefineID.TypeSpecificID = 1104002022;
            }


            if (strstr(strWeaponId.c_str(), "101006")) {
                if (skinaug == 1)
                    PARAMS->DefineID.TypeSpecificID = 1101006033;
                if (skinaug == 2)
                    PARAMS->DefineID.TypeSpecificID = 1101006044;
                if (skinaug == 3)
                    PARAMS->DefineID.TypeSpecificID = 1101006062;
            }
            if (strstr(strWeaponId.c_str(), "101006")) {
                if (skins12k == 1)
                    PARAMS->DefineID.TypeSpecificID = 1104003026;
            }



        }

    }











    if (std::string(pObj->GetName().c_str()).find("DeadBoxAvatarComponent") != std::string::npos) {
        UDeadBoxAvatarComponent* DeadBoxPointer = (UDeadBoxAvatarComponent*)pObj;
        if (std::string(pFunc->GetFullName().c_str()).find("GetLuaFilePath") != std::string::npos) {
            uint32_t Key = DeadBoxPointer->IsSelf();
            auto GWorld = GetWorld();
            if (GWorld) {
                if (GWorld->NetDriver->ServerConnection)
                    if (GWorld->NetDriver->ServerConnection->PlayerController) {
                        ASTExtraPlayerController* localController = (ASTExtraPlayerController*)GWorld->NetDriver->ServerConnection->PlayerController;
                        ASTExtraPlayerCharacter* localPlayer = (ASTExtraPlayerCharacter*)localController->AcknowledgedPawn;
                        if (localPlayer->WeaponManagerComponent->CurrentWeaponReplicated) {
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "M416")) {
                                if (skinm4 == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1101004046, true); //m4 glacier
                                if (skinm4 == 2)
                                    DeadBoxPointer->ChangeItemAvatar(1101004062, true); //m4 glacier
                                if (skinm4 == 3)
                                    DeadBoxPointer->ChangeItemAvatar(1101004086, true); //m4 glacier
                                if (skinm4 == 4)
                                    DeadBoxPointer->ChangeItemAvatar(1101004078, true); //m4 glacier
                                if (skinm4 == 5)
                                    DeadBoxPointer->ChangeItemAvatar(1101004098, true); //m4 glacier
                                if (skinm4 == 6)
                                    DeadBoxPointer->ChangeItemAvatar(1101004163, true); //m4 glacier
                                if (skinm4 == 7)
                                    DeadBoxPointer->ChangeItemAvatar(1101004201, true); //m4 glacier
                                if (skinm4 == 8)
                                    DeadBoxPointer->ChangeItemAvatar(1101004138, true); //m4 glacier
                                if (skinm4 == 9)
                                    DeadBoxPointer->ChangeItemAvatar(1101004218, true); //m4 glacier
                                if (skinm4 == 10)
                                    DeadBoxPointer->ChangeItemAvatar(1101004209, true); //m4 glacier

                            }
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "AKM")) {
                                if (skinakm == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1101001037, true); //Sculpture - AKM
                                if (skinakm == 2)
                                    DeadBoxPointer->ChangeItemAvatar(1101001057, true); //The Seven Seas - AKM
                                if (skinakm == 3)
                                    DeadBoxPointer->ChangeItemAvatar(1101001065, true); //Roaring Tiger - AKM
                                if (skinakm == 4)
                                    DeadBoxPointer->ChangeItemAvatar(1101001089, true); //Glacier - AKM
                                if (skinakm == 5)
                                    DeadBoxPointer->ChangeItemAvatar(1101001103, true); //Desert Fossil - AKM
                                if (skinakm == 6)
                                    DeadBoxPointer->ChangeItemAvatar(1101001116, true); //Jack-o'-lantern - AKM
                                if (skinakm == 7)
                                    DeadBoxPointer->ChangeItemAvatar(1101001128, true); //Ghillie Dragon - AKM 
                                if (skinakm == 8)
                                    DeadBoxPointer->ChangeItemAvatar(1101001143, true); //Gold Pirate - AKM
                                if (skinakm == 9)
                                    DeadBoxPointer->ChangeItemAvatar(1101001174, true); //Wandering Tyrant - AKM
                                if (skinakm == 10)
                                    DeadBoxPointer->ChangeItemAvatar(1101001213, true); //Star Admiral - AKM
                                if (skinakm == 11)
                                    DeadBoxPointer->ChangeItemAvatar(1101001023, true); //Hellfire - AKM      
                            }
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "M762")) {
                                if (skinm7 == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1101008026, true); //8-bit Unicorn - M762
                                else if (skinm7 == 2)
                                    DeadBoxPointer->ChangeItemAvatar(1101008070, true); //GACKT MOONSAGA-M762
                                else if (skinm7 == 3)
                                    DeadBoxPointer->ChangeItemAvatar(1101008036, true); //Lotus Fury - M762
                                else if (skinm7 == 4)
                                    DeadBoxPointer->ChangeItemAvatar(1101008116, true); //Messi Football Icon M762
                                else if (skinm7 == 5)
                                    DeadBoxPointer->ChangeItemAvatar(1101008051, true); //Concerto of Love - M762
                                else if (skinm7 == 6)
                                    DeadBoxPointer->ChangeItemAvatar(1101008104, true); //StarCore-M762
                                else if (skinm7 == 7)
                                    DeadBoxPointer->ChangeItemAvatar(1101008081, true); //Stray Rebellion - M762
                            }
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "SCAR-L")) {
                                if (skinscar == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1101003057, true); //8-bit Unicorn - M762
                                else if (skinscar == 2)
                                    DeadBoxPointer->ChangeItemAvatar(1101003070, true); //GACKT MOONSAGA-M762
                                else if (skinscar == 3)
                                    DeadBoxPointer->ChangeItemAvatar(1101003079, true); //Lotus Fury - M762
                                else if (skinscar == 4)
                                    DeadBoxPointer->ChangeItemAvatar(1101003099, true); //Messi Football Icon M762
                                else if (skinscar == 5)
                                    DeadBoxPointer->ChangeItemAvatar(1101003119, true); //Concerto of Love - M762
                                else if (skinscar == 6)
                                    DeadBoxPointer->ChangeItemAvatar(1101003146, true); //StarCore-M762
                                else if (skinscar == 7)
                                    DeadBoxPointer->ChangeItemAvatar(1101003181, true); //Stray Rebellion - M762
                            }
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "UMP45")) {
                                if (skinump45 == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1102002043, true); //8-bit Unicorn - M762
                                else if (skinump45 == 2)
                                    DeadBoxPointer->ChangeItemAvatar(1102002053, true); //GACKT MOONSAGA-M762
                                else if (skinump45 == 3)
                                    DeadBoxPointer->ChangeItemAvatar(1102002061, true); //Lotus Fury - M762
                                else if (skinump45 == 4)
                                    DeadBoxPointer->ChangeItemAvatar(1102002070, true); //Messi Football Icon M762
                                else if (skinump45 == 5)
                                    DeadBoxPointer->ChangeItemAvatar(1102002030, true); //Concerto of Love - M762
                                else if (skinump45 == 6)
                                    DeadBoxPointer->ChangeItemAvatar(1102002090, true); //StarCore-M762
                                else if (skinump45 == 7)
                                    DeadBoxPointer->ChangeItemAvatar(1102002136, true); //Stray Rebellion - M762
                            }
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "UZI")) {
                                if (skinuzi == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1102001024, true); //8-bit Unicorn - M762
                                else if (skinuzi == 2)
                                    DeadBoxPointer->ChangeItemAvatar(1102001036, true); //GACKT MOONSAGA-M762
                                else if (skinuzi == 3)
                                    DeadBoxPointer->ChangeItemAvatar(1102001058, true); //Lotus Fury - M762
                                else if (skinuzi == 4)
                                    DeadBoxPointer->ChangeItemAvatar(1102001069, true); //Messi Football Icon M762
                            }
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "Vector")) {
                                if (skinvector == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1102003020, true); //8-bit Unicorn - M762
                                else if (skinvector == 2)
                                    DeadBoxPointer->ChangeItemAvatar(1102003031, true); //GACKT MOONSAGA-M762
                                else if (skinvector == 3)
                                    DeadBoxPointer->ChangeItemAvatar(1102003039, true); //Lotus Fury - M762
                                else if (skinvector == 4)
                                    DeadBoxPointer->ChangeItemAvatar(1102003072, true); //Messi Football Icon M762
                                else if (skinvector == 5)
                                    DeadBoxPointer->ChangeItemAvatar(1102003060, true); //Concerto of Love - M762

                            }
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "Thompson")) {
                                if (skinThompson == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1102003060, true); //8-bit Unicorn - M762
                            }
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "Groza")) {
                                if (skingroza == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1101005019, true); //8-bit Unicorn - M762
                                else if (skingroza == 2)
                                    DeadBoxPointer->ChangeItemAvatar(1101005052, true); //GACKT MOONSAGA-M762
                                else if (skingroza == 3)
                                    DeadBoxPointer->ChangeItemAvatar(1101005025, true); //Lotus Fury - M762
                                else if (skingroza == 4)
                                    DeadBoxPointer->ChangeItemAvatar(1101005038, true); //Messi Football Icon M762
                            }
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "Kar98K")) {
                                if (skinkar == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1103001060, true); //8-bit Unicorn - M762
                                else if (skinkar == 2)
                                    DeadBoxPointer->ChangeItemAvatar(1103001079, true); //GACKT MOONSAGA-M762
                                else if (skinkar == 3)
                                    DeadBoxPointer->ChangeItemAvatar(1103001085, true); //Lotus Fury - M762
                                else if (skinkar == 4)
                                    DeadBoxPointer->ChangeItemAvatar(1103001101, true); //Messi Football Icon M762
                            }
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "M24")) {
                                if (skinm24 == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1103002018, true); //8-bit Unicorn - M762
                                else if (skinm24 == 2)
                                    DeadBoxPointer->ChangeItemAvatar(1103002030, true); //GACKT MOONSAGA-M762
                                else if (skinm24 == 3)
                                    DeadBoxPointer->ChangeItemAvatar(1103002049, true); //Lotus Fury - M762
                                else if (skinm24 == 4)
                                    DeadBoxPointer->ChangeItemAvatar(1103002047, true); //Messi Football Icon M762
                                else if (skinm24 == 5)
                                    DeadBoxPointer->ChangeItemAvatar(1103002059, true); //Messi Football Icon M762
                            }
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "AWM")) {
                                if (skinawm == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1103003022, true); //8-bit Unicorn - M762
                                else if (skinawm == 2)
                                    DeadBoxPointer->ChangeItemAvatar(1103003030, true); //GACKT MOONSAGA-M762
                                else if (skinawm == 3)
                                    DeadBoxPointer->ChangeItemAvatar(1103003042, true); //Lotus Fury - M762
                                else if (skinawm == 4)
                                    DeadBoxPointer->ChangeItemAvatar(1103003062, true); //Messi Football Icon M762
                            }
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "DP-28")) {
                                if (skindp28 == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1105002018, true); //8-bit Unicorn - M762
                                else if (skindp28 == 2)
                                    DeadBoxPointer->ChangeItemAvatar(1105002035, true); //GACKT MOONSAGA-M762
                            }
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "AUG")) {
                                if (skinm249 == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1105001034, true); //8-bit Unicorn - M762
                                else if (skinm249 == 2)
                                    DeadBoxPointer->ChangeItemAvatar(1105001020, true); //GACKT MOONSAGA-M762
                                else if (skinm249 == 3)
                                    DeadBoxPointer->ChangeItemAvatar(1105001048, true); //Lotus Fury - M762
                            }
                            if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "M16A4")) {
                                if (skinm16a4 == 1)
                                    DeadBoxPointer->ChangeItemAvatar(1101002029, true); //8-bit Unicorn - M762
                                else if (skinm16a4 == 2)
                                    DeadBoxPointer->ChangeItemAvatar(1101002056, true); //GACKT MOONSAGA-M762
                                else if (skinm16a4 == 3)
                                    DeadBoxPointer->ChangeItemAvatar(1101002068, true); //Lotus Fury - M762
                                else if (skinm16a4 == 4)
                                    DeadBoxPointer->ChangeItemAvatar(1101002081, true); //Messi Football Icon M762
                            }
                        }
                    }
            }
        }
    }






    return oProcessEvent(pObj, pFunc, pArgs);
}



DefineHook(int, sub_288C090, (int a1, int a2))
{
    auto GWorld = GetWorld();
    if (GWorld) {
        if (GWorld->NetDriver->ServerConnection)
            if (GWorld->NetDriver->ServerConnection->PlayerController) {
                ASTExtraPlayerController* localController = (ASTExtraPlayerController*)GWorld->NetDriver->ServerConnection->PlayerController;
                uint32_t key = *(int*)(a2 + 0x70);
                if (key == localController->PlayerKey) {
                    ASTExtraPlayerCharacter* localPlayer = (ASTExtraPlayerCharacter*)localController->AcknowledgedPawn;
                    if (xsuit == 1)
                        *(int*)(a2 + 0x7c) = 1405909; //blood raven x suit
                    if (xsuit == 2)
                        *(int*)(a2 + 0x7c) = 1405628; //Golden Pharaoh X-Suit


                    if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "AKM")) {
                        if (skinakm == 1)
                            *(int*)(a2 + 0x78) = 1101001037; //Sculpture - AKM
                        if (skinakm == 2)
                            *(int*)(a2 + 0x78) = 1101001057; //The Seven Seas - AKM
                        if (skinakm == 3)
                            *(int*)(a2 + 0x78) = 1101001065; //Roaring Tiger - AKM
                        if (skinakm == 4)
                            *(int*)(a2 + 0x78) = 1101001089; //Glacier - AKM
                        if (skinakm == 5)
                            *(int*)(a2 + 0x78) = 1101001103; //Desert Fossil - AKM
                        if (skinakm == 6)
                            *(int*)(a2 + 0x78) = 1101001116; //Jack-o'-lantern - AKM
                        if (skinakm == 7)
                            *(int*)(a2 + 0x78) = 1101001128; //Ghillie Dragon - AKM 
                        if (skinakm == 8)
                            *(int*)(a2 + 0x78) = 1101001143; //Gold Pirate - AKM
                        if (skinakm == 9)
                            *(int*)(a2 + 0x78) = 1101001174; //Wandering Tyrant - AKM
                        if (skinakm == 10)
                            *(int*)(a2 + 0x78) = 1101001213; //Star Admiral - AKM
                        if (skinakm == 12)
                            *(int*)(a2 + 0x78) = 1101001023; //Hellfire - AKM                 				
                    }

                    else if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "M416")) {
                        if (skinm4 == 1)
                            *(int*)(a2 + 0x78) = 1101004044; //Glacier - M416 
                        else if (skinm4 == 2)
                            *(int*)(a2 + 0x78) = 1101004062; //The Fool - M416
                        else if (skinm4 == 3)
                            *(int*)(a2 + 0x78) = 1101004086; //Lizard Roar - M416
                        else if (skinm4 == 4)
                            *(int*)(a2 + 0x78) = 1101004078; //Wanderer - M416
                        else if (skinm4 == 5)
                            *(int*)(a2 + 0x78) = 1101004098; //Call of the Wild - M416
                        else if (skinm4 == 6)
                            *(int*)(a2 + 0x78) = 1101004163; //Shinobi Kami- M416
                        else if (skinm4 == 7)
                            *(int*)(a2 + 0x78) = 1101004201; //Shinobi Kami- M416
                        else if (skinm4 == 8)
                            *(int*)(a2 + 0x78) = 1101004138; //Shinobi Kami- M416
                        else if (skinm4 == 9)
                            *(int*)(a2 + 0x78) = 1101004218; //Shinobi Kami- M416
                        else if (skinm4 == 10)
                            *(int*)(a2 + 0x78) = 1101004209; //Shinobi Kami- M416
                    }

                    else if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "SCAR-L")) {
                        if (skinscar == 1)
                            *(int*)(a2 + 0x78) = 1101003057; //Water Blaster - SCAR-L
                        else if (skinscar == 2)
                            *(int*)(a2 + 0x78) = 1101003070; //Enchanted Pumpkin - SCAR-L
                        else if (skinscar == 3)
                            *(int*)(a2 + 0x78) = 1101003079; //Operation Tomorrow - SCAR-L
                        else if (skinscar == 4)
                            *(int*)(a2 + 0x78) = 1101003099; //Drop the Bass - SCAR-L 
                        else if (skinscar == 5)
                            *(int*)(a2 + 0x78) = 1101003119; //Hextech Crystal - SCAR-L 
                        else if (skinscar == 6)
                            *(int*)(a2 + 0x78) = 1101003146; //THORN OF MALICE - SCAR-L 
                        else if (skinscar == 7)
                            *(int*)(a2 + 0x78) = 1101003181; //THORN OF MALICE - SCAR-L 

                    }
                    else if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "M762")) {

                        if (skinm7 == 1)
                            *(int*)(a2 + 0x78) = 1101008026; //8-bit Unicorn - M762
                        else if (skinm7 == 2)
                            *(int*)(a2 + 0x78) = 1101008070; //GACKT MOONSAGA-M762
                        else if (skinm7 == 3)
                            *(int*)(a2 + 0x78) = 1101008036; //Lotus Fury - M762
                        else if (skinm7 == 4)
                            *(int*)(a2 + 0x78) = 1101008116; //Messi Football Icon M762
                        else if (skinm7 == 5)
                            *(int*)(a2 + 0x78) = 1101008051; //Concerto of Love - M762
                        else if (skinm7 == 6)
                            *(int*)(a2 + 0x78) = 1101008104; //StarCore-M762
                        else if (skinm7 == 7)
                            *(int*)(a2 + 0x78) = 1101008081; //Stray Rebellion - M762
                        // *(int*)(a2 + 0x78) = 1101008026; //8-bit unicorn

                    }
                    else if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "UZI")) {
                        if (skinuzi == 1)
                            *(int*)(a2 + 0x78) = 1102001024; //Savagery - UZI
                        if (skinuzi == 2)
                            *(int*)(a2 + 0x78) = 1102001036; //Ethereal Emblem - UZI
                        if (skinuzi == 3)
                            *(int*)(a2 + 0x78) = 1102001058; //Romantic Moments - UZI
                        if (skinuzi == 4)
                            *(int*)(a2 + 0x78) = 1102001069; //Shimmer Power - UZI


                    }
                    else if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "UMP45")) {

                        if (skinump45 == 1)
                            *(int*)(a2 + 0x78) = 1102002043;
                        if (skinump45 == 2)
                            *(int*)(a2 + 0x78) = 1102002053;
                        if (skinump45 == 3)
                            *(int*)(a2 + 0x78) = 1102002061;
                        if (skinump45 == 4)
                            *(int*)(a2 + 0x78) = 1102002070;
                        if (skinump45 == 5)
                            *(int*)(a2 + 0x78) = 1102002030;
                        if (skinump45 == 6)
                            *(int*)(a2 + 0x78) = 1102002090;
                        if (skinump45 == 7)
                            *(int*)(a2 + 0x78) = 1102002136;

                    }
                    else if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "Vector")) {

                        if (skinvector == 1)
                            *(int*)(a2 + 0x78) = 1102003020;
                        if (skinvector == 2)
                            *(int*)(a2 + 0x78) = 1102003031;
                        if (skinvector == 3)
                            *(int*)(a2 + 0x78) = 1102003039;
                        if (skinvector == 4)
                            *(int*)(a2 + 0x78) = 1102003072;
                        if (skinvector == 5)
                            *(int*)(a2 + 0x78) = 1102003060;

                    }
                    else if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "Thompson")) {

                        if (skinThompson == 1)
                            *(int*)(a2 + 0x78) = 1102003060;  //candy cane

                    }

                    else if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "PP-19 Bizon")) {

                        if (skinbizon == 1)
                            *(int*)(a2 + 0x78) = 1102005007;
                        if (skinbizon == 2)
                            *(int*)(a2 + 0x78) = 1102005020;

                    }
                    else if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "Groza")) {

                        if (skingroza == 1)
                            *(int*)(a2 + 0x78) = 1101005019;
                        if (skingroza == 2)
                            *(int*)(a2 + 0x78) = 1101005052;
                        if (skingroza == 3)
                            *(int*)(a2 + 0x78) = 1101005025;
                        if (skingroza == 4)
                            *(int*)(a2 + 0x78) = 1101005038;


                    }
                    else if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "Kar98K")) {

                        if (skinkar == 1)
                            *(int*)(a2 + 0x78) = 1103001060;
                        if (skinkar == 2)
                            *(int*)(a2 + 0x78) = 1103001079;
                        if (skinkar == 3)
                            *(int*)(a2 + 0x78) = 1103001085;
                        if (skinkar == 4)
                            *(int*)(a2 + 0x78) = 1103001101;

                    }
                    else if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "M24")) {

                        if (skinm24 == 1)
                            *(int*)(a2 + 0x78) = 1103002018;
                        if (skinm24 == 2)
                            *(int*)(a2 + 0x78) = 1103002030;
                        if (skinm24 == 3)
                            *(int*)(a2 + 0x78) = 1103002049;
                        if (skinm24 == 4)
                            *(int*)(a2 + 0x78) = 1103002047;
                        if (skinm24 == 5)
                            *(int*)(a2 + 0x78) = 1103002059;

                    }
                    else if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "AWM")) {

                        if (skinawm == 1)
                            *(int*)(a2 + 0x78) = 1103003022;
                        if (skinawm == 2)
                            *(int*)(a2 + 0x78) = 1103003030;
                        if (skinawm == 3)
                            *(int*)(a2 + 0x78) = 1103003042;
                        if (skinawm == 4)
                            *(int*)(a2 + 0x78) = 1103003062;

                    }
                    else if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "DP-28")) {

                        if (skindp28 == 1)
                            *(int*)(a2 + 0x78) = 1105002018;
                        if (skindp28 == 2)
                            *(int*)(a2 + 0x78) = 1105002035;

                    }
                    else if (strstr(localPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "Pan")) {

                        *(int*)(a2 + 0x78) = 1108004125; //Honeypot

                    }
                    else if (strstr(g_LocalPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "Vss")) {
                        if (skinvss == 1)
                            *(int*)(a2 + 0x78) = 1103005024;
                    }
                    else if (strstr(g_LocalPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "MK14")) {
                        if (skinmk14 == 1)
                            *(int*)(a2 + 0x78) = 1103007020;
                        if (skinmk14 == 2)
                            *(int*)(a2 + 0x78) = 1103007028;
                    }
                    else if (strstr(g_LocalPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "S1897")) {
                        if (skins1897 == 1)
                            *(int*)(a2 + 0x78) = 1104002022;
                    }
                    else if (strstr(g_LocalPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "AUG")) {
                        if (skinaug == 1)
                            *(int*)(a2 + 0x78) = 1101006033;
                        if (skinaug == 2)
                            *(int*)(a2 + 0x78) = 1101006044;
                        if (skinaug == 3)
                            *(int*)(a2 + 0x78) = 1101006062;


                    }
                    else if (strstr(g_LocalPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "S12K")) {
                        if (skins12k == 1)
                            *(int*)(a2 + 0x78) = 1104003026;
                    }



                    else if (strstr(g_LocalPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "M249")) {
                        if (skinm249 == 1)
                            *(int*)(a2 + 0x78) = 1105001034;
                        if (skinm249 == 2)
                            *(int*)(a2 + 0x78) = 1105001020;
                        if (skinm249 == 3)
                            *(int*)(a2 + 0x78) = 1105001048;
                    }

                    else if (strstr(g_LocalPlayer->WeaponManagerComponent->CurrentWeaponReplicated->GetWeaponName().ToString(), "M16A4")) {
                        if (skinm16a4 == 1)
                            *(int*)(a2 + 0x78) = 1101002029;
                        if (skinm16a4 == 2)
                            *(int*)(a2 + 0x78) = 1101002056;
                        if (skinm16a4 == 3)
                            *(int*)(a2 + 0x78) = 1101002068;
                        if (skinm16a4 == 4)
                            *(int*)(a2 + 0x78) = 1101002081;
                    }
                }
            }
    }
    return Orig_sub_288C090(a1, a2);
}
void AddText(const ImFont* font, float font_size, const ImVec2& pos, ImColor col, const char* text_begin, bool bCenter, bool bOutLine)
{
    ImVec2 TextSize = font->CalcTextSizeA(font_size, FLT_MAX, 0.0f, text_begin);
    if (bOutLine)
    {
        ImGui::GetForegroundDrawList()->AddText(font, font_size, ImVec2((bCenter ? pos.x - TextSize.x / 2.0f : pos.x) + 1.0f, pos.y + 1.0f), IM_COL32(0, 0, 0, 255), text_begin);
        ImGui::GetForegroundDrawList()->AddText(font, font_size, ImVec2((bCenter ? pos.x - TextSize.x / 2.0f : pos.x) - 1.0f, pos.y - 1.0f), IM_COL32(0, 0, 0, 255), text_begin);
        ImGui::GetForegroundDrawList()->AddText(font, font_size, ImVec2((bCenter ? pos.x - TextSize.x / 2.0f : pos.x) + 1.0f, pos.y - 1.0f), IM_COL32(0, 0, 0, 255), text_begin);
        ImGui::GetForegroundDrawList()->AddText(font, font_size, ImVec2((bCenter ? pos.x - TextSize.x / 2.0f : pos.x) - 1.0f, pos.y + 1.0f), IM_COL32(0, 0, 0, 255), text_begin);
    }
    ImGui::GetForegroundDrawList()->AddText(font, font_size, ImVec2(bCenter ? pos.x - TextSize.x / 2.0f : pos.x, pos.y), col, text_begin);
}

void* skin_thread(void*) {
    if (deadbox1) {
        Tools::Hook(reinterpret_cast<void*>(Tools::GetBaseAddress("libUE4.so") + 0x2CDE644),
            reinterpret_cast<void*>(Hook_sub_288C090), reinterpret_cast<void**>(&Orig_sub_288C090));
    }
    else {
        Tools::Hook((void*)(0x56E30000 + 0x2CDE644), (void*)Orig_sub_288C090, (void**)&Hook_sub_288C090);
    }
    return 0;
}
const char* GetVehicleName(ASTExtraVehicleBase* Vehicle) {
    switch (Vehicle->VehicleShapeType) {
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_Motorbike:
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_Motorbike_SideCart:
        return "Motorbike";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_Dacia:
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_HeavyDacia:
        return "Dacia";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_MiniBus:
        return "Mini Bus";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_PickUp:
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_PickUp01:
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_HeavyPickup:
        return "Pick Up";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_Buggy:
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_HeavyBuggy:
        return "Buggy";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_UAZ:
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_UAZ01:
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_UAZ02:
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_UAZ03:
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_HeavyUAZ:
        return "UAZ";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_PG117:
        return "PG117";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_Aquarail:
        return "Aquarail";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_Mirado:
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_Mirado01:
        return "Mirado";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_Rony:
        return "Rony";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_Scooter:
        return "Scooter";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_SnowMobile:
        return "Snow Mobile";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_TukTukTuk:
        return "Tuk Tuk";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_SnowBike:
        return "Snow Bike";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_Surfboard:
        return "Surf Board";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_Snowboard:
        return "Snow Board";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_Amphibious:
        return "Amphibious";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_LadaNiva:
        return "Lada Niva";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_UAV:
        return "UAV";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_MegaDrop:
        return "Mega Drop";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_Lamborghini:
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_Lamborghini01:
        return "Lamborghini";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_GoldMirado:
        return "Gold Mirado";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_BigFoot:
        return "Big Foot";
        break;
    case ESTExtraVehicleShapeType::ESTExtraVehicleShapeType__VST_HeavyUH60:
        return "UH60";
        break;
    default:
        return "Vehicle";
        break;
    }
    return "Vehicle";
}

void (*orig_shoot_event)(USTExtraShootWeaponComponent* thiz, FVector start, FRotator rot, void* unk1, int unk2) = 0;
void shoot_event(USTExtraShootWeaponComponent* thiz, FVector start, FRotator rot, ASTExtraShootWeapon* weapon, int unk1) {
    FVector ViewPosY{ 0, 0, 0 };
    if (g_LocalPlayer) {
        ViewPosY = g_LocalPlayer->GetBonePos("Head", {});
        ViewPosY.Z += 15.f;
    }

    if (Config.SilentAim.Enable) {
        ASTExtraPlayerCharacter* Target = GetTargetForAiming();

        if (Target) {
            bool triggerOk = false;
            if (Config.SilentAim.Trigger != EAimTrigger::None) {
                if (Config.SilentAim.Trigger == EAimTrigger::Shooting) {
                    triggerOk = g_LocalPlayer->bIsWeaponFiring;
                }
                else if (Config.SilentAim.Trigger == EAimTrigger::Scoping) {
                    triggerOk = g_LocalPlayer->bIsGunADS;
                }
                else if (Config.SilentAim.Trigger == EAimTrigger::Both) {
                    triggerOk = g_LocalPlayer->bIsWeaponFiring && g_LocalPlayer->bIsGunADS;
                }
                else if (Config.SilentAim.Trigger == EAimTrigger::Any) {
                    triggerOk = g_LocalPlayer->bIsWeaponFiring || g_LocalPlayer->bIsGunADS;
                }
            }
            else triggerOk = true;
            if (triggerOk) {

                FVector targetAimPos = Target->GetBonePos("Head", {});
                if (Config.SilentAim.Target == EAimTarget::Chest) {
                    targetAimPos.Z -= 17.0f;
                }
                UShootWeaponEntity* ShootWeaponEntityComponent = thiz->ShootWeaponEntityComponent;
                if (ShootWeaponEntityComponent) {
                    if (Config.SilentAim.Pred) {
                        ASTExtraVehicleBase* CurrentVehicle = Target->CurrentVehicle;
                        if (CurrentVehicle) {
                            FVector LinearVelocity = CurrentVehicle->ReplicatedMovement.LinearVelocity;

                            float dist = g_LocalPlayer->GetDistanceTo(Target);

                            auto timeToTravel = dist / ShootWeaponEntityComponent->BulletRange;

                            targetAimPos = UKismetMathLibrary::Add_VectorVector(targetAimPos, UKismetMathLibrary::Multiply_VectorFloat(LinearVelocity, timeToTravel));


                            targetAimPos.Z += LinearVelocity.Z * timeToTravel + 0.5 * Config.Line * timeToTravel * timeToTravel;
                        }
                        else {
                            FVector Velocity = Target->GetVelocity();
                            float dist = g_LocalPlayer->GetDistanceTo(Target);
                            auto timeToTravel = dist / ShootWeaponEntityComponent->BulletRange;


                            targetAimPos = UKismetMathLibrary::Add_VectorVector(targetAimPos, UKismetMathLibrary::Multiply_VectorFloat(Velocity, timeToTravel));

                            targetAimPos.Z += Velocity.Z * timeToTravel + 0.5 * Config.Line * timeToTravel * timeToTravel;

                        }
                    }
                    FVector fDir = UKismetMathLibrary::Subtract_VectorVector(targetAimPos, g_LocalController->PlayerCameraManager->CameraCache.POV.Location);
                    rot = UKismetMathLibrary::Conv_VectorToRotator(fDir);


                }
            }
        }
    }
    return orig_shoot_event(thiz, start, rot, weapon, unk1);
}
//=======================================================//

//3D BOX

bool W2S2(FVector worldPos, FVector2D* screenPos) {
    return g_LocalController->ProjectWorldLocationToScreen(worldPos, true, screenPos);
}
void Line(ImDrawList* draw, FVector2D origin, FVector2D dest, ImColor color)
{
    draw->AddLine({ origin.X, origin.Y }, { dest.X, dest.Y }, color, 1.0f);
}
void Box4Line(ImDrawList* draw, float thicc, int x, int y, int w, int h, int color) {
    int iw = w / 4;
    int ih = h / 4;
    // top
    draw->AddRect(ImVec2(x, y), ImVec2(x + iw, y), color, thicc);
    draw->AddRect(ImVec2(x + w - iw, y), ImVec2(x + w, y), color, thicc);
    draw->AddRect(ImVec2(x, y), ImVec2(x, y + ih), color, thicc);
    draw->AddRect(ImVec2(x + w - 1, y), ImVec2(x + w - 1, y + ih), color, thicc);;
    // bottom
    draw->AddRect(ImVec2(x, y + h), ImVec2(x + iw, y + h), color, thicc);
    draw->AddRect(ImVec2(x + w - iw, y + h), ImVec2(x + w, y + h), color, thicc);
    draw->AddRect(ImVec2(x, y + h - ih), ImVec2(x, y + h), color, thicc);
    draw->AddRect(ImVec2(x + w - 1, y + h - ih), ImVec2(x + w - 1, y + h), color, thicc);
}
void Box3D(ImDrawList* draw, FVector origin, Vector3 extends, ImColor col) {

    origin.X -= extends.X / 2.f;
    origin.Y -= extends.Y / 2.f;
    origin.Z -= extends.Z / 2.f;
    FVector one = origin;
    FVector two = origin; two.X += extends.X;
    FVector tree = origin; tree.X += extends.X; tree.Y += extends.Y;
    FVector four = origin; four.Y += extends.Y;

    FVector five = one; five.Z += extends.Z;
    FVector six = two; six.Z += extends.Z;
    FVector seven = tree; seven.Z += extends.Z;
    FVector eight = four; eight.Z += extends.Z;

    FVector2D s1, s2, s3, s4, s5, s6, s7, s8;
    if (W2S2(one, &s1) && W2S2(two, &s2) && W2S2(tree, &s3) && W2S2(four, &s4) &&
        W2S2(five, &s5) && W2S2(six, &s6) && W2S2(seven, &s7) && W2S2(eight, &s8))
    {

        Line(draw, s1, s2, col);
        Line(draw, s2, s3, col);
        Line(draw, s3, s4, col);
        Line(draw, s4, s1, col);

        Line(draw, s5, s6, col);
        Line(draw, s6, s7, col);
        Line(draw, s7, s8, col);
        Line(draw, s8, s5, col);

        Line(draw, s1, s5, col);
        Line(draw, s2, s6, col);
        Line(draw, s3, s7, col);
        Line(draw, s4, s8, col);

    }
}
//=======================================================//
void RotateArrows(std::array<Vector3, 7>& points, float rotation) {
    const auto points_center = (points.at(0) + points.at(1) + points.at(2)) / 3;
    for (auto& point : points) {
        point = point - points_center;
        const auto temp_x = point.X;
        const auto temp_y = point.Y;
        const auto theta = DEG2RAD(rotation);
        const auto c = cosf(theta);
        const auto s = sinf(theta);
        point.X = temp_x * c - temp_y * s;
        point.Y = temp_x * s + temp_y * c;
        point = point + points_center;
    }
}

void DrawOutlinedText(AHUD* HUD, FString Text, FVector2D Pos, FLinearColor Color, FLinearColor OutlineColor, bool isCenter = false) {
    UCanvas* Canvas = HUD->Canvas;
    Canvas->K2_DrawText(tslFont, Text, Pos, Color, 1.f, {}, {}, isCenter, isCenter, true, OutlineColor);
}
void LineE(ImDrawList* draw, Vector3 posFrom, Vector3 posTo, float Thickness, ImColor col) {
    draw->AddLine({ posFrom.X, posFrom.Y }, { posTo.X, posTo.Y }, col, 2.0f);
}
void DrawArrowsFilled(ImDrawList* draw, Vector3 xy1, Vector3 xy2, Vector3 xy3, Vector3 xy4, Vector3 xy5, Vector3 xy6, Vector3 xy7, float Thickness, ImColor col) {
    LineE(draw, xy1, xy2, Thickness, col);
    LineE(draw, xy2, xy3, Thickness, col);
    LineE(draw, xy3, xy7, Thickness, col);
    LineE(draw, xy7, xy6, Thickness, col);
    LineE(draw, xy6, xy5, Thickness, col);
    LineE(draw, xy5, xy4, Thickness, col);
    LineE(draw, xy4, xy1, Thickness, col);
}
//-------------------------------------------------------------------------------------------------------------------------------------//
void DrawESP(ImDrawList* draw) {

    auto Actors = getActors();

    int totalEnemies = 0, totalBots = 0;

    ASTExtraPlayerCharacter* localPlayer = 0;
    ASTExtraPlayerController* localController = 0;

    ImFont* Font1 = ImGui::GetFont();




    for (int i = 0; i < Actors.size(); i++) {
        auto Actor = Actors[i];
        if (isObjectInvalid(Actor))
            continue;

        if (Actor->IsA(ASTExtraPlayerController::StaticClass())) {
            localController = (ASTExtraPlayerController*)Actor;
            break;
        }
    }

    if (localController) {
        for (int i = 0; i < Actors.size(); i++) {
            auto Actor = Actors[i];
            if (isObjectInvalid(Actor))
                continue;

            if (Actor->IsA(ASTExtraPlayerCharacter::StaticClass())) {
                if (((ASTExtraPlayerCharacter*)Actor)->PlayerKey == localController->PlayerKey) {
                    localPlayer = (ASTExtraPlayerCharacter*)Actor;
                    break;
                }
            }
        }

        if (localPlayer) {
            if (localPlayer->PartHitComponent) {
                auto ConfigCollisionDistSqAngles = localPlayer->PartHitComponent->ConfigCollisionDistSqAngles;
                for (int j = 0; j < ConfigCollisionDistSqAngles.Num(); j++) {
                    ConfigCollisionDistSqAngles[j].Angle = 180.0f;
                }
                localPlayer->PartHitComponent->ConfigCollisionDistSqAngles = ConfigCollisionDistSqAngles;
            }

            if (Config.SilentAim.Enable) {
                auto WeaponManagerComponent = localPlayer->WeaponManagerComponent;
                if (WeaponManagerComponent) {
                    auto propSlot = WeaponManagerComponent->GetCurrentUsingPropSlot();
                    if ((int)propSlot.GetValue() >= 1 && (int)propSlot.GetValue() <= 3) {
                        auto CurrentWeaponReplicated = (ASTExtraShootWeapon*)WeaponManagerComponent->CurrentWeaponReplicated;
                        if (CurrentWeaponReplicated) {
                            auto ShootWeaponComponent = CurrentWeaponReplicated->ShootWeaponComponent;
                            if (ShootWeaponComponent) {
                                int shoot_event_idx = 168;
                                auto VTable = (void**)ShootWeaponComponent->VTable;
                                // CHANGE22222 add lambda function f_mprotect
                                auto f_mprotect = [](uintptr_t addr, size_t len, int32_t prot) -> int32_t {
                                    static_assert(PAGE_SIZE == 4096);
                                    constexpr size_t page_size = static_cast<size_t>(PAGE_SIZE);
                                    void* start = reinterpret_cast<void*>(addr & -page_size);
                                    uintptr_t end = (addr + len + page_size - 1) & -page_size;
                                    return mprotect(start, end - reinterpret_cast<uintptr_t>(start), prot);
                                    };
                                if (VTable && (VTable[shoot_event_idx] != shoot_event)) {
                                    orig_shoot_event = decltype(orig_shoot_event)(
                                        VTable[shoot_event_idx]);
                                    // CHANGE22222 add call of f_mprotect
                                    f_mprotect((uintptr_t)(&VTable[shoot_event_idx]), sizeof(uintptr_t), PROT_READ | PROT_WRITE);
                                    VTable[shoot_event_idx] = (void*)shoot_event;
                                }
                            }
                        }
                    }
                }
            }
            FVector ViewPosY{ 0, 0, 0 };
            if (localPlayer) {
                ViewPosY = localPlayer->GetBonePos("Head", {});
                ViewPosY.Z += 10.f;
            }
            //Aimbot//
            if (Config.AimBot.Enable) {
                ASTExtraPlayerCharacter* Target = GetTargetByCrossDist();
                if (Target) {
                    bool triggerOk = false;
                    if (Config.SilentAim.Trigger != EAimTrigger::None) {
                        if (Config.SilentAim.Trigger == EAimTrigger::Shooting) {
                            triggerOk = localPlayer->bIsWeaponFiring;
                        }
                        else if (Config.SilentAim.Trigger == EAimTrigger::Scoping) {
                            triggerOk = localPlayer->bIsGunADS;
                        }
                        else if (Config.SilentAim.Trigger == EAimTrigger::Both) {
                            triggerOk = localPlayer->bIsWeaponFiring && localPlayer->bIsGunADS;
                        }
                        else if (Config.SilentAim.Trigger == EAimTrigger::Any) {
                            triggerOk = localPlayer->bIsWeaponFiring || localPlayer->bIsGunADS;
                        }
                    }
                    else triggerOk = true;
                    if (triggerOk) {
                        FVector targetAimPos = Target->GetBonePos("Head", {});
                        if (Config.SilentAim.Target == EAimTarget::Chest)
                        {
                            targetAimPos.Z -= 25.0f;
                        }

                        auto WeaponManagerComponent = localPlayer->WeaponManagerComponent;
                        if (WeaponManagerComponent)
                        {
                            auto propSlot = WeaponManagerComponent->GetCurrentUsingPropSlot();
                            if ((int)propSlot.GetValue() >= 1 && (int)propSlot.GetValue() <= 3)
                            {
                                auto CurrentWeaponReplicated = (ASTExtraShootWeapon*)WeaponManagerComponent->CurrentWeaponReplicated;
                                if (CurrentWeaponReplicated)
                                {
                                    auto ShootWeaponComponent = CurrentWeaponReplicated->ShootWeaponComponent;
                                    if (ShootWeaponComponent)
                                    {
                                        UShootWeaponEntity* ShootWeaponEntityComponent = ShootWeaponComponent->ShootWeaponEntityComponent;
                                        if (ShootWeaponEntityComponent)
                                        {
                                            /*   ASTExtraVehicleBase *CurrentVehicle = Target->CurrentVehicle;
                                               if (CurrentVehicle)
                                               {
                                                   FVector LinearVelocity = CurrentVehicle->ReplicatedMovement.LinearVelocity;
                                                   float dist = localPlayer->GetDistanceTo(Target);
                                                   auto timeToTravel = dist / ShootWeaponEntityComponent->BulletFireSpeed;
                                                   targetAimPos = UKismetMathLibrary::Add_VectorVector(targetAimPos, UKismetMathLibrary::Multiply_VectorFloat(LinearVelocity, timeToTravel));
                                               }
                                               else
                                               {
                                                   FVector Velocity = Target->GetVelocity();
                                                   float dist = localPlayer->GetDistanceTo(Target);
                                                   auto timeToTravel = dist / ShootWeaponEntityComponent->BulletFireSpeed;
                                                   targetAimPos = UKismetMathLibrary::Add_VectorVector(targetAimPos, UKismetMathLibrary::Multiply_VectorFloat(Velocity, timeToTravel));
                                               }*/
                                            if (Config.AimBot.Enable) {
                                                if (g_LocalPlayer->bIsGunADS) {
                                                    if (g_LocalPlayer->bIsWeaponFiring) {
                                                        float dist = g_LocalPlayer->GetDistanceTo(Target) / 100.f;
                                                        targetAimPos.Z -= dist * Config.SilentAim.Recc;
                                                        Config.SilentAim.Recc = 1.200;

                                                    }
                                                }
                                            }
                                            localController->SetControlRotation(ToRotator(localController->PlayerCameraManager->CameraCache.POV.Location, targetAimPos), "");
                                        }
                                    }
                                }
                            }
                        }
                    }
                }
            }
			
			          if (Config.PlayerESP.wide_view)
                     localPlayer->ThirdPersonCameraComponent->SetFieldOfView(Config.PlayerESP.set_field_of_view);
            //      if (g_LocalPlayer -> AvatarComponent2) {
            //  auto AvatarComp = g_LocalPlayer -> AvatarComponent2;
            //  FNetAvatarSyncData NetAvatarComp = * (FNetAvatarSyncData * )((uintptr_t) AvatarComp + 0x2A0);//NetAvatarSyncData NetAvatarData;//[Offset:
            //  auto Slotsybc = NetAvatarComp.SlotSyncData;

            //  Slotsybc[5].ItemId = new_Skin.XSuits;
            //}

            for (int i = 0; i < Actors.size(); i++) {
                auto Actor = Actors[i];
                if (isObjectInvalid(Actor))
                    continue;
                long Pl;
                if (Actor->IsA(ASTExtraPlayerCharacter::StaticClass())) {
                    long PlayerBoxClrCf = IM_COL32(0, 255, 47, 255);
                    long PlayerBoxClrCf2 = IM_COL32(0, 255, 47, 25);
                    auto Player = (ASTExtraPlayerCharacter*)Actor;
                    if (!localController->LineOfSightTo(Player, { 0, 0, 0 }, true)) {
                        PlayerBoxClrCf = IM_COL32(255, 119, 0, 255);
                        PlayerBoxClrCf2 = IM_COL32(255, 119, 0, 25);
                    }

                    float Distance = localPlayer->GetDistanceTo(Player) / 100.0f;
                    if (Distance > 500.0f)
                        continue;

                    if (Player->PlayerKey == localController->PlayerKey)
                        continue;

                    if (Player->TeamID == localController->TeamID)
                        continue;

                    if (Player->bDead)
                        continue;

                    if (!Player->RootComponent)
                        continue;

                    if (Player->bEnsure)
                        totalBots++;
                    else totalEnemies++;

                    if (Config.Alert360) {
                        bool ITACH = false; FVector MyPosition, EnemyPosition;
                        ASTExtraVehicleBase* CurrentVehiclea = Player->CurrentVehicle;
                        if (CurrentVehiclea) {
                            MyPosition = CurrentVehiclea->RootComponent->RelativeLocation;
                        }
                        else {
                            MyPosition = Player->RootComponent->RelativeLocation;
                        } ASTExtraVehicleBase* CurrentVehicle = localPlayer->CurrentVehicle;
                        if (CurrentVehicle) {
                            EnemyPosition = CurrentVehicle->RootComponent->RelativeLocation;
                        }
                        else {
                            EnemyPosition = localPlayer->RootComponent->RelativeLocation;
                        }FVector EntityPos = WorldToRadar(localController->PlayerCameraManager->CameraCache.POV.Rotation.Yaw, MyPosition, EnemyPosition, NULL, NULL, Vector3(glWidth, glHeight, 0), ITACH);
                        FVector angle = FVector();
                        Vector3 forward = Vector3((float)(glWidth / 2) - EntityPos.X, (float)(glHeight / 2) - EntityPos.Y, 0.0f);
                        VectorAnglesRadar(forward, angle);
                        const auto angle_yaw_rad = DEG2RAD(angle.Y + 180.f);
                        const auto new_point_x = (glWidth / 2) + (64) / 2 * 8 * cosf(angle_yaw_rad);
                        const auto new_point_y = (glHeight / 2) + (64) / 2 * 8 * sinf(angle_yaw_rad);
                        std::array<Vector3, 7> points{
                        Vector3(new_point_x - (5.6f * (float)1.5f), new_point_y - (7.31272f * 1.5272f)),
                        Vector3(new_point_x + (10.607f * 1.529f) , new_point_y),
                        Vector3(new_point_x - (5.6282f * 1.529f), new_point_y + (7.308828f * 1.5383f)),
                        Vector3(new_point_x - (5.6702f * 1.5899f) , new_point_y - (4.30282f * 1.5282f)),
                        Vector3(new_point_x - (17.5718f * 1.53822f) , new_point_y - (4.30282f * 1.5282f)),
                        Vector3(new_point_x - (17.5292f * 1.522f) , new_point_y + (4.30828f * 1.5282f)),
                        Vector3(new_point_x - (5.628f * 1.5229f) , new_point_y + (4.30238f * 1.5282f)) };
                        RotateArrows(points, angle.Y + 180.f);
                        bool IsVisible = localController->LineOfSightTo(Player, { 0, 0, 0 }, true);
                        DrawArrowsFilled(draw, points.at(0), points.at(1), points.at(2), points.at(3), points.at(4), points.at(5), points.at(6), 1.5, PlayerBoxClrCf2);
                        draw->AddTriangleFilled(ImVec2(points.at(0).X, points.at(0).Y), ImVec2(points.at(1).X, points.at(1).Y), ImVec2(points.at(2).X, points.at(2).Y), Pl);
                        std::string s;
                        s += std::to_string((int)Distance);/*            0...D      */
                        if (IsVisible) {                  /*           /|\        */
                            if (Player->bEnsure) {             /*           / \        */
                            }
                            else {
                                auto textSize = ImGui::CalcTextSize(s.c_str(), 0, ((float)density / 20.0f));
                                draw->AddText(NULL, ((float)density / 12.0f), { new_point_x - (textSize.x / 2), new_point_y + 7.1f }, IM_COL32(0, 0, 0, 255), s.c_str());
                                draw->AddText(NULL, ((float)density / 12.0f), { new_point_x - (textSize.x / 2), new_point_y + 6.9f }, IM_COL32(0, 0, 0, 255), s.c_str());
                                draw->AddText(NULL, ((float)density / 12.0f), { new_point_x - (textSize.x / 2), new_point_y + 7.f }, IM_COL32(255, 0, 0, 255), s.c_str());

                            }
                        }
                        else {
                            if (Player->bEnsure) {
                            }
                            else {
                                auto textSize = ImGui::CalcTextSize(s.c_str(), 0, ((float)density / 20.0f));
                                draw->AddText(NULL, ((float)density / 12.0f), { new_point_x - (textSize.x / 2), new_point_y + 7.1f }, IM_COL32(0, 0, 0, 255), s.c_str());
                                draw->AddText(NULL, ((float)density / 12.0f), { new_point_x - (textSize.x / 2), new_point_y + 6.9f }, IM_COL32(0, 0, 0, 255), s.c_str());
                                draw->AddText(NULL, ((float)density / 12.0f), { new_point_x - (textSize.x / 2), new_point_y + 7.f }, IM_COL32(255, 255, 0, 255), s.c_str());

                            }
                        }
                    }

                    if (Config.Hide_Bot)
                        if (Player->bEnsure)
                            continue;
                    float magic_number = (Distance);
                    float mx = (glWidth / 4) / magic_number;

                    float healthLength = glWidth / 19;
                    if (healthLength < mx)
                        healthLength = mx;

                    auto HeadPos = Player->GetBonePos("Head", {});
                    ImVec2 HeadPosSC;

                    auto RootPos = Player->GetBonePos("Root", {});
                    ImVec2 RootPosSC;
                    auto upper_r = Player->GetBonePos("upperarm_r", {});
                    ImVec2 upper_rPoSC;
                    auto lowerarm_r = Player->GetBonePos("lowerarm_r", {});
                    ImVec2 lowerarm_rPoSC;
                    auto hand_r = Player->GetBonePos("hand_r", {});
                    ImVec2 hand_rPoSC;
                    auto upper_l = Player->GetBonePos("upperarm_l", {});
                    ImVec2 upper_lPoSC;
                    auto lowerarm_l = Player->GetBonePos("lowerarm_l", {});
                    ImVec2 lowerarm_lSC;
                    auto hand_l = Player->GetBonePos("hand_l", {});
                    ImVec2 hand_lPoSC;
                    auto thigh_l = Player->GetBonePos("thigh_l", {});
                    ImVec2 thigh_lPoSC;
                    auto calf_l = Player->GetBonePos("calf_l", {});
                    ImVec2 calf_lPoSC;
                    auto foot_l = Player->GetBonePos("foot_l", {});
                    ImVec2 foot_lPoSC;
                    auto thigh_r = Player->GetBonePos("thigh_r", {});
                    ImVec2 thigh_rPoSC;
                    auto calf_r = Player->GetBonePos("calf_r", {});
                    ImVec2 calf_rPoSC;
                    auto foot_r = Player->GetBonePos("foot_r", {});
                    ImVec2 foot_rPoSC;
                    auto neck_01 = Player->GetBonePos("neck_01", {});
                    ImVec2 neck_01PoSC;

                    ImVec2 pelvisPoSC;
                    bool IsVisible = localController->LineOfSightTo(Player, { 0, 0, 0 }, true);

                    int SCOLOR, SCOLOR2;

                    if (IsVisible)
                    {
                        SCOLOR = ToColor(Config.ColorsESP.SkeletonVisible);
                        SCOLOR2 = IM_COL32(0, 255, 0, 255); // yeşil renk
                    }
                    else {
                        SCOLOR = ToColor(Config.ColorsESP.Skeleton);
                        SCOLOR2 = IM_COL32(255, 0, 0, 255);  // Kırmızı renk

                    }

                    FVector Root = Player->GetBonePos("Root", {});

                    FVector Spin2 = Player->GetBonePos("spine_03", {});

                    FVector ViewPosY{ 0, 0, 0 };
                    if (localPlayer) {
                        ViewPosY = localPlayer->GetBonePos("Head", {});
                        ViewPosY.Z += 10.f;
                    }





                    if (W2S(HeadPos, (FVector2D*)&HeadPosSC) && W2S(RootPos, (FVector2D*)&RootPosSC)) {



                        int SCOLOR;
                        // ======================================================================== //			
                        if (Config.PlayerESP.TeamID || Config.PlayerESP.Name || Config.PlayerESP.Distance)
                        {
                            float boxHeight = abs(HeadPosSC.y - RootPosSC.y);
                            float boxWidth = boxHeight * 0.65f;
                            std::string s;

                            if (Config.PlayerESP.TeamID)
                            {
                                s += "[";
                                s += std::to_string(Player->TeamID);
                                s += "]";
                            }

                            if (Config.PlayerESP.Name)
                            {
                                std::string name;
                                if (Player->bEnsure)
                                {
                                    name += "BOT";
                                }
                                else
                                {
                                    name += (u8"%s", Player->PlayerName.ToString());
                                }

                                auto nameSize = ImGui::CalcTextSize2(name.c_str(), 0, FONT_SIZE_FACTOR);
                                AddTextName(Font1, FONT_SIZE_FACTOR, { RootPosSC.x - (nameSize.x / 2.5), RootPosSC.y }, IM_COL32(200, 200, 0, 255), name.c_str(), false, false);

                            }

                            if (Config.PlayerESP.Distance)
                            {
                                if (!s.empty())
                                {
                                    s += " - ";
                                }
                                s += std::to_string((int)Distance);
                                s += "m";
                            }

                            auto textSize = ImGui::CalcTextSize2(s.c_str(), 0, FONT_SIZE_FACTOR);

                            // yeşil gölgelendirme ekle
                            AddText(Font1, FONT_SIZE_FACTOR,
                                { RootPosSC.x - (textSize.x / 2.5) + 1, RootPosSC.y + (textSize.x / 2.5) + 1 },
                                IM_COL32(0, 255, 0, 100), s.c_str(), false, false);
                            AddText(Font1, FONT_SIZE_FACTOR,
                                { RootPosSC.x - (textSize.x / 2.5) - 1, RootPosSC.y + (textSize.x / 2.5) - 1 },
                                IM_COL32(0, 255, 0, 100), s.c_str(), false, false);
                            AddText(Font1, FONT_SIZE_FACTOR,
                                { RootPosSC.x - (textSize.x / 2.5) + 1, RootPosSC.y + (textSize.x / 2.5) - 1 },
                                IM_COL32(0, 255, 0, 100), s.c_str(), false, false);
                            AddText(Font1, FONT_SIZE_FACTOR,
                                { RootPosSC.x - (textSize.x / 2.5) - 1, RootPosSC.y + (textSize.x / 2.5) + 1 },
                                IM_COL32(0, 255, 0, 100), s.c_str(), false, false);

                            // koyu siyah renkli metni çiz
                            AddText(Font1, FONT_SIZE_FACTOR,
                                { RootPosSC.x - (textSize.x / 2.5), RootPosSC.y + (textSize.x / 2.5) },
                                IM_COL32(0, 0, 0, 255), s.c_str(), false, false);


                        }


                        if (Config.PlayerESP.Health) {
                            int CurHP = (int)std::max(0, std::min((int)Player->Health, 100));
                            int MaxHP = 100;
                            long HpColor;

                            // Can rengine göre renk belirleme
                            if (Player->Health == 100.0f) {
                                HpColor = IM_COL32(43, 189, 65, 200);  // Yeşil renk, tam can
                            }
                            else {
                                HpColor = IM_COL32(255, 255, 0, 200);  // Sarı renk, azalmış can
                            }

                            // Can barını ortalamak için x koordinatlarını ayarlama
                            float barWidth = 50.0f;  // Can barı genişliği
                            float barHeight = 2.5f;  // Can barı yüksekliği
                            float barXStart = HeadPosSC.x - barWidth / 2;
                            float barXEnd = barXStart + (barWidth * (CurHP / (float)MaxHP));

                            // Can barını çizme
                            draw->AddRectFilled({ barXStart, HeadPosSC.y - 22 }, { barXEnd, HeadPosSC.y - 22 + barHeight }, HpColor, 0.0f, 0);
                            draw->AddRect({ barXStart - 1, HeadPosSC.y - 22 - 1 }, { barXStart + barWidth + 1, HeadPosSC.y - 22 + barHeight + 1 }, IM_COL32(0, 0, 0, 255), 0.0f, 0, 1.0f);

                            if (Player->Health == 0.0f && !Player->bDead) { //--<knocked
                                CurHP = (int)std::max(0, std::min((int)Player->NearDeathBreath, 100));
                                if (Player->NearDeatchComponent) {
                                    MaxHP = 100;
                                    HpColor = IM_COL32(255, 0, 0, 255);  // Kırmızı renk, knocked durumu

                                    // Knocked durumunda can barını çizme
                                    barXEnd = barXStart + (barWidth * (CurHP / (float)MaxHP));
                                    draw->AddRectFilled({ barXStart, HeadPosSC.y - 22 }, { barXEnd, HeadPosSC.y - 22 + barHeight }, HpColor, 0.0f, 0);
                                    draw->AddRect({ barXStart - 1, HeadPosSC.y - 22 - 1 }, { barXStart + barWidth + 1, HeadPosSC.y - 22 + barHeight + 1 }, IM_COL32(0, 0, 0, 255), 0.0f, 0, 1.0f);

                                }
                            }
                        }

                        if (Config.Line) {
                            draw->AddLine({ (float)glWidth / 2, 0 }, ImVec2(HeadPosSC.x, HeadPosSC.y - 55.0f), SCOLOR2, Config.L_size);
                        }


                        if (Config.PlayerESP.Box)
                        {
                            float boxHeight = abs(HeadPosSC.y - RootPosSC.y);
                            float boxWidth = boxHeight * 0.65f;
                            Box4Line(draw, 4.0, HeadPosSC.x - (boxWidth / 2), HeadPosSC.y, boxWidth, boxHeight, GetRandomColorByIndex(Player->TeamID));
                        }

                        if (Config.PlayerESP.LootBox)
                        {
                            if (Actors[i]->IsA(APickUpListWrapperActor::StaticClass()))
                            {
                                auto Pick = (APickUpListWrapperActor*)Actors[i];
                                if (!Pick->RootComponent)
                                    continue;
                                float Distance = Pick->GetDistanceTo(localPlayer) / 100.f;
                                FVector2D PickUpListsPos;
                                Vector3 origin, extends;

                                if (W2S(Pick->K2_GetActorLocation(), &PickUpListsPos))
                                {

                                    // std::string s;
                                    std::string s = "Dead Box";
                                    s += " - ";
                                    s += std::to_string((int)Distance);
                                    s += "M";
                                    draw->AddText(NULL, FONT_SIZE_FACTOR, { PickUpListsPos.X, PickUpListsPos.Y }, IM_COL32(255, 0, 0, 255), s.c_str());
                                }
                            }
                        }


                        if (Config.Radar)
                        {
                            bool out = false;
                            struct Vector3 Pos;
                            Pos.X = screenWidth / 4.395;
                            Pos.Y = screenHeight - 210 - (screenHeight / 500);
                            ;
                            struct Vector3 Size;
                            Size.X = 200; // Width of Radar Box.
                            Size.Y = 210; // Height of Radar Box.
                            float RadarCenterX = Pos.X + (Size.X / 2);
                            float RadarCenterY = Pos.Y + (Size.Y / 2);
                            ImColor CircleColor = ImColor(0, 0, 0, 20);
                            ImColor PointColor = ImColor(0, 255, 0, 255);
                            draw->AddLine(ImVec2(RadarCenterX, RadarCenterY), ImVec2(RadarCenterX, Pos.Y), IM_COL32(255, 0, 0, 255), 1.f);
                            draw->AddLine(ImVec2(RadarCenterX, RadarCenterY), ImVec2(Pos.X, RadarCenterY), IM_COL32(255, 0, 0, 255), 1.f);
                            draw->AddLine(ImVec2(Pos.X, RadarCenterY), ImVec2(Pos.X + Size.X, RadarCenterY), IM_COL32(255, 0, 0, 255), 1.f);
                            draw->AddLine(ImVec2(RadarCenterX, RadarCenterY), ImVec2(RadarCenterX, Pos.Y + Size.Y), IM_COL32(255, 0, 0, 255), 1.f);

                            draw->AddCircleFilled(ImVec2(RadarCenterX, RadarCenterY), 100.f, CircleColor, 1000);            // Background
                            draw->AddCircle(ImVec2(RadarCenterX, RadarCenterY), 100.f, PointColor, 1000);                   // Circle Around Background
                            draw->AddCircleFilled(ImVec2(RadarCenterX + 0.5f, RadarCenterY + 0.5f), 3.f, PointColor, 1000); // Center of Cross Ci
                        }
                        if (Config.Radar)
                        {
                            FVector MyPosition;
                            ASTExtraVehicleBase* CurrentVehiclea = Player->CurrentVehicle;
                            if (CurrentVehiclea)
                            {
                                MyPosition = CurrentVehiclea->RootComponent->RelativeLocation;
                            }
                            else
                            {
                                MyPosition = Player->RootComponent->RelativeLocation;
                            }
                            FVector EnemyPosition;
                            ASTExtraVehicleBase* CurrentVehicle = localPlayer->CurrentVehicle;
                            if (CurrentVehicle)
                            {
                                EnemyPosition = CurrentVehicle->RootComponent->RelativeLocation;
                            }
                            else
                            {
                                EnemyPosition = localPlayer->RootComponent->RelativeLocation;
                            }
                            bool out = false;
                            struct Vector3 Pos;
                            Pos.X = screenWidth / 4.395;
                            Pos.Y = screenHeight - 210 - (screenHeight / 500);
                            ;
                            struct Vector3 Size;
                            Size.X = 200; // Width of Radar Box.
                            Size.Y = 210; // Height of Radar Box.
                            float RadarCenterX = Pos.X + (Size.X / 2);
                            float RadarCenterY = Pos.Y + (Size.Y / 2);

                            bool IsVisible = true;
                            FVector RadarSketch = WorldToRadar(localController->PlayerCameraManager->CameraCache.POV.Rotation.Yaw, MyPosition, EnemyPosition, Pos.X, Pos.Y, Vector3(Size.X, Size.Y, 0), out);
                            if (Distance >= 0.f)
                            {
                                if (IsVisible)
                                {
                                    if (Player->bIsAI)
                                    {
                                        draw->AddCircle(ImVec2(RadarSketch.X, RadarSketch.Y), 5,
                                            IM_COL32(000, 255, 000, 255),
                                            100, 0.0f);
                                    }
                                    else
                                    {
                                        draw->AddCircle(ImVec2(RadarSketch.X, RadarSketch.Y), 5,
                                            IM_COL32(255, 000, 000, 255), 100,
                                            0.0f);
                                    }
                                }
                            }
                        }

                        if (Config.Team) {
                            std::string s;
                            auto textSize = ImGui::CalcTextSize(s.c_str(), 0);
                            if (Player->TeamID < 10) {
                                s += " 0";
                                s += std::to_string(Player->TeamID);
                                draw->AddText(basic, 30, ImVec2(HeadPosSC.x - 91.3 - (textSize.x / 2), HeadPosSC.y - 59.5), IM_COL32(0, 0, 0, 60), s.c_str());
                                draw->AddText(basic, 30, ImVec2(HeadPosSC.x - 92.3 - (textSize.x / 2), HeadPosSC.y - 60.5), IM_COL32(255, 255, 255, 255), s.c_str());

                            }
                            else if (Player->TeamID < 100) {
                                s += " ";
                                s += std::to_string(Player->TeamID);
                                draw->AddText(basic, 30, ImVec2(HeadPosSC.x - 90 - (textSize.x / 2), HeadPosSC.y - 59.5), IM_COL32(0, 0, 0, 60), s.c_str());
                                draw->AddText(basic, 30, ImVec2(HeadPosSC.x - 91 - (textSize.x / 2), HeadPosSC.y - 60.5), IM_COL32(255, 255, 255, 255), s.c_str());
                            }
                            else {
                                s += std::to_string(Player->TeamID);
                                draw->AddText(basic, 30, ImVec2(HeadPosSC.x - 91 - (textSize.x / 2), HeadPosSC.y - 59.5), IM_COL32(0, 0, 0, 60), s.c_str());
                                draw->AddText(basic, 30, ImVec2(HeadPosSC.x - 92 - 1 - (textSize.x / 2), HeadPosSC.y - 60.5), IM_COL32(255, 255, 255, 255), s.c_str());
                            }
                        }


                        if (Config.PlayerESP.Skeleton) {
                            static std::vector<std::string> right_arm{ "neck_01",
                                                                      "clavicle_r",
                                                                      "upperarm_r",
                                                                      "lowerarm_r",
                                                                      "hand_r", "item_r" };
                            static std::vector<std::string> left_arm{ "neck_01",
                                                                     "clavicle_l",
                                                                     "upperarm_l",
                                                                     "lowerarm_l",
                                                                     "hand_l", "item_l" };
                            static std::vector<std::string> spine{ "Head", "neck_01",
                                                                  "spine_03",
                                                                  "spine_02", "spine_01" };
                            static std::vector<std::string> lower_right{ "thigh_r",
                                                                        "calf_r", "foot_r" };
                            static std::vector<std::string> lower_left{ "thigh_l",
                                                                       "calf_l", "foot_l" };
                            static std::vector<std::vector<std::string>> skeleton{ right_arm,
                                                                                  left_arm,
                                                                                  spine,
                                                                                  lower_right,
                                                                                  lower_left };

                            for (auto& boneStructure : skeleton) {
                                std::string lastBone;
                                for (std::string& currentBone : boneStructure) {
                                    if (!lastBone.empty()) {
                                        ImVec2 boneFrom, boneTo;
                                        if (W2S(Player->GetBonePos(lastBone.c_str(), {}),
                                            (FVector2D*)&boneFrom) &&
                                            W2S(Player->GetBonePos(currentBone.c_str(), {}),
                                                (FVector2D*)&boneTo)) {
                                            draw->AddLine(boneFrom, boneTo,
                                                PlayerBoxClrCf, Config.S_size);
                                        }
                                    }
                                    lastBone = currentBone;
                                }
                            }
                        }



                    }


                }

                if (Config.Grenade)
                {
                    if (Actors[i]->IsA(ASTExtraGrenadeBase::StaticClass()))
                    {
                        auto grenade = (ASTExtraGrenadeBase*)Actors[i];
                        if (!grenade)
                            continue;
                        float Distance = grenade->GetDistanceTo(localPlayer) / 100.f;
                        if (Distance <= 500.f)
                        {
                            //   draw->AddText(NULL, 65.0f, ImVec2(glWidth / 3.0 - 50.f, 350), IM_COL32(255, 0, 0, 100), "!!! MOVE, MOVE, MOVE !!!");
                            FVector2D grenadePos;
                            if (W2S(grenade->K2_GetActorLocation(), &grenadePos))
                            {
                                std::string s = "[";
                                s += "Throwable-";
                                s += std::to_string((int)Distance);
                                s += "M]";

                                draw->AddText(NULL, FONT_SIZE_FACTOR,
                                    { grenadePos.X, grenadePos.Y },
                                    ImColor(isRed, isBlue, isGreen, 8.0f), s.c_str());
                            }
                        }
                    }
                }


                if (Config.Vehicle)
                {
                    if (Actors[i]->IsA(ASTExtraVehicleBase::StaticClass()))
                    {
                        auto Vehicle = (ASTExtraVehicleBase*)Actors[i];
                        if (!Vehicle->Mesh)
                            continue;

                        int CurHP = (int)std::max(0, std::min((int)Vehicle->VehicleCommon->HP, (int)Vehicle->VehicleCommon->HPMax));
                        int MaxHP = (int)Vehicle->VehicleCommon->HPMax;
                        long curHP_Color = IM_COL32(std::min(((510 * (MaxHP - CurHP)) / MaxHP), 255), std::min(((510 * CurHP) / MaxHP), 255), 0, 155);

                        float Distance = Vehicle->GetDistanceTo(localPlayer) / 100.f;
                        FVector2D vehiclePos;
                        if (W2S(Vehicle->K2_GetActorLocation(), &vehiclePos))
                        {
                            auto mWidthScale = std::min(0.10f * Distance, 50.f);
                            auto mWidth = 70.f - mWidthScale;
                            auto mHeight = mWidth * 0.15f;

                            std::string s = GetVehicleName(Vehicle);
                            s += " [";
                            s += std::to_string((int)Distance);
                            s += " M]";

                            // Beyaz gölgelendirmeyi kalınlaştırmak için farklı konumlarda birden fazla çizim yap
                            draw->AddText(NULL, FONT_SIZE_FACTOR,
                                { vehiclePos.X - (mWidth / 2) + 1, vehiclePos.Y + 1 },
                                IM_COL32(255, 255, 255, 100), s.c_str());
                            draw->AddText(NULL, FONT_SIZE_FACTOR,
                                { vehiclePos.X - (mWidth / 2) - 1, vehiclePos.Y - 1 },
                                IM_COL32(255, 255, 255, 100), s.c_str());
                            draw->AddText(NULL, FONT_SIZE_FACTOR,
                                { vehiclePos.X - (mWidth / 2) + 1, vehiclePos.Y - 1 },
                                IM_COL32(255, 255, 255, 100), s.c_str());
                            draw->AddText(NULL, FONT_SIZE_FACTOR,
                                { vehiclePos.X - (mWidth / 2) - 1, vehiclePos.Y + 1 },
                                IM_COL32(255, 255, 255, 100), s.c_str());

                            // Koyu mavi renkli metni çiz
                            draw->AddText(NULL, FONT_SIZE_FACTOR,
                                { vehiclePos.X - (mWidth / 2), vehiclePos.Y },
                                IM_COL32(0, 0, 0, 255), s.c_str());
                        }
                    }
                }
                if (Actors[i]->IsA(APickUpWrapperActor::StaticClass()))
                {
                    auto PickUp = (APickUpWrapperActor*)Actors[i];
                    if (Items[PickUp->DefineID.TypeSpecificID])
                    {
                        auto RootComponent = PickUp->RootComponent;
                        if (!RootComponent)
                            continue;

                        float Distance = PickUp->GetDistanceTo(localPlayer) / 100.f;

                        FVector2D itemPos;
                        if (W2S(PickUp->K2_GetActorLocation(), &itemPos))
                        {
                            std::string s;

                            for (auto& category : items_data)
                            {
                                for (auto& item : category["Items"])
                                {
                                    if (item["itemId"] == PickUp->DefineID.TypeSpecificID)
                                    {
                                        s = item["itemName"].get<std::string>();
                                        break;
                                    }
                                }
                            }

                            s += " - ";
                            s += std::to_string((int)Distance);
                            s += "m";

                            draw->AddText(NULL, FONT_SIZE_FACTOR, { itemPos.X, itemPos.Y }, IM_COL32(139, 0, 0, 255), s.c_str());
                        }
                    }
                }


            }


            int TotalCount = totalEnemies;
            int TotalCountt = totalBots;

            //Total Enemy//
            ImGui::GetForegroundDrawList()->AddRectFilled({ glWidth / 2 - 160,40 }, { glWidth / 2,80 }, ImColor(255, 0, 0, 200));
            ImGui::GetForegroundDrawList()->AddRect({ glWidth / 2 - 160,40 }, { glWidth / 2,80 }, ImColor(0, 0, 0, 250), 0, 0, 2.5f);
            ImGui::GetForegroundDrawList()->AddRectFilled({ glWidth / 2 + 160,40 }, { glWidth / 2,80 }, ImColor(255, 255, 255, 200));
            ImGui::GetForegroundDrawList()->AddRect({ glWidth / 2 + 160,40 }, { glWidth / 2,80 }, ImColor(0, 0, 0, 250), 0, 0, 2.5f);


            sprintf(extra, "PLAYER: %d ", totalEnemies);
            ImGui::GetForegroundDrawList()->AddText({ glWidth / 2 - 130,45 }, ImColor(0, 0, 0), extra);
            sprintf(extra, "BOT: %d", totalBots);
            ImGui::GetForegroundDrawList()->AddText({ glWidth / 2 + 25,45 }, ImColor(0, 0, 0), extra);
        }

        std::string credit = "";
        auto textSize = ImGui::CalcTextSize(credit.c_str(), 0, ((float)density / 10.5f));

        draw->AddText(NULL, ((float)density / 10.5f), { ((float)glWidth / 2) - (textSize.x / 2), 90 }, IM_COL32(255, 000, 000, 255), credit.c_str());

        ImGui::End();
        g_LocalController = localController;
        g_LocalPlayer = localPlayer;



    }
    if (Config.AimBot.Enable) {
        draw->AddCircle(ImVec2(glWidth / 2.0f, glHeight / 2.0f), Config.SilentAim.Cross * 0.5f, ToColor(Config.Fov), 100, 0.f);
    }

    if (Config.SilentAim.Enable) {
        draw->AddCircle(ImVec2(glWidth / 2.0f, glHeight / 2.0f), Config.SilentAim.Cross * 0.5f, ToColor(Config.Fov), 100, 0.f);
    }
}
// ======================================================================== //

std::string getClipboardText() {
    if (!g_App)
        return "";

    auto activity = g_App->activity;
    if (!activity)
        return "";

    auto vm = activity->vm;
    if (!vm)
        return "";

    auto object = activity->clazz;
    if (!object)
        return "";

    std::string result;

    JNIEnv* env;
    vm->AttachCurrentThread(&env, 0);
    {
        auto ContextClass = env->FindClass("android/content/Context");
        auto getSystemServiceMethod = env->GetMethodID(ContextClass, "getSystemService", "(Ljava/lang/String;)Ljava/lang/Object;");
        auto str = env->NewStringUTF("clipboard");
        auto clipboardManager = env->CallObjectMethod(object, getSystemServiceMethod, str);
        env->DeleteLocalRef(str);
        auto ClipboardManagerClass = env->FindClass("android/content/ClipboardManager");
        auto getText = env->GetMethodID(ClipboardManagerClass, "getText", "()Ljava/lang/CharSequence;");
        auto CharSequenceClass = env->FindClass("java/lang/CharSequence");
        auto toStringMethod = env->GetMethodID(CharSequenceClass, "toString", "()Ljava/lang/String;");
        auto text = env->CallObjectMethod(clipboardManager, getText);
        if (text) {
            str = (jstring)env->CallObjectMethod(text, toStringMethod);
            result = env->GetStringUTFChars(str, 0);
            env->DeleteLocalRef(str);
            env->DeleteLocalRef(text);
        }

        env->DeleteLocalRef(CharSequenceClass);
        env->DeleteLocalRef(ClipboardManagerClass);
        env->DeleteLocalRef(clipboardManager);
        env->DeleteLocalRef(ContextClass);
    }
    vm->DetachCurrentThread();

    return result;
}

// ======================================================================== //
const char* GetAndroidID(JNIEnv* env, jobject context) {
    jclass contextClass = env->FindClass(/*android/content/Context*/ StrEnc("`L+&0^[S+-:J^$,r9q92(as", "\x01\x22\x4F\x54\x5F\x37\x3F\x7C\x48\x42\x54\x3E\x3B\x4A\x58\x5D\x7A\x1E\x57\x46\x4D\x19\x07", 23).c_str());
    jmethodID getContentResolverMethod = env->GetMethodID(contextClass, /*getContentResolver*/ StrEnc("E8X\\7r7ys_Q%JS+L+~", "\x22\x5D\x2C\x1F\x58\x1C\x43\x1C\x1D\x2B\x03\x40\x39\x3C\x47\x3A\x4E\x0C", 18).c_str(), /*()Landroid/content/ContentResolver;*/ StrEnc("8^QKmj< }5D:9q7f.BXkef]A*GYLNg}B!/L", "\x10\x77\x1D\x2A\x03\x0E\x4E\x4F\x14\x51\x6B\x59\x56\x1F\x43\x03\x40\x36\x77\x28\x0A\x08\x29\x24\x44\x33\x0B\x29\x3D\x08\x11\x34\x44\x5D\x77", 35).c_str());
    jclass settingSecureClass = env->FindClass(/*android/provider/Settings$Secure*/ StrEnc("T1yw^BCF^af&dB_@Raf}\\FS,zT~L(3Z\"", "\x35\x5F\x1D\x05\x31\x2B\x27\x69\x2E\x13\x09\x50\x0D\x26\x3A\x32\x7D\x32\x03\x09\x28\x2F\x3D\x4B\x09\x70\x2D\x29\x4B\x46\x28\x47", 32).c_str());
    jmethodID getStringMethod = env->GetStaticMethodID(settingSecureClass, /*getString*/ StrEnc("e<F*J5c0Y", "\x02\x59\x32\x79\x3E\x47\x0A\x5E\x3E", 9).c_str(), /*(Landroid/content/ContentResolver;Ljava/lang/String;)Ljava/lang/String;*/ StrEnc("$6*%R*!XO\"m18o,0S!*`uI$IW)l_/_knSdlRiO1T`2sH|Ouy__^}%Y)JsQ:-\"(2_^-$i{?H", "\x0C\x7A\x4B\x4B\x36\x58\x4E\x31\x2B\x0D\x0E\x5E\x56\x1B\x49\x5E\x27\x0E\x69\x0F\x1B\x3D\x41\x27\x23\x7B\x09\x2C\x40\x33\x1D\x0B\x21\x5F\x20\x38\x08\x39\x50\x7B\x0C\x53\x1D\x2F\x53\x1C\x01\x0B\x36\x31\x39\x46\x0C\x15\x43\x2B\x05\x30\x15\x41\x43\x46\x55\x70\x0D\x59\x56\x00\x15\x58\x73", 71).c_str());

    auto obj = env->CallObjectMethod(context, getContentResolverMethod);
    auto str = (jstring)env->CallStaticObjectMethod(settingSecureClass, getStringMethod, obj, env->NewStringUTF(/*android_id*/ StrEnc("ujHO)8OfOE", "\x14\x04\x2C\x3D\x46\x51\x2B\x39\x26\x21", 10).c_str()));
    return env->GetStringUTFChars(str, 0);
}

const char* GetDeviceModel(JNIEnv* env) {
    jclass buildClass = env->FindClass(/*android/os/Build*/ StrEnc("m5I{GKGWBP-VOxkA", "\x0C\x5B\x2D\x09\x28\x22\x23\x78\x2D\x23\x02\x14\x3A\x11\x07\x25", 16).c_str());
    jfieldID modelId = env->GetStaticFieldID(buildClass, /*MODEL*/ StrEnc("|}[q:", "\x31\x32\x1F\x34\x76", 5).c_str(), /*Ljava/lang/String;*/ StrEnc(".D:C:ETZ1O-Ib&^h.Y", "\x62\x2E\x5B\x35\x5B\x6A\x38\x3B\x5F\x28\x02\x1A\x16\x54\x37\x06\x49\x62", 18).c_str());

    auto str = (jstring)env->GetStaticObjectField(buildClass, modelId);
    return env->GetStringUTFChars(str, 0);
}

const char* GetDeviceBrand(JNIEnv* env) {
    jclass buildClass = env->FindClass(/*android/os/Build*/ StrEnc("0iW=2^>0zTRB!B90", "\x51\x07\x33\x4F\x5D\x37\x5A\x1F\x15\x27\x7D\x00\x54\x2B\x55\x54", 16).c_str());
    jfieldID modelId = env->GetStaticFieldID(buildClass, /*BRAND*/ StrEnc("@{[FP", "\x02\x29\x1A\x08\x14", 5).c_str(), /*Ljava/lang/String;*/ StrEnc(".D:C:ETZ1O-Ib&^h.Y", "\x62\x2E\x5B\x35\x5B\x6A\x38\x3B\x5F\x28\x02\x1A\x16\x54\x37\x06\x49\x62", 18).c_str());

    auto str = (jstring)env->GetStaticObjectField(buildClass, modelId);
    return env->GetStringUTFChars(str, 0);
}

const char* GetPackageName(JNIEnv* env, jobject context) {
    jclass contextClass = env->FindClass(/*android/content/Context*/ StrEnc("`L+&0^[S+-:J^$,r9q92(as", "\x01\x22\x4F\x54\x5F\x37\x3F\x7C\x48\x42\x54\x3E\x3B\x4A\x58\x5D\x7A\x1E\x57\x46\x4D\x19\x07", 23).c_str());
    jmethodID getPackageNameId = env->GetMethodID(contextClass, /*getPackageName*/ StrEnc("YN4DaP)!{wRGN}", "\x3E\x2B\x40\x14\x00\x33\x42\x40\x1C\x12\x1C\x26\x23\x18", 14).c_str(), /*()Ljava/lang/String;*/ StrEnc("VnpibEspM(b]<s#[9cQD", "\x7E\x47\x3C\x03\x03\x33\x12\x5F\x21\x49\x0C\x3A\x13\x20\x57\x29\x50\x0D\x36\x7F", 20).c_str());

    auto str = (jstring)env->CallObjectMethod(context, getPackageNameId);
    return env->GetStringUTFChars(str, 0);
}

const char* GetDeviceUniqueIdentifier(JNIEnv* env, const char* uuid) {
    jclass uuidClass = env->FindClass(/*java/util/UUID*/ StrEnc("B/TxJ=3BZ_]SFx", "\x28\x4E\x22\x19\x65\x48\x47\x2B\x36\x70\x08\x06\x0F\x3C", 14).c_str());

    auto len = strlen(uuid);

    jbyteArray myJByteArray = env->NewByteArray(len);
    env->SetByteArrayRegion(myJByteArray, 0, len, (jbyte*)uuid);

    jmethodID nameUUIDFromBytesMethod = env->GetStaticMethodID(uuidClass, /*nameUUIDFromBytes*/ StrEnc("P6LV|'0#A+zQmoat,", "\x3E\x57\x21\x33\x29\x72\x79\x67\x07\x59\x15\x3C\x2F\x16\x15\x11\x5F", 17).c_str(), /*([B)Ljava/util/UUID;*/ StrEnc("sW[\"Q[W3,7@H.vT0) xB", "\x5B\x0C\x19\x0B\x1D\x31\x36\x45\x4D\x18\x35\x3C\x47\x1A\x7B\x65\x7C\x69\x3C\x79", 20).c_str());
    jmethodID toStringMethod = env->GetMethodID(uuidClass, /*toString*/ StrEnc("2~5292eW", "\x46\x11\x66\x46\x4B\x5B\x0B\x30", 8).c_str(), /*()Ljava/lang/String;*/ StrEnc("P$BMc' #j?<:myTh_*h0", "\x78\x0D\x0E\x27\x02\x51\x41\x0C\x06\x5E\x52\x5D\x42\x2A\x20\x1A\x36\x44\x0F\x0B", 20).c_str());

    auto obj = env->CallStaticObjectMethod(uuidClass, nameUUIDFromBytesMethod, myJByteArray);
    auto str = (jstring)env->CallObjectMethod(obj, toStringMethod);
    return env->GetStringUTFChars(str, 0);
}

struct MemoryStruct {
    char* memory;
    size_t size;
};

static size_t WriteMemoryCallback(void* contents, size_t size, size_t nmemb, void* userp) {
    size_t realsize = size * nmemb;
    struct MemoryStruct* mem = (struct MemoryStruct*)userp;

    mem->memory = (char*)realloc(mem->memory, mem->size + realsize + 1);
    if (mem->memory == NULL) {
        return 0;
    }

    memcpy(&(mem->memory[mem->size]), contents, realsize);
    mem->size += realsize;
    mem->memory[mem->size] = 0;

    return realsize;
}

//=========================MAIN LOGIN =================//
std::string Login(const char* user_key) {
    if (!g_App)
        return "Internal Error";

    auto activity = g_App->activity;
    if (!activity)
        return "Internal Error";

    auto vm = activity->vm;
    if (!vm)
        return "Internal Error";

    auto object = activity->clazz;
    if (!object)
        return "Internal Error";

    JNIEnv* env;
    vm->AttachCurrentThread(&env, 0);

    std::string hwid = user_key;
    hwid += GetAndroidID(env, object);
    hwid += GetDeviceModel(env);
    hwid += GetDeviceBrand(env);

    std::string UUID = GetDeviceUniqueIdentifier(env, hwid.c_str());

    vm->DetachCurrentThread();

    std::string errMsg;

    struct MemoryStruct chunk {};
    chunk.memory = (char*)malloc(1);
    chunk.size = 0;

    CURL* curl;
    CURLcode res;
    curl = curl_easy_init();


    // ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ ᴍᴀᴅᴇʙʏɴᴏᴄᴀꜱʜ ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ //

    if (curl) {
        curl_easy_setopt(curl, CURLOPT_CUSTOMREQUEST, /*POST*/ StrEnc(",IL=", "\x7C\x06\x1F\x69", 4).c_str());
        std::string api_key = OBFUSCATE("https://bantai.vipbombay.online/connect");
        curl_easy_setopt(curl, CURLOPT_URL, (api_key.c_str()));
        curl_easy_setopt(curl, CURLOPT_FOLLOWLOCATION, 1L);
        curl_easy_setopt(curl, CURLOPT_DEFAULT_PROTOCOL, /*https*/ StrEnc("!mLBO", "\x49\x19\x38\x32\x3C", 5).c_str());
        struct curl_slist* headers = NULL;
        headers = curl_slist_append(headers, /*Content-Type: application/x-www-form-urlencoded*/ StrEnc("@;Ls\\(KP4Qrop`b#d3094/r1cf<c<=H)AiiBG6i|Ta66s2[", "\x03\x54\x22\x07\x39\x46\x3F\x7D\x60\x28\x02\x0A\x4A\x40\x03\x53\x14\x5F\x59\x5A\x55\x5B\x1B\x5E\x0D\x49\x44\x4E\x4B\x4A\x3F\x04\x27\x06\x1B\x2F\x6A\x43\x1B\x10\x31\x0F\x55\x59\x17\x57\x3F", 47).c_str());
        curl_easy_setopt(curl, CURLOPT_HTTPHEADER, headers);
        char data[4096];
        sprintf(data, /*game=PUBG&user_key=%s&serial=%s*/ StrEnc("qu2yXK,YkJyGD@ut0.u~Nb'5(:.:chK", "\x16\x14\x5F\x1C\x65\x1B\x79\x1B\x2C\x6C\x0C\x34\x21\x32\x2A\x1F\x55\x57\x48\x5B\x3D\x44\x54\x50\x5A\x53\x4F\x56\x5E\x4D\x38", 31).c_str(), user_key, UUID.c_str());
        curl_easy_setopt(curl, CURLOPT_POSTFIELDS, data);
        curl_easy_setopt(curl, CURLOPT_WRITEFUNCTION, WriteMemoryCallback);
        curl_easy_setopt(curl, CURLOPT_WRITEDATA, (void*)&chunk);
        curl_easy_setopt(curl, CURLOPT_SSL_VERIFYPEER, 0L);
        curl_easy_setopt(curl, CURLOPT_SSL_VERIFYHOST, 0L);

        res = curl_easy_perform(curl);
        if (res == CURLE_OK) {
            try {
                json result = json::parse(chunk.memory);
                if (result[/*status*/ StrEnc("(>_LBm", "\x5B\x4A\x3E\x38\x37\x1E", 6).c_str()] == true) {
                    std::string token = result[/*data*/ StrEnc("fAVA", "\x02\x20\x22\x20", 4).c_str()][/*token*/ StrEnc("{>3Lr", "\x0F\x51\x58\x29\x1C", 5).c_str()].get<std::string>();
                    time_t rng = result[/*data*/ StrEnc("fAVA", "\x02\x20\x22\x20", 4).c_str()][/*rng*/ StrEnc("+n,", "\x59\x00\x4B", 3).c_str()].get<time_t>();
                    //   expiredDate = result[/*data*/ StrEnc("fAVA", "\x02\x20\x22\x20", 4).c_str()][/*ts*/ StrEnc("4`", "\x40\x13", 2).c_str()].get<std::string>();
                    //  modStatus = result[/*data*/ StrEnc("fAVA", "\x02\x20\x22\x20", 4).c_str()][/*ms*/ StrEnc("#e", "\x4E\x16", 2).c_str()].get<std::string>();
                    if (rng + 30 > time(0)) {
                        std::string auth = /*PUBG*/ StrEnc("Q*) ", "\x01\x7F\x6B\x67", 4).c_str();;
                        auth += "-";
                        auth += user_key;
                        auth += "-";
                        auth += UUID;
                        auth += "-";
                        auth += /*Vm8Lk7Uj2JmsjCPVPVjrLa7zgfx3uz9E*/ StrEnc("ZD$_K NtaM8Fu=n0fFyO;!Ae<H)*Gy4%", "\x0C\x29\x1C\x13\x20\x17\x1B\x1E\x53\x07\x55\x35\x1F\x7E\x3E\x66\x36\x10\x13\x3D\x77\x40\x76\x1F\x5B\x2E\x51\x19\x32\x03\x0D\x60", 32).c_str();
                        std::string outputAuth = Tools::CalcMD5(auth);
                        g_Token = token;
                        g_Auth = outputAuth;

                        bValid = g_Token == g_Auth;
                    }
                }
                else {
                    errMsg = result[/*reason*/ StrEnc("LW(3(c", "\x3E\x32\x49\x40\x47\x0D", 6).c_str()].get<std::string>();
                }
            }
            catch (json::exception& e) {
                errMsg = "{";
                errMsg += e.what();
                errMsg += "}\n{";
                errMsg += chunk.memory;
                errMsg += "}";
            }
        }
        else {
            errMsg = curl_easy_strerror(res);
        }
    }
    curl_easy_cleanup(curl);
    vm->DetachCurrentThread();

    return bValid ? "OK" : errMsg;
}


// ======================================================================== //
// sConfig.SilentAim.VisCheck = true;
// ======================================================================== //

#define IM_CLAMP(V, MN, MX)     ((V) < (MN) ? (MN) : (V) > (MX) ? (MX) : (V))
namespace Settings
{
    static int Tab = 1;
}

// ======================================================================== //


//void loadConfig()
//{
//    int fd = open("/data/data/com.tencent.ig/files/never.ini", O_RDONLY);
//    
//        read(fd, &Config.PlayerESP , sizeof(Config.PlayerESP));
//    read(fd, &Config.SilentAim , sizeof(Config.SilentAim));
//    
//    read(fd, &Config.PlayerESP , sizeof(Config.PlayerESP));
//        
//        close(fd);
//    
//}
//void DeleteConfig()
//{
//
//    int fd = remove("/data/data/com.tencent.ig/files/never.ini");
//    close(fd);
//}
//
//void saveConfig()
//{
//    
//    int fd = open("/data/data/com.tencent.ig/files/never.ini", O_WRONLY | O_CREAT);
//    system("chmod 777 /data/data/com.tencent.ig/files/never.ini");
//    write(fd, &Config.PlayerESP , sizeof(Config.PlayerESP));
//    write(fd, &Config.SilentAim , sizeof(Config.SilentAim));
//    
//    write(fd, &Config.PlayerESP , sizeof(Config.PlayerESP));
//    write(fd, &Config.ColorsESP , sizeof(Config.ColorsESP));
//
//    close(fd);
//}

EGLBoolean(*orig_eglSwapBuffers) (EGLDisplay dpy, EGLSurface surface);
EGLBoolean _eglSwapBuffers(EGLDisplay dpy, EGLSurface surface) {
    eglQuerySurface(dpy, surface, EGL_WIDTH, &glWidth);
    eglQuerySurface(dpy, surface, EGL_HEIGHT, &glHeight);
    if (glWidth <= 0b0 || glHeight <= 0b0) {
        return orig_eglSwapBuffers(dpy, surface);
    }
    if (!g_App) {
        return orig_eglSwapBuffers(dpy, surface);
    }
    screenWidth = ANativeWindow_getWidth(g_App->window);
    screenHeight = ANativeWindow_getHeight(g_App->window);
    density = AConfiguration_getDensity(g_App->config);

    // ======================================================================== //

    if (!initImGui) {
        ImGui::CreateContext();
        ImGuiIO& io = ImGui::GetIO(); (void)io;
        ImGuiStyle* style = &ImGui::GetStyle();
        //  LoadImage();//add


        style->WindowRounding = 0;
        style->FrameRounding = 0;
        style->ScrollbarRounding = 0.2f;
        style->ScrollbarSize = 13;
        style->ScrollbarRounding = 10;
        style->PopupRounding = 10;
        style->GrabRounding = 10;
        style->ChildBorderSize = 7.6f;

        style->FramePadding = ImVec2(4, 4);
        style->FrameBorderSize = 3.2f;
        style->WindowTitleAlign = ImVec2(0.5, 0.5);
        style->ScaleAllSizes(std::max(2.0f, density / 400.0f));
        style->ScrollbarSize /= 1;

        ImGui_ImplAndroid_Init();
        ImGui_ImplOpenGL3_Init();

        io.ConfigWindowsMoveFromTitleBarOnly = true;
        io.IniFilename = NULL;

        ImVec4* colors = ImGui::GetStyle().Colors;
        // Diğer renk tanımlamaları
        colors[ImGuiCol_Text] = ImVec4(1.0f, 1.0f, 1.0f, 1.0f);  // Normal metin rengi - Beyaz
        colors[ImGuiCol_TextDisabled] = ImVec4(1.0f, 1.0f, 1.0f, 1.0f); // Devre dışı metin rengi - Beyaz
        colors[ImGuiCol_WindowBg] = ImVec4(0.0f, 0.0f, 0.0f, 1.0f);  // Pencere arka plan rengi - Siyah
        colors[ImGuiCol_ChildBg] = ImVec4(0.17f, 0.18f, 0.20f, 1.00f);  // Çocuk pencere arka plan rengi - Çok koyu gri
        colors[ImGuiCol_PopupBg] = ImVec4(0.22f, 0.24f, 0.25f, 1.00f);  // Açılır pencere arka plan rengi - Koyu gri
        colors[ImGuiCol_Border] = ImVec4(0.16f, 0.17f, 0.18f, 1.00f);  // Kenarlık rengi - Çok koyu gri
        colors[ImGuiCol_BorderShadow] = ImVec4(0.16f, 0.17f, 0.18f, 1.00f);  // Kenarlık gölge rengi - Çok koyu gri
        colors[ImGuiCol_FrameBg] = ImVec4(0.14f, 0.15f, 0.16f, 1.00f);  // Çerçeve arka plan rengi - Koyu gri
        colors[ImGuiCol_FrameBgHovered] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f);  // Çerçeve üzerine gelindiğinde renk - Yeşil
        colors[ImGuiCol_FrameBgActive] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f);  // Çerçeve aktif durumda renk - Yeşil
        colors[ImGuiCol_TitleBg] = ImVec4(0.0f, 0.0f, 0.0f, 1.0f);  // Başlık arka plan rengi - Siyah
        colors[ImGuiCol_TitleBgActive] = ImVec4(0.0f, 0.0f, 0.0f, 1.0f);  // Aktif başlık arka plan rengi - Siyah
        colors[ImGuiCol_TitleBgCollapsed] = ImVec4(0.13f, 0.14f, 0.16f, 0.5f);  // Küçültülmüş başlık arka plan rengi - Koyu gri (şeffaf)
        colors[ImGuiCol_MenuBarBg] = ImVec4(0.13f, 0.14f, 0.16f, 1.00f);  // Menü çubuğu arka plan rengi - Koyu gri
        colors[ImGuiCol_ScrollbarBg] = ImVec4(0.13f, 0.14f, 0.16f, 1.00f);  // Kaydırıcı arka plan rengi - Koyu gri
        colors[ImGuiCol_ScrollbarGrab] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f);  // Kaydırıcı tutamaç rengi - Gri - yeşil oldu
        colors[ImGuiCol_ScrollbarGrabHovered] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f);  // Kaydırıcı tutamaç üzerine gelindiğinde renk - Yeşil
        colors[ImGuiCol_ScrollbarGrabActive] = ImVec4(0.51f, 0.51f, 0.51f, 1.00f);  // Kaydırıcı tutamaç aktif durumda renk - Gri
        colors[ImGuiCol_CheckMark] = ImVec4(0.90f, 0.90f, 0.90f, 0.50f);  // Onay işareti rengi - Çok açık gri (şeffaf)
        colors[ImGuiCol_SliderGrab] = ImVec4(1.00f, 1.00f, 1.00f, 0.30f);  // Kaydırıcı tutamaç rengi (aktif değilken) - Beyaz (şeffaf)
        colors[ImGuiCol_SliderGrabActive] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f); // Kaydırıcı tutamaç aktif durumda renk - Gri
        colors[ImGuiCol_Button] = ImVec4(0.19f, 0.20f, 0.22f, 1.00f); // Buton normal rengi - Çok koyu gri
        colors[ImGuiCol_ButtonHovered] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f); // Buton üzerine gelindiğinde renk - yeşil
        colors[ImGuiCol_ButtonActive] = ImVec4(0.0f, 1.0f, 0.0f, 1.00f); // Buton aktif durumda renk - Yeşil
        colors[ImGuiCol_Header] = ImVec4(0.22f, 0.23f, 0.25f, 1.00f);  // Başlık arka plan rengi - Koyu gri
        colors[ImGuiCol_HeaderHovered] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f);  // Başlık üzerine gelindiğinde renk - yeşil
        colors[ImGuiCol_HeaderActive] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f);  // Başlık aktif durumda  - Yeşil
        colors[ImGuiCol_Separator] = ImVec4(0.17f, 0.18f, 0.20f, 1.00f);  // Ayırıcı rengi - Çok koyu gri
        colors[ImGuiCol_SeparatorHovered] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f);  // Ayırıcı üzerine gelindiğinde renk - Yeşil
        colors[ImGuiCol_SeparatorActive] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f);  // Ayırıcı aktif durumda renk - Yeşil
        colors[ImGuiCol_ResizeGrip] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f);  // Yeniden boyutlandırma tutamaç rengi (aktif değilken) - Yeşil
        colors[ImGuiCol_ResizeGripHovered] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f);  // Yeniden boyutlandırma tutamaç üzerine gelindiğinde renk - Yeşil
        colors[ImGuiCol_ResizeGripActive] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f);  // Yeniden boyutlandırma tutamaç aktif durumda renk - Yeşil
        colors[ImGuiCol_Tab] = ImVec4(0.16f, 0.16f, 0.16f, 1.00f);  // Sekme arka plan rengi - Koyu gri
        colors[ImGuiCol_TabHovered] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f);  // Sekme üzerine gelindiğinde renk - Yeşil
        colors[ImGuiCol_TabActive] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f);  // Sekme aktif durumda renk - Yeşil
        colors[ImGuiCol_TabUnfocused] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f); // Sekme odaklanmamış durumda renk - Koyu gri - Yeşil oldu
        colors[ImGuiCol_TabUnfocusedActive] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f); // Sekme odaklanmamış aktif durumda renk - Yeşil

        colors[ImGuiCol_PlotLines] = ImVec4(1.00f, 1.00f, 1.00f, 1.00f); // Grafik çizgileri rengi - Beyaz
        colors[ImGuiCol_PlotLinesHovered] = ImVec4(0.90f, 0.70f, 0.00f, 1.00f); // Grafik çizgileri üzerine gelindiğinde renk - Sarı
        colors[ImGuiCol_PlotHistogram] = ImVec4(0.90f, 0.70f, 0.00f, 1.00f); // Grafik histogramı rengi - Sarı
        colors[ImGuiCol_PlotHistogramHovered] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f); // Grafik histogramı üzerine gelindiğinde renk - Yeşil
        colors[ImGuiCol_TextSelectedBg] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f); // Seçili metin arka plan rengi - Yeşil
        colors[ImGuiCol_DragDropTarget] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f); // Sürükle ve bırak hedefi rengi - Yeşil
        colors[ImGuiCol_NavHighlight] = ImVec4(0.0f, 1.0f, 0.0f, 1.0f); // Navigasyon vurgulama rengi - Yeşil
        colors[ImGuiCol_NavWindowingHighlight] = ImVec4(1.00f, 1.00f, 1.00f, 0.70f); // Navigasyon penceresi vurgulama rengi - Beyaz (şeffaf)
        colors[ImGuiCol_NavWindowingDimBg] = ImVec4(0.80f, 0.80f, 0.80f, 0.20f); // Navigasyon penceresi karartma arka plan rengi - Açık gri (şeffaf)
        colors[ImGuiCol_ModalWindowDimBg] = ImVec4(0.20f, 0.20f, 0.20f, 0.35f); // Modal pencere karartma arka plan rengi - Koyu gri (şeffaf)



        //ImGui::StyleColorsDark();

        ImFontConfig font_config;
        font_config.OversampleH = 1;
        font_config.OversampleV = 1;
        font_config.FontBuilderFlags = 1;
        static const ImWchar ranges[] =
        {
            0x0020, 0x00FF, // Basic Latin + Latin Supplement
            0x0400, 0x052F, // Cyrillic + Cyrillic Supplement
            0x2DE0, 0x2DFF, // Cyrillic Extended-A
            0xA640, 0xA69F, // Cyrillic Extended-B
            0xE000, 0xE226, // icons
            0,
        };
        static const ImWchar icons_ranges[] = { 0xf000, 0xf3ff, 0 };
        ImFontConfig icons_config;
        ImFontConfig CustomFont;
        CustomFont.FontDataOwnedByAtlas = false;
        icons_config.MergeMode = true;
        icons_config.PixelSnapH = true;
        icons_config.OversampleH = 2.5;
        icons_config.OversampleV = 2.5;
        font_config.GlyphRanges = ranges;
        // ======================================================================== //		
        basic = io.Fonts->AddFontFromMemoryTTF((void*)Customm, sizeof(Customm), 23.f, &CustomFont);
        io.Fonts->AddFontFromMemoryTTF(&bold_segue, sizeof bold_segue, 22, NULL, io.Fonts->GetGlyphRangesCyrillic());
        default_segu = io.Fonts->AddFontFromMemoryTTF(&bold_segue, sizeof bold_segue, 22, NULL, io.Fonts->GetGlyphRangesCyrillic());
        segu = io.Fonts->AddFontFromMemoryTTF(&bold_segue, sizeof bold_segue, 40, NULL, io.Fonts->GetGlyphRangesCyrillic());
        bold_segu = io.Fonts->AddFontFromMemoryTTF(&bold_segue, sizeof bold_segue, 40, NULL, io.Fonts->GetGlyphRangesCyrillic());
        ico = io.Fonts->AddFontFromMemoryTTF(&icon, sizeof icon, 24, NULL, io.Fonts->GetGlyphRangesCyrillic());
        ico_combo = io.Fonts->AddFontFromMemoryTTF(&icon, sizeof icon, 19, NULL, io.Fonts->GetGlyphRangesCyrillic());
        ico_button = io.Fonts->AddFontFromMemoryTTF(&icon, sizeof icon, 25, NULL, io.Fonts->GetGlyphRangesCyrillic());
        ico_grande = io.Fonts->AddFontFromMemoryTTF(&icon, sizeof icon, 40, NULL, io.Fonts->GetGlyphRangesCyrillic());
        logoicon = io.Fonts->AddFontFromMemoryTTF(Loginc, sizeof(Loginc), 20.0f, &font_config, ranges);
        logoicon2 = io.Fonts->AddFontFromMemoryTTF(Loginc, sizeof(Loginc), 40.0f, &font_config, ranges);
        bold = io.Fonts->AddFontFromMemoryTTF((void*)Custom1, sizeof(Custom1), 55.0f, &CustomFont);
        bankai = io.Fonts->AddFontFromMemoryTTF((void*)Custom3, sizeof(Custom3), 22.2, &CustomFont);
        ico_default = io.Fonts->AddFontFromMemoryTTF(&my_font_icon, sizeof my_font_icon, 26, NULL, io.Fonts->GetGlyphRangesCyrillic());
        //Snowflake::CreateSnowFlakes(Snow, SNOW_LIMIT, 5.f/*minimum size*/, 25.f/*maximum size*/, 0/*imgui window x position*/, 0/*imgui window y position*/, glWidth, glHeight, Snowflake::vec3(0.f, 0.005f)/*gravity*/, IM_COL32(99, 124, 146, 50)/*color*/);
        flamee = io.Fonts->AddFontFromMemoryTTF((void*)_data, _size, 35.0f, &font_config, io.Fonts->GetGlyphRangesCyrillic());


        // ======================================================================== //   

        ImFontConfig cfg;
        cfg.SizePixels = ((float)density / 70.0f);
        io.Fonts->AddFontDefault(&cfg);
        memset(&Config, 0, sizeof(sConfig));

        // ===============================ESPCOLOR ================================== //

        Config.B_non = CREATE_COLOR(255, 255, 255, 255);  // Beyaz
        Config.B_vis = CREATE_COLOR(255, 255, 0, 255);    // Sarı
        Config.P_non = CREATE_COLOR(255, 255, 255, 255);  // Beyaz
        Config.P_vis = CREATE_COLOR(255, 0, 255, 255);    // Pembe
        Config.VehicleColor = CREATE_COLOR(255, 255, 255, 255); // Beyaz
        Config.VehicleS = CREATE_COLOR(0, 255, 0, 255);    // Yeşil
        Config.Fov = CREATE_COLOR(139, 0, 0, 255);     // Koyu Kırmızı
        Config.ColorsESP.Line = CREATE_COLOR(255, 0, 0, 255); // Kırmızı
        Config.ColorsESP.Box = CREATE_COLOR(255, 0, 0, 255);  // Kırmızı
        Config.ColorsESP.Name = CREATE_COLOR(255, 255, 255, 255); // Beyaz
        Config.ColorsESP.Skeleton = CREATE_COLOR(255, 255, 255, 255); // Beyaz
        Config.ColorsESP.Vehicle = CREATE_COLOR(255, 255, 255, 255); // Beyaz
        Config.ColorsESP.SkeletonVisible = CREATE_COLOR(0, 255, 0, 255); // Yeşil
        Config.ColorsESP.Fov = CREATE_COLOR(255, 0, 0, 255); // Kırmızı

        // ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ //
        initImGui = true;
        items_data = json::parse(JSON_ITEMS);

        for (auto& i : items_data)
        {
            for (auto& item : i["Items"])
            {
                // Kırmızı rengi sabit olarak belirliyoruz
                int r = 255;
                int g = 0;
                int b = 0;

                // Sabit kırmızı rengi kullanarak renk oluşturuyoruz
                ItemColors[item["itemId"].get<int>()] = CREATE_COLOR(r, g, b, 255);

            }
        }
        initImGui = true;
        Config.Logo = true;
        Config.PlayerESP.Distance = 100;
        //loadConfig();

    }

    ImGuiIO& io = ImGui::GetIO();
    ImGui_ImplOpenGL3_NewFrame();
    ImGui_ImplAndroid_NewFrame(glWidth, glHeight);
    ImGui::NewFrame();
    DrawESP(ImGui::GetBackgroundDrawList());


    static bool show = false;
    static bool ava;
    // ImGui::SetNextWindowSize(ImVec2((float)glWidth * 0.38f, (float)glHeight * 0.53f), ImGuiCond_Once);
    //     ImVec2 center = ImGui::GetMainViewport()->GetCenter();
      //   ImGui::SetNextWindowPos(center, ImGuiCond_Appearing, ImVec2(0.5f, 0.5f)); //0.5 0.5
    ImGui::SetNextWindowSize(ImVec2((float)glWidth * 0.40f, (float)glHeight * 0.65f), ImGuiCond_Once); // 45% width 70% height
    //ImGui::SetNextWindowSize( ImVec2(870, 625) );
   // Config.PlayerESP.Skeleton = true;
   // Config.PlayerESP.Name = true;
    Config.SilentAim.VisCheck = true;
    // Config.PlayerESP.Health = true;
    // Config.PlayerESP.Box = true;
    if (ShowMenu)
    {



        //config</>//
        if (ShowMenu)
        {

            if (ImGui::Begin(OBFUSCATE(" ALFA HUB [ PUBG MOBILE 3.3 ] "), 0, ImGuiWindowFlags_NoBringToFrontOnFocus))
            {


                static bool isLogin = true;

                if (!isLogin) {
                    ImGui::Text("Please Login! (Copy Key to Clipboard)");

                    ImGui::PushItemWidth(-1);
                    static char s[64];
                    ImGui::InputText("##key", s, sizeof s);
                    ImGui::PopItemWidth();

                    if (ImGui::Button("Paste Key", ImVec2(ImGui::GetContentRegionAvailWidth(), 0))) {
                        auto key = getClipboardText();
                        strncpy(s, key.c_str(), sizeof s);
                    }

                    static std::string err;
                    if (ImGui::Button("Login", ImVec2(ImGui::GetContentRegionAvailWidth(), 0))) {
                        err = Login(s);
                        if (err == "OK") {
                            isLogin = bValid && g_Auth == g_Token;
                        }
                    }

                    if (!err.empty() && err != "OK") {
                        ImGui::Text("Error: %s", err.c_str());
                    }

                }
                else {


                    ImGui::Columns(2);
                    ImGui::SetColumnOffset(1, 140); //270
                    {
                        if (ImGui::Button(" AIMBOT ", ImVec2(115, 45)))
                            Settings::Tab = 1;

                        if (ImGui::Button(" ESP ", ImVec2(115, 45))) //230
                            Settings::Tab = 2;

                        if (ImGui::Button(" ITEMS", ImVec2(115, 45)))
                            Settings::Tab = 3;

                        if (ImGui::Button(" IPAD VIEW", ImVec2(115, 45)))
                            Settings::Tab = 4;
                        //deleted memory in there

                    }
                    ImGui::NextColumn();


                    if (Settings::Tab == 2) {
                        if (ImGui::BeginTable("split", 2));
                        {
                            ImGui::TableNextColumn();

                            ImGui::Checkbox("Line", &Config.Line);
                            ImGui::TableNextColumn();

                            //ImGui::Checkbox("Box", &Config.PlayerESP.Box);
                            //ImGui::TableNextColumn();

                            ImGui::Checkbox("Health", &Config.PlayerESP.Health);
                            ImGui::TableNextColumn();

                            ImGui::Checkbox("Name", &Config.PlayerESP.Name);
                            ImGui::TableNextColumn();

                            ImGui::Checkbox("Skeleton", &Config.PlayerESP.Skeleton);
                            ImGui::TableNextColumn();

                            ImGui::Checkbox("Distance", &Config.PlayerESP.Distance);
                            ImGui::TableNextColumn();

                            //ImGui::Checkbox("TeamID", &Config.PlayerESP.TeamID);
                            //ImGui::TableNextColumn();

                            //ImGui::Checkbox("360 Alert", &Config.Alert360);
                            //ImGui::TableNextColumn();

                            //ImGui::Checkbox("Grenade Alert", &Config.Grenade);
                            //ImGui::TableNextColumn();

                            ImGui::Checkbox("Enable Vehicle", &Config.Vehicle);
                            ImGui::TableNextColumn();

                            //ImGui::Checkbox("Dead Box", &Config.PlayerESP.LootBox);
                            //ImGui::TableNextColumn();

                            //ImGui::Checkbox("Player Weapen", &Config.P_Weapon);
                            //ImGui::TableNextColumn();
                            
                            ImGui::Text("- Buy : WWW.GAMEPROHACK.COM");
                            ImGui::TableNextColumn();
                        }
                        ImGui::EndTable();

                    }
                    else if (Settings::Tab == 1) {
                        ImGui::TableNextColumn();
                        ImGui::TextColored(ImVec4(123.0f / 255.0f, 104.0f / 255.0f, 238.0f / 255.0f, 1.0f), "");
                        ImGui::Checkbox("Enable Aim", &Config.AimBot.Enable); //SilentAim
                        ImGui::Checkbox("Ignore Bots", &Config.SilentAim.IgnoreBots);
                        ImGui::Checkbox("Ignore Knocks", &Config.SilentAim.IgnoreKnocked);
                        ImGui::SliderInt("Aim Metre", &Config.Maters, 0.000f, 175.000f);
                        ImGui::SliderInt("Fov Cross", &Config.SilentAim.Cross, 0.000f, 150.000f);
						
                        ImGui::TextColored(ImVec4(1.0f, 1.0f, 1.0f, 1.0f), "- Developed - Game Pro Team");


                    }

                    else if (Settings::Tab == 4) {
                        ImGui::TableNextColumn();
                        ImGui::TextColored(ImVec4(123.0f / 255.0f, 104.0f / 255.0f, 238.0f / 255.0f, 1.0f), "");
                     
                        ImGui::Checkbox("Ipad View:", &Config.PlayerESP.wide_view);
                        ImGui::SliderFloat("", &Config.PlayerESP.set_field_of_view, 70.0f, 95.0f);
                        ImGui::TableNextColumn();
                        ImGui::TextColored(ImVec4(1.0f, 1.0f, 1.0f, 1.0f), "- Developed - Game Pro Team");


                    }

                    else if (Settings::Tab == 3) {

                        ImGui::TableNextColumn();
                        for (auto& i : items_data)
                        {
                            if (ImGui::TreeNode(i["Category"].get<std::string>().c_str()))
                            {
                                for (auto& item : i["Items"])
                                {
                                    ImGui::Checkbox(item["itemName"].get<std::string>().c_str(), (bool*)&Items[item["itemId"].get<int>()]);
                                    ImGui::SameLine(ImGui::GetWindowContentRegionMax().x - 20);
                                    ImGui::SetNextWindowSize(ImVec2((float)glWidth * 0.25f, (float)glHeight * 0.25f), ImGuiCond_Once);
                                    ImGui::ColorEdit3(item["itemName"].get<std::string>().c_str(), ItemColors[item["itemId"].get<int>()], ImGuiColorEditFlags_NoLabel | ImGuiColorEditFlags_NoInputs);
                                }
                                ImGui::TreePop();
                            }
                        }
                    }

                }


            }
        }
    }

    ImGui::End();
    ImGui::Render();

    ImGui_ImplOpenGL3_RenderDrawData(ImGui::GetDrawData());

    return orig_eglSwapBuffers(dpy, surface);
}
int32_t(*orig_onInputEvent)(struct android_app* app, AInputEvent* inputEvent);

int32_t onInputEvent(struct android_app* app, AInputEvent* inputEvent) {
    if (initImGui) {
        ImGui_ImplAndroid_HandleInputEvent(inputEvent, { (float)screenWidth / (float)glWidth, (float)screenHeight / (float)glHeight });
    }
    return orig_onInputEvent(app, inputEvent);
}

[[noreturn]] void* skins22_thread(void*) {


    uint32_t  EmuBp = *(uint32_t*)(0x56e30000 + 0x904F3AC);
    uint32_t  EmuBp22 = *(uint32_t*)(0x56e30000 + 0x904F3A8);


    while (true) {



        if (deadbox1)

            if (g_LocalPlayer)
            {
                if (g_LocalPlayer->WeaponManagerComponent)
                {

                    auto WeaponComp = g_LocalPlayer->WeaponManagerComponent->GetAllInventoryWeaponList(true);
                    for (int i = 0; i < WeaponComp.Num(); i++)
                    {
                        auto syncWep = WeaponComp[i]->synData;
                        for (int i = 0; i < syncWep.Num(); i++)
                        {
                            int wepID = syncWep[i].DefineID.TypeSpecificID;
                            if (wepID == 101004)
                            {
                                if (skinm4 == 1)

                                    syncWep[i].DefineID.TypeSpecificID = 1101004046; //Glacier - M416 
                                if (skinm4 == 2)
                                    syncWep[i].DefineID.TypeSpecificID = 1101004062; //Glacier - M416 
                                if (skinm4 == 3)
                                    syncWep[i].DefineID.TypeSpecificID = 1101004086; //Glacier - M416 
                                if (skinm4 == 4)
                                    syncWep[i].DefineID.TypeSpecificID = 1101004078; //Glacier - M416 
                                if (skinm4 == 5)
                                    syncWep[i].DefineID.TypeSpecificID = 1101004098; //Glacier - M416 
                                if (skinm4 == 9)
                                    syncWep[i].DefineID.TypeSpecificID = 1101004218; //Glacier - M416 
                                if (skinm4 == 6)
                                    syncWep[i].DefineID.TypeSpecificID = 1101004163; //Glacier - M416 
                                if (skinm4 == 7)
                                    syncWep[i].DefineID.TypeSpecificID = 1101004201; //Glacier - M416 
                                if (skinm4 == 8)
                                    syncWep[i].DefineID.TypeSpecificID = 1101004138; //Glacier - M416 
                                if (skinm4 == 10)
                                    syncWep[i].DefineID.TypeSpecificID = 1101004209; //Glacier - M416 
                            }
                            else if (wepID == 101001)
                            {
                                if (skinakm == 1)
                                    syncWep[i].DefineID.TypeSpecificID = 1101001037; //Sculpture - AKM
                                if (skinakm == 2)
                                    syncWep[i].DefineID.TypeSpecificID = 1101001057; //The Seven Seas - AKM
                                if (skinakm == 3)
                                    syncWep[i].DefineID.TypeSpecificID = 1101001065; //Roaring Tiger - AKM
                                if (skinakm == 4)
                                    syncWep[i].DefineID.TypeSpecificID = 1101001089; //Glacier - AKM
                                if (skinakm == 5)
                                    syncWep[i].DefineID.TypeSpecificID = 1101001103; //Desert Fossil - AKM
                                if (skinakm == 6)
                                    syncWep[i].DefineID.TypeSpecificID = 1101001116; //Jack-o'-lantern - AKM
                                if (skinakm == 7)
                                    syncWep[i].DefineID.TypeSpecificID = 1101001128; //Ghillie Dragon - AKM 
                                if (skinakm == 8)
                                    syncWep[i].DefineID.TypeSpecificID = 1101001143; //Gold Pirate - AKM
                                if (skinakm == 9)
                                    syncWep[i].DefineID.TypeSpecificID = 1101001174; //Wandering Tyrant - AKM
                                if (skinakm == 10)
                                    syncWep[i].DefineID.TypeSpecificID = 1101001213; //Star Admiral - AKM
                                if (skinakm == 11)
                                    syncWep[i].DefineID.TypeSpecificID = 1101001023; //Hellfire - AKM
                            }
                        }
                    }
                }
            }

    }




}


#define SLEEP_TIME 1000LL / 60LL


void* maps_thread(void*) {
    while (true) {
        auto t1 = std::chrono::duration_cast<std::chrono::milliseconds>(std::chrono::system_clock::now().time_since_epoch()).count();

        std::vector<MemTrap_t> tmp;

        FILE* f = fopen("/proc/self/maps", "r");
        if (f) {
            char line[512];
            while (fgets(line, sizeof line, f)) {
                uintptr_t tmpBase, tmpEnd;
                char tmpProt[8];
                if (sscanf(line, "%" PRIXPTR "-%" PRIXPTR " %s %*s %*s %*s %*s", &tmpBase, &tmpEnd, tmpProt) > 0) {
                    if (tmpProt[0] != 'r') {
                        MemTrap_t mt = MemTrap_t();
                        mt.baseAddr = tmpBase;
                        mt.endAddr = tmpEnd;
                        tmp.push_back(mt);
                    }
                }
            }

            fclose(f);
        }

        MemTraps = tmp;

        auto td = std::chrono::duration_cast<std::chrono::milliseconds>(std::chrono::system_clock::now().time_since_epoch()).count() - t1;
        std::this_thread::sleep_for(std::chrono::milliseconds(std::max(std::min(0LL, SLEEP_TIME - td), SLEEP_TIME)));
    }
    return 0;
}


int (*osub_8E5F6)(int a1, unsigned char* a2, size_t a3);
int __fastcall hsub_8E5F6(int a1, unsigned char* a2, size_t a3)
{
    unsigned int v7; // r0
    while (true)
    {
        if (a2 && !((a3 - 1) >> 10))
        {
            if ((unsigned int)((*(unsigned int*)(a1 + 4) - *(unsigned int*)a1) >> 2) > 0x400)

                return 0;
            LOGI("Case 35 Blocked");
            v7 = *a2;

            if (v7 >= 0x11)
            {
                return 0;
                LOGI("Case 35 0x11 Blocked");
            }
        }
    }
    return osub_8E5F6(a1, a2, a3);
}
int (*osub_B2D56)(int a1, unsigned char* a2, size_t a3);
int __fastcall hsub_B2D56(int a1, unsigned char* a2, size_t a3)
{
    //102 lobby & match
    LOGI(OBFUSCATE("Case 35: |a1: %lld |a2: %p |a3: %zx"), a1, a2, a3);
    if (a3 == 30)
    {
        return osub_B2D56(a1, a2, 0);
    }
    if (a3 == 58)
    {
        return osub_B2D56(a1, a2, 0);
    }
    if (a3 == 39) //2month fix
    {
        return osub_B2D56(a1, a2, 0);
    }
    else
    {
        return osub_B2D56(a1, a2, a3);
    }
    return osub_B2D56(a1, a2, a3);

}


char* (*oAnoSDKIoctl_0)(int a1, int a2);
char* __fastcall hAnoSDKIoctl_0(int a1, int a2)
{
    LOGI("AnoSDKIoctl_0 Calls %d", a1);
    switch (a1)
    {
    case 23:
        return oAnoSDKIoctl_0(0, a2);
        break;
    }
    return oAnoSDKIoctl_0(a1, a2);
}

std::vector<uintptr_t> retList;
DWORD libanogsBase = 0;
DWORD libUE4Base = 0;
DWORD libanortBase = 0;
DWORD libEGLBase = 0;
DWORD libanogsAlloc = 0;
DWORD libUE4Alloc = 0;
DWORD libEGLAlloc = 0;
DWORD libanogsSize = 0x3DFF44;
DWORD libUE4Size = 0x7E55520;
DWORD libEGLSize = 0x2000;
DWORD NewBase = 0;

int __fastcall (*Osub_GuestLink)(int a1);
int __fastcall sub_GuestLink(int a1) {
    if (a1) {
        const char* Search = (const char*)(*(int(__fastcall*)(int, int, _DWORD))(g_UE4 + 0x6A881A0))(a1, 1, 0);

        if (strstr(Search, OBFUSCATE("GuestBindHandler")) || strstr(Search, OBFUSCATE("Client.Ban")) || strstr(Search, "client.network.Protocol.BattleReportHandler")) {
            LOGE("%s", Search);
            return false;
        }

    }
    return Osub_GuestLink(a1);
}

int sub_22B6BB4()
{

}
//====Venix===3.0===IMPORTANT===OFFSET====64BIT===ll		 
void* hook_dlopen2(const char* file, int mode)
{

    if (strstr(file, OBFUSCATE("dlopen")) || strstr(file, OBFUSCATE("libEGL.so")) || strstr(file, "libm.so") || strstr(file, "libgcloud.so") || strstr(file, "libTDataMaster.so") || strstr(file, "libgnustl_shared.so") || strstr(file, "libCrashSight.so") || strstr(file, "lib"))
    {
        return (void*)hook_dlopen2("BASETHREAD", mode);
    }
    if (file) {
        LOGI("FILE {%s}", file);
    }
    return dlopen(file, mode);
}



void* hook_dlopen(void* a1, const void* a2, size_t a3)
{
    if (a3 == 0x58u || a3 == 0x44u) {
        LOGI("%p", a3);
        return (void*)hook_dlopen(0, 0, 0);
        // memcpy(a1, a2, 0);
    }
    return memcpy(a1, a2, a3);
}

int* __fastcall (*osub_27D814)(int* result, unsigned int a2);
int* __fastcall hsub_27D814(int* result, unsigned int a2) {

    if (a2 == 6)
    {
        return 0;
    }
    if (a2 == 4)
    {
        return 0;
    }
    LOGI("RPDATA -> a2 : 0x%x", a2);

    return osub_27D814(result, a2);//redirect to original function
}
int (*osub_95F2E)(int a1, unsigned char* a2, size_t a3); //case 35 power
int __fastcall hsub_95F2E(int a1, unsigned char* a2, size_t a3) {
    if (a3 == 0x16 || a3 == 0x32) {
        //LOGI("%p",a3);
        return osub_95F2E(a1, a2, a3);
    }
    else return 0;
    return osub_95F2E(a1, a2, a3);
}
size_t h2k_strlen(const char* s) {

    if (strstr(s, "egl")) {
        s = "www.fuckpubg.com";
        //LOGI("S {%s}",s);
    }

    return strlen(s);
}

size_t hok___strlen(const char* s)
{
    if (strstr(s, "Thread-4")) {
        s = "www.gameprohack.com";
    }
    //LOGI("libCrashSight %s",s);
    return strlen(s);
}

void* hok___memcpy(void* a1, const void* a2, size_t a3)
{
    if (a3 == 0x12 || a3 == 0x14 || a3 == 0x4) {
        return (void*)hok___memcpy(a1, a2, 0x13);
    }
    //LOGI("copy {%p}",a3);
    return memcpy(a1, a2, a3);
}
int anog = Tools::GetBaseAddress("libanogs.so");


int __fastcall (*sub_1B4E58)(int a1);
int __fastcall ffsub_1B4E58(int a1) {
    int v7[17];
    int v1; // r0
    int i;
    int dest[17];
    char byte_4[4];
    int v6[17];
    int v5;
    v6[0] = a1;
    v6[1] = a1 + 0;
    v6[2] = a1 + 0;
    v6[3] = a1 + 0;
    v6[4] = a1 + 0;
    v6[5] = a1 + 0;
    v6[6] = a1 + 0;
    v6[7] = a1 + 0;
    v6[8] = a1 + 0;
    v6[9] = a1 + 0;
    v6[10] = a1 + 0;
    v6[11] = a1 + 0;
    v6[12] = a1 + 0;
    v6[13] = a1 + 0;
    v6[14] = a1 + 0;
    v6[15] = a1 + 0;
    v6[16] = a1 + 0;

    LOGI("v6 ");

    return sub_1B4E58(a1);
}
int __fastcall (*sub_1556FC)(int a1, int a2, int* a3);
int __fastcall fssub_1556FC(int a1, int a2, int* a3) {
    int v4; // [sp+Ch] [bp-34h]
    int v6; // [sp+18h] [bp-28h]
    unsigned int v7; // [sp+20h] [bp-20h]
    char v10; // [sp+37h] [bp-9h]
    unsigned int v11; // [sp+38h] [bp-8h] BYREF
    if ((*(_BYTE*)(a2 + 36) & 1) == 1)
    {
        LOGI("STACH");
        /////*(_BYTE *)(a2 + 36) = -0;
    }
    else {
        v11 = 0;
        *(_BYTE*)(a2 + 36) = -0;
        *(_WORD*)(a2 + 38) = -0;
        if (*(_WORD*)(v6 + 520))
        {


        }
        else {
            LOGI("STACHSTACHSTACH");
            v11 = 0;
        }
        *(_BYTE*)(a2 + 36) = -1;
    }
    return sub_1556FC(a1, a2, a3);

}


int __fastcall (*sub_1062B8)(int a1, const char* a2);
int __fastcall ggsub_1062B8(int a1, const char* a2) {

    if (a2) {
        a2 = "www.gameprohack.com";
        LOGI("sub_1062B8 [%s]", a2);
    }
    return sub_1062B8(a1, a2);
}


int __fastcall (*ReleaseDolphin)(int result);
int __fastcall ffReleaseDolphin(int result) {

    DWORD* v1; // r4

    v1 = (DWORD*)result;
    if (result)
    {
        LOGI("ffReleaseDolphin");
        result = *(DWORD*)0;
        if (result)
        {
            result = (*(int(__fastcall**)(int))(*(DWORD*)result + 0))(result);
            *v1 = 0;
        }
    }
    return result;
    return ReleaseDolphin(result);
}




void* hoook___memset(void* s, int c, size_t n)
{
    if (n == 0x10) {
        LOGI("{s %s} {C %d} {N %p}", s, c, n);
        return 0;
    }
    return memset(s, c, n);
}



int (*osub_E2172)(const char* a1, unsigned int a2);
int hsub_E2172(const char* a1, unsigned int a2)
{
    while (true)
    {
        sleep(10000);
    }
    return osub_E2172(a1, a2);
}
int (*osub_retzero)(const char* a1, unsigned int a2);
int hsub_retzero(const char* a1, unsigned int a2)
{
    return 0;
}
int ret_32()
{
    return 32;
}
int retzero()
{
    return 0;
}
int ret_55()
{
    return 0;
}
int __fastcall (*sub_2BD1C)(int a1);
int __fastcall ffsub_2BD1C(int a1) {

    LOGI("libTDataMaster.so");
    return sub_2BD1C(a1);
}

int (*oBatteryMod)(int a1, int a2, int ChargingState, int BatteryLevel, float a5);
int hBatteryMod(int a1, int a2, int ChargingState, int BatteryLevel, float a5)
{
    //a3 = charging state
    //2 = charging | 1 = not charging
    int NewChargingState = 1;
    *(int*)(libUE4Base + 0x8E7F60C) = NewChargingState;
    BatteryLevel = 90;
    *(int*)(libUE4Base + 0x8E7F610) = BatteryLevel;
    oBatteryMod(a1, a2, NewChargingState, BatteryLevel, a5);
    return 0;
}
void* SuperThread(void* parms) {

    LOGI(OBFUSCATE("Hooking method started..."));
    HOOK_LIB("libanort.so", "0xD49DF", hsub_E2172, osub_E2172);

    UE4 = Tools::GetBaseAddress("libUE4.so");
    while (!UE4) {
        UE4 = Tools::GetBaseAddress("libUE4.so");
        sleep(1);
    }



    while (!g_App) {
        g_App = *(android_app**)(UE4 + GNativeAndroidApp_Offset);
        sleep(1);
    }
    while (!g_App->onInputEvent)
        sleep(1);
    orig_onInputEvent = decltype(orig_onInputEvent)(g_App->onInputEvent);
    g_App->onInputEvent = onInputEvent;



    FName::GNames = GetGNames();
    while (!FName::GNames) {
        FName::GNames = GetGNames();
        sleep(1);
    }


    UObject::GUObjectArray = (FUObjectArray*)(UE4 + GUObject_Offset); // REMOVE GUEST FORCE LINK


    //HOOKSYM_LIB("/system/lib/libEGL.so", "eglSwapBuffers", _eglSwapBuffers, orig_eglSwapBuffers);
    // 
    // hile gelmesi
    Tools::Hook((void*)DobbySymbolResolver(OBFUSCATE("/system/lib/libandroid_runtime.so"), OBFUSCATE("eglSwapBuffers")), (void*)_eglSwapBuffers, (void**)&orig_eglSwapBuffers);
    pthread_t ptid1;
    pthread_create(&ptid1, 0, maps_thread, 0);


    return nullptr;

}
#define HOOK(target, hook, original) Tools::Hook((void *)(target), (void *)(hook), (void **)(original))

__attribute__((constructor))
void _init() {
    pthread_t ptid1;
    pthread_create(&ptid1, NULL, SuperThread, NULL);


    //if (!FileExist("/data/system/settings_policy.db"))
    //{}
    //else {

    //}
    //if (!FileExist("/data/data/gameloop")) //yoksa
    //{

    //}
    //else {
    //    pthread_t ptid1;
    //    pthread_create(&ptid1, NULL, SuperThread, NULL);
    //}

}
