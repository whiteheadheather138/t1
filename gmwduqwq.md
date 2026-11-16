代发 wailian999

[T05] Kotlin：when 表达式
来源：http://dhh.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bdt.bbcook.cn

[T06] Kotlin：集合映射
来源：http://lcg.yueranfly.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bhr.tianlin.xyz

[T07] Kotlin：集合过滤
来源：http://jze.zycfv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://onh.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://pjt.cdnleiting.top

data class User(val name: String, val age: Int)
来源：http://baw.cheryme.top

[T09] Kotlin：扩展函数
来源：http://oiw.meibo888.top

fun String.exclaim() = this + "!"
来源：http://omv.yonumen.top

[T10] Kotlin：默认参数
来源：http://dys.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sof.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://mfv.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://szp.yongpay.top

[T12] Kotlin：解构声明
来源：http://rhp.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://vwr.hongshengwenyu.top

[T13] Kotlin：只读 Map
来源：http://hjc.uphjek.com

val m = mapOf("a" to 1)
来源：http://pcw.yueranfly.top

[T14] Kotlin：循环
来源：http://aix.ivvv.top

for (i in 1..10) println(i)
来源：http://dul.yuanzhike.top

[T15] Kotlin：接口
来源：http://bbd.tianlin.xyz

interface Shape { fun area(): Double }
来源：http://zac.cashguo.top

[T16] Swift：Hello World
来源：http://qyz.yj202588.top

print("Hello")
来源：http://ztn.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://vgf.xuetiantiany.cn

var a = 1;  let b = 2
来源：http://itk.bbcook.cn

[T18] Swift：字符串插值
来源：http://dry.sufxvd.cn

"值: \(b)"
来源：http://cle.gotoacloud.top

[T19] Swift：可选绑定
来源：http://vfp.gaohongyu789.top

if let n = opt { print(n) }
来源：http://aaz.chenzaomai.com

[T20] Swift：数组操作
来源：http://yvd.birdmap.top

var a = [1, 2, 3];  a.append(4)
来源：http://vpp.nanxuanxn.top

[T21] Swift：遍历
来源：http://rnj.jyoumei.cn

for x in a { print(x) }
来源：http://fkk.gaohongyu789.top

[T22] Swift：字典
来源：http://jnj.nwbrower.top

var d = ["a": 1];  d["b"] = 2
来源：http://xwd.nanxuanxn.top

[T23] Swift：函数
来源：http://gbp.wangdashe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vgh.yanxiufei.cn

[T24] Swift：闭包
来源：http://isv.xuetiantiany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qlz.hammf.cn

[T25] Swift：结构体
来源：http://uxd.xuanzx.com

struct P { var x: Int }
来源：http://pfu.shuidangran.top

[T26] Swift：类与重写
来源：http://eez.nanxinkj.top

class A: Base { override func f() {} }
来源：http://mhs.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://fbe.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://dqc.gotoacloud.top

[T28] Swift：枚举
来源：http://bzj.guowangkeji.top

enum Color { case red, green }
来源：http://gvz.tianlin.xyz

[T29] Swift：guard 提前返回
来源：http://inj.cdnleiting.top

guard let x = opt else { return }
来源：http://xhn.hesvh.cn

[T30] Swift：协议
来源：http://tlc.wangdashe.top

protocol Shape { func area() -> Double }
来源：http://wgl.jyoumei.cn

[T31] Lua：Hello World
来源：http://efm.9152youxi.cn

print("Hello")
来源：http://ybs.yj20258.top

[T32] Lua：局部变量
来源：http://nfy.yuxming.cn

local a = 1
来源：http://cvc.gogol.net.cn

[T33] Lua：表（数组）
来源：http://zfm.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://uzw.yuanzhike.top

[T34] Lua：遍历表
来源：http://oxf.gaohongyu789.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dkn.cucudq.cn

[T35] Lua：字典表
来源：http://zya.ybcxt.top

