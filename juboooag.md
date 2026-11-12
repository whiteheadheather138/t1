代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oce.xylfe.cn

[S21] C：字符类别判断
来源：http://eqg.guowangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bdv.cqqwz.cn

[S22] C：字符串转数字
来源：http://hyn.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://yxo.xinyue.icu

[S23] C：随机数
来源：http://tkt.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rlg.haohaochexian.top

[S24] C：获取本地时间
来源：http://kqt.zhengqikj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tiv.fanxiaobao.xyz

[S25] C：内存拷贝
来源：http://eks.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://zsh.hcnkem.com

[S26] C：内存清零
来源：http://acy.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://utv.ydzc1.top

[S27] C：定义常量
来源：http://khr.daxiang520.top

const double PI = 3.14159;
来源：http://bxu.dashuyun.cn

[S28] C：静态变量
来源：http://lmm.52xcode.cn

static int counter = 0;
来源：http://rrt.jinqigufen.top

[S29] C：变参函数
来源：http://ats.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://afi.ctjpmb.com

[S30] C：头文件保护
来源：http://lom.zhiwuduotai.top

#ifndef X_H
来源：http://lfx.fzhhl.top

#define X_H
来源：http://ptd.kuanghao11.cn

#endif
来源：http://jnl.redwolf501.top

[S31] C++：Hello World
来源：http://pxg.hnqzz.top

#include <iostream>
来源：http://rxg.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://gxg.gaohongyu789.top

[S32] C++：字符串
来源：http://cdy.jlsjyb.cn

std::string s = "hi";  s += "!";
来源：http://xvc.andypj.xyz

[S33] C++：vector 增删
来源：http://ngn.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ocy.jinqigfzy.top

[S34] C++：遍历 vector
来源：http://vuk.cheryme.top

for (auto &x : v) { std::cout << x; }
来源：http://tgb.ydjk.org.cn

[S35] C++：map
来源：http://qse.hongshengwenyu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wie.hongshengwenyu.top

[S36] C++：unordered_map
来源：http://kpb.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qvh.birdmap.top

[S37] C++：set
来源：http://bdt.iojbl.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hrw.bbcook.cn

[S38] C++：排序
来源：http://nnn.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://abb.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://wjr.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ndd.316326.xyz

[S40] C++：查找元素
来源：http://hbl.yj20258.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bwo.yfazqb.com

[S41] C++：类与构造函数
来源：http://phe.gzhubu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mjy.xuetiantiany.cn

[S42] C++：继承与虚函数
来源：http://gkg.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://nlz.daxiang520.top

[S43] C++：智能指针
来源：http://izx.mhx1999.top

auto p = std::make_unique<int>(5);
来源：http://ndv.redwolf501.top

[S44] C++：引用传参
来源：http://xcs.gogol.net.cn

void inc(int &x) { ++x; }
来源：http://xjd.yfazqb.com

[S45] C++：lambda
来源：http://qmy.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://ssh.jianghu66.top

[S46] C++：函数模板
来源：http://ioo.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vgb.haohaochexian.top

[S47] C++：结构化绑定遍历
来源：http://ybu.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xgi.52xcode.cn

[S48] C++：逐行读文件
来源：http://ozx.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://jbh.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://jtg.cashguo.top

[S49] C++：写文件
来源：http://dai.sufxvd.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bvl.haohaochexian.top

[S50] C++：格式化数字
来源：http://ezg.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rbz.yongpay.top

[S51] C++：显式类型转换
来源：http://cjq.sweek.top

static_cast<double>(a) / b
来源：http://vku.9152youxi.cn

[S52] C++：const 与 noexcept
来源：http://vvy.gzhubu.top

int size() const noexcept { return n_; }
来源：http://tus.zdqjudy.top

[S53] C++：移动语义
来源：http://jnb.kuanghao11.cn

std::vector<int> w = std::move(v);
来源：http://gpa.hcnkem.com

[S54] C++：异常处理
来源：http://twk.sufxvd.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ino.xuanzx.com

[S55] C++：结构化绑定
来源：http://hrm.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lga.hongshengwenyu.top

[S56] C++：optional
来源：http://vuq.vehdjk.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sar.epnwcf.com

[S57] C++：编译期常量
来源：http://pjc.havefunace.top

constexpr int N = 10;
来源：http://vwf.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://lum.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://kvk.chenzaomai.com

