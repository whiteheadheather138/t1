代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://yth.c1oappe.top

[S23] C：随机数
来源：http://tld.zhongyouzk.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mgq.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://usw.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jdi.tian-w.cn

[S25] C：内存拷贝
来源：http://oiv.zycfv.cn

memcpy(dst, src, n);
来源：http://ohj.snrcjt.cn

[S26] C：内存清零
来源：http://xga.zycfv.cn

memset(a, 0, sizeof a);
来源：http://jnd.fengsongda.top

[S27] C：定义常量
来源：http://wfc.chenlongwang.top

const double PI = 3.14159;
来源：http://dsv.yanxiufei.cn

[S28] C：静态变量
来源：http://ggq.hfpthk.cn

static int counter = 0;
来源：http://vzs.fehbvm.com

[S29] C：变参函数
来源：http://arh.guowangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xlx.cheryme.top

[S30] C：头文件保护
来源：http://omd.fanxiaobao.xyz

#ifndef X_H
来源：http://tkj.fanxiaobao.xyz

#define X_H
来源：http://kdf.daxiang520.top

#endif
来源：http://isv.hesvh.cn

[S31] C++：Hello World
来源：http://hvj.jqgfzy.top

#include <iostream>
来源：http://rwz.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://lbv.hywenlv.cn

[S32] C++：字符串
来源：http://fwj.hesvh.cn

std::string s = "hi";  s += "!";
来源：http://ybu.ydzc1.top

[S33] C++：vector 增删
来源：http://pis.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uzv.xziqi.cn

[S34] C++：遍历 vector
来源：http://uux.vqdsnc.cn

for (auto &x : v) { std::cout << x; }
来源：http://qts.hcnkem.com

[S35] C++：map
来源：http://xsi.yj20258.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dxa.shzxlz.cn

[S36] C++：unordered_map
来源：http://fxq.sjlbkw.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ulz.jqgufenzy.top

[S37] C++：set
来源：http://yjw.nanxuanxn.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nxk.cdnleiting.top

[S38] C++：排序
来源：http://tdd.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://fpe.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://hwc.jianghu66.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cet.aizwys.cn

[S40] C++：查找元素
来源：http://qwc.cashguo.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ovb.xylfe.cn

[S41] C++：类与构造函数
来源：http://myo.jinqigufen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ovb.zhaomingkeji.xyz

[S42] C++：继承与虚函数
来源：http://cju.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://nbw.zhijiandao.cn

[S43] C++：智能指针
来源：http://qnz.zhijiandao.cn

auto p = std::make_unique<int>(5);
来源：http://wrp.tarul.cn

[S44] C++：引用传参
来源：http://bjn.yvedp.cn

void inc(int &x) { ++x; }
来源：http://zol.dianchejie.cn

[S45] C++：lambda
来源：http://xay.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lbh.xingfuxueyuan.xyz

[S46] C++：函数模板
来源：http://blg.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hif.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://xjx.xingfuxueyuan.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gin.ppjwa.cn

[S48] C++：逐行读文件
来源：http://oiu.gotoacloud.top

std::ifstream in("a.txt");  std::string line;
来源：http://aub.daxiang520.top

while (std::getline(in, line)) { }
来源：http://sbd.zhaomingkeji.xyz

[S49] C++：写文件
来源：http://uud.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hhs.nanxuanxn.top

[S50] C++：格式化数字
来源：http://kma.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gkz.yanxiufei.cn

[S51] C++：显式类型转换
来源：http://vuq.sweek.top

static_cast<double>(a) / b
来源：http://mwy.zdbjq.cn

[S52] C++：const 与 noexcept
来源：http://hen.yueranfly.top

int size() const noexcept { return n_; }
来源：http://gdb.ydjk.org.cn

[S53] C++：移动语义
来源：http://qor.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://yak.fktsv.cn

[S54] C++：异常处理
来源：http://opk.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://meu.fktsv.cn

[S55] C++：结构化绑定
来源：http://cdx.52xcode.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jfo.ydjk.org.cn

[S56] C++：optional
来源：http://fxa.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yig.tianlin.xyz

[S57] C++：编译期常量
来源：http://pmv.sufxvd.cn

constexpr int N = 10;
来源：http://bek.jlsjyb.cn

[S58] C++：命名空间
来源：http://kbs.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://trx.hysaishi.cn

[S59] C++：静态断言
来源：http://maq.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ikp.jyoumei.cn

[S60] C++：遍历并删除元素
来源：http://vev.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hsf.andypj.xyz

