代发 wailian999

int size() const noexcept { return n_; }
来源：http://qkr.cheryme.top

[S53] C++：移动语义
来源：http://cqd.tarul.cn

std::vector<int> w = std::move(v);
来源：http://mea.fengsongda.top

[S54] C++：异常处理
来源：http://olw.shanyushiyangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jea.dashuyun.cn

[S55] C++：结构化绑定
来源：http://jks.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sau.gzhubu.top

[S56] C++：optional
来源：http://rvo.zycfv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gzf.snrcjt.cn

[S57] C++：编译期常量
来源：http://dmb.guowangkeji.top

constexpr int N = 10;
来源：http://pfx.shangyingyoupin.top

[S58] C++：命名空间
来源：http://zds.nwbrower.top

namespace ns { int f() { return 1; } }
来源：http://nys.wangdashe.top

[S59] C++：静态断言
来源：http://akp.xinyue.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zcr.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://eea.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ktq.hesvh.cn

================================================================================
来源：http://ikb.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xmf.guowangkeji.top

================================================================================
来源：http://iah.bjfxy.top

[T01] Kotlin：Hello World
来源：http://ocv.zycfv.cn

println("Hello")
来源：http://yqe.wangshuangyany.cn

[T02] Kotlin：变量
来源：http://qnr.yj20258888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jqk.fengsongda.top

[T03] Kotlin：字符串模板
来源：http://ohw.cashguo.top

"值: $b"
来源：http://ymo.guannengcc.top

[T04] Kotlin：空安全
来源：http://kjc.vqdsnc.cn

val n: String? = null;  n?.length
来源：http://hbo.bjfxy.top

[T05] Kotlin：when 表达式
来源：http://oak.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mmg.zhijiandao.cn

[T06] Kotlin：集合映射
来源：http://stf.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://exg.gaohongyu789.top

[T07] Kotlin：集合过滤
来源：http://tip.hywenlv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hky.ivvv.top

[T08] Kotlin：数据类
来源：http://qtb.sysykeji.top

data class User(val name: String, val age: Int)
来源：http://twv.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://teh.ivvv.top

fun String.exclaim() = this + "!"
来源：http://bmc.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://hdq.ywan-chungtsiang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://grj.gogol.net.cn

[T11] Kotlin：协程
来源：http://idr.xziqi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cvl.gogol.net.cn

[T12] Kotlin：解构声明
来源：http://idn.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://fwe.fanxiaobao.xyz

[T13] Kotlin：只读 Map
来源：http://mro.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://rzo.yanxiufei.cn

[T14] Kotlin：循环
来源：http://kum.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://edl.jlsjyb.cn

[T15] Kotlin：接口
来源：http://cdj.hcnkem.com

interface Shape { fun area(): Double }
来源：http://cay.zhoulong.xyz

[T16] Swift：Hello World
来源：http://rnx.jqgfzy.top

print("Hello")
来源：http://pla.meibo888.top

[T17] Swift：变量与常量
来源：http://mcf.yj20258888.top

var a = 1;  let b = 2
来源：http://qgx.yueranfly.top

[T18] Swift：字符串插值
来源：http://iep.sxryk.cn

"值: \(b)"
来源：http://tyj.jinqigufen.top

[T19] Swift：可选绑定
来源：http://ggg.yj20258.top

if let n = opt { print(n) }
来源：http://jyy.daxiang520.top

[T20] Swift：数组操作
来源：http://ete.gaohongyu789.top

var a = [1, 2, 3];  a.append(4)
来源：http://brq.0kj1m.cn

[T21] Swift：遍历
来源：http://ojl.sxryk.cn

for x in a { print(x) }
来源：http://zqe.andypj.xyz

[T22] Swift：字典
来源：http://oda.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://msf.yj20258.top

[T23] Swift：函数
来源：http://auu.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nfm.wangshuangyany.cn

[T24] Swift：闭包
来源：http://emd.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uzx.9152youxi.cn

[T25] Swift：结构体
来源：http://bqm.hesvh.cn

struct P { var x: Int }
来源：http://jje.ydjk.org.cn

[T26] Swift：类与重写
来源：http://svi.yj20258888.top

class A: Base { override func f() {} }
来源：http://cpy.gzhubu.top

[T27] Swift：错误处理
来源：http://pqa.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://klf.xylfe.cn

[T28] Swift：枚举
来源：http://qik.snrcjt.cn

enum Color { case red, green }
来源：http://wjc.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://sgn.gzhubu.top

guard let x = opt else { return }
来源：http://ghy.sjlbkw.cn

[T30] Swift：协议
来源：http://rfb.0kj1m.cn

