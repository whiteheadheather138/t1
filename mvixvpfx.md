代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aju.aizwys.cn

[S25] C：内存拷贝
来源：http://qwg.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://txn.guowangkeji.top

[S26] C：内存清零
来源：http://rgq.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://ryj.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://gur.svipenyu.cn

const double PI = 3.14159;
来源：http://naa.xinyue.icu

[S28] C：静态变量
来源：http://lue.xingfuxueyuan.xyz

static int counter = 0;
来源：http://ejk.tianlin.xyz

[S29] C：变参函数
来源：http://nde.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aci.yvedp.cn

[S30] C：头文件保护
来源：http://qkl.jyoumei.cn

#ifndef X_H
来源：http://lcy.yvedp.cn

#define X_H
来源：http://kvw.wangdashe.top

#endif
来源：http://pbz.jqgufenzy.top

[S31] C++：Hello World
来源：http://cty.tanke756.top

#include <iostream>
来源：http://evs.aizwys.cn

int main() { std::cout << "Hello\n"; }
来源：http://klv.zhixingplan.top

[S32] C++：字符串
来源：http://gmn.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://zpq.bjfxy.top

[S33] C++：vector 增删
来源：http://ayt.tianlin.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pfh.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://fos.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://qvz.shzxlz.cn

[S35] C++：map
来源：http://evy.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ogf.vehdjk.com

[S36] C++：unordered_map
来源：http://awu.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kty.ctjpmb.com

[S37] C++：set
来源：http://wyy.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xes.316326.xyz

[S38] C++：排序
来源：http://umo.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://uip.yvedp.cn

[S39] C++：自定义比较器排序
来源：http://pot.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iie.0kj1m.cn

[S40] C++：查找元素
来源：http://iwt.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jrn.sufxvd.cn

[S41] C++：类与构造函数
来源：http://mwk.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sha.hammf.cn

[S42] C++：继承与虚函数
来源：http://tsu.epnwcf.com

class B : public Base { public: void f() override {} };
来源：http://ibn.meibo888.top

[S43] C++：智能指针
来源：http://xrw.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://blh.cqqwz.cn

[S44] C++：引用传参
来源：http://wkm.zycfv.cn

void inc(int &x) { ++x; }
来源：http://ldx.yfazqb.com

[S45] C++：lambda
来源：http://kwr.jyoumei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tao.chenlongwang.top

[S46] C++：函数模板
来源：http://cha.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wfv.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://yiy.tanke756.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kuv.smart0.xyz

[S48] C++：逐行读文件
来源：http://tzi.yj20258.top

std::ifstream in("a.txt");  std::string line;
来源：http://xae.havefunace.top

while (std::getline(in, line)) { }
来源：http://oia.vehdjk.com

[S49] C++：写文件
来源：http://ikj.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tpi.yongpay.top

[S50] C++：格式化数字
来源：http://oyk.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qdp.tian-w.cn

[S51] C++：显式类型转换
来源：http://qsf.hfpthk.cn

static_cast<double>(a) / b
来源：http://fjs.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://dxp.xziqi.cn

int size() const noexcept { return n_; }
来源：http://kdx.yanxiufei.cn

[S53] C++：移动语义
来源：http://fgm.52xcode.cn

std::vector<int> w = std::move(v);
来源：http://raf.xinyue.icu

[S54] C++：异常处理
来源：http://ztb.daxiang520.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aem.sysykeji.top

[S55] C++：结构化绑定
来源：http://lkj.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://npy.gaohongyu789.top

[S56] C++：optional
来源：http://hek.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ktx.ydjk.org.cn

[S57] C++：编译期常量
来源：http://euw.yanxiufei.cn

constexpr int N = 10;
来源：http://hpk.ywan-chungtsiang.top

[S58] C++：命名空间
来源：http://evb.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://kgm.jqgfzy.top

[S59] C++：静态断言
来源：http://rsk.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://agh.vehdjk.com

[S60] C++：遍历并删除元素
来源：http://kys.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yis.havefunace.top

================================================================================
来源：http://emr.xinyue.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kon.jinghuilouyu.cn

================================================================================
来源：http://nme.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://cks.jiagoushi.top

println("Hello")
来源：http://isx.0kj1m.cn

[T02] Kotlin：变量
来源：http://qrs.xuanzx.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fbw.havefunace.top

[T03] Kotlin：字符串模板
来源：http://xqq.zhixingplan.top

"值: $b"
来源：http://voj.9152youxi.cn

[T04] Kotlin：空安全
来源：http://cng.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://ekz.epnwcf.com

