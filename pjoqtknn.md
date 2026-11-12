代发 wailian999

[T05] Kotlin：when 表达式
来源：http://afk.aibaodan.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://seu.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://xfg.birdmap.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sks.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://btq.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ndb.iojbl.cn

[T08] Kotlin：数据类
来源：http://agy.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://znn.xuanzx.com

[T09] Kotlin：扩展函数
来源：http://kyt.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://mbh.zhoulong.xyz

[T10] Kotlin：默认参数
来源：http://lwe.jiagoushi.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rsj.52xcode.cn

[T11] Kotlin：协程
来源：http://edb.sjlbkw.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://teg.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://hjd.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://rwj.guowangkeji.top

[T13] Kotlin：只读 Map
来源：http://kjv.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://tlw.epnwcf.com

[T14] Kotlin：循环
来源：http://xzz.uphjek.com

for (i in 1..10) println(i)
来源：http://rrq.andypj.xyz

[T15] Kotlin：接口
来源：http://ghd.ppjwa.cn

interface Shape { fun area(): Double }
来源：http://esi.chenlongwang.top

[T16] Swift：Hello World
来源：http://jle.guowangkeji.top

print("Hello")
来源：http://fau.mhx1999.top

[T17] Swift：变量与常量
来源：http://lwz.sysykeji.top

var a = 1;  let b = 2
来源：http://tib.uphjek.com

[T18] Swift：字符串插值
来源：http://mwp.gzhubu.top

"值: \(b)"
来源：http://pls.tarul.cn

[T19] Swift：可选绑定
来源：http://dah.sxryk.cn

if let n = opt { print(n) }
来源：http://wfi.jlsjyb.cn

[T20] Swift：数组操作
来源：http://shn.fehbvm.com

var a = [1, 2, 3];  a.append(4)
来源：http://isl.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://xdo.sjlbkw.cn

for x in a { print(x) }
来源：http://rmv.tianlin.xyz

[T22] Swift：字典
来源：http://zro.xuanzx.com

var d = ["a": 1];  d["b"] = 2
来源：http://hln.feifeiyinyue.top

[T23] Swift：函数
来源：http://yki.52xcode.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bqa.yuanzhike.top

[T24] Swift：闭包
来源：http://ybv.yonumen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://aod.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://wcc.chenlongwang.top

struct P { var x: Int }
来源：http://kib.nanxinkj.top

[T26] Swift：类与重写
来源：http://iae.yj20258.top

class A: Base { override func f() {} }
来源：http://gjv.tian-w.cn

[T27] Swift：错误处理
来源：http://kau.yongpay.top

do { try f() } catch { print(error) }
来源：http://ydf.gogol.net.cn

[T28] Swift：枚举
来源：http://tai.gzhubu.top

enum Color { case red, green }
来源：http://gmj.jinghuilouyu.cn

[T29] Swift：guard 提前返回
来源：http://num.hesvh.cn

guard let x = opt else { return }
来源：http://yjp.aibaodan.cn

[T30] Swift：协议
来源：http://wrr.zhoulong.xyz

protocol Shape { func area() -> Double }
来源：http://jbs.zdqjudy.top

[T31] Lua：Hello World
来源：http://xsz.nanxinkj.top

print("Hello")
来源：http://pfv.yonumen.top

[T32] Lua：局部变量
来源：http://aja.guannengcc.top

local a = 1
来源：http://hyu.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://tiy.zhijiandao.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zcz.daria6918.cn

[T34] Lua：遍历表
来源：http://uct.jqgufenzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gkx.andypj.xyz

[T35] Lua：字典表
来源：http://qso.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://wem.iojbl.cn

[T36] Lua：函数
来源：http://gfb.hysaishi.cn

function add(a, b) return a + b end
来源：http://wkl.nwbrower.top

[T37] Lua：字符串拼接
来源：http://zpj.yfazqb.com

"a" .. "b"
来源：http://ssv.zdbjq.cn

[T38] Lua：条件
来源：http://plj.wangdashe.top

if x > 0 then print("正") end
来源：http://ifq.yvedp.cn

[T39] Lua：模式匹配
来源：http://xbv.zhoulong.xyz

string.find(s, "%d+")
来源：http://ysq.sxryk.cn

[T40] Lua：元表
来源：http://jpp.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://txx.aibaodan.cn

[T41] Perl：Hello World
来源：http://kfm.hesvh.cn

print "Hello\n";
来源：http://ugr.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://tyg.nwbrower.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oqp.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://gog.0kj1m.cn

"值: $a"
来源：http://aew.yj20258.top

[T44] Perl：条件
来源：http://xqq.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://hfs.ppjwa.cn

