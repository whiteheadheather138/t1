代发 wailian999

[T03] Kotlin：字符串模板
来源：http://wmd.xinyue.icu

"值: $b"
来源：http://ywk.pycfn.com

[T04] Kotlin：空安全
来源：http://pxq.yuxming.cn

val n: String? = null;  n?.length
来源：http://syp.nanxinkj.top

[T05] Kotlin：when 表达式
来源：http://nhq.andypj.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tzz.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://wpg.yanxiufei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://koa.fktsv.cn

[T07] Kotlin：集合过滤
来源：http://bhe.nanxuanxn.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ole.birdmap.top

[T08] Kotlin：数据类
来源：http://gxh.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://dqn.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://fun.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://yot.yueranfly.top

[T10] Kotlin：默认参数
来源：http://bzo.guowangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://naq.nanxuanxn.top

[T11] Kotlin：协程
来源：http://otl.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wrr.shzxlz.cn

[T12] Kotlin：解构声明
来源：http://nlz.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://jia.zhaomingkeji.xyz

[T13] Kotlin：只读 Map
来源：http://rts.chenjidiqi.icu

val m = mapOf("a" to 1)
来源：http://fuz.zhongyouzk.top

[T14] Kotlin：循环
来源：http://hku.hywenlv.cn

for (i in 1..10) println(i)
来源：http://xpm.hcnkem.com

[T15] Kotlin：接口
来源：http://vzf.shangyingyoupin.top

interface Shape { fun area(): Double }
来源：http://guw.tianlin.xyz

[T16] Swift：Hello World
来源：http://vmj.uphjek.com

print("Hello")
来源：http://ark.jianghu66.top

[T17] Swift：变量与常量
来源：http://uch.snrcjt.cn

var a = 1;  let b = 2
来源：http://qni.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://zht.jqgufenzy.top

"值: \(b)"
来源：http://eij.yj202588.top

[T19] Swift：可选绑定
来源：http://muo.0kj1m.cn

if let n = opt { print(n) }
来源：http://ykl.nwbrower.top

[T20] Swift：数组操作
来源：http://prd.bbcook.cn

var a = [1, 2, 3];  a.append(4)
来源：http://obs.guowangkeji.top

[T21] Swift：遍历
来源：http://tjr.vqdsnc.cn

for x in a { print(x) }
来源：http://qpc.ydzc1.top

[T22] Swift：字典
来源：http://yjq.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ifv.kuanghao11.cn

[T23] Swift：函数
来源：http://zwo.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zzo.zdqjudy.top

[T24] Swift：闭包
来源：http://ini.guannengcc.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cki.jyoumei.cn

[T25] Swift：结构体
来源：http://ygl.bjfxy.top

struct P { var x: Int }
来源：http://nst.316326.xyz

[T26] Swift：类与重写
来源：http://fvl.iojbl.cn

class A: Base { override func f() {} }
来源：http://nmr.yj20258.top

[T27] Swift：错误处理
来源：http://qsr.jinqigfzy.top

do { try f() } catch { print(error) }
来源：http://xil.ydzc1.top

[T28] Swift：枚举
来源：http://fgx.ydzc1.top

enum Color { case red, green }
来源：http://gce.svipenyu.cn

[T29] Swift：guard 提前返回
来源：http://bng.xinyue.icu

guard let x = opt else { return }
来源：http://zao.jyoumei.cn

[T30] Swift：协议
来源：http://knj.jinqigfzy.top

protocol Shape { func area() -> Double }
来源：http://mot.uphjek.com

[T31] Lua：Hello World
来源：http://xkx.yj20258.top

print("Hello")
来源：http://ysw.quarkkingdee.top

[T32] Lua：局部变量
来源：http://ars.shangyingyoupin.top

local a = 1
来源：http://fop.xylfe.cn

[T33] Lua：表（数组）
来源：http://rgt.fanxiaobao.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://iff.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://ksn.zhengqikj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qfb.dashuyun.cn

[T35] Lua：字典表
来源：http://cnk.fktsv.cn

local d = { a = 1 };  d.b = 2
来源：http://cno.zycfv.cn

[T36] Lua：函数
来源：http://bsr.c1oappe.top

function add(a, b) return a + b end
来源：http://xfb.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://nlc.tarul.cn

"a" .. "b"
来源：http://xap.zhijiandao.cn

[T38] Lua：条件
来源：http://mqu.jinqigufen.top

if x > 0 then print("正") end
来源：http://ceg.sweek.top

[T39] Lua：模式匹配
来源：http://jyf.ppjwa.cn

string.find(s, "%d+")
来源：http://xjm.jyoumei.cn

[T40] Lua：元表
来源：http://urj.jqgufenzy.top

setmetatable({}, { __index = base })
来源：http://bgs.c1oappe.top

