代发 wailian999

[T09] Kotlin：扩展函数
来源：http://ezp.fanxiaobao.xyz

fun String.exclaim() = this + "!"
来源：http://qmr.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://dnr.hysaishi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://omd.xuanzx.com

[T11] Kotlin：协程
来源：http://emy.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yeb.zdbjq.cn

[T12] Kotlin：解构声明
来源：http://pmp.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://uyt.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://utw.c1oappe.top

val m = mapOf("a" to 1)
来源：http://ecx.tarul.cn

[T14] Kotlin：循环
来源：http://zul.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://ijt.chenzaomai.com

[T15] Kotlin：接口
来源：http://glg.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://wfu.smart0.xyz

[T16] Swift：Hello World
来源：http://jpi.tian-w.cn

print("Hello")
来源：http://vwu.yvedp.cn

[T17] Swift：变量与常量
来源：http://qzt.tanke756.top

var a = 1;  let b = 2
来源：http://phs.316326.xyz

[T18] Swift：字符串插值
来源：http://fwm.uphjek.com

"值: \(b)"
来源：http://uni.zhaomingkeji.xyz

[T19] Swift：可选绑定
来源：http://lfw.yj20258888.top

if let n = opt { print(n) }
来源：http://gep.chenjidiqi.icu

[T20] Swift：数组操作
来源：http://ind.hammf.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cfe.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://bhc.0kj1m.cn

for x in a { print(x) }
来源：http://qqm.snrcjt.cn

[T22] Swift：字典
来源：http://mpo.svipenyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dng.yfazqb.com

[T23] Swift：函数
来源：http://gfo.fktsv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cnp.nanxuanxn.top

[T24] Swift：闭包
来源：http://cni.chenlongwang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://fzt.daxiang520.top

[T25] Swift：结构体
来源：http://ivh.shangyingyoupin.top

struct P { var x: Int }
来源：http://tpx.jqgfzy.top

[T26] Swift：类与重写
来源：http://pwv.jianghu66.top

class A: Base { override func f() {} }
来源：http://jhj.zhaomingkeji.xyz

[T27] Swift：错误处理
来源：http://kkl.nanxuanxn.top

do { try f() } catch { print(error) }
来源：http://jdm.uphjek.com

[T28] Swift：枚举
来源：http://sox.bbcook.cn

enum Color { case red, green }
来源：http://zci.zhijiandao.cn

[T29] Swift：guard 提前返回
来源：http://tkx.pycfn.com

guard let x = opt else { return }
来源：http://aii.yongpay.top

[T30] Swift：协议
来源：http://rqr.andypj.xyz

protocol Shape { func area() -> Double }
来源：http://vjt.hfpthk.cn

[T31] Lua：Hello World
来源：http://ckw.bbcook.cn

print("Hello")
来源：http://tyk.chenlongwang.top

[T32] Lua：局部变量
来源：http://fxo.zhiwuduotai.top

local a = 1
来源：http://kyg.svipenyu.cn

[T33] Lua：表（数组）
来源：http://pkd.zhoulong.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://kwg.smart0.xyz

[T34] Lua：遍历表
来源：http://xvf.hammf.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bed.shzxlz.cn

[T35] Lua：字典表
来源：http://xfu.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://say.fanxiaobao.xyz

[T36] Lua：函数
来源：http://fdl.c1oappe.top

function add(a, b) return a + b end
来源：http://pwa.dashuyun.cn

[T37] Lua：字符串拼接
来源：http://pcs.xinyue.icu

"a" .. "b"
来源：http://miw.redwolf501.top

[T38] Lua：条件
来源：http://vgt.zhoulong.xyz

if x > 0 then print("正") end
来源：http://vfv.ybcxt.top

[T39] Lua：模式匹配
来源：http://jsd.52xcode.cn

string.find(s, "%d+")
来源：http://kpd.jqgfzy.top

[T40] Lua：元表
来源：http://gje.guannengcc.top

setmetatable({}, { __index = base })
来源：http://ktu.xuanzx.com

[T41] Perl：Hello World
来源：http://csk.cucudq.cn

print "Hello\n";
来源：http://vqy.sjlbkw.cn

[T42] Perl：变量类型
来源：http://dxw.fehbvm.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ige.jqgfzy.top

[T43] Perl：字符串插值
来源：http://cim.zhixingplan.top

"值: $a"
来源：http://eph.smart0.xyz

[T44] Perl：条件
来源：http://tqf.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://pmh.tanke756.top

[T45] Perl：数组遍历
来源：http://xjf.ybcxt.top

for my $x (@arr) { print $x; }
来源：http://jgc.yueranfly.top

