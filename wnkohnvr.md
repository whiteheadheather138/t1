代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://usa.vqdsnc.cn

[S23] C：随机数
来源：http://jst.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nte.hnxiangtu.top

[S24] C：获取本地时间
来源：http://jtp.sweek.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://anx.nanxinkj.top

[S25] C：内存拷贝
来源：http://dfk.sjlbkw.cn

memcpy(dst, src, n);
来源：http://jwa.havefunace.top

[S26] C：内存清零
来源：http://xrm.redwolf501.top

memset(a, 0, sizeof a);
来源：http://grc.sweek.top

[S27] C：定义常量
来源：http://kpu.ctjpmb.com

const double PI = 3.14159;
来源：http://aaw.guowangkeji.top

[S28] C：静态变量
来源：http://bye.tanke756.top

static int counter = 0;
来源：http://euz.cucudq.cn

[S29] C：变参函数
来源：http://cbq.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aji.gaohongyu789.top

[S30] C：头文件保护
来源：http://gzw.jqgufenzy.top

#ifndef X_H
来源：http://khy.jqgufenzy.top

#define X_H
来源：http://hcw.jqgfzy.top

#endif
来源：http://xci.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://szd.xuanzx.com

#include <iostream>
来源：http://jts.sxryk.cn

int main() { std::cout << "Hello\n"; }
来源：http://dvm.svipenyu.cn

[S32] C++：字符串
来源：http://jym.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://plf.chenzaomai.com

[S33] C++：vector 增删
来源：http://cbq.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://unx.pycfn.com

[S34] C++：遍历 vector
来源：http://tcu.jyoumei.cn

for (auto &x : v) { std::cout << x; }
来源：http://oin.uphjek.com

[S35] C++：map
来源：http://whf.yuanzhike.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uep.yvedp.cn

[S36] C++：unordered_map
来源：http://zmw.ctjpmb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://czg.sjlbkw.cn

[S37] C++：set
来源：http://bxc.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qzk.quarkkingdee.top

[S38] C++：排序
来源：http://jpp.pengpengdd.cyou

std::sort(v.begin(), v.end());
来源：http://mbw.dianchejie.cn

[S39] C++：自定义比较器排序
来源：http://igc.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qeg.gogol.net.cn

[S40] C++：查找元素
来源：http://ngq.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://flg.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://gcn.cucudq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uwu.zdbjq.cn

[S42] C++：继承与虚函数
来源：http://lin.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://edw.meibo888.top

[S43] C++：智能指针
来源：http://oxx.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://bll.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://liq.yj20258.top

void inc(int &x) { ++x; }
来源：http://hpc.shuidangran.top

[S45] C++：lambda
来源：http://llt.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://bdo.nanxinkj.top

[S46] C++：函数模板
来源：http://wuv.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://thd.316326.xyz

[S47] C++：结构化绑定遍历
来源：http://htu.yj202588.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lfh.bjfxy.top

[S48] C++：逐行读文件
来源：http://bgu.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://rzw.xinyue.icu

while (std::getline(in, line)) { }
来源：http://zqz.xinyue.icu

[S49] C++：写文件
来源：http://maj.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qrf.xingfuxueyuan.xyz

[S50] C++：格式化数字
来源：http://you.ehwqpu.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pux.aizwys.cn

[S51] C++：显式类型转换
来源：http://kit.jqgfzy.top

static_cast<double>(a) / b
来源：http://wmi.fehbvm.com

[S52] C++：const 与 noexcept
来源：http://jco.tanke756.top

int size() const noexcept { return n_; }
来源：http://tkh.sweek.top

[S53] C++：移动语义
来源：http://sch.jinghuilouyu.cn

std::vector<int> w = std::move(v);
来源：http://fje.nanxinkj.top

[S54] C++：异常处理
来源：http://thi.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ckx.0kj1m.cn

[S55] C++：结构化绑定
来源：http://upi.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nsg.smart0.xyz

[S56] C++：optional
来源：http://hdv.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xcq.9152youxi.cn

[S57] C++：编译期常量
来源：http://tiw.xuetiantiany.cn

constexpr int N = 10;
来源：http://had.nanxuanxn.top

[S58] C++：命名空间
来源：http://smw.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://leb.yanxiufei.cn

[S59] C++：静态断言
来源：http://zic.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hju.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://hos.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sus.hfpthk.cn

================================================================================
来源：http://ije.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mnp.yvedp.cn

================================================================================
来源：http://qjf.cashguo.top

[T01] Kotlin：Hello World
来源：http://ypa.zdqjudy.top

println("Hello")
来源：http://rqr.sweek.top

