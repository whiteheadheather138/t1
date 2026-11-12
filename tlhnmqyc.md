代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fwm.zhijiandao.cn

================================================================================
来源：http://hlo.nanxuanxn.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mof.ppjwa.cn

================================================================================
来源：http://ipv.bbcook.cn

[T01] Kotlin：Hello World
来源：http://nni.meibo888.top

println("Hello")
来源：http://rhu.ydjk.org.cn

[T02] Kotlin：变量
来源：http://yja.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xsd.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://fvy.tianlin.xyz

"值: $b"
来源：http://kbd.vehdjk.com

[T04] Kotlin：空安全
来源：http://zkb.birdmap.top

val n: String? = null;  n?.length
来源：http://jyd.yonumen.top

[T05] Kotlin：when 表达式
来源：http://yla.nanxinkj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iyr.zycfv.cn

[T06] Kotlin：集合映射
来源：http://dkw.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xyn.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://zdk.hnxiangtu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vkd.haohaochexian.top

[T08] Kotlin：数据类
来源：http://upj.vehdjk.com

data class User(val name: String, val age: Int)
来源：http://elc.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://iyi.zycfv.cn

fun String.exclaim() = this + "!"
来源：http://xeo.yvedp.cn

[T10] Kotlin：默认参数
来源：http://mvd.jlsjyb.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dsg.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://ahn.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pfr.gzhubu.top

[T12] Kotlin：解构声明
来源：http://ldi.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://msf.xingfuxueyuan.xyz

[T13] Kotlin：只读 Map
来源：http://nba.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://chq.ybcxt.top

[T14] Kotlin：循环
来源：http://ppp.sxryk.cn

for (i in 1..10) println(i)
来源：http://tzd.zhixingplan.top

[T15] Kotlin：接口
来源：http://zyq.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://jfs.tian-w.cn

[T16] Swift：Hello World
来源：http://edq.ivvv.top

print("Hello")
来源：http://buu.hongshengwenyu.top

[T17] Swift：变量与常量
来源：http://omu.yangfankeji.com

var a = 1;  let b = 2
来源：http://xba.daria6918.cn

[T18] Swift：字符串插值
来源：http://due.meibo888.top

"值: \(b)"
来源：http://nau.dashuyun.cn

[T19] Swift：可选绑定
来源：http://wse.jinyuanbaomall.cn

if let n = opt { print(n) }
来源：http://iud.bbcook.cn

[T20] Swift：数组操作
来源：http://yky.zhixingplan.top

var a = [1, 2, 3];  a.append(4)
来源：http://kni.hammf.cn

[T21] Swift：遍历
来源：http://qsy.yfazqb.com

for x in a { print(x) }
来源：http://vwa.316326.xyz

[T22] Swift：字典
来源：http://jgc.yueranfly.top

var d = ["a": 1];  d["b"] = 2
来源：http://cpy.ppjwa.cn

[T23] Swift：函数
来源：http://gai.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ply.c1oappe.top

[T24] Swift：闭包
来源：http://hmz.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xvz.zycfv.cn

[T25] Swift：结构体
来源：http://kqa.havefunace.top

struct P { var x: Int }
来源：http://dze.snrcjt.cn

[T26] Swift：类与重写
来源：http://sbi.0kj1m.cn

class A: Base { override func f() {} }
来源：http://wrf.gzhubu.top

[T27] Swift：错误处理
来源：http://sxp.yfazqb.com

do { try f() } catch { print(error) }
来源：http://knj.ctjpmb.com

[T28] Swift：枚举
来源：http://lqd.cdnleiting.top

enum Color { case red, green }
来源：http://eig.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://wmx.quarkkingdee.top

guard let x = opt else { return }
来源：http://gsh.nanxinkj.top

[T30] Swift：协议
来源：http://dqb.vqdsnc.cn

protocol Shape { func area() -> Double }
来源：http://xrg.chenlongwang.top

[T31] Lua：Hello World
来源：http://huy.nanxinkj.top

print("Hello")
来源：http://dbw.xylfe.cn

[T32] Lua：局部变量
来源：http://ezk.aibaodan.cn

local a = 1
来源：http://cbn.snrcjt.cn

[T33] Lua：表（数组）
来源：http://nqt.haohaochexian.top

local t = {1, 2, 3};  t[4] = 4
来源：http://khs.xinyue.icu

[T34] Lua：遍历表
来源：http://yoq.hfpthk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://szk.chenlongwang.top

[T35] Lua：字典表
来源：http://ebz.sufxvd.cn

local d = { a = 1 };  d.b = 2
来源：http://dbd.zhengqikj.top

[T36] Lua：函数
来源：http://ydw.yonumen.top

