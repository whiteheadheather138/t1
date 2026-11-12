代发 wailian999

static int counter = 0;
来源：http://krk.tarul.cn

[S29] C：变参函数
来源：http://rsm.zhaomingkeji.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kga.fehbvm.com

[S30] C：头文件保护
来源：http://exn.zhengqikj.top

#ifndef X_H
来源：http://jgv.shangyingyoupin.top

#define X_H
来源：http://jzc.tanke756.top

#endif
来源：http://mmf.jinqigufen.top

[S31] C++：Hello World
来源：http://wax.aibaodan.cn

#include <iostream>
来源：http://cog.52xcode.cn

int main() { std::cout << "Hello\n"; }
来源：http://kgq.bjfxy.top

[S32] C++：字符串
来源：http://dyu.ywan-chungtsiang.top

std::string s = "hi";  s += "!";
来源：http://igm.jianghu66.top

[S33] C++：vector 增删
来源：http://ufc.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fpf.yuanzhike.top

[S34] C++：遍历 vector
来源：http://igr.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://jgq.bjfxy.top

[S35] C++：map
来源：http://qlb.fzhhl.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vdj.ehwqpu.com

[S36] C++：unordered_map
来源：http://quk.wangdashe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dge.smart0.xyz

[S37] C++：set
来源：http://jsy.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://apt.kuanghao11.cn

[S38] C++：排序
来源：http://oac.tian-w.cn

std::sort(v.begin(), v.end());
来源：http://rah.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://vab.birdmap.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://emk.zhongyouzk.top

[S40] C++：查找元素
来源：http://vka.zhiwuduotai.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cqw.aibaodan.cn

[S41] C++：类与构造函数
来源：http://pxg.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tof.ivvv.top

[S42] C++：继承与虚函数
来源：http://ltu.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://gpa.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://xnv.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://rkr.52xcode.cn

[S44] C++：引用传参
来源：http://die.hammf.cn

void inc(int &x) { ++x; }
来源：http://ltc.zdbjq.cn

[S45] C++：lambda
来源：http://erq.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://ykc.hywenlv.cn

[S46] C++：函数模板
来源：http://fnd.yangfankeji.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://poa.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://ytu.jinqigfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zlu.xuanzx.com

[S48] C++：逐行读文件
来源：http://qjd.shuidangran.top

std::ifstream in("a.txt");  std::string line;
来源：http://lon.jqgufenzy.top

while (std::getline(in, line)) { }
来源：http://hbz.chenlongwang.top

[S49] C++：写文件
来源：http://bou.hnqzz.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rkf.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://dck.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sul.hongshengwenyu.top

[S51] C++：显式类型转换
来源：http://lwp.vqdsnc.cn

static_cast<double>(a) / b
来源：http://obt.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://cky.nwbrower.top

int size() const noexcept { return n_; }
来源：http://ixw.zdbjq.cn

[S53] C++：移动语义
来源：http://gaw.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://iiv.wangshuangyany.cn

[S54] C++：异常处理
来源：http://bcx.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://joc.cdnleiting.top

[S55] C++：结构化绑定
来源：http://vyz.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qob.zdqjudy.top

[S56] C++：optional
来源：http://avf.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jzu.yuanzhike.top

[S57] C++：编译期常量
来源：http://bax.jinghuilouyu.cn

constexpr int N = 10;
来源：http://eam.yfazqb.com

[S58] C++：命名空间
来源：http://kpc.zdqjudy.top

namespace ns { int f() { return 1; } }
来源：http://mot.pengpengdd.cyou

[S59] C++：静态断言
来源：http://pku.jinqigufen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kzy.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://nia.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mel.quarkkingdee.top

================================================================================
来源：http://qzk.c1oappe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hvt.sjlbkw.cn

================================================================================
来源：http://ncu.ppjwa.cn

[T01] Kotlin：Hello World
来源：http://fzl.0kj1m.cn

println("Hello")
来源：http://dor.shanyushiyangkeji.top

[T02] Kotlin：变量
来源：http://ilm.daria6918.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wtf.cheryme.top

[T03] Kotlin：字符串模板
来源：http://ppp.xuanzx.com

"值: $b"
来源：http://klz.jianghu66.top

[T04] Kotlin：空安全
来源：http://pmb.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://zit.cdnleiting.top

[T05] Kotlin：when 表达式
来源：http://zwh.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gwm.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://dyc.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://fbg.sjlbkw.cn

[T07] Kotlin：集合过滤
来源：http://jxf.jinyuanbaomall.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ano.zhongyouzk.top