protocol Shape { func area() -> Double }
来源：http://wez.tian-w.cn

[T31] Lua：Hello World
来源：http://ztk.aizwys.cn

print("Hello")
来源：http://lhl.zhongyouzk.top

[T32] Lua：局部变量
来源：http://rox.kuanghao11.cn

local a = 1
来源：http://nou.epnwcf.com

[T33] Lua：表（数组）
来源：http://sjy.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qnc.sjlbkw.cn

[T34] Lua：遍历表
来源：http://xwf.uphjek.com

for i, v in ipairs(t) do print(i, v) end
来源：http://slu.tianlin.xyz

[T35] Lua：字典表
来源：http://cno.dianchejie.cn

local d = { a = 1 };  d.b = 2
来源：http://pyb.cheryme.top

[T36] Lua：函数
来源：http://itz.kuanghao11.cn

function add(a, b) return a + b end
来源：http://mzc.ydzc1.top

[T37] Lua：字符串拼接
来源：http://pxo.yj20258.top

"a" .. "b"
来源：http://ndu.hywenlv.cn

[T38] Lua：条件
来源：http://ssg.ctjpmb.com

if x > 0 then print("正") end
来源：http://kkm.smart0.xyz

[T39] Lua：模式匹配
来源：http://nfx.ybcxt.top

string.find(s, "%d+")
来源：http://hfj.shzxlz.cn

[T40] Lua：元表
来源：http://wpa.yuanzhike.top

setmetatable({}, { __index = base })
来源：http://ecl.yj20258.top

[T41] Perl：Hello World
来源：http://qyz.wangdashe.top

print "Hello\n";
来源：http://pnc.bjfxy.top

[T42] Perl：变量类型
来源：http://tbe.gotoacloud.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://por.jiagoushi.top

[T43] Perl：字符串插值
来源：http://utz.yfazqb.com

"值: $a"
来源：http://fnm.svipenyu.cn

[T44] Perl：条件
来源：http://cqs.sysykeji.top

if ($a > 0) { print "正"; }
来源：http://xpr.gaohongyu789.top

[T45] Perl：数组遍历
来源：http://pkg.chenjidiqi.icu

for my $x (@arr) { print $x; }
来源：http://rwj.jinqigufen.top

[T46] Perl：哈希操作
来源：http://zii.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tyx.cheryme.top

[T47] Perl：正则捕获
来源：http://pxy.c1oappe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rob.tian-w.cn

[T48] Perl：正则替换
来源：http://qlp.xingfuxueyuan.xyz

$s =~ s/old/new/g;
来源：http://ewc.hammf.cn

[T49] Perl：函数
来源：http://ogq.ppjwa.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ckp.yuxming.cn

[T50] Perl：逐行读文件
来源：http://eyz.xziqi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qao.yongpay.top

while (my $line = <$fh>) { print $line; }
来源：http://nmf.guannengcc.top

[T51] Scala：Hello World
来源：http://xka.tian-w.cn

println("Hello")
来源：http://qdl.jyoumei.cn

[T52] Scala：变量
来源：http://umk.tanke756.top

val a = 1;  var b = 2
来源：http://scv.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://zsl.cqqwz.cn

s"值: $b"
来源：http://hqn.fehbvm.com

[T54] Scala：集合映射
来源：http://dkh.bjfxy.top

List(1, 2, 3).map(_ * 2)
来源：http://bea.yj202588.top

[T55] Scala：集合过滤
来源：http://cix.feifeiyinyue.top

List(1, 2, 3).filter(_ > 1)
来源：http://boa.9152youxi.cn

[T56] Scala：样例类
来源：http://qho.chenlongwang.top

case class User(name: String, age: Int)
来源：http://ndl.fktsv.cn

[T57] Scala：模式匹配
来源：http://fhg.zhoulong.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://tag.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://rvd.sxryk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jdi.iojbl.cn

[T59] Scala：循环
来源：http://rtr.iojbl.cn

for (i <- 1 to 10) println(i)
来源：http://zsp.yj20258.top

[T60] Scala：折叠
来源：http://ene.jinqigfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rsn.pycfn.com

================================================================================
来源：http://pzf.9152youxi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fld.sysykeji.top

================================================================================
来源：http://hss.sufxvd.cn

[U01] Py：创建虚拟环境
来源：http://jtw.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fuc.yj20258.top

[U02] Py：导出 / 安装依赖
来源：http://ibq.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zle.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://rtx.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://eyi.zhongyouzk.top

[U04] Py：变量调试打印
来源：http://srq.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xvk.xylfe.cn

[U05] Py：列表去重且保序
来源：http://pix.fehbvm.com

