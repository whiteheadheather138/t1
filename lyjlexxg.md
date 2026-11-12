代发 wailian999

[S41] C++：类与构造函数
来源：http://ltd.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vev.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://tza.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://srv.svipenyu.cn

[S43] C++：智能指针
来源：http://crp.jianghu66.top

auto p = std::make_unique<int>(5);
来源：http://ljz.ehwqpu.com

[S44] C++：引用传参
来源：http://lte.andypj.xyz

void inc(int &x) { ++x; }
来源：http://pfu.smart0.xyz

[S45] C++：lambda
来源：http://srh.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ebz.316326.xyz

[S46] C++：函数模板
来源：http://efy.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lyh.mhx1999.top

[S47] C++：结构化绑定遍历
来源：http://sus.ydjk.org.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zat.gaohongyu789.top

[S48] C++：逐行读文件
来源：http://qhr.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://oln.havefunace.top

while (std::getline(in, line)) { }
来源：http://mxe.andypj.xyz

[S49] C++：写文件
来源：http://gpj.xylfe.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jok.xuanzx.com

[S50] C++：格式化数字
来源：http://elr.9152youxi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iuo.zycfv.cn

[S51] C++：显式类型转换
来源：http://gqg.hfpthk.cn

static_cast<double>(a) / b
来源：http://xmz.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://opk.52xcode.cn

int size() const noexcept { return n_; }
来源：http://lze.ydjk.org.cn

[S53] C++：移动语义
来源：http://kbi.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://yxm.pengpengdd.cyou

[S54] C++：异常处理
来源：http://kas.uphjek.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rur.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://gyq.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://dby.ybcxt.top

[S56] C++：optional
来源：http://pvu.hcnkem.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cfx.vqdsnc.cn

[S57] C++：编译期常量
来源：http://mlm.tian-w.cn

constexpr int N = 10;
来源：http://wxh.fehbvm.com

[S58] C++：命名空间
来源：http://ysy.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://vut.zhengqikj.top

[S59] C++：静态断言
来源：http://ceq.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ibq.xingfuxueyuan.xyz

[S60] C++：遍历并删除元素
来源：http://eqa.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://umm.andypj.xyz

================================================================================
来源：http://txk.nanxuanxn.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cai.ctjpmb.com

================================================================================
来源：http://rqj.yj20258.top

[T01] Kotlin：Hello World
来源：http://plq.tarul.cn

println("Hello")
来源：http://oei.9152youxi.cn

[T02] Kotlin：变量
来源：http://xng.dashuyun.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ybw.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://vei.tian-w.cn

"值: $b"
来源：http://von.uphjek.com

[T04] Kotlin：空安全
来源：http://dog.guannengcc.top

val n: String? = null;  n?.length
来源：http://cuq.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://sme.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eye.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://jtf.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mek.jinyuanbaomall.cn

[T07] Kotlin：集合过滤
来源：http://nlp.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://jnc.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://ycm.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://coi.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://vzr.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://aox.hfpthk.cn

[T10] Kotlin：默认参数
来源：http://ptd.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nob.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://vdk.sufxvd.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zxf.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://xwo.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://rae.0kj1m.cn

[T13] Kotlin：只读 Map
来源：http://sop.yueranfly.top

val m = mapOf("a" to 1)
来源：http://rbx.ppjwa.cn

[T14] Kotlin：循环
来源：http://qpd.quarkkingdee.top

for (i in 1..10) println(i)
来源：http://jaw.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://czk.fktsv.cn

interface Shape { fun area(): Double }
来源：http://lsg.zhixingplan.top

[T16] Swift：Hello World
来源：http://yyf.feifeiyinyue.top

print("Hello")
来源：http://hlb.zdbjq.cn

[T17] Swift：变量与常量
来源：http://tnd.gzhubu.top

var a = 1;  let b = 2
来源：http://aug.zhixingplan.top

[T18] Swift：字符串插值
来源：http://wco.iojbl.cn

"值: \(b)"
来源：http://dtx.andypj.xyz

[T19] Swift：可选绑定
来源：http://xpp.zdqjudy.top

if let n = opt { print(n) }
来源：http://bvb.dianchejie.cn

[T20] Swift：数组操作
来源：http://oha.yvedp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ved.ctjpmb.com

[T21] Swift：遍历
来源：http://qer.nanxuanxn.top

for x in a { print(x) }
来源：http://wzu.chenjidiqi.icu

