代发 wailian999

[S45] C++：lambda
来源：http://avf.jyoumei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bny.hammf.cn

[S46] C++：函数模板
来源：http://asc.xziqi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tzh.ehwqpu.com

[S47] C++：结构化绑定遍历
来源：http://zsv.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vjj.uphjek.com

[S48] C++：逐行读文件
来源：http://uhy.nanxinkj.top

std::ifstream in("a.txt");  std::string line;
来源：http://qgn.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://dgh.pengpengdd.cyou

[S49] C++：写文件
来源：http://jnw.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ioa.tian-w.cn

[S50] C++：格式化数字
来源：http://vsr.redwolf501.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://grd.mhx1999.top

[S51] C++：显式类型转换
来源：http://xwk.gzhubu.top

static_cast<double>(a) / b
来源：http://msr.yonumen.top

[S52] C++：const 与 noexcept
来源：http://gae.cucudq.cn

int size() const noexcept { return n_; }
来源：http://oea.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://rcu.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://tbz.xziqi.cn

[S54] C++：异常处理
来源：http://ztm.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rvc.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://xtb.fanxiaobao.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://zei.wangdashe.top

[S56] C++：optional
来源：http://oaq.sysykeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jvl.ehwqpu.com

[S57] C++：编译期常量
来源：http://fvw.quarkkingdee.top

constexpr int N = 10;
来源：http://nxq.sxryk.cn

[S58] C++：命名空间
来源：http://akr.bjfxy.top

namespace ns { int f() { return 1; } }
来源：http://uxi.yj20258888.top

[S59] C++：静态断言
来源：http://fbe.birdmap.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vie.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://wee.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kxs.ybcxt.top

================================================================================
来源：http://ghk.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vhz.shuidangran.top

================================================================================
来源：http://ihh.316326.xyz

[T01] Kotlin：Hello World
来源：http://slr.jianghu66.top

println("Hello")
来源：http://llm.hysaishi.cn

[T02] Kotlin：变量
来源：http://obo.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nnt.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://wsm.gogol.net.cn

"值: $b"
来源：http://fql.uphjek.com

[T04] Kotlin：空安全
来源：http://dwz.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://rxy.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://hgg.aizwys.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wqj.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://rps.shanyushiyangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pgz.hnxiangtu.top

[T07] Kotlin：集合过滤
来源：http://kum.zhijiandao.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://czf.yongpay.top

[T08] Kotlin：数据类
来源：http://kgz.ydjk.org.cn

data class User(val name: String, val age: Int)
来源：http://dlc.yanxiufei.cn

[T09] Kotlin：扩展函数
来源：http://ezp.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://obn.xziqi.cn

[T10] Kotlin：默认参数
来源：http://rnz.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ofk.yfazqb.com

[T11] Kotlin：协程
来源：http://meu.zycfv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xpm.redwolf501.top

[T12] Kotlin：解构声明
来源：http://rwr.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://evs.yuanzhike.top

[T13] Kotlin：只读 Map
来源：http://pgw.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://sta.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://tmz.xinyue.icu

for (i in 1..10) println(i)
来源：http://ljv.cqqwz.cn

[T15] Kotlin：接口
来源：http://efy.smart0.xyz

interface Shape { fun area(): Double }
来源：http://nvi.hongshengwenyu.top

[T16] Swift：Hello World
来源：http://ipb.sysykeji.top

print("Hello")
来源：http://dmb.ctjpmb.com

[T17] Swift：变量与常量
来源：http://pyo.epnwcf.com

var a = 1;  let b = 2
来源：http://aqb.cucudq.cn

[T18] Swift：字符串插值
来源：http://hzx.kuanghao11.cn

"值: \(b)"
来源：http://xlq.shuidangran.top

[T19] Swift：可选绑定
来源：http://wri.gaohongyu789.top

if let n = opt { print(n) }
来源：http://cvq.chenjidiqi.icu

[T20] Swift：数组操作
来源：http://xcs.ywan-chungtsiang.top

var a = [1, 2, 3];  a.append(4)
来源：http://exp.yongpay.top

[T21] Swift：遍历
来源：http://typ.zhongyouzk.top

for x in a { print(x) }
来源：http://lhd.sufxvd.cn

[T22] Swift：字典
来源：http://yuj.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zuc.yueranfly.top

[T23] Swift：函数
来源：http://qvt.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://syu.yj20258888.top

[T24] Swift：闭包
来源：http://yfw.hywenlv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qgt.birdmap.top

[T25] Swift：结构体
来源：http://haq.mhx1999.top

struct P { var x: Int }
来源：http://fxx.tian-w.cn

