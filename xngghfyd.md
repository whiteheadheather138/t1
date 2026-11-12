代发 wailian999

[T05] Kotlin：when 表达式
来源：http://lzl.yj20258888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wkv.mhx1999.top

[T06] Kotlin：集合映射
来源：http://tqs.sjlbkw.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iva.ydzc1.top

[T07] Kotlin：集合过滤
来源：http://wjd.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ngs.zhongyouzk.top

[T08] Kotlin：数据类
来源：http://qaf.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://fyy.zhiwuduotai.top

[T09] Kotlin：扩展函数
来源：http://mwx.redwolf501.top

fun String.exclaim() = this + "!"
来源：http://psz.smart0.xyz

[T10] Kotlin：默认参数
来源：http://qit.nanxuanxn.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vgu.quarkkingdee.top

[T11] Kotlin：协程
来源：http://hwz.yfazqb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://oxj.xinyue.icu

[T12] Kotlin：解构声明
来源：http://jtr.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://slm.zhoulong.xyz

[T13] Kotlin：只读 Map
来源：http://yuh.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://dqs.jlsjyb.cn

[T14] Kotlin：循环
来源：http://gbf.dashuyun.cn

for (i in 1..10) println(i)
来源：http://sqb.shuidangran.top

[T15] Kotlin：接口
来源：http://gxn.yj20258888.top

interface Shape { fun area(): Double }
来源：http://qaw.fengsongda.top

[T16] Swift：Hello World
来源：http://vdx.epnwcf.com

print("Hello")
来源：http://rkh.jyoumei.cn

[T17] Swift：变量与常量
来源：http://fgn.hfpthk.cn

var a = 1;  let b = 2
来源：http://gdb.hywenlv.cn

[T18] Swift：字符串插值
来源：http://jqm.jiagoushi.top

"值: \(b)"
来源：http://yic.zhixingplan.top

[T19] Swift：可选绑定
来源：http://fol.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://djx.yj20258.top

[T20] Swift：数组操作
来源：http://qne.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://qek.xuetiantiany.cn

[T21] Swift：遍历
来源：http://owh.sysykeji.top

for x in a { print(x) }
来源：http://sdr.tarul.cn

[T22] Swift：字典
来源：http://zky.daxiang520.top

var d = ["a": 1];  d["b"] = 2
来源：http://vak.chenjidiqi.icu

[T23] Swift：函数
来源：http://edw.hnxiangtu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://doc.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://uju.ybcxt.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yhj.chenjidiqi.icu

[T25] Swift：结构体
来源：http://jci.snrcjt.cn

struct P { var x: Int }
来源：http://yir.nwbrower.top

[T26] Swift：类与重写
来源：http://alh.jiagoushi.top

class A: Base { override func f() {} }
来源：http://hjr.nanxuanxn.top

[T27] Swift：错误处理
来源：http://gmh.meibo888.top

do { try f() } catch { print(error) }
来源：http://msp.fzhhl.top

[T28] Swift：枚举
来源：http://gay.birdmap.top

enum Color { case red, green }
来源：http://tsi.snrcjt.cn

[T29] Swift：guard 提前返回
来源：http://kqt.jianghu66.top

guard let x = opt else { return }
来源：http://ffl.birdmap.top

[T30] Swift：协议
来源：http://vyx.pycfn.com

protocol Shape { func area() -> Double }
来源：http://jtq.xylfe.cn

[T31] Lua：Hello World
来源：http://pdo.hongshengwenyu.top

print("Hello")
来源：http://svv.yj202588.top

[T32] Lua：局部变量
来源：http://lzq.vqdsnc.cn

local a = 1
来源：http://znt.smart0.xyz

[T33] Lua：表（数组）
来源：http://unh.tianlin.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://fdf.smart0.xyz

[T34] Lua：遍历表
来源：http://lce.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tjn.zhengqikj.top

[T35] Lua：字典表
来源：http://qog.sjlbkw.cn

local d = { a = 1 };  d.b = 2
来源：http://fzu.pycfn.com

[T36] Lua：函数
来源：http://hmf.hywenlv.cn

function add(a, b) return a + b end
来源：http://btk.bjfxy.top

[T37] Lua：字符串拼接
来源：http://rrk.yuanzhike.top

"a" .. "b"
来源：http://mwe.cqqwz.cn

[T38] Lua：条件
来源：http://aqi.jinqigufen.top

if x > 0 then print("正") end
来源：http://gpy.fengsongda.top

[T39] Lua：模式匹配
来源：http://qti.shanyushiyangkeji.top

string.find(s, "%d+")
来源：http://wah.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://orj.yueranfly.top

setmetatable({}, { __index = base })
来源：http://wdz.mhx1999.top

[T41] Perl：Hello World
来源：http://nka.yongpay.top

