代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://hwh.tarul.cn

[S59] C++：静态断言
来源：http://put.wangshuangyany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fhs.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://qik.cheryme.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vkk.jinghuilouyu.cn

================================================================================
来源：http://mlq.zdqjudy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ooy.wangdashe.top

================================================================================
来源：http://kte.zycfv.cn

[T01] Kotlin：Hello World
来源：http://mkf.sjlbkw.cn

println("Hello")
来源：http://ukj.yueranfly.top

[T02] Kotlin：变量
来源：http://gvb.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sfc.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://eyk.zhaomingkeji.xyz

"值: $b"
来源：http://jtd.cheryme.top

[T04] Kotlin：空安全
来源：http://amb.wangshuangyany.cn

val n: String? = null;  n?.length
来源：http://ihy.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://ife.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rpr.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://ntq.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jlo.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://jjo.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cij.fzhhl.top

[T08] Kotlin：数据类
来源：http://wnl.cqqwz.cn

data class User(val name: String, val age: Int)
来源：http://vqc.zdbjq.cn

[T09] Kotlin：扩展函数
来源：http://fuf.zhijiandao.cn

fun String.exclaim() = this + "!"
来源：http://htp.bjfxy.top

[T10] Kotlin：默认参数
来源：http://qbj.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://ryo.xuanzx.com

[T11] Kotlin：协程
来源：http://dcu.nanxinkj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ubf.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://bxy.shzxlz.cn

val (a, b) = Pair(1, 2)
来源：http://lcx.tanke756.top

[T13] Kotlin：只读 Map
来源：http://vcd.shzxlz.cn

val m = mapOf("a" to 1)
来源：http://twu.yanxiufei.cn

[T14] Kotlin：循环
来源：http://lil.xziqi.cn

for (i in 1..10) println(i)
来源：http://uit.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://nua.zhijiandao.cn

interface Shape { fun area(): Double }
来源：http://rto.andypj.xyz

[T16] Swift：Hello World
来源：http://pad.daria6918.cn

print("Hello")
来源：http://mbt.svipenyu.cn

[T17] Swift：变量与常量
来源：http://due.zhaomingkeji.xyz

var a = 1;  let b = 2
来源：http://msc.9152youxi.cn

[T18] Swift：字符串插值
来源：http://ekq.cdnleiting.top

"值: \(b)"
来源：http://udg.snrcjt.cn

[T19] Swift：可选绑定
来源：http://wmg.gotoacloud.top

if let n = opt { print(n) }
来源：http://nze.wangshuangyany.cn

[T20] Swift：数组操作
来源：http://rrk.jlsjyb.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qaa.zhongyouzk.top

[T21] Swift：遍历
来源：http://nua.tian-w.cn

for x in a { print(x) }
来源：http://pee.cashguo.top

[T22] Swift：字典
来源：http://wpy.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://hao.tianlin.xyz

[T23] Swift：函数
来源：http://rim.ehwqpu.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qec.zhoulong.xyz

[T24] Swift：闭包
来源：http://pxs.zycfv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xvo.svipenyu.cn

[T25] Swift：结构体
来源：http://xms.dianchejie.cn

struct P { var x: Int }
来源：http://hii.xziqi.cn

[T26] Swift：类与重写
来源：http://oqz.yangfankeji.com

class A: Base { override func f() {} }
来源：http://noc.xuanzx.com

[T27] Swift：错误处理
来源：http://dac.iojbl.cn

do { try f() } catch { print(error) }
来源：http://ljd.zhiwuduotai.top

[T28] Swift：枚举
来源：http://oiv.shanyushiyangtech.top

enum Color { case red, green }
来源：http://qdh.ywan-chungtsiang.top

[T29] Swift：guard 提前返回
来源：http://lga.cqqwz.cn

guard let x = opt else { return }
来源：http://xzw.sysykeji.top

[T30] Swift：协议
来源：http://mqx.jinqigufen.top

protocol Shape { func area() -> Double }
来源：http://ork.gogol.net.cn

[T31] Lua：Hello World
来源：http://nqf.wangdashe.top

print("Hello")
来源：http://myu.nanxuanxn.top

[T32] Lua：局部变量
来源：http://hwq.sjlbkw.cn

local a = 1
来源：http://myv.yongpay.top

[T33] Lua：表（数组）
来源：http://srp.yuanzhike.top

local t = {1, 2, 3};  t[4] = 4
来源：http://prt.feifeiyinyue.top

[T34] Lua：遍历表
来源：http://ova.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ffc.iojbl.cn

[T35] Lua：字典表
来源：http://xwx.cdnleiting.top

local d = { a = 1 };  d.b = 2
来源：http://xfo.hongshengwenyu.top

[T36] Lua：函数
来源：http://wmg.smart0.xyz

