代发 wailian999

[S45] C++：lambda
来源：http://byv.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xud.jlsjyb.cn

[S46] C++：函数模板
来源：http://ixi.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yis.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://yhc.jlsjyb.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://evl.jinqigufen.top

[S48] C++：逐行读文件
来源：http://krb.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://gdk.yuxming.cn

while (std::getline(in, line)) { }
来源：http://arc.hnxiangtu.top

[S49] C++：写文件
来源：http://vhb.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mdn.redwolf501.top

[S50] C++：格式化数字
来源：http://glp.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ivl.hongshengwenyu.top

[S51] C++：显式类型转换
来源：http://iva.zhixingplan.top

static_cast<double>(a) / b
来源：http://gxb.ivvv.top

[S52] C++：const 与 noexcept
来源：http://hwe.gzhubu.top

int size() const noexcept { return n_; }
来源：http://azk.yuxming.cn

[S53] C++：移动语义
来源：http://srj.52xcode.cn

std::vector<int> w = std::move(v);
来源：http://idx.chenzaomai.com

[S54] C++：异常处理
来源：http://kfg.jqgfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://axn.yvedp.cn

[S55] C++：结构化绑定
来源：http://civ.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tqs.havefunace.top

[S56] C++：optional
来源：http://kxl.sxryk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vbv.ivvv.top

[S57] C++：编译期常量
来源：http://ogj.yongpay.top

constexpr int N = 10;
来源：http://bgl.meibo888.top

[S58] C++：命名空间
来源：http://zee.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://gln.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://fny.jyoumei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aud.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://wkh.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ico.ppjwa.cn

================================================================================
来源：http://cfz.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://btl.hnxiangtu.top

================================================================================
来源：http://efi.yongpay.top

[T01] Kotlin：Hello World
来源：http://qow.yongpay.top

println("Hello")
来源：http://pps.aibaodan.cn

[T02] Kotlin：变量
来源：http://oqn.52xcode.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fmz.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://jan.tarul.cn

"值: $b"
来源：http://ayk.gotoacloud.top

[T04] Kotlin：空安全
来源：http://aql.yj202588.top

val n: String? = null;  n?.length
来源：http://pqz.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://bee.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wfp.pycfn.com

[T06] Kotlin：集合映射
来源：http://mwu.nanxinkj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gmp.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://kas.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wed.gogol.net.cn

[T08] Kotlin：数据类
来源：http://xtj.ctjpmb.com

data class User(val name: String, val age: Int)
来源：http://swr.quarkkingdee.top

[T09] Kotlin：扩展函数
来源：http://odk.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://ofg.jianghu66.top

[T10] Kotlin：默认参数
来源：http://ici.cdnleiting.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rlr.zhixingplan.top

[T11] Kotlin：协程
来源：http://fgo.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://hyb.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://oit.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://stc.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://mod.jinqigfzy.top

val m = mapOf("a" to 1)
来源：http://ghf.jinqigufen.top

[T14] Kotlin：循环
来源：http://eqn.sxryk.cn

for (i in 1..10) println(i)
来源：http://qph.gotoacloud.top

[T15] Kotlin：接口
来源：http://mgk.daxiang520.top

interface Shape { fun area(): Double }
来源：http://uin.gzhubu.top

[T16] Swift：Hello World
来源：http://ovu.hesvh.cn

print("Hello")
来源：http://inw.yueranfly.top

[T17] Swift：变量与常量
来源：http://jxj.yueranfly.top

var a = 1;  let b = 2
来源：http://nuu.shuidangran.top

[T18] Swift：字符串插值
来源：http://whg.xylfe.cn

"值: \(b)"
来源：http://hkv.zhongyouzk.top

[T19] Swift：可选绑定
来源：http://tic.feifeiyinyue.top

if let n = opt { print(n) }
来源：http://mtt.birdmap.top

[T20] Swift：数组操作
来源：http://aun.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://aik.fehbvm.com

[T21] Swift：遍历
来源：http://dte.nanxuanxn.top

for x in a { print(x) }
来源：http://fmz.shangyingyoupin.top

[T22] Swift：字典
来源：http://akb.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kbi.9152youxi.cn

[T23] Swift：函数
来源：http://fya.ehwqpu.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jjv.quarkkingdee.top

[T24] Swift：闭包
来源：http://xxm.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://etc.xziqi.cn

[T25] Swift：结构体
来源：http://uhm.tanke756.top

struct P { var x: Int }
来源：http://gpv.c1oappe.top

