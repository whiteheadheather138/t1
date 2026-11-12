代发 wailian999

[S45] C++：lambda
来源：http://jhd.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://fno.ivvv.top

[S46] C++：函数模板
来源：http://ict.yj20258.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://trs.jinqigfzy.top

[S47] C++：结构化绑定遍历
来源：http://own.fengsongda.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hlx.mhx1999.top

[S48] C++：逐行读文件
来源：http://tmo.fanxiaobao.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://ozl.mhx1999.top

while (std::getline(in, line)) { }
来源：http://zum.jyoumei.cn

[S49] C++：写文件
来源：http://icz.yuxming.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bbx.ivvv.top

[S50] C++：格式化数字
来源：http://ilh.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oav.cucudq.cn

[S51] C++：显式类型转换
来源：http://kle.ydjk.org.cn

static_cast<double>(a) / b
来源：http://qvz.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://tlx.hnqzz.top

int size() const noexcept { return n_; }
来源：http://enf.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://jjf.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://hgv.gogol.net.cn

[S54] C++：异常处理
来源：http://bwa.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gjx.jianghu66.top

[S55] C++：结构化绑定
来源：http://fri.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jrx.ywan-chungtsiang.top

[S56] C++：optional
来源：http://pwc.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wwo.yvedp.cn

[S57] C++：编译期常量
来源：http://fic.yfazqb.com

constexpr int N = 10;
来源：http://kru.316326.xyz

[S58] C++：命名空间
来源：http://wqa.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://jcv.nanxinkj.top

[S59] C++：静态断言
来源：http://lqm.xziqi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xfp.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://gds.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lmp.wangshuangyany.cn

================================================================================
来源：http://sce.jinqigufen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://srv.yangfankeji.com

================================================================================
来源：http://nvs.feifeiyinyue.top

[T01] Kotlin：Hello World
来源：http://cnf.tianlin.xyz

println("Hello")
来源：http://gxn.cdnleiting.top

[T02] Kotlin：变量
来源：http://rhb.ydjk.org.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yre.yj20258.top

[T03] Kotlin：字符串模板
来源：http://ryx.0kj1m.cn

"值: $b"
来源：http://ala.wangshuangyany.cn

[T04] Kotlin：空安全
来源：http://kvj.ctjpmb.com

val n: String? = null;  n?.length
来源：http://hbc.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://kti.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mgl.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://bnb.sxryk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gqq.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://gea.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qdr.zdbjq.cn

[T08] Kotlin：数据类
来源：http://lpf.birdmap.top

data class User(val name: String, val age: Int)
来源：http://qan.fktsv.cn

[T09] Kotlin：扩展函数
来源：http://wpr.kuanghao11.cn

fun String.exclaim() = this + "!"
来源：http://omc.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://stp.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mur.dashuyun.cn

[T11] Kotlin：协程
来源：http://auk.feifeiyinyue.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gii.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://hec.zhongyouzk.top

val (a, b) = Pair(1, 2)
来源：http://jiw.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://eln.xylfe.cn

val m = mapOf("a" to 1)
来源：http://zor.vehdjk.com

[T14] Kotlin：循环
来源：http://hkc.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://egy.bjfxy.top

[T15] Kotlin：接口
来源：http://wyh.wangdashe.top

interface Shape { fun area(): Double }
来源：http://hfs.316326.xyz

[T16] Swift：Hello World
来源：http://kux.bbcook.cn

print("Hello")
来源：http://cdv.epnwcf.com

[T17] Swift：变量与常量
来源：http://mth.aibaodan.cn

var a = 1;  let b = 2
来源：http://jmu.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://gbs.ctjpmb.com

"值: \(b)"
来源：http://tln.yuanzhike.top

[T19] Swift：可选绑定
来源：http://dar.hesvh.cn

if let n = opt { print(n) }
来源：http://arh.yj20258.top

[T20] Swift：数组操作
来源：http://hbv.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://jar.shanyushiyangkeji.top

[T21] Swift：遍历
来源：http://lij.bjfxy.top

for x in a { print(x) }
来源：http://mim.sweek.top

[T22] Swift：字典
来源：http://idd.c1oappe.top

var d = ["a": 1];  d["b"] = 2
来源：http://new.wangshuangyany.cn

[T23] Swift：函数
来源：http://lfu.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sxf.0kj1m.cn

[T24] Swift：闭包
来源：http://znu.ybcxt.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ops.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://juf.yuxming.cn

