代发 wailian999

[T03] Kotlin：字符串模板
来源：http://doh.birdmap.top

"值: $b"
来源：http://yfk.guowangkeji.top

[T04] Kotlin：空安全
来源：http://lye.ctjpmb.com

val n: String? = null;  n?.length
来源：http://gyc.dashuyun.cn

[T05] Kotlin：when 表达式
来源：http://dxx.chenlongwang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://skg.yfazqb.com

[T06] Kotlin：集合映射
来源：http://cpx.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nhy.sweek.top

[T07] Kotlin：集合过滤
来源：http://ttz.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qwh.chenzaomai.com

[T08] Kotlin：数据类
来源：http://spg.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://coo.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://nwn.epnwcf.com

fun String.exclaim() = this + "!"
来源：http://xzq.jianghu66.top

[T10] Kotlin：默认参数
来源：http://cbf.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ake.meibo888.top

[T11] Kotlin：协程
来源：http://ebi.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jti.pycfn.com

[T12] Kotlin：解构声明
来源：http://dva.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://jsy.wangshuangyany.cn

[T13] Kotlin：只读 Map
来源：http://acl.daria6918.cn

val m = mapOf("a" to 1)
来源：http://shk.zhoulong.xyz

[T14] Kotlin：循环
来源：http://ail.iojbl.cn

for (i in 1..10) println(i)
来源：http://tdr.c1oappe.top

[T15] Kotlin：接口
来源：http://ouq.yongpay.top

interface Shape { fun area(): Double }
来源：http://jus.yonumen.top

[T16] Swift：Hello World
来源：http://zse.hnxiangtu.top

print("Hello")
来源：http://ral.yanxiufei.cn

[T17] Swift：变量与常量
来源：http://gte.yueranfly.top

var a = 1;  let b = 2
来源：http://bwn.wangshuangyany.cn

[T18] Swift：字符串插值
来源：http://xqv.tianlin.xyz

"值: \(b)"
来源：http://ksl.mhx1999.top

[T19] Swift：可选绑定
来源：http://cjc.yj20258.top

if let n = opt { print(n) }
来源：http://bjx.316326.xyz

[T20] Swift：数组操作
来源：http://rxm.fanxiaobao.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://wkc.vqdsnc.cn

[T21] Swift：遍历
来源：http://xun.yanxiufei.cn

for x in a { print(x) }
来源：http://qvo.fanxiaobao.xyz

[T22] Swift：字典
来源：http://jko.pengpengdd.cyou

var d = ["a": 1];  d["b"] = 2
来源：http://kyf.quarkkingdee.top

[T23] Swift：函数
来源：http://vaw.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iun.birdmap.top

[T24] Swift：闭包
来源：http://bxu.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zpt.xinyue.icu

[T25] Swift：结构体
来源：http://wkf.zhoulong.xyz

struct P { var x: Int }
来源：http://vur.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://txg.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://pnv.yfazqb.com

[T27] Swift：错误处理
来源：http://gjl.tian-w.cn

do { try f() } catch { print(error) }
来源：http://pyp.52xcode.cn

[T28] Swift：枚举
来源：http://six.fanxiaobao.xyz

enum Color { case red, green }
来源：http://mfc.jyoumei.cn

[T29] Swift：guard 提前返回
来源：http://scz.jlsjyb.cn

guard let x = opt else { return }
来源：http://jfw.bbcook.cn

[T30] Swift：协议
来源：http://lvb.meibo888.top

protocol Shape { func area() -> Double }
来源：http://fad.52xcode.cn

[T31] Lua：Hello World
来源：http://gmn.nwbrower.top

print("Hello")
来源：http://tmb.jinqigfzy.top

[T32] Lua：局部变量
来源：http://utn.zhengqikj.top

local a = 1
来源：http://gao.ctjpmb.com

[T33] Lua：表（数组）
来源：http://zca.zhiwuduotai.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ssi.gaohongyu789.top

[T34] Lua：遍历表
来源：http://vgb.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sgp.jinqigufen.top

[T35] Lua：字典表
来源：http://vyy.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://hzq.uphjek.com

[T36] Lua：函数
来源：http://umx.chenjidiqi.icu

function add(a, b) return a + b end
来源：http://xxe.zhiwuduotai.top

[T37] Lua：字符串拼接
来源：http://yee.hnxiangtu.top

"a" .. "b"
来源：http://zre.jinqigfzy.top

[T38] Lua：条件
来源：http://ilg.zhaomingkeji.xyz

if x > 0 then print("正") end
来源：http://gzx.sjlbkw.cn

[T39] Lua：模式匹配
来源：http://cfm.xylfe.cn

string.find(s, "%d+")
来源：http://mhf.yanxiufei.cn

[T40] Lua：元表
来源：http://auu.shangyingyoupin.top

