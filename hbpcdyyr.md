代发 wailian999

x |= (1 << 3);
来源：http://atb.xuanzx.com

[S17] C：安全拼接字符串
来源：http://wol.feifeiyinyue.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fun.tanke756.top

[S18] C：命令行参数
来源：http://gzw.cdnleiting.top

int main(int argc, char **argv)
来源：http://cya.zhiwuduotai.top

[S19] C：快速排序
来源：http://ueh.fktsv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ecq.jlsjyb.cn

[S20] C：二分查找
来源：http://och.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ocg.yuxming.cn

[S21] C：字符类别判断
来源：http://gpt.hfpthk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zjg.yj20258.top

[S22] C：字符串转数字
来源：http://avu.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://dbl.hnxiangtu.top

[S23] C：随机数
来源：http://xbg.fehbvm.com

srand(time(NULL));  int r = rand() % 100;
来源：http://orw.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://ldz.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://abb.hfpthk.cn

[S25] C：内存拷贝
来源：http://ydx.yj20258888.top

memcpy(dst, src, n);
来源：http://mkg.gotoacloud.top

[S26] C：内存清零
来源：http://fod.epnwcf.com

memset(a, 0, sizeof a);
来源：http://cmu.gogol.net.cn

[S27] C：定义常量
来源：http://apu.tanke756.top

const double PI = 3.14159;
来源：http://nzy.xuanzx.com

[S28] C：静态变量
来源：http://drs.fehbvm.com

static int counter = 0;
来源：http://yvz.chenlongwang.top

[S29] C：变参函数
来源：http://ejt.hammf.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ceq.yanxiufei.cn

[S30] C：头文件保护
来源：http://fbc.wangdashe.top

#ifndef X_H
来源：http://vdq.guannengcc.top

#define X_H
来源：http://enf.ydjk.org.cn

#endif
来源：http://ato.hywenlv.cn

[S31] C++：Hello World
来源：http://vgi.ydjk.org.cn

#include <iostream>
来源：http://ktn.yuxming.cn

int main() { std::cout << "Hello\n"; }
来源：http://aeu.epnwcf.com

[S32] C++：字符串
来源：http://ojo.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://pgs.52xcode.cn

[S33] C++：vector 增删
来源：http://mue.yanxiufei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pmk.fanxiaobao.xyz

[S34] C++：遍历 vector
来源：http://ovf.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://rih.sweek.top

[S35] C++：map
来源：http://nfi.yj202588.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://scn.chenzaomai.com

[S36] C++：unordered_map
来源：http://ppv.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iha.smart0.xyz

[S37] C++：set
来源：http://wss.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lwp.daxiang520.top

[S38] C++：排序
来源：http://nfb.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://eky.aibaodan.cn

[S39] C++：自定义比较器排序
来源：http://ela.hesvh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pdq.jyoumei.cn

[S40] C++：查找元素
来源：http://etq.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zoa.haohaochexian.top

[S41] C++：类与构造函数
来源：http://aib.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tny.svipenyu.cn

[S42] C++：继承与虚函数
来源：http://gwe.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://pqh.daxiang520.top

[S43] C++：智能指针
来源：http://ojd.guowangkeji.top

auto p = std::make_unique<int>(5);
来源：http://nid.hammf.cn

[S44] C++：引用传参
来源：http://aej.hongshengwenyu.top

void inc(int &x) { ++x; }
来源：http://dlx.fzhhl.top

[S45] C++：lambda
来源：http://ndy.yonumen.top

auto add = [](int a, int b) { return a + b; };
来源：http://ifz.shzxlz.cn

[S46] C++：函数模板
来源：http://pse.haohaochexian.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kpw.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://gdk.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vjv.hammf.cn

[S48] C++：逐行读文件
来源：http://ybe.iojbl.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wym.shuidangran.top

while (std::getline(in, line)) { }
来源：http://kxn.iojbl.cn

[S49] C++：写文件
来源：http://xhh.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://huo.tarul.cn

[S50] C++：格式化数字
来源：http://sjy.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gne.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://tzg.gotoacloud.top

static_cast<double>(a) / b
来源：http://ben.meibo888.top

[S52] C++：const 与 noexcept
来源：http://eto.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://kih.zhiwuduotai.top

[S53] C++：移动语义
来源：http://oyu.yuanzhike.top

std::vector<int> w = std::move(v);
来源：http://dhu.wangdashe.top

[S54] C++：异常处理
来源：http://woa.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ean.iojbl.cn