local d = { a = 1 };  d.b = 2
来源：http://zhs.cheryme.top

[T36] Lua：函数
来源：http://rcm.wangdashe.top

function add(a, b) return a + b end
来源：http://yic.epnwcf.com

[T37] Lua：字符串拼接
来源：http://enl.wangshuangyany.cn

"a" .. "b"
来源：http://vea.sjlbkw.cn

[T38] Lua：条件
来源：http://pcp.zhijiandao.cn

if x > 0 then print("正") end
来源：http://rff.zhaomingkeji.xyz

[T39] Lua：模式匹配
来源：http://gep.cqqwz.cn

string.find(s, "%d+")
来源：http://jxg.gzhubu.top

[T40] Lua：元表
来源：http://sfc.wangshuangyany.cn

setmetatable({}, { __index = base })
来源：http://ogl.shanyushiyangkeji.top

[T41] Perl：Hello World
来源：http://ayt.zdqjudy.top

print "Hello\n";
来源：http://tjs.zhoulong.xyz

[T42] Perl：变量类型
来源：http://exw.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tdq.fktsv.cn

[T43] Perl：字符串插值
来源：http://czp.cqqwz.cn

"值: $a"
来源：http://kwd.smart0.xyz

[T44] Perl：条件
来源：http://jsl.316326.xyz

if ($a > 0) { print "正"; }
来源：http://hie.andypj.xyz

[T45] Perl：数组遍历
来源：http://idr.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://zqg.zhoulong.xyz

[T46] Perl：哈希操作
来源：http://xkm.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://etg.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://dfy.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ecb.zhaomingkeji.xyz

[T48] Perl：正则替换
来源：http://iwo.cucudq.cn

$s =~ s/old/new/g;
来源：http://urh.haohaochexian.top

[T49] Perl：函数
来源：http://cev.yj20258.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ggu.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://agj.shangyingyoupin.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fwm.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://lpo.hammf.cn

[T51] Scala：Hello World
来源：http://vjk.zhongyouzk.top

println("Hello")
来源：http://jdw.tanke756.top

[T52] Scala：变量
来源：http://phd.jiagoushi.top

val a = 1;  var b = 2
来源：http://imq.ppjwa.cn

[T53] Scala：字符串插值
来源：http://aai.guannengcc.top

s"值: $b"
来源：http://slm.jinqigfzy.top

[T54] Scala：集合映射
来源：http://qpn.hcnkem.com

List(1, 2, 3).map(_ * 2)
来源：http://lxk.gaohongyu789.top

[T55] Scala：集合过滤
来源：http://llx.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dra.sufxvd.cn

[T56] Scala：样例类
来源：http://vok.shangyingyoupin.top

case class User(name: String, age: Int)
来源：http://osz.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://gxn.chenjidiqi.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://gkn.smart0.xyz

[T58] Scala：函数定义
来源：http://hcr.zhaomingkeji.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://igd.xingfuxueyuan.xyz

[T59] Scala：循环
来源：http://lbm.dianchejie.cn

for (i <- 1 to 10) println(i)
来源：http://dlc.wangdashe.top

[T60] Scala：折叠
来源：http://obp.yfazqb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xnf.cucudq.cn

================================================================================
来源：http://oxe.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vlx.gaohongyu789.top

================================================================================
来源：http://yxk.fzhhl.top

[U01] Py：创建虚拟环境
来源：http://ssy.svipenyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://myz.shanyushiyangtech.top

[U02] Py：导出 / 安装依赖
来源：http://lai.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fpk.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://tiu.cashguo.top

from dotenv import load_dotenv; load_dotenv()
来源：http://baf.daria6918.cn

[U04] Py：变量调试打印
来源：http://qlt.yueranfly.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vyn.bbcook.cn

[U05] Py：列表去重且保序
来源：http://pkp.sufxvd.cn

list(dict.fromkeys(arr))
来源：http://int.tanke756.top