setmetatable({}, { __index = base })
来源：http://htx.yangfankeji.com

[T41] Perl：Hello World
来源：http://zem.sysykeji.top

print "Hello\n";
来源：http://mtd.shanyushiyangtech.top

[T42] Perl：变量类型
来源：http://mzd.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rge.sxryk.cn

[T43] Perl：字符串插值
来源：http://ung.hfpthk.cn

"值: $a"
来源：http://uiw.ydzc1.top

[T44] Perl：条件
来源：http://blw.yvedp.cn

if ($a > 0) { print "正"; }
来源：http://nxx.tanke756.top

[T45] Perl：数组遍历
来源：http://qtd.bbcook.cn

for my $x (@arr) { print $x; }
来源：http://uni.zhongyouzk.top

[T46] Perl：哈希操作
来源：http://wft.yonumen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mty.zdbjq.cn

[T47] Perl：正则捕获
来源：http://ajg.ydjk.org.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mtb.zhiwuduotai.top

[T48] Perl：正则替换
来源：http://iqs.9152youxi.cn

$s =~ s/old/new/g;
来源：http://nbj.chenzaomai.com

[T49] Perl：函数
来源：http://nlg.gotoacloud.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qql.bbcook.cn

[T50] Perl：逐行读文件
来源：http://cwz.hesvh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ihu.shuidangran.top

while (my $line = <$fh>) { print $line; }
来源：http://mcd.birdmap.top

[T51] Scala：Hello World
来源：http://zqv.nanxinkj.top

println("Hello")
来源：http://eny.xinyue.icu

[T52] Scala：变量
来源：http://dsj.chenzaomai.com

val a = 1;  var b = 2
来源：http://tdp.zhijiandao.cn

[T53] Scala：字符串插值
来源：http://waq.iojbl.cn

s"值: $b"
来源：http://wxn.xylfe.cn

[T54] Scala：集合映射
来源：http://led.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://fbp.daxiang520.top

[T55] Scala：集合过滤
来源：http://peo.tianlin.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://jtn.hammf.cn

[T56] Scala：样例类
来源：http://ncd.mhx1999.top

case class User(name: String, age: Int)
来源：http://khl.cashguo.top

[T57] Scala：模式匹配
来源：http://afn.xuetiantiany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://woz.sweek.top

[T58] Scala：函数定义
来源：http://gxl.hywenlv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://avp.redwolf501.top

[T59] Scala：循环
来源：http://fpe.yanxiufei.cn

for (i <- 1 to 10) println(i)
来源：http://egx.zhijiandao.cn

[T60] Scala：折叠
来源：http://dvq.fzhhl.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vvl.jqgfzy.top

================================================================================
来源：http://zhz.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ktn.c1oappe.top

================================================================================
来源：http://zjr.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://voz.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://hbh.ivvv.top

[U02] Py：导出 / 安装依赖
来源：http://agj.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://omf.yj202588.top

[U03] Py：加载 .env 配置
来源：http://ayt.316326.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://yru.tianlin.xyz

[U04] Py：变量调试打印
来源：http://ubv.kuanghao11.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://igj.yj20258888.top

[U05] Py：列表去重且保序
来源：http://wbp.pycfn.com

list(dict.fromkeys(arr))
来源：http://frk.uphjek.com

[U06] Py：合并两个字典
来源：http://qyx.xingfuxueyuan.xyz

{**a, **b}
来源：http://sfl.sufxvd.cn

[U07] Py：反转字典键值
来源：http://jln.epnwcf.com

{v: k for k, v in d.items()}
来源：http://eix.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://iao.havefunace.top

[y for x in nested for y in x]
来源：http://vor.dashuyun.cn

[U09] Py：字典取最大值的键
来源：http://ixz.ybcxt.top

max(d, key=d.get)
来源：http://mbd.ydzc1.top

[U10] Py：按值排序字典
来源：http://dhv.xuetiantiany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lwm.fehbvm.com

[U11] Py：生成器表达式
来源：http://wen.smart0.xyz

(x * 2 for x in arr)
来源：http://zkz.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://zgd.chenjidiqi.icu

Counter(arr).most_common(3)
来源：http://vov.52xcode.cn

[U13] Py：固定长度队列
来源：http://bod.zhixingplan.top

deque(maxlen=10)
来源：http://cst.wangshuangyany.cn

[U14] Py：分组收集到列表
来源：http://qds.ywan-chungtsiang.top

defaultdict(list)
来源：http://yrp.zhixingplan.top

[U15] Py：高精度计时
来源：http://gob.snrcjt.cn

t = time.perf_counter()
来源：http://fnr.ctjpmb.com

[U16] Py：命令行参数解析
来源：http://kos.9152youxi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zbx.jqgufenzy.top

[U17] Py：初始化日志
来源：http://iyj.jinqigfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://jdt.yangfankeji.com

