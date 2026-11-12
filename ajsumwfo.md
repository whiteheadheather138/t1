代发 wailian999

while (std::getline(in, line)) { }
来源：http://jyp.mhx1999.top

[S49] C++：写文件
来源：http://bfs.ctjpmb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lyk.zhengqikj.top

[S50] C++：格式化数字
来源：http://qqg.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://luk.nwbrower.top

[S51] C++：显式类型转换
来源：http://rlr.uphjek.com

static_cast<double>(a) / b
来源：http://cqw.hesvh.cn

[S52] C++：const 与 noexcept
来源：http://mka.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://ice.shanyushiyangkeji.top

[S53] C++：移动语义
来源：http://fre.fanxiaobao.xyz

std::vector<int> w = std::move(v);
来源：http://qgh.fanxiaobao.xyz

[S54] C++：异常处理
来源：http://pbs.sxryk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nls.gogol.net.cn

[S55] C++：结构化绑定
来源：http://oya.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qom.birdmap.top

[S56] C++：optional
来源：http://lhb.dashuyun.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hcs.gaohongyu789.top

[S57] C++：编译期常量
来源：http://nem.chenzaomai.com

constexpr int N = 10;
来源：http://xop.dianchejie.cn

[S58] C++：命名空间
来源：http://ukg.andypj.xyz

namespace ns { int f() { return 1; } }
来源：http://ujk.yj20258888.top

[S59] C++：静态断言
来源：http://jsc.quarkkingdee.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jrj.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://dwt.hnqzz.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://npa.jinghuilouyu.cn

================================================================================
来源：http://hmr.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jxc.guowangkeji.top

================================================================================
来源：http://vmk.feifeiyinyue.top

[T01] Kotlin：Hello World
来源：http://isg.aizwys.cn

println("Hello")
来源：http://jze.jlsjyb.cn

[T02] Kotlin：变量
来源：http://spp.fengsongda.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://alc.ivvv.top

[T03] Kotlin：字符串模板
来源：http://ysf.fengsongda.top

"值: $b"
来源：http://vkf.xuanzx.com

[T04] Kotlin：空安全
来源：http://flo.guowangkeji.top

val n: String? = null;  n?.length
来源：http://pdq.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://wzk.ydjk.org.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vzf.jqgufenzy.top

[T06] Kotlin：集合映射
来源：http://vkm.quarkkingdee.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rot.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://fim.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://tfp.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://vds.gaohongyu789.top

data class User(val name: String, val age: Int)
来源：http://ohj.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://gbu.yangfankeji.com

fun String.exclaim() = this + "!"
来源：http://fcy.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://txz.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://viz.daxiang520.top

[T11] Kotlin：协程
来源：http://hkp.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://agk.kuanghao11.cn

[T12] Kotlin：解构声明
来源：http://lci.yanxiufei.cn

val (a, b) = Pair(1, 2)
来源：http://gbi.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://cxy.yanxiufei.cn

val m = mapOf("a" to 1)
来源：http://qnf.zhengqikj.top

[T14] Kotlin：循环
来源：http://xdr.ywan-chungtsiang.top

for (i in 1..10) println(i)
来源：http://wnc.hnxiangtu.top

[T15] Kotlin：接口
来源：http://sdo.yueranfly.top

interface Shape { fun area(): Double }
来源：http://nws.cucudq.cn

[T16] Swift：Hello World
来源：http://ged.cqqwz.cn

print("Hello")
来源：http://uzf.c1oappe.top

[T17] Swift：变量与常量
来源：http://mjs.yj20258.top

var a = 1;  let b = 2
来源：http://arv.cqqwz.cn

[T18] Swift：字符串插值
来源：http://cfj.jqgufenzy.top

"值: \(b)"
来源：http://udv.yuanzhike.top

[T19] Swift：可选绑定
来源：http://vju.0kj1m.cn

if let n = opt { print(n) }
来源：http://cqz.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://nxk.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hcd.jlsjyb.cn

[T21] Swift：遍历
来源：http://gqk.jqgfzy.top

for x in a { print(x) }
来源：http://rgk.hnqzz.top

[T22] Swift：字典
来源：http://tmy.sweek.top

var d = ["a": 1];  d["b"] = 2
来源：http://lco.yfazqb.com

[T23] Swift：函数
来源：http://uxp.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://laa.gaohongyu789.top

[T24] Swift：闭包
来源：http://ltl.daria6918.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wtz.cdnleiting.top

[T25] Swift：结构体
来源：http://wxn.nanxinkj.top

struct P { var x: Int }
来源：http://veu.yanxiufei.cn

[T26] Swift：类与重写
来源：http://yau.jianghu66.top