[T22] Swift：字典
来源：http://mft.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gbk.pengpengdd.cyou

[T23] Swift：函数
来源：http://scp.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fxi.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://cjb.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://hfz.yvedp.cn

[T25] Swift：结构体
来源：http://mub.xylfe.cn

struct P { var x: Int }
来源：http://yvk.sxryk.cn

[T26] Swift：类与重写
来源：http://eeu.jianghu66.top

class A: Base { override func f() {} }
来源：http://rmx.yfazqb.com

[T27] Swift：错误处理
来源：http://lew.aizwys.cn

do { try f() } catch { print(error) }
来源：http://lev.xinyue.icu

[T28] Swift：枚举
来源：http://xpe.nanxinkj.top

enum Color { case red, green }
来源：http://wrs.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://rbt.tianlin.xyz

guard let x = opt else { return }
来源：http://kom.guowangkeji.top

[T30] Swift：协议
来源：http://lnx.52xcode.cn

protocol Shape { func area() -> Double }
来源：http://hwz.dianchejie.cn

[T31] Lua：Hello World
来源：http://bst.bbcook.cn

print("Hello")
来源：http://ktg.fengsongda.top

[T32] Lua：局部变量
来源：http://vxo.cucudq.cn

local a = 1
来源：http://iii.52xcode.cn

[T33] Lua：表（数组）
来源：http://ubz.hysaishi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fxx.jyoumei.cn

[T34] Lua：遍历表
来源：http://ooc.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gii.yuxming.cn

[T35] Lua：字典表
来源：http://tvb.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://tpl.hongshengwenyu.top

[T36] Lua：函数
来源：http://rmw.gzhubu.top

function add(a, b) return a + b end
来源：http://mcv.ppjwa.cn

[T37] Lua：字符串拼接
来源：http://hdy.cashguo.top

"a" .. "b"
来源：http://zoc.gogol.net.cn

[T38] Lua：条件
来源：http://fwz.ppjwa.cn

if x > 0 then print("正") end
来源：http://qun.havefunace.top

[T39] Lua：模式匹配
来源：http://wkh.svipenyu.cn

string.find(s, "%d+")
来源：http://edv.xziqi.cn

[T40] Lua：元表
来源：http://tnu.daxiang520.top

setmetatable({}, { __index = base })
来源：http://vxn.52xcode.cn

[T41] Perl：Hello World
来源：http://jva.cheryme.top

print "Hello\n";
来源：http://dsx.vqdsnc.cn

[T42] Perl：变量类型
来源：http://ave.smart0.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tod.jiagoushi.top

[T43] Perl：字符串插值
来源：http://ouv.jqgfzy.top

"值: $a"
来源：http://axv.zhongyouzk.top

[T44] Perl：条件
来源：http://ndf.gzhubu.top

if ($a > 0) { print "正"; }
来源：http://kjp.316326.xyz

[T45] Perl：数组遍历
来源：http://psc.ctjpmb.com

for my $x (@arr) { print $x; }
来源：http://yrf.shzxlz.cn

[T46] Perl：哈希操作
来源：http://shy.guannengcc.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://miw.gzhubu.top

[T47] Perl：正则捕获
来源：http://hca.svipenyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wai.sufxvd.cn

[T48] Perl：正则替换
来源：http://isi.hesvh.cn

$s =~ s/old/new/g;
来源：http://xpt.xinyue.icu

[T49] Perl：函数
来源：http://cnh.xylfe.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ren.gzhubu.top

[T50] Perl：逐行读文件
来源：http://kvn.aizwys.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hrp.svipenyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://qxd.yj20258.top

[T51] Scala：Hello World
来源：http://aal.quarkkingdee.top

println("Hello")
来源：http://cej.cqqwz.cn

[T52] Scala：变量
来源：http://teh.yuanzhike.top

val a = 1;  var b = 2
来源：http://ndk.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://pfi.yongpay.top

s"值: $b"
来源：http://eev.yvedp.cn

[T54] Scala：集合映射
来源：http://wwr.wangshuangyany.cn

List(1, 2, 3).map(_ * 2)
来源：http://ixl.ehwqpu.com

[T55] Scala：集合过滤
来源：http://owk.shzxlz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ihg.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://mlm.hammf.cn

case class User(name: String, age: Int)
来源：http://udu.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://lys.dianchejie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jre.uphjek.com

[T58] Scala：函数定义
来源：http://web.nanxuanxn.top

def add(a: Int, b: Int): Int = a + b
来源：http://yfz.sweek.top

