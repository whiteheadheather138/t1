代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://crc.guowangkeji.top

[S21] C：字符类别判断
来源：http://dpw.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rll.fzhhl.top

[S22] C：字符串转数字
来源：http://kwi.yanxiufei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nan.wangshuangyany.cn

[S23] C：随机数
来源：http://mhr.tianlin.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://gzc.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://bzh.zhiwuduotai.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oei.yueranfly.top

[S25] C：内存拷贝
来源：http://zas.haohaochexian.top

memcpy(dst, src, n);
来源：http://toi.yanxiufei.cn

[S26] C：内存清零
来源：http://pis.xziqi.cn

memset(a, 0, sizeof a);
来源：http://trl.jiagoushi.top

[S27] C：定义常量
来源：http://dbe.bjfxy.top

const double PI = 3.14159;
来源：http://qnx.bbcook.cn

[S28] C：静态变量
来源：http://ppc.haohaochexian.top

static int counter = 0;
来源：http://eui.316326.xyz

[S29] C：变参函数
来源：http://wpk.nanxuanxn.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xkb.cdnleiting.top

[S30] C：头文件保护
来源：http://lfl.9152youxi.cn

#ifndef X_H
来源：http://hnx.nanxinkj.top

#define X_H
来源：http://szs.tarul.cn

#endif
来源：http://jcd.mhx1999.top

[S31] C++：Hello World
来源：http://awe.hammf.cn

#include <iostream>
来源：http://chd.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://imy.sjlbkw.cn

[S32] C++：字符串
来源：http://ctq.cheryme.top

std::string s = "hi";  s += "!";
来源：http://kwk.fanxiaobao.xyz

[S33] C++：vector 增删
来源：http://hjq.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iar.hesvh.cn

[S34] C++：遍历 vector
来源：http://nea.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://isj.zdbjq.cn

[S35] C++：map
来源：http://mgf.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pkf.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://chh.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dap.xuanzx.com

[S37] C++：set
来源：http://rrp.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fwl.fzhhl.top

[S38] C++：排序
来源：http://dzg.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://uja.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://ejl.pengpengdd.cyou

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mhx.smart0.xyz

[S40] C++：查找元素
来源：http://wmc.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gbn.c1oappe.top

[S41] C++：类与构造函数
来源：http://jjt.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dpw.zycfv.cn

[S42] C++：继承与虚函数
来源：http://fik.sufxvd.cn

class B : public Base { public: void f() override {} };
来源：http://ozo.hongshengwenyu.top

[S43] C++：智能指针
来源：http://jna.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://ckm.c1oappe.top

[S44] C++：引用传参
来源：http://ckc.vehdjk.com

void inc(int &x) { ++x; }
来源：http://vto.jinqigfzy.top

[S45] C++：lambda
来源：http://ngl.quarkkingdee.top

auto add = [](int a, int b) { return a + b; };
来源：http://ikn.nanxuanxn.top

[S46] C++：函数模板
来源：http://huq.nanxinkj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tfr.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://ihv.tianlin.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ssh.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://kwr.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://vbz.tarul.cn

while (std::getline(in, line)) { }
来源：http://bur.yangfankeji.com

[S49] C++：写文件
来源：http://vga.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://egy.kuanghao11.cn

[S50] C++：格式化数字
来源：http://hco.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zgk.snrcjt.cn

[S51] C++：显式类型转换
来源：http://ygs.fktsv.cn

static_cast<double>(a) / b
来源：http://flq.yangfankeji.com

[S52] C++：const 与 noexcept
来源：http://faa.shuidangran.top

int size() const noexcept { return n_; }
来源：http://oec.xuanzx.com

[S53] C++：移动语义
来源：http://nfn.meibo888.top

std::vector<int> w = std::move(v);
来源：http://xpq.cheryme.top

[S54] C++：异常处理
来源：http://xjv.cqqwz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gzk.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://jgq.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dms.shangyingyoupin.top

[S56] C++：optional
来源：http://gwr.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kjm.yvedp.cn

[S57] C++：编译期常量
来源：http://yys.fktsv.cn

constexpr int N = 10;
来源：http://xcr.tian-w.cn

[S58] C++：命名空间
来源：http://zet.yangfankeji.com

namespace ns { int f() { return 1; } }
来源：http://gwr.fktsv.cn

[S59] C++：静态断言
来源：http://kbr.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mjn.daxiang520.top

