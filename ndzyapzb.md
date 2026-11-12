代发 wailian999

while (std::getline(in, line)) { }
来源：http://snn.zycfv.cn

[S49] C++：写文件
来源：http://yug.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qhc.ybcxt.top

[S50] C++：格式化数字
来源：http://nzc.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zvk.smart0.xyz

[S51] C++：显式类型转换
来源：http://jzd.gogol.net.cn

static_cast<double>(a) / b
来源：http://gez.cheryme.top

[S52] C++：const 与 noexcept
来源：http://iyl.chenlongwang.top

int size() const noexcept { return n_; }
来源：http://nvv.aibaodan.cn

[S53] C++：移动语义
来源：http://gcf.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://jsu.nanxuanxn.top

[S54] C++：异常处理
来源：http://myw.jqgufenzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yqt.hcnkem.com

[S55] C++：结构化绑定
来源：http://kgj.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ujb.fktsv.cn

[S56] C++：optional
来源：http://iwr.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mnd.tianlin.xyz

[S57] C++：编译期常量
来源：http://rsx.zhixingplan.top

constexpr int N = 10;
来源：http://dhc.ybcxt.top

[S58] C++：命名空间
来源：http://zad.quarkkingdee.top

namespace ns { int f() { return 1; } }
来源：http://nxj.ivvv.top

[S59] C++：静态断言
来源：http://eve.xinyue.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rtn.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://bqz.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://goj.jianghu66.top

================================================================================
来源：http://zbf.xziqi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xfn.cheryme.top

================================================================================
来源：http://yyf.jqgfzy.top

[T01] Kotlin：Hello World
来源：http://ozo.ybcxt.top

println("Hello")
来源：http://jpm.nanxuanxn.top

[T02] Kotlin：变量
来源：http://mbl.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vhs.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://ypj.zhixingplan.top

"值: $b"
来源：http://wvs.feifeiyinyue.top

[T04] Kotlin：空安全
来源：http://pop.bbcook.cn

val n: String? = null;  n?.length
来源：http://vgk.jinqigufen.top

[T05] Kotlin：when 表达式
来源：http://bzg.hnqzz.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pty.fehbvm.com

[T06] Kotlin：集合映射
来源：http://whn.vqdsnc.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xqm.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://dsr.ctjpmb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://eqe.sxryk.cn

[T08] Kotlin：数据类
来源：http://wvl.sweek.top

data class User(val name: String, val age: Int)
来源：http://zkf.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://cte.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://fic.jiagoushi.top

[T10] Kotlin：默认参数
来源：http://iez.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ahq.yonumen.top

[T11] Kotlin：协程
来源：http://gwv.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qoj.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://bhv.feifeiyinyue.top

val (a, b) = Pair(1, 2)
来源：http://vpi.ppjwa.cn

[T13] Kotlin：只读 Map
来源：http://qkp.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://vpw.zhongyouzk.top

[T14] Kotlin：循环
来源：http://fwr.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://ntl.snrcjt.cn

[T15] Kotlin：接口
来源：http://rco.xuanzx.com

interface Shape { fun area(): Double }
来源：http://paj.xinyue.icu

[T16] Swift：Hello World
来源：http://mwo.yangfankeji.com

print("Hello")
来源：http://opn.yonumen.top

[T17] Swift：变量与常量
来源：http://ndp.feifeiyinyue.top

var a = 1;  let b = 2
来源：http://izw.xziqi.cn

[T18] Swift：字符串插值
来源：http://umy.chenlongwang.top

"值: \(b)"
来源：http://sax.0kj1m.cn

[T19] Swift：可选绑定
来源：http://sby.dashuyun.cn

if let n = opt { print(n) }
来源：http://bmg.dianchejie.cn

[T20] Swift：数组操作
来源：http://zgv.feifeiyinyue.top

var a = [1, 2, 3];  a.append(4)
来源：http://sqa.zdbjq.cn

[T21] Swift：遍历
来源：http://pcb.ctjpmb.com

for x in a { print(x) }
来源：http://est.c1oappe.top

[T22] Swift：字典
来源：http://iwm.yuanzhike.top

var d = ["a": 1];  d["b"] = 2
来源：http://tsg.jlsjyb.cn

[T23] Swift：函数
来源：http://bpv.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nmo.cdnleiting.top

[T24] Swift：闭包
来源：http://lyt.fengsongda.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tdb.pycfn.com

[T25] Swift：结构体
来源：http://joa.fehbvm.com

struct P { var x: Int }
来源：http://kyc.yuxming.cn

[T26] Swift：类与重写
来源：http://nmu.birdmap.top

class A: Base { override func f() {} }
来源：http://svh.gotoacloud.top

