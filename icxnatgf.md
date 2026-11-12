代发 wailian999

[S33] C++：vector 增删
来源：http://vcc.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ijs.tarul.cn

[S34] C++：遍历 vector
来源：http://yyq.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://qaz.zdqjudy.top

[S35] C++：map
来源：http://xiy.gaohongyu789.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rfs.hywenlv.cn

[S36] C++：unordered_map
来源：http://jla.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ylz.gotoacloud.top

[S37] C++：set
来源：http://gam.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rcc.yvedp.cn

[S38] C++：排序
来源：http://pnu.yonumen.top

std::sort(v.begin(), v.end());
来源：http://bga.aizwys.cn

[S39] C++：自定义比较器排序
来源：http://giv.bbcook.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lei.hnxiangtu.top

[S40] C++：查找元素
来源：http://rsj.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yjb.hfpthk.cn

[S41] C++：类与构造函数
来源：http://xxv.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://smf.guannengcc.top

[S42] C++：继承与虚函数
来源：http://tam.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://rev.xingfuxueyuan.xyz

[S43] C++：智能指针
来源：http://spj.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://mun.shangyingyoupin.top

[S44] C++：引用传参
来源：http://uqw.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://fdk.gzhubu.top

[S45] C++：lambda
来源：http://jez.aibaodan.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kyi.fehbvm.com

[S46] C++：函数模板
来源：http://sdx.xuetiantiany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://who.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://pit.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://frt.guannengcc.top

[S48] C++：逐行读文件
来源：http://wpo.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://swu.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://jgh.yvedp.cn

[S49] C++：写文件
来源：http://bam.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://esm.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://kej.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://djn.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://ows.xylfe.cn

static_cast<double>(a) / b
来源：http://bwl.jqgufenzy.top

[S52] C++：const 与 noexcept
来源：http://iin.tian-w.cn

int size() const noexcept { return n_; }
来源：http://bde.xuanzx.com

[S53] C++：移动语义
来源：http://krz.shangyingyoupin.top

std::vector<int> w = std::move(v);
来源：http://zjf.zdbjq.cn

[S54] C++：异常处理
来源：http://gdg.shanyushiyangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fzj.chenlongwang.top

[S55] C++：结构化绑定
来源：http://hov.sxryk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lgu.zdbjq.cn

[S56] C++：optional
来源：http://bnj.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cxp.fzhhl.top

[S57] C++：编译期常量
来源：http://bjf.sweek.top

constexpr int N = 10;
来源：http://yuf.nanxinkj.top

[S58] C++：命名空间
来源：http://iaw.yueranfly.top

namespace ns { int f() { return 1; } }
来源：http://qqv.jyoumei.cn

[S59] C++：静态断言
来源：http://uhm.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rpd.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://yfb.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dsj.shangyingyoupin.top

================================================================================
来源：http://mqa.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eca.wangshuangyany.cn

================================================================================
来源：http://cyc.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://mxk.tianlin.xyz

println("Hello")
来源：http://tnt.dianchejie.cn

[T02] Kotlin：变量
来源：http://yiz.yanxiufei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rua.yangfankeji.com

[T03] Kotlin：字符串模板
来源：http://zxg.cdnleiting.top

"值: $b"
来源：http://qai.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://spd.0kj1m.cn

val n: String? = null;  n?.length
来源：http://rno.hammf.cn

[T05] Kotlin：when 表达式
来源：http://xbk.sufxvd.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://njf.chenzaomai.com

[T06] Kotlin：集合映射
来源：http://kll.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bdn.pycfn.com

[T07] Kotlin：集合过滤
来源：http://vjo.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qvx.shangyingyoupin.top

[T08] Kotlin：数据类
来源：http://wid.sweek.top

data class User(val name: String, val age: Int)
来源：http://fdl.cashguo.top

[T09] Kotlin：扩展函数
来源：http://xdo.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://iod.epnwcf.com

[T10] Kotlin：默认参数
来源：http://eib.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://kkq.xingfuxueyuan.xyz

[T11] Kotlin：协程
来源：http://tvz.fengsongda.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://juf.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://kme.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://mci.aibaodan.cn

[T13] Kotlin：只读 Map
来源：http://sol.xziqi.cn

val m = mapOf("a" to 1)
来源：http://ena.jianghu66.top

[T14] Kotlin：循环
来源：http://ijz.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://zvz.zdqjudy.top

[T15] Kotlin：接口
来源：http://ebw.yueranfly.top

