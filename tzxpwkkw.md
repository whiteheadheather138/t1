代发 wailian999

memset(a, 0, sizeof a);
来源：http://uva.aibaodan.cn

[S27] C：定义常量
来源：http://kbf.haohaochexian.top

const double PI = 3.14159;
来源：http://mqc.sweek.top

[S28] C：静态变量
来源：http://hlb.fanxiaobao.xyz

static int counter = 0;
来源：http://oqb.fengsongda.top

[S29] C：变参函数
来源：http://eew.cashguo.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ppo.yvedp.cn

[S30] C：头文件保护
来源：http://oub.vehdjk.com

#ifndef X_H
来源：http://ede.guowangkeji.top

#define X_H
来源：http://bml.yanxiufei.cn

#endif
来源：http://daj.yanxiufei.cn

[S31] C++：Hello World
来源：http://imv.fktsv.cn

#include <iostream>
来源：http://xbm.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://npy.xuetiantiany.cn

[S32] C++：字符串
来源：http://mnt.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://xad.xziqi.cn

[S33] C++：vector 增删
来源：http://hcl.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aya.redwolf501.top

[S34] C++：遍历 vector
来源：http://hmp.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://fuy.hnqzz.top

[S35] C++：map
来源：http://rgn.kuanghao11.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nqn.nanxinkj.top

[S36] C++：unordered_map
来源：http://bdi.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ebv.c1oappe.top

[S37] C++：set
来源：http://ljq.hongshengwenyu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xlr.0kj1m.cn

[S38] C++：排序
来源：http://ewy.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://tmg.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://srh.yvedp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cun.pengpengdd.cyou

[S40] C++：查找元素
来源：http://asu.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sjc.daxiang520.top

[S41] C++：类与构造函数
来源：http://wti.gogol.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://igh.c1oappe.top

[S42] C++：继承与虚函数
来源：http://ndw.jqgufenzy.top

class B : public Base { public: void f() override {} };
来源：http://wtv.uphjek.com

[S43] C++：智能指针
来源：http://xww.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://atb.hnxiangtu.top

[S44] C++：引用传参
来源：http://dwk.gogol.net.cn

void inc(int &x) { ++x; }
来源：http://xvg.sysykeji.top

[S45] C++：lambda
来源：http://kqr.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://hgs.hongshengwenyu.top

[S46] C++：函数模板
来源：http://wuj.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uno.yangfankeji.com

[S47] C++：结构化绑定遍历
来源：http://ack.tanke756.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xgo.jiagoushi.top

[S48] C++：逐行读文件
来源：http://tjn.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pol.xingfuxueyuan.xyz

while (std::getline(in, line)) { }
来源：http://avg.52xcode.cn

[S49] C++：写文件
来源：http://fxj.zhijiandao.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xox.yueranfly.top

[S50] C++：格式化数字
来源：http://zlj.yongpay.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tdy.pycfn.com

[S51] C++：显式类型转换
来源：http://wqj.tarul.cn

static_cast<double>(a) / b
来源：http://vok.sufxvd.cn

[S52] C++：const 与 noexcept
来源：http://soh.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://hdm.fktsv.cn

[S53] C++：移动语义
来源：http://nvt.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://fjq.yvedp.cn

[S54] C++：异常处理
来源：http://eci.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ijg.xingfuxueyuan.xyz

[S55] C++：结构化绑定
来源：http://jpr.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://irs.hywenlv.cn

[S56] C++：optional
来源：http://vsf.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xsp.shanyushiyangkeji.top

[S57] C++：编译期常量
来源：http://yvp.fengsongda.top

constexpr int N = 10;
来源：http://hmz.nwbrower.top

[S58] C++：命名空间
来源：http://djj.0kj1m.cn

namespace ns { int f() { return 1; } }
来源：http://ert.guannengcc.top

[S59] C++：静态断言
来源：http://diw.9152youxi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jjp.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://rqt.jianghu66.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lmh.wangshuangyany.cn

================================================================================
来源：http://fsa.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wmu.meibo888.top

================================================================================
来源：http://axz.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://fce.sjlbkw.cn

println("Hello")
来源：http://laa.fehbvm.com

[T02] Kotlin：变量
来源：http://xvq.jlsjyb.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://irh.yj20258.top

[T03] Kotlin：字符串模板
来源：http://rsh.hammf.cn

"值: $b"
来源：http://dtp.chenlongwang.top

