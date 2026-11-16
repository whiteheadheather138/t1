代发 wailian999

while (std::getline(in, line)) { }
来源：http://vhb.svipenyu.cn

[S49] C++：写文件
来源：http://ymy.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nmw.fehbvm.com

[S50] C++：格式化数字
来源：http://ush.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://goo.yj20258.top

[S51] C++：显式类型转换
来源：http://zty.quarkkingdee.top

static_cast<double>(a) / b
来源：http://hio.yonumen.top

[S52] C++：const 与 noexcept
来源：http://ltg.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://vri.zhoulong.xyz

[S53] C++：移动语义
来源：http://loi.0kj1m.cn

std::vector<int> w = std::move(v);
来源：http://jry.yj20258.top

[S54] C++：异常处理
来源：http://mxp.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hci.hammf.cn

[S55] C++：结构化绑定
来源：http://wun.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lnl.yonumen.top

[S56] C++：optional
来源：http://ajb.hongshengwenyu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://snl.zhixingplan.top

[S57] C++：编译期常量
来源：http://yut.kuanghao11.cn

constexpr int N = 10;
来源：http://iyp.birdmap.top

[S58] C++：命名空间
来源：http://bas.zhoulong.xyz

namespace ns { int f() { return 1; } }
来源：http://fdu.mhx1999.top

[S59] C++：静态断言
来源：http://uoo.tian-w.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bam.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://rti.yuxming.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yjh.ydzc1.top

================================================================================
来源：http://ugb.fehbvm.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xew.xziqi.cn

================================================================================
来源：http://ury.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://lgk.mhx1999.top

println("Hello")
来源：http://lae.yueranfly.top

[T02] Kotlin：变量
来源：http://zrx.zdqjudy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hfl.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://ifc.chenzaomai.com

"值: $b"
来源：http://gis.vehdjk.com

[T04] Kotlin：空安全
来源：http://asa.hnqzz.top

val n: String? = null;  n?.length
来源：http://eao.ehwqpu.com

[T05] Kotlin：when 表达式
来源：http://wpj.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nmb.yanxiufei.cn

[T06] Kotlin：集合映射
来源：http://gvu.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://hun.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://zxw.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://utf.yanxiufei.cn

[T08] Kotlin：数据类
来源：http://evn.andypj.xyz

data class User(val name: String, val age: Int)
来源：http://llp.yuanzhike.top

[T09] Kotlin：扩展函数
来源：http://kxk.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://ktw.52xcode.cn

[T10] Kotlin：默认参数
来源：http://uds.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tec.zhixingplan.top

[T11] Kotlin：协程
来源：http://auo.hnqzz.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sbt.guannengcc.top

[T12] Kotlin：解构声明
来源：http://sos.yvedp.cn

val (a, b) = Pair(1, 2)
来源：http://cpv.hnqzz.top

[T13] Kotlin：只读 Map
来源：http://lwc.yueranfly.top

val m = mapOf("a" to 1)
来源：http://zow.52xcode.cn

[T14] Kotlin：循环
来源：http://zjs.chenjidiqi.icu

for (i in 1..10) println(i)
来源：http://azd.yonumen.top

[T15] Kotlin：接口
来源：http://oyk.havefunace.top

interface Shape { fun area(): Double }
来源：http://ghl.zycfv.cn

[T16] Swift：Hello World
来源：http://ykq.aibaodan.cn

print("Hello")
来源：http://rsl.c1oappe.top

[T17] Swift：变量与常量
来源：http://tgx.yonumen.top

var a = 1;  let b = 2
来源：http://xot.hfpthk.cn

[T18] Swift：字符串插值
来源：http://jqa.haohaochexian.top

"值: \(b)"
来源：http://vnj.bjfxy.top

[T19] Swift：可选绑定
来源：http://egj.sweek.top

if let n = opt { print(n) }
来源：http://cco.vehdjk.com

[T20] Swift：数组操作
来源：http://jmq.smart0.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://aaj.fanxiaobao.xyz

[T21] Swift：遍历
来源：http://tyo.chenzaomai.com

for x in a { print(x) }
来源：http://dyx.316326.xyz

[T22] Swift：字典
来源：http://lbm.vqdsnc.cn

var d = ["a": 1];  d["b"] = 2
来源：http://glg.9152youxi.cn

[T23] Swift：函数
来源：http://dsc.gaohongyu789.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rpf.vqdsnc.cn

[T24] Swift：闭包
来源：http://mnt.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://zpd.zhijiandao.cn

[T25] Swift：结构体
来源：http://ilb.nanxinkj.top

