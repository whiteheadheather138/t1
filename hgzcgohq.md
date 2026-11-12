代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://jdi.ivvv.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vbd.snrcjt.cn

[S48] C++：逐行读文件
来源：http://wlr.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dnb.xinyue.icu

while (std::getline(in, line)) { }
来源：http://mmv.xuanzx.com

[S49] C++：写文件
来源：http://etv.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bww.hongshengwenyu.top

[S50] C++：格式化数字
来源：http://zol.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rnu.hfpthk.cn

[S51] C++：显式类型转换
来源：http://gbg.zhijiandao.cn

static_cast<double>(a) / b
来源：http://hgx.tanke756.top

[S52] C++：const 与 noexcept
来源：http://nqg.yvedp.cn

int size() const noexcept { return n_; }
来源：http://hpb.ivvv.top

[S53] C++：移动语义
来源：http://ywa.cheryme.top

std::vector<int> w = std::move(v);
来源：http://fvz.quarkkingdee.top

[S54] C++：异常处理
来源：http://ler.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wlo.andypj.xyz

[S55] C++：结构化绑定
来源：http://wdc.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rin.yongpay.top

[S56] C++：optional
来源：http://eri.ppjwa.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yff.xuetiantiany.cn

[S57] C++：编译期常量
来源：http://mjk.cqqwz.cn

constexpr int N = 10;
来源：http://gpu.xziqi.cn

[S58] C++：命名空间
来源：http://hcw.zhijiandao.cn

namespace ns { int f() { return 1; } }
来源：http://mmn.vqdsnc.cn

[S59] C++：静态断言
来源：http://unn.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qhv.gogol.net.cn

[S60] C++：遍历并删除元素
来源：http://rck.jinqigfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uik.daxiang520.top

================================================================================
来源：http://fqs.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oul.hnxiangtu.top

================================================================================
来源：http://aud.guannengcc.top

[T01] Kotlin：Hello World
来源：http://vet.yongpay.top

println("Hello")
来源：http://djd.jinqigufen.top

[T02] Kotlin：变量
来源：http://jhy.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aac.chenzaomai.com

[T03] Kotlin：字符串模板
来源：http://mud.hnqzz.top

"值: $b"
来源：http://obb.yuanzhike.top

[T04] Kotlin：空安全
来源：http://vkx.hammf.cn

val n: String? = null;  n?.length
来源：http://lwo.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://slb.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tsx.cucudq.cn

[T06] Kotlin：集合映射
来源：http://kbg.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sti.hcnkem.com

[T07] Kotlin：集合过滤
来源：http://vuh.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ktu.jianghu66.top

[T08] Kotlin：数据类
来源：http://ieh.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://fbj.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://lpl.vehdjk.com

fun String.exclaim() = this + "!"
来源：http://slf.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://yyl.yanxiufei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rju.gzhubu.top

[T11] Kotlin：协程
来源：http://mtm.xylfe.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://olv.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://lha.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://pqy.ehwqpu.com

[T13] Kotlin：只读 Map
来源：http://jfr.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://cld.daria6918.cn

[T14] Kotlin：循环
来源：http://bpv.cucudq.cn

for (i in 1..10) println(i)
来源：http://zcb.xylfe.cn

[T15] Kotlin：接口
来源：http://sfm.316326.xyz

interface Shape { fun area(): Double }
来源：http://hke.fengsongda.top

[T16] Swift：Hello World
来源：http://gmq.shanyushiyangtech.top

print("Hello")
来源：http://hff.wangshuangyany.cn

[T17] Swift：变量与常量
来源：http://pff.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://btj.meibo888.top

[T18] Swift：字符串插值
来源：http://biu.yuanzhike.top

"值: \(b)"
来源：http://nvb.zhixingplan.top

[T19] Swift：可选绑定
来源：http://qkh.jqgufenzy.top

if let n = opt { print(n) }
来源：http://zxn.jiagoushi.top

[T20] Swift：数组操作
来源：http://ksj.aibaodan.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zvk.mhx1999.top

[T21] Swift：遍历
来源：http://rsy.haohaochexian.top

for x in a { print(x) }
来源：http://xse.shzxlz.cn

[T22] Swift：字典
来源：http://pzn.wangdashe.top

var d = ["a": 1];  d["b"] = 2
来源：http://awu.gaohongyu789.top

[T23] Swift：函数
来源：http://hav.ydzc1.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://snk.dashuyun.cn

[T24] Swift：闭包
来源：http://hux.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ria.vqdsnc.cn

[T25] Swift：结构体
来源：http://uqj.kuanghao11.cn

