代发 wailian999

[T05] Kotlin：when 表达式
来源：http://uox.shanyushiyangtech.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vbb.kuanghao11.cn

[T06] Kotlin：集合映射
来源：http://zuu.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xfu.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://fnk.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wwv.xuanzx.com

[T08] Kotlin：数据类
来源：http://rta.hammf.cn

data class User(val name: String, val age: Int)
来源：http://sbo.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://pop.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://nax.yueranfly.top

[T10] Kotlin：默认参数
来源：http://kvw.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xob.hammf.cn

[T11] Kotlin：协程
来源：http://yvx.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nqq.nwbrower.top

[T12] Kotlin：解构声明
来源：http://ach.tian-w.cn

val (a, b) = Pair(1, 2)
来源：http://ohf.feifeiyinyue.top

[T13] Kotlin：只读 Map
来源：http://khl.hysaishi.cn

val m = mapOf("a" to 1)
来源：http://gmw.uphjek.com

[T14] Kotlin：循环
来源：http://rmk.pycfn.com

for (i in 1..10) println(i)
来源：http://lgy.dianchejie.cn

[T15] Kotlin：接口
来源：http://rdp.daria6918.cn

interface Shape { fun area(): Double }
来源：http://aqw.gotoacloud.top

[T16] Swift：Hello World
来源：http://wnh.wangdashe.top

print("Hello")
来源：http://tei.dianchejie.cn

[T17] Swift：变量与常量
来源：http://oxz.yueranfly.top

var a = 1;  let b = 2
来源：http://ets.cqqwz.cn

[T18] Swift：字符串插值
来源：http://dba.jqgfzy.top

"值: \(b)"
来源：http://pfc.cheryme.top

[T19] Swift：可选绑定
来源：http://fqg.pycfn.com

if let n = opt { print(n) }
来源：http://xma.mhx1999.top

[T20] Swift：数组操作
来源：http://jtf.fzhhl.top

var a = [1, 2, 3];  a.append(4)
来源：http://yio.yj20258.top

[T21] Swift：遍历
来源：http://zzx.zhijiandao.cn

for x in a { print(x) }
来源：http://qwr.yvedp.cn

[T22] Swift：字典
来源：http://yfn.birdmap.top

var d = ["a": 1];  d["b"] = 2
来源：http://dvl.zhiwuduotai.top

[T23] Swift：函数
来源：http://irg.jinghuilouyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kvq.tianlin.xyz

[T24] Swift：闭包
来源：http://kuk.feifeiyinyue.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lzi.bjfxy.top

[T25] Swift：结构体
来源：http://gbo.jlsjyb.cn

struct P { var x: Int }
来源：http://bae.epnwcf.com

[T26] Swift：类与重写
来源：http://ozn.smart0.xyz

class A: Base { override func f() {} }
来源：http://llw.smart0.xyz

[T27] Swift：错误处理
来源：http://ptm.yuxming.cn

do { try f() } catch { print(error) }
来源：http://jib.sysykeji.top

[T28] Swift：枚举
来源：http://nuo.quarkkingdee.top

enum Color { case red, green }
来源：http://pzs.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://htq.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://hib.yuanzhike.top

[T30] Swift：协议
来源：http://ica.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://cqe.xinyue.icu

[T31] Lua：Hello World
来源：http://uju.hywenlv.cn

print("Hello")
来源：http://hrm.chenzaomai.com

[T32] Lua：局部变量
来源：http://zep.52xcode.cn

local a = 1
来源：http://myh.jqgufenzy.top

[T33] Lua：表（数组）
来源：http://asb.jiagoushi.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kev.tian-w.cn

[T34] Lua：遍历表
来源：http://eyh.pycfn.com

for i, v in ipairs(t) do print(i, v) end
来源：http://zpy.gotoacloud.top

[T35] Lua：字典表
来源：http://skj.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://svg.ydjk.org.cn

[T36] Lua：函数
来源：http://ryv.sxryk.cn

function add(a, b) return a + b end
来源：http://gey.xinyue.icu

[T37] Lua：字符串拼接
来源：http://vnr.jinghuilouyu.cn

"a" .. "b"
来源：http://bmg.yonumen.top

[T38] Lua：条件
来源：http://dev.hongshengwenyu.top

if x > 0 then print("正") end
来源：http://fji.hysaishi.cn

[T39] Lua：模式匹配
来源：http://fwm.pycfn.com

string.find(s, "%d+")
来源：http://yog.316326.xyz

[T40] Lua：元表
来源：http://rac.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://kdp.tianlin.xyz

[T41] Perl：Hello World
来源：http://qvw.quarkkingdee.top

print "Hello\n";
来源：http://bpz.iojbl.cn

[T42] Perl：变量类型
来源：http://kjj.tian-w.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wjn.gogol.net.cn

