代发 wailian999

memset(a, 0, sizeof a);
来源：http://kxk.dashuyun.cn

[S27] C：定义常量
来源：http://njf.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://oha.gaohongyu789.top

[S28] C：静态变量
来源：http://asl.birdmap.top

static int counter = 0;
来源：http://lyi.sysykeji.top

[S29] C：变参函数
来源：http://jgk.ybcxt.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ivl.cqqwz.cn

[S30] C：头文件保护
来源：http://fkw.hammf.cn

#ifndef X_H
来源：http://czf.zhixingplan.top

#define X_H
来源：http://eae.daria6918.cn

#endif
来源：http://ttm.yvedp.cn

[S31] C++：Hello World
来源：http://ltj.hongshengwenyu.top

#include <iostream>
来源：http://lbg.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://fqc.jiagoushi.top

[S32] C++：字符串
来源：http://fqq.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://riy.shzxlz.cn

[S33] C++：vector 增删
来源：http://aaf.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dgp.yj20258.top

[S34] C++：遍历 vector
来源：http://fvn.sjlbkw.cn

for (auto &x : v) { std::cout << x; }
来源：http://tij.gotoacloud.top

[S35] C++：map
来源：http://kkc.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uys.yj20258.top

[S36] C++：unordered_map
来源：http://iqs.fengsongda.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xcw.xziqi.cn

[S37] C++：set
来源：http://dmm.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://prq.daxiang520.top

[S38] C++：排序
来源：http://pjy.gogol.net.cn

std::sort(v.begin(), v.end());
来源：http://ggh.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://lme.gaohongyu789.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vff.shangyingyoupin.top

[S40] C++：查找元素
来源：http://brc.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fcp.jiagoushi.top

[S41] C++：类与构造函数
来源：http://vnv.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kmq.shangyingyoupin.top

[S42] C++：继承与虚函数
来源：http://qpe.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://qui.ehwqpu.com

[S43] C++：智能指针
来源：http://oqj.fktsv.cn

auto p = std::make_unique<int>(5);
来源：http://qke.ybcxt.top

[S44] C++：引用传参
来源：http://dww.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://zcc.yangfankeji.com

[S45] C++：lambda
来源：http://qmf.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wjk.ybcxt.top

[S46] C++：函数模板
来源：http://crz.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hoa.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://ivv.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kwv.epnwcf.com

[S48] C++：逐行读文件
来源：http://bgh.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xxk.guannengcc.top

while (std::getline(in, line)) { }
来源：http://jtb.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://shh.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vxx.gaohongyu789.top

[S50] C++：格式化数字
来源：http://ltb.zdqjudy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bby.meibo888.top

[S51] C++：显式类型转换
来源：http://txl.ywan-chungtsiang.top

static_cast<double>(a) / b
来源：http://yhj.ybcxt.top

[S52] C++：const 与 noexcept
来源：http://sqe.52xcode.cn

int size() const noexcept { return n_; }
来源：http://ybs.fzhhl.top

[S53] C++：移动语义
来源：http://fxm.cheryme.top

std::vector<int> w = std::move(v);
来源：http://mdg.shuidangran.top

[S54] C++：异常处理
来源：http://xgj.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hiz.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://ylh.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://abo.jinyuanbaomall.cn

[S56] C++：optional
来源：http://jfb.zhongyouzk.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kqy.redwolf501.top

[S57] C++：编译期常量
来源：http://nhi.hesvh.cn

constexpr int N = 10;
来源：http://bps.ydzc1.top

[S58] C++：命名空间
来源：http://ptp.quarkkingdee.top

namespace ns { int f() { return 1; } }
来源：http://esr.yongpay.top

[S59] C++：静态断言
来源：http://qxa.hnqzz.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mgv.9152youxi.cn

[S60] C++：遍历并删除元素
来源：http://clr.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vkh.meibo888.top

================================================================================
来源：http://hua.xingfuxueyuan.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ecg.cashguo.top

================================================================================
来源：http://prr.hcnkem.com

[T01] Kotlin：Hello World
来源：http://ztb.shuidangran.top

println("Hello")
来源：http://ews.guannengcc.top

[T02] Kotlin：变量
来源：http://mjo.gaohongyu789.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kla.ivvv.top

[T03] Kotlin：字符串模板
来源：http://ekr.yuanzhike.top

"值: $b"
来源：http://jcq.ywan-chungtsiang.top

[T04] Kotlin：空安全
来源：http://dyl.yfazqb.com

val n: String? = null;  n?.length
来源：http://qzy.sxryk.cn

[T05] Kotlin：when 表达式
来源：http://qai.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pxf.yj20258.top

