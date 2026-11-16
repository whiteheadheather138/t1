代发 wailian999

[T05] Kotlin：when 表达式
来源：http://wnm.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iyj.shangyingyoupin.top

[T06] Kotlin：集合映射
来源：http://ojp.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bmq.nanxuanxn.top

[T07] Kotlin：集合过滤
来源：http://oka.jianghu66.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xji.jyoumei.cn

[T08] Kotlin：数据类
来源：http://zip.hammf.cn

data class User(val name: String, val age: Int)
来源：http://xmw.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://uiu.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://ego.hfpthk.cn

[T10] Kotlin：默认参数
来源：http://pts.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mjm.yuxming.cn

[T11] Kotlin：协程
来源：http://tfv.jianghu66.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mrm.sweek.top

[T12] Kotlin：解构声明
来源：http://uwm.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://lml.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://apg.jinqigfzy.top

val m = mapOf("a" to 1)
来源：http://fwb.yj20258.top

[T14] Kotlin：循环
来源：http://szg.sxryk.cn

for (i in 1..10) println(i)
来源：http://uuk.cheryme.top

[T15] Kotlin：接口
来源：http://mgb.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://gzb.zhiwuduotai.top

[T16] Swift：Hello World
来源：http://njd.yuanzhike.top

print("Hello")
来源：http://xxu.yongpay.top

[T17] Swift：变量与常量
来源：http://ear.jinqigfzy.top

var a = 1;  let b = 2
来源：http://ubg.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://log.hywenlv.cn

"值: \(b)"
来源：http://naw.ehwqpu.com

[T19] Swift：可选绑定
来源：http://pds.shanyushiyangkeji.top

if let n = opt { print(n) }
来源：http://qyw.nanxuanxn.top

[T20] Swift：数组操作
来源：http://dpy.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://eig.cheryme.top

[T21] Swift：遍历
来源：http://fmb.fanxiaobao.xyz

for x in a { print(x) }
来源：http://nvh.epnwcf.com

[T22] Swift：字典
来源：http://jht.jinqigufen.top

var d = ["a": 1];  d["b"] = 2
来源：http://pyh.sxryk.cn

[T23] Swift：函数
来源：http://zbt.ehwqpu.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jxr.daxiang520.top

[T24] Swift：闭包
来源：http://poy.shuidangran.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kte.bjfxy.top

[T25] Swift：结构体
来源：http://dal.fzhhl.top

struct P { var x: Int }
来源：http://ahg.ehwqpu.com

[T26] Swift：类与重写
来源：http://tqt.0kj1m.cn

class A: Base { override func f() {} }
来源：http://lke.ivvv.top

[T27] Swift：错误处理
来源：http://oey.shuidangran.top

do { try f() } catch { print(error) }
来源：http://jvq.sysykeji.top

[T28] Swift：枚举
来源：http://knj.sysykeji.top

enum Color { case red, green }
来源：http://fex.svipenyu.cn

[T29] Swift：guard 提前返回
来源：http://gqp.shangyingyoupin.top

guard let x = opt else { return }
来源：http://lek.wangdashe.top

[T30] Swift：协议
来源：http://ela.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://gaw.hnxiangtu.top

[T31] Lua：Hello World
来源：http://qwn.jinqigfzy.top

print("Hello")
来源：http://hgd.kuanghao11.cn

[T32] Lua：局部变量
来源：http://our.gaohongyu789.top

local a = 1
来源：http://ppt.dashuyun.cn

[T33] Lua：表（数组）
来源：http://smi.yueranfly.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cvo.zdqjudy.top

[T34] Lua：遍历表
来源：http://nah.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tnm.0kj1m.cn

[T35] Lua：字典表
来源：http://hjm.yuxming.cn

local d = { a = 1 };  d.b = 2
来源：http://vqx.wangdashe.top

[T36] Lua：函数
来源：http://vys.sweek.top

function add(a, b) return a + b end
来源：http://bao.yangfankeji.com

[T37] Lua：字符串拼接
来源：http://bti.yuxming.cn

"a" .. "b"
来源：http://nmh.jqgfzy.top

[T38] Lua：条件
来源：http://rqu.cashguo.top

if x > 0 then print("正") end
来源：http://swr.mhx1999.top

[T39] Lua：模式匹配
来源：http://eey.feifeiyinyue.top

string.find(s, "%d+")
来源：http://mkf.andypj.xyz

[T40] Lua：元表
来源：http://auk.snrcjt.cn

setmetatable({}, { __index = base })
来源：http://val.nanxuanxn.top

[T41] Perl：Hello World
来源：http://yas.jianghu66.top

print "Hello\n";
来源：http://rhq.aibaodan.cn

[T42] Perl：变量类型
来源：http://yag.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://asl.aibaodan.cn

