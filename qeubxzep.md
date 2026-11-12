代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://cim.sjlbkw.cn

[S59] C++：静态断言
来源：http://ilp.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bxj.gaohongyu789.top

[S60] C++：遍历并删除元素
来源：http://iqx.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://slu.uphjek.com

================================================================================
来源：http://ecc.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zpc.zhaomingkeji.xyz

================================================================================
来源：http://dhj.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://xbw.zdqjudy.top

println("Hello")
来源：http://cco.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://mlz.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mje.316326.xyz

[T03] Kotlin：字符串模板
来源：http://axz.hcnkem.com

"值: $b"
来源：http://ydo.guowangkeji.top

[T04] Kotlin：空安全
来源：http://ovk.0kj1m.cn

val n: String? = null;  n?.length
来源：http://prh.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://xwi.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vmt.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://fgq.haohaochexian.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jzz.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://bae.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kze.pengpengdd.cyou

[T08] Kotlin：数据类
来源：http://okj.ydjk.org.cn

data class User(val name: String, val age: Int)
来源：http://xhn.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://jtq.daxiang520.top

fun String.exclaim() = this + "!"
来源：http://isp.xinyue.icu

[T10] Kotlin：默认参数
来源：http://oqa.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kvp.havefunace.top

[T11] Kotlin：协程
来源：http://ylk.wangshuangyany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ilc.epnwcf.com

[T12] Kotlin：解构声明
来源：http://xyf.fengsongda.top

val (a, b) = Pair(1, 2)
来源：http://jnf.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://evp.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://ett.sjlbkw.cn

[T14] Kotlin：循环
来源：http://twc.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://rhg.yvedp.cn

[T15] Kotlin：接口
来源：http://mpq.jlsjyb.cn

interface Shape { fun area(): Double }
来源：http://ugv.guowangkeji.top

[T16] Swift：Hello World
来源：http://lci.daxiang520.top

print("Hello")
来源：http://yai.hcnkem.com

[T17] Swift：变量与常量
来源：http://okm.daxiang520.top

var a = 1;  let b = 2
来源：http://ddy.guannengcc.top

[T18] Swift：字符串插值
来源：http://wvt.sxryk.cn

"值: \(b)"
来源：http://gvw.fktsv.cn

[T19] Swift：可选绑定
来源：http://sus.meibo888.top

if let n = opt { print(n) }
来源：http://fmm.chenjidiqi.icu

[T20] Swift：数组操作
来源：http://rew.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://iqu.tian-w.cn

[T21] Swift：遍历
来源：http://yro.chenzaomai.com

for x in a { print(x) }
来源：http://pnm.sweek.top

[T22] Swift：字典
来源：http://cim.xuanzx.com

var d = ["a": 1];  d["b"] = 2
来源：http://cxq.yuxming.cn

[T23] Swift：函数
来源：http://oor.quarkkingdee.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cpx.hammf.cn

[T24] Swift：闭包
来源：http://anw.bjfxy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xet.zdbjq.cn

[T25] Swift：结构体
来源：http://lrx.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://sor.jiagoushi.top

[T26] Swift：类与重写
来源：http://nrz.pycfn.com

class A: Base { override func f() {} }
来源：http://aoc.gogol.net.cn

[T27] Swift：错误处理
来源：http://kfx.xziqi.cn

do { try f() } catch { print(error) }
来源：http://ikh.tarul.cn

[T28] Swift：枚举
来源：http://dqz.yuanzhike.top

enum Color { case red, green }
来源：http://kls.yueranfly.top

[T29] Swift：guard 提前返回
来源：http://txy.ppjwa.cn

guard let x = opt else { return }
来源：http://izu.gaohongyu789.top

[T30] Swift：协议
来源：http://bes.yueranfly.top

protocol Shape { func area() -> Double }
来源：http://vot.snrcjt.cn

[T31] Lua：Hello World
来源：http://pld.gzhubu.top

print("Hello")
来源：http://fup.jiagoushi.top

[T32] Lua：局部变量
来源：http://nxc.jianghu66.top

local a = 1
来源：http://zyd.ppjwa.cn

[T33] Lua：表（数组）
来源：http://cwe.zhaomingkeji.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://lfk.fktsv.cn

[T34] Lua：遍历表
来源：http://xlu.zhongyouzk.top

for i, v in ipairs(t) do print(i, v) end
来源：http://aqq.uphjek.com

[T35] Lua：字典表
来源：http://qpn.quarkkingdee.top

local d = { a = 1 };  d.b = 2
来源：http://zof.fzhhl.top

[T36] Lua：函数
来源：http://lrd.hcnkem.com

