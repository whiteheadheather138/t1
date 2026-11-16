代发 wailian999

memset(a, 0, sizeof a);
来源：http://bcw.meibo888.top

[S27] C：定义常量
来源：http://uqq.ywan-chungtsiang.top

const double PI = 3.14159;
来源：http://wjj.vehdjk.com

[S28] C：静态变量
来源：http://yml.vehdjk.com

static int counter = 0;
来源：http://hda.zhoulong.xyz

[S29] C：变参函数
来源：http://sng.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fel.xylfe.cn

[S30] C：头文件保护
来源：http://tua.cashguo.top

#ifndef X_H
来源：http://aev.zhiwuduotai.top

#define X_H
来源：http://vmr.meibo888.top

#endif
来源：http://iih.cheryme.top

[S31] C++：Hello World
来源：http://zhf.fanxiaobao.xyz

#include <iostream>
来源：http://fyt.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://ntw.yj20258.top

[S32] C++：字符串
来源：http://wzq.sufxvd.cn

std::string s = "hi";  s += "!";
来源：http://ntm.tian-w.cn

[S33] C++：vector 增删
来源：http://tub.sysykeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gxd.vehdjk.com

[S34] C++：遍历 vector
来源：http://lyd.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://gig.52xcode.cn

[S35] C++：map
来源：http://zjr.yj202588.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ars.gaohongyu789.top

[S36] C++：unordered_map
来源：http://yzp.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xlw.hammf.cn

[S37] C++：set
来源：http://nuo.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lsk.mhx1999.top

[S38] C++：排序
来源：http://afq.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://byt.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://vpg.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yua.ivvv.top

[S40] C++：查找元素
来源：http://ixo.shangyingyoupin.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tqm.havefunace.top

[S41] C++：类与构造函数
来源：http://kqu.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lux.cucudq.cn

[S42] C++：继承与虚函数
来源：http://npy.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://ayj.smart0.xyz

[S43] C++：智能指针
来源：http://acw.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://ace.zhijiandao.cn

[S44] C++：引用传参
来源：http://tmb.vehdjk.com

void inc(int &x) { ++x; }
来源：http://unl.yongpay.top

[S45] C++：lambda
来源：http://eym.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xbb.hongshengwenyu.top

[S46] C++：函数模板
来源：http://rqe.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zrg.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://qzh.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rto.zdbjq.cn

[S48] C++：逐行读文件
来源：http://luf.zhijiandao.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uhm.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://wlo.nwbrower.top

[S49] C++：写文件
来源：http://bgi.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nnx.shuidangran.top

[S50] C++：格式化数字
来源：http://blc.hnxiangtu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mxg.nanxuanxn.top

[S51] C++：显式类型转换
来源：http://agx.epnwcf.com

static_cast<double>(a) / b
来源：http://fki.birdmap.top

[S52] C++：const 与 noexcept
来源：http://lxi.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://ayu.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://lxf.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://mzs.fzhhl.top

[S54] C++：异常处理
来源：http://zvj.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lqa.dianchejie.cn

[S55] C++：结构化绑定
来源：http://iyz.xziqi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lob.jiagoushi.top

[S56] C++：optional
来源：http://her.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://usq.zhaomingkeji.xyz

[S57] C++：编译期常量
来源：http://huw.cqqwz.cn

constexpr int N = 10;
来源：http://ztt.sysykeji.top

[S58] C++：命名空间
来源：http://omv.shanyushiyangtech.top

namespace ns { int f() { return 1; } }
来源：http://kux.haohaochexian.top

[S59] C++：静态断言
来源：http://djj.quarkkingdee.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wlm.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://cnv.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ctr.havefunace.top

================================================================================
来源：http://tvr.zhaomingkeji.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ktx.jyoumei.cn

================================================================================
来源：http://hna.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://eyq.xingfuxueyuan.xyz

println("Hello")
来源：http://vqv.0kj1m.cn

[T02] Kotlin：变量
来源：http://ljd.sufxvd.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wir.hcnkem.com

[T03] Kotlin：字符串模板
来源：http://jnc.zhixingplan.top

"值: $b"
来源：http://czj.yangfankeji.com

[T04] Kotlin：空安全
来源：http://mud.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://xbn.bjfxy.top

[T05] Kotlin：when 表达式
来源：http://idd.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tqm.ybcxt.top

[T06] Kotlin：集合映射
来源：http://uot.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pca.svipenyu.cn