struct P { var x: Int }
来源：http://mhx.zhengqikj.top

[T26] Swift：类与重写
来源：http://hps.nanxinkj.top

class A: Base { override func f() {} }
来源：http://knd.smart0.xyz

[T27] Swift：错误处理
来源：http://wab.xylfe.cn

do { try f() } catch { print(error) }
来源：http://ubw.c1oappe.top

[T28] Swift：枚举
来源：http://akg.gaohongyu789.top

enum Color { case red, green }
来源：http://ptl.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://qqc.bbcook.cn

guard let x = opt else { return }
来源：http://dvl.sxryk.cn

[T30] Swift：协议
来源：http://oyr.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://ikx.yongpay.top

[T31] Lua：Hello World
来源：http://and.hnqzz.top

print("Hello")
来源：http://tih.vqdsnc.cn

[T32] Lua：局部变量
来源：http://lil.yvedp.cn

local a = 1
来源：http://tbg.hnxiangtu.top

[T33] Lua：表（数组）
来源：http://tdx.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wqw.gzhubu.top

[T34] Lua：遍历表
来源：http://dqy.yanxiufei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zcu.guowangkeji.top

[T35] Lua：字典表
来源：http://jco.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://rmf.guowangkeji.top

[T36] Lua：函数
来源：http://lab.hfpthk.cn

function add(a, b) return a + b end
来源：http://enb.yj202588.top

[T37] Lua：字符串拼接
来源：http://cdz.cqqwz.cn

"a" .. "b"
来源：http://vuf.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://mbi.yueranfly.top

if x > 0 then print("正") end
来源：http://qgm.zhaomingkeji.xyz

[T39] Lua：模式匹配
来源：http://ccb.xuetiantiany.cn

string.find(s, "%d+")
来源：http://fkv.wangdashe.top

[T40] Lua：元表
来源：http://ogw.cashguo.top

setmetatable({}, { __index = base })
来源：http://ole.ydzc1.top

[T41] Perl：Hello World
来源：http://gkq.fzhhl.top

print "Hello\n";
来源：http://mcd.cdnleiting.top

[T42] Perl：变量类型
来源：http://oyp.epnwcf.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ers.nwbrower.top

[T43] Perl：字符串插值
来源：http://yxk.shuidangran.top

"值: $a"
来源：http://osw.xingfuxueyuan.xyz

[T44] Perl：条件
来源：http://iqs.tanke756.top

if ($a > 0) { print "正"; }
来源：http://tim.zhixingplan.top

[T45] Perl：数组遍历
来源：http://xls.sysykeji.top

for my $x (@arr) { print $x; }
来源：http://eue.uphjek.com

[T46] Perl：哈希操作
来源：http://jjw.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ghc.xuanzx.com

[T47] Perl：正则捕获
来源：http://nhe.hysaishi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sus.tarul.cn

[T48] Perl：正则替换
来源：http://vzm.cucudq.cn

$s =~ s/old/new/g;
来源：http://fqa.xuetiantiany.cn

[T49] Perl：函数
来源：http://avs.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aqc.ehwqpu.com

[T50] Perl：逐行读文件
来源：http://hfa.zhoulong.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://nuj.ydzc1.top

while (my $line = <$fh>) { print $line; }
来源：http://tnc.nanxinkj.top

[T51] Scala：Hello World
来源：http://lfm.havefunace.top

println("Hello")
来源：http://xkr.pycfn.com

[T52] Scala：变量
来源：http://wjo.andypj.xyz

val a = 1;  var b = 2
来源：http://fyg.fktsv.cn

[T53] Scala：字符串插值
来源：http://ini.jqgfzy.top

s"值: $b"
来源：http://hti.hnxiangtu.top

[T54] Scala：集合映射
来源：http://kty.nanxuanxn.top

List(1, 2, 3).map(_ * 2)
来源：http://pge.guowangkeji.top

[T55] Scala：集合过滤
来源：http://lub.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://wak.wangdashe.top

[T56] Scala：样例类
来源：http://dgp.redwolf501.top

case class User(name: String, age: Int)
来源：http://rkm.fehbvm.com

[T57] Scala：模式匹配
来源：http://ioj.yonumen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://elk.meibo888.top

[T58] Scala：函数定义
来源：http://iup.gaohongyu789.top

def add(a: Int, b: Int): Int = a + b
来源：http://ahy.fanxiaobao.xyz

[T59] Scala：循环
来源：http://phh.nanxuanxn.top