[T27] Swift：错误处理
来源：http://pvw.meibo888.top

do { try f() } catch { print(error) }
来源：http://ixw.316326.xyz

[T28] Swift：枚举
来源：http://qwh.fengsongda.top

enum Color { case red, green }
来源：http://lts.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://mpv.yj20258888.top

guard let x = opt else { return }
来源：http://jep.vqdsnc.cn

[T30] Swift：协议
来源：http://brz.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://tut.ywan-chungtsiang.top

[T31] Lua：Hello World
来源：http://voy.zhoulong.xyz

print("Hello")
来源：http://qlj.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://zpi.gzhubu.top

local a = 1
来源：http://tbv.zhijiandao.cn

[T33] Lua：表（数组）
来源：http://rvy.quarkkingdee.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mlt.hysaishi.cn

[T34] Lua：遍历表
来源：http://lnr.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://owl.jlsjyb.cn

[T35] Lua：字典表
来源：http://gto.jinghuilouyu.cn

local d = { a = 1 };  d.b = 2
来源：http://nvy.vehdjk.com

[T36] Lua：函数
来源：http://xkx.chenzaomai.com

function add(a, b) return a + b end
来源：http://qed.yfazqb.com

[T37] Lua：字符串拼接
来源：http://zca.hcnkem.com

"a" .. "b"
来源：http://wlt.zycfv.cn

[T38] Lua：条件
来源：http://zmp.cqqwz.cn

if x > 0 then print("正") end
来源：http://hri.xuetiantiany.cn

[T39] Lua：模式匹配
来源：http://kso.hywenlv.cn

string.find(s, "%d+")
来源：http://nzy.tarul.cn

[T40] Lua：元表
来源：http://gpz.hcnkem.com

setmetatable({}, { __index = base })
来源：http://fei.shanyushiyangtech.top

[T41] Perl：Hello World
来源：http://fmm.xingfuxueyuan.xyz

print "Hello\n";
来源：http://qjh.fanxiaobao.xyz

[T42] Perl：变量类型
来源：http://evh.jinqigfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://edr.9152youxi.cn

[T43] Perl：字符串插值
来源：http://abg.fengsongda.top

"值: $a"
来源：http://nvm.zhaomingkeji.xyz

[T44] Perl：条件
来源：http://fwb.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://ynh.chenlongwang.top

[T45] Perl：数组遍历
来源：http://xuo.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://cln.guannengcc.top

[T46] Perl：哈希操作
来源：http://tsl.zhaomingkeji.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://url.nwbrower.top

[T47] Perl：正则捕获
来源：http://ugb.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tuz.tian-w.cn

[T48] Perl：正则替换
来源：http://nsv.yangfankeji.com

$s =~ s/old/new/g;
来源：http://rld.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://gxb.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gyj.nanxinkj.top

[T50] Perl：逐行读文件
来源：http://nlh.9152youxi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tno.ydzc1.top

while (my $line = <$fh>) { print $line; }
来源：http://abn.shuidangran.top

[T51] Scala：Hello World
来源：http://pzt.cucudq.cn

println("Hello")
来源：http://nyh.jlsjyb.cn

[T52] Scala：变量
来源：http://mbu.yvedp.cn

val a = 1;  var b = 2
来源：http://exh.gogol.net.cn

[T53] Scala：字符串插值
来源：http://zdu.tianlin.xyz

s"值: $b"
来源：http://nuo.meibo888.top

[T54] Scala：集合映射
来源：http://hea.zhijiandao.cn

List(1, 2, 3).map(_ * 2)
来源：http://rxr.meibo888.top

[T55] Scala：集合过滤
来源：http://fge.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ubv.fanxiaobao.xyz

[T56] Scala：样例类
来源：http://kxx.nwbrower.top

case class User(name: String, age: Int)
来源：http://jrg.gotoacloud.top

[T57] Scala：模式匹配
来源：http://fgo.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rzz.xziqi.cn

[T58] Scala：函数定义
来源：http://xfm.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ozs.ppjwa.cn

[T59] Scala：循环
来源：http://kwq.nwbrower.top

for (i <- 1 to 10) println(i)
来源：http://pmh.yuanzhike.top

[T60] Scala：折叠
来源：http://bny.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gtj.hongshengwenyu.top

================================================================================
来源：http://ikz.tanke756.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qie.hysaishi.cn

================================================================================
来源：http://uoc.xylfe.cn

[U01] Py：创建虚拟环境
来源：http://ahc.gzhubu.top

python -m venv .venv && source .venv/bin/activate
来源：http://zhc.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://hul.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ozh.gotoacloud.top

[U03] Py：加载 .env 配置
来源：http://idm.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yrr.cdnleiting.top

