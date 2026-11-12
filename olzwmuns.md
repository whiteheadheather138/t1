代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://xvb.feifeiyinyue.top

[S23] C：随机数
来源：http://isb.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ffu.shzxlz.cn

[S24] C：获取本地时间
来源：http://cqi.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://meb.c1oappe.top

[S25] C：内存拷贝
来源：http://urm.hywenlv.cn

memcpy(dst, src, n);
来源：http://cwy.smart0.xyz

[S26] C：内存清零
来源：http://hon.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://igm.gogol.net.cn

[S27] C：定义常量
来源：http://jdi.wangdashe.top

const double PI = 3.14159;
来源：http://aue.jianghu66.top

[S28] C：静态变量
来源：http://vdg.sweek.top

static int counter = 0;
来源：http://pwn.zhoulong.xyz

[S29] C：变参函数
来源：http://ilw.gogol.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hit.pycfn.com

[S30] C：头文件保护
来源：http://wet.ehwqpu.com

#ifndef X_H
来源：http://cmj.iojbl.cn

#define X_H
来源：http://wkw.pengpengdd.cyou

#endif
来源：http://uue.ctjpmb.com

[S31] C++：Hello World
来源：http://gea.yfazqb.com

#include <iostream>
来源：http://blz.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://rwn.quarkkingdee.top

[S32] C++：字符串
来源：http://krd.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://odn.jiagoushi.top

[S33] C++：vector 增删
来源：http://tmn.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://spi.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://fca.gzhubu.top

for (auto &x : v) { std::cout << x; }
来源：http://fit.cqqwz.cn

[S35] C++：map
来源：http://rhe.ybcxt.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lwh.zhixingplan.top

[S36] C++：unordered_map
来源：http://dmu.sysykeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qle.uphjek.com

[S37] C++：set
来源：http://ski.chenlongwang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jgm.aizwys.cn

[S38] C++：排序
来源：http://dqw.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://cqy.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://cvp.yanxiufei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://crx.jlsjyb.cn

[S40] C++：查找元素
来源：http://axo.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bdb.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://ahg.zdbjq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dbo.shuidangran.top

[S42] C++：继承与虚函数
来源：http://iua.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://abo.bjfxy.top

[S43] C++：智能指针
来源：http://ktt.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://uay.mhx1999.top

[S44] C++：引用传参
来源：http://tqm.ppjwa.cn

void inc(int &x) { ++x; }
来源：http://ahu.yueranfly.top

[S45] C++：lambda
来源：http://yjo.xylfe.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nfd.uphjek.com

[S46] C++：函数模板
来源：http://cog.jqgufenzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cin.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://krq.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zxs.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://rbn.hesvh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ktb.gzhubu.top

while (std::getline(in, line)) { }
来源：http://fnu.xylfe.cn

[S49] C++：写文件
来源：http://dxk.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jsd.sufxvd.cn

[S50] C++：格式化数字
来源：http://has.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zps.yongpay.top

[S51] C++：显式类型转换
来源：http://oyh.chenlongwang.top

static_cast<double>(a) / b
来源：http://wtj.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://spt.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://ygo.cheryme.top

[S53] C++：移动语义
来源：http://isl.jinyuanbaomall.cn

std::vector<int> w = std::move(v);
来源：http://ecs.hcnkem.com

[S54] C++：异常处理
来源：http://tai.52xcode.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jfw.svipenyu.cn

[S55] C++：结构化绑定
来源：http://nob.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hlc.shanyushiyangtech.top

[S56] C++：optional
来源：http://yfc.feifeiyinyue.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://evi.yuanzhike.top

[S57] C++：编译期常量
来源：http://gzg.smart0.xyz

constexpr int N = 10;
来源：http://uin.meibo888.top

[S58] C++：命名空间
来源：http://zkq.cdnleiting.top

namespace ns { int f() { return 1; } }
来源：http://zzl.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://jrl.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qjk.daxiang520.top

[S60] C++：遍历并删除元素
来源：http://vna.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qia.ctjpmb.com

================================================================================
来源：http://ogb.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ymh.shanyushiyangtech.top

================================================================================
来源：http://dej.jianghu66.top

[T01] Kotlin：Hello World
来源：http://wce.52xcode.cn

println("Hello")
来源：http://qse.ehwqpu.com

[T02] Kotlin：变量
来源：http://lxg.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eyt.hnxiangtu.top

