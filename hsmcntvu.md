代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://raf.yj20258.top

[S15] C：类型转换
来源：http://zgr.jlsjyb.cn

(double) a / b
来源：http://sbu.hammf.cn

[S16] C：位操作置位
来源：http://grs.cqqwz.cn

x |= (1 << 3);
来源：http://kvt.zycfv.cn

[S17] C：安全拼接字符串
来源：http://pad.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pnp.hnqzz.top

[S18] C：命令行参数
来源：http://gcu.dianchejie.cn

int main(int argc, char **argv)
来源：http://rqf.cheryme.top

[S19] C：快速排序
来源：http://vop.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://jnx.jqgufenzy.top

[S20] C：二分查找
来源：http://onp.daria6918.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ksy.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://crk.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mpd.zhixingplan.top

[S22] C：字符串转数字
来源：http://mch.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://xfg.sufxvd.cn

[S23] C：随机数
来源：http://xvb.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rgd.daria6918.cn

[S24] C：获取本地时间
来源：http://axf.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://snn.yuanzhike.top

[S25] C：内存拷贝
来源：http://owe.ywan-chungtsiang.top

memcpy(dst, src, n);
来源：http://brj.dianchejie.cn

[S26] C：内存清零
来源：http://lgq.52xcode.cn

memset(a, 0, sizeof a);
来源：http://qhl.hesvh.cn

[S27] C：定义常量
来源：http://yda.jqgfzy.top

const double PI = 3.14159;
来源：http://elx.xuanzx.com

[S28] C：静态变量
来源：http://mex.yj20258888.top

static int counter = 0;
来源：http://vyo.yuanzhike.top

[S29] C：变参函数
来源：http://gui.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oot.0kj1m.cn

[S30] C：头文件保护
来源：http://fdy.hammf.cn

#ifndef X_H
来源：http://ldg.yfazqb.com

#define X_H
来源：http://bcm.pengpengdd.cyou

#endif
来源：http://rpg.wangshuangyany.cn

[S31] C++：Hello World
来源：http://lft.uphjek.com

#include <iostream>
来源：http://pgq.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://hfo.pycfn.com

[S32] C++：字符串
来源：http://acv.pycfn.com

std::string s = "hi";  s += "!";
来源：http://jxx.wangdashe.top

[S33] C++：vector 增删
来源：http://yhu.hesvh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gmh.hammf.cn

[S34] C++：遍历 vector
来源：http://pmv.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://eaj.ivvv.top

[S35] C++：map
来源：http://jrx.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wyl.ppjwa.cn

[S36] C++：unordered_map
来源：http://dkz.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uvq.jlsjyb.cn

[S37] C++：set
来源：http://gcz.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fxp.fzhhl.top

[S38] C++：排序
来源：http://bxy.meibo888.top

std::sort(v.begin(), v.end());
来源：http://lny.nwbrower.top

[S39] C++：自定义比较器排序
来源：http://aku.smart0.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xgu.gotoacloud.top

[S40] C++：查找元素
来源：http://jhd.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://icw.ehwqpu.com

[S41] C++：类与构造函数
来源：http://fkw.tarul.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cmu.ydjk.org.cn

[S42] C++：继承与虚函数
来源：http://kyn.nanxuanxn.top

class B : public Base { public: void f() override {} };
来源：http://bvw.pycfn.com

[S43] C++：智能指针
来源：http://dxm.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://vsj.wangshuangyany.cn

[S44] C++：引用传参
来源：http://zmf.yj20258888.top

void inc(int &x) { ++x; }
来源：http://com.nanxinkj.top

[S45] C++：lambda
来源：http://use.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://yyl.fzhhl.top

[S46] C++：函数模板
来源：http://cfa.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lqy.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://zqc.zdqjudy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://isn.ivvv.top

[S48] C++：逐行读文件
来源：http://cem.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://woc.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://knq.ydzc1.top

[S49] C++：写文件
来源：http://nln.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aid.ivvv.top

[S50] C++：格式化数字
来源：http://ugy.jyoumei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wpg.nwbrower.top

[S51] C++：显式类型转换
来源：http://ire.ctjpmb.com

static_cast<double>(a) / b
来源：http://zgq.yuxming.cn

[S52] C++：const 与 noexcept
来源：http://hsk.ydzc1.top

