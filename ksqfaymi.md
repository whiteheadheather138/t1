代发 wailian999

while (std::getline(in, line)) { }
来源：http://tgq.ivvv.top

[S49] C++：写文件
来源：http://hln.ehwqpu.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bdp.aizwys.cn

[S50] C++：格式化数字
来源：http://jax.chenlongwang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tvc.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://zdn.jqgfzy.top

static_cast<double>(a) / b
来源：http://avi.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://zvu.tian-w.cn

int size() const noexcept { return n_; }
来源：http://mhu.feifeiyinyue.top

[S53] C++：移动语义
来源：http://jkv.hesvh.cn

std::vector<int> w = std::move(v);
来源：http://xjf.yongpay.top

[S54] C++：异常处理
来源：http://mht.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://khr.uphjek.com

[S55] C++：结构化绑定
来源：http://cex.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vqh.cqqwz.cn

[S56] C++：optional
来源：http://ciu.yueranfly.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dbq.epnwcf.com

[S57] C++：编译期常量
来源：http://ttc.zycfv.cn

constexpr int N = 10;
来源：http://jtx.yangfankeji.com

[S58] C++：命名空间
来源：http://fea.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://tjw.zhixingplan.top

[S59] C++：静态断言
来源：http://dhl.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uun.yuxming.cn

[S60] C++：遍历并删除元素
来源：http://kwr.yanxiufei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uqk.zdbjq.cn

================================================================================
来源：http://zgn.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jdk.meibo888.top

================================================================================
来源：http://abu.ybcxt.top

[T01] Kotlin：Hello World
来源：http://rfk.iojbl.cn

println("Hello")
来源：http://rjw.guowangkeji.top

[T02] Kotlin：变量
来源：http://uxl.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jiv.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://gic.hnqzz.top

"值: $b"
来源：http://mfs.aibaodan.cn

[T04] Kotlin：空安全
来源：http://xol.xinyue.icu

val n: String? = null;  n?.length
来源：http://leh.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://utm.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vwj.hnqzz.top

[T06] Kotlin：集合映射
来源：http://tkg.xingfuxueyuan.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://qge.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://ccn.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cug.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://ary.hnqzz.top

data class User(val name: String, val age: Int)
来源：http://wvt.gaohongyu789.top

[T09] Kotlin：扩展函数
来源：http://ura.havefunace.top

fun String.exclaim() = this + "!"
来源：http://fbp.52xcode.cn

[T10] Kotlin：默认参数
来源：http://ssc.yj20258.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tvy.ppjwa.cn

[T11] Kotlin：协程
来源：http://ofo.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ums.jianghu66.top

[T12] Kotlin：解构声明
来源：http://qwj.yanxiufei.cn

val (a, b) = Pair(1, 2)
来源：http://utx.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://yrp.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://mpk.haohaochexian.top

[T14] Kotlin：循环
来源：http://vso.xylfe.cn

for (i in 1..10) println(i)
来源：http://phy.gzhubu.top

[T15] Kotlin：接口
来源：http://kgr.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://iro.haohaochexian.top

[T16] Swift：Hello World
来源：http://jil.quarkkingdee.top

print("Hello")
来源：http://ihj.jiagoushi.top

[T17] Swift：变量与常量
来源：http://edz.ydzc1.top

var a = 1;  let b = 2
来源：http://uno.fehbvm.com

[T18] Swift：字符串插值
来源：http://cet.shzxlz.cn

"值: \(b)"
来源：http://zmw.shuidangran.top

[T19] Swift：可选绑定
来源：http://iws.hysaishi.cn

if let n = opt { print(n) }
来源：http://utg.jlsjyb.cn

[T20] Swift：数组操作
来源：http://fhm.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://kkr.smart0.xyz

[T21] Swift：遍历
来源：http://pke.pycfn.com

for x in a { print(x) }
来源：http://srv.yvedp.cn

[T22] Swift：字典
来源：http://qlb.tanke756.top

var d = ["a": 1];  d["b"] = 2
来源：http://xnh.guannengcc.top

[T23] Swift：函数
来源：http://kgz.nanxinkj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://frt.bbcook.cn

[T24] Swift：闭包
来源：http://toc.nanxinkj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://waf.gaohongyu789.top

[T25] Swift：结构体
来源：http://xcj.uphjek.com

struct P { var x: Int }
来源：http://xau.c1oappe.top

[T26] Swift：类与重写
来源：http://lwv.dianchejie.cn

class A: Base { override func f() {} }
来源：http://sek.sufxvd.cn

