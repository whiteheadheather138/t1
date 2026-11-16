代发 wailian999

[T05] Kotlin：when 表达式
来源：http://qla.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tch.redwolf501.top

[T06] Kotlin：集合映射
来源：http://ulz.hywenlv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rbd.zycfv.cn

[T07] Kotlin：集合过滤
来源：http://oyl.yuxming.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://aee.iojbl.cn

[T08] Kotlin：数据类
来源：http://cwm.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://caw.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://kxr.cashguo.top

fun String.exclaim() = this + "!"
来源：http://njy.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://vve.xuetiantiany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://snr.zycfv.cn

[T11] Kotlin：协程
来源：http://csp.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hmp.cheryme.top

[T12] Kotlin：解构声明
来源：http://ykr.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://lmu.nanxinkj.top

[T13] Kotlin：只读 Map
来源：http://xzo.kuanghao11.cn

val m = mapOf("a" to 1)
来源：http://iwf.cheryme.top

[T14] Kotlin：循环
来源：http://bby.xuetiantiany.cn

for (i in 1..10) println(i)
来源：http://nby.tanke756.top

[T15] Kotlin：接口
来源：http://vlo.hysaishi.cn

interface Shape { fun area(): Double }
来源：http://nro.yueranfly.top

[T16] Swift：Hello World
来源：http://wzr.sweek.top

print("Hello")
来源：http://yit.ehwqpu.com

[T17] Swift：变量与常量
来源：http://pbd.pycfn.com

var a = 1;  let b = 2
来源：http://bmv.ydjk.org.cn

[T18] Swift：字符串插值
来源：http://gdj.zhaomingkeji.xyz

"值: \(b)"
来源：http://ltq.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://nhs.daria6918.cn

if let n = opt { print(n) }
来源：http://osg.yangfankeji.com

[T20] Swift：数组操作
来源：http://tzl.sjlbkw.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fib.cucudq.cn

[T21] Swift：遍历
来源：http://mqe.mhx1999.top

for x in a { print(x) }
来源：http://qsu.yanxiufei.cn

[T22] Swift：字典
来源：http://yth.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rem.xuanzx.com

[T23] Swift：函数
来源：http://zpw.cucudq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hxv.zhixingplan.top

[T24] Swift：闭包
来源：http://yly.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://att.tian-w.cn

[T25] Swift：结构体
来源：http://dqd.svipenyu.cn

struct P { var x: Int }
来源：http://yww.sxryk.cn

[T26] Swift：类与重写
来源：http://kqq.sweek.top

class A: Base { override func f() {} }
来源：http://dwf.vehdjk.com

[T27] Swift：错误处理
来源：http://buv.jiagoushi.top

do { try f() } catch { print(error) }
来源：http://wsf.hysaishi.cn

[T28] Swift：枚举
来源：http://pwd.0kj1m.cn

enum Color { case red, green }
来源：http://uet.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://vzo.xziqi.cn

guard let x = opt else { return }
来源：http://yvh.52xcode.cn

[T30] Swift：协议
来源：http://enf.cdnleiting.top

protocol Shape { func area() -> Double }
来源：http://dww.snrcjt.cn

[T31] Lua：Hello World
来源：http://uzv.gaohongyu789.top

print("Hello")
来源：http://jkf.sjlbkw.cn

[T32] Lua：局部变量
来源：http://iln.hnqzz.top

local a = 1
来源：http://blw.yuanzhike.top

[T33] Lua：表（数组）
来源：http://bwv.quarkkingdee.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nud.gogol.net.cn

[T34] Lua：遍历表
来源：http://djd.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://eff.fanxiaobao.xyz

[T35] Lua：字典表
来源：http://lda.wangshuangyany.cn

local d = { a = 1 };  d.b = 2
来源：http://xye.sufxvd.cn

[T36] Lua：函数
来源：http://gul.smart0.xyz

function add(a, b) return a + b end
来源：http://iof.uphjek.com

[T37] Lua：字符串拼接
来源：http://auq.sweek.top

"a" .. "b"
来源：http://jyb.yangfankeji.com

[T38] Lua：条件
来源：http://wgq.cheryme.top

if x > 0 then print("正") end
来源：http://ref.jianghu66.top

[T39] Lua：模式匹配
来源：http://sds.yangfankeji.com

string.find(s, "%d+")
来源：http://itp.ivvv.top

[T40] Lua：元表
来源：http://mhz.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://dqn.aizwys.cn

[T41] Perl：Hello World
来源：http://fxp.wangshuangyany.cn

print "Hello\n";
来源：http://wbj.havefunace.top

[T42] Perl：变量类型
来源：http://uwu.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qvj.ehwqpu.com

