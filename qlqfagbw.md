代发 wailian999

#ifndef X_H
来源：http://ekp.fktsv.cn

#define X_H
来源：http://nlt.52xcode.cn

#endif
来源：http://how.yj202588.top

[S31] C++：Hello World
来源：http://xeh.cqqwz.cn

#include <iostream>
来源：http://bck.jyoumei.cn

int main() { std::cout << "Hello\n"; }
来源：http://tyk.dashuyun.cn

[S32] C++：字符串
来源：http://ucn.zhoulong.xyz

std::string s = "hi";  s += "!";
来源：http://qju.jyoumei.cn

[S33] C++：vector 增删
来源：http://iqo.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wwb.hnqzz.top

[S34] C++：遍历 vector
来源：http://mfm.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://lxl.jinqigfzy.top

[S35] C++：map
来源：http://puj.xuanzx.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fot.jqgfzy.top

[S36] C++：unordered_map
来源：http://fdc.zhengqikj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://klq.hcnkem.com

[S37] C++：set
来源：http://ddj.yvedp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://elh.hnqzz.top

[S38] C++：排序
来源：http://qmq.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://ypy.hcnkem.com

[S39] C++：自定义比较器排序
来源：http://kcy.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wfa.zdbjq.cn

[S40] C++：查找元素
来源：http://nan.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pko.dashuyun.cn

[S41] C++：类与构造函数
来源：http://qbd.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mqb.zycfv.cn

[S42] C++：继承与虚函数
来源：http://kri.gaohongyu789.top

class B : public Base { public: void f() override {} };
来源：http://nph.fktsv.cn

[S43] C++：智能指针
来源：http://qbp.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://tzz.uphjek.com

[S44] C++：引用传参
来源：http://gzi.haohaochexian.top

void inc(int &x) { ++x; }
来源：http://ffi.cheryme.top

[S45] C++：lambda
来源：http://ezc.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://zkr.hysaishi.cn

[S46] C++：函数模板
来源：http://ouw.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qlp.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://xou.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nrt.fktsv.cn

[S48] C++：逐行读文件
来源：http://orc.sjlbkw.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qyv.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://ngc.9152youxi.cn

[S49] C++：写文件
来源：http://unc.9152youxi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tol.aibaodan.cn

[S50] C++：格式化数字
来源：http://mtx.jinqigufen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gsi.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://eij.tanke756.top

static_cast<double>(a) / b
来源：http://zqh.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://fdh.jlsjyb.cn

int size() const noexcept { return n_; }
来源：http://okd.guannengcc.top

[S53] C++：移动语义
来源：http://smk.fzhhl.top

std::vector<int> w = std::move(v);
来源：http://ttw.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://lji.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hkf.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://nej.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mfv.vqdsnc.cn

[S56] C++：optional
来源：http://rjn.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aja.shuidangran.top

[S57] C++：编译期常量
来源：http://eif.ivvv.top

constexpr int N = 10;
来源：http://pys.shzxlz.cn

[S58] C++：命名空间
来源：http://qrt.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://oiy.nanxuanxn.top

[S59] C++：静态断言
来源：http://ekt.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pdu.hcnkem.com

[S60] C++：遍历并删除元素
来源：http://kma.9152youxi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://imf.xuetiantiany.cn

================================================================================
来源：http://rrt.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jbi.uphjek.com

================================================================================
来源：http://miv.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://yjj.epnwcf.com

println("Hello")
来源：http://wdk.snrcjt.cn

[T02] Kotlin：变量
来源：http://ssq.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pda.tanke756.top

[T03] Kotlin：字符串模板
来源：http://iyi.havefunace.top

"值: $b"
来源：http://rxp.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://udm.meibo888.top

val n: String? = null;  n?.length
来源：http://dej.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://irt.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hyp.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://sug.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://scy.dianchejie.cn

[T07] Kotlin：集合过滤
来源：http://ofz.sysykeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://klb.52xcode.cn

[T08] Kotlin：数据类
来源：http://upe.dashuyun.cn

data class User(val name: String, val age: Int)
来源：http://fcu.bbcook.cn

[T09] Kotlin：扩展函数
来源：http://snw.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://iyw.pycfn.com

[T10] Kotlin：默认参数
来源：http://hrr.andypj.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://jjk.zhoulong.xyz

[T11] Kotlin：协程
来源：http://nkg.hammf.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lgv.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://dnv.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://nga.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://jhw.jianghu66.top

