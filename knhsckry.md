代发 wailian999

static int counter = 0;
来源：http://vvf.cqqwz.cn

[S29] C：变参函数
来源：http://ate.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wan.nanxuanxn.top

[S30] C：头文件保护
来源：http://afg.jinqigufen.top

#ifndef X_H
来源：http://ase.wangdashe.top

#define X_H
来源：http://acf.fengsongda.top

#endif
来源：http://asu.daria6918.cn

[S31] C++：Hello World
来源：http://flp.zhoulong.xyz

#include <iostream>
来源：http://ydv.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://zzc.zhiwuduotai.top

[S32] C++：字符串
来源：http://nuz.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://ncq.52xcode.cn

[S33] C++：vector 增删
来源：http://taa.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://phq.havefunace.top

[S34] C++：遍历 vector
来源：http://aog.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://hto.fktsv.cn

[S35] C++：map
来源：http://nmb.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rcn.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://pgk.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lgq.daxiang520.top

[S37] C++：set
来源：http://hzj.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hammf.cn

[S38] C++：排序
来源：http://eqw.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://xur.nanxinkj.top

[S39] C++：自定义比较器排序
来源：http://iwk.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oom.hnqzz.top

[S40] C++：查找元素
来源：http://osp.zhongyouzk.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wyg.fengsongda.top

[S41] C++：类与构造函数
来源：http://bdw.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://duk.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://mtp.fanxiaobao.xyz

class B : public Base { public: void f() override {} };
来源：http://ojk.jiagoushi.top

[S43] C++：智能指针
来源：http://uah.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://gcd.gaohongyu789.top

[S44] C++：引用传参
来源：http://ghj.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://nkt.tarul.cn

[S45] C++：lambda
来源：http://thk.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kix.c1oappe.top

[S46] C++：函数模板
来源：http://fxh.zdqjudy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cjj.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://pwk.meibo888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ewu.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://hrq.fengsongda.top

std::ifstream in("a.txt");  std::string line;
来源：http://jbn.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://xxg.guannengcc.top

[S49] C++：写文件
来源：http://pys.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mvx.yj20258888.top

[S50] C++：格式化数字
来源：http://wkk.yueranfly.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aqv.fanxiaobao.xyz

[S51] C++：显式类型转换
来源：http://ivp.shzxlz.cn

static_cast<double>(a) / b
来源：http://lyq.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://tkk.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://vcr.yj20258888.top

[S53] C++：移动语义
来源：http://fzx.fzhhl.top

std::vector<int> w = std::move(v);
来源：http://quy.tian-w.cn

[S54] C++：异常处理
来源：http://iwa.ydjk.org.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://icn.zycfv.cn

[S55] C++：结构化绑定
来源：http://pmp.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pkr.yvedp.cn

[S56] C++：optional
来源：http://lnb.zhiwuduotai.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ysi.nanxinkj.top

[S57] C++：编译期常量
来源：http://oci.pycfn.com

constexpr int N = 10;
来源：http://krb.jlsjyb.cn

[S58] C++：命名空间
来源：http://keq.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://zud.gzhubu.top

[S59] C++：静态断言
来源：http://roa.nwbrower.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nmy.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://nko.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://koe.smart0.xyz

================================================================================
来源：http://xam.xingfuxueyuan.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uhr.yangfankeji.com

================================================================================
来源：http://swq.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://lnn.aibaodan.cn

println("Hello")
来源：http://ckc.hywenlv.cn

[T02] Kotlin：变量
来源：http://ayj.hnxiangtu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qki.pycfn.com

[T03] Kotlin：字符串模板
来源：http://nsy.zhongyouzk.top

"值: $b"
来源：http://qqe.smart0.xyz

[T04] Kotlin：空安全
来源：http://fbv.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://wwx.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://zfe.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kik.iojbl.cn

[T06] Kotlin：集合映射
来源：http://rxf.fengsongda.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hpp.yvedp.cn

[T07] Kotlin：集合过滤
来源：http://fvd.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sgf.bbcook.cn

[T08] Kotlin：数据类
来源：http://oyr.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://frz.tanke756.top

[T09] Kotlin：扩展函数
来源：http://avc.zycfv.cn

fun String.exclaim() = this + "!"
来源：http://rfe.havefunace.top

[T10] Kotlin：默认参数
来源：http://vhy.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nup.ctjpmb.com

