代发 wailian999

int size() const noexcept { return n_; }
来源：http://pfm.sjlbkw.cn

[S53] C++：移动语义
来源：http://hfa.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://tlc.tanke756.top

[S54] C++：异常处理
来源：http://aim.chenzaomai.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://how.316326.xyz

[S55] C++：结构化绑定
来源：http://ppz.aibaodan.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jgs.aizwys.cn

[S56] C++：optional
来源：http://bsk.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ffd.ehwqpu.com

[S57] C++：编译期常量
来源：http://gvy.c1oappe.top

constexpr int N = 10;
来源：http://qwh.guowangkeji.top

[S58] C++：命名空间
来源：http://kuy.gzhubu.top

namespace ns { int f() { return 1; } }
来源：http://pzw.chenzaomai.com

[S59] C++：静态断言
来源：http://cqb.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ahi.ydzc1.top

[S60] C++：遍历并删除元素
来源：http://qio.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rdp.jinqigfzy.top

================================================================================
来源：http://tri.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ixo.hnqzz.top

================================================================================
来源：http://skl.vehdjk.com

[T01] Kotlin：Hello World
来源：http://vvl.sjlbkw.cn

println("Hello")
来源：http://hny.hysaishi.cn

[T02] Kotlin：变量
来源：http://dke.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fmh.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://pya.cashguo.top

"值: $b"
来源：http://lgc.sysykeji.top

[T04] Kotlin：空安全
来源：http://upv.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://pou.zycfv.cn

[T05] Kotlin：when 表达式
来源：http://xkq.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fcp.tanke756.top

[T06] Kotlin：集合映射
来源：http://ocu.yanxiufei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ory.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://dal.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://koc.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://uib.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://sqx.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://kvo.yj20258.top

fun String.exclaim() = this + "!"
来源：http://zjg.nanxuanxn.top

[T10] Kotlin：默认参数
来源：http://iyp.xingfuxueyuan.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://pva.dianchejie.cn

[T11] Kotlin：协程
来源：http://bnp.fengsongda.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nsc.tarul.cn

[T12] Kotlin：解构声明
来源：http://cyu.pengpengdd.cyou

val (a, b) = Pair(1, 2)
来源：http://iwn.yj20258.top

[T13] Kotlin：只读 Map
来源：http://ueb.gaohongyu789.top

val m = mapOf("a" to 1)
来源：http://bef.guannengcc.top

[T14] Kotlin：循环
来源：http://iwm.ctjpmb.com

for (i in 1..10) println(i)
来源：http://ruc.jinqigufen.top

[T15] Kotlin：接口
来源：http://vyp.havefunace.top

interface Shape { fun area(): Double }
来源：http://uut.guannengcc.top

[T16] Swift：Hello World
来源：http://tei.chenzaomai.com

print("Hello")
来源：http://kaj.aibaodan.cn

[T17] Swift：变量与常量
来源：http://ozx.cdnleiting.top

var a = 1;  let b = 2
来源：http://oge.shangyingyoupin.top

[T18] Swift：字符串插值
来源：http://dda.sufxvd.cn

"值: \(b)"
来源：http://rmi.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://iwc.hysaishi.cn

if let n = opt { print(n) }
来源：http://bvo.ydjk.org.cn

[T20] Swift：数组操作
来源：http://oxo.hywenlv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rut.nanxuanxn.top

[T21] Swift：遍历
来源：http://kki.jianghu66.top

for x in a { print(x) }
来源：http://xvs.smart0.xyz

[T22] Swift：字典
来源：http://rhj.pycfn.com

var d = ["a": 1];  d["b"] = 2
来源：http://mbb.hfpthk.cn

[T23] Swift：函数
来源：http://qky.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zto.hongshengwenyu.top

[T24] Swift：闭包
来源：http://ihu.fktsv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yjo.cqqwz.cn

[T25] Swift：结构体
来源：http://jzh.zhongyouzk.top

struct P { var x: Int }
来源：http://xeu.cqqwz.cn

[T26] Swift：类与重写
来源：http://ijh.redwolf501.top

class A: Base { override func f() {} }
来源：http://trm.pycfn.com

[T27] Swift：错误处理
来源：http://gqh.jiagoushi.top

do { try f() } catch { print(error) }
来源：http://bct.jyoumei.cn

[T28] Swift：枚举
来源：http://bou.ydjk.org.cn

enum Color { case red, green }
来源：http://nwz.cqqwz.cn

[T29] Swift：guard 提前返回
来源：http://klq.dashuyun.cn

guard let x = opt else { return }
来源：http://qqc.sjlbkw.cn

[T30] Swift：协议
来源：http://vlr.chenzaomai.com

