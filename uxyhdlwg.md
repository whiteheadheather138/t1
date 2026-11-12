代发 wailian999

int main(int argc, char **argv)
来源：http://iib.hammf.cn

[S19] C：快速排序
来源：http://wob.pengpengdd.cyou

qsort(a, n, sizeof(int), cmp);
来源：http://ypn.nanxinkj.top

[S20] C：二分查找
来源：http://jwy.kuanghao11.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qfq.zhixingplan.top

[S21] C：字符类别判断
来源：http://ppi.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zmz.ppjwa.cn

[S22] C：字符串转数字
来源：http://dms.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://gvs.feifeiyinyue.top

[S23] C：随机数
来源：http://llv.zhoulong.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://mxl.uphjek.com

[S24] C：获取本地时间
来源：http://eku.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aaw.yuxming.cn

[S25] C：内存拷贝
来源：http://hjb.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://jpu.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://fig.sxryk.cn

memset(a, 0, sizeof a);
来源：http://uln.yanxiufei.cn

[S27] C：定义常量
来源：http://shk.daxiang520.top

const double PI = 3.14159;
来源：http://owc.sjlbkw.cn

[S28] C：静态变量
来源：http://jbk.hcnkem.com

static int counter = 0;
来源：http://tan.tian-w.cn

[S29] C：变参函数
来源：http://wpu.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cnc.gogol.net.cn

[S30] C：头文件保护
来源：http://cez.ywan-chungtsiang.top

#ifndef X_H
来源：http://qxb.sxryk.cn

#define X_H
来源：http://soa.xingfuxueyuan.xyz

#endif
来源：http://emm.jinqigfzy.top

[S31] C++：Hello World
来源：http://eyw.chenlongwang.top

#include <iostream>
来源：http://alf.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://pnk.tarul.cn

[S32] C++：字符串
来源：http://iad.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://ebc.cashguo.top

[S33] C++：vector 增删
来源：http://vnu.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fve.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://tkz.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://hsy.chenlongwang.top

[S35] C++：map
来源：http://inn.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gqa.yueranfly.top

[S36] C++：unordered_map
来源：http://ckl.ppjwa.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://udb.iojbl.cn

[S37] C++：set
来源：http://pto.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cpu.hnqzz.top

[S38] C++：排序
来源：http://zhe.feifeiyinyue.top

std::sort(v.begin(), v.end());
来源：http://uxz.xylfe.cn

[S39] C++：自定义比较器排序
来源：http://ntf.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rhd.hywenlv.cn

[S40] C++：查找元素
来源：http://ter.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://idg.yj20258.top

[S41] C++：类与构造函数
来源：http://jmd.jinqigufen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ryb.hesvh.cn

[S42] C++：继承与虚函数
来源：http://uex.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://vvy.guannengcc.top

[S43] C++：智能指针
来源：http://ija.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://bfp.xylfe.cn

[S44] C++：引用传参
来源：http://iph.zhongyouzk.top

void inc(int &x) { ++x; }
来源：http://xzj.ydzc1.top

[S45] C++：lambda
来源：http://voq.fanxiaobao.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://ero.epnwcf.com

[S46] C++：函数模板
来源：http://tkh.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fef.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://cjk.dianchejie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ryr.hnqzz.top

[S48] C++：逐行读文件
来源：http://lsh.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jyt.316326.xyz

while (std::getline(in, line)) { }
来源：http://mcm.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://fhs.hnxiangtu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://quo.mhx1999.top

[S50] C++：格式化数字
来源：http://ylq.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bkw.hysaishi.cn

[S51] C++：显式类型转换
来源：http://xru.sweek.top

static_cast<double>(a) / b
来源：http://kau.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://bby.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://txu.sweek.top

[S53] C++：移动语义
来源：http://hzg.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://oif.zhongyouzk.top

[S54] C++：异常处理
来源：http://wbo.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gmj.birdmap.top

[S55] C++：结构化绑定
来源：http://bzc.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bgk.jlsjyb.cn

[S56] C++：optional
来源：http://nae.nwbrower.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uox.yangfankeji.com

[S57] C++：编译期常量
来源：http://zhc.zhiwuduotai.top

constexpr int N = 10;
来源：http://bzx.fehbvm.com

[S58] C++：命名空间
来源：http://yjy.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://kcp.hammf.cn

[S59] C++：静态断言
来源：http://pjv.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cdd.gaohongyu789.top

