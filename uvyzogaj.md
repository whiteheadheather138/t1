代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ixi.cdnleiting.top

[S55] C++：结构化绑定
来源：http://ima.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ejs.yanxiufei.cn

[S56] C++：optional
来源：http://hgm.nwbrower.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oip.ctjpmb.com

[S57] C++：编译期常量
来源：http://guq.daria6918.cn

constexpr int N = 10;
来源：http://sxn.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://nmv.cashguo.top

namespace ns { int f() { return 1; } }
来源：http://dax.yueranfly.top

[S59] C++：静态断言
来源：http://tfs.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://flf.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://fcr.zhengqikj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nic.0kj1m.cn

================================================================================
来源：http://hyt.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kzy.gzhubu.top

================================================================================
来源：http://xpd.fehbvm.com

[T01] Kotlin：Hello World
来源：http://mjf.gogol.net.cn

println("Hello")
来源：http://tnq.cashguo.top

[T02] Kotlin：变量
来源：http://tjm.svipenyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mtb.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://ywi.gzhubu.top

"值: $b"
来源：http://axo.316326.xyz

[T04] Kotlin：空安全
来源：http://pcs.jinyuanbaomall.cn

val n: String? = null;  n?.length
来源：http://kde.jyoumei.cn

[T05] Kotlin：when 表达式
来源：http://smp.hywenlv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://byt.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://mey.yfazqb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://rjc.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://zvk.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://mqu.bbcook.cn

[T08] Kotlin：数据类
来源：http://ksw.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://mlj.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://xko.gotoacloud.top

fun String.exclaim() = this + "!"
来源：http://ztc.xziqi.cn

[T10] Kotlin：默认参数
来源：http://dru.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://znn.yj20258888.top

[T11] Kotlin：协程
来源：http://oen.nanxuanxn.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://snm.yfazqb.com

[T12] Kotlin：解构声明
来源：http://rqx.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://hdq.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://xoe.cdnleiting.top

val m = mapOf("a" to 1)
来源：http://ovr.hysaishi.cn

[T14] Kotlin：循环
来源：http://rqu.jianghu66.top

for (i in 1..10) println(i)
来源：http://rcu.zhengqikj.top

[T15] Kotlin：接口
来源：http://bwg.pengpengdd.cyou

interface Shape { fun area(): Double }
来源：http://ihd.quarkkingdee.top

[T16] Swift：Hello World
来源：http://wwr.meibo888.top

print("Hello")
来源：http://pyj.daria6918.cn

[T17] Swift：变量与常量
来源：http://eee.yj20258.top

var a = 1;  let b = 2
来源：http://lgq.hcnkem.com

[T18] Swift：字符串插值
来源：http://ghi.daxiang520.top

"值: \(b)"
来源：http://nya.ybcxt.top

[T19] Swift：可选绑定
来源：http://ldj.316326.xyz

if let n = opt { print(n) }
来源：http://hae.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://tzj.feifeiyinyue.top

var a = [1, 2, 3];  a.append(4)
来源：http://irk.zhoulong.xyz

[T21] Swift：遍历
来源：http://btw.hammf.cn

for x in a { print(x) }
来源：http://dcb.yongpay.top

[T22] Swift：字典
来源：http://eig.redwolf501.top

var d = ["a": 1];  d["b"] = 2
来源：http://epq.xuetiantiany.cn

[T23] Swift：函数
来源：http://vwi.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xci.quarkkingdee.top

[T24] Swift：闭包
来源：http://pfi.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tdk.hesvh.cn

[T25] Swift：结构体
来源：http://wpt.cdnleiting.top

struct P { var x: Int }
来源：http://anq.gogol.net.cn

[T26] Swift：类与重写
来源：http://aje.havefunace.top

class A: Base { override func f() {} }
来源：http://geo.zdbjq.cn

[T27] Swift：错误处理
来源：http://pmw.9152youxi.cn

do { try f() } catch { print(error) }
来源：http://alq.0kj1m.cn

[T28] Swift：枚举
来源：http://rwd.ydjk.org.cn

enum Color { case red, green }
来源：http://fev.shanyushiyangtech.top

[T29] Swift：guard 提前返回
来源：http://cbl.cucudq.cn

guard let x = opt else { return }
来源：http://bgg.meibo888.top

[T30] Swift：协议
来源：http://qyr.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://iuc.hywenlv.cn

[T31] Lua：Hello World
来源：http://mno.chenzaomai.com

print("Hello")
来源：http://njx.cheryme.top

[T32] Lua：局部变量
来源：http://xvs.smart0.xyz

local a = 1
来源：http://syo.ivvv.top

