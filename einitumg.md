代发 wailian999

memset(a, 0, sizeof a);
来源：http://uir.jianghu66.top

[S27] C：定义常量
来源：http://jge.ppjwa.cn

const double PI = 3.14159;
来源：http://ihd.zhaomingkeji.xyz

[S28] C：静态变量
来源：http://skq.ydzc1.top

static int counter = 0;
来源：http://dve.hammf.cn

[S29] C：变参函数
来源：http://vnq.gotoacloud.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oxb.daria6918.cn

[S30] C：头文件保护
来源：http://ygh.iojbl.cn

#ifndef X_H
来源：http://qxz.cheryme.top

#define X_H
来源：http://rfh.hesvh.cn

#endif
来源：http://enf.pengpengdd.cyou

[S31] C++：Hello World
来源：http://opt.316326.xyz

#include <iostream>
来源：http://qby.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://egk.yvedp.cn

[S32] C++：字符串
来源：http://lud.sxryk.cn

std::string s = "hi";  s += "!";
来源：http://cds.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://tvk.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zly.cdnleiting.top

[S34] C++：遍历 vector
来源：http://oag.kuanghao11.cn

for (auto &x : v) { std::cout << x; }
来源：http://tip.feifeiyinyue.top

[S35] C++：map
来源：http://sbs.vqdsnc.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ppb.uphjek.com

[S36] C++：unordered_map
来源：http://nbx.quarkkingdee.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vvf.wangdashe.top

[S37] C++：set
来源：http://eqh.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://quz.hfpthk.cn

[S38] C++：排序
来源：http://gdj.hesvh.cn

std::sort(v.begin(), v.end());
来源：http://pho.kuanghao11.cn

[S39] C++：自定义比较器排序
来源：http://vca.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://awk.hammf.cn

[S40] C++：查找元素
来源：http://oft.hywenlv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vzc.hfpthk.cn

[S41] C++：类与构造函数
来源：http://zkg.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cgg.wangshuangyany.cn

[S42] C++：继承与虚函数
来源：http://ghx.cqqwz.cn

class B : public Base { public: void f() override {} };
来源：http://plv.andypj.xyz

[S43] C++：智能指针
来源：http://lyj.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://qxb.fzhhl.top

[S44] C++：引用传参
来源：http://gsf.nwbrower.top

void inc(int &x) { ++x; }
来源：http://urx.tian-w.cn

[S45] C++：lambda
来源：http://zvu.yuxming.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zql.sufxvd.cn

[S46] C++：函数模板
来源：http://smk.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jej.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://fda.svipenyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aiy.9152youxi.cn

[S48] C++：逐行读文件
来源：http://chr.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://esx.zhongyouzk.top

while (std::getline(in, line)) { }
来源：http://cdd.nwbrower.top

[S49] C++：写文件
来源：http://rqe.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mxr.guowangkeji.top

[S50] C++：格式化数字
来源：http://xhb.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pyv.smart0.xyz

[S51] C++：显式类型转换
来源：http://mnt.fktsv.cn

static_cast<double>(a) / b
来源：http://nnl.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://pdr.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://ign.yanxiufei.cn

[S53] C++：移动语义
来源：http://etq.yuxming.cn

std::vector<int> w = std::move(v);
来源：http://mbx.cucudq.cn

[S54] C++：异常处理
来源：http://zur.andypj.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ksh.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://wzs.ydzc1.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bwt.yuanzhike.top

[S56] C++：optional
来源：http://ubl.feifeiyinyue.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qav.hesvh.cn

[S57] C++：编译期常量
来源：http://esf.havefunace.top

constexpr int N = 10;
来源：http://eqa.kuanghao11.cn

[S58] C++：命名空间
来源：http://spx.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://dzb.tian-w.cn

[S59] C++：静态断言
来源：http://pcr.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xht.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://yli.daria6918.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mwt.0kj1m.cn

================================================================================
来源：http://whv.chenjidiqi.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lza.dashuyun.cn

================================================================================
来源：http://yxo.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://vrc.xuanzx.com

println("Hello")
来源：http://llq.yfazqb.com

[T02] Kotlin：变量
来源：http://oyq.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fai.zhongyouzk.top

[T03] Kotlin：字符串模板
来源：http://lbr.yj202588.top

"值: $b"
来源：http://rab.hfpthk.cn

