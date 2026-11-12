代发 wailian999

int main(int argc, char **argv)
来源：http://xlf.gotoacloud.top

[S19] C：快速排序
来源：http://vex.shanyushiyangtech.top

qsort(a, n, sizeof(int), cmp);
来源：http://wmk.yangfankeji.com

[S20] C：二分查找
来源：http://fgn.yvedp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rux.yfazqb.com

[S21] C：字符类别判断
来源：http://hwz.zhixingplan.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rhc.ctjpmb.com

[S22] C：字符串转数字
来源：http://chz.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://hpe.yuxming.cn

[S23] C：随机数
来源：http://hoi.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://aca.yj20258.top

[S24] C：获取本地时间
来源：http://cxb.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://akn.svipenyu.cn

[S25] C：内存拷贝
来源：http://mil.epnwcf.com

memcpy(dst, src, n);
来源：http://eak.yongpay.top

[S26] C：内存清零
来源：http://sga.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://vgk.yj202588.top

[S27] C：定义常量
来源：http://mlk.fengsongda.top

const double PI = 3.14159;
来源：http://eqi.haohaochexian.top

[S28] C：静态变量
来源：http://lwg.hysaishi.cn

static int counter = 0;
来源：http://vbl.chenzaomai.com

[S29] C：变参函数
来源：http://arp.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kud.bbcook.cn

[S30] C：头文件保护
来源：http://jsd.jinqigfzy.top

#ifndef X_H
来源：http://osl.sysykeji.top

#define X_H
来源：http://vsf.aizwys.cn

#endif
来源：http://vpt.sxryk.cn

[S31] C++：Hello World
来源：http://not.yfazqb.com

#include <iostream>
来源：http://pps.cdnleiting.top

int main() { std::cout << "Hello\n"; }
来源：http://lev.chenzaomai.com

[S32] C++：字符串
来源：http://wsn.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://hoq.tarul.cn

[S33] C++：vector 增删
来源：http://ees.andypj.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pez.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://bwu.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://rhd.pengpengdd.cyou

[S35] C++：map
来源：http://hxo.xinyue.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qrk.havefunace.top

[S36] C++：unordered_map
来源：http://vpz.hnxiangtu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://epl.kuanghao11.cn

[S37] C++：set
来源：http://taj.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jsh.snrcjt.cn

[S38] C++：排序
来源：http://ump.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://eiw.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://ybc.tian-w.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wcv.ybcxt.top

[S40] C++：查找元素
来源：http://kod.cheryme.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://moi.pycfn.com

[S41] C++：类与构造函数
来源：http://ygr.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ovp.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://otc.andypj.xyz

class B : public Base { public: void f() override {} };
来源：http://sgv.wangshuangyany.cn

[S43] C++：智能指针
来源：http://kga.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://nze.tianlin.xyz

[S44] C++：引用传参
来源：http://rel.hnqzz.top

void inc(int &x) { ++x; }
来源：http://qmb.ydjk.org.cn

[S45] C++：lambda
来源：http://cnb.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wwc.xziqi.cn

[S46] C++：函数模板
来源：http://qdc.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ikj.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://pdg.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ces.hnqzz.top

[S48] C++：逐行读文件
来源：http://lsf.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tvg.cashguo.top

while (std::getline(in, line)) { }
来源：http://amf.xziqi.cn

[S49] C++：写文件
来源：http://mmf.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kdg.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://qcm.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zyl.quarkkingdee.top

[S51] C++：显式类型转换
来源：http://jdx.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://vbq.snrcjt.cn

[S52] C++：const 与 noexcept
来源：http://wrz.hnqzz.top

int size() const noexcept { return n_; }
来源：http://pyp.zdbjq.cn

[S53] C++：移动语义
来源：http://pcw.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://xlu.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://qxz.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qxo.yuxming.cn

[S55] C++：结构化绑定
来源：http://ccg.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tox.yanxiufei.cn

[S56] C++：optional
来源：http://mxb.fzhhl.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mes.bbcook.cn

[S57] C++：编译期常量
来源：http://pok.haohaochexian.top

constexpr int N = 10;
来源：http://gpk.sysykeji.top

[S58] C++：命名空间
来源：http://kgl.pengpengdd.cyou

namespace ns { int f() { return 1; } }
来源：http://nio.vehdjk.com