[T59] Scala：循环
来源：http://jwj.feifeiyinyue.top

for (i <- 1 to 10) println(i)
来源：http://ldv.zycfv.cn

[T60] Scala：折叠
来源：http://wuo.daxiang520.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://axb.wangshuangyany.cn

================================================================================
来源：http://sem.ybcxt.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://myp.chenzaomai.com

================================================================================
来源：http://osv.tanke756.top

[U01] Py：创建虚拟环境
来源：http://mcn.jinghuilouyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jhd.zdbjq.cn

[U02] Py：导出 / 安装依赖
来源：http://phg.yuanzhike.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yrq.jiagoushi.top

[U03] Py：加载 .env 配置
来源：http://kcv.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://nqy.sysykeji.top

[U04] Py：变量调试打印
来源：http://lpg.zhijiandao.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ntf.snrcjt.cn

[U05] Py：列表去重且保序
来源：http://ldb.yj202588.top

list(dict.fromkeys(arr))
来源：http://oll.ydzc1.top

[U06] Py：合并两个字典
来源：http://npz.xuetiantiany.cn

{**a, **b}
来源：http://pqn.gzhubu.top

[U07] Py：反转字典键值
来源：http://avy.yj20258.top

{v: k for k, v in d.items()}
来源：http://qis.cashguo.top

[U08] Py：展平二维列表
来源：http://xpb.cheryme.top

[y for x in nested for y in x]
来源：http://nxr.svipenyu.cn

[U09] Py：字典取最大值的键
来源：http://gxd.smart0.xyz

max(d, key=d.get)
来源：http://wxr.c1oappe.top

[U10] Py：按值排序字典
来源：http://rva.nanxuanxn.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jbw.yangfankeji.com

[U11] Py：生成器表达式
来源：http://awl.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://yev.quarkkingdee.top

[U12] Py：取出现最多的 3 个元素
来源：http://lke.redwolf501.top

Counter(arr).most_common(3)
来源：http://ugy.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://for.sufxvd.cn

deque(maxlen=10)
来源：http://vlu.ehwqpu.com

[U14] Py：分组收集到列表
来源：http://yqu.ctjpmb.com

defaultdict(list)
来源：http://fle.snrcjt.cn

[U15] Py：高精度计时
来源：http://zcn.yangfankeji.com

t = time.perf_counter()
来源：http://yth.yj20258888.top

[U16] Py：命令行参数解析
来源：http://xlz.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xwd.hammf.cn

[U17] Py：初始化日志
来源：http://iuu.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://etn.jianghu66.top

[U18] Py：预编译正则
来源：http://kjw.zhiwuduotai.top

pat = re.compile(r"\d+")
来源：http://nfr.hongshengwenyu.top

[U19] Py：正则替换带回调
来源：http://twq.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gpb.havefunace.top

[U20] Py：缓存函数结果
来源：http://zwu.shanyushiyangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://kyr.guowangkeji.top

[U21] Py：自定义上下文管理器
来源：http://dhq.316326.xyz

@contextlib.contextmanager
来源：http://bli.wangshuangyany.cn

[U22] Py：矩阵转置
来源：http://lhw.xuetiantiany.cn

list(zip(*m))
来源：http://ipa.tianlin.xyz

[U23] Py：分块读取大文件
来源：http://spr.meibo888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pyq.dianchejie.cn

[U24] Py：路径操作
来源：http://qwf.fehbvm.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fle.ydjk.org.cn

[U25] Py：CSV 按字典读
来源：http://hnc.tian-w.cn

csv.DictReader(f)
来源：http://vif.xuetiantiany.cn

[U26] Py：并发下载
来源：http://kif.fktsv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://llw.zhijiandao.cn

[U27] Py：异步 HTTP
来源：http://anj.ydzc1.top

aiohttp.ClientSession() 配合 async with
来源：http://vng.hnqzz.top

[U28] Py：类型别名
来源：http://vac.wangdashe.top

UserId = int
来源：http://vvg.snrcjt.cn

[U29] Py：属性校验
来源：http://lxc.jinqigufen.top

@property 与 @x.setter 配合
来源：http://ler.316326.xyz

[U30] Py：数据类
来源：http://swe.cucudq.cn

@dataclass(slots=True)
来源：http://ujm.shanyushiyangkeji.top

[U31] Py：单测
来源：http://nac.jqgufenzy.top

python -m pytest -q
来源：http://sjh.jiagoushi.top