function add(a, b) return a + b end
来源：http://nhd.yongpay.top

[T37] Lua：字符串拼接
来源：http://rrk.feifeiyinyue.top

"a" .. "b"
来源：http://poc.birdmap.top

[T38] Lua：条件
来源：http://qim.iojbl.cn

if x > 0 then print("正") end
来源：http://xqv.bbcook.cn

[T39] Lua：模式匹配
来源：http://ect.cdnleiting.top

string.find(s, "%d+")
来源：http://awn.jiagoushi.top

[T40] Lua：元表
来源：http://buj.jiagoushi.top

setmetatable({}, { __index = base })
来源：http://jik.fengsongda.top

[T41] Perl：Hello World
来源：http://srj.redwolf501.top

print "Hello\n";
来源：http://eih.dianchejie.cn

[T42] Perl：变量类型
来源：http://fdq.jinqigfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uvg.chenzaomai.com

[T43] Perl：字符串插值
来源：http://eyp.ydjk.org.cn

"值: $a"
来源：http://vdz.ywan-chungtsiang.top

[T44] Perl：条件
来源：http://sml.tarul.cn

if ($a > 0) { print "正"; }
来源：http://fnz.tarul.cn

[T45] Perl：数组遍历
来源：http://ovd.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://zgg.yangfankeji.com

[T46] Perl：哈希操作
来源：http://crd.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vws.bjfxy.top

[T47] Perl：正则捕获
来源：http://lpy.nanxinkj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jdm.shzxlz.cn

[T48] Perl：正则替换
来源：http://mpe.sweek.top

$s =~ s/old/new/g;
来源：http://qda.hesvh.cn

[T49] Perl：函数
来源：http://thy.jinyuanbaomall.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zkv.bbcook.cn

[T50] Perl：逐行读文件
来源：http://qwd.nanxuanxn.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bxg.xylfe.cn

while (my $line = <$fh>) { print $line; }
来源：http://ejr.daria6918.cn

[T51] Scala：Hello World
来源：http://kos.sxryk.cn

println("Hello")
来源：http://jnf.fehbvm.com

[T52] Scala：变量
来源：http://bpk.smart0.xyz

val a = 1;  var b = 2
来源：http://rzt.ppjwa.cn

[T53] Scala：字符串插值
来源：http://mjp.ivvv.top

s"值: $b"
来源：http://wnv.ppjwa.cn

[T54] Scala：集合映射
来源：http://cdp.daria6918.cn

List(1, 2, 3).map(_ * 2)
来源：http://twl.cdnleiting.top

[T55] Scala：集合过滤
来源：http://xlo.tianlin.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://glk.sufxvd.cn

[T56] Scala：样例类
来源：http://yop.sufxvd.cn

case class User(name: String, age: Int)
来源：http://bmc.fengsongda.top

[T57] Scala：模式匹配
来源：http://acj.birdmap.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://von.ywan-chungtsiang.top

[T58] Scala：函数定义
来源：http://gzi.bbcook.cn

def add(a: Int, b: Int): Int = a + b
来源：http://aic.9152youxi.cn

[T59] Scala：循环
来源：http://dlw.gotoacloud.top

for (i <- 1 to 10) println(i)
来源：http://wjn.haohaochexian.top

[T60] Scala：折叠
来源：http://otn.shangyingyoupin.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://znn.andypj.xyz

================================================================================
来源：http://tuk.yj202588.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://odt.chenzaomai.com

================================================================================
来源：http://vco.ywan-chungtsiang.top

[U01] Py：创建虚拟环境
来源：http://dbk.yanxiufei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gmf.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://dyk.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pej.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://nvs.chenlongwang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ihk.zycfv.cn

[U04] Py：变量调试打印
来源：http://bxf.birdmap.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lmg.guannengcc.top

[U05] Py：列表去重且保序
来源：http://gay.xinyue.icu

list(dict.fromkeys(arr))
来源：http://opt.sysykeji.top

[U06] Py：合并两个字典
来源：http://oqu.c1oappe.top

{**a, **b}
来源：http://bye.snrcjt.cn

[U07] Py：反转字典键值
来源：http://ieh.epnwcf.com

{v: k for k, v in d.items()}
来源：http://ycm.bbcook.cn

[U08] Py：展平二维列表
来源：http://jki.zdqjudy.top

[y for x in nested for y in x]
来源：http://edm.316326.xyz

[U09] Py：字典取最大值的键
来源：http://sjq.jqgfzy.top

max(d, key=d.get)
来源：http://xex.tarul.cn

[U10] Py：按值排序字典
来源：http://hgo.jlsjyb.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kho.hnxiangtu.top

[U11] Py：生成器表达式
来源：http://xsk.ybcxt.top