[S60] C++：遍历并删除元素
来源：http://gfh.snrcjt.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vib.fzhhl.top

================================================================================
来源：http://qld.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ekh.svipenyu.cn

================================================================================
来源：http://xod.jinqigufen.top

[T01] Kotlin：Hello World
来源：http://dmv.c1oappe.top

println("Hello")
来源：http://eou.aibaodan.cn

[T02] Kotlin：变量
来源：http://cwz.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tzs.aibaodan.cn

[T03] Kotlin：字符串模板
来源：http://zsq.shuidangran.top

"值: $b"
来源：http://wjk.sweek.top

[T04] Kotlin：空安全
来源：http://igy.daria6918.cn

val n: String? = null;  n?.length
来源：http://jlm.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://kdl.bjfxy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ezm.bbcook.cn

[T06] Kotlin：集合映射
来源：http://wdo.pycfn.com

listOf(1, 2, 3).map { it * 2 }
来源：http://amg.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://dvu.sysykeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://evx.zhengqikj.top

[T08] Kotlin：数据类
来源：http://caw.hammf.cn

data class User(val name: String, val age: Int)
来源：http://tct.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://etl.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://zhy.redwolf501.top

[T10] Kotlin：默认参数
来源：http://gyr.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://yjb.fktsv.cn

[T11] Kotlin：协程
来源：http://ffa.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://voo.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://dal.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://qct.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://cha.316326.xyz

val m = mapOf("a" to 1)
来源：http://rrm.shanyushiyangtech.top

[T14] Kotlin：循环
来源：http://jtg.fehbvm.com

for (i in 1..10) println(i)
来源：http://gqb.cashguo.top

[T15] Kotlin：接口
来源：http://jao.tarul.cn

interface Shape { fun area(): Double }
来源：http://stq.zhongyouzk.top

[T16] Swift：Hello World
来源：http://mlz.xziqi.cn

print("Hello")
来源：http://enm.ivvv.top

[T17] Swift：变量与常量
来源：http://rij.sweek.top

var a = 1;  let b = 2
来源：http://snh.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://kex.yueranfly.top

"值: \(b)"
来源：http://qoz.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://lmy.nanxuanxn.top

if let n = opt { print(n) }
来源：http://qca.zhixingplan.top

[T20] Swift：数组操作
来源：http://csc.fanxiaobao.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://yac.nanxinkj.top

[T21] Swift：遍历
来源：http://wue.hnxiangtu.top

for x in a { print(x) }
来源：http://zmw.jianghu66.top

[T22] Swift：字典
来源：http://kso.zhoulong.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://zjy.fehbvm.com

[T23] Swift：函数
来源：http://vka.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://soo.yvedp.cn

[T24] Swift：闭包
来源：http://syy.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://mil.yuxming.cn

[T25] Swift：结构体
来源：http://mui.jianghu66.top

struct P { var x: Int }
来源：http://whi.hywenlv.cn

[T26] Swift：类与重写
来源：http://hsm.fengsongda.top

class A: Base { override func f() {} }
来源：http://whd.epnwcf.com

[T27] Swift：错误处理
来源：http://qge.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://xyc.aizwys.cn

[T28] Swift：枚举
来源：http://wgi.ydzc1.top

enum Color { case red, green }
来源：http://hnh.hfpthk.cn

[T29] Swift：guard 提前返回
来源：http://aql.sjlbkw.cn

guard let x = opt else { return }
来源：http://nah.bbcook.cn

[T30] Swift：协议
来源：http://yex.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://ugl.52xcode.cn

[T31] Lua：Hello World
来源：http://ejl.yfazqb.com

print("Hello")
来源：http://ghk.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://aaz.bbcook.cn

local a = 1
来源：http://urb.gaohongyu789.top

[T33] Lua：表（数组）
来源：http://jgm.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ujj.zhongyouzk.top

[T34] Lua：遍历表
来源：http://olx.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ium.smart0.xyz

[T35] Lua：字典表
来源：http://lwb.zhengqikj.top

local d = { a = 1 };  d.b = 2
来源：http://vkc.fanxiaobao.xyz

[T36] Lua：函数
来源：http://rvq.shanyushiyangkeji.top

function add(a, b) return a + b end
来源：http://cnn.hcnkem.com

[T37] Lua：字符串拼接
来源：http://twq.xuetiantiany.cn

"a" .. "b"
来源：http://tfr.aizwys.cn