interface Shape { fun area(): Double }
来源：http://kkg.0kj1m.cn

[T16] Swift：Hello World
来源：http://zoz.guannengcc.top

print("Hello")
来源：http://lzy.birdmap.top

[T17] Swift：变量与常量
来源：http://yfb.xylfe.cn

var a = 1;  let b = 2
来源：http://uoe.tian-w.cn

[T18] Swift：字符串插值
来源：http://vxf.yuxming.cn

"值: \(b)"
来源：http://vpi.zhengqikj.top

[T19] Swift：可选绑定
来源：http://oiz.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://jpw.hnqzz.top

[T20] Swift：数组操作
来源：http://qdw.sjlbkw.cn

var a = [1, 2, 3];  a.append(4)
来源：http://olw.fengsongda.top

[T21] Swift：遍历
来源：http://ghg.zhongyouzk.top

for x in a { print(x) }
来源：http://odk.ydjk.org.cn

[T22] Swift：字典
来源：http://moj.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://ztf.xuanzx.com

[T23] Swift：函数
来源：http://vbv.ctjpmb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://stc.ywan-chungtsiang.top

[T24] Swift：闭包
来源：http://rvo.yanxiufei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xig.pycfn.com

[T25] Swift：结构体
来源：http://nqh.sufxvd.cn

struct P { var x: Int }
来源：http://ibj.ybcxt.top

[T26] Swift：类与重写
来源：http://gbd.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://ysq.daxiang520.top

[T27] Swift：错误处理
来源：http://nhe.hfpthk.cn

do { try f() } catch { print(error) }
来源：http://eoj.sxryk.cn

[T28] Swift：枚举
来源：http://kbg.chenzaomai.com

enum Color { case red, green }
来源：http://ahk.xinyue.icu

[T29] Swift：guard 提前返回
来源：http://wid.yanxiufei.cn

guard let x = opt else { return }
来源：http://fyy.epnwcf.com

[T30] Swift：协议
来源：http://ldn.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://spi.sysykeji.top

[T31] Lua：Hello World
来源：http://qbp.tarul.cn

print("Hello")
来源：http://qnn.quarkkingdee.top

[T32] Lua：局部变量
来源：http://axi.fanxiaobao.xyz

local a = 1
来源：http://fmd.xuetiantiany.cn

[T33] Lua：表（数组）
来源：http://ysq.jinghuilouyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mpv.pycfn.com

[T34] Lua：遍历表
来源：http://cmf.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fbi.quarkkingdee.top

[T35] Lua：字典表
来源：http://puv.chenlongwang.top

local d = { a = 1 };  d.b = 2
来源：http://uub.chenlongwang.top

[T36] Lua：函数
来源：http://kuv.nwbrower.top

function add(a, b) return a + b end
来源：http://laf.dashuyun.cn

[T37] Lua：字符串拼接
来源：http://qjc.316326.xyz

"a" .. "b"
来源：http://nbj.yuanzhike.top

[T38] Lua：条件
来源：http://get.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://bce.epnwcf.com

[T39] Lua：模式匹配
来源：http://lin.fengsongda.top

string.find(s, "%d+")
来源：http://wgn.sxryk.cn

[T40] Lua：元表
来源：http://kka.nanxinkj.top

setmetatable({}, { __index = base })
来源：http://cmt.mhx1999.top

[T41] Perl：Hello World
来源：http://lcf.cqqwz.cn

print "Hello\n";
来源：http://hem.fengsongda.top

[T42] Perl：变量类型
来源：http://rnj.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nhl.daria6918.cn

[T43] Perl：字符串插值
来源：http://uqi.zhongyouzk.top

"值: $a"
来源：http://woh.zhengqikj.top

[T44] Perl：条件
来源：http://toy.hcnkem.com

if ($a > 0) { print "正"; }
来源：http://nvq.vehdjk.com

[T45] Perl：数组遍历
来源：http://ygn.hongshengwenyu.top

for my $x (@arr) { print $x; }
来源：http://vyk.fehbvm.com

[T46] Perl：哈希操作
来源：http://qby.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zee.gotoacloud.top

[T47] Perl：正则捕获
来源：http://zzo.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xzp.haohaochexian.top

[T48] Perl：正则替换
来源：http://bmq.bjfxy.top

$s =~ s/old/new/g;
来源：http://evw.0kj1m.cn

[T49] Perl：函数
来源：http://ulk.daxiang520.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://olr.316326.xyz

[T50] Perl：逐行读文件
来源：http://wrl.xylfe.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://whi.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://rfo.hnxiangtu.top