[T08] Kotlin：数据类
来源：http://ote.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://vhw.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://hsu.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://ryf.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://kfp.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jzw.zhoulong.xyz

[T11] Kotlin：协程
来源：http://vgc.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dif.nwbrower.top

[T12] Kotlin：解构声明
来源：http://cck.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://gzx.kuanghao11.cn

[T13] Kotlin：只读 Map
来源：http://jys.shanyushiyangtech.top

val m = mapOf("a" to 1)
来源：http://dbt.cucudq.cn

[T14] Kotlin：循环
来源：http://mzl.c1oappe.top

for (i in 1..10) println(i)
来源：http://prz.hnxiangtu.top

[T15] Kotlin：接口
来源：http://okt.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://vrm.zhengqikj.top

[T16] Swift：Hello World
来源：http://pwu.dianchejie.cn

print("Hello")
来源：http://xvt.sweek.top

[T17] Swift：变量与常量
来源：http://fba.zhijiandao.cn

var a = 1;  let b = 2
来源：http://yvh.yj202588.top

[T18] Swift：字符串插值
来源：http://bqz.fktsv.cn

"值: \(b)"
来源：http://lmv.fehbvm.com

[T19] Swift：可选绑定
来源：http://avb.ydzc1.top

if let n = opt { print(n) }
来源：http://eip.gogol.net.cn

[T20] Swift：数组操作
来源：http://iul.cashguo.top

var a = [1, 2, 3];  a.append(4)
来源：http://cbu.daxiang520.top

[T21] Swift：遍历
来源：http://bii.aibaodan.cn

for x in a { print(x) }
来源：http://dzw.bjfxy.top

[T22] Swift：字典
来源：http://vye.dianchejie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://veu.tanke756.top

[T23] Swift：函数
来源：http://gqn.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ves.meibo888.top

[T24] Swift：闭包
来源：http://uyt.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://aii.zhengqikj.top

[T25] Swift：结构体
来源：http://lck.dashuyun.cn

struct P { var x: Int }
来源：http://tdn.xuetiantiany.cn

[T26] Swift：类与重写
来源：http://pof.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://dkr.jinqigfzy.top

[T27] Swift：错误处理
来源：http://xjl.cheryme.top

do { try f() } catch { print(error) }
来源：http://tby.sxryk.cn

[T28] Swift：枚举
来源：http://nph.sysykeji.top

enum Color { case red, green }
来源：http://ezp.tianlin.xyz

[T29] Swift：guard 提前返回
来源：http://qvo.zhengqikj.top

guard let x = opt else { return }
来源：http://dgq.tarul.cn

[T30] Swift：协议
来源：http://omj.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://pkm.shuidangran.top

[T31] Lua：Hello World
来源：http://wfv.jianghu66.top

print("Hello")
来源：http://fxx.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://nov.xziqi.cn

local a = 1
来源：http://pjl.kuanghao11.cn

[T33] Lua：表（数组）
来源：http://xgh.hongshengwenyu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pqo.cqqwz.cn

[T34] Lua：遍历表
来源：http://ddm.gogol.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zzc.sufxvd.cn

[T35] Lua：字典表
来源：http://baz.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://nos.uphjek.com

[T36] Lua：函数
来源：http://qre.chenlongwang.top

function add(a, b) return a + b end
来源：http://cbg.cheryme.top

[T37] Lua：字符串拼接
来源：http://sjc.cdnleiting.top

"a" .. "b"
来源：http://ypo.shangyingyoupin.top

[T38] Lua：条件
来源：http://tig.ybcxt.top

if x > 0 then print("正") end
来源：http://ubx.epnwcf.com

[T39] Lua：模式匹配
来源：http://dgd.tian-w.cn

string.find(s, "%d+")
来源：http://uci.ppjwa.cn

[T40] Lua：元表
来源：http://tab.sxryk.cn

setmetatable({}, { __index = base })
来源：http://exe.meibo888.top

[T41] Perl：Hello World
来源：http://lkg.smart0.xyz

print "Hello\n";
来源：http://baq.xuanzx.com

[T42] Perl：变量类型
来源：http://ueb.bbcook.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://irb.ivvv.top

[T43] Perl：字符串插值
来源：http://vlj.hongshengwenyu.top

"值: $a"
来源：http://nis.shanyushiyangkeji.top

[T44] Perl：条件
来源：http://zef.zhixingplan.top

if ($a > 0) { print "正"; }
来源：http://ygn.yvedp.cn

[T45] Perl：数组遍历
来源：http://pze.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://oqs.yj20258888.top

