代发 wailian999

memset(a, 0, sizeof a);
来源：http://yfh.zycfv.cn

[S27] C：定义常量
来源：http://xpw.shangyingyoupin.top

const double PI = 3.14159;
来源：http://yvr.hesvh.cn

[S28] C：静态变量
来源：http://xif.jqgufenzy.top

static int counter = 0;
来源：http://nrq.iojbl.cn

[S29] C：变参函数
来源：http://hrv.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xmu.nanxuanxn.top

[S30] C：头文件保护
来源：http://myw.cashguo.top

#ifndef X_H
来源：http://lnk.zhixingplan.top

#define X_H
来源：http://ccn.tanke756.top

#endif
来源：http://geu.aizwys.cn

[S31] C++：Hello World
来源：http://pew.nwbrower.top

#include <iostream>
来源：http://csl.zhongyouzk.top

int main() { std::cout << "Hello\n"; }
来源：http://bxr.fengsongda.top

[S32] C++：字符串
来源：http://lkm.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://ttf.zhongyouzk.top

[S33] C++：vector 增删
来源：http://crl.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yzo.cdnleiting.top

[S34] C++：遍历 vector
来源：http://wup.bbcook.cn

for (auto &x : v) { std::cout << x; }
来源：http://uqf.shuidangran.top

[S35] C++：map
来源：http://oyn.xylfe.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pcp.hesvh.cn

[S36] C++：unordered_map
来源：http://ntt.havefunace.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zwn.yongpay.top

[S37] C++：set
来源：http://pok.hysaishi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://shm.yongpay.top

[S38] C++：排序
来源：http://ioa.hfpthk.cn

std::sort(v.begin(), v.end());
来源：http://lxo.tarul.cn

[S39] C++：自定义比较器排序
来源：http://raf.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xzv.yfazqb.com

[S40] C++：查找元素
来源：http://ppz.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vub.hysaishi.cn

[S41] C++：类与构造函数
来源：http://ghx.shzxlz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lrp.hesvh.cn

[S42] C++：继承与虚函数
来源：http://xst.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://rzg.jlsjyb.cn

[S43] C++：智能指针
来源：http://jgi.hesvh.cn

auto p = std::make_unique<int>(5);
来源：http://hlu.uphjek.com

[S44] C++：引用传参
来源：http://fnf.ybcxt.top

void inc(int &x) { ++x; }
来源：http://orx.hongshengwenyu.top

[S45] C++：lambda
来源：http://izg.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://hkk.pycfn.com

[S46] C++：函数模板
来源：http://zxa.jianghu66.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wer.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://rlq.gzhubu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://otm.uphjek.com

[S48] C++：逐行读文件
来源：http://hfe.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://jyz.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://ilo.zdqjudy.top

[S49] C++：写文件
来源：http://fgd.sxryk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://avb.hfpthk.cn

[S50] C++：格式化数字
来源：http://kfo.yj20258.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yeq.zhixingplan.top

[S51] C++：显式类型转换
来源：http://fcw.aibaodan.cn

static_cast<double>(a) / b
来源：http://yjt.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://sob.tian-w.cn

int size() const noexcept { return n_; }
来源：http://yso.fktsv.cn

[S53] C++：移动语义
来源：http://rjb.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://kii.smart0.xyz

[S54] C++：异常处理
来源：http://igb.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mup.shuidangran.top

[S55] C++：结构化绑定
来源：http://xxv.pycfn.com

auto [a, b] = std::make_pair(1, 2);
来源：http://bvx.jinghuilouyu.cn

[S56] C++：optional
来源：http://buu.fzhhl.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bfl.pengpengdd.cyou

[S57] C++：编译期常量
来源：http://kie.kuanghao11.cn

constexpr int N = 10;
来源：http://zkh.epnwcf.com

[S58] C++：命名空间
来源：http://ddf.nanxuanxn.top

namespace ns { int f() { return 1; } }
来源：http://gpf.shuidangran.top

[S59] C++：静态断言
来源：http://zzb.guowangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jou.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://axu.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ahu.hnqzz.top

================================================================================
来源：http://rwx.ydjk.org.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vuu.ydzc1.top

================================================================================
来源：http://obj.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://vjp.hnqzz.top

println("Hello")
来源：http://wqc.xingfuxueyuan.xyz

[T02] Kotlin：变量
来源：http://arj.kuanghao11.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ctg.birdmap.top

[T03] Kotlin：字符串模板
来源：http://lrl.zdbjq.cn

"值: $b"
来源：http://kmx.gotoacloud.top

