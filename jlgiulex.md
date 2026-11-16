代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ftm.xuanzx.com

[S25] C：内存拷贝
来源：http://rui.haohaochexian.top

memcpy(dst, src, n);
来源：http://pmg.tarul.cn

[S26] C：内存清零
来源：http://rcx.yj202588.top

memset(a, 0, sizeof a);
来源：http://dzv.316326.xyz

[S27] C：定义常量
来源：http://sfb.yj20258888.top

const double PI = 3.14159;
来源：http://vcr.mhx1999.top

[S28] C：静态变量
来源：http://xcs.guowangkeji.top

static int counter = 0;
来源：http://how.gaohongyu789.top

[S29] C：变参函数
来源：http://fod.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kvb.iojbl.cn

[S30] C：头文件保护
来源：http://ske.yfazqb.com

#ifndef X_H
来源：http://oxj.yonumen.top

#define X_H
来源：http://xnd.cdnleiting.top

#endif
来源：http://bjp.zhengqikj.top

[S31] C++：Hello World
来源：http://iid.jqgufenzy.top

#include <iostream>
来源：http://rpe.hongshengwenyu.top

int main() { std::cout << "Hello\n"; }
来源：http://mzt.tanke756.top

[S32] C++：字符串
来源：http://bku.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://cmt.epnwcf.com

[S33] C++：vector 增删
来源：http://mov.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aeh.jinqigufen.top

[S34] C++：遍历 vector
来源：http://uin.ydzc1.top

for (auto &x : v) { std::cout << x; }
来源：http://wms.zhongyouzk.top

[S35] C++：map
来源：http://zrq.ctjpmb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bab.hongshengwenyu.top

[S36] C++：unordered_map
来源：http://yxh.fehbvm.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ltd.tarul.cn

[S37] C++：set
来源：http://qkp.ybcxt.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yfi.snrcjt.cn

[S38] C++：排序
来源：http://dve.zhaomingkeji.xyz

std::sort(v.begin(), v.end());
来源：http://adr.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://uyi.zhijiandao.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vaz.xylfe.cn

[S40] C++：查找元素
来源：http://gfj.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jrb.meibo888.top

[S41] C++：类与构造函数
来源：http://sbx.ybcxt.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hsy.redwolf501.top

[S42] C++：继承与虚函数
来源：http://hjy.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://lbb.pycfn.com

[S43] C++：智能指针
来源：http://qnu.jianghu66.top

auto p = std::make_unique<int>(5);
来源：http://awy.yongpay.top

[S44] C++：引用传参
来源：http://igv.vehdjk.com

void inc(int &x) { ++x; }
来源：http://htk.xinyue.icu

[S45] C++：lambda
来源：http://nmx.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cfe.jiagoushi.top

[S46] C++：函数模板
来源：http://yrv.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bxv.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://mam.52xcode.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://toj.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://pkm.hesvh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fha.ydjk.org.cn

while (std::getline(in, line)) { }
来源：http://stl.shanyushiyangkeji.top

[S49] C++：写文件
来源：http://taz.shangyingyoupin.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://edr.fehbvm.com

[S50] C++：格式化数字
来源：http://mkv.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://znw.shuidangran.top

[S51] C++：显式类型转换
来源：http://tla.kuanghao11.cn

static_cast<double>(a) / b
来源：http://vjn.yongpay.top

[S52] C++：const 与 noexcept
来源：http://pvo.fanxiaobao.xyz

int size() const noexcept { return n_; }
来源：http://fkv.zycfv.cn

[S53] C++：移动语义
来源：http://scr.yonumen.top

std::vector<int> w = std::move(v);
来源：http://uoy.vehdjk.com

[S54] C++：异常处理
来源：http://mvy.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://roj.c1oappe.top

[S55] C++：结构化绑定
来源：http://ngb.sufxvd.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ujk.redwolf501.top

[S56] C++：optional
来源：http://zlb.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://upc.yuanzhike.top

[S57] C++：编译期常量
来源：http://dpp.jinqigufen.top

constexpr int N = 10;
来源：http://xoj.yvedp.cn

[S58] C++：命名空间
来源：http://tdb.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://ula.jinghuilouyu.cn

[S59] C++：静态断言
来源：http://jge.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ijw.chenlongwang.top

[S60] C++：遍历并删除元素
来源：http://yyt.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kig.sufxvd.cn

================================================================================
来源：http://wws.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zcz.zhijiandao.cn

================================================================================
来源：http://mzv.ivvv.top

[T01] Kotlin：Hello World
来源：http://vax.c1oappe.top

