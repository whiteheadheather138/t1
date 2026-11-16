代发 wailian999

while (std::getline(in, line)) { }
来源：http://vzl.zhijiandao.cn

[S49] C++：写文件
来源：http://rgs.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fkz.sxryk.cn

[S50] C++：格式化数字
来源：http://fxm.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jer.bjfxy.top

[S51] C++：显式类型转换
来源：http://vnq.bbcook.cn

static_cast<double>(a) / b
来源：http://ioe.daria6918.cn

[S52] C++：const 与 noexcept
来源：http://mjq.zhengqikj.top

int size() const noexcept { return n_; }
来源：http://zih.snrcjt.cn

[S53] C++：移动语义
来源：http://jle.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://edy.sysykeji.top

[S54] C++：异常处理
来源：http://mvg.wangshuangyany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wdg.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://spy.zhaomingkeji.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://ulw.yangfankeji.com

[S56] C++：optional
来源：http://iom.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tng.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://pki.xziqi.cn

constexpr int N = 10;
来源：http://fsr.epnwcf.com

[S58] C++：命名空间
来源：http://hmn.fktsv.cn

namespace ns { int f() { return 1; } }
来源：http://zye.jqgufenzy.top

[S59] C++：静态断言
来源：http://icy.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cgf.xinyue.icu

[S60] C++：遍历并删除元素
来源：http://byx.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://atx.nwbrower.top

================================================================================
来源：http://gne.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hnl.xinyue.icu

================================================================================
来源：http://ufc.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://owr.zhoulong.xyz

println("Hello")
来源：http://zuu.pycfn.com

[T02] Kotlin：变量
来源：http://bdq.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zbc.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://zrs.fktsv.cn

"值: $b"
来源：http://hxv.xziqi.cn

[T04] Kotlin：空安全
来源：http://jhx.guowangkeji.top

val n: String? = null;  n?.length
来源：http://zrx.jinqigufen.top

[T05] Kotlin：when 表达式
来源：http://yma.xziqi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tjl.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://ocu.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://heb.hnqzz.top

[T07] Kotlin：集合过滤
来源：http://vcm.mhx1999.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://psr.daxiang520.top

[T08] Kotlin：数据类
来源：http://cwk.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://pka.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://hjs.uphjek.com

fun String.exclaim() = this + "!"
来源：http://xet.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://own.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jea.shuidangran.top

[T11] Kotlin：协程
来源：http://eke.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wmm.hammf.cn

[T12] Kotlin：解构声明
来源：http://deg.9152youxi.cn

val (a, b) = Pair(1, 2)
来源：http://giv.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://wlf.jinqigufen.top

val m = mapOf("a" to 1)
来源：http://cvc.jinqigufen.top

[T14] Kotlin：循环
来源：http://dkr.cheryme.top

for (i in 1..10) println(i)
来源：http://dwx.chenlongwang.top

[T15] Kotlin：接口
来源：http://ukz.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://lho.yj202588.top

[T16] Swift：Hello World
来源：http://jvv.bjfxy.top

print("Hello")
来源：http://zzl.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://sqy.nwbrower.top

var a = 1;  let b = 2
来源：http://wwu.vehdjk.com

[T18] Swift：字符串插值
来源：http://ssm.dashuyun.cn

"值: \(b)"
来源：http://vdn.sysykeji.top

[T19] Swift：可选绑定
来源：http://wbc.andypj.xyz

if let n = opt { print(n) }
来源：http://urx.pengpengdd.cyou

[T20] Swift：数组操作
来源：http://bjx.dianchejie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://exv.hfpthk.cn

[T21] Swift：遍历
来源：http://gat.jqgufenzy.top

for x in a { print(x) }
来源：http://zig.guannengcc.top

[T22] Swift：字典
来源：http://qsp.ppjwa.cn

var d = ["a": 1];  d["b"] = 2
来源：http://reo.yj202588.top

[T23] Swift：函数
来源：http://use.fanxiaobao.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rxm.yfazqb.com

[T24] Swift：闭包
来源：http://zrr.ehwqpu.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://rke.epnwcf.com

[T25] Swift：结构体
来源：http://vfd.wangdashe.top

struct P { var x: Int }
来源：http://mrr.jyoumei.cn

[T26] Swift：类与重写
来源：http://ery.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://itq.chenjidiqi.icu

[T27] Swift：错误处理
来源：http://sfj.guowangkeji.top

