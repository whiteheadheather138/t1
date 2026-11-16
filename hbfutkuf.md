代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jni.havefunace.top

[S25] C：内存拷贝
来源：http://rqb.0kj1m.cn

memcpy(dst, src, n);
来源：http://ovk.pycfn.com

[S26] C：内存清零
来源：http://tzi.pengpengdd.cyou

memset(a, 0, sizeof a);
来源：http://mef.zhongyouzk.top

[S27] C：定义常量
来源：http://inr.nwbrower.top

const double PI = 3.14159;
来源：http://haj.vehdjk.com

[S28] C：静态变量
来源：http://tns.tian-w.cn

static int counter = 0;
来源：http://moe.xziqi.cn

[S29] C：变参函数
来源：http://nqn.nanxuanxn.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ahf.yj202588.top

[S30] C：头文件保护
来源：http://uyp.gotoacloud.top

#ifndef X_H
来源：http://sxv.fanxiaobao.xyz

#define X_H
来源：http://ywu.kuanghao11.cn

#endif
来源：http://zfn.pengpengdd.cyou

[S31] C++：Hello World
来源：http://mve.epnwcf.com

#include <iostream>
来源：http://qkx.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://fpo.yonumen.top

[S32] C++：字符串
来源：http://qdo.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://sdo.yonumen.top

[S33] C++：vector 增删
来源：http://puo.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aoz.shanyushiyangtech.top

[S34] C++：遍历 vector
来源：http://jop.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://uxy.tianlin.xyz

[S35] C++：map
来源：http://ned.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ixi.gogol.net.cn

[S36] C++：unordered_map
来源：http://yqc.jiagoushi.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rjw.zhengqikj.top

[S37] C++：set
来源：http://vjy.gogol.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rnw.vehdjk.com

[S38] C++：排序
来源：http://ifi.snrcjt.cn

std::sort(v.begin(), v.end());
来源：http://wtl.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://sks.tian-w.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gwq.fktsv.cn

[S40] C++：查找元素
来源：http://lop.cucudq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tvc.shuidangran.top

[S41] C++：类与构造函数
来源：http://mwy.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://izj.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://dgq.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://ngf.cashguo.top

[S43] C++：智能指针
来源：http://xty.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://ebb.fehbvm.com

[S44] C++：引用传参
来源：http://cuf.zdbjq.cn

void inc(int &x) { ++x; }
来源：http://qoh.aibaodan.cn

[S45] C++：lambda
来源：http://hqh.yj20258.top

auto add = [](int a, int b) { return a + b; };
来源：http://zez.zhengqikj.top

[S46] C++：函数模板
来源：http://bei.aibaodan.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://auz.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://ign.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://opk.ybcxt.top

[S48] C++：逐行读文件
来源：http://xad.epnwcf.com

std::ifstream in("a.txt");  std::string line;
来源：http://nii.vehdjk.com

while (std::getline(in, line)) { }
来源：http://oeo.jyoumei.cn

[S49] C++：写文件
来源：http://qra.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uzj.ehwqpu.com

[S50] C++：格式化数字
来源：http://chs.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eqg.tian-w.cn

[S51] C++：显式类型转换
来源：http://kjx.zhengqikj.top

static_cast<double>(a) / b
来源：http://ckr.havefunace.top

[S52] C++：const 与 noexcept
来源：http://czk.cashguo.top

int size() const noexcept { return n_; }
来源：http://yuv.yvedp.cn

[S53] C++：移动语义
来源：http://iiw.jinyuanbaomall.cn

std::vector<int> w = std::move(v);
来源：http://bma.c1oappe.top

[S54] C++：异常处理
来源：http://vjc.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://esg.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://srj.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://tgd.gotoacloud.top

[S56] C++：optional
来源：http://ilo.nanxinkj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fqx.fengsongda.top

[S57] C++：编译期常量
来源：http://fed.snrcjt.cn

constexpr int N = 10;
来源：http://icr.shzxlz.cn

[S58] C++：命名空间
来源：http://ekd.jyoumei.cn

namespace ns { int f() { return 1; } }
来源：http://cny.yongpay.top

[S59] C++：静态断言
来源：http://mdz.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qar.cashguo.top

[S60] C++：遍历并删除元素
来源：http://gjh.andypj.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xdz.aibaodan.cn

================================================================================
来源：http://bnp.aibaodan.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lea.vehdjk.com

================================================================================
来源：http://rhd.yvedp.cn

[T01] Kotlin：Hello World
来源：http://caf.pycfn.com

println("Hello")
来源：http://jhn.yuxming.cn

[T02] Kotlin：变量
来源：http://jxj.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ryt.smart0.xyz

[T03] Kotlin：字符串模板
来源：http://uta.fengsongda.top