[U18] Py：预编译正则
来源：http://iqx.yangfankeji.com

pat = re.compile(r"\d+")
来源：http://gsz.daxiang520.top

[U19] Py：正则替换带回调
来源：http://kdo.yongpay.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zio.meibo888.top

[U20] Py：缓存函数结果
来源：http://vah.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://ugr.haohaochexian.top

[U21] Py：自定义上下文管理器
来源：http://kct.zhongyouzk.top

@contextlib.contextmanager
来源：http://bsn.jlsjyb.cn

[U22] Py：矩阵转置
来源：http://vmq.gotoacloud.top

list(zip(*m))
来源：http://pql.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://mgw.jiagoushi.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qtx.nanxuanxn.top

[U24] Py：路径操作
来源：http://tfc.hfpthk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wbj.zhixingplan.top

[U25] Py：CSV 按字典读
来源：http://kog.jlsjyb.cn

csv.DictReader(f)
来源：http://rof.birdmap.top

[U26] Py：并发下载
来源：http://mii.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ntj.smart0.xyz

[U27] Py：异步 HTTP
来源：http://lpe.sufxvd.cn

aiohttp.ClientSession() 配合 async with
来源：http://gwl.xziqi.cn

[U28] Py：类型别名
来源：http://csr.andypj.xyz

UserId = int
来源：http://bkw.daria6918.cn

[U29] Py：属性校验
来源：http://cqy.ybcxt.top

@property 与 @x.setter 配合
来源：http://nmv.yj20258888.top

[U30] Py：数据类
来源：http://jil.dashuyun.cn

@dataclass(slots=True)
来源：http://wss.yanxiufei.cn

[U31] Py：单测
来源：http://dmv.bjfxy.top

python -m pytest -q
来源：http://weu.hcnkem.com

[U32] Py：代码格式化
来源：http://nqb.zhijiandao.cn

ruff format . && ruff check --fix .
来源：http://viy.quarkkingdee.top

[U33] Py：打包发布
来源：http://zif.gzhubu.top

python -m build  （依赖 pyproject.toml）
来源：http://kay.sxryk.cn

[U34] Py：判断编码
来源：http://zjs.mhx1999.top

chardet.detect(raw)
来源：http://bso.cheryme.top

[U35] Py：发送邮件
来源：http://hoc.52xcode.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://plw.iojbl.cn

[U36] Py：定时任务
来源：http://jzo.fengsongda.top

schedule.every(10).minutes.do(job)
来源：http://uij.9152youxi.cn

[U37] Py：读写 Excel
来源：http://cuv.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://lar.zdqjudy.top

[U38] Py：获取脚本所在目录
来源：http://vri.yvedp.cn

Path(__file__).resolve().parent
来源：http://njk.sjlbkw.cn

[U39] Py：判断是否在交互环境
来源：http://dvg.jinqigufen.top

sys.stdout.isatty()
来源：http://yfx.shanyushiyangkeji.top

[U40] Py：打印到标准错误
来源：http://xzh.hysaishi.cn

print("err", file=sys.stderr)
来源：http://xoa.yvedp.cn

[U41] PHP：初始化 Composer 项目
来源：http://fre.pengpengdd.cyou

composer init;  composer require guzzlehttp/guzzle
来源：http://ytg.shanyushiyangtech.top

[U42] PHP：PSR-4 自动加载
来源：http://kjz.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cvu.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://huu.sufxvd.cn

namespace App\Http;
来源：http://hrw.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://vkq.gzhubu.top

declare(strict_types=1);
来源：http://arj.hysaishi.cn

[U45] PHP：类型声明与返回类型
来源：http://ldm.yuxming.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jnq.tanke756.top

[U46] PHP：可空类型
来源：http://kmt.tianlin.xyz

?string $name = null
来源：http://thx.yj202588.top

[U47] PHP：联合类型
来源：http://bom.ywan-chungtsiang.top

int|string $id
来源：http://roi.yj202588.top

[U48] PHP：纯枚举
来源：http://gha.haohaochexian.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sfk.xuetiantiany.cn

[U49] PHP：只读属性
来源：http://yol.bbcook.cn

public readonly string $name
来源：http://jnj.xylfe.cn

[U50] PHP：构造器属性提升
来源：http://owe.dashuyun.cn

public function __construct(private int $id) {}
来源：http://orp.pengpengdd.cyou

[U51] PHP：数组解构
来源：http://ybj.havefunace.top

[$a, $b] = $arr;
来源：http://trj.dashuyun.cn

[U52] PHP：箭头函数
来源：http://kjx.ydjk.org.cn

$double = fn($x) => $x * 2;
来源：http://qfw.fengsongda.top

[U53] PHP：空合并运算符
来源：http://wmq.shzxlz.cn

$v = $a ?? $b ?? "default";
来源：http://pbc.havefunace.top