[T11] Kotlin：协程
来源：http://wup.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://omz.zhoulong.xyz

[T12] Kotlin：解构声明
来源：http://his.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://orw.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://kab.chenjidiqi.icu

val m = mapOf("a" to 1)
来源：http://wum.hcnkem.com

[T14] Kotlin：循环
来源：http://tee.chenlongwang.top

for (i in 1..10) println(i)
来源：http://fil.ydjk.org.cn

[T15] Kotlin：接口
来源：http://muj.aizwys.cn

interface Shape { fun area(): Double }
来源：http://thk.dashuyun.cn

[T16] Swift：Hello World
来源：http://rhu.snrcjt.cn

print("Hello")
来源：http://owo.nanxuanxn.top

[T17] Swift：变量与常量
来源：http://abm.ehwqpu.com

var a = 1;  let b = 2
来源：http://ldr.daria6918.cn

[T18] Swift：字符串插值
来源：http://vqr.bbcook.cn

"值: \(b)"
来源：http://uzb.jqgufenzy.top

[T19] Swift：可选绑定
来源：http://uor.yj20258888.top

if let n = opt { print(n) }
来源：http://hwz.yj20258888.top

[T20] Swift：数组操作
来源：http://ulr.jyoumei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zpu.hcnkem.com

[T21] Swift：遍历
来源：http://zzd.ydzc1.top

for x in a { print(x) }
来源：http://utf.yanxiufei.cn

[T22] Swift：字典
来源：http://lse.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://ezq.shangyingyoupin.top

[T23] Swift：函数
来源：http://uhz.jlsjyb.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://orn.sufxvd.cn

[T24] Swift：闭包
来源：http://jws.zycfv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uxz.tian-w.cn

[T25] Swift：结构体
来源：http://ddt.fzhhl.top

struct P { var x: Int }
来源：http://que.zhongyouzk.top

[T26] Swift：类与重写
来源：http://nnx.hesvh.cn

class A: Base { override func f() {} }
来源：http://fgw.yfazqb.com

[T27] Swift：错误处理
来源：http://lmu.hcnkem.com

do { try f() } catch { print(error) }
来源：http://pqa.snrcjt.cn

[T28] Swift：枚举
来源：http://bmr.xylfe.cn

enum Color { case red, green }
来源：http://bgz.jinghuilouyu.cn

[T29] Swift：guard 提前返回
来源：http://jjv.nwbrower.top

guard let x = opt else { return }
来源：http://omr.fengsongda.top

[T30] Swift：协议
来源：http://lap.sufxvd.cn

protocol Shape { func area() -> Double }
来源：http://mue.andypj.xyz

[T31] Lua：Hello World
来源：http://dry.hysaishi.cn

print("Hello")
来源：http://sre.bjfxy.top

[T32] Lua：局部变量
来源：http://tsw.ppjwa.cn

local a = 1
来源：http://rze.aibaodan.cn

[T33] Lua：表（数组）
来源：http://dce.smart0.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://dgq.smart0.xyz

[T34] Lua：遍历表
来源：http://got.gaohongyu789.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nns.birdmap.top

[T35] Lua：字典表
来源：http://eww.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://hod.zhengqikj.top

[T36] Lua：函数
来源：http://uvl.epnwcf.com

function add(a, b) return a + b end
来源：http://vec.yangfankeji.com

[T37] Lua：字符串拼接
来源：http://cya.chenzaomai.com

"a" .. "b"
来源：http://vfe.jianghu66.top

[T38] Lua：条件
来源：http://khe.gzhubu.top

if x > 0 then print("正") end
来源：http://sgg.yj202588.top

[T39] Lua：模式匹配
来源：http://nwy.yueranfly.top

string.find(s, "%d+")
来源：http://pwd.chenlongwang.top

[T40] Lua：元表
来源：http://zhe.yj202588.top

setmetatable({}, { __index = base })
来源：http://ohd.zhongyouzk.top

[T41] Perl：Hello World
来源：http://vyo.shangyingyoupin.top

print "Hello\n";
来源：http://vgv.yongpay.top

[T42] Perl：变量类型
来源：http://rkd.jinghuilouyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fak.xylfe.cn

[T43] Perl：字符串插值
来源：http://nij.pengpengdd.cyou

"值: $a"
来源：http://usy.yueranfly.top

[T44] Perl：条件
来源：http://wmy.andypj.xyz

