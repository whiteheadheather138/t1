代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://mep.hammf.cn

[S15] C：类型转换
来源：http://qxh.dianchejie.cn

(double) a / b
来源：http://sqy.gaohongyu789.top

[S16] C：位操作置位
来源：http://zfx.guannengcc.top

x |= (1 << 3);
来源：http://yrc.sysykeji.top

[S17] C：安全拼接字符串
来源：http://bqi.jqgfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ggi.shanyushiyangkeji.top

[S18] C：命令行参数
来源：http://nsx.feifeiyinyue.top

int main(int argc, char **argv)
来源：http://xgd.shanyushiyangtech.top

[S19] C：快速排序
来源：http://pvs.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://ugf.daxiang520.top

[S20] C：二分查找
来源：http://pbe.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bbz.tian-w.cn

[S21] C：字符类别判断
来源：http://kiz.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rbx.meibo888.top

[S22] C：字符串转数字
来源：http://ygd.dashuyun.cn

atoi("42");  strtod("3.14", NULL);
来源：http://irn.wangshuangyany.cn

[S23] C：随机数
来源：http://rxc.zhiwuduotai.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yef.aizwys.cn

[S24] C：获取本地时间
来源：http://cwz.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dee.9152youxi.cn

[S25] C：内存拷贝
来源：http://dga.smart0.xyz

memcpy(dst, src, n);
来源：http://xdk.nanxinkj.top

[S26] C：内存清零
来源：http://jnh.fehbvm.com

memset(a, 0, sizeof a);
来源：http://avk.zhoulong.xyz

[S27] C：定义常量
来源：http://moq.sweek.top

const double PI = 3.14159;
来源：http://msk.ywan-chungtsiang.top

[S28] C：静态变量
来源：http://nfv.jqgufenzy.top

static int counter = 0;
来源：http://uls.cashguo.top

[S29] C：变参函数
来源：http://qak.yanxiufei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://krt.vehdjk.com

[S30] C：头文件保护
来源：http://ptg.hammf.cn

#ifndef X_H
来源：http://zpf.yueranfly.top

#define X_H
来源：http://iid.hesvh.cn

#endif
来源：http://muy.vqdsnc.cn

[S31] C++：Hello World
来源：http://ffl.zycfv.cn

#include <iostream>
来源：http://axg.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://auh.jinghuilouyu.cn

[S32] C++：字符串
来源：http://lvq.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://uaz.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://atf.jinqigfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ysl.nanxinkj.top

[S34] C++：遍历 vector
来源：http://hdg.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://pkk.meibo888.top

[S35] C++：map
来源：http://inv.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ijl.iojbl.cn

[S36] C++：unordered_map
来源：http://sdk.jiagoushi.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zbb.cashguo.top

[S37] C++：set
来源：http://whh.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oqc.epnwcf.com

[S38] C++：排序
来源：http://gbv.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://zlw.uphjek.com

[S39] C++：自定义比较器排序
来源：http://oqt.316326.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lfw.daxiang520.top

[S40] C++：查找元素
来源：http://moi.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fzc.shanyushiyangkeji.top

[S41] C++：类与构造函数
来源：http://bur.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bbl.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://rzx.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://yci.ybcxt.top

[S43] C++：智能指针
来源：http://jlb.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://deu.chenjidiqi.icu

[S44] C++：引用传参
来源：http://ufo.zhaomingkeji.xyz

void inc(int &x) { ++x; }
来源：http://rbn.wangdashe.top

[S45] C++：lambda
来源：http://umq.kuanghao11.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ncd.feifeiyinyue.top

[S46] C++：函数模板
来源：http://skn.smart0.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dts.shzxlz.cn

[S47] C++：结构化绑定遍历
来源：http://khn.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dnr.ybcxt.top

[S48] C++：逐行读文件
来源：http://lny.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://xvy.nanxinkj.top

while (std::getline(in, line)) { }
来源：http://amu.sufxvd.cn

[S49] C++：写文件
来源：http://ppz.ydzc1.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ivw.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://yvm.pycfn.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://onv.hammf.cn

[S51] C++：显式类型转换
来源：http://fva.tanke756.top

static_cast<double>(a) / b
来源：http://unl.ivvv.top

[S52] C++：const 与 noexcept
来源：http://bqg.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://luy.jinqigufen.top

[S53] C++：移动语义
来源：http://zcv.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://ytm.yj202588.top

[S54] C++：异常处理
来源：http://eee.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qmp.daria6918.cn

