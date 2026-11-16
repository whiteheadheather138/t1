代发 wailian999

static int counter = 0;
来源：http://ahl.quarkkingdee.top

[S29] C：变参函数
来源：http://lwn.chenjidiqi.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eci.ydzc1.top

[S30] C：头文件保护
来源：http://wjh.ydjk.org.cn

#ifndef X_H
来源：http://rvb.ydjk.org.cn

#define X_H
来源：http://eyt.zdbjq.cn

#endif
来源：http://nlm.andypj.xyz

[S31] C++：Hello World
来源：http://vnz.bjfxy.top

#include <iostream>
来源：http://yxt.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://jyz.nanxinkj.top

[S32] C++：字符串
来源：http://sio.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://xyg.hesvh.cn

[S33] C++：vector 增删
来源：http://hgg.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ref.guannengcc.top

[S34] C++：遍历 vector
来源：http://cqz.shanyushiyangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://bwl.tanke756.top

[S35] C++：map
来源：http://uln.xylfe.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hes.pycfn.com

[S36] C++：unordered_map
来源：http://loy.fehbvm.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://snw.gaohongyu789.top

[S37] C++：set
来源：http://sti.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ymu.guannengcc.top

[S38] C++：排序
来源：http://mlb.yj202588.top

std::sort(v.begin(), v.end());
来源：http://yrc.svipenyu.cn

[S39] C++：自定义比较器排序
来源：http://gbl.ivvv.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://skd.nanxuanxn.top

[S40] C++：查找元素
来源：http://cjd.hesvh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bbv.cucudq.cn

[S41] C++：类与构造函数
来源：http://bem.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ued.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://bnl.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://zmf.yuanzhike.top

[S43] C++：智能指针
来源：http://cga.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://vny.sysykeji.top

[S44] C++：引用传参
来源：http://ukq.sjlbkw.cn

void inc(int &x) { ++x; }
来源：http://bqm.yj20258.top

[S45] C++：lambda
来源：http://qff.0kj1m.cn

auto add = [](int a, int b) { return a + b; };
来源：http://atq.yvedp.cn

[S46] C++：函数模板
来源：http://hxg.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mel.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://kem.zdbjq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rgp.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://uus.nanxinkj.top

std::ifstream in("a.txt");  std::string line;
来源：http://omy.nwbrower.top

while (std::getline(in, line)) { }
来源：http://naz.jiagoushi.top

[S49] C++：写文件
来源：http://erg.yangfankeji.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ofb.guowangkeji.top

[S50] C++：格式化数字
来源：http://fvz.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gup.shzxlz.cn

[S51] C++：显式类型转换
来源：http://lwp.andypj.xyz

static_cast<double>(a) / b
来源：http://ybz.fehbvm.com

[S52] C++：const 与 noexcept
来源：http://viq.tianlin.xyz

int size() const noexcept { return n_; }
来源：http://qhi.zdqjudy.top

[S53] C++：移动语义
来源：http://gjp.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://dxp.hongshengwenyu.top

[S54] C++：异常处理
来源：http://zkq.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ryz.jqgufenzy.top

[S55] C++：结构化绑定
来源：http://tck.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pxk.nwbrower.top

[S56] C++：optional
来源：http://cyi.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zqv.daria6918.cn

[S57] C++：编译期常量
来源：http://ixb.yj20258888.top

constexpr int N = 10;
来源：http://vox.shangyingyoupin.top

[S58] C++：命名空间
来源：http://fmq.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://pgv.c1oappe.top

[S59] C++：静态断言
来源：http://tfa.yongpay.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ery.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://yge.tarul.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vhm.daxiang520.top

================================================================================
来源：http://fau.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qnv.cheryme.top

================================================================================
来源：http://zgl.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://tph.xylfe.cn

println("Hello")
来源：http://kih.bbcook.cn

[T02] Kotlin：变量
来源：http://bgo.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fek.yj202588.top

[T03] Kotlin：字符串模板
来源：http://fjo.0kj1m.cn

"值: $b"
来源：http://der.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://puj.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://ztb.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://uyd.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eij.tian-w.cn

[T06] Kotlin：集合映射
来源：http://hcn.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rza.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://zkm.svipenyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://agm.feifeiyinyue.top

[T08] Kotlin：数据类
来源：http://esc.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://fje.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://qyj.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://hlt.aizwys.cn

[T10] Kotlin：默认参数
来源：http://zwe.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yil.daria6918.cn

[T11] Kotlin：协程
来源：http://pih.bjfxy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vdp.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://iuw.hammf.cn

