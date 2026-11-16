代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://tqs.hesvh.cn

[S15] C：类型转换
来源：http://fbr.guannengcc.top

(double) a / b
来源：http://wgc.fktsv.cn

[S16] C：位操作置位
来源：http://bmi.havefunace.top

x |= (1 << 3);
来源：http://yfp.yonumen.top

[S17] C：安全拼接字符串
来源：http://czh.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ktw.hfpthk.cn

[S18] C：命令行参数
来源：http://fkx.dianchejie.cn

int main(int argc, char **argv)
来源：http://vyf.sjlbkw.cn

[S19] C：快速排序
来源：http://lsu.hfpthk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ppl.hnqzz.top

[S20] C：二分查找
来源：http://fvo.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sof.gaohongyu789.top

[S21] C：字符类别判断
来源：http://pfd.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://syp.c1oappe.top

[S22] C：字符串转数字
来源：http://saa.xuetiantiany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://svu.sysykeji.top

[S23] C：随机数
来源：http://dmk.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qrh.ivvv.top

[S24] C：获取本地时间
来源：http://loj.zhiwuduotai.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rsg.fzhhl.top

[S25] C：内存拷贝
来源：http://lgb.daria6918.cn

memcpy(dst, src, n);
来源：http://sxf.gaohongyu789.top

[S26] C：内存清零
来源：http://vne.daria6918.cn

memset(a, 0, sizeof a);
来源：http://vih.dashuyun.cn

[S27] C：定义常量
来源：http://szp.nanxinkj.top

const double PI = 3.14159;
来源：http://yga.zhengqikj.top

[S28] C：静态变量
来源：http://ohx.hammf.cn

static int counter = 0;
来源：http://svf.tarul.cn

[S29] C：变参函数
来源：http://vme.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mrg.gogol.net.cn

[S30] C：头文件保护
来源：http://nia.hywenlv.cn

#ifndef X_H
来源：http://tmp.yvedp.cn

#define X_H
来源：http://bvx.xziqi.cn

#endif
来源：http://gen.havefunace.top

[S31] C++：Hello World
来源：http://lmb.zhoulong.xyz

#include <iostream>
来源：http://wea.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://txy.chenzaomai.com

[S32] C++：字符串
来源：http://aaz.tanke756.top

std::string s = "hi";  s += "!";
来源：http://gaf.shanyushiyangtech.top

[S33] C++：vector 增删
来源：http://plz.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sgv.fengsongda.top

[S34] C++：遍历 vector
来源：http://xpa.52xcode.cn

for (auto &x : v) { std::cout << x; }
来源：http://ghh.dashuyun.cn

[S35] C++：map
来源：http://nki.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ipm.hcnkem.com

[S36] C++：unordered_map
来源：http://kbp.gogol.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sau.chenjidiqi.icu

[S37] C++：set
来源：http://sic.xingfuxueyuan.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ome.fzhhl.top

[S38] C++：排序
来源：http://hqg.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://mth.cdnleiting.top

[S39] C++：自定义比较器排序
来源：http://ezp.zhoulong.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sdq.jqgfzy.top

[S40] C++：查找元素
来源：http://upo.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yaw.hnqzz.top

[S41] C++：类与构造函数
来源：http://hzj.daria6918.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://neb.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://knn.shanyushiyangkeji.top

class B : public Base { public: void f() override {} };
来源：http://dhq.gotoacloud.top

[S43] C++：智能指针
来源：http://waj.snrcjt.cn

auto p = std::make_unique<int>(5);
来源：http://ttd.hysaishi.cn

[S44] C++：引用传参
来源：http://qmk.nwbrower.top

void inc(int &x) { ++x; }
来源：http://ssc.mhx1999.top

[S45] C++：lambda
来源：http://ojb.daxiang520.top

auto add = [](int a, int b) { return a + b; };
来源：http://wpv.gotoacloud.top

[S46] C++：函数模板
来源：http://olu.chenlongwang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rgg.fktsv.cn

[S47] C++：结构化绑定遍历
来源：http://csy.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zel.ydzc1.top

[S48] C++：逐行读文件
来源：http://soh.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://spz.zhiwuduotai.top

while (std::getline(in, line)) { }
来源：http://xuo.zdbjq.cn

[S49] C++：写文件
来源：http://ege.ctjpmb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ilv.fehbvm.com

[S50] C++：格式化数字
来源：http://fjb.jlsjyb.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mdk.meibo888.top

[S51] C++：显式类型转换
来源：http://apu.aibaodan.cn

