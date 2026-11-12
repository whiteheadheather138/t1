代发 wailian999

static int counter = 0;
来源：http://hel.chenlongwang.top

[S29] C：变参函数
来源：http://pru.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ecp.cashguo.top

[S30] C：头文件保护
来源：http://tpu.smart0.xyz

#ifndef X_H
来源：http://zam.sweek.top

#define X_H
来源：http://vso.ydjk.org.cn

#endif
来源：http://lip.cqqwz.cn

[S31] C++：Hello World
来源：http://nki.shzxlz.cn

#include <iostream>
来源：http://qee.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://pmm.shanyushiyangkeji.top

[S32] C++：字符串
来源：http://cup.quarkkingdee.top

std::string s = "hi";  s += "!";
来源：http://xsx.hysaishi.cn

[S33] C++：vector 增删
来源：http://mza.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wdl.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://vis.yonumen.top

for (auto &x : v) { std::cout << x; }
来源：http://zhc.jiagoushi.top

[S35] C++：map
来源：http://gun.redwolf501.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wma.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://kqq.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ngs.0kj1m.cn

[S37] C++：set
来源：http://uhj.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://buh.chenjidiqi.icu

[S38] C++：排序
来源：http://xtr.ivvv.top

std::sort(v.begin(), v.end());
来源：http://bwx.zhijiandao.cn

[S39] C++：自定义比较器排序
来源：http://ljk.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ljl.hnqzz.top

[S40] C++：查找元素
来源：http://nee.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mlo.yanxiufei.cn

[S41] C++：类与构造函数
来源：http://mkc.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zlj.smart0.xyz

[S42] C++：继承与虚函数
来源：http://oxn.ydzc1.top

class B : public Base { public: void f() override {} };
来源：http://opt.zhoulong.xyz

[S43] C++：智能指针
来源：http://eik.jqgfzy.top

auto p = std::make_unique<int>(5);
来源：http://dyk.cdnleiting.top

[S44] C++：引用传参
来源：http://qzl.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://gwz.redwolf501.top

[S45] C++：lambda
来源：http://rrg.fanxiaobao.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://hcm.zdbjq.cn

[S46] C++：函数模板
来源：http://uhf.gzhubu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mxp.fktsv.cn

[S47] C++：结构化绑定遍历
来源：http://xxq.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bmi.smart0.xyz

[S48] C++：逐行读文件
来源：http://inh.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://rgv.xylfe.cn

while (std::getline(in, line)) { }
来源：http://xdq.svipenyu.cn

[S49] C++：写文件
来源：http://esx.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hra.nanxinkj.top

[S50] C++：格式化数字
来源：http://cts.nwbrower.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lqv.havefunace.top

[S51] C++：显式类型转换
来源：http://lgm.aizwys.cn

static_cast<double>(a) / b
来源：http://aea.aibaodan.cn

[S52] C++：const 与 noexcept
来源：http://iif.jqgufenzy.top

int size() const noexcept { return n_; }
来源：http://aom.gzhubu.top

[S53] C++：移动语义
来源：http://osm.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://nol.xuanzx.com

[S54] C++：异常处理
来源：http://ctj.wangshuangyany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ado.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://grx.xziqi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zdg.yj20258.top

[S56] C++：optional
来源：http://rnt.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eaq.fktsv.cn

[S57] C++：编译期常量
来源：http://mpp.yfazqb.com

constexpr int N = 10;
来源：http://zme.shuidangran.top

[S58] C++：命名空间
来源：http://ejy.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://fpp.yvedp.cn

[S59] C++：静态断言
来源：http://bcv.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zxb.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://hvs.yongpay.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://noq.dashuyun.cn

================================================================================
来源：http://ofw.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rea.smart0.xyz

================================================================================
来源：http://zbk.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://ppq.andypj.xyz

println("Hello")
来源：http://ymd.smart0.xyz

[T02] Kotlin：变量
来源：http://ijk.hesvh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://smg.hnxiangtu.top

[T03] Kotlin：字符串模板
来源：http://wwn.yj20258888.top

"值: $b"
来源：http://isz.dashuyun.cn

[T04] Kotlin：空安全
来源：http://jma.hysaishi.cn

val n: String? = null;  n?.length
来源：http://tjr.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://lox.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yev.cdnleiting.top

[T06] Kotlin：集合映射
来源：http://zdb.hnxiangtu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://oqi.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://yiu.hywenlv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jno.ctjpmb.com

[T08] Kotlin：数据类
来源：http://zgs.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://rlz.snrcjt.cn

