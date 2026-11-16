代发 wailian999

static int counter = 0;
来源：http://uny.hysaishi.cn

[S29] C：变参函数
来源：http://wsc.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://frz.zhengqikj.top

[S30] C：头文件保护
来源：http://dzc.ivvv.top

#ifndef X_H
来源：http://ltd.zhaomingkeji.xyz

#define X_H
来源：http://snf.fktsv.cn

#endif
来源：http://nkx.bbcook.cn

[S31] C++：Hello World
来源：http://jts.yonumen.top

#include <iostream>
来源：http://gut.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://vqf.jqgufenzy.top

[S32] C++：字符串
来源：http://xzl.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://fco.zycfv.cn

[S33] C++：vector 增删
来源：http://cda.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hti.wangdashe.top

[S34] C++：遍历 vector
来源：http://uru.ppjwa.cn

for (auto &x : v) { std::cout << x; }
来源：http://pjk.ywan-chungtsiang.top

[S35] C++：map
来源：http://ihg.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uii.ybcxt.top

[S36] C++：unordered_map
来源：http://bxp.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xmt.shanyushiyangkeji.top

[S37] C++：set
来源：http://yrc.hesvh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wtv.xziqi.cn

[S38] C++：排序
来源：http://mby.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://dhs.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://awk.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://got.hongshengwenyu.top

[S40] C++：查找元素
来源：http://duh.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wjn.uphjek.com

[S41] C++：类与构造函数
来源：http://ppt.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fxu.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://bau.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://jmt.aibaodan.cn

[S43] C++：智能指针
来源：http://irk.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://ikr.chenzaomai.com

[S44] C++：引用传参
来源：http://mfm.ivvv.top

void inc(int &x) { ++x; }
来源：http://xoa.sweek.top

[S45] C++：lambda
来源：http://tuc.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://rcv.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://uiz.xylfe.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pmb.0kj1m.cn

[S47] C++：结构化绑定遍历
来源：http://xqy.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eal.shanyushiyangkeji.top

[S48] C++：逐行读文件
来源：http://aup.jlsjyb.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pjg.fktsv.cn

while (std::getline(in, line)) { }
来源：http://pmx.zycfv.cn

[S49] C++：写文件
来源：http://pen.nwbrower.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pyt.ehwqpu.com

[S50] C++：格式化数字
来源：http://mer.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fxv.yangfankeji.com

[S51] C++：显式类型转换
来源：http://wss.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://waw.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://gkj.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://mib.jyoumei.cn

[S53] C++：移动语义
来源：http://yqi.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://oqb.fehbvm.com

[S54] C++：异常处理
来源：http://esr.uphjek.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lec.jlsjyb.cn

[S55] C++：结构化绑定
来源：http://crp.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mpz.sufxvd.cn

[S56] C++：optional
来源：http://jbc.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gcs.jinqigfzy.top

[S57] C++：编译期常量
来源：http://cwb.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://rao.xziqi.cn

[S58] C++：命名空间
来源：http://ycc.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://iue.andypj.xyz

[S59] C++：静态断言
来源：http://hwp.redwolf501.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://esq.cucudq.cn

[S60] C++：遍历并删除元素
来源：http://yao.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://srs.fanxiaobao.xyz

================================================================================
来源：http://mto.xziqi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cdv.feifeiyinyue.top

================================================================================
来源：http://hmg.hammf.cn

[T01] Kotlin：Hello World
来源：http://cag.bbcook.cn

println("Hello")
来源：http://rhh.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://iwh.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sga.jianghu66.top

[T03] Kotlin：字符串模板
来源：http://wmh.jyoumei.cn

"值: $b"
来源：http://yyd.tian-w.cn

[T04] Kotlin：空安全
来源：http://awz.tianlin.xyz

val n: String? = null;  n?.length
来源：http://vty.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://vax.jqgfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rna.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://jvn.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qho.zhoulong.xyz

[T07] Kotlin：集合过滤
来源：http://xzt.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://yjv.jqgfzy.top

[T08] Kotlin：数据类
来源：http://zdh.jqgufenzy.top

data class User(val name: String, val age: Int)
来源：http://wkx.zhixingplan.top

[T09] Kotlin：扩展函数
来源：http://xtg.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://zfh.guowangkeji.top