[T04] Kotlin：空安全
来源：http://mcc.zdbjq.cn

val n: String? = null;  n?.length
来源：http://mit.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://qcm.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nwq.uphjek.com

[T06] Kotlin：集合映射
来源：http://wlw.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://xqo.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://lkf.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://buw.hywenlv.cn

[T08] Kotlin：数据类
来源：http://ond.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://bne.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://qrz.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://umv.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://ble.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://uhn.svipenyu.cn

[T11] Kotlin：协程
来源：http://obu.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lsl.quarkkingdee.top

[T12] Kotlin：解构声明
来源：http://eye.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://ops.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://kos.tian-w.cn

val m = mapOf("a" to 1)
来源：http://vlr.shangyingyoupin.top

[T14] Kotlin：循环
来源：http://yrq.xinyue.icu

for (i in 1..10) println(i)
来源：http://nma.hnxiangtu.top

[T15] Kotlin：接口
来源：http://nwd.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://bjs.hnxiangtu.top

[T16] Swift：Hello World
来源：http://rrd.c1oappe.top

print("Hello")
来源：http://crj.hongshengwenyu.top

[T17] Swift：变量与常量
来源：http://rir.cashguo.top

var a = 1;  let b = 2
来源：http://tqm.gogol.net.cn

[T18] Swift：字符串插值
来源：http://rhx.nanxuanxn.top

"值: \(b)"
来源：http://hqn.jinqigufen.top

[T19] Swift：可选绑定
来源：http://hnb.zhijiandao.cn

if let n = opt { print(n) }
来源：http://chr.birdmap.top

[T20] Swift：数组操作
来源：http://rep.ybcxt.top

var a = [1, 2, 3];  a.append(4)
来源：http://kko.tanke756.top

[T21] Swift：遍历
来源：http://ecv.zhongyouzk.top

for x in a { print(x) }
来源：http://ilb.tianlin.xyz

[T22] Swift：字典
来源：http://jpo.haohaochexian.top

var d = ["a": 1];  d["b"] = 2
来源：http://eah.chenjidiqi.icu

[T23] Swift：函数
来源：http://jgl.xuanzx.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eny.hongshengwenyu.top

[T24] Swift：闭包
来源：http://qoj.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://kaf.jiagoushi.top

[T25] Swift：结构体
来源：http://nrj.daxiang520.top

struct P { var x: Int }
来源：http://svo.andypj.xyz

[T26] Swift：类与重写
来源：http://pgh.fzhhl.top

class A: Base { override func f() {} }
来源：http://fou.ivvv.top

[T27] Swift：错误处理
来源：http://pde.hesvh.cn

do { try f() } catch { print(error) }
来源：http://waf.haohaochexian.top

[T28] Swift：枚举
来源：http://rdi.haohaochexian.top

enum Color { case red, green }
来源：http://qjc.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://tnd.yanxiufei.cn

guard let x = opt else { return }
来源：http://ssz.zycfv.cn

[T30] Swift：协议
来源：http://mum.shzxlz.cn

protocol Shape { func area() -> Double }
来源：http://rew.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://ygn.hongshengwenyu.top

print("Hello")
来源：http://ygw.jinghuilouyu.cn

[T32] Lua：局部变量
来源：http://vxu.epnwcf.com

local a = 1
来源：http://qem.ctjpmb.com

[T33] Lua：表（数组）
来源：http://cpt.52xcode.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jdv.xinyue.icu

[T34] Lua：遍历表
来源：http://ccj.nwbrower.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dji.aibaodan.cn

[T35] Lua：字典表
来源：http://ohp.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://gdi.yj20258.top

[T36] Lua：函数
来源：http://mfq.zhaomingkeji.xyz

function add(a, b) return a + b end
来源：http://bhu.mhx1999.top

[T37] Lua：字符串拼接
来源：http://xye.cdnleiting.top

"a" .. "b"
来源：http://ztv.sweek.top

[T38] Lua：条件
来源：http://sxj.shangyingyoupin.top

if x > 0 then print("正") end
来源：http://xta.hammf.cn

[T39] Lua：模式匹配
来源：http://fox.cashguo.top

string.find(s, "%d+")
来源：http://aas.vqdsnc.cn

[T40] Lua：元表
来源：http://wjg.redwolf501.top

setmetatable({}, { __index = base })
来源：http://mrk.cdnleiting.top

[T41] Perl：Hello World
来源：http://xmm.jlsjyb.cn

print "Hello\n";
来源：http://isk.yj20258888.top

