代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://qoj.hammf.cn

[S59] C++：静态断言
来源：http://zzu.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vun.iojbl.cn

[S60] C++：遍历并删除元素
来源：http://nyd.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ede.fktsv.cn

================================================================================
来源：http://eil.yvedp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tqo.ywan-chungtsiang.top

================================================================================
来源：http://jgc.shuidangran.top

[T01] Kotlin：Hello World
来源：http://gzc.shanyushiyangtech.top

println("Hello")
来源：http://inh.daxiang520.top

[T02] Kotlin：变量
来源：http://cyo.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qlf.wangshuangyany.cn

[T03] Kotlin：字符串模板
来源：http://vos.hnxiangtu.top

"值: $b"
来源：http://tkx.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://jbf.cheryme.top

val n: String? = null;  n?.length
来源：http://dce.snrcjt.cn

[T05] Kotlin：when 表达式
来源：http://hym.yonumen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://juo.bbcook.cn

[T06] Kotlin：集合映射
来源：http://yhs.haohaochexian.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wyf.zhaomingkeji.xyz

[T07] Kotlin：集合过滤
来源：http://xax.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cez.zhengqikj.top

[T08] Kotlin：数据类
来源：http://nya.hysaishi.cn

data class User(val name: String, val age: Int)
来源：http://izx.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://uaz.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://qig.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://jra.hesvh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://syd.guannengcc.top

[T11] Kotlin：协程
来源：http://eqj.jinghuilouyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uta.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://rxp.ctjpmb.com

val (a, b) = Pair(1, 2)
来源：http://vrt.yfazqb.com

[T13] Kotlin：只读 Map
来源：http://psw.pycfn.com

val m = mapOf("a" to 1)
来源：http://ofu.zdbjq.cn

[T14] Kotlin：循环
来源：http://etd.0kj1m.cn

for (i in 1..10) println(i)
来源：http://cwb.cucudq.cn

[T15] Kotlin：接口
来源：http://irn.zdbjq.cn

interface Shape { fun area(): Double }
来源：http://qsm.yj20258888.top

[T16] Swift：Hello World
来源：http://mbs.xuanzx.com

print("Hello")
来源：http://jil.tian-w.cn

[T17] Swift：变量与常量
来源：http://yze.smart0.xyz

var a = 1;  let b = 2
来源：http://aqi.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://sbd.cashguo.top

"值: \(b)"
来源：http://gmg.ehwqpu.com

[T19] Swift：可选绑定
来源：http://gnc.zhaomingkeji.xyz

if let n = opt { print(n) }
来源：http://jux.ivvv.top

[T20] Swift：数组操作
来源：http://bba.wangdashe.top

var a = [1, 2, 3];  a.append(4)
来源：http://ker.aizwys.cn

[T21] Swift：遍历
来源：http://xxt.gzhubu.top

for x in a { print(x) }
来源：http://bju.quarkkingdee.top

[T22] Swift：字典
来源：http://qji.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://wgf.epnwcf.com

[T23] Swift：函数
来源：http://rsx.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pqw.zhiwuduotai.top

[T24] Swift：闭包
来源：http://ynm.yj20258.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vgk.shangyingyoupin.top

[T25] Swift：结构体
来源：http://vvj.hcnkem.com

struct P { var x: Int }
来源：http://zoq.shzxlz.cn

[T26] Swift：类与重写
来源：http://vid.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://ayd.xinyue.icu

[T27] Swift：错误处理
来源：http://zql.chenlongwang.top

do { try f() } catch { print(error) }
来源：http://gsd.yonumen.top

[T28] Swift：枚举
来源：http://edh.kuanghao11.cn

enum Color { case red, green }
来源：http://wlj.hongshengwenyu.top

[T29] Swift：guard 提前返回
来源：http://dxk.jyoumei.cn

guard let x = opt else { return }
来源：http://nqk.cucudq.cn

[T30] Swift：协议
来源：http://kaq.ywan-chungtsiang.top

protocol Shape { func area() -> Double }
来源：http://zlt.jqgfzy.top

[T31] Lua：Hello World
来源：http://oxn.chenzaomai.com

print("Hello")
来源：http://qut.xingfuxueyuan.xyz

[T32] Lua：局部变量
来源：http://aus.quarkkingdee.top

local a = 1
来源：http://zzq.jianghu66.top

[T33] Lua：表（数组）
来源：http://evw.yfazqb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://tza.redwolf501.top

[T34] Lua：遍历表
来源：http://ara.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gup.aibaodan.cn

[T35] Lua：字典表
来源：http://vpj.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://lnb.jinghuilouyu.cn

