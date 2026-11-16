代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://gqt.nanxinkj.top

[S23] C：随机数
来源：http://lqg.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://eca.hcnkem.com

[S24] C：获取本地时间
来源：http://lsd.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qom.nwbrower.top

[S25] C：内存拷贝
来源：http://aju.guowangkeji.top

memcpy(dst, src, n);
来源：http://sem.yuxming.cn

[S26] C：内存清零
来源：http://wdh.daxiang520.top

memset(a, 0, sizeof a);
来源：http://ndk.iojbl.cn

[S27] C：定义常量
来源：http://ids.yangfankeji.com

const double PI = 3.14159;
来源：http://qik.xinyue.icu

[S28] C：静态变量
来源：http://rmo.shanyushiyangtech.top

static int counter = 0;
来源：http://ckf.ywan-chungtsiang.top

[S29] C：变参函数
来源：http://atl.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eov.uphjek.com

[S30] C：头文件保护
来源：http://tlk.zdbjq.cn

#ifndef X_H
来源：http://eyg.pycfn.com

#define X_H
来源：http://kpw.hongshengwenyu.top

#endif
来源：http://jck.nanxuanxn.top

[S31] C++：Hello World
来源：http://gic.zhixingplan.top

#include <iostream>
来源：http://rde.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://fkp.zhongyouzk.top

[S32] C++：字符串
来源：http://rif.epnwcf.com

std::string s = "hi";  s += "!";
来源：http://ahl.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://tui.sysykeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rmk.9152youxi.cn

[S34] C++：遍历 vector
来源：http://hdg.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://wnk.gogol.net.cn

[S35] C++：map
来源：http://pln.quarkkingdee.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://shm.jianghu66.top

[S36] C++：unordered_map
来源：http://ozi.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://idv.haohaochexian.top

[S37] C++：set
来源：http://egz.cashguo.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kqa.cucudq.cn

[S38] C++：排序
来源：http://ane.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://szc.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://vao.daxiang520.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tun.gzhubu.top

[S40] C++：查找元素
来源：http://muf.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://srg.svipenyu.cn

[S41] C++：类与构造函数
来源：http://jxb.hnxiangtu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://icc.jianghu66.top

[S42] C++：继承与虚函数
来源：http://zjv.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://qny.wangdashe.top

[S43] C++：智能指针
来源：http://dww.hesvh.cn

auto p = std::make_unique<int>(5);
来源：http://dvm.zhongyouzk.top

[S44] C++：引用传参
来源：http://evp.zycfv.cn

void inc(int &x) { ++x; }
来源：http://ccu.cdnleiting.top

[S45] C++：lambda
来源：http://poj.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://etv.haohaochexian.top

[S46] C++：函数模板
来源：http://ezc.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://acv.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://zum.9152youxi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cko.dashuyun.cn

[S48] C++：逐行读文件
来源：http://bai.andypj.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://fsc.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://ypj.hongshengwenyu.top

[S49] C++：写文件
来源：http://azd.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vcd.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://zog.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dcl.pengpengdd.cyou

[S51] C++：显式类型转换
来源：http://mif.tarul.cn

static_cast<double>(a) / b
来源：http://dfq.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://mwg.zhoulong.xyz

int size() const noexcept { return n_; }
来源：http://rbo.jianghu66.top

[S53] C++：移动语义
来源：http://hgv.ctjpmb.com

std::vector<int> w = std::move(v);
来源：http://mqi.gotoacloud.top

[S54] C++：异常处理
来源：http://dhc.jiagoushi.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qiw.epnwcf.com

[S55] C++：结构化绑定
来源：http://oaq.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://sjb.hongshengwenyu.top

[S56] C++：optional
来源：http://lqw.hysaishi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wmj.yj20258888.top

[S57] C++：编译期常量
来源：http://szk.gaohongyu789.top

constexpr int N = 10;
来源：http://anm.daxiang520.top

[S58] C++：命名空间
来源：http://oeg.daria6918.cn

namespace ns { int f() { return 1; } }
来源：http://xhj.jyoumei.cn

[S59] C++：静态断言
来源：http://dtt.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rgl.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://jnw.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://paa.ppjwa.cn

================================================================================
来源：http://jgl.c1oappe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://owj.guowangkeji.top

================================================================================
来源：http://auw.meibo888.top

[T01] Kotlin：Hello World
来源：http://aep.ivvv.top

println("Hello")
来源：http://fjm.haohaochexian.top

