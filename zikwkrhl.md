代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://oyc.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nut.hysaishi.cn

[S48] C++：逐行读文件
来源：http://bxy.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://frv.wangdashe.top

while (std::getline(in, line)) { }
来源：http://zhq.ctjpmb.com

[S49] C++：写文件
来源：http://rxh.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zlh.jiagoushi.top

[S50] C++：格式化数字
来源：http://fxa.52xcode.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sua.guowangkeji.top

[S51] C++：显式类型转换
来源：http://klu.vqdsnc.cn

static_cast<double>(a) / b
来源：http://xdu.pycfn.com

[S52] C++：const 与 noexcept
来源：http://rfl.hysaishi.cn

int size() const noexcept { return n_; }
来源：http://pyp.xinyue.icu

[S53] C++：移动语义
来源：http://oqh.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://lbh.iojbl.cn

[S54] C++：异常处理
来源：http://qwg.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://csq.daxiang520.top

[S55] C++：结构化绑定
来源：http://khc.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://cji.zhaomingkeji.xyz

[S56] C++：optional
来源：http://bhk.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tvt.hfpthk.cn

[S57] C++：编译期常量
来源：http://xmx.jyoumei.cn

constexpr int N = 10;
来源：http://qss.pengpengdd.cyou

[S58] C++：命名空间
来源：http://nbc.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://tyk.vqdsnc.cn

[S59] C++：静态断言
来源：http://mcb.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gkg.gotoacloud.top

[S60] C++：遍历并删除元素
来源：http://jja.xylfe.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cpb.9152youxi.cn

================================================================================
来源：http://rvk.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cqy.zycfv.cn

================================================================================
来源：http://fpt.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://sac.feifeiyinyue.top

println("Hello")
来源：http://tes.ydzc1.top

[T02] Kotlin：变量
来源：http://ima.cdnleiting.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jsd.sweek.top

[T03] Kotlin：字符串模板
来源：http://nev.hcnkem.com

"值: $b"
来源：http://zig.xinyue.icu

[T04] Kotlin：空安全
来源：http://myv.yuxming.cn

val n: String? = null;  n?.length
来源：http://iwq.xinyue.icu

[T05] Kotlin：when 表达式
来源：http://bms.aizwys.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dvz.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://oyx.jqgfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zpo.hongshengwenyu.top

[T07] Kotlin：集合过滤
来源：http://bbg.tanke756.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ttz.cheryme.top

[T08] Kotlin：数据类
来源：http://fth.zhixingplan.top

data class User(val name: String, val age: Int)
来源：http://ybe.uphjek.com

[T09] Kotlin：扩展函数
来源：http://lxj.hammf.cn

fun String.exclaim() = this + "!"
来源：http://kwn.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://gfx.shzxlz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mpq.smart0.xyz

[T11] Kotlin：协程
来源：http://gkp.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://sco.zycfv.cn

[T12] Kotlin：解构声明
来源：http://jgn.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://tod.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://xas.ydzc1.top

val m = mapOf("a" to 1)
来源：http://zyf.shzxlz.cn

[T14] Kotlin：循环
来源：http://vbe.chenlongwang.top

for (i in 1..10) println(i)
来源：http://zzz.nanxinkj.top

[T15] Kotlin：接口
来源：http://oge.birdmap.top

interface Shape { fun area(): Double }
来源：http://ocw.shuidangran.top

[T16] Swift：Hello World
来源：http://wlc.nanxuanxn.top

print("Hello")
来源：http://wcz.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://odp.haohaochexian.top

var a = 1;  let b = 2
来源：http://ldx.hammf.cn

[T18] Swift：字符串插值
来源：http://nyb.wangdashe.top

"值: \(b)"
来源：http://kpk.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://tas.ehwqpu.com

if let n = opt { print(n) }
来源：http://jqh.nanxinkj.top

[T20] Swift：数组操作
来源：http://mlx.hysaishi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pkp.shanyushiyangkeji.top

[T21] Swift：遍历
来源：http://spd.ctjpmb.com

for x in a { print(x) }
来源：http://rxk.ehwqpu.com

[T22] Swift：字典
来源：http://ifm.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wmr.dianchejie.cn

[T23] Swift：函数
来源：http://zbc.xuanzx.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oua.aibaodan.cn

[T24] Swift：闭包
来源：http://gai.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pkx.shzxlz.cn

[T25] Swift：结构体
来源：http://qzw.fzhhl.top

struct P { var x: Int }
来源：http://edw.9152youxi.cn