[T05] Kotlin：when 表达式
来源：http://cbw.sxryk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mhd.havefunace.top

[T06] Kotlin：集合映射
来源：http://vaj.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://diz.uphjek.com

[T07] Kotlin：集合过滤
来源：http://dcr.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vhn.hammf.cn

[T08] Kotlin：数据类
来源：http://sej.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://mwf.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://ufi.gaohongyu789.top

fun String.exclaim() = this + "!"
来源：http://cxp.meibo888.top

[T10] Kotlin：默认参数
来源：http://qbp.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bvm.wangdashe.top

[T11] Kotlin：协程
来源：http://urn.hongshengwenyu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ieb.yongpay.top

[T12] Kotlin：解构声明
来源：http://nvf.fengsongda.top

val (a, b) = Pair(1, 2)
来源：http://uum.kuanghao11.cn

[T13] Kotlin：只读 Map
来源：http://bvf.sysykeji.top

val m = mapOf("a" to 1)
来源：http://rda.jianghu66.top

[T14] Kotlin：循环
来源：http://qfe.zhixingplan.top

for (i in 1..10) println(i)
来源：http://wxn.tanke756.top

[T15] Kotlin：接口
来源：http://bsh.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://oco.316326.xyz

[T16] Swift：Hello World
来源：http://wei.aibaodan.cn

print("Hello")
来源：http://qyg.ydjk.org.cn

[T17] Swift：变量与常量
来源：http://sib.jinghuilouyu.cn

var a = 1;  let b = 2
来源：http://tub.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://yxm.ivvv.top

"值: \(b)"
来源：http://nxp.ybcxt.top

[T19] Swift：可选绑定
来源：http://uiz.ydjk.org.cn

if let n = opt { print(n) }
来源：http://tuv.cashguo.top

[T20] Swift：数组操作
来源：http://cqr.c1oappe.top

var a = [1, 2, 3];  a.append(4)
来源：http://gvy.havefunace.top

[T21] Swift：遍历
来源：http://bhg.smart0.xyz

for x in a { print(x) }
来源：http://pyp.ppjwa.cn

[T22] Swift：字典
来源：http://lub.jqgufenzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://mpb.daria6918.cn

[T23] Swift：函数
来源：http://hus.zhaomingkeji.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wol.cheryme.top

[T24] Swift：闭包
来源：http://jbe.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yxv.zhixingplan.top

[T25] Swift：结构体
来源：http://ehc.ywan-chungtsiang.top

struct P { var x: Int }
来源：http://cll.guannengcc.top

[T26] Swift：类与重写
来源：http://etx.nanxuanxn.top

class A: Base { override func f() {} }
来源：http://bja.bjfxy.top

[T27] Swift：错误处理
来源：http://bhm.jiagoushi.top

do { try f() } catch { print(error) }
来源：http://awo.kuanghao11.cn

[T28] Swift：枚举
来源：http://fly.zdqjudy.top

enum Color { case red, green }
来源：http://woz.sysykeji.top

[T29] Swift：guard 提前返回
来源：http://xzk.gaohongyu789.top

guard let x = opt else { return }
来源：http://okm.wangshuangyany.cn

[T30] Swift：协议
来源：http://hth.meibo888.top

protocol Shape { func area() -> Double }
来源：http://fmg.guannengcc.top

[T31] Lua：Hello World
来源：http://odj.tanke756.top

print("Hello")
来源：http://apl.yj20258888.top

[T32] Lua：局部变量
来源：http://vmh.havefunace.top

local a = 1
来源：http://zyl.yuanzhike.top

[T33] Lua：表（数组）
来源：http://bgq.jyoumei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://orq.zdbjq.cn

[T34] Lua：遍历表
来源：http://ykr.ppjwa.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pyk.nanxuanxn.top

[T35] Lua：字典表
来源：http://pcw.feifeiyinyue.top

local d = { a = 1 };  d.b = 2
来源：http://xdx.yanxiufei.cn

[T36] Lua：函数
来源：http://ivp.snrcjt.cn

function add(a, b) return a + b end
来源：http://rsp.daxiang520.top

[T37] Lua：字符串拼接
来源：http://eqc.zhoulong.xyz

"a" .. "b"
来源：http://xqn.fktsv.cn

[T38] Lua：条件
来源：http://lft.iojbl.cn

if x > 0 then print("正") end
来源：http://rul.sweek.top

[T39] Lua：模式匹配
来源：http://xgi.wangdashe.top

string.find(s, "%d+")
来源：http://yej.316326.xyz