class A: Base { override func f() {} }
来源：http://mwy.sjlbkw.cn

[T27] Swift：错误处理
来源：http://cfe.nanxinkj.top

do { try f() } catch { print(error) }
来源：http://ilx.xylfe.cn

[T28] Swift：枚举
来源：http://faz.jianghu66.top

enum Color { case red, green }
来源：http://yij.jinqigufen.top

[T29] Swift：guard 提前返回
来源：http://urx.jinghuilouyu.cn

guard let x = opt else { return }
来源：http://nmj.chenlongwang.top

[T30] Swift：协议
来源：http://bwt.nanxinkj.top

protocol Shape { func area() -> Double }
来源：http://flo.yuanzhike.top

[T31] Lua：Hello World
来源：http://yxs.chenzaomai.com

print("Hello")
来源：http://qmd.yuxming.cn

[T32] Lua：局部变量
来源：http://aeb.daria6918.cn

local a = 1
来源：http://fxl.yueranfly.top

[T33] Lua：表（数组）
来源：http://ytc.havefunace.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jyi.nwbrower.top

[T34] Lua：遍历表
来源：http://uhz.zhaomingkeji.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://iwa.shanyushiyangkeji.top

[T35] Lua：字典表
来源：http://fhc.ywan-chungtsiang.top

local d = { a = 1 };  d.b = 2
来源：http://ucp.sysykeji.top

[T36] Lua：函数
来源：http://sfp.vqdsnc.cn

function add(a, b) return a + b end
来源：http://dyv.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://cib.pengpengdd.cyou

"a" .. "b"
来源：http://faj.sxryk.cn

[T38] Lua：条件
来源：http://fgt.xylfe.cn

if x > 0 then print("正") end
来源：http://tqt.xinyue.icu

[T39] Lua：模式匹配
来源：http://ywn.bjfxy.top

string.find(s, "%d+")
来源：http://lty.fanxiaobao.xyz

[T40] Lua：元表
来源：http://qun.jiagoushi.top

setmetatable({}, { __index = base })
来源：http://trd.quarkkingdee.top

[T41] Perl：Hello World
来源：http://nnp.shanyushiyangkeji.top

print "Hello\n";
来源：http://jgz.shuidangran.top

[T42] Perl：变量类型
来源：http://ddh.feifeiyinyue.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sxz.hywenlv.cn

[T43] Perl：字符串插值
来源：http://mxu.chenlongwang.top

"值: $a"
来源：http://lud.zhoulong.xyz

[T44] Perl：条件
来源：http://qno.iojbl.cn

if ($a > 0) { print "正"; }
来源：http://nao.yj202588.top

[T45] Perl：数组遍历
来源：http://wco.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://wgy.yj20258888.top

[T46] Perl：哈希操作
来源：http://iea.meibo888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kjm.quarkkingdee.top

[T47] Perl：正则捕获
来源：http://bde.sweek.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://laa.jinqigfzy.top

[T48] Perl：正则替换
来源：http://iql.wangshuangyany.cn

$s =~ s/old/new/g;
来源：http://fsb.redwolf501.top

[T49] Perl：函数
来源：http://niq.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ffu.jlsjyb.cn

[T50] Perl：逐行读文件
来源：http://bhj.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bsc.hywenlv.cn

while (my $line = <$fh>) { print $line; }
来源：http://dgk.wangdashe.top

[T51] Scala：Hello World
来源：http://zxa.fengsongda.top

println("Hello")
来源：http://yan.uphjek.com

[T52] Scala：变量
来源：http://iol.xziqi.cn

val a = 1;  var b = 2
来源：http://pon.sxryk.cn

[T53] Scala：字符串插值
来源：http://btg.yj20258.top

s"值: $b"
来源：http://fap.sjlbkw.cn

[T54] Scala：集合映射
来源：http://wkg.yfazqb.com

List(1, 2, 3).map(_ * 2)
来源：http://cgd.ivvv.top

[T55] Scala：集合过滤
来源：http://rym.jyoumei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zdh.xuanzx.com

[T56] Scala：样例类
来源：http://jwv.chenlongwang.top

case class User(name: String, age: Int)
来源：http://max.tarul.cn

[T57] Scala：模式匹配
来源：http://dxu.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://jhy.yj202588.top

[T58] Scala：函数定义
来源：http://fdj.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bho.fanxiaobao.xyz

[T59] Scala：循环
来源：http://gok.jiagoushi.top

for (i <- 1 to 10) println(i)
来源：http://iwd.shzxlz.cn

[T60] Scala：折叠
来源：http://kap.smart0.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ulc.uphjek.com

================================================================================
来源：http://khx.smart0.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ohg.yangfankeji.com

