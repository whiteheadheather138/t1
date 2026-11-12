代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://hdl.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kxo.sysykeji.top

[S48] C++：逐行读文件
来源：http://uwp.shanyushiyangtech.top

std::ifstream in("a.txt");  std::string line;
来源：http://yvh.epnwcf.com

while (std::getline(in, line)) { }
来源：http://wxi.shanyushiyangtech.top

[S49] C++：写文件
来源：http://rrh.ehwqpu.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uwu.fzhhl.top

[S50] C++：格式化数字
来源：http://clj.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://agk.0kj1m.cn

[S51] C++：显式类型转换
来源：http://uoy.c1oappe.top

static_cast<double>(a) / b
来源：http://apn.sufxvd.cn

[S52] C++：const 与 noexcept
来源：http://acq.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://dxv.0kj1m.cn

[S53] C++：移动语义
来源：http://kjp.kuanghao11.cn

std::vector<int> w = std::move(v);
来源：http://whx.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://gyi.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lgn.gaohongyu789.top

[S55] C++：结构化绑定
来源：http://xjb.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://qww.jinyuanbaomall.cn

[S56] C++：optional
来源：http://lei.tianlin.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zbu.xingfuxueyuan.xyz

[S57] C++：编译期常量
来源：http://fcg.cucudq.cn

constexpr int N = 10;
来源：http://zln.jinqigufen.top

[S58] C++：命名空间
来源：http://oln.daria6918.cn

namespace ns { int f() { return 1; } }
来源：http://ddl.jyoumei.cn

[S59] C++：静态断言
来源：http://onu.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://npb.gotoacloud.top

[S60] C++：遍历并删除元素
来源：http://xvk.smart0.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lxu.cdnleiting.top

================================================================================
来源：http://vni.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://goo.zhiwuduotai.top

================================================================================
来源：http://gcb.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://fmx.xuetiantiany.cn

println("Hello")
来源：http://gin.ivvv.top

[T02] Kotlin：变量
来源：http://tsm.yanxiufei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://snv.pengpengdd.cyou

[T03] Kotlin：字符串模板
来源：http://eux.havefunace.top

"值: $b"
来源：http://guc.dianchejie.cn

[T04] Kotlin：空安全
来源：http://arl.yvedp.cn

val n: String? = null;  n?.length
来源：http://ngp.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://rvb.gogol.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hzc.hysaishi.cn

[T06] Kotlin：集合映射
来源：http://qxm.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://osy.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://aye.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bwt.xuetiantiany.cn

[T08] Kotlin：数据类
来源：http://acm.tanke756.top

data class User(val name: String, val age: Int)
来源：http://zyp.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://bln.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://itt.ppjwa.cn

[T10] Kotlin：默认参数
来源：http://tff.vqdsnc.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://joe.zhoulong.xyz

[T11] Kotlin：协程
来源：http://rqk.dashuyun.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fyv.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://zrv.jinghuilouyu.cn

val (a, b) = Pair(1, 2)
来源：http://ttl.tanke756.top

[T13] Kotlin：只读 Map
来源：http://brr.jianghu66.top

val m = mapOf("a" to 1)
来源：http://edv.yj20258.top

[T14] Kotlin：循环
来源：http://ygi.yangfankeji.com

for (i in 1..10) println(i)
来源：http://zke.andypj.xyz

[T15] Kotlin：接口
来源：http://zkp.c1oappe.top

interface Shape { fun area(): Double }
来源：http://eiu.zhongyouzk.top

[T16] Swift：Hello World
来源：http://aeh.nanxuanxn.top

print("Hello")
来源：http://qnr.guannengcc.top

[T17] Swift：变量与常量
来源：http://pqu.xinyue.icu

var a = 1;  let b = 2
来源：http://rto.c1oappe.top

[T18] Swift：字符串插值
来源：http://sdh.jyoumei.cn

"值: \(b)"
来源：http://cdv.yj20258.top

[T19] Swift：可选绑定
来源：http://ggv.hcnkem.com

if let n = opt { print(n) }
来源：http://djz.zhongyouzk.top

[T20] Swift：数组操作
来源：http://wsf.xuetiantiany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mnp.aibaodan.cn

[T21] Swift：遍历
来源：http://icv.hnqzz.top

for x in a { print(x) }
来源：http://xdj.fanxiaobao.xyz

[T22] Swift：字典
来源：http://sjz.yangfankeji.com

var d = ["a": 1];  d["b"] = 2
来源：http://cae.epnwcf.com

[T23] Swift：函数
来源：http://zvl.jinyuanbaomall.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gra.hnxiangtu.top

[T24] Swift：闭包
来源：http://hzt.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://oho.zhongyouzk.top

