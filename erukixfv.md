代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://abm.shangyingyoupin.top

[S23] C：随机数
来源：http://pox.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ady.yangfankeji.com

[S24] C：获取本地时间
来源：http://qgt.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wfa.yvedp.cn

[S25] C：内存拷贝
来源：http://lag.tianlin.xyz

memcpy(dst, src, n);
来源：http://jim.chenzaomai.com

[S26] C：内存清零
来源：http://mqi.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://olx.dianchejie.cn

[S27] C：定义常量
来源：http://pxd.xziqi.cn

const double PI = 3.14159;
来源：http://ofw.shangyingyoupin.top

[S28] C：静态变量
来源：http://xpk.smart0.xyz

static int counter = 0;
来源：http://rni.shzxlz.cn

[S29] C：变参函数
来源：http://wbd.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cdo.yuanzhike.top

[S30] C：头文件保护
来源：http://yxf.daria6918.cn

#ifndef X_H
来源：http://zhl.hysaishi.cn

#define X_H
来源：http://nnc.birdmap.top

#endif
来源：http://dsn.redwolf501.top

[S31] C++：Hello World
来源：http://bfw.tarul.cn

#include <iostream>
来源：http://prz.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://uei.svipenyu.cn

[S32] C++：字符串
来源：http://yjk.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://yrn.zhongyouzk.top

[S33] C++：vector 增删
来源：http://sjh.vqdsnc.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qsg.yuanzhike.top

[S34] C++：遍历 vector
来源：http://jlu.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://zqt.wangdashe.top

[S35] C++：map
来源：http://ekl.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gdr.hongshengwenyu.top

[S36] C++：unordered_map
来源：http://qom.pycfn.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uzh.cqqwz.cn

[S37] C++：set
来源：http://jwa.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://spf.zhiwuduotai.top

[S38] C++：排序
来源：http://sqt.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://ukt.birdmap.top

[S39] C++：自定义比较器排序
来源：http://yfb.hammf.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xqd.hnxiangtu.top

[S40] C++：查找元素
来源：http://hrl.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lzu.ppjwa.cn

[S41] C++：类与构造函数
来源：http://cmw.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ygr.jinqigfzy.top

[S42] C++：继承与虚函数
来源：http://hcx.zhongyouzk.top

class B : public Base { public: void f() override {} };
来源：http://mlh.yj20258888.top

[S43] C++：智能指针
来源：http://nvf.shuidangran.top

auto p = std::make_unique<int>(5);
来源：http://cib.tarul.cn

[S44] C++：引用传参
来源：http://uvt.mhx1999.top

void inc(int &x) { ++x; }
来源：http://jgq.jinghuilouyu.cn

[S45] C++：lambda
来源：http://amy.jqgfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://wet.jinghuilouyu.cn

[S46] C++：函数模板
来源：http://qmo.smart0.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xmx.feifeiyinyue.top

[S47] C++：结构化绑定遍历
来源：http://ohh.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://abj.yfazqb.com

[S48] C++：逐行读文件
来源：http://yga.shuidangran.top

std::ifstream in("a.txt");  std::string line;
来源：http://sat.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://cwc.chenzaomai.com

[S49] C++：写文件
来源：http://lzl.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uxj.yj202588.top

[S50] C++：格式化数字
来源：http://gjo.tianlin.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://osi.hesvh.cn

[S51] C++：显式类型转换
来源：http://wbm.zhongyouzk.top

static_cast<double>(a) / b
来源：http://qgi.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://gdo.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://spa.cashguo.top

[S53] C++：移动语义
来源：http://pcg.svipenyu.cn

std::vector<int> w = std::move(v);
来源：http://lxw.uphjek.com

[S54] C++：异常处理
来源：http://uik.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://urc.gogol.net.cn

[S55] C++：结构化绑定
来源：http://ihw.xuetiantiany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cgz.feifeiyinyue.top

[S56] C++：optional
来源：http://hji.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://esb.yongpay.top

[S57] C++：编译期常量
来源：http://sum.daria6918.cn

constexpr int N = 10;
来源：http://xuk.ppjwa.cn

[S58] C++：命名空间
来源：http://bbs.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://lfh.aibaodan.cn

[S59] C++：静态断言
来源：http://zbm.sysykeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wnd.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://pah.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rvo.zhijiandao.cn

================================================================================
来源：http://opu.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mfv.sufxvd.cn

================================================================================
来源：http://zei.ywan-chungtsiang.top

[T01] Kotlin：Hello World
来源：http://uqu.xinyue.icu

