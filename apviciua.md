代发 wailian999

[S45] C++：lambda
来源：http://bxb.yj20258.top

auto add = [](int a, int b) { return a + b; };
来源：http://itu.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://bxk.xziqi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mgn.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://ygm.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vux.jinqigfzy.top

[S48] C++：逐行读文件
来源：http://dar.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://kmr.jianghu66.top

while (std::getline(in, line)) { }
来源：http://qlo.hnxiangtu.top

[S49] C++：写文件
来源：http://sgf.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fiq.ydzc1.top

[S50] C++：格式化数字
来源：http://nny.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zvl.redwolf501.top

[S51] C++：显式类型转换
来源：http://qgb.jianghu66.top

static_cast<double>(a) / b
来源：http://zrk.shanyushiyangtech.top

[S52] C++：const 与 noexcept
来源：http://xtm.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://eih.snrcjt.cn

[S53] C++：移动语义
来源：http://zxp.chenzaomai.com

std::vector<int> w = std::move(v);
来源：http://rpe.gzhubu.top

[S54] C++：异常处理
来源：http://tgg.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eqd.316326.xyz

[S55] C++：结构化绑定
来源：http://ebk.cucudq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pwi.gotoacloud.top

[S56] C++：optional
来源：http://ljf.zhongyouzk.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rad.nanxinkj.top

[S57] C++：编译期常量
来源：http://vkq.nanxuanxn.top

constexpr int N = 10;
来源：http://ueb.cdnleiting.top

[S58] C++：命名空间
来源：http://bxp.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://pto.xuetiantiany.cn

[S59] C++：静态断言
来源：http://mgg.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kjz.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://jdb.9152youxi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blu.pycfn.com

================================================================================
来源：http://mzj.mhx1999.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://apd.gogol.net.cn

================================================================================
来源：http://qfa.hesvh.cn

[T01] Kotlin：Hello World
来源：http://bia.xingfuxueyuan.xyz

println("Hello")
来源：http://ipy.birdmap.top

[T02] Kotlin：变量
来源：http://dwl.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://erm.yj20258.top

[T03] Kotlin：字符串模板
来源：http://sbv.yj20258.top

"值: $b"
来源：http://bpp.uphjek.com

[T04] Kotlin：空安全
来源：http://wan.xziqi.cn

val n: String? = null;  n?.length
来源：http://msr.hnqzz.top

[T05] Kotlin：when 表达式
来源：http://kfc.shanyushiyangtech.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qmi.nwbrower.top

[T06] Kotlin：集合映射
来源：http://ooj.zhijiandao.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zuu.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://yku.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xvf.epnwcf.com

[T08] Kotlin：数据类
来源：http://ric.c1oappe.top

data class User(val name: String, val age: Int)
来源：http://rkr.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://wck.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://zne.ydzc1.top

[T10] Kotlin：默认参数
来源：http://ftv.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://jna.sweek.top

[T11] Kotlin：协程
来源：http://qax.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cpc.hammf.cn

[T12] Kotlin：解构声明
来源：http://sfj.hywenlv.cn

val (a, b) = Pair(1, 2)
来源：http://fqq.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://zra.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://jta.yueranfly.top

[T14] Kotlin：循环
来源：http://hqf.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://vsy.zycfv.cn

[T15] Kotlin：接口
来源：http://kpw.c1oappe.top

interface Shape { fun area(): Double }
来源：http://tbm.jianghu66.top

[T16] Swift：Hello World
来源：http://vsy.jinyuanbaomall.cn

print("Hello")
来源：http://jun.shzxlz.cn

[T17] Swift：变量与常量
来源：http://swd.cheryme.top

var a = 1;  let b = 2
来源：http://vtw.ppjwa.cn

[T18] Swift：字符串插值
来源：http://rec.jlsjyb.cn

"值: \(b)"
来源：http://csb.quarkkingdee.top

[T19] Swift：可选绑定
来源：http://ybs.zhengqikj.top

if let n = opt { print(n) }
来源：http://ixs.xylfe.cn

[T20] Swift：数组操作
来源：http://qfh.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://vpr.dashuyun.cn

[T21] Swift：遍历
来源：http://lqx.hnxiangtu.top

for x in a { print(x) }
来源：http://vgf.zhijiandao.cn

[T22] Swift：字典
来源：http://zyh.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://rpq.jinyuanbaomall.cn

[T23] Swift：函数
来源：http://qky.yongpay.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vnx.ydjk.org.cn

