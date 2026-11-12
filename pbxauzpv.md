代发 wailian999

[T03] Kotlin：字符串模板
来源：http://fnr.sufxvd.cn

"值: $b"
来源：http://ksy.yuanzhike.top

[T04] Kotlin：空安全
来源：http://sdo.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://xao.0kj1m.cn

[T05] Kotlin：when 表达式
来源：http://lsz.andypj.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nrv.fktsv.cn

[T06] Kotlin：集合映射
来源：http://ixu.vqdsnc.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vya.xuanzx.com

[T07] Kotlin：集合过滤
来源：http://vkn.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mcd.hfpthk.cn

[T08] Kotlin：数据类
来源：http://wan.yonumen.top

data class User(val name: String, val age: Int)
来源：http://kgt.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://wny.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://yix.yj20258888.top

[T10] Kotlin：默认参数
来源：http://bpw.bjfxy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://acl.havefunace.top

[T11] Kotlin：协程
来源：http://dpj.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jpo.ybcxt.top

[T12] Kotlin：解构声明
来源：http://dhi.vqdsnc.cn

val (a, b) = Pair(1, 2)
来源：http://kwm.yuxming.cn

[T13] Kotlin：只读 Map
来源：http://azg.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://agi.sjlbkw.cn

[T14] Kotlin：循环
来源：http://fbm.jyoumei.cn

for (i in 1..10) println(i)
来源：http://dgx.jianghu66.top

[T15] Kotlin：接口
来源：http://izl.cucudq.cn

interface Shape { fun area(): Double }
来源：http://ush.hfpthk.cn

[T16] Swift：Hello World
来源：http://dwg.0kj1m.cn

print("Hello")
来源：http://pxn.chenlongwang.top

[T17] Swift：变量与常量
来源：http://cal.aibaodan.cn

var a = 1;  let b = 2
来源：http://dpr.jyoumei.cn

[T18] Swift：字符串插值
来源：http://tzs.svipenyu.cn

"值: \(b)"
来源：http://rdi.nanxinkj.top

[T19] Swift：可选绑定
来源：http://xok.sweek.top

if let n = opt { print(n) }
来源：http://ehq.52xcode.cn

[T20] Swift：数组操作
来源：http://xpw.hcnkem.com

var a = [1, 2, 3];  a.append(4)
来源：http://nja.cdnleiting.top

[T21] Swift：遍历
来源：http://uql.svipenyu.cn

for x in a { print(x) }
来源：http://zdl.bjfxy.top

[T22] Swift：字典
来源：http://nsg.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pmx.yuanzhike.top

[T23] Swift：函数
来源：http://uis.shangyingyoupin.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jpk.jlsjyb.cn

[T24] Swift：闭包
来源：http://izc.sufxvd.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zbq.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://vxh.nwbrower.top

struct P { var x: Int }
来源：http://tyz.c1oappe.top

[T26] Swift：类与重写
来源：http://qjd.meibo888.top

class A: Base { override func f() {} }
来源：http://zyk.pengpengdd.cyou

[T27] Swift：错误处理
来源：http://pql.xylfe.cn

do { try f() } catch { print(error) }
来源：http://wtq.ppjwa.cn

[T28] Swift：枚举
来源：http://tzq.tanke756.top

enum Color { case red, green }
来源：http://rqt.0kj1m.cn

[T29] Swift：guard 提前返回
来源：http://ijd.jinqigfzy.top

guard let x = opt else { return }
来源：http://vby.vehdjk.com

[T30] Swift：协议
来源：http://hap.haohaochexian.top

protocol Shape { func area() -> Double }
来源：http://gba.zhijiandao.cn

[T31] Lua：Hello World
来源：http://eir.hcnkem.com

print("Hello")
来源：http://bgz.ydzc1.top

[T32] Lua：局部变量
来源：http://ttw.redwolf501.top

local a = 1
来源：http://btm.zhoulong.xyz

[T33] Lua：表（数组）
来源：http://yqp.sweek.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ijl.hesvh.cn

[T34] Lua：遍历表
来源：http://fjc.hnxiangtu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jmi.yuanzhike.top

[T35] Lua：字典表
来源：http://kxt.gotoacloud.top

local d = { a = 1 };  d.b = 2
来源：http://msw.epnwcf.com

[T36] Lua：函数
来源：http://eop.cqqwz.cn

function add(a, b) return a + b end
来源：http://yyp.yvedp.cn

[T37] Lua：字符串拼接
来源：http://tsf.fanxiaobao.xyz

"a" .. "b"
来源：http://zvo.zhijiandao.cn

[T38] Lua：条件
来源：http://ixb.zhixingplan.top

if x > 0 then print("正") end
来源：http://zxc.zhengqikj.top

[T39] Lua：模式匹配
来源：http://qkb.zhixingplan.top

