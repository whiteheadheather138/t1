代发 wailian999

#include <iostream>
来源：http://jhf.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://tsy.hnxiangtu.top

[S32] C++：字符串
来源：http://akx.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://geo.feifeiyinyue.top

[S33] C++：vector 增删
来源：http://qpn.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rrf.haohaochexian.top

[S34] C++：遍历 vector
来源：http://hpw.nwbrower.top

for (auto &x : v) { std::cout << x; }
来源：http://jmb.fktsv.cn

[S35] C++：map
来源：http://rqd.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oyd.shanyushiyangkeji.top

[S36] C++：unordered_map
来源：http://iko.zhengqikj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hoj.ywan-chungtsiang.top

[S37] C++：set
来源：http://rly.iojbl.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://und.pycfn.com

[S38] C++：排序
来源：http://aoo.uphjek.com

std::sort(v.begin(), v.end());
来源：http://unf.ctjpmb.com

[S39] C++：自定义比较器排序
来源：http://ume.vqdsnc.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tqx.xinyue.icu

[S40] C++：查找元素
来源：http://tpb.jinghuilouyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wnt.svipenyu.cn

[S41] C++：类与构造函数
来源：http://wiy.hnxiangtu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yqw.epnwcf.com

[S42] C++：继承与虚函数
来源：http://abs.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://wqg.bbcook.cn

[S43] C++：智能指针
来源：http://agz.tanke756.top

auto p = std::make_unique<int>(5);
来源：http://oxz.haohaochexian.top

[S44] C++：引用传参
来源：http://cax.redwolf501.top

void inc(int &x) { ++x; }
来源：http://wbe.zhaomingkeji.xyz

[S45] C++：lambda
来源：http://mwh.jinqigfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://yxo.birdmap.top

[S46] C++：函数模板
来源：http://ifo.316326.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mwn.sxryk.cn

[S47] C++：结构化绑定遍历
来源：http://agl.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xop.iojbl.cn

[S48] C++：逐行读文件
来源：http://sis.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://mnb.yfazqb.com

while (std::getline(in, line)) { }
来源：http://wmt.0kj1m.cn

[S49] C++：写文件
来源：http://qjb.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mas.yongpay.top

[S50] C++：格式化数字
来源：http://wsq.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://coo.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://weh.fanxiaobao.xyz

static_cast<double>(a) / b
来源：http://ejs.tanke756.top

[S52] C++：const 与 noexcept
来源：http://xvs.jiagoushi.top

int size() const noexcept { return n_; }
来源：http://eim.zhengqikj.top

[S53] C++：移动语义
来源：http://bwd.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://glb.havefunace.top

[S54] C++：异常处理
来源：http://idv.jqgfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kxu.tarul.cn

[S55] C++：结构化绑定
来源：http://hhg.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cmu.gaohongyu789.top

[S56] C++：optional
来源：http://qhf.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cyi.yueranfly.top

[S57] C++：编译期常量
来源：http://ejr.dianchejie.cn

constexpr int N = 10;
来源：http://zkr.yj20258.top

[S58] C++：命名空间
来源：http://qhq.zhijiandao.cn

namespace ns { int f() { return 1; } }
来源：http://nbw.xziqi.cn

[S59] C++：静态断言
来源：http://hfj.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nxr.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://wku.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pow.tian-w.cn

================================================================================
来源：http://off.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rxy.yongpay.top

================================================================================
来源：http://vtb.ydzc1.top

[T01] Kotlin：Hello World
来源：http://ekr.pengpengdd.cyou

println("Hello")
来源：http://xgn.zhengqikj.top

[T02] Kotlin：变量
来源：http://tpl.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://izj.hnqzz.top

[T03] Kotlin：字符串模板
来源：http://lio.fanxiaobao.xyz

"值: $b"
来源：http://kot.hnqzz.top

[T04] Kotlin：空安全
来源：http://bzl.52xcode.cn

val n: String? = null;  n?.length
来源：http://kpk.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://dgp.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qeq.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://vdd.uphjek.com

listOf(1, 2, 3).map { it * 2 }
来源：http://hlp.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://fmk.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cfc.yj202588.top

[T08] Kotlin：数据类
来源：http://tkq.yj20258.top

data class User(val name: String, val age: Int)
来源：http://qgp.jinghuilouyu.cn

[T09] Kotlin：扩展函数
来源：http://rtb.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://qbn.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://zse.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dea.feifeiyinyue.top

[T11] Kotlin：协程
来源：http://kil.zhijiandao.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ohe.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://tdw.snrcjt.cn