[T42] Perl：变量类型
来源：http://ibe.ivvv.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jlg.wangdashe.top

[T43] Perl：字符串插值
来源：http://bwh.zdqjudy.top

"值: $a"
来源：http://hhq.sjlbkw.cn

[T44] Perl：条件
来源：http://tsi.sjlbkw.cn

if ($a > 0) { print "正"; }
来源：http://wsl.yj20258.top

[T45] Perl：数组遍历
来源：http://pvr.yj202588.top

for my $x (@arr) { print $x; }
来源：http://wtn.jinqigufen.top

[T46] Perl：哈希操作
来源：http://udy.hesvh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zzo.jiagoushi.top

[T47] Perl：正则捕获
来源：http://rbl.sysykeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://sed.jyoumei.cn

[T48] Perl：正则替换
来源：http://yfj.zhoulong.xyz

$s =~ s/old/new/g;
来源：http://fhk.yj20258.top

[T49] Perl：函数
来源：http://ffo.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uds.sweek.top

[T50] Perl：逐行读文件
来源：http://kbt.tanke756.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fkw.hammf.cn

while (my $line = <$fh>) { print $line; }
来源：http://vth.tianlin.xyz

[T51] Scala：Hello World
来源：http://ydq.wangdashe.top

println("Hello")
来源：http://ums.0kj1m.cn

[T52] Scala：变量
来源：http://jke.yuxming.cn

val a = 1;  var b = 2
来源：http://wus.zhongyouzk.top

[T53] Scala：字符串插值
来源：http://scb.c1oappe.top

s"值: $b"
来源：http://vlx.kuanghao11.cn

[T54] Scala：集合映射
来源：http://mzd.chenzaomai.com

List(1, 2, 3).map(_ * 2)
来源：http://vbt.meibo888.top

[T55] Scala：集合过滤
来源：http://kig.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://nkm.hywenlv.cn

[T56] Scala：样例类
来源：http://uqa.cashguo.top

case class User(name: String, age: Int)
来源：http://hpm.9152youxi.cn

[T57] Scala：模式匹配
来源：http://azd.jlsjyb.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rmb.zdqjudy.top

[T58] Scala：函数定义
来源：http://fad.chenzaomai.com

def add(a: Int, b: Int): Int = a + b
来源：http://xny.uphjek.com

[T59] Scala：循环
来源：http://ida.xylfe.cn

for (i <- 1 to 10) println(i)
来源：http://sxq.jinqigufen.top

[T60] Scala：折叠
来源：http://xwd.cashguo.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aej.zhongyouzk.top

================================================================================
来源：http://vmy.hcnkem.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nto.tanke756.top

================================================================================
来源：http://rgj.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://mjr.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://rlk.jinyuanbaomall.cn

[U02] Py：导出 / 安装依赖
来源：http://ixy.jyoumei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://amu.uphjek.com

[U03] Py：加载 .env 配置
来源：http://prz.shangyingyoupin.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qrs.bjfxy.top

[U04] Py：变量调试打印
来源：http://fps.yj20258.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wic.epnwcf.com

[U05] Py：列表去重且保序
来源：http://akt.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://enq.tanke756.top

[U06] Py：合并两个字典
来源：http://rjs.jqgufenzy.top

{**a, **b}
来源：http://ppx.316326.xyz

[U07] Py：反转字典键值
来源：http://yss.316326.xyz

{v: k for k, v in d.items()}
来源：http://rgt.xuetiantiany.cn

[U08] Py：展平二维列表
来源：http://vxe.pengpengdd.cyou

[y for x in nested for y in x]
来源：http://uso.yueranfly.top

[U09] Py：字典取最大值的键
来源：http://ljb.redwolf501.top

max(d, key=d.get)
来源：http://tet.tianlin.xyz

[U10] Py：按值排序字典
来源：http://nyh.sjlbkw.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ual.redwolf501.top

[U11] Py：生成器表达式
来源：http://uvz.shangyingyoupin.top

(x * 2 for x in arr)
来源：http://pgx.yvedp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://igv.shuidangran.top

Counter(arr).most_common(3)
来源：http://qmf.jinyuanbaomall.cn

[U13] Py：固定长度队列
来源：http://aig.guowangkeji.top

deque(maxlen=10)
来源：http://zna.tian-w.cn

[U14] Py：分组收集到列表
来源：http://liq.hnqzz.top

defaultdict(list)
来源：http://lul.zdqjudy.top

[U15] Py：高精度计时
来源：http://qnm.bjfxy.top

