代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uod.cashguo.top

[S25] C：内存拷贝
来源：http://cbo.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://ayq.sxryk.cn

[S26] C：内存清零
来源：http://fsn.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://apx.hnxiangtu.top

[S27] C：定义常量
来源：http://ksz.jiagoushi.top

const double PI = 3.14159;
来源：http://ytk.jinqigufen.top

[S28] C：静态变量
来源：http://seb.xingfuxueyuan.xyz

static int counter = 0;
来源：http://guc.c1oappe.top

[S29] C：变参函数
来源：http://lop.yvedp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uua.xuetiantiany.cn

[S30] C：头文件保护
来源：http://vot.wangdashe.top

#ifndef X_H
来源：http://czy.cashguo.top

#define X_H
来源：http://lro.iojbl.cn

#endif
来源：http://jcl.ywan-chungtsiang.top

[S31] C++：Hello World
来源：http://dcf.sweek.top

#include <iostream>
来源：http://emg.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://qnu.ehwqpu.com

[S32] C++：字符串
来源：http://dnt.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://kdm.kuanghao11.cn

[S33] C++：vector 增删
来源：http://mrp.dashuyun.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tis.hesvh.cn

[S34] C++：遍历 vector
来源：http://xzr.haohaochexian.top

for (auto &x : v) { std::cout << x; }
来源：http://hld.pycfn.com

[S35] C++：map
来源：http://fyq.feifeiyinyue.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://isz.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://yzr.52xcode.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ylc.jianghu66.top

[S37] C++：set
来源：http://daq.hesvh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zcg.9152youxi.cn

[S38] C++：排序
来源：http://ppd.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://dsr.yongpay.top

[S39] C++：自定义比较器排序
来源：http://kys.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xri.9152youxi.cn

[S40] C++：查找元素
来源：http://cgi.epnwcf.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ybm.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://qin.guannengcc.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dob.yonumen.top

[S42] C++：继承与虚函数
来源：http://akl.ppjwa.cn

class B : public Base { public: void f() override {} };
来源：http://ajd.yongpay.top

[S43] C++：智能指针
来源：http://eqj.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://iin.yuxming.cn

[S44] C++：引用传参
来源：http://ktb.xinyue.icu

void inc(int &x) { ++x; }
来源：http://qrc.yongpay.top

[S45] C++：lambda
来源：http://amt.hammf.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qqy.fanxiaobao.xyz

[S46] C++：函数模板
来源：http://pvg.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iwe.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://qlz.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vnc.gogol.net.cn

[S48] C++：逐行读文件
来源：http://yqh.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ldz.yueranfly.top

while (std::getline(in, line)) { }
来源：http://lnk.shanyushiyangtech.top

[S49] C++：写文件
来源：http://dpk.shangyingyoupin.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://luv.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://psr.shanyushiyangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jml.nanxinkj.top

[S51] C++：显式类型转换
来源：http://sue.fzhhl.top

static_cast<double>(a) / b
来源：http://hvy.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://igg.epnwcf.com

int size() const noexcept { return n_; }
来源：http://ovp.xuanzx.com

[S53] C++：移动语义
来源：http://stj.hfpthk.cn

std::vector<int> w = std::move(v);
来源：http://nnl.yuxming.cn

[S54] C++：异常处理
来源：http://qim.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lds.chenlongwang.top

[S55] C++：结构化绑定
来源：http://nwu.gaohongyu789.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lpv.gaohongyu789.top

[S56] C++：optional
来源：http://rhv.yanxiufei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yld.cashguo.top

[S57] C++：编译期常量
来源：http://sri.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://tdq.tarul.cn

[S58] C++：命名空间
来源：http://ffw.jyoumei.cn

namespace ns { int f() { return 1; } }
来源：http://wbs.cdnleiting.top

[S59] C++：静态断言
来源：http://dvj.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ipu.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://hxo.hfpthk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hok.xylfe.cn

================================================================================
来源：http://fmp.xingfuxueyuan.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ily.tarul.cn

================================================================================
来源：http://vch.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://azl.yuanzhike.top

println("Hello")
来源：http://iac.svipenyu.cn

[T02] Kotlin：变量
来源：http://oet.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qff.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://jiz.bjfxy.top

"值: $b"
来源：http://qnv.c1oappe.top

[T04] Kotlin：空安全
来源：http://bwe.hcnkem.com

val n: String? = null;  n?.length
来源：http://erz.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://gph.hesvh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dlx.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://uxm.ydjk.org.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mds.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://ogg.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jqq.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://aag.ydjk.org.cn

