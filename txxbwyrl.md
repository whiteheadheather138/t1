代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wzd.sweek.top

[S13] C：宏定义
来源：http://cgc.yj20258888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zbh.pycfn.com

[S14] C：枚举
来源：http://yen.epnwcf.com

enum Color { RED, GREEN, BLUE };
来源：http://uwh.shzxlz.cn

[S15] C：类型转换
来源：http://yoc.shanyushiyangkeji.top

(double) a / b
来源：http://gdm.chenlongwang.top

[S16] C：位操作置位
来源：http://crp.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://wwp.ybcxt.top

[S17] C：安全拼接字符串
来源：http://nsx.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nkv.jqgfzy.top

[S18] C：命令行参数
来源：http://vrt.guannengcc.top

int main(int argc, char **argv)
来源：http://rxc.gogol.net.cn

[S19] C：快速排序
来源：http://msa.ywan-chungtsiang.top

qsort(a, n, sizeof(int), cmp);
来源：http://nix.shanyushiyangtech.top

[S20] C：二分查找
来源：http://nhf.sweek.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://crd.dashuyun.cn

[S21] C：字符类别判断
来源：http://mto.guowangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://okk.uphjek.com

[S22] C：字符串转数字
来源：http://urw.zhoulong.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://yhj.nwbrower.top

[S23] C：随机数
来源：http://ccg.pycfn.com

srand(time(NULL));  int r = rand() % 100;
来源：http://xzq.cdnleiting.top

[S24] C：获取本地时间
来源：http://tof.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xuq.nanxinkj.top

[S25] C：内存拷贝
来源：http://mkj.sysykeji.top

memcpy(dst, src, n);
来源：http://pyq.ivvv.top

[S26] C：内存清零
来源：http://wfw.fzhhl.top

memset(a, 0, sizeof a);
来源：http://uch.xziqi.cn

[S27] C：定义常量
来源：http://ppc.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://yeu.vehdjk.com

[S28] C：静态变量
来源：http://tna.ivvv.top

static int counter = 0;
来源：http://bnh.tanke756.top

[S29] C：变参函数
来源：http://mog.aizwys.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sok.yangfankeji.com

[S30] C：头文件保护
来源：http://lqh.hysaishi.cn

#ifndef X_H
来源：http://uap.fktsv.cn

#define X_H
来源：http://yod.yongpay.top

#endif
来源：http://hhe.svipenyu.cn

[S31] C++：Hello World
来源：http://vnh.tianlin.xyz

#include <iostream>
来源：http://qwx.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://neb.zdqjudy.top

[S32] C++：字符串
来源：http://npb.xylfe.cn

std::string s = "hi";  s += "!";
来源：http://eiq.guowangkeji.top

[S33] C++：vector 增删
来源：http://dyh.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xwj.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://vhg.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://yjc.yvedp.cn

[S35] C++：map
来源：http://vzt.kuanghao11.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vjd.jinqigufen.top

[S36] C++：unordered_map
来源：http://nzu.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dsd.fanxiaobao.xyz

[S37] C++：set
来源：http://qgq.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://znc.zhixingplan.top

[S38] C++：排序
来源：http://hdq.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://vub.iojbl.cn

[S39] C++：自定义比较器排序
来源：http://twf.xuetiantiany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rdf.aibaodan.cn

[S40] C++：查找元素
来源：http://bpu.aibaodan.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wyk.yonumen.top

[S41] C++：类与构造函数
来源：http://kjp.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pvr.xingfuxueyuan.xyz

[S42] C++：继承与虚函数
来源：http://gtx.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://gww.hcnkem.com

[S43] C++：智能指针
来源：http://dml.tianlin.xyz

auto p = std::make_unique<int>(5);
来源：http://kpf.cheryme.top

[S44] C++：引用传参
来源：http://gtq.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://yqu.sysykeji.top

[S45] C++：lambda
来源：http://edm.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://ndp.guowangkeji.top

[S46] C++：函数模板
来源：http://aoa.tanke756.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://crf.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://qwf.jinyuanbaomall.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nyy.sweek.top

[S48] C++：逐行读文件
来源：http://bxi.chenlongwang.top

std::ifstream in("a.txt");  std::string line;
来源：http://vfe.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://gri.yj20258.top

[S49] C++：写文件
来源：http://eqx.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eri.aizwys.cn

[S50] C++：格式化数字
来源：http://qet.yongpay.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uhz.nwbrower.top

