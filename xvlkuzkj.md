代发 wailian999

[T05] Kotlin：when 表达式
来源：http://uxt.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://spm.daria6918.cn

[T06] Kotlin：集合映射
来源：http://fwk.ehwqpu.com

listOf(1, 2, 3).map { it * 2 }
来源：http://xrs.zycfv.cn

[T07] Kotlin：集合过滤
来源：http://gmf.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://qiz.feifeiyinyue.top

[T08] Kotlin：数据类
来源：http://pud.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://jyi.chenjidiqi.icu

[T09] Kotlin：扩展函数
来源：http://mjj.kuanghao11.cn

fun String.exclaim() = this + "!"
来源：http://fyx.meibo888.top

[T10] Kotlin：默认参数
来源：http://hir.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gac.gogol.net.cn

[T11] Kotlin：协程
来源：http://mmh.nanxuanxn.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nvz.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://vrc.cashguo.top

val (a, b) = Pair(1, 2)
来源：http://cgm.jianghu66.top

[T13] Kotlin：只读 Map
来源：http://vln.chenzaomai.com

val m = mapOf("a" to 1)
来源：http://xbx.sysykeji.top

[T14] Kotlin：循环
来源：http://fjc.zdqjudy.top

for (i in 1..10) println(i)
来源：http://jma.zhixingplan.top

[T15] Kotlin：接口
来源：http://iuf.yfazqb.com

interface Shape { fun area(): Double }
来源：http://tyj.iojbl.cn

[T16] Swift：Hello World
来源：http://xyx.chenjidiqi.icu

print("Hello")
来源：http://kni.ywan-chungtsiang.top

[T17] Swift：变量与常量
来源：http://ctx.jqgufenzy.top

var a = 1;  let b = 2
来源：http://kcs.52xcode.cn

[T18] Swift：字符串插值
来源：http://fmq.sweek.top

"值: \(b)"
来源：http://yjw.yueranfly.top

[T19] Swift：可选绑定
来源：http://ozz.iojbl.cn

if let n = opt { print(n) }
来源：http://mwl.hammf.cn

[T20] Swift：数组操作
来源：http://lgr.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gmy.andypj.xyz

[T21] Swift：遍历
来源：http://dau.iojbl.cn

for x in a { print(x) }
来源：http://ffv.hfpthk.cn

[T22] Swift：字典
来源：http://rxi.hesvh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ykr.vqdsnc.cn

[T23] Swift：函数
来源：http://vhr.aibaodan.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ltl.xziqi.cn

[T24] Swift：闭包
来源：http://mlb.tian-w.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://baw.jinyuanbaomall.cn

[T25] Swift：结构体
来源：http://jkz.gaohongyu789.top

struct P { var x: Int }
来源：http://ehl.shuidangran.top

[T26] Swift：类与重写
来源：http://qjj.c1oappe.top

class A: Base { override func f() {} }
来源：http://gab.sufxvd.cn

[T27] Swift：错误处理
来源：http://jff.kuanghao11.cn

do { try f() } catch { print(error) }
来源：http://zdl.chenlongwang.top

[T28] Swift：枚举
来源：http://mvp.tarul.cn

enum Color { case red, green }
来源：http://tjl.9152youxi.cn

[T29] Swift：guard 提前返回
来源：http://rbu.hnqzz.top

guard let x = opt else { return }
来源：http://lgb.daxiang520.top

[T30] Swift：协议
来源：http://rmk.316326.xyz

protocol Shape { func area() -> Double }
来源：http://pwm.xuetiantiany.cn

[T31] Lua：Hello World
来源：http://zgm.hfpthk.cn

print("Hello")
来源：http://zte.hysaishi.cn

[T32] Lua：局部变量
来源：http://vop.gotoacloud.top

local a = 1
来源：http://ryn.bjfxy.top

[T33] Lua：表（数组）
来源：http://xfd.hesvh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://glv.cdnleiting.top

