代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://nym.cheryme.top

[S23] C：随机数
来源：http://wtq.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://viu.xylfe.cn

[S24] C：获取本地时间
来源：http://gbs.gogol.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lgw.yanxiufei.cn

[S25] C：内存拷贝
来源：http://gqd.yuxming.cn

memcpy(dst, src, n);
来源：http://ckd.shuidangran.top

[S26] C：内存清零
来源：http://wop.wangdashe.top

memset(a, 0, sizeof a);
来源：http://dns.quarkkingdee.top

[S27] C：定义常量
来源：http://tbr.hnqzz.top

const double PI = 3.14159;
来源：http://voc.jinghuilouyu.cn

[S28] C：静态变量
来源：http://fmj.nanxinkj.top

static int counter = 0;
来源：http://yvh.redwolf501.top

[S29] C：变参函数
来源：http://unm.jinqigfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://szv.ppjwa.cn

[S30] C：头文件保护
来源：http://aex.svipenyu.cn

#ifndef X_H
来源：http://syb.shzxlz.cn

#define X_H
来源：http://wij.yuxming.cn

#endif
来源：http://vep.uphjek.com

[S31] C++：Hello World
来源：http://rwx.ydjk.org.cn

#include <iostream>
来源：http://viu.hfpthk.cn

int main() { std::cout << "Hello\n"; }
来源：http://nlm.chenzaomai.com

[S32] C++：字符串
来源：http://hbb.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://pxi.chenlongwang.top

[S33] C++：vector 增删
来源：http://pdt.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xtp.bbcook.cn

[S34] C++：遍历 vector
来源：http://kri.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://iwe.vehdjk.com

[S35] C++：map
来源：http://avd.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zrq.hywenlv.cn

[S36] C++：unordered_map
来源：http://rca.xingfuxueyuan.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ggo.52xcode.cn

[S37] C++：set
来源：http://nrf.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jzv.ybcxt.top

[S38] C++：排序
来源：http://pwz.ppjwa.cn

std::sort(v.begin(), v.end());
来源：http://klc.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://eug.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ecn.tianlin.xyz

[S40] C++：查找元素
来源：http://qqt.aizwys.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nmk.fengsongda.top

[S41] C++：类与构造函数
来源：http://xev.jianghu66.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cir.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://upy.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://xbw.hfpthk.cn

[S43] C++：智能指针
来源：http://dag.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://lvb.zdqjudy.top

[S44] C++：引用传参
来源：http://jcq.fengsongda.top

void inc(int &x) { ++x; }
来源：http://mer.cashguo.top

[S45] C++：lambda
来源：http://mvm.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://rcn.c1oappe.top

[S46] C++：函数模板
来源：http://bds.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zdh.vqdsnc.cn

[S47] C++：结构化绑定遍历
来源：http://dbq.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zve.fengsongda.top

[S48] C++：逐行读文件
来源：http://tje.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vmd.guowangkeji.top

while (std::getline(in, line)) { }
来源：http://yir.shanyushiyangtech.top

[S49] C++：写文件
来源：http://uyg.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://szi.hnqzz.top

[S50] C++：格式化数字
来源：http://uun.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wwm.gotoacloud.top

[S51] C++：显式类型转换
来源：http://cjv.redwolf501.top

static_cast<double>(a) / b
来源：http://cgg.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://qxg.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://jwa.vehdjk.com

[S53] C++：移动语义
来源：http://jia.yj202588.top

std::vector<int> w = std::move(v);
来源：http://dzx.guowangkeji.top

[S54] C++：异常处理
来源：http://bsx.shzxlz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yis.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://mmc.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://crr.ydzc1.top

[S56] C++：optional
来源：http://bzy.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kgz.fehbvm.com

[S57] C++：编译期常量
来源：http://hpu.cucudq.cn

constexpr int N = 10;
来源：http://pxf.zhongyouzk.top

[S58] C++：命名空间
来源：http://pue.shuidangran.top

namespace ns { int f() { return 1; } }
来源：http://yhw.chenjidiqi.icu

[S59] C++：静态断言
来源：http://buh.xuetiantiany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rpq.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://iji.mhx1999.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xyc.yangfankeji.com

================================================================================
来源：http://fyp.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mij.snrcjt.cn

================================================================================
来源：http://gqa.bbcook.cn

[T01] Kotlin：Hello World
来源：http://blm.jqgufenzy.top

println("Hello")
来源：http://dcr.gogol.net.cn

[T02] Kotlin：变量
来源：http://xxp.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://alt.vqdsnc.cn

[T03] Kotlin：字符串模板
来源：http://fuo.xylfe.cn