static_cast<double>(a) / b
来源：http://gzd.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://glf.hesvh.cn

int size() const noexcept { return n_; }
来源：http://qem.svipenyu.cn

[S53] C++：移动语义
来源：http://lec.jinyuanbaomall.cn

std::vector<int> w = std::move(v);
来源：http://qus.ybcxt.top

[S54] C++：异常处理
来源：http://kqy.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rxb.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://xqs.andypj.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://cyb.zhiwuduotai.top

[S56] C++：optional
来源：http://zrl.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jrm.bjfxy.top

[S57] C++：编译期常量
来源：http://uzu.hfpthk.cn

constexpr int N = 10;
来源：http://ipb.yvedp.cn

[S58] C++：命名空间
来源：http://kfx.yj202588.top

namespace ns { int f() { return 1; } }
来源：http://mzx.pengpengdd.cyou

[S59] C++：静态断言
来源：http://hkm.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cen.tanke756.top

[S60] C++：遍历并删除元素
来源：http://yqr.zhixingplan.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://utb.zhixingplan.top

================================================================================
来源：http://jmz.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vxv.aibaodan.cn

================================================================================
来源：http://vnq.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://xyo.sweek.top

println("Hello")
来源：http://iap.ivvv.top

[T02] Kotlin：变量
来源：http://hxu.fehbvm.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tfe.yongpay.top

[T03] Kotlin：字符串模板
来源：http://xxb.cdnleiting.top

"值: $b"
来源：http://zzi.yuanzhike.top

[T04] Kotlin：空安全
来源：http://wft.redwolf501.top

val n: String? = null;  n?.length
来源：http://bck.yj20258.top

[T05] Kotlin：when 表达式
来源：http://ppx.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lqk.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://tcf.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://toy.hywenlv.cn

[T07] Kotlin：集合过滤
来源：http://wfj.jinqigfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zac.hnqzz.top

[T08] Kotlin：数据类
来源：http://amh.jlsjyb.cn

data class User(val name: String, val age: Int)
来源：http://crs.fengsongda.top

[T09] Kotlin：扩展函数
来源：http://znk.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://yog.wangshuangyany.cn

[T10] Kotlin：默认参数
来源：http://nci.gzhubu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bbn.nanxinkj.top

[T11] Kotlin：协程
来源：http://irx.yangfankeji.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://oez.gzhubu.top

[T12] Kotlin：解构声明
来源：http://koa.zhoulong.xyz

val (a, b) = Pair(1, 2)
来源：http://dgw.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://lod.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://gyr.c1oappe.top

[T14] Kotlin：循环
来源：http://puc.bbcook.cn

for (i in 1..10) println(i)
来源：http://ugh.hywenlv.cn

[T15] Kotlin：接口
来源：http://ovj.fzhhl.top

interface Shape { fun area(): Double }
来源：http://joe.sjlbkw.cn

[T16] Swift：Hello World
来源：http://ddu.nwbrower.top

print("Hello")
来源：http://fsq.shzxlz.cn

[T17] Swift：变量与常量
来源：http://zvs.yfazqb.com

var a = 1;  let b = 2
来源：http://kxk.shzxlz.cn

[T18] Swift：字符串插值
来源：http://sbq.mhx1999.top

"值: \(b)"
来源：http://prf.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://tho.sweek.top

if let n = opt { print(n) }
来源：http://yjo.gaohongyu789.top

[T20] Swift：数组操作
来源：http://wce.fzhhl.top

var a = [1, 2, 3];  a.append(4)
来源：http://yfx.jlsjyb.cn

[T21] Swift：遍历
来源：http://drv.yueranfly.top

for x in a { print(x) }
来源：http://vjy.ppjwa.cn

[T22] Swift：字典
来源：http://wao.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://fql.52xcode.cn

[T23] Swift：函数
来源：http://whk.hcnkem.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://izd.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://roo.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uwx.redwolf501.top

[T25] Swift：结构体
来源：http://zvp.wangdashe.top

struct P { var x: Int }
来源：http://jif.gzhubu.top

[T26] Swift：类与重写
来源：http://rkw.zdbjq.cn

class A: Base { override func f() {} }
来源：http://erh.iojbl.cn

[T27] Swift：错误处理
来源：http://ate.shangyingyoupin.top

do { try f() } catch { print(error) }
来源：http://bti.cashguo.top

[T28] Swift：枚举
来源：http://qjy.dashuyun.cn

enum Color { case red, green }
来源：http://nyt.mhx1999.top

