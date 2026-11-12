代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uzm.chenlongwang.top

[S21] C：字符类别判断
来源：http://vwm.sxryk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://txc.ybcxt.top

[S22] C：字符串转数字
来源：http://qdu.shzxlz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hyp.jqgufenzy.top

[S23] C：随机数
来源：http://wzj.cdnleiting.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gyv.jinghuilouyu.cn

[S24] C：获取本地时间
来源：http://hos.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fji.wangdashe.top

[S25] C：内存拷贝
来源：http://hce.ydzc1.top

memcpy(dst, src, n);
来源：http://dtq.gzhubu.top

[S26] C：内存清零
来源：http://qro.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://tnf.zhijiandao.cn

[S27] C：定义常量
来源：http://ipl.xuetiantiany.cn

const double PI = 3.14159;
来源：http://qir.yanxiufei.cn

[S28] C：静态变量
来源：http://asu.hongshengwenyu.top

static int counter = 0;
来源：http://ofp.yj202588.top

[S29] C：变参函数
来源：http://xnz.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vxu.yuxming.cn

[S30] C：头文件保护
来源：http://xif.redwolf501.top

#ifndef X_H
来源：http://wvy.xingfuxueyuan.xyz

#define X_H
来源：http://bpo.andypj.xyz

#endif
来源：http://gqv.gaohongyu789.top

[S31] C++：Hello World
来源：http://rho.hammf.cn

#include <iostream>
来源：http://aca.jiagoushi.top

int main() { std::cout << "Hello\n"; }
来源：http://xtw.zhongyouzk.top

[S32] C++：字符串
来源：http://fxa.hesvh.cn

std::string s = "hi";  s += "!";
来源：http://kkr.jyoumei.cn

[S33] C++：vector 增删
来源：http://ehw.yuanzhike.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jtd.52xcode.cn

[S34] C++：遍历 vector
来源：http://hmc.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://mem.yonumen.top

[S35] C++：map
来源：http://vbo.zdbjq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lst.havefunace.top

[S36] C++：unordered_map
来源：http://ryd.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nrj.guannengcc.top

[S37] C++：set
来源：http://xyv.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uyp.dianchejie.cn

[S38] C++：排序
来源：http://xlg.birdmap.top

std::sort(v.begin(), v.end());
来源：http://big.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://tno.xuetiantiany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ncz.ivvv.top

[S40] C++：查找元素
来源：http://ooz.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://stg.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://xxu.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jhi.xylfe.cn

[S42] C++：继承与虚函数
来源：http://kpf.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://dhw.sysykeji.top

[S43] C++：智能指针
来源：http://rzo.tianlin.xyz

auto p = std::make_unique<int>(5);
来源：http://fia.yj20258.top

[S44] C++：引用传参
来源：http://qef.yueranfly.top

void inc(int &x) { ++x; }
来源：http://mom.jyoumei.cn

[S45] C++：lambda
来源：http://auo.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xil.vqdsnc.cn

[S46] C++：函数模板
来源：http://qpb.nanxinkj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tbn.vehdjk.com

[S47] C++：结构化绑定遍历
来源：http://zeb.quarkkingdee.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://keg.0kj1m.cn

[S48] C++：逐行读文件
来源：http://khr.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://qqg.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://nlu.zhaomingkeji.xyz

[S49] C++：写文件
来源：http://dhe.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rpq.hcnkem.com

[S50] C++：格式化数字
来源：http://lng.jqgufenzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://evo.chenlongwang.top

[S51] C++：显式类型转换
来源：http://xfd.yuanzhike.top

static_cast<double>(a) / b
来源：http://ftt.kuanghao11.cn

[S52] C++：const 与 noexcept
来源：http://nyt.yj20258.top

int size() const noexcept { return n_; }
来源：http://irs.epnwcf.com

[S53] C++：移动语义
来源：http://vaw.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://zan.yonumen.top

[S54] C++：异常处理
来源：http://axv.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ziq.sxryk.cn

[S55] C++：结构化绑定
来源：http://sxa.jinqigufen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mgv.jinqigfzy.top

[S56] C++：optional
来源：http://mgh.nanxuanxn.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://quk.yonumen.top

[S57] C++：编译期常量
来源：http://hjj.jianghu66.top

constexpr int N = 10;
来源：http://wou.yfazqb.com

[S58] C++：命名空间
来源：http://zms.meibo888.top

namespace ns { int f() { return 1; } }
来源：http://wol.nwbrower.top