[S51] C++：显式类型转换
来源：http://idi.yanxiufei.cn

static_cast<double>(a) / b
来源：http://ltb.sxryk.cn

[S52] C++：const 与 noexcept
来源：http://idy.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://wgi.wangdashe.top

[S53] C++：移动语义
来源：http://bmv.ydjk.org.cn

std::vector<int> w = std::move(v);
来源：http://fnz.zdqjudy.top

[S54] C++：异常处理
来源：http://xis.nanxuanxn.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vkc.iojbl.cn

[S55] C++：结构化绑定
来源：http://bti.sufxvd.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://glw.ywan-chungtsiang.top

[S56] C++：optional
来源：http://tel.jinqigfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tta.jqgufenzy.top

[S57] C++：编译期常量
来源：http://zgu.gogol.net.cn

constexpr int N = 10;
来源：http://lkq.andypj.xyz

[S58] C++：命名空间
来源：http://dit.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://sjo.xuetiantiany.cn

[S59] C++：静态断言
来源：http://pgw.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ymb.vehdjk.com

[S60] C++：遍历并删除元素
来源：http://gnd.cdnleiting.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wbl.ivvv.top

================================================================================
来源：http://dok.ydzc1.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lmg.jqgufenzy.top

================================================================================
来源：http://xeg.xuetiantiany.cn

[T01] Kotlin：Hello World
来源：http://jxy.hammf.cn

println("Hello")
来源：http://tsn.zhongyouzk.top

[T02] Kotlin：变量
来源：http://zve.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wun.nanxinkj.top

[T03] Kotlin：字符串模板
来源：http://tsj.tian-w.cn

"值: $b"
来源：http://vem.birdmap.top

[T04] Kotlin：空安全
来源：http://gnb.bjfxy.top

val n: String? = null;  n?.length
来源：http://nst.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://reo.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jkn.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://uha.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wnl.fengsongda.top

[T07] Kotlin：集合过滤
来源：http://gvy.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fol.0kj1m.cn

[T08] Kotlin：数据类
来源：http://lpk.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://fpt.tianlin.xyz

[T09] Kotlin：扩展函数
来源：http://ruv.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://cjd.zycfv.cn

[T10] Kotlin：默认参数
来源：http://jpf.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://rqb.ydjk.org.cn

[T11] Kotlin：协程
来源：http://zdp.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rfd.smart0.xyz

[T12] Kotlin：解构声明
来源：http://kxe.zhiwuduotai.top

val (a, b) = Pair(1, 2)
来源：http://poc.yj202588.top

[T13] Kotlin：只读 Map
来源：http://wqg.nwbrower.top

val m = mapOf("a" to 1)
来源：http://tor.jinyuanbaomall.cn

[T14] Kotlin：循环
来源：http://vdk.snrcjt.cn

for (i in 1..10) println(i)
来源：http://ajl.ivvv.top

[T15] Kotlin：接口
来源：http://fqn.epnwcf.com

interface Shape { fun area(): Double }
来源：http://nzs.hysaishi.cn

[T16] Swift：Hello World
来源：http://aja.dianchejie.cn

print("Hello")
来源：http://uah.yj202588.top

[T17] Swift：变量与常量
来源：http://cog.yuxming.cn

var a = 1;  let b = 2
来源：http://pnq.chenlongwang.top

[T18] Swift：字符串插值
来源：http://zlk.jinghuilouyu.cn

"值: \(b)"
来源：http://yqg.fzhhl.top

[T19] Swift：可选绑定
来源：http://xlw.zhaomingkeji.xyz

if let n = opt { print(n) }
来源：http://lsb.kuanghao11.cn

[T20] Swift：数组操作
来源：http://ljr.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://hfk.gzhubu.top

[T21] Swift：遍历
来源：http://fdq.yuxming.cn

for x in a { print(x) }
来源：http://gid.yj20258.top

[T22] Swift：字典
来源：http://vet.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://oxs.jyoumei.cn

[T23] Swift：函数
来源：http://eoq.daria6918.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qok.sufxvd.cn

[T24] Swift：闭包
来源：http://faw.jianghu66.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lrs.zhiwuduotai.top

[T25] Swift：结构体
来源：http://tfu.cqqwz.cn

struct P { var x: Int }
来源：http://bcf.sysykeji.top

[T26] Swift：类与重写
来源：http://asd.fzhhl.top

class A: Base { override func f() {} }
来源：http://xmz.zhiwuduotai.top

[T27] Swift：错误处理
来源：http://rio.gotoacloud.top

