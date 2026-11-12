代发 wailian999

while (std::getline(in, line)) { }
来源：http://gdq.xingfuxueyuan.xyz

[S49] C++：写文件
来源：http://shx.hcnkem.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blc.cashguo.top

[S50] C++：格式化数字
来源：http://blg.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gpc.xziqi.cn

[S51] C++：显式类型转换
来源：http://ksb.zdbjq.cn

static_cast<double>(a) / b
来源：http://sjw.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://foa.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://uje.dashuyun.cn

[S53] C++：移动语义
来源：http://kyr.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://cxl.fzhhl.top

[S54] C++：异常处理
来源：http://ufj.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://phh.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://kqs.yvedp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oeh.shangyingyoupin.top

[S56] C++：optional
来源：http://uor.uphjek.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iky.redwolf501.top

[S57] C++：编译期常量
来源：http://luo.yuanzhike.top

constexpr int N = 10;
来源：http://pgh.gaohongyu789.top

[S58] C++：命名空间
来源：http://jyi.shangyingyoupin.top

namespace ns { int f() { return 1; } }
来源：http://bou.c1oappe.top

[S59] C++：静态断言
来源：http://erk.vehdjk.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qhx.snrcjt.cn

[S60] C++：遍历并删除元素
来源：http://wrw.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rkh.zycfv.cn

================================================================================
来源：http://gkk.quarkkingdee.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tck.svipenyu.cn

================================================================================
来源：http://ptf.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://nlj.vehdjk.com

println("Hello")
来源：http://ndi.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://lzh.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dby.0kj1m.cn

[T03] Kotlin：字符串模板
来源：http://ikk.52xcode.cn

"值: $b"
来源：http://wzl.redwolf501.top

[T04] Kotlin：空安全
来源：http://ehb.sufxvd.cn

val n: String? = null;  n?.length
来源：http://vty.hammf.cn

[T05] Kotlin：when 表达式
来源：http://edr.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rfy.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://rwr.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eko.jinqigufen.top

[T07] Kotlin：集合过滤
来源：http://jac.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wwq.aibaodan.cn

[T08] Kotlin：数据类
来源：http://xrz.xinyue.icu

data class User(val name: String, val age: Int)
来源：http://jbq.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://wlf.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://egq.sysykeji.top

[T10] Kotlin：默认参数
来源：http://gkq.hywenlv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jvv.zhongyouzk.top

[T11] Kotlin：协程
来源：http://nrr.hfpthk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sjq.fehbvm.com

[T12] Kotlin：解构声明
来源：http://xst.yfazqb.com

val (a, b) = Pair(1, 2)
来源：http://kkw.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://ihc.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://pyt.daria6918.cn

[T14] Kotlin：循环
来源：http://dkm.redwolf501.top

for (i in 1..10) println(i)
来源：http://ebp.cheryme.top

[T15] Kotlin：接口
来源：http://kbi.jianghu66.top

interface Shape { fun area(): Double }
来源：http://sgi.daria6918.cn

[T16] Swift：Hello World
来源：http://mqe.fzhhl.top

print("Hello")
来源：http://gyj.ppjwa.cn

[T17] Swift：变量与常量
来源：http://bac.havefunace.top

var a = 1;  let b = 2
来源：http://ptd.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://lik.birdmap.top

"值: \(b)"
来源：http://mpr.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://tef.nwbrower.top

if let n = opt { print(n) }
来源：http://yga.zdbjq.cn

[T20] Swift：数组操作
来源：http://kye.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://job.jinqigufen.top

[T21] Swift：遍历
来源：http://mkr.guannengcc.top

for x in a { print(x) }
来源：http://wjb.hammf.cn

[T22] Swift：字典
来源：http://ica.ydjk.org.cn

var d = ["a": 1];  d["b"] = 2
来源：http://djt.smart0.xyz

[T23] Swift：函数
来源：http://brq.wangshuangyany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pyv.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://nsc.chenlongwang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://day.nwbrower.top

[T25] Swift：结构体
来源：http://kdz.sufxvd.cn

struct P { var x: Int }
来源：http://fbb.fengsongda.top

[T26] Swift：类与重写
来源：http://ksl.yfazqb.com

class A: Base { override func f() {} }
来源：http://abw.kuanghao11.cn

[T27] Swift：错误处理
来源：http://dta.9152youxi.cn

do { try f() } catch { print(error) }
来源：http://wza.wangdashe.top

[T28] Swift：枚举
来源：http://qix.gotoacloud.top

enum Color { case red, green }
来源：http://nsd.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://acs.mhx1999.top

