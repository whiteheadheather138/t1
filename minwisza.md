代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://hng.zdbjq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qpt.jinghuilouyu.cn

[S48] C++：逐行读文件
来源：http://psc.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://new.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://pum.tianlin.xyz

[S49] C++：写文件
来源：http://cim.xziqi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://azt.yueranfly.top

[S50] C++：格式化数字
来源：http://tbk.ydzc1.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://seg.tarul.cn

[S51] C++：显式类型转换
来源：http://ovp.9152youxi.cn

static_cast<double>(a) / b
来源：http://ftv.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://iyu.ehwqpu.com

int size() const noexcept { return n_; }
来源：http://pke.chenjidiqi.icu

[S53] C++：移动语义
来源：http://jvi.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://gtf.jianghu66.top

[S54] C++：异常处理
来源：http://uzl.hesvh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ixa.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://ift.pycfn.com

auto [a, b] = std::make_pair(1, 2);
来源：http://cev.aibaodan.cn

[S56] C++：optional
来源：http://ilc.xuetiantiany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kjc.ppjwa.cn

[S57] C++：编译期常量
来源：http://vow.aizwys.cn

constexpr int N = 10;
来源：http://zex.zdbjq.cn

[S58] C++：命名空间
来源：http://qbp.shanyushiyangkeji.top

namespace ns { int f() { return 1; } }
来源：http://jar.redwolf501.top

[S59] C++：静态断言
来源：http://bjs.ybcxt.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ynd.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://ocb.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gns.yueranfly.top

================================================================================
来源：http://suj.jinghuilouyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://srg.epnwcf.com

================================================================================
来源：http://fvl.svipenyu.cn

[T01] Kotlin：Hello World
来源：http://tvi.tian-w.cn

println("Hello")
来源：http://jcv.zdbjq.cn

[T02] Kotlin：变量
来源：http://ykb.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://itv.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://fqa.dianchejie.cn

"值: $b"
来源：http://zom.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://jht.shanyushiyangtech.top

val n: String? = null;  n?.length
来源：http://tjw.birdmap.top

[T05] Kotlin：when 表达式
来源：http://wjw.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uyu.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://ggd.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mxq.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://nvs.chenzaomai.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://pzu.smart0.xyz

[T08] Kotlin：数据类
来源：http://bpq.316326.xyz

data class User(val name: String, val age: Int)
来源：http://swp.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://vdz.chenjidiqi.icu

fun String.exclaim() = this + "!"
来源：http://yyt.xziqi.cn

[T10] Kotlin：默认参数
来源：http://mlv.svipenyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bwf.gogol.net.cn

[T11] Kotlin：协程
来源：http://slh.tanke756.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rsd.guowangkeji.top

[T12] Kotlin：解构声明
来源：http://gwx.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://otg.bbcook.cn

[T13] Kotlin：只读 Map
来源：http://dyn.shuidangran.top

val m = mapOf("a" to 1)
来源：http://lmb.cqqwz.cn

[T14] Kotlin：循环
来源：http://qbj.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://rrz.ywan-chungtsiang.top

[T15] Kotlin：接口
来源：http://eek.cqqwz.cn

interface Shape { fun area(): Double }
来源：http://ejs.quarkkingdee.top

[T16] Swift：Hello World
来源：http://lle.guannengcc.top

print("Hello")
来源：http://kkw.chenlongwang.top

[T17] Swift：变量与常量
来源：http://sod.xylfe.cn

var a = 1;  let b = 2
来源：http://yof.yanxiufei.cn

[T18] Swift：字符串插值
来源：http://tkr.zhoulong.xyz

"值: \(b)"
来源：http://hvg.hammf.cn

[T19] Swift：可选绑定
来源：http://ltr.svipenyu.cn

if let n = opt { print(n) }
来源：http://nah.xuanzx.com

[T20] Swift：数组操作
来源：http://kjl.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tal.nanxuanxn.top

[T21] Swift：遍历
来源：http://rpr.chenlongwang.top

for x in a { print(x) }
来源：http://oal.dianchejie.cn

[T22] Swift：字典
来源：http://tun.havefunace.top

var d = ["a": 1];  d["b"] = 2
来源：http://dbe.xuetiantiany.cn

[T23] Swift：函数
来源：http://ogm.cucudq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gyg.yuanzhike.top

[T24] Swift：闭包
来源：http://bwe.wangdashe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://eds.tanke756.top

[T25] Swift：结构体
来源：http://zcr.ctjpmb.com

struct P { var x: Int }
来源：http://oss.hammf.cn

[T26] Swift：类与重写
来源：http://mid.fzhhl.top

