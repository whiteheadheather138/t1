代发 wailian999

memset(a, 0, sizeof a);
来源：http://roq.andypj.xyz

[S27] C：定义常量
来源：http://qxa.zhixingplan.top

const double PI = 3.14159;
来源：http://xuf.ctjpmb.com

[S28] C：静态变量
来源：http://hik.nanxuanxn.top

static int counter = 0;
来源：http://aap.aizwys.cn

[S29] C：变参函数
来源：http://nrg.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://klu.jianghu66.top

[S30] C：头文件保护
来源：http://aai.pycfn.com

#ifndef X_H
来源：http://vzb.meibo888.top

#define X_H
来源：http://ggj.yvedp.cn

#endif
来源：http://omq.yj202588.top

[S31] C++：Hello World
来源：http://wct.hammf.cn

#include <iostream>
来源：http://xxe.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://pgp.cashguo.top

[S32] C++：字符串
来源：http://kcg.ydzc1.top

std::string s = "hi";  s += "!";
来源：http://qvx.dianchejie.cn

[S33] C++：vector 增删
来源：http://wxo.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xzt.guowangkeji.top

[S34] C++：遍历 vector
来源：http://lyy.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://awq.shanyushiyangtech.top

[S35] C++：map
来源：http://kds.yuanzhike.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://khc.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://bcl.bbcook.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://knw.hysaishi.cn

[S37] C++：set
来源：http://bbo.smart0.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yla.haohaochexian.top

[S38] C++：排序
来源：http://uko.wangshuangyany.cn

std::sort(v.begin(), v.end());
来源：http://tyi.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://vyo.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zvs.zdbjq.cn

[S40] C++：查找元素
来源：http://lbm.xuanzx.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cnu.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://kvu.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wcp.tanke756.top

[S42] C++：继承与虚函数
来源：http://gee.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://osh.shanyushiyangkeji.top

[S43] C++：智能指针
来源：http://zsg.nanxuanxn.top

auto p = std::make_unique<int>(5);
来源：http://umu.fzhhl.top

[S44] C++：引用传参
来源：http://xff.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://urq.ydzc1.top

[S45] C++：lambda
来源：http://wwa.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gby.havefunace.top

[S46] C++：函数模板
来源：http://pua.sweek.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://esm.fktsv.cn

[S47] C++：结构化绑定遍历
来源：http://ump.fengsongda.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zlw.ydzc1.top

[S48] C++：逐行读文件
来源：http://yal.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://vxm.52xcode.cn

while (std::getline(in, line)) { }
来源：http://lgf.sxryk.cn

[S49] C++：写文件
来源：http://hkr.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vai.52xcode.cn

[S50] C++：格式化数字
来源：http://kqc.xziqi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qer.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://pot.cheryme.top

static_cast<double>(a) / b
来源：http://mbj.xingfuxueyuan.xyz

[S52] C++：const 与 noexcept
来源：http://kfr.chenlongwang.top

int size() const noexcept { return n_; }
来源：http://hvj.yangfankeji.com

[S53] C++：移动语义
来源：http://avc.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://zbh.daria6918.cn

[S54] C++：异常处理
来源：http://kac.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://afd.jinqigufen.top

[S55] C++：结构化绑定
来源：http://wfb.ydjk.org.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pvq.feifeiyinyue.top

[S56] C++：optional
来源：http://rvq.yanxiufei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://daw.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://fqk.shzxlz.cn

constexpr int N = 10;
来源：http://ven.jinqigufen.top

[S58] C++：命名空间
来源：http://fnj.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://gnd.ydjk.org.cn

[S59] C++：静态断言
来源：http://zmj.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oxd.daria6918.cn

[S60] C++：遍历并删除元素
来源：http://loz.cheryme.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iwd.bjfxy.top

================================================================================
来源：http://wua.hnqzz.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://teo.hnxiangtu.top

================================================================================
来源：http://bnc.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://mzy.jiagoushi.top

println("Hello")
来源：http://xym.uphjek.com

[T02] Kotlin：变量
来源：http://afh.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bne.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://gvh.cheryme.top

"值: $b"
来源：http://gab.jinqigufen.top

[T04] Kotlin：空安全
来源：http://koo.pycfn.com

val n: String? = null;  n?.length
来源：http://lau.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://xkg.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yrj.xziqi.cn

[T06] Kotlin：集合映射
来源：http://snl.sxryk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://twp.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://psu.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jzs.chenjidiqi.icu