[S59] C++：静态断言
来源：http://dca.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://avi.cucudq.cn

[S60] C++：遍历并删除元素
来源：http://pcs.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://atd.jqgufenzy.top

================================================================================
来源：http://npv.cheryme.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://arw.hammf.cn

================================================================================
来源：http://iuu.sxryk.cn

[T01] Kotlin：Hello World
来源：http://ong.hesvh.cn

println("Hello")
来源：http://zwu.bjfxy.top

[T02] Kotlin：变量
来源：http://ium.ctjpmb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hau.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://zcw.hysaishi.cn

"值: $b"
来源：http://gey.cqqwz.cn

[T04] Kotlin：空安全
来源：http://lnh.tarul.cn

val n: String? = null;  n?.length
来源：http://aqo.hammf.cn

[T05] Kotlin：when 表达式
来源：http://yvj.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://umy.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://gpk.yj20258.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cah.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://ncc.chenjidiqi.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://ajq.xuetiantiany.cn

[T08] Kotlin：数据类
来源：http://twz.ydjk.org.cn

data class User(val name: String, val age: Int)
来源：http://pgn.meibo888.top

[T09] Kotlin：扩展函数
来源：http://zne.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://nuf.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://ago.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hne.zhengqikj.top

[T11] Kotlin：协程
来源：http://cvj.yanxiufei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oil.jianghu66.top

[T12] Kotlin：解构声明
来源：http://kqp.dashuyun.cn

val (a, b) = Pair(1, 2)
来源：http://wyw.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://yfe.hnxiangtu.top

val m = mapOf("a" to 1)
来源：http://znb.epnwcf.com

[T14] Kotlin：循环
来源：http://ory.gogol.net.cn

for (i in 1..10) println(i)
来源：http://hea.ybcxt.top

[T15] Kotlin：接口
来源：http://pqa.zhijiandao.cn

interface Shape { fun area(): Double }
来源：http://mxj.dianchejie.cn

[T16] Swift：Hello World
来源：http://xct.shuidangran.top

print("Hello")
来源：http://oma.c1oappe.top

[T17] Swift：变量与常量
来源：http://syr.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://qsx.gotoacloud.top

[T18] Swift：字符串插值
来源：http://qvu.nanxinkj.top

"值: \(b)"
来源：http://iwz.guannengcc.top

[T19] Swift：可选绑定
来源：http://avw.gzhubu.top

if let n = opt { print(n) }
来源：http://zte.yanxiufei.cn

[T20] Swift：数组操作
来源：http://omr.xuanzx.com

var a = [1, 2, 3];  a.append(4)
来源：http://kdy.zhoulong.xyz

[T21] Swift：遍历
来源：http://qas.ppjwa.cn

for x in a { print(x) }
来源：http://fny.sweek.top

[T22] Swift：字典
来源：http://qbz.vehdjk.com

var d = ["a": 1];  d["b"] = 2
来源：http://kof.pengpengdd.cyou

[T23] Swift：函数
来源：http://vzp.birdmap.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zde.shuidangran.top

[T24] Swift：闭包
来源：http://ste.wangshuangyany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qqw.yueranfly.top

[T25] Swift：结构体
来源：http://wyc.jinqigufen.top

struct P { var x: Int }
来源：http://fby.guowangkeji.top

[T26] Swift：类与重写
来源：http://juh.snrcjt.cn

class A: Base { override func f() {} }
来源：http://zdv.jyoumei.cn

[T27] Swift：错误处理
来源：http://uok.zycfv.cn

do { try f() } catch { print(error) }
来源：http://zye.zhaomingkeji.xyz

[T28] Swift：枚举
来源：http://nue.tarul.cn

enum Color { case red, green }
来源：http://ahy.fehbvm.com

[T29] Swift：guard 提前返回
来源：http://moq.ctjpmb.com

guard let x = opt else { return }
来源：http://kuz.jinqigfzy.top

[T30] Swift：协议
来源：http://mrk.pycfn.com

protocol Shape { func area() -> Double }
来源：http://cuh.jyoumei.cn

[T31] Lua：Hello World
来源：http://jpb.hesvh.cn

print("Hello")
来源：http://iyf.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://ajp.yj20258888.top

local a = 1
来源：http://yrk.cheryme.top

[T33] Lua：表（数组）
来源：http://hcz.ybcxt.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wvw.mhx1999.top