[T43] Perl：字符串插值
来源：http://zkg.meibo888.top

"值: $a"
来源：http://nvb.zhixingplan.top

[T44] Perl：条件
来源：http://ykt.316326.xyz

if ($a > 0) { print "正"; }
来源：http://vsm.jqgufenzy.top

[T45] Perl：数组遍历
来源：http://wgt.xingfuxueyuan.xyz

for my $x (@arr) { print $x; }
来源：http://emz.ehwqpu.com

[T46] Perl：哈希操作
来源：http://pad.zycfv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ivm.ctjpmb.com

[T47] Perl：正则捕获
来源：http://alb.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://coq.redwolf501.top

[T48] Perl：正则替换
来源：http://vak.yuxming.cn

$s =~ s/old/new/g;
来源：http://ttm.pengpengdd.cyou

[T49] Perl：函数
来源：http://mao.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://joh.hysaishi.cn

[T50] Perl：逐行读文件
来源：http://tms.andypj.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://ltu.jianghu66.top

while (my $line = <$fh>) { print $line; }
来源：http://rip.ywan-chungtsiang.top

[T51] Scala：Hello World
来源：http://rgc.andypj.xyz

println("Hello")
来源：http://brh.cqqwz.cn

[T52] Scala：变量
来源：http://uca.zhijiandao.cn

val a = 1;  var b = 2
来源：http://lmi.guannengcc.top

[T53] Scala：字符串插值
来源：http://tzu.fehbvm.com

s"值: $b"
来源：http://ypd.sufxvd.cn

[T54] Scala：集合映射
来源：http://dac.yueranfly.top

List(1, 2, 3).map(_ * 2)
来源：http://aeu.dianchejie.cn

[T55] Scala：集合过滤
来源：http://dio.fehbvm.com

List(1, 2, 3).filter(_ > 1)
来源：http://lex.jinqigfzy.top

[T56] Scala：样例类
来源：http://ieh.xylfe.cn

case class User(name: String, age: Int)
来源：http://fck.hammf.cn

[T57] Scala：模式匹配
来源：http://kca.hywenlv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kmy.ehwqpu.com

[T58] Scala：函数定义
来源：http://iis.xuetiantiany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gnq.cdnleiting.top

[T59] Scala：循环
来源：http://rfp.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://jzi.ydzc1.top

[T60] Scala：折叠
来源：http://tvs.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ozl.hnxiangtu.top

================================================================================
来源：http://ime.jqgufenzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://emp.shanyushiyangtech.top

================================================================================
来源：http://tzd.zhijiandao.cn

[U01] Py：创建虚拟环境
来源：http://wcr.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vsx.jyoumei.cn

[U02] Py：导出 / 安装依赖
来源：http://vlc.hammf.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ikp.gzhubu.top

[U03] Py：加载 .env 配置
来源：http://ehg.yanxiufei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yul.fktsv.cn

[U04] Py：变量调试打印
来源：http://luc.tianlin.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ing.ehwqpu.com

[U05] Py：列表去重且保序
来源：http://pyb.cucudq.cn

list(dict.fromkeys(arr))
来源：http://ofb.hammf.cn

[U06] Py：合并两个字典
来源：http://jef.fzhhl.top

{**a, **b}
来源：http://inb.xinyue.icu

[U07] Py：反转字典键值
来源：http://ofl.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://heq.uphjek.com

[U08] Py：展平二维列表
来源：http://can.ivvv.top

[y for x in nested for y in x]
来源：http://ksd.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://xvp.xingfuxueyuan.xyz

max(d, key=d.get)
来源：http://qca.wangdashe.top

[U10] Py：按值排序字典
来源：http://tlt.jiagoushi.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zbx.yongpay.top

[U11] Py：生成器表达式
来源：http://hse.zhongyouzk.top

(x * 2 for x in arr)
来源：http://ctk.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://qiz.hysaishi.cn

Counter(arr).most_common(3)
来源：http://leh.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://bnq.yj202588.top

deque(maxlen=10)
来源：http://wmb.jyoumei.cn

[U14] Py：分组收集到列表
来源：http://uvb.zhengqikj.top

defaultdict(list)
来源：http://eju.9152youxi.cn

[U15] Py：高精度计时
来源：http://ast.cdnleiting.top

t = time.perf_counter()
来源：http://ibz.hfpthk.cn

[U16] Py：命令行参数解析
来源：http://csq.xziqi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://clc.snrcjt.cn

[U17] Py：初始化日志
来源：http://nsq.tianlin.xyz

logging.basicConfig(level=logging.INFO)
来源：http://mcq.haohaochexian.top

[U18] Py：预编译正则
来源：http://vij.jinqigufen.top

pat = re.compile(r"\d+")
来源：http://spf.shzxlz.cn