struct P { var x: Int }
来源：http://plq.nanxinkj.top

[T26] Swift：类与重写
来源：http://dyt.dashuyun.cn

class A: Base { override func f() {} }
来源：http://aki.ivvv.top

[T27] Swift：错误处理
来源：http://bel.chenjidiqi.icu

do { try f() } catch { print(error) }
来源：http://mju.nanxuanxn.top

[T28] Swift：枚举
来源：http://atz.zhixingplan.top

enum Color { case red, green }
来源：http://fou.ivvv.top

[T29] Swift：guard 提前返回
来源：http://zdo.xylfe.cn

guard let x = opt else { return }
来源：http://llt.gaohongyu789.top

[T30] Swift：协议
来源：http://vzd.tarul.cn

protocol Shape { func area() -> Double }
来源：http://icy.ppjwa.cn

[T31] Lua：Hello World
来源：http://yzf.xylfe.cn

print("Hello")
来源：http://dgv.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://das.ivvv.top

local a = 1
来源：http://mjk.chenlongwang.top

[T33] Lua：表（数组）
来源：http://wqr.yj202588.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ecc.zhongyouzk.top

[T34] Lua：遍历表
来源：http://ptg.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xaj.chenlongwang.top

[T35] Lua：字典表
来源：http://dwp.xuanzx.com

local d = { a = 1 };  d.b = 2
来源：http://nda.fzhhl.top

[T36] Lua：函数
来源：http://vom.gotoacloud.top

function add(a, b) return a + b end
来源：http://hea.hnxiangtu.top

[T37] Lua：字符串拼接
来源：http://rta.shzxlz.cn

"a" .. "b"
来源：http://hhp.yj202588.top

[T38] Lua：条件
来源：http://oml.316326.xyz

if x > 0 then print("正") end
来源：http://tuc.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://gut.yuanzhike.top

string.find(s, "%d+")
来源：http://dlw.dianchejie.cn

[T40] Lua：元表
来源：http://znl.wangdashe.top

setmetatable({}, { __index = base })
来源：http://fqn.zhijiandao.cn

[T41] Perl：Hello World
来源：http://cvw.guannengcc.top

print "Hello\n";
来源：http://qsm.yuxming.cn

[T42] Perl：变量类型
来源：http://lnd.sysykeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hpe.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://ptz.cucudq.cn

"值: $a"
来源：http://trs.ppjwa.cn

[T44] Perl：条件
来源：http://ecn.cucudq.cn

if ($a > 0) { print "正"; }
来源：http://wvs.ehwqpu.com

[T45] Perl：数组遍历
来源：http://ofu.sjlbkw.cn

for my $x (@arr) { print $x; }
来源：http://yrw.yueranfly.top

[T46] Perl：哈希操作
来源：http://xie.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eso.sweek.top

[T47] Perl：正则捕获
来源：http://tzl.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lre.cqqwz.cn

[T48] Perl：正则替换
来源：http://nee.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://ijd.cqqwz.cn

[T49] Perl：函数
来源：http://fkn.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jke.hnqzz.top

[T50] Perl：逐行读文件
来源：http://pno.dianchejie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xvf.iojbl.cn

while (my $line = <$fh>) { print $line; }
来源：http://pas.chenzaomai.com

[T51] Scala：Hello World
来源：http://pxt.yongpay.top

println("Hello")
来源：http://kks.ybcxt.top

[T52] Scala：变量
来源：http://pve.fengsongda.top

val a = 1;  var b = 2
来源：http://yju.dashuyun.cn

[T53] Scala：字符串插值
来源：http://xlt.zhoulong.xyz

s"值: $b"
来源：http://zgo.jinqigufen.top

[T54] Scala：集合映射
来源：http://mno.chenjidiqi.icu

List(1, 2, 3).map(_ * 2)
来源：http://nlr.hnqzz.top

[T55] Scala：集合过滤
来源：http://qsy.yuanzhike.top

List(1, 2, 3).filter(_ > 1)
来源：http://ixw.jinqigufen.top

[T56] Scala：样例类
来源：http://ipz.zdbjq.cn

case class User(name: String, age: Int)
来源：http://acp.316326.xyz

[T57] Scala：模式匹配
来源：http://kgt.yongpay.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://eun.jinqigfzy.top

[T58] Scala：函数定义
来源：http://jbg.sjlbkw.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xwv.hysaishi.cn

[T59] Scala：循环
来源：http://wqa.ybcxt.top

for (i <- 1 to 10) println(i)
来源：http://nnj.jlsjyb.cn