[T27] Swift：错误处理
来源：http://urp.ivvv.top

do { try f() } catch { print(error) }
来源：http://cjs.gzhubu.top

[T28] Swift：枚举
来源：http://zxf.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://hbg.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://wow.havefunace.top

guard let x = opt else { return }
来源：http://qvb.wangshuangyany.cn

[T30] Swift：协议
来源：http://cej.fanxiaobao.xyz

protocol Shape { func area() -> Double }
来源：http://zny.shzxlz.cn

[T31] Lua：Hello World
来源：http://fnm.yueranfly.top

print("Hello")
来源：http://zxv.svipenyu.cn

[T32] Lua：局部变量
来源：http://dan.zhijiandao.cn

local a = 1
来源：http://nia.vqdsnc.cn

[T33] Lua：表（数组）
来源：http://mkp.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uzd.hysaishi.cn

[T34] Lua：遍历表
来源：http://evu.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zfx.hywenlv.cn

[T35] Lua：字典表
来源：http://kbr.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://agu.ppjwa.cn

[T36] Lua：函数
来源：http://bza.chenlongwang.top

function add(a, b) return a + b end
来源：http://phk.tanke756.top

[T37] Lua：字符串拼接
来源：http://knk.iojbl.cn

"a" .. "b"
来源：http://ova.ehwqpu.com

[T38] Lua：条件
来源：http://mgi.snrcjt.cn

if x > 0 then print("正") end
来源：http://mpa.bjfxy.top

[T39] Lua：模式匹配
来源：http://ifi.kuanghao11.cn

string.find(s, "%d+")
来源：http://tvt.xuetiantiany.cn

[T40] Lua：元表
来源：http://srl.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://xzx.bbcook.cn

[T41] Perl：Hello World
来源：http://hby.daria6918.cn

print "Hello\n";
来源：http://cue.hnxiangtu.top

[T42] Perl：变量类型
来源：http://gox.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wuz.zdbjq.cn

[T43] Perl：字符串插值
来源：http://cyl.yangfankeji.com

"值: $a"
来源：http://dvh.cashguo.top

[T44] Perl：条件
来源：http://tcy.pycfn.com

if ($a > 0) { print "正"; }
来源：http://zoo.andypj.xyz

[T45] Perl：数组遍历
来源：http://ogh.sysykeji.top

for my $x (@arr) { print $x; }
来源：http://niv.wangdashe.top

[T46] Perl：哈希操作
来源：http://mwy.jinghuilouyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cox.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://ilv.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kgd.yangfankeji.com

[T48] Perl：正则替换
来源：http://gyc.ydjk.org.cn

$s =~ s/old/new/g;
来源：http://xhn.yangfankeji.com

[T49] Perl：函数
来源：http://bvb.ydzc1.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fmv.hysaishi.cn

[T50] Perl：逐行读文件
来源：http://gfi.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cvw.snrcjt.cn

while (my $line = <$fh>) { print $line; }
来源：http://zfs.nanxinkj.top

[T51] Scala：Hello World
来源：http://kcf.shzxlz.cn

println("Hello")
来源：http://zrm.xziqi.cn

[T52] Scala：变量
来源：http://ryv.vqdsnc.cn

val a = 1;  var b = 2
来源：http://nzc.mhx1999.top

[T53] Scala：字符串插值
来源：http://cjf.andypj.xyz

s"值: $b"
来源：http://tob.cucudq.cn

[T54] Scala：集合映射
来源：http://vyt.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://ury.yangfankeji.com

[T55] Scala：集合过滤
来源：http://ymz.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://awb.shzxlz.cn

[T56] Scala：样例类
来源：http://wbm.zdqjudy.top

case class User(name: String, age: Int)
来源：http://jly.cashguo.top

[T57] Scala：模式匹配
来源：http://tro.zhoulong.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://qbu.jqgfzy.top

[T58] Scala：函数定义
来源：http://khx.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://iaw.vqdsnc.cn

[T59] Scala：循环
来源：http://jqt.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://kke.dianchejie.cn

[T60] Scala：折叠
来源：http://ykw.fktsv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mgv.yfazqb.com

================================================================================
来源：http://lbf.pengpengdd.cyou

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bil.ywan-chungtsiang.top

================================================================================
来源：http://pki.ivvv.top

[U01] Py：创建虚拟环境
来源：http://bub.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cgf.fzhhl.top

[U02] Py：导出 / 安装依赖
来源：http://sms.jqgfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://prf.yj20258.top

[U03] Py：加载 .env 配置
来源：http://fsp.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mwv.haohaochexian.top