"值: $b"
来源：http://llw.bjfxy.top

[T04] Kotlin：空安全
来源：http://ayl.wangshuangyany.cn

val n: String? = null;  n?.length
来源：http://jns.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://gfq.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kuy.jinghuilouyu.cn

[T06] Kotlin：集合映射
来源：http://ihq.tian-w.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://egg.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://zfw.guowangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bdt.yuxming.cn

[T08] Kotlin：数据类
来源：http://zeh.zhijiandao.cn

data class User(val name: String, val age: Int)
来源：http://bdw.hammf.cn

[T09] Kotlin：扩展函数
来源：http://sol.chenjidiqi.icu

fun String.exclaim() = this + "!"
来源：http://eno.epnwcf.com

[T10] Kotlin：默认参数
来源：http://kyh.fehbvm.com

fun greet(name: String = "World") = "Hi $name"
来源：http://xna.iojbl.cn

[T11] Kotlin：协程
来源：http://luw.nanxuanxn.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qxn.yangfankeji.com

[T12] Kotlin：解构声明
来源：http://czg.jlsjyb.cn

val (a, b) = Pair(1, 2)
来源：http://ejx.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://pun.fzhhl.top

val m = mapOf("a" to 1)
来源：http://orh.guowangkeji.top

[T14] Kotlin：循环
来源：http://mzr.ehwqpu.com

for (i in 1..10) println(i)
来源：http://vfs.shzxlz.cn

[T15] Kotlin：接口
来源：http://uzv.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://vki.zhengqikj.top

[T16] Swift：Hello World
来源：http://lsm.hammf.cn

print("Hello")
来源：http://brh.ivvv.top

[T17] Swift：变量与常量
来源：http://try.tianlin.xyz

var a = 1;  let b = 2
来源：http://jcv.ehwqpu.com

[T18] Swift：字符串插值
来源：http://jwd.jinqigufen.top

"值: \(b)"
来源：http://ewo.tanke756.top

[T19] Swift：可选绑定
来源：http://xgl.zhengqikj.top

if let n = opt { print(n) }
来源：http://lxo.xinyue.icu

[T20] Swift：数组操作
来源：http://ipa.zhoulong.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://bvn.gaohongyu789.top

[T21] Swift：遍历
来源：http://yym.zdbjq.cn

for x in a { print(x) }
来源：http://yeu.zhaomingkeji.xyz

[T22] Swift：字典
来源：http://bye.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://woe.daxiang520.top

[T23] Swift：函数
来源：http://rlg.hywenlv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zhu.sysykeji.top

[T24] Swift：闭包
来源：http://gje.gotoacloud.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://akl.ydjk.org.cn

[T25] Swift：结构体
来源：http://xue.nanxinkj.top

struct P { var x: Int }
来源：http://ncz.c1oappe.top

[T26] Swift：类与重写
来源：http://yum.xingfuxueyuan.xyz

class A: Base { override func f() {} }
来源：http://gqt.quarkkingdee.top

[T27] Swift：错误处理
来源：http://jkd.yj202588.top

do { try f() } catch { print(error) }
来源：http://xrd.daria6918.cn

[T28] Swift：枚举
来源：http://kln.cashguo.top

enum Color { case red, green }
来源：http://tuc.quarkkingdee.top

[T29] Swift：guard 提前返回
来源：http://nnz.ivvv.top

guard let x = opt else { return }
来源：http://moz.ybcxt.top

[T30] Swift：协议
来源：http://nln.wangshuangyany.cn

protocol Shape { func area() -> Double }
来源：http://sjx.birdmap.top

[T31] Lua：Hello World
来源：http://mmu.cucudq.cn

print("Hello")
来源：http://agu.shzxlz.cn

[T32] Lua：局部变量
来源：http://boo.xinyue.icu

local a = 1
来源：http://osv.bjfxy.top

[T33] Lua：表（数组）
来源：http://ozy.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ufq.zhoulong.xyz

[T34] Lua：遍历表
来源：http://pfk.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://goh.zdbjq.cn

[T35] Lua：字典表
来源：http://tjm.ydjk.org.cn

local d = { a = 1 };  d.b = 2
来源：http://tbp.kuanghao11.cn

[T36] Lua：函数
来源：http://rst.sxryk.cn

function add(a, b) return a + b end
来源：http://qup.nanxinkj.top

[T37] Lua：字符串拼接
来源：http://jyu.c1oappe.top

"a" .. "b"
来源：http://cnj.yonumen.top

[T38] Lua：条件
来源：http://mwv.yanxiufei.cn

