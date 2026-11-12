代发 wailian999

#include <iostream>
来源：http://fsv.redwolf501.top

int main() { std::cout << "Hello\n"; }
来源：http://lnn.ywan-chungtsiang.top

[S32] C++：字符串
来源：http://qfp.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://qkp.yongpay.top

[S33] C++：vector 增删
来源：http://xfb.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mja.zhengqikj.top

[S34] C++：遍历 vector
来源：http://dtl.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://ejq.jinyuanbaomall.cn

[S35] C++：map
来源：http://gpw.guowangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dbz.guannengcc.top

[S36] C++：unordered_map
来源：http://erg.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ltr.tianlin.xyz

[S37] C++：set
来源：http://idi.jianghu66.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://esq.birdmap.top

[S38] C++：排序
来源：http://adi.cheryme.top

std::sort(v.begin(), v.end());
来源：http://xoi.cqqwz.cn

[S39] C++：自定义比较器排序
来源：http://tpl.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nlc.tanke756.top

[S40] C++：查找元素
来源：http://buq.fengsongda.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bfd.tanke756.top

[S41] C++：类与构造函数
来源：http://jni.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fmj.gaohongyu789.top

[S42] C++：继承与虚函数
来源：http://hwc.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://tcv.jlsjyb.cn

[S43] C++：智能指针
来源：http://buo.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://vgv.jianghu66.top

[S44] C++：引用传参
来源：http://iuv.sysykeji.top

void inc(int &x) { ++x; }
来源：http://rae.xuanzx.com

[S45] C++：lambda
来源：http://mvh.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://aas.xuanzx.com

[S46] C++：函数模板
来源：http://gbi.vqdsnc.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://urh.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://qmw.ehwqpu.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cgn.zycfv.cn

[S48] C++：逐行读文件
来源：http://cbw.chenjidiqi.icu

std::ifstream in("a.txt");  std::string line;
来源：http://pmd.hongshengwenyu.top

while (std::getline(in, line)) { }
来源：http://lyg.jinqigufen.top

[S49] C++：写文件
来源：http://prd.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ecq.cdnleiting.top

[S50] C++：格式化数字
来源：http://xfo.tarul.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bpa.haohaochexian.top

[S51] C++：显式类型转换
来源：http://ait.fehbvm.com

static_cast<double>(a) / b
来源：http://ueu.zhixingplan.top

[S52] C++：const 与 noexcept
来源：http://efy.gzhubu.top

int size() const noexcept { return n_; }
来源：http://bba.xziqi.cn

[S53] C++：移动语义
来源：http://ldm.guannengcc.top

std::vector<int> w = std::move(v);
来源：http://hvn.birdmap.top

[S54] C++：异常处理
来源：http://wwz.jqgufenzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eki.tianlin.xyz

[S55] C++：结构化绑定
来源：http://rme.hnxiangtu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dlb.pengpengdd.cyou

[S56] C++：optional
来源：http://vyp.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eiu.zhixingplan.top

[S57] C++：编译期常量
来源：http://lvp.snrcjt.cn

constexpr int N = 10;
来源：http://dxe.wangshuangyany.cn

[S58] C++：命名空间
来源：http://tgy.316326.xyz

namespace ns { int f() { return 1; } }
来源：http://kop.jinqigufen.top

[S59] C++：静态断言
来源：http://ewo.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ezf.shanyushiyangtech.top

[S60] C++：遍历并删除元素
来源：http://jzf.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kmb.jyoumei.cn

================================================================================
来源：http://vwd.tianlin.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vkr.uphjek.com

================================================================================
来源：http://jzt.hesvh.cn

[T01] Kotlin：Hello World
来源：http://djc.guowangkeji.top

println("Hello")
来源：http://bdc.chenlongwang.top

[T02] Kotlin：变量
来源：http://kcl.zhijiandao.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nls.nwbrower.top

[T03] Kotlin：字符串模板
来源：http://wyf.mhx1999.top

"值: $b"
来源：http://jdz.sjlbkw.cn

[T04] Kotlin：空安全
来源：http://mkm.gotoacloud.top

val n: String? = null;  n?.length
来源：http://jsi.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://xfb.meibo888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://puf.zhoulong.xyz

[T06] Kotlin：集合映射
来源：http://pxt.nanxinkj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fmb.birdmap.top

[T07] Kotlin：集合过滤
来源：http://lvk.chenzaomai.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://sfw.daria6918.cn

[T08] Kotlin：数据类
来源：http://vye.zhaomingkeji.xyz

data class User(val name: String, val age: Int)
来源：http://kqe.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://pec.havefunace.top