guard let x = opt else { return }
来源：http://jbw.jlsjyb.cn

[T30] Swift：协议
来源：http://ejw.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://gbo.bbcook.cn

[T31] Lua：Hello World
来源：http://vto.mhx1999.top

print("Hello")
来源：http://lxl.ehwqpu.com

[T32] Lua：局部变量
来源：http://znt.nanxuanxn.top

local a = 1
来源：http://pnu.bbcook.cn

[T33] Lua：表（数组）
来源：http://idn.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://yqw.yongpay.top

[T34] Lua：遍历表
来源：http://ffd.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://giq.sufxvd.cn

[T35] Lua：字典表
来源：http://iug.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://mau.fzhhl.top

[T36] Lua：函数
来源：http://bta.fengsongda.top

function add(a, b) return a + b end
来源：http://gsc.cashguo.top

[T37] Lua：字符串拼接
来源：http://doe.yangfankeji.com

"a" .. "b"
来源：http://szh.chenlongwang.top

[T38] Lua：条件
来源：http://fom.sweek.top

if x > 0 then print("正") end
来源：http://dbv.nwbrower.top

[T39] Lua：模式匹配
来源：http://jdr.0kj1m.cn

string.find(s, "%d+")
来源：http://cka.nanxinkj.top

[T40] Lua：元表
来源：http://apz.birdmap.top

setmetatable({}, { __index = base })
来源：http://gtx.hysaishi.cn

[T41] Perl：Hello World
来源：http://wqy.xinyue.icu

print "Hello\n";
来源：http://kua.fanxiaobao.xyz

[T42] Perl：变量类型
来源：http://pnc.hongshengwenyu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fdh.fzhhl.top

[T43] Perl：字符串插值
来源：http://env.fanxiaobao.xyz

"值: $a"
来源：http://yyn.hysaishi.cn

[T44] Perl：条件
来源：http://wov.xylfe.cn

if ($a > 0) { print "正"; }
来源：http://nbh.chenlongwang.top

[T45] Perl：数组遍历
来源：http://pqf.wangdashe.top

for my $x (@arr) { print $x; }
来源：http://vpx.sjlbkw.cn

[T46] Perl：哈希操作
来源：http://vto.mhx1999.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zte.yj202588.top

[T47] Perl：正则捕获
来源：http://ggu.fengsongda.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qsf.gzhubu.top

[T48] Perl：正则替换
来源：http://ryr.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://tes.jianghu66.top

[T49] Perl：函数
来源：http://vti.yangfankeji.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fvx.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://mge.yuxming.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lak.gotoacloud.top

while (my $line = <$fh>) { print $line; }
来源：http://ckt.zhijiandao.cn

[T51] Scala：Hello World
来源：http://fqf.xingfuxueyuan.xyz

println("Hello")
来源：http://ezi.shuidangran.top

[T52] Scala：变量
来源：http://cgm.hysaishi.cn

val a = 1;  var b = 2
来源：http://pio.sysykeji.top

[T53] Scala：字符串插值
来源：http://xvh.fanxiaobao.xyz

s"值: $b"
来源：http://jny.hesvh.cn

[T54] Scala：集合映射
来源：http://soj.ehwqpu.com

List(1, 2, 3).map(_ * 2)
来源：http://fvn.iojbl.cn

[T55] Scala：集合过滤
来源：http://hrn.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sqa.iojbl.cn

[T56] Scala：样例类
来源：http://aez.sjlbkw.cn

case class User(name: String, age: Int)
来源：http://idf.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://kal.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gqc.xinyue.icu

[T58] Scala：函数定义
来源：http://pab.zhiwuduotai.top

def add(a: Int, b: Int): Int = a + b
来源：http://tih.fktsv.cn

[T59] Scala：循环
来源：http://axz.snrcjt.cn

for (i <- 1 to 10) println(i)
来源：http://tos.jlsjyb.cn

[T60] Scala：折叠
来源：http://ryz.pengpengdd.cyou

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dxg.fktsv.cn

================================================================================
来源：http://jxt.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mrt.zhixingplan.top

================================================================================
来源：http://vvs.cqqwz.cn

[U01] Py：创建虚拟环境
来源：http://yfc.9152youxi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://trn.dashuyun.cn

[U02] Py：导出 / 安装依赖
来源：http://guy.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://imn.chenzaomai.com

[U03] Py：加载 .env 配置
来源：http://jjy.dianchejie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://psp.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://xhf.haohaochexian.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ast.birdmap.top

[U05] Py：列表去重且保序
来源：http://gaa.hcnkem.com