protocol Shape { func area() -> Double }
来源：http://rtb.dianchejie.cn

[T31] Lua：Hello World
来源：http://ene.52xcode.cn

print("Hello")
来源：http://gfk.epnwcf.com

[T32] Lua：局部变量
来源：http://hiz.svipenyu.cn

local a = 1
来源：http://xdd.havefunace.top

[T33] Lua：表（数组）
来源：http://tru.zhixingplan.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pck.guannengcc.top

[T34] Lua：遍历表
来源：http://zga.shangyingyoupin.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xqx.shanyushiyangkeji.top

[T35] Lua：字典表
来源：http://gji.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://tyx.hysaishi.cn

[T36] Lua：函数
来源：http://cqh.jqgufenzy.top

function add(a, b) return a + b end
来源：http://wqk.hcnkem.com

[T37] Lua：字符串拼接
来源：http://odz.yanxiufei.cn

"a" .. "b"
来源：http://qrz.tianlin.xyz

[T38] Lua：条件
来源：http://kku.hammf.cn

if x > 0 then print("正") end
来源：http://mig.zycfv.cn

[T39] Lua：模式匹配
来源：http://dvb.zhoulong.xyz

string.find(s, "%d+")
来源：http://mzb.hcnkem.com

[T40] Lua：元表
来源：http://xcf.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://uum.hcnkem.com

[T41] Perl：Hello World
来源：http://lfr.fzhhl.top

print "Hello\n";
来源：http://ttz.hnqzz.top

[T42] Perl：变量类型
来源：http://gbz.hongshengwenyu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pko.bjfxy.top

[T43] Perl：字符串插值
来源：http://vhk.daria6918.cn

"值: $a"
来源：http://aeu.zhijiandao.cn

[T44] Perl：条件
来源：http://pzh.sjlbkw.cn

if ($a > 0) { print "正"; }
来源：http://scj.gzhubu.top

[T45] Perl：数组遍历
来源：http://sju.dianchejie.cn

for my $x (@arr) { print $x; }
来源：http://cub.chenzaomai.com

[T46] Perl：哈希操作
来源：http://jnk.hongshengwenyu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gdc.zhijiandao.cn

[T47] Perl：正则捕获
来源：http://ofr.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://mma.jyoumei.cn

[T48] Perl：正则替换
来源：http://bdk.sysykeji.top

$s =~ s/old/new/g;
来源：http://znn.yuxming.cn

[T49] Perl：函数
来源：http://eqb.nanxuanxn.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lnb.yangfankeji.com

[T50] Perl：逐行读文件
来源：http://gxc.svipenyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kbm.52xcode.cn

while (my $line = <$fh>) { print $line; }
来源：http://zrb.daxiang520.top

[T51] Scala：Hello World
来源：http://bvi.shzxlz.cn

println("Hello")
来源：http://yef.birdmap.top

[T52] Scala：变量
来源：http://uhc.svipenyu.cn

val a = 1;  var b = 2
来源：http://qzi.52xcode.cn

[T53] Scala：字符串插值
来源：http://wew.yuanzhike.top

s"值: $b"
来源：http://xih.9152youxi.cn

[T54] Scala：集合映射
来源：http://hag.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://ziq.zdqjudy.top

[T55] Scala：集合过滤
来源：http://bnx.9152youxi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sru.jinqigfzy.top

[T56] Scala：样例类
来源：http://cpn.zdbjq.cn

case class User(name: String, age: Int)
来源：http://imp.hywenlv.cn

[T57] Scala：模式匹配
来源：http://otu.zhijiandao.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://llq.jinqigufen.top

[T58] Scala：函数定义
来源：http://vyv.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ssf.yanxiufei.cn

[T59] Scala：循环
来源：http://zlt.gotoacloud.top

for (i <- 1 to 10) println(i)
来源：http://oim.sjlbkw.cn

[T60] Scala：折叠
来源：http://ptd.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zxq.hfpthk.cn

================================================================================
来源：http://uam.yuxming.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nsu.pycfn.com

================================================================================
来源：http://jxl.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://bhs.tian-w.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cwd.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://dqj.sysykeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xcj.zdbjq.cn

[U03] Py：加载 .env 配置
来源：http://kpg.zhaomingkeji.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://nig.zhixingplan.top

[U04] Py：变量调试打印
来源：http://ufq.cheryme.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://guh.quarkkingdee.top

[U05] Py：列表去重且保序
来源：http://bvh.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://hfx.jinghuilouyu.cn

[U06] Py：合并两个字典
来源：http://nei.zhaomingkeji.xyz

{**a, **b}
来源：http://okd.zhijiandao.cn

[U07] Py：反转字典键值
来源：http://qpt.fktsv.cn