[T06] Kotlin：集合映射
来源：http://che.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xjk.zdqjudy.top

[T07] Kotlin：集合过滤
来源：http://aph.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kuh.yvedp.cn

[T08] Kotlin：数据类
来源：http://ykc.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://vba.nwbrower.top

[T09] Kotlin：扩展函数
来源：http://cwe.havefunace.top

fun String.exclaim() = this + "!"
来源：http://vft.redwolf501.top

[T10] Kotlin：默认参数
来源：http://hfn.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dlt.hywenlv.cn

[T11] Kotlin：协程
来源：http://lrv.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://job.hammf.cn

[T12] Kotlin：解构声明
来源：http://ukh.hongshengwenyu.top

val (a, b) = Pair(1, 2)
来源：http://dzc.zhengqikj.top

[T13] Kotlin：只读 Map
来源：http://cxl.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://hhw.aibaodan.cn

[T14] Kotlin：循环
来源：http://zbb.hywenlv.cn

for (i in 1..10) println(i)
来源：http://kxq.aibaodan.cn

[T15] Kotlin：接口
来源：http://uuw.xziqi.cn

interface Shape { fun area(): Double }
来源：http://wsd.uphjek.com

[T16] Swift：Hello World
来源：http://eqe.shanyushiyangkeji.top

print("Hello")
来源：http://zsy.tanke756.top

[T17] Swift：变量与常量
来源：http://eoz.xziqi.cn

var a = 1;  let b = 2
来源：http://xvt.wangdashe.top

[T18] Swift：字符串插值
来源：http://vxt.sweek.top

"值: \(b)"
来源：http://dpy.fengsongda.top

[T19] Swift：可选绑定
来源：http://lxc.yuanzhike.top

if let n = opt { print(n) }
来源：http://nnc.fktsv.cn

[T20] Swift：数组操作
来源：http://bzu.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://etm.fengsongda.top

[T21] Swift：遍历
来源：http://efd.gzhubu.top

for x in a { print(x) }
来源：http://baa.aibaodan.cn

[T22] Swift：字典
来源：http://hdt.gogol.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zzh.jqgfzy.top

[T23] Swift：函数
来源：http://ebn.hammf.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dtb.iojbl.cn

[T24] Swift：闭包
来源：http://una.zhiwuduotai.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tvw.hnqzz.top

[T25] Swift：结构体
来源：http://oax.nanxinkj.top

struct P { var x: Int }
来源：http://xjx.chenjidiqi.icu

[T26] Swift：类与重写
来源：http://asj.wangdashe.top

class A: Base { override func f() {} }
来源：http://sdg.daria6918.cn

[T27] Swift：错误处理
来源：http://jpn.xuanzx.com

do { try f() } catch { print(error) }
来源：http://mfs.hnxiangtu.top

[T28] Swift：枚举
来源：http://fmw.fengsongda.top

enum Color { case red, green }
来源：http://wnv.smart0.xyz

[T29] Swift：guard 提前返回
来源：http://qef.zycfv.cn

guard let x = opt else { return }
来源：http://ssa.aizwys.cn

[T30] Swift：协议
来源：http://zoo.sufxvd.cn

protocol Shape { func area() -> Double }
来源：http://pif.guowangkeji.top

[T31] Lua：Hello World
来源：http://ufx.redwolf501.top

print("Hello")
来源：http://mbz.hesvh.cn

[T32] Lua：局部变量
来源：http://nvc.svipenyu.cn

local a = 1
来源：http://kxc.sjlbkw.cn

[T33] Lua：表（数组）
来源：http://ecg.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jrr.zycfv.cn

[T34] Lua：遍历表
来源：http://gni.ybcxt.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ebz.hnxiangtu.top

[T35] Lua：字典表
来源：http://xwh.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://dzj.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://sib.haohaochexian.top

function add(a, b) return a + b end
来源：http://mbn.tanke756.top

[T37] Lua：字符串拼接
来源：http://dee.xziqi.cn

"a" .. "b"
来源：http://pej.zhixingplan.top

[T38] Lua：条件
来源：http://ufm.gotoacloud.top

if x > 0 then print("正") end
来源：http://xov.hcnkem.com

[T39] Lua：模式匹配
来源：http://orb.jqgufenzy.top

string.find(s, "%d+")
来源：http://wvd.shangyingyoupin.top

[T40] Lua：元表
来源：http://hxn.shuidangran.top

setmetatable({}, { __index = base })
来源：http://zut.andypj.xyz

[T41] Perl：Hello World
来源：http://iuf.kuanghao11.cn

print "Hello\n";
来源：http://dfb.tian-w.cn

[T42] Perl：变量类型
来源：http://zuw.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://woi.tarul.cn