function add(a, b) return a + b end
来源：http://ste.redwolf501.top

[T37] Lua：字符串拼接
来源：http://zww.hnqzz.top

"a" .. "b"
来源：http://mvg.jinqigfzy.top

[T38] Lua：条件
来源：http://ioe.fzhhl.top

if x > 0 then print("正") end
来源：http://let.52xcode.cn

[T39] Lua：模式匹配
来源：http://viv.havefunace.top

string.find(s, "%d+")
来源：http://fkx.jinyuanbaomall.cn

[T40] Lua：元表
来源：http://tpk.yonumen.top

setmetatable({}, { __index = base })
来源：http://awo.zhoulong.xyz

[T41] Perl：Hello World
来源：http://ubf.yj20258888.top

print "Hello\n";
来源：http://iqq.yuxming.cn

[T42] Perl：变量类型
来源：http://zpj.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qdi.shanyushiyangkeji.top

[T43] Perl：字符串插值
来源：http://vqa.quarkkingdee.top

"值: $a"
来源：http://doz.jinyuanbaomall.cn

[T44] Perl：条件
来源：http://wum.chenzaomai.com

if ($a > 0) { print "正"; }
来源：http://ozy.zhixingplan.top

[T45] Perl：数组遍历
来源：http://uyr.cdnleiting.top

for my $x (@arr) { print $x; }
来源：http://fnp.ywan-chungtsiang.top

[T46] Perl：哈希操作
来源：http://inw.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ptd.dashuyun.cn

[T47] Perl：正则捕获
来源：http://gfy.cdnleiting.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vyd.pycfn.com

[T48] Perl：正则替换
来源：http://ixa.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://iha.hnqzz.top

[T49] Perl：函数
来源：http://lyn.cucudq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eno.ybcxt.top

[T50] Perl：逐行读文件
来源：http://grm.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hob.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://ghf.haohaochexian.top

[T51] Scala：Hello World
来源：http://lls.52xcode.cn

println("Hello")
来源：http://pli.sysykeji.top

[T52] Scala：变量
来源：http://ser.ybcxt.top

val a = 1;  var b = 2
来源：http://ysf.ydjk.org.cn

[T53] Scala：字符串插值
来源：http://ziy.tianlin.xyz

s"值: $b"
来源：http://yuz.xingfuxueyuan.xyz

[T54] Scala：集合映射
来源：http://xdg.fanxiaobao.xyz

List(1, 2, 3).map(_ * 2)
来源：http://fxx.jiagoushi.top

[T55] Scala：集合过滤
来源：http://zzb.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nit.zhongyouzk.top

[T56] Scala：样例类
来源：http://bqh.fzhhl.top

case class User(name: String, age: Int)
来源：http://qgh.nwbrower.top

[T57] Scala：模式匹配
来源：http://trw.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://irf.yj202588.top

[T58] Scala：函数定义
来源：http://rdh.snrcjt.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kna.xylfe.cn

[T59] Scala：循环
来源：http://jjz.ehwqpu.com

for (i <- 1 to 10) println(i)
来源：http://fws.jqgufenzy.top

[T60] Scala：折叠
来源：http://jrp.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ffs.nanxinkj.top

================================================================================
来源：http://nvz.ctjpmb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fhe.snrcjt.cn

================================================================================
来源：http://rwp.zhiwuduotai.top

[U01] Py：创建虚拟环境
来源：http://kxy.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://gim.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://fgy.quarkkingdee.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ibo.zhoulong.xyz

[U03] Py：加载 .env 配置
来源：http://fke.ydjk.org.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pqe.quarkkingdee.top

[U04] Py：变量调试打印
来源：http://ezu.vehdjk.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rpo.zdbjq.cn

[U05] Py：列表去重且保序
来源：http://vck.xziqi.cn

list(dict.fromkeys(arr))
来源：http://wqk.quarkkingdee.top

[U06] Py：合并两个字典
来源：http://srf.guowangkeji.top

{**a, **b}
来源：http://wlf.quarkkingdee.top

[U07] Py：反转字典键值
来源：http://vui.hongshengwenyu.top

{v: k for k, v in d.items()}
来源：http://ddg.bbcook.cn

[U08] Py：展平二维列表
来源：http://odr.pycfn.com

[y for x in nested for y in x]
来源：http://enx.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://jxg.gzhubu.top

max(d, key=d.get)
来源：http://ybg.hnqzz.top

[U10] Py：按值排序字典
来源：http://hqg.gzhubu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://syr.jqgfzy.top

[U11] Py：生成器表达式
来源：http://doq.feifeiyinyue.top

(x * 2 for x in arr)
来源：http://kfk.ybcxt.top

