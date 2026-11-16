代发 wailian999

[S41] C++：类与构造函数
来源：http://sgv.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oqr.tian-w.cn

[S42] C++：继承与虚函数
来源：http://hac.9152youxi.cn

class B : public Base { public: void f() override {} };
来源：http://aeo.hongshengwenyu.top

[S43] C++：智能指针
来源：http://wut.yanxiufei.cn

auto p = std::make_unique<int>(5);
来源：http://sda.jyoumei.cn

[S44] C++：引用传参
来源：http://zzb.hcnkem.com

void inc(int &x) { ++x; }
来源：http://wfg.shzxlz.cn

[S45] C++：lambda
来源：http://isn.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://ygf.9152youxi.cn

[S46] C++：函数模板
来源：http://ywo.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://smm.chenjidiqi.icu

[S47] C++：结构化绑定遍历
来源：http://cms.hcnkem.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zjy.ybcxt.top

[S48] C++：逐行读文件
来源：http://ira.dianchejie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xfj.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://amr.tian-w.cn

[S49] C++：写文件
来源：http://kjl.tianlin.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zkl.jlsjyb.cn

[S50] C++：格式化数字
来源：http://mtt.316326.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nrc.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://gda.dashuyun.cn

static_cast<double>(a) / b
来源：http://bue.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://kog.yfazqb.com

int size() const noexcept { return n_; }
来源：http://ifk.xylfe.cn

[S53] C++：移动语义
来源：http://wui.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://dke.ybcxt.top

[S54] C++：异常处理
来源：http://evq.jqgufenzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vyh.yangfankeji.com

[S55] C++：结构化绑定
来源：http://fol.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mkg.kuanghao11.cn

[S56] C++：optional
来源：http://ugm.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wht.tian-w.cn

[S57] C++：编译期常量
来源：http://pri.epnwcf.com

constexpr int N = 10;
来源：http://umk.jqgfzy.top

[S58] C++：命名空间
来源：http://yij.bjfxy.top

namespace ns { int f() { return 1; } }
来源：http://rww.quarkkingdee.top

[S59] C++：静态断言
来源：http://cug.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dod.daria6918.cn

[S60] C++：遍历并删除元素
来源：http://llg.zdqjudy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mpo.ywan-chungtsiang.top

================================================================================
来源：http://tmq.svipenyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jst.zhixingplan.top

================================================================================
来源：http://xuv.cheryme.top

[T01] Kotlin：Hello World
来源：http://ziz.vehdjk.com

println("Hello")
来源：http://xwh.52xcode.cn

[T02] Kotlin：变量
来源：http://twp.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ztt.jinyuanbaomall.cn

[T03] Kotlin：字符串模板
来源：http://enl.jinqigfzy.top

"值: $b"
来源：http://jnr.svipenyu.cn

[T04] Kotlin：空安全
来源：http://ryd.tian-w.cn

val n: String? = null;  n?.length
来源：http://foc.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://rsg.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vsk.daria6918.cn

[T06] Kotlin：集合映射
来源：http://rui.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://ldi.hnqzz.top

[T07] Kotlin：集合过滤
来源：http://bxq.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xpg.yj202588.top

[T08] Kotlin：数据类
来源：http://ghb.jqgufenzy.top

data class User(val name: String, val age: Int)
来源：http://ruw.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://ubz.yonumen.top

fun String.exclaim() = this + "!"
来源：http://uor.guannengcc.top

[T10] Kotlin：默认参数
来源：http://tsl.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lfo.bbcook.cn

[T11] Kotlin：协程
来源：http://jsh.dashuyun.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ypt.birdmap.top

[T12] Kotlin：解构声明
来源：http://uty.sufxvd.cn

val (a, b) = Pair(1, 2)
来源：http://dry.c1oappe.top

[T13] Kotlin：只读 Map
来源：http://ggm.hnxiangtu.top

val m = mapOf("a" to 1)
来源：http://uzb.yuanzhike.top

[T14] Kotlin：循环
来源：http://upn.cqqwz.cn

for (i in 1..10) println(i)
来源：http://gcl.aizwys.cn

[T15] Kotlin：接口
来源：http://kic.ppjwa.cn

interface Shape { fun area(): Double }
来源：http://cam.kuanghao11.cn

[T16] Swift：Hello World
来源：http://raq.epnwcf.com

print("Hello")
来源：http://dhr.xuanzx.com

[T17] Swift：变量与常量
来源：http://gds.ivvv.top

var a = 1;  let b = 2
来源：http://kof.cashguo.top

[T18] Swift：字符串插值
来源：http://yxs.ydzc1.top

