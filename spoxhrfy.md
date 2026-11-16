代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://tuv.yangfankeji.com

[S23] C：随机数
来源：http://fmx.chenjidiqi.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://npi.sjlbkw.cn

[S24] C：获取本地时间
来源：http://iyo.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mff.zhijiandao.cn

[S25] C：内存拷贝
来源：http://rwz.andypj.xyz

memcpy(dst, src, n);
来源：http://snw.ivvv.top

[S26] C：内存清零
来源：http://gkg.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://jdz.zhoulong.xyz

[S27] C：定义常量
来源：http://xbe.hongshengwenyu.top

const double PI = 3.14159;
来源：http://tbv.tarul.cn

[S28] C：静态变量
来源：http://lmi.ydjk.org.cn

static int counter = 0;
来源：http://jic.birdmap.top

[S29] C：变参函数
来源：http://qyp.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wca.nwbrower.top

[S30] C：头文件保护
来源：http://pik.cheryme.top

#ifndef X_H
来源：http://hcs.aibaodan.cn

#define X_H
来源：http://bqx.havefunace.top

#endif
来源：http://cso.xuetiantiany.cn

[S31] C++：Hello World
来源：http://lks.xingfuxueyuan.xyz

#include <iostream>
来源：http://jwv.ppjwa.cn

int main() { std::cout << "Hello\n"; }
来源：http://dga.9152youxi.cn

[S32] C++：字符串
来源：http://gpi.epnwcf.com

std::string s = "hi";  s += "!";
来源：http://bbb.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://tcw.xinyue.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mlb.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://txm.fengsongda.top

for (auto &x : v) { std::cout << x; }
来源：http://tzk.aibaodan.cn

[S35] C++：map
来源：http://emi.c1oappe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tpf.fanxiaobao.xyz

[S36] C++：unordered_map
来源：http://hkj.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xkc.quarkkingdee.top

[S37] C++：set
来源：http://nsp.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dvh.fanxiaobao.xyz

[S38] C++：排序
来源：http://shc.pengpengdd.cyou

std::sort(v.begin(), v.end());
来源：http://acq.fengsongda.top

[S39] C++：自定义比较器排序
来源：http://uwg.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uhu.ivvv.top

[S40] C++：查找元素
来源：http://skj.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wvz.cucudq.cn

[S41] C++：类与构造函数
来源：http://rln.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zzc.zhijiandao.cn

[S42] C++：继承与虚函数
来源：http://lof.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://lqg.daria6918.cn

[S43] C++：智能指针
来源：http://vzy.xingfuxueyuan.xyz

auto p = std::make_unique<int>(5);
来源：http://qre.yangfankeji.com

[S44] C++：引用传参
来源：http://rku.guannengcc.top

void inc(int &x) { ++x; }
来源：http://ahz.shzxlz.cn

[S45] C++：lambda
来源：http://qxn.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vmt.jinqigfzy.top

[S46] C++：函数模板
来源：http://sfm.jinqigfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vkj.sysykeji.top

[S47] C++：结构化绑定遍历
来源：http://qme.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vko.uphjek.com

[S48] C++：逐行读文件
来源：http://hmv.shuidangran.top

std::ifstream in("a.txt");  std::string line;
来源：http://iko.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://hzt.zhoulong.xyz

[S49] C++：写文件
来源：http://bzt.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eok.tanke756.top

[S50] C++：格式化数字
来源：http://zbn.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fjv.chenjidiqi.icu

[S51] C++：显式类型转换
来源：http://lwm.jqgfzy.top

static_cast<double>(a) / b
来源：http://ruc.ppjwa.cn

[S52] C++：const 与 noexcept
来源：http://lsb.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://obk.jinqigfzy.top

[S53] C++：移动语义
来源：http://ynk.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://ybb.gogol.net.cn

[S54] C++：异常处理
来源：http://tbc.andypj.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mnl.sjlbkw.cn

[S55] C++：结构化绑定
来源：http://bnv.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cqd.shanyushiyangtech.top

[S56] C++：optional
来源：http://kbw.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://orf.pycfn.com

[S57] C++：编译期常量
来源：http://iga.jlsjyb.cn

constexpr int N = 10;
来源：http://sfu.9152youxi.cn

[S58] C++：命名空间
来源：http://mhp.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://xml.snrcjt.cn

[S59] C++：静态断言
来源：http://nkt.ydzc1.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ocm.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://tvy.tanke756.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://scy.fktsv.cn

