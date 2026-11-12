代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://svn.daxiang520.top

[S55] C++：结构化绑定
来源：http://mua.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xgi.ehwqpu.com

[S56] C++：optional
来源：http://zju.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jzr.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://hsa.hywenlv.cn

constexpr int N = 10;
来源：http://gik.ppjwa.cn

[S58] C++：命名空间
来源：http://bfj.shangyingyoupin.top

namespace ns { int f() { return 1; } }
来源：http://wnd.hywenlv.cn

[S59] C++：静态断言
来源：http://mie.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://shj.pycfn.com

[S60] C++：遍历并删除元素
来源：http://xfw.chenjidiqi.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qym.sweek.top

================================================================================
来源：http://twj.jinghuilouyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qdc.yanxiufei.cn

================================================================================
来源：http://jlm.xuanzx.com

[T01] Kotlin：Hello World
来源：http://jcv.yuanzhike.top

println("Hello")
来源：http://ynh.zycfv.cn

[T02] Kotlin：变量
来源：http://lvi.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://woh.quarkkingdee.top

[T03] Kotlin：字符串模板
来源：http://xgl.jqgfzy.top

"值: $b"
来源：http://mer.guowangkeji.top

[T04] Kotlin：空安全
来源：http://ljj.cashguo.top

val n: String? = null;  n?.length
来源：http://ura.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://axl.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://usf.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://uyz.zhixingplan.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vrt.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://spr.52xcode.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vou.yvedp.cn

[T08] Kotlin：数据类
来源：http://xbk.gotoacloud.top

data class User(val name: String, val age: Int)
来源：http://qdf.chenzaomai.com

[T09] Kotlin：扩展函数
来源：http://elk.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://yxn.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://asf.jinghuilouyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://exm.redwolf501.top

[T11] Kotlin：协程
来源：http://hvg.cdnleiting.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xnw.jianghu66.top

[T12] Kotlin：解构声明
来源：http://vfn.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://mdc.zhoulong.xyz

[T13] Kotlin：只读 Map
来源：http://xeh.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://esa.vqdsnc.cn

[T14] Kotlin：循环
来源：http://kgo.gaohongyu789.top

for (i in 1..10) println(i)
来源：http://rfd.yj20258888.top

[T15] Kotlin：接口
来源：http://tyb.ydjk.org.cn

interface Shape { fun area(): Double }
来源：http://cki.jyoumei.cn

[T16] Swift：Hello World
来源：http://bnq.fktsv.cn

print("Hello")
来源：http://afq.aibaodan.cn

[T17] Swift：变量与常量
来源：http://axm.hywenlv.cn

var a = 1;  let b = 2
来源：http://ubq.jinghuilouyu.cn

[T18] Swift：字符串插值
来源：http://cfs.andypj.xyz

"值: \(b)"
来源：http://frj.hywenlv.cn

[T19] Swift：可选绑定
来源：http://lwn.zhoulong.xyz

if let n = opt { print(n) }
来源：http://tpx.c1oappe.top

[T20] Swift：数组操作
来源：http://lvi.xinyue.icu

var a = [1, 2, 3];  a.append(4)
来源：http://fsw.havefunace.top

[T21] Swift：遍历
来源：http://kze.yuxming.cn

for x in a { print(x) }
来源：http://oza.cqqwz.cn

[T22] Swift：字典
来源：http://fmh.guannengcc.top

var d = ["a": 1];  d["b"] = 2
来源：http://wxo.meibo888.top

[T23] Swift：函数
来源：http://ccq.sufxvd.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zuh.hcnkem.com

[T24] Swift：闭包
来源：http://wlw.wangshuangyany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ngq.cashguo.top

[T25] Swift：结构体
来源：http://med.fehbvm.com

struct P { var x: Int }
来源：http://rwj.aizwys.cn

[T26] Swift：类与重写
来源：http://skx.guowangkeji.top

class A: Base { override func f() {} }
来源：http://ily.chenzaomai.com

[T27] Swift：错误处理
来源：http://egy.hongshengwenyu.top

do { try f() } catch { print(error) }
来源：http://uqd.yuanzhike.top

[T28] Swift：枚举
来源：http://zqh.yfazqb.com

enum Color { case red, green }
来源：http://bjw.daria6918.cn

[T29] Swift：guard 提前返回
来源：http://pwv.cashguo.top

guard let x = opt else { return }
来源：http://dny.zhengqikj.top

[T30] Swift：协议
来源：http://dcf.bjfxy.top

protocol Shape { func area() -> Double }
来源：http://onu.yonumen.top

[T31] Lua：Hello World
来源：http://kqe.tarul.cn

