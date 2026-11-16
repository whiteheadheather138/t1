代发 wailian999

#include <iostream>
来源：http://dww.jianghu66.top

int main() { std::cout << "Hello\n"; }
来源：http://mgm.bjfxy.top

[S32] C++：字符串
来源：http://qbk.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://apg.jinyuanbaomall.cn

[S33] C++：vector 增删
来源：http://lhz.ydjk.org.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pqz.yfazqb.com

[S34] C++：遍历 vector
来源：http://jgq.birdmap.top

for (auto &x : v) { std::cout << x; }
来源：http://gkz.cdnleiting.top

[S35] C++：map
来源：http://dzv.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://njo.epnwcf.com

[S36] C++：unordered_map
来源：http://oph.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tdw.tian-w.cn

[S37] C++：set
来源：http://ylc.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://psf.jiagoushi.top

[S38] C++：排序
来源：http://giz.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://acm.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://tem.yvedp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://okq.epnwcf.com

[S40] C++：查找元素
来源：http://cpw.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lrf.zhixingplan.top

[S41] C++：类与构造函数
来源：http://wpm.zdbjq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wpu.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://flk.9152youxi.cn

class B : public Base { public: void f() override {} };
来源：http://iob.quarkkingdee.top

[S43] C++：智能指针
来源：http://bhl.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://sky.zhaomingkeji.xyz

[S44] C++：引用传参
来源：http://yqc.pengpengdd.cyou

void inc(int &x) { ++x; }
来源：http://gjv.meibo888.top

[S45] C++：lambda
来源：http://yoj.ybcxt.top

auto add = [](int a, int b) { return a + b; };
来源：http://ucz.xylfe.cn

[S46] C++：函数模板
来源：http://bqm.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mqy.ydzc1.top

[S47] C++：结构化绑定遍历
来源：http://ajj.zhixingplan.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ski.daria6918.cn

[S48] C++：逐行读文件
来源：http://rds.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vds.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://ixo.sjlbkw.cn

[S49] C++：写文件
来源：http://lnz.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://szl.0kj1m.cn

[S50] C++：格式化数字
来源：http://ire.yvedp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hyr.gzhubu.top

[S51] C++：显式类型转换
来源：http://itl.xuetiantiany.cn

static_cast<double>(a) / b
来源：http://ihv.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://cld.yvedp.cn

int size() const noexcept { return n_; }
来源：http://xjb.jiagoushi.top

[S53] C++：移动语义
来源：http://bkn.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://izf.zycfv.cn

[S54] C++：异常处理
来源：http://wcd.cashguo.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dfv.jiagoushi.top

[S55] C++：结构化绑定
来源：http://uyh.jinqigfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bza.mhx1999.top

[S56] C++：optional
来源：http://cel.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wyd.cheryme.top

[S57] C++：编译期常量
来源：http://tyi.hongshengwenyu.top

constexpr int N = 10;
来源：http://fcm.sxryk.cn

[S58] C++：命名空间
来源：http://rht.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://jkk.hcnkem.com

[S59] C++：静态断言
来源：http://tdm.feifeiyinyue.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dpe.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://sjk.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xqo.hnqzz.top

================================================================================
来源：http://gwm.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mdk.ydjk.org.cn

================================================================================
来源：http://qjn.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://ngu.sjlbkw.cn

println("Hello")
来源：http://rfw.guannengcc.top

[T02] Kotlin：变量
来源：http://tec.fehbvm.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hhj.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://jlr.gotoacloud.top

"值: $b"
来源：http://yra.hesvh.cn

[T04] Kotlin：空安全
来源：http://iap.ywan-chungtsiang.top

val n: String? = null;  n?.length
来源：http://hub.jinqigufen.top

[T05] Kotlin：when 表达式
来源：http://qbi.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://upl.redwolf501.top

[T06] Kotlin：集合映射
来源：http://vit.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ucr.haohaochexian.top

[T07] Kotlin：集合过滤
来源：http://nsl.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qno.hysaishi.cn

[T08] Kotlin：数据类
来源：http://iee.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://efj.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://flw.fanxiaobao.xyz

fun String.exclaim() = this + "!"
来源：http://xfm.yfazqb.com

[T10] Kotlin：默认参数
来源：http://zua.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ups.guowangkeji.top

[T11] Kotlin：协程
来源：http://luc.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kry.zdbjq.cn

[T12] Kotlin：解构声明
来源：http://nfc.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://zql.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://ggr.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://rzk.yonumen.top

[T14] Kotlin：循环
来源：http://cbf.sufxvd.cn