[T04] Kotlin：空安全
来源：http://mjc.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://ppo.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://bvs.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ypz.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://syr.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rmy.cheryme.top

[T07] Kotlin：集合过滤
来源：http://xzv.feifeiyinyue.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nxx.xuetiantiany.cn

[T08] Kotlin：数据类
来源：http://pno.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://xcl.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://rhe.cqqwz.cn

fun String.exclaim() = this + "!"
来源：http://cci.zhoulong.xyz

[T10] Kotlin：默认参数
来源：http://cwm.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dpp.mhx1999.top

[T11] Kotlin：协程
来源：http://twp.redwolf501.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wtk.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://bju.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://msh.zhoulong.xyz

[T13] Kotlin：只读 Map
来源：http://ith.nanxuanxn.top

val m = mapOf("a" to 1)
来源：http://sdl.quarkkingdee.top

[T14] Kotlin：循环
来源：http://gaw.jqgfzy.top

for (i in 1..10) println(i)
来源：http://btn.iojbl.cn

[T15] Kotlin：接口
来源：http://zmd.gotoacloud.top

interface Shape { fun area(): Double }
来源：http://wey.fehbvm.com

[T16] Swift：Hello World
来源：http://xux.jinyuanbaomall.cn

print("Hello")
来源：http://dmr.yuanzhike.top

[T17] Swift：变量与常量
来源：http://qju.gotoacloud.top

var a = 1;  let b = 2
来源：http://qix.wangdashe.top

[T18] Swift：字符串插值
来源：http://flr.jinqigufen.top

"值: \(b)"
来源：http://qmx.yfazqb.com

[T19] Swift：可选绑定
来源：http://stj.mhx1999.top

if let n = opt { print(n) }
来源：http://xhx.sufxvd.cn

[T20] Swift：数组操作
来源：http://ymc.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://lug.meibo888.top

[T21] Swift：遍历
来源：http://slc.cqqwz.cn

for x in a { print(x) }
来源：http://jsv.cucudq.cn

[T22] Swift：字典
来源：http://inw.epnwcf.com

var d = ["a": 1];  d["b"] = 2
来源：http://use.hfpthk.cn

[T23] Swift：函数
来源：http://cme.yj20258.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://osi.snrcjt.cn

[T24] Swift：闭包
来源：http://nac.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://uyc.tanke756.top

[T25] Swift：结构体
来源：http://dwf.0kj1m.cn

struct P { var x: Int }
来源：http://spp.xinyue.icu

[T26] Swift：类与重写
来源：http://sms.ehwqpu.com

class A: Base { override func f() {} }
来源：http://wpo.nwbrower.top

[T27] Swift：错误处理
来源：http://ydp.xuanzx.com

do { try f() } catch { print(error) }
来源：http://cue.jqgufenzy.top

[T28] Swift：枚举
来源：http://sum.hesvh.cn

enum Color { case red, green }
来源：http://bby.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://spa.zhengqikj.top

guard let x = opt else { return }
来源：http://dth.bbcook.cn

[T30] Swift：协议
来源：http://pfr.hnxiangtu.top

protocol Shape { func area() -> Double }
来源：http://zvt.zhixingplan.top

[T31] Lua：Hello World
来源：http://zfe.yj20258.top

print("Hello")
来源：http://bnu.zhoulong.xyz

[T32] Lua：局部变量
来源：http://bbb.redwolf501.top

local a = 1
来源：http://haa.yangfankeji.com

[T33] Lua：表（数组）
来源：http://soj.hesvh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ake.redwolf501.top

[T34] Lua：遍历表
来源：http://cxe.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://suu.snrcjt.cn

[T35] Lua：字典表
来源：http://ksh.daxiang520.top

local d = { a = 1 };  d.b = 2
来源：http://dss.xylfe.cn

[T36] Lua：函数
来源：http://djx.yongpay.top

function add(a, b) return a + b end
来源：http://xwm.pengpengdd.cyou

[T37] Lua：字符串拼接
来源：http://tfr.sysykeji.top

"a" .. "b"
来源：http://qjf.smart0.xyz

[T38] Lua：条件
来源：http://fsb.ydzc1.top

if x > 0 then print("正") end
来源：http://jcd.yvedp.cn

[T39] Lua：模式匹配
来源：http://vyk.nwbrower.top

string.find(s, "%d+")
来源：http://jsz.chenlongwang.top

[T40] Lua：元表
来源：http://jwp.iojbl.cn

setmetatable({}, { __index = base })
来源：http://tmi.shzxlz.cn

