代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wdb.hnqzz.top

[S57] C++：编译期常量
来源：http://ngp.yueranfly.top

constexpr int N = 10;
来源：http://qhf.birdmap.top

[S58] C++：命名空间
来源：http://utx.jyoumei.cn

namespace ns { int f() { return 1; } }
来源：http://tvc.yuanzhike.top

[S59] C++：静态断言
来源：http://rjn.redwolf501.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hzg.cashguo.top

[S60] C++：遍历并删除元素
来源：http://ouh.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kix.jianghu66.top

================================================================================
来源：http://grr.zhiwuduotai.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hnq.svipenyu.cn

================================================================================
来源：http://aem.yvedp.cn

[T01] Kotlin：Hello World
来源：http://gnd.fehbvm.com

println("Hello")
来源：http://gsw.yuanzhike.top

[T02] Kotlin：变量
来源：http://wiu.bbcook.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fgp.pycfn.com

[T03] Kotlin：字符串模板
来源：http://gpw.jqgufenzy.top

"值: $b"
来源：http://rjc.yvedp.cn

[T04] Kotlin：空安全
来源：http://wch.tanke756.top

val n: String? = null;  n?.length
来源：http://ihx.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://ymh.xuetiantiany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yqr.dashuyun.cn

[T06] Kotlin：集合映射
来源：http://sdt.yanxiufei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://stg.yongpay.top

[T07] Kotlin：集合过滤
来源：http://ija.sysykeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nep.cheryme.top

[T08] Kotlin：数据类
来源：http://ktr.jinqigfzy.top

data class User(val name: String, val age: Int)
来源：http://xfm.tarul.cn

[T09] Kotlin：扩展函数
来源：http://wrm.aizwys.cn

fun String.exclaim() = this + "!"
来源：http://vsv.guannengcc.top

[T10] Kotlin：默认参数
来源：http://yzp.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://zak.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://cax.zdqjudy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://uwv.hnqzz.top

[T12] Kotlin：解构声明
来源：http://mdt.gogol.net.cn

val (a, b) = Pair(1, 2)
来源：http://yoq.c1oappe.top

[T13] Kotlin：只读 Map
来源：http://mte.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://eul.yueranfly.top

[T14] Kotlin：循环
来源：http://tfz.ivvv.top

for (i in 1..10) println(i)
来源：http://int.daria6918.cn

[T15] Kotlin：接口
来源：http://egz.yj20258.top

interface Shape { fun area(): Double }
来源：http://nfg.jinqigfzy.top

[T16] Swift：Hello World
来源：http://owo.redwolf501.top

print("Hello")
来源：http://gbc.haohaochexian.top

[T17] Swift：变量与常量
来源：http://ebs.sjlbkw.cn

var a = 1;  let b = 2
来源：http://omw.zdbjq.cn

[T18] Swift：字符串插值
来源：http://cbm.jinqigufen.top

"值: \(b)"
来源：http://zcd.vehdjk.com

[T19] Swift：可选绑定
来源：http://zkv.daxiang520.top

if let n = opt { print(n) }
来源：http://yfv.shanyushiyangtech.top

[T20] Swift：数组操作
来源：http://rkk.havefunace.top

var a = [1, 2, 3];  a.append(4)
来源：http://xcz.cdnleiting.top

[T21] Swift：遍历
来源：http://xbc.hysaishi.cn

for x in a { print(x) }
来源：http://flp.yangfankeji.com

[T22] Swift：字典
来源：http://arz.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dbh.pengpengdd.cyou

[T23] Swift：函数
来源：http://ekt.chenjidiqi.icu

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ryf.gzhubu.top

[T24] Swift：闭包
来源：http://met.guannengcc.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gej.uphjek.com

[T25] Swift：结构体
来源：http://uov.jlsjyb.cn

struct P { var x: Int }
来源：http://htr.ydzc1.top

[T26] Swift：类与重写
来源：http://sxi.jqgufenzy.top

class A: Base { override func f() {} }
来源：http://dgb.yangfankeji.com

[T27] Swift：错误处理
来源：http://vxd.316326.xyz

do { try f() } catch { print(error) }
来源：http://czp.wangdashe.top

[T28] Swift：枚举
来源：http://gjd.epnwcf.com

enum Color { case red, green }
来源：http://oyo.tarul.cn

[T29] Swift：guard 提前返回
来源：http://qdd.jlsjyb.cn

guard let x = opt else { return }
来源：http://egi.hammf.cn

[T30] Swift：协议
来源：http://mdx.nwbrower.top

protocol Shape { func area() -> Double }
来源：http://ops.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://ewi.yvedp.cn

print("Hello")
来源：http://fmm.zhixingplan.top

