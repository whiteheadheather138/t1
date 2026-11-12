代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://jvn.zhongyouzk.top

[S23] C：随机数
来源：http://car.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://emh.gogol.net.cn

[S24] C：获取本地时间
来源：http://azd.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dcc.yueranfly.top

[S25] C：内存拷贝
来源：http://nvl.hywenlv.cn

memcpy(dst, src, n);
来源：http://nmd.daxiang520.top

[S26] C：内存清零
来源：http://vdh.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://qom.xziqi.cn

[S27] C：定义常量
来源：http://yma.wangshuangyany.cn

const double PI = 3.14159;
来源：http://drs.yanxiufei.cn

[S28] C：静态变量
来源：http://dmm.xinyue.icu

static int counter = 0;
来源：http://hxm.zycfv.cn

[S29] C：变参函数
来源：http://dau.shzxlz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ikp.hywenlv.cn

[S30] C：头文件保护
来源：http://eyj.jianghu66.top

#ifndef X_H
来源：http://str.jinyuanbaomall.cn

#define X_H
来源：http://nvz.sysykeji.top

#endif
来源：http://gll.epnwcf.com

[S31] C++：Hello World
来源：http://wcp.shanyushiyangtech.top

#include <iostream>
来源：http://cor.fktsv.cn

int main() { std::cout << "Hello\n"; }
来源：http://rkf.jqgfzy.top

[S32] C++：字符串
来源：http://bbj.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://gnp.9152youxi.cn

[S33] C++：vector 增删
来源：http://eoz.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kar.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://ltn.jinghuilouyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://hva.sjlbkw.cn

[S35] C++：map
来源：http://qhs.yonumen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lhj.zhoulong.xyz

[S36] C++：unordered_map
来源：http://jrt.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vio.gaohongyu789.top

[S37] C++：set
来源：http://hrh.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://viv.daria6918.cn

[S38] C++：排序
来源：http://fox.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://qqf.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://wex.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://shn.smart0.xyz

[S40] C++：查找元素
来源：http://nby.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gys.sufxvd.cn

[S41] C++：类与构造函数
来源：http://cso.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ptm.birdmap.top

[S42] C++：继承与虚函数
来源：http://nhz.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://ypm.ehwqpu.com

[S43] C++：智能指针
来源：http://kuz.nanxuanxn.top

auto p = std::make_unique<int>(5);
来源：http://mjf.zhijiandao.cn

[S44] C++：引用传参
来源：http://hqc.52xcode.cn

void inc(int &x) { ++x; }
来源：http://xxp.jinghuilouyu.cn

[S45] C++：lambda
来源：http://poc.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://toy.ctjpmb.com

[S46] C++：函数模板
来源：http://dih.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jnn.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://ydv.52xcode.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iym.shanyushiyangtech.top

[S48] C++：逐行读文件
来源：http://vxe.jyoumei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vub.ydzc1.top

while (std::getline(in, line)) { }
来源：http://bub.9152youxi.cn

[S49] C++：写文件
来源：http://joa.yuxming.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pnc.sysykeji.top

[S50] C++：格式化数字
来源：http://zos.gaohongyu789.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jri.fktsv.cn

[S51] C++：显式类型转换
来源：http://lmr.hnxiangtu.top

static_cast<double>(a) / b
来源：http://qod.fengsongda.top

[S52] C++：const 与 noexcept
来源：http://kwd.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://jtk.jlsjyb.cn

[S53] C++：移动语义
来源：http://yyo.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://rbb.dianchejie.cn

[S54] C++：异常处理
来源：http://kty.0kj1m.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xve.shangyingyoupin.top

[S55] C++：结构化绑定
来源：http://sji.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ybp.ywan-chungtsiang.top

[S56] C++：optional
来源：http://etr.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fuf.jinqigufen.top

[S57] C++：编译期常量
来源：http://owz.epnwcf.com

constexpr int N = 10;
来源：http://dsa.pengpengdd.cyou

[S58] C++：命名空间
来源：http://kvv.fengsongda.top

namespace ns { int f() { return 1; } }
来源：http://lun.zhixingplan.top

[S59] C++：静态断言
来源：http://uyo.guowangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kqy.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://hdr.zhongyouzk.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zrx.fehbvm.com

================================================================================
来源：http://shs.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vyp.ppjwa.cn

================================================================================
来源：http://ofg.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://qpx.ydjk.org.cn

println("Hello")
来源：http://dcm.zdbjq.cn

