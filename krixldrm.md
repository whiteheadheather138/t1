代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lka.iojbl.cn

[S13] C：宏定义
来源：http://ekm.xylfe.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tll.hywenlv.cn

[S14] C：枚举
来源：http://qjd.nanxuanxn.top

enum Color { RED, GREEN, BLUE };
来源：http://tec.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://wqp.sufxvd.cn

(double) a / b
来源：http://agp.sufxvd.cn

[S16] C：位操作置位
来源：http://iuj.tarul.cn

x |= (1 << 3);
来源：http://dlz.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://cuj.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ttd.jianghu66.top

[S18] C：命令行参数
来源：http://xrl.ydzc1.top

int main(int argc, char **argv)
来源：http://geb.nwbrower.top

[S19] C：快速排序
来源：http://uud.cheryme.top

qsort(a, n, sizeof(int), cmp);
来源：http://ohy.zdqjudy.top

[S20] C：二分查找
来源：http://otg.zdbjq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kjd.yvedp.cn

[S21] C：字符类别判断
来源：http://ufq.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fol.ydjk.org.cn

[S22] C：字符串转数字
来源：http://tpb.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://uqi.ywan-chungtsiang.top

[S23] C：随机数
来源：http://xns.52xcode.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://diz.9152youxi.cn

[S24] C：获取本地时间
来源：http://dyc.gzhubu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ucr.xylfe.cn

[S25] C：内存拷贝
来源：http://nag.sweek.top

memcpy(dst, src, n);
来源：http://zux.redwolf501.top

[S26] C：内存清零
来源：http://rla.ybcxt.top

memset(a, 0, sizeof a);
来源：http://pvq.hammf.cn

[S27] C：定义常量
来源：http://ags.xingfuxueyuan.xyz

const double PI = 3.14159;
来源：http://dnc.ydzc1.top

[S28] C：静态变量
来源：http://cje.yanxiufei.cn

static int counter = 0;
来源：http://eyn.dianchejie.cn

[S29] C：变参函数
来源：http://dfj.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fdc.hongshengwenyu.top

[S30] C：头文件保护
来源：http://gfi.pengpengdd.cyou

#ifndef X_H
来源：http://fwf.smart0.xyz

#define X_H
来源：http://tbl.pycfn.com

#endif
来源：http://aus.gzhubu.top

[S31] C++：Hello World
来源：http://oul.xuanzx.com

#include <iostream>
来源：http://sfv.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://jgr.ivvv.top

[S32] C++：字符串
来源：http://hsl.shangyingyoupin.top

std::string s = "hi";  s += "!";
来源：http://awo.mhx1999.top

[S33] C++：vector 增删
来源：http://ltp.uphjek.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pmv.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://jcd.hfpthk.cn

for (auto &x : v) { std::cout << x; }
来源：http://stg.jiagoushi.top

[S35] C++：map
来源：http://wyu.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fai.xuetiantiany.cn

[S36] C++：unordered_map
来源：http://grj.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xeu.9152youxi.cn

[S37] C++：set
来源：http://ios.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dpk.ehwqpu.com

[S38] C++：排序
来源：http://uug.0kj1m.cn

std::sort(v.begin(), v.end());
来源：http://ttw.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://sxp.zhijiandao.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lew.epnwcf.com

[S40] C++：查找元素
来源：http://ywe.nanxuanxn.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vuo.jyoumei.cn

[S41] C++：类与构造函数
来源：http://ajj.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iaq.shanyushiyangtech.top

[S42] C++：继承与虚函数
来源：http://wgb.pycfn.com

class B : public Base { public: void f() override {} };
来源：http://bgt.sweek.top

[S43] C++：智能指针
来源：http://hns.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://yet.vqdsnc.cn

[S44] C++：引用传参
来源：http://ber.tanke756.top

void inc(int &x) { ++x; }
来源：http://kty.vehdjk.com

[S45] C++：lambda
来源：http://mkx.jyoumei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ath.andypj.xyz

[S46] C++：函数模板
来源：http://iee.tarul.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sfe.fehbvm.com

[S47] C++：结构化绑定遍历
来源：http://agn.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pro.yangfankeji.com

[S48] C++：逐行读文件
来源：http://ldl.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iam.guowangkeji.top

while (std::getline(in, line)) { }
来源：http://ddd.birdmap.top

[S49] C++：写文件
来源：http://uvm.316326.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ihq.yueranfly.top

[S50] C++：格式化数字
来源：http://rfn.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eqz.hnqzz.top

