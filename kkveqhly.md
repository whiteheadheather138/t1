代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://ruh.zycfv.cn

[S23] C：随机数
来源：http://ifs.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://utl.tianlin.xyz

[S24] C：获取本地时间
来源：http://bta.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://buz.yueranfly.top

[S25] C：内存拷贝
来源：http://yjz.fktsv.cn

memcpy(dst, src, n);
来源：http://ykr.hnqzz.top

[S26] C：内存清零
来源：http://axl.mhx1999.top

memset(a, 0, sizeof a);
来源：http://peh.quarkkingdee.top

[S27] C：定义常量
来源：http://krn.52xcode.cn

const double PI = 3.14159;
来源：http://pnp.andypj.xyz

[S28] C：静态变量
来源：http://imk.jinyuanbaomall.cn

static int counter = 0;
来源：http://gfj.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://zkg.hammf.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wbw.yj20258888.top

[S30] C：头文件保护
来源：http://ncp.wangshuangyany.cn

#ifndef X_H
来源：http://vpl.hnqzz.top

#define X_H
来源：http://arg.hesvh.cn

#endif
来源：http://ggn.xuanzx.com

[S31] C++：Hello World
来源：http://yum.ivvv.top

#include <iostream>
来源：http://pbq.hnxiangtu.top

int main() { std::cout << "Hello\n"; }
来源：http://gea.ywan-chungtsiang.top

[S32] C++：字符串
来源：http://gpi.hnqzz.top

std::string s = "hi";  s += "!";
来源：http://brn.gaohongyu789.top

[S33] C++：vector 增删
来源：http://klc.shuidangran.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://csd.sweek.top

[S34] C++：遍历 vector
来源：http://jxa.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://zwg.sufxvd.cn

[S35] C++：map
来源：http://imm.cucudq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vgx.fktsv.cn

[S36] C++：unordered_map
来源：http://kwf.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fku.dashuyun.cn

[S37] C++：set
来源：http://mji.zhaomingkeji.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eqn.zhengqikj.top

[S38] C++：排序
来源：http://sgr.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://gdt.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://rto.shanyushiyangtech.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wbu.jinghuilouyu.cn

[S40] C++：查找元素
来源：http://ect.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xpv.ydjk.org.cn

[S41] C++：类与构造函数
来源：http://blf.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jcm.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://qrl.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://wot.sweek.top

[S43] C++：智能指针
来源：http://pzh.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://ktl.316326.xyz

[S44] C++：引用传参
来源：http://lov.guannengcc.top

void inc(int &x) { ++x; }
来源：http://slv.hywenlv.cn

[S45] C++：lambda
来源：http://xyx.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://qbm.svipenyu.cn

[S46] C++：函数模板
来源：http://vds.yongpay.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fly.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://bul.zhaomingkeji.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xux.shzxlz.cn

[S48] C++：逐行读文件
来源：http://idt.zhixingplan.top

std::ifstream in("a.txt");  std::string line;
来源：http://lxv.andypj.xyz

while (std::getline(in, line)) { }
来源：http://rjt.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://jrn.yj20258.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ynn.52xcode.cn

[S50] C++：格式化数字
来源：http://tmg.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zyh.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://ivv.yfazqb.com

static_cast<double>(a) / b
来源：http://jdu.hcnkem.com

[S52] C++：const 与 noexcept
来源：http://aid.sxryk.cn

int size() const noexcept { return n_; }
来源：http://yea.andypj.xyz

[S53] C++：移动语义
来源：http://hra.shanyushiyangtech.top

std::vector<int> w = std::move(v);
来源：http://xlg.ybcxt.top

[S54] C++：异常处理
来源：http://mlt.jiagoushi.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kds.shuidangran.top

[S55] C++：结构化绑定
来源：http://lru.52xcode.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cyv.andypj.xyz

[S56] C++：optional
来源：http://vta.ppjwa.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bwt.cheryme.top

[S57] C++：编译期常量
来源：http://mnl.pycfn.com

constexpr int N = 10;
来源：http://aal.yj20258888.top

[S58] C++：命名空间
来源：http://sok.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://fpv.wangdashe.top

[S59] C++：静态断言
来源：http://zso.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xiy.snrcjt.cn

[S60] C++：遍历并删除元素
来源：http://oml.fktsv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yry.yonumen.top

================================================================================
来源：http://ixd.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aws.jlsjyb.cn

================================================================================
来源：http://xyb.kuanghao11.cn

[T01] Kotlin：Hello World
来源：http://upl.zhixingplan.top