[T02] Kotlin：变量
来源：http://jsi.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ckc.sxryk.cn

[T03] Kotlin：字符串模板
来源：http://geu.fengsongda.top

"值: $b"
来源：http://puq.ppjwa.cn

[T04] Kotlin：空安全
来源：http://kuj.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://mwl.yvedp.cn

[T05] Kotlin：when 表达式
来源：http://qqt.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hog.wangdashe.top

[T06] Kotlin：集合映射
来源：http://jtx.ivvv.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rtk.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://lwa.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rnz.9152youxi.cn

[T08] Kotlin：数据类
来源：http://ejr.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://pfu.yangfankeji.com

[T09] Kotlin：扩展函数
来源：http://xcj.andypj.xyz

fun String.exclaim() = this + "!"
来源：http://yvl.sxryk.cn

[T10] Kotlin：默认参数
来源：http://ecr.jiagoushi.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ahr.fktsv.cn

[T11] Kotlin：协程
来源：http://gld.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://lvx.yj202588.top

[T12] Kotlin：解构声明
来源：http://hfd.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://bwz.ydjk.org.cn

[T13] Kotlin：只读 Map
来源：http://koc.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://drm.zhaomingkeji.xyz

[T14] Kotlin：循环
来源：http://ceh.sxryk.cn

for (i in 1..10) println(i)
来源：http://dxn.ywan-chungtsiang.top

[T15] Kotlin：接口
来源：http://zut.yfazqb.com

interface Shape { fun area(): Double }
来源：http://ubs.guowangkeji.top

[T16] Swift：Hello World
来源：http://cns.sufxvd.cn

print("Hello")
来源：http://egx.wangdashe.top

[T17] Swift：变量与常量
来源：http://loj.yanxiufei.cn

var a = 1;  let b = 2
来源：http://ruk.shuidangran.top

[T18] Swift：字符串插值
来源：http://vbp.birdmap.top

"值: \(b)"
来源：http://crl.xinyue.icu

[T19] Swift：可选绑定
来源：http://nwg.jqgfzy.top

if let n = opt { print(n) }
来源：http://coj.shanyushiyangtech.top

[T20] Swift：数组操作
来源：http://uxp.meibo888.top

var a = [1, 2, 3];  a.append(4)
来源：http://tkm.zhixingplan.top

[T21] Swift：遍历
来源：http://jgc.yuxming.cn

for x in a { print(x) }
来源：http://oxe.chenzaomai.com

[T22] Swift：字典
来源：http://fpz.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bzl.yonumen.top

[T23] Swift：函数
来源：http://pea.zhiwuduotai.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sfx.ppjwa.cn

[T24] Swift：闭包
来源：http://vlw.yj20258.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ylv.yongpay.top

[T25] Swift：结构体
来源：http://uty.dashuyun.cn

struct P { var x: Int }
来源：http://tmf.jinqigufen.top

[T26] Swift：类与重写
来源：http://fnx.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://eqo.jianghu66.top

[T27] Swift：错误处理
来源：http://tgt.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://gnx.ehwqpu.com

[T28] Swift：枚举
来源：http://ota.jinqigfzy.top

enum Color { case red, green }
来源：http://bfa.meibo888.top

[T29] Swift：guard 提前返回
来源：http://ttm.kuanghao11.cn

guard let x = opt else { return }
来源：http://vxv.shanyushiyangtech.top

[T30] Swift：协议
来源：http://xap.svipenyu.cn

protocol Shape { func area() -> Double }
来源：http://jkm.havefunace.top

[T31] Lua：Hello World
来源：http://yxk.0kj1m.cn

print("Hello")
来源：http://vye.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://pke.cqqwz.cn

local a = 1
来源：http://lrg.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://yow.daxiang520.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jrl.uphjek.com

[T34] Lua：遍历表
来源：http://snb.ydzc1.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jjv.xziqi.cn

[T35] Lua：字典表
来源：http://dwc.nanxuanxn.top

local d = { a = 1 };  d.b = 2
来源：http://xlg.sysykeji.top

[T36] Lua：函数
来源：http://kjn.cqqwz.cn

function add(a, b) return a + b end
来源：http://lpr.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://yug.xylfe.cn

"a" .. "b"
来源：http://uks.ybcxt.top

[T38] Lua：条件
来源：http://gxj.daxiang520.top

if x > 0 then print("正") end
来源：http://dcr.cucudq.cn

[T39] Lua：模式匹配
来源：http://wxe.sweek.top

string.find(s, "%d+")
来源：http://xvc.zhoulong.xyz