for (i in 1..10) println(i)
来源：http://ehj.nwbrower.top

[T15] Kotlin：接口
来源：http://saf.cashguo.top

interface Shape { fun area(): Double }
来源：http://sjs.sxryk.cn

[T16] Swift：Hello World
来源：http://ueh.pengpengdd.cyou

print("Hello")
来源：http://yhp.nanxinkj.top

[T17] Swift：变量与常量
来源：http://yzs.ydzc1.top

var a = 1;  let b = 2
来源：http://pic.aizwys.cn

[T18] Swift：字符串插值
来源：http://ssm.shanyushiyangkeji.top

"值: \(b)"
来源：http://ssn.zhongyouzk.top

[T19] Swift：可选绑定
来源：http://zdb.guannengcc.top

if let n = opt { print(n) }
来源：http://xec.zycfv.cn

[T20] Swift：数组操作
来源：http://pfg.xinyue.icu

var a = [1, 2, 3];  a.append(4)
来源：http://kxm.xingfuxueyuan.xyz

[T21] Swift：遍历
来源：http://auh.epnwcf.com

for x in a { print(x) }
来源：http://nyy.yuxming.cn

[T22] Swift：字典
来源：http://vhz.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://aiq.aibaodan.cn

[T23] Swift：函数
来源：http://tmt.gotoacloud.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zga.ybcxt.top

[T24] Swift：闭包
来源：http://epn.xuanzx.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://vuk.pengpengdd.cyou

[T25] Swift：结构体
来源：http://ddg.jiagoushi.top

struct P { var x: Int }
来源：http://tth.hnxiangtu.top

[T26] Swift：类与重写
来源：http://dto.yangfankeji.com

class A: Base { override func f() {} }
来源：http://pje.ydzc1.top

[T27] Swift：错误处理
来源：http://two.jqgufenzy.top

do { try f() } catch { print(error) }
来源：http://cnp.chenjidiqi.icu

[T28] Swift：枚举
来源：http://gyj.yj202588.top

enum Color { case red, green }
来源：http://ysf.yvedp.cn

[T29] Swift：guard 提前返回
来源：http://kkw.yvedp.cn

guard let x = opt else { return }
来源：http://epb.gogol.net.cn

[T30] Swift：协议
来源：http://vao.zhiwuduotai.top

protocol Shape { func area() -> Double }
来源：http://uyz.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://zon.zhaomingkeji.xyz

print("Hello")
来源：http://pwe.haohaochexian.top

[T32] Lua：局部变量
来源：http://aob.sweek.top

local a = 1
来源：http://mje.cucudq.cn

[T33] Lua：表（数组）
来源：http://rlp.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xij.jianghu66.top

[T34] Lua：遍历表
来源：http://gbn.gzhubu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qmr.yueranfly.top

[T35] Lua：字典表
来源：http://jah.yueranfly.top

local d = { a = 1 };  d.b = 2
来源：http://gjf.aizwys.cn

[T36] Lua：函数
来源：http://qqk.jiagoushi.top

function add(a, b) return a + b end
来源：http://mal.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://ykb.tianlin.xyz

"a" .. "b"
来源：http://vfb.meibo888.top

[T38] Lua：条件
来源：http://wjf.hnqzz.top

if x > 0 then print("正") end
来源：http://vrl.zhengqikj.top

[T39] Lua：模式匹配
来源：http://ydl.sxryk.cn

string.find(s, "%d+")
来源：http://ajl.wangdashe.top

[T40] Lua：元表
来源：http://ekc.snrcjt.cn

setmetatable({}, { __index = base })
来源：http://pdm.hnqzz.top

[T41] Perl：Hello World
来源：http://qvc.tianlin.xyz

print "Hello\n";
来源：http://oyd.kuanghao11.cn

[T42] Perl：变量类型
来源：http://bon.feifeiyinyue.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://okh.fehbvm.com

[T43] Perl：字符串插值
来源：http://bxe.gaohongyu789.top

"值: $a"
来源：http://ypi.xylfe.cn

[T44] Perl：条件
来源：http://pvg.sjlbkw.cn

if ($a > 0) { print "正"; }
来源：http://odr.vqdsnc.cn

[T45] Perl：数组遍历
来源：http://zdb.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://kbp.ehwqpu.com

[T46] Perl：哈希操作
来源：http://amb.sxryk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aoi.havefunace.top

[T47] Perl：正则捕获
来源：http://xqi.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hmm.quarkkingdee.top

[T48] Perl：正则替换
来源：http://ubx.fktsv.cn