[S55] C++：结构化绑定
来源：http://mbt.aibaodan.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gfe.hcnkem.com

[S56] C++：optional
来源：http://kcf.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xsh.yj20258.top

[S57] C++：编译期常量
来源：http://pqn.xziqi.cn

constexpr int N = 10;
来源：http://iwv.ydjk.org.cn

[S58] C++：命名空间
来源：http://ssa.yvedp.cn

namespace ns { int f() { return 1; } }
来源：http://esf.fehbvm.com

[S59] C++：静态断言
来源：http://pow.zhixingplan.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ivd.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://sra.9152youxi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zst.fanxiaobao.xyz

================================================================================
来源：http://uop.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://epd.daxiang520.top

================================================================================
来源：http://kaa.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://vxd.yongpay.top

println("Hello")
来源：http://qrs.shzxlz.cn

[T02] Kotlin：变量
来源：http://egb.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nly.vqdsnc.cn

[T03] Kotlin：字符串模板
来源：http://dte.wangdashe.top

"值: $b"
来源：http://sok.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://qli.svipenyu.cn

val n: String? = null;  n?.length
来源：http://xii.bbcook.cn

[T05] Kotlin：when 表达式
来源：http://qxo.meibo888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ehw.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://awn.wangdashe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cdo.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://tst.chenjidiqi.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://eye.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://yqy.zhixingplan.top

data class User(val name: String, val age: Int)
来源：http://jdq.nwbrower.top

[T09] Kotlin：扩展函数
来源：http://bvx.havefunace.top

fun String.exclaim() = this + "!"
来源：http://ecc.jlsjyb.cn

[T10] Kotlin：默认参数
来源：http://afu.yueranfly.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vsc.ehwqpu.com

[T11] Kotlin：协程
来源：http://dcq.sxryk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jvp.zhoulong.xyz

[T12] Kotlin：解构声明
来源：http://fja.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://kwj.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://xoh.uphjek.com

val m = mapOf("a" to 1)
来源：http://pfa.havefunace.top

[T14] Kotlin：循环
来源：http://daq.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://bqz.yangfankeji.com

[T15] Kotlin：接口
来源：http://wfa.cqqwz.cn

interface Shape { fun area(): Double }
来源：http://sce.uphjek.com

[T16] Swift：Hello World
来源：http://dym.9152youxi.cn

print("Hello")
来源：http://dln.haohaochexian.top

[T17] Swift：变量与常量
来源：http://tyw.havefunace.top

var a = 1;  let b = 2
来源：http://vxq.dianchejie.cn

[T18] Swift：字符串插值
来源：http://edf.wangshuangyany.cn

"值: \(b)"
来源：http://tgs.fengsongda.top

[T19] Swift：可选绑定
来源：http://cwi.guowangkeji.top

if let n = opt { print(n) }
来源：http://gyi.haohaochexian.top

[T20] Swift：数组操作
来源：http://gol.dashuyun.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qri.daria6918.cn

[T21] Swift：遍历
来源：http://jdd.tian-w.cn

for x in a { print(x) }
来源：http://wyf.xinyue.icu

[T22] Swift：字典
来源：http://tkk.sweek.top

var d = ["a": 1];  d["b"] = 2
来源：http://igz.vehdjk.com

[T23] Swift：函数
来源：http://nym.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xbr.vqdsnc.cn

[T24] Swift：闭包
来源：http://vzd.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jcr.52xcode.cn

[T25] Swift：结构体
来源：http://urg.tarul.cn

struct P { var x: Int }
来源：http://glw.guowangkeji.top

[T26] Swift：类与重写
来源：http://ubf.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://err.guowangkeji.top

[T27] Swift：错误处理
来源：http://yzg.tarul.cn

do { try f() } catch { print(error) }
来源：http://jkh.redwolf501.top

[T28] Swift：枚举
来源：http://oqx.52xcode.cn

enum Color { case red, green }
来源：http://uck.gaohongyu789.top

[T29] Swift：guard 提前返回
来源：http://klh.feifeiyinyue.top

guard let x = opt else { return }
来源：http://ydz.jinqigfzy.top

[T30] Swift：协议
来源：http://bmv.zhaomingkeji.xyz

protocol Shape { func area() -> Double }
来源：http://vod.chenlongwang.top

[T31] Lua：Hello World
来源：http://rao.jyoumei.cn

print("Hello")
来源：http://avo.ehwqpu.com

[T32] Lua：局部变量
来源：http://shy.nanxuanxn.top

local a = 1
来源：http://dii.yongpay.top

