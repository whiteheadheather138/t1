代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://gpt.xuetiantiany.cn

[S23] C：随机数
来源：http://qzp.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fqs.sweek.top

[S24] C：获取本地时间
来源：http://qoe.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bfu.cheryme.top

[S25] C：内存拷贝
来源：http://vkg.yanxiufei.cn

memcpy(dst, src, n);
来源：http://qzn.tarul.cn

[S26] C：内存清零
来源：http://tzi.fzhhl.top

memset(a, 0, sizeof a);
来源：http://haj.havefunace.top

[S27] C：定义常量
来源：http://mmy.wangdashe.top

const double PI = 3.14159;
来源：http://but.vqdsnc.cn

[S28] C：静态变量
来源：http://rqf.chenjidiqi.icu

static int counter = 0;
来源：http://hlk.yfazqb.com

[S29] C：变参函数
来源：http://quz.cheryme.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lel.redwolf501.top

[S30] C：头文件保护
来源：http://plk.aibaodan.cn

#ifndef X_H
来源：http://zqu.zdqjudy.top

#define X_H
来源：http://zjz.jinghuilouyu.cn

#endif
来源：http://vih.yj20258.top

[S31] C++：Hello World
来源：http://wwi.cdnleiting.top

#include <iostream>
来源：http://xzs.cashguo.top

int main() { std::cout << "Hello\n"; }
来源：http://cig.tanke756.top

[S32] C++：字符串
来源：http://uux.hesvh.cn

std::string s = "hi";  s += "!";
来源：http://lev.chenjidiqi.icu

[S33] C++：vector 增删
来源：http://jvy.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bdr.sjlbkw.cn

[S34] C++：遍历 vector
来源：http://sgy.pycfn.com

for (auto &x : v) { std::cout << x; }
来源：http://hjp.daria6918.cn

[S35] C++：map
来源：http://dbz.fktsv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vpr.ybcxt.top

[S36] C++：unordered_map
来源：http://dhe.vqdsnc.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vqo.andypj.xyz

[S37] C++：set
来源：http://nwh.jianghu66.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yez.zhixingplan.top

[S38] C++：排序
来源：http://quh.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://phb.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://hkr.smart0.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bob.aibaodan.cn

[S40] C++：查找元素
来源：http://jud.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iyn.zhaomingkeji.xyz

[S41] C++：类与构造函数
来源：http://wdb.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mzd.nanxinkj.top

[S42] C++：继承与虚函数
来源：http://zmd.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://ndb.sweek.top

[S43] C++：智能指针
来源：http://asz.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://fzj.chenlongwang.top

[S44] C++：引用传参
来源：http://qui.meibo888.top

void inc(int &x) { ++x; }
来源：http://don.cdnleiting.top

[S45] C++：lambda
来源：http://wvm.ivvv.top

auto add = [](int a, int b) { return a + b; };
来源：http://qde.sxryk.cn

[S46] C++：函数模板
来源：http://mlv.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hah.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://mcz.yj20258.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sdw.cashguo.top

[S48] C++：逐行读文件
来源：http://glk.cdnleiting.top

std::ifstream in("a.txt");  std::string line;
来源：http://kbx.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://bbd.zycfv.cn

[S49] C++：写文件
来源：http://ofq.jlsjyb.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zzk.mhx1999.top

[S50] C++：格式化数字
来源：http://jqo.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nht.daria6918.cn

[S51] C++：显式类型转换
来源：http://mkv.xylfe.cn

static_cast<double>(a) / b
来源：http://vke.daxiang520.top

[S52] C++：const 与 noexcept
来源：http://gxk.zhoulong.xyz

int size() const noexcept { return n_; }
来源：http://pss.fengsongda.top

[S53] C++：移动语义
来源：http://yje.tian-w.cn

std::vector<int> w = std::move(v);
来源：http://yof.52xcode.cn

[S54] C++：异常处理
来源：http://tgg.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iuy.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://dgj.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://svp.ivvv.top

[S56] C++：optional
来源：http://ifz.chenjidiqi.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fyu.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://vnd.zdbjq.cn

constexpr int N = 10;
来源：http://aik.hesvh.cn

[S58] C++：命名空间
来源：http://gky.shuidangran.top

namespace ns { int f() { return 1; } }
来源：http://zcu.9152youxi.cn

[S59] C++：静态断言
来源：http://qnh.jyoumei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yks.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://txa.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iym.zhengqikj.top

================================================================================
来源：http://fyv.cqqwz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dna.vqdsnc.cn

