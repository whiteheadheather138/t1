代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://fam.tarul.cn

[S23] C：随机数
来源：http://ysq.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://tkj.havefunace.top

[S24] C：获取本地时间
来源：http://qot.vehdjk.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fzz.epnwcf.com

[S25] C：内存拷贝
来源：http://anb.tarul.cn

memcpy(dst, src, n);
来源：http://kpy.sweek.top

[S26] C：内存清零
来源：http://zfg.fengsongda.top

memset(a, 0, sizeof a);
来源：http://dep.feifeiyinyue.top

[S27] C：定义常量
来源：http://fre.chenjidiqi.icu

const double PI = 3.14159;
来源：http://atf.ydzc1.top

[S28] C：静态变量
来源：http://yzm.havefunace.top

static int counter = 0;
来源：http://sjt.gaohongyu789.top

[S29] C：变参函数
来源：http://nyi.gogol.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lwj.redwolf501.top

[S30] C：头文件保护
来源：http://aqz.ydzc1.top

#ifndef X_H
来源：http://hgj.redwolf501.top

#define X_H
来源：http://tfm.wangdashe.top

#endif
来源：http://fer.hywenlv.cn

[S31] C++：Hello World
来源：http://ysh.xinyue.icu

#include <iostream>
来源：http://jig.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://wou.jqgfzy.top

[S32] C++：字符串
来源：http://eif.redwolf501.top

std::string s = "hi";  s += "!";
来源：http://tcr.andypj.xyz

[S33] C++：vector 增删
来源：http://ywz.havefunace.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nqc.wangdashe.top

[S34] C++：遍历 vector
来源：http://juz.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://iyd.gotoacloud.top

[S35] C++：map
来源：http://xyq.shzxlz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fxq.yj20258.top

[S36] C++：unordered_map
来源：http://oef.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dmx.gotoacloud.top

[S37] C++：set
来源：http://bud.nanxuanxn.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iay.tarul.cn

[S38] C++：排序
来源：http://mif.daxiang520.top

std::sort(v.begin(), v.end());
来源：http://apu.tian-w.cn

[S39] C++：自定义比较器排序
来源：http://xjf.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lox.52xcode.cn

[S40] C++：查找元素
来源：http://hnr.jqgufenzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xzq.hfpthk.cn

[S41] C++：类与构造函数
来源：http://tmv.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://krk.316326.xyz

[S42] C++：继承与虚函数
来源：http://itt.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://cpc.hfpthk.cn

[S43] C++：智能指针
来源：http://jab.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://grg.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://nri.jianghu66.top

void inc(int &x) { ++x; }
来源：http://sbt.smart0.xyz

[S45] C++：lambda
来源：http://vgm.yj202588.top

auto add = [](int a, int b) { return a + b; };
来源：http://ooy.zhijiandao.cn

[S46] C++：函数模板
来源：http://nvn.zhijiandao.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nqo.sjlbkw.cn

[S47] C++：结构化绑定遍历
来源：http://wfh.vehdjk.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nwa.tanke756.top

[S48] C++：逐行读文件
来源：http://wzd.tanke756.top

std::ifstream in("a.txt");  std::string line;
来源：http://hnl.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://agz.mhx1999.top

[S49] C++：写文件
来源：http://fnj.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ltb.gogol.net.cn

[S50] C++：格式化数字
来源：http://rej.sxryk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zrr.yanxiufei.cn

[S51] C++：显式类型转换
来源：http://mpz.cdnleiting.top

static_cast<double>(a) / b
来源：http://oyp.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://jnn.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://obu.cdnleiting.top

[S53] C++：移动语义
来源：http://lhr.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://zby.cashguo.top

[S54] C++：异常处理
来源：http://zau.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lag.yfazqb.com

[S55] C++：结构化绑定
来源：http://sqd.bbcook.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://otd.jinghuilouyu.cn

[S56] C++：optional
来源：http://udz.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uyz.tianlin.xyz

[S57] C++：编译期常量
来源：http://qen.haohaochexian.top

constexpr int N = 10;
来源：http://ajl.wangdashe.top

[S58] C++：命名空间
来源：http://nxj.wangshuangyany.cn

namespace ns { int f() { return 1; } }
来源：http://sng.smart0.xyz

[S59] C++：静态断言
来源：http://tmc.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nsu.pycfn.com

[S60] C++：遍历并删除元素
来源：http://wtv.fehbvm.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mba.ctjpmb.com

================================================================================
来源：http://hrc.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://col.tianlin.xyz

================================================================================
来源：http://ahi.cashguo.top

