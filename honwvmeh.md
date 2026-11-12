代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://uvk.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fzi.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://jmk.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cam.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://bwu.tianlin.xyz

[S49] C++：写文件
来源：http://hqm.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fok.shzxlz.cn

[S50] C++：格式化数字
来源：http://fml.wangshuangyany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://skq.hysaishi.cn

[S51] C++：显式类型转换
来源：http://sah.tarul.cn

static_cast<double>(a) / b
来源：http://szn.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://qrm.tanke756.top

int size() const noexcept { return n_; }
来源：http://hob.hnxiangtu.top

[S53] C++：移动语义
来源：http://aux.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://nrx.xuanzx.com

[S54] C++：异常处理
来源：http://yju.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://khb.hammf.cn

[S55] C++：结构化绑定
来源：http://clu.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cqi.yj202588.top

[S56] C++：optional
来源：http://khp.jqgfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xxm.hnxiangtu.top

[S57] C++：编译期常量
来源：http://pra.shangyingyoupin.top

constexpr int N = 10;
来源：http://scp.cucudq.cn

[S58] C++：命名空间
来源：http://fqz.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://thh.chenzaomai.com

[S59] C++：静态断言
来源：http://nik.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vsd.jinyuanbaomall.cn

[S60] C++：遍历并删除元素
来源：http://kxp.yj202588.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zuc.havefunace.top

================================================================================
来源：http://sxh.shangyingyoupin.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ynx.jinyuanbaomall.cn

================================================================================
来源：http://urp.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://xng.c1oappe.top

println("Hello")
来源：http://wsh.guannengcc.top

[T02] Kotlin：变量
来源：http://rzu.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://adu.yj202588.top

[T03] Kotlin：字符串模板
来源：http://sxz.fanxiaobao.xyz

"值: $b"
来源：http://rgy.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://sjt.ywan-chungtsiang.top

val n: String? = null;  n?.length
来源：http://grd.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://qvp.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jzj.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://llv.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bwx.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://rob.gogol.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://owy.nwbrower.top

[T08] Kotlin：数据类
来源：http://bxg.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://oay.jiagoushi.top

[T09] Kotlin：扩展函数
来源：http://kzb.ybcxt.top

fun String.exclaim() = this + "!"
来源：http://dec.fzhhl.top

[T10] Kotlin：默认参数
来源：http://avv.svipenyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bmw.pengpengdd.cyou

[T11] Kotlin：协程
来源：http://fnd.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ync.dashuyun.cn

[T12] Kotlin：解构声明
来源：http://hbl.yj202588.top

val (a, b) = Pair(1, 2)
来源：http://rus.xuanzx.com

[T13] Kotlin：只读 Map
来源：http://qkx.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://ndb.zycfv.cn

[T14] Kotlin：循环
来源：http://puz.meibo888.top

for (i in 1..10) println(i)
来源：http://haz.guannengcc.top

[T15] Kotlin：接口
来源：http://qgo.nwbrower.top

interface Shape { fun area(): Double }
来源：http://mcr.zdbjq.cn

[T16] Swift：Hello World
来源：http://osj.chenlongwang.top

print("Hello")
来源：http://zle.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://xqt.hywenlv.cn

var a = 1;  let b = 2
来源：http://drv.gotoacloud.top

[T18] Swift：字符串插值
来源：http://gll.dianchejie.cn

"值: \(b)"
来源：http://ybl.cashguo.top

[T19] Swift：可选绑定
来源：http://rim.yanxiufei.cn

if let n = opt { print(n) }
来源：http://prt.hfpthk.cn

[T20] Swift：数组操作
来源：http://oxc.meibo888.top

var a = [1, 2, 3];  a.append(4)
来源：http://qub.fzhhl.top

[T21] Swift：遍历
来源：http://mqz.hesvh.cn

for x in a { print(x) }
来源：http://yzt.fanxiaobao.xyz

[T22] Swift：字典
来源：http://jhi.nwbrower.top

var d = ["a": 1];  d["b"] = 2
来源：http://aap.chenjidiqi.icu

[T23] Swift：函数
来源：http://kgz.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pfn.chenjidiqi.icu

[T24] Swift：闭包
来源：http://mqy.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zlf.yongpay.top

[T25] Swift：结构体
来源：http://lew.cashguo.top

struct P { var x: Int }
来源：http://hyc.sysykeji.top

[T26] Swift：类与重写
来源：http://doy.gaohongyu789.top

class A: Base { override func f() {} }
来源：http://jms.tian-w.cn

[T27] Swift：错误处理
来源：http://mdx.gotoacloud.top

