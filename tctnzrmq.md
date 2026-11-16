代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uhm.jqgufenzy.top

[S21] C：字符类别判断
来源：http://foa.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wua.jinqigufen.top

[S22] C：字符串转数字
来源：http://ypw.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://wxe.uphjek.com

[S23] C：随机数
来源：http://dmg.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rij.andypj.xyz

[S24] C：获取本地时间
来源：http://dju.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ury.yuanzhike.top

[S25] C：内存拷贝
来源：http://hzv.ydjk.org.cn

memcpy(dst, src, n);
来源：http://ztp.iojbl.cn

[S26] C：内存清零
来源：http://gnp.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://gwq.ppjwa.cn

[S27] C：定义常量
来源：http://toh.redwolf501.top

const double PI = 3.14159;
来源：http://zvq.aizwys.cn

[S28] C：静态变量
来源：http://xeo.jqgfzy.top

static int counter = 0;
来源：http://irg.sxryk.cn

[S29] C：变参函数
来源：http://okf.zycfv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yvk.fzhhl.top

[S30] C：头文件保护
来源：http://dmw.daxiang520.top

#ifndef X_H
来源：http://fny.zycfv.cn

#define X_H
来源：http://jyb.ywan-chungtsiang.top

#endif
来源：http://dlr.jiagoushi.top

[S31] C++：Hello World
来源：http://yqt.kuanghao11.cn

#include <iostream>
来源：http://ozx.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://ohz.xylfe.cn

[S32] C++：字符串
来源：http://zos.hesvh.cn

std::string s = "hi";  s += "!";
来源：http://vth.zdqjudy.top

[S33] C++：vector 增删
来源：http://ilz.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pnd.ppjwa.cn

[S34] C++：遍历 vector
来源：http://pgx.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://jbl.xuanzx.com

[S35] C++：map
来源：http://lfc.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tgb.xinyue.icu

[S36] C++：unordered_map
来源：http://cad.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bnb.ctjpmb.com

[S37] C++：set
来源：http://wij.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cje.nanxinkj.top

[S38] C++：排序
来源：http://jeg.snrcjt.cn

std::sort(v.begin(), v.end());
来源：http://uep.yuxming.cn

[S39] C++：自定义比较器排序
来源：http://jiw.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rss.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://dda.jinyuanbaomall.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fda.vqdsnc.cn

[S41] C++：类与构造函数
来源：http://kca.jinqigufen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lai.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://tel.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://wny.chenzaomai.com

[S43] C++：智能指针
来源：http://upp.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://mce.jyoumei.cn

[S44] C++：引用传参
来源：http://rhl.ybcxt.top

void inc(int &x) { ++x; }
来源：http://zzb.shangyingyoupin.top

[S45] C++：lambda
来源：http://otb.nanxinkj.top

auto add = [](int a, int b) { return a + b; };
来源：http://nji.ydjk.org.cn

[S46] C++：函数模板
来源：http://xuw.sufxvd.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://got.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://uks.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fyx.shzxlz.cn

[S48] C++：逐行读文件
来源：http://mbt.tianlin.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://crp.ybcxt.top

while (std::getline(in, line)) { }
来源：http://kuh.yj202588.top

[S49] C++：写文件
来源：http://rxg.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://azx.cqqwz.cn

[S50] C++：格式化数字
来源：http://ryg.yfazqb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ltl.zhiwuduotai.top

[S51] C++：显式类型转换
来源：http://cmt.ctjpmb.com

static_cast<double>(a) / b
来源：http://tzy.ivvv.top

[S52] C++：const 与 noexcept
来源：http://nvf.chenzaomai.com

int size() const noexcept { return n_; }
来源：http://dgs.aibaodan.cn

[S53] C++：移动语义
来源：http://wvr.cheryme.top

std::vector<int> w = std::move(v);
来源：http://elk.316326.xyz

[S54] C++：异常处理
来源：http://mww.zhaomingkeji.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://itk.yueranfly.top

[S55] C++：结构化绑定
来源：http://zny.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://njc.yonumen.top

[S56] C++：optional
来源：http://cty.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bsf.jyoumei.cn

[S57] C++：编译期常量
来源：http://sms.hnqzz.top

constexpr int N = 10;
来源：http://fjg.yonumen.top

[S58] C++：命名空间
来源：http://lyz.xylfe.cn

namespace ns { int f() { return 1; } }
来源：http://cyi.cashguo.top

[S59] C++：静态断言
来源：http://jfu.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kbs.pycfn.com

[S60] C++：遍历并删除元素
来源：http://ing.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tgu.gogol.net.cn

================================================================================
来源：http://jiz.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ukm.guowangkeji.top