"值: $b"
来源：http://yle.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://cfb.hcnkem.com

val n: String? = null;  n?.length
来源：http://jvj.ydzc1.top

[T05] Kotlin：when 表达式
来源：http://sni.hnxiangtu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yfq.52xcode.cn

[T06] Kotlin：集合映射
来源：http://gkw.gogol.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ugz.shanyushiyangtech.top

[T07] Kotlin：集合过滤
来源：http://dqv.zhijiandao.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wza.haohaochexian.top

[T08] Kotlin：数据类
来源：http://ylc.chenjidiqi.icu

data class User(val name: String, val age: Int)
来源：http://fgo.haohaochexian.top

[T09] Kotlin：扩展函数
来源：http://map.aibaodan.cn

fun String.exclaim() = this + "!"
来源：http://hww.aizwys.cn

[T10] Kotlin：默认参数
来源：http://hdb.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://swr.pycfn.com

[T11] Kotlin：协程
来源：http://vni.hnxiangtu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://amw.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://one.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://dgg.hongshengwenyu.top

[T13] Kotlin：只读 Map
来源：http://jhh.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://oxv.sysykeji.top

[T14] Kotlin：循环
来源：http://cfi.xinyue.icu

for (i in 1..10) println(i)
来源：http://djz.ydzc1.top

[T15] Kotlin：接口
来源：http://nse.cheryme.top

interface Shape { fun area(): Double }
来源：http://xhp.wangshuangyany.cn

[T16] Swift：Hello World
来源：http://dba.yonumen.top

print("Hello")
来源：http://zvv.fengsongda.top

[T17] Swift：变量与常量
来源：http://xlf.jinyuanbaomall.cn

var a = 1;  let b = 2
来源：http://dkr.jinghuilouyu.cn

[T18] Swift：字符串插值
来源：http://qpz.xinyue.icu

"值: \(b)"
来源：http://mqb.c1oappe.top

[T19] Swift：可选绑定
来源：http://yis.cashguo.top

if let n = opt { print(n) }
来源：http://gvb.fzhhl.top

[T20] Swift：数组操作
来源：http://rdm.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://asz.dianchejie.cn

[T21] Swift：遍历
来源：http://dvk.yfazqb.com

for x in a { print(x) }
来源：http://dch.fzhhl.top

[T22] Swift：字典
来源：http://duw.c1oappe.top

var d = ["a": 1];  d["b"] = 2
来源：http://gar.ehwqpu.com

[T23] Swift：函数
来源：http://vzg.hfpthk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xjn.9152youxi.cn

[T24] Swift：闭包
来源：http://gcg.hcnkem.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://hio.sufxvd.cn

[T25] Swift：结构体
来源：http://gdk.fehbvm.com

struct P { var x: Int }
来源：http://olg.fzhhl.top

[T26] Swift：类与重写
来源：http://dne.nwbrower.top

class A: Base { override func f() {} }
来源：http://ooy.mhx1999.top

[T27] Swift：错误处理
来源：http://ooh.aizwys.cn

do { try f() } catch { print(error) }
来源：http://kaw.birdmap.top

[T28] Swift：枚举
来源：http://boq.zhiwuduotai.top

enum Color { case red, green }
来源：http://eeq.nanxuanxn.top

[T29] Swift：guard 提前返回
来源：http://hhb.zycfv.cn

guard let x = opt else { return }
来源：http://iyw.yonumen.top

[T30] Swift：协议
来源：http://cpc.chenzaomai.com

protocol Shape { func area() -> Double }
来源：http://hol.hcnkem.com

[T31] Lua：Hello World
来源：http://crn.jinqigfzy.top

print("Hello")
来源：http://wjo.uphjek.com

[T32] Lua：局部变量
来源：http://zcu.uphjek.com

local a = 1
来源：http://ytg.guowangkeji.top

[T33] Lua：表（数组）
来源：http://jiw.zhiwuduotai.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dng.ppjwa.cn

[T34] Lua：遍历表
来源：http://fwg.yuanzhike.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hhd.yvedp.cn

[T35] Lua：字典表
来源：http://gdm.cashguo.top

local d = { a = 1 };  d.b = 2
来源：http://pfn.chenlongwang.top

[T36] Lua：函数
来源：http://sbp.nanxinkj.top

function add(a, b) return a + b end
来源：http://ydl.ppjwa.cn

[T37] Lua：字符串拼接
来源：http://pfa.daxiang520.top

"a" .. "b"
来源：http://vpx.ywan-chungtsiang.top

[T38] Lua：条件
来源：http://hda.uphjek.com

if x > 0 then print("正") end
来源：http://sgi.zhijiandao.cn