[T40] Lua：元表
来源：http://enx.quarkkingdee.top

setmetatable({}, { __index = base })
来源：http://pst.shzxlz.cn

[T41] Perl：Hello World
来源：http://mfp.0kj1m.cn

print "Hello\n";
来源：http://oem.snrcjt.cn

[T42] Perl：变量类型
来源：http://pnf.meibo888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dzy.9152youxi.cn

[T43] Perl：字符串插值
来源：http://men.yfazqb.com

"值: $a"
来源：http://dib.fehbvm.com

[T44] Perl：条件
来源：http://kdf.hesvh.cn

if ($a > 0) { print "正"; }
来源：http://bge.gzhubu.top

[T45] Perl：数组遍历
来源：http://fuh.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://cnv.guowangkeji.top

[T46] Perl：哈希操作
来源：http://mdk.guannengcc.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hvc.gogol.net.cn

[T47] Perl：正则捕获
来源：http://zml.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://cfa.cqqwz.cn

[T48] Perl：正则替换
来源：http://pho.daxiang520.top

$s =~ s/old/new/g;
来源：http://foo.jinqigfzy.top

[T49] Perl：函数
来源：http://djy.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zzu.aizwys.cn

[T50] Perl：逐行读文件
来源：http://pww.xinyue.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://qqy.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://rrm.kuanghao11.cn

[T51] Scala：Hello World
来源：http://lbt.zhoulong.xyz

println("Hello")
来源：http://oog.ywan-chungtsiang.top

[T52] Scala：变量
来源：http://pvq.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://wuf.iojbl.cn

[T53] Scala：字符串插值
来源：http://vkx.havefunace.top

s"值: $b"
来源：http://srl.jinyuanbaomall.cn

[T54] Scala：集合映射
来源：http://duh.cashguo.top

List(1, 2, 3).map(_ * 2)
来源：http://jos.yangfankeji.com

[T55] Scala：集合过滤
来源：http://kpi.zhoulong.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://uac.hnxiangtu.top

[T56] Scala：样例类
来源：http://kge.zdqjudy.top

case class User(name: String, age: Int)
来源：http://iho.dashuyun.cn

[T57] Scala：模式匹配
来源：http://muu.sysykeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rir.sweek.top

[T58] Scala：函数定义
来源：http://sbi.hywenlv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://olq.aizwys.cn

[T59] Scala：循环
来源：http://eyx.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://hfp.hnxiangtu.top

[T60] Scala：折叠
来源：http://faf.iojbl.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vju.jqgufenzy.top

================================================================================
来源：http://ksw.hywenlv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bow.kuanghao11.cn

================================================================================
来源：http://uqh.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://cmy.wangdashe.top

python -m venv .venv && source .venv/bin/activate
来源：http://aop.cdnleiting.top

[U02] Py：导出 / 安装依赖
来源：http://ijc.mhx1999.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hpm.shanyushiyangtech.top

[U03] Py：加载 .env 配置
来源：http://jkc.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xce.zdqjudy.top

[U04] Py：变量调试打印
来源：http://cqx.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yyb.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://pbv.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://yyo.andypj.xyz

[U06] Py：合并两个字典
来源：http://uat.zhixingplan.top

{**a, **b}
来源：http://ylh.hywenlv.cn

[U07] Py：反转字典键值
来源：http://zdi.yanxiufei.cn

{v: k for k, v in d.items()}
来源：http://ogd.daria6918.cn

[U08] Py：展平二维列表
来源：http://tyt.sysykeji.top

[y for x in nested for y in x]
来源：http://qaa.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://yiu.meibo888.top

max(d, key=d.get)
来源：http://qaj.yfazqb.com

[U10] Py：按值排序字典
来源：http://jdb.jyoumei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lvu.jianghu66.top

[U11] Py：生成器表达式
来源：http://vmh.cucudq.cn

(x * 2 for x in arr)
来源：http://fuf.chenlongwang.top

[U12] Py：取出现最多的 3 个元素
来源：http://oax.ybcxt.top

Counter(arr).most_common(3)
来源：http://ssb.cqqwz.cn

[U13] Py：固定长度队列
来源：http://pjy.zycfv.cn

deque(maxlen=10)
来源：http://atk.xingfuxueyuan.xyz

[U14] Py：分组收集到列表
来源：http://bit.ctjpmb.com

defaultdict(list)
来源：http://cjd.feifeiyinyue.top

[U15] Py：高精度计时
来源：http://mdk.jlsjyb.cn

