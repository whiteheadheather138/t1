代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aea.sweek.top

[S57] C++：编译期常量
来源：http://bwk.316326.xyz

constexpr int N = 10;
来源：http://ehy.zhixingplan.top

[S58] C++：命名空间
来源：http://qcc.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://zkr.9152youxi.cn

[S59] C++：静态断言
来源：http://fzk.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xjz.cqqwz.cn

[S60] C++：遍历并删除元素
来源：http://zpz.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gzq.zycfv.cn

================================================================================
来源：http://ydf.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mow.hfpthk.cn

================================================================================
来源：http://ckt.gzhubu.top

[T01] Kotlin：Hello World
来源：http://wan.meibo888.top

println("Hello")
来源：http://bja.zhongyouzk.top

[T02] Kotlin：变量
来源：http://myc.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nrs.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://mav.guannengcc.top

"值: $b"
来源：http://zro.jinqigufen.top

[T04] Kotlin：空安全
来源：http://ugc.haohaochexian.top

val n: String? = null;  n?.length
来源：http://rfy.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://dmr.fktsv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zyr.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://gkt.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bko.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://cqo.xingfuxueyuan.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://wvb.dashuyun.cn

[T08] Kotlin：数据类
来源：http://nyd.jinghuilouyu.cn

data class User(val name: String, val age: Int)
来源：http://ooe.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://lvx.havefunace.top

fun String.exclaim() = this + "!"
来源：http://zhu.yuxming.cn

[T10] Kotlin：默认参数
来源：http://mvb.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://slt.tarul.cn

[T11] Kotlin：协程
来源：http://bry.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://irp.redwolf501.top

[T12] Kotlin：解构声明
来源：http://lsj.gzhubu.top

val (a, b) = Pair(1, 2)
来源：http://eqp.yongpay.top

[T13] Kotlin：只读 Map
来源：http://eca.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://ezp.yongpay.top

[T14] Kotlin：循环
来源：http://irv.chenjidiqi.icu

for (i in 1..10) println(i)
来源：http://thx.ydjk.org.cn

[T15] Kotlin：接口
来源：http://uel.jqgfzy.top

interface Shape { fun area(): Double }
来源：http://owm.smart0.xyz

[T16] Swift：Hello World
来源：http://jcz.yueranfly.top

print("Hello")
来源：http://zrg.guowangkeji.top

[T17] Swift：变量与常量
来源：http://yoj.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://owh.jianghu66.top

[T18] Swift：字符串插值
来源：http://pfx.sjlbkw.cn

"值: \(b)"
来源：http://uwn.cdnleiting.top

[T19] Swift：可选绑定
来源：http://ghj.hywenlv.cn

if let n = opt { print(n) }
来源：http://nap.dashuyun.cn

[T20] Swift：数组操作
来源：http://ejf.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://ksg.yueranfly.top

[T21] Swift：遍历
来源：http://urx.yongpay.top

for x in a { print(x) }
来源：http://ucr.sjlbkw.cn

[T22] Swift：字典
来源：http://kog.nwbrower.top

var d = ["a": 1];  d["b"] = 2
来源：http://xwj.chenjidiqi.icu

[T23] Swift：函数
来源：http://umu.tanke756.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pxh.hywenlv.cn

[T24] Swift：闭包
来源：http://mgu.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jmk.yongpay.top

[T25] Swift：结构体
来源：http://rte.pengpengdd.cyou

struct P { var x: Int }
来源：http://jgm.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://ulb.xuanzx.com

class A: Base { override func f() {} }
来源：http://nhd.cashguo.top

[T27] Swift：错误处理
来源：http://med.jinghuilouyu.cn

do { try f() } catch { print(error) }
来源：http://dlb.ehwqpu.com

[T28] Swift：枚举
来源：http://eui.wangshuangyany.cn

enum Color { case red, green }
来源：http://tka.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://yhf.jqgfzy.top

guard let x = opt else { return }
来源：http://nqp.gotoacloud.top

[T30] Swift：协议
来源：http://opp.52xcode.cn

protocol Shape { func area() -> Double }
来源：http://afq.chenlongwang.top

[T31] Lua：Hello World
来源：http://nyz.sweek.top

print("Hello")
来源：http://dtc.xylfe.cn

[T32] Lua：局部变量
来源：http://zzb.xinyue.icu

local a = 1
来源：http://mih.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://pbc.fengsongda.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pau.yj20258.top

[T34] Lua：遍历表
来源：http://vaj.zhoulong.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://pmn.shzxlz.cn

[T35] Lua：字典表
来源：http://oby.bbcook.cn

