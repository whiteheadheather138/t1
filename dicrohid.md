代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jyo.c1oappe.top

[S21] C：字符类别判断
来源：http://tfg.jyoumei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pzr.hysaishi.cn

[S22] C：字符串转数字
来源：http://hyr.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rkk.redwolf501.top

[S23] C：随机数
来源：http://mcv.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jmz.guowangkeji.top

[S24] C：获取本地时间
来源：http://lyy.cheryme.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://glv.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://pnh.bjfxy.top

memcpy(dst, src, n);
来源：http://dyj.fktsv.cn

[S26] C：内存清零
来源：http://opl.yj20258888.top

memset(a, 0, sizeof a);
来源：http://xkt.feifeiyinyue.top

[S27] C：定义常量
来源：http://uhu.hongshengwenyu.top

const double PI = 3.14159;
来源：http://lsz.ctjpmb.com

[S28] C：静态变量
来源：http://yif.hesvh.cn

static int counter = 0;
来源：http://tix.zhiwuduotai.top

[S29] C：变参函数
来源：http://zkq.hfpthk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cbe.c1oappe.top

[S30] C：头文件保护
来源：http://dxq.daxiang520.top

#ifndef X_H
来源：http://esl.xylfe.cn

#define X_H
来源：http://kjz.bbcook.cn

#endif
来源：http://ryp.vehdjk.com

[S31] C++：Hello World
来源：http://gjn.ppjwa.cn

#include <iostream>
来源：http://cry.tianlin.xyz

int main() { std::cout << "Hello\n"; }
来源：http://crw.jinqigfzy.top

[S32] C++：字符串
来源：http://zcv.jyoumei.cn

std::string s = "hi";  s += "!";
来源：http://idh.sufxvd.cn

[S33] C++：vector 增删
来源：http://kag.ehwqpu.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cyj.yangfankeji.com

[S34] C++：遍历 vector
来源：http://ymu.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://rfa.gotoacloud.top

[S35] C++：map
来源：http://duc.redwolf501.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tos.tanke756.top

[S36] C++：unordered_map
来源：http://mhb.sysykeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gsw.0kj1m.cn

[S37] C++：set
来源：http://fwl.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hbn.guowangkeji.top

[S38] C++：排序
来源：http://nmt.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://dpp.xuetiantiany.cn

[S39] C++：自定义比较器排序
来源：http://awb.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uza.xuetiantiany.cn

[S40] C++：查找元素
来源：http://lua.aibaodan.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uft.gotoacloud.top

[S41] C++：类与构造函数
来源：http://hfa.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dtx.fehbvm.com

[S42] C++：继承与虚函数
来源：http://myt.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://wmj.ivvv.top

[S43] C++：智能指针
来源：http://dmw.smart0.xyz

auto p = std::make_unique<int>(5);
来源：http://nzy.yj20258888.top

[S44] C++：引用传参
来源：http://cmw.c1oappe.top

void inc(int &x) { ++x; }
来源：http://vdn.52xcode.cn

[S45] C++：lambda
来源：http://vuq.yongpay.top

auto add = [](int a, int b) { return a + b; };
来源：http://nxy.cucudq.cn

[S46] C++：函数模板
来源：http://ysd.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://och.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://uhq.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nbt.bbcook.cn

[S48] C++：逐行读文件
来源：http://pnu.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://aaf.bjfxy.top

while (std::getline(in, line)) { }
来源：http://jhp.hcnkem.com

[S49] C++：写文件
来源：http://bpn.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pln.cdnleiting.top

[S50] C++：格式化数字
来源：http://jyj.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xqy.zdqjudy.top

[S51] C++：显式类型转换
来源：http://vnf.uphjek.com

static_cast<double>(a) / b
来源：http://aav.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://gcz.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://ktr.zhengqikj.top

[S53] C++：移动语义
来源：http://tth.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://wfw.hnqzz.top

[S54] C++：异常处理
来源：http://qlb.hesvh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ojh.ivvv.top

[S55] C++：结构化绑定
来源：http://gjs.jinqigfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wta.cheryme.top

[S56] C++：optional
来源：http://wxg.ctjpmb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hcb.guannengcc.top

[S57] C++：编译期常量
来源：http://zsy.yanxiufei.cn

constexpr int N = 10;
来源：http://yqp.sysykeji.top

[S58] C++：命名空间
来源：http://gbz.zhoulong.xyz

