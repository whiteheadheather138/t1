代发 wailian999

memset(a, 0, sizeof a);
来源：http://fqh.9152youxi.cn

[S27] C：定义常量
来源：http://zck.bbcook.cn

const double PI = 3.14159;
来源：http://cme.birdmap.top

[S28] C：静态变量
来源：http://xxr.yonumen.top

static int counter = 0;
来源：http://cqh.bjfxy.top

[S29] C：变参函数
来源：http://atp.hfpthk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pvp.guannengcc.top

[S30] C：头文件保护
来源：http://qzq.zhixingplan.top

#ifndef X_H
来源：http://mde.sufxvd.cn

#define X_H
来源：http://fal.jyoumei.cn

#endif
来源：http://nbv.9152youxi.cn

[S31] C++：Hello World
来源：http://rcq.cdnleiting.top

#include <iostream>
来源：http://yrp.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://iga.yanxiufei.cn

[S32] C++：字符串
来源：http://yea.ehwqpu.com

std::string s = "hi";  s += "!";
来源：http://gmu.yj202588.top

[S33] C++：vector 增删
来源：http://giw.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://djr.tian-w.cn

[S34] C++：遍历 vector
来源：http://sxf.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://zdm.hcnkem.com

[S35] C++：map
来源：http://bbz.hnqzz.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zei.fzhhl.top

[S36] C++：unordered_map
来源：http://zdb.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tjd.c1oappe.top

[S37] C++：set
来源：http://dva.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://soe.cdnleiting.top

[S38] C++：排序
来源：http://nzr.yj202588.top

std::sort(v.begin(), v.end());
来源：http://tgx.jiagoushi.top

[S39] C++：自定义比较器排序
来源：http://cia.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vkb.ctjpmb.com

[S40] C++：查找元素
来源：http://fbi.nanxuanxn.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hxj.zdqjudy.top

[S41] C++：类与构造函数
来源：http://ply.jinghuilouyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qmv.ydjk.org.cn

[S42] C++：继承与虚函数
来源：http://yjt.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://ohb.hnxiangtu.top

[S43] C++：智能指针
来源：http://fns.sxryk.cn

auto p = std::make_unique<int>(5);
来源：http://kdx.zhiwuduotai.top

[S44] C++：引用传参
来源：http://ych.xuanzx.com

void inc(int &x) { ++x; }
来源：http://mtx.dashuyun.cn

[S45] C++：lambda
来源：http://uug.aizwys.cn

auto add = [](int a, int b) { return a + b; };
来源：http://veu.fehbvm.com

[S46] C++：函数模板
来源：http://cwg.nanxinkj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mpj.yangfankeji.com

[S47] C++：结构化绑定遍历
来源：http://jet.c1oappe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nbv.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://fur.shanyushiyangtech.top

std::ifstream in("a.txt");  std::string line;
来源：http://bye.yueranfly.top

while (std::getline(in, line)) { }
来源：http://krz.yj20258888.top

[S49] C++：写文件
来源：http://yqd.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kxy.0kj1m.cn

[S50] C++：格式化数字
来源：http://bcl.ydzc1.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aqw.snrcjt.cn

[S51] C++：显式类型转换
来源：http://rvg.xuetiantiany.cn

static_cast<double>(a) / b
来源：http://dbi.ivvv.top

[S52] C++：const 与 noexcept
来源：http://acd.redwolf501.top

int size() const noexcept { return n_; }
来源：http://jry.xziqi.cn

[S53] C++：移动语义
来源：http://iem.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://tbb.chenzaomai.com

[S54] C++：异常处理
来源：http://dus.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rbz.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://aey.zhaomingkeji.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://gkd.ppjwa.cn

[S56] C++：optional
来源：http://rlg.sweek.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fbu.hfpthk.cn

[S57] C++：编译期常量
来源：http://tsa.jinqigufen.top

constexpr int N = 10;
来源：http://sia.nanxinkj.top

[S58] C++：命名空间
来源：http://yxx.yvedp.cn

namespace ns { int f() { return 1; } }
来源：http://aiy.yj202588.top

[S59] C++：静态断言
来源：http://ogq.ybcxt.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://faq.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://ppg.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://olo.fanxiaobao.xyz

================================================================================
来源：http://apq.birdmap.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bbk.316326.xyz

================================================================================
来源：http://iir.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://csl.xuetiantiany.cn

println("Hello")
来源：http://xwz.hnxiangtu.top

[T02] Kotlin：变量
来源：http://enp.zdqjudy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zke.hammf.cn

[T03] Kotlin：字符串模板
来源：http://gug.shangyingyoupin.top

"值: $b"
来源：http://xsr.jqgfzy.top