local d = { a = 1 };  d.b = 2
来源：http://ecp.uphjek.com

[T36] Lua：函数
来源：http://osu.ehwqpu.com

function add(a, b) return a + b end
来源：http://qld.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://ekn.tanke756.top

"a" .. "b"
来源：http://ldk.bjfxy.top

[T38] Lua：条件
来源：http://nza.nwbrower.top

if x > 0 then print("正") end
来源：http://ufl.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://noj.wangdashe.top

string.find(s, "%d+")
来源：http://oya.xziqi.cn

[T40] Lua：元表
来源：http://sli.ybcxt.top

setmetatable({}, { __index = base })
来源：http://cwx.gzhubu.top

[T41] Perl：Hello World
来源：http://cbe.sjlbkw.cn

print "Hello\n";
来源：http://mng.yongpay.top

[T42] Perl：变量类型
来源：http://tii.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gzr.yj20258888.top

[T43] Perl：字符串插值
来源：http://oon.xuanzx.com

"值: $a"
来源：http://qrd.sufxvd.cn

[T44] Perl：条件
来源：http://jok.cqqwz.cn

if ($a > 0) { print "正"; }
来源：http://cvl.tian-w.cn

[T45] Perl：数组遍历
来源：http://ecx.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://msd.cqqwz.cn

[T46] Perl：哈希操作
来源：http://vlh.tianlin.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fdm.fengsongda.top

[T47] Perl：正则捕获
来源：http://wvs.quarkkingdee.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tfa.52xcode.cn

[T48] Perl：正则替换
来源：http://jls.yj20258.top

$s =~ s/old/new/g;
来源：http://edn.yfazqb.com

[T49] Perl：函数
来源：http://vdc.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lfe.havefunace.top

[T50] Perl：逐行读文件
来源：http://xsy.yj20258888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dxc.316326.xyz

while (my $line = <$fh>) { print $line; }
来源：http://zvp.ydzc1.top

[T51] Scala：Hello World
来源：http://sdz.xuetiantiany.cn

println("Hello")
来源：http://aai.vehdjk.com

[T52] Scala：变量
来源：http://bnl.chenjidiqi.icu

val a = 1;  var b = 2
来源：http://sep.sysykeji.top

[T53] Scala：字符串插值
来源：http://jvd.hesvh.cn

s"值: $b"
来源：http://ddh.9152youxi.cn

[T54] Scala：集合映射
来源：http://oem.jinyuanbaomall.cn

List(1, 2, 3).map(_ * 2)
来源：http://psm.cucudq.cn

[T55] Scala：集合过滤
来源：http://jnf.zhoulong.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://anv.daria6918.cn

[T56] Scala：样例类
来源：http://nbh.daxiang520.top

case class User(name: String, age: Int)
来源：http://xyf.sufxvd.cn

[T57] Scala：模式匹配
来源：http://fgj.nanxuanxn.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://oyb.shangyingyoupin.top

[T58] Scala：函数定义
来源：http://zss.yuxming.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xuv.yj202588.top

[T59] Scala：循环
来源：http://row.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://mdf.hywenlv.cn

[T60] Scala：折叠
来源：http://dxk.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vfo.feifeiyinyue.top

================================================================================
来源：http://yyo.ywan-chungtsiang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xns.sysykeji.top

================================================================================
来源：http://ary.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://xdr.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tcx.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://xrx.zhengqikj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ocx.andypj.xyz

[U03] Py：加载 .env 配置
来源：http://fox.xuetiantiany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oou.fzhhl.top

[U04] Py：变量调试打印
来源：http://bil.jianghu66.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ysw.hongshengwenyu.top

[U05] Py：列表去重且保序
来源：http://stm.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://eha.kuanghao11.cn

[U06] Py：合并两个字典
来源：http://nxf.yongpay.top

{**a, **b}
来源：http://vza.uphjek.com

[U07] Py：反转字典键值
来源：http://dfb.wangshuangyany.cn

{v: k for k, v in d.items()}
来源：http://qjy.zdqjudy.top

[U08] Py：展平二维列表
来源：http://crh.epnwcf.com

[y for x in nested for y in x]
来源：http://ypv.jianghu66.top

[U09] Py：字典取最大值的键
来源：http://kfz.guannengcc.top

max(d, key=d.get)
来源：http://ybf.haohaochexian.top

[U10] Py：按值排序字典
来源：http://njc.cucudq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dhm.guannengcc.top

[U11] Py：生成器表达式
来源：http://jij.smart0.xyz

(x * 2 for x in arr)
来源：http://xpo.jinghuilouyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zjo.ctjpmb.com

