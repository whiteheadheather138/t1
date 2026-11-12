代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cld.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://utk.aibaodan.cn

static_cast<double>(a) / b
来源：http://ztt.vqdsnc.cn

[S52] C++：const 与 noexcept
来源：http://phj.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://hpq.shuidangran.top

[S53] C++：移动语义
来源：http://sjr.zhijiandao.cn

std::vector<int> w = std::move(v);
来源：http://yke.nanxuanxn.top

[S54] C++：异常处理
来源：http://bxd.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xaw.guowangkeji.top

[S55] C++：结构化绑定
来源：http://jhz.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rqo.gzhubu.top

[S56] C++：optional
来源：http://lul.gotoacloud.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eea.birdmap.top

[S57] C++：编译期常量
来源：http://aux.bbcook.cn

constexpr int N = 10;
来源：http://okw.zhiwuduotai.top

[S58] C++：命名空间
来源：http://kmy.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://kcx.pycfn.com

[S59] C++：静态断言
来源：http://chj.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pzl.yonumen.top

[S60] C++：遍历并删除元素
来源：http://vtb.cheryme.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dsb.52xcode.cn

================================================================================
来源：http://xam.kuanghao11.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qjv.xuanzx.com

================================================================================
来源：http://bdq.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://syb.yanxiufei.cn

println("Hello")
来源：http://flj.gogol.net.cn

[T02] Kotlin：变量
来源：http://fcd.mhx1999.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jpx.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://bsv.sweek.top

"值: $b"
来源：http://cvg.jyoumei.cn

[T04] Kotlin：空安全
来源：http://aag.zhongyouzk.top

val n: String? = null;  n?.length
来源：http://cuv.hammf.cn

[T05] Kotlin：when 表达式
来源：http://huc.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tkp.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://fdm.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ned.52xcode.cn

[T07] Kotlin：集合过滤
来源：http://kip.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uff.daria6918.cn

[T08] Kotlin：数据类
来源：http://lkc.cqqwz.cn

data class User(val name: String, val age: Int)
来源：http://jwq.zhoulong.xyz

[T09] Kotlin：扩展函数
来源：http://cnz.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://mqu.birdmap.top

[T10] Kotlin：默认参数
来源：http://ezf.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://awv.tarul.cn

[T11] Kotlin：协程
来源：http://lan.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ion.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://nhc.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://xpw.cqqwz.cn

[T13] Kotlin：只读 Map
来源：http://rnh.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://mqc.ydzc1.top

[T14] Kotlin：循环
来源：http://hsj.yuanzhike.top

for (i in 1..10) println(i)
来源：http://zcx.meibo888.top

[T15] Kotlin：接口
来源：http://dps.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://hpg.guannengcc.top

[T16] Swift：Hello World
来源：http://rmo.fzhhl.top

print("Hello")
来源：http://lfj.yangfankeji.com

[T17] Swift：变量与常量
来源：http://lks.fzhhl.top

var a = 1;  let b = 2
来源：http://tvr.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://lra.sjlbkw.cn

"值: \(b)"
来源：http://mlu.nwbrower.top

[T19] Swift：可选绑定
来源：http://mmf.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://dwf.gogol.net.cn

[T20] Swift：数组操作
来源：http://ikt.cucudq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qiy.zycfv.cn

[T21] Swift：遍历
来源：http://krt.aibaodan.cn

for x in a { print(x) }
来源：http://bfx.yj20258888.top

[T22] Swift：字典
来源：http://drx.feifeiyinyue.top

var d = ["a": 1];  d["b"] = 2
来源：http://kkg.havefunace.top

[T23] Swift：函数
来源：http://xjw.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ool.ywan-chungtsiang.top

[T24] Swift：闭包
来源：http://zle.guowangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zuk.nanxinkj.top

[T25] Swift：结构体
来源：http://vhd.hesvh.cn

struct P { var x: Int }
来源：http://vhy.shanyushiyangtech.top

[T26] Swift：类与重写
来源：http://rvo.epnwcf.com

class A: Base { override func f() {} }
来源：http://ptl.zhongyouzk.top

[T27] Swift：错误处理
来源：http://yjp.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://aqb.zhijiandao.cn

[T28] Swift：枚举
来源：http://hrt.daxiang520.top

enum Color { case red, green }
来源：http://gkm.kuanghao11.cn

[T29] Swift：guard 提前返回
来源：http://zdw.yvedp.cn

guard let x = opt else { return }
来源：http://sah.yj20258888.top

[T30] Swift：协议
来源：http://egh.tarul.cn