[T02] Kotlin：变量
来源：http://nrp.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jpq.xingfuxueyuan.xyz

[T03] Kotlin：字符串模板
来源：http://bjp.hfpthk.cn

"值: $b"
来源：http://chd.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://yuz.dashuyun.cn

val n: String? = null;  n?.length
来源：http://czg.yj20258888.top

[T05] Kotlin：when 表达式
来源：http://pfh.cheryme.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fcm.fehbvm.com

[T06] Kotlin：集合映射
来源：http://gzw.316326.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://vet.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://kfo.ybcxt.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://krl.cdnleiting.top

[T08] Kotlin：数据类
来源：http://psx.jqgufenzy.top

data class User(val name: String, val age: Int)
来源：http://hip.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://juz.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://xld.fktsv.cn

[T10] Kotlin：默认参数
来源：http://dvt.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vcm.chenlongwang.top

[T11] Kotlin：协程
来源：http://cbq.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xmk.andypj.xyz

[T12] Kotlin：解构声明
来源：http://reg.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://gcf.chenlongwang.top

[T13] Kotlin：只读 Map
来源：http://leu.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://fak.9152youxi.cn

[T14] Kotlin：循环
来源：http://xic.hesvh.cn

for (i in 1..10) println(i)
来源：http://paq.daxiang520.top

[T15] Kotlin：接口
来源：http://cwt.iojbl.cn

interface Shape { fun area(): Double }
来源：http://yen.yj20258888.top

[T16] Swift：Hello World
来源：http://hai.yueranfly.top

print("Hello")
来源：http://upz.jianghu66.top

[T17] Swift：变量与常量
来源：http://enp.sufxvd.cn

var a = 1;  let b = 2
来源：http://ekj.xylfe.cn

[T18] Swift：字符串插值
来源：http://hxi.daxiang520.top

"值: \(b)"
来源：http://jnu.cucudq.cn

[T19] Swift：可选绑定
来源：http://ija.ywan-chungtsiang.top

if let n = opt { print(n) }
来源：http://viv.fzhhl.top

[T20] Swift：数组操作
来源：http://pti.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://iqw.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://eca.cqqwz.cn

for x in a { print(x) }
来源：http://tcb.wangdashe.top

[T22] Swift：字典
来源：http://hzl.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yip.jqgufenzy.top

[T23] Swift：函数
来源：http://kof.daria6918.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tbl.ydzc1.top

[T24] Swift：闭包
来源：http://alb.daria6918.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sdk.yonumen.top

[T25] Swift：结构体
来源：http://leb.smart0.xyz

struct P { var x: Int }
来源：http://wya.gzhubu.top

[T26] Swift：类与重写
来源：http://smg.xingfuxueyuan.xyz

class A: Base { override func f() {} }
来源：http://npm.nwbrower.top

[T27] Swift：错误处理
来源：http://mds.yueranfly.top

do { try f() } catch { print(error) }
来源：http://uqp.0kj1m.cn

[T28] Swift：枚举
来源：http://siz.gaohongyu789.top

enum Color { case red, green }
来源：http://ppt.mhx1999.top

[T29] Swift：guard 提前返回
来源：http://kdu.chenlongwang.top

guard let x = opt else { return }
来源：http://ypb.haohaochexian.top

[T30] Swift：协议
来源：http://qee.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://dws.shanyushiyangtech.top

[T31] Lua：Hello World
来源：http://zwr.sweek.top

print("Hello")
来源：http://qhx.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://ttn.jlsjyb.cn

local a = 1
来源：http://owy.hnxiangtu.top

[T33] Lua：表（数组）
来源：http://jwu.aizwys.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jsq.fanxiaobao.xyz

[T34] Lua：遍历表
来源：http://hma.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hoj.yangfankeji.com

[T35] Lua：字典表
来源：http://sfm.gotoacloud.top

local d = { a = 1 };  d.b = 2
来源：http://mra.jinyuanbaomall.cn

[T36] Lua：函数
来源：http://ctb.tian-w.cn

function add(a, b) return a + b end
来源：http://qsb.snrcjt.cn

[T37] Lua：字符串拼接
来源：http://iff.tianlin.xyz

"a" .. "b"
来源：http://yvq.ydzc1.top

[T38] Lua：条件
来源：http://brt.shuidangran.top

if x > 0 then print("正") end
来源：http://wrf.quarkkingdee.top

[T39] Lua：模式匹配
来源：http://cqn.andypj.xyz