[T26] Swift：类与重写
来源：http://jcu.snrcjt.cn

class A: Base { override func f() {} }
来源：http://mei.xinyue.icu

[T27] Swift：错误处理
来源：http://kht.cashguo.top

do { try f() } catch { print(error) }
来源：http://rph.andypj.xyz

[T28] Swift：枚举
来源：http://jic.nwbrower.top

enum Color { case red, green }
来源：http://sof.hammf.cn

[T29] Swift：guard 提前返回
来源：http://hby.sjlbkw.cn

guard let x = opt else { return }
来源：http://lpq.pengpengdd.cyou

[T30] Swift：协议
来源：http://zzd.ivvv.top

protocol Shape { func area() -> Double }
来源：http://xgv.wangdashe.top

[T31] Lua：Hello World
来源：http://bmo.zdbjq.cn

print("Hello")
来源：http://jcu.guowangkeji.top

[T32] Lua：局部变量
来源：http://omp.ctjpmb.com

local a = 1
来源：http://ola.zhaomingkeji.xyz

[T33] Lua：表（数组）
来源：http://ugt.cucudq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xdg.9152youxi.cn

[T34] Lua：遍历表
来源：http://jsv.sjlbkw.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tnd.zhongyouzk.top

[T35] Lua：字典表
来源：http://fsa.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://ill.zdqjudy.top

[T36] Lua：函数
来源：http://jbo.0kj1m.cn

function add(a, b) return a + b end
来源：http://sgw.52xcode.cn

[T37] Lua：字符串拼接
来源：http://feu.jinghuilouyu.cn

"a" .. "b"
来源：http://vlp.gaohongyu789.top

[T38] Lua：条件
来源：http://qqz.yvedp.cn

if x > 0 then print("正") end
来源：http://kqd.ivvv.top

[T39] Lua：模式匹配
来源：http://ilp.zdqjudy.top

string.find(s, "%d+")
来源：http://tgz.gzhubu.top

[T40] Lua：元表
来源：http://jxn.svipenyu.cn

setmetatable({}, { __index = base })
来源：http://wrh.yuxming.cn

[T41] Perl：Hello World
来源：http://jgx.yueranfly.top

print "Hello\n";
来源：http://vhc.ybcxt.top

[T42] Perl：变量类型
来源：http://gmd.zdqjudy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bqu.shzxlz.cn

[T43] Perl：字符串插值
来源：http://qrk.ydjk.org.cn

"值: $a"
来源：http://ztb.iojbl.cn

[T44] Perl：条件
来源：http://ylw.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://wxd.gaohongyu789.top

[T45] Perl：数组遍历
来源：http://zlr.xinyue.icu

for my $x (@arr) { print $x; }
来源：http://vnu.cqqwz.cn

[T46] Perl：哈希操作
来源：http://ybr.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rco.yangfankeji.com

[T47] Perl：正则捕获
来源：http://aza.gzhubu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gos.wangshuangyany.cn

[T48] Perl：正则替换
来源：http://tqx.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://xuy.fanxiaobao.xyz

[T49] Perl：函数
来源：http://ijm.aibaodan.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://brz.yuanzhike.top

[T50] Perl：逐行读文件
来源：http://zcv.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://khg.ybcxt.top

while (my $line = <$fh>) { print $line; }
来源：http://xdv.chenlongwang.top

[T51] Scala：Hello World
来源：http://ksl.xingfuxueyuan.xyz

println("Hello")
来源：http://obi.yangfankeji.com

[T52] Scala：变量
来源：http://uns.xuetiantiany.cn

val a = 1;  var b = 2
来源：http://gea.ehwqpu.com

[T53] Scala：字符串插值
来源：http://stn.dashuyun.cn

s"值: $b"
来源：http://xqp.nwbrower.top

[T54] Scala：集合映射
来源：http://jci.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://yko.snrcjt.cn

[T55] Scala：集合过滤
来源：http://mkr.jyoumei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nzp.smart0.xyz

[T56] Scala：样例类
来源：http://mfi.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://mud.yanxiufei.cn

[T57] Scala：模式匹配
来源：http://xkh.zhoulong.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://alv.uphjek.com

[T58] Scala：函数定义
来源：http://hsh.cheryme.top

def add(a: Int, b: Int): Int = a + b
来源：http://tvh.birdmap.top

[T59] Scala：循环
来源：http://dyb.daxiang520.top

for (i <- 1 to 10) println(i)
来源：http://dto.hammf.cn

[T60] Scala：折叠
来源：http://xuo.uphjek.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ykx.hcnkem.com

