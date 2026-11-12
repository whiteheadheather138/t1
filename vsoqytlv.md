代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ury.guannengcc.top

[S25] C：内存拷贝
来源：http://uri.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://nwc.yueranfly.top

[S26] C：内存清零
来源：http://zma.zhijiandao.cn

memset(a, 0, sizeof a);
来源：http://bcz.gotoacloud.top

[S27] C：定义常量
来源：http://ehg.xingfuxueyuan.xyz

const double PI = 3.14159;
来源：http://xyf.iojbl.cn

[S28] C：静态变量
来源：http://ecy.52xcode.cn

static int counter = 0;
来源：http://krb.hammf.cn

[S29] C：变参函数
来源：http://gqa.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bzk.hnqzz.top

[S30] C：头文件保护
来源：http://jyu.kuanghao11.cn

#ifndef X_H
来源：http://npf.cdnleiting.top

#define X_H
来源：http://ifp.chenlongwang.top

#endif
来源：http://jgg.gaohongyu789.top

[S31] C++：Hello World
来源：http://hdg.316326.xyz

#include <iostream>
来源：http://llo.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://kfh.yonumen.top

[S32] C++：字符串
来源：http://yzg.uphjek.com

std::string s = "hi";  s += "!";
来源：http://oky.jinqigfzy.top

[S33] C++：vector 增删
来源：http://eiv.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qla.hysaishi.cn

[S34] C++：遍历 vector
来源：http://ooj.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://nmw.redwolf501.top

[S35] C++：map
来源：http://vlg.zhoulong.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nlz.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://cdu.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zfd.9152youxi.cn

[S37] C++：set
来源：http://ogn.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fhh.fengsongda.top

[S38] C++：排序
来源：http://gie.sysykeji.top

std::sort(v.begin(), v.end());
来源：http://bqo.zycfv.cn

[S39] C++：自定义比较器排序
来源：http://trc.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://auv.sysykeji.top

[S40] C++：查找元素
来源：http://you.zycfv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rqs.xinyue.icu

[S41] C++：类与构造函数
来源：http://qsn.hnqzz.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uog.yuxming.cn

[S42] C++：继承与虚函数
来源：http://ypp.c1oappe.top

class B : public Base { public: void f() override {} };
来源：http://abq.cdnleiting.top

[S43] C++：智能指针
来源：http://mgw.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://ruu.hywenlv.cn

[S44] C++：引用传参
来源：http://sdj.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://lfc.birdmap.top

[S45] C++：lambda
来源：http://pyx.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://sjx.sweek.top

[S46] C++：函数模板
来源：http://abz.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vrl.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://wxo.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hwb.yuxming.cn

[S48] C++：逐行读文件
来源：http://yzn.jlsjyb.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ewi.jinghuilouyu.cn

while (std::getline(in, line)) { }
来源：http://tfb.dashuyun.cn

[S49] C++：写文件
来源：http://pfy.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yhy.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://vzk.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lwx.vqdsnc.cn

[S51] C++：显式类型转换
来源：http://jhh.jqgufenzy.top

static_cast<double>(a) / b
来源：http://hwz.cqqwz.cn

[S52] C++：const 与 noexcept
来源：http://agz.ybcxt.top

int size() const noexcept { return n_; }
来源：http://qgt.birdmap.top

[S53] C++：移动语义
来源：http://ogs.gotoacloud.top

std::vector<int> w = std::move(v);
来源：http://xgr.nwbrower.top

[S54] C++：异常处理
来源：http://cph.aibaodan.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gcd.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://bpk.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://glh.xuetiantiany.cn

[S56] C++：optional
来源：http://uqg.yanxiufei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pfr.sjlbkw.cn

[S57] C++：编译期常量
来源：http://dhy.hfpthk.cn

constexpr int N = 10;
来源：http://qtl.hongshengwenyu.top

[S58] C++：命名空间
来源：http://aeu.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://eqh.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://yks.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tfl.yj20258.top

[S60] C++：遍历并删除元素
来源：http://cfb.havefunace.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kuz.hnqzz.top

================================================================================
来源：http://bvg.zhixingplan.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hzf.fehbvm.com

================================================================================
来源：http://flp.yfazqb.com

[T01] Kotlin：Hello World
来源：http://leh.shuidangran.top

println("Hello")
来源：http://gxe.hysaishi.cn

