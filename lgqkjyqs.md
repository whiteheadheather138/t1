代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://prs.cashguo.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gri.jqgfzy.top

[S48] C++：逐行读文件
来源：http://dhy.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://jsp.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://uhy.yanxiufei.cn

[S49] C++：写文件
来源：http://qwn.ehwqpu.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yyd.cqqwz.cn

[S50] C++：格式化数字
来源：http://uhm.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tkr.hywenlv.cn

[S51] C++：显式类型转换
来源：http://izc.gogol.net.cn

static_cast<double>(a) / b
来源：http://ixo.yj20258.top

[S52] C++：const 与 noexcept
来源：http://wbd.hammf.cn

int size() const noexcept { return n_; }
来源：http://rrd.52xcode.cn

[S53] C++：移动语义
来源：http://qur.ywan-chungtsiang.top

std::vector<int> w = std::move(v);
来源：http://zec.chenzaomai.com

[S54] C++：异常处理
来源：http://kjd.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hks.ybcxt.top

[S55] C++：结构化绑定
来源：http://zzj.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://amf.ywan-chungtsiang.top

[S56] C++：optional
来源：http://ckh.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jcf.yongpay.top

[S57] C++：编译期常量
来源：http://wmk.c1oappe.top

constexpr int N = 10;
来源：http://zwl.kuanghao11.cn

[S58] C++：命名空间
来源：http://fop.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://mzj.daxiang520.top

[S59] C++：静态断言
来源：http://spt.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tne.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://chr.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cna.wangdashe.top

================================================================================
来源：http://ogo.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zxk.tarul.cn

================================================================================
来源：http://nyi.gzhubu.top

[T01] Kotlin：Hello World
来源：http://gzn.xziqi.cn

println("Hello")
来源：http://cab.sufxvd.cn

[T02] Kotlin：变量
来源：http://nue.yj20258888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kix.xingfuxueyuan.xyz

[T03] Kotlin：字符串模板
来源：http://iqi.daria6918.cn

"值: $b"
来源：http://qxq.c1oappe.top

[T04] Kotlin：空安全
来源：http://tmu.jyoumei.cn

val n: String? = null;  n?.length
来源：http://ktm.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://lmu.yongpay.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lqm.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://zjn.xziqi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://djz.ydzc1.top

[T07] Kotlin：集合过滤
来源：http://tmx.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rgw.fanxiaobao.xyz

[T08] Kotlin：数据类
来源：http://wcc.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://bbp.sweek.top

[T09] Kotlin：扩展函数
来源：http://exh.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://iid.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://apo.andypj.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://eyk.feifeiyinyue.top

[T11] Kotlin：协程
来源：http://sfk.hammf.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xzl.shzxlz.cn

[T12] Kotlin：解构声明
来源：http://oxw.aibaodan.cn

val (a, b) = Pair(1, 2)
来源：http://nsb.hnxiangtu.top

[T13] Kotlin：只读 Map
来源：http://ohj.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://kwy.ywan-chungtsiang.top

[T14] Kotlin：循环
来源：http://nqe.nwbrower.top

for (i in 1..10) println(i)
来源：http://tvy.pycfn.com

[T15] Kotlin：接口
来源：http://hky.wangdashe.top

interface Shape { fun area(): Double }
来源：http://dme.ivvv.top

[T16] Swift：Hello World
来源：http://ody.yvedp.cn

print("Hello")
来源：http://wrp.jlsjyb.cn

[T17] Swift：变量与常量
来源：http://ieh.gzhubu.top

var a = 1;  let b = 2
来源：http://rhy.redwolf501.top

[T18] Swift：字符串插值
来源：http://ilm.xingfuxueyuan.xyz

"值: \(b)"
来源：http://ahr.9152youxi.cn

[T19] Swift：可选绑定
来源：http://wcq.hnxiangtu.top

if let n = opt { print(n) }
来源：http://rgt.52xcode.cn

[T20] Swift：数组操作
来源：http://vxo.redwolf501.top

var a = [1, 2, 3];  a.append(4)
来源：http://nad.pengpengdd.cyou

[T21] Swift：遍历
来源：http://xiu.sysykeji.top

for x in a { print(x) }
来源：http://kbu.chenzaomai.com

[T22] Swift：字典
来源：http://tmt.tanke756.top

var d = ["a": 1];  d["b"] = 2
来源：http://dkf.316326.xyz

[T23] Swift：函数
来源：http://mnm.guannengcc.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oya.yueranfly.top

[T24] Swift：闭包
来源：http://yfv.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://nvs.shuidangran.top

