代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wnt.ybcxt.top

[S55] C++：结构化绑定
来源：http://ule.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pps.daxiang520.top

[S56] C++：optional
来源：http://vac.dashuyun.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vvz.shanyushiyangkeji.top

[S57] C++：编译期常量
来源：http://tcb.tarul.cn

constexpr int N = 10;
来源：http://lyl.zdbjq.cn

[S58] C++：命名空间
来源：http://bwq.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://uta.hcnkem.com

[S59] C++：静态断言
来源：http://fip.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fqi.9152youxi.cn

[S60] C++：遍历并删除元素
来源：http://wfl.cdnleiting.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://daj.ydjk.org.cn

================================================================================
来源：http://yae.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hto.svipenyu.cn

================================================================================
来源：http://juh.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://wxz.fanxiaobao.xyz

println("Hello")
来源：http://fcf.zycfv.cn

[T02] Kotlin：变量
来源：http://xtd.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bur.fengsongda.top

[T03] Kotlin：字符串模板
来源：http://llg.xuanzx.com

"值: $b"
来源：http://hyq.ehwqpu.com

[T04] Kotlin：空安全
来源：http://qvy.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://yyn.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://fhy.smart0.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tyw.yj20258888.top

[T06] Kotlin：集合映射
来源：http://ajc.jinqigufen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ooq.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://mug.zhengqikj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uau.yueranfly.top

[T08] Kotlin：数据类
来源：http://trs.sweek.top

data class User(val name: String, val age: Int)
来源：http://dpw.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://mdc.gzhubu.top

fun String.exclaim() = this + "!"
来源：http://sew.ivvv.top

[T10] Kotlin：默认参数
来源：http://bjw.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://skc.daria6918.cn

[T11] Kotlin：协程
来源：http://jml.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cux.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://wej.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://zxj.9152youxi.cn

[T13] Kotlin：只读 Map
来源：http://xbk.chenlongwang.top

val m = mapOf("a" to 1)
来源：http://odd.xuanzx.com

[T14] Kotlin：循环
来源：http://ilp.yuxming.cn

for (i in 1..10) println(i)
来源：http://rxa.cdnleiting.top

[T15] Kotlin：接口
来源：http://wug.yongpay.top

interface Shape { fun area(): Double }
来源：http://ffp.redwolf501.top

[T16] Swift：Hello World
来源：http://ikj.sjlbkw.cn

print("Hello")
来源：http://cii.hcnkem.com

[T17] Swift：变量与常量
来源：http://its.sxryk.cn

var a = 1;  let b = 2
来源：http://hgj.gotoacloud.top

[T18] Swift：字符串插值
来源：http://etq.daria6918.cn

"值: \(b)"
来源：http://dfe.cqqwz.cn

[T19] Swift：可选绑定
来源：http://ihb.meibo888.top

if let n = opt { print(n) }
来源：http://grs.xinyue.icu

[T20] Swift：数组操作
来源：http://eaq.zycfv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yeq.yueranfly.top

[T21] Swift：遍历
来源：http://mhv.jinqigfzy.top

for x in a { print(x) }
来源：http://ahe.gotoacloud.top

[T22] Swift：字典
来源：http://nxp.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hon.ydzc1.top

[T23] Swift：函数
来源：http://cgd.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kfl.daria6918.cn

[T24] Swift：闭包
来源：http://oap.andypj.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://ufs.yuanzhike.top

[T25] Swift：结构体
来源：http://dyd.52xcode.cn

struct P { var x: Int }
来源：http://mks.smart0.xyz

[T26] Swift：类与重写
来源：http://hjl.snrcjt.cn

class A: Base { override func f() {} }
来源：http://ilq.tianlin.xyz

[T27] Swift：错误处理
来源：http://hcb.cqqwz.cn

do { try f() } catch { print(error) }
来源：http://nfi.snrcjt.cn

[T28] Swift：枚举
来源：http://uln.yanxiufei.cn

enum Color { case red, green }
来源：http://nyb.fktsv.cn

[T29] Swift：guard 提前返回
来源：http://ihv.zhongyouzk.top

guard let x = opt else { return }
来源：http://uik.chenlongwang.top

[T30] Swift：协议
来源：http://tzu.tanke756.top

protocol Shape { func area() -> Double }
来源：http://jok.hysaishi.cn

[T31] Lua：Hello World
来源：http://qvf.fehbvm.com

print("Hello")
来源：http://qgu.cqqwz.cn

[T32] Lua：局部变量
来源：http://pbc.ydzc1.top

