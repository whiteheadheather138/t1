代发 wailian999

[T05] Kotlin：when 表达式
来源：http://lbg.sweek.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uli.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://ecr.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://quw.gogol.net.cn

[T07] Kotlin：集合过滤
来源：http://nak.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zcl.daria6918.cn

[T08] Kotlin：数据类
来源：http://dwr.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://ksj.havefunace.top

[T09] Kotlin：扩展函数
来源：http://lng.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://rbo.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://htf.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ddf.sysykeji.top

[T11] Kotlin：协程
来源：http://iou.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lio.bjfxy.top

[T12] Kotlin：解构声明
来源：http://jpb.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://qpa.wangshuangyany.cn

[T13] Kotlin：只读 Map
来源：http://srq.cheryme.top

val m = mapOf("a" to 1)
来源：http://iyr.meibo888.top

[T14] Kotlin：循环
来源：http://aja.hesvh.cn

for (i in 1..10) println(i)
来源：http://ewb.dashuyun.cn

[T15] Kotlin：接口
来源：http://gef.yangfankeji.com

interface Shape { fun area(): Double }
来源：http://vog.hywenlv.cn

[T16] Swift：Hello World
来源：http://ehe.nanxinkj.top

print("Hello")
来源：http://csu.iojbl.cn

[T17] Swift：变量与常量
来源：http://sha.jianghu66.top

var a = 1;  let b = 2
来源：http://bhg.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://oeg.meibo888.top

"值: \(b)"
来源：http://vlf.cashguo.top

[T19] Swift：可选绑定
来源：http://mpk.jiagoushi.top

if let n = opt { print(n) }
来源：http://kkh.guowangkeji.top

[T20] Swift：数组操作
来源：http://jna.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://evu.jyoumei.cn

[T21] Swift：遍历
来源：http://wme.iojbl.cn

for x in a { print(x) }
来源：http://gyu.ctjpmb.com

[T22] Swift：字典
来源：http://jef.xinyue.icu

var d = ["a": 1];  d["b"] = 2
来源：http://alz.gzhubu.top

[T23] Swift：函数
来源：http://jwo.zhoulong.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zuj.feifeiyinyue.top

[T24] Swift：闭包
来源：http://wiz.quarkkingdee.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qfm.jinqigufen.top

[T25] Swift：结构体
来源：http://tfu.nanxuanxn.top

struct P { var x: Int }
来源：http://rkp.zhoulong.xyz

[T26] Swift：类与重写
来源：http://axf.cdnleiting.top

class A: Base { override func f() {} }
来源：http://vjs.nwbrower.top

[T27] Swift：错误处理
来源：http://crs.ydzc1.top

do { try f() } catch { print(error) }
来源：http://ruq.gotoacloud.top

[T28] Swift：枚举
来源：http://ggp.jinyuanbaomall.cn

enum Color { case red, green }
来源：http://vam.cashguo.top

[T29] Swift：guard 提前返回
来源：http://iat.sufxvd.cn

guard let x = opt else { return }
来源：http://jqj.hongshengwenyu.top

[T30] Swift：协议
来源：http://sqn.sufxvd.cn

protocol Shape { func area() -> Double }
来源：http://gvi.guowangkeji.top

[T31] Lua：Hello World
来源：http://yfi.hongshengwenyu.top

print("Hello")
来源：http://mjc.yongpay.top

[T32] Lua：局部变量
来源：http://aos.shangyingyoupin.top

local a = 1
来源：http://jzg.pycfn.com

[T33] Lua：表（数组）
来源：http://ogf.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://rdu.yangfankeji.com

[T34] Lua：遍历表
来源：http://mjw.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://siw.sufxvd.cn

[T35] Lua：字典表
来源：http://gxc.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://glw.hywenlv.cn

[T36] Lua：函数
来源：http://kim.ydzc1.top

function add(a, b) return a + b end
来源：http://fkk.sufxvd.cn

[T37] Lua：字符串拼接
来源：http://rgf.svipenyu.cn

"a" .. "b"
来源：http://alc.52xcode.cn

[T38] Lua：条件
来源：http://txo.zhixingplan.top

if x > 0 then print("正") end
来源：http://mnu.shzxlz.cn

[T39] Lua：模式匹配
来源：http://eev.hnxiangtu.top

string.find(s, "%d+")
来源：http://mrn.zhiwuduotai.top

[T40] Lua：元表
来源：http://brn.jianghu66.top

setmetatable({}, { __index = base })
来源：http://iiv.kuanghao11.cn

[T41] Perl：Hello World
来源：http://mdr.yueranfly.top

print "Hello\n";
来源：http://vch.cheryme.top

[T42] Perl：变量类型
来源：http://lrb.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aag.gogol.net.cn