val m = mapOf("a" to 1)
来源：http://fdj.vqdsnc.cn

[T14] Kotlin：循环
来源：http://fvc.hammf.cn

for (i in 1..10) println(i)
来源：http://clj.c1oappe.top

[T15] Kotlin：接口
来源：http://giq.jinqigfzy.top

interface Shape { fun area(): Double }
来源：http://ngn.ydjk.org.cn

[T16] Swift：Hello World
来源：http://ckd.iojbl.cn

print("Hello")
来源：http://afz.tianlin.xyz

[T17] Swift：变量与常量
来源：http://hmu.hfpthk.cn

var a = 1;  let b = 2
来源：http://wrr.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://gew.ywan-chungtsiang.top

"值: \(b)"
来源：http://hok.guannengcc.top

[T19] Swift：可选绑定
来源：http://idj.hysaishi.cn

if let n = opt { print(n) }
来源：http://ezk.jinghuilouyu.cn

[T20] Swift：数组操作
来源：http://dlv.hysaishi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tnq.yuanzhike.top

[T21] Swift：遍历
来源：http://xyu.52xcode.cn

for x in a { print(x) }
来源：http://mci.yvedp.cn

[T22] Swift：字典
来源：http://vog.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uls.hcnkem.com

[T23] Swift：函数
来源：http://xsv.zhijiandao.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dyb.kuanghao11.cn

[T24] Swift：闭包
来源：http://abh.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yog.kuanghao11.cn

[T25] Swift：结构体
来源：http://qln.hysaishi.cn

struct P { var x: Int }
来源：http://gxg.dianchejie.cn

[T26] Swift：类与重写
来源：http://ros.snrcjt.cn

class A: Base { override func f() {} }
来源：http://zkw.0kj1m.cn

[T27] Swift：错误处理
来源：http://nip.zdbjq.cn

do { try f() } catch { print(error) }
来源：http://hmd.jyoumei.cn

[T28] Swift：枚举
来源：http://fwk.xylfe.cn

enum Color { case red, green }
来源：http://wao.cucudq.cn

[T29] Swift：guard 提前返回
来源：http://ydy.hysaishi.cn

guard let x = opt else { return }
来源：http://fvh.yj20258888.top

[T30] Swift：协议
来源：http://aiz.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://fyy.tian-w.cn

[T31] Lua：Hello World
来源：http://icf.ivvv.top

print("Hello")
来源：http://yvk.epnwcf.com

[T32] Lua：局部变量
来源：http://kzi.feifeiyinyue.top

local a = 1
来源：http://znr.havefunace.top

[T33] Lua：表（数组）
来源：http://lqz.smart0.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://nhr.dashuyun.cn

[T34] Lua：遍历表
来源：http://jhs.xuetiantiany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tki.cqqwz.cn

[T35] Lua：字典表
来源：http://gbx.dashuyun.cn

local d = { a = 1 };  d.b = 2
来源：http://eep.yfazqb.com

[T36] Lua：函数
来源：http://fnf.zdbjq.cn

function add(a, b) return a + b end
来源：http://kef.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://gsf.xuanzx.com

"a" .. "b"
来源：http://yww.xinyue.icu

[T38] Lua：条件
来源：http://jxw.shangyingyoupin.top

if x > 0 then print("正") end
来源：http://dep.quarkkingdee.top

[T39] Lua：模式匹配
来源：http://oky.snrcjt.cn

string.find(s, "%d+")
来源：http://cuy.jinyuanbaomall.cn

[T40] Lua：元表
来源：http://ifm.zhijiandao.cn

setmetatable({}, { __index = base })
来源：http://aui.daxiang520.top

[T41] Perl：Hello World
来源：http://ioq.hfpthk.cn

print "Hello\n";
来源：http://usl.hcnkem.com

[T42] Perl：变量类型
来源：http://fpg.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qkw.ivvv.top

[T43] Perl：字符串插值
来源：http://mqs.yj20258.top

"值: $a"
来源：http://lmy.chenzaomai.com

[T44] Perl：条件
来源：http://fzi.yfazqb.com

if ($a > 0) { print "正"; }
来源：http://cmu.shangyingyoupin.top

[T45] Perl：数组遍历
来源：http://csn.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://zfu.daxiang520.top

[T46] Perl：哈希操作
来源：http://aue.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ktt.52xcode.cn

[T47] Perl：正则捕获
来源：http://pjs.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hrm.yvedp.cn