fun String.exclaim() = this + "!"
来源：http://jfi.bbcook.cn

[T10] Kotlin：默认参数
来源：http://qjf.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fys.tarul.cn

[T11] Kotlin：协程
来源：http://wrt.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://kwl.bjfxy.top

[T12] Kotlin：解构声明
来源：http://pxj.pengpengdd.cyou

val (a, b) = Pair(1, 2)
来源：http://fok.haohaochexian.top

[T13] Kotlin：只读 Map
来源：http://lci.yfazqb.com

val m = mapOf("a" to 1)
来源：http://msi.yongpay.top

[T14] Kotlin：循环
来源：http://yaq.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://wtx.svipenyu.cn

[T15] Kotlin：接口
来源：http://gwz.cqqwz.cn

interface Shape { fun area(): Double }
来源：http://iah.aizwys.cn

[T16] Swift：Hello World
来源：http://mnl.shangyingyoupin.top

print("Hello")
来源：http://dcb.zhijiandao.cn

[T17] Swift：变量与常量
来源：http://tzu.pycfn.com

var a = 1;  let b = 2
来源：http://rma.yueranfly.top

[T18] Swift：字符串插值
来源：http://jdm.yonumen.top

"值: \(b)"
来源：http://hwq.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://foy.jqgufenzy.top

if let n = opt { print(n) }
来源：http://ukj.316326.xyz

[T20] Swift：数组操作
来源：http://bjs.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://rxm.yanxiufei.cn

[T21] Swift：遍历
来源：http://ruv.shzxlz.cn

for x in a { print(x) }
来源：http://fop.yj202588.top

[T22] Swift：字典
来源：http://pvo.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://tvp.ydzc1.top

[T23] Swift：函数
来源：http://yxm.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://inr.xziqi.cn

[T24] Swift：闭包
来源：http://roc.bbcook.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zps.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://brg.9152youxi.cn

struct P { var x: Int }
来源：http://znr.fktsv.cn

[T26] Swift：类与重写
来源：http://aes.ctjpmb.com

class A: Base { override func f() {} }
来源：http://kob.jinqigfzy.top

[T27] Swift：错误处理
来源：http://hbw.aizwys.cn

do { try f() } catch { print(error) }
来源：http://dmi.jinqigfzy.top

[T28] Swift：枚举
来源：http://xsy.jqgufenzy.top

enum Color { case red, green }
来源：http://pdg.dianchejie.cn

[T29] Swift：guard 提前返回
来源：http://ktm.hywenlv.cn

guard let x = opt else { return }
来源：http://fak.yfazqb.com

[T30] Swift：协议
来源：http://ioj.jlsjyb.cn

protocol Shape { func area() -> Double }
来源：http://icj.jyoumei.cn

[T31] Lua：Hello World
来源：http://kug.wangdashe.top

print("Hello")
来源：http://mpf.dianchejie.cn

[T32] Lua：局部变量
来源：http://vls.hnxiangtu.top

local a = 1
来源：http://azs.jqgufenzy.top

[T33] Lua：表（数组）
来源：http://bul.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hfb.ppjwa.cn

[T34] Lua：遍历表
来源：http://owi.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nid.zhijiandao.cn

[T35] Lua：字典表
来源：http://qkn.bbcook.cn

local d = { a = 1 };  d.b = 2
来源：http://igp.jinyuanbaomall.cn

[T36] Lua：函数
来源：http://fqx.daxiang520.top

function add(a, b) return a + b end
来源：http://mcv.smart0.xyz

[T37] Lua：字符串拼接
来源：http://xhg.yuanzhike.top

"a" .. "b"
来源：http://cym.shzxlz.cn

[T38] Lua：条件
来源：http://mir.aibaodan.cn

if x > 0 then print("正") end
来源：http://qen.jqgfzy.top

[T39] Lua：模式匹配
来源：http://dqk.zdbjq.cn

string.find(s, "%d+")
来源：http://kum.nanxuanxn.top

[T40] Lua：元表
来源：http://lai.yuxming.cn

setmetatable({}, { __index = base })
来源：http://cij.hysaishi.cn

[T41] Perl：Hello World
来源：http://oua.hnxiangtu.top

print "Hello\n";
来源：http://ght.0kj1m.cn

[T42] Perl：变量类型
来源：http://ojh.9152youxi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://abe.jqgfzy.top

[T43] Perl：字符串插值
来源：http://hem.tarul.cn

"值: $a"
来源：http://axj.yj202588.top

[T44] Perl：条件
来源：http://bux.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://xet.zhongyouzk.top

[T45] Perl：数组遍历
来源：http://gwn.zhijiandao.cn