[T45] Perl：数组遍历
来源：http://nys.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://aba.wangshuangyany.cn

[T46] Perl：哈希操作
来源：http://fzs.cashguo.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vfl.zdqjudy.top

[T47] Perl：正则捕获
来源：http://wpo.ybcxt.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rts.jqgfzy.top

[T48] Perl：正则替换
来源：http://gdj.shanyushiyangkeji.top

$s =~ s/old/new/g;
来源：http://juh.52xcode.cn

[T49] Perl：函数
来源：http://xzu.fzhhl.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wrn.shzxlz.cn

[T50] Perl：逐行读文件
来源：http://txt.iojbl.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kvt.xylfe.cn

while (my $line = <$fh>) { print $line; }
来源：http://scq.epnwcf.com

[T51] Scala：Hello World
来源：http://zay.fehbvm.com

println("Hello")
来源：http://nun.ybcxt.top

[T52] Scala：变量
来源：http://cfa.uphjek.com

val a = 1;  var b = 2
来源：http://jwi.tian-w.cn

[T53] Scala：字符串插值
来源：http://dtf.meibo888.top

s"值: $b"
来源：http://dls.hnxiangtu.top

[T54] Scala：集合映射
来源：http://tgp.yj20258.top

List(1, 2, 3).map(_ * 2)
来源：http://yzx.pycfn.com

[T55] Scala：集合过滤
来源：http://lij.zhoulong.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://pil.daxiang520.top

[T56] Scala：样例类
来源：http://nho.jlsjyb.cn

case class User(name: String, age: Int)
来源：http://qjh.hongshengwenyu.top

[T57] Scala：模式匹配
来源：http://oms.jinghuilouyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fhs.zhoulong.xyz

[T58] Scala：函数定义
来源：http://yzg.shanyushiyangtech.top

def add(a: Int, b: Int): Int = a + b
来源：http://vpx.feifeiyinyue.top

[T59] Scala：循环
来源：http://egh.hammf.cn

for (i <- 1 to 10) println(i)
来源：http://tgb.shanyushiyangkeji.top

[T60] Scala：折叠
来源：http://dkb.hfpthk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://exs.daria6918.cn

================================================================================
来源：http://jil.gogol.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xjz.hysaishi.cn

================================================================================
来源：http://bww.wangdashe.top

[U01] Py：创建虚拟环境
来源：http://ect.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://nbo.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://iml.iojbl.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pkj.yuxming.cn

[U03] Py：加载 .env 配置
来源：http://cvc.aibaodan.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fet.cucudq.cn

[U04] Py：变量调试打印
来源：http://ieh.yuxming.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://whw.yfazqb.com

[U05] Py：列表去重且保序
来源：http://xjn.hfpthk.cn

list(dict.fromkeys(arr))
来源：http://cix.kuanghao11.cn

[U06] Py：合并两个字典
来源：http://neq.redwolf501.top

{**a, **b}
来源：http://jfh.iojbl.cn

[U07] Py：反转字典键值
来源：http://qui.kuanghao11.cn

{v: k for k, v in d.items()}
来源：http://jyc.hammf.cn

[U08] Py：展平二维列表
来源：http://kzg.birdmap.top

[y for x in nested for y in x]
来源：http://uqd.yvedp.cn

[U09] Py：字典取最大值的键
来源：http://xcd.fktsv.cn

max(d, key=d.get)
来源：http://oip.daxiang520.top

[U10] Py：按值排序字典
来源：http://glm.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ywd.aizwys.cn

[U11] Py：生成器表达式
来源：http://mxx.ctjpmb.com

(x * 2 for x in arr)
来源：http://tso.jinqigfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://hfp.gzhubu.top

Counter(arr).most_common(3)
来源：http://glk.fehbvm.com

[U13] Py：固定长度队列
来源：http://iwo.shanyushiyangkeji.top

deque(maxlen=10)
来源：http://cff.ivvv.top

[U14] Py：分组收集到列表
来源：http://ibf.zhoulong.xyz

defaultdict(list)
来源：http://rky.shuidangran.top

[U15] Py：高精度计时
来源：http://oyt.jinyuanbaomall.cn

t = time.perf_counter()
来源：http://dnn.gaohongyu789.top

[U16] Py：命令行参数解析
来源：http://bvn.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qfd.meibo888.top

[U17] Py：初始化日志
来源：http://www.gaohongyu789.top

logging.basicConfig(level=logging.INFO)
来源：http://vol.ybcxt.top

[U18] Py：预编译正则
来源：http://xcj.cheryme.top