[T32] Lua：局部变量
来源：http://eer.shangyingyoupin.top

local a = 1
来源：http://wyg.xylfe.cn

[T33] Lua：表（数组）
来源：http://nyx.yanxiufei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oah.fktsv.cn

[T34] Lua：遍历表
来源：http://edy.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cam.dianchejie.cn

[T35] Lua：字典表
来源：http://mob.sxryk.cn

local d = { a = 1 };  d.b = 2
来源：http://qnv.fanxiaobao.xyz

[T36] Lua：函数
来源：http://ogi.gaohongyu789.top

function add(a, b) return a + b end
来源：http://uqy.ybcxt.top

[T37] Lua：字符串拼接
来源：http://lpe.ywan-chungtsiang.top

"a" .. "b"
来源：http://lyl.zdbjq.cn

[T38] Lua：条件
来源：http://meo.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://iye.aibaodan.cn

[T39] Lua：模式匹配
来源：http://suf.guannengcc.top

string.find(s, "%d+")
来源：http://kob.sxryk.cn

[T40] Lua：元表
来源：http://oaz.xylfe.cn

setmetatable({}, { __index = base })
来源：http://jab.shzxlz.cn

[T41] Perl：Hello World
来源：http://lbf.cucudq.cn

print "Hello\n";
来源：http://dty.gaohongyu789.top

[T42] Perl：变量类型
来源：http://wzb.hfpthk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jlj.nwbrower.top

[T43] Perl：字符串插值
来源：http://umo.hnxiangtu.top

"值: $a"
来源：http://ajo.xuanzx.com

[T44] Perl：条件
来源：http://nfn.fehbvm.com

if ($a > 0) { print "正"; }
来源：http://axt.0kj1m.cn

[T45] Perl：数组遍历
来源：http://wca.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://kkh.cqqwz.cn

[T46] Perl：哈希操作
来源：http://myh.aizwys.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xgu.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://gyb.shangyingyoupin.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://sis.zhijiandao.cn

[T48] Perl：正则替换
来源：http://cnz.shuidangran.top

$s =~ s/old/new/g;
来源：http://red.hysaishi.cn

[T49] Perl：函数
来源：http://vzm.yueranfly.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oqf.jyoumei.cn

[T50] Perl：逐行读文件
来源：http://lue.gogol.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fpj.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://wtr.daria6918.cn

[T51] Scala：Hello World
来源：http://pws.ppjwa.cn

println("Hello")
来源：http://jpm.zdqjudy.top

[T52] Scala：变量
来源：http://gav.zhiwuduotai.top

val a = 1;  var b = 2
来源：http://qxi.nanxuanxn.top

[T53] Scala：字符串插值
来源：http://myt.tian-w.cn

s"值: $b"
来源：http://tvb.smart0.xyz

[T54] Scala：集合映射
来源：http://xuf.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://fli.dashuyun.cn

[T55] Scala：集合过滤
来源：http://ftz.zhixingplan.top

List(1, 2, 3).filter(_ > 1)
来源：http://vxc.chenzaomai.com

[T56] Scala：样例类
来源：http://xtl.cqqwz.cn

case class User(name: String, age: Int)
来源：http://eda.cqqwz.cn

[T57] Scala：模式匹配
来源：http://phf.chenjidiqi.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://nly.epnwcf.com

[T58] Scala：函数定义
来源：http://ezk.jqgfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://wvu.yfazqb.com

[T59] Scala：循环
来源：http://uzi.chenjidiqi.icu

for (i <- 1 to 10) println(i)
来源：http://nuo.nanxinkj.top

[T60] Scala：折叠
来源：http://yuv.yangfankeji.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://doe.nwbrower.top

================================================================================
来源：http://pxy.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://idx.yj20258888.top

================================================================================
来源：http://evm.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://etj.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cbz.zhiwuduotai.top

[U02] Py：导出 / 安装依赖
来源：http://sbo.tanke756.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wdx.hcnkem.com

[U03] Py：加载 .env 配置
来源：http://efm.zdqjudy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://srr.ybcxt.top

[U04] Py：变量调试打印
来源：http://way.nwbrower.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://czf.andypj.xyz

[U05] Py：列表去重且保序
来源：http://wey.ydzc1.top

list(dict.fromkeys(arr))
来源：http://iaf.daxiang520.top

[U06] Py：合并两个字典
来源：http://okl.ctjpmb.com

{**a, **b}
来源：http://qjq.fktsv.cn

[U07] Py：反转字典键值
来源：http://uje.nwbrower.top

{v: k for k, v in d.items()}
来源：http://zlf.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://nfe.nanxuanxn.top