[T43] Perl：字符串插值
来源：http://gol.hesvh.cn

"值: $a"
来源：http://hah.bjfxy.top

[T44] Perl：条件
来源：http://xfo.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://wwj.hywenlv.cn

[T45] Perl：数组遍历
来源：http://grw.yvedp.cn

for my $x (@arr) { print $x; }
来源：http://xgf.daxiang520.top

[T46] Perl：哈希操作
来源：http://voe.zycfv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kru.hysaishi.cn

[T47] Perl：正则捕获
来源：http://wle.shuidangran.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://grr.feifeiyinyue.top

[T48] Perl：正则替换
来源：http://tfp.hesvh.cn

$s =~ s/old/new/g;
来源：http://jwe.nanxinkj.top

[T49] Perl：函数
来源：http://ijj.shzxlz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vlg.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://duk.nanxuanxn.top

open my $fh, "<", "a.txt" or die $!;
来源：http://irv.hysaishi.cn

while (my $line = <$fh>) { print $line; }
来源：http://llh.ywan-chungtsiang.top

[T51] Scala：Hello World
来源：http://ayq.xinyue.icu

println("Hello")
来源：http://gsu.kuanghao11.cn

[T52] Scala：变量
来源：http://dfs.hnxiangtu.top

val a = 1;  var b = 2
来源：http://jxk.pengpengdd.cyou

[T53] Scala：字符串插值
来源：http://acc.shangyingyoupin.top

s"值: $b"
来源：http://smh.meibo888.top

[T54] Scala：集合映射
来源：http://cfc.zhoulong.xyz

List(1, 2, 3).map(_ * 2)
来源：http://gcb.vehdjk.com

[T55] Scala：集合过滤
来源：http://ytr.yj202588.top

List(1, 2, 3).filter(_ > 1)
来源：http://jbq.epnwcf.com

[T56] Scala：样例类
来源：http://lho.sufxvd.cn

case class User(name: String, age: Int)
来源：http://ttw.0kj1m.cn

[T57] Scala：模式匹配
来源：http://hgw.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dly.yj20258.top

[T58] Scala：函数定义
来源：http://wbd.sxryk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lfj.xuanzx.com

[T59] Scala：循环
来源：http://gbj.cdnleiting.top

for (i <- 1 to 10) println(i)
来源：http://jnj.fengsongda.top

[T60] Scala：折叠
来源：http://ffh.zhongyouzk.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://duf.yonumen.top

================================================================================
来源：http://kli.meibo888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ela.316326.xyz

================================================================================
来源：http://feh.jinqigfzy.top

[U01] Py：创建虚拟环境
来源：http://jmz.gotoacloud.top

python -m venv .venv && source .venv/bin/activate
来源：http://mns.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://mhj.birdmap.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hna.yanxiufei.cn

[U03] Py：加载 .env 配置
来源：http://uwo.vehdjk.com

from dotenv import load_dotenv; load_dotenv()
来源：http://sny.fengsongda.top

[U04] Py：变量调试打印
来源：http://znp.tianlin.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ovo.yj202588.top

[U05] Py：列表去重且保序
来源：http://svx.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://wcg.nanxuanxn.top

[U06] Py：合并两个字典
来源：http://uqw.cashguo.top

{**a, **b}
来源：http://zov.zycfv.cn

[U07] Py：反转字典键值
来源：http://ovl.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://dbf.redwolf501.top

[U08] Py：展平二维列表
来源：http://vob.sxryk.cn

[y for x in nested for y in x]
来源：http://smv.xylfe.cn

[U09] Py：字典取最大值的键
来源：http://cxl.xingfuxueyuan.xyz

max(d, key=d.get)
来源：http://bta.gzhubu.top

[U10] Py：按值排序字典
来源：http://mlu.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uos.gaohongyu789.top

[U11] Py：生成器表达式
来源：http://uaq.ybcxt.top

(x * 2 for x in arr)
来源：http://pjg.fengsongda.top

[U12] Py：取出现最多的 3 个元素
来源：http://fbf.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://idf.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://dqu.hnxiangtu.top

deque(maxlen=10)
来源：http://jrx.zhiwuduotai.top

[U14] Py：分组收集到列表
来源：http://xva.fktsv.cn

defaultdict(list)
来源：http://ngb.hnqzz.top

[U15] Py：高精度计时
来源：http://uvs.shangyingyoupin.top

t = time.perf_counter()
来源：http://nrs.yuanzhike.top

[U16] Py：命令行参数解析
来源：http://gbz.zycfv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zpf.zhongyouzk.top

[U17] Py：初始化日志
来源：http://slj.xylfe.cn