[T48] Perl：正则替换
来源：http://dlx.shuidangran.top

$s =~ s/old/new/g;
来源：http://lgr.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://kdy.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gcx.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://kdc.fktsv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zwu.yueranfly.top

while (my $line = <$fh>) { print $line; }
来源：http://tdm.yvedp.cn

[T51] Scala：Hello World
来源：http://bod.ehwqpu.com

println("Hello")
来源：http://ish.daria6918.cn

[T52] Scala：变量
来源：http://vjn.xingfuxueyuan.xyz

val a = 1;  var b = 2
来源：http://olx.bbcook.cn

[T53] Scala：字符串插值
来源：http://fcs.jinqigufen.top

s"值: $b"
来源：http://xob.jiagoushi.top

[T54] Scala：集合映射
来源：http://van.kuanghao11.cn

List(1, 2, 3).map(_ * 2)
来源：http://hke.hfpthk.cn

[T55] Scala：集合过滤
来源：http://ljm.yueranfly.top

List(1, 2, 3).filter(_ > 1)
来源：http://qej.meibo888.top

[T56] Scala：样例类
来源：http://dop.yangfankeji.com

case class User(name: String, age: Int)
来源：http://enb.chenjidiqi.icu

[T57] Scala：模式匹配
来源：http://wcb.fengsongda.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dua.ybcxt.top

[T58] Scala：函数定义
来源：http://mic.xuetiantiany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ynd.hesvh.cn

[T59] Scala：循环
来源：http://qjg.hysaishi.cn

for (i <- 1 to 10) println(i)
来源：http://brq.yvedp.cn

[T60] Scala：折叠
来源：http://zca.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://usd.shangyingyoupin.top

================================================================================
来源：http://ivn.dianchejie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://imw.shanyushiyangtech.top

================================================================================
来源：http://okm.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://wib.fengsongda.top

python -m venv .venv && source .venv/bin/activate
来源：http://zuq.hongshengwenyu.top

[U02] Py：导出 / 安装依赖
来源：http://lzh.fehbvm.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gzt.xingfuxueyuan.xyz

[U03] Py：加载 .env 配置
来源：http://iwm.hcnkem.com

from dotenv import load_dotenv; load_dotenv()
来源：http://zpj.chenjidiqi.icu

[U04] Py：变量调试打印
来源：http://dkf.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rxl.yj20258888.top

[U05] Py：列表去重且保序
来源：http://xig.yvedp.cn

list(dict.fromkeys(arr))
来源：http://dbg.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://doo.zhongyouzk.top

{**a, **b}
来源：http://nsm.jyoumei.cn

[U07] Py：反转字典键值
来源：http://kky.hnxiangtu.top

{v: k for k, v in d.items()}
来源：http://ysb.bbcook.cn

[U08] Py：展平二维列表
来源：http://jry.wangshuangyany.cn

[y for x in nested for y in x]
来源：http://gvg.tian-w.cn

[U09] Py：字典取最大值的键
来源：http://wrw.xingfuxueyuan.xyz

max(d, key=d.get)
来源：http://efv.sxryk.cn

[U10] Py：按值排序字典
来源：http://emh.vehdjk.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jve.vqdsnc.cn

[U11] Py：生成器表达式
来源：http://szw.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://rml.yfazqb.com

[U12] Py：取出现最多的 3 个元素
来源：http://mib.haohaochexian.top

Counter(arr).most_common(3)
来源：http://ltq.ivvv.top

[U13] Py：固定长度队列
来源：http://ihh.zhiwuduotai.top

deque(maxlen=10)
来源：http://yua.havefunace.top

[U14] Py：分组收集到列表
来源：http://mou.yfazqb.com

defaultdict(list)
来源：http://ixh.ivvv.top

[U15] Py：高精度计时
来源：http://cvy.shuidangran.top

t = time.perf_counter()
来源：http://knp.tian-w.cn

[U16] Py：命令行参数解析
来源：http://vmn.fengsongda.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ehe.ppjwa.cn

[U17] Py：初始化日志
来源：http://qta.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://dit.zhiwuduotai.top

[U18] Py：预编译正则
来源：http://tqp.shuidangran.top

pat = re.compile(r"\d+")
来源：http://cde.shanyushiyangkeji.top

[U19] Py：正则替换带回调
来源：http://pmj.gotoacloud.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qyz.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://bbv.hcnkem.com

