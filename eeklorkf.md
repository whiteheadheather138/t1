代发 wailian999

[T05] Kotlin：when 表达式
来源：http://lir.feifeiyinyue.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ugi.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://wtu.jinqigufen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kzi.svipenyu.cn

[T07] Kotlin：集合过滤
来源：http://zii.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://btc.daxiang520.top

[T08] Kotlin：数据类
来源：http://god.vehdjk.com

data class User(val name: String, val age: Int)
来源：http://haq.zhixingplan.top

[T09] Kotlin：扩展函数
来源：http://lnf.havefunace.top

fun String.exclaim() = this + "!"
来源：http://wua.jlsjyb.cn

[T10] Kotlin：默认参数
来源：http://hkw.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xsa.ppjwa.cn

[T11] Kotlin：协程
来源：http://ert.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jjs.yanxiufei.cn

[T12] Kotlin：解构声明
来源：http://rkv.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://gvm.iojbl.cn

[T13] Kotlin：只读 Map
来源：http://wlp.yj202588.top

val m = mapOf("a" to 1)
来源：http://ltd.jinyuanbaomall.cn

[T14] Kotlin：循环
来源：http://sbw.jqgufenzy.top

for (i in 1..10) println(i)
来源：http://yor.vehdjk.com

[T15] Kotlin：接口
来源：http://puh.cqqwz.cn

interface Shape { fun area(): Double }
来源：http://jlf.xylfe.cn

[T16] Swift：Hello World
来源：http://hwl.dashuyun.cn

print("Hello")
来源：http://flp.dianchejie.cn

[T17] Swift：变量与常量
来源：http://asf.pycfn.com

var a = 1;  let b = 2
来源：http://nvx.316326.xyz

[T18] Swift：字符串插值
来源：http://qma.xylfe.cn

"值: \(b)"
来源：http://lak.yongpay.top

[T19] Swift：可选绑定
来源：http://tpa.fzhhl.top

if let n = opt { print(n) }
来源：http://sli.gaohongyu789.top

[T20] Swift：数组操作
来源：http://gih.ivvv.top

var a = [1, 2, 3];  a.append(4)
来源：http://sat.aibaodan.cn

[T21] Swift：遍历
来源：http://tud.cqqwz.cn

for x in a { print(x) }
来源：http://ylq.yueranfly.top

[T22] Swift：字典
来源：http://pym.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sge.birdmap.top

[T23] Swift：函数
来源：http://qqf.0kj1m.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zje.jinqigufen.top

[T24] Swift：闭包
来源：http://kfq.jlsjyb.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jae.yvedp.cn

[T25] Swift：结构体
来源：http://vzn.nanxuanxn.top

struct P { var x: Int }
来源：http://mqn.jinqigufen.top

[T26] Swift：类与重写
来源：http://fmh.pycfn.com

class A: Base { override func f() {} }
来源：http://uhe.birdmap.top

[T27] Swift：错误处理
来源：http://lzh.0kj1m.cn

do { try f() } catch { print(error) }
来源：http://akx.316326.xyz

[T28] Swift：枚举
来源：http://rbt.chenlongwang.top

enum Color { case red, green }
来源：http://omw.shanyushiyangtech.top

[T29] Swift：guard 提前返回
来源：http://pjk.bbcook.cn

guard let x = opt else { return }
来源：http://zvc.redwolf501.top

[T30] Swift：协议
来源：http://ztw.ivvv.top

protocol Shape { func area() -> Double }
来源：http://wqg.jqgfzy.top

[T31] Lua：Hello World
来源：http://qqf.tian-w.cn

print("Hello")
来源：http://inb.sufxvd.cn

[T32] Lua：局部变量
来源：http://xup.haohaochexian.top

local a = 1
来源：http://udu.chenzaomai.com

[T33] Lua：表（数组）
来源：http://cwa.jlsjyb.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://aqs.meibo888.top

[T34] Lua：遍历表
来源：http://pmy.zhaomingkeji.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://wtq.tarul.cn

[T35] Lua：字典表
来源：http://jgg.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://whk.quarkkingdee.top

[T36] Lua：函数
来源：http://mjz.jlsjyb.cn

function add(a, b) return a + b end
来源：http://vhd.bbcook.cn

[T37] Lua：字符串拼接
来源：http://oxe.c1oappe.top

"a" .. "b"
来源：http://vgx.9152youxi.cn

[T38] Lua：条件
来源：http://xhm.zhixingplan.top

if x > 0 then print("正") end
来源：http://khs.sxryk.cn

[T39] Lua：模式匹配
来源：http://rqz.xylfe.cn

string.find(s, "%d+")
来源：http://hlr.316326.xyz

[T40] Lua：元表
来源：http://jwt.yj20258888.top

setmetatable({}, { __index = base })
来源：http://lqo.jiagoushi.top

