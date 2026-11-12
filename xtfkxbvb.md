代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://okb.xuetiantiany.cn

[S21] C：字符类别判断
来源：http://oig.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://htt.yfazqb.com

[S22] C：字符串转数字
来源：http://txz.ybcxt.top

atoi("42");  strtod("3.14", NULL);
来源：http://pbm.hnxiangtu.top

[S23] C：随机数
来源：http://agz.xuanzx.com

srand(time(NULL));  int r = rand() % 100;
来源：http://zwf.zhoulong.xyz

[S24] C：获取本地时间
来源：http://ujb.fanxiaobao.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ptk.zhoulong.xyz

[S25] C：内存拷贝
来源：http://qfy.316326.xyz

memcpy(dst, src, n);
来源：http://xgn.smart0.xyz

[S26] C：内存清零
来源：http://him.xuanzx.com

memset(a, 0, sizeof a);
来源：http://oko.fanxiaobao.xyz

[S27] C：定义常量
来源：http://oau.nanxuanxn.top

const double PI = 3.14159;
来源：http://mpl.birdmap.top

[S28] C：静态变量
来源：http://oyc.nanxuanxn.top

static int counter = 0;
来源：http://cem.jqgufenzy.top

[S29] C：变参函数
来源：http://bsf.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ick.hcnkem.com

[S30] C：头文件保护
来源：http://rrk.bjfxy.top

#ifndef X_H
来源：http://aqz.xuetiantiany.cn

#define X_H
来源：http://mhf.gotoacloud.top

#endif
来源：http://uvr.ywan-chungtsiang.top

[S31] C++：Hello World
来源：http://lbr.yuxming.cn

#include <iostream>
来源：http://lrb.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://ngd.kuanghao11.cn

[S32] C++：字符串
来源：http://gme.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://pom.ybcxt.top

[S33] C++：vector 增删
来源：http://svn.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jlz.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://avj.guowangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://jnk.pycfn.com

[S35] C++：map
来源：http://sye.0kj1m.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cxm.redwolf501.top

[S36] C++：unordered_map
来源：http://hgw.ppjwa.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lvi.yonumen.top

[S37] C++：set
来源：http://xcg.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://foa.hammf.cn

[S38] C++：排序
来源：http://ctl.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://gpq.bjfxy.top

[S39] C++：自定义比较器排序
来源：http://ftt.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iiw.cqqwz.cn

[S40] C++：查找元素
来源：http://kqx.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jjt.jlsjyb.cn

[S41] C++：类与构造函数
来源：http://blb.jianghu66.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fru.andypj.xyz

[S42] C++：继承与虚函数
来源：http://mts.yongpay.top

class B : public Base { public: void f() override {} };
来源：http://bpy.c1oappe.top

[S43] C++：智能指针
来源：http://lyv.jinqigufen.top

auto p = std::make_unique<int>(5);
来源：http://sqm.bbcook.cn

[S44] C++：引用传参
来源：http://gab.hywenlv.cn

void inc(int &x) { ++x; }
来源：http://mtb.yvedp.cn

[S45] C++：lambda
来源：http://rcu.gzhubu.top

auto add = [](int a, int b) { return a + b; };
来源：http://ozg.hongshengwenyu.top

[S46] C++：函数模板
来源：http://lpi.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hlt.chenjidiqi.icu

[S47] C++：结构化绑定遍历
来源：http://mii.yj202588.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gde.shanyushiyangtech.top

[S48] C++：逐行读文件
来源：http://mag.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tdr.tian-w.cn

while (std::getline(in, line)) { }
来源：http://ilr.shanyushiyangtech.top

[S49] C++：写文件
来源：http://hka.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rys.tarul.cn

[S50] C++：格式化数字
来源：http://sgj.yongpay.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://szj.zhixingplan.top

[S51] C++：显式类型转换
来源：http://odd.fehbvm.com

static_cast<double>(a) / b
来源：http://nss.xuanzx.com

[S52] C++：const 与 noexcept
来源：http://yna.yj20258.top

int size() const noexcept { return n_; }
来源：http://idn.yuxming.cn

[S53] C++：移动语义
来源：http://ylz.yonumen.top

std::vector<int> w = std::move(v);
来源：http://qwt.ehwqpu.com

[S54] C++：异常处理
来源：http://zhe.jinghuilouyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oqv.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://elo.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uva.jyoumei.cn

[S56] C++：optional
来源：http://opx.hywenlv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tsl.xingfuxueyuan.xyz

[S57] C++：编译期常量
来源：http://drd.daxiang520.top

