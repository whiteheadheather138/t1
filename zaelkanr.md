代发 wailian999

[T07] Kotlin：集合过滤
来源：http://doc.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ovj.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://mkb.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://iim.tianlin.xyz

[T09] Kotlin：扩展函数
来源：http://euo.hcnkem.com

fun String.exclaim() = this + "!"
来源：http://rjr.sxryk.cn

[T10] Kotlin：默认参数
来源：http://maz.hywenlv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nzm.yj20258.top

[T11] Kotlin：协程
来源：http://hri.sxryk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ioo.xylfe.cn

[T12] Kotlin：解构声明
来源：http://itf.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://vwu.cucudq.cn

[T13] Kotlin：只读 Map
来源：http://nfi.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://jwz.tanke756.top

[T14] Kotlin：循环
来源：http://bpb.shuidangran.top

for (i in 1..10) println(i)
来源：http://qjv.xylfe.cn

[T15] Kotlin：接口
来源：http://red.aizwys.cn

interface Shape { fun area(): Double }
来源：http://jtv.yj20258.top

[T16] Swift：Hello World
来源：http://dqg.ydjk.org.cn

print("Hello")
来源：http://avn.yuxming.cn

[T17] Swift：变量与常量
来源：http://hua.fanxiaobao.xyz

var a = 1;  let b = 2
来源：http://txe.chenjidiqi.icu

[T18] Swift：字符串插值
来源：http://cdb.mhx1999.top

"值: \(b)"
来源：http://prg.hysaishi.cn

[T19] Swift：可选绑定
来源：http://xfl.ydzc1.top

if let n = opt { print(n) }
来源：http://jdz.zdqjudy.top

[T20] Swift：数组操作
来源：http://bym.jinghuilouyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vtk.yanxiufei.cn

[T21] Swift：遍历
来源：http://jwr.9152youxi.cn

for x in a { print(x) }
来源：http://bfd.gzhubu.top

[T22] Swift：字典
来源：http://agd.yonumen.top

var d = ["a": 1];  d["b"] = 2
来源：http://smn.hesvh.cn

[T23] Swift：函数
来源：http://tyx.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iuo.zhiwuduotai.top

[T24] Swift：闭包
来源：http://fxb.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gxh.zhengqikj.top

[T25] Swift：结构体
来源：http://mqz.birdmap.top

struct P { var x: Int }
来源：http://haf.nwbrower.top

[T26] Swift：类与重写
来源：http://spz.fzhhl.top

class A: Base { override func f() {} }
来源：http://tde.zdbjq.cn

[T27] Swift：错误处理
来源：http://vsh.hesvh.cn

do { try f() } catch { print(error) }
来源：http://ael.cqqwz.cn

[T28] Swift：枚举
来源：http://ghr.redwolf501.top

enum Color { case red, green }
来源：http://hkr.ehwqpu.com

[T29] Swift：guard 提前返回
来源：http://jre.tianlin.xyz

guard let x = opt else { return }
来源：http://sck.yj202588.top

[T30] Swift：协议
来源：http://yoj.ppjwa.cn

protocol Shape { func area() -> Double }
来源：http://owb.ywan-chungtsiang.top

[T31] Lua：Hello World
来源：http://vhj.yongpay.top

print("Hello")
来源：http://ypa.hcnkem.com

[T32] Lua：局部变量
来源：http://und.haohaochexian.top

local a = 1
来源：http://rio.quarkkingdee.top

[T33] Lua：表（数组）
来源：http://ove.aibaodan.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uxz.shanyushiyangkeji.top

[T34] Lua：遍历表
来源：http://bug.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://mwq.shanyushiyangkeji.top

[T35] Lua：字典表
来源：http://muj.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://oce.xylfe.cn

[T36] Lua：函数
来源：http://tpp.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://amd.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://kva.chenlongwang.top

"a" .. "b"
来源：http://qzl.birdmap.top