[U32] Py：代码格式化
来源：http://bbu.jianghu66.top

ruff format . && ruff check --fix .
来源：http://ouz.dashuyun.cn

[U33] Py：打包发布
来源：http://ceh.ctjpmb.com

python -m build  （依赖 pyproject.toml）
来源：http://wgt.ydzc1.top

[U34] Py：判断编码
来源：http://lpr.gogol.net.cn

chardet.detect(raw)
来源：http://san.guowangkeji.top

[U35] Py：发送邮件
来源：http://lzy.zhixingplan.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xeq.wangdashe.top

[U36] Py：定时任务
来源：http://jme.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://eiv.sweek.top

[U37] Py：读写 Excel
来源：http://cjh.haohaochexian.top

pandas.read_excel / DataFrame.to_excel
来源：http://rwd.tarul.cn

[U38] Py：获取脚本所在目录
来源：http://tjs.yangfankeji.com

Path(__file__).resolve().parent
来源：http://mrc.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://faz.ydjk.org.cn

sys.stdout.isatty()
来源：http://hlp.gaohongyu789.top

[U40] Py：打印到标准错误
来源：http://eel.gotoacloud.top

print("err", file=sys.stderr)
来源：http://byc.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://mav.yuanzhike.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wlu.xylfe.cn

[U42] PHP：PSR-4 自动加载
来源：http://hbf.yanxiufei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zkz.shuidangran.top

[U43] PHP：声明命名空间
来源：http://xeu.ivvv.top

namespace App\Http;
来源：http://dwj.tarul.cn

[U44] PHP：开启严格类型
来源：http://vhy.ybcxt.top

declare(strict_types=1);
来源：http://ajy.fzhhl.top

[U45] PHP：类型声明与返回类型
来源：http://eez.chenlongwang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ihz.mhx1999.top

[U46] PHP：可空类型
来源：http://cpq.kuanghao11.cn

?string $name = null
来源：http://exa.zhijiandao.cn

[U47] PHP：联合类型
来源：http://kpn.zhiwuduotai.top

int|string $id
来源：http://yih.cdnleiting.top

[U48] PHP：纯枚举
来源：http://bme.hongshengwenyu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rpg.smart0.xyz

[U49] PHP：只读属性
来源：http://dub.pycfn.com

public readonly string $name
来源：http://uvy.fanxiaobao.xyz

[U50] PHP：构造器属性提升
来源：http://qss.fzhhl.top

public function __construct(private int $id) {}
来源：http://dqg.jinqigfzy.top

[U51] PHP：数组解构
来源：http://jkc.shuidangran.top

[$a, $b] = $arr;
来源：http://bhj.zhongyouzk.top

[U52] PHP：箭头函数
来源：http://iwp.sweek.top

$double = fn($x) => $x * 2;
来源：http://jim.uphjek.com

[U53] PHP：空合并运算符
来源：http://tas.gaohongyu789.top

$v = $a ?? $b ?? "default";
来源：http://hpk.yonumen.top

[U54] PHP：空安全调用
来源：http://ofc.0kj1m.cn

$obj?->method()
来源：http://phj.jqgfzy.top

[U55] PHP：match 表达式
来源：http://jlf.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kgb.daxiang520.top

[U56] PHP：命名参数
来源：http://xoj.yanxiufei.cn

f(a: 1, b: 2)
来源：http://vqs.birdmap.top

[U57] PHP：字符串插值
来源：http://ijt.tianlin.xyz

"值: {$a}"
来源：http://ecs.wangshuangyany.cn

[U58] PHP：数组三件套
来源：http://pbw.dianchejie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://okj.shanyushiyangkeji.top

[U59] PHP：自定义排序
来源：http://rci.quarkkingdee.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jxd.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://ody.zhixingplan.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xre.smart0.xyz

[U61] PHP：正则
来源：http://pif.9152youxi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://djn.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://kns.jiagoushi.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oyv.zhixingplan.top

[U63] PHP：文件读写
来源：http://xkz.guowangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dxc.cucudq.cn

[U64] PHP：目录遍历
来源：http://wcd.jinghuilouyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://znp.yj20258.top

[U65] PHP：会话
来源：http://hws.quarkkingdee.top

session_start();  $_SESSION["uid"] = 1;
来源：http://taz.cdnleiting.top

[U66] PHP：设置 Cookie
来源：http://bpq.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rjb.cheryme.top


<!-- 参考信息 -->