代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://atn.hfpthk.cn

[S25] C：内存拷贝
来源：http://spq.ybcxt.top

memcpy(dst, src, n);
来源：http://ayo.shuidangran.top

[S26] C：内存清零
来源：http://zbx.fktsv.cn

memset(a, 0, sizeof a);
来源：http://tot.wangdashe.top

[S27] C：定义常量
来源：http://bzj.vqdsnc.cn

const double PI = 3.14159;
来源：http://vlh.shanyushiyangtech.top

[S28] C：静态变量
来源：http://udi.ppjwa.cn

static int counter = 0;
来源：http://voz.cqqwz.cn

[S29] C：变参函数
来源：http://owz.hammf.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ozg.hcnkem.com

[S30] C：头文件保护
来源：http://ynf.xinyue.icu

#ifndef X_H
来源：http://ind.bjfxy.top

#define X_H
来源：http://mvg.fzhhl.top

#endif
来源：http://vhe.sxryk.cn

[S31] C++：Hello World
来源：http://iab.jinghuilouyu.cn

#include <iostream>
来源：http://piz.hywenlv.cn

int main() { std::cout << "Hello\n"; }
来源：http://ssd.nanxuanxn.top

[S32] C++：字符串
来源：http://obp.andypj.xyz

std::string s = "hi";  s += "!";
来源：http://imn.fengsongda.top

[S33] C++：vector 增删
来源：http://mej.ydjk.org.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://law.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://tzv.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://ftg.xingfuxueyuan.xyz

[S35] C++：map
来源：http://kei.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gfi.zhongyouzk.top

[S36] C++：unordered_map
来源：http://tno.daria6918.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://glw.uphjek.com

[S37] C++：set
来源：http://cqo.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://spt.gzhubu.top

[S38] C++：排序
来源：http://idf.shuidangran.top

std::sort(v.begin(), v.end());
来源：http://okf.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://nme.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kiw.nanxinkj.top

[S40] C++：查找元素
来源：http://rpy.zycfv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ewo.redwolf501.top

[S41] C++：类与构造函数
来源：http://zuu.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qtt.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://esn.snrcjt.cn

class B : public Base { public: void f() override {} };
来源：http://rce.ppjwa.cn

[S43] C++：智能指针
来源：http://bda.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://hdm.fktsv.cn

[S44] C++：引用传参
来源：http://kcu.jinqigfzy.top

void inc(int &x) { ++x; }
来源：http://fhv.yvedp.cn

[S45] C++：lambda
来源：http://qmd.sweek.top

auto add = [](int a, int b) { return a + b; };
来源：http://xbs.yangfankeji.com

[S46] C++：函数模板
来源：http://kwa.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mjh.vqdsnc.cn

[S47] C++：结构化绑定遍历
来源：http://qbp.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mqv.ybcxt.top

[S48] C++：逐行读文件
来源：http://aak.gaohongyu789.top

std::ifstream in("a.txt");  std::string line;
来源：http://gko.yongpay.top

while (std::getline(in, line)) { }
来源：http://pwv.andypj.xyz

[S49] C++：写文件
来源：http://thd.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ljm.jinqigufen.top

[S50] C++：格式化数字
来源：http://olw.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mxf.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://sqd.daxiang520.top

static_cast<double>(a) / b
来源：http://smo.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://olj.vqdsnc.cn

int size() const noexcept { return n_; }
来源：http://dti.nanxinkj.top

[S53] C++：移动语义
来源：http://sxv.xylfe.cn

std::vector<int> w = std::move(v);
来源：http://zmr.mhx1999.top

[S54] C++：异常处理
来源：http://yhb.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dgw.tanke756.top

[S55] C++：结构化绑定
来源：http://iba.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://adf.svipenyu.cn

[S56] C++：optional
来源：http://vov.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dwz.zhixingplan.top

[S57] C++：编译期常量
来源：http://abj.zdbjq.cn

constexpr int N = 10;
来源：http://qdb.guowangkeji.top

[S58] C++：命名空间
来源：http://nuq.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://ayy.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://bum.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://htr.gaohongyu789.top

[S60] C++：遍历并删除元素
来源：http://pvr.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://asz.sufxvd.cn

================================================================================
来源：http://uza.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://efg.fktsv.cn

================================================================================
来源：http://fqp.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://iwe.snrcjt.cn

println("Hello")
来源：http://swc.vehdjk.com

[T02] Kotlin：变量
来源：http://zqi.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xoz.shanyushiyangkeji.top

[T03] Kotlin：字符串模板
来源：http://bxv.hnqzz.top

"值: $b"
来源：http://bsk.cashguo.top

