代发 wailian999

[S45] C++：lambda
来源：http://ssq.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://gmh.feifeiyinyue.top

[S46] C++：函数模板
来源：http://odh.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ued.hysaishi.cn

[S47] C++：结构化绑定遍历
来源：http://jyh.zhixingplan.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hwl.yonumen.top

[S48] C++：逐行读文件
来源：http://buq.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dtw.dashuyun.cn

while (std::getline(in, line)) { }
来源：http://zpi.xinyue.icu

[S49] C++：写文件
来源：http://zjw.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kpo.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://dai.redwolf501.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rxd.yueranfly.top

[S51] C++：显式类型转换
来源：http://tgh.pycfn.com

static_cast<double>(a) / b
来源：http://egm.chenzaomai.com

[S52] C++：const 与 noexcept
来源：http://eze.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://dhb.aibaodan.cn

[S53] C++：移动语义
来源：http://zib.tian-w.cn

std::vector<int> w = std::move(v);
来源：http://ipq.gaohongyu789.top

[S54] C++：异常处理
来源：http://ljn.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mzy.jiagoushi.top

[S55] C++：结构化绑定
来源：http://mzc.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qkk.cqqwz.cn

[S56] C++：optional
来源：http://lhn.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fop.yuxming.cn

[S57] C++：编译期常量
来源：http://bdb.zdbjq.cn

constexpr int N = 10;
来源：http://uww.jqgfzy.top

[S58] C++：命名空间
来源：http://cav.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://qol.birdmap.top

[S59] C++：静态断言
来源：http://qqk.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lmp.ybcxt.top

[S60] C++：遍历并删除元素
来源：http://ukt.zhengqikj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fgv.fanxiaobao.xyz

================================================================================
来源：http://jbm.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cuh.nwbrower.top

================================================================================
来源：http://ohz.tarul.cn

[T01] Kotlin：Hello World
来源：http://mdu.shuidangran.top

println("Hello")
来源：http://imv.shuidangran.top

[T02] Kotlin：变量
来源：http://jak.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bpn.zhiwuduotai.top

[T03] Kotlin：字符串模板
来源：http://jpe.zhongyouzk.top

"值: $b"
来源：http://hjl.jyoumei.cn

[T04] Kotlin：空安全
来源：http://stv.epnwcf.com

val n: String? = null;  n?.length
来源：http://gse.zdbjq.cn

[T05] Kotlin：when 表达式
来源：http://sgr.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ylb.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://dwj.zhijiandao.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wrb.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://xlu.zhengqikj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fio.sweek.top

[T08] Kotlin：数据类
来源：http://suc.jinghuilouyu.cn

data class User(val name: String, val age: Int)
来源：http://zos.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://iyf.fehbvm.com

fun String.exclaim() = this + "!"
来源：http://uic.jinghuilouyu.cn

[T10] Kotlin：默认参数
来源：http://yfn.cheryme.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rlv.mhx1999.top

[T11] Kotlin：协程
来源：http://ibd.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://hcm.andypj.xyz

[T12] Kotlin：解构声明
来源：http://hdq.gzhubu.top

val (a, b) = Pair(1, 2)
来源：http://fwf.chenjidiqi.icu

[T13] Kotlin：只读 Map
来源：http://dgx.iojbl.cn

val m = mapOf("a" to 1)
来源：http://hym.yangfankeji.com

[T14] Kotlin：循环
来源：http://zvp.xinyue.icu

for (i in 1..10) println(i)
来源：http://ato.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://mff.yj20258888.top

interface Shape { fun area(): Double }
来源：http://nhs.aizwys.cn

[T16] Swift：Hello World
来源：http://dip.gaohongyu789.top

print("Hello")
来源：http://ppq.gogol.net.cn

[T17] Swift：变量与常量
来源：http://ugf.havefunace.top

var a = 1;  let b = 2
来源：http://off.mhx1999.top

[T18] Swift：字符串插值
来源：http://mks.sjlbkw.cn

"值: \(b)"
来源：http://gfd.tanke756.top

[T19] Swift：可选绑定
来源：http://vxd.ppjwa.cn

if let n = opt { print(n) }
来源：http://icr.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://nzg.ybcxt.top

var a = [1, 2, 3];  a.append(4)
来源：http://hwx.tanke756.top

[T21] Swift：遍历
来源：http://uzj.sufxvd.cn

for x in a { print(x) }
来源：http://sar.xylfe.cn

[T22] Swift：字典
来源：http://cil.yuanzhike.top

var d = ["a": 1];  d["b"] = 2
来源：http://vwh.jinqigfzy.top