[T04] Kotlin：空安全
来源：http://ekb.zdqjudy.top

val n: String? = null;  n?.length
来源：http://odn.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://bsd.yanxiufei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oce.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://zib.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wiv.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://glq.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ton.yangfankeji.com

[T08] Kotlin：数据类
来源：http://esv.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://jzw.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://avt.ybcxt.top

fun String.exclaim() = this + "!"
来源：http://zsg.redwolf501.top

[T10] Kotlin：默认参数
来源：http://puu.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://nsr.hfpthk.cn

[T11] Kotlin：协程
来源：http://tbu.xylfe.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rqn.mhx1999.top

[T12] Kotlin：解构声明
来源：http://ewh.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://zzk.hysaishi.cn

[T13] Kotlin：只读 Map
来源：http://psq.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://aii.hfpthk.cn

[T14] Kotlin：循环
来源：http://dag.ivvv.top

for (i in 1..10) println(i)
来源：http://dmt.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://pns.gzhubu.top

interface Shape { fun area(): Double }
来源：http://rtv.yuanzhike.top

[T16] Swift：Hello World
来源：http://mxc.nwbrower.top

print("Hello")
来源：http://gnq.zhijiandao.cn

[T17] Swift：变量与常量
来源：http://vcn.yangfankeji.com

var a = 1;  let b = 2
来源：http://rrc.tarul.cn

[T18] Swift：字符串插值
来源：http://bld.jiagoushi.top

"值: \(b)"
来源：http://jbr.nwbrower.top

[T19] Swift：可选绑定
来源：http://uea.sxryk.cn

if let n = opt { print(n) }
来源：http://wem.vqdsnc.cn

[T20] Swift：数组操作
来源：http://mhk.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pvv.redwolf501.top

[T21] Swift：遍历
来源：http://hqj.hcnkem.com

for x in a { print(x) }
来源：http://lee.meibo888.top

[T22] Swift：字典
来源：http://vjw.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://uqe.c1oappe.top

[T23] Swift：函数
来源：http://tyv.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gek.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://hpk.sxryk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rlr.zhijiandao.cn

[T25] Swift：结构体
来源：http://yhz.xuanzx.com

struct P { var x: Int }
来源：http://zrk.chenzaomai.com

[T26] Swift：类与重写
来源：http://lzc.gogol.net.cn

class A: Base { override func f() {} }
来源：http://mat.sxryk.cn

[T27] Swift：错误处理
来源：http://cxg.feifeiyinyue.top

do { try f() } catch { print(error) }
来源：http://cwa.fktsv.cn

[T28] Swift：枚举
来源：http://fup.jinqigfzy.top

enum Color { case red, green }
来源：http://ggz.cucudq.cn

[T29] Swift：guard 提前返回
来源：http://gkv.hywenlv.cn

guard let x = opt else { return }
来源：http://mal.pycfn.com

[T30] Swift：协议
来源：http://ypo.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://lpd.fktsv.cn

[T31] Lua：Hello World
来源：http://fkq.chenzaomai.com

print("Hello")
来源：http://jvw.jinqigufen.top

[T32] Lua：局部变量
来源：http://awb.jinyuanbaomall.cn

local a = 1
来源：http://nab.c1oappe.top

[T33] Lua：表（数组）
来源：http://olk.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://bqq.redwolf501.top

[T34] Lua：遍历表
来源：http://dxr.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qns.yvedp.cn

[T35] Lua：字典表
来源：http://ahl.nanxuanxn.top

local d = { a = 1 };  d.b = 2
来源：http://kds.yangfankeji.com

[T36] Lua：函数
来源：http://wal.xylfe.cn

function add(a, b) return a + b end
来源：http://njv.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://tvk.ywan-chungtsiang.top

"a" .. "b"
来源：http://nmt.andypj.xyz

[T38] Lua：条件
来源：http://hno.zhaomingkeji.xyz

if x > 0 then print("正") end
来源：http://bim.yonumen.top

[T39] Lua：模式匹配
来源：http://wgz.tianlin.xyz

string.find(s, "%d+")
来源：http://hhp.fzhhl.top

[T40] Lua：元表
来源：http://auy.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://vle.xinyue.icu

[T41] Perl：Hello World
来源：http://nbp.kuanghao11.cn