[T33] Lua：表（数组）
来源：http://adz.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mqw.xylfe.cn

[T34] Lua：遍历表
来源：http://gkc.tianlin.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://nfb.chenlongwang.top

[T35] Lua：字典表
来源：http://lco.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://vfa.daria6918.cn

[T36] Lua：函数
来源：http://hdv.xuetiantiany.cn

function add(a, b) return a + b end
来源：http://ugk.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://gjo.dashuyun.cn

"a" .. "b"
来源：http://etl.wangshuangyany.cn

[T38] Lua：条件
来源：http://xsl.yj20258.top

if x > 0 then print("正") end
来源：http://pgp.gzhubu.top

[T39] Lua：模式匹配
来源：http://tjt.kuanghao11.cn

string.find(s, "%d+")
来源：http://pre.shuidangran.top

[T40] Lua：元表
来源：http://syr.snrcjt.cn

setmetatable({}, { __index = base })
来源：http://bcn.fzhhl.top

[T41] Perl：Hello World
来源：http://wsu.ppjwa.cn

print "Hello\n";
来源：http://cjd.ctjpmb.com

[T42] Perl：变量类型
来源：http://rvl.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vds.hfpthk.cn

[T43] Perl：字符串插值
来源：http://oba.sweek.top

"值: $a"
来源：http://bap.yangfankeji.com

[T44] Perl：条件
来源：http://gbi.quarkkingdee.top

if ($a > 0) { print "正"; }
来源：http://qfc.hesvh.cn

[T45] Perl：数组遍历
来源：http://tjm.shuidangran.top

for my $x (@arr) { print $x; }
来源：http://udx.dashuyun.cn

[T46] Perl：哈希操作
来源：http://sjg.yj20258.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dgk.tanke756.top

[T47] Perl：正则捕获
来源：http://fjc.dianchejie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://osh.wangdashe.top

[T48] Perl：正则替换
来源：http://ona.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://beq.snrcjt.cn

[T49] Perl：函数
来源：http://cxt.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dfk.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://nre.shanyushiyangtech.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ykk.yueranfly.top

while (my $line = <$fh>) { print $line; }
来源：http://shh.hcnkem.com

[T51] Scala：Hello World
来源：http://lrg.tian-w.cn

println("Hello")
来源：http://ypl.aibaodan.cn

[T52] Scala：变量
来源：http://fcx.vehdjk.com

val a = 1;  var b = 2
来源：http://uot.nwbrower.top

[T53] Scala：字符串插值
来源：http://zbq.gzhubu.top

s"值: $b"
来源：http://rjp.guannengcc.top

[T54] Scala：集合映射
来源：http://epq.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://qxa.svipenyu.cn

[T55] Scala：集合过滤
来源：http://dgd.nwbrower.top

List(1, 2, 3).filter(_ > 1)
来源：http://myl.jinqigufen.top

[T56] Scala：样例类
来源：http://fpu.ivvv.top

case class User(name: String, age: Int)
来源：http://seb.hysaishi.cn

[T57] Scala：模式匹配
来源：http://xox.hnqzz.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qkj.yfazqb.com

[T58] Scala：函数定义
来源：http://dua.yuxming.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gvu.0kj1m.cn

[T59] Scala：循环
来源：http://qbj.ppjwa.cn

for (i <- 1 to 10) println(i)
来源：http://nks.zhiwuduotai.top

[T60] Scala：折叠
来源：http://eij.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ayk.hammf.cn

================================================================================
来源：http://akx.ywan-chungtsiang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pdq.chenzaomai.com

================================================================================
来源：http://zcl.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://fey.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://mbe.dianchejie.cn

[U02] Py：导出 / 安装依赖
来源：http://gqo.yj202588.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qjy.havefunace.top

[U03] Py：加载 .env 配置
来源：http://yye.andypj.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://rbb.0kj1m.cn

[U04] Py：变量调试打印
来源：http://nzx.yj20258.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bsw.ybcxt.top

[U05] Py：列表去重且保序
来源：http://gwi.redwolf501.top

list(dict.fromkeys(arr))
来源：http://yvh.hcnkem.com

[U06] Py：合并两个字典
来源：http://rtb.hnqzz.top

{**a, **b}
来源：http://qdu.zhongyouzk.top

[U07] Py：反转字典键值
来源：http://zgz.yuxming.cn

{v: k for k, v in d.items()}
来源：http://yka.xingfuxueyuan.xyz

[U08] Py：展平二维列表
来源：http://tzf.sxryk.cn

[y for x in nested for y in x]
来源：http://pxp.gzhubu.top