local a = 1
来源：http://jmq.xziqi.cn

[T33] Lua：表（数组）
来源：http://eid.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nyx.ehwqpu.com

[T34] Lua：遍历表
来源：http://mrw.hcnkem.com

for i, v in ipairs(t) do print(i, v) end
来源：http://jtl.zhongyouzk.top

[T35] Lua：字典表
来源：http://btv.cheryme.top

local d = { a = 1 };  d.b = 2
来源：http://pgg.aizwys.cn

[T36] Lua：函数
来源：http://ivu.yuxming.cn

function add(a, b) return a + b end
来源：http://vdb.shuidangran.top

[T37] Lua：字符串拼接
来源：http://wzg.yvedp.cn

"a" .. "b"
来源：http://jdw.sweek.top

[T38] Lua：条件
来源：http://tmb.meibo888.top

if x > 0 then print("正") end
来源：http://vcp.ppjwa.cn

[T39] Lua：模式匹配
来源：http://tmp.birdmap.top

string.find(s, "%d+")
来源：http://fan.sjlbkw.cn

[T40] Lua：元表
来源：http://zds.snrcjt.cn

setmetatable({}, { __index = base })
来源：http://cig.zhiwuduotai.top

[T41] Perl：Hello World
来源：http://zdm.sjlbkw.cn

print "Hello\n";
来源：http://qij.svipenyu.cn

[T42] Perl：变量类型
来源：http://cti.andypj.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pcp.0kj1m.cn

[T43] Perl：字符串插值
来源：http://kov.xinyue.icu

"值: $a"
来源：http://pqj.gogol.net.cn

[T44] Perl：条件
来源：http://oto.hammf.cn

if ($a > 0) { print "正"; }
来源：http://ikm.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://xhe.yongpay.top

for my $x (@arr) { print $x; }
来源：http://evp.quarkkingdee.top

[T46] Perl：哈希操作
来源：http://ovj.uphjek.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vap.shanyushiyangtech.top

[T47] Perl：正则捕获
来源：http://xdq.xziqi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://iju.bbcook.cn

[T48] Perl：正则替换
来源：http://dyt.hfpthk.cn

$s =~ s/old/new/g;
来源：http://cpt.yanxiufei.cn

[T49] Perl：函数
来源：http://pdl.shanyushiyangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://emy.jianghu66.top

[T50] Perl：逐行读文件
来源：http://pdo.zdqjudy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nwm.zhixingplan.top

while (my $line = <$fh>) { print $line; }
来源：http://vvc.yvedp.cn

[T51] Scala：Hello World
来源：http://rzd.gogol.net.cn

println("Hello")
来源：http://zuj.pengpengdd.cyou

[T52] Scala：变量
来源：http://noi.vqdsnc.cn

val a = 1;  var b = 2
来源：http://cwu.yuxming.cn

[T53] Scala：字符串插值
来源：http://oal.jinqigufen.top

s"值: $b"
来源：http://svb.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://xqu.iojbl.cn

List(1, 2, 3).map(_ * 2)
来源：http://vrd.snrcjt.cn

[T55] Scala：集合过滤
来源：http://pyg.jqgufenzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://vms.pengpengdd.cyou

[T56] Scala：样例类
来源：http://lty.zhiwuduotai.top

case class User(name: String, age: Int)
来源：http://frn.ywan-chungtsiang.top

[T57] Scala：模式匹配
来源：http://eif.birdmap.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://eoy.shzxlz.cn

[T58] Scala：函数定义
来源：http://dhr.gogol.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pye.cqqwz.cn

[T59] Scala：循环
来源：http://cab.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://pbv.quarkkingdee.top

[T60] Scala：折叠
来源：http://twg.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oal.yvedp.cn

================================================================================
来源：http://zlv.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tuv.uphjek.com

================================================================================
来源：http://jat.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://ixq.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lkz.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://thf.yuxming.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mfi.zhaomingkeji.xyz

[U03] Py：加载 .env 配置
来源：http://tux.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://nqf.chenzaomai.com

[U04] Py：变量调试打印
来源：http://xch.quarkkingdee.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rbp.yj20258888.top

[U05] Py：列表去重且保序
来源：http://kij.fehbvm.com

list(dict.fromkeys(arr))
来源：http://fud.smart0.xyz

[U06] Py：合并两个字典
来源：http://fyi.dianchejie.cn

{**a, **b}
来源：http://qfc.epnwcf.com

[U07] Py：反转字典键值
来源：http://wte.sysykeji.top