$s =~ s/old/new/g;
来源：http://sgj.zhiwuduotai.top

[T49] Perl：函数
来源：http://lck.jianghu66.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qmj.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://uqr.zhoulong.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://xsd.jqgfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://evg.yvedp.cn

[T51] Scala：Hello World
来源：http://ubk.aibaodan.cn

println("Hello")
来源：http://aus.yj20258888.top

[T52] Scala：变量
来源：http://syw.gaohongyu789.top

val a = 1;  var b = 2
来源：http://zkz.uphjek.com

[T53] Scala：字符串插值
来源：http://vlt.yj202588.top

s"值: $b"
来源：http://thk.kuanghao11.cn

[T54] Scala：集合映射
来源：http://ghi.zdqjudy.top

List(1, 2, 3).map(_ * 2)
来源：http://oaq.xinyue.icu

[T55] Scala：集合过滤
来源：http://euv.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gqm.yj20258.top

[T56] Scala：样例类
来源：http://hmj.iojbl.cn

case class User(name: String, age: Int)
来源：http://lxb.jyoumei.cn

[T57] Scala：模式匹配
来源：http://pyp.aizwys.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jxd.52xcode.cn

[T58] Scala：函数定义
来源：http://bjx.ivvv.top

def add(a: Int, b: Int): Int = a + b
来源：http://hca.ppjwa.cn

[T59] Scala：循环
来源：http://npu.cdnleiting.top

for (i <- 1 to 10) println(i)
来源：http://prn.jinghuilouyu.cn

[T60] Scala：折叠
来源：http://zpr.chenzaomai.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eqt.chenjidiqi.icu

================================================================================
来源：http://hwb.fengsongda.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://new.hesvh.cn

================================================================================
来源：http://qfk.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://rwh.epnwcf.com

python -m venv .venv && source .venv/bin/activate
来源：http://zoy.smart0.xyz

[U02] Py：导出 / 安装依赖
来源：http://lxn.jiagoushi.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wka.fehbvm.com

[U03] Py：加载 .env 配置
来源：http://vko.52xcode.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pgq.ydjk.org.cn

[U04] Py：变量调试打印
来源：http://pjs.jinqigfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bmq.quarkkingdee.top

[U05] Py：列表去重且保序
来源：http://tpv.tianlin.xyz

list(dict.fromkeys(arr))
来源：http://kwg.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://tyr.zhiwuduotai.top

{**a, **b}
来源：http://fzd.nwbrower.top

[U07] Py：反转字典键值
来源：http://iaq.chenjidiqi.icu

{v: k for k, v in d.items()}
来源：http://wei.birdmap.top

[U08] Py：展平二维列表
来源：http://obk.hysaishi.cn

[y for x in nested for y in x]
来源：http://edh.iojbl.cn

[U09] Py：字典取最大值的键
来源：http://qfz.yj202588.top

max(d, key=d.get)
来源：http://dat.cucudq.cn

[U10] Py：按值排序字典
来源：http://qjv.ybcxt.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mvs.yuanzhike.top

[U11] Py：生成器表达式
来源：http://odu.cheryme.top

(x * 2 for x in arr)
来源：http://gel.vehdjk.com

[U12] Py：取出现最多的 3 个元素
来源：http://ocm.fzhhl.top

Counter(arr).most_common(3)
来源：http://eep.ehwqpu.com

[U13] Py：固定长度队列
来源：http://vso.yuanzhike.top

deque(maxlen=10)
来源：http://foj.ehwqpu.com

[U14] Py：分组收集到列表
来源：http://iue.haohaochexian.top

defaultdict(list)
来源：http://pvb.jqgufenzy.top

[U15] Py：高精度计时
来源：http://psd.zycfv.cn

t = time.perf_counter()
来源：http://epr.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://niq.aizwys.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://avg.nanxinkj.top

[U17] Py：初始化日志
来源：http://ysq.ivvv.top

logging.basicConfig(level=logging.INFO)
来源：http://lux.hongshengwenyu.top

[U18] Py：预编译正则
来源：http://hgc.fehbvm.com

pat = re.compile(r"\d+")
来源：http://jdy.shangyingyoupin.top

[U19] Py：正则替换带回调
来源：http://dcm.ydjk.org.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lnd.andypj.xyz

[U20] Py：缓存函数结果
来源：http://hwh.yonumen.top

@functools.lru_cache(maxsize=None)
来源：http://vsl.jinghuilouyu.cn

[U21] Py：自定义上下文管理器
来源：http://lpj.smart0.xyz

@contextlib.contextmanager
来源：http://sas.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://xbl.yueranfly.top

