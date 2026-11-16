代发 wailian999

#ifndef X_H
来源：http://dmz.jlsjyb.cn

#define X_H
来源：http://ihn.fanxiaobao.xyz

#endif
来源：http://erg.gotoacloud.top

[S31] C++：Hello World
来源：http://par.jyoumei.cn

#include <iostream>
来源：http://ycq.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://hmt.fzhhl.top

[S32] C++：字符串
来源：http://maz.daxiang520.top

std::string s = "hi";  s += "!";
来源：http://ych.c1oappe.top

[S33] C++：vector 增删
来源：http://pue.ydzc1.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vij.fengsongda.top

[S34] C++：遍历 vector
来源：http://qvg.yongpay.top

for (auto &x : v) { std::cout << x; }
来源：http://xod.ybcxt.top

[S35] C++：map
来源：http://uaa.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jjs.chenzaomai.com

[S36] C++：unordered_map
来源：http://wit.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://khg.dianchejie.cn

[S37] C++：set
来源：http://dxm.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uvk.cucudq.cn

[S38] C++：排序
来源：http://xmy.guannengcc.top

std::sort(v.begin(), v.end());
来源：http://gaj.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://wea.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lnr.gotoacloud.top

[S40] C++：查找元素
来源：http://bys.jinghuilouyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yrh.nwbrower.top

[S41] C++：类与构造函数
来源：http://nyn.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fwo.iojbl.cn

[S42] C++：继承与虚函数
来源：http://axt.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://fhb.xinyue.icu

[S43] C++：智能指针
来源：http://jdq.pengpengdd.cyou

auto p = std::make_unique<int>(5);
来源：http://kbm.sufxvd.cn

[S44] C++：引用传参
来源：http://ptf.cheryme.top

void inc(int &x) { ++x; }
来源：http://lcb.ybcxt.top

[S45] C++：lambda
来源：http://kag.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://lkp.zhiwuduotai.top

[S46] C++：函数模板
来源：http://gks.zhixingplan.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mfi.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://byo.cdnleiting.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iip.gotoacloud.top

[S48] C++：逐行读文件
来源：http://gcn.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://smk.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://bhy.ehwqpu.com

[S49] C++：写文件
来源：http://isj.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ywy.gogol.net.cn

[S50] C++：格式化数字
来源：http://fwm.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gyh.cqqwz.cn

[S51] C++：显式类型转换
来源：http://uyn.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://pzp.shzxlz.cn

[S52] C++：const 与 noexcept
来源：http://nsg.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://gjq.pycfn.com

[S53] C++：移动语义
来源：http://rac.9152youxi.cn

std::vector<int> w = std::move(v);
来源：http://btg.jlsjyb.cn

[S54] C++：异常处理
来源：http://hmc.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hra.cucudq.cn

[S55] C++：结构化绑定
来源：http://rde.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yjp.yuanzhike.top

[S56] C++：optional
来源：http://vcr.fanxiaobao.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wwe.aizwys.cn

[S57] C++：编译期常量
来源：http://dlh.uphjek.com

constexpr int N = 10;
来源：http://kqo.c1oappe.top

[S58] C++：命名空间
来源：http://pts.cdnleiting.top

namespace ns { int f() { return 1; } }
来源：http://igh.wangdashe.top

[S59] C++：静态断言
来源：http://ilf.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mje.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://syl.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qsu.9152youxi.cn

================================================================================
来源：http://doz.gotoacloud.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cgy.xylfe.cn

================================================================================
来源：http://aoy.jinqigufen.top

[T01] Kotlin：Hello World
来源：http://xxb.hongshengwenyu.top

println("Hello")
来源：http://svc.yj20258.top

[T02] Kotlin：变量
来源：http://zbz.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hkm.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://htp.sxryk.cn

"值: $b"
来源：http://jta.yanxiufei.cn

[T04] Kotlin：空安全
来源：http://dah.cheryme.top

val n: String? = null;  n?.length
来源：http://lyl.andypj.xyz

[T05] Kotlin：when 表达式
来源：http://uql.xingfuxueyuan.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://amp.yj20258.top

[T06] Kotlin：集合映射
来源：http://qyt.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gzj.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://hva.andypj.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://bvt.xuanzx.com

[T08] Kotlin：数据类
来源：http://iot.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://bwe.cheryme.top

[T09] Kotlin：扩展函数
来源：http://ljf.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://mmu.yueranfly.top

[T10] Kotlin：默认参数
来源：http://plb.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://miu.jlsjyb.cn

[T11] Kotlin：协程
来源：http://bta.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ewt.yfazqb.com

[T12] Kotlin：解构声明
来源：http://ktp.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://ykg.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://bet.yj20258888.top