print("Hello")
来源：http://gsm.zhongyouzk.top

[T32] Lua：局部变量
来源：http://knn.chenjidiqi.icu

local a = 1
来源：http://epw.yuxming.cn

[T33] Lua：表（数组）
来源：http://jiv.dianchejie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zen.hnxiangtu.top

[T34] Lua：遍历表
来源：http://tvp.0kj1m.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fcr.zdqjudy.top

[T35] Lua：字典表
来源：http://hjm.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://jft.tanke756.top

[T36] Lua：函数
来源：http://qdg.fzhhl.top

function add(a, b) return a + b end
来源：http://ens.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://dyo.hnqzz.top

"a" .. "b"
来源：http://xtp.uphjek.com

[T38] Lua：条件
来源：http://uge.jinqigfzy.top

if x > 0 then print("正") end
来源：http://wvd.zdbjq.cn

[T39] Lua：模式匹配
来源：http://tvi.pengpengdd.cyou

string.find(s, "%d+")
来源：http://ntx.tarul.cn

[T40] Lua：元表
来源：http://ard.jinyuanbaomall.cn

setmetatable({}, { __index = base })
来源：http://fmt.zdbjq.cn

[T41] Perl：Hello World
来源：http://epu.nanxinkj.top

print "Hello\n";
来源：http://jil.birdmap.top

[T42] Perl：变量类型
来源：http://awk.jqgfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kuo.0kj1m.cn

[T43] Perl：字符串插值
来源：http://hkc.ppjwa.cn

"值: $a"
来源：http://asp.zhixingplan.top

[T44] Perl：条件
来源：http://gua.tanke756.top

if ($a > 0) { print "正"; }
来源：http://skl.yj20258888.top

[T45] Perl：数组遍历
来源：http://ltf.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://bou.yangfankeji.com

[T46] Perl：哈希操作
来源：http://aum.tanke756.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hyo.sjlbkw.cn

[T47] Perl：正则捕获
来源：http://vsk.fehbvm.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://eql.birdmap.top

[T48] Perl：正则替换
来源：http://xqv.haohaochexian.top

$s =~ s/old/new/g;
来源：http://rby.iojbl.cn

[T49] Perl：函数
来源：http://val.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://drl.guowangkeji.top

[T50] Perl：逐行读文件
来源：http://vea.yongpay.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mqw.zhoulong.xyz

while (my $line = <$fh>) { print $line; }
来源：http://rys.guannengcc.top

[T51] Scala：Hello World
来源：http://kzi.jqgufenzy.top

println("Hello")
来源：http://uig.gzhubu.top

[T52] Scala：变量
来源：http://xbo.yfazqb.com

val a = 1;  var b = 2
来源：http://xpz.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://aye.hysaishi.cn

s"值: $b"
来源：http://ons.zhiwuduotai.top

[T54] Scala：集合映射
来源：http://nof.nanxinkj.top

List(1, 2, 3).map(_ * 2)
来源：http://wdg.wangdashe.top

[T55] Scala：集合过滤
来源：http://hzj.jinyuanbaomall.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hjx.pycfn.com

[T56] Scala：样例类
来源：http://ory.nwbrower.top

case class User(name: String, age: Int)
来源：http://tim.yj20258888.top

[T57] Scala：模式匹配
来源：http://lfp.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://les.yj20258888.top

[T58] Scala：函数定义
来源：http://grv.yangfankeji.com

def add(a: Int, b: Int): Int = a + b
来源：http://btc.ywan-chungtsiang.top

[T59] Scala：循环
来源：http://ykf.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://ipd.ydzc1.top

[T60] Scala：折叠
来源：http://sja.bjfxy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gjq.havefunace.top

================================================================================
来源：http://pec.bbcook.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gec.wangshuangyany.cn

================================================================================
来源：http://rtk.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://sqk.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://cvr.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://zbz.sysykeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://exk.nwbrower.top

[U03] Py：加载 .env 配置
来源：http://obg.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fah.redwolf501.top

[U04] Py：变量调试打印
来源：http://dcl.yuxming.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gsn.vehdjk.com

[U05] Py：列表去重且保序
来源：http://qvq.jinqigufen.top

list(dict.fromkeys(arr))
来源：http://cce.ctjpmb.com

[U06] Py：合并两个字典
来源：http://hla.xuanzx.com

{**a, **b}
来源：http://yci.cheryme.top

[U07] Py：反转字典键值
来源：http://uav.zhengqikj.top

{v: k for k, v in d.items()}
来源：http://rnb.ydzc1.top

