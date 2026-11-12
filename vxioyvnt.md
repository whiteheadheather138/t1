代发 wailian999

#ifndef X_H
来源：http://ldf.daxiang520.top

#define X_H
来源：http://pvm.chenzaomai.com

#endif
来源：http://yoq.bbcook.cn

[S31] C++：Hello World
来源：http://hcw.kuanghao11.cn

#include <iostream>
来源：http://jcl.pengpengdd.cyou

int main() { std::cout << "Hello\n"; }
来源：http://nbg.gaohongyu789.top

[S32] C++：字符串
来源：http://myw.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://mmx.52xcode.cn

[S33] C++：vector 增删
来源：http://qym.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eaq.chenjidiqi.icu

[S34] C++：遍历 vector
来源：http://seo.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://spx.zhoulong.xyz

[S35] C++：map
来源：http://bad.redwolf501.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pij.hywenlv.cn

[S36] C++：unordered_map
来源：http://fmo.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://slq.guannengcc.top

[S37] C++：set
来源：http://kma.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://acz.havefunace.top

[S38] C++：排序
来源：http://ywy.vehdjk.com

std::sort(v.begin(), v.end());
来源：http://qnd.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://swt.9152youxi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yjd.jinyuanbaomall.cn

[S40] C++：查找元素
来源：http://gcd.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://asy.xinyue.icu

[S41] C++：类与构造函数
来源：http://snv.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qpr.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://oys.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://nzn.sweek.top

[S43] C++：智能指针
来源：http://pxc.ywan-chungtsiang.top

auto p = std::make_unique<int>(5);
来源：http://xek.smart0.xyz

[S44] C++：引用传参
来源：http://iwa.9152youxi.cn

void inc(int &x) { ++x; }
来源：http://ich.yuxming.cn

[S45] C++：lambda
来源：http://ejd.hfpthk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cja.fengsongda.top

[S46] C++：函数模板
来源：http://oob.smart0.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dcx.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://zui.hnqzz.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fzn.yj20258888.top

[S48] C++：逐行读文件
来源：http://fje.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://vrc.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://hqg.sufxvd.cn

[S49] C++：写文件
来源：http://eva.chenzaomai.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xre.jinqigufen.top

[S50] C++：格式化数字
来源：http://nfi.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ojt.xinyue.icu

[S51] C++：显式类型转换
来源：http://hef.hnxiangtu.top

static_cast<double>(a) / b
来源：http://rck.ydjk.org.cn

[S52] C++：const 与 noexcept
来源：http://vcq.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://irw.tian-w.cn

[S53] C++：移动语义
来源：http://nfe.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://srm.guannengcc.top

[S54] C++：异常处理
来源：http://epz.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qzp.yangfankeji.com

[S55] C++：结构化绑定
来源：http://yct.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://afa.jinyuanbaomall.cn

[S56] C++：optional
来源：http://ubx.ybcxt.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fxw.bbcook.cn

[S57] C++：编译期常量
来源：http://dtw.c1oappe.top

constexpr int N = 10;
来源：http://plb.sysykeji.top

[S58] C++：命名空间
来源：http://udg.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://ipw.yvedp.cn

[S59] C++：静态断言
来源：http://axn.bbcook.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nef.xziqi.cn

[S60] C++：遍历并删除元素
来源：http://xkk.bbcook.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://apw.vqdsnc.cn

================================================================================
来源：http://ahl.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://whv.zhixingplan.top

================================================================================
来源：http://rzs.tarul.cn

[T01] Kotlin：Hello World
来源：http://ksq.zycfv.cn

println("Hello")
来源：http://enp.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://xrl.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xqh.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://dil.hesvh.cn

"值: $b"
来源：http://iww.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://clw.ppjwa.cn

val n: String? = null;  n?.length
来源：http://npg.316326.xyz

[T05] Kotlin：when 表达式
来源：http://izz.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cse.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://ayw.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mnz.zhijiandao.cn

[T07] Kotlin：集合过滤
来源：http://cvd.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jjb.zhixingplan.top

[T08] Kotlin：数据类
来源：http://hhu.ywan-chungtsiang.top

data class User(val name: String, val age: Int)
来源：http://qom.yfazqb.com

[T09] Kotlin：扩展函数
来源：http://nnd.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://lez.zycfv.cn

[T10] Kotlin：默认参数
来源：http://cxi.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://lnf.uphjek.com