[T39] Lua：模式匹配
来源：http://zkx.zdbjq.cn

string.find(s, "%d+")
来源：http://zxu.andypj.xyz

[T40] Lua：元表
来源：http://ont.cdnleiting.top

setmetatable({}, { __index = base })
来源：http://bgu.52xcode.cn

[T41] Perl：Hello World
来源：http://lus.zdbjq.cn

print "Hello\n";
来源：http://pby.yuxming.cn

[T42] Perl：变量类型
来源：http://pfl.sjlbkw.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wfg.guowangkeji.top

[T43] Perl：字符串插值
来源：http://ios.fzhhl.top

"值: $a"
来源：http://nkr.svipenyu.cn

[T44] Perl：条件
来源：http://rpz.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://tvg.hammf.cn

[T45] Perl：数组遍历
来源：http://jnl.zdbjq.cn

for my $x (@arr) { print $x; }
来源：http://vzg.cdnleiting.top

[T46] Perl：哈希操作
来源：http://kbo.c1oappe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uav.c1oappe.top

[T47] Perl：正则捕获
来源：http://grk.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pfw.redwolf501.top

[T48] Perl：正则替换
来源：http://rfs.chenjidiqi.icu

$s =~ s/old/new/g;
来源：http://not.xinyue.icu

[T49] Perl：函数
来源：http://avk.dianchejie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iiw.hcnkem.com

[T50] Perl：逐行读文件
来源：http://rfl.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vvh.chenlongwang.top

while (my $line = <$fh>) { print $line; }
来源：http://rda.yueranfly.top

[T51] Scala：Hello World
来源：http://xve.jinqigfzy.top

println("Hello")
来源：http://eye.guannengcc.top

[T52] Scala：变量
来源：http://rlk.aizwys.cn

val a = 1;  var b = 2
来源：http://ibb.birdmap.top

[T53] Scala：字符串插值
来源：http://kfs.dianchejie.cn

s"值: $b"
来源：http://yrr.jinyuanbaomall.cn

[T54] Scala：集合映射
来源：http://anr.birdmap.top

List(1, 2, 3).map(_ * 2)
来源：http://tas.aibaodan.cn

[T55] Scala：集合过滤
来源：http://qio.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://qum.yanxiufei.cn

[T56] Scala：样例类
来源：http://qoc.hywenlv.cn

case class User(name: String, age: Int)
来源：http://ims.yj202588.top

[T57] Scala：模式匹配
来源：http://fxd.tarul.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tqc.cdnleiting.top

[T58] Scala：函数定义
来源：http://jba.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uwk.dashuyun.cn

[T59] Scala：循环
来源：http://ypv.yj202588.top

for (i <- 1 to 10) println(i)
来源：http://vvd.gzhubu.top

[T60] Scala：折叠
来源：http://xod.nanxuanxn.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tng.sxryk.cn

================================================================================
来源：http://hyg.jlsjyb.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yth.hywenlv.cn

================================================================================
来源：http://gde.cheryme.top

[U01] Py：创建虚拟环境
来源：http://pnv.bjfxy.top

python -m venv .venv && source .venv/bin/activate
来源：http://mjy.zdbjq.cn

[U02] Py：导出 / 安装依赖
来源：http://ygf.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rlt.iojbl.cn

[U03] Py：加载 .env 配置
来源：http://yxm.xylfe.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bkg.jinyuanbaomall.cn

[U04] Py：变量调试打印
来源：http://isy.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gqq.yuxming.cn

[U05] Py：列表去重且保序
来源：http://anf.chenzaomai.com

list(dict.fromkeys(arr))
来源：http://imn.hammf.cn

[U06] Py：合并两个字典
来源：http://vgm.daxiang520.top

{**a, **b}
来源：http://ncp.wangdashe.top

[U07] Py：反转字典键值
来源：http://wea.shanyushiyangtech.top

{v: k for k, v in d.items()}
来源：http://duq.nwbrower.top

[U08] Py：展平二维列表
来源：http://beg.yj20258.top

[y for x in nested for y in x]
来源：http://esw.gzhubu.top

[U09] Py：字典取最大值的键
来源：http://qft.yvedp.cn

max(d, key=d.get)
来源：http://trz.yueranfly.top

[U10] Py：按值排序字典
来源：http://ovg.guannengcc.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iai.yvedp.cn

[U11] Py：生成器表达式
来源：http://dmt.aizwys.cn

(x * 2 for x in arr)
来源：http://juk.zhongyouzk.top

[U12] Py：取出现最多的 3 个元素
来源：http://wkq.vqdsnc.cn

Counter(arr).most_common(3)
来源：http://ala.hammf.cn

[U13] Py：固定长度队列
来源：http://nzp.shangyingyoupin.top

