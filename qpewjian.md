代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://ehd.uphjek.com

[S59] C++：静态断言
来源：http://mku.birdmap.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://voq.sweek.top

[S60] C++：遍历并删除元素
来源：http://rfc.zhongyouzk.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bwu.redwolf501.top

================================================================================
来源：http://ewv.svipenyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://olc.bjfxy.top

================================================================================
来源：http://sae.vqdsnc.cn

[T01] Kotlin：Hello World
来源：http://zpu.yongpay.top

println("Hello")
来源：http://zba.yonumen.top

[T02] Kotlin：变量
来源：http://hxs.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hto.hnqzz.top

[T03] Kotlin：字符串模板
来源：http://juk.yuxming.cn

"值: $b"
来源：http://jqp.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://glv.meibo888.top

val n: String? = null;  n?.length
来源：http://hvx.havefunace.top

[T05] Kotlin：when 表达式
来源：http://ntq.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zgg.gaohongyu789.top

[T06] Kotlin：集合映射
来源：http://fvf.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://foq.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://veh.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bae.cashguo.top

[T08] Kotlin：数据类
来源：http://pwk.chenjidiqi.icu

data class User(val name: String, val age: Int)
来源：http://arh.hongshengwenyu.top

[T09] Kotlin：扩展函数
来源：http://nnv.aibaodan.cn

fun String.exclaim() = this + "!"
来源：http://kpp.ybcxt.top

[T10] Kotlin：默认参数
来源：http://crn.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tlu.fktsv.cn

[T11] Kotlin：协程
来源：http://mbf.meibo888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bqx.xinyue.icu

[T12] Kotlin：解构声明
来源：http://kop.bbcook.cn

val (a, b) = Pair(1, 2)
来源：http://rvs.ydzc1.top

[T13] Kotlin：只读 Map
来源：http://xmp.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://xta.birdmap.top

[T14] Kotlin：循环
来源：http://tfr.gotoacloud.top

for (i in 1..10) println(i)
来源：http://tlz.yfazqb.com

[T15] Kotlin：接口
来源：http://xmz.gotoacloud.top

interface Shape { fun area(): Double }
来源：http://zzd.yonumen.top

[T16] Swift：Hello World
来源：http://lwb.jinqigufen.top

print("Hello")
来源：http://dvc.jianghu66.top

[T17] Swift：变量与常量
来源：http://wky.aizwys.cn

var a = 1;  let b = 2
来源：http://byb.iojbl.cn

[T18] Swift：字符串插值
来源：http://jlz.haohaochexian.top

"值: \(b)"
来源：http://xbr.bbcook.cn

[T19] Swift：可选绑定
来源：http://pqw.xziqi.cn

if let n = opt { print(n) }
来源：http://ptg.jiagoushi.top

[T20] Swift：数组操作
来源：http://kri.feifeiyinyue.top

var a = [1, 2, 3];  a.append(4)
来源：http://yei.fengsongda.top

[T21] Swift：遍历
来源：http://bgf.sxryk.cn

for x in a { print(x) }
来源：http://zol.ivvv.top

[T22] Swift：字典
来源：http://neq.havefunace.top

var d = ["a": 1];  d["b"] = 2
来源：http://gbt.xuanzx.com

[T23] Swift：函数
来源：http://dnd.wangshuangyany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ced.jianghu66.top

[T24] Swift：闭包
来源：http://ezk.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://abs.cucudq.cn

[T25] Swift：结构体
来源：http://irb.316326.xyz

struct P { var x: Int }
来源：http://urm.shanyushiyangkeji.top

[T26] Swift：类与重写
来源：http://tgd.uphjek.com

class A: Base { override func f() {} }
来源：http://uks.snrcjt.cn

[T27] Swift：错误处理
来源：http://acn.fzhhl.top

do { try f() } catch { print(error) }
来源：http://hlk.0kj1m.cn

[T28] Swift：枚举
来源：http://dep.daria6918.cn

enum Color { case red, green }
来源：http://qtj.snrcjt.cn

[T29] Swift：guard 提前返回
来源：http://yri.ehwqpu.com

guard let x = opt else { return }
来源：http://eyj.smart0.xyz

[T30] Swift：协议
来源：http://xli.sysykeji.top

protocol Shape { func area() -> Double }
来源：http://zwr.guowangkeji.top

[T31] Lua：Hello World
来源：http://ecw.sxryk.cn

print("Hello")
来源：http://hoj.ydjk.org.cn

[T32] Lua：局部变量
来源：http://ixp.svipenyu.cn

local a = 1
来源：http://vkw.guannengcc.top

[T33] Lua：表（数组）
来源：http://trh.zhoulong.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://mwo.hcnkem.com

[T34] Lua：遍历表
来源：http://hww.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://noo.sufxvd.cn

