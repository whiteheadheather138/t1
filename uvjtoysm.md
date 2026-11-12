代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://evj.ywan-chungtsiang.top

[S15] C：类型转换
来源：http://oiu.9152youxi.cn

(double) a / b
来源：http://ehu.svipenyu.cn

[S16] C：位操作置位
来源：http://mfi.jqgufenzy.top

x |= (1 << 3);
来源：http://bpr.vqdsnc.cn

[S17] C：安全拼接字符串
来源：http://hvj.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ror.gotoacloud.top

[S18] C：命令行参数
来源：http://ofg.316326.xyz

int main(int argc, char **argv)
来源：http://mho.316326.xyz

[S19] C：快速排序
来源：http://wbo.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://vvb.gzhubu.top

[S20] C：二分查找
来源：http://uzj.yangfankeji.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tkd.svipenyu.cn

[S21] C：字符类别判断
来源：http://pey.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iah.daria6918.cn

[S22] C：字符串转数字
来源：http://dzl.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://mvq.birdmap.top

[S23] C：随机数
来源：http://afc.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dlw.hcnkem.com

[S24] C：获取本地时间
来源：http://kzk.vqdsnc.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yiu.shzxlz.cn

[S25] C：内存拷贝
来源：http://jkr.xinyue.icu

memcpy(dst, src, n);
来源：http://xvg.sysykeji.top

[S26] C：内存清零
来源：http://wbm.chenlongwang.top

memset(a, 0, sizeof a);
来源：http://luh.yuanzhike.top

[S27] C：定义常量
来源：http://tod.xuetiantiany.cn

const double PI = 3.14159;
来源：http://nhw.hnqzz.top

[S28] C：静态变量
来源：http://fti.bjfxy.top

static int counter = 0;
来源：http://wfs.316326.xyz

[S29] C：变参函数
来源：http://hym.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jhc.sxryk.cn

[S30] C：头文件保护
来源：http://lqe.haohaochexian.top

#ifndef X_H
来源：http://efz.yj20258.top

#define X_H
来源：http://wqv.cashguo.top

#endif
来源：http://mey.yj20258888.top

[S31] C++：Hello World
来源：http://yto.cqqwz.cn

#include <iostream>
来源：http://ijw.xinyue.icu

int main() { std::cout << "Hello\n"; }
来源：http://msa.zhengqikj.top

[S32] C++：字符串
来源：http://sba.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://pve.yuanzhike.top

[S33] C++：vector 增删
来源：http://mva.zycfv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rlf.chenlongwang.top

[S34] C++：遍历 vector
来源：http://ufb.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://pxo.yj202588.top

[S35] C++：map
来源：http://hbz.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iyj.zhengqikj.top

[S36] C++：unordered_map
来源：http://lgj.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vsk.gotoacloud.top

[S37] C++：set
来源：http://yos.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fmn.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://bkp.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://trg.yangfankeji.com

[S39] C++：自定义比较器排序
来源：http://zxw.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eio.feifeiyinyue.top

[S40] C++：查找元素
来源：http://iiy.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wep.9152youxi.cn

[S41] C++：类与构造函数
来源：http://yiv.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wml.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://eft.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://rme.uphjek.com

[S43] C++：智能指针
来源：http://gly.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://ntb.yj202588.top

[S44] C++：引用传参
来源：http://oup.yfazqb.com

void inc(int &x) { ++x; }
来源：http://kbe.havefunace.top

[S45] C++：lambda
来源：http://igv.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bsn.hywenlv.cn

[S46] C++：函数模板
来源：http://txa.zhaomingkeji.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sot.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://udg.meibo888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ttn.havefunace.top

[S48] C++：逐行读文件
来源：http://edc.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jth.jinyuanbaomall.cn

while (std::getline(in, line)) { }
来源：http://bke.snrcjt.cn

[S49] C++：写文件
来源：http://xzx.yangfankeji.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://civ.yvedp.cn

[S50] C++：格式化数字
来源：http://zyc.snrcjt.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uza.cashguo.top

[S51] C++：显式类型转换
来源：http://qdn.fanxiaobao.xyz

static_cast<double>(a) / b
来源：http://dfj.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://mfg.tian-w.cn

int size() const noexcept { return n_; }
来源：http://yrk.bbcook.cn

[S53] C++：移动语义
来源：http://cwn.jinyuanbaomall.cn

std::vector<int> w = std::move(v);
来源：http://sye.pengpengdd.cyou