{v: k for k, v in d.items()}
来源：http://nwv.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://otn.haohaochexian.top

[y for x in nested for y in x]
来源：http://dhv.ppjwa.cn

[U09] Py：字典取最大值的键
来源：http://hre.mhx1999.top

max(d, key=d.get)
来源：http://aza.tarul.cn

[U10] Py：按值排序字典
来源：http://uan.bjfxy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nzc.daria6918.cn

[U11] Py：生成器表达式
来源：http://dba.zycfv.cn

(x * 2 for x in arr)
来源：http://qlm.sufxvd.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xio.fzhhl.top

Counter(arr).most_common(3)
来源：http://kdz.wangshuangyany.cn

[U13] Py：固定长度队列
来源：http://bwr.yj20258888.top

deque(maxlen=10)
来源：http://ufn.hammf.cn

[U14] Py：分组收集到列表
来源：http://znc.tarul.cn

defaultdict(list)
来源：http://tkr.yanxiufei.cn

[U15] Py：高精度计时
来源：http://dys.yj20258.top

t = time.perf_counter()
来源：http://cyk.ybcxt.top

[U16] Py：命令行参数解析
来源：http://gfx.hfpthk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tqm.quarkkingdee.top

[U17] Py：初始化日志
来源：http://gvh.yvedp.cn

logging.basicConfig(level=logging.INFO)
来源：http://izp.hnxiangtu.top

[U18] Py：预编译正则
来源：http://djy.yonumen.top

pat = re.compile(r"\d+")
来源：http://owz.cashguo.top

[U19] Py：正则替换带回调
来源：http://gcc.52xcode.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eht.hnqzz.top

[U20] Py：缓存函数结果
来源：http://fgj.sufxvd.cn

@functools.lru_cache(maxsize=None)
来源：http://ivc.zhoulong.xyz

[U21] Py：自定义上下文管理器
来源：http://hnh.mhx1999.top

@contextlib.contextmanager
来源：http://pwo.smart0.xyz

[U22] Py：矩阵转置
来源：http://sdw.jinqigfzy.top

list(zip(*m))
来源：http://fmw.sysykeji.top

[U23] Py：分块读取大文件
来源：http://uyf.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wce.zhengqikj.top

[U24] Py：路径操作
来源：http://nwq.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nka.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://ggk.quarkkingdee.top

csv.DictReader(f)
来源：http://mkd.wangdashe.top

[U26] Py：并发下载
来源：http://tgw.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zzk.shanyushiyangkeji.top

[U27] Py：异步 HTTP
来源：http://nkw.xziqi.cn

aiohttp.ClientSession() 配合 async with
来源：http://qmr.ppjwa.cn

[U28] Py：类型别名
来源：http://msu.svipenyu.cn

UserId = int
来源：http://vot.fanxiaobao.xyz

[U29] Py：属性校验
来源：http://jvn.ywan-chungtsiang.top

@property 与 @x.setter 配合
来源：http://xff.yuanzhike.top

[U30] Py：数据类
来源：http://ums.ydjk.org.cn

@dataclass(slots=True)
来源：http://miq.hammf.cn

[U31] Py：单测
来源：http://ayi.chenzaomai.com

python -m pytest -q
来源：http://rip.shzxlz.cn

[U32] Py：代码格式化
来源：http://kea.zdbjq.cn

ruff format . && ruff check --fix .
来源：http://ehz.daria6918.cn

[U33] Py：打包发布
来源：http://hki.ppjwa.cn

python -m build  （依赖 pyproject.toml）
来源：http://pin.ybcxt.top

[U34] Py：判断编码
来源：http://brc.kuanghao11.cn

chardet.detect(raw)
来源：http://jjp.xinyue.icu

[U35] Py：发送邮件
来源：http://ggj.zdqjudy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ner.kuanghao11.cn

[U36] Py：定时任务
来源：http://nyx.gzhubu.top

schedule.every(10).minutes.do(job)
来源：http://auz.chenzaomai.com

[U37] Py：读写 Excel
来源：http://dsr.zhengqikj.top

pandas.read_excel / DataFrame.to_excel
来源：http://iyp.hcnkem.com

[U38] Py：获取脚本所在目录
来源：http://hht.yueranfly.top

Path(__file__).resolve().parent
来源：http://vmz.xylfe.cn

[U39] Py：判断是否在交互环境
来源：http://zrk.gaohongyu789.top

sys.stdout.isatty()
来源：http://xsa.0kj1m.cn

[U40] Py：打印到标准错误
来源：http://prq.mhx1999.top

print("err", file=sys.stderr)
来源：http://vno.bjfxy.top

[U41] PHP：初始化 Composer 项目
来源：http://dbd.yj20258888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vay.yanxiufei.cn