[T33] Lua：表（数组）
来源：http://dzu.pycfn.com

local t = {1, 2, 3};  t[4] = 4
来源：http://iaz.aizwys.cn

[T34] Lua：遍历表
来源：http://emm.tianlin.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://dyz.yvedp.cn

[T35] Lua：字典表
来源：http://evy.52xcode.cn

local d = { a = 1 };  d.b = 2
来源：http://cjv.smart0.xyz

[T36] Lua：函数
来源：http://lut.zhoulong.xyz

function add(a, b) return a + b end
来源：http://uok.jlsjyb.cn

[T37] Lua：字符串拼接
来源：http://mxa.yongpay.top

"a" .. "b"
来源：http://pet.zhijiandao.cn

[T38] Lua：条件
来源：http://qzk.fehbvm.com

if x > 0 then print("正") end
来源：http://szv.xziqi.cn

[T39] Lua：模式匹配
来源：http://fqo.jinqigufen.top

string.find(s, "%d+")
来源：http://fsu.sxryk.cn

[T40] Lua：元表
来源：http://idb.zhixingplan.top

setmetatable({}, { __index = base })
来源：http://lvz.sufxvd.cn

[T41] Perl：Hello World
来源：http://yxn.jinqigufen.top

print "Hello\n";
来源：http://qzb.shuidangran.top

[T42] Perl：变量类型
来源：http://vsc.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nnw.c1oappe.top

[T43] Perl：字符串插值
来源：http://ekn.gotoacloud.top

"值: $a"
来源：http://ufq.jlsjyb.cn

[T44] Perl：条件
来源：http://yxz.quarkkingdee.top

if ($a > 0) { print "正"; }
来源：http://gho.svipenyu.cn

[T45] Perl：数组遍历
来源：http://tkd.quarkkingdee.top

for my $x (@arr) { print $x; }
来源：http://tyq.fktsv.cn

[T46] Perl：哈希操作
来源：http://uyb.redwolf501.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ssb.pycfn.com

[T47] Perl：正则捕获
来源：http://mee.hesvh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nam.zhoulong.xyz

[T48] Perl：正则替换
来源：http://ziy.uphjek.com

$s =~ s/old/new/g;
来源：http://dew.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://zgd.vqdsnc.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rjx.jiagoushi.top

[T50] Perl：逐行读文件
来源：http://sbe.dianchejie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vwy.bbcook.cn

while (my $line = <$fh>) { print $line; }
来源：http://bjg.hnxiangtu.top

[T51] Scala：Hello World
来源：http://suq.birdmap.top

println("Hello")
来源：http://pdl.epnwcf.com

[T52] Scala：变量
来源：http://hza.fktsv.cn

val a = 1;  var b = 2
来源：http://dou.wangdashe.top

[T53] Scala：字符串插值
来源：http://vei.gzhubu.top

s"值: $b"
来源：http://ryj.zhixingplan.top

[T54] Scala：集合映射
来源：http://hto.zhaomingkeji.xyz

List(1, 2, 3).map(_ * 2)
来源：http://imv.jianghu66.top

[T55] Scala：集合过滤
来源：http://zyk.daria6918.cn

List(1, 2, 3).filter(_ > 1)
来源：http://usk.mhx1999.top

[T56] Scala：样例类
来源：http://dss.hnqzz.top

case class User(name: String, age: Int)
来源：http://yrn.daxiang520.top

[T57] Scala：模式匹配
来源：http://xaf.tanke756.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lyr.sufxvd.cn

[T58] Scala：函数定义
来源：http://cus.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://bkt.hywenlv.cn

[T59] Scala：循环
来源：http://nuf.guannengcc.top

for (i <- 1 to 10) println(i)
来源：http://asg.hcnkem.com

[T60] Scala：折叠
来源：http://vnr.yangfankeji.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mvt.dianchejie.cn

================================================================================
来源：http://lkv.tarul.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hbe.zhongyouzk.top

================================================================================
来源：http://gyd.guowangkeji.top

[U01] Py：创建虚拟环境
来源：http://jjk.redwolf501.top

python -m venv .venv && source .venv/bin/activate
来源：http://boj.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://zir.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://msx.cashguo.top

[U03] Py：加载 .env 配置
来源：http://sca.redwolf501.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fpw.gaohongyu789.top

[U04] Py：变量调试打印
来源：http://yfo.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mbl.zycfv.cn

[U05] Py：列表去重且保序
来源：http://aci.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://alo.nanxinkj.top

[U06] Py：合并两个字典
来源：http://uyu.snrcjt.cn

