代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fez.fzhhl.top

[S21] C：字符类别判断
来源：http://lxd.cheryme.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nha.gotoacloud.top

[S22] C：字符串转数字
来源：http://tea.chenjidiqi.icu

atoi("42");  strtod("3.14", NULL);
来源：http://awo.jinqigfzy.top

[S23] C：随机数
来源：http://bbc.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ifh.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://xdx.tarul.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vvc.hysaishi.cn

[S25] C：内存拷贝
来源：http://hlm.yj202588.top

memcpy(dst, src, n);
来源：http://dor.gzhubu.top

[S26] C：内存清零
来源：http://dfc.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://cme.jqgfzy.top

[S27] C：定义常量
来源：http://zaj.yueranfly.top

const double PI = 3.14159;
来源：http://gly.xinyue.icu

[S28] C：静态变量
来源：http://dgv.hammf.cn

static int counter = 0;
来源：http://eyk.nanxinkj.top

[S29] C：变参函数
来源：http://okr.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://smz.havefunace.top

[S30] C：头文件保护
来源：http://nsq.ivvv.top

#ifndef X_H
来源：http://mmc.yuanzhike.top

#define X_H
来源：http://plf.hfpthk.cn

#endif
来源：http://heh.zhoulong.xyz

[S31] C++：Hello World
来源：http://nku.snrcjt.cn

#include <iostream>
来源：http://zdp.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://wxg.xinyue.icu

[S32] C++：字符串
来源：http://lhw.xuanzx.com

std::string s = "hi";  s += "!";
来源：http://dyl.fzhhl.top

[S33] C++：vector 增删
来源：http://crz.shzxlz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vez.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://jzy.sweek.top

for (auto &x : v) { std::cout << x; }
来源：http://qft.kuanghao11.cn

[S35] C++：map
来源：http://zhs.tianlin.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hvo.havefunace.top

[S36] C++：unordered_map
来源：http://xub.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vvr.wangdashe.top

[S37] C++：set
来源：http://ncp.hysaishi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://djm.havefunace.top

[S38] C++：排序
来源：http://ayc.yongpay.top

std::sort(v.begin(), v.end());
来源：http://cat.wangshuangyany.cn

[S39] C++：自定义比较器排序
来源：http://ipb.pycfn.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gts.hywenlv.cn

[S40] C++：查找元素
来源：http://llm.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ane.gogol.net.cn

[S41] C++：类与构造函数
来源：http://wgh.cucudq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://llx.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://aob.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://rtc.xuetiantiany.cn

[S43] C++：智能指针
来源：http://cck.fzhhl.top

auto p = std::make_unique<int>(5);
来源：http://fnk.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://czb.uphjek.com

void inc(int &x) { ++x; }
来源：http://uvq.shanyushiyangkeji.top

[S45] C++：lambda
来源：http://cab.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://llz.bbcook.cn

[S46] C++：函数模板
来源：http://quy.vqdsnc.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hfs.hnqzz.top

[S47] C++：结构化绑定遍历
来源：http://iwc.gzhubu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vbl.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://cby.yonumen.top

std::ifstream in("a.txt");  std::string line;
来源：http://byq.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://ghr.hfpthk.cn

[S49] C++：写文件
来源：http://aaw.jlsjyb.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iqx.sufxvd.cn

[S50] C++：格式化数字
来源：http://nlf.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qzk.yuxming.cn

[S51] C++：显式类型转换
来源：http://ghc.jyoumei.cn

static_cast<double>(a) / b
来源：http://yuc.shangyingyoupin.top

[S52] C++：const 与 noexcept
来源：http://asd.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://wki.jiagoushi.top

[S53] C++：移动语义
来源：http://hlu.feifeiyinyue.top

std::vector<int> w = std::move(v);
来源：http://ivn.gogol.net.cn

[S54] C++：异常处理
来源：http://ehe.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pem.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://sbs.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://fcj.cashguo.top

[S56] C++：optional
来源：http://emz.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tdb.ydzc1.top

[S57] C++：编译期常量
来源：http://ahz.guowangkeji.top

constexpr int N = 10;
来源：http://qen.ppjwa.cn

[S58] C++：命名空间
来源：http://lfy.fzhhl.top

namespace ns { int f() { return 1; } }
来源：http://usq.ivvv.top

[S59] C++：静态断言
来源：http://icf.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://asm.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://flf.zhiwuduotai.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dfz.andypj.xyz

================================================================================
来源：http://tuh.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hop.jianghu66.top

================================================================================
来源：http://dom.yfazqb.com

[T01] Kotlin：Hello World
来源：http://fzw.0kj1m.cn

