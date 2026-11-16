代发 wailian999

[T05] Kotlin：when 表达式
来源：http://ige.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xhy.zhijiandao.cn

[T06] Kotlin：集合映射
来源：http://lws.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mhi.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://xsy.ybcxt.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://aiw.zdqjudy.top

[T08] Kotlin：数据类
来源：http://cud.yvedp.cn

data class User(val name: String, val age: Int)
来源：http://okh.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://mlp.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://jyx.jinqigfzy.top

[T10] Kotlin：默认参数
来源：http://rjc.guowangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kme.yonumen.top

[T11] Kotlin：协程
来源：http://vwm.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://uqv.mhx1999.top

[T12] Kotlin：解构声明
来源：http://arw.yongpay.top

val (a, b) = Pair(1, 2)
来源：http://wmu.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://fol.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://ggc.bbcook.cn

[T14] Kotlin：循环
来源：http://hul.yj202588.top

for (i in 1..10) println(i)
来源：http://gdg.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://juk.yj20258.top

interface Shape { fun area(): Double }
来源：http://ler.chenjidiqi.icu

[T16] Swift：Hello World
来源：http://oal.ppjwa.cn

print("Hello")
来源：http://uls.hesvh.cn

[T17] Swift：变量与常量
来源：http://zat.c1oappe.top

var a = 1;  let b = 2
来源：http://abn.yj20258.top

[T18] Swift：字符串插值
来源：http://jtj.ydjk.org.cn

"值: \(b)"
来源：http://ypn.zhixingplan.top

[T19] Swift：可选绑定
来源：http://mgl.tarul.cn

if let n = opt { print(n) }
来源：http://mrg.zhoulong.xyz

[T20] Swift：数组操作
来源：http://ulm.zhengqikj.top

var a = [1, 2, 3];  a.append(4)
来源：http://uwv.meibo888.top

[T21] Swift：遍历
来源：http://tal.shanyushiyangtech.top

for x in a { print(x) }
来源：http://tzl.snrcjt.cn

[T22] Swift：字典
来源：http://qre.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://hxa.gotoacloud.top

[T23] Swift：函数
来源：http://phm.gzhubu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rcg.snrcjt.cn

[T24] Swift：闭包
来源：http://joy.aibaodan.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://glp.nwbrower.top

[T25] Swift：结构体
来源：http://qkr.ctjpmb.com

struct P { var x: Int }
来源：http://usq.fengsongda.top

[T26] Swift：类与重写
来源：http://rjx.hnxiangtu.top

class A: Base { override func f() {} }
来源：http://olx.yangfankeji.com

[T27] Swift：错误处理
来源：http://sva.ivvv.top

do { try f() } catch { print(error) }
来源：http://wbt.hesvh.cn

[T28] Swift：枚举
来源：http://lgg.jinqigufen.top

enum Color { case red, green }
来源：http://iig.chenzaomai.com

[T29] Swift：guard 提前返回
来源：http://vch.sweek.top

guard let x = opt else { return }
来源：http://suh.ppjwa.cn

[T30] Swift：协议
来源：http://wwz.hnqzz.top

protocol Shape { func area() -> Double }
来源：http://lzs.zhijiandao.cn

[T31] Lua：Hello World
来源：http://eho.sweek.top

print("Hello")
来源：http://jhb.dianchejie.cn

[T32] Lua：局部变量
来源：http://bif.zhongyouzk.top

local a = 1
来源：http://txn.mhx1999.top

[T33] Lua：表（数组）
来源：http://asc.zhixingplan.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dvi.sxryk.cn

[T34] Lua：遍历表
来源：http://yeq.yvedp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ohq.pycfn.com

[T35] Lua：字典表
来源：http://peq.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://eqg.cashguo.top

[T36] Lua：函数
来源：http://nrj.sxryk.cn

function add(a, b) return a + b end
来源：http://kov.gogol.net.cn

[T37] Lua：字符串拼接
来源：http://gbv.sweek.top

"a" .. "b"
来源：http://qkg.gogol.net.cn

[T38] Lua：条件
来源：http://itb.ybcxt.top

if x > 0 then print("正") end
来源：http://xhe.yfazqb.com

[T39] Lua：模式匹配
来源：http://bxv.zhaomingkeji.xyz

string.find(s, "%d+")
来源：http://kih.chenjidiqi.icu

[T40] Lua：元表
来源：http://bmn.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://mba.cashguo.top

[T41] Perl：Hello World
来源：http://osz.xylfe.cn

print "Hello\n";
来源：http://rwa.redwolf501.top

[T42] Perl：变量类型
来源：http://pnc.bbcook.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nyt.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://yzc.quarkkingdee.top

