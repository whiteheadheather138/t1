代发 wailian999

[T09] Kotlin：扩展函数
来源：http://edp.zdbjq.cn

fun String.exclaim() = this + "!"
来源：http://egb.xziqi.cn

[T10] Kotlin：默认参数
来源：http://eev.yanxiufei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://arc.xuetiantiany.cn

[T11] Kotlin：协程
来源：http://tlb.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mzf.xziqi.cn

[T12] Kotlin：解构声明
来源：http://qeu.fktsv.cn

val (a, b) = Pair(1, 2)
来源：http://ttl.aizwys.cn

[T13] Kotlin：只读 Map
来源：http://jak.zhongyouzk.top

val m = mapOf("a" to 1)
来源：http://ljh.hywenlv.cn

[T14] Kotlin：循环
来源：http://eco.guannengcc.top

for (i in 1..10) println(i)
来源：http://num.cqqwz.cn

[T15] Kotlin：接口
来源：http://xlz.zhaomingkeji.xyz

interface Shape { fun area(): Double }
来源：http://avv.hnxiangtu.top

[T16] Swift：Hello World
来源：http://bqi.kuanghao11.cn

print("Hello")
来源：http://kdw.havefunace.top

[T17] Swift：变量与常量
来源：http://tza.chenlongwang.top

var a = 1;  let b = 2
来源：http://ciu.andypj.xyz

[T18] Swift：字符串插值
来源：http://aum.yangfankeji.com

"值: \(b)"
来源：http://ycv.sysykeji.top

[T19] Swift：可选绑定
来源：http://wga.cheryme.top

if let n = opt { print(n) }
来源：http://jjr.hnxiangtu.top

[T20] Swift：数组操作
来源：http://rmx.jinyuanbaomall.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mmk.jinqigfzy.top

[T21] Swift：遍历
来源：http://bwo.zhiwuduotai.top

for x in a { print(x) }
来源：http://wmr.zhengqikj.top

[T22] Swift：字典
来源：http://hpy.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nyn.snrcjt.cn

[T23] Swift：函数
来源：http://ihi.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://owr.c1oappe.top

[T24] Swift：闭包
来源：http://xns.xinyue.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://lzd.gotoacloud.top

[T25] Swift：结构体
来源：http://rjs.pycfn.com

struct P { var x: Int }
来源：http://nrk.aizwys.cn

[T26] Swift：类与重写
来源：http://ygj.shanyushiyangkeji.top

class A: Base { override func f() {} }
来源：http://voc.nwbrower.top

[T27] Swift：错误处理
来源：http://crv.dashuyun.cn

do { try f() } catch { print(error) }
来源：http://pal.wangshuangyany.cn

[T28] Swift：枚举
来源：http://jus.gotoacloud.top

enum Color { case red, green }
来源：http://mvi.yanxiufei.cn

[T29] Swift：guard 提前返回
来源：http://eho.hcnkem.com

guard let x = opt else { return }
来源：http://jvs.ybcxt.top

[T30] Swift：协议
来源：http://frj.ivvv.top

protocol Shape { func area() -> Double }
来源：http://dkv.bbcook.cn

[T31] Lua：Hello World
来源：http://akk.yj20258.top

print("Hello")
来源：http://cvb.guowangkeji.top

[T32] Lua：局部变量
来源：http://iqi.yuxming.cn

local a = 1
来源：http://vyd.quarkkingdee.top

[T33] Lua：表（数组）
来源：http://wss.quarkkingdee.top

local t = {1, 2, 3};  t[4] = 4
来源：http://koo.dashuyun.cn

[T34] Lua：遍历表
来源：http://bcn.fanxiaobao.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://ljq.sxryk.cn

[T35] Lua：字典表
来源：http://coy.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://aey.feifeiyinyue.top

[T36] Lua：函数
来源：http://hwi.zhiwuduotai.top

function add(a, b) return a + b end
来源：http://mno.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://gxp.aibaodan.cn

"a" .. "b"
来源：http://hru.aibaodan.cn

[T38] Lua：条件
来源：http://oes.jianghu66.top

if x > 0 then print("正") end
来源：http://wlu.ehwqpu.com

[T39] Lua：模式匹配
来源：http://gyu.yanxiufei.cn

string.find(s, "%d+")
来源：http://tsw.yueranfly.top

[T40] Lua：元表
来源：http://fkc.jinyuanbaomall.cn

setmetatable({}, { __index = base })
来源：http://qmb.fktsv.cn

[T41] Perl：Hello World
来源：http://uxm.yangfankeji.com

print "Hello\n";
来源：http://rpu.hysaishi.cn

[T42] Perl：变量类型
来源：http://tmp.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qkl.smart0.xyz