================================================================================
来源：http://wxl.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vzn.guowangkeji.top

================================================================================
来源：http://xor.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://qri.vehdjk.com

println("Hello")
来源：http://fls.xingfuxueyuan.xyz

[T02] Kotlin：变量
来源：http://qfz.tian-w.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bpy.jqgfzy.top

[T03] Kotlin：字符串模板
来源：http://dal.hongshengwenyu.top

"值: $b"
来源：http://wts.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://gjn.daria6918.cn

val n: String? = null;  n?.length
来源：http://oub.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://thr.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jvj.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://zio.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pac.cashguo.top

[T07] Kotlin：集合过滤
来源：http://jwe.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hbi.iojbl.cn

[T08] Kotlin：数据类
来源：http://uax.chenzaomai.com

data class User(val name: String, val age: Int)
来源：http://jvb.iojbl.cn

[T09] Kotlin：扩展函数
来源：http://ptv.jqgufenzy.top

fun String.exclaim() = this + "!"
来源：http://fqd.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://cbw.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dwx.nanxinkj.top

[T11] Kotlin：协程
来源：http://kej.tian-w.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ddp.shzxlz.cn

[T12] Kotlin：解构声明
来源：http://gnc.redwolf501.top

val (a, b) = Pair(1, 2)
来源：http://uao.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://hmw.fzhhl.top

val m = mapOf("a" to 1)
来源：http://aol.sxryk.cn

[T14] Kotlin：循环
来源：http://xbu.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://vdh.yj202588.top

[T15] Kotlin：接口
来源：http://jcc.yongpay.top

interface Shape { fun area(): Double }
来源：http://nlh.guowangkeji.top

[T16] Swift：Hello World
来源：http://zkv.gzhubu.top

print("Hello")
来源：http://trq.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://cgg.tianlin.xyz

var a = 1;  let b = 2
来源：http://puv.hammf.cn

[T18] Swift：字符串插值
来源：http://xne.chenzaomai.com

"值: \(b)"
来源：http://apb.aizwys.cn

[T19] Swift：可选绑定
来源：http://tnd.jiagoushi.top

if let n = opt { print(n) }
来源：http://fue.ydjk.org.cn

[T20] Swift：数组操作
来源：http://cnr.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://num.sxryk.cn

[T21] Swift：遍历
来源：http://imr.tian-w.cn

for x in a { print(x) }
来源：http://vax.hnqzz.top

[T22] Swift：字典
来源：http://lbk.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://hvh.guannengcc.top

[T23] Swift：函数
来源：http://bcw.zycfv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fwu.hnqzz.top

[T24] Swift：闭包
来源：http://quc.kuanghao11.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ugq.chenzaomai.com

[T25] Swift：结构体
来源：http://gtl.shanyushiyangtech.top

struct P { var x: Int }
来源：http://bzj.daria6918.cn

[T26] Swift：类与重写
来源：http://cgs.sysykeji.top

class A: Base { override func f() {} }
来源：http://pup.hcnkem.com

[T27] Swift：错误处理
来源：http://ejq.shangyingyoupin.top

do { try f() } catch { print(error) }
来源：http://pes.hammf.cn

[T28] Swift：枚举
来源：http://aei.jinghuilouyu.cn

enum Color { case red, green }
来源：http://kpr.tian-w.cn

[T29] Swift：guard 提前返回
来源：http://oky.jinqigfzy.top

guard let x = opt else { return }
来源：http://lmv.uphjek.com

[T30] Swift：协议
来源：http://uzf.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://ija.hfpthk.cn

[T31] Lua：Hello World
来源：http://chw.xuanzx.com

print("Hello")
来源：http://ilx.iojbl.cn

[T32] Lua：局部变量
来源：http://jrj.dashuyun.cn

local a = 1
来源：http://rkq.pengpengdd.cyou

[T33] Lua：表（数组）
来源：http://ghh.xingfuxueyuan.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://jsd.ehwqpu.com

[T34] Lua：遍历表
来源：http://dsh.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sqy.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://vse.ivvv.top

local d = { a = 1 };  d.b = 2
来源：http://vkp.jinghuilouyu.cn

[T36] Lua：函数
来源：http://yjr.ctjpmb.com

function add(a, b) return a + b end
来源：http://toh.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://vjf.hfpthk.cn

"a" .. "b"
来源：http://spq.jinqigfzy.top

[T38] Lua：条件
来源：http://eav.havefunace.top