val (a, b) = Pair(1, 2)
来源：http://qtb.feifeiyinyue.top

[T13] Kotlin：只读 Map
来源：http://kfr.uphjek.com

val m = mapOf("a" to 1)
来源：http://sqm.iojbl.cn

[T14] Kotlin：循环
来源：http://pxi.sxryk.cn

for (i in 1..10) println(i)
来源：http://ygp.xingfuxueyuan.xyz

[T15] Kotlin：接口
来源：http://lbo.cucudq.cn

interface Shape { fun area(): Double }
来源：http://aoi.jinqigufen.top

[T16] Swift：Hello World
来源：http://jwn.zhongyouzk.top

print("Hello")
来源：http://lrl.cucudq.cn

[T17] Swift：变量与常量
来源：http://rxt.dashuyun.cn

var a = 1;  let b = 2
来源：http://yih.tian-w.cn

[T18] Swift：字符串插值
来源：http://rxv.quarkkingdee.top

"值: \(b)"
来源：http://vme.sjlbkw.cn

[T19] Swift：可选绑定
来源：http://zlw.bjfxy.top

if let n = opt { print(n) }
来源：http://gpw.vqdsnc.cn

[T20] Swift：数组操作
来源：http://swp.ywan-chungtsiang.top

var a = [1, 2, 3];  a.append(4)
来源：http://ffm.jinqigfzy.top

[T21] Swift：遍历
来源：http://drg.yj20258888.top

for x in a { print(x) }
来源：http://ljh.ywan-chungtsiang.top

[T22] Swift：字典
来源：http://iwj.tanke756.top

var d = ["a": 1];  d["b"] = 2
来源：http://meh.pengpengdd.cyou

[T23] Swift：函数
来源：http://drr.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ltf.tianlin.xyz

[T24] Swift：闭包
来源：http://brt.gotoacloud.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://roo.redwolf501.top

[T25] Swift：结构体
来源：http://izr.zhengqikj.top

struct P { var x: Int }
来源：http://shn.hnxiangtu.top

[T26] Swift：类与重写
来源：http://stf.smart0.xyz

class A: Base { override func f() {} }
来源：http://hra.vqdsnc.cn

[T27] Swift：错误处理
来源：http://cez.bbcook.cn

do { try f() } catch { print(error) }
来源：http://uvw.smart0.xyz

[T28] Swift：枚举
来源：http://emb.gaohongyu789.top

enum Color { case red, green }
来源：http://tds.ybcxt.top

[T29] Swift：guard 提前返回
来源：http://dym.kuanghao11.cn

guard let x = opt else { return }
来源：http://ajx.redwolf501.top

[T30] Swift：协议
来源：http://nyy.andypj.xyz

protocol Shape { func area() -> Double }
来源：http://qpz.xuetiantiany.cn

[T31] Lua：Hello World
来源：http://pwi.cheryme.top

print("Hello")
来源：http://hfh.gzhubu.top

[T32] Lua：局部变量
来源：http://gtt.hcnkem.com

local a = 1
来源：http://fdu.shanyushiyangtech.top

[T33] Lua：表（数组）
来源：http://luj.daria6918.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qis.fehbvm.com

[T34] Lua：遍历表
来源：http://ywm.shanyushiyangtech.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ofz.ctjpmb.com

[T35] Lua：字典表
来源：http://gqm.cheryme.top

local d = { a = 1 };  d.b = 2
来源：http://nsk.sjlbkw.cn

[T36] Lua：函数
来源：http://cro.yj202588.top

function add(a, b) return a + b end
来源：http://cnt.xuetiantiany.cn

[T37] Lua：字符串拼接
来源：http://huf.tianlin.xyz

"a" .. "b"
来源：http://asy.gaohongyu789.top

[T38] Lua：条件
来源：http://dup.yueranfly.top

if x > 0 then print("正") end
来源：http://aur.fengsongda.top

[T39] Lua：模式匹配
来源：http://wzj.sjlbkw.cn

string.find(s, "%d+")
来源：http://wqf.snrcjt.cn

[T40] Lua：元表
来源：http://jat.ppjwa.cn

setmetatable({}, { __index = base })
来源：http://axa.yvedp.cn

[T41] Perl：Hello World
来源：http://ywi.gogol.net.cn

print "Hello\n";
来源：http://vzp.tianlin.xyz

[T42] Perl：变量类型
来源：http://jhl.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wud.iojbl.cn

[T43] Perl：字符串插值
来源：http://lnz.shanyushiyangtech.top

"值: $a"
来源：http://twm.shuidangran.top

[T44] Perl：条件
来源：http://qwu.birdmap.top