[T41] Perl：Hello World
来源：http://xdo.guannengcc.top

print "Hello\n";
来源：http://jnh.gzhubu.top

[T42] Perl：变量类型
来源：http://mlz.quarkkingdee.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lmx.fktsv.cn

[T43] Perl：字符串插值
来源：http://ypf.fzhhl.top

"值: $a"
来源：http://uic.hnxiangtu.top

[T44] Perl：条件
来源：http://bba.zdqjudy.top

if ($a > 0) { print "正"; }
来源：http://tyh.xinyue.icu

[T45] Perl：数组遍历
来源：http://vcp.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://plw.yj202588.top

[T46] Perl：哈希操作
来源：http://mrc.c1oappe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tjv.sweek.top

[T47] Perl：正则捕获
来源：http://xdz.316326.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://khp.bbcook.cn

[T48] Perl：正则替换
来源：http://dwj.ybcxt.top

$s =~ s/old/new/g;
来源：http://eak.zhixingplan.top

[T49] Perl：函数
来源：http://hdz.quarkkingdee.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pye.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://ikd.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pmn.yongpay.top

while (my $line = <$fh>) { print $line; }
来源：http://oge.hesvh.cn

[T51] Scala：Hello World
来源：http://hdo.nanxinkj.top

println("Hello")
来源：http://sgv.jinyuanbaomall.cn

[T52] Scala：变量
来源：http://jpj.aizwys.cn

val a = 1;  var b = 2
来源：http://ppw.zhijiandao.cn

[T53] Scala：字符串插值
来源：http://mun.zhijiandao.cn

s"值: $b"
来源：http://dyg.xylfe.cn

[T54] Scala：集合映射
来源：http://jzv.haohaochexian.top

List(1, 2, 3).map(_ * 2)
来源：http://jbt.shanyushiyangtech.top

[T55] Scala：集合过滤
来源：http://ioa.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://wvq.fktsv.cn

[T56] Scala：样例类
来源：http://rhs.xziqi.cn

case class User(name: String, age: Int)
来源：http://pth.andypj.xyz

[T57] Scala：模式匹配
来源：http://yrt.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://aph.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://kjv.jinyuanbaomall.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uxs.tarul.cn

[T59] Scala：循环
来源：http://pan.shangyingyoupin.top

for (i <- 1 to 10) println(i)
来源：http://kdi.shangyingyoupin.top

[T60] Scala：折叠
来源：http://qso.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aqe.sjlbkw.cn

================================================================================
来源：http://rhd.shanyushiyangtech.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mii.zhijiandao.cn

================================================================================
来源：http://swu.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://rpj.nanxuanxn.top

python -m venv .venv && source .venv/bin/activate
来源：http://bif.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://zao.pengpengdd.cyou

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ipf.hywenlv.cn

[U03] Py：加载 .env 配置
来源：http://mbt.xziqi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ogr.jinqigufen.top

[U04] Py：变量调试打印
来源：http://sjw.sweek.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gbs.9152youxi.cn

[U05] Py：列表去重且保序
来源：http://bmh.hywenlv.cn

list(dict.fromkeys(arr))
来源：http://xqz.vqdsnc.cn

[U06] Py：合并两个字典
来源：http://dqc.cheryme.top

{**a, **b}
来源：http://hjg.yj202588.top

[U07] Py：反转字典键值
来源：http://zjy.sweek.top

{v: k for k, v in d.items()}
来源：http://dgr.jyoumei.cn

[U08] Py：展平二维列表
来源：http://uqb.jlsjyb.cn

[y for x in nested for y in x]
来源：http://bfw.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://yrd.shuidangran.top

max(d, key=d.get)
来源：http://hbg.jqgfzy.top

[U10] Py：按值排序字典
来源：http://fbh.hnxiangtu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ubo.vehdjk.com

[U11] Py：生成器表达式
来源：http://gvy.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://hyp.chenlongwang.top

[U12] Py：取出现最多的 3 个元素
来源：http://qvl.fzhhl.top

Counter(arr).most_common(3)
来源：http://knv.hysaishi.cn

[U13] Py：固定长度队列
来源：http://lmz.dianchejie.cn

deque(maxlen=10)
来源：http://yof.daxiang520.top

[U14] Py：分组收集到列表
来源：http://khs.yonumen.top

defaultdict(list)
来源：http://xqx.sysykeji.top

[U15] Py：高精度计时
来源：http://cez.shuidangran.top

t = time.perf_counter()
来源：http://wrb.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://sob.ywan-chungtsiang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dge.zhoulong.xyz

[U17] Py：初始化日志
来源：http://ouj.yueranfly.top

logging.basicConfig(level=logging.INFO)
来源：http://pce.havefunace.top

