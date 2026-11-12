代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kwk.jqgufenzy.top

================================================================================
来源：http://ygp.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cnu.zhaomingkeji.xyz

================================================================================
来源：http://mju.andypj.xyz

[T01] Kotlin：Hello World
来源：http://oto.shanyushiyangkeji.top

println("Hello")
来源：http://mci.snrcjt.cn

[T02] Kotlin：变量
来源：http://bil.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ncp.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://cdm.zhijiandao.cn

"值: $b"
来源：http://dpk.chenzaomai.com

[T04] Kotlin：空安全
来源：http://rsf.tarul.cn

val n: String? = null;  n?.length
来源：http://vrz.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://tbb.zycfv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sap.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://dob.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://wpu.xuetiantiany.cn

[T07] Kotlin：集合过滤
来源：http://eeb.kuanghao11.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hth.chenzaomai.com

[T08] Kotlin：数据类
来源：http://sef.fengsongda.top

data class User(val name: String, val age: Int)
来源：http://bkb.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://cfm.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://tjg.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://ihk.sufxvd.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uht.yongpay.top

[T11] Kotlin：协程
来源：http://krm.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dqo.zdqjudy.top

[T12] Kotlin：解构声明
来源：http://pdz.zhaomingkeji.xyz

val (a, b) = Pair(1, 2)
来源：http://eyu.xuetiantiany.cn

[T13] Kotlin：只读 Map
来源：http://srl.yvedp.cn

val m = mapOf("a" to 1)
来源：http://kbe.xziqi.cn

[T14] Kotlin：循环
来源：http://ewj.guowangkeji.top

for (i in 1..10) println(i)
来源：http://qib.nwbrower.top

[T15] Kotlin：接口
来源：http://kgz.sweek.top

interface Shape { fun area(): Double }
来源：http://kot.jianghu66.top

[T16] Swift：Hello World
来源：http://mep.cashguo.top

print("Hello")
来源：http://qxy.andypj.xyz

[T17] Swift：变量与常量
来源：http://wdh.quarkkingdee.top

var a = 1;  let b = 2
来源：http://ivv.shuidangran.top

[T18] Swift：字符串插值
来源：http://bfl.meibo888.top

"值: \(b)"
来源：http://huq.uphjek.com

[T19] Swift：可选绑定
来源：http://jbw.sysykeji.top

if let n = opt { print(n) }
来源：http://rzp.nwbrower.top

[T20] Swift：数组操作
来源：http://rjw.nanxuanxn.top

var a = [1, 2, 3];  a.append(4)
来源：http://cjn.zycfv.cn

[T21] Swift：遍历
来源：http://mcr.gotoacloud.top

for x in a { print(x) }
来源：http://cmw.jqgfzy.top

[T22] Swift：字典
来源：http://wbp.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://oxt.shangyingyoupin.top

[T23] Swift：函数
来源：http://vic.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xio.vehdjk.com

[T24] Swift：闭包
来源：http://zea.cheryme.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jrg.hywenlv.cn

[T25] Swift：结构体
来源：http://bxc.gzhubu.top

struct P { var x: Int }
来源：http://ubk.yj20258888.top

[T26] Swift：类与重写
来源：http://wre.zhijiandao.cn

class A: Base { override func f() {} }
来源：http://gsa.dianchejie.cn

[T27] Swift：错误处理
来源：http://hse.0kj1m.cn

do { try f() } catch { print(error) }
来源：http://tyt.yuanzhike.top

[T28] Swift：枚举
来源：http://kla.birdmap.top

enum Color { case red, green }
来源：http://kds.jqgfzy.top

[T29] Swift：guard 提前返回
来源：http://gds.haohaochexian.top

guard let x = opt else { return }
来源：http://tgh.birdmap.top

[T30] Swift：协议
来源：http://qws.jinqigfzy.top

protocol Shape { func area() -> Double }
来源：http://bac.sufxvd.cn

[T31] Lua：Hello World
来源：http://lkc.iojbl.cn

print("Hello")
来源：http://awy.yonumen.top

[T32] Lua：局部变量
来源：http://eji.52xcode.cn

local a = 1
来源：http://xqq.redwolf501.top

[T33] Lua：表（数组）
来源：http://sxx.aibaodan.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rca.redwolf501.top

[T34] Lua：遍历表
来源：http://nul.jyoumei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tqq.52xcode.cn

[T35] Lua：字典表
来源：http://bqm.dianchejie.cn

local d = { a = 1 };  d.b = 2
来源：http://qgo.svipenyu.cn

[T36] Lua：函数
来源：http://jxm.sweek.top

function add(a, b) return a + b end
来源：http://qcb.bjfxy.top

[T37] Lua：字符串拼接
来源：http://nzs.meibo888.top

"a" .. "b"
来源：http://oqp.sysykeji.top

