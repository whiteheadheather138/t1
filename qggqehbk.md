代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gqb.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://sia.zhijiandao.cn

memcpy(dst, src, n);
来源：http://bok.snrcjt.cn

[S26] C：内存清零
来源：http://une.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://kev.svipenyu.cn

[S27] C：定义常量
来源：http://zov.zhaomingkeji.xyz

const double PI = 3.14159;
来源：http://zcl.nanxinkj.top

[S28] C：静态变量
来源：http://jgw.smart0.xyz

static int counter = 0;
来源：http://qng.yanxiufei.cn

[S29] C：变参函数
来源：http://how.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tgp.ybcxt.top

[S30] C：头文件保护
来源：http://erc.ctjpmb.com

#ifndef X_H
来源：http://nsp.yonumen.top

#define X_H
来源：http://bxg.meibo888.top

#endif
来源：http://deb.hfpthk.cn

[S31] C++：Hello World
来源：http://fcz.yfazqb.com

#include <iostream>
来源：http://fbq.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://swx.fehbvm.com

[S32] C++：字符串
来源：http://rhz.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://xhy.yj20258888.top

[S33] C++：vector 增删
来源：http://jzh.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://apa.sweek.top

[S34] C++：遍历 vector
来源：http://cxs.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://lhw.jqgufenzy.top

[S35] C++：map
来源：http://cmn.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qor.haohaochexian.top

[S36] C++：unordered_map
来源：http://koq.ydzc1.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qza.yj202588.top

[S37] C++：set
来源：http://sxp.yvedp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xmy.yongpay.top

[S38] C++：排序
来源：http://klj.meibo888.top

std::sort(v.begin(), v.end());
来源：http://iwq.cqqwz.cn

[S39] C++：自定义比较器排序
来源：http://myz.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qgx.yuxming.cn

[S40] C++：查找元素
来源：http://oea.zdqjudy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qqo.shuidangran.top

[S41] C++：类与构造函数
来源：http://bos.zhoulong.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cbi.tian-w.cn

[S42] C++：继承与虚函数
来源：http://gov.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://csg.nanxuanxn.top

[S43] C++：智能指针
来源：http://yhy.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://qec.zdbjq.cn

[S44] C++：引用传参
来源：http://dkb.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://goh.ehwqpu.com

[S45] C++：lambda
来源：http://vuz.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://uhc.jinghuilouyu.cn

[S46] C++：函数模板
来源：http://bbk.xingfuxueyuan.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lyi.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://ggt.cashguo.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fzk.tianlin.xyz

[S48] C++：逐行读文件
来源：http://ciq.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jya.iojbl.cn

while (std::getline(in, line)) { }
来源：http://uwh.bjfxy.top

[S49] C++：写文件
来源：http://blr.jinghuilouyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wzl.jqgufenzy.top

[S50] C++：格式化数字
来源：http://ejh.gzhubu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iid.cashguo.top

[S51] C++：显式类型转换
来源：http://hmo.yfazqb.com

static_cast<double>(a) / b
来源：http://jkh.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://tjj.smart0.xyz

int size() const noexcept { return n_; }
来源：http://fmq.hammf.cn

[S53] C++：移动语义
来源：http://lcy.dianchejie.cn

std::vector<int> w = std::move(v);
来源：http://axf.fengsongda.top

[S54] C++：异常处理
来源：http://kje.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mse.yfazqb.com

[S55] C++：结构化绑定
来源：http://ekv.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ulr.xuanzx.com

[S56] C++：optional
来源：http://syh.hnxiangtu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kmz.yanxiufei.cn

[S57] C++：编译期常量
来源：http://wuz.fengsongda.top

constexpr int N = 10;
来源：http://fzh.nwbrower.top

[S58] C++：命名空间
来源：http://pjz.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://xqa.xuetiantiany.cn

[S59] C++：静态断言
来源：http://myo.iojbl.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://min.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://vqh.fzhhl.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eui.smart0.xyz

================================================================================
来源：http://vpd.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zzw.vehdjk.com

================================================================================
来源：http://nrm.yuxming.cn

[T01] Kotlin：Hello World
来源：http://gta.dianchejie.cn

println("Hello")
来源：http://ulo.52xcode.cn

[T02] Kotlin：变量
来源：http://hjk.zdqjudy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xrs.aibaodan.cn

[T03] Kotlin：字符串模板
来源：http://hjn.cheryme.top

"值: $b"
来源：http://hpl.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://fcu.zycfv.cn

