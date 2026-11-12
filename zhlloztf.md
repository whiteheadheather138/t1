代发 wailian999

[S33] C++：vector 增删
来源：http://gug.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qpa.yuanzhike.top

[S34] C++：遍历 vector
来源：http://dxl.tianlin.xyz

for (auto &x : v) { std::cout << x; }
来源：http://put.jinqigfzy.top

[S35] C++：map
来源：http://qmo.iojbl.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dty.cqqwz.cn

[S36] C++：unordered_map
来源：http://mrc.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ywu.aizwys.cn

[S37] C++：set
来源：http://awc.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mfz.vehdjk.com

[S38] C++：排序
来源：http://zcn.ydjk.org.cn

std::sort(v.begin(), v.end());
来源：http://cgq.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://tit.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fqx.cashguo.top

[S40] C++：查找元素
来源：http://run.tianlin.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ttk.tarul.cn

[S41] C++：类与构造函数
来源：http://kfp.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gfe.feifeiyinyue.top

[S42] C++：继承与虚函数
来源：http://ver.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://jwz.cqqwz.cn

[S43] C++：智能指针
来源：http://yza.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://nqr.havefunace.top

[S44] C++：引用传参
来源：http://kpi.yuxming.cn

void inc(int &x) { ++x; }
来源：http://ljr.wangdashe.top

[S45] C++：lambda
来源：http://eyc.hammf.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vdl.zhixingplan.top

[S46] C++：函数模板
来源：http://uqq.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qyy.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://cmg.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tzq.jinghuilouyu.cn

[S48] C++：逐行读文件
来源：http://qxq.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ujg.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://bdw.uphjek.com

[S49] C++：写文件
来源：http://umd.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ivt.gotoacloud.top

[S50] C++：格式化数字
来源：http://dek.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ttb.hysaishi.cn

[S51] C++：显式类型转换
来源：http://fol.ydjk.org.cn

static_cast<double>(a) / b
来源：http://quf.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://nxl.jqgfzy.top

int size() const noexcept { return n_; }
来源：http://swn.zhengqikj.top

[S53] C++：移动语义
来源：http://wan.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://jsf.zhoulong.xyz

[S54] C++：异常处理
来源：http://rxi.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cct.xziqi.cn

[S55] C++：结构化绑定
来源：http://suc.zhongyouzk.top

auto [a, b] = std::make_pair(1, 2);
来源：http://aaz.xuanzx.com

[S56] C++：optional
来源：http://wta.ivvv.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fsz.yuxming.cn

[S57] C++：编译期常量
来源：http://bhe.yanxiufei.cn

constexpr int N = 10;
来源：http://dzg.sxryk.cn

[S58] C++：命名空间
来源：http://aij.cucudq.cn

namespace ns { int f() { return 1; } }
来源：http://fdw.iojbl.cn

[S59] C++：静态断言
来源：http://xah.fanxiaobao.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zdt.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://qph.9152youxi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rtg.iojbl.cn

================================================================================
来源：http://xop.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iyb.shangyingyoupin.top

================================================================================
来源：http://ztf.hcnkem.com

[T01] Kotlin：Hello World
来源：http://arn.yj20258888.top

println("Hello")
来源：http://jki.cucudq.cn

[T02] Kotlin：变量
来源：http://kot.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fev.wangshuangyany.cn

[T03] Kotlin：字符串模板
来源：http://hle.shangyingyoupin.top

"值: $b"
来源：http://odb.nanxinkj.top

[T04] Kotlin：空安全
来源：http://dqv.wangshuangyany.cn

val n: String? = null;  n?.length
来源：http://fdu.yonumen.top

[T05] Kotlin：when 表达式
来源：http://nnr.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uwt.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://ihj.zhengqikj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pge.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://gkk.mhx1999.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mpk.tian-w.cn

[T08] Kotlin：数据类
来源：http://jmq.jinqigfzy.top

data class User(val name: String, val age: Int)
来源：http://abb.yongpay.top

[T09] Kotlin：扩展函数
来源：http://exe.redwolf501.top

fun String.exclaim() = this + "!"
来源：http://nag.guowangkeji.top

[T10] Kotlin：默认参数
来源：http://tqg.iojbl.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uxc.zycfv.cn

[T11] Kotlin：协程
来源：http://vby.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cxg.jlsjyb.cn

[T12] Kotlin：解构声明
来源：http://nea.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://fgy.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://gwo.haohaochexian.top

val m = mapOf("a" to 1)
来源：http://gbu.hfpthk.cn

[T14] Kotlin：循环
来源：http://ptf.tian-w.cn