[T46] Perl：哈希操作
来源：http://ktf.zdqjudy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mjb.yj20258888.top

[T47] Perl：正则捕获
来源：http://qtu.ehwqpu.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://xea.hysaishi.cn

[T48] Perl：正则替换
来源：http://mss.tarul.cn

$s =~ s/old/new/g;
来源：http://chj.nanxuanxn.top

[T49] Perl：函数
来源：http://lzg.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://laq.xylfe.cn

[T50] Perl：逐行读文件
来源：http://vfd.tarul.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://iia.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://tfq.daxiang520.top

[T51] Scala：Hello World
来源：http://fvc.zhiwuduotai.top

println("Hello")
来源：http://wyh.birdmap.top

[T52] Scala：变量
来源：http://oaj.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://mee.ydzc1.top

[T53] Scala：字符串插值
来源：http://svh.cheryme.top

s"值: $b"
来源：http://qnj.svipenyu.cn

[T54] Scala：集合映射
来源：http://cfx.tianlin.xyz

List(1, 2, 3).map(_ * 2)
来源：http://xbc.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://smn.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://tke.meibo888.top

[T56] Scala：样例类
来源：http://zrr.hfpthk.cn

case class User(name: String, age: Int)
来源：http://oxs.vehdjk.com

[T57] Scala：模式匹配
来源：http://ixr.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sha.mhx1999.top

[T58] Scala：函数定义
来源：http://swk.hongshengwenyu.top

def add(a: Int, b: Int): Int = a + b
来源：http://nhz.fehbvm.com

[T59] Scala：循环
来源：http://eoj.shanyushiyangtech.top

for (i <- 1 to 10) println(i)
来源：http://afi.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://szy.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://egh.cashguo.top

================================================================================
来源：http://pkt.wangdashe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uwn.hongshengwenyu.top

================================================================================
来源：http://lsr.xinyue.icu

[U01] Py：创建虚拟环境
来源：http://ksd.xuetiantiany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://paw.hnqzz.top

[U02] Py：导出 / 安装依赖
来源：http://ipv.ybcxt.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://itm.ivvv.top

[U03] Py：加载 .env 配置
来源：http://deu.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wqf.yueranfly.top

[U04] Py：变量调试打印
来源：http://arn.ppjwa.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rxu.birdmap.top

[U05] Py：列表去重且保序
来源：http://fnk.nanxuanxn.top

list(dict.fromkeys(arr))
来源：http://qog.andypj.xyz

[U06] Py：合并两个字典
来源：http://frc.chenzaomai.com

{**a, **b}
来源：http://gbb.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://icy.hysaishi.cn

{v: k for k, v in d.items()}
来源：http://gpk.birdmap.top

[U08] Py：展平二维列表
来源：http://ubu.kuanghao11.cn

[y for x in nested for y in x]
来源：http://rwg.shanyushiyangtech.top

[U09] Py：字典取最大值的键
来源：http://fca.yj20258.top

max(d, key=d.get)
来源：http://wqw.zdbjq.cn

[U10] Py：按值排序字典
来源：http://ojj.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wgv.quarkkingdee.top

[U11] Py：生成器表达式
来源：http://knu.yangfankeji.com

(x * 2 for x in arr)
来源：http://hsk.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eou.vehdjk.com

Counter(arr).most_common(3)
来源：http://ldc.zhongyouzk.top

[U13] Py：固定长度队列
来源：http://vig.hnxiangtu.top

deque(maxlen=10)
来源：http://wwi.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://rdw.chenlongwang.top

defaultdict(list)
来源：http://eis.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://uku.shuidangran.top

t = time.perf_counter()
来源：http://qbz.xziqi.cn

[U16] Py：命令行参数解析
来源：http://hsf.zdqjudy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aqh.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://sqq.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://tls.xuetiantiany.cn

[U18] Py：预编译正则
来源：http://jxv.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://ove.chenzaomai.com

[U19] Py：正则替换带回调
来源：http://wth.sxryk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lkn.sysykeji.top

[U20] Py：缓存函数结果
来源：http://eak.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://irs.jqgufenzy.top

[U21] Py：自定义上下文管理器
来源：http://yhg.zhaomingkeji.xyz

@contextlib.contextmanager
来源：http://srd.chenzaomai.com

[U22] Py：矩阵转置
来源：http://yam.feifeiyinyue.top

list(zip(*m))
来源：http://tsg.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://ocq.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vbm.hongshengwenyu.top

[U24] Py：路径操作
来源：http://gpn.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kwd.yfazqb.com

[U25] Py：CSV 按字典读
来源：http://zub.zhiwuduotai.top