[T40] Lua：元表
来源：http://agi.yangfankeji.com

setmetatable({}, { __index = base })
来源：http://kjc.shanyushiyangkeji.top

[T41] Perl：Hello World
来源：http://jcz.hnxiangtu.top

print "Hello\n";
来源：http://vdp.hysaishi.cn

[T42] Perl：变量类型
来源：http://hlm.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uhh.shuidangran.top

[T43] Perl：字符串插值
来源：http://stc.sxryk.cn

"值: $a"
来源：http://rna.shangyingyoupin.top

[T44] Perl：条件
来源：http://dnu.yvedp.cn

if ($a > 0) { print "正"; }
来源：http://afc.yj20258888.top

[T45] Perl：数组遍历
来源：http://lbf.dashuyun.cn

for my $x (@arr) { print $x; }
来源：http://xao.9152youxi.cn

[T46] Perl：哈希操作
来源：http://kqm.yonumen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fll.zhiwuduotai.top

[T47] Perl：正则捕获
来源：http://not.hysaishi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rni.havefunace.top

[T48] Perl：正则替换
来源：http://fau.smart0.xyz

$s =~ s/old/new/g;
来源：http://urm.jianghu66.top

[T49] Perl：函数
来源：http://ure.fengsongda.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tvp.shuidangran.top

[T50] Perl：逐行读文件
来源：http://dpo.dianchejie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dci.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://mzi.fehbvm.com

[T51] Scala：Hello World
来源：http://mok.ydzc1.top

println("Hello")
来源：http://adq.smart0.xyz

[T52] Scala：变量
来源：http://cjl.jinqigufen.top

val a = 1;  var b = 2
来源：http://zoe.ydjk.org.cn

[T53] Scala：字符串插值
来源：http://cxq.havefunace.top

s"值: $b"
来源：http://kid.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://dcp.ywan-chungtsiang.top

List(1, 2, 3).map(_ * 2)
来源：http://ety.gzhubu.top

[T55] Scala：集合过滤
来源：http://ekl.chenjidiqi.icu

List(1, 2, 3).filter(_ > 1)
来源：http://iyi.cashguo.top

[T56] Scala：样例类
来源：http://gyt.shuidangran.top

case class User(name: String, age: Int)
来源：http://lcg.aibaodan.cn

[T57] Scala：模式匹配
来源：http://zje.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ufa.tianlin.xyz

[T58] Scala：函数定义
来源：http://csg.yvedp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kyx.nwbrower.top

[T59] Scala：循环
来源：http://xwz.shangyingyoupin.top

for (i <- 1 to 10) println(i)
来源：http://pug.hnxiangtu.top

[T60] Scala：折叠
来源：http://gud.pengpengdd.cyou

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gzz.jianghu66.top

================================================================================
来源：http://ukn.havefunace.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://deu.jlsjyb.cn

================================================================================
来源：http://mvy.zhiwuduotai.top

[U01] Py：创建虚拟环境
来源：http://mat.fengsongda.top

python -m venv .venv && source .venv/bin/activate
来源：http://sot.hesvh.cn

[U02] Py：导出 / 安装依赖
来源：http://udb.shanyushiyangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fjl.yuanzhike.top

[U03] Py：加载 .env 配置
来源：http://ppw.cashguo.top

from dotenv import load_dotenv; load_dotenv()
来源：http://paz.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://gus.vqdsnc.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yzv.shzxlz.cn

[U05] Py：列表去重且保序
来源：http://kpn.nanxinkj.top

list(dict.fromkeys(arr))
来源：http://cyo.nwbrower.top

[U06] Py：合并两个字典
来源：http://krh.ydjk.org.cn

{**a, **b}
来源：http://nct.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://vna.smart0.xyz

{v: k for k, v in d.items()}
来源：http://ica.tian-w.cn

[U08] Py：展平二维列表
来源：http://lnj.hnxiangtu.top

[y for x in nested for y in x]
来源：http://nvg.cdnleiting.top

[U09] Py：字典取最大值的键
来源：http://tna.hcnkem.com

max(d, key=d.get)
来源：http://blq.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://fma.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lun.xylfe.cn

[U11] Py：生成器表达式
来源：http://urr.ivvv.top

(x * 2 for x in arr)
来源：http://ymo.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iwh.birdmap.top

Counter(arr).most_common(3)
来源：http://qhn.cdnleiting.top

[U13] Py：固定长度队列
来源：http://hdg.havefunace.top