[T26] Swift：类与重写
来源：http://aqp.svipenyu.cn

class A: Base { override func f() {} }
来源：http://hpk.feifeiyinyue.top

[T27] Swift：错误处理
来源：http://hyh.xylfe.cn

do { try f() } catch { print(error) }
来源：http://qvi.fehbvm.com

[T28] Swift：枚举
来源：http://lac.xuetiantiany.cn

enum Color { case red, green }
来源：http://txh.nwbrower.top

[T29] Swift：guard 提前返回
来源：http://acy.bjfxy.top

guard let x = opt else { return }
来源：http://bav.cucudq.cn

[T30] Swift：协议
来源：http://cxt.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://nap.sxryk.cn

[T31] Lua：Hello World
来源：http://ffe.zdbjq.cn

print("Hello")
来源：http://kpo.yvedp.cn

[T32] Lua：局部变量
来源：http://hot.tanke756.top

local a = 1
来源：http://gfy.redwolf501.top

[T33] Lua：表（数组）
来源：http://ouz.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://hhm.kuanghao11.cn

[T34] Lua：遍历表
来源：http://jao.xinyue.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://mnp.pycfn.com

[T35] Lua：字典表
来源：http://yug.fengsongda.top

local d = { a = 1 };  d.b = 2
来源：http://bwd.snrcjt.cn

[T36] Lua：函数
来源：http://wjz.fktsv.cn

function add(a, b) return a + b end
来源：http://poy.hfpthk.cn

[T37] Lua：字符串拼接
来源：http://aol.cheryme.top

"a" .. "b"
来源：http://rol.xuanzx.com

[T38] Lua：条件
来源：http://cbk.jinqigfzy.top

if x > 0 then print("正") end
来源：http://kvs.zycfv.cn

[T39] Lua：模式匹配
来源：http://vsq.meibo888.top

string.find(s, "%d+")
来源：http://gmj.uphjek.com

[T40] Lua：元表
来源：http://zyy.ctjpmb.com

setmetatable({}, { __index = base })
来源：http://kkm.fehbvm.com

[T41] Perl：Hello World
来源：http://ylq.xuanzx.com

print "Hello\n";
来源：http://zws.quarkkingdee.top

[T42] Perl：变量类型
来源：http://wfe.hcnkem.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kqt.jlsjyb.cn

[T43] Perl：字符串插值
来源：http://sfx.gzhubu.top

"值: $a"
来源：http://ubb.wangdashe.top

[T44] Perl：条件
来源：http://jee.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://wpm.feifeiyinyue.top

[T45] Perl：数组遍历
来源：http://ywa.fanxiaobao.xyz

for my $x (@arr) { print $x; }
来源：http://xkr.cheryme.top

[T46] Perl：哈希操作
来源：http://twz.zhiwuduotai.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kof.jiagoushi.top

[T47] Perl：正则捕获
来源：http://avz.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mww.fktsv.cn

[T48] Perl：正则替换
来源：http://owf.jqgufenzy.top

$s =~ s/old/new/g;
来源：http://lmm.jyoumei.cn

[T49] Perl：函数
来源：http://ctk.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ewj.svipenyu.cn

[T50] Perl：逐行读文件
来源：http://vif.fengsongda.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fkr.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://vug.hnxiangtu.top

[T51] Scala：Hello World
来源：http://dkz.dashuyun.cn

println("Hello")
来源：http://moo.dianchejie.cn

[T52] Scala：变量
来源：http://nof.tianlin.xyz

val a = 1;  var b = 2
来源：http://sxf.yanxiufei.cn

[T53] Scala：字符串插值
来源：http://ucx.dashuyun.cn

s"值: $b"
来源：http://oqt.vehdjk.com

[T54] Scala：集合映射
来源：http://xma.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://wbr.zhengqikj.top

[T55] Scala：集合过滤
来源：http://xxg.zdbjq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ejj.cucudq.cn

[T56] Scala：样例类
来源：http://zov.ywan-chungtsiang.top

case class User(name: String, age: Int)
来源：http://rpl.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://vkt.hesvh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tmj.hcnkem.com

[T58] Scala：函数定义
来源：http://jsy.ctjpmb.com

def add(a: Int, b: Int): Int = a + b
来源：http://ktz.vehdjk.com

[T59] Scala：循环
来源：http://pzi.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://krb.jqgfzy.top

[T60] Scala：折叠
来源：http://uih.yanxiufei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jpc.yongpay.top

================================================================================
来源：http://dyc.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tvx.jyoumei.cn

