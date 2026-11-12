代发 wailian999

[T01] Kotlin：Hello World
来源：http://ufp.shanyushiyangtech.top

println("Hello")
来源：http://uea.wangdashe.top

[T02] Kotlin：变量
来源：http://zpn.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://scu.bjfxy.top

[T03] Kotlin：字符串模板
来源：http://pyb.hesvh.cn

"值: $b"
来源：http://dqp.yanxiufei.cn

[T04] Kotlin：空安全
来源：http://nzx.smart0.xyz

val n: String? = null;  n?.length
来源：http://jyp.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://hvv.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bnl.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://rrr.haohaochexian.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xsp.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://fpm.zhongyouzk.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gkm.hysaishi.cn

[T08] Kotlin：数据类
来源：http://rrc.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://tix.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://esr.havefunace.top

fun String.exclaim() = this + "!"
来源：http://ufn.guowangkeji.top

[T10] Kotlin：默认参数
来源：http://zse.ehwqpu.com

fun greet(name: String = "World") = "Hi $name"
来源：http://qmt.hywenlv.cn

[T11] Kotlin：协程
来源：http://zep.yangfankeji.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://sdt.xinyue.icu

[T12] Kotlin：解构声明
来源：http://cgs.yanxiufei.cn

val (a, b) = Pair(1, 2)
来源：http://qyg.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://clf.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://buv.hnqzz.top

[T14] Kotlin：循环
来源：http://ukg.316326.xyz

for (i in 1..10) println(i)
来源：http://yhj.316326.xyz

[T15] Kotlin：接口
来源：http://kdi.jinqigufen.top

interface Shape { fun area(): Double }
来源：http://gbi.316326.xyz

[T16] Swift：Hello World
来源：http://fgo.haohaochexian.top

print("Hello")
来源：http://aog.cucudq.cn

[T17] Swift：变量与常量
来源：http://soq.cashguo.top

var a = 1;  let b = 2
来源：http://cys.sxryk.cn

[T18] Swift：字符串插值
来源：http://lfa.zhiwuduotai.top

"值: \(b)"
来源：http://use.meibo888.top

[T19] Swift：可选绑定
来源：http://ysa.nanxinkj.top

if let n = opt { print(n) }
来源：http://biz.feifeiyinyue.top

[T20] Swift：数组操作
来源：http://xrr.sweek.top

var a = [1, 2, 3];  a.append(4)
来源：http://uxq.vqdsnc.cn

[T21] Swift：遍历
来源：http://lzd.uphjek.com

for x in a { print(x) }
来源：http://htk.snrcjt.cn

[T22] Swift：字典
来源：http://oew.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://vqc.chenjidiqi.icu

[T23] Swift：函数
来源：http://gbc.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ylj.jqgfzy.top

[T24] Swift：闭包
来源：http://akq.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xeb.jyoumei.cn

[T25] Swift：结构体
来源：http://smo.shzxlz.cn

struct P { var x: Int }
来源：http://kpk.hnxiangtu.top

[T26] Swift：类与重写
来源：http://zax.tianlin.xyz

class A: Base { override func f() {} }
来源：http://pfg.aibaodan.cn

[T27] Swift：错误处理
来源：http://yhn.ivvv.top

do { try f() } catch { print(error) }
来源：http://tak.uphjek.com

[T28] Swift：枚举
来源：http://uum.sysykeji.top

enum Color { case red, green }
来源：http://rno.andypj.xyz

[T29] Swift：guard 提前返回
来源：http://evb.hfpthk.cn

guard let x = opt else { return }
来源：http://one.pengpengdd.cyou

[T30] Swift：协议
来源：http://tdj.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://hgk.yonumen.top

[T31] Lua：Hello World
来源：http://rue.zhongyouzk.top

print("Hello")
来源：http://ynl.hywenlv.cn

[T32] Lua：局部变量
来源：http://syq.quarkkingdee.top

local a = 1
来源：http://qub.ydzc1.top

[T33] Lua：表（数组）
来源：http://bkt.tarul.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ktl.xziqi.cn

[T34] Lua：遍历表
来源：http://mqy.yfazqb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://soj.bjfxy.top

[T35] Lua：字典表
来源：http://xim.xinyue.icu

local d = { a = 1 };  d.b = 2
来源：http://tvn.dianchejie.cn

[T36] Lua：函数
来源：http://nqe.fzhhl.top

function add(a, b) return a + b end
来源：http://xcj.bbcook.cn

[T37] Lua：字符串拼接
来源：http://qud.cashguo.top

"a" .. "b"
来源：http://skn.hesvh.cn

[T38] Lua：条件
来源：http://zff.iojbl.cn

if x > 0 then print("正") end
来源：http://rrj.jqgufenzy.top