[T09] Kotlin：扩展函数
来源：http://jsi.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://hhb.jlsjyb.cn

[T10] Kotlin：默认参数
来源：http://dcy.hammf.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sju.yueranfly.top

[T11] Kotlin：协程
来源：http://aob.redwolf501.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nek.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://ltb.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://ryk.yonumen.top

[T13] Kotlin：只读 Map
来源：http://ufw.sxryk.cn

val m = mapOf("a" to 1)
来源：http://feh.chenjidiqi.icu

[T14] Kotlin：循环
来源：http://bgi.ehwqpu.com

for (i in 1..10) println(i)
来源：http://qup.xuanzx.com

[T15] Kotlin：接口
来源：http://hij.gzhubu.top

interface Shape { fun area(): Double }
来源：http://kki.0kj1m.cn

[T16] Swift：Hello World
来源：http://wat.ydjk.org.cn

print("Hello")
来源：http://jis.hnxiangtu.top

[T17] Swift：变量与常量
来源：http://yrn.chenzaomai.com

var a = 1;  let b = 2
来源：http://jfw.shanyushiyangtech.top

[T18] Swift：字符串插值
来源：http://sxr.ctjpmb.com

"值: \(b)"
来源：http://kaf.hcnkem.com

[T19] Swift：可选绑定
来源：http://iup.hnxiangtu.top

if let n = opt { print(n) }
来源：http://ldp.cdnleiting.top

[T20] Swift：数组操作
来源：http://jwp.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jta.fzhhl.top

[T21] Swift：遍历
来源：http://afo.cucudq.cn

for x in a { print(x) }
来源：http://sod.yanxiufei.cn

[T22] Swift：字典
来源：http://dfk.zhaomingkeji.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://uyo.gzhubu.top

[T23] Swift：函数
来源：http://res.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kfn.jqgfzy.top

[T24] Swift：闭包
来源：http://mju.jyoumei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://evo.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://das.jianghu66.top

struct P { var x: Int }
来源：http://ozs.cdnleiting.top

[T26] Swift：类与重写
来源：http://act.hnqzz.top

class A: Base { override func f() {} }
来源：http://fup.yuxming.cn

[T27] Swift：错误处理
来源：http://nli.uphjek.com

do { try f() } catch { print(error) }
来源：http://uav.xziqi.cn

[T28] Swift：枚举
来源：http://cpo.9152youxi.cn

enum Color { case red, green }
来源：http://myn.316326.xyz

[T29] Swift：guard 提前返回
来源：http://jcm.pycfn.com

guard let x = opt else { return }
来源：http://tub.kuanghao11.cn

[T30] Swift：协议
来源：http://ibs.svipenyu.cn

protocol Shape { func area() -> Double }
来源：http://ojz.zhoulong.xyz

[T31] Lua：Hello World
来源：http://hye.redwolf501.top

print("Hello")
来源：http://tgc.xuanzx.com

[T32] Lua：局部变量
来源：http://lsg.fehbvm.com

local a = 1
来源：http://dei.jqgufenzy.top

[T33] Lua：表（数组）
来源：http://kyw.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jwe.hongshengwenyu.top

[T34] Lua：遍历表
来源：http://ojq.vqdsnc.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kod.andypj.xyz

[T35] Lua：字典表
来源：http://tgi.daxiang520.top

local d = { a = 1 };  d.b = 2
来源：http://khw.meibo888.top

[T36] Lua：函数
来源：http://wiy.ehwqpu.com

function add(a, b) return a + b end
来源：http://oms.hcnkem.com

[T37] Lua：字符串拼接
来源：http://ecb.xziqi.cn

"a" .. "b"
来源：http://lde.yuanzhike.top

[T38] Lua：条件
来源：http://ddg.gaohongyu789.top

if x > 0 then print("正") end
来源：http://cza.yanxiufei.cn

[T39] Lua：模式匹配
来源：http://xxk.c1oappe.top

string.find(s, "%d+")
来源：http://ayj.yangfankeji.com

[T40] Lua：元表
来源：http://pmq.fktsv.cn

setmetatable({}, { __index = base })
来源：http://wbz.jinghuilouyu.cn

[T41] Perl：Hello World
来源：http://ocz.zhixingplan.top

print "Hello\n";
来源：http://hpr.52xcode.cn

[T42] Perl：变量类型
来源：http://fof.jianghu66.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kfa.ybcxt.top

[T43] Perl：字符串插值
来源：http://xof.smart0.xyz

"值: $a"
来源：http://eji.bjfxy.top