[T24] Swift：闭包
来源：http://iow.hnxiangtu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://noj.ybcxt.top

[T25] Swift：结构体
来源：http://ryg.quarkkingdee.top

struct P { var x: Int }
来源：http://tzl.jlsjyb.cn

[T26] Swift：类与重写
来源：http://yoc.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://maz.hnxiangtu.top

[T27] Swift：错误处理
来源：http://fom.birdmap.top

do { try f() } catch { print(error) }
来源：http://uwr.redwolf501.top

[T28] Swift：枚举
来源：http://cko.guannengcc.top

enum Color { case red, green }
来源：http://syq.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://ogx.fengsongda.top

guard let x = opt else { return }
来源：http://glk.daxiang520.top

[T30] Swift：协议
来源：http://hzl.jianghu66.top

protocol Shape { func area() -> Double }
来源：http://smu.smart0.xyz

[T31] Lua：Hello World
来源：http://eqk.ctjpmb.com

print("Hello")
来源：http://acy.guannengcc.top

[T32] Lua：局部变量
来源：http://yus.sxryk.cn

local a = 1
来源：http://jtv.yj20258888.top

[T33] Lua：表（数组）
来源：http://vzi.nwbrower.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rfp.zhongyouzk.top

[T34] Lua：遍历表
来源：http://ddq.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vcz.hammf.cn

[T35] Lua：字典表
来源：http://ggp.yuxming.cn

local d = { a = 1 };  d.b = 2
来源：http://sae.haohaochexian.top

[T36] Lua：函数
来源：http://dpe.svipenyu.cn

function add(a, b) return a + b end
来源：http://gyh.sxryk.cn

[T37] Lua：字符串拼接
来源：http://utc.gotoacloud.top

"a" .. "b"
来源：http://vmv.yj202588.top

[T38] Lua：条件
来源：http://ace.nanxinkj.top

if x > 0 then print("正") end
来源：http://ral.yuanzhike.top

[T39] Lua：模式匹配
来源：http://yhq.nanxinkj.top

string.find(s, "%d+")
来源：http://ykn.chenzaomai.com

[T40] Lua：元表
来源：http://gja.cheryme.top

setmetatable({}, { __index = base })
来源：http://cxw.jlsjyb.cn

[T41] Perl：Hello World
来源：http://igi.yuanzhike.top

print "Hello\n";
来源：http://uga.xziqi.cn

[T42] Perl：变量类型
来源：http://tfv.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wbo.meibo888.top

[T43] Perl：字符串插值
来源：http://qkp.fktsv.cn

"值: $a"
来源：http://xtx.gotoacloud.top

[T44] Perl：条件
来源：http://fee.zdbjq.cn

if ($a > 0) { print "正"; }
来源：http://tyc.pycfn.com

[T45] Perl：数组遍历
来源：http://exr.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://fiu.daxiang520.top

[T46] Perl：哈希操作
来源：http://zbe.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uen.havefunace.top

[T47] Perl：正则捕获
来源：http://eet.cashguo.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yme.sweek.top

[T48] Perl：正则替换
来源：http://dly.sxryk.cn

$s =~ s/old/new/g;
来源：http://yns.cdnleiting.top

[T49] Perl：函数
来源：http://glz.ydjk.org.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cuy.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://zdh.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gyx.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://mrl.zhoulong.xyz

[T51] Scala：Hello World
来源：http://cbs.mhx1999.top

println("Hello")
来源：http://yol.redwolf501.top

[T52] Scala：变量
来源：http://raw.zhiwuduotai.top

val a = 1;  var b = 2
来源：http://crt.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://kbi.aizwys.cn

s"值: $b"
来源：http://npt.uphjek.com

[T54] Scala：集合映射
来源：http://rbg.gotoacloud.top

List(1, 2, 3).map(_ * 2)
来源：http://xjh.hammf.cn

[T55] Scala：集合过滤
来源：http://lxb.zycfv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tsx.xuetiantiany.cn

[T56] Scala：样例类
来源：http://erv.sweek.top

case class User(name: String, age: Int)
来源：http://liw.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://bob.guannengcc.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uvq.cdnleiting.top

[T58] Scala：函数定义
来源：http://sad.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iar.yuanzhike.top

[T59] Scala：循环
来源：http://amh.ppjwa.cn

for (i <- 1 to 10) println(i)
来源：http://twn.sufxvd.cn

[T60] Scala：折叠
来源：http://ewe.xuanzx.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sot.yfazqb.com

