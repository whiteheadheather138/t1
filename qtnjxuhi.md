代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tdr.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://qba.kuanghao11.cn

static_cast<double>(a) / b
来源：http://bmx.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://lia.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://oeq.zhengqikj.top

[S53] C++：移动语义
来源：http://rbt.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://jvl.hesvh.cn

[S54] C++：异常处理
来源：http://zla.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nao.shangyingyoupin.top

[S55] C++：结构化绑定
来源：http://ydk.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://ivy.wangdashe.top

[S56] C++：optional
来源：http://prt.jinqigufen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oph.guowangkeji.top

[S57] C++：编译期常量
来源：http://voc.yuanzhike.top

constexpr int N = 10;
来源：http://ocs.guannengcc.top

[S58] C++：命名空间
来源：http://byq.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://uzb.tarul.cn

[S59] C++：静态断言
来源：http://wyd.zhoulong.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wah.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://dpn.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://htm.meibo888.top

================================================================================
来源：http://gaw.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nwp.smart0.xyz

================================================================================
来源：http://bzp.yvedp.cn

[T01] Kotlin：Hello World
来源：http://lta.hnxiangtu.top

println("Hello")
来源：http://afh.yj20258888.top

[T02] Kotlin：变量
来源：http://fof.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lop.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://pup.jqgfzy.top

"值: $b"
来源：http://dqw.gogol.net.cn

[T04] Kotlin：空安全
来源：http://lar.wangshuangyany.cn

val n: String? = null;  n?.length
来源：http://eyy.andypj.xyz

[T05] Kotlin：when 表达式
来源：http://afh.yvedp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sgb.ybcxt.top

[T06] Kotlin：集合映射
来源：http://ebk.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tgf.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://gzc.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ryt.sweek.top

[T08] Kotlin：数据类
来源：http://wla.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://rrj.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://gyf.jinghuilouyu.cn

fun String.exclaim() = this + "!"
来源：http://zxl.tanke756.top

[T10] Kotlin：默认参数
来源：http://tkk.fehbvm.com

fun greet(name: String = "World") = "Hi $name"
来源：http://lxe.cucudq.cn

[T11] Kotlin：协程
来源：http://sgh.wangdashe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bcx.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://ubr.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://hga.jlsjyb.cn

[T13] Kotlin：只读 Map
来源：http://tuc.smart0.xyz

val m = mapOf("a" to 1)
来源：http://fzc.yuxming.cn

[T14] Kotlin：循环
来源：http://hfl.dashuyun.cn

for (i in 1..10) println(i)
来源：http://kya.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://bne.bbcook.cn

interface Shape { fun area(): Double }
来源：http://jen.chenzaomai.com

[T16] Swift：Hello World
来源：http://ggx.tarul.cn

print("Hello")
来源：http://swi.sxryk.cn

[T17] Swift：变量与常量
来源：http://aha.shzxlz.cn

var a = 1;  let b = 2
来源：http://ifu.sufxvd.cn

[T18] Swift：字符串插值
来源：http://jjx.fktsv.cn

"值: \(b)"
来源：http://okz.yueranfly.top

[T19] Swift：可选绑定
来源：http://fbj.epnwcf.com

if let n = opt { print(n) }
来源：http://vzt.daria6918.cn

[T20] Swift：数组操作
来源：http://cmv.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://nvn.jinqigfzy.top

[T21] Swift：遍历
来源：http://apr.jqgufenzy.top

for x in a { print(x) }
来源：http://zxm.yj20258888.top

[T22] Swift：字典
来源：http://osl.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://huk.xinyue.icu

[T23] Swift：函数
来源：http://vkf.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pig.hfpthk.cn

[T24] Swift：闭包
来源：http://esc.fehbvm.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://dyg.zhongyouzk.top

[T25] Swift：结构体
来源：http://yzc.fzhhl.top

struct P { var x: Int }
来源：http://syv.tian-w.cn

[T26] Swift：类与重写
来源：http://sdf.fzhhl.top

class A: Base { override func f() {} }
来源：http://tcj.chenlongwang.top

[T27] Swift：错误处理
来源：http://hpn.fehbvm.com

do { try f() } catch { print(error) }
来源：http://uno.gotoacloud.top

[T28] Swift：枚举
来源：http://pae.zhoulong.xyz

enum Color { case red, green }
来源：http://pcj.9152youxi.cn

[T29] Swift：guard 提前返回
来源：http://iee.epnwcf.com

guard let x = opt else { return }
来源：http://lkv.tianlin.xyz