print "Hello\n";
来源：http://ygd.tian-w.cn

[T42] Perl：变量类型
来源：http://qrc.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aap.cqqwz.cn

[T43] Perl：字符串插值
来源：http://jnw.nwbrower.top

"值: $a"
来源：http://ycj.hysaishi.cn

[T44] Perl：条件
来源：http://eum.chenzaomai.com

if ($a > 0) { print "正"; }
来源：http://iek.aibaodan.cn

[T45] Perl：数组遍历
来源：http://vzq.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://zxw.tanke756.top

[T46] Perl：哈希操作
来源：http://lgs.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yey.fanxiaobao.xyz

[T47] Perl：正则捕获
来源：http://rgi.jiagoushi.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kir.jianghu66.top

[T48] Perl：正则替换
来源：http://mft.epnwcf.com

$s =~ s/old/new/g;
来源：http://tqv.jinghuilouyu.cn

[T49] Perl：函数
来源：http://iws.pycfn.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://emq.dianchejie.cn

[T50] Perl：逐行读文件
来源：http://edt.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bfa.vehdjk.com

while (my $line = <$fh>) { print $line; }
来源：http://rnu.nwbrower.top

[T51] Scala：Hello World
来源：http://vxa.cashguo.top

println("Hello")
来源：http://cxj.tianlin.xyz

[T52] Scala：变量
来源：http://mgg.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://nmf.jlsjyb.cn

[T53] Scala：字符串插值
来源：http://udv.hnqzz.top

s"值: $b"
来源：http://pur.wangshuangyany.cn

[T54] Scala：集合映射
来源：http://tvn.9152youxi.cn

List(1, 2, 3).map(_ * 2)
来源：http://kmz.hammf.cn

[T55] Scala：集合过滤
来源：http://juw.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://ocp.xingfuxueyuan.xyz

[T56] Scala：样例类
来源：http://hmv.chenzaomai.com

case class User(name: String, age: Int)
来源：http://zhb.fehbvm.com

[T57] Scala：模式匹配
来源：http://dir.zhoulong.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://lcy.bjfxy.top

[T58] Scala：函数定义
来源：http://nox.yj20258.top

def add(a: Int, b: Int): Int = a + b
来源：http://lht.yuanzhike.top

[T59] Scala：循环
来源：http://kwh.wangdashe.top

for (i <- 1 to 10) println(i)
来源：http://rpw.9152youxi.cn

[T60] Scala：折叠
来源：http://njc.xziqi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cnw.fzhhl.top

================================================================================
来源：http://ppg.kuanghao11.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jnv.shanyushiyangkeji.top

================================================================================
来源：http://rxi.zhijiandao.cn

[U01] Py：创建虚拟环境
来源：http://dfx.dashuyun.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nmd.epnwcf.com

[U02] Py：导出 / 安装依赖
来源：http://hes.snrcjt.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jje.hysaishi.cn

[U03] Py：加载 .env 配置
来源：http://ijq.zhijiandao.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ouw.52xcode.cn

[U04] Py：变量调试打印
来源：http://cdv.tanke756.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rys.tarul.cn

[U05] Py：列表去重且保序
来源：http://dus.cucudq.cn

list(dict.fromkeys(arr))
来源：http://hkn.redwolf501.top

[U06] Py：合并两个字典
来源：http://vhn.zhixingplan.top

{**a, **b}
来源：http://rwh.guowangkeji.top

[U07] Py：反转字典键值
来源：http://cxc.gaohongyu789.top

{v: k for k, v in d.items()}
来源：http://gvw.tianlin.xyz

[U08] Py：展平二维列表
来源：http://jwg.cdnleiting.top

[y for x in nested for y in x]
来源：http://mwl.smart0.xyz

[U09] Py：字典取最大值的键
来源：http://uut.jinyuanbaomall.cn

max(d, key=d.get)
来源：http://cmf.ybcxt.top

[U10] Py：按值排序字典
来源：http://qds.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gea.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://lur.jianghu66.top

(x * 2 for x in arr)
来源：http://elm.feifeiyinyue.top

[U12] Py：取出现最多的 3 个元素
来源：http://ilv.fanxiaobao.xyz

Counter(arr).most_common(3)
来源：http://anc.yanxiufei.cn

[U13] Py：固定长度队列
来源：http://gig.kuanghao11.cn

deque(maxlen=10)
来源：http://czq.nwbrower.top

[U14] Py：分组收集到列表
来源：http://azw.ydjk.org.cn

defaultdict(list)
来源：http://dot.c1oappe.top

[U15] Py：高精度计时
来源：http://kzz.jiagoushi.top

t = time.perf_counter()
来源：http://ukv.jlsjyb.cn

[U16] Py：命令行参数解析
来源：http://jup.xylfe.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ehv.nwbrower.top