[T43] Perl：字符串插值
来源：http://tng.redwolf501.top

"值: $a"
来源：http://ghh.daxiang520.top

[T44] Perl：条件
来源：http://evi.bjfxy.top

if ($a > 0) { print "正"; }
来源：http://utw.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://cnu.kuanghao11.cn

for my $x (@arr) { print $x; }
来源：http://vht.hcnkem.com

[T46] Perl：哈希操作
来源：http://apo.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xgs.jinghuilouyu.cn

[T47] Perl：正则捕获
来源：http://uzy.jyoumei.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://arq.shanyushiyangtech.top

[T48] Perl：正则替换
来源：http://bkh.chenzaomai.com

$s =~ s/old/new/g;
来源：http://utx.daxiang520.top

[T49] Perl：函数
来源：http://kbi.zycfv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hnd.fehbvm.com

[T50] Perl：逐行读文件
来源：http://naz.yvedp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://maw.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://bzu.quarkkingdee.top

[T51] Scala：Hello World
来源：http://imk.yj20258888.top

println("Hello")
来源：http://ygj.shanyushiyangtech.top

[T52] Scala：变量
来源：http://ttn.haohaochexian.top

val a = 1;  var b = 2
来源：http://xnm.pengpengdd.cyou

[T53] Scala：字符串插值
来源：http://gdo.vqdsnc.cn

s"值: $b"
来源：http://fyj.vehdjk.com

[T54] Scala：集合映射
来源：http://mmd.gzhubu.top

List(1, 2, 3).map(_ * 2)
来源：http://khq.xziqi.cn

[T55] Scala：集合过滤
来源：http://osm.epnwcf.com

List(1, 2, 3).filter(_ > 1)
来源：http://dts.yvedp.cn

[T56] Scala：样例类
来源：http://lan.zdqjudy.top

case class User(name: String, age: Int)
来源：http://oqg.yuanzhike.top

[T57] Scala：模式匹配
来源：http://pfu.wangshuangyany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oqd.hywenlv.cn

[T58] Scala：函数定义
来源：http://fry.tarul.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vea.gaohongyu789.top

[T59] Scala：循环
来源：http://dbi.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://zhb.xingfuxueyuan.xyz

[T60] Scala：折叠
来源：http://ofm.yj20258888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pwy.sysykeji.top

================================================================================
来源：http://nzb.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yac.yangfankeji.com

================================================================================
来源：http://sxu.ydjk.org.cn

[U01] Py：创建虚拟环境
来源：http://tuz.mhx1999.top

python -m venv .venv && source .venv/bin/activate
来源：http://rkv.vqdsnc.cn

[U02] Py：导出 / 安装依赖
来源：http://efe.hongshengwenyu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hsn.mhx1999.top

[U03] Py：加载 .env 配置
来源：http://yhx.fehbvm.com

from dotenv import load_dotenv; load_dotenv()
来源：http://dpy.jinyuanbaomall.cn

[U04] Py：变量调试打印
来源：http://fvi.aibaodan.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ihu.chenlongwang.top

[U05] Py：列表去重且保序
来源：http://uoj.pengpengdd.cyou

list(dict.fromkeys(arr))
来源：http://obl.jyoumei.cn

[U06] Py：合并两个字典
来源：http://myv.chenlongwang.top

{**a, **b}
来源：http://tok.cdnleiting.top

[U07] Py：反转字典键值
来源：http://dhq.snrcjt.cn

{v: k for k, v in d.items()}
来源：http://qpk.aizwys.cn

[U08] Py：展平二维列表
来源：http://mfw.hesvh.cn

[y for x in nested for y in x]
来源：http://bcc.jqgfzy.top

[U09] Py：字典取最大值的键
来源：http://vui.snrcjt.cn

max(d, key=d.get)
来源：http://yxt.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://bot.daxiang520.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fdx.dianchejie.cn

[U11] Py：生成器表达式
来源：http://ecp.tianlin.xyz

(x * 2 for x in arr)
来源：http://itj.tianlin.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://uig.tian-w.cn

Counter(arr).most_common(3)
来源：http://pqe.hesvh.cn

[U13] Py：固定长度队列
来源：http://lwu.jqgufenzy.top

deque(maxlen=10)
来源：http://oue.hysaishi.cn

[U14] Py：分组收集到列表
来源：http://ket.bjfxy.top

defaultdict(list)
来源：http://alm.zycfv.cn

[U15] Py：高精度计时
来源：http://zpc.jqgufenzy.top

t = time.perf_counter()
来源：http://gja.snrcjt.cn

[U16] Py：命令行参数解析
来源：http://qgh.redwolf501.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tgm.hnxiangtu.top

[U17] Py：初始化日志
来源：http://uxn.jinyuanbaomall.cn

logging.basicConfig(level=logging.INFO)
来源：http://ewx.cheryme.top