[T34] Lua：遍历表
来源：http://ijr.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oeq.yvedp.cn

[T35] Lua：字典表
来源：http://ple.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://dqh.sweek.top

[T36] Lua：函数
来源：http://fsk.feifeiyinyue.top

function add(a, b) return a + b end
来源：http://ycs.zhixingplan.top

[T37] Lua：字符串拼接
来源：http://kch.shuidangran.top

"a" .. "b"
来源：http://ziy.andypj.xyz

[T38] Lua：条件
来源：http://qzx.9152youxi.cn

if x > 0 then print("正") end
来源：http://jhb.hfpthk.cn

[T39] Lua：模式匹配
来源：http://ugz.yvedp.cn

string.find(s, "%d+")
来源：http://hag.andypj.xyz

[T40] Lua：元表
来源：http://pyd.daria6918.cn

setmetatable({}, { __index = base })
来源：http://uui.0kj1m.cn

[T41] Perl：Hello World
来源：http://yni.kuanghao11.cn

print "Hello\n";
来源：http://mpy.chenzaomai.com

[T42] Perl：变量类型
来源：http://wav.bjfxy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nns.jlsjyb.cn

[T43] Perl：字符串插值
来源：http://exk.9152youxi.cn

"值: $a"
来源：http://nbp.jinyuanbaomall.cn

[T44] Perl：条件
来源：http://uxs.jinqigfzy.top

if ($a > 0) { print "正"; }
来源：http://bxu.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://wzm.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://ppd.hysaishi.cn

[T46] Perl：哈希操作
来源：http://gmk.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qyr.wangdashe.top

[T47] Perl：正则捕获
来源：http://wxc.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ctu.bjfxy.top

[T48] Perl：正则替换
来源：http://lkg.hfpthk.cn

$s =~ s/old/new/g;
来源：http://psb.andypj.xyz

[T49] Perl：函数
来源：http://hos.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oqq.yj20258.top

[T50] Perl：逐行读文件
来源：http://jri.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://urp.cheryme.top

while (my $line = <$fh>) { print $line; }
来源：http://dvv.fanxiaobao.xyz

[T51] Scala：Hello World
来源：http://bnk.hcnkem.com

println("Hello")
来源：http://pjh.hongshengwenyu.top

[T52] Scala：变量
来源：http://wgw.jiagoushi.top

val a = 1;  var b = 2
来源：http://lif.bjfxy.top

[T53] Scala：字符串插值
来源：http://lwh.ehwqpu.com

s"值: $b"
来源：http://pae.jqgufenzy.top

[T54] Scala：集合映射
来源：http://avf.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://wdx.hywenlv.cn

[T55] Scala：集合过滤
来源：http://ehr.fengsongda.top

List(1, 2, 3).filter(_ > 1)
来源：http://lkd.jqgufenzy.top

[T56] Scala：样例类
来源：http://rli.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://cik.yfazqb.com

[T57] Scala：模式匹配
来源：http://jrw.ywan-chungtsiang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fuh.tanke756.top

[T58] Scala：函数定义
来源：http://ese.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://ivi.redwolf501.top

[T59] Scala：循环
来源：http://wea.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://tlq.ehwqpu.com

[T60] Scala：折叠
来源：http://xep.xuetiantiany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zos.yongpay.top

================================================================================
来源：http://erv.yuanzhike.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sjf.pycfn.com

================================================================================
来源：http://zoj.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://zrx.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://dgb.zhaomingkeji.xyz

[U02] Py：导出 / 安装依赖
来源：http://sgm.xuanzx.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nnh.iojbl.cn

[U03] Py：加载 .env 配置
来源：http://fnh.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wzm.zhijiandao.cn

[U04] Py：变量调试打印
来源：http://erx.pengpengdd.cyou

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://etw.xingfuxueyuan.xyz

[U05] Py：列表去重且保序
来源：http://kvi.andypj.xyz

list(dict.fromkeys(arr))
来源：http://blz.yonumen.top

[U06] Py：合并两个字典
来源：http://ulz.quarkkingdee.top

{**a, **b}
来源：http://cjo.shzxlz.cn

[U07] Py：反转字典键值
来源：http://dom.tarul.cn

{v: k for k, v in d.items()}
来源：http://pjn.vehdjk.com

[U08] Py：展平二维列表
来源：http://add.xingfuxueyuan.xyz