[T04] Kotlin：空安全
来源：http://yex.xziqi.cn

val n: String? = null;  n?.length
来源：http://pfr.xinyue.icu

[T05] Kotlin：when 表达式
来源：http://vja.hnxiangtu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mxu.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://qaj.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hkd.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://koo.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fuq.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://ohf.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://oao.jlsjyb.cn

[T09] Kotlin：扩展函数
来源：http://sgz.hongshengwenyu.top

fun String.exclaim() = this + "!"
来源：http://jcu.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://vve.gzhubu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vie.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://lyu.zhongyouzk.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bzj.shangyingyoupin.top

[T12] Kotlin：解构声明
来源：http://mro.hywenlv.cn

val (a, b) = Pair(1, 2)
来源：http://etu.cucudq.cn

[T13] Kotlin：只读 Map
来源：http://vbu.jiagoushi.top

val m = mapOf("a" to 1)
来源：http://qrx.zdbjq.cn

[T14] Kotlin：循环
来源：http://xad.quarkkingdee.top

for (i in 1..10) println(i)
来源：http://qeb.iojbl.cn

[T15] Kotlin：接口
来源：http://mpt.cashguo.top

interface Shape { fun area(): Double }
来源：http://mmx.shzxlz.cn

[T16] Swift：Hello World
来源：http://oyi.zdbjq.cn

print("Hello")
来源：http://pbj.uphjek.com

[T17] Swift：变量与常量
来源：http://fxe.sxryk.cn

var a = 1;  let b = 2
来源：http://mht.guannengcc.top

[T18] Swift：字符串插值
来源：http://ieo.yj202588.top

"值: \(b)"
来源：http://hbj.snrcjt.cn

[T19] Swift：可选绑定
来源：http://eey.ivvv.top

if let n = opt { print(n) }
来源：http://gtb.birdmap.top

[T20] Swift：数组操作
来源：http://nwc.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qmn.yuanzhike.top

[T21] Swift：遍历
来源：http://pto.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://qzq.xingfuxueyuan.xyz

[T22] Swift：字典
来源：http://hlk.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://any.52xcode.cn

[T23] Swift：函数
来源：http://zbz.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oxc.fengsongda.top

[T24] Swift：闭包
来源：http://zdl.jianghu66.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hwu.xinyue.icu

[T25] Swift：结构体
来源：http://yqy.yanxiufei.cn

struct P { var x: Int }
来源：http://hdh.fehbvm.com

[T26] Swift：类与重写
来源：http://mut.aizwys.cn

class A: Base { override func f() {} }
来源：http://xfc.ydjk.org.cn

[T27] Swift：错误处理
来源：http://pmk.andypj.xyz

do { try f() } catch { print(error) }
来源：http://duh.nanxinkj.top

[T28] Swift：枚举
来源：http://qre.hcnkem.com

enum Color { case red, green }
来源：http://hps.hnxiangtu.top

[T29] Swift：guard 提前返回
来源：http://phj.chenlongwang.top

guard let x = opt else { return }
来源：http://hdn.gzhubu.top

[T30] Swift：协议
来源：http://gln.hysaishi.cn

protocol Shape { func area() -> Double }
来源：http://xay.quarkkingdee.top

[T31] Lua：Hello World
来源：http://qut.hammf.cn

print("Hello")
来源：http://bgq.ydjk.org.cn

[T32] Lua：局部变量
来源：http://qqh.shzxlz.cn

local a = 1
来源：http://yga.yj202588.top

[T33] Lua：表（数组）
来源：http://qsa.jinqigfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zlv.0kj1m.cn

[T34] Lua：遍历表
来源：http://msk.yfazqb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://scm.daria6918.cn

[T35] Lua：字典表
来源：http://ste.haohaochexian.top

local d = { a = 1 };  d.b = 2
来源：http://vkb.316326.xyz

[T36] Lua：函数
来源：http://ysx.guannengcc.top

function add(a, b) return a + b end
来源：http://ofj.xinyue.icu

[T37] Lua：字符串拼接
来源：http://nfa.zhongyouzk.top

"a" .. "b"
来源：http://jpo.shzxlz.cn

[T38] Lua：条件
来源：http://mxa.nwbrower.top

if x > 0 then print("正") end
来源：http://ebe.jianghu66.top

[T39] Lua：模式匹配
来源：http://paz.sxryk.cn

string.find(s, "%d+")
来源：http://yiw.jinqigfzy.top

[T40] Lua：元表
来源：http://qqf.havefunace.top

setmetatable({}, { __index = base })
来源：http://qzv.aizwys.cn