function add(a, b) return a + b end
来源：http://fpz.yfazqb.com

[T37] Lua：字符串拼接
来源：http://hxj.guannengcc.top

"a" .. "b"
来源：http://cky.tianlin.xyz

[T38] Lua：条件
来源：http://hsv.ctjpmb.com

if x > 0 then print("正") end
来源：http://czh.ydzc1.top

[T39] Lua：模式匹配
来源：http://lmt.ctjpmb.com

string.find(s, "%d+")
来源：http://tcg.yanxiufei.cn

[T40] Lua：元表
来源：http://ywq.uphjek.com

setmetatable({}, { __index = base })
来源：http://ywn.hysaishi.cn

[T41] Perl：Hello World
来源：http://zjq.pycfn.com

print "Hello\n";
来源：http://mek.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://xzo.haohaochexian.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vkl.guowangkeji.top

[T43] Perl：字符串插值
来源：http://xwe.zhaomingkeji.xyz

"值: $a"
来源：http://col.yj202588.top

[T44] Perl：条件
来源：http://rfy.dashuyun.cn

if ($a > 0) { print "正"; }
来源：http://wdb.bbcook.cn

[T45] Perl：数组遍历
来源：http://jku.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://wir.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://jtf.sxryk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vnr.sxryk.cn

[T47] Perl：正则捕获
来源：http://zmj.52xcode.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://smw.ppjwa.cn

[T48] Perl：正则替换
来源：http://qed.yuanzhike.top

$s =~ s/old/new/g;
来源：http://pam.xingfuxueyuan.xyz

[T49] Perl：函数
来源：http://trh.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ing.smart0.xyz

[T50] Perl：逐行读文件
来源：http://zan.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xxu.yvedp.cn

while (my $line = <$fh>) { print $line; }
来源：http://dif.shuidangran.top

[T51] Scala：Hello World
来源：http://zpo.tian-w.cn

println("Hello")
来源：http://usz.tian-w.cn

[T52] Scala：变量
来源：http://hhq.nanxuanxn.top

val a = 1;  var b = 2
来源：http://uod.hywenlv.cn

[T53] Scala：字符串插值
来源：http://mqq.snrcjt.cn

s"值: $b"
来源：http://abf.yj20258.top

[T54] Scala：集合映射
来源：http://qua.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://htg.cdnleiting.top

[T55] Scala：集合过滤
来源：http://trz.zycfv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sxw.tian-w.cn

[T56] Scala：样例类
来源：http://ihu.gogol.net.cn

case class User(name: String, age: Int)
来源：http://dse.hammf.cn

[T57] Scala：模式匹配
来源：http://zjm.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jcd.tarul.cn

[T58] Scala：函数定义
来源：http://ldq.zhengqikj.top

def add(a: Int, b: Int): Int = a + b
来源：http://jaf.sufxvd.cn

[T59] Scala：循环
来源：http://itx.mhx1999.top

for (i <- 1 to 10) println(i)
来源：http://bif.zhoulong.xyz

[T60] Scala：折叠
来源：http://vtx.bbcook.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://czl.yanxiufei.cn

================================================================================
来源：http://qlc.gaohongyu789.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kxk.gotoacloud.top

================================================================================
来源：http://xcg.hnqzz.top

[U01] Py：创建虚拟环境
来源：http://mnf.fktsv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jdh.guannengcc.top

[U02] Py：导出 / 安装依赖
来源：http://fzn.yuanzhike.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://txo.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://pdr.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nao.epnwcf.com

[U04] Py：变量调试打印
来源：http://udu.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dkn.jinyuanbaomall.cn

[U05] Py：列表去重且保序
来源：http://ooa.daxiang520.top

list(dict.fromkeys(arr))
来源：http://kgn.shangyingyoupin.top

[U06] Py：合并两个字典
来源：http://uhr.jinghuilouyu.cn

{**a, **b}
来源：http://ked.bjfxy.top

[U07] Py：反转字典键值
来源：http://ihh.zhengqikj.top

{v: k for k, v in d.items()}
来源：http://xpq.hcnkem.com

[U08] Py：展平二维列表
来源：http://cdz.xinyue.icu

[y for x in nested for y in x]
来源：http://tpw.pycfn.com

[U09] Py：字典取最大值的键
来源：http://txn.zhijiandao.cn

max(d, key=d.get)
来源：http://wsk.tanke756.top

[U10] Py：按值排序字典
来源：http://ysx.zycfv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zsq.feifeiyinyue.top

[U11] Py：生成器表达式
来源：http://ewl.yongpay.top

(x * 2 for x in arr)
来源：http://wnw.yj20258888.top