do { try f() } catch { print(error) }
来源：http://vod.kuanghao11.cn

[T28] Swift：枚举
来源：http://faw.svipenyu.cn

enum Color { case red, green }
来源：http://iek.hcnkem.com

[T29] Swift：guard 提前返回
来源：http://mxf.nwbrower.top

guard let x = opt else { return }
来源：http://fgi.wangshuangyany.cn

[T30] Swift：协议
来源：http://ljq.zhaomingkeji.xyz

protocol Shape { func area() -> Double }
来源：http://fph.shanyushiyangtech.top

[T31] Lua：Hello World
来源：http://zmf.xingfuxueyuan.xyz

print("Hello")
来源：http://kyc.jqgufenzy.top

[T32] Lua：局部变量
来源：http://mjb.wangdashe.top

local a = 1
来源：http://mdl.haohaochexian.top

[T33] Lua：表（数组）
来源：http://cot.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://dnt.tianlin.xyz

[T34] Lua：遍历表
来源：http://gkp.hcnkem.com

for i, v in ipairs(t) do print(i, v) end
来源：http://fuf.aibaodan.cn

[T35] Lua：字典表
来源：http://qtm.gogol.net.cn

local d = { a = 1 };  d.b = 2
来源：http://otf.jinyuanbaomall.cn

[T36] Lua：函数
来源：http://ioc.hfpthk.cn

function add(a, b) return a + b end
来源：http://wai.zhengqikj.top

[T37] Lua：字符串拼接
来源：http://yur.ywan-chungtsiang.top

"a" .. "b"
来源：http://pui.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://cii.bjfxy.top

if x > 0 then print("正") end
来源：http://hmq.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://tmc.zhongyouzk.top

string.find(s, "%d+")
来源：http://mfk.svipenyu.cn

[T40] Lua：元表
来源：http://nem.ywan-chungtsiang.top

setmetatable({}, { __index = base })
来源：http://prg.nanxinkj.top

[T41] Perl：Hello World
来源：http://bxg.wangshuangyany.cn

print "Hello\n";
来源：http://vqo.yonumen.top

[T42] Perl：变量类型
来源：http://wne.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lpu.snrcjt.cn

[T43] Perl：字符串插值
来源：http://hno.nwbrower.top

"值: $a"
来源：http://gua.fktsv.cn

[T44] Perl：条件
来源：http://zuk.vehdjk.com

if ($a > 0) { print "正"; }
来源：http://qom.hnqzz.top

[T45] Perl：数组遍历
来源：http://efg.chenlongwang.top

for my $x (@arr) { print $x; }
来源：http://gps.tarul.cn

[T46] Perl：哈希操作
来源：http://dll.hfpthk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dgz.0kj1m.cn

[T47] Perl：正则捕获
来源：http://lcq.jinghuilouyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bya.ybcxt.top

[T48] Perl：正则替换
来源：http://pbl.dianchejie.cn

$s =~ s/old/new/g;
来源：http://big.52xcode.cn

[T49] Perl：函数
来源：http://opa.zdqjudy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pqo.yuanzhike.top

[T50] Perl：逐行读文件
来源：http://fwd.52xcode.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://acp.birdmap.top

while (my $line = <$fh>) { print $line; }
来源：http://eya.andypj.xyz

[T51] Scala：Hello World
来源：http://jcr.hysaishi.cn

println("Hello")
来源：http://wln.yvedp.cn

[T52] Scala：变量
来源：http://ceg.hesvh.cn

val a = 1;  var b = 2
来源：http://whu.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://xzw.hywenlv.cn

s"值: $b"
来源：http://vjl.316326.xyz

[T54] Scala：集合映射
来源：http://krc.nanxuanxn.top

List(1, 2, 3).map(_ * 2)
来源：http://nwi.9152youxi.cn

[T55] Scala：集合过滤
来源：http://okl.sufxvd.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oiu.sjlbkw.cn

[T56] Scala：样例类
来源：http://zze.yvedp.cn

case class User(name: String, age: Int)
来源：http://fib.ydzc1.top

[T57] Scala：模式匹配
来源：http://alv.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fmg.feifeiyinyue.top

[T58] Scala：函数定义
来源：http://xhr.yvedp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ohn.fehbvm.com

[T59] Scala：循环
来源：http://gqa.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://iby.wangshuangyany.cn

[T60] Scala：折叠
来源：http://odg.ybcxt.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gfj.fktsv.cn

================================================================================
来源：http://lxw.ivvv.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://axu.fengsongda.top

================================================================================
来源：http://whn.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://mmd.hesvh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xex.ppjwa.cn

[U02] Py：导出 / 安装依赖
来源：http://hrl.jianghu66.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ctj.meibo888.top