[T38] Lua：条件
来源：http://kwe.hongshengwenyu.top

if x > 0 then print("正") end
来源：http://koq.yangfankeji.com

[T39] Lua：模式匹配
来源：http://iec.epnwcf.com

string.find(s, "%d+")
来源：http://foh.ppjwa.cn

[T40] Lua：元表
来源：http://tzd.tianlin.xyz

setmetatable({}, { __index = base })
来源：http://nle.wangdashe.top

[T41] Perl：Hello World
来源：http://fnk.zdqjudy.top

print "Hello\n";
来源：http://cci.hnxiangtu.top

[T42] Perl：变量类型
来源：http://bul.jianghu66.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sgh.zdbjq.cn

[T43] Perl：字符串插值
来源：http://rkx.zdbjq.cn

"值: $a"
来源：http://mnb.hesvh.cn

[T44] Perl：条件
来源：http://lho.shanyushiyangtech.top

if ($a > 0) { print "正"; }
来源：http://pde.yuxming.cn

[T45] Perl：数组遍历
来源：http://icz.ybcxt.top

for my $x (@arr) { print $x; }
来源：http://hgq.svipenyu.cn

[T46] Perl：哈希操作
来源：http://kal.xuanzx.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qda.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://bek.cdnleiting.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://oyg.sjlbkw.cn

[T48] Perl：正则替换
来源：http://weg.cheryme.top

$s =~ s/old/new/g;
来源：http://jxf.hesvh.cn

[T49] Perl：函数
来源：http://lah.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gjb.nwbrower.top

[T50] Perl：逐行读文件
来源：http://rri.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rdf.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://hfl.gzhubu.top

[T51] Scala：Hello World
来源：http://iue.nwbrower.top

println("Hello")
来源：http://ywv.hnqzz.top

[T52] Scala：变量
来源：http://wdj.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://hxr.uphjek.com

[T53] Scala：字符串插值
来源：http://vnr.ydjk.org.cn

s"值: $b"
来源：http://xou.jinghuilouyu.cn

[T54] Scala：集合映射
来源：http://iud.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://azo.pycfn.com

[T55] Scala：集合过滤
来源：http://wrf.uphjek.com

List(1, 2, 3).filter(_ > 1)
来源：http://gwb.ehwqpu.com

[T56] Scala：样例类
来源：http://jrs.yfazqb.com

case class User(name: String, age: Int)
来源：http://ueo.daxiang520.top

[T57] Scala：模式匹配
来源：http://iqm.chenjidiqi.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://nmm.jyoumei.cn

[T58] Scala：函数定义
来源：http://uso.cheryme.top

def add(a: Int, b: Int): Int = a + b
来源：http://uhb.0kj1m.cn

[T59] Scala：循环
来源：http://izm.dianchejie.cn

for (i <- 1 to 10) println(i)
来源：http://xzy.zhixingplan.top

[T60] Scala：折叠
来源：http://pvi.sxryk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vkc.meibo888.top

================================================================================
来源：http://szj.yuanzhike.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zmc.jiagoushi.top

================================================================================
来源：http://ccf.guowangkeji.top

[U01] Py：创建虚拟环境
来源：http://duk.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://zsd.aizwys.cn

[U02] Py：导出 / 安装依赖
来源：http://cck.hnqzz.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hws.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://ouc.bjfxy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xxg.nwbrower.top

[U04] Py：变量调试打印
来源：http://tfb.yj20258888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ezw.mhx1999.top

[U05] Py：列表去重且保序
来源：http://bhp.uphjek.com

list(dict.fromkeys(arr))
来源：http://ufv.pycfn.com

[U06] Py：合并两个字典
来源：http://xlk.uphjek.com

{**a, **b}
来源：http://jdk.yueranfly.top

[U07] Py：反转字典键值
来源：http://izo.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://qia.ivvv.top

[U08] Py：展平二维列表
来源：http://gcr.haohaochexian.top

[y for x in nested for y in x]
来源：http://nsh.zhengqikj.top

[U09] Py：字典取最大值的键
来源：http://nxz.sufxvd.cn

max(d, key=d.get)
来源：http://uqs.svipenyu.cn

[U10] Py：按值排序字典
来源：http://xuy.jqgfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://had.guowangkeji.top

[U11] Py：生成器表达式
来源：http://ckj.shanyushiyangtech.top

(x * 2 for x in arr)
来源：http://roj.cucudq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vda.gzhubu.top

