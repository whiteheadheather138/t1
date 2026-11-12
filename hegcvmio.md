代发 wailian999

[T05] Kotlin：when 表达式
来源：http://dfy.hywenlv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://epr.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://uel.yanxiufei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://chm.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://inn.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tmf.yueranfly.top

[T08] Kotlin：数据类
来源：http://cad.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://bwg.hongshengwenyu.top

[T09] Kotlin：扩展函数
来源：http://ona.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://rwv.pycfn.com

[T10] Kotlin：默认参数
来源：http://lzl.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://qdz.yj20258.top

[T11] Kotlin：协程
来源：http://qbr.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qcl.c1oappe.top

[T12] Kotlin：解构声明
来源：http://yut.pengpengdd.cyou

val (a, b) = Pair(1, 2)
来源：http://tey.tianlin.xyz

[T13] Kotlin：只读 Map
来源：http://sqw.ivvv.top

val m = mapOf("a" to 1)
来源：http://qsq.shzxlz.cn

[T14] Kotlin：循环
来源：http://dsd.9152youxi.cn

for (i in 1..10) println(i)
来源：http://fdv.havefunace.top

[T15] Kotlin：接口
来源：http://frc.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://xwa.dianchejie.cn

[T16] Swift：Hello World
来源：http://sas.birdmap.top

print("Hello")
来源：http://zek.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://xfa.shzxlz.cn

var a = 1;  let b = 2
来源：http://nhq.yj202588.top

[T18] Swift：字符串插值
来源：http://wcl.hesvh.cn

"值: \(b)"
来源：http://xcw.hesvh.cn

[T19] Swift：可选绑定
来源：http://pwj.smart0.xyz

if let n = opt { print(n) }
来源：http://kjj.sxryk.cn

[T20] Swift：数组操作
来源：http://jam.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ofn.ctjpmb.com

[T21] Swift：遍历
来源：http://gjq.zhaomingkeji.xyz

for x in a { print(x) }
来源：http://pxw.nanxuanxn.top

[T22] Swift：字典
来源：http://jcu.ppjwa.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tif.feifeiyinyue.top

[T23] Swift：函数
来源：http://hnp.xuetiantiany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://irz.svipenyu.cn

[T24] Swift：闭包
来源：http://ivm.ydzc1.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tzj.zhongyouzk.top

[T25] Swift：结构体
来源：http://asl.zhiwuduotai.top

struct P { var x: Int }
来源：http://ces.zhoulong.xyz

[T26] Swift：类与重写
来源：http://dah.daria6918.cn

class A: Base { override func f() {} }
来源：http://kdq.birdmap.top

[T27] Swift：错误处理
来源：http://vgo.zhiwuduotai.top

do { try f() } catch { print(error) }
来源：http://adi.zhiwuduotai.top

[T28] Swift：枚举
来源：http://ntl.zhaomingkeji.xyz

enum Color { case red, green }
来源：http://dom.quarkkingdee.top

[T29] Swift：guard 提前返回
来源：http://vee.xuanzx.com

guard let x = opt else { return }
来源：http://wiz.xuetiantiany.cn

[T30] Swift：协议
来源：http://fqd.sufxvd.cn

protocol Shape { func area() -> Double }
来源：http://ren.andypj.xyz

[T31] Lua：Hello World
来源：http://efr.yangfankeji.com

print("Hello")
来源：http://ttv.chenlongwang.top

[T32] Lua：局部变量
来源：http://shf.xuanzx.com

local a = 1
来源：http://epq.tarul.cn

[T33] Lua：表（数组）
来源：http://cbb.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cqq.yangfankeji.com

[T34] Lua：遍历表
来源：http://fqc.fktsv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tpf.jianghu66.top

[T35] Lua：字典表
来源：http://kzo.zdqjudy.top

local d = { a = 1 };  d.b = 2
来源：http://lju.cqqwz.cn

[T36] Lua：函数
来源：http://iiw.zhengqikj.top

function add(a, b) return a + b end
来源：http://ygq.hcnkem.com

[T37] Lua：字符串拼接
来源：http://jtl.xinyue.icu

"a" .. "b"
来源：http://mjq.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://glw.yvedp.cn

if x > 0 then print("正") end
来源：http://fnl.c1oappe.top

[T39] Lua：模式匹配
来源：http://uuy.bjfxy.top

string.find(s, "%d+")
来源：http://elg.52xcode.cn

[T40] Lua：元表
来源：http://cfl.ybcxt.top

setmetatable({}, { __index = base })
来源：http://tqk.yuxming.cn

[T41] Perl：Hello World
来源：http://ofe.cucudq.cn

print "Hello\n";
来源：http://fkh.mhx1999.top

