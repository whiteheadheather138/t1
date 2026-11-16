代发 wailian999

[T03] Kotlin：字符串模板
来源：http://sti.wangshuangyany.cn

"值: $b"
来源：http://qny.yangfankeji.com

[T04] Kotlin：空安全
来源：http://ith.jinyuanbaomall.cn

val n: String? = null;  n?.length
来源：http://rjt.tarul.cn

[T05] Kotlin：when 表达式
来源：http://bad.dashuyun.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jqw.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://idv.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yqi.sxryk.cn

[T07] Kotlin：集合过滤
来源：http://xzc.zhongyouzk.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vob.guowangkeji.top

[T08] Kotlin：数据类
来源：http://vkl.vqdsnc.cn

data class User(val name: String, val age: Int)
来源：http://jmf.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://lot.yueranfly.top

fun String.exclaim() = this + "!"
来源：http://nmh.fzhhl.top

[T10] Kotlin：默认参数
来源：http://wwe.yangfankeji.com

fun greet(name: String = "World") = "Hi $name"
来源：http://xsv.xuanzx.com

[T11] Kotlin：协程
来源：http://pzj.zhixingplan.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ppk.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://aql.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://ngh.zdbjq.cn

[T13] Kotlin：只读 Map
来源：http://org.redwolf501.top

val m = mapOf("a" to 1)
来源：http://wdg.cqqwz.cn

[T14] Kotlin：循环
来源：http://sei.fanxiaobao.xyz

for (i in 1..10) println(i)
来源：http://tim.sysykeji.top

[T15] Kotlin：接口
来源：http://xlw.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://mkw.sweek.top

[T16] Swift：Hello World
来源：http://ltb.chenjidiqi.icu

print("Hello")
来源：http://zlp.ehwqpu.com

[T17] Swift：变量与常量
来源：http://gwk.yanxiufei.cn

var a = 1;  let b = 2
来源：http://ixd.mhx1999.top

[T18] Swift：字符串插值
来源：http://aif.gotoacloud.top

"值: \(b)"
来源：http://ohq.ppjwa.cn

[T19] Swift：可选绑定
来源：http://qpg.zhoulong.xyz

if let n = opt { print(n) }
来源：http://hxu.nwbrower.top

[T20] Swift：数组操作
来源：http://sdo.cashguo.top

var a = [1, 2, 3];  a.append(4)
来源：http://eze.sjlbkw.cn

[T21] Swift：遍历
来源：http://ppi.yuxming.cn

for x in a { print(x) }
来源：http://dcj.sysykeji.top

[T22] Swift：字典
来源：http://ufb.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://tyj.hywenlv.cn

[T23] Swift：函数
来源：http://add.cucudq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dla.feifeiyinyue.top

[T24] Swift：闭包
来源：http://vqq.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hdt.hesvh.cn

[T25] Swift：结构体
来源：http://bpu.vqdsnc.cn

struct P { var x: Int }
来源：http://los.jqgufenzy.top

[T26] Swift：类与重写
来源：http://exi.tanke756.top

class A: Base { override func f() {} }
来源：http://srf.yuxming.cn

[T27] Swift：错误处理
来源：http://hsx.xziqi.cn

do { try f() } catch { print(error) }
来源：http://xqa.sufxvd.cn

[T28] Swift：枚举
来源：http://lki.yongpay.top

enum Color { case red, green }
来源：http://ogi.quarkkingdee.top

[T29] Swift：guard 提前返回
来源：http://vei.yvedp.cn

guard let x = opt else { return }
来源：http://rls.fktsv.cn

[T30] Swift：协议
来源：http://bmn.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://klm.fehbvm.com

[T31] Lua：Hello World
来源：http://gqk.zhixingplan.top

print("Hello")
来源：http://xxs.havefunace.top

[T32] Lua：局部变量
来源：http://ttd.quarkkingdee.top

local a = 1
来源：http://znu.xuanzx.com

[T33] Lua：表（数组）
来源：http://uff.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ptb.xylfe.cn

[T34] Lua：遍历表
来源：http://tdj.xuetiantiany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kre.hcnkem.com

[T35] Lua：字典表
来源：http://xzu.zhixingplan.top

local d = { a = 1 };  d.b = 2
来源：http://ect.aibaodan.cn

[T36] Lua：函数
来源：http://umq.fzhhl.top

function add(a, b) return a + b end
来源：http://nxr.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://vms.jiagoushi.top

"a" .. "b"
来源：http://vgk.sjlbkw.cn

[T38] Lua：条件
来源：http://lpe.guannengcc.top

if x > 0 then print("正") end
来源：http://ode.ppjwa.cn

[T39] Lua：模式匹配
来源：http://udn.gzhubu.top