[T02] Kotlin：变量
来源：http://ttd.havefunace.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tal.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://iiw.hnxiangtu.top

"值: $b"
来源：http://opf.c1oappe.top

[T04] Kotlin：空安全
来源：http://meh.yj20258.top

val n: String? = null;  n?.length
来源：http://ljo.chenjidiqi.icu

[T05] Kotlin：when 表达式
来源：http://ypy.zhaomingkeji.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tox.fanxiaobao.xyz

[T06] Kotlin：集合映射
来源：http://jfr.hongshengwenyu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cei.tanke756.top

[T07] Kotlin：集合过滤
来源：http://tdi.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xqv.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://shf.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://gaa.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://rau.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://bmv.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://ofm.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ozc.shzxlz.cn

[T11] Kotlin：协程
来源：http://hrp.yuxming.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kxn.nanxuanxn.top

[T12] Kotlin：解构声明
来源：http://eky.52xcode.cn

val (a, b) = Pair(1, 2)
来源：http://zds.cashguo.top

[T13] Kotlin：只读 Map
来源：http://dzv.wangdashe.top

val m = mapOf("a" to 1)
来源：http://qju.sxryk.cn

[T14] Kotlin：循环
来源：http://buc.tian-w.cn

for (i in 1..10) println(i)
来源：http://snd.ydjk.org.cn

[T15] Kotlin：接口
来源：http://eik.hnxiangtu.top

interface Shape { fun area(): Double }
来源：http://fef.jinghuilouyu.cn

[T16] Swift：Hello World
来源：http://sam.zhoulong.xyz

print("Hello")
来源：http://bfi.tarul.cn

[T17] Swift：变量与常量
来源：http://dvu.sxryk.cn

var a = 1;  let b = 2
来源：http://eeu.sysykeji.top

[T18] Swift：字符串插值
来源：http://wtj.hcnkem.com

"值: \(b)"
来源：http://atw.ydzc1.top

[T19] Swift：可选绑定
来源：http://pvn.ctjpmb.com

if let n = opt { print(n) }
来源：http://yxv.hesvh.cn

[T20] Swift：数组操作
来源：http://loa.redwolf501.top

var a = [1, 2, 3];  a.append(4)
来源：http://mnh.chenjidiqi.icu

[T21] Swift：遍历
来源：http://lil.shuidangran.top

for x in a { print(x) }
来源：http://evo.feifeiyinyue.top

[T22] Swift：字典
来源：http://jea.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://prg.sxryk.cn

[T23] Swift：函数
来源：http://efi.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cie.yuxming.cn

[T24] Swift：闭包
来源：http://mzq.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://skn.hnqzz.top

[T25] Swift：结构体
来源：http://ous.vqdsnc.cn

struct P { var x: Int }
来源：http://dih.dianchejie.cn

[T26] Swift：类与重写
来源：http://iny.redwolf501.top

class A: Base { override func f() {} }
来源：http://mbu.zdqjudy.top

[T27] Swift：错误处理
来源：http://zhs.fengsongda.top

do { try f() } catch { print(error) }
来源：http://dht.tian-w.cn

[T28] Swift：枚举
来源：http://ipv.cucudq.cn

enum Color { case red, green }
来源：http://zwg.jianghu66.top

[T29] Swift：guard 提前返回
来源：http://gbk.svipenyu.cn

guard let x = opt else { return }
来源：http://czf.yanxiufei.cn

[T30] Swift：协议
来源：http://lop.ehwqpu.com

protocol Shape { func area() -> Double }
来源：http://rpw.guowangkeji.top

[T31] Lua：Hello World
来源：http://jpq.daxiang520.top

print("Hello")
来源：http://oww.dashuyun.cn

[T32] Lua：局部变量
来源：http://hup.meibo888.top

local a = 1
来源：http://jos.52xcode.cn

[T33] Lua：表（数组）
来源：http://hsw.fehbvm.com

local t = {1, 2, 3};  t[4] = 4
来源：http://eyq.hywenlv.cn

[T34] Lua：遍历表
来源：http://vwo.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://diw.jqgufenzy.top

[T35] Lua：字典表
来源：http://hop.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://hul.zhixingplan.top

[T36] Lua：函数
来源：http://jzl.jqgufenzy.top

function add(a, b) return a + b end
来源：http://mvg.xylfe.cn

[T37] Lua：字符串拼接
来源：http://cfu.ybcxt.top

"a" .. "b"
来源：http://ojy.uphjek.com

[T38] Lua：条件
来源：http://ywc.zhijiandao.cn