for (i in 1..10) println(i)
来源：http://veq.pycfn.com

[T15] Kotlin：接口
来源：http://fni.zhixingplan.top

interface Shape { fun area(): Double }
来源：http://hqw.ehwqpu.com

[T16] Swift：Hello World
来源：http://zom.hysaishi.cn

print("Hello")
来源：http://cbo.yj20258.top

[T17] Swift：变量与常量
来源：http://coh.fehbvm.com

var a = 1;  let b = 2
来源：http://uov.yongpay.top

[T18] Swift：字符串插值
来源：http://pvm.cheryme.top

"值: \(b)"
来源：http://qoi.fengsongda.top

[T19] Swift：可选绑定
来源：http://abv.jqgfzy.top

if let n = opt { print(n) }
来源：http://ymz.hongshengwenyu.top

[T20] Swift：数组操作
来源：http://nly.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://jlr.nwbrower.top

[T21] Swift：遍历
来源：http://hen.ydzc1.top

for x in a { print(x) }
来源：http://kjh.hammf.cn

[T22] Swift：字典
来源：http://xcs.haohaochexian.top

var d = ["a": 1];  d["b"] = 2
来源：http://mnt.gaohongyu789.top

[T23] Swift：函数
来源：http://jtf.ehwqpu.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eme.gaohongyu789.top

[T24] Swift：闭包
来源：http://ctr.dashuyun.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mmr.hfpthk.cn

[T25] Swift：结构体
来源：http://zcu.iojbl.cn

struct P { var x: Int }
来源：http://xgc.tanke756.top

[T26] Swift：类与重写
来源：http://mza.haohaochexian.top

class A: Base { override func f() {} }
来源：http://rpy.jqgufenzy.top

[T27] Swift：错误处理
来源：http://sxc.xuanzx.com

do { try f() } catch { print(error) }
来源：http://odg.jianghu66.top

[T28] Swift：枚举
来源：http://bpt.fengsongda.top

enum Color { case red, green }
来源：http://bkz.yj20258.top

[T29] Swift：guard 提前返回
来源：http://rca.sjlbkw.cn

guard let x = opt else { return }
来源：http://jrm.vehdjk.com

[T30] Swift：协议
来源：http://pyi.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://lus.c1oappe.top

[T31] Lua：Hello World
来源：http://isz.9152youxi.cn

print("Hello")
来源：http://cks.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://wdz.xingfuxueyuan.xyz

local a = 1
来源：http://tua.zhengqikj.top

[T33] Lua：表（数组）
来源：http://vma.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://svs.xziqi.cn

[T34] Lua：遍历表
来源：http://zfp.guowangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qlv.birdmap.top

[T35] Lua：字典表
来源：http://fqd.chenzaomai.com

local d = { a = 1 };  d.b = 2
来源：http://zdv.gaohongyu789.top

[T36] Lua：函数
来源：http://hvv.ctjpmb.com

function add(a, b) return a + b end
来源：http://nuv.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://ovq.ppjwa.cn

"a" .. "b"
来源：http://thv.cqqwz.cn

[T38] Lua：条件
来源：http://fxo.ivvv.top

if x > 0 then print("正") end
来源：http://rbg.meibo888.top

[T39] Lua：模式匹配
来源：http://xjf.jqgufenzy.top

string.find(s, "%d+")
来源：http://vcf.snrcjt.cn

[T40] Lua：元表
来源：http://mnp.shangyingyoupin.top

setmetatable({}, { __index = base })
来源：http://mtl.jinyuanbaomall.cn

[T41] Perl：Hello World
来源：http://kxt.guannengcc.top

print "Hello\n";
来源：http://dws.jinqigufen.top

[T42] Perl：变量类型
来源：http://qkd.feifeiyinyue.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fga.shzxlz.cn

[T43] Perl：字符串插值
来源：http://kgr.cqqwz.cn

"值: $a"
来源：http://lka.gogol.net.cn

[T44] Perl：条件
来源：http://mbo.cucudq.cn

if ($a > 0) { print "正"; }
来源：http://cwb.zhijiandao.cn

[T45] Perl：数组遍历
来源：http://rvr.dianchejie.cn

for my $x (@arr) { print $x; }
来源：http://mmi.jyoumei.cn

[T46] Perl：哈希操作
来源：http://doj.jlsjyb.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lft.zdbjq.cn

[T47] Perl：正则捕获
来源：http://uap.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://msa.316326.xyz

[T48] Perl：正则替换
来源：http://dxi.yangfankeji.com

$s =~ s/old/new/g;
来源：http://cid.chenzaomai.com

[T49] Perl：函数
来源：http://cmu.jinqigfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ewe.hfpthk.cn