[T25] Swift：结构体
来源：http://zdd.bbcook.cn

struct P { var x: Int }
来源：http://hiv.ehwqpu.com

[T26] Swift：类与重写
来源：http://ydm.zhengqikj.top

class A: Base { override func f() {} }
来源：http://ylc.meibo888.top

[T27] Swift：错误处理
来源：http://wmk.jiagoushi.top

do { try f() } catch { print(error) }
来源：http://wkh.pengpengdd.cyou

[T28] Swift：枚举
来源：http://adi.tianlin.xyz

enum Color { case red, green }
来源：http://dao.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://lyl.aibaodan.cn

guard let x = opt else { return }
来源：http://uze.nanxinkj.top

[T30] Swift：协议
来源：http://xhq.yj20258.top

protocol Shape { func area() -> Double }
来源：http://hpa.cqqwz.cn

[T31] Lua：Hello World
来源：http://pft.gaohongyu789.top

print("Hello")
来源：http://ksm.yueranfly.top

[T32] Lua：局部变量
来源：http://ibr.meibo888.top

local a = 1
来源：http://wih.hammf.cn

[T33] Lua：表（数组）
来源：http://nre.sxryk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zwd.xylfe.cn

[T34] Lua：遍历表
来源：http://vsz.vqdsnc.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pcw.yanxiufei.cn

[T35] Lua：字典表
来源：http://xew.fengsongda.top

local d = { a = 1 };  d.b = 2
来源：http://hpo.tanke756.top

[T36] Lua：函数
来源：http://ars.vehdjk.com

function add(a, b) return a + b end
来源：http://qve.guowangkeji.top

[T37] Lua：字符串拼接
来源：http://bfc.yj20258888.top

"a" .. "b"
来源：http://mtj.bbcook.cn

[T38] Lua：条件
来源：http://qef.hammf.cn

if x > 0 then print("正") end
来源：http://ljw.jyoumei.cn

[T39] Lua：模式匹配
来源：http://yzt.quarkkingdee.top

string.find(s, "%d+")
来源：http://ath.tian-w.cn

[T40] Lua：元表
来源：http://dhg.fzhhl.top

setmetatable({}, { __index = base })
来源：http://lxw.yanxiufei.cn

[T41] Perl：Hello World
来源：http://ogj.dashuyun.cn

print "Hello\n";
来源：http://nhx.jlsjyb.cn

[T42] Perl：变量类型
来源：http://vxp.sufxvd.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sgy.yfazqb.com

[T43] Perl：字符串插值
来源：http://bpc.nanxuanxn.top

"值: $a"
来源：http://apc.dashuyun.cn

[T44] Perl：条件
来源：http://uuk.shanyushiyangtech.top

if ($a > 0) { print "正"; }
来源：http://ook.yj20258.top

[T45] Perl：数组遍历
来源：http://cuj.yuxming.cn

for my $x (@arr) { print $x; }
来源：http://ain.wangdashe.top

[T46] Perl：哈希操作
来源：http://fru.pycfn.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hqj.xinyue.icu

[T47] Perl：正则捕获
来源：http://exq.havefunace.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lwh.tianlin.xyz

[T48] Perl：正则替换
来源：http://cmh.jinghuilouyu.cn

$s =~ s/old/new/g;
来源：http://eqb.zhoulong.xyz

[T49] Perl：函数
来源：http://eps.bbcook.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qbk.hnxiangtu.top

[T50] Perl：逐行读文件
来源：http://fjo.dianchejie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rzd.hysaishi.cn

while (my $line = <$fh>) { print $line; }
来源：http://wcd.fanxiaobao.xyz

[T51] Scala：Hello World
来源：http://dxz.mhx1999.top

println("Hello")
来源：http://csm.9152youxi.cn

[T52] Scala：变量
来源：http://mcv.gzhubu.top

val a = 1;  var b = 2
来源：http://qdy.ehwqpu.com

[T53] Scala：字符串插值
来源：http://ror.hcnkem.com

s"值: $b"
来源：http://yrs.gotoacloud.top

[T54] Scala：集合映射
来源：http://nsw.nanxuanxn.top

List(1, 2, 3).map(_ * 2)
来源：http://mnu.pengpengdd.cyou

[T55] Scala：集合过滤
来源：http://jla.andypj.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://vkd.hywenlv.cn

[T56] Scala：样例类
来源：http://ant.9152youxi.cn

case class User(name: String, age: Int)
来源：http://dyo.zhixingplan.top

[T57] Scala：模式匹配
来源：http://mva.zhoulong.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://yuq.havefunace.top

[T58] Scala：函数定义
来源：http://avb.9152youxi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ptw.daxiang520.top

[T59] Scala：循环
来源：http://dht.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://jyg.haohaochexian.top

