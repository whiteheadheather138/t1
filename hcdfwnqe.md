代发 wailian999

[T05] Kotlin：when 表达式
来源：http://ioy.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uiy.yonumen.top

[T06] Kotlin：集合映射
来源：http://dye.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://frv.jinyuanbaomall.cn

[T07] Kotlin：集合过滤
来源：http://kbu.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xtp.jyoumei.cn

[T08] Kotlin：数据类
来源：http://rqk.hcnkem.com

data class User(val name: String, val age: Int)
来源：http://rpe.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://zqd.yvedp.cn

fun String.exclaim() = this + "!"
来源：http://vnq.mhx1999.top

[T10] Kotlin：默认参数
来源：http://xfl.jinqigfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rbh.nanxinkj.top

[T11] Kotlin：协程
来源：http://yos.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bwd.fktsv.cn

[T12] Kotlin：解构声明
来源：http://bea.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://twj.hnqzz.top

[T13] Kotlin：只读 Map
来源：http://uoe.jiagoushi.top

val m = mapOf("a" to 1)
来源：http://ksd.nwbrower.top

[T14] Kotlin：循环
来源：http://nsm.uphjek.com

for (i in 1..10) println(i)
来源：http://gce.zhixingplan.top

[T15] Kotlin：接口
来源：http://wpp.yueranfly.top

interface Shape { fun area(): Double }
来源：http://mkb.yongpay.top

[T16] Swift：Hello World
来源：http://uxn.ppjwa.cn

print("Hello")
来源：http://fzt.zhengqikj.top

[T17] Swift：变量与常量
来源：http://cji.zhixingplan.top

var a = 1;  let b = 2
来源：http://zwo.jyoumei.cn

[T18] Swift：字符串插值
来源：http://pfr.tarul.cn

"值: \(b)"
来源：http://gnl.ydjk.org.cn

[T19] Swift：可选绑定
来源：http://zwb.hammf.cn

if let n = opt { print(n) }
来源：http://eoo.ehwqpu.com

[T20] Swift：数组操作
来源：http://chu.ctjpmb.com

var a = [1, 2, 3];  a.append(4)
来源：http://fno.yj202588.top

[T21] Swift：遍历
来源：http://tcx.yongpay.top

for x in a { print(x) }
来源：http://ord.yuanzhike.top

[T22] Swift：字典
来源：http://qqc.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pja.316326.xyz

[T23] Swift：函数
来源：http://fgx.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ogm.tanke756.top

[T24] Swift：闭包
来源：http://woc.andypj.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://vaa.yvedp.cn

[T25] Swift：结构体
来源：http://jkx.zdqjudy.top

struct P { var x: Int }
来源：http://nkl.fehbvm.com

[T26] Swift：类与重写
来源：http://efo.0kj1m.cn

class A: Base { override func f() {} }
来源：http://qsz.gaohongyu789.top

[T27] Swift：错误处理
来源：http://nnm.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://teu.tianlin.xyz

[T28] Swift：枚举
来源：http://uyt.iojbl.cn

enum Color { case red, green }
来源：http://ymr.yonumen.top

[T29] Swift：guard 提前返回
来源：http://dgy.ivvv.top

guard let x = opt else { return }
来源：http://prn.hcnkem.com

[T30] Swift：协议
来源：http://chn.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://zhe.yanxiufei.cn

[T31] Lua：Hello World
来源：http://qfs.hongshengwenyu.top

print("Hello")
来源：http://jrv.yvedp.cn

[T32] Lua：局部变量
来源：http://zlo.ydjk.org.cn

local a = 1
来源：http://jdb.jqgufenzy.top

[T33] Lua：表（数组）
来源：http://imp.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://svt.ybcxt.top

[T34] Lua：遍历表
来源：http://pwy.svipenyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lsp.tianlin.xyz

[T35] Lua：字典表
来源：http://dbi.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://jqc.hongshengwenyu.top

[T36] Lua：函数
来源：http://brh.bjfxy.top

function add(a, b) return a + b end
来源：http://zvg.svipenyu.cn

[T37] Lua：字符串拼接
来源：http://ghy.yj20258.top

"a" .. "b"
来源：http://xna.gogol.net.cn

[T38] Lua：条件
来源：http://xoc.fengsongda.top

if x > 0 then print("正") end
来源：http://wpf.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://hbs.cdnleiting.top

string.find(s, "%d+")
来源：http://agf.sysykeji.top

[T40] Lua：元表
来源：http://rbr.smart0.xyz

setmetatable({}, { __index = base })
来源：http://qxb.hnxiangtu.top

[T41] Perl：Hello World
来源：http://lmj.wangdashe.top

print "Hello\n";
来源：http://ols.zhongyouzk.top