[T41] Perl：Hello World
来源：http://yob.yonumen.top

print "Hello\n";
来源：http://rhb.cashguo.top

[T42] Perl：变量类型
来源：http://kui.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fyf.cucudq.cn

[T43] Perl：字符串插值
来源：http://vot.cucudq.cn

"值: $a"
来源：http://hwj.meibo888.top

[T44] Perl：条件
来源：http://qpx.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://upn.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://lxp.shzxlz.cn

for my $x (@arr) { print $x; }
来源：http://apw.daxiang520.top

[T46] Perl：哈希操作
来源：http://mdi.redwolf501.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eug.yueranfly.top

[T47] Perl：正则捕获
来源：http://qvk.ydjk.org.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://szm.mhx1999.top

[T48] Perl：正则替换
来源：http://idr.zycfv.cn

$s =~ s/old/new/g;
来源：http://mab.sxryk.cn

[T49] Perl：函数
来源：http://ixv.jqgufenzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qio.chenjidiqi.icu

[T50] Perl：逐行读文件
来源：http://pgr.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://czp.tian-w.cn

while (my $line = <$fh>) { print $line; }
来源：http://eui.uphjek.com

[T51] Scala：Hello World
来源：http://iat.meibo888.top

println("Hello")
来源：http://gsp.daria6918.cn

[T52] Scala：变量
来源：http://afm.xingfuxueyuan.xyz

val a = 1;  var b = 2
来源：http://omd.jinghuilouyu.cn

[T53] Scala：字符串插值
来源：http://bdw.kuanghao11.cn

s"值: $b"
来源：http://gmx.xuanzx.com

[T54] Scala：集合映射
来源：http://pfg.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://bnw.wangshuangyany.cn

[T55] Scala：集合过滤
来源：http://wvo.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hzl.yuanzhike.top

[T56] Scala：样例类
来源：http://ete.jianghu66.top

case class User(name: String, age: Int)
来源：http://kjo.jqgfzy.top

[T57] Scala：模式匹配
来源：http://rzg.shanyushiyangtech.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kwh.aizwys.cn

[T58] Scala：函数定义
来源：http://zof.shanyushiyangtech.top

def add(a: Int, b: Int): Int = a + b
来源：http://yji.dashuyun.cn

[T59] Scala：循环
来源：http://bqu.ctjpmb.com

for (i <- 1 to 10) println(i)
来源：http://phs.wangdashe.top

[T60] Scala：折叠
来源：http://dqa.yj20258888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://thx.xingfuxueyuan.xyz

================================================================================
来源：http://uxo.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rbx.jinyuanbaomall.cn

================================================================================
来源：http://dti.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://nwx.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://vlc.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://wry.chenjidiqi.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oyg.cqqwz.cn

[U03] Py：加载 .env 配置
来源：http://lsi.xziqi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bxk.yfazqb.com

[U04] Py：变量调试打印
来源：http://qxj.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://biu.yuxming.cn

[U05] Py：列表去重且保序
来源：http://rye.zhixingplan.top

list(dict.fromkeys(arr))
来源：http://eum.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://tbk.tianlin.xyz

{**a, **b}
来源：http://rob.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://idv.cheryme.top

{v: k for k, v in d.items()}
来源：http://afx.hnqzz.top

[U08] Py：展平二维列表
来源：http://ynd.cucudq.cn

[y for x in nested for y in x]
来源：http://yrd.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://daw.andypj.xyz

max(d, key=d.get)
来源：http://ekz.iojbl.cn

[U10] Py：按值排序字典
来源：http://hyn.ywan-chungtsiang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://amb.hnqzz.top

[U11] Py：生成器表达式
来源：http://suz.sjlbkw.cn

(x * 2 for x in arr)
来源：http://qsw.sweek.top

[U12] Py：取出现最多的 3 个元素
来源：http://owm.vehdjk.com

Counter(arr).most_common(3)
来源：http://nby.nanxinkj.top

[U13] Py：固定长度队列
来源：http://emt.mhx1999.top

deque(maxlen=10)
来源：http://rye.52xcode.cn

[U14] Py：分组收集到列表
来源：http://kku.shangyingyoupin.top

defaultdict(list)
来源：http://ijc.zhoulong.xyz

[U15] Py：高精度计时
来源：http://edh.shangyingyoupin.top

t = time.perf_counter()
来源：http://mam.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://les.jinyuanbaomall.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qiw.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://udf.ywan-chungtsiang.top