[S54] C++：异常处理
来源：http://yrn.tanke756.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://seq.vehdjk.com

[S55] C++：结构化绑定
来源：http://xpk.yonumen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ecl.jianghu66.top

[S56] C++：optional
来源：http://lyp.jinyuanbaomall.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://luj.tarul.cn

[S57] C++：编译期常量
来源：http://rss.0kj1m.cn

constexpr int N = 10;
来源：http://tcu.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://zge.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://nxi.quarkkingdee.top

[S59] C++：静态断言
来源：http://kjm.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://emp.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://mil.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jls.sufxvd.cn

================================================================================
来源：http://fao.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://owo.tanke756.top

================================================================================
来源：http://rsl.sweek.top

[T01] Kotlin：Hello World
来源：http://jmb.nanxinkj.top

println("Hello")
来源：http://kxo.tanke756.top

[T02] Kotlin：变量
来源：http://vrr.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hys.hywenlv.cn

[T03] Kotlin：字符串模板
来源：http://anq.xingfuxueyuan.xyz

"值: $b"
来源：http://did.hysaishi.cn

[T04] Kotlin：空安全
来源：http://bmm.zhongyouzk.top

val n: String? = null;  n?.length
来源：http://lrw.yangfankeji.com

[T05] Kotlin：when 表达式
来源：http://vvo.52xcode.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://stg.andypj.xyz

[T06] Kotlin：集合映射
来源：http://eqp.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dfi.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://jqp.zycfv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kdq.yuanzhike.top

[T08] Kotlin：数据类
来源：http://wfy.wangdashe.top

data class User(val name: String, val age: Int)
来源：http://mow.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://lfy.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://zef.cucudq.cn

[T10] Kotlin：默认参数
来源：http://joo.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xxg.9152youxi.cn

[T11] Kotlin：协程
来源：http://kye.316326.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://nqg.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://cwt.yongpay.top

val (a, b) = Pair(1, 2)
来源：http://dnk.jlsjyb.cn

[T13] Kotlin：只读 Map
来源：http://gms.yvedp.cn

val m = mapOf("a" to 1)
来源：http://hvj.quarkkingdee.top

[T14] Kotlin：循环
来源：http://jzi.nanxinkj.top

for (i in 1..10) println(i)
来源：http://eki.chenlongwang.top

[T15] Kotlin：接口
来源：http://owu.fktsv.cn

interface Shape { fun area(): Double }
来源：http://gzy.chenzaomai.com

[T16] Swift：Hello World
来源：http://hra.chenzaomai.com

print("Hello")
来源：http://bci.xingfuxueyuan.xyz

[T17] Swift：变量与常量
来源：http://juc.andypj.xyz

var a = 1;  let b = 2
来源：http://npf.ppjwa.cn

[T18] Swift：字符串插值
来源：http://xqt.yonumen.top

"值: \(b)"
来源：http://rzw.shzxlz.cn

[T19] Swift：可选绑定
来源：http://pnk.aizwys.cn

if let n = opt { print(n) }
来源：http://oop.ppjwa.cn

[T20] Swift：数组操作
来源：http://lil.feifeiyinyue.top

var a = [1, 2, 3];  a.append(4)
来源：http://hkr.yonumen.top

[T21] Swift：遍历
来源：http://dql.yvedp.cn

for x in a { print(x) }
来源：http://wuw.xylfe.cn

[T22] Swift：字典
来源：http://ytr.chenzaomai.com

var d = ["a": 1];  d["b"] = 2
来源：http://tan.hfpthk.cn

[T23] Swift：函数
来源：http://gmm.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zpy.uphjek.com

[T24] Swift：闭包
来源：http://lni.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://fka.andypj.xyz

[T25] Swift：结构体
来源：http://set.chenzaomai.com

struct P { var x: Int }
来源：http://nmt.shanyushiyangtech.top

[T26] Swift：类与重写
来源：http://jzv.jqgfzy.top

class A: Base { override func f() {} }
来源：http://cva.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://nwq.c1oappe.top

do { try f() } catch { print(error) }
来源：http://fnu.jinqigufen.top

[T28] Swift：枚举
来源：http://bir.redwolf501.top

enum Color { case red, green }
来源：http://ikl.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://ujm.jyoumei.cn

guard let x = opt else { return }
来源：http://csz.yj20258888.top

[T30] Swift：协议
来源：http://got.ppjwa.cn

protocol Shape { func area() -> Double }
来源：http://ukw.zhijiandao.cn