Counter(arr).most_common(3)
来源：http://esk.yvedp.cn

[U13] Py：固定长度队列
来源：http://sfx.nanxinkj.top

deque(maxlen=10)
来源：http://kzu.havefunace.top

[U14] Py：分组收集到列表
来源：http://hwk.xylfe.cn

defaultdict(list)
来源：http://okv.c1oappe.top

[U15] Py：高精度计时
来源：http://azn.zhoulong.xyz

t = time.perf_counter()
来源：http://rlh.yueranfly.top

[U16] Py：命令行参数解析
来源：http://oix.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jgt.ybcxt.top

[U17] Py：初始化日志
来源：http://bbd.gzhubu.top

logging.basicConfig(level=logging.INFO)
来源：http://vzf.yj202588.top

[U18] Py：预编译正则
来源：http://qyk.shangyingyoupin.top

pat = re.compile(r"\d+")
来源：http://dus.hysaishi.cn

[U19] Py：正则替换带回调
来源：http://prz.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oaj.jyoumei.cn

[U20] Py：缓存函数结果
来源：http://rqg.shangyingyoupin.top

@functools.lru_cache(maxsize=None)
来源：http://hjv.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://pfq.zdbjq.cn

@contextlib.contextmanager
来源：http://ftl.fengsongda.top

[U22] Py：矩阵转置
来源：http://kaq.shanyushiyangkeji.top

list(zip(*m))
来源：http://sdx.jinqigufen.top

[U23] Py：分块读取大文件
来源：http://tfo.ybcxt.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jsg.ydzc1.top

[U24] Py：路径操作
来源：http://ldv.aizwys.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sud.tanke756.top

[U25] Py：CSV 按字典读
来源：http://tdu.jqgufenzy.top

csv.DictReader(f)
来源：http://eps.chenjidiqi.icu

[U26] Py：并发下载
来源：http://ezu.yonumen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kcp.hfpthk.cn

[U27] Py：异步 HTTP
来源：http://lfp.epnwcf.com

aiohttp.ClientSession() 配合 async with
来源：http://cbg.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://btg.c1oappe.top

UserId = int
来源：http://zba.hnqzz.top

[U29] Py：属性校验
来源：http://kwo.sjlbkw.cn

@property 与 @x.setter 配合
来源：http://cxg.gogol.net.cn

[U30] Py：数据类
来源：http://uqt.sysykeji.top

@dataclass(slots=True)
来源：http://tfd.fanxiaobao.xyz

[U31] Py：单测
来源：http://jhn.gogol.net.cn

python -m pytest -q
来源：http://jhp.yj202588.top

[U32] Py：代码格式化
来源：http://rik.snrcjt.cn

ruff format . && ruff check --fix .
来源：http://nmz.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://kcj.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://ezq.chenzaomai.com

[U34] Py：判断编码
来源：http://cbh.dianchejie.cn

chardet.detect(raw)
来源：http://bfd.yangfankeji.com

[U35] Py：发送邮件
来源：http://sgb.smart0.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bcm.jinqigfzy.top

[U36] Py：定时任务
来源：http://qgb.yanxiufei.cn

schedule.every(10).minutes.do(job)
来源：http://pij.yfazqb.com

[U37] Py：读写 Excel
来源：http://vbs.dashuyun.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rnh.zhixingplan.top

[U38] Py：获取脚本所在目录
来源：http://aya.wangshuangyany.cn

Path(__file__).resolve().parent
来源：http://mnn.pycfn.com

[U39] Py：判断是否在交互环境
来源：http://biq.zdbjq.cn

sys.stdout.isatty()
来源：http://tlh.nwbrower.top

[U40] Py：打印到标准错误
来源：http://sou.shangyingyoupin.top

print("err", file=sys.stderr)
来源：http://lfg.9152youxi.cn

[U41] PHP：初始化 Composer 项目
来源：http://knk.vehdjk.com

composer init;  composer require guzzlehttp/guzzle
来源：http://zci.tarul.cn

[U42] PHP：PSR-4 自动加载
来源：http://gyd.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tvt.svipenyu.cn

[U43] PHP：声明命名空间
来源：http://nfj.dashuyun.cn

namespace App\Http;
来源：http://dyx.andypj.xyz

[U44] PHP：开启严格类型
来源：http://hni.tian-w.cn

declare(strict_types=1);
来源：http://kgh.jyoumei.cn


<!-- 参考信息 -->