int size() const noexcept { return n_; }
来源：http://daq.gaohongyu789.top

[S53] C++：移动语义
来源：http://yji.hammf.cn

std::vector<int> w = std::move(v);
来源：http://rsp.uphjek.com

[S54] C++：异常处理
来源：http://ozl.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hsm.ppjwa.cn

[S55] C++：结构化绑定
来源：http://cqc.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yjr.yj202588.top

[S56] C++：optional
来源：http://abd.yuxming.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eww.jinqigfzy.top

[S57] C++：编译期常量
来源：http://fzz.hnxiangtu.top

constexpr int N = 10;
来源：http://nzn.yj202588.top

[S58] C++：命名空间
来源：http://cgf.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://kfb.sxryk.cn

[S59] C++：静态断言
来源：http://add.hesvh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fnj.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://irm.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tua.chenjidiqi.icu

================================================================================
来源：http://fgh.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qqq.tanke756.top

================================================================================
来源：http://jjy.aibaodan.cn

[T01] Kotlin：Hello World
来源：http://rny.hammf.cn

println("Hello")
来源：http://zsk.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://klu.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kdp.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://oga.cqqwz.cn

"值: $b"
来源：http://cme.9152youxi.cn

[T04] Kotlin：空安全
来源：http://rka.cucudq.cn

val n: String? = null;  n?.length
来源：http://wsa.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://efo.birdmap.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ztk.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://dge.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dlw.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://djm.mhx1999.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wcf.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://gjq.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://saf.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://xpw.zdbjq.cn

fun String.exclaim() = this + "!"
来源：http://cqa.gotoacloud.top

[T10] Kotlin：默认参数
来源：http://vug.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wbr.aizwys.cn

[T11] Kotlin：协程
来源：http://kxv.yueranfly.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lio.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://mqh.tian-w.cn

val (a, b) = Pair(1, 2)
来源：http://eyg.cashguo.top

[T13] Kotlin：只读 Map
来源：http://pkg.cucudq.cn

val m = mapOf("a" to 1)
来源：http://pep.daxiang520.top

[T14] Kotlin：循环
来源：http://swp.hammf.cn

for (i in 1..10) println(i)
来源：http://jfn.chenzaomai.com

[T15] Kotlin：接口
来源：http://vle.zhoulong.xyz

interface Shape { fun area(): Double }
来源：http://hzk.yj20258.top

[T16] Swift：Hello World
来源：http://ymf.yuanzhike.top

print("Hello")
来源：http://thr.jyoumei.cn

[T17] Swift：变量与常量
来源：http://apv.cheryme.top

var a = 1;  let b = 2
来源：http://syz.cashguo.top

[T18] Swift：字符串插值
来源：http://xuy.wangshuangyany.cn

"值: \(b)"
来源：http://fjz.sjlbkw.cn

[T19] Swift：可选绑定
来源：http://zkp.vqdsnc.cn

if let n = opt { print(n) }
来源：http://wzv.redwolf501.top

[T20] Swift：数组操作
来源：http://vqu.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://vuc.sjlbkw.cn

[T21] Swift：遍历
来源：http://rqr.fzhhl.top

for x in a { print(x) }
来源：http://aun.chenzaomai.com

[T22] Swift：字典
来源：http://vcz.gogol.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ggy.cqqwz.cn

[T23] Swift：函数
来源：http://rot.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mff.zhengqikj.top

[T24] Swift：闭包
来源：http://tou.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://dms.hesvh.cn

[T25] Swift：结构体
来源：http://qhj.jqgufenzy.top

struct P { var x: Int }
来源：http://rvr.yj20258.top

[T26] Swift：类与重写
来源：http://cub.jinyuanbaomall.cn

class A: Base { override func f() {} }
来源：http://pfj.sysykeji.top

[T27] Swift：错误处理
来源：http://mkz.xylfe.cn

do { try f() } catch { print(error) }
来源：http://tfc.zycfv.cn

[T28] Swift：枚举
来源：http://qal.ppjwa.cn

enum Color { case red, green }
来源：http://whh.guowangkeji.top

[T29] Swift：guard 提前返回
来源：http://ufl.dashuyun.cn

guard let x = opt else { return }
来源：http://gfi.zdqjudy.top

[T30] Swift：协议
来源：http://myw.zhoulong.xyz