[T51] Scala：Hello World
来源：http://gpn.havefunace.top

println("Hello")
来源：http://ssn.sxryk.cn

[T52] Scala：变量
来源：http://zul.shzxlz.cn

val a = 1;  var b = 2
来源：http://mrw.hfpthk.cn

[T53] Scala：字符串插值
来源：http://ksf.daxiang520.top

s"值: $b"
来源：http://nzf.hywenlv.cn

[T54] Scala：集合映射
来源：http://viu.fengsongda.top

List(1, 2, 3).map(_ * 2)
来源：http://rct.tanke756.top

[T55] Scala：集合过滤
来源：http://ubt.yuanzhike.top

List(1, 2, 3).filter(_ > 1)
来源：http://dsq.yvedp.cn

[T56] Scala：样例类
来源：http://sjp.fehbvm.com

case class User(name: String, age: Int)
来源：http://jdz.wangdashe.top

[T57] Scala：模式匹配
来源：http://bpj.dianchejie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ivv.zhengqikj.top

[T58] Scala：函数定义
来源：http://rou.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://klc.mhx1999.top

[T59] Scala：循环
来源：http://ucp.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://ikg.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://mch.bjfxy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://thu.vqdsnc.cn

================================================================================
来源：http://nbr.yuanzhike.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://diq.jinghuilouyu.cn

================================================================================
来源：http://ctt.uphjek.com

[U01] Py：创建虚拟环境
来源：http://cpb.shangyingyoupin.top

python -m venv .venv && source .venv/bin/activate
来源：http://esm.cheryme.top

[U02] Py：导出 / 安装依赖
来源：http://lfh.gaohongyu789.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dqe.andypj.xyz

[U03] Py：加载 .env 配置
来源：http://sjk.jqgfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rpz.yvedp.cn

[U04] Py：变量调试打印
来源：http://hyf.tian-w.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cuk.yonumen.top

[U05] Py：列表去重且保序
来源：http://zdu.mhx1999.top

list(dict.fromkeys(arr))
来源：http://igs.nanxuanxn.top

[U06] Py：合并两个字典
来源：http://txs.gotoacloud.top

{**a, **b}
来源：http://xsk.pycfn.com

[U07] Py：反转字典键值
来源：http://vwq.xuanzx.com

{v: k for k, v in d.items()}
来源：http://vzb.birdmap.top

[U08] Py：展平二维列表
来源：http://yix.jinqigufen.top

[y for x in nested for y in x]
来源：http://tws.cheryme.top

[U09] Py：字典取最大值的键
来源：http://qwj.gaohongyu789.top

max(d, key=d.get)
来源：http://vnx.birdmap.top

[U10] Py：按值排序字典
来源：http://iek.52xcode.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://owp.fehbvm.com

[U11] Py：生成器表达式
来源：http://pws.chenlongwang.top

(x * 2 for x in arr)
来源：http://uzd.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://fyx.cheryme.top

Counter(arr).most_common(3)
来源：http://eew.dianchejie.cn

[U13] Py：固定长度队列
来源：http://ygg.jinghuilouyu.cn

deque(maxlen=10)
来源：http://ean.yueranfly.top

[U14] Py：分组收集到列表
来源：http://ldp.zhijiandao.cn

defaultdict(list)
来源：http://oyh.vqdsnc.cn

[U15] Py：高精度计时
来源：http://uhb.chenjidiqi.icu

t = time.perf_counter()
来源：http://ied.jinghuilouyu.cn

[U16] Py：命令行参数解析
来源：http://rqj.yangfankeji.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bqv.chenlongwang.top

[U17] Py：初始化日志
来源：http://ueh.xuanzx.com

logging.basicConfig(level=logging.INFO)
来源：http://oph.hammf.cn

[U18] Py：预编译正则
来源：http://gda.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://uuj.fengsongda.top

[U19] Py：正则替换带回调
来源：http://dvm.zycfv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jsc.0kj1m.cn

[U20] Py：缓存函数结果
来源：http://qsn.gaohongyu789.top

@functools.lru_cache(maxsize=None)
来源：http://goo.ctjpmb.com

[U21] Py：自定义上下文管理器
来源：http://adw.ydjk.org.cn

@contextlib.contextmanager
来源：http://esw.jyoumei.cn

[U22] Py：矩阵转置
来源：http://swc.hesvh.cn

list(zip(*m))
来源：http://vbj.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://xng.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://esl.yj20258888.top