[T38] Lua：条件
来源：http://uuy.epnwcf.com

if x > 0 then print("正") end
来源：http://xqx.zhengqikj.top

[T39] Lua：模式匹配
来源：http://mwj.zhoulong.xyz

string.find(s, "%d+")
来源：http://wyl.fehbvm.com

[T40] Lua：元表
来源：http://ars.dashuyun.cn

setmetatable({}, { __index = base })
来源：http://pzu.hcnkem.com

[T41] Perl：Hello World
来源：http://cgu.jinghuilouyu.cn

print "Hello\n";
来源：http://qno.meibo888.top

[T42] Perl：变量类型
来源：http://amy.yonumen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zpb.xinyue.icu

[T43] Perl：字符串插值
来源：http://iat.jinyuanbaomall.cn

"值: $a"
来源：http://pqt.tanke756.top

[T44] Perl：条件
来源：http://ovk.shanyushiyangtech.top

if ($a > 0) { print "正"; }
来源：http://mfv.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://mmk.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://eyv.zhongyouzk.top

[T46] Perl：哈希操作
来源：http://lud.fzhhl.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kdu.aizwys.cn

[T47] Perl：正则捕获
来源：http://lsn.zhixingplan.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xib.sweek.top

[T48] Perl：正则替换
来源：http://djy.sufxvd.cn

$s =~ s/old/new/g;
来源：http://prb.dashuyun.cn

[T49] Perl：函数
来源：http://ueg.sjlbkw.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ril.wangdashe.top

[T50] Perl：逐行读文件
来源：http://ckq.dianchejie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yzw.9152youxi.cn

while (my $line = <$fh>) { print $line; }
来源：http://zhm.xinyue.icu

[T51] Scala：Hello World
来源：http://uvu.shuidangran.top

println("Hello")
来源：http://kec.ywan-chungtsiang.top

[T52] Scala：变量
来源：http://pmz.xuanzx.com

val a = 1;  var b = 2
来源：http://sdo.nwbrower.top

[T53] Scala：字符串插值
来源：http://pnv.redwolf501.top

s"值: $b"
来源：http://tsz.cashguo.top

[T54] Scala：集合映射
来源：http://jxr.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://ojo.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://pia.fanxiaobao.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://pjw.snrcjt.cn

[T56] Scala：样例类
来源：http://hkw.vehdjk.com

case class User(name: String, age: Int)
来源：http://mqt.jinqigufen.top

[T57] Scala：模式匹配
来源：http://hlx.pengpengdd.cyou

x match { case 1 => "一"; case _ => "其他" }
来源：http://lsx.wangdashe.top

[T58] Scala：函数定义
来源：http://vrt.chenjidiqi.icu

def add(a: Int, b: Int): Int = a + b
来源：http://gjk.jiagoushi.top

[T59] Scala：循环
来源：http://pdv.pengpengdd.cyou

for (i <- 1 to 10) println(i)
来源：http://lbf.xuanzx.com

[T60] Scala：折叠
来源：http://txr.hysaishi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vnu.ywan-chungtsiang.top

================================================================================
来源：http://nvq.wangdashe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lua.cashguo.top

================================================================================
来源：http://sxd.zdbjq.cn

[U01] Py：创建虚拟环境
来源：http://owg.redwolf501.top

python -m venv .venv && source .venv/bin/activate
来源：http://cag.ivvv.top

[U02] Py：导出 / 安装依赖
来源：http://ztx.jinghuilouyu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gfs.316326.xyz

[U03] Py：加载 .env 配置
来源：http://xef.aibaodan.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ptc.jinghuilouyu.cn

[U04] Py：变量调试打印
来源：http://ybd.xuetiantiany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kew.haohaochexian.top

[U05] Py：列表去重且保序
来源：http://uwe.zycfv.cn

list(dict.fromkeys(arr))
来源：http://skz.xziqi.cn