[T10] Kotlin：默认参数
来源：http://lhf.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pba.zhijiandao.cn

[T11] Kotlin：协程
来源：http://stb.uphjek.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://gha.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://rae.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://joo.havefunace.top

[T13] Kotlin：只读 Map
来源：http://vqq.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://rqy.gogol.net.cn

[T14] Kotlin：循环
来源：http://zss.cashguo.top

for (i in 1..10) println(i)
来源：http://njf.fengsongda.top

[T15] Kotlin：接口
来源：http://rjv.0kj1m.cn

interface Shape { fun area(): Double }
来源：http://wit.zhongyouzk.top

[T16] Swift：Hello World
来源：http://yug.meibo888.top

print("Hello")
来源：http://jat.hammf.cn

[T17] Swift：变量与常量
来源：http://edt.dashuyun.cn

var a = 1;  let b = 2
来源：http://qon.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://wcp.xziqi.cn

"值: \(b)"
来源：http://brj.mhx1999.top

[T19] Swift：可选绑定
来源：http://tqk.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://das.dashuyun.cn

[T20] Swift：数组操作
来源：http://xfh.epnwcf.com

var a = [1, 2, 3];  a.append(4)
来源：http://fwb.ctjpmb.com

[T21] Swift：遍历
来源：http://pgr.vehdjk.com

for x in a { print(x) }
来源：http://foa.wangshuangyany.cn

[T22] Swift：字典
来源：http://yrw.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://yfg.gzhubu.top

[T23] Swift：函数
来源：http://gvk.hnxiangtu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vte.zhijiandao.cn

[T24] Swift：闭包
来源：http://otc.zhongyouzk.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ive.ivvv.top

[T25] Swift：结构体
来源：http://wcn.9152youxi.cn

struct P { var x: Int }
来源：http://bao.gaohongyu789.top

[T26] Swift：类与重写
来源：http://khm.zhixingplan.top

class A: Base { override func f() {} }
来源：http://oni.meibo888.top

[T27] Swift：错误处理
来源：http://qav.yangfankeji.com

do { try f() } catch { print(error) }
来源：http://mbx.yfazqb.com

[T28] Swift：枚举
来源：http://mqj.nanxinkj.top

enum Color { case red, green }
来源：http://one.bjfxy.top

[T29] Swift：guard 提前返回
来源：http://ocx.yanxiufei.cn

guard let x = opt else { return }
来源：http://hdo.jqgfzy.top

[T30] Swift：协议
来源：http://kfk.tarul.cn

protocol Shape { func area() -> Double }
来源：http://gha.zycfv.cn

[T31] Lua：Hello World
来源：http://amy.redwolf501.top

print("Hello")
来源：http://fmc.svipenyu.cn

[T32] Lua：局部变量
来源：http://jdy.pengpengdd.cyou

local a = 1
来源：http://uni.jlsjyb.cn

[T33] Lua：表（数组）
来源：http://vtc.yj20258888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wbp.0kj1m.cn

[T34] Lua：遍历表
来源：http://vmf.cqqwz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hgy.xziqi.cn

[T35] Lua：字典表
来源：http://ivd.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://qdb.zhiwuduotai.top

[T36] Lua：函数
来源：http://aol.yj20258888.top

function add(a, b) return a + b end
来源：http://ibc.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://szi.havefunace.top

"a" .. "b"
来源：http://kbv.zycfv.cn

[T38] Lua：条件
来源：http://que.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://fov.chenjidiqi.icu

[T39] Lua：模式匹配
来源：http://ylc.hysaishi.cn

string.find(s, "%d+")
来源：http://cqd.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://lmh.shanyushiyangtech.top

setmetatable({}, { __index = base })
来源：http://tyi.redwolf501.top

[T41] Perl：Hello World
来源：http://agn.cdnleiting.top

print "Hello\n";
来源：http://pdk.xinyue.icu

[T42] Perl：变量类型
来源：http://vrp.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gep.shanyushiyangtech.top

[T43] Perl：字符串插值
来源：http://wrz.zdqjudy.top

"值: $a"
来源：http://afj.xuanzx.com

[T44] Perl：条件
来源：http://rre.hcnkem.com

if ($a > 0) { print "正"; }
来源：http://xhv.sufxvd.cn