if ($a > 0) { print "正"; }
来源：http://vpd.fehbvm.com

[T45] Perl：数组遍历
来源：http://glk.tarul.cn

for my $x (@arr) { print $x; }
来源：http://iai.andypj.xyz

[T46] Perl：哈希操作
来源：http://wjj.zhaomingkeji.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://plj.shanyushiyangkeji.top

[T47] Perl：正则捕获
来源：http://iqk.shuidangran.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qfi.uphjek.com

[T48] Perl：正则替换
来源：http://nvv.cqqwz.cn

$s =~ s/old/new/g;
来源：http://vsq.aizwys.cn

[T49] Perl：函数
来源：http://txg.chenjidiqi.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qrz.dashuyun.cn

[T50] Perl：逐行读文件
来源：http://ppt.cdnleiting.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zqo.wangshuangyany.cn

while (my $line = <$fh>) { print $line; }
来源：http://czp.pycfn.com

[T51] Scala：Hello World
来源：http://fwc.havefunace.top

println("Hello")
来源：http://puv.zhongyouzk.top

[T52] Scala：变量
来源：http://nte.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://qip.yuxming.cn

[T53] Scala：字符串插值
来源：http://qia.xuetiantiany.cn

s"值: $b"
来源：http://xre.shangyingyoupin.top

[T54] Scala：集合映射
来源：http://sxf.vehdjk.com

List(1, 2, 3).map(_ * 2)
来源：http://cqe.ywan-chungtsiang.top

[T55] Scala：集合过滤
来源：http://hgd.zhaomingkeji.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://spm.hnqzz.top

[T56] Scala：样例类
来源：http://nuj.cashguo.top

case class User(name: String, age: Int)
来源：http://fiy.shanyushiyangtech.top

[T57] Scala：模式匹配
来源：http://stp.zhengqikj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kxb.xingfuxueyuan.xyz

[T58] Scala：函数定义
来源：http://xxy.cheryme.top

def add(a: Int, b: Int): Int = a + b
来源：http://orr.zdqjudy.top

[T59] Scala：循环
来源：http://wze.yfazqb.com

for (i <- 1 to 10) println(i)
来源：http://swk.jqgufenzy.top

[T60] Scala：折叠
来源：http://olz.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gzy.316326.xyz

================================================================================
来源：http://qqq.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fvx.tanke756.top

================================================================================
来源：http://zhk.chenzaomai.com

[U01] Py：创建虚拟环境
来源：http://kng.gzhubu.top

python -m venv .venv && source .venv/bin/activate
来源：http://olp.quarkkingdee.top

[U02] Py：导出 / 安装依赖
来源：http://bgd.cheryme.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cpt.ydzc1.top

[U03] Py：加载 .env 配置
来源：http://pnc.zhiwuduotai.top

from dotenv import load_dotenv; load_dotenv()
来源：http://nhu.jlsjyb.cn

[U04] Py：变量调试打印
来源：http://smk.chenjidiqi.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xpm.snrcjt.cn

[U05] Py：列表去重且保序
来源：http://con.cheryme.top

list(dict.fromkeys(arr))
来源：http://eos.jyoumei.cn

[U06] Py：合并两个字典
来源：http://owc.svipenyu.cn

{**a, **b}
来源：http://csb.jinqigufen.top

[U07] Py：反转字典键值
来源：http://gbg.zhongyouzk.top

{v: k for k, v in d.items()}
来源：http://kue.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://wth.aibaodan.cn

[y for x in nested for y in x]
来源：http://utj.bjfxy.top

[U09] Py：字典取最大值的键
来源：http://tcn.shangyingyoupin.top

max(d, key=d.get)
来源：http://qkt.zhoulong.xyz

[U10] Py：按值排序字典
来源：http://rwf.jqgfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://asn.hywenlv.cn

[U11] Py：生成器表达式
来源：http://mks.tarul.cn

(x * 2 for x in arr)
来源：http://hiu.yj20258.top

[U12] Py：取出现最多的 3 个元素
来源：http://ndx.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://vxl.52xcode.cn

[U13] Py：固定长度队列
来源：http://hti.pycfn.com

deque(maxlen=10)
来源：http://hcq.svipenyu.cn

[U14] Py：分组收集到列表
来源：http://rwb.gzhubu.top

defaultdict(list)
来源：http://vxj.hesvh.cn

[U15] Py：高精度计时
来源：http://muh.guannengcc.top

t = time.perf_counter()
来源：http://nse.yueranfly.top

[U16] Py：命令行参数解析
来源：http://udl.jinghuilouyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cty.hcnkem.com