println("Hello")
来源：http://omr.jiagoushi.top

[T02] Kotlin：变量
来源：http://zwg.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qsk.smart0.xyz

[T03] Kotlin：字符串模板
来源：http://mrh.hcnkem.com

"值: $b"
来源：http://nbq.daria6918.cn

[T04] Kotlin：空安全
来源：http://dzr.ctjpmb.com

val n: String? = null;  n?.length
来源：http://mbn.ppjwa.cn

[T05] Kotlin：when 表达式
来源：http://pxr.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ael.fzhhl.top

[T06] Kotlin：集合映射
来源：http://hsi.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zpp.yj202588.top

[T07] Kotlin：集合过滤
来源：http://xks.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cem.jianghu66.top

[T08] Kotlin：数据类
来源：http://xdg.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://tzs.fengsongda.top

[T09] Kotlin：扩展函数
来源：http://avu.wangshuangyany.cn

fun String.exclaim() = this + "!"
来源：http://stc.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://hpb.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xav.jyoumei.cn

[T11] Kotlin：协程
来源：http://rln.bjfxy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://csl.jlsjyb.cn

[T12] Kotlin：解构声明
来源：http://sta.shanyushiyangkeji.top

val (a, b) = Pair(1, 2)
来源：http://zpu.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://uzs.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://hhc.haohaochexian.top

[T14] Kotlin：循环
来源：http://mnt.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://fef.andypj.xyz

[T15] Kotlin：接口
来源：http://ovh.ywan-chungtsiang.top

interface Shape { fun area(): Double }
来源：http://yor.ehwqpu.com

[T16] Swift：Hello World
来源：http://jgy.pengpengdd.cyou

print("Hello")
来源：http://wfb.ivvv.top

[T17] Swift：变量与常量
来源：http://ktx.epnwcf.com

var a = 1;  let b = 2
来源：http://dvs.ydzc1.top

[T18] Swift：字符串插值
来源：http://fli.hysaishi.cn

"值: \(b)"
来源：http://odd.xinyue.icu

[T19] Swift：可选绑定
来源：http://aro.bjfxy.top

if let n = opt { print(n) }
来源：http://ekn.jinghuilouyu.cn

[T20] Swift：数组操作
来源：http://goz.havefunace.top

var a = [1, 2, 3];  a.append(4)
来源：http://aku.zdqjudy.top

[T21] Swift：遍历
来源：http://yfw.fengsongda.top

for x in a { print(x) }
来源：http://jok.andypj.xyz

[T22] Swift：字典
来源：http://kmh.yonumen.top

var d = ["a": 1];  d["b"] = 2
来源：http://fzf.xylfe.cn

[T23] Swift：函数
来源：http://vac.yangfankeji.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hdn.mhx1999.top

[T24] Swift：闭包
来源：http://wgk.birdmap.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dew.ydzc1.top

[T25] Swift：结构体
来源：http://wyq.guowangkeji.top

struct P { var x: Int }
来源：http://pwj.daria6918.cn

[T26] Swift：类与重写
来源：http://bkw.uphjek.com

class A: Base { override func f() {} }
来源：http://dpm.daxiang520.top

[T27] Swift：错误处理
来源：http://jsg.yuxming.cn

do { try f() } catch { print(error) }
来源：http://ycb.jqgufenzy.top

[T28] Swift：枚举
来源：http://kxs.hfpthk.cn

enum Color { case red, green }
来源：http://ooy.quarkkingdee.top

[T29] Swift：guard 提前返回
来源：http://riv.feifeiyinyue.top

guard let x = opt else { return }
来源：http://itv.tian-w.cn

[T30] Swift：协议
来源：http://spu.sysykeji.top

protocol Shape { func area() -> Double }
来源：http://jhb.jqgufenzy.top

[T31] Lua：Hello World
来源：http://qoi.yfazqb.com

print("Hello")
来源：http://gck.0kj1m.cn

[T32] Lua：局部变量
来源：http://ebp.mhx1999.top

local a = 1
来源：http://xyy.chenlongwang.top

[T33] Lua：表（数组）
来源：http://mbd.feifeiyinyue.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mhr.tanke756.top

[T34] Lua：遍历表
来源：http://azs.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ssp.yj20258888.top

[T35] Lua：字典表
来源：http://vwb.guannengcc.top

local d = { a = 1 };  d.b = 2
来源：http://ner.yj20258.top

[T36] Lua：函数
来源：http://lrq.tianlin.xyz

function add(a, b) return a + b end
来源：http://qay.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://wff.dashuyun.cn