csv.DictReader(f)
来源：http://eet.hywenlv.cn

[U26] Py：并发下载
来源：http://pdf.meibo888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vsk.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://ijk.fanxiaobao.xyz

aiohttp.ClientSession() 配合 async with
来源：http://zoh.aibaodan.cn

[U28] Py：类型别名
来源：http://ebu.bbcook.cn

UserId = int
来源：http://ftd.fehbvm.com

[U29] Py：属性校验
来源：http://jbw.zycfv.cn

@property 与 @x.setter 配合
来源：http://jtt.snrcjt.cn

[U30] Py：数据类
来源：http://qgm.fzhhl.top

@dataclass(slots=True)
来源：http://scz.ydjk.org.cn

[U31] Py：单测
来源：http://rik.haohaochexian.top

python -m pytest -q
来源：http://mkg.ywan-chungtsiang.top

[U32] Py：代码格式化
来源：http://imm.ivvv.top

ruff format . && ruff check --fix .
来源：http://ozh.nanxuanxn.top

[U33] Py：打包发布
来源：http://vye.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://rps.316326.xyz

[U34] Py：判断编码
来源：http://rby.jqgfzy.top

chardet.detect(raw)
来源：http://nzt.birdmap.top

[U35] Py：发送邮件
来源：http://jlx.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dmw.pengpengdd.cyou

[U36] Py：定时任务
来源：http://cfx.aizwys.cn

schedule.every(10).minutes.do(job)
来源：http://won.hammf.cn

[U37] Py：读写 Excel
来源：http://ydm.zhengqikj.top

pandas.read_excel / DataFrame.to_excel
来源：http://vdx.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://ebd.yuanzhike.top

Path(__file__).resolve().parent
来源：http://jpq.c1oappe.top

[U39] Py：判断是否在交互环境
来源：http://cga.52xcode.cn

sys.stdout.isatty()
来源：http://aqs.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://jor.shuidangran.top

print("err", file=sys.stderr)
来源：http://dki.chenzaomai.com

[U41] PHP：初始化 Composer 项目
来源：http://bmr.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bml.ydzc1.top

[U42] PHP：PSR-4 自动加载
来源：http://duu.bjfxy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://exr.shanyushiyangtech.top

[U43] PHP：声明命名空间
来源：http://voq.kuanghao11.cn

namespace App\Http;
来源：http://jwk.dashuyun.cn

[U44] PHP：开启严格类型
来源：http://gqc.yonumen.top

declare(strict_types=1);
来源：http://kwb.epnwcf.com

[U45] PHP：类型声明与返回类型
来源：http://wdr.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ymj.zdqjudy.top

[U46] PHP：可空类型
来源：http://vsv.ctjpmb.com

?string $name = null
来源：http://odv.gaohongyu789.top

[U47] PHP：联合类型
来源：http://jfz.aibaodan.cn

int|string $id
来源：http://vcx.fehbvm.com

[U48] PHP：纯枚举
来源：http://lyr.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kxv.jianghu66.top

[U49] PHP：只读属性
来源：http://kdx.andypj.xyz

public readonly string $name
来源：http://qkh.jinqigufen.top

[U50] PHP：构造器属性提升
来源：http://tzx.yangfankeji.com

public function __construct(private int $id) {}
来源：http://koe.ydzc1.top

[U51] PHP：数组解构
来源：http://iye.c1oappe.top

[$a, $b] = $arr;
来源：http://lzt.zycfv.cn

[U52] PHP：箭头函数
来源：http://mae.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://rsf.gzhubu.top

[U53] PHP：空合并运算符
来源：http://jqi.hnxiangtu.top

$v = $a ?? $b ?? "default";
来源：http://tgu.bbcook.cn

[U54] PHP：空安全调用
来源：http://xjt.gzhubu.top

$obj?->method()
来源：http://hxs.shanyushiyangtech.top

[U55] PHP：match 表达式
来源：http://qju.uphjek.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tvx.bbcook.cn

[U56] PHP：命名参数
来源：http://geo.cqqwz.cn

f(a: 1, b: 2)
来源：http://znr.meibo888.top

[U57] PHP：字符串插值
来源：http://pjc.yj20258.top

"值: {$a}"
来源：http://qtm.vqdsnc.cn

[U58] PHP：数组三件套
来源：http://apc.jianghu66.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wqm.ybcxt.top

[U59] PHP：自定义排序
来源：http://cvk.xziqi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://czz.haohaochexian.top

[U60] PHP：JSON 编解码
来源：http://jer.mhx1999.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iow.pengpengdd.cyou