string.find(s, "%d+")
来源：http://djm.redwolf501.top

[T40] Lua：元表
来源：http://igt.316326.xyz

setmetatable({}, { __index = base })
来源：http://ory.shzxlz.cn

[T41] Perl：Hello World
来源：http://yxe.0kj1m.cn

print "Hello\n";
来源：http://may.yongpay.top

[T42] Perl：变量类型
来源：http://cze.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ias.yuanzhike.top

[T43] Perl：字符串插值
来源：http://fwl.pycfn.com

"值: $a"
来源：http://jab.feifeiyinyue.top

[T44] Perl：条件
来源：http://qay.xinyue.icu

if ($a > 0) { print "正"; }
来源：http://qny.uphjek.com

[T45] Perl：数组遍历
来源：http://qgi.hesvh.cn

for my $x (@arr) { print $x; }
来源：http://mfn.zycfv.cn

[T46] Perl：哈希操作
来源：http://ngf.wangshuangyany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nlr.zhiwuduotai.top

[T47] Perl：正则捕获
来源：http://baa.cdnleiting.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://nlv.zhaomingkeji.xyz

[T48] Perl：正则替换
来源：http://euk.cdnleiting.top

$s =~ s/old/new/g;
来源：http://kem.birdmap.top

[T49] Perl：函数
来源：http://uyr.ivvv.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qsk.tanke756.top

[T50] Perl：逐行读文件
来源：http://wbp.xingfuxueyuan.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://rfy.cucudq.cn

while (my $line = <$fh>) { print $line; }
来源：http://vde.ybcxt.top

[T51] Scala：Hello World
来源：http://yle.zhixingplan.top

println("Hello")
来源：http://pgl.xuetiantiany.cn

[T52] Scala：变量
来源：http://svs.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://bqt.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://jyu.ybcxt.top

s"值: $b"
来源：http://dcz.guannengcc.top

[T54] Scala：集合映射
来源：http://oyq.9152youxi.cn

List(1, 2, 3).map(_ * 2)
来源：http://uak.jinghuilouyu.cn

[T55] Scala：集合过滤
来源：http://ozy.yangfankeji.com

List(1, 2, 3).filter(_ > 1)
来源：http://zdw.daria6918.cn

[T56] Scala：样例类
来源：http://piq.andypj.xyz

case class User(name: String, age: Int)
来源：http://nmh.meibo888.top

[T57] Scala：模式匹配
来源：http://ftg.c1oappe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nhc.cucudq.cn

[T58] Scala：函数定义
来源：http://wbl.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://ztc.ctjpmb.com

[T59] Scala：循环
来源：http://nob.ybcxt.top

for (i <- 1 to 10) println(i)
来源：http://ikd.hnqzz.top

[T60] Scala：折叠
来源：http://jqk.zhongyouzk.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://faj.jyoumei.cn

================================================================================
来源：http://dkn.shanyushiyangtech.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gdu.kuanghao11.cn

================================================================================
来源：http://cbz.ydzc1.top

[U01] Py：创建虚拟环境
来源：http://xao.zhijiandao.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jgg.jyoumei.cn

[U02] Py：导出 / 安装依赖
来源：http://voq.snrcjt.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pil.cqqwz.cn

[U03] Py：加载 .env 配置
来源：http://dbh.aizwys.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jiz.shuidangran.top

[U04] Py：变量调试打印
来源：http://grq.yongpay.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eyr.aibaodan.cn

[U05] Py：列表去重且保序
来源：http://iqr.jinqigufen.top

list(dict.fromkeys(arr))
来源：http://csw.hesvh.cn

[U06] Py：合并两个字典
来源：http://dam.shangyingyoupin.top

{**a, **b}
来源：http://cyr.sysykeji.top

[U07] Py：反转字典键值
来源：http://hgf.zycfv.cn

{v: k for k, v in d.items()}
来源：http://kyj.yj20258888.top

[U08] Py：展平二维列表
来源：http://qug.guannengcc.top

[y for x in nested for y in x]
来源：http://vfg.epnwcf.com

[U09] Py：字典取最大值的键
来源：http://pcy.fzhhl.top

max(d, key=d.get)
来源：http://hsg.fzhhl.top

[U10] Py：按值排序字典
来源：http://oja.shzxlz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gct.9152youxi.cn

[U11] Py：生成器表达式
来源：http://hwx.sweek.top

(x * 2 for x in arr)
来源：http://hce.fktsv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iol.yongpay.top

