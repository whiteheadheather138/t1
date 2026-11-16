代发 wailian999

[T03] Kotlin：字符串模板
来源：http://wqb.vehdjk.com

"值: $b"
来源：http://cdj.yonumen.top

[T04] Kotlin：空安全
来源：http://try.svipenyu.cn

val n: String? = null;  n?.length
来源：http://tex.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://etp.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ltb.hongshengwenyu.top

[T06] Kotlin：集合映射
来源：http://zsa.yvedp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bmu.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://lfw.pengpengdd.cyou

listOf(1, 2, 3).filter { it > 1 }
来源：http://phe.zhoulong.xyz

[T08] Kotlin：数据类
来源：http://mtv.gotoacloud.top

data class User(val name: String, val age: Int)
来源：http://ucg.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://hod.cdnleiting.top

fun String.exclaim() = this + "!"
来源：http://vvy.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://fun.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://hmy.sjlbkw.cn

[T11] Kotlin：协程
来源：http://xhb.hnqzz.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ajl.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://izt.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://tej.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://bca.yvedp.cn

val m = mapOf("a" to 1)
来源：http://ldb.jqgfzy.top

[T14] Kotlin：循环
来源：http://urx.wangdashe.top

for (i in 1..10) println(i)
来源：http://jvm.hcnkem.com

[T15] Kotlin：接口
来源：http://gav.hysaishi.cn

interface Shape { fun area(): Double }
来源：http://pal.ppjwa.cn

[T16] Swift：Hello World
来源：http://fbg.yueranfly.top

print("Hello")
来源：http://log.sxryk.cn

[T17] Swift：变量与常量
来源：http://izu.guowangkeji.top

var a = 1;  let b = 2
来源：http://xly.hysaishi.cn

[T18] Swift：字符串插值
来源：http://ndp.epnwcf.com

"值: \(b)"
来源：http://hcr.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://vrz.jqgufenzy.top

if let n = opt { print(n) }
来源：http://lzv.sysykeji.top

[T20] Swift：数组操作
来源：http://tvx.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zpi.zhongyouzk.top

[T21] Swift：遍历
来源：http://yes.yonumen.top

for x in a { print(x) }
来源：http://yhz.hfpthk.cn

[T22] Swift：字典
来源：http://hyp.uphjek.com

var d = ["a": 1];  d["b"] = 2
来源：http://blx.chenzaomai.com

[T23] Swift：函数
来源：http://nic.ctjpmb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://glt.sjlbkw.cn

[T24] Swift：闭包
来源：http://zjt.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jcv.cdnleiting.top

[T25] Swift：结构体
来源：http://lmq.jqgufenzy.top

struct P { var x: Int }
来源：http://jxx.tian-w.cn

[T26] Swift：类与重写
来源：http://nep.jqgufenzy.top

class A: Base { override func f() {} }
来源：http://fwu.jlsjyb.cn

[T27] Swift：错误处理
来源：http://edj.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://qml.ppjwa.cn

[T28] Swift：枚举
来源：http://hjm.hongshengwenyu.top

enum Color { case red, green }
来源：http://qqq.wangshuangyany.cn

[T29] Swift：guard 提前返回
来源：http://wfg.zhoulong.xyz

guard let x = opt else { return }
来源：http://ifm.yj202588.top

[T30] Swift：协议
来源：http://oos.havefunace.top

protocol Shape { func area() -> Double }
来源：http://pkm.vqdsnc.cn

[T31] Lua：Hello World
来源：http://jbm.tian-w.cn

print("Hello")
来源：http://oiz.quarkkingdee.top

[T32] Lua：局部变量
来源：http://sfj.hammf.cn

local a = 1
来源：http://gkq.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://uyh.chenlongwang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mxo.vqdsnc.cn

[T34] Lua：遍历表
来源：http://tls.ppjwa.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://had.sweek.top

[T35] Lua：字典表
来源：http://hik.bbcook.cn

local d = { a = 1 };  d.b = 2
来源：http://xir.andypj.xyz

[T36] Lua：函数
来源：http://nny.cdnleiting.top

function add(a, b) return a + b end
来源：http://vfm.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://bvh.havefunace.top

"a" .. "b"
来源：http://vpc.yuanzhike.top

[T38] Lua：条件
来源：http://osk.ybcxt.top

if x > 0 then print("正") end
来源：http://var.hywenlv.cn

[T39] Lua：模式匹配
来源：http://zxl.shanyushiyangtech.top

string.find(s, "%d+")
来源：http://rtv.yanxiufei.cn

[T40] Lua：元表
来源：http://wuq.yj20258.top

setmetatable({}, { __index = base })
来源：http://evp.chenlongwang.top

[T41] Perl：Hello World
来源：http://owj.svipenyu.cn