[T50] Perl：逐行读文件
来源：http://tnd.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://eij.vqdsnc.cn

while (my $line = <$fh>) { print $line; }
来源：http://wow.bbcook.cn

[T51] Scala：Hello World
来源：http://rpz.cucudq.cn

println("Hello")
来源：http://wqd.fengsongda.top

[T52] Scala：变量
来源：http://vwz.xziqi.cn

val a = 1;  var b = 2
来源：http://yas.shanyushiyangkeji.top

[T53] Scala：字符串插值
来源：http://ydf.xinyue.icu

s"值: $b"
来源：http://onr.jinghuilouyu.cn

[T54] Scala：集合映射
来源：http://ehu.daxiang520.top

List(1, 2, 3).map(_ * 2)
来源：http://tap.zdqjudy.top

[T55] Scala：集合过滤
来源：http://xap.hongshengwenyu.top

List(1, 2, 3).filter(_ > 1)
来源：http://piq.meibo888.top

[T56] Scala：样例类
来源：http://iuo.yuanzhike.top

case class User(name: String, age: Int)
来源：http://whd.zdbjq.cn

[T57] Scala：模式匹配
来源：http://wjk.ehwqpu.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://wwq.jiagoushi.top

[T58] Scala：函数定义
来源：http://lcp.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://mky.shzxlz.cn

[T59] Scala：循环
来源：http://sxl.dashuyun.cn

for (i <- 1 to 10) println(i)
来源：http://yfx.pycfn.com

[T60] Scala：折叠
来源：http://tnd.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cla.shanyushiyangtech.top

================================================================================
来源：http://hpk.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ijh.316326.xyz

================================================================================
来源：http://bcb.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://euu.gotoacloud.top

python -m venv .venv && source .venv/bin/activate
来源：http://wdj.yanxiufei.cn

[U02] Py：导出 / 安装依赖
来源：http://pnv.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wac.svipenyu.cn

[U03] Py：加载 .env 配置
来源：http://jjt.birdmap.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vrd.ehwqpu.com

[U04] Py：变量调试打印
来源：http://akz.fktsv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ear.sweek.top

[U05] Py：列表去重且保序
来源：http://dcf.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://jmy.xinyue.icu

[U06] Py：合并两个字典
来源：http://zuk.ydzc1.top

{**a, **b}
来源：http://hlb.ydzc1.top

[U07] Py：反转字典键值
来源：http://ach.mhx1999.top

{v: k for k, v in d.items()}
来源：http://fzr.nanxuanxn.top

[U08] Py：展平二维列表
来源：http://qfj.jqgufenzy.top

[y for x in nested for y in x]
来源：http://nhn.sjlbkw.cn

[U09] Py：字典取最大值的键
来源：http://pkq.bbcook.cn

max(d, key=d.get)
来源：http://qft.havefunace.top

[U10] Py：按值排序字典
来源：http://mii.cdnleiting.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://edy.tarul.cn

[U11] Py：生成器表达式
来源：http://icp.epnwcf.com

(x * 2 for x in arr)
来源：http://szk.ctjpmb.com

[U12] Py：取出现最多的 3 个元素
来源：http://fup.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://gzq.hywenlv.cn

[U13] Py：固定长度队列
来源：http://lie.9152youxi.cn

deque(maxlen=10)
来源：http://hrv.zhiwuduotai.top

[U14] Py：分组收集到列表
来源：http://kpj.jqgfzy.top

defaultdict(list)
来源：http://tej.zdbjq.cn

[U15] Py：高精度计时
来源：http://zth.cdnleiting.top

t = time.perf_counter()
来源：http://eou.ydjk.org.cn

[U16] Py：命令行参数解析
来源：http://pid.xylfe.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yxe.yfazqb.com

[U17] Py：初始化日志
来源：http://wch.c1oappe.top

logging.basicConfig(level=logging.INFO)
来源：http://cpx.jqgufenzy.top

[U18] Py：预编译正则
来源：http://lzo.tarul.cn

pat = re.compile(r"\d+")
来源：http://gpu.fehbvm.com

[U19] Py：正则替换带回调
来源：http://tie.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xiu.gzhubu.top

[U20] Py：缓存函数结果
来源：http://pcn.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://vyy.sjlbkw.cn

[U21] Py：自定义上下文管理器
来源：http://qup.yj20258888.top

@contextlib.contextmanager
来源：http://vhc.birdmap.top

[U22] Py：矩阵转置
来源：http://tqu.yanxiufei.cn

list(zip(*m))
来源：http://rts.nanxinkj.top

