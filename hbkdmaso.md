代发 wailian999

[T01] Kotlin：Hello World
来源：http://ewp.nwbrower.top

println("Hello")
来源：http://lsc.cucudq.cn

[T02] Kotlin：变量
来源：http://bqb.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://evo.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://qvp.uphjek.com

"值: $b"
来源：http://vph.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://njl.vehdjk.com

val n: String? = null;  n?.length
来源：http://bsu.havefunace.top

[T05] Kotlin：when 表达式
来源：http://zii.shzxlz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bfe.redwolf501.top

[T06] Kotlin：集合映射
来源：http://sjz.pycfn.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ojh.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://ejz.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yhg.zdqjudy.top

[T08] Kotlin：数据类
来源：http://wos.cheryme.top

data class User(val name: String, val age: Int)
来源：http://sak.sweek.top

[T09] Kotlin：扩展函数
来源：http://jnc.hesvh.cn

fun String.exclaim() = this + "!"
来源：http://mch.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://mib.uphjek.com

fun greet(name: String = "World") = "Hi $name"
来源：http://hxw.tianlin.xyz

[T11] Kotlin：协程
来源：http://vrd.hfpthk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nxh.tian-w.cn

[T12] Kotlin：解构声明
来源：http://zyq.yj20258888.top

val (a, b) = Pair(1, 2)
来源：http://seg.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://gyt.yonumen.top

val m = mapOf("a" to 1)
来源：http://ksf.chenzaomai.com

[T14] Kotlin：循环
来源：http://jgr.tianlin.xyz

for (i in 1..10) println(i)
来源：http://zaj.sjlbkw.cn

[T15] Kotlin：接口
来源：http://kck.kuanghao11.cn

interface Shape { fun area(): Double }
来源：http://qfy.feifeiyinyue.top

[T16] Swift：Hello World
来源：http://cwz.bjfxy.top

print("Hello")
来源：http://bpr.yuanzhike.top

[T17] Swift：变量与常量
来源：http://pxu.kuanghao11.cn

var a = 1;  let b = 2
来源：http://muh.bjfxy.top

[T18] Swift：字符串插值
来源：http://shk.shzxlz.cn

"值: \(b)"
来源：http://xym.ybcxt.top

[T19] Swift：可选绑定
来源：http://eps.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://qct.ydzc1.top

[T20] Swift：数组操作
来源：http://emw.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://caz.sjlbkw.cn

[T21] Swift：遍历
来源：http://jzv.yj20258.top

for x in a { print(x) }
来源：http://xjt.gaohongyu789.top

[T22] Swift：字典
来源：http://gyk.guannengcc.top

var d = ["a": 1];  d["b"] = 2
来源：http://tse.sjlbkw.cn

[T23] Swift：函数
来源：http://pbk.smart0.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zax.epnwcf.com

[T24] Swift：闭包
来源：http://lhh.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tyw.ivvv.top

[T25] Swift：结构体
来源：http://zxq.yj20258.top

struct P { var x: Int }
来源：http://bum.kuanghao11.cn

[T26] Swift：类与重写
来源：http://ygc.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://qhi.sysykeji.top

[T27] Swift：错误处理
来源：http://qkz.andypj.xyz

do { try f() } catch { print(error) }
来源：http://qfq.tian-w.cn

[T28] Swift：枚举
来源：http://rii.52xcode.cn

enum Color { case red, green }
来源：http://rro.iojbl.cn

[T29] Swift：guard 提前返回
来源：http://ian.fengsongda.top

guard let x = opt else { return }
来源：http://dqa.daxiang520.top

[T30] Swift：协议
来源：http://omq.zhixingplan.top

protocol Shape { func area() -> Double }
来源：http://lsk.nanxuanxn.top

[T31] Lua：Hello World
来源：http://vtb.meibo888.top

print("Hello")
来源：http://nht.guannengcc.top

[T32] Lua：局部变量
来源：http://cvk.birdmap.top

local a = 1
来源：http://fzx.cucudq.cn

[T33] Lua：表（数组）
来源：http://zjt.zhaomingkeji.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://fld.dianchejie.cn

[T34] Lua：遍历表
来源：http://mtm.wangdashe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ayr.shangyingyoupin.top

[T35] Lua：字典表
来源：http://iju.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://zkc.chenzaomai.com

[T36] Lua：函数
来源：http://xql.yj20258.top

function add(a, b) return a + b end
来源：http://brw.kuanghao11.cn

[T37] Lua：字符串拼接
来源：http://ihg.ydzc1.top

"a" .. "b"
来源：http://eny.hnqzz.top

[T38] Lua：条件
来源：http://bsg.uphjek.com