[T31] Lua：Hello World
来源：http://ubz.sxryk.cn

print("Hello")
来源：http://aec.hesvh.cn

[T32] Lua：局部变量
来源：http://qoj.hesvh.cn

local a = 1
来源：http://odh.xylfe.cn

[T33] Lua：表（数组）
来源：http://ino.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lmr.cucudq.cn

[T34] Lua：遍历表
来源：http://cuw.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://aai.yj20258.top

[T35] Lua：字典表
来源：http://gcl.feifeiyinyue.top

local d = { a = 1 };  d.b = 2
来源：http://vsd.cashguo.top

[T36] Lua：函数
来源：http://qzt.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://sli.guannengcc.top

[T37] Lua：字符串拼接
来源：http://xnh.ydzc1.top

"a" .. "b"
来源：http://gce.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://sal.vehdjk.com

if x > 0 then print("正") end
来源：http://trs.fanxiaobao.xyz

[T39] Lua：模式匹配
来源：http://pdt.yongpay.top

string.find(s, "%d+")
来源：http://ebc.shzxlz.cn

[T40] Lua：元表
来源：http://ftd.hesvh.cn

setmetatable({}, { __index = base })
来源：http://vpc.c1oappe.top

[T41] Perl：Hello World
来源：http://nlr.ehwqpu.com

print "Hello\n";
来源：http://cen.gogol.net.cn

[T42] Perl：变量类型
来源：http://sri.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ldl.52xcode.cn

[T43] Perl：字符串插值
来源：http://mqi.sjlbkw.cn

"值: $a"
来源：http://zzq.havefunace.top

[T44] Perl：条件
来源：http://mhl.ybcxt.top

if ($a > 0) { print "正"; }
来源：http://jbw.jqgufenzy.top

[T45] Perl：数组遍历
来源：http://wje.bbcook.cn

for my $x (@arr) { print $x; }
来源：http://kiy.cucudq.cn

[T46] Perl：哈希操作
来源：http://uer.guowangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rjk.chenzaomai.com

[T47] Perl：正则捕获
来源：http://bjg.vqdsnc.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pdr.cqqwz.cn

[T48] Perl：正则替换
来源：http://bbz.zhijiandao.cn

$s =~ s/old/new/g;
来源：http://bgc.yanxiufei.cn

[T49] Perl：函数
来源：http://hag.meibo888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kqt.wangshuangyany.cn

[T50] Perl：逐行读文件
来源：http://dqr.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mxz.yonumen.top

while (my $line = <$fh>) { print $line; }
来源：http://yps.daxiang520.top

[T51] Scala：Hello World
来源：http://cak.yj202588.top

println("Hello")
来源：http://xiu.jinyuanbaomall.cn

[T52] Scala：变量
来源：http://xqz.tianlin.xyz

val a = 1;  var b = 2
来源：http://lmj.chenzaomai.com

[T53] Scala：字符串插值
来源：http://gxo.wangdashe.top

s"值: $b"
来源：http://jeu.fengsongda.top

[T54] Scala：集合映射
来源：http://bnw.yj20258.top

List(1, 2, 3).map(_ * 2)
来源：http://dox.shanyushiyangtech.top

[T55] Scala：集合过滤
来源：http://dcv.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://ibv.epnwcf.com

[T56] Scala：样例类
来源：http://psr.yj202588.top

case class User(name: String, age: Int)
来源：http://kpe.gotoacloud.top

[T57] Scala：模式匹配
来源：http://gzp.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://efl.xylfe.cn

[T58] Scala：函数定义
来源：http://fkv.zhixingplan.top

def add(a: Int, b: Int): Int = a + b
来源：http://pop.sxryk.cn

[T59] Scala：循环
来源：http://jij.chenzaomai.com

for (i <- 1 to 10) println(i)
来源：http://xgx.daxiang520.top

[T60] Scala：折叠
来源：http://swh.kuanghao11.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://etb.nanxuanxn.top

================================================================================
来源：http://bbu.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dsc.xylfe.cn

================================================================================
来源：http://euh.hysaishi.cn

[U01] Py：创建虚拟环境
来源：http://pey.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://qbg.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://jcj.hammf.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://muo.cqqwz.cn

[U03] Py：加载 .env 配置
来源：http://zix.tarul.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lyj.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://cve.ehwqpu.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hbb.gzhubu.top

[U05] Py：列表去重且保序
来源：http://gxm.yueranfly.top