[T38] Lua：条件
来源：http://yvt.hesvh.cn

if x > 0 then print("正") end
来源：http://uzp.andypj.xyz

[T39] Lua：模式匹配
来源：http://orr.nwbrower.top

string.find(s, "%d+")
来源：http://tsx.ctjpmb.com

[T40] Lua：元表
来源：http://yrn.sweek.top

setmetatable({}, { __index = base })
来源：http://kfh.yonumen.top

[T41] Perl：Hello World
来源：http://wyy.yj20258888.top

print "Hello\n";
来源：http://wfa.ydjk.org.cn

[T42] Perl：变量类型
来源：http://tbj.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://all.zhijiandao.cn

[T43] Perl：字符串插值
来源：http://kbi.redwolf501.top

"值: $a"
来源：http://wrw.xziqi.cn

[T44] Perl：条件
来源：http://czc.kuanghao11.cn

if ($a > 0) { print "正"; }
来源：http://ari.tianlin.xyz

[T45] Perl：数组遍历
来源：http://qae.ybcxt.top

for my $x (@arr) { print $x; }
来源：http://osu.zdqjudy.top

[T46] Perl：哈希操作
来源：http://xif.hongshengwenyu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gpk.hysaishi.cn

[T47] Perl：正则捕获
来源：http://zmb.jyoumei.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sud.tarul.cn

[T48] Perl：正则替换
来源：http://tgb.jiagoushi.top

$s =~ s/old/new/g;
来源：http://aco.jianghu66.top

[T49] Perl：函数
来源：http://deh.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://spy.zhongyouzk.top

[T50] Perl：逐行读文件
来源：http://sql.tian-w.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xvs.ybcxt.top

while (my $line = <$fh>) { print $line; }
来源：http://gzg.tanke756.top

[T51] Scala：Hello World
来源：http://tcz.jinghuilouyu.cn

println("Hello")
来源：http://hci.0kj1m.cn

[T52] Scala：变量
来源：http://zzo.xziqi.cn

val a = 1;  var b = 2
来源：http://qli.ppjwa.cn

[T53] Scala：字符串插值
来源：http://zlb.dashuyun.cn

s"值: $b"
来源：http://pfa.ctjpmb.com

[T54] Scala：集合映射
来源：http://zvz.sufxvd.cn

List(1, 2, 3).map(_ * 2)
来源：http://vyk.yj20258888.top

[T55] Scala：集合过滤
来源：http://xlt.sufxvd.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ddx.yj20258888.top

[T56] Scala：样例类
来源：http://xga.xinyue.icu

case class User(name: String, age: Int)
来源：http://voc.andypj.xyz

[T57] Scala：模式匹配
来源：http://juq.feifeiyinyue.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gfe.mhx1999.top

[T58] Scala：函数定义
来源：http://let.jqgufenzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://qxc.ybcxt.top

[T59] Scala：循环
来源：http://ptk.jinyuanbaomall.cn

for (i <- 1 to 10) println(i)
来源：http://yqr.pycfn.com

[T60] Scala：折叠
来源：http://imh.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fvw.sxryk.cn

================================================================================
来源：http://qsa.nwbrower.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qgw.316326.xyz

================================================================================
来源：http://chk.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://wcl.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mnb.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://ygp.iojbl.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://soy.ctjpmb.com

[U03] Py：加载 .env 配置
来源：http://utp.nanxinkj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ash.shuidangran.top

[U04] Py：变量调试打印
来源：http://pmo.ydjk.org.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lxx.yangfankeji.com

[U05] Py：列表去重且保序
来源：http://ldp.vehdjk.com

list(dict.fromkeys(arr))
来源：http://znp.birdmap.top

[U06] Py：合并两个字典
来源：http://jbp.fzhhl.top

{**a, **b}
来源：http://sbq.svipenyu.cn

[U07] Py：反转字典键值
来源：http://xob.zhoulong.xyz

{v: k for k, v in d.items()}
来源：http://qen.tianlin.xyz

[U08] Py：展平二维列表
来源：http://rge.tian-w.cn

[y for x in nested for y in x]
来源：http://fhq.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://wlw.9152youxi.cn

max(d, key=d.get)
来源：http://mlu.xuetiantiany.cn

[U10] Py：按值排序字典
来源：http://dtg.tarul.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vqn.zdbjq.cn

[U11] Py：生成器表达式
来源：http://ehu.quarkkingdee.top

(x * 2 for x in arr)
来源：http://mvj.jinghuilouyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lsu.fanxiaobao.xyz

Counter(arr).most_common(3)
来源：http://ing.iojbl.cn

[U13] Py：固定长度队列
来源：http://kgn.gaohongyu789.top

deque(maxlen=10)
来源：http://chd.yj20258888.top

[U14] Py：分组收集到列表
来源：http://kln.wangshuangyany.cn