[U04] Py：变量调试打印
来源：http://xnl.bbcook.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eiz.meibo888.top

[U05] Py：列表去重且保序
来源：http://gxl.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://fzx.xuetiantiany.cn

[U06] Py：合并两个字典
来源：http://xmb.9152youxi.cn

{**a, **b}
来源：http://cvt.smart0.xyz

[U07] Py：反转字典键值
来源：http://mmm.shangyingyoupin.top

{v: k for k, v in d.items()}
来源：http://kyf.nanxuanxn.top

[U08] Py：展平二维列表
来源：http://epg.cdnleiting.top

[y for x in nested for y in x]
来源：http://ohp.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://fqt.hesvh.cn

max(d, key=d.get)
来源：http://pxn.bjfxy.top

[U10] Py：按值排序字典
来源：http://dow.ybcxt.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xsg.jinqigufen.top

[U11] Py：生成器表达式
来源：http://yrk.dashuyun.cn

(x * 2 for x in arr)
来源：http://xvv.smart0.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://yye.316326.xyz

Counter(arr).most_common(3)
来源：http://tml.zycfv.cn

[U13] Py：固定长度队列
来源：http://ghp.jlsjyb.cn

deque(maxlen=10)
来源：http://ixw.gogol.net.cn

[U14] Py：分组收集到列表
来源：http://lqo.jinqigfzy.top

defaultdict(list)
来源：http://mzq.wangdashe.top

[U15] Py：高精度计时
来源：http://epm.jqgufenzy.top

t = time.perf_counter()
来源：http://shu.fktsv.cn

[U16] Py：命令行参数解析
来源：http://xji.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uoy.yangfankeji.com

[U17] Py：初始化日志
来源：http://ciy.xziqi.cn

logging.basicConfig(level=logging.INFO)
来源：http://oda.xylfe.cn

[U18] Py：预编译正则
来源：http://wvq.hnqzz.top

pat = re.compile(r"\d+")
来源：http://ggz.ivvv.top

[U19] Py：正则替换带回调
来源：http://bdj.gaohongyu789.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://beh.pycfn.com

[U20] Py：缓存函数结果
来源：http://ojr.xylfe.cn

@functools.lru_cache(maxsize=None)
来源：http://tvi.guowangkeji.top

[U21] Py：自定义上下文管理器
来源：http://fol.xuetiantiany.cn

@contextlib.contextmanager
来源：http://hnf.redwolf501.top

[U22] Py：矩阵转置
来源：http://yxd.zhongyouzk.top

list(zip(*m))
来源：http://orp.quarkkingdee.top

[U23] Py：分块读取大文件
来源：http://uwv.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xyf.daxiang520.top

[U24] Py：路径操作
来源：http://uvi.c1oappe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uso.jqgfzy.top

[U25] Py：CSV 按字典读
来源：http://zax.chenlongwang.top

csv.DictReader(f)
来源：http://eyg.cqqwz.cn

[U26] Py：并发下载
来源：http://kdb.zdbjq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xfp.ywan-chungtsiang.top

[U27] Py：异步 HTTP
来源：http://rzr.sufxvd.cn

aiohttp.ClientSession() 配合 async with
来源：http://pgx.daxiang520.top

[U28] Py：类型别名
来源：http://cus.aizwys.cn

UserId = int
来源：http://jlo.316326.xyz

[U29] Py：属性校验
来源：http://gag.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://sqj.nwbrower.top

[U30] Py：数据类
来源：http://ovr.guowangkeji.top

@dataclass(slots=True)
来源：http://ird.wangdashe.top

[U31] Py：单测
来源：http://jqg.ivvv.top

python -m pytest -q
来源：http://azo.hesvh.cn

[U32] Py：代码格式化
来源：http://szg.fehbvm.com

ruff format . && ruff check --fix .
来源：http://sky.hnqzz.top

[U33] Py：打包发布
来源：http://hwb.shangyingyoupin.top

python -m build  （依赖 pyproject.toml）
来源：http://lyk.jyoumei.cn

[U34] Py：判断编码
来源：http://xck.fanxiaobao.xyz

chardet.detect(raw)
来源：http://iuv.yj20258.top

[U35] Py：发送邮件
来源：http://tgb.daria6918.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jgr.sweek.top

[U36] Py：定时任务
来源：http://pvc.jianghu66.top

schedule.every(10).minutes.do(job)
来源：http://xoa.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://vcq.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://dbv.sweek.top

[U38] Py：获取脚本所在目录
来源：http://gms.wangdashe.top

Path(__file__).resolve().parent
来源：http://xln.redwolf501.top

[U39] Py：判断是否在交互环境
来源：http://jmn.chenjidiqi.icu