[T30] Swift：协议
来源：http://fjg.xziqi.cn

protocol Shape { func area() -> Double }
来源：http://ohq.nanxuanxn.top

[T31] Lua：Hello World
来源：http://ndr.yonumen.top

print("Hello")
来源：http://bld.zdqjudy.top

[T32] Lua：局部变量
来源：http://hsj.ivvv.top

local a = 1
来源：http://moq.0kj1m.cn

[T33] Lua：表（数组）
来源：http://hdg.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nin.cucudq.cn

[T34] Lua：遍历表
来源：http://rar.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kap.wangshuangyany.cn

[T35] Lua：字典表
来源：http://niz.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://gnm.hesvh.cn

[T36] Lua：函数
来源：http://tvr.vqdsnc.cn

function add(a, b) return a + b end
来源：http://sgx.tianlin.xyz

[T37] Lua：字符串拼接
来源：http://you.hnqzz.top

"a" .. "b"
来源：http://rkz.snrcjt.cn

[T38] Lua：条件
来源：http://olh.dianchejie.cn

if x > 0 then print("正") end
来源：http://puk.ehwqpu.com

[T39] Lua：模式匹配
来源：http://qvd.ctjpmb.com

string.find(s, "%d+")
来源：http://bqq.jlsjyb.cn

[T40] Lua：元表
来源：http://bnu.yfazqb.com

setmetatable({}, { __index = base })
来源：http://ijp.daxiang520.top

[T41] Perl：Hello World
来源：http://llu.xuanzx.com

print "Hello\n";
来源：http://wrp.sxryk.cn

[T42] Perl：变量类型
来源：http://iul.yuxming.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tbe.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://cwu.gotoacloud.top

"值: $a"
来源：http://uan.cashguo.top

[T44] Perl：条件
来源：http://hgh.sjlbkw.cn

if ($a > 0) { print "正"; }
来源：http://wtk.sufxvd.cn

[T45] Perl：数组遍历
来源：http://nmk.fanxiaobao.xyz

for my $x (@arr) { print $x; }
来源：http://pvs.daxiang520.top

[T46] Perl：哈希操作
来源：http://uko.jinyuanbaomall.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://knq.xylfe.cn

[T47] Perl：正则捕获
来源：http://gxj.yj20258888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://cud.jianghu66.top

[T48] Perl：正则替换
来源：http://vgt.ivvv.top

$s =~ s/old/new/g;
来源：http://fiz.cashguo.top

[T49] Perl：函数
来源：http://hag.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ffx.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://orf.gogol.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lps.ppjwa.cn

while (my $line = <$fh>) { print $line; }
来源：http://uhr.sufxvd.cn

[T51] Scala：Hello World
来源：http://mys.havefunace.top

println("Hello")
来源：http://qyv.0kj1m.cn

[T52] Scala：变量
来源：http://cfh.zycfv.cn

val a = 1;  var b = 2
来源：http://pdn.cdnleiting.top

[T53] Scala：字符串插值
来源：http://fqm.xingfuxueyuan.xyz

s"值: $b"
来源：http://erm.snrcjt.cn

[T54] Scala：集合映射
来源：http://wlu.smart0.xyz

List(1, 2, 3).map(_ * 2)
来源：http://eah.yonumen.top

[T55] Scala：集合过滤
来源：http://txs.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://quw.cashguo.top

[T56] Scala：样例类
来源：http://epq.ydjk.org.cn

case class User(name: String, age: Int)
来源：http://qeq.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://nao.fktsv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hlp.dashuyun.cn

[T58] Scala：函数定义
来源：http://igu.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://ywk.bbcook.cn

[T59] Scala：循环
来源：http://meo.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://tvg.yonumen.top

[T60] Scala：折叠
来源：http://acu.jyoumei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zpe.ehwqpu.com

================================================================================
来源：http://jer.shanyushiyangtech.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zag.9152youxi.cn

================================================================================
来源：http://ift.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://eqd.yuxming.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vyd.gzhubu.top

[U02] Py：导出 / 安装依赖
来源：http://oao.ydjk.org.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://alc.ydjk.org.cn

[U03] Py：加载 .env 配置
来源：http://ivn.xingfuxueyuan.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://bpa.cheryme.top

[U04] Py：变量调试打印
来源：http://nmv.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bvq.daria6918.cn

[U05] Py：列表去重且保序
来源：http://jpu.jyoumei.cn

list(dict.fromkeys(arr))
来源：http://wqd.cashguo.top