string.find(s, "%d+")
来源：http://zqq.jinghuilouyu.cn

[T40] Lua：元表
来源：http://rik.ctjpmb.com

setmetatable({}, { __index = base })
来源：http://lpo.hfpthk.cn

[T41] Perl：Hello World
来源：http://gsm.vehdjk.com

print "Hello\n";
来源：http://nue.jianghu66.top

[T42] Perl：变量类型
来源：http://hnr.hongshengwenyu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lmo.yuanzhike.top

[T43] Perl：字符串插值
来源：http://wfq.iojbl.cn

"值: $a"
来源：http://afn.fzhhl.top

[T44] Perl：条件
来源：http://ajn.haohaochexian.top

if ($a > 0) { print "正"; }
来源：http://wfv.xinyue.icu

[T45] Perl：数组遍历
来源：http://ova.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://sbz.gogol.net.cn

[T46] Perl：哈希操作
来源：http://jvd.guowangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nym.birdmap.top

[T47] Perl：正则捕获
来源：http://arq.c1oappe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xbc.yonumen.top

[T48] Perl：正则替换
来源：http://jsx.yj20258.top

$s =~ s/old/new/g;
来源：http://aqj.hfpthk.cn

[T49] Perl：函数
来源：http://ltv.ivvv.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pjo.birdmap.top

[T50] Perl：逐行读文件
来源：http://lqg.nwbrower.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jgh.shzxlz.cn

while (my $line = <$fh>) { print $line; }
来源：http://pse.jinqigufen.top

[T51] Scala：Hello World
来源：http://jwq.ydzc1.top

println("Hello")
来源：http://cph.yuanzhike.top

[T52] Scala：变量
来源：http://tzh.ydzc1.top

val a = 1;  var b = 2
来源：http://bvg.tianlin.xyz

[T53] Scala：字符串插值
来源：http://zso.guannengcc.top

s"值: $b"
来源：http://bdp.pycfn.com

[T54] Scala：集合映射
来源：http://ysk.fehbvm.com

List(1, 2, 3).map(_ * 2)
来源：http://iuv.sysykeji.top

[T55] Scala：集合过滤
来源：http://lsf.gogol.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vzu.hongshengwenyu.top

[T56] Scala：样例类
来源：http://isb.redwolf501.top

case class User(name: String, age: Int)
来源：http://gii.ivvv.top

[T57] Scala：模式匹配
来源：http://zds.pycfn.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://cdi.hnqzz.top

[T58] Scala：函数定义
来源：http://jxz.zycfv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cql.dashuyun.cn

[T59] Scala：循环
来源：http://crw.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://jnn.cashguo.top

[T60] Scala：折叠
来源：http://njz.nwbrower.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yvr.aizwys.cn

================================================================================
来源：http://lnj.yuanzhike.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tqt.yangfankeji.com

================================================================================
来源：http://cty.guowangkeji.top

[U01] Py：创建虚拟环境
来源：http://vex.tian-w.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mes.smart0.xyz

[U02] Py：导出 / 安装依赖
来源：http://lbi.zhongyouzk.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fli.meibo888.top

[U03] Py：加载 .env 配置
来源：http://yej.sysykeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://scr.shangyingyoupin.top

[U04] Py：变量调试打印
来源：http://nao.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oyl.yvedp.cn

[U05] Py：列表去重且保序
来源：http://orp.epnwcf.com

list(dict.fromkeys(arr))
来源：http://ijk.jlsjyb.cn

[U06] Py：合并两个字典
来源：http://dij.jyoumei.cn

{**a, **b}
来源：http://luz.wangshuangyany.cn

[U07] Py：反转字典键值
来源：http://rif.wangshuangyany.cn

{v: k for k, v in d.items()}
来源：http://dfg.birdmap.top

[U08] Py：展平二维列表
来源：http://tmf.quarkkingdee.top

[y for x in nested for y in x]
来源：http://kql.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://xus.mhx1999.top

max(d, key=d.get)
来源：http://lzc.zhixingplan.top

[U10] Py：按值排序字典
来源：http://frd.nanxuanxn.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qth.jyoumei.cn

[U11] Py：生成器表达式
来源：http://vbo.xziqi.cn

(x * 2 for x in arr)
来源：http://kee.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zsq.c1oappe.top

Counter(arr).most_common(3)
来源：http://xny.shanyushiyangkeji.top

[U13] Py：固定长度队列
来源：http://qgh.bbcook.cn

deque(maxlen=10)
来源：http://ocg.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://qru.yj20258888.top

defaultdict(list)
来源：http://egc.gaohongyu789.top

[U15] Py：高精度计时
来源：http://adk.cheryme.top

t = time.perf_counter()
来源：http://feq.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://jqj.ehwqpu.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pvj.shzxlz.cn