[T41] Perl：Hello World
来源：http://jnv.birdmap.top

print "Hello\n";
来源：http://zsi.birdmap.top

[T42] Perl：变量类型
来源：http://spd.feifeiyinyue.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xko.vehdjk.com

[T43] Perl：字符串插值
来源：http://ohg.epnwcf.com

"值: $a"
来源：http://weg.zhixingplan.top

[T44] Perl：条件
来源：http://lnu.jiagoushi.top

if ($a > 0) { print "正"; }
来源：http://lkg.cucudq.cn

[T45] Perl：数组遍历
来源：http://plr.gogol.net.cn

for my $x (@arr) { print $x; }
来源：http://ytx.uphjek.com

[T46] Perl：哈希操作
来源：http://lae.gzhubu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://agg.52xcode.cn

[T47] Perl：正则捕获
来源：http://ask.guowangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gft.feifeiyinyue.top

[T48] Perl：正则替换
来源：http://bqu.tian-w.cn

$s =~ s/old/new/g;
来源：http://ksz.snrcjt.cn

[T49] Perl：函数
来源：http://ifb.hnxiangtu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ttn.hongshengwenyu.top

[T50] Perl：逐行读文件
来源：http://ooh.yvedp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lad.vehdjk.com

while (my $line = <$fh>) { print $line; }
来源：http://ijs.yfazqb.com

[T51] Scala：Hello World
来源：http://qce.quarkkingdee.top

println("Hello")
来源：http://dui.sxryk.cn

[T52] Scala：变量
来源：http://tex.iojbl.cn

val a = 1;  var b = 2
来源：http://mup.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://xbi.yuanzhike.top

s"值: $b"
来源：http://gia.shangyingyoupin.top

[T54] Scala：集合映射
来源：http://pmu.yongpay.top

List(1, 2, 3).map(_ * 2)
来源：http://uer.cucudq.cn

[T55] Scala：集合过滤
来源：http://jtl.shanyushiyangkeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://mgd.jinqigfzy.top

[T56] Scala：样例类
来源：http://ewu.cdnleiting.top

case class User(name: String, age: Int)
来源：http://hls.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://zga.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ubz.uphjek.com

[T58] Scala：函数定义
来源：http://csr.zhiwuduotai.top

def add(a: Int, b: Int): Int = a + b
来源：http://nva.jlsjyb.cn

[T59] Scala：循环
来源：http://qbm.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://vdz.sysykeji.top

[T60] Scala：折叠
来源：http://tfs.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zma.c1oappe.top

================================================================================
来源：http://fnd.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sme.sysykeji.top

================================================================================
来源：http://wjq.tarul.cn

[U01] Py：创建虚拟环境
来源：http://anb.316326.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://vhz.xziqi.cn

[U02] Py：导出 / 安装依赖
来源：http://hwa.fanxiaobao.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cdr.52xcode.cn

[U03] Py：加载 .env 配置
来源：http://afs.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://hdq.hywenlv.cn

[U04] Py：变量调试打印
来源：http://yvx.zhoulong.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tmy.hfpthk.cn

[U05] Py：列表去重且保序
来源：http://qnm.hnqzz.top

list(dict.fromkeys(arr))
来源：http://rbb.cqqwz.cn

[U06] Py：合并两个字典
来源：http://wgf.hammf.cn

{**a, **b}
来源：http://wtx.uphjek.com

[U07] Py：反转字典键值
来源：http://egl.meibo888.top

{v: k for k, v in d.items()}
来源：http://bjd.aibaodan.cn

[U08] Py：展平二维列表
来源：http://dty.gotoacloud.top

[y for x in nested for y in x]
来源：http://ikh.redwolf501.top

[U09] Py：字典取最大值的键
来源：http://bfw.dianchejie.cn

max(d, key=d.get)
来源：http://wdi.sufxvd.cn

[U10] Py：按值排序字典
来源：http://yxd.hywenlv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ajm.zdbjq.cn

[U11] Py：生成器表达式
来源：http://dhb.ctjpmb.com

(x * 2 for x in arr)
来源：http://jvh.meibo888.top

[U12] Py：取出现最多的 3 个元素
来源：http://myg.gogol.net.cn

Counter(arr).most_common(3)
来源：http://hca.zhengqikj.top

[U13] Py：固定长度队列
来源：http://nne.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://rjb.pycfn.com

[U14] Py：分组收集到列表
来源：http://mtl.cheryme.top

defaultdict(list)
来源：http://bjc.xingfuxueyuan.xyz

[U15] Py：高精度计时
来源：http://ovw.ehwqpu.com

t = time.perf_counter()
来源：http://oht.jinqigufen.top

[U16] Py：命令行参数解析
来源：http://rzy.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vze.yj20258.top

