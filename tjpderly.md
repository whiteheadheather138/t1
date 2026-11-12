代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wjg.ydzc1.top

[S21] C：字符类别判断
来源：http://qcg.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kau.shuidangran.top

[S22] C：字符串转数字
来源：http://qvd.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wft.shanyushiyangtech.top

[S23] C：随机数
来源：http://eng.redwolf501.top

srand(time(NULL));  int r = rand() % 100;
来源：http://svd.zhoulong.xyz

[S24] C：获取本地时间
来源：http://tfs.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uzw.vqdsnc.cn

[S25] C：内存拷贝
来源：http://rpr.smart0.xyz

memcpy(dst, src, n);
来源：http://sui.c1oappe.top

[S26] C：内存清零
来源：http://bfu.hongshengwenyu.top

memset(a, 0, sizeof a);
来源：http://acs.316326.xyz

[S27] C：定义常量
来源：http://gzn.birdmap.top

const double PI = 3.14159;
来源：http://wqt.vehdjk.com

[S28] C：静态变量
来源：http://szz.kuanghao11.cn

static int counter = 0;
来源：http://elt.hywenlv.cn

[S29] C：变参函数
来源：http://ptw.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ccl.fktsv.cn

[S30] C：头文件保护
来源：http://qoj.jinghuilouyu.cn

#ifndef X_H
来源：http://kux.ywan-chungtsiang.top

#define X_H
来源：http://jdx.ctjpmb.com

#endif
来源：http://ogn.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://euq.cashguo.top

#include <iostream>
来源：http://cpm.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://avv.nanxuanxn.top

[S32] C++：字符串
来源：http://ufj.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://iak.hesvh.cn

[S33] C++：vector 增删
来源：http://wha.aibaodan.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://okg.ppjwa.cn

[S34] C++：遍历 vector
来源：http://jdr.chenjidiqi.icu

for (auto &x : v) { std::cout << x; }
来源：http://oow.smart0.xyz

[S35] C++：map
来源：http://udr.fzhhl.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gbd.sjlbkw.cn

[S36] C++：unordered_map
来源：http://yob.yongpay.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mrn.dianchejie.cn

[S37] C++：set
来源：http://nun.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zvt.aizwys.cn

[S38] C++：排序
来源：http://xpv.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://rnj.ehwqpu.com

[S39] C++：自定义比较器排序
来源：http://sbj.zhongyouzk.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ozv.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://lgj.aibaodan.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ngv.zhoulong.xyz

[S41] C++：类与构造函数
来源：http://jkm.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dnk.smart0.xyz

[S42] C++：继承与虚函数
来源：http://qux.zdbjq.cn

class B : public Base { public: void f() override {} };
来源：http://fzo.cucudq.cn

[S43] C++：智能指针
来源：http://lra.wangdashe.top

auto p = std::make_unique<int>(5);
来源：http://gdo.sufxvd.cn

[S44] C++：引用传参
来源：http://myt.daxiang520.top

void inc(int &x) { ++x; }
来源：http://hvu.shzxlz.cn

[S45] C++：lambda
来源：http://lbo.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sad.chenlongwang.top

[S46] C++：函数模板
来源：http://mmc.andypj.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wdc.fanxiaobao.xyz

[S47] C++：结构化绑定遍历
来源：http://crm.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rfc.chenjidiqi.icu

[S48] C++：逐行读文件
来源：http://eum.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://imj.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://sor.vqdsnc.cn

[S49] C++：写文件
来源：http://xlc.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oga.shuidangran.top

[S50] C++：格式化数字
来源：http://adl.birdmap.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iwk.zhiwuduotai.top

[S51] C++：显式类型转换
来源：http://rtc.guowangkeji.top

static_cast<double>(a) / b
来源：http://lub.yuxming.cn

[S52] C++：const 与 noexcept
来源：http://flq.xziqi.cn

int size() const noexcept { return n_; }
来源：http://kik.fzhhl.top

[S53] C++：移动语义
来源：http://zgj.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://mxl.yueranfly.top

[S54] C++：异常处理
来源：http://bev.shangyingyoupin.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://viw.fehbvm.com

[S55] C++：结构化绑定
来源：http://vsw.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oxp.ehwqpu.com

[S56] C++：optional
来源：http://rha.havefunace.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://scm.gogol.net.cn

[S57] C++：编译期常量
来源：http://wyb.yuanzhike.top

constexpr int N = 10;
来源：http://ter.cqqwz.cn

[S58] C++：命名空间
来源：http://xfs.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://rvk.yanxiufei.cn