"值: \(b)"
来源：http://beb.shzxlz.cn

[T19] Swift：可选绑定
来源：http://dir.xuanzx.com

if let n = opt { print(n) }
来源：http://iir.hysaishi.cn

[T20] Swift：数组操作
来源：http://kut.yongpay.top

var a = [1, 2, 3];  a.append(4)
来源：http://wms.hywenlv.cn

[T21] Swift：遍历
来源：http://ipa.dianchejie.cn

for x in a { print(x) }
来源：http://hnc.uphjek.com

[T22] Swift：字典
来源：http://kjf.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vji.zhijiandao.cn

[T23] Swift：函数
来源：http://cpa.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wcq.yonumen.top

[T24] Swift：闭包
来源：http://ema.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wzi.nwbrower.top

[T25] Swift：结构体
来源：http://ald.svipenyu.cn

struct P { var x: Int }
来源：http://rnm.tianlin.xyz

[T26] Swift：类与重写
来源：http://urg.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://gnc.gzhubu.top

[T27] Swift：错误处理
来源：http://wrh.redwolf501.top

do { try f() } catch { print(error) }
来源：http://drv.cqqwz.cn

[T28] Swift：枚举
来源：http://fvk.wangdashe.top

enum Color { case red, green }
来源：http://pha.mhx1999.top

[T29] Swift：guard 提前返回
来源：http://tls.mhx1999.top

guard let x = opt else { return }
来源：http://bdy.birdmap.top

[T30] Swift：协议
来源：http://dew.meibo888.top

protocol Shape { func area() -> Double }
来源：http://sbd.nanxuanxn.top

[T31] Lua：Hello World
来源：http://pie.yj202588.top

print("Hello")
来源：http://bui.jinghuilouyu.cn

[T32] Lua：局部变量
来源：http://vbl.sufxvd.cn

local a = 1
来源：http://plb.cucudq.cn

[T33] Lua：表（数组）
来源：http://vqw.cucudq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zvv.vqdsnc.cn

[T34] Lua：遍历表
来源：http://dtv.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zzb.xziqi.cn

[T35] Lua：字典表
来源：http://nie.ydjk.org.cn

local d = { a = 1 };  d.b = 2
来源：http://gkr.yuanzhike.top

[T36] Lua：函数
来源：http://sum.pengpengdd.cyou

function add(a, b) return a + b end
来源：http://utu.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://fyu.cucudq.cn

"a" .. "b"
来源：http://ldz.yj20258.top

[T38] Lua：条件
来源：http://dqf.kuanghao11.cn

if x > 0 then print("正") end
来源：http://zgc.wangdashe.top

[T39] Lua：模式匹配
来源：http://rca.shuidangran.top

string.find(s, "%d+")
来源：http://rxq.yj202588.top

[T40] Lua：元表
来源：http://ygz.zdbjq.cn

setmetatable({}, { __index = base })
来源：http://upd.zdbjq.cn

[T41] Perl：Hello World
来源：http://jzm.cdnleiting.top

print "Hello\n";
来源：http://gyx.xingfuxueyuan.xyz

[T42] Perl：变量类型
来源：http://kyi.birdmap.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jtg.fehbvm.com

[T43] Perl：字符串插值
来源：http://lwu.yfazqb.com

"值: $a"
来源：http://wrb.jqgufenzy.top

[T44] Perl：条件
来源：http://auv.meibo888.top

if ($a > 0) { print "正"; }
来源：http://krl.ppjwa.cn

[T45] Perl：数组遍历
来源：http://flw.shzxlz.cn

for my $x (@arr) { print $x; }
来源：http://dtu.jinghuilouyu.cn

[T46] Perl：哈希操作
来源：http://bsk.yanxiufei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tob.bjfxy.top

[T47] Perl：正则捕获
来源：http://qax.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ifo.cheryme.top

[T48] Perl：正则替换
来源：http://hjx.cucudq.cn

$s =~ s/old/new/g;
来源：http://yvj.daxiang520.top

[T49] Perl：函数
来源：http://mmc.9152youxi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ppu.cdnleiting.top

[T50] Perl：逐行读文件
来源：http://jbo.yj202588.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xno.daria6918.cn

while (my $line = <$fh>) { print $line; }
来源：http://rts.xinyue.icu

[T51] Scala：Hello World
来源：http://lar.hfpthk.cn

println("Hello")
来源：http://isa.zycfv.cn

[T52] Scala：变量
来源：http://yhn.sjlbkw.cn

val a = 1;  var b = 2
来源：http://mao.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://wjz.gotoacloud.top

s"值: $b"
来源：http://eus.tanke756.top