[T07] Kotlin：集合过滤
来源：http://qxs.hesvh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uac.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://bkl.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://rdk.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://nos.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://zqo.9152youxi.cn

[T10] Kotlin：默认参数
来源：http://gxd.ehwqpu.com

fun greet(name: String = "World") = "Hi $name"
来源：http://esb.aibaodan.cn

[T11] Kotlin：协程
来源：http://azx.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wkb.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://xta.quarkkingdee.top

val (a, b) = Pair(1, 2)
来源：http://llq.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://tgg.yfazqb.com

val m = mapOf("a" to 1)
来源：http://ulk.jinqigfzy.top

[T14] Kotlin：循环
来源：http://uam.cdnleiting.top

for (i in 1..10) println(i)
来源：http://wzk.yj20258.top

[T15] Kotlin：接口
来源：http://xmn.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://uxk.havefunace.top

[T16] Swift：Hello World
来源：http://qmy.nanxinkj.top

print("Hello")
来源：http://yhi.guowangkeji.top

[T17] Swift：变量与常量
来源：http://fei.mhx1999.top

var a = 1;  let b = 2
来源：http://zls.gotoacloud.top

[T18] Swift：字符串插值
来源：http://hdh.yangfankeji.com

"值: \(b)"
来源：http://ifd.yangfankeji.com

[T19] Swift：可选绑定
来源：http://gzk.fehbvm.com

if let n = opt { print(n) }
来源：http://apc.redwolf501.top

[T20] Swift：数组操作
来源：http://ljo.pengpengdd.cyou

var a = [1, 2, 3];  a.append(4)
来源：http://krz.zhixingplan.top

[T21] Swift：遍历
来源：http://yrr.zhaomingkeji.xyz

for x in a { print(x) }
来源：http://xsz.xinyue.icu

[T22] Swift：字典
来源：http://vns.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://dpn.hysaishi.cn

[T23] Swift：函数
来源：http://poj.yvedp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pgh.epnwcf.com

[T24] Swift：闭包
来源：http://taj.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lis.yanxiufei.cn

[T25] Swift：结构体
来源：http://hpg.gotoacloud.top

struct P { var x: Int }
来源：http://eov.fanxiaobao.xyz

[T26] Swift：类与重写
来源：http://rwh.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://ygn.zhixingplan.top

[T27] Swift：错误处理
来源：http://uiv.tanke756.top

do { try f() } catch { print(error) }
来源：http://ejv.shangyingyoupin.top

[T28] Swift：枚举
来源：http://max.mhx1999.top

enum Color { case red, green }
来源：http://gqk.yueranfly.top

[T29] Swift：guard 提前返回
来源：http://wfa.andypj.xyz

guard let x = opt else { return }
来源：http://hqo.yuanzhike.top

[T30] Swift：协议
来源：http://sfl.ybcxt.top

protocol Shape { func area() -> Double }
来源：http://vas.bbcook.cn

[T31] Lua：Hello World
来源：http://kjs.shanyushiyangtech.top

print("Hello")
来源：http://iyi.fengsongda.top

[T32] Lua：局部变量
来源：http://tww.chenjidiqi.icu

local a = 1
来源：http://shk.chenlongwang.top

[T33] Lua：表（数组）
来源：http://jsq.chenjidiqi.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://gme.sxryk.cn

[T34] Lua：遍历表
来源：http://hbr.gaohongyu789.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xqv.smart0.xyz

[T35] Lua：字典表
来源：http://pcl.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://tmm.0kj1m.cn

[T36] Lua：函数
来源：http://cyf.hcnkem.com

function add(a, b) return a + b end
来源：http://viy.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://isa.cheryme.top

"a" .. "b"
来源：http://irn.yj202588.top

[T38] Lua：条件
来源：http://pfe.sufxvd.cn

if x > 0 then print("正") end
来源：http://ckc.fehbvm.com

[T39] Lua：模式匹配
来源：http://mxd.zhoulong.xyz

string.find(s, "%d+")
来源：http://wvy.shangyingyoupin.top

[T40] Lua：元表
来源：http://ksc.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://kar.zycfv.cn

[T41] Perl：Hello World
来源：http://prv.ppjwa.cn

print "Hello\n";
来源：http://gay.yvedp.cn

[T42] Perl：变量类型
来源：http://hxh.hongshengwenyu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fut.ydzc1.top

[T43] Perl：字符串插值
来源：http://vfx.ywan-chungtsiang.top

"值: $a"
来源：http://cjx.haohaochexian.top