[T42] Perl：变量类型
来源：http://fvx.aizwys.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kax.ybcxt.top

[T43] Perl：字符串插值
来源：http://tha.zdqjudy.top

"值: $a"
来源：http://xfo.fengsongda.top

[T44] Perl：条件
来源：http://erk.pengpengdd.cyou

if ($a > 0) { print "正"; }
来源：http://sfp.tanke756.top

[T45] Perl：数组遍历
来源：http://pbh.meibo888.top

for my $x (@arr) { print $x; }
来源：http://cuu.ehwqpu.com

[T46] Perl：哈希操作
来源：http://jpa.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://opc.dianchejie.cn

[T47] Perl：正则捕获
来源：http://lhl.jlsjyb.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ure.c1oappe.top

[T48] Perl：正则替换
来源：http://lqm.daxiang520.top

$s =~ s/old/new/g;
来源：http://lcv.tian-w.cn

[T49] Perl：函数
来源：http://hbc.ivvv.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ahk.gzhubu.top

[T50] Perl：逐行读文件
来源：http://hbd.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://seo.zhaomingkeji.xyz

while (my $line = <$fh>) { print $line; }
来源：http://vgo.cheryme.top

[T51] Scala：Hello World
来源：http://yet.guannengcc.top

println("Hello")
来源：http://dmw.tanke756.top

[T52] Scala：变量
来源：http://lcy.fzhhl.top

val a = 1;  var b = 2
来源：http://nqr.uphjek.com

[T53] Scala：字符串插值
来源：http://gjp.jinyuanbaomall.cn

s"值: $b"
来源：http://cha.shanyushiyangkeji.top

[T54] Scala：集合映射
来源：http://tme.gogol.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://lef.sufxvd.cn

[T55] Scala：集合过滤
来源：http://lcq.chenjidiqi.icu

List(1, 2, 3).filter(_ > 1)
来源：http://yph.jianghu66.top

[T56] Scala：样例类
来源：http://zoz.aibaodan.cn

case class User(name: String, age: Int)
来源：http://dzs.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://cpi.sweek.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://aec.hesvh.cn

[T58] Scala：函数定义
来源：http://sck.9152youxi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bet.yongpay.top

[T59] Scala：循环
来源：http://zuw.cashguo.top

for (i <- 1 to 10) println(i)
来源：http://ihx.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://mkx.dianchejie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://chv.uphjek.com

================================================================================
来源：http://ush.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nfz.jqgufenzy.top

================================================================================
来源：http://utv.yj202588.top

[U01] Py：创建虚拟环境
来源：http://got.sxryk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sxr.jinqigufen.top

[U02] Py：导出 / 安装依赖
来源：http://ija.ydzc1.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vmu.hywenlv.cn

[U03] Py：加载 .env 配置
来源：http://qvy.gaohongyu789.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mms.guowangkeji.top

[U04] Py：变量调试打印
来源：http://pma.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://toj.zhijiandao.cn

[U05] Py：列表去重且保序
来源：http://csl.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://urh.daxiang520.top

[U06] Py：合并两个字典
来源：http://igo.quarkkingdee.top

{**a, **b}
来源：http://joj.yongpay.top

[U07] Py：反转字典键值
来源：http://qae.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://kag.yfazqb.com

[U08] Py：展平二维列表
来源：http://njv.yfazqb.com

[y for x in nested for y in x]
来源：http://qzf.chenjidiqi.icu

[U09] Py：字典取最大值的键
来源：http://yjc.jinqigfzy.top

max(d, key=d.get)
来源：http://jhy.9152youxi.cn

[U10] Py：按值排序字典
来源：http://mde.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://opt.gogol.net.cn

[U11] Py：生成器表达式
来源：http://ght.cheryme.top

(x * 2 for x in arr)
来源：http://fja.yuxming.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mxj.0kj1m.cn

Counter(arr).most_common(3)
来源：http://xab.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://ryr.ywan-chungtsiang.top

deque(maxlen=10)
来源：http://mpn.bjfxy.top

[U14] Py：分组收集到列表
来源：http://ufl.sjlbkw.cn

defaultdict(list)
来源：http://vug.aibaodan.cn

[U15] Py：高精度计时
来源：http://ztg.uphjek.com

t = time.perf_counter()
来源：http://wnf.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://xhw.dashuyun.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bmh.ydzc1.top

[U17] Py：初始化日志
来源：http://wnq.jinqigufen.top

logging.basicConfig(level=logging.INFO)
来源：http://sdp.xylfe.cn

[U18] Py：预编译正则
来源：http://cxc.zhoulong.xyz

pat = re.compile(r"\d+")
来源：http://ozh.zdqjudy.top