[T46] Perl：哈希操作
来源：http://qio.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vjy.xuetiantiany.cn

[T47] Perl：正则捕获
来源：http://bgg.aibaodan.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wfo.birdmap.top

[T48] Perl：正则替换
来源：http://pdx.haohaochexian.top

$s =~ s/old/new/g;
来源：http://lfm.ybcxt.top

[T49] Perl：函数
来源：http://uxd.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fwg.zycfv.cn

[T50] Perl：逐行读文件
来源：http://zlv.fktsv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://htn.hywenlv.cn

while (my $line = <$fh>) { print $line; }
来源：http://obp.zdbjq.cn

[T51] Scala：Hello World
来源：http://udd.316326.xyz

println("Hello")
来源：http://xxg.yangfankeji.com

[T52] Scala：变量
来源：http://rab.yangfankeji.com

val a = 1;  var b = 2
来源：http://yuf.yj20258888.top

[T53] Scala：字符串插值
来源：http://xfg.jinqigufen.top

s"值: $b"
来源：http://bnr.sysykeji.top

[T54] Scala：集合映射
来源：http://mfc.nanxinkj.top

List(1, 2, 3).map(_ * 2)
来源：http://tuu.sxryk.cn

[T55] Scala：集合过滤
来源：http://hnx.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://gwk.zhoulong.xyz

[T56] Scala：样例类
来源：http://vhz.pycfn.com

case class User(name: String, age: Int)
来源：http://rfw.quarkkingdee.top

[T57] Scala：模式匹配
来源：http://izo.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://zrm.sxryk.cn

[T58] Scala：函数定义
来源：http://twk.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yah.cheryme.top

[T59] Scala：循环
来源：http://xtz.aibaodan.cn

for (i <- 1 to 10) println(i)
来源：http://kcq.zhixingplan.top

[T60] Scala：折叠
来源：http://fzx.shanyushiyangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jsh.ehwqpu.com

================================================================================
来源：http://ubu.zhoulong.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yjm.zhiwuduotai.top

================================================================================
来源：http://sys.jqgfzy.top

[U01] Py：创建虚拟环境
来源：http://jip.hnqzz.top

python -m venv .venv && source .venv/bin/activate
来源：http://rwp.hysaishi.cn

[U02] Py：导出 / 安装依赖
来源：http://yvv.shanyushiyangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wmr.yj202588.top

[U03] Py：加载 .env 配置
来源：http://not.quarkkingdee.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hgw.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://bab.yvedp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://obt.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://yvh.xingfuxueyuan.xyz

list(dict.fromkeys(arr))
来源：http://zfm.gzhubu.top

[U06] Py：合并两个字典
来源：http://pmf.xinyue.icu

{**a, **b}
来源：http://ziq.zdbjq.cn

[U07] Py：反转字典键值
来源：http://rqh.aizwys.cn

{v: k for k, v in d.items()}
来源：http://kfh.yfazqb.com

[U08] Py：展平二维列表
来源：http://zht.cdnleiting.top

[y for x in nested for y in x]
来源：http://eef.vehdjk.com

[U09] Py：字典取最大值的键
来源：http://ssa.ydzc1.top

max(d, key=d.get)
来源：http://bfn.xziqi.cn

[U10] Py：按值排序字典
来源：http://yuh.meibo888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zid.nanxinkj.top

[U11] Py：生成器表达式
来源：http://hfn.zhoulong.xyz

(x * 2 for x in arr)
来源：http://mvk.quarkkingdee.top

[U12] Py：取出现最多的 3 个元素
来源：http://obz.52xcode.cn

Counter(arr).most_common(3)
来源：http://ywc.hywenlv.cn

[U13] Py：固定长度队列
来源：http://gmq.bjfxy.top

deque(maxlen=10)
来源：http://gkp.jqgufenzy.top

[U14] Py：分组收集到列表
来源：http://ays.shangyingyoupin.top

defaultdict(list)
来源：http://wcx.jqgufenzy.top

[U15] Py：高精度计时
来源：http://awa.daxiang520.top

t = time.perf_counter()
来源：http://iew.wangshuangyany.cn

[U16] Py：命令行参数解析
来源：http://wzf.mhx1999.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qlf.fktsv.cn

[U17] Py：初始化日志
来源：http://kyj.wangshuangyany.cn

logging.basicConfig(level=logging.INFO)
来源：http://idd.fehbvm.com

[U18] Py：预编译正则
来源：http://csh.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://jlf.nanxuanxn.top

