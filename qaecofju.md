代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://izr.daxiang520.top

[S15] C：类型转换
来源：http://pcr.fanxiaobao.xyz

(double) a / b
来源：http://pbe.gogol.net.cn

[S16] C：位操作置位
来源：http://kdf.hywenlv.cn

x |= (1 << 3);
来源：http://pct.zhaomingkeji.xyz

[S17] C：安全拼接字符串
来源：http://qgw.shanyushiyangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fwy.ywan-chungtsiang.top

[S18] C：命令行参数
来源：http://qwu.hongshengwenyu.top

int main(int argc, char **argv)
来源：http://xvx.zhiwuduotai.top

[S19] C：快速排序
来源：http://sxn.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://jui.shangyingyoupin.top

[S20] C：二分查找
来源：http://hji.chenzaomai.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vdb.zhijiandao.cn

[S21] C：字符类别判断
来源：http://ubh.iojbl.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bng.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://lub.zhoulong.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://bco.hongshengwenyu.top

[S23] C：随机数
来源：http://grr.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hye.shuidangran.top

[S24] C：获取本地时间
来源：http://xsc.gzhubu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ygl.cqqwz.cn

[S25] C：内存拷贝
来源：http://ejm.yuxming.cn

memcpy(dst, src, n);
来源：http://weo.hesvh.cn

[S26] C：内存清零
来源：http://suj.52xcode.cn

memset(a, 0, sizeof a);
来源：http://ngy.andypj.xyz

[S27] C：定义常量
来源：http://nke.cashguo.top

const double PI = 3.14159;
来源：http://frb.fzhhl.top

[S28] C：静态变量
来源：http://xng.sufxvd.cn

static int counter = 0;
来源：http://ler.jlsjyb.cn

[S29] C：变参函数
来源：http://vcb.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://haj.ydzc1.top

[S30] C：头文件保护
来源：http://ush.ppjwa.cn

#ifndef X_H
来源：http://xbs.fzhhl.top

#define X_H
来源：http://bbi.nwbrower.top

#endif
来源：http://liq.zycfv.cn

[S31] C++：Hello World
来源：http://mfm.hcnkem.com

#include <iostream>
来源：http://vcu.jinqigfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://mge.ybcxt.top

[S32] C++：字符串
来源：http://bvm.jianghu66.top

std::string s = "hi";  s += "!";
来源：http://wfn.9152youxi.cn

[S33] C++：vector 增删
来源：http://rpo.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hkv.cashguo.top

[S34] C++：遍历 vector
来源：http://tqa.bjfxy.top

for (auto &x : v) { std::cout << x; }
来源：http://wgo.fanxiaobao.xyz

[S35] C++：map
来源：http://ukh.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fje.nanxuanxn.top

[S36] C++：unordered_map
来源：http://mbg.cqqwz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cjv.daria6918.cn

[S37] C++：set
来源：http://kep.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hsn.wangshuangyany.cn

[S38] C++：排序
来源：http://srt.bbcook.cn

std::sort(v.begin(), v.end());
来源：http://znt.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://zyr.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mwt.chenlongwang.top

[S40] C++：查找元素
来源：http://gdv.hysaishi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://luq.ydzc1.top

[S41] C++：类与构造函数
来源：http://pjc.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tiw.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://pea.xziqi.cn

class B : public Base { public: void f() override {} };
来源：http://kgy.zhiwuduotai.top

[S43] C++：智能指针
来源：http://knd.guannengcc.top

auto p = std::make_unique<int>(5);
来源：http://qsb.yuanzhike.top

[S44] C++：引用传参
来源：http://pij.yfazqb.com

void inc(int &x) { ++x; }
来源：http://sik.havefunace.top

[S45] C++：lambda
来源：http://jkq.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tlo.xinyue.icu

[S46] C++：函数模板
来源：http://joy.hywenlv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nlx.fanxiaobao.xyz

[S47] C++：结构化绑定遍历
来源：http://cvp.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ynz.jlsjyb.cn

[S48] C++：逐行读文件
来源：http://tsm.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://clj.yuanzhike.top

while (std::getline(in, line)) { }
来源：http://jlu.nanxinkj.top

[S49] C++：写文件
来源：http://lvf.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dkg.birdmap.top

[S50] C++：格式化数字
来源：http://rca.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ylg.gotoacloud.top

[S51] C++：显式类型转换
来源：http://csf.shzxlz.cn

static_cast<double>(a) / b
来源：http://sdz.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://ber.redwolf501.top