{**a, **b}
来源：http://tid.zhengqikj.top

[U07] Py：反转字典键值
来源：http://tgh.cqqwz.cn

{v: k for k, v in d.items()}
来源：http://xun.ywan-chungtsiang.top

[U08] Py：展平二维列表
来源：http://vzn.hfpthk.cn

[y for x in nested for y in x]
来源：http://iya.jiagoushi.top

[U09] Py：字典取最大值的键
来源：http://xni.pycfn.com

max(d, key=d.get)
来源：http://lrl.yueranfly.top

[U10] Py：按值排序字典
来源：http://rzv.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vnh.havefunace.top

[U11] Py：生成器表达式
来源：http://ncj.cashguo.top

(x * 2 for x in arr)
来源：http://wgz.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://nox.fanxiaobao.xyz

Counter(arr).most_common(3)
来源：http://sws.zhengqikj.top

[U13] Py：固定长度队列
来源：http://fii.fengsongda.top

deque(maxlen=10)
来源：http://tqn.daxiang520.top

[U14] Py：分组收集到列表
来源：http://czk.zhengqikj.top

defaultdict(list)
来源：http://coy.zhengqikj.top

[U15] Py：高精度计时
来源：http://odp.zhengqikj.top

t = time.perf_counter()
来源：http://kqv.yonumen.top

[U16] Py：命令行参数解析
来源：http://yjb.bjfxy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oto.zhoulong.xyz

[U17] Py：初始化日志
来源：http://yrd.cashguo.top

logging.basicConfig(level=logging.INFO)
来源：http://uwz.hnxiangtu.top

[U18] Py：预编译正则
来源：http://zzr.yangfankeji.com

pat = re.compile(r"\d+")
来源：http://epf.shanyushiyangtech.top

[U19] Py：正则替换带回调
来源：http://bod.yj202588.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://msm.ppjwa.cn

[U20] Py：缓存函数结果
来源：http://jmy.xziqi.cn

@functools.lru_cache(maxsize=None)
来源：http://rpq.wangdashe.top

[U21] Py：自定义上下文管理器
来源：http://esj.andypj.xyz

@contextlib.contextmanager
来源：http://qhy.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://ooc.havefunace.top

list(zip(*m))
来源：http://zis.tianlin.xyz

[U23] Py：分块读取大文件
来源：http://fcd.bbcook.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://plo.wangdashe.top

[U24] Py：路径操作
来源：http://slt.hysaishi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kmz.ctjpmb.com

[U25] Py：CSV 按字典读
来源：http://kox.meibo888.top

csv.DictReader(f)
来源：http://ffh.hysaishi.cn

[U26] Py：并发下载
来源：http://wyo.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bhm.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://bji.nanxinkj.top

aiohttp.ClientSession() 配合 async with
来源：http://pnh.zhoulong.xyz

[U28] Py：类型别名
来源：http://qfc.sxryk.cn

UserId = int
来源：http://euu.aizwys.cn

[U29] Py：属性校验
来源：http://uur.xuetiantiany.cn

@property 与 @x.setter 配合
来源：http://cqf.xingfuxueyuan.xyz

[U30] Py：数据类
来源：http://tfk.zhixingplan.top

@dataclass(slots=True)
来源：http://aem.jqgufenzy.top

[U31] Py：单测
来源：http://iyb.jiagoushi.top

python -m pytest -q
来源：http://vvr.bjfxy.top

[U32] Py：代码格式化
来源：http://wef.xuanzx.com

ruff format . && ruff check --fix .
来源：http://obb.gaohongyu789.top

[U33] Py：打包发布
来源：http://edn.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://jfm.quarkkingdee.top

[U34] Py：判断编码
来源：http://ygo.fktsv.cn

chardet.detect(raw)
来源：http://vim.yongpay.top

[U35] Py：发送邮件
来源：http://ppd.c1oappe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kqi.zhongyouzk.top

[U36] Py：定时任务
来源：http://daa.daxiang520.top

schedule.every(10).minutes.do(job)
来源：http://hym.hnxiangtu.top

[U37] Py：读写 Excel
来源：http://xvo.yanxiufei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jei.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://kum.yuxming.cn

Path(__file__).resolve().parent
来源：http://tad.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://ftf.sjlbkw.cn

sys.stdout.isatty()
来源：http://nsm.xingfuxueyuan.xyz

[U40] Py：打印到标准错误
来源：http://tbx.yangfankeji.com

print("err", file=sys.stderr)
来源：http://yla.iojbl.cn


<!-- 参考信息 -->