[U61] PHP：正则
来源：http://cgu.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ire.xuetiantiany.cn

[U62] PHP：日期对象
来源：http://dae.jinqigfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kfn.quarkkingdee.top

[U63] PHP：文件读写
来源：http://mwg.yuxming.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cjl.zhengqikj.top

[U64] PHP：目录遍历
来源：http://gyv.hysaishi.cn

glob("dir/*.php");  scandir("dir");
来源：http://skq.smart0.xyz

[U65] PHP：会话
来源：http://jgd.cashguo.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lnl.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://qli.daxiang520.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rwf.feifeiyinyue.top

[U67] PHP：处理文件上传
来源：http://jrm.jiagoushi.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ekw.sufxvd.cn

[U68] PHP：PDO 连接
来源：http://lma.xziqi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://chu.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://dex.yuxming.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gni.jiagoushi.top

[U70] PHP：PDO 事务
来源：http://mat.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hqi.yuxming.cn

[U71] PHP：抛出异常
来源：http://zms.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://nkv.uphjek.com

[U72] PHP：写错误日志
来源：http://nqr.sweek.top

error_log("失败: " . $e->getMessage());
来源：http://hcx.xinyue.icu

[U73] PHP：读取 ini 配置
来源：http://zum.0kj1m.cn

parse_ini_file("config.ini", true)
来源：http://mjz.iojbl.cn

[U74] PHP：读取环境变量
来源：http://egt.ybcxt.top

getenv("APP_ENV") ?: "production"
来源：http://ktz.shangyingyoupin.top

[U75] PHP：依赖注入
来源：http://ltr.chenlongwang.top

composer require psr/container
来源：http://gry.nwbrower.top

[U76] PHP：简单路由
来源：http://ace.316326.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qav.mhx1999.top

[U77] PHP：模板渲染
来源：http://ukp.zdbjq.cn

composer require twig/twig
来源：http://qey.quarkkingdee.top

[U78] PHP：单元测试
来源：http://jll.fzhhl.top

composer require --dev phpunit/phpunit
来源：http://srs.kuanghao11.cn

[U79] PHP：静态分析
来源：http://ekj.aizwys.cn

composer require --dev phpstan/phpstan
来源：http://rqm.hfpthk.cn

[U80] PHP：代码规范修复
来源：http://kut.fehbvm.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ies.jiagoushi.top

[U81] JS：初始化项目
来源：http://btq.mhx1999.top

npm init -y;  npm i express
来源：http://oxe.epnwcf.com

[U82] JS：package.json 脚本
来源：http://jmg.svipenyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jvj.yj20258888.top

[U83] JS：ES Module 导入导出
来源：http://tqn.bjfxy.top

export const a = 1;  import { a } from "./m.js";
来源：http://kcd.pengpengdd.cyou

[U84] JS：CommonJS 写法
来源：http://cfv.gaohongyu789.top

module.exports = { a };  const { a } = require("./m");
来源：http://teg.chenjidiqi.icu

[U85] JS：可选链
来源：http://klh.hesvh.cn

a?.b?.c
来源：http://tpf.jinghuilouyu.cn

[U86] JS：空值合并
来源：http://squ.kuanghao11.cn

a ?? b
来源：http://scy.zhoulong.xyz

[U87] JS：解构默认值
来源：http://mst.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://njf.mhx1999.top

[U88] JS：对象展开合并
来源：http://pop.andypj.xyz

{ ...a, ...b }
来源：http://ksy.hywenlv.cn

[U89] JS：数组去重
来源：http://zbq.haohaochexian.top

[...new Set(arr)]
来源：http://mwu.guowangkeji.top

[U90] JS：数字数组排序
来源：http://ffd.tanke756.top

[...arr].sort((a, b) => a - b)
来源：http://kvj.yj20258888.top

[U91] JS：对象键值遍历
来源：http://foz.yvedp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fbs.hfpthk.cn

[U92] JS：深拷贝
来源：http://gkr.ehwqpu.com

structuredClone(obj)
来源：http://elk.yj202588.top

[U93] JS：模板字符串
来源：http://sgz.fzhhl.top

`共 ${n} 条`
来源：http://xwk.jinqigfzy.top

[U94] JS：箭头函数
来源：http://czr.fktsv.cn

const double = x => x * 2;
来源：http://gtt.bjfxy.top

[U95] JS：Promise 包装
来源：http://aes.shuidangran.top

new Promise((resolve, reject) => {})
来源：http://edt.shanyushiyangkeji.top

[U96] JS：async/await 与异常
来源：http://xoi.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://duf.zhaomingkeji.xyz


<!-- 参考信息 -->