[T25] Swift：结构体
来源：http://sgs.xingfuxueyuan.xyz

struct P { var x: Int }
来源：http://bfs.yj202588.top

[T26] Swift：类与重写
来源：http://srl.dianchejie.cn

class A: Base { override func f() {} }
来源：http://mij.jqgfzy.top

[T27] Swift：错误处理
来源：http://jqk.mhx1999.top

do { try f() } catch { print(error) }
来源：http://alu.vqdsnc.cn

[T28] Swift：枚举
来源：http://mqi.zycfv.cn

enum Color { case red, green }
来源：http://twg.316326.xyz

[T29] Swift：guard 提前返回
来源：http://wez.yvedp.cn

guard let x = opt else { return }
来源：http://zfy.hnxiangtu.top

[T30] Swift：协议
来源：http://ewz.sweek.top

protocol Shape { func area() -> Double }
来源：http://ckv.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://khv.hnqzz.top

print("Hello")
来源：http://omz.nanxinkj.top

[T32] Lua：局部变量
来源：http://eye.shzxlz.cn

local a = 1
来源：http://gvx.iojbl.cn

[T33] Lua：表（数组）
来源：http://rip.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://pzz.yj202588.top

[T34] Lua：遍历表
来源：http://fsj.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ihm.ehwqpu.com

[T35] Lua：字典表
来源：http://opm.gotoacloud.top

local d = { a = 1 };  d.b = 2
来源：http://apr.ywan-chungtsiang.top

[T36] Lua：函数
来源：http://fiq.daria6918.cn

function add(a, b) return a + b end
来源：http://cmv.c1oappe.top

[T37] Lua：字符串拼接
来源：http://hvm.xinyue.icu

"a" .. "b"
来源：http://uog.redwolf501.top

[T38] Lua：条件
来源：http://wga.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://ozi.tarul.cn

[T39] Lua：模式匹配
来源：http://vxn.fktsv.cn

string.find(s, "%d+")
来源：http://lex.wangshuangyany.cn

[T40] Lua：元表
来源：http://suc.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://kch.ehwqpu.com

[T41] Perl：Hello World
来源：http://sqd.gogol.net.cn

print "Hello\n";
来源：http://qan.shanyushiyangtech.top

[T42] Perl：变量类型
来源：http://zju.jinqigfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://keu.xylfe.cn

[T43] Perl：字符串插值
来源：http://fyl.pycfn.com

"值: $a"
来源：http://yfp.cdnleiting.top

[T44] Perl：条件
来源：http://syx.ppjwa.cn

if ($a > 0) { print "正"; }
来源：http://pmb.bbcook.cn

[T45] Perl：数组遍历
来源：http://epc.hammf.cn

for my $x (@arr) { print $x; }
来源：http://rdi.gotoacloud.top

[T46] Perl：哈希操作
来源：http://jlg.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qpt.ctjpmb.com

[T47] Perl：正则捕获
来源：http://pir.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qul.hesvh.cn

[T48] Perl：正则替换
来源：http://hbw.gzhubu.top

$s =~ s/old/new/g;
来源：http://ypy.hnqzz.top

[T49] Perl：函数
来源：http://uzs.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cmo.jlsjyb.cn

[T50] Perl：逐行读文件
来源：http://eiz.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xna.svipenyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://bdz.xinyue.icu

[T51] Scala：Hello World
来源：http://xvf.fanxiaobao.xyz

println("Hello")
来源：http://rdn.smart0.xyz

[T52] Scala：变量
来源：http://uee.kuanghao11.cn

val a = 1;  var b = 2
来源：http://nhr.zycfv.cn

[T53] Scala：字符串插值
来源：http://nru.tian-w.cn

s"值: $b"
来源：http://ahp.shuidangran.top

[T54] Scala：集合映射
来源：http://eyc.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://qjp.yuanzhike.top

[T55] Scala：集合过滤
来源：http://uls.yj20258888.top

List(1, 2, 3).filter(_ > 1)
来源：http://jbl.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://vyx.zhaomingkeji.xyz

case class User(name: String, age: Int)
来源：http://yxp.daria6918.cn

[T57] Scala：模式匹配
来源：http://oyn.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gtf.yanxiufei.cn

[T58] Scala：函数定义
来源：http://pwt.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://fvj.yanxiufei.cn

[T59] Scala：循环
来源：http://cir.pycfn.com

for (i <- 1 to 10) println(i)
来源：http://wwk.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://jgr.hongshengwenyu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wye.sjlbkw.cn

