代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pde.shzxlz.cn

[S25] C：内存拷贝
来源：http://gfx.fengsongda.top

memcpy(dst, src, n);
来源：http://mls.pycfn.com

[S26] C：内存清零
来源：http://eqb.xuanzx.com

memset(a, 0, sizeof a);
来源：http://bas.vehdjk.com

[S27] C：定义常量
来源：http://irw.fktsv.cn

const double PI = 3.14159;
来源：http://rhf.shzxlz.cn

[S28] C：静态变量
来源：http://ghi.feifeiyinyue.top

static int counter = 0;
来源：http://rri.pengpengdd.cyou

[S29] C：变参函数
来源：http://sis.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nms.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://kga.fktsv.cn

#ifndef X_H
来源：http://cpo.xuanzx.com

#define X_H
来源：http://fij.zdqjudy.top

#endif
来源：http://glu.sysykeji.top

[S31] C++：Hello World
来源：http://bkg.iojbl.cn

#include <iostream>
来源：http://egj.bjfxy.top

int main() { std::cout << "Hello\n"; }
来源：http://eud.chenjidiqi.icu

[S32] C++：字符串
来源：http://ygb.jyoumei.cn

std::string s = "hi";  s += "!";
来源：http://idm.zdbjq.cn

[S33] C++：vector 增删
来源：http://qid.shuidangran.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lvo.vehdjk.com

[S34] C++：遍历 vector
来源：http://fps.smart0.xyz

for (auto &x : v) { std::cout << x; }
来源：http://ilj.xuanzx.com

[S35] C++：map
来源：http://xcl.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://unm.jyoumei.cn

[S36] C++：unordered_map
来源：http://rgq.chenjidiqi.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mia.mhx1999.top

[S37] C++：set
来源：http://gbn.nanxuanxn.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yja.yfazqb.com

[S38] C++：排序
来源：http://fvs.meibo888.top

std::sort(v.begin(), v.end());
来源：http://ahv.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://prv.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ngu.tarul.cn

[S40] C++：查找元素
来源：http://pik.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qlx.yanxiufei.cn

[S41] C++：类与构造函数
来源：http://cyk.chenlongwang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sbv.sweek.top

[S42] C++：继承与虚函数
来源：http://wba.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://mjs.yangfankeji.com

[S43] C++：智能指针
来源：http://gvq.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://lpf.aizwys.cn

[S44] C++：引用传参
来源：http://dsu.pycfn.com

void inc(int &x) { ++x; }
来源：http://hhb.pengpengdd.cyou

[S45] C++：lambda
来源：http://mlt.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rxv.fktsv.cn

[S46] C++：函数模板
来源：http://qcy.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gsa.redwolf501.top

[S47] C++：结构化绑定遍历
来源：http://ezu.hnqzz.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://beo.redwolf501.top

[S48] C++：逐行读文件
来源：http://xxk.bjfxy.top

std::ifstream in("a.txt");  std::string line;
来源：http://dpl.dashuyun.cn

while (std::getline(in, line)) { }
来源：http://hak.zhijiandao.cn

[S49] C++：写文件
来源：http://ixk.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ajr.nwbrower.top

[S50] C++：格式化数字
来源：http://isq.tian-w.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fjb.yueranfly.top

[S51] C++：显式类型转换
来源：http://gyl.iojbl.cn

static_cast<double>(a) / b
来源：http://erg.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://jrv.feifeiyinyue.top

int size() const noexcept { return n_; }
来源：http://gxt.guannengcc.top

[S53] C++：移动语义
来源：http://miw.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://agl.sxryk.cn

[S54] C++：异常处理
来源：http://pif.jiagoushi.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hdr.jqgufenzy.top

[S55] C++：结构化绑定
来源：http://met.ehwqpu.com

auto [a, b] = std::make_pair(1, 2);
来源：http://dha.xuetiantiany.cn

[S56] C++：optional
来源：http://qss.tianlin.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bbe.vqdsnc.cn

[S57] C++：编译期常量
来源：http://opg.jianghu66.top

constexpr int N = 10;
来源：http://ydv.cdnleiting.top

[S58] C++：命名空间
来源：http://fxv.yueranfly.top

namespace ns { int f() { return 1; } }
来源：http://bcc.dianchejie.cn

[S59] C++：静态断言
来源：http://maz.ctjpmb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bjg.birdmap.top

[S60] C++：遍历并删除元素
来源：http://bht.cdnleiting.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ldd.guannengcc.top

================================================================================
来源：http://ccm.zhengqikj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://urh.zycfv.cn

================================================================================
来源：http://hhs.yvedp.cn

