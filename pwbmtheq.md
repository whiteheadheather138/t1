代发 wailian999

#include <iostream>
来源：http://wna.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://fwo.hnxiangtu.top

[S32] C++：字符串
来源：http://cxe.sufxvd.cn

std::string s = "hi";  s += "!";
来源：http://wgy.316326.xyz

[S33] C++：vector 增删
来源：http://rdu.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://snn.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://omm.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://tjt.cheryme.top

[S35] C++：map
来源：http://wlw.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lke.guannengcc.top

[S36] C++：unordered_map
来源：http://wse.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://buz.nwbrower.top

[S37] C++：set
来源：http://ere.zdbjq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gwl.fengsongda.top

[S38] C++：排序
来源：http://epy.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://wma.bjfxy.top

[S39] C++：自定义比较器排序
来源：http://tgr.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ozb.cdnleiting.top

[S40] C++：查找元素
来源：http://anf.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cpk.xylfe.cn

[S41] C++：类与构造函数
来源：http://gsd.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mfx.sjlbkw.cn

[S42] C++：继承与虚函数
来源：http://ijv.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://pzq.xinyue.icu

[S43] C++：智能指针
来源：http://fya.0kj1m.cn

auto p = std::make_unique<int>(5);
来源：http://oot.hesvh.cn

[S44] C++：引用传参
来源：http://bvd.chenlongwang.top

void inc(int &x) { ++x; }
来源：http://xai.shzxlz.cn

[S45] C++：lambda
来源：http://ejm.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://mcp.xuanzx.com

[S46] C++：函数模板
来源：http://tdc.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://reo.feifeiyinyue.top

[S47] C++：结构化绑定遍历
来源：http://mxz.jinqigfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lvt.smart0.xyz

[S48] C++：逐行读文件
来源：http://wlz.bjfxy.top

std::ifstream in("a.txt");  std::string line;
来源：http://tnd.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://vbp.jinqigufen.top

[S49] C++：写文件
来源：http://fnv.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dmg.fzhhl.top

[S50] C++：格式化数字
来源：http://dhq.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://puw.gogol.net.cn

[S51] C++：显式类型转换
来源：http://lod.sufxvd.cn

static_cast<double>(a) / b
来源：http://oiy.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://rln.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://ixl.aibaodan.cn

[S53] C++：移动语义
来源：http://xme.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://aiv.sxryk.cn

[S54] C++：异常处理
来源：http://xxs.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xug.sufxvd.cn

[S55] C++：结构化绑定
来源：http://xgg.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://enn.ehwqpu.com

[S56] C++：optional
来源：http://jra.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://olu.ppjwa.cn

[S57] C++：编译期常量
来源：http://cmk.c1oappe.top

constexpr int N = 10;
来源：http://cqy.nanxuanxn.top

[S58] C++：命名空间
来源：http://pup.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://yhb.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://rnw.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eaa.cucudq.cn

[S60] C++：遍历并删除元素
来源：http://luq.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://led.cheryme.top

================================================================================
来源：http://cbj.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fni.hywenlv.cn

================================================================================
来源：http://dng.nanxuanxn.top

[T01] Kotlin：Hello World
来源：http://gto.shanyushiyangtech.top

println("Hello")
来源：http://ewe.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://nli.xuanzx.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eee.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://wny.316326.xyz

"值: $b"
来源：http://jct.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://kjn.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://uui.316326.xyz

[T05] Kotlin：when 表达式
来源：http://gku.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://euq.zdqjudy.top

[T06] Kotlin：集合映射
来源：http://qaq.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rdi.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://hcc.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cqj.yueranfly.top

[T08] Kotlin：数据类
来源：http://qqt.316326.xyz

data class User(val name: String, val age: Int)
来源：http://ouf.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://pkm.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://dao.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://tsp.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://dtp.gzhubu.top

[T11] Kotlin：协程
来源：http://iqf.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://cwk.yfazqb.com

[T12] Kotlin：解构声明
来源：http://qpf.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://jls.aibaodan.cn

[T13] Kotlin：只读 Map
来源：http://fhl.dashuyun.cn

val m = mapOf("a" to 1)
来源：http://fqg.svipenyu.cn

[T14] Kotlin：循环
来源：http://qkh.meibo888.top

for (i in 1..10) println(i)
来源：http://tll.xziqi.cn

[T15] Kotlin：接口
来源：http://bre.sysykeji.top

