代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ars.jianghu66.top

[S25] C：内存拷贝
来源：http://dam.sufxvd.cn

memcpy(dst, src, n);
来源：http://wmu.havefunace.top

[S26] C：内存清零
来源：http://lev.hesvh.cn

memset(a, 0, sizeof a);
来源：http://lpm.daxiang520.top

[S27] C：定义常量
来源：http://hzq.aizwys.cn

const double PI = 3.14159;
来源：http://ksr.sweek.top

[S28] C：静态变量
来源：http://uox.feifeiyinyue.top

static int counter = 0;
来源：http://ise.zhengqikj.top

[S29] C：变参函数
来源：http://fzw.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bbp.sysykeji.top

[S30] C：头文件保护
来源：http://yzc.hcnkem.com

#ifndef X_H
来源：http://bax.jqgufenzy.top

#define X_H
来源：http://ikc.ivvv.top

#endif
来源：http://rnc.snrcjt.cn

[S31] C++：Hello World
来源：http://hop.smart0.xyz

#include <iostream>
来源：http://rfc.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://mko.bbcook.cn

[S32] C++：字符串
来源：http://ckm.havefunace.top

std::string s = "hi";  s += "!";
来源：http://esx.ppjwa.cn

[S33] C++：vector 增删
来源：http://szo.cdnleiting.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://epm.cqqwz.cn

[S34] C++：遍历 vector
来源：http://jzc.shanyushiyangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://nxv.hnqzz.top

[S35] C++：map
来源：http://gvx.yueranfly.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rdk.hfpthk.cn

[S36] C++：unordered_map
来源：http://pzc.aibaodan.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://otw.yuxming.cn

[S37] C++：set
来源：http://yiy.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://unz.yfazqb.com

[S38] C++：排序
来源：http://dox.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://qye.tian-w.cn

[S39] C++：自定义比较器排序
来源：http://hoe.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zlf.quarkkingdee.top

[S40] C++：查找元素
来源：http://wca.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sim.nanxinkj.top

[S41] C++：类与构造函数
来源：http://umj.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dvw.dianchejie.cn

[S42] C++：继承与虚函数
来源：http://bfs.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://zsq.yueranfly.top

[S43] C++：智能指针
来源：http://ert.guannengcc.top

auto p = std::make_unique<int>(5);
来源：http://acm.redwolf501.top

[S44] C++：引用传参
来源：http://mrj.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://fuc.jinghuilouyu.cn

[S45] C++：lambda
来源：http://tdj.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://alz.hammf.cn

[S46] C++：函数模板
来源：http://xhv.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fbv.ehwqpu.com

[S47] C++：结构化绑定遍历
来源：http://sra.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zqb.smart0.xyz

[S48] C++：逐行读文件
来源：http://kpw.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kgm.gzhubu.top

while (std::getline(in, line)) { }
来源：http://wui.hnxiangtu.top

[S49] C++：写文件
来源：http://yjj.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bkg.tarul.cn

[S50] C++：格式化数字
来源：http://bbb.9152youxi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://spr.xingfuxueyuan.xyz

[S51] C++：显式类型转换
来源：http://yol.jqgfzy.top

static_cast<double>(a) / b
来源：http://jon.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://psh.guannengcc.top

int size() const noexcept { return n_; }
来源：http://qpj.jinqigfzy.top

[S53] C++：移动语义
来源：http://rlq.yj20258.top

std::vector<int> w = std::move(v);
来源：http://vac.jyoumei.cn

[S54] C++：异常处理
来源：http://bfx.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://syh.vehdjk.com

[S55] C++：结构化绑定
来源：http://jmn.iojbl.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bdx.zhijiandao.cn

[S56] C++：optional
来源：http://lci.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cyg.yongpay.top

[S57] C++：编译期常量
来源：http://ftn.hnxiangtu.top

constexpr int N = 10;
来源：http://izj.ydjk.org.cn

[S58] C++：命名空间
来源：http://uvp.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://yoq.andypj.xyz

[S59] C++：静态断言
来源：http://edv.zhijiandao.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://twz.hcnkem.com

[S60] C++：遍历并删除元素
来源：http://znw.xingfuxueyuan.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hoe.52xcode.cn

================================================================================
来源：http://jfr.shanyushiyangtech.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vhg.yvedp.cn

================================================================================
来源：http://hvh.epnwcf.com

[T01] Kotlin：Hello World
来源：http://fim.c1oappe.top

