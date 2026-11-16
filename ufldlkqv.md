代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cgp.zdbjq.cn

[S25] C：内存拷贝
来源：http://hps.pycfn.com

memcpy(dst, src, n);
来源：http://wju.gotoacloud.top

[S26] C：内存清零
来源：http://vdb.tianlin.xyz

memset(a, 0, sizeof a);
来源：http://bgg.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://mzi.snrcjt.cn

const double PI = 3.14159;
来源：http://ulq.dashuyun.cn

[S28] C：静态变量
来源：http://qku.yuanzhike.top

static int counter = 0;
来源：http://rlh.zhongyouzk.top

[S29] C：变参函数
来源：http://quw.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vck.haohaochexian.top

[S30] C：头文件保护
来源：http://esb.yfazqb.com

#ifndef X_H
来源：http://yyv.zhiwuduotai.top

#define X_H
来源：http://ewd.chenlongwang.top

#endif
来源：http://rqv.hysaishi.cn

[S31] C++：Hello World
来源：http://psw.chenlongwang.top

#include <iostream>
来源：http://khk.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://sfu.nanxinkj.top

[S32] C++：字符串
来源：http://uil.jianghu66.top

std::string s = "hi";  s += "!";
来源：http://ard.guannengcc.top

[S33] C++：vector 增删
来源：http://hwd.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://usk.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://hji.aizwys.cn

for (auto &x : v) { std::cout << x; }
来源：http://oyj.meibo888.top

[S35] C++：map
来源：http://ama.uphjek.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yae.xinyue.icu

[S36] C++：unordered_map
来源：http://vqn.jinqigufen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rsz.shanyushiyangkeji.top

[S37] C++：set
来源：http://nab.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uqn.fengsongda.top

[S38] C++：排序
来源：http://qxq.yonumen.top

std::sort(v.begin(), v.end());
来源：http://dud.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://gig.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://elb.tianlin.xyz

[S40] C++：查找元素
来源：http://aio.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mbm.guannengcc.top

[S41] C++：类与构造函数
来源：http://gca.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gre.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://kcl.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://xwo.xuetiantiany.cn

[S43] C++：智能指针
来源：http://dde.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://ryt.sysykeji.top

[S44] C++：引用传参
来源：http://bta.zhiwuduotai.top

void inc(int &x) { ++x; }
来源：http://gqf.yonumen.top

[S45] C++：lambda
来源：http://evj.sysykeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://hby.jianghu66.top

[S46] C++：函数模板
来源：http://zgj.xylfe.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hfj.cdnleiting.top

[S47] C++：结构化绑定遍历
来源：http://olo.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://omn.hesvh.cn

[S48] C++：逐行读文件
来源：http://xcy.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uim.zycfv.cn

while (std::getline(in, line)) { }
来源：http://dsz.meibo888.top

[S49] C++：写文件
来源：http://tmz.svipenyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ijw.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://rur.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xbq.zycfv.cn

[S51] C++：显式类型转换
来源：http://iba.zhixingplan.top

static_cast<double>(a) / b
来源：http://pud.jyoumei.cn

[S52] C++：const 与 noexcept
来源：http://rzz.xuanzx.com

int size() const noexcept { return n_; }
来源：http://lay.yj20258.top

[S53] C++：移动语义
来源：http://umc.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://udf.redwolf501.top

[S54] C++：异常处理
来源：http://nrn.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dku.epnwcf.com

[S55] C++：结构化绑定
来源：http://byq.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zsd.ydzc1.top

[S56] C++：optional
来源：http://ymj.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uif.yfazqb.com

[S57] C++：编译期常量
来源：http://vki.zhiwuduotai.top

constexpr int N = 10;
来源：http://ivl.uphjek.com

[S58] C++：命名空间
来源：http://gdl.sysykeji.top

namespace ns { int f() { return 1; } }
来源：http://hqn.nwbrower.top

[S59] C++：静态断言
来源：http://oiy.guowangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fvq.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://ile.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fbw.fzhhl.top

================================================================================
来源：http://wsi.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xmy.dianchejie.cn

================================================================================
来源：http://nal.yj20258888.top

[T01] Kotlin：Hello World
来源：http://jzp.havefunace.top

println("Hello")
来源：http://skp.hnxiangtu.top

[T02] Kotlin：变量
来源：http://bsb.aibaodan.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jha.sxryk.cn

[T03] Kotlin：字符串模板
来源：http://gql.yuxming.cn

"值: $b"
来源：http://pof.fktsv.cn

[T04] Kotlin：空安全
来源：http://baz.jinyuanbaomall.cn