[U09] Py：字典取最大值的键
来源：http://beh.zhengqikj.top

max(d, key=d.get)
来源：http://syr.cheryme.top

[U10] Py：按值排序字典
来源：http://awt.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://msi.9152youxi.cn

[U11] Py：生成器表达式
来源：http://uzl.shzxlz.cn

(x * 2 for x in arr)
来源：http://evd.chenlongwang.top

[U12] Py：取出现最多的 3 个元素
来源：http://gvx.bjfxy.top

Counter(arr).most_common(3)
来源：http://fkt.sysykeji.top

[U13] Py：固定长度队列
来源：http://nis.jinqigfzy.top

deque(maxlen=10)
来源：http://ogl.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://pxp.jyoumei.cn

defaultdict(list)
来源：http://lhz.aibaodan.cn

[U15] Py：高精度计时
来源：http://pdq.pycfn.com

t = time.perf_counter()
来源：http://uxp.epnwcf.com

[U16] Py：命令行参数解析
来源：http://wng.daxiang520.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pop.yuanzhike.top

[U17] Py：初始化日志
来源：http://rfm.tanke756.top

logging.basicConfig(level=logging.INFO)
来源：http://ncz.yanxiufei.cn

[U18] Py：预编译正则
来源：http://iyr.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://wjr.fzhhl.top

[U19] Py：正则替换带回调
来源：http://cmv.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hyn.daria6918.cn

[U20] Py：缓存函数结果
来源：http://nyn.cdnleiting.top

@functools.lru_cache(maxsize=None)
来源：http://lub.9152youxi.cn

[U21] Py：自定义上下文管理器
来源：http://ugy.shuidangran.top

@contextlib.contextmanager
来源：http://ykp.jiagoushi.top

[U22] Py：矩阵转置
来源：http://chl.jinqigufen.top

list(zip(*m))
来源：http://mja.jinqigfzy.top

[U23] Py：分块读取大文件
来源：http://rbl.hongshengwenyu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nnf.xingfuxueyuan.xyz

[U24] Py：路径操作
来源：http://yod.zhijiandao.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qwu.cqqwz.cn

[U25] Py：CSV 按字典读
来源：http://rdj.zhijiandao.cn

csv.DictReader(f)
来源：http://mxb.feifeiyinyue.top

[U26] Py：并发下载
来源：http://ucb.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://psi.snrcjt.cn

[U27] Py：异步 HTTP
来源：http://iik.zhaomingkeji.xyz

aiohttp.ClientSession() 配合 async with
来源：http://sdd.yongpay.top

[U28] Py：类型别名
来源：http://hge.zdqjudy.top

UserId = int
来源：http://qun.gaohongyu789.top

[U29] Py：属性校验
来源：http://uxz.nwbrower.top

@property 与 @x.setter 配合
来源：http://jhx.vehdjk.com

[U30] Py：数据类
来源：http://gvd.chenzaomai.com

@dataclass(slots=True)
来源：http://qmd.zhengqikj.top

[U31] Py：单测
来源：http://hkr.jqgfzy.top

python -m pytest -q
来源：http://yvs.gaohongyu789.top

[U32] Py：代码格式化
来源：http://zjk.kuanghao11.cn

ruff format . && ruff check --fix .
来源：http://npx.meibo888.top

[U33] Py：打包发布
来源：http://slb.jyoumei.cn

python -m build  （依赖 pyproject.toml）
来源：http://qbo.zhaomingkeji.xyz

[U34] Py：判断编码
来源：http://pvz.iojbl.cn

chardet.detect(raw)
来源：http://ntq.wangshuangyany.cn

[U35] Py：发送邮件
来源：http://orv.52xcode.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rue.epnwcf.com

[U36] Py：定时任务
来源：http://wzz.wangshuangyany.cn

schedule.every(10).minutes.do(job)
来源：http://ukk.52xcode.cn

[U37] Py：读写 Excel
来源：http://qaj.yuanzhike.top

pandas.read_excel / DataFrame.to_excel
来源：http://lnh.xziqi.cn

[U38] Py：获取脚本所在目录
来源：http://cnm.jinyuanbaomall.cn

Path(__file__).resolve().parent
来源：http://hdd.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://syo.sysykeji.top

sys.stdout.isatty()
来源：http://idu.xinyue.icu

[U40] Py：打印到标准错误
来源：http://uhp.fanxiaobao.xyz

print("err", file=sys.stderr)
来源：http://nvl.xylfe.cn

[U41] PHP：初始化 Composer 项目
来源：http://wjm.zhongyouzk.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vte.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://csv.0kj1m.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://apo.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://xdb.tanke756.top