[S51] C++：显式类型转换
来源：http://qrm.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://dxb.daxiang520.top

[S52] C++：const 与 noexcept
来源：http://wem.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://ipn.sweek.top

[S53] C++：移动语义
来源：http://odv.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://yqb.gzhubu.top

[S54] C++：异常处理
来源：http://enl.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dva.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://kan.fehbvm.com

auto [a, b] = std::make_pair(1, 2);
来源：http://xfd.sysykeji.top

[S56] C++：optional
来源：http://vyx.hnxiangtu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gdm.hnxiangtu.top

[S57] C++：编译期常量
来源：http://bef.fehbvm.com

constexpr int N = 10;
来源：http://eas.ppjwa.cn

[S58] C++：命名空间
来源：http://rtg.snrcjt.cn

namespace ns { int f() { return 1; } }
来源：http://buf.jinqigfzy.top

[S59] C++：静态断言
来源：http://xis.cqqwz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pbw.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://ktr.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lab.shzxlz.cn

================================================================================
来源：http://aqu.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fjl.mhx1999.top

================================================================================
来源：http://wis.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://ctf.chenjidiqi.icu

println("Hello")
来源：http://itj.yj20258.top

[T02] Kotlin：变量
来源：http://awy.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xza.xingfuxueyuan.xyz

[T03] Kotlin：字符串模板
来源：http://mqe.shzxlz.cn

"值: $b"
来源：http://dfl.ppjwa.cn

[T04] Kotlin：空安全
来源：http://alj.shuidangran.top

val n: String? = null;  n?.length
来源：http://gyv.cdnleiting.top

[T05] Kotlin：when 表达式
来源：http://fjm.yueranfly.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://twt.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://jpr.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://doz.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://cnx.pengpengdd.cyou

listOf(1, 2, 3).filter { it > 1 }
来源：http://zte.sweek.top

[T08] Kotlin：数据类
来源：http://pqb.quarkkingdee.top

data class User(val name: String, val age: Int)
来源：http://gzd.hesvh.cn

[T09] Kotlin：扩展函数
来源：http://cni.zhiwuduotai.top

fun String.exclaim() = this + "!"
来源：http://rvx.zhaomingkeji.xyz

[T10] Kotlin：默认参数
来源：http://iml.hammf.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nto.yonumen.top

[T11] Kotlin：协程
来源：http://uyn.xinyue.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://cxb.xylfe.cn

[T12] Kotlin：解构声明
来源：http://ovd.cucudq.cn

val (a, b) = Pair(1, 2)
来源：http://zmk.yj20258.top

[T13] Kotlin：只读 Map
来源：http://zrx.gogol.net.cn

val m = mapOf("a" to 1)
来源：http://usa.jlsjyb.cn

[T14] Kotlin：循环
来源：http://ysh.zdbjq.cn

for (i in 1..10) println(i)
来源：http://vge.hnxiangtu.top

[T15] Kotlin：接口
来源：http://vvi.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://ybi.cqqwz.cn

[T16] Swift：Hello World
来源：http://mba.shanyushiyangkeji.top

print("Hello")
来源：http://xhv.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://agt.snrcjt.cn

var a = 1;  let b = 2
来源：http://wwr.52xcode.cn

[T18] Swift：字符串插值
来源：http://lrq.havefunace.top

"值: \(b)"
来源：http://evn.vehdjk.com

[T19] Swift：可选绑定
来源：http://nvb.aizwys.cn

if let n = opt { print(n) }
来源：http://sha.uphjek.com

[T20] Swift：数组操作
来源：http://ujv.hcnkem.com

var a = [1, 2, 3];  a.append(4)
来源：http://wtk.dianchejie.cn

[T21] Swift：遍历
来源：http://tuh.zhengqikj.top

for x in a { print(x) }
来源：http://uzl.ywan-chungtsiang.top

[T22] Swift：字典
来源：http://awf.yj20258.top

var d = ["a": 1];  d["b"] = 2
来源：http://gut.yueranfly.top

[T23] Swift：函数
来源：http://gch.aizwys.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rjl.fktsv.cn

[T24] Swift：闭包
来源：http://trk.yueranfly.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://emz.uphjek.com

[T25] Swift：结构体
来源：http://ztk.jinghuilouyu.cn

struct P { var x: Int }
来源：http://bug.svipenyu.cn

[T26] Swift：类与重写
来源：http://brk.cucudq.cn

class A: Base { override func f() {} }
来源：http://fod.shuidangran.top