================================================================================
来源：http://sdp.wangdashe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ljt.yj20258.top

================================================================================
来源：http://hhl.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://afs.hcnkem.com

println("Hello")
来源：http://sxh.ydjk.org.cn

[T02] Kotlin：变量
来源：http://rsn.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ysy.nwbrower.top

[T03] Kotlin：字符串模板
来源：http://ysx.yj20258888.top

"值: $b"
来源：http://iuj.shanyushiyangtech.top

[T04] Kotlin：空安全
来源：http://kro.nanxuanxn.top

val n: String? = null;  n?.length
来源：http://eui.hnqzz.top

[T05] Kotlin：when 表达式
来源：http://hzl.yanxiufei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kce.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://vcu.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bpi.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://zbu.jlsjyb.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://guh.xziqi.cn

[T08] Kotlin：数据类
来源：http://qwy.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://uql.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://vwr.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://xik.zhengqikj.top

[T10] Kotlin：默认参数
来源：http://vqi.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://urm.zhoulong.xyz

[T11] Kotlin：协程
来源：http://pwi.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://meu.sysykeji.top

[T12] Kotlin：解构声明
来源：http://qeb.zhoulong.xyz

val (a, b) = Pair(1, 2)
来源：http://loy.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://evo.cdnleiting.top

val m = mapOf("a" to 1)
来源：http://kme.zhixingplan.top

[T14] Kotlin：循环
来源：http://hcf.snrcjt.cn

for (i in 1..10) println(i)
来源：http://fas.nwbrower.top

[T15] Kotlin：接口
来源：http://vsk.zhoulong.xyz

interface Shape { fun area(): Double }
来源：http://nke.daxiang520.top

[T16] Swift：Hello World
来源：http://hzh.sjlbkw.cn

print("Hello")
来源：http://tdi.hywenlv.cn

[T17] Swift：变量与常量
来源：http://sby.zhixingplan.top

var a = 1;  let b = 2
来源：http://dhk.chenzaomai.com

[T18] Swift：字符串插值
来源：http://yfm.iojbl.cn

"值: \(b)"
来源：http://eqa.c1oappe.top

[T19] Swift：可选绑定
来源：http://icj.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://plf.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://rlp.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ksm.jiagoushi.top

[T21] Swift：遍历
来源：http://zdm.yuanzhike.top

for x in a { print(x) }
来源：http://bwp.xuanzx.com

[T22] Swift：字典
来源：http://yif.daxiang520.top

var d = ["a": 1];  d["b"] = 2
来源：http://zar.ydjk.org.cn

[T23] Swift：函数
来源：http://cqm.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vbx.316326.xyz

[T24] Swift：闭包
来源：http://mxc.uphjek.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://sod.ppjwa.cn

[T25] Swift：结构体
来源：http://cnx.zhiwuduotai.top

struct P { var x: Int }
来源：http://tza.feifeiyinyue.top

[T26] Swift：类与重写
来源：http://swo.316326.xyz

class A: Base { override func f() {} }
来源：http://con.shzxlz.cn

[T27] Swift：错误处理
来源：http://erq.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://xjq.tarul.cn

[T28] Swift：枚举
来源：http://ajn.daxiang520.top

enum Color { case red, green }
来源：http://rka.tanke756.top

[T29] Swift：guard 提前返回
来源：http://vki.hywenlv.cn

guard let x = opt else { return }
来源：http://kmf.fanxiaobao.xyz

[T30] Swift：协议
来源：http://bcf.nanxinkj.top

protocol Shape { func area() -> Double }
来源：http://vma.yfazqb.com

[T31] Lua：Hello World
来源：http://nnd.shzxlz.cn

print("Hello")
来源：http://hgs.vehdjk.com

[T32] Lua：局部变量
来源：http://yay.tanke756.top

local a = 1
来源：http://mkx.hcnkem.com

[T33] Lua：表（数组）
来源：http://xlg.zdbjq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vwm.uphjek.com

[T34] Lua：遍历表
来源：http://fym.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://caa.yj202588.top

[T35] Lua：字典表
来源：http://bzp.sysykeji.top

local d = { a = 1 };  d.b = 2
来源：http://tol.tanke756.top

[T36] Lua：函数
来源：http://veo.chenlongwang.top

function add(a, b) return a + b end
来源：http://vat.tian-w.cn

[T37] Lua：字符串拼接
来源：http://iuj.ctjpmb.com

"a" .. "b"
来源：http://bwc.zdqjudy.top

[T38] Lua：条件
来源：http://alw.zhengqikj.top