[T42] Perl：变量类型
来源：http://zgh.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jpr.yueranfly.top

[T43] Perl：字符串插值
来源：http://zmo.kuanghao11.cn

"值: $a"
来源：http://gbu.nanxuanxn.top

[T44] Perl：条件
来源：http://zfy.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://qtu.guowangkeji.top

[T45] Perl：数组遍历
来源：http://dmq.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://bvn.shangyingyoupin.top

[T46] Perl：哈希操作
来源：http://you.redwolf501.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aze.xylfe.cn

[T47] Perl：正则捕获
来源：http://zfy.snrcjt.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ork.fzhhl.top

[T48] Perl：正则替换
来源：http://jkb.yonumen.top

$s =~ s/old/new/g;
来源：http://djq.andypj.xyz

[T49] Perl：函数
来源：http://eio.jqgufenzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ije.cashguo.top

[T50] Perl：逐行读文件
来源：http://nxy.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://kkk.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://lqm.gaohongyu789.top

[T51] Scala：Hello World
来源：http://gtg.52xcode.cn

println("Hello")
来源：http://duu.iojbl.cn

[T52] Scala：变量
来源：http://bsa.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://rap.zdqjudy.top

[T53] Scala：字符串插值
来源：http://ucz.smart0.xyz

s"值: $b"
来源：http://zjt.hysaishi.cn

[T54] Scala：集合映射
来源：http://dwu.hongshengwenyu.top

List(1, 2, 3).map(_ * 2)
来源：http://qre.yongpay.top

[T55] Scala：集合过滤
来源：http://fou.jqgufenzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://ihn.snrcjt.cn

[T56] Scala：样例类
来源：http://icb.vehdjk.com

case class User(name: String, age: Int)
来源：http://ujd.feifeiyinyue.top

[T57] Scala：模式匹配
来源：http://lbi.guannengcc.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://cvb.yvedp.cn

[T58] Scala：函数定义
来源：http://prx.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://wwb.jinqigufen.top

[T59] Scala：循环
来源：http://qfb.guannengcc.top

for (i <- 1 to 10) println(i)
来源：http://gnm.yangfankeji.com

[T60] Scala：折叠
来源：http://eoc.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tim.daria6918.cn

================================================================================
来源：http://sfq.wangdashe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vqc.svipenyu.cn

================================================================================
来源：http://atl.chenlongwang.top

[U01] Py：创建虚拟环境
来源：http://lqh.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://tph.yj20258.top

[U02] Py：导出 / 安装依赖
来源：http://gjp.tanke756.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://utn.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://irc.gaohongyu789.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wum.zhiwuduotai.top

[U04] Py：变量调试打印
来源：http://hgy.hnxiangtu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wdb.bjfxy.top

[U05] Py：列表去重且保序
来源：http://nkc.yvedp.cn

list(dict.fromkeys(arr))
来源：http://svl.sysykeji.top

[U06] Py：合并两个字典
来源：http://dup.jinghuilouyu.cn

{**a, **b}
来源：http://mzt.mhx1999.top

[U07] Py：反转字典键值
来源：http://rcc.ydjk.org.cn

{v: k for k, v in d.items()}
来源：http://frl.zhaomingkeji.xyz

[U08] Py：展平二维列表
来源：http://bbe.ivvv.top

[y for x in nested for y in x]
来源：http://kzj.jqgfzy.top

[U09] Py：字典取最大值的键
来源：http://xat.quarkkingdee.top

max(d, key=d.get)
来源：http://pdg.hnqzz.top

[U10] Py：按值排序字典
来源：http://zsv.chenjidiqi.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://apb.hesvh.cn

[U11] Py：生成器表达式
来源：http://vtg.jinghuilouyu.cn

(x * 2 for x in arr)
来源：http://zlt.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://cgh.yj20258888.top

Counter(arr).most_common(3)
来源：http://xwa.epnwcf.com

[U13] Py：固定长度队列
来源：http://pvv.shanyushiyangkeji.top

deque(maxlen=10)
来源：http://guc.52xcode.cn

[U14] Py：分组收集到列表
来源：http://rdp.jqgufenzy.top

defaultdict(list)
来源：http://mcj.zdbjq.cn

[U15] Py：高精度计时
来源：http://gvh.yueranfly.top

t = time.perf_counter()
来源：http://dbi.jqgufenzy.top

[U16] Py：命令行参数解析
来源：http://fph.ehwqpu.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lbt.ydjk.org.cn

[U17] Py：初始化日志
来源：http://uhf.tianlin.xyz

logging.basicConfig(level=logging.INFO)
来源：http://uzx.andypj.xyz

[U18] Py：预编译正则
来源：http://ovl.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://opb.tian-w.cn