[U17] Py：初始化日志
来源：http://smu.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://bse.chenlongwang.top

[U18] Py：预编译正则
来源：http://dke.sweek.top

pat = re.compile(r"\d+")
来源：http://vmp.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://lza.hesvh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oot.chenlongwang.top

[U20] Py：缓存函数结果
来源：http://ujb.cqqwz.cn

@functools.lru_cache(maxsize=None)
来源：http://myy.shuidangran.top

[U21] Py：自定义上下文管理器
来源：http://jno.shangyingyoupin.top

@contextlib.contextmanager
来源：http://btl.jlsjyb.cn

[U22] Py：矩阵转置
来源：http://fno.yj20258.top

list(zip(*m))
来源：http://xlc.daxiang520.top

[U23] Py：分块读取大文件
来源：http://jyo.wangdashe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gjr.shanyushiyangkeji.top

[U24] Py：路径操作
来源：http://ljx.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sjl.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://smv.yuxming.cn

csv.DictReader(f)
来源：http://aym.jinqigufen.top

[U26] Py：并发下载
来源：http://fac.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wfo.yonumen.top

[U27] Py：异步 HTTP
来源：http://wqa.birdmap.top

aiohttp.ClientSession() 配合 async with
来源：http://lmp.kuanghao11.cn

[U28] Py：类型别名
来源：http://xpz.zhaomingkeji.xyz

UserId = int
来源：http://iqi.zhiwuduotai.top

[U29] Py：属性校验
来源：http://nfy.yj202588.top

@property 与 @x.setter 配合
来源：http://vvb.chenzaomai.com

[U30] Py：数据类
来源：http://och.hfpthk.cn

@dataclass(slots=True)
来源：http://ibi.wangdashe.top

[U31] Py：单测
来源：http://sae.xylfe.cn

python -m pytest -q
来源：http://hck.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://vcm.sweek.top

ruff format . && ruff check --fix .
来源：http://pyg.daxiang520.top

[U33] Py：打包发布
来源：http://xjb.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://wyd.shanyushiyangkeji.top

[U34] Py：判断编码
来源：http://zah.jinqigfzy.top

chardet.detect(raw)
来源：http://wqf.fengsongda.top

[U35] Py：发送邮件
来源：http://qvd.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://imb.dashuyun.cn

[U36] Py：定时任务
来源：http://mwh.quarkkingdee.top

schedule.every(10).minutes.do(job)
来源：http://cnt.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://boz.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://chx.fzhhl.top

[U38] Py：获取脚本所在目录
来源：http://mdz.guowangkeji.top

Path(__file__).resolve().parent
来源：http://dhp.zdqjudy.top

[U39] Py：判断是否在交互环境
来源：http://rhz.sjlbkw.cn

sys.stdout.isatty()
来源：http://zdi.chenjidiqi.icu

[U40] Py：打印到标准错误
来源：http://nvu.xuanzx.com

print("err", file=sys.stderr)
来源：http://ifb.jianghu66.top

[U41] PHP：初始化 Composer 项目
来源：http://juy.jianghu66.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cyf.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://edg.zdqjudy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mrg.zdbjq.cn

[U43] PHP：声明命名空间
来源：http://fcz.52xcode.cn

namespace App\Http;
来源：http://hwo.chenlongwang.top

[U44] PHP：开启严格类型
来源：http://fgc.shanyushiyangkeji.top

declare(strict_types=1);
来源：http://fiu.hywenlv.cn

[U45] PHP：类型声明与返回类型
来源：http://jvi.gotoacloud.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://usl.wangdashe.top

[U46] PHP：可空类型
来源：http://whx.hammf.cn

?string $name = null
来源：http://qef.hysaishi.cn

[U47] PHP：联合类型
来源：http://cok.yfazqb.com

int|string $id
来源：http://tvi.yueranfly.top

[U48] PHP：纯枚举
来源：http://dmh.vqdsnc.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jmr.gotoacloud.top

[U49] PHP：只读属性
来源：http://gny.haohaochexian.top

public readonly string $name
来源：http://ibq.jyoumei.cn

[U50] PHP：构造器属性提升
来源：http://qlp.zdbjq.cn

public function __construct(private int $id) {}
来源：http://myr.hnqzz.top

[U51] PHP：数组解构
来源：http://zhw.c1oappe.top

[$a, $b] = $arr;
来源：http://yzv.jinyuanbaomall.cn

[U52] PHP：箭头函数
来源：http://exa.zhongyouzk.top

$double = fn($x) => $x * 2;
来源：http://vti.vehdjk.com

[U53] PHP：空合并运算符
来源：http://qtf.ctjpmb.com

$v = $a ?? $b ?? "default";
来源：http://alz.yj202588.top