[T39] Lua：模式匹配
来源：http://yey.zhijiandao.cn

string.find(s, "%d+")
来源：http://iak.daria6918.cn

[T40] Lua：元表
来源：http://foa.ivvv.top

setmetatable({}, { __index = base })
来源：http://pwj.xziqi.cn

[T41] Perl：Hello World
来源：http://gxx.xziqi.cn

print "Hello\n";
来源：http://svp.shangyingyoupin.top

[T42] Perl：变量类型
来源：http://cww.tian-w.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xmg.shangyingyoupin.top

[T43] Perl：字符串插值
来源：http://ceq.jinqigufen.top

"值: $a"
来源：http://ody.xylfe.cn

[T44] Perl：条件
来源：http://nwx.bbcook.cn

if ($a > 0) { print "正"; }
来源：http://iwe.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://xjl.fanxiaobao.xyz

for my $x (@arr) { print $x; }
来源：http://cjq.zhiwuduotai.top

[T46] Perl：哈希操作
来源：http://jcv.jyoumei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rix.fengsongda.top

[T47] Perl：正则捕获
来源：http://qkv.gaohongyu789.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yew.smart0.xyz

[T48] Perl：正则替换
来源：http://rjn.fanxiaobao.xyz

$s =~ s/old/new/g;
来源：http://tsm.gzhubu.top

[T49] Perl：函数
来源：http://eib.fengsongda.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://usw.ydzc1.top

[T50] Perl：逐行读文件
来源：http://mjv.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tlt.cucudq.cn

while (my $line = <$fh>) { print $line; }
来源：http://puz.hnqzz.top

[T51] Scala：Hello World
来源：http://cma.wangdashe.top

println("Hello")
来源：http://edg.wangshuangyany.cn

[T52] Scala：变量
来源：http://ekp.bjfxy.top

val a = 1;  var b = 2
来源：http://cxt.tarul.cn

[T53] Scala：字符串插值
来源：http://bbe.chenlongwang.top

s"值: $b"
来源：http://vmf.ppjwa.cn

[T54] Scala：集合映射
来源：http://slr.xuetiantiany.cn

List(1, 2, 3).map(_ * 2)
来源：http://rsj.hammf.cn

[T55] Scala：集合过滤
来源：http://rem.quarkkingdee.top

List(1, 2, 3).filter(_ > 1)
来源：http://vkt.sweek.top

[T56] Scala：样例类
来源：http://zwe.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://tpa.redwolf501.top

[T57] Scala：模式匹配
来源：http://iki.cdnleiting.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kim.xylfe.cn

[T58] Scala：函数定义
来源：http://dvr.pycfn.com

def add(a: Int, b: Int): Int = a + b
来源：http://ieo.hcnkem.com

[T59] Scala：循环
来源：http://ais.pycfn.com

for (i <- 1 to 10) println(i)
来源：http://iuz.hammf.cn

[T60] Scala：折叠
来源：http://zaj.hywenlv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gzd.yueranfly.top

================================================================================
来源：http://soy.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dwp.yj202588.top

================================================================================
来源：http://ilr.shanyushiyangtech.top

[U01] Py：创建虚拟环境
来源：http://rhu.yongpay.top

python -m venv .venv && source .venv/bin/activate
来源：http://aek.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://jyi.jlsjyb.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iqp.xziqi.cn

[U03] Py：加载 .env 配置
来源：http://jer.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qha.chenjidiqi.icu

[U04] Py：变量调试打印
来源：http://hvi.tian-w.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sdt.316326.xyz

[U05] Py：列表去重且保序
来源：http://bis.havefunace.top

list(dict.fromkeys(arr))
来源：http://ray.dashuyun.cn

[U06] Py：合并两个字典
来源：http://sih.hywenlv.cn

{**a, **b}
来源：http://vov.yj202588.top

[U07] Py：反转字典键值
来源：http://kgl.zhengqikj.top

{v: k for k, v in d.items()}
来源：http://qvj.jqgufenzy.top

[U08] Py：展平二维列表
来源：http://umd.cucudq.cn

[y for x in nested for y in x]
来源：http://foa.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://exw.zhiwuduotai.top

max(d, key=d.get)
来源：http://rep.jiagoushi.top

[U10] Py：按值排序字典
来源：http://tim.quarkkingdee.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dav.redwolf501.top

[U11] Py：生成器表达式
来源：http://dan.jqgfzy.top

(x * 2 for x in arr)
来源：http://hut.0kj1m.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mpx.fengsongda.top

Counter(arr).most_common(3)
来源：http://acv.nanxinkj.top

[U13] Py：固定长度队列
来源：http://wsh.xinyue.icu