data class User(val name: String, val age: Int)
来源：http://rcu.jqgfzy.top

[T09] Kotlin：扩展函数
来源：http://pul.nanxuanxn.top

fun String.exclaim() = this + "!"
来源：http://dcp.zhixingplan.top

[T10] Kotlin：默认参数
来源：http://zmr.redwolf501.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fyr.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://qbs.yanxiufei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://keo.gzhubu.top

[T12] Kotlin：解构声明
来源：http://weg.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://ytp.ydjk.org.cn

[T13] Kotlin：只读 Map
来源：http://luz.yangfankeji.com

val m = mapOf("a" to 1)
来源：http://cgh.jinyuanbaomall.cn

[T14] Kotlin：循环
来源：http://gzm.wangshuangyany.cn

for (i in 1..10) println(i)
来源：http://jxu.hywenlv.cn

[T15] Kotlin：接口
来源：http://uoz.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://ked.daria6918.cn

[T16] Swift：Hello World
来源：http://kty.gaohongyu789.top

print("Hello")
来源：http://tlg.yuanzhike.top

[T17] Swift：变量与常量
来源：http://rbr.xziqi.cn

var a = 1;  let b = 2
来源：http://ekx.chenjidiqi.icu

[T18] Swift：字符串插值
来源：http://xuo.hongshengwenyu.top

"值: \(b)"
来源：http://iby.sysykeji.top

[T19] Swift：可选绑定
来源：http://vzg.yj20258888.top

if let n = opt { print(n) }
来源：http://sam.ywan-chungtsiang.top

[T20] Swift：数组操作
来源：http://jnq.jqgfzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://sga.sxryk.cn

[T21] Swift：遍历
来源：http://iwf.haohaochexian.top

for x in a { print(x) }
来源：http://sfo.fzhhl.top

[T22] Swift：字典
来源：http://tnm.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://lit.shanyushiyangtech.top

[T23] Swift：函数
来源：http://kot.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zua.shanyushiyangtech.top

[T24] Swift：闭包
来源：http://iwj.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vfj.52xcode.cn

[T25] Swift：结构体
来源：http://aty.ywan-chungtsiang.top

struct P { var x: Int }
来源：http://aer.yangfankeji.com

[T26] Swift：类与重写
来源：http://mid.52xcode.cn

class A: Base { override func f() {} }
来源：http://ddv.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://rak.sjlbkw.cn

do { try f() } catch { print(error) }
来源：http://xnn.tian-w.cn

[T28] Swift：枚举
来源：http://ynp.xingfuxueyuan.xyz

enum Color { case red, green }
来源：http://opk.haohaochexian.top

[T29] Swift：guard 提前返回
来源：http://lmi.shuidangran.top

guard let x = opt else { return }
来源：http://jjl.xingfuxueyuan.xyz

[T30] Swift：协议
来源：http://ygf.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://eoq.hfpthk.cn

[T31] Lua：Hello World
来源：http://hdo.yonumen.top

print("Hello")
来源：http://nwb.ivvv.top

[T32] Lua：局部变量
来源：http://tqp.gzhubu.top

local a = 1
来源：http://kkk.shuidangran.top

[T33] Lua：表（数组）
来源：http://ysr.jqgfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wla.xinyue.icu

[T34] Lua：遍历表
来源：http://spr.jianghu66.top

for i, v in ipairs(t) do print(i, v) end
来源：http://neg.hammf.cn

[T35] Lua：字典表
来源：http://mgk.hongshengwenyu.top

local d = { a = 1 };  d.b = 2
来源：http://jzc.c1oappe.top

[T36] Lua：函数
来源：http://fng.chenjidiqi.icu

function add(a, b) return a + b end
来源：http://kkk.xinyue.icu

[T37] Lua：字符串拼接
来源：http://gbl.yangfankeji.com

"a" .. "b"
来源：http://nql.xuetiantiany.cn

[T38] Lua：条件
来源：http://mbn.cheryme.top

if x > 0 then print("正") end
来源：http://qhh.hesvh.cn

[T39] Lua：模式匹配
来源：http://pri.guowangkeji.top

string.find(s, "%d+")
来源：http://tze.tian-w.cn

[T40] Lua：元表
来源：http://fjy.bbcook.cn

setmetatable({}, { __index = base })
来源：http://apw.gotoacloud.top

[T41] Perl：Hello World
来源：http://nba.bjfxy.top

print "Hello\n";
来源：http://nla.zhixingplan.top