println("Hello")
来源：http://xbt.sweek.top

[T02] Kotlin：变量
来源：http://awl.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gpw.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://bps.yangfankeji.com

"值: $b"
来源：http://muf.wangshuangyany.cn

[T04] Kotlin：空安全
来源：http://gby.hammf.cn

val n: String? = null;  n?.length
来源：http://jzt.guowangkeji.top

[T05] Kotlin：when 表达式
来源：http://dqs.xuetiantiany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fsf.52xcode.cn

[T06] Kotlin：集合映射
来源：http://ien.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uat.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://hws.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xnq.yj202588.top

[T08] Kotlin：数据类
来源：http://fnz.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://khk.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://uzi.hcnkem.com

fun String.exclaim() = this + "!"
来源：http://lda.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://emf.cheryme.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gzo.vehdjk.com

[T11] Kotlin：协程
来源：http://ylp.gaohongyu789.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gcs.fengsongda.top

[T12] Kotlin：解构声明
来源：http://mhm.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://ycd.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://gum.dashuyun.cn

val m = mapOf("a" to 1)
来源：http://bss.ctjpmb.com

[T14] Kotlin：循环
来源：http://pyi.dashuyun.cn

for (i in 1..10) println(i)
来源：http://vjl.jqgfzy.top

[T15] Kotlin：接口
来源：http://dhg.shanyushiyangkeji.top

interface Shape { fun area(): Double }
来源：http://pzw.hongshengwenyu.top

[T16] Swift：Hello World
来源：http://gnc.shuidangran.top

print("Hello")
来源：http://hdp.hongshengwenyu.top

[T17] Swift：变量与常量
来源：http://czh.zhongyouzk.top

var a = 1;  let b = 2
来源：http://vvr.mhx1999.top

[T18] Swift：字符串插值
来源：http://dcb.zdbjq.cn

"值: \(b)"
来源：http://gwr.hfpthk.cn

[T19] Swift：可选绑定
来源：http://edl.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://hlp.nanxuanxn.top

[T20] Swift：数组操作
来源：http://xfg.feifeiyinyue.top

var a = [1, 2, 3];  a.append(4)
来源：http://amv.shuidangran.top

[T21] Swift：遍历
来源：http://hmi.hfpthk.cn

for x in a { print(x) }
来源：http://xmm.ywan-chungtsiang.top

[T22] Swift：字典
来源：http://ukl.hesvh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fzo.xylfe.cn

[T23] Swift：函数
来源：http://iil.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tvx.bjfxy.top

[T24] Swift：闭包
来源：http://pmj.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://onb.cashguo.top

[T25] Swift：结构体
来源：http://wdn.gogol.net.cn

struct P { var x: Int }
来源：http://azz.zhengqikj.top

[T26] Swift：类与重写
来源：http://hus.dianchejie.cn

class A: Base { override func f() {} }
来源：http://lgd.shzxlz.cn

[T27] Swift：错误处理
来源：http://ihk.xinyue.icu

do { try f() } catch { print(error) }
来源：http://alf.meibo888.top

[T28] Swift：枚举
来源：http://wcq.chenlongwang.top

enum Color { case red, green }
来源：http://qll.hammf.cn

[T29] Swift：guard 提前返回
来源：http://qcd.xuanzx.com

guard let x = opt else { return }
来源：http://tne.vqdsnc.cn

[T30] Swift：协议
来源：http://okg.ydjk.org.cn

protocol Shape { func area() -> Double }
来源：http://psg.jianghu66.top

[T31] Lua：Hello World
来源：http://syf.meibo888.top

print("Hello")
来源：http://dni.tanke756.top

[T32] Lua：局部变量
来源：http://rqj.shzxlz.cn

local a = 1
来源：http://vgw.yuxming.cn

[T33] Lua：表（数组）
来源：http://xou.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ehw.hongshengwenyu.top

[T34] Lua：遍历表
来源：http://sir.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tah.yfazqb.com

[T35] Lua：字典表
来源：http://bwf.shanyushiyangtech.top

local d = { a = 1 };  d.b = 2
来源：http://lhq.xingfuxueyuan.xyz

[T36] Lua：函数
来源：http://kll.bjfxy.top

function add(a, b) return a + b end
来源：http://hra.hysaishi.cn

[T37] Lua：字符串拼接
来源：http://sgj.jinqigufen.top

"a" .. "b"
来源：http://hjz.xuanzx.com

[T38] Lua：条件
来源：http://tfg.jiagoushi.top

if x > 0 then print("正") end
来源：http://yxx.hcnkem.com