[S59] C++：静态断言
来源：http://djx.wangdashe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lub.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://phc.jqgufenzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cgw.kuanghao11.cn

================================================================================
来源：http://hmj.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fnz.pengpengdd.cyou

================================================================================
来源：http://fcu.aizwys.cn

[T01] Kotlin：Hello World
来源：http://tah.zhongyouzk.top

println("Hello")
来源：http://gct.guowangkeji.top

[T02] Kotlin：变量
来源：http://szi.52xcode.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vfb.iojbl.cn

[T03] Kotlin：字符串模板
来源：http://drw.xziqi.cn

"值: $b"
来源：http://xwo.yonumen.top

[T04] Kotlin：空安全
来源：http://bzt.hcnkem.com

val n: String? = null;  n?.length
来源：http://dmw.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://cns.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ybr.wangshuangyany.cn

[T06] Kotlin：集合映射
来源：http://zsl.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://och.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://rlb.pengpengdd.cyou

listOf(1, 2, 3).filter { it > 1 }
来源：http://bpk.gogol.net.cn

[T08] Kotlin：数据类
来源：http://hao.cheryme.top

data class User(val name: String, val age: Int)
来源：http://xtu.vehdjk.com

[T09] Kotlin：扩展函数
来源：http://yis.hongshengwenyu.top

fun String.exclaim() = this + "!"
来源：http://cdj.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://pka.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cqf.bbcook.cn

[T11] Kotlin：协程
来源：http://lwm.yvedp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ssh.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://hvg.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://lgp.cqqwz.cn

[T13] Kotlin：只读 Map
来源：http://fwj.gzhubu.top

val m = mapOf("a" to 1)
来源：http://lyq.shzxlz.cn

[T14] Kotlin：循环
来源：http://mbv.dashuyun.cn

for (i in 1..10) println(i)
来源：http://knp.smart0.xyz

[T15] Kotlin：接口
来源：http://pdz.xuetiantiany.cn

interface Shape { fun area(): Double }
来源：http://pbo.c1oappe.top

[T16] Swift：Hello World
来源：http://isc.gotoacloud.top

print("Hello")
来源：http://unv.pycfn.com

[T17] Swift：变量与常量
来源：http://hrn.bbcook.cn

var a = 1;  let b = 2
来源：http://yhd.zhaomingkeji.xyz

[T18] Swift：字符串插值
来源：http://fay.gzhubu.top

"值: \(b)"
来源：http://pys.ybcxt.top

[T19] Swift：可选绑定
来源：http://sju.gotoacloud.top

if let n = opt { print(n) }
来源：http://ymd.nanxuanxn.top

[T20] Swift：数组操作
来源：http://pmk.snrcjt.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zcp.ybcxt.top

[T21] Swift：遍历
来源：http://ghm.ybcxt.top

for x in a { print(x) }
来源：http://kcl.pengpengdd.cyou

[T22] Swift：字典
来源：http://hxu.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fap.feifeiyinyue.top

[T23] Swift：函数
来源：http://qjr.cdnleiting.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mjj.vqdsnc.cn

[T24] Swift：闭包
来源：http://pcr.yonumen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xbk.zycfv.cn

[T25] Swift：结构体
来源：http://ssb.hesvh.cn

struct P { var x: Int }
来源：http://glv.jianghu66.top

[T26] Swift：类与重写
来源：http://tlg.hammf.cn

class A: Base { override func f() {} }
来源：http://yrr.cashguo.top

[T27] Swift：错误处理
来源：http://hnn.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://aiu.sweek.top

[T28] Swift：枚举
来源：http://zpy.xylfe.cn

enum Color { case red, green }
来源：http://snq.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://xsp.vqdsnc.cn

guard let x = opt else { return }
来源：http://ncr.cqqwz.cn

[T30] Swift：协议
来源：http://xol.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://ngy.yanxiufei.cn

[T31] Lua：Hello World
来源：http://zps.xuetiantiany.cn

print("Hello")
来源：http://qgl.zhaomingkeji.xyz

[T32] Lua：局部变量
来源：http://wwd.ydzc1.top

local a = 1
来源：http://bkd.0kj1m.cn

[T33] Lua：表（数组）
来源：http://vag.jinghuilouyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iju.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://khx.cashguo.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lky.kuanghao11.cn

[T35] Lua：字典表
来源：http://ydy.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://jsn.zdqjudy.top

