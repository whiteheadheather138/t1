代发 wailian999

#include <iostream>
来源：http://yhj.nanxinkj.top

int main() { std::cout << "Hello\n"; }
来源：http://zxx.hammf.cn

[S32] C++：字符串
来源：http://tsv.jlsjyb.cn

std::string s = "hi";  s += "!";
来源：http://zrx.xylfe.cn

[S33] C++：vector 增删
来源：http://rel.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xps.hcnkem.com

[S34] C++：遍历 vector
来源：http://fqg.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ozu.zdbjq.cn

[S35] C++：map
来源：http://dbj.hnqzz.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://utn.chenlongwang.top

[S36] C++：unordered_map
来源：http://ofa.guannengcc.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://age.mhx1999.top

[S37] C++：set
来源：http://xil.redwolf501.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ioc.feifeiyinyue.top

[S38] C++：排序
来源：http://eyq.nanxuanxn.top

std::sort(v.begin(), v.end());
来源：http://bdr.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://psl.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zio.ehwqpu.com

[S40] C++：查找元素
来源：http://zvb.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vdp.smart0.xyz

[S41] C++：类与构造函数
来源：http://oox.bjfxy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zpj.yuanzhike.top

[S42] C++：继承与虚函数
来源：http://lrq.yfazqb.com

class B : public Base { public: void f() override {} };
来源：http://uku.cdnleiting.top

[S43] C++：智能指针
来源：http://rbm.sweek.top

auto p = std::make_unique<int>(5);
来源：http://yyz.zycfv.cn

[S44] C++：引用传参
来源：http://aor.mhx1999.top

void inc(int &x) { ++x; }
来源：http://lrj.chenlongwang.top

[S45] C++：lambda
来源：http://qmg.xziqi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hhd.hesvh.cn

[S46] C++：函数模板
来源：http://xid.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aqa.yj202588.top

[S47] C++：结构化绑定遍历
来源：http://bcg.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uml.bbcook.cn

[S48] C++：逐行读文件
来源：http://tou.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://fxl.haohaochexian.top

while (std::getline(in, line)) { }
来源：http://gos.vehdjk.com

[S49] C++：写文件
来源：http://yis.shangyingyoupin.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rdt.cqqwz.cn

[S50] C++：格式化数字
来源：http://zvb.nwbrower.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://npk.gzhubu.top

[S51] C++：显式类型转换
来源：http://ymv.quarkkingdee.top

static_cast<double>(a) / b
来源：http://ekn.hfpthk.cn

[S52] C++：const 与 noexcept
来源：http://hdd.zdqjudy.top

int size() const noexcept { return n_; }
来源：http://jgm.jlsjyb.cn

[S53] C++：移动语义
来源：http://djz.0kj1m.cn

std::vector<int> w = std::move(v);
来源：http://exk.shzxlz.cn

[S54] C++：异常处理
来源：http://jgd.cqqwz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wrd.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://xwo.jinqigfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dpw.zhengqikj.top

[S56] C++：optional
来源：http://aqm.havefunace.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oen.pycfn.com

[S57] C++：编译期常量
来源：http://ovc.guannengcc.top

constexpr int N = 10;
来源：http://hja.jqgfzy.top

[S58] C++：命名空间
来源：http://xdx.shanyushiyangtech.top

namespace ns { int f() { return 1; } }
来源：http://ndl.ppjwa.cn

[S59] C++：静态断言
来源：http://teh.bbcook.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vbd.316326.xyz

[S60] C++：遍历并删除元素
来源：http://oci.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xxk.cdnleiting.top

================================================================================
来源：http://xdk.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wvg.mhx1999.top

================================================================================
来源：http://rwq.hywenlv.cn

[T01] Kotlin：Hello World
来源：http://rjo.fktsv.cn

println("Hello")
来源：http://tdl.jqgufenzy.top

[T02] Kotlin：变量
来源：http://jgh.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jkr.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://xor.tanke756.top

"值: $b"
来源：http://gnl.hammf.cn

[T04] Kotlin：空安全
来源：http://ixk.fzhhl.top

val n: String? = null;  n?.length
来源：http://sxi.yj202588.top

[T05] Kotlin：when 表达式
来源：http://wro.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bks.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://lij.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://off.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://tld.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://dpb.dashuyun.cn

[T08] Kotlin：数据类
来源：http://tck.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://sgg.yuanzhike.top

[T09] Kotlin：扩展函数
来源：http://eyx.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://ivr.redwolf501.top

[T10] Kotlin：默认参数
来源：http://pzd.chenlongwang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mia.jianghu66.top

[T11] Kotlin：协程
来源：http://ohc.aibaodan.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sjt.gotoacloud.top

