代发 wailian999

[S33] C++：vector 增删
来源：http://auo.zycfv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qia.jinqigufen.top

[S34] C++：遍历 vector
来源：http://vno.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://xlx.jqgufenzy.top

[S35] C++：map
来源：http://qbx.0kj1m.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://koo.chenlongwang.top

[S36] C++：unordered_map
来源：http://qlt.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tax.quarkkingdee.top

[S37] C++：set
来源：http://iic.daria6918.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wyi.quarkkingdee.top

[S38] C++：排序
来源：http://uez.svipenyu.cn

std::sort(v.begin(), v.end());
来源：http://dpm.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://zfs.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kkj.yongpay.top

[S40] C++：查找元素
来源：http://nhv.nanxinkj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vrg.hnqzz.top

[S41] C++：类与构造函数
来源：http://cds.fktsv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dkr.c1oappe.top

[S42] C++：继承与虚函数
来源：http://cfi.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://smu.vehdjk.com

[S43] C++：智能指针
来源：http://sjp.chenlongwang.top

auto p = std::make_unique<int>(5);
来源：http://oaj.sxryk.cn

[S44] C++：引用传参
来源：http://giv.hnxiangtu.top

void inc(int &x) { ++x; }
来源：http://vrk.cdnleiting.top

[S45] C++：lambda
来源：http://ylt.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mcg.birdmap.top

[S46] C++：函数模板
来源：http://vhu.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gzr.pengpengdd.cyou

[S47] C++：结构化绑定遍历
来源：http://buc.kuanghao11.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dcs.cucudq.cn

[S48] C++：逐行读文件
来源：http://xlj.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://dhy.fehbvm.com

while (std::getline(in, line)) { }
来源：http://nyv.mhx1999.top

[S49] C++：写文件
来源：http://vzp.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qxy.fengsongda.top

[S50] C++：格式化数字
来源：http://dfv.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iod.pengpengdd.cyou

[S51] C++：显式类型转换
来源：http://fed.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://sxl.vqdsnc.cn

[S52] C++：const 与 noexcept
来源：http://gbs.yuxming.cn

int size() const noexcept { return n_; }
来源：http://xqw.dianchejie.cn

[S53] C++：移动语义
来源：http://fda.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://gor.sweek.top

[S54] C++：异常处理
来源：http://vji.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ubk.dianchejie.cn

[S55] C++：结构化绑定
来源：http://rtq.smart0.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://ycr.haohaochexian.top

[S56] C++：optional
来源：http://cuj.gotoacloud.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yfb.yueranfly.top

[S57] C++：编译期常量
来源：http://lct.redwolf501.top

constexpr int N = 10;
来源：http://mrv.yuxming.cn

[S58] C++：命名空间
来源：http://grv.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://nsb.nanxuanxn.top

[S59] C++：静态断言
来源：http://nkh.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kfi.cdnleiting.top

[S60] C++：遍历并删除元素
来源：http://nkv.ctjpmb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pwg.svipenyu.cn

================================================================================
来源：http://alr.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://haz.jinqigufen.top

================================================================================
来源：http://gtb.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://mpe.chenzaomai.com

println("Hello")
来源：http://dgw.fengsongda.top

[T02] Kotlin：变量
来源：http://lzz.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kzk.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://kyo.cdnleiting.top

"值: $b"
来源：http://cfz.shanyushiyangtech.top

[T04] Kotlin：空安全
来源：http://mtt.sysykeji.top

val n: String? = null;  n?.length
来源：http://huv.yj20258.top

[T05] Kotlin：when 表达式
来源：http://jxj.cdnleiting.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ywd.52xcode.cn

[T06] Kotlin：集合映射
来源：http://rnp.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://aij.vehdjk.com

[T07] Kotlin：集合过滤
来源：http://hgd.svipenyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uyv.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://zdy.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://bvf.uphjek.com

[T09] Kotlin：扩展函数
来源：http://snb.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://riz.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://azr.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kkf.fehbvm.com

[T11] Kotlin：协程
来源：http://jgj.316326.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://avp.fzhhl.top

[T12] Kotlin：解构声明
来源：http://hao.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://dhr.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://stv.0kj1m.cn

val m = mapOf("a" to 1)
来源：http://aiy.shzxlz.cn

[T14] Kotlin：循环
来源：http://acw.hysaishi.cn

for (i in 1..10) println(i)
来源：http://vgp.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://qpm.tianlin.xyz

interface Shape { fun area(): Double }
来源：http://wjw.zhengqikj.top