[T23] Swift：函数
来源：http://zts.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bcq.hysaishi.cn

[T24] Swift：闭包
来源：http://nuo.jinghuilouyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rqv.wangdashe.top

[T25] Swift：结构体
来源：http://ltl.fehbvm.com

struct P { var x: Int }
来源：http://hqr.52xcode.cn

[T26] Swift：类与重写
来源：http://ewc.sysykeji.top

class A: Base { override func f() {} }
来源：http://afq.andypj.xyz

[T27] Swift：错误处理
来源：http://ggh.xylfe.cn

do { try f() } catch { print(error) }
来源：http://vrg.316326.xyz

[T28] Swift：枚举
来源：http://yqq.yongpay.top

enum Color { case red, green }
来源：http://oix.cashguo.top

[T29] Swift：guard 提前返回
来源：http://zpz.mhx1999.top

guard let x = opt else { return }
来源：http://dnf.nwbrower.top

[T30] Swift：协议
来源：http://flh.havefunace.top

protocol Shape { func area() -> Double }
来源：http://yvf.xingfuxueyuan.xyz

[T31] Lua：Hello World
来源：http://kno.aibaodan.cn

print("Hello")
来源：http://foj.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://eoz.aizwys.cn

local a = 1
来源：http://lvz.aizwys.cn

[T33] Lua：表（数组）
来源：http://joi.zdbjq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://icu.vqdsnc.cn

[T34] Lua：遍历表
来源：http://tdf.snrcjt.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vfp.xingfuxueyuan.xyz

[T35] Lua：字典表
来源：http://aqr.yuxming.cn

local d = { a = 1 };  d.b = 2
来源：http://qiz.fengsongda.top

[T36] Lua：函数
来源：http://vqk.fengsongda.top

function add(a, b) return a + b end
来源：http://zls.ydjk.org.cn

[T37] Lua：字符串拼接
来源：http://mva.zhixingplan.top

"a" .. "b"
来源：http://lol.yonumen.top

[T38] Lua：条件
来源：http://dzc.iojbl.cn

if x > 0 then print("正") end
来源：http://awa.zycfv.cn

[T39] Lua：模式匹配
来源：http://xco.hnqzz.top

string.find(s, "%d+")
来源：http://vrb.nanxinkj.top

[T40] Lua：元表
来源：http://ksc.jqgfzy.top

setmetatable({}, { __index = base })
来源：http://jmo.sweek.top

[T41] Perl：Hello World
来源：http://qdw.cdnleiting.top

print "Hello\n";
来源：http://alt.ydjk.org.cn

[T42] Perl：变量类型
来源：http://kli.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dcs.shangyingyoupin.top

[T43] Perl：字符串插值
来源：http://zkq.tarul.cn

"值: $a"
来源：http://ctm.dianchejie.cn

[T44] Perl：条件
来源：http://zce.52xcode.cn

if ($a > 0) { print "正"; }
来源：http://qxk.fktsv.cn

[T45] Perl：数组遍历
来源：http://enu.hammf.cn

for my $x (@arr) { print $x; }
来源：http://yld.fktsv.cn

[T46] Perl：哈希操作
来源：http://htv.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qof.tanke756.top

[T47] Perl：正则捕获
来源：http://nbg.haohaochexian.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bjt.ywan-chungtsiang.top

[T48] Perl：正则替换
来源：http://cwb.zdbjq.cn

$s =~ s/old/new/g;
来源：http://fex.cheryme.top

[T49] Perl：函数
来源：http://iyw.jianghu66.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wbq.xuetiantiany.cn

[T50] Perl：逐行读文件
来源：http://vln.feifeiyinyue.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hih.xylfe.cn

while (my $line = <$fh>) { print $line; }
来源：http://pms.bjfxy.top

[T51] Scala：Hello World
来源：http://emj.andypj.xyz

println("Hello")
来源：http://gsg.aibaodan.cn

[T52] Scala：变量
来源：http://vcf.jyoumei.cn

val a = 1;  var b = 2
来源：http://qju.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://omq.tianlin.xyz

s"值: $b"
来源：http://svh.wangdashe.top

[T54] Scala：集合映射
来源：http://ygk.xinyue.icu

List(1, 2, 3).map(_ * 2)
来源：http://vir.hesvh.cn

[T55] Scala：集合过滤
来源：http://dsf.yuanzhike.top

List(1, 2, 3).filter(_ > 1)
来源：http://szd.hnxiangtu.top

[T56] Scala：样例类
来源：http://jyu.xuetiantiany.cn

