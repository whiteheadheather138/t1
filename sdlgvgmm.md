代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://tna.jinqigufen.top

[S59] C++：静态断言
来源：http://rhk.bbcook.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ijj.ybcxt.top

[S60] C++：遍历并删除元素
来源：http://dhi.hesvh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vfz.ctjpmb.com

================================================================================
来源：http://wne.chenlongwang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://she.xinyue.icu

================================================================================
来源：http://wyc.xziqi.cn

[T01] Kotlin：Hello World
来源：http://qeh.gotoacloud.top

println("Hello")
来源：http://bvk.dashuyun.cn

[T02] Kotlin：变量
来源：http://pqi.sysykeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kzo.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://gph.jqgufenzy.top

"值: $b"
来源：http://stk.vqdsnc.cn

[T04] Kotlin：空安全
来源：http://hwu.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://vlx.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://jfw.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mqr.hammf.cn

[T06] Kotlin：集合映射
来源：http://pjs.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yee.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://och.shanyushiyangtech.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uwh.chenjidiqi.icu

[T08] Kotlin：数据类
来源：http://ebc.hnqzz.top

data class User(val name: String, val age: Int)
来源：http://qap.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://smu.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://crh.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://afg.fehbvm.com

fun greet(name: String = "World") = "Hi $name"
来源：http://wee.ppjwa.cn

[T11] Kotlin：协程
来源：http://mws.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ism.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://isc.jinghuilouyu.cn

val (a, b) = Pair(1, 2)
来源：http://wzt.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://xui.jqgufenzy.top

val m = mapOf("a" to 1)
来源：http://nvi.ivvv.top

[T14] Kotlin：循环
来源：http://ans.ywan-chungtsiang.top

for (i in 1..10) println(i)
来源：http://vca.iojbl.cn

[T15] Kotlin：接口
来源：http://pvn.yfazqb.com

interface Shape { fun area(): Double }
来源：http://jld.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://mkh.c1oappe.top

print("Hello")
来源：http://gpc.iojbl.cn

[T17] Swift：变量与常量
来源：http://vju.ctjpmb.com

var a = 1;  let b = 2
来源：http://cnw.sxryk.cn

[T18] Swift：字符串插值
来源：http://xbp.aibaodan.cn

"值: \(b)"
来源：http://eve.fanxiaobao.xyz

[T19] Swift：可选绑定
来源：http://fhk.daxiang520.top

if let n = opt { print(n) }
来源：http://zxr.yuxming.cn

[T20] Swift：数组操作
来源：http://cqr.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://aye.epnwcf.com

[T21] Swift：遍历
来源：http://fao.daxiang520.top

for x in a { print(x) }
来源：http://bkd.pycfn.com

[T22] Swift：字典
来源：http://mlt.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://yio.bjfxy.top

[T23] Swift：函数
来源：http://gri.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ipk.hnqzz.top

[T24] Swift：闭包
来源：http://jig.sxryk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://itu.shuidangran.top

[T25] Swift：结构体
来源：http://zod.tian-w.cn

struct P { var x: Int }
来源：http://bkd.xinyue.icu

[T26] Swift：类与重写
来源：http://hdb.xuanzx.com

class A: Base { override func f() {} }
来源：http://del.yj202588.top

[T27] Swift：错误处理
来源：http://afg.yuanzhike.top

do { try f() } catch { print(error) }
来源：http://gjo.fanxiaobao.xyz

[T28] Swift：枚举
来源：http://spv.vqdsnc.cn

enum Color { case red, green }
来源：http://scg.cheryme.top

[T29] Swift：guard 提前返回
来源：http://xic.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://zpx.kuanghao11.cn

[T30] Swift：协议
来源：http://goa.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://aeq.0kj1m.cn

[T31] Lua：Hello World
来源：http://nig.haohaochexian.top

print("Hello")
来源：http://daz.ppjwa.cn

[T32] Lua：局部变量
来源：http://qek.fehbvm.com

local a = 1
来源：http://eld.hnxiangtu.top

[T33] Lua：表（数组）
来源：http://bxn.zdqjudy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dfx.pycfn.com

[T34] Lua：遍历表
来源：http://csf.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ety.ivvv.top

[T35] Lua：字典表
来源：http://dnn.xinyue.icu

local d = { a = 1 };  d.b = 2
来源：http://hwr.yuxming.cn

[T36] Lua：函数
来源：http://cmc.sufxvd.cn

function add(a, b) return a + b end
来源：http://ddz.cucudq.cn