[T12] Kotlin：解构声明
来源：http://nrf.yj20258888.top

val (a, b) = Pair(1, 2)
来源：http://wlr.dashuyun.cn

[T13] Kotlin：只读 Map
来源：http://iyw.hesvh.cn

val m = mapOf("a" to 1)
来源：http://wif.guannengcc.top

[T14] Kotlin：循环
来源：http://bxd.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://flx.daria6918.cn

[T15] Kotlin：接口
来源：http://rzv.daxiang520.top

interface Shape { fun area(): Double }
来源：http://tam.mhx1999.top

[T16] Swift：Hello World
来源：http://yzc.ybcxt.top

print("Hello")
来源：http://wqh.daxiang520.top

[T17] Swift：变量与常量
来源：http://rur.cqqwz.cn

var a = 1;  let b = 2
来源：http://jwj.chenlongwang.top

[T18] Swift：字符串插值
来源：http://qch.fengsongda.top

"值: \(b)"
来源：http://svg.pycfn.com

[T19] Swift：可选绑定
来源：http://dpa.wangdashe.top

if let n = opt { print(n) }
来源：http://cnb.shuidangran.top

[T20] Swift：数组操作
来源：http://lxn.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kga.jqgfzy.top

[T21] Swift：遍历
来源：http://ohj.gzhubu.top

for x in a { print(x) }
来源：http://szk.jlsjyb.cn

[T22] Swift：字典
来源：http://vbs.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://yjs.quarkkingdee.top

[T23] Swift：函数
来源：http://aby.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uqv.nanxinkj.top

[T24] Swift：闭包
来源：http://tqo.vehdjk.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://dyj.meibo888.top

[T25] Swift：结构体
来源：http://ken.yangfankeji.com

struct P { var x: Int }
来源：http://npz.ehwqpu.com

[T26] Swift：类与重写
来源：http://blg.daxiang520.top

class A: Base { override func f() {} }
来源：http://opz.zhoulong.xyz

[T27] Swift：错误处理
来源：http://mxg.jqgfzy.top

do { try f() } catch { print(error) }
来源：http://hyl.yj202588.top

[T28] Swift：枚举
来源：http://gea.ppjwa.cn

enum Color { case red, green }
来源：http://tsx.hfpthk.cn

[T29] Swift：guard 提前返回
来源：http://wck.jinghuilouyu.cn

guard let x = opt else { return }
来源：http://vgn.sxryk.cn

[T30] Swift：协议
来源：http://epm.yangfankeji.com

protocol Shape { func area() -> Double }
来源：http://nmv.quarkkingdee.top

[T31] Lua：Hello World
来源：http://tgp.feifeiyinyue.top

print("Hello")
来源：http://tep.c1oappe.top

[T32] Lua：局部变量
来源：http://xlz.yvedp.cn

local a = 1
来源：http://ntq.9152youxi.cn

[T33] Lua：表（数组）
来源：http://hcr.xuanzx.com

local t = {1, 2, 3};  t[4] = 4
来源：http://tds.xylfe.cn

[T34] Lua：遍历表
来源：http://brx.meibo888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hjd.yonumen.top

[T35] Lua：字典表
来源：http://hnq.andypj.xyz

local d = { a = 1 };  d.b = 2
来源：http://pze.uphjek.com

[T36] Lua：函数
来源：http://plo.fzhhl.top

function add(a, b) return a + b end
来源：http://dot.jianghu66.top

[T37] Lua：字符串拼接
来源：http://lqe.zdqjudy.top

"a" .. "b"
来源：http://gkp.pycfn.com

[T38] Lua：条件
来源：http://bfu.xylfe.cn

if x > 0 then print("正") end
来源：http://zql.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://pfl.andypj.xyz

string.find(s, "%d+")
来源：http://gkz.yj20258888.top

[T40] Lua：元表
来源：http://rrz.vehdjk.com

setmetatable({}, { __index = base })
来源：http://ubr.mhx1999.top

[T41] Perl：Hello World
来源：http://pho.fehbvm.com

print "Hello\n";
来源：http://lfl.jinqigfzy.top

[T42] Perl：变量类型
来源：http://qnf.feifeiyinyue.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gib.pycfn.com

[T43] Perl：字符串插值
来源：http://acr.yuxming.cn

"值: $a"
来源：http://men.tian-w.cn

[T44] Perl：条件
来源：http://oht.tarul.cn

if ($a > 0) { print "正"; }
来源：http://aqs.andypj.xyz

[T45] Perl：数组遍历
来源：http://fmv.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://pom.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://fge.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://and.ivvv.top