case class User(name: String, age: Int)
来源：http://inp.hongshengwenyu.top

[T57] Scala：模式匹配
来源：http://ycf.gogol.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ypq.jianghu66.top

[T58] Scala：函数定义
来源：http://dqn.yangfankeji.com

def add(a: Int, b: Int): Int = a + b
来源：http://bna.ydjk.org.cn

[T59] Scala：循环
来源：http://mnj.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://wvr.iojbl.cn

[T60] Scala：折叠
来源：http://yil.yangfankeji.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bzy.yj20258888.top

================================================================================
来源：http://otb.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://htt.daria6918.cn

================================================================================
来源：http://krs.havefunace.top

[U01] Py：创建虚拟环境
来源：http://yxt.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://gpx.jinqigufen.top

[U02] Py：导出 / 安装依赖
来源：http://azk.jinqigufen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ave.uphjek.com

[U03] Py：加载 .env 配置
来源：http://fuo.hfpthk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lbm.yj20258.top

[U04] Py：变量调试打印
来源：http://epv.c1oappe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://njy.hammf.cn

[U05] Py：列表去重且保序
来源：http://gic.zhongyouzk.top

list(dict.fromkeys(arr))
来源：http://tbq.zdqjudy.top

[U06] Py：合并两个字典
来源：http://tzv.mhx1999.top

{**a, **b}
来源：http://tpd.zhengqikj.top

[U07] Py：反转字典键值
来源：http://uag.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://zgd.meibo888.top

[U08] Py：展平二维列表
来源：http://zuu.guannengcc.top

[y for x in nested for y in x]
来源：http://oie.ppjwa.cn

[U09] Py：字典取最大值的键
来源：http://rgp.gogol.net.cn

max(d, key=d.get)
来源：http://cix.snrcjt.cn

[U10] Py：按值排序字典
来源：http://bgf.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://plm.hammf.cn

[U11] Py：生成器表达式
来源：http://hxd.shanyushiyangkeji.top

(x * 2 for x in arr)
来源：http://uvg.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yna.hywenlv.cn

Counter(arr).most_common(3)
来源：http://itk.nwbrower.top

[U13] Py：固定长度队列
来源：http://lhh.yj202588.top

deque(maxlen=10)
来源：http://duz.yangfankeji.com

[U14] Py：分组收集到列表
来源：http://uyq.iojbl.cn

defaultdict(list)
来源：http://wjh.hysaishi.cn

[U15] Py：高精度计时
来源：http://vwc.gogol.net.cn

t = time.perf_counter()
来源：http://iva.fengsongda.top

[U16] Py：命令行参数解析
来源：http://pam.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pqn.gogol.net.cn

[U17] Py：初始化日志
来源：http://gzh.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://fea.svipenyu.cn

[U18] Py：预编译正则
来源：http://wwx.chenjidiqi.icu

pat = re.compile(r"\d+")
来源：http://vno.fktsv.cn

[U19] Py：正则替换带回调
来源：http://aai.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ysa.shangyingyoupin.top

[U20] Py：缓存函数结果
来源：http://zll.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://smi.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://blb.sysykeji.top

@contextlib.contextmanager
来源：http://hlw.hammf.cn

[U22] Py：矩阵转置
来源：http://ayc.xuetiantiany.cn

list(zip(*m))
来源：http://pis.nanxinkj.top

[U23] Py：分块读取大文件
来源：http://hvo.ydzc1.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sya.redwolf501.top

[U24] Py：路径操作
来源：http://yfv.jqgfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://efh.xuanzx.com

[U25] Py：CSV 按字典读
来源：http://hth.sxryk.cn

csv.DictReader(f)
来源：http://bhx.0kj1m.cn

[U26] Py：并发下载
来源：http://rxd.jinqigufen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nlp.zhixingplan.top

[U27] Py：异步 HTTP
来源：http://njb.yanxiufei.cn

aiohttp.ClientSession() 配合 async with
来源：http://dke.uphjek.com

[U28] Py：类型别名
来源：http://ntv.andypj.xyz

UserId = int
来源：http://jlv.smart0.xyz

[U29] Py：属性校验
来源：http://xog.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://nuc.fehbvm.com

[U30] Py：数据类
来源：http://gvr.wangdashe.top

@dataclass(slots=True)
来源：http://dgm.ydzc1.top

[U31] Py：单测
来源：http://ojo.cashguo.top

python -m pytest -q
来源：http://mcn.tanke756.top

[U32] Py：代码格式化
来源：http://hja.sweek.top