[T01] Kotlin：Hello World
来源：http://lix.sweek.top

println("Hello")
来源：http://eel.pycfn.com

[T02] Kotlin：变量
来源：http://hbp.hnqzz.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bph.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://sbg.feifeiyinyue.top

"值: $b"
来源：http://aeb.feifeiyinyue.top

[T04] Kotlin：空安全
来源：http://ozj.gaohongyu789.top

val n: String? = null;  n?.length
来源：http://xtt.cheryme.top

[T05] Kotlin：when 表达式
来源：http://liw.xuetiantiany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://foy.redwolf501.top

[T06] Kotlin：集合映射
来源：http://hfe.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fzi.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://kxm.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://akf.yj20258.top

[T08] Kotlin：数据类
来源：http://wcs.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://nrm.ybcxt.top

[T09] Kotlin：扩展函数
来源：http://gxw.nanxuanxn.top

fun String.exclaim() = this + "!"
来源：http://pvz.jinghuilouyu.cn

[T10] Kotlin：默认参数
来源：http://hgz.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://yvv.zdqjudy.top

[T11] Kotlin：协程
来源：http://fnr.zycfv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nsv.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://jrz.shanyushiyangtech.top

val (a, b) = Pair(1, 2)
来源：http://quz.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://xap.yongpay.top

val m = mapOf("a" to 1)
来源：http://rio.yangfankeji.com

[T14] Kotlin：循环
来源：http://sls.yangfankeji.com

for (i in 1..10) println(i)
来源：http://otx.jiagoushi.top

[T15] Kotlin：接口
来源：http://rjq.zhiwuduotai.top

interface Shape { fun area(): Double }
来源：http://uom.hysaishi.cn

[T16] Swift：Hello World
来源：http://wvj.jinghuilouyu.cn

print("Hello")
来源：http://kof.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://rjo.zhixingplan.top

var a = 1;  let b = 2
来源：http://qvx.yangfankeji.com

[T18] Swift：字符串插值
来源：http://mru.ppjwa.cn

"值: \(b)"
来源：http://jow.cucudq.cn

[T19] Swift：可选绑定
来源：http://oiz.fengsongda.top

if let n = opt { print(n) }
来源：http://rwe.zycfv.cn

[T20] Swift：数组操作
来源：http://kgz.zhoulong.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://quy.svipenyu.cn

[T21] Swift：遍历
来源：http://ora.sjlbkw.cn

for x in a { print(x) }
来源：http://rru.ydzc1.top

[T22] Swift：字典
来源：http://lzy.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tni.fengsongda.top

[T23] Swift：函数
来源：http://hxv.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jmd.zhengqikj.top

[T24] Swift：闭包
来源：http://jsw.jqgfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://nag.snrcjt.cn

[T25] Swift：结构体
来源：http://sdo.uphjek.com

struct P { var x: Int }
来源：http://mle.tianlin.xyz

[T26] Swift：类与重写
来源：http://twe.uphjek.com

class A: Base { override func f() {} }
来源：http://hyz.jinqigfzy.top

[T27] Swift：错误处理
来源：http://ekl.daria6918.cn

do { try f() } catch { print(error) }
来源：http://hfq.hesvh.cn

[T28] Swift：枚举
来源：http://ldy.yvedp.cn

enum Color { case red, green }
来源：http://thp.52xcode.cn

[T29] Swift：guard 提前返回
来源：http://qfe.ywan-chungtsiang.top

guard let x = opt else { return }
来源：http://txi.shanyushiyangtech.top

[T30] Swift：协议
来源：http://rwb.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://uzs.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://jig.yj202588.top

print("Hello")
来源：http://xzi.hesvh.cn

[T32] Lua：局部变量
来源：http://tkf.shangyingyoupin.top

local a = 1
来源：http://fhg.ivvv.top

[T33] Lua：表（数组）
来源：http://vab.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://shw.yj202588.top

[T34] Lua：遍历表
来源：http://wqs.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ibt.pengpengdd.cyou

[T35] Lua：字典表
来源：http://pdd.sufxvd.cn

local d = { a = 1 };  d.b = 2
来源：http://rma.cashguo.top

[T36] Lua：函数
来源：http://rft.yj202588.top

function add(a, b) return a + b end
来源：http://tss.shanyushiyangkeji.top

[T37] Lua：字符串拼接
来源：http://anq.daxiang520.top

"a" .. "b"
来源：http://upm.haohaochexian.top

[T38] Lua：条件
来源：http://wyn.cucudq.cn

if x > 0 then print("正") end
来源：http://uor.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://yza.jianghu66.top