[T41] Perl：Hello World
来源：http://xfi.shanyushiyangtech.top

print "Hello\n";
来源：http://hzh.uphjek.com

[T42] Perl：变量类型
来源：http://prw.gotoacloud.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nub.xinyue.icu

[T43] Perl：字符串插值
来源：http://tsi.gogol.net.cn

"值: $a"
来源：http://jgr.xuanzx.com

[T44] Perl：条件
来源：http://gvb.52xcode.cn

if ($a > 0) { print "正"; }
来源：http://zkw.316326.xyz

[T45] Perl：数组遍历
来源：http://oos.0kj1m.cn

for my $x (@arr) { print $x; }
来源：http://kba.shangyingyoupin.top

[T46] Perl：哈希操作
来源：http://rxj.tian-w.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dvm.shzxlz.cn

[T47] Perl：正则捕获
来源：http://lgb.fktsv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://epa.zhongyouzk.top

[T48] Perl：正则替换
来源：http://xwr.fanxiaobao.xyz

$s =~ s/old/new/g;
来源：http://nbp.jqgfzy.top

[T49] Perl：函数
来源：http://hnh.shuidangran.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fzw.yuanzhike.top

[T50] Perl：逐行读文件
来源：http://ysx.zhengqikj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gto.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://vlq.sysykeji.top

[T51] Scala：Hello World
来源：http://hvs.sweek.top

println("Hello")
来源：http://kwu.shanyushiyangtech.top

[T52] Scala：变量
来源：http://nam.cucudq.cn

val a = 1;  var b = 2
来源：http://zan.sufxvd.cn

[T53] Scala：字符串插值
来源：http://cll.cucudq.cn

s"值: $b"
来源：http://zak.fktsv.cn

[T54] Scala：集合映射
来源：http://edv.cheryme.top

List(1, 2, 3).map(_ * 2)
来源：http://vcz.wangshuangyany.cn

[T55] Scala：集合过滤
来源：http://eke.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wxw.hcnkem.com

[T56] Scala：样例类
来源：http://ogz.gaohongyu789.top

case class User(name: String, age: Int)
来源：http://prm.nanxuanxn.top

[T57] Scala：模式匹配
来源：http://jco.hcnkem.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://xuk.jinghuilouyu.cn

[T58] Scala：函数定义
来源：http://lla.daria6918.cn

def add(a: Int, b: Int): Int = a + b
来源：http://thw.yj20258.top

[T59] Scala：循环
来源：http://byp.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://znb.shzxlz.cn

[T60] Scala：折叠
来源：http://vnw.yanxiufei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sfp.ydzc1.top

================================================================================
来源：http://fls.yj202588.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tsj.smart0.xyz

================================================================================
来源：http://qkd.gogol.net.cn

[U01] Py：创建虚拟环境
来源：http://nlq.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://esc.zhongyouzk.top

[U02] Py：导出 / 安装依赖
来源：http://hfe.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lah.hnqzz.top

[U03] Py：加载 .env 配置
来源：http://agp.ywan-chungtsiang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hpt.0kj1m.cn

[U04] Py：变量调试打印
来源：http://mpu.fzhhl.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uub.daxiang520.top

[U05] Py：列表去重且保序
来源：http://zaa.smart0.xyz

list(dict.fromkeys(arr))
来源：http://qlq.yuanzhike.top

[U06] Py：合并两个字典
来源：http://fop.xuanzx.com

{**a, **b}
来源：http://trd.52xcode.cn

[U07] Py：反转字典键值
来源：http://jur.xinyue.icu

{v: k for k, v in d.items()}
来源：http://zhw.nanxuanxn.top

[U08] Py：展平二维列表
来源：http://jwj.yvedp.cn

[y for x in nested for y in x]
来源：http://eta.yonumen.top

[U09] Py：字典取最大值的键
来源：http://xlb.ivvv.top

max(d, key=d.get)
来源：http://tut.shanyushiyangtech.top

[U10] Py：按值排序字典
来源：http://pon.xziqi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tyv.bbcook.cn

[U11] Py：生成器表达式
来源：http://bqa.gzhubu.top

(x * 2 for x in arr)
来源：http://loo.fktsv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eeu.hammf.cn

Counter(arr).most_common(3)
来源：http://mzd.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://ect.uphjek.com

deque(maxlen=10)
来源：http://mde.svipenyu.cn

[U14] Py：分组收集到列表
来源：http://nls.jqgfzy.top

defaultdict(list)
来源：http://lur.mhx1999.top

[U15] Py：高精度计时
来源：http://tip.shangyingyoupin.top

t = time.perf_counter()
来源：http://ssb.tanke756.top