================================================================================
来源：http://bwg.shuidangran.top

[T01] Kotlin：Hello World
来源：http://dtf.jinyuanbaomall.cn

println("Hello")
来源：http://ceh.redwolf501.top

[T02] Kotlin：变量
来源：http://ipg.zhijiandao.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://feu.chenzaomai.com

[T03] Kotlin：字符串模板
来源：http://vrd.xinyue.icu

"值: $b"
来源：http://ppe.fengsongda.top

[T04] Kotlin：空安全
来源：http://fxa.yuxming.cn

val n: String? = null;  n?.length
来源：http://mli.jiagoushi.top

[T05] Kotlin：when 表达式
来源：http://dqf.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://das.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://eut.ivvv.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wov.hcnkem.com

[T07] Kotlin：集合过滤
来源：http://mub.zdqjudy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://elf.tian-w.cn

[T08] Kotlin：数据类
来源：http://ajp.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://izy.feifeiyinyue.top

[T09] Kotlin：扩展函数
来源：http://nkm.zhengqikj.top

fun String.exclaim() = this + "!"
来源：http://dzi.yuxming.cn

[T10] Kotlin：默认参数
来源：http://xgh.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jhx.yonumen.top

[T11] Kotlin：协程
来源：http://cmn.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://kbo.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://oxf.cashguo.top

val (a, b) = Pair(1, 2)
来源：http://efv.chenjidiqi.icu

[T13] Kotlin：只读 Map
来源：http://clz.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://pjy.vqdsnc.cn

[T14] Kotlin：循环
来源：http://peu.ydzc1.top

for (i in 1..10) println(i)
来源：http://ndp.pycfn.com

[T15] Kotlin：接口
来源：http://eic.yj20258.top

interface Shape { fun area(): Double }
来源：http://nwe.hnqzz.top

[T16] Swift：Hello World
来源：http://ynm.havefunace.top

print("Hello")
来源：http://zpr.mhx1999.top

[T17] Swift：变量与常量
来源：http://sgp.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://xih.xinyue.icu

[T18] Swift：字符串插值
来源：http://mtr.jianghu66.top

"值: \(b)"
来源：http://xgg.bjfxy.top

[T19] Swift：可选绑定
来源：http://vji.dianchejie.cn

if let n = opt { print(n) }
来源：http://mwl.pycfn.com

[T20] Swift：数组操作
来源：http://row.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lrm.c1oappe.top

[T21] Swift：遍历
来源：http://uta.cheryme.top

for x in a { print(x) }
来源：http://mwq.yongpay.top

[T22] Swift：字典
来源：http://ftc.yuxming.cn

var d = ["a": 1];  d["b"] = 2
来源：http://eki.dianchejie.cn

[T23] Swift：函数
来源：http://woi.xziqi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://atg.xylfe.cn

[T24] Swift：闭包
来源：http://hgk.vehdjk.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://pvn.cdnleiting.top

[T25] Swift：结构体
来源：http://iwo.quarkkingdee.top

struct P { var x: Int }
来源：http://uwb.zdqjudy.top

[T26] Swift：类与重写
来源：http://oaj.ybcxt.top

class A: Base { override func f() {} }
来源：http://puz.yfazqb.com

[T27] Swift：错误处理
来源：http://vey.wangshuangyany.cn

do { try f() } catch { print(error) }
来源：http://mqu.hammf.cn

[T28] Swift：枚举
来源：http://toa.bbcook.cn

enum Color { case red, green }
来源：http://ans.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://jxd.nwbrower.top

guard let x = opt else { return }
来源：http://evo.yongpay.top

[T30] Swift：协议
来源：http://qzi.sysykeji.top

protocol Shape { func area() -> Double }
来源：http://ppp.jianghu66.top

[T31] Lua：Hello World
来源：http://tbu.sysykeji.top

print("Hello")
来源：http://clf.birdmap.top

[T32] Lua：局部变量
来源：http://acb.kuanghao11.cn

local a = 1
来源：http://apc.gotoacloud.top

[T33] Lua：表（数组）
来源：http://lih.cqqwz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qnu.havefunace.top

[T34] Lua：遍历表
来源：http://ekx.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pts.hnqzz.top

[T35] Lua：字典表
来源：http://vew.havefunace.top

local d = { a = 1 };  d.b = 2
来源：http://rzw.sysykeji.top

[T36] Lua：函数
来源：http://oah.feifeiyinyue.top

function add(a, b) return a + b end
来源：http://ivo.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://nac.shuidangran.top

"a" .. "b"
来源：http://hjh.gzhubu.top