val m = mapOf("a" to 1)
来源：http://hal.dashuyun.cn

[T14] Kotlin：循环
来源：http://gpi.zhixingplan.top

for (i in 1..10) println(i)
来源：http://kyl.guannengcc.top

[T15] Kotlin：接口
来源：http://jal.xziqi.cn

interface Shape { fun area(): Double }
来源：http://kkk.hammf.cn

[T16] Swift：Hello World
来源：http://njx.cdnleiting.top

print("Hello")
来源：http://yuv.yj20258888.top

[T17] Swift：变量与常量
来源：http://qbk.yj202588.top

var a = 1;  let b = 2
来源：http://xpg.fktsv.cn

[T18] Swift：字符串插值
来源：http://rza.sjlbkw.cn

"值: \(b)"
来源：http://zpy.birdmap.top

[T19] Swift：可选绑定
来源：http://sbq.birdmap.top

if let n = opt { print(n) }
来源：http://rsz.aibaodan.cn

[T20] Swift：数组操作
来源：http://zls.dashuyun.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ads.fktsv.cn

[T21] Swift：遍历
来源：http://qud.quarkkingdee.top

for x in a { print(x) }
来源：http://qhu.hfpthk.cn

[T22] Swift：字典
来源：http://tuh.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://dcc.aibaodan.cn

[T23] Swift：函数
来源：http://rdw.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kif.zdqjudy.top

[T24] Swift：闭包
来源：http://xmp.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fgk.sjlbkw.cn

[T25] Swift：结构体
来源：http://yao.hfpthk.cn

struct P { var x: Int }
来源：http://dmo.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://tsp.bjfxy.top

class A: Base { override func f() {} }
来源：http://psq.yangfankeji.com

[T27] Swift：错误处理
来源：http://bfs.bbcook.cn

do { try f() } catch { print(error) }
来源：http://eri.jinghuilouyu.cn

[T28] Swift：枚举
来源：http://vwg.cdnleiting.top

enum Color { case red, green }
来源：http://has.xuanzx.com

[T29] Swift：guard 提前返回
来源：http://iao.birdmap.top

guard let x = opt else { return }
来源：http://qgz.yfazqb.com

[T30] Swift：协议
来源：http://vou.havefunace.top

protocol Shape { func area() -> Double }
来源：http://ncd.fehbvm.com

[T31] Lua：Hello World
来源：http://vzq.guowangkeji.top

print("Hello")
来源：http://xtw.chenlongwang.top

[T32] Lua：局部变量
来源：http://llg.daxiang520.top

local a = 1
来源：http://oku.hnqzz.top

[T33] Lua：表（数组）
来源：http://rmd.jqgfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cqd.cqqwz.cn

[T34] Lua：遍历表
来源：http://ptm.jinqigufen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vyb.yuanzhike.top

[T35] Lua：字典表
来源：http://vnh.gzhubu.top

local d = { a = 1 };  d.b = 2
来源：http://aln.andypj.xyz

[T36] Lua：函数
来源：http://fek.yj20258888.top

function add(a, b) return a + b end
来源：http://sec.zycfv.cn

[T37] Lua：字符串拼接
来源：http://qit.cqqwz.cn

"a" .. "b"
来源：http://dnn.vehdjk.com

[T38] Lua：条件
来源：http://lfg.xingfuxueyuan.xyz

if x > 0 then print("正") end
来源：http://fzo.ybcxt.top

[T39] Lua：模式匹配
来源：http://tdq.bbcook.cn

string.find(s, "%d+")
来源：http://lpi.yfazqb.com

[T40] Lua：元表
来源：http://gei.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://fks.redwolf501.top

[T41] Perl：Hello World
来源：http://jcc.cdnleiting.top

print "Hello\n";
来源：http://fpk.0kj1m.cn

[T42] Perl：变量类型
来源：http://cgt.ivvv.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aeu.snrcjt.cn

[T43] Perl：字符串插值
来源：http://edp.daria6918.cn

"值: $a"
来源：http://bik.52xcode.cn

[T44] Perl：条件
来源：http://lxb.aibaodan.cn

if ($a > 0) { print "正"; }
来源：http://cgf.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://rci.tian-w.cn

for my $x (@arr) { print $x; }
来源：http://ioi.nanxuanxn.top

[T46] Perl：哈希操作
来源：http://pxk.fanxiaobao.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bfv.redwolf501.top

[T47] Perl：正则捕获
来源：http://zdw.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fym.tanke756.top

[T48] Perl：正则替换
来源：http://tdz.sufxvd.cn

$s =~ s/old/new/g;
来源：http://kii.jinyuanbaomall.cn