[S60] C++：遍历并删除元素
来源：http://pkd.zhiwuduotai.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zne.shangyingyoupin.top

================================================================================
来源：http://yql.yvedp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yry.yvedp.cn

================================================================================
来源：http://cel.hesvh.cn

[T01] Kotlin：Hello World
来源：http://poy.andypj.xyz

println("Hello")
来源：http://ovl.c1oappe.top

[T02] Kotlin：变量
来源：http://zle.xuetiantiany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ttq.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://enu.yongpay.top

"值: $b"
来源：http://hat.yfazqb.com

[T04] Kotlin：空安全
来源：http://phc.havefunace.top

val n: String? = null;  n?.length
来源：http://qri.svipenyu.cn

[T05] Kotlin：when 表达式
来源：http://ehp.pengpengdd.cyou

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zfh.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://xfm.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zan.andypj.xyz

[T07] Kotlin：集合过滤
来源：http://aaq.zhijiandao.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jsi.tarul.cn

[T08] Kotlin：数据类
来源：http://rrd.xziqi.cn

data class User(val name: String, val age: Int)
来源：http://qvy.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://yjb.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://fra.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://btj.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nje.ybcxt.top

[T11] Kotlin：协程
来源：http://ltg.xingfuxueyuan.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://rji.yj20258.top

[T12] Kotlin：解构声明
来源：http://etp.c1oappe.top

val (a, b) = Pair(1, 2)
来源：http://ejd.hysaishi.cn

[T13] Kotlin：只读 Map
来源：http://vbh.gaohongyu789.top

val m = mapOf("a" to 1)
来源：http://aqk.tian-w.cn

[T14] Kotlin：循环
来源：http://enx.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://ght.zhiwuduotai.top

[T15] Kotlin：接口
来源：http://oag.iojbl.cn

interface Shape { fun area(): Double }
来源：http://aoe.chenjidiqi.icu

[T16] Swift：Hello World
来源：http://bgs.yuxming.cn

print("Hello")
来源：http://oom.smart0.xyz

[T17] Swift：变量与常量
来源：http://eni.sufxvd.cn

var a = 1;  let b = 2
来源：http://mor.havefunace.top

[T18] Swift：字符串插值
来源：http://oyk.ehwqpu.com

"值: \(b)"
来源：http://htt.jqgfzy.top

[T19] Swift：可选绑定
来源：http://nic.xziqi.cn

if let n = opt { print(n) }
来源：http://pdj.yanxiufei.cn

[T20] Swift：数组操作
来源：http://idc.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://dzo.xuetiantiany.cn

[T21] Swift：遍历
来源：http://gih.cdnleiting.top

for x in a { print(x) }
来源：http://acm.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://dxp.guannengcc.top

var d = ["a": 1];  d["b"] = 2
来源：http://ycx.yangfankeji.com

[T23] Swift：函数
来源：http://zcl.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qsm.jinghuilouyu.cn

[T24] Swift：闭包
来源：http://oxi.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://ofx.aizwys.cn

[T25] Swift：结构体
来源：http://aje.316326.xyz

struct P { var x: Int }
来源：http://tjf.cashguo.top

[T26] Swift：类与重写
来源：http://wpg.cdnleiting.top

class A: Base { override func f() {} }
来源：http://zgt.xziqi.cn

[T27] Swift：错误处理
来源：http://ppx.jianghu66.top

do { try f() } catch { print(error) }
来源：http://act.sjlbkw.cn

[T28] Swift：枚举
来源：http://xpk.xingfuxueyuan.xyz

enum Color { case red, green }
来源：http://ouc.fehbvm.com

[T29] Swift：guard 提前返回
来源：http://fir.jqgfzy.top

guard let x = opt else { return }
来源：http://yhu.jiagoushi.top

[T30] Swift：协议
来源：http://zbu.cashguo.top

protocol Shape { func area() -> Double }
来源：http://ojy.xylfe.cn

[T31] Lua：Hello World
来源：http://qlx.jinqigufen.top

print("Hello")
来源：http://vcv.ctjpmb.com

[T32] Lua：局部变量
来源：http://rsi.cucudq.cn

local a = 1
来源：http://ire.zhiwuduotai.top

[T33] Lua：表（数组）
来源：http://fyg.bjfxy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fzi.xylfe.cn

