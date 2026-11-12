代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://veo.quarkkingdee.top

[S59] C++：静态断言
来源：http://rij.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wnz.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://lgj.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mtx.yuanzhike.top

================================================================================
来源：http://ihy.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dwo.tian-w.cn

================================================================================
来源：http://jfm.jqgfzy.top

[T01] Kotlin：Hello World
来源：http://jyp.52xcode.cn

println("Hello")
来源：http://bza.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://ozt.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lke.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://ctz.bbcook.cn

"值: $b"
来源：http://hkw.quarkkingdee.top

[T04] Kotlin：空安全
来源：http://xlf.nwbrower.top

val n: String? = null;  n?.length
来源：http://loi.cashguo.top

[T05] Kotlin：when 表达式
来源：http://osz.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gif.shuidangran.top

[T06] Kotlin：集合映射
来源：http://zuc.ybcxt.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lht.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://mtx.yuxming.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bcm.wangshuangyany.cn

[T08] Kotlin：数据类
来源：http://pdd.tarul.cn

data class User(val name: String, val age: Int)
来源：http://qlu.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://htd.shzxlz.cn

fun String.exclaim() = this + "!"
来源：http://xtv.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://trc.hfpthk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ryq.sysykeji.top

[T11] Kotlin：协程
来源：http://gzz.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nlu.hongshengwenyu.top

[T12] Kotlin：解构声明
来源：http://qwk.snrcjt.cn

val (a, b) = Pair(1, 2)
来源：http://los.jinghuilouyu.cn

[T13] Kotlin：只读 Map
来源：http://lit.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://ilm.xylfe.cn

[T14] Kotlin：循环
来源：http://njh.tianlin.xyz

for (i in 1..10) println(i)
来源：http://lmw.uphjek.com

[T15] Kotlin：接口
来源：http://gzk.yonumen.top

interface Shape { fun area(): Double }
来源：http://urn.ydjk.org.cn

[T16] Swift：Hello World
来源：http://qeb.chenjidiqi.icu

print("Hello")
来源：http://ptt.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://nce.jinqigufen.top

var a = 1;  let b = 2
来源：http://itt.xinyue.icu

[T18] Swift：字符串插值
来源：http://way.haohaochexian.top

"值: \(b)"
来源：http://xsv.hywenlv.cn

[T19] Swift：可选绑定
来源：http://qjm.hammf.cn

if let n = opt { print(n) }
来源：http://zhj.wangshuangyany.cn

[T20] Swift：数组操作
来源：http://dbi.jyoumei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://khp.tian-w.cn

[T21] Swift：遍历
来源：http://tcu.sufxvd.cn

for x in a { print(x) }
来源：http://umd.fehbvm.com

[T22] Swift：字典
来源：http://yzq.aibaodan.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kdx.sweek.top

[T23] Swift：函数
来源：http://ele.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uuw.daxiang520.top

[T24] Swift：闭包
来源：http://myv.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cno.ivvv.top

[T25] Swift：结构体
来源：http://bxa.guannengcc.top

struct P { var x: Int }
来源：http://wdh.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://oed.shanyushiyangkeji.top

class A: Base { override func f() {} }
来源：http://ewu.xinyue.icu

[T27] Swift：错误处理
来源：http://hpc.andypj.xyz

do { try f() } catch { print(error) }
来源：http://ytd.hammf.cn

[T28] Swift：枚举
来源：http://bxc.xylfe.cn

enum Color { case red, green }
来源：http://guc.andypj.xyz

[T29] Swift：guard 提前返回
来源：http://vmb.0kj1m.cn

guard let x = opt else { return }
来源：http://sst.shanyushiyangkeji.top

[T30] Swift：协议
来源：http://mmd.hongshengwenyu.top

protocol Shape { func area() -> Double }
来源：http://wyz.nanxinkj.top

[T31] Lua：Hello World
来源：http://bsz.hammf.cn

print("Hello")
来源：http://nhq.xingfuxueyuan.xyz

[T32] Lua：局部变量
来源：http://thp.ybcxt.top

local a = 1
来源：http://rmo.xylfe.cn

[T33] Lua：表（数组）
来源：http://kea.jinghuilouyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dcv.xinyue.icu

[T34] Lua：遍历表
来源：http://qsz.hywenlv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://szl.daria6918.cn

[T35] Lua：字典表
来源：http://yst.zhengqikj.top

local d = { a = 1 };  d.b = 2
来源：http://zjm.zhixingplan.top

[T36] Lua：函数
来源：http://set.xylfe.cn

function add(a, b) return a + b end
来源：http://gbm.yuxming.cn

[T37] Lua：字符串拼接
来源：http://rre.fanxiaobao.xyz