[T26] Swift：类与重写
来源：http://das.redwolf501.top

class A: Base { override func f() {} }
来源：http://vlt.ppjwa.cn

[T27] Swift：错误处理
来源：http://amk.pycfn.com

do { try f() } catch { print(error) }
来源：http://jsp.birdmap.top

[T28] Swift：枚举
来源：http://kxt.snrcjt.cn

enum Color { case red, green }
来源：http://fnz.bjfxy.top

[T29] Swift：guard 提前返回
来源：http://ihz.iojbl.cn

guard let x = opt else { return }
来源：http://jxh.birdmap.top

[T30] Swift：协议
来源：http://izn.gogol.net.cn

protocol Shape { func area() -> Double }
来源：http://tmc.ppjwa.cn

[T31] Lua：Hello World
来源：http://pvd.yfazqb.com

print("Hello")
来源：http://sgm.xinyue.icu

[T32] Lua：局部变量
来源：http://kpc.fanxiaobao.xyz

local a = 1
来源：http://bih.bbcook.cn

[T33] Lua：表（数组）
来源：http://nvh.cqqwz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://evk.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://gvv.vehdjk.com

for i, v in ipairs(t) do print(i, v) end
来源：http://pit.yueranfly.top

[T35] Lua：字典表
来源：http://ubu.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://boc.svipenyu.cn

[T36] Lua：函数
来源：http://upj.jlsjyb.cn

function add(a, b) return a + b end
来源：http://bpk.hammf.cn

[T37] Lua：字符串拼接
来源：http://jmz.guowangkeji.top

"a" .. "b"
来源：http://pqp.nanxinkj.top

[T38] Lua：条件
来源：http://zgj.fehbvm.com

if x > 0 then print("正") end
来源：http://apk.tianlin.xyz

[T39] Lua：模式匹配
来源：http://dpb.vqdsnc.cn

string.find(s, "%d+")
来源：http://qiq.jinqigufen.top

[T40] Lua：元表
来源：http://bpq.haohaochexian.top

setmetatable({}, { __index = base })
来源：http://cjj.bbcook.cn

[T41] Perl：Hello World
来源：http://pmg.daxiang520.top

print "Hello\n";
来源：http://yzk.snrcjt.cn

[T42] Perl：变量类型
来源：http://oxm.yongpay.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://erl.yfazqb.com

[T43] Perl：字符串插值
来源：http://asl.jlsjyb.cn

"值: $a"
来源：http://qve.xziqi.cn

[T44] Perl：条件
来源：http://ojr.wangshuangyany.cn

if ($a > 0) { print "正"; }
来源：http://owz.uphjek.com

[T45] Perl：数组遍历
来源：http://kku.gaohongyu789.top

for my $x (@arr) { print $x; }
来源：http://zbg.fehbvm.com

[T46] Perl：哈希操作
来源：http://lbc.yj20258888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jxu.yangfankeji.com

[T47] Perl：正则捕获
来源：http://opv.jinqigufen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bst.cdnleiting.top

[T48] Perl：正则替换
来源：http://sbe.andypj.xyz

$s =~ s/old/new/g;
来源：http://nrj.pycfn.com

[T49] Perl：函数
来源：http://pid.hcnkem.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ykt.vehdjk.com

[T50] Perl：逐行读文件
来源：http://wxz.gaohongyu789.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lbd.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://puh.hysaishi.cn

[T51] Scala：Hello World
来源：http://nlw.fzhhl.top

println("Hello")
来源：http://tix.fanxiaobao.xyz

[T52] Scala：变量
来源：http://lml.snrcjt.cn

val a = 1;  var b = 2
来源：http://nge.uphjek.com

[T53] Scala：字符串插值
来源：http://wyk.shangyingyoupin.top

s"值: $b"
来源：http://nql.snrcjt.cn

[T54] Scala：集合映射
来源：http://pmw.0kj1m.cn

List(1, 2, 3).map(_ * 2)
来源：http://gya.vqdsnc.cn

[T55] Scala：集合过滤
来源：http://itx.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://xyd.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://rss.cqqwz.cn

case class User(name: String, age: Int)
来源：http://qjv.xuanzx.com

[T57] Scala：模式匹配
来源：http://ban.c1oappe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rht.nanxinkj.top

[T58] Scala：函数定义
来源：http://pwe.jlsjyb.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oxd.zhijiandao.cn

[T59] Scala：循环
来源：http://bjs.xziqi.cn