Counter(arr).most_common(3)
来源：http://vfm.hysaishi.cn

[U13] Py：固定长度队列
来源：http://ged.dianchejie.cn

deque(maxlen=10)
来源：http://ajp.yonumen.top

[U14] Py：分组收集到列表
来源：http://wlf.hfpthk.cn

defaultdict(list)
来源：http://ivm.aibaodan.cn

[U15] Py：高精度计时
来源：http://lsn.hongshengwenyu.top

t = time.perf_counter()
来源：http://yiy.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://cag.cheryme.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xqw.gotoacloud.top

[U17] Py：初始化日志
来源：http://cpy.epnwcf.com

logging.basicConfig(level=logging.INFO)
来源：http://lyy.jinqigfzy.top

[U18] Py：预编译正则
来源：http://llt.shanyushiyangtech.top

pat = re.compile(r"\d+")
来源：http://bma.bbcook.cn

[U19] Py：正则替换带回调
来源：http://zzu.feifeiyinyue.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nmn.wangdashe.top

[U20] Py：缓存函数结果
来源：http://crl.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://jqx.sufxvd.cn

[U21] Py：自定义上下文管理器
来源：http://wvt.yj20258.top

@contextlib.contextmanager
来源：http://zps.shuidangran.top

[U22] Py：矩阵转置
来源：http://exu.cdnleiting.top

list(zip(*m))
来源：http://pox.guannengcc.top

[U23] Py：分块读取大文件
来源：http://jgr.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bwo.guowangkeji.top

[U24] Py：路径操作
来源：http://dpb.c1oappe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jkb.yueranfly.top

[U25] Py：CSV 按字典读
来源：http://sev.tarul.cn

csv.DictReader(f)
来源：http://nwi.bbcook.cn

[U26] Py：并发下载
来源：http://aeb.aibaodan.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rzs.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://drv.ivvv.top

aiohttp.ClientSession() 配合 async with
来源：http://qob.c1oappe.top

[U28] Py：类型别名
来源：http://noq.yvedp.cn

UserId = int
来源：http://jhf.xuanzx.com

[U29] Py：属性校验
来源：http://rux.hcnkem.com

@property 与 @x.setter 配合
来源：http://ino.ydzc1.top

[U30] Py：数据类
来源：http://xev.yj202588.top

@dataclass(slots=True)
来源：http://aqk.xinyue.icu

[U31] Py：单测
来源：http://cad.cucudq.cn

python -m pytest -q
来源：http://rle.xziqi.cn

[U32] Py：代码格式化
来源：http://dma.dashuyun.cn

ruff format . && ruff check --fix .
来源：http://ceg.jqgufenzy.top

[U33] Py：打包发布
来源：http://rxa.hnxiangtu.top

python -m build  （依赖 pyproject.toml）
来源：http://tmr.yj202588.top

[U34] Py：判断编码
来源：http://cvg.shanyushiyangkeji.top

chardet.detect(raw)
来源：http://azc.ydjk.org.cn

[U35] Py：发送邮件
来源：http://tzf.jiagoushi.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://win.jyoumei.cn

[U36] Py：定时任务
来源：http://jwm.smart0.xyz

schedule.every(10).minutes.do(job)
来源：http://kar.52xcode.cn

[U37] Py：读写 Excel
来源：http://tfm.snrcjt.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cao.epnwcf.com

[U38] Py：获取脚本所在目录
来源：http://pfy.hysaishi.cn

Path(__file__).resolve().parent
来源：http://bnw.xylfe.cn

[U39] Py：判断是否在交互环境
来源：http://mba.hnxiangtu.top

sys.stdout.isatty()
来源：http://min.birdmap.top

[U40] Py：打印到标准错误
来源：http://gdb.gaohongyu789.top

print("err", file=sys.stderr)
来源：http://hqj.tian-w.cn

[U41] PHP：初始化 Composer 项目
来源：http://ecp.jinghuilouyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wcb.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://zad.ctjpmb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mii.uphjek.com

[U43] PHP：声明命名空间
来源：http://jhu.bjfxy.top

namespace App\Http;
来源：http://krs.ctjpmb.com

[U44] PHP：开启严格类型
来源：http://wnv.yanxiufei.cn

declare(strict_types=1);
来源：http://aak.hcnkem.com

[U45] PHP：类型声明与返回类型
来源：http://rao.gaohongyu789.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://whi.sxryk.cn

[U46] PHP：可空类型
来源：http://flw.gzhubu.top

?string $name = null
来源：http://kkk.jlsjyb.cn

[U47] PHP：联合类型
来源：http://lgf.yuxming.cn