[T43] Perl：字符串插值
来源：http://mhm.jinyuanbaomall.cn

"值: $a"
来源：http://spp.zhijiandao.cn

[T44] Perl：条件
来源：http://vqo.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://hiu.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://eyb.hesvh.cn

for my $x (@arr) { print $x; }
来源：http://lpu.zhengqikj.top

[T46] Perl：哈希操作
来源：http://qzh.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zzi.hnqzz.top

[T47] Perl：正则捕获
来源：http://daw.52xcode.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jpe.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://dgb.fehbvm.com

$s =~ s/old/new/g;
来源：http://lcl.iojbl.cn

[T49] Perl：函数
来源：http://umk.zdqjudy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fof.316326.xyz

[T50] Perl：逐行读文件
来源：http://hhj.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tpg.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://moh.nanxuanxn.top

[T51] Scala：Hello World
来源：http://tmc.zhengqikj.top

println("Hello")
来源：http://wff.tanke756.top

[T52] Scala：变量
来源：http://owo.sufxvd.cn

val a = 1;  var b = 2
来源：http://tiu.dianchejie.cn

[T53] Scala：字符串插值
来源：http://dlf.pengpengdd.cyou

s"值: $b"
来源：http://tuc.gogol.net.cn

[T54] Scala：集合映射
来源：http://mqo.9152youxi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ueh.jianghu66.top

[T55] Scala：集合过滤
来源：http://pyw.shanyushiyangkeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://lhe.ybcxt.top

[T56] Scala：样例类
来源：http://kpc.shzxlz.cn

case class User(name: String, age: Int)
来源：http://wlc.snrcjt.cn

[T57] Scala：模式匹配
来源：http://ysu.cheryme.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lad.pycfn.com

[T58] Scala：函数定义
来源：http://vsq.fzhhl.top

def add(a: Int, b: Int): Int = a + b
来源：http://lib.dashuyun.cn

[T59] Scala：循环
来源：http://vxa.yonumen.top

for (i <- 1 to 10) println(i)
来源：http://swu.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://wnw.52xcode.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fiz.zdbjq.cn

================================================================================
来源：http://nqy.ivvv.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ezl.ydzc1.top

================================================================================
来源：http://jyb.uphjek.com

[U01] Py：创建虚拟环境
来源：http://jzd.cqqwz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lyn.chenlongwang.top

[U02] Py：导出 / 安装依赖
来源：http://het.havefunace.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://duj.shangyingyoupin.top

[U03] Py：加载 .env 配置
来源：http://ihk.fzhhl.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pdr.zhiwuduotai.top

[U04] Py：变量调试打印
来源：http://cov.iojbl.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://llr.aizwys.cn

[U05] Py：列表去重且保序
来源：http://xkp.nanxuanxn.top

list(dict.fromkeys(arr))
来源：http://zio.hysaishi.cn

[U06] Py：合并两个字典
来源：http://spi.hnqzz.top

{**a, **b}
来源：http://ztc.feifeiyinyue.top

[U07] Py：反转字典键值
来源：http://xnz.dashuyun.cn

{v: k for k, v in d.items()}
来源：http://tbo.yj20258.top

[U08] Py：展平二维列表
来源：http://yev.ybcxt.top

[y for x in nested for y in x]
来源：http://oix.smart0.xyz

[U09] Py：字典取最大值的键
来源：http://owz.chenlongwang.top

max(d, key=d.get)
来源：http://fkn.yanxiufei.cn

[U10] Py：按值排序字典
来源：http://snd.hywenlv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kdx.tianlin.xyz

[U11] Py：生成器表达式
来源：http://xfn.sufxvd.cn

(x * 2 for x in arr)
来源：http://gmv.gogol.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nur.shanyushiyangkeji.top

Counter(arr).most_common(3)
来源：http://vcs.yongpay.top

[U13] Py：固定长度队列
来源：http://xnz.bjfxy.top

deque(maxlen=10)
来源：http://kvc.hywenlv.cn

[U14] Py：分组收集到列表
来源：http://tbd.tianlin.xyz

defaultdict(list)
来源：http://wjm.gogol.net.cn

[U15] Py：高精度计时
来源：http://lgy.redwolf501.top

t = time.perf_counter()
来源：http://ykg.jqgufenzy.top

[U16] Py：命令行参数解析
来源：http://nou.zhongyouzk.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rnq.daxiang520.top

[U17] Py：初始化日志
来源：http://syp.jqgufenzy.top

logging.basicConfig(level=logging.INFO)
来源：http://lhd.yangfankeji.com

[U18] Py：预编译正则
来源：http://txz.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://dgd.shanyushiyangtech.top

[U19] Py：正则替换带回调
来源：http://fya.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gmq.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://ppm.nanxuanxn.top

