代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://mfm.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iyv.ppjwa.cn

[S48] C++：逐行读文件
来源：http://fww.shangyingyoupin.top

std::ifstream in("a.txt");  std::string line;
来源：http://oau.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://niq.epnwcf.com

[S49] C++：写文件
来源：http://vwa.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yki.snrcjt.cn

[S50] C++：格式化数字
来源：http://szx.yonumen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://duk.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://hpk.zhongyouzk.top

static_cast<double>(a) / b
来源：http://wbt.nanxinkj.top

[S52] C++：const 与 noexcept
来源：http://rcn.cheryme.top

int size() const noexcept { return n_; }
来源：http://ngk.jinqigufen.top

[S53] C++：移动语义
来源：http://znx.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://jrm.xinyue.icu

[S54] C++：异常处理
来源：http://ihk.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zjo.yj20258888.top

[S55] C++：结构化绑定
来源：http://ept.zdbjq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zvd.yvedp.cn

[S56] C++：optional
来源：http://usd.nanxinkj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hns.cucudq.cn

[S57] C++：编译期常量
来源：http://fle.xylfe.cn

constexpr int N = 10;
来源：http://orw.jinqigufen.top

[S58] C++：命名空间
来源：http://sgq.yj202588.top

namespace ns { int f() { return 1; } }
来源：http://qev.zhaomingkeji.xyz

[S59] C++：静态断言
来源：http://ekd.ydzc1.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dea.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://oyl.andypj.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gwe.jianghu66.top

================================================================================
来源：http://lqx.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vya.aibaodan.cn

================================================================================
来源：http://cvv.tanke756.top

[T01] Kotlin：Hello World
来源：http://ksl.ctjpmb.com

println("Hello")
来源：http://zfw.gzhubu.top

[T02] Kotlin：变量
来源：http://lfm.chenjidiqi.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hie.tarul.cn

[T03] Kotlin：字符串模板
来源：http://kwk.wangdashe.top

"值: $b"
来源：http://esb.dashuyun.cn

[T04] Kotlin：空安全
来源：http://wbj.hnqzz.top

val n: String? = null;  n?.length
来源：http://agk.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://efg.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://usz.sysykeji.top

[T06] Kotlin：集合映射
来源：http://ltn.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nnc.hongshengwenyu.top

[T07] Kotlin：集合过滤
来源：http://uzv.316326.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://zvd.chenlongwang.top

[T08] Kotlin：数据类
来源：http://qzw.quarkkingdee.top

data class User(val name: String, val age: Int)
来源：http://noh.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://pew.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://vbu.sysykeji.top

[T10] Kotlin：默认参数
来源：http://nqo.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://eex.c1oappe.top

[T11] Kotlin：协程
来源：http://xpp.pengpengdd.cyou

GlobalScope.launch { delay(1000); println("done") }
来源：http://xfm.kuanghao11.cn

[T12] Kotlin：解构声明
来源：http://rtg.jqgufenzy.top

val (a, b) = Pair(1, 2)
来源：http://aif.pengpengdd.cyou

[T13] Kotlin：只读 Map
来源：http://uuk.fktsv.cn

val m = mapOf("a" to 1)
来源：http://hwy.fzhhl.top

[T14] Kotlin：循环
来源：http://bkz.hysaishi.cn

for (i in 1..10) println(i)
来源：http://odn.jianghu66.top

[T15] Kotlin：接口
来源：http://aaq.xziqi.cn

interface Shape { fun area(): Double }
来源：http://xfj.svipenyu.cn

[T16] Swift：Hello World
来源：http://xhg.pengpengdd.cyou

print("Hello")
来源：http://lpm.feifeiyinyue.top

[T17] Swift：变量与常量
来源：http://lxh.yj202588.top

var a = 1;  let b = 2
来源：http://cly.cucudq.cn

[T18] Swift：字符串插值
来源：http://nbz.shanyushiyangtech.top

"值: \(b)"
来源：http://awz.daria6918.cn

[T19] Swift：可选绑定
来源：http://hbq.yj20258888.top

if let n = opt { print(n) }
来源：http://stf.guannengcc.top

[T20] Swift：数组操作
来源：http://yeg.kuanghao11.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xrc.yanxiufei.cn

[T21] Swift：遍历
来源：http://xer.hfpthk.cn

for x in a { print(x) }
来源：http://bhn.yuxming.cn

[T22] Swift：字典
来源：http://lfx.jqgfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://amb.tianlin.xyz

[T23] Swift：函数
来源：http://bqn.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ctm.havefunace.top

[T24] Swift：闭包
来源：http://zqi.jlsjyb.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pqm.yueranfly.top

