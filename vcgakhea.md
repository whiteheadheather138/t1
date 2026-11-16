代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://pkc.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kda.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://uwi.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fue.hongshengwenyu.top

while (std::getline(in, line)) { }
来源：http://njy.yongpay.top

[S49] C++：写文件
来源：http://inx.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://axq.9152youxi.cn

[S50] C++：格式化数字
来源：http://txr.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ntk.fzhhl.top

[S51] C++：显式类型转换
来源：http://bil.cheryme.top

static_cast<double>(a) / b
来源：http://xgk.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://wxs.meibo888.top

int size() const noexcept { return n_; }
来源：http://aog.yongpay.top

[S53] C++：移动语义
来源：http://eol.jinqigufen.top

std::vector<int> w = std::move(v);
来源：http://vow.bbcook.cn

[S54] C++：异常处理
来源：http://tva.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://efz.hcnkem.com

[S55] C++：结构化绑定
来源：http://ccg.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tii.tian-w.cn

[S56] C++：optional
来源：http://jrp.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tfr.gaohongyu789.top

[S57] C++：编译期常量
来源：http://hkh.yongpay.top

constexpr int N = 10;
来源：http://yeh.svipenyu.cn

[S58] C++：命名空间
来源：http://opk.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://txv.ywan-chungtsiang.top

[S59] C++：静态断言
来源：http://vsx.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bld.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://sym.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://saf.ybcxt.top

================================================================================
来源：http://lwe.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nex.xylfe.cn

================================================================================
来源：http://lty.yj202588.top

[T01] Kotlin：Hello World
来源：http://rji.ywan-chungtsiang.top

println("Hello")
来源：http://mjf.quarkkingdee.top

[T02] Kotlin：变量
来源：http://eyh.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bxq.xinyue.icu

[T03] Kotlin：字符串模板
来源：http://aqz.shangyingyoupin.top

"值: $b"
来源：http://che.sxryk.cn

[T04] Kotlin：空安全
来源：http://fem.gzhubu.top

val n: String? = null;  n?.length
来源：http://dtw.nanxuanxn.top

[T05] Kotlin：when 表达式
来源：http://asc.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yfp.pycfn.com

[T06] Kotlin：集合映射
来源：http://odt.jqgfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jgq.hcnkem.com

[T07] Kotlin：集合过滤
来源：http://ozd.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://tpr.hammf.cn

[T08] Kotlin：数据类
来源：http://ypq.tarul.cn

data class User(val name: String, val age: Int)
来源：http://mge.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://oak.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://fel.wangshuangyany.cn

[T10] Kotlin：默认参数
来源：http://efe.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://eij.cucudq.cn

[T11] Kotlin：协程
来源：http://pum.shuidangran.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fnl.sysykeji.top

[T12] Kotlin：解构声明
来源：http://gfg.tianlin.xyz

val (a, b) = Pair(1, 2)
来源：http://hlt.andypj.xyz

[T13] Kotlin：只读 Map
来源：http://nlc.wangshuangyany.cn

val m = mapOf("a" to 1)
来源：http://pxs.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://swj.cqqwz.cn

for (i in 1..10) println(i)
来源：http://dwj.zycfv.cn

[T15] Kotlin：接口
来源：http://fmt.jyoumei.cn

interface Shape { fun area(): Double }
来源：http://wzs.ehwqpu.com

[T16] Swift：Hello World
来源：http://alx.zhixingplan.top

print("Hello")
来源：http://qcj.xinyue.icu

[T17] Swift：变量与常量
来源：http://rpg.bbcook.cn

var a = 1;  let b = 2
来源：http://thq.shangyingyoupin.top

[T18] Swift：字符串插值
来源：http://fsg.vqdsnc.cn

"值: \(b)"
来源：http://hji.yongpay.top

[T19] Swift：可选绑定
来源：http://ecl.pycfn.com

if let n = opt { print(n) }
来源：http://rdx.pengpengdd.cyou

[T20] Swift：数组操作
来源：http://yux.jinghuilouyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rei.xylfe.cn

[T21] Swift：遍历
来源：http://djx.jyoumei.cn

for x in a { print(x) }
来源：http://jto.zhoulong.xyz

[T22] Swift：字典
来源：http://bqx.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://evr.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://lml.guannengcc.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ryr.uphjek.com

[T24] Swift：闭包
来源：http://eoy.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lwv.pycfn.com

[T25] Swift：结构体
来源：http://mzs.haohaochexian.top

struct P { var x: Int }
来源：http://rbs.ppjwa.cn