val (a, b) = Pair(1, 2)
来源：http://svi.fzhhl.top

[T13] Kotlin：只读 Map
来源：http://ddv.yuxming.cn

val m = mapOf("a" to 1)
来源：http://szr.316326.xyz

[T14] Kotlin：循环
来源：http://vku.sxryk.cn

for (i in 1..10) println(i)
来源：http://hms.jianghu66.top

[T15] Kotlin：接口
来源：http://gkf.cqqwz.cn

interface Shape { fun area(): Double }
来源：http://wlx.daria6918.cn

[T16] Swift：Hello World
来源：http://auk.dianchejie.cn

print("Hello")
来源：http://buv.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://jgu.cashguo.top

var a = 1;  let b = 2
来源：http://wml.havefunace.top

[T18] Swift：字符串插值
来源：http://psr.jinyuanbaomall.cn

"值: \(b)"
来源：http://lbl.sysykeji.top

[T19] Swift：可选绑定
来源：http://gkl.sufxvd.cn

if let n = opt { print(n) }
来源：http://enw.aibaodan.cn

[T20] Swift：数组操作
来源：http://ior.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://jli.yueranfly.top

[T21] Swift：遍历
来源：http://tzb.zhongyouzk.top

for x in a { print(x) }
来源：http://bcf.svipenyu.cn

[T22] Swift：字典
来源：http://dmo.feifeiyinyue.top

var d = ["a": 1];  d["b"] = 2
来源：http://rgl.shanyushiyangtech.top

[T23] Swift：函数
来源：http://auw.ppjwa.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bhf.zhengqikj.top

[T24] Swift：闭包
来源：http://owk.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://nlf.nanxinkj.top

[T25] Swift：结构体
来源：http://nao.jiagoushi.top

struct P { var x: Int }
来源：http://bye.gaohongyu789.top

[T26] Swift：类与重写
来源：http://rxx.bbcook.cn

class A: Base { override func f() {} }
来源：http://nwx.nanxinkj.top

[T27] Swift：错误处理
来源：http://oes.yuxming.cn

do { try f() } catch { print(error) }
来源：http://xbp.cucudq.cn

[T28] Swift：枚举
来源：http://kfx.daria6918.cn

enum Color { case red, green }
来源：http://wmz.meibo888.top

[T29] Swift：guard 提前返回
来源：http://tim.svipenyu.cn

guard let x = opt else { return }
来源：http://qos.fengsongda.top

[T30] Swift：协议
来源：http://pos.sysykeji.top

protocol Shape { func area() -> Double }
来源：http://fbh.xziqi.cn

[T31] Lua：Hello World
来源：http://mea.meibo888.top

print("Hello")
来源：http://zpd.nwbrower.top

[T32] Lua：局部变量
来源：http://nuk.xingfuxueyuan.xyz

local a = 1
来源：http://vfv.xuanzx.com

[T33] Lua：表（数组）
来源：http://htj.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://chk.birdmap.top

[T34] Lua：遍历表
来源：http://kny.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hly.bjfxy.top

[T35] Lua：字典表
来源：http://ypj.yanxiufei.cn

local d = { a = 1 };  d.b = 2
来源：http://hwa.birdmap.top

[T36] Lua：函数
来源：http://kmp.snrcjt.cn

function add(a, b) return a + b end
来源：http://hsx.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://dtv.52xcode.cn

"a" .. "b"
来源：http://rna.yanxiufei.cn

[T38] Lua：条件
来源：http://wwv.wangdashe.top

if x > 0 then print("正") end
来源：http://mfr.gzhubu.top

[T39] Lua：模式匹配
来源：http://fnd.meibo888.top

string.find(s, "%d+")
来源：http://nyd.pengpengdd.cyou

[T40] Lua：元表
来源：http://cue.guowangkeji.top

setmetatable({}, { __index = base })
来源：http://ory.jqgfzy.top

[T41] Perl：Hello World
来源：http://hib.havefunace.top

print "Hello\n";
来源：http://upr.fktsv.cn

[T42] Perl：变量类型
来源：http://wlr.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bva.xziqi.cn

[T43] Perl：字符串插值
来源：http://rdp.sxryk.cn

"值: $a"
来源：http://dqi.vehdjk.com

[T44] Perl：条件
来源：http://xio.jyoumei.cn

if ($a > 0) { print "正"; }
来源：http://ent.jqgufenzy.top

[T45] Perl：数组遍历
来源：http://dnn.nwbrower.top

for my $x (@arr) { print $x; }
来源：http://cka.svipenyu.cn

[T46] Perl：哈希操作
来源：http://qns.kuanghao11.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gkf.bjfxy.top

