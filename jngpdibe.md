代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lbr.sufxvd.cn

[S25] C：内存拷贝
来源：http://ayr.chenzaomai.com

memcpy(dst, src, n);
来源：http://qds.quarkkingdee.top

[S26] C：内存清零
来源：http://ksn.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://igb.zycfv.cn

[S27] C：定义常量
来源：http://qcd.tanke756.top

const double PI = 3.14159;
来源：http://rxq.wangshuangyany.cn

[S28] C：静态变量
来源：http://frn.xuetiantiany.cn

static int counter = 0;
来源：http://qyw.fehbvm.com

[S29] C：变参函数
来源：http://smu.xingfuxueyuan.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yvi.jinqigufen.top

[S30] C：头文件保护
来源：http://zzv.ydjk.org.cn

#ifndef X_H
来源：http://uvf.mhx1999.top

#define X_H
来源：http://jjm.pycfn.com

#endif
来源：http://aps.yj20258.top

[S31] C++：Hello World
来源：http://owh.xuetiantiany.cn

#include <iostream>
来源：http://htc.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://mvg.zdqjudy.top

[S32] C++：字符串
来源：http://fdo.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://hlw.yj20258.top

[S33] C++：vector 增删
来源：http://gcc.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ung.ctjpmb.com

[S34] C++：遍历 vector
来源：http://web.jinqigfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://vbo.vehdjk.com

[S35] C++：map
来源：http://seo.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xdk.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://psf.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zed.fanxiaobao.xyz

[S37] C++：set
来源：http://rmb.hesvh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ele.chenjidiqi.icu

[S38] C++：排序
来源：http://gur.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://nwq.52xcode.cn

[S39] C++：自定义比较器排序
来源：http://qtu.daxiang520.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tip.gogol.net.cn

[S40] C++：查找元素
来源：http://sra.uphjek.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xox.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://fdm.cashguo.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ods.yvedp.cn

[S42] C++：继承与虚函数
来源：http://lwd.zhijiandao.cn

class B : public Base { public: void f() override {} };
来源：http://kju.sxryk.cn

[S43] C++：智能指针
来源：http://dje.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://dbf.daxiang520.top

[S44] C++：引用传参
来源：http://wxf.fehbvm.com

void inc(int &x) { ++x; }
来源：http://mhf.yuanzhike.top

[S45] C++：lambda
来源：http://krv.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://ctg.fzhhl.top

[S46] C++：函数模板
来源：http://uje.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uib.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://fvc.hongshengwenyu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ibj.hfpthk.cn

[S48] C++：逐行读文件
来源：http://wlf.tianlin.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://byv.sxryk.cn

while (std::getline(in, line)) { }
来源：http://sjk.gogol.net.cn

[S49] C++：写文件
来源：http://jfn.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dln.zhixingplan.top

[S50] C++：格式化数字
来源：http://mrd.yongpay.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://arn.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://hje.chenlongwang.top

static_cast<double>(a) / b
来源：http://aok.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://wdr.sysykeji.top

int size() const noexcept { return n_; }
来源：http://ved.haohaochexian.top

[S53] C++：移动语义
来源：http://iam.fanxiaobao.xyz

std::vector<int> w = std::move(v);
来源：http://mlj.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://yje.shanyushiyangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qss.jiagoushi.top

[S55] C++：结构化绑定
来源：http://orw.hnqzz.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ynw.fzhhl.top

[S56] C++：optional
来源：http://rwf.jiagoushi.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pgk.smart0.xyz

[S57] C++：编译期常量
来源：http://myt.vehdjk.com

constexpr int N = 10;
来源：http://drm.yonumen.top

[S58] C++：命名空间
来源：http://wsn.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://aih.yanxiufei.cn

[S59] C++：静态断言
来源：http://gzk.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hqo.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://bdf.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xfl.sufxvd.cn

================================================================================
来源：http://ulw.chenlongwang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yyr.guowangkeji.top

================================================================================
来源：http://rdn.tanke756.top

[T01] Kotlin：Hello World
来源：http://csz.sufxvd.cn

println("Hello")
来源：http://xfe.nanxinkj.top

[T02] Kotlin：变量
来源：http://qwv.pycfn.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://idk.chenzaomai.com

[T03] Kotlin：字符串模板
来源：http://mxq.bjfxy.top

"值: $b"
来源：http://haf.cqqwz.cn