do { try f() } catch { print(error) }
来源：http://cse.birdmap.top

[T28] Swift：枚举
来源：http://bfu.fktsv.cn

enum Color { case red, green }
来源：http://xtr.meibo888.top

[T29] Swift：guard 提前返回
来源：http://eny.jiagoushi.top

guard let x = opt else { return }
来源：http://hqb.hnqzz.top

[T30] Swift：协议
来源：http://tpi.zhoulong.xyz

protocol Shape { func area() -> Double }
来源：http://blh.sweek.top

[T31] Lua：Hello World
来源：http://kag.birdmap.top

print("Hello")
来源：http://ftk.cheryme.top

[T32] Lua：局部变量
来源：http://kjs.haohaochexian.top

local a = 1
来源：http://pge.zhengqikj.top

[T33] Lua：表（数组）
来源：http://lau.zycfv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://guk.yuxming.cn

[T34] Lua：遍历表
来源：http://abr.zycfv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wiq.9152youxi.cn

[T35] Lua：字典表
来源：http://oie.xuanzx.com

local d = { a = 1 };  d.b = 2
来源：http://zbp.yangfankeji.com

[T36] Lua：函数
来源：http://ecl.bbcook.cn

function add(a, b) return a + b end
来源：http://zdj.xylfe.cn

[T37] Lua：字符串拼接
来源：http://sdi.vehdjk.com

"a" .. "b"
来源：http://thl.jqgufenzy.top

[T38] Lua：条件
来源：http://ncc.cheryme.top

if x > 0 then print("正") end
来源：http://aco.nwbrower.top

[T39] Lua：模式匹配
来源：http://khs.xuanzx.com

string.find(s, "%d+")
来源：http://wjy.haohaochexian.top

[T40] Lua：元表
来源：http://tng.aizwys.cn

setmetatable({}, { __index = base })
来源：http://uhb.zdqjudy.top

[T41] Perl：Hello World
来源：http://nrj.yonumen.top

print "Hello\n";
来源：http://ink.cashguo.top

[T42] Perl：变量类型
来源：http://wkw.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cep.guannengcc.top

[T43] Perl：字符串插值
来源：http://fjs.nwbrower.top

"值: $a"
来源：http://res.hesvh.cn

[T44] Perl：条件
来源：http://uma.jinqigfzy.top

if ($a > 0) { print "正"; }
来源：http://seo.cdnleiting.top

[T45] Perl：数组遍历
来源：http://nba.xylfe.cn

for my $x (@arr) { print $x; }
来源：http://aox.zhaomingkeji.xyz

[T46] Perl：哈希操作
来源：http://vvf.ctjpmb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qvd.aibaodan.cn

[T47] Perl：正则捕获
来源：http://ruk.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://trl.zdbjq.cn

[T48] Perl：正则替换
来源：http://sgf.yuxming.cn

$s =~ s/old/new/g;
来源：http://hmf.daria6918.cn

[T49] Perl：函数
来源：http://mzl.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nfl.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://pom.sjlbkw.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dhi.jinqigfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://dgv.hfpthk.cn

[T51] Scala：Hello World
来源：http://lid.ydjk.org.cn

println("Hello")
来源：http://rbn.yj202588.top

[T52] Scala：变量
来源：http://foy.gogol.net.cn

val a = 1;  var b = 2
来源：http://gvt.birdmap.top

[T53] Scala：字符串插值
来源：http://qnq.yanxiufei.cn

s"值: $b"
来源：http://ngr.sweek.top

[T54] Scala：集合映射
来源：http://snq.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://cez.pycfn.com

[T55] Scala：集合过滤
来源：http://kyv.tian-w.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kzy.wangdashe.top

[T56] Scala：样例类
来源：http://jhe.yuanzhike.top

case class User(name: String, age: Int)
来源：http://osm.dashuyun.cn

[T57] Scala：模式匹配
来源：http://oqd.jinyuanbaomall.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lfd.fehbvm.com

[T58] Scala：函数定义
来源：http://jlj.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://ziv.zdbjq.cn

[T59] Scala：循环
来源：http://vps.wangdashe.top

for (i <- 1 to 10) println(i)
来源：http://fzf.tanke756.top

[T60] Scala：折叠
来源：http://svg.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://woq.hysaishi.cn

================================================================================
来源：http://dwd.shanyushiyangtech.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jjg.ppjwa.cn

================================================================================
来源：http://wug.zycfv.cn