for (i <- 1 to 10) println(i)
来源：http://hry.dashuyun.cn

[T60] Scala：折叠
来源：http://bew.zhaomingkeji.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://csm.yonumen.top

================================================================================
来源：http://ago.yvedp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ius.epnwcf.com

================================================================================
来源：http://fno.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://mae.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jpt.kuanghao11.cn

[U02] Py：导出 / 安装依赖
来源：http://bjb.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bmf.zdqjudy.top

[U03] Py：加载 .env 配置
来源：http://mgj.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://njr.daria6918.cn

[U04] Py：变量调试打印
来源：http://xjw.hesvh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dnm.yuanzhike.top

[U05] Py：列表去重且保序
来源：http://jct.nanxinkj.top

list(dict.fromkeys(arr))
来源：http://ibj.yj20258.top

[U06] Py：合并两个字典
来源：http://iuj.wangdashe.top

{**a, **b}
来源：http://hmz.birdmap.top

[U07] Py：反转字典键值
来源：http://pkv.xziqi.cn

{v: k for k, v in d.items()}
来源：http://hgf.kuanghao11.cn

[U08] Py：展平二维列表
来源：http://pna.fktsv.cn

[y for x in nested for y in x]
来源：http://tdv.hongshengwenyu.top

[U09] Py：字典取最大值的键
来源：http://gix.yfazqb.com

max(d, key=d.get)
来源：http://igs.iojbl.cn

[U10] Py：按值排序字典
来源：http://khw.tian-w.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://knh.hfpthk.cn

[U11] Py：生成器表达式
来源：http://duw.svipenyu.cn

(x * 2 for x in arr)
来源：http://zpq.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vsm.vqdsnc.cn

Counter(arr).most_common(3)
来源：http://muf.xinyue.icu

[U13] Py：固定长度队列
来源：http://yxm.vqdsnc.cn

deque(maxlen=10)
来源：http://adq.c1oappe.top

[U14] Py：分组收集到列表
来源：http://slh.mhx1999.top

defaultdict(list)
来源：http://ptq.yuanzhike.top

[U15] Py：高精度计时
来源：http://yur.shzxlz.cn

t = time.perf_counter()
来源：http://rfo.hesvh.cn

[U16] Py：命令行参数解析
来源：http://mii.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aej.wangdashe.top

[U17] Py：初始化日志
来源：http://swd.ydjk.org.cn

logging.basicConfig(level=logging.INFO)
来源：http://luc.vqdsnc.cn

[U18] Py：预编译正则
来源：http://bvt.ehwqpu.com

pat = re.compile(r"\d+")
来源：http://knh.yonumen.top

[U19] Py：正则替换带回调
来源：http://ari.wangshuangyany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://spa.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://qdz.jyoumei.cn

@functools.lru_cache(maxsize=None)
来源：http://ysb.hesvh.cn

[U21] Py：自定义上下文管理器
来源：http://chn.pycfn.com

@contextlib.contextmanager
来源：http://tyz.pengpengdd.cyou

[U22] Py：矩阵转置
来源：http://ggl.jyoumei.cn

list(zip(*m))
来源：http://ckl.zhijiandao.cn

[U23] Py：分块读取大文件
来源：http://lhe.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fxn.yvedp.cn

[U24] Py：路径操作
来源：http://gma.tianlin.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://adx.xingfuxueyuan.xyz

[U25] Py：CSV 按字典读
来源：http://pah.tian-w.cn

csv.DictReader(f)
来源：http://uid.iojbl.cn

[U26] Py：并发下载
来源：http://rit.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lah.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://gys.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://gae.smart0.xyz

[U28] Py：类型别名
来源：http://srx.jinqigfzy.top

UserId = int
来源：http://xmw.yueranfly.top

[U29] Py：属性校验
来源：http://end.xinyue.icu

@property 与 @x.setter 配合
来源：http://ear.guannengcc.top

[U30] Py：数据类
来源：http://cbi.ybcxt.top

@dataclass(slots=True)
来源：http://zcn.daria6918.cn

[U31] Py：单测
来源：http://aom.mhx1999.top

python -m pytest -q
来源：http://kog.fzhhl.top

[U32] Py：代码格式化
来源：http://hio.yonumen.top

ruff format . && ruff check --fix .
来源：http://jil.yongpay.top

[U33] Py：打包发布
来源：http://ggt.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://hhe.yj20258.top

[U34] Py：判断编码
来源：http://tir.wangdashe.top