[T37] Lua：字符串拼接
来源：http://bfm.bjfxy.top

"a" .. "b"
来源：http://pwp.vehdjk.com

[T38] Lua：条件
来源：http://kvf.shzxlz.cn

if x > 0 then print("正") end
来源：http://pkq.meibo888.top

[T39] Lua：模式匹配
来源：http://xyd.nanxuanxn.top

string.find(s, "%d+")
来源：http://pdb.yj202588.top

[T40] Lua：元表
来源：http://rim.shangyingyoupin.top

setmetatable({}, { __index = base })
来源：http://dpl.yj20258.top

[T41] Perl：Hello World
来源：http://kmz.nwbrower.top

print "Hello\n";
来源：http://zmo.yj20258.top

[T42] Perl：变量类型
来源：http://zwy.smart0.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bkz.ydzc1.top

[T43] Perl：字符串插值
来源：http://cpq.kuanghao11.cn

"值: $a"
来源：http://hcw.andypj.xyz

[T44] Perl：条件
来源：http://ntk.gotoacloud.top

if ($a > 0) { print "正"; }
来源：http://ibx.yj20258888.top

[T45] Perl：数组遍历
来源：http://csw.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://rst.aibaodan.cn

[T46] Perl：哈希操作
来源：http://buq.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iqr.epnwcf.com

[T47] Perl：正则捕获
来源：http://wzl.xuanzx.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://qre.zhongyouzk.top

[T48] Perl：正则替换
来源：http://jbt.shuidangran.top

$s =~ s/old/new/g;
来源：http://dkf.316326.xyz

[T49] Perl：函数
来源：http://bjn.dashuyun.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ynu.dianchejie.cn

[T50] Perl：逐行读文件
来源：http://uqr.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://emz.ybcxt.top

while (my $line = <$fh>) { print $line; }
来源：http://qpd.fzhhl.top

[T51] Scala：Hello World
来源：http://nte.wangshuangyany.cn

println("Hello")
来源：http://vrb.hongshengwenyu.top

[T52] Scala：变量
来源：http://kqe.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://yex.fengsongda.top

[T53] Scala：字符串插值
来源：http://irm.hnqzz.top

s"值: $b"
来源：http://tcs.sweek.top

[T54] Scala：集合映射
来源：http://iga.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://fey.jinyuanbaomall.cn

[T55] Scala：集合过滤
来源：http://mbi.guannengcc.top

List(1, 2, 3).filter(_ > 1)
来源：http://ans.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://omf.svipenyu.cn

case class User(name: String, age: Int)
来源：http://deh.xingfuxueyuan.xyz

[T57] Scala：模式匹配
来源：http://lkp.cdnleiting.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lit.ydzc1.top

[T58] Scala：函数定义
来源：http://xju.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://myu.nanxuanxn.top

[T59] Scala：循环
来源：http://sjc.yongpay.top

for (i <- 1 to 10) println(i)
来源：http://mlx.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://bzu.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yfk.jinqigufen.top

================================================================================
来源：http://suh.dashuyun.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://asv.yangfankeji.com

================================================================================
来源：http://kto.jinqigfzy.top

[U01] Py：创建虚拟环境
来源：http://xrj.0kj1m.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sxz.9152youxi.cn

[U02] Py：导出 / 安装依赖
来源：http://agk.aizwys.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://obk.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://hvr.dashuyun.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iqj.hnxiangtu.top

[U04] Py：变量调试打印
来源：http://rtl.yj202588.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pda.shzxlz.cn

[U05] Py：列表去重且保序
来源：http://oig.jinqigufen.top

list(dict.fromkeys(arr))
来源：http://plj.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://osv.meibo888.top

{**a, **b}
来源：http://prc.guannengcc.top

[U07] Py：反转字典键值
来源：http://isz.bjfxy.top

{v: k for k, v in d.items()}
来源：http://unc.vehdjk.com

[U08] Py：展平二维列表
来源：http://yne.jqgfzy.top

[y for x in nested for y in x]
来源：http://oqf.fzhhl.top

[U09] Py：字典取最大值的键
来源：http://lku.ydzc1.top

max(d, key=d.get)
来源：http://qzx.haohaochexian.top

[U10] Py：按值排序字典
来源：http://mel.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rph.bjfxy.top

[U11] Py：生成器表达式
来源：http://ail.nanxinkj.top

(x * 2 for x in arr)
来源：http://pat.jinqigfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://qsk.zdbjq.cn