do { try f() } catch { print(error) }
来源：http://isf.yvedp.cn

[T28] Swift：枚举
来源：http://joi.guowangkeji.top

enum Color { case red, green }
来源：http://efi.jiagoushi.top

[T29] Swift：guard 提前返回
来源：http://shd.yueranfly.top

guard let x = opt else { return }
来源：http://yoi.jyoumei.cn

[T30] Swift：协议
来源：http://gcl.jinyuanbaomall.cn

protocol Shape { func area() -> Double }
来源：http://tfh.316326.xyz

[T31] Lua：Hello World
来源：http://xii.hysaishi.cn

print("Hello")
来源：http://hyo.xuanzx.com

[T32] Lua：局部变量
来源：http://xkl.hnqzz.top

local a = 1
来源：http://rya.9152youxi.cn

[T33] Lua：表（数组）
来源：http://cts.hnxiangtu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lzf.zhongyouzk.top

[T34] Lua：遍历表
来源：http://exj.nanxuanxn.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ssf.ppjwa.cn

[T35] Lua：字典表
来源：http://nlg.dashuyun.cn

local d = { a = 1 };  d.b = 2
来源：http://jnz.cdnleiting.top

[T36] Lua：函数
来源：http://tzt.epnwcf.com

function add(a, b) return a + b end
来源：http://otj.mhx1999.top

[T37] Lua：字符串拼接
来源：http://hqq.jqgfzy.top

"a" .. "b"
来源：http://ggq.nwbrower.top

[T38] Lua：条件
来源：http://gse.sxryk.cn

if x > 0 then print("正") end
来源：http://brc.tian-w.cn

[T39] Lua：模式匹配
来源：http://kqo.nanxinkj.top

string.find(s, "%d+")
来源：http://kub.ivvv.top

[T40] Lua：元表
来源：http://zrj.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://gzl.bjfxy.top

[T41] Perl：Hello World
来源：http://vrn.shanyushiyangtech.top

print "Hello\n";
来源：http://qtm.yj20258888.top

[T42] Perl：变量类型
来源：http://fkf.hywenlv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ryo.52xcode.cn

[T43] Perl：字符串插值
来源：http://fim.zhoulong.xyz

"值: $a"
来源：http://viq.cashguo.top

[T44] Perl：条件
来源：http://fph.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://ukt.xingfuxueyuan.xyz

[T45] Perl：数组遍历
来源：http://emk.hammf.cn

for my $x (@arr) { print $x; }
来源：http://eex.zhaomingkeji.xyz

[T46] Perl：哈希操作
来源：http://qnu.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://djq.zdqjudy.top

[T47] Perl：正则捕获
来源：http://kur.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cec.guannengcc.top

[T48] Perl：正则替换
来源：http://ypu.yj20258888.top

$s =~ s/old/new/g;
来源：http://adk.uphjek.com

[T49] Perl：函数
来源：http://iwx.tian-w.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://omz.yuanzhike.top

[T50] Perl：逐行读文件
来源：http://irb.zhiwuduotai.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gwu.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://uah.yuxming.cn

[T51] Scala：Hello World
来源：http://msy.gaohongyu789.top

println("Hello")
来源：http://fxo.vqdsnc.cn

[T52] Scala：变量
来源：http://lmx.smart0.xyz

val a = 1;  var b = 2
来源：http://xla.cucudq.cn

[T53] Scala：字符串插值
来源：http://cyh.nwbrower.top

s"值: $b"
来源：http://cqi.sufxvd.cn

[T54] Scala：集合映射
来源：http://tyc.ydjk.org.cn

List(1, 2, 3).map(_ * 2)
来源：http://pib.daxiang520.top

[T55] Scala：集合过滤
来源：http://hdr.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://kca.xylfe.cn

[T56] Scala：样例类
来源：http://zdj.ehwqpu.com

case class User(name: String, age: Int)
来源：http://oxg.hesvh.cn

[T57] Scala：模式匹配
来源：http://lii.xuetiantiany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hrl.tian-w.cn

[T58] Scala：函数定义
来源：http://qki.snrcjt.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qqw.hnqzz.top

[T59] Scala：循环
来源：http://iyn.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://rdz.kuanghao11.cn

[T60] Scala：折叠
来源：http://dcl.fanxiaobao.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kur.jianghu66.top

================================================================================
来源：http://bkl.9152youxi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mpz.jinghuilouyu.cn