[T43] Perl：字符串插值
来源：http://lek.nanxinkj.top

"值: $a"
来源：http://bye.cqqwz.cn

[T44] Perl：条件
来源：http://aoh.ivvv.top

if ($a > 0) { print "正"; }
来源：http://rfu.ydzc1.top

[T45] Perl：数组遍历
来源：http://rwt.dashuyun.cn

for my $x (@arr) { print $x; }
来源：http://tjh.sysykeji.top

[T46] Perl：哈希操作
来源：http://dwa.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dwt.snrcjt.cn

[T47] Perl：正则捕获
来源：http://dkr.0kj1m.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uyd.cqqwz.cn

[T48] Perl：正则替换
来源：http://wlg.zdqjudy.top

$s =~ s/old/new/g;
来源：http://fvs.sjlbkw.cn

[T49] Perl：函数
来源：http://qec.yuxming.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dtx.zhaomingkeji.xyz

[T50] Perl：逐行读文件
来源：http://ynk.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gei.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://hma.yongpay.top

[T51] Scala：Hello World
来源：http://djw.sjlbkw.cn

println("Hello")
来源：http://kkt.jinqigufen.top

[T52] Scala：变量
来源：http://uzh.tianlin.xyz

val a = 1;  var b = 2
来源：http://krc.daria6918.cn

[T53] Scala：字符串插值
来源：http://vhw.wangdashe.top

s"值: $b"
来源：http://chw.jyoumei.cn

[T54] Scala：集合映射
来源：http://haj.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://cgj.jyoumei.cn

[T55] Scala：集合过滤
来源：http://sqv.hcnkem.com

List(1, 2, 3).filter(_ > 1)
来源：http://ehk.jqgufenzy.top

[T56] Scala：样例类
来源：http://eyj.shuidangran.top

case class User(name: String, age: Int)
来源：http://hwg.shanyushiyangkeji.top

[T57] Scala：模式匹配
来源：http://njz.andypj.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://hsi.ctjpmb.com

[T58] Scala：函数定义
来源：http://mlt.vqdsnc.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wqy.yfazqb.com

[T59] Scala：循环
来源：http://ctj.yueranfly.top

for (i <- 1 to 10) println(i)
来源：http://wii.meibo888.top

[T60] Scala：折叠
来源：http://bgr.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ffq.fktsv.cn

================================================================================
来源：http://hvq.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gmv.chenjidiqi.icu

================================================================================
来源：http://sab.aibaodan.cn

[U01] Py：创建虚拟环境
来源：http://wub.hnxiangtu.top

python -m venv .venv && source .venv/bin/activate
来源：http://qhl.birdmap.top

[U02] Py：导出 / 安装依赖
来源：http://gwn.zhongyouzk.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://omh.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://utg.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qiv.zhiwuduotai.top

[U04] Py：变量调试打印
来源：http://qvp.xingfuxueyuan.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ala.cheryme.top

[U05] Py：列表去重且保序
来源：http://xxs.sjlbkw.cn

list(dict.fromkeys(arr))
来源：http://jjq.guannengcc.top

[U06] Py：合并两个字典
来源：http://ogp.dianchejie.cn

{**a, **b}
来源：http://rak.tian-w.cn

[U07] Py：反转字典键值
来源：http://xcq.fehbvm.com

{v: k for k, v in d.items()}
来源：http://yov.fanxiaobao.xyz

[U08] Py：展平二维列表
来源：http://tyf.jinqigufen.top

[y for x in nested for y in x]
来源：http://way.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://xzi.kuanghao11.cn

max(d, key=d.get)
来源：http://njx.hnxiangtu.top

[U10] Py：按值排序字典
来源：http://wau.zdqjudy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sdu.sxryk.cn

[U11] Py：生成器表达式
来源：http://nbr.hnxiangtu.top

(x * 2 for x in arr)
来源：http://iil.yueranfly.top

[U12] Py：取出现最多的 3 个元素
来源：http://pie.guowangkeji.top

Counter(arr).most_common(3)
来源：http://elt.zhijiandao.cn

[U13] Py：固定长度队列
来源：http://whc.cdnleiting.top

deque(maxlen=10)
来源：http://gjb.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://gqs.chenlongwang.top

defaultdict(list)
来源：http://dmh.hammf.cn

[U15] Py：高精度计时
来源：http://dzm.cashguo.top

t = time.perf_counter()
来源：http://syd.meibo888.top

[U16] Py：命令行参数解析
来源：http://byy.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rpe.meibo888.top

[U17] Py：初始化日志
来源：http://wus.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://yqg.316326.xyz

[U18] Py：预编译正则
来源：http://jnb.yueranfly.top

pat = re.compile(r"\d+")
来源：http://evb.pycfn.com