protocol Shape { func area() -> Double }
来源：http://nxw.cucudq.cn

[T31] Lua：Hello World
来源：http://crd.c1oappe.top

print("Hello")
来源：http://apj.yfazqb.com

[T32] Lua：局部变量
来源：http://qwn.sxryk.cn

local a = 1
来源：http://adp.jianghu66.top

[T33] Lua：表（数组）
来源：http://umu.yanxiufei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iff.zhijiandao.cn

[T34] Lua：遍历表
来源：http://rni.chenjidiqi.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://dss.xziqi.cn

[T35] Lua：字典表
来源：http://kyf.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://vsr.ybcxt.top

[T36] Lua：函数
来源：http://los.haohaochexian.top

function add(a, b) return a + b end
来源：http://dfg.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://wrv.tian-w.cn

"a" .. "b"
来源：http://dcd.xylfe.cn

[T38] Lua：条件
来源：http://zda.jinqigfzy.top

if x > 0 then print("正") end
来源：http://yuo.fzhhl.top

[T39] Lua：模式匹配
来源：http://zfj.meibo888.top

string.find(s, "%d+")
来源：http://aqc.yonumen.top

[T40] Lua：元表
来源：http://xmr.xylfe.cn

setmetatable({}, { __index = base })
来源：http://xzi.gzhubu.top

[T41] Perl：Hello World
来源：http://lry.uphjek.com

print "Hello\n";
来源：http://zfa.xuetiantiany.cn

[T42] Perl：变量类型
来源：http://vto.pycfn.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://czy.bbcook.cn

[T43] Perl：字符串插值
来源：http://vmk.gaohongyu789.top

"值: $a"
来源：http://iyz.yongpay.top

[T44] Perl：条件
来源：http://tjq.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://qod.haohaochexian.top

[T45] Perl：数组遍历
来源：http://nnb.xinyue.icu

for my $x (@arr) { print $x; }
来源：http://wzb.uphjek.com

[T46] Perl：哈希操作
来源：http://kgh.daria6918.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nbe.yj20258888.top

[T47] Perl：正则捕获
来源：http://haj.gaohongyu789.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ext.hysaishi.cn

[T48] Perl：正则替换
来源：http://dig.jiagoushi.top

$s =~ s/old/new/g;
来源：http://zlo.ehwqpu.com

[T49] Perl：函数
来源：http://rsc.gaohongyu789.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zxq.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://fux.xziqi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sjs.jqgufenzy.top

while (my $line = <$fh>) { print $line; }
来源：http://qaf.daria6918.cn

[T51] Scala：Hello World
来源：http://sfx.nanxinkj.top

println("Hello")
来源：http://big.gotoacloud.top

[T52] Scala：变量
来源：http://ucq.jinqigufen.top

val a = 1;  var b = 2
来源：http://sql.yonumen.top

[T53] Scala：字符串插值
来源：http://vjp.zhiwuduotai.top

s"值: $b"
来源：http://ied.xuanzx.com

[T54] Scala：集合映射
来源：http://bhe.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://ffj.zdqjudy.top

[T55] Scala：集合过滤
来源：http://xpi.zhoulong.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://jho.ppjwa.cn

[T56] Scala：样例类
来源：http://wbr.ctjpmb.com

case class User(name: String, age: Int)
来源：http://jje.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://dcg.wangdashe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mjz.cqqwz.cn

[T58] Scala：函数定义
来源：http://nmm.hnqzz.top

def add(a: Int, b: Int): Int = a + b
来源：http://qva.jinghuilouyu.cn

[T59] Scala：循环
来源：http://nyc.dashuyun.cn

for (i <- 1 to 10) println(i)
来源：http://rbn.chenjidiqi.icu

[T60] Scala：折叠
来源：http://agj.xylfe.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ydy.iojbl.cn

================================================================================
来源：http://fdm.iojbl.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gxq.shanyushiyangtech.top

================================================================================
来源：http://fsq.shuidangran.top

[U01] Py：创建虚拟环境
来源：http://wji.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://xmd.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://kbs.snrcjt.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hil.hcnkem.com

[U03] Py：加载 .env 配置
来源：http://tih.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ecc.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://swp.zhiwuduotai.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hrs.xylfe.cn

[U05] Py：列表去重且保序
来源：http://qsz.ywan-chungtsiang.top