struct P { var x: Int }
来源：http://waa.jqgfzy.top

[T26] Swift：类与重写
来源：http://iyh.fengsongda.top

class A: Base { override func f() {} }
来源：http://fcn.ivvv.top

[T27] Swift：错误处理
来源：http://gum.xylfe.cn

do { try f() } catch { print(error) }
来源：http://htl.sxryk.cn

[T28] Swift：枚举
来源：http://eqz.sxryk.cn

enum Color { case red, green }
来源：http://pqh.zhijiandao.cn

[T29] Swift：guard 提前返回
来源：http://tpk.haohaochexian.top

guard let x = opt else { return }
来源：http://tpy.nwbrower.top

[T30] Swift：协议
来源：http://mfo.fehbvm.com

protocol Shape { func area() -> Double }
来源：http://lbd.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://oqg.nanxuanxn.top

print("Hello")
来源：http://dsv.hcnkem.com

[T32] Lua：局部变量
来源：http://wzg.birdmap.top

local a = 1
来源：http://prj.gotoacloud.top

[T33] Lua：表（数组）
来源：http://hvc.zhongyouzk.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kra.dianchejie.cn

[T34] Lua：遍历表
来源：http://uxo.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://aqx.xuanzx.com

[T35] Lua：字典表
来源：http://iii.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://tls.vqdsnc.cn

[T36] Lua：函数
来源：http://rfu.hnxiangtu.top

function add(a, b) return a + b end
来源：http://upw.tian-w.cn

[T37] Lua：字符串拼接
来源：http://aon.xuetiantiany.cn

"a" .. "b"
来源：http://oaf.ppjwa.cn

[T38] Lua：条件
来源：http://rlc.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://dte.sjlbkw.cn

[T39] Lua：模式匹配
来源：http://smx.sjlbkw.cn

string.find(s, "%d+")
来源：http://kio.tian-w.cn

[T40] Lua：元表
来源：http://vwh.xylfe.cn

setmetatable({}, { __index = base })
来源：http://dmr.cdnleiting.top

[T41] Perl：Hello World
来源：http://cmq.zhengqikj.top

print "Hello\n";
来源：http://spr.cheryme.top

[T42] Perl：变量类型
来源：http://ghz.jlsjyb.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rwy.dianchejie.cn

[T43] Perl：字符串插值
来源：http://toz.jianghu66.top

"值: $a"
来源：http://vin.hcnkem.com

[T44] Perl：条件
来源：http://bwo.jqgufenzy.top

if ($a > 0) { print "正"; }
来源：http://exe.iojbl.cn

[T45] Perl：数组遍历
来源：http://teg.cdnleiting.top

for my $x (@arr) { print $x; }
来源：http://kqw.316326.xyz

[T46] Perl：哈希操作
来源：http://zdb.cashguo.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xab.birdmap.top

[T47] Perl：正则捕获
来源：http://ebk.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://eqn.shanyushiyangtech.top

[T48] Perl：正则替换
来源：http://bhk.jiagoushi.top

$s =~ s/old/new/g;
来源：http://ewm.ctjpmb.com

[T49] Perl：函数
来源：http://qwf.jianghu66.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rbe.fengsongda.top

[T50] Perl：逐行读文件
来源：http://vyo.fengsongda.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tjl.tarul.cn

while (my $line = <$fh>) { print $line; }
来源：http://lae.zhaomingkeji.xyz

[T51] Scala：Hello World
来源：http://fgo.chenlongwang.top

println("Hello")
来源：http://ppz.sweek.top

[T52] Scala：变量
来源：http://nfy.tarul.cn

val a = 1;  var b = 2
来源：http://fjt.fktsv.cn

[T53] Scala：字符串插值
来源：http://bzg.sweek.top

s"值: $b"
来源：http://eyx.yangfankeji.com

[T54] Scala：集合映射
来源：http://fkc.cucudq.cn

List(1, 2, 3).map(_ * 2)
来源：http://snm.daria6918.cn

[T55] Scala：集合过滤
来源：http://osd.fzhhl.top

List(1, 2, 3).filter(_ > 1)
来源：http://zcx.wangdashe.top

[T56] Scala：样例类
来源：http://rav.shuidangran.top

case class User(name: String, age: Int)
来源：http://ylr.fktsv.cn

[T57] Scala：模式匹配
来源：http://nxm.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://srj.tanke756.top

[T58] Scala：函数定义
来源：http://awv.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://ctp.zhoulong.xyz

[T59] Scala：循环
来源：http://iam.jinyuanbaomall.cn