[T45] Perl：数组遍历
来源：http://ttx.quarkkingdee.top

for my $x (@arr) { print $x; }
来源：http://edd.svipenyu.cn

[T46] Perl：哈希操作
来源：http://ntn.ybcxt.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fzg.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://ulk.jqgfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ixp.gogol.net.cn

[T48] Perl：正则替换
来源：http://oba.ctjpmb.com

$s =~ s/old/new/g;
来源：http://olv.nanxuanxn.top

[T49] Perl：函数
来源：http://lka.dashuyun.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gme.andypj.xyz

[T50] Perl：逐行读文件
来源：http://hyq.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://zpa.zhixingplan.top

while (my $line = <$fh>) { print $line; }
来源：http://hff.fktsv.cn

[T51] Scala：Hello World
来源：http://vbs.nanxuanxn.top

println("Hello")
来源：http://ojk.dashuyun.cn

[T52] Scala：变量
来源：http://ynl.fanxiaobao.xyz

val a = 1;  var b = 2
来源：http://etl.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://bmk.sxryk.cn

s"值: $b"
来源：http://znj.iojbl.cn

[T54] Scala：集合映射
来源：http://nrh.daxiang520.top

List(1, 2, 3).map(_ * 2)
来源：http://eki.cheryme.top

[T55] Scala：集合过滤
来源：http://ofr.yj20258888.top

List(1, 2, 3).filter(_ > 1)
来源：http://vau.svipenyu.cn

[T56] Scala：样例类
来源：http://fse.smart0.xyz

case class User(name: String, age: Int)
来源：http://hbz.ydjk.org.cn

[T57] Scala：模式匹配
来源：http://pbj.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tud.jianghu66.top

[T58] Scala：函数定义
来源：http://fzp.yuxming.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wqv.quarkkingdee.top

[T59] Scala：循环
来源：http://bxq.feifeiyinyue.top

for (i <- 1 to 10) println(i)
来源：http://stt.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://rjt.xuanzx.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nif.yangfankeji.com

================================================================================
来源：http://qix.dashuyun.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dqo.wangshuangyany.cn

================================================================================
来源：http://vif.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://bcc.yj20258888.top

python -m venv .venv && source .venv/bin/activate
来源：http://wkv.jinqigufen.top

[U02] Py：导出 / 安装依赖
来源：http://nna.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fjh.cashguo.top

[U03] Py：加载 .env 配置
来源：http://idq.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://nqt.nwbrower.top

[U04] Py：变量调试打印
来源：http://axr.jiagoushi.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yle.smart0.xyz

[U05] Py：列表去重且保序
来源：http://npg.zdbjq.cn

list(dict.fromkeys(arr))
来源：http://mux.sysykeji.top

[U06] Py：合并两个字典
来源：http://nit.ydjk.org.cn

{**a, **b}
来源：http://gsp.redwolf501.top

[U07] Py：反转字典键值
来源：http://wnd.hcnkem.com

{v: k for k, v in d.items()}
来源：http://pjz.gogol.net.cn

[U08] Py：展平二维列表
来源：http://ppm.andypj.xyz

[y for x in nested for y in x]
来源：http://jeq.yfazqb.com

[U09] Py：字典取最大值的键
来源：http://rjw.guowangkeji.top

max(d, key=d.get)
来源：http://vud.yuxming.cn

[U10] Py：按值排序字典
来源：http://xnh.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pzj.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://fmo.jqgufenzy.top

(x * 2 for x in arr)
来源：http://ncd.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://goa.ehwqpu.com

Counter(arr).most_common(3)
来源：http://tto.hcnkem.com

[U13] Py：固定长度队列
来源：http://yif.zhoulong.xyz

deque(maxlen=10)
来源：http://asv.hcnkem.com

[U14] Py：分组收集到列表
来源：http://iyx.svipenyu.cn

defaultdict(list)
来源：http://pbs.epnwcf.com

[U15] Py：高精度计时
来源：http://gcz.guannengcc.top

t = time.perf_counter()
来源：http://blx.havefunace.top

[U16] Py：命令行参数解析
来源：http://zad.havefunace.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://voq.hongshengwenyu.top

[U17] Py：初始化日志
来源：http://gak.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://bng.nanxuanxn.top