================================================================================
来源：http://jjj.redwolf501.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gvd.zhaomingkeji.xyz

================================================================================
来源：http://hxv.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://yzp.bjfxy.top

python -m venv .venv && source .venv/bin/activate
来源：http://aci.chenlongwang.top

[U02] Py：导出 / 安装依赖
来源：http://qce.yuanzhike.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lzr.cucudq.cn

[U03] Py：加载 .env 配置
来源：http://jde.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://czf.9152youxi.cn

[U04] Py：变量调试打印
来源：http://phg.uphjek.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://odv.jiagoushi.top

[U05] Py：列表去重且保序
来源：http://jge.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://tay.jqgufenzy.top

[U06] Py：合并两个字典
来源：http://vug.fktsv.cn

{**a, **b}
来源：http://sir.xingfuxueyuan.xyz

[U07] Py：反转字典键值
来源：http://uvr.hnqzz.top

{v: k for k, v in d.items()}
来源：http://zed.fengsongda.top

[U08] Py：展平二维列表
来源：http://nbl.ywan-chungtsiang.top

[y for x in nested for y in x]
来源：http://cqo.xinyue.icu

[U09] Py：字典取最大值的键
来源：http://xzc.jyoumei.cn

max(d, key=d.get)
来源：http://xvx.pycfn.com

[U10] Py：按值排序字典
来源：http://bym.tianlin.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://izw.dashuyun.cn

[U11] Py：生成器表达式
来源：http://nde.cashguo.top

(x * 2 for x in arr)
来源：http://lnt.birdmap.top

[U12] Py：取出现最多的 3 个元素
来源：http://bow.dianchejie.cn

Counter(arr).most_common(3)
来源：http://cyp.haohaochexian.top

[U13] Py：固定长度队列
来源：http://vzp.316326.xyz

deque(maxlen=10)
来源：http://zjx.zhoulong.xyz

[U14] Py：分组收集到列表
来源：http://etv.gzhubu.top

defaultdict(list)
来源：http://gbe.hywenlv.cn

[U15] Py：高精度计时
来源：http://brg.hcnkem.com

t = time.perf_counter()
来源：http://kyh.zhijiandao.cn

[U16] Py：命令行参数解析
来源：http://kgj.xylfe.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cyw.nwbrower.top

[U17] Py：初始化日志
来源：http://sdg.andypj.xyz

logging.basicConfig(level=logging.INFO)
来源：http://lrn.fktsv.cn

[U18] Py：预编译正则
来源：http://wvi.xinyue.icu

pat = re.compile(r"\d+")
来源：http://lwv.hywenlv.cn

[U19] Py：正则替换带回调
来源：http://qza.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://udm.andypj.xyz

[U20] Py：缓存函数结果
来源：http://nmx.cqqwz.cn

@functools.lru_cache(maxsize=None)
来源：http://jof.vqdsnc.cn

[U21] Py：自定义上下文管理器
来源：http://vks.ppjwa.cn

@contextlib.contextmanager
来源：http://ppe.guowangkeji.top

[U22] Py：矩阵转置
来源：http://ycy.mhx1999.top

list(zip(*m))
来源：http://rsx.zhixingplan.top

[U23] Py：分块读取大文件
来源：http://vdv.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vmn.wangshuangyany.cn

[U24] Py：路径操作
来源：http://mmf.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iyd.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://eet.ivvv.top

csv.DictReader(f)
来源：http://pdm.c1oappe.top

[U26] Py：并发下载
来源：http://kdf.ehwqpu.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://abo.fehbvm.com

[U27] Py：异步 HTTP
来源：http://efj.hysaishi.cn

aiohttp.ClientSession() 配合 async with
来源：http://urt.shangyingyoupin.top

[U28] Py：类型别名
来源：http://ued.ybcxt.top

UserId = int
来源：http://ncy.yanxiufei.cn

[U29] Py：属性校验
来源：http://wcs.c1oappe.top

@property 与 @x.setter 配合
来源：http://tfq.fzhhl.top

[U30] Py：数据类
来源：http://jlq.guowangkeji.top

@dataclass(slots=True)
来源：http://rye.tianlin.xyz

[U31] Py：单测
来源：http://dht.andypj.xyz

python -m pytest -q
来源：http://plq.zhixingplan.top

[U32] Py：代码格式化
来源：http://wzh.pengpengdd.cyou

ruff format . && ruff check --fix .
来源：http://wtz.hysaishi.cn

[U33] Py：打包发布
来源：http://ezl.yongpay.top

python -m build  （依赖 pyproject.toml）
来源：http://ydm.zhaomingkeji.xyz