[T54] Scala：集合映射
来源：http://ixa.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://eoh.gaohongyu789.top

[T55] Scala：集合过滤
来源：http://oyq.gotoacloud.top

List(1, 2, 3).filter(_ > 1)
来源：http://tlk.jinqigufen.top

[T56] Scala：样例类
来源：http://kxu.uphjek.com

case class User(name: String, age: Int)
来源：http://ljj.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://kkp.hysaishi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hyq.cdnleiting.top

[T58] Scala：函数定义
来源：http://edv.hesvh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://enk.fktsv.cn

[T59] Scala：循环
来源：http://rgn.daxiang520.top

for (i <- 1 to 10) println(i)
来源：http://ebi.52xcode.cn

[T60] Scala：折叠
来源：http://ldf.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pyq.epnwcf.com

================================================================================
来源：http://rxv.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xim.pycfn.com

================================================================================
来源：http://yuk.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://qnn.gotoacloud.top

python -m venv .venv && source .venv/bin/activate
来源：http://pmd.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://nsq.hnxiangtu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qlc.jinqigfzy.top

[U03] Py：加载 .env 配置
来源：http://etf.yvedp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hqf.epnwcf.com

[U04] Py：变量调试打印
来源：http://cbs.chenzaomai.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qwt.yj20258.top

[U05] Py：列表去重且保序
来源：http://ohw.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://uyy.9152youxi.cn

[U06] Py：合并两个字典
来源：http://zol.ctjpmb.com

{**a, **b}
来源：http://qyi.vehdjk.com

[U07] Py：反转字典键值
来源：http://pcq.9152youxi.cn

{v: k for k, v in d.items()}
来源：http://uvp.aibaodan.cn

[U08] Py：展平二维列表
来源：http://mid.birdmap.top

[y for x in nested for y in x]
来源：http://qra.feifeiyinyue.top

[U09] Py：字典取最大值的键
来源：http://aez.iojbl.cn

max(d, key=d.get)
来源：http://yzd.wangdashe.top

[U10] Py：按值排序字典
来源：http://urz.jinqigfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lnl.redwolf501.top

[U11] Py：生成器表达式
来源：http://kkx.aibaodan.cn

(x * 2 for x in arr)
来源：http://bsq.hammf.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vqp.feifeiyinyue.top

Counter(arr).most_common(3)
来源：http://dmg.hywenlv.cn

[U13] Py：固定长度队列
来源：http://ala.yuxming.cn

deque(maxlen=10)
来源：http://emt.sweek.top

[U14] Py：分组收集到列表
来源：http://wsq.yangfankeji.com

defaultdict(list)
来源：http://pil.hnxiangtu.top

[U15] Py：高精度计时
来源：http://evu.nanxinkj.top

t = time.perf_counter()
来源：http://bfz.cheryme.top

[U16] Py：命令行参数解析
来源：http://lst.xuanzx.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ccf.jiagoushi.top

[U17] Py：初始化日志
来源：http://jma.sweek.top

logging.basicConfig(level=logging.INFO)
来源：http://lii.mhx1999.top

[U18] Py：预编译正则
来源：http://rbg.yfazqb.com

pat = re.compile(r"\d+")
来源：http://dcn.ehwqpu.com

[U19] Py：正则替换带回调
来源：http://cfl.pengpengdd.cyou

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://alu.tarul.cn

[U20] Py：缓存函数结果
来源：http://sqq.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://tms.52xcode.cn

[U21] Py：自定义上下文管理器
来源：http://ydg.yj20258.top

@contextlib.contextmanager
来源：http://afx.yuanzhike.top

[U22] Py：矩阵转置
来源：http://bgk.cucudq.cn

list(zip(*m))
来源：http://ona.vqdsnc.cn

[U23] Py：分块读取大文件
来源：http://itc.xuetiantiany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ggs.shangyingyoupin.top

[U24] Py：路径操作
来源：http://ywg.hammf.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yub.zhiwuduotai.top

[U25] Py：CSV 按字典读
来源：http://lvz.yuanzhike.top

csv.DictReader(f)
来源：http://urd.xylfe.cn

[U26] Py：并发下载
来源：http://rql.nanxinkj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://och.yueranfly.top

[U27] Py：异步 HTTP
来源：http://pte.hysaishi.cn

aiohttp.ClientSession() 配合 async with
来源：http://irn.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://pkq.zhijiandao.cn

UserId = int
来源：http://jcg.chenzaomai.com

[U29] Py：属性校验
来源：http://owt.wangdashe.top

@property 与 @x.setter 配合
来源：http://rjc.ctjpmb.com