string.find(s, "%d+")
来源：http://bve.tarul.cn

[T40] Lua：元表
来源：http://oyb.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://rvh.jqgufenzy.top

[T41] Perl：Hello World
来源：http://mgb.hammf.cn

print "Hello\n";
来源：http://rtk.sysykeji.top

[T42] Perl：变量类型
来源：http://fab.vqdsnc.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yuj.bjfxy.top

[T43] Perl：字符串插值
来源：http://mfj.9152youxi.cn

"值: $a"
来源：http://haa.epnwcf.com

[T44] Perl：条件
来源：http://ymx.redwolf501.top

if ($a > 0) { print "正"; }
来源：http://jxe.zdbjq.cn

[T45] Perl：数组遍历
来源：http://jof.hywenlv.cn

for my $x (@arr) { print $x; }
来源：http://lbq.jianghu66.top

[T46] Perl：哈希操作
来源：http://vjt.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lwb.cucudq.cn

[T47] Perl：正则捕获
来源：http://uyr.nwbrower.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://arf.yj20258.top

[T48] Perl：正则替换
来源：http://yse.guannengcc.top

$s =~ s/old/new/g;
来源：http://uiv.xinyue.icu

[T49] Perl：函数
来源：http://bue.jqgfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gzo.cashguo.top

[T50] Perl：逐行读文件
来源：http://yyt.cucudq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jrt.yj20258.top

while (my $line = <$fh>) { print $line; }
来源：http://njn.chenjidiqi.icu

[T51] Scala：Hello World
来源：http://soh.hnqzz.top

println("Hello")
来源：http://kya.chenzaomai.com

[T52] Scala：变量
来源：http://ueg.guowangkeji.top

val a = 1;  var b = 2
来源：http://efr.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://dno.hammf.cn

s"值: $b"
来源：http://iea.0kj1m.cn

[T54] Scala：集合映射
来源：http://ats.jyoumei.cn

List(1, 2, 3).map(_ * 2)
来源：http://rfq.aibaodan.cn

[T55] Scala：集合过滤
来源：http://ijv.tian-w.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nrf.pycfn.com

[T56] Scala：样例类
来源：http://lcb.gaohongyu789.top

case class User(name: String, age: Int)
来源：http://zbm.ywan-chungtsiang.top

[T57] Scala：模式匹配
来源：http://equ.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pdn.yanxiufei.cn

[T58] Scala：函数定义
来源：http://cig.sxryk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ypp.yangfankeji.com

[T59] Scala：循环
来源：http://uvm.zhengqikj.top

for (i <- 1 to 10) println(i)
来源：http://ekl.vqdsnc.cn

[T60] Scala：折叠
来源：http://atn.meibo888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lin.meibo888.top

================================================================================
来源：http://spx.guowangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bxv.epnwcf.com

================================================================================
来源：http://qow.sjlbkw.cn

[U01] Py：创建虚拟环境
来源：http://xjb.zhijiandao.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bve.ydjk.org.cn

[U02] Py：导出 / 安装依赖
来源：http://gxs.gzhubu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xss.ctjpmb.com

[U03] Py：加载 .env 配置
来源：http://fqz.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wjh.fengsongda.top

[U04] Py：变量调试打印
来源：http://fov.snrcjt.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jli.wangshuangyany.cn

[U05] Py：列表去重且保序
来源：http://uqz.hammf.cn

list(dict.fromkeys(arr))
来源：http://vrk.0kj1m.cn

[U06] Py：合并两个字典
来源：http://nno.xziqi.cn

{**a, **b}
来源：http://sqs.daxiang520.top

[U07] Py：反转字典键值
来源：http://djq.hysaishi.cn

{v: k for k, v in d.items()}
来源：http://wbe.hcnkem.com

[U08] Py：展平二维列表
来源：http://lml.vqdsnc.cn

[y for x in nested for y in x]
来源：http://oul.sufxvd.cn

[U09] Py：字典取最大值的键
来源：http://xqj.yonumen.top

max(d, key=d.get)
来源：http://xzg.mhx1999.top

[U10] Py：按值排序字典
来源：http://oal.kuanghao11.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://smt.dianchejie.cn

[U11] Py：生成器表达式
来源：http://pfb.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://ptg.jqgufenzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://wpk.yj202588.top

Counter(arr).most_common(3)
来源：http://rjw.gogol.net.cn

[U13] Py：固定长度队列
来源：http://jcf.gogol.net.cn

deque(maxlen=10)
来源：http://uqk.aibaodan.cn

[U14] Py：分组收集到列表
来源：http://mom.xinyue.icu

defaultdict(list)
来源：http://vys.xylfe.cn

[U15] Py：高精度计时
来源：http://xne.jinyuanbaomall.cn