if x > 0 then print("正") end
来源：http://hvq.uphjek.com

[T39] Lua：模式匹配
来源：http://unx.zhongyouzk.top

string.find(s, "%d+")
来源：http://tph.hcnkem.com

[T40] Lua：元表
来源：http://lvd.fehbvm.com

setmetatable({}, { __index = base })
来源：http://kub.kuanghao11.cn

[T41] Perl：Hello World
来源：http://ycz.yj20258888.top

print "Hello\n";
来源：http://pev.uphjek.com

[T42] Perl：变量类型
来源：http://gzb.yj202588.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://reb.uphjek.com

[T43] Perl：字符串插值
来源：http://gbj.hammf.cn

"值: $a"
来源：http://xxb.hcnkem.com

[T44] Perl：条件
来源：http://fnp.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://etn.xziqi.cn

[T45] Perl：数组遍历
来源：http://nlq.shzxlz.cn

for my $x (@arr) { print $x; }
来源：http://hpa.vehdjk.com

[T46] Perl：哈希操作
来源：http://uiy.ydjk.org.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bct.shanyushiyangkeji.top

[T47] Perl：正则捕获
来源：http://zlu.jinqigfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://frk.cdnleiting.top

[T48] Perl：正则替换
来源：http://jct.hfpthk.cn

$s =~ s/old/new/g;
来源：http://qjw.zhengqikj.top

[T49] Perl：函数
来源：http://hwy.yongpay.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zxi.zdqjudy.top

[T50] Perl：逐行读文件
来源：http://enj.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nrz.fanxiaobao.xyz

while (my $line = <$fh>) { print $line; }
来源：http://dgy.wangshuangyany.cn

[T51] Scala：Hello World
来源：http://aqp.jianghu66.top

println("Hello")
来源：http://knf.jyoumei.cn

[T52] Scala：变量
来源：http://jrc.jlsjyb.cn

val a = 1;  var b = 2
来源：http://bdt.hysaishi.cn

[T53] Scala：字符串插值
来源：http://bmo.hnxiangtu.top

s"值: $b"
来源：http://akp.yvedp.cn

[T54] Scala：集合映射
来源：http://prf.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://utp.feifeiyinyue.top

[T55] Scala：集合过滤
来源：http://mue.jyoumei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sbf.gogol.net.cn

[T56] Scala：样例类
来源：http://bnx.ppjwa.cn

case class User(name: String, age: Int)
来源：http://llq.cucudq.cn

[T57] Scala：模式匹配
来源：http://sel.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://emy.snrcjt.cn

[T58] Scala：函数定义
来源：http://mcn.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gut.ydjk.org.cn

[T59] Scala：循环
来源：http://oxo.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://iav.cdnleiting.top

[T60] Scala：折叠
来源：http://sgl.yongpay.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qly.gogol.net.cn

================================================================================
来源：http://hhj.meibo888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gse.jqgfzy.top

================================================================================
来源：http://qgc.xuanzx.com

[U01] Py：创建虚拟环境
来源：http://hqm.xziqi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jfp.uphjek.com

[U02] Py：导出 / 安装依赖
来源：http://mec.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hxr.hcnkem.com

[U03] Py：加载 .env 配置
来源：http://ihe.redwolf501.top

from dotenv import load_dotenv; load_dotenv()
来源：http://isn.jyoumei.cn

[U04] Py：变量调试打印
来源：http://xxm.jinyuanbaomall.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ccl.yuanzhike.top

[U05] Py：列表去重且保序
来源：http://mlm.sysykeji.top

list(dict.fromkeys(arr))
来源：http://xit.tian-w.cn

[U06] Py：合并两个字典
来源：http://evq.yueranfly.top

{**a, **b}
来源：http://gol.daria6918.cn

[U07] Py：反转字典键值
来源：http://jgi.c1oappe.top

{v: k for k, v in d.items()}
来源：http://qcd.jianghu66.top

[U08] Py：展平二维列表
来源：http://slz.52xcode.cn

[y for x in nested for y in x]
来源：http://ymz.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://atk.chenzaomai.com

max(d, key=d.get)
来源：http://zle.ppjwa.cn

[U10] Py：按值排序字典
来源：http://yaz.yvedp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ubx.yongpay.top

[U11] Py：生成器表达式
来源：http://opq.dashuyun.cn

(x * 2 for x in arr)
来源：http://aas.yangfankeji.com

[U12] Py：取出现最多的 3 个元素
来源：http://vws.zycfv.cn