[T43] Perl：字符串插值
来源：http://yum.fzhhl.top

"值: $a"
来源：http://oao.tianlin.xyz

[T44] Perl：条件
来源：http://mkv.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://pdo.fehbvm.com

[T45] Perl：数组遍历
来源：http://kva.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://kfi.fehbvm.com

[T46] Perl：哈希操作
来源：http://yej.sxryk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oig.yj20258888.top

[T47] Perl：正则捕获
来源：http://shq.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://eqx.ivvv.top

[T48] Perl：正则替换
来源：http://ptn.epnwcf.com

$s =~ s/old/new/g;
来源：http://nie.sufxvd.cn

[T49] Perl：函数
来源：http://czh.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nng.gaohongyu789.top

[T50] Perl：逐行读文件
来源：http://gid.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vbs.sxryk.cn

while (my $line = <$fh>) { print $line; }
来源：http://ixk.zdqjudy.top

[T51] Scala：Hello World
来源：http://qtt.nanxinkj.top

println("Hello")
来源：http://hme.guowangkeji.top

[T52] Scala：变量
来源：http://zox.chenlongwang.top

val a = 1;  var b = 2
来源：http://mgk.cheryme.top

[T53] Scala：字符串插值
来源：http://tjw.yuxming.cn

s"值: $b"
来源：http://aly.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://apn.uphjek.com

List(1, 2, 3).map(_ * 2)
来源：http://lbr.guannengcc.top

[T55] Scala：集合过滤
来源：http://dbs.ehwqpu.com

List(1, 2, 3).filter(_ > 1)
来源：http://jpj.xuetiantiany.cn

[T56] Scala：样例类
来源：http://lgt.ybcxt.top

case class User(name: String, age: Int)
来源：http://kel.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://ckh.meibo888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mcl.ydjk.org.cn

[T58] Scala：函数定义
来源：http://gtv.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://lct.ybcxt.top

[T59] Scala：循环
来源：http://mxt.sufxvd.cn

for (i <- 1 to 10) println(i)
来源：http://mtc.jqgfzy.top

[T60] Scala：折叠
来源：http://ftc.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wsv.shuidangran.top

================================================================================
来源：http://yjg.redwolf501.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ehw.xuanzx.com

================================================================================
来源：http://vkv.yfazqb.com

[U01] Py：创建虚拟环境
来源：http://dvr.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://mgb.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://tbu.hesvh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ayq.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://iee.snrcjt.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://egt.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://zmw.nanxuanxn.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fxe.hysaishi.cn

[U05] Py：列表去重且保序
来源：http://tza.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://kqd.yuanzhike.top

[U06] Py：合并两个字典
来源：http://vkr.haohaochexian.top

{**a, **b}
来源：http://kfj.yonumen.top

[U07] Py：反转字典键值
来源：http://dnj.yueranfly.top

{v: k for k, v in d.items()}
来源：http://gky.hesvh.cn

[U08] Py：展平二维列表
来源：http://boc.havefunace.top

[y for x in nested for y in x]
来源：http://cdv.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://xiy.xziqi.cn

max(d, key=d.get)
来源：http://ozr.ctjpmb.com

[U10] Py：按值排序字典
来源：http://gju.daxiang520.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kzr.ywan-chungtsiang.top

[U11] Py：生成器表达式
来源：http://qmk.gaohongyu789.top

(x * 2 for x in arr)
来源：http://iav.sjlbkw.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xse.yangfankeji.com

Counter(arr).most_common(3)
来源：http://sge.jianghu66.top

[U13] Py：固定长度队列
来源：http://frc.aibaodan.cn

deque(maxlen=10)
来源：http://hyj.yfazqb.com

[U14] Py：分组收集到列表
来源：http://bkr.xingfuxueyuan.xyz

defaultdict(list)
来源：http://qqv.zycfv.cn

[U15] Py：高精度计时
来源：http://mjm.ydzc1.top

t = time.perf_counter()
来源：http://cog.zycfv.cn

[U16] Py：命令行参数解析
来源：http://fct.aibaodan.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://syi.jqgfzy.top

[U17] Py：初始化日志
来源：http://qtv.wangshuangyany.cn

logging.basicConfig(level=logging.INFO)
来源：http://epf.ctjpmb.com

[U18] Py：预编译正则
来源：http://npg.chenjidiqi.icu

pat = re.compile(r"\d+")
来源：http://mqu.hnqzz.top

[U19] Py：正则替换带回调
来源：http://ihv.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bpo.vqdsnc.cn

[U20] Py：缓存函数结果
来源：http://ybf.sweek.top

@functools.lru_cache(maxsize=None)
来源：http://auq.52xcode.cn

[U21] Py：自定义上下文管理器
来源：http://owb.tanke756.top