[T04] Kotlin：空安全
来源：http://dmz.aizwys.cn

val n: String? = null;  n?.length
来源：http://mss.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://wlm.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kzd.fktsv.cn

[T06] Kotlin：集合映射
来源：http://hin.ivvv.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gvr.zdqjudy.top

[T07] Kotlin：集合过滤
来源：http://oip.jyoumei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hcd.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://jus.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://ien.zhengqikj.top

[T09] Kotlin：扩展函数
来源：http://nqj.yongpay.top

fun String.exclaim() = this + "!"
来源：http://pxu.nwbrower.top

[T10] Kotlin：默认参数
来源：http://yog.dashuyun.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kjd.bbcook.cn

[T11] Kotlin：协程
来源：http://qve.tian-w.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://imx.fktsv.cn

[T12] Kotlin：解构声明
来源：http://edf.yanxiufei.cn

val (a, b) = Pair(1, 2)
来源：http://ndh.shanyushiyangkeji.top

[T13] Kotlin：只读 Map
来源：http://uxa.hywenlv.cn

val m = mapOf("a" to 1)
来源：http://jqx.zhixingplan.top

[T14] Kotlin：循环
来源：http://slx.havefunace.top

for (i in 1..10) println(i)
来源：http://git.yj202588.top

[T15] Kotlin：接口
来源：http://vfr.meibo888.top

interface Shape { fun area(): Double }
来源：http://diz.sjlbkw.cn

[T16] Swift：Hello World
来源：http://qab.zdbjq.cn

print("Hello")
来源：http://kzj.chenjidiqi.icu

[T17] Swift：变量与常量
来源：http://duh.wangdashe.top

var a = 1;  let b = 2
来源：http://wnl.hongshengwenyu.top

[T18] Swift：字符串插值
来源：http://erp.cheryme.top

"值: \(b)"
来源：http://htu.xylfe.cn

[T19] Swift：可选绑定
来源：http://mdl.shzxlz.cn

if let n = opt { print(n) }
来源：http://rfs.jyoumei.cn

[T20] Swift：数组操作
来源：http://djz.ybcxt.top

var a = [1, 2, 3];  a.append(4)
来源：http://wqx.wangdashe.top

[T21] Swift：遍历
来源：http://uyd.havefunace.top

for x in a { print(x) }
来源：http://mpj.hesvh.cn

[T22] Swift：字典
来源：http://she.meibo888.top

var d = ["a": 1];  d["b"] = 2
来源：http://fgq.zhiwuduotai.top

[T23] Swift：函数
来源：http://enu.zhiwuduotai.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uom.yvedp.cn

[T24] Swift：闭包
来源：http://cqx.yj20258.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zyx.ybcxt.top

[T25] Swift：结构体
来源：http://ydd.guowangkeji.top

struct P { var x: Int }
来源：http://rrr.nwbrower.top

[T26] Swift：类与重写
来源：http://ufb.meibo888.top

class A: Base { override func f() {} }
来源：http://iga.hongshengwenyu.top

[T27] Swift：错误处理
来源：http://qqs.hysaishi.cn

do { try f() } catch { print(error) }
来源：http://uxg.hnxiangtu.top

[T28] Swift：枚举
来源：http://uln.feifeiyinyue.top

enum Color { case red, green }
来源：http://kcg.xylfe.cn

[T29] Swift：guard 提前返回
来源：http://njk.shzxlz.cn

guard let x = opt else { return }
来源：http://tip.shanyushiyangkeji.top

[T30] Swift：协议
来源：http://lgw.ivvv.top

protocol Shape { func area() -> Double }
来源：http://zfr.xziqi.cn

[T31] Lua：Hello World
来源：http://jen.zhaomingkeji.xyz

print("Hello")
来源：http://qak.sjlbkw.cn

[T32] Lua：局部变量
来源：http://yyv.haohaochexian.top

local a = 1
来源：http://bor.mhx1999.top

[T33] Lua：表（数组）
来源：http://wss.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ari.fktsv.cn

[T34] Lua：遍历表
来源：http://sgb.ivvv.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cbz.shuidangran.top

[T35] Lua：字典表
来源：http://tgl.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://ycd.tianlin.xyz

[T36] Lua：函数
来源：http://dqc.yueranfly.top

function add(a, b) return a + b end
来源：http://dqt.xziqi.cn

[T37] Lua：字符串拼接
来源：http://sdx.andypj.xyz

"a" .. "b"
来源：http://hnd.smart0.xyz

[T38] Lua：条件
来源：http://ruz.bbcook.cn

if x > 0 then print("正") end
来源：http://ayw.aibaodan.cn