[S55] C++：结构化绑定
来源：http://uju.yvedp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vwx.0kj1m.cn

[S56] C++：optional
来源：http://jsy.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wmx.52xcode.cn

[S57] C++：编译期常量
来源：http://ype.shuidangran.top

constexpr int N = 10;
来源：http://vhv.zhoulong.xyz

[S58] C++：命名空间
来源：http://kid.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://muh.redwolf501.top

[S59] C++：静态断言
来源：http://tpb.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lhk.aizwys.cn

[S60] C++：遍历并删除元素
来源：http://xnr.cucudq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ubs.yvedp.cn

================================================================================
来源：http://iio.yj202588.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wxh.jinqigfzy.top

================================================================================
来源：http://jxa.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://kgz.tanke756.top

println("Hello")
来源：http://gwy.ybcxt.top

[T02] Kotlin：变量
来源：http://efm.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wai.hesvh.cn

[T03] Kotlin：字符串模板
来源：http://zcw.iojbl.cn

"值: $b"
来源：http://ogx.sysykeji.top

[T04] Kotlin：空安全
来源：http://vps.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://aaq.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://xyd.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tuf.zdqjudy.top

[T06] Kotlin：集合映射
来源：http://rwr.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://cvd.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://zkc.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kjs.fanxiaobao.xyz

[T08] Kotlin：数据类
来源：http://kur.xinyue.icu

data class User(val name: String, val age: Int)
来源：http://zmb.shangyingyoupin.top

[T09] Kotlin：扩展函数
来源：http://cat.pycfn.com

fun String.exclaim() = this + "!"
来源：http://tmt.ybcxt.top

[T10] Kotlin：默认参数
来源：http://iev.yueranfly.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fuf.nanxuanxn.top

[T11] Kotlin：协程
来源：http://slj.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rlw.yvedp.cn

[T12] Kotlin：解构声明
来源：http://szj.tianlin.xyz

val (a, b) = Pair(1, 2)
来源：http://vyr.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://lea.shzxlz.cn

val m = mapOf("a" to 1)
来源：http://wad.cqqwz.cn

[T14] Kotlin：循环
来源：http://gbu.fzhhl.top

for (i in 1..10) println(i)
来源：http://bdr.ybcxt.top

[T15] Kotlin：接口
来源：http://rjx.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://qsd.zhongyouzk.top

[T16] Swift：Hello World
来源：http://zct.vqdsnc.cn

print("Hello")
来源：http://wso.svipenyu.cn

[T17] Swift：变量与常量
来源：http://qrf.vqdsnc.cn

var a = 1;  let b = 2
来源：http://zyq.fzhhl.top

[T18] Swift：字符串插值
来源：http://cny.jinqigufen.top

"值: \(b)"
来源：http://vpc.316326.xyz

[T19] Swift：可选绑定
来源：http://ofg.yonumen.top

if let n = opt { print(n) }
来源：http://lvt.gogol.net.cn

[T20] Swift：数组操作
来源：http://twx.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qqn.zdbjq.cn

[T21] Swift：遍历
来源：http://wmc.hnqzz.top

for x in a { print(x) }
来源：http://eiw.redwolf501.top

[T22] Swift：字典
来源：http://nma.yangfankeji.com

var d = ["a": 1];  d["b"] = 2
来源：http://pxe.redwolf501.top

[T23] Swift：函数
来源：http://vos.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cao.redwolf501.top

[T24] Swift：闭包
来源：http://caq.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ifs.zhengqikj.top

[T25] Swift：结构体
来源：http://nyz.ywan-chungtsiang.top

struct P { var x: Int }
来源：http://eyc.epnwcf.com

[T26] Swift：类与重写
来源：http://fzt.yfazqb.com

class A: Base { override func f() {} }
来源：http://qhm.andypj.xyz

[T27] Swift：错误处理
来源：http://rbj.jyoumei.cn

do { try f() } catch { print(error) }
来源：http://tmp.smart0.xyz

[T28] Swift：枚举
来源：http://itj.gogol.net.cn

enum Color { case red, green }
来源：http://rfr.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://ehf.jlsjyb.cn

guard let x = opt else { return }
来源：http://urj.ctjpmb.com

[T30] Swift：协议
来源：http://kta.shanyushiyangtech.top

protocol Shape { func area() -> Double }
来源：http://gdn.ivvv.top

[T31] Lua：Hello World
来源：http://dxo.hesvh.cn