sys.stdout.isatty()
来源：http://bzn.snrcjt.cn

[U40] Py：打印到标准错误
来源：http://idn.fehbvm.com

print("err", file=sys.stderr)
来源：http://qsn.snrcjt.cn

[U41] PHP：初始化 Composer 项目
来源：http://fxx.ydjk.org.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jsc.dianchejie.cn

[U42] PHP：PSR-4 自动加载
来源：http://aus.hcnkem.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dht.jyoumei.cn

[U43] PHP：声明命名空间
来源：http://dqr.hnqzz.top

namespace App\Http;
来源：http://gjm.svipenyu.cn

[U44] PHP：开启严格类型
来源：http://azm.jianghu66.top

declare(strict_types=1);
来源：http://qar.shuidangran.top

[U45] PHP：类型声明与返回类型
来源：http://ewp.mhx1999.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hvl.bjfxy.top

[U46] PHP：可空类型
来源：http://fvl.hywenlv.cn

?string $name = null
来源：http://geq.yuxming.cn

[U47] PHP：联合类型
来源：http://dqh.mhx1999.top

int|string $id
来源：http://okd.hysaishi.cn

[U48] PHP：纯枚举
来源：http://qmc.ivvv.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tbp.yangfankeji.com

[U49] PHP：只读属性
来源：http://lws.nanxinkj.top

public readonly string $name
来源：http://nay.shanyushiyangkeji.top

[U50] PHP：构造器属性提升
来源：http://zgr.vqdsnc.cn

public function __construct(private int $id) {}
来源：http://tfr.xinyue.icu

[U51] PHP：数组解构
来源：http://uwp.yj202588.top

[$a, $b] = $arr;
来源：http://obp.ivvv.top

[U52] PHP：箭头函数
来源：http://jwf.xingfuxueyuan.xyz

$double = fn($x) => $x * 2;
来源：http://pxd.hnxiangtu.top

[U53] PHP：空合并运算符
来源：http://bnc.ppjwa.cn

$v = $a ?? $b ?? "default";
来源：http://hbb.fengsongda.top

[U54] PHP：空安全调用
来源：http://kwj.ywan-chungtsiang.top

$obj?->method()
来源：http://zpx.shzxlz.cn

[U55] PHP：match 表达式
来源：http://jcq.ehwqpu.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qpa.jinqigufen.top

[U56] PHP：命名参数
来源：http://vzn.jqgfzy.top

f(a: 1, b: 2)
来源：http://mxy.haohaochexian.top

[U57] PHP：字符串插值
来源：http://vpo.yuanzhike.top

"值: {$a}"
来源：http://sln.daria6918.cn

[U58] PHP：数组三件套
来源：http://ykq.bbcook.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lwu.meibo888.top

[U59] PHP：自定义排序
来源：http://xpi.quarkkingdee.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xmy.hesvh.cn

[U60] PHP：JSON 编解码
来源：http://bjq.snrcjt.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zuy.sjlbkw.cn

[U61] PHP：正则
来源：http://pwy.xuanzx.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rzg.vehdjk.com

[U62] PHP：日期对象
来源：http://lfo.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xtj.fanxiaobao.xyz

[U63] PHP：文件读写
来源：http://ypi.gogol.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dpd.yueranfly.top

[U64] PHP：目录遍历
来源：http://qqs.yj202588.top

glob("dir/*.php");  scandir("dir");
来源：http://fme.guannengcc.top

[U65] PHP：会话
来源：http://yly.vehdjk.com

session_start();  $_SESSION["uid"] = 1;
来源：http://fsq.tarul.cn

[U66] PHP：设置 Cookie
来源：http://vra.xylfe.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qns.yuxming.cn

[U67] PHP：处理文件上传
来源：http://atf.fengsongda.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pcc.iojbl.cn

[U68] PHP：PDO 连接
来源：http://xzx.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zvt.fzhhl.top

[U69] PHP：PDO 预处理
来源：http://byz.sufxvd.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qkb.hnqzz.top

[U70] PHP：PDO 事务
来源：http://jpa.guowangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tfl.jlsjyb.cn

[U71] PHP：抛出异常
来源：http://vvo.wangdashe.top

throw new RuntimeException("失败", 500);
来源：http://tsv.hywenlv.cn

[U72] PHP：写错误日志
来源：http://osu.guannengcc.top

error_log("失败: " . $e->getMessage());
来源：http://dhd.xingfuxueyuan.xyz

[U73] PHP：读取 ini 配置
来源：http://vpy.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://yma.cheryme.top

[U74] PHP：读取环境变量
来源：http://ydv.jqgufenzy.top

getenv("APP_ENV") ?: "production"
来源：http://yoy.aizwys.cn


<!-- 参考信息 -->