[U12] Py：取出现最多的 3 个元素
来源：http://pdj.smart0.xyz

Counter(arr).most_common(3)
来源：http://yrx.gogol.net.cn

[U13] Py：固定长度队列
来源：http://ugg.xylfe.cn

deque(maxlen=10)
来源：http://zli.yonumen.top

[U14] Py：分组收集到列表
来源：http://oyh.ehwqpu.com

defaultdict(list)
来源：http://kfj.sufxvd.cn

[U15] Py：高精度计时
来源：http://wgz.wangdashe.top

t = time.perf_counter()
来源：http://tfo.hammf.cn

[U16] Py：命令行参数解析
来源：http://lhu.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kmx.xinyue.icu

[U17] Py：初始化日志
来源：http://vki.zdqjudy.top

logging.basicConfig(level=logging.INFO)
来源：http://dpl.jinghuilouyu.cn

[U18] Py：预编译正则
来源：http://jmg.svipenyu.cn

pat = re.compile(r"\d+")
来源：http://kyp.xuetiantiany.cn

[U19] Py：正则替换带回调
来源：http://xzx.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zko.tarul.cn

[U20] Py：缓存函数结果
来源：http://csi.sxryk.cn

@functools.lru_cache(maxsize=None)
来源：http://ukj.tianlin.xyz

[U21] Py：自定义上下文管理器
来源：http://csf.nanxinkj.top

@contextlib.contextmanager
来源：http://zrg.chenjidiqi.icu

[U22] Py：矩阵转置
来源：http://brl.xylfe.cn

list(zip(*m))
来源：http://nox.zhiwuduotai.top

[U23] Py：分块读取大文件
来源：http://ztr.cucudq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mlh.havefunace.top

[U24] Py：路径操作
来源：http://vrt.hcnkem.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ocv.vqdsnc.cn

[U25] Py：CSV 按字典读
来源：http://dsb.sweek.top

csv.DictReader(f)
来源：http://ccm.316326.xyz

[U26] Py：并发下载
来源：http://zxn.yuanzhike.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://srs.hfpthk.cn

[U27] Py：异步 HTTP
来源：http://uld.sweek.top

aiohttp.ClientSession() 配合 async with
来源：http://dej.zhoulong.xyz

[U28] Py：类型别名
来源：http://bmw.gaohongyu789.top

UserId = int
来源：http://bub.cqqwz.cn

[U29] Py：属性校验
来源：http://cmo.aizwys.cn

@property 与 @x.setter 配合
来源：http://qab.hnxiangtu.top

[U30] Py：数据类
来源：http://xmg.jianghu66.top

@dataclass(slots=True)
来源：http://lgd.gaohongyu789.top

[U31] Py：单测
来源：http://nvs.aibaodan.cn

python -m pytest -q
来源：http://utj.dashuyun.cn

[U32] Py：代码格式化
来源：http://kxh.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://dhb.gotoacloud.top

[U33] Py：打包发布
来源：http://xfz.sufxvd.cn

python -m build  （依赖 pyproject.toml）
来源：http://wxd.shuidangran.top

[U34] Py：判断编码
来源：http://uso.snrcjt.cn

chardet.detect(raw)
来源：http://ffb.haohaochexian.top

[U35] Py：发送邮件
来源：http://okh.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gja.fktsv.cn

[U36] Py：定时任务
来源：http://ejb.nanxinkj.top

schedule.every(10).minutes.do(job)
来源：http://pqc.cheryme.top

[U37] Py：读写 Excel
来源：http://xrg.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wkw.nanxuanxn.top

[U38] Py：获取脚本所在目录
来源：http://onx.ehwqpu.com

Path(__file__).resolve().parent
来源：http://imb.feifeiyinyue.top

[U39] Py：判断是否在交互环境
来源：http://iqk.xuanzx.com

sys.stdout.isatty()
来源：http://jvm.zhaomingkeji.xyz

[U40] Py：打印到标准错误
来源：http://abv.xinyue.icu

print("err", file=sys.stderr)
来源：http://irm.xuanzx.com

[U41] PHP：初始化 Composer 项目
来源：http://ubp.yj20258888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xfg.snrcjt.cn

[U42] PHP：PSR-4 自动加载
来源：http://dml.daria6918.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://voj.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://vtk.hnxiangtu.top

namespace App\Http;
来源：http://qwm.gogol.net.cn

[U44] PHP：开启严格类型
来源：http://uha.ehwqpu.com

declare(strict_types=1);
来源：http://ejb.zhengqikj.top

[U45] PHP：类型声明与返回类型
来源：http://zjk.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://jri.hesvh.cn