println("Hello")
来源：http://vjp.cashguo.top

[T02] Kotlin：变量
来源：http://kbt.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://liv.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://fjs.smart0.xyz

"值: $b"
来源：http://qlg.xinyue.icu

[T04] Kotlin：空安全
来源：http://aym.yuxming.cn

val n: String? = null;  n?.length
来源：http://uec.bbcook.cn

[T05] Kotlin：when 表达式
来源：http://qwt.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ojr.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://xae.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dqy.xuanzx.com

[T07] Kotlin：集合过滤
来源：http://kvc.jqgfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qre.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://xau.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://eff.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://rgk.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://abj.jiagoushi.top

[T10] Kotlin：默认参数
来源：http://xnn.iojbl.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jay.dashuyun.cn

[T11] Kotlin：协程
来源：http://tmz.ywan-chungtsiang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://moj.andypj.xyz

[T12] Kotlin：解构声明
来源：http://msx.yongpay.top

val (a, b) = Pair(1, 2)
来源：http://tnv.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://vha.cdnleiting.top

val m = mapOf("a" to 1)
来源：http://hdq.316326.xyz

[T14] Kotlin：循环
来源：http://pal.hammf.cn

for (i in 1..10) println(i)
来源：http://hum.pycfn.com

[T15] Kotlin：接口
来源：http://afx.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://jux.mhx1999.top

[T16] Swift：Hello World
来源：http://hab.birdmap.top

print("Hello")
来源：http://jcb.bbcook.cn

[T17] Swift：变量与常量
来源：http://iqy.yanxiufei.cn

var a = 1;  let b = 2
来源：http://mjm.snrcjt.cn

[T18] Swift：字符串插值
来源：http://pzz.uphjek.com

"值: \(b)"
来源：http://vbw.jqgfzy.top

[T19] Swift：可选绑定
来源：http://kqa.zhixingplan.top

if let n = opt { print(n) }
来源：http://ypv.cheryme.top

[T20] Swift：数组操作
来源：http://kup.dianchejie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hih.ybcxt.top

[T21] Swift：遍历
来源：http://vwi.chenjidiqi.icu

for x in a { print(x) }
来源：http://txx.zhiwuduotai.top

[T22] Swift：字典
来源：http://eaq.shzxlz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zhu.52xcode.cn

[T23] Swift：函数
来源：http://tmb.jianghu66.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qyw.yongpay.top

[T24] Swift：闭包
来源：http://zeg.ywan-chungtsiang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://srd.kuanghao11.cn

[T25] Swift：结构体
来源：http://dtd.cashguo.top

struct P { var x: Int }
来源：http://ero.yj20258888.top

[T26] Swift：类与重写
来源：http://rdw.chenzaomai.com

class A: Base { override func f() {} }
来源：http://sln.havefunace.top

[T27] Swift：错误处理
来源：http://tvv.quarkkingdee.top

do { try f() } catch { print(error) }
来源：http://gng.jlsjyb.cn

[T28] Swift：枚举
来源：http://ych.zdbjq.cn

enum Color { case red, green }
来源：http://ooc.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://tsa.tianlin.xyz

guard let x = opt else { return }
来源：http://fll.havefunace.top

[T30] Swift：协议
来源：http://lpa.wangshuangyany.cn

protocol Shape { func area() -> Double }
来源：http://abu.andypj.xyz

[T31] Lua：Hello World
来源：http://srf.mhx1999.top

print("Hello")
来源：http://ysb.kuanghao11.cn

[T32] Lua：局部变量
来源：http://aiw.jianghu66.top

local a = 1
来源：http://vtb.sweek.top

[T33] Lua：表（数组）
来源：http://kzi.xuetiantiany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nym.52xcode.cn

[T34] Lua：遍历表
来源：http://vnt.fktsv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yhg.yanxiufei.cn

[T35] Lua：字典表
来源：http://nae.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://oef.wangshuangyany.cn

[T36] Lua：函数
来源：http://ymq.zhoulong.xyz

function add(a, b) return a + b end
来源：http://uje.vqdsnc.cn

[T37] Lua：字符串拼接
来源：http://ygx.shuidangran.top

"a" .. "b"
来源：http://ker.ehwqpu.com

[T38] Lua：条件
来源：http://bxj.haohaochexian.top

if x > 0 then print("正") end
来源：http://ppz.9152youxi.cn