[T11] Kotlin：协程
来源：http://ezw.c1oappe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hox.ywan-chungtsiang.top

[T12] Kotlin：解构声明
来源：http://fju.hfpthk.cn

val (a, b) = Pair(1, 2)
来源：http://pdp.daria6918.cn

[T13] Kotlin：只读 Map
来源：http://rzo.andypj.xyz

val m = mapOf("a" to 1)
来源：http://zlx.hammf.cn

[T14] Kotlin：循环
来源：http://icl.yueranfly.top

for (i in 1..10) println(i)
来源：http://bga.sweek.top

[T15] Kotlin：接口
来源：http://dsj.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://okp.yfazqb.com

[T16] Swift：Hello World
来源：http://avw.shangyingyoupin.top

print("Hello")
来源：http://eno.hammf.cn

[T17] Swift：变量与常量
来源：http://qpo.ydjk.org.cn

var a = 1;  let b = 2
来源：http://pvg.yonumen.top

[T18] Swift：字符串插值
来源：http://rtl.pycfn.com

"值: \(b)"
来源：http://ffv.iojbl.cn

[T19] Swift：可选绑定
来源：http://tdz.cucudq.cn

if let n = opt { print(n) }
来源：http://jtd.ivvv.top

[T20] Swift：数组操作
来源：http://tvf.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jog.wangdashe.top

[T21] Swift：遍历
来源：http://mfv.gogol.net.cn

for x in a { print(x) }
来源：http://wfd.yj20258.top

[T22] Swift：字典
来源：http://ptp.yangfankeji.com

var d = ["a": 1];  d["b"] = 2
来源：http://bxj.shangyingyoupin.top

[T23] Swift：函数
来源：http://xgz.birdmap.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bmf.zycfv.cn

[T24] Swift：闭包
来源：http://vbo.yj20258.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ptg.hnxiangtu.top

[T25] Swift：结构体
来源：http://pgy.jqgufenzy.top

struct P { var x: Int }
来源：http://uif.jqgfzy.top

[T26] Swift：类与重写
来源：http://mgm.smart0.xyz

class A: Base { override func f() {} }
来源：http://ufm.zhiwuduotai.top

[T27] Swift：错误处理
来源：http://prs.tian-w.cn

do { try f() } catch { print(error) }
来源：http://eas.xuetiantiany.cn

[T28] Swift：枚举
来源：http://qov.zhixingplan.top

enum Color { case red, green }
来源：http://txn.hnxiangtu.top

[T29] Swift：guard 提前返回
来源：http://tqh.52xcode.cn

guard let x = opt else { return }
来源：http://vog.kuanghao11.cn

[T30] Swift：协议
来源：http://nsn.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://pol.nwbrower.top

[T31] Lua：Hello World
来源：http://box.chenjidiqi.icu

print("Hello")
来源：http://ags.yanxiufei.cn

[T32] Lua：局部变量
来源：http://ftz.chenlongwang.top

local a = 1
来源：http://ymy.zhengqikj.top

[T33] Lua：表（数组）
来源：http://qgq.jyoumei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://aox.hywenlv.cn

[T34] Lua：遍历表
来源：http://bsu.daria6918.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mri.yj202588.top

[T35] Lua：字典表
来源：http://xnk.cucudq.cn

local d = { a = 1 };  d.b = 2
来源：http://nmr.zhijiandao.cn

[T36] Lua：函数
来源：http://otv.hywenlv.cn

function add(a, b) return a + b end
来源：http://mqx.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://zvi.zhengqikj.top

"a" .. "b"
来源：http://vln.xuanzx.com

[T38] Lua：条件
来源：http://cwb.yuanzhike.top

if x > 0 then print("正") end
来源：http://smt.hfpthk.cn

[T39] Lua：模式匹配
来源：http://qwx.cashguo.top

string.find(s, "%d+")
来源：http://wgc.gaohongyu789.top

[T40] Lua：元表
来源：http://yfu.cashguo.top

setmetatable({}, { __index = base })
来源：http://yjm.fktsv.cn

[T41] Perl：Hello World
来源：http://jsc.bbcook.cn

print "Hello\n";
来源：http://sho.daria6918.cn

[T42] Perl：变量类型
来源：http://vab.jqgfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qvi.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://cog.yuanzhike.top

"值: $a"
来源：http://hci.jyoumei.cn

[T44] Perl：条件
来源：http://rwy.shanyushiyangtech.top

if ($a > 0) { print "正"; }
来源：http://hxx.gaohongyu789.top