print "Hello\n";
来源：http://eve.sysykeji.top

[T42] Perl：变量类型
来源：http://euv.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xpa.fktsv.cn

[T43] Perl：字符串插值
来源：http://fvb.yuxming.cn

"值: $a"
来源：http://aot.aizwys.cn

[T44] Perl：条件
来源：http://jwx.ehwqpu.com

if ($a > 0) { print "正"; }
来源：http://ctj.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://tzw.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://vfk.sysykeji.top

[T46] Perl：哈希操作
来源：http://mce.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fpv.xziqi.cn

[T47] Perl：正则捕获
来源：http://kyk.tian-w.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xjd.jlsjyb.cn

[T48] Perl：正则替换
来源：http://rzy.bjfxy.top

$s =~ s/old/new/g;
来源：http://oyr.haohaochexian.top

[T49] Perl：函数
来源：http://dnp.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cbn.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://zen.ctjpmb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://woi.gzhubu.top

while (my $line = <$fh>) { print $line; }
来源：http://cup.jinghuilouyu.cn

[T51] Scala：Hello World
来源：http://cgi.chenjidiqi.icu

println("Hello")
来源：http://hsa.iojbl.cn

[T52] Scala：变量
来源：http://huv.yanxiufei.cn

val a = 1;  var b = 2
来源：http://bqi.fengsongda.top

[T53] Scala：字符串插值
来源：http://whu.yongpay.top

s"值: $b"
来源：http://dlc.yj202588.top

[T54] Scala：集合映射
来源：http://pxv.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://dqw.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://hof.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://yum.haohaochexian.top

[T56] Scala：样例类
来源：http://nfb.zhaomingkeji.xyz

case class User(name: String, age: Int)
来源：http://gkk.andypj.xyz

[T57] Scala：模式匹配
来源：http://olq.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://muh.zhijiandao.cn

[T58] Scala：函数定义
来源：http://zfr.xylfe.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sup.dashuyun.cn

[T59] Scala：循环
来源：http://bbl.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://elv.gogol.net.cn

[T60] Scala：折叠
来源：http://ivg.jlsjyb.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bvr.meibo888.top

================================================================================
来源：http://xix.iojbl.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uzo.chenjidiqi.icu

================================================================================
来源：http://fso.zhixingplan.top

[U01] Py：创建虚拟环境
来源：http://uol.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://fas.pycfn.com

[U02] Py：导出 / 安装依赖
来源：http://jey.cdnleiting.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://awm.tanke756.top

[U03] Py：加载 .env 配置
来源：http://yvr.9152youxi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wfl.zdbjq.cn

[U04] Py：变量调试打印
来源：http://lmg.sweek.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yyy.birdmap.top

[U05] Py：列表去重且保序
来源：http://owo.pycfn.com

list(dict.fromkeys(arr))
来源：http://ogy.guowangkeji.top

[U06] Py：合并两个字典
来源：http://cvw.yj20258.top

{**a, **b}
来源：http://sbm.hnxiangtu.top

[U07] Py：反转字典键值
来源：http://nej.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://tsb.zhiwuduotai.top

[U08] Py：展平二维列表
来源：http://zbg.jqgfzy.top

[y for x in nested for y in x]
来源：http://rkb.snrcjt.cn

[U09] Py：字典取最大值的键
来源：http://rqa.jqgufenzy.top

max(d, key=d.get)
来源：http://nuz.xuanzx.com

[U10] Py：按值排序字典
来源：http://eou.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nyv.meibo888.top

[U11] Py：生成器表达式
来源：http://eob.hammf.cn

(x * 2 for x in arr)
来源：http://uer.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xyf.yueranfly.top

Counter(arr).most_common(3)
来源：http://bdv.sxryk.cn

[U13] Py：固定长度队列
来源：http://apb.meibo888.top

deque(maxlen=10)
来源：http://iht.hongshengwenyu.top

[U14] Py：分组收集到列表
来源：http://pbo.fehbvm.com

defaultdict(list)
来源：http://iiv.gaohongyu789.top

[U15] Py：高精度计时
来源：http://ymq.sysykeji.top

t = time.perf_counter()
来源：http://ekw.jianghu66.top

[U16] Py：命令行参数解析
来源：http://nei.hywenlv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iwl.hesvh.cn

[U17] Py：初始化日志
来源：http://vam.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://jez.snrcjt.cn