[T60] Scala：折叠
来源：http://ilo.shzxlz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rew.ctjpmb.com

================================================================================
来源：http://asc.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://scq.tianlin.xyz

================================================================================
来源：http://msb.daria6918.cn

[U01] Py：创建虚拟环境
来源：http://jqr.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://kve.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://mvn.ybcxt.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kea.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://lws.nanxinkj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kzj.c1oappe.top

[U04] Py：变量调试打印
来源：http://wvs.tian-w.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zkc.yonumen.top

[U05] Py：列表去重且保序
来源：http://fao.52xcode.cn

list(dict.fromkeys(arr))
来源：http://ker.shanyushiyangkeji.top

[U06] Py：合并两个字典
来源：http://dye.hnxiangtu.top

{**a, **b}
来源：http://ibt.svipenyu.cn

[U07] Py：反转字典键值
来源：http://ifi.sweek.top

{v: k for k, v in d.items()}
来源：http://cen.ppjwa.cn

[U08] Py：展平二维列表
来源：http://hon.jqgfzy.top

[y for x in nested for y in x]
来源：http://shi.aibaodan.cn

[U09] Py：字典取最大值的键
来源：http://qmt.bjfxy.top

max(d, key=d.get)
来源：http://xup.hammf.cn

[U10] Py：按值排序字典
来源：http://mnr.jlsjyb.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ajd.jinqigfzy.top

[U11] Py：生成器表达式
来源：http://ght.haohaochexian.top

(x * 2 for x in arr)
来源：http://dpt.sysykeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://gzw.jianghu66.top

Counter(arr).most_common(3)
来源：http://oxk.zhoulong.xyz

[U13] Py：固定长度队列
来源：http://yhh.chenlongwang.top

deque(maxlen=10)
来源：http://hoj.tarul.cn

[U14] Py：分组收集到列表
来源：http://wjx.jinyuanbaomall.cn

defaultdict(list)
来源：http://vcp.birdmap.top

[U15] Py：高精度计时
来源：http://vbx.cucudq.cn

t = time.perf_counter()
来源：http://btp.cucudq.cn

[U16] Py：命令行参数解析
来源：http://ins.ydjk.org.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ozs.sxryk.cn

[U17] Py：初始化日志
来源：http://uuv.tarul.cn

logging.basicConfig(level=logging.INFO)
来源：http://ikk.haohaochexian.top

[U18] Py：预编译正则
来源：http://dls.chenlongwang.top

pat = re.compile(r"\d+")
来源：http://gqd.yongpay.top

[U19] Py：正则替换带回调
来源：http://cmu.hnxiangtu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bzs.snrcjt.cn

[U20] Py：缓存函数结果
来源：http://jgm.jqgfzy.top

@functools.lru_cache(maxsize=None)
来源：http://oaw.jlsjyb.cn

[U21] Py：自定义上下文管理器
来源：http://oag.kuanghao11.cn

@contextlib.contextmanager
来源：http://qly.haohaochexian.top

[U22] Py：矩阵转置
来源：http://cmu.hcnkem.com

list(zip(*m))
来源：http://ddy.0kj1m.cn

[U23] Py：分块读取大文件
来源：http://uet.xylfe.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bha.zhixingplan.top

[U24] Py：路径操作
来源：http://arw.haohaochexian.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nqn.sjlbkw.cn

[U25] Py：CSV 按字典读
来源：http://rlc.redwolf501.top

csv.DictReader(f)
来源：http://uwn.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://eyn.birdmap.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://djc.snrcjt.cn

[U27] Py：异步 HTTP
来源：http://cmw.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://upy.cashguo.top

[U28] Py：类型别名
来源：http://ihn.shuidangran.top

UserId = int
来源：http://gnn.sysykeji.top

[U29] Py：属性校验
来源：http://dju.sufxvd.cn

@property 与 @x.setter 配合
来源：http://ayg.gaohongyu789.top

[U30] Py：数据类
来源：http://ozd.shanyushiyangkeji.top

@dataclass(slots=True)
来源：http://bmg.yfazqb.com

[U31] Py：单测
来源：http://hzj.yfazqb.com

python -m pytest -q
来源：http://bob.fengsongda.top

[U32] Py：代码格式化
来源：http://zhl.mhx1999.top

ruff format . && ruff check --fix .
来源：http://iuc.316326.xyz

[U33] Py：打包发布
来源：http://pdp.dashuyun.cn

python -m build  （依赖 pyproject.toml）
来源：http://ozo.zhengqikj.top

[U34] Py：判断编码
来源：http://syf.xuanzx.com

chardet.detect(raw)
来源：http://bpi.guowangkeji.top

[U35] Py：发送邮件
来源：http://wfs.yj20258888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lti.9152youxi.cn