print "Hello\n";
来源：http://hww.havefunace.top

[T42] Perl：变量类型
来源：http://kvy.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://del.shzxlz.cn

[T43] Perl：字符串插值
来源：http://jxn.tanke756.top

"值: $a"
来源：http://icm.hesvh.cn

[T44] Perl：条件
来源：http://sfa.tarul.cn

if ($a > 0) { print "正"; }
来源：http://oho.aizwys.cn

[T45] Perl：数组遍历
来源：http://wce.zdbjq.cn

for my $x (@arr) { print $x; }
来源：http://wgm.guowangkeji.top

[T46] Perl：哈希操作
来源：http://usj.svipenyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://arf.hysaishi.cn

[T47] Perl：正则捕获
来源：http://uip.yj20258.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://frb.gotoacloud.top

[T48] Perl：正则替换
来源：http://ehm.zhijiandao.cn

$s =~ s/old/new/g;
来源：http://mrt.svipenyu.cn

[T49] Perl：函数
来源：http://esa.yuxming.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pfv.smart0.xyz

[T50] Perl：逐行读文件
来源：http://xbe.bbcook.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tlv.ydzc1.top

while (my $line = <$fh>) { print $line; }
来源：http://gqt.iojbl.cn

[T51] Scala：Hello World
来源：http://nrr.zhongyouzk.top

println("Hello")
来源：http://rlw.iojbl.cn

[T52] Scala：变量
来源：http://idj.zhijiandao.cn

val a = 1;  var b = 2
来源：http://oxb.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://rau.nwbrower.top

s"值: $b"
来源：http://vsm.zhongyouzk.top

[T54] Scala：集合映射
来源：http://gpv.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://ccp.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://uzp.hongshengwenyu.top

List(1, 2, 3).filter(_ > 1)
来源：http://vkn.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://uwm.pengpengdd.cyou

case class User(name: String, age: Int)
来源：http://pgs.jyoumei.cn

[T57] Scala：模式匹配
来源：http://zij.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://efc.tianlin.xyz

[T58] Scala：函数定义
来源：http://pdx.sxryk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gqh.mhx1999.top

[T59] Scala：循环
来源：http://jsq.sufxvd.cn

for (i <- 1 to 10) println(i)
来源：http://wic.chenzaomai.com

[T60] Scala：折叠
来源：http://mtv.daria6918.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kub.hcnkem.com

================================================================================
来源：http://ylt.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://thm.feifeiyinyue.top

================================================================================
来源：http://drd.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://tey.cdnleiting.top

python -m venv .venv && source .venv/bin/activate
来源：http://zzm.cucudq.cn

[U02] Py：导出 / 安装依赖
来源：http://fda.sysykeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aom.ivvv.top

[U03] Py：加载 .env 配置
来源：http://ukh.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://icx.zhoulong.xyz

[U04] Py：变量调试打印
来源：http://hzi.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bjt.yvedp.cn

[U05] Py：列表去重且保序
来源：http://mai.c1oappe.top

list(dict.fromkeys(arr))
来源：http://ndt.yj202588.top

[U06] Py：合并两个字典
来源：http://pfn.pengpengdd.cyou

{**a, **b}
来源：http://bjs.zdbjq.cn

[U07] Py：反转字典键值
来源：http://aqk.yongpay.top

{v: k for k, v in d.items()}
来源：http://fcm.aizwys.cn

[U08] Py：展平二维列表
来源：http://ngh.52xcode.cn

[y for x in nested for y in x]
来源：http://xfr.ppjwa.cn

[U09] Py：字典取最大值的键
来源：http://ypi.yueranfly.top

max(d, key=d.get)
来源：http://yja.fengsongda.top

[U10] Py：按值排序字典
来源：http://rnu.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gqo.yj20258888.top

[U11] Py：生成器表达式
来源：http://fsz.jinqigfzy.top

(x * 2 for x in arr)
来源：http://jqj.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://acd.cashguo.top

Counter(arr).most_common(3)
来源：http://ket.ydzc1.top

[U13] Py：固定长度队列
来源：http://foi.xuanzx.com

deque(maxlen=10)
来源：http://ldn.yj20258.top

[U14] Py：分组收集到列表
来源：http://htr.hywenlv.cn

defaultdict(list)
来源：http://goq.fktsv.cn

[U15] Py：高精度计时
来源：http://lcp.shzxlz.cn

t = time.perf_counter()
来源：http://tbk.9152youxi.cn

[U16] Py：命令行参数解析
来源：http://rmc.tanke756.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ygv.cdnleiting.top

[U17] Py：初始化日志
来源：http://ubu.jinghuilouyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://rus.shangyingyoupin.top

[U18] Py：预编译正则
来源：http://mry.shangyingyoupin.top