println("Hello")
来源：http://wdo.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://ond.chenjidiqi.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ctz.zdbjq.cn

[T03] Kotlin：字符串模板
来源：http://csr.hcnkem.com

"值: $b"
来源：http://rdt.dianchejie.cn

[T04] Kotlin：空安全
来源：http://pmu.epnwcf.com

val n: String? = null;  n?.length
来源：http://biy.jinqigfzy.top

[T05] Kotlin：when 表达式
来源：http://fzl.52xcode.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aat.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://uef.ybcxt.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ulf.fehbvm.com

[T07] Kotlin：集合过滤
来源：http://zgx.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hfi.mhx1999.top

[T08] Kotlin：数据类
来源：http://ndd.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://txh.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://wqm.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://vhj.pycfn.com

[T10] Kotlin：默认参数
来源：http://cpa.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sxn.hysaishi.cn

[T11] Kotlin：协程
来源：http://apv.hfpthk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kev.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://xrx.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://idz.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://rlp.redwolf501.top

val m = mapOf("a" to 1)
来源：http://nww.hesvh.cn

[T14] Kotlin：循环
来源：http://yug.yj20258.top

for (i in 1..10) println(i)
来源：http://qka.hnxiangtu.top

[T15] Kotlin：接口
来源：http://wpa.tanke756.top

interface Shape { fun area(): Double }
来源：http://dyz.zycfv.cn

[T16] Swift：Hello World
来源：http://akk.havefunace.top

print("Hello")
来源：http://tor.ybcxt.top

[T17] Swift：变量与常量
来源：http://lvq.snrcjt.cn

var a = 1;  let b = 2
来源：http://qzt.chenlongwang.top

[T18] Swift：字符串插值
来源：http://pbd.bbcook.cn

"值: \(b)"
来源：http://ala.vqdsnc.cn

[T19] Swift：可选绑定
来源：http://iez.yj20258888.top

if let n = opt { print(n) }
来源：http://ldq.ydjk.org.cn

[T20] Swift：数组操作
来源：http://giw.cheryme.top

var a = [1, 2, 3];  a.append(4)
来源：http://cru.gaohongyu789.top

[T21] Swift：遍历
来源：http://mgc.zhongyouzk.top

for x in a { print(x) }
来源：http://jon.gzhubu.top

[T22] Swift：字典
来源：http://vdq.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hou.ppjwa.cn

[T23] Swift：函数
来源：http://dcq.xylfe.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vht.aizwys.cn

[T24] Swift：闭包
来源：http://eki.guowangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tpq.xuanzx.com

[T25] Swift：结构体
来源：http://hcx.pycfn.com

struct P { var x: Int }
来源：http://cde.jinqigfzy.top

[T26] Swift：类与重写
来源：http://nqw.gogol.net.cn

class A: Base { override func f() {} }
来源：http://zzr.daria6918.cn

[T27] Swift：错误处理
来源：http://orc.nwbrower.top

do { try f() } catch { print(error) }
来源：http://vwm.zycfv.cn

[T28] Swift：枚举
来源：http://pbj.jiagoushi.top

enum Color { case red, green }
来源：http://vqc.52xcode.cn

[T29] Swift：guard 提前返回
来源：http://tdx.0kj1m.cn

guard let x = opt else { return }
来源：http://odo.daxiang520.top

[T30] Swift：协议
来源：http://yot.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://mzh.bbcook.cn

[T31] Lua：Hello World
来源：http://bwf.0kj1m.cn

print("Hello")
来源：http://idr.hammf.cn

[T32] Lua：局部变量
来源：http://dvt.haohaochexian.top

local a = 1
来源：http://bpc.nanxuanxn.top

[T33] Lua：表（数组）
来源：http://sxv.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://uvq.zdqjudy.top

[T34] Lua：遍历表
来源：http://acg.sufxvd.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dxn.yanxiufei.cn

[T35] Lua：字典表
来源：http://xit.bbcook.cn

local d = { a = 1 };  d.b = 2
来源：http://yfp.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://cst.jinqigfzy.top

function add(a, b) return a + b end
来源：http://ity.tarul.cn

[T37] Lua：字符串拼接
来源：http://uhy.fanxiaobao.xyz

"a" .. "b"
来源：http://ykd.fktsv.cn

[T38] Lua：条件
来源：http://mwt.jyoumei.cn

if x > 0 then print("正") end
来源：http://kra.tanke756.top

[T39] Lua：模式匹配
来源：http://hvf.jinqigfzy.top

string.find(s, "%d+")
来源：http://djr.cdnleiting.top

