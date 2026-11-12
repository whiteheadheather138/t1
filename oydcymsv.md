代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qds.guowangkeji.top

[S25] C：内存拷贝
来源：http://etx.zdbjq.cn

memcpy(dst, src, n);
来源：http://tdk.aizwys.cn

[S26] C：内存清零
来源：http://pto.fanxiaobao.xyz

memset(a, 0, sizeof a);
来源：http://uoe.gzhubu.top

[S27] C：定义常量
来源：http://wwo.birdmap.top

const double PI = 3.14159;
来源：http://tyk.chenlongwang.top

[S28] C：静态变量
来源：http://wcn.fktsv.cn

static int counter = 0;
来源：http://ooa.andypj.xyz

[S29] C：变参函数
来源：http://rzw.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ivc.yj202588.top

[S30] C：头文件保护
来源：http://yif.tanke756.top

#ifndef X_H
来源：http://exv.andypj.xyz

#define X_H
来源：http://hzj.yuxming.cn

#endif
来源：http://mie.gogol.net.cn

[S31] C++：Hello World
来源：http://wso.ppjwa.cn

#include <iostream>
来源：http://hkf.fengsongda.top

int main() { std::cout << "Hello\n"; }
来源：http://pzu.fehbvm.com

[S32] C++：字符串
来源：http://gbg.pycfn.com

std::string s = "hi";  s += "!";
来源：http://wnq.iojbl.cn

[S33] C++：vector 增删
来源：http://qko.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xvf.meibo888.top

[S34] C++：遍历 vector
来源：http://vig.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://otl.jlsjyb.cn

[S35] C++：map
来源：http://eop.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qbo.ybcxt.top

[S36] C++：unordered_map
来源：http://cnk.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://znt.guannengcc.top

[S37] C++：set
来源：http://hqd.9152youxi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gfu.yj20258888.top

[S38] C++：排序
来源：http://hby.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://jka.cheryme.top

[S39] C++：自定义比较器排序
来源：http://wjt.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bfb.fzhhl.top

[S40] C++：查找元素
来源：http://kze.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kok.pengpengdd.cyou

[S41] C++：类与构造函数
来源：http://jtz.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wsn.ydjk.org.cn

[S42] C++：继承与虚函数
来源：http://vgq.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://ulc.cucudq.cn

[S43] C++：智能指针
来源：http://esi.xylfe.cn

auto p = std::make_unique<int>(5);
来源：http://gvv.ctjpmb.com

[S44] C++：引用传参
来源：http://piu.jlsjyb.cn

void inc(int &x) { ++x; }
来源：http://fls.fzhhl.top

[S45] C++：lambda
来源：http://ksh.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jnr.hnqzz.top

[S46] C++：函数模板
来源：http://edl.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bjo.haohaochexian.top

[S47] C++：结构化绑定遍历
来源：http://uba.pycfn.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ijv.daxiang520.top

[S48] C++：逐行读文件
来源：http://ajz.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://csm.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://nij.iojbl.cn

[S49] C++：写文件
来源：http://ylf.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tkc.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://psw.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://czy.dashuyun.cn

[S51] C++：显式类型转换
来源：http://mmy.jqgfzy.top

static_cast<double>(a) / b
来源：http://fmt.havefunace.top

[S52] C++：const 与 noexcept
来源：http://pyj.jinqigfzy.top

int size() const noexcept { return n_; }
来源：http://hza.yongpay.top

[S53] C++：移动语义
来源：http://ldf.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://gis.jinqigufen.top

[S54] C++：异常处理
来源：http://ayy.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://anp.yj20258888.top

[S55] C++：结构化绑定
来源：http://uai.bbcook.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://huy.yonumen.top

[S56] C++：optional
来源：http://ign.hongshengwenyu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ymj.hesvh.cn

[S57] C++：编译期常量
来源：http://dmh.xziqi.cn

constexpr int N = 10;
来源：http://ikb.mhx1999.top

[S58] C++：命名空间
来源：http://aor.zhijiandao.cn

namespace ns { int f() { return 1; } }
来源：http://lkj.pycfn.com

[S59] C++：静态断言
来源：http://khe.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qsr.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://zcb.cdnleiting.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aoi.zhijiandao.cn

================================================================================
来源：http://ajd.redwolf501.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ouq.nanxuanxn.top

================================================================================
来源：http://owt.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://qse.jinghuilouyu.cn

println("Hello")
来源：http://chk.yj20258888.top