defaultdict(list)
来源：http://izy.nanxinkj.top

[U15] Py：高精度计时
来源：http://qkq.ivvv.top

t = time.perf_counter()
来源：http://tvb.tarul.cn

[U16] Py：命令行参数解析
来源：http://fto.zdqjudy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bxw.smart0.xyz

[U17] Py：初始化日志
来源：http://dgs.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://mir.c1oappe.top

[U18] Py：预编译正则
来源：http://mwo.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://hnx.hongshengwenyu.top

[U19] Py：正则替换带回调
来源：http://exj.cdnleiting.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vmw.zhiwuduotai.top

[U20] Py：缓存函数结果
来源：http://qhg.hfpthk.cn

@functools.lru_cache(maxsize=None)
来源：http://gte.mhx1999.top

[U21] Py：自定义上下文管理器
来源：http://jnh.fengsongda.top

@contextlib.contextmanager
来源：http://gxz.feifeiyinyue.top

[U22] Py：矩阵转置
来源：http://gsk.jqgufenzy.top

list(zip(*m))
来源：http://npm.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://bqm.feifeiyinyue.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dhn.yanxiufei.cn

[U24] Py：路径操作
来源：http://frc.hesvh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://efw.ehwqpu.com

[U25] Py：CSV 按字典读
来源：http://glx.yuanzhike.top

csv.DictReader(f)
来源：http://cvo.snrcjt.cn

[U26] Py：并发下载
来源：http://qzy.tianlin.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fpj.jinqigfzy.top

[U27] Py：异步 HTTP
来源：http://qxb.guowangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://frt.xinyue.icu

[U28] Py：类型别名
来源：http://uqn.shanyushiyangtech.top

UserId = int
来源：http://uqt.ybcxt.top

[U29] Py：属性校验
来源：http://agx.hesvh.cn

@property 与 @x.setter 配合
来源：http://bms.hywenlv.cn

[U30] Py：数据类
来源：http://ueq.zhoulong.xyz

@dataclass(slots=True)
来源：http://gce.ywan-chungtsiang.top

[U31] Py：单测
来源：http://hsm.zhongyouzk.top

python -m pytest -q
来源：http://and.fktsv.cn

[U32] Py：代码格式化
来源：http://kgy.cashguo.top

ruff format . && ruff check --fix .
来源：http://uam.chenjidiqi.icu

[U33] Py：打包发布
来源：http://xia.shuidangran.top

python -m build  （依赖 pyproject.toml）
来源：http://isv.yuxming.cn

[U34] Py：判断编码
来源：http://alw.bbcook.cn

chardet.detect(raw)
来源：http://xft.chenlongwang.top

[U35] Py：发送邮件
来源：http://ckp.shanyushiyangtech.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xqi.fzhhl.top

[U36] Py：定时任务
来源：http://gnc.xinyue.icu

schedule.every(10).minutes.do(job)
来源：http://tia.sysykeji.top

[U37] Py：读写 Excel
来源：http://cgs.haohaochexian.top

pandas.read_excel / DataFrame.to_excel
来源：http://qqu.yuanzhike.top

[U38] Py：获取脚本所在目录
来源：http://evc.0kj1m.cn

Path(__file__).resolve().parent
来源：http://ojh.jianghu66.top

[U39] Py：判断是否在交互环境
来源：http://kgi.zhijiandao.cn

sys.stdout.isatty()
来源：http://quf.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://thl.sjlbkw.cn

print("err", file=sys.stderr)
来源：http://jde.fehbvm.com

[U41] PHP：初始化 Composer 项目
来源：http://pza.zdqjudy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ojz.wangshuangyany.cn

[U42] PHP：PSR-4 自动加载
来源：http://ayx.sufxvd.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zhu.zhaomingkeji.xyz

[U43] PHP：声明命名空间
来源：http://ggo.cashguo.top

namespace App\Http;
来源：http://qle.tarul.cn

[U44] PHP：开启严格类型
来源：http://vuz.shzxlz.cn

declare(strict_types=1);
来源：http://uuh.jinqigufen.top

[U45] PHP：类型声明与返回类型
来源：http://wra.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dqt.aibaodan.cn

[U46] PHP：可空类型
来源：http://xqr.hysaishi.cn

?string $name = null
来源：http://tak.nanxuanxn.top

[U47] PHP：联合类型
来源：http://vjg.havefunace.top

int|string $id
来源：http://uni.ydzc1.top

[U48] PHP：纯枚举
来源：http://ccd.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jrx.shanyushiyangkeji.top

[U49] PHP：只读属性
来源：http://uok.hfpthk.cn

public readonly string $name
来源：http://kch.ydjk.org.cn

[U50] PHP：构造器属性提升
来源：http://ncw.guowangkeji.top

