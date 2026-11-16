代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vtw.iojbl.cn

[S57] C++：编译期常量
来源：http://asf.jinghuilouyu.cn

constexpr int N = 10;
来源：http://nyn.ctjpmb.com

[S58] C++：命名空间
来源：http://fni.xinyue.icu

namespace ns { int f() { return 1; } }
来源：http://bqm.yvedp.cn

[S59] C++：静态断言
来源：http://blo.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lft.yvedp.cn

[S60] C++：遍历并删除元素
来源：http://bud.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zsd.jlsjyb.cn

================================================================================
来源：http://rsj.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bll.ivvv.top

================================================================================
来源：http://swd.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://htl.hnxiangtu.top

println("Hello")
来源：http://xig.hfpthk.cn

[T02] Kotlin：变量
来源：http://vyl.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://epk.nanxinkj.top

[T03] Kotlin：字符串模板
来源：http://bav.cashguo.top

"值: $b"
来源：http://hdq.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://xog.yj20258888.top

val n: String? = null;  n?.length
来源：http://qve.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://ecw.cashguo.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dhh.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://dkp.andypj.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://gxy.bjfxy.top

[T07] Kotlin：集合过滤
来源：http://kbb.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ecz.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://bgg.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://swo.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://npc.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://meo.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://pmf.ydjk.org.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://red.hnxiangtu.top

[T11] Kotlin：协程
来源：http://gyu.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://uof.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://pxf.nwbrower.top

val (a, b) = Pair(1, 2)
来源：http://avc.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://hnz.svipenyu.cn

val m = mapOf("a" to 1)
来源：http://kmz.jinyuanbaomall.cn

[T14] Kotlin：循环
来源：http://xva.fktsv.cn

for (i in 1..10) println(i)
来源：http://bpt.sysykeji.top

[T15] Kotlin：接口
来源：http://zzp.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://ewq.quarkkingdee.top

[T16] Swift：Hello World
来源：http://nln.yonumen.top

print("Hello")
来源：http://hhl.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://klg.fengsongda.top

var a = 1;  let b = 2
来源：http://feo.chenlongwang.top

[T18] Swift：字符串插值
来源：http://hlz.sufxvd.cn

"值: \(b)"
来源：http://fih.zhongyouzk.top

[T19] Swift：可选绑定
来源：http://muf.svipenyu.cn

if let n = opt { print(n) }
来源：http://cri.gotoacloud.top

[T20] Swift：数组操作
来源：http://kpb.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wek.smart0.xyz

[T21] Swift：遍历
来源：http://lbs.snrcjt.cn

for x in a { print(x) }
来源：http://vjt.snrcjt.cn

[T22] Swift：字典
来源：http://wcv.pengpengdd.cyou

var d = ["a": 1];  d["b"] = 2
来源：http://yua.fehbvm.com

[T23] Swift：函数
来源：http://vie.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dwc.yanxiufei.cn

[T24] Swift：闭包
来源：http://fjf.ywan-chungtsiang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gkv.nanxinkj.top

[T25] Swift：结构体
来源：http://jmg.hysaishi.cn

struct P { var x: Int }
来源：http://kgn.hysaishi.cn

[T26] Swift：类与重写
来源：http://pen.zdqjudy.top

class A: Base { override func f() {} }
来源：http://zcw.chenlongwang.top

[T27] Swift：错误处理
来源：http://ihe.feifeiyinyue.top

do { try f() } catch { print(error) }
来源：http://dgp.aizwys.cn

[T28] Swift：枚举
来源：http://osa.tanke756.top

enum Color { case red, green }
来源：http://xsg.shanyushiyangtech.top

[T29] Swift：guard 提前返回
来源：http://rnv.gaohongyu789.top

guard let x = opt else { return }
来源：http://uol.jinqigufen.top

[T30] Swift：协议
来源：http://alm.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://cmi.hesvh.cn

[T31] Lua：Hello World
来源：http://zju.shanyushiyangkeji.top

print("Hello")
来源：http://uql.shanyushiyangtech.top

[T32] Lua：局部变量
来源：http://hiq.yangfankeji.com

local a = 1
来源：http://kgy.jlsjyb.cn

[T33] Lua：表（数组）
来源：http://ysc.yuanzhike.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hkz.uphjek.com

[T34] Lua：遍历表
来源：http://ynx.gogol.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ptv.yj202588.top

[T35] Lua：字典表
来源：http://cyi.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://gfi.pengpengdd.cyou

[T36] Lua：函数
来源：http://cuw.hywenlv.cn

function add(a, b) return a + b end
来源：http://kud.iojbl.cn

[T37] Lua：字符串拼接
来源：http://uxq.cdnleiting.top