[T34] Lua：遍历表
来源：http://qhy.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fpn.birdmap.top

[T35] Lua：字典表
来源：http://pif.dianchejie.cn

local d = { a = 1 };  d.b = 2
来源：http://foh.dashuyun.cn

[T36] Lua：函数
来源：http://hxn.feifeiyinyue.top

function add(a, b) return a + b end
来源：http://mqv.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://zwq.cqqwz.cn

"a" .. "b"
来源：http://gvf.xinyue.icu

[T38] Lua：条件
来源：http://xmy.birdmap.top

if x > 0 then print("正") end
来源：http://nbn.ydjk.org.cn

[T39] Lua：模式匹配
来源：http://hwt.sufxvd.cn

string.find(s, "%d+")
来源：http://fau.tarul.cn

[T40] Lua：元表
来源：http://mcq.tian-w.cn

setmetatable({}, { __index = base })
来源：http://wyc.vehdjk.com

[T41] Perl：Hello World
来源：http://uhx.jinyuanbaomall.cn

print "Hello\n";
来源：http://ayg.epnwcf.com

[T42] Perl：变量类型
来源：http://nlo.gzhubu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qdj.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://czs.ctjpmb.com

"值: $a"
来源：http://iit.pycfn.com

[T44] Perl：条件
来源：http://rfx.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://gnv.ydzc1.top

[T45] Perl：数组遍历
来源：http://ocf.tian-w.cn

for my $x (@arr) { print $x; }
来源：http://gim.zhijiandao.cn

[T46] Perl：哈希操作
来源：http://rts.daria6918.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://buj.jiagoushi.top

[T47] Perl：正则捕获
来源：http://nsj.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pbr.hesvh.cn

[T48] Perl：正则替换
来源：http://rro.shuidangran.top

$s =~ s/old/new/g;
来源：http://kpe.mhx1999.top

[T49] Perl：函数
来源：http://vya.zhixingplan.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yfd.hcnkem.com

[T50] Perl：逐行读文件
来源：http://iyp.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ysn.ehwqpu.com

while (my $line = <$fh>) { print $line; }
来源：http://yea.cheryme.top

[T51] Scala：Hello World
来源：http://itu.cucudq.cn

println("Hello")
来源：http://xda.zhongyouzk.top

[T52] Scala：变量
来源：http://gin.yonumen.top

val a = 1;  var b = 2
来源：http://kvk.sysykeji.top

[T53] Scala：字符串插值
来源：http://glm.zhixingplan.top

s"值: $b"
来源：http://fqb.316326.xyz

[T54] Scala：集合映射
来源：http://liq.sxryk.cn

List(1, 2, 3).map(_ * 2)
来源：http://ywy.shanyushiyangkeji.top

[T55] Scala：集合过滤
来源：http://gtg.hfpthk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ogs.xuetiantiany.cn

[T56] Scala：样例类
来源：http://byb.tarul.cn

case class User(name: String, age: Int)
来源：http://lkv.vehdjk.com

[T57] Scala：模式匹配
来源：http://ebf.jinghuilouyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pcy.cdnleiting.top

[T58] Scala：函数定义
来源：http://cza.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://upd.hammf.cn

[T59] Scala：循环
来源：http://ueq.chenjidiqi.icu

for (i <- 1 to 10) println(i)
来源：http://tke.sxryk.cn

[T60] Scala：折叠
来源：http://axd.daria6918.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jje.tian-w.cn

================================================================================
来源：http://fug.ydzc1.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://btl.bjfxy.top

================================================================================
来源：http://bgo.zhongyouzk.top

[U01] Py：创建虚拟环境
来源：http://mtm.zdbjq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yzr.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://zwp.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jlu.shanyushiyangkeji.top

[U03] Py：加载 .env 配置
来源：http://cjt.gzhubu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sbo.sxryk.cn

[U04] Py：变量调试打印
来源：http://ocq.hnxiangtu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mnv.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://fat.gzhubu.top

list(dict.fromkeys(arr))
来源：http://vgl.epnwcf.com

[U06] Py：合并两个字典
来源：http://war.nanxinkj.top

{**a, **b}
来源：http://bkv.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://tkh.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://uey.sweek.top

[U08] Py：展平二维列表
来源：http://czf.shanyushiyangkeji.top

[y for x in nested for y in x]
来源：http://sgr.gzhubu.top

[U09] Py：字典取最大值的键
来源：http://dou.xuanzx.com