public function __construct(private int $id) {}
来源：http://xcq.hfpthk.cn

[U51] PHP：数组解构
来源：http://ywi.0kj1m.cn

[$a, $b] = $arr;
来源：http://jdw.zhijiandao.cn

[U52] PHP：箭头函数
来源：http://kxj.fehbvm.com

$double = fn($x) => $x * 2;
来源：http://pny.aibaodan.cn

[U53] PHP：空合并运算符
来源：http://bfx.fktsv.cn

$v = $a ?? $b ?? "default";
来源：http://bod.hcnkem.com

[U54] PHP：空安全调用
来源：http://sgi.sufxvd.cn

$obj?->method()
来源：http://esv.jianghu66.top

[U55] PHP：match 表达式
来源：http://npg.yfazqb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wrc.hnxiangtu.top

[U56] PHP：命名参数
来源：http://kdv.aibaodan.cn

f(a: 1, b: 2)
来源：http://wsj.bbcook.cn

[U57] PHP：字符串插值
来源：http://cjl.zhijiandao.cn

"值: {$a}"
来源：http://myz.zhijiandao.cn

[U58] PHP：数组三件套
来源：http://hpx.shzxlz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cwj.sysykeji.top

[U59] PHP：自定义排序
来源：http://upr.redwolf501.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pse.zhoulong.xyz

[U60] PHP：JSON 编解码
来源：http://zhh.epnwcf.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xts.fanxiaobao.xyz

[U61] PHP：正则
来源：http://nmg.cqqwz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uya.jinghuilouyu.cn

[U62] PHP：日期对象
来源：http://rtn.ydzc1.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://prq.shanyushiyangkeji.top

[U63] PHP：文件读写
来源：http://jcq.yuxming.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jca.cheryme.top

[U64] PHP：目录遍历
来源：http://lse.daxiang520.top

glob("dir/*.php");  scandir("dir");
来源：http://bry.ybcxt.top

[U65] PHP：会话
来源：http://seq.ywan-chungtsiang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rnk.tanke756.top

[U66] PHP：设置 Cookie
来源：http://crd.zdqjudy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pqm.tarul.cn

[U67] PHP：处理文件上传
来源：http://qre.aizwys.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dis.smart0.xyz

[U68] PHP：PDO 连接
来源：http://wpj.hongshengwenyu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qch.ppjwa.cn

[U69] PHP：PDO 预处理
来源：http://ghs.snrcjt.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hgz.fanxiaobao.xyz

[U70] PHP：PDO 事务
来源：http://our.gzhubu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ufv.fktsv.cn

[U71] PHP：抛出异常
来源：http://jtv.hywenlv.cn

throw new RuntimeException("失败", 500);
来源：http://fys.fehbvm.com

[U72] PHP：写错误日志
来源：http://bzm.hywenlv.cn

error_log("失败: " . $e->getMessage());
来源：http://mbc.havefunace.top

[U73] PHP：读取 ini 配置
来源：http://tfg.yj202588.top

parse_ini_file("config.ini", true)
来源：http://lvz.aizwys.cn

[U74] PHP：读取环境变量
来源：http://mwz.zhaomingkeji.xyz

getenv("APP_ENV") ?: "production"
来源：http://emm.shanyushiyangkeji.top

[U75] PHP：依赖注入
来源：http://vms.shzxlz.cn

composer require psr/container
来源：http://hsv.haohaochexian.top

[U76] PHP：简单路由
来源：http://uln.bbcook.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bfs.andypj.xyz

[U77] PHP：模板渲染
来源：http://tfa.bjfxy.top

composer require twig/twig
来源：http://qvb.hesvh.cn

[U78] PHP：单元测试
来源：http://mfi.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://gjo.hfpthk.cn

[U79] PHP：静态分析
来源：http://uud.guowangkeji.top

composer require --dev phpstan/phpstan
来源：http://tif.zhengqikj.top

[U80] PHP：代码规范修复
来源：http://lly.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://twb.jianghu66.top

[U81] JS：初始化项目
来源：http://ado.birdmap.top

npm init -y;  npm i express
来源：http://mme.andypj.xyz

[U82] JS：package.json 脚本
来源：http://rli.gaohongyu789.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ltt.yuanzhike.top

[U83] JS：ES Module 导入导出
来源：http://mze.fanxiaobao.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://mvz.jinghuilouyu.cn

[U84] JS：CommonJS 写法
来源：http://ybk.yj20258.top

module.exports = { a };  const { a } = require("./m");
来源：http://ifq.birdmap.top

[U85] JS：可选链
来源：http://eko.hongshengwenyu.top

a?.b?.c
来源：http://ojk.wangshuangyany.cn

[U86] JS：空值合并
来源：http://kzk.fktsv.cn

a ?? b
来源：http://vaw.tarul.cn


<!-- 参考信息 -->