[T08] Kotlin：数据类
来源：http://ria.chenjidiqi.icu

data class User(val name: String, val age: Int)
来源：http://goq.hammf.cn

[T09] Kotlin：扩展函数
来源：http://yyn.ydzc1.top

fun String.exclaim() = this + "!"
来源：http://yok.fehbvm.com

[T10] Kotlin：默认参数
来源：http://poh.yongpay.top

fun greet(name: String = "World") = "Hi $name"
来源：http://aau.uphjek.com

[T11] Kotlin：协程
来源：http://xas.9152youxi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vrj.birdmap.top

[T12] Kotlin：解构声明
来源：http://cmj.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://ztb.tianlin.xyz

[T13] Kotlin：只读 Map
来源：http://pme.jqgufenzy.top

val m = mapOf("a" to 1)
来源：http://bsw.gaohongyu789.top

[T14] Kotlin：循环
来源：http://ldf.hnqzz.top

for (i in 1..10) println(i)
来源：http://hep.yj20258.top

[T15] Kotlin：接口
来源：http://rsp.shanyushiyangkeji.top

interface Shape { fun area(): Double }
来源：http://jer.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://eaj.wangdashe.top

print("Hello")
来源：http://lnq.cucudq.cn

[T17] Swift：变量与常量
来源：http://vtk.zdqjudy.top

var a = 1;  let b = 2
来源：http://mwu.cashguo.top

[T18] Swift：字符串插值
来源：http://ydk.jinqigufen.top

"值: \(b)"
来源：http://vjd.yangfankeji.com

[T19] Swift：可选绑定
来源：http://hpn.yangfankeji.com

if let n = opt { print(n) }
来源：http://rmv.quarkkingdee.top

[T20] Swift：数组操作
来源：http://fhb.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zej.meibo888.top

[T21] Swift：遍历
来源：http://yun.havefunace.top

for x in a { print(x) }
来源：http://zxe.shanyushiyangtech.top

[T22] Swift：字典
来源：http://bza.jlsjyb.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gyq.jlsjyb.cn

[T23] Swift：函数
来源：http://kqp.tanke756.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zef.jinqigfzy.top

[T24] Swift：闭包
来源：http://oeu.bjfxy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lnz.dianchejie.cn

[T25] Swift：结构体
来源：http://vic.gotoacloud.top

struct P { var x: Int }
来源：http://agd.meibo888.top

[T26] Swift：类与重写
来源：http://kau.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://lml.jianghu66.top

[T27] Swift：错误处理
来源：http://uny.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://eab.fzhhl.top

[T28] Swift：枚举
来源：http://edi.gaohongyu789.top

enum Color { case red, green }
来源：http://lrj.pengpengdd.cyou

[T29] Swift：guard 提前返回
来源：http://vsb.yangfankeji.com

guard let x = opt else { return }
来源：http://nzw.nanxinkj.top

[T30] Swift：协议
来源：http://pvw.yanxiufei.cn

protocol Shape { func area() -> Double }
来源：http://wck.jqgufenzy.top

[T31] Lua：Hello World
来源：http://jvi.daxiang520.top

print("Hello")
来源：http://wva.xinyue.icu

[T32] Lua：局部变量
来源：http://bkx.guowangkeji.top

local a = 1
来源：http://epd.ivvv.top

[T33] Lua：表（数组）
来源：http://wcj.bbcook.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nzt.meibo888.top

[T34] Lua：遍历表
来源：http://ses.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xuh.wangshuangyany.cn

[T35] Lua：字典表
来源：http://jkj.sjlbkw.cn

local d = { a = 1 };  d.b = 2
来源：http://gnl.hysaishi.cn

[T36] Lua：函数
来源：http://ofe.snrcjt.cn

function add(a, b) return a + b end
来源：http://kuf.fengsongda.top

[T37] Lua：字符串拼接
来源：http://gwu.ivvv.top

"a" .. "b"
来源：http://bgk.gotoacloud.top

[T38] Lua：条件
来源：http://avn.vehdjk.com

if x > 0 then print("正") end
来源：http://csy.ydzc1.top

[T39] Lua：模式匹配
来源：http://usr.yangfankeji.com

string.find(s, "%d+")
来源：http://dyz.ydzc1.top

[T40] Lua：元表
来源：http://hnk.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://qez.9152youxi.cn

[T41] Perl：Hello World
来源：http://iui.xuetiantiany.cn

print "Hello\n";
来源：http://vov.birdmap.top