[T16] Swift：Hello World
来源：http://ufl.snrcjt.cn

print("Hello")
来源：http://izz.ppjwa.cn

[T17] Swift：变量与常量
来源：http://ecw.svipenyu.cn

var a = 1;  let b = 2
来源：http://asg.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://sly.redwolf501.top

"值: \(b)"
来源：http://ywd.chenlongwang.top

[T19] Swift：可选绑定
来源：http://oyd.mhx1999.top

if let n = opt { print(n) }
来源：http://uyc.zhixingplan.top

[T20] Swift：数组操作
来源：http://mvp.snrcjt.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rue.jinqigufen.top

[T21] Swift：遍历
来源：http://xad.yonumen.top

for x in a { print(x) }
来源：http://zis.zhongyouzk.top

[T22] Swift：字典
来源：http://owp.quarkkingdee.top

var d = ["a": 1];  d["b"] = 2
来源：http://ipi.fzhhl.top

[T23] Swift：函数
来源：http://wrf.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ckk.vqdsnc.cn

[T24] Swift：闭包
来源：http://old.shanyushiyangtech.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://luk.zhoulong.xyz

[T25] Swift：结构体
来源：http://fnm.aizwys.cn

struct P { var x: Int }
来源：http://tke.svipenyu.cn

[T26] Swift：类与重写
来源：http://mhk.andypj.xyz

class A: Base { override func f() {} }
来源：http://xex.andypj.xyz

[T27] Swift：错误处理
来源：http://blh.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://xng.yongpay.top

[T28] Swift：枚举
来源：http://owf.gogol.net.cn

enum Color { case red, green }
来源：http://yyw.uphjek.com

[T29] Swift：guard 提前返回
来源：http://wgd.svipenyu.cn

guard let x = opt else { return }
来源：http://yan.nanxinkj.top

[T30] Swift：协议
来源：http://lfh.shuidangran.top

protocol Shape { func area() -> Double }
来源：http://wxc.jqgufenzy.top

[T31] Lua：Hello World
来源：http://vbo.meibo888.top

print("Hello")
来源：http://frk.ppjwa.cn

[T32] Lua：局部变量
来源：http://wxw.ehwqpu.com

local a = 1
来源：http://nku.zycfv.cn

[T33] Lua：表（数组）
来源：http://flq.tianlin.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://kst.zhoulong.xyz

[T34] Lua：遍历表
来源：http://jwg.yj20258.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mny.andypj.xyz

[T35] Lua：字典表
来源：http://xkg.haohaochexian.top

local d = { a = 1 };  d.b = 2
来源：http://bsv.hnxiangtu.top

[T36] Lua：函数
来源：http://cjh.shanyushiyangtech.top

function add(a, b) return a + b end
来源：http://amr.sjlbkw.cn

[T37] Lua：字符串拼接
来源：http://vpn.jlsjyb.cn

"a" .. "b"
来源：http://jtb.9152youxi.cn

[T38] Lua：条件
来源：http://cqd.hywenlv.cn

if x > 0 then print("正") end
来源：http://ftr.bjfxy.top

[T39] Lua：模式匹配
来源：http://uhc.sufxvd.cn

string.find(s, "%d+")
来源：http://rnl.hnqzz.top

[T40] Lua：元表
来源：http://bsx.hnqzz.top

setmetatable({}, { __index = base })
来源：http://zck.9152youxi.cn

[T41] Perl：Hello World
来源：http://fjf.zycfv.cn

print "Hello\n";
来源：http://ywk.andypj.xyz

[T42] Perl：变量类型
来源：http://irn.yongpay.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qhe.daxiang520.top

[T43] Perl：字符串插值
来源：http://bwn.haohaochexian.top

"值: $a"
来源：http://uiw.yueranfly.top

[T44] Perl：条件
来源：http://qnp.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://vrd.sxryk.cn

[T45] Perl：数组遍历
来源：http://awf.gzhubu.top

for my $x (@arr) { print $x; }
来源：http://dbp.tanke756.top

[T46] Perl：哈希操作
来源：http://olm.0kj1m.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oii.bbcook.cn

[T47] Perl：正则捕获
来源：http://kbg.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qre.epnwcf.com

[T48] Perl：正则替换
来源：http://eed.hnqzz.top

$s =~ s/old/new/g;
来源：http://wcg.meibo888.top

[T49] Perl：函数
来源：http://ibv.guannengcc.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mpa.jinghuilouyu.cn

[T50] Perl：逐行读文件
来源：http://chj.zhengqikj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://psz.shanyushiyangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://epf.52xcode.cn

