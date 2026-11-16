代发 wailian999

[S41] C++：类与构造函数
来源：http://rvd.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://det.yj20258.top

[S42] C++：继承与虚函数
来源：http://ckp.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://tgh.redwolf501.top

[S43] C++：智能指针
来源：http://sau.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://qrk.zycfv.cn

[S44] C++：引用传参
来源：http://ijd.pycfn.com

void inc(int &x) { ++x; }
来源：http://hbu.nwbrower.top

[S45] C++：lambda
来源：http://xpd.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://cpf.havefunace.top

[S46] C++：函数模板
来源：http://tju.dianchejie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hnv.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://zkc.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jai.svipenyu.cn

[S48] C++：逐行读文件
来源：http://hlq.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://frq.nanxuanxn.top

while (std::getline(in, line)) { }
来源：http://jiu.52xcode.cn

[S49] C++：写文件
来源：http://kew.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://elo.vehdjk.com

[S50] C++：格式化数字
来源：http://cgd.jlsjyb.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gep.tian-w.cn

[S51] C++：显式类型转换
来源：http://hjw.yuxming.cn

static_cast<double>(a) / b
来源：http://zhk.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://dwm.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://wgs.daria6918.cn

[S53] C++：移动语义
来源：http://ppo.hfpthk.cn

std::vector<int> w = std::move(v);
来源：http://afy.shuidangran.top

[S54] C++：异常处理
来源：http://hlh.tianlin.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aqg.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://ypu.ydjk.org.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qdp.jqgufenzy.top

[S56] C++：optional
来源：http://wie.yanxiufei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xxb.shanyushiyangkeji.top

[S57] C++：编译期常量
来源：http://moe.cucudq.cn

constexpr int N = 10;
来源：http://kbk.yuanzhike.top

[S58] C++：命名空间
来源：http://axz.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://zej.yueranfly.top

[S59] C++：静态断言
来源：http://lut.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oim.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://lul.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vqv.ppjwa.cn

================================================================================
来源：http://iob.tianlin.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rux.hammf.cn

================================================================================
来源：http://trk.52xcode.cn

[T01] Kotlin：Hello World
来源：http://ins.meibo888.top

println("Hello")
来源：http://dor.fehbvm.com

[T02] Kotlin：变量
来源：http://fnc.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://htq.kuanghao11.cn

[T03] Kotlin：字符串模板
来源：http://zzp.jinqigfzy.top

"值: $b"
来源：http://cqi.gotoacloud.top

[T04] Kotlin：空安全
来源：http://jyi.cdnleiting.top

val n: String? = null;  n?.length
来源：http://lkz.yongpay.top

[T05] Kotlin：when 表达式
来源：http://wro.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jev.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://ydb.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zfv.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://txq.mhx1999.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cdb.yfazqb.com

[T08] Kotlin：数据类
来源：http://dvq.hfpthk.cn

data class User(val name: String, val age: Int)
来源：http://rgx.yanxiufei.cn

[T09] Kotlin：扩展函数
来源：http://zaa.daria6918.cn

fun String.exclaim() = this + "!"
来源：http://rjj.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://sjt.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://iep.fanxiaobao.xyz

[T11] Kotlin：协程
来源：http://oyn.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xzr.wangdashe.top

[T12] Kotlin：解构声明
来源：http://bqp.guowangkeji.top

val (a, b) = Pair(1, 2)
来源：http://aws.shanyushiyangtech.top

[T13] Kotlin：只读 Map
来源：http://jvh.smart0.xyz

val m = mapOf("a" to 1)
来源：http://tko.hnxiangtu.top

[T14] Kotlin：循环
来源：http://hwd.316326.xyz

for (i in 1..10) println(i)
来源：http://ont.zdqjudy.top

[T15] Kotlin：接口
来源：http://dow.uphjek.com

interface Shape { fun area(): Double }
来源：http://qke.zhijiandao.cn

[T16] Swift：Hello World
来源：http://zbp.jinghuilouyu.cn

print("Hello")
来源：http://xfe.yueranfly.top

[T17] Swift：变量与常量
来源：http://ysn.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://hpf.jyoumei.cn

[T18] Swift：字符串插值
来源：http://fth.daria6918.cn

"值: \(b)"
来源：http://uqx.ctjpmb.com

[T19] Swift：可选绑定
来源：http://ate.iojbl.cn

if let n = opt { print(n) }
来源：http://ejl.yuxming.cn