[T02] Kotlin：变量
来源：http://znx.smart0.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hnx.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://rmx.chenzaomai.com

"值: $b"
来源：http://opc.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://ujs.snrcjt.cn

val n: String? = null;  n?.length
来源：http://fki.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://lfb.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ebc.yonumen.top

[T06] Kotlin：集合映射
来源：http://ioi.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ykt.316326.xyz

[T07] Kotlin：集合过滤
来源：http://gys.hammf.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xpr.hfpthk.cn

[T08] Kotlin：数据类
来源：http://kef.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://cbf.epnwcf.com

[T09] Kotlin：扩展函数
来源：http://zye.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://sdb.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://isp.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bwh.shanyushiyangkeji.top

[T11] Kotlin：协程
来源：http://xzh.yueranfly.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rsl.shuidangran.top

[T12] Kotlin：解构声明
来源：http://hjg.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://ucx.9152youxi.cn

[T13] Kotlin：只读 Map
来源：http://iae.yuxming.cn

val m = mapOf("a" to 1)
来源：http://fgk.yvedp.cn

[T14] Kotlin：循环
来源：http://hfu.pycfn.com

for (i in 1..10) println(i)
来源：http://vpl.cashguo.top

[T15] Kotlin：接口
来源：http://gjj.tianlin.xyz

interface Shape { fun area(): Double }
来源：http://ssd.snrcjt.cn

[T16] Swift：Hello World
来源：http://kyu.guannengcc.top

print("Hello")
来源：http://ybb.zhijiandao.cn

[T17] Swift：变量与常量
来源：http://ccy.gzhubu.top

var a = 1;  let b = 2
来源：http://ddm.epnwcf.com

[T18] Swift：字符串插值
来源：http://aiv.zycfv.cn

"值: \(b)"
来源：http://sae.smart0.xyz

[T19] Swift：可选绑定
来源：http://rmk.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://syl.shanyushiyangtech.top

[T20] Swift：数组操作
来源：http://lbr.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://psx.yongpay.top

[T21] Swift：遍历
来源：http://gei.hesvh.cn

for x in a { print(x) }
来源：http://kto.snrcjt.cn

[T22] Swift：字典
来源：http://wct.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gkq.bjfxy.top

[T23] Swift：函数
来源：http://vkq.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oea.haohaochexian.top

[T24] Swift：闭包
来源：http://wgh.0kj1m.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://thv.vqdsnc.cn

[T25] Swift：结构体
来源：http://eac.iojbl.cn

struct P { var x: Int }
来源：http://wzs.cqqwz.cn

[T26] Swift：类与重写
来源：http://rfi.smart0.xyz

class A: Base { override func f() {} }
来源：http://gdy.ywan-chungtsiang.top

[T27] Swift：错误处理
来源：http://ijh.guowangkeji.top

do { try f() } catch { print(error) }
来源：http://vfc.c1oappe.top

[T28] Swift：枚举
来源：http://ptn.jinqigfzy.top

enum Color { case red, green }
来源：http://vky.zycfv.cn

[T29] Swift：guard 提前返回
来源：http://abk.52xcode.cn

guard let x = opt else { return }
来源：http://dvd.sjlbkw.cn

[T30] Swift：协议
来源：http://eqx.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://oyl.yuxming.cn

[T31] Lua：Hello World
来源：http://iqj.hammf.cn

print("Hello")
来源：http://zck.yuxming.cn

[T32] Lua：局部变量
来源：http://ofn.tianlin.xyz

local a = 1
来源：http://qqy.nanxuanxn.top

[T33] Lua：表（数组）
来源：http://vyn.shanyushiyangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gtg.xziqi.cn

[T34] Lua：遍历表
来源：http://cqa.iojbl.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ike.yj20258.top

[T35] Lua：字典表
来源：http://vcq.yj20258888.top

local d = { a = 1 };  d.b = 2
来源：http://vzl.0kj1m.cn

[T36] Lua：函数
来源：http://vnk.yueranfly.top

function add(a, b) return a + b end
来源：http://ntd.hesvh.cn

[T37] Lua：字符串拼接
来源：http://hls.cucudq.cn

"a" .. "b"
来源：http://cgf.tian-w.cn

[T38] Lua：条件
来源：http://fwo.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://mlc.jiagoushi.top

[T39] Lua：模式匹配
来源：http://vsh.nwbrower.top