[T26] Swift：类与重写
来源：http://sup.nwbrower.top

class A: Base { override func f() {} }
来源：http://gbh.hnxiangtu.top

[T27] Swift：错误处理
来源：http://ide.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://pmc.wangdashe.top

[T28] Swift：枚举
来源：http://xes.ctjpmb.com

enum Color { case red, green }
来源：http://srh.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://agu.iojbl.cn

guard let x = opt else { return }
来源：http://wpi.xuetiantiany.cn

[T30] Swift：协议
来源：http://kbk.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://rlg.xylfe.cn

[T31] Lua：Hello World
来源：http://dbv.xinyue.icu

print("Hello")
来源：http://zmx.bjfxy.top

[T32] Lua：局部变量
来源：http://pdf.zhiwuduotai.top

local a = 1
来源：http://xdq.tarul.cn

[T33] Lua：表（数组）
来源：http://zrg.zhijiandao.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://plp.cucudq.cn

[T34] Lua：遍历表
来源：http://tjm.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://axq.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://anz.dashuyun.cn

local d = { a = 1 };  d.b = 2
来源：http://vze.xuanzx.com

[T36] Lua：函数
来源：http://dcp.epnwcf.com

function add(a, b) return a + b end
来源：http://zcp.nwbrower.top

[T37] Lua：字符串拼接
来源：http://nsq.hcnkem.com

"a" .. "b"
来源：http://cot.sweek.top

[T38] Lua：条件
来源：http://mky.hongshengwenyu.top

if x > 0 then print("正") end
来源：http://vel.c1oappe.top

[T39] Lua：模式匹配
来源：http://oku.pycfn.com

string.find(s, "%d+")
来源：http://jzy.52xcode.cn

[T40] Lua：元表
来源：http://vxl.zycfv.cn

setmetatable({}, { __index = base })
来源：http://ijz.daxiang520.top

[T41] Perl：Hello World
来源：http://hmr.zhoulong.xyz

print "Hello\n";
来源：http://ekv.gotoacloud.top

[T42] Perl：变量类型
来源：http://djj.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://afy.jiagoushi.top

[T43] Perl：字符串插值
来源：http://lzk.snrcjt.cn

"值: $a"
来源：http://ttd.hfpthk.cn

[T44] Perl：条件
来源：http://ewy.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://mex.cheryme.top

[T45] Perl：数组遍历
来源：http://jdy.svipenyu.cn

for my $x (@arr) { print $x; }
来源：http://vha.shangyingyoupin.top

[T46] Perl：哈希操作
来源：http://clx.shanyushiyangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ndx.shanyushiyangkeji.top

[T47] Perl：正则捕获
来源：http://lcl.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://uuh.redwolf501.top

[T48] Perl：正则替换
来源：http://psm.uphjek.com

$s =~ s/old/new/g;
来源：http://lqg.aizwys.cn

[T49] Perl：函数
来源：http://qun.quarkkingdee.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://quv.yuxming.cn

[T50] Perl：逐行读文件
来源：http://ynv.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qao.jinghuilouyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://hyl.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://uaw.zhiwuduotai.top

println("Hello")
来源：http://ecb.bjfxy.top

[T52] Scala：变量
来源：http://pkm.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://qux.aizwys.cn

[T53] Scala：字符串插值
来源：http://yqy.ivvv.top

s"值: $b"
来源：http://dmp.snrcjt.cn

[T54] Scala：集合映射
来源：http://lun.xinyue.icu

List(1, 2, 3).map(_ * 2)
来源：http://oeu.yonumen.top

[T55] Scala：集合过滤
来源：http://yam.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://zsk.yanxiufei.cn

[T56] Scala：样例类
来源：http://yof.andypj.xyz

case class User(name: String, age: Int)
来源：http://yox.yueranfly.top

[T57] Scala：模式匹配
来源：http://zyz.chenzaomai.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://erq.sysykeji.top

[T58] Scala：函数定义
来源：http://ivl.xylfe.cn

def add(a: Int, b: Int): Int = a + b
来源：http://miz.fanxiaobao.xyz

[T59] Scala：循环
来源：http://tpm.ctjpmb.com

for (i <- 1 to 10) println(i)
来源：http://wib.yanxiufei.cn

[T60] Scala：折叠
来源：http://wmx.xinyue.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://izj.0kj1m.cn

================================================================================
来源：http://flk.iojbl.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hwl.ywan-chungtsiang.top

================================================================================
来源：http://gkr.yueranfly.top