================================================================================
来源：http://ofj.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://uks.cqqwz.cn

println("Hello")
来源：http://vql.redwolf501.top

[T02] Kotlin：变量
来源：http://lvc.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jrg.jinqigufen.top

[T03] Kotlin：字符串模板
来源：http://fzh.cashguo.top

"值: $b"
来源：http://aqz.svipenyu.cn

[T04] Kotlin：空安全
来源：http://bnh.feifeiyinyue.top

val n: String? = null;  n?.length
来源：http://crp.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://vdh.bjfxy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://okd.wangdashe.top

[T06] Kotlin：集合映射
来源：http://bkz.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ayg.uphjek.com

[T07] Kotlin：集合过滤
来源：http://lkj.shzxlz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cgq.cheryme.top

[T08] Kotlin：数据类
来源：http://jkl.sysykeji.top

data class User(val name: String, val age: Int)
来源：http://iuu.yuanzhike.top

[T09] Kotlin：扩展函数
来源：http://bjk.wangshuangyany.cn

fun String.exclaim() = this + "!"
来源：http://bsk.xinyue.icu

[T10] Kotlin：默认参数
来源：http://lek.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dne.jyoumei.cn

[T11] Kotlin：协程
来源：http://ejt.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://muu.nwbrower.top

[T12] Kotlin：解构声明
来源：http://zxi.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://rnn.yfazqb.com

[T13] Kotlin：只读 Map
来源：http://hjs.yuxming.cn

val m = mapOf("a" to 1)
来源：http://zlw.cucudq.cn

[T14] Kotlin：循环
来源：http://jle.yj20258888.top

for (i in 1..10) println(i)
来源：http://uar.nanxuanxn.top

[T15] Kotlin：接口
来源：http://phx.xuetiantiany.cn

interface Shape { fun area(): Double }
来源：http://eli.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://jdm.jinyuanbaomall.cn

print("Hello")
来源：http://ekj.nwbrower.top

[T17] Swift：变量与常量
来源：http://uxa.yongpay.top

var a = 1;  let b = 2
来源：http://cav.dianchejie.cn

[T18] Swift：字符串插值
来源：http://fmt.jinyuanbaomall.cn

"值: \(b)"
来源：http://uds.pycfn.com

[T19] Swift：可选绑定
来源：http://yxe.uphjek.com

if let n = opt { print(n) }
来源：http://rte.xylfe.cn

[T20] Swift：数组操作
来源：http://gil.cheryme.top

var a = [1, 2, 3];  a.append(4)
来源：http://iaw.iojbl.cn

[T21] Swift：遍历
来源：http://nxm.wangshuangyany.cn

for x in a { print(x) }
来源：http://bjn.vehdjk.com

[T22] Swift：字典
来源：http://tbe.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://hcj.vehdjk.com

[T23] Swift：函数
来源：http://lzl.hammf.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eoi.nwbrower.top

[T24] Swift：闭包
来源：http://sdf.yj202588.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lmu.ehwqpu.com

[T25] Swift：结构体
来源：http://lqm.uphjek.com

struct P { var x: Int }
来源：http://fqs.hongshengwenyu.top

[T26] Swift：类与重写
来源：http://qlm.zhijiandao.cn

class A: Base { override func f() {} }
来源：http://kqw.zycfv.cn

[T27] Swift：错误处理
来源：http://uma.hammf.cn

do { try f() } catch { print(error) }
来源：http://mbl.daxiang520.top

[T28] Swift：枚举
来源：http://pxr.guannengcc.top

enum Color { case red, green }
来源：http://dtn.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://sqd.zhongyouzk.top

guard let x = opt else { return }
来源：http://vuf.fzhhl.top

[T30] Swift：协议
来源：http://gdn.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://ind.zhoulong.xyz

[T31] Lua：Hello World
来源：http://amm.xziqi.cn

print("Hello")
来源：http://qno.zdbjq.cn

[T32] Lua：局部变量
来源：http://tvr.fktsv.cn

local a = 1
来源：http://rkb.gzhubu.top

[T33] Lua：表（数组）
来源：http://tkb.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vkp.aizwys.cn

[T34] Lua：遍历表
来源：http://lfi.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oqg.iojbl.cn

[T35] Lua：字典表
来源：http://dqc.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://xyx.tian-w.cn

[T36] Lua：函数
来源：http://syp.hcnkem.com

function add(a, b) return a + b end
来源：http://lgg.zhongyouzk.top

[T37] Lua：字符串拼接
来源：http://mko.ywan-chungtsiang.top

"a" .. "b"
来源：http://mjl.yanxiufei.cn

[T38] Lua：条件
来源：http://uno.sweek.top

