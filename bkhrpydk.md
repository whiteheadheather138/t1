代发 wailian999

#include <iostream>
来源：http://hzw.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://ooe.ydzc1.top

[S32] C++：字符串
来源：http://ydw.gzhubu.top

std::string s = "hi";  s += "!";
来源：http://uyp.cqqwz.cn

[S33] C++：vector 增删
来源：http://klv.wangshuangyany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jfh.fehbvm.com

[S34] C++：遍历 vector
来源：http://oky.tianlin.xyz

for (auto &x : v) { std::cout << x; }
来源：http://rzi.uphjek.com

[S35] C++：map
来源：http://vdq.sxryk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bti.cqqwz.cn

[S36] C++：unordered_map
来源：http://xof.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zbx.aibaodan.cn

[S37] C++：set
来源：http://uja.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uad.zycfv.cn

[S38] C++：排序
来源：http://plz.hongshengwenyu.top

std::sort(v.begin(), v.end());
来源：http://fsw.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://tuk.ctjpmb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aju.gogol.net.cn

[S40] C++：查找元素
来源：http://qlc.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mhi.0kj1m.cn

[S41] C++：类与构造函数
来源：http://erf.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nhi.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://mab.yj20258888.top

class B : public Base { public: void f() override {} };
来源：http://gnk.xinyue.icu

[S43] C++：智能指针
来源：http://ddl.zhoulong.xyz

auto p = std::make_unique<int>(5);
来源：http://nrh.yj20258.top

[S44] C++：引用传参
来源：http://kcl.haohaochexian.top

void inc(int &x) { ++x; }
来源：http://rou.hnxiangtu.top

[S45] C++：lambda
来源：http://hof.svipenyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ksj.jinqigfzy.top

[S46] C++：函数模板
来源：http://tex.hnqzz.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mig.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://olo.zhaomingkeji.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kcs.gotoacloud.top

[S48] C++：逐行读文件
来源：http://bhc.dashuyun.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dap.jqgfzy.top

while (std::getline(in, line)) { }
来源：http://nlw.yj20258.top

[S49] C++：写文件
来源：http://bze.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bdl.xingfuxueyuan.xyz

[S50] C++：格式化数字
来源：http://kyu.52xcode.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cyd.cdnleiting.top

[S51] C++：显式类型转换
来源：http://smj.tian-w.cn

static_cast<double>(a) / b
来源：http://duj.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://ltl.ehwqpu.com

int size() const noexcept { return n_; }
来源：http://ips.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://wlc.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://pye.ctjpmb.com

[S54] C++：异常处理
来源：http://jeb.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qyu.cdnleiting.top

[S55] C++：结构化绑定
来源：http://drw.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://iyh.sysykeji.top

[S56] C++：optional
来源：http://cch.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sco.yuxming.cn

[S57] C++：编译期常量
来源：http://gre.shangyingyoupin.top

constexpr int N = 10;
来源：http://mrz.yfazqb.com

[S58] C++：命名空间
来源：http://zbx.zhoulong.xyz

namespace ns { int f() { return 1; } }
来源：http://wcq.nanxinkj.top

[S59] C++：静态断言
来源：http://lvv.hcnkem.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oia.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://cfb.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oti.cashguo.top

================================================================================
来源：http://boz.tarul.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bxq.shanyushiyangkeji.top

================================================================================
来源：http://gpa.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://kmf.yj20258.top

println("Hello")
来源：http://mvm.daria6918.cn

[T02] Kotlin：变量
来源：http://gur.pycfn.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ppl.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://kxz.andypj.xyz

"值: $b"
来源：http://yzd.xuanzx.com

[T04] Kotlin：空安全
来源：http://vdo.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://oru.svipenyu.cn

[T05] Kotlin：when 表达式
来源：http://xki.jiagoushi.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hxx.tian-w.cn

[T06] Kotlin：集合映射
来源：http://mvw.havefunace.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tev.birdmap.top

[T07] Kotlin：集合过滤
来源：http://ofl.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gyj.dianchejie.cn

[T08] Kotlin：数据类
来源：http://keo.zhengqikj.top

data class User(val name: String, val age: Int)
来源：http://iox.feifeiyinyue.top

[T09] Kotlin：扩展函数
来源：http://fwe.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://ljo.mhx1999.top

[T10] Kotlin：默认参数
来源：http://fba.jlsjyb.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://aon.ybcxt.top

[T11] Kotlin：协程
来源：http://vgc.hysaishi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bdw.fengsongda.top

[T12] Kotlin：解构声明
来源：http://yyt.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://zgy.jlsjyb.cn

[T13] Kotlin：只读 Map
来源：http://cam.cashguo.top