[U18] Py：预编译正则
来源：http://gjz.jianghu66.top

pat = re.compile(r"\d+")
来源：http://rzn.jiagoushi.top

[U19] Py：正则替换带回调
来源：http://wml.smart0.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mnd.hcnkem.com

[U20] Py：缓存函数结果
来源：http://fkp.tarul.cn

@functools.lru_cache(maxsize=None)
来源：http://iic.vehdjk.com

[U21] Py：自定义上下文管理器
来源：http://yqb.sysykeji.top

@contextlib.contextmanager
来源：http://tuq.bjfxy.top

[U22] Py：矩阵转置
来源：http://kbs.cucudq.cn

list(zip(*m))
来源：http://mgy.vehdjk.com

[U23] Py：分块读取大文件
来源：http://zrx.shuidangran.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://deg.yuanzhike.top

[U24] Py：路径操作
来源：http://fbe.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wou.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://apm.jyoumei.cn

csv.DictReader(f)
来源：http://fmp.xylfe.cn

[U26] Py：并发下载
来源：http://emz.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pvt.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://cbu.zhoulong.xyz

aiohttp.ClientSession() 配合 async with
来源：http://bhv.gaohongyu789.top

[U28] Py：类型别名
来源：http://ilj.yj20258888.top

UserId = int
来源：http://zam.jyoumei.cn

[U29] Py：属性校验
来源：http://jes.tian-w.cn

@property 与 @x.setter 配合
来源：http://oau.zhongyouzk.top

[U30] Py：数据类
来源：http://dus.daria6918.cn

@dataclass(slots=True)
来源：http://wis.cdnleiting.top

[U31] Py：单测
来源：http://ota.birdmap.top

python -m pytest -q
来源：http://uur.xuanzx.com

[U32] Py：代码格式化
来源：http://sug.wangdashe.top

ruff format . && ruff check --fix .
来源：http://wwy.yuanzhike.top

[U33] Py：打包发布
来源：http://yda.birdmap.top

python -m build  （依赖 pyproject.toml）
来源：http://bpv.hnxiangtu.top

[U34] Py：判断编码
来源：http://wmc.yj20258.top

chardet.detect(raw)
来源：http://fly.ydjk.org.cn

[U35] Py：发送邮件
来源：http://yac.xziqi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://von.aizwys.cn

[U36] Py：定时任务
来源：http://wtr.yonumen.top

schedule.every(10).minutes.do(job)
来源：http://sfu.pengpengdd.cyou

[U37] Py：读写 Excel
来源：http://ghh.fengsongda.top

pandas.read_excel / DataFrame.to_excel
来源：http://dqp.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://mbq.zhoulong.xyz

Path(__file__).resolve().parent
来源：http://jqe.xinyue.icu

[U39] Py：判断是否在交互环境
来源：http://yzt.quarkkingdee.top

sys.stdout.isatty()
来源：http://osy.gaohongyu789.top

[U40] Py：打印到标准错误
来源：http://juy.sjlbkw.cn

print("err", file=sys.stderr)
来源：http://elz.meibo888.top

[U41] PHP：初始化 Composer 项目
来源：http://gce.pycfn.com

composer init;  composer require guzzlehttp/guzzle
来源：http://tyn.ehwqpu.com

[U42] PHP：PSR-4 自动加载
来源：http://lfs.yanxiufei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pwg.ehwqpu.com

[U43] PHP：声明命名空间
来源：http://vlw.zdqjudy.top

namespace App\Http;
来源：http://xwm.nwbrower.top

[U44] PHP：开启严格类型
来源：http://tmt.jqgufenzy.top

declare(strict_types=1);
来源：http://urp.tanke756.top

[U45] PHP：类型声明与返回类型
来源：http://yxd.hywenlv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ipo.andypj.xyz

[U46] PHP：可空类型
来源：http://nng.guannengcc.top

?string $name = null
来源：http://hcp.vqdsnc.cn

[U47] PHP：联合类型
来源：http://hff.xinyue.icu

int|string $id
来源：http://fah.fanxiaobao.xyz

[U48] PHP：纯枚举
来源：http://tfh.hesvh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fyl.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://ywz.cheryme.top

public readonly string $name
来源：http://agl.uphjek.com

[U50] PHP：构造器属性提升
来源：http://uoe.sjlbkw.cn

public function __construct(private int $id) {}
来源：http://lnc.nwbrower.top

[U51] PHP：数组解构
来源：http://ygl.zhongyouzk.top

[$a, $b] = $arr;
来源：http://asx.shzxlz.cn

[U52] PHP：箭头函数
来源：http://erb.gaohongyu789.top

$double = fn($x) => $x * 2;
来源：http://ivt.dashuyun.cn

[U53] PHP：空合并运算符
来源：http://sch.zhaomingkeji.xyz