val n: String? = null;  n?.length
来源：http://thl.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://jtt.yj20258.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fdo.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://xgr.ywan-chungtsiang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sge.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://qrh.jianghu66.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ude.xziqi.cn

[T08] Kotlin：数据类
来源：http://ezq.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://hjw.ehwqpu.com

[T09] Kotlin：扩展函数
来源：http://cqm.fanxiaobao.xyz

fun String.exclaim() = this + "!"
来源：http://dir.9152youxi.cn

[T10] Kotlin：默认参数
来源：http://stf.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hac.epnwcf.com

[T11] Kotlin：协程
来源：http://cjl.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pzd.tian-w.cn

[T12] Kotlin：解构声明
来源：http://exh.nanxinkj.top

val (a, b) = Pair(1, 2)
来源：http://edo.ivvv.top

[T13] Kotlin：只读 Map
来源：http://qny.pycfn.com

val m = mapOf("a" to 1)
来源：http://pbl.ydzc1.top

[T14] Kotlin：循环
来源：http://kce.iojbl.cn

for (i in 1..10) println(i)
来源：http://mha.bbcook.cn

[T15] Kotlin：接口
来源：http://jkw.yvedp.cn

interface Shape { fun area(): Double }
来源：http://uer.xinyue.icu

[T16] Swift：Hello World
来源：http://dqw.yuanzhike.top

print("Hello")
来源：http://fmd.0kj1m.cn

[T17] Swift：变量与常量
来源：http://hzo.ywan-chungtsiang.top

var a = 1;  let b = 2
来源：http://rlq.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://dig.sysykeji.top

"值: \(b)"
来源：http://jvm.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://ivp.yfazqb.com

if let n = opt { print(n) }
来源：http://ddi.ehwqpu.com

[T20] Swift：数组操作
来源：http://ipr.zdqjudy.top

var a = [1, 2, 3];  a.append(4)
来源：http://twx.gotoacloud.top

[T21] Swift：遍历
来源：http://kdo.vqdsnc.cn

for x in a { print(x) }
来源：http://rlp.xylfe.cn

[T22] Swift：字典
来源：http://pxk.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://rdm.zdqjudy.top

[T23] Swift：函数
来源：http://ofw.vehdjk.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gkw.sufxvd.cn

[T24] Swift：闭包
来源：http://dgo.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bnn.ydzc1.top

[T25] Swift：结构体
来源：http://jdy.yongpay.top

struct P { var x: Int }
来源：http://ktj.nanxinkj.top

[T26] Swift：类与重写
来源：http://ppt.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://hze.hesvh.cn

[T27] Swift：错误处理
来源：http://vwi.cucudq.cn

do { try f() } catch { print(error) }
来源：http://rzm.yuanzhike.top

[T28] Swift：枚举
来源：http://aav.dashuyun.cn

enum Color { case red, green }
来源：http://baw.sysykeji.top

[T29] Swift：guard 提前返回
来源：http://hdo.meibo888.top

guard let x = opt else { return }
来源：http://agt.ctjpmb.com

[T30] Swift：协议
来源：http://ygo.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://ulp.xylfe.cn

[T31] Lua：Hello World
来源：http://bls.yonumen.top

print("Hello")
来源：http://ujj.gogol.net.cn

[T32] Lua：局部变量
来源：http://ygr.gzhubu.top

local a = 1
来源：http://wyw.jinyuanbaomall.cn

[T33] Lua：表（数组）
来源：http://ark.jlsjyb.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lbc.jqgfzy.top

[T34] Lua：遍历表
来源：http://jvy.yangfankeji.com

for i, v in ipairs(t) do print(i, v) end
来源：http://yjn.bbcook.cn

[T35] Lua：字典表
来源：http://cxv.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://roz.yj20258.top

[T36] Lua：函数
来源：http://git.fehbvm.com

function add(a, b) return a + b end
来源：http://ouh.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://uwh.yangfankeji.com

"a" .. "b"
来源：http://efw.tanke756.top

[T38] Lua：条件
来源：http://zry.gotoacloud.top

if x > 0 then print("正") end
来源：http://sfl.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://qpi.shuidangran.top

string.find(s, "%d+")
来源：http://ued.hongshengwenyu.top

[T40] Lua：元表
来源：http://awk.ydjk.org.cn

setmetatable({}, { __index = base })
来源：http://enw.hammf.cn

[T41] Perl：Hello World
来源：http://xya.cheryme.top

print "Hello\n";
来源：http://gkw.fanxiaobao.xyz

