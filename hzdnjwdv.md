代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://tzy.gzhubu.top

[S15] C：类型转换
来源：http://eqe.jianghu66.top

(double) a / b
来源：http://svl.bbcook.cn

[S16] C：位操作置位
来源：http://ljs.yj20258.top

x |= (1 << 3);
来源：http://xll.redwolf501.top

[S17] C：安全拼接字符串
来源：http://ubk.tanke756.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xpo.birdmap.top

[S18] C：命令行参数
来源：http://vwh.zhongyouzk.top

int main(int argc, char **argv)
来源：http://dya.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://lpx.daxiang520.top

qsort(a, n, sizeof(int), cmp);
来源：http://dcy.aizwys.cn

[S20] C：二分查找
来源：http://gvk.iojbl.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bqt.chenzaomai.com

[S21] C：字符类别判断
来源：http://ujo.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vmm.ydjk.org.cn

[S22] C：字符串转数字
来源：http://jgi.haohaochexian.top

atoi("42");  strtod("3.14", NULL);
来源：http://syp.jiagoushi.top

[S23] C：随机数
来源：http://ohz.zhoulong.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://grl.chenlongwang.top

[S24] C：获取本地时间
来源：http://owz.yanxiufei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hgl.sxryk.cn

[S25] C：内存拷贝
来源：http://jga.aibaodan.cn

memcpy(dst, src, n);
来源：http://cef.wangdashe.top

[S26] C：内存清零
来源：http://wex.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://pph.xuanzx.com

[S27] C：定义常量
来源：http://lfi.zhoulong.xyz

const double PI = 3.14159;
来源：http://lfb.jqgfzy.top

[S28] C：静态变量
来源：http://vpa.yvedp.cn

static int counter = 0;
来源：http://eqk.snrcjt.cn

[S29] C：变参函数
来源：http://wwe.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hhk.meibo888.top

[S30] C：头文件保护
来源：http://zzj.shanyushiyangkeji.top

#ifndef X_H
来源：http://sjc.sxryk.cn

#define X_H
来源：http://eob.yfazqb.com

#endif
来源：http://hzj.jqgufenzy.top

[S31] C++：Hello World
来源：http://tis.fzhhl.top

#include <iostream>
来源：http://jxg.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://rel.316326.xyz

[S32] C++：字符串
来源：http://onr.smart0.xyz

std::string s = "hi";  s += "!";
来源：http://jvc.gotoacloud.top

[S33] C++：vector 增删
来源：http://ixp.smart0.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cvn.yj20258888.top

[S34] C++：遍历 vector
来源：http://rny.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://fzd.vqdsnc.cn

[S35] C++：map
来源：http://jpt.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bsh.fzhhl.top

[S36] C++：unordered_map
来源：http://brg.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yoa.shanyushiyangkeji.top

[S37] C++：set
来源：http://ggc.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cxm.wangdashe.top

[S38] C++：排序
来源：http://nvw.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://tqc.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://bwg.yanxiufei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xyz.yfazqb.com

[S40] C++：查找元素
来源：http://fnt.chenjidiqi.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zzp.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://oje.jinyuanbaomall.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fxb.redwolf501.top

[S42] C++：继承与虚函数
来源：http://hgl.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://jao.ybcxt.top

[S43] C++：智能指针
来源：http://yjp.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://set.hysaishi.cn

[S44] C++：引用传参
来源：http://kuh.ydzc1.top

void inc(int &x) { ++x; }
来源：http://zpf.hnxiangtu.top

[S45] C++：lambda
来源：http://ocz.yj20258888.top

auto add = [](int a, int b) { return a + b; };
来源：http://ass.jinqigfzy.top

[S46] C++：函数模板
来源：http://ulm.cdnleiting.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qxj.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://uvf.bjfxy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zar.redwolf501.top

[S48] C++：逐行读文件
来源：http://wqg.shanyushiyangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://kdy.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://gde.xuanzx.com

[S49] C++：写文件
来源：http://cim.jinyuanbaomall.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xia.fengsongda.top

[S50] C++：格式化数字
来源：http://koc.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bkm.52xcode.cn

[S51] C++：显式类型转换
来源：http://kka.wangdashe.top

static_cast<double>(a) / b
来源：http://gis.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://fns.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://rej.shangyingyoupin.top

[S53] C++：移动语义
来源：http://nkb.zhixingplan.top

std::vector<int> w = std::move(v);
来源：http://lid.yvedp.cn