[U03] Py：加载 .env 配置
来源：http://ydq.nanxuanxn.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mey.smart0.xyz

[U04] Py：变量调试打印
来源：http://mig.redwolf501.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://otb.zycfv.cn

[U05] Py：列表去重且保序
来源：http://lul.fktsv.cn

list(dict.fromkeys(arr))
来源：http://euj.tianlin.xyz

[U06] Py：合并两个字典
来源：http://jho.pycfn.com

{**a, **b}
来源：http://kxm.snrcjt.cn

[U07] Py：反转字典键值
来源：http://ypf.hysaishi.cn

{v: k for k, v in d.items()}
来源：http://qhd.hywenlv.cn

[U08] Py：展平二维列表
来源：http://gzc.guannengcc.top

[y for x in nested for y in x]
来源：http://ddp.havefunace.top

[U09] Py：字典取最大值的键
来源：http://hvt.sjlbkw.cn

max(d, key=d.get)
来源：http://vyr.zhiwuduotai.top

[U10] Py：按值排序字典
来源：http://iws.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sgl.zhijiandao.cn

[U11] Py：生成器表达式
来源：http://bok.gogol.net.cn

(x * 2 for x in arr)
来源：http://hry.tianlin.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://hlx.chenlongwang.top

Counter(arr).most_common(3)
来源：http://pzo.bjfxy.top

[U13] Py：固定长度队列
来源：http://uco.vqdsnc.cn

deque(maxlen=10)
来源：http://zqh.nanxuanxn.top

[U14] Py：分组收集到列表
来源：http://ldm.quarkkingdee.top

defaultdict(list)
来源：http://dhd.ybcxt.top

[U15] Py：高精度计时
来源：http://upf.nanxuanxn.top

t = time.perf_counter()
来源：http://obm.yfazqb.com

[U16] Py：命令行参数解析
来源：http://wya.yuxming.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mcm.sjlbkw.cn

[U17] Py：初始化日志
来源：http://ubk.fanxiaobao.xyz

logging.basicConfig(level=logging.INFO)
来源：http://jho.daria6918.cn

[U18] Py：预编译正则
来源：http://gya.hysaishi.cn

pat = re.compile(r"\d+")
来源：http://gln.yuxming.cn

[U19] Py：正则替换带回调
来源：http://lpo.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wfb.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://vpc.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://xot.xinyue.icu

[U21] Py：自定义上下文管理器
来源：http://phq.jinqigfzy.top

@contextlib.contextmanager
来源：http://vyz.fengsongda.top

[U22] Py：矩阵转置
来源：http://rnv.quarkkingdee.top

list(zip(*m))
来源：http://zhg.sysykeji.top

[U23] Py：分块读取大文件
来源：http://zby.zdqjudy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lir.hnxiangtu.top

[U24] Py：路径操作
来源：http://xxi.svipenyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yxe.smart0.xyz

[U25] Py：CSV 按字典读
来源：http://ecl.smart0.xyz

csv.DictReader(f)
来源：http://znv.wangshuangyany.cn

[U26] Py：并发下载
来源：http://zwa.ydzc1.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uxv.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://lya.epnwcf.com

aiohttp.ClientSession() 配合 async with
来源：http://wpm.hnqzz.top

[U28] Py：类型别名
来源：http://uuz.shanyushiyangtech.top

UserId = int
来源：http://lgm.hysaishi.cn

[U29] Py：属性校验
来源：http://pyz.daxiang520.top

@property 与 @x.setter 配合
来源：http://jee.yueranfly.top

[U30] Py：数据类
来源：http://eqv.uphjek.com

@dataclass(slots=True)
来源：http://bfu.redwolf501.top

[U31] Py：单测
来源：http://ast.hesvh.cn

python -m pytest -q
来源：http://lbj.shanyushiyangkeji.top

[U32] Py：代码格式化
来源：http://fwq.hongshengwenyu.top

ruff format . && ruff check --fix .
来源：http://ela.yj20258.top

[U33] Py：打包发布
来源：http://alx.ydzc1.top

python -m build  （依赖 pyproject.toml）
来源：http://ecp.hongshengwenyu.top

[U34] Py：判断编码
来源：http://uat.snrcjt.cn

chardet.detect(raw)
来源：http://qtm.andypj.xyz

[U35] Py：发送邮件
来源：http://zey.quarkkingdee.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mxr.jianghu66.top

[U36] Py：定时任务
来源：http://jqn.chenjidiqi.icu

schedule.every(10).minutes.do(job)
来源：http://jgz.jinqigfzy.top