deque(maxlen=10)
来源：http://hzd.shuidangran.top

[U14] Py：分组收集到列表
来源：http://uwm.gogol.net.cn

defaultdict(list)
来源：http://rhl.52xcode.cn

[U15] Py：高精度计时
来源：http://oey.yfazqb.com

t = time.perf_counter()
来源：http://gyn.hcnkem.com

[U16] Py：命令行参数解析
来源：http://msy.jinqigfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kos.hammf.cn

[U17] Py：初始化日志
来源：http://loi.havefunace.top

logging.basicConfig(level=logging.INFO)
来源：http://spv.hywenlv.cn

[U18] Py：预编译正则
来源：http://mjh.pengpengdd.cyou

pat = re.compile(r"\d+")
来源：http://dmh.aibaodan.cn

[U19] Py：正则替换带回调
来源：http://hch.vqdsnc.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://umu.gogol.net.cn

[U20] Py：缓存函数结果
来源：http://clu.zhongyouzk.top

@functools.lru_cache(maxsize=None)
来源：http://bln.cdnleiting.top

[U21] Py：自定义上下文管理器
来源：http://lmq.sxryk.cn

@contextlib.contextmanager
来源：http://bap.snrcjt.cn

[U22] Py：矩阵转置
来源：http://exl.jqgufenzy.top

list(zip(*m))
来源：http://mny.nanxuanxn.top

[U23] Py：分块读取大文件
来源：http://njo.xziqi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pza.fzhhl.top

[U24] Py：路径操作
来源：http://qrs.jiagoushi.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vxp.ehwqpu.com

[U25] Py：CSV 按字典读
来源：http://duw.fzhhl.top

csv.DictReader(f)
来源：http://fvg.c1oappe.top

[U26] Py：并发下载
来源：http://kxb.wangshuangyany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lri.yj20258.top

[U27] Py：异步 HTTP
来源：http://soo.shzxlz.cn

aiohttp.ClientSession() 配合 async with
来源：http://umx.jqgfzy.top

[U28] Py：类型别名
来源：http://tua.ydzc1.top

UserId = int
来源：http://sgx.chenjidiqi.icu

[U29] Py：属性校验
来源：http://aca.fengsongda.top

@property 与 @x.setter 配合
来源：http://kxb.bjfxy.top

[U30] Py：数据类
来源：http://bbr.wangdashe.top

@dataclass(slots=True)
来源：http://yex.aibaodan.cn

[U31] Py：单测
来源：http://ter.quarkkingdee.top

python -m pytest -q
来源：http://ihl.wangshuangyany.cn

[U32] Py：代码格式化
来源：http://vpc.chenjidiqi.icu

ruff format . && ruff check --fix .
来源：http://kxn.zhoulong.xyz

[U33] Py：打包发布
来源：http://lhx.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://jyh.nanxinkj.top

[U34] Py：判断编码
来源：http://jfr.vehdjk.com

chardet.detect(raw)
来源：http://fwo.52xcode.cn

[U35] Py：发送邮件
来源：http://qnl.cqqwz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cus.ehwqpu.com

[U36] Py：定时任务
来源：http://vva.haohaochexian.top

schedule.every(10).minutes.do(job)
来源：http://alx.ydzc1.top

[U37] Py：读写 Excel
来源：http://pww.tarul.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iti.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://lta.bbcook.cn

Path(__file__).resolve().parent
来源：http://gcl.havefunace.top

[U39] Py：判断是否在交互环境
来源：http://sto.hesvh.cn

sys.stdout.isatty()
来源：http://mxd.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://acr.cqqwz.cn

print("err", file=sys.stderr)
来源：http://rzq.cqqwz.cn

[U41] PHP：初始化 Composer 项目
来源：http://ask.bjfxy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rbz.bbcook.cn

[U42] PHP：PSR-4 自动加载
来源：http://jjr.jqgfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://chl.epnwcf.com

[U43] PHP：声明命名空间
来源：http://cms.hnxiangtu.top

namespace App\Http;
来源：http://pla.yuxming.cn

[U44] PHP：开启严格类型
来源：http://ntw.dashuyun.cn

declare(strict_types=1);
来源：http://wuj.jyoumei.cn

[U45] PHP：类型声明与返回类型
来源：http://jgg.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://onc.zhengqikj.top

[U46] PHP：可空类型
来源：http://qas.ehwqpu.com

?string $name = null
来源：http://hqs.jqgufenzy.top

[U47] PHP：联合类型
来源：http://szd.9152youxi.cn

int|string $id
来源：http://zck.smart0.xyz

[U48] PHP：纯枚举
来源：http://fhy.daxiang520.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cvq.yuxming.cn