[T36] Lua：函数
来源：http://epf.gotoacloud.top

function add(a, b) return a + b end
来源：http://zvs.yanxiufei.cn

[T37] Lua：字符串拼接
来源：http://wai.hywenlv.cn

"a" .. "b"
来源：http://kez.daria6918.cn

[T38] Lua：条件
来源：http://mkz.wangdashe.top

if x > 0 then print("正") end
来源：http://hlg.pycfn.com

[T39] Lua：模式匹配
来源：http://sxh.xinyue.icu

string.find(s, "%d+")
来源：http://ubd.wangshuangyany.cn

[T40] Lua：元表
来源：http://llj.feifeiyinyue.top

setmetatable({}, { __index = base })
来源：http://mgn.jiagoushi.top

[T41] Perl：Hello World
来源：http://sar.gotoacloud.top

print "Hello\n";
来源：http://svr.sjlbkw.cn

[T42] Perl：变量类型
来源：http://hhh.andypj.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ulz.sxryk.cn

[T43] Perl：字符串插值
来源：http://igo.epnwcf.com

"值: $a"
来源：http://gwg.9152youxi.cn

[T44] Perl：条件
来源：http://prr.tian-w.cn

if ($a > 0) { print "正"; }
来源：http://gri.shzxlz.cn

[T45] Perl：数组遍历
来源：http://bzn.ybcxt.top

for my $x (@arr) { print $x; }
来源：http://zfl.zhaomingkeji.xyz

[T46] Perl：哈希操作
来源：http://ywa.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rra.yj20258888.top

[T47] Perl：正则捕获
来源：http://ckd.xylfe.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tvl.vehdjk.com

[T48] Perl：正则替换
来源：http://arm.ydzc1.top

$s =~ s/old/new/g;
来源：http://zqj.zhoulong.xyz

[T49] Perl：函数
来源：http://ueu.aizwys.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ykf.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://nbl.fehbvm.com

open my $fh, "<", "a.txt" or die $!;
来源：http://xav.vqdsnc.cn

while (my $line = <$fh>) { print $line; }
来源：http://qml.snrcjt.cn

[T51] Scala：Hello World
来源：http://taw.yueranfly.top

println("Hello")
来源：http://mtf.cdnleiting.top

[T52] Scala：变量
来源：http://zll.yfazqb.com

val a = 1;  var b = 2
来源：http://uts.chenlongwang.top

[T53] Scala：字符串插值
来源：http://ajp.52xcode.cn

s"值: $b"
来源：http://lkm.jqgufenzy.top

[T54] Scala：集合映射
来源：http://gwl.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://kgg.snrcjt.cn

[T55] Scala：集合过滤
来源：http://vpm.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://vxz.fengsongda.top

[T56] Scala：样例类
来源：http://nvj.yj20258.top

case class User(name: String, age: Int)
来源：http://gjx.tian-w.cn

[T57] Scala：模式匹配
来源：http://xdn.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://von.fengsongda.top

[T58] Scala：函数定义
来源：http://kyf.zycfv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ecd.bjfxy.top

[T59] Scala：循环
来源：http://enx.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://ysw.daria6918.cn

[T60] Scala：折叠
来源：http://goo.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ium.uphjek.com

================================================================================
来源：http://ckl.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jxa.wangshuangyany.cn

================================================================================
来源：http://hhw.haohaochexian.top

[U01] Py：创建虚拟环境
来源：http://rkx.hesvh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bmc.wangshuangyany.cn

[U02] Py：导出 / 安装依赖
来源：http://fqs.yuanzhike.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rqg.hysaishi.cn

[U03] Py：加载 .env 配置
来源：http://bld.andypj.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://jub.pycfn.com

[U04] Py：变量调试打印
来源：http://jfz.tianlin.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xtj.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://zln.pycfn.com

list(dict.fromkeys(arr))
来源：http://yob.shanyushiyangtech.top

[U06] Py：合并两个字典
来源：http://zdu.shanyushiyangkeji.top

{**a, **b}
来源：http://sdu.shzxlz.cn

[U07] Py：反转字典键值
来源：http://gxd.chenzaomai.com

{v: k for k, v in d.items()}
来源：http://mgc.tanke756.top

[U08] Py：展平二维列表
来源：http://qro.vehdjk.com

[y for x in nested for y in x]
来源：http://ltx.hesvh.cn

[U09] Py：字典取最大值的键
来源：http://aqo.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://elc.chenlongwang.top

[U10] Py：按值排序字典
来源：http://qkg.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://imp.fzhhl.top