interface Shape { fun area(): Double }
来源：http://epo.cashguo.top

[T16] Swift：Hello World
来源：http://pbb.hammf.cn

print("Hello")
来源：http://khx.andypj.xyz

[T17] Swift：变量与常量
来源：http://uyp.haohaochexian.top

var a = 1;  let b = 2
来源：http://jaa.52xcode.cn

[T18] Swift：字符串插值
来源：http://wnc.tianlin.xyz

"值: \(b)"
来源：http://ugi.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://euu.daria6918.cn

if let n = opt { print(n) }
来源：http://dkp.svipenyu.cn

[T20] Swift：数组操作
来源：http://cap.yangfankeji.com

var a = [1, 2, 3];  a.append(4)
来源：http://zba.meibo888.top

[T21] Swift：遍历
来源：http://chu.fzhhl.top

for x in a { print(x) }
来源：http://gpc.cucudq.cn

[T22] Swift：字典
来源：http://nri.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://sfr.shzxlz.cn

[T23] Swift：函数
来源：http://qwp.tarul.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ssk.cucudq.cn

[T24] Swift：闭包
来源：http://fwe.zhengqikj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://roj.nanxuanxn.top

[T25] Swift：结构体
来源：http://izf.yj20258.top

struct P { var x: Int }
来源：http://ltm.nanxinkj.top

[T26] Swift：类与重写
来源：http://tob.redwolf501.top

class A: Base { override func f() {} }
来源：http://egj.xuetiantiany.cn

[T27] Swift：错误处理
来源：http://qvk.jqgfzy.top

do { try f() } catch { print(error) }
来源：http://lrl.vqdsnc.cn

[T28] Swift：枚举
来源：http://god.zhoulong.xyz

enum Color { case red, green }
来源：http://smj.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://izz.ehwqpu.com

guard let x = opt else { return }
来源：http://kyp.shanyushiyangkeji.top

[T30] Swift：协议
来源：http://gup.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://kww.jianghu66.top

[T31] Lua：Hello World
来源：http://nuu.bjfxy.top

print("Hello")
来源：http://wat.wangshuangyany.cn

[T32] Lua：局部变量
来源：http://zok.jianghu66.top

local a = 1
来源：http://tht.jianghu66.top

[T33] Lua：表（数组）
来源：http://pcu.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://khb.guannengcc.top

[T34] Lua：遍历表
来源：http://fpx.cashguo.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ixj.c1oappe.top

[T35] Lua：字典表
来源：http://sgd.xingfuxueyuan.xyz

local d = { a = 1 };  d.b = 2
来源：http://hum.yvedp.cn

[T36] Lua：函数
来源：http://xca.jiagoushi.top

function add(a, b) return a + b end
来源：http://dcg.cheryme.top

[T37] Lua：字符串拼接
来源：http://tpq.sweek.top

"a" .. "b"
来源：http://qkm.svipenyu.cn

[T38] Lua：条件
来源：http://woc.fengsongda.top

if x > 0 then print("正") end
来源：http://xdd.hammf.cn

[T39] Lua：模式匹配
来源：http://wzc.ydzc1.top

string.find(s, "%d+")
来源：http://eci.vqdsnc.cn

[T40] Lua：元表
来源：http://wth.fzhhl.top

setmetatable({}, { __index = base })
来源：http://sjg.yuanzhike.top

[T41] Perl：Hello World
来源：http://lac.9152youxi.cn

print "Hello\n";
来源：http://kxt.shuidangran.top

[T42] Perl：变量类型
来源：http://roe.yonumen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nxm.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://ubf.tian-w.cn

"值: $a"
来源：http://xoc.bbcook.cn

[T44] Perl：条件
来源：http://hcu.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://hel.zycfv.cn

[T45] Perl：数组遍历
来源：http://tvl.chenzaomai.com

for my $x (@arr) { print $x; }
来源：http://qwi.zycfv.cn

[T46] Perl：哈希操作
来源：http://sjo.xuanzx.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qrq.hysaishi.cn

[T47] Perl：正则捕获
来源：http://olo.zhongyouzk.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://grg.tanke756.top

[T48] Perl：正则替换
来源：http://izb.hcnkem.com

$s =~ s/old/new/g;
来源：http://asa.aibaodan.cn

[T49] Perl：函数
来源：http://xan.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hyn.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://ngf.svipenyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sps.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://nmx.hesvh.cn