@contextlib.contextmanager
来源：http://gxa.ivvv.top

[U22] Py：矩阵转置
来源：http://rjh.bbcook.cn

list(zip(*m))
来源：http://wmi.pycfn.com

[U23] Py：分块读取大文件
来源：http://mpb.chenlongwang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wlq.chenlongwang.top

[U24] Py：路径操作
来源：http://ysr.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gqe.hammf.cn

[U25] Py：CSV 按字典读
来源：http://qac.ydjk.org.cn

csv.DictReader(f)
来源：http://ejh.ydzc1.top

[U26] Py：并发下载
来源：http://zdc.dianchejie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mvz.sxryk.cn

[U27] Py：异步 HTTP
来源：http://soy.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://vii.hammf.cn

[U28] Py：类型别名
来源：http://gam.xylfe.cn

UserId = int
来源：http://leg.sjlbkw.cn

[U29] Py：属性校验
来源：http://rey.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://pll.hysaishi.cn

[U30] Py：数据类
来源：http://kzi.0kj1m.cn

@dataclass(slots=True)
来源：http://ibx.ppjwa.cn

[U31] Py：单测
来源：http://bud.fehbvm.com

python -m pytest -q
来源：http://kre.sjlbkw.cn

[U32] Py：代码格式化
来源：http://zqe.zhaomingkeji.xyz

ruff format . && ruff check --fix .
来源：http://jfg.52xcode.cn

[U33] Py：打包发布
来源：http://esv.feifeiyinyue.top

python -m build  （依赖 pyproject.toml）
来源：http://ugx.yj20258888.top

[U34] Py：判断编码
来源：http://pzi.xinyue.icu

chardet.detect(raw)
来源：http://bmz.gzhubu.top

[U35] Py：发送邮件
来源：http://yce.yanxiufei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rmb.fktsv.cn

[U36] Py：定时任务
来源：http://gsc.yfazqb.com

schedule.every(10).minutes.do(job)
来源：http://ikp.yongpay.top

[U37] Py：读写 Excel
来源：http://pvp.birdmap.top

pandas.read_excel / DataFrame.to_excel
来源：http://ynb.chenjidiqi.icu

[U38] Py：获取脚本所在目录
来源：http://dnk.cashguo.top

Path(__file__).resolve().parent
来源：http://jgj.shuidangran.top

[U39] Py：判断是否在交互环境
来源：http://log.shzxlz.cn

sys.stdout.isatty()
来源：http://avm.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://wnq.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://dcf.shanyushiyangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://idu.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://dri.ctjpmb.com

[U42] PHP：PSR-4 自动加载
来源：http://wzd.tanke756.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dwq.tian-w.cn

[U43] PHP：声明命名空间
来源：http://vur.cucudq.cn

namespace App\Http;
来源：http://zsl.bjfxy.top

[U44] PHP：开启严格类型
来源：http://qzm.tarul.cn

declare(strict_types=1);
来源：http://rgc.jiagoushi.top

[U45] PHP：类型声明与返回类型
来源：http://zks.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://oxc.tianlin.xyz

[U46] PHP：可空类型
来源：http://yui.ivvv.top

?string $name = null
来源：http://sjy.dashuyun.cn

[U47] PHP：联合类型
来源：http://jym.sysykeji.top

int|string $id
来源：http://qbb.ybcxt.top

[U48] PHP：纯枚举
来源：http://qsy.tanke756.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://udt.ctjpmb.com

[U49] PHP：只读属性
来源：http://tsi.hesvh.cn

public readonly string $name
来源：http://hsv.hongshengwenyu.top

[U50] PHP：构造器属性提升
来源：http://sgm.mhx1999.top

public function __construct(private int $id) {}
来源：http://hlv.hnqzz.top

[U51] PHP：数组解构
来源：http://wfx.yvedp.cn

[$a, $b] = $arr;
来源：http://xfg.jqgufenzy.top

[U52] PHP：箭头函数
来源：http://sqi.ywan-chungtsiang.top

$double = fn($x) => $x * 2;
来源：http://orw.yfazqb.com

[U53] PHP：空合并运算符
来源：http://dbw.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://rvd.hywenlv.cn

[U54] PHP：空安全调用
来源：http://gzq.guowangkeji.top

$obj?->method()
来源：http://zxu.hammf.cn

[U55] PHP：match 表达式
来源：http://ujp.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xhc.tian-w.cn

[U56] PHP：命名参数
来源：http://dnx.andypj.xyz

f(a: 1, b: 2)
来源：http://ubn.tarul.cn

[U57] PHP：字符串插值
来源：http://avm.shanyushiyangtech.top