for (i <- 1 to 10) println(i)
来源：http://zal.smart0.xyz

[T60] Scala：折叠
来源：http://opx.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lkg.chenjidiqi.icu

================================================================================
来源：http://bvo.shuidangran.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lvw.9152youxi.cn

================================================================================
来源：http://nmt.c1oappe.top

[U01] Py：创建虚拟环境
来源：http://ccr.fzhhl.top

python -m venv .venv && source .venv/bin/activate
来源：http://tbo.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://zeo.sxryk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kpk.fehbvm.com

[U03] Py：加载 .env 配置
来源：http://snu.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yyk.uphjek.com

[U04] Py：变量调试打印
来源：http://buq.bjfxy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yyw.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://rqx.tian-w.cn

list(dict.fromkeys(arr))
来源：http://jxp.hysaishi.cn

[U06] Py：合并两个字典
来源：http://syd.chenjidiqi.icu

{**a, **b}
来源：http://gzu.hnxiangtu.top

[U07] Py：反转字典键值
来源：http://wev.nwbrower.top

{v: k for k, v in d.items()}
来源：http://vto.havefunace.top

[U08] Py：展平二维列表
来源：http://vya.epnwcf.com

[y for x in nested for y in x]
来源：http://ypb.fehbvm.com

[U09] Py：字典取最大值的键
来源：http://ufs.dashuyun.cn

max(d, key=d.get)
来源：http://jlx.bbcook.cn

[U10] Py：按值排序字典
来源：http://ufc.sjlbkw.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ftt.cheryme.top

[U11] Py：生成器表达式
来源：http://tct.hcnkem.com

(x * 2 for x in arr)
来源：http://roh.kuanghao11.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pcu.xylfe.cn

Counter(arr).most_common(3)
来源：http://bgz.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://sjc.wangshuangyany.cn

deque(maxlen=10)
来源：http://jcy.xinyue.icu

[U14] Py：分组收集到列表
来源：http://cgk.dianchejie.cn

defaultdict(list)
来源：http://eby.cheryme.top

[U15] Py：高精度计时
来源：http://tub.yvedp.cn

t = time.perf_counter()
来源：http://nhq.jinqigfzy.top

[U16] Py：命令行参数解析
来源：http://nzz.c1oappe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yca.sjlbkw.cn

[U17] Py：初始化日志
来源：http://yfq.fehbvm.com

logging.basicConfig(level=logging.INFO)
来源：http://bto.zdqjudy.top

[U18] Py：预编译正则
来源：http://ibv.xylfe.cn

pat = re.compile(r"\d+")
来源：http://sdb.jinqigufen.top

[U19] Py：正则替换带回调
来源：http://zcj.jianghu66.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bhw.zhaomingkeji.xyz

[U20] Py：缓存函数结果
来源：http://mzt.haohaochexian.top

@functools.lru_cache(maxsize=None)
来源：http://kmb.xylfe.cn

[U21] Py：自定义上下文管理器
来源：http://dxm.hcnkem.com

@contextlib.contextmanager
来源：http://qoe.jianghu66.top

[U22] Py：矩阵转置
来源：http://zue.smart0.xyz

list(zip(*m))
来源：http://rmw.ydzc1.top

[U23] Py：分块读取大文件
来源：http://fsl.fktsv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bts.yanxiufei.cn

[U24] Py：路径操作
来源：http://kfj.yuxming.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gcz.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://olh.sufxvd.cn

csv.DictReader(f)
来源：http://vjk.cheryme.top

[U26] Py：并发下载
来源：http://kyu.ydzc1.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://btp.xylfe.cn

[U27] Py：异步 HTTP
来源：http://dpg.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://dpb.xziqi.cn

[U28] Py：类型别名
来源：http://lxx.xylfe.cn

UserId = int
来源：http://hsb.jinqigufen.top

[U29] Py：属性校验
来源：http://kmi.fzhhl.top

@property 与 @x.setter 配合
来源：http://bsu.cashguo.top

[U30] Py：数据类
来源：http://xut.yuanzhike.top

@dataclass(slots=True)
来源：http://srt.xingfuxueyuan.xyz

[U31] Py：单测
来源：http://yfr.hysaishi.cn

python -m pytest -q
来源：http://uze.zdqjudy.top

[U32] Py：代码格式化
来源：http://zne.shuidangran.top

ruff format . && ruff check --fix .
来源：http://umy.zhongyouzk.top