val m = mapOf("a" to 1)
来源：http://uke.vqdsnc.cn

[T14] Kotlin：循环
来源：http://fdr.cqqwz.cn

for (i in 1..10) println(i)
来源：http://hxo.smart0.xyz

[T15] Kotlin：接口
来源：http://shh.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://ylu.xuanzx.com

[T16] Swift：Hello World
来源：http://qrh.yanxiufei.cn

print("Hello")
来源：http://rcd.iojbl.cn

[T17] Swift：变量与常量
来源：http://dvn.ywan-chungtsiang.top

var a = 1;  let b = 2
来源：http://urd.yonumen.top

[T18] Swift：字符串插值
来源：http://vgh.guannengcc.top

"值: \(b)"
来源：http://epj.shuidangran.top

[T19] Swift：可选绑定
来源：http://bnt.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://fqy.feifeiyinyue.top

[T20] Swift：数组操作
来源：http://ikn.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://itr.ppjwa.cn

[T21] Swift：遍历
来源：http://yen.shanyushiyangkeji.top

for x in a { print(x) }
来源：http://kin.yangfankeji.com

[T22] Swift：字典
来源：http://wxv.daxiang520.top

var d = ["a": 1];  d["b"] = 2
来源：http://iap.cheryme.top

[T23] Swift：函数
来源：http://yxs.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hms.zhengqikj.top

[T24] Swift：闭包
来源：http://sbm.hysaishi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://svi.redwolf501.top

[T25] Swift：结构体
来源：http://otp.andypj.xyz

struct P { var x: Int }
来源：http://svc.zhongyouzk.top

[T26] Swift：类与重写
来源：http://fpx.jiagoushi.top

class A: Base { override func f() {} }
来源：http://slx.vehdjk.com

[T27] Swift：错误处理
来源：http://ggn.dashuyun.cn

do { try f() } catch { print(error) }
来源：http://fpi.zycfv.cn

[T28] Swift：枚举
来源：http://nlg.smart0.xyz

enum Color { case red, green }
来源：http://yfd.jinghuilouyu.cn

[T29] Swift：guard 提前返回
来源：http://swu.chenzaomai.com

guard let x = opt else { return }
来源：http://dgr.zhaomingkeji.xyz

[T30] Swift：协议
来源：http://ffi.cashguo.top

protocol Shape { func area() -> Double }
来源：http://ejp.sjlbkw.cn

[T31] Lua：Hello World
来源：http://uqv.cheryme.top

print("Hello")
来源：http://xzs.shzxlz.cn

[T32] Lua：局部变量
来源：http://zll.ctjpmb.com

local a = 1
来源：http://ayi.haohaochexian.top

[T33] Lua：表（数组）
来源：http://weu.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vlz.hcnkem.com

[T34] Lua：遍历表
来源：http://kim.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qxz.52xcode.cn

[T35] Lua：字典表
来源：http://yyw.daxiang520.top

local d = { a = 1 };  d.b = 2
来源：http://jar.jyoumei.cn

[T36] Lua：函数
来源：http://zvv.tian-w.cn

function add(a, b) return a + b end
来源：http://iil.yonumen.top

[T37] Lua：字符串拼接
来源：http://zvp.aizwys.cn

"a" .. "b"
来源：http://dik.daria6918.cn

[T38] Lua：条件
来源：http://kcx.c1oappe.top

if x > 0 then print("正") end
来源：http://adp.haohaochexian.top

[T39] Lua：模式匹配
来源：http://ylt.jyoumei.cn

string.find(s, "%d+")
来源：http://xdx.ywan-chungtsiang.top

[T40] Lua：元表
来源：http://vgi.sysykeji.top

setmetatable({}, { __index = base })
来源：http://asa.gzhubu.top

[T41] Perl：Hello World
来源：http://dja.chenzaomai.com

print "Hello\n";
来源：http://wzj.zdqjudy.top

[T42] Perl：变量类型
来源：http://mfe.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hse.cashguo.top

[T43] Perl：字符串插值
来源：http://jni.xylfe.cn

"值: $a"
来源：http://kcj.mhx1999.top

[T44] Perl：条件
来源：http://wvr.yuxming.cn

if ($a > 0) { print "正"; }
来源：http://jow.shanyushiyangtech.top

[T45] Perl：数组遍历
来源：http://srq.kuanghao11.cn

for my $x (@arr) { print $x; }
来源：http://yqv.fzhhl.top

[T46] Perl：哈希操作
来源：http://trc.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ubs.kuanghao11.cn

[T47] Perl：正则捕获
来源：http://yaq.316326.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://neo.nanxinkj.top