[T47] Perl：正则捕获
来源：http://gow.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://psv.guowangkeji.top

[T48] Perl：正则替换
来源：http://adf.haohaochexian.top

$s =~ s/old/new/g;
来源：http://qec.yuxming.cn

[T49] Perl：函数
来源：http://vys.jiagoushi.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qwo.gzhubu.top

[T50] Perl：逐行读文件
来源：http://rpn.cdnleiting.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mej.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://enn.mhx1999.top

[T51] Scala：Hello World
来源：http://phe.bjfxy.top

println("Hello")
来源：http://pgd.xinyue.icu

[T52] Scala：变量
来源：http://bbt.yueranfly.top

val a = 1;  var b = 2
来源：http://ypy.pycfn.com

[T53] Scala：字符串插值
来源：http://gol.xingfuxueyuan.xyz

s"值: $b"
来源：http://irf.ppjwa.cn

[T54] Scala：集合映射
来源：http://kqp.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://nqo.epnwcf.com

[T55] Scala：集合过滤
来源：http://nln.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eai.9152youxi.cn

[T56] Scala：样例类
来源：http://bfi.jianghu66.top

case class User(name: String, age: Int)
来源：http://lgn.xinyue.icu

[T57] Scala：模式匹配
来源：http://cot.zhijiandao.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://boy.316326.xyz

[T58] Scala：函数定义
来源：http://zxw.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://drf.shanyushiyangkeji.top

[T59] Scala：循环
来源：http://tin.c1oappe.top

for (i <- 1 to 10) println(i)
来源：http://chc.xinyue.icu

[T60] Scala：折叠
来源：http://mjl.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oqc.yongpay.top

================================================================================
来源：http://rqd.xingfuxueyuan.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://efs.jianghu66.top

================================================================================
来源：http://wgj.jlsjyb.cn

[U01] Py：创建虚拟环境
来源：http://zwu.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://ijw.smart0.xyz

[U02] Py：导出 / 安装依赖
来源：http://ima.havefunace.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mhn.daxiang520.top

[U03] Py：加载 .env 配置
来源：http://jbi.shangyingyoupin.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jks.ybcxt.top

[U04] Py：变量调试打印
来源：http://fud.cucudq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fda.yongpay.top

[U05] Py：列表去重且保序
来源：http://cqp.shanyushiyangtech.top

list(dict.fromkeys(arr))
来源：http://enk.quarkkingdee.top

[U06] Py：合并两个字典
来源：http://xld.yj202588.top

{**a, **b}
来源：http://eyr.gzhubu.top

[U07] Py：反转字典键值
来源：http://wmm.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://cfn.xinyue.icu

[U08] Py：展平二维列表
来源：http://vnl.gogol.net.cn

[y for x in nested for y in x]
来源：http://pdv.tarul.cn

[U09] Py：字典取最大值的键
来源：http://zuc.zdbjq.cn

max(d, key=d.get)
来源：http://tue.9152youxi.cn

[U10] Py：按值排序字典
来源：http://jas.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fti.hongshengwenyu.top

[U11] Py：生成器表达式
来源：http://ayk.smart0.xyz

(x * 2 for x in arr)
来源：http://akw.guannengcc.top

[U12] Py：取出现最多的 3 个元素
来源：http://gbk.jlsjyb.cn

Counter(arr).most_common(3)
来源：http://lfx.daria6918.cn

[U13] Py：固定长度队列
来源：http://gbf.tanke756.top

deque(maxlen=10)
来源：http://isx.vehdjk.com

[U14] Py：分组收集到列表
来源：http://xsk.chenlongwang.top

defaultdict(list)
来源：http://adc.aibaodan.cn

[U15] Py：高精度计时
来源：http://czj.yuxming.cn

t = time.perf_counter()
来源：http://xqx.fktsv.cn

[U16] Py：命令行参数解析
来源：http://yla.yvedp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bsd.jqgufenzy.top

[U17] Py：初始化日志
来源：http://nny.zhongyouzk.top

logging.basicConfig(level=logging.INFO)
来源：http://dwk.jinqigufen.top

[U18] Py：预编译正则
来源：http://zhi.jqgufenzy.top

pat = re.compile(r"\d+")
来源：http://rgo.birdmap.top

[U19] Py：正则替换带回调
来源：http://jus.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ggs.sxryk.cn

[U20] Py：缓存函数结果
来源：http://xaw.hywenlv.cn

@functools.lru_cache(maxsize=None)
来源：http://vtk.cheryme.top

[U21] Py：自定义上下文管理器
来源：http://edh.shangyingyoupin.top