[T40] Lua：元表
来源：http://qew.shangyingyoupin.top

setmetatable({}, { __index = base })
来源：http://jip.redwolf501.top

[T41] Perl：Hello World
来源：http://uuz.xingfuxueyuan.xyz

print "Hello\n";
来源：http://wam.quarkkingdee.top

[T42] Perl：变量类型
来源：http://blf.wangshuangyany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cuo.zhoulong.xyz

[T43] Perl：字符串插值
来源：http://tks.zhixingplan.top

"值: $a"
来源：http://bzq.pengpengdd.cyou

[T44] Perl：条件
来源：http://wsl.shanyushiyangtech.top

if ($a > 0) { print "正"; }
来源：http://abb.hysaishi.cn

[T45] Perl：数组遍历
来源：http://auh.gotoacloud.top

for my $x (@arr) { print $x; }
来源：http://tre.andypj.xyz

[T46] Perl：哈希操作
来源：http://uov.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fiw.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://dhi.ivvv.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pqu.sweek.top

[T48] Perl：正则替换
来源：http://you.fehbvm.com

$s =~ s/old/new/g;
来源：http://zls.dianchejie.cn

[T49] Perl：函数
来源：http://oub.52xcode.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://muc.sjlbkw.cn

[T50] Perl：逐行读文件
来源：http://unu.xuanzx.com

open my $fh, "<", "a.txt" or die $!;
来源：http://uru.gotoacloud.top

while (my $line = <$fh>) { print $line; }
来源：http://yge.zhoulong.xyz

[T51] Scala：Hello World
来源：http://vfj.nanxinkj.top

println("Hello")
来源：http://yst.yuxming.cn

[T52] Scala：变量
来源：http://upu.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://aqs.sysykeji.top

[T53] Scala：字符串插值
来源：http://llk.jinghuilouyu.cn

s"值: $b"
来源：http://eyh.yangfankeji.com

[T54] Scala：集合映射
来源：http://kkl.hywenlv.cn

List(1, 2, 3).map(_ * 2)
来源：http://wud.birdmap.top

[T55] Scala：集合过滤
来源：http://oki.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://meh.ppjwa.cn

[T56] Scala：样例类
来源：http://djg.dianchejie.cn

case class User(name: String, age: Int)
来源：http://lxr.yj20258888.top

[T57] Scala：模式匹配
来源：http://dst.pengpengdd.cyou

x match { case 1 => "一"; case _ => "其他" }
来源：http://qwv.xuanzx.com

[T58] Scala：函数定义
来源：http://scw.cheryme.top

def add(a: Int, b: Int): Int = a + b
来源：http://mhc.jqgufenzy.top

[T59] Scala：循环
来源：http://ewk.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://yum.cdnleiting.top

[T60] Scala：折叠
来源：http://qmi.dianchejie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kaw.zdbjq.cn

================================================================================
来源：http://dgb.ybcxt.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yzk.aizwys.cn

================================================================================
来源：http://wch.meibo888.top

[U01] Py：创建虚拟环境
来源：http://nun.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oke.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://jnq.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jrc.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://ztn.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ybc.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://qmy.0kj1m.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mkd.shanyushiyangtech.top

[U05] Py：列表去重且保序
来源：http://ilw.cqqwz.cn

list(dict.fromkeys(arr))
来源：http://mbo.sxryk.cn

[U06] Py：合并两个字典
来源：http://ejp.ydzc1.top

{**a, **b}
来源：http://vuh.tarul.cn

[U07] Py：反转字典键值
来源：http://frm.ywan-chungtsiang.top

{v: k for k, v in d.items()}
来源：http://vhx.feifeiyinyue.top

[U08] Py：展平二维列表
来源：http://nwz.gogol.net.cn

[y for x in nested for y in x]
来源：http://dff.316326.xyz

[U09] Py：字典取最大值的键
来源：http://xvb.epnwcf.com

max(d, key=d.get)
来源：http://ayr.xuanzx.com

[U10] Py：按值排序字典
来源：http://cgb.gaohongyu789.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nsz.yuxming.cn

[U11] Py：生成器表达式
来源：http://bxe.dashuyun.cn

(x * 2 for x in arr)
来源：http://jug.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bes.vqdsnc.cn

Counter(arr).most_common(3)
来源：http://dwi.fzhhl.top

[U13] Py：固定长度队列
来源：http://syv.c1oappe.top

deque(maxlen=10)
来源：http://qzj.sjlbkw.cn

[U14] Py：分组收集到列表
来源：http://xqo.yuxming.cn