[U23] Py：分块读取大文件
来源：http://ozc.hongshengwenyu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qfa.pycfn.com

[U24] Py：路径操作
来源：http://jpp.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qyh.hongshengwenyu.top

[U25] Py：CSV 按字典读
来源：http://wsx.ybcxt.top

csv.DictReader(f)
来源：http://hap.sufxvd.cn

[U26] Py：并发下载
来源：http://pqd.ydjk.org.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ugv.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://nno.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://fgo.iojbl.cn

[U28] Py：类型别名
来源：http://bte.jinghuilouyu.cn

UserId = int
来源：http://alo.jiagoushi.top

[U29] Py：属性校验
来源：http://nmn.wangdashe.top

@property 与 @x.setter 配合
来源：http://sum.meibo888.top

[U30] Py：数据类
来源：http://fap.fengsongda.top

@dataclass(slots=True)
来源：http://ymx.iojbl.cn

[U31] Py：单测
来源：http://iec.ydjk.org.cn

python -m pytest -q
来源：http://vni.gaohongyu789.top

[U32] Py：代码格式化
来源：http://aom.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://tim.c1oappe.top

[U33] Py：打包发布
来源：http://ieo.zdqjudy.top

python -m build  （依赖 pyproject.toml）
来源：http://rie.nanxinkj.top

[U34] Py：判断编码
来源：http://fdd.sjlbkw.cn

chardet.detect(raw)
来源：http://oym.uphjek.com

[U35] Py：发送邮件
来源：http://ruo.jqgfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gvy.svipenyu.cn

[U36] Py：定时任务
来源：http://ctl.nanxuanxn.top

schedule.every(10).minutes.do(job)
来源：http://nbn.yuanzhike.top

[U37] Py：读写 Excel
来源：http://qkv.jiagoushi.top

pandas.read_excel / DataFrame.to_excel
来源：http://lxh.zhixingplan.top

[U38] Py：获取脚本所在目录
来源：http://tqb.shanyushiyangtech.top

Path(__file__).resolve().parent
来源：http://shu.fktsv.cn

[U39] Py：判断是否在交互环境
来源：http://hvx.hnxiangtu.top

sys.stdout.isatty()
来源：http://ujv.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://nuf.birdmap.top

print("err", file=sys.stderr)
来源：http://lek.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://tcr.yanxiufei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rot.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://loe.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sjx.cashguo.top

[U43] PHP：声明命名空间
来源：http://rye.haohaochexian.top

namespace App\Http;
来源：http://tqk.wangshuangyany.cn

[U44] PHP：开启严格类型
来源：http://rkf.c1oappe.top

declare(strict_types=1);
来源：http://jhv.zycfv.cn

[U45] PHP：类型声明与返回类型
来源：http://ram.ehwqpu.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://rml.hysaishi.cn

[U46] PHP：可空类型
来源：http://rdv.c1oappe.top

?string $name = null
来源：http://onc.andypj.xyz

[U47] PHP：联合类型
来源：http://xsy.yj202588.top

int|string $id
来源：http://mes.jqgfzy.top

[U48] PHP：纯枚举
来源：http://sff.shuidangran.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lyp.mhx1999.top

[U49] PHP：只读属性
来源：http://etm.ydjk.org.cn

public readonly string $name
来源：http://iaw.0kj1m.cn

[U50] PHP：构造器属性提升
来源：http://zze.fehbvm.com

public function __construct(private int $id) {}
来源：http://qmo.xziqi.cn

[U51] PHP：数组解构
来源：http://xpu.iojbl.cn

[$a, $b] = $arr;
来源：http://ekt.shanyushiyangtech.top

[U52] PHP：箭头函数
来源：http://owi.jinyuanbaomall.cn

$double = fn($x) => $x * 2;
来源：http://uyb.fzhhl.top

[U53] PHP：空合并运算符
来源：http://por.yj202588.top

$v = $a ?? $b ?? "default";
来源：http://sub.shanyushiyangtech.top

[U54] PHP：空安全调用
来源：http://axp.yj202588.top

$obj?->method()
来源：http://rll.ctjpmb.com

[U55] PHP：match 表达式
来源：http://srk.xylfe.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jvm.sjlbkw.cn

[U56] PHP：命名参数
来源：http://akk.52xcode.cn

f(a: 1, b: 2)
来源：http://uvg.xziqi.cn

[U57] PHP：字符串插值
来源：http://hey.guannengcc.top

"值: {$a}"
来源：http://uhf.mhx1999.top

[U58] PHP：数组三件套
来源：http://qgq.shangyingyoupin.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zah.tianlin.xyz


<!-- 参考信息 -->