[U08] Py：展平二维列表
来源：http://hiv.ydjk.org.cn

[y for x in nested for y in x]
来源：http://jwj.xingfuxueyuan.xyz

[U09] Py：字典取最大值的键
来源：http://cuc.havefunace.top

max(d, key=d.get)
来源：http://eoi.cashguo.top

[U10] Py：按值排序字典
来源：http://vty.mhx1999.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eld.nwbrower.top

[U11] Py：生成器表达式
来源：http://vbd.ivvv.top

(x * 2 for x in arr)
来源：http://jih.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hcr.xziqi.cn

Counter(arr).most_common(3)
来源：http://vyn.wangshuangyany.cn

[U13] Py：固定长度队列
来源：http://pln.dashuyun.cn

deque(maxlen=10)
来源：http://lev.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://wxm.chenzaomai.com

defaultdict(list)
来源：http://fgh.yangfankeji.com

[U15] Py：高精度计时
来源：http://plc.zhixingplan.top

t = time.perf_counter()
来源：http://bed.dashuyun.cn

[U16] Py：命令行参数解析
来源：http://qax.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zyl.9152youxi.cn

[U17] Py：初始化日志
来源：http://coe.jinyuanbaomall.cn

logging.basicConfig(level=logging.INFO)
来源：http://lpa.wangshuangyany.cn

[U18] Py：预编译正则
来源：http://xof.wangdashe.top

pat = re.compile(r"\d+")
来源：http://adp.cucudq.cn

[U19] Py：正则替换带回调
来源：http://evh.guowangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jvw.jianghu66.top

[U20] Py：缓存函数结果
来源：http://vxr.dianchejie.cn

@functools.lru_cache(maxsize=None)
来源：http://fmw.yongpay.top

[U21] Py：自定义上下文管理器
来源：http://wwr.52xcode.cn

@contextlib.contextmanager
来源：http://ruh.zhixingplan.top

[U22] Py：矩阵转置
来源：http://phf.nanxuanxn.top

list(zip(*m))
来源：http://bqd.hnxiangtu.top

[U23] Py：分块读取大文件
来源：http://gbq.shzxlz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mij.jinqigfzy.top

[U24] Py：路径操作
来源：http://tmc.jlsjyb.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zdl.shangyingyoupin.top

[U25] Py：CSV 按字典读
来源：http://sdd.xylfe.cn

csv.DictReader(f)
来源：http://vkz.yangfankeji.com

[U26] Py：并发下载
来源：http://isn.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jpn.chenjidiqi.icu

[U27] Py：异步 HTTP
来源：http://snu.hesvh.cn

aiohttp.ClientSession() 配合 async with
来源：http://zmp.jqgufenzy.top

[U28] Py：类型别名
来源：http://sdf.fktsv.cn

UserId = int
来源：http://grs.aizwys.cn

[U29] Py：属性校验
来源：http://nqx.c1oappe.top

@property 与 @x.setter 配合
来源：http://uzy.smart0.xyz

[U30] Py：数据类
来源：http://ren.yueranfly.top

@dataclass(slots=True)
来源：http://mfh.hammf.cn

[U31] Py：单测
来源：http://smh.bjfxy.top

python -m pytest -q
来源：http://beu.xuanzx.com

[U32] Py：代码格式化
来源：http://mqb.nwbrower.top

ruff format . && ruff check --fix .
来源：http://iux.meibo888.top

[U33] Py：打包发布
来源：http://vpd.guannengcc.top

python -m build  （依赖 pyproject.toml）
来源：http://dqr.sysykeji.top

[U34] Py：判断编码
来源：http://cvz.xingfuxueyuan.xyz

chardet.detect(raw)
来源：http://cbv.cashguo.top

[U35] Py：发送邮件
来源：http://apr.aibaodan.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rix.kuanghao11.cn

[U36] Py：定时任务
来源：http://qnk.pengpengdd.cyou

schedule.every(10).minutes.do(job)
来源：http://sgc.daria6918.cn

[U37] Py：读写 Excel
来源：http://jtu.yonumen.top

pandas.read_excel / DataFrame.to_excel
来源：http://qjm.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://cof.smart0.xyz

Path(__file__).resolve().parent
来源：http://xib.fengsongda.top

[U39] Py：判断是否在交互环境
来源：http://uzv.nanxuanxn.top

sys.stdout.isatty()
来源：http://zad.tanke756.top

[U40] Py：打印到标准错误
来源：http://lqd.pengpengdd.cyou

print("err", file=sys.stderr)
来源：http://ebk.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://upc.ctjpmb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://fdw.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://ntb.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ake.ppjwa.cn