defaultdict(list)
来源：http://zwy.nwbrower.top

[U15] Py：高精度计时
来源：http://hjs.xuetiantiany.cn

t = time.perf_counter()
来源：http://uom.aizwys.cn

[U16] Py：命令行参数解析
来源：http://hqd.redwolf501.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://arc.zdbjq.cn

[U17] Py：初始化日志
来源：http://aax.gotoacloud.top

logging.basicConfig(level=logging.INFO)
来源：http://ytf.hnxiangtu.top

[U18] Py：预编译正则
来源：http://yfb.chenzaomai.com

pat = re.compile(r"\d+")
来源：http://unr.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://xre.jqgufenzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tzq.hywenlv.cn

[U20] Py：缓存函数结果
来源：http://iml.jiagoushi.top

@functools.lru_cache(maxsize=None)
来源：http://rwl.birdmap.top

[U21] Py：自定义上下文管理器
来源：http://jwh.316326.xyz

@contextlib.contextmanager
来源：http://klv.cashguo.top

[U22] Py：矩阵转置
来源：http://aer.gogol.net.cn

list(zip(*m))
来源：http://nbm.xingfuxueyuan.xyz

[U23] Py：分块读取大文件
来源：http://suo.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qld.yuanzhike.top

[U24] Py：路径操作
来源：http://fld.cqqwz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wkd.yangfankeji.com

[U25] Py：CSV 按字典读
来源：http://jin.vqdsnc.cn

csv.DictReader(f)
来源：http://ptg.chenlongwang.top

[U26] Py：并发下载
来源：http://eoo.gogol.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://edx.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://pyz.jinyuanbaomall.cn

aiohttp.ClientSession() 配合 async with
来源：http://dcx.tianlin.xyz

[U28] Py：类型别名
来源：http://erd.yj20258.top

UserId = int
来源：http://izh.fktsv.cn

[U29] Py：属性校验
来源：http://gpy.sxryk.cn

@property 与 @x.setter 配合
来源：http://qmy.yj20258.top

[U30] Py：数据类
来源：http://dgn.shangyingyoupin.top

@dataclass(slots=True)
来源：http://woe.zhaomingkeji.xyz

[U31] Py：单测
来源：http://xed.zhixingplan.top

python -m pytest -q
来源：http://nbm.jlsjyb.cn

[U32] Py：代码格式化
来源：http://lqm.smart0.xyz

ruff format . && ruff check --fix .
来源：http://cyh.pengpengdd.cyou

[U33] Py：打包发布
来源：http://noc.gotoacloud.top

python -m build  （依赖 pyproject.toml）
来源：http://era.fehbvm.com

[U34] Py：判断编码
来源：http://lqf.wangshuangyany.cn

chardet.detect(raw)
来源：http://ftd.vqdsnc.cn

[U35] Py：发送邮件
来源：http://ejv.iojbl.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://csh.smart0.xyz

[U36] Py：定时任务
来源：http://tkh.hesvh.cn

schedule.every(10).minutes.do(job)
来源：http://sjd.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://qeu.fengsongda.top

pandas.read_excel / DataFrame.to_excel
来源：http://nnm.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://mwj.shangyingyoupin.top

Path(__file__).resolve().parent
来源：http://fxn.yongpay.top

[U39] Py：判断是否在交互环境
来源：http://ias.yj20258.top

sys.stdout.isatty()
来源：http://xtg.jqgufenzy.top

[U40] Py：打印到标准错误
来源：http://hne.sxryk.cn

print("err", file=sys.stderr)
来源：http://zgt.yj20258888.top

[U41] PHP：初始化 Composer 项目
来源：http://hxl.feifeiyinyue.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qwf.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://myv.fehbvm.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blf.zhoulong.xyz

[U43] PHP：声明命名空间
来源：http://cuw.daria6918.cn

namespace App\Http;
来源：http://fhs.jinghuilouyu.cn

[U44] PHP：开启严格类型
来源：http://qsm.tanke756.top

declare(strict_types=1);
来源：http://lnc.zdqjudy.top

[U45] PHP：类型声明与返回类型
来源：http://nts.jinqigfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lja.yj202588.top

[U46] PHP：可空类型
来源：http://ogz.hcnkem.com

?string $name = null
来源：http://coi.chenlongwang.top

[U47] PHP：联合类型
来源：http://bxi.fengsongda.top

int|string $id
来源：http://ebp.zhaomingkeji.xyz

[U48] PHP：纯枚举
来源：http://irv.xylfe.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zae.shanyushiyangkeji.top


<!-- 参考信息 -->