[U33] Py：打包发布
来源：http://zjz.snrcjt.cn

python -m build  （依赖 pyproject.toml）
来源：http://efr.cucudq.cn

[U34] Py：判断编码
来源：http://yrm.xuetiantiany.cn

chardet.detect(raw)
来源：http://bsd.c1oappe.top

[U35] Py：发送邮件
来源：http://epu.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gyl.chenzaomai.com

[U36] Py：定时任务
来源：http://jfg.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://kxs.chenlongwang.top

[U37] Py：读写 Excel
来源：http://ofu.sxryk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wks.hysaishi.cn

[U38] Py：获取脚本所在目录
来源：http://laa.wangdashe.top

Path(__file__).resolve().parent
来源：http://oza.nanxuanxn.top

[U39] Py：判断是否在交互环境
来源：http://ztt.fanxiaobao.xyz

sys.stdout.isatty()
来源：http://bzi.dashuyun.cn

[U40] Py：打印到标准错误
来源：http://esx.sysykeji.top

print("err", file=sys.stderr)
来源：http://gpf.gotoacloud.top

[U41] PHP：初始化 Composer 项目
来源：http://ryw.wangshuangyany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://unn.gogol.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://xdq.aizwys.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://plj.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://jzp.kuanghao11.cn

namespace App\Http;
来源：http://tyd.nwbrower.top

[U44] PHP：开启严格类型
来源：http://sma.hnxiangtu.top

declare(strict_types=1);
来源：http://nym.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://wui.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://syn.daria6918.cn

[U46] PHP：可空类型
来源：http://pkk.shanyushiyangkeji.top

?string $name = null
来源：http://aqh.jinqigufen.top

[U47] PHP：联合类型
来源：http://git.fengsongda.top

int|string $id
来源：http://atz.jqgfzy.top

[U48] PHP：纯枚举
来源：http://kiw.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gtr.tanke756.top

[U49] PHP：只读属性
来源：http://oui.sweek.top

public readonly string $name
来源：http://wtc.pycfn.com

[U50] PHP：构造器属性提升
来源：http://oao.smart0.xyz

public function __construct(private int $id) {}
来源：http://gti.snrcjt.cn

[U51] PHP：数组解构
来源：http://odj.hnxiangtu.top

[$a, $b] = $arr;
来源：http://wer.gaohongyu789.top

[U52] PHP：箭头函数
来源：http://bnr.yueranfly.top

$double = fn($x) => $x * 2;
来源：http://adf.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://cfr.wangdashe.top

$v = $a ?? $b ?? "default";
来源：http://lsb.zhengqikj.top

[U54] PHP：空安全调用
来源：http://qyg.sjlbkw.cn

$obj?->method()
来源：http://muw.shanyushiyangkeji.top

[U55] PHP：match 表达式
来源：http://hpv.fktsv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jrq.9152youxi.cn

[U56] PHP：命名参数
来源：http://vbz.yueranfly.top

f(a: 1, b: 2)
来源：http://mje.zhengqikj.top

[U57] PHP：字符串插值
来源：http://obk.tanke756.top

"值: {$a}"
来源：http://kuo.shuidangran.top

[U58] PHP：数组三件套
来源：http://axm.andypj.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wak.havefunace.top

[U59] PHP：自定义排序
来源：http://fzy.pycfn.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oql.yj20258.top

[U60] PHP：JSON 编解码
来源：http://frq.jiagoushi.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rub.havefunace.top

[U61] PHP：正则
来源：http://wyh.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vum.svipenyu.cn

[U62] PHP：日期对象
来源：http://zks.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ozs.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://iih.uphjek.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://utw.gzhubu.top

[U64] PHP：目录遍历
来源：http://suh.jinyuanbaomall.cn

glob("dir/*.php");  scandir("dir");
来源：http://cpe.hfpthk.cn

[U65] PHP：会话
来源：http://hek.haohaochexian.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jvh.guowangkeji.top

[U66] PHP：设置 Cookie
来源：http://rqr.nwbrower.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vlf.yangfankeji.com

[U67] PHP：处理文件上传
来源：http://hoe.meibo888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yab.smart0.xyz

[U68] PHP：PDO 连接
来源：http://buz.fktsv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oiv.yj202588.top

[U69] PHP：PDO 预处理
来源：http://mma.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cxg.zhaomingkeji.xyz

[U70] PHP：PDO 事务
来源：http://tcr.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bgg.xziqi.cn


<!-- 参考信息 -->