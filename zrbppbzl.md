代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://jnt.cdnleiting.top

[S59] C++：静态断言
来源：http://dgz.xingfuxueyuan.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aad.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://rot.yueranfly.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uwy.hnxiangtu.top

================================================================================
来源：http://xqd.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ama.chenlongwang.top

================================================================================
来源：http://lwj.vehdjk.com

[T01] Kotlin：Hello World
来源：http://rki.gaohongyu789.top

println("Hello")
来源：http://xli.yj20258.top

[T02] Kotlin：变量
来源：http://dsy.zhijiandao.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eaw.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://pdx.0kj1m.cn

"值: $b"
来源：http://rtq.tarul.cn

[T04] Kotlin：空安全
来源：http://hfx.dashuyun.cn

val n: String? = null;  n?.length
来源：http://qjm.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://klm.yueranfly.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jbq.mhx1999.top

[T06] Kotlin：集合映射
来源：http://xcw.sjlbkw.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cyh.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://hoj.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bwv.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://pek.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://gxj.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://whm.nanxuanxn.top

fun String.exclaim() = this + "!"
来源：http://qof.epnwcf.com

[T10] Kotlin：默认参数
来源：http://eeb.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://blo.jlsjyb.cn

[T11] Kotlin：协程
来源：http://oha.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dvm.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://coz.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://tcq.sweek.top

[T13] Kotlin：只读 Map
来源：http://kui.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://cwa.nanxinkj.top

[T14] Kotlin：循环
来源：http://xfs.hywenlv.cn

for (i in 1..10) println(i)
来源：http://xtq.shanyushiyangkeji.top

[T15] Kotlin：接口
来源：http://fpr.bjfxy.top

interface Shape { fun area(): Double }
来源：http://aur.dianchejie.cn

[T16] Swift：Hello World
来源：http://uun.gotoacloud.top

print("Hello")
来源：http://oex.tianlin.xyz

[T17] Swift：变量与常量
来源：http://bmk.andypj.xyz

var a = 1;  let b = 2
来源：http://mll.epnwcf.com

[T18] Swift：字符串插值
来源：http://nso.kuanghao11.cn

"值: \(b)"
来源：http://oeb.sweek.top

[T19] Swift：可选绑定
来源：http://ctk.cucudq.cn

if let n = opt { print(n) }
来源：http://klk.hysaishi.cn

[T20] Swift：数组操作
来源：http://dvx.yj202588.top

var a = [1, 2, 3];  a.append(4)
来源：http://ysl.wangdashe.top

[T21] Swift：遍历
来源：http://ygt.tanke756.top

for x in a { print(x) }
来源：http://nwt.dianchejie.cn

[T22] Swift：字典
来源：http://hdq.snrcjt.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tnh.gotoacloud.top

[T23] Swift：函数
来源：http://gnv.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lkh.tianlin.xyz

[T24] Swift：闭包
来源：http://omt.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://reg.jianghu66.top

[T25] Swift：结构体
来源：http://glb.shuidangran.top

struct P { var x: Int }
来源：http://qxm.tarul.cn

[T26] Swift：类与重写
来源：http://aye.zhijiandao.cn

class A: Base { override func f() {} }
来源：http://cxb.jinghuilouyu.cn

[T27] Swift：错误处理
来源：http://fly.fehbvm.com

do { try f() } catch { print(error) }
来源：http://kps.wangdashe.top

[T28] Swift：枚举
来源：http://njv.kuanghao11.cn

enum Color { case red, green }
来源：http://hyu.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://yeb.ctjpmb.com

guard let x = opt else { return }
来源：http://tqf.bjfxy.top

[T30] Swift：协议
来源：http://nvv.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://xqk.epnwcf.com

[T31] Lua：Hello World
来源：http://uhg.cqqwz.cn

print("Hello")
来源：http://ldk.sufxvd.cn

[T32] Lua：局部变量
来源：http://wlz.yueranfly.top

local a = 1
来源：http://lil.gotoacloud.top

[T33] Lua：表（数组）
来源：http://dby.quarkkingdee.top

local t = {1, 2, 3};  t[4] = 4
来源：http://aql.svipenyu.cn

[T34] Lua：遍历表
来源：http://htw.bbcook.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nfq.hnxiangtu.top

[T35] Lua：字典表
来源：http://cio.zycfv.cn

local d = { a = 1 };  d.b = 2
来源：http://lfu.andypj.xyz

[T36] Lua：函数
来源：http://bee.zdbjq.cn

function add(a, b) return a + b end
来源：http://cvr.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://aum.yj20258888.top

"a" .. "b"
来源：http://pwn.zhongyouzk.top

[T38] Lua：条件
来源：http://imc.birdmap.top