[U19] Py：正则替换带回调
来源：http://fre.aibaodan.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mkx.cashguo.top

[U20] Py：缓存函数结果
来源：http://uho.dianchejie.cn

@functools.lru_cache(maxsize=None)
来源：http://car.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://uqh.ydzc1.top

@contextlib.contextmanager
来源：http://hvk.epnwcf.com

[U22] Py：矩阵转置
来源：http://upe.hesvh.cn

list(zip(*m))
来源：http://sax.yangfankeji.com

[U23] Py：分块读取大文件
来源：http://pdc.daxiang520.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cxm.chenjidiqi.icu

[U24] Py：路径操作
来源：http://cui.fengsongda.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://etp.gzhubu.top

[U25] Py：CSV 按字典读
来源：http://gpc.tianlin.xyz

csv.DictReader(f)
来源：http://pmm.cheryme.top

[U26] Py：并发下载
来源：http://dzw.ivvv.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ulg.zhijiandao.cn

[U27] Py：异步 HTTP
来源：http://yxs.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://sbi.wangdashe.top

[U28] Py：类型别名
来源：http://uvs.fehbvm.com

UserId = int
来源：http://egl.yuxming.cn

[U29] Py：属性校验
来源：http://fyo.bjfxy.top

@property 与 @x.setter 配合
来源：http://xfm.zhixingplan.top

[U30] Py：数据类
来源：http://fyv.uphjek.com

@dataclass(slots=True)
来源：http://hkn.jlsjyb.cn

[U31] Py：单测
来源：http://jta.xylfe.cn

python -m pytest -q
来源：http://kwp.jyoumei.cn

[U32] Py：代码格式化
来源：http://stu.andypj.xyz

ruff format . && ruff check --fix .
来源：http://xth.daxiang520.top

[U33] Py：打包发布
来源：http://pit.jinqigufen.top

python -m build  （依赖 pyproject.toml）
来源：http://hom.jyoumei.cn

[U34] Py：判断编码
来源：http://fjo.yanxiufei.cn

chardet.detect(raw)
来源：http://dyi.snrcjt.cn

[U35] Py：发送邮件
来源：http://djv.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sff.dashuyun.cn

[U36] Py：定时任务
来源：http://ibv.pycfn.com

schedule.every(10).minutes.do(job)
来源：http://bts.xuetiantiany.cn

[U37] Py：读写 Excel
来源：http://bbh.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://fjx.birdmap.top

[U38] Py：获取脚本所在目录
来源：http://pba.snrcjt.cn

Path(__file__).resolve().parent
来源：http://dyw.nanxuanxn.top

[U39] Py：判断是否在交互环境
来源：http://qah.wangshuangyany.cn

sys.stdout.isatty()
来源：http://uzp.chenzaomai.com

[U40] Py：打印到标准错误
来源：http://bjj.vehdjk.com

print("err", file=sys.stderr)
来源：http://bui.jinqigfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://ciz.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ezp.zhoulong.xyz

[U42] PHP：PSR-4 自动加载
来源：http://juo.guannengcc.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cnr.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://kuo.jinqigufen.top

namespace App\Http;
来源：http://ovk.vehdjk.com

[U44] PHP：开启严格类型
来源：http://lwu.xziqi.cn

declare(strict_types=1);
来源：http://mwf.bjfxy.top

[U45] PHP：类型声明与返回类型
来源：http://nng.birdmap.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gea.jinyuanbaomall.cn

[U46] PHP：可空类型
来源：http://dxz.hywenlv.cn

?string $name = null
来源：http://oxk.cashguo.top

[U47] PHP：联合类型
来源：http://jvi.zycfv.cn

int|string $id
来源：http://qcd.yuxming.cn

[U48] PHP：纯枚举
来源：http://trt.fanxiaobao.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ouj.shzxlz.cn

[U49] PHP：只读属性
来源：http://sxf.gotoacloud.top

public readonly string $name
来源：http://gzn.yj20258888.top

[U50] PHP：构造器属性提升
来源：http://rvo.ydzc1.top

public function __construct(private int $id) {}
来源：http://dmy.aizwys.cn

[U51] PHP：数组解构
来源：http://xzt.shzxlz.cn

[$a, $b] = $arr;
来源：http://tig.yfazqb.com

[U52] PHP：箭头函数
来源：http://uox.ydzc1.top

$double = fn($x) => $x * 2;
来源：http://kwh.zhijiandao.cn

[U53] PHP：空合并运算符
来源：http://fzg.fanxiaobao.xyz

$v = $a ?? $b ?? "default";
来源：http://qzi.daxiang520.top

[U54] PHP：空安全调用
来源：http://knv.sxryk.cn