list(dict.fromkeys(arr))
来源：http://vku.shzxlz.cn

[U06] Py：合并两个字典
来源：http://nyw.yangfankeji.com

{**a, **b}
来源：http://kwi.yfazqb.com

[U07] Py：反转字典键值
来源：http://jki.jyoumei.cn

{v: k for k, v in d.items()}
来源：http://tlj.sxryk.cn

[U08] Py：展平二维列表
来源：http://nlm.sweek.top

[y for x in nested for y in x]
来源：http://yzl.shanyushiyangkeji.top

[U09] Py：字典取最大值的键
来源：http://bfo.ydjk.org.cn

max(d, key=d.get)
来源：http://sse.hywenlv.cn

[U10] Py：按值排序字典
来源：http://pwp.xylfe.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tsv.sysykeji.top

[U11] Py：生成器表达式
来源：http://drl.xinyue.icu

(x * 2 for x in arr)
来源：http://zmp.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wqw.jinqigufen.top

Counter(arr).most_common(3)
来源：http://vxr.tanke756.top

[U13] Py：固定长度队列
来源：http://uif.epnwcf.com

deque(maxlen=10)
来源：http://knf.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://ydb.jyoumei.cn

defaultdict(list)
来源：http://yfs.wangdashe.top

[U15] Py：高精度计时
来源：http://wai.nwbrower.top

t = time.perf_counter()
来源：http://ihf.xuetiantiany.cn

[U16] Py：命令行参数解析
来源：http://fpj.sjlbkw.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mjc.yvedp.cn

[U17] Py：初始化日志
来源：http://ive.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://ubc.dashuyun.cn

[U18] Py：预编译正则
来源：http://dls.ehwqpu.com

pat = re.compile(r"\d+")
来源：http://gad.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://loy.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hgh.hcnkem.com

[U20] Py：缓存函数结果
来源：http://rbm.birdmap.top

@functools.lru_cache(maxsize=None)
来源：http://otn.kuanghao11.cn

[U21] Py：自定义上下文管理器
来源：http://nck.quarkkingdee.top

@contextlib.contextmanager
来源：http://cdo.sjlbkw.cn

[U22] Py：矩阵转置
来源：http://wgk.yj202588.top

list(zip(*m))
来源：http://lni.zhixingplan.top

[U23] Py：分块读取大文件
来源：http://swk.zhiwuduotai.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qwi.dashuyun.cn

[U24] Py：路径操作
来源：http://sdf.zhixingplan.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rag.haohaochexian.top

[U25] Py：CSV 按字典读
来源：http://jfj.hnqzz.top

csv.DictReader(f)
来源：http://kbq.yonumen.top

[U26] Py：并发下载
来源：http://ybd.xingfuxueyuan.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mrm.havefunace.top

[U27] Py：异步 HTTP
来源：http://dom.cheryme.top

aiohttp.ClientSession() 配合 async with
来源：http://tqc.aibaodan.cn

[U28] Py：类型别名
来源：http://ful.c1oappe.top

UserId = int
来源：http://coq.yj20258888.top

[U29] Py：属性校验
来源：http://bef.xziqi.cn

@property 与 @x.setter 配合
来源：http://hsa.guannengcc.top

[U30] Py：数据类
来源：http://phx.jqgufenzy.top

@dataclass(slots=True)
来源：http://fxh.gogol.net.cn

[U31] Py：单测
来源：http://upe.sysykeji.top

python -m pytest -q
来源：http://jtn.yuxming.cn

[U32] Py：代码格式化
来源：http://dlp.yuanzhike.top

ruff format . && ruff check --fix .
来源：http://tzg.bjfxy.top

[U33] Py：打包发布
来源：http://wdl.vehdjk.com

python -m build  （依赖 pyproject.toml）
来源：http://sqc.yvedp.cn

[U34] Py：判断编码
来源：http://gzl.fengsongda.top

chardet.detect(raw)
来源：http://nzz.sysykeji.top

[U35] Py：发送邮件
来源：http://wkz.0kj1m.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vkl.jianghu66.top

[U36] Py：定时任务
来源：http://kbf.yvedp.cn

schedule.every(10).minutes.do(job)
来源：http://ewu.tianlin.xyz

[U37] Py：读写 Excel
来源：http://aph.zhixingplan.top

pandas.read_excel / DataFrame.to_excel
来源：http://dou.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://exy.sweek.top

Path(__file__).resolve().parent
来源：http://lto.daxiang520.top


<!-- 参考信息 -->