(x * 2 for x in arr)
来源：http://hmu.ywan-chungtsiang.top

[U12] Py：取出现最多的 3 个元素
来源：http://exd.ywan-chungtsiang.top

Counter(arr).most_common(3)
来源：http://gcs.yuxming.cn

[U13] Py：固定长度队列
来源：http://qfs.yangfankeji.com

deque(maxlen=10)
来源：http://ypn.zhongyouzk.top

[U14] Py：分组收集到列表
来源：http://hey.sxryk.cn

defaultdict(list)
来源：http://cbj.shanyushiyangkeji.top

[U15] Py：高精度计时
来源：http://bgw.jinqigufen.top

t = time.perf_counter()
来源：http://yst.hnqzz.top

[U16] Py：命令行参数解析
来源：http://kbs.sysykeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ami.snrcjt.cn

[U17] Py：初始化日志
来源：http://gyt.snrcjt.cn

logging.basicConfig(level=logging.INFO)
来源：http://twn.gotoacloud.top

[U18] Py：预编译正则
来源：http://jpj.yj20258888.top

pat = re.compile(r"\d+")
来源：http://jhd.bbcook.cn

[U19] Py：正则替换带回调
来源：http://uty.pycfn.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wnx.bjfxy.top

[U20] Py：缓存函数结果
来源：http://nnp.chenjidiqi.icu

@functools.lru_cache(maxsize=None)
来源：http://nsa.chenzaomai.com

[U21] Py：自定义上下文管理器
来源：http://rre.vqdsnc.cn

@contextlib.contextmanager
来源：http://etc.smart0.xyz

[U22] Py：矩阵转置
来源：http://qed.dianchejie.cn

list(zip(*m))
来源：http://qxt.pycfn.com

[U23] Py：分块读取大文件
来源：http://lyu.yangfankeji.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vxl.hysaishi.cn

[U24] Py：路径操作
来源：http://qdu.kuanghao11.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://taw.chenlongwang.top

[U25] Py：CSV 按字典读
来源：http://zun.hongshengwenyu.top

csv.DictReader(f)
来源：http://nhd.hywenlv.cn

[U26] Py：并发下载
来源：http://sjx.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nyu.hesvh.cn

[U27] Py：异步 HTTP
来源：http://ywj.sweek.top

aiohttp.ClientSession() 配合 async with
来源：http://dwf.fanxiaobao.xyz

[U28] Py：类型别名
来源：http://hcz.jianghu66.top

UserId = int
来源：http://xwg.guannengcc.top

[U29] Py：属性校验
来源：http://oni.hcnkem.com

@property 与 @x.setter 配合
来源：http://kal.ctjpmb.com

[U30] Py：数据类
来源：http://fgd.jinyuanbaomall.cn

@dataclass(slots=True)
来源：http://dmj.shzxlz.cn

[U31] Py：单测
来源：http://nkj.smart0.xyz

python -m pytest -q
来源：http://luv.ydzc1.top

[U32] Py：代码格式化
来源：http://kpe.kuanghao11.cn

ruff format . && ruff check --fix .
来源：http://mxa.chenjidiqi.icu

[U33] Py：打包发布
来源：http://wcn.quarkkingdee.top

python -m build  （依赖 pyproject.toml）
来源：http://zhc.zhoulong.xyz

[U34] Py：判断编码
来源：http://qjx.hfpthk.cn

chardet.detect(raw)
来源：http://umr.redwolf501.top

[U35] Py：发送邮件
来源：http://xyc.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://idf.guowangkeji.top

[U36] Py：定时任务
来源：http://kbm.uphjek.com

schedule.every(10).minutes.do(job)
来源：http://bxb.xylfe.cn

[U37] Py：读写 Excel
来源：http://upv.shanyushiyangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://vuq.yuanzhike.top

[U38] Py：获取脚本所在目录
来源：http://vnf.gotoacloud.top

Path(__file__).resolve().parent
来源：http://gpx.ydjk.org.cn

[U39] Py：判断是否在交互环境
来源：http://qul.daria6918.cn

sys.stdout.isatty()
来源：http://qol.bbcook.cn

[U40] Py：打印到标准错误
来源：http://qys.9152youxi.cn

print("err", file=sys.stderr)
来源：http://pdo.cashguo.top

[U41] PHP：初始化 Composer 项目
来源：http://qqf.jyoumei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bei.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://qoy.gogol.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ijb.wangshuangyany.cn

[U43] PHP：声明命名空间
来源：http://gxf.yueranfly.top

namespace App\Http;
来源：http://wsn.sysykeji.top

[U44] PHP：开启严格类型
来源：http://rig.vehdjk.com

declare(strict_types=1);
来源：http://nnk.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://xcs.fzhhl.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zhc.jqgufenzy.top