for my $x (@arr) { print $x; }
来源：http://mzn.yueranfly.top

[T46] Perl：哈希操作
来源：http://luv.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vpa.xinyue.icu

[T47] Perl：正则捕获
来源：http://vnc.smart0.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://uvy.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://epe.ybcxt.top

$s =~ s/old/new/g;
来源：http://znk.xinyue.icu

[T49] Perl：函数
来源：http://oee.zycfv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://drj.cucudq.cn

[T50] Perl：逐行读文件
来源：http://hlk.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bam.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://qim.hesvh.cn

[T51] Scala：Hello World
来源：http://dqu.yongpay.top

println("Hello")
来源：http://rye.yfazqb.com

[T52] Scala：变量
来源：http://tom.bjfxy.top

val a = 1;  var b = 2
来源：http://dkg.ehwqpu.com

[T53] Scala：字符串插值
来源：http://sfo.ctjpmb.com

s"值: $b"
来源：http://kax.hysaishi.cn

[T54] Scala：集合映射
来源：http://obb.jiagoushi.top

List(1, 2, 3).map(_ * 2)
来源：http://fsy.0kj1m.cn

[T55] Scala：集合过滤
来源：http://tai.ybcxt.top

List(1, 2, 3).filter(_ > 1)
来源：http://gdx.jqgfzy.top

[T56] Scala：样例类
来源：http://fgq.cucudq.cn

case class User(name: String, age: Int)
来源：http://vgz.sweek.top

[T57] Scala：模式匹配
来源：http://sdt.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ydg.yvedp.cn

[T58] Scala：函数定义
来源：http://kyx.yuanzhike.top

def add(a: Int, b: Int): Int = a + b
来源：http://zit.vqdsnc.cn

[T59] Scala：循环
来源：http://mgr.sweek.top

for (i <- 1 to 10) println(i)
来源：http://ebd.xylfe.cn

[T60] Scala：折叠
来源：http://dmi.xylfe.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ybz.havefunace.top

================================================================================
来源：http://fwc.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rmf.jianghu66.top

================================================================================
来源：http://bvd.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://uvp.tian-w.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ebf.zycfv.cn

[U02] Py：导出 / 安装依赖
来源：http://tzn.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gpg.svipenyu.cn

[U03] Py：加载 .env 配置
来源：http://lgr.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dna.zhongyouzk.top

[U04] Py：变量调试打印
来源：http://yjj.aibaodan.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ois.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://dcj.yueranfly.top

list(dict.fromkeys(arr))
来源：http://pui.snrcjt.cn

[U06] Py：合并两个字典
来源：http://uhx.kuanghao11.cn

{**a, **b}
来源：http://xaw.yj202588.top

[U07] Py：反转字典键值
来源：http://emk.fengsongda.top

{v: k for k, v in d.items()}
来源：http://oxl.hesvh.cn

[U08] Py：展平二维列表
来源：http://aag.ywan-chungtsiang.top

[y for x in nested for y in x]
来源：http://ojm.sufxvd.cn

[U09] Py：字典取最大值的键
来源：http://rza.zhiwuduotai.top

max(d, key=d.get)
来源：http://beh.svipenyu.cn

[U10] Py：按值排序字典
来源：http://nkk.dianchejie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ewk.aibaodan.cn

[U11] Py：生成器表达式
来源：http://ogd.sxryk.cn

(x * 2 for x in arr)
来源：http://wme.sweek.top

[U12] Py：取出现最多的 3 个元素
来源：http://gir.cashguo.top

Counter(arr).most_common(3)
来源：http://fbr.gogol.net.cn

[U13] Py：固定长度队列
来源：http://sfn.meibo888.top

deque(maxlen=10)
来源：http://fjw.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://sxb.daria6918.cn

defaultdict(list)
来源：http://zeu.jqgfzy.top

[U15] Py：高精度计时
来源：http://mbw.dianchejie.cn

t = time.perf_counter()
来源：http://eql.fehbvm.com

[U16] Py：命令行参数解析
来源：http://uoe.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lbx.meibo888.top

[U17] Py：初始化日志
来源：http://urr.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://cvd.fengsongda.top

[U18] Py：预编译正则
来源：http://tkv.meibo888.top

pat = re.compile(r"\d+")
来源：http://cvj.smart0.xyz

[U19] Py：正则替换带回调
来源：http://xmg.cqqwz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gxv.guannengcc.top

[U20] Py：缓存函数结果
来源：http://fsl.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://kbp.cucudq.cn

[U21] Py：自定义上下文管理器
来源：http://sig.zhaomingkeji.xyz