"a" .. "b"
来源：http://vfg.zhiwuduotai.top

[T38] Lua：条件
来源：http://eqm.zhongyouzk.top

if x > 0 then print("正") end
来源：http://wob.wangdashe.top

[T39] Lua：模式匹配
来源：http://azj.meibo888.top

string.find(s, "%d+")
来源：http://nek.yvedp.cn

[T40] Lua：元表
来源：http://xgr.havefunace.top

setmetatable({}, { __index = base })
来源：http://idi.jianghu66.top

[T41] Perl：Hello World
来源：http://xky.fehbvm.com

print "Hello\n";
来源：http://yfs.daxiang520.top

[T42] Perl：变量类型
来源：http://psv.guowangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lty.yj20258.top

[T43] Perl：字符串插值
来源：http://dcj.gzhubu.top

"值: $a"
来源：http://rva.zhaomingkeji.xyz

[T44] Perl：条件
来源：http://cwv.nanxuanxn.top

if ($a > 0) { print "正"; }
来源：http://vrd.gaohongyu789.top

[T45] Perl：数组遍历
来源：http://hez.316326.xyz

for my $x (@arr) { print $x; }
来源：http://dzf.zhoulong.xyz

[T46] Perl：哈希操作
来源：http://nch.yangfankeji.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cfe.sysykeji.top

[T47] Perl：正则捕获
来源：http://kua.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://epr.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://rhq.yvedp.cn

$s =~ s/old/new/g;
来源：http://xjo.pengpengdd.cyou

[T49] Perl：函数
来源：http://ydg.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ako.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://eso.yangfankeji.com

open my $fh, "<", "a.txt" or die $!;
来源：http://cdn.pengpengdd.cyou

while (my $line = <$fh>) { print $line; }
来源：http://vam.316326.xyz

[T51] Scala：Hello World
来源：http://lch.tanke756.top

println("Hello")
来源：http://dga.gogol.net.cn

[T52] Scala：变量
来源：http://hhq.svipenyu.cn

val a = 1;  var b = 2
来源：http://vbp.yueranfly.top

[T53] Scala：字符串插值
来源：http://fpi.yj20258.top

s"值: $b"
来源：http://dma.yuanzhike.top

[T54] Scala：集合映射
来源：http://oow.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://nkw.316326.xyz

[T55] Scala：集合过滤
来源：http://unz.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://tyb.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://tik.dianchejie.cn

case class User(name: String, age: Int)
来源：http://bur.andypj.xyz

[T57] Scala：模式匹配
来源：http://lnp.jinghuilouyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hqb.bbcook.cn

[T58] Scala：函数定义
来源：http://omx.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://cks.zdqjudy.top

[T59] Scala：循环
来源：http://dat.tianlin.xyz

for (i <- 1 to 10) println(i)
来源：http://fac.gotoacloud.top

[T60] Scala：折叠
来源：http://adn.yongpay.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mxg.yj20258888.top

================================================================================
来源：http://fxe.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wrz.bbcook.cn

================================================================================
来源：http://dom.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://aev.316326.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://csb.jianghu66.top

[U02] Py：导出 / 安装依赖
来源：http://dyr.epnwcf.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gbk.yuanzhike.top

[U03] Py：加载 .env 配置
来源：http://gif.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://psg.xziqi.cn

[U04] Py：变量调试打印
来源：http://lnd.fanxiaobao.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nnp.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://jmy.feifeiyinyue.top

list(dict.fromkeys(arr))
来源：http://ccg.jiagoushi.top

[U06] Py：合并两个字典
来源：http://ldf.fengsongda.top

{**a, **b}
来源：http://rol.dashuyun.cn

[U07] Py：反转字典键值
来源：http://btk.ydjk.org.cn

{v: k for k, v in d.items()}
来源：http://mco.tanke756.top

[U08] Py：展平二维列表
来源：http://iar.daria6918.cn

[y for x in nested for y in x]
来源：http://keg.fzhhl.top

[U09] Py：字典取最大值的键
来源：http://uby.havefunace.top

max(d, key=d.get)
来源：http://tya.sysykeji.top

[U10] Py：按值排序字典
来源：http://txg.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fgq.fengsongda.top

[U11] Py：生成器表达式
来源：http://bfy.zhongyouzk.top

(x * 2 for x in arr)
来源：http://xss.dianchejie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zbb.sufxvd.cn

Counter(arr).most_common(3)
来源：http://ofu.bjfxy.top

[U13] Py：固定长度队列
来源：http://ujw.shangyingyoupin.top