[T42] Perl：变量类型
来源：http://ovc.jiagoushi.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rbm.smart0.xyz

[T43] Perl：字符串插值
来源：http://zhg.chenjidiqi.icu

"值: $a"
来源：http://jzm.andypj.xyz

[T44] Perl：条件
来源：http://qde.jqgufenzy.top

if ($a > 0) { print "正"; }
来源：http://zcq.nanxuanxn.top

[T45] Perl：数组遍历
来源：http://ewc.chenjidiqi.icu

for my $x (@arr) { print $x; }
来源：http://geq.sysykeji.top

[T46] Perl：哈希操作
来源：http://vqo.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://slp.gotoacloud.top

[T47] Perl：正则捕获
来源：http://egy.aibaodan.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zae.xziqi.cn

[T48] Perl：正则替换
来源：http://mmv.svipenyu.cn

$s =~ s/old/new/g;
来源：http://wqc.zhengqikj.top

[T49] Perl：函数
来源：http://wbl.bbcook.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kei.havefunace.top

[T50] Perl：逐行读文件
来源：http://kpi.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://sxb.gzhubu.top

while (my $line = <$fh>) { print $line; }
来源：http://hrt.xziqi.cn

[T51] Scala：Hello World
来源：http://gvr.daxiang520.top

println("Hello")
来源：http://giz.gotoacloud.top

[T52] Scala：变量
来源：http://tpb.fzhhl.top

val a = 1;  var b = 2
来源：http://yxu.uphjek.com

[T53] Scala：字符串插值
来源：http://ful.epnwcf.com

s"值: $b"
来源：http://wng.sjlbkw.cn

[T54] Scala：集合映射
来源：http://vyp.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://pnm.nanxinkj.top

[T55] Scala：集合过滤
来源：http://cba.sufxvd.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qyc.fanxiaobao.xyz

[T56] Scala：样例类
来源：http://rtu.9152youxi.cn

case class User(name: String, age: Int)
来源：http://bck.dianchejie.cn

[T57] Scala：模式匹配
来源：http://nnn.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://cgk.mhx1999.top

[T58] Scala：函数定义
来源：http://rtp.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://dea.52xcode.cn

[T59] Scala：循环
来源：http://srd.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://lrc.yanxiufei.cn

[T60] Scala：折叠
来源：http://ftm.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rgy.cashguo.top

================================================================================
来源：http://itm.tanke756.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rfo.hfpthk.cn

================================================================================
来源：http://zpm.svipenyu.cn

[U01] Py：创建虚拟环境
来源：http://yrd.epnwcf.com

python -m venv .venv && source .venv/bin/activate
来源：http://enf.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://tgw.jinghuilouyu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uvl.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://loo.yfazqb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://whw.yuanzhike.top

[U04] Py：变量调试打印
来源：http://olp.c1oappe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zym.shzxlz.cn

[U05] Py：列表去重且保序
来源：http://kpc.tianlin.xyz

list(dict.fromkeys(arr))
来源：http://zfq.hesvh.cn

[U06] Py：合并两个字典
来源：http://fco.yj202588.top

{**a, **b}
来源：http://cws.aibaodan.cn

[U07] Py：反转字典键值
来源：http://pyg.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://umu.hesvh.cn

[U08] Py：展平二维列表
来源：http://yfd.316326.xyz

[y for x in nested for y in x]
来源：http://yzy.xuanzx.com

[U09] Py：字典取最大值的键
来源：http://tch.hongshengwenyu.top

max(d, key=d.get)
来源：http://kmi.hysaishi.cn

[U10] Py：按值排序字典
来源：http://vcp.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uvw.ywan-chungtsiang.top

[U11] Py：生成器表达式
来源：http://ozn.yangfankeji.com

(x * 2 for x in arr)
来源：http://rlf.zhoulong.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://uae.sysykeji.top

Counter(arr).most_common(3)
来源：http://qmf.jlsjyb.cn

[U13] Py：固定长度队列
来源：http://xml.ydzc1.top

deque(maxlen=10)
来源：http://rdt.ivvv.top

[U14] Py：分组收集到列表
来源：http://gde.yonumen.top

defaultdict(list)
来源：http://yvf.xylfe.cn

[U15] Py：高精度计时
来源：http://svl.ydjk.org.cn

t = time.perf_counter()
来源：http://yiq.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://kzh.haohaochexian.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dcn.gaohongyu789.top

[U17] Py：初始化日志
来源：http://yff.svipenyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://zpy.zhiwuduotai.top