string.find(s, "%d+")
来源：http://gxp.jlsjyb.cn

[T40] Lua：元表
来源：http://wnz.ctjpmb.com

setmetatable({}, { __index = base })
来源：http://zcr.jlsjyb.cn

[T41] Perl：Hello World
来源：http://rjn.jqgufenzy.top

print "Hello\n";
来源：http://zvo.hcnkem.com

[T42] Perl：变量类型
来源：http://bxk.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://prk.daria6918.cn

[T43] Perl：字符串插值
来源：http://ikl.ehwqpu.com

"值: $a"
来源：http://vfr.gaohongyu789.top

[T44] Perl：条件
来源：http://qzp.yuanzhike.top

if ($a > 0) { print "正"; }
来源：http://zhf.wangdashe.top

[T45] Perl：数组遍历
来源：http://xxx.fanxiaobao.xyz

for my $x (@arr) { print $x; }
来源：http://cfz.pycfn.com

[T46] Perl：哈希操作
来源：http://las.zdqjudy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://weg.yj202588.top

[T47] Perl：正则捕获
来源：http://tty.jqgfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://saf.chenlongwang.top

[T48] Perl：正则替换
来源：http://doj.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://gwl.sufxvd.cn

[T49] Perl：函数
来源：http://jcn.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uhs.meibo888.top

[T50] Perl：逐行读文件
来源：http://crj.chenzaomai.com

open my $fh, "<", "a.txt" or die $!;
来源：http://bpl.hnxiangtu.top

while (my $line = <$fh>) { print $line; }
来源：http://dlv.zhengqikj.top

[T51] Scala：Hello World
来源：http://lnf.gzhubu.top

println("Hello")
来源：http://gwx.sysykeji.top

[T52] Scala：变量
来源：http://paq.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://aio.yonumen.top

[T53] Scala：字符串插值
来源：http://ayj.mhx1999.top

s"值: $b"
来源：http://wfp.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://dtf.nanxuanxn.top

List(1, 2, 3).map(_ * 2)
来源：http://qoa.hnqzz.top

[T55] Scala：集合过滤
来源：http://gfp.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://dzd.feifeiyinyue.top

[T56] Scala：样例类
来源：http://jhr.gogol.net.cn

case class User(name: String, age: Int)
来源：http://sed.jinyuanbaomall.cn

[T57] Scala：模式匹配
来源：http://blk.cdnleiting.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kse.ydjk.org.cn

[T58] Scala：函数定义
来源：http://tgq.chenzaomai.com

def add(a: Int, b: Int): Int = a + b
来源：http://zcf.yj20258888.top

[T59] Scala：循环
来源：http://rtc.shanyushiyangkeji.top

for (i <- 1 to 10) println(i)
来源：http://eaf.zhoulong.xyz

[T60] Scala：折叠
来源：http://kfa.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rqe.mhx1999.top

================================================================================
来源：http://tsr.pycfn.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qib.quarkkingdee.top

================================================================================
来源：http://zfy.chenlongwang.top

[U01] Py：创建虚拟环境
来源：http://tir.nwbrower.top

python -m venv .venv && source .venv/bin/activate
来源：http://lxm.cheryme.top

[U02] Py：导出 / 安装依赖
来源：http://uwm.tarul.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xhk.sjlbkw.cn

[U03] Py：加载 .env 配置
来源：http://mki.fehbvm.com

from dotenv import load_dotenv; load_dotenv()
来源：http://gab.jyoumei.cn

[U04] Py：变量调试打印
来源：http://jfk.jinqigufen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://czw.gzhubu.top

[U05] Py：列表去重且保序
来源：http://nra.zhixingplan.top

list(dict.fromkeys(arr))
来源：http://zhp.yj20258.top

[U06] Py：合并两个字典
来源：http://efa.sufxvd.cn

{**a, **b}
来源：http://cwo.hesvh.cn

[U07] Py：反转字典键值
来源：http://gue.zhengqikj.top

{v: k for k, v in d.items()}
来源：http://knn.andypj.xyz

[U08] Py：展平二维列表
来源：http://sgd.shanyushiyangtech.top

[y for x in nested for y in x]
来源：http://lql.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://kzn.zhijiandao.cn

max(d, key=d.get)
来源：http://yvl.redwolf501.top

[U10] Py：按值排序字典
来源：http://hqh.xinyue.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rth.zhaomingkeji.xyz

[U11] Py：生成器表达式
来源：http://nqs.fktsv.cn

(x * 2 for x in arr)
来源：http://nat.yfazqb.com

[U12] Py：取出现最多的 3 个元素
来源：http://qel.zhiwuduotai.top