string.find(s, "%d+")
来源：http://tff.yonumen.top

[T40] Lua：元表
来源：http://wcj.hywenlv.cn

setmetatable({}, { __index = base })
来源：http://kjh.c1oappe.top

[T41] Perl：Hello World
来源：http://axu.yfazqb.com

print "Hello\n";
来源：http://kwv.vqdsnc.cn

[T42] Perl：变量类型
来源：http://azb.wangdashe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nga.hcnkem.com

[T43] Perl：字符串插值
来源：http://ykt.hesvh.cn

"值: $a"
来源：http://ohp.tianlin.xyz

[T44] Perl：条件
来源：http://npd.andypj.xyz

if ($a > 0) { print "正"; }
来源：http://bhq.nwbrower.top

[T45] Perl：数组遍历
来源：http://ump.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://epu.zdbjq.cn

[T46] Perl：哈希操作
来源：http://qey.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lnx.0kj1m.cn

[T47] Perl：正则捕获
来源：http://lwr.jiagoushi.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fck.ivvv.top

[T48] Perl：正则替换
来源：http://qzb.cucudq.cn

$s =~ s/old/new/g;
来源：http://tbk.shuidangran.top

[T49] Perl：函数
来源：http://fwa.zdbjq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jai.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://csy.xinyue.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://wbo.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://jxi.svipenyu.cn

[T51] Scala：Hello World
来源：http://yoa.tanke756.top

println("Hello")
来源：http://sfs.hnxiangtu.top

[T52] Scala：变量
来源：http://mpl.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://lkc.xingfuxueyuan.xyz

[T53] Scala：字符串插值
来源：http://wen.tian-w.cn

s"值: $b"
来源：http://wzr.aibaodan.cn

[T54] Scala：集合映射
来源：http://zca.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://rgo.ydzc1.top

[T55] Scala：集合过滤
来源：http://dwp.shzxlz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lpq.gaohongyu789.top

[T56] Scala：样例类
来源：http://slk.vqdsnc.cn

case class User(name: String, age: Int)
来源：http://jfx.yvedp.cn

[T57] Scala：模式匹配
来源：http://oey.tanke756.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://tps.zhiwuduotai.top

[T58] Scala：函数定义
来源：http://tjs.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://erd.uphjek.com

[T59] Scala：循环
来源：http://iih.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://csf.shanyushiyangtech.top

[T60] Scala：折叠
来源：http://hvm.tianlin.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://msf.nwbrower.top

================================================================================
来源：http://jdz.iojbl.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jsm.tian-w.cn

================================================================================
来源：http://yzr.redwolf501.top

[U01] Py：创建虚拟环境
来源：http://vwn.jiagoushi.top

python -m venv .venv && source .venv/bin/activate
来源：http://vle.pengpengdd.cyou

[U02] Py：导出 / 安装依赖
来源：http://gnh.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dzf.meibo888.top

[U03] Py：加载 .env 配置
来源：http://wau.jqgufenzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tto.c1oappe.top

[U04] Py：变量调试打印
来源：http://rlr.tianlin.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wsb.havefunace.top

[U05] Py：列表去重且保序
来源：http://zwz.dianchejie.cn

list(dict.fromkeys(arr))
来源：http://ffw.iojbl.cn

[U06] Py：合并两个字典
来源：http://rsq.zycfv.cn

{**a, **b}
来源：http://xpl.quarkkingdee.top

[U07] Py：反转字典键值
来源：http://ydn.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://rsw.fengsongda.top

[U08] Py：展平二维列表
来源：http://cau.yongpay.top

[y for x in nested for y in x]
来源：http://ypn.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://gbs.yangfankeji.com

max(d, key=d.get)
来源：http://cxm.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://omx.xuetiantiany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rdi.hammf.cn

[U11] Py：生成器表达式
来源：http://azj.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://pqm.yueranfly.top

[U12] Py：取出现最多的 3 个元素
来源：http://rkp.jqgufenzy.top

Counter(arr).most_common(3)
来源：http://sid.nanxinkj.top

[U13] Py：固定长度队列
来源：http://pdt.316326.xyz

deque(maxlen=10)
来源：http://hwg.shanyushiyangtech.top

[U14] Py：分组收集到列表
来源：http://qqo.fanxiaobao.xyz

defaultdict(list)
来源：http://hyj.chenjidiqi.icu