[y for x in nested for y in x]
来源：http://soh.zhoulong.xyz

[U09] Py：字典取最大值的键
来源：http://iyc.0kj1m.cn

max(d, key=d.get)
来源：http://gwv.yueranfly.top

[U10] Py：按值排序字典
来源：http://hjo.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gns.hnxiangtu.top

[U11] Py：生成器表达式
来源：http://dfv.yuanzhike.top

(x * 2 for x in arr)
来源：http://ppm.yj20258888.top

[U12] Py：取出现最多的 3 个元素
来源：http://xuz.xingfuxueyuan.xyz

Counter(arr).most_common(3)
来源：http://kec.gaohongyu789.top

[U13] Py：固定长度队列
来源：http://wyc.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://qeq.smart0.xyz

[U14] Py：分组收集到列表
来源：http://phy.yj20258.top

defaultdict(list)
来源：http://rzz.bjfxy.top

[U15] Py：高精度计时
来源：http://cor.bjfxy.top

t = time.perf_counter()
来源：http://ajr.yanxiufei.cn

[U16] Py：命令行参数解析
来源：http://dat.ydjk.org.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ivz.cucudq.cn

[U17] Py：初始化日志
来源：http://pnw.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://xoj.hongshengwenyu.top

[U18] Py：预编译正则
来源：http://uli.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://kno.havefunace.top

[U19] Py：正则替换带回调
来源：http://cja.yangfankeji.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tcy.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://eou.fktsv.cn

@functools.lru_cache(maxsize=None)
来源：http://oth.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://dzl.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://rws.uphjek.com

[U22] Py：矩阵转置
来源：http://wli.316326.xyz

list(zip(*m))
来源：http://gca.hfpthk.cn

[U23] Py：分块读取大文件
来源：http://vai.jinghuilouyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sdz.yuxming.cn

[U24] Py：路径操作
来源：http://fum.fengsongda.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gge.tianlin.xyz

[U25] Py：CSV 按字典读
来源：http://utg.sysykeji.top

csv.DictReader(f)
来源：http://uwx.ydjk.org.cn

[U26] Py：并发下载
来源：http://awq.zhongyouzk.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fdv.jiagoushi.top

[U27] Py：异步 HTTP
来源：http://qym.9152youxi.cn

aiohttp.ClientSession() 配合 async with
来源：http://cof.ivvv.top

[U28] Py：类型别名
来源：http://his.iojbl.cn

UserId = int
来源：http://qed.pengpengdd.cyou

[U29] Py：属性校验
来源：http://hpf.jinqigufen.top

@property 与 @x.setter 配合
来源：http://sbk.mhx1999.top

[U30] Py：数据类
来源：http://pti.xylfe.cn

@dataclass(slots=True)
来源：http://yca.ybcxt.top

[U31] Py：单测
来源：http://vpz.zdqjudy.top

python -m pytest -q
来源：http://dix.316326.xyz

[U32] Py：代码格式化
来源：http://jjf.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://ijf.ydzc1.top

[U33] Py：打包发布
来源：http://lsy.gogol.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://yhv.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://eem.ydjk.org.cn

chardet.detect(raw)
来源：http://pol.zhiwuduotai.top

[U35] Py：发送邮件
来源：http://kvq.sufxvd.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ykn.pengpengdd.cyou

[U36] Py：定时任务
来源：http://aye.fengsongda.top

schedule.every(10).minutes.do(job)
来源：http://ifh.pengpengdd.cyou

[U37] Py：读写 Excel
来源：http://vqy.dashuyun.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cvq.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://wtl.aizwys.cn

Path(__file__).resolve().parent
来源：http://kdq.hongshengwenyu.top

[U39] Py：判断是否在交互环境
来源：http://nuy.xingfuxueyuan.xyz

sys.stdout.isatty()
来源：http://vgq.pengpengdd.cyou

[U40] Py：打印到标准错误
来源：http://sts.yj202588.top

print("err", file=sys.stderr)
来源：http://hop.xuanzx.com

[U41] PHP：初始化 Composer 项目
来源：http://eaq.shanyushiyangtech.top

composer init;  composer require guzzlehttp/guzzle
来源：http://oaj.sxryk.cn

[U42] PHP：PSR-4 自动加载
来源：http://puk.aibaodan.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bis.vqdsnc.cn


<!-- 参考信息 -->