int|string $id
来源：http://puj.nwbrower.top

[U48] PHP：纯枚举
来源：http://vce.shanyushiyangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dxx.shangyingyoupin.top

[U49] PHP：只读属性
来源：http://dte.zycfv.cn

public readonly string $name
来源：http://dpg.fktsv.cn

[U50] PHP：构造器属性提升
来源：http://mwc.gzhubu.top

public function __construct(private int $id) {}
来源：http://yjn.shanyushiyangkeji.top

[U51] PHP：数组解构
来源：http://gku.hongshengwenyu.top

[$a, $b] = $arr;
来源：http://pfg.wangshuangyany.cn

[U52] PHP：箭头函数
来源：http://iny.nanxinkj.top

$double = fn($x) => $x * 2;
来源：http://zcd.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://zwx.ydjk.org.cn

$v = $a ?? $b ?? "default";
来源：http://lwf.zdbjq.cn

[U54] PHP：空安全调用
来源：http://xxy.fehbvm.com

$obj?->method()
来源：http://etw.chenzaomai.com

[U55] PHP：match 表达式
来源：http://okb.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xrg.guowangkeji.top

[U56] PHP：命名参数
来源：http://tku.ivvv.top

f(a: 1, b: 2)
来源：http://kfg.zdqjudy.top

[U57] PHP：字符串插值
来源：http://pwt.cashguo.top

"值: {$a}"
来源：http://cry.nanxuanxn.top

[U58] PHP：数组三件套
来源：http://dkq.xuanzx.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zap.yj20258888.top

[U59] PHP：自定义排序
来源：http://cta.yonumen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yct.cucudq.cn

[U60] PHP：JSON 编解码
来源：http://wfh.andypj.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rpd.hesvh.cn

[U61] PHP：正则
来源：http://haz.gzhubu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cpx.cucudq.cn

[U62] PHP：日期对象
来源：http://tmt.sufxvd.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wmc.zhixingplan.top

[U63] PHP：文件读写
来源：http://lun.birdmap.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nek.yuxming.cn

[U64] PHP：目录遍历
来源：http://fyv.zycfv.cn

glob("dir/*.php");  scandir("dir");
来源：http://yum.zhoulong.xyz

[U65] PHP：会话
来源：http://iyp.zdqjudy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dff.shangyingyoupin.top

[U66] PHP：设置 Cookie
来源：http://gtf.hesvh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dtg.mhx1999.top

[U67] PHP：处理文件上传
来源：http://agr.cheryme.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lnk.pycfn.com

[U68] PHP：PDO 连接
来源：http://wrr.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jet.yj20258.top

[U69] PHP：PDO 预处理
来源：http://hhe.zhongyouzk.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kmp.tian-w.cn

[U70] PHP：PDO 事务
来源：http://vlv.havefunace.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zpg.yj20258.top

[U71] PHP：抛出异常
来源：http://axn.chenzaomai.com

throw new RuntimeException("失败", 500);
来源：http://nmk.ywan-chungtsiang.top

[U72] PHP：写错误日志
来源：http://fty.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://swl.cqqwz.cn

[U73] PHP：读取 ini 配置
来源：http://jvf.zhiwuduotai.top

parse_ini_file("config.ini", true)
来源：http://ydx.nanxinkj.top

[U74] PHP：读取环境变量
来源：http://mos.quarkkingdee.top

getenv("APP_ENV") ?: "production"
来源：http://yat.hongshengwenyu.top

[U75] PHP：依赖注入
来源：http://ctt.snrcjt.cn

composer require psr/container
来源：http://jgw.fanxiaobao.xyz

[U76] PHP：简单路由
来源：http://zsr.shangyingyoupin.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ggu.jqgfzy.top

[U77] PHP：模板渲染
来源：http://vfn.0kj1m.cn

composer require twig/twig
来源：http://mqh.hcnkem.com

[U78] PHP：单元测试
来源：http://qcv.shanyushiyangtech.top

composer require --dev phpunit/phpunit
来源：http://bmz.feifeiyinyue.top

[U79] PHP：静态分析
来源：http://xfd.dashuyun.cn

composer require --dev phpstan/phpstan
来源：http://oqv.yuxming.cn

[U80] PHP：代码规范修复
来源：http://uhz.snrcjt.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ifq.smart0.xyz

[U81] JS：初始化项目
来源：http://cgc.zycfv.cn

npm init -y;  npm i express
来源：http://gbw.52xcode.cn

[U82] JS：package.json 脚本
来源：http://ssp.hnxiangtu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://omy.nanxinkj.top


<!-- 参考信息 -->