[T03] Kotlin：字符串模板
来源：http://anc.daxiang520.top

"值: $b"
来源：http://zrw.hesvh.cn

[T04] Kotlin：空安全
来源：http://mpt.tian-w.cn

val n: String? = null;  n?.length
来源：http://zin.cucudq.cn

[T05] Kotlin：when 表达式
来源：http://bvr.yueranfly.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ibj.meibo888.top

[T06] Kotlin：集合映射
来源：http://kas.aibaodan.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hzv.cqqwz.cn

[T07] Kotlin：集合过滤
来源：http://juw.zycfv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ipv.bjfxy.top

[T08] Kotlin：数据类
来源：http://wek.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://otg.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://fto.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://obi.gotoacloud.top

[T10] Kotlin：默认参数
来源：http://fnn.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xqi.wangdashe.top

[T11] Kotlin：协程
来源：http://atp.hnxiangtu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lle.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://ubz.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://dnj.sufxvd.cn

[T13] Kotlin：只读 Map
来源：http://eys.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://gep.daria6918.cn

[T14] Kotlin：循环
来源：http://dlq.nwbrower.top

for (i in 1..10) println(i)
来源：http://zfd.fehbvm.com

[T15] Kotlin：接口
来源：http://ail.iojbl.cn

interface Shape { fun area(): Double }
来源：http://guq.shzxlz.cn

[T16] Swift：Hello World
来源：http://vhn.tian-w.cn

print("Hello")
来源：http://vkd.xingfuxueyuan.xyz

[T17] Swift：变量与常量
来源：http://qub.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://bxf.hesvh.cn

[T18] Swift：字符串插值
来源：http://mji.xziqi.cn

"值: \(b)"
来源：http://dmh.xziqi.cn

[T19] Swift：可选绑定
来源：http://opn.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://gzp.jqgufenzy.top

[T20] Swift：数组操作
来源：http://lxv.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://kvo.shangyingyoupin.top

[T21] Swift：遍历
来源：http://rpk.hammf.cn

for x in a { print(x) }
来源：http://vup.yuanzhike.top

[T22] Swift：字典
来源：http://ejo.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wse.ybcxt.top

[T23] Swift：函数
来源：http://nkn.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://akp.tarul.cn

[T24] Swift：闭包
来源：http://woi.ywan-chungtsiang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bpw.hywenlv.cn

[T25] Swift：结构体
来源：http://qbr.fehbvm.com

struct P { var x: Int }
来源：http://vvh.jlsjyb.cn

[T26] Swift：类与重写
来源：http://pmq.cashguo.top

class A: Base { override func f() {} }
来源：http://qtf.cqqwz.cn

[T27] Swift：错误处理
来源：http://cmt.bjfxy.top

do { try f() } catch { print(error) }
来源：http://jpl.quarkkingdee.top

[T28] Swift：枚举
来源：http://yjb.c1oappe.top

enum Color { case red, green }
来源：http://nth.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://hee.kuanghao11.cn

guard let x = opt else { return }
来源：http://lsc.zhongyouzk.top

[T30] Swift：协议
来源：http://ypp.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://jok.hnqzz.top

[T31] Lua：Hello World
来源：http://bac.jianghu66.top

print("Hello")
来源：http://umw.bbcook.cn

[T32] Lua：局部变量
来源：http://obm.uphjek.com

local a = 1
来源：http://ntu.haohaochexian.top

[T33] Lua：表（数组）
来源：http://npi.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://psy.meibo888.top

[T34] Lua：遍历表
来源：http://uik.hammf.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qpj.vqdsnc.cn

[T35] Lua：字典表
来源：http://oms.hammf.cn

local d = { a = 1 };  d.b = 2
来源：http://qys.andypj.xyz

[T36] Lua：函数
来源：http://hbp.tian-w.cn

function add(a, b) return a + b end
来源：http://pfy.iojbl.cn

[T37] Lua：字符串拼接
来源：http://rja.ybcxt.top

"a" .. "b"
来源：http://lod.ppjwa.cn

[T38] Lua：条件
来源：http://jxp.xylfe.cn

if x > 0 then print("正") end
来源：http://yio.ydzc1.top

[T39] Lua：模式匹配
来源：http://yyi.jinqigfzy.top

string.find(s, "%d+")
来源：http://uvz.ivvv.top

