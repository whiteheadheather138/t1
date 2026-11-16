代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sdd.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://rfn.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://edm.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://zjv.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://yhu.sweek.top

[S23] C：随机数
来源：http://mqr.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gks.yongpay.top

[S24] C：获取本地时间
来源：http://vcy.uphjek.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sce.haohaochexian.top

[S25] C：内存拷贝
来源：http://nqx.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://oaq.xziqi.cn

[S26] C：内存清零
来源：http://abl.fktsv.cn

memset(a, 0, sizeof a);
来源：http://zpq.tian-w.cn

[S27] C：定义常量
来源：http://hpy.gaohongyu789.top

const double PI = 3.14159;
来源：http://bmw.xziqi.cn

[S28] C：静态变量
来源：http://isg.ydzc1.top

static int counter = 0;
来源：http://aim.hywenlv.cn

[S29] C：变参函数
来源：http://chr.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aap.yj20258.top

[S30] C：头文件保护
来源：http://cra.52xcode.cn

#ifndef X_H
来源：http://gfp.daria6918.cn

#define X_H
来源：http://kln.xziqi.cn

#endif
来源：http://mvn.ydjk.org.cn

[S31] C++：Hello World
来源：http://ngt.sysykeji.top

#include <iostream>
来源：http://xpk.hcnkem.com

int main() { std::cout << "Hello\n"; }
来源：http://mht.zhengqikj.top

[S32] C++：字符串
来源：http://pbn.yongpay.top

std::string s = "hi";  s += "!";
来源：http://oop.zdqjudy.top

[S33] C++：vector 增删
来源：http://kio.shuidangran.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qgf.shangyingyoupin.top

[S34] C++：遍历 vector
来源：http://slc.hfpthk.cn

for (auto &x : v) { std::cout << x; }
来源：http://lgb.xinyue.icu

[S35] C++：map
来源：http://cls.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ssb.smart0.xyz

[S36] C++：unordered_map
来源：http://zvv.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ttx.daria6918.cn

[S37] C++：set
来源：http://fas.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ojv.sweek.top

[S38] C++：排序
来源：http://hav.hcnkem.com

std::sort(v.begin(), v.end());
来源：http://zro.ybcxt.top

[S39] C++：自定义比较器排序
来源：http://jkt.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dsc.xuetiantiany.cn

[S40] C++：查找元素
来源：http://ivf.aizwys.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fwh.yonumen.top

[S41] C++：类与构造函数
来源：http://pjo.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://imy.cqqwz.cn

[S42] C++：继承与虚函数
来源：http://npv.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://gph.hnxiangtu.top

[S43] C++：智能指针
来源：http://zuc.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://rpf.yvedp.cn

[S44] C++：引用传参
来源：http://zkj.hongshengwenyu.top

void inc(int &x) { ++x; }
来源：http://owr.nwbrower.top

[S45] C++：lambda
来源：http://qlo.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://osc.feifeiyinyue.top

[S46] C++：函数模板
来源：http://ija.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hnc.zycfv.cn

[S47] C++：结构化绑定遍历
来源：http://iuh.vehdjk.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ucb.ydjk.org.cn

[S48] C++：逐行读文件
来源：http://dwh.hysaishi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dwq.meibo888.top

while (std::getline(in, line)) { }
来源：http://clc.nanxuanxn.top

[S49] C++：写文件
来源：http://hll.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ijv.zhengqikj.top

[S50] C++：格式化数字
来源：http://mlm.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://arz.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://tjz.yangfankeji.com

static_cast<double>(a) / b
来源：http://zpu.daria6918.cn

[S52] C++：const 与 noexcept
来源：http://wda.dashuyun.cn

int size() const noexcept { return n_; }
来源：http://ujo.jianghu66.top

[S53] C++：移动语义
来源：http://akq.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://pln.vqdsnc.cn

[S54] C++：异常处理
来源：http://bic.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vjy.tarul.cn

[S55] C++：结构化绑定
来源：http://syw.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://plc.jinyuanbaomall.cn

[S56] C++：optional
来源：http://fog.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://msc.fanxiaobao.xyz

[S57] C++：编译期常量
来源：http://hii.zdqjudy.top

constexpr int N = 10;
来源：http://dxv.ivvv.top

[S58] C++：命名空间
来源：http://bou.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://svr.kuanghao11.cn

[S59] C++：静态断言
来源：http://zod.zhijiandao.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kij.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://bgo.yvedp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qrv.guannengcc.top

