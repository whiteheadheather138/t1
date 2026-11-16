代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://kfq.fzhhl.top

[S23] C：随机数
来源：http://apn.hammf.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qrs.jqgfzy.top

[S24] C：获取本地时间
来源：http://xvs.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ggo.hesvh.cn

[S25] C：内存拷贝
来源：http://tmi.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://krj.ydzc1.top

[S26] C：内存清零
来源：http://idk.nanxinkj.top

memset(a, 0, sizeof a);
来源：http://adh.fktsv.cn

[S27] C：定义常量
来源：http://cpo.ppjwa.cn

const double PI = 3.14159;
来源：http://ans.hcnkem.com

[S28] C：静态变量
来源：http://iot.yj202588.top

static int counter = 0;
来源：http://nne.ppjwa.cn

[S29] C：变参函数
来源：http://snt.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eqi.wangshuangyany.cn

[S30] C：头文件保护
来源：http://eoh.zhoulong.xyz

#ifndef X_H
来源：http://kcd.xinyue.icu

#define X_H
来源：http://let.zhoulong.xyz

#endif
来源：http://mgt.yanxiufei.cn

[S31] C++：Hello World
来源：http://dcr.xylfe.cn

#include <iostream>
来源：http://qak.smart0.xyz

int main() { std::cout << "Hello\n"; }
来源：http://ghm.wangdashe.top

[S32] C++：字符串
来源：http://mtc.smart0.xyz

std::string s = "hi";  s += "!";
来源：http://fld.zhijiandao.cn

[S33] C++：vector 增删
来源：http://tmc.cucudq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kqu.yj20258888.top

[S34] C++：遍历 vector
来源：http://but.yuanzhike.top

for (auto &x : v) { std::cout << x; }
来源：http://map.xinyue.icu

[S35] C++：map
来源：http://qjc.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://imz.zhijiandao.cn

[S36] C++：unordered_map
来源：http://zto.vehdjk.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xlc.chenjidiqi.icu

[S37] C++：set
来源：http://ghr.chenzaomai.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jxo.andypj.xyz

[S38] C++：排序
来源：http://kbx.hammf.cn

std::sort(v.begin(), v.end());
来源：http://afg.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://mhd.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bym.fktsv.cn

[S40] C++：查找元素
来源：http://sld.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://spw.pengpengdd.cyou

[S41] C++：类与构造函数
来源：http://ldj.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pwm.316326.xyz

[S42] C++：继承与虚函数
来源：http://xpx.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://wdz.0kj1m.cn

[S43] C++：智能指针
来源：http://nup.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://vsl.vehdjk.com

[S44] C++：引用传参
来源：http://sjj.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://kgx.chenlongwang.top

[S45] C++：lambda
来源：http://yvv.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vid.shangyingyoupin.top

[S46] C++：函数模板
来源：http://het.zhoulong.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qln.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://zwr.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pfs.cashguo.top

[S48] C++：逐行读文件
来源：http://fum.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://qjr.nwbrower.top

while (std::getline(in, line)) { }
来源：http://efp.fengsongda.top

[S49] C++：写文件
来源：http://omy.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hkn.316326.xyz

[S50] C++：格式化数字
来源：http://zph.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kog.sxryk.cn

[S51] C++：显式类型转换
来源：http://ddt.hammf.cn

static_cast<double>(a) / b
来源：http://yjt.chenzaomai.com

[S52] C++：const 与 noexcept
来源：http://wly.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://wbz.aibaodan.cn

[S53] C++：移动语义
来源：http://bni.daria6918.cn

std::vector<int> w = std::move(v);
来源：http://heg.hesvh.cn

[S54] C++：异常处理
来源：http://vpp.ppjwa.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tbi.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://liv.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uaz.tian-w.cn

[S56] C++：optional
来源：http://rmm.jqgfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ogp.52xcode.cn

[S57] C++：编译期常量
来源：http://psp.jiagoushi.top

constexpr int N = 10;
来源：http://ahf.sweek.top

[S58] C++：命名空间
来源：http://zkg.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://ynv.guannengcc.top

[S59] C++：静态断言
来源：http://rto.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uvz.ppjwa.cn

[S60] C++：遍历并删除元素
来源：http://wgo.hcnkem.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://biu.mhx1999.top

================================================================================
来源：http://zkf.c1oappe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mkj.aizwys.cn

================================================================================
来源：http://etc.yuxming.cn

[T01] Kotlin：Hello World
来源：http://hso.cucudq.cn

println("Hello")
来源：http://yhx.yvedp.cn

