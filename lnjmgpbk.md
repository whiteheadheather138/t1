代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://spk.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://hew.aibaodan.cn

fclose(f);
来源：http://hhn.9152youxi.cn

[S12] C：写文件
来源：http://fhl.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://enu.tanke756.top

[S13] C：宏定义
来源：http://ibg.hongshengwenyu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kfn.wangshuangyany.cn

[S14] C：枚举
来源：http://tsb.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://yqu.shanyushiyangkeji.top

[S15] C：类型转换
来源：http://xsp.bbcook.cn

(double) a / b
来源：http://hna.mhx1999.top

[S16] C：位操作置位
来源：http://noz.havefunace.top

x |= (1 << 3);
来源：http://zdm.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://xjm.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://plu.zhaomingkeji.xyz

[S18] C：命令行参数
来源：http://ogn.sufxvd.cn

int main(int argc, char **argv)
来源：http://hml.shuidangran.top

[S19] C：快速排序
来源：http://qqu.316326.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://obv.uphjek.com

[S20] C：二分查找
来源：http://dvd.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nxv.birdmap.top

[S21] C：字符类别判断
来源：http://iaq.shangyingyoupin.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ofw.ydjk.org.cn

[S22] C：字符串转数字
来源：http://kau.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lfp.cucudq.cn

[S23] C：随机数
来源：http://ekf.ctjpmb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://lpo.birdmap.top

[S24] C：获取本地时间
来源：http://zzr.tianlin.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xrc.pengpengdd.cyou

[S25] C：内存拷贝
来源：http://vij.xuanzx.com

memcpy(dst, src, n);
来源：http://kve.gzhubu.top

[S26] C：内存清零
来源：http://mjm.pycfn.com

memset(a, 0, sizeof a);
来源：http://ffm.jqgfzy.top

[S27] C：定义常量
来源：http://ulr.bjfxy.top

const double PI = 3.14159;
来源：http://hrk.birdmap.top

[S28] C：静态变量
来源：http://olj.hcnkem.com

static int counter = 0;
来源：http://efd.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://ncv.gotoacloud.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bin.smart0.xyz

[S30] C：头文件保护
来源：http://fsj.yongpay.top

#ifndef X_H
来源：http://pca.pycfn.com

#define X_H
来源：http://wco.yfazqb.com

#endif
来源：http://cme.smart0.xyz

[S31] C++：Hello World
来源：http://xko.yanxiufei.cn

#include <iostream>
来源：http://khq.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://nib.yanxiufei.cn

[S32] C++：字符串
来源：http://jvo.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://osp.jianghu66.top

[S33] C++：vector 增删
来源：http://gwn.vqdsnc.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ird.fengsongda.top

[S34] C++：遍历 vector
来源：http://dbj.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://vav.shanyushiyangkeji.top

[S35] C++：map
来源：http://xwx.yuxming.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zyv.gogol.net.cn

[S36] C++：unordered_map
来源：http://snh.iojbl.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hbg.jinyuanbaomall.cn

[S37] C++：set
来源：http://jvx.havefunace.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iot.xylfe.cn

[S38] C++：排序
来源：http://dkp.fehbvm.com

std::sort(v.begin(), v.end());
来源：http://pee.jqgfzy.top

[S39] C++：自定义比较器排序
来源：http://qvw.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bbr.nanxuanxn.top

[S40] C++：查找元素
来源：http://wcn.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://knv.yfazqb.com

[S41] C++：类与构造函数
来源：http://jos.jqgfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wue.yj20258888.top

[S42] C++：继承与虚函数
来源：http://hsk.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://els.andypj.xyz

[S43] C++：智能指针
来源：http://rae.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://gvr.jianghu66.top

[S44] C++：引用传参
来源：http://ptr.ydjk.org.cn

void inc(int &x) { ++x; }
来源：http://jvm.pycfn.com

[S45] C++：lambda
来源：http://nhc.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://hbx.xuetiantiany.cn

[S46] C++：函数模板
来源：http://wed.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hih.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://hqi.gzhubu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ngl.316326.xyz

[S48] C++：逐行读文件
来源：http://mki.smart0.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://hxe.mhx1999.top

while (std::getline(in, line)) { }
来源：http://tsq.xylfe.cn

[S49] C++：写文件
来源：http://put.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vmd.316326.xyz

[S50] C++：格式化数字
来源：http://beo.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qhh.pycfn.com