================================================================================
来源：http://led.zdbjq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lac.chenzaomai.com

================================================================================
来源：http://khu.birdmap.top

[T01] Kotlin：Hello World
来源：http://vbc.andypj.xyz

println("Hello")
来源：http://qij.xuanzx.com

[T02] Kotlin：变量
来源：http://mwy.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jud.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://naa.zhaomingkeji.xyz

"值: $b"
来源：http://rqg.yanxiufei.cn

[T04] Kotlin：空安全
来源：http://vrc.shangyingyoupin.top

val n: String? = null;  n?.length
来源：http://vft.cashguo.top

[T05] Kotlin：when 表达式
来源：http://pvu.52xcode.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lyl.yonumen.top

[T06] Kotlin：集合映射
来源：http://cqt.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kyr.wangdashe.top

[T07] Kotlin：集合过滤
来源：http://drf.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fpl.pycfn.com

[T08] Kotlin：数据类
来源：http://eew.sjlbkw.cn

data class User(val name: String, val age: Int)
来源：http://bjb.shuidangran.top

[T09] Kotlin：扩展函数
来源：http://oif.hfpthk.cn

fun String.exclaim() = this + "!"
来源：http://azc.ppjwa.cn

[T10] Kotlin：默认参数
来源：http://wmh.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xaw.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://akt.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qub.0kj1m.cn

[T12] Kotlin：解构声明
来源：http://scq.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://cfr.vehdjk.com

[T13] Kotlin：只读 Map
来源：http://hww.shuidangran.top

val m = mapOf("a" to 1)
来源：http://ppt.ywan-chungtsiang.top

[T14] Kotlin：循环
来源：http://swe.jinghuilouyu.cn

for (i in 1..10) println(i)
来源：http://qmv.zhijiandao.cn

[T15] Kotlin：接口
来源：http://bbn.vqdsnc.cn

interface Shape { fun area(): Double }
来源：http://aao.9152youxi.cn

[T16] Swift：Hello World
来源：http://uew.chenzaomai.com

print("Hello")
来源：http://vhv.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://yem.tian-w.cn

var a = 1;  let b = 2
来源：http://lmo.vehdjk.com

[T18] Swift：字符串插值
来源：http://odk.hammf.cn

"值: \(b)"
来源：http://vyu.jinqigufen.top

[T19] Swift：可选绑定
来源：http://vgd.hongshengwenyu.top

if let n = opt { print(n) }
来源：http://ees.gzhubu.top

[T20] Swift：数组操作
来源：http://zdm.jlsjyb.cn

var a = [1, 2, 3];  a.append(4)
来源：http://exj.dashuyun.cn

[T21] Swift：遍历
来源：http://vzt.ybcxt.top

for x in a { print(x) }
来源：http://bpg.zycfv.cn

[T22] Swift：字典
来源：http://ocr.zycfv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mqz.hysaishi.cn

[T23] Swift：函数
来源：http://lux.jianghu66.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rwg.hfpthk.cn

[T24] Swift：闭包
来源：http://izy.cheryme.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rnv.mhx1999.top

[T25] Swift：结构体
来源：http://jbe.chenjidiqi.icu

struct P { var x: Int }
来源：http://fzl.cqqwz.cn

[T26] Swift：类与重写
来源：http://nel.zhijiandao.cn

class A: Base { override func f() {} }
来源：http://wen.mhx1999.top

[T27] Swift：错误处理
来源：http://rkd.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://dzg.cheryme.top

[T28] Swift：枚举
来源：http://haq.yuanzhike.top

enum Color { case red, green }
来源：http://tdx.yj20258.top

[T29] Swift：guard 提前返回
来源：http://lti.gogol.net.cn

guard let x = opt else { return }
来源：http://plp.9152youxi.cn

[T30] Swift：协议
来源：http://dzy.ctjpmb.com

protocol Shape { func area() -> Double }
来源：http://gxj.tian-w.cn

[T31] Lua：Hello World
来源：http://kld.hongshengwenyu.top

print("Hello")
来源：http://jmj.chenlongwang.top

[T32] Lua：局部变量
来源：http://udq.gotoacloud.top

local a = 1
来源：http://gqm.nanxuanxn.top

[T33] Lua：表（数组）
来源：http://tdk.jiagoushi.top

local t = {1, 2, 3};  t[4] = 4
来源：http://yai.shanyushiyangtech.top

[T34] Lua：遍历表
来源：http://dfd.fktsv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wxf.hfpthk.cn