[U17] Py：初始化日志
来源：http://mfz.aizwys.cn

logging.basicConfig(level=logging.INFO)
来源：http://tdm.yj202588.top

[U18] Py：预编译正则
来源：http://lsg.bbcook.cn

pat = re.compile(r"\d+")
来源：http://fmk.hnqzz.top

[U19] Py：正则替换带回调
来源：http://lwj.mhx1999.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ibf.yj20258.top

[U20] Py：缓存函数结果
来源：http://kvw.jinqigfzy.top

@functools.lru_cache(maxsize=None)
来源：http://mih.ehwqpu.com

[U21] Py：自定义上下文管理器
来源：http://dwn.hywenlv.cn

@contextlib.contextmanager
来源：http://ddd.redwolf501.top

[U22] Py：矩阵转置
来源：http://zeo.bbcook.cn

list(zip(*m))
来源：http://xvp.hfpthk.cn

[U23] Py：分块读取大文件
来源：http://zfm.bbcook.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iqg.birdmap.top

[U24] Py：路径操作
来源：http://wwe.ybcxt.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mao.yueranfly.top

[U25] Py：CSV 按字典读
来源：http://dyl.kuanghao11.cn

csv.DictReader(f)
来源：http://qys.fehbvm.com

[U26] Py：并发下载
来源：http://hgb.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://esg.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://ong.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://phm.sxryk.cn

[U28] Py：类型别名
来源：http://edp.fengsongda.top

UserId = int
来源：http://zcx.birdmap.top

[U29] Py：属性校验
来源：http://nds.ivvv.top

@property 与 @x.setter 配合
来源：http://otj.jqgfzy.top

[U30] Py：数据类
来源：http://mrt.9152youxi.cn

@dataclass(slots=True)
来源：http://ljd.bbcook.cn

[U31] Py：单测
来源：http://kox.yfazqb.com

python -m pytest -q
来源：http://erq.tarul.cn

[U32] Py：代码格式化
来源：http://xfy.yfazqb.com

ruff format . && ruff check --fix .
来源：http://kkx.fengsongda.top

[U33] Py：打包发布
来源：http://vuy.iojbl.cn

python -m build  （依赖 pyproject.toml）
来源：http://afo.c1oappe.top

[U34] Py：判断编码
来源：http://dra.zdqjudy.top

chardet.detect(raw)
来源：http://gga.cashguo.top

[U35] Py：发送邮件
来源：http://crk.shangyingyoupin.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gnn.zhiwuduotai.top

[U36] Py：定时任务
来源：http://cya.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://ank.cqqwz.cn

[U37] Py：读写 Excel
来源：http://taz.yfazqb.com

pandas.read_excel / DataFrame.to_excel
来源：http://soi.daria6918.cn

[U38] Py：获取脚本所在目录
来源：http://nji.shanyushiyangtech.top

Path(__file__).resolve().parent
来源：http://bko.yfazqb.com

[U39] Py：判断是否在交互环境
来源：http://ekw.zhiwuduotai.top

sys.stdout.isatty()
来源：http://mrn.iojbl.cn

[U40] Py：打印到标准错误
来源：http://bky.yj202588.top

print("err", file=sys.stderr)
来源：http://pui.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://bnb.fzhhl.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fii.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://oxk.andypj.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lvd.hammf.cn

[U43] PHP：声明命名空间
来源：http://hqk.hnxiangtu.top

namespace App\Http;
来源：http://bix.chenjidiqi.icu

[U44] PHP：开启严格类型
来源：http://szc.zdqjudy.top

declare(strict_types=1);
来源：http://ipl.zdbjq.cn

[U45] PHP：类型声明与返回类型
来源：http://xon.c1oappe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rmy.haohaochexian.top

[U46] PHP：可空类型
来源：http://qix.hfpthk.cn

?string $name = null
来源：http://jjc.ppjwa.cn

[U47] PHP：联合类型
来源：http://jrv.quarkkingdee.top

int|string $id
来源：http://lku.haohaochexian.top

[U48] PHP：纯枚举
来源：http://fjw.fktsv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rqn.vehdjk.com

[U49] PHP：只读属性
来源：http://hwx.nanxuanxn.top

public readonly string $name
来源：http://hiq.ywan-chungtsiang.top

[U50] PHP：构造器属性提升
来源：http://gmu.hywenlv.cn

public function __construct(private int $id) {}
来源：http://tvx.ydzc1.top

[U51] PHP：数组解构
来源：http://xje.jqgfzy.top

[$a, $b] = $arr;
来源：http://leq.haohaochexian.top

[U52] PHP：箭头函数
来源：http://ikv.jinqigfzy.top

$double = fn($x) => $x * 2;
来源：http://zig.tanke756.top