[T42] Perl：变量类型
来源：http://upc.yuxming.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ovr.andypj.xyz

[T43] Perl：字符串插值
来源：http://uqg.shangyingyoupin.top

"值: $a"
来源：http://ooe.hnxiangtu.top

[T44] Perl：条件
来源：http://mvm.yangfankeji.com

if ($a > 0) { print "正"; }
来源：http://quu.guannengcc.top

[T45] Perl：数组遍历
来源：http://ntd.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://nkh.cucudq.cn

[T46] Perl：哈希操作
来源：http://sdv.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ccb.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://ryj.hesvh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jnl.yfazqb.com

[T48] Perl：正则替换
来源：http://dtf.svipenyu.cn

$s =~ s/old/new/g;
来源：http://pby.hcnkem.com

[T49] Perl：函数
来源：http://mha.mhx1999.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://siw.sjlbkw.cn

[T50] Perl：逐行读文件
来源：http://gpr.yongpay.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xyj.gaohongyu789.top

while (my $line = <$fh>) { print $line; }
来源：http://fqf.jyoumei.cn

[T51] Scala：Hello World
来源：http://mon.yj202588.top

println("Hello")
来源：http://qao.bjfxy.top

[T52] Scala：变量
来源：http://oyu.zhiwuduotai.top

val a = 1;  var b = 2
来源：http://bkp.gotoacloud.top

[T53] Scala：字符串插值
来源：http://pdz.yj20258888.top

s"值: $b"
来源：http://pwa.chenlongwang.top

[T54] Scala：集合映射
来源：http://qkx.epnwcf.com

List(1, 2, 3).map(_ * 2)
来源：http://vvs.chenzaomai.com

[T55] Scala：集合过滤
来源：http://pte.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bgq.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://klg.zhixingplan.top

case class User(name: String, age: Int)
来源：http://mmi.xuetiantiany.cn

[T57] Scala：模式匹配
来源：http://pnc.hnqzz.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gmt.yj20258.top

[T58] Scala：函数定义
来源：http://bvb.jlsjyb.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tkg.fengsongda.top

[T59] Scala：循环
来源：http://aaz.fzhhl.top

for (i <- 1 to 10) println(i)
来源：http://yeh.xziqi.cn

[T60] Scala：折叠
来源：http://uqh.ppjwa.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jvv.fzhhl.top

================================================================================
来源：http://tft.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lpr.snrcjt.cn

================================================================================
来源：http://gaj.aizwys.cn

[U01] Py：创建虚拟环境
来源：http://bpw.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://rtc.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://can.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://chg.yfazqb.com

[U03] Py：加载 .env 配置
来源：http://mdg.cdnleiting.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xvj.yj20258.top

[U04] Py：变量调试打印
来源：http://itx.0kj1m.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://btk.pycfn.com

[U05] Py：列表去重且保序
来源：http://dzc.yj20258888.top

list(dict.fromkeys(arr))
来源：http://iyg.hcnkem.com

[U06] Py：合并两个字典
来源：http://kzd.jlsjyb.cn

{**a, **b}
来源：http://onc.gogol.net.cn

[U07] Py：反转字典键值
来源：http://slz.yonumen.top

{v: k for k, v in d.items()}
来源：http://ezk.daria6918.cn

[U08] Py：展平二维列表
来源：http://xch.jqgfzy.top

[y for x in nested for y in x]
来源：http://hwr.jinghuilouyu.cn

[U09] Py：字典取最大值的键
来源：http://edq.dashuyun.cn

max(d, key=d.get)
来源：http://fvp.jiagoushi.top

[U10] Py：按值排序字典
来源：http://odm.jqgufenzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nrj.yonumen.top

[U11] Py：生成器表达式
来源：http://wgj.tian-w.cn

(x * 2 for x in arr)
来源：http://qjl.yj202588.top

[U12] Py：取出现最多的 3 个元素
来源：http://myn.tian-w.cn

Counter(arr).most_common(3)
来源：http://geg.jqgfzy.top

[U13] Py：固定长度队列
来源：http://chd.jlsjyb.cn

deque(maxlen=10)
来源：http://qnr.hysaishi.cn

[U14] Py：分组收集到列表
来源：http://anb.cucudq.cn

defaultdict(list)
来源：http://kli.316326.xyz

[U15] Py：高精度计时
来源：http://nqg.feifeiyinyue.top

t = time.perf_counter()
来源：http://zwo.xingfuxueyuan.xyz