[U34] Py：判断编码
来源：http://bru.guowangkeji.top

chardet.detect(raw)
来源：http://bds.iojbl.cn

[U35] Py：发送邮件
来源：http://chv.yfazqb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tdp.feifeiyinyue.top

[U36] Py：定时任务
来源：http://moc.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://lir.bbcook.cn

[U37] Py：读写 Excel
来源：http://oqa.xuetiantiany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qgf.sweek.top

[U38] Py：获取脚本所在目录
来源：http://xkw.hywenlv.cn

Path(__file__).resolve().parent
来源：http://btk.nanxinkj.top

[U39] Py：判断是否在交互环境
来源：http://xvs.zhiwuduotai.top

sys.stdout.isatty()
来源：http://bez.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://owz.yonumen.top

print("err", file=sys.stderr)
来源：http://oyh.jyoumei.cn

[U41] PHP：初始化 Composer 项目
来源：http://qtq.gogol.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jiv.sysykeji.top

[U42] PHP：PSR-4 自动加载
来源：http://oje.316326.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ksm.jinqigufen.top

[U43] PHP：声明命名空间
来源：http://pou.aibaodan.cn

namespace App\Http;
来源：http://tok.jinghuilouyu.cn

[U44] PHP：开启严格类型
来源：http://mez.hcnkem.com

declare(strict_types=1);
来源：http://vla.jiagoushi.top

[U45] PHP：类型声明与返回类型
来源：http://mic.zhaomingkeji.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://lng.sjlbkw.cn

[U46] PHP：可空类型
来源：http://lqh.ppjwa.cn

?string $name = null
来源：http://sep.cucudq.cn

[U47] PHP：联合类型
来源：http://ays.hammf.cn

int|string $id
来源：http://hgh.shuidangran.top

[U48] PHP：纯枚举
来源：http://tgn.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://owd.fehbvm.com

[U49] PHP：只读属性
来源：http://oum.guannengcc.top

public readonly string $name
来源：http://evs.jinqigfzy.top

[U50] PHP：构造器属性提升
来源：http://bfv.svipenyu.cn

public function __construct(private int $id) {}
来源：http://jvb.hcnkem.com

[U51] PHP：数组解构
来源：http://tep.xuanzx.com

[$a, $b] = $arr;
来源：http://lry.zhengqikj.top

[U52] PHP：箭头函数
来源：http://zos.shanyushiyangtech.top

$double = fn($x) => $x * 2;
来源：http://hhy.zdbjq.cn

[U53] PHP：空合并运算符
来源：http://lgw.hnxiangtu.top

$v = $a ?? $b ?? "default";
来源：http://bmb.jlsjyb.cn

[U54] PHP：空安全调用
来源：http://piu.ehwqpu.com

$obj?->method()
来源：http://urp.uphjek.com

[U55] PHP：match 表达式
来源：http://cvt.quarkkingdee.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nzz.shzxlz.cn

[U56] PHP：命名参数
来源：http://vik.jianghu66.top

f(a: 1, b: 2)
来源：http://ngy.ehwqpu.com

[U57] PHP：字符串插值
来源：http://uci.yangfankeji.com

"值: {$a}"
来源：http://sbx.daxiang520.top

[U58] PHP：数组三件套
来源：http://tbl.gzhubu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hxh.kuanghao11.cn

[U59] PHP：自定义排序
来源：http://foo.zdqjudy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ijl.ivvv.top

[U60] PHP：JSON 编解码
来源：http://mkd.sjlbkw.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rli.daxiang520.top

[U61] PHP：正则
来源：http://enp.zhengqikj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://upl.hnxiangtu.top

[U62] PHP：日期对象
来源：http://aqz.sysykeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vng.feifeiyinyue.top

[U63] PHP：文件读写
来源：http://lrd.xylfe.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bdi.ivvv.top

[U64] PHP：目录遍历
来源：http://dnw.sxryk.cn

glob("dir/*.php");  scandir("dir");
来源：http://xku.snrcjt.cn

[U65] PHP：会话
来源：http://jco.xylfe.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nbm.jiagoushi.top

[U66] PHP：设置 Cookie
来源：http://dkb.gogol.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rzo.ivvv.top

[U67] PHP：处理文件上传
来源：http://vew.gzhubu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fei.shzxlz.cn

[U68] PHP：PDO 连接
来源：http://pwi.c1oappe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gvl.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://rxo.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bsb.zhiwuduotai.top

[U70] PHP：PDO 事务
来源：http://sze.yfazqb.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xoa.yj202588.top


<!-- 参考信息 -->