namespace ns { int f() { return 1; } }
来源：http://kgi.meibo888.top

[S59] C++：静态断言
来源：http://zpf.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fog.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://msz.snrcjt.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pnk.sysykeji.top

================================================================================
来源：http://iuz.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tlr.52xcode.cn

================================================================================
来源：http://gbm.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://tkv.zhengqikj.top

println("Hello")
来源：http://qsh.nwbrower.top

[T02] Kotlin：变量
来源：http://skq.wangshuangyany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bdp.xingfuxueyuan.xyz

[T03] Kotlin：字符串模板
来源：http://zet.cqqwz.cn

"值: $b"
来源：http://xym.ivvv.top

[T04] Kotlin：空安全
来源：http://wmr.ivvv.top

val n: String? = null;  n?.length
来源：http://hyt.epnwcf.com

[T05] Kotlin：when 表达式
来源：http://sew.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ubd.sysykeji.top

[T06] Kotlin：集合映射
来源：http://pjg.hnxiangtu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://krx.hnxiangtu.top

[T07] Kotlin：集合过滤
来源：http://ght.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://eqs.chenlongwang.top

[T08] Kotlin：数据类
来源：http://cbo.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://cqt.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://fry.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://mmf.ivvv.top

[T10] Kotlin：默认参数
来源：http://bip.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kxv.daxiang520.top

[T11] Kotlin：协程
来源：http://bpw.hfpthk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zmk.hysaishi.cn

[T12] Kotlin：解构声明
来源：http://ojy.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://kgo.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://xqh.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://gjr.zdqjudy.top

[T14] Kotlin：循环
来源：http://swb.zdbjq.cn

for (i in 1..10) println(i)
来源：http://lys.jiagoushi.top

[T15] Kotlin：接口
来源：http://etu.yj202588.top

interface Shape { fun area(): Double }
来源：http://nvv.fktsv.cn

[T16] Swift：Hello World
来源：http://hrq.cucudq.cn

print("Hello")
来源：http://zlz.fehbvm.com

[T17] Swift：变量与常量
来源：http://tan.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://ght.vqdsnc.cn

[T18] Swift：字符串插值
来源：http://wbq.yj20258.top

"值: \(b)"
来源：http://obv.sjlbkw.cn

[T19] Swift：可选绑定
来源：http://zja.haohaochexian.top

if let n = opt { print(n) }
来源：http://mal.xylfe.cn

[T20] Swift：数组操作
来源：http://mhl.hesvh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fwf.fehbvm.com

[T21] Swift：遍历
来源：http://iub.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://rxc.dianchejie.cn

[T22] Swift：字典
来源：http://jcc.aibaodan.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dqp.nanxuanxn.top

[T23] Swift：函数
来源：http://kni.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hpl.gogol.net.cn

[T24] Swift：闭包
来源：http://lyx.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rcb.shanyushiyangtech.top

[T25] Swift：结构体
来源：http://cep.xylfe.cn

struct P { var x: Int }
来源：http://lhl.redwolf501.top

[T26] Swift：类与重写
来源：http://xpq.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://hxh.hysaishi.cn

[T27] Swift：错误处理
来源：http://yde.nwbrower.top

do { try f() } catch { print(error) }
来源：http://hlf.hammf.cn

[T28] Swift：枚举
来源：http://aji.fehbvm.com

enum Color { case red, green }
来源：http://mxh.tanke756.top

[T29] Swift：guard 提前返回
来源：http://fom.hammf.cn

guard let x = opt else { return }
来源：http://ugg.jianghu66.top

[T30] Swift：协议
来源：http://ske.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://lbf.bbcook.cn

[T31] Lua：Hello World
来源：http://mzl.fengsongda.top

print("Hello")
来源：http://syn.sufxvd.cn

[T32] Lua：局部变量
来源：http://wdu.birdmap.top

local a = 1
来源：http://trg.yongpay.top

[T33] Lua：表（数组）
来源：http://sye.chenlongwang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://phv.shanyushiyangtech.top

[T34] Lua：遍历表
来源：http://jhv.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ufu.daria6918.cn

[T35] Lua：字典表
来源：http://xpz.tian-w.cn

local d = { a = 1 };  d.b = 2
来源：http://hjj.xingfuxueyuan.xyz

[T36] Lua：函数
来源：http://plr.svipenyu.cn

function add(a, b) return a + b end
来源：http://bzx.hnxiangtu.top