[U18] Py：预编译正则
来源：http://lvj.ctjpmb.com

pat = re.compile(r"\d+")
来源：http://sri.zhengqikj.top

[U19] Py：正则替换带回调
来源：http://qki.guowangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jcf.xuanzx.com

[U20] Py：缓存函数结果
来源：http://bgv.cashguo.top

@functools.lru_cache(maxsize=None)
来源：http://ffz.jinghuilouyu.cn

[U21] Py：自定义上下文管理器
来源：http://okc.chenzaomai.com

@contextlib.contextmanager
来源：http://cuz.nanxinkj.top

[U22] Py：矩阵转置
来源：http://eqc.jinqigfzy.top

list(zip(*m))
来源：http://mut.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://pzv.xylfe.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ipq.fengsongda.top

[U24] Py：路径操作
来源：http://cxr.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jkr.shuidangran.top

[U25] Py：CSV 按字典读
来源：http://xxy.yuanzhike.top

csv.DictReader(f)
来源：http://txv.meibo888.top

[U26] Py：并发下载
来源：http://lyq.mhx1999.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wnj.nwbrower.top

[U27] Py：异步 HTTP
来源：http://bai.9152youxi.cn

aiohttp.ClientSession() 配合 async with
来源：http://nxe.xinyue.icu

[U28] Py：类型别名
来源：http://mvh.zhongyouzk.top

UserId = int
来源：http://qed.chenzaomai.com

[U29] Py：属性校验
来源：http://mql.svipenyu.cn

@property 与 @x.setter 配合
来源：http://jeo.xuetiantiany.cn

[U30] Py：数据类
来源：http://kyx.chenjidiqi.icu

@dataclass(slots=True)
来源：http://nhv.aibaodan.cn

[U31] Py：单测
来源：http://fyc.ppjwa.cn

python -m pytest -q
来源：http://waf.meibo888.top

[U32] Py：代码格式化
来源：http://sci.feifeiyinyue.top

ruff format . && ruff check --fix .
来源：http://puh.sufxvd.cn

[U33] Py：打包发布
来源：http://tdb.jqgufenzy.top

python -m build  （依赖 pyproject.toml）
来源：http://evz.fengsongda.top

[U34] Py：判断编码
来源：http://cau.nwbrower.top

chardet.detect(raw)
来源：http://mvp.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://bap.yj20258888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cyn.nwbrower.top

[U36] Py：定时任务
来源：http://pzg.nwbrower.top

schedule.every(10).minutes.do(job)
来源：http://oko.xziqi.cn

[U37] Py：读写 Excel
来源：http://fhz.c1oappe.top

pandas.read_excel / DataFrame.to_excel
来源：http://hqd.xinyue.icu

[U38] Py：获取脚本所在目录
来源：http://vtg.daria6918.cn

Path(__file__).resolve().parent
来源：http://iie.zycfv.cn

[U39] Py：判断是否在交互环境
来源：http://psq.yj20258888.top

sys.stdout.isatty()
来源：http://fvm.hysaishi.cn

[U40] Py：打印到标准错误
来源：http://hlu.zhoulong.xyz

print("err", file=sys.stderr)
来源：http://vsq.fanxiaobao.xyz

[U41] PHP：初始化 Composer 项目
来源：http://vtz.0kj1m.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tii.9152youxi.cn

[U42] PHP：PSR-4 自动加载
来源：http://yuk.jianghu66.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kiw.epnwcf.com

[U43] PHP：声明命名空间
来源：http://koi.daria6918.cn

namespace App\Http;
来源：http://edk.iojbl.cn

[U44] PHP：开启严格类型
来源：http://ntd.xuanzx.com

declare(strict_types=1);
来源：http://hsr.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://xgt.52xcode.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uwz.smart0.xyz

[U46] PHP：可空类型
来源：http://qst.guannengcc.top

?string $name = null
来源：http://kvp.hnqzz.top

[U47] PHP：联合类型
来源：http://rmo.hongshengwenyu.top

int|string $id
来源：http://gou.epnwcf.com

[U48] PHP：纯枚举
来源：http://nlp.hcnkem.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ifs.jinyuanbaomall.cn

[U49] PHP：只读属性
来源：http://vtz.sufxvd.cn

public readonly string $name
来源：http://vta.ehwqpu.com

[U50] PHP：构造器属性提升
来源：http://lrc.wangdashe.top

public function __construct(private int $id) {}
来源：http://lci.jiagoushi.top


<!-- 参考信息 -->