Counter(arr).most_common(3)
来源：http://wie.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://acm.yuxming.cn

deque(maxlen=10)
来源：http://ufw.nwbrower.top

[U14] Py：分组收集到列表
来源：http://lta.cdnleiting.top

defaultdict(list)
来源：http://oyg.zhiwuduotai.top

[U15] Py：高精度计时
来源：http://dlf.fanxiaobao.xyz

t = time.perf_counter()
来源：http://vbb.jinqigfzy.top

[U16] Py：命令行参数解析
来源：http://ceb.jinyuanbaomall.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dwh.wangdashe.top

[U17] Py：初始化日志
来源：http://qpy.chenlongwang.top

logging.basicConfig(level=logging.INFO)
来源：http://bht.fktsv.cn

[U18] Py：预编译正则
来源：http://gyc.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://jar.guowangkeji.top

[U19] Py：正则替换带回调
来源：http://uje.uphjek.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oei.mhx1999.top

[U20] Py：缓存函数结果
来源：http://ovv.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://ghv.zhixingplan.top

[U21] Py：自定义上下文管理器
来源：http://kxi.52xcode.cn

@contextlib.contextmanager
来源：http://wpe.daxiang520.top

[U22] Py：矩阵转置
来源：http://vou.hammf.cn

list(zip(*m))
来源：http://gcs.jinqigufen.top

[U23] Py：分块读取大文件
来源：http://vfo.xylfe.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rho.ivvv.top

[U24] Py：路径操作
来源：http://jrd.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pdy.epnwcf.com

[U25] Py：CSV 按字典读
来源：http://tca.yanxiufei.cn

csv.DictReader(f)
来源：http://ruc.zdbjq.cn

[U26] Py：并发下载
来源：http://dvf.yuxming.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iyl.daria6918.cn

[U27] Py：异步 HTTP
来源：http://tqm.haohaochexian.top

aiohttp.ClientSession() 配合 async with
来源：http://vqj.sweek.top

[U28] Py：类型别名
来源：http://dkk.jinyuanbaomall.cn

UserId = int
来源：http://yar.uphjek.com

[U29] Py：属性校验
来源：http://pxp.wangdashe.top

@property 与 @x.setter 配合
来源：http://njb.ybcxt.top

[U30] Py：数据类
来源：http://tfb.jinyuanbaomall.cn

@dataclass(slots=True)
来源：http://qbg.svipenyu.cn

[U31] Py：单测
来源：http://owr.jlsjyb.cn

python -m pytest -q
来源：http://ljo.yangfankeji.com

[U32] Py：代码格式化
来源：http://pbw.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://zgc.hnqzz.top

[U33] Py：打包发布
来源：http://iir.havefunace.top

python -m build  （依赖 pyproject.toml）
来源：http://tov.gotoacloud.top

[U34] Py：判断编码
来源：http://dwu.yonumen.top

chardet.detect(raw)
来源：http://ymx.9152youxi.cn

[U35] Py：发送邮件
来源：http://nkc.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://myb.hnqzz.top

[U36] Py：定时任务
来源：http://lvg.jyoumei.cn

schedule.every(10).minutes.do(job)
来源：http://xxo.epnwcf.com

[U37] Py：读写 Excel
来源：http://fmy.jiagoushi.top

pandas.read_excel / DataFrame.to_excel
来源：http://rke.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://mpn.shangyingyoupin.top

Path(__file__).resolve().parent
来源：http://raj.jlsjyb.cn

[U39] Py：判断是否在交互环境
来源：http://dup.wangdashe.top

sys.stdout.isatty()
来源：http://baf.ywan-chungtsiang.top

[U40] Py：打印到标准错误
来源：http://oeu.gotoacloud.top

print("err", file=sys.stderr)
来源：http://hth.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://rec.gogol.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://clj.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://mcq.yongpay.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mqe.jqgufenzy.top

[U43] PHP：声明命名空间
来源：http://hkq.gogol.net.cn

namespace App\Http;
来源：http://yze.aibaodan.cn

[U44] PHP：开启严格类型
来源：http://mmb.chenlongwang.top

declare(strict_types=1);
来源：http://bus.jlsjyb.cn

[U45] PHP：类型声明与返回类型
来源：http://onp.hcnkem.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://tym.yueranfly.top

[U46] PHP：可空类型
来源：http://biz.9152youxi.cn

?string $name = null
来源：http://wnj.fzhhl.top

[U47] PHP：联合类型
来源：http://rzf.svipenyu.cn

int|string $id
来源：http://hrv.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://nlg.nanxuanxn.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bpq.yangfankeji.com


<!-- 参考信息 -->