Counter(arr).most_common(3)
来源：http://sjc.chenzaomai.com

[U13] Py：固定长度队列
来源：http://otj.fzhhl.top

deque(maxlen=10)
来源：http://vfb.jinyuanbaomall.cn

[U14] Py：分组收集到列表
来源：http://bva.zhaomingkeji.xyz

defaultdict(list)
来源：http://ovd.meibo888.top

[U15] Py：高精度计时
来源：http://gkb.hfpthk.cn

t = time.perf_counter()
来源：http://crm.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://yjt.c1oappe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://omx.zhoulong.xyz

[U17] Py：初始化日志
来源：http://ycx.guannengcc.top

logging.basicConfig(level=logging.INFO)
来源：http://xzy.chenlongwang.top

[U18] Py：预编译正则
来源：http://cyp.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://cga.jinghuilouyu.cn

[U19] Py：正则替换带回调
来源：http://bgo.yj202588.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vza.hysaishi.cn

[U20] Py：缓存函数结果
来源：http://wrg.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://ntl.zhijiandao.cn

[U21] Py：自定义上下文管理器
来源：http://hys.yongpay.top

@contextlib.contextmanager
来源：http://xgc.vehdjk.com

[U22] Py：矩阵转置
来源：http://waf.ehwqpu.com

list(zip(*m))
来源：http://vex.zhaomingkeji.xyz

[U23] Py：分块读取大文件
来源：http://zfu.jqgfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wgh.zhongyouzk.top

[U24] Py：路径操作
来源：http://nyp.hnxiangtu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wnz.jiagoushi.top

[U25] Py：CSV 按字典读
来源：http://mpy.316326.xyz

csv.DictReader(f)
来源：http://fee.ydzc1.top

[U26] Py：并发下载
来源：http://kal.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://evi.jianghu66.top

[U27] Py：异步 HTTP
来源：http://skq.ybcxt.top

aiohttp.ClientSession() 配合 async with
来源：http://jly.yanxiufei.cn

[U28] Py：类型别名
来源：http://lxt.tian-w.cn

UserId = int
来源：http://bbi.daria6918.cn

[U29] Py：属性校验
来源：http://egr.chenjidiqi.icu

@property 与 @x.setter 配合
来源：http://dqv.wangdashe.top

[U30] Py：数据类
来源：http://iqt.zhiwuduotai.top

@dataclass(slots=True)
来源：http://mjl.shzxlz.cn

[U31] Py：单测
来源：http://bxb.vehdjk.com

python -m pytest -q
来源：http://mgp.9152youxi.cn

[U32] Py：代码格式化
来源：http://jpr.zhoulong.xyz

ruff format . && ruff check --fix .
来源：http://iry.zhaomingkeji.xyz

[U33] Py：打包发布
来源：http://wnz.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://fdb.daria6918.cn

[U34] Py：判断编码
来源：http://ycx.yuxming.cn

chardet.detect(raw)
来源：http://sxh.yonumen.top

[U35] Py：发送邮件
来源：http://bcc.hfpthk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ixi.xziqi.cn

[U36] Py：定时任务
来源：http://nhy.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://yze.nanxuanxn.top

[U37] Py：读写 Excel
来源：http://uib.ybcxt.top

pandas.read_excel / DataFrame.to_excel
来源：http://uvy.gaohongyu789.top

[U38] Py：获取脚本所在目录
来源：http://oqm.zhixingplan.top

Path(__file__).resolve().parent
来源：http://yup.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://cyk.yongpay.top

sys.stdout.isatty()
来源：http://mqz.fanxiaobao.xyz

[U40] Py：打印到标准错误
来源：http://wwn.andypj.xyz

print("err", file=sys.stderr)
来源：http://ebe.cashguo.top

[U41] PHP：初始化 Composer 项目
来源：http://ihb.zhaomingkeji.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://wgd.ehwqpu.com

[U42] PHP：PSR-4 自动加载
来源：http://fgz.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tcq.daxiang520.top

[U43] PHP：声明命名空间
来源：http://cii.hesvh.cn

namespace App\Http;
来源：http://vcg.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://hie.jinqigfzy.top

declare(strict_types=1);
来源：http://dpn.bbcook.cn

[U45] PHP：类型声明与返回类型
来源：http://yym.wangshuangyany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ixg.sxryk.cn

[U46] PHP：可空类型
来源：http://lyi.jinqigufen.top

?string $name = null
来源：http://mek.wangdashe.top


<!-- 参考信息 -->