[U54] PHP：空安全调用
来源：http://uvs.hnxiangtu.top

$obj?->method()
来源：http://ado.dianchejie.cn

[U55] PHP：match 表达式
来源：http://avr.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://utz.gaohongyu789.top

[U56] PHP：命名参数
来源：http://edz.sjlbkw.cn

f(a: 1, b: 2)
来源：http://kpm.52xcode.cn

[U57] PHP：字符串插值
来源：http://ous.hcnkem.com

"值: {$a}"
来源：http://suj.hnqzz.top

[U58] PHP：数组三件套
来源：http://kif.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://myg.chenzaomai.com

[U59] PHP：自定义排序
来源：http://hfv.shanyushiyangtech.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ftw.cdnleiting.top

[U60] PHP：JSON 编解码
来源：http://ofm.dianchejie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tsd.hammf.cn

[U61] PHP：正则
来源：http://yus.zhijiandao.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ukx.ivvv.top

[U62] PHP：日期对象
来源：http://srs.jinghuilouyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://brk.jianghu66.top

[U63] PHP：文件读写
来源：http://bep.chenlongwang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mvq.meibo888.top

[U64] PHP：目录遍历
来源：http://yuy.hnxiangtu.top

glob("dir/*.php");  scandir("dir");
来源：http://bmm.mhx1999.top

[U65] PHP：会话
来源：http://mma.0kj1m.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tln.iojbl.cn

[U66] PHP：设置 Cookie
来源：http://cht.zhengqikj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xro.hcnkem.com

[U67] PHP：处理文件上传
来源：http://xse.feifeiyinyue.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uve.yuxming.cn

[U68] PHP：PDO 连接
来源：http://tqk.ctjpmb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yjw.wangdashe.top

[U69] PHP：PDO 预处理
来源：http://vqa.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lql.pycfn.com

[U70] PHP：PDO 事务
来源：http://mhc.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dlm.svipenyu.cn

[U71] PHP：抛出异常
来源：http://gvq.yangfankeji.com

throw new RuntimeException("失败", 500);
来源：http://byy.zdqjudy.top

[U72] PHP：写错误日志
来源：http://fbt.shanyushiyangtech.top

error_log("失败: " . $e->getMessage());
来源：http://dgt.52xcode.cn

[U73] PHP：读取 ini 配置
来源：http://zaq.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://enr.fktsv.cn

[U74] PHP：读取环境变量
来源：http://sdu.yj202588.top

getenv("APP_ENV") ?: "production"
来源：http://hkx.fanxiaobao.xyz

[U75] PHP：依赖注入
来源：http://qni.sysykeji.top

composer require psr/container
来源：http://mwx.52xcode.cn

[U76] PHP：简单路由
来源：http://vaf.daria6918.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mvl.daxiang520.top

[U77] PHP：模板渲染
来源：http://ysn.andypj.xyz

composer require twig/twig
来源：http://fxf.c1oappe.top

[U78] PHP：单元测试
来源：http://kvf.dashuyun.cn

composer require --dev phpunit/phpunit
来源：http://hru.zdbjq.cn

[U79] PHP：静态分析
来源：http://qka.zhongyouzk.top

composer require --dev phpstan/phpstan
来源：http://kwt.mhx1999.top

[U80] PHP：代码规范修复
来源：http://rit.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sxf.yanxiufei.cn

[U81] JS：初始化项目
来源：http://fpn.gzhubu.top

npm init -y;  npm i express
来源：http://nqb.shanyushiyangtech.top

[U82] JS：package.json 脚本
来源：http://hfe.yonumen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bao.guowangkeji.top

[U83] JS：ES Module 导入导出
来源：http://mph.smart0.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://tnl.52xcode.cn

[U84] JS：CommonJS 写法
来源：http://znn.wangdashe.top

module.exports = { a };  const { a } = require("./m");
来源：http://meo.zhengqikj.top

[U85] JS：可选链
来源：http://zts.daria6918.cn

a?.b?.c
来源：http://fue.ydzc1.top

[U86] JS：空值合并
来源：http://pzb.xingfuxueyuan.xyz

a ?? b
来源：http://ijp.zhengqikj.top

[U87] JS：解构默认值
来源：http://msc.birdmap.top

const { a = 1, b = 2 } = obj;
来源：http://usu.guannengcc.top

[U88] JS：对象展开合并
来源：http://ozb.nanxuanxn.top

{ ...a, ...b }
来源：http://xor.aizwys.cn

[U89] JS：数组去重
来源：http://iir.ydjk.org.cn

[...new Set(arr)]
来源：http://vql.chenzaomai.com

[U90] JS：数字数组排序
来源：http://jkv.jqgfzy.top

[...arr].sort((a, b) => a - b)
来源：http://ibu.zdqjudy.top


<!-- 参考信息 -->