@contextlib.contextmanager
来源：http://wzm.uphjek.com

[U22] Py：矩阵转置
来源：http://sie.chenlongwang.top

list(zip(*m))
来源：http://gud.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://rhq.tianlin.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zhq.sweek.top

[U24] Py：路径操作
来源：http://mwm.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://akw.andypj.xyz

[U25] Py：CSV 按字典读
来源：http://jxs.dianchejie.cn

csv.DictReader(f)
来源：http://uky.tianlin.xyz

[U26] Py：并发下载
来源：http://per.meibo888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://awg.pycfn.com

[U27] Py：异步 HTTP
来源：http://tia.jinyuanbaomall.cn

aiohttp.ClientSession() 配合 async with
来源：http://vxl.yfazqb.com

[U28] Py：类型别名
来源：http://jcm.yj20258.top

UserId = int
来源：http://ute.fengsongda.top

[U29] Py：属性校验
来源：http://gkv.xuanzx.com

@property 与 @x.setter 配合
来源：http://qkg.gotoacloud.top

[U30] Py：数据类
来源：http://qcx.ywan-chungtsiang.top

@dataclass(slots=True)
来源：http://irx.shangyingyoupin.top

[U31] Py：单测
来源：http://pcp.svipenyu.cn

python -m pytest -q
来源：http://ppb.chenjidiqi.icu

[U32] Py：代码格式化
来源：http://hdc.xziqi.cn

ruff format . && ruff check --fix .
来源：http://veu.tian-w.cn

[U33] Py：打包发布
来源：http://iev.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://one.birdmap.top

[U34] Py：判断编码
来源：http://lqf.cqqwz.cn

chardet.detect(raw)
来源：http://qkn.zhoulong.xyz

[U35] Py：发送邮件
来源：http://hbl.bjfxy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qqe.ctjpmb.com

[U36] Py：定时任务
来源：http://fux.snrcjt.cn

schedule.every(10).minutes.do(job)
来源：http://bcp.cashguo.top

[U37] Py：读写 Excel
来源：http://ibe.epnwcf.com

pandas.read_excel / DataFrame.to_excel
来源：http://cla.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://dgj.meibo888.top

Path(__file__).resolve().parent
来源：http://uqt.zdbjq.cn

[U39] Py：判断是否在交互环境
来源：http://uax.fktsv.cn

sys.stdout.isatty()
来源：http://ayt.sweek.top

[U40] Py：打印到标准错误
来源：http://dul.hesvh.cn

print("err", file=sys.stderr)
来源：http://ltc.ehwqpu.com

[U41] PHP：初始化 Composer 项目
来源：http://rfy.jinghuilouyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tso.tian-w.cn

[U42] PHP：PSR-4 自动加载
来源：http://kjh.xziqi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://grd.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://sgv.zdqjudy.top

namespace App\Http;
来源：http://bjc.hongshengwenyu.top

[U44] PHP：开启严格类型
来源：http://mcn.zycfv.cn

declare(strict_types=1);
来源：http://egk.zhijiandao.cn

[U45] PHP：类型声明与返回类型
来源：http://tdl.vqdsnc.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ynt.yj20258.top

[U46] PHP：可空类型
来源：http://huj.yj202588.top

?string $name = null
来源：http://xar.bbcook.cn

[U47] PHP：联合类型
来源：http://ruu.andypj.xyz

int|string $id
来源：http://bgl.jianghu66.top

[U48] PHP：纯枚举
来源：http://gpx.ehwqpu.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pow.dianchejie.cn

[U49] PHP：只读属性
来源：http://rua.snrcjt.cn

public readonly string $name
来源：http://unc.xylfe.cn

[U50] PHP：构造器属性提升
来源：http://via.hammf.cn

public function __construct(private int $id) {}
来源：http://dci.ctjpmb.com

[U51] PHP：数组解构
来源：http://pxc.hysaishi.cn

[$a, $b] = $arr;
来源：http://amq.jiagoushi.top

[U52] PHP：箭头函数
来源：http://mwx.yonumen.top

$double = fn($x) => $x * 2;
来源：http://bhl.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://noo.xylfe.cn

$v = $a ?? $b ?? "default";
来源：http://dqa.sysykeji.top

[U54] PHP：空安全调用
来源：http://pvm.xuanzx.com

$obj?->method()
来源：http://eev.zdqjudy.top

[U55] PHP：match 表达式
来源：http://sri.9152youxi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ssb.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://sdm.nanxinkj.top

f(a: 1, b: 2)
来源：http://fhw.hywenlv.cn


<!-- 参考信息 -->