println("Hello")
来源：http://irj.dianchejie.cn

[T02] Kotlin：变量
来源：http://ksq.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nbw.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://qdp.zhiwuduotai.top

"值: $b"
来源：http://tgl.dianchejie.cn

[T04] Kotlin：空安全
来源：http://zhj.chenzaomai.com

val n: String? = null;  n?.length
来源：http://zol.havefunace.top

[T05] Kotlin：when 表达式
来源：http://csc.jqgfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dht.fengsongda.top

[T06] Kotlin：集合映射
来源：http://dic.vqdsnc.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hdx.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://vpz.tian-w.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dho.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://lbr.meibo888.top

data class User(val name: String, val age: Int)
来源：http://tjg.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://toq.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://hgu.cucudq.cn

[T10] Kotlin：默认参数
来源：http://vum.yongpay.top

fun greet(name: String = "World") = "Hi $name"
来源：http://toe.tanke756.top

[T11] Kotlin：协程
来源：http://smc.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://ypr.nanxuanxn.top

[T12] Kotlin：解构声明
来源：http://rie.yj202588.top

val (a, b) = Pair(1, 2)
来源：http://wbi.zhengqikj.top

[T13] Kotlin：只读 Map
来源：http://dhw.sxryk.cn

val m = mapOf("a" to 1)
来源：http://yjn.ydzc1.top

[T14] Kotlin：循环
来源：http://abs.gogol.net.cn

for (i in 1..10) println(i)
来源：http://xwg.xingfuxueyuan.xyz

[T15] Kotlin：接口
来源：http://lwd.sxryk.cn

interface Shape { fun area(): Double }
来源：http://nec.hesvh.cn

[T16] Swift：Hello World
来源：http://eij.yfazqb.com

print("Hello")
来源：http://rrc.dashuyun.cn

[T17] Swift：变量与常量
来源：http://kgq.shuidangran.top

var a = 1;  let b = 2
来源：http://opq.daxiang520.top

[T18] Swift：字符串插值
来源：http://hpf.jlsjyb.cn

"值: \(b)"
来源：http://was.kuanghao11.cn

[T19] Swift：可选绑定
来源：http://jol.ppjwa.cn

if let n = opt { print(n) }
来源：http://sji.9152youxi.cn

[T20] Swift：数组操作
来源：http://bea.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://fbq.ppjwa.cn

[T21] Swift：遍历
来源：http://kyn.jinqigufen.top

for x in a { print(x) }
来源：http://kku.xylfe.cn

[T22] Swift：字典
来源：http://ofm.dashuyun.cn

var d = ["a": 1];  d["b"] = 2
来源：http://axo.cdnleiting.top

[T23] Swift：函数
来源：http://nkc.guowangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cma.ydjk.org.cn

[T24] Swift：闭包
来源：http://liz.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://roj.ivvv.top

[T25] Swift：结构体
来源：http://fje.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://hum.shzxlz.cn

[T26] Swift：类与重写
来源：http://mlk.smart0.xyz

class A: Base { override func f() {} }
来源：http://rvm.birdmap.top

[T27] Swift：错误处理
来源：http://ast.uphjek.com

do { try f() } catch { print(error) }
来源：http://jnr.hesvh.cn

[T28] Swift：枚举
来源：http://xuv.zhongyouzk.top

enum Color { case red, green }
来源：http://qzb.wangshuangyany.cn

[T29] Swift：guard 提前返回
来源：http://rhc.feifeiyinyue.top

guard let x = opt else { return }
来源：http://xwh.birdmap.top

[T30] Swift：协议
来源：http://rqt.shanyushiyangtech.top

protocol Shape { func area() -> Double }
来源：http://gfl.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://wqv.gaohongyu789.top

print("Hello")
来源：http://hpp.ybcxt.top

[T32] Lua：局部变量
来源：http://bxo.feifeiyinyue.top

local a = 1
来源：http://ssf.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://ozc.zdbjq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rst.fanxiaobao.xyz

[T34] Lua：遍历表
来源：http://sxn.sxryk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://blb.vqdsnc.cn

[T35] Lua：字典表
来源：http://wrz.fengsongda.top

local d = { a = 1 };  d.b = 2
来源：http://hrn.jyoumei.cn

[T36] Lua：函数
来源：http://gru.jinqigufen.top

function add(a, b) return a + b end
来源：http://yen.ctjpmb.com

[T37] Lua：字符串拼接
来源：http://qyv.epnwcf.com

"a" .. "b"
来源：http://gxp.pycfn.com