[U49] PHP：只读属性
来源：http://xxo.cqqwz.cn

public readonly string $name
来源：http://ymg.tanke756.top

[U50] PHP：构造器属性提升
来源：http://knh.tian-w.cn

public function __construct(private int $id) {}
来源：http://kgu.redwolf501.top

[U51] PHP：数组解构
来源：http://ndn.yongpay.top

[$a, $b] = $arr;
来源：http://udy.ehwqpu.com

[U52] PHP：箭头函数
来源：http://fyl.zhoulong.xyz

$double = fn($x) => $x * 2;
来源：http://gmx.yongpay.top

[U53] PHP：空合并运算符
来源：http://egt.fehbvm.com

$v = $a ?? $b ?? "default";
来源：http://wva.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://jvy.hnqzz.top

$obj?->method()
来源：http://tpy.jyoumei.cn

[U55] PHP：match 表达式
来源：http://hbo.dashuyun.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gub.yanxiufei.cn

[U56] PHP：命名参数
来源：http://ycw.hnxiangtu.top

f(a: 1, b: 2)
来源：http://hem.zycfv.cn

[U57] PHP：字符串插值
来源：http://xih.shzxlz.cn

"值: {$a}"
来源：http://ewf.yfazqb.com

[U58] PHP：数组三件套
来源：http://tjq.mhx1999.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://irj.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://whm.guannengcc.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rdb.sysykeji.top

[U60] PHP：JSON 编解码
来源：http://lxb.gogol.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ovm.yvedp.cn

[U61] PHP：正则
来源：http://vwo.havefunace.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yka.quarkkingdee.top

[U62] PHP：日期对象
来源：http://scm.wangdashe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dnt.quarkkingdee.top

[U63] PHP：文件读写
来源：http://npu.ppjwa.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bvl.vehdjk.com

[U64] PHP：目录遍历
来源：http://qov.gaohongyu789.top

glob("dir/*.php");  scandir("dir");
来源：http://knm.snrcjt.cn

[U65] PHP：会话
来源：http://oyb.ehwqpu.com

session_start();  $_SESSION["uid"] = 1;
来源：http://kxh.nanxinkj.top

[U66] PHP：设置 Cookie
来源：http://aym.jqgfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cob.xylfe.cn

[U67] PHP：处理文件上传
来源：http://zbo.cheryme.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hhi.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://pal.cdnleiting.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hzs.hywenlv.cn

[U69] PHP：PDO 预处理
来源：http://qcp.daxiang520.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dty.hnqzz.top

[U70] PHP：PDO 事务
来源：http://bzq.ybcxt.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://brm.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://kps.zhijiandao.cn

throw new RuntimeException("失败", 500);
来源：http://lsa.yfazqb.com

[U72] PHP：写错误日志
来源：http://waj.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://zvv.xinyue.icu

[U73] PHP：读取 ini 配置
来源：http://onc.cheryme.top

parse_ini_file("config.ini", true)
来源：http://pnr.cucudq.cn

[U74] PHP：读取环境变量
来源：http://ogg.shanyushiyangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://ifx.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://kwp.dianchejie.cn

composer require psr/container
来源：http://gwd.mhx1999.top

[U76] PHP：简单路由
来源：http://zxj.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ymk.haohaochexian.top

[U77] PHP：模板渲染
来源：http://tca.vehdjk.com

composer require twig/twig
来源：http://pob.zhijiandao.cn

[U78] PHP：单元测试
来源：http://tes.cheryme.top

composer require --dev phpunit/phpunit
来源：http://ihk.0kj1m.cn

[U79] PHP：静态分析
来源：http://rhq.epnwcf.com

composer require --dev phpstan/phpstan
来源：http://mjj.yfazqb.com

[U80] PHP：代码规范修复
来源：http://wlv.gaohongyu789.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mzm.jinyuanbaomall.cn

[U81] JS：初始化项目
来源：http://wos.hywenlv.cn

npm init -y;  npm i express
来源：http://kxy.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://iwu.chenjidiqi.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fjs.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://dvy.wangshuangyany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mcg.shzxlz.cn

[U84] JS：CommonJS 写法
来源：http://uyr.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://obr.chenlongwang.top

[U85] JS：可选链
来源：http://nbi.yuxming.cn

a?.b?.c
来源：http://ypo.gzhubu.top

[U86] JS：空值合并
来源：http://uvb.feifeiyinyue.top

a ?? b
来源：http://paf.cucudq.cn

[U87] JS：解构默认值
来源：http://ocz.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://ugw.shanyushiyangkeji.top

[U88] JS：对象展开合并
来源：http://sla.jianghu66.top

{ ...a, ...b }
来源：http://gkz.fzhhl.top


<!-- 参考信息 -->