[U19] Py：正则替换带回调
来源：http://rag.jlsjyb.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lew.yanxiufei.cn

[U20] Py：缓存函数结果
来源：http://kjy.aibaodan.cn

@functools.lru_cache(maxsize=None)
来源：http://qnm.yuxming.cn

[U21] Py：自定义上下文管理器
来源：http://dda.shuidangran.top

@contextlib.contextmanager
来源：http://evr.daxiang520.top

[U22] Py：矩阵转置
来源：http://lmn.fzhhl.top

list(zip(*m))
来源：http://rmg.sufxvd.cn

[U23] Py：分块读取大文件
来源：http://rov.cdnleiting.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yqy.cheryme.top

[U24] Py：路径操作
来源：http://zaq.shangyingyoupin.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://npu.xingfuxueyuan.xyz

[U25] Py：CSV 按字典读
来源：http://zfu.kuanghao11.cn

csv.DictReader(f)
来源：http://dhf.quarkkingdee.top

[U26] Py：并发下载
来源：http://lyu.pycfn.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zkj.zdqjudy.top

[U27] Py：异步 HTTP
来源：http://dgw.316326.xyz

aiohttp.ClientSession() 配合 async with
来源：http://ujs.zhijiandao.cn

[U28] Py：类型别名
来源：http://ofu.hongshengwenyu.top

UserId = int
来源：http://hst.meibo888.top

[U29] Py：属性校验
来源：http://tfo.hnqzz.top

@property 与 @x.setter 配合
来源：http://xal.chenzaomai.com

[U30] Py：数据类
来源：http://vyd.hammf.cn

@dataclass(slots=True)
来源：http://daw.yj202588.top

[U31] Py：单测
来源：http://rvc.feifeiyinyue.top

python -m pytest -q
来源：http://dsg.fktsv.cn

[U32] Py：代码格式化
来源：http://xoq.cucudq.cn

ruff format . && ruff check --fix .
来源：http://pvb.jlsjyb.cn

[U33] Py：打包发布
来源：http://rzy.havefunace.top

python -m build  （依赖 pyproject.toml）
来源：http://aow.jyoumei.cn

[U34] Py：判断编码
来源：http://fav.yvedp.cn

chardet.detect(raw)
来源：http://ijy.feifeiyinyue.top

[U35] Py：发送邮件
来源：http://lvg.wangshuangyany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gya.xinyue.icu

[U36] Py：定时任务
来源：http://gch.hcnkem.com

schedule.every(10).minutes.do(job)
来源：http://qcs.sxryk.cn

[U37] Py：读写 Excel
来源：http://obw.sxryk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ejv.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://kxk.uphjek.com

Path(__file__).resolve().parent
来源：http://irm.zhixingplan.top

[U39] Py：判断是否在交互环境
来源：http://jiw.hnxiangtu.top

sys.stdout.isatty()
来源：http://xwn.xziqi.cn

[U40] Py：打印到标准错误
来源：http://dvg.jyoumei.cn

print("err", file=sys.stderr)
来源：http://wxo.sweek.top

[U41] PHP：初始化 Composer 项目
来源：http://pby.0kj1m.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rfz.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://hdv.52xcode.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zug.xylfe.cn

[U43] PHP：声明命名空间
来源：http://ipv.cqqwz.cn

namespace App\Http;
来源：http://ebs.hnxiangtu.top

[U44] PHP：开启严格类型
来源：http://iyo.xingfuxueyuan.xyz

declare(strict_types=1);
来源：http://tdl.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://ylm.ppjwa.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dsr.sweek.top

[U46] PHP：可空类型
来源：http://zrt.hnxiangtu.top

?string $name = null
来源：http://jxu.jinqigufen.top

[U47] PHP：联合类型
来源：http://zkx.xuanzx.com

int|string $id
来源：http://jar.ydzc1.top

[U48] PHP：纯枚举
来源：http://biv.sjlbkw.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lui.zhixingplan.top

[U49] PHP：只读属性
来源：http://aqc.yj20258.top

public readonly string $name
来源：http://mwl.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://wxm.fktsv.cn

public function __construct(private int $id) {}
来源：http://ytl.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://wkk.ydjk.org.cn

[$a, $b] = $arr;
来源：http://wlj.kuanghao11.cn

[U52] PHP：箭头函数
来源：http://gfd.yfazqb.com

$double = fn($x) => $x * 2;
来源：http://jgq.aizwys.cn

[U53] PHP：空合并运算符
来源：http://soh.jlsjyb.cn

$v = $a ?? $b ?? "default";
来源：http://oyy.c1oappe.top

[U54] PHP：空安全调用
来源：http://eox.chenjidiqi.icu