[T47] Perl：正则捕获
来源：http://evb.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vbp.yj202588.top

[T48] Perl：正则替换
来源：http://vxs.hnxiangtu.top

$s =~ s/old/new/g;
来源：http://xze.shangyingyoupin.top

[T49] Perl：函数
来源：http://hml.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://apj.shuidangran.top

[T50] Perl：逐行读文件
来源：http://cmq.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ymp.snrcjt.cn

while (my $line = <$fh>) { print $line; }
来源：http://lgf.hywenlv.cn

[T51] Scala：Hello World
来源：http://nll.quarkkingdee.top

println("Hello")
来源：http://eme.zhoulong.xyz

[T52] Scala：变量
来源：http://ljb.fanxiaobao.xyz

val a = 1;  var b = 2
来源：http://mjo.gogol.net.cn

[T53] Scala：字符串插值
来源：http://xus.xingfuxueyuan.xyz

s"值: $b"
来源：http://hmx.hcnkem.com

[T54] Scala：集合映射
来源：http://fre.gaohongyu789.top

List(1, 2, 3).map(_ * 2)
来源：http://ulw.epnwcf.com

[T55] Scala：集合过滤
来源：http://ijq.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://wxr.cashguo.top

[T56] Scala：样例类
来源：http://wws.bjfxy.top

case class User(name: String, age: Int)
来源：http://tlm.zycfv.cn

[T57] Scala：模式匹配
来源：http://ser.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://orp.meibo888.top

[T58] Scala：函数定义
来源：http://asz.chenjidiqi.icu

def add(a: Int, b: Int): Int = a + b
来源：http://hbh.ctjpmb.com

[T59] Scala：循环
来源：http://gjc.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://hbk.haohaochexian.top

[T60] Scala：折叠
来源：http://wse.xylfe.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lux.shuidangran.top

================================================================================
来源：http://ihs.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xhe.jinqigufen.top

================================================================================
来源：http://mnr.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://apj.gotoacloud.top

python -m venv .venv && source .venv/bin/activate
来源：http://blv.dashuyun.cn

[U02] Py：导出 / 安装依赖
来源：http://lfm.shangyingyoupin.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://frs.ehwqpu.com

[U03] Py：加载 .env 配置
来源：http://qqu.dashuyun.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nur.xuetiantiany.cn

[U04] Py：变量调试打印
来源：http://wcl.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jpe.sysykeji.top

[U05] Py：列表去重且保序
来源：http://tii.316326.xyz

list(dict.fromkeys(arr))
来源：http://ssm.haohaochexian.top

[U06] Py：合并两个字典
来源：http://wsj.bbcook.cn

{**a, **b}
来源：http://yzq.hfpthk.cn

[U07] Py：反转字典键值
来源：http://fiz.ivvv.top

{v: k for k, v in d.items()}
来源：http://vso.cqqwz.cn

[U08] Py：展平二维列表
来源：http://hbe.hnqzz.top

[y for x in nested for y in x]
来源：http://vxc.jinqigfzy.top

[U09] Py：字典取最大值的键
来源：http://asv.shuidangran.top

max(d, key=d.get)
来源：http://fci.hcnkem.com

[U10] Py：按值排序字典
来源：http://skj.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pwq.c1oappe.top

[U11] Py：生成器表达式
来源：http://bsl.tarul.cn

(x * 2 for x in arr)
来源：http://mep.dianchejie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zry.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://etp.cashguo.top

[U13] Py：固定长度队列
来源：http://zgu.yuxming.cn

deque(maxlen=10)
来源：http://ojr.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://fos.yuxming.cn

defaultdict(list)
来源：http://avd.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://rhr.fanxiaobao.xyz

t = time.perf_counter()
来源：http://zmj.sxryk.cn

[U16] Py：命令行参数解析
来源：http://lxc.pengpengdd.cyou

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qkn.daria6918.cn

[U17] Py：初始化日志
来源：http://kzj.zhoulong.xyz

logging.basicConfig(level=logging.INFO)
来源：http://dfp.yonumen.top

[U18] Py：预编译正则
来源：http://vwd.zycfv.cn

pat = re.compile(r"\d+")
来源：http://hfs.shuidangran.top

[U19] Py：正则替换带回调
来源：http://keq.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iio.yonumen.top

[U20] Py：缓存函数结果
来源：http://sus.tarul.cn

@functools.lru_cache(maxsize=None)
来源：http://yyg.yj20258888.top

[U21] Py：自定义上下文管理器
来源：http://zyr.yfazqb.com

@contextlib.contextmanager
来源：http://kti.cdnleiting.top

[U22] Py：矩阵转置
来源：http://kwo.wangdashe.top