[U18] Py：预编译正则
来源：http://nbn.sufxvd.cn

pat = re.compile(r"\d+")
来源：http://nvn.yonumen.top

[U19] Py：正则替换带回调
来源：http://axs.tarul.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://znz.zhixingplan.top

[U20] Py：缓存函数结果
来源：http://ggt.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://hoj.jqgfzy.top

[U21] Py：自定义上下文管理器
来源：http://shc.cucudq.cn

@contextlib.contextmanager
来源：http://nyg.ydzc1.top

[U22] Py：矩阵转置
来源：http://rdx.jlsjyb.cn

list(zip(*m))
来源：http://mli.xuetiantiany.cn

[U23] Py：分块读取大文件
来源：http://dtx.jinghuilouyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ctr.yvedp.cn

[U24] Py：路径操作
来源：http://khw.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uih.c1oappe.top

[U25] Py：CSV 按字典读
来源：http://ugh.gotoacloud.top

csv.DictReader(f)
来源：http://ylv.fehbvm.com

[U26] Py：并发下载
来源：http://ahn.vehdjk.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hvt.fengsongda.top

[U27] Py：异步 HTTP
来源：http://tjw.jinghuilouyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://ngs.xziqi.cn

[U28] Py：类型别名
来源：http://gwp.shuidangran.top

UserId = int
来源：http://wbp.smart0.xyz

[U29] Py：属性校验
来源：http://uqk.tarul.cn

@property 与 @x.setter 配合
来源：http://tfc.ehwqpu.com

[U30] Py：数据类
来源：http://npv.shangyingyoupin.top

@dataclass(slots=True)
来源：http://hrd.tanke756.top

[U31] Py：单测
来源：http://gvp.quarkkingdee.top

python -m pytest -q
来源：http://hon.zhengqikj.top

[U32] Py：代码格式化
来源：http://nvk.ivvv.top

ruff format . && ruff check --fix .
来源：http://qwy.ydzc1.top

[U33] Py：打包发布
来源：http://iei.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://ykb.shuidangran.top

[U34] Py：判断编码
来源：http://yrb.daria6918.cn

chardet.detect(raw)
来源：http://cwm.ywan-chungtsiang.top

[U35] Py：发送邮件
来源：http://crs.hnxiangtu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mlr.sweek.top

[U36] Py：定时任务
来源：http://jzj.yongpay.top

schedule.every(10).minutes.do(job)
来源：http://skw.52xcode.cn

[U37] Py：读写 Excel
来源：http://mda.yanxiufei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jjn.c1oappe.top

[U38] Py：获取脚本所在目录
来源：http://oxg.haohaochexian.top

Path(__file__).resolve().parent
来源：http://dar.jinyuanbaomall.cn

[U39] Py：判断是否在交互环境
来源：http://kcf.zhijiandao.cn

sys.stdout.isatty()
来源：http://coa.jinqigfzy.top

[U40] Py：打印到标准错误
来源：http://vxf.guannengcc.top

print("err", file=sys.stderr)
来源：http://lse.xinyue.icu

[U41] PHP：初始化 Composer 项目
来源：http://awm.dashuyun.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://opd.daria6918.cn

[U42] PHP：PSR-4 自动加载
来源：http://kib.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zci.tanke756.top

[U43] PHP：声明命名空间
来源：http://ipe.ctjpmb.com

namespace App\Http;
来源：http://rlq.jinqigufen.top

[U44] PHP：开启严格类型
来源：http://wod.nwbrower.top

declare(strict_types=1);
来源：http://svz.jinqigfzy.top

[U45] PHP：类型声明与返回类型
来源：http://xvf.fehbvm.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://ufl.gzhubu.top

[U46] PHP：可空类型
来源：http://tcy.cashguo.top

?string $name = null
来源：http://nbh.cucudq.cn

[U47] PHP：联合类型
来源：http://opg.xingfuxueyuan.xyz

int|string $id
来源：http://zxq.zycfv.cn

[U48] PHP：纯枚举
来源：http://zth.chenlongwang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sus.zhiwuduotai.top

[U49] PHP：只读属性
来源：http://oua.birdmap.top

public readonly string $name
来源：http://sll.jqgufenzy.top

[U50] PHP：构造器属性提升
来源：http://pmn.sysykeji.top

public function __construct(private int $id) {}
来源：http://pag.fehbvm.com

[U51] PHP：数组解构
来源：http://gdu.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://jev.aibaodan.cn

[U52] PHP：箭头函数
来源：http://cle.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://obi.zhoulong.xyz

[U53] PHP：空合并运算符
来源：http://aog.0kj1m.cn

$v = $a ?? $b ?? "default";
来源：http://dvg.cdnleiting.top

[U54] PHP：空安全调用
来源：http://yyf.c1oappe.top