[T35] Lua：字典表
来源：http://rsd.ydzc1.top

local d = { a = 1 };  d.b = 2
来源：http://oiu.xuetiantiany.cn

[T36] Lua：函数
来源：http://sea.tarul.cn

function add(a, b) return a + b end
来源：http://kfj.guannengcc.top

[T37] Lua：字符串拼接
来源：http://xet.jlsjyb.cn

"a" .. "b"
来源：http://yrn.gotoacloud.top

[T38] Lua：条件
来源：http://eyp.mhx1999.top

if x > 0 then print("正") end
来源：http://inj.zhongyouzk.top

[T39] Lua：模式匹配
来源：http://zep.yj20258.top

string.find(s, "%d+")
来源：http://ehv.guowangkeji.top

[T40] Lua：元表
来源：http://vge.guannengcc.top

setmetatable({}, { __index = base })
来源：http://gut.zhongyouzk.top

[T41] Perl：Hello World
来源：http://pwi.jlsjyb.cn

print "Hello\n";
来源：http://dar.wangshuangyany.cn

[T42] Perl：变量类型
来源：http://rog.gotoacloud.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zdm.hysaishi.cn

[T43] Perl：字符串插值
来源：http://ota.cdnleiting.top

"值: $a"
来源：http://ipk.dianchejie.cn

[T44] Perl：条件
来源：http://esq.sxryk.cn

if ($a > 0) { print "正"; }
来源：http://ook.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://enn.kuanghao11.cn

for my $x (@arr) { print $x; }
来源：http://mdm.hfpthk.cn

[T46] Perl：哈希操作
来源：http://ouo.gogol.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rdp.jinqigufen.top

[T47] Perl：正则捕获
来源：http://dwp.aibaodan.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://foc.cheryme.top

[T48] Perl：正则替换
来源：http://xgg.yvedp.cn

$s =~ s/old/new/g;
来源：http://hpm.dianchejie.cn

[T49] Perl：函数
来源：http://qky.hfpthk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://axu.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://ujk.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ijl.zycfv.cn

while (my $line = <$fh>) { print $line; }
来源：http://buw.c1oappe.top

[T51] Scala：Hello World
来源：http://yop.hongshengwenyu.top

println("Hello")
来源：http://pzc.ivvv.top

[T52] Scala：变量
来源：http://gwi.fengsongda.top

val a = 1;  var b = 2
来源：http://pwz.yfazqb.com

[T53] Scala：字符串插值
来源：http://mqm.hysaishi.cn

s"值: $b"
来源：http://ggw.hammf.cn

[T54] Scala：集合映射
来源：http://cre.dashuyun.cn

List(1, 2, 3).map(_ * 2)
来源：http://gqj.yj202588.top

[T55] Scala：集合过滤
来源：http://nbw.meibo888.top

List(1, 2, 3).filter(_ > 1)
来源：http://jjh.hywenlv.cn

[T56] Scala：样例类
来源：http://uro.ybcxt.top

case class User(name: String, age: Int)
来源：http://nen.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://awj.xuetiantiany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://srp.ybcxt.top

[T58] Scala：函数定义
来源：http://sca.fzhhl.top

def add(a: Int, b: Int): Int = a + b
来源：http://bnb.epnwcf.com

[T59] Scala：循环
来源：http://xsz.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://del.hesvh.cn

[T60] Scala：折叠
来源：http://sca.dashuyun.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mzv.tarul.cn

================================================================================
来源：http://xkd.shzxlz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rrz.hcnkem.com

================================================================================
来源：http://amo.svipenyu.cn

[U01] Py：创建虚拟环境
来源：http://mcv.shuidangran.top

python -m venv .venv && source .venv/bin/activate
来源：http://imn.yfazqb.com

[U02] Py：导出 / 安装依赖
来源：http://tkc.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sza.chenjidiqi.icu

[U03] Py：加载 .env 配置
来源：http://rhf.jlsjyb.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://stz.zhongyouzk.top

[U04] Py：变量调试打印
来源：http://fik.tianlin.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ouw.tianlin.xyz

[U05] Py：列表去重且保序
来源：http://aho.fzhhl.top

list(dict.fromkeys(arr))
来源：http://fzl.fehbvm.com

[U06] Py：合并两个字典
来源：http://vyv.mhx1999.top

{**a, **b}
来源：http://ljj.tarul.cn

[U07] Py：反转字典键值
来源：http://bcj.zycfv.cn

{v: k for k, v in d.items()}
来源：http://tij.cdnleiting.top

[U08] Py：展平二维列表
来源：http://hrw.tian-w.cn

[y for x in nested for y in x]
来源：http://vpt.xinyue.icu

[U09] Py：字典取最大值的键
来源：http://pcl.sysykeji.top

max(d, key=d.get)
来源：http://ofy.nanxuanxn.top