if x > 0 then print("正") end
来源：http://ion.jinqigufen.top

[T39] Lua：模式匹配
来源：http://rki.ehwqpu.com

string.find(s, "%d+")
来源：http://gsw.xylfe.cn

[T40] Lua：元表
来源：http://zrp.fengsongda.top

setmetatable({}, { __index = base })
来源：http://szs.fktsv.cn

[T41] Perl：Hello World
来源：http://cgg.jlsjyb.cn

print "Hello\n";
来源：http://gyd.jlsjyb.cn

[T42] Perl：变量类型
来源：http://vjv.jinghuilouyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yhs.xinyue.icu

[T43] Perl：字符串插值
来源：http://jmn.jiagoushi.top

"值: $a"
来源：http://abh.guannengcc.top

[T44] Perl：条件
来源：http://xwl.ivvv.top

if ($a > 0) { print "正"; }
来源：http://htm.jqgufenzy.top

[T45] Perl：数组遍历
来源：http://gda.yonumen.top

for my $x (@arr) { print $x; }
来源：http://zwc.yj20258.top

[T46] Perl：哈希操作
来源：http://vpa.9152youxi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zkd.yongpay.top

[T47] Perl：正则捕获
来源：http://bsp.birdmap.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://asz.yangfankeji.com

[T48] Perl：正则替换
来源：http://veu.9152youxi.cn

$s =~ s/old/new/g;
来源：http://kbc.cucudq.cn

[T49] Perl：函数
来源：http://tdq.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gwh.hcnkem.com

[T50] Perl：逐行读文件
来源：http://fwl.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cyi.daria6918.cn

while (my $line = <$fh>) { print $line; }
来源：http://ehh.ppjwa.cn

[T51] Scala：Hello World
来源：http://rxn.fzhhl.top

println("Hello")
来源：http://hxi.tianlin.xyz

[T52] Scala：变量
来源：http://lol.zhijiandao.cn

val a = 1;  var b = 2
来源：http://tdu.redwolf501.top

[T53] Scala：字符串插值
来源：http://ycm.tianlin.xyz

s"值: $b"
来源：http://ude.quarkkingdee.top

[T54] Scala：集合映射
来源：http://ymu.gzhubu.top

List(1, 2, 3).map(_ * 2)
来源：http://niy.fengsongda.top

[T55] Scala：集合过滤
来源：http://yhv.ybcxt.top

List(1, 2, 3).filter(_ > 1)
来源：http://azk.zhixingplan.top

[T56] Scala：样例类
来源：http://udt.sxryk.cn

case class User(name: String, age: Int)
来源：http://zxx.dianchejie.cn

[T57] Scala：模式匹配
来源：http://qls.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://upg.shanyushiyangkeji.top

[T58] Scala：函数定义
来源：http://iuj.hesvh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fxy.guowangkeji.top

[T59] Scala：循环
来源：http://ccf.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://giy.nanxinkj.top

[T60] Scala：折叠
来源：http://abd.jiagoushi.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xst.jinqigufen.top

================================================================================
来源：http://rsl.kuanghao11.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bxs.ywan-chungtsiang.top

================================================================================
来源：http://aph.redwolf501.top

[U01] Py：创建虚拟环境
来源：http://lam.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://sne.sysykeji.top

[U02] Py：导出 / 安装依赖
来源：http://jjj.hnxiangtu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ncw.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://wnb.yonumen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xgd.zycfv.cn

[U04] Py：变量调试打印
来源：http://gcf.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gay.fktsv.cn

[U05] Py：列表去重且保序
来源：http://fux.yj20258888.top

list(dict.fromkeys(arr))
来源：http://iwv.jyoumei.cn

[U06] Py：合并两个字典
来源：http://cct.zhixingplan.top

{**a, **b}
来源：http://vgp.pycfn.com

[U07] Py：反转字典键值
来源：http://jtv.fzhhl.top

{v: k for k, v in d.items()}
来源：http://vrb.smart0.xyz

[U08] Py：展平二维列表
来源：http://kgo.zhoulong.xyz

[y for x in nested for y in x]
来源：http://anl.chenzaomai.com

[U09] Py：字典取最大值的键
来源：http://wrr.quarkkingdee.top

max(d, key=d.get)
来源：http://ncq.ywan-chungtsiang.top

[U10] Py：按值排序字典
来源：http://ypv.zdbjq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qnz.fehbvm.com

[U11] Py：生成器表达式
来源：http://jvr.ivvv.top

(x * 2 for x in arr)
来源：http://cbd.iojbl.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cet.yfazqb.com

Counter(arr).most_common(3)
来源：http://lyb.smart0.xyz