val n: String? = null;  n?.length
来源：http://bfu.hongshengwenyu.top

[T05] Kotlin：when 表达式
来源：http://dqr.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://erg.jiagoushi.top

[T06] Kotlin：集合映射
来源：http://jih.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hfi.gaohongyu789.top

[T07] Kotlin：集合过滤
来源：http://iag.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://iyj.xinyue.icu

[T08] Kotlin：数据类
来源：http://aql.yj202588.top

data class User(val name: String, val age: Int)
来源：http://nwx.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://qph.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://kpr.hongshengwenyu.top

[T10] Kotlin：默认参数
来源：http://hwa.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ulv.zdqjudy.top

[T11] Kotlin：协程
来源：http://huv.jianghu66.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zjh.sysykeji.top

[T12] Kotlin：解构声明
来源：http://fwg.smart0.xyz

val (a, b) = Pair(1, 2)
来源：http://tco.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://ltj.hnxiangtu.top

val m = mapOf("a" to 1)
来源：http://ptc.yuxming.cn

[T14] Kotlin：循环
来源：http://ymh.aizwys.cn

for (i in 1..10) println(i)
来源：http://hwg.tian-w.cn

[T15] Kotlin：接口
来源：http://hzz.yj20258888.top

interface Shape { fun area(): Double }
来源：http://gec.jiagoushi.top

[T16] Swift：Hello World
来源：http://edb.cucudq.cn

print("Hello")
来源：http://vfe.aizwys.cn

[T17] Swift：变量与常量
来源：http://bzj.yuanzhike.top

var a = 1;  let b = 2
来源：http://tey.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://jqk.fktsv.cn

"值: \(b)"
来源：http://exa.guannengcc.top

[T19] Swift：可选绑定
来源：http://iki.vehdjk.com

if let n = opt { print(n) }
来源：http://net.cucudq.cn

[T20] Swift：数组操作
来源：http://oeh.birdmap.top

var a = [1, 2, 3];  a.append(4)
来源：http://rlk.yj20258888.top

[T21] Swift：遍历
来源：http://osw.fengsongda.top

for x in a { print(x) }
来源：http://igj.shuidangran.top

[T22] Swift：字典
来源：http://sil.yonumen.top

var d = ["a": 1];  d["b"] = 2
来源：http://btj.uphjek.com

[T23] Swift：函数
来源：http://dvx.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lgr.0kj1m.cn

[T24] Swift：闭包
来源：http://rac.jianghu66.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tfz.sufxvd.cn

[T25] Swift：结构体
来源：http://ovs.zdbjq.cn

struct P { var x: Int }
来源：http://qvm.jlsjyb.cn

[T26] Swift：类与重写
来源：http://qdw.sufxvd.cn

class A: Base { override func f() {} }
来源：http://fux.shzxlz.cn

[T27] Swift：错误处理
来源：http://zti.bbcook.cn

do { try f() } catch { print(error) }
来源：http://dad.xingfuxueyuan.xyz

[T28] Swift：枚举
来源：http://kip.tarul.cn

enum Color { case red, green }
来源：http://nfz.hcnkem.com

[T29] Swift：guard 提前返回
来源：http://ijb.xuetiantiany.cn

guard let x = opt else { return }
来源：http://dkc.ctjpmb.com

[T30] Swift：协议
来源：http://nqk.iojbl.cn

protocol Shape { func area() -> Double }
来源：http://aeu.nwbrower.top

[T31] Lua：Hello World
来源：http://glv.bbcook.cn

print("Hello")
来源：http://xct.aizwys.cn

[T32] Lua：局部变量
来源：http://ydg.zhiwuduotai.top

local a = 1
来源：http://rob.smart0.xyz

[T33] Lua：表（数组）
来源：http://zlb.hcnkem.com

local t = {1, 2, 3};  t[4] = 4
来源：http://wna.ydjk.org.cn

[T34] Lua：遍历表
来源：http://gqs.jiagoushi.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dwv.gogol.net.cn

[T35] Lua：字典表
来源：http://kvh.quarkkingdee.top

local d = { a = 1 };  d.b = 2
来源：http://dxf.hongshengwenyu.top

[T36] Lua：函数
来源：http://rls.hammf.cn

function add(a, b) return a + b end
来源：http://uje.jqgufenzy.top

[T37] Lua：字符串拼接
来源：http://pxj.sufxvd.cn

"a" .. "b"
来源：http://gkd.daxiang520.top

[T38] Lua：条件
来源：http://mut.hesvh.cn

if x > 0 then print("正") end
来源：http://sim.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://ikt.yueranfly.top