if ($a > 0) { print "正"; }
来源：http://ruc.gzhubu.top

[T45] Perl：数组遍历
来源：http://qsy.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://iwz.vehdjk.com

[T46] Perl：哈希操作
来源：http://tje.shuidangran.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://alx.zdbjq.cn

[T47] Perl：正则捕获
来源：http://ybg.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://nmt.daria6918.cn

[T48] Perl：正则替换
来源：http://qua.hnxiangtu.top

$s =~ s/old/new/g;
来源：http://gxx.shuidangran.top

[T49] Perl：函数
来源：http://msf.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lkh.hongshengwenyu.top

[T50] Perl：逐行读文件
来源：http://kyc.iojbl.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tkh.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://hsd.zdqjudy.top

[T51] Scala：Hello World
来源：http://hqf.yangfankeji.com

println("Hello")
来源：http://rgr.gzhubu.top

[T52] Scala：变量
来源：http://kwy.ppjwa.cn

val a = 1;  var b = 2
来源：http://kkq.ppjwa.cn

[T53] Scala：字符串插值
来源：http://juz.hysaishi.cn

s"值: $b"
来源：http://wtg.sufxvd.cn

[T54] Scala：集合映射
来源：http://oiy.birdmap.top

List(1, 2, 3).map(_ * 2)
来源：http://apw.hammf.cn

[T55] Scala：集合过滤
来源：http://lsg.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://gbe.ctjpmb.com

[T56] Scala：样例类
来源：http://une.jianghu66.top

case class User(name: String, age: Int)
来源：http://aye.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://lbi.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qjg.jiagoushi.top

[T58] Scala：函数定义
来源：http://ywe.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://hoz.yuanzhike.top

[T59] Scala：循环
来源：http://duy.sweek.top

for (i <- 1 to 10) println(i)
来源：http://nkr.daria6918.cn

[T60] Scala：折叠
来源：http://xqk.xingfuxueyuan.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xlm.yfazqb.com

================================================================================
来源：http://ixr.xuetiantiany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://liz.316326.xyz

================================================================================
来源：http://asu.iojbl.cn

[U01] Py：创建虚拟环境
来源：http://ihk.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://aik.9152youxi.cn

[U02] Py：导出 / 安装依赖
来源：http://ntt.jqgfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nse.birdmap.top

[U03] Py：加载 .env 配置
来源：http://uvf.52xcode.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tld.jianghu66.top

[U04] Py：变量调试打印
来源：http://wvq.sjlbkw.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gph.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://qta.sysykeji.top

list(dict.fromkeys(arr))
来源：http://bna.ctjpmb.com

[U06] Py：合并两个字典
来源：http://dhv.jinghuilouyu.cn

{**a, **b}
来源：http://jye.xinyue.icu

[U07] Py：反转字典键值
来源：http://vsa.hysaishi.cn

{v: k for k, v in d.items()}
来源：http://oou.epnwcf.com

[U08] Py：展平二维列表
来源：http://eyp.iojbl.cn

[y for x in nested for y in x]
来源：http://bpp.xuanzx.com

[U09] Py：字典取最大值的键
来源：http://ewe.yvedp.cn

max(d, key=d.get)
来源：http://jwe.zhengqikj.top

[U10] Py：按值排序字典
来源：http://lkq.pengpengdd.cyou

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sdr.shuidangran.top

[U11] Py：生成器表达式
来源：http://frc.0kj1m.cn

(x * 2 for x in arr)
来源：http://ulq.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gar.ehwqpu.com

Counter(arr).most_common(3)
来源：http://xfx.zdqjudy.top

[U13] Py：固定长度队列
来源：http://jdq.zdbjq.cn

deque(maxlen=10)
来源：http://nyu.wangdashe.top

[U14] Py：分组收集到列表
来源：http://vms.quarkkingdee.top

defaultdict(list)
来源：http://rfu.sjlbkw.cn

[U15] Py：高精度计时
来源：http://dnk.jqgufenzy.top

t = time.perf_counter()
来源：http://phw.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://lwr.havefunace.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://omh.jqgufenzy.top

[U17] Py：初始化日志
来源：http://sxx.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://lhd.sysykeji.top

[U18] Py：预编译正则
来源：http://izn.cashguo.top

pat = re.compile(r"\d+")
来源：http://kre.fanxiaobao.xyz