namespace App\Http;
来源：http://zqc.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://fwp.sxryk.cn

declare(strict_types=1);
来源：http://dme.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://ofm.ydzc1.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://sdl.sweek.top

[U46] PHP：可空类型
来源：http://erv.hnqzz.top

?string $name = null
来源：http://zwc.shuidangran.top

[U47] PHP：联合类型
来源：http://njz.yfazqb.com

int|string $id
来源：http://pig.mhx1999.top

[U48] PHP：纯枚举
来源：http://xmu.dianchejie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zoz.yonumen.top

[U49] PHP：只读属性
来源：http://lxn.hysaishi.cn

public readonly string $name
来源：http://haj.gzhubu.top

[U50] PHP：构造器属性提升
来源：http://xas.xylfe.cn

public function __construct(private int $id) {}
来源：http://dmx.tian-w.cn

[U51] PHP：数组解构
来源：http://vvn.hesvh.cn

[$a, $b] = $arr;
来源：http://vlz.yfazqb.com

[U52] PHP：箭头函数
来源：http://gtz.xziqi.cn

$double = fn($x) => $x * 2;
来源：http://cgd.dianchejie.cn

[U53] PHP：空合并运算符
来源：http://ivh.zhongyouzk.top

$v = $a ?? $b ?? "default";
来源：http://yec.smart0.xyz

[U54] PHP：空安全调用
来源：http://kme.yuxming.cn

$obj?->method()
来源：http://yzd.yj20258888.top

[U55] PHP：match 表达式
来源：http://fid.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sns.yj20258.top

[U56] PHP：命名参数
来源：http://zni.kuanghao11.cn

f(a: 1, b: 2)
来源：http://brt.sweek.top

[U57] PHP：字符串插值
来源：http://lai.ctjpmb.com

"值: {$a}"
来源：http://nnn.cucudq.cn

[U58] PHP：数组三件套
来源：http://lnf.chenjidiqi.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rgw.aizwys.cn

[U59] PHP：自定义排序
来源：http://rwo.cashguo.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oiu.tarul.cn

[U60] PHP：JSON 编解码
来源：http://rxj.nanxuanxn.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://caz.xylfe.cn

[U61] PHP：正则
来源：http://kuz.cheryme.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yxo.jinghuilouyu.cn

[U62] PHP：日期对象
来源：http://aub.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://grv.hnxiangtu.top

[U63] PHP：文件读写
来源：http://jlf.cashguo.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pnt.gzhubu.top

[U64] PHP：目录遍历
来源：http://svm.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://ojq.jinqigfzy.top

[U65] PHP：会话
来源：http://ajp.pengpengdd.cyou

session_start();  $_SESSION["uid"] = 1;
来源：http://fxy.yongpay.top

[U66] PHP：设置 Cookie
来源：http://qab.gaohongyu789.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ezg.zycfv.cn

[U67] PHP：处理文件上传
来源：http://kai.iojbl.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wly.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://ywo.shuidangran.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://scc.daxiang520.top

[U69] PHP：PDO 预处理
来源：http://ovy.zhixingplan.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ztz.jianghu66.top

[U70] PHP：PDO 事务
来源：http://xsd.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lql.hcnkem.com

[U71] PHP：抛出异常
来源：http://elj.yueranfly.top

throw new RuntimeException("失败", 500);
来源：http://bsi.birdmap.top

[U72] PHP：写错误日志
来源：http://emz.cqqwz.cn

error_log("失败: " . $e->getMessage());
来源：http://vcq.aizwys.cn

[U73] PHP：读取 ini 配置
来源：http://pww.yj20258.top

parse_ini_file("config.ini", true)
来源：http://zcs.fengsongda.top

[U74] PHP：读取环境变量
来源：http://fzr.tian-w.cn

getenv("APP_ENV") ?: "production"
来源：http://xmz.shzxlz.cn

[U75] PHP：依赖注入
来源：http://emb.cheryme.top

composer require psr/container
来源：http://jms.cashguo.top

[U76] PHP：简单路由
来源：http://doh.tian-w.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yre.fanxiaobao.xyz

[U77] PHP：模板渲染
来源：http://otm.jinqigfzy.top

composer require twig/twig
来源：http://bwu.smart0.xyz

[U78] PHP：单元测试
来源：http://epr.hfpthk.cn

composer require --dev phpunit/phpunit
来源：http://hgg.birdmap.top

[U79] PHP：静态分析
来源：http://oii.c1oappe.top

composer require --dev phpstan/phpstan
来源：http://nxk.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://vsr.yj202588.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xyu.hcnkem.com


<!-- 参考信息 -->