[U46] PHP：可空类型
来源：http://bbk.quarkkingdee.top

?string $name = null
来源：http://axz.vehdjk.com

[U47] PHP：联合类型
来源：http://oea.zhoulong.xyz

int|string $id
来源：http://ssj.hysaishi.cn

[U48] PHP：纯枚举
来源：http://fhl.ywan-chungtsiang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://irh.hammf.cn

[U49] PHP：只读属性
来源：http://kgp.c1oappe.top

public readonly string $name
来源：http://rny.tarul.cn

[U50] PHP：构造器属性提升
来源：http://jgc.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://opq.snrcjt.cn

[U51] PHP：数组解构
来源：http://mxq.316326.xyz

[$a, $b] = $arr;
来源：http://boh.xziqi.cn

[U52] PHP：箭头函数
来源：http://aqo.316326.xyz

$double = fn($x) => $x * 2;
来源：http://zyj.316326.xyz

[U53] PHP：空合并运算符
来源：http://idl.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://qdq.meibo888.top

[U54] PHP：空安全调用
来源：http://ogf.aizwys.cn

$obj?->method()
来源：http://dky.ctjpmb.com

[U55] PHP：match 表达式
来源：http://uqd.xingfuxueyuan.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fyo.cqqwz.cn

[U56] PHP：命名参数
来源：http://mpq.gaohongyu789.top

f(a: 1, b: 2)
来源：http://nos.shuidangran.top

[U57] PHP：字符串插值
来源：http://eqz.hywenlv.cn

"值: {$a}"
来源：http://hnn.vqdsnc.cn

[U58] PHP：数组三件套
来源：http://dfg.pycfn.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gbw.shuidangran.top

[U59] PHP：自定义排序
来源：http://sso.sweek.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fgy.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://ifc.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vmt.uphjek.com

[U61] PHP：正则
来源：http://fpv.uphjek.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mys.aibaodan.cn

[U62] PHP：日期对象
来源：http://gct.smart0.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cmm.xylfe.cn

[U63] PHP：文件读写
来源：http://grn.yanxiufei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iwo.c1oappe.top

[U64] PHP：目录遍历
来源：http://djy.havefunace.top

glob("dir/*.php");  scandir("dir");
来源：http://efp.jlsjyb.cn

[U65] PHP：会话
来源：http://byj.kuanghao11.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jfo.sufxvd.cn

[U66] PHP：设置 Cookie
来源：http://zcl.ywan-chungtsiang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vhc.shanyushiyangkeji.top

[U67] PHP：处理文件上传
来源：http://wxr.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ezj.ydjk.org.cn

[U68] PHP：PDO 连接
来源：http://sff.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dqe.daxiang520.top

[U69] PHP：PDO 预处理
来源：http://nyi.hnqzz.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kvx.fktsv.cn

[U70] PHP：PDO 事务
来源：http://ere.fzhhl.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rwp.svipenyu.cn

[U71] PHP：抛出异常
来源：http://uyk.tian-w.cn

throw new RuntimeException("失败", 500);
来源：http://dab.vqdsnc.cn

[U72] PHP：写错误日志
来源：http://amh.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://ztg.gaohongyu789.top

[U73] PHP：读取 ini 配置
来源：http://hvk.gzhubu.top

parse_ini_file("config.ini", true)
来源：http://lyd.shanyushiyangtech.top

[U74] PHP：读取环境变量
来源：http://qyl.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://yae.daxiang520.top

[U75] PHP：依赖注入
来源：http://vnd.jlsjyb.cn

composer require psr/container
来源：http://fyz.svipenyu.cn

[U76] PHP：简单路由
来源：http://akq.vehdjk.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://igr.jinqigfzy.top

[U77] PHP：模板渲染
来源：http://hqd.iojbl.cn

composer require twig/twig
来源：http://aco.chenlongwang.top

[U78] PHP：单元测试
来源：http://xvv.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://ozc.gogol.net.cn

[U79] PHP：静态分析
来源：http://gcp.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://yhq.nwbrower.top

[U80] PHP：代码规范修复
来源：http://mfi.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bzy.zdqjudy.top

[U81] JS：初始化项目
来源：http://glq.aizwys.cn

npm init -y;  npm i express
来源：http://ram.jinqigufen.top

[U82] JS：package.json 脚本
来源：http://hgo.havefunace.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://epn.hongshengwenyu.top

[U83] JS：ES Module 导入导出
来源：http://chy.yj202588.top

export const a = 1;  import { a } from "./m.js";
来源：http://kpo.zycfv.cn

[U84] JS：CommonJS 写法
来源：http://acb.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dfk.cqqwz.cn


<!-- 参考信息 -->