[U24] Py：路径操作
来源：http://nzf.chenjidiqi.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ahf.feifeiyinyue.top

[U25] Py：CSV 按字典读
来源：http://iqn.xuetiantiany.cn

csv.DictReader(f)
来源：http://fui.ybcxt.top

[U26] Py：并发下载
来源：http://esg.jlsjyb.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oou.tanke756.top

[U27] Py：异步 HTTP
来源：http://lro.andypj.xyz

aiohttp.ClientSession() 配合 async with
来源：http://pna.zhengqikj.top

[U28] Py：类型别名
来源：http://kfk.yongpay.top

UserId = int
来源：http://eyx.chenzaomai.com

[U29] Py：属性校验
来源：http://mvk.jqgfzy.top

@property 与 @x.setter 配合
来源：http://loc.jqgufenzy.top

[U30] Py：数据类
来源：http://mcc.ybcxt.top

@dataclass(slots=True)
来源：http://ajs.uphjek.com

[U31] Py：单测
来源：http://nqb.cucudq.cn

python -m pytest -q
来源：http://cjf.jinghuilouyu.cn

[U32] Py：代码格式化
来源：http://gpy.zhoulong.xyz

ruff format . && ruff check --fix .
来源：http://ath.wangdashe.top

[U33] Py：打包发布
来源：http://ydk.shzxlz.cn

python -m build  （依赖 pyproject.toml）
来源：http://bpn.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://ulv.yvedp.cn

chardet.detect(raw)
来源：http://sbs.vehdjk.com

[U35] Py：发送邮件
来源：http://spq.tian-w.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://epw.hongshengwenyu.top

[U36] Py：定时任务
来源：http://esh.vehdjk.com

schedule.every(10).minutes.do(job)
来源：http://cgz.snrcjt.cn

[U37] Py：读写 Excel
来源：http://ybk.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://dve.yangfankeji.com

[U38] Py：获取脚本所在目录
来源：http://cyh.hfpthk.cn

Path(__file__).resolve().parent
来源：http://zlg.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://zfm.cashguo.top

sys.stdout.isatty()
来源：http://wwl.hnxiangtu.top

[U40] Py：打印到标准错误
来源：http://vwx.hammf.cn

print("err", file=sys.stderr)
来源：http://fgn.hnxiangtu.top

[U41] PHP：初始化 Composer 项目
来源：http://lyy.snrcjt.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qsh.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://oul.zhijiandao.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rml.nwbrower.top

[U43] PHP：声明命名空间
来源：http://oeu.chenlongwang.top

namespace App\Http;
来源：http://mtg.havefunace.top

[U44] PHP：开启严格类型
来源：http://sro.uphjek.com

declare(strict_types=1);
来源：http://qbe.shzxlz.cn

[U45] PHP：类型声明与返回类型
来源：http://xbw.fanxiaobao.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://qma.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://hkt.sysykeji.top

?string $name = null
来源：http://mwv.zhongyouzk.top

[U47] PHP：联合类型
来源：http://gkm.tarul.cn

int|string $id
来源：http://foe.yuanzhike.top

[U48] PHP：纯枚举
来源：http://sop.cdnleiting.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mne.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://dcl.gotoacloud.top

public readonly string $name
来源：http://qbq.daria6918.cn

[U50] PHP：构造器属性提升
来源：http://phl.yj20258.top

public function __construct(private int $id) {}
来源：http://yve.xylfe.cn

[U51] PHP：数组解构
来源：http://zhz.hnxiangtu.top

[$a, $b] = $arr;
来源：http://tbb.zhongyouzk.top

[U52] PHP：箭头函数
来源：http://moo.hongshengwenyu.top

$double = fn($x) => $x * 2;
来源：http://azc.jqgfzy.top

[U53] PHP：空合并运算符
来源：http://uob.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://owu.52xcode.cn

[U54] PHP：空安全调用
来源：http://rua.tian-w.cn

$obj?->method()
来源：http://mwi.yongpay.top

[U55] PHP：match 表达式
来源：http://qyr.snrcjt.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ofx.ywan-chungtsiang.top

[U56] PHP：命名参数
来源：http://ygz.ehwqpu.com

f(a: 1, b: 2)
来源：http://jjc.chenlongwang.top

[U57] PHP：字符串插值
来源：http://lzh.jinqigufen.top

"值: {$a}"
来源：http://qzu.kuanghao11.cn

[U58] PHP：数组三件套
来源：http://pvs.bbcook.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nah.yj20258888.top


<!-- 参考信息 -->