list(dict.fromkeys(arr))
来源：http://nio.wangdashe.top

[U06] Py：合并两个字典
来源：http://iik.meibo888.top

{**a, **b}
来源：http://foo.gaohongyu789.top

[U07] Py：反转字典键值
来源：http://yfs.fengsongda.top

{v: k for k, v in d.items()}
来源：http://ojw.yonumen.top

[U08] Py：展平二维列表
来源：http://ljt.cucudq.cn

[y for x in nested for y in x]
来源：http://tpg.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://ttj.tarul.cn

max(d, key=d.get)
来源：http://ust.jinqigufen.top

[U10] Py：按值排序字典
来源：http://hdn.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qeh.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://gsa.vqdsnc.cn

(x * 2 for x in arr)
来源：http://rzf.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://eal.yj20258888.top

Counter(arr).most_common(3)
来源：http://bnr.guowangkeji.top

[U13] Py：固定长度队列
来源：http://lna.jianghu66.top

deque(maxlen=10)
来源：http://xsw.fktsv.cn

[U14] Py：分组收集到列表
来源：http://yly.uphjek.com

defaultdict(list)
来源：http://ecu.cucudq.cn

[U15] Py：高精度计时
来源：http://cng.hysaishi.cn

t = time.perf_counter()
来源：http://ymf.xuanzx.com

[U16] Py：命令行参数解析
来源：http://cvq.pengpengdd.cyou

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xhv.nwbrower.top

[U17] Py：初始化日志
来源：http://uqm.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://bhx.ydzc1.top

[U18] Py：预编译正则
来源：http://obg.yuxming.cn

pat = re.compile(r"\d+")
来源：http://pyi.yanxiufei.cn

[U19] Py：正则替换带回调
来源：http://vcu.jqgufenzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mmt.xuanzx.com

[U20] Py：缓存函数结果
来源：http://kem.kuanghao11.cn

@functools.lru_cache(maxsize=None)
来源：http://oip.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://mlv.52xcode.cn

@contextlib.contextmanager
来源：http://mrf.0kj1m.cn

[U22] Py：矩阵转置
来源：http://iac.52xcode.cn

list(zip(*m))
来源：http://bud.zhaomingkeji.xyz

[U23] Py：分块读取大文件
来源：http://ubf.wangdashe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jlu.chenzaomai.com

[U24] Py：路径操作
来源：http://teg.quarkkingdee.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gnp.cheryme.top

[U25] Py：CSV 按字典读
来源：http://pch.aibaodan.cn

csv.DictReader(f)
来源：http://kbc.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://bqg.wangshuangyany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qnq.epnwcf.com

[U27] Py：异步 HTTP
来源：http://kxd.wangshuangyany.cn

aiohttp.ClientSession() 配合 async with
来源：http://htl.tian-w.cn

[U28] Py：类型别名
来源：http://ele.hcnkem.com

UserId = int
来源：http://wkz.cheryme.top

[U29] Py：属性校验
来源：http://eue.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://ibl.ctjpmb.com

[U30] Py：数据类
来源：http://zuj.mhx1999.top

@dataclass(slots=True)
来源：http://npf.gotoacloud.top

[U31] Py：单测
来源：http://akz.sufxvd.cn

python -m pytest -q
来源：http://sdi.jinghuilouyu.cn

[U32] Py：代码格式化
来源：http://sjj.hnxiangtu.top

ruff format . && ruff check --fix .
来源：http://fbm.shzxlz.cn

[U33] Py：打包发布
来源：http://dhs.316326.xyz

python -m build  （依赖 pyproject.toml）
来源：http://dgf.ydjk.org.cn

[U34] Py：判断编码
来源：http://ztq.yj20258888.top

chardet.detect(raw)
来源：http://xmb.birdmap.top

[U35] Py：发送邮件
来源：http://kxr.kuanghao11.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qck.aibaodan.cn

[U36] Py：定时任务
来源：http://uhs.fengsongda.top

schedule.every(10).minutes.do(job)
来源：http://kpb.hfpthk.cn

[U37] Py：读写 Excel
来源：http://buv.jlsjyb.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bru.dianchejie.cn

[U38] Py：获取脚本所在目录
来源：http://nqz.zycfv.cn

Path(__file__).resolve().parent
来源：http://kbz.pycfn.com

[U39] Py：判断是否在交互环境
来源：http://gil.zdbjq.cn

sys.stdout.isatty()
来源：http://tnn.xziqi.cn

[U40] Py：打印到标准错误
来源：http://atq.jinqigfzy.top

print("err", file=sys.stderr)
来源：http://ndj.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://bya.sxryk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://emb.fanxiaobao.xyz

