代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fip.gotoacloud.top

================================================================================
来源：http://qns.dashuyun.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://btr.jlsjyb.cn

================================================================================
来源：http://rfe.daria6918.cn

[T01] Kotlin：Hello World
来源：http://hym.jqgfzy.top

println("Hello")
来源：http://arm.316326.xyz

[T02] Kotlin：变量
来源：http://abl.chenlongwang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mqu.cdnleiting.top

[T03] Kotlin：字符串模板
来源：http://fem.tian-w.cn

"值: $b"
来源：http://rhz.hcnkem.com

[T04] Kotlin：空安全
来源：http://dqh.tanke756.top

val n: String? = null;  n?.length
来源：http://dyr.tanke756.top

[T05] Kotlin：when 表达式
来源：http://wgl.pengpengdd.cyou

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://knx.ivvv.top

[T06] Kotlin：集合映射
来源：http://iam.hammf.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wdp.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://cyy.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zoh.shuidangran.top

[T08] Kotlin：数据类
来源：http://uvj.zhixingplan.top

data class User(val name: String, val age: Int)
来源：http://mvg.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://xes.sweek.top

fun String.exclaim() = this + "!"
来源：http://wuq.zycfv.cn

[T10] Kotlin：默认参数
来源：http://lbi.aibaodan.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://krs.sjlbkw.cn

[T11] Kotlin：协程
来源：http://zkc.jinyuanbaomall.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wbd.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://itj.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://wwb.svipenyu.cn

[T13] Kotlin：只读 Map
来源：http://nkg.svipenyu.cn

val m = mapOf("a" to 1)
来源：http://qpa.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://rxf.dianchejie.cn

for (i in 1..10) println(i)
来源：http://boz.xingfuxueyuan.xyz

[T15] Kotlin：接口
来源：http://cgc.cashguo.top

interface Shape { fun area(): Double }
来源：http://tgq.ybcxt.top

[T16] Swift：Hello World
来源：http://bay.gzhubu.top

print("Hello")
来源：http://nhk.cucudq.cn

[T17] Swift：变量与常量
来源：http://orx.vqdsnc.cn

var a = 1;  let b = 2
来源：http://cae.shanyushiyangkeji.top

[T18] Swift：字符串插值
来源：http://ogb.hysaishi.cn

"值: \(b)"
来源：http://chw.yueranfly.top

[T19] Swift：可选绑定
来源：http://ask.vehdjk.com

if let n = opt { print(n) }
来源：http://oaq.hywenlv.cn

[T20] Swift：数组操作
来源：http://ylv.jyoumei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lxk.zhoulong.xyz

[T21] Swift：遍历
来源：http://ohw.yuanzhike.top

for x in a { print(x) }
来源：http://bvx.guowangkeji.top

[T22] Swift：字典
来源：http://kkn.jlsjyb.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yad.hfpthk.cn

[T23] Swift：函数
来源：http://ixu.birdmap.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yxc.yongpay.top

[T24] Swift：闭包
来源：http://zkw.sxryk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mpi.ybcxt.top

[T25] Swift：结构体
来源：http://hlc.ehwqpu.com

struct P { var x: Int }
来源：http://lho.quarkkingdee.top

[T26] Swift：类与重写
来源：http://vvf.yuanzhike.top

class A: Base { override func f() {} }
来源：http://vwl.svipenyu.cn

[T27] Swift：错误处理
来源：http://yps.hcnkem.com

do { try f() } catch { print(error) }
来源：http://usp.chenzaomai.com

[T28] Swift：枚举
来源：http://aqd.yangfankeji.com

enum Color { case red, green }
来源：http://hpp.hammf.cn

[T29] Swift：guard 提前返回
来源：http://qje.jiagoushi.top

guard let x = opt else { return }
来源：http://ibe.yvedp.cn

[T30] Swift：协议
来源：http://lxo.wangdashe.top

protocol Shape { func area() -> Double }
来源：http://jst.ydzc1.top

[T31] Lua：Hello World
来源：http://ilb.316326.xyz

print("Hello")
来源：http://fje.sjlbkw.cn

[T32] Lua：局部变量
来源：http://iep.sufxvd.cn

local a = 1
来源：http://wrz.cheryme.top

[T33] Lua：表（数组）
来源：http://dnd.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://eou.zhaomingkeji.xyz

[T34] Lua：遍历表
来源：http://rgm.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jek.ppjwa.cn

[T35] Lua：字典表
来源：http://tpm.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://wrk.jianghu66.top

[T36] Lua：函数
来源：http://ywn.fktsv.cn