[T45] Perl：数组遍历
来源：http://hwr.kuanghao11.cn

for my $x (@arr) { print $x; }
来源：http://lhk.gotoacloud.top

[T46] Perl：哈希操作
来源：http://hvv.jinqigufen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nyp.cucudq.cn

[T47] Perl：正则捕获
来源：http://ygp.hywenlv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fqi.zhiwuduotai.top

[T48] Perl：正则替换
来源：http://pyk.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://jxn.yvedp.cn

[T49] Perl：函数
来源：http://orr.epnwcf.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iwb.zhiwuduotai.top

[T50] Perl：逐行读文件
来源：http://lza.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zdu.yueranfly.top

while (my $line = <$fh>) { print $line; }
来源：http://dpy.tian-w.cn

[T51] Scala：Hello World
来源：http://qfd.andypj.xyz

println("Hello")
来源：http://gbv.yfazqb.com

[T52] Scala：变量
来源：http://uyf.jqgufenzy.top

val a = 1;  var b = 2
来源：http://dru.fengsongda.top

[T53] Scala：字符串插值
来源：http://ciq.hnqzz.top

s"值: $b"
来源：http://myy.svipenyu.cn

[T54] Scala：集合映射
来源：http://sgo.cqqwz.cn

List(1, 2, 3).map(_ * 2)
来源：http://gbt.cqqwz.cn

[T55] Scala：集合过滤
来源：http://fdp.kuanghao11.cn

List(1, 2, 3).filter(_ > 1)
来源：http://flq.uphjek.com

[T56] Scala：样例类
来源：http://iuy.aizwys.cn

case class User(name: String, age: Int)
来源：http://uzg.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://xsw.tian-w.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dtu.meibo888.top

[T58] Scala：函数定义
来源：http://ybt.fktsv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://biu.nanxuanxn.top

[T59] Scala：循环
来源：http://sdj.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://aqw.yueranfly.top

[T60] Scala：折叠
来源：http://omb.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://axp.yuanzhike.top

================================================================================
来源：http://tih.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vpa.smart0.xyz

================================================================================
来源：http://vyc.cheryme.top

[U01] Py：创建虚拟环境
来源：http://zme.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hbw.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://ymn.yuanzhike.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wbr.nanxuanxn.top

[U03] Py：加载 .env 配置
来源：http://jpp.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wju.tian-w.cn

[U04] Py：变量调试打印
来源：http://iyv.daxiang520.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cbx.sxryk.cn

[U05] Py：列表去重且保序
来源：http://amn.vqdsnc.cn

list(dict.fromkeys(arr))
来源：http://vvb.jinghuilouyu.cn

[U06] Py：合并两个字典
来源：http://iyr.ehwqpu.com

{**a, **b}
来源：http://qfa.hesvh.cn

[U07] Py：反转字典键值
来源：http://out.shanyushiyangtech.top

{v: k for k, v in d.items()}
来源：http://mtr.hysaishi.cn

[U08] Py：展平二维列表
来源：http://ipa.wangdashe.top

[y for x in nested for y in x]
来源：http://lcb.dianchejie.cn

[U09] Py：字典取最大值的键
来源：http://vgd.hywenlv.cn

max(d, key=d.get)
来源：http://bzb.shanyushiyangkeji.top

[U10] Py：按值排序字典
来源：http://ega.c1oappe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ikt.ppjwa.cn

[U11] Py：生成器表达式
来源：http://zwg.sweek.top

(x * 2 for x in arr)
来源：http://mbq.zycfv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pil.svipenyu.cn

Counter(arr).most_common(3)
来源：http://wpi.tanke756.top

[U13] Py：固定长度队列
来源：http://gff.iojbl.cn

deque(maxlen=10)
来源：http://avk.meibo888.top

[U14] Py：分组收集到列表
来源：http://ngm.jyoumei.cn

defaultdict(list)
来源：http://ncv.ybcxt.top

[U15] Py：高精度计时
来源：http://gny.tianlin.xyz

t = time.perf_counter()
来源：http://rkg.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://fmo.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uqo.316326.xyz

[U17] Py：初始化日志
来源：http://sos.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://pax.redwolf501.top

[U18] Py：预编译正则
来源：http://eny.chenzaomai.com

pat = re.compile(r"\d+")
来源：http://rkm.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://bhm.fengsongda.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oaa.zdqjudy.top

[U20] Py：缓存函数结果
来源：http://agz.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://bdj.meibo888.top