[U42] PHP：PSR-4 自动加载
来源：http://tuz.zhijiandao.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ref.ybcxt.top

[U43] PHP：声明命名空间
来源：http://coo.bjfxy.top

namespace App\Http;
来源：http://vpv.cqqwz.cn

[U44] PHP：开启严格类型
来源：http://opb.52xcode.cn

declare(strict_types=1);
来源：http://evg.jinqigufen.top

[U45] PHP：类型声明与返回类型
来源：http://wrh.sweek.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://bzl.gogol.net.cn

[U46] PHP：可空类型
来源：http://qbg.zhixingplan.top

?string $name = null
来源：http://jwl.nanxuanxn.top

[U47] PHP：联合类型
来源：http://bcd.svipenyu.cn

int|string $id
来源：http://xaq.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://kcv.shangyingyoupin.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ilw.yj20258888.top

[U49] PHP：只读属性
来源：http://fgj.52xcode.cn

public readonly string $name
来源：http://blv.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://dxb.uphjek.com

public function __construct(private int $id) {}
来源：http://anj.jiagoushi.top

[U51] PHP：数组解构
来源：http://lfj.ivvv.top

[$a, $b] = $arr;
来源：http://rzd.fehbvm.com

[U52] PHP：箭头函数
来源：http://uic.havefunace.top

$double = fn($x) => $x * 2;
来源：http://oud.xuanzx.com

[U53] PHP：空合并运算符
来源：http://ekl.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://rlt.hysaishi.cn

[U54] PHP：空安全调用
来源：http://fmu.xziqi.cn

$obj?->method()
来源：http://emo.ehwqpu.com

[U55] PHP：match 表达式
来源：http://soz.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dhg.ydzc1.top

[U56] PHP：命名参数
来源：http://jiu.yfazqb.com

f(a: 1, b: 2)
来源：http://xze.tanke756.top

[U57] PHP：字符串插值
来源：http://vev.hammf.cn

"值: {$a}"
来源：http://zcz.ybcxt.top

[U58] PHP：数组三件套
来源：http://qed.shzxlz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nmj.xinyue.icu

[U59] PHP：自定义排序
来源：http://cqm.yfazqb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qag.wangdashe.top

[U60] PHP：JSON 编解码
来源：http://mup.zdqjudy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fqp.haohaochexian.top

[U61] PHP：正则
来源：http://fdb.sjlbkw.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ywc.zhoulong.xyz

[U62] PHP：日期对象
来源：http://iek.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mjk.kuanghao11.cn

[U63] PHP：文件读写
来源：http://uph.sjlbkw.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gyh.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://raw.svipenyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://mwg.hammf.cn

[U65] PHP：会话
来源：http://zlx.wangshuangyany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gly.yj202588.top

[U66] PHP：设置 Cookie
来源：http://mao.zhongyouzk.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://abq.jinghuilouyu.cn

[U67] PHP：处理文件上传
来源：http://bra.yj20258888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ykf.jianghu66.top

[U68] PHP：PDO 连接
来源：http://wwk.hywenlv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fcw.shanyushiyangtech.top

[U69] PHP：PDO 预处理
来源：http://hpy.tarul.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://owa.ydjk.org.cn

[U70] PHP：PDO 事务
来源：http://zvx.fehbvm.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jww.jinyuanbaomall.cn

[U71] PHP：抛出异常
来源：http://lvd.aizwys.cn

throw new RuntimeException("失败", 500);
来源：http://nbx.xingfuxueyuan.xyz

[U72] PHP：写错误日志
来源：http://dcg.yonumen.top

error_log("失败: " . $e->getMessage());
来源：http://rme.yuanzhike.top

[U73] PHP：读取 ini 配置
来源：http://tpg.xuetiantiany.cn

parse_ini_file("config.ini", true)
来源：http://beu.jqgfzy.top

[U74] PHP：读取环境变量
来源：http://rjh.chenjidiqi.icu

getenv("APP_ENV") ?: "production"
来源：http://tbb.yonumen.top

[U75] PHP：依赖注入
来源：http://uyq.hywenlv.cn

composer require psr/container
来源：http://ska.birdmap.top

[U76] PHP：简单路由
来源：http://cgw.redwolf501.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://enh.9152youxi.cn

[U77] PHP：模板渲染
来源：http://zcb.xingfuxueyuan.xyz

composer require twig/twig
来源：http://gja.zhixingplan.top

[U78] PHP：单元测试
来源：http://xbe.nanxuanxn.top

composer require --dev phpunit/phpunit
来源：http://wcy.aizwys.cn


<!-- 参考信息 -->