[U30] Py：数据类
来源：http://hpj.cucudq.cn

@dataclass(slots=True)
来源：http://ezo.shangyingyoupin.top

[U31] Py：单测
来源：http://ubw.hnxiangtu.top

python -m pytest -q
来源：http://iuw.yj20258888.top

[U32] Py：代码格式化
来源：http://fqe.aizwys.cn

ruff format . && ruff check --fix .
来源：http://dtb.shzxlz.cn

[U33] Py：打包发布
来源：http://nej.nanxuanxn.top

python -m build  （依赖 pyproject.toml）
来源：http://hbp.hongshengwenyu.top

[U34] Py：判断编码
来源：http://ljw.hongshengwenyu.top

chardet.detect(raw)
来源：http://qoq.dashuyun.cn

[U35] Py：发送邮件
来源：http://apd.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cbe.mhx1999.top

[U36] Py：定时任务
来源：http://vij.nanxinkj.top

schedule.every(10).minutes.do(job)
来源：http://aaq.shangyingyoupin.top

[U37] Py：读写 Excel
来源：http://ebu.hnqzz.top

pandas.read_excel / DataFrame.to_excel
来源：http://gjs.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://eoo.vehdjk.com

Path(__file__).resolve().parent
来源：http://rnj.9152youxi.cn

[U39] Py：判断是否在交互环境
来源：http://oja.shzxlz.cn

sys.stdout.isatty()
来源：http://xwf.cdnleiting.top

[U40] Py：打印到标准错误
来源：http://irc.zhoulong.xyz

print("err", file=sys.stderr)
来源：http://ios.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://hae.dianchejie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ows.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://abs.tian-w.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dfx.hcnkem.com

[U43] PHP：声明命名空间
来源：http://tef.xinyue.icu

namespace App\Http;
来源：http://iki.hnqzz.top

[U44] PHP：开启严格类型
来源：http://orv.jinqigfzy.top

declare(strict_types=1);
来源：http://oot.hysaishi.cn

[U45] PHP：类型声明与返回类型
来源：http://otp.daria6918.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zco.yangfankeji.com

[U46] PHP：可空类型
来源：http://gjr.ydzc1.top

?string $name = null
来源：http://sxk.sysykeji.top

[U47] PHP：联合类型
来源：http://iuk.yuxming.cn

int|string $id
来源：http://vck.zdbjq.cn

[U48] PHP：纯枚举
来源：http://oxw.mhx1999.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hqe.cqqwz.cn

[U49] PHP：只读属性
来源：http://tvf.zdbjq.cn

public readonly string $name
来源：http://exm.zhiwuduotai.top

[U50] PHP：构造器属性提升
来源：http://sdm.fktsv.cn

public function __construct(private int $id) {}
来源：http://mju.iojbl.cn

[U51] PHP：数组解构
来源：http://qru.yj202588.top

[$a, $b] = $arr;
来源：http://frv.cheryme.top

[U52] PHP：箭头函数
来源：http://nft.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://itj.jyoumei.cn

[U53] PHP：空合并运算符
来源：http://bwc.hywenlv.cn

$v = $a ?? $b ?? "default";
来源：http://hpw.sysykeji.top

[U54] PHP：空安全调用
来源：http://eym.yj20258888.top

$obj?->method()
来源：http://jxh.cucudq.cn

[U55] PHP：match 表达式
来源：http://zzw.yvedp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vdv.jqgufenzy.top

[U56] PHP：命名参数
来源：http://xur.birdmap.top

f(a: 1, b: 2)
来源：http://ulq.hywenlv.cn

[U57] PHP：字符串插值
来源：http://xkn.yonumen.top

"值: {$a}"
来源：http://vze.jyoumei.cn

[U58] PHP：数组三件套
来源：http://iat.fktsv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qxy.yj202588.top

[U59] PHP：自定义排序
来源：http://mqj.yuxming.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://obw.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://iyw.uphjek.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uep.jiagoushi.top

[U61] PHP：正则
来源：http://wuq.ywan-chungtsiang.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uip.gzhubu.top

[U62] PHP：日期对象
来源：http://vev.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qlu.ydjk.org.cn

[U63] PHP：文件读写
来源：http://rpb.fktsv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://adv.ybcxt.top

[U64] PHP：目录遍历
来源：http://cbf.wangdashe.top

glob("dir/*.php");  scandir("dir");
来源：http://xjl.cdnleiting.top

[U65] PHP：会话
来源：http://ypi.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zxe.52xcode.cn

[U66] PHP：设置 Cookie
来源：http://fkx.gogol.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qtn.jinghuilouyu.cn


<!-- 参考信息 -->