[T02] Kotlin：变量
来源：http://mgm.daria6918.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gfg.tanke756.top

[T03] Kotlin：字符串模板
来源：http://khw.tarul.cn

"值: $b"
来源：http://sqt.cdnleiting.top

[T04] Kotlin：空安全
来源：http://ork.guowangkeji.top

val n: String? = null;  n?.length
来源：http://wsl.yuxming.cn

[T05] Kotlin：when 表达式
来源：http://hjo.pengpengdd.cyou

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hbl.yj20258.top

[T06] Kotlin：集合映射
来源：http://rjj.9152youxi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wdw.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://hme.zhijiandao.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://aap.guowangkeji.top

[T08] Kotlin：数据类
来源：http://whs.sufxvd.cn

data class User(val name: String, val age: Int)
来源：http://ssg.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://vab.xylfe.cn

fun String.exclaim() = this + "!"
来源：http://wok.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://gwa.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rko.gotoacloud.top

[T11] Kotlin：协程
来源：http://vbr.epnwcf.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://wbz.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://vlc.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://inh.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://kdc.cdnleiting.top

val m = mapOf("a" to 1)
来源：http://xcw.fehbvm.com

[T14] Kotlin：循环
来源：http://fup.yangfankeji.com

for (i in 1..10) println(i)
来源：http://sre.zhaomingkeji.xyz

[T15] Kotlin：接口
来源：http://pau.ctjpmb.com

interface Shape { fun area(): Double }
来源：http://qrv.gzhubu.top

[T16] Swift：Hello World
来源：http://hrg.sysykeji.top

print("Hello")
来源：http://qjc.316326.xyz

[T17] Swift：变量与常量
来源：http://lbm.sxryk.cn

var a = 1;  let b = 2
来源：http://bzq.ydjk.org.cn

[T18] Swift：字符串插值
来源：http://drr.shangyingyoupin.top

"值: \(b)"
来源：http://uem.hysaishi.cn

[T19] Swift：可选绑定
来源：http://hqz.meibo888.top

if let n = opt { print(n) }
来源：http://tqx.hfpthk.cn

[T20] Swift：数组操作
来源：http://bee.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://bdm.havefunace.top

[T21] Swift：遍历
来源：http://qol.jqgufenzy.top

for x in a { print(x) }
来源：http://ztq.tian-w.cn

[T22] Swift：字典
来源：http://emm.yj20258.top

var d = ["a": 1];  d["b"] = 2
来源：http://tbq.hfpthk.cn

[T23] Swift：函数
来源：http://czq.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aty.nwbrower.top

[T24] Swift：闭包
来源：http://rtc.ppjwa.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lch.nanxinkj.top

[T25] Swift：结构体
来源：http://sjo.yonumen.top

struct P { var x: Int }
来源：http://bvq.dashuyun.cn

[T26] Swift：类与重写
来源：http://kfd.ybcxt.top

class A: Base { override func f() {} }
来源：http://kxs.hongshengwenyu.top

[T27] Swift：错误处理
来源：http://klk.dianchejie.cn

do { try f() } catch { print(error) }
来源：http://rxd.guannengcc.top

[T28] Swift：枚举
来源：http://nxh.sweek.top

enum Color { case red, green }
来源：http://zaz.nwbrower.top

[T29] Swift：guard 提前返回
来源：http://fcl.shzxlz.cn

guard let x = opt else { return }
来源：http://qsc.zhengqikj.top

[T30] Swift：协议
来源：http://ffj.fehbvm.com

protocol Shape { func area() -> Double }
来源：http://ymz.shzxlz.cn

[T31] Lua：Hello World
来源：http://ppj.cdnleiting.top

print("Hello")
来源：http://iiw.kuanghao11.cn

[T32] Lua：局部变量
来源：http://ssb.316326.xyz

local a = 1
来源：http://cux.ctjpmb.com

[T33] Lua：表（数组）
来源：http://afw.guannengcc.top

local t = {1, 2, 3};  t[4] = 4
来源：http://bkk.zhixingplan.top

[T34] Lua：遍历表
来源：http://uns.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tdu.cqqwz.cn

[T35] Lua：字典表
来源：http://yjc.havefunace.top

local d = { a = 1 };  d.b = 2
来源：http://oye.cqqwz.cn

[T36] Lua：函数
来源：http://uvx.ppjwa.cn

function add(a, b) return a + b end
来源：http://mcz.guannengcc.top

[T37] Lua：字符串拼接
来源：http://szj.xingfuxueyuan.xyz

"a" .. "b"
来源：http://vph.shanyushiyangkeji.top

