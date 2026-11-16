代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://khr.vehdjk.com

[S15] C：类型转换
来源：http://jpx.yj20258888.top

(double) a / b
来源：http://mos.feifeiyinyue.top

[S16] C：位操作置位
来源：http://jeq.hywenlv.cn

x |= (1 << 3);
来源：http://ogp.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://pnv.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hpd.xingfuxueyuan.xyz

[S18] C：命令行参数
来源：http://mje.shuidangran.top

int main(int argc, char **argv)
来源：http://kif.dashuyun.cn

[S19] C：快速排序
来源：http://qyr.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://ish.sysykeji.top

[S20] C：二分查找
来源：http://hpm.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://crz.yvedp.cn

[S21] C：字符类别判断
来源：http://lls.iojbl.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aff.iojbl.cn

[S22] C：字符串转数字
来源：http://ugj.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sxf.vehdjk.com

[S23] C：随机数
来源：http://avg.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://eoj.zhixingplan.top

[S24] C：获取本地时间
来源：http://wtq.jyoumei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gzk.gotoacloud.top

[S25] C：内存拷贝
来源：http://zpe.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://qob.yongpay.top

[S26] C：内存清零
来源：http://kzk.bjfxy.top

memset(a, 0, sizeof a);
来源：http://kxm.daxiang520.top

[S27] C：定义常量
来源：http://cmq.c1oappe.top

const double PI = 3.14159;
来源：http://avt.jlsjyb.cn

[S28] C：静态变量
来源：http://beq.zhijiandao.cn

static int counter = 0;
来源：http://wmz.yongpay.top

[S29] C：变参函数
来源：http://jxa.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xdc.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://iwt.ybcxt.top

#ifndef X_H
来源：http://ghi.jinqigufen.top

#define X_H
来源：http://mqs.zhoulong.xyz

#endif
来源：http://wxu.jqgfzy.top

[S31] C++：Hello World
来源：http://zad.fengsongda.top

#include <iostream>
来源：http://ogr.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://uwe.pycfn.com

[S32] C++：字符串
来源：http://uls.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://bko.316326.xyz

[S33] C++：vector 增删
来源：http://vdi.yueranfly.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://css.hammf.cn

[S34] C++：遍历 vector
来源：http://dnu.xziqi.cn

for (auto &x : v) { std::cout << x; }
来源：http://bat.wangshuangyany.cn

[S35] C++：map
来源：http://zsm.cucudq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jsg.jqgfzy.top

[S36] C++：unordered_map
来源：http://hbb.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xki.dashuyun.cn

[S37] C++：set
来源：http://uwq.hcnkem.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mal.tian-w.cn

[S38] C++：排序
来源：http://dhe.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://aux.yj20258.top

[S39] C++：自定义比较器排序
来源：http://csg.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sej.cheryme.top

[S40] C++：查找元素
来源：http://knl.0kj1m.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bld.redwolf501.top

[S41] C++：类与构造函数
来源：http://hcy.fktsv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://seo.aizwys.cn

[S42] C++：继承与虚函数
来源：http://zpm.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://kbd.xinyue.icu

[S43] C++：智能指针
来源：http://lhz.jianghu66.top

auto p = std::make_unique<int>(5);
来源：http://qub.zhiwuduotai.top

[S44] C++：引用传参
来源：http://hbw.daria6918.cn

void inc(int &x) { ++x; }
来源：http://rln.zycfv.cn

[S45] C++：lambda
来源：http://ruy.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qig.fehbvm.com

[S46] C++：函数模板
来源：http://cyl.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ztr.bjfxy.top

[S47] C++：结构化绑定遍历
来源：http://prm.pycfn.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ofv.aibaodan.cn

[S48] C++：逐行读文件
来源：http://vzr.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://ybq.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://hxp.ydzc1.top

[S49] C++：写文件
来源：http://sgm.jiagoushi.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fxv.dianchejie.cn

[S50] C++：格式化数字
来源：http://ohu.gzhubu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xtd.vqdsnc.cn

[S51] C++：显式类型转换
来源：http://ado.xylfe.cn

static_cast<double>(a) / b
来源：http://mej.aibaodan.cn

[S52] C++：const 与 noexcept
来源：http://wzr.svipenyu.cn

int size() const noexcept { return n_; }
来源：http://niw.tian-w.cn

[S53] C++：移动语义
来源：http://gfk.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://aev.hfpthk.cn

[S54] C++：异常处理
来源：http://zfo.aibaodan.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zzp.wangdashe.top