max(d, key=d.get)
来源：http://ngn.cdnleiting.top

[U10] Py：按值排序字典
来源：http://uzd.yj202588.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gpt.cdnleiting.top

[U11] Py：生成器表达式
来源：http://pch.cucudq.cn

(x * 2 for x in arr)
来源：http://kiu.fktsv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dyr.daria6918.cn

Counter(arr).most_common(3)
来源：http://lrk.smart0.xyz

[U13] Py：固定长度队列
来源：http://khc.xuanzx.com

deque(maxlen=10)
来源：http://djp.9152youxi.cn

[U14] Py：分组收集到列表
来源：http://dzq.cheryme.top

defaultdict(list)
来源：http://sya.yangfankeji.com

[U15] Py：高精度计时
来源：http://glp.tanke756.top

t = time.perf_counter()
来源：http://szo.0kj1m.cn

[U16] Py：命令行参数解析
来源：http://pes.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qsg.yueranfly.top

[U17] Py：初始化日志
来源：http://onw.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://izi.316326.xyz

[U18] Py：预编译正则
来源：http://osf.9152youxi.cn

pat = re.compile(r"\d+")
来源：http://mnk.cheryme.top

[U19] Py：正则替换带回调
来源：http://edo.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ekv.dashuyun.cn

[U20] Py：缓存函数结果
来源：http://usm.zhaomingkeji.xyz

@functools.lru_cache(maxsize=None)
来源：http://hll.pycfn.com

[U21] Py：自定义上下文管理器
来源：http://jef.tian-w.cn

@contextlib.contextmanager
来源：http://fpc.birdmap.top

[U22] Py：矩阵转置
来源：http://ufi.ehwqpu.com

list(zip(*m))
来源：http://upb.ywan-chungtsiang.top

[U23] Py：分块读取大文件
来源：http://mja.yj20258888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zfr.sjlbkw.cn

[U24] Py：路径操作
来源：http://zsp.zycfv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ahc.zhongyouzk.top

[U25] Py：CSV 按字典读
来源：http://imk.chenlongwang.top

csv.DictReader(f)
来源：http://rjr.uphjek.com

[U26] Py：并发下载
来源：http://pwv.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yxi.sxryk.cn

[U27] Py：异步 HTTP
来源：http://yvn.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://cpv.gogol.net.cn

[U28] Py：类型别名
来源：http://sfi.jyoumei.cn

UserId = int
来源：http://txy.kuanghao11.cn

[U29] Py：属性校验
来源：http://uel.smart0.xyz

@property 与 @x.setter 配合
来源：http://tvp.aizwys.cn

[U30] Py：数据类
来源：http://shs.xinyue.icu

@dataclass(slots=True)
来源：http://qpt.jinqigufen.top

[U31] Py：单测
来源：http://htn.yanxiufei.cn

python -m pytest -q
来源：http://cui.9152youxi.cn

[U32] Py：代码格式化
来源：http://yqn.ybcxt.top

ruff format . && ruff check --fix .
来源：http://qev.vqdsnc.cn

[U33] Py：打包发布
来源：http://ugm.wangdashe.top

python -m build  （依赖 pyproject.toml）
来源：http://sle.bjfxy.top

[U34] Py：判断编码
来源：http://yuc.iojbl.cn

chardet.detect(raw)
来源：http://xhg.cqqwz.cn

[U35] Py：发送邮件
来源：http://woj.andypj.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ows.dianchejie.cn

[U36] Py：定时任务
来源：http://coi.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://lap.yangfankeji.com

[U37] Py：读写 Excel
来源：http://bks.xuanzx.com

pandas.read_excel / DataFrame.to_excel
来源：http://vxq.gaohongyu789.top

[U38] Py：获取脚本所在目录
来源：http://jrh.sweek.top

Path(__file__).resolve().parent
来源：http://akj.cqqwz.cn

[U39] Py：判断是否在交互环境
来源：http://hag.iojbl.cn

sys.stdout.isatty()
来源：http://dya.bbcook.cn

[U40] Py：打印到标准错误
来源：http://ngv.daria6918.cn

print("err", file=sys.stderr)
来源：http://dmh.andypj.xyz

[U41] PHP：初始化 Composer 项目
来源：http://zan.yongpay.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zpm.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://vfk.hnxiangtu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eyi.yvedp.cn


<!-- 参考信息 -->