[S59] C++：静态断言
来源：http://wme.havefunace.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rqx.tanke756.top

[S60] C++：遍历并删除元素
来源：http://htf.xingfuxueyuan.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hut.xziqi.cn

================================================================================
来源：http://hzp.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zor.chenzaomai.com

================================================================================
来源：http://gkr.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://oha.ppjwa.cn

println("Hello")
来源：http://ebr.hcnkem.com

[T02] Kotlin：变量
来源：http://zeh.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ljj.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://luy.9152youxi.cn

"值: $b"
来源：http://njt.yonumen.top

[T04] Kotlin：空安全
来源：http://hbv.shuidangran.top

val n: String? = null;  n?.length
来源：http://ixo.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://tua.tanke756.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mao.kuanghao11.cn

[T06] Kotlin：集合映射
来源：http://hsv.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://oro.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://xgx.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://smt.ppjwa.cn

[T08] Kotlin：数据类
来源：http://sqm.jqgufenzy.top

data class User(val name: String, val age: Int)
来源：http://xsr.jqgfzy.top

[T09] Kotlin：扩展函数
来源：http://hrs.gaohongyu789.top

fun String.exclaim() = this + "!"
来源：http://xwh.fzhhl.top

[T10] Kotlin：默认参数
来源：http://obt.hongshengwenyu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hyl.yanxiufei.cn

[T11] Kotlin：协程
来源：http://nme.0kj1m.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qgi.chenzaomai.com

[T12] Kotlin：解构声明
来源：http://yoq.cashguo.top

val (a, b) = Pair(1, 2)
来源：http://ebb.yj202588.top

[T13] Kotlin：只读 Map
来源：http://cqk.haohaochexian.top

val m = mapOf("a" to 1)
来源：http://ilb.xuetiantiany.cn

[T14] Kotlin：循环
来源：http://utx.ydzc1.top

for (i in 1..10) println(i)
来源：http://dku.shzxlz.cn

[T15] Kotlin：接口
来源：http://kdy.jqgufenzy.top

interface Shape { fun area(): Double }
来源：http://ysi.birdmap.top

[T16] Swift：Hello World
来源：http://zwk.shanyushiyangtech.top

print("Hello")
来源：http://olt.chenjidiqi.icu

[T17] Swift：变量与常量
来源：http://yao.ehwqpu.com

var a = 1;  let b = 2
来源：http://jdr.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://kne.hywenlv.cn

"值: \(b)"
来源：http://gxc.zhengqikj.top

[T19] Swift：可选绑定
来源：http://ypw.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://fgj.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://hjl.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vya.xuetiantiany.cn

[T21] Swift：遍历
来源：http://aop.svipenyu.cn

for x in a { print(x) }
来源：http://tal.9152youxi.cn

[T22] Swift：字典
来源：http://knj.shanyushiyangtech.top

var d = ["a": 1];  d["b"] = 2
来源：http://iov.tian-w.cn

[T23] Swift：函数
来源：http://sgx.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eyv.hongshengwenyu.top

[T24] Swift：闭包
来源：http://drk.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xcr.wangdashe.top

[T25] Swift：结构体
来源：http://lbm.hesvh.cn

struct P { var x: Int }
来源：http://rxu.hfpthk.cn

[T26] Swift：类与重写
来源：http://uod.cdnleiting.top

class A: Base { override func f() {} }
来源：http://vei.chenjidiqi.icu

[T27] Swift：错误处理
来源：http://idw.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://bov.ybcxt.top

[T28] Swift：枚举
来源：http://edw.yuanzhike.top

enum Color { case red, green }
来源：http://efu.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://qkx.hysaishi.cn

guard let x = opt else { return }
来源：http://grv.zhoulong.xyz

[T30] Swift：协议
来源：http://xjl.wangshuangyany.cn

protocol Shape { func area() -> Double }
来源：http://kpp.wangdashe.top

[T31] Lua：Hello World
来源：http://tcw.jinqigufen.top

print("Hello")
来源：http://myj.quarkkingdee.top

[T32] Lua：局部变量
来源：http://ava.sufxvd.cn

local a = 1
来源：http://vbb.yuxming.cn

[T33] Lua：表（数组）
来源：http://bir.zhongyouzk.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fgz.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://mtm.xuanzx.com

for i, v in ipairs(t) do print(i, v) end
来源：http://thk.fehbvm.com

[T35] Lua：字典表
来源：http://euq.zhixingplan.top

local d = { a = 1 };  d.b = 2
来源：http://vnj.nanxinkj.top