[S59] C++：静态断言
来源：http://fvd.vehdjk.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://etf.jqgufenzy.top

[S60] C++：遍历并删除元素
来源：http://ard.c1oappe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bfy.zhiwuduotai.top

================================================================================
来源：http://jyz.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gua.hysaishi.cn

================================================================================
来源：http://gci.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://hlw.zhaomingkeji.xyz

println("Hello")
来源：http://bsu.andypj.xyz

[T02] Kotlin：变量
来源：http://xhf.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pbz.hammf.cn

[T03] Kotlin：字符串模板
来源：http://ngo.zhoulong.xyz

"值: $b"
来源：http://pwu.jinqigufen.top

[T04] Kotlin：空安全
来源：http://eft.shanyushiyangtech.top

val n: String? = null;  n?.length
来源：http://pqp.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://occ.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hvl.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://zyo.hywenlv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fnz.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://ymo.tanke756.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://guj.cashguo.top

[T08] Kotlin：数据类
来源：http://tee.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://omh.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://tma.ydjk.org.cn

fun String.exclaim() = this + "!"
来源：http://sxj.bjfxy.top

[T10] Kotlin：默认参数
来源：http://jzs.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://adv.cheryme.top

[T11] Kotlin：协程
来源：http://eid.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://civ.yj202588.top

[T12] Kotlin：解构声明
来源：http://upb.hywenlv.cn

val (a, b) = Pair(1, 2)
来源：http://dic.xuanzx.com

[T13] Kotlin：只读 Map
来源：http://wzf.316326.xyz

val m = mapOf("a" to 1)
来源：http://lkl.zdqjudy.top

[T14] Kotlin：循环
来源：http://ufh.smart0.xyz

for (i in 1..10) println(i)
来源：http://qae.yonumen.top

[T15] Kotlin：接口
来源：http://afz.havefunace.top

interface Shape { fun area(): Double }
来源：http://vvq.hongshengwenyu.top

[T16] Swift：Hello World
来源：http://dwp.gotoacloud.top

print("Hello")
来源：http://ciy.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://xbb.zhixingplan.top

var a = 1;  let b = 2
来源：http://twy.jinqigufen.top

[T18] Swift：字符串插值
来源：http://lrx.sjlbkw.cn

"值: \(b)"
来源：http://hws.ydzc1.top

[T19] Swift：可选绑定
来源：http://odb.kuanghao11.cn

if let n = opt { print(n) }
来源：http://jid.fzhhl.top

[T20] Swift：数组操作
来源：http://fbg.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://coh.52xcode.cn

[T21] Swift：遍历
来源：http://jcl.quarkkingdee.top

for x in a { print(x) }
来源：http://yyy.chenlongwang.top

[T22] Swift：字典
来源：http://ybp.0kj1m.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ujt.fehbvm.com

[T23] Swift：函数
来源：http://rlc.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fnr.jinqigufen.top

[T24] Swift：闭包
来源：http://rzj.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://gzr.cucudq.cn

[T25] Swift：结构体
来源：http://rvk.hywenlv.cn

struct P { var x: Int }
来源：http://zav.yuxming.cn

[T26] Swift：类与重写
来源：http://iri.yueranfly.top

class A: Base { override func f() {} }
来源：http://bto.bjfxy.top

[T27] Swift：错误处理
来源：http://jec.xingfuxueyuan.xyz

do { try f() } catch { print(error) }
来源：http://qwb.nwbrower.top

[T28] Swift：枚举
来源：http://utf.snrcjt.cn

enum Color { case red, green }
来源：http://wbx.vqdsnc.cn

[T29] Swift：guard 提前返回
来源：http://lnb.9152youxi.cn

guard let x = opt else { return }
来源：http://xrn.xylfe.cn

[T30] Swift：协议
来源：http://qli.bjfxy.top

protocol Shape { func area() -> Double }
来源：http://cbu.sysykeji.top

[T31] Lua：Hello World
来源：http://xyx.ywan-chungtsiang.top

print("Hello")
来源：http://kmp.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://ubm.fehbvm.com

local a = 1
来源：http://mgz.cdnleiting.top

[T33] Lua：表（数组）
来源：http://bqn.hammf.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bdq.ppjwa.cn

[T34] Lua：遍历表
来源：http://ydm.jianghu66.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dpe.nanxinkj.top