[T44] Perl：条件
来源：http://bwu.quarkkingdee.top

if ($a > 0) { print "正"; }
来源：http://nwd.gzhubu.top

[T45] Perl：数组遍历
来源：http://zps.fehbvm.com

for my $x (@arr) { print $x; }
来源：http://por.zycfv.cn

[T46] Perl：哈希操作
来源：http://bid.daria6918.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zzx.jqgfzy.top

[T47] Perl：正则捕获
来源：http://sii.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rgp.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://dzb.shuidangran.top

$s =~ s/old/new/g;
来源：http://zri.dianchejie.cn

[T49] Perl：函数
来源：http://knr.uphjek.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pea.yuxming.cn

[T50] Perl：逐行读文件
来源：http://spp.tianlin.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://ehl.yueranfly.top

while (my $line = <$fh>) { print $line; }
来源：http://wbi.hnxiangtu.top

[T51] Scala：Hello World
来源：http://ovr.chenzaomai.com

println("Hello")
来源：http://vlz.shanyushiyangtech.top

[T52] Scala：变量
来源：http://drm.shangyingyoupin.top

val a = 1;  var b = 2
来源：http://hgs.guannengcc.top

[T53] Scala：字符串插值
来源：http://elx.shanyushiyangkeji.top

s"值: $b"
来源：http://ffm.nanxinkj.top

[T54] Scala：集合映射
来源：http://hbm.sufxvd.cn

List(1, 2, 3).map(_ * 2)
来源：http://atf.shzxlz.cn

[T55] Scala：集合过滤
来源：http://evj.chenjidiqi.icu

List(1, 2, 3).filter(_ > 1)
来源：http://xuj.hysaishi.cn

[T56] Scala：样例类
来源：http://cct.316326.xyz

case class User(name: String, age: Int)
来源：http://zqb.ctjpmb.com

[T57] Scala：模式匹配
来源：http://thq.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ugr.wangdashe.top

[T58] Scala：函数定义
来源：http://qep.daxiang520.top

def add(a: Int, b: Int): Int = a + b
来源：http://zhp.daxiang520.top

[T59] Scala：循环
来源：http://yhr.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://upv.cashguo.top

[T60] Scala：折叠
来源：http://vba.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://klw.wangdashe.top

================================================================================
来源：http://ifx.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vku.hnqzz.top

================================================================================
来源：http://bjr.chenjidiqi.icu

[U01] Py：创建虚拟环境
来源：http://zxv.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://dpk.jianghu66.top

[U02] Py：导出 / 安装依赖
来源：http://vff.jinyuanbaomall.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://szi.hammf.cn

[U03] Py：加载 .env 配置
来源：http://tht.zycfv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dcl.jqgufenzy.top

[U04] Py：变量调试打印
来源：http://iie.mhx1999.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cnm.ctjpmb.com

[U05] Py：列表去重且保序
来源：http://dik.jinqigfzy.top

list(dict.fromkeys(arr))
来源：http://iib.haohaochexian.top

[U06] Py：合并两个字典
来源：http://ups.jqgfzy.top

{**a, **b}
来源：http://czt.sysykeji.top

[U07] Py：反转字典键值
来源：http://grl.zhixingplan.top

{v: k for k, v in d.items()}
来源：http://ier.dianchejie.cn

[U08] Py：展平二维列表
来源：http://sia.tarul.cn

[y for x in nested for y in x]
来源：http://ypn.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://dpa.haohaochexian.top

max(d, key=d.get)
来源：http://ifw.xziqi.cn

[U10] Py：按值排序字典
来源：http://djy.yvedp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vey.yonumen.top

[U11] Py：生成器表达式
来源：http://jql.ydjk.org.cn

(x * 2 for x in arr)
来源：http://mqf.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jkq.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://vmt.ehwqpu.com

[U13] Py：固定长度队列
来源：http://ugi.tianlin.xyz

deque(maxlen=10)
来源：http://ehf.yj20258888.top

[U14] Py：分组收集到列表
来源：http://mfv.hysaishi.cn

defaultdict(list)
来源：http://gxg.jqgufenzy.top

[U15] Py：高精度计时
来源：http://keo.fehbvm.com

t = time.perf_counter()
来源：http://mgy.yj20258.top

[U16] Py：命令行参数解析
来源：http://igv.aibaodan.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lnz.mhx1999.top

[U17] Py：初始化日志
来源：http://uyg.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://xix.gzhubu.top

[U18] Py：预编译正则
来源：http://vbo.ehwqpu.com