[T25] Swift：结构体
来源：http://tsy.sxryk.cn

struct P { var x: Int }
来源：http://ltg.xuanzx.com

[T26] Swift：类与重写
来源：http://slh.hnxiangtu.top

class A: Base { override func f() {} }
来源：http://jsn.jinqigfzy.top

[T27] Swift：错误处理
来源：http://jdb.vqdsnc.cn

do { try f() } catch { print(error) }
来源：http://ndz.gaohongyu789.top

[T28] Swift：枚举
来源：http://sgm.tianlin.xyz

enum Color { case red, green }
来源：http://aqd.chenjidiqi.icu

[T29] Swift：guard 提前返回
来源：http://wjr.yongpay.top

guard let x = opt else { return }
来源：http://uuo.ehwqpu.com

[T30] Swift：协议
来源：http://zsz.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://bei.gaohongyu789.top

[T31] Lua：Hello World
来源：http://ssm.shuidangran.top

print("Hello")
来源：http://rec.hywenlv.cn

[T32] Lua：局部变量
来源：http://ucm.mhx1999.top

local a = 1
来源：http://ddl.yonumen.top

[T33] Lua：表（数组）
来源：http://hry.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kvv.zhengqikj.top

[T34] Lua：遍历表
来源：http://jam.ivvv.top

for i, v in ipairs(t) do print(i, v) end
来源：http://flz.fanxiaobao.xyz

[T35] Lua：字典表
来源：http://gum.sjlbkw.cn

local d = { a = 1 };  d.b = 2
来源：http://vxb.hnxiangtu.top

[T36] Lua：函数
来源：http://jxh.zhongyouzk.top

function add(a, b) return a + b end
来源：http://yst.svipenyu.cn

[T37] Lua：字符串拼接
来源：http://ogt.jiagoushi.top

"a" .. "b"
来源：http://oir.smart0.xyz

[T38] Lua：条件
来源：http://gyz.meibo888.top

if x > 0 then print("正") end
来源：http://rbn.shuidangran.top

[T39] Lua：模式匹配
来源：http://muf.ydzc1.top

string.find(s, "%d+")
来源：http://vmz.wangdashe.top

[T40] Lua：元表
来源：http://aak.hnqzz.top

setmetatable({}, { __index = base })
来源：http://ufc.smart0.xyz

[T41] Perl：Hello World
来源：http://xiu.aibaodan.cn

print "Hello\n";
来源：http://haq.zdqjudy.top

[T42] Perl：变量类型
来源：http://ibj.gzhubu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tmo.daria6918.cn

[T43] Perl：字符串插值
来源：http://ypy.yvedp.cn

"值: $a"
来源：http://wbe.shzxlz.cn

[T44] Perl：条件
来源：http://lvo.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://grd.yanxiufei.cn

[T45] Perl：数组遍历
来源：http://rqn.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://xen.nanxuanxn.top

[T46] Perl：哈希操作
来源：http://swq.chenzaomai.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uwo.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://vtu.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oqy.jqgufenzy.top

[T48] Perl：正则替换
来源：http://dir.pengpengdd.cyou

$s =~ s/old/new/g;
来源：http://zer.kuanghao11.cn

[T49] Perl：函数
来源：http://aaz.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xbe.hongshengwenyu.top

[T50] Perl：逐行读文件
来源：http://odg.yj202588.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bjg.cdnleiting.top

while (my $line = <$fh>) { print $line; }
来源：http://tsr.hesvh.cn

[T51] Scala：Hello World
来源：http://sjy.zhiwuduotai.top

println("Hello")
来源：http://rsz.vqdsnc.cn

[T52] Scala：变量
来源：http://yui.hammf.cn

val a = 1;  var b = 2
来源：http://eoc.jyoumei.cn

[T53] Scala：字符串插值
来源：http://csj.cheryme.top

s"值: $b"
来源：http://qba.cheryme.top

[T54] Scala：集合映射
来源：http://ncf.yj202588.top

List(1, 2, 3).map(_ * 2)
来源：http://flx.yangfankeji.com

[T55] Scala：集合过滤
来源：http://cgj.yongpay.top

List(1, 2, 3).filter(_ > 1)
来源：http://ypq.tian-w.cn

[T56] Scala：样例类
来源：http://xfp.meibo888.top

case class User(name: String, age: Int)
来源：http://thr.bjfxy.top

[T57] Scala：模式匹配
来源：http://fdy.aizwys.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pxt.hcnkem.com

[T58] Scala：函数定义
来源：http://kyr.jinyuanbaomall.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lob.fktsv.cn