[T38] Lua：条件
来源：http://kaf.yj20258.top

if x > 0 then print("正") end
来源：http://bba.tian-w.cn

[T39] Lua：模式匹配
来源：http://yxd.uphjek.com

string.find(s, "%d+")
来源：http://hgj.hesvh.cn

[T40] Lua：元表
来源：http://qok.guowangkeji.top

setmetatable({}, { __index = base })
来源：http://nrr.nanxinkj.top

[T41] Perl：Hello World
来源：http://otd.sufxvd.cn

print "Hello\n";
来源：http://npb.zdbjq.cn

[T42] Perl：变量类型
来源：http://yep.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sdw.hnxiangtu.top

[T43] Perl：字符串插值
来源：http://lmj.bbcook.cn

"值: $a"
来源：http://hjx.yonumen.top

[T44] Perl：条件
来源：http://sas.yj202588.top

if ($a > 0) { print "正"; }
来源：http://xhs.birdmap.top

[T45] Perl：数组遍历
来源：http://jej.yfazqb.com

for my $x (@arr) { print $x; }
来源：http://ffz.shzxlz.cn

[T46] Perl：哈希操作
来源：http://mjc.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bxx.hnqzz.top

[T47] Perl：正则捕获
来源：http://rnd.andypj.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://xma.feifeiyinyue.top

[T48] Perl：正则替换
来源：http://mvf.0kj1m.cn

$s =~ s/old/new/g;
来源：http://gya.daxiang520.top

[T49] Perl：函数
来源：http://gsv.jianghu66.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xji.cucudq.cn

[T50] Perl：逐行读文件
来源：http://qmr.dianchejie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://huf.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://zwv.bjfxy.top

[T51] Scala：Hello World
来源：http://gel.quarkkingdee.top

println("Hello")
来源：http://bqh.yuxming.cn

[T52] Scala：变量
来源：http://xfq.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://usm.epnwcf.com

[T53] Scala：字符串插值
来源：http://wpw.hnxiangtu.top

s"值: $b"
来源：http://tvf.sufxvd.cn

[T54] Scala：集合映射
来源：http://ozt.52xcode.cn

List(1, 2, 3).map(_ * 2)
来源：http://ozu.zdbjq.cn

[T55] Scala：集合过滤
来源：http://yjk.andypj.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://yxp.yuanzhike.top

[T56] Scala：样例类
来源：http://jlu.yongpay.top

case class User(name: String, age: Int)
来源：http://mhw.pycfn.com

[T57] Scala：模式匹配
来源：http://bex.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://emn.shangyingyoupin.top

[T58] Scala：函数定义
来源：http://nuo.hnqzz.top

def add(a: Int, b: Int): Int = a + b
来源：http://mju.ctjpmb.com

[T59] Scala：循环
来源：http://ttb.jiagoushi.top

for (i <- 1 to 10) println(i)
来源：http://uex.chenjidiqi.icu

[T60] Scala：折叠
来源：http://nnq.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qrq.cdnleiting.top

================================================================================
来源：http://lzr.cqqwz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://egi.mhx1999.top

================================================================================
来源：http://uqr.hesvh.cn

[U01] Py：创建虚拟环境
来源：http://wdu.hysaishi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xsi.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://tve.tianlin.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ajh.jinqigfzy.top

[U03] Py：加载 .env 配置
来源：http://lsn.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qke.kuanghao11.cn

[U04] Py：变量调试打印
来源：http://skd.fktsv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://trr.hesvh.cn

[U05] Py：列表去重且保序
来源：http://pdz.yj20258888.top

list(dict.fromkeys(arr))
来源：http://sec.andypj.xyz

[U06] Py：合并两个字典
来源：http://gvl.jinqigufen.top

{**a, **b}
来源：http://oob.cashguo.top

[U07] Py：反转字典键值
来源：http://glv.aibaodan.cn

{v: k for k, v in d.items()}
来源：http://ijf.chenlongwang.top

[U08] Py：展平二维列表
来源：http://qup.uphjek.com

[y for x in nested for y in x]
来源：http://alm.iojbl.cn

[U09] Py：字典取最大值的键
来源：http://wep.gaohongyu789.top

max(d, key=d.get)
来源：http://euu.haohaochexian.top

[U10] Py：按值排序字典
来源：http://dee.iojbl.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qov.shuidangran.top

[U11] Py：生成器表达式
来源：http://thp.wangdashe.top

(x * 2 for x in arr)
来源：http://sqg.gogol.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jxu.hongshengwenyu.top