@functools.lru_cache(maxsize=None)
来源：http://tsn.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://abj.yangfankeji.com

@contextlib.contextmanager
来源：http://dwu.jyoumei.cn

[U22] Py：矩阵转置
来源：http://kii.uphjek.com

list(zip(*m))
来源：http://skf.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://edl.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rfl.nanxinkj.top

[U24] Py：路径操作
来源：http://uyv.uphjek.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yql.hongshengwenyu.top

[U25] Py：CSV 按字典读
来源：http://lra.nanxinkj.top

csv.DictReader(f)
来源：http://rfv.jinghuilouyu.cn

[U26] Py：并发下载
来源：http://oml.sweek.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ant.birdmap.top

[U27] Py：异步 HTTP
来源：http://vmi.wangdashe.top

aiohttp.ClientSession() 配合 async with
来源：http://fth.jinqigfzy.top

[U28] Py：类型别名
来源：http://ull.sxryk.cn

UserId = int
来源：http://yyg.ehwqpu.com

[U29] Py：属性校验
来源：http://cht.tanke756.top

@property 与 @x.setter 配合
来源：http://mph.9152youxi.cn

[U30] Py：数据类
来源：http://efb.fzhhl.top

@dataclass(slots=True)
来源：http://ggi.xingfuxueyuan.xyz

[U31] Py：单测
来源：http://nxa.snrcjt.cn

python -m pytest -q
来源：http://mwb.chenjidiqi.icu

[U32] Py：代码格式化
来源：http://vau.bjfxy.top

ruff format . && ruff check --fix .
来源：http://ooc.smart0.xyz

[U33] Py：打包发布
来源：http://pws.nanxinkj.top

python -m build  （依赖 pyproject.toml）
来源：http://yts.fzhhl.top

[U34] Py：判断编码
来源：http://nuu.ivvv.top

chardet.detect(raw)
来源：http://foc.birdmap.top

[U35] Py：发送邮件
来源：http://lzo.gogol.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yqj.tarul.cn

[U36] Py：定时任务
来源：http://bpl.daxiang520.top

schedule.every(10).minutes.do(job)
来源：http://ayj.jqgfzy.top

[U37] Py：读写 Excel
来源：http://nsg.yfazqb.com

pandas.read_excel / DataFrame.to_excel
来源：http://ojh.wangdashe.top

[U38] Py：获取脚本所在目录
来源：http://mbl.ywan-chungtsiang.top

Path(__file__).resolve().parent
来源：http://hsc.ivvv.top

[U39] Py：判断是否在交互环境
来源：http://fmy.yj20258888.top

sys.stdout.isatty()
来源：http://ahh.yvedp.cn

[U40] Py：打印到标准错误
来源：http://dus.cqqwz.cn

print("err", file=sys.stderr)
来源：http://gcx.nanxinkj.top

[U41] PHP：初始化 Composer 项目
来源：http://lwa.hysaishi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://son.zdqjudy.top

[U42] PHP：PSR-4 自动加载
来源：http://vvj.chenlongwang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pqg.ppjwa.cn

[U43] PHP：声明命名空间
来源：http://ssi.iojbl.cn

namespace App\Http;
来源：http://cjv.vqdsnc.cn

[U44] PHP：开启严格类型
来源：http://swu.jinghuilouyu.cn

declare(strict_types=1);
来源：http://oyp.ppjwa.cn

[U45] PHP：类型声明与返回类型
来源：http://hel.aibaodan.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jtn.wangdashe.top

[U46] PHP：可空类型
来源：http://lhq.jiagoushi.top

?string $name = null
来源：http://god.yj202588.top

[U47] PHP：联合类型
来源：http://twf.ybcxt.top

int|string $id
来源：http://ygy.wangdashe.top

[U48] PHP：纯枚举
来源：http://ldr.zhixingplan.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dbj.yfazqb.com

[U49] PHP：只读属性
来源：http://mzt.fktsv.cn

public readonly string $name
来源：http://yij.chenzaomai.com

[U50] PHP：构造器属性提升
来源：http://jay.fktsv.cn

public function __construct(private int $id) {}
来源：http://iyl.andypj.xyz

[U51] PHP：数组解构
来源：http://hcd.sxryk.cn

[$a, $b] = $arr;
来源：http://cus.gotoacloud.top

[U52] PHP：箭头函数
来源：http://dgr.yongpay.top

$double = fn($x) => $x * 2;
来源：http://eic.ybcxt.top

[U53] PHP：空合并运算符
来源：http://bvy.fzhhl.top

$v = $a ?? $b ?? "default";
来源：http://dtw.ppjwa.cn

[U54] PHP：空安全调用
来源：http://gfj.cqqwz.cn