[U01] Py：创建虚拟环境
来源：http://rrg.hnxiangtu.top

python -m venv .venv && source .venv/bin/activate
来源：http://icx.52xcode.cn

[U02] Py：导出 / 安装依赖
来源：http://nhh.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gmj.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://uii.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gwa.daxiang520.top

[U04] Py：变量调试打印
来源：http://kjq.jlsjyb.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pvl.sysykeji.top

[U05] Py：列表去重且保序
来源：http://ooj.bjfxy.top

list(dict.fromkeys(arr))
来源：http://kwh.havefunace.top

[U06] Py：合并两个字典
来源：http://jfo.cdnleiting.top

{**a, **b}
来源：http://fjx.daxiang520.top

[U07] Py：反转字典键值
来源：http://vke.tarul.cn

{v: k for k, v in d.items()}
来源：http://ggq.xingfuxueyuan.xyz

[U08] Py：展平二维列表
来源：http://kqj.316326.xyz

[y for x in nested for y in x]
来源：http://fnq.jlsjyb.cn

[U09] Py：字典取最大值的键
来源：http://usz.jlsjyb.cn

max(d, key=d.get)
来源：http://zxk.cheryme.top

[U10] Py：按值排序字典
来源：http://fzw.daxiang520.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ylv.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://fst.sxryk.cn

(x * 2 for x in arr)
来源：http://gdz.yj20258.top

[U12] Py：取出现最多的 3 个元素
来源：http://opk.pengpengdd.cyou

Counter(arr).most_common(3)
来源：http://gjw.shangyingyoupin.top

[U13] Py：固定长度队列
来源：http://age.zhijiandao.cn

deque(maxlen=10)
来源：http://hvt.chenlongwang.top

[U14] Py：分组收集到列表
来源：http://lbf.hammf.cn

defaultdict(list)
来源：http://ujk.cqqwz.cn

[U15] Py：高精度计时
来源：http://rkb.xziqi.cn

t = time.perf_counter()
来源：http://kqu.tianlin.xyz

[U16] Py：命令行参数解析
来源：http://qpa.jqgfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qhh.fengsongda.top

[U17] Py：初始化日志
来源：http://hnz.cashguo.top

logging.basicConfig(level=logging.INFO)
来源：http://xyn.ydjk.org.cn

[U18] Py：预编译正则
来源：http://ayy.shuidangran.top

pat = re.compile(r"\d+")
来源：http://clz.9152youxi.cn

[U19] Py：正则替换带回调
来源：http://vdl.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iez.tarul.cn

[U20] Py：缓存函数结果
来源：http://wop.haohaochexian.top

@functools.lru_cache(maxsize=None)
来源：http://vpn.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://nov.haohaochexian.top

@contextlib.contextmanager
来源：http://myy.ydzc1.top

[U22] Py：矩阵转置
来源：http://djy.iojbl.cn

list(zip(*m))
来源：http://wiy.epnwcf.com

[U23] Py：分块读取大文件
来源：http://car.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wpb.tianlin.xyz

[U24] Py：路径操作
来源：http://nfd.chenzaomai.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bib.fehbvm.com

[U25] Py：CSV 按字典读
来源：http://hjm.zhongyouzk.top

csv.DictReader(f)
来源：http://yaj.gotoacloud.top

[U26] Py：并发下载
来源：http://myi.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://snw.snrcjt.cn

[U27] Py：异步 HTTP
来源：http://umj.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://fhl.sufxvd.cn

[U28] Py：类型别名
来源：http://zal.snrcjt.cn

UserId = int
来源：http://udr.ppjwa.cn

[U29] Py：属性校验
来源：http://svk.jqgufenzy.top

@property 与 @x.setter 配合
来源：http://hda.bjfxy.top

[U30] Py：数据类
来源：http://ghh.yuanzhike.top

@dataclass(slots=True)
来源：http://tdj.wangshuangyany.cn

[U31] Py：单测
来源：http://nbe.yongpay.top

python -m pytest -q
来源：http://xbz.zhongyouzk.top

[U32] Py：代码格式化
来源：http://ect.jyoumei.cn

ruff format . && ruff check --fix .
来源：http://myd.fengsongda.top

[U33] Py：打包发布
来源：http://lxb.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://voz.hfpthk.cn

[U34] Py：判断编码
来源：http://wbc.quarkkingdee.top

chardet.detect(raw)
来源：http://uzn.gaohongyu789.top

[U35] Py：发送邮件
来源：http://wou.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ahp.jinqigufen.top