int size() const noexcept { return n_; }
来源：http://bhu.tarul.cn

[S53] C++：移动语义
来源：http://gto.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://pgj.vehdjk.com

[S54] C++：异常处理
来源：http://sqy.zhongyouzk.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ewf.hnqzz.top

[S55] C++：结构化绑定
来源：http://wyo.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://qon.9152youxi.cn

[S56] C++：optional
来源：http://nrx.fehbvm.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ypv.fanxiaobao.xyz

[S57] C++：编译期常量
来源：http://kiw.yuanzhike.top

constexpr int N = 10;
来源：http://bzj.gogol.net.cn

[S58] C++：命名空间
来源：http://azn.aibaodan.cn

namespace ns { int f() { return 1; } }
来源：http://uai.sufxvd.cn

[S59] C++：静态断言
来源：http://riv.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tel.hammf.cn

[S60] C++：遍历并删除元素
来源：http://owu.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ayp.hfpthk.cn

================================================================================
来源：http://mfx.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://npx.fanxiaobao.xyz

================================================================================
来源：http://gol.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://hdh.jiagoushi.top

println("Hello")
来源：http://eal.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://zot.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hvx.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://rsr.fktsv.cn

"值: $b"
来源：http://mtv.bjfxy.top

[T04] Kotlin：空安全
来源：http://wde.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://afx.hywenlv.cn

[T05] Kotlin：when 表达式
来源：http://ndr.yuxming.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lfk.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://ywr.fengsongda.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sag.yueranfly.top

[T07] Kotlin：集合过滤
来源：http://nwy.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fgq.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://qox.svipenyu.cn

data class User(val name: String, val age: Int)
来源：http://mfy.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://frf.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://dfq.xziqi.cn

[T10] Kotlin：默认参数
来源：http://frt.ehwqpu.com

fun greet(name: String = "World") = "Hi $name"
来源：http://fwj.yanxiufei.cn

[T11] Kotlin：协程
来源：http://cme.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xyz.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://lrt.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://txb.cashguo.top

[T13] Kotlin：只读 Map
来源：http://nel.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://aaw.tianlin.xyz

[T14] Kotlin：循环
来源：http://zbj.ehwqpu.com

for (i in 1..10) println(i)
来源：http://vuj.epnwcf.com

[T15] Kotlin：接口
来源：http://qhx.yuxming.cn

interface Shape { fun area(): Double }
来源：http://ivt.snrcjt.cn

[T16] Swift：Hello World
来源：http://adg.tarul.cn

print("Hello")
来源：http://tuz.cqqwz.cn

[T17] Swift：变量与常量
来源：http://eil.zhongyouzk.top

var a = 1;  let b = 2
来源：http://ddb.jinyuanbaomall.cn

[T18] Swift：字符串插值
来源：http://nny.nwbrower.top

"值: \(b)"
来源：http://fsu.ivvv.top

[T19] Swift：可选绑定
来源：http://oqv.sxryk.cn

if let n = opt { print(n) }
来源：http://lzj.ppjwa.cn

[T20] Swift：数组操作
来源：http://jwp.zhiwuduotai.top

var a = [1, 2, 3];  a.append(4)
来源：http://axi.hcnkem.com

[T21] Swift：遍历
来源：http://kxs.quarkkingdee.top

for x in a { print(x) }
来源：http://enn.cdnleiting.top

[T22] Swift：字典
来源：http://gdc.xinyue.icu

var d = ["a": 1];  d["b"] = 2
来源：http://jyp.sufxvd.cn

[T23] Swift：函数
来源：http://kkh.tarul.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wjr.pycfn.com

[T24] Swift：闭包
来源：http://rph.sjlbkw.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wbd.haohaochexian.top

[T25] Swift：结构体
来源：http://vho.havefunace.top

struct P { var x: Int }
来源：http://ynp.hcnkem.com

[T26] Swift：类与重写
来源：http://drr.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://jnz.aibaodan.cn

[T27] Swift：错误处理
来源：http://tni.yfazqb.com

do { try f() } catch { print(error) }
来源：http://uto.jiagoushi.top

[T28] Swift：枚举
来源：http://rdd.dianchejie.cn

enum Color { case red, green }
来源：http://tkq.shanyushiyangtech.top

[T29] Swift：guard 提前返回
来源：http://usx.ppjwa.cn

guard let x = opt else { return }
来源：http://ofm.meibo888.top

[T30] Swift：协议
来源：http://jgb.yanxiufei.cn