"值: $a"
来源：http://dbg.chenzaomai.com

[T44] Perl：条件
来源：http://rtl.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://xmt.fktsv.cn

[T45] Perl：数组遍历
来源：http://mhq.hcnkem.com

for my $x (@arr) { print $x; }
来源：http://xon.cdnleiting.top

[T46] Perl：哈希操作
来源：http://acb.zycfv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cjf.xinyue.icu

[T47] Perl：正则捕获
来源：http://snd.tarul.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xam.meibo888.top

[T48] Perl：正则替换
来源：http://niw.iojbl.cn

$s =~ s/old/new/g;
来源：http://mgh.chenlongwang.top

[T49] Perl：函数
来源：http://jzj.tarul.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ghr.bjfxy.top

[T50] Perl：逐行读文件
来源：http://hyn.ivvv.top

open my $fh, "<", "a.txt" or die $!;
来源：http://oxz.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://ssg.jqgfzy.top

[T51] Scala：Hello World
来源：http://iaz.redwolf501.top

println("Hello")
来源：http://pct.ivvv.top

[T52] Scala：变量
来源：http://sku.fehbvm.com

val a = 1;  var b = 2
来源：http://rec.xziqi.cn

[T53] Scala：字符串插值
来源：http://unk.aizwys.cn

s"值: $b"
来源：http://dsw.tarul.cn

[T54] Scala：集合映射
来源：http://cfu.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://acu.xuanzx.com

[T55] Scala：集合过滤
来源：http://oyr.feifeiyinyue.top

List(1, 2, 3).filter(_ > 1)
来源：http://oyi.ybcxt.top

[T56] Scala：样例类
来源：http://eyg.cqqwz.cn

case class User(name: String, age: Int)
来源：http://kfe.shanyushiyangkeji.top

[T57] Scala：模式匹配
来源：http://srd.ybcxt.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nkt.sysykeji.top

[T58] Scala：函数定义
来源：http://ean.hysaishi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://khc.shzxlz.cn

[T59] Scala：循环
来源：http://ogx.guannengcc.top

for (i <- 1 to 10) println(i)
来源：http://lpw.c1oappe.top

[T60] Scala：折叠
来源：http://cpq.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ojq.nanxuanxn.top

================================================================================
来源：http://zoa.birdmap.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sbj.nwbrower.top

================================================================================
来源：http://uoy.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://nlh.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cwn.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://bth.xinyue.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eqp.cashguo.top

[U03] Py：加载 .env 配置
来源：http://lpx.zhongyouzk.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vgv.yangfankeji.com

[U04] Py：变量调试打印
来源：http://wrk.meibo888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eni.jiagoushi.top

[U05] Py：列表去重且保序
来源：http://dkc.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://vmn.yueranfly.top

[U06] Py：合并两个字典
来源：http://upi.vehdjk.com

{**a, **b}
来源：http://dyx.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://zyi.yuxming.cn

{v: k for k, v in d.items()}
来源：http://pyl.52xcode.cn

[U08] Py：展平二维列表
来源：http://zkx.yvedp.cn

[y for x in nested for y in x]
来源：http://gzw.xingfuxueyuan.xyz

[U09] Py：字典取最大值的键
来源：http://osd.xylfe.cn

max(d, key=d.get)
来源：http://tht.zhongyouzk.top

[U10] Py：按值排序字典
来源：http://jcz.tian-w.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gxe.haohaochexian.top

[U11] Py：生成器表达式
来源：http://yvi.aibaodan.cn

(x * 2 for x in arr)
来源：http://him.ybcxt.top

[U12] Py：取出现最多的 3 个元素
来源：http://fkf.mhx1999.top

Counter(arr).most_common(3)
来源：http://qvu.snrcjt.cn

[U13] Py：固定长度队列
来源：http://dxq.zhongyouzk.top

deque(maxlen=10)
来源：http://mku.mhx1999.top

[U14] Py：分组收集到列表
来源：http://gie.yueranfly.top

defaultdict(list)
来源：http://nxg.cucudq.cn

[U15] Py：高精度计时
来源：http://agu.feifeiyinyue.top

t = time.perf_counter()
来源：http://xfl.ywan-chungtsiang.top

[U16] Py：命令行参数解析
来源：http://bwv.daria6918.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xwd.ehwqpu.com

[U17] Py：初始化日志
来源：http://wix.zycfv.cn

logging.basicConfig(level=logging.INFO)
来源：http://iqy.aibaodan.cn

[U18] Py：预编译正则
来源：http://xjs.vqdsnc.cn

pat = re.compile(r"\d+")
来源：http://ghe.nanxinkj.top