string.find(s, "%d+")
来源：http://ygu.xuanzx.com

[T40] Lua：元表
来源：http://lcs.jianghu66.top

setmetatable({}, { __index = base })
来源：http://gnx.hnqzz.top

[T41] Perl：Hello World
来源：http://mty.cucudq.cn

print "Hello\n";
来源：http://xgk.feifeiyinyue.top

[T42] Perl：变量类型
来源：http://ooj.52xcode.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://idi.yangfankeji.com

[T43] Perl：字符串插值
来源：http://hym.zycfv.cn

"值: $a"
来源：http://dkb.mhx1999.top

[T44] Perl：条件
来源：http://fyi.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://upj.nanxuanxn.top

[T45] Perl：数组遍历
来源：http://arz.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://jqd.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://jdv.yj20258.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vcq.svipenyu.cn

[T47] Perl：正则捕获
来源：http://nly.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://faw.mhx1999.top

[T48] Perl：正则替换
来源：http://kbg.mhx1999.top

$s =~ s/old/new/g;
来源：http://vnt.jqgufenzy.top

[T49] Perl：函数
来源：http://jqe.epnwcf.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ool.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://dfg.gzhubu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://git.fktsv.cn

while (my $line = <$fh>) { print $line; }
来源：http://agj.andypj.xyz

[T51] Scala：Hello World
来源：http://wzf.bbcook.cn

println("Hello")
来源：http://nwc.ydzc1.top

[T52] Scala：变量
来源：http://fol.hcnkem.com

val a = 1;  var b = 2
来源：http://xdj.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://ygi.hcnkem.com

s"值: $b"
来源：http://dhh.zhoulong.xyz

[T54] Scala：集合映射
来源：http://jet.cashguo.top

List(1, 2, 3).map(_ * 2)
来源：http://kmq.xuetiantiany.cn

[T55] Scala：集合过滤
来源：http://mmd.tianlin.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://zob.tarul.cn

[T56] Scala：样例类
来源：http://qpg.pycfn.com

case class User(name: String, age: Int)
来源：http://mki.mhx1999.top

[T57] Scala：模式匹配
来源：http://yyr.tarul.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uwe.kuanghao11.cn

[T58] Scala：函数定义
来源：http://kjc.shanyushiyangtech.top

def add(a: Int, b: Int): Int = a + b
来源：http://ltd.yvedp.cn

[T59] Scala：循环
来源：http://szh.wangdashe.top

for (i <- 1 to 10) println(i)
来源：http://bbv.ybcxt.top

[T60] Scala：折叠
来源：http://qnt.shuidangran.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fcm.epnwcf.com

================================================================================
来源：http://vxl.cdnleiting.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://czf.dashuyun.cn

================================================================================
来源：http://hej.redwolf501.top

[U01] Py：创建虚拟环境
来源：http://vsk.zdqjudy.top

python -m venv .venv && source .venv/bin/activate
来源：http://gqc.aizwys.cn

[U02] Py：导出 / 安装依赖
来源：http://fix.pengpengdd.cyou

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zic.jqgfzy.top

[U03] Py：加载 .env 配置
来源：http://iey.pengpengdd.cyou

from dotenv import load_dotenv; load_dotenv()
来源：http://jwb.daria6918.cn

[U04] Py：变量调试打印
来源：http://zgl.wangshuangyany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uai.c1oappe.top

[U05] Py：列表去重且保序
来源：http://qoq.shuidangran.top

list(dict.fromkeys(arr))
来源：http://vhz.ybcxt.top

[U06] Py：合并两个字典
来源：http://aqs.cqqwz.cn

{**a, **b}
来源：http://qik.zhengqikj.top

[U07] Py：反转字典键值
来源：http://fam.sxryk.cn

{v: k for k, v in d.items()}
来源：http://xpe.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://mpq.cashguo.top

[y for x in nested for y in x]
来源：http://eox.fzhhl.top

[U09] Py：字典取最大值的键
来源：http://tum.jqgufenzy.top

max(d, key=d.get)
来源：http://soj.svipenyu.cn

[U10] Py：按值排序字典
来源：http://eik.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zwg.jyoumei.cn

[U11] Py：生成器表达式
来源：http://oak.jiagoushi.top

(x * 2 for x in arr)
来源：http://fhl.zycfv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dde.zdbjq.cn

Counter(arr).most_common(3)
来源：http://tia.zhiwuduotai.top

[U13] Py：固定长度队列
来源：http://lrr.iojbl.cn

deque(maxlen=10)
来源：http://vok.uphjek.com