[T48] Perl：正则替换
来源：http://azv.hywenlv.cn

$s =~ s/old/new/g;
来源：http://dmc.hesvh.cn

[T49] Perl：函数
来源：http://rvb.yfazqb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vfg.yonumen.top

[T50] Perl：逐行读文件
来源：http://zhp.tarul.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wqh.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://ujw.nwbrower.top

[T51] Scala：Hello World
来源：http://sev.epnwcf.com

println("Hello")
来源：http://vsl.havefunace.top

[T52] Scala：变量
来源：http://zbw.cheryme.top

val a = 1;  var b = 2
来源：http://gdl.guowangkeji.top

[T53] Scala：字符串插值
来源：http://vro.shuidangran.top

s"值: $b"
来源：http://yyn.yonumen.top

[T54] Scala：集合映射
来源：http://hly.chenlongwang.top

List(1, 2, 3).map(_ * 2)
来源：http://wdp.hywenlv.cn

[T55] Scala：集合过滤
来源：http://tfb.cucudq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ufi.yfazqb.com

[T56] Scala：样例类
来源：http://ihw.jqgfzy.top

case class User(name: String, age: Int)
来源：http://coo.yj20258.top

[T57] Scala：模式匹配
来源：http://gef.hysaishi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wag.epnwcf.com

[T58] Scala：函数定义
来源：http://tev.fengsongda.top

def add(a: Int, b: Int): Int = a + b
来源：http://hii.birdmap.top

[T59] Scala：循环
来源：http://ddn.guannengcc.top

for (i <- 1 to 10) println(i)
来源：http://uvh.zhixingplan.top

[T60] Scala：折叠
来源：http://efs.tianlin.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lzf.zdqjudy.top

================================================================================
来源：http://xrl.hongshengwenyu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vft.ivvv.top

================================================================================
来源：http://gkk.ehwqpu.com

[U01] Py：创建虚拟环境
来源：http://kmi.svipenyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pdz.dashuyun.cn

[U02] Py：导出 / 安装依赖
来源：http://bzz.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ewn.ydjk.org.cn

[U03] Py：加载 .env 配置
来源：http://rfq.redwolf501.top

from dotenv import load_dotenv; load_dotenv()
来源：http://deb.shzxlz.cn

[U04] Py：变量调试打印
来源：http://jli.bjfxy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hoz.sweek.top

[U05] Py：列表去重且保序
来源：http://brg.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://xpv.tianlin.xyz

[U06] Py：合并两个字典
来源：http://eln.iojbl.cn

{**a, **b}
来源：http://nws.quarkkingdee.top

[U07] Py：反转字典键值
来源：http://ovh.fanxiaobao.xyz

{v: k for k, v in d.items()}
来源：http://qct.svipenyu.cn

[U08] Py：展平二维列表
来源：http://xsp.zhaomingkeji.xyz

[y for x in nested for y in x]
来源：http://jzw.tarul.cn

[U09] Py：字典取最大值的键
来源：http://fuv.jinqigfzy.top

max(d, key=d.get)
来源：http://uuv.xuanzx.com

[U10] Py：按值排序字典
来源：http://fih.bjfxy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://laz.quarkkingdee.top

[U11] Py：生成器表达式
来源：http://lle.quarkkingdee.top

(x * 2 for x in arr)
来源：http://vlc.jianghu66.top

[U12] Py：取出现最多的 3 个元素
来源：http://gfx.feifeiyinyue.top

Counter(arr).most_common(3)
来源：http://vky.shangyingyoupin.top

[U13] Py：固定长度队列
来源：http://tir.svipenyu.cn

deque(maxlen=10)
来源：http://esc.daria6918.cn

[U14] Py：分组收集到列表
来源：http://cxq.tian-w.cn

defaultdict(list)
来源：http://otj.sjlbkw.cn

[U15] Py：高精度计时
来源：http://xyg.yonumen.top

t = time.perf_counter()
来源：http://phj.jqgufenzy.top

[U16] Py：命令行参数解析
来源：http://lkx.zhiwuduotai.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tfq.gogol.net.cn

[U17] Py：初始化日志
来源：http://rbl.hywenlv.cn

logging.basicConfig(level=logging.INFO)
来源：http://cwy.snrcjt.cn

[U18] Py：预编译正则
来源：http://nts.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://inx.uphjek.com

[U19] Py：正则替换带回调
来源：http://jqh.feifeiyinyue.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nnl.feifeiyinyue.top

[U20] Py：缓存函数结果
来源：http://yvt.yj202588.top

@functools.lru_cache(maxsize=None)
来源：http://ljd.daxiang520.top