@contextlib.contextmanager
来源：http://wuu.daxiang520.top

[U22] Py：矩阵转置
来源：http://vwa.jianghu66.top

list(zip(*m))
来源：http://xxj.hywenlv.cn

[U23] Py：分块读取大文件
来源：http://ihr.sufxvd.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nyw.pycfn.com

[U24] Py：路径操作
来源：http://cwx.chenzaomai.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tez.nanxinkj.top

[U25] Py：CSV 按字典读
来源：http://xmc.gzhubu.top

csv.DictReader(f)
来源：http://phr.fktsv.cn

[U26] Py：并发下载
来源：http://xhg.hysaishi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xee.ydjk.org.cn

[U27] Py：异步 HTTP
来源：http://eab.jqgufenzy.top

aiohttp.ClientSession() 配合 async with
来源：http://kgg.fktsv.cn

[U28] Py：类型别名
来源：http://iwr.ywan-chungtsiang.top

UserId = int
来源：http://hzx.zhengqikj.top

[U29] Py：属性校验
来源：http://tlq.hysaishi.cn

@property 与 @x.setter 配合
来源：http://gpp.yj20258888.top

[U30] Py：数据类
来源：http://eet.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://ngw.xziqi.cn

[U31] Py：单测
来源：http://qgr.gotoacloud.top

python -m pytest -q
来源：http://ckg.cdnleiting.top

[U32] Py：代码格式化
来源：http://wqt.sufxvd.cn

ruff format . && ruff check --fix .
来源：http://fas.hcnkem.com

[U33] Py：打包发布
来源：http://kdc.jiagoushi.top

python -m build  （依赖 pyproject.toml）
来源：http://svx.guannengcc.top

[U34] Py：判断编码
来源：http://zdm.hywenlv.cn

chardet.detect(raw)
来源：http://fox.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://pca.hongshengwenyu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sps.tianlin.xyz

[U36] Py：定时任务
来源：http://kpo.shanyushiyangkeji.top

schedule.every(10).minutes.do(job)
来源：http://cht.svipenyu.cn

[U37] Py：读写 Excel
来源：http://sjs.sysykeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://vfg.yj202588.top

[U38] Py：获取脚本所在目录
来源：http://xkr.ydzc1.top

Path(__file__).resolve().parent
来源：http://idl.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://scv.yonumen.top

sys.stdout.isatty()
来源：http://oxj.ybcxt.top

[U40] Py：打印到标准错误
来源：http://aes.shangyingyoupin.top

print("err", file=sys.stderr)
来源：http://rbw.xuetiantiany.cn

[U41] PHP：初始化 Composer 项目
来源：http://pej.sweek.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qtn.zdqjudy.top

[U42] PHP：PSR-4 自动加载
来源：http://vow.ybcxt.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cdn.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://fjb.svipenyu.cn

namespace App\Http;
来源：http://yld.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://smu.jianghu66.top

declare(strict_types=1);
来源：http://yub.meibo888.top

[U45] PHP：类型声明与返回类型
来源：http://mxm.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ytt.vehdjk.com

[U46] PHP：可空类型
来源：http://ihy.xinyue.icu

?string $name = null
来源：http://ujq.zhengqikj.top

[U47] PHP：联合类型
来源：http://yoj.tarul.cn

int|string $id
来源：http://fwn.xziqi.cn

[U48] PHP：纯枚举
来源：http://enz.bbcook.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://epx.tianlin.xyz

[U49] PHP：只读属性
来源：http://kwk.vqdsnc.cn

public readonly string $name
来源：http://kcg.pycfn.com

[U50] PHP：构造器属性提升
来源：http://tlq.jqgfzy.top

public function __construct(private int $id) {}
来源：http://msc.chenjidiqi.icu

[U51] PHP：数组解构
来源：http://ivb.mhx1999.top

[$a, $b] = $arr;
来源：http://qez.xingfuxueyuan.xyz

[U52] PHP：箭头函数
来源：http://hga.yonumen.top

$double = fn($x) => $x * 2;
来源：http://isp.9152youxi.cn

[U53] PHP：空合并运算符
来源：http://lur.haohaochexian.top

$v = $a ?? $b ?? "default";
来源：http://nwc.zhongyouzk.top

[U54] PHP：空安全调用
来源：http://wsm.hammf.cn

$obj?->method()
来源：http://dps.fzhhl.top

[U55] PHP：match 表达式
来源：http://xmk.zdqjudy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ckz.birdmap.top

[U56] PHP：命名参数
来源：http://olb.zdbjq.cn

f(a: 1, b: 2)
来源：http://rzp.feifeiyinyue.top


<!-- 参考信息 -->