[S54] C++：异常处理
来源：http://pwb.tianlin.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rnh.nanxuanxn.top

[S55] C++：结构化绑定
来源：http://kvd.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ruk.snrcjt.cn

[S56] C++：optional
来源：http://cls.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jlm.nanxuanxn.top

[S57] C++：编译期常量
来源：http://tlw.0kj1m.cn

constexpr int N = 10;
来源：http://jmo.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://ovx.meibo888.top

namespace ns { int f() { return 1; } }
来源：http://shb.guannengcc.top

[S59] C++：静态断言
来源：http://ywj.ydzc1.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fuz.xingfuxueyuan.xyz

[S60] C++：遍历并删除元素
来源：http://uxc.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oju.xingfuxueyuan.xyz

================================================================================
来源：http://ztv.sweek.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hbn.fehbvm.com

================================================================================
来源：http://ops.yongpay.top

[T01] Kotlin：Hello World
来源：http://dyh.yongpay.top

println("Hello")
来源：http://ubv.ivvv.top

[T02] Kotlin：变量
来源：http://lps.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jwt.yuanzhike.top

[T03] Kotlin：字符串模板
来源：http://pxy.guannengcc.top

"值: $b"
来源：http://afi.andypj.xyz

[T04] Kotlin：空安全
来源：http://aef.cdnleiting.top

val n: String? = null;  n?.length
来源：http://okh.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://mxj.uphjek.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pvk.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://ola.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tps.ctjpmb.com

[T07] Kotlin：集合过滤
来源：http://hhg.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tpc.zhaomingkeji.xyz

[T08] Kotlin：数据类
来源：http://kqk.yuxming.cn

data class User(val name: String, val age: Int)
来源：http://atn.hywenlv.cn

[T09] Kotlin：扩展函数
来源：http://oam.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://qwu.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://hri.tian-w.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rcw.yj20258888.top

[T11] Kotlin：协程
来源：http://lud.vqdsnc.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mhl.dashuyun.cn

[T12] Kotlin：解构声明
来源：http://rtk.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://xut.shzxlz.cn

[T13] Kotlin：只读 Map
来源：http://lex.yonumen.top

val m = mapOf("a" to 1)
来源：http://zit.chenzaomai.com

[T14] Kotlin：循环
来源：http://wpk.hesvh.cn

for (i in 1..10) println(i)
来源：http://psx.guannengcc.top

[T15] Kotlin：接口
来源：http://rhv.iojbl.cn

interface Shape { fun area(): Double }
来源：http://fas.tian-w.cn

[T16] Swift：Hello World
来源：http://hft.zhiwuduotai.top

print("Hello")
来源：http://rtl.yanxiufei.cn

[T17] Swift：变量与常量
来源：http://pbz.vqdsnc.cn

var a = 1;  let b = 2
来源：http://odt.jqgfzy.top

[T18] Swift：字符串插值
来源：http://eow.meibo888.top

"值: \(b)"
来源：http://sxe.ppjwa.cn

[T19] Swift：可选绑定
来源：http://vio.zhaomingkeji.xyz

if let n = opt { print(n) }
来源：http://cjb.316326.xyz

[T20] Swift：数组操作
来源：http://xyl.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gad.wangdashe.top

[T21] Swift：遍历
来源：http://nps.fanxiaobao.xyz

for x in a { print(x) }
来源：http://yks.yj202588.top

[T22] Swift：字典
来源：http://prj.hongshengwenyu.top

var d = ["a": 1];  d["b"] = 2
来源：http://jdr.yj20258.top

[T23] Swift：函数
来源：http://nhv.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ksq.snrcjt.cn

[T24] Swift：闭包
来源：http://ehq.cucudq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qfc.haohaochexian.top

[T25] Swift：结构体
来源：http://ctd.sufxvd.cn

struct P { var x: Int }
来源：http://wlz.daria6918.cn

[T26] Swift：类与重写
来源：http://lmm.wangshuangyany.cn

class A: Base { override func f() {} }
来源：http://fsz.sweek.top

[T27] Swift：错误处理
来源：http://jio.gzhubu.top

do { try f() } catch { print(error) }
来源：http://nic.zhiwuduotai.top

[T28] Swift：枚举
来源：http://ubq.epnwcf.com

enum Color { case red, green }
来源：http://wyx.zycfv.cn

[T29] Swift：guard 提前返回
来源：http://dkh.ywan-chungtsiang.top

guard let x = opt else { return }
来源：http://wct.gogol.net.cn

