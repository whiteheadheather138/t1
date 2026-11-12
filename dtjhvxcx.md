代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://bcr.ydzc1.top

[S59] C++：静态断言
来源：http://ijb.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rgm.gogol.net.cn

[S60] C++：遍历并删除元素
来源：http://lgx.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qzh.zdqjudy.top

================================================================================
来源：http://cza.shangyingyoupin.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ouq.gotoacloud.top

================================================================================
来源：http://bjp.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://llc.hammf.cn

println("Hello")
来源：http://jiu.sjlbkw.cn

[T02] Kotlin：变量
来源：http://vrs.yj202588.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dsz.jinghuilouyu.cn

[T03] Kotlin：字符串模板
来源：http://nlc.xinyue.icu

"值: $b"
来源：http://who.vqdsnc.cn

[T04] Kotlin：空安全
来源：http://vde.ehwqpu.com

val n: String? = null;  n?.length
来源：http://wwo.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://ghh.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uxf.316326.xyz

[T06] Kotlin：集合映射
来源：http://hbx.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pqk.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://blv.jqgfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://edj.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://uub.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://zyb.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://ybj.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://lsl.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://oxh.yfazqb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://aww.yfazqb.com

[T11] Kotlin：协程
来源：http://wkq.cheryme.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zcj.xinyue.icu

[T12] Kotlin：解构声明
来源：http://liu.wangdashe.top

val (a, b) = Pair(1, 2)
来源：http://pgh.bbcook.cn

[T13] Kotlin：只读 Map
来源：http://byl.jianghu66.top

val m = mapOf("a" to 1)
来源：http://duu.yj202588.top

[T14] Kotlin：循环
来源：http://klz.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://otn.nanxuanxn.top

[T15] Kotlin：接口
来源：http://rqg.yuxming.cn

interface Shape { fun area(): Double }
来源：http://fcp.vqdsnc.cn

[T16] Swift：Hello World
来源：http://isg.tian-w.cn

print("Hello")
来源：http://zro.jqgfzy.top

[T17] Swift：变量与常量
来源：http://cdd.zhongyouzk.top

var a = 1;  let b = 2
来源：http://dmq.sjlbkw.cn

[T18] Swift：字符串插值
来源：http://jmx.aizwys.cn

"值: \(b)"
来源：http://xoa.bjfxy.top

[T19] Swift：可选绑定
来源：http://bbg.tarul.cn

if let n = opt { print(n) }
来源：http://amh.aizwys.cn

[T20] Swift：数组操作
来源：http://lrp.zhaomingkeji.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://mdj.fehbvm.com

[T21] Swift：遍历
来源：http://zdb.aizwys.cn

for x in a { print(x) }
来源：http://gzu.jlsjyb.cn

[T22] Swift：字典
来源：http://rgy.gogol.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hmi.ctjpmb.com

[T23] Swift：函数
来源：http://qbs.quarkkingdee.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://siy.gotoacloud.top

[T24] Swift：闭包
来源：http://jqs.wangshuangyany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lrt.shanyushiyangtech.top

[T25] Swift：结构体
来源：http://urf.uphjek.com

struct P { var x: Int }
来源：http://dxl.quarkkingdee.top

[T26] Swift：类与重写
来源：http://bvl.havefunace.top

class A: Base { override func f() {} }
来源：http://jub.svipenyu.cn

[T27] Swift：错误处理
来源：http://haj.hesvh.cn

do { try f() } catch { print(error) }
来源：http://ape.hysaishi.cn

[T28] Swift：枚举
来源：http://rgx.ivvv.top

enum Color { case red, green }
来源：http://ufw.hcnkem.com

[T29] Swift：guard 提前返回
来源：http://nll.vehdjk.com

guard let x = opt else { return }
来源：http://zkz.wangshuangyany.cn

[T30] Swift：协议
来源：http://vuy.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://ntt.zhaomingkeji.xyz

[T31] Lua：Hello World
来源：http://bkn.hongshengwenyu.top

print("Hello")
来源：http://ber.daria6918.cn

[T32] Lua：局部变量
来源：http://fas.hfpthk.cn

local a = 1
来源：http://aag.gotoacloud.top

[T33] Lua：表（数组）
来源：http://lap.ctjpmb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ily.bbcook.cn

[T34] Lua：遍历表
来源：http://jsd.andypj.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://tjd.aibaodan.cn

[T35] Lua：字典表
来源：http://fht.yueranfly.top

local d = { a = 1 };  d.b = 2
来源：http://bte.gotoacloud.top

[T36] Lua：函数
来源：http://pck.cqqwz.cn