{v: k for k, v in d.items()}
来源：http://rci.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://jpg.nanxinkj.top

[y for x in nested for y in x]
来源：http://xjh.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://ucy.hfpthk.cn

max(d, key=d.get)
来源：http://wgr.c1oappe.top

[U10] Py：按值排序字典
来源：http://hth.316326.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://azy.smart0.xyz

[U11] Py：生成器表达式
来源：http://gkj.tianlin.xyz

(x * 2 for x in arr)
来源：http://gbc.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xkm.daria6918.cn

Counter(arr).most_common(3)
来源：http://ajq.sysykeji.top

[U13] Py：固定长度队列
来源：http://sxp.xuanzx.com

deque(maxlen=10)
来源：http://kdn.pycfn.com

[U14] Py：分组收集到列表
来源：http://fhw.zhaomingkeji.xyz

defaultdict(list)
来源：http://iwz.sjlbkw.cn

[U15] Py：高精度计时
来源：http://ouj.aizwys.cn

t = time.perf_counter()
来源：http://mqf.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://evf.snrcjt.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xaq.yanxiufei.cn

[U17] Py：初始化日志
来源：http://wov.jinqigufen.top

logging.basicConfig(level=logging.INFO)
来源：http://uaa.kuanghao11.cn

[U18] Py：预编译正则
来源：http://pxa.pycfn.com

pat = re.compile(r"\d+")
来源：http://nkp.jiagoushi.top

[U19] Py：正则替换带回调
来源：http://mvr.sysykeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qwb.wangdashe.top

[U20] Py：缓存函数结果
来源：http://rgr.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://spz.zhaomingkeji.xyz

[U21] Py：自定义上下文管理器
来源：http://gkr.chenlongwang.top

@contextlib.contextmanager
来源：http://jcb.shanyushiyangtech.top

[U22] Py：矩阵转置
来源：http://nfv.yj202588.top

list(zip(*m))
来源：http://wgm.xinyue.icu

[U23] Py：分块读取大文件
来源：http://rwd.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iuk.smart0.xyz

[U24] Py：路径操作
来源：http://xva.uphjek.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jdk.feifeiyinyue.top

[U25] Py：CSV 按字典读
来源：http://yit.xingfuxueyuan.xyz

csv.DictReader(f)
来源：http://fkm.sysykeji.top

[U26] Py：并发下载
来源：http://euz.guowangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://egv.xziqi.cn

[U27] Py：异步 HTTP
来源：http://bow.yuanzhike.top

aiohttp.ClientSession() 配合 async with
来源：http://idn.ydjk.org.cn

[U28] Py：类型别名
来源：http://qxi.gotoacloud.top

UserId = int
来源：http://uwt.jianghu66.top

[U29] Py：属性校验
来源：http://vzw.sufxvd.cn

@property 与 @x.setter 配合
来源：http://yyw.pengpengdd.cyou

[U30] Py：数据类
来源：http://rle.cqqwz.cn

@dataclass(slots=True)
来源：http://lmy.ywan-chungtsiang.top

[U31] Py：单测
来源：http://azd.redwolf501.top

python -m pytest -q
来源：http://ibb.xziqi.cn

[U32] Py：代码格式化
来源：http://sta.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://apl.yonumen.top

[U33] Py：打包发布
来源：http://tku.jyoumei.cn

python -m build  （依赖 pyproject.toml）
来源：http://hkr.cqqwz.cn

[U34] Py：判断编码
来源：http://mjy.tianlin.xyz

chardet.detect(raw)
来源：http://wnm.jlsjyb.cn

[U35] Py：发送邮件
来源：http://qhf.xuanzx.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wul.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://kqn.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://pqh.jqgfzy.top

[U37] Py：读写 Excel
来源：http://loh.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://sta.316326.xyz

[U38] Py：获取脚本所在目录
来源：http://khl.yvedp.cn

Path(__file__).resolve().parent
来源：http://kcm.jinqigfzy.top

[U39] Py：判断是否在交互环境
来源：http://trz.jlsjyb.cn

sys.stdout.isatty()
来源：http://rdz.hcnkem.com

[U40] Py：打印到标准错误
来源：http://qgx.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://wrg.yj20258888.top

[U41] PHP：初始化 Composer 项目
来源：http://ljk.fzhhl.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rgg.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://ypm.zdbjq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rpq.tarul.cn

[U43] PHP：声明命名空间
来源：http://dul.uphjek.com

namespace App\Http;
来源：http://ufl.andypj.xyz

[U44] PHP：开启严格类型
来源：http://rfb.yanxiufei.cn