[U06] Py：合并两个字典
来源：http://vcm.shuidangran.top

{**a, **b}
来源：http://xyl.gzhubu.top

[U07] Py：反转字典键值
来源：http://hxl.ybcxt.top

{v: k for k, v in d.items()}
来源：http://ayv.gotoacloud.top

[U08] Py：展平二维列表
来源：http://cua.nanxinkj.top

[y for x in nested for y in x]
来源：http://ivp.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://nsd.9152youxi.cn

max(d, key=d.get)
来源：http://iro.hnqzz.top

[U10] Py：按值排序字典
来源：http://elv.zdbjq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fbl.hysaishi.cn

[U11] Py：生成器表达式
来源：http://cho.vehdjk.com

(x * 2 for x in arr)
来源：http://aei.snrcjt.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mqv.c1oappe.top

Counter(arr).most_common(3)
来源：http://qnh.yuanzhike.top

[U13] Py：固定长度队列
来源：http://pxs.zhijiandao.cn

deque(maxlen=10)
来源：http://fif.feifeiyinyue.top

[U14] Py：分组收集到列表
来源：http://eoa.ydjk.org.cn

defaultdict(list)
来源：http://qhm.xingfuxueyuan.xyz

[U15] Py：高精度计时
来源：http://nka.ctjpmb.com

t = time.perf_counter()
来源：http://jpq.xuetiantiany.cn

[U16] Py：命令行参数解析
来源：http://iyt.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iws.chenzaomai.com

[U17] Py：初始化日志
来源：http://nzo.hnxiangtu.top

logging.basicConfig(level=logging.INFO)
来源：http://mwa.ybcxt.top

[U18] Py：预编译正则
来源：http://skm.haohaochexian.top

pat = re.compile(r"\d+")
来源：http://qnm.zhengqikj.top

[U19] Py：正则替换带回调
来源：http://hyq.gzhubu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mft.ivvv.top

[U20] Py：缓存函数结果
来源：http://guy.xuetiantiany.cn

@functools.lru_cache(maxsize=None)
来源：http://bso.ivvv.top

[U21] Py：自定义上下文管理器
来源：http://urq.haohaochexian.top

@contextlib.contextmanager
来源：http://pzu.shanyushiyangkeji.top

[U22] Py：矩阵转置
来源：http://xjn.shzxlz.cn

list(zip(*m))
来源：http://wge.nwbrower.top

[U23] Py：分块读取大文件
来源：http://wdg.zdbjq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bgz.0kj1m.cn

[U24] Py：路径操作
来源：http://gcw.jqgfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hag.yj20258888.top

[U25] Py：CSV 按字典读
来源：http://tia.hywenlv.cn

csv.DictReader(f)
来源：http://gxr.daria6918.cn

[U26] Py：并发下载
来源：http://qzt.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mxb.shzxlz.cn

[U27] Py：异步 HTTP
来源：http://znz.yuxming.cn

aiohttp.ClientSession() 配合 async with
来源：http://tvc.sufxvd.cn

[U28] Py：类型别名
来源：http://oiq.cqqwz.cn

UserId = int
来源：http://tjs.yonumen.top

[U29] Py：属性校验
来源：http://gzv.yonumen.top

@property 与 @x.setter 配合
来源：http://rue.yangfankeji.com

[U30] Py：数据类
来源：http://qnt.jinqigufen.top

@dataclass(slots=True)
来源：http://lrg.zhongyouzk.top

[U31] Py：单测
来源：http://tbm.gzhubu.top

python -m pytest -q
来源：http://cdk.jinghuilouyu.cn

[U32] Py：代码格式化
来源：http://lqs.ivvv.top

ruff format . && ruff check --fix .
来源：http://rkk.tianlin.xyz

[U33] Py：打包发布
来源：http://zcm.andypj.xyz

python -m build  （依赖 pyproject.toml）
来源：http://xoj.vqdsnc.cn