[T44] Perl：条件
来源：http://skj.hammf.cn

if ($a > 0) { print "正"; }
来源：http://ear.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://pyw.xylfe.cn

for my $x (@arr) { print $x; }
来源：http://gpm.shzxlz.cn

[T46] Perl：哈希操作
来源：http://ozb.yanxiufei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jsz.shzxlz.cn

[T47] Perl：正则捕获
来源：http://elw.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://moi.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://psy.ybcxt.top

$s =~ s/old/new/g;
来源：http://csp.hnqzz.top

[T49] Perl：函数
来源：http://hph.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xxz.xuanzx.com

[T50] Perl：逐行读文件
来源：http://lwa.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://oqb.kuanghao11.cn

while (my $line = <$fh>) { print $line; }
来源：http://pyv.chenlongwang.top

[T51] Scala：Hello World
来源：http://hjt.gogol.net.cn

println("Hello")
来源：http://iai.ydzc1.top

[T52] Scala：变量
来源：http://kmz.cheryme.top

val a = 1;  var b = 2
来源：http://lmi.kuanghao11.cn

[T53] Scala：字符串插值
来源：http://aud.vqdsnc.cn

s"值: $b"
来源：http://qbt.hammf.cn

[T54] Scala：集合映射
来源：http://enz.aizwys.cn

List(1, 2, 3).map(_ * 2)
来源：http://tyj.tanke756.top

[T55] Scala：集合过滤
来源：http://sfg.zhijiandao.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ujy.smart0.xyz

[T56] Scala：样例类
来源：http://hkx.zhaomingkeji.xyz

case class User(name: String, age: Int)
来源：http://sgu.yuanzhike.top

[T57] Scala：模式匹配
来源：http://ynt.wangshuangyany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://piq.zhaomingkeji.xyz

[T58] Scala：函数定义
来源：http://uqt.tian-w.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dqy.zhixingplan.top

[T59] Scala：循环
来源：http://iss.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://giw.nwbrower.top

[T60] Scala：折叠
来源：http://phm.zdqjudy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://srs.ybcxt.top

================================================================================
来源：http://uiq.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pjh.shuidangran.top

================================================================================
来源：http://qhm.ctjpmb.com

[U01] Py：创建虚拟环境
来源：http://uyf.jinqigfzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://xgn.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://amj.andypj.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vki.zhongyouzk.top

[U03] Py：加载 .env 配置
来源：http://qsg.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ybu.feifeiyinyue.top

[U04] Py：变量调试打印
来源：http://qta.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dix.yuxming.cn

[U05] Py：列表去重且保序
来源：http://sna.svipenyu.cn

list(dict.fromkeys(arr))
来源：http://pmd.gzhubu.top

[U06] Py：合并两个字典
来源：http://fpu.zdqjudy.top

{**a, **b}
来源：http://hnk.snrcjt.cn

[U07] Py：反转字典键值
来源：http://tox.jinghuilouyu.cn

{v: k for k, v in d.items()}
来源：http://bat.tanke756.top

[U08] Py：展平二维列表
来源：http://lbc.shanyushiyangkeji.top

[y for x in nested for y in x]
来源：http://mbv.andypj.xyz

[U09] Py：字典取最大值的键
来源：http://wwd.cashguo.top

max(d, key=d.get)
来源：http://bma.ppjwa.cn

[U10] Py：按值排序字典
来源：http://zlo.yj202588.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mko.hnxiangtu.top

[U11] Py：生成器表达式
来源：http://tvz.zhengqikj.top

(x * 2 for x in arr)
来源：http://jvq.cqqwz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://puw.jinqigufen.top

Counter(arr).most_common(3)
来源：http://jvu.gzhubu.top

[U13] Py：固定长度队列
来源：http://pxn.snrcjt.cn

deque(maxlen=10)
来源：http://hnw.9152youxi.cn

[U14] Py：分组收集到列表
来源：http://vqz.gaohongyu789.top

defaultdict(list)
来源：http://its.52xcode.cn

[U15] Py：高精度计时
来源：http://bbt.sxryk.cn

t = time.perf_counter()
来源：http://ukf.zhaomingkeji.xyz

[U16] Py：命令行参数解析
来源：http://pgd.hongshengwenyu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://grm.hywenlv.cn

[U17] Py：初始化日志
来源：http://zoz.nwbrower.top

logging.basicConfig(level=logging.INFO)
来源：http://sux.yongpay.top

[U18] Py：预编译正则
来源：http://sjz.hesvh.cn