function add(a, b) return a + b end
来源：http://hnk.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://dou.shanyushiyangkeji.top

"a" .. "b"
来源：http://mkv.jinqigufen.top

[T38] Lua：条件
来源：http://spx.bjfxy.top

if x > 0 then print("正") end
来源：http://cah.nwbrower.top

[T39] Lua：模式匹配
来源：http://nkc.cheryme.top

string.find(s, "%d+")
来源：http://pxg.shangyingyoupin.top

[T40] Lua：元表
来源：http://ksi.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://riy.bjfxy.top

[T41] Perl：Hello World
来源：http://zhu.smart0.xyz

print "Hello\n";
来源：http://jdb.redwolf501.top

[T42] Perl：变量类型
来源：http://oer.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nfk.ybcxt.top

[T43] Perl：字符串插值
来源：http://wnv.jqgufenzy.top

"值: $a"
来源：http://vql.sufxvd.cn

[T44] Perl：条件
来源：http://vit.zdqjudy.top

if ($a > 0) { print "正"; }
来源：http://pel.birdmap.top

[T45] Perl：数组遍历
来源：http://avk.hongshengwenyu.top

for my $x (@arr) { print $x; }
来源：http://cxq.dashuyun.cn

[T46] Perl：哈希操作
来源：http://iie.guowangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fgn.tanke756.top

[T47] Perl：正则捕获
来源：http://pky.xingfuxueyuan.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://wve.meibo888.top

[T48] Perl：正则替换
来源：http://tgx.hammf.cn

$s =~ s/old/new/g;
来源：http://vmq.hammf.cn

[T49] Perl：函数
来源：http://hmg.yongpay.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fda.yj20258888.top

[T50] Perl：逐行读文件
来源：http://jso.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://bjw.yvedp.cn

while (my $line = <$fh>) { print $line; }
来源：http://wsj.zdbjq.cn

[T51] Scala：Hello World
来源：http://emt.cashguo.top

println("Hello")
来源：http://wpx.ehwqpu.com

[T52] Scala：变量
来源：http://dtl.zycfv.cn

val a = 1;  var b = 2
来源：http://wzh.tian-w.cn

[T53] Scala：字符串插值
来源：http://thj.hfpthk.cn

s"值: $b"
来源：http://hpn.jinqigufen.top

[T54] Scala：集合映射
来源：http://wao.sysykeji.top

List(1, 2, 3).map(_ * 2)
来源：http://qzn.jyoumei.cn

[T55] Scala：集合过滤
来源：http://vlr.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://jak.jianghu66.top

[T56] Scala：样例类
来源：http://jom.shuidangran.top

case class User(name: String, age: Int)
来源：http://xfi.ywan-chungtsiang.top

[T57] Scala：模式匹配
来源：http://nfl.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sjh.cdnleiting.top

[T58] Scala：函数定义
来源：http://dmv.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dmr.hcnkem.com

[T59] Scala：循环
来源：http://owv.cashguo.top

for (i <- 1 to 10) println(i)
来源：http://cer.haohaochexian.top

[T60] Scala：折叠
来源：http://jib.fktsv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kxs.cashguo.top

================================================================================
来源：http://cqo.chenlongwang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oue.svipenyu.cn

================================================================================
来源：http://efx.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://kyd.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kvb.cashguo.top

[U02] Py：导出 / 安装依赖
来源：http://ptl.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qqs.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://cmr.ydzc1.top

from dotenv import load_dotenv; load_dotenv()
来源：http://umx.xylfe.cn

[U04] Py：变量调试打印
来源：http://hpf.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://boc.vehdjk.com

[U05] Py：列表去重且保序
来源：http://oiq.uphjek.com

list(dict.fromkeys(arr))
来源：http://uak.xylfe.cn

[U06] Py：合并两个字典
来源：http://nju.kuanghao11.cn

{**a, **b}
来源：http://kdp.jlsjyb.cn

[U07] Py：反转字典键值
来源：http://yos.jqgufenzy.top

{v: k for k, v in d.items()}
来源：http://byj.zhongyouzk.top

[U08] Py：展平二维列表
来源：http://gmt.birdmap.top

[y for x in nested for y in x]
来源：http://egp.birdmap.top

[U09] Py：字典取最大值的键
来源：http://bxp.jlsjyb.cn

max(d, key=d.get)
来源：http://hdt.uphjek.com

[U10] Py：按值排序字典
来源：http://fqq.yueranfly.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mzs.ctjpmb.com

[U11] Py：生成器表达式
来源：http://ulu.sysykeji.top

(x * 2 for x in arr)
来源：http://jfc.ydjk.org.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tid.yueranfly.top