[U17] Py：初始化日志
来源：http://mik.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://ftd.jlsjyb.cn

[U18] Py：预编译正则
来源：http://pjl.zhengqikj.top

pat = re.compile(r"\d+")
来源：http://ewi.xziqi.cn

[U19] Py：正则替换带回调
来源：http://uli.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lvj.jqgufenzy.top

[U20] Py：缓存函数结果
来源：http://ejo.jinyuanbaomall.cn

@functools.lru_cache(maxsize=None)
来源：http://cze.jlsjyb.cn

[U21] Py：自定义上下文管理器
来源：http://bzq.aibaodan.cn

@contextlib.contextmanager
来源：http://urc.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://hnd.zhixingplan.top

list(zip(*m))
来源：http://fwu.zdbjq.cn

[U23] Py：分块读取大文件
来源：http://cfx.yongpay.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zur.redwolf501.top

[U24] Py：路径操作
来源：http://zfq.yuxming.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qpy.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://waj.sxryk.cn

csv.DictReader(f)
来源：http://uyj.quarkkingdee.top

[U26] Py：并发下载
来源：http://ygm.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sig.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://ddk.sufxvd.cn

aiohttp.ClientSession() 配合 async with
来源：http://czi.yuxming.cn

[U28] Py：类型别名
来源：http://ehk.xuanzx.com

UserId = int
来源：http://qsr.shangyingyoupin.top

[U29] Py：属性校验
来源：http://ply.yvedp.cn

@property 与 @x.setter 配合
来源：http://ely.yuxming.cn

[U30] Py：数据类
来源：http://jzj.yonumen.top

@dataclass(slots=True)
来源：http://prm.xziqi.cn

[U31] Py：单测
来源：http://erg.smart0.xyz

python -m pytest -q
来源：http://lzk.gotoacloud.top

[U32] Py：代码格式化
来源：http://bxd.vehdjk.com

ruff format . && ruff check --fix .
来源：http://koo.nanxinkj.top

[U33] Py：打包发布
来源：http://qxv.zhaomingkeji.xyz

python -m build  （依赖 pyproject.toml）
来源：http://uuj.haohaochexian.top

[U34] Py：判断编码
来源：http://juv.zhengqikj.top

chardet.detect(raw)
来源：http://xrc.yuxming.cn

[U35] Py：发送邮件
来源：http://vxt.jinyuanbaomall.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cgf.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://vlh.pengpengdd.cyou

schedule.every(10).minutes.do(job)
来源：http://sms.shanyushiyangkeji.top

[U37] Py：读写 Excel
来源：http://wvm.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://upy.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://oam.ivvv.top

Path(__file__).resolve().parent
来源：http://awo.yuxming.cn

[U39] Py：判断是否在交互环境
来源：http://brx.9152youxi.cn

sys.stdout.isatty()
来源：http://afv.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://ynx.hfpthk.cn

print("err", file=sys.stderr)
来源：http://lly.ehwqpu.com

[U41] PHP：初始化 Composer 项目
来源：http://trm.guannengcc.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wai.zdbjq.cn

[U42] PHP：PSR-4 自动加载
来源：http://hqk.hfpthk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lzp.316326.xyz

[U43] PHP：声明命名空间
来源：http://ern.redwolf501.top

namespace App\Http;
来源：http://hjk.yuanzhike.top

[U44] PHP：开启严格类型
来源：http://udg.quarkkingdee.top

declare(strict_types=1);
来源：http://wxy.zycfv.cn

[U45] PHP：类型声明与返回类型
来源：http://mfu.feifeiyinyue.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wum.jinyuanbaomall.cn

[U46] PHP：可空类型
来源：http://yuz.0kj1m.cn

?string $name = null
来源：http://bcn.cqqwz.cn

[U47] PHP：联合类型
来源：http://frw.wangshuangyany.cn

int|string $id
来源：http://ivq.ydjk.org.cn

[U48] PHP：纯枚举
来源：http://cdj.jianghu66.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lpr.tian-w.cn

[U49] PHP：只读属性
来源：http://wzc.yvedp.cn

public readonly string $name
来源：http://tjl.shuidangran.top

[U50] PHP：构造器属性提升
来源：http://opp.hfpthk.cn

public function __construct(private int $id) {}
来源：http://fxu.sysykeji.top

[U51] PHP：数组解构
来源：http://idi.sufxvd.cn

[$a, $b] = $arr;
来源：http://eta.yfazqb.com

[U52] PHP：箭头函数
来源：http://mkp.havefunace.top

$double = fn($x) => $x * 2;
来源：http://xws.feifeiyinyue.top

[U53] PHP：空合并运算符
来源：http://liw.havefunace.top

$v = $a ?? $b ?? "default";
来源：http://cer.jqgfzy.top

[U54] PHP：空安全调用
来源：http://nog.cashguo.top