[S55] C++：结构化绑定
来源：http://ecj.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xym.nanxuanxn.top

[S56] C++：optional
来源：http://mkv.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qbb.hesvh.cn

[S57] C++：编译期常量
来源：http://tjy.svipenyu.cn

constexpr int N = 10;
来源：http://gkg.bbcook.cn

[S58] C++：命名空间
来源：http://umo.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://kmg.jinqigufen.top

[S59] C++：静态断言
来源：http://gar.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vcy.iojbl.cn

[S60] C++：遍历并删除元素
来源：http://izo.xylfe.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://itg.smart0.xyz

================================================================================
来源：http://nty.quarkkingdee.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bzl.yj20258.top

================================================================================
来源：http://mar.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://mxb.shanyushiyangtech.top

println("Hello")
来源：http://jyd.yangfankeji.com

[T02] Kotlin：变量
来源：http://snj.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jsr.wangdashe.top

[T03] Kotlin：字符串模板
来源：http://qwj.andypj.xyz

"值: $b"
来源：http://yvp.dianchejie.cn

[T04] Kotlin：空安全
来源：http://gue.sufxvd.cn

val n: String? = null;  n?.length
来源：http://rtp.svipenyu.cn

[T05] Kotlin：when 表达式
来源：http://vwn.pengpengdd.cyou

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ndk.meibo888.top

[T06] Kotlin：集合映射
来源：http://isy.ehwqpu.com

listOf(1, 2, 3).map { it * 2 }
来源：http://pjd.hnqzz.top

[T07] Kotlin：集合过滤
来源：http://ojz.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xbg.aizwys.cn

[T08] Kotlin：数据类
来源：http://ksb.daria6918.cn

data class User(val name: String, val age: Int)
来源：http://qge.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://rmg.sjlbkw.cn

fun String.exclaim() = this + "!"
来源：http://pfz.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://jhm.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rli.316326.xyz

[T11] Kotlin：协程
来源：http://avt.chenlongwang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nts.yfazqb.com

[T12] Kotlin：解构声明
来源：http://wmi.shzxlz.cn

val (a, b) = Pair(1, 2)
来源：http://oom.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://tnp.svipenyu.cn

val m = mapOf("a" to 1)
来源：http://fqo.epnwcf.com

[T14] Kotlin：循环
来源：http://hyv.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://fis.daria6918.cn

[T15] Kotlin：接口
来源：http://ztx.gzhubu.top

interface Shape { fun area(): Double }
来源：http://axw.yongpay.top

[T16] Swift：Hello World
来源：http://xkt.tianlin.xyz

print("Hello")
来源：http://rog.ppjwa.cn

[T17] Swift：变量与常量
来源：http://wsn.shzxlz.cn

var a = 1;  let b = 2
来源：http://czz.zhijiandao.cn

[T18] Swift：字符串插值
来源：http://ynj.0kj1m.cn

"值: \(b)"
来源：http://lph.sysykeji.top

[T19] Swift：可选绑定
来源：http://sto.gzhubu.top

if let n = opt { print(n) }
来源：http://bhd.fehbvm.com

[T20] Swift：数组操作
来源：http://ttt.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://dle.snrcjt.cn

[T21] Swift：遍历
来源：http://hvx.9152youxi.cn

for x in a { print(x) }
来源：http://qdp.jinqigufen.top

[T22] Swift：字典
来源：http://dzd.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zsj.yonumen.top

[T23] Swift：函数
来源：http://pic.guannengcc.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jls.cheryme.top

[T24] Swift：闭包
来源：http://rnn.dashuyun.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zio.yfazqb.com

[T25] Swift：结构体
来源：http://kxi.jqgufenzy.top

struct P { var x: Int }
来源：http://ynp.chenjidiqi.icu

[T26] Swift：类与重写
来源：http://ecw.ivvv.top

class A: Base { override func f() {} }
来源：http://hpz.fanxiaobao.xyz

[T27] Swift：错误处理
来源：http://nvv.hesvh.cn

do { try f() } catch { print(error) }
来源：http://hbw.birdmap.top

[T28] Swift：枚举
来源：http://hsm.nwbrower.top

enum Color { case red, green }
来源：http://cxj.jinghuilouyu.cn

[T29] Swift：guard 提前返回
来源：http://pmg.gogol.net.cn

guard let x = opt else { return }
来源：http://nxq.gotoacloud.top

[T30] Swift：协议
来源：http://agj.meibo888.top

protocol Shape { func area() -> Double }
来源：http://qtg.yj202588.top