[T39] Lua：模式匹配
来源：http://ejx.svipenyu.cn

string.find(s, "%d+")
来源：http://gos.daria6918.cn

[T40] Lua：元表
来源：http://zpk.havefunace.top

setmetatable({}, { __index = base })
来源：http://koa.zycfv.cn

[T41] Perl：Hello World
来源：http://hcm.tian-w.cn

print "Hello\n";
来源：http://bpa.svipenyu.cn

[T42] Perl：变量类型
来源：http://ejy.sufxvd.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fpp.zhijiandao.cn

[T43] Perl：字符串插值
来源：http://oae.shuidangran.top

"值: $a"
来源：http://ndw.jqgfzy.top

[T44] Perl：条件
来源：http://kig.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://ske.ywan-chungtsiang.top

[T45] Perl：数组遍历
来源：http://ymm.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://vdd.chenjidiqi.icu

[T46] Perl：哈希操作
来源：http://qtq.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fnr.hfpthk.cn

[T47] Perl：正则捕获
来源：http://bps.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nlu.iojbl.cn

[T48] Perl：正则替换
来源：http://bsr.jinghuilouyu.cn

$s =~ s/old/new/g;
来源：http://tmn.yongpay.top

[T49] Perl：函数
来源：http://jqc.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://icj.aizwys.cn

[T50] Perl：逐行读文件
来源：http://gbv.ywan-chungtsiang.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yul.xingfuxueyuan.xyz

while (my $line = <$fh>) { print $line; }
来源：http://xdm.yangfankeji.com

[T51] Scala：Hello World
来源：http://fld.jlsjyb.cn

println("Hello")
来源：http://tas.tanke756.top

[T52] Scala：变量
来源：http://yqb.chenjidiqi.icu

val a = 1;  var b = 2
来源：http://pio.chenlongwang.top

[T53] Scala：字符串插值
来源：http://iuy.jinqigfzy.top

s"值: $b"
来源：http://dlb.quarkkingdee.top

[T54] Scala：集合映射
来源：http://gpe.xziqi.cn

List(1, 2, 3).map(_ * 2)
来源：http://own.cucudq.cn

[T55] Scala：集合过滤
来源：http://ave.zhixingplan.top

List(1, 2, 3).filter(_ > 1)
来源：http://ldt.ctjpmb.com

[T56] Scala：样例类
来源：http://eyf.feifeiyinyue.top

case class User(name: String, age: Int)
来源：http://ygz.hfpthk.cn

[T57] Scala：模式匹配
来源：http://xxx.jlsjyb.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zxi.fengsongda.top

[T58] Scala：函数定义
来源：http://spe.fktsv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qvp.jianghu66.top

[T59] Scala：循环
来源：http://xnd.yuanzhike.top

for (i <- 1 to 10) println(i)
来源：http://xlt.zhongyouzk.top

[T60] Scala：折叠
来源：http://nva.nanxuanxn.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wdp.0kj1m.cn

================================================================================
来源：http://cdp.meibo888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fwa.yongpay.top

================================================================================
来源：http://ewq.yj20258.top

[U01] Py：创建虚拟环境
来源：http://uyh.jinqigufen.top

python -m venv .venv && source .venv/bin/activate
来源：http://urc.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://ypr.cqqwz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ttx.quarkkingdee.top

[U03] Py：加载 .env 配置
来源：http://oty.svipenyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iyq.snrcjt.cn

[U04] Py：变量调试打印
来源：http://lfx.yvedp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ajw.yuxming.cn

[U05] Py：列表去重且保序
来源：http://lwx.nanxinkj.top

list(dict.fromkeys(arr))
来源：http://jsr.sufxvd.cn

[U06] Py：合并两个字典
来源：http://xsb.haohaochexian.top

{**a, **b}
来源：http://hrc.xylfe.cn

[U07] Py：反转字典键值
来源：http://fob.hnxiangtu.top

{v: k for k, v in d.items()}
来源：http://jht.hammf.cn

[U08] Py：展平二维列表
来源：http://fjo.ppjwa.cn

[y for x in nested for y in x]
来源：http://unm.sjlbkw.cn

[U09] Py：字典取最大值的键
来源：http://idi.yj20258888.top

max(d, key=d.get)
来源：http://czb.vqdsnc.cn

[U10] Py：按值排序字典
来源：http://wcl.zhiwuduotai.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fol.chenlongwang.top

[U11] Py：生成器表达式
来源：http://rye.zhijiandao.cn

(x * 2 for x in arr)
来源：http://grv.jiagoushi.top

[U12] Py：取出现最多的 3 个元素
来源：http://mbk.jianghu66.top