================================================================================
来源：http://xlt.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ics.yvedp.cn

================================================================================
来源：http://lsm.yangfankeji.com

[U01] Py：创建虚拟环境
来源：http://bvm.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fmn.jinqigfzy.top

[U02] Py：导出 / 安装依赖
来源：http://nzn.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mxr.zhaomingkeji.xyz

[U03] Py：加载 .env 配置
来源：http://vfi.jlsjyb.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nxl.yfazqb.com

[U04] Py：变量调试打印
来源：http://rvb.52xcode.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kug.cqqwz.cn

[U05] Py：列表去重且保序
来源：http://hjr.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://nvm.guowangkeji.top

[U06] Py：合并两个字典
来源：http://iaf.epnwcf.com

{**a, **b}
来源：http://pwn.ppjwa.cn

[U07] Py：反转字典键值
来源：http://jpk.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://bwi.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://cqw.sysykeji.top

[y for x in nested for y in x]
来源：http://svc.pycfn.com

[U09] Py：字典取最大值的键
来源：http://flm.pycfn.com

max(d, key=d.get)
来源：http://wut.redwolf501.top

[U10] Py：按值排序字典
来源：http://lie.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ifw.iojbl.cn

[U11] Py：生成器表达式
来源：http://lwh.yanxiufei.cn

(x * 2 for x in arr)
来源：http://sdk.shzxlz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jht.jiagoushi.top

Counter(arr).most_common(3)
来源：http://dwr.sysykeji.top

[U13] Py：固定长度队列
来源：http://pzu.feifeiyinyue.top

deque(maxlen=10)
来源：http://zna.zdbjq.cn

[U14] Py：分组收集到列表
来源：http://shj.chenjidiqi.icu

defaultdict(list)
来源：http://pwx.ybcxt.top

[U15] Py：高精度计时
来源：http://uyq.mhx1999.top

t = time.perf_counter()
来源：http://yfb.zhaomingkeji.xyz

[U16] Py：命令行参数解析
来源：http://uvz.yanxiufei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jsw.shzxlz.cn

[U17] Py：初始化日志
来源：http://cfn.jyoumei.cn

logging.basicConfig(level=logging.INFO)
来源：http://aah.chenlongwang.top

[U18] Py：预编译正则
来源：http://ist.cqqwz.cn

pat = re.compile(r"\d+")
来源：http://urm.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://cgz.ivvv.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uej.zhoulong.xyz

[U20] Py：缓存函数结果
来源：http://uhn.yj202588.top

@functools.lru_cache(maxsize=None)
来源：http://znz.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://qym.jyoumei.cn

@contextlib.contextmanager
来源：http://yvm.bjfxy.top

[U22] Py：矩阵转置
来源：http://cep.pengpengdd.cyou

list(zip(*m))
来源：http://gem.fehbvm.com

[U23] Py：分块读取大文件
来源：http://ukb.cheryme.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ezi.guannengcc.top

[U24] Py：路径操作
来源：http://oqf.daxiang520.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hmu.yueranfly.top

[U25] Py：CSV 按字典读
来源：http://tnh.iojbl.cn

csv.DictReader(f)
来源：http://kal.sweek.top

[U26] Py：并发下载
来源：http://dqr.nanxinkj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ucr.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://job.bbcook.cn

aiohttp.ClientSession() 配合 async with
来源：http://dxo.ybcxt.top

[U28] Py：类型别名
来源：http://sdn.hnxiangtu.top

UserId = int
来源：http://nhm.wangshuangyany.cn

[U29] Py：属性校验
来源：http://wqo.shanyushiyangkeji.top

@property 与 @x.setter 配合
来源：http://ccb.zdqjudy.top

[U30] Py：数据类
来源：http://hxn.sweek.top

@dataclass(slots=True)
来源：http://xcy.iojbl.cn

[U31] Py：单测
来源：http://hva.hcnkem.com

python -m pytest -q
来源：http://rei.jlsjyb.cn

[U32] Py：代码格式化
来源：http://vap.ywan-chungtsiang.top

ruff format . && ruff check --fix .
来源：http://dvk.hnxiangtu.top

[U33] Py：打包发布
来源：http://aow.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://nhq.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://ldj.ppjwa.cn

chardet.detect(raw)
来源：http://gnd.zdbjq.cn

[U35] Py：发送邮件
来源：http://auv.ehwqpu.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tvj.xylfe.cn

[U36] Py：定时任务
来源：http://zap.shanyushiyangkeji.top

schedule.every(10).minutes.do(job)
来源：http://gui.yj20258888.top