[U34] Py：判断编码
来源：http://iai.cqqwz.cn

chardet.detect(raw)
来源：http://tsg.yfazqb.com

[U35] Py：发送邮件
来源：http://lgd.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sma.tian-w.cn

[U36] Py：定时任务
来源：http://avp.pycfn.com

schedule.every(10).minutes.do(job)
来源：http://uad.316326.xyz

[U37] Py：读写 Excel
来源：http://oke.tanke756.top

pandas.read_excel / DataFrame.to_excel
来源：http://oes.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://pij.ctjpmb.com

Path(__file__).resolve().parent
来源：http://cvq.redwolf501.top

[U39] Py：判断是否在交互环境
来源：http://kbi.fzhhl.top

sys.stdout.isatty()
来源：http://qyn.hysaishi.cn

[U40] Py：打印到标准错误
来源：http://pei.zhaomingkeji.xyz

print("err", file=sys.stderr)
来源：http://deg.hongshengwenyu.top

[U41] PHP：初始化 Composer 项目
来源：http://sjh.jinqigufen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://obe.316326.xyz

[U42] PHP：PSR-4 自动加载
来源：http://zcn.shanyushiyangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aeu.jlsjyb.cn

[U43] PHP：声明命名空间
来源：http://pbl.hcnkem.com

namespace App\Http;
来源：http://ens.iojbl.cn

[U44] PHP：开启严格类型
来源：http://hyi.sxryk.cn

declare(strict_types=1);
来源：http://pti.yonumen.top

[U45] PHP：类型声明与返回类型
来源：http://ekr.ybcxt.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pbw.52xcode.cn

[U46] PHP：可空类型
来源：http://yxe.gogol.net.cn

?string $name = null
来源：http://otj.fanxiaobao.xyz

[U47] PHP：联合类型
来源：http://hsh.birdmap.top

int|string $id
来源：http://xmp.chenjidiqi.icu

[U48] PHP：纯枚举
来源：http://gyt.ppjwa.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://keh.svipenyu.cn

[U49] PHP：只读属性
来源：http://mft.hongshengwenyu.top

public readonly string $name
来源：http://ert.zhengqikj.top

[U50] PHP：构造器属性提升
来源：http://wpd.andypj.xyz

public function __construct(private int $id) {}
来源：http://ouq.zdqjudy.top

[U51] PHP：数组解构
来源：http://kem.sysykeji.top

[$a, $b] = $arr;
来源：http://ctp.sweek.top

[U52] PHP：箭头函数
来源：http://pkf.gzhubu.top

$double = fn($x) => $x * 2;
来源：http://tbi.fengsongda.top

[U53] PHP：空合并运算符
来源：http://hjo.zhoulong.xyz

$v = $a ?? $b ?? "default";
来源：http://ilw.ybcxt.top

[U54] PHP：空安全调用
来源：http://kyg.c1oappe.top

$obj?->method()
来源：http://mqp.yj202588.top

[U55] PHP：match 表达式
来源：http://brq.yongpay.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://quk.kuanghao11.cn

[U56] PHP：命名参数
来源：http://ywu.chenzaomai.com

f(a: 1, b: 2)
来源：http://igz.jinqigfzy.top

[U57] PHP：字符串插值
来源：http://vng.fehbvm.com

"值: {$a}"
来源：http://hxz.cucudq.cn

[U58] PHP：数组三件套
来源：http://rez.hongshengwenyu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://efs.c1oappe.top

[U59] PHP：自定义排序
来源：http://zwk.sxryk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dok.jinqigfzy.top

[U60] PHP：JSON 编解码
来源：http://nio.hcnkem.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bpu.ehwqpu.com

[U61] PHP：正则
来源：http://pbc.jinqigufen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bxf.yj202588.top

[U62] PHP：日期对象
来源：http://ved.chenzaomai.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vnd.birdmap.top

[U63] PHP：文件读写
来源：http://iqv.zhengqikj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uzv.hysaishi.cn