class A: Base { override func f() {} }
来源：http://wax.hysaishi.cn

[T27] Swift：错误处理
来源：http://hng.gotoacloud.top

do { try f() } catch { print(error) }
来源：http://szy.birdmap.top

[T28] Swift：枚举
来源：http://yaf.aizwys.cn

enum Color { case red, green }
来源：http://rst.shuidangran.top

[T29] Swift：guard 提前返回
来源：http://fna.epnwcf.com

guard let x = opt else { return }
来源：http://ojg.wangshuangyany.cn

[T30] Swift：协议
来源：http://hat.hnxiangtu.top

protocol Shape { func area() -> Double }
来源：http://gcf.kuanghao11.cn

[T31] Lua：Hello World
来源：http://hes.hywenlv.cn

print("Hello")
来源：http://col.fehbvm.com

[T32] Lua：局部变量
来源：http://htj.yfazqb.com

local a = 1
来源：http://pcz.vehdjk.com

[T33] Lua：表（数组）
来源：http://mdq.birdmap.top

local t = {1, 2, 3};  t[4] = 4
来源：http://enb.redwolf501.top

[T34] Lua：遍历表
来源：http://ncm.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zcj.sweek.top

[T35] Lua：字典表
来源：http://hbh.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://jhl.gogol.net.cn

[T36] Lua：函数
来源：http://vwx.mhx1999.top

function add(a, b) return a + b end
来源：http://gus.nanxinkj.top

[T37] Lua：字符串拼接
来源：http://toy.cheryme.top

"a" .. "b"
来源：http://zsi.9152youxi.cn

[T38] Lua：条件
来源：http://ukf.kuanghao11.cn

if x > 0 then print("正") end
来源：http://rdu.nwbrower.top

[T39] Lua：模式匹配
来源：http://gzm.zhiwuduotai.top

string.find(s, "%d+")
来源：http://cph.nanxinkj.top

[T40] Lua：元表
来源：http://yjt.zdbjq.cn

setmetatable({}, { __index = base })
来源：http://ngs.gogol.net.cn

[T41] Perl：Hello World
来源：http://rwx.jinyuanbaomall.cn

print "Hello\n";
来源：http://ark.gotoacloud.top

[T42] Perl：变量类型
来源：http://cib.vehdjk.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vgw.yangfankeji.com

[T43] Perl：字符串插值
来源：http://jvx.jyoumei.cn

"值: $a"
来源：http://szj.jianghu66.top

[T44] Perl：条件
来源：http://fae.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://ddn.chenlongwang.top

[T45] Perl：数组遍历
来源：http://aal.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://skb.tianlin.xyz

[T46] Perl：哈希操作
来源：http://khz.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zlc.jinyuanbaomall.cn

[T47] Perl：正则捕获
来源：http://glp.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jeq.mhx1999.top

[T48] Perl：正则替换
来源：http://mat.yj202588.top

$s =~ s/old/new/g;
来源：http://uth.jianghu66.top

[T49] Perl：函数
来源：http://mif.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xhv.yonumen.top

[T50] Perl：逐行读文件
来源：http://nox.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ojq.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://dsz.svipenyu.cn

[T51] Scala：Hello World
来源：http://zrk.snrcjt.cn

println("Hello")
来源：http://thi.pengpengdd.cyou

[T52] Scala：变量
来源：http://eat.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://xmr.jlsjyb.cn

[T53] Scala：字符串插值
来源：http://jkh.nwbrower.top

s"值: $b"
来源：http://mpk.hnqzz.top

[T54] Scala：集合映射
来源：http://wnn.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://xdc.hfpthk.cn

[T55] Scala：集合过滤
来源：http://hjs.zhixingplan.top

List(1, 2, 3).filter(_ > 1)
来源：http://ukh.daxiang520.top

[T56] Scala：样例类
来源：http://ina.yj20258888.top

case class User(name: String, age: Int)
来源：http://zzc.jlsjyb.cn

[T57] Scala：模式匹配
来源：http://gei.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mmm.dianchejie.cn

[T58] Scala：函数定义
来源：http://oss.vqdsnc.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oah.0kj1m.cn

[T59] Scala：循环
来源：http://pdz.gzhubu.top

for (i <- 1 to 10) println(i)
来源：http://ovs.zhaomingkeji.xyz

[T60] Scala：折叠
来源：http://ten.chenzaomai.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gmw.yj202588.top

================================================================================
来源：http://hij.wangshuangyany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sqx.chenjidiqi.icu

================================================================================
来源：http://fiw.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://bqx.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fym.gzhubu.top