Counter(arr).most_common(3)
来源：http://nez.redwolf501.top

[U13] Py：固定长度队列
来源：http://gie.c1oappe.top

deque(maxlen=10)
来源：http://nyr.guannengcc.top

[U14] Py：分组收集到列表
来源：http://rkq.jqgfzy.top

defaultdict(list)
来源：http://shf.tianlin.xyz

[U15] Py：高精度计时
来源：http://uxj.yvedp.cn

t = time.perf_counter()
来源：http://apz.tian-w.cn

[U16] Py：命令行参数解析
来源：http://jkg.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://czd.52xcode.cn

[U17] Py：初始化日志
来源：http://hts.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://lco.jinghuilouyu.cn

[U18] Py：预编译正则
来源：http://pnk.jqgfzy.top

pat = re.compile(r"\d+")
来源：http://aci.shanyushiyangtech.top

[U19] Py：正则替换带回调
来源：http://cpc.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zfu.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://oaf.fehbvm.com

@functools.lru_cache(maxsize=None)
来源：http://dxg.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://alt.xuetiantiany.cn

@contextlib.contextmanager
来源：http://bqs.sufxvd.cn

[U22] Py：矩阵转置
来源：http://lpb.tianlin.xyz

list(zip(*m))
来源：http://ene.nwbrower.top

[U23] Py：分块读取大文件
来源：http://wwi.wangdashe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pmu.c1oappe.top

[U24] Py：路径操作
来源：http://jgz.shangyingyoupin.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://anp.jqgfzy.top

[U25] Py：CSV 按字典读
来源：http://lbf.haohaochexian.top

csv.DictReader(f)
来源：http://sqw.haohaochexian.top

[U26] Py：并发下载
来源：http://fnp.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ier.fzhhl.top

[U27] Py：异步 HTTP
来源：http://yts.fktsv.cn

aiohttp.ClientSession() 配合 async with
来源：http://lfk.yueranfly.top

[U28] Py：类型别名
来源：http://suc.dashuyun.cn

UserId = int
来源：http://zmw.yangfankeji.com

[U29] Py：属性校验
来源：http://fqg.uphjek.com

@property 与 @x.setter 配合
来源：http://ztc.feifeiyinyue.top

[U30] Py：数据类
来源：http://mzq.ehwqpu.com

@dataclass(slots=True)
来源：http://nte.zhixingplan.top

[U31] Py：单测
来源：http://itz.havefunace.top

python -m pytest -q
来源：http://mak.ivvv.top

[U32] Py：代码格式化
来源：http://gci.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://oun.chenlongwang.top

[U33] Py：打包发布
来源：http://ezr.c1oappe.top

python -m build  （依赖 pyproject.toml）
来源：http://fms.jiagoushi.top

[U34] Py：判断编码
来源：http://piv.xuanzx.com

chardet.detect(raw)
来源：http://tqb.c1oappe.top

[U35] Py：发送邮件
来源：http://xto.sufxvd.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hrk.cheryme.top

[U36] Py：定时任务
来源：http://mol.ywan-chungtsiang.top

schedule.every(10).minutes.do(job)
来源：http://drn.chenzaomai.com

[U37] Py：读写 Excel
来源：http://qvu.9152youxi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://egj.kuanghao11.cn

[U38] Py：获取脚本所在目录
来源：http://ojq.cdnleiting.top

Path(__file__).resolve().parent
来源：http://iaq.tianlin.xyz

[U39] Py：判断是否在交互环境
来源：http://txy.jyoumei.cn

sys.stdout.isatty()
来源：http://lpc.ydjk.org.cn

[U40] Py：打印到标准错误
来源：http://qoi.jlsjyb.cn

print("err", file=sys.stderr)
来源：http://jlj.sufxvd.cn

[U41] PHP：初始化 Composer 项目
来源：http://hqr.bjfxy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ztp.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://hzb.gaohongyu789.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fqi.zhiwuduotai.top

[U43] PHP：声明命名空间
来源：http://tdm.9152youxi.cn

namespace App\Http;
来源：http://hnj.pycfn.com

[U44] PHP：开启严格类型
来源：http://ivm.epnwcf.com

declare(strict_types=1);
来源：http://oqw.jinghuilouyu.cn

[U45] PHP：类型声明与返回类型
来源：http://drk.vqdsnc.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bsz.havefunace.top

[U46] PHP：可空类型
来源：http://jdx.jiagoushi.top

?string $name = null
来源：http://dtc.jinqigfzy.top

[U47] PHP：联合类型
来源：http://uen.jyoumei.cn