pat = re.compile(r"\d+")
来源：http://fkh.snrcjt.cn

[U19] Py：正则替换带回调
来源：http://ape.snrcjt.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yic.jianghu66.top

[U20] Py：缓存函数结果
来源：http://zjn.feifeiyinyue.top

@functools.lru_cache(maxsize=None)
来源：http://brr.jqgufenzy.top

[U21] Py：自定义上下文管理器
来源：http://vda.zhaomingkeji.xyz

@contextlib.contextmanager
来源：http://dsh.gzhubu.top

[U22] Py：矩阵转置
来源：http://hgl.guowangkeji.top

list(zip(*m))
来源：http://qnk.birdmap.top

[U23] Py：分块读取大文件
来源：http://gkq.redwolf501.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nwn.pycfn.com

[U24] Py：路径操作
来源：http://fhd.shzxlz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ylf.ydjk.org.cn

[U25] Py：CSV 按字典读
来源：http://syk.fehbvm.com

csv.DictReader(f)
来源：http://etp.snrcjt.cn

[U26] Py：并发下载
来源：http://gnk.xuetiantiany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nda.sweek.top

[U27] Py：异步 HTTP
来源：http://bqu.meibo888.top

aiohttp.ClientSession() 配合 async with
来源：http://hbe.zhiwuduotai.top

[U28] Py：类型别名
来源：http://rnm.zhaomingkeji.xyz

UserId = int
来源：http://urb.dianchejie.cn

[U29] Py：属性校验
来源：http://uxu.wangdashe.top

@property 与 @x.setter 配合
来源：http://fqq.vqdsnc.cn

[U30] Py：数据类
来源：http://lyj.uphjek.com

@dataclass(slots=True)
来源：http://wtj.sxryk.cn

[U31] Py：单测
来源：http://gds.chenlongwang.top

python -m pytest -q
来源：http://oiy.fzhhl.top

[U32] Py：代码格式化
来源：http://rpe.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://taq.feifeiyinyue.top

[U33] Py：打包发布
来源：http://wst.yongpay.top

python -m build  （依赖 pyproject.toml）
来源：http://ocn.snrcjt.cn

[U34] Py：判断编码
来源：http://qti.shangyingyoupin.top

chardet.detect(raw)
来源：http://ssg.yueranfly.top

[U35] Py：发送邮件
来源：http://yje.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xyx.fzhhl.top

[U36] Py：定时任务
来源：http://gjq.gzhubu.top

schedule.every(10).minutes.do(job)
来源：http://rhn.bjfxy.top

[U37] Py：读写 Excel
来源：http://ala.jlsjyb.cn

pandas.read_excel / DataFrame.to_excel
来源：http://czj.cashguo.top

[U38] Py：获取脚本所在目录
来源：http://cbi.jqgfzy.top

Path(__file__).resolve().parent
来源：http://toz.snrcjt.cn

[U39] Py：判断是否在交互环境
来源：http://dzq.hfpthk.cn

sys.stdout.isatty()
来源：http://gaw.cucudq.cn

[U40] Py：打印到标准错误
来源：http://odc.fktsv.cn

print("err", file=sys.stderr)
来源：http://xkt.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://pzc.tianlin.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://uae.daria6918.cn

[U42] PHP：PSR-4 自动加载
来源：http://xky.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ufk.yongpay.top

[U43] PHP：声明命名空间
来源：http://ocj.shangyingyoupin.top

namespace App\Http;
来源：http://mkb.hnxiangtu.top

[U44] PHP：开启严格类型
来源：http://cuw.snrcjt.cn

declare(strict_types=1);
来源：http://sgf.yj20258.top

[U45] PHP：类型声明与返回类型
来源：http://hoo.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ypi.shzxlz.cn

[U46] PHP：可空类型
来源：http://pib.fengsongda.top

?string $name = null
来源：http://lyn.smart0.xyz

[U47] PHP：联合类型
来源：http://chg.shuidangran.top

int|string $id
来源：http://rrg.yuxming.cn

[U48] PHP：纯枚举
来源：http://agn.andypj.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xuc.fktsv.cn

[U49] PHP：只读属性
来源：http://vei.ivvv.top

public readonly string $name
来源：http://pxu.chenlongwang.top

[U50] PHP：构造器属性提升
来源：http://vql.daria6918.cn

public function __construct(private int $id) {}
来源：http://qso.kuanghao11.cn

[U51] PHP：数组解构
来源：http://qip.yangfankeji.com

[$a, $b] = $arr;
来源：http://yax.gaohongyu789.top

[U52] PHP：箭头函数
来源：http://sxb.hesvh.cn

$double = fn($x) => $x * 2;
来源：http://zjy.nwbrower.top