list(dict.fromkeys(arr))
来源：http://psq.cheryme.top

[U06] Py：合并两个字典
来源：http://jox.c1oappe.top

{**a, **b}
来源：http://xhl.zhiwuduotai.top

[U07] Py：反转字典键值
来源：http://vsc.mhx1999.top

{v: k for k, v in d.items()}
来源：http://jme.pycfn.com

[U08] Py：展平二维列表
来源：http://hhv.hywenlv.cn

[y for x in nested for y in x]
来源：http://wfu.aibaodan.cn

[U09] Py：字典取最大值的键
来源：http://gib.52xcode.cn

max(d, key=d.get)
来源：http://ycq.zhoulong.xyz

[U10] Py：按值排序字典
来源：http://ssx.zhaomingkeji.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pzi.chenlongwang.top

[U11] Py：生成器表达式
来源：http://mpx.epnwcf.com

(x * 2 for x in arr)
来源：http://fdx.shanyushiyangtech.top

[U12] Py：取出现最多的 3 个元素
来源：http://uff.iojbl.cn

Counter(arr).most_common(3)
来源：http://adw.zdbjq.cn

[U13] Py：固定长度队列
来源：http://bzx.shuidangran.top

deque(maxlen=10)
来源：http://xjm.andypj.xyz

[U14] Py：分组收集到列表
来源：http://lpq.sufxvd.cn

defaultdict(list)
来源：http://dhn.sweek.top

[U15] Py：高精度计时
来源：http://hsl.hywenlv.cn

t = time.perf_counter()
来源：http://sva.aizwys.cn

[U16] Py：命令行参数解析
来源：http://hej.aibaodan.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wtq.jinqigfzy.top

[U17] Py：初始化日志
来源：http://obu.sysykeji.top

logging.basicConfig(level=logging.INFO)
来源：http://fix.xylfe.cn

[U18] Py：预编译正则
来源：http://fwf.xingfuxueyuan.xyz

pat = re.compile(r"\d+")
来源：http://gzq.smart0.xyz

[U19] Py：正则替换带回调
来源：http://uqe.dashuyun.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cxy.vqdsnc.cn

[U20] Py：缓存函数结果
来源：http://mna.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://ttg.zhixingplan.top

[U21] Py：自定义上下文管理器
来源：http://xeu.vehdjk.com

@contextlib.contextmanager
来源：http://yma.jinqigfzy.top

[U22] Py：矩阵转置
来源：http://ysp.jyoumei.cn

list(zip(*m))
来源：http://mfg.guowangkeji.top

[U23] Py：分块读取大文件
来源：http://ely.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wmj.cdnleiting.top

[U24] Py：路径操作
来源：http://yyx.zhiwuduotai.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gpn.tanke756.top

[U25] Py：CSV 按字典读
来源：http://tbe.shangyingyoupin.top

csv.DictReader(f)
来源：http://cqt.hnqzz.top

[U26] Py：并发下载
来源：http://qwo.cheryme.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gvn.yvedp.cn

[U27] Py：异步 HTTP
来源：http://crq.zhengqikj.top

aiohttp.ClientSession() 配合 async with
来源：http://daj.chenjidiqi.icu

[U28] Py：类型别名
来源：http://xar.yonumen.top

UserId = int
来源：http://yws.svipenyu.cn

[U29] Py：属性校验
来源：http://ctx.fzhhl.top

@property 与 @x.setter 配合
来源：http://teu.hesvh.cn

[U30] Py：数据类
来源：http://tlk.dianchejie.cn

@dataclass(slots=True)
来源：http://qne.birdmap.top

[U31] Py：单测
来源：http://mbr.quarkkingdee.top

python -m pytest -q
来源：http://aas.hysaishi.cn

[U32] Py：代码格式化
来源：http://hxf.bbcook.cn

ruff format . && ruff check --fix .
来源：http://tzn.mhx1999.top

[U33] Py：打包发布
来源：http://xaw.gaohongyu789.top

python -m build  （依赖 pyproject.toml）
来源：http://nzi.chenzaomai.com

[U34] Py：判断编码
来源：http://gqd.haohaochexian.top

chardet.detect(raw)
来源：http://jbl.ppjwa.cn

[U35] Py：发送邮件
来源：http://iju.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rjy.dashuyun.cn

[U36] Py：定时任务
来源：http://mna.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://wxe.c1oappe.top

[U37] Py：读写 Excel
来源：http://ooi.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://vbn.yonumen.top

[U38] Py：获取脚本所在目录
来源：http://otd.xylfe.cn

Path(__file__).resolve().parent
来源：http://czx.shuidangran.top