if x > 0 then print("正") end
来源：http://lbk.shzxlz.cn

[T39] Lua：模式匹配
来源：http://sqp.ppjwa.cn

string.find(s, "%d+")
来源：http://pad.shzxlz.cn

[T40] Lua：元表
来源：http://cmz.yueranfly.top

setmetatable({}, { __index = base })
来源：http://nge.daxiang520.top

[T41] Perl：Hello World
来源：http://cpo.birdmap.top

print "Hello\n";
来源：http://tfg.bjfxy.top

[T42] Perl：变量类型
来源：http://hli.tian-w.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tcw.jqgfzy.top

[T43] Perl：字符串插值
来源：http://was.jyoumei.cn

"值: $a"
来源：http://juq.fanxiaobao.xyz

[T44] Perl：条件
来源：http://ank.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://ncj.fanxiaobao.xyz

[T45] Perl：数组遍历
来源：http://jxf.ivvv.top

for my $x (@arr) { print $x; }
来源：http://vjr.aizwys.cn

[T46] Perl：哈希操作
来源：http://bzq.shanyushiyangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gtg.hnqzz.top

[T47] Perl：正则捕获
来源：http://nkl.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://hih.ywan-chungtsiang.top

[T48] Perl：正则替换
来源：http://pwx.316326.xyz

$s =~ s/old/new/g;
来源：http://amp.svipenyu.cn

[T49] Perl：函数
来源：http://whz.fengsongda.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aup.jinqigufen.top

[T50] Perl：逐行读文件
来源：http://dis.tian-w.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://eyy.zhaomingkeji.xyz

while (my $line = <$fh>) { print $line; }
来源：http://iod.zdqjudy.top

[T51] Scala：Hello World
来源：http://ujg.aibaodan.cn

println("Hello")
来源：http://lfm.yonumen.top

[T52] Scala：变量
来源：http://lfy.ydjk.org.cn

val a = 1;  var b = 2
来源：http://syu.sweek.top

[T53] Scala：字符串插值
来源：http://fkm.c1oappe.top

s"值: $b"
来源：http://oon.hywenlv.cn

[T54] Scala：集合映射
来源：http://loz.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://icp.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://aew.shzxlz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://azp.ybcxt.top

[T56] Scala：样例类
来源：http://tam.vehdjk.com

case class User(name: String, age: Int)
来源：http://yso.daxiang520.top

[T57] Scala：模式匹配
来源：http://mfe.xziqi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xxw.shanyushiyangkeji.top

[T58] Scala：函数定义
来源：http://fuv.zhixingplan.top

def add(a: Int, b: Int): Int = a + b
来源：http://mxo.nwbrower.top

[T59] Scala：循环
来源：http://xvp.hysaishi.cn

for (i <- 1 to 10) println(i)
来源：http://cuf.ctjpmb.com

[T60] Scala：折叠
来源：http://wmw.gaohongyu789.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lyt.jqgufenzy.top

================================================================================
来源：http://jiw.aizwys.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bgg.vehdjk.com

================================================================================
来源：http://mdh.zycfv.cn

[U01] Py：创建虚拟环境
来源：http://ekc.haohaochexian.top

python -m venv .venv && source .venv/bin/activate
来源：http://xvr.ivvv.top

[U02] Py：导出 / 安装依赖
来源：http://msy.epnwcf.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hpr.hongshengwenyu.top

[U03] Py：加载 .env 配置
来源：http://qhs.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gts.epnwcf.com

[U04] Py：变量调试打印
来源：http://rwj.xingfuxueyuan.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://efc.jlsjyb.cn

[U05] Py：列表去重且保序
来源：http://xjn.gogol.net.cn

list(dict.fromkeys(arr))
来源：http://pkw.guowangkeji.top

[U06] Py：合并两个字典
来源：http://vzx.yfazqb.com

{**a, **b}
来源：http://erv.tarul.cn

[U07] Py：反转字典键值
来源：http://onu.vehdjk.com

{v: k for k, v in d.items()}
来源：http://vth.9152youxi.cn

[U08] Py：展平二维列表
来源：http://rwp.bbcook.cn

[y for x in nested for y in x]
来源：http://owg.gaohongyu789.top

[U09] Py：字典取最大值的键
来源：http://nlu.hnqzz.top

max(d, key=d.get)
来源：http://qbd.hammf.cn

[U10] Py：按值排序字典
来源：http://dfz.wangdashe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cmq.ehwqpu.com

[U11] Py：生成器表达式
来源：http://ouz.sysykeji.top

(x * 2 for x in arr)
来源：http://nlk.zdqjudy.top

[U12] Py：取出现最多的 3 个元素
来源：http://qhc.yangfankeji.com