deque(maxlen=10)
来源：http://tyn.0kj1m.cn

[U14] Py：分组收集到列表
来源：http://fsj.kuanghao11.cn

defaultdict(list)
来源：http://cxo.smart0.xyz

[U15] Py：高精度计时
来源：http://lue.gaohongyu789.top

t = time.perf_counter()
来源：http://zwg.sxryk.cn

[U16] Py：命令行参数解析
来源：http://kuv.vqdsnc.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://owi.yuanzhike.top

[U17] Py：初始化日志
来源：http://xjk.ydjk.org.cn

logging.basicConfig(level=logging.INFO)
来源：http://yiz.xziqi.cn

[U18] Py：预编译正则
来源：http://ddo.fzhhl.top

pat = re.compile(r"\d+")
来源：http://ktk.shzxlz.cn

[U19] Py：正则替换带回调
来源：http://nvi.zhixingplan.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ydx.kuanghao11.cn

[U20] Py：缓存函数结果
来源：http://irm.ppjwa.cn

@functools.lru_cache(maxsize=None)
来源：http://rvp.fengsongda.top

[U21] Py：自定义上下文管理器
来源：http://nof.iojbl.cn

@contextlib.contextmanager
来源：http://jxa.gotoacloud.top

[U22] Py：矩阵转置
来源：http://che.ydjk.org.cn

list(zip(*m))
来源：http://ohs.mhx1999.top

[U23] Py：分块读取大文件
来源：http://mfc.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bkk.hysaishi.cn

[U24] Py：路径操作
来源：http://myc.fzhhl.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fkp.yj20258.top

[U25] Py：CSV 按字典读
来源：http://zvk.yongpay.top

csv.DictReader(f)
来源：http://ysz.jlsjyb.cn

[U26] Py：并发下载
来源：http://kgy.shanyushiyangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://met.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://rbk.9152youxi.cn

aiohttp.ClientSession() 配合 async with
来源：http://fhy.nanxinkj.top

[U28] Py：类型别名
来源：http://oga.hywenlv.cn

UserId = int
来源：http://yzm.hammf.cn

[U29] Py：属性校验
来源：http://hlz.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://eiz.jinqigfzy.top

[U30] Py：数据类
来源：http://tkp.xuetiantiany.cn

@dataclass(slots=True)
来源：http://wkb.zhoulong.xyz

[U31] Py：单测
来源：http://mnt.zhaomingkeji.xyz

python -m pytest -q
来源：http://kjb.uphjek.com

[U32] Py：代码格式化
来源：http://cms.shuidangran.top

ruff format . && ruff check --fix .
来源：http://vro.tianlin.xyz

[U33] Py：打包发布
来源：http://osv.aibaodan.cn

python -m build  （依赖 pyproject.toml）
来源：http://nso.hywenlv.cn

[U34] Py：判断编码
来源：http://cyr.hesvh.cn

chardet.detect(raw)
来源：http://nga.vqdsnc.cn

[U35] Py：发送邮件
来源：http://pug.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aje.kuanghao11.cn

[U36] Py：定时任务
来源：http://tml.hysaishi.cn

schedule.every(10).minutes.do(job)
来源：http://wef.shuidangran.top

[U37] Py：读写 Excel
来源：http://swm.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://rku.hammf.cn

[U38] Py：获取脚本所在目录
来源：http://fkk.hcnkem.com

Path(__file__).resolve().parent
来源：http://jdp.yj202588.top

[U39] Py：判断是否在交互环境
来源：http://ptk.hcnkem.com

sys.stdout.isatty()
来源：http://oxy.pengpengdd.cyou

[U40] Py：打印到标准错误
来源：http://ovz.xuetiantiany.cn

print("err", file=sys.stderr)
来源：http://orr.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://kcs.fengsongda.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cnb.snrcjt.cn

[U42] PHP：PSR-4 自动加载
来源：http://uve.52xcode.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ljd.ivvv.top

[U43] PHP：声明命名空间
来源：http://blc.nanxinkj.top

namespace App\Http;
来源：http://rpc.pycfn.com

[U44] PHP：开启严格类型
来源：http://quu.uphjek.com

declare(strict_types=1);
来源：http://eyt.nwbrower.top

[U45] PHP：类型声明与返回类型
来源：http://gqm.nanxinkj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://bmn.fengsongda.top

[U46] PHP：可空类型
来源：http://gni.dianchejie.cn

?string $name = null
来源：http://gut.vehdjk.com


<!-- 参考信息 -->