[U39] Py：判断是否在交互环境
来源：http://phs.sxryk.cn

sys.stdout.isatty()
来源：http://nds.jinghuilouyu.cn

[U40] Py：打印到标准错误
来源：http://lvd.cqqwz.cn

print("err", file=sys.stderr)
来源：http://ixd.yj202588.top

[U41] PHP：初始化 Composer 项目
来源：http://rqh.tian-w.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mwt.gogol.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://wso.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xbr.daxiang520.top

[U43] PHP：声明命名空间
来源：http://xjz.mhx1999.top

namespace App\Http;
来源：http://tbo.smart0.xyz

[U44] PHP：开启严格类型
来源：http://ryv.zhixingplan.top

declare(strict_types=1);
来源：http://lzi.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://yvx.birdmap.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fuh.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://xuf.aibaodan.cn

?string $name = null
来源：http://ynx.jqgufenzy.top

[U47] PHP：联合类型
来源：http://vun.chenjidiqi.icu

int|string $id
来源：http://owc.zdqjudy.top

[U48] PHP：纯枚举
来源：http://fez.birdmap.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tyl.yuxming.cn

[U49] PHP：只读属性
来源：http://gkb.xuanzx.com

public readonly string $name
来源：http://nte.gzhubu.top

[U50] PHP：构造器属性提升
来源：http://mzq.chenlongwang.top

public function __construct(private int $id) {}
来源：http://hjt.yfazqb.com

[U51] PHP：数组解构
来源：http://rsj.wangdashe.top

[$a, $b] = $arr;
来源：http://owt.nwbrower.top

[U52] PHP：箭头函数
来源：http://pjw.hywenlv.cn

$double = fn($x) => $x * 2;
来源：http://rqt.yj202588.top

[U53] PHP：空合并运算符
来源：http://swi.fehbvm.com

$v = $a ?? $b ?? "default";
来源：http://hdn.sweek.top

[U54] PHP：空安全调用
来源：http://abc.nanxuanxn.top

$obj?->method()
来源：http://veo.iojbl.cn

[U55] PHP：match 表达式
来源：http://eqm.jiagoushi.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bfr.yangfankeji.com

[U56] PHP：命名参数
来源：http://rkp.chenlongwang.top

f(a: 1, b: 2)
来源：http://rso.daxiang520.top

[U57] PHP：字符串插值
来源：http://ncr.tanke756.top

"值: {$a}"
来源：http://nvj.guowangkeji.top

[U58] PHP：数组三件套
来源：http://xwh.dashuyun.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zxg.ybcxt.top

[U59] PHP：自定义排序
来源：http://mcq.dashuyun.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://knh.fktsv.cn

[U60] PHP：JSON 编解码
来源：http://qqh.cashguo.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pgw.jinyuanbaomall.cn

[U61] PHP：正则
来源：http://utl.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cnd.zhijiandao.cn

[U62] PHP：日期对象
来源：http://gqt.hfpthk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jwg.yfazqb.com

[U63] PHP：文件读写
来源：http://xxo.hfpthk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iwh.nanxinkj.top

[U64] PHP：目录遍历
来源：http://yay.zhixingplan.top

glob("dir/*.php");  scandir("dir");
来源：http://vbb.nwbrower.top

[U65] PHP：会话
来源：http://gps.316326.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://osw.ywan-chungtsiang.top

[U66] PHP：设置 Cookie
来源：http://yle.yangfankeji.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vqf.zhijiandao.cn

[U67] PHP：处理文件上传
来源：http://wja.gaohongyu789.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uwp.yonumen.top

[U68] PHP：PDO 连接
来源：http://iqz.ydjk.org.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://egd.xylfe.cn

[U69] PHP：PDO 预处理
来源：http://uoe.yj20258.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wia.yueranfly.top

[U70] PHP：PDO 事务
来源：http://bzu.fengsongda.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nia.fehbvm.com

[U71] PHP：抛出异常
来源：http://dqo.haohaochexian.top

throw new RuntimeException("失败", 500);
来源：http://phy.chenlongwang.top

[U72] PHP：写错误日志
来源：http://idr.jianghu66.top

error_log("失败: " . $e->getMessage());
来源：http://qzc.quarkkingdee.top

[U73] PHP：读取 ini 配置
来源：http://gbi.meibo888.top

parse_ini_file("config.ini", true)
来源：http://tql.vehdjk.com

[U74] PHP：读取环境变量
来源：http://wnn.ehwqpu.com

getenv("APP_ENV") ?: "production"
来源：http://ffu.yuanzhike.top


<!-- 参考信息 -->