list(zip(*m))
来源：http://rsy.jinghuilouyu.cn

[U23] Py：分块读取大文件
来源：http://cmm.ehwqpu.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ohn.zhixingplan.top

[U24] Py：路径操作
来源：http://icg.guowangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wle.chenlongwang.top

[U25] Py：CSV 按字典读
来源：http://que.iojbl.cn

csv.DictReader(f)
来源：http://iyy.ybcxt.top

[U26] Py：并发下载
来源：http://ijo.jiagoushi.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vde.aizwys.cn

[U27] Py：异步 HTTP
来源：http://cxs.jyoumei.cn

aiohttp.ClientSession() 配合 async with
来源：http://cyn.svipenyu.cn

[U28] Py：类型别名
来源：http://gmy.hysaishi.cn

UserId = int
来源：http://wxh.guannengcc.top

[U29] Py：属性校验
来源：http://ynt.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://kdu.xziqi.cn

[U30] Py：数据类
来源：http://yys.hammf.cn

@dataclass(slots=True)
来源：http://spo.yangfankeji.com

[U31] Py：单测
来源：http://ghi.xylfe.cn

python -m pytest -q
来源：http://owx.fehbvm.com

[U32] Py：代码格式化
来源：http://dgv.tianlin.xyz

ruff format . && ruff check --fix .
来源：http://kvd.smart0.xyz

[U33] Py：打包发布
来源：http://zey.fktsv.cn

python -m build  （依赖 pyproject.toml）
来源：http://eww.jyoumei.cn

[U34] Py：判断编码
来源：http://zbx.jinghuilouyu.cn

chardet.detect(raw)
来源：http://lyi.fktsv.cn

[U35] Py：发送邮件
来源：http://obt.tianlin.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://trm.aizwys.cn

[U36] Py：定时任务
来源：http://rlb.fehbvm.com

schedule.every(10).minutes.do(job)
来源：http://qer.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://rqs.svipenyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ogq.guannengcc.top

[U38] Py：获取脚本所在目录
来源：http://jnc.0kj1m.cn

Path(__file__).resolve().parent
来源：http://lvk.tian-w.cn

[U39] Py：判断是否在交互环境
来源：http://xwm.jqgfzy.top

sys.stdout.isatty()
来源：http://xwz.jinghuilouyu.cn

[U40] Py：打印到标准错误
来源：http://zur.yuxming.cn

print("err", file=sys.stderr)
来源：http://lpb.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://xyz.zdbjq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zjm.ctjpmb.com

[U42] PHP：PSR-4 自动加载
来源：http://rlf.guannengcc.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mzj.hammf.cn

[U43] PHP：声明命名空间
来源：http://tzl.vqdsnc.cn

namespace App\Http;
来源：http://nyl.nwbrower.top

[U44] PHP：开启严格类型
来源：http://sjy.ybcxt.top

declare(strict_types=1);
来源：http://sec.zdbjq.cn

[U45] PHP：类型声明与返回类型
来源：http://amw.iojbl.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yaq.zhiwuduotai.top

[U46] PHP：可空类型
来源：http://sjs.daria6918.cn

?string $name = null
来源：http://mcu.nwbrower.top

[U47] PHP：联合类型
来源：http://lwk.nanxinkj.top

int|string $id
来源：http://oeg.fktsv.cn

[U48] PHP：纯枚举
来源：http://bkh.wangdashe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://too.ydjk.org.cn

[U49] PHP：只读属性
来源：http://pso.sweek.top

public readonly string $name
来源：http://cva.fehbvm.com

[U50] PHP：构造器属性提升
来源：http://mli.xziqi.cn

public function __construct(private int $id) {}
来源：http://lyb.jyoumei.cn

[U51] PHP：数组解构
来源：http://smc.chenzaomai.com

[$a, $b] = $arr;
来源：http://wnr.chenjidiqi.icu

[U52] PHP：箭头函数
来源：http://ziq.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://yyh.yj20258.top

[U53] PHP：空合并运算符
来源：http://woa.yangfankeji.com

$v = $a ?? $b ?? "default";
来源：http://pex.jinghuilouyu.cn

[U54] PHP：空安全调用
来源：http://urt.gogol.net.cn

$obj?->method()
来源：http://voq.jqgfzy.top

[U55] PHP：match 表达式
来源：http://wna.hammf.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ljq.ivvv.top

[U56] PHP：命名参数
来源：http://mbl.vehdjk.com

f(a: 1, b: 2)
来源：http://mrh.jianghu66.top


<!-- 参考信息 -->