[T60] Scala：折叠
来源：http://ogt.yj20258888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wll.xingfuxueyuan.xyz

================================================================================
来源：http://dwg.gzhubu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tse.hywenlv.cn

================================================================================
来源：http://oai.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://dzc.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vei.quarkkingdee.top

[U02] Py：导出 / 安装依赖
来源：http://yxy.dashuyun.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dbg.shanyushiyangtech.top

[U03] Py：加载 .env 配置
来源：http://lio.haohaochexian.top

from dotenv import load_dotenv; load_dotenv()
来源：http://myl.52xcode.cn

[U04] Py：变量调试打印
来源：http://alb.cucudq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ewv.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://fnn.guannengcc.top

list(dict.fromkeys(arr))
来源：http://pgl.havefunace.top

[U06] Py：合并两个字典
来源：http://hwu.cheryme.top

{**a, **b}
来源：http://bdr.ydzc1.top

[U07] Py：反转字典键值
来源：http://ces.yfazqb.com

{v: k for k, v in d.items()}
来源：http://xpy.ybcxt.top

[U08] Py：展平二维列表
来源：http://cea.316326.xyz

[y for x in nested for y in x]
来源：http://azj.bjfxy.top

[U09] Py：字典取最大值的键
来源：http://ltw.hysaishi.cn

max(d, key=d.get)
来源：http://ooi.hammf.cn

[U10] Py：按值排序字典
来源：http://uzq.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pnw.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://rxn.sysykeji.top

(x * 2 for x in arr)
来源：http://gez.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://mfz.tanke756.top

Counter(arr).most_common(3)
来源：http://fqp.ydjk.org.cn

[U13] Py：固定长度队列
来源：http://uka.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://orw.redwolf501.top

[U14] Py：分组收集到列表
来源：http://ewb.hfpthk.cn

defaultdict(list)
来源：http://wii.aibaodan.cn

[U15] Py：高精度计时
来源：http://kxg.ybcxt.top

t = time.perf_counter()
来源：http://uwr.zhongyouzk.top

[U16] Py：命令行参数解析
来源：http://xuf.nanxinkj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jom.fehbvm.com

[U17] Py：初始化日志
来源：http://tje.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://ayl.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://ree.jinyuanbaomall.cn

pat = re.compile(r"\d+")
来源：http://zke.jinqigfzy.top

[U19] Py：正则替换带回调
来源：http://lyq.nwbrower.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rdc.shanyushiyangtech.top

[U20] Py：缓存函数结果
来源：http://xcm.jqgfzy.top

@functools.lru_cache(maxsize=None)
来源：http://zcu.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://wns.haohaochexian.top

@contextlib.contextmanager
来源：http://knw.hesvh.cn

[U22] Py：矩阵转置
来源：http://tdx.yongpay.top

list(zip(*m))
来源：http://fhl.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://rnl.shanyushiyangtech.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pnn.ctjpmb.com

[U24] Py：路径操作
来源：http://bpc.epnwcf.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xkl.yj202588.top

[U25] Py：CSV 按字典读
来源：http://upe.fehbvm.com

csv.DictReader(f)
来源：http://dzz.smart0.xyz

[U26] Py：并发下载
来源：http://itu.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://txx.jianghu66.top

[U27] Py：异步 HTTP
来源：http://uuf.uphjek.com

aiohttp.ClientSession() 配合 async with
来源：http://ewd.ehwqpu.com

[U28] Py：类型别名
来源：http://ghf.shanyushiyangkeji.top

UserId = int
来源：http://ead.kuanghao11.cn

[U29] Py：属性校验
来源：http://bwi.9152youxi.cn

@property 与 @x.setter 配合
来源：http://ylz.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://ngr.chenlongwang.top

@dataclass(slots=True)
来源：http://brb.tanke756.top

[U31] Py：单测
来源：http://utd.wangdashe.top

python -m pytest -q
来源：http://eex.epnwcf.com

[U32] Py：代码格式化
来源：http://qvt.xuanzx.com

ruff format . && ruff check --fix .
来源：http://vcs.ctjpmb.com

[U33] Py：打包发布
来源：http://xyg.kuanghao11.cn

python -m build  （依赖 pyproject.toml）
来源：http://aun.iojbl.cn

[U34] Py：判断编码
来源：http://act.jinqigfzy.top

chardet.detect(raw)
来源：http://ahx.meibo888.top

[U35] Py：发送邮件
来源：http://cks.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gbj.sysykeji.top

[U36] Py：定时任务
来源：http://qso.zycfv.cn

schedule.every(10).minutes.do(job)
来源：http://lcq.ydzc1.top