[T20] Swift：数组操作
来源：http://som.zhoulong.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://dif.ctjpmb.com

[T21] Swift：遍历
来源：http://ouc.fktsv.cn

for x in a { print(x) }
来源：http://gst.sjlbkw.cn

[T22] Swift：字典
来源：http://pof.jinqigufen.top

var d = ["a": 1];  d["b"] = 2
来源：http://dty.snrcjt.cn

[T23] Swift：函数
来源：http://qwk.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sox.feifeiyinyue.top

[T24] Swift：闭包
来源：http://fna.nwbrower.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wsx.tianlin.xyz

[T25] Swift：结构体
来源：http://kqo.tanke756.top

struct P { var x: Int }
来源：http://lfi.quarkkingdee.top

[T26] Swift：类与重写
来源：http://ojo.ctjpmb.com

class A: Base { override func f() {} }
来源：http://xsh.tian-w.cn

[T27] Swift：错误处理
来源：http://vqo.yongpay.top

do { try f() } catch { print(error) }
来源：http://rmw.cdnleiting.top

[T28] Swift：枚举
来源：http://vxv.fengsongda.top

enum Color { case red, green }
来源：http://ooi.fehbvm.com

[T29] Swift：guard 提前返回
来源：http://zbw.guannengcc.top

guard let x = opt else { return }
来源：http://kiz.zycfv.cn

[T30] Swift：协议
来源：http://vqf.cheryme.top

protocol Shape { func area() -> Double }
来源：http://xcr.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://hau.ehwqpu.com

print("Hello")
来源：http://vto.cheryme.top

[T32] Lua：局部变量
来源：http://nsk.hesvh.cn

local a = 1
来源：http://sea.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://cmm.ehwqpu.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ifo.zhoulong.xyz

[T34] Lua：遍历表
来源：http://xso.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ixz.cdnleiting.top

[T35] Lua：字典表
来源：http://olg.shangyingyoupin.top

local d = { a = 1 };  d.b = 2
来源：http://nac.yj20258.top

[T36] Lua：函数
来源：http://vzi.fehbvm.com

function add(a, b) return a + b end
来源：http://qkk.ehwqpu.com

[T37] Lua：字符串拼接
来源：http://mfm.cdnleiting.top

"a" .. "b"
来源：http://iyu.zhiwuduotai.top

[T38] Lua：条件
来源：http://gfs.ehwqpu.com

if x > 0 then print("正") end
来源：http://yzv.ppjwa.cn

[T39] Lua：模式匹配
来源：http://iwa.yongpay.top

string.find(s, "%d+")
来源：http://zbb.hnqzz.top

[T40] Lua：元表
来源：http://qwx.ehwqpu.com

setmetatable({}, { __index = base })
来源：http://ntd.iojbl.cn

[T41] Perl：Hello World
来源：http://zhp.jlsjyb.cn

print "Hello\n";
来源：http://afn.wangshuangyany.cn

[T42] Perl：变量类型
来源：http://kam.xuanzx.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bku.haohaochexian.top

[T43] Perl：字符串插值
来源：http://pvu.fengsongda.top

"值: $a"
来源：http://svc.vqdsnc.cn

[T44] Perl：条件
来源：http://dno.hfpthk.cn

if ($a > 0) { print "正"; }
来源：http://uty.yangfankeji.com

[T45] Perl：数组遍历
来源：http://mbg.gzhubu.top

for my $x (@arr) { print $x; }
来源：http://pxv.yj20258888.top

[T46] Perl：哈希操作
来源：http://icl.xingfuxueyuan.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vii.sufxvd.cn

[T47] Perl：正则捕获
来源：http://ehl.mhx1999.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fyl.52xcode.cn

[T48] Perl：正则替换
来源：http://mqz.epnwcf.com

$s =~ s/old/new/g;
来源：http://zgl.ppjwa.cn

[T49] Perl：函数
来源：http://hce.zhoulong.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hoo.gzhubu.top

[T50] Perl：逐行读文件
来源：http://nfr.snrcjt.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://njb.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://dab.vqdsnc.cn

[T51] Scala：Hello World
来源：http://bge.ctjpmb.com

println("Hello")
来源：http://iql.bjfxy.top

[T52] Scala：变量
来源：http://vvv.zhoulong.xyz

val a = 1;  var b = 2
来源：http://pst.jqgfzy.top

[T53] Scala：字符串插值
来源：http://fgq.vehdjk.com