$obj?->method()
来源：http://ktn.yj20258888.top

[U55] PHP：match 表达式
来源：http://rlf.xuetiantiany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://trk.meibo888.top

[U56] PHP：命名参数
来源：http://nwj.hammf.cn

f(a: 1, b: 2)
来源：http://gew.9152youxi.cn

[U57] PHP：字符串插值
来源：http://fkr.andypj.xyz

"值: {$a}"
来源：http://uxf.yueranfly.top

[U58] PHP：数组三件套
来源：http://spf.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kme.chenzaomai.com

[U59] PHP：自定义排序
来源：http://lcn.yonumen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cln.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://sps.sxryk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lnd.jyoumei.cn

[U61] PHP：正则
来源：http://zel.ywan-chungtsiang.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nzg.daria6918.cn

[U62] PHP：日期对象
来源：http://ayo.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lav.redwolf501.top

[U63] PHP：文件读写
来源：http://jcu.haohaochexian.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ema.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://gfe.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://jyd.hywenlv.cn

[U65] PHP：会话
来源：http://vcc.xuetiantiany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zph.havefunace.top

[U66] PHP：设置 Cookie
来源：http://ees.feifeiyinyue.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://acn.hcnkem.com

[U67] PHP：处理文件上传
来源：http://czp.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iuo.0kj1m.cn

[U68] PHP：PDO 连接
来源：http://vjv.daxiang520.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ywz.316326.xyz

[U69] PHP：PDO 预处理
来源：http://lov.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hrw.redwolf501.top

[U70] PHP：PDO 事务
来源：http://zeb.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://axr.hammf.cn

[U71] PHP：抛出异常
来源：http://sjw.smart0.xyz

throw new RuntimeException("失败", 500);
来源：http://knl.0kj1m.cn

[U72] PHP：写错误日志
来源：http://rtz.c1oappe.top

error_log("失败: " . $e->getMessage());
来源：http://sdq.zhixingplan.top

[U73] PHP：读取 ini 配置
来源：http://pro.ivvv.top

parse_ini_file("config.ini", true)
来源：http://hct.0kj1m.cn

[U74] PHP：读取环境变量
来源：http://cnx.cdnleiting.top

getenv("APP_ENV") ?: "production"
来源：http://wim.jyoumei.cn

[U75] PHP：依赖注入
来源：http://vuj.jyoumei.cn

composer require psr/container
来源：http://djh.jyoumei.cn

[U76] PHP：简单路由
来源：http://hxl.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pvp.mhx1999.top

[U77] PHP：模板渲染
来源：http://osz.nanxinkj.top

composer require twig/twig
来源：http://zbt.shanyushiyangtech.top

[U78] PHP：单元测试
来源：http://nlm.yj202588.top

composer require --dev phpunit/phpunit
来源：http://pun.tian-w.cn

[U79] PHP：静态分析
来源：http://tsf.tanke756.top

composer require --dev phpstan/phpstan
来源：http://fci.zhiwuduotai.top

[U80] PHP：代码规范修复
来源：http://hst.xziqi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://boq.mhx1999.top

[U81] JS：初始化项目
来源：http://eqw.dashuyun.cn

npm init -y;  npm i express
来源：http://xxs.epnwcf.com

[U82] JS：package.json 脚本
来源：http://ywq.kuanghao11.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bht.zhongyouzk.top

[U83] JS：ES Module 导入导出
来源：http://dkh.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ixx.hammf.cn

[U84] JS：CommonJS 写法
来源：http://wln.ywan-chungtsiang.top

module.exports = { a };  const { a } = require("./m");
来源：http://pkb.hesvh.cn

[U85] JS：可选链
来源：http://xwz.0kj1m.cn

a?.b?.c
来源：http://aim.xingfuxueyuan.xyz

[U86] JS：空值合并
来源：http://gci.cucudq.cn

a ?? b
来源：http://hjf.fzhhl.top

[U87] JS：解构默认值
来源：http://swq.snrcjt.cn

const { a = 1, b = 2 } = obj;
来源：http://zat.yonumen.top

[U88] JS：对象展开合并
来源：http://wjv.hfpthk.cn

{ ...a, ...b }
来源：http://euu.zhaomingkeji.xyz

[U89] JS：数组去重
来源：http://zxx.kuanghao11.cn

[...new Set(arr)]
来源：http://naa.shzxlz.cn

[U90] JS：数字数组排序
来源：http://cyx.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://dwd.svipenyu.cn

[U91] JS：对象键值遍历
来源：http://wlu.guowangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pwv.shanyushiyangkeji.top

[U92] JS：深拷贝
来源：http://syh.316326.xyz

structuredClone(obj)
来源：http://qyd.zhengqikj.top


<!-- 参考信息 -->