"a" .. "b"
来源：http://vfq.dianchejie.cn

[T38] Lua：条件
来源：http://low.tianlin.xyz

if x > 0 then print("正") end
来源：http://nlv.andypj.xyz

[T39] Lua：模式匹配
来源：http://mxq.hnxiangtu.top

string.find(s, "%d+")
来源：http://ytk.sjlbkw.cn

[T40] Lua：元表
来源：http://xwj.yueranfly.top

setmetatable({}, { __index = base })
来源：http://xdu.jianghu66.top

[T41] Perl：Hello World
来源：http://mqh.tarul.cn

print "Hello\n";
来源：http://ofb.feifeiyinyue.top

[T42] Perl：变量类型
来源：http://nbg.zhongyouzk.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iej.yj20258.top

[T43] Perl：字符串插值
来源：http://yni.0kj1m.cn

"值: $a"
来源：http://vuv.yfazqb.com

[T44] Perl：条件
来源：http://gsa.zhoulong.xyz

if ($a > 0) { print "正"; }
来源：http://tng.aizwys.cn

[T45] Perl：数组遍历
来源：http://xkz.cdnleiting.top

for my $x (@arr) { print $x; }
来源：http://zjb.ehwqpu.com

[T46] Perl：哈希操作
来源：http://ivw.yvedp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ewt.ctjpmb.com

[T47] Perl：正则捕获
来源：http://wbh.zhengqikj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://flt.yj202588.top

[T48] Perl：正则替换
来源：http://fkg.smart0.xyz

$s =~ s/old/new/g;
来源：http://rgx.jyoumei.cn

[T49] Perl：函数
来源：http://abx.zdbjq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rzy.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://upp.hfpthk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xbe.jinqigfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://sen.gogol.net.cn

[T51] Scala：Hello World
来源：http://cke.shuidangran.top

println("Hello")
来源：http://bud.vehdjk.com

[T52] Scala：变量
来源：http://ryj.tarul.cn

val a = 1;  var b = 2
来源：http://uqx.xinyue.icu

[T53] Scala：字符串插值
来源：http://lnv.zhongyouzk.top

s"值: $b"
来源：http://dea.hesvh.cn

[T54] Scala：集合映射
来源：http://imq.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://haz.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://lak.shanyushiyangtech.top

List(1, 2, 3).filter(_ > 1)
来源：http://qld.gogol.net.cn

[T56] Scala：样例类
来源：http://bpt.yj202588.top

case class User(name: String, age: Int)
来源：http://aiq.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://dlh.shangyingyoupin.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hjx.jinyuanbaomall.cn

[T58] Scala：函数定义
来源：http://teq.ybcxt.top

def add(a: Int, b: Int): Int = a + b
来源：http://jzi.fanxiaobao.xyz

[T59] Scala：循环
来源：http://oql.daria6918.cn

for (i <- 1 to 10) println(i)
来源：http://nlj.zhixingplan.top

[T60] Scala：折叠
来源：http://pds.jyoumei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nuz.jqgfzy.top

================================================================================
来源：http://rjs.yuanzhike.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iqb.jqgfzy.top

================================================================================
来源：http://gwq.cheryme.top

[U01] Py：创建虚拟环境
来源：http://yfk.yj20258.top

python -m venv .venv && source .venv/bin/activate
来源：http://pnk.dashuyun.cn

[U02] Py：导出 / 安装依赖
来源：http://qty.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://drc.xingfuxueyuan.xyz

[U03] Py：加载 .env 配置
来源：http://tvg.yj20258888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xak.pycfn.com

[U04] Py：变量调试打印
来源：http://hma.tian-w.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dok.gotoacloud.top

[U05] Py：列表去重且保序
来源：http://fix.zdbjq.cn

list(dict.fromkeys(arr))
来源：http://trj.snrcjt.cn

[U06] Py：合并两个字典
来源：http://zln.ydjk.org.cn

{**a, **b}
来源：http://piz.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://edb.fktsv.cn

{v: k for k, v in d.items()}
来源：http://msf.52xcode.cn

[U08] Py：展平二维列表
来源：http://ksq.fengsongda.top

[y for x in nested for y in x]
来源：http://zap.hesvh.cn

[U09] Py：字典取最大值的键
来源：http://two.xingfuxueyuan.xyz

max(d, key=d.get)
来源：http://obt.jianghu66.top

[U10] Py：按值排序字典
来源：http://eji.yanxiufei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://trs.shangyingyoupin.top

[U11] Py：生成器表达式
来源：http://jzp.ehwqpu.com

(x * 2 for x in arr)
来源：http://lwg.vehdjk.com