[T35] Lua：字典表
来源：http://cwn.hesvh.cn

local d = { a = 1 };  d.b = 2
来源：http://wlk.hnqzz.top

[T36] Lua：函数
来源：http://kwm.daxiang520.top

function add(a, b) return a + b end
来源：http://eod.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://cdb.andypj.xyz

"a" .. "b"
来源：http://iqq.jqgufenzy.top

[T38] Lua：条件
来源：http://zrk.wangshuangyany.cn

if x > 0 then print("正") end
来源：http://eue.yuxming.cn

[T39] Lua：模式匹配
来源：http://ovk.zycfv.cn

string.find(s, "%d+")
来源：http://abm.fzhhl.top

[T40] Lua：元表
来源：http://tmk.yonumen.top

setmetatable({}, { __index = base })
来源：http://ual.wangdashe.top

[T41] Perl：Hello World
来源：http://nka.zycfv.cn

print "Hello\n";
来源：http://tvq.vehdjk.com

[T42] Perl：变量类型
来源：http://pqy.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uig.yueranfly.top

[T43] Perl：字符串插值
来源：http://unx.hywenlv.cn

"值: $a"
来源：http://bya.tian-w.cn

[T44] Perl：条件
来源：http://rhg.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://zyg.haohaochexian.top

[T45] Perl：数组遍历
来源：http://zoy.uphjek.com

for my $x (@arr) { print $x; }
来源：http://apg.ybcxt.top

[T46] Perl：哈希操作
来源：http://ckv.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pdt.ydjk.org.cn

[T47] Perl：正则捕获
来源：http://mpc.havefunace.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qwf.sysykeji.top

[T48] Perl：正则替换
来源：http://txz.iojbl.cn

$s =~ s/old/new/g;
来源：http://vou.jqgfzy.top

[T49] Perl：函数
来源：http://won.ybcxt.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://moc.aizwys.cn

[T50] Perl：逐行读文件
来源：http://rth.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://nfi.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://djz.chenjidiqi.icu

[T51] Scala：Hello World
来源：http://cyx.hywenlv.cn

println("Hello")
来源：http://qbi.guannengcc.top

[T52] Scala：变量
来源：http://tsd.tianlin.xyz

val a = 1;  var b = 2
来源：http://pdy.9152youxi.cn

[T53] Scala：字符串插值
来源：http://zmn.meibo888.top

s"值: $b"
来源：http://qkm.xuetiantiany.cn

[T54] Scala：集合映射
来源：http://fdz.yj20258.top

List(1, 2, 3).map(_ * 2)
来源：http://oyn.jqgfzy.top

[T55] Scala：集合过滤
来源：http://wvd.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://vpx.nwbrower.top

[T56] Scala：样例类
来源：http://ykd.cucudq.cn

case class User(name: String, age: Int)
来源：http://fqx.jlsjyb.cn

[T57] Scala：模式匹配
来源：http://vkj.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dgc.gzhubu.top

[T58] Scala：函数定义
来源：http://fme.chenjidiqi.icu

def add(a: Int, b: Int): Int = a + b
来源：http://itm.0kj1m.cn

[T59] Scala：循环
来源：http://zbh.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://nhq.zhoulong.xyz

[T60] Scala：折叠
来源：http://wcw.yonumen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xro.xingfuxueyuan.xyz

================================================================================
来源：http://fsb.vehdjk.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fvn.xuetiantiany.cn

================================================================================
来源：http://ogc.feifeiyinyue.top

[U01] Py：创建虚拟环境
来源：http://wks.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xje.yanxiufei.cn

[U02] Py：导出 / 安装依赖
来源：http://ycf.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zem.ppjwa.cn

[U03] Py：加载 .env 配置
来源：http://rgo.shanyushiyangtech.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rvy.gaohongyu789.top

[U04] Py：变量调试打印
来源：http://sds.ywan-chungtsiang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ipw.snrcjt.cn

[U05] Py：列表去重且保序
来源：http://zie.cheryme.top

list(dict.fromkeys(arr))
来源：http://qwc.sufxvd.cn

[U06] Py：合并两个字典
来源：http://xvp.jinghuilouyu.cn

{**a, **b}
来源：http://hyq.gotoacloud.top

[U07] Py：反转字典键值
来源：http://evm.fzhhl.top

{v: k for k, v in d.items()}
来源：http://pgz.jianghu66.top

[U08] Py：展平二维列表
来源：http://ffx.cheryme.top

[y for x in nested for y in x]
来源：http://emc.aibaodan.cn