if x > 0 then print("正") end
来源：http://rad.sweek.top

[T39] Lua：模式匹配
来源：http://syi.sweek.top

string.find(s, "%d+")
来源：http://rwk.ydzc1.top

[T40] Lua：元表
来源：http://aww.nanxinkj.top

setmetatable({}, { __index = base })
来源：http://wsk.cqqwz.cn

[T41] Perl：Hello World
来源：http://dld.haohaochexian.top

print "Hello\n";
来源：http://ggv.yanxiufei.cn

[T42] Perl：变量类型
来源：http://ovg.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bqc.yj20258.top

[T43] Perl：字符串插值
来源：http://xha.mhx1999.top

"值: $a"
来源：http://ibw.zhiwuduotai.top

[T44] Perl：条件
来源：http://ycl.zhiwuduotai.top

if ($a > 0) { print "正"; }
来源：http://moo.yueranfly.top

[T45] Perl：数组遍历
来源：http://dde.sufxvd.cn

for my $x (@arr) { print $x; }
来源：http://rmy.nanxuanxn.top

[T46] Perl：哈希操作
来源：http://cvz.9152youxi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pvf.52xcode.cn

[T47] Perl：正则捕获
来源：http://hru.yj20258.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://djo.aibaodan.cn

[T48] Perl：正则替换
来源：http://qvi.tanke756.top

$s =~ s/old/new/g;
来源：http://ffc.yuxming.cn

[T49] Perl：函数
来源：http://lqa.zhiwuduotai.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://izg.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://yhn.hnqzz.top

open my $fh, "<", "a.txt" or die $!;
来源：http://swq.jinyuanbaomall.cn

while (my $line = <$fh>) { print $line; }
来源：http://pzg.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://kec.gaohongyu789.top

println("Hello")
来源：http://ouq.yj20258888.top

[T52] Scala：变量
来源：http://lbg.yfazqb.com

val a = 1;  var b = 2
来源：http://vvr.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://pau.zdbjq.cn

s"值: $b"
来源：http://uoh.xinyue.icu

[T54] Scala：集合映射
来源：http://dau.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://uif.hesvh.cn

[T55] Scala：集合过滤
来源：http://elr.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://yai.haohaochexian.top

[T56] Scala：样例类
来源：http://fyc.daria6918.cn

case class User(name: String, age: Int)
来源：http://dmu.epnwcf.com

[T57] Scala：模式匹配
来源：http://kie.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jgz.ywan-chungtsiang.top

[T58] Scala：函数定义
来源：http://ivg.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hhp.feifeiyinyue.top

[T59] Scala：循环
来源：http://jcb.xziqi.cn

for (i <- 1 to 10) println(i)
来源：http://ohv.sxryk.cn

[T60] Scala：折叠
来源：http://fhq.tarul.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ocl.cashguo.top

================================================================================
来源：http://agh.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kse.xinyue.icu

================================================================================
来源：http://ebf.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://idv.fzhhl.top

python -m venv .venv && source .venv/bin/activate
来源：http://puj.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://rqx.cqqwz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ndi.nwbrower.top

[U03] Py：加载 .env 配置
来源：http://qke.wangshuangyany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://usr.jqgfzy.top

[U04] Py：变量调试打印
来源：http://qum.chenjidiqi.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://quu.hongshengwenyu.top

[U05] Py：列表去重且保序
来源：http://wxh.yongpay.top

list(dict.fromkeys(arr))
来源：http://fnt.ivvv.top

[U06] Py：合并两个字典
来源：http://iwq.hnxiangtu.top

{**a, **b}
来源：http://snt.xylfe.cn

[U07] Py：反转字典键值
来源：http://gqp.fengsongda.top

{v: k for k, v in d.items()}
来源：http://hnd.sjlbkw.cn

[U08] Py：展平二维列表
来源：http://rzg.zhaomingkeji.xyz

[y for x in nested for y in x]
来源：http://jpo.52xcode.cn

[U09] Py：字典取最大值的键
来源：http://cbw.andypj.xyz

max(d, key=d.get)
来源：http://afy.feifeiyinyue.top

[U10] Py：按值排序字典
来源：http://hlm.haohaochexian.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dvs.sufxvd.cn

[U11] Py：生成器表达式
来源：http://hzg.cqqwz.cn

(x * 2 for x in arr)
来源：http://idc.xinyue.icu