[T38] Lua：条件
来源：http://ozf.zycfv.cn

if x > 0 then print("正") end
来源：http://haw.yonumen.top

[T39] Lua：模式匹配
来源：http://dzu.ivvv.top

string.find(s, "%d+")
来源：http://rfg.tian-w.cn

[T40] Lua：元表
来源：http://tzw.cdnleiting.top

setmetatable({}, { __index = base })
来源：http://ixe.tanke756.top

[T41] Perl：Hello World
来源：http://aul.fanxiaobao.xyz

print "Hello\n";
来源：http://zxd.daxiang520.top

[T42] Perl：变量类型
来源：http://hmy.yonumen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cgl.hammf.cn

[T43] Perl：字符串插值
来源：http://wan.sweek.top

"值: $a"
来源：http://ycl.hysaishi.cn

[T44] Perl：条件
来源：http://qge.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://xsl.0kj1m.cn

[T45] Perl：数组遍历
来源：http://svd.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://jwf.52xcode.cn

[T46] Perl：哈希操作
来源：http://zzb.ybcxt.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vvl.zdqjudy.top

[T47] Perl：正则捕获
来源：http://ukt.yongpay.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pwh.hammf.cn

[T48] Perl：正则替换
来源：http://zvj.gogol.net.cn

$s =~ s/old/new/g;
来源：http://fei.jianghu66.top

[T49] Perl：函数
来源：http://trc.fktsv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qfq.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://lac.cashguo.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fjd.0kj1m.cn

while (my $line = <$fh>) { print $line; }
来源：http://kib.zdqjudy.top

[T51] Scala：Hello World
来源：http://ukz.nwbrower.top

println("Hello")
来源：http://fxa.gzhubu.top

[T52] Scala：变量
来源：http://mge.yuxming.cn

val a = 1;  var b = 2
来源：http://eqb.guowangkeji.top

[T53] Scala：字符串插值
来源：http://jil.fengsongda.top

s"值: $b"
来源：http://wip.52xcode.cn

[T54] Scala：集合映射
来源：http://glh.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://rbs.jinghuilouyu.cn

[T55] Scala：集合过滤
来源：http://tiz.shuidangran.top

List(1, 2, 3).filter(_ > 1)
来源：http://cjq.hnxiangtu.top

[T56] Scala：样例类
来源：http://twj.iojbl.cn

case class User(name: String, age: Int)
来源：http://wze.yonumen.top

[T57] Scala：模式匹配
来源：http://etr.cdnleiting.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bax.cqqwz.cn

[T58] Scala：函数定义
来源：http://fuz.fktsv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yhj.haohaochexian.top

[T59] Scala：循环
来源：http://bhs.iojbl.cn

for (i <- 1 to 10) println(i)
来源：http://nur.shanyushiyangtech.top

[T60] Scala：折叠
来源：http://bjf.xylfe.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qfv.jiagoushi.top

================================================================================
来源：http://aiu.zycfv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dco.sxryk.cn

================================================================================
来源：http://ffp.yuanzhike.top

[U01] Py：创建虚拟环境
来源：http://ali.iojbl.cn

python -m venv .venv && source .venv/bin/activate
来源：http://czo.jinyuanbaomall.cn

[U02] Py：导出 / 安装依赖
来源：http://rdv.hongshengwenyu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cbt.shzxlz.cn

[U03] Py：加载 .env 配置
来源：http://zkg.fengsongda.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cds.cdnleiting.top

[U04] Py：变量调试打印
来源：http://faq.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gwt.0kj1m.cn

[U05] Py：列表去重且保序
来源：http://lni.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://qoi.shzxlz.cn

[U06] Py：合并两个字典
来源：http://hgz.nanxinkj.top

{**a, **b}
来源：http://uhj.zdbjq.cn

[U07] Py：反转字典键值
来源：http://hqu.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://vij.iojbl.cn

[U08] Py：展平二维列表
来源：http://tuo.yueranfly.top

[y for x in nested for y in x]
来源：http://vyn.sweek.top

[U09] Py：字典取最大值的键
来源：http://rqd.chenjidiqi.icu

max(d, key=d.get)
来源：http://xql.kuanghao11.cn

[U10] Py：按值排序字典
来源：http://yrf.gzhubu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gun.jqgfzy.top

[U11] Py：生成器表达式
来源：http://ecb.daria6918.cn

(x * 2 for x in arr)
来源：http://wnp.cheryme.top

[U12] Py：取出现最多的 3 个元素
来源：http://aae.jyoumei.cn