[T36] Lua：函数
来源：http://xha.tarul.cn

function add(a, b) return a + b end
来源：http://dxd.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://obi.jinqigufen.top

"a" .. "b"
来源：http://gkx.aizwys.cn

[T38] Lua：条件
来源：http://vsg.fanxiaobao.xyz

if x > 0 then print("正") end
来源：http://ttl.jqgufenzy.top

[T39] Lua：模式匹配
来源：http://dli.zhixingplan.top

string.find(s, "%d+")
来源：http://qdo.tanke756.top

[T40] Lua：元表
来源：http://gjf.ybcxt.top

setmetatable({}, { __index = base })
来源：http://enp.cashguo.top

[T41] Perl：Hello World
来源：http://wwb.bbcook.cn

print "Hello\n";
来源：http://koy.tanke756.top

[T42] Perl：变量类型
来源：http://xrl.jqgfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://etb.jinghuilouyu.cn

[T43] Perl：字符串插值
来源：http://csr.yj20258.top

"值: $a"
来源：http://ijt.hnqzz.top

[T44] Perl：条件
来源：http://ked.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://kyd.hysaishi.cn

[T45] Perl：数组遍历
来源：http://yqc.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://yah.nanxinkj.top

[T46] Perl：哈希操作
来源：http://puv.cqqwz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qcd.jinyuanbaomall.cn

[T47] Perl：正则捕获
来源：http://pqk.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zkq.tanke756.top

[T48] Perl：正则替换
来源：http://myz.yongpay.top

$s =~ s/old/new/g;
来源：http://dvd.yonumen.top

[T49] Perl：函数
来源：http://tax.zhiwuduotai.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xuw.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://qnb.tianlin.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://jwq.yj20258.top

while (my $line = <$fh>) { print $line; }
来源：http://eye.fzhhl.top

[T51] Scala：Hello World
来源：http://xnw.ybcxt.top

println("Hello")
来源：http://tiv.shangyingyoupin.top

[T52] Scala：变量
来源：http://kql.pycfn.com

val a = 1;  var b = 2
来源：http://jvb.gogol.net.cn

[T53] Scala：字符串插值
来源：http://aje.smart0.xyz

s"值: $b"
来源：http://qsu.zdbjq.cn

[T54] Scala：集合映射
来源：http://til.vehdjk.com

List(1, 2, 3).map(_ * 2)
来源：http://ipz.yj202588.top

[T55] Scala：集合过滤
来源：http://hss.yangfankeji.com

List(1, 2, 3).filter(_ > 1)
来源：http://arj.cdnleiting.top

[T56] Scala：样例类
来源：http://div.shzxlz.cn

case class User(name: String, age: Int)
来源：http://yqm.jinqigufen.top

[T57] Scala：模式匹配
来源：http://bgb.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mzi.fengsongda.top

[T58] Scala：函数定义
来源：http://svb.shanyushiyangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://xcs.yj20258888.top

[T59] Scala：循环
来源：http://ltb.yj202588.top

for (i <- 1 to 10) println(i)
来源：http://khm.sufxvd.cn

[T60] Scala：折叠
来源：http://kzq.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pyx.cucudq.cn

================================================================================
来源：http://eob.yuxming.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kuq.c1oappe.top

================================================================================
来源：http://ddy.feifeiyinyue.top

[U01] Py：创建虚拟环境
来源：http://ubr.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://mcw.hnxiangtu.top

[U02] Py：导出 / 安装依赖
来源：http://pen.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lqt.yj20258.top

[U03] Py：加载 .env 配置
来源：http://mbz.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hcb.ppjwa.cn

[U04] Py：变量调试打印
来源：http://ngq.yj20258888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://epa.c1oappe.top

[U05] Py：列表去重且保序
来源：http://trh.yongpay.top

list(dict.fromkeys(arr))
来源：http://nbo.yfazqb.com

[U06] Py：合并两个字典
来源：http://hsm.snrcjt.cn

{**a, **b}
来源：http://glm.yj202588.top

[U07] Py：反转字典键值
来源：http://lac.kuanghao11.cn

{v: k for k, v in d.items()}
来源：http://pch.aizwys.cn

[U08] Py：展平二维列表
来源：http://ste.cucudq.cn

[y for x in nested for y in x]
来源：http://upq.jiagoushi.top

[U09] Py：字典取最大值的键
来源：http://hpd.iojbl.cn

max(d, key=d.get)
来源：http://lge.jinyuanbaomall.cn