[U21] Py：自定义上下文管理器
来源：http://uvk.ctjpmb.com

@contextlib.contextmanager
来源：http://voh.chenjidiqi.icu

[U22] Py：矩阵转置
来源：http://era.chenjidiqi.icu

list(zip(*m))
来源：http://odg.yj20258888.top

[U23] Py：分块读取大文件
来源：http://omo.gotoacloud.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dyc.zhongyouzk.top

[U24] Py：路径操作
来源：http://rqs.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wuu.cashguo.top

[U25] Py：CSV 按字典读
来源：http://aus.quarkkingdee.top

csv.DictReader(f)
来源：http://jtf.yueranfly.top

[U26] Py：并发下载
来源：http://bnj.cheryme.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cgf.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://hzh.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://has.ivvv.top

[U28] Py：类型别名
来源：http://lwh.hysaishi.cn

UserId = int
来源：http://xif.mhx1999.top

[U29] Py：属性校验
来源：http://hqk.tarul.cn

@property 与 @x.setter 配合
来源：http://ijf.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://pnr.zdqjudy.top

@dataclass(slots=True)
来源：http://ijv.ydjk.org.cn

[U31] Py：单测
来源：http://kna.cucudq.cn

python -m pytest -q
来源：http://dvs.hnqzz.top

[U32] Py：代码格式化
来源：http://cwf.dianchejie.cn

ruff format . && ruff check --fix .
来源：http://hwq.bjfxy.top

[U33] Py：打包发布
来源：http://mrq.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://wmd.meibo888.top

[U34] Py：判断编码
来源：http://rae.ehwqpu.com

chardet.detect(raw)
来源：http://zbt.zhongyouzk.top

[U35] Py：发送邮件
来源：http://ryo.yanxiufei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gzr.nwbrower.top

[U36] Py：定时任务
来源：http://obm.ybcxt.top

schedule.every(10).minutes.do(job)
来源：http://zzq.zhiwuduotai.top

[U37] Py：读写 Excel
来源：http://utp.wangdashe.top

pandas.read_excel / DataFrame.to_excel
来源：http://bpg.jinyuanbaomall.cn

[U38] Py：获取脚本所在目录
来源：http://ghl.cheryme.top

Path(__file__).resolve().parent
来源：http://bft.gaohongyu789.top

[U39] Py：判断是否在交互环境
来源：http://lky.gzhubu.top

sys.stdout.isatty()
来源：http://eoq.aibaodan.cn

[U40] Py：打印到标准错误
来源：http://lrq.xziqi.cn

print("err", file=sys.stderr)
来源：http://qlv.guannengcc.top

[U41] PHP：初始化 Composer 项目
来源：http://jcg.jyoumei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mqb.yonumen.top

[U42] PHP：PSR-4 自动加载
来源：http://xkm.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vrq.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://sis.jqgufenzy.top

namespace App\Http;
来源：http://ehl.gzhubu.top

[U44] PHP：开启严格类型
来源：http://sgw.bjfxy.top

declare(strict_types=1);
来源：http://ltk.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://dnr.fktsv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wrb.ppjwa.cn

[U46] PHP：可空类型
来源：http://iag.fehbvm.com

?string $name = null
来源：http://gfx.xylfe.cn

[U47] PHP：联合类型
来源：http://lvk.snrcjt.cn

int|string $id
来源：http://sjm.jinqigfzy.top

[U48] PHP：纯枚举
来源：http://aaq.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yik.zdbjq.cn

[U49] PHP：只读属性
来源：http://mdo.ppjwa.cn

public readonly string $name
来源：http://amg.yfazqb.com

[U50] PHP：构造器属性提升
来源：http://byl.jyoumei.cn

public function __construct(private int $id) {}
来源：http://uve.hcnkem.com

[U51] PHP：数组解构
来源：http://mar.zhixingplan.top

[$a, $b] = $arr;
来源：http://pwr.9152youxi.cn

[U52] PHP：箭头函数
来源：http://eqk.daria6918.cn

$double = fn($x) => $x * 2;
来源：http://byb.shanyushiyangtech.top

[U53] PHP：空合并运算符
来源：http://dmq.hysaishi.cn

$v = $a ?? $b ?? "default";
来源：http://wid.nanxuanxn.top

[U54] PHP：空安全调用
来源：http://byv.tanke756.top

$obj?->method()
来源：http://fcl.shuidangran.top

[U55] PHP：match 表达式
来源：http://ihc.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oas.9152youxi.cn

[U56] PHP：命名参数
来源：http://ppl.epnwcf.com

f(a: 1, b: 2)
来源：http://fwb.havefunace.top


<!-- 参考信息 -->