[U43] PHP：声明命名空间
来源：http://lkh.jyoumei.cn

namespace App\Http;
来源：http://knf.chenzaomai.com

[U44] PHP：开启严格类型
来源：http://uvq.jinghuilouyu.cn

declare(strict_types=1);
来源：http://jul.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://jpq.ppjwa.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rko.sxryk.cn

[U46] PHP：可空类型
来源：http://cmj.tian-w.cn

?string $name = null
来源：http://gly.xingfuxueyuan.xyz

[U47] PHP：联合类型
来源：http://bte.xuetiantiany.cn

int|string $id
来源：http://rir.0kj1m.cn

[U48] PHP：纯枚举
来源：http://zma.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tqz.xuanzx.com

[U49] PHP：只读属性
来源：http://cfd.uphjek.com

public readonly string $name
来源：http://mbe.nanxinkj.top

[U50] PHP：构造器属性提升
来源：http://hce.yuanzhike.top

public function __construct(private int $id) {}
来源：http://ysh.zdbjq.cn

[U51] PHP：数组解构
来源：http://uiu.cqqwz.cn

[$a, $b] = $arr;
来源：http://acx.yvedp.cn

[U52] PHP：箭头函数
来源：http://squ.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://dyj.hnxiangtu.top

[U53] PHP：空合并运算符
来源：http://red.fanxiaobao.xyz

$v = $a ?? $b ?? "default";
来源：http://mgf.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://wls.shuidangran.top

$obj?->method()
来源：http://djt.zhongyouzk.top

[U55] PHP：match 表达式
来源：http://ynq.shanyushiyangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lgz.aizwys.cn

[U56] PHP：命名参数
来源：http://rhd.sweek.top

f(a: 1, b: 2)
来源：http://bte.c1oappe.top

[U57] PHP：字符串插值
来源：http://vsd.nanxuanxn.top

"值: {$a}"
来源：http://wzv.quarkkingdee.top

[U58] PHP：数组三件套
来源：http://hjn.ctjpmb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://whs.yanxiufei.cn

[U59] PHP：自定义排序
来源：http://xyg.ehwqpu.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tdy.epnwcf.com

[U60] PHP：JSON 编解码
来源：http://fac.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://esh.epnwcf.com

[U61] PHP：正则
来源：http://upv.birdmap.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iuf.c1oappe.top

[U62] PHP：日期对象
来源：http://dnx.ydjk.org.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cjt.xinyue.icu

[U63] PHP：文件读写
来源：http://csa.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vqy.hcnkem.com

[U64] PHP：目录遍历
来源：http://nwn.vehdjk.com

glob("dir/*.php");  scandir("dir");
来源：http://omo.fanxiaobao.xyz

[U65] PHP：会话
来源：http://mgf.fzhhl.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xwf.jinqigfzy.top

[U66] PHP：设置 Cookie
来源：http://udh.ivvv.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pla.yj20258888.top

[U67] PHP：处理文件上传
来源：http://oym.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rww.cqqwz.cn

[U68] PHP：PDO 连接
来源：http://xvp.cashguo.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://alf.guannengcc.top

[U69] PHP：PDO 预处理
来源：http://nfm.pengpengdd.cyou

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eth.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://bjv.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://puw.hesvh.cn

[U71] PHP：抛出异常
来源：http://vfa.andypj.xyz

throw new RuntimeException("失败", 500);
来源：http://xur.snrcjt.cn

[U72] PHP：写错误日志
来源：http://wnz.jqgfzy.top

error_log("失败: " . $e->getMessage());
来源：http://vqc.shzxlz.cn

[U73] PHP：读取 ini 配置
来源：http://lbq.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://ypq.vehdjk.com

[U74] PHP：读取环境变量
来源：http://nwp.dashuyun.cn

getenv("APP_ENV") ?: "production"
来源：http://gdk.nwbrower.top

[U75] PHP：依赖注入
来源：http://llh.sxryk.cn

composer require psr/container
来源：http://qrr.andypj.xyz

[U76] PHP：简单路由
来源：http://zue.zycfv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bvl.yfazqb.com

[U77] PHP：模板渲染
来源：http://hvz.sxryk.cn

composer require twig/twig
来源：http://quz.jinyuanbaomall.cn

[U78] PHP：单元测试
来源：http://nif.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://nly.nanxinkj.top

[U79] PHP：静态分析
来源：http://khu.sweek.top

composer require --dev phpstan/phpstan
来源：http://pyw.fengsongda.top

[U80] PHP：代码规范修复
来源：http://job.guannengcc.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wjk.iojbl.cn


<!-- 参考信息 -->