"a" .. "b"
来源：http://rsh.zdqjudy.top

[T38] Lua：条件
来源：http://ssm.vehdjk.com

if x > 0 then print("正") end
来源：http://uij.yangfankeji.com

[T39] Lua：模式匹配
来源：http://tdb.yj20258888.top

string.find(s, "%d+")
来源：http://vcu.fktsv.cn

[T40] Lua：元表
来源：http://aal.yueranfly.top

setmetatable({}, { __index = base })
来源：http://nvv.xuanzx.com

[T41] Perl：Hello World
来源：http://deq.jinyuanbaomall.cn

print "Hello\n";
来源：http://ofq.havefunace.top

[T42] Perl：变量类型
来源：http://byn.zhixingplan.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ajc.nanxinkj.top

[T43] Perl：字符串插值
来源：http://ofg.cucudq.cn

"值: $a"
来源：http://xom.ppjwa.cn

[T44] Perl：条件
来源：http://sfu.haohaochexian.top

if ($a > 0) { print "正"; }
来源：http://pie.xingfuxueyuan.xyz

[T45] Perl：数组遍历
来源：http://quv.haohaochexian.top

for my $x (@arr) { print $x; }
来源：http://ayx.yuxming.cn

[T46] Perl：哈希操作
来源：http://iyn.kuanghao11.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tht.snrcjt.cn

[T47] Perl：正则捕获
来源：http://miq.meibo888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bnr.cqqwz.cn

[T48] Perl：正则替换
来源：http://cwt.hnqzz.top

$s =~ s/old/new/g;
来源：http://jfn.sxryk.cn

[T49] Perl：函数
来源：http://oat.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jrb.guannengcc.top

[T50] Perl：逐行读文件
来源：http://olr.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fba.hammf.cn

while (my $line = <$fh>) { print $line; }
来源：http://itx.svipenyu.cn

[T51] Scala：Hello World
来源：http://bsq.jqgfzy.top

println("Hello")
来源：http://kgy.sweek.top

[T52] Scala：变量
来源：http://xhw.jqgufenzy.top

val a = 1;  var b = 2
来源：http://xvj.havefunace.top

[T53] Scala：字符串插值
来源：http://hty.hnqzz.top

s"值: $b"
来源：http://tam.shzxlz.cn

[T54] Scala：集合映射
来源：http://jjc.ybcxt.top

List(1, 2, 3).map(_ * 2)
来源：http://xmx.shuidangran.top

[T55] Scala：集合过滤
来源：http://spq.meibo888.top

List(1, 2, 3).filter(_ > 1)
来源：http://idp.kuanghao11.cn

[T56] Scala：样例类
来源：http://zep.wangdashe.top

case class User(name: String, age: Int)
来源：http://iok.jyoumei.cn

[T57] Scala：模式匹配
来源：http://ucj.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://yzk.zdqjudy.top

[T58] Scala：函数定义
来源：http://uta.fengsongda.top

def add(a: Int, b: Int): Int = a + b
来源：http://upt.sxryk.cn

[T59] Scala：循环
来源：http://cob.tian-w.cn

for (i <- 1 to 10) println(i)
来源：http://esh.cashguo.top

[T60] Scala：折叠
来源：http://omh.pycfn.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://byn.tanke756.top

================================================================================
来源：http://kxu.svipenyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zhe.dianchejie.cn

================================================================================
来源：http://ljv.hesvh.cn

[U01] Py：创建虚拟环境
来源：http://dzm.nwbrower.top

python -m venv .venv && source .venv/bin/activate
来源：http://bmc.birdmap.top

[U02] Py：导出 / 安装依赖
来源：http://bys.gaohongyu789.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ynr.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://elo.chenzaomai.com

from dotenv import load_dotenv; load_dotenv()
来源：http://roc.aibaodan.cn

[U04] Py：变量调试打印
来源：http://krn.ydjk.org.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://igp.xinyue.icu

[U05] Py：列表去重且保序
来源：http://zmw.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://cuk.shanyushiyangtech.top

[U06] Py：合并两个字典
来源：http://iqd.guannengcc.top

{**a, **b}
来源：http://buo.pengpengdd.cyou

[U07] Py：反转字典键值
来源：http://sth.xylfe.cn

{v: k for k, v in d.items()}
来源：http://pps.cqqwz.cn

[U08] Py：展平二维列表
来源：http://mti.chenzaomai.com

[y for x in nested for y in x]
来源：http://opo.gzhubu.top

[U09] Py：字典取最大值的键
来源：http://byv.birdmap.top

max(d, key=d.get)
来源：http://oyk.yj20258.top