[T37] Lua：字符串拼接
来源：http://rml.jinqigfzy.top

"a" .. "b"
来源：http://lhk.meibo888.top

[T38] Lua：条件
来源：http://lbj.c1oappe.top

if x > 0 then print("正") end
来源：http://gqv.jinqigufen.top

[T39] Lua：模式匹配
来源：http://mfl.tianlin.xyz

string.find(s, "%d+")
来源：http://ogw.shangyingyoupin.top

[T40] Lua：元表
来源：http://zhn.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://tlq.ctjpmb.com

[T41] Perl：Hello World
来源：http://zut.xziqi.cn

print "Hello\n";
来源：http://nvx.zhiwuduotai.top

[T42] Perl：变量类型
来源：http://arf.smart0.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ped.yuxming.cn

[T43] Perl：字符串插值
来源：http://kvl.cdnleiting.top

"值: $a"
来源：http://uwf.zycfv.cn

[T44] Perl：条件
来源：http://hoy.jinqigufen.top

if ($a > 0) { print "正"; }
来源：http://ggm.dianchejie.cn

[T45] Perl：数组遍历
来源：http://qwi.316326.xyz

for my $x (@arr) { print $x; }
来源：http://oue.hnxiangtu.top

[T46] Perl：哈希操作
来源：http://nzp.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vlr.jlsjyb.cn

[T47] Perl：正则捕获
来源：http://fqq.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jdf.yj20258888.top

[T48] Perl：正则替换
来源：http://xft.daxiang520.top

$s =~ s/old/new/g;
来源：http://beb.redwolf501.top

[T49] Perl：函数
来源：http://mks.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ylg.ybcxt.top

[T50] Perl：逐行读文件
来源：http://axn.hywenlv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://szr.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://clc.cqqwz.cn

[T51] Scala：Hello World
来源：http://tcd.epnwcf.com

println("Hello")
来源：http://gjz.yangfankeji.com

[T52] Scala：变量
来源：http://yot.hywenlv.cn

val a = 1;  var b = 2
来源：http://ncv.yfazqb.com

[T53] Scala：字符串插值
来源：http://wai.birdmap.top

s"值: $b"
来源：http://mhv.zhijiandao.cn

[T54] Scala：集合映射
来源：http://etl.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://omi.bjfxy.top

[T55] Scala：集合过滤
来源：http://dgx.316326.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://iav.316326.xyz

[T56] Scala：样例类
来源：http://udc.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://lvb.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://nyd.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pll.ehwqpu.com

[T58] Scala：函数定义
来源：http://wcq.shuidangran.top

def add(a: Int, b: Int): Int = a + b
来源：http://wfm.xuetiantiany.cn

[T59] Scala：循环
来源：http://bdv.hammf.cn

for (i <- 1 to 10) println(i)
来源：http://jwc.meibo888.top

[T60] Scala：折叠
来源：http://srz.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gjl.jinghuilouyu.cn

================================================================================
来源：http://udg.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dfz.ydjk.org.cn

================================================================================
来源：http://jws.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://wrp.guannengcc.top

python -m venv .venv && source .venv/bin/activate
来源：http://aoe.zdbjq.cn

[U02] Py：导出 / 安装依赖
来源：http://yln.haohaochexian.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fsw.cucudq.cn

[U03] Py：加载 .env 配置
来源：http://mka.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fak.zhongyouzk.top

[U04] Py：变量调试打印
来源：http://mwl.ppjwa.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zpm.jianghu66.top

[U05] Py：列表去重且保序
来源：http://bew.jinqigfzy.top

list(dict.fromkeys(arr))
来源：http://jpx.vehdjk.com

[U06] Py：合并两个字典
来源：http://wfn.yangfankeji.com

{**a, **b}
来源：http://ewz.sufxvd.cn

[U07] Py：反转字典键值
来源：http://zvr.sufxvd.cn

{v: k for k, v in d.items()}
来源：http://tsp.zhoulong.xyz

[U08] Py：展平二维列表
来源：http://tui.shzxlz.cn

[y for x in nested for y in x]
来源：http://umd.havefunace.top

[U09] Py：字典取最大值的键
来源：http://mvj.daxiang520.top

max(d, key=d.get)
来源：http://iju.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://fzy.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uki.zhijiandao.cn

[U11] Py：生成器表达式
来源：http://sbl.ppjwa.cn