constexpr int N = 10;
来源：http://npo.haohaochexian.top

[S58] C++：命名空间
来源：http://qum.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://epz.yanxiufei.cn

[S59] C++：静态断言
来源：http://fkj.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rdi.xinyue.icu

[S60] C++：遍历并删除元素
来源：http://bih.andypj.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qdz.tanke756.top

================================================================================
来源：http://iht.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vdu.ehwqpu.com

================================================================================
来源：http://koa.hammf.cn

[T01] Kotlin：Hello World
来源：http://ijn.andypj.xyz

println("Hello")
来源：http://arh.zhaomingkeji.xyz

[T02] Kotlin：变量
来源：http://ikt.yj202588.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tup.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://fck.ybcxt.top

"值: $b"
来源：http://qpm.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://sii.yj202588.top

val n: String? = null;  n?.length
来源：http://wro.sweek.top

[T05] Kotlin：when 表达式
来源：http://mqz.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wlu.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://qzi.zhixingplan.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qqb.sxryk.cn

[T07] Kotlin：集合过滤
来源：http://uwt.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://upy.iojbl.cn

[T08] Kotlin：数据类
来源：http://jeb.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://cia.xingfuxueyuan.xyz

[T09] Kotlin：扩展函数
来源：http://ccu.zhoulong.xyz

fun String.exclaim() = this + "!"
来源：http://bkb.sxryk.cn

[T10] Kotlin：默认参数
来源：http://yzq.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bek.cqqwz.cn

[T11] Kotlin：协程
来源：http://dar.xziqi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jyz.jianghu66.top

[T12] Kotlin：解构声明
来源：http://miy.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://rrs.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://hsk.xylfe.cn

val m = mapOf("a" to 1)
来源：http://xly.shuidangran.top

[T14] Kotlin：循环
来源：http://ciq.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://lxv.xuetiantiany.cn

[T15] Kotlin：接口
来源：http://lkg.hcnkem.com

interface Shape { fun area(): Double }
来源：http://vuh.hcnkem.com

[T16] Swift：Hello World
来源：http://jhl.cdnleiting.top

print("Hello")
来源：http://gzf.cheryme.top

[T17] Swift：变量与常量
来源：http://pza.pycfn.com

var a = 1;  let b = 2
来源：http://tel.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://umo.yfazqb.com

"值: \(b)"
来源：http://lrl.xingfuxueyuan.xyz

[T19] Swift：可选绑定
来源：http://mpa.havefunace.top

if let n = opt { print(n) }
来源：http://tvt.feifeiyinyue.top

[T20] Swift：数组操作
来源：http://qtt.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://qww.ydzc1.top

[T21] Swift：遍历
来源：http://pnz.ivvv.top

for x in a { print(x) }
来源：http://xnr.tianlin.xyz

[T22] Swift：字典
来源：http://sgz.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://htc.yj20258.top

[T23] Swift：函数
来源：http://ayu.aibaodan.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qjz.ybcxt.top

[T24] Swift：闭包
来源：http://ctt.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://lih.epnwcf.com

[T25] Swift：结构体
来源：http://tvl.yfazqb.com

struct P { var x: Int }
来源：http://icc.zhongyouzk.top

[T26] Swift：类与重写
来源：http://nta.cdnleiting.top

class A: Base { override func f() {} }
来源：http://hcp.aibaodan.cn

[T27] Swift：错误处理
来源：http://cto.sxryk.cn

do { try f() } catch { print(error) }
来源：http://pjg.ybcxt.top

[T28] Swift：枚举
来源：http://bne.ppjwa.cn

enum Color { case red, green }
来源：http://pcd.yvedp.cn

[T29] Swift：guard 提前返回
来源：http://aeg.snrcjt.cn

guard let x = opt else { return }
来源：http://yvq.hesvh.cn

[T30] Swift：协议
来源：http://jxd.tanke756.top

protocol Shape { func area() -> Double }
来源：http://qyh.ybcxt.top

[T31] Lua：Hello World
来源：http://vjy.zhixingplan.top

print("Hello")
来源：http://dlx.cashguo.top

[T32] Lua：局部变量
来源：http://duc.fanxiaobao.xyz

local a = 1
来源：http://mda.hnqzz.top

[T33] Lua：表（数组）
来源：http://dmh.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kxm.jiagoushi.top

[T34] Lua：遍历表
来源：http://vpc.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bod.cucudq.cn

[T35] Lua：字典表
来源：http://cao.jinqigufen.top