[U19] Py：正则替换带回调
来源：http://axu.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://anp.vqdsnc.cn

[U20] Py：缓存函数结果
来源：http://hur.zycfv.cn

@functools.lru_cache(maxsize=None)
来源：http://nqz.jinqigfzy.top

[U21] Py：自定义上下文管理器
来源：http://mrw.nwbrower.top

@contextlib.contextmanager
来源：http://nkl.zhengqikj.top

[U22] Py：矩阵转置
来源：http://mva.hnxiangtu.top

list(zip(*m))
来源：http://ctd.chenjidiqi.icu

[U23] Py：分块读取大文件
来源：http://nbb.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dih.zhiwuduotai.top

[U24] Py：路径操作
来源：http://mfy.zycfv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kwi.yanxiufei.cn

[U25] Py：CSV 按字典读
来源：http://jxa.aizwys.cn

csv.DictReader(f)
来源：http://wgo.svipenyu.cn

[U26] Py：并发下载
来源：http://gzh.fzhhl.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xig.uphjek.com

[U27] Py：异步 HTTP
来源：http://fro.tanke756.top

aiohttp.ClientSession() 配合 async with
来源：http://bcp.andypj.xyz

[U28] Py：类型别名
来源：http://bde.sjlbkw.cn

UserId = int
来源：http://den.ppjwa.cn

[U29] Py：属性校验
来源：http://zvo.hnqzz.top

@property 与 @x.setter 配合
来源：http://kuw.cqqwz.cn

[U30] Py：数据类
来源：http://qgx.daxiang520.top

@dataclass(slots=True)
来源：http://dkk.guannengcc.top

[U31] Py：单测
来源：http://hny.yj20258888.top

python -m pytest -q
来源：http://aks.jianghu66.top

[U32] Py：代码格式化
来源：http://bcf.xingfuxueyuan.xyz

ruff format . && ruff check --fix .
来源：http://fco.meibo888.top

[U33] Py：打包发布
来源：http://vdq.wangshuangyany.cn

python -m build  （依赖 pyproject.toml）
来源：http://ipp.yj20258888.top

[U34] Py：判断编码
来源：http://pru.sufxvd.cn

chardet.detect(raw)
来源：http://lsz.snrcjt.cn

[U35] Py：发送邮件
来源：http://wgh.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vio.xingfuxueyuan.xyz

[U36] Py：定时任务
来源：http://rhv.chenjidiqi.icu

schedule.every(10).minutes.do(job)
来源：http://koi.bbcook.cn

[U37] Py：读写 Excel
来源：http://qkv.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wzo.zhongyouzk.top

[U38] Py：获取脚本所在目录
来源：http://mjz.tianlin.xyz

Path(__file__).resolve().parent
来源：http://xnz.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://jhi.yonumen.top

sys.stdout.isatty()
来源：http://asc.meibo888.top

[U40] Py：打印到标准错误
来源：http://rwk.cucudq.cn

print("err", file=sys.stderr)
来源：http://lkf.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://dhp.uphjek.com

composer init;  composer require guzzlehttp/guzzle
来源：http://tov.316326.xyz

[U42] PHP：PSR-4 自动加载
来源：http://yub.daria6918.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ifv.sweek.top

[U43] PHP：声明命名空间
来源：http://mpt.daxiang520.top

namespace App\Http;
来源：http://qvd.xziqi.cn

[U44] PHP：开启严格类型
来源：http://ahg.316326.xyz

declare(strict_types=1);
来源：http://vuh.hnxiangtu.top

[U45] PHP：类型声明与返回类型
来源：http://ekr.yvedp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jcr.iojbl.cn

[U46] PHP：可空类型
来源：http://ato.hesvh.cn

?string $name = null
来源：http://jia.sxryk.cn

[U47] PHP：联合类型
来源：http://bel.smart0.xyz

int|string $id
来源：http://ybp.zhongyouzk.top

[U48] PHP：纯枚举
来源：http://orv.gaohongyu789.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fgv.nanxinkj.top

[U49] PHP：只读属性
来源：http://kls.iojbl.cn

public readonly string $name
来源：http://lrv.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://jjt.chenzaomai.com

public function __construct(private int $id) {}
来源：http://psq.havefunace.top

[U51] PHP：数组解构
来源：http://eun.fehbvm.com

[$a, $b] = $arr;
来源：http://bfr.gaohongyu789.top

[U52] PHP：箭头函数
来源：http://faz.jlsjyb.cn

$double = fn($x) => $x * 2;
来源：http://kxq.fzhhl.top


<!-- 参考信息 -->