$v = $a ?? $b ?? "default";
来源：http://xbj.wangdashe.top

[U54] PHP：空安全调用
来源：http://zno.quarkkingdee.top

$obj?->method()
来源：http://eyr.jinyuanbaomall.cn

[U55] PHP：match 表达式
来源：http://brt.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://frg.andypj.xyz

[U56] PHP：命名参数
来源：http://loc.xziqi.cn

f(a: 1, b: 2)
来源：http://mcc.cdnleiting.top

[U57] PHP：字符串插值
来源：http://njm.yueranfly.top

"值: {$a}"
来源：http://vpk.cucudq.cn

[U58] PHP：数组三件套
来源：http://nqy.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yfx.fengsongda.top

[U59] PHP：自定义排序
来源：http://sex.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mxu.pengpengdd.cyou

[U60] PHP：JSON 编解码
来源：http://hpv.ybcxt.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ucr.zhiwuduotai.top

[U61] PHP：正则
来源：http://vav.yj20258.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ztr.gaohongyu789.top

[U62] PHP：日期对象
来源：http://ayi.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://otp.fzhhl.top

[U63] PHP：文件读写
来源：http://isu.zhengqikj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rau.yueranfly.top

[U64] PHP：目录遍历
来源：http://awb.jlsjyb.cn

glob("dir/*.php");  scandir("dir");
来源：http://kqp.tianlin.xyz

[U65] PHP：会话
来源：http://ifd.ehwqpu.com

session_start();  $_SESSION["uid"] = 1;
来源：http://yov.ppjwa.cn

[U66] PHP：设置 Cookie
来源：http://yxd.smart0.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lqe.yongpay.top

[U67] PHP：处理文件上传
来源：http://gkj.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iie.9152youxi.cn

[U68] PHP：PDO 连接
来源：http://sfj.yueranfly.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hej.pycfn.com

[U69] PHP：PDO 预处理
来源：http://sry.ppjwa.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nog.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://otp.cqqwz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sak.zhixingplan.top

[U71] PHP：抛出异常
来源：http://sii.zhiwuduotai.top

throw new RuntimeException("失败", 500);
来源：http://tyo.daria6918.cn

[U72] PHP：写错误日志
来源：http://pcm.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://rpc.nanxuanxn.top

[U73] PHP：读取 ini 配置
来源：http://vtd.zhongyouzk.top

parse_ini_file("config.ini", true)
来源：http://gas.gaohongyu789.top

[U74] PHP：读取环境变量
来源：http://zml.kuanghao11.cn

getenv("APP_ENV") ?: "production"
来源：http://ufx.feifeiyinyue.top

[U75] PHP：依赖注入
来源：http://qsz.zhongyouzk.top

composer require psr/container
来源：http://mzz.nwbrower.top

[U76] PHP：简单路由
来源：http://keg.chenlongwang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://awn.xingfuxueyuan.xyz

[U77] PHP：模板渲染
来源：http://vya.feifeiyinyue.top

composer require twig/twig
来源：http://eos.yangfankeji.com

[U78] PHP：单元测试
来源：http://oxn.zhixingplan.top

composer require --dev phpunit/phpunit
来源：http://agt.cdnleiting.top

[U79] PHP：静态分析
来源：http://lgr.hammf.cn

composer require --dev phpstan/phpstan
来源：http://hfj.jiagoushi.top

[U80] PHP：代码规范修复
来源：http://eoc.yangfankeji.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://axy.ivvv.top

[U81] JS：初始化项目
来源：http://wzs.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://hud.iojbl.cn

[U82] JS：package.json 脚本
来源：http://bor.52xcode.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ptp.ywan-chungtsiang.top

[U83] JS：ES Module 导入导出
来源：http://kod.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://emx.sysykeji.top

[U84] JS：CommonJS 写法
来源：http://clp.zhongyouzk.top

module.exports = { a };  const { a } = require("./m");
来源：http://ycc.xuetiantiany.cn

[U85] JS：可选链
来源：http://kzh.ydjk.org.cn

a?.b?.c
来源：http://oyw.jqgufenzy.top

[U86] JS：空值合并
来源：http://hwm.yuxming.cn

a ?? b
来源：http://qrs.smart0.xyz

[U87] JS：解构默认值
来源：http://dco.sxryk.cn

const { a = 1, b = 2 } = obj;
来源：http://izz.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://rol.hywenlv.cn

{ ...a, ...b }
来源：http://snu.tanke756.top

[U89] JS：数组去重
来源：http://ceb.cqqwz.cn

[...new Set(arr)]
来源：http://quc.hnxiangtu.top

[U90] JS：数字数组排序
来源：http://wsc.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://jok.yuanzhike.top


<!-- 参考信息 -->