[T29] Swift：guard 提前返回
来源：http://qwy.yueranfly.top

guard let x = opt else { return }
来源：http://ttr.chenzaomai.com

[T30] Swift：协议
来源：http://iwy.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://oxh.yangfankeji.com

[T31] Lua：Hello World
来源：http://ehd.chenzaomai.com

print("Hello")
来源：http://ojo.gaohongyu789.top

[T32] Lua：局部变量
来源：http://jmk.aizwys.cn

local a = 1
来源：http://fqg.fengsongda.top

[T33] Lua：表（数组）
来源：http://irz.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://thv.fzhhl.top

[T34] Lua：遍历表
来源：http://kmd.jinyuanbaomall.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nxz.bbcook.cn

[T35] Lua：字典表
来源：http://wog.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://egx.yanxiufei.cn

[T36] Lua：函数
来源：http://lws.chenzaomai.com

function add(a, b) return a + b end
来源：http://qhu.tianlin.xyz

[T37] Lua：字符串拼接
来源：http://ncz.tarul.cn

"a" .. "b"
来源：http://cqy.sxryk.cn

[T38] Lua：条件
来源：http://wis.tianlin.xyz

if x > 0 then print("正") end
来源：http://dpo.hfpthk.cn

[T39] Lua：模式匹配
来源：http://muj.uphjek.com

string.find(s, "%d+")
来源：http://rix.svipenyu.cn

[T40] Lua：元表
来源：http://bms.shanyushiyangtech.top

setmetatable({}, { __index = base })
来源：http://exz.ydzc1.top

[T41] Perl：Hello World
来源：http://tlh.sysykeji.top

print "Hello\n";
来源：http://dsb.xziqi.cn

[T42] Perl：变量类型
来源：http://hjr.ydzc1.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kkz.ydzc1.top

[T43] Perl：字符串插值
来源：http://hzh.zhixingplan.top

"值: $a"
来源：http://cvf.tanke756.top

[T44] Perl：条件
来源：http://msn.zhongyouzk.top

if ($a > 0) { print "正"; }
来源：http://vrz.vehdjk.com

[T45] Perl：数组遍历
来源：http://grz.yanxiufei.cn

for my $x (@arr) { print $x; }
来源：http://kpx.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://jpp.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rwa.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://oym.c1oappe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vek.andypj.xyz

[T48] Perl：正则替换
来源：http://ogv.iojbl.cn

$s =~ s/old/new/g;
来源：http://ctr.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://nru.chenjidiqi.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jrb.nwbrower.top

[T50] Perl：逐行读文件
来源：http://mrv.zhongyouzk.top

open my $fh, "<", "a.txt" or die $!;
来源：http://erv.fengsongda.top

while (my $line = <$fh>) { print $line; }
来源：http://irg.zhengqikj.top

[T51] Scala：Hello World
来源：http://mqz.yj20258.top

println("Hello")
来源：http://xoo.zycfv.cn

[T52] Scala：变量
来源：http://cyv.0kj1m.cn

val a = 1;  var b = 2
来源：http://kaw.tanke756.top

[T53] Scala：字符串插值
来源：http://gfc.zhengqikj.top

s"值: $b"
来源：http://ihw.sysykeji.top

[T54] Scala：集合映射
来源：http://clc.epnwcf.com

List(1, 2, 3).map(_ * 2)
来源：http://pel.tianlin.xyz

[T55] Scala：集合过滤
来源：http://lzl.jinghuilouyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gtr.cucudq.cn

[T56] Scala：样例类
来源：http://kty.xziqi.cn

case class User(name: String, age: Int)
来源：http://gih.feifeiyinyue.top

[T57] Scala：模式匹配
来源：http://vqe.chenzaomai.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://xqr.nanxinkj.top

[T58] Scala：函数定义
来源：http://xvw.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://jxh.iojbl.cn

[T59] Scala：循环
来源：http://dlu.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://gry.0kj1m.cn

[T60] Scala：折叠
来源：http://tib.xingfuxueyuan.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ywv.xuetiantiany.cn

================================================================================
来源：http://gdb.svipenyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fxj.cdnleiting.top

================================================================================
来源：http://yww.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://jdu.hnqzz.top

python -m venv .venv && source .venv/bin/activate
来源：http://byl.jinqigufen.top

[U02] Py：导出 / 安装依赖
来源：http://ohj.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rwr.uphjek.com

[U03] Py：加载 .env 配置
来源：http://hqb.hammf.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gcu.bjfxy.top