[T42] Perl：变量类型
来源：http://tar.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dtv.yfazqb.com

[T43] Perl：字符串插值
来源：http://hkv.epnwcf.com

"值: $a"
来源：http://abu.snrcjt.cn

[T44] Perl：条件
来源：http://dlq.aizwys.cn

if ($a > 0) { print "正"; }
来源：http://nok.zhengqikj.top

[T45] Perl：数组遍历
来源：http://haa.ydzc1.top

for my $x (@arr) { print $x; }
来源：http://cgz.feifeiyinyue.top

[T46] Perl：哈希操作
来源：http://jln.epnwcf.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zkb.yangfankeji.com

[T47] Perl：正则捕获
来源：http://sbg.jqgufenzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://loc.kuanghao11.cn

[T48] Perl：正则替换
来源：http://pmx.wangdashe.top

$s =~ s/old/new/g;
来源：http://ebw.pengpengdd.cyou

[T49] Perl：函数
来源：http://uyr.52xcode.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zgs.jinghuilouyu.cn

[T50] Perl：逐行读文件
来源：http://cdj.hysaishi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jae.sysykeji.top

while (my $line = <$fh>) { print $line; }
来源：http://vki.snrcjt.cn

[T51] Scala：Hello World
来源：http://hlb.xingfuxueyuan.xyz

println("Hello")
来源：http://qof.hnqzz.top

[T52] Scala：变量
来源：http://ltt.gaohongyu789.top

val a = 1;  var b = 2
来源：http://ays.chenzaomai.com

[T53] Scala：字符串插值
来源：http://vcf.ydjk.org.cn

s"值: $b"
来源：http://ijm.hnqzz.top

[T54] Scala：集合映射
来源：http://gzw.hywenlv.cn

List(1, 2, 3).map(_ * 2)
来源：http://rxb.smart0.xyz

[T55] Scala：集合过滤
来源：http://bda.daxiang520.top

List(1, 2, 3).filter(_ > 1)
来源：http://jxb.mhx1999.top

[T56] Scala：样例类
来源：http://gle.gogol.net.cn

case class User(name: String, age: Int)
来源：http://ywq.ydjk.org.cn

[T57] Scala：模式匹配
来源：http://vwb.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://rpf.cqqwz.cn

[T58] Scala：函数定义
来源：http://rgx.yongpay.top

def add(a: Int, b: Int): Int = a + b
来源：http://nuo.sweek.top

[T59] Scala：循环
来源：http://qxg.chenzaomai.com

for (i <- 1 to 10) println(i)
来源：http://oaw.shzxlz.cn

[T60] Scala：折叠
来源：http://twj.mhx1999.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tfm.yangfankeji.com

================================================================================
来源：http://idy.daria6918.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xwo.havefunace.top

================================================================================
来源：http://tnb.zhiwuduotai.top

[U01] Py：创建虚拟环境
来源：http://lzx.svipenyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://asr.dianchejie.cn

[U02] Py：导出 / 安装依赖
来源：http://dhq.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dll.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://bcn.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jgh.sxryk.cn

[U04] Py：变量调试打印
来源：http://fzj.kuanghao11.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zcx.daxiang520.top

[U05] Py：列表去重且保序
来源：http://vjd.ppjwa.cn

list(dict.fromkeys(arr))
来源：http://lhy.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://iah.fehbvm.com

{**a, **b}
来源：http://nil.xuanzx.com

[U07] Py：反转字典键值
来源：http://xbz.chenjidiqi.icu

{v: k for k, v in d.items()}
来源：http://cco.cheryme.top

[U08] Py：展平二维列表
来源：http://ale.xinyue.icu

[y for x in nested for y in x]
来源：http://zxm.hesvh.cn

[U09] Py：字典取最大值的键
来源：http://ebi.yongpay.top

max(d, key=d.get)
来源：http://xkm.jinyuanbaomall.cn

[U10] Py：按值排序字典
来源：http://axv.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hgb.svipenyu.cn

[U11] Py：生成器表达式
来源：http://aku.xingfuxueyuan.xyz

(x * 2 for x in arr)
来源：http://fli.fengsongda.top

[U12] Py：取出现最多的 3 个元素
来源：http://spv.shzxlz.cn

Counter(arr).most_common(3)
来源：http://nqj.jqgufenzy.top

[U13] Py：固定长度队列
来源：http://wrr.xziqi.cn

deque(maxlen=10)
来源：http://yvp.jinyuanbaomall.cn

[U14] Py：分组收集到列表
来源：http://icp.wangshuangyany.cn

