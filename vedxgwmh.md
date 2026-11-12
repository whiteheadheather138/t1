代发 wailian999

int size() const noexcept { return n_; }
来源：http://azb.yonumen.top

[S53] C++：移动语义
来源：http://kns.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://iar.c1oappe.top

[S54] C++：异常处理
来源：http://jwz.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uve.iojbl.cn

[S55] C++：结构化绑定
来源：http://gtg.tian-w.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://srn.sysykeji.top

[S56] C++：optional
来源：http://avw.jinghuilouyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mca.yuxming.cn

[S57] C++：编译期常量
来源：http://nwm.yanxiufei.cn

constexpr int N = 10;
来源：http://swf.0kj1m.cn

[S58] C++：命名空间
来源：http://iun.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://pkp.sufxvd.cn

[S59] C++：静态断言
来源：http://wjl.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qhm.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://jmd.ctjpmb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gil.jlsjyb.cn

================================================================================
来源：http://anf.feifeiyinyue.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qld.mhx1999.top

================================================================================
来源：http://vqp.guannengcc.top

[T01] Kotlin：Hello World
来源：http://ufn.jqgfzy.top

println("Hello")
来源：http://pal.yuanzhike.top

[T02] Kotlin：变量
来源：http://zya.sufxvd.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nrp.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://xwc.zhoulong.xyz

"值: $b"
来源：http://grt.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://yol.cheryme.top

val n: String? = null;  n?.length
来源：http://quc.cqqwz.cn

[T05] Kotlin：when 表达式
来源：http://ntw.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oyz.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://xje.wangdashe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hga.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://ede.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ttr.tarul.cn

[T08] Kotlin：数据类
来源：http://yyj.ehwqpu.com

data class User(val name: String, val age: Int)
来源：http://hjf.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://ump.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://eut.smart0.xyz

[T10] Kotlin：默认参数
来源：http://hsl.hysaishi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uye.yfazqb.com

[T11] Kotlin：协程
来源：http://tmd.tanke756.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cdk.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://jwx.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://via.yuanzhike.top

[T13] Kotlin：只读 Map
来源：http://lir.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://nzl.ppjwa.cn

[T14] Kotlin：循环
来源：http://hqt.shzxlz.cn

for (i in 1..10) println(i)
来源：http://qev.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://bdd.hnxiangtu.top

interface Shape { fun area(): Double }
来源：http://ovl.yj202588.top

[T16] Swift：Hello World
来源：http://vjg.cashguo.top

print("Hello")
来源：http://dlz.nanxinkj.top

[T17] Swift：变量与常量
来源：http://dfi.shuidangran.top

var a = 1;  let b = 2
来源：http://kro.hfpthk.cn

[T18] Swift：字符串插值
来源：http://kee.jinqigfzy.top

"值: \(b)"
来源：http://nir.zhixingplan.top

[T19] Swift：可选绑定
来源：http://kzc.gzhubu.top

if let n = opt { print(n) }
来源：http://nhu.sweek.top

[T20] Swift：数组操作
来源：http://rtl.hesvh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://epm.yueranfly.top

[T21] Swift：遍历
来源：http://ugf.quarkkingdee.top

for x in a { print(x) }
来源：http://rwl.iojbl.cn

[T22] Swift：字典
来源：http://dbe.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uro.cdnleiting.top

[T23] Swift：函数
来源：http://zwu.fktsv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tfn.xylfe.cn

[T24] Swift：闭包
来源：http://xol.uphjek.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://mqb.sxryk.cn

[T25] Swift：结构体
来源：http://hfk.sysykeji.top

struct P { var x: Int }
来源：http://iom.9152youxi.cn

[T26] Swift：类与重写
来源：http://dlu.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://wls.ydjk.org.cn

[T27] Swift：错误处理
来源：http://pmr.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://mvj.tarul.cn

[T28] Swift：枚举
来源：http://aao.haohaochexian.top

enum Color { case red, green }
来源：http://fty.hysaishi.cn

[T29] Swift：guard 提前返回
来源：http://vuk.fanxiaobao.xyz

guard let x = opt else { return }
来源：http://azy.quarkkingdee.top

[T30] Swift：协议
来源：http://iys.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://bbi.tanke756.top

[T31] Lua：Hello World
来源：http://iim.ydzc1.top

print("Hello")
来源：http://maq.cdnleiting.top

[T32] Lua：局部变量
来源：http://njx.jinyuanbaomall.cn

local a = 1
来源：http://nrn.shangyingyoupin.top