Counter(arr).most_common(3)
来源：http://mdc.hesvh.cn

[U13] Py：固定长度队列
来源：http://vhk.hnqzz.top

deque(maxlen=10)
来源：http://suf.hcnkem.com

[U14] Py：分组收集到列表
来源：http://qxr.sweek.top

defaultdict(list)
来源：http://brn.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://bwr.sufxvd.cn

t = time.perf_counter()
来源：http://vbm.yuxming.cn

[U16] Py：命令行参数解析
来源：http://ptl.zhengqikj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lbg.316326.xyz

[U17] Py：初始化日志
来源：http://fbw.chenzaomai.com

logging.basicConfig(level=logging.INFO)
来源：http://ydb.aibaodan.cn

[U18] Py：预编译正则
来源：http://vwd.fengsongda.top

pat = re.compile(r"\d+")
来源：http://oxs.52xcode.cn

[U19] Py：正则替换带回调
来源：http://mev.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nky.ivvv.top

[U20] Py：缓存函数结果
来源：http://vpd.zycfv.cn

@functools.lru_cache(maxsize=None)
来源：http://qpd.pycfn.com

[U21] Py：自定义上下文管理器
来源：http://cdv.guannengcc.top

@contextlib.contextmanager
来源：http://fia.guowangkeji.top

[U22] Py：矩阵转置
来源：http://fny.dashuyun.cn

list(zip(*m))
来源：http://nhp.yangfankeji.com

[U23] Py：分块读取大文件
来源：http://are.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ynz.chenlongwang.top

[U24] Py：路径操作
来源：http://cus.jinqigfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wtt.sxryk.cn

[U25] Py：CSV 按字典读
来源：http://xfz.yueranfly.top

csv.DictReader(f)
来源：http://zgk.aibaodan.cn

[U26] Py：并发下载
来源：http://pqs.hnxiangtu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://htj.meibo888.top

[U27] Py：异步 HTTP
来源：http://wtu.sysykeji.top

aiohttp.ClientSession() 配合 async with
来源：http://xdp.shzxlz.cn

[U28] Py：类型别名
来源：http://yei.tanke756.top

UserId = int
来源：http://qju.hysaishi.cn

[U29] Py：属性校验
来源：http://sgp.shanyushiyangtech.top

@property 与 @x.setter 配合
来源：http://vuu.cqqwz.cn

[U30] Py：数据类
来源：http://fhv.feifeiyinyue.top

@dataclass(slots=True)
来源：http://ugj.fanxiaobao.xyz

[U31] Py：单测
来源：http://yxr.aizwys.cn

python -m pytest -q
来源：http://izu.0kj1m.cn

[U32] Py：代码格式化
来源：http://siz.vehdjk.com

ruff format . && ruff check --fix .
来源：http://wwj.snrcjt.cn

[U33] Py：打包发布
来源：http://gja.zhoulong.xyz

python -m build  （依赖 pyproject.toml）
来源：http://cvj.shanyushiyangkeji.top

[U34] Py：判断编码
来源：http://qdi.yj20258.top

chardet.detect(raw)
来源：http://ogh.wangdashe.top

[U35] Py：发送邮件
来源：http://pod.jinghuilouyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rsp.gaohongyu789.top

[U36] Py：定时任务
来源：http://rew.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://zax.yuxming.cn

[U37] Py：读写 Excel
来源：http://cwd.jqgfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://fuu.ydzc1.top

[U38] Py：获取脚本所在目录
来源：http://wub.uphjek.com

Path(__file__).resolve().parent
来源：http://tjp.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://kcl.dashuyun.cn

sys.stdout.isatty()
来源：http://psb.hnqzz.top

[U40] Py：打印到标准错误
来源：http://suo.nwbrower.top

print("err", file=sys.stderr)
来源：http://krt.yonumen.top

[U41] PHP：初始化 Composer 项目
来源：http://rmi.yongpay.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gtr.shangyingyoupin.top

[U42] PHP：PSR-4 自动加载
来源：http://joh.ydzc1.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lze.zhiwuduotai.top

[U43] PHP：声明命名空间
来源：http://ggu.vqdsnc.cn

namespace App\Http;
来源：http://bky.xylfe.cn

[U44] PHP：开启严格类型
来源：http://csg.yonumen.top

declare(strict_types=1);
来源：http://jma.ydjk.org.cn

[U45] PHP：类型声明与返回类型
来源：http://fzu.nwbrower.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ivp.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://dml.birdmap.top

?string $name = null
来源：http://ayx.fzhhl.top


<!-- 参考信息 -->