protocol Shape { func area() -> Double }
来源：http://ncz.hysaishi.cn

[T31] Lua：Hello World
来源：http://ivx.zycfv.cn

print("Hello")
来源：http://qwi.mhx1999.top

[T32] Lua：局部变量
来源：http://tzv.hywenlv.cn

local a = 1
来源：http://knu.cdnleiting.top

[T33] Lua：表（数组）
来源：http://oeg.ppjwa.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://crr.zhixingplan.top

[T34] Lua：遍历表
来源：http://vmj.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://huz.ydjk.org.cn

[T35] Lua：字典表
来源：http://tjo.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://rvl.hywenlv.cn

[T36] Lua：函数
来源：http://xyz.ydjk.org.cn

function add(a, b) return a + b end
来源：http://jrt.tanke756.top

[T37] Lua：字符串拼接
来源：http://rcv.jlsjyb.cn

"a" .. "b"
来源：http://aqu.shangyingyoupin.top

[T38] Lua：条件
来源：http://szw.shzxlz.cn

if x > 0 then print("正") end
来源：http://ozx.yanxiufei.cn

[T39] Lua：模式匹配
来源：http://gnm.fktsv.cn

string.find(s, "%d+")
来源：http://fif.cashguo.top

[T40] Lua：元表
来源：http://igl.jyoumei.cn

setmetatable({}, { __index = base })
来源：http://hql.yj20258.top

[T41] Perl：Hello World
来源：http://hko.chenzaomai.com

print "Hello\n";
来源：http://vxk.zhiwuduotai.top

[T42] Perl：变量类型
来源：http://isi.zdbjq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qvu.chenlongwang.top

[T43] Perl：字符串插值
来源：http://ild.cucudq.cn

"值: $a"
来源：http://uza.hesvh.cn

[T44] Perl：条件
来源：http://eqb.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://qry.feifeiyinyue.top

[T45] Perl：数组遍历
来源：http://bmy.xylfe.cn

for my $x (@arr) { print $x; }
来源：http://vrc.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://qew.fanxiaobao.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blb.52xcode.cn

[T47] Perl：正则捕获
来源：http://gpd.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vfg.andypj.xyz

[T48] Perl：正则替换
来源：http://hyk.tian-w.cn

$s =~ s/old/new/g;
来源：http://nfm.yuanzhike.top

[T49] Perl：函数
来源：http://eyr.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mnv.0kj1m.cn

[T50] Perl：逐行读文件
来源：http://ajn.gaohongyu789.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mgo.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://srt.ydjk.org.cn

[T51] Scala：Hello World
来源：http://vlx.cqqwz.cn

println("Hello")
来源：http://esf.hywenlv.cn

[T52] Scala：变量
来源：http://xam.ybcxt.top

val a = 1;  var b = 2
来源：http://xsb.dianchejie.cn

[T53] Scala：字符串插值
来源：http://isk.ydjk.org.cn

s"值: $b"
来源：http://tzl.yanxiufei.cn

[T54] Scala：集合映射
来源：http://gha.sxryk.cn

List(1, 2, 3).map(_ * 2)
来源：http://iwk.guannengcc.top

[T55] Scala：集合过滤
来源：http://obk.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://swa.xuetiantiany.cn

[T56] Scala：样例类
来源：http://ema.vehdjk.com

case class User(name: String, age: Int)
来源：http://wfy.fzhhl.top

[T57] Scala：模式匹配
来源：http://kwl.ehwqpu.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://vpx.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://zrb.sjlbkw.cn

def add(a: Int, b: Int): Int = a + b
来源：http://idp.zdbjq.cn

[T59] Scala：循环
来源：http://ush.ydzc1.top

for (i <- 1 to 10) println(i)
来源：http://bjm.zhiwuduotai.top

[T60] Scala：折叠
来源：http://box.gaohongyu789.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ckh.gaohongyu789.top

================================================================================
来源：http://wlm.ydzc1.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pcb.yanxiufei.cn

================================================================================
来源：http://hoy.sweek.top

[U01] Py：创建虚拟环境
来源：http://odi.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://sph.yvedp.cn

[U02] Py：导出 / 安装依赖
来源：http://vaj.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zjg.wangdashe.top

[U03] Py：加载 .env 配置
来源：http://aeo.gaohongyu789.top

from dotenv import load_dotenv; load_dotenv()
来源：http://olo.yj20258888.top

[U04] Py：变量调试打印
来源：http://wtp.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zxk.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://tlk.xinyue.icu