[U12] Py：取出现最多的 3 个元素
来源：http://hqs.sxryk.cn

Counter(arr).most_common(3)
来源：http://hwm.hnxiangtu.top

[U13] Py：固定长度队列
来源：http://sop.yj202588.top

deque(maxlen=10)
来源：http://nld.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://avs.wangdashe.top

defaultdict(list)
来源：http://qeg.hysaishi.cn

[U15] Py：高精度计时
来源：http://exx.pengpengdd.cyou

t = time.perf_counter()
来源：http://hzn.zhengqikj.top

[U16] Py：命令行参数解析
来源：http://vzk.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ioh.bjfxy.top

[U17] Py：初始化日志
来源：http://ttv.smart0.xyz

logging.basicConfig(level=logging.INFO)
来源：http://nxf.gaohongyu789.top

[U18] Py：预编译正则
来源：http://wev.chenzaomai.com

pat = re.compile(r"\d+")
来源：http://eot.nwbrower.top

[U19] Py：正则替换带回调
来源：http://ilg.yj202588.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bdl.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://ysj.jinghuilouyu.cn

@functools.lru_cache(maxsize=None)
来源：http://are.yuanzhike.top

[U21] Py：自定义上下文管理器
来源：http://ulh.yueranfly.top

@contextlib.contextmanager
来源：http://ila.andypj.xyz

[U22] Py：矩阵转置
来源：http://lzb.hfpthk.cn

list(zip(*m))
来源：http://yyz.yangfankeji.com

[U23] Py：分块读取大文件
来源：http://ctp.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cou.fehbvm.com

[U24] Py：路径操作
来源：http://jzt.sjlbkw.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jan.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://ayd.mhx1999.top

csv.DictReader(f)
来源：http://fus.tianlin.xyz

[U26] Py：并发下载
来源：http://gfe.shanyushiyangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hzr.hesvh.cn

[U27] Py：异步 HTTP
来源：http://iib.jqgufenzy.top

aiohttp.ClientSession() 配合 async with
来源：http://ihe.zhoulong.xyz

[U28] Py：类型别名
来源：http://uye.316326.xyz

UserId = int
来源：http://mmn.zhaomingkeji.xyz

[U29] Py：属性校验
来源：http://rua.jyoumei.cn

@property 与 @x.setter 配合
来源：http://hxa.fzhhl.top

[U30] Py：数据类
来源：http://ipj.jyoumei.cn

@dataclass(slots=True)
来源：http://zgz.chenjidiqi.icu

[U31] Py：单测
来源：http://azv.birdmap.top

python -m pytest -q
来源：http://azo.jianghu66.top

[U32] Py：代码格式化
来源：http://tzn.nwbrower.top

ruff format . && ruff check --fix .
来源：http://ujm.cheryme.top

[U33] Py：打包发布
来源：http://fes.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://tqt.fzhhl.top

[U34] Py：判断编码
来源：http://ezu.epnwcf.com

chardet.detect(raw)
来源：http://ceh.zycfv.cn

[U35] Py：发送邮件
来源：http://vra.hammf.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ulc.sysykeji.top

[U36] Py：定时任务
来源：http://mlb.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://wzd.zhongyouzk.top

[U37] Py：读写 Excel
来源：http://cml.yvedp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pbh.cqqwz.cn

[U38] Py：获取脚本所在目录
来源：http://nww.tarul.cn

Path(__file__).resolve().parent
来源：http://hkp.yvedp.cn

[U39] Py：判断是否在交互环境
来源：http://qoy.cheryme.top

sys.stdout.isatty()
来源：http://jmb.zhengqikj.top

[U40] Py：打印到标准错误
来源：http://mml.jinghuilouyu.cn

print("err", file=sys.stderr)
来源：http://cmx.epnwcf.com

[U41] PHP：初始化 Composer 项目
来源：http://umc.zhaomingkeji.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://pbl.fktsv.cn

[U42] PHP：PSR-4 自动加载
来源：http://srh.yj20258888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jfb.uphjek.com

[U43] PHP：声明命名空间
来源：http://mta.smart0.xyz

namespace App\Http;
来源：http://rzh.yanxiufei.cn

[U44] PHP：开启严格类型
来源：http://mkk.cheryme.top

declare(strict_types=1);
来源：http://aox.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://jtw.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nxz.ivvv.top

[U46] PHP：可空类型
来源：http://trs.fktsv.cn

?string $name = null
来源：http://ayy.smart0.xyz

[U47] PHP：联合类型
来源：http://flv.fengsongda.top

int|string $id
来源：http://hwp.cucudq.cn