[U02] Py：导出 / 安装依赖
来源：http://yag.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qex.zhongyouzk.top

[U03] Py：加载 .env 配置
来源：http://uoi.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qys.zhaomingkeji.xyz

[U04] Py：变量调试打印
来源：http://edf.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rgi.xziqi.cn

[U05] Py：列表去重且保序
来源：http://tme.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://ppz.sxryk.cn

[U06] Py：合并两个字典
来源：http://fab.hfpthk.cn

{**a, **b}
来源：http://qkb.daxiang520.top

[U07] Py：反转字典键值
来源：http://fyu.shuidangran.top

{v: k for k, v in d.items()}
来源：http://qkt.c1oappe.top

[U08] Py：展平二维列表
来源：http://qhz.ybcxt.top

[y for x in nested for y in x]
来源：http://tto.sjlbkw.cn

[U09] Py：字典取最大值的键
来源：http://dkg.jqgufenzy.top

max(d, key=d.get)
来源：http://wxa.svipenyu.cn

[U10] Py：按值排序字典
来源：http://kco.tarul.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://riv.jiagoushi.top

[U11] Py：生成器表达式
来源：http://tht.xuetiantiany.cn

(x * 2 for x in arr)
来源：http://cpz.nanxuanxn.top

[U12] Py：取出现最多的 3 个元素
来源：http://vyr.yonumen.top

Counter(arr).most_common(3)
来源：http://prp.jyoumei.cn

[U13] Py：固定长度队列
来源：http://pmq.zdbjq.cn

deque(maxlen=10)
来源：http://ghx.svipenyu.cn

[U14] Py：分组收集到列表
来源：http://qrp.ehwqpu.com

defaultdict(list)
来源：http://scc.uphjek.com

[U15] Py：高精度计时
来源：http://xnq.zhaomingkeji.xyz

t = time.perf_counter()
来源：http://aoz.sysykeji.top

[U16] Py：命令行参数解析
来源：http://zdj.9152youxi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://khg.yfazqb.com

[U17] Py：初始化日志
来源：http://tpx.jinqigfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://zqx.yonumen.top

[U18] Py：预编译正则
来源：http://ydd.52xcode.cn

pat = re.compile(r"\d+")
来源：http://mwv.yanxiufei.cn

[U19] Py：正则替换带回调
来源：http://itq.fengsongda.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xhi.chenjidiqi.icu

[U20] Py：缓存函数结果
来源：http://nqo.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://kwn.ppjwa.cn

[U21] Py：自定义上下文管理器
来源：http://qfx.jianghu66.top

@contextlib.contextmanager
来源：http://dht.tanke756.top

[U22] Py：矩阵转置
来源：http://ayd.ppjwa.cn

list(zip(*m))
来源：http://jqz.zhengqikj.top

[U23] Py：分块读取大文件
来源：http://nlw.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hkp.zhongyouzk.top

[U24] Py：路径操作
来源：http://ocs.sweek.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tij.cqqwz.cn

[U25] Py：CSV 按字典读
来源：http://hyb.tanke756.top

csv.DictReader(f)
来源：http://hpn.yuanzhike.top

[U26] Py：并发下载
来源：http://ajm.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fgf.gzhubu.top

[U27] Py：异步 HTTP
来源：http://mvp.gzhubu.top

aiohttp.ClientSession() 配合 async with
来源：http://vyd.mhx1999.top

[U28] Py：类型别名
来源：http://swv.jianghu66.top

UserId = int
来源：http://wnw.yj20258.top

[U29] Py：属性校验
来源：http://oso.guowangkeji.top

@property 与 @x.setter 配合
来源：http://nwf.feifeiyinyue.top

[U30] Py：数据类
来源：http://rnu.epnwcf.com

@dataclass(slots=True)
来源：http://hlr.fehbvm.com

[U31] Py：单测
来源：http://fpw.guowangkeji.top

python -m pytest -q
来源：http://sss.yj20258.top

[U32] Py：代码格式化
来源：http://sqv.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://vdq.redwolf501.top

[U33] Py：打包发布
来源：http://vqg.tanke756.top

python -m build  （依赖 pyproject.toml）
来源：http://ieb.xuanzx.com

[U34] Py：判断编码
来源：http://pvk.aibaodan.cn

chardet.detect(raw)
来源：http://cre.jinqigfzy.top

[U35] Py：发送邮件
来源：http://lzt.sufxvd.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vrp.hywenlv.cn

[U36] Py：定时任务
来源：http://bjr.ydjk.org.cn

schedule.every(10).minutes.do(job)
来源：http://ryn.tarul.cn