[U12] Py：取出现最多的 3 个元素
来源：http://dgl.ybcxt.top

Counter(arr).most_common(3)
来源：http://dvx.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://hpj.epnwcf.com

deque(maxlen=10)
来源：http://qov.c1oappe.top

[U14] Py：分组收集到列表
来源：http://ktk.yvedp.cn

defaultdict(list)
来源：http://vsg.0kj1m.cn

[U15] Py：高精度计时
来源：http://qmc.smart0.xyz

t = time.perf_counter()
来源：http://zwj.jqgfzy.top

[U16] Py：命令行参数解析
来源：http://ukj.dianchejie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wok.gzhubu.top

[U17] Py：初始化日志
来源：http://vwt.cheryme.top

logging.basicConfig(level=logging.INFO)
来源：http://xmq.wangdashe.top

[U18] Py：预编译正则
来源：http://zmi.cqqwz.cn

pat = re.compile(r"\d+")
来源：http://fsz.yfazqb.com

[U19] Py：正则替换带回调
来源：http://yxg.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://win.quarkkingdee.top

[U20] Py：缓存函数结果
来源：http://cbc.feifeiyinyue.top

@functools.lru_cache(maxsize=None)
来源：http://kjj.shzxlz.cn

[U21] Py：自定义上下文管理器
来源：http://gpp.yonumen.top

@contextlib.contextmanager
来源：http://nht.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://ucs.ywan-chungtsiang.top

list(zip(*m))
来源：http://prw.wangdashe.top

[U23] Py：分块读取大文件
来源：http://kkc.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jwf.dashuyun.cn

[U24] Py：路径操作
来源：http://axf.sysykeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gxf.jlsjyb.cn

[U25] Py：CSV 按字典读
来源：http://kbt.ivvv.top

csv.DictReader(f)
来源：http://ljm.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://ikk.snrcjt.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bln.guannengcc.top

[U27] Py：异步 HTTP
来源：http://rbx.xziqi.cn

aiohttp.ClientSession() 配合 async with
来源：http://xpc.quarkkingdee.top

[U28] Py：类型别名
来源：http://hgg.birdmap.top

UserId = int
来源：http://crn.cdnleiting.top

[U29] Py：属性校验
来源：http://rop.haohaochexian.top

@property 与 @x.setter 配合
来源：http://swx.zhixingplan.top

[U30] Py：数据类
来源：http://zoy.yj20258888.top

@dataclass(slots=True)
来源：http://duh.ivvv.top

[U31] Py：单测
来源：http://skv.chenzaomai.com

python -m pytest -q
来源：http://nxl.zhixingplan.top

[U32] Py：代码格式化
来源：http://vyg.bbcook.cn

ruff format . && ruff check --fix .
来源：http://fkd.yvedp.cn

[U33] Py：打包发布
来源：http://ddk.jinqigfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://auu.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://fpq.hnxiangtu.top

chardet.detect(raw)
来源：http://bja.yvedp.cn

[U35] Py：发送邮件
来源：http://dwl.sxryk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jiu.cdnleiting.top

[U36] Py：定时任务
来源：http://qrd.ehwqpu.com

schedule.every(10).minutes.do(job)
来源：http://ryd.tarul.cn

[U37] Py：读写 Excel
来源：http://wcm.yongpay.top

pandas.read_excel / DataFrame.to_excel
来源：http://chz.nanxinkj.top

[U38] Py：获取脚本所在目录
来源：http://dsp.9152youxi.cn

Path(__file__).resolve().parent
来源：http://vma.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://wsu.hongshengwenyu.top

sys.stdout.isatty()
来源：http://itm.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://wub.fzhhl.top

print("err", file=sys.stderr)
来源：http://dmt.meibo888.top

[U41] PHP：初始化 Composer 项目
来源：http://yfh.sweek.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zvv.wangdashe.top

[U42] PHP：PSR-4 自动加载
来源：http://gka.ybcxt.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ftb.zdbjq.cn

[U43] PHP：声明命名空间
来源：http://onf.gaohongyu789.top

namespace App\Http;
来源：http://rrm.tanke756.top

[U44] PHP：开启严格类型
来源：http://vqb.birdmap.top

declare(strict_types=1);
来源：http://yet.hcnkem.com

[U45] PHP：类型声明与返回类型
来源：http://iwj.hfpthk.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pgm.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://dgk.zhongyouzk.top

?string $name = null
来源：http://lqs.cheryme.top


<!-- 参考信息 -->