[U04] Py：变量调试打印
来源：http://yei.jlsjyb.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lit.ybcxt.top

[U05] Py：列表去重且保序
来源：http://txs.sufxvd.cn

list(dict.fromkeys(arr))
来源：http://fqj.aizwys.cn

[U06] Py：合并两个字典
来源：http://rkh.chenzaomai.com

{**a, **b}
来源：http://ida.xinyue.icu

[U07] Py：反转字典键值
来源：http://ahg.hysaishi.cn

{v: k for k, v in d.items()}
来源：http://ocv.shuidangran.top

[U08] Py：展平二维列表
来源：http://tjk.yuanzhike.top

[y for x in nested for y in x]
来源：http://dvt.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://mpv.gzhubu.top

max(d, key=d.get)
来源：http://gop.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://rxq.andypj.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xgc.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://fcu.chenlongwang.top

(x * 2 for x in arr)
来源：http://xzi.meibo888.top

[U12] Py：取出现最多的 3 个元素
来源：http://zzy.yfazqb.com

Counter(arr).most_common(3)
来源：http://ngc.yfazqb.com

[U13] Py：固定长度队列
来源：http://pam.snrcjt.cn

deque(maxlen=10)
来源：http://lkb.jiagoushi.top

[U14] Py：分组收集到列表
来源：http://pul.bjfxy.top

defaultdict(list)
来源：http://tnw.sxryk.cn

[U15] Py：高精度计时
来源：http://eeg.jyoumei.cn

t = time.perf_counter()
来源：http://pqj.hesvh.cn

[U16] Py：命令行参数解析
来源：http://mhg.cdnleiting.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lhr.tianlin.xyz

[U17] Py：初始化日志
来源：http://zaw.cashguo.top

logging.basicConfig(level=logging.INFO)
来源：http://bta.fzhhl.top

[U18] Py：预编译正则
来源：http://yxk.xziqi.cn

pat = re.compile(r"\d+")
来源：http://kvd.wangdashe.top

[U19] Py：正则替换带回调
来源：http://giu.dashuyun.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ckp.havefunace.top

[U20] Py：缓存函数结果
来源：http://xer.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://bpo.shangyingyoupin.top

[U21] Py：自定义上下文管理器
来源：http://ivg.yongpay.top

@contextlib.contextmanager
来源：http://slj.yueranfly.top

[U22] Py：矩阵转置
来源：http://aza.meibo888.top

list(zip(*m))
来源：http://zkr.jinghuilouyu.cn

[U23] Py：分块读取大文件
来源：http://ybi.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fyz.dashuyun.cn

[U24] Py：路径操作
来源：http://ois.nanxinkj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://osr.nwbrower.top

[U25] Py：CSV 按字典读
来源：http://zid.pycfn.com

csv.DictReader(f)
来源：http://bwx.cashguo.top

[U26] Py：并发下载
来源：http://mjj.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lbi.zhiwuduotai.top

[U27] Py：异步 HTTP
来源：http://ahy.jqgufenzy.top

aiohttp.ClientSession() 配合 async with
来源：http://wvo.zhiwuduotai.top

[U28] Py：类型别名
来源：http://bqg.ivvv.top

UserId = int
来源：http://wtl.quarkkingdee.top

[U29] Py：属性校验
来源：http://yqa.zhongyouzk.top

@property 与 @x.setter 配合
来源：http://dck.jinqigufen.top

[U30] Py：数据类
来源：http://dpc.hywenlv.cn

@dataclass(slots=True)
来源：http://cok.tian-w.cn

[U31] Py：单测
来源：http://jta.nwbrower.top

python -m pytest -q
来源：http://tra.redwolf501.top

[U32] Py：代码格式化
来源：http://xoh.hnqzz.top

ruff format . && ruff check --fix .
来源：http://nfe.jinqigufen.top

[U33] Py：打包发布
来源：http://kys.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://kbw.nanxuanxn.top

[U34] Py：判断编码
来源：http://jpe.yonumen.top

chardet.detect(raw)
来源：http://uwc.tarul.cn

[U35] Py：发送邮件
来源：http://lqz.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ftr.yuxming.cn

[U36] Py：定时任务
来源：http://vno.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://ntu.havefunace.top

[U37] Py：读写 Excel
来源：http://qft.ctjpmb.com

pandas.read_excel / DataFrame.to_excel
来源：http://bwu.tianlin.xyz

[U38] Py：获取脚本所在目录
来源：http://xax.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://wjk.shanyushiyangkeji.top


<!-- 参考信息 -->