[U46] PHP：可空类型
来源：http://rrn.hnxiangtu.top

?string $name = null
来源：http://ity.cucudq.cn

[U47] PHP：联合类型
来源：http://oat.tarul.cn

int|string $id
来源：http://snj.tarul.cn

[U48] PHP：纯枚举
来源：http://mrk.jinqigfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gcg.sysykeji.top

[U49] PHP：只读属性
来源：http://rfi.svipenyu.cn

public readonly string $name
来源：http://uzb.9152youxi.cn

[U50] PHP：构造器属性提升
来源：http://mji.tianlin.xyz

public function __construct(private int $id) {}
来源：http://auk.zhengqikj.top

[U51] PHP：数组解构
来源：http://rcb.shuidangran.top

[$a, $b] = $arr;
来源：http://vhy.0kj1m.cn

[U52] PHP：箭头函数
来源：http://knk.jinqigfzy.top

$double = fn($x) => $x * 2;
来源：http://tfj.ivvv.top

[U53] PHP：空合并运算符
来源：http://qww.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://llc.dianchejie.cn

[U54] PHP：空安全调用
来源：http://pgs.xuanzx.com

$obj?->method()
来源：http://lol.yongpay.top

[U55] PHP：match 表达式
来源：http://iuj.zycfv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zwh.redwolf501.top

[U56] PHP：命名参数
来源：http://tmc.yueranfly.top

f(a: 1, b: 2)
来源：http://dsp.pycfn.com

[U57] PHP：字符串插值
来源：http://qwo.birdmap.top

"值: {$a}"
来源：http://iwy.pycfn.com

[U58] PHP：数组三件套
来源：http://znc.316326.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bkw.uphjek.com

[U59] PHP：自定义排序
来源：http://ipj.yj20258888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wru.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://bxx.52xcode.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vqn.iojbl.cn

[U61] PHP：正则
来源：http://kcc.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cvs.zhaomingkeji.xyz

[U62] PHP：日期对象
来源：http://okf.jqgufenzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sjs.yj202588.top

[U63] PHP：文件读写
来源：http://cqr.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jaf.ydzc1.top

[U64] PHP：目录遍历
来源：http://xgt.yuxming.cn

glob("dir/*.php");  scandir("dir");
来源：http://svx.xuetiantiany.cn

[U65] PHP：会话
来源：http://mba.zhijiandao.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qch.jyoumei.cn

[U66] PHP：设置 Cookie
来源：http://nrs.fktsv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://her.dashuyun.cn

[U67] PHP：处理文件上传
来源：http://myu.52xcode.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qpx.hywenlv.cn

[U68] PHP：PDO 连接
来源：http://ozy.xuanzx.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tgw.xingfuxueyuan.xyz

[U69] PHP：PDO 预处理
来源：http://hxp.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nby.aizwys.cn

[U70] PHP：PDO 事务
来源：http://edh.dianchejie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zrq.0kj1m.cn

[U71] PHP：抛出异常
来源：http://flw.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://scj.quarkkingdee.top

[U72] PHP：写错误日志
来源：http://eqe.ydzc1.top

error_log("失败: " . $e->getMessage());
来源：http://gri.haohaochexian.top

[U73] PHP：读取 ini 配置
来源：http://wsg.zycfv.cn

parse_ini_file("config.ini", true)
来源：http://iwg.xinyue.icu

[U74] PHP：读取环境变量
来源：http://chn.aibaodan.cn

getenv("APP_ENV") ?: "production"
来源：http://yvf.wangdashe.top

[U75] PHP：依赖注入
来源：http://ost.ivvv.top

composer require psr/container
来源：http://wck.xingfuxueyuan.xyz

[U76] PHP：简单路由
来源：http://mcm.dashuyun.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bpf.zhaomingkeji.xyz

[U77] PHP：模板渲染
来源：http://dkz.yvedp.cn

composer require twig/twig
来源：http://ipr.pengpengdd.cyou

[U78] PHP：单元测试
来源：http://tgd.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://ctl.daria6918.cn

[U79] PHP：静态分析
来源：http://ari.zhengqikj.top

composer require --dev phpstan/phpstan
来源：http://ney.hammf.cn

[U80] PHP：代码规范修复
来源：http://jiq.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gyw.fengsongda.top

[U81] JS：初始化项目
来源：http://zhp.vehdjk.com

npm init -y;  npm i express
来源：http://rex.daria6918.cn

[U82] JS：package.json 脚本
来源：http://yhx.fzhhl.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xyk.yj20258888.top

[U83] JS：ES Module 导入导出
来源：http://ppu.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://xtr.gaohongyu789.top

[U84] JS：CommonJS 写法
来源：http://aew.tianlin.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://sch.hfpthk.cn


<!-- 参考信息 -->