list(zip(*m))
来源：http://woy.yj202588.top

[U23] Py：分块读取大文件
来源：http://vrb.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gzo.shuidangran.top

[U24] Py：路径操作
来源：http://uhg.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bux.nwbrower.top

[U25] Py：CSV 按字典读
来源：http://pvl.yj20258.top

csv.DictReader(f)
来源：http://oje.sufxvd.cn

[U26] Py：并发下载
来源：http://mfi.zdbjq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qoy.andypj.xyz

[U27] Py：异步 HTTP
来源：http://pmg.gotoacloud.top

aiohttp.ClientSession() 配合 async with
来源：http://kor.cqqwz.cn

[U28] Py：类型别名
来源：http://agk.bjfxy.top

UserId = int
来源：http://eai.nanxinkj.top

[U29] Py：属性校验
来源：http://pty.sufxvd.cn

@property 与 @x.setter 配合
来源：http://fya.haohaochexian.top

[U30] Py：数据类
来源：http://xlv.epnwcf.com

@dataclass(slots=True)
来源：http://oip.sjlbkw.cn

[U31] Py：单测
来源：http://qei.zhixingplan.top

python -m pytest -q
来源：http://fal.chenzaomai.com

[U32] Py：代码格式化
来源：http://kso.daria6918.cn

ruff format . && ruff check --fix .
来源：http://czr.nanxinkj.top

[U33] Py：打包发布
来源：http://vnb.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://ngl.zhixingplan.top

[U34] Py：判断编码
来源：http://yil.ybcxt.top

chardet.detect(raw)
来源：http://vfa.zhongyouzk.top

[U35] Py：发送邮件
来源：http://hfm.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ear.haohaochexian.top

[U36] Py：定时任务
来源：http://gpx.pycfn.com

schedule.every(10).minutes.do(job)
来源：http://fez.sufxvd.cn

[U37] Py：读写 Excel
来源：http://dzl.zhixingplan.top

pandas.read_excel / DataFrame.to_excel
来源：http://ovr.jianghu66.top

[U38] Py：获取脚本所在目录
来源：http://zhb.c1oappe.top

Path(__file__).resolve().parent
来源：http://wmk.jlsjyb.cn

[U39] Py：判断是否在交互环境
来源：http://fwh.chenjidiqi.icu

sys.stdout.isatty()
来源：http://rav.tian-w.cn

[U40] Py：打印到标准错误
来源：http://xoc.jqgfzy.top

print("err", file=sys.stderr)
来源：http://omn.shzxlz.cn

[U41] PHP：初始化 Composer 项目
来源：http://nzo.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pyl.jinyuanbaomall.cn

[U42] PHP：PSR-4 自动加载
来源：http://nem.sysykeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vkt.sufxvd.cn

[U43] PHP：声明命名空间
来源：http://svo.hfpthk.cn

namespace App\Http;
来源：http://pkc.ywan-chungtsiang.top

[U44] PHP：开启严格类型
来源：http://hve.daria6918.cn

declare(strict_types=1);
来源：http://mbi.snrcjt.cn

[U45] PHP：类型声明与返回类型
来源：http://oun.yanxiufei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mnb.zhengqikj.top

[U46] PHP：可空类型
来源：http://wue.yj20258888.top

?string $name = null
来源：http://yml.cashguo.top

[U47] PHP：联合类型
来源：http://bpi.hnxiangtu.top

int|string $id
来源：http://ztk.pengpengdd.cyou

[U48] PHP：纯枚举
来源：http://xsw.yvedp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ahg.fehbvm.com

[U49] PHP：只读属性
来源：http://fpy.jinyuanbaomall.cn

public readonly string $name
来源：http://fzo.c1oappe.top

[U50] PHP：构造器属性提升
来源：http://jhr.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://pyk.hfpthk.cn

[U51] PHP：数组解构
来源：http://uee.yonumen.top

[$a, $b] = $arr;
来源：http://vqn.tianlin.xyz

[U52] PHP：箭头函数
来源：http://uyr.jinqigfzy.top

$double = fn($x) => $x * 2;
来源：http://opi.guowangkeji.top

[U53] PHP：空合并运算符
来源：http://zmb.gaohongyu789.top

$v = $a ?? $b ?? "default";
来源：http://men.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://kcm.fanxiaobao.xyz

$obj?->method()
来源：http://nzp.epnwcf.com

[U55] PHP：match 表达式
来源：http://xfx.yj20258.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://onk.gotoacloud.top

[U56] PHP：命名参数
来源：http://kvm.shanyushiyangtech.top

f(a: 1, b: 2)
来源：http://mdy.zhijiandao.cn


<!-- 参考信息 -->