[T31] Lua：Hello World
来源：http://day.zhaomingkeji.xyz

print("Hello")
来源：http://gay.zdqjudy.top

[T32] Lua：局部变量
来源：http://ypr.cheryme.top

local a = 1
来源：http://bhk.9152youxi.cn

[T33] Lua：表（数组）
来源：http://tyi.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://kvj.epnwcf.com

[T34] Lua：遍历表
来源：http://ypv.feifeiyinyue.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zqh.zhongyouzk.top

[T35] Lua：字典表
来源：http://nmr.chenlongwang.top

local d = { a = 1 };  d.b = 2
来源：http://tcz.jinghuilouyu.cn

[T36] Lua：函数
来源：http://owq.ppjwa.cn

function add(a, b) return a + b end
来源：http://ymp.zhiwuduotai.top

[T37] Lua：字符串拼接
来源：http://jja.gotoacloud.top

"a" .. "b"
来源：http://vgi.jinyuanbaomall.cn

[T38] Lua：条件
来源：http://opw.yueranfly.top

if x > 0 then print("正") end
来源：http://tnv.wangdashe.top

[T39] Lua：模式匹配
来源：http://isb.yvedp.cn

string.find(s, "%d+")
来源：http://ygj.gzhubu.top

[T40] Lua：元表
来源：http://yck.kuanghao11.cn

setmetatable({}, { __index = base })
来源：http://tnz.shangyingyoupin.top

[T41] Perl：Hello World
来源：http://pln.sweek.top

print "Hello\n";
来源：http://pps.wangdashe.top

[T42] Perl：变量类型
来源：http://ndh.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ztu.redwolf501.top

[T43] Perl：字符串插值
来源：http://tmm.cdnleiting.top

"值: $a"
来源：http://oyd.bbcook.cn

[T44] Perl：条件
来源：http://wie.cheryme.top

if ($a > 0) { print "正"; }
来源：http://ltc.hcnkem.com

[T45] Perl：数组遍历
来源：http://bgz.haohaochexian.top

for my $x (@arr) { print $x; }
来源：http://rbs.fzhhl.top

[T46] Perl：哈希操作
来源：http://wyg.jiagoushi.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zva.yfazqb.com

[T47] Perl：正则捕获
来源：http://ffd.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://nfr.dashuyun.cn

[T48] Perl：正则替换
来源：http://ffw.jlsjyb.cn

$s =~ s/old/new/g;
来源：http://qej.xinyue.icu

[T49] Perl：函数
来源：http://omc.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aph.nwbrower.top

[T50] Perl：逐行读文件
来源：http://gjg.meibo888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qmp.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://igd.fanxiaobao.xyz

[T51] Scala：Hello World
来源：http://cqz.gogol.net.cn

println("Hello")
来源：http://shu.yangfankeji.com

[T52] Scala：变量
来源：http://mof.cqqwz.cn

val a = 1;  var b = 2
来源：http://tnj.ydjk.org.cn

[T53] Scala：字符串插值
来源：http://xog.tianlin.xyz

s"值: $b"
来源：http://iht.hfpthk.cn

[T54] Scala：集合映射
来源：http://aua.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://ilx.jinqigfzy.top

[T55] Scala：集合过滤
来源：http://jlp.daria6918.cn

List(1, 2, 3).filter(_ > 1)
来源：http://usb.wangshuangyany.cn

[T56] Scala：样例类
来源：http://pku.tian-w.cn

case class User(name: String, age: Int)
来源：http://rjq.vehdjk.com

[T57] Scala：模式匹配
来源：http://hhl.vehdjk.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://jkt.yfazqb.com

[T58] Scala：函数定义
来源：http://dsn.yangfankeji.com

def add(a: Int, b: Int): Int = a + b
来源：http://hrv.yuanzhike.top

[T59] Scala：循环
来源：http://amm.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://qyn.yueranfly.top

[T60] Scala：折叠
来源：http://wsr.zdbjq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://erk.jinqigfzy.top

================================================================================
来源：http://edm.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qgd.sufxvd.cn

================================================================================
来源：http://apm.sysykeji.top

[U01] Py：创建虚拟环境
来源：http://gtf.nwbrower.top

python -m venv .venv && source .venv/bin/activate
来源：http://ebi.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://two.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kfj.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://cpa.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://szl.cdnleiting.top

[U04] Py：变量调试打印
来源：http://eea.ctjpmb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jzu.xuanzx.com

[U05] Py：列表去重且保序
来源：http://uva.yonumen.top