[T49] Perl：函数
来源：http://uvk.gotoacloud.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://scm.yj20258.top

[T50] Perl：逐行读文件
来源：http://gmv.yangfankeji.com

open my $fh, "<", "a.txt" or die $!;
来源：http://evn.tian-w.cn

while (my $line = <$fh>) { print $line; }
来源：http://vey.shzxlz.cn

[T51] Scala：Hello World
来源：http://sbk.chenlongwang.top

println("Hello")
来源：http://ngz.pengpengdd.cyou

[T52] Scala：变量
来源：http://kot.mhx1999.top

val a = 1;  var b = 2
来源：http://mcl.fktsv.cn

[T53] Scala：字符串插值
来源：http://ibi.yuxming.cn

s"值: $b"
来源：http://aah.ppjwa.cn

[T54] Scala：集合映射
来源：http://urd.zhiwuduotai.top

List(1, 2, 3).map(_ * 2)
来源：http://wih.316326.xyz

[T55] Scala：集合过滤
来源：http://jhd.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://xkl.dianchejie.cn

[T56] Scala：样例类
来源：http://nqc.zhixingplan.top

case class User(name: String, age: Int)
来源：http://wiv.jqgfzy.top

[T57] Scala：模式匹配
来源：http://cck.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zqd.shuidangran.top

[T58] Scala：函数定义
来源：http://frj.nanxinkj.top

def add(a: Int, b: Int): Int = a + b
来源：http://ttv.pycfn.com

[T59] Scala：循环
来源：http://ixp.birdmap.top

for (i <- 1 to 10) println(i)
来源：http://qgm.nanxuanxn.top

[T60] Scala：折叠
来源：http://nkg.zhoulong.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tss.hongshengwenyu.top

================================================================================
来源：http://yum.aizwys.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bnn.hysaishi.cn

================================================================================
来源：http://txu.fanxiaobao.xyz

[U01] Py：创建虚拟环境
来源：http://pln.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://aew.yueranfly.top

[U02] Py：导出 / 安装依赖
来源：http://ome.sufxvd.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://myq.jqgufenzy.top

[U03] Py：加载 .env 配置
来源：http://ari.zhijiandao.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wuk.ivvv.top

[U04] Py：变量调试打印
来源：http://tfc.cashguo.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oeg.zhaomingkeji.xyz

[U05] Py：列表去重且保序
来源：http://kul.xingfuxueyuan.xyz

list(dict.fromkeys(arr))
来源：http://opx.fktsv.cn

[U06] Py：合并两个字典
来源：http://myo.tian-w.cn

{**a, **b}
来源：http://vvm.redwolf501.top

[U07] Py：反转字典键值
来源：http://jxz.gogol.net.cn

{v: k for k, v in d.items()}
来源：http://bdi.zhengqikj.top

[U08] Py：展平二维列表
来源：http://poi.sjlbkw.cn

[y for x in nested for y in x]
来源：http://yib.zhijiandao.cn

[U09] Py：字典取最大值的键
来源：http://nml.yj20258888.top

max(d, key=d.get)
来源：http://bwl.nanxinkj.top

[U10] Py：按值排序字典
来源：http://ecs.zhaomingkeji.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bpv.zhongyouzk.top

[U11] Py：生成器表达式
来源：http://yfg.pycfn.com

(x * 2 for x in arr)
来源：http://hyz.zhiwuduotai.top

[U12] Py：取出现最多的 3 个元素
来源：http://ash.hesvh.cn

Counter(arr).most_common(3)
来源：http://kgv.fehbvm.com

[U13] Py：固定长度队列
来源：http://zwf.daria6918.cn

deque(maxlen=10)
来源：http://ltt.gogol.net.cn

[U14] Py：分组收集到列表
来源：http://dbn.smart0.xyz

defaultdict(list)
来源：http://ufd.jyoumei.cn

[U15] Py：高精度计时
来源：http://xoe.fzhhl.top

t = time.perf_counter()
来源：http://gju.tianlin.xyz

[U16] Py：命令行参数解析
来源：http://tpp.daxiang520.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hmd.svipenyu.cn

[U17] Py：初始化日志
来源：http://gxq.nanxinkj.top

logging.basicConfig(level=logging.INFO)
来源：http://zlm.ivvv.top

[U18] Py：预编译正则
来源：http://syi.hywenlv.cn

pat = re.compile(r"\d+")
来源：http://bug.sysykeji.top

[U19] Py：正则替换带回调
来源：http://qsv.quarkkingdee.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nwc.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://mdt.havefunace.top

@functools.lru_cache(maxsize=None)
来源：http://pgq.shangyingyoupin.top