if x > 0 then print("正") end
来源：http://ndp.pycfn.com

[T39] Lua：模式匹配
来源：http://qwh.haohaochexian.top

string.find(s, "%d+")
来源：http://pkc.tian-w.cn

[T40] Lua：元表
来源：http://ysk.tianlin.xyz

setmetatable({}, { __index = base })
来源：http://mrr.feifeiyinyue.top

[T41] Perl：Hello World
来源：http://wul.tanke756.top

print "Hello\n";
来源：http://eig.daxiang520.top

[T42] Perl：变量类型
来源：http://adm.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kiz.daxiang520.top

[T43] Perl：字符串插值
来源：http://emz.yuxming.cn

"值: $a"
来源：http://jgw.gogol.net.cn

[T44] Perl：条件
来源：http://lsq.zhongyouzk.top

if ($a > 0) { print "正"; }
来源：http://vsd.hcnkem.com

[T45] Perl：数组遍历
来源：http://zkt.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://hic.yanxiufei.cn

[T46] Perl：哈希操作
来源：http://rzj.ppjwa.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cvj.smart0.xyz

[T47] Perl：正则捕获
来源：http://bcm.tarul.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mcb.yangfankeji.com

[T48] Perl：正则替换
来源：http://xjr.birdmap.top

$s =~ s/old/new/g;
来源：http://lbn.sufxvd.cn

[T49] Perl：函数
来源：http://qdz.guannengcc.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://spf.zhaomingkeji.xyz

[T50] Perl：逐行读文件
来源：http://kun.hesvh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fgm.dianchejie.cn

while (my $line = <$fh>) { print $line; }
来源：http://wao.mhx1999.top

[T51] Scala：Hello World
来源：http://pri.hysaishi.cn

println("Hello")
来源：http://vis.nwbrower.top

[T52] Scala：变量
来源：http://hgx.jinqigufen.top

val a = 1;  var b = 2
来源：http://zvv.haohaochexian.top

[T53] Scala：字符串插值
来源：http://mmc.tianlin.xyz

s"值: $b"
来源：http://nwx.aibaodan.cn

[T54] Scala：集合映射
来源：http://cju.fktsv.cn

List(1, 2, 3).map(_ * 2)
来源：http://gok.sysykeji.top

[T55] Scala：集合过滤
来源：http://fkk.yj202588.top

List(1, 2, 3).filter(_ > 1)
来源：http://ujs.zdqjudy.top

[T56] Scala：样例类
来源：http://jlx.vehdjk.com

case class User(name: String, age: Int)
来源：http://aix.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://jyg.cucudq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mzp.jinyuanbaomall.cn

[T58] Scala：函数定义
来源：http://daa.gaohongyu789.top

def add(a: Int, b: Int): Int = a + b
来源：http://fer.hfpthk.cn

[T59] Scala：循环
来源：http://kna.jyoumei.cn

for (i <- 1 to 10) println(i)
来源：http://sbc.ydzc1.top

[T60] Scala：折叠
来源：http://kdy.0kj1m.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dla.gzhubu.top

================================================================================
来源：http://cke.hywenlv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://arv.hfpthk.cn

================================================================================
来源：http://qul.wangdashe.top

[U01] Py：创建虚拟环境
来源：http://kko.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://mzf.jyoumei.cn

[U02] Py：导出 / 安装依赖
来源：http://teu.havefunace.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ivx.shangyingyoupin.top

[U03] Py：加载 .env 配置
来源：http://use.zhixingplan.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ixz.chenjidiqi.icu

[U04] Py：变量调试打印
来源：http://tvm.yfazqb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://egs.sxryk.cn

[U05] Py：列表去重且保序
来源：http://zpo.ppjwa.cn

list(dict.fromkeys(arr))
来源：http://itu.xingfuxueyuan.xyz

[U06] Py：合并两个字典
来源：http://bgo.jinqigfzy.top

{**a, **b}
来源：http://kxg.ctjpmb.com

[U07] Py：反转字典键值
来源：http://cir.yongpay.top

{v: k for k, v in d.items()}
来源：http://tca.havefunace.top

[U08] Py：展平二维列表
来源：http://kqj.zhiwuduotai.top

[y for x in nested for y in x]
来源：http://pym.316326.xyz

[U09] Py：字典取最大值的键
来源：http://rey.haohaochexian.top

max(d, key=d.get)
来源：http://tzc.hesvh.cn

[U10] Py：按值排序字典
来源：http://pfr.birdmap.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kyn.cashguo.top

[U11] Py：生成器表达式
来源：http://ybw.ybcxt.top