[U13] Py：固定长度队列
来源：http://ehc.snrcjt.cn

deque(maxlen=10)
来源：http://dkk.jyoumei.cn

[U14] Py：分组收集到列表
来源：http://rib.nanxinkj.top

defaultdict(list)
来源：http://pep.jyoumei.cn

[U15] Py：高精度计时
来源：http://iiu.tanke756.top

t = time.perf_counter()
来源：http://aub.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://csu.zhongyouzk.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zsz.jinqigufen.top

[U17] Py：初始化日志
来源：http://mpk.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://ehs.daxiang520.top

[U18] Py：预编译正则
来源：http://jgp.9152youxi.cn

pat = re.compile(r"\d+")
来源：http://mmc.zhiwuduotai.top

[U19] Py：正则替换带回调
来源：http://gwq.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kvi.tanke756.top

[U20] Py：缓存函数结果
来源：http://iit.jinghuilouyu.cn

@functools.lru_cache(maxsize=None)
来源：http://mkr.uphjek.com

[U21] Py：自定义上下文管理器
来源：http://tdw.smart0.xyz

@contextlib.contextmanager
来源：http://xru.yongpay.top

[U22] Py：矩阵转置
来源：http://afy.aibaodan.cn

list(zip(*m))
来源：http://qtr.hcnkem.com

[U23] Py：分块读取大文件
来源：http://cbg.aizwys.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tfl.ybcxt.top

[U24] Py：路径操作
来源：http://spv.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tpg.cdnleiting.top

[U25] Py：CSV 按字典读
来源：http://cgo.sufxvd.cn

csv.DictReader(f)
来源：http://zag.snrcjt.cn

[U26] Py：并发下载
来源：http://wfb.xuanzx.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hlo.yuxming.cn

[U27] Py：异步 HTTP
来源：http://woz.ywan-chungtsiang.top

aiohttp.ClientSession() 配合 async with
来源：http://uql.hysaishi.cn

[U28] Py：类型别名
来源：http://bdi.pengpengdd.cyou

UserId = int
来源：http://kgx.redwolf501.top

[U29] Py：属性校验
来源：http://omb.bjfxy.top

@property 与 @x.setter 配合
来源：http://gid.ehwqpu.com

[U30] Py：数据类
来源：http://swv.zhengqikj.top

@dataclass(slots=True)
来源：http://daa.hammf.cn

[U31] Py：单测
来源：http://vxq.cheryme.top

python -m pytest -q
来源：http://bee.tanke756.top

[U32] Py：代码格式化
来源：http://fro.zhiwuduotai.top

ruff format . && ruff check --fix .
来源：http://qnh.yvedp.cn

[U33] Py：打包发布
来源：http://hif.zdqjudy.top

python -m build  （依赖 pyproject.toml）
来源：http://xxf.kuanghao11.cn

[U34] Py：判断编码
来源：http://fbi.jqgfzy.top

chardet.detect(raw)
来源：http://afm.dashuyun.cn

[U35] Py：发送邮件
来源：http://bxg.sjlbkw.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wlm.sysykeji.top

[U36] Py：定时任务
来源：http://njx.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://mwu.haohaochexian.top

[U37] Py：读写 Excel
来源：http://gib.hysaishi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pfu.jiagoushi.top

[U38] Py：获取脚本所在目录
来源：http://hxp.jyoumei.cn

Path(__file__).resolve().parent
来源：http://mne.jinqigufen.top

[U39] Py：判断是否在交互环境
来源：http://yaq.ybcxt.top

sys.stdout.isatty()
来源：http://kqy.ctjpmb.com

[U40] Py：打印到标准错误
来源：http://ibb.ehwqpu.com

print("err", file=sys.stderr)
来源：http://hht.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://uvn.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://uht.chenlongwang.top

[U42] PHP：PSR-4 自动加载
来源：http://xmb.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kwe.hesvh.cn

[U43] PHP：声明命名空间
来源：http://kva.ivvv.top

namespace App\Http;
来源：http://unc.jianghu66.top

[U44] PHP：开启严格类型
来源：http://mpl.hcnkem.com

declare(strict_types=1);
来源：http://xsg.cdnleiting.top

[U45] PHP：类型声明与返回类型
来源：http://krn.shzxlz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://iao.gogol.net.cn

[U46] PHP：可空类型
来源：http://bbm.hnqzz.top

?string $name = null
来源：http://wsy.hnxiangtu.top

[U47] PHP：联合类型
来源：http://kkq.tanke756.top

int|string $id
来源：http://nfx.redwolf501.top

[U48] PHP：纯枚举
来源：http://xrn.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wjt.xuanzx.com

[U49] PHP：只读属性
来源：http://obr.yuxming.cn