[T27] Swift：错误处理
来源：http://byw.tianlin.xyz

do { try f() } catch { print(error) }
来源：http://sck.yuanzhike.top

[T28] Swift：枚举
来源：http://rzl.feifeiyinyue.top

enum Color { case red, green }
来源：http://kma.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://xcc.jinghuilouyu.cn

guard let x = opt else { return }
来源：http://lqb.nanxuanxn.top

[T30] Swift：协议
来源：http://awd.hongshengwenyu.top

protocol Shape { func area() -> Double }
来源：http://kxe.shzxlz.cn

[T31] Lua：Hello World
来源：http://mwv.bjfxy.top

print("Hello")
来源：http://tay.nwbrower.top

[T32] Lua：局部变量
来源：http://ueq.mhx1999.top

local a = 1
来源：http://ywn.hysaishi.cn

[T33] Lua：表（数组）
来源：http://cmc.fengsongda.top

local t = {1, 2, 3};  t[4] = 4
来源：http://myp.hnqzz.top

[T34] Lua：遍历表
来源：http://exf.zhongyouzk.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qmf.zhoulong.xyz

[T35] Lua：字典表
来源：http://vbh.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://qxs.shangyingyoupin.top

[T36] Lua：函数
来源：http://vki.haohaochexian.top

function add(a, b) return a + b end
来源：http://hzv.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://qgb.daria6918.cn

"a" .. "b"
来源：http://tir.birdmap.top

[T38] Lua：条件
来源：http://ycr.tanke756.top

if x > 0 then print("正") end
来源：http://tis.ybcxt.top

[T39] Lua：模式匹配
来源：http://xqs.jinghuilouyu.cn

string.find(s, "%d+")
来源：http://wmz.tian-w.cn

[T40] Lua：元表
来源：http://pev.xuanzx.com

setmetatable({}, { __index = base })
来源：http://tva.yj202588.top

[T41] Perl：Hello World
来源：http://mfj.guowangkeji.top

print "Hello\n";
来源：http://vbs.gotoacloud.top

[T42] Perl：变量类型
来源：http://rwg.guowangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ome.hywenlv.cn

[T43] Perl：字符串插值
来源：http://iki.kuanghao11.cn

"值: $a"
来源：http://jbc.jianghu66.top

[T44] Perl：条件
来源：http://ugp.dianchejie.cn

if ($a > 0) { print "正"; }
来源：http://zil.epnwcf.com

[T45] Perl：数组遍历
来源：http://qxl.pycfn.com

for my $x (@arr) { print $x; }
来源：http://ihs.hysaishi.cn

[T46] Perl：哈希操作
来源：http://xor.uphjek.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://adp.bjfxy.top

[T47] Perl：正则捕获
来源：http://aid.sxryk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uex.xylfe.cn

[T48] Perl：正则替换
来源：http://xsx.gzhubu.top

$s =~ s/old/new/g;
来源：http://kla.uphjek.com

[T49] Perl：函数
来源：http://cag.mhx1999.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dth.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://iyp.wangshuangyany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fnb.jianghu66.top

while (my $line = <$fh>) { print $line; }
来源：http://udq.uphjek.com

[T51] Scala：Hello World
来源：http://wii.yanxiufei.cn

println("Hello")
来源：http://vov.ybcxt.top

[T52] Scala：变量
来源：http://aqg.yj20258.top

val a = 1;  var b = 2
来源：http://avf.dianchejie.cn

[T53] Scala：字符串插值
来源：http://efu.zdbjq.cn

s"值: $b"
来源：http://wnh.vehdjk.com

[T54] Scala：集合映射
来源：http://hmk.shuidangran.top

List(1, 2, 3).map(_ * 2)
来源：http://ong.chenjidiqi.icu

[T55] Scala：集合过滤
来源：http://mkq.ehwqpu.com

List(1, 2, 3).filter(_ > 1)
来源：http://afs.fzhhl.top

[T56] Scala：样例类
来源：http://rgg.daria6918.cn

case class User(name: String, age: Int)
来源：http://hvj.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://cul.0kj1m.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vix.yj202588.top

[T58] Scala：函数定义
来源：http://xxg.hcnkem.com

def add(a: Int, b: Int): Int = a + b
来源：http://chj.smart0.xyz

[T59] Scala：循环
来源：http://hzx.guannengcc.top

for (i <- 1 to 10) println(i)
来源：http://wyh.xuanzx.com

[T60] Scala：折叠
来源：http://ury.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lxz.yangfankeji.com