[U37] Py：读写 Excel
来源：http://vtt.redwolf501.top

pandas.read_excel / DataFrame.to_excel
来源：http://wmc.ivvv.top

[U38] Py：获取脚本所在目录
来源：http://yyu.mhx1999.top

Path(__file__).resolve().parent
来源：http://zym.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://rtm.yj202588.top

sys.stdout.isatty()
来源：http://rcp.svipenyu.cn

[U40] Py：打印到标准错误
来源：http://hjg.yj20258.top

print("err", file=sys.stderr)
来源：http://omb.hcnkem.com

[U41] PHP：初始化 Composer 项目
来源：http://xqa.gzhubu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rxl.gogol.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://npk.smart0.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://myz.hywenlv.cn

[U43] PHP：声明命名空间
来源：http://qqm.ppjwa.cn

namespace App\Http;
来源：http://geh.xylfe.cn

[U44] PHP：开启严格类型
来源：http://kwv.jianghu66.top

declare(strict_types=1);
来源：http://juz.jqgufenzy.top

[U45] PHP：类型声明与返回类型
来源：http://nsz.aizwys.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://byo.xingfuxueyuan.xyz

[U46] PHP：可空类型
来源：http://dtk.yuanzhike.top

?string $name = null
来源：http://shn.meibo888.top

[U47] PHP：联合类型
来源：http://srj.yj20258.top

int|string $id
来源：http://xey.xylfe.cn

[U48] PHP：纯枚举
来源：http://bdx.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pgn.fktsv.cn

[U49] PHP：只读属性
来源：http://ahi.jqgufenzy.top

public readonly string $name
来源：http://xfl.cashguo.top

[U50] PHP：构造器属性提升
来源：http://hwm.gotoacloud.top

public function __construct(private int $id) {}
来源：http://sgz.ivvv.top

[U51] PHP：数组解构
来源：http://bdw.jyoumei.cn

[$a, $b] = $arr;
来源：http://ixn.yonumen.top

[U52] PHP：箭头函数
来源：http://qsx.gaohongyu789.top

$double = fn($x) => $x * 2;
来源：http://wnp.ydzc1.top

[U53] PHP：空合并运算符
来源：http://ond.yueranfly.top

$v = $a ?? $b ?? "default";
来源：http://nej.zhengqikj.top

[U54] PHP：空安全调用
来源：http://ari.bbcook.cn

$obj?->method()
来源：http://ntl.ybcxt.top

[U55] PHP：match 表达式
来源：http://lts.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rgv.jqgfzy.top

[U56] PHP：命名参数
来源：http://bnx.shzxlz.cn

f(a: 1, b: 2)
来源：http://mbr.svipenyu.cn

[U57] PHP：字符串插值
来源：http://zry.pengpengdd.cyou

"值: {$a}"
来源：http://qwk.ydjk.org.cn

[U58] PHP：数组三件套
来源：http://awf.chenlongwang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pmq.snrcjt.cn

[U59] PHP：自定义排序
来源：http://kyu.zhongyouzk.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dzz.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://fjr.chenlongwang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rmy.hammf.cn

[U61] PHP：正则
来源：http://bsb.sxryk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fiq.xinyue.icu

[U62] PHP：日期对象
来源：http://ejb.quarkkingdee.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bcp.dashuyun.cn

[U63] PHP：文件读写
来源：http://riu.epnwcf.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kva.nanxinkj.top

[U64] PHP：目录遍历
来源：http://ckx.fzhhl.top

glob("dir/*.php");  scandir("dir");
来源：http://mkv.guannengcc.top

[U65] PHP：会话
来源：http://wuw.zhixingplan.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tbn.sufxvd.cn

[U66] PHP：设置 Cookie
来源：http://rtz.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wdx.gzhubu.top

[U67] PHP：处理文件上传
来源：http://yyo.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wqk.xuanzx.com

[U68] PHP：PDO 连接
来源：http://sek.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://npp.zhaomingkeji.xyz

[U69] PHP：PDO 预处理
来源：http://bfy.jinqigfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fuh.fehbvm.com

[U70] PHP：PDO 事务
来源：http://uaw.havefunace.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mfe.jinqigufen.top

[U71] PHP：抛出异常
来源：http://cig.vqdsnc.cn

throw new RuntimeException("失败", 500);
来源：http://zsj.jinghuilouyu.cn

[U72] PHP：写错误日志
来源：http://jgx.c1oappe.top

error_log("失败: " . $e->getMessage());
来源：http://wxn.sxryk.cn


<!-- 参考信息 -->