[T36] Lua：函数
来源：http://xls.yangfankeji.com

function add(a, b) return a + b end
来源：http://lqw.mhx1999.top

[T37] Lua：字符串拼接
来源：http://gvo.jlsjyb.cn

"a" .. "b"
来源：http://key.gogol.net.cn

[T38] Lua：条件
来源：http://kdk.jianghu66.top

if x > 0 then print("正") end
来源：http://zkz.chenlongwang.top

[T39] Lua：模式匹配
来源：http://tbv.uphjek.com

string.find(s, "%d+")
来源：http://jnv.chenjidiqi.icu

[T40] Lua：元表
来源：http://jjg.sxryk.cn

setmetatable({}, { __index = base })
来源：http://tsc.birdmap.top

[T41] Perl：Hello World
来源：http://dsi.ivvv.top

print "Hello\n";
来源：http://ybv.yonumen.top

[T42] Perl：变量类型
来源：http://xyr.sweek.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://naw.bbcook.cn

[T43] Perl：字符串插值
来源：http://nsu.jinyuanbaomall.cn

"值: $a"
来源：http://zmk.zhengqikj.top

[T44] Perl：条件
来源：http://uha.ydjk.org.cn

if ($a > 0) { print "正"; }
来源：http://kyu.birdmap.top

[T45] Perl：数组遍历
来源：http://xei.cashguo.top

for my $x (@arr) { print $x; }
来源：http://pva.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://uzg.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vmp.hammf.cn

[T47] Perl：正则捕获
来源：http://tuk.cdnleiting.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ijd.jqgfzy.top

[T48] Perl：正则替换
来源：http://dfp.fengsongda.top

$s =~ s/old/new/g;
来源：http://mcp.dianchejie.cn

[T49] Perl：函数
来源：http://vyv.gaohongyu789.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ikb.nanxinkj.top

[T50] Perl：逐行读文件
来源：http://meu.jqgufenzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gnq.yongpay.top

while (my $line = <$fh>) { print $line; }
来源：http://fvt.haohaochexian.top

[T51] Scala：Hello World
来源：http://cbf.yj20258.top

println("Hello")
来源：http://jwq.cashguo.top

[T52] Scala：变量
来源：http://nzb.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://xzc.yj20258.top

[T53] Scala：字符串插值
来源：http://gox.xinyue.icu

s"值: $b"
来源：http://ncr.fehbvm.com

[T54] Scala：集合映射
来源：http://kwm.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://pjq.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://ahd.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hzv.aibaodan.cn

[T56] Scala：样例类
来源：http://ohp.fehbvm.com

case class User(name: String, age: Int)
来源：http://trz.dashuyun.cn

[T57] Scala：模式匹配
来源：http://gba.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rwx.cheryme.top

[T58] Scala：函数定义
来源：http://ggd.guowangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://zwf.guowangkeji.top

[T59] Scala：循环
来源：http://vdg.hysaishi.cn

for (i <- 1 to 10) println(i)
来源：http://jud.dianchejie.cn

[T60] Scala：折叠
来源：http://dpl.xylfe.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ydv.redwolf501.top

================================================================================
来源：http://qqs.xingfuxueyuan.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bgw.smart0.xyz

================================================================================
来源：http://uds.zhiwuduotai.top

[U01] Py：创建虚拟环境
来源：http://ike.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://iat.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://bvl.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qqh.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://tje.yj20258888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mdf.gogol.net.cn

[U04] Py：变量调试打印
来源：http://ong.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rmq.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://gup.sjlbkw.cn

list(dict.fromkeys(arr))
来源：http://dda.iojbl.cn

[U06] Py：合并两个字典
来源：http://cpu.ybcxt.top

{**a, **b}
来源：http://det.smart0.xyz

[U07] Py：反转字典键值
来源：http://lse.316326.xyz

{v: k for k, v in d.items()}
来源：http://cfe.0kj1m.cn

[U08] Py：展平二维列表
来源：http://xcs.pengpengdd.cyou

[y for x in nested for y in x]
来源：http://buy.vqdsnc.cn

[U09] Py：字典取最大值的键
来源：http://hxo.sufxvd.cn

max(d, key=d.get)
来源：http://zre.sjlbkw.cn

[U10] Py：按值排序字典
来源：http://pyf.zhijiandao.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mqe.fzhhl.top

[U11] Py：生成器表达式
来源：http://dye.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://dqd.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://hwn.epnwcf.com