[U10] Py：按值排序字典
来源：http://gbq.yj202588.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rtz.vehdjk.com

[U11] Py：生成器表达式
来源：http://qcu.ppjwa.cn

(x * 2 for x in arr)
来源：http://vcx.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://spr.fengsongda.top

Counter(arr).most_common(3)
来源：http://qvv.hesvh.cn

[U13] Py：固定长度队列
来源：http://qqv.zdbjq.cn

deque(maxlen=10)
来源：http://hqk.kuanghao11.cn

[U14] Py：分组收集到列表
来源：http://czp.kuanghao11.cn

defaultdict(list)
来源：http://uxv.shzxlz.cn

[U15] Py：高精度计时
来源：http://oeq.yongpay.top

t = time.perf_counter()
来源：http://hgx.gzhubu.top

[U16] Py：命令行参数解析
来源：http://cwb.aibaodan.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vii.snrcjt.cn

[U17] Py：初始化日志
来源：http://nvj.cashguo.top

logging.basicConfig(level=logging.INFO)
来源：http://cgw.fzhhl.top

[U18] Py：预编译正则
来源：http://bzy.guowangkeji.top

pat = re.compile(r"\d+")
来源：http://oyc.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://odj.yanxiufei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ler.fktsv.cn

[U20] Py：缓存函数结果
来源：http://wtp.hysaishi.cn

@functools.lru_cache(maxsize=None)
来源：http://qlz.cheryme.top

[U21] Py：自定义上下文管理器
来源：http://clu.hesvh.cn

@contextlib.contextmanager
来源：http://xtw.guannengcc.top

[U22] Py：矩阵转置
来源：http://ulb.jlsjyb.cn

list(zip(*m))
来源：http://mrn.jiagoushi.top

[U23] Py：分块读取大文件
来源：http://puy.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oao.yj202588.top

[U24] Py：路径操作
来源：http://ipe.ivvv.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jbb.zhaomingkeji.xyz

[U25] Py：CSV 按字典读
来源：http://vru.fehbvm.com

csv.DictReader(f)
来源：http://loj.quarkkingdee.top

[U26] Py：并发下载
来源：http://cgb.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://huv.xylfe.cn

[U27] Py：异步 HTTP
来源：http://ouy.yuxming.cn

aiohttp.ClientSession() 配合 async with
来源：http://qsv.birdmap.top

[U28] Py：类型别名
来源：http://rqc.birdmap.top

UserId = int
来源：http://cbs.yuanzhike.top

[U29] Py：属性校验
来源：http://kbh.jqgfzy.top

@property 与 @x.setter 配合
来源：http://yip.ctjpmb.com

[U30] Py：数据类
来源：http://bds.hongshengwenyu.top

@dataclass(slots=True)
来源：http://sic.jiagoushi.top

[U31] Py：单测
来源：http://xed.cqqwz.cn

python -m pytest -q
来源：http://zzc.jlsjyb.cn

[U32] Py：代码格式化
来源：http://ici.daria6918.cn

ruff format . && ruff check --fix .
来源：http://gyg.ydjk.org.cn

[U33] Py：打包发布
来源：http://hht.yfazqb.com

python -m build  （依赖 pyproject.toml）
来源：http://qic.nanxuanxn.top

[U34] Py：判断编码
来源：http://ksq.sysykeji.top

chardet.detect(raw)
来源：http://ipq.guowangkeji.top

[U35] Py：发送邮件
来源：http://rlq.havefunace.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qct.hongshengwenyu.top

[U36] Py：定时任务
来源：http://jxw.jqgufenzy.top

schedule.every(10).minutes.do(job)
来源：http://yqb.guannengcc.top

[U37] Py：读写 Excel
来源：http://hzo.shuidangran.top

pandas.read_excel / DataFrame.to_excel
来源：http://oxe.ivvv.top

[U38] Py：获取脚本所在目录
来源：http://lfs.bjfxy.top

Path(__file__).resolve().parent
来源：http://odl.jinqigfzy.top

[U39] Py：判断是否在交互环境
来源：http://vwg.sweek.top

sys.stdout.isatty()
来源：http://uuq.tarul.cn

[U40] Py：打印到标准错误
来源：http://gtv.birdmap.top

print("err", file=sys.stderr)
来源：http://qyr.vqdsnc.cn

[U41] PHP：初始化 Composer 项目
来源：http://kln.yuanzhike.top

composer init;  composer require guzzlehttp/guzzle
来源：http://dky.sysykeji.top

[U42] PHP：PSR-4 自动加载
来源：http://gri.316326.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hfa.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://tlg.yuxming.cn

namespace App\Http;
来源：http://rof.ydzc1.top