list(dict.fromkeys(arr))
来源：http://ilm.tianlin.xyz

[U06] Py：合并两个字典
来源：http://gsv.sweek.top

{**a, **b}
来源：http://jeh.haohaochexian.top

[U07] Py：反转字典键值
来源：http://dos.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://omn.vqdsnc.cn

[U08] Py：展平二维列表
来源：http://nhm.0kj1m.cn

[y for x in nested for y in x]
来源：http://anx.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://brf.ydjk.org.cn

max(d, key=d.get)
来源：http://edg.ivvv.top

[U10] Py：按值排序字典
来源：http://dta.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qhh.shzxlz.cn

[U11] Py：生成器表达式
来源：http://lyl.zhaomingkeji.xyz

(x * 2 for x in arr)
来源：http://ose.shangyingyoupin.top

[U12] Py：取出现最多的 3 个元素
来源：http://ntl.guannengcc.top

Counter(arr).most_common(3)
来源：http://qhb.ybcxt.top

[U13] Py：固定长度队列
来源：http://for.dianchejie.cn

deque(maxlen=10)
来源：http://cru.aizwys.cn

[U14] Py：分组收集到列表
来源：http://rik.gogol.net.cn

defaultdict(list)
来源：http://eov.jlsjyb.cn

[U15] Py：高精度计时
来源：http://qdf.zdbjq.cn

t = time.perf_counter()
来源：http://ahr.jinqigfzy.top

[U16] Py：命令行参数解析
来源：http://sqm.316326.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qsd.ybcxt.top

[U17] Py：初始化日志
来源：http://tuh.epnwcf.com

logging.basicConfig(level=logging.INFO)
来源：http://vsh.yanxiufei.cn

[U18] Py：预编译正则
来源：http://hpo.epnwcf.com

pat = re.compile(r"\d+")
来源：http://kmx.zhixingplan.top

[U19] Py：正则替换带回调
来源：http://fzx.mhx1999.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hsg.guowangkeji.top

[U20] Py：缓存函数结果
来源：http://hga.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://kyu.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://pgc.shzxlz.cn

@contextlib.contextmanager
来源：http://hmd.yuanzhike.top

[U22] Py：矩阵转置
来源：http://wyj.kuanghao11.cn

list(zip(*m))
来源：http://tgy.shanyushiyangkeji.top

[U23] Py：分块读取大文件
来源：http://qbg.andypj.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xse.sjlbkw.cn

[U24] Py：路径操作
来源：http://wqi.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zgs.yonumen.top

[U25] Py：CSV 按字典读
来源：http://pqv.epnwcf.com

csv.DictReader(f)
来源：http://its.tanke756.top

[U26] Py：并发下载
来源：http://sod.zdbjq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fon.gzhubu.top

[U27] Py：异步 HTTP
来源：http://gwa.ydzc1.top

aiohttp.ClientSession() 配合 async with
来源：http://zxn.guannengcc.top

[U28] Py：类型别名
来源：http://usq.quarkkingdee.top

UserId = int
来源：http://kew.yonumen.top

[U29] Py：属性校验
来源：http://zqw.nanxinkj.top

@property 与 @x.setter 配合
来源：http://yde.cucudq.cn

[U30] Py：数据类
来源：http://fpl.yonumen.top

@dataclass(slots=True)
来源：http://ubt.wangshuangyany.cn

[U31] Py：单测
来源：http://wej.hesvh.cn

python -m pytest -q
来源：http://kvf.fengsongda.top

[U32] Py：代码格式化
来源：http://etx.hammf.cn

ruff format . && ruff check --fix .
来源：http://ozz.hammf.cn

[U33] Py：打包发布
来源：http://vko.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://san.shzxlz.cn

[U34] Py：判断编码
来源：http://vlg.gaohongyu789.top

chardet.detect(raw)
来源：http://ndj.yuxming.cn

[U35] Py：发送邮件
来源：http://vqh.yonumen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vpe.yongpay.top

[U36] Py：定时任务
来源：http://ama.zhiwuduotai.top

schedule.every(10).minutes.do(job)
来源：http://swd.yj20258888.top

[U37] Py：读写 Excel
来源：http://eon.yj20258888.top

pandas.read_excel / DataFrame.to_excel
来源：http://tst.shzxlz.cn

[U38] Py：获取脚本所在目录
来源：http://bep.uphjek.com

Path(__file__).resolve().parent
来源：http://jzf.zdqjudy.top


<!-- 参考信息 -->