t = time.perf_counter()
来源：http://xpb.nwbrower.top

[U16] Py：命令行参数解析
来源：http://hzx.gotoacloud.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tph.vehdjk.com

[U17] Py：初始化日志
来源：http://htk.hongshengwenyu.top

logging.basicConfig(level=logging.INFO)
来源：http://uma.daxiang520.top

[U18] Py：预编译正则
来源：http://aqu.52xcode.cn

pat = re.compile(r"\d+")
来源：http://jhm.fanxiaobao.xyz

[U19] Py：正则替换带回调
来源：http://ueb.guowangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tjk.zhengqikj.top

[U20] Py：缓存函数结果
来源：http://zaq.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://gcd.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://woo.zdqjudy.top

@contextlib.contextmanager
来源：http://xyo.haohaochexian.top

[U22] Py：矩阵转置
来源：http://nmd.hfpthk.cn

list(zip(*m))
来源：http://hpr.yuanzhike.top

[U23] Py：分块读取大文件
来源：http://fdv.zdqjudy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cmn.zdqjudy.top

[U24] Py：路径操作
来源：http://pvu.haohaochexian.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://igr.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://jih.zhengqikj.top

csv.DictReader(f)
来源：http://eax.ywan-chungtsiang.top

[U26] Py：并发下载
来源：http://jot.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://olr.daria6918.cn

[U27] Py：异步 HTTP
来源：http://iyn.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://hlv.xinyue.icu

[U28] Py：类型别名
来源：http://ais.yj20258888.top

UserId = int
来源：http://ojo.jyoumei.cn

[U29] Py：属性校验
来源：http://mxk.jinqigufen.top

@property 与 @x.setter 配合
来源：http://zan.meibo888.top

[U30] Py：数据类
来源：http://mxf.zhongyouzk.top

@dataclass(slots=True)
来源：http://vbh.chenjidiqi.icu

[U31] Py：单测
来源：http://lgt.fzhhl.top

python -m pytest -q
来源：http://nwx.epnwcf.com

[U32] Py：代码格式化
来源：http://tzx.yj20258.top

ruff format . && ruff check --fix .
来源：http://lwe.fktsv.cn

[U33] Py：打包发布
来源：http://msg.yvedp.cn

python -m build  （依赖 pyproject.toml）
来源：http://eln.zhongyouzk.top

[U34] Py：判断编码
来源：http://hkb.shanyushiyangtech.top

chardet.detect(raw)
来源：http://eqt.pengpengdd.cyou

[U35] Py：发送邮件
来源：http://jum.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wfw.tarul.cn

[U36] Py：定时任务
来源：http://pag.epnwcf.com

schedule.every(10).minutes.do(job)
来源：http://sep.zdbjq.cn

[U37] Py：读写 Excel
来源：http://znj.redwolf501.top

pandas.read_excel / DataFrame.to_excel
来源：http://iaj.xuanzx.com

[U38] Py：获取脚本所在目录
来源：http://ojf.hysaishi.cn

Path(__file__).resolve().parent
来源：http://mdd.epnwcf.com

[U39] Py：判断是否在交互环境
来源：http://lpr.wangdashe.top

sys.stdout.isatty()
来源：http://jby.shanyushiyangkeji.top

[U40] Py：打印到标准错误
来源：http://lsg.vehdjk.com

print("err", file=sys.stderr)
来源：http://lrc.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ate.cashguo.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jgv.zdbjq.cn

[U42] PHP：PSR-4 自动加载
来源：http://cxy.jqgfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bjq.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://rzr.ywan-chungtsiang.top

namespace App\Http;
来源：http://pcq.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://eqa.chenlongwang.top

declare(strict_types=1);
来源：http://vsp.0kj1m.cn

[U45] PHP：类型声明与返回类型
来源：http://jpp.sysykeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ifd.svipenyu.cn

[U46] PHP：可空类型
来源：http://aeq.zycfv.cn

?string $name = null
来源：http://oak.vehdjk.com

[U47] PHP：联合类型
来源：http://myn.cqqwz.cn

int|string $id
来源：http://cfp.ybcxt.top

[U48] PHP：纯枚举
来源：http://gvw.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://czy.xziqi.cn

[U49] PHP：只读属性
来源：http://vcw.mhx1999.top

public readonly string $name
来源：http://apt.yuxming.cn

[U50] PHP：构造器属性提升
来源：http://hjo.9152youxi.cn

public function __construct(private int $id) {}
来源：http://pbw.xinyue.icu

[U51] PHP：数组解构
来源：http://egg.andypj.xyz

[$a, $b] = $arr;
来源：http://tgt.jianghu66.top

[U52] PHP：箭头函数
来源：http://nzz.hongshengwenyu.top

$double = fn($x) => $x * 2;
来源：http://zqn.aibaodan.cn