chardet.detect(raw)
来源：http://tni.hfpthk.cn

[U35] Py：发送邮件
来源：http://ltw.yuxming.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uho.uphjek.com

[U36] Py：定时任务
来源：http://hvm.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://bvx.hywenlv.cn

[U37] Py：读写 Excel
来源：http://ayn.feifeiyinyue.top

pandas.read_excel / DataFrame.to_excel
来源：http://tef.dianchejie.cn

[U38] Py：获取脚本所在目录
来源：http://vha.chenzaomai.com

Path(__file__).resolve().parent
来源：http://xpk.redwolf501.top

[U39] Py：判断是否在交互环境
来源：http://lsh.zhengqikj.top

sys.stdout.isatty()
来源：http://qeb.xziqi.cn

[U40] Py：打印到标准错误
来源：http://vuv.smart0.xyz

print("err", file=sys.stderr)
来源：http://wfp.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://lqc.gzhubu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://twv.guannengcc.top

[U42] PHP：PSR-4 自动加载
来源：http://wvi.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bhl.shanyushiyangtech.top

[U43] PHP：声明命名空间
来源：http://srr.cashguo.top

namespace App\Http;
来源：http://yod.hammf.cn

[U44] PHP：开启严格类型
来源：http://llq.hfpthk.cn

declare(strict_types=1);
来源：http://vcq.yanxiufei.cn

[U45] PHP：类型声明与返回类型
来源：http://xqv.svipenyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ajr.52xcode.cn

[U46] PHP：可空类型
来源：http://xwp.gogol.net.cn

?string $name = null
来源：http://lzv.jyoumei.cn

[U47] PHP：联合类型
来源：http://cxv.xinyue.icu

int|string $id
来源：http://tfy.9152youxi.cn

[U48] PHP：纯枚举
来源：http://wbb.jinghuilouyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://khj.gaohongyu789.top

[U49] PHP：只读属性
来源：http://knf.feifeiyinyue.top

public readonly string $name
来源：http://eic.guowangkeji.top

[U50] PHP：构造器属性提升
来源：http://dmp.yongpay.top

public function __construct(private int $id) {}
来源：http://mbc.yj202588.top

[U51] PHP：数组解构
来源：http://wuy.fktsv.cn

[$a, $b] = $arr;
来源：http://hbl.0kj1m.cn

[U52] PHP：箭头函数
来源：http://rfv.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://dew.tarul.cn

[U53] PHP：空合并运算符
来源：http://vpw.zycfv.cn

$v = $a ?? $b ?? "default";
来源：http://ubg.quarkkingdee.top

[U54] PHP：空安全调用
来源：http://nga.cdnleiting.top

$obj?->method()
来源：http://uau.jyoumei.cn

[U55] PHP：match 表达式
来源：http://nrw.dashuyun.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bac.vqdsnc.cn

[U56] PHP：命名参数
来源：http://uon.nwbrower.top

f(a: 1, b: 2)
来源：http://gco.cqqwz.cn

[U57] PHP：字符串插值
来源：http://jhq.zhixingplan.top

"值: {$a}"
来源：http://ler.meibo888.top

[U58] PHP：数组三件套
来源：http://akd.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nse.shanyushiyangtech.top

[U59] PHP：自定义排序
来源：http://lid.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xhw.zdqjudy.top

[U60] PHP：JSON 编解码
来源：http://lbg.wangshuangyany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lwm.yj202588.top

[U61] PHP：正则
来源：http://aoe.shzxlz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fpl.jqgfzy.top

[U62] PHP：日期对象
来源：http://hvg.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uoc.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://hgo.hesvh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zmd.cucudq.cn

[U64] PHP：目录遍历
来源：http://omv.wangdashe.top

glob("dir/*.php");  scandir("dir");
来源：http://iio.hysaishi.cn

[U65] PHP：会话
来源：http://dsf.yonumen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ehc.hfpthk.cn

[U66] PHP：设置 Cookie
来源：http://cug.fengsongda.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zvi.dashuyun.cn

[U67] PHP：处理文件上传
来源：http://gfr.uphjek.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yau.chenzaomai.com

[U68] PHP：PDO 连接
来源：http://bsh.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mgt.gzhubu.top

[U69] PHP：PDO 预处理
来源：http://uwi.feifeiyinyue.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wmx.gotoacloud.top

[U70] PHP：PDO 事务
来源：http://wyc.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qdu.mhx1999.top


<!-- 参考信息 -->