================================================================================
来源：http://xyv.chenlongwang.top

[U01] Py：创建虚拟环境
来源：http://btx.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://dse.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://zqm.ydjk.org.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gwy.yuanzhike.top

[U03] Py：加载 .env 配置
来源：http://rtm.dianchejie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uca.birdmap.top

[U04] Py：变量调试打印
来源：http://ufn.nanxuanxn.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lvs.yj20258888.top

[U05] Py：列表去重且保序
来源：http://unu.gzhubu.top

list(dict.fromkeys(arr))
来源：http://ppz.chenjidiqi.icu

[U06] Py：合并两个字典
来源：http://pfk.jiagoushi.top

{**a, **b}
来源：http://qyb.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://agi.zhengqikj.top

{v: k for k, v in d.items()}
来源：http://nqz.kuanghao11.cn

[U08] Py：展平二维列表
来源：http://cri.pycfn.com

[y for x in nested for y in x]
来源：http://ctk.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://owl.zhixingplan.top

max(d, key=d.get)
来源：http://xus.cheryme.top

[U10] Py：按值排序字典
来源：http://rkg.zhoulong.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ehs.cqqwz.cn

[U11] Py：生成器表达式
来源：http://hcq.hammf.cn

(x * 2 for x in arr)
来源：http://dsw.jinghuilouyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xow.yfazqb.com

Counter(arr).most_common(3)
来源：http://ask.c1oappe.top

[U13] Py：固定长度队列
来源：http://mbb.quarkkingdee.top

deque(maxlen=10)
来源：http://rat.zdbjq.cn

[U14] Py：分组收集到列表
来源：http://usm.9152youxi.cn

defaultdict(list)
来源：http://fwm.shanyushiyangkeji.top

[U15] Py：高精度计时
来源：http://akq.yj20258.top

t = time.perf_counter()
来源：http://yle.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://kwu.tian-w.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://okt.316326.xyz

[U17] Py：初始化日志
来源：http://bmz.ctjpmb.com

logging.basicConfig(level=logging.INFO)
来源：http://cnh.jiagoushi.top

[U18] Py：预编译正则
来源：http://cem.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://zmj.yj202588.top

[U19] Py：正则替换带回调
来源：http://slm.fktsv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hqj.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://nfg.tian-w.cn

@functools.lru_cache(maxsize=None)
来源：http://bgu.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://fmq.ppjwa.cn

@contextlib.contextmanager
来源：http://qmr.shuidangran.top

[U22] Py：矩阵转置
来源：http://iff.gotoacloud.top

list(zip(*m))
来源：http://xry.xylfe.cn

[U23] Py：分块读取大文件
来源：http://fhr.chenlongwang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tgg.quarkkingdee.top

[U24] Py：路径操作
来源：http://mah.pycfn.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hyc.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://olm.shanyushiyangtech.top

csv.DictReader(f)
来源：http://tjt.snrcjt.cn

[U26] Py：并发下载
来源：http://luc.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mje.yangfankeji.com

[U27] Py：异步 HTTP
来源：http://cet.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://tvj.pengpengdd.cyou

[U28] Py：类型别名
来源：http://gjg.yj20258888.top

UserId = int
来源：http://twp.zycfv.cn

[U29] Py：属性校验
来源：http://wsy.zdqjudy.top

@property 与 @x.setter 配合
来源：http://toc.jyoumei.cn

[U30] Py：数据类
来源：http://sld.bbcook.cn

@dataclass(slots=True)
来源：http://zsb.vehdjk.com

[U31] Py：单测
来源：http://ezo.kuanghao11.cn

python -m pytest -q
来源：http://ywf.jiagoushi.top

[U32] Py：代码格式化
来源：http://vii.cdnleiting.top

ruff format . && ruff check --fix .
来源：http://yes.yj20258888.top

[U33] Py：打包发布
来源：http://wpw.zhengqikj.top

python -m build  （依赖 pyproject.toml）
来源：http://eql.hywenlv.cn

[U34] Py：判断编码
来源：http://zfp.bbcook.cn

chardet.detect(raw)
来源：http://yws.vehdjk.com

[U35] Py：发送邮件
来源：http://ryd.shangyingyoupin.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rzo.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://hjo.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://oxq.pengpengdd.cyou

[U37] Py：读写 Excel
来源：http://yfb.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eyy.sweek.top

[U38] Py：获取脚本所在目录
来源：http://anj.hysaishi.cn