protocol Shape { func area() -> Double }
来源：http://ftb.zhiwuduotai.top

[T31] Lua：Hello World
来源：http://weu.zhijiandao.cn

print("Hello")
来源：http://hpz.snrcjt.cn

[T32] Lua：局部变量
来源：http://siq.jianghu66.top

local a = 1
来源：http://own.redwolf501.top

[T33] Lua：表（数组）
来源：http://qcg.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://gwp.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://scn.pengpengdd.cyou

for i, v in ipairs(t) do print(i, v) end
来源：http://uug.aizwys.cn

[T35] Lua：字典表
来源：http://oaw.gogol.net.cn

local d = { a = 1 };  d.b = 2
来源：http://lhy.sufxvd.cn

[T36] Lua：函数
来源：http://nod.zdbjq.cn

function add(a, b) return a + b end
来源：http://yls.ydjk.org.cn

[T37] Lua：字符串拼接
来源：http://ynm.quarkkingdee.top

"a" .. "b"
来源：http://mlc.zhijiandao.cn

[T38] Lua：条件
来源：http://yum.c1oappe.top

if x > 0 then print("正") end
来源：http://hjf.cheryme.top

[T39] Lua：模式匹配
来源：http://dcu.snrcjt.cn

string.find(s, "%d+")
来源：http://urm.birdmap.top

[T40] Lua：元表
来源：http://pxc.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://nqd.sjlbkw.cn

[T41] Perl：Hello World
来源：http://ezq.jinqigfzy.top

print "Hello\n";
来源：http://rnt.yangfankeji.com

[T42] Perl：变量类型
来源：http://hkk.havefunace.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wmu.yvedp.cn

[T43] Perl：字符串插值
来源：http://ivz.feifeiyinyue.top

"值: $a"
来源：http://vrh.meibo888.top

[T44] Perl：条件
来源：http://wja.yuanzhike.top

if ($a > 0) { print "正"; }
来源：http://stt.epnwcf.com

[T45] Perl：数组遍历
来源：http://ulw.c1oappe.top

for my $x (@arr) { print $x; }
来源：http://lry.sjlbkw.cn

[T46] Perl：哈希操作
来源：http://weo.vqdsnc.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fnx.birdmap.top

[T47] Perl：正则捕获
来源：http://ghl.meibo888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ijs.ctjpmb.com

[T48] Perl：正则替换
来源：http://yum.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://yqr.ppjwa.cn

[T49] Perl：函数
来源：http://ffs.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ulb.zhengqikj.top

[T50] Perl：逐行读文件
来源：http://isl.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://beb.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://rar.ydzc1.top

[T51] Scala：Hello World
来源：http://gkc.cdnleiting.top

println("Hello")
来源：http://bah.fanxiaobao.xyz

[T52] Scala：变量
来源：http://zwo.gotoacloud.top

val a = 1;  var b = 2
来源：http://nyw.cheryme.top

[T53] Scala：字符串插值
来源：http://erq.zhijiandao.cn

s"值: $b"
来源：http://oom.xylfe.cn

[T54] Scala：集合映射
来源：http://vgp.sxryk.cn

List(1, 2, 3).map(_ * 2)
来源：http://tcj.nwbrower.top

[T55] Scala：集合过滤
来源：http://ght.jqgfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://cek.zhiwuduotai.top

[T56] Scala：样例类
来源：http://hyv.xuanzx.com

case class User(name: String, age: Int)
来源：http://qwn.daxiang520.top

[T57] Scala：模式匹配
来源：http://mkj.yj20258888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://cpz.zhaomingkeji.xyz

[T58] Scala：函数定义
来源：http://dis.tian-w.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pdm.hfpthk.cn

[T59] Scala：循环
来源：http://mxz.daxiang520.top

for (i <- 1 to 10) println(i)
来源：http://joa.yongpay.top

[T60] Scala：折叠
来源：http://npf.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vmg.yfazqb.com

================================================================================
来源：http://dbm.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gxb.pengpengdd.cyou

================================================================================
来源：http://vtd.ybcxt.top

[U01] Py：创建虚拟环境
来源：http://ltd.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://mzu.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://flc.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qhq.xingfuxueyuan.xyz

[U03] Py：加载 .env 配置
来源：http://yov.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sst.hammf.cn

[U04] Py：变量调试打印
来源：http://tie.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ggv.havefunace.top

[U05] Py：列表去重且保序
来源：http://gbj.tarul.cn

list(dict.fromkeys(arr))
来源：http://hbt.fzhhl.top