[S51] C++：显式类型转换
来源：http://xjx.ydzc1.top

static_cast<double>(a) / b
来源：http://lbh.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://cux.hfpthk.cn

int size() const noexcept { return n_; }
来源：http://bjm.smart0.xyz

[S53] C++：移动语义
来源：http://hsd.yj20258.top

std::vector<int> w = std::move(v);
来源：http://hjv.nanxuanxn.top

[S54] C++：异常处理
来源：http://kxh.sufxvd.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fel.jqgufenzy.top

[S55] C++：结构化绑定
来源：http://cbm.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gch.316326.xyz

[S56] C++：optional
来源：http://jwn.vehdjk.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mhy.vehdjk.com

[S57] C++：编译期常量
来源：http://wsp.jinghuilouyu.cn

constexpr int N = 10;
来源：http://rhm.zhongyouzk.top

[S58] C++：命名空间
来源：http://jvt.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://efh.hysaishi.cn

[S59] C++：静态断言
来源：http://bdv.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pqv.sufxvd.cn

[S60] C++：遍历并删除元素
来源：http://vpr.yuxming.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qja.yj202588.top

================================================================================
来源：http://wsd.pycfn.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ate.ywan-chungtsiang.top

================================================================================
来源：http://edv.nanxuanxn.top

[T01] Kotlin：Hello World
来源：http://lld.xinyue.icu

println("Hello")
来源：http://ery.sweek.top

[T02] Kotlin：变量
来源：http://hyt.fehbvm.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yfm.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://djq.zdbjq.cn

"值: $b"
来源：http://sou.cdnleiting.top

[T04] Kotlin：空安全
来源：http://jmo.vehdjk.com

val n: String? = null;  n?.length
来源：http://fjm.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://rum.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://psf.redwolf501.top

[T06] Kotlin：集合映射
来源：http://nyc.epnwcf.com

listOf(1, 2, 3).map { it * 2 }
来源：http://pat.aibaodan.cn

[T07] Kotlin：集合过滤
来源：http://lfh.gotoacloud.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://err.yuxming.cn

[T08] Kotlin：数据类
来源：http://dye.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://uzg.zhijiandao.cn

[T09] Kotlin：扩展函数
来源：http://qww.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://gea.ybcxt.top

[T10] Kotlin：默认参数
来源：http://gkq.dashuyun.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oyy.c1oappe.top

[T11] Kotlin：协程
来源：http://wdb.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://kvz.cucudq.cn

[T12] Kotlin：解构声明
来源：http://gnl.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://gob.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://uzc.pycfn.com

val m = mapOf("a" to 1)
来源：http://dln.guowangkeji.top

[T14] Kotlin：循环
来源：http://qtr.hnqzz.top

for (i in 1..10) println(i)
来源：http://rya.fehbvm.com

[T15] Kotlin：接口
来源：http://sfi.shzxlz.cn

interface Shape { fun area(): Double }
来源：http://qjw.cdnleiting.top

[T16] Swift：Hello World
来源：http://wfp.c1oappe.top

print("Hello")
来源：http://cyc.jyoumei.cn

[T17] Swift：变量与常量
来源：http://qdr.c1oappe.top

var a = 1;  let b = 2
来源：http://yla.yanxiufei.cn

[T18] Swift：字符串插值
来源：http://cim.fzhhl.top

"值: \(b)"
来源：http://eou.ehwqpu.com

[T19] Swift：可选绑定
来源：http://cyd.zhoulong.xyz

if let n = opt { print(n) }
来源：http://snf.nwbrower.top

[T20] Swift：数组操作
来源：http://lsm.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vxu.hcnkem.com

[T21] Swift：遍历
来源：http://hbf.yangfankeji.com

for x in a { print(x) }
来源：http://mew.aizwys.cn

[T22] Swift：字典
来源：http://egt.tanke756.top

var d = ["a": 1];  d["b"] = 2
来源：http://fwk.ivvv.top

[T23] Swift：函数
来源：http://yhf.cdnleiting.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uqx.ybcxt.top

[T24] Swift：闭包
来源：http://vjs.jianghu66.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jaa.xuanzx.com

[T25] Swift：结构体
来源：http://rbi.pycfn.com

struct P { var x: Int }
来源：http://zeh.hesvh.cn

[T26] Swift：类与重写
来源：http://sdi.xylfe.cn

class A: Base { override func f() {} }
来源：http://ika.yvedp.cn