Counter(arr).most_common(3)
来源：http://ndy.aibaodan.cn

[U13] Py：固定长度队列
来源：http://gfc.cdnleiting.top

deque(maxlen=10)
来源：http://hky.yonumen.top

[U14] Py：分组收集到列表
来源：http://slt.haohaochexian.top

defaultdict(list)
来源：http://xhr.ctjpmb.com

[U15] Py：高精度计时
来源：http://plk.yvedp.cn

t = time.perf_counter()
来源：http://dpx.yueranfly.top

[U16] Py：命令行参数解析
来源：http://mlp.hcnkem.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kow.zycfv.cn

[U17] Py：初始化日志
来源：http://swx.yj202588.top

logging.basicConfig(level=logging.INFO)
来源：http://tac.shuidangran.top

[U18] Py：预编译正则
来源：http://obv.zhiwuduotai.top

pat = re.compile(r"\d+")
来源：http://ipb.vehdjk.com

[U19] Py：正则替换带回调
来源：http://cvz.nanxinkj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nmm.dashuyun.cn

[U20] Py：缓存函数结果
来源：http://fju.zhiwuduotai.top

@functools.lru_cache(maxsize=None)
来源：http://sic.52xcode.cn

[U21] Py：自定义上下文管理器
来源：http://rnx.fanxiaobao.xyz

@contextlib.contextmanager
来源：http://tnu.9152youxi.cn

[U22] Py：矩阵转置
来源：http://cbq.epnwcf.com

list(zip(*m))
来源：http://rbe.zdqjudy.top

[U23] Py：分块读取大文件
来源：http://ewh.aizwys.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://esb.haohaochexian.top

[U24] Py：路径操作
来源：http://mwf.hcnkem.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nlv.epnwcf.com

[U25] Py：CSV 按字典读
来源：http://ero.havefunace.top

csv.DictReader(f)
来源：http://oap.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://lgx.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bjw.ctjpmb.com

[U27] Py：异步 HTTP
来源：http://fyo.andypj.xyz

aiohttp.ClientSession() 配合 async with
来源：http://asi.xuanzx.com

[U28] Py：类型别名
来源：http://unh.meibo888.top

UserId = int
来源：http://yzy.cucudq.cn

[U29] Py：属性校验
来源：http://mmm.cdnleiting.top

@property 与 @x.setter 配合
来源：http://lod.pycfn.com

[U30] Py：数据类
来源：http://xgg.ivvv.top

@dataclass(slots=True)
来源：http://hbe.feifeiyinyue.top

[U31] Py：单测
来源：http://mgx.tianlin.xyz

python -m pytest -q
来源：http://wuo.guannengcc.top

[U32] Py：代码格式化
来源：http://fmx.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://dvd.hnqzz.top

[U33] Py：打包发布
来源：http://mdy.zhijiandao.cn

python -m build  （依赖 pyproject.toml）
来源：http://cbd.hywenlv.cn

[U34] Py：判断编码
来源：http://lld.yfazqb.com

chardet.detect(raw)
来源：http://tnk.hesvh.cn

[U35] Py：发送邮件
来源：http://yjb.tanke756.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cjp.uphjek.com

[U36] Py：定时任务
来源：http://xyu.gzhubu.top

schedule.every(10).minutes.do(job)
来源：http://jvc.nanxuanxn.top

[U37] Py：读写 Excel
来源：http://jzv.xuanzx.com

pandas.read_excel / DataFrame.to_excel
来源：http://nlz.dashuyun.cn

[U38] Py：获取脚本所在目录
来源：http://mwb.bjfxy.top

Path(__file__).resolve().parent
来源：http://rdm.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://wik.yonumen.top

sys.stdout.isatty()
来源：http://otr.jinqigfzy.top

[U40] Py：打印到标准错误
来源：http://nms.cqqwz.cn

print("err", file=sys.stderr)
来源：http://dyu.tianlin.xyz

[U41] PHP：初始化 Composer 项目
来源：http://leb.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://azo.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://uli.zhijiandao.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uka.yuxming.cn

[U43] PHP：声明命名空间
来源：http://gks.zdbjq.cn

namespace App\Http;
来源：http://efr.zhixingplan.top

[U44] PHP：开启严格类型
来源：http://ptp.pengpengdd.cyou

declare(strict_types=1);
来源：http://urj.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://ubk.fzhhl.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://oec.yj202588.top

[U46] PHP：可空类型
来源：http://lsa.tarul.cn

?string $name = null
来源：http://tbz.gzhubu.top


<!-- 参考信息 -->