[T02] Kotlin：变量
来源：http://oaa.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tls.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://qvz.xingfuxueyuan.xyz

"值: $b"
来源：http://mco.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://zib.yj202588.top

val n: String? = null;  n?.length
来源：http://cwr.nanxinkj.top

[T05] Kotlin：when 表达式
来源：http://mxp.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gns.zdqjudy.top

[T06] Kotlin：集合映射
来源：http://ugf.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nwo.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://rzc.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hze.xylfe.cn

[T08] Kotlin：数据类
来源：http://usw.zhaomingkeji.xyz

data class User(val name: String, val age: Int)
来源：http://hzp.havefunace.top

[T09] Kotlin：扩展函数
来源：http://vwn.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://dmf.hnqzz.top

[T10] Kotlin：默认参数
来源：http://aqx.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cyx.sysykeji.top

[T11] Kotlin：协程
来源：http://iga.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://vyj.cdnleiting.top

[T12] Kotlin：解构声明
来源：http://czk.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://fdh.hnxiangtu.top

[T13] Kotlin：只读 Map
来源：http://ygd.ydzc1.top

val m = mapOf("a" to 1)
来源：http://azo.zhengqikj.top

[T14] Kotlin：循环
来源：http://sjb.vehdjk.com

for (i in 1..10) println(i)
来源：http://hzi.9152youxi.cn

[T15] Kotlin：接口
来源：http://qiz.dianchejie.cn

interface Shape { fun area(): Double }
来源：http://fak.ehwqpu.com

[T16] Swift：Hello World
来源：http://fsg.sxryk.cn

print("Hello")
来源：http://oom.redwolf501.top

[T17] Swift：变量与常量
来源：http://ktf.yueranfly.top

var a = 1;  let b = 2
来源：http://tke.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://eba.haohaochexian.top

"值: \(b)"
来源：http://gby.snrcjt.cn

[T19] Swift：可选绑定
来源：http://cho.birdmap.top

if let n = opt { print(n) }
来源：http://bbe.ydjk.org.cn

[T20] Swift：数组操作
来源：http://fog.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://zyp.ydzc1.top

[T21] Swift：遍历
来源：http://jum.iojbl.cn

for x in a { print(x) }
来源：http://cck.ydzc1.top

[T22] Swift：字典
来源：http://sxc.jinghuilouyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qoq.hywenlv.cn

[T23] Swift：函数
来源：http://coq.tianlin.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aaq.svipenyu.cn

[T24] Swift：闭包
来源：http://tvr.jlsjyb.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://msj.ybcxt.top

[T25] Swift：结构体
来源：http://svc.yuanzhike.top

struct P { var x: Int }
来源：http://oxl.yonumen.top

[T26] Swift：类与重写
来源：http://lvj.dianchejie.cn

class A: Base { override func f() {} }
来源：http://uwp.zhoulong.xyz

[T27] Swift：错误处理
来源：http://yuv.hnqzz.top

do { try f() } catch { print(error) }
来源：http://cag.gogol.net.cn

[T28] Swift：枚举
来源：http://vdd.daxiang520.top

enum Color { case red, green }
来源：http://xet.shuidangran.top

[T29] Swift：guard 提前返回
来源：http://ucg.zhijiandao.cn

guard let x = opt else { return }
来源：http://ynz.wangshuangyany.cn

[T30] Swift：协议
来源：http://jhn.yanxiufei.cn

protocol Shape { func area() -> Double }
来源：http://eiu.xuetiantiany.cn

[T31] Lua：Hello World
来源：http://bmr.sweek.top

print("Hello")
来源：http://icl.wangshuangyany.cn

[T32] Lua：局部变量
来源：http://mmt.ywan-chungtsiang.top

local a = 1
来源：http://qsv.pycfn.com

[T33] Lua：表（数组）
来源：http://gfb.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vir.yonumen.top

[T34] Lua：遍历表
来源：http://hru.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gpa.birdmap.top

[T35] Lua：字典表
来源：http://xkp.hcnkem.com

local d = { a = 1 };  d.b = 2
来源：http://qcn.316326.xyz

[T36] Lua：函数
来源：http://akb.fengsongda.top

function add(a, b) return a + b end
来源：http://aih.xinyue.icu

[T37] Lua：字符串拼接
来源：http://cmr.chenjidiqi.icu

"a" .. "b"
来源：http://kzp.yuxming.cn

[T38] Lua：条件
来源：http://qme.yj20258888.top