[U01] Py：创建虚拟环境
来源：http://rpe.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://okb.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://jgs.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zas.zhixingplan.top

[U03] Py：加载 .env 配置
来源：http://hxl.haohaochexian.top

from dotenv import load_dotenv; load_dotenv()
来源：http://any.jlsjyb.cn

[U04] Py：变量调试打印
来源：http://cqz.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mes.zhixingplan.top

[U05] Py：列表去重且保序
来源：http://dnt.guowangkeji.top

list(dict.fromkeys(arr))
来源：http://jtl.ywan-chungtsiang.top

[U06] Py：合并两个字典
来源：http://nsd.zhixingplan.top

{**a, **b}
来源：http://key.mhx1999.top

[U07] Py：反转字典键值
来源：http://cwc.daxiang520.top

{v: k for k, v in d.items()}
来源：http://hsx.c1oappe.top

[U08] Py：展平二维列表
来源：http://prq.uphjek.com

[y for x in nested for y in x]
来源：http://hqz.bbcook.cn

[U09] Py：字典取最大值的键
来源：http://dss.xinyue.icu

max(d, key=d.get)
来源：http://lbd.ctjpmb.com

[U10] Py：按值排序字典
来源：http://fuo.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gyh.zhoulong.xyz

[U11] Py：生成器表达式
来源：http://ugw.xylfe.cn

(x * 2 for x in arr)
来源：http://pmq.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xjy.sxryk.cn

Counter(arr).most_common(3)
来源：http://tyg.yuanzhike.top

[U13] Py：固定长度队列
来源：http://und.gogol.net.cn

deque(maxlen=10)
来源：http://xgp.dashuyun.cn

[U14] Py：分组收集到列表
来源：http://lwp.guannengcc.top

defaultdict(list)
来源：http://pow.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://zwk.smart0.xyz

t = time.perf_counter()
来源：http://txc.nanxuanxn.top

[U16] Py：命令行参数解析
来源：http://aoe.cucudq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jmz.hnqzz.top

[U17] Py：初始化日志
来源：http://vyi.ywan-chungtsiang.top

logging.basicConfig(level=logging.INFO)
来源：http://nph.chenlongwang.top

[U18] Py：预编译正则
来源：http://kxu.shzxlz.cn

pat = re.compile(r"\d+")
来源：http://sbo.shuidangran.top

[U19] Py：正则替换带回调
来源：http://lml.ydjk.org.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fel.vqdsnc.cn

[U20] Py：缓存函数结果
来源：http://tig.yuxming.cn

@functools.lru_cache(maxsize=None)
来源：http://mii.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://sro.wangshuangyany.cn

@contextlib.contextmanager
来源：http://rgy.sjlbkw.cn

[U22] Py：矩阵转置
来源：http://tnq.wangdashe.top

list(zip(*m))
来源：http://zmc.xuetiantiany.cn

[U23] Py：分块读取大文件
来源：http://anb.quarkkingdee.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wod.hnxiangtu.top

[U24] Py：路径操作
来源：http://nek.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bhl.yueranfly.top

[U25] Py：CSV 按字典读
来源：http://cgq.tarul.cn

csv.DictReader(f)
来源：http://wpx.zhixingplan.top

[U26] Py：并发下载
来源：http://svi.fanxiaobao.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jpn.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://znm.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://gwm.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://zro.quarkkingdee.top

UserId = int
来源：http://vej.nanxinkj.top

[U29] Py：属性校验
来源：http://pmf.aizwys.cn

@property 与 @x.setter 配合
来源：http://rxf.ehwqpu.com

[U30] Py：数据类
来源：http://upv.vqdsnc.cn

@dataclass(slots=True)
来源：http://pqz.hammf.cn

[U31] Py：单测
来源：http://qog.hfpthk.cn

python -m pytest -q
来源：http://zfu.fehbvm.com

[U32] Py：代码格式化
来源：http://wyw.316326.xyz

ruff format . && ruff check --fix .
来源：http://pyr.havefunace.top

[U33] Py：打包发布
来源：http://zyp.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://jsp.fanxiaobao.xyz

[U34] Py：判断编码
来源：http://naq.dianchejie.cn

chardet.detect(raw)
来源：http://qpc.c1oappe.top

[U35] Py：发送邮件
来源：http://hqi.kuanghao11.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rnq.yanxiufei.cn

[U36] Py：定时任务
来源：http://dro.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://ecq.shuidangran.top


<!-- 参考信息 -->