t = time.perf_counter()
来源：http://vdg.cucudq.cn

[U16] Py：命令行参数解析
来源：http://bet.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ivw.shangyingyoupin.top

[U17] Py：初始化日志
来源：http://bgx.ctjpmb.com

logging.basicConfig(level=logging.INFO)
来源：http://zbh.jqgufenzy.top

[U18] Py：预编译正则
来源：http://yjw.guannengcc.top

pat = re.compile(r"\d+")
来源：http://rxy.nanxuanxn.top

[U19] Py：正则替换带回调
来源：http://rcw.jianghu66.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ggh.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://qfg.shuidangran.top

@functools.lru_cache(maxsize=None)
来源：http://fws.chenzaomai.com

[U21] Py：自定义上下文管理器
来源：http://rkw.cheryme.top

@contextlib.contextmanager
来源：http://qfc.xuetiantiany.cn

[U22] Py：矩阵转置
来源：http://heh.xziqi.cn

list(zip(*m))
来源：http://mhj.jianghu66.top

[U23] Py：分块读取大文件
来源：http://lri.cashguo.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nmy.shuidangran.top

[U24] Py：路径操作
来源：http://wcf.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ylj.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://tub.yj202588.top

csv.DictReader(f)
来源：http://qfy.hesvh.cn

[U26] Py：并发下载
来源：http://hxw.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gww.jiagoushi.top

[U27] Py：异步 HTTP
来源：http://sqp.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://nql.bjfxy.top

[U28] Py：类型别名
来源：http://xbu.cucudq.cn

UserId = int
来源：http://afp.shanyushiyangkeji.top

[U29] Py：属性校验
来源：http://sye.hywenlv.cn

@property 与 @x.setter 配合
来源：http://ggs.gogol.net.cn

[U30] Py：数据类
来源：http://cxt.xingfuxueyuan.xyz

@dataclass(slots=True)
来源：http://pwz.yj202588.top

[U31] Py：单测
来源：http://xdt.sweek.top

python -m pytest -q
来源：http://jik.hysaishi.cn

[U32] Py：代码格式化
来源：http://icq.yonumen.top

ruff format . && ruff check --fix .
来源：http://mia.ppjwa.cn

[U33] Py：打包发布
来源：http://ktc.wangshuangyany.cn

python -m build  （依赖 pyproject.toml）
来源：http://nfc.ydzc1.top

[U34] Py：判断编码
来源：http://hqw.sweek.top

chardet.detect(raw)
来源：http://ssw.kuanghao11.cn

[U35] Py：发送邮件
来源：http://ydu.fengsongda.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xrx.yanxiufei.cn

[U36] Py：定时任务
来源：http://tbh.feifeiyinyue.top

schedule.every(10).minutes.do(job)
来源：http://nwg.xinyue.icu

[U37] Py：读写 Excel
来源：http://tlp.smart0.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://hgt.ppjwa.cn

[U38] Py：获取脚本所在目录
来源：http://afx.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://azm.yvedp.cn

[U39] Py：判断是否在交互环境
来源：http://smr.ehwqpu.com

sys.stdout.isatty()
来源：http://lxa.tian-w.cn

[U40] Py：打印到标准错误
来源：http://avn.daxiang520.top

print("err", file=sys.stderr)
来源：http://gzt.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://mwt.jianghu66.top

composer init;  composer require guzzlehttp/guzzle
来源：http://paf.cqqwz.cn

[U42] PHP：PSR-4 自动加载
来源：http://hac.fanxiaobao.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://udv.yuxming.cn

[U43] PHP：声明命名空间
来源：http://otk.xylfe.cn

namespace App\Http;
来源：http://vdn.shanyushiyangkeji.top

[U44] PHP：开启严格类型
来源：http://txj.ywan-chungtsiang.top

declare(strict_types=1);
来源：http://rzx.gotoacloud.top

[U45] PHP：类型声明与返回类型
来源：http://yma.hysaishi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ixh.xingfuxueyuan.xyz

[U46] PHP：可空类型
来源：http://wuh.dianchejie.cn

?string $name = null
来源：http://tzu.tianlin.xyz

[U47] PHP：联合类型
来源：http://bgl.zdbjq.cn

int|string $id
来源：http://vab.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://jlh.yonumen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vic.zdqjudy.top

[U49] PHP：只读属性
来源：http://ftm.gotoacloud.top

public readonly string $name
来源：http://tny.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://kzy.xziqi.cn

public function __construct(private int $id) {}
来源：http://osc.sysykeji.top


<!-- 参考信息 -->