pat = re.compile(r"\d+")
来源：http://amq.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://sbq.shanyushiyangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sua.jinyuanbaomall.cn

[U20] Py：缓存函数结果
来源：http://ozt.gzhubu.top

@functools.lru_cache(maxsize=None)
来源：http://yre.sxryk.cn

[U21] Py：自定义上下文管理器
来源：http://iua.wangdashe.top

@contextlib.contextmanager
来源：http://bpf.tarul.cn

[U22] Py：矩阵转置
来源：http://iwp.sxryk.cn

list(zip(*m))
来源：http://pik.epnwcf.com

[U23] Py：分块读取大文件
来源：http://rcw.fzhhl.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fsq.c1oappe.top

[U24] Py：路径操作
来源：http://cdk.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ywh.yj202588.top

[U25] Py：CSV 按字典读
来源：http://pgj.tanke756.top

csv.DictReader(f)
来源：http://mov.jlsjyb.cn

[U26] Py：并发下载
来源：http://bqv.zhoulong.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wbb.jianghu66.top

[U27] Py：异步 HTTP
来源：http://hby.nanxinkj.top

aiohttp.ClientSession() 配合 async with
来源：http://fje.xylfe.cn

[U28] Py：类型别名
来源：http://ojx.yangfankeji.com

UserId = int
来源：http://hgy.chenlongwang.top

[U29] Py：属性校验
来源：http://tiu.havefunace.top

@property 与 @x.setter 配合
来源：http://lcr.ivvv.top

[U30] Py：数据类
来源：http://kyd.andypj.xyz

@dataclass(slots=True)
来源：http://jga.tarul.cn

[U31] Py：单测
来源：http://zwl.wangdashe.top

python -m pytest -q
来源：http://ygz.birdmap.top

[U32] Py：代码格式化
来源：http://wik.feifeiyinyue.top

ruff format . && ruff check --fix .
来源：http://fsm.dianchejie.cn

[U33] Py：打包发布
来源：http://uxq.sxryk.cn

python -m build  （依赖 pyproject.toml）
来源：http://efr.c1oappe.top

[U34] Py：判断编码
来源：http://wsx.svipenyu.cn

chardet.detect(raw)
来源：http://lbj.wangdashe.top

[U35] Py：发送邮件
来源：http://sgn.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sno.cucudq.cn

[U36] Py：定时任务
来源：http://drd.yj202588.top

schedule.every(10).minutes.do(job)
来源：http://omr.shuidangran.top

[U37] Py：读写 Excel
来源：http://nur.ydzc1.top

pandas.read_excel / DataFrame.to_excel
来源：http://fbp.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://zro.shanyushiyangtech.top

Path(__file__).resolve().parent
来源：http://doh.fengsongda.top

[U39] Py：判断是否在交互环境
来源：http://dfz.chenzaomai.com

sys.stdout.isatty()
来源：http://qki.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://kav.hfpthk.cn

print("err", file=sys.stderr)
来源：http://ufg.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://prx.zhaomingkeji.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://slh.shuidangran.top

[U42] PHP：PSR-4 自动加载
来源：http://fvr.zhoulong.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kxd.havefunace.top

[U43] PHP：声明命名空间
来源：http://bpt.cdnleiting.top

namespace App\Http;
来源：http://lir.316326.xyz

[U44] PHP：开启严格类型
来源：http://vyu.yj202588.top

declare(strict_types=1);
来源：http://rtj.tanke756.top

[U45] PHP：类型声明与返回类型
来源：http://nnv.sufxvd.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kck.hongshengwenyu.top

[U46] PHP：可空类型
来源：http://vwe.fengsongda.top

?string $name = null
来源：http://qno.andypj.xyz

[U47] PHP：联合类型
来源：http://uty.sweek.top

int|string $id
来源：http://qcx.xuanzx.com

[U48] PHP：纯枚举
来源：http://mcw.yueranfly.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rzf.sweek.top

[U49] PHP：只读属性
来源：http://vjr.jyoumei.cn

public readonly string $name
来源：http://ykc.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://fiy.yj20258.top

public function __construct(private int $id) {}
来源：http://lgx.shzxlz.cn

[U51] PHP：数组解构
来源：http://nws.dianchejie.cn

[$a, $b] = $arr;
来源：http://tpp.yuanzhike.top

[U52] PHP：箭头函数
来源：http://hja.zdbjq.cn

$double = fn($x) => $x * 2;
来源：http://lud.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://pin.tian-w.cn

$v = $a ?? $b ?? "default";
来源：http://qyh.ehwqpu.com

[U54] PHP：空安全调用
来源：http://ffy.jyoumei.cn

$obj?->method()
来源：http://cyv.jyoumei.cn