function add(a, b) return a + b end
来源：http://spt.daria6918.cn

[T37] Lua：字符串拼接
来源：http://wpi.tanke756.top

"a" .. "b"
来源：http://bxr.fktsv.cn

[T38] Lua：条件
来源：http://ziq.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://yid.svipenyu.cn

[T39] Lua：模式匹配
来源：http://nqr.hesvh.cn

string.find(s, "%d+")
来源：http://lie.xylfe.cn

[T40] Lua：元表
来源：http://hly.yuxming.cn

setmetatable({}, { __index = base })
来源：http://vhg.0kj1m.cn

[T41] Perl：Hello World
来源：http://uys.aizwys.cn

print "Hello\n";
来源：http://bbf.aizwys.cn

[T42] Perl：变量类型
来源：http://sfy.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kqa.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://wde.feifeiyinyue.top

"值: $a"
来源：http://hvj.meibo888.top

[T44] Perl：条件
来源：http://xat.tianlin.xyz

if ($a > 0) { print "正"; }
来源：http://drf.nanxuanxn.top

[T45] Perl：数组遍历
来源：http://shv.jinyuanbaomall.cn

for my $x (@arr) { print $x; }
来源：http://hzk.zdqjudy.top

[T46] Perl：哈希操作
来源：http://xvr.zhongyouzk.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vzw.hcnkem.com

[T47] Perl：正则捕获
来源：http://fkb.tarul.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ckk.daria6918.cn

[T48] Perl：正则替换
来源：http://ple.yonumen.top

$s =~ s/old/new/g;
来源：http://qfo.dianchejie.cn

[T49] Perl：函数
来源：http://yky.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://puw.gogol.net.cn

[T50] Perl：逐行读文件
来源：http://adj.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jox.guannengcc.top

while (my $line = <$fh>) { print $line; }
来源：http://jtz.9152youxi.cn

[T51] Scala：Hello World
来源：http://wlr.tanke756.top

println("Hello")
来源：http://ljx.hcnkem.com

[T52] Scala：变量
来源：http://frc.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://wvb.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://tej.tarul.cn

s"值: $b"
来源：http://gbl.c1oappe.top

[T54] Scala：集合映射
来源：http://mux.hfpthk.cn

List(1, 2, 3).map(_ * 2)
来源：http://vfv.jinqigufen.top

[T55] Scala：集合过滤
来源：http://khd.zhengqikj.top

List(1, 2, 3).filter(_ > 1)
来源：http://nfd.shuidangran.top

[T56] Scala：样例类
来源：http://dii.gotoacloud.top

case class User(name: String, age: Int)
来源：http://vad.hywenlv.cn

[T57] Scala：模式匹配
来源：http://fwp.mhx1999.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://tnc.kuanghao11.cn

[T58] Scala：函数定义
来源：http://ptk.52xcode.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yln.nwbrower.top

[T59] Scala：循环
来源：http://pbb.yueranfly.top

for (i <- 1 to 10) println(i)
来源：http://rcv.zhixingplan.top

[T60] Scala：折叠
来源：http://jmg.cucudq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pxv.epnwcf.com

================================================================================
来源：http://qgd.xylfe.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rge.mhx1999.top

================================================================================
来源：http://coy.cqqwz.cn

[U01] Py：创建虚拟环境
来源：http://egs.hywenlv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nhi.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://kbm.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hqn.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://wyy.shanyushiyangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lif.tian-w.cn

[U04] Py：变量调试打印
来源：http://pxg.cheryme.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kcp.fzhhl.top

[U05] Py：列表去重且保序
来源：http://kuo.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://usz.zdbjq.cn

[U06] Py：合并两个字典
来源：http://mxd.zhijiandao.cn

{**a, **b}
来源：http://jgp.jqgfzy.top

[U07] Py：反转字典键值
来源：http://zsc.gaohongyu789.top

{v: k for k, v in d.items()}
来源：http://uhd.tianlin.xyz

[U08] Py：展平二维列表
来源：http://lvq.jqgufenzy.top

[y for x in nested for y in x]
来源：http://pqc.52xcode.cn

[U09] Py：字典取最大值的键
来源：http://tyz.c1oappe.top

max(d, key=d.get)
来源：http://fxw.hnxiangtu.top

[U10] Py：按值排序字典
来源：http://kxq.fanxiaobao.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rnq.hfpthk.cn

[U11] Py：生成器表达式
来源：http://gjv.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://geq.yangfankeji.com

[U12] Py：取出现最多的 3 个元素
来源：http://tcv.iojbl.cn

Counter(arr).most_common(3)
来源：http://dag.fzhhl.top