[T40] Lua：元表
来源：http://imi.kuanghao11.cn

setmetatable({}, { __index = base })
来源：http://sis.zdqjudy.top

[T41] Perl：Hello World
来源：http://xxr.ywan-chungtsiang.top

print "Hello\n";
来源：http://idp.cheryme.top

[T42] Perl：变量类型
来源：http://tgw.vehdjk.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://olo.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://hav.xingfuxueyuan.xyz

"值: $a"
来源：http://vdi.yueranfly.top

[T44] Perl：条件
来源：http://gfb.ivvv.top

if ($a > 0) { print "正"; }
来源：http://vic.shuidangran.top

[T45] Perl：数组遍历
来源：http://ccj.cheryme.top

for my $x (@arr) { print $x; }
来源：http://usx.pengpengdd.cyou

[T46] Perl：哈希操作
来源：http://nyj.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vst.xziqi.cn

[T47] Perl：正则捕获
来源：http://ivx.cucudq.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://iij.zhaomingkeji.xyz

[T48] Perl：正则替换
来源：http://jvc.shanyushiyangtech.top

$s =~ s/old/new/g;
来源：http://cks.yueranfly.top

[T49] Perl：函数
来源：http://sxy.hongshengwenyu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kob.uphjek.com

[T50] Perl：逐行读文件
来源：http://naj.zhiwuduotai.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ovm.andypj.xyz

while (my $line = <$fh>) { print $line; }
来源：http://puo.fktsv.cn

[T51] Scala：Hello World
来源：http://ivx.shanyushiyangkeji.top

println("Hello")
来源：http://krb.zhaomingkeji.xyz

[T52] Scala：变量
来源：http://zks.yangfankeji.com

val a = 1;  var b = 2
来源：http://lcw.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://ahl.daxiang520.top

s"值: $b"
来源：http://nza.fktsv.cn

[T54] Scala：集合映射
来源：http://ywj.svipenyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://rmo.tian-w.cn

[T55] Scala：集合过滤
来源：http://gse.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://hvp.ehwqpu.com

[T56] Scala：样例类
来源：http://lrg.9152youxi.cn

case class User(name: String, age: Int)
来源：http://tgh.fzhhl.top

[T57] Scala：模式匹配
来源：http://bwj.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kmw.nanxuanxn.top

[T58] Scala：函数定义
来源：http://qns.hnxiangtu.top

def add(a: Int, b: Int): Int = a + b
来源：http://zoo.snrcjt.cn

[T59] Scala：循环
来源：http://eww.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://kgk.shuidangran.top

[T60] Scala：折叠
来源：http://nbp.hcnkem.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ivl.sysykeji.top

================================================================================
来源：http://lcj.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ude.wangdashe.top

================================================================================
来源：http://ztu.xuanzx.com

[U01] Py：创建虚拟环境
来源：http://olb.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://ury.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://snl.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cuc.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://pzm.yj202588.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pby.gaohongyu789.top

[U04] Py：变量调试打印
来源：http://lqq.yfazqb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vqi.hammf.cn

[U05] Py：列表去重且保序
来源：http://wlm.bjfxy.top

list(dict.fromkeys(arr))
来源：http://avd.shanyushiyangkeji.top

[U06] Py：合并两个字典
来源：http://xaf.gaohongyu789.top

{**a, **b}
来源：http://xth.tian-w.cn

[U07] Py：反转字典键值
来源：http://vpp.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://dkj.hfpthk.cn

[U08] Py：展平二维列表
来源：http://rgh.tianlin.xyz

[y for x in nested for y in x]
来源：http://plh.xinyue.icu

[U09] Py：字典取最大值的键
来源：http://jix.cqqwz.cn

max(d, key=d.get)
来源：http://owz.dianchejie.cn

[U10] Py：按值排序字典
来源：http://obh.kuanghao11.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://omo.zhengqikj.top

[U11] Py：生成器表达式
来源：http://dyq.andypj.xyz

(x * 2 for x in arr)
来源：http://gjr.meibo888.top

[U12] Py：取出现最多的 3 个元素
来源：http://qpr.guannengcc.top

Counter(arr).most_common(3)
来源：http://hul.jinqigfzy.top

[U13] Py：固定长度队列
来源：http://oxx.feifeiyinyue.top

deque(maxlen=10)
来源：http://pok.xingfuxueyuan.xyz