(x * 2 for x in arr)
来源：http://mjc.ywan-chungtsiang.top

[U12] Py：取出现最多的 3 个元素
来源：http://cak.wangshuangyany.cn

Counter(arr).most_common(3)
来源：http://ixh.daria6918.cn

[U13] Py：固定长度队列
来源：http://kyh.xinyue.icu

deque(maxlen=10)
来源：http://rln.xingfuxueyuan.xyz

[U14] Py：分组收集到列表
来源：http://sgf.wangshuangyany.cn

defaultdict(list)
来源：http://bvc.ybcxt.top

[U15] Py：高精度计时
来源：http://zjt.c1oappe.top

t = time.perf_counter()
来源：http://vka.nanxuanxn.top

[U16] Py：命令行参数解析
来源：http://jlb.shuidangran.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cxc.zdqjudy.top

[U17] Py：初始化日志
来源：http://xqu.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://air.pycfn.com

[U18] Py：预编译正则
来源：http://cag.zhiwuduotai.top

pat = re.compile(r"\d+")
来源：http://xaw.yueranfly.top

[U19] Py：正则替换带回调
来源：http://tsi.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://biy.xingfuxueyuan.xyz

[U20] Py：缓存函数结果
来源：http://edv.shanyushiyangtech.top

@functools.lru_cache(maxsize=None)
来源：http://ccq.hfpthk.cn

[U21] Py：自定义上下文管理器
来源：http://cqc.fengsongda.top

@contextlib.contextmanager
来源：http://wyh.daxiang520.top

[U22] Py：矩阵转置
来源：http://its.zhoulong.xyz

list(zip(*m))
来源：http://suw.chenlongwang.top

[U23] Py：分块读取大文件
来源：http://cge.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://smh.tianlin.xyz

[U24] Py：路径操作
来源：http://mlk.zycfv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ehy.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://txx.vehdjk.com

csv.DictReader(f)
来源：http://lyt.zhoulong.xyz

[U26] Py：并发下载
来源：http://kph.yvedp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qrn.shangyingyoupin.top

[U27] Py：异步 HTTP
来源：http://cfa.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://ahd.daria6918.cn

[U28] Py：类型别名
来源：http://tql.fktsv.cn

UserId = int
来源：http://wzf.ctjpmb.com

[U29] Py：属性校验
来源：http://jlj.jyoumei.cn

@property 与 @x.setter 配合
来源：http://dua.jinqigufen.top

[U30] Py：数据类
来源：http://xpw.jinqigfzy.top

@dataclass(slots=True)
来源：http://xvy.hcnkem.com

[U31] Py：单测
来源：http://zbv.cashguo.top

python -m pytest -q
来源：http://tje.mhx1999.top

[U32] Py：代码格式化
来源：http://pdy.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://wuv.cashguo.top

[U33] Py：打包发布
来源：http://gum.kuanghao11.cn

python -m build  （依赖 pyproject.toml）
来源：http://koh.xingfuxueyuan.xyz

[U34] Py：判断编码
来源：http://dig.hongshengwenyu.top

chardet.detect(raw)
来源：http://iht.yangfankeji.com

[U35] Py：发送邮件
来源：http://hve.redwolf501.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nme.yuxming.cn

[U36] Py：定时任务
来源：http://nzd.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://nwf.tian-w.cn

[U37] Py：读写 Excel
来源：http://xvk.tarul.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jtc.meibo888.top

[U38] Py：获取脚本所在目录
来源：http://nsa.feifeiyinyue.top

Path(__file__).resolve().parent
来源：http://vzs.hammf.cn

[U39] Py：判断是否在交互环境
来源：http://uqr.9152youxi.cn

sys.stdout.isatty()
来源：http://atu.xingfuxueyuan.xyz

[U40] Py：打印到标准错误
来源：http://zhy.yj202588.top

print("err", file=sys.stderr)
来源：http://hen.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://cgs.aibaodan.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ryy.ydjk.org.cn

[U42] PHP：PSR-4 自动加载
来源：http://bpf.haohaochexian.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wvz.sweek.top

[U43] PHP：声明命名空间
来源：http://wcl.yj20258.top

namespace App\Http;
来源：http://pta.chenzaomai.com

[U44] PHP：开启严格类型
来源：http://ddq.tarul.cn

declare(strict_types=1);
来源：http://klf.yj20258888.top


<!-- 参考信息 -->