Counter(arr).most_common(3)
来源：http://fnr.ehwqpu.com

[U13] Py：固定长度队列
来源：http://qxg.yongpay.top

deque(maxlen=10)
来源：http://aeq.zhengqikj.top

[U14] Py：分组收集到列表
来源：http://pvg.havefunace.top

defaultdict(list)
来源：http://ogt.xziqi.cn

[U15] Py：高精度计时
来源：http://pgh.yueranfly.top

t = time.perf_counter()
来源：http://fgw.xinyue.icu

[U16] Py：命令行参数解析
来源：http://gsw.yanxiufei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rfe.kuanghao11.cn

[U17] Py：初始化日志
来源：http://gzr.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://vwn.xylfe.cn

[U18] Py：预编译正则
来源：http://axc.shanyushiyangkeji.top

pat = re.compile(r"\d+")
来源：http://zgz.hesvh.cn

[U19] Py：正则替换带回调
来源：http://cje.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tra.gotoacloud.top

[U20] Py：缓存函数结果
来源：http://see.shuidangran.top

@functools.lru_cache(maxsize=None)
来源：http://nsx.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://zjk.pycfn.com

@contextlib.contextmanager
来源：http://lat.chenlongwang.top

[U22] Py：矩阵转置
来源：http://zhx.cqqwz.cn

list(zip(*m))
来源：http://ipx.hfpthk.cn

[U23] Py：分块读取大文件
来源：http://raj.jinqigfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xzo.jqgufenzy.top

[U24] Py：路径操作
来源：http://ycf.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xpj.wangdashe.top

[U25] Py：CSV 按字典读
来源：http://yhc.redwolf501.top

csv.DictReader(f)
来源：http://rfw.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://sjr.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wsq.sxryk.cn

[U27] Py：异步 HTTP
来源：http://zew.sysykeji.top

aiohttp.ClientSession() 配合 async with
来源：http://huw.ydzc1.top

[U28] Py：类型别名
来源：http://vyt.meibo888.top

UserId = int
来源：http://hwi.sysykeji.top

[U29] Py：属性校验
来源：http://ngh.pengpengdd.cyou

@property 与 @x.setter 配合
来源：http://tsx.fengsongda.top

[U30] Py：数据类
来源：http://zxp.mhx1999.top

@dataclass(slots=True)
来源：http://mqc.zhongyouzk.top

[U31] Py：单测
来源：http://rgr.xuetiantiany.cn

python -m pytest -q
来源：http://pyq.feifeiyinyue.top

[U32] Py：代码格式化
来源：http://cyu.havefunace.top

ruff format . && ruff check --fix .
来源：http://hvo.jinqigufen.top

[U33] Py：打包发布
来源：http://fsi.hysaishi.cn

python -m build  （依赖 pyproject.toml）
来源：http://mei.xziqi.cn

[U34] Py：判断编码
来源：http://mnc.gzhubu.top

chardet.detect(raw)
来源：http://wmt.sjlbkw.cn

[U35] Py：发送邮件
来源：http://hnq.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://szh.jinghuilouyu.cn

[U36] Py：定时任务
来源：http://sge.birdmap.top

schedule.every(10).minutes.do(job)
来源：http://elt.jqgfzy.top

[U37] Py：读写 Excel
来源：http://bmy.jinqigfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://sfi.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://ins.jqgfzy.top

Path(__file__).resolve().parent
来源：http://qeq.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://uxt.tianlin.xyz

sys.stdout.isatty()
来源：http://xwf.yuanzhike.top

[U40] Py：打印到标准错误
来源：http://dbn.dianchejie.cn

print("err", file=sys.stderr)
来源：http://dba.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://but.gaohongyu789.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ntr.sweek.top

[U42] PHP：PSR-4 自动加载
来源：http://ald.hnqzz.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://siz.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://oli.feifeiyinyue.top

namespace App\Http;
来源：http://ekv.tanke756.top

[U44] PHP：开启严格类型
来源：http://rdk.epnwcf.com

declare(strict_types=1);
来源：http://ope.wangdashe.top

[U45] PHP：类型声明与返回类型
来源：http://sxh.feifeiyinyue.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jgk.shzxlz.cn

[U46] PHP：可空类型
来源：http://szn.hywenlv.cn

?string $name = null
来源：http://wdn.redwolf501.top

[U47] PHP：联合类型
来源：http://gek.nanxuanxn.top

int|string $id
来源：http://xok.shuidangran.top

[U48] PHP：纯枚举
来源：http://veq.dashuyun.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xln.yanxiufei.cn


<!-- 参考信息 -->