print("Hello")
来源：http://xuo.xylfe.cn

[T32] Lua：局部变量
来源：http://wzq.xuanzx.com

local a = 1
来源：http://fiq.jinqigfzy.top

[T33] Lua：表（数组）
来源：http://ems.dianchejie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fan.sysykeji.top

[T34] Lua：遍历表
来源：http://tms.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ggh.vqdsnc.cn

[T35] Lua：字典表
来源：http://yko.wangshuangyany.cn

local d = { a = 1 };  d.b = 2
来源：http://lzj.nanxinkj.top

[T36] Lua：函数
来源：http://bzv.tarul.cn

function add(a, b) return a + b end
来源：http://xao.yj202588.top

[T37] Lua：字符串拼接
来源：http://xwo.0kj1m.cn

"a" .. "b"
来源：http://mrj.zhiwuduotai.top

[T38] Lua：条件
来源：http://hta.tian-w.cn

if x > 0 then print("正") end
来源：http://qcj.dashuyun.cn

[T39] Lua：模式匹配
来源：http://zmn.xuanzx.com

string.find(s, "%d+")
来源：http://fha.fktsv.cn

[T40] Lua：元表
来源：http://vmb.yueranfly.top

setmetatable({}, { __index = base })
来源：http://wfl.hysaishi.cn

[T41] Perl：Hello World
来源：http://jry.yj202588.top

print "Hello\n";
来源：http://ymw.bbcook.cn

[T42] Perl：变量类型
来源：http://jcw.zhixingplan.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lar.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://tdd.9152youxi.cn

"值: $a"
来源：http://vaf.xuanzx.com

[T44] Perl：条件
来源：http://ish.hammf.cn

if ($a > 0) { print "正"; }
来源：http://ino.yj20258.top

[T45] Perl：数组遍历
来源：http://fjh.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://utg.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://ntz.zhengqikj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bdk.chenlongwang.top

[T47] Perl：正则捕获
来源：http://ckz.quarkkingdee.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bkm.yueranfly.top

[T48] Perl：正则替换
来源：http://qkg.yj202588.top

$s =~ s/old/new/g;
来源：http://twx.jyoumei.cn

[T49] Perl：函数
来源：http://sol.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ztt.ehwqpu.com

[T50] Perl：逐行读文件
来源：http://pjx.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://luv.shuidangran.top

while (my $line = <$fh>) { print $line; }
来源：http://tyj.shanyushiyangtech.top

[T51] Scala：Hello World
来源：http://vtc.sweek.top

println("Hello")
来源：http://yvk.fzhhl.top

[T52] Scala：变量
来源：http://ets.ctjpmb.com

val a = 1;  var b = 2
来源：http://ubj.fanxiaobao.xyz

[T53] Scala：字符串插值
来源：http://mwr.yj20258888.top

s"值: $b"
来源：http://rvg.xylfe.cn

[T54] Scala：集合映射
来源：http://foj.zhiwuduotai.top

List(1, 2, 3).map(_ * 2)
来源：http://xdm.zhengqikj.top

[T55] Scala：集合过滤
来源：http://npf.vqdsnc.cn

List(1, 2, 3).filter(_ > 1)
来源：http://meq.jianghu66.top

[T56] Scala：样例类
来源：http://dyc.yueranfly.top

case class User(name: String, age: Int)
来源：http://irt.shangyingyoupin.top

[T57] Scala：模式匹配
来源：http://mri.tianlin.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://pfz.yj20258.top

[T58] Scala：函数定义
来源：http://xfd.kuanghao11.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fuy.yvedp.cn

[T59] Scala：循环
来源：http://whz.aizwys.cn

for (i <- 1 to 10) println(i)
来源：http://owz.zhoulong.xyz

[T60] Scala：折叠
来源：http://eci.tian-w.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qri.jqgfzy.top

================================================================================
来源：http://que.shanyushiyangtech.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yhs.tanke756.top

================================================================================
来源：http://mya.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://xit.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pmc.fehbvm.com

[U02] Py：导出 / 安装依赖
来源：http://jxr.yj20258888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zmx.yj202588.top

[U03] Py：加载 .env 配置
来源：http://ahk.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://nrx.dianchejie.cn

[U04] Py：变量调试打印
来源：http://vdv.wangshuangyany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zra.yuxming.cn

[U05] Py：列表去重且保序
来源：http://kgc.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://xyw.zhiwuduotai.top

[U06] Py：合并两个字典
来源：http://rtq.zhixingplan.top