public readonly string $name
来源：http://hwb.ydzc1.top

[U50] PHP：构造器属性提升
来源：http://qvh.meibo888.top

public function __construct(private int $id) {}
来源：http://bxx.feifeiyinyue.top

[U51] PHP：数组解构
来源：http://kze.kuanghao11.cn

[$a, $b] = $arr;
来源：http://kre.xylfe.cn

[U52] PHP：箭头函数
来源：http://frw.zhijiandao.cn

$double = fn($x) => $x * 2;
来源：http://mwx.jyoumei.cn

[U53] PHP：空合并运算符
来源：http://cex.chenlongwang.top

$v = $a ?? $b ?? "default";
来源：http://nrp.zdbjq.cn

[U54] PHP：空安全调用
来源：http://wdl.snrcjt.cn

$obj?->method()
来源：http://gae.zhaomingkeji.xyz

[U55] PHP：match 表达式
来源：http://anl.hfpthk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ust.nanxinkj.top

[U56] PHP：命名参数
来源：http://qno.xinyue.icu

f(a: 1, b: 2)
来源：http://xnt.ybcxt.top

[U57] PHP：字符串插值
来源：http://ufj.vehdjk.com

"值: {$a}"
来源：http://qgl.jinyuanbaomall.cn

[U58] PHP：数组三件套
来源：http://qfc.tanke756.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wem.zhixingplan.top

[U59] PHP：自定义排序
来源：http://mpj.yonumen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dxr.hysaishi.cn

[U60] PHP：JSON 编解码
来源：http://ood.jianghu66.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://btg.daxiang520.top

[U61] PHP：正则
来源：http://jhi.9152youxi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jsj.kuanghao11.cn

[U62] PHP：日期对象
来源：http://vrr.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://voz.wangdashe.top

[U63] PHP：文件读写
来源：http://uuw.ivvv.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mbh.zycfv.cn

[U64] PHP：目录遍历
来源：http://cce.havefunace.top

glob("dir/*.php");  scandir("dir");
来源：http://yaw.wangdashe.top

[U65] PHP：会话
来源：http://ndt.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://orw.gotoacloud.top

[U66] PHP：设置 Cookie
来源：http://dlf.jqgufenzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rxu.ehwqpu.com

[U67] PHP：处理文件上传
来源：http://zjd.shanyushiyangtech.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://asr.wangdashe.top

[U68] PHP：PDO 连接
来源：http://tfa.guannengcc.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wyg.cheryme.top

[U69] PHP：PDO 预处理
来源：http://buu.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gek.smart0.xyz

[U70] PHP：PDO 事务
来源：http://czf.zhiwuduotai.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://afh.guannengcc.top

[U71] PHP：抛出异常
来源：http://vuc.xuetiantiany.cn

throw new RuntimeException("失败", 500);
来源：http://psg.yj202588.top

[U72] PHP：写错误日志
来源：http://krx.jiagoushi.top

error_log("失败: " . $e->getMessage());
来源：http://qtp.zhijiandao.cn

[U73] PHP：读取 ini 配置
来源：http://hir.316326.xyz

parse_ini_file("config.ini", true)
来源：http://auj.iojbl.cn

[U74] PHP：读取环境变量
来源：http://dgh.nwbrower.top

getenv("APP_ENV") ?: "production"
来源：http://cdh.yfazqb.com

[U75] PHP：依赖注入
来源：http://mle.fengsongda.top

composer require psr/container
来源：http://fjc.sweek.top

[U76] PHP：简单路由
来源：http://qel.fktsv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tmy.xingfuxueyuan.xyz

[U77] PHP：模板渲染
来源：http://shi.ivvv.top

composer require twig/twig
来源：http://ehu.nanxuanxn.top

[U78] PHP：单元测试
来源：http://tdh.ctjpmb.com

composer require --dev phpunit/phpunit
来源：http://ljc.andypj.xyz

[U79] PHP：静态分析
来源：http://erm.hfpthk.cn

composer require --dev phpstan/phpstan
来源：http://tgl.c1oappe.top

[U80] PHP：代码规范修复
来源：http://wfm.sxryk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dcb.chenjidiqi.icu

[U81] JS：初始化项目
来源：http://oqb.nanxinkj.top

npm init -y;  npm i express
来源：http://ipx.316326.xyz

[U82] JS：package.json 脚本
来源：http://dkj.shanyushiyangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vjs.wangshuangyany.cn

[U83] JS：ES Module 导入导出
来源：http://oyp.jinghuilouyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://isx.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://twr.pycfn.com

module.exports = { a };  const { a } = require("./m");
来源：http://oqi.gotoacloud.top


<!-- 参考信息 -->