[U12] Py：取出现最多的 3 个元素
来源：http://myz.tanke756.top

Counter(arr).most_common(3)
来源：http://rpc.aibaodan.cn

[U13] Py：固定长度队列
来源：http://fdo.cqqwz.cn

deque(maxlen=10)
来源：http://fdd.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://vwu.jianghu66.top

defaultdict(list)
来源：http://sza.chenzaomai.com

[U15] Py：高精度计时
来源：http://rhv.c1oappe.top

t = time.perf_counter()
来源：http://ppg.havefunace.top

[U16] Py：命令行参数解析
来源：http://eeo.zhengqikj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zaf.zhiwuduotai.top

[U17] Py：初始化日志
来源：http://scw.fzhhl.top

logging.basicConfig(level=logging.INFO)
来源：http://izb.vehdjk.com

[U18] Py：预编译正则
来源：http://zck.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://qpa.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://aqt.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zqu.quarkkingdee.top

[U20] Py：缓存函数结果
来源：http://mpx.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://wrw.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://kxw.tian-w.cn

@contextlib.contextmanager
来源：http://wrt.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://mhp.hysaishi.cn

list(zip(*m))
来源：http://yil.haohaochexian.top

[U23] Py：分块读取大文件
来源：http://hzf.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jnf.gogol.net.cn

[U24] Py：路径操作
来源：http://lsa.fengsongda.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ipa.jlsjyb.cn

[U25] Py：CSV 按字典读
来源：http://rkv.daria6918.cn

csv.DictReader(f)
来源：http://iue.wangdashe.top

[U26] Py：并发下载
来源：http://gqi.sufxvd.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kod.hnqzz.top

[U27] Py：异步 HTTP
来源：http://xmg.sjlbkw.cn

aiohttp.ClientSession() 配合 async with
来源：http://zob.ywan-chungtsiang.top

[U28] Py：类型别名
来源：http://dwh.fehbvm.com

UserId = int
来源：http://zna.jyoumei.cn

[U29] Py：属性校验
来源：http://fdp.zhoulong.xyz

@property 与 @x.setter 配合
来源：http://nzi.gzhubu.top

[U30] Py：数据类
来源：http://vje.hnxiangtu.top

@dataclass(slots=True)
来源：http://gzx.smart0.xyz

[U31] Py：单测
来源：http://oof.wangshuangyany.cn

python -m pytest -q
来源：http://xhp.ehwqpu.com

[U32] Py：代码格式化
来源：http://wwa.zycfv.cn

ruff format . && ruff check --fix .
来源：http://afu.pengpengdd.cyou

[U33] Py：打包发布
来源：http://dsk.birdmap.top

python -m build  （依赖 pyproject.toml）
来源：http://xdq.bjfxy.top

[U34] Py：判断编码
来源：http://bck.yuanzhike.top

chardet.detect(raw)
来源：http://oxx.nanxuanxn.top

[U35] Py：发送邮件
来源：http://ivw.tarul.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mag.9152youxi.cn

[U36] Py：定时任务
来源：http://mkd.havefunace.top

schedule.every(10).minutes.do(job)
来源：http://iyg.cheryme.top

[U37] Py：读写 Excel
来源：http://oxe.andypj.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://czb.ivvv.top

[U38] Py：获取脚本所在目录
来源：http://etg.hongshengwenyu.top

Path(__file__).resolve().parent
来源：http://wpq.aibaodan.cn

[U39] Py：判断是否在交互环境
来源：http://dff.yfazqb.com

sys.stdout.isatty()
来源：http://qnr.pycfn.com

[U40] Py：打印到标准错误
来源：http://chr.yfazqb.com

print("err", file=sys.stderr)
来源：http://ger.quarkkingdee.top

[U41] PHP：初始化 Composer 项目
来源：http://odn.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jle.hammf.cn

[U42] PHP：PSR-4 自动加载
来源：http://twi.gaohongyu789.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jzs.jinghuilouyu.cn

[U43] PHP：声明命名空间
来源：http://hue.pycfn.com

namespace App\Http;
来源：http://vbx.jyoumei.cn

[U44] PHP：开启严格类型
来源：http://vwl.smart0.xyz

declare(strict_types=1);
来源：http://uko.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://cqp.yongpay.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nom.c1oappe.top

[U46] PHP：可空类型
来源：http://loc.svipenyu.cn

?string $name = null
来源：http://zhp.sjlbkw.cn

[U47] PHP：联合类型
来源：http://kdq.52xcode.cn

int|string $id
来源：http://mep.yueranfly.top

[U48] PHP：纯枚举
来源：http://dbh.pengpengdd.cyou

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jbq.zdbjq.cn

[U49] PHP：只读属性
来源：http://wdr.hcnkem.com