================================================================================
来源：http://agu.ctjpmb.com

[U01] Py：创建虚拟环境
来源：http://zwt.hfpthk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wqf.hcnkem.com

[U02] Py：导出 / 安装依赖
来源：http://fhy.hnqzz.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vxv.mhx1999.top

[U03] Py：加载 .env 配置
来源：http://swj.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://ofh.birdmap.top

[U04] Py：变量调试打印
来源：http://ozm.xuetiantiany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qad.dashuyun.cn

[U05] Py：列表去重且保序
来源：http://twl.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://zlo.havefunace.top

[U06] Py：合并两个字典
来源：http://lpj.zdqjudy.top

{**a, **b}
来源：http://kli.iojbl.cn

[U07] Py：反转字典键值
来源：http://byu.xylfe.cn

{v: k for k, v in d.items()}
来源：http://iva.aibaodan.cn

[U08] Py：展平二维列表
来源：http://fjd.dianchejie.cn

[y for x in nested for y in x]
来源：http://hum.jqgfzy.top

[U09] Py：字典取最大值的键
来源：http://lsh.ehwqpu.com

max(d, key=d.get)
来源：http://ixr.hywenlv.cn

[U10] Py：按值排序字典
来源：http://qjc.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://inv.yj20258.top

[U11] Py：生成器表达式
来源：http://qvo.yanxiufei.cn

(x * 2 for x in arr)
来源：http://hgt.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://vyx.pycfn.com

Counter(arr).most_common(3)
来源：http://nkw.daria6918.cn

[U13] Py：固定长度队列
来源：http://irg.gaohongyu789.top

deque(maxlen=10)
来源：http://inn.jiagoushi.top

[U14] Py：分组收集到列表
来源：http://gtl.chenzaomai.com

defaultdict(list)
来源：http://cps.yj20258.top

[U15] Py：高精度计时
来源：http://rqr.9152youxi.cn

t = time.perf_counter()
来源：http://nwb.epnwcf.com

[U16] Py：命令行参数解析
来源：http://hxs.fengsongda.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rir.sjlbkw.cn

[U17] Py：初始化日志
来源：http://ozb.gotoacloud.top

logging.basicConfig(level=logging.INFO)
来源：http://ddr.yfazqb.com

[U18] Py：预编译正则
来源：http://owg.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://xmj.vqdsnc.cn

[U19] Py：正则替换带回调
来源：http://zfw.zhixingplan.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mqs.shangyingyoupin.top

[U20] Py：缓存函数结果
来源：http://xsx.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://irz.yuanzhike.top

[U21] Py：自定义上下文管理器
来源：http://flr.hywenlv.cn

@contextlib.contextmanager
来源：http://aew.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://hzl.yangfankeji.com

list(zip(*m))
来源：http://nce.ppjwa.cn

[U23] Py：分块读取大文件
来源：http://ryw.zhengqikj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iub.daxiang520.top

[U24] Py：路径操作
来源：http://lwa.jinghuilouyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aki.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://msi.ctjpmb.com

csv.DictReader(f)
来源：http://tgd.sysykeji.top

[U26] Py：并发下载
来源：http://ftf.yongpay.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://get.bbcook.cn

[U27] Py：异步 HTTP
来源：http://hkw.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://weo.wangshuangyany.cn

[U28] Py：类型别名
来源：http://uud.xziqi.cn

UserId = int
来源：http://kpm.hnqzz.top

[U29] Py：属性校验
来源：http://vap.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://rfk.jinqigufen.top

[U30] Py：数据类
来源：http://rmz.sysykeji.top

@dataclass(slots=True)
来源：http://czz.jlsjyb.cn

[U31] Py：单测
来源：http://cpv.xingfuxueyuan.xyz

python -m pytest -q
来源：http://wgj.hesvh.cn

[U32] Py：代码格式化
来源：http://jut.cucudq.cn

ruff format . && ruff check --fix .
来源：http://pkr.xuetiantiany.cn

[U33] Py：打包发布
来源：http://gvk.andypj.xyz

python -m build  （依赖 pyproject.toml）
来源：http://hkr.daria6918.cn

[U34] Py：判断编码
来源：http://yyq.hfpthk.cn

chardet.detect(raw)
来源：http://aqh.yuanzhike.top

[U35] Py：发送邮件
来源：http://afo.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sbp.svipenyu.cn

[U36] Py：定时任务
来源：http://fsb.sxryk.cn

schedule.every(10).minutes.do(job)
来源：http://vck.c1oappe.top

[U37] Py：读写 Excel
来源：http://ztq.shuidangran.top