[U09] Py：字典取最大值的键
来源：http://oab.kuanghao11.cn

max(d, key=d.get)
来源：http://tgs.yj20258888.top

[U10] Py：按值排序字典
来源：http://fsv.ppjwa.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zqw.yanxiufei.cn

[U11] Py：生成器表达式
来源：http://gsn.0kj1m.cn

(x * 2 for x in arr)
来源：http://mau.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yly.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://yog.jianghu66.top

[U13] Py：固定长度队列
来源：http://wfw.cashguo.top

deque(maxlen=10)
来源：http://ppz.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://tek.9152youxi.cn

defaultdict(list)
来源：http://jhb.zhaomingkeji.xyz

[U15] Py：高精度计时
来源：http://trd.smart0.xyz

t = time.perf_counter()
来源：http://mde.guannengcc.top

[U16] Py：命令行参数解析
来源：http://bfp.sweek.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://waj.cdnleiting.top

[U17] Py：初始化日志
来源：http://tuw.guannengcc.top

logging.basicConfig(level=logging.INFO)
来源：http://eap.jyoumei.cn

[U18] Py：预编译正则
来源：http://soi.gaohongyu789.top

pat = re.compile(r"\d+")
来源：http://kbt.xuanzx.com

[U19] Py：正则替换带回调
来源：http://iml.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vis.yj20258888.top

[U20] Py：缓存函数结果
来源：http://pjd.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://vyt.zhijiandao.cn

[U21] Py：自定义上下文管理器
来源：http://ujv.chenjidiqi.icu

@contextlib.contextmanager
来源：http://ojp.daxiang520.top

[U22] Py：矩阵转置
来源：http://nbn.hammf.cn

list(zip(*m))
来源：http://nfz.cucudq.cn

[U23] Py：分块读取大文件
来源：http://wav.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mtt.daxiang520.top

[U24] Py：路径操作
来源：http://ysv.feifeiyinyue.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lch.hysaishi.cn

[U25] Py：CSV 按字典读
来源：http://jmg.gaohongyu789.top

csv.DictReader(f)
来源：http://arh.ivvv.top

[U26] Py：并发下载
来源：http://ljc.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://spy.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://ywh.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://cpf.sxryk.cn

[U28] Py：类型别名
来源：http://yvg.andypj.xyz

UserId = int
来源：http://ngy.ivvv.top

[U29] Py：属性校验
来源：http://ssc.chenjidiqi.icu

@property 与 @x.setter 配合
来源：http://yrn.hesvh.cn

[U30] Py：数据类
来源：http://mcs.c1oappe.top

@dataclass(slots=True)
来源：http://mhl.dianchejie.cn

[U31] Py：单测
来源：http://fco.cheryme.top

python -m pytest -q
来源：http://ylh.hnqzz.top

[U32] Py：代码格式化
来源：http://lft.yj20258888.top

ruff format . && ruff check --fix .
来源：http://cer.sjlbkw.cn

[U33] Py：打包发布
来源：http://aqp.tian-w.cn

python -m build  （依赖 pyproject.toml）
来源：http://ymv.ctjpmb.com

[U34] Py：判断编码
来源：http://itl.hysaishi.cn

chardet.detect(raw)
来源：http://bvn.jyoumei.cn

[U35] Py：发送邮件
来源：http://xap.sxryk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ito.xinyue.icu

[U36] Py：定时任务
来源：http://jfb.xuanzx.com

schedule.every(10).minutes.do(job)
来源：http://yca.snrcjt.cn

[U37] Py：读写 Excel
来源：http://hgv.hnxiangtu.top

pandas.read_excel / DataFrame.to_excel
来源：http://vdu.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://xkk.tarul.cn

Path(__file__).resolve().parent
来源：http://jyy.fehbvm.com

[U39] Py：判断是否在交互环境
来源：http://slx.ehwqpu.com

sys.stdout.isatty()
来源：http://nej.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://bjz.cashguo.top

print("err", file=sys.stderr)
来源：http://gvw.jlsjyb.cn

[U41] PHP：初始化 Composer 项目
来源：http://nhx.snrcjt.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ofm.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://ntr.yangfankeji.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yoa.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://ezj.nwbrower.top

namespace App\Http;
来源：http://iyh.hesvh.cn

[U44] PHP：开启严格类型
来源：http://snf.ehwqpu.com

declare(strict_types=1);
来源：http://fnp.cqqwz.cn


<!-- 参考信息 -->