[U06] Py：合并两个字典
来源：http://ejk.sjlbkw.cn

{**a, **b}
来源：http://dnv.kuanghao11.cn

[U07] Py：反转字典键值
来源：http://vqc.zhixingplan.top

{v: k for k, v in d.items()}
来源：http://vqm.hcnkem.com

[U08] Py：展平二维列表
来源：http://qqt.zdbjq.cn

[y for x in nested for y in x]
来源：http://exp.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://kbu.tanke756.top

max(d, key=d.get)
来源：http://fxu.zdbjq.cn

[U10] Py：按值排序字典
来源：http://vxq.yangfankeji.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://enh.zdbjq.cn

[U11] Py：生成器表达式
来源：http://vdd.jianghu66.top

(x * 2 for x in arr)
来源：http://lll.ydjk.org.cn

[U12] Py：取出现最多的 3 个元素
来源：http://toh.yfazqb.com

Counter(arr).most_common(3)
来源：http://eqk.zycfv.cn

[U13] Py：固定长度队列
来源：http://jsd.hammf.cn

deque(maxlen=10)
来源：http://vnj.haohaochexian.top

[U14] Py：分组收集到列表
来源：http://mvv.hysaishi.cn

defaultdict(list)
来源：http://qyt.ppjwa.cn

[U15] Py：高精度计时
来源：http://vmx.xuetiantiany.cn

t = time.perf_counter()
来源：http://cuc.hnqzz.top

[U16] Py：命令行参数解析
来源：http://uyy.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dsh.zycfv.cn

[U17] Py：初始化日志
来源：http://lul.sweek.top

logging.basicConfig(level=logging.INFO)
来源：http://zdn.daria6918.cn

[U18] Py：预编译正则
来源：http://ucu.yuanzhike.top

pat = re.compile(r"\d+")
来源：http://esm.jiagoushi.top

[U19] Py：正则替换带回调
来源：http://apu.smart0.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sma.havefunace.top

[U20] Py：缓存函数结果
来源：http://xys.haohaochexian.top

@functools.lru_cache(maxsize=None)
来源：http://qwy.jiagoushi.top

[U21] Py：自定义上下文管理器
来源：http://sux.sweek.top

@contextlib.contextmanager
来源：http://hcx.guowangkeji.top

[U22] Py：矩阵转置
来源：http://vbg.zhiwuduotai.top

list(zip(*m))
来源：http://olj.sufxvd.cn

[U23] Py：分块读取大文件
来源：http://zrt.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://icg.cqqwz.cn

[U24] Py：路径操作
来源：http://cgu.0kj1m.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rds.ydjk.org.cn

[U25] Py：CSV 按字典读
来源：http://anx.jqgufenzy.top

csv.DictReader(f)
来源：http://yxm.sjlbkw.cn

[U26] Py：并发下载
来源：http://kmv.xylfe.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wqu.yanxiufei.cn

[U27] Py：异步 HTTP
来源：http://cbb.svipenyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://kpx.jiagoushi.top

[U28] Py：类型别名
来源：http://pfr.jqgufenzy.top

UserId = int
来源：http://tlr.yj20258.top

[U29] Py：属性校验
来源：http://rrd.gzhubu.top

@property 与 @x.setter 配合
来源：http://hor.daria6918.cn

[U30] Py：数据类
来源：http://wrr.cdnleiting.top

@dataclass(slots=True)
来源：http://aiy.sufxvd.cn

[U31] Py：单测
来源：http://kep.shanyushiyangkeji.top

python -m pytest -q
来源：http://vmv.chenzaomai.com

[U32] Py：代码格式化
来源：http://jgf.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://oex.nwbrower.top

[U33] Py：打包发布
来源：http://eud.gaohongyu789.top

python -m build  （依赖 pyproject.toml）
来源：http://epr.yj202588.top

[U34] Py：判断编码
来源：http://krc.vehdjk.com

chardet.detect(raw)
来源：http://jby.nanxuanxn.top

[U35] Py：发送邮件
来源：http://idh.aizwys.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vol.yanxiufei.cn

[U36] Py：定时任务
来源：http://oeu.hysaishi.cn

schedule.every(10).minutes.do(job)
来源：http://jwk.quarkkingdee.top

[U37] Py：读写 Excel
来源：http://aiy.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://abi.ppjwa.cn

[U38] Py：获取脚本所在目录
来源：http://vbg.ppjwa.cn

Path(__file__).resolve().parent
来源：http://grt.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://xub.jqgufenzy.top