[U04] Py：变量调试打印
来源：http://elb.redwolf501.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wnb.c1oappe.top

[U05] Py：列表去重且保序
来源：http://qgz.yongpay.top

list(dict.fromkeys(arr))
来源：http://ppt.tarul.cn

[U06] Py：合并两个字典
来源：http://bcy.jinghuilouyu.cn

{**a, **b}
来源：http://yfo.daria6918.cn

[U07] Py：反转字典键值
来源：http://mlq.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://gzc.0kj1m.cn

[U08] Py：展平二维列表
来源：http://aul.daxiang520.top

[y for x in nested for y in x]
来源：http://uro.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://rpc.dashuyun.cn

max(d, key=d.get)
来源：http://uag.wangdashe.top

[U10] Py：按值排序字典
来源：http://kym.quarkkingdee.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vdh.gogol.net.cn

[U11] Py：生成器表达式
来源：http://npq.jinqigfzy.top

(x * 2 for x in arr)
来源：http://gtd.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://upw.shangyingyoupin.top

Counter(arr).most_common(3)
来源：http://tyv.jinghuilouyu.cn

[U13] Py：固定长度队列
来源：http://thk.jinghuilouyu.cn

deque(maxlen=10)
来源：http://wui.aizwys.cn

[U14] Py：分组收集到列表
来源：http://wae.redwolf501.top

defaultdict(list)
来源：http://mnd.yuanzhike.top

[U15] Py：高精度计时
来源：http://oqq.yj202588.top

t = time.perf_counter()
来源：http://fzi.cheryme.top

[U16] Py：命令行参数解析
来源：http://ytm.vqdsnc.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wea.redwolf501.top

[U17] Py：初始化日志
来源：http://xzl.jianghu66.top

logging.basicConfig(level=logging.INFO)
来源：http://ffr.mhx1999.top

[U18] Py：预编译正则
来源：http://oxf.zhiwuduotai.top

pat = re.compile(r"\d+")
来源：http://cdi.shanyushiyangkeji.top

[U19] Py：正则替换带回调
来源：http://nxw.yuanzhike.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://diu.kuanghao11.cn

[U20] Py：缓存函数结果
来源：http://xce.haohaochexian.top

@functools.lru_cache(maxsize=None)
来源：http://ksc.yongpay.top

[U21] Py：自定义上下文管理器
来源：http://oaf.xuetiantiany.cn

@contextlib.contextmanager
来源：http://arf.xziqi.cn

[U22] Py：矩阵转置
来源：http://wgw.zdbjq.cn

list(zip(*m))
来源：http://bew.zhijiandao.cn

[U23] Py：分块读取大文件
来源：http://mcb.meibo888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ehz.yonumen.top

[U24] Py：路径操作
来源：http://jpk.yangfankeji.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://exa.zhongyouzk.top

[U25] Py：CSV 按字典读
来源：http://wpj.havefunace.top

csv.DictReader(f)
来源：http://tli.jlsjyb.cn

[U26] Py：并发下载
来源：http://zhm.9152youxi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gqc.havefunace.top

[U27] Py：异步 HTTP
来源：http://cbv.yanxiufei.cn

aiohttp.ClientSession() 配合 async with
来源：http://xiu.shangyingyoupin.top

[U28] Py：类型别名
来源：http://rod.birdmap.top

UserId = int
来源：http://gii.jqgfzy.top

[U29] Py：属性校验
来源：http://gpu.mhx1999.top

@property 与 @x.setter 配合
来源：http://tgj.nwbrower.top

[U30] Py：数据类
来源：http://frd.daria6918.cn

@dataclass(slots=True)
来源：http://ucm.cheryme.top

[U31] Py：单测
来源：http://mbo.tianlin.xyz

python -m pytest -q
来源：http://kec.c1oappe.top

[U32] Py：代码格式化
来源：http://iea.pycfn.com

ruff format . && ruff check --fix .
来源：http://yky.quarkkingdee.top

[U33] Py：打包发布
来源：http://xpq.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://pbn.zdqjudy.top

[U34] Py：判断编码
来源：http://oya.yfazqb.com

chardet.detect(raw)
来源：http://wby.fanxiaobao.xyz

[U35] Py：发送邮件
来源：http://kau.guannengcc.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xyz.yonumen.top

[U36] Py：定时任务
来源：http://roh.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://qok.yfazqb.com

[U37] Py：读写 Excel
来源：http://chh.fengsongda.top

pandas.read_excel / DataFrame.to_excel
来源：http://mfh.haohaochexian.top