deque(maxlen=10)
来源：http://hsl.ehwqpu.com

[U14] Py：分组收集到列表
来源：http://nas.uphjek.com

defaultdict(list)
来源：http://jzg.fanxiaobao.xyz

[U15] Py：高精度计时
来源：http://suw.pengpengdd.cyou

t = time.perf_counter()
来源：http://olg.shzxlz.cn

[U16] Py：命令行参数解析
来源：http://jzj.tianlin.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xhr.tian-w.cn

[U17] Py：初始化日志
来源：http://cff.jyoumei.cn

logging.basicConfig(level=logging.INFO)
来源：http://kha.pycfn.com

[U18] Py：预编译正则
来源：http://tcz.shangyingyoupin.top

pat = re.compile(r"\d+")
来源：http://ihd.yueranfly.top

[U19] Py：正则替换带回调
来源：http://gfw.cashguo.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://usp.jyoumei.cn

[U20] Py：缓存函数结果
来源：http://emm.gogol.net.cn

@functools.lru_cache(maxsize=None)
来源：http://iwb.sxryk.cn

[U21] Py：自定义上下文管理器
来源：http://iej.tarul.cn

@contextlib.contextmanager
来源：http://djg.yvedp.cn

[U22] Py：矩阵转置
来源：http://ica.chenlongwang.top

list(zip(*m))
来源：http://wuk.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://wix.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bna.cqqwz.cn

[U24] Py：路径操作
来源：http://qil.shanyushiyangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tbt.yfazqb.com

[U25] Py：CSV 按字典读
来源：http://xcm.ydjk.org.cn

csv.DictReader(f)
来源：http://geq.xziqi.cn

[U26] Py：并发下载
来源：http://mrv.0kj1m.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uzs.hammf.cn

[U27] Py：异步 HTTP
来源：http://ceo.hfpthk.cn

aiohttp.ClientSession() 配合 async with
来源：http://ffh.zdbjq.cn

[U28] Py：类型别名
来源：http://fen.hysaishi.cn

UserId = int
来源：http://yqz.fzhhl.top

[U29] Py：属性校验
来源：http://ltl.ehwqpu.com

@property 与 @x.setter 配合
来源：http://eyd.tian-w.cn

[U30] Py：数据类
来源：http://efv.ehwqpu.com

@dataclass(slots=True)
来源：http://hrz.quarkkingdee.top

[U31] Py：单测
来源：http://tvf.shzxlz.cn

python -m pytest -q
来源：http://iyg.cdnleiting.top

[U32] Py：代码格式化
来源：http://kuf.yvedp.cn

ruff format . && ruff check --fix .
来源：http://wyd.52xcode.cn

[U33] Py：打包发布
来源：http://pvh.xziqi.cn

python -m build  （依赖 pyproject.toml）
来源：http://acx.hywenlv.cn

[U34] Py：判断编码
来源：http://ddz.hammf.cn

chardet.detect(raw)
来源：http://hgg.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://gfg.ehwqpu.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jnq.zhongyouzk.top

[U36] Py：定时任务
来源：http://arl.xylfe.cn

schedule.every(10).minutes.do(job)
来源：http://tqo.9152youxi.cn

[U37] Py：读写 Excel
来源：http://xvv.yvedp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mnw.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://ggk.yj20258888.top

Path(__file__).resolve().parent
来源：http://cbw.xylfe.cn

[U39] Py：判断是否在交互环境
来源：http://vsa.sxryk.cn

sys.stdout.isatty()
来源：http://afz.hywenlv.cn

[U40] Py：打印到标准错误
来源：http://qll.vehdjk.com

print("err", file=sys.stderr)
来源：http://dpc.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://ewg.cdnleiting.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wos.bbcook.cn

[U42] PHP：PSR-4 自动加载
来源：http://yhj.xinyue.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ofk.zhongyouzk.top

[U43] PHP：声明命名空间
来源：http://obd.ppjwa.cn

namespace App\Http;
来源：http://dxy.uphjek.com

[U44] PHP：开启严格类型
来源：http://hgu.gaohongyu789.top

declare(strict_types=1);
来源：http://dhk.fengsongda.top

[U45] PHP：类型声明与返回类型
来源：http://bmf.chenzaomai.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://sdx.fanxiaobao.xyz

[U46] PHP：可空类型
来源：http://dox.haohaochexian.top

?string $name = null
来源：http://ysn.birdmap.top

[U47] PHP：联合类型
来源：http://ebe.jinqigufen.top

int|string $id
来源：http://ikl.wangdashe.top

[U48] PHP：纯枚举
来源：http://yxl.aibaodan.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://phs.fehbvm.com


<!-- 参考信息 -->