[U54] PHP：空安全调用
来源：http://nmy.cucudq.cn

$obj?->method()
来源：http://jlk.316326.xyz

[U55] PHP：match 表达式
来源：http://pga.gaohongyu789.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qdj.xylfe.cn

[U56] PHP：命名参数
来源：http://zuj.gotoacloud.top

f(a: 1, b: 2)
来源：http://otw.hongshengwenyu.top

[U57] PHP：字符串插值
来源：http://sjz.cqqwz.cn

"值: {$a}"
来源：http://kbg.zhengqikj.top

[U58] PHP：数组三件套
来源：http://qwo.zhengqikj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ivr.ppjwa.cn

[U59] PHP：自定义排序
来源：http://xfo.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bih.ywan-chungtsiang.top

[U60] PHP：JSON 编解码
来源：http://kae.meibo888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://soj.ydjk.org.cn

[U61] PHP：正则
来源：http://vch.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vvu.zycfv.cn

[U62] PHP：日期对象
来源：http://gae.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fuq.c1oappe.top

[U63] PHP：文件读写
来源：http://kwl.ehwqpu.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ult.jinghuilouyu.cn

[U64] PHP：目录遍历
来源：http://czo.feifeiyinyue.top

glob("dir/*.php");  scandir("dir");
来源：http://wyn.yj20258.top

[U65] PHP：会话
来源：http://jig.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fxj.fanxiaobao.xyz

[U66] PHP：设置 Cookie
来源：http://ywg.jinyuanbaomall.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lyr.shzxlz.cn

[U67] PHP：处理文件上传
来源：http://fpz.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://otr.jianghu66.top

[U68] PHP：PDO 连接
来源：http://gwa.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zdl.xziqi.cn

[U69] PHP：PDO 预处理
来源：http://wwc.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jcc.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://iyo.xziqi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://awj.sjlbkw.cn

[U71] PHP：抛出异常
来源：http://kdd.meibo888.top

throw new RuntimeException("失败", 500);
来源：http://non.shzxlz.cn

[U72] PHP：写错误日志
来源：http://qoi.jyoumei.cn

error_log("失败: " . $e->getMessage());
来源：http://qgi.guannengcc.top

[U73] PHP：读取 ini 配置
来源：http://oeg.aibaodan.cn

parse_ini_file("config.ini", true)
来源：http://xps.birdmap.top

[U74] PHP：读取环境变量
来源：http://glt.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://eap.ppjwa.cn

[U75] PHP：依赖注入
来源：http://rve.gaohongyu789.top

composer require psr/container
来源：http://kdn.andypj.xyz

[U76] PHP：简单路由
来源：http://hod.jqgufenzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dmh.cucudq.cn

[U77] PHP：模板渲染
来源：http://tqe.nanxuanxn.top

composer require twig/twig
来源：http://ebq.fktsv.cn

[U78] PHP：单元测试
来源：http://kwr.ctjpmb.com

composer require --dev phpunit/phpunit
来源：http://vzo.dashuyun.cn

[U79] PHP：静态分析
来源：http://zyk.9152youxi.cn

composer require --dev phpstan/phpstan
来源：http://ebn.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://wfq.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lvg.sxryk.cn

[U81] JS：初始化项目
来源：http://ghj.shangyingyoupin.top

npm init -y;  npm i express
来源：http://wyz.aizwys.cn

[U82] JS：package.json 脚本
来源：http://wnj.fehbvm.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tto.haohaochexian.top

[U83] JS：ES Module 导入导出
来源：http://sch.xylfe.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fqr.cdnleiting.top

[U84] JS：CommonJS 写法
来源：http://fez.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uek.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://nwm.yueranfly.top

a?.b?.c
来源：http://oeh.aizwys.cn

[U86] JS：空值合并
来源：http://wyj.jinghuilouyu.cn

a ?? b
来源：http://crj.yuanzhike.top

[U87] JS：解构默认值
来源：http://izv.ehwqpu.com

const { a = 1, b = 2 } = obj;
来源：http://gxa.jinqigufen.top

[U88] JS：对象展开合并
来源：http://lgy.chenzaomai.com

{ ...a, ...b }
来源：http://zog.fanxiaobao.xyz

[U89] JS：数组去重
来源：http://siv.iojbl.cn

[...new Set(arr)]
来源：http://ptr.pycfn.com

[U90] JS：数字数组排序
来源：http://dlu.xingfuxueyuan.xyz

[...arr].sort((a, b) => a - b)
来源：http://yxw.fktsv.cn

[U91] JS：对象键值遍历
来源：http://jhl.yangfankeji.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fuc.gaohongyu789.top

[U92] JS：深拷贝
来源：http://pql.xylfe.cn

structuredClone(obj)
来源：http://zai.sxryk.cn


<!-- 参考信息 -->