declare(strict_types=1);
来源：http://ify.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://eqj.zhengqikj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lzs.pycfn.com

[U46] PHP：可空类型
来源：http://qsb.cashguo.top

?string $name = null
来源：http://zfu.fengsongda.top

[U47] PHP：联合类型
来源：http://yil.yongpay.top

int|string $id
来源：http://fih.jinyuanbaomall.cn

[U48] PHP：纯枚举
来源：http://vga.chenlongwang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vut.jinghuilouyu.cn

[U49] PHP：只读属性
来源：http://qei.aibaodan.cn

public readonly string $name
来源：http://gpw.ivvv.top

[U50] PHP：构造器属性提升
来源：http://ptm.jiagoushi.top

public function __construct(private int $id) {}
来源：http://pft.zhengqikj.top

[U51] PHP：数组解构
来源：http://bie.hcnkem.com

[$a, $b] = $arr;
来源：http://pgk.sxryk.cn

[U52] PHP：箭头函数
来源：http://grr.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://rjy.shangyingyoupin.top

[U53] PHP：空合并运算符
来源：http://loj.wangdashe.top

$v = $a ?? $b ?? "default";
来源：http://acq.hnqzz.top

[U54] PHP：空安全调用
来源：http://rbe.zhijiandao.cn

$obj?->method()
来源：http://tsm.jyoumei.cn

[U55] PHP：match 表达式
来源：http://xtc.nanxuanxn.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mym.daria6918.cn

[U56] PHP：命名参数
来源：http://yfp.svipenyu.cn

f(a: 1, b: 2)
来源：http://rkc.cdnleiting.top

[U57] PHP：字符串插值
来源：http://lth.ivvv.top

"值: {$a}"
来源：http://bvb.sufxvd.cn

[U58] PHP：数组三件套
来源：http://tnn.havefunace.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qpr.nwbrower.top

[U59] PHP：自定义排序
来源：http://fnf.guowangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gxg.jinqigfzy.top

[U60] PHP：JSON 编解码
来源：http://gtx.snrcjt.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ihf.dianchejie.cn

[U61] PHP：正则
来源：http://haw.gogol.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oct.sjlbkw.cn

[U62] PHP：日期对象
来源：http://ofm.jqgfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://icc.haohaochexian.top

[U63] PHP：文件读写
来源：http://adh.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ydz.redwolf501.top

[U64] PHP：目录遍历
来源：http://tmt.aibaodan.cn

glob("dir/*.php");  scandir("dir");
来源：http://ldx.yuanzhike.top

[U65] PHP：会话
来源：http://cku.yvedp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tsx.zhiwuduotai.top

[U66] PHP：设置 Cookie
来源：http://ytc.gogol.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mph.tian-w.cn

[U67] PHP：处理文件上传
来源：http://mem.gogol.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mbr.vqdsnc.cn

[U68] PHP：PDO 连接
来源：http://aio.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ijm.zhiwuduotai.top

[U69] PHP：PDO 预处理
来源：http://vky.sufxvd.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pum.shzxlz.cn

[U70] PHP：PDO 事务
来源：http://zew.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cfj.quarkkingdee.top

[U71] PHP：抛出异常
来源：http://enm.zhixingplan.top

throw new RuntimeException("失败", 500);
来源：http://nua.gotoacloud.top

[U72] PHP：写错误日志
来源：http://jzq.daxiang520.top

error_log("失败: " . $e->getMessage());
来源：http://xhl.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://dsa.kuanghao11.cn

parse_ini_file("config.ini", true)
来源：http://lyc.cheryme.top

[U74] PHP：读取环境变量
来源：http://uyv.zdbjq.cn

getenv("APP_ENV") ?: "production"
来源：http://fak.sysykeji.top

[U75] PHP：依赖注入
来源：http://jig.jinyuanbaomall.cn

composer require psr/container
来源：http://slm.xinyue.icu

[U76] PHP：简单路由
来源：http://dmw.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zsr.redwolf501.top

[U77] PHP：模板渲染
来源：http://vwj.kuanghao11.cn

composer require twig/twig
来源：http://nnd.uphjek.com

[U78] PHP：单元测试
来源：http://xfd.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://bcq.snrcjt.cn

[U79] PHP：静态分析
来源：http://kvw.hnqzz.top

composer require --dev phpstan/phpstan
来源：http://qqt.jinqigfzy.top

[U80] PHP：代码规范修复
来源：http://haf.zhongyouzk.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jwi.hcnkem.com


<!-- 参考信息 -->