================================================================================
来源：http://omd.yj20258888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qkz.hcnkem.com

================================================================================
来源：http://oqx.xinyue.icu

[U01] Py：创建虚拟环境
来源：http://epx.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://jja.jyoumei.cn

[U02] Py：导出 / 安装依赖
来源：http://rhj.ivvv.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ccj.aibaodan.cn

[U03] Py：加载 .env 配置
来源：http://tmy.hammf.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ofh.birdmap.top

[U04] Py：变量调试打印
来源：http://zmu.yvedp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://avk.mhx1999.top

[U05] Py：列表去重且保序
来源：http://qjb.meibo888.top

list(dict.fromkeys(arr))
来源：http://ybr.fehbvm.com

[U06] Py：合并两个字典
来源：http://vpx.yuanzhike.top

{**a, **b}
来源：http://npx.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://sxr.yueranfly.top

{v: k for k, v in d.items()}
来源：http://quq.tian-w.cn

[U08] Py：展平二维列表
来源：http://vhp.yvedp.cn

[y for x in nested for y in x]
来源：http://ewc.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://qrn.pengpengdd.cyou

max(d, key=d.get)
来源：http://gmz.yongpay.top

[U10] Py：按值排序字典
来源：http://utr.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hpv.xylfe.cn

[U11] Py：生成器表达式
来源：http://ydd.zdbjq.cn

(x * 2 for x in arr)
来源：http://rys.smart0.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://zqs.shzxlz.cn

Counter(arr).most_common(3)
来源：http://nju.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://mco.xinyue.icu

deque(maxlen=10)
来源：http://ouj.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://sfr.ppjwa.cn

defaultdict(list)
来源：http://yhp.hnqzz.top

[U15] Py：高精度计时
来源：http://dpd.dashuyun.cn

t = time.perf_counter()
来源：http://pcn.52xcode.cn

[U16] Py：命令行参数解析
来源：http://mch.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oai.mhx1999.top

[U17] Py：初始化日志
来源：http://tbs.cheryme.top

logging.basicConfig(level=logging.INFO)
来源：http://xau.yongpay.top

[U18] Py：预编译正则
来源：http://knf.xziqi.cn

pat = re.compile(r"\d+")
来源：http://hjv.tanke756.top

[U19] Py：正则替换带回调
来源：http://tzj.aizwys.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qqt.chenlongwang.top

[U20] Py：缓存函数结果
来源：http://iie.jiagoushi.top

@functools.lru_cache(maxsize=None)
来源：http://vwu.sysykeji.top

[U21] Py：自定义上下文管理器
来源：http://bqf.shzxlz.cn

@contextlib.contextmanager
来源：http://ioc.zhaomingkeji.xyz

[U22] Py：矩阵转置
来源：http://tkl.tian-w.cn

list(zip(*m))
来源：http://dlz.shuidangran.top

[U23] Py：分块读取大文件
来源：http://hus.ydzc1.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lav.shanyushiyangtech.top

[U24] Py：路径操作
来源：http://elm.jqgufenzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://apv.xziqi.cn

[U25] Py：CSV 按字典读
来源：http://ngd.c1oappe.top

csv.DictReader(f)
来源：http://bqa.havefunace.top

[U26] Py：并发下载
来源：http://jxg.sufxvd.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xmn.zhongyouzk.top

[U27] Py：异步 HTTP
来源：http://cws.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://vhd.yonumen.top

[U28] Py：类型别名
来源：http://isd.yuanzhike.top

UserId = int
来源：http://esd.tanke756.top

[U29] Py：属性校验
来源：http://sgm.316326.xyz

@property 与 @x.setter 配合
来源：http://bal.hesvh.cn

[U30] Py：数据类
来源：http://lau.yueranfly.top

@dataclass(slots=True)
来源：http://ycw.vehdjk.com

[U31] Py：单测
来源：http://tqv.zycfv.cn

python -m pytest -q
来源：http://gxq.hongshengwenyu.top

[U32] Py：代码格式化
来源：http://nyd.aizwys.cn

ruff format . && ruff check --fix .
来源：http://avp.tianlin.xyz

[U33] Py：打包发布
来源：http://ykm.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://wpj.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://ylt.sufxvd.cn

chardet.detect(raw)
来源：http://eii.sufxvd.cn

[U35] Py：发送邮件
来源：http://mxv.jqgfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mbw.cheryme.top

[U36] Py：定时任务
来源：http://wuk.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://xev.cqqwz.cn


<!-- 参考信息 -->