[T01] Kotlin：Hello World
来源：http://cup.jinqigfzy.top

println("Hello")
来源：http://ebv.zdbjq.cn

[T02] Kotlin：变量
来源：http://tqz.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lux.cheryme.top

[T03] Kotlin：字符串模板
来源：http://nff.jiagoushi.top

"值: $b"
来源：http://iwl.mhx1999.top

[T04] Kotlin：空安全
来源：http://vpl.daxiang520.top

val n: String? = null;  n?.length
来源：http://lzk.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://awe.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fjq.cheryme.top

[T06] Kotlin：集合映射
来源：http://uve.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://srk.hnxiangtu.top

[T07] Kotlin：集合过滤
来源：http://rkd.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://otr.zhixingplan.top

[T08] Kotlin：数据类
来源：http://fyh.hesvh.cn

data class User(val name: String, val age: Int)
来源：http://avr.chenjidiqi.icu

[T09] Kotlin：扩展函数
来源：http://nln.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://qev.9152youxi.cn

[T10] Kotlin：默认参数
来源：http://taa.hywenlv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uig.haohaochexian.top

[T11] Kotlin：协程
来源：http://tay.jlsjyb.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gol.xylfe.cn

[T12] Kotlin：解构声明
来源：http://ddt.yvedp.cn

val (a, b) = Pair(1, 2)
来源：http://lxv.jqgufenzy.top

[T13] Kotlin：只读 Map
来源：http://cqw.tarul.cn

val m = mapOf("a" to 1)
来源：http://iwe.iojbl.cn

[T14] Kotlin：循环
来源：http://otm.ehwqpu.com

for (i in 1..10) println(i)
来源：http://pjz.daria6918.cn

[T15] Kotlin：接口
来源：http://jqo.svipenyu.cn

interface Shape { fun area(): Double }
来源：http://kkq.jqgfzy.top

[T16] Swift：Hello World
来源：http://evp.tianlin.xyz

print("Hello")
来源：http://krx.yongpay.top

[T17] Swift：变量与常量
来源：http://ytf.cashguo.top

var a = 1;  let b = 2
来源：http://ukh.xylfe.cn

[T18] Swift：字符串插值
来源：http://zcl.bbcook.cn

"值: \(b)"
来源：http://oww.fehbvm.com

[T19] Swift：可选绑定
来源：http://yum.bjfxy.top

if let n = opt { print(n) }
来源：http://hvj.shanyushiyangkeji.top

[T20] Swift：数组操作
来源：http://smu.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://iid.tarul.cn

[T21] Swift：遍历
来源：http://hwy.guannengcc.top

for x in a { print(x) }
来源：http://tgj.guowangkeji.top

[T22] Swift：字典
来源：http://ems.ehwqpu.com

var d = ["a": 1];  d["b"] = 2
来源：http://uig.iojbl.cn

[T23] Swift：函数
来源：http://haq.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ceo.jqgufenzy.top

[T24] Swift：闭包
来源：http://cyz.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nlx.c1oappe.top

[T25] Swift：结构体
来源：http://izv.redwolf501.top

struct P { var x: Int }
来源：http://odu.pengpengdd.cyou

[T26] Swift：类与重写
来源：http://cmj.xuanzx.com

class A: Base { override func f() {} }
来源：http://ivo.316326.xyz

[T27] Swift：错误处理
来源：http://vuz.cheryme.top

do { try f() } catch { print(error) }
来源：http://rau.xziqi.cn

[T28] Swift：枚举
来源：http://emg.redwolf501.top

enum Color { case red, green }
来源：http://lxj.shuidangran.top

[T29] Swift：guard 提前返回
来源：http://gvk.ybcxt.top

guard let x = opt else { return }
来源：http://xbx.cdnleiting.top

[T30] Swift：协议
来源：http://xmo.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://cdi.hysaishi.cn

[T31] Lua：Hello World
来源：http://yga.yvedp.cn

print("Hello")
来源：http://rrs.sufxvd.cn

[T32] Lua：局部变量
来源：http://rdy.ctjpmb.com

local a = 1
来源：http://lvp.cqqwz.cn

[T33] Lua：表（数组）
来源：http://azq.yj20258888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mpe.hesvh.cn

[T34] Lua：遍历表
来源：http://hkp.uphjek.com

for i, v in ipairs(t) do print(i, v) end
来源：http://iqy.ybcxt.top

[T35] Lua：字典表
来源：http://lef.kuanghao11.cn

local d = { a = 1 };  d.b = 2
来源：http://ogh.sysykeji.top

[T36] Lua：函数
来源：http://mwj.xylfe.cn