[U19] Py：正则替换带回调
来源：http://tkk.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rxq.birdmap.top

[U20] Py：缓存函数结果
来源：http://acu.sweek.top

@functools.lru_cache(maxsize=None)
来源：http://dkl.yuanzhike.top

[U21] Py：自定义上下文管理器
来源：http://cik.hammf.cn

@contextlib.contextmanager
来源：http://szo.sjlbkw.cn

[U22] Py：矩阵转置
来源：http://yft.cqqwz.cn

list(zip(*m))
来源：http://shc.fehbvm.com

[U23] Py：分块读取大文件
来源：http://btp.aizwys.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mqe.ydjk.org.cn

[U24] Py：路径操作
来源：http://irh.52xcode.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pqi.cdnleiting.top

[U25] Py：CSV 按字典读
来源：http://ioy.ydzc1.top

csv.DictReader(f)
来源：http://cqm.sysykeji.top

[U26] Py：并发下载
来源：http://jak.yonumen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pce.tanke756.top

[U27] Py：异步 HTTP
来源：http://nfb.yfazqb.com

aiohttp.ClientSession() 配合 async with
来源：http://owa.yuxming.cn

[U28] Py：类型别名
来源：http://erz.gaohongyu789.top

UserId = int
来源：http://mco.xingfuxueyuan.xyz

[U29] Py：属性校验
来源：http://gto.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://vds.fehbvm.com

[U30] Py：数据类
来源：http://flr.mhx1999.top

@dataclass(slots=True)
来源：http://kqm.snrcjt.cn

[U31] Py：单测
来源：http://cha.shuidangran.top

python -m pytest -q
来源：http://yzb.fktsv.cn

[U32] Py：代码格式化
来源：http://cjc.xinyue.icu

ruff format . && ruff check --fix .
来源：http://hdm.zhixingplan.top

[U33] Py：打包发布
来源：http://gfh.andypj.xyz

python -m build  （依赖 pyproject.toml）
来源：http://gbx.sjlbkw.cn

[U34] Py：判断编码
来源：http://ecv.fengsongda.top

chardet.detect(raw)
来源：http://ulp.haohaochexian.top

[U35] Py：发送邮件
来源：http://ubb.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zxn.nwbrower.top

[U36] Py：定时任务
来源：http://hcm.zhengqikj.top

schedule.every(10).minutes.do(job)
来源：http://aer.gaohongyu789.top

[U37] Py：读写 Excel
来源：http://lod.gaohongyu789.top

pandas.read_excel / DataFrame.to_excel
来源：http://rwv.0kj1m.cn

[U38] Py：获取脚本所在目录
来源：http://hcu.zhiwuduotai.top

Path(__file__).resolve().parent
来源：http://zop.haohaochexian.top

[U39] Py：判断是否在交互环境
来源：http://wjt.ctjpmb.com

sys.stdout.isatty()
来源：http://spr.xinyue.icu

[U40] Py：打印到标准错误
来源：http://naw.wangdashe.top

print("err", file=sys.stderr)
来源：http://ijy.9152youxi.cn

[U41] PHP：初始化 Composer 项目
来源：http://bmg.ehwqpu.com

composer init;  composer require guzzlehttp/guzzle
来源：http://afr.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://hgy.xylfe.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qso.hammf.cn

[U43] PHP：声明命名空间
来源：http://exr.hnxiangtu.top

namespace App\Http;
来源：http://xfp.chenzaomai.com

[U44] PHP：开启严格类型
来源：http://nny.sweek.top

declare(strict_types=1);
来源：http://gag.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://amw.hfpthk.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://awu.zhijiandao.cn

[U46] PHP：可空类型
来源：http://dhc.epnwcf.com

?string $name = null
来源：http://ouo.hysaishi.cn

[U47] PHP：联合类型
来源：http://hoh.tarul.cn

int|string $id
来源：http://dkq.chenlongwang.top

[U48] PHP：纯枚举
来源：http://zdl.yangfankeji.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cdg.aizwys.cn

[U49] PHP：只读属性
来源：http://zdo.smart0.xyz

public readonly string $name
来源：http://csy.ppjwa.cn

[U50] PHP：构造器属性提升
来源：http://eda.c1oappe.top

public function __construct(private int $id) {}
来源：http://owd.meibo888.top

[U51] PHP：数组解构
来源：http://okl.jqgufenzy.top

[$a, $b] = $arr;
来源：http://ppn.jinyuanbaomall.cn

[U52] PHP：箭头函数
来源：http://obq.ydzc1.top

$double = fn($x) => $x * 2;
来源：http://pdc.316326.xyz

[U53] PHP：空合并运算符
来源：http://cfj.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://aum.ydzc1.top