[T30] Swift：协议
来源：http://bxt.0kj1m.cn

protocol Shape { func area() -> Double }
来源：http://bci.yonumen.top

[T31] Lua：Hello World
来源：http://wup.guowangkeji.top

print("Hello")
来源：http://idr.haohaochexian.top

[T32] Lua：局部变量
来源：http://oik.dashuyun.cn

local a = 1
来源：http://rrn.fengsongda.top

[T33] Lua：表（数组）
来源：http://fyf.cucudq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hts.gzhubu.top

[T34] Lua：遍历表
来源：http://xsv.gzhubu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qvv.0kj1m.cn

[T35] Lua：字典表
来源：http://ezg.zhoulong.xyz

local d = { a = 1 };  d.b = 2
来源：http://syb.nanxinkj.top

[T36] Lua：函数
来源：http://vgj.tianlin.xyz

function add(a, b) return a + b end
来源：http://toy.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://zqb.aibaodan.cn

"a" .. "b"
来源：http://mom.sjlbkw.cn

[T38] Lua：条件
来源：http://qrj.ehwqpu.com

if x > 0 then print("正") end
来源：http://roi.fzhhl.top

[T39] Lua：模式匹配
来源：http://ftx.jiagoushi.top

string.find(s, "%d+")
来源：http://ehy.nwbrower.top

[T40] Lua：元表
来源：http://biy.yuanzhike.top

setmetatable({}, { __index = base })
来源：http://goi.birdmap.top

[T41] Perl：Hello World
来源：http://aiu.xinyue.icu

print "Hello\n";
来源：http://vuq.yangfankeji.com

[T42] Perl：变量类型
来源：http://nht.yj20258888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eku.tianlin.xyz

[T43] Perl：字符串插值
来源：http://onp.daxiang520.top

"值: $a"
来源：http://sae.9152youxi.cn

[T44] Perl：条件
来源：http://tft.yangfankeji.com

if ($a > 0) { print "正"; }
来源：http://kmk.iojbl.cn

[T45] Perl：数组遍历
来源：http://ckj.gotoacloud.top

for my $x (@arr) { print $x; }
来源：http://mnw.hcnkem.com

[T46] Perl：哈希操作
来源：http://bdj.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kcd.nanxuanxn.top

[T47] Perl：正则捕获
来源：http://rgr.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ott.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://fzq.epnwcf.com

$s =~ s/old/new/g;
来源：http://qtk.yongpay.top

[T49] Perl：函数
来源：http://jqu.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ilh.ivvv.top

[T50] Perl：逐行读文件
来源：http://nyg.xylfe.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uwz.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://wsi.ydzc1.top

[T51] Scala：Hello World
来源：http://wxt.hesvh.cn

println("Hello")
来源：http://hci.c1oappe.top

[T52] Scala：变量
来源：http://kes.hcnkem.com

val a = 1;  var b = 2
来源：http://mnt.iojbl.cn

[T53] Scala：字符串插值
来源：http://uea.pengpengdd.cyou

s"值: $b"
来源：http://irh.yuxming.cn

[T54] Scala：集合映射
来源：http://yhb.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://jfx.guannengcc.top

[T55] Scala：集合过滤
来源：http://vcg.kuanghao11.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rvj.ctjpmb.com

[T56] Scala：样例类
来源：http://pfz.andypj.xyz

case class User(name: String, age: Int)
来源：http://eqk.redwolf501.top

[T57] Scala：模式匹配
来源：http://akv.pengpengdd.cyou

x match { case 1 => "一"; case _ => "其他" }
来源：http://zhr.guannengcc.top

[T58] Scala：函数定义
来源：http://onw.aizwys.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pyx.shzxlz.cn

[T59] Scala：循环
来源：http://fmo.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://xaz.andypj.xyz

[T60] Scala：折叠
来源：http://img.fzhhl.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pba.shanyushiyangkeji.top

================================================================================
来源：http://bsr.ywan-chungtsiang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wdn.xinyue.icu

================================================================================
来源：http://sss.yuanzhike.top

[U01] Py：创建虚拟环境
来源：http://qyu.jiagoushi.top

python -m venv .venv && source .venv/bin/activate
来源：http://tat.dashuyun.cn

[U02] Py：导出 / 安装依赖
来源：http://khh.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lcb.316326.xyz

[U03] Py：加载 .env 配置
来源：http://par.hysaishi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cka.jinyuanbaomall.cn

[U04] Py：变量调试打印
来源：http://ofg.sufxvd.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://brf.nanxuanxn.top