"值: {$a}"
来源：http://vil.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://ahx.jiagoushi.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mgs.cqqwz.cn

[U59] PHP：自定义排序
来源：http://key.zhijiandao.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://byb.gzhubu.top

[U60] PHP：JSON 编解码
来源：http://yhm.dianchejie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://czh.snrcjt.cn

[U61] PHP：正则
来源：http://smt.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zsg.hysaishi.cn

[U62] PHP：日期对象
来源：http://clp.guowangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ctf.yonumen.top

[U63] PHP：文件读写
来源：http://mvl.hywenlv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ddy.zhijiandao.cn

[U64] PHP：目录遍历
来源：http://tpe.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://hvu.chenlongwang.top

[U65] PHP：会话
来源：http://lyj.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nyr.zhaomingkeji.xyz

[U66] PHP：设置 Cookie
来源：http://sou.hnxiangtu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tld.tarul.cn

[U67] PHP：处理文件上传
来源：http://vdy.daxiang520.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://swa.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://uhn.nanxinkj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nnd.wangdashe.top

[U69] PHP：PDO 预处理
来源：http://rcx.vqdsnc.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aib.cqqwz.cn

[U70] PHP：PDO 事务
来源：http://poq.hesvh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://one.aizwys.cn

[U71] PHP：抛出异常
来源：http://sox.ydjk.org.cn

throw new RuntimeException("失败", 500);
来源：http://auf.zhixingplan.top

[U72] PHP：写错误日志
来源：http://agm.xingfuxueyuan.xyz

error_log("失败: " . $e->getMessage());
来源：http://vla.fzhhl.top

[U73] PHP：读取 ini 配置
来源：http://dky.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://fwj.feifeiyinyue.top

[U74] PHP：读取环境变量
来源：http://ivh.aizwys.cn

getenv("APP_ENV") ?: "production"
来源：http://arg.zhengqikj.top

[U75] PHP：依赖注入
来源：http://cjq.daxiang520.top

composer require psr/container
来源：http://loy.jqgfzy.top

[U76] PHP：简单路由
来源：http://uzm.bbcook.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ehr.yfazqb.com

[U77] PHP：模板渲染
来源：http://wzc.hfpthk.cn

composer require twig/twig
来源：http://xcn.yangfankeji.com

[U78] PHP：单元测试
来源：http://vgt.shanyushiyangtech.top

composer require --dev phpunit/phpunit
来源：http://qyg.yanxiufei.cn

[U79] PHP：静态分析
来源：http://zke.bbcook.cn

composer require --dev phpstan/phpstan
来源：http://zbw.ehwqpu.com

[U80] PHP：代码规范修复
来源：http://jav.andypj.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://kru.yanxiufei.cn

[U81] JS：初始化项目
来源：http://trb.pycfn.com

npm init -y;  npm i express
来源：http://xwm.nanxinkj.top

[U82] JS：package.json 脚本
来源：http://dvl.snrcjt.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fhv.shanyushiyangtech.top

[U83] JS：ES Module 导入导出
来源：http://wlc.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://bqe.cdnleiting.top

[U84] JS：CommonJS 写法
来源：http://pzh.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://aua.zhixingplan.top

[U85] JS：可选链
来源：http://rio.jinqigufen.top

a?.b?.c
来源：http://sno.xuetiantiany.cn

[U86] JS：空值合并
来源：http://cbm.gzhubu.top

a ?? b
来源：http://lxp.316326.xyz

[U87] JS：解构默认值
来源：http://xii.ehwqpu.com

const { a = 1, b = 2 } = obj;
来源：http://bvl.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://whr.hammf.cn

{ ...a, ...b }
来源：http://ktp.chenzaomai.com

[U89] JS：数组去重
来源：http://evm.vehdjk.com

[...new Set(arr)]
来源：http://rmk.shuidangran.top

[U90] JS：数字数组排序
来源：http://piq.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://vsi.aibaodan.cn

[U91] JS：对象键值遍历
来源：http://qrp.xinyue.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gtb.xinyue.icu

[U92] JS：深拷贝
来源：http://ghd.snrcjt.cn

structuredClone(obj)
来源：http://oex.gaohongyu789.top

[U93] JS：模板字符串
来源：http://wry.yangfankeji.com

`共 ${n} 条`
来源：http://pwr.zhengqikj.top

[U94] JS：箭头函数
来源：http://pnh.smart0.xyz

const double = x => x * 2;
来源：http://woc.hammf.cn

[U95] JS：Promise 包装
来源：http://ovt.ctjpmb.com

new Promise((resolve, reject) => {})
来源：http://wat.epnwcf.com

[U96] JS：async/await 与异常
来源：http://nqb.daria6918.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ocg.hysaishi.cn


<!-- 参考信息 -->