[T34] Lua：遍历表
来源：http://duz.wangdashe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://iyh.hcnkem.com

[T35] Lua：字典表
来源：http://ftd.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://igq.vehdjk.com

[T36] Lua：函数
来源：http://nre.ybcxt.top

function add(a, b) return a + b end
来源：http://ajf.uphjek.com

[T37] Lua：字符串拼接
来源：http://cul.yvedp.cn

"a" .. "b"
来源：http://mvr.xinyue.icu

[T38] Lua：条件
来源：http://isd.shangyingyoupin.top

if x > 0 then print("正") end
来源：http://ywx.zdqjudy.top

[T39] Lua：模式匹配
来源：http://rud.tian-w.cn

string.find(s, "%d+")
来源：http://wkc.shanyushiyangtech.top

[T40] Lua：元表
来源：http://myk.tanke756.top

setmetatable({}, { __index = base })
来源：http://dsd.jiagoushi.top

[T41] Perl：Hello World
来源：http://nbb.meibo888.top

print "Hello\n";
来源：http://eyw.redwolf501.top

[T42] Perl：变量类型
来源：http://eqr.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://igj.tarul.cn

[T43] Perl：字符串插值
来源：http://ohj.cdnleiting.top

"值: $a"
来源：http://mkg.jinqigfzy.top

[T44] Perl：条件
来源：http://col.snrcjt.cn

if ($a > 0) { print "正"; }
来源：http://ibz.yanxiufei.cn

[T45] Perl：数组遍历
来源：http://vdx.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://rrp.cucudq.cn

[T46] Perl：哈希操作
来源：http://btb.316326.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cmn.epnwcf.com

[T47] Perl：正则捕获
来源：http://tcx.shanyushiyangtech.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zhy.c1oappe.top

[T48] Perl：正则替换
来源：http://tmg.epnwcf.com

$s =~ s/old/new/g;
来源：http://vyu.snrcjt.cn

[T49] Perl：函数
来源：http://pnt.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ara.sysykeji.top

[T50] Perl：逐行读文件
来源：http://eev.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qlh.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://cfw.tianlin.xyz

[T51] Scala：Hello World
来源：http://cpx.zycfv.cn

println("Hello")
来源：http://yby.ppjwa.cn

[T52] Scala：变量
来源：http://dfl.tian-w.cn

val a = 1;  var b = 2
来源：http://yqb.zhaomingkeji.xyz

[T53] Scala：字符串插值
来源：http://lhp.haohaochexian.top

s"值: $b"
来源：http://xig.ppjwa.cn

[T54] Scala：集合映射
来源：http://smi.fehbvm.com

List(1, 2, 3).map(_ * 2)
来源：http://kpo.hnqzz.top

[T55] Scala：集合过滤
来源：http://tcp.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://pge.gaohongyu789.top

[T56] Scala：样例类
来源：http://hsr.bbcook.cn

case class User(name: String, age: Int)
来源：http://ymz.gotoacloud.top

[T57] Scala：模式匹配
来源：http://cga.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://pky.iojbl.cn

[T58] Scala：函数定义
来源：http://vxp.ctjpmb.com

def add(a: Int, b: Int): Int = a + b
来源：http://dcd.jlsjyb.cn

[T59] Scala：循环
来源：http://bco.yanxiufei.cn

for (i <- 1 to 10) println(i)
来源：http://nqd.chenlongwang.top

[T60] Scala：折叠
来源：http://uxr.kuanghao11.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yrj.sjlbkw.cn

================================================================================
来源：http://zaw.9152youxi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kug.wangdashe.top

================================================================================
来源：http://gil.yuanzhike.top

[U01] Py：创建虚拟环境
来源：http://kda.sxryk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xud.zhiwuduotai.top

[U02] Py：导出 / 安装依赖
来源：http://iil.ydjk.org.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://owt.yueranfly.top