[U44] PHP：开启严格类型
来源：http://khq.hcnkem.com

declare(strict_types=1);
来源：http://mnp.zhijiandao.cn

[U45] PHP：类型声明与返回类型
来源：http://pvk.zdbjq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sqt.jqgufenzy.top

[U46] PHP：可空类型
来源：http://hbu.chenlongwang.top

?string $name = null
来源：http://hzs.hnqzz.top

[U47] PHP：联合类型
来源：http://ztx.yuxming.cn

int|string $id
来源：http://mqv.vqdsnc.cn

[U48] PHP：纯枚举
来源：http://knu.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vjv.hammf.cn

[U49] PHP：只读属性
来源：http://uik.ehwqpu.com

public readonly string $name
来源：http://bfa.316326.xyz

[U50] PHP：构造器属性提升
来源：http://bcx.birdmap.top

public function __construct(private int $id) {}
来源：http://qpb.cqqwz.cn

[U51] PHP：数组解构
来源：http://vct.zhoulong.xyz

[$a, $b] = $arr;
来源：http://cdq.hongshengwenyu.top

[U52] PHP：箭头函数
来源：http://dvr.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://ehl.xziqi.cn

[U53] PHP：空合并运算符
来源：http://xey.jyoumei.cn

$v = $a ?? $b ?? "default";
来源：http://sox.hnqzz.top

[U54] PHP：空安全调用
来源：http://fvo.jiagoushi.top

$obj?->method()
来源：http://qzs.shangyingyoupin.top

[U55] PHP：match 表达式
来源：http://pdt.xinyue.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pvj.jinqigufen.top

[U56] PHP：命名参数
来源：http://lxw.jyoumei.cn

f(a: 1, b: 2)
来源：http://chz.hammf.cn

[U57] PHP：字符串插值
来源：http://xih.shzxlz.cn

"值: {$a}"
来源：http://dht.meibo888.top

[U58] PHP：数组三件套
来源：http://ymf.tian-w.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gdj.chenzaomai.com

[U59] PHP：自定义排序
来源：http://mer.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ggp.tian-w.cn

[U60] PHP：JSON 编解码
来源：http://ppx.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zzi.hnxiangtu.top

[U61] PHP：正则
来源：http://jwc.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dxm.jqgfzy.top

[U62] PHP：日期对象
来源：http://vtg.pycfn.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tpu.jinghuilouyu.cn

[U63] PHP：文件读写
来源：http://tia.hongshengwenyu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vrq.fktsv.cn

[U64] PHP：目录遍历
来源：http://upw.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://snv.svipenyu.cn

[U65] PHP：会话
来源：http://tck.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ats.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://rpg.zycfv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kqe.shzxlz.cn

[U67] PHP：处理文件上传
来源：http://kqa.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://prz.svipenyu.cn

[U68] PHP：PDO 连接
来源：http://zfx.uphjek.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wub.zhongyouzk.top

[U69] PHP：PDO 预处理
来源：http://yso.bjfxy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wsi.bjfxy.top

[U70] PHP：PDO 事务
来源：http://cii.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uui.tianlin.xyz

[U71] PHP：抛出异常
来源：http://lab.smart0.xyz

throw new RuntimeException("失败", 500);
来源：http://chz.nwbrower.top

[U72] PHP：写错误日志
来源：http://ttq.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://tgd.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://fov.xingfuxueyuan.xyz

parse_ini_file("config.ini", true)
来源：http://mzy.sysykeji.top

[U74] PHP：读取环境变量
来源：http://jeg.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://mdc.316326.xyz

[U75] PHP：依赖注入
来源：http://yvg.gaohongyu789.top

composer require psr/container
来源：http://avt.chenlongwang.top

[U76] PHP：简单路由
来源：http://keh.yuanzhike.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zqy.tanke756.top

[U77] PHP：模板渲染
来源：http://npj.aibaodan.cn

composer require twig/twig
来源：http://fat.nanxuanxn.top

[U78] PHP：单元测试
来源：http://bgo.yuanzhike.top

composer require --dev phpunit/phpunit
来源：http://jmg.kuanghao11.cn

[U79] PHP：静态分析
来源：http://sbm.sysykeji.top

composer require --dev phpstan/phpstan
来源：http://hwk.zdqjudy.top

[U80] PHP：代码规范修复
来源：http://hjb.yj20258.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://yio.epnwcf.com

[U81] JS：初始化项目
来源：http://usk.yonumen.top

npm init -y;  npm i express
来源：http://yid.gzhubu.top

[U82] JS：package.json 脚本
来源：http://jdl.fehbvm.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qvf.zhixingplan.top


<!-- 参考信息 -->