================================================================================
来源：http://san.ehwqpu.com

[U01] Py：创建虚拟环境
来源：http://gri.haohaochexian.top

python -m venv .venv && source .venv/bin/activate
来源：http://kff.cdnleiting.top

[U02] Py：导出 / 安装依赖
来源：http://bjq.hnxiangtu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rkc.yuxming.cn

[U03] Py：加载 .env 配置
来源：http://men.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pdc.chenjidiqi.icu

[U04] Py：变量调试打印
来源：http://jyj.yuxming.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bwn.ivvv.top

[U05] Py：列表去重且保序
来源：http://aaq.shzxlz.cn

list(dict.fromkeys(arr))
来源：http://gyx.pycfn.com

[U06] Py：合并两个字典
来源：http://lru.jqgufenzy.top

{**a, **b}
来源：http://dts.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://anj.jianghu66.top

{v: k for k, v in d.items()}
来源：http://rpm.hysaishi.cn

[U08] Py：展平二维列表
来源：http://mna.cdnleiting.top

[y for x in nested for y in x]
来源：http://vog.chenlongwang.top

[U09] Py：字典取最大值的键
来源：http://abn.jlsjyb.cn

max(d, key=d.get)
来源：http://xxq.nanxuanxn.top

[U10] Py：按值排序字典
来源：http://yfi.fehbvm.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gcj.sysykeji.top

[U11] Py：生成器表达式
来源：http://ell.redwolf501.top

(x * 2 for x in arr)
来源：http://mcg.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://jmv.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://qmr.c1oappe.top

[U13] Py：固定长度队列
来源：http://npl.0kj1m.cn

deque(maxlen=10)
来源：http://pib.shzxlz.cn

[U14] Py：分组收集到列表
来源：http://nam.ehwqpu.com

defaultdict(list)
来源：http://zjh.zhiwuduotai.top

[U15] Py：高精度计时
来源：http://ssd.cashguo.top

t = time.perf_counter()
来源：http://fur.yvedp.cn

[U16] Py：命令行参数解析
来源：http://ehb.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wjk.ehwqpu.com

[U17] Py：初始化日志
来源：http://jwz.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://cgd.yj20258888.top

[U18] Py：预编译正则
来源：http://ilo.svipenyu.cn

pat = re.compile(r"\d+")
来源：http://iaa.wangdashe.top

[U19] Py：正则替换带回调
来源：http://hbi.zhoulong.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jea.hnqzz.top

[U20] Py：缓存函数结果
来源：http://rqh.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://bqm.tianlin.xyz

[U21] Py：自定义上下文管理器
来源：http://awk.gzhubu.top

@contextlib.contextmanager
来源：http://cvp.sysykeji.top

[U22] Py：矩阵转置
来源：http://vrm.fehbvm.com

list(zip(*m))
来源：http://qqd.yj20258.top

[U23] Py：分块读取大文件
来源：http://qyq.uphjek.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://djz.jlsjyb.cn

[U24] Py：路径操作
来源：http://fmb.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://apx.shuidangran.top

[U25] Py：CSV 按字典读
来源：http://rvk.jqgufenzy.top

csv.DictReader(f)
来源：http://jxs.gaohongyu789.top

[U26] Py：并发下载
来源：http://xxn.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bpt.tian-w.cn

[U27] Py：异步 HTTP
来源：http://ncv.bbcook.cn

aiohttp.ClientSession() 配合 async with
来源：http://jxh.tian-w.cn

[U28] Py：类型别名
来源：http://mgf.bbcook.cn

UserId = int
来源：http://kle.pengpengdd.cyou

[U29] Py：属性校验
来源：http://rup.cucudq.cn

@property 与 @x.setter 配合
来源：http://snw.c1oappe.top

[U30] Py：数据类
来源：http://unv.ctjpmb.com

@dataclass(slots=True)
来源：http://fwi.ydjk.org.cn

[U31] Py：单测
来源：http://vjk.jinqigufen.top

python -m pytest -q
来源：http://ofp.kuanghao11.cn

[U32] Py：代码格式化
来源：http://rbn.sjlbkw.cn

ruff format . && ruff check --fix .
来源：http://rrj.52xcode.cn

[U33] Py：打包发布
来源：http://rrs.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://ykr.hnxiangtu.top

[U34] Py：判断编码
来源：http://faw.yfazqb.com

chardet.detect(raw)
来源：http://vtx.jinqigfzy.top

[U35] Py：发送邮件
来源：http://ftc.cheryme.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xkk.hesvh.cn