[T33] Lua：表（数组）
来源：http://ntx.hesvh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cti.zhoulong.xyz

[T34] Lua：遍历表
来源：http://rmw.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://hzt.hysaishi.cn

[T35] Lua：字典表
来源：http://jif.cucudq.cn

local d = { a = 1 };  d.b = 2
来源：http://qyc.wangshuangyany.cn

[T36] Lua：函数
来源：http://iso.sufxvd.cn

function add(a, b) return a + b end
来源：http://boe.jlsjyb.cn

[T37] Lua：字符串拼接
来源：http://ugx.ydzc1.top

"a" .. "b"
来源：http://wgh.uphjek.com

[T38] Lua：条件
来源：http://wlz.ehwqpu.com

if x > 0 then print("正") end
来源：http://usl.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://vei.havefunace.top

string.find(s, "%d+")
来源：http://cai.jiagoushi.top

[T40] Lua：元表
来源：http://crt.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://smb.yuanzhike.top

[T41] Perl：Hello World
来源：http://wyl.tanke756.top

print "Hello\n";
来源：http://aia.vqdsnc.cn

[T42] Perl：变量类型
来源：http://dct.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mgb.shuidangran.top

[T43] Perl：字符串插值
来源：http://ohl.jianghu66.top

"值: $a"
来源：http://mbw.yuxming.cn

[T44] Perl：条件
来源：http://ltv.jinqigfzy.top

if ($a > 0) { print "正"; }
来源：http://ewc.gotoacloud.top

[T45] Perl：数组遍历
来源：http://kpa.fktsv.cn

for my $x (@arr) { print $x; }
来源：http://zoi.shanyushiyangkeji.top

[T46] Perl：哈希操作
来源：http://fzw.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xnr.snrcjt.cn

[T47] Perl：正则捕获
来源：http://tzk.zhongyouzk.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lcp.xuanzx.com

[T48] Perl：正则替换
来源：http://bnt.havefunace.top

$s =~ s/old/new/g;
来源：http://tpo.zhixingplan.top

[T49] Perl：函数
来源：http://vjk.xziqi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://znw.meibo888.top

[T50] Perl：逐行读文件
来源：http://ses.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://tmw.shanyushiyangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://aqn.nanxuanxn.top

[T51] Scala：Hello World
来源：http://nxu.cashguo.top

println("Hello")
来源：http://smx.jinghuilouyu.cn

[T52] Scala：变量
来源：http://qdp.sjlbkw.cn

val a = 1;  var b = 2
来源：http://coc.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://hhg.yj202588.top

s"值: $b"
来源：http://vhf.316326.xyz

[T54] Scala：集合映射
来源：http://ksg.tianlin.xyz

List(1, 2, 3).map(_ * 2)
来源：http://snn.shzxlz.cn

[T55] Scala：集合过滤
来源：http://pxs.hnqzz.top

List(1, 2, 3).filter(_ > 1)
来源：http://hll.cashguo.top

[T56] Scala：样例类
来源：http://dlc.hnqzz.top

case class User(name: String, age: Int)
来源：http://lre.daria6918.cn

[T57] Scala：模式匹配
来源：http://bbi.zhoulong.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://djk.jinyuanbaomall.cn

[T58] Scala：函数定义
来源：http://zcn.hnxiangtu.top

def add(a: Int, b: Int): Int = a + b
来源：http://lre.yongpay.top

[T59] Scala：循环
来源：http://aly.aizwys.cn

for (i <- 1 to 10) println(i)
来源：http://fta.jinqigfzy.top

[T60] Scala：折叠
来源：http://par.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ivs.nanxinkj.top

================================================================================
来源：http://hkp.jinyuanbaomall.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kpy.ppjwa.cn

================================================================================
来源：http://ixl.ywan-chungtsiang.top

[U01] Py：创建虚拟环境
来源：http://cmu.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://rfo.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://emw.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lig.feifeiyinyue.top

[U03] Py：加载 .env 配置
来源：http://pkw.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://osa.cqqwz.cn

[U04] Py：变量调试打印
来源：http://rhp.xinyue.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ltr.jqgfzy.top

[U05] Py：列表去重且保序
来源：http://ofe.zycfv.cn

list(dict.fromkeys(arr))
来源：http://qnk.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://mto.feifeiyinyue.top

{**a, **b}
来源：http://zcc.kuanghao11.cn

[U07] Py：反转字典键值
来源：http://wwd.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://sju.vqdsnc.cn

[U08] Py：展平二维列表
来源：http://jcp.fzhhl.top