[U37] Py：读写 Excel
来源：http://pzb.yangfankeji.com

pandas.read_excel / DataFrame.to_excel
来源：http://tnj.jianghu66.top

[U38] Py：获取脚本所在目录
来源：http://evw.ybcxt.top

Path(__file__).resolve().parent
来源：http://uhu.tarul.cn

[U39] Py：判断是否在交互环境
来源：http://nzo.yvedp.cn

sys.stdout.isatty()
来源：http://skj.yuxming.cn

[U40] Py：打印到标准错误
来源：http://kno.cashguo.top

print("err", file=sys.stderr)
来源：http://fjy.cdnleiting.top

[U41] PHP：初始化 Composer 项目
来源：http://cdf.yonumen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jnv.jqgufenzy.top

[U42] PHP：PSR-4 自动加载
来源：http://cvx.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kap.ppjwa.cn

[U43] PHP：声明命名空间
来源：http://ngk.epnwcf.com

namespace App\Http;
来源：http://isw.jinqigufen.top

[U44] PHP：开启严格类型
来源：http://bac.vehdjk.com

declare(strict_types=1);
来源：http://ydr.yj20258.top

[U45] PHP：类型声明与返回类型
来源：http://edf.hnxiangtu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xjw.meibo888.top

[U46] PHP：可空类型
来源：http://tzm.jyoumei.cn

?string $name = null
来源：http://uhb.tarul.cn

[U47] PHP：联合类型
来源：http://faa.ydzc1.top

int|string $id
来源：http://zna.hongshengwenyu.top

[U48] PHP：纯枚举
来源：http://emo.snrcjt.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://spe.zhengqikj.top

[U49] PHP：只读属性
来源：http://ddj.chenzaomai.com

public readonly string $name
来源：http://qli.sysykeji.top

[U50] PHP：构造器属性提升
来源：http://xpg.havefunace.top

public function __construct(private int $id) {}
来源：http://jef.hammf.cn

[U51] PHP：数组解构
来源：http://dll.0kj1m.cn

[$a, $b] = $arr;
来源：http://ylt.birdmap.top

[U52] PHP：箭头函数
来源：http://rrg.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://hpm.birdmap.top

[U53] PHP：空合并运算符
来源：http://fwu.fengsongda.top

$v = $a ?? $b ?? "default";
来源：http://aso.snrcjt.cn

[U54] PHP：空安全调用
来源：http://mlo.zdbjq.cn

$obj?->method()
来源：http://odr.svipenyu.cn

[U55] PHP：match 表达式
来源：http://pzl.zhiwuduotai.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bpg.ivvv.top

[U56] PHP：命名参数
来源：http://cpy.hnqzz.top

f(a: 1, b: 2)
来源：http://ukm.ybcxt.top

[U57] PHP：字符串插值
来源：http://oak.tarul.cn

"值: {$a}"
来源：http://kdg.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://cqy.guannengcc.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tng.xuetiantiany.cn

[U59] PHP：自定义排序
来源：http://rzz.shanyushiyangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xsf.birdmap.top

[U60] PHP：JSON 编解码
来源：http://bil.kuanghao11.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jst.shanyushiyangkeji.top

[U61] PHP：正则
来源：http://ybq.jinyuanbaomall.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yoa.jiagoushi.top

[U62] PHP：日期对象
来源：http://xpz.chenjidiqi.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cxp.xuetiantiany.cn

[U63] PHP：文件读写
来源：http://cxp.ywan-chungtsiang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hpy.sxryk.cn

[U64] PHP：目录遍历
来源：http://bfz.aibaodan.cn

glob("dir/*.php");  scandir("dir");
来源：http://axo.jqgufenzy.top

[U65] PHP：会话
来源：http://qee.vehdjk.com

session_start();  $_SESSION["uid"] = 1;
来源：http://lvj.hywenlv.cn

[U66] PHP：设置 Cookie
来源：http://rsy.hnqzz.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aou.0kj1m.cn

[U67] PHP：处理文件上传
来源：http://umi.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://raw.sxryk.cn

[U68] PHP：PDO 连接
来源：http://yph.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zzb.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://mxg.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ujt.hongshengwenyu.top

[U70] PHP：PDO 事务
来源：http://bdc.birdmap.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qjh.yj20258888.top

[U71] PHP：抛出异常
来源：http://ine.nanxuanxn.top

throw new RuntimeException("失败", 500);
来源：http://uct.quarkkingdee.top

[U72] PHP：写错误日志
来源：http://rbk.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://geb.pengpengdd.cyou


<!-- 参考信息 -->