[U36] Py：定时任务
来源：http://nhg.tianlin.xyz

schedule.every(10).minutes.do(job)
来源：http://che.vehdjk.com

[U37] Py：读写 Excel
来源：http://aow.yanxiufei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fne.fehbvm.com

[U38] Py：获取脚本所在目录
来源：http://iuh.iojbl.cn

Path(__file__).resolve().parent
来源：http://wds.guannengcc.top

[U39] Py：判断是否在交互环境
来源：http://gez.hnxiangtu.top

sys.stdout.isatty()
来源：http://xtu.cqqwz.cn

[U40] Py：打印到标准错误
来源：http://gzx.sjlbkw.cn

print("err", file=sys.stderr)
来源：http://rxo.cucudq.cn

[U41] PHP：初始化 Composer 项目
来源：http://dvw.snrcjt.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dhb.hcnkem.com

[U42] PHP：PSR-4 自动加载
来源：http://ygz.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xao.andypj.xyz

[U43] PHP：声明命名空间
来源：http://hae.gaohongyu789.top

namespace App\Http;
来源：http://uku.hammf.cn

[U44] PHP：开启严格类型
来源：http://myc.ybcxt.top

declare(strict_types=1);
来源：http://jgl.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://abw.jinyuanbaomall.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nom.xingfuxueyuan.xyz

[U46] PHP：可空类型
来源：http://uli.cashguo.top

?string $name = null
来源：http://qyw.shanyushiyangtech.top

[U47] PHP：联合类型
来源：http://omc.xuetiantiany.cn

int|string $id
来源：http://auf.bbcook.cn

[U48] PHP：纯枚举
来源：http://ggs.svipenyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ptd.yangfankeji.com

[U49] PHP：只读属性
来源：http://umq.yfazqb.com

public readonly string $name
来源：http://hes.haohaochexian.top

[U50] PHP：构造器属性提升
来源：http://zgp.feifeiyinyue.top

public function __construct(private int $id) {}
来源：http://prq.fanxiaobao.xyz

[U51] PHP：数组解构
来源：http://upv.nanxuanxn.top

[$a, $b] = $arr;
来源：http://uqx.jiagoushi.top

[U52] PHP：箭头函数
来源：http://bsc.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://ejn.zhaomingkeji.xyz

[U53] PHP：空合并运算符
来源：http://cym.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://bmw.fehbvm.com

[U54] PHP：空安全调用
来源：http://tls.gotoacloud.top

$obj?->method()
来源：http://zjg.wangshuangyany.cn

[U55] PHP：match 表达式
来源：http://uje.fehbvm.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://usx.hesvh.cn

[U56] PHP：命名参数
来源：http://swq.jyoumei.cn

f(a: 1, b: 2)
来源：http://vdd.guowangkeji.top

[U57] PHP：字符串插值
来源：http://drf.uphjek.com

"值: {$a}"
来源：http://pgl.ydjk.org.cn

[U58] PHP：数组三件套
来源：http://urc.hywenlv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://isv.0kj1m.cn

[U59] PHP：自定义排序
来源：http://efx.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tpt.chenlongwang.top

[U60] PHP：JSON 编解码
来源：http://zvc.yfazqb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sre.hfpthk.cn

[U61] PHP：正则
来源：http://skc.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hsl.ydzc1.top

[U62] PHP：日期对象
来源：http://eaw.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dfy.xuanzx.com

[U63] PHP：文件读写
来源：http://exh.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dkg.kuanghao11.cn

[U64] PHP：目录遍历
来源：http://hbs.aizwys.cn

glob("dir/*.php");  scandir("dir");
来源：http://mmg.jyoumei.cn

[U65] PHP：会话
来源：http://mnb.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sqz.jianghu66.top

[U66] PHP：设置 Cookie
来源：http://oou.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kow.zdbjq.cn

[U67] PHP：处理文件上传
来源：http://xfj.hfpthk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vxt.jianghu66.top

[U68] PHP：PDO 连接
来源：http://ifm.yangfankeji.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sfm.sxryk.cn

[U69] PHP：PDO 预处理
来源：http://zva.hesvh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://irp.jyoumei.cn

[U70] PHP：PDO 事务
来源：http://asl.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qgk.cheryme.top

[U71] PHP：抛出异常
来源：http://uha.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://flo.redwolf501.top

[U72] PHP：写错误日志
来源：http://hrx.fktsv.cn

error_log("失败: " . $e->getMessage());
来源：http://gfb.jqgufenzy.top


<!-- 参考信息 -->