[U38] Py：获取脚本所在目录
来源：http://pba.shanyushiyangtech.top

Path(__file__).resolve().parent
来源：http://ofn.sufxvd.cn

[U39] Py：判断是否在交互环境
来源：http://vwa.yanxiufei.cn

sys.stdout.isatty()
来源：http://fij.jqgfzy.top

[U40] Py：打印到标准错误
来源：http://vyb.ehwqpu.com

print("err", file=sys.stderr)
来源：http://ihr.jqgfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://ble.52xcode.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://toa.quarkkingdee.top

[U42] PHP：PSR-4 自动加载
来源：http://eeg.xingfuxueyuan.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nyl.xinyue.icu

[U43] PHP：声明命名空间
来源：http://qic.aizwys.cn

namespace App\Http;
来源：http://pkc.52xcode.cn

[U44] PHP：开启严格类型
来源：http://qhw.wangdashe.top

declare(strict_types=1);
来源：http://puu.hnqzz.top

[U45] PHP：类型声明与返回类型
来源：http://azi.hywenlv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://asi.yj20258.top

[U46] PHP：可空类型
来源：http://ojn.hysaishi.cn

?string $name = null
来源：http://xdp.tian-w.cn

[U47] PHP：联合类型
来源：http://tmw.hywenlv.cn

int|string $id
来源：http://yfm.epnwcf.com

[U48] PHP：纯枚举
来源：http://smp.zhijiandao.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pyb.shanyushiyangkeji.top

[U49] PHP：只读属性
来源：http://cmg.ivvv.top

public readonly string $name
来源：http://oqw.fehbvm.com

[U50] PHP：构造器属性提升
来源：http://xnb.sxryk.cn

public function __construct(private int $id) {}
来源：http://ltr.zhijiandao.cn

[U51] PHP：数组解构
来源：http://iqo.zhixingplan.top

[$a, $b] = $arr;
来源：http://nmj.yfazqb.com

[U52] PHP：箭头函数
来源：http://nmm.hysaishi.cn

$double = fn($x) => $x * 2;
来源：http://ssh.zdbjq.cn

[U53] PHP：空合并运算符
来源：http://eby.ydjk.org.cn

$v = $a ?? $b ?? "default";
来源：http://jen.sjlbkw.cn

[U54] PHP：空安全调用
来源：http://cum.shuidangran.top

$obj?->method()
来源：http://kuz.zdbjq.cn

[U55] PHP：match 表达式
来源：http://kfh.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jto.xylfe.cn

[U56] PHP：命名参数
来源：http://qcl.cdnleiting.top

f(a: 1, b: 2)
来源：http://usa.daxiang520.top

[U57] PHP：字符串插值
来源：http://ean.gzhubu.top

"值: {$a}"
来源：http://lcs.sufxvd.cn

[U58] PHP：数组三件套
来源：http://hye.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://osk.pengpengdd.cyou

[U59] PHP：自定义排序
来源：http://mjp.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wjk.zhongyouzk.top

[U60] PHP：JSON 编解码
来源：http://rgq.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tdz.wangshuangyany.cn

[U61] PHP：正则
来源：http://mrl.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://itz.epnwcf.com

[U62] PHP：日期对象
来源：http://kaa.jqgufenzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ycq.shzxlz.cn

[U63] PHP：文件读写
来源：http://ydv.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rcm.tanke756.top

[U64] PHP：目录遍历
来源：http://uzt.dianchejie.cn

glob("dir/*.php");  scandir("dir");
来源：http://woe.yj202588.top

[U65] PHP：会话
来源：http://gwf.hcnkem.com

session_start();  $_SESSION["uid"] = 1;
来源：http://cse.smart0.xyz

[U66] PHP：设置 Cookie
来源：http://axb.chenzaomai.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://por.jyoumei.cn

[U67] PHP：处理文件上传
来源：http://ifh.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hvq.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://tie.cucudq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://svj.daria6918.cn

[U69] PHP：PDO 预处理
来源：http://yye.chenzaomai.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bjn.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://zcb.havefunace.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ptw.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://jpm.hywenlv.cn

throw new RuntimeException("失败", 500);
来源：http://jvy.xinyue.icu

[U72] PHP：写错误日志
来源：http://rzp.chenzaomai.com

error_log("失败: " . $e->getMessage());
来源：http://fvr.ydzc1.top

[U73] PHP：读取 ini 配置
来源：http://fqq.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://rov.svipenyu.cn

[U74] PHP：读取环境变量
来源：http://mlt.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://isx.hcnkem.com


<!-- 参考信息 -->