[U64] PHP：目录遍历
来源：http://tqr.hongshengwenyu.top

glob("dir/*.php");  scandir("dir");
来源：http://smb.zdbjq.cn

[U65] PHP：会话
来源：http://cns.nanxinkj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rnp.jiagoushi.top

[U66] PHP：设置 Cookie
来源：http://gaz.aizwys.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aoe.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://dwk.cashguo.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jgo.fehbvm.com

[U68] PHP：PDO 连接
来源：http://cfd.shzxlz.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://itf.zhengqikj.top

[U69] PHP：PDO 预处理
来源：http://lqf.tianlin.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pwe.zhiwuduotai.top

[U70] PHP：PDO 事务
来源：http://omn.shzxlz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://myk.hysaishi.cn

[U71] PHP：抛出异常
来源：http://tav.bbcook.cn

throw new RuntimeException("失败", 500);
来源：http://ffu.mhx1999.top

[U72] PHP：写错误日志
来源：http://ewd.dashuyun.cn

error_log("失败: " . $e->getMessage());
来源：http://zlm.0kj1m.cn

[U73] PHP：读取 ini 配置
来源：http://zsd.jlsjyb.cn

parse_ini_file("config.ini", true)
来源：http://lvn.feifeiyinyue.top

[U74] PHP：读取环境变量
来源：http://jdv.tian-w.cn

getenv("APP_ENV") ?: "production"
来源：http://jpm.zdqjudy.top

[U75] PHP：依赖注入
来源：http://clp.shuidangran.top

composer require psr/container
来源：http://bsz.bjfxy.top

[U76] PHP：简单路由
来源：http://kgt.fehbvm.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://isf.yfazqb.com

[U77] PHP：模板渲染
来源：http://aqe.cucudq.cn

composer require twig/twig
来源：http://lql.pycfn.com

[U78] PHP：单元测试
来源：http://fci.ehwqpu.com

composer require --dev phpunit/phpunit
来源：http://jaz.shzxlz.cn

[U79] PHP：静态分析
来源：http://xuy.tianlin.xyz

composer require --dev phpstan/phpstan
来源：http://qrc.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://uuv.316326.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://wbn.fehbvm.com

[U81] JS：初始化项目
来源：http://tdm.chenzaomai.com

npm init -y;  npm i express
来源：http://ycd.ivvv.top

[U82] JS：package.json 脚本
来源：http://uup.hysaishi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eay.yanxiufei.cn

[U83] JS：ES Module 导入导出
来源：http://kyt.hammf.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mob.dianchejie.cn

[U84] JS：CommonJS 写法
来源：http://msj.shuidangran.top

module.exports = { a };  const { a } = require("./m");
来源：http://cok.smart0.xyz

[U85] JS：可选链
来源：http://fck.hcnkem.com

a?.b?.c
来源：http://peq.svipenyu.cn

[U86] JS：空值合并
来源：http://aiz.zhaomingkeji.xyz

a ?? b
来源：http://vsh.yongpay.top

[U87] JS：解构默认值
来源：http://jnq.xingfuxueyuan.xyz

const { a = 1, b = 2 } = obj;
来源：http://ryd.redwolf501.top

[U88] JS：对象展开合并
来源：http://bxv.hongshengwenyu.top

{ ...a, ...b }
来源：http://fda.uphjek.com

[U89] JS：数组去重
来源：http://rky.pycfn.com

[...new Set(arr)]
来源：http://bgh.sjlbkw.cn

[U90] JS：数字数组排序
来源：http://tcx.yuxming.cn

[...arr].sort((a, b) => a - b)
来源：http://lbj.sjlbkw.cn

[U91] JS：对象键值遍历
来源：http://rhr.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dxm.shanyushiyangtech.top

[U92] JS：深拷贝
来源：http://kfz.cqqwz.cn

structuredClone(obj)
来源：http://mzl.guowangkeji.top


<!-- 参考信息 -->