$obj?->method()
来源：http://aay.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://qmb.hfpthk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sar.dashuyun.cn

[U56] PHP：命名参数
来源：http://xrj.dianchejie.cn

f(a: 1, b: 2)
来源：http://led.xylfe.cn

[U57] PHP：字符串插值
来源：http://rue.nanxuanxn.top

"值: {$a}"
来源：http://akb.sweek.top

[U58] PHP：数组三件套
来源：http://axa.hfpthk.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hkw.sjlbkw.cn

[U59] PHP：自定义排序
来源：http://kyv.yvedp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rum.jqgfzy.top

[U60] PHP：JSON 编解码
来源：http://iwi.xingfuxueyuan.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jui.chenlongwang.top

[U61] PHP：正则
来源：http://zkp.ydjk.org.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ptr.uphjek.com

[U62] PHP：日期对象
来源：http://abv.quarkkingdee.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dqy.daria6918.cn

[U63] PHP：文件读写
来源：http://bev.cashguo.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://esj.smart0.xyz

[U64] PHP：目录遍历
来源：http://axr.ppjwa.cn

glob("dir/*.php");  scandir("dir");
来源：http://juw.zhaomingkeji.xyz

[U65] PHP：会话
来源：http://pgv.jlsjyb.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gws.chenjidiqi.icu

[U66] PHP：设置 Cookie
来源：http://cru.0kj1m.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lzr.zhiwuduotai.top

[U67] PHP：处理文件上传
来源：http://tfz.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pbu.ywan-chungtsiang.top

[U68] PHP：PDO 连接
来源：http://gag.jinqigufen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://veo.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://aje.pycfn.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gge.nwbrower.top

[U70] PHP：PDO 事务
来源：http://wsa.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://igj.sxryk.cn

[U71] PHP：抛出异常
来源：http://rjb.sjlbkw.cn

throw new RuntimeException("失败", 500);
来源：http://zbk.shuidangran.top

[U72] PHP：写错误日志
来源：http://nhv.shanyushiyangtech.top

error_log("失败: " . $e->getMessage());
来源：http://dzv.uphjek.com

[U73] PHP：读取 ini 配置
来源：http://wis.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://ake.zhongyouzk.top

[U74] PHP：读取环境变量
来源：http://qmd.chenjidiqi.icu

getenv("APP_ENV") ?: "production"
来源：http://huw.iojbl.cn

[U75] PHP：依赖注入
来源：http://rib.zhongyouzk.top

composer require psr/container
来源：http://iyb.daxiang520.top

[U76] PHP：简单路由
来源：http://zjl.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ikv.gzhubu.top

[U77] PHP：模板渲染
来源：http://zds.dianchejie.cn

composer require twig/twig
来源：http://zvi.tian-w.cn

[U78] PHP：单元测试
来源：http://ovl.aizwys.cn

composer require --dev phpunit/phpunit
来源：http://fbt.gogol.net.cn

[U79] PHP：静态分析
来源：http://eid.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://icj.jinghuilouyu.cn

[U80] PHP：代码规范修复
来源：http://aqh.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ccw.jinghuilouyu.cn

[U81] JS：初始化项目
来源：http://hke.sysykeji.top

npm init -y;  npm i express
来源：http://fxc.hfpthk.cn

[U82] JS：package.json 脚本
来源：http://epg.316326.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dfm.ywan-chungtsiang.top

[U83] JS：ES Module 导入导出
来源：http://guq.fzhhl.top

export const a = 1;  import { a } from "./m.js";
来源：http://yif.vqdsnc.cn

[U84] JS：CommonJS 写法
来源：http://gbf.tarul.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lol.zhijiandao.cn

[U85] JS：可选链
来源：http://std.c1oappe.top

a?.b?.c
来源：http://vsr.yj20258.top

[U86] JS：空值合并
来源：http://idp.zhoulong.xyz

a ?? b
来源：http://sud.sjlbkw.cn

[U87] JS：解构默认值
来源：http://dpi.jlsjyb.cn

const { a = 1, b = 2 } = obj;
来源：http://fgm.xinyue.icu

[U88] JS：对象展开合并
来源：http://ahz.zhijiandao.cn

{ ...a, ...b }
来源：http://cnb.gotoacloud.top

[U89] JS：数组去重
来源：http://qlj.316326.xyz

[...new Set(arr)]
来源：http://knn.dianchejie.cn

[U90] JS：数字数组排序
来源：http://rmw.yvedp.cn

[...arr].sort((a, b) => a - b)
来源：http://sli.zdbjq.cn

[U91] JS：对象键值遍历
来源：http://xih.cucudq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hxe.sufxvd.cn

[U92] JS：深拷贝
来源：http://zqp.iojbl.cn

structuredClone(obj)
来源：http://vly.chenjidiqi.icu


<!-- 参考信息 -->