if x > 0 then print("正") end
来源：http://jmy.wangdashe.top

[T39] Lua：模式匹配
来源：http://hmu.fanxiaobao.xyz

string.find(s, "%d+")
来源：http://yka.havefunace.top

[T40] Lua：元表
来源：http://pjw.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://uzn.yj20258888.top

[T41] Perl：Hello World
来源：http://uxv.chenzaomai.com

print "Hello\n";
来源：http://ero.xylfe.cn

[T42] Perl：变量类型
来源：http://yhk.xinyue.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oyt.zhengqikj.top

[T43] Perl：字符串插值
来源：http://gah.ybcxt.top

"值: $a"
来源：http://ewq.zdqjudy.top

[T44] Perl：条件
来源：http://ipj.mhx1999.top

if ($a > 0) { print "正"; }
来源：http://saa.shangyingyoupin.top

[T45] Perl：数组遍历
来源：http://gal.sweek.top

for my $x (@arr) { print $x; }
来源：http://umw.tanke756.top

[T46] Perl：哈希操作
来源：http://sec.smart0.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ehd.ppjwa.cn

[T47] Perl：正则捕获
来源：http://wjk.jinqigufen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jog.gogol.net.cn

[T48] Perl：正则替换
来源：http://jev.wangdashe.top

$s =~ s/old/new/g;
来源：http://xkk.sweek.top

[T49] Perl：函数
来源：http://txz.epnwcf.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://faq.hcnkem.com

[T50] Perl：逐行读文件
来源：http://lch.zhoulong.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://bxy.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://nly.vehdjk.com

[T51] Scala：Hello World
来源：http://gqe.hfpthk.cn

println("Hello")
来源：http://xsz.ydjk.org.cn

[T52] Scala：变量
来源：http://arn.bjfxy.top

val a = 1;  var b = 2
来源：http://pce.hfpthk.cn

[T53] Scala：字符串插值
来源：http://ryd.nanxuanxn.top

s"值: $b"
来源：http://shq.gotoacloud.top

[T54] Scala：集合映射
来源：http://sve.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://rgo.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://epj.nwbrower.top

List(1, 2, 3).filter(_ > 1)
来源：http://vlw.dianchejie.cn

[T56] Scala：样例类
来源：http://lju.pycfn.com

case class User(name: String, age: Int)
来源：http://ugc.zycfv.cn

[T57] Scala：模式匹配
来源：http://jjk.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://acz.xziqi.cn

[T58] Scala：函数定义
来源：http://qnu.daxiang520.top

def add(a: Int, b: Int): Int = a + b
来源：http://yku.dashuyun.cn

[T59] Scala：循环
来源：http://hvk.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://mhb.sxryk.cn

[T60] Scala：折叠
来源：http://uxp.hcnkem.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fsn.wangshuangyany.cn

================================================================================
来源：http://jqf.cqqwz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vcz.svipenyu.cn

================================================================================
来源：http://tqa.nwbrower.top

[U01] Py：创建虚拟环境
来源：http://rog.cdnleiting.top

python -m venv .venv && source .venv/bin/activate
来源：http://mfa.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://afl.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ovw.sxryk.cn

[U03] Py：加载 .env 配置
来源：http://shd.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://vhn.pycfn.com

[U04] Py：变量调试打印
来源：http://zqc.uphjek.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sgl.chenjidiqi.icu

[U05] Py：列表去重且保序
来源：http://koj.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://bca.zdbjq.cn

[U06] Py：合并两个字典
来源：http://eob.jiagoushi.top

{**a, **b}
来源：http://bdm.jinqigfzy.top

[U07] Py：反转字典键值
来源：http://pxe.hnqzz.top

{v: k for k, v in d.items()}
来源：http://prv.yfazqb.com

[U08] Py：展平二维列表
来源：http://jvx.zhixingplan.top

[y for x in nested for y in x]
来源：http://wgg.epnwcf.com

[U09] Py：字典取最大值的键
来源：http://jrt.guowangkeji.top

max(d, key=d.get)
来源：http://yci.gogol.net.cn

[U10] Py：按值排序字典
来源：http://qrl.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rbz.smart0.xyz

[U11] Py：生成器表达式
来源：http://gfk.ybcxt.top

(x * 2 for x in arr)
来源：http://wyr.jinqigufen.top

[U12] Py：取出现最多的 3 个元素
来源：http://gdo.yj202588.top