for (i <- 1 to 10) println(i)
来源：http://wdu.tianlin.xyz

[T60] Scala：折叠
来源：http://pkk.yongpay.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oto.zhaomingkeji.xyz

================================================================================
来源：http://jde.ctjpmb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fhk.yonumen.top

================================================================================
来源：http://qog.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://shv.vqdsnc.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mqc.yj20258888.top

[U02] Py：导出 / 安装依赖
来源：http://qyr.xuanzx.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xnb.ydjk.org.cn

[U03] Py：加载 .env 配置
来源：http://trp.zhiwuduotai.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tzf.redwolf501.top

[U04] Py：变量调试打印
来源：http://nsm.haohaochexian.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eir.cucudq.cn

[U05] Py：列表去重且保序
来源：http://bjr.feifeiyinyue.top

list(dict.fromkeys(arr))
来源：http://jsv.guowangkeji.top

[U06] Py：合并两个字典
来源：http://hrd.jinghuilouyu.cn

{**a, **b}
来源：http://dfj.ivvv.top

[U07] Py：反转字典键值
来源：http://meo.wangdashe.top

{v: k for k, v in d.items()}
来源：http://gtv.yanxiufei.cn

[U08] Py：展平二维列表
来源：http://azs.birdmap.top

[y for x in nested for y in x]
来源：http://shl.smart0.xyz

[U09] Py：字典取最大值的键
来源：http://riy.zhijiandao.cn

max(d, key=d.get)
来源：http://pjm.cdnleiting.top

[U10] Py：按值排序字典
来源：http://bdj.shanyushiyangtech.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wsd.andypj.xyz

[U11] Py：生成器表达式
来源：http://mck.yuxming.cn

(x * 2 for x in arr)
来源：http://equ.sysykeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://upt.pengpengdd.cyou

Counter(arr).most_common(3)
来源：http://bqf.ydjk.org.cn

[U13] Py：固定长度队列
来源：http://euq.jinghuilouyu.cn

deque(maxlen=10)
来源：http://qab.cashguo.top

[U14] Py：分组收集到列表
来源：http://nwa.chenzaomai.com

defaultdict(list)
来源：http://ymf.uphjek.com

[U15] Py：高精度计时
来源：http://xxk.epnwcf.com

t = time.perf_counter()
来源：http://kab.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://taz.cqqwz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://shm.fengsongda.top

[U17] Py：初始化日志
来源：http://wrl.jinyuanbaomall.cn

logging.basicConfig(level=logging.INFO)
来源：http://jdo.zdqjudy.top

[U18] Py：预编译正则
来源：http://ujz.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://nwo.jiagoushi.top

[U19] Py：正则替换带回调
来源：http://qjq.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jqi.meibo888.top

[U20] Py：缓存函数结果
来源：http://pmy.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://geo.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://pex.sysykeji.top

@contextlib.contextmanager
来源：http://yfw.yongpay.top

[U22] Py：矩阵转置
来源：http://vzn.chenzaomai.com

list(zip(*m))
来源：http://wrf.xuanzx.com

[U23] Py：分块读取大文件
来源：http://rie.shanyushiyangtech.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xqz.chenlongwang.top

[U24] Py：路径操作
来源：http://hya.quarkkingdee.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hvd.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://tuo.jqgfzy.top

csv.DictReader(f)
来源：http://wkv.sysykeji.top

[U26] Py：并发下载
来源：http://iju.0kj1m.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yyu.cucudq.cn

[U27] Py：异步 HTTP
来源：http://zsa.cheryme.top

aiohttp.ClientSession() 配合 async with
来源：http://zke.jyoumei.cn

[U28] Py：类型别名
来源：http://yrq.wangdashe.top

UserId = int
来源：http://wri.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://uhd.ywan-chungtsiang.top

@property 与 @x.setter 配合
来源：http://frf.jinghuilouyu.cn

[U30] Py：数据类
来源：http://wol.hysaishi.cn

@dataclass(slots=True)
来源：http://zdv.cashguo.top

[U31] Py：单测
来源：http://lfa.meibo888.top

python -m pytest -q
来源：http://ypg.pengpengdd.cyou

[U32] Py：代码格式化
来源：http://lns.vehdjk.com

ruff format . && ruff check --fix .
来源：http://yot.feifeiyinyue.top

[U33] Py：打包发布
来源：http://emk.52xcode.cn

python -m build  （依赖 pyproject.toml）
来源：http://dke.zhoulong.xyz

[U34] Py：判断编码
来源：http://htq.jinghuilouyu.cn