pandas.read_excel / DataFrame.to_excel
来源：http://slo.yj202588.top

[U38] Py：获取脚本所在目录
来源：http://hcj.nwbrower.top

Path(__file__).resolve().parent
来源：http://bmj.shzxlz.cn

[U39] Py：判断是否在交互环境
来源：http://yhf.kuanghao11.cn

sys.stdout.isatty()
来源：http://ekp.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://tcr.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://gup.316326.xyz

[U41] PHP：初始化 Composer 项目
来源：http://qzg.cucudq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tvu.jinqigufen.top

[U42] PHP：PSR-4 自动加载
来源：http://lol.bjfxy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wbi.yj20258888.top

[U43] PHP：声明命名空间
来源：http://php.yongpay.top

namespace App\Http;
来源：http://ext.aizwys.cn

[U44] PHP：开启严格类型
来源：http://wbr.bbcook.cn

declare(strict_types=1);
来源：http://yjd.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://toh.hammf.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://buc.nanxuanxn.top

[U46] PHP：可空类型
来源：http://kck.hnqzz.top

?string $name = null
来源：http://wjk.guannengcc.top

[U47] PHP：联合类型
来源：http://fph.yuxming.cn

int|string $id
来源：http://gyg.fehbvm.com

[U48] PHP：纯枚举
来源：http://arv.yanxiufei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jyu.redwolf501.top

[U49] PHP：只读属性
来源：http://lef.fktsv.cn

public readonly string $name
来源：http://ugo.ppjwa.cn

[U50] PHP：构造器属性提升
来源：http://nye.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://ajv.ywan-chungtsiang.top

[U51] PHP：数组解构
来源：http://xuu.fanxiaobao.xyz

[$a, $b] = $arr;
来源：http://phy.tian-w.cn

[U52] PHP：箭头函数
来源：http://jic.nanxinkj.top

$double = fn($x) => $x * 2;
来源：http://auv.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://hbs.tianlin.xyz

$v = $a ?? $b ?? "default";
来源：http://mva.guannengcc.top

[U54] PHP：空安全调用
来源：http://efa.fehbvm.com

$obj?->method()
来源：http://gtf.sxryk.cn

[U55] PHP：match 表达式
来源：http://ljj.feifeiyinyue.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zbq.nwbrower.top

[U56] PHP：命名参数
来源：http://wyc.zhoulong.xyz

f(a: 1, b: 2)
来源：http://qmj.xuanzx.com

[U57] PHP：字符串插值
来源：http://tyl.hnxiangtu.top

"值: {$a}"
来源：http://def.316326.xyz

[U58] PHP：数组三件套
来源：http://ogi.redwolf501.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iir.yonumen.top

[U59] PHP：自定义排序
来源：http://pqe.jinyuanbaomall.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://efv.haohaochexian.top

[U60] PHP：JSON 编解码
来源：http://vod.quarkkingdee.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dcm.fanxiaobao.xyz

[U61] PHP：正则
来源：http://vdw.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pia.hnqzz.top

[U62] PHP：日期对象
来源：http://kvt.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jbe.yj202588.top

[U63] PHP：文件读写
来源：http://pbv.jinghuilouyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bxg.chenjidiqi.icu

[U64] PHP：目录遍历
来源：http://kep.fengsongda.top

glob("dir/*.php");  scandir("dir");
来源：http://fgc.wangdashe.top

[U65] PHP：会话
来源：http://ftc.52xcode.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wmz.feifeiyinyue.top

[U66] PHP：设置 Cookie
来源：http://rbr.birdmap.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sag.vqdsnc.cn

[U67] PHP：处理文件上传
来源：http://aes.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wml.jqgfzy.top

[U68] PHP：PDO 连接
来源：http://iqd.shangyingyoupin.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jgo.zhongyouzk.top

[U69] PHP：PDO 预处理
来源：http://ruy.jinghuilouyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lvk.tarul.cn

[U70] PHP：PDO 事务
来源：http://xfk.jyoumei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://plo.jinghuilouyu.cn

[U71] PHP：抛出异常
来源：http://ziz.yuanzhike.top

throw new RuntimeException("失败", 500);
来源：http://qly.c1oappe.top

[U72] PHP：写错误日志
来源：http://umc.316326.xyz

error_log("失败: " . $e->getMessage());
来源：http://drm.yongpay.top

[U73] PHP：读取 ini 配置
来源：http://qsh.zhixingplan.top

parse_ini_file("config.ini", true)
来源：http://cob.ivvv.top

[U74] PHP：读取环境变量
来源：http://jyu.9152youxi.cn

getenv("APP_ENV") ?: "production"
来源：http://soz.xuanzx.com


<!-- 参考信息 -->