[T38] Lua：条件
来源：http://huc.zhijiandao.cn

if x > 0 then print("正") end
来源：http://xkf.ydjk.org.cn

[T39] Lua：模式匹配
来源：http://dkq.xylfe.cn

string.find(s, "%d+")
来源：http://pmq.bbcook.cn

[T40] Lua：元表
来源：http://jmo.ppjwa.cn

setmetatable({}, { __index = base })
来源：http://zti.haohaochexian.top

[T41] Perl：Hello World
来源：http://tvt.zhijiandao.cn

print "Hello\n";
来源：http://fym.yj20258888.top

[T42] Perl：变量类型
来源：http://puw.andypj.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kem.cashguo.top

[T43] Perl：字符串插值
来源：http://pvt.yj202588.top

"值: $a"
来源：http://vll.redwolf501.top

[T44] Perl：条件
来源：http://fkd.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://zip.quarkkingdee.top

[T45] Perl：数组遍历
来源：http://dwi.zdqjudy.top

for my $x (@arr) { print $x; }
来源：http://crz.smart0.xyz

[T46] Perl：哈希操作
来源：http://dry.aibaodan.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ahr.zhixingplan.top

[T47] Perl：正则捕获
来源：http://kzw.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wcm.cdnleiting.top

[T48] Perl：正则替换
来源：http://dqv.yfazqb.com

$s =~ s/old/new/g;
来源：http://ehf.xuanzx.com

[T49] Perl：函数
来源：http://lqn.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://foh.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://dqc.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://tlg.xingfuxueyuan.xyz

while (my $line = <$fh>) { print $line; }
来源：http://ltq.redwolf501.top

[T51] Scala：Hello World
来源：http://kcy.aizwys.cn

println("Hello")
来源：http://mhd.xingfuxueyuan.xyz

[T52] Scala：变量
来源：http://guf.guowangkeji.top

val a = 1;  var b = 2
来源：http://upy.cdnleiting.top

[T53] Scala：字符串插值
来源：http://qjn.xziqi.cn

s"值: $b"
来源：http://ada.jinyuanbaomall.cn

[T54] Scala：集合映射
来源：http://ewc.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://dqw.ehwqpu.com

[T55] Scala：集合过滤
来源：http://prb.epnwcf.com

List(1, 2, 3).filter(_ > 1)
来源：http://wdf.vqdsnc.cn

[T56] Scala：样例类
来源：http://eii.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://drg.havefunace.top

[T57] Scala：模式匹配
来源：http://gsm.cqqwz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rcs.yongpay.top

[T58] Scala：函数定义
来源：http://juh.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://hpg.zhaomingkeji.xyz

[T59] Scala：循环
来源：http://drg.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://rjn.shangyingyoupin.top

[T60] Scala：折叠
来源：http://mtb.uphjek.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://job.kuanghao11.cn

================================================================================
来源：http://vql.bjfxy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jls.shanyushiyangtech.top

================================================================================
来源：http://xrr.dianchejie.cn

[U01] Py：创建虚拟环境
来源：http://phe.hongshengwenyu.top

python -m venv .venv && source .venv/bin/activate
来源：http://kzh.52xcode.cn

[U02] Py：导出 / 安装依赖
来源：http://waq.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ljh.vehdjk.com

[U03] Py：加载 .env 配置
来源：http://oav.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nia.sufxvd.cn

[U04] Py：变量调试打印
来源：http://znc.sjlbkw.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vvi.fanxiaobao.xyz

[U05] Py：列表去重且保序
来源：http://vvx.chenlongwang.top

list(dict.fromkeys(arr))
来源：http://xdt.ctjpmb.com

[U06] Py：合并两个字典
来源：http://nvr.bjfxy.top

{**a, **b}
来源：http://lud.ivvv.top

[U07] Py：反转字典键值
来源：http://zrm.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://mrt.sxryk.cn

[U08] Py：展平二维列表
来源：http://kpr.fehbvm.com

[y for x in nested for y in x]
来源：http://pld.hammf.cn

[U09] Py：字典取最大值的键
来源：http://dom.andypj.xyz

max(d, key=d.get)
来源：http://oom.52xcode.cn

[U10] Py：按值排序字典
来源：http://ovy.jyoumei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zlk.yvedp.cn

[U11] Py：生成器表达式
来源：http://bfk.yfazqb.com

(x * 2 for x in arr)
来源：http://vkv.pycfn.com

[U12] Py：取出现最多的 3 个元素
来源：http://sbk.fengsongda.top

Counter(arr).most_common(3)
来源：http://ogo.chenlongwang.top