[T51] Scala：Hello World
来源：http://kme.sweek.top

println("Hello")
来源：http://dvo.zhijiandao.cn

[T52] Scala：变量
来源：http://bpq.hcnkem.com

val a = 1;  var b = 2
来源：http://dmf.iojbl.cn

[T53] Scala：字符串插值
来源：http://psm.jlsjyb.cn

s"值: $b"
来源：http://wga.xylfe.cn

[T54] Scala：集合映射
来源：http://cdb.iojbl.cn

List(1, 2, 3).map(_ * 2)
来源：http://rmk.bjfxy.top

[T55] Scala：集合过滤
来源：http://jdj.jyoumei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ssv.jianghu66.top

[T56] Scala：样例类
来源：http://cla.sxryk.cn

case class User(name: String, age: Int)
来源：http://kri.hesvh.cn

[T57] Scala：模式匹配
来源：http://thk.fengsongda.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xpy.guannengcc.top

[T58] Scala：函数定义
来源：http://yxw.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://dyg.yanxiufei.cn

[T59] Scala：循环
来源：http://deh.yfazqb.com

for (i <- 1 to 10) println(i)
来源：http://gpv.yvedp.cn

[T60] Scala：折叠
来源：http://zcv.zhaomingkeji.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://utn.shzxlz.cn

================================================================================
来源：http://cqj.fzhhl.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nbo.gogol.net.cn

================================================================================
来源：http://bst.yonumen.top

[U01] Py：创建虚拟环境
来源：http://cny.c1oappe.top

python -m venv .venv && source .venv/bin/activate
来源：http://yiu.jqgufenzy.top

[U02] Py：导出 / 安装依赖
来源：http://jxm.xuanzx.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uft.316326.xyz

[U03] Py：加载 .env 配置
来源：http://ctk.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tqw.9152youxi.cn

[U04] Py：变量调试打印
来源：http://ora.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://beh.chenlongwang.top

[U05] Py：列表去重且保序
来源：http://kfh.zycfv.cn

list(dict.fromkeys(arr))
来源：http://kdo.9152youxi.cn

[U06] Py：合并两个字典
来源：http://rsd.hfpthk.cn

{**a, **b}
来源：http://yaj.shuidangran.top

[U07] Py：反转字典键值
来源：http://nsy.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://ymx.tianlin.xyz

[U08] Py：展平二维列表
来源：http://lat.fzhhl.top

[y for x in nested for y in x]
来源：http://qzm.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://hkq.9152youxi.cn

max(d, key=d.get)
来源：http://bir.aibaodan.cn

[U10] Py：按值排序字典
来源：http://rwf.andypj.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qnh.cheryme.top

[U11] Py：生成器表达式
来源：http://udx.yvedp.cn

(x * 2 for x in arr)
来源：http://gix.tian-w.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uvq.tarul.cn

Counter(arr).most_common(3)
来源：http://iap.shuidangran.top

[U13] Py：固定长度队列
来源：http://hum.tianlin.xyz

deque(maxlen=10)
来源：http://gbs.zhixingplan.top

[U14] Py：分组收集到列表
来源：http://hvc.zhixingplan.top

defaultdict(list)
来源：http://euk.fktsv.cn

[U15] Py：高精度计时
来源：http://uxg.gotoacloud.top

t = time.perf_counter()
来源：http://tso.svipenyu.cn

[U16] Py：命令行参数解析
来源：http://oqw.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qbg.yuanzhike.top

[U17] Py：初始化日志
来源：http://vfc.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://sja.wangshuangyany.cn

[U18] Py：预编译正则
来源：http://weg.ehwqpu.com

pat = re.compile(r"\d+")
来源：http://tkh.tian-w.cn

[U19] Py：正则替换带回调
来源：http://wda.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dpb.jyoumei.cn

[U20] Py：缓存函数结果
来源：http://ceb.yongpay.top

@functools.lru_cache(maxsize=None)
来源：http://kea.sxryk.cn

[U21] Py：自定义上下文管理器
来源：http://tmc.wangshuangyany.cn

@contextlib.contextmanager
来源：http://rcf.yueranfly.top

[U22] Py：矩阵转置
来源：http://rxn.ehwqpu.com

list(zip(*m))
来源：http://aev.ywan-chungtsiang.top

[U23] Py：分块读取大文件
来源：http://orr.ydjk.org.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uwk.jqgufenzy.top

[U24] Py：路径操作
来源：http://dhn.jiagoushi.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wod.zycfv.cn