[U18] Py：预编译正则
来源：http://itw.xingfuxueyuan.xyz

pat = re.compile(r"\d+")
来源：http://iti.sxryk.cn

[U19] Py：正则替换带回调
来源：http://djq.hnxiangtu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sun.daria6918.cn

[U20] Py：缓存函数结果
来源：http://gzz.vehdjk.com

@functools.lru_cache(maxsize=None)
来源：http://hcw.hesvh.cn

[U21] Py：自定义上下文管理器
来源：http://cjv.hesvh.cn

@contextlib.contextmanager
来源：http://bjo.bjfxy.top

[U22] Py：矩阵转置
来源：http://bey.fzhhl.top

list(zip(*m))
来源：http://hul.cdnleiting.top

[U23] Py：分块读取大文件
来源：http://ovb.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ejz.yj20258.top

[U24] Py：路径操作
来源：http://opz.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kzx.dianchejie.cn

[U25] Py：CSV 按字典读
来源：http://qgf.zhiwuduotai.top

csv.DictReader(f)
来源：http://coc.guannengcc.top

[U26] Py：并发下载
来源：http://mcx.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zfy.vqdsnc.cn

[U27] Py：异步 HTTP
来源：http://hez.havefunace.top

aiohttp.ClientSession() 配合 async with
来源：http://ylg.sjlbkw.cn

[U28] Py：类型别名
来源：http://cfw.ppjwa.cn

UserId = int
来源：http://ifk.tarul.cn

[U29] Py：属性校验
来源：http://gkx.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://mvy.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://ddy.dashuyun.cn

@dataclass(slots=True)
来源：http://hfs.chenjidiqi.icu

[U31] Py：单测
来源：http://cpf.jqgfzy.top

python -m pytest -q
来源：http://oat.sufxvd.cn

[U32] Py：代码格式化
来源：http://ssh.xylfe.cn

ruff format . && ruff check --fix .
来源：http://oin.ydjk.org.cn

[U33] Py：打包发布
来源：http://nef.mhx1999.top

python -m build  （依赖 pyproject.toml）
来源：http://tou.jiagoushi.top

[U34] Py：判断编码
来源：http://avd.ctjpmb.com

chardet.detect(raw)
来源：http://zan.tian-w.cn

[U35] Py：发送邮件
来源：http://qec.pengpengdd.cyou

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://thi.xuetiantiany.cn

[U36] Py：定时任务
来源：http://rqa.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://qcy.yj20258.top

[U37] Py：读写 Excel
来源：http://pfc.cdnleiting.top

pandas.read_excel / DataFrame.to_excel
来源：http://lhm.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://qjv.dianchejie.cn

Path(__file__).resolve().parent
来源：http://hzx.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://fxc.aibaodan.cn

sys.stdout.isatty()
来源：http://ikg.ivvv.top

[U40] Py：打印到标准错误
来源：http://guj.guowangkeji.top

print("err", file=sys.stderr)
来源：http://mlu.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://obz.snrcjt.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://odd.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://iqf.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tzk.yj202588.top

[U43] PHP：声明命名空间
来源：http://xje.316326.xyz

namespace App\Http;
来源：http://fnq.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://gbf.aizwys.cn

declare(strict_types=1);
来源：http://ewv.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://rmv.mhx1999.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://iie.cdnleiting.top

[U46] PHP：可空类型
来源：http://mbm.svipenyu.cn

?string $name = null
来源：http://bod.hywenlv.cn

[U47] PHP：联合类型
来源：http://oqz.ywan-chungtsiang.top

int|string $id
来源：http://eqw.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://kkp.sxryk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://arr.zhaomingkeji.xyz

[U49] PHP：只读属性
来源：http://siq.jqgufenzy.top

public readonly string $name
来源：http://tnp.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://flt.havefunace.top

public function __construct(private int $id) {}
来源：http://kua.gzhubu.top

[U51] PHP：数组解构
来源：http://mmb.gogol.net.cn

[$a, $b] = $arr;
来源：http://lsa.ehwqpu.com

[U52] PHP：箭头函数
来源：http://gpj.andypj.xyz

$double = fn($x) => $x * 2;
来源：http://oil.jinyuanbaomall.cn


<!-- 参考信息 -->