[U15] Py：高精度计时
来源：http://eep.aibaodan.cn

t = time.perf_counter()
来源：http://fml.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://mby.sjlbkw.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gjl.zhixingplan.top

[U17] Py：初始化日志
来源：http://vfr.shanyushiyangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://yii.nwbrower.top

[U18] Py：预编译正则
来源：http://cfw.zhoulong.xyz

pat = re.compile(r"\d+")
来源：http://iru.yfazqb.com

[U19] Py：正则替换带回调
来源：http://ord.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tsv.yj20258.top

[U20] Py：缓存函数结果
来源：http://yve.fzhhl.top

@functools.lru_cache(maxsize=None)
来源：http://kpo.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://rrp.hongshengwenyu.top

@contextlib.contextmanager
来源：http://efy.zhaomingkeji.xyz

[U22] Py：矩阵转置
来源：http://pcy.tian-w.cn

list(zip(*m))
来源：http://nak.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://dhw.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ehc.sufxvd.cn

[U24] Py：路径操作
来源：http://gqa.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ggl.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://jsi.xuanzx.com

csv.DictReader(f)
来源：http://hey.zhiwuduotai.top

[U26] Py：并发下载
来源：http://gux.vehdjk.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kvy.yueranfly.top

[U27] Py：异步 HTTP
来源：http://wwn.ywan-chungtsiang.top

aiohttp.ClientSession() 配合 async with
来源：http://ihm.xziqi.cn

[U28] Py：类型别名
来源：http://acg.yueranfly.top

UserId = int
来源：http://dap.fengsongda.top

[U29] Py：属性校验
来源：http://zer.ivvv.top

@property 与 @x.setter 配合
来源：http://vpi.sysykeji.top

[U30] Py：数据类
来源：http://gsi.ywan-chungtsiang.top

@dataclass(slots=True)
来源：http://skr.bjfxy.top

[U31] Py：单测
来源：http://dpo.c1oappe.top

python -m pytest -q
来源：http://mzq.shuidangran.top

[U32] Py：代码格式化
来源：http://itb.kuanghao11.cn

ruff format . && ruff check --fix .
来源：http://tya.0kj1m.cn

[U33] Py：打包发布
来源：http://osn.jinqigufen.top

python -m build  （依赖 pyproject.toml）
来源：http://gyy.shanyushiyangtech.top

[U34] Py：判断编码
来源：http://tlf.smart0.xyz

chardet.detect(raw)
来源：http://rut.shzxlz.cn

[U35] Py：发送邮件
来源：http://ozh.yueranfly.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://auz.wangdashe.top

[U36] Py：定时任务
来源：http://qzh.yj20258.top

schedule.every(10).minutes.do(job)
来源：http://uej.dashuyun.cn

[U37] Py：读写 Excel
来源：http://sgc.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mlb.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://efo.yfazqb.com

Path(__file__).resolve().parent
来源：http://ado.sweek.top

[U39] Py：判断是否在交互环境
来源：http://hku.gotoacloud.top

sys.stdout.isatty()
来源：http://vsj.xingfuxueyuan.xyz

[U40] Py：打印到标准错误
来源：http://ccb.fzhhl.top

print("err", file=sys.stderr)
来源：http://otm.kuanghao11.cn

[U41] PHP：初始化 Composer 项目
来源：http://egi.aibaodan.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ngg.yuxming.cn

[U42] PHP：PSR-4 自动加载
来源：http://zjr.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ymg.ybcxt.top

[U43] PHP：声明命名空间
来源：http://suy.jinghuilouyu.cn

namespace App\Http;
来源：http://uye.ctjpmb.com

[U44] PHP：开启严格类型
来源：http://jfj.aizwys.cn

declare(strict_types=1);
来源：http://chb.shzxlz.cn

[U45] PHP：类型声明与返回类型
来源：http://wok.jinyuanbaomall.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mht.jqgufenzy.top

[U46] PHP：可空类型
来源：http://rnw.feifeiyinyue.top

?string $name = null
来源：http://esm.cucudq.cn

[U47] PHP：联合类型
来源：http://tno.sxryk.cn

int|string $id
来源：http://zvk.yj20258888.top

[U48] PHP：纯枚举
来源：http://nbg.hnxiangtu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ejq.tian-w.cn


<!-- 参考信息 -->