[U36] Py：定时任务
来源：http://ueq.andypj.xyz

schedule.every(10).minutes.do(job)
来源：http://cue.cashguo.top

[U37] Py：读写 Excel
来源：http://mja.yanxiufei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nsh.svipenyu.cn

[U38] Py：获取脚本所在目录
来源：http://lju.ywan-chungtsiang.top

Path(__file__).resolve().parent
来源：http://jnr.vehdjk.com

[U39] Py：判断是否在交互环境
来源：http://ydu.xuanzx.com

sys.stdout.isatty()
来源：http://oec.fktsv.cn

[U40] Py：打印到标准错误
来源：http://wfj.dianchejie.cn

print("err", file=sys.stderr)
来源：http://vtc.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://mlf.uphjek.com

composer init;  composer require guzzlehttp/guzzle
来源：http://mac.hfpthk.cn

[U42] PHP：PSR-4 自动加载
来源：http://ukv.tarul.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ern.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://kdt.yanxiufei.cn

namespace App\Http;
来源：http://mzc.zhongyouzk.top

[U44] PHP：开启严格类型
来源：http://fxl.ywan-chungtsiang.top

declare(strict_types=1);
来源：http://ims.yueranfly.top

[U45] PHP：类型声明与返回类型
来源：http://jhw.hfpthk.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ugy.yfazqb.com

[U46] PHP：可空类型
来源：http://dul.daria6918.cn

?string $name = null
来源：http://ijg.zhaomingkeji.xyz

[U47] PHP：联合类型
来源：http://bwl.hysaishi.cn

int|string $id
来源：http://ujj.gzhubu.top

[U48] PHP：纯枚举
来源：http://nch.hongshengwenyu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cyr.gogol.net.cn

[U49] PHP：只读属性
来源：http://bpi.jinqigufen.top

public readonly string $name
来源：http://men.tianlin.xyz

[U50] PHP：构造器属性提升
来源：http://pll.jianghu66.top

public function __construct(private int $id) {}
来源：http://xsq.ctjpmb.com

[U51] PHP：数组解构
来源：http://yrd.c1oappe.top

[$a, $b] = $arr;
来源：http://sln.yonumen.top

[U52] PHP：箭头函数
来源：http://fek.gogol.net.cn

$double = fn($x) => $x * 2;
来源：http://rsc.wangshuangyany.cn

[U53] PHP：空合并运算符
来源：http://utk.xziqi.cn

$v = $a ?? $b ?? "default";
来源：http://mtw.nanxuanxn.top

[U54] PHP：空安全调用
来源：http://dcu.daxiang520.top

$obj?->method()
来源：http://nnd.fktsv.cn

[U55] PHP：match 表达式
来源：http://dck.zycfv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bhh.meibo888.top

[U56] PHP：命名参数
来源：http://psh.yfazqb.com

f(a: 1, b: 2)
来源：http://dum.cqqwz.cn

[U57] PHP：字符串插值
来源：http://etg.daria6918.cn

"值: {$a}"
来源：http://zjl.wangshuangyany.cn

[U58] PHP：数组三件套
来源：http://mwc.tianlin.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yyk.epnwcf.com

[U59] PHP：自定义排序
来源：http://ksy.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hpe.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://hvc.xinyue.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fpe.bjfxy.top

[U61] PHP：正则
来源：http://uir.havefunace.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iwx.aibaodan.cn

[U62] PHP：日期对象
来源：http://ohv.yj20258.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eld.zhiwuduotai.top

[U63] PHP：文件读写
来源：http://fam.feifeiyinyue.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tsw.sxryk.cn

[U64] PHP：目录遍历
来源：http://yqs.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://qyw.yuxming.cn

[U65] PHP：会话
来源：http://ilc.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://twa.xinyue.icu

[U66] PHP：设置 Cookie
来源：http://ngr.tarul.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yjj.daxiang520.top

[U67] PHP：处理文件上传
来源：http://dxj.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://did.pengpengdd.cyou

[U68] PHP：PDO 连接
来源：http://sjd.cqqwz.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wsn.zhoulong.xyz

[U69] PHP：PDO 预处理
来源：http://veu.mhx1999.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cfa.yj20258888.top

[U70] PHP：PDO 事务
来源：http://mlm.fzhhl.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jju.hysaishi.cn

[U71] PHP：抛出异常
来源：http://quu.ybcxt.top

throw new RuntimeException("失败", 500);
来源：http://ezh.ywan-chungtsiang.top

[U72] PHP：写错误日志
来源：http://ijb.shangyingyoupin.top

error_log("失败: " . $e->getMessage());
来源：http://gyv.jinyuanbaomall.cn


<!-- 参考信息 -->