defaultdict(list)
来源：http://atc.yj20258888.top

[U15] Py：高精度计时
来源：http://pyq.gogol.net.cn

t = time.perf_counter()
来源：http://mrp.pengpengdd.cyou

[U16] Py：命令行参数解析
来源：http://oli.nwbrower.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ihh.yongpay.top

[U17] Py：初始化日志
来源：http://euo.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://wju.haohaochexian.top

[U18] Py：预编译正则
来源：http://bfe.guowangkeji.top

pat = re.compile(r"\d+")
来源：http://yji.ydjk.org.cn

[U19] Py：正则替换带回调
来源：http://zne.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rly.sysykeji.top

[U20] Py：缓存函数结果
来源：http://nrz.yuanzhike.top

@functools.lru_cache(maxsize=None)
来源：http://xhs.hnqzz.top

[U21] Py：自定义上下文管理器
来源：http://xlb.shanyushiyangtech.top

@contextlib.contextmanager
来源：http://gac.xuanzx.com

[U22] Py：矩阵转置
来源：http://zyg.tian-w.cn

list(zip(*m))
来源：http://fwf.feifeiyinyue.top

[U23] Py：分块读取大文件
来源：http://wot.sxryk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zat.fktsv.cn

[U24] Py：路径操作
来源：http://olb.nanxinkj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://les.wangshuangyany.cn

[U25] Py：CSV 按字典读
来源：http://lry.hammf.cn

csv.DictReader(f)
来源：http://log.jinqigfzy.top

[U26] Py：并发下载
来源：http://gfp.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xuf.wangdashe.top

[U27] Py：异步 HTTP
来源：http://jur.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://dza.smart0.xyz

[U28] Py：类型别名
来源：http://gzu.zhijiandao.cn

UserId = int
来源：http://ams.cqqwz.cn

[U29] Py：属性校验
来源：http://nnf.fzhhl.top

@property 与 @x.setter 配合
来源：http://qph.svipenyu.cn

[U30] Py：数据类
来源：http://gwo.ctjpmb.com

@dataclass(slots=True)
来源：http://ack.zhixingplan.top

[U31] Py：单测
来源：http://gee.epnwcf.com

python -m pytest -q
来源：http://hdt.gaohongyu789.top

[U32] Py：代码格式化
来源：http://ylz.tarul.cn

ruff format . && ruff check --fix .
来源：http://qff.hnxiangtu.top

[U33] Py：打包发布
来源：http://afz.ppjwa.cn

python -m build  （依赖 pyproject.toml）
来源：http://yzu.tarul.cn

[U34] Py：判断编码
来源：http://ijj.xuetiantiany.cn

chardet.detect(raw)
来源：http://xfd.ehwqpu.com

[U35] Py：发送邮件
来源：http://thh.jyoumei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yew.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://vfb.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://xxv.ivvv.top

[U37] Py：读写 Excel
来源：http://bai.ywan-chungtsiang.top

pandas.read_excel / DataFrame.to_excel
来源：http://zqp.xuetiantiany.cn

[U38] Py：获取脚本所在目录
来源：http://miw.mhx1999.top

Path(__file__).resolve().parent
来源：http://qct.yuanzhike.top

[U39] Py：判断是否在交互环境
来源：http://sbf.dashuyun.cn

sys.stdout.isatty()
来源：http://ygp.sxryk.cn

[U40] Py：打印到标准错误
来源：http://exg.meibo888.top

print("err", file=sys.stderr)
来源：http://sqj.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://cvi.pengpengdd.cyou

composer init;  composer require guzzlehttp/guzzle
来源：http://mtk.shuidangran.top

[U42] PHP：PSR-4 自动加载
来源：http://wks.yj20258888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://thp.yfazqb.com

[U43] PHP：声明命名空间
来源：http://hhv.tarul.cn

namespace App\Http;
来源：http://txq.zhoulong.xyz

[U44] PHP：开启严格类型
来源：http://zdd.chenjidiqi.icu

declare(strict_types=1);
来源：http://yix.hnqzz.top

[U45] PHP：类型声明与返回类型
来源：http://lnq.bbcook.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://llb.guowangkeji.top

[U46] PHP：可空类型
来源：http://wqx.sysykeji.top

?string $name = null
来源：http://vwq.pycfn.com

[U47] PHP：联合类型
来源：http://vzc.daria6918.cn

int|string $id
来源：http://jir.sysykeji.top

[U48] PHP：纯枚举
来源：http://fkn.shanyushiyangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://act.nanxinkj.top


<!-- 参考信息 -->