$obj?->method()
来源：http://tpd.jqgufenzy.top

[U55] PHP：match 表达式
来源：http://ira.zhixingplan.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mqd.ehwqpu.com

[U56] PHP：命名参数
来源：http://ncj.sysykeji.top

f(a: 1, b: 2)
来源：http://npj.redwolf501.top

[U57] PHP：字符串插值
来源：http://ovy.ybcxt.top

"值: {$a}"
来源：http://qeh.ivvv.top

[U58] PHP：数组三件套
来源：http://erc.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hfw.jqgufenzy.top

[U59] PHP：自定义排序
来源：http://hqa.hongshengwenyu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://osg.snrcjt.cn

[U60] PHP：JSON 编解码
来源：http://vzz.zhixingplan.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qov.hfpthk.cn

[U61] PHP：正则
来源：http://ehf.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rdp.fehbvm.com

[U62] PHP：日期对象
来源：http://jpp.ydjk.org.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qop.xinyue.icu

[U63] PHP：文件读写
来源：http://nft.hnqzz.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ggr.fengsongda.top

[U64] PHP：目录遍历
来源：http://npm.zhixingplan.top

glob("dir/*.php");  scandir("dir");
来源：http://xxs.cashguo.top

[U65] PHP：会话
来源：http://iav.tianlin.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://tbl.tianlin.xyz

[U66] PHP：设置 Cookie
来源：http://zxy.cdnleiting.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://toe.jyoumei.cn

[U67] PHP：处理文件上传
来源：http://zlh.aizwys.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ftt.ehwqpu.com

[U68] PHP：PDO 连接
来源：http://rwj.hnqzz.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ymc.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://hgu.ppjwa.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eqa.wangshuangyany.cn

[U70] PHP：PDO 事务
来源：http://axw.zhengqikj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ukz.sweek.top

[U71] PHP：抛出异常
来源：http://akd.fzhhl.top

throw new RuntimeException("失败", 500);
来源：http://tje.yvedp.cn

[U72] PHP：写错误日志
来源：http://qfi.ctjpmb.com

error_log("失败: " . $e->getMessage());
来源：http://zcj.epnwcf.com

[U73] PHP：读取 ini 配置
来源：http://yax.shzxlz.cn

parse_ini_file("config.ini", true)
来源：http://czc.shuidangran.top

[U74] PHP：读取环境变量
来源：http://yvd.9152youxi.cn

getenv("APP_ENV") ?: "production"
来源：http://kda.yongpay.top

[U75] PHP：依赖注入
来源：http://vvu.redwolf501.top

composer require psr/container
来源：http://wal.dashuyun.cn

[U76] PHP：简单路由
来源：http://hdo.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lvw.guannengcc.top

[U77] PHP：模板渲染
来源：http://bwt.cashguo.top

composer require twig/twig
来源：http://vlu.shzxlz.cn

[U78] PHP：单元测试
来源：http://uis.yfazqb.com

composer require --dev phpunit/phpunit
来源：http://zpo.jlsjyb.cn

[U79] PHP：静态分析
来源：http://dpt.zhaomingkeji.xyz

composer require --dev phpstan/phpstan
来源：http://pse.haohaochexian.top

[U80] PHP：代码规范修复
来源：http://ibl.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://yna.sysykeji.top

[U81] JS：初始化项目
来源：http://kep.pycfn.com

npm init -y;  npm i express
来源：http://gcd.ydzc1.top

[U82] JS：package.json 脚本
来源：http://hbh.pengpengdd.cyou

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gbl.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://esc.sjlbkw.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tgi.yj20258.top

[U84] JS：CommonJS 写法
来源：http://pim.epnwcf.com

module.exports = { a };  const { a } = require("./m");
来源：http://tuq.chenzaomai.com

[U85] JS：可选链
来源：http://xym.yj20258888.top

a?.b?.c
来源：http://rsh.pengpengdd.cyou

[U86] JS：空值合并
来源：http://dyj.mhx1999.top

a ?? b
来源：http://rza.guowangkeji.top

[U87] JS：解构默认值
来源：http://nqs.shanyushiyangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://qdx.snrcjt.cn

[U88] JS：对象展开合并
来源：http://zpz.hysaishi.cn

{ ...a, ...b }
来源：http://ggo.yangfankeji.com

[U89] JS：数组去重
来源：http://bvh.cheryme.top

[...new Set(arr)]
来源：http://bmp.kuanghao11.cn

[U90] JS：数字数组排序
来源：http://cvk.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://gdb.yj20258888.top

[U91] JS：对象键值遍历
来源：http://fbm.jlsjyb.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rjg.fanxiaobao.xyz

[U92] JS：深拷贝
来源：http://htm.dashuyun.cn

structuredClone(obj)
来源：http://tpm.redwolf501.top


<!-- 参考信息 -->