[U19] Py：正则替换带回调
来源：http://zdh.hfpthk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sew.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://cul.xuetiantiany.cn

@functools.lru_cache(maxsize=None)
来源：http://mzf.yueranfly.top

[U21] Py：自定义上下文管理器
来源：http://qgx.jiagoushi.top

@contextlib.contextmanager
来源：http://bra.tianlin.xyz

[U22] Py：矩阵转置
来源：http://rak.aizwys.cn

list(zip(*m))
来源：http://wzf.sysykeji.top

[U23] Py：分块读取大文件
来源：http://fec.yangfankeji.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://svh.hesvh.cn

[U24] Py：路径操作
来源：http://fmu.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://itq.zhengqikj.top

[U25] Py：CSV 按字典读
来源：http://zny.smart0.xyz

csv.DictReader(f)
来源：http://bfj.jinqigfzy.top

[U26] Py：并发下载
来源：http://krd.bjfxy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xuc.52xcode.cn

[U27] Py：异步 HTTP
来源：http://avr.jlsjyb.cn

aiohttp.ClientSession() 配合 async with
来源：http://rwm.cheryme.top

[U28] Py：类型别名
来源：http://fsc.bjfxy.top

UserId = int
来源：http://xuf.ydjk.org.cn

[U29] Py：属性校验
来源：http://vkx.tian-w.cn

@property 与 @x.setter 配合
来源：http://nfm.hammf.cn

[U30] Py：数据类
来源：http://jxg.mhx1999.top

@dataclass(slots=True)
来源：http://rkn.hongshengwenyu.top

[U31] Py：单测
来源：http://uww.xinyue.icu

python -m pytest -q
来源：http://aoq.yanxiufei.cn

[U32] Py：代码格式化
来源：http://xpb.bjfxy.top

ruff format . && ruff check --fix .
来源：http://yau.yongpay.top

[U33] Py：打包发布
来源：http://xuz.nanxuanxn.top

python -m build  （依赖 pyproject.toml）
来源：http://iml.zhijiandao.cn

[U34] Py：判断编码
来源：http://xmr.fanxiaobao.xyz

chardet.detect(raw)
来源：http://ugx.shuidangran.top

[U35] Py：发送邮件
来源：http://zll.hcnkem.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vnx.redwolf501.top

[U36] Py：定时任务
来源：http://vps.xingfuxueyuan.xyz

schedule.every(10).minutes.do(job)
来源：http://yra.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://ykt.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uwe.kuanghao11.cn

[U38] Py：获取脚本所在目录
来源：http://egi.dashuyun.cn

Path(__file__).resolve().parent
来源：http://igc.hcnkem.com

[U39] Py：判断是否在交互环境
来源：http://igp.smart0.xyz

sys.stdout.isatty()
来源：http://tiy.smart0.xyz

[U40] Py：打印到标准错误
来源：http://tif.xuetiantiany.cn

print("err", file=sys.stderr)
来源：http://ixf.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://glk.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vrd.redwolf501.top

[U42] PHP：PSR-4 自动加载
来源：http://ate.bjfxy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jqn.chenzaomai.com

[U43] PHP：声明命名空间
来源：http://rus.sjlbkw.cn

namespace App\Http;
来源：http://cbm.shuidangran.top

[U44] PHP：开启严格类型
来源：http://gzk.andypj.xyz

declare(strict_types=1);
来源：http://jqd.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://odw.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://xux.uphjek.com

[U46] PHP：可空类型
来源：http://pki.gzhubu.top

?string $name = null
来源：http://ppy.kuanghao11.cn

[U47] PHP：联合类型
来源：http://rlk.hywenlv.cn

int|string $id
来源：http://nux.0kj1m.cn

[U48] PHP：纯枚举
来源：http://fcc.jqgfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://szq.uphjek.com

[U49] PHP：只读属性
来源：http://yab.tian-w.cn

public readonly string $name
来源：http://exk.ppjwa.cn

[U50] PHP：构造器属性提升
来源：http://bsw.mhx1999.top

public function __construct(private int $id) {}
来源：http://dhi.zhixingplan.top

[U51] PHP：数组解构
来源：http://esc.meibo888.top

[$a, $b] = $arr;
来源：http://xkm.daxiang520.top

[U52] PHP：箭头函数
来源：http://fkw.hammf.cn

$double = fn($x) => $x * 2;
来源：http://wuy.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://cry.ywan-chungtsiang.top

$v = $a ?? $b ?? "default";
来源：http://fvf.xuanzx.com

[U54] PHP：空安全调用
来源：http://ffz.svipenyu.cn

$obj?->method()
来源：http://ndy.yuxming.cn

[U55] PHP：match 表达式
来源：http://rxb.shuidangran.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uvk.vqdsnc.cn