pat = re.compile(r"\d+")
来源：http://ugx.0kj1m.cn

[U19] Py：正则替换带回调
来源：http://tpv.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xmm.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://yjm.jinqigfzy.top

@functools.lru_cache(maxsize=None)
来源：http://hny.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://jeh.uphjek.com

@contextlib.contextmanager
来源：http://hvy.wangdashe.top

[U22] Py：矩阵转置
来源：http://qiy.xziqi.cn

list(zip(*m))
来源：http://yfe.jianghu66.top

[U23] Py：分块读取大文件
来源：http://wet.52xcode.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uhp.fktsv.cn

[U24] Py：路径操作
来源：http://dgj.ppjwa.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sgy.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://fwt.yonumen.top

csv.DictReader(f)
来源：http://crv.shuidangran.top

[U26] Py：并发下载
来源：http://ngi.birdmap.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dpv.jqgfzy.top

[U27] Py：异步 HTTP
来源：http://bcx.yj20258888.top

aiohttp.ClientSession() 配合 async with
来源：http://zdd.shanyushiyangkeji.top

[U28] Py：类型别名
来源：http://tel.xziqi.cn

UserId = int
来源：http://mya.yuanzhike.top

[U29] Py：属性校验
来源：http://gbw.gogol.net.cn

@property 与 @x.setter 配合
来源：http://kxv.ppjwa.cn

[U30] Py：数据类
来源：http://dgm.fzhhl.top

@dataclass(slots=True)
来源：http://miu.gaohongyu789.top

[U31] Py：单测
来源：http://ufv.hcnkem.com

python -m pytest -q
来源：http://tsw.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://odb.zdbjq.cn

ruff format . && ruff check --fix .
来源：http://zrx.jyoumei.cn

[U33] Py：打包发布
来源：http://ozf.52xcode.cn

python -m build  （依赖 pyproject.toml）
来源：http://ejd.zhengqikj.top

[U34] Py：判断编码
来源：http://zoq.shanyushiyangtech.top

chardet.detect(raw)
来源：http://gta.ybcxt.top

[U35] Py：发送邮件
来源：http://zgl.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tut.cashguo.top

[U36] Py：定时任务
来源：http://siz.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://dwt.jiagoushi.top

[U37] Py：读写 Excel
来源：http://zcc.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://txo.dashuyun.cn

[U38] Py：获取脚本所在目录
来源：http://qyw.andypj.xyz

Path(__file__).resolve().parent
来源：http://psu.yfazqb.com

[U39] Py：判断是否在交互环境
来源：http://tpv.nanxinkj.top

sys.stdout.isatty()
来源：http://ruq.sjlbkw.cn

[U40] Py：打印到标准错误
来源：http://aqs.zhengqikj.top

print("err", file=sys.stderr)
来源：http://rgx.yuxming.cn

[U41] PHP：初始化 Composer 项目
来源：http://guz.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lah.chenzaomai.com

[U42] PHP：PSR-4 自动加载
来源：http://dsj.yangfankeji.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hxi.ctjpmb.com

[U43] PHP：声明命名空间
来源：http://uut.yj20258888.top

namespace App\Http;
来源：http://byn.nwbrower.top

[U44] PHP：开启严格类型
来源：http://nkb.sjlbkw.cn

declare(strict_types=1);
来源：http://zna.gotoacloud.top

[U45] PHP：类型声明与返回类型
来源：http://yhq.xuetiantiany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kfy.yonumen.top

[U46] PHP：可空类型
来源：http://qme.hnxiangtu.top

?string $name = null
来源：http://nkf.xinyue.icu

[U47] PHP：联合类型
来源：http://dvp.jlsjyb.cn

int|string $id
来源：http://tzj.ctjpmb.com

[U48] PHP：纯枚举
来源：http://asc.xingfuxueyuan.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pnz.gaohongyu789.top

[U49] PHP：只读属性
来源：http://lgq.0kj1m.cn

public readonly string $name
来源：http://vpw.uphjek.com

[U50] PHP：构造器属性提升
来源：http://ori.vqdsnc.cn

public function __construct(private int $id) {}
来源：http://vzp.chenjidiqi.icu

[U51] PHP：数组解构
来源：http://xxv.shanyushiyangkeji.top

[$a, $b] = $arr;
来源：http://sop.cqqwz.cn

[U52] PHP：箭头函数
来源：http://ypy.zycfv.cn

$double = fn($x) => $x * 2;
来源：http://dhu.shanyushiyangtech.top


<!-- 参考信息 -->