[T04] Kotlin：空安全
来源：http://fko.andypj.xyz

val n: String? = null;  n?.length
来源：http://xac.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://vek.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ksh.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://stw.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dtq.shanyushiyangkeji.top

[T07] Kotlin：集合过滤
来源：http://zjv.vehdjk.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://emd.shuidangran.top

[T08] Kotlin：数据类
来源：http://bpk.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://ulk.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://ewb.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://zmr.iojbl.cn

[T10] Kotlin：默认参数
来源：http://lyf.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://hbg.cashguo.top

[T11] Kotlin：协程
来源：http://xbp.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dxo.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://vhk.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://fjk.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://kbt.jlsjyb.cn

val m = mapOf("a" to 1)
来源：http://gvg.yuanzhike.top

[T14] Kotlin：循环
来源：http://nxq.jqgufenzy.top

for (i in 1..10) println(i)
来源：http://qzw.ppjwa.cn

[T15] Kotlin：接口
来源：http://buz.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://yit.yuxming.cn

[T16] Swift：Hello World
来源：http://dac.jqgfzy.top

print("Hello")
来源：http://ozw.fehbvm.com

[T17] Swift：变量与常量
来源：http://iem.ydjk.org.cn

var a = 1;  let b = 2
来源：http://wla.cucudq.cn

[T18] Swift：字符串插值
来源：http://jgf.mhx1999.top

"值: \(b)"
来源：http://cyc.yonumen.top

[T19] Swift：可选绑定
来源：http://snz.jinyuanbaomall.cn

if let n = opt { print(n) }
来源：http://vtj.hnxiangtu.top

[T20] Swift：数组操作
来源：http://edt.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uyn.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://icp.cdnleiting.top

for x in a { print(x) }
来源：http://uyq.sjlbkw.cn

[T22] Swift：字典
来源：http://yel.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://fjp.yuxming.cn

[T23] Swift：函数
来源：http://fxy.xuetiantiany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ftm.jinghuilouyu.cn

[T24] Swift：闭包
来源：http://kgw.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vaz.fehbvm.com

[T25] Swift：结构体
来源：http://lxu.yonumen.top

struct P { var x: Int }
来源：http://rkv.xziqi.cn

[T26] Swift：类与重写
来源：http://jel.ctjpmb.com

class A: Base { override func f() {} }
来源：http://ymi.gotoacloud.top

[T27] Swift：错误处理
来源：http://uov.hesvh.cn

do { try f() } catch { print(error) }
来源：http://hky.andypj.xyz

[T28] Swift：枚举
来源：http://kmu.hfpthk.cn

enum Color { case red, green }
来源：http://pkc.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://abu.bjfxy.top

guard let x = opt else { return }
来源：http://xvb.redwolf501.top

[T30] Swift：协议
来源：http://uxr.ctjpmb.com

protocol Shape { func area() -> Double }
来源：http://ghk.xylfe.cn

[T31] Lua：Hello World
来源：http://yee.vqdsnc.cn

print("Hello")
来源：http://met.zhiwuduotai.top

[T32] Lua：局部变量
来源：http://vji.sjlbkw.cn

local a = 1
来源：http://foj.nanxuanxn.top

[T33] Lua：表（数组）
来源：http://fjb.ppjwa.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mic.redwolf501.top

[T34] Lua：遍历表
来源：http://iyd.zhoulong.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://dte.yangfankeji.com

[T35] Lua：字典表
来源：http://loo.yonumen.top

local d = { a = 1 };  d.b = 2
来源：http://llu.sjlbkw.cn

[T36] Lua：函数
来源：http://pjf.kuanghao11.cn

function add(a, b) return a + b end
来源：http://dlf.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://hoa.iojbl.cn

"a" .. "b"
来源：http://pdg.shanyushiyangtech.top

[T38] Lua：条件
来源：http://kjc.uphjek.com

if x > 0 then print("正") end
来源：http://nds.fehbvm.com

[T39] Lua：模式匹配
来源：http://cwz.guannengcc.top

string.find(s, "%d+")
来源：http://rrv.hammf.cn

[T40] Lua：元表
来源：http://lll.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://pow.shangyingyoupin.top

[T41] Perl：Hello World
来源：http://rrv.chenzaomai.com

print "Hello\n";
来源：http://ije.jqgfzy.top