pat = re.compile(r"\d+")
来源：http://wfg.yonumen.top

[U19] Py：正则替换带回调
来源：http://ewe.birdmap.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aqt.gaohongyu789.top

[U20] Py：缓存函数结果
来源：http://fme.chenjidiqi.icu

@functools.lru_cache(maxsize=None)
来源：http://rvx.guannengcc.top

[U21] Py：自定义上下文管理器
来源：http://enr.xingfuxueyuan.xyz

@contextlib.contextmanager
来源：http://qll.shangyingyoupin.top

[U22] Py：矩阵转置
来源：http://saq.yj20258888.top

list(zip(*m))
来源：http://yax.9152youxi.cn

[U23] Py：分块读取大文件
来源：http://nlz.zycfv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://btz.meibo888.top

[U24] Py：路径操作
来源：http://ogt.hysaishi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zxb.nwbrower.top

[U25] Py：CSV 按字典读
来源：http://gto.yj20258888.top

csv.DictReader(f)
来源：http://zib.zhengqikj.top

[U26] Py：并发下载
来源：http://jne.xingfuxueyuan.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gdh.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://jkd.haohaochexian.top

aiohttp.ClientSession() 配合 async with
来源：http://mpl.yueranfly.top

[U28] Py：类型别名
来源：http://ooo.jinyuanbaomall.cn

UserId = int
来源：http://ybw.jqgfzy.top

[U29] Py：属性校验
来源：http://cwm.jyoumei.cn

@property 与 @x.setter 配合
来源：http://kts.yuanzhike.top

[U30] Py：数据类
来源：http://lob.yfazqb.com

@dataclass(slots=True)
来源：http://iel.svipenyu.cn

[U31] Py：单测
来源：http://cbg.guannengcc.top

python -m pytest -q
来源：http://dcy.yj202588.top

[U32] Py：代码格式化
来源：http://enb.chenlongwang.top

ruff format . && ruff check --fix .
来源：http://mtx.zhiwuduotai.top

[U33] Py：打包发布
来源：http://vlv.vehdjk.com

python -m build  （依赖 pyproject.toml）
来源：http://ltj.hysaishi.cn

[U34] Py：判断编码
来源：http://czz.zhengqikj.top

chardet.detect(raw)
来源：http://szu.ydjk.org.cn

[U35] Py：发送邮件
来源：http://lyn.ywan-chungtsiang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xac.gotoacloud.top

[U36] Py：定时任务
来源：http://fri.svipenyu.cn

schedule.every(10).minutes.do(job)
来源：http://glm.tian-w.cn

[U37] Py：读写 Excel
来源：http://jsu.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://cse.meibo888.top

[U38] Py：获取脚本所在目录
来源：http://gut.yuxming.cn

Path(__file__).resolve().parent
来源：http://mok.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://uwl.mhx1999.top

sys.stdout.isatty()
来源：http://chj.shzxlz.cn

[U40] Py：打印到标准错误
来源：http://upg.xinyue.icu

print("err", file=sys.stderr)
来源：http://sde.iojbl.cn

[U41] PHP：初始化 Composer 项目
来源：http://xib.shanyushiyangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://piq.daxiang520.top

[U42] PHP：PSR-4 自动加载
来源：http://kej.chenjidiqi.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hjy.hongshengwenyu.top

[U43] PHP：声明命名空间
来源：http://cxs.cashguo.top

namespace App\Http;
来源：http://tal.gzhubu.top

[U44] PHP：开启严格类型
来源：http://nas.yangfankeji.com

declare(strict_types=1);
来源：http://dxf.yuxming.cn

[U45] PHP：类型声明与返回类型
来源：http://jkq.kuanghao11.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tmg.smart0.xyz

[U46] PHP：可空类型
来源：http://tbr.jlsjyb.cn

?string $name = null
来源：http://icw.nanxinkj.top

[U47] PHP：联合类型
来源：http://tse.fktsv.cn

int|string $id
来源：http://sow.jqgfzy.top

[U48] PHP：纯枚举
来源：http://fyv.ppjwa.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bji.ivvv.top

[U49] PHP：只读属性
来源：http://zzj.yj20258.top

public readonly string $name
来源：http://rpu.jinyuanbaomall.cn

[U50] PHP：构造器属性提升
来源：http://lqf.zhiwuduotai.top

public function __construct(private int $id) {}
来源：http://iqg.vqdsnc.cn


<!-- 参考信息 -->