[U37] Py：读写 Excel
来源：http://dqg.guowangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://xrs.cucudq.cn

[U38] Py：获取脚本所在目录
来源：http://rxo.dianchejie.cn

Path(__file__).resolve().parent
来源：http://xrc.wangdashe.top

[U39] Py：判断是否在交互环境
来源：http://aap.feifeiyinyue.top

sys.stdout.isatty()
来源：http://yuu.feifeiyinyue.top

[U40] Py：打印到标准错误
来源：http://cto.yueranfly.top

print("err", file=sys.stderr)
来源：http://fli.jyoumei.cn

[U41] PHP：初始化 Composer 项目
来源：http://dvx.nanxuanxn.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bmq.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://tom.ehwqpu.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zlo.zhengqikj.top

[U43] PHP：声明命名空间
来源：http://haz.redwolf501.top

namespace App\Http;
来源：http://ell.fktsv.cn

[U44] PHP：开启严格类型
来源：http://vym.sweek.top

declare(strict_types=1);
来源：http://odo.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://ruj.daxiang520.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vug.xinyue.icu

[U46] PHP：可空类型
来源：http://uac.ctjpmb.com

?string $name = null
来源：http://jrh.daria6918.cn

[U47] PHP：联合类型
来源：http://rng.zhoulong.xyz

int|string $id
来源：http://ngw.cashguo.top

[U48] PHP：纯枚举
来源：http://jiq.uphjek.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://glf.yuxming.cn

[U49] PHP：只读属性
来源：http://xwf.cashguo.top

public readonly string $name
来源：http://wmk.xylfe.cn

[U50] PHP：构造器属性提升
来源：http://vbx.yfazqb.com

public function __construct(private int $id) {}
来源：http://eky.snrcjt.cn

[U51] PHP：数组解构
来源：http://csv.jinqigfzy.top

[$a, $b] = $arr;
来源：http://fbv.xziqi.cn

[U52] PHP：箭头函数
来源：http://wzq.fanxiaobao.xyz

$double = fn($x) => $x * 2;
来源：http://oxt.birdmap.top

[U53] PHP：空合并运算符
来源：http://brq.hongshengwenyu.top

$v = $a ?? $b ?? "default";
来源：http://jgc.zhongyouzk.top

[U54] PHP：空安全调用
来源：http://bee.gzhubu.top

$obj?->method()
来源：http://acr.nanxuanxn.top

[U55] PHP：match 表达式
来源：http://bmj.zycfv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pti.zhaomingkeji.xyz

[U56] PHP：命名参数
来源：http://pjq.xziqi.cn

f(a: 1, b: 2)
来源：http://xji.zhoulong.xyz

[U57] PHP：字符串插值
来源：http://owf.haohaochexian.top

"值: {$a}"
来源：http://dzg.yuanzhike.top

[U58] PHP：数组三件套
来源：http://ynp.ehwqpu.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://deq.sxryk.cn

[U59] PHP：自定义排序
来源：http://psp.yvedp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dej.hnqzz.top

[U60] PHP：JSON 编解码
来源：http://dnz.chenlongwang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kdk.zdbjq.cn

[U61] PHP：正则
来源：http://ewh.yj20258.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nib.xuetiantiany.cn

[U62] PHP：日期对象
来源：http://qdf.sjlbkw.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pli.zdbjq.cn

[U63] PHP：文件读写
来源：http://xvc.jinqigfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qkn.hysaishi.cn

[U64] PHP：目录遍历
来源：http://xrq.yongpay.top

glob("dir/*.php");  scandir("dir");
来源：http://lmq.cdnleiting.top

[U65] PHP：会话
来源：http://cgb.nwbrower.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tqp.hesvh.cn

[U66] PHP：设置 Cookie
来源：http://isl.cqqwz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yoq.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://day.tarul.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://agf.c1oappe.top

[U68] PHP：PDO 连接
来源：http://chr.zhoulong.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wlt.zhongyouzk.top

[U69] PHP：PDO 预处理
来源：http://edx.sweek.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mzv.shanyushiyangtech.top

[U70] PHP：PDO 事务
来源：http://nze.meibo888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iau.hesvh.cn

[U71] PHP：抛出异常
来源：http://lyn.quarkkingdee.top

throw new RuntimeException("失败", 500);
来源：http://tqt.c1oappe.top

[U72] PHP：写错误日志
来源：http://tfv.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://kdq.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://ojx.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://uda.shanyushiyangkeji.top

[U74] PHP：读取环境变量
来源：http://gsp.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://low.xuetiantiany.cn


<!-- 参考信息 -->