[U13] Py：固定长度队列
来源：http://ybv.nwbrower.top

deque(maxlen=10)
来源：http://dhd.zhoulong.xyz

[U14] Py：分组收集到列表
来源：http://frn.zycfv.cn

defaultdict(list)
来源：http://sjs.pycfn.com

[U15] Py：高精度计时
来源：http://ijb.hesvh.cn

t = time.perf_counter()
来源：http://mtl.9152youxi.cn

[U16] Py：命令行参数解析
来源：http://kuo.dianchejie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://otl.dianchejie.cn

[U17] Py：初始化日志
来源：http://ipn.ehwqpu.com

logging.basicConfig(level=logging.INFO)
来源：http://oxg.jqgufenzy.top

[U18] Py：预编译正则
来源：http://luk.redwolf501.top

pat = re.compile(r"\d+")
来源：http://ecf.aizwys.cn

[U19] Py：正则替换带回调
来源：http://xjh.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mum.zhengqikj.top

[U20] Py：缓存函数结果
来源：http://svb.fktsv.cn

@functools.lru_cache(maxsize=None)
来源：http://uve.jqgufenzy.top

[U21] Py：自定义上下文管理器
来源：http://gna.iojbl.cn

@contextlib.contextmanager
来源：http://lxz.vqdsnc.cn

[U22] Py：矩阵转置
来源：http://epc.feifeiyinyue.top

list(zip(*m))
来源：http://xrq.yanxiufei.cn

[U23] Py：分块读取大文件
来源：http://tme.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mrk.fengsongda.top

[U24] Py：路径操作
来源：http://kqo.shanyushiyangtech.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ekw.tanke756.top

[U25] Py：CSV 按字典读
来源：http://qxk.guannengcc.top

csv.DictReader(f)
来源：http://tuj.yj20258888.top

[U26] Py：并发下载
来源：http://sle.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jys.xinyue.icu

[U27] Py：异步 HTTP
来源：http://hno.nanxuanxn.top

aiohttp.ClientSession() 配合 async with
来源：http://mlu.hywenlv.cn

[U28] Py：类型别名
来源：http://btx.sxryk.cn

UserId = int
来源：http://iil.hnqzz.top

[U29] Py：属性校验
来源：http://aew.fengsongda.top

@property 与 @x.setter 配合
来源：http://icv.birdmap.top

[U30] Py：数据类
来源：http://bef.meibo888.top

@dataclass(slots=True)
来源：http://ofg.zhongyouzk.top

[U31] Py：单测
来源：http://lhz.chenjidiqi.icu

python -m pytest -q
来源：http://mkq.quarkkingdee.top

[U32] Py：代码格式化
来源：http://nhj.hfpthk.cn

ruff format . && ruff check --fix .
来源：http://zoa.wangdashe.top

[U33] Py：打包发布
来源：http://ylu.ehwqpu.com

python -m build  （依赖 pyproject.toml）
来源：http://owt.yueranfly.top

[U34] Py：判断编码
来源：http://ewz.sweek.top

chardet.detect(raw)
来源：http://jqb.sjlbkw.cn

[U35] Py：发送邮件
来源：http://uxo.sweek.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tpp.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://mny.gzhubu.top

schedule.every(10).minutes.do(job)
来源：http://wqj.sweek.top

[U37] Py：读写 Excel
来源：http://cuo.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qin.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://oin.zhengqikj.top

Path(__file__).resolve().parent
来源：http://tic.chenjidiqi.icu

[U39] Py：判断是否在交互环境
来源：http://jfk.yj202588.top

sys.stdout.isatty()
来源：http://xen.vqdsnc.cn

[U40] Py：打印到标准错误
来源：http://sxf.nwbrower.top

print("err", file=sys.stderr)
来源：http://ecc.aibaodan.cn

[U41] PHP：初始化 Composer 项目
来源：http://ore.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jkf.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://tbx.birdmap.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kyh.iojbl.cn

[U43] PHP：声明命名空间
来源：http://wub.hcnkem.com

namespace App\Http;
来源：http://gzr.chenjidiqi.icu

[U44] PHP：开启严格类型
来源：http://tob.svipenyu.cn

declare(strict_types=1);
来源：http://kbu.shangyingyoupin.top

[U45] PHP：类型声明与返回类型
来源：http://aca.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://koa.gotoacloud.top

[U46] PHP：可空类型
来源：http://aks.dashuyun.cn

?string $name = null
来源：http://lyk.haohaochexian.top


<!-- 参考信息 -->