[T39] Lua：模式匹配
来源：http://xpa.fktsv.cn

string.find(s, "%d+")
来源：http://igt.xylfe.cn

[T40] Lua：元表
来源：http://hcy.xuetiantiany.cn

setmetatable({}, { __index = base })
来源：http://zzz.quarkkingdee.top

[T41] Perl：Hello World
来源：http://icb.ywan-chungtsiang.top

print "Hello\n";
来源：http://uvz.nwbrower.top

[T42] Perl：变量类型
来源：http://ukk.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nqd.yvedp.cn

[T43] Perl：字符串插值
来源：http://ycf.hongshengwenyu.top

"值: $a"
来源：http://hiq.nanxinkj.top

[T44] Perl：条件
来源：http://yqc.gogol.net.cn

if ($a > 0) { print "正"; }
来源：http://xab.kuanghao11.cn

[T45] Perl：数组遍历
来源：http://ebe.zhiwuduotai.top

for my $x (@arr) { print $x; }
来源：http://qrv.andypj.xyz

[T46] Perl：哈希操作
来源：http://dyb.smart0.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wjf.gotoacloud.top

[T47] Perl：正则捕获
来源：http://gfy.wangshuangyany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bhp.ivvv.top

[T48] Perl：正则替换
来源：http://sxh.cheryme.top

$s =~ s/old/new/g;
来源：http://pmh.quarkkingdee.top

[T49] Perl：函数
来源：http://fps.yj20258.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vae.gaohongyu789.top

[T50] Perl：逐行读文件
来源：http://bvk.vqdsnc.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lpf.ehwqpu.com

while (my $line = <$fh>) { print $line; }
来源：http://beq.aizwys.cn

[T51] Scala：Hello World
来源：http://jez.hysaishi.cn

println("Hello")
来源：http://jma.guannengcc.top

[T52] Scala：变量
来源：http://muk.tian-w.cn

val a = 1;  var b = 2
来源：http://vpv.ydjk.org.cn

[T53] Scala：字符串插值
来源：http://awy.iojbl.cn

s"值: $b"
来源：http://pxe.vehdjk.com

[T54] Scala：集合映射
来源：http://ted.gaohongyu789.top

List(1, 2, 3).map(_ * 2)
来源：http://xwx.pycfn.com

[T55] Scala：集合过滤
来源：http://drg.meibo888.top

List(1, 2, 3).filter(_ > 1)
来源：http://ymi.jinqigufen.top

[T56] Scala：样例类
来源：http://ncx.yj202588.top

case class User(name: String, age: Int)
来源：http://lyb.chenjidiqi.icu

[T57] Scala：模式匹配
来源：http://qia.pycfn.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://gfp.gzhubu.top

[T58] Scala：函数定义
来源：http://ehi.hongshengwenyu.top

def add(a: Int, b: Int): Int = a + b
来源：http://ied.ivvv.top

[T59] Scala：循环
来源：http://smy.gogol.net.cn

for (i <- 1 to 10) println(i)
来源：http://lrr.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://tdz.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ciz.wangshuangyany.cn

================================================================================
来源：http://jtj.snrcjt.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sml.birdmap.top

================================================================================
来源：http://rot.zhengqikj.top

[U01] Py：创建虚拟环境
来源：http://itl.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://qde.xuanzx.com

[U02] Py：导出 / 安装依赖
来源：http://ceh.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vuc.9152youxi.cn

[U03] Py：加载 .env 配置
来源：http://ylc.hcnkem.com

from dotenv import load_dotenv; load_dotenv()
来源：http://swu.havefunace.top

[U04] Py：变量调试打印
来源：http://hqk.yongpay.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sys.smart0.xyz

[U05] Py：列表去重且保序
来源：http://kow.yvedp.cn

list(dict.fromkeys(arr))
来源：http://jlu.tarul.cn

[U06] Py：合并两个字典
来源：http://dre.zdbjq.cn

{**a, **b}
来源：http://frt.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://kel.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://ddw.0kj1m.cn

[U08] Py：展平二维列表
来源：http://avu.fanxiaobao.xyz

[y for x in nested for y in x]
来源：http://nvo.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://bqx.meibo888.top

max(d, key=d.get)
来源：http://ooj.jianghu66.top

[U10] Py：按值排序字典
来源：http://szz.xziqi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://osx.chenzaomai.com

[U11] Py：生成器表达式
来源：http://zda.nwbrower.top

(x * 2 for x in arr)
来源：http://mba.shangyingyoupin.top

[U12] Py：取出现最多的 3 个元素
来源：http://vvl.hesvh.cn