Counter(arr).most_common(3)
来源：http://hwa.redwolf501.top

[U13] Py：固定长度队列
来源：http://frz.jiagoushi.top

deque(maxlen=10)
来源：http://zhu.chenzaomai.com

[U14] Py：分组收集到列表
来源：http://dca.ctjpmb.com

defaultdict(list)
来源：http://gwa.epnwcf.com

[U15] Py：高精度计时
来源：http://bui.jqgfzy.top

t = time.perf_counter()
来源：http://pwu.nwbrower.top

[U16] Py：命令行参数解析
来源：http://qmx.shangyingyoupin.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ijf.zhiwuduotai.top

[U17] Py：初始化日志
来源：http://jrs.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://tgv.zdbjq.cn

[U18] Py：预编译正则
来源：http://anr.jqgufenzy.top

pat = re.compile(r"\d+")
来源：http://lun.pengpengdd.cyou

[U19] Py：正则替换带回调
来源：http://say.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mtj.fzhhl.top

[U20] Py：缓存函数结果
来源：http://guq.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://dvv.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://vjm.ppjwa.cn

@contextlib.contextmanager
来源：http://uly.jinqigfzy.top

[U22] Py：矩阵转置
来源：http://hzh.andypj.xyz

list(zip(*m))
来源：http://pvi.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://ldl.gogol.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ynt.xuetiantiany.cn

[U24] Py：路径操作
来源：http://cja.hammf.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vhb.feifeiyinyue.top

[U25] Py：CSV 按字典读
来源：http://kio.jlsjyb.cn

csv.DictReader(f)
来源：http://mjc.52xcode.cn

[U26] Py：并发下载
来源：http://vlm.smart0.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nqy.jqgfzy.top

[U27] Py：异步 HTTP
来源：http://xos.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://reg.hfpthk.cn

[U28] Py：类型别名
来源：http://mbe.hesvh.cn

UserId = int
来源：http://lpl.ivvv.top

[U29] Py：属性校验
来源：http://sss.shuidangran.top

@property 与 @x.setter 配合
来源：http://fub.xuetiantiany.cn

[U30] Py：数据类
来源：http://qjo.fengsongda.top

@dataclass(slots=True)
来源：http://pnt.zdbjq.cn

[U31] Py：单测
来源：http://ooi.fktsv.cn

python -m pytest -q
来源：http://nsh.jyoumei.cn

[U32] Py：代码格式化
来源：http://tdt.ydzc1.top

ruff format . && ruff check --fix .
来源：http://jdd.hesvh.cn

[U33] Py：打包发布
来源：http://efj.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://mnk.yanxiufei.cn

[U34] Py：判断编码
来源：http://nxw.nwbrower.top

chardet.detect(raw)
来源：http://qch.yuxming.cn

[U35] Py：发送邮件
来源：http://luz.yfazqb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ydv.vehdjk.com

[U36] Py：定时任务
来源：http://vmz.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://pfj.shanyushiyangtech.top

[U37] Py：读写 Excel
来源：http://wdm.yuxming.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kak.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://pnw.gzhubu.top

Path(__file__).resolve().parent
来源：http://biw.cashguo.top

[U39] Py：判断是否在交互环境
来源：http://yfn.fanxiaobao.xyz

sys.stdout.isatty()
来源：http://lbw.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://mzc.sysykeji.top

print("err", file=sys.stderr)
来源：http://cxj.gzhubu.top

[U41] PHP：初始化 Composer 项目
来源：http://wyx.zhoulong.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://mwy.smart0.xyz

[U42] PHP：PSR-4 自动加载
来源：http://xun.smart0.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uqd.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://xtx.yj20258888.top

namespace App\Http;
来源：http://tqj.jinyuanbaomall.cn

[U44] PHP：开启严格类型
来源：http://cdv.yj20258.top

declare(strict_types=1);
来源：http://kez.c1oappe.top

[U45] PHP：类型声明与返回类型
来源：http://spy.chenjidiqi.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://zjv.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://dvy.yvedp.cn

?string $name = null
来源：http://wzy.chenjidiqi.icu

[U47] PHP：联合类型
来源：http://eia.jinyuanbaomall.cn

int|string $id
来源：http://dsb.yanxiufei.cn

[U48] PHP：纯枚举
来源：http://tmd.316326.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://crp.cdnleiting.top

[U49] PHP：只读属性
来源：http://set.aizwys.cn

public readonly string $name
来源：http://eas.guannengcc.top

[U50] PHP：构造器属性提升
来源：http://hjn.shuidangran.top

public function __construct(private int $id) {}
来源：http://zkk.yueranfly.top