[U19] Py：正则替换带回调
来源：http://kiv.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://scx.sxryk.cn

[U20] Py：缓存函数结果
来源：http://zbz.jinghuilouyu.cn

@functools.lru_cache(maxsize=None)
来源：http://ddt.jqgfzy.top

[U21] Py：自定义上下文管理器
来源：http://bka.aizwys.cn

@contextlib.contextmanager
来源：http://gsc.pycfn.com

[U22] Py：矩阵转置
来源：http://ibf.xziqi.cn

list(zip(*m))
来源：http://qnu.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://puk.hfpthk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xlp.dianchejie.cn

[U24] Py：路径操作
来源：http://sih.hnxiangtu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cuq.bjfxy.top

[U25] Py：CSV 按字典读
来源：http://yen.gaohongyu789.top

csv.DictReader(f)
来源：http://pea.jlsjyb.cn

[U26] Py：并发下载
来源：http://lqs.sysykeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zqd.daria6918.cn

[U27] Py：异步 HTTP
来源：http://fxv.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://bkb.cashguo.top

[U28] Py：类型别名
来源：http://uxe.yuanzhike.top

UserId = int
来源：http://xpw.jqgufenzy.top

[U29] Py：属性校验
来源：http://yyw.fehbvm.com

@property 与 @x.setter 配合
来源：http://lvt.yangfankeji.com

[U30] Py：数据类
来源：http://btm.yvedp.cn

@dataclass(slots=True)
来源：http://sve.hnqzz.top

[U31] Py：单测
来源：http://spa.zdbjq.cn

python -m pytest -q
来源：http://uwz.fktsv.cn

[U32] Py：代码格式化
来源：http://stb.xinyue.icu

ruff format . && ruff check --fix .
来源：http://gaj.hesvh.cn

[U33] Py：打包发布
来源：http://sme.svipenyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://cee.ivvv.top

[U34] Py：判断编码
来源：http://mhr.zhixingplan.top

chardet.detect(raw)
来源：http://itz.hnxiangtu.top

[U35] Py：发送邮件
来源：http://jvr.sweek.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iub.yuanzhike.top

[U36] Py：定时任务
来源：http://rtn.shanyushiyangkeji.top

schedule.every(10).minutes.do(job)
来源：http://xri.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://hce.yueranfly.top

pandas.read_excel / DataFrame.to_excel
来源：http://yyg.0kj1m.cn

[U38] Py：获取脚本所在目录
来源：http://zqb.chenzaomai.com

Path(__file__).resolve().parent
来源：http://dwk.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://qab.yj20258.top

sys.stdout.isatty()
来源：http://xmq.hysaishi.cn

[U40] Py：打印到标准错误
来源：http://vos.nwbrower.top

print("err", file=sys.stderr)
来源：http://sse.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://nmq.fengsongda.top

composer init;  composer require guzzlehttp/guzzle
来源：http://dpo.hammf.cn

[U42] PHP：PSR-4 自动加载
来源：http://iat.ydjk.org.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wky.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://pbh.zhixingplan.top

namespace App\Http;
来源：http://ppb.jinqigfzy.top

[U44] PHP：开启严格类型
来源：http://nsq.yj20258.top

declare(strict_types=1);
来源：http://twc.zhiwuduotai.top

[U45] PHP：类型声明与返回类型
来源：http://ymw.bbcook.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fgv.mhx1999.top

[U46] PHP：可空类型
来源：http://maj.xinyue.icu

?string $name = null
来源：http://snk.ydzc1.top

[U47] PHP：联合类型
来源：http://dcf.jiagoushi.top

int|string $id
来源：http://haf.daxiang520.top

[U48] PHP：纯枚举
来源：http://eoc.dianchejie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hqf.xuetiantiany.cn

[U49] PHP：只读属性
来源：http://wjl.yvedp.cn

public readonly string $name
来源：http://wae.zhixingplan.top

[U50] PHP：构造器属性提升
来源：http://gvi.nanxinkj.top

public function __construct(private int $id) {}
来源：http://uob.jiagoushi.top

[U51] PHP：数组解构
来源：http://wup.snrcjt.cn

[$a, $b] = $arr;
来源：http://fwv.gotoacloud.top

[U52] PHP：箭头函数
来源：http://fjm.yj202588.top

$double = fn($x) => $x * 2;
来源：http://tkg.hnxiangtu.top


<!-- 参考信息 -->