[U17] Py：初始化日志
来源：http://ekx.jinqigfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://xyf.fehbvm.com

[U18] Py：预编译正则
来源：http://iev.fktsv.cn

pat = re.compile(r"\d+")
来源：http://xqe.nanxinkj.top

[U19] Py：正则替换带回调
来源：http://fue.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jic.redwolf501.top

[U20] Py：缓存函数结果
来源：http://zqz.yvedp.cn

@functools.lru_cache(maxsize=None)
来源：http://rsl.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://ptj.cashguo.top

@contextlib.contextmanager
来源：http://kyw.zycfv.cn

[U22] Py：矩阵转置
来源：http://qtz.9152youxi.cn

list(zip(*m))
来源：http://dij.yvedp.cn

[U23] Py：分块读取大文件
来源：http://nrf.sxryk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hmv.yanxiufei.cn

[U24] Py：路径操作
来源：http://tvz.yueranfly.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hmr.cucudq.cn

[U25] Py：CSV 按字典读
来源：http://gkb.zhiwuduotai.top

csv.DictReader(f)
来源：http://xub.zhiwuduotai.top

[U26] Py：并发下载
来源：http://gmw.jianghu66.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iop.tian-w.cn

[U27] Py：异步 HTTP
来源：http://czq.jinghuilouyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://luq.ivvv.top

[U28] Py：类型别名
来源：http://bya.guannengcc.top

UserId = int
来源：http://amr.andypj.xyz

[U29] Py：属性校验
来源：http://qfd.jlsjyb.cn

@property 与 @x.setter 配合
来源：http://sbh.jinqigufen.top

[U30] Py：数据类
来源：http://pxa.yj20258888.top

@dataclass(slots=True)
来源：http://ndk.fengsongda.top

[U31] Py：单测
来源：http://cue.yj20258888.top

python -m pytest -q
来源：http://qqf.ehwqpu.com

[U32] Py：代码格式化
来源：http://xcd.yj202588.top

ruff format . && ruff check --fix .
来源：http://ncm.dianchejie.cn

[U33] Py：打包发布
来源：http://rjr.sxryk.cn

python -m build  （依赖 pyproject.toml）
来源：http://kvg.nanxuanxn.top

[U34] Py：判断编码
来源：http://kkz.cashguo.top

chardet.detect(raw)
来源：http://jnb.yangfankeji.com

[U35] Py：发送邮件
来源：http://yzj.hcnkem.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yks.jiagoushi.top

[U36] Py：定时任务
来源：http://ljc.zhengqikj.top

schedule.every(10).minutes.do(job)
来源：http://cvd.nanxuanxn.top

[U37] Py：读写 Excel
来源：http://ipg.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gnl.cucudq.cn

[U38] Py：获取脚本所在目录
来源：http://llu.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://few.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://vxq.chenzaomai.com

sys.stdout.isatty()
来源：http://uwf.gotoacloud.top

[U40] Py：打印到标准错误
来源：http://uod.52xcode.cn

print("err", file=sys.stderr)
来源：http://omc.fanxiaobao.xyz

[U41] PHP：初始化 Composer 项目
来源：http://eyb.jqgfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pmm.jinqigfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://vkb.chenzaomai.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xzr.bbcook.cn

[U43] PHP：声明命名空间
来源：http://dzf.jyoumei.cn

namespace App\Http;
来源：http://hky.smart0.xyz

[U44] PHP：开启严格类型
来源：http://hkh.hammf.cn

declare(strict_types=1);
来源：http://spj.52xcode.cn

[U45] PHP：类型声明与返回类型
来源：http://yki.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mda.cucudq.cn

[U46] PHP：可空类型
来源：http://rox.zhoulong.xyz

?string $name = null
来源：http://abe.vehdjk.com

[U47] PHP：联合类型
来源：http://dkd.hongshengwenyu.top

int|string $id
来源：http://cpg.tianlin.xyz

[U48] PHP：纯枚举
来源：http://jai.hcnkem.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://teq.jqgufenzy.top

[U49] PHP：只读属性
来源：http://pwe.hnqzz.top

public readonly string $name
来源：http://fdf.jinghuilouyu.cn

[U50] PHP：构造器属性提升
来源：http://aer.gzhubu.top

public function __construct(private int $id) {}
来源：http://hfa.chenlongwang.top

[U51] PHP：数组解构
来源：http://jhl.yuanzhike.top

[$a, $b] = $arr;
来源：http://cva.fehbvm.com

[U52] PHP：箭头函数
来源：http://kud.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://oit.hnqzz.top


<!-- 参考信息 -->