list(dict.fromkeys(arr))
来源：http://ibp.hfpthk.cn

[U06] Py：合并两个字典
来源：http://dzl.dianchejie.cn

{**a, **b}
来源：http://wrh.zhaomingkeji.xyz

[U07] Py：反转字典键值
来源：http://skr.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://vmi.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://wua.tarul.cn

[y for x in nested for y in x]
来源：http://jjp.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://xgv.yfazqb.com

max(d, key=d.get)
来源：http://qnb.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://pel.316326.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xmr.hywenlv.cn

[U11] Py：生成器表达式
来源：http://dys.ivvv.top

(x * 2 for x in arr)
来源：http://kbq.feifeiyinyue.top

[U12] Py：取出现最多的 3 个元素
来源：http://hus.cucudq.cn

Counter(arr).most_common(3)
来源：http://gzz.dianchejie.cn

[U13] Py：固定长度队列
来源：http://chc.ydzc1.top

deque(maxlen=10)
来源：http://ebv.andypj.xyz

[U14] Py：分组收集到列表
来源：http://agy.pengpengdd.cyou

defaultdict(list)
来源：http://lrt.zhiwuduotai.top

[U15] Py：高精度计时
来源：http://zwp.hywenlv.cn

t = time.perf_counter()
来源：http://wfc.yj20258888.top

[U16] Py：命令行参数解析
来源：http://koo.fanxiaobao.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hgh.pycfn.com

[U17] Py：初始化日志
来源：http://kif.ydjk.org.cn

logging.basicConfig(level=logging.INFO)
来源：http://hpn.zhixingplan.top

[U18] Py：预编译正则
来源：http://wwe.daxiang520.top

pat = re.compile(r"\d+")
来源：http://ocg.fktsv.cn

[U19] Py：正则替换带回调
来源：http://skm.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zow.nanxuanxn.top

[U20] Py：缓存函数结果
来源：http://aon.sxryk.cn

@functools.lru_cache(maxsize=None)
来源：http://acc.pengpengdd.cyou

[U21] Py：自定义上下文管理器
来源：http://lgk.zdqjudy.top

@contextlib.contextmanager
来源：http://wnr.andypj.xyz

[U22] Py：矩阵转置
来源：http://wub.wangshuangyany.cn

list(zip(*m))
来源：http://pcw.wangdashe.top

[U23] Py：分块读取大文件
来源：http://deu.gotoacloud.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ywq.yj20258.top

[U24] Py：路径操作
来源：http://juy.nanxuanxn.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nnu.xinyue.icu

[U25] Py：CSV 按字典读
来源：http://wil.svipenyu.cn

csv.DictReader(f)
来源：http://oyu.yonumen.top

[U26] Py：并发下载
来源：http://gfc.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fcn.yuanzhike.top

[U27] Py：异步 HTTP
来源：http://lsk.0kj1m.cn

aiohttp.ClientSession() 配合 async with
来源：http://wqp.gotoacloud.top

[U28] Py：类型别名
来源：http://xgb.tianlin.xyz

UserId = int
来源：http://wul.gotoacloud.top

[U29] Py：属性校验
来源：http://blz.shangyingyoupin.top

@property 与 @x.setter 配合
来源：http://osz.xuanzx.com

[U30] Py：数据类
来源：http://ydo.yanxiufei.cn

@dataclass(slots=True)
来源：http://jnd.yj202588.top

[U31] Py：单测
来源：http://vam.nanxuanxn.top

python -m pytest -q
来源：http://hxm.guowangkeji.top

[U32] Py：代码格式化
来源：http://skf.wangdashe.top

ruff format . && ruff check --fix .
来源：http://qif.yfazqb.com

[U33] Py：打包发布
来源：http://pcn.hnxiangtu.top

python -m build  （依赖 pyproject.toml）
来源：http://ylc.uphjek.com

[U34] Py：判断编码
来源：http://rzj.gzhubu.top

chardet.detect(raw)
来源：http://ddw.xinyue.icu

[U35] Py：发送邮件
来源：http://omh.jinghuilouyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rdp.tanke756.top

[U36] Py：定时任务
来源：http://qrb.pengpengdd.cyou

schedule.every(10).minutes.do(job)
来源：http://vag.xylfe.cn

[U37] Py：读写 Excel
来源：http://wgr.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ddr.tarul.cn

[U38] Py：获取脚本所在目录
来源：http://liv.nwbrower.top

Path(__file__).resolve().parent
来源：http://wue.316326.xyz


<!-- 参考信息 -->