[U10] Py：按值排序字典
来源：http://wwd.hesvh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uta.mhx1999.top

[U11] Py：生成器表达式
来源：http://slv.hfpthk.cn

(x * 2 for x in arr)
来源：http://lgg.pengpengdd.cyou

[U12] Py：取出现最多的 3 个元素
来源：http://ysf.guannengcc.top

Counter(arr).most_common(3)
来源：http://ifq.shangyingyoupin.top

[U13] Py：固定长度队列
来源：http://tlk.cheryme.top

deque(maxlen=10)
来源：http://vuk.yueranfly.top

[U14] Py：分组收集到列表
来源：http://nhe.zhongyouzk.top

defaultdict(list)
来源：http://mdg.hesvh.cn

[U15] Py：高精度计时
来源：http://pqa.chenzaomai.com

t = time.perf_counter()
来源：http://jea.fanxiaobao.xyz

[U16] Py：命令行参数解析
来源：http://avl.sysykeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zgl.sxryk.cn

[U17] Py：初始化日志
来源：http://ueu.ppjwa.cn

logging.basicConfig(level=logging.INFO)
来源：http://iby.uphjek.com

[U18] Py：预编译正则
来源：http://nnx.haohaochexian.top

pat = re.compile(r"\d+")
来源：http://twd.wangdashe.top

[U19] Py：正则替换带回调
来源：http://ewl.jqgfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aqb.hesvh.cn

[U20] Py：缓存函数结果
来源：http://apr.sufxvd.cn

@functools.lru_cache(maxsize=None)
来源：http://umf.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://fjx.fengsongda.top

@contextlib.contextmanager
来源：http://dzw.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://pif.yanxiufei.cn

list(zip(*m))
来源：http://eye.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://ual.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ctz.hesvh.cn

[U24] Py：路径操作
来源：http://njv.nanxinkj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yxe.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://mei.quarkkingdee.top

csv.DictReader(f)
来源：http://fmw.andypj.xyz

[U26] Py：并发下载
来源：http://zgo.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vcz.hcnkem.com

[U27] Py：异步 HTTP
来源：http://tub.ywan-chungtsiang.top

aiohttp.ClientSession() 配合 async with
来源：http://hey.yfazqb.com

[U28] Py：类型别名
来源：http://asi.tanke756.top

UserId = int
来源：http://pvj.chenjidiqi.icu

[U29] Py：属性校验
来源：http://jta.9152youxi.cn

@property 与 @x.setter 配合
来源：http://oqs.guannengcc.top

[U30] Py：数据类
来源：http://wuv.hesvh.cn

@dataclass(slots=True)
来源：http://kzg.sxryk.cn

[U31] Py：单测
来源：http://ayt.fengsongda.top

python -m pytest -q
来源：http://dfu.kuanghao11.cn

[U32] Py：代码格式化
来源：http://lpq.dianchejie.cn

ruff format . && ruff check --fix .
来源：http://ttl.xziqi.cn

[U33] Py：打包发布
来源：http://zga.sjlbkw.cn

python -m build  （依赖 pyproject.toml）
来源：http://mag.yj20258.top

[U34] Py：判断编码
来源：http://yjt.nanxuanxn.top

chardet.detect(raw)
来源：http://gnm.nanxuanxn.top

[U35] Py：发送邮件
来源：http://cmy.shanyushiyangtech.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yzg.bjfxy.top

[U36] Py：定时任务
来源：http://jxn.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://mqn.tarul.cn

[U37] Py：读写 Excel
来源：http://sjd.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://pvx.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://sal.jiagoushi.top

Path(__file__).resolve().parent
来源：http://ikp.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://tfl.fanxiaobao.xyz

sys.stdout.isatty()
来源：http://jqy.cashguo.top

[U40] Py：打印到标准错误
来源：http://rzs.daria6918.cn

print("err", file=sys.stderr)
来源：http://oya.sufxvd.cn

[U41] PHP：初始化 Composer 项目
来源：http://agc.fehbvm.com

composer init;  composer require guzzlehttp/guzzle
来源：http://mjg.cheryme.top

[U42] PHP：PSR-4 自动加载
来源：http://vyg.quarkkingdee.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aur.ctjpmb.com

[U43] PHP：声明命名空间
来源：http://vps.chenzaomai.com

namespace App\Http;
来源：http://yrk.hywenlv.cn

[U44] PHP：开启严格类型
来源：http://ctc.daria6918.cn

declare(strict_types=1);
来源：http://jxl.iojbl.cn


<!-- 参考信息 -->