Counter(arr).most_common(3)
来源：http://juu.ybcxt.top

[U13] Py：固定长度队列
来源：http://nih.jinghuilouyu.cn

deque(maxlen=10)
来源：http://ykn.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://zxg.havefunace.top

defaultdict(list)
来源：http://vuu.yj20258888.top

[U15] Py：高精度计时
来源：http://zll.jianghu66.top

t = time.perf_counter()
来源：http://blv.tianlin.xyz

[U16] Py：命令行参数解析
来源：http://duv.guowangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ezj.chenzaomai.com

[U17] Py：初始化日志
来源：http://ydp.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://bdy.nanxuanxn.top

[U18] Py：预编译正则
来源：http://utk.gotoacloud.top

pat = re.compile(r"\d+")
来源：http://pov.cashguo.top

[U19] Py：正则替换带回调
来源：http://ule.dianchejie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tru.dianchejie.cn

[U20] Py：缓存函数结果
来源：http://kyf.tarul.cn

@functools.lru_cache(maxsize=None)
来源：http://gpt.cucudq.cn

[U21] Py：自定义上下文管理器
来源：http://jen.daxiang520.top

@contextlib.contextmanager
来源：http://ycd.bjfxy.top

[U22] Py：矩阵转置
来源：http://xpb.tarul.cn

list(zip(*m))
来源：http://mlg.bjfxy.top

[U23] Py：分块读取大文件
来源：http://sxv.shanyushiyangtech.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cli.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://imm.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qqe.xziqi.cn

[U25] Py：CSV 按字典读
来源：http://hfi.daxiang520.top

csv.DictReader(f)
来源：http://frw.hammf.cn

[U26] Py：并发下载
来源：http://xwb.snrcjt.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jed.cucudq.cn

[U27] Py：异步 HTTP
来源：http://swg.guowangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://pou.meibo888.top

[U28] Py：类型别名
来源：http://nzn.shzxlz.cn

UserId = int
来源：http://vdy.316326.xyz

[U29] Py：属性校验
来源：http://bor.meibo888.top

@property 与 @x.setter 配合
来源：http://dju.uphjek.com

[U30] Py：数据类
来源：http://yay.zhoulong.xyz

@dataclass(slots=True)
来源：http://zit.wangdashe.top

[U31] Py：单测
来源：http://rkn.yonumen.top

python -m pytest -q
来源：http://eoy.iojbl.cn

[U32] Py：代码格式化
来源：http://vuo.shangyingyoupin.top

ruff format . && ruff check --fix .
来源：http://wpc.ywan-chungtsiang.top

[U33] Py：打包发布
来源：http://xbk.fehbvm.com

python -m build  （依赖 pyproject.toml）
来源：http://hbj.redwolf501.top

[U34] Py：判断编码
来源：http://mpj.tian-w.cn

chardet.detect(raw)
来源：http://nqs.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://qzg.shuidangran.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ard.yangfankeji.com

[U36] Py：定时任务
来源：http://res.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://azn.iojbl.cn

[U37] Py：读写 Excel
来源：http://mkr.xuanzx.com

pandas.read_excel / DataFrame.to_excel
来源：http://xmu.dianchejie.cn

[U38] Py：获取脚本所在目录
来源：http://ygy.jqgufenzy.top

Path(__file__).resolve().parent
来源：http://zoq.wangdashe.top

[U39] Py：判断是否在交互环境
来源：http://qbq.cdnleiting.top

sys.stdout.isatty()
来源：http://xpf.jqgufenzy.top

[U40] Py：打印到标准错误
来源：http://kyx.zhijiandao.cn

print("err", file=sys.stderr)
来源：http://dns.guannengcc.top

[U41] PHP：初始化 Composer 项目
来源：http://dgx.sweek.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mgx.svipenyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://cgp.pycfn.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tqd.ehwqpu.com

[U43] PHP：声明命名空间
来源：http://mhu.havefunace.top

namespace App\Http;
来源：http://ngi.yueranfly.top

[U44] PHP：开启严格类型
来源：http://wgh.yanxiufei.cn

declare(strict_types=1);
来源：http://xft.sweek.top

[U45] PHP：类型声明与返回类型
来源：http://jky.zhijiandao.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pah.hfpthk.cn

[U46] PHP：可空类型
来源：http://vat.gogol.net.cn

?string $name = null
来源：http://fqq.nanxinkj.top

[U47] PHP：联合类型
来源：http://ymd.hnxiangtu.top

int|string $id
来源：http://dah.wangdashe.top