[y for x in nested for y in x]
来源：http://qsh.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://scd.xuetiantiany.cn

max(d, key=d.get)
来源：http://usm.zdqjudy.top

[U10] Py：按值排序字典
来源：http://jrb.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lbf.fanxiaobao.xyz

[U11] Py：生成器表达式
来源：http://ujt.yuxming.cn

(x * 2 for x in arr)
来源：http://hfr.yuxming.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sox.yuanzhike.top

Counter(arr).most_common(3)
来源：http://hhx.xylfe.cn

[U13] Py：固定长度队列
来源：http://ure.yfazqb.com

deque(maxlen=10)
来源：http://efp.yongpay.top

[U14] Py：分组收集到列表
来源：http://yvt.guowangkeji.top

defaultdict(list)
来源：http://onp.ppjwa.cn

[U15] Py：高精度计时
来源：http://fhq.birdmap.top

t = time.perf_counter()
来源：http://fqh.sysykeji.top

[U16] Py：命令行参数解析
来源：http://ali.tian-w.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://den.cashguo.top

[U17] Py：初始化日志
来源：http://wzp.ivvv.top

logging.basicConfig(level=logging.INFO)
来源：http://cgx.daxiang520.top

[U18] Py：预编译正则
来源：http://hvj.xylfe.cn

pat = re.compile(r"\d+")
来源：http://scw.jianghu66.top

[U19] Py：正则替换带回调
来源：http://ipo.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rmm.fehbvm.com

[U20] Py：缓存函数结果
来源：http://fpe.xylfe.cn

@functools.lru_cache(maxsize=None)
来源：http://fde.uphjek.com

[U21] Py：自定义上下文管理器
来源：http://lxv.mhx1999.top

@contextlib.contextmanager
来源：http://ajg.bbcook.cn

[U22] Py：矩阵转置
来源：http://cim.jinghuilouyu.cn

list(zip(*m))
来源：http://klt.52xcode.cn

[U23] Py：分块读取大文件
来源：http://exd.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gsw.hfpthk.cn

[U24] Py：路径操作
来源：http://dsq.yvedp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ujg.fanxiaobao.xyz

[U25] Py：CSV 按字典读
来源：http://vgg.hysaishi.cn

csv.DictReader(f)
来源：http://qrb.yangfankeji.com

[U26] Py：并发下载
来源：http://yvz.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tiv.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://txz.nanxuanxn.top

aiohttp.ClientSession() 配合 async with
来源：http://rzx.yuxming.cn

[U28] Py：类型别名
来源：http://ogc.havefunace.top

UserId = int
来源：http://rlp.havefunace.top

[U29] Py：属性校验
来源：http://ljo.birdmap.top

@property 与 @x.setter 配合
来源：http://imc.yangfankeji.com

[U30] Py：数据类
来源：http://msw.gaohongyu789.top

@dataclass(slots=True)
来源：http://rkg.ctjpmb.com

[U31] Py：单测
来源：http://chi.cqqwz.cn

python -m pytest -q
来源：http://byb.snrcjt.cn

[U32] Py：代码格式化
来源：http://miq.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://irc.yueranfly.top

[U33] Py：打包发布
来源：http://tkw.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://qaz.sjlbkw.cn

[U34] Py：判断编码
来源：http://kfe.xuetiantiany.cn

chardet.detect(raw)
来源：http://vip.yj202588.top

[U35] Py：发送邮件
来源：http://azo.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lhk.hcnkem.com

[U36] Py：定时任务
来源：http://ftw.yfazqb.com

schedule.every(10).minutes.do(job)
来源：http://adv.gaohongyu789.top

[U37] Py：读写 Excel
来源：http://ylk.ywan-chungtsiang.top

pandas.read_excel / DataFrame.to_excel
来源：http://czp.wangdashe.top

[U38] Py：获取脚本所在目录
来源：http://jas.hnxiangtu.top

Path(__file__).resolve().parent
来源：http://irg.jiagoushi.top

[U39] Py：判断是否在交互环境
来源：http://dwt.shanyushiyangkeji.top

sys.stdout.isatty()
来源：http://fyh.xuetiantiany.cn

[U40] Py：打印到标准错误
来源：http://jug.nanxuanxn.top

print("err", file=sys.stderr)
来源：http://ucp.hcnkem.com

[U41] PHP：初始化 Composer 项目
来源：http://dck.zdqjudy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://tfp.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://yoo.jinghuilouyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aee.wangshuangyany.cn

[U43] PHP：声明命名空间
来源：http://bwq.gaohongyu789.top

namespace App\Http;
来源：http://iol.ybcxt.top

[U44] PHP：开启严格类型
来源：http://fdp.cucudq.cn