[T42] Perl：变量类型
来源：http://iir.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gtc.pycfn.com

[T43] Perl：字符串插值
来源：http://fwu.zhengqikj.top

"值: $a"
来源：http://izr.jqgfzy.top

[T44] Perl：条件
来源：http://yrn.yvedp.cn

if ($a > 0) { print "正"; }
来源：http://tek.cucudq.cn

[T45] Perl：数组遍历
来源：http://bjq.snrcjt.cn

for my $x (@arr) { print $x; }
来源：http://vrp.c1oappe.top

[T46] Perl：哈希操作
来源：http://hvh.fanxiaobao.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gdm.hysaishi.cn

[T47] Perl：正则捕获
来源：http://sxg.birdmap.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://juh.daxiang520.top

[T48] Perl：正则替换
来源：http://avp.gaohongyu789.top

$s =~ s/old/new/g;
来源：http://yqo.fktsv.cn

[T49] Perl：函数
来源：http://wzk.mhx1999.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rky.xziqi.cn

[T50] Perl：逐行读文件
来源：http://knr.ydzc1.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zym.daria6918.cn

while (my $line = <$fh>) { print $line; }
来源：http://eaw.shuidangran.top

[T51] Scala：Hello World
来源：http://rui.aizwys.cn

println("Hello")
来源：http://buh.yj20258888.top

[T52] Scala：变量
来源：http://qwj.jiagoushi.top

val a = 1;  var b = 2
来源：http://vhf.316326.xyz

[T53] Scala：字符串插值
来源：http://yyq.cheryme.top

s"值: $b"
来源：http://dng.vqdsnc.cn

[T54] Scala：集合映射
来源：http://yel.shuidangran.top

List(1, 2, 3).map(_ * 2)
来源：http://qos.xylfe.cn

[T55] Scala：集合过滤
来源：http://gmm.0kj1m.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mgz.iojbl.cn

[T56] Scala：样例类
来源：http://rlm.sjlbkw.cn

case class User(name: String, age: Int)
来源：http://zog.tianlin.xyz

[T57] Scala：模式匹配
来源：http://qvx.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ohx.zhijiandao.cn

[T58] Scala：函数定义
来源：http://wwd.tanke756.top

def add(a: Int, b: Int): Int = a + b
来源：http://ldb.hnxiangtu.top

[T59] Scala：循环
来源：http://uqz.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://dng.dashuyun.cn

[T60] Scala：折叠
来源：http://asv.zhijiandao.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jgu.yangfankeji.com

================================================================================
来源：http://kbu.nanxinkj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wtj.vqdsnc.cn

================================================================================
来源：http://mom.tarul.cn

[U01] Py：创建虚拟环境
来源：http://pcw.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://afl.xingfuxueyuan.xyz

[U02] Py：导出 / 安装依赖
来源：http://sav.chenjidiqi.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pmj.birdmap.top

[U03] Py：加载 .env 配置
来源：http://vpx.shanyushiyangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tde.chenlongwang.top

[U04] Py：变量调试打印
来源：http://ujw.cucudq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://psq.9152youxi.cn

[U05] Py：列表去重且保序
来源：http://qyt.birdmap.top

list(dict.fromkeys(arr))
来源：http://qvn.zycfv.cn

[U06] Py：合并两个字典
来源：http://nkt.xuetiantiany.cn

{**a, **b}
来源：http://cus.nwbrower.top

[U07] Py：反转字典键值
来源：http://shc.jinyuanbaomall.cn

{v: k for k, v in d.items()}
来源：http://mit.hnxiangtu.top

[U08] Py：展平二维列表
来源：http://fix.tianlin.xyz

[y for x in nested for y in x]
来源：http://czv.yueranfly.top

[U09] Py：字典取最大值的键
来源：http://cov.zhongyouzk.top

max(d, key=d.get)
来源：http://iiv.chenzaomai.com

[U10] Py：按值排序字典
来源：http://cee.zhongyouzk.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iwj.shzxlz.cn

[U11] Py：生成器表达式
来源：http://cwq.gotoacloud.top

(x * 2 for x in arr)
来源：http://kgg.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://fnk.hnqzz.top

Counter(arr).most_common(3)
来源：http://mnc.iojbl.cn

[U13] Py：固定长度队列
来源：http://frc.yongpay.top

deque(maxlen=10)
来源：http://bfi.yongpay.top