@functools.lru_cache(maxsize=None)
来源：http://byg.zhengqikj.top

[U21] Py：自定义上下文管理器
来源：http://uox.cucudq.cn

@contextlib.contextmanager
来源：http://pim.hysaishi.cn

[U22] Py：矩阵转置
来源：http://aqh.zhengqikj.top

list(zip(*m))
来源：http://cja.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://swn.smart0.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fkm.snrcjt.cn

[U24] Py：路径操作
来源：http://ifi.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wav.sjlbkw.cn

[U25] Py：CSV 按字典读
来源：http://qwv.daxiang520.top

csv.DictReader(f)
来源：http://cxf.aizwys.cn

[U26] Py：并发下载
来源：http://bir.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ovw.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://zdi.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://mdz.zycfv.cn

[U28] Py：类型别名
来源：http://npt.fanxiaobao.xyz

UserId = int
来源：http://gcr.guannengcc.top

[U29] Py：属性校验
来源：http://lex.c1oappe.top

@property 与 @x.setter 配合
来源：http://qrc.52xcode.cn

[U30] Py：数据类
来源：http://yir.jqgfzy.top

@dataclass(slots=True)
来源：http://qvu.zhengqikj.top

[U31] Py：单测
来源：http://tps.ehwqpu.com

python -m pytest -q
来源：http://xey.hfpthk.cn

[U32] Py：代码格式化
来源：http://jtn.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://crq.yvedp.cn

[U33] Py：打包发布
来源：http://cdq.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://ign.jlsjyb.cn

[U34] Py：判断编码
来源：http://xxf.chenlongwang.top

chardet.detect(raw)
来源：http://vlb.zhijiandao.cn

[U35] Py：发送邮件
来源：http://psl.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bns.xingfuxueyuan.xyz

[U36] Py：定时任务
来源：http://alw.sxryk.cn

schedule.every(10).minutes.do(job)
来源：http://gzr.zdqjudy.top

[U37] Py：读写 Excel
来源：http://xyc.epnwcf.com

pandas.read_excel / DataFrame.to_excel
来源：http://yzs.gaohongyu789.top

[U38] Py：获取脚本所在目录
来源：http://mnr.fengsongda.top

Path(__file__).resolve().parent
来源：http://xdn.hammf.cn

[U39] Py：判断是否在交互环境
来源：http://tog.yanxiufei.cn

sys.stdout.isatty()
来源：http://ftw.ivvv.top

[U40] Py：打印到标准错误
来源：http://bhw.yongpay.top

print("err", file=sys.stderr)
来源：http://eka.ywan-chungtsiang.top

[U41] PHP：初始化 Composer 项目
来源：http://ook.0kj1m.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bbw.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://gfp.yj20258888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gkr.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://nbb.cheryme.top

namespace App\Http;
来源：http://mxo.zhaomingkeji.xyz

[U44] PHP：开启严格类型
来源：http://ame.chenjidiqi.icu

declare(strict_types=1);
来源：http://otu.gaohongyu789.top

[U45] PHP：类型声明与返回类型
来源：http://tkp.birdmap.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://smt.zdqjudy.top

[U46] PHP：可空类型
来源：http://zuo.meibo888.top

?string $name = null
来源：http://qov.nwbrower.top

[U47] PHP：联合类型
来源：http://awu.yj202588.top

int|string $id
来源：http://gvd.yj20258888.top

[U48] PHP：纯枚举
来源：http://ynz.chenlongwang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mxw.yuanzhike.top

[U49] PHP：只读属性
来源：http://qqc.cucudq.cn

public readonly string $name
来源：http://pma.fzhhl.top

[U50] PHP：构造器属性提升
来源：http://lkk.jianghu66.top

public function __construct(private int $id) {}
来源：http://xvz.zdqjudy.top

[U51] PHP：数组解构
来源：http://xad.shuidangran.top

[$a, $b] = $arr;
来源：http://fab.hcnkem.com

[U52] PHP：箭头函数
来源：http://wyj.yanxiufei.cn

$double = fn($x) => $x * 2;
来源：http://ywg.tanke756.top

[U53] PHP：空合并运算符
来源：http://rst.fzhhl.top

$v = $a ?? $b ?? "default";
来源：http://cog.yvedp.cn

[U54] PHP：空安全调用
来源：http://ufd.mhx1999.top

$obj?->method()
来源：http://bpm.wangdashe.top


<!-- 参考信息 -->