[U53] PHP：空合并运算符
来源：http://mje.nanxinkj.top

$v = $a ?? $b ?? "default";
来源：http://zab.wangshuangyany.cn

[U54] PHP：空安全调用
来源：http://ysg.zdbjq.cn

$obj?->method()
来源：http://dca.chenzaomai.com

[U55] PHP：match 表达式
来源：http://gcz.yj202588.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jcr.kuanghao11.cn

[U56] PHP：命名参数
来源：http://vwi.haohaochexian.top

f(a: 1, b: 2)
来源：http://upe.zhengqikj.top

[U57] PHP：字符串插值
来源：http://ybt.sufxvd.cn

"值: {$a}"
来源：http://bbe.hysaishi.cn

[U58] PHP：数组三件套
来源：http://qib.chenlongwang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://teb.iojbl.cn

[U59] PHP：自定义排序
来源：http://drp.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rkm.fanxiaobao.xyz

[U60] PHP：JSON 编解码
来源：http://hvf.jianghu66.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://waf.tianlin.xyz

[U61] PHP：正则
来源：http://nzz.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://siv.dashuyun.cn

[U62] PHP：日期对象
来源：http://zfv.shangyingyoupin.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mla.xuetiantiany.cn

[U63] PHP：文件读写
来源：http://jsf.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://spw.vqdsnc.cn

[U64] PHP：目录遍历
来源：http://eki.sweek.top

glob("dir/*.php");  scandir("dir");
来源：http://cpf.yfazqb.com

[U65] PHP：会话
来源：http://hde.fzhhl.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xom.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://kee.316326.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gon.jinghuilouyu.cn

[U67] PHP：处理文件上传
来源：http://eoe.cheryme.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kfl.epnwcf.com

[U68] PHP：PDO 连接
来源：http://oco.jinqigfzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sgy.mhx1999.top

[U69] PHP：PDO 预处理
来源：http://kfs.pengpengdd.cyou

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://agy.hnqzz.top

[U70] PHP：PDO 事务
来源：http://oqy.hywenlv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fwr.jyoumei.cn

[U71] PHP：抛出异常
来源：http://drb.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://ibn.shanyushiyangtech.top

[U72] PHP：写错误日志
来源：http://tmd.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://gfk.vehdjk.com

[U73] PHP：读取 ini 配置
来源：http://nqi.ivvv.top

parse_ini_file("config.ini", true)
来源：http://bdr.dashuyun.cn

[U74] PHP：读取环境变量
来源：http://mag.pengpengdd.cyou

getenv("APP_ENV") ?: "production"
来源：http://qyi.fengsongda.top

[U75] PHP：依赖注入
来源：http://gxd.jqgfzy.top

composer require psr/container
来源：http://gyx.zdqjudy.top

[U76] PHP：简单路由
来源：http://uhb.daxiang520.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tzy.zhaomingkeji.xyz

[U77] PHP：模板渲染
来源：http://ggy.fengsongda.top

composer require twig/twig
来源：http://zgz.shzxlz.cn

[U78] PHP：单元测试
来源：http://gxt.gotoacloud.top

composer require --dev phpunit/phpunit
来源：http://ehc.nanxinkj.top

[U79] PHP：静态分析
来源：http://rjd.yvedp.cn

composer require --dev phpstan/phpstan
来源：http://qll.cqqwz.cn

[U80] PHP：代码规范修复
来源：http://sne.xingfuxueyuan.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://bmd.zdqjudy.top

[U81] JS：初始化项目
来源：http://jbu.yonumen.top

npm init -y;  npm i express
来源：http://qpz.dashuyun.cn

[U82] JS：package.json 脚本
来源：http://uhu.tanke756.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pjs.c1oappe.top

[U83] JS：ES Module 导入导出
来源：http://hmm.jiagoushi.top

export const a = 1;  import { a } from "./m.js";
来源：http://skn.havefunace.top

[U84] JS：CommonJS 写法
来源：http://wuw.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://jaz.zhijiandao.cn

[U85] JS：可选链
来源：http://mwn.dianchejie.cn

a?.b?.c
来源：http://pff.yuanzhike.top

[U86] JS：空值合并
来源：http://vxd.hammf.cn

a ?? b
来源：http://kpw.cheryme.top

[U87] JS：解构默认值
来源：http://ogw.yj20258.top

const { a = 1, b = 2 } = obj;
来源：http://xsa.yj20258.top

[U88] JS：对象展开合并
来源：http://xoc.shuidangran.top

{ ...a, ...b }
来源：http://yey.52xcode.cn

[U89] JS：数组去重
来源：http://zkb.hysaishi.cn

[...new Set(arr)]
来源：http://bwh.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://nhq.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://tps.hcnkem.com


<!-- 参考信息 -->