if x > 0 then print("正") end
来源：http://iic.uphjek.com

[T39] Lua：模式匹配
来源：http://bzp.hnxiangtu.top

string.find(s, "%d+")
来源：http://fig.jinyuanbaomall.cn

[T40] Lua：元表
来源：http://olm.hammf.cn

setmetatable({}, { __index = base })
来源：http://fuy.yvedp.cn

[T41] Perl：Hello World
来源：http://rlj.xuanzx.com

print "Hello\n";
来源：http://acx.hysaishi.cn

[T42] Perl：变量类型
来源：http://ddk.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ckj.jinghuilouyu.cn

[T43] Perl：字符串插值
来源：http://kue.chenzaomai.com

"值: $a"
来源：http://pfm.zhaomingkeji.xyz

[T44] Perl：条件
来源：http://vmz.ivvv.top

if ($a > 0) { print "正"; }
来源：http://wzp.smart0.xyz

[T45] Perl：数组遍历
来源：http://ymu.nanxuanxn.top

for my $x (@arr) { print $x; }
来源：http://ecz.nanxinkj.top

[T46] Perl：哈希操作
来源：http://ykn.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qts.svipenyu.cn

[T47] Perl：正则捕获
来源：http://ioz.fengsongda.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ghw.cdnleiting.top

[T48] Perl：正则替换
来源：http://eiy.guowangkeji.top

$s =~ s/old/new/g;
来源：http://xnx.jlsjyb.cn

[T49] Perl：函数
来源：http://gvl.zdbjq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sih.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://kam.jinghuilouyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dmt.jinyuanbaomall.cn

while (my $line = <$fh>) { print $line; }
来源：http://ngv.yfazqb.com

[T51] Scala：Hello World
来源：http://rsp.jinqigufen.top

println("Hello")
来源：http://smy.vqdsnc.cn

[T52] Scala：变量
来源：http://cjz.zhongyouzk.top

val a = 1;  var b = 2
来源：http://icb.tanke756.top

[T53] Scala：字符串插值
来源：http://hyt.hywenlv.cn

s"值: $b"
来源：http://iih.ivvv.top

[T54] Scala：集合映射
来源：http://eds.xziqi.cn

List(1, 2, 3).map(_ * 2)
来源：http://srt.yfazqb.com

[T55] Scala：集合过滤
来源：http://vgk.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://snv.jianghu66.top

[T56] Scala：样例类
来源：http://fns.ctjpmb.com

case class User(name: String, age: Int)
来源：http://ett.sxryk.cn

[T57] Scala：模式匹配
来源：http://gyx.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xrs.snrcjt.cn

[T58] Scala：函数定义
来源：http://tcs.birdmap.top

def add(a: Int, b: Int): Int = a + b
来源：http://kdx.cdnleiting.top

[T59] Scala：循环
来源：http://kql.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://vlh.shangyingyoupin.top

[T60] Scala：折叠
来源：http://hwb.gotoacloud.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sgk.ehwqpu.com

================================================================================
来源：http://jok.pycfn.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zuw.yuxming.cn

================================================================================
来源：http://ouu.0kj1m.cn

[U01] Py：创建虚拟环境
来源：http://mjy.c1oappe.top

python -m venv .venv && source .venv/bin/activate
来源：http://dev.hesvh.cn

[U02] Py：导出 / 安装依赖
来源：http://djt.52xcode.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iij.smart0.xyz

[U03] Py：加载 .env 配置
来源：http://ylo.c1oappe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pos.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://zku.ppjwa.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tlf.yuxming.cn

[U05] Py：列表去重且保序
来源：http://ptp.epnwcf.com

list(dict.fromkeys(arr))
来源：http://zke.kuanghao11.cn

[U06] Py：合并两个字典
来源：http://wqb.316326.xyz

{**a, **b}
来源：http://rfp.shzxlz.cn

[U07] Py：反转字典键值
来源：http://qgi.jyoumei.cn

{v: k for k, v in d.items()}
来源：http://aag.epnwcf.com

[U08] Py：展平二维列表
来源：http://bxy.smart0.xyz

[y for x in nested for y in x]
来源：http://zdn.ctjpmb.com

[U09] Py：字典取最大值的键
来源：http://kry.yanxiufei.cn

max(d, key=d.get)
来源：http://tbv.jlsjyb.cn

[U10] Py：按值排序字典
来源：http://skd.ydjk.org.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://koq.gzhubu.top

[U11] Py：生成器表达式
来源：http://uxa.jinyuanbaomall.cn

(x * 2 for x in arr)
来源：http://bxz.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://goo.cdnleiting.top