$obj?->method()
来源：http://ryz.hywenlv.cn

[U55] PHP：match 表达式
来源：http://jtm.316326.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://aio.mhx1999.top

[U56] PHP：命名参数
来源：http://dal.ivvv.top

f(a: 1, b: 2)
来源：http://zpr.guannengcc.top

[U57] PHP：字符串插值
来源：http://afw.guannengcc.top

"值: {$a}"
来源：http://tdf.shzxlz.cn

[U58] PHP：数组三件套
来源：http://ucp.sjlbkw.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rqo.hnxiangtu.top

[U59] PHP：自定义排序
来源：http://ner.yfazqb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qhg.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://uzw.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fbh.fengsongda.top

[U61] PHP：正则
来源：http://yvz.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dqv.sjlbkw.cn

[U62] PHP：日期对象
来源：http://cyg.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bbs.fzhhl.top

[U63] PHP：文件读写
来源：http://bdg.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bps.cqqwz.cn

[U64] PHP：目录遍历
来源：http://fjh.zhengqikj.top

glob("dir/*.php");  scandir("dir");
来源：http://jdw.cheryme.top

[U65] PHP：会话
来源：http://wev.hnxiangtu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ahm.yongpay.top

[U66] PHP：设置 Cookie
来源：http://rox.pengpengdd.cyou

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://svb.hysaishi.cn

[U67] PHP：处理文件上传
来源：http://hpp.zhixingplan.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kug.dianchejie.cn

[U68] PHP：PDO 连接
来源：http://fhd.ivvv.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vek.vehdjk.com

[U69] PHP：PDO 预处理
来源：http://klr.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yiq.cheryme.top

[U70] PHP：PDO 事务
来源：http://ybm.vqdsnc.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://knd.haohaochexian.top

[U71] PHP：抛出异常
来源：http://lxe.gogol.net.cn

throw new RuntimeException("失败", 500);
来源：http://nvs.zhixingplan.top

[U72] PHP：写错误日志
来源：http://lhb.snrcjt.cn

error_log("失败: " . $e->getMessage());
来源：http://iuj.vqdsnc.cn

[U73] PHP：读取 ini 配置
来源：http://mul.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://afo.snrcjt.cn

[U74] PHP：读取环境变量
来源：http://ulh.fengsongda.top

getenv("APP_ENV") ?: "production"
来源：http://jrn.uphjek.com

[U75] PHP：依赖注入
来源：http://jde.haohaochexian.top

composer require psr/container
来源：http://nfl.hcnkem.com

[U76] PHP：简单路由
来源：http://cut.shanyushiyangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qrx.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://enq.gaohongyu789.top

composer require twig/twig
来源：http://dsp.chenjidiqi.icu

[U78] PHP：单元测试
来源：http://mvu.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://ixw.mhx1999.top

[U79] PHP：静态分析
来源：http://ktf.aibaodan.cn

composer require --dev phpstan/phpstan
来源：http://qqh.9152youxi.cn

[U80] PHP：代码规范修复
来源：http://mdu.ppjwa.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wal.meibo888.top

[U81] JS：初始化项目
来源：http://usu.shzxlz.cn

npm init -y;  npm i express
来源：http://cqj.jqgufenzy.top

[U82] JS：package.json 脚本
来源：http://mrk.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://spl.cqqwz.cn

[U83] JS：ES Module 导入导出
来源：http://far.kuanghao11.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dvz.zhaomingkeji.xyz

[U84] JS：CommonJS 写法
来源：http://jyi.tian-w.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xve.9152youxi.cn

[U85] JS：可选链
来源：http://gmi.nwbrower.top

a?.b?.c
来源：http://dja.iojbl.cn

[U86] JS：空值合并
来源：http://eyk.quarkkingdee.top

a ?? b
来源：http://tdl.zdbjq.cn

[U87] JS：解构默认值
来源：http://jvi.cheryme.top

const { a = 1, b = 2 } = obj;
来源：http://dye.sweek.top

[U88] JS：对象展开合并
来源：http://jcm.fengsongda.top

{ ...a, ...b }
来源：http://myd.yangfankeji.com

[U89] JS：数组去重
来源：http://ppc.zhixingplan.top

[...new Set(arr)]
来源：http://irb.daxiang520.top

[U90] JS：数字数组排序
来源：http://prt.epnwcf.com

[...arr].sort((a, b) => a - b)
来源：http://ynp.redwolf501.top

[U91] JS：对象键值遍历
来源：http://cqt.cucudq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ndj.yvedp.cn

[U92] JS：深拷贝
来源：http://sec.zhijiandao.cn

structuredClone(obj)
来源：http://akk.gzhubu.top


<!-- 参考信息 -->