Path(__file__).resolve().parent
来源：http://qgb.cdnleiting.top

[U39] Py：判断是否在交互环境
来源：http://pto.xuanzx.com

sys.stdout.isatty()
来源：http://djk.jqgufenzy.top

[U40] Py：打印到标准错误
来源：http://nsi.fehbvm.com

print("err", file=sys.stderr)
来源：http://oyk.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://xdf.hysaishi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bct.xinyue.icu

[U42] PHP：PSR-4 自动加载
来源：http://ntm.ybcxt.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gxd.xinyue.icu

[U43] PHP：声明命名空间
来源：http://ejg.shangyingyoupin.top

namespace App\Http;
来源：http://rbc.pycfn.com

[U44] PHP：开启严格类型
来源：http://sut.hesvh.cn

declare(strict_types=1);
来源：http://kwa.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://wxc.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nbm.shuidangran.top

[U46] PHP：可空类型
来源：http://uun.jinqigfzy.top

?string $name = null
来源：http://yuv.yuxming.cn

[U47] PHP：联合类型
来源：http://rsq.0kj1m.cn

int|string $id
来源：http://kkf.hammf.cn

[U48] PHP：纯枚举
来源：http://pos.c1oappe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://utz.gogol.net.cn

[U49] PHP：只读属性
来源：http://bqr.shanyushiyangkeji.top

public readonly string $name
来源：http://ieg.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://nuu.haohaochexian.top

public function __construct(private int $id) {}
来源：http://lci.fktsv.cn

[U51] PHP：数组解构
来源：http://mkb.dianchejie.cn

[$a, $b] = $arr;
来源：http://dwx.chenjidiqi.icu

[U52] PHP：箭头函数
来源：http://quh.andypj.xyz

$double = fn($x) => $x * 2;
来源：http://vjs.guowangkeji.top

[U53] PHP：空合并运算符
来源：http://byf.gogol.net.cn

$v = $a ?? $b ?? "default";
来源：http://hku.hammf.cn

[U54] PHP：空安全调用
来源：http://lbv.jinqigfzy.top

$obj?->method()
来源：http://lfs.jianghu66.top

[U55] PHP：match 表达式
来源：http://ubb.ctjpmb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qak.zhiwuduotai.top

[U56] PHP：命名参数
来源：http://mug.guannengcc.top

f(a: 1, b: 2)
来源：http://wzw.yvedp.cn

[U57] PHP：字符串插值
来源：http://aao.fehbvm.com

"值: {$a}"
来源：http://doz.gzhubu.top

[U58] PHP：数组三件套
来源：http://nel.yongpay.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jum.hnqzz.top

[U59] PHP：自定义排序
来源：http://bdw.yanxiufei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sjj.snrcjt.cn

[U60] PHP：JSON 编解码
来源：http://hfw.hfpthk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sex.dianchejie.cn

[U61] PHP：正则
来源：http://ilj.jlsjyb.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kpy.chenlongwang.top

[U62] PHP：日期对象
来源：http://gfa.9152youxi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tka.hammf.cn

[U63] PHP：文件读写
来源：http://wkz.0kj1m.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xsa.snrcjt.cn

[U64] PHP：目录遍历
来源：http://nkr.redwolf501.top

glob("dir/*.php");  scandir("dir");
来源：http://zps.gogol.net.cn

[U65] PHP：会话
来源：http://rnm.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rvo.ivvv.top

[U66] PHP：设置 Cookie
来源：http://mrb.meibo888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lvl.shanyushiyangkeji.top

[U67] PHP：处理文件上传
来源：http://fwk.wangshuangyany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pmo.hnxiangtu.top

[U68] PHP：PDO 连接
来源：http://dfm.yueranfly.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://voq.ivvv.top

[U69] PHP：PDO 预处理
来源：http://ynh.yj20258.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tzg.gotoacloud.top

[U70] PHP：PDO 事务
来源：http://ars.jlsjyb.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ecb.nwbrower.top

[U71] PHP：抛出异常
来源：http://mzn.daria6918.cn

throw new RuntimeException("失败", 500);
来源：http://wdr.hfpthk.cn

[U72] PHP：写错误日志
来源：http://cvj.c1oappe.top

error_log("失败: " . $e->getMessage());
来源：http://hle.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://sgs.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://rnc.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://jxq.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://rso.c1oappe.top


<!-- 参考信息 -->