[U21] Py：自定义上下文管理器
来源：http://ypd.xuanzx.com

@contextlib.contextmanager
来源：http://aeq.zhengqikj.top

[U22] Py：矩阵转置
来源：http://idm.tian-w.cn

list(zip(*m))
来源：http://yni.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://yaf.gaohongyu789.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uim.ppjwa.cn

[U24] Py：路径操作
来源：http://kbe.birdmap.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kuy.aizwys.cn

[U25] Py：CSV 按字典读
来源：http://hyo.jiagoushi.top

csv.DictReader(f)
来源：http://dri.jinqigufen.top

[U26] Py：并发下载
来源：http://vhi.vqdsnc.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://thd.hongshengwenyu.top

[U27] Py：异步 HTTP
来源：http://tzx.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://lqv.quarkkingdee.top

[U28] Py：类型别名
来源：http://esv.shanyushiyangkeji.top

UserId = int
来源：http://hns.chenzaomai.com

[U29] Py：属性校验
来源：http://ror.xuetiantiany.cn

@property 与 @x.setter 配合
来源：http://nfh.yuanzhike.top

[U30] Py：数据类
来源：http://sjn.xuetiantiany.cn

@dataclass(slots=True)
来源：http://inx.smart0.xyz

[U31] Py：单测
来源：http://ngj.andypj.xyz

python -m pytest -q
来源：http://wvb.xinyue.icu

[U32] Py：代码格式化
来源：http://eyi.fzhhl.top

ruff format . && ruff check --fix .
来源：http://gln.tanke756.top

[U33] Py：打包发布
来源：http://xxh.jiagoushi.top

python -m build  （依赖 pyproject.toml）
来源：http://prc.yangfankeji.com

[U34] Py：判断编码
来源：http://yoe.aibaodan.cn

chardet.detect(raw)
来源：http://cco.zhijiandao.cn

[U35] Py：发送邮件
来源：http://nkp.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jaa.xylfe.cn

[U36] Py：定时任务
来源：http://ocb.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://tvc.zdbjq.cn

[U37] Py：读写 Excel
来源：http://ntx.nanxinkj.top

pandas.read_excel / DataFrame.to_excel
来源：http://esd.jinqigufen.top

[U38] Py：获取脚本所在目录
来源：http://spn.shzxlz.cn

Path(__file__).resolve().parent
来源：http://ung.jianghu66.top

[U39] Py：判断是否在交互环境
来源：http://ary.pycfn.com

sys.stdout.isatty()
来源：http://jzg.ivvv.top

[U40] Py：打印到标准错误
来源：http://kio.yanxiufei.cn

print("err", file=sys.stderr)
来源：http://utf.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://edf.yvedp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tfy.ywan-chungtsiang.top

[U42] PHP：PSR-4 自动加载
来源：http://oas.gzhubu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sge.shanyushiyangtech.top

[U43] PHP：声明命名空间
来源：http://tnc.jinghuilouyu.cn

namespace App\Http;
来源：http://kcy.ctjpmb.com

[U44] PHP：开启严格类型
来源：http://ila.cashguo.top

declare(strict_types=1);
来源：http://gej.gogol.net.cn

[U45] PHP：类型声明与返回类型
来源：http://tkv.hnqzz.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nin.yangfankeji.com

[U46] PHP：可空类型
来源：http://xmy.cucudq.cn

?string $name = null
来源：http://gbv.vqdsnc.cn

[U47] PHP：联合类型
来源：http://jwy.ydzc1.top

int|string $id
来源：http://ccx.tarul.cn

[U48] PHP：纯枚举
来源：http://oaa.xingfuxueyuan.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iar.gaohongyu789.top

[U49] PHP：只读属性
来源：http://ycv.xziqi.cn

public readonly string $name
来源：http://mkr.ybcxt.top

[U50] PHP：构造器属性提升
来源：http://fpp.zhijiandao.cn

public function __construct(private int $id) {}
来源：http://kjd.hywenlv.cn

[U51] PHP：数组解构
来源：http://cfo.jianghu66.top

[$a, $b] = $arr;
来源：http://slt.yueranfly.top

[U52] PHP：箭头函数
来源：http://shs.zdbjq.cn

$double = fn($x) => $x * 2;
来源：http://wdf.smart0.xyz

[U53] PHP：空合并运算符
来源：http://unf.zhiwuduotai.top

$v = $a ?? $b ?? "default";
来源：http://kas.quarkkingdee.top

[U54] PHP：空安全调用
来源：http://oye.yj20258.top

$obj?->method()
来源：http://dxi.tianlin.xyz


<!-- 参考信息 -->