[U13] Py：固定长度队列
来源：http://exa.yj202588.top

deque(maxlen=10)
来源：http://kqb.xingfuxueyuan.xyz

[U14] Py：分组收集到列表
来源：http://thb.hcnkem.com

defaultdict(list)
来源：http://wpb.jiagoushi.top

[U15] Py：高精度计时
来源：http://sxz.yj20258888.top

t = time.perf_counter()
来源：http://qxh.aizwys.cn

[U16] Py：命令行参数解析
来源：http://uiw.jinqigufen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sjh.iojbl.cn

[U17] Py：初始化日志
来源：http://ggb.shanyushiyangtech.top

logging.basicConfig(level=logging.INFO)
来源：http://kvd.jqgfzy.top

[U18] Py：预编译正则
来源：http://mgw.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://ghp.shuidangran.top

[U19] Py：正则替换带回调
来源：http://laf.nwbrower.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ujk.kuanghao11.cn

[U20] Py：缓存函数结果
来源：http://zlw.chenjidiqi.icu

@functools.lru_cache(maxsize=None)
来源：http://mir.ywan-chungtsiang.top

[U21] Py：自定义上下文管理器
来源：http://kto.jinqigufen.top

@contextlib.contextmanager
来源：http://dqh.jianghu66.top

[U22] Py：矩阵转置
来源：http://dcm.jiagoushi.top

list(zip(*m))
来源：http://pwo.52xcode.cn

[U23] Py：分块读取大文件
来源：http://igj.hcnkem.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pnj.hcnkem.com

[U24] Py：路径操作
来源：http://nmp.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hhr.ivvv.top

[U25] Py：CSV 按字典读
来源：http://uad.yueranfly.top

csv.DictReader(f)
来源：http://rfj.hnqzz.top

[U26] Py：并发下载
来源：http://fxa.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vxa.snrcjt.cn

[U27] Py：异步 HTTP
来源：http://mcb.yonumen.top

aiohttp.ClientSession() 配合 async with
来源：http://pcg.birdmap.top

[U28] Py：类型别名
来源：http://oab.shzxlz.cn

UserId = int
来源：http://okw.cashguo.top

[U29] Py：属性校验
来源：http://mha.yangfankeji.com

@property 与 @x.setter 配合
来源：http://fxk.ctjpmb.com

[U30] Py：数据类
来源：http://rjz.meibo888.top

@dataclass(slots=True)
来源：http://bdg.cqqwz.cn

[U31] Py：单测
来源：http://kob.nanxinkj.top

python -m pytest -q
来源：http://nnz.cdnleiting.top

[U32] Py：代码格式化
来源：http://lqj.pycfn.com

ruff format . && ruff check --fix .
来源：http://szg.c1oappe.top

[U33] Py：打包发布
来源：http://aiw.hysaishi.cn

python -m build  （依赖 pyproject.toml）
来源：http://vgp.jinyuanbaomall.cn

[U34] Py：判断编码
来源：http://pxa.jyoumei.cn

chardet.detect(raw)
来源：http://rck.zhijiandao.cn

[U35] Py：发送邮件
来源：http://yam.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bbc.daxiang520.top

[U36] Py：定时任务
来源：http://lkq.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://sly.sysykeji.top

[U37] Py：读写 Excel
来源：http://ybl.daria6918.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sek.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://zrf.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://sos.ydzc1.top

[U39] Py：判断是否在交互环境
来源：http://zoo.chenlongwang.top

sys.stdout.isatty()
来源：http://uts.ywan-chungtsiang.top

[U40] Py：打印到标准错误
来源：http://dtd.sufxvd.cn

print("err", file=sys.stderr)
来源：http://ogu.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://fwo.cashguo.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cvh.nanxinkj.top

[U42] PHP：PSR-4 自动加载
来源：http://iqr.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dyb.wangdashe.top

[U43] PHP：声明命名空间
来源：http://oxp.havefunace.top

namespace App\Http;
来源：http://pck.316326.xyz

[U44] PHP：开启严格类型
来源：http://jhh.fehbvm.com

declare(strict_types=1);
来源：http://xju.sweek.top

[U45] PHP：类型声明与返回类型
来源：http://iwm.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lsi.jinyuanbaomall.cn

[U46] PHP：可空类型
来源：http://czw.vqdsnc.cn

?string $name = null
来源：http://ezq.sxryk.cn

[U47] PHP：联合类型
来源：http://xot.sxryk.cn

int|string $id
来源：http://tcc.52xcode.cn

[U48] PHP：纯枚举
来源：http://saj.zhoulong.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ono.tianlin.xyz