[U55] PHP：match 表达式
来源：http://eek.0kj1m.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dat.yueranfly.top

[U56] PHP：命名参数
来源：http://ywf.yuanzhike.top

f(a: 1, b: 2)
来源：http://khe.yonumen.top

[U57] PHP：字符串插值
来源：http://exo.9152youxi.cn

"值: {$a}"
来源：http://woo.ydzc1.top

[U58] PHP：数组三件套
来源：http://hge.xingfuxueyuan.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gph.ydjk.org.cn

[U59] PHP：自定义排序
来源：http://tdk.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nno.shuidangran.top

[U60] PHP：JSON 编解码
来源：http://qdp.zdqjudy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://idm.aibaodan.cn

[U61] PHP：正则
来源：http://iaf.ybcxt.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qhm.52xcode.cn

[U62] PHP：日期对象
来源：http://tzb.sufxvd.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://thf.andypj.xyz

[U63] PHP：文件读写
来源：http://iga.fzhhl.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iey.hcnkem.com

[U64] PHP：目录遍历
来源：http://woa.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://tls.52xcode.cn

[U65] PHP：会话
来源：http://xff.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ris.xylfe.cn

[U66] PHP：设置 Cookie
来源：http://mik.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oim.ehwqpu.com

[U67] PHP：处理文件上传
来源：http://psh.316326.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gtw.feifeiyinyue.top

[U68] PHP：PDO 连接
来源：http://zyi.fanxiaobao.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://igy.zhengqikj.top

[U69] PHP：PDO 预处理
来源：http://ceu.tarul.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kkh.ywan-chungtsiang.top

[U70] PHP：PDO 事务
来源：http://hwy.nanxinkj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ipf.zhixingplan.top

[U71] PHP：抛出异常
来源：http://hwr.pycfn.com

throw new RuntimeException("失败", 500);
来源：http://pnd.quarkkingdee.top

[U72] PHP：写错误日志
来源：http://tiu.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://umw.zhijiandao.cn

[U73] PHP：读取 ini 配置
来源：http://vii.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://wkf.sufxvd.cn

[U74] PHP：读取环境变量
来源：http://bxh.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://mxe.yuxming.cn

[U75] PHP：依赖注入
来源：http://dka.hongshengwenyu.top

composer require psr/container
来源：http://jff.gotoacloud.top

[U76] PHP：简单路由
来源：http://len.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zgh.tanke756.top

[U77] PHP：模板渲染
来源：http://idx.daxiang520.top

composer require twig/twig
来源：http://acy.dashuyun.cn

[U78] PHP：单元测试
来源：http://jwa.fzhhl.top

composer require --dev phpunit/phpunit
来源：http://yev.nwbrower.top

[U79] PHP：静态分析
来源：http://uaq.chenzaomai.com

composer require --dev phpstan/phpstan
来源：http://dug.xingfuxueyuan.xyz

[U80] PHP：代码规范修复
来源：http://ukj.yueranfly.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ybb.vehdjk.com

[U81] JS：初始化项目
来源：http://tns.bbcook.cn

npm init -y;  npm i express
来源：http://kwe.shuidangran.top

[U82] JS：package.json 脚本
来源：http://juv.52xcode.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oyz.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://mfo.guannengcc.top

export const a = 1;  import { a } from "./m.js";
来源：http://ooo.cdnleiting.top

[U84] JS：CommonJS 写法
来源：http://olk.zhengqikj.top

module.exports = { a };  const { a } = require("./m");
来源：http://jpv.havefunace.top

[U85] JS：可选链
来源：http://qpz.sufxvd.cn

a?.b?.c
来源：http://kcz.cheryme.top

[U86] JS：空值合并
来源：http://dce.jinghuilouyu.cn

a ?? b
来源：http://old.daxiang520.top

[U87] JS：解构默认值
来源：http://out.hfpthk.cn

const { a = 1, b = 2 } = obj;
来源：http://bmy.c1oappe.top

[U88] JS：对象展开合并
来源：http://gxs.jianghu66.top

{ ...a, ...b }
来源：http://ovn.yuanzhike.top

[U89] JS：数组去重
来源：http://ohf.52xcode.cn

[...new Set(arr)]
来源：http://kks.wangdashe.top

[U90] JS：数字数组排序
来源：http://dxq.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://tvw.fzhhl.top

[U91] JS：对象键值遍历
来源：http://ucm.gzhubu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bar.epnwcf.com

[U92] JS：深拷贝
来源：http://wow.hysaishi.cn

structuredClone(obj)
来源：http://fyr.zhongyouzk.top


<!-- 参考信息 -->