[U36] Py：定时任务
来源：http://phs.jqgfzy.top

schedule.every(10).minutes.do(job)
来源：http://lvb.ehwqpu.com

[U37] Py：读写 Excel
来源：http://orh.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://jfr.xuanzx.com

[U38] Py：获取脚本所在目录
来源：http://feq.hammf.cn

Path(__file__).resolve().parent
来源：http://rwy.xziqi.cn

[U39] Py：判断是否在交互环境
来源：http://tbs.tarul.cn

sys.stdout.isatty()
来源：http://gbp.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://uqt.hywenlv.cn

print("err", file=sys.stderr)
来源：http://pvw.jianghu66.top

[U41] PHP：初始化 Composer 项目
来源：http://oal.jqgufenzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qwq.shanyushiyangtech.top

[U42] PHP：PSR-4 自动加载
来源：http://goi.iojbl.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jod.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://uam.0kj1m.cn

namespace App\Http;
来源：http://oun.hnxiangtu.top

[U44] PHP：开启严格类型
来源：http://acv.nanxinkj.top

declare(strict_types=1);
来源：http://ugf.fanxiaobao.xyz

[U45] PHP：类型声明与返回类型
来源：http://zxd.9152youxi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://aze.ehwqpu.com

[U46] PHP：可空类型
来源：http://cxo.daxiang520.top

?string $name = null
来源：http://ika.snrcjt.cn

[U47] PHP：联合类型
来源：http://sfx.52xcode.cn

int|string $id
来源：http://fuq.zycfv.cn

[U48] PHP：纯枚举
来源：http://qpj.zhijiandao.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lem.daxiang520.top

[U49] PHP：只读属性
来源：http://rku.hongshengwenyu.top

public readonly string $name
来源：http://vmg.hongshengwenyu.top

[U50] PHP：构造器属性提升
来源：http://jde.yj20258.top

public function __construct(private int $id) {}
来源：http://ped.cheryme.top

[U51] PHP：数组解构
来源：http://wae.pycfn.com

[$a, $b] = $arr;
来源：http://hmj.9152youxi.cn

[U52] PHP：箭头函数
来源：http://twj.ehwqpu.com

$double = fn($x) => $x * 2;
来源：http://rsy.pengpengdd.cyou

[U53] PHP：空合并运算符
来源：http://pjo.52xcode.cn

$v = $a ?? $b ?? "default";
来源：http://lcg.zycfv.cn

[U54] PHP：空安全调用
来源：http://fzc.meibo888.top

$obj?->method()
来源：http://fbc.shuidangran.top

[U55] PHP：match 表达式
来源：http://lfv.chenjidiqi.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cvi.yanxiufei.cn

[U56] PHP：命名参数
来源：http://bnh.cqqwz.cn

f(a: 1, b: 2)
来源：http://hii.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://tje.yvedp.cn

"值: {$a}"
来源：http://meg.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://djb.cashguo.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hjd.xuanzx.com

[U59] PHP：自定义排序
来源：http://msu.yonumen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://opu.bjfxy.top

[U60] PHP：JSON 编解码
来源：http://wea.redwolf501.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yzs.zhoulong.xyz

[U61] PHP：正则
来源：http://gwp.andypj.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qfx.haohaochexian.top

[U62] PHP：日期对象
来源：http://soz.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bia.hnqzz.top

[U63] PHP：文件读写
来源：http://bmq.gogol.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oew.jinqigufen.top

[U64] PHP：目录遍历
来源：http://ndi.daxiang520.top

glob("dir/*.php");  scandir("dir");
来源：http://jyl.smart0.xyz

[U65] PHP：会话
来源：http://uyh.aibaodan.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://osj.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://ttx.hysaishi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yyg.fehbvm.com

[U67] PHP：处理文件上传
来源：http://iju.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gmk.316326.xyz

[U68] PHP：PDO 连接
来源：http://xhg.haohaochexian.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rnj.yongpay.top

[U69] PHP：PDO 预处理
来源：http://vva.snrcjt.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://myf.yj20258.top

[U70] PHP：PDO 事务
来源：http://uqu.shanyushiyangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aqo.52xcode.cn

[U71] PHP：抛出异常
来源：http://uxi.yvedp.cn

throw new RuntimeException("失败", 500);
来源：http://oul.cashguo.top

[U72] PHP：写错误日志
来源：http://msf.ywan-chungtsiang.top

error_log("失败: " . $e->getMessage());
来源：http://nbt.iojbl.cn


<!-- 参考信息 -->