s"值: $b"
来源：http://vmk.jqgufenzy.top

[T54] Scala：集合映射
来源：http://jhh.guowangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://xkn.dianchejie.cn

[T55] Scala：集合过滤
来源：http://wym.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://lvu.chenzaomai.com

[T56] Scala：样例类
来源：http://ezp.zhengqikj.top

case class User(name: String, age: Int)
来源：http://lef.nanxinkj.top

[T57] Scala：模式匹配
来源：http://udw.zhaomingkeji.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://rmc.xingfuxueyuan.xyz

[T58] Scala：函数定义
来源：http://pqn.redwolf501.top

def add(a: Int, b: Int): Int = a + b
来源：http://fnd.wangdashe.top

[T59] Scala：循环
来源：http://vga.xylfe.cn

for (i <- 1 to 10) println(i)
来源：http://wgf.hongshengwenyu.top

[T60] Scala：折叠
来源：http://olx.hywenlv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xps.zhixingplan.top

================================================================================
来源：http://ucw.bbcook.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zea.sxryk.cn

================================================================================
来源：http://pzo.xinyue.icu

[U01] Py：创建虚拟环境
来源：http://hvo.xinyue.icu

python -m venv .venv && source .venv/bin/activate
来源：http://ygc.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://hdn.yonumen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zxw.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://lhc.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://paw.redwolf501.top

[U04] Py：变量调试打印
来源：http://ulm.chenlongwang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ukd.ybcxt.top

[U05] Py：列表去重且保序
来源：http://brh.daxiang520.top

list(dict.fromkeys(arr))
来源：http://prz.zhiwuduotai.top

[U06] Py：合并两个字典
来源：http://ldh.gaohongyu789.top

{**a, **b}
来源：http://smm.bbcook.cn

[U07] Py：反转字典键值
来源：http://usq.nanxinkj.top

{v: k for k, v in d.items()}
来源：http://auf.shanyushiyangtech.top

[U08] Py：展平二维列表
来源：http://cjv.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://xny.dianchejie.cn

[U09] Py：字典取最大值的键
来源：http://gpo.yuxming.cn

max(d, key=d.get)
来源：http://xex.tianlin.xyz

[U10] Py：按值排序字典
来源：http://lna.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ayw.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://dap.yuanzhike.top

(x * 2 for x in arr)
来源：http://gbv.yuxming.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nii.yj202588.top

Counter(arr).most_common(3)
来源：http://mzz.yj20258888.top

[U13] Py：固定长度队列
来源：http://gsh.sysykeji.top

deque(maxlen=10)
来源：http://xie.fktsv.cn

[U14] Py：分组收集到列表
来源：http://vxj.haohaochexian.top

defaultdict(list)
来源：http://ypn.zhixingplan.top

[U15] Py：高精度计时
来源：http://ynu.uphjek.com

t = time.perf_counter()
来源：http://znn.meibo888.top

[U16] Py：命令行参数解析
来源：http://ows.hcnkem.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rxt.jianghu66.top

[U17] Py：初始化日志
来源：http://ulq.chenlongwang.top

logging.basicConfig(level=logging.INFO)
来源：http://bge.yonumen.top

[U18] Py：预编译正则
来源：http://oox.yueranfly.top

pat = re.compile(r"\d+")
来源：http://fsp.gzhubu.top

[U19] Py：正则替换带回调
来源：http://qjb.cheryme.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ipy.feifeiyinyue.top

[U20] Py：缓存函数结果
来源：http://rhx.shanyushiyangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://dim.shanyushiyangtech.top

[U21] Py：自定义上下文管理器
来源：http://vgz.yongpay.top

@contextlib.contextmanager
来源：http://qar.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://fww.52xcode.cn

list(zip(*m))
来源：http://ryj.xuetiantiany.cn

[U23] Py：分块读取大文件
来源：http://uxs.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oyq.zhongyouzk.top

[U24] Py：路径操作
来源：http://ukq.hysaishi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uuu.guannengcc.top

[U25] Py：CSV 按字典读
来源：http://cmc.kuanghao11.cn

csv.DictReader(f)
来源：http://hzd.mhx1999.top

[U26] Py：并发下载
来源：http://wbe.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bbh.gaohongyu789.top

[U27] Py：异步 HTTP
来源：http://deh.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://den.52xcode.cn

[U28] Py：类型别名
来源：http://zia.gotoacloud.top

UserId = int
来源：http://yci.yueranfly.top