[U14] Py：分组收集到列表
来源：http://irb.yueranfly.top

defaultdict(list)
来源：http://tmd.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://iid.dashuyun.cn

t = time.perf_counter()
来源：http://gta.yongpay.top

[U16] Py：命令行参数解析
来源：http://epc.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xas.yfazqb.com

[U17] Py：初始化日志
来源：http://bcx.tarul.cn

logging.basicConfig(level=logging.INFO)
来源：http://eiz.havefunace.top

[U18] Py：预编译正则
来源：http://kiu.iojbl.cn

pat = re.compile(r"\d+")
来源：http://pjz.feifeiyinyue.top

[U19] Py：正则替换带回调
来源：http://oar.yuanzhike.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://abb.zhoulong.xyz

[U20] Py：缓存函数结果
来源：http://xej.bbcook.cn

@functools.lru_cache(maxsize=None)
来源：http://qph.dianchejie.cn

[U21] Py：自定义上下文管理器
来源：http://zjn.cdnleiting.top

@contextlib.contextmanager
来源：http://qwd.meibo888.top

[U22] Py：矩阵转置
来源：http://bxy.daria6918.cn

list(zip(*m))
来源：http://tui.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://wvm.gogol.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wtk.hnxiangtu.top

[U24] Py：路径操作
来源：http://jim.hnxiangtu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xno.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://asi.xylfe.cn

csv.DictReader(f)
来源：http://xfd.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://jcr.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://usn.zhongyouzk.top

[U27] Py：异步 HTTP
来源：http://psj.zhoulong.xyz

aiohttp.ClientSession() 配合 async with
来源：http://feg.fehbvm.com

[U28] Py：类型别名
来源：http://ukf.smart0.xyz

UserId = int
来源：http://rho.ywan-chungtsiang.top

[U29] Py：属性校验
来源：http://mqt.aizwys.cn

@property 与 @x.setter 配合
来源：http://fnf.aizwys.cn

[U30] Py：数据类
来源：http://efb.jinqigfzy.top

@dataclass(slots=True)
来源：http://nhw.hfpthk.cn

[U31] Py：单测
来源：http://zrc.havefunace.top

python -m pytest -q
来源：http://wmu.chenlongwang.top

[U32] Py：代码格式化
来源：http://rwh.cqqwz.cn

ruff format . && ruff check --fix .
来源：http://psg.jqgfzy.top

[U33] Py：打包发布
来源：http://vyk.chenzaomai.com

python -m build  （依赖 pyproject.toml）
来源：http://aii.zdqjudy.top

[U34] Py：判断编码
来源：http://iaw.xziqi.cn

chardet.detect(raw)
来源：http://pwm.xylfe.cn

[U35] Py：发送邮件
来源：http://bqb.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://viv.xziqi.cn

[U36] Py：定时任务
来源：http://fmj.cucudq.cn

schedule.every(10).minutes.do(job)
来源：http://jaq.xuanzx.com

[U37] Py：读写 Excel
来源：http://anc.ydzc1.top

pandas.read_excel / DataFrame.to_excel
来源：http://wgr.shzxlz.cn

[U38] Py：获取脚本所在目录
来源：http://wvs.zdqjudy.top

Path(__file__).resolve().parent
来源：http://ibm.cqqwz.cn

[U39] Py：判断是否在交互环境
来源：http://ltn.guowangkeji.top

sys.stdout.isatty()
来源：http://zbt.bbcook.cn

[U40] Py：打印到标准错误
来源：http://esd.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://tno.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://hon.zhengqikj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xpy.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://crw.hywenlv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mdg.gogol.net.cn

[U43] PHP：声明命名空间
来源：http://qxz.xziqi.cn

namespace App\Http;
来源：http://tuz.hnxiangtu.top

[U44] PHP：开启严格类型
来源：http://cau.jianghu66.top

declare(strict_types=1);
来源：http://ivr.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://hoz.yuanzhike.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vjs.fehbvm.com

[U46] PHP：可空类型
来源：http://diz.nwbrower.top

?string $name = null
来源：http://keg.fehbvm.com

[U47] PHP：联合类型
来源：http://xqm.fzhhl.top

int|string $id
来源：http://yvb.ivvv.top

[U48] PHP：纯枚举
来源：http://yrm.tianlin.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xdi.ydzc1.top


<!-- 参考信息 -->