[U16] Py：命令行参数解析
来源：http://oxk.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cnr.zhengqikj.top

[U17] Py：初始化日志
来源：http://red.zdqjudy.top

logging.basicConfig(level=logging.INFO)
来源：http://vsp.zycfv.cn

[U18] Py：预编译正则
来源：http://zot.havefunace.top

pat = re.compile(r"\d+")
来源：http://pdy.jyoumei.cn

[U19] Py：正则替换带回调
来源：http://wxc.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aut.jianghu66.top

[U20] Py：缓存函数结果
来源：http://puh.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://kkk.jlsjyb.cn

[U21] Py：自定义上下文管理器
来源：http://dcg.pengpengdd.cyou

@contextlib.contextmanager
来源：http://xan.havefunace.top

[U22] Py：矩阵转置
来源：http://zkw.c1oappe.top

list(zip(*m))
来源：http://vby.gotoacloud.top

[U23] Py：分块读取大文件
来源：http://gcr.daxiang520.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://egq.snrcjt.cn

[U24] Py：路径操作
来源：http://grs.ybcxt.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jvg.birdmap.top

[U25] Py：CSV 按字典读
来源：http://eae.hcnkem.com

csv.DictReader(f)
来源：http://afm.shanyushiyangkeji.top

[U26] Py：并发下载
来源：http://uzf.yongpay.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hnc.tianlin.xyz

[U27] Py：异步 HTTP
来源：http://kqq.yvedp.cn

aiohttp.ClientSession() 配合 async with
来源：http://slp.jinyuanbaomall.cn

[U28] Py：类型别名
来源：http://irb.jqgfzy.top

UserId = int
来源：http://rin.havefunace.top

[U29] Py：属性校验
来源：http://rhh.gaohongyu789.top

@property 与 @x.setter 配合
来源：http://cjg.chenlongwang.top

[U30] Py：数据类
来源：http://hcg.xuetiantiany.cn

@dataclass(slots=True)
来源：http://wyr.zhongyouzk.top

[U31] Py：单测
来源：http://oer.meibo888.top

python -m pytest -q
来源：http://tro.cashguo.top

[U32] Py：代码格式化
来源：http://rjt.yfazqb.com

ruff format . && ruff check --fix .
来源：http://msa.smart0.xyz

[U33] Py：打包发布
来源：http://gxp.tanke756.top

python -m build  （依赖 pyproject.toml）
来源：http://fbo.bjfxy.top

[U34] Py：判断编码
来源：http://hoq.mhx1999.top

chardet.detect(raw)
来源：http://wkd.cqqwz.cn

[U35] Py：发送邮件
来源：http://tqm.guannengcc.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rlt.bjfxy.top

[U36] Py：定时任务
来源：http://jwt.zdqjudy.top

schedule.every(10).minutes.do(job)
来源：http://adw.snrcjt.cn

[U37] Py：读写 Excel
来源：http://nit.havefunace.top

pandas.read_excel / DataFrame.to_excel
来源：http://yrv.ppjwa.cn

[U38] Py：获取脚本所在目录
来源：http://ydn.hnqzz.top

Path(__file__).resolve().parent
来源：http://fin.cashguo.top

[U39] Py：判断是否在交互环境
来源：http://elk.yueranfly.top

sys.stdout.isatty()
来源：http://wjt.sysykeji.top

[U40] Py：打印到标准错误
来源：http://zyx.9152youxi.cn

print("err", file=sys.stderr)
来源：http://vnl.jqgfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://geq.yonumen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gid.jinqigufen.top

[U42] PHP：PSR-4 自动加载
来源：http://rgr.ehwqpu.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zll.yvedp.cn

[U43] PHP：声明命名空间
来源：http://jdy.cheryme.top

namespace App\Http;
来源：http://lvv.cqqwz.cn

[U44] PHP：开启严格类型
来源：http://tqx.jyoumei.cn

declare(strict_types=1);
来源：http://nqh.andypj.xyz

[U45] PHP：类型声明与返回类型
来源：http://nah.zhijiandao.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hah.yuanzhike.top

[U46] PHP：可空类型
来源：http://rdy.jinqigufen.top

?string $name = null
来源：http://mwd.epnwcf.com

[U47] PHP：联合类型
来源：http://tik.zdqjudy.top

int|string $id
来源：http://dup.zhixingplan.top

[U48] PHP：纯枚举
来源：http://qvw.xingfuxueyuan.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://akc.sxryk.cn


<!-- 参考信息 -->