[U53] PHP：空合并运算符
来源：http://cqz.nwbrower.top

$v = $a ?? $b ?? "default";
来源：http://cdh.cdnleiting.top

[U54] PHP：空安全调用
来源：http://zga.redwolf501.top

$obj?->method()
来源：http://sgx.jyoumei.cn

[U55] PHP：match 表达式
来源：http://byd.ydjk.org.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rzu.tarul.cn

[U56] PHP：命名参数
来源：http://hfh.shzxlz.cn

f(a: 1, b: 2)
来源：http://mdr.shanyushiyangkeji.top

[U57] PHP：字符串插值
来源：http://izp.vehdjk.com

"值: {$a}"
来源：http://eou.andypj.xyz

[U58] PHP：数组三件套
来源：http://aej.316326.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://afp.birdmap.top

[U59] PHP：自定义排序
来源：http://ejj.wangdashe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gtc.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://erv.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ove.pycfn.com

[U61] PHP：正则
来源：http://vol.mhx1999.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jfz.jyoumei.cn

[U62] PHP：日期对象
来源：http://jne.jinqigfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jqk.fanxiaobao.xyz

[U63] PHP：文件读写
来源：http://lme.wangshuangyany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://egp.xuetiantiany.cn

[U64] PHP：目录遍历
来源：http://ujx.316326.xyz

glob("dir/*.php");  scandir("dir");
来源：http://ssn.zhengqikj.top

[U65] PHP：会话
来源：http://brh.zhixingplan.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dvf.shuidangran.top

[U66] PHP：设置 Cookie
来源：http://kuz.hnxiangtu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ceo.yuxming.cn

[U67] PHP：处理文件上传
来源：http://xpy.fktsv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xcd.jiagoushi.top

[U68] PHP：PDO 连接
来源：http://mub.shuidangran.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wlf.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://ibz.chenlongwang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rhg.jinqigfzy.top

[U70] PHP：PDO 事务
来源：http://ybt.hywenlv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dhs.jinyuanbaomall.cn

[U71] PHP：抛出异常
来源：http://ffm.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://hwe.hnqzz.top

[U72] PHP：写错误日志
来源：http://sps.fzhhl.top

error_log("失败: " . $e->getMessage());
来源：http://tom.hnqzz.top

[U73] PHP：读取 ini 配置
来源：http://qvv.yuanzhike.top

parse_ini_file("config.ini", true)
来源：http://oyf.nanxinkj.top

[U74] PHP：读取环境变量
来源：http://zdu.hnxiangtu.top

getenv("APP_ENV") ?: "production"
来源：http://wjd.sweek.top

[U75] PHP：依赖注入
来源：http://lpe.pycfn.com

composer require psr/container
来源：http://icg.wangshuangyany.cn

[U76] PHP：简单路由
来源：http://zgf.meibo888.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sbm.guowangkeji.top

[U77] PHP：模板渲染
来源：http://pyu.gaohongyu789.top

composer require twig/twig
来源：http://sjr.zhoulong.xyz

[U78] PHP：单元测试
来源：http://bog.ehwqpu.com

composer require --dev phpunit/phpunit
来源：http://cgx.hnxiangtu.top

[U79] PHP：静态分析
来源：http://mib.hammf.cn

composer require --dev phpstan/phpstan
来源：http://nwk.haohaochexian.top

[U80] PHP：代码规范修复
来源：http://egi.tianlin.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://sbn.cdnleiting.top

[U81] JS：初始化项目
来源：http://vzy.jianghu66.top

npm init -y;  npm i express
来源：http://pcq.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://taj.tianlin.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uyg.cdnleiting.top

[U83] JS：ES Module 导入导出
来源：http://dlf.sjlbkw.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wzd.wangshuangyany.cn

[U84] JS：CommonJS 写法
来源：http://ojf.shanyushiyangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://eps.zhoulong.xyz

[U85] JS：可选链
来源：http://fdz.dianchejie.cn

a?.b?.c
来源：http://qff.sweek.top

[U86] JS：空值合并
来源：http://qut.cucudq.cn

a ?? b
来源：http://brn.nanxuanxn.top

[U87] JS：解构默认值
来源：http://dhl.fengsongda.top

const { a = 1, b = 2 } = obj;
来源：http://mia.aibaodan.cn

[U88] JS：对象展开合并
来源：http://esx.xuanzx.com

{ ...a, ...b }
来源：http://hgs.yuxming.cn

[U89] JS：数组去重
来源：http://niz.cucudq.cn

[...new Set(arr)]
来源：http://kdc.fengsongda.top

[U90] JS：数字数组排序
来源：http://ben.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://tbv.ybcxt.top


<!-- 参考信息 -->