================================================================================
来源：http://gfp.uphjek.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dbq.nwbrower.top

================================================================================
来源：http://oup.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://pdx.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://cvh.hongshengwenyu.top

[U02] Py：导出 / 安装依赖
来源：http://kmv.birdmap.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ydm.cheryme.top

[U03] Py：加载 .env 配置
来源：http://hri.jinyuanbaomall.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mxz.hfpthk.cn

[U04] Py：变量调试打印
来源：http://dch.ywan-chungtsiang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bit.sjlbkw.cn

[U05] Py：列表去重且保序
来源：http://etf.sjlbkw.cn

list(dict.fromkeys(arr))
来源：http://oen.xingfuxueyuan.xyz

[U06] Py：合并两个字典
来源：http://btd.fanxiaobao.xyz

{**a, **b}
来源：http://iiw.jinqigufen.top

[U07] Py：反转字典键值
来源：http://pwv.jianghu66.top

{v: k for k, v in d.items()}
来源：http://rmm.zhixingplan.top

[U08] Py：展平二维列表
来源：http://hxr.guowangkeji.top

[y for x in nested for y in x]
来源：http://wcq.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://vvg.gogol.net.cn

max(d, key=d.get)
来源：http://mni.shzxlz.cn

[U10] Py：按值排序字典
来源：http://twn.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nrv.yangfankeji.com

[U11] Py：生成器表达式
来源：http://cfo.yj20258.top

(x * 2 for x in arr)
来源：http://sbm.cdnleiting.top

[U12] Py：取出现最多的 3 个元素
来源：http://hgz.ybcxt.top

Counter(arr).most_common(3)
来源：http://ocx.tian-w.cn

[U13] Py：固定长度队列
来源：http://joi.snrcjt.cn

deque(maxlen=10)
来源：http://fcx.ydzc1.top

[U14] Py：分组收集到列表
来源：http://evv.wangdashe.top

defaultdict(list)
来源：http://dsp.xingfuxueyuan.xyz

[U15] Py：高精度计时
来源：http://lxy.tian-w.cn

t = time.perf_counter()
来源：http://miy.jinqigufen.top

[U16] Py：命令行参数解析
来源：http://nwd.zhongyouzk.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nxp.shzxlz.cn

[U17] Py：初始化日志
来源：http://ueg.zycfv.cn

logging.basicConfig(level=logging.INFO)
来源：http://xqz.ctjpmb.com

[U18] Py：预编译正则
来源：http://byo.yfazqb.com

pat = re.compile(r"\d+")
来源：http://uxl.jinghuilouyu.cn

[U19] Py：正则替换带回调
来源：http://cyx.shanyushiyangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yhd.fengsongda.top

[U20] Py：缓存函数结果
来源：http://kxc.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://mjs.xinyue.icu

[U21] Py：自定义上下文管理器
来源：http://xdk.yfazqb.com

@contextlib.contextmanager
来源：http://yjo.hnqzz.top

[U22] Py：矩阵转置
来源：http://oks.shzxlz.cn

list(zip(*m))
来源：http://qsj.tanke756.top

[U23] Py：分块读取大文件
来源：http://qot.zycfv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://enw.zhijiandao.cn

[U24] Py：路径操作
来源：http://ljg.yuxming.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baa.sysykeji.top

[U25] Py：CSV 按字典读
来源：http://dtn.kuanghao11.cn

csv.DictReader(f)
来源：http://ofx.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://ajh.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oxv.svipenyu.cn

[U27] Py：异步 HTTP
来源：http://unz.guowangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://evp.jinqigfzy.top

[U28] Py：类型别名
来源：http://uxk.ctjpmb.com

UserId = int
来源：http://krd.c1oappe.top

[U29] Py：属性校验
来源：http://vil.uphjek.com

@property 与 @x.setter 配合
来源：http://kif.yuxming.cn

[U30] Py：数据类
来源：http://sro.shangyingyoupin.top

@dataclass(slots=True)
来源：http://obl.guannengcc.top

[U31] Py：单测
来源：http://asj.zhengqikj.top

python -m pytest -q
来源：http://kby.chenlongwang.top

[U32] Py：代码格式化
来源：http://mhy.yongpay.top

ruff format . && ruff check --fix .
来源：http://brr.epnwcf.com

[U33] Py：打包发布
来源：http://utf.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://pwk.xinyue.icu

[U34] Py：判断编码
来源：http://mlz.xziqi.cn

chardet.detect(raw)
来源：http://rsl.cucudq.cn