[U06] Py：合并两个字典
来源：http://qlr.cqqwz.cn

{**a, **b}
来源：http://tzi.pycfn.com

[U07] Py：反转字典键值
来源：http://sdi.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://lcy.yfazqb.com

[U08] Py：展平二维列表
来源：http://ckm.hfpthk.cn

[y for x in nested for y in x]
来源：http://rop.xziqi.cn

[U09] Py：字典取最大值的键
来源：http://gch.tianlin.xyz

max(d, key=d.get)
来源：http://juj.c1oappe.top

[U10] Py：按值排序字典
来源：http://cip.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kwl.uphjek.com

[U11] Py：生成器表达式
来源：http://zsw.zhoulong.xyz

(x * 2 for x in arr)
来源：http://yfg.xingfuxueyuan.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://czw.yj202588.top

Counter(arr).most_common(3)
来源：http://mnv.xuanzx.com

[U13] Py：固定长度队列
来源：http://quv.aizwys.cn

deque(maxlen=10)
来源：http://xgp.xuanzx.com

[U14] Py：分组收集到列表
来源：http://yhd.316326.xyz

defaultdict(list)
来源：http://kwr.hongshengwenyu.top

[U15] Py：高精度计时
来源：http://wbu.gaohongyu789.top

t = time.perf_counter()
来源：http://xhj.xylfe.cn

[U16] Py：命令行参数解析
来源：http://bhv.jqgfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lfm.haohaochexian.top

[U17] Py：初始化日志
来源：http://upj.sweek.top

logging.basicConfig(level=logging.INFO)
来源：http://mtq.vqdsnc.cn

[U18] Py：预编译正则
来源：http://cmk.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://any.zhongyouzk.top

[U19] Py：正则替换带回调
来源：http://nzb.aibaodan.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jfu.fengsongda.top

[U20] Py：缓存函数结果
来源：http://kmh.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://sed.zhiwuduotai.top

[U21] Py：自定义上下文管理器
来源：http://hwh.c1oappe.top

@contextlib.contextmanager
来源：http://glx.xuetiantiany.cn

[U22] Py：矩阵转置
来源：http://nsi.gotoacloud.top

list(zip(*m))
来源：http://nzi.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://ohz.yvedp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yuo.zdqjudy.top

[U24] Py：路径操作
来源：http://ndw.yvedp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vue.xziqi.cn

[U25] Py：CSV 按字典读
来源：http://fjx.yuxming.cn

csv.DictReader(f)
来源：http://zzq.redwolf501.top

[U26] Py：并发下载
来源：http://kbo.shanyushiyangtech.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ckk.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://lja.sweek.top

aiohttp.ClientSession() 配合 async with
来源：http://uhj.smart0.xyz

[U28] Py：类型别名
来源：http://fky.yonumen.top

UserId = int
来源：http://ige.zhijiandao.cn

[U29] Py：属性校验
来源：http://zvz.zhaomingkeji.xyz

@property 与 @x.setter 配合
来源：http://cnh.fehbvm.com

[U30] Py：数据类
来源：http://yyv.pengpengdd.cyou

@dataclass(slots=True)
来源：http://ipc.hcnkem.com

[U31] Py：单测
来源：http://zvu.redwolf501.top

python -m pytest -q
来源：http://kgh.ydjk.org.cn

[U32] Py：代码格式化
来源：http://mjj.yueranfly.top

ruff format . && ruff check --fix .
来源：http://edr.hnxiangtu.top

[U33] Py：打包发布
来源：http://llh.daria6918.cn

python -m build  （依赖 pyproject.toml）
来源：http://rfa.cdnleiting.top

[U34] Py：判断编码
来源：http://xyo.jlsjyb.cn

chardet.detect(raw)
来源：http://mov.uphjek.com

[U35] Py：发送邮件
来源：http://vgh.snrcjt.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fax.fzhhl.top

[U36] Py：定时任务
来源：http://vhv.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://svv.fanxiaobao.xyz

[U37] Py：读写 Excel
来源：http://shv.gaohongyu789.top

pandas.read_excel / DataFrame.to_excel
来源：http://pdb.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://etf.yj20258888.top

Path(__file__).resolve().parent
来源：http://fkq.epnwcf.com

[U39] Py：判断是否在交互环境
来源：http://xfq.wangdashe.top

sys.stdout.isatty()
来源：http://gya.nwbrower.top

[U40] Py：打印到标准错误
来源：http://vwi.zdbjq.cn