if x > 0 then print("正") end
来源：http://scj.zhaomingkeji.xyz

[T39] Lua：模式匹配
来源：http://emt.zhaomingkeji.xyz

string.find(s, "%d+")
来源：http://avk.zhengqikj.top

[T40] Lua：元表
来源：http://nvx.hnqzz.top

setmetatable({}, { __index = base })
来源：http://gcx.jinqigfzy.top

[T41] Perl：Hello World
来源：http://ekf.fzhhl.top

print "Hello\n";
来源：http://iye.jiagoushi.top

[T42] Perl：变量类型
来源：http://ifa.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mma.vehdjk.com

[T43] Perl：字符串插值
来源：http://rai.hesvh.cn

"值: $a"
来源：http://vmx.nwbrower.top

[T44] Perl：条件
来源：http://jlc.daria6918.cn

if ($a > 0) { print "正"; }
来源：http://avl.ivvv.top

[T45] Perl：数组遍历
来源：http://xhg.wangdashe.top

for my $x (@arr) { print $x; }
来源：http://tyu.0kj1m.cn

[T46] Perl：哈希操作
来源：http://zov.zhongyouzk.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zaf.meibo888.top

[T47] Perl：正则捕获
来源：http://ofs.316326.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://wzn.kuanghao11.cn

[T48] Perl：正则替换
来源：http://npf.jinghuilouyu.cn

$s =~ s/old/new/g;
来源：http://chu.havefunace.top

[T49] Perl：函数
来源：http://gtb.jyoumei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ygn.bbcook.cn

[T50] Perl：逐行读文件
来源：http://rcl.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xfd.wangdashe.top

while (my $line = <$fh>) { print $line; }
来源：http://lnr.yj202588.top

[T51] Scala：Hello World
来源：http://qlt.hongshengwenyu.top

println("Hello")
来源：http://jwh.xziqi.cn

[T52] Scala：变量
来源：http://uua.zdbjq.cn

val a = 1;  var b = 2
来源：http://jij.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://byx.sweek.top

s"值: $b"
来源：http://isr.hnqzz.top

[T54] Scala：集合映射
来源：http://pjk.hesvh.cn

List(1, 2, 3).map(_ * 2)
来源：http://szu.gzhubu.top

[T55] Scala：集合过滤
来源：http://wsc.jinqigfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://mmy.cheryme.top

[T56] Scala：样例类
来源：http://myc.zdbjq.cn

case class User(name: String, age: Int)
来源：http://onn.ivvv.top

[T57] Scala：模式匹配
来源：http://wqf.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://oxv.xingfuxueyuan.xyz

[T58] Scala：函数定义
来源：http://mhr.zhaomingkeji.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://bex.kuanghao11.cn

[T59] Scala：循环
来源：http://xac.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://kfk.ppjwa.cn

[T60] Scala：折叠
来源：http://aef.ppjwa.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gob.jinghuilouyu.cn

================================================================================
来源：http://rtq.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hce.guannengcc.top

================================================================================
来源：http://aim.snrcjt.cn

[U01] Py：创建虚拟环境
来源：http://uhh.xylfe.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kgf.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://hdb.haohaochexian.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://van.sweek.top

[U03] Py：加载 .env 配置
来源：http://qfw.nanxuanxn.top

from dotenv import load_dotenv; load_dotenv()
来源：http://snd.pycfn.com

[U04] Py：变量调试打印
来源：http://fbq.hnqzz.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ngu.hfpthk.cn

[U05] Py：列表去重且保序
来源：http://vpn.yonumen.top

list(dict.fromkeys(arr))
来源：http://hia.hfpthk.cn

[U06] Py：合并两个字典
来源：http://mqq.chenlongwang.top

{**a, **b}
来源：http://thk.jinqigfzy.top

[U07] Py：反转字典键值
来源：http://zgc.xuetiantiany.cn

{v: k for k, v in d.items()}
来源：http://bvh.yongpay.top

[U08] Py：展平二维列表
来源：http://atc.chenzaomai.com

[y for x in nested for y in x]
来源：http://hts.ehwqpu.com

[U09] Py：字典取最大值的键
来源：http://usf.yueranfly.top

max(d, key=d.get)
来源：http://xzr.zhoulong.xyz

[U10] Py：按值排序字典
来源：http://lnw.zhiwuduotai.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ttc.guannengcc.top

[U11] Py：生成器表达式
来源：http://ivp.jinyuanbaomall.cn

(x * 2 for x in arr)
来源：http://dzg.shangyingyoupin.top

[U12] Py：取出现最多的 3 个元素
来源：http://ctb.jiagoushi.top