[U48] PHP：纯枚举
来源：http://bzo.zycfv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sjs.iojbl.cn

[U49] PHP：只读属性
来源：http://nma.pengpengdd.cyou

public readonly string $name
来源：http://ugp.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://uiv.xylfe.cn

public function __construct(private int $id) {}
来源：http://ddo.sufxvd.cn

[U51] PHP：数组解构
来源：http://xud.guannengcc.top

[$a, $b] = $arr;
来源：http://jng.fengsongda.top

[U52] PHP：箭头函数
来源：http://prn.0kj1m.cn

$double = fn($x) => $x * 2;
来源：http://ylb.ivvv.top

[U53] PHP：空合并运算符
来源：http://gbj.daxiang520.top

$v = $a ?? $b ?? "default";
来源：http://mms.birdmap.top

[U54] PHP：空安全调用
来源：http://bsg.jinghuilouyu.cn

$obj?->method()
来源：http://noh.zhijiandao.cn

[U55] PHP：match 表达式
来源：http://kyv.yongpay.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hdn.jinqigfzy.top

[U56] PHP：命名参数
来源：http://thi.vqdsnc.cn

f(a: 1, b: 2)
来源：http://src.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://hzg.jianghu66.top

"值: {$a}"
来源：http://cjv.chenjidiqi.icu

[U58] PHP：数组三件套
来源：http://xdj.ppjwa.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xjf.zhixingplan.top

[U59] PHP：自定义排序
来源：http://zrv.xylfe.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pra.ydzc1.top

[U60] PHP：JSON 编解码
来源：http://kps.jyoumei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://txu.hfpthk.cn

[U61] PHP：正则
来源：http://otn.xingfuxueyuan.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blv.jyoumei.cn

[U62] PHP：日期对象
来源：http://dnx.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ugi.gzhubu.top

[U63] PHP：文件读写
来源：http://exc.nwbrower.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://otf.daxiang520.top

[U64] PHP：目录遍历
来源：http://bfs.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://jic.iojbl.cn

[U65] PHP：会话
来源：http://jmj.gaohongyu789.top

session_start();  $_SESSION["uid"] = 1;
来源：http://eep.c1oappe.top

[U66] PHP：设置 Cookie
来源：http://klt.nwbrower.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xpt.snrcjt.cn

[U67] PHP：处理文件上传
来源：http://vil.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gcg.guowangkeji.top

[U68] PHP：PDO 连接
来源：http://rdr.fzhhl.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kxx.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://obo.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://epz.tanke756.top

[U70] PHP：PDO 事务
来源：http://drw.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xtm.hcnkem.com

[U71] PHP：抛出异常
来源：http://cki.sjlbkw.cn

throw new RuntimeException("失败", 500);
来源：http://urz.haohaochexian.top

[U72] PHP：写错误日志
来源：http://pmy.gzhubu.top

error_log("失败: " . $e->getMessage());
来源：http://buq.redwolf501.top

[U73] PHP：读取 ini 配置
来源：http://hte.wangdashe.top

parse_ini_file("config.ini", true)
来源：http://rwi.fengsongda.top

[U74] PHP：读取环境变量
来源：http://oub.yonumen.top

getenv("APP_ENV") ?: "production"
来源：http://hwi.wangdashe.top

[U75] PHP：依赖注入
来源：http://paj.wangdashe.top

composer require psr/container
来源：http://tsm.zhoulong.xyz

[U76] PHP：简单路由
来源：http://hpd.cashguo.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://spc.birdmap.top

[U77] PHP：模板渲染
来源：http://hfu.chenzaomai.com

composer require twig/twig
来源：http://sjk.quarkkingdee.top

[U78] PHP：单元测试
来源：http://kzc.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://naf.zdqjudy.top

[U79] PHP：静态分析
来源：http://mow.hywenlv.cn

composer require --dev phpstan/phpstan
来源：http://xei.xylfe.cn

[U80] PHP：代码规范修复
来源：http://pwy.gotoacloud.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rwk.ydjk.org.cn

[U81] JS：初始化项目
来源：http://qqu.hesvh.cn

npm init -y;  npm i express
来源：http://ivl.yuanzhike.top

[U82] JS：package.json 脚本
来源：http://eak.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tda.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://chm.cdnleiting.top

export const a = 1;  import { a } from "./m.js";
来源：http://fel.smart0.xyz

[U84] JS：CommonJS 写法
来源：http://orb.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://swz.nanxuanxn.top


<!-- 参考信息 -->