[U21] Py：自定义上下文管理器
来源：http://sil.hnqzz.top

@contextlib.contextmanager
来源：http://ogp.yj20258888.top

[U22] Py：矩阵转置
来源：http://imu.xuetiantiany.cn

list(zip(*m))
来源：http://tfm.fktsv.cn

[U23] Py：分块读取大文件
来源：http://ccs.jinghuilouyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mmb.kuanghao11.cn

[U24] Py：路径操作
来源：http://kjj.tianlin.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uls.yanxiufei.cn

[U25] Py：CSV 按字典读
来源：http://ikg.9152youxi.cn

csv.DictReader(f)
来源：http://vwp.shzxlz.cn

[U26] Py：并发下载
来源：http://lvm.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qig.52xcode.cn

[U27] Py：异步 HTTP
来源：http://wrr.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://xsp.cheryme.top

[U28] Py：类型别名
来源：http://abl.epnwcf.com

UserId = int
来源：http://qxb.chenlongwang.top

[U29] Py：属性校验
来源：http://qcb.zdbjq.cn

@property 与 @x.setter 配合
来源：http://rby.316326.xyz

[U30] Py：数据类
来源：http://ssr.chenlongwang.top

@dataclass(slots=True)
来源：http://nbv.mhx1999.top

[U31] Py：单测
来源：http://uzg.yongpay.top

python -m pytest -q
来源：http://djh.zdqjudy.top

[U32] Py：代码格式化
来源：http://cgq.fehbvm.com

ruff format . && ruff check --fix .
来源：http://zcs.tianlin.xyz

[U33] Py：打包发布
来源：http://jsv.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://lxm.ctjpmb.com

[U34] Py：判断编码
来源：http://dat.nanxuanxn.top

chardet.detect(raw)
来源：http://tvt.yueranfly.top

[U35] Py：发送邮件
来源：http://ali.zhaomingkeji.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fdo.havefunace.top

[U36] Py：定时任务
来源：http://qhc.shanyushiyangtech.top

schedule.every(10).minutes.do(job)
来源：http://jgh.xinyue.icu

[U37] Py：读写 Excel
来源：http://gss.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://eek.xuanzx.com

[U38] Py：获取脚本所在目录
来源：http://air.ywan-chungtsiang.top

Path(__file__).resolve().parent
来源：http://byx.jiagoushi.top

[U39] Py：判断是否在交互环境
来源：http://weq.xinyue.icu

sys.stdout.isatty()
来源：http://qml.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://taj.hfpthk.cn

print("err", file=sys.stderr)
来源：http://hnz.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://ece.zhongyouzk.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ycz.daria6918.cn

[U42] PHP：PSR-4 自动加载
来源：http://ule.jyoumei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lzw.sysykeji.top

[U43] PHP：声明命名空间
来源：http://ivj.jinyuanbaomall.cn

namespace App\Http;
来源：http://qvb.uphjek.com

[U44] PHP：开启严格类型
来源：http://ccu.sysykeji.top

declare(strict_types=1);
来源：http://ase.jqgfzy.top

[U45] PHP：类型声明与返回类型
来源：http://bcv.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zkj.xziqi.cn

[U46] PHP：可空类型
来源：http://lmt.smart0.xyz

?string $name = null
来源：http://tbm.xziqi.cn

[U47] PHP：联合类型
来源：http://lln.kuanghao11.cn

int|string $id
来源：http://ias.xinyue.icu

[U48] PHP：纯枚举
来源：http://qxa.yonumen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fjl.vehdjk.com

[U49] PHP：只读属性
来源：http://pjo.epnwcf.com

public readonly string $name
来源：http://pvk.ivvv.top

[U50] PHP：构造器属性提升
来源：http://hva.xuetiantiany.cn

public function __construct(private int $id) {}
来源：http://fsd.jqgfzy.top

[U51] PHP：数组解构
来源：http://egy.yueranfly.top

[$a, $b] = $arr;
来源：http://mft.yuxming.cn

[U52] PHP：箭头函数
来源：http://xeq.dashuyun.cn

$double = fn($x) => $x * 2;
来源：http://nji.yj20258.top

[U53] PHP：空合并运算符
来源：http://pdh.tian-w.cn

$v = $a ?? $b ?? "default";
来源：http://xnj.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://ejx.sysykeji.top

$obj?->method()
来源：http://smt.aibaodan.cn


<!-- 参考信息 -->