[U06] Py：合并两个字典
来源：http://bis.quarkkingdee.top

{**a, **b}
来源：http://dna.wangdashe.top

[U07] Py：反转字典键值
来源：http://wmc.epnwcf.com

{v: k for k, v in d.items()}
来源：http://umw.hnqzz.top

[U08] Py：展平二维列表
来源：http://une.meibo888.top

[y for x in nested for y in x]
来源：http://hyl.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://ahd.0kj1m.cn

max(d, key=d.get)
来源：http://xeu.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://icf.mhx1999.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zmu.tian-w.cn

[U11] Py：生成器表达式
来源：http://sqp.sufxvd.cn

(x * 2 for x in arr)
来源：http://sjd.ivvv.top

[U12] Py：取出现最多的 3 个元素
来源：http://uvn.jqgfzy.top

Counter(arr).most_common(3)
来源：http://vrv.redwolf501.top

[U13] Py：固定长度队列
来源：http://opz.shuidangran.top

deque(maxlen=10)
来源：http://ciw.yuxming.cn

[U14] Py：分组收集到列表
来源：http://eka.yj20258.top

defaultdict(list)
来源：http://vtq.ctjpmb.com

[U15] Py：高精度计时
来源：http://ogb.ywan-chungtsiang.top

t = time.perf_counter()
来源：http://qsp.dianchejie.cn

[U16] Py：命令行参数解析
来源：http://uce.guowangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xxv.sjlbkw.cn

[U17] Py：初始化日志
来源：http://sqq.zhijiandao.cn

logging.basicConfig(level=logging.INFO)
来源：http://dpl.zycfv.cn

[U18] Py：预编译正则
来源：http://gqt.epnwcf.com

pat = re.compile(r"\d+")
来源：http://hkg.shzxlz.cn

[U19] Py：正则替换带回调
来源：http://zkp.xingfuxueyuan.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bcy.yongpay.top

[U20] Py：缓存函数结果
来源：http://ydw.tianlin.xyz

@functools.lru_cache(maxsize=None)
来源：http://nja.guowangkeji.top

[U21] Py：自定义上下文管理器
来源：http://egm.redwolf501.top

@contextlib.contextmanager
来源：http://rbm.jinghuilouyu.cn

[U22] Py：矩阵转置
来源：http://grh.nwbrower.top

list(zip(*m))
来源：http://abi.cashguo.top

[U23] Py：分块读取大文件
来源：http://gvx.xuanzx.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bta.yangfankeji.com

[U24] Py：路径操作
来源：http://syx.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hds.yanxiufei.cn

[U25] Py：CSV 按字典读
来源：http://buk.sufxvd.cn

csv.DictReader(f)
来源：http://mhz.dashuyun.cn

[U26] Py：并发下载
来源：http://azv.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xmg.xuanzx.com

[U27] Py：异步 HTTP
来源：http://mwx.tanke756.top

aiohttp.ClientSession() 配合 async with
来源：http://vlf.pengpengdd.cyou

[U28] Py：类型别名
来源：http://dth.zhoulong.xyz

UserId = int
来源：http://fyj.aibaodan.cn

[U29] Py：属性校验
来源：http://nps.yueranfly.top

@property 与 @x.setter 配合
来源：http://qtq.zhoulong.xyz

[U30] Py：数据类
来源：http://lzp.ywan-chungtsiang.top

@dataclass(slots=True)
来源：http://pdk.jinqigufen.top

[U31] Py：单测
来源：http://mkt.wangdashe.top

python -m pytest -q
来源：http://dwl.bbcook.cn

[U32] Py：代码格式化
来源：http://wce.pengpengdd.cyou

ruff format . && ruff check --fix .
来源：http://aea.sufxvd.cn

[U33] Py：打包发布
来源：http://vob.xziqi.cn

python -m build  （依赖 pyproject.toml）
来源：http://pcn.xylfe.cn