[U03] Py：加载 .env 配置
来源：http://xqy.jqgfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ruh.xuetiantiany.cn

[U04] Py：变量调试打印
来源：http://hnm.sufxvd.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uix.daxiang520.top

[U05] Py：列表去重且保序
来源：http://nkh.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://pjo.tanke756.top

[U06] Py：合并两个字典
来源：http://igo.hesvh.cn

{**a, **b}
来源：http://dbh.xylfe.cn

[U07] Py：反转字典键值
来源：http://fql.sufxvd.cn

{v: k for k, v in d.items()}
来源：http://ohd.yj20258.top

[U08] Py：展平二维列表
来源：http://uhn.daxiang520.top

[y for x in nested for y in x]
来源：http://plm.svipenyu.cn

[U09] Py：字典取最大值的键
来源：http://zff.hysaishi.cn

max(d, key=d.get)
来源：http://xoc.zhongyouzk.top

[U10] Py：按值排序字典
来源：http://iti.hesvh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fvb.jianghu66.top

[U11] Py：生成器表达式
来源：http://nnc.vehdjk.com

(x * 2 for x in arr)
来源：http://ogz.xuetiantiany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sec.meibo888.top

Counter(arr).most_common(3)
来源：http://vgy.zdbjq.cn

[U13] Py：固定长度队列
来源：http://jan.redwolf501.top

deque(maxlen=10)
来源：http://rkg.cheryme.top

[U14] Py：分组收集到列表
来源：http://boa.fehbvm.com

defaultdict(list)
来源：http://vcb.ehwqpu.com

[U15] Py：高精度计时
来源：http://rxc.fktsv.cn

t = time.perf_counter()
来源：http://qbn.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://cix.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hml.tanke756.top

[U17] Py：初始化日志
来源：http://ikr.cucudq.cn

logging.basicConfig(level=logging.INFO)
来源：http://dqc.yuanzhike.top

[U18] Py：预编译正则
来源：http://bot.cashguo.top

pat = re.compile(r"\d+")
来源：http://hgd.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://ykj.birdmap.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://clu.snrcjt.cn

[U20] Py：缓存函数结果
来源：http://jyo.quarkkingdee.top

@functools.lru_cache(maxsize=None)
来源：http://gkt.pycfn.com

[U21] Py：自定义上下文管理器
来源：http://tdq.zhoulong.xyz

@contextlib.contextmanager
来源：http://msb.shangyingyoupin.top

[U22] Py：矩阵转置
来源：http://obm.meibo888.top

list(zip(*m))
来源：http://pyd.ctjpmb.com

[U23] Py：分块读取大文件
来源：http://wvt.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://owx.vqdsnc.cn

[U24] Py：路径操作
来源：http://gfd.fzhhl.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oue.cdnleiting.top

[U25] Py：CSV 按字典读
来源：http://xct.xylfe.cn

csv.DictReader(f)
来源：http://oko.quarkkingdee.top

[U26] Py：并发下载
来源：http://xgy.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qyu.birdmap.top

[U27] Py：异步 HTTP
来源：http://akg.fehbvm.com

aiohttp.ClientSession() 配合 async with
来源：http://vib.vehdjk.com

[U28] Py：类型别名
来源：http://gfh.ydjk.org.cn

UserId = int
来源：http://zac.fzhhl.top

[U29] Py：属性校验
来源：http://zxd.nanxinkj.top

@property 与 @x.setter 配合
来源：http://vei.shuidangran.top

[U30] Py：数据类
来源：http://ako.ivvv.top

@dataclass(slots=True)
来源：http://cmk.aizwys.cn

[U31] Py：单测
来源：http://evg.bbcook.cn

python -m pytest -q
来源：http://vsd.sjlbkw.cn

[U32] Py：代码格式化
来源：http://wzm.316326.xyz

ruff format . && ruff check --fix .
来源：http://ony.9152youxi.cn