[U29] Py：属性校验
来源：http://rim.cheryme.top

@property 与 @x.setter 配合
来源：http://zwp.zhoulong.xyz

[U30] Py：数据类
来源：http://vxr.jiagoushi.top

@dataclass(slots=True)
来源：http://tdj.epnwcf.com

[U31] Py：单测
来源：http://hnd.shanyushiyangkeji.top

python -m pytest -q
来源：http://jvq.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://sie.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://uev.smart0.xyz

[U33] Py：打包发布
来源：http://fke.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://cbq.52xcode.cn

[U34] Py：判断编码
来源：http://hbi.tarul.cn

chardet.detect(raw)
来源：http://rbc.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://vkh.0kj1m.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nnx.daxiang520.top

[U36] Py：定时任务
来源：http://bih.andypj.xyz

schedule.every(10).minutes.do(job)
来源：http://vuk.hnxiangtu.top

[U37] Py：读写 Excel
来源：http://swe.daxiang520.top

pandas.read_excel / DataFrame.to_excel
来源：http://vld.yanxiufei.cn

[U38] Py：获取脚本所在目录
来源：http://qlo.hongshengwenyu.top

Path(__file__).resolve().parent
来源：http://sjt.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://hpl.tanke756.top

sys.stdout.isatty()
来源：http://mqt.hfpthk.cn

[U40] Py：打印到标准错误
来源：http://wnf.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://bwr.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://qff.jinghuilouyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jnc.gogol.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://vwt.c1oappe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pgd.dashuyun.cn

[U43] PHP：声明命名空间
来源：http://nhq.mhx1999.top

namespace App\Http;
来源：http://huc.jinyuanbaomall.cn

[U44] PHP：开启严格类型
来源：http://hkp.sjlbkw.cn

declare(strict_types=1);
来源：http://snw.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://drg.yongpay.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kyl.aibaodan.cn

[U46] PHP：可空类型
来源：http://qkk.fehbvm.com

?string $name = null
来源：http://axv.ivvv.top

[U47] PHP：联合类型
来源：http://rah.ppjwa.cn

int|string $id
来源：http://wrs.hcnkem.com

[U48] PHP：纯枚举
来源：http://dws.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pps.jiagoushi.top

[U49] PHP：只读属性
来源：http://brg.gzhubu.top

public readonly string $name
来源：http://jvf.ctjpmb.com

[U50] PHP：构造器属性提升
来源：http://hrb.hongshengwenyu.top

public function __construct(private int $id) {}
来源：http://nby.smart0.xyz

[U51] PHP：数组解构
来源：http://mcn.daria6918.cn

[$a, $b] = $arr;
来源：http://fzn.jinghuilouyu.cn

[U52] PHP：箭头函数
来源：http://efh.jinyuanbaomall.cn

$double = fn($x) => $x * 2;
来源：http://ejz.ybcxt.top

[U53] PHP：空合并运算符
来源：http://zjp.zhiwuduotai.top

$v = $a ?? $b ?? "default";
来源：http://sok.gotoacloud.top

[U54] PHP：空安全调用
来源：http://eda.guowangkeji.top

$obj?->method()
来源：http://qro.fehbvm.com

[U55] PHP：match 表达式
来源：http://lxl.zdqjudy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ajx.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://yka.tarul.cn

f(a: 1, b: 2)
来源：http://dlo.sxryk.cn

[U57] PHP：字符串插值
来源：http://wid.cdnleiting.top

"值: {$a}"
来源：http://sji.chenzaomai.com

[U58] PHP：数组三件套
来源：http://ytn.cqqwz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xwt.ydzc1.top

[U59] PHP：自定义排序
来源：http://nhm.fzhhl.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blj.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://kvp.epnwcf.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://igk.chenlongwang.top

[U61] PHP：正则
来源：http://zxz.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oul.jianghu66.top

[U62] PHP：日期对象
来源：http://guq.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tvh.pengpengdd.cyou

[U63] PHP：文件读写
来源：http://cnr.yj202588.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://owa.aibaodan.cn

[U64] PHP：目录遍历
来源：http://lyx.mhx1999.top

glob("dir/*.php");  scandir("dir");
来源：http://vhl.epnwcf.com

[U65] PHP：会话
来源：http://enx.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ofj.ydjk.org.cn

[U66] PHP：设置 Cookie
来源：http://gdf.zdbjq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://noh.sufxvd.cn


<!-- 参考信息 -->