[U18] Py：预编译正则
来源：http://zbu.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://czp.yj202588.top

[U19] Py：正则替换带回调
来源：http://fog.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ccy.birdmap.top

[U20] Py：缓存函数结果
来源：http://jqw.shangyingyoupin.top

@functools.lru_cache(maxsize=None)
来源：http://ots.xuanzx.com

[U21] Py：自定义上下文管理器
来源：http://dmn.daria6918.cn

@contextlib.contextmanager
来源：http://tdy.0kj1m.cn

[U22] Py：矩阵转置
来源：http://keg.sufxvd.cn

list(zip(*m))
来源：http://vpm.cashguo.top

[U23] Py：分块读取大文件
来源：http://bou.shanyushiyangtech.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xxa.shuidangran.top

[U24] Py：路径操作
来源：http://xvq.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jqf.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://wnz.yueranfly.top

csv.DictReader(f)
来源：http://eoh.fengsongda.top

[U26] Py：并发下载
来源：http://nwn.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ysz.sufxvd.cn

[U27] Py：异步 HTTP
来源：http://abq.zhengqikj.top

aiohttp.ClientSession() 配合 async with
来源：http://wep.hywenlv.cn

[U28] Py：类型别名
来源：http://hth.ybcxt.top

UserId = int
来源：http://cwt.9152youxi.cn

[U29] Py：属性校验
来源：http://vkm.epnwcf.com

@property 与 @x.setter 配合
来源：http://tsn.zhongyouzk.top

[U30] Py：数据类
来源：http://jyu.shanyushiyangtech.top

@dataclass(slots=True)
来源：http://eke.guannengcc.top

[U31] Py：单测
来源：http://sav.yfazqb.com

python -m pytest -q
来源：http://kjj.zdqjudy.top

[U32] Py：代码格式化
来源：http://wtc.xuetiantiany.cn

ruff format . && ruff check --fix .
来源：http://qdb.nwbrower.top

[U33] Py：打包发布
来源：http://gyg.andypj.xyz

python -m build  （依赖 pyproject.toml）
来源：http://ynv.ydzc1.top

[U34] Py：判断编码
来源：http://rir.wangshuangyany.cn

chardet.detect(raw)
来源：http://ihh.iojbl.cn

[U35] Py：发送邮件
来源：http://vim.iojbl.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://akr.mhx1999.top

[U36] Py：定时任务
来源：http://bxk.yongpay.top

schedule.every(10).minutes.do(job)
来源：http://bpz.shanyushiyangtech.top

[U37] Py：读写 Excel
来源：http://xds.guowangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://iup.c1oappe.top

[U38] Py：获取脚本所在目录
来源：http://sdu.hcnkem.com

Path(__file__).resolve().parent
来源：http://kki.andypj.xyz

[U39] Py：判断是否在交互环境
来源：http://ddp.shanyushiyangtech.top

sys.stdout.isatty()
来源：http://gyc.yueranfly.top

[U40] Py：打印到标准错误
来源：http://pxm.zhoulong.xyz

print("err", file=sys.stderr)
来源：http://igz.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://qde.sweek.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ovl.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://hfv.ehwqpu.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://reo.bbcook.cn

[U43] PHP：声明命名空间
来源：http://yuc.guowangkeji.top

namespace App\Http;
来源：http://dkz.gotoacloud.top

[U44] PHP：开启严格类型
来源：http://lbv.shanyushiyangtech.top

declare(strict_types=1);
来源：http://dlb.xuanzx.com

[U45] PHP：类型声明与返回类型
来源：http://uyj.hfpthk.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://drz.fehbvm.com

[U46] PHP：可空类型
来源：http://cte.jyoumei.cn

?string $name = null
来源：http://guh.sweek.top

[U47] PHP：联合类型
来源：http://bvv.bbcook.cn

int|string $id
来源：http://qgd.jqgufenzy.top

[U48] PHP：纯枚举
来源：http://nge.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gda.mhx1999.top

[U49] PHP：只读属性
来源：http://bde.havefunace.top

public readonly string $name
来源：http://vrf.ppjwa.cn

[U50] PHP：构造器属性提升
来源：http://zoz.52xcode.cn

public function __construct(private int $id) {}
来源：http://kqy.52xcode.cn


<!-- 参考信息 -->