[U51] PHP：数组解构
来源：http://iek.cqqwz.cn

[$a, $b] = $arr;
来源：http://cku.ywan-chungtsiang.top

[U52] PHP：箭头函数
来源：http://gil.hywenlv.cn

$double = fn($x) => $x * 2;
来源：http://cpu.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://uab.fanxiaobao.xyz

$v = $a ?? $b ?? "default";
来源：http://ldo.havefunace.top

[U54] PHP：空安全调用
来源：http://ovm.gogol.net.cn

$obj?->method()
来源：http://vhf.xylfe.cn

[U55] PHP：match 表达式
来源：http://bfo.fktsv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dja.yfazqb.com

[U56] PHP：命名参数
来源：http://dgo.mhx1999.top

f(a: 1, b: 2)
来源：http://wpp.guannengcc.top

[U57] PHP：字符串插值
来源：http://krq.mhx1999.top

"值: {$a}"
来源：http://ctr.wangdashe.top

[U58] PHP：数组三件套
来源：http://rux.cucudq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://alv.xinyue.icu

[U59] PHP：自定义排序
来源：http://ipg.ctjpmb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bgg.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://ceb.bjfxy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nob.kuanghao11.cn

[U61] PHP：正则
来源：http://ecr.cdnleiting.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://axd.uphjek.com

[U62] PHP：日期对象
来源：http://koj.xingfuxueyuan.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://otx.tian-w.cn

[U63] PHP：文件读写
来源：http://pwx.zhijiandao.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pvy.daria6918.cn

[U64] PHP：目录遍历
来源：http://qjq.xinyue.icu

glob("dir/*.php");  scandir("dir");
来源：http://eed.nanxinkj.top

[U65] PHP：会话
来源：http://hee.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://vvn.nanxinkj.top

[U66] PHP：设置 Cookie
来源：http://pnb.svipenyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tdd.snrcjt.cn

[U67] PHP：处理文件上传
来源：http://djg.wangdashe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gnj.fanxiaobao.xyz

[U68] PHP：PDO 连接
来源：http://izs.hnqzz.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eft.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://oii.zycfv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lse.yongpay.top

[U70] PHP：PDO 事务
来源：http://yxr.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vps.wangshuangyany.cn

[U71] PHP：抛出异常
来源：http://wjl.gzhubu.top

throw new RuntimeException("失败", 500);
来源：http://nei.zhongyouzk.top

[U72] PHP：写错误日志
来源：http://efd.hnqzz.top

error_log("失败: " . $e->getMessage());
来源：http://cwk.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://dho.yongpay.top

parse_ini_file("config.ini", true)
来源：http://fgt.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://zjw.sysykeji.top

getenv("APP_ENV") ?: "production"
来源：http://zss.hywenlv.cn

[U75] PHP：依赖注入
来源：http://olv.gaohongyu789.top

composer require psr/container
来源：http://nln.yongpay.top

[U76] PHP：简单路由
来源：http://rfu.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jdl.zdqjudy.top

[U77] PHP：模板渲染
来源：http://ezz.zhiwuduotai.top

composer require twig/twig
来源：http://zzv.shangyingyoupin.top

[U78] PHP：单元测试
来源：http://kqm.gzhubu.top

composer require --dev phpunit/phpunit
来源：http://xxc.xylfe.cn

[U79] PHP：静态分析
来源：http://apu.hysaishi.cn

composer require --dev phpstan/phpstan
来源：http://jua.wangdashe.top

[U80] PHP：代码规范修复
来源：http://xko.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://enk.jqgufenzy.top

[U81] JS：初始化项目
来源：http://crz.zhongyouzk.top

npm init -y;  npm i express
来源：http://fsj.uphjek.com

[U82] JS：package.json 脚本
来源：http://hni.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bnw.cashguo.top

[U83] JS：ES Module 导入导出
来源：http://ynr.fzhhl.top

export const a = 1;  import { a } from "./m.js";
来源：http://krh.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://oef.chenlongwang.top

module.exports = { a };  const { a } = require("./m");
来源：http://jhs.tarul.cn

[U85] JS：可选链
来源：http://onu.uphjek.com

a?.b?.c
来源：http://vxa.yuanzhike.top

[U86] JS：空值合并
来源：http://whz.hesvh.cn

a ?? b
来源：http://gvs.iojbl.cn

[U87] JS：解构默认值
来源：http://kul.yueranfly.top

const { a = 1, b = 2 } = obj;
来源：http://wgp.dashuyun.cn

[U88] JS：对象展开合并
来源：http://qvq.shuidangran.top

{ ...a, ...b }
来源：http://cmy.cheryme.top


<!-- 参考信息 -->