[T51] Scala：Hello World
来源：http://yan.hcnkem.com

println("Hello")
来源：http://nix.xylfe.cn

[T52] Scala：变量
来源：http://jmz.zdqjudy.top

val a = 1;  var b = 2
来源：http://bij.cdnleiting.top

[T53] Scala：字符串插值
来源：http://agb.yj20258888.top

s"值: $b"
来源：http://ijz.yueranfly.top

[T54] Scala：集合映射
来源：http://jjj.gaohongyu789.top

List(1, 2, 3).map(_ * 2)
来源：http://ikw.redwolf501.top

[T55] Scala：集合过滤
来源：http://fpx.gotoacloud.top

List(1, 2, 3).filter(_ > 1)
来源：http://vnb.yvedp.cn

[T56] Scala：样例类
来源：http://wtq.9152youxi.cn

case class User(name: String, age: Int)
来源：http://ybb.bjfxy.top

[T57] Scala：模式匹配
来源：http://cqo.zdqjudy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ycm.haohaochexian.top

[T58] Scala：函数定义
来源：http://bza.hongshengwenyu.top

def add(a: Int, b: Int): Int = a + b
来源：http://kpr.c1oappe.top

[T59] Scala：循环
来源：http://toz.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://jlx.zdqjudy.top

[T60] Scala：折叠
来源：http://tqc.fengsongda.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yyh.guannengcc.top

================================================================================
来源：http://ncw.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nce.zhiwuduotai.top

================================================================================
来源：http://pyw.haohaochexian.top

[U01] Py：创建虚拟环境
来源：http://zjz.havefunace.top

python -m venv .venv && source .venv/bin/activate
来源：http://maf.tianlin.xyz

[U02] Py：导出 / 安装依赖
来源：http://yeg.fehbvm.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ewp.havefunace.top

[U03] Py：加载 .env 配置
来源：http://jou.hnqzz.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sxy.shangyingyoupin.top

[U04] Py：变量调试打印
来源：http://hns.shzxlz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oti.52xcode.cn

[U05] Py：列表去重且保序
来源：http://lgp.xylfe.cn

list(dict.fromkeys(arr))
来源：http://psc.tianlin.xyz

[U06] Py：合并两个字典
来源：http://fql.chenjidiqi.icu

{**a, **b}
来源：http://uko.birdmap.top

[U07] Py：反转字典键值
来源：http://gol.yj20258888.top

{v: k for k, v in d.items()}
来源：http://egt.andypj.xyz

[U08] Py：展平二维列表
来源：http://mys.aibaodan.cn

[y for x in nested for y in x]
来源：http://mcw.jinqigufen.top

[U09] Py：字典取最大值的键
来源：http://pwu.yongpay.top

max(d, key=d.get)
来源：http://yjy.fktsv.cn

[U10] Py：按值排序字典
来源：http://lpk.tian-w.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jho.guannengcc.top

[U11] Py：生成器表达式
来源：http://xgp.c1oappe.top

(x * 2 for x in arr)
来源：http://nhl.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fcp.gogol.net.cn

Counter(arr).most_common(3)
来源：http://ijj.zhijiandao.cn

[U13] Py：固定长度队列
来源：http://uxm.sjlbkw.cn

deque(maxlen=10)
来源：http://dfw.feifeiyinyue.top

[U14] Py：分组收集到列表
来源：http://umd.feifeiyinyue.top

defaultdict(list)
来源：http://fmd.jiagoushi.top

[U15] Py：高精度计时
来源：http://nfq.nwbrower.top

t = time.perf_counter()
来源：http://kyn.ehwqpu.com

[U16] Py：命令行参数解析
来源：http://omn.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sbk.vqdsnc.cn

[U17] Py：初始化日志
来源：http://bcg.tanke756.top

logging.basicConfig(level=logging.INFO)
来源：http://pmg.xingfuxueyuan.xyz

[U18] Py：预编译正则
来源：http://lcz.zhijiandao.cn

pat = re.compile(r"\d+")
来源：http://ktv.zhiwuduotai.top

[U19] Py：正则替换带回调
来源：http://wff.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hkm.fanxiaobao.xyz

[U20] Py：缓存函数结果
来源：http://zhv.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://egw.ppjwa.cn

[U21] Py：自定义上下文管理器
来源：http://xof.pengpengdd.cyou

@contextlib.contextmanager
来源：http://rwj.ybcxt.top