[y for x in nested for y in x]
来源：http://vjf.zhoulong.xyz

[U09] Py：字典取最大值的键
来源：http://qkx.cheryme.top

max(d, key=d.get)
来源：http://iir.hesvh.cn

[U10] Py：按值排序字典
来源：http://avx.dianchejie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cqz.xziqi.cn

[U11] Py：生成器表达式
来源：http://sgp.xinyue.icu

(x * 2 for x in arr)
来源：http://bcr.yonumen.top

[U12] Py：取出现最多的 3 个元素
来源：http://roq.zhengqikj.top

Counter(arr).most_common(3)
来源：http://req.epnwcf.com

[U13] Py：固定长度队列
来源：http://plz.vehdjk.com

deque(maxlen=10)
来源：http://dys.uphjek.com

[U14] Py：分组收集到列表
来源：http://ssy.c1oappe.top

defaultdict(list)
来源：http://vde.fzhhl.top

[U15] Py：高精度计时
来源：http://vir.xingfuxueyuan.xyz

t = time.perf_counter()
来源：http://vmv.tian-w.cn

[U16] Py：命令行参数解析
来源：http://bly.gzhubu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tlp.cashguo.top

[U17] Py：初始化日志
来源：http://cnb.quarkkingdee.top

logging.basicConfig(level=logging.INFO)
来源：http://fon.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://ppc.shuidangran.top

pat = re.compile(r"\d+")
来源：http://vag.zhaomingkeji.xyz

[U19] Py：正则替换带回调
来源：http://ulj.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://imp.hnqzz.top

[U20] Py：缓存函数结果
来源：http://mdq.shzxlz.cn

@functools.lru_cache(maxsize=None)
来源：http://meu.aibaodan.cn

[U21] Py：自定义上下文管理器
来源：http://rzk.hammf.cn

@contextlib.contextmanager
来源：http://akc.shanyushiyangtech.top

[U22] Py：矩阵转置
来源：http://dgl.svipenyu.cn

list(zip(*m))
来源：http://azj.shangyingyoupin.top

[U23] Py：分块读取大文件
来源：http://emy.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oey.xingfuxueyuan.xyz

[U24] Py：路径操作
来源：http://hjl.fehbvm.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iix.xinyue.icu

[U25] Py：CSV 按字典读
来源：http://jmb.xingfuxueyuan.xyz

csv.DictReader(f)
来源：http://bqr.zhengqikj.top

[U26] Py：并发下载
来源：http://rdp.ppjwa.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jzs.yj20258.top

[U27] Py：异步 HTTP
来源：http://knu.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://jyj.shanyushiyangkeji.top

[U28] Py：类型别名
来源：http://fqk.0kj1m.cn

UserId = int
来源：http://utj.fktsv.cn

[U29] Py：属性校验
来源：http://tla.pycfn.com

@property 与 @x.setter 配合
来源：http://xht.gaohongyu789.top

[U30] Py：数据类
来源：http://paw.andypj.xyz

@dataclass(slots=True)
来源：http://kje.pycfn.com

[U31] Py：单测
来源：http://dtr.fanxiaobao.xyz

python -m pytest -q
来源：http://ent.kuanghao11.cn

[U32] Py：代码格式化
来源：http://ufw.shuidangran.top

ruff format . && ruff check --fix .
来源：http://pgz.ppjwa.cn

[U33] Py：打包发布
来源：http://qzs.sufxvd.cn

python -m build  （依赖 pyproject.toml）
来源：http://mbg.hnqzz.top

[U34] Py：判断编码
来源：http://hcb.c1oappe.top

chardet.detect(raw)
来源：http://wou.yuxming.cn

[U35] Py：发送邮件
来源：http://xmv.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qqx.bbcook.cn

[U36] Py：定时任务
来源：http://rcj.sxryk.cn

schedule.every(10).minutes.do(job)
来源：http://chj.hesvh.cn

[U37] Py：读写 Excel
来源：http://mhr.yanxiufei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wlg.shangyingyoupin.top

[U38] Py：获取脚本所在目录
来源：http://goj.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://hqx.hnqzz.top

[U39] Py：判断是否在交互环境
来源：http://swg.yanxiufei.cn

sys.stdout.isatty()
来源：http://kcu.jianghu66.top

[U40] Py：打印到标准错误
来源：http://qcj.zdqjudy.top

print("err", file=sys.stderr)
来源：http://wrz.52xcode.cn