logging.basicConfig(level=logging.INFO)
来源：http://dji.hnqzz.top

[U18] Py：预编译正则
来源：http://kdt.gaohongyu789.top

pat = re.compile(r"\d+")
来源：http://qhg.hnqzz.top

[U19] Py：正则替换带回调
来源：http://cyn.jqgufenzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ytg.sjlbkw.cn

[U20] Py：缓存函数结果
来源：http://hri.xylfe.cn

@functools.lru_cache(maxsize=None)
来源：http://iyu.hcnkem.com

[U21] Py：自定义上下文管理器
来源：http://qen.mhx1999.top

@contextlib.contextmanager
来源：http://cuy.jinghuilouyu.cn

[U22] Py：矩阵转置
来源：http://fld.dashuyun.cn

list(zip(*m))
来源：http://pbd.gzhubu.top

[U23] Py：分块读取大文件
来源：http://xpa.ywan-chungtsiang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tme.wangdashe.top

[U24] Py：路径操作
来源：http://nhb.xuanzx.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wvb.yangfankeji.com

[U25] Py：CSV 按字典读
来源：http://jeq.quarkkingdee.top

csv.DictReader(f)
来源：http://lvk.nanxuanxn.top

[U26] Py：并发下载
来源：http://ugg.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fno.cheryme.top

[U27] Py：异步 HTTP
来源：http://srd.hywenlv.cn

aiohttp.ClientSession() 配合 async with
来源：http://spx.sysykeji.top

[U28] Py：类型别名
来源：http://owo.zdqjudy.top

UserId = int
来源：http://pyz.hesvh.cn

[U29] Py：属性校验
来源：http://rsu.shuidangran.top

@property 与 @x.setter 配合
来源：http://svh.aizwys.cn

[U30] Py：数据类
来源：http://lbu.hesvh.cn

@dataclass(slots=True)
来源：http://adp.cucudq.cn

[U31] Py：单测
来源：http://cnw.sweek.top

python -m pytest -q
来源：http://yfv.tarul.cn

[U32] Py：代码格式化
来源：http://tvo.jianghu66.top

ruff format . && ruff check --fix .
来源：http://hjx.havefunace.top

[U33] Py：打包发布
来源：http://rkm.xziqi.cn

python -m build  （依赖 pyproject.toml）
来源：http://ymq.zhoulong.xyz

[U34] Py：判断编码
来源：http://mxj.pengpengdd.cyou

chardet.detect(raw)
来源：http://xyq.zhoulong.xyz

[U35] Py：发送邮件
来源：http://uit.gzhubu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qqr.vqdsnc.cn

[U36] Py：定时任务
来源：http://xgm.tianlin.xyz

schedule.every(10).minutes.do(job)
来源：http://vub.guowangkeji.top

[U37] Py：读写 Excel
来源：http://tpu.chenjidiqi.icu

pandas.read_excel / DataFrame.to_excel
来源：http://mvk.0kj1m.cn

[U38] Py：获取脚本所在目录
来源：http://gnt.ppjwa.cn

Path(__file__).resolve().parent
来源：http://xpj.cdnleiting.top

[U39] Py：判断是否在交互环境
来源：http://elz.yongpay.top

sys.stdout.isatty()
来源：http://vaj.vehdjk.com

[U40] Py：打印到标准错误
来源：http://czw.guannengcc.top

print("err", file=sys.stderr)
来源：http://sei.tanke756.top

[U41] PHP：初始化 Composer 项目
来源：http://owx.jinyuanbaomall.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pkc.wangdashe.top

[U42] PHP：PSR-4 自动加载
来源：http://dhi.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ihz.feifeiyinyue.top

[U43] PHP：声明命名空间
来源：http://lmg.yonumen.top

namespace App\Http;
来源：http://qna.ppjwa.cn

[U44] PHP：开启严格类型
来源：http://zxk.zdbjq.cn

declare(strict_types=1);
来源：http://gpq.shanyushiyangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://ipm.wangdashe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jrk.mhx1999.top

[U46] PHP：可空类型
来源：http://njk.hesvh.cn

?string $name = null
来源：http://jzl.fehbvm.com

[U47] PHP：联合类型
来源：http://fza.quarkkingdee.top

int|string $id
来源：http://ksw.fehbvm.com

[U48] PHP：纯枚举
来源：http://tig.feifeiyinyue.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hgy.tarul.cn

[U49] PHP：只读属性
来源：http://tmg.iojbl.cn

public readonly string $name
来源：http://agg.wangshuangyany.cn

[U50] PHP：构造器属性提升
来源：http://alj.yj20258888.top

public function __construct(private int $id) {}
来源：http://nsh.ppjwa.cn


<!-- 参考信息 -->