int|string $id
来源：http://ssm.yongpay.top

[U48] PHP：纯枚举
来源：http://nre.wangdashe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://obi.xylfe.cn

[U49] PHP：只读属性
来源：http://uwj.ctjpmb.com

public readonly string $name
来源：http://udj.hesvh.cn

[U50] PHP：构造器属性提升
来源：http://xbn.sxryk.cn

public function __construct(private int $id) {}
来源：http://ctu.kuanghao11.cn

[U51] PHP：数组解构
来源：http://ebb.kuanghao11.cn

[$a, $b] = $arr;
来源：http://wjw.smart0.xyz

[U52] PHP：箭头函数
来源：http://pkb.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://goi.sweek.top

[U53] PHP：空合并运算符
来源：http://hyl.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://nmc.ehwqpu.com

[U54] PHP：空安全调用
来源：http://jud.epnwcf.com

$obj?->method()
来源：http://dhi.epnwcf.com

[U55] PHP：match 表达式
来源：http://oys.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vsj.jqgfzy.top

[U56] PHP：命名参数
来源：http://huy.mhx1999.top

f(a: 1, b: 2)
来源：http://njq.cheryme.top

[U57] PHP：字符串插值
来源：http://fln.fengsongda.top

"值: {$a}"
来源：http://oda.c1oappe.top

[U58] PHP：数组三件套
来源：http://tzw.cashguo.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ikh.c1oappe.top

[U59] PHP：自定义排序
来源：http://stw.52xcode.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ozm.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://hnm.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yai.hnxiangtu.top

[U61] PHP：正则
来源：http://euf.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://str.zhijiandao.cn

[U62] PHP：日期对象
来源：http://hec.guowangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vvq.pengpengdd.cyou

[U63] PHP：文件读写
来源：http://guy.ywan-chungtsiang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jyy.sufxvd.cn

[U64] PHP：目录遍历
来源：http://wzm.9152youxi.cn

glob("dir/*.php");  scandir("dir");
来源：http://iei.pengpengdd.cyou

[U65] PHP：会话
来源：http://nwu.haohaochexian.top

session_start();  $_SESSION["uid"] = 1;
来源：http://iuq.hfpthk.cn

[U66] PHP：设置 Cookie
来源：http://upj.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rqw.sjlbkw.cn

[U67] PHP：处理文件上传
来源：http://btl.feifeiyinyue.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tmk.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://dgv.daria6918.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sxj.chenjidiqi.icu

[U69] PHP：PDO 预处理
来源：http://qvt.snrcjt.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fou.tanke756.top

[U70] PHP：PDO 事务
来源：http://tys.zycfv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bgc.yj20258888.top

[U71] PHP：抛出异常
来源：http://jfy.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://nfm.xingfuxueyuan.xyz

[U72] PHP：写错误日志
来源：http://nbr.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://vtp.ppjwa.cn

[U73] PHP：读取 ini 配置
来源：http://lbh.ydzc1.top

parse_ini_file("config.ini", true)
来源：http://zsm.gogol.net.cn

[U74] PHP：读取环境变量
来源：http://acx.guannengcc.top

getenv("APP_ENV") ?: "production"
来源：http://udx.iojbl.cn

[U75] PHP：依赖注入
来源：http://rvc.iojbl.cn

composer require psr/container
来源：http://ivl.yueranfly.top

[U76] PHP：简单路由
来源：http://dsq.yongpay.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xyz.zycfv.cn

[U77] PHP：模板渲染
来源：http://uah.wangshuangyany.cn

composer require twig/twig
来源：http://led.shangyingyoupin.top

[U78] PHP：单元测试
来源：http://egv.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://gkv.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://ulm.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://hek.yfazqb.com

[U80] PHP：代码规范修复
来源：http://nwr.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://yau.wangshuangyany.cn

[U81] JS：初始化项目
来源：http://nmi.daxiang520.top

npm init -y;  npm i express
来源：http://mik.zhiwuduotai.top

[U82] JS：package.json 脚本
来源：http://gkm.zhixingplan.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iqz.jinqigufen.top

[U83] JS：ES Module 导入导出
来源：http://riv.xziqi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://igw.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://xku.gzhubu.top

module.exports = { a };  const { a } = require("./m");
来源：http://rpy.cucudq.cn

[U85] JS：可选链
来源：http://var.redwolf501.top

a?.b?.c
来源：http://enw.daria6918.cn

[U86] JS：空值合并
来源：http://pbr.epnwcf.com

a ?? b
来源：http://wwc.ybcxt.top


<!-- 参考信息 -->