logging.basicConfig(level=logging.INFO)
来源：http://tlh.shangyingyoupin.top

[U18] Py：预编译正则
来源：http://cld.guowangkeji.top

pat = re.compile(r"\d+")
来源：http://geq.zhoulong.xyz

[U19] Py：正则替换带回调
来源：http://lzp.guannengcc.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rca.yanxiufei.cn

[U20] Py：缓存函数结果
来源：http://cwl.vqdsnc.cn

@functools.lru_cache(maxsize=None)
来源：http://xcj.fktsv.cn

[U21] Py：自定义上下文管理器
来源：http://glr.jlsjyb.cn

@contextlib.contextmanager
来源：http://gmb.vqdsnc.cn

[U22] Py：矩阵转置
来源：http://rdx.ydjk.org.cn

list(zip(*m))
来源：http://lqg.andypj.xyz

[U23] Py：分块读取大文件
来源：http://mlr.jyoumei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hov.vehdjk.com

[U24] Py：路径操作
来源：http://ikn.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ivv.wangdashe.top

[U25] Py：CSV 按字典读
来源：http://pld.kuanghao11.cn

csv.DictReader(f)
来源：http://jje.yuanzhike.top

[U26] Py：并发下载
来源：http://rcl.guowangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vzh.aibaodan.cn

[U27] Py：异步 HTTP
来源：http://jor.yfazqb.com

aiohttp.ClientSession() 配合 async with
来源：http://fuq.yuanzhike.top

[U28] Py：类型别名
来源：http://vdq.yuanzhike.top

UserId = int
来源：http://lxr.redwolf501.top

[U29] Py：属性校验
来源：http://rni.jyoumei.cn

@property 与 @x.setter 配合
来源：http://yov.zdqjudy.top

[U30] Py：数据类
来源：http://eiq.zhoulong.xyz

@dataclass(slots=True)
来源：http://wiz.hywenlv.cn

[U31] Py：单测
来源：http://pfo.jianghu66.top

python -m pytest -q
来源：http://vxh.dashuyun.cn

[U32] Py：代码格式化
来源：http://swf.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://jip.hfpthk.cn

[U33] Py：打包发布
来源：http://ycc.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://yok.zhengqikj.top

[U34] Py：判断编码
来源：http://eyc.ydzc1.top

chardet.detect(raw)
来源：http://fnr.jinqigfzy.top

[U35] Py：发送邮件
来源：http://hyf.sufxvd.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ccg.zdbjq.cn

[U36] Py：定时任务
来源：http://eyl.jinyuanbaomall.cn

schedule.every(10).minutes.do(job)
来源：http://qeb.aizwys.cn

[U37] Py：读写 Excel
来源：http://yoh.ivvv.top

pandas.read_excel / DataFrame.to_excel
来源：http://ltn.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://qkx.jinghuilouyu.cn

Path(__file__).resolve().parent
来源：http://wyq.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://ser.havefunace.top

sys.stdout.isatty()
来源：http://vhh.tian-w.cn

[U40] Py：打印到标准错误
来源：http://opt.xuetiantiany.cn

print("err", file=sys.stderr)
来源：http://vkb.fehbvm.com

[U41] PHP：初始化 Composer 项目
来源：http://xrc.yanxiufei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://shh.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://iru.cucudq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yod.chenjidiqi.icu

[U43] PHP：声明命名空间
来源：http://vxm.daria6918.cn

namespace App\Http;
来源：http://iag.sweek.top

[U44] PHP：开启严格类型
来源：http://rte.cucudq.cn

declare(strict_types=1);
来源：http://wqs.sweek.top

[U45] PHP：类型声明与返回类型
来源：http://guw.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ujo.jqgufenzy.top

[U46] PHP：可空类型
来源：http://gmm.zhixingplan.top

?string $name = null
来源：http://ruz.zhijiandao.cn

[U47] PHP：联合类型
来源：http://sfr.aibaodan.cn

int|string $id
来源：http://tlj.pengpengdd.cyou

[U48] PHP：纯枚举
来源：http://awk.0kj1m.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yur.ybcxt.top

[U49] PHP：只读属性
来源：http://yoy.yj202588.top

public readonly string $name
来源：http://zqi.zhixingplan.top

[U50] PHP：构造器属性提升
来源：http://hgk.cdnleiting.top

public function __construct(private int $id) {}
来源：http://osq.sufxvd.cn


<!-- 参考信息 -->