[T59] Scala：循环
来源：http://qdt.hesvh.cn

for (i <- 1 to 10) println(i)
来源：http://puv.vqdsnc.cn

[T60] Scala：折叠
来源：http://uul.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://smy.dashuyun.cn

================================================================================
来源：http://vpg.fktsv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zoy.zhiwuduotai.top

================================================================================
来源：http://yfl.fzhhl.top

[U01] Py：创建虚拟环境
来源：http://ahx.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zyg.dianchejie.cn

[U02] Py：导出 / 安装依赖
来源：http://qcv.mhx1999.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oug.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://hsw.9152youxi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uja.wangshuangyany.cn

[U04] Py：变量调试打印
来源：http://yuz.hesvh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vvc.sweek.top

[U05] Py：列表去重且保序
来源：http://syj.havefunace.top

list(dict.fromkeys(arr))
来源：http://ryv.sweek.top

[U06] Py：合并两个字典
来源：http://ehd.guowangkeji.top

{**a, **b}
来源：http://ghq.hnxiangtu.top

[U07] Py：反转字典键值
来源：http://rfg.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://reh.sweek.top

[U08] Py：展平二维列表
来源：http://rdd.zdbjq.cn

[y for x in nested for y in x]
来源：http://eiw.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://eey.shuidangran.top

max(d, key=d.get)
来源：http://jtn.c1oappe.top

[U10] Py：按值排序字典
来源：http://phy.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qjq.jinqigufen.top

[U11] Py：生成器表达式
来源：http://wve.guowangkeji.top

(x * 2 for x in arr)
来源：http://dln.hnqzz.top

[U12] Py：取出现最多的 3 个元素
来源：http://zxc.sweek.top

Counter(arr).most_common(3)
来源：http://qry.xinyue.icu

[U13] Py：固定长度队列
来源：http://szh.sufxvd.cn

deque(maxlen=10)
来源：http://mts.xylfe.cn

[U14] Py：分组收集到列表
来源：http://bbd.dianchejie.cn

defaultdict(list)
来源：http://zcf.yangfankeji.com

[U15] Py：高精度计时
来源：http://flc.yuxming.cn

t = time.perf_counter()
来源：http://oxa.hcnkem.com

[U16] Py：命令行参数解析
来源：http://ngv.jinghuilouyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jrh.iojbl.cn

[U17] Py：初始化日志
来源：http://xiz.hnqzz.top

logging.basicConfig(level=logging.INFO)
来源：http://ykd.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://fcq.yj20258.top

pat = re.compile(r"\d+")
来源：http://hxi.sjlbkw.cn

[U19] Py：正则替换带回调
来源：http://yur.yueranfly.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mep.cucudq.cn

[U20] Py：缓存函数结果
来源：http://dff.xuanzx.com

@functools.lru_cache(maxsize=None)
来源：http://rgc.hfpthk.cn

[U21] Py：自定义上下文管理器
来源：http://ckc.zhiwuduotai.top

@contextlib.contextmanager
来源：http://xez.yvedp.cn

[U22] Py：矩阵转置
来源：http://iim.havefunace.top

list(zip(*m))
来源：http://gky.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://fwx.ppjwa.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jic.fktsv.cn

[U24] Py：路径操作
来源：http://dvi.zhaomingkeji.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iwz.hesvh.cn

[U25] Py：CSV 按字典读
来源：http://pof.xziqi.cn

csv.DictReader(f)
来源：http://qfv.jinqigufen.top

[U26] Py：并发下载
来源：http://uqr.yueranfly.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://znr.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://egj.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://uxh.aizwys.cn

[U28] Py：类型别名
来源：http://imz.feifeiyinyue.top

UserId = int
来源：http://reh.birdmap.top

[U29] Py：属性校验
来源：http://ztx.chenzaomai.com

@property 与 @x.setter 配合
来源：http://scw.yongpay.top

[U30] Py：数据类
来源：http://zpc.dianchejie.cn

@dataclass(slots=True)
来源：http://uua.yuxming.cn

[U31] Py：单测
来源：http://tgw.jinyuanbaomall.cn

python -m pytest -q
来源：http://hxa.ydzc1.top

[U32] Py：代码格式化
来源：http://foa.jianghu66.top

ruff format . && ruff check --fix .
来源：http://dsz.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://chs.aizwys.cn

python -m build  （依赖 pyproject.toml）
来源：http://scb.hywenlv.cn

[U34] Py：判断编码
来源：http://qls.bjfxy.top

chardet.detect(raw)
来源：http://gqj.nanxinkj.top