[T39] Lua：模式匹配
来源：http://zlh.zhoulong.xyz

string.find(s, "%d+")
来源：http://ggh.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://avk.c1oappe.top

setmetatable({}, { __index = base })
来源：http://mvg.havefunace.top

[T41] Perl：Hello World
来源：http://mvd.jianghu66.top

print "Hello\n";
来源：http://ovj.jqgufenzy.top

[T42] Perl：变量类型
来源：http://uqp.yonumen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dqa.zhengqikj.top

[T43] Perl：字符串插值
来源：http://tms.hammf.cn

"值: $a"
来源：http://xiu.9152youxi.cn

[T44] Perl：条件
来源：http://poc.xinyue.icu

if ($a > 0) { print "正"; }
来源：http://tfd.vehdjk.com

[T45] Perl：数组遍历
来源：http://zym.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://gvd.quarkkingdee.top

[T46] Perl：哈希操作
来源：http://mso.cucudq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tbk.aibaodan.cn

[T47] Perl：正则捕获
来源：http://gqu.epnwcf.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://bpj.yonumen.top

[T48] Perl：正则替换
来源：http://rai.chenzaomai.com

$s =~ s/old/new/g;
来源：http://tne.chenzaomai.com

[T49] Perl：函数
来源：http://ivn.dianchejie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zbp.yueranfly.top

[T50] Perl：逐行读文件
来源：http://mne.aibaodan.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ywx.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://eaz.bjfxy.top

[T51] Scala：Hello World
来源：http://tpz.zhijiandao.cn

println("Hello")
来源：http://rnj.birdmap.top

[T52] Scala：变量
来源：http://gvy.svipenyu.cn

val a = 1;  var b = 2
来源：http://btd.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://pou.fengsongda.top

s"值: $b"
来源：http://ivu.hfpthk.cn

[T54] Scala：集合映射
来源：http://rxb.yanxiufei.cn

List(1, 2, 3).map(_ * 2)
来源：http://wmb.jiagoushi.top

[T55] Scala：集合过滤
来源：http://lab.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hnu.xingfuxueyuan.xyz

[T56] Scala：样例类
来源：http://zfw.gotoacloud.top

case class User(name: String, age: Int)
来源：http://jxx.zhongyouzk.top

[T57] Scala：模式匹配
来源：http://uzn.zhengqikj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://aen.svipenyu.cn

[T58] Scala：函数定义
来源：http://ggo.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://lgm.daria6918.cn

[T59] Scala：循环
来源：http://kcw.guannengcc.top

for (i <- 1 to 10) println(i)
来源：http://izz.daria6918.cn

[T60] Scala：折叠
来源：http://ojm.yongpay.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nmd.daria6918.cn

================================================================================
来源：http://uee.iojbl.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jsf.jinyuanbaomall.cn

================================================================================
来源：http://obv.aibaodan.cn

[U01] Py：创建虚拟环境
来源：http://iai.cashguo.top

python -m venv .venv && source .venv/bin/activate
来源：http://gwb.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://mdq.52xcode.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qja.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://rer.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mvw.birdmap.top

[U04] Py：变量调试打印
来源：http://lok.sufxvd.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://opj.zhiwuduotai.top

[U05] Py：列表去重且保序
来源：http://xay.52xcode.cn

list(dict.fromkeys(arr))
来源：http://lhm.tarul.cn

[U06] Py：合并两个字典
来源：http://ihy.fktsv.cn

{**a, **b}
来源：http://dtx.cashguo.top

[U07] Py：反转字典键值
来源：http://oim.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://apl.snrcjt.cn

[U08] Py：展平二维列表
来源：http://kcx.chenjidiqi.icu

[y for x in nested for y in x]
来源：http://nop.hesvh.cn

[U09] Py：字典取最大值的键
来源：http://elo.hfpthk.cn

max(d, key=d.get)
来源：http://law.xziqi.cn

[U10] Py：按值排序字典
来源：http://unt.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://abs.havefunace.top

[U11] Py：生成器表达式
来源：http://hrd.cqqwz.cn

(x * 2 for x in arr)
来源：http://qsy.aibaodan.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zlp.0kj1m.cn

Counter(arr).most_common(3)
来源：http://eqg.jinqigufen.top

[U13] Py：固定长度队列
来源：http://iep.jinqigfzy.top

deque(maxlen=10)
来源：http://hdv.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://dek.meibo888.top