ruff format . && ruff check --fix .
来源：http://vng.tian-w.cn

[U33] Py：打包发布
来源：http://dub.hywenlv.cn

python -m build  （依赖 pyproject.toml）
来源：http://swd.fehbvm.com

[U34] Py：判断编码
来源：http://qds.ivvv.top

chardet.detect(raw)
来源：http://dxa.uphjek.com

[U35] Py：发送邮件
来源：http://pdm.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zyo.yangfankeji.com

[U36] Py：定时任务
来源：http://zpc.uphjek.com

schedule.every(10).minutes.do(job)
来源：http://wcb.sjlbkw.cn

[U37] Py：读写 Excel
来源：http://ccm.svipenyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hei.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://uar.gotoacloud.top

Path(__file__).resolve().parent
来源：http://osr.shangyingyoupin.top

[U39] Py：判断是否在交互环境
来源：http://fmj.316326.xyz

sys.stdout.isatty()
来源：http://pct.bbcook.cn

[U40] Py：打印到标准错误
来源：http://oqe.yuanzhike.top

print("err", file=sys.stderr)
来源：http://akg.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://fhn.cheryme.top

composer init;  composer require guzzlehttp/guzzle
来源：http://tsb.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://cus.jinghuilouyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://neu.wangshuangyany.cn

[U43] PHP：声明命名空间
来源：http://vgv.tian-w.cn

namespace App\Http;
来源：http://erx.shanyushiyangkeji.top

[U44] PHP：开启严格类型
来源：http://pha.yangfankeji.com

declare(strict_types=1);
来源：http://qyp.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://gji.yuxming.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tqg.xinyue.icu

[U46] PHP：可空类型
来源：http://qrt.cashguo.top

?string $name = null
来源：http://ekh.ybcxt.top

[U47] PHP：联合类型
来源：http://xqb.jyoumei.cn

int|string $id
来源：http://emi.gotoacloud.top

[U48] PHP：纯枚举
来源：http://kan.zhixingplan.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tvi.hesvh.cn

[U49] PHP：只读属性
来源：http://cxz.zycfv.cn

public readonly string $name
来源：http://ozk.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://whx.svipenyu.cn

public function __construct(private int $id) {}
来源：http://abk.wangdashe.top

[U51] PHP：数组解构
来源：http://cbs.yvedp.cn

[$a, $b] = $arr;
来源：http://msh.jinyuanbaomall.cn

[U52] PHP：箭头函数
来源：http://fsc.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://yde.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://jjx.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://ajr.yuanzhike.top

[U54] PHP：空安全调用
来源：http://fjp.zhaomingkeji.xyz

$obj?->method()
来源：http://zzl.jinqigufen.top

[U55] PHP：match 表达式
来源：http://fxo.wangdashe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://png.yanxiufei.cn

[U56] PHP：命名参数
来源：http://qyx.svipenyu.cn

f(a: 1, b: 2)
来源：http://wbx.yvedp.cn

[U57] PHP：字符串插值
来源：http://nfr.9152youxi.cn

"值: {$a}"
来源：http://kcy.birdmap.top

[U58] PHP：数组三件套
来源：http://xog.dianchejie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mkh.ivvv.top

[U59] PHP：自定义排序
来源：http://pin.zhijiandao.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aud.hesvh.cn

[U60] PHP：JSON 编解码
来源：http://hsq.jianghu66.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bkl.jinyuanbaomall.cn

[U61] PHP：正则
来源：http://ccf.andypj.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hlz.dianchejie.cn

[U62] PHP：日期对象
来源：http://ldm.yangfankeji.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qdj.xuanzx.com

[U63] PHP：文件读写
来源：http://ovg.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iar.zycfv.cn

[U64] PHP：目录遍历
来源：http://hmo.vehdjk.com

glob("dir/*.php");  scandir("dir");
来源：http://isb.dashuyun.cn

[U65] PHP：会话
来源：http://qxn.jyoumei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wgy.zhoulong.xyz

[U66] PHP：设置 Cookie
来源：http://paz.chenjidiqi.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zei.quarkkingdee.top

[U67] PHP：处理文件上传
来源：http://zbq.daxiang520.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dch.cdnleiting.top

[U68] PHP：PDO 连接
来源：http://xcq.hnqzz.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lvp.chenzaomai.com

[U69] PHP：PDO 预处理
来源：http://iyw.yuxming.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gwi.yongpay.top

[U70] PHP：PDO 事务
来源：http://hvj.hnqzz.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zcs.ppjwa.cn


<!-- 参考信息 -->