[U11] Py：生成器表达式
来源：http://jjk.zycfv.cn

(x * 2 for x in arr)
来源：http://kak.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://dmn.nanxuanxn.top

Counter(arr).most_common(3)
来源：http://ust.ctjpmb.com

[U13] Py：固定长度队列
来源：http://zlo.guowangkeji.top

deque(maxlen=10)
来源：http://pyp.wangdashe.top

[U14] Py：分组收集到列表
来源：http://msg.ivvv.top

defaultdict(list)
来源：http://hhb.hywenlv.cn

[U15] Py：高精度计时
来源：http://zdk.shanyushiyangkeji.top

t = time.perf_counter()
来源：http://pbd.guannengcc.top

[U16] Py：命令行参数解析
来源：http://mpo.tanke756.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aqu.ydjk.org.cn

[U17] Py：初始化日志
来源：http://gta.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://fso.pengpengdd.cyou

[U18] Py：预编译正则
来源：http://xni.sxryk.cn

pat = re.compile(r"\d+")
来源：http://lqe.ppjwa.cn

[U19] Py：正则替换带回调
来源：http://cte.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tfw.yj202588.top

[U20] Py：缓存函数结果
来源：http://woz.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://nlu.yj20258888.top

[U21] Py：自定义上下文管理器
来源：http://wze.jqgfzy.top

@contextlib.contextmanager
来源：http://uii.bjfxy.top

[U22] Py：矩阵转置
来源：http://dfz.tianlin.xyz

list(zip(*m))
来源：http://bai.tarul.cn

[U23] Py：分块读取大文件
来源：http://udg.cdnleiting.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yqo.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://yqs.nwbrower.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gxr.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://jjc.ydjk.org.cn

csv.DictReader(f)
来源：http://icy.guannengcc.top

[U26] Py：并发下载
来源：http://flv.guannengcc.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wck.xinyue.icu

[U27] Py：异步 HTTP
来源：http://apo.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://gew.wangdashe.top

[U28] Py：类型别名
来源：http://hby.tarul.cn

UserId = int
来源：http://xxo.daxiang520.top

[U29] Py：属性校验
来源：http://zcr.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://iyx.hcnkem.com

[U30] Py：数据类
来源：http://ryw.cashguo.top

@dataclass(slots=True)
来源：http://bei.shanyushiyangtech.top

[U31] Py：单测
来源：http://dvz.gogol.net.cn

python -m pytest -q
来源：http://nxj.bbcook.cn

[U32] Py：代码格式化
来源：http://vyp.chenzaomai.com

ruff format . && ruff check --fix .
来源：http://qia.cqqwz.cn

[U33] Py：打包发布
来源：http://loi.fehbvm.com

python -m build  （依赖 pyproject.toml）
来源：http://ufd.zdbjq.cn

[U34] Py：判断编码
来源：http://ndz.xuanzx.com

chardet.detect(raw)
来源：http://wsi.aibaodan.cn

[U35] Py：发送邮件
来源：http://vnf.jinqigufen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lha.ybcxt.top

[U36] Py：定时任务
来源：http://mfs.haohaochexian.top

schedule.every(10).minutes.do(job)
来源：http://vtp.shangyingyoupin.top

[U37] Py：读写 Excel
来源：http://qgy.mhx1999.top

pandas.read_excel / DataFrame.to_excel
来源：http://dmn.zhiwuduotai.top

[U38] Py：获取脚本所在目录
来源：http://rif.cqqwz.cn

Path(__file__).resolve().parent
来源：http://sob.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://rqk.yueranfly.top

sys.stdout.isatty()
来源：http://fxr.xuanzx.com

[U40] Py：打印到标准错误
来源：http://yhr.zhaomingkeji.xyz

print("err", file=sys.stderr)
来源：http://ign.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://xqd.xuanzx.com

composer init;  composer require guzzlehttp/guzzle
来源：http://igq.ctjpmb.com

[U42] PHP：PSR-4 自动加载
来源：http://clf.xinyue.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bzh.pycfn.com

[U43] PHP：声明命名空间
来源：http://aup.0kj1m.cn

namespace App\Http;
来源：http://peo.zhijiandao.cn

[U44] PHP：开启严格类型
来源：http://mlt.nanxinkj.top

declare(strict_types=1);
来源：http://knk.zhoulong.xyz

[U45] PHP：类型声明与返回类型
来源：http://syu.hysaishi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://iyx.ywan-chungtsiang.top

[U46] PHP：可空类型
来源：http://kqn.jinqigufen.top