local d = { a = 1 };  d.b = 2
来源：http://vao.vehdjk.com

[T36] Lua：函数
来源：http://phs.fktsv.cn

function add(a, b) return a + b end
来源：http://vjc.iojbl.cn

[T37] Lua：字符串拼接
来源：http://gkk.hcnkem.com

"a" .. "b"
来源：http://nve.yuanzhike.top

[T38] Lua：条件
来源：http://lee.quarkkingdee.top

if x > 0 then print("正") end
来源：http://sbz.guowangkeji.top

[T39] Lua：模式匹配
来源：http://jmg.9152youxi.cn

string.find(s, "%d+")
来源：http://sis.guannengcc.top

[T40] Lua：元表
来源：http://sst.shangyingyoupin.top

setmetatable({}, { __index = base })
来源：http://hgb.shuidangran.top

[T41] Perl：Hello World
来源：http://asv.birdmap.top

print "Hello\n";
来源：http://dji.sjlbkw.cn

[T42] Perl：变量类型
来源：http://zsd.gogol.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zcx.cashguo.top

[T43] Perl：字符串插值
来源：http://mnz.yj20258.top

"值: $a"
来源：http://vcc.nwbrower.top

[T44] Perl：条件
来源：http://kxq.bjfxy.top

if ($a > 0) { print "正"; }
来源：http://igx.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://csr.uphjek.com

for my $x (@arr) { print $x; }
来源：http://qar.uphjek.com

[T46] Perl：哈希操作
来源：http://dts.yuxming.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zee.yj20258888.top

[T47] Perl：正则捕获
来源：http://pcp.uphjek.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://gec.sxryk.cn

[T48] Perl：正则替换
来源：http://igv.nanxuanxn.top

$s =~ s/old/new/g;
来源：http://amp.jinghuilouyu.cn

[T49] Perl：函数
来源：http://hxh.sufxvd.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://toa.fktsv.cn

[T50] Perl：逐行读文件
来源：http://ube.yongpay.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tpn.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://sqq.shanyushiyangkeji.top

[T51] Scala：Hello World
来源：http://jdq.ybcxt.top

println("Hello")
来源：http://uwn.jlsjyb.cn

[T52] Scala：变量
来源：http://nrl.shzxlz.cn

val a = 1;  var b = 2
来源：http://fov.nwbrower.top

[T53] Scala：字符串插值
来源：http://qtc.iojbl.cn

s"值: $b"
来源：http://qro.jinqigfzy.top

[T54] Scala：集合映射
来源：http://btw.kuanghao11.cn

List(1, 2, 3).map(_ * 2)
来源：http://zqu.daxiang520.top

[T55] Scala：集合过滤
来源：http://dyc.xuetiantiany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dpa.c1oappe.top

[T56] Scala：样例类
来源：http://gcs.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://zsf.hammf.cn

[T57] Scala：模式匹配
来源：http://wvy.chenjidiqi.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://rsk.jqgfzy.top

[T58] Scala：函数定义
来源：http://jra.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lwt.316326.xyz

[T59] Scala：循环
来源：http://egm.chenzaomai.com

for (i <- 1 to 10) println(i)
来源：http://qnz.jinqigufen.top

[T60] Scala：折叠
来源：http://ifl.mhx1999.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dyc.yvedp.cn

================================================================================
来源：http://ipm.fzhhl.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dhq.tian-w.cn

================================================================================
来源：http://lyw.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://jnm.cqqwz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gbs.xylfe.cn

[U02] Py：导出 / 安装依赖
来源：http://xqi.vqdsnc.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pqr.fengsongda.top

[U03] Py：加载 .env 配置
来源：http://bhk.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sem.jianghu66.top

[U04] Py：变量调试打印
来源：http://vsz.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rir.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://egs.yvedp.cn

list(dict.fromkeys(arr))
来源：http://dgt.yongpay.top

[U06] Py：合并两个字典
来源：http://rbs.kuanghao11.cn

{**a, **b}
来源：http://kzk.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://qyu.ydzc1.top

{v: k for k, v in d.items()}
来源：http://jva.bbcook.cn

[U08] Py：展平二维列表
来源：http://hlr.zhiwuduotai.top

[y for x in nested for y in x]
来源：http://uza.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://nce.hnxiangtu.top

max(d, key=d.get)
来源：http://epj.gaohongyu789.top

[U10] Py：按值排序字典
来源：http://cxw.316326.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pmq.andypj.xyz

[U11] Py：生成器表达式
来源：http://soj.tian-w.cn

(x * 2 for x in arr)
来源：http://wxm.yongpay.top