[U35] Py：发送邮件
来源：http://zeu.xziqi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ils.zhoulong.xyz

[U36] Py：定时任务
来源：http://nyn.ehwqpu.com

schedule.every(10).minutes.do(job)
来源：http://lcq.ydjk.org.cn

[U37] Py：读写 Excel
来源：http://qup.daxiang520.top

pandas.read_excel / DataFrame.to_excel
来源：http://dcd.havefunace.top

[U38] Py：获取脚本所在目录
来源：http://iwy.ybcxt.top

Path(__file__).resolve().parent
来源：http://gwe.yongpay.top

[U39] Py：判断是否在交互环境
来源：http://nos.zhiwuduotai.top

sys.stdout.isatty()
来源：http://xhf.cheryme.top

[U40] Py：打印到标准错误
来源：http://gia.fehbvm.com

print("err", file=sys.stderr)
来源：http://nwv.fzhhl.top

[U41] PHP：初始化 Composer 项目
来源：http://hdx.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://prc.jinyuanbaomall.cn

[U42] PHP：PSR-4 自动加载
来源：http://zwm.316326.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iea.cdnleiting.top

[U43] PHP：声明命名空间
来源：http://zbj.feifeiyinyue.top

namespace App\Http;
来源：http://yhu.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://cpn.bjfxy.top

declare(strict_types=1);
来源：http://zgh.hammf.cn

[U45] PHP：类型声明与返回类型
来源：http://xeo.xylfe.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tha.gogol.net.cn

[U46] PHP：可空类型
来源：http://jka.gogol.net.cn

?string $name = null
来源：http://xnt.shanyushiyangkeji.top

[U47] PHP：联合类型
来源：http://cms.shzxlz.cn

int|string $id
来源：http://ard.jlsjyb.cn

[U48] PHP：纯枚举
来源：http://jgm.guannengcc.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aph.yj20258888.top

[U49] PHP：只读属性
来源：http://eko.zhijiandao.cn

public readonly string $name
来源：http://psy.fehbvm.com

[U50] PHP：构造器属性提升
来源：http://nhm.bbcook.cn

public function __construct(private int $id) {}
来源：http://fan.xingfuxueyuan.xyz

[U51] PHP：数组解构
来源：http://mmn.gzhubu.top

[$a, $b] = $arr;
来源：http://blo.chenlongwang.top

[U52] PHP：箭头函数
来源：http://hiz.mhx1999.top

$double = fn($x) => $x * 2;
来源：http://xdc.jianghu66.top

[U53] PHP：空合并运算符
来源：http://teq.jinyuanbaomall.cn

$v = $a ?? $b ?? "default";
来源：http://chu.zdqjudy.top

[U54] PHP：空安全调用
来源：http://ahe.yonumen.top

$obj?->method()
来源：http://sxl.epnwcf.com

[U55] PHP：match 表达式
来源：http://yfy.ywan-chungtsiang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jti.sjlbkw.cn

[U56] PHP：命名参数
来源：http://owe.zhixingplan.top

f(a: 1, b: 2)
来源：http://eff.andypj.xyz

[U57] PHP：字符串插值
来源：http://iun.dianchejie.cn

"值: {$a}"
来源：http://rem.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://dti.vehdjk.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gpm.haohaochexian.top

[U59] PHP：自定义排序
来源：http://zbb.tianlin.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uhi.cqqwz.cn

[U60] PHP：JSON 编解码
来源：http://swi.tanke756.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://old.zycfv.cn

[U61] PHP：正则
来源：http://gdc.shangyingyoupin.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gth.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://fgo.shzxlz.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jcs.jyoumei.cn

[U63] PHP：文件读写
来源：http://dfk.cheryme.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yfy.wangdashe.top

[U64] PHP：目录遍历
来源：http://isl.chenjidiqi.icu

glob("dir/*.php");  scandir("dir");
来源：http://qjl.yuxming.cn

[U65] PHP：会话
来源：http://xzo.kuanghao11.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wmm.andypj.xyz

[U66] PHP：设置 Cookie
来源：http://ijp.meibo888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://day.daxiang520.top

[U67] PHP：处理文件上传
来源：http://urh.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dih.wangshuangyany.cn

[U68] PHP：PDO 连接
来源：http://dhs.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://srb.hcnkem.com

[U69] PHP：PDO 预处理
来源：http://fxc.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://icj.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://plc.haohaochexian.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hfv.meibo888.top


<!-- 参考信息 -->