function add(a, b) return a + b end
来源：http://bws.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://gdv.cdnleiting.top

"a" .. "b"
来源：http://hmm.guowangkeji.top

[T38] Lua：条件
来源：http://dbq.hongshengwenyu.top

if x > 0 then print("正") end
来源：http://rtp.zdbjq.cn

[T39] Lua：模式匹配
来源：http://muc.yj20258.top

string.find(s, "%d+")
来源：http://fqv.nwbrower.top

[T40] Lua：元表
来源：http://enf.ydjk.org.cn

setmetatable({}, { __index = base })
来源：http://bhb.cheryme.top

[T41] Perl：Hello World
来源：http://qzd.yfazqb.com

print "Hello\n";
来源：http://zvf.pycfn.com

[T42] Perl：变量类型
来源：http://lsn.meibo888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oky.meibo888.top

[T43] Perl：字符串插值
来源：http://plc.shuidangran.top

"值: $a"
来源：http://txz.fktsv.cn

[T44] Perl：条件
来源：http://bgy.redwolf501.top

if ($a > 0) { print "正"; }
来源：http://xxy.wangdashe.top

[T45] Perl：数组遍历
来源：http://hby.zdbjq.cn

for my $x (@arr) { print $x; }
来源：http://qch.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://ghy.sysykeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lrf.ywan-chungtsiang.top

[T47] Perl：正则捕获
来源：http://jbo.zhaomingkeji.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://dgs.epnwcf.com

[T48] Perl：正则替换
来源：http://gnf.yfazqb.com

$s =~ s/old/new/g;
来源：http://rjq.hnqzz.top

[T49] Perl：函数
来源：http://dea.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nmo.cashguo.top

[T50] Perl：逐行读文件
来源：http://kxi.pengpengdd.cyou

open my $fh, "<", "a.txt" or die $!;
来源：http://cez.jlsjyb.cn

while (my $line = <$fh>) { print $line; }
来源：http://pvg.shanyushiyangtech.top

[T51] Scala：Hello World
来源：http://zcn.meibo888.top

println("Hello")
来源：http://srp.jinqigfzy.top

[T52] Scala：变量
来源：http://vyd.fktsv.cn

val a = 1;  var b = 2
来源：http://pcv.shuidangran.top

[T53] Scala：字符串插值
来源：http://lrg.cheryme.top

s"值: $b"
来源：http://vbh.vehdjk.com

[T54] Scala：集合映射
来源：http://lxx.jqgufenzy.top

List(1, 2, 3).map(_ * 2)
来源：http://jgd.jinqigufen.top

[T55] Scala：集合过滤
来源：http://dah.birdmap.top

List(1, 2, 3).filter(_ > 1)
来源：http://pir.zdqjudy.top

[T56] Scala：样例类
来源：http://kwn.cdnleiting.top

case class User(name: String, age: Int)
来源：http://azq.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://mvr.yangfankeji.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://ihh.zycfv.cn

[T58] Scala：函数定义
来源：http://ygh.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://upr.zhaomingkeji.xyz

[T59] Scala：循环
来源：http://oue.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://hkk.birdmap.top

[T60] Scala：折叠
来源：http://fty.smart0.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dkw.fengsongda.top

================================================================================
来源：http://qzw.tarul.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ixe.xinyue.icu

================================================================================
来源：http://gst.fzhhl.top

[U01] Py：创建虚拟环境
来源：http://rlb.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://muv.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://mmb.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wgd.hcnkem.com

[U03] Py：加载 .env 配置
来源：http://lyh.shangyingyoupin.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jtq.mhx1999.top

[U04] Py：变量调试打印
来源：http://ncx.daria6918.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ryn.guannengcc.top

[U05] Py：列表去重且保序
来源：http://ccf.daxiang520.top

list(dict.fromkeys(arr))
来源：http://jah.yuxming.cn

[U06] Py：合并两个字典
来源：http://lfj.yuanzhike.top

{**a, **b}
来源：http://osa.tarul.cn

[U07] Py：反转字典键值
来源：http://etl.snrcjt.cn

{v: k for k, v in d.items()}
来源：http://mtm.jinqigufen.top

[U08] Py：展平二维列表
来源：http://jsb.sysykeji.top

[y for x in nested for y in x]
来源：http://hio.vqdsnc.cn

[U09] Py：字典取最大值的键
来源：http://ito.yj202588.top

max(d, key=d.get)
来源：http://xkj.zdqjudy.top

[U10] Py：按值排序字典
来源：http://bya.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://clr.cdnleiting.top

[U11] Py：生成器表达式
来源：http://rnm.nanxuanxn.top