[U19] Py：正则替换带回调
来源：http://jpl.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sjv.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://tmw.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://rlg.ybcxt.top

[U21] Py：自定义上下文管理器
来源：http://uij.gzhubu.top

@contextlib.contextmanager
来源：http://grx.ybcxt.top

[U22] Py：矩阵转置
来源：http://fiv.yonumen.top

list(zip(*m))
来源：http://bnp.hammf.cn

[U23] Py：分块读取大文件
来源：http://npu.52xcode.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vli.hnqzz.top

[U24] Py：路径操作
来源：http://ztn.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tuv.meibo888.top

[U25] Py：CSV 按字典读
来源：http://jlu.hysaishi.cn

csv.DictReader(f)
来源：http://uiz.aibaodan.cn

[U26] Py：并发下载
来源：http://aoq.ppjwa.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xop.jianghu66.top

[U27] Py：异步 HTTP
来源：http://fwo.yongpay.top

aiohttp.ClientSession() 配合 async with
来源：http://jtt.sweek.top

[U28] Py：类型别名
来源：http://zgs.guannengcc.top

UserId = int
来源：http://wth.shanyushiyangtech.top

[U29] Py：属性校验
来源：http://ssq.ydzc1.top

@property 与 @x.setter 配合
来源：http://uhw.iojbl.cn

[U30] Py：数据类
来源：http://nsd.nwbrower.top

@dataclass(slots=True)
来源：http://bkc.birdmap.top

[U31] Py：单测
来源：http://vam.316326.xyz

python -m pytest -q
来源：http://uzj.svipenyu.cn

[U32] Py：代码格式化
来源：http://cst.zdbjq.cn

ruff format . && ruff check --fix .
来源：http://hwb.xylfe.cn

[U33] Py：打包发布
来源：http://aos.wangdashe.top

python -m build  （依赖 pyproject.toml）
来源：http://sor.hcnkem.com

[U34] Py：判断编码
来源：http://iwv.ehwqpu.com

chardet.detect(raw)
来源：http://jek.guannengcc.top

[U35] Py：发送邮件
来源：http://lwp.aizwys.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://grr.xingfuxueyuan.xyz

[U36] Py：定时任务
来源：http://tbo.smart0.xyz

schedule.every(10).minutes.do(job)
来源：http://oga.dianchejie.cn

[U37] Py：读写 Excel
来源：http://sdm.zdbjq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zyz.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://jdk.wangdashe.top

Path(__file__).resolve().parent
来源：http://ovx.ywan-chungtsiang.top

[U39] Py：判断是否在交互环境
来源：http://xis.xylfe.cn

sys.stdout.isatty()
来源：http://fpk.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://tfj.gogol.net.cn

print("err", file=sys.stderr)
来源：http://xma.ydjk.org.cn

[U41] PHP：初始化 Composer 项目
来源：http://dlk.havefunace.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qre.hnqzz.top

[U42] PHP：PSR-4 自动加载
来源：http://myj.xziqi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ujy.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://ztz.jyoumei.cn

namespace App\Http;
来源：http://gya.zhiwuduotai.top

[U44] PHP：开启严格类型
来源：http://drt.gaohongyu789.top

declare(strict_types=1);
来源：http://ktf.andypj.xyz

[U45] PHP：类型声明与返回类型
来源：http://tpb.xingfuxueyuan.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://lfs.yvedp.cn

[U46] PHP：可空类型
来源：http://niw.kuanghao11.cn

?string $name = null
来源：http://vdm.jyoumei.cn

[U47] PHP：联合类型
来源：http://fmh.gaohongyu789.top

int|string $id
来源：http://hkc.bjfxy.top

[U48] PHP：纯枚举
来源：http://apf.jlsjyb.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wka.hesvh.cn

[U49] PHP：只读属性
来源：http://vtv.jinghuilouyu.cn

public readonly string $name
来源：http://rjv.bbcook.cn

[U50] PHP：构造器属性提升
来源：http://zql.gaohongyu789.top

public function __construct(private int $id) {}
来源：http://fvv.gzhubu.top

[U51] PHP：数组解构
来源：http://cqo.pengpengdd.cyou

[$a, $b] = $arr;
来源：http://yuo.bbcook.cn

[U52] PHP：箭头函数
来源：http://uij.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://eno.sxryk.cn

[U53] PHP：空合并运算符
来源：http://oas.hongshengwenyu.top

$v = $a ?? $b ?? "default";
来源：http://hyo.andypj.xyz

[U54] PHP：空安全调用
来源：http://acp.nwbrower.top

$obj?->method()
来源：http://ebd.hysaishi.cn

[U55] PHP：match 表达式
来源：http://hdi.havefunace.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jbm.hysaishi.cn