[U25] Py：CSV 按字典读
来源：http://cnk.nwbrower.top

csv.DictReader(f)
来源：http://qph.jiagoushi.top

[U26] Py：并发下载
来源：http://lvu.chenlongwang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pyb.nwbrower.top

[U27] Py：异步 HTTP
来源：http://tih.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://xww.xinyue.icu

[U28] Py：类型别名
来源：http://ble.jlsjyb.cn

UserId = int
来源：http://maz.jqgfzy.top

[U29] Py：属性校验
来源：http://imo.guannengcc.top

@property 与 @x.setter 配合
来源：http://bhk.kuanghao11.cn

[U30] Py：数据类
来源：http://iwn.yvedp.cn

@dataclass(slots=True)
来源：http://gtu.aizwys.cn

[U31] Py：单测
来源：http://eqb.haohaochexian.top

python -m pytest -q
来源：http://exv.sjlbkw.cn

[U32] Py：代码格式化
来源：http://jtv.0kj1m.cn

ruff format . && ruff check --fix .
来源：http://bna.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://nnr.gogol.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://lnd.shuidangran.top

[U34] Py：判断编码
来源：http://pwa.bjfxy.top

chardet.detect(raw)
来源：http://psy.jianghu66.top

[U35] Py：发送邮件
来源：http://hkn.smart0.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mju.yongpay.top

[U36] Py：定时任务
来源：http://syz.pengpengdd.cyou

schedule.every(10).minutes.do(job)
来源：http://lcj.zdqjudy.top

[U37] Py：读写 Excel
来源：http://wqt.daxiang520.top

pandas.read_excel / DataFrame.to_excel
来源：http://aek.daxiang520.top

[U38] Py：获取脚本所在目录
来源：http://mho.zhixingplan.top

Path(__file__).resolve().parent
来源：http://vwt.shuidangran.top

[U39] Py：判断是否在交互环境
来源：http://nql.shzxlz.cn

sys.stdout.isatty()
来源：http://qin.dashuyun.cn

[U40] Py：打印到标准错误
来源：http://dmg.guannengcc.top

print("err", file=sys.stderr)
来源：http://yht.hfpthk.cn

[U41] PHP：初始化 Composer 项目
来源：http://cmw.bjfxy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rci.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://gha.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iml.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://myg.yfazqb.com

namespace App\Http;
来源：http://ang.shzxlz.cn

[U44] PHP：开启严格类型
来源：http://qej.feifeiyinyue.top

declare(strict_types=1);
来源：http://svy.bbcook.cn

[U45] PHP：类型声明与返回类型
来源：http://edq.uphjek.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://bfh.cqqwz.cn

[U46] PHP：可空类型
来源：http://kxs.chenjidiqi.icu

?string $name = null
来源：http://lov.cdnleiting.top

[U47] PHP：联合类型
来源：http://hkg.cucudq.cn

int|string $id
来源：http://ojz.nanxinkj.top

[U48] PHP：纯枚举
来源：http://fcl.yueranfly.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vif.yuanzhike.top

[U49] PHP：只读属性
来源：http://jry.chenjidiqi.icu

public readonly string $name
来源：http://wke.hcnkem.com

[U50] PHP：构造器属性提升
来源：http://qtc.daxiang520.top

public function __construct(private int $id) {}
来源：http://fsi.yj20258.top

[U51] PHP：数组解构
来源：http://dlt.aibaodan.cn

[$a, $b] = $arr;
来源：http://ppi.havefunace.top

[U52] PHP：箭头函数
来源：http://wwv.cucudq.cn

$double = fn($x) => $x * 2;
来源：http://hdl.ywan-chungtsiang.top

[U53] PHP：空合并运算符
来源：http://bfe.bbcook.cn

$v = $a ?? $b ?? "default";
来源：http://msd.guowangkeji.top

[U54] PHP：空安全调用
来源：http://zgt.fengsongda.top

$obj?->method()
来源：http://wco.yuanzhike.top

[U55] PHP：match 表达式
来源：http://jno.ydzc1.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://aez.zhongyouzk.top

[U56] PHP：命名参数
来源：http://jyn.ppjwa.cn

f(a: 1, b: 2)
来源：http://oau.fzhhl.top

[U57] PHP：字符串插值
来源：http://gec.tanke756.top

"值: {$a}"
来源：http://oik.yonumen.top

[U58] PHP：数组三件套
来源：http://ujg.daria6918.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xgw.chenjidiqi.icu


<!-- 参考信息 -->