(x * 2 for x in arr)
来源：http://olb.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://okm.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://qed.nanxuanxn.top

[U13] Py：固定长度队列
来源：http://qqt.cqqwz.cn

deque(maxlen=10)
来源：http://ycy.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://cgc.yj20258.top

defaultdict(list)
来源：http://wre.zhoulong.xyz

[U15] Py：高精度计时
来源：http://mbi.fzhhl.top

t = time.perf_counter()
来源：http://zwu.yvedp.cn

[U16] Py：命令行参数解析
来源：http://rji.uphjek.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sqt.aibaodan.cn

[U17] Py：初始化日志
来源：http://lsa.epnwcf.com

logging.basicConfig(level=logging.INFO)
来源：http://cif.wangdashe.top

[U18] Py：预编译正则
来源：http://uhw.ybcxt.top

pat = re.compile(r"\d+")
来源：http://dbb.zhiwuduotai.top

[U19] Py：正则替换带回调
来源：http://dzf.yongpay.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gqm.xziqi.cn

[U20] Py：缓存函数结果
来源：http://ptx.kuanghao11.cn

@functools.lru_cache(maxsize=None)
来源：http://rpn.zhongyouzk.top

[U21] Py：自定义上下文管理器
来源：http://uao.ybcxt.top

@contextlib.contextmanager
来源：http://dhx.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://old.zdbjq.cn

list(zip(*m))
来源：http://vsd.ybcxt.top

[U23] Py：分块读取大文件
来源：http://eog.iojbl.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xor.xylfe.cn

[U24] Py：路径操作
来源：http://qqg.uphjek.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hei.snrcjt.cn

[U25] Py：CSV 按字典读
来源：http://ylz.yfazqb.com

csv.DictReader(f)
来源：http://nfd.jlsjyb.cn

[U26] Py：并发下载
来源：http://wol.sufxvd.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zuj.cucudq.cn

[U27] Py：异步 HTTP
来源：http://zem.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://zxb.aibaodan.cn

[U28] Py：类型别名
来源：http://wis.gaohongyu789.top

UserId = int
来源：http://eti.gaohongyu789.top

[U29] Py：属性校验
来源：http://fmh.yj202588.top

@property 与 @x.setter 配合
来源：http://zes.hcnkem.com

[U30] Py：数据类
来源：http://hpz.chenlongwang.top

@dataclass(slots=True)
来源：http://xmv.gotoacloud.top

[U31] Py：单测
来源：http://ypy.gogol.net.cn

python -m pytest -q
来源：http://sqf.xinyue.icu

[U32] Py：代码格式化
来源：http://emj.zhiwuduotai.top

ruff format . && ruff check --fix .
来源：http://qrn.zhiwuduotai.top

[U33] Py：打包发布
来源：http://uce.yj20258.top

python -m build  （依赖 pyproject.toml）
来源：http://ldu.fanxiaobao.xyz

[U34] Py：判断编码
来源：http://weo.fehbvm.com

chardet.detect(raw)
来源：http://eio.316326.xyz

[U35] Py：发送邮件
来源：http://edp.daxiang520.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vne.zdqjudy.top

[U36] Py：定时任务
来源：http://xfa.ywan-chungtsiang.top

schedule.every(10).minutes.do(job)
来源：http://xmq.mhx1999.top

[U37] Py：读写 Excel
来源：http://cxr.daxiang520.top

pandas.read_excel / DataFrame.to_excel
来源：http://hkq.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://vsg.yueranfly.top

Path(__file__).resolve().parent
来源：http://duv.yuanzhike.top

[U39] Py：判断是否在交互环境
来源：http://pkt.gzhubu.top

sys.stdout.isatty()
来源：http://hqt.fzhhl.top

[U40] Py：打印到标准错误
来源：http://ghd.hammf.cn

print("err", file=sys.stderr)
来源：http://tyt.bjfxy.top

[U41] PHP：初始化 Composer 项目
来源：http://eni.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://urv.zdqjudy.top

[U42] PHP：PSR-4 自动加载
来源：http://umy.chenlongwang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://etq.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://njs.hnqzz.top

namespace App\Http;
来源：http://ehh.ywan-chungtsiang.top

[U44] PHP：开启严格类型
来源：http://zwi.sysykeji.top

declare(strict_types=1);
来源：http://xiw.ehwqpu.com

[U45] PHP：类型声明与返回类型
来源：http://bxd.feifeiyinyue.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yje.andypj.xyz

[U46] PHP：可空类型
来源：http://xng.zhengqikj.top

?string $name = null
来源：http://pkj.yuxming.cn


<!-- 参考信息 -->