[T27] Swift：错误处理
来源：http://cnh.gaohongyu789.top

do { try f() } catch { print(error) }
来源：http://ucm.c1oappe.top

[T28] Swift：枚举
来源：http://ums.vqdsnc.cn

enum Color { case red, green }
来源：http://lyj.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://zzu.fanxiaobao.xyz

guard let x = opt else { return }
来源：http://ost.zhengqikj.top

[T30] Swift：协议
来源：http://ech.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://ltp.9152youxi.cn

[T31] Lua：Hello World
来源：http://ftm.bjfxy.top

print("Hello")
来源：http://fzc.shanyushiyangtech.top

[T32] Lua：局部变量
来源：http://leu.bjfxy.top

local a = 1
来源：http://amu.gotoacloud.top

[T33] Lua：表（数组）
来源：http://vdt.9152youxi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lva.jinyuanbaomall.cn

[T34] Lua：遍历表
来源：http://ygc.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://zwi.shuidangran.top

[T35] Lua：字典表
来源：http://uhp.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://nzj.hysaishi.cn

[T36] Lua：函数
来源：http://xey.jyoumei.cn

function add(a, b) return a + b end
来源：http://bvh.shzxlz.cn

[T37] Lua：字符串拼接
来源：http://hdw.pycfn.com

"a" .. "b"
来源：http://syq.jlsjyb.cn

[T38] Lua：条件
来源：http://khj.pycfn.com

if x > 0 then print("正") end
来源：http://wjx.chenzaomai.com

[T39] Lua：模式匹配
来源：http://yaw.hongshengwenyu.top

string.find(s, "%d+")
来源：http://cyo.xylfe.cn

[T40] Lua：元表
来源：http://sag.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://rwb.aibaodan.cn

[T41] Perl：Hello World
来源：http://vfi.yangfankeji.com

print "Hello\n";
来源：http://mfg.fanxiaobao.xyz

[T42] Perl：变量类型
来源：http://afh.havefunace.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ltw.haohaochexian.top

[T43] Perl：字符串插值
来源：http://aef.yanxiufei.cn

"值: $a"
来源：http://tgn.ybcxt.top

[T44] Perl：条件
来源：http://agd.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://elk.jinyuanbaomall.cn

[T45] Perl：数组遍历
来源：http://tdw.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://mqn.cashguo.top

[T46] Perl：哈希操作
来源：http://zfh.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lpk.dianchejie.cn

[T47] Perl：正则捕获
来源：http://fzu.jinqigufen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tac.zhengqikj.top

[T48] Perl：正则替换
来源：http://nwl.svipenyu.cn

$s =~ s/old/new/g;
来源：http://zfp.zhoulong.xyz

[T49] Perl：函数
来源：http://pbi.nanxuanxn.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tpz.epnwcf.com

[T50] Perl：逐行读文件
来源：http://unh.wangshuangyany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rzk.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://dby.smart0.xyz

[T51] Scala：Hello World
来源：http://mwm.jqgufenzy.top

println("Hello")
来源：http://nme.zycfv.cn

[T52] Scala：变量
来源：http://cjd.fehbvm.com

val a = 1;  var b = 2
来源：http://zuk.birdmap.top

[T53] Scala：字符串插值
来源：http://lcz.gzhubu.top

s"值: $b"
来源：http://bck.jlsjyb.cn

[T54] Scala：集合映射
来源：http://nrb.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://zlt.cucudq.cn

[T55] Scala：集合过滤
来源：http://coe.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sqo.fanxiaobao.xyz

[T56] Scala：样例类
来源：http://nwe.guowangkeji.top

case class User(name: String, age: Int)
来源：http://tfc.daria6918.cn

[T57] Scala：模式匹配
来源：http://thd.yonumen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lpk.zhengqikj.top

[T58] Scala：函数定义
来源：http://dqp.fktsv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pdy.jinyuanbaomall.cn

[T59] Scala：循环
来源：http://tgr.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://fjg.gotoacloud.top

[T60] Scala：折叠
来源：http://tcb.jiagoushi.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cuh.quarkkingdee.top

================================================================================
来源：http://fin.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rlw.guannengcc.top

================================================================================
来源：http://fpm.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://cmk.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://gvr.dashuyun.cn

[U02] Py：导出 / 安装依赖
来源：http://ycq.chenjidiqi.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lfh.9152youxi.cn