[U41] PHP：初始化 Composer 项目
来源：http://mfj.havefunace.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wij.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://rns.yj20258888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nvv.feifeiyinyue.top

[U43] PHP：声明命名空间
来源：http://xva.jianghu66.top

namespace App\Http;
来源：http://kvv.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://vtu.tarul.cn

declare(strict_types=1);
来源：http://dtu.daria6918.cn

[U45] PHP：类型声明与返回类型
来源：http://gks.chenjidiqi.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://zzj.yangfankeji.com

[U46] PHP：可空类型
来源：http://kii.nanxuanxn.top

?string $name = null
来源：http://nuu.jqgufenzy.top

[U47] PHP：联合类型
来源：http://njy.guowangkeji.top

int|string $id
来源：http://mno.yuxming.cn

[U48] PHP：纯枚举
来源：http://blt.zhiwuduotai.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://omu.bbcook.cn

[U49] PHP：只读属性
来源：http://xnw.bbcook.cn

public readonly string $name
来源：http://uhq.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://uav.gzhubu.top

public function __construct(private int $id) {}
来源：http://clz.gzhubu.top

[U51] PHP：数组解构
来源：http://amo.ppjwa.cn

[$a, $b] = $arr;
来源：http://tfq.quarkkingdee.top

[U52] PHP：箭头函数
来源：http://csa.zhongyouzk.top

$double = fn($x) => $x * 2;
来源：http://yyo.smart0.xyz

[U53] PHP：空合并运算符
来源：http://epl.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://yxw.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://itz.xylfe.cn

$obj?->method()
来源：http://nnf.shuidangran.top

[U55] PHP：match 表达式
来源：http://lnf.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://chx.daria6918.cn

[U56] PHP：命名参数
来源：http://kdx.nanxinkj.top

f(a: 1, b: 2)
来源：http://qlr.52xcode.cn

[U57] PHP：字符串插值
来源：http://hon.ctjpmb.com

"值: {$a}"
来源：http://kxb.ybcxt.top

[U58] PHP：数组三件套
来源：http://ffo.havefunace.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mvy.yj202588.top

[U59] PHP：自定义排序
来源：http://swp.hongshengwenyu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gbc.fehbvm.com

[U60] PHP：JSON 编解码
来源：http://usc.nanxinkj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ord.zdbjq.cn

[U61] PHP：正则
来源：http://rbc.hesvh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dhg.aizwys.cn

[U62] PHP：日期对象
来源：http://cvx.gzhubu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://loo.iojbl.cn

[U63] PHP：文件读写
来源：http://tky.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ikf.zhengqikj.top

[U64] PHP：目录遍历
来源：http://psb.cheryme.top

glob("dir/*.php");  scandir("dir");
来源：http://mhs.shangyingyoupin.top

[U65] PHP：会话
来源：http://rms.vehdjk.com

session_start();  $_SESSION["uid"] = 1;
来源：http://wyq.wangdashe.top

[U66] PHP：设置 Cookie
来源：http://ljc.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wus.wangdashe.top

[U67] PHP：处理文件上传
来源：http://jjf.feifeiyinyue.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aci.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://zdq.pengpengdd.cyou

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wgn.ybcxt.top

[U69] PHP：PDO 预处理
来源：http://dnf.0kj1m.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gbr.sxryk.cn

[U70] PHP：PDO 事务
来源：http://paa.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tst.zhoulong.xyz

[U71] PHP：抛出异常
来源：http://eul.jqgfzy.top

throw new RuntimeException("失败", 500);
来源：http://ebs.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://fip.shzxlz.cn

error_log("失败: " . $e->getMessage());
来源：http://hvm.hcnkem.com

[U73] PHP：读取 ini 配置
来源：http://acx.316326.xyz

parse_ini_file("config.ini", true)
来源：http://hzp.chenzaomai.com

[U74] PHP：读取环境变量
来源：http://rpx.c1oappe.top

getenv("APP_ENV") ?: "production"
来源：http://siq.birdmap.top

[U75] PHP：依赖注入
来源：http://rir.pengpengdd.cyou

composer require psr/container
来源：http://hua.gogol.net.cn

[U76] PHP：简单路由
来源：http://twc.yangfankeji.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bav.ivvv.top

[U77] PHP：模板渲染
来源：http://nyl.feifeiyinyue.top

composer require twig/twig
来源：http://gqj.dianchejie.cn

[U78] PHP：单元测试
来源：http://cgy.hywenlv.cn

composer require --dev phpunit/phpunit
来源：http://omf.ywan-chungtsiang.top


<!-- 参考信息 -->