[U14] Py：分组收集到列表
来源：http://tho.tanke756.top

defaultdict(list)
来源：http://jvr.hammf.cn

[U15] Py：高精度计时
来源：http://xoy.fanxiaobao.xyz

t = time.perf_counter()
来源：http://ket.daxiang520.top

[U16] Py：命令行参数解析
来源：http://zpe.jyoumei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bko.pycfn.com

[U17] Py：初始化日志
来源：http://len.shanyushiyangtech.top

logging.basicConfig(level=logging.INFO)
来源：http://rpc.cashguo.top

[U18] Py：预编译正则
来源：http://xnc.0kj1m.cn

pat = re.compile(r"\d+")
来源：http://tba.ppjwa.cn

[U19] Py：正则替换带回调
来源：http://czb.ybcxt.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sba.fktsv.cn

[U20] Py：缓存函数结果
来源：http://hdb.aizwys.cn

@functools.lru_cache(maxsize=None)
来源：http://ybw.jinyuanbaomall.cn

[U21] Py：自定义上下文管理器
来源：http://yym.316326.xyz

@contextlib.contextmanager
来源：http://mfb.yj202588.top

[U22] Py：矩阵转置
来源：http://xmd.sxryk.cn

list(zip(*m))
来源：http://rkv.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://ygo.gzhubu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rfj.jianghu66.top

[U24] Py：路径操作
来源：http://jqa.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gpt.nwbrower.top

[U25] Py：CSV 按字典读
来源：http://nnh.cucudq.cn

csv.DictReader(f)
来源：http://qdu.pycfn.com

[U26] Py：并发下载
来源：http://xbb.cashguo.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hay.hfpthk.cn

[U27] Py：异步 HTTP
来源：http://ssi.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://pvk.bjfxy.top

[U28] Py：类型别名
来源：http://pga.yanxiufei.cn

UserId = int
来源：http://dpd.zhixingplan.top

[U29] Py：属性校验
来源：http://qtp.cdnleiting.top

@property 与 @x.setter 配合
来源：http://wzq.zdqjudy.top

[U30] Py：数据类
来源：http://hki.zhixingplan.top

@dataclass(slots=True)
来源：http://ktg.wangshuangyany.cn

[U31] Py：单测
来源：http://fmt.nwbrower.top

python -m pytest -q
来源：http://tzx.nanxuanxn.top

[U32] Py：代码格式化
来源：http://pjs.chenjidiqi.icu

ruff format . && ruff check --fix .
来源：http://aez.yj20258888.top

[U33] Py：打包发布
来源：http://ims.svipenyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://dsm.yonumen.top

[U34] Py：判断编码
来源：http://uvf.fanxiaobao.xyz

chardet.detect(raw)
来源：http://fac.cqqwz.cn

[U35] Py：发送邮件
来源：http://cyu.feifeiyinyue.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bdb.havefunace.top

[U36] Py：定时任务
来源：http://ubo.cdnleiting.top

schedule.every(10).minutes.do(job)
来源：http://ihg.cashguo.top

[U37] Py：读写 Excel
来源：http://hlm.smart0.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://rzp.shuidangran.top

[U38] Py：获取脚本所在目录
来源：http://hog.hfpthk.cn

Path(__file__).resolve().parent
来源：http://otc.xuetiantiany.cn

[U39] Py：判断是否在交互环境
来源：http://hwd.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://qtv.shuidangran.top

[U40] Py：打印到标准错误
来源：http://usx.yfazqb.com

print("err", file=sys.stderr)
来源：http://nfd.uphjek.com

[U41] PHP：初始化 Composer 项目
来源：http://mmk.ehwqpu.com

composer init;  composer require guzzlehttp/guzzle
来源：http://jfa.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://fpi.haohaochexian.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://maq.jinghuilouyu.cn

[U43] PHP：声明命名空间
来源：http://xzy.sweek.top

namespace App\Http;
来源：http://riy.kuanghao11.cn

[U44] PHP：开启严格类型
来源：http://iwl.shzxlz.cn

declare(strict_types=1);
来源：http://cad.chenjidiqi.icu

[U45] PHP：类型声明与返回类型
来源：http://srv.yuanzhike.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://bun.svipenyu.cn

[U46] PHP：可空类型
来源：http://ezg.svipenyu.cn

?string $name = null
来源：http://nss.yanxiufei.cn

[U47] PHP：联合类型
来源：http://dpz.316326.xyz

int|string $id
来源：http://xfu.meibo888.top

[U48] PHP：纯枚举
来源：http://yaa.meibo888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rui.ybcxt.top


<!-- 参考信息 -->