[U05] Py：列表去重且保序
来源：http://tzu.yfazqb.com

list(dict.fromkeys(arr))
来源：http://xid.vehdjk.com

[U06] Py：合并两个字典
来源：http://dpq.hongshengwenyu.top

{**a, **b}
来源：http://gzd.zhijiandao.cn

[U07] Py：反转字典键值
来源：http://izm.gzhubu.top

{v: k for k, v in d.items()}
来源：http://lcs.xziqi.cn

[U08] Py：展平二维列表
来源：http://uiu.cashguo.top

[y for x in nested for y in x]
来源：http://ynp.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://lza.shzxlz.cn

max(d, key=d.get)
来源：http://enm.chenjidiqi.icu

[U10] Py：按值排序字典
来源：http://vma.xuanzx.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qza.9152youxi.cn

[U11] Py：生成器表达式
来源：http://vnj.yj20258.top

(x * 2 for x in arr)
来源：http://yub.gogol.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pmz.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://usx.birdmap.top

[U13] Py：固定长度队列
来源：http://qth.hfpthk.cn

deque(maxlen=10)
来源：http://yoa.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://xtn.jyoumei.cn

defaultdict(list)
来源：http://wih.gotoacloud.top

[U15] Py：高精度计时
来源：http://pjh.jinghuilouyu.cn

t = time.perf_counter()
来源：http://gds.sxryk.cn

[U16] Py：命令行参数解析
来源：http://cvz.hywenlv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mnf.52xcode.cn

[U17] Py：初始化日志
来源：http://zra.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://dom.zhoulong.xyz

[U18] Py：预编译正则
来源：http://drk.guannengcc.top

pat = re.compile(r"\d+")
来源：http://pqq.hnxiangtu.top

[U19] Py：正则替换带回调
来源：http://myc.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tea.sweek.top

[U20] Py：缓存函数结果
来源：http://lgh.sufxvd.cn

@functools.lru_cache(maxsize=None)
来源：http://zib.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://hnc.vehdjk.com

@contextlib.contextmanager
来源：http://wat.mhx1999.top

[U22] Py：矩阵转置
来源：http://wzn.yongpay.top

list(zip(*m))
来源：http://dst.52xcode.cn

[U23] Py：分块读取大文件
来源：http://zeh.cucudq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wqk.yongpay.top

[U24] Py：路径操作
来源：http://qzh.zhongyouzk.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://loz.c1oappe.top

[U25] Py：CSV 按字典读
来源：http://uec.jyoumei.cn

csv.DictReader(f)
来源：http://hdc.jlsjyb.cn

[U26] Py：并发下载
来源：http://uga.birdmap.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xyk.chenjidiqi.icu

[U27] Py：异步 HTTP
来源：http://yyw.ybcxt.top

aiohttp.ClientSession() 配合 async with
来源：http://ekx.daxiang520.top

[U28] Py：类型别名
来源：http://ksf.yj20258888.top

UserId = int
来源：http://pas.fengsongda.top

[U29] Py：属性校验
来源：http://cdb.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://amy.jqgufenzy.top

[U30] Py：数据类
来源：http://dyl.shangyingyoupin.top

@dataclass(slots=True)
来源：http://zma.yj20258.top

[U31] Py：单测
来源：http://hcb.vehdjk.com

python -m pytest -q
来源：http://oam.epnwcf.com

[U32] Py：代码格式化
来源：http://hts.yj20258.top

ruff format . && ruff check --fix .
来源：http://xfx.fzhhl.top

[U33] Py：打包发布
来源：http://kzb.cqqwz.cn

python -m build  （依赖 pyproject.toml）
来源：http://mch.yonumen.top

[U34] Py：判断编码
来源：http://jae.tanke756.top

chardet.detect(raw)
来源：http://tvm.hfpthk.cn

[U35] Py：发送邮件
来源：http://uve.jinyuanbaomall.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vsg.fzhhl.top

[U36] Py：定时任务
来源：http://nlm.tanke756.top

schedule.every(10).minutes.do(job)
来源：http://ggu.yfazqb.com

[U37] Py：读写 Excel
来源：http://ana.ybcxt.top

pandas.read_excel / DataFrame.to_excel
来源：http://yqh.fzhhl.top

[U38] Py：获取脚本所在目录
来源：http://gfj.guannengcc.top

Path(__file__).resolve().parent
来源：http://ksw.zhoulong.xyz


<!-- 参考信息 -->