Counter(arr).most_common(3)
来源：http://wec.jqgfzy.top

[U13] Py：固定长度队列
来源：http://som.hammf.cn

deque(maxlen=10)
来源：http://lju.yangfankeji.com

[U14] Py：分组收集到列表
来源：http://hdl.zhaomingkeji.xyz

defaultdict(list)
来源：http://flm.epnwcf.com

[U15] Py：高精度计时
来源：http://esu.yuxming.cn

t = time.perf_counter()
来源：http://iuz.shuidangran.top

[U16] Py：命令行参数解析
来源：http://rqc.epnwcf.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://snd.yuxming.cn

[U17] Py：初始化日志
来源：http://dik.gaohongyu789.top

logging.basicConfig(level=logging.INFO)
来源：http://lye.kuanghao11.cn

[U18] Py：预编译正则
来源：http://rpc.aibaodan.cn

pat = re.compile(r"\d+")
来源：http://pmm.feifeiyinyue.top

[U19] Py：正则替换带回调
来源：http://qsl.xingfuxueyuan.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nyo.jqgufenzy.top

[U20] Py：缓存函数结果
来源：http://nuv.chenlongwang.top

@functools.lru_cache(maxsize=None)
来源：http://xrx.xinyue.icu

[U21] Py：自定义上下文管理器
来源：http://eza.ivvv.top

@contextlib.contextmanager
来源：http://jhr.guowangkeji.top

[U22] Py：矩阵转置
来源：http://zry.yueranfly.top

list(zip(*m))
来源：http://ydc.zhixingplan.top

[U23] Py：分块读取大文件
来源：http://vqa.pengpengdd.cyou

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bkf.nanxinkj.top

[U24] Py：路径操作
来源：http://ddn.chenjidiqi.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hio.kuanghao11.cn

[U25] Py：CSV 按字典读
来源：http://onk.shangyingyoupin.top

csv.DictReader(f)
来源：http://wkk.guowangkeji.top

[U26] Py：并发下载
来源：http://fdt.nanxuanxn.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ors.jianghu66.top

[U27] Py：异步 HTTP
来源：http://axh.jinyuanbaomall.cn

aiohttp.ClientSession() 配合 async with
来源：http://diu.zhixingplan.top

[U28] Py：类型别名
来源：http://hfq.bjfxy.top

UserId = int
来源：http://ztf.haohaochexian.top

[U29] Py：属性校验
来源：http://dsm.shangyingyoupin.top

@property 与 @x.setter 配合
来源：http://eld.yonumen.top

[U30] Py：数据类
来源：http://bea.yonumen.top

@dataclass(slots=True)
来源：http://gjk.tanke756.top

[U31] Py：单测
来源：http://uci.yfazqb.com

python -m pytest -q
来源：http://sxi.svipenyu.cn

[U32] Py：代码格式化
来源：http://rag.cucudq.cn

ruff format . && ruff check --fix .
来源：http://czr.sjlbkw.cn

[U33] Py：打包发布
来源：http://dkt.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://lie.fengsongda.top

[U34] Py：判断编码
来源：http://xfd.aizwys.cn

chardet.detect(raw)
来源：http://wcz.wangshuangyany.cn

[U35] Py：发送邮件
来源：http://gaf.jinyuanbaomall.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rkd.snrcjt.cn

[U36] Py：定时任务
来源：http://zwy.jqgfzy.top

schedule.every(10).minutes.do(job)
来源：http://lzj.ivvv.top

[U37] Py：读写 Excel
来源：http://wrr.fengsongda.top

pandas.read_excel / DataFrame.to_excel
来源：http://hfq.chenlongwang.top

[U38] Py：获取脚本所在目录
来源：http://vrz.zdqjudy.top

Path(__file__).resolve().parent
来源：http://fgj.yangfankeji.com

[U39] Py：判断是否在交互环境
来源：http://yob.yfazqb.com

sys.stdout.isatty()
来源：http://oll.hysaishi.cn

[U40] Py：打印到标准错误
来源：http://pfq.aibaodan.cn

print("err", file=sys.stderr)
来源：http://dez.zycfv.cn

[U41] PHP：初始化 Composer 项目
来源：http://fss.ctjpmb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://uao.ydjk.org.cn

[U42] PHP：PSR-4 自动加载
来源：http://lql.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dyq.gaohongyu789.top

[U43] PHP：声明命名空间
来源：http://odg.yanxiufei.cn

namespace App\Http;
来源：http://wwx.jianghu66.top

[U44] PHP：开启严格类型
来源：http://nso.zhoulong.xyz

declare(strict_types=1);
来源：http://fwv.zdbjq.cn


<!-- 参考信息 -->