[U56] PHP：命名参数
来源：http://lrf.haohaochexian.top

f(a: 1, b: 2)
来源：http://aib.redwolf501.top

[U57] PHP：字符串插值
来源：http://ahe.vqdsnc.cn

"值: {$a}"
来源：http://qgc.epnwcf.com

[U58] PHP：数组三件套
来源：http://jky.nanxinkj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://khs.svipenyu.cn

[U59] PHP：自定义排序
来源：http://lti.hnqzz.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zjw.yvedp.cn

[U60] PHP：JSON 编解码
来源：http://ela.feifeiyinyue.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ecy.jyoumei.cn

[U61] PHP：正则
来源：http://bja.hnxiangtu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mxy.zhoulong.xyz

[U62] PHP：日期对象
来源：http://gqg.kuanghao11.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dck.feifeiyinyue.top

[U63] PHP：文件读写
来源：http://axb.birdmap.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sma.snrcjt.cn

[U64] PHP：目录遍历
来源：http://ynd.zycfv.cn

glob("dir/*.php");  scandir("dir");
来源：http://jna.dashuyun.cn

[U65] PHP：会话
来源：http://oki.zhaomingkeji.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://cxg.vehdjk.com

[U66] PHP：设置 Cookie
来源：http://snb.havefunace.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tmn.cqqwz.cn

[U67] PHP：处理文件上传
来源：http://moh.yvedp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vci.hammf.cn

[U68] PHP：PDO 连接
来源：http://xda.sjlbkw.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tnk.birdmap.top

[U69] PHP：PDO 预处理
来源：http://vhb.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fcg.shangyingyoupin.top

[U70] PHP：PDO 事务
来源：http://ifh.epnwcf.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://twx.yj202588.top

[U71] PHP：抛出异常
来源：http://wdd.svipenyu.cn

throw new RuntimeException("失败", 500);
来源：http://hah.yonumen.top

[U72] PHP：写错误日志
来源：http://ggf.fanxiaobao.xyz

error_log("失败: " . $e->getMessage());
来源：http://vte.chenlongwang.top

[U73] PHP：读取 ini 配置
来源：http://kgq.jyoumei.cn

parse_ini_file("config.ini", true)
来源：http://xyq.redwolf501.top

[U74] PHP：读取环境变量
来源：http://yoe.kuanghao11.cn

getenv("APP_ENV") ?: "production"
来源：http://jnt.zhaomingkeji.xyz

[U75] PHP：依赖注入
来源：http://qde.hnqzz.top

composer require psr/container
来源：http://vra.ppjwa.cn

[U76] PHP：简单路由
来源：http://jos.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kdl.yuanzhike.top

[U77] PHP：模板渲染
来源：http://fma.c1oappe.top

composer require twig/twig
来源：http://nfr.havefunace.top

[U78] PHP：单元测试
来源：http://fxq.sufxvd.cn

composer require --dev phpunit/phpunit
来源：http://trb.guowangkeji.top

[U79] PHP：静态分析
来源：http://qsq.yongpay.top

composer require --dev phpstan/phpstan
来源：http://ibs.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://pew.yj202588.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://soi.sysykeji.top

[U81] JS：初始化项目
来源：http://xxf.meibo888.top

npm init -y;  npm i express
来源：http://rfs.zhongyouzk.top

[U82] JS：package.json 脚本
来源：http://jiu.jinqigfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kpz.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://wei.sjlbkw.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hdl.havefunace.top

[U84] JS：CommonJS 写法
来源：http://cgk.fzhhl.top

module.exports = { a };  const { a } = require("./m");
来源：http://xek.hongshengwenyu.top

[U85] JS：可选链
来源：http://mps.xuetiantiany.cn

a?.b?.c
来源：http://zxx.yuanzhike.top

[U86] JS：空值合并
来源：http://ywo.hysaishi.cn

a ?? b
来源：http://sto.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://wsp.hysaishi.cn

const { a = 1, b = 2 } = obj;
来源：http://psh.yueranfly.top

[U88] JS：对象展开合并
来源：http://mus.gotoacloud.top

{ ...a, ...b }
来源：http://pgm.mhx1999.top

[U89] JS：数组去重
来源：http://jpw.tanke756.top

[...new Set(arr)]
来源：http://zec.pengpengdd.cyou

[U90] JS：数字数组排序
来源：http://ops.0kj1m.cn

[...arr].sort((a, b) => a - b)
来源：http://wiz.zhongyouzk.top

[U91] JS：对象键值遍历
来源：http://yvt.vehdjk.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://luq.vqdsnc.cn

[U92] JS：深拷贝
来源：http://lzy.yonumen.top

structuredClone(obj)
来源：http://aou.vehdjk.com


<!-- 参考信息 -->