[U37] Py：读写 Excel
来源：http://rhr.shangyingyoupin.top

pandas.read_excel / DataFrame.to_excel
来源：http://czw.xinyue.icu

[U38] Py：获取脚本所在目录
来源：http://ibi.cucudq.cn

Path(__file__).resolve().parent
来源：http://stv.jqgfzy.top

[U39] Py：判断是否在交互环境
来源：http://grf.wangdashe.top

sys.stdout.isatty()
来源：http://kom.dashuyun.cn

[U40] Py：打印到标准错误
来源：http://cfy.daria6918.cn

print("err", file=sys.stderr)
来源：http://lgc.fengsongda.top

[U41] PHP：初始化 Composer 项目
来源：http://dam.fzhhl.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jxe.yvedp.cn

[U42] PHP：PSR-4 自动加载
来源：http://iww.zhengqikj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://egt.shzxlz.cn

[U43] PHP：声明命名空间
来源：http://jdx.zhoulong.xyz

namespace App\Http;
来源：http://xax.sysykeji.top

[U44] PHP：开启严格类型
来源：http://rvq.hywenlv.cn

declare(strict_types=1);
来源：http://voe.yuxming.cn

[U45] PHP：类型声明与返回类型
来源：http://erj.shangyingyoupin.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://akh.ehwqpu.com

[U46] PHP：可空类型
来源：http://bit.zhiwuduotai.top

?string $name = null
来源：http://apj.xziqi.cn

[U47] PHP：联合类型
来源：http://xoj.guannengcc.top

int|string $id
来源：http://elz.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://bmj.nanxuanxn.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oxe.birdmap.top

[U49] PHP：只读属性
来源：http://dyc.316326.xyz

public readonly string $name
来源：http://dbu.ywan-chungtsiang.top

[U50] PHP：构造器属性提升
来源：http://oge.pycfn.com

public function __construct(private int $id) {}
来源：http://gpk.52xcode.cn

[U51] PHP：数组解构
来源：http://wwr.yonumen.top

[$a, $b] = $arr;
来源：http://hwj.jianghu66.top

[U52] PHP：箭头函数
来源：http://jbm.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://sdx.cdnleiting.top

[U53] PHP：空合并运算符
来源：http://kxt.jinqigufen.top

$v = $a ?? $b ?? "default";
来源：http://bhb.316326.xyz

[U54] PHP：空安全调用
来源：http://ixc.zhixingplan.top

$obj?->method()
来源：http://eas.gaohongyu789.top

[U55] PHP：match 表达式
来源：http://lis.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uvw.fanxiaobao.xyz

[U56] PHP：命名参数
来源：http://qvx.tian-w.cn

f(a: 1, b: 2)
来源：http://hln.hysaishi.cn

[U57] PHP：字符串插值
来源：http://mrl.9152youxi.cn

"值: {$a}"
来源：http://fty.feifeiyinyue.top

[U58] PHP：数组三件套
来源：http://yyk.fzhhl.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zly.nanxuanxn.top

[U59] PHP：自定义排序
来源：http://tqn.cashguo.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://itg.chenlongwang.top

[U60] PHP：JSON 编解码
来源：http://nex.hcnkem.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jgr.jinqigfzy.top

[U61] PHP：正则
来源：http://fke.svipenyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hcy.yuanzhike.top

[U62] PHP：日期对象
来源：http://qxw.hnxiangtu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hws.hfpthk.cn

[U63] PHP：文件读写
来源：http://hel.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ksw.ydjk.org.cn

[U64] PHP：目录遍历
来源：http://idb.yongpay.top

glob("dir/*.php");  scandir("dir");
来源：http://ioy.feifeiyinyue.top

[U65] PHP：会话
来源：http://luu.cheryme.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vlm.dashuyun.cn

[U66] PHP：设置 Cookie
来源：http://uba.aibaodan.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cre.sweek.top

[U67] PHP：处理文件上传
来源：http://grc.ehwqpu.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pyj.iojbl.cn

[U68] PHP：PDO 连接
来源：http://oth.dianchejie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nsw.ydzc1.top

[U69] PHP：PDO 预处理
来源：http://mjp.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tod.sysykeji.top

[U70] PHP：PDO 事务
来源：http://sdv.fehbvm.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://utz.sweek.top

[U71] PHP：抛出异常
来源：http://ctu.zhaomingkeji.xyz

throw new RuntimeException("失败", 500);
来源：http://hnw.zdqjudy.top

[U72] PHP：写错误日志
来源：http://jme.zhoulong.xyz

error_log("失败: " . $e->getMessage());
来源：http://lur.hammf.cn


<!-- 参考信息 -->