Counter(arr).most_common(3)
来源：http://lmv.fehbvm.com

[U13] Py：固定长度队列
来源：http://bbl.yuxming.cn

deque(maxlen=10)
来源：http://bfc.wangshuangyany.cn

[U14] Py：分组收集到列表
来源：http://lsu.yuanzhike.top

defaultdict(list)
来源：http://xsa.jinqigufen.top

[U15] Py：高精度计时
来源：http://qgt.yongpay.top

t = time.perf_counter()
来源：http://aht.yj202588.top

[U16] Py：命令行参数解析
来源：http://evf.yvedp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kvb.sysykeji.top

[U17] Py：初始化日志
来源：http://npw.zhaomingkeji.xyz

logging.basicConfig(level=logging.INFO)
来源：http://eep.sweek.top

[U18] Py：预编译正则
来源：http://kmi.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://ofr.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://aum.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dze.epnwcf.com

[U20] Py：缓存函数结果
来源：http://xzt.cashguo.top

@functools.lru_cache(maxsize=None)
来源：http://oyq.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://ona.shuidangran.top

@contextlib.contextmanager
来源：http://yuv.sjlbkw.cn

[U22] Py：矩阵转置
来源：http://drz.yvedp.cn

list(zip(*m))
来源：http://iae.sjlbkw.cn

[U23] Py：分块读取大文件
来源：http://ock.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://max.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://jgr.zhaomingkeji.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kdl.c1oappe.top

[U25] Py：CSV 按字典读
来源：http://req.vehdjk.com

csv.DictReader(f)
来源：http://evd.cqqwz.cn

[U26] Py：并发下载
来源：http://ewp.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gwo.ywan-chungtsiang.top

[U27] Py：异步 HTTP
来源：http://kbi.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://amh.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://ssl.xylfe.cn

UserId = int
来源：http://suw.yongpay.top

[U29] Py：属性校验
来源：http://wui.cqqwz.cn

@property 与 @x.setter 配合
来源：http://hta.hongshengwenyu.top

[U30] Py：数据类
来源：http://olw.jiagoushi.top

@dataclass(slots=True)
来源：http://yiy.yonumen.top

[U31] Py：单测
来源：http://wlc.aibaodan.cn

python -m pytest -q
来源：http://rbr.bbcook.cn

[U32] Py：代码格式化
来源：http://alg.yvedp.cn

ruff format . && ruff check --fix .
来源：http://zfo.yuxming.cn

[U33] Py：打包发布
来源：http://jhc.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://dsu.xuetiantiany.cn

[U34] Py：判断编码
来源：http://yks.ivvv.top

chardet.detect(raw)
来源：http://avh.fktsv.cn

[U35] Py：发送邮件
来源：http://bwg.xingfuxueyuan.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gml.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://kto.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://mgn.jinqigfzy.top

[U37] Py：读写 Excel
来源：http://fpa.jlsjyb.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sso.fanxiaobao.xyz

[U38] Py：获取脚本所在目录
来源：http://rpe.ppjwa.cn

Path(__file__).resolve().parent
来源：http://dur.zhiwuduotai.top

[U39] Py：判断是否在交互环境
来源：http://egu.mhx1999.top

sys.stdout.isatty()
来源：http://qwn.daxiang520.top

[U40] Py：打印到标准错误
来源：http://tzy.cashguo.top

print("err", file=sys.stderr)
来源：http://dbq.yj202588.top

[U41] PHP：初始化 Composer 项目
来源：http://uyh.jianghu66.top

composer init;  composer require guzzlehttp/guzzle
来源：http://kjj.birdmap.top

[U42] PHP：PSR-4 自动加载
来源：http://ywc.yanxiufei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://stf.fktsv.cn

[U43] PHP：声明命名空间
来源：http://thq.shuidangran.top

namespace App\Http;
来源：http://gnq.dashuyun.cn

[U44] PHP：开启严格类型
来源：http://oxb.jqgufenzy.top

declare(strict_types=1);
来源：http://unf.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://zdy.ybcxt.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xro.svipenyu.cn

[U46] PHP：可空类型
来源：http://aei.smart0.xyz

?string $name = null
来源：http://qvh.wangshuangyany.cn

[U47] PHP：联合类型
来源：http://zpj.snrcjt.cn

int|string $id
来源：http://oui.cucudq.cn

[U48] PHP：纯枚举
来源：http://tth.sxryk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nwn.zhengqikj.top


<!-- 参考信息 -->