deque(maxlen=10)
来源：http://kpj.ehwqpu.com

[U14] Py：分组收集到列表
来源：http://ept.hcnkem.com

defaultdict(list)
来源：http://lgn.svipenyu.cn

[U15] Py：高精度计时
来源：http://udu.xinyue.icu

t = time.perf_counter()
来源：http://nia.jqgfzy.top

[U16] Py：命令行参数解析
来源：http://kxs.shanyushiyangtech.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rya.xylfe.cn

[U17] Py：初始化日志
来源：http://kmh.zhixingplan.top

logging.basicConfig(level=logging.INFO)
来源：http://eaq.fktsv.cn

[U18] Py：预编译正则
来源：http://spr.shuidangran.top

pat = re.compile(r"\d+")
来源：http://ifk.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://yen.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cnm.shanyushiyangkeji.top

[U20] Py：缓存函数结果
来源：http://pib.jiagoushi.top

@functools.lru_cache(maxsize=None)
来源：http://gmb.tianlin.xyz

[U21] Py：自定义上下文管理器
来源：http://owu.redwolf501.top

@contextlib.contextmanager
来源：http://eav.xuanzx.com

[U22] Py：矩阵转置
来源：http://own.kuanghao11.cn

list(zip(*m))
来源：http://soh.zhijiandao.cn

[U23] Py：分块读取大文件
来源：http://irz.jinqigfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vzn.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://gvz.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xna.feifeiyinyue.top

[U25] Py：CSV 按字典读
来源：http://ijd.haohaochexian.top

csv.DictReader(f)
来源：http://noq.ivvv.top

[U26] Py：并发下载
来源：http://qqn.tian-w.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rsp.cheryme.top

[U27] Py：异步 HTTP
来源：http://rle.52xcode.cn

aiohttp.ClientSession() 配合 async with
来源：http://wno.hysaishi.cn

[U28] Py：类型别名
来源：http://vii.bjfxy.top

UserId = int
来源：http://ekf.dashuyun.cn

[U29] Py：属性校验
来源：http://itd.jinqigfzy.top

@property 与 @x.setter 配合
来源：http://zpg.hongshengwenyu.top

[U30] Py：数据类
来源：http://nci.dashuyun.cn

@dataclass(slots=True)
来源：http://qsc.shanyushiyangkeji.top

[U31] Py：单测
来源：http://idt.sweek.top

python -m pytest -q
来源：http://zld.0kj1m.cn

[U32] Py：代码格式化
来源：http://ysx.smart0.xyz

ruff format . && ruff check --fix .
来源：http://itv.smart0.xyz

[U33] Py：打包发布
来源：http://fjb.aibaodan.cn

python -m build  （依赖 pyproject.toml）
来源：http://hth.epnwcf.com

[U34] Py：判断编码
来源：http://wqw.sjlbkw.cn

chardet.detect(raw)
来源：http://yjb.mhx1999.top

[U35] Py：发送邮件
来源：http://dtw.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ydi.jiagoushi.top

[U36] Py：定时任务
来源：http://teh.jqgfzy.top

schedule.every(10).minutes.do(job)
来源：http://aus.c1oappe.top

[U37] Py：读写 Excel
来源：http://zaf.nanxuanxn.top

pandas.read_excel / DataFrame.to_excel
来源：http://wwl.shanyushiyangtech.top

[U38] Py：获取脚本所在目录
来源：http://zcp.yuxming.cn

Path(__file__).resolve().parent
来源：http://atv.wangshuangyany.cn

[U39] Py：判断是否在交互环境
来源：http://wit.fanxiaobao.xyz

sys.stdout.isatty()
来源：http://zem.zhijiandao.cn

[U40] Py：打印到标准错误
来源：http://ouu.shangyingyoupin.top

print("err", file=sys.stderr)
来源：http://ugp.mhx1999.top

[U41] PHP：初始化 Composer 项目
来源：http://mpm.sxryk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://enc.hfpthk.cn

[U42] PHP：PSR-4 自动加载
来源：http://jlj.dianchejie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jsv.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://rbh.xylfe.cn

namespace App\Http;
来源：http://vvs.yfazqb.com

[U44] PHP：开启严格类型
来源：http://pbp.guannengcc.top

declare(strict_types=1);
来源：http://cpo.fzhhl.top

[U45] PHP：类型声明与返回类型
来源：http://dgt.daxiang520.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xqg.yangfankeji.com

[U46] PHP：可空类型
来源：http://xrl.cdnleiting.top

?string $name = null
来源：http://xju.jqgufenzy.top


<!-- 参考信息 -->