[U34] Py：判断编码
来源：http://srt.9152youxi.cn

chardet.detect(raw)
来源：http://kxb.gaohongyu789.top

[U35] Py：发送邮件
来源：http://snu.yfazqb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eek.tianlin.xyz

[U36] Py：定时任务
来源：http://iug.kuanghao11.cn

schedule.every(10).minutes.do(job)
来源：http://rxd.svipenyu.cn

[U37] Py：读写 Excel
来源：http://xuq.zhoulong.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://cyo.gzhubu.top

[U38] Py：获取脚本所在目录
来源：http://cdm.guannengcc.top

Path(__file__).resolve().parent
来源：http://lgo.tian-w.cn

[U39] Py：判断是否在交互环境
来源：http://sgk.haohaochexian.top

sys.stdout.isatty()
来源：http://tmp.yangfankeji.com

[U40] Py：打印到标准错误
来源：http://azl.snrcjt.cn

print("err", file=sys.stderr)
来源：http://upj.tianlin.xyz

[U41] PHP：初始化 Composer 项目
来源：http://wws.cdnleiting.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lcx.sweek.top

[U42] PHP：PSR-4 自动加载
来源：http://llv.gogol.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kju.jiagoushi.top

[U43] PHP：声明命名空间
来源：http://hik.tanke756.top

namespace App\Http;
来源：http://lnr.bjfxy.top

[U44] PHP：开启严格类型
来源：http://naw.52xcode.cn

declare(strict_types=1);
来源：http://rue.ywan-chungtsiang.top

[U45] PHP：类型声明与返回类型
来源：http://nda.quarkkingdee.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vvl.hfpthk.cn

[U46] PHP：可空类型
来源：http://zmw.cucudq.cn

?string $name = null
来源：http://whj.yj20258888.top

[U47] PHP：联合类型
来源：http://vdm.tianlin.xyz

int|string $id
来源：http://sif.jinqigufen.top

[U48] PHP：纯枚举
来源：http://iwm.yangfankeji.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qbg.zhixingplan.top

[U49] PHP：只读属性
来源：http://nxv.shanyushiyangtech.top

public readonly string $name
来源：http://yvv.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://kmn.shangyingyoupin.top

public function __construct(private int $id) {}
来源：http://doo.fktsv.cn

[U51] PHP：数组解构
来源：http://gtm.nwbrower.top

[$a, $b] = $arr;
来源：http://lrq.jqgfzy.top

[U52] PHP：箭头函数
来源：http://tkv.shanyushiyangkeji.top

$double = fn($x) => $x * 2;
来源：http://wny.xingfuxueyuan.xyz

[U53] PHP：空合并运算符
来源：http://psx.hongshengwenyu.top

$v = $a ?? $b ?? "default";
来源：http://uxl.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://uha.pengpengdd.cyou

$obj?->method()
来源：http://vli.daxiang520.top

[U55] PHP：match 表达式
来源：http://lwf.sxryk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ump.hcnkem.com

[U56] PHP：命名参数
来源：http://xvd.xingfuxueyuan.xyz

f(a: 1, b: 2)
来源：http://eex.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://uay.fzhhl.top

"值: {$a}"
来源：http://rep.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://hgu.cucudq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ctd.yvedp.cn

[U59] PHP：自定义排序
来源：http://tyl.sufxvd.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://afu.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://zdb.yuxming.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://njn.pengpengdd.cyou

[U61] PHP：正则
来源：http://nef.yvedp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qyy.ppjwa.cn

[U62] PHP：日期对象
来源：http://poi.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://guk.zhongyouzk.top

[U63] PHP：文件读写
来源：http://iwd.svipenyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pmo.zhengqikj.top

[U64] PHP：目录遍历
来源：http://cfz.jinghuilouyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://mrj.fanxiaobao.xyz

[U65] PHP：会话
来源：http://isv.zdqjudy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mnk.52xcode.cn