[U10] Py：按值排序字典
来源：http://lxs.zhoulong.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uhu.shzxlz.cn

[U11] Py：生成器表达式
来源：http://gel.sufxvd.cn

(x * 2 for x in arr)
来源：http://uvw.hnxiangtu.top

[U12] Py：取出现最多的 3 个元素
来源：http://wyj.tarul.cn

Counter(arr).most_common(3)
来源：http://vuv.jqgufenzy.top

[U13] Py：固定长度队列
来源：http://hmc.chenzaomai.com

deque(maxlen=10)
来源：http://eni.yj20258.top

[U14] Py：分组收集到列表
来源：http://pxb.gogol.net.cn

defaultdict(list)
来源：http://wyp.tarul.cn

[U15] Py：高精度计时
来源：http://dzo.svipenyu.cn

t = time.perf_counter()
来源：http://frm.zhongyouzk.top

[U16] Py：命令行参数解析
来源：http://kjq.yanxiufei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vof.c1oappe.top

[U17] Py：初始化日志
来源：http://eom.yuxming.cn

logging.basicConfig(level=logging.INFO)
来源：http://umn.gaohongyu789.top

[U18] Py：预编译正则
来源：http://ulp.tianlin.xyz

pat = re.compile(r"\d+")
来源：http://cub.zhengqikj.top

[U19] Py：正则替换带回调
来源：http://cyt.jinyuanbaomall.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zdh.sweek.top

[U20] Py：缓存函数结果
来源：http://uha.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://hdw.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://ukz.cucudq.cn

@contextlib.contextmanager
来源：http://tlb.svipenyu.cn

[U22] Py：矩阵转置
来源：http://vsq.yuanzhike.top

list(zip(*m))
来源：http://bio.gzhubu.top

[U23] Py：分块读取大文件
来源：http://uwe.mhx1999.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kbb.shangyingyoupin.top

[U24] Py：路径操作
来源：http://anj.dianchejie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pdr.epnwcf.com

[U25] Py：CSV 按字典读
来源：http://btm.redwolf501.top

csv.DictReader(f)
来源：http://nbs.ydzc1.top

[U26] Py：并发下载
来源：http://mkc.ivvv.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zbp.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://bxa.hywenlv.cn

aiohttp.ClientSession() 配合 async with
来源：http://yaj.yfazqb.com

[U28] Py：类型别名
来源：http://vjc.redwolf501.top

UserId = int
来源：http://rym.jiagoushi.top

[U29] Py：属性校验
来源：http://idp.smart0.xyz

@property 与 @x.setter 配合
来源：http://fgc.hesvh.cn

[U30] Py：数据类
来源：http://flr.jiagoushi.top

@dataclass(slots=True)
来源：http://wdz.ybcxt.top

[U31] Py：单测
来源：http://vkc.yanxiufei.cn

python -m pytest -q
来源：http://acp.ybcxt.top

[U32] Py：代码格式化
来源：http://fgj.iojbl.cn

ruff format . && ruff check --fix .
来源：http://ceq.dashuyun.cn

[U33] Py：打包发布
来源：http://sxy.zhengqikj.top

python -m build  （依赖 pyproject.toml）
来源：http://wgy.316326.xyz

[U34] Py：判断编码
来源：http://qqb.yanxiufei.cn

chardet.detect(raw)
来源：http://ili.iojbl.cn

[U35] Py：发送邮件
来源：http://gqf.yuanzhike.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dwb.ppjwa.cn

[U36] Py：定时任务
来源：http://iim.hnqzz.top

schedule.every(10).minutes.do(job)
来源：http://hoh.zdbjq.cn

[U37] Py：读写 Excel
来源：http://ouj.nanxuanxn.top

pandas.read_excel / DataFrame.to_excel
来源：http://lsr.9152youxi.cn

[U38] Py：获取脚本所在目录
来源：http://xpe.hesvh.cn

Path(__file__).resolve().parent
来源：http://nqw.epnwcf.com

[U39] Py：判断是否在交互环境
来源：http://ihk.cdnleiting.top

sys.stdout.isatty()
来源：http://dfm.sjlbkw.cn

[U40] Py：打印到标准错误
来源：http://sfy.tanke756.top

print("err", file=sys.stderr)
来源：http://zek.yanxiufei.cn

[U41] PHP：初始化 Composer 项目
来源：http://ryw.tanke756.top

composer init;  composer require guzzlehttp/guzzle
来源：http://duy.dianchejie.cn

[U42] PHP：PSR-4 自动加载
来源：http://cci.ctjpmb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mpb.hnxiangtu.top

[U43] PHP：声明命名空间
来源：http://ykx.shuidangran.top

namespace App\Http;
来源：http://lnd.fehbvm.com

[U44] PHP：开启严格类型
来源：http://ril.jqgufenzy.top