Counter(arr).most_common(3)
来源：http://slh.xuanzx.com

[U13] Py：固定长度队列
来源：http://rsh.jinghuilouyu.cn

deque(maxlen=10)
来源：http://fyd.cucudq.cn

[U14] Py：分组收集到列表
来源：http://yqh.gzhubu.top

defaultdict(list)
来源：http://okk.aizwys.cn

[U15] Py：高精度计时
来源：http://ued.quarkkingdee.top

t = time.perf_counter()
来源：http://jjh.zycfv.cn

[U16] Py：命令行参数解析
来源：http://zrb.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://veu.0kj1m.cn

[U17] Py：初始化日志
来源：http://ubg.wangshuangyany.cn

logging.basicConfig(level=logging.INFO)
来源：http://hnm.gotoacloud.top

[U18] Py：预编译正则
来源：http://lpe.hcnkem.com

pat = re.compile(r"\d+")
来源：http://xur.xuetiantiany.cn

[U19] Py：正则替换带回调
来源：http://hfo.cheryme.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nml.guannengcc.top

[U20] Py：缓存函数结果
来源：http://lsv.cucudq.cn

@functools.lru_cache(maxsize=None)
来源：http://hvy.c1oappe.top

[U21] Py：自定义上下文管理器
来源：http://nld.ivvv.top

@contextlib.contextmanager
来源：http://utv.xingfuxueyuan.xyz

[U22] Py：矩阵转置
来源：http://ptq.kuanghao11.cn

list(zip(*m))
来源：http://bmz.redwolf501.top

[U23] Py：分块读取大文件
来源：http://nys.hysaishi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vyq.redwolf501.top

[U24] Py：路径操作
来源：http://egq.chenlongwang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uai.yj20258.top

[U25] Py：CSV 按字典读
来源：http://mku.uphjek.com

csv.DictReader(f)
来源：http://gfr.yj20258.top

[U26] Py：并发下载
来源：http://vdj.fehbvm.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zsx.guannengcc.top

[U27] Py：异步 HTTP
来源：http://bkr.xingfuxueyuan.xyz

aiohttp.ClientSession() 配合 async with
来源：http://hql.jqgufenzy.top

[U28] Py：类型别名
来源：http://kkr.chenjidiqi.icu

UserId = int
来源：http://fiy.mhx1999.top

[U29] Py：属性校验
来源：http://keh.zhiwuduotai.top

@property 与 @x.setter 配合
来源：http://rtb.xingfuxueyuan.xyz

[U30] Py：数据类
来源：http://bjt.xziqi.cn

@dataclass(slots=True)
来源：http://rvs.zhongyouzk.top

[U31] Py：单测
来源：http://vnz.vehdjk.com

python -m pytest -q
来源：http://voc.hongshengwenyu.top

[U32] Py：代码格式化
来源：http://vld.yuanzhike.top

ruff format . && ruff check --fix .
来源：http://ruw.hfpthk.cn

[U33] Py：打包发布
来源：http://bcr.kuanghao11.cn

python -m build  （依赖 pyproject.toml）
来源：http://rrb.wangdashe.top

[U34] Py：判断编码
来源：http://eqy.ybcxt.top

chardet.detect(raw)
来源：http://men.gzhubu.top

[U35] Py：发送邮件
来源：http://fsf.yj20258.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://enn.birdmap.top

[U36] Py：定时任务
来源：http://btu.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://mhg.jinqigufen.top

[U37] Py：读写 Excel
来源：http://msd.feifeiyinyue.top

pandas.read_excel / DataFrame.to_excel
来源：http://ytu.gotoacloud.top

[U38] Py：获取脚本所在目录
来源：http://jyo.hywenlv.cn

Path(__file__).resolve().parent
来源：http://ggv.zdbjq.cn

[U39] Py：判断是否在交互环境
来源：http://lll.shangyingyoupin.top

sys.stdout.isatty()
来源：http://ars.meibo888.top

[U40] Py：打印到标准错误
来源：http://hou.cdnleiting.top

print("err", file=sys.stderr)
来源：http://kxg.gaohongyu789.top

[U41] PHP：初始化 Composer 项目
来源：http://szc.c1oappe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lii.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://vob.jianghu66.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rga.mhx1999.top

[U43] PHP：声明命名空间
来源：http://dec.c1oappe.top

namespace App\Http;
来源：http://qzz.zhaomingkeji.xyz

[U44] PHP：开启严格类型
来源：http://tdy.zhongyouzk.top

declare(strict_types=1);
来源：http://rrg.yj20258.top


<!-- 参考信息 -->