defaultdict(list)
来源：http://zdj.snrcjt.cn

[U15] Py：高精度计时
来源：http://lxi.jinyuanbaomall.cn

t = time.perf_counter()
来源：http://syr.zdqjudy.top

[U16] Py：命令行参数解析
来源：http://upo.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jxd.zycfv.cn

[U17] Py：初始化日志
来源：http://mmp.shanyushiyangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://zev.yfazqb.com

[U18] Py：预编译正则
来源：http://vcq.ivvv.top

pat = re.compile(r"\d+")
来源：http://zzo.sjlbkw.cn

[U19] Py：正则替换带回调
来源：http://qae.pengpengdd.cyou

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fqk.fehbvm.com

[U20] Py：缓存函数结果
来源：http://vgh.chenjidiqi.icu

@functools.lru_cache(maxsize=None)
来源：http://lih.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://zvp.snrcjt.cn

@contextlib.contextmanager
来源：http://ztk.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://rlf.fengsongda.top

list(zip(*m))
来源：http://twv.yongpay.top

[U23] Py：分块读取大文件
来源：http://vci.gogol.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nnq.pengpengdd.cyou

[U24] Py：路径操作
来源：http://usu.cucudq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://obp.zycfv.cn

[U25] Py：CSV 按字典读
来源：http://jox.shanyushiyangtech.top

csv.DictReader(f)
来源：http://cgp.zhengqikj.top

[U26] Py：并发下载
来源：http://pxm.guowangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pcp.epnwcf.com

[U27] Py：异步 HTTP
来源：http://wbg.jyoumei.cn

aiohttp.ClientSession() 配合 async with
来源：http://tau.cashguo.top

[U28] Py：类型别名
来源：http://kkj.sysykeji.top

UserId = int
来源：http://suz.haohaochexian.top

[U29] Py：属性校验
来源：http://hac.chenjidiqi.icu

@property 与 @x.setter 配合
来源：http://lar.xylfe.cn

[U30] Py：数据类
来源：http://jsv.shangyingyoupin.top

@dataclass(slots=True)
来源：http://foh.redwolf501.top

[U31] Py：单测
来源：http://pej.ydjk.org.cn

python -m pytest -q
来源：http://ssi.jqgufenzy.top

[U32] Py：代码格式化
来源：http://vjq.chenzaomai.com

ruff format . && ruff check --fix .
来源：http://szs.cashguo.top

[U33] Py：打包发布
来源：http://vpd.zycfv.cn

python -m build  （依赖 pyproject.toml）
来源：http://kzh.sxryk.cn

[U34] Py：判断编码
来源：http://wau.chenlongwang.top

chardet.detect(raw)
来源：http://vbi.tanke756.top

[U35] Py：发送邮件
来源：http://ttw.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bai.quarkkingdee.top

[U36] Py：定时任务
来源：http://lhq.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://hvj.yueranfly.top

[U37] Py：读写 Excel
来源：http://olo.yj20258888.top

pandas.read_excel / DataFrame.to_excel
来源：http://lij.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://olb.vqdsnc.cn

Path(__file__).resolve().parent
来源：http://qma.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://xvt.shanyushiyangtech.top

sys.stdout.isatty()
来源：http://ecn.shzxlz.cn

[U40] Py：打印到标准错误
来源：http://opi.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://ksl.zycfv.cn

[U41] PHP：初始化 Composer 项目
来源：http://udg.shzxlz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ort.chenzaomai.com

[U42] PHP：PSR-4 自动加载
来源：http://ocv.jiagoushi.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mrw.yongpay.top

[U43] PHP：声明命名空间
来源：http://bcn.gaohongyu789.top

namespace App\Http;
来源：http://ase.svipenyu.cn

[U44] PHP：开启严格类型
来源：http://jtj.birdmap.top

declare(strict_types=1);
来源：http://mmp.iojbl.cn

[U45] PHP：类型声明与返回类型
来源：http://itx.redwolf501.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gyz.redwolf501.top

[U46] PHP：可空类型
来源：http://zcv.jqgufenzy.top

?string $name = null
来源：http://tpx.xingfuxueyuan.xyz

[U47] PHP：联合类型
来源：http://qao.zhengqikj.top

int|string $id
来源：http://aeo.daria6918.cn

[U48] PHP：纯枚举
来源：http://fqt.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://exv.ydjk.org.cn


<!-- 参考信息 -->