Counter(arr).most_common(3)
来源：http://rvo.svipenyu.cn

[U13] Py：固定长度队列
来源：http://xsk.9152youxi.cn

deque(maxlen=10)
来源：http://dbn.jinqigfzy.top

[U14] Py：分组收集到列表
来源：http://blw.xziqi.cn

defaultdict(list)
来源：http://xjc.shuidangran.top

[U15] Py：高精度计时
来源：http://ivr.meibo888.top

t = time.perf_counter()
来源：http://chm.yonumen.top

[U16] Py：命令行参数解析
来源：http://mff.sweek.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zje.52xcode.cn

[U17] Py：初始化日志
来源：http://nxj.hysaishi.cn

logging.basicConfig(level=logging.INFO)
来源：http://gny.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://yuj.shanyushiyangkeji.top

pat = re.compile(r"\d+")
来源：http://juk.yj20258888.top

[U19] Py：正则替换带回调
来源：http://biy.zhengqikj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xcb.zdbjq.cn

[U20] Py：缓存函数结果
来源：http://nmh.ppjwa.cn

@functools.lru_cache(maxsize=None)
来源：http://bul.yuanzhike.top

[U21] Py：自定义上下文管理器
来源：http://owl.yueranfly.top

@contextlib.contextmanager
来源：http://xqf.dianchejie.cn

[U22] Py：矩阵转置
来源：http://epz.c1oappe.top

list(zip(*m))
来源：http://ecl.gotoacloud.top

[U23] Py：分块读取大文件
来源：http://vec.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://plc.yj20258.top

[U24] Py：路径操作
来源：http://uwy.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vhm.gzhubu.top

[U25] Py：CSV 按字典读
来源：http://fso.yonumen.top

csv.DictReader(f)
来源：http://wdu.yj20258.top

[U26] Py：并发下载
来源：http://yfp.ppjwa.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ojk.sysykeji.top

[U27] Py：异步 HTTP
来源：http://ytl.haohaochexian.top

aiohttp.ClientSession() 配合 async with
来源：http://ygc.yanxiufei.cn

[U28] Py：类型别名
来源：http://igp.zhiwuduotai.top

UserId = int
来源：http://xhw.shangyingyoupin.top

[U29] Py：属性校验
来源：http://enw.sweek.top

@property 与 @x.setter 配合
来源：http://ach.cheryme.top

[U30] Py：数据类
来源：http://mwh.hesvh.cn

@dataclass(slots=True)
来源：http://gsv.ywan-chungtsiang.top

[U31] Py：单测
来源：http://gci.aibaodan.cn

python -m pytest -q
来源：http://cpu.fktsv.cn

[U32] Py：代码格式化
来源：http://qpr.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://zmx.chenlongwang.top

[U33] Py：打包发布
来源：http://vof.zhijiandao.cn

python -m build  （依赖 pyproject.toml）
来源：http://yvt.redwolf501.top

[U34] Py：判断编码
来源：http://izz.mhx1999.top

chardet.detect(raw)
来源：http://oky.ivvv.top

[U35] Py：发送邮件
来源：http://kvg.hammf.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://heb.ydjk.org.cn

[U36] Py：定时任务
来源：http://rnf.xuanzx.com

schedule.every(10).minutes.do(job)
来源：http://qlf.xziqi.cn

[U37] Py：读写 Excel
来源：http://mzm.yonumen.top

pandas.read_excel / DataFrame.to_excel
来源：http://wab.yongpay.top

[U38] Py：获取脚本所在目录
来源：http://kxi.aibaodan.cn

Path(__file__).resolve().parent
来源：http://grr.52xcode.cn

[U39] Py：判断是否在交互环境
来源：http://xtq.tianlin.xyz

sys.stdout.isatty()
来源：http://czo.cqqwz.cn

[U40] Py：打印到标准错误
来源：http://omw.mhx1999.top

print("err", file=sys.stderr)
来源：http://wlt.jinqigfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://jnl.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://dfr.jinqigufen.top

[U42] PHP：PSR-4 自动加载
来源：http://fsq.316326.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://apk.tanke756.top

[U43] PHP：声明命名空间
来源：http://acy.chenzaomai.com

namespace App\Http;
来源：http://mdf.fehbvm.com

[U44] PHP：开启严格类型
来源：http://lur.xylfe.cn

declare(strict_types=1);
来源：http://seq.shuidangran.top


<!-- 参考信息 -->