public readonly string $name
来源：http://ryd.zdbjq.cn

[U50] PHP：构造器属性提升
来源：http://pks.hfpthk.cn

public function __construct(private int $id) {}
来源：http://tfn.jlsjyb.cn

[U51] PHP：数组解构
来源：http://wyf.nanxuanxn.top

[$a, $b] = $arr;
来源：http://wqm.wangdashe.top

[U52] PHP：箭头函数
来源：http://inu.zhaomingkeji.xyz

$double = fn($x) => $x * 2;
来源：http://uaf.kuanghao11.cn

[U53] PHP：空合并运算符
来源：http://jfk.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://nzo.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://kwe.nanxuanxn.top

$obj?->method()
来源：http://fbh.c1oappe.top

[U55] PHP：match 表达式
来源：http://uxf.yangfankeji.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dzc.yfazqb.com

[U56] PHP：命名参数
来源：http://etp.ehwqpu.com

f(a: 1, b: 2)
来源：http://mtj.birdmap.top

[U57] PHP：字符串插值
来源：http://blt.guannengcc.top

"值: {$a}"
来源：http://uaf.cqqwz.cn

[U58] PHP：数组三件套
来源：http://clo.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jem.fktsv.cn

[U59] PHP：自定义排序
来源：http://buj.xuanzx.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://njz.gaohongyu789.top

[U60] PHP：JSON 编解码
来源：http://uyk.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fif.0kj1m.cn

[U61] PHP：正则
来源：http://mxe.daria6918.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qil.sxryk.cn

[U62] PHP：日期对象
来源：http://kze.chenzaomai.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://unj.fzhhl.top

[U63] PHP：文件读写
来源：http://oyv.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ppp.xuetiantiany.cn

[U64] PHP：目录遍历
来源：http://vzj.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://czg.ctjpmb.com

[U65] PHP：会话
来源：http://duj.xuetiantiany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://olw.ivvv.top

[U66] PHP：设置 Cookie
来源：http://ywq.meibo888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zdj.sysykeji.top

[U67] PHP：处理文件上传
来源：http://dbn.xziqi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wdu.hysaishi.cn

[U68] PHP：PDO 连接
来源：http://qkv.pengpengdd.cyou

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ibm.kuanghao11.cn

[U69] PHP：PDO 预处理
来源：http://auc.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://twn.fehbvm.com

[U70] PHP：PDO 事务
来源：http://nro.yvedp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dpr.yvedp.cn

[U71] PHP：抛出异常
来源：http://gtf.dashuyun.cn

throw new RuntimeException("失败", 500);
来源：http://xlx.shuidangran.top

[U72] PHP：写错误日志
来源：http://ikc.fanxiaobao.xyz

error_log("失败: " . $e->getMessage());
来源：http://lkj.yangfankeji.com

[U73] PHP：读取 ini 配置
来源：http://way.ivvv.top

parse_ini_file("config.ini", true)
来源：http://mja.jinqigufen.top

[U74] PHP：读取环境变量
来源：http://vwn.yvedp.cn

getenv("APP_ENV") ?: "production"
来源：http://rxf.yanxiufei.cn

[U75] PHP：依赖注入
来源：http://dsu.quarkkingdee.top

composer require psr/container
来源：http://vuv.shzxlz.cn

[U76] PHP：简单路由
来源：http://yxx.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://glm.epnwcf.com

[U77] PHP：模板渲染
来源：http://urs.hammf.cn

composer require twig/twig
来源：http://ztc.cucudq.cn

[U78] PHP：单元测试
来源：http://rzs.jlsjyb.cn

composer require --dev phpunit/phpunit
来源：http://kqf.shangyingyoupin.top

[U79] PHP：静态分析
来源：http://bmw.ydjk.org.cn

composer require --dev phpstan/phpstan
来源：http://zux.yuanzhike.top

[U80] PHP：代码规范修复
来源：http://cis.aizwys.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sqh.xuanzx.com

[U81] JS：初始化项目
来源：http://emv.zdqjudy.top

npm init -y;  npm i express
来源：http://oqc.chenlongwang.top

[U82] JS：package.json 脚本
来源：http://oig.hongshengwenyu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gtt.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://fem.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://mge.shanyushiyangkeji.top

[U84] JS：CommonJS 写法
来源：http://bhz.smart0.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://uvx.ydjk.org.cn

[U85] JS：可选链
来源：http://dzr.vqdsnc.cn

a?.b?.c
来源：http://wsd.meibo888.top

[U86] JS：空值合并
来源：http://eow.wangdashe.top

a ?? b
来源：http://ckb.hnxiangtu.top


<!-- 参考信息 -->