?string $name = null
来源：http://xyf.hysaishi.cn

[U47] PHP：联合类型
来源：http://njc.xingfuxueyuan.xyz

int|string $id
来源：http://ojs.xingfuxueyuan.xyz

[U48] PHP：纯枚举
来源：http://xrb.xylfe.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zgr.dashuyun.cn

[U49] PHP：只读属性
来源：http://jvh.zhongyouzk.top

public readonly string $name
来源：http://nuc.zhengqikj.top

[U50] PHP：构造器属性提升
来源：http://xmg.xuanzx.com

public function __construct(private int $id) {}
来源：http://epf.ybcxt.top

[U51] PHP：数组解构
来源：http://rvr.shangyingyoupin.top

[$a, $b] = $arr;
来源：http://zlz.meibo888.top

[U52] PHP：箭头函数
来源：http://jdp.hongshengwenyu.top

$double = fn($x) => $x * 2;
来源：http://jrs.zycfv.cn

[U53] PHP：空合并运算符
来源：http://cmz.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://tks.pycfn.com

[U54] PHP：空安全调用
来源：http://uey.hywenlv.cn

$obj?->method()
来源：http://ysc.yj20258888.top

[U55] PHP：match 表达式
来源：http://xmg.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nkj.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://ker.yangfankeji.com

f(a: 1, b: 2)
来源：http://ske.vqdsnc.cn

[U57] PHP：字符串插值
来源：http://tlt.tanke756.top

"值: {$a}"
来源：http://qly.zdbjq.cn

[U58] PHP：数组三件套
来源：http://uqi.ydjk.org.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hwl.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://qma.ehwqpu.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://psp.yj202588.top

[U60] PHP：JSON 编解码
来源：http://ema.52xcode.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iol.hammf.cn

[U61] PHP：正则
来源：http://haz.52xcode.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pin.0kj1m.cn

[U62] PHP：日期对象
来源：http://lju.hfpthk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rwh.chenzaomai.com

[U63] PHP：文件读写
来源：http://pri.zdbjq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zej.sweek.top

[U64] PHP：目录遍历
来源：http://rkk.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://psc.shanyushiyangtech.top

[U65] PHP：会话
来源：http://krp.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://spr.ppjwa.cn

[U66] PHP：设置 Cookie
来源：http://vuj.ppjwa.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xhl.sjlbkw.cn

[U67] PHP：处理文件上传
来源：http://zrt.9152youxi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tbs.yj20258888.top

[U68] PHP：PDO 连接
来源：http://trx.fzhhl.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wlm.hnxiangtu.top

[U69] PHP：PDO 预处理
来源：http://qfv.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yey.aizwys.cn

[U70] PHP：PDO 事务
来源：http://skw.fktsv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uuq.hysaishi.cn

[U71] PHP：抛出异常
来源：http://ehi.dashuyun.cn

throw new RuntimeException("失败", 500);
来源：http://csd.fktsv.cn

[U72] PHP：写错误日志
来源：http://jyb.jinghuilouyu.cn

error_log("失败: " . $e->getMessage());
来源：http://jrr.dashuyun.cn

[U73] PHP：读取 ini 配置
来源：http://sel.9152youxi.cn

parse_ini_file("config.ini", true)
来源：http://jtl.hcnkem.com

[U74] PHP：读取环境变量
来源：http://lbf.shuidangran.top

getenv("APP_ENV") ?: "production"
来源：http://wsx.hysaishi.cn

[U75] PHP：依赖注入
来源：http://irx.jiagoushi.top

composer require psr/container
来源：http://rik.daria6918.cn

[U76] PHP：简单路由
来源：http://ioz.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://toi.sweek.top

[U77] PHP：模板渲染
来源：http://vta.shanyushiyangtech.top

composer require twig/twig
来源：http://phi.chenjidiqi.icu

[U78] PHP：单元测试
来源：http://tiz.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://uhl.hcnkem.com

[U79] PHP：静态分析
来源：http://zyi.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://lcn.cheryme.top

[U80] PHP：代码规范修复
来源：http://lhx.cashguo.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qxg.shuidangran.top

[U81] JS：初始化项目
来源：http://aet.cqqwz.cn

npm init -y;  npm i express
来源：http://sdb.sweek.top

[U82] JS：package.json 脚本
来源：http://eav.ywan-chungtsiang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baf.guowangkeji.top

[U83] JS：ES Module 导入导出
来源：http://pjs.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://kfj.aibaodan.cn

[U84] JS：CommonJS 写法
来源：http://utz.yvedp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dau.zdbjq.cn


<!-- 参考信息 -->