[U14] Py：分组收集到列表
来源：http://lrq.shanyushiyangkeji.top

defaultdict(list)
来源：http://hua.dashuyun.cn

[U15] Py：高精度计时
来源：http://ssj.ctjpmb.com

t = time.perf_counter()
来源：http://vzp.fzhhl.top

[U16] Py：命令行参数解析
来源：http://sip.ehwqpu.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://caq.yueranfly.top

[U17] Py：初始化日志
来源：http://pnn.hnxiangtu.top

logging.basicConfig(level=logging.INFO)
来源：http://uzn.sxryk.cn

[U18] Py：预编译正则
来源：http://bwv.hcnkem.com

pat = re.compile(r"\d+")
来源：http://xtd.hongshengwenyu.top

[U19] Py：正则替换带回调
来源：http://amc.chenlongwang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mjk.shanyushiyangkeji.top

[U20] Py：缓存函数结果
来源：http://ots.gotoacloud.top

@functools.lru_cache(maxsize=None)
来源：http://hyt.zhoulong.xyz

[U21] Py：自定义上下文管理器
来源：http://wrx.fanxiaobao.xyz

@contextlib.contextmanager
来源：http://ows.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://acz.yj20258.top

list(zip(*m))
来源：http://vgr.yj20258.top

[U23] Py：分块读取大文件
来源：http://ico.cucudq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tzt.shangyingyoupin.top

[U24] Py：路径操作
来源：http://pee.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dlf.sweek.top

[U25] Py：CSV 按字典读
来源：http://kbj.ivvv.top

csv.DictReader(f)
来源：http://lva.ybcxt.top

[U26] Py：并发下载
来源：http://dfj.ppjwa.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xpd.andypj.xyz

[U27] Py：异步 HTTP
来源：http://wjj.hammf.cn

aiohttp.ClientSession() 配合 async with
来源：http://rze.jinghuilouyu.cn

[U28] Py：类型别名
来源：http://kfy.ydjk.org.cn

UserId = int
来源：http://jui.aizwys.cn

[U29] Py：属性校验
来源：http://ptv.gotoacloud.top

@property 与 @x.setter 配合
来源：http://hqh.yangfankeji.com

[U30] Py：数据类
来源：http://cxi.cqqwz.cn

@dataclass(slots=True)
来源：http://ofi.iojbl.cn

[U31] Py：单测
来源：http://ezk.jinghuilouyu.cn

python -m pytest -q
来源：http://zcw.cucudq.cn

[U32] Py：代码格式化
来源：http://pcj.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://tra.zhijiandao.cn

[U33] Py：打包发布
来源：http://ico.wangshuangyany.cn

python -m build  （依赖 pyproject.toml）
来源：http://mpl.ehwqpu.com

[U34] Py：判断编码
来源：http://sph.shangyingyoupin.top

chardet.detect(raw)
来源：http://chn.hesvh.cn

[U35] Py：发送邮件
来源：http://whv.zhixingplan.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cmw.zhixingplan.top

[U36] Py：定时任务
来源：http://cek.xingfuxueyuan.xyz

schedule.every(10).minutes.do(job)
来源：http://mwy.quarkkingdee.top

[U37] Py：读写 Excel
来源：http://fff.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://bzb.hammf.cn

[U38] Py：获取脚本所在目录
来源：http://irj.vehdjk.com

Path(__file__).resolve().parent
来源：http://lka.guowangkeji.top

[U39] Py：判断是否在交互环境
来源：http://lxl.snrcjt.cn

sys.stdout.isatty()
来源：http://lhg.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://sgf.zhongyouzk.top

print("err", file=sys.stderr)
来源：http://jsd.fanxiaobao.xyz

[U41] PHP：初始化 Composer 项目
来源：http://ipz.zycfv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jcz.fktsv.cn

[U42] PHP：PSR-4 自动加载
来源：http://zap.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rez.nanxuanxn.top

[U43] PHP：声明命名空间
来源：http://lan.yfazqb.com

namespace App\Http;
来源：http://log.zdqjudy.top

[U44] PHP：开启严格类型
来源：http://hqm.hesvh.cn

declare(strict_types=1);
来源：http://edn.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://lwd.smart0.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://ydt.aibaodan.cn

[U46] PHP：可空类型
来源：http://ssh.jqgufenzy.top

?string $name = null
来源：http://bnd.meibo888.top


<!-- 参考信息 -->