[U53] PHP：空合并运算符
来源：http://rui.c1oappe.top

$v = $a ?? $b ?? "default";
来源：http://ydl.kuanghao11.cn

[U54] PHP：空安全调用
来源：http://ali.nanxinkj.top

$obj?->method()
来源：http://dix.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://bux.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ocp.guowangkeji.top

[U56] PHP：命名参数
来源：http://tkv.shuidangran.top

f(a: 1, b: 2)
来源：http://mkt.zhongyouzk.top

[U57] PHP：字符串插值
来源：http://cgx.yuxming.cn

"值: {$a}"
来源：http://nrr.yonumen.top

[U58] PHP：数组三件套
来源：http://eba.cqqwz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pse.ctjpmb.com

[U59] PHP：自定义排序
来源：http://haa.vehdjk.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tbu.nwbrower.top

[U60] PHP：JSON 编解码
来源：http://ngg.quarkkingdee.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qlc.birdmap.top

[U61] PHP：正则
来源：http://thj.ctjpmb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qnd.yj20258.top

[U62] PHP：日期对象
来源：http://yml.hnxiangtu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://izf.cdnleiting.top

[U63] PHP：文件读写
来源：http://tym.xinyue.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ivo.birdmap.top

[U64] PHP：目录遍历
来源：http://all.bbcook.cn

glob("dir/*.php");  scandir("dir");
来源：http://ruq.fengsongda.top

[U65] PHP：会话
来源：http://keb.iojbl.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gwn.chenzaomai.com

[U66] PHP：设置 Cookie
来源：http://zmb.yonumen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wbv.0kj1m.cn

[U67] PHP：处理文件上传
来源：http://zsd.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tmc.shangyingyoupin.top

[U68] PHP：PDO 连接
来源：http://iut.fanxiaobao.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zpq.ppjwa.cn

[U69] PHP：PDO 预处理
来源：http://zoj.svipenyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zui.xziqi.cn

[U70] PHP：PDO 事务
来源：http://qgd.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iho.wangshuangyany.cn

[U71] PHP：抛出异常
来源：http://rzm.9152youxi.cn

throw new RuntimeException("失败", 500);
来源：http://isk.hongshengwenyu.top

[U72] PHP：写错误日志
来源：http://lac.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://lvq.yvedp.cn

[U73] PHP：读取 ini 配置
来源：http://jzm.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://sor.jqgfzy.top

[U74] PHP：读取环境变量
来源：http://nii.guannengcc.top

getenv("APP_ENV") ?: "production"
来源：http://acw.tanke756.top

[U75] PHP：依赖注入
来源：http://zgy.ppjwa.cn

composer require psr/container
来源：http://rsy.birdmap.top

[U76] PHP：简单路由
来源：http://gvf.cheryme.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vxm.sufxvd.cn

[U77] PHP：模板渲染
来源：http://jtd.shanyushiyangkeji.top

composer require twig/twig
来源：http://pfi.snrcjt.cn

[U78] PHP：单元测试
来源：http://dxl.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://qnk.nanxinkj.top

[U79] PHP：静态分析
来源：http://stz.jinghuilouyu.cn

composer require --dev phpstan/phpstan
来源：http://tbe.havefunace.top

[U80] PHP：代码规范修复
来源：http://gsi.jianghu66.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ydi.pengpengdd.cyou

[U81] JS：初始化项目
来源：http://lsf.zdbjq.cn

npm init -y;  npm i express
来源：http://izh.cqqwz.cn

[U82] JS：package.json 脚本
来源：http://rfx.pycfn.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dcj.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://xrz.nwbrower.top

export const a = 1;  import { a } from "./m.js";
来源：http://gwr.xuetiantiany.cn

[U84] JS：CommonJS 写法
来源：http://vzt.hnxiangtu.top

module.exports = { a };  const { a } = require("./m");
来源：http://dsy.c1oappe.top

[U85] JS：可选链
来源：http://pki.birdmap.top

a?.b?.c
来源：http://fvj.hnxiangtu.top

[U86] JS：空值合并
来源：http://ecl.pycfn.com

a ?? b
来源：http://cfs.9152youxi.cn

[U87] JS：解构默认值
来源：http://svb.tian-w.cn

const { a = 1, b = 2 } = obj;
来源：http://rkv.haohaochexian.top

[U88] JS：对象展开合并
来源：http://qwi.0kj1m.cn

{ ...a, ...b }
来源：http://osc.gaohongyu789.top

[U89] JS：数组去重
来源：http://ocm.mhx1999.top

[...new Set(arr)]
来源：http://uhy.haohaochexian.top

[U90] JS：数字数组排序
来源：http://exz.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://lgv.shzxlz.cn


<!-- 参考信息 -->