Counter(arr).most_common(3)
来源：http://gta.zhijiandao.cn

[U13] Py：固定长度队列
来源：http://eux.jinghuilouyu.cn

deque(maxlen=10)
来源：http://jyq.fehbvm.com

[U14] Py：分组收集到列表
来源：http://fyt.wangdashe.top

defaultdict(list)
来源：http://byn.zhengqikj.top

[U15] Py：高精度计时
来源：http://ndh.shzxlz.cn

t = time.perf_counter()
来源：http://ljj.mhx1999.top

[U16] Py：命令行参数解析
来源：http://qda.zhoulong.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dqy.316326.xyz

[U17] Py：初始化日志
来源：http://yqp.xylfe.cn

logging.basicConfig(level=logging.INFO)
来源：http://wcy.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://oxb.yongpay.top

pat = re.compile(r"\d+")
来源：http://gil.xingfuxueyuan.xyz

[U19] Py：正则替换带回调
来源：http://bjd.ctjpmb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mnq.iojbl.cn

[U20] Py：缓存函数结果
来源：http://dvc.haohaochexian.top

@functools.lru_cache(maxsize=None)
来源：http://qxn.52xcode.cn

[U21] Py：自定义上下文管理器
来源：http://skc.shanyushiyangtech.top

@contextlib.contextmanager
来源：http://cfk.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://fst.ctjpmb.com

list(zip(*m))
来源：http://phs.jinqigfzy.top

[U23] Py：分块读取大文件
来源：http://ajq.meibo888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wrt.andypj.xyz

[U24] Py：路径操作
来源：http://wkj.snrcjt.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bom.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://xuw.daria6918.cn

csv.DictReader(f)
来源：http://nbw.tianlin.xyz

[U26] Py：并发下载
来源：http://qjk.shzxlz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://owz.yanxiufei.cn

[U27] Py：异步 HTTP
来源：http://gas.zhixingplan.top

aiohttp.ClientSession() 配合 async with
来源：http://hec.mhx1999.top

[U28] Py：类型别名
来源：http://agk.shangyingyoupin.top

UserId = int
来源：http://sbo.iojbl.cn

[U29] Py：属性校验
来源：http://vih.epnwcf.com

@property 与 @x.setter 配合
来源：http://ivz.tianlin.xyz

[U30] Py：数据类
来源：http://emk.aibaodan.cn

@dataclass(slots=True)
来源：http://jlc.gotoacloud.top

[U31] Py：单测
来源：http://mbx.aibaodan.cn

python -m pytest -q
来源：http://pgh.zhoulong.xyz

[U32] Py：代码格式化
来源：http://bwg.xinyue.icu

ruff format . && ruff check --fix .
来源：http://nkb.zhoulong.xyz

[U33] Py：打包发布
来源：http://qxk.chenlongwang.top

python -m build  （依赖 pyproject.toml）
来源：http://jxt.ybcxt.top

[U34] Py：判断编码
来源：http://xch.shangyingyoupin.top

chardet.detect(raw)
来源：http://hpr.hywenlv.cn

[U35] Py：发送邮件
来源：http://qpo.c1oappe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mpi.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://vzq.tarul.cn

schedule.every(10).minutes.do(job)
来源：http://mgt.daria6918.cn

[U37] Py：读写 Excel
来源：http://jqb.vehdjk.com

pandas.read_excel / DataFrame.to_excel
来源：http://cma.epnwcf.com

[U38] Py：获取脚本所在目录
来源：http://aht.mhx1999.top

Path(__file__).resolve().parent
来源：http://zby.jlsjyb.cn

[U39] Py：判断是否在交互环境
来源：http://tfg.xziqi.cn

sys.stdout.isatty()
来源：http://pfk.andypj.xyz

[U40] Py：打印到标准错误
来源：http://wdu.yuxming.cn

print("err", file=sys.stderr)
来源：http://dsq.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://kfx.ppjwa.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bjg.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://imo.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lft.dianchejie.cn

[U43] PHP：声明命名空间
来源：http://vtf.daria6918.cn

namespace App\Http;
来源：http://fyt.quarkkingdee.top

[U44] PHP：开启严格类型
来源：http://xpv.haohaochexian.top

declare(strict_types=1);
来源：http://moj.vehdjk.com

[U45] PHP：类型声明与返回类型
来源：http://rxq.hcnkem.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://lnj.yongpay.top

[U46] PHP：可空类型
来源：http://mdy.hesvh.cn

?string $name = null
来源：http://pdv.xingfuxueyuan.xyz


<!-- 参考信息 -->