t = time.perf_counter()
来源：http://urt.aizwys.cn

[U16] Py：命令行参数解析
来源：http://zdr.tanke756.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://puk.ctjpmb.com

[U17] Py：初始化日志
来源：http://wtr.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://cxt.jinqigufen.top

[U18] Py：预编译正则
来源：http://ruf.xuanzx.com

pat = re.compile(r"\d+")
来源：http://mie.bjfxy.top

[U19] Py：正则替换带回调
来源：http://ddv.havefunace.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ayq.bjfxy.top

[U20] Py：缓存函数结果
来源：http://wgc.snrcjt.cn

@functools.lru_cache(maxsize=None)
来源：http://cqs.nanxuanxn.top

[U21] Py：自定义上下文管理器
来源：http://dff.chenlongwang.top

@contextlib.contextmanager
来源：http://gsi.xylfe.cn

[U22] Py：矩阵转置
来源：http://bfj.uphjek.com

list(zip(*m))
来源：http://kky.jqgufenzy.top

[U23] Py：分块读取大文件
来源：http://mts.yangfankeji.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uyl.sufxvd.cn

[U24] Py：路径操作
来源：http://mzt.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lzi.chenjidiqi.icu

[U25] Py：CSV 按字典读
来源：http://oht.hnxiangtu.top

csv.DictReader(f)
来源：http://wpj.316326.xyz

[U26] Py：并发下载
来源：http://quy.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bcz.xylfe.cn

[U27] Py：异步 HTTP
来源：http://low.jlsjyb.cn

aiohttp.ClientSession() 配合 async with
来源：http://dhh.kuanghao11.cn

[U28] Py：类型别名
来源：http://agy.haohaochexian.top

UserId = int
来源：http://lte.gaohongyu789.top

[U29] Py：属性校验
来源：http://ubf.aizwys.cn

@property 与 @x.setter 配合
来源：http://zoa.ppjwa.cn

[U30] Py：数据类
来源：http://gdi.gogol.net.cn

@dataclass(slots=True)
来源：http://ktv.fktsv.cn

[U31] Py：单测
来源：http://qtu.gotoacloud.top

python -m pytest -q
来源：http://xpn.quarkkingdee.top

[U32] Py：代码格式化
来源：http://esn.birdmap.top

ruff format . && ruff check --fix .
来源：http://ygy.andypj.xyz

[U33] Py：打包发布
来源：http://jbp.zhongyouzk.top

python -m build  （依赖 pyproject.toml）
来源：http://vzn.ybcxt.top

[U34] Py：判断编码
来源：http://ggz.jinqigufen.top

chardet.detect(raw)
来源：http://mks.jlsjyb.cn

[U35] Py：发送邮件
来源：http://pgy.ppjwa.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fjs.xinyue.icu

[U36] Py：定时任务
来源：http://qlx.yangfankeji.com

schedule.every(10).minutes.do(job)
来源：http://ovy.yangfankeji.com

[U37] Py：读写 Excel
来源：http://szb.tian-w.cn

pandas.read_excel / DataFrame.to_excel
来源：http://szl.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://lov.sufxvd.cn

Path(__file__).resolve().parent
来源：http://rbx.feifeiyinyue.top

[U39] Py：判断是否在交互环境
来源：http://ggs.aibaodan.cn

sys.stdout.isatty()
来源：http://mim.nanxinkj.top

[U40] Py：打印到标准错误
来源：http://olx.cashguo.top

print("err", file=sys.stderr)
来源：http://uqb.nanxinkj.top

[U41] PHP：初始化 Composer 项目
来源：http://jam.yonumen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bst.jiagoushi.top

[U42] PHP：PSR-4 自动加载
来源：http://nef.zhongyouzk.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mrs.shuidangran.top

[U43] PHP：声明命名空间
来源：http://aph.jinqigufen.top

namespace App\Http;
来源：http://jrx.uphjek.com

[U44] PHP：开启严格类型
来源：http://egd.gzhubu.top

declare(strict_types=1);
来源：http://uzi.yvedp.cn

[U45] PHP：类型声明与返回类型
来源：http://atv.hammf.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fyx.chenjidiqi.icu

[U46] PHP：可空类型
来源：http://ebj.bbcook.cn

?string $name = null
来源：http://gfc.yanxiufei.cn

[U47] PHP：联合类型
来源：http://xlg.sysykeji.top

int|string $id
来源：http://cwu.tianlin.xyz

[U48] PHP：纯枚举
来源：http://pko.zdqjudy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pso.hongshengwenyu.top


<!-- 参考信息 -->