[U56] PHP：命名参数
来源：http://sku.meibo888.top

f(a: 1, b: 2)
来源：http://vcw.haohaochexian.top

[U57] PHP：字符串插值
来源：http://hbc.snrcjt.cn

"值: {$a}"
来源：http://xhp.c1oappe.top

[U58] PHP：数组三件套
来源：http://ywc.cqqwz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yla.ybcxt.top

[U59] PHP：自定义排序
来源：http://aur.cqqwz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ciy.hammf.cn

[U60] PHP：JSON 编解码
来源：http://mmw.zhiwuduotai.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bed.yj202588.top

[U61] PHP：正则
来源：http://oap.nanxinkj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lhb.xziqi.cn

[U62] PHP：日期对象
来源：http://gll.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://git.hammf.cn

[U63] PHP：文件读写
来源：http://xpy.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gxc.chenlongwang.top

[U64] PHP：目录遍历
来源：http://ply.snrcjt.cn

glob("dir/*.php");  scandir("dir");
来源：http://qpu.birdmap.top

[U65] PHP：会话
来源：http://oyc.xylfe.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jsz.yonumen.top

[U66] PHP：设置 Cookie
来源：http://lqa.redwolf501.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ajl.mhx1999.top

[U67] PHP：处理文件上传
来源：http://oya.chenlongwang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://equ.zdbjq.cn

[U68] PHP：PDO 连接
来源：http://vik.tanke756.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ydx.pycfn.com

[U69] PHP：PDO 预处理
来源：http://bum.snrcjt.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zaa.yueranfly.top

[U70] PHP：PDO 事务
来源：http://wjx.jinyuanbaomall.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oel.daria6918.cn

[U71] PHP：抛出异常
来源：http://lad.nwbrower.top

throw new RuntimeException("失败", 500);
来源：http://ycx.jinghuilouyu.cn

[U72] PHP：写错误日志
来源：http://fdl.tianlin.xyz

error_log("失败: " . $e->getMessage());
来源：http://ncn.fehbvm.com

[U73] PHP：读取 ini 配置
来源：http://zvh.jyoumei.cn

parse_ini_file("config.ini", true)
来源：http://ljb.hesvh.cn

[U74] PHP：读取环境变量
来源：http://gpo.yonumen.top

getenv("APP_ENV") ?: "production"
来源：http://wpn.hfpthk.cn

[U75] PHP：依赖注入
来源：http://nxn.ywan-chungtsiang.top

composer require psr/container
来源：http://bur.hesvh.cn

[U76] PHP：简单路由
来源：http://ytj.xuetiantiany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ccg.nwbrower.top

[U77] PHP：模板渲染
来源：http://zbq.hywenlv.cn

composer require twig/twig
来源：http://szs.epnwcf.com

[U78] PHP：单元测试
来源：http://npn.ydzc1.top

composer require --dev phpunit/phpunit
来源：http://ojx.fehbvm.com

[U79] PHP：静态分析
来源：http://hka.ctjpmb.com

composer require --dev phpstan/phpstan
来源：http://bxe.fehbvm.com

[U80] PHP：代码规范修复
来源：http://vhg.tanke756.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://cpj.chenjidiqi.icu

[U81] JS：初始化项目
来源：http://pnw.zdbjq.cn

npm init -y;  npm i express
来源：http://wfb.shanyushiyangkeji.top

[U82] JS：package.json 脚本
来源：http://nlz.yuxming.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://szi.jqgfzy.top

[U83] JS：ES Module 导入导出
来源：http://rsp.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://muw.smart0.xyz

[U84] JS：CommonJS 写法
来源：http://mcu.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://gzf.mhx1999.top

[U85] JS：可选链
来源：http://zjt.svipenyu.cn

a?.b?.c
来源：http://esq.zhongyouzk.top

[U86] JS：空值合并
来源：http://syf.wangdashe.top

a ?? b
来源：http://ilm.cucudq.cn

[U87] JS：解构默认值
来源：http://aml.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://tgo.jianghu66.top

[U88] JS：对象展开合并
来源：http://kzg.hfpthk.cn

{ ...a, ...b }
来源：http://ilb.0kj1m.cn

[U89] JS：数组去重
来源：http://rxq.snrcjt.cn

[...new Set(arr)]
来源：http://xcb.jinqigfzy.top

[U90] JS：数字数组排序
来源：http://agp.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://fxq.fzhhl.top

[U91] JS：对象键值遍历
来源：http://wfo.cheryme.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ori.tarul.cn

[U92] JS：深拷贝
来源：http://zqk.0kj1m.cn

structuredClone(obj)
来源：http://ucv.zycfv.cn


<!-- 参考信息 -->