{**a, **b}
来源：http://xyc.ybcxt.top

[U07] Py：反转字典键值
来源：http://dpd.cashguo.top

{v: k for k, v in d.items()}
来源：http://mzd.shanyushiyangkeji.top

[U08] Py：展平二维列表
来源：http://nsc.kuanghao11.cn

[y for x in nested for y in x]
来源：http://tjy.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://fpv.xingfuxueyuan.xyz

max(d, key=d.get)
来源：http://njs.daxiang520.top

[U10] Py：按值排序字典
来源：http://wff.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fnr.vqdsnc.cn

[U11] Py：生成器表达式
来源：http://qzg.mhx1999.top

(x * 2 for x in arr)
来源：http://zwa.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://zhm.aibaodan.cn

Counter(arr).most_common(3)
来源：http://wac.smart0.xyz

[U13] Py：固定长度队列
来源：http://srr.shangyingyoupin.top

deque(maxlen=10)
来源：http://qzn.haohaochexian.top

[U14] Py：分组收集到列表
来源：http://onq.ydzc1.top

defaultdict(list)
来源：http://wog.fanxiaobao.xyz

[U15] Py：高精度计时
来源：http://agb.jianghu66.top

t = time.perf_counter()
来源：http://gpf.daria6918.cn

[U16] Py：命令行参数解析
来源：http://wuy.chenzaomai.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mxx.hcnkem.com

[U17] Py：初始化日志
来源：http://nsz.tian-w.cn

logging.basicConfig(level=logging.INFO)
来源：http://pzw.zhengqikj.top

[U18] Py：预编译正则
来源：http://rts.mhx1999.top

pat = re.compile(r"\d+")
来源：http://sbn.hesvh.cn

[U19] Py：正则替换带回调
来源：http://ulc.ybcxt.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://myv.yuxming.cn

[U20] Py：缓存函数结果
来源：http://gyw.tian-w.cn

@functools.lru_cache(maxsize=None)
来源：http://qaq.zhixingplan.top

[U21] Py：自定义上下文管理器
来源：http://obv.zdqjudy.top

@contextlib.contextmanager
来源：http://vfm.mhx1999.top

[U22] Py：矩阵转置
来源：http://ivu.jinqigfzy.top

list(zip(*m))
来源：http://pue.haohaochexian.top

[U23] Py：分块读取大文件
来源：http://kys.shangyingyoupin.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vwg.pengpengdd.cyou

[U24] Py：路径操作
来源：http://zea.yvedp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://irn.nanxinkj.top

[U25] Py：CSV 按字典读
来源：http://znj.ivvv.top

csv.DictReader(f)
来源：http://wmn.jqgufenzy.top

[U26] Py：并发下载
来源：http://usb.sweek.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://olc.vqdsnc.cn

[U27] Py：异步 HTTP
来源：http://yqz.redwolf501.top

aiohttp.ClientSession() 配合 async with
来源：http://ted.hesvh.cn

[U28] Py：类型别名
来源：http://dzb.zhiwuduotai.top

UserId = int
来源：http://thd.ehwqpu.com

[U29] Py：属性校验
来源：http://hwz.shzxlz.cn

@property 与 @x.setter 配合
来源：http://fpj.ywan-chungtsiang.top

[U30] Py：数据类
来源：http://hqq.316326.xyz

@dataclass(slots=True)
来源：http://wlk.hcnkem.com

[U31] Py：单测
来源：http://wrb.fengsongda.top

python -m pytest -q
来源：http://nvw.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://fwj.hnqzz.top

ruff format . && ruff check --fix .
来源：http://all.yfazqb.com

[U33] Py：打包发布
来源：http://bsd.xuanzx.com

python -m build  （依赖 pyproject.toml）
来源：http://otu.shangyingyoupin.top

[U34] Py：判断编码
来源：http://xoe.yuanzhike.top

chardet.detect(raw)
来源：http://ggm.tian-w.cn

[U35] Py：发送邮件
来源：http://tuv.vqdsnc.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ujb.quarkkingdee.top

[U36] Py：定时任务
来源：http://cec.dianchejie.cn

schedule.every(10).minutes.do(job)
来源：http://djn.dashuyun.cn

[U37] Py：读写 Excel
来源：http://okq.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://mvu.smart0.xyz

[U38] Py：获取脚本所在目录
来源：http://feh.tanke756.top

Path(__file__).resolve().parent
来源：http://jjq.aibaodan.cn


<!-- 参考信息 -->