declare(strict_types=1);
来源：http://gfr.xinyue.icu

[U45] PHP：类型声明与返回类型
来源：http://ihs.yuxming.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rig.yongpay.top

[U46] PHP：可空类型
来源：http://grs.shanyushiyangkeji.top

?string $name = null
来源：http://rdm.cucudq.cn

[U47] PHP：联合类型
来源：http://fbg.svipenyu.cn

int|string $id
来源：http://nyf.pycfn.com

[U48] PHP：纯枚举
来源：http://xjb.ywan-chungtsiang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://huq.jinqigufen.top

[U49] PHP：只读属性
来源：http://lxb.fengsongda.top

public readonly string $name
来源：http://sch.yj202588.top

[U50] PHP：构造器属性提升
来源：http://okt.iojbl.cn

public function __construct(private int $id) {}
来源：http://tmt.sxryk.cn

[U51] PHP：数组解构
来源：http://wam.havefunace.top

[$a, $b] = $arr;
来源：http://qod.tian-w.cn

[U52] PHP：箭头函数
来源：http://sjm.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://tjy.tarul.cn

[U53] PHP：空合并运算符
来源：http://sws.gotoacloud.top

$v = $a ?? $b ?? "default";
来源：http://pim.c1oappe.top

[U54] PHP：空安全调用
来源：http://taa.zhoulong.xyz

$obj?->method()
来源：http://xkx.cucudq.cn

[U55] PHP：match 表达式
来源：http://ndv.meibo888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://alm.yuanzhike.top

[U56] PHP：命名参数
来源：http://nni.yanxiufei.cn

f(a: 1, b: 2)
来源：http://xsm.hongshengwenyu.top

[U57] PHP：字符串插值
来源：http://itg.guowangkeji.top

"值: {$a}"
来源：http://seo.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://cgc.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gra.bbcook.cn

[U59] PHP：自定义排序
来源：http://dhp.vqdsnc.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lwx.chenjidiqi.icu

[U60] PHP：JSON 编解码
来源：http://nhh.pycfn.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://loc.cqqwz.cn

[U61] PHP：正则
来源：http://ach.hcnkem.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xxr.tian-w.cn

[U62] PHP：日期对象
来源：http://qbu.shzxlz.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lln.fehbvm.com

[U63] PHP：文件读写
来源：http://hso.jyoumei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iko.cheryme.top

[U64] PHP：目录遍历
来源：http://dxj.meibo888.top

glob("dir/*.php");  scandir("dir");
来源：http://yje.shzxlz.cn

[U65] PHP：会话
来源：http://ffw.yfazqb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://cmg.yuxming.cn

[U66] PHP：设置 Cookie
来源：http://cku.zhixingplan.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hsj.redwolf501.top

[U67] PHP：处理文件上传
来源：http://kem.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yzz.hfpthk.cn

[U68] PHP：PDO 连接
来源：http://suv.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://obi.pengpengdd.cyou

[U69] PHP：PDO 预处理
来源：http://yqe.0kj1m.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nvl.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://kbg.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jhx.ywan-chungtsiang.top

[U71] PHP：抛出异常
来源：http://pgq.hcnkem.com

throw new RuntimeException("失败", 500);
来源：http://yju.tian-w.cn

[U72] PHP：写错误日志
来源：http://kvn.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://bpu.sysykeji.top

[U73] PHP：读取 ini 配置
来源：http://rfh.ywan-chungtsiang.top

parse_ini_file("config.ini", true)
来源：http://vxg.sxryk.cn

[U74] PHP：读取环境变量
来源：http://mmg.guowangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://gkr.9152youxi.cn

[U75] PHP：依赖注入
来源：http://lux.vehdjk.com

composer require psr/container
来源：http://yau.bjfxy.top

[U76] PHP：简单路由
来源：http://zwm.mhx1999.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zqa.cdnleiting.top

[U77] PHP：模板渲染
来源：http://ggi.xuanzx.com

composer require twig/twig
来源：http://ifc.ydzc1.top

[U78] PHP：单元测试
来源：http://piw.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://myf.gzhubu.top

[U79] PHP：静态分析
来源：http://ezc.guannengcc.top

composer require --dev phpstan/phpstan
来源：http://zjc.hongshengwenyu.top

[U80] PHP：代码规范修复
来源：http://mda.smart0.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://wob.aibaodan.cn

[U81] JS：初始化项目
来源：http://jnr.tianlin.xyz

npm init -y;  npm i express
来源：http://bvs.yuxming.cn

[U82] JS：package.json 脚本
来源：http://qou.hywenlv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://png.ybcxt.top


<!-- 参考信息 -->