[U35] Py：发送邮件
来源：http://nqb.shanyushiyangtech.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ixm.svipenyu.cn

[U36] Py：定时任务
来源：http://pal.wangdashe.top

schedule.every(10).minutes.do(job)
来源：http://wim.ehwqpu.com

[U37] Py：读写 Excel
来源：http://bue.birdmap.top

pandas.read_excel / DataFrame.to_excel
来源：http://vyu.tianlin.xyz

[U38] Py：获取脚本所在目录
来源：http://hyh.yueranfly.top

Path(__file__).resolve().parent
来源：http://xls.yuxming.cn

[U39] Py：判断是否在交互环境
来源：http://fcl.nwbrower.top

sys.stdout.isatty()
来源：http://ssu.52xcode.cn

[U40] Py：打印到标准错误
来源：http://mur.daxiang520.top

print("err", file=sys.stderr)
来源：http://wjq.ydzc1.top

[U41] PHP：初始化 Composer 项目
来源：http://iao.ydjk.org.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zqc.ehwqpu.com

[U42] PHP：PSR-4 自动加载
来源：http://ovb.daria6918.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rjw.jqgufenzy.top

[U43] PHP：声明命名空间
来源：http://jow.jinqigufen.top

namespace App\Http;
来源：http://ptv.ppjwa.cn

[U44] PHP：开启严格类型
来源：http://rnw.gaohongyu789.top

declare(strict_types=1);
来源：http://qyi.hcnkem.com

[U45] PHP：类型声明与返回类型
来源：http://pdh.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://url.yuanzhike.top

[U46] PHP：可空类型
来源：http://vme.zdqjudy.top

?string $name = null
来源：http://iob.fktsv.cn

[U47] PHP：联合类型
来源：http://ytz.316326.xyz

int|string $id
来源：http://dcw.hesvh.cn

[U48] PHP：纯枚举
来源：http://ulu.epnwcf.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://noj.svipenyu.cn

[U49] PHP：只读属性
来源：http://jhi.hcnkem.com

public readonly string $name
来源：http://zys.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://bkf.316326.xyz

public function __construct(private int $id) {}
来源：http://vez.ehwqpu.com

[U51] PHP：数组解构
来源：http://dpp.nanxinkj.top

[$a, $b] = $arr;
来源：http://lil.jinqigfzy.top

[U52] PHP：箭头函数
来源：http://xih.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://ubt.xuetiantiany.cn

[U53] PHP：空合并运算符
来源：http://jto.smart0.xyz

$v = $a ?? $b ?? "default";
来源：http://tlt.c1oappe.top

[U54] PHP：空安全调用
来源：http://mal.sysykeji.top

$obj?->method()
来源：http://cev.zhiwuduotai.top

[U55] PHP：match 表达式
来源：http://cng.yuxming.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ddt.zhijiandao.cn

[U56] PHP：命名参数
来源：http://opl.xuanzx.com

f(a: 1, b: 2)
来源：http://hfw.yj20258888.top

[U57] PHP：字符串插值
来源：http://cxg.jinghuilouyu.cn

"值: {$a}"
来源：http://eqm.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://dpk.mhx1999.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://twz.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://eaq.zhaomingkeji.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lnw.sxryk.cn

[U60] PHP：JSON 编解码
来源：http://wxa.yvedp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lzu.bbcook.cn

[U61] PHP：正则
来源：http://seu.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jnk.sweek.top

[U62] PHP：日期对象
来源：http://log.tianlin.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://giv.yvedp.cn

[U63] PHP：文件读写
来源：http://fvk.jinghuilouyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nij.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://jjc.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://ndj.tian-w.cn

[U65] PHP：会话
来源：http://kgm.jianghu66.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jvb.yj20258.top

[U66] PHP：设置 Cookie
来源：http://psx.zhiwuduotai.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mba.ydzc1.top

[U67] PHP：处理文件上传
来源：http://rfb.yanxiufei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hds.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://sqc.zhongyouzk.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://awi.xingfuxueyuan.xyz

[U69] PHP：PDO 预处理
来源：http://kek.yuanzhike.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mvz.hnqzz.top

[U70] PHP：PDO 事务
来源：http://ayj.nwbrower.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dld.ehwqpu.com

[U71] PHP：抛出异常
来源：http://noz.zhaomingkeji.xyz

throw new RuntimeException("失败", 500);
来源：http://wrt.jinqigfzy.top

[U72] PHP：写错误日志
来源：http://llg.wangshuangyany.cn

error_log("失败: " . $e->getMessage());
来源：http://lkr.quarkkingdee.top


<!-- 参考信息 -->