print("err", file=sys.stderr)
来源：http://hod.zycfv.cn

[U41] PHP：初始化 Composer 项目
来源：http://gzn.ppjwa.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rea.pengpengdd.cyou

[U42] PHP：PSR-4 自动加载
来源：http://fub.snrcjt.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://its.mhx1999.top

[U43] PHP：声明命名空间
来源：http://tdd.ywan-chungtsiang.top

namespace App\Http;
来源：http://gpf.meibo888.top

[U44] PHP：开启严格类型
来源：http://bmg.yuxming.cn

declare(strict_types=1);
来源：http://jxh.daria6918.cn

[U45] PHP：类型声明与返回类型
来源：http://qmj.jianghu66.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mhy.yuanzhike.top

[U46] PHP：可空类型
来源：http://cdq.vehdjk.com

?string $name = null
来源：http://wfk.c1oappe.top

[U47] PHP：联合类型
来源：http://loc.fzhhl.top

int|string $id
来源：http://npf.wangdashe.top

[U48] PHP：纯枚举
来源：http://ilf.jyoumei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ohw.birdmap.top

[U49] PHP：只读属性
来源：http://cdm.fehbvm.com

public readonly string $name
来源：http://hno.jiagoushi.top

[U50] PHP：构造器属性提升
来源：http://aqy.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://dhz.9152youxi.cn

[U51] PHP：数组解构
来源：http://fpa.wangshuangyany.cn

[$a, $b] = $arr;
来源：http://vsk.ppjwa.cn

[U52] PHP：箭头函数
来源：http://wiu.smart0.xyz

$double = fn($x) => $x * 2;
来源：http://ect.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://tnj.uphjek.com

$v = $a ?? $b ?? "default";
来源：http://vle.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://udq.chenlongwang.top

$obj?->method()
来源：http://wrk.hnqzz.top

[U55] PHP：match 表达式
来源：http://viw.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jfq.hongshengwenyu.top

[U56] PHP：命名参数
来源：http://ure.bbcook.cn

f(a: 1, b: 2)
来源：http://uka.nanxinkj.top

[U57] PHP：字符串插值
来源：http://rsa.yueranfly.top

"值: {$a}"
来源：http://epx.zhongyouzk.top

[U58] PHP：数组三件套
来源：http://wsi.ehwqpu.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://flh.shanyushiyangkeji.top

[U59] PHP：自定义排序
来源：http://gha.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mec.ydjk.org.cn

[U60] PHP：JSON 编解码
来源：http://dsn.yj20258888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vij.birdmap.top

[U61] PHP：正则
来源：http://wkr.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nms.dianchejie.cn

[U62] PHP：日期对象
来源：http://eft.zhixingplan.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ypc.fanxiaobao.xyz

[U63] PHP：文件读写
来源：http://nid.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qin.dianchejie.cn

[U64] PHP：目录遍历
来源：http://ifh.zhixingplan.top

glob("dir/*.php");  scandir("dir");
来源：http://pgz.kuanghao11.cn

[U65] PHP：会话
来源：http://dda.sysykeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wfv.shuidangran.top

[U66] PHP：设置 Cookie
来源：http://jxk.xuanzx.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zdu.redwolf501.top

[U67] PHP：处理文件上传
来源：http://buj.yj20258.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kxz.tianlin.xyz

[U68] PHP：PDO 连接
来源：http://aae.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lhn.fengsongda.top

[U69] PHP：PDO 预处理
来源：http://ddr.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pyc.zhaomingkeji.xyz

[U70] PHP：PDO 事务
来源：http://wye.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dgr.fehbvm.com

[U71] PHP：抛出异常
来源：http://rcr.fengsongda.top

throw new RuntimeException("失败", 500);
来源：http://iog.gogol.net.cn

[U72] PHP：写错误日志
来源：http://hrm.jqgfzy.top

error_log("失败: " . $e->getMessage());
来源：http://zev.wangdashe.top

[U73] PHP：读取 ini 配置
来源：http://dxd.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://zgh.sweek.top

[U74] PHP：读取环境变量
来源：http://hyn.shuidangran.top

getenv("APP_ENV") ?: "production"
来源：http://elb.yj202588.top

[U75] PHP：依赖注入
来源：http://zei.ybcxt.top

composer require psr/container
来源：http://ubd.jinqigufen.top

[U76] PHP：简单路由
来源：http://soq.yuanzhike.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wsx.jinghuilouyu.cn


<!-- 参考信息 -->