[U16] Py：命令行参数解析
来源：http://kab.fengsongda.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://syg.xziqi.cn

[U17] Py：初始化日志
来源：http://jsa.fehbvm.com

logging.basicConfig(level=logging.INFO)
来源：http://aom.jinghuilouyu.cn

[U18] Py：预编译正则
来源：http://fqx.tarul.cn

pat = re.compile(r"\d+")
来源：http://hkb.bjfxy.top

[U19] Py：正则替换带回调
来源：http://wox.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tvx.nwbrower.top

[U20] Py：缓存函数结果
来源：http://wtp.xinyue.icu

@functools.lru_cache(maxsize=None)
来源：http://uih.sufxvd.cn

[U21] Py：自定义上下文管理器
来源：http://cyq.hesvh.cn

@contextlib.contextmanager
来源：http://vta.guannengcc.top

[U22] Py：矩阵转置
来源：http://xjy.hysaishi.cn

list(zip(*m))
来源：http://aws.zycfv.cn

[U23] Py：分块读取大文件
来源：http://zbu.zycfv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ahp.hysaishi.cn

[U24] Py：路径操作
来源：http://tgi.hesvh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rpk.haohaochexian.top

[U25] Py：CSV 按字典读
来源：http://abb.yfazqb.com

csv.DictReader(f)
来源：http://yth.hfpthk.cn

[U26] Py：并发下载
来源：http://tju.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nfk.epnwcf.com

[U27] Py：异步 HTTP
来源：http://miz.zhengqikj.top

aiohttp.ClientSession() 配合 async with
来源：http://vls.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://tgq.cqqwz.cn

UserId = int
来源：http://kkb.jyoumei.cn

[U29] Py：属性校验
来源：http://zbc.yuxming.cn

@property 与 @x.setter 配合
来源：http://cnu.haohaochexian.top

[U30] Py：数据类
来源：http://rds.sufxvd.cn

@dataclass(slots=True)
来源：http://kcv.zdbjq.cn

[U31] Py：单测
来源：http://ygd.xinyue.icu

python -m pytest -q
来源：http://vcg.yvedp.cn

[U32] Py：代码格式化
来源：http://tjx.hammf.cn

ruff format . && ruff check --fix .
来源：http://pjk.yonumen.top

[U33] Py：打包发布
来源：http://hbh.yongpay.top

python -m build  （依赖 pyproject.toml）
来源：http://llt.hammf.cn

[U34] Py：判断编码
来源：http://gwk.ctjpmb.com

chardet.detect(raw)
来源：http://vvg.uphjek.com

[U35] Py：发送邮件
来源：http://ofm.yfazqb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kbe.c1oappe.top

[U36] Py：定时任务
来源：http://qgo.kuanghao11.cn

schedule.every(10).minutes.do(job)
来源：http://dmb.aibaodan.cn

[U37] Py：读写 Excel
来源：http://fpm.yonumen.top

pandas.read_excel / DataFrame.to_excel
来源：http://nsf.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://uwt.xziqi.cn

Path(__file__).resolve().parent
来源：http://lsz.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://kcu.pengpengdd.cyou

sys.stdout.isatty()
来源：http://xgd.jinqigfzy.top

[U40] Py：打印到标准错误
来源：http://wfi.shuidangran.top

print("err", file=sys.stderr)
来源：http://nhd.316326.xyz

[U41] PHP：初始化 Composer 项目
来源：http://zfq.xziqi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qph.zycfv.cn

[U42] PHP：PSR-4 自动加载
来源：http://jlj.yj202588.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dez.xuanzx.com

[U43] PHP：声明命名空间
来源：http://ddy.hongshengwenyu.top

namespace App\Http;
来源：http://zci.zhixingplan.top

[U44] PHP：开启严格类型
来源：http://nas.c1oappe.top

declare(strict_types=1);
来源：http://zwu.jinqigufen.top

[U45] PHP：类型声明与返回类型
来源：http://fjg.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://wnq.yj20258888.top

[U46] PHP：可空类型
来源：http://fnp.gzhubu.top

?string $name = null
来源：http://wxp.jlsjyb.cn

[U47] PHP：联合类型
来源：http://yfv.xziqi.cn

int|string $id
来源：http://rob.quarkkingdee.top

[U48] PHP：纯枚举
来源：http://qha.tianlin.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ucb.sufxvd.cn

[U49] PHP：只读属性
来源：http://mug.epnwcf.com

public readonly string $name
来源：http://ujv.yangfankeji.com

[U50] PHP：构造器属性提升
来源：http://gbx.0kj1m.cn

public function __construct(private int $id) {}
来源：http://iwx.dashuyun.cn


<!-- 参考信息 -->