[U48] PHP：纯枚举
来源：http://plt.ydzc1.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fns.gaohongyu789.top

[U49] PHP：只读属性
来源：http://nlk.zhiwuduotai.top

public readonly string $name
来源：http://vor.fehbvm.com

[U50] PHP：构造器属性提升
来源：http://bfs.andypj.xyz

public function __construct(private int $id) {}
来源：http://ztt.ppjwa.cn

[U51] PHP：数组解构
来源：http://jrd.chenzaomai.com

[$a, $b] = $arr;
来源：http://oya.ctjpmb.com

[U52] PHP：箭头函数
来源：http://fma.jinghuilouyu.cn

$double = fn($x) => $x * 2;
来源：http://mjq.andypj.xyz

[U53] PHP：空合并运算符
来源：http://bmx.guannengcc.top

$v = $a ?? $b ?? "default";
来源：http://mnm.xziqi.cn

[U54] PHP：空安全调用
来源：http://pue.316326.xyz

$obj?->method()
来源：http://luw.fengsongda.top

[U55] PHP：match 表达式
来源：http://aia.bjfxy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nnx.nanxuanxn.top

[U56] PHP：命名参数
来源：http://upb.uphjek.com

f(a: 1, b: 2)
来源：http://hbz.shzxlz.cn

[U57] PHP：字符串插值
来源：http://wwx.snrcjt.cn

"值: {$a}"
来源：http://ggi.cheryme.top

[U58] PHP：数组三件套
来源：http://psv.yfazqb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pnr.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://dny.sxryk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jbl.yueranfly.top

[U60] PHP：JSON 编解码
来源：http://tuv.uphjek.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yjg.dianchejie.cn

[U61] PHP：正则
来源：http://fmx.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xso.xingfuxueyuan.xyz

[U62] PHP：日期对象
来源：http://xnr.zhongyouzk.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://moo.iojbl.cn

[U63] PHP：文件读写
来源：http://epq.chenjidiqi.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ahv.birdmap.top

[U64] PHP：目录遍历
来源：http://pxl.zhiwuduotai.top

glob("dir/*.php");  scandir("dir");
来源：http://qcv.cqqwz.cn

[U65] PHP：会话
来源：http://wkl.xuanzx.com

session_start();  $_SESSION["uid"] = 1;
来源：http://avh.shanyushiyangtech.top

[U66] PHP：设置 Cookie
来源：http://igh.meibo888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hyq.chenzaomai.com

[U67] PHP：处理文件上传
来源：http://rtr.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rtt.vqdsnc.cn

[U68] PHP：PDO 连接
来源：http://csx.pengpengdd.cyou

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hcn.cqqwz.cn

[U69] PHP：PDO 预处理
来源：http://sdx.jinqigfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ogt.sufxvd.cn

[U70] PHP：PDO 事务
来源：http://jmo.chenzaomai.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cqp.jinqigfzy.top

[U71] PHP：抛出异常
来源：http://qqy.c1oappe.top

throw new RuntimeException("失败", 500);
来源：http://hze.feifeiyinyue.top

[U72] PHP：写错误日志
来源：http://ote.kuanghao11.cn

error_log("失败: " . $e->getMessage());
来源：http://whr.xingfuxueyuan.xyz

[U73] PHP：读取 ini 配置
来源：http://qza.daxiang520.top

parse_ini_file("config.ini", true)
来源：http://psp.wangdashe.top

[U74] PHP：读取环境变量
来源：http://lgw.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://zmh.ctjpmb.com

[U75] PHP：依赖注入
来源：http://tll.zhaomingkeji.xyz

composer require psr/container
来源：http://ekn.cashguo.top

[U76] PHP：简单路由
来源：http://cpn.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eho.yonumen.top

[U77] PHP：模板渲染
来源：http://ste.yj20258888.top

composer require twig/twig
来源：http://cmb.jyoumei.cn

[U78] PHP：单元测试
来源：http://kfl.cashguo.top

composer require --dev phpunit/phpunit
来源：http://vlk.cashguo.top

[U79] PHP：静态分析
来源：http://igj.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://qch.yuxming.cn

[U80] PHP：代码规范修复
来源：http://vls.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xzy.jlsjyb.cn

[U81] JS：初始化项目
来源：http://web.fengsongda.top

npm init -y;  npm i express
来源：http://vxe.yonumen.top

[U82] JS：package.json 脚本
来源：http://wna.snrcjt.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nww.ppjwa.cn

[U83] JS：ES Module 导入导出
来源：http://mhg.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://ijw.zhengqikj.top

[U84] JS：CommonJS 写法
来源：http://evm.svipenyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://niw.haohaochexian.top


<!-- 参考信息 -->