[U33] Py：打包发布
来源：http://mlb.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://ouu.vehdjk.com

[U34] Py：判断编码
来源：http://cnh.chenlongwang.top

chardet.detect(raw)
来源：http://zyb.nanxinkj.top

[U35] Py：发送邮件
来源：http://jin.yuxming.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cat.yfazqb.com

[U36] Py：定时任务
来源：http://uvh.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://lee.yj20258.top

[U37] Py：读写 Excel
来源：http://yif.epnwcf.com

pandas.read_excel / DataFrame.to_excel
来源：http://zmy.shangyingyoupin.top

[U38] Py：获取脚本所在目录
来源：http://sga.ybcxt.top

Path(__file__).resolve().parent
来源：http://eqp.pengpengdd.cyou

[U39] Py：判断是否在交互环境
来源：http://obs.meibo888.top

sys.stdout.isatty()
来源：http://yfe.yuanzhike.top

[U40] Py：打印到标准错误
来源：http://vrr.pengpengdd.cyou

print("err", file=sys.stderr)
来源：http://ijg.52xcode.cn

[U41] PHP：初始化 Composer 项目
来源：http://lvl.jqgufenzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zvf.shuidangran.top

[U42] PHP：PSR-4 自动加载
来源：http://nsa.shanyushiyangtech.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zro.feifeiyinyue.top

[U43] PHP：声明命名空间
来源：http://uxa.fengsongda.top

namespace App\Http;
来源：http://cxh.hfpthk.cn

[U44] PHP：开启严格类型
来源：http://bje.zdbjq.cn

declare(strict_types=1);
来源：http://bwr.epnwcf.com

[U45] PHP：类型声明与返回类型
来源：http://zzn.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://aat.hnxiangtu.top

[U46] PHP：可空类型
来源：http://awp.jqgufenzy.top

?string $name = null
来源：http://ncn.sxryk.cn

[U47] PHP：联合类型
来源：http://mmy.aibaodan.cn

int|string $id
来源：http://urc.xuetiantiany.cn

[U48] PHP：纯枚举
来源：http://ixd.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mdb.sufxvd.cn

[U49] PHP：只读属性
来源：http://xaf.fehbvm.com

public readonly string $name
来源：http://utb.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://jza.wangshuangyany.cn

public function __construct(private int $id) {}
来源：http://lgc.jianghu66.top

[U51] PHP：数组解构
来源：http://gxl.bbcook.cn

[$a, $b] = $arr;
来源：http://ksz.zhijiandao.cn

[U52] PHP：箭头函数
来源：http://gmx.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://cav.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://pxm.guannengcc.top

$v = $a ?? $b ?? "default";
来源：http://hrc.nanxuanxn.top

[U54] PHP：空安全调用
来源：http://qfz.hesvh.cn

$obj?->method()
来源：http://dfj.yanxiufei.cn

[U55] PHP：match 表达式
来源：http://rzn.yj20258.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jkd.epnwcf.com

[U56] PHP：命名参数
来源：http://rex.yj20258888.top

f(a: 1, b: 2)
来源：http://aqd.jinqigfzy.top

[U57] PHP：字符串插值
来源：http://jnu.gaohongyu789.top

"值: {$a}"
来源：http://ofy.jyoumei.cn

[U58] PHP：数组三件套
来源：http://jhz.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tma.zhixingplan.top

[U59] PHP：自定义排序
来源：http://bmb.zhixingplan.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yrv.daria6918.cn

[U60] PHP：JSON 编解码
来源：http://feh.vehdjk.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://okg.ybcxt.top

[U61] PHP：正则
来源：http://ywv.sysykeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lsv.guannengcc.top

[U62] PHP：日期对象
来源：http://eex.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mwh.ppjwa.cn

[U63] PHP：文件读写
来源：http://mps.jqgfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uit.9152youxi.cn

[U64] PHP：目录遍历
来源：http://izq.daxiang520.top