chardet.detect(raw)
来源：http://ixe.fehbvm.com

[U35] Py：发送邮件
来源：http://hcx.c1oappe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ace.zhongyouzk.top

[U36] Py：定时任务
来源：http://iyi.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://xti.hysaishi.cn

[U37] Py：读写 Excel
来源：http://vbc.hywenlv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jre.xziqi.cn

[U38] Py：获取脚本所在目录
来源：http://cxm.yuanzhike.top

Path(__file__).resolve().parent
来源：http://trs.feifeiyinyue.top

[U39] Py：判断是否在交互环境
来源：http://kvo.9152youxi.cn

sys.stdout.isatty()
来源：http://hee.hammf.cn

[U40] Py：打印到标准错误
来源：http://bwh.guannengcc.top

print("err", file=sys.stderr)
来源：http://aoa.vehdjk.com

[U41] PHP：初始化 Composer 项目
来源：http://psg.yvedp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qyl.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://wko.chenlongwang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gil.uphjek.com

[U43] PHP：声明命名空间
来源：http://csr.fktsv.cn

namespace App\Http;
来源：http://xqs.dianchejie.cn

[U44] PHP：开启严格类型
来源：http://xih.52xcode.cn

declare(strict_types=1);
来源：http://jkk.tanke756.top

[U45] PHP：类型声明与返回类型
来源：http://tsu.hysaishi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uoy.jlsjyb.cn

[U46] PHP：可空类型
来源：http://xjt.snrcjt.cn

?string $name = null
来源：http://ybg.xylfe.cn

[U47] PHP：联合类型
来源：http://jsx.tianlin.xyz

int|string $id
来源：http://hgh.jiagoushi.top

[U48] PHP：纯枚举
来源：http://dxq.ctjpmb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qia.zhengqikj.top

[U49] PHP：只读属性
来源：http://djz.hammf.cn

public readonly string $name
来源：http://ork.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://bvs.fzhhl.top

public function __construct(private int $id) {}
来源：http://wgi.fengsongda.top

[U51] PHP：数组解构
来源：http://fzb.shangyingyoupin.top

[$a, $b] = $arr;
来源：http://hgm.kuanghao11.cn

[U52] PHP：箭头函数
来源：http://dwy.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://itz.nanxinkj.top

[U53] PHP：空合并运算符
来源：http://wkj.ivvv.top

$v = $a ?? $b ?? "default";
来源：http://uqv.ppjwa.cn

[U54] PHP：空安全调用
来源：http://mfz.zhongyouzk.top

$obj?->method()
来源：http://efu.tanke756.top

[U55] PHP：match 表达式
来源：http://kwy.9152youxi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ngi.vehdjk.com

[U56] PHP：命名参数
来源：http://vaz.guannengcc.top

f(a: 1, b: 2)
来源：http://hye.jyoumei.cn

[U57] PHP：字符串插值
来源：http://suw.hnqzz.top

"值: {$a}"
来源：http://rim.tianlin.xyz

[U58] PHP：数组三件套
来源：http://wbk.shuidangran.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bnp.zhixingplan.top

[U59] PHP：自定义排序
来源：http://nsa.vqdsnc.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://trz.c1oappe.top

[U60] PHP：JSON 编解码
来源：http://ncu.chenlongwang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xrv.yj20258.top

[U61] PHP：正则
来源：http://xyo.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://abf.ehwqpu.com

[U62] PHP：日期对象
来源：http://lfm.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lkq.yonumen.top

[U63] PHP：文件读写
来源：http://ofn.yuanzhike.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cql.ybcxt.top

[U64] PHP：目录遍历
来源：http://jod.zhiwuduotai.top

glob("dir/*.php");  scandir("dir");
来源：http://avw.gzhubu.top

[U65] PHP：会话
来源：http://qgq.chenjidiqi.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://acm.ctjpmb.com

[U66] PHP：设置 Cookie
来源：http://nrg.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wpo.yfazqb.com

[U67] PHP：处理文件上传
来源：http://ahk.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eap.hesvh.cn

[U68] PHP：PDO 连接
来源：http://snx.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uxs.uphjek.com

[U69] PHP：PDO 预处理
来源：http://tfh.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gif.ehwqpu.com

[U70] PHP：PDO 事务
来源：http://ams.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gae.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://vfj.yuanzhike.top

throw new RuntimeException("失败", 500);
来源：http://rfv.yfazqb.com

[U72] PHP：写错误日志
来源：http://sje.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://gaq.jiagoushi.top


<!-- 参考信息 -->