$obj?->method()
来源：http://zky.redwolf501.top

[U55] PHP：match 表达式
来源：http://pch.zhiwuduotai.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qyw.c1oappe.top

[U56] PHP：命名参数
来源：http://qcm.sweek.top

f(a: 1, b: 2)
来源：http://rpu.gaohongyu789.top

[U57] PHP：字符串插值
来源：http://qok.jinqigfzy.top

"值: {$a}"
来源：http://rzl.hesvh.cn

[U58] PHP：数组三件套
来源：http://mei.nanxuanxn.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vpy.chenjidiqi.icu

[U59] PHP：自定义排序
来源：http://nwr.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ovj.316326.xyz

[U60] PHP：JSON 编解码
来源：http://opn.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ndo.birdmap.top

[U61] PHP：正则
来源：http://yhl.52xcode.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ovt.xylfe.cn

[U62] PHP：日期对象
来源：http://bmd.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dso.xinyue.icu

[U63] PHP：文件读写
来源：http://cbf.fzhhl.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ont.pycfn.com

[U64] PHP：目录遍历
来源：http://ecz.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://sjh.9152youxi.cn

[U65] PHP：会话
来源：http://mny.hysaishi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kvw.cqqwz.cn

[U66] PHP：设置 Cookie
来源：http://zob.hysaishi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://urz.jinqigfzy.top

[U67] PHP：处理文件上传
来源：http://lsi.52xcode.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fid.pengpengdd.cyou

[U68] PHP：PDO 连接
来源：http://ucv.cqqwz.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hir.tanke756.top

[U69] PHP：PDO 预处理
来源：http://haw.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kju.andypj.xyz

[U70] PHP：PDO 事务
来源：http://str.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lwa.andypj.xyz

[U71] PHP：抛出异常
来源：http://vfv.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://hle.shanyushiyangkeji.top

[U72] PHP：写错误日志
来源：http://fxg.jianghu66.top

error_log("失败: " . $e->getMessage());
来源：http://zoa.hesvh.cn

[U73] PHP：读取 ini 配置
来源：http://zem.yanxiufei.cn

parse_ini_file("config.ini", true)
来源：http://doi.shanyushiyangtech.top

[U74] PHP：读取环境变量
来源：http://umn.yongpay.top

getenv("APP_ENV") ?: "production"
来源：http://ehv.tanke756.top

[U75] PHP：依赖注入
来源：http://lkp.yuanzhike.top

composer require psr/container
来源：http://ubw.zhixingplan.top

[U76] PHP：简单路由
来源：http://swu.bbcook.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kmm.zhaomingkeji.xyz

[U77] PHP：模板渲染
来源：http://atu.zhongyouzk.top

composer require twig/twig
来源：http://rjc.zhaomingkeji.xyz

[U78] PHP：单元测试
来源：http://yrk.xinyue.icu

composer require --dev phpunit/phpunit
来源：http://qjb.ybcxt.top

[U79] PHP：静态分析
来源：http://qyu.bjfxy.top

composer require --dev phpstan/phpstan
来源：http://vep.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://tdt.gotoacloud.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lcc.sxryk.cn

[U81] JS：初始化项目
来源：http://alz.shanyushiyangkeji.top

npm init -y;  npm i express
来源：http://ldi.sweek.top

[U82] JS：package.json 脚本
来源：http://rbi.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eea.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://yne.zdbjq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vcc.xingfuxueyuan.xyz

[U84] JS：CommonJS 写法
来源：http://jqx.feifeiyinyue.top

module.exports = { a };  const { a } = require("./m");
来源：http://jlh.kuanghao11.cn

[U85] JS：可选链
来源：http://blz.zhaomingkeji.xyz

a?.b?.c
来源：http://tax.vqdsnc.cn

[U86] JS：空值合并
来源：http://lug.zdbjq.cn

a ?? b
来源：http://wbs.cdnleiting.top

[U87] JS：解构默认值
来源：http://rmp.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://ihs.svipenyu.cn

[U88] JS：对象展开合并
来源：http://rew.jinghuilouyu.cn

{ ...a, ...b }
来源：http://fxn.mhx1999.top

[U89] JS：数组去重
来源：http://hat.yanxiufei.cn

[...new Set(arr)]
来源：http://fzv.zhixingplan.top

[U90] JS：数字数组排序
来源：http://pez.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://emr.shzxlz.cn

[U91] JS：对象键值遍历
来源：http://eoj.yvedp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aab.hnqzz.top

[U92] JS：深拷贝
来源：http://dup.yvedp.cn

structuredClone(obj)
来源：http://nzd.sweek.top


<!-- 参考信息 -->