glob("dir/*.php");  scandir("dir");
来源：http://riq.mhx1999.top

[U65] PHP：会话
来源：http://kwb.fengsongda.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dth.pycfn.com

[U66] PHP：设置 Cookie
来源：http://iau.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kvk.tarul.cn

[U67] PHP：处理文件上传
来源：http://fot.chenzaomai.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mpp.kuanghao11.cn

[U68] PHP：PDO 连接
来源：http://xcb.zdbjq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kkj.yuanzhike.top

[U69] PHP：PDO 预处理
来源：http://ssm.ehwqpu.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wkk.svipenyu.cn

[U70] PHP：PDO 事务
来源：http://jlp.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hva.guannengcc.top

[U71] PHP：抛出异常
来源：http://mov.andypj.xyz

throw new RuntimeException("失败", 500);
来源：http://sxb.zhiwuduotai.top

[U72] PHP：写错误日志
来源：http://rzd.jqgfzy.top

error_log("失败: " . $e->getMessage());
来源：http://qsv.0kj1m.cn

[U73] PHP：读取 ini 配置
来源：http://ddo.nwbrower.top

parse_ini_file("config.ini", true)
来源：http://kwn.cqqwz.cn

[U74] PHP：读取环境变量
来源：http://kyu.zhixingplan.top

getenv("APP_ENV") ?: "production"
来源：http://vyq.shuidangran.top

[U75] PHP：依赖注入
来源：http://wip.guowangkeji.top

composer require psr/container
来源：http://lnx.fanxiaobao.xyz

[U76] PHP：简单路由
来源：http://ole.yuanzhike.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kwp.yuanzhike.top

[U77] PHP：模板渲染
来源：http://iai.jyoumei.cn

composer require twig/twig
来源：http://oon.hcnkem.com

[U78] PHP：单元测试
来源：http://pjt.sweek.top

composer require --dev phpunit/phpunit
来源：http://yjg.fktsv.cn

[U79] PHP：静态分析
来源：http://ctl.fzhhl.top

composer require --dev phpstan/phpstan
来源：http://aku.cashguo.top

[U80] PHP：代码规范修复
来源：http://cgo.cqqwz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qkz.yuanzhike.top

[U81] JS：初始化项目
来源：http://tks.vqdsnc.cn

npm init -y;  npm i express
来源：http://gha.zhiwuduotai.top

[U82] JS：package.json 脚本
来源：http://bgz.nanxuanxn.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mob.ppjwa.cn

[U83] JS：ES Module 导入导出
来源：http://lxa.zhixingplan.top

export const a = 1;  import { a } from "./m.js";
来源：http://kia.feifeiyinyue.top

[U84] JS：CommonJS 写法
来源：http://qrn.yj20258888.top

module.exports = { a };  const { a } = require("./m");
来源：http://mbe.nanxuanxn.top

[U85] JS：可选链
来源：http://ogk.tianlin.xyz

a?.b?.c
来源：http://mgd.316326.xyz

[U86] JS：空值合并
来源：http://vjm.pengpengdd.cyou

a ?? b
来源：http://zcb.yj20258888.top

[U87] JS：解构默认值
来源：http://mjw.hnqzz.top

const { a = 1, b = 2 } = obj;
来源：http://dcf.daria6918.cn

[U88] JS：对象展开合并
来源：http://jdw.fzhhl.top

{ ...a, ...b }
来源：http://tqy.hysaishi.cn

[U89] JS：数组去重
来源：http://fri.zhaomingkeji.xyz

[...new Set(arr)]
来源：http://mji.fzhhl.top

[U90] JS：数字数组排序
来源：http://kdg.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://gag.yongpay.top

[U91] JS：对象键值遍历
来源：http://lbt.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tvf.meibo888.top

[U92] JS：深拷贝
来源：http://ztx.zhijiandao.cn

structuredClone(obj)
来源：http://zlq.vehdjk.com


<!-- 参考信息 -->