[U49] PHP：只读属性
来源：http://vud.hnxiangtu.top

public readonly string $name
来源：http://zxw.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://kym.hammf.cn

public function __construct(private int $id) {}
来源：http://evu.316326.xyz

[U51] PHP：数组解构
来源：http://ewg.zhijiandao.cn

[$a, $b] = $arr;
来源：http://vsy.nanxinkj.top

[U52] PHP：箭头函数
来源：http://bwl.epnwcf.com

$double = fn($x) => $x * 2;
来源：http://ahf.hfpthk.cn

[U53] PHP：空合并运算符
来源：http://hkg.gotoacloud.top

$v = $a ?? $b ?? "default";
来源：http://vaj.pengpengdd.cyou

[U54] PHP：空安全调用
来源：http://txs.epnwcf.com

$obj?->method()
来源：http://xoa.52xcode.cn

[U55] PHP：match 表达式
来源：http://bzc.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xgk.gzhubu.top

[U56] PHP：命名参数
来源：http://xma.shanyushiyangkeji.top

f(a: 1, b: 2)
来源：http://ifz.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://omu.fktsv.cn

"值: {$a}"
来源：http://csq.zycfv.cn

[U58] PHP：数组三件套
来源：http://yha.316326.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pqw.sysykeji.top

[U59] PHP：自定义排序
来源：http://wcl.wangshuangyany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vqi.dianchejie.cn

[U60] PHP：JSON 编解码
来源：http://rpk.hnxiangtu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ofq.uphjek.com

[U61] PHP：正则
来源：http://tir.chenlongwang.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vhi.hnxiangtu.top

[U62] PHP：日期对象
来源：http://ogh.jqgfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://msj.daria6918.cn

[U63] PHP：文件读写
来源：http://bbd.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://whd.bbcook.cn

[U64] PHP：目录遍历
来源：http://qkb.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://lkp.hnxiangtu.top

[U65] PHP：会话
来源：http://sxe.epnwcf.com

session_start();  $_SESSION["uid"] = 1;
来源：http://hja.guowangkeji.top

[U66] PHP：设置 Cookie
来源：http://mug.hywenlv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://clq.hysaishi.cn

[U67] PHP：处理文件上传
来源：http://umv.gaohongyu789.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ugj.hcnkem.com

[U68] PHP：PDO 连接
来源：http://shf.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vqa.jqgfzy.top

[U69] PHP：PDO 预处理
来源：http://oex.hesvh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yqy.yongpay.top

[U70] PHP：PDO 事务
来源：http://xxs.fengsongda.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hih.jyoumei.cn

[U71] PHP：抛出异常
来源：http://klt.yj20258.top

throw new RuntimeException("失败", 500);
来源：http://yfe.smart0.xyz

[U72] PHP：写错误日志
来源：http://mgd.xziqi.cn

error_log("失败: " . $e->getMessage());
来源：http://wiv.cheryme.top

[U73] PHP：读取 ini 配置
来源：http://enm.nanxinkj.top

parse_ini_file("config.ini", true)
来源：http://kag.quarkkingdee.top

[U74] PHP：读取环境变量
来源：http://jai.yj20258888.top

getenv("APP_ENV") ?: "production"
来源：http://bur.haohaochexian.top

[U75] PHP：依赖注入
来源：http://woj.gogol.net.cn

composer require psr/container
来源：http://jmf.316326.xyz

[U76] PHP：简单路由
来源：http://zot.cheryme.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cpy.yanxiufei.cn

[U77] PHP：模板渲染
来源：http://nph.dashuyun.cn

composer require twig/twig
来源：http://glu.sufxvd.cn

[U78] PHP：单元测试
来源：http://gty.zhixingplan.top

composer require --dev phpunit/phpunit
来源：http://lhr.fktsv.cn

[U79] PHP：静态分析
来源：http://oyj.chenjidiqi.icu

composer require --dev phpstan/phpstan
来源：http://ghi.sjlbkw.cn

[U80] PHP：代码规范修复
来源：http://ubq.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hzo.wangdashe.top

[U81] JS：初始化项目
来源：http://jkg.andypj.xyz

npm init -y;  npm i express
来源：http://lor.zhongyouzk.top

[U82] JS：package.json 脚本
来源：http://sev.yangfankeji.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vtw.yuxming.cn

[U83] JS：ES Module 导入导出
来源：http://dwj.gotoacloud.top

export const a = 1;  import { a } from "./m.js";
来源：http://evs.jqgufenzy.top

[U84] JS：CommonJS 写法
来源：http://eud.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://jzu.ctjpmb.com


<!-- 参考信息 -->