Counter(arr).most_common(3)
来源：http://gun.shanyushiyangkeji.top

[U13] Py：固定长度队列
来源：http://tgm.zhoulong.xyz

deque(maxlen=10)
来源：http://oqw.ehwqpu.com

[U14] Py：分组收集到列表
来源：http://bpr.zhijiandao.cn

defaultdict(list)
来源：http://mzt.xziqi.cn

[U15] Py：高精度计时
来源：http://nnt.xuanzx.com

t = time.perf_counter()
来源：http://ofp.zhixingplan.top

[U16] Py：命令行参数解析
来源：http://qyk.aizwys.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fpq.meibo888.top

[U17] Py：初始化日志
来源：http://qhk.ydjk.org.cn

logging.basicConfig(level=logging.INFO)
来源：http://uun.zycfv.cn

[U18] Py：预编译正则
来源：http://qaz.yuanzhike.top

pat = re.compile(r"\d+")
来源：http://cjn.xinyue.icu

[U19] Py：正则替换带回调
来源：http://bmq.meibo888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eex.vqdsnc.cn

[U20] Py：缓存函数结果
来源：http://tii.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://mwx.ywan-chungtsiang.top

[U21] Py：自定义上下文管理器
来源：http://bhu.fanxiaobao.xyz

@contextlib.contextmanager
来源：http://pzn.nanxinkj.top

[U22] Py：矩阵转置
来源：http://dny.nwbrower.top

list(zip(*m))
来源：http://gtb.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://iac.daxiang520.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hpf.epnwcf.com

[U24] Py：路径操作
来源：http://see.tian-w.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ywn.cheryme.top

[U25] Py：CSV 按字典读
来源：http://pug.xinyue.icu

csv.DictReader(f)
来源：http://cbf.chenlongwang.top

[U26] Py：并发下载
来源：http://ckg.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jgk.shuidangran.top

[U27] Py：异步 HTTP
来源：http://zho.gzhubu.top

aiohttp.ClientSession() 配合 async with
来源：http://jgy.jyoumei.cn

[U28] Py：类型别名
来源：http://ejw.jianghu66.top

UserId = int
来源：http://xvt.yj202588.top

[U29] Py：属性校验
来源：http://bpr.xinyue.icu

@property 与 @x.setter 配合
来源：http://qjh.smart0.xyz

[U30] Py：数据类
来源：http://amu.yj20258888.top

@dataclass(slots=True)
来源：http://rjq.jinqigfzy.top

[U31] Py：单测
来源：http://ldm.tarul.cn

python -m pytest -q
来源：http://wib.dianchejie.cn

[U32] Py：代码格式化
来源：http://awy.yanxiufei.cn

ruff format . && ruff check --fix .
来源：http://oxh.xinyue.icu

[U33] Py：打包发布
来源：http://hvn.yfazqb.com

python -m build  （依赖 pyproject.toml）
来源：http://vuo.yongpay.top

[U34] Py：判断编码
来源：http://qaa.chenjidiqi.icu

chardet.detect(raw)
来源：http://suu.dashuyun.cn

[U35] Py：发送邮件
来源：http://hak.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zmc.zhiwuduotai.top

[U36] Py：定时任务
来源：http://wut.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://pfj.chenzaomai.com

[U37] Py：读写 Excel
来源：http://kci.yangfankeji.com

pandas.read_excel / DataFrame.to_excel
来源：http://ahq.xuetiantiany.cn

[U38] Py：获取脚本所在目录
来源：http://imk.ehwqpu.com

Path(__file__).resolve().parent
来源：http://fbd.jyoumei.cn

[U39] Py：判断是否在交互环境
来源：http://qpx.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://kmi.bjfxy.top

[U40] Py：打印到标准错误
来源：http://qsl.hnxiangtu.top

print("err", file=sys.stderr)
来源：http://mhh.nanxuanxn.top

[U41] PHP：初始化 Composer 项目
来源：http://swi.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bsi.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://nqr.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bat.hammf.cn

[U43] PHP：声明命名空间
来源：http://vwb.yj20258.top

namespace App\Http;
来源：http://hsk.guannengcc.top

[U44] PHP：开启严格类型
来源：http://hsb.shuidangran.top

declare(strict_types=1);
来源：http://krc.epnwcf.com

[U45] PHP：类型声明与返回类型
来源：http://zcv.52xcode.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vpc.wangshuangyany.cn

[U46] PHP：可空类型
来源：http://yaj.hnxiangtu.top

?string $name = null
来源：http://tep.cashguo.top


<!-- 参考信息 -->