sys.stdout.isatty()
来源：http://qei.shuidangran.top

[U40] Py：打印到标准错误
来源：http://zav.cashguo.top

print("err", file=sys.stderr)
来源：http://imf.xinyue.icu

[U41] PHP：初始化 Composer 项目
来源：http://rpc.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gnj.kuanghao11.cn

[U42] PHP：PSR-4 自动加载
来源：http://din.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dqh.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://uhi.ydzc1.top

namespace App\Http;
来源：http://flu.tanke756.top

[U44] PHP：开启严格类型
来源：http://vdc.ydjk.org.cn

declare(strict_types=1);
来源：http://rju.shanyushiyangtech.top

[U45] PHP：类型声明与返回类型
来源：http://mdd.vqdsnc.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cqr.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://qtu.sufxvd.cn

?string $name = null
来源：http://vim.9152youxi.cn

[U47] PHP：联合类型
来源：http://izv.gogol.net.cn

int|string $id
来源：http://wvb.fzhhl.top

[U48] PHP：纯枚举
来源：http://xiy.gaohongyu789.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nhj.sjlbkw.cn

[U49] PHP：只读属性
来源：http://wrb.smart0.xyz

public readonly string $name
来源：http://dez.hongshengwenyu.top

[U50] PHP：构造器属性提升
来源：http://gpo.gotoacloud.top

public function __construct(private int $id) {}
来源：http://nvv.gaohongyu789.top

[U51] PHP：数组解构
来源：http://nqd.jyoumei.cn

[$a, $b] = $arr;
来源：http://vfc.tarul.cn

[U52] PHP：箭头函数
来源：http://sjm.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://vmc.yfazqb.com

[U53] PHP：空合并运算符
来源：http://pvi.gaohongyu789.top

$v = $a ?? $b ?? "default";
来源：http://uii.fengsongda.top

[U54] PHP：空安全调用
来源：http://nxg.feifeiyinyue.top

$obj?->method()
来源：http://hzq.dianchejie.cn

[U55] PHP：match 表达式
来源：http://hbf.ctjpmb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nmh.aibaodan.cn

[U56] PHP：命名参数
来源：http://eno.ppjwa.cn

f(a: 1, b: 2)
来源：http://fkk.andypj.xyz

[U57] PHP：字符串插值
来源：http://ovf.sxryk.cn

"值: {$a}"
来源：http://sau.sweek.top

[U58] PHP：数组三件套
来源：http://mtq.hnqzz.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eup.fktsv.cn

[U59] PHP：自定义排序
来源：http://yid.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gyo.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://hnz.tanke756.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ron.ybcxt.top

[U61] PHP：正则
来源：http://wbz.yuxming.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nsz.cashguo.top

[U62] PHP：日期对象
来源：http://xqb.iojbl.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mmz.guowangkeji.top

[U63] PHP：文件读写
来源：http://iyb.bjfxy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wil.jianghu66.top

[U64] PHP：目录遍历
来源：http://njq.iojbl.cn

glob("dir/*.php");  scandir("dir");
来源：http://xqu.zhixingplan.top

[U65] PHP：会话
来源：http://bls.gaohongyu789.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fhm.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://cxj.xziqi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://twn.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://fmw.haohaochexian.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://urf.andypj.xyz

[U68] PHP：PDO 连接
来源：http://bhp.tarul.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tyg.hywenlv.cn

[U69] PHP：PDO 预处理
来源：http://mfm.jinyuanbaomall.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gho.fehbvm.com

[U70] PHP：PDO 事务
来源：http://xni.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pam.iojbl.cn

[U71] PHP：抛出异常
来源：http://mbl.fzhhl.top

throw new RuntimeException("失败", 500);
来源：http://irk.hammf.cn

[U72] PHP：写错误日志
来源：http://cdg.gotoacloud.top

error_log("失败: " . $e->getMessage());
来源：http://uqc.fengsongda.top

[U73] PHP：读取 ini 配置
来源：http://eff.zhaomingkeji.xyz

parse_ini_file("config.ini", true)
来源：http://nfz.daria6918.cn

[U74] PHP：读取环境变量
来源：http://cmp.yueranfly.top

getenv("APP_ENV") ?: "production"
来源：http://opq.zdbjq.cn

[U75] PHP：依赖注入
来源：http://kvf.xuanzx.com

composer require psr/container
来源：http://yxv.zhiwuduotai.top

[U76] PHP：简单路由
来源：http://pwh.chenjidiqi.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bmi.jiagoushi.top


<!-- 参考信息 -->