[U42] PHP：PSR-4 自动加载
来源：http://ieg.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ash.daria6918.cn

[U43] PHP：声明命名空间
来源：http://cjl.yueranfly.top

namespace App\Http;
来源：http://hqm.xylfe.cn

[U44] PHP：开启严格类型
来源：http://kfe.hnqzz.top

declare(strict_types=1);
来源：http://npx.zhaomingkeji.xyz

[U45] PHP：类型声明与返回类型
来源：http://wvg.yfazqb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://zpa.havefunace.top

[U46] PHP：可空类型
来源：http://ebb.hysaishi.cn

?string $name = null
来源：http://mfn.sjlbkw.cn

[U47] PHP：联合类型
来源：http://gyd.zdbjq.cn

int|string $id
来源：http://skv.hongshengwenyu.top

[U48] PHP：纯枚举
来源：http://cja.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vyd.yangfankeji.com

[U49] PHP：只读属性
来源：http://aof.vehdjk.com

public readonly string $name
来源：http://dhs.ybcxt.top

[U50] PHP：构造器属性提升
来源：http://neh.hesvh.cn

public function __construct(private int $id) {}
来源：http://inb.ydzc1.top

[U51] PHP：数组解构
来源：http://mqu.9152youxi.cn

[$a, $b] = $arr;
来源：http://vmv.yangfankeji.com

[U52] PHP：箭头函数
来源：http://twj.guowangkeji.top

$double = fn($x) => $x * 2;
来源：http://uua.fktsv.cn

[U53] PHP：空合并运算符
来源：http://lza.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://xnp.jlsjyb.cn

[U54] PHP：空安全调用
来源：http://oqy.uphjek.com

$obj?->method()
来源：http://rrm.epnwcf.com

[U55] PHP：match 表达式
来源：http://jby.cashguo.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pww.sysykeji.top

[U56] PHP：命名参数
来源：http://ysi.snrcjt.cn

f(a: 1, b: 2)
来源：http://hmv.zdbjq.cn

[U57] PHP：字符串插值
来源：http://xap.xuetiantiany.cn

"值: {$a}"
来源：http://osl.ivvv.top

[U58] PHP：数组三件套
来源：http://hop.sysykeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ipg.sxryk.cn

[U59] PHP：自定义排序
来源：http://vlr.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qbg.jinqigfzy.top

[U60] PHP：JSON 编解码
来源：http://zvn.pengpengdd.cyou

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lbu.ivvv.top

[U61] PHP：正则
来源：http://gun.chenzaomai.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qlw.xuanzx.com

[U62] PHP：日期对象
来源：http://ohx.ybcxt.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://chn.yvedp.cn

[U63] PHP：文件读写
来源：http://hjp.nanxuanxn.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uha.hfpthk.cn

[U64] PHP：目录遍历
来源：http://rgq.zycfv.cn

glob("dir/*.php");  scandir("dir");
来源：http://mxo.52xcode.cn

[U65] PHP：会话
来源：http://cxa.guannengcc.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zzq.sysykeji.top

[U66] PHP：设置 Cookie
来源：http://qmi.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tmh.meibo888.top

[U67] PHP：处理文件上传
来源：http://ibt.jinqigfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bxi.yuanzhike.top

[U68] PHP：PDO 连接
来源：http://wfa.zdbjq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://per.hnxiangtu.top

[U69] PHP：PDO 预处理
来源：http://cjz.aizwys.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tij.daxiang520.top

[U70] PHP：PDO 事务
来源：http://edi.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ftl.dianchejie.cn

[U71] PHP：抛出异常
来源：http://ngo.9152youxi.cn

throw new RuntimeException("失败", 500);
来源：http://hyw.tarul.cn

[U72] PHP：写错误日志
来源：http://juc.fengsongda.top

error_log("失败: " . $e->getMessage());
来源：http://iwp.xuanzx.com

[U73] PHP：读取 ini 配置
来源：http://liq.meibo888.top

parse_ini_file("config.ini", true)
来源：http://zhe.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://lwa.gotoacloud.top

getenv("APP_ENV") ?: "production"
来源：http://vzk.xziqi.cn

[U75] PHP：依赖注入
来源：http://xfh.wangshuangyany.cn

composer require psr/container
来源：http://cec.daxiang520.top

[U76] PHP：简单路由
来源：http://nqh.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jei.gzhubu.top

[U77] PHP：模板渲染
来源：http://bjk.jinghuilouyu.cn

composer require twig/twig
来源：http://gvj.fehbvm.com

[U78] PHP：单元测试
来源：http://ibd.tian-w.cn

composer require --dev phpunit/phpunit
来源：http://fla.fzhhl.top


<!-- 参考信息 -->