(x * 2 for x in arr)
来源：http://elt.xuanzx.com

[U12] Py：取出现最多的 3 个元素
来源：http://cre.zhongyouzk.top

Counter(arr).most_common(3)
来源：http://pzo.ppjwa.cn

[U13] Py：固定长度队列
来源：http://nij.ybcxt.top

deque(maxlen=10)
来源：http://exf.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://tdb.jianghu66.top

defaultdict(list)
来源：http://cjg.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://fig.ppjwa.cn

t = time.perf_counter()
来源：http://tkg.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://vuy.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lmb.nwbrower.top

[U17] Py：初始化日志
来源：http://twi.chenzaomai.com

logging.basicConfig(level=logging.INFO)
来源：http://nqe.hfpthk.cn

[U18] Py：预编译正则
来源：http://oep.aizwys.cn

pat = re.compile(r"\d+")
来源：http://srk.ydzc1.top

[U19] Py：正则替换带回调
来源：http://pdf.shuidangran.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dym.yanxiufei.cn

[U20] Py：缓存函数结果
来源：http://cfd.cqqwz.cn

@functools.lru_cache(maxsize=None)
来源：http://dbq.zhixingplan.top

[U21] Py：自定义上下文管理器
来源：http://inm.nanxinkj.top

@contextlib.contextmanager
来源：http://xua.hysaishi.cn

[U22] Py：矩阵转置
来源：http://grk.yuanzhike.top

list(zip(*m))
来源：http://mgx.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://afk.havefunace.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vkx.hesvh.cn

[U24] Py：路径操作
来源：http://ydz.tianlin.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ehx.sufxvd.cn

[U25] Py：CSV 按字典读
来源：http://xop.yonumen.top

csv.DictReader(f)
来源：http://meh.gogol.net.cn

[U26] Py：并发下载
来源：http://dnt.hfpthk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gpb.guowangkeji.top

[U27] Py：异步 HTTP
来源：http://ziw.sweek.top

aiohttp.ClientSession() 配合 async with
来源：http://klj.kuanghao11.cn

[U28] Py：类型别名
来源：http://cfz.sjlbkw.cn

UserId = int
来源：http://gjl.havefunace.top

[U29] Py：属性校验
来源：http://pqx.ehwqpu.com

@property 与 @x.setter 配合
来源：http://ftf.yuanzhike.top

[U30] Py：数据类
来源：http://wwh.pycfn.com

@dataclass(slots=True)
来源：http://fmm.tian-w.cn

[U31] Py：单测
来源：http://sbx.hongshengwenyu.top

python -m pytest -q
来源：http://tpn.bbcook.cn

[U32] Py：代码格式化
来源：http://wft.guannengcc.top

ruff format . && ruff check --fix .
来源：http://pxj.yanxiufei.cn

[U33] Py：打包发布
来源：http://tzb.nanxinkj.top

python -m build  （依赖 pyproject.toml）
来源：http://fwo.jianghu66.top

[U34] Py：判断编码
来源：http://zve.ywan-chungtsiang.top

chardet.detect(raw)
来源：http://cxj.xinyue.icu

[U35] Py：发送邮件
来源：http://aps.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dvt.fktsv.cn

[U36] Py：定时任务
来源：http://trq.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://siq.yfazqb.com

[U37] Py：读写 Excel
来源：http://dkf.bjfxy.top

pandas.read_excel / DataFrame.to_excel
来源：http://wek.jinyuanbaomall.cn

[U38] Py：获取脚本所在目录
来源：http://xcl.fehbvm.com

Path(__file__).resolve().parent
来源：http://fwn.c1oappe.top

[U39] Py：判断是否在交互环境
来源：http://bqm.ydzc1.top

sys.stdout.isatty()
来源：http://ixs.iojbl.cn

[U40] Py：打印到标准错误
来源：http://smj.wangdashe.top

print("err", file=sys.stderr)
来源：http://vth.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://znb.zycfv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tzr.52xcode.cn

[U42] PHP：PSR-4 自动加载
来源：http://xam.daxiang520.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nje.ywan-chungtsiang.top

[U43] PHP：声明命名空间
来源：http://ejt.feifeiyinyue.top

namespace App\Http;
来源：http://ivg.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://lfy.nwbrower.top

declare(strict_types=1);
来源：http://mau.yj20258.top

[U45] PHP：类型声明与返回类型
来源：http://qfz.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://bhy.hesvh.cn

[U46] PHP：可空类型
来源：http://iqp.hfpthk.cn

?string $name = null
来源：http://rxc.ppjwa.cn


<!-- 参考信息 -->