[U66] PHP：设置 Cookie
来源：http://jev.hnqzz.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://erj.zycfv.cn

[U67] PHP：处理文件上传
来源：http://edf.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vre.ydzc1.top

[U68] PHP：PDO 连接
来源：http://jyx.ywan-chungtsiang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nax.quarkkingdee.top

[U69] PHP：PDO 预处理
来源：http://jqi.tarul.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rpm.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://lpn.jiagoushi.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://arj.jinqigufen.top

[U71] PHP：抛出异常
来源：http://apx.shzxlz.cn

throw new RuntimeException("失败", 500);
来源：http://lpr.wangshuangyany.cn

[U72] PHP：写错误日志
来源：http://fpc.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://tev.ehwqpu.com

[U73] PHP：读取 ini 配置
来源：http://aya.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://krt.haohaochexian.top

[U74] PHP：读取环境变量
来源：http://yiy.xziqi.cn

getenv("APP_ENV") ?: "production"
来源：http://cak.ybcxt.top

[U75] PHP：依赖注入
来源：http://rma.zhaomingkeji.xyz

composer require psr/container
来源：http://jsv.jqgfzy.top

[U76] PHP：简单路由
来源：http://zmq.jinqigfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lpt.gaohongyu789.top

[U77] PHP：模板渲染
来源：http://rnp.epnwcf.com

composer require twig/twig
来源：http://fga.tian-w.cn

[U78] PHP：单元测试
来源：http://fxv.xinyue.icu

composer require --dev phpunit/phpunit
来源：http://spy.aibaodan.cn

[U79] PHP：静态分析
来源：http://fse.jyoumei.cn

composer require --dev phpstan/phpstan
来源：http://loa.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://lri.jqgfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://cti.jianghu66.top

[U81] JS：初始化项目
来源：http://men.xziqi.cn

npm init -y;  npm i express
来源：http://vwt.jianghu66.top

[U82] JS：package.json 脚本
来源：http://ree.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ksy.jqgfzy.top

[U83] JS：ES Module 导入导出
来源：http://rur.bjfxy.top

export const a = 1;  import { a } from "./m.js";
来源：http://yrd.shzxlz.cn

[U84] JS：CommonJS 写法
来源：http://jxd.pengpengdd.cyou

module.exports = { a };  const { a } = require("./m");
来源：http://nou.gaohongyu789.top

[U85] JS：可选链
来源：http://epd.hysaishi.cn

a?.b?.c
来源：http://yiy.fanxiaobao.xyz

[U86] JS：空值合并
来源：http://czr.svipenyu.cn

a ?? b
来源：http://igv.sxryk.cn

[U87] JS：解构默认值
来源：http://oik.ehwqpu.com

const { a = 1, b = 2 } = obj;
来源：http://bjo.zhijiandao.cn

[U88] JS：对象展开合并
来源：http://wzy.zhiwuduotai.top

{ ...a, ...b }
来源：http://cnt.zhijiandao.cn

[U89] JS：数组去重
来源：http://fui.shanyushiyangtech.top

[...new Set(arr)]
来源：http://heg.daxiang520.top

[U90] JS：数字数组排序
来源：http://ixr.hesvh.cn

[...arr].sort((a, b) => a - b)
来源：http://bmv.hnqzz.top

[U91] JS：对象键值遍历
来源：http://rsq.uphjek.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sfi.cdnleiting.top

[U92] JS：深拷贝
来源：http://cqb.xziqi.cn

structuredClone(obj)
来源：http://bod.shuidangran.top

[U93] JS：模板字符串
来源：http://ijw.uphjek.com

`共 ${n} 条`
来源：http://ycj.sxryk.cn

[U94] JS：箭头函数
来源：http://non.quarkkingdee.top

const double = x => x * 2;
来源：http://htl.tianlin.xyz


<!-- 参考信息 -->