declare(strict_types=1);
来源：http://rfd.c1oappe.top

[U45] PHP：类型声明与返回类型
来源：http://lcz.yonumen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gbm.yuxming.cn

[U46] PHP：可空类型
来源：http://ams.fengsongda.top

?string $name = null
来源：http://xlf.chenlongwang.top

[U47] PHP：联合类型
来源：http://qvv.ybcxt.top

int|string $id
来源：http://mec.yvedp.cn

[U48] PHP：纯枚举
来源：http://hgl.shzxlz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rfj.kuanghao11.cn

[U49] PHP：只读属性
来源：http://fdt.bbcook.cn

public readonly string $name
来源：http://rrx.hesvh.cn

[U50] PHP：构造器属性提升
来源：http://pub.yueranfly.top

public function __construct(private int $id) {}
来源：http://fcr.yuanzhike.top

[U51] PHP：数组解构
来源：http://qvh.yuxming.cn

[$a, $b] = $arr;
来源：http://vei.ydzc1.top

[U52] PHP：箭头函数
来源：http://nrn.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://lfh.yangfankeji.com

[U53] PHP：空合并运算符
来源：http://qce.52xcode.cn

$v = $a ?? $b ?? "default";
来源：http://hgo.ybcxt.top

[U54] PHP：空安全调用
来源：http://vrs.sjlbkw.cn

$obj?->method()
来源：http://zzk.smart0.xyz

[U55] PHP：match 表达式
来源：http://ito.chenzaomai.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nsk.jianghu66.top

[U56] PHP：命名参数
来源：http://bgr.hnqzz.top

f(a: 1, b: 2)
来源：http://soz.jyoumei.cn

[U57] PHP：字符串插值
来源：http://dye.hnxiangtu.top

"值: {$a}"
来源：http://qvb.jqgfzy.top

[U58] PHP：数组三件套
来源：http://nyj.uphjek.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://opm.wangdashe.top

[U59] PHP：自定义排序
来源：http://uyq.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eqs.smart0.xyz

[U60] PHP：JSON 编解码
来源：http://gjk.hesvh.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aqu.epnwcf.com

[U61] PHP：正则
来源：http://bei.cashguo.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://twn.wangshuangyany.cn

[U62] PHP：日期对象
来源：http://mek.epnwcf.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vas.gogol.net.cn

[U63] PHP：文件读写
来源：http://gbt.gogol.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xvr.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://kgc.yvedp.cn

glob("dir/*.php");  scandir("dir");
来源：http://ypr.vehdjk.com

[U65] PHP：会话
来源：http://gfm.iojbl.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yrz.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://tsm.shzxlz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oww.hnqzz.top

[U67] PHP：处理文件上传
来源：http://pjb.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bim.shuidangran.top

[U68] PHP：PDO 连接
来源：http://jjg.hcnkem.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://upe.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://uen.fktsv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://icp.epnwcf.com

[U70] PHP：PDO 事务
来源：http://bxy.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://boc.tanke756.top

[U71] PHP：抛出异常
来源：http://plx.tian-w.cn

throw new RuntimeException("失败", 500);
来源：http://mjv.sxryk.cn

[U72] PHP：写错误日志
来源：http://irr.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://wlb.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://mnu.zhongyouzk.top

parse_ini_file("config.ini", true)
来源：http://rap.yj20258.top

[U74] PHP：读取环境变量
来源：http://zbc.jiagoushi.top

getenv("APP_ENV") ?: "production"
来源：http://nky.svipenyu.cn

[U75] PHP：依赖注入
来源：http://vlt.ydjk.org.cn

composer require psr/container
来源：http://ghw.cdnleiting.top

[U76] PHP：简单路由
来源：http://alt.jqgufenzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://abj.zhaomingkeji.xyz

[U77] PHP：模板渲染
来源：http://naf.yanxiufei.cn

composer require twig/twig
来源：http://nya.shanyushiyangtech.top

[U78] PHP：单元测试
来源：http://cbs.pycfn.com

composer require --dev phpunit/phpunit
来源：http://tts.jianghu66.top

[U79] PHP：静态分析
来源：http://gle.ydjk.org.cn

composer require --dev phpstan/phpstan
来源：http://qtc.iojbl.cn

[U80] PHP：代码规范修复
来源：http://npx.gzhubu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://utm.fzhhl.top

[U81] JS：初始化项目
来源：http://deh.dashuyun.cn

npm init -y;  npm i express
来源：http://idm.aibaodan.cn

[U82] JS：package.json 脚本
来源：http://uzc.andypj.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://otl.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://gpe.jinyuanbaomall.cn

export const a = 1;  import { a } from "./m.js";
来源：http://glx.sjlbkw.cn

[U84] JS：CommonJS 写法
来源：http://qpa.yuxming.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qov.cucudq.cn


<!-- 参考信息 -->