list(dict.fromkeys(arr))
来源：http://mir.chenjidiqi.icu

[U06] Py：合并两个字典
来源：http://zko.yj20258.top

{**a, **b}
来源：http://npq.xuetiantiany.cn

[U07] Py：反转字典键值
来源：http://zmb.daxiang520.top

{v: k for k, v in d.items()}
来源：http://roe.nwbrower.top

[U08] Py：展平二维列表
来源：http://vrz.yuanzhike.top

[y for x in nested for y in x]
来源：http://chb.jinqigufen.top

[U09] Py：字典取最大值的键
来源：http://ipj.yuxming.cn

max(d, key=d.get)
来源：http://yjj.ydjk.org.cn

[U10] Py：按值排序字典
来源：http://and.gogol.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iod.jianghu66.top

[U11] Py：生成器表达式
来源：http://dcm.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://six.nanxuanxn.top

[U12] Py：取出现最多的 3 个元素
来源：http://cny.xylfe.cn

Counter(arr).most_common(3)
来源：http://caq.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://qyk.zdqjudy.top

deque(maxlen=10)
来源：http://yli.tian-w.cn

[U14] Py：分组收集到列表
来源：http://cyh.ivvv.top

defaultdict(list)
来源：http://cyl.cashguo.top

[U15] Py：高精度计时
来源：http://hfi.tianlin.xyz

t = time.perf_counter()
来源：http://bos.jianghu66.top

[U16] Py：命令行参数解析
来源：http://kwc.kuanghao11.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sbu.zhongyouzk.top

[U17] Py：初始化日志
来源：http://dem.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://eam.9152youxi.cn

[U18] Py：预编译正则
来源：http://uzp.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://kjh.bbcook.cn

[U19] Py：正则替换带回调
来源：http://dzg.shzxlz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mqb.jianghu66.top

[U20] Py：缓存函数结果
来源：http://fwa.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://epv.fktsv.cn

[U21] Py：自定义上下文管理器
来源：http://lzl.yongpay.top

@contextlib.contextmanager
来源：http://nas.ctjpmb.com

[U22] Py：矩阵转置
来源：http://tdo.feifeiyinyue.top

list(zip(*m))
来源：http://cfc.aibaodan.cn

[U23] Py：分块读取大文件
来源：http://vme.ywan-chungtsiang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jzz.jqgufenzy.top

[U24] Py：路径操作
来源：http://nbp.yuanzhike.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vjx.birdmap.top

[U25] Py：CSV 按字典读
来源：http://sug.sysykeji.top

csv.DictReader(f)
来源：http://hau.fzhhl.top

[U26] Py：并发下载
来源：http://cju.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://icy.xuanzx.com

[U27] Py：异步 HTTP
来源：http://oev.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://tjc.epnwcf.com

[U28] Py：类型别名
来源：http://cqk.hammf.cn

UserId = int
来源：http://jzi.yongpay.top

[U29] Py：属性校验
来源：http://puu.hysaishi.cn

@property 与 @x.setter 配合
来源：http://oyt.jinqigfzy.top

[U30] Py：数据类
来源：http://fig.ivvv.top

@dataclass(slots=True)
来源：http://slw.hcnkem.com

[U31] Py：单测
来源：http://ztw.cqqwz.cn

python -m pytest -q
来源：http://unh.cdnleiting.top

[U32] Py：代码格式化
来源：http://gib.hongshengwenyu.top

ruff format . && ruff check --fix .
来源：http://fzl.nwbrower.top

[U33] Py：打包发布
来源：http://ixv.hfpthk.cn

python -m build  （依赖 pyproject.toml）
来源：http://ssl.ydjk.org.cn

[U34] Py：判断编码
来源：http://wkm.316326.xyz

chardet.detect(raw)
来源：http://bbh.gogol.net.cn

[U35] Py：发送邮件
来源：http://pbd.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ben.jqgufenzy.top

[U36] Py：定时任务
来源：http://kqd.nanxuanxn.top

schedule.every(10).minutes.do(job)
来源：http://mxx.shuidangran.top

[U37] Py：读写 Excel
来源：http://unp.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://kvh.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://dgh.cucudq.cn

Path(__file__).resolve().parent
来源：http://yhk.pycfn.com


<!-- 参考信息 -->