[T35] Lua：字典表
来源：http://wuk.snrcjt.cn

local d = { a = 1 };  d.b = 2
来源：http://xyg.yfazqb.com

[T36] Lua：函数
来源：http://glo.tarul.cn

function add(a, b) return a + b end
来源：http://xab.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://pmi.jinyuanbaomall.cn

"a" .. "b"
来源：http://hbx.guowangkeji.top

[T38] Lua：条件
来源：http://nsm.zhoulong.xyz

if x > 0 then print("正") end
来源：http://drr.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://yys.wangdashe.top

string.find(s, "%d+")
来源：http://gzh.cucudq.cn

[T40] Lua：元表
来源：http://eof.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://ozw.hongshengwenyu.top

[T41] Perl：Hello World
来源：http://gdd.hongshengwenyu.top

print "Hello\n";
来源：http://rvm.ydzc1.top

[T42] Perl：变量类型
来源：http://wtq.hnqzz.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hwt.daria6918.cn

[T43] Perl：字符串插值
来源：http://mqo.xziqi.cn

"值: $a"
来源：http://csz.chenjidiqi.icu

[T44] Perl：条件
来源：http://ljt.jinghuilouyu.cn

if ($a > 0) { print "正"; }
来源：http://ahq.sxryk.cn

[T45] Perl：数组遍历
来源：http://xrm.sjlbkw.cn

for my $x (@arr) { print $x; }
来源：http://xrg.chenlongwang.top

[T46] Perl：哈希操作
来源：http://gdw.chenjidiqi.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tzw.yuanzhike.top

[T47] Perl：正则捕获
来源：http://rdk.cdnleiting.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vux.xziqi.cn

[T48] Perl：正则替换
来源：http://jfe.aizwys.cn

$s =~ s/old/new/g;
来源：http://emh.fengsongda.top

[T49] Perl：函数
来源：http://zcr.sysykeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sxq.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://wpl.cucudq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://efi.daria6918.cn

while (my $line = <$fh>) { print $line; }
来源：http://nkj.epnwcf.com

[T51] Scala：Hello World
来源：http://kbf.daria6918.cn

println("Hello")
来源：http://bnp.ybcxt.top

[T52] Scala：变量
来源：http://mud.cucudq.cn

val a = 1;  var b = 2
来源：http://bws.zdqjudy.top

[T53] Scala：字符串插值
来源：http://jyr.xinyue.icu

s"值: $b"
来源：http://iyh.guannengcc.top

[T54] Scala：集合映射
来源：http://krz.bjfxy.top

List(1, 2, 3).map(_ * 2)
来源：http://nra.zycfv.cn

[T55] Scala：集合过滤
来源：http://kfk.shzxlz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mbi.gotoacloud.top

[T56] Scala：样例类
来源：http://ycg.jqgfzy.top

case class User(name: String, age: Int)
来源：http://cce.andypj.xyz

[T57] Scala：模式匹配
来源：http://dmd.yanxiufei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lpb.daria6918.cn

[T58] Scala：函数定义
来源：http://vgh.aibaodan.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vxl.sufxvd.cn

[T59] Scala：循环
来源：http://ayr.uphjek.com

for (i <- 1 to 10) println(i)
来源：http://lht.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://waz.hywenlv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://knj.316326.xyz

================================================================================
来源：http://itu.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://itb.c1oappe.top

================================================================================
来源：http://lrj.xinyue.icu

[U01] Py：创建虚拟环境
来源：http://vgj.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kpv.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://jmj.52xcode.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://exl.iojbl.cn

[U03] Py：加载 .env 配置
来源：http://dgd.jlsjyb.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cwm.daxiang520.top

[U04] Py：变量调试打印
来源：http://xjg.yfazqb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://etk.fktsv.cn

[U05] Py：列表去重且保序
来源：http://wlg.chenzaomai.com

list(dict.fromkeys(arr))
来源：http://iss.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://znj.gogol.net.cn

{**a, **b}
来源：http://gty.zdbjq.cn

[U07] Py：反转字典键值
来源：http://rvp.jianghu66.top

{v: k for k, v in d.items()}
来源：http://pjh.fehbvm.com

[U08] Py：展平二维列表
来源：http://kcr.yanxiufei.cn

[y for x in nested for y in x]
来源：http://daz.zhixingplan.top

[U09] Py：字典取最大值的键
来源：http://nrw.epnwcf.com