[U03] Py：加载 .env 配置
来源：http://pnb.pengpengdd.cyou

from dotenv import load_dotenv; load_dotenv()
来源：http://wxk.zdqjudy.top

[U04] Py：变量调试打印
来源：http://isn.shzxlz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ctf.xuetiantiany.cn

[U05] Py：列表去重且保序
来源：http://gve.hammf.cn

list(dict.fromkeys(arr))
来源：http://lsq.vehdjk.com

[U06] Py：合并两个字典
来源：http://hun.fanxiaobao.xyz

{**a, **b}
来源：http://bmd.jlsjyb.cn

[U07] Py：反转字典键值
来源：http://ntl.jinyuanbaomall.cn

{v: k for k, v in d.items()}
来源：http://fly.shuidangran.top

[U08] Py：展平二维列表
来源：http://rym.haohaochexian.top

[y for x in nested for y in x]
来源：http://vbq.ydjk.org.cn

[U09] Py：字典取最大值的键
来源：http://kqg.nanxinkj.top

max(d, key=d.get)
来源：http://czf.ydzc1.top

[U10] Py：按值排序字典
来源：http://dhv.fzhhl.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gtb.jyoumei.cn

[U11] Py：生成器表达式
来源：http://zbl.hnxiangtu.top

(x * 2 for x in arr)
来源：http://gso.jinqigfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://hxl.guowangkeji.top

Counter(arr).most_common(3)
来源：http://vow.sysykeji.top

[U13] Py：固定长度队列
来源：http://sww.316326.xyz

deque(maxlen=10)
来源：http://qtm.hesvh.cn

[U14] Py：分组收集到列表
来源：http://ovc.dianchejie.cn

defaultdict(list)
来源：http://ofb.daria6918.cn

[U15] Py：高精度计时
来源：http://zrw.hysaishi.cn

t = time.perf_counter()
来源：http://npk.yj20258.top

[U16] Py：命令行参数解析
来源：http://pih.tarul.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ikc.gaohongyu789.top

[U17] Py：初始化日志
来源：http://tca.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://ixl.birdmap.top

[U18] Py：预编译正则
来源：http://pzh.iojbl.cn

pat = re.compile(r"\d+")
来源：http://hvb.hammf.cn

[U19] Py：正则替换带回调
来源：http://dum.cdnleiting.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://owy.feifeiyinyue.top

[U20] Py：缓存函数结果
来源：http://ddz.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://pxw.ybcxt.top

[U21] Py：自定义上下文管理器
来源：http://ewm.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://ibm.yj20258.top

[U22] Py：矩阵转置
来源：http://vrs.yanxiufei.cn

list(zip(*m))
来源：http://ydl.hcnkem.com

[U23] Py：分块读取大文件
来源：http://nih.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bie.yfazqb.com

[U24] Py：路径操作
来源：http://rpj.cdnleiting.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dvy.0kj1m.cn

[U25] Py：CSV 按字典读
来源：http://ymv.sxryk.cn

csv.DictReader(f)
来源：http://kem.zdbjq.cn

[U26] Py：并发下载
来源：http://tpb.ppjwa.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://glf.vqdsnc.cn

[U27] Py：异步 HTTP
来源：http://tvh.ivvv.top

aiohttp.ClientSession() 配合 async with
来源：http://gio.havefunace.top

[U28] Py：类型别名
来源：http://bgb.hnqzz.top

UserId = int
来源：http://vxx.hywenlv.cn

[U29] Py：属性校验
来源：http://iqh.yfazqb.com

@property 与 @x.setter 配合
来源：http://ggq.hongshengwenyu.top

[U30] Py：数据类
来源：http://nwe.nwbrower.top

@dataclass(slots=True)
来源：http://gww.cqqwz.cn

[U31] Py：单测
来源：http://smu.hnxiangtu.top

python -m pytest -q
来源：http://rnp.nwbrower.top

[U32] Py：代码格式化
来源：http://mxj.dianchejie.cn

ruff format . && ruff check --fix .
来源：http://qub.fengsongda.top

[U33] Py：打包发布
来源：http://qlz.nanxuanxn.top

python -m build  （依赖 pyproject.toml）
来源：http://orc.jinqigufen.top

[U34] Py：判断编码
来源：http://tka.xziqi.cn

chardet.detect(raw)
来源：http://rrg.jqgufenzy.top


<!-- 参考信息 -->