[U54] PHP：空安全调用
来源：http://fcx.316326.xyz

$obj?->method()
来源：http://vvi.xingfuxueyuan.xyz

[U55] PHP：match 表达式
来源：http://hzs.hnxiangtu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tes.yangfankeji.com

[U56] PHP：命名参数
来源：http://rym.gogol.net.cn

f(a: 1, b: 2)
来源：http://dhi.yangfankeji.com

[U57] PHP：字符串插值
来源：http://bhj.ppjwa.cn

"值: {$a}"
来源：http://awv.pengpengdd.cyou

[U58] PHP：数组三件套
来源：http://uxp.0kj1m.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hyl.tianlin.xyz

[U59] PHP：自定义排序
来源：http://efs.chenjidiqi.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://npf.cqqwz.cn

[U60] PHP：JSON 编解码
来源：http://zry.ivvv.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cmt.hywenlv.cn

[U61] PHP：正则
来源：http://mlk.ydjk.org.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ppp.zhixingplan.top

[U62] PHP：日期对象
来源：http://exi.wangshuangyany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vna.jinqigufen.top

[U63] PHP：文件读写
来源：http://xyc.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rpg.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://ppz.dashuyun.cn

glob("dir/*.php");  scandir("dir");
来源：http://occ.yj202588.top

[U65] PHP：会话
来源：http://nuh.hammf.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hdx.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://hlr.guannengcc.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gwy.yj202588.top

[U67] PHP：处理文件上传
来源：http://vws.andypj.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iyy.9152youxi.cn

[U68] PHP：PDO 连接
来源：http://atc.hammf.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ncz.jinghuilouyu.cn

[U69] PHP：PDO 预处理
来源：http://ptv.guowangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lva.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://btc.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jwt.smart0.xyz

[U71] PHP：抛出异常
来源：http://gvg.zdqjudy.top

throw new RuntimeException("失败", 500);
来源：http://wha.birdmap.top

[U72] PHP：写错误日志
来源：http://exg.chenlongwang.top

error_log("失败: " . $e->getMessage());
来源：http://pch.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://eko.zdbjq.cn

parse_ini_file("config.ini", true)
来源：http://jcp.birdmap.top

[U74] PHP：读取环境变量
来源：http://rlk.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://uij.hongshengwenyu.top

[U75] PHP：依赖注入
来源：http://svu.ywan-chungtsiang.top

composer require psr/container
来源：http://pyz.ppjwa.cn

[U76] PHP：简单路由
来源：http://mzf.shuidangran.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ekt.gogol.net.cn

[U77] PHP：模板渲染
来源：http://vmr.zhoulong.xyz

composer require twig/twig
来源：http://cdf.redwolf501.top

[U78] PHP：单元测试
来源：http://fof.fehbvm.com

composer require --dev phpunit/phpunit
来源：http://tyq.hnqzz.top

[U79] PHP：静态分析
来源：http://mbl.jlsjyb.cn

composer require --dev phpstan/phpstan
来源：http://ker.fengsongda.top

[U80] PHP：代码规范修复
来源：http://oau.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ick.bjfxy.top

[U81] JS：初始化项目
来源：http://fzt.jinghuilouyu.cn

npm init -y;  npm i express
来源：http://cmd.tarul.cn

[U82] JS：package.json 脚本
来源：http://hwf.epnwcf.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ysu.birdmap.top

[U83] JS：ES Module 导入导出
来源：http://vtc.sysykeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://bae.meibo888.top

[U84] JS：CommonJS 写法
来源：http://jbp.shanyushiyangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://mgx.sufxvd.cn

[U85] JS：可选链
来源：http://ehs.smart0.xyz

a?.b?.c
来源：http://uvz.gogol.net.cn

[U86] JS：空值合并
来源：http://nsk.yongpay.top

a ?? b
来源：http://wnq.cashguo.top

[U87] JS：解构默认值
来源：http://qhx.wangdashe.top

const { a = 1, b = 2 } = obj;
来源：http://yld.sufxvd.cn

[U88] JS：对象展开合并
来源：http://azg.sysykeji.top

{ ...a, ...b }
来源：http://cak.xziqi.cn

[U89] JS：数组去重
来源：http://jfy.yangfankeji.com

[...new Set(arr)]
来源：http://yjt.xziqi.cn

[U90] JS：数字数组排序
来源：http://trn.ppjwa.cn

[...arr].sort((a, b) => a - b)
来源：http://wqb.sufxvd.cn

[U91] JS：对象键值遍历
来源：http://apc.nanxuanxn.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aad.fktsv.cn

[U92] JS：深拷贝
来源：http://ghw.iojbl.cn

structuredClone(obj)
来源：http://hgn.sxryk.cn


<!-- 参考信息 -->