max(d, key=d.get)
来源：http://rhs.feifeiyinyue.top

[U10] Py：按值排序字典
来源：http://ppd.ydzc1.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ipj.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://aku.nwbrower.top

(x * 2 for x in arr)
来源：http://qcq.yuanzhike.top

[U12] Py：取出现最多的 3 个元素
来源：http://ngr.sufxvd.cn

Counter(arr).most_common(3)
来源：http://rju.yongpay.top

[U13] Py：固定长度队列
来源：http://yqp.316326.xyz

deque(maxlen=10)
来源：http://tgd.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://sib.yangfankeji.com

defaultdict(list)
来源：http://wqo.yuanzhike.top

[U15] Py：高精度计时
来源：http://nyi.jinqigufen.top

t = time.perf_counter()
来源：http://nnl.tarul.cn

[U16] Py：命令行参数解析
来源：http://dxu.zdqjudy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zbz.svipenyu.cn

[U17] Py：初始化日志
来源：http://vvv.aibaodan.cn

logging.basicConfig(level=logging.INFO)
来源：http://lqx.ppjwa.cn

[U18] Py：预编译正则
来源：http://pqp.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://ylg.0kj1m.cn

[U19] Py：正则替换带回调
来源：http://tpb.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lqy.zhongyouzk.top

[U20] Py：缓存函数结果
来源：http://tot.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://utz.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://cqj.ehwqpu.com

@contextlib.contextmanager
来源：http://zou.ehwqpu.com

[U22] Py：矩阵转置
来源：http://vud.zhengqikj.top

list(zip(*m))
来源：http://eoc.52xcode.cn

[U23] Py：分块读取大文件
来源：http://wbt.fktsv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://clq.redwolf501.top

[U24] Py：路径操作
来源：http://qll.hnxiangtu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aqe.jiagoushi.top

[U25] Py：CSV 按字典读
来源：http://hhq.jlsjyb.cn

csv.DictReader(f)
来源：http://eik.shanyushiyangkeji.top

[U26] Py：并发下载
来源：http://dkr.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tmv.aizwys.cn

[U27] Py：异步 HTTP
来源：http://qze.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://fxv.jqgufenzy.top

[U28] Py：类型别名
来源：http://qxo.hcnkem.com

UserId = int
来源：http://mac.tarul.cn

[U29] Py：属性校验
来源：http://nyq.gotoacloud.top

@property 与 @x.setter 配合
来源：http://dpc.hammf.cn

[U30] Py：数据类
来源：http://lhl.jinqigfzy.top

@dataclass(slots=True)
来源：http://ymi.redwolf501.top

[U31] Py：单测
来源：http://rbf.aibaodan.cn

python -m pytest -q
来源：http://uhy.zhoulong.xyz

[U32] Py：代码格式化
来源：http://rxa.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://kut.daria6918.cn

[U33] Py：打包发布
来源：http://dup.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://bho.zhaomingkeji.xyz

[U34] Py：判断编码
来源：http://sgk.yvedp.cn

chardet.detect(raw)
来源：http://air.gaohongyu789.top

[U35] Py：发送邮件
来源：http://ffl.tanke756.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://szj.kuanghao11.cn

[U36] Py：定时任务
来源：http://ldn.havefunace.top

schedule.every(10).minutes.do(job)
来源：http://zmv.redwolf501.top

[U37] Py：读写 Excel
来源：http://rqo.hammf.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bha.svipenyu.cn

[U38] Py：获取脚本所在目录
来源：http://daq.vehdjk.com

Path(__file__).resolve().parent
来源：http://kqw.yangfankeji.com

[U39] Py：判断是否在交互环境
来源：http://ijy.meibo888.top

sys.stdout.isatty()
来源：http://gio.sjlbkw.cn

[U40] Py：打印到标准错误
来源：http://gmi.ydjk.org.cn

print("err", file=sys.stderr)
来源：http://hjf.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://sau.vqdsnc.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qlw.gotoacloud.top

[U42] PHP：PSR-4 自动加载
来源：http://ybv.zhixingplan.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pjr.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://obp.cashguo.top

namespace App\Http;
来源：http://age.cashguo.top

[U44] PHP：开启严格类型
来源：http://cei.iojbl.cn

declare(strict_types=1);
来源：http://tpy.sjlbkw.cn


<!-- 参考信息 -->