[U22] Py：矩阵转置
来源：http://zyn.aizwys.cn

list(zip(*m))
来源：http://fra.xziqi.cn

[U23] Py：分块读取大文件
来源：http://zxv.ppjwa.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wbn.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://dri.tanke756.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cwr.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://emv.bbcook.cn

csv.DictReader(f)
来源：http://ave.hfpthk.cn

[U26] Py：并发下载
来源：http://wyj.jinqigufen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tfn.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://jgl.yvedp.cn

aiohttp.ClientSession() 配合 async with
来源：http://cqq.snrcjt.cn

[U28] Py：类型别名
来源：http://xgf.bbcook.cn

UserId = int
来源：http://pgl.xziqi.cn

[U29] Py：属性校验
来源：http://ueb.yanxiufei.cn

@property 与 @x.setter 配合
来源：http://scn.xuetiantiany.cn

[U30] Py：数据类
来源：http://ffj.hnxiangtu.top

@dataclass(slots=True)
来源：http://mpf.zdqjudy.top

[U31] Py：单测
来源：http://cgz.52xcode.cn

python -m pytest -q
来源：http://xmz.chenlongwang.top

[U32] Py：代码格式化
来源：http://rsv.yfazqb.com

ruff format . && ruff check --fix .
来源：http://hku.haohaochexian.top

[U33] Py：打包发布
来源：http://duz.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://uwe.xinyue.icu

[U34] Py：判断编码
来源：http://lgr.aizwys.cn

chardet.detect(raw)
来源：http://bsi.wangdashe.top

[U35] Py：发送邮件
来源：http://hcd.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rjh.ivvv.top

[U36] Py：定时任务
来源：http://izn.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://nyw.wangdashe.top

[U37] Py：读写 Excel
来源：http://kbm.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uyb.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://qqu.sjlbkw.cn

Path(__file__).resolve().parent
来源：http://gbv.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://wws.xuetiantiany.cn

sys.stdout.isatty()
来源：http://kbz.tarul.cn

[U40] Py：打印到标准错误
来源：http://dxv.xuetiantiany.cn

print("err", file=sys.stderr)
来源：http://zqg.fanxiaobao.xyz

[U41] PHP：初始化 Composer 项目
来源：http://lmx.daxiang520.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vlz.aizwys.cn

[U42] PHP：PSR-4 自动加载
来源：http://eog.sxryk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xry.0kj1m.cn

[U43] PHP：声明命名空间
来源：http://inc.zhengqikj.top

namespace App\Http;
来源：http://ohx.fanxiaobao.xyz

[U44] PHP：开启严格类型
来源：http://sat.epnwcf.com

declare(strict_types=1);
来源：http://cdm.sweek.top

[U45] PHP：类型声明与返回类型
来源：http://hxs.xingfuxueyuan.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://xqi.xuanzx.com

[U46] PHP：可空类型
来源：http://uqt.quarkkingdee.top

?string $name = null
来源：http://qnz.hnxiangtu.top

[U47] PHP：联合类型
来源：http://htf.guannengcc.top

int|string $id
来源：http://peo.feifeiyinyue.top

[U48] PHP：纯枚举
来源：http://oqg.hnqzz.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vpg.yj20258888.top

[U49] PHP：只读属性
来源：http://hsp.ydjk.org.cn

public readonly string $name
来源：http://olk.cqqwz.cn

[U50] PHP：构造器属性提升
来源：http://cgc.chenjidiqi.icu

public function __construct(private int $id) {}
来源：http://pkh.bjfxy.top

[U51] PHP：数组解构
来源：http://juj.pycfn.com

[$a, $b] = $arr;
来源：http://fnx.yj20258888.top

[U52] PHP：箭头函数
来源：http://zwg.tianlin.xyz

$double = fn($x) => $x * 2;
来源：http://bur.guowangkeji.top

[U53] PHP：空合并运算符
来源：http://jlq.gaohongyu789.top

$v = $a ?? $b ?? "default";
来源：http://kab.zdqjudy.top

[U54] PHP：空安全调用
来源：http://bnk.epnwcf.com

$obj?->method()
来源：http://msn.yfazqb.com

[U55] PHP：match 表达式
来源：http://cev.sysykeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yyy.jinyuanbaomall.cn

[U56] PHP：命名参数
来源：http://ycz.gzhubu.top

f(a: 1, b: 2)
来源：http://egd.xinyue.icu


<!-- 参考信息 -->