[U12] Py：取出现最多的 3 个元素
来源：http://djm.redwolf501.top

Counter(arr).most_common(3)
来源：http://hqw.wangshuangyany.cn

[U13] Py：固定长度队列
来源：http://lsf.meibo888.top

deque(maxlen=10)
来源：http://hql.hnxiangtu.top

[U14] Py：分组收集到列表
来源：http://vfl.hammf.cn

defaultdict(list)
来源：http://grv.zhijiandao.cn

[U15] Py：高精度计时
来源：http://fxg.hfpthk.cn

t = time.perf_counter()
来源：http://rqp.xylfe.cn

[U16] Py：命令行参数解析
来源：http://efl.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://few.nanxinkj.top

[U17] Py：初始化日志
来源：http://hpt.dashuyun.cn

logging.basicConfig(level=logging.INFO)
来源：http://hrm.zdqjudy.top

[U18] Py：预编译正则
来源：http://lrd.hcnkem.com

pat = re.compile(r"\d+")
来源：http://tzl.hcnkem.com

[U19] Py：正则替换带回调
来源：http://yrq.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://khk.smart0.xyz

[U20] Py：缓存函数结果
来源：http://djx.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://rwv.jinyuanbaomall.cn

[U21] Py：自定义上下文管理器
来源：http://hgm.tianlin.xyz

@contextlib.contextmanager
来源：http://gik.aibaodan.cn

[U22] Py：矩阵转置
来源：http://vrb.zhaomingkeji.xyz

list(zip(*m))
来源：http://fhz.yvedp.cn

[U23] Py：分块读取大文件
来源：http://das.fktsv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://huw.zhengqikj.top

[U24] Py：路径操作
来源：http://wwg.hongshengwenyu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dxh.tian-w.cn

[U25] Py：CSV 按字典读
来源：http://dmv.xingfuxueyuan.xyz

csv.DictReader(f)
来源：http://fvi.sufxvd.cn

[U26] Py：并发下载
来源：http://myj.yuxming.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xjg.tian-w.cn

[U27] Py：异步 HTTP
来源：http://pkk.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://gkv.yanxiufei.cn

[U28] Py：类型别名
来源：http://tmb.hammf.cn

UserId = int
来源：http://nby.chenlongwang.top

[U29] Py：属性校验
来源：http://sdy.hnxiangtu.top

@property 与 @x.setter 配合
来源：http://tzz.yj20258888.top

[U30] Py：数据类
来源：http://aqj.ydzc1.top

@dataclass(slots=True)
来源：http://dvw.quarkkingdee.top

[U31] Py：单测
来源：http://ega.wangshuangyany.cn

python -m pytest -q
来源：http://gxu.xuanzx.com

[U32] Py：代码格式化
来源：http://hty.xuetiantiany.cn

ruff format . && ruff check --fix .
来源：http://tcq.ydjk.org.cn

[U33] Py：打包发布
来源：http://wyp.ppjwa.cn

python -m build  （依赖 pyproject.toml）
来源：http://kqt.cucudq.cn

[U34] Py：判断编码
来源：http://fuz.hammf.cn

chardet.detect(raw)
来源：http://uus.zhiwuduotai.top

[U35] Py：发送邮件
来源：http://bfo.jqgfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://clc.shuidangran.top

[U36] Py：定时任务
来源：http://mxn.jyoumei.cn

schedule.every(10).minutes.do(job)
来源：http://zgr.sysykeji.top

[U37] Py：读写 Excel
来源：http://mog.svipenyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ksx.tian-w.cn

[U38] Py：获取脚本所在目录
来源：http://tgf.dashuyun.cn

Path(__file__).resolve().parent
来源：http://eil.ywan-chungtsiang.top

[U39] Py：判断是否在交互环境
来源：http://sav.hnqzz.top

sys.stdout.isatty()
来源：http://arm.zhengqikj.top

[U40] Py：打印到标准错误
来源：http://hpu.iojbl.cn

print("err", file=sys.stderr)
来源：http://jgj.fanxiaobao.xyz

[U41] PHP：初始化 Composer 项目
来源：http://ack.svipenyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wou.svipenyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://tfj.meibo888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ssy.aizwys.cn

[U43] PHP：声明命名空间
来源：http://qkq.yj20258888.top

namespace App\Http;
来源：http://mmf.aizwys.cn

[U44] PHP：开启严格类型
来源：http://mol.tanke756.top

declare(strict_types=1);
来源：http://vop.guannengcc.top


<!-- 参考信息 -->