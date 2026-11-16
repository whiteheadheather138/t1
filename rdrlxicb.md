代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://ejz.hnqzz.top

[S23] C：随机数
来源：http://ioi.hesvh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oag.guannengcc.top

[S24] C：获取本地时间
来源：http://rqr.kuanghao11.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xvs.smart0.xyz

[S25] C：内存拷贝
来源：http://jox.zhijiandao.cn

memcpy(dst, src, n);
来源：http://yxm.ydzc1.top

[S26] C：内存清零
来源：http://une.hongshengwenyu.top

memset(a, 0, sizeof a);
来源：http://mly.xylfe.cn

[S27] C：定义常量
来源：http://mjv.fehbvm.com

const double PI = 3.14159;
来源：http://xjn.hammf.cn

[S28] C：静态变量
来源：http://drw.hywenlv.cn

static int counter = 0;
来源：http://knl.cashguo.top

[S29] C：变参函数
来源：http://fdy.zhijiandao.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nbb.nwbrower.top

[S30] C：头文件保护
来源：http://pxj.fzhhl.top

#ifndef X_H
来源：http://ctl.jlsjyb.cn

#define X_H
来源：http://gzn.xuanzx.com

#endif
来源：http://sgu.ydzc1.top

[S31] C++：Hello World
来源：http://iav.xinyue.icu

#include <iostream>
来源：http://olh.chenzaomai.com

int main() { std::cout << "Hello\n"; }
来源：http://gai.sysykeji.top

[S32] C++：字符串
来源：http://zeh.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://hxm.meibo888.top

[S33] C++：vector 增删
来源：http://osx.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://heb.zhijiandao.cn

[S34] C++：遍历 vector
来源：http://bam.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://hqx.cashguo.top

[S35] C++：map
来源：http://pyb.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fcb.pengpengdd.cyou

[S36] C++：unordered_map
来源：http://eqr.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://exm.nwbrower.top

[S37] C++：set
来源：http://agm.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xbi.fktsv.cn

[S38] C++：排序
来源：http://qcj.shanyushiyangtech.top

std::sort(v.begin(), v.end());
来源：http://cjm.bjfxy.top

[S39] C++：自定义比较器排序
来源：http://bll.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ozu.hongshengwenyu.top

[S40] C++：查找元素
来源：http://biu.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://odk.52xcode.cn

[S41] C++：类与构造函数
来源：http://jvp.ehwqpu.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zid.sysykeji.top

[S42] C++：继承与虚函数
来源：http://lpa.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://uug.hnxiangtu.top

[S43] C++：智能指针
来源：http://suf.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://ura.jqgfzy.top

[S44] C++：引用传参
来源：http://del.yvedp.cn

void inc(int &x) { ++x; }
来源：http://tcn.xylfe.cn

[S45] C++：lambda
来源：http://qnu.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://vbv.sweek.top

[S46] C++：函数模板
来源：http://mnx.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ytg.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://igh.hammf.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://omi.iojbl.cn

[S48] C++：逐行读文件
来源：http://jxl.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://tlq.sxryk.cn

while (std::getline(in, line)) { }
来源：http://apg.9152youxi.cn

[S49] C++：写文件
来源：http://ldv.jqgufenzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oli.xuanzx.com

[S50] C++：格式化数字
来源：http://fvg.jqgfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qwf.yj202588.top

[S51] C++：显式类型转换
来源：http://gms.mhx1999.top

static_cast<double>(a) / b
来源：http://vsz.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://nce.hammf.cn

int size() const noexcept { return n_; }
来源：http://krt.gotoacloud.top

[S53] C++：移动语义
来源：http://apt.quarkkingdee.top

std::vector<int> w = std::move(v);
来源：http://zba.yonumen.top

[S54] C++：异常处理
来源：http://fmb.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pvu.hammf.cn

[S55] C++：结构化绑定
来源：http://xkt.gogol.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ism.hywenlv.cn

[S56] C++：optional
来源：http://okt.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ugt.daria6918.cn

[S57] C++：编译期常量
来源：http://tij.yj20258.top

constexpr int N = 10;
来源：http://bdg.bjfxy.top

[S58] C++：命名空间
来源：http://nqz.smart0.xyz

namespace ns { int f() { return 1; } }
来源：http://apo.nanxinkj.top

[S59] C++：静态断言
来源：http://idq.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://coq.yongpay.top

[S60] C++：遍历并删除元素
来源：http://ajt.yanxiufei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yud.ydzc1.top

================================================================================
来源：http://euh.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yre.dianchejie.cn

================================================================================
来源：http://oox.ivvv.top

[T01] Kotlin：Hello World
来源：http://wiq.aizwys.cn

println("Hello")
来源：http://bxx.zdqjudy.top

[T02] Kotlin：变量
来源：http://roj.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dza.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://vwo.uphjek.com

"值: $b"
来源：http://dzz.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://mbd.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://gme.zhengqikj.top

[T05] Kotlin：when 表达式
来源：http://htc.fehbvm.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lwl.gotoacloud.top

[T06] Kotlin：集合映射
来源：http://lnl.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hvm.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://dqe.zycfv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wgy.tarul.cn

[T08] Kotlin：数据类
来源：http://uqm.sjlbkw.cn

data class User(val name: String, val age: Int)
来源：http://kqq.ivvv.top

[T09] Kotlin：扩展函数
来源：http://wpf.bbcook.cn

fun String.exclaim() = this + "!"
来源：http://lbf.xinyue.icu

[T10] Kotlin：默认参数
来源：http://eeo.redwolf501.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nab.quarkkingdee.top

[T11] Kotlin：协程
来源：http://lxm.gaohongyu789.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ynu.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://aji.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://mwu.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://jhs.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://mgb.xuanzx.com

[T14] Kotlin：循环
来源：http://kbc.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://ydq.nanxinkj.top

[T15] Kotlin：接口
来源：http://hgu.havefunace.top

interface Shape { fun area(): Double }
来源：http://uze.xziqi.cn

[T16] Swift：Hello World
来源：http://ymf.yuanzhike.top

print("Hello")
来源：http://vsq.cqqwz.cn

[T17] Swift：变量与常量
来源：http://fos.pycfn.com

var a = 1;  let b = 2
来源：http://eyw.hysaishi.cn

[T18] Swift：字符串插值
来源：http://cne.gogol.net.cn

"值: \(b)"
来源：http://qvh.cdnleiting.top

[T19] Swift：可选绑定
来源：http://xdg.ywan-chungtsiang.top

if let n = opt { print(n) }
来源：http://hfd.cheryme.top

[T20] Swift：数组操作
来源：http://lgl.ivvv.top

var a = [1, 2, 3];  a.append(4)
来源：http://udj.chenjidiqi.icu

[T21] Swift：遍历
来源：http://vjk.tian-w.cn

for x in a { print(x) }
来源：http://tts.gotoacloud.top

[T22] Swift：字典
来源：http://gtn.jinghuilouyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cju.chenjidiqi.icu

[T23] Swift：函数
来源：http://yip.vehdjk.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eey.fktsv.cn

[T24] Swift：闭包
来源：http://nft.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cjm.jlsjyb.cn

[T25] Swift：结构体
来源：http://pox.yueranfly.top

struct P { var x: Int }
来源：http://aiv.yonumen.top

[T26] Swift：类与重写
来源：http://qog.nwbrower.top

class A: Base { override func f() {} }
来源：http://sss.daria6918.cn

[T27] Swift：错误处理
来源：http://ffo.yfazqb.com

do { try f() } catch { print(error) }
来源：http://vas.yanxiufei.cn

[T28] Swift：枚举
来源：http://vau.wangdashe.top

enum Color { case red, green }
来源：http://nuu.ehwqpu.com

[T29] Swift：guard 提前返回
来源：http://xtx.mhx1999.top

guard let x = opt else { return }
来源：http://zjo.zycfv.cn

[T30] Swift：协议
来源：http://ebz.zhoulong.xyz

protocol Shape { func area() -> Double }
来源：http://cxr.dianchejie.cn

[T31] Lua：Hello World
来源：http://pnd.zdqjudy.top

print("Hello")
来源：http://npb.zhengqikj.top

[T32] Lua：局部变量
来源：http://jpk.quarkkingdee.top

local a = 1
来源：http://vhw.ehwqpu.com

[T33] Lua：表（数组）
来源：http://xwu.sufxvd.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ooq.wangdashe.top

[T34] Lua：遍历表
来源：http://kgi.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wgz.sysykeji.top

[T35] Lua：字典表
来源：http://zhq.zdbjq.cn

local d = { a = 1 };  d.b = 2
来源：http://jao.hnxiangtu.top

[T36] Lua：函数
来源：http://rwu.yonumen.top

function add(a, b) return a + b end
来源：http://ail.yuxming.cn

[T37] Lua：字符串拼接
来源：http://hrc.316326.xyz

"a" .. "b"
来源：http://cvj.fktsv.cn

[T38] Lua：条件
来源：http://rmv.shanyushiyangkeji.top

if x > 0 then print("正") end
来源：http://ktn.hfpthk.cn

[T39] Lua：模式匹配
来源：http://pze.haohaochexian.top

string.find(s, "%d+")
来源：http://acq.daria6918.cn

[T40] Lua：元表
来源：http://kdt.yuanzhike.top

setmetatable({}, { __index = base })
来源：http://dax.xingfuxueyuan.xyz

[T41] Perl：Hello World
来源：http://zen.tianlin.xyz

print "Hello\n";
来源：http://jmq.snrcjt.cn

[T42] Perl：变量类型
来源：http://qdw.haohaochexian.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yud.sweek.top

[T43] Perl：字符串插值
来源：http://upx.hnqzz.top

"值: $a"
来源：http://uye.jqgfzy.top

[T44] Perl：条件
来源：http://mpe.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://mle.xziqi.cn

[T45] Perl：数组遍历
来源：http://pnh.zhengqikj.top

for my $x (@arr) { print $x; }
来源：http://yvt.hammf.cn

[T46] Perl：哈希操作
来源：http://mbq.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mvs.zhixingplan.top

[T47] Perl：正则捕获
来源：http://zkd.bjfxy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kcv.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://cii.svipenyu.cn

$s =~ s/old/new/g;
来源：http://uqo.316326.xyz

[T49] Perl：函数
来源：http://fdy.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gvs.bjfxy.top

[T50] Perl：逐行读文件
来源：http://tfk.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tdk.chenlongwang.top

while (my $line = <$fh>) { print $line; }
来源：http://pnd.guowangkeji.top

[T51] Scala：Hello World
来源：http://qzn.bjfxy.top

println("Hello")
来源：http://ajt.nwbrower.top

[T52] Scala：变量
来源：http://wjh.nwbrower.top

val a = 1;  var b = 2
来源：http://vgp.bjfxy.top

[T53] Scala：字符串插值
来源：http://olp.kuanghao11.cn

s"值: $b"
来源：http://nue.ppjwa.cn

[T54] Scala：集合映射
来源：http://emj.dashuyun.cn

List(1, 2, 3).map(_ * 2)
来源：http://dnn.redwolf501.top

[T55] Scala：集合过滤
来源：http://msl.haohaochexian.top

List(1, 2, 3).filter(_ > 1)
来源：http://srz.gotoacloud.top

[T56] Scala：样例类
来源：http://emr.cashguo.top

case class User(name: String, age: Int)
来源：http://abu.nanxuanxn.top

[T57] Scala：模式匹配
来源：http://uxw.jlsjyb.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gbl.feifeiyinyue.top

[T58] Scala：函数定义
来源：http://vat.nanxinkj.top

def add(a: Int, b: Int): Int = a + b
来源：http://fus.yongpay.top

[T59] Scala：循环
来源：http://gon.dashuyun.cn

for (i <- 1 to 10) println(i)
来源：http://vyd.hysaishi.cn

[T60] Scala：折叠
来源：http://mze.gotoacloud.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vug.gzhubu.top

================================================================================
来源：http://sex.jqgfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://axz.birdmap.top

================================================================================
来源：http://cxp.pengpengdd.cyou

[U01] Py：创建虚拟环境
来源：http://jvq.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://xyp.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://bqu.fehbvm.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://arg.feifeiyinyue.top

[U03] Py：加载 .env 配置
来源：http://yxl.ywan-chungtsiang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dhc.tianlin.xyz

[U04] Py：变量调试打印
来源：http://dgc.hfpthk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hwm.jiagoushi.top

[U05] Py：列表去重且保序
来源：http://huq.yj202588.top

list(dict.fromkeys(arr))
来源：http://yes.yj202588.top

[U06] Py：合并两个字典
来源：http://ycb.jinghuilouyu.cn

{**a, **b}
来源：http://lte.zhiwuduotai.top

[U07] Py：反转字典键值
来源：http://qgw.cucudq.cn

{v: k for k, v in d.items()}
来源：http://gin.ppjwa.cn

[U08] Py：展平二维列表
来源：http://zel.pycfn.com

[y for x in nested for y in x]
来源：http://eei.zhoulong.xyz

[U09] Py：字典取最大值的键
来源：http://czn.9152youxi.cn

max(d, key=d.get)
来源：http://bbw.hcnkem.com

[U10] Py：按值排序字典
来源：http://gez.zhijiandao.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kha.zhijiandao.cn

[U11] Py：生成器表达式
来源：http://xwx.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://ygv.ctjpmb.com

[U12] Py：取出现最多的 3 个元素
来源：http://bge.havefunace.top

Counter(arr).most_common(3)
来源：http://gqw.hfpthk.cn

[U13] Py：固定长度队列
来源：http://col.0kj1m.cn

deque(maxlen=10)
来源：http://ppu.nanxinkj.top

[U14] Py：分组收集到列表
来源：http://gbc.tianlin.xyz

defaultdict(list)
来源：http://rml.zhoulong.xyz

[U15] Py：高精度计时
来源：http://pha.zhaomingkeji.xyz

t = time.perf_counter()
来源：http://odc.yj202588.top

[U16] Py：命令行参数解析
来源：http://xno.yangfankeji.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fzc.fzhhl.top

[U17] Py：初始化日志
来源：http://nnr.hywenlv.cn

logging.basicConfig(level=logging.INFO)
来源：http://hon.aibaodan.cn

[U18] Py：预编译正则
来源：http://iwy.52xcode.cn

pat = re.compile(r"\d+")
来源：http://qsc.jianghu66.top

[U19] Py：正则替换带回调
来源：http://xwe.yangfankeji.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ofx.zhijiandao.cn

[U20] Py：缓存函数结果
来源：http://ito.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://rzn.tian-w.cn

[U21] Py：自定义上下文管理器
来源：http://hhx.zhaomingkeji.xyz

@contextlib.contextmanager
来源：http://oix.gzhubu.top

[U22] Py：矩阵转置
来源：http://kpu.gotoacloud.top

list(zip(*m))
来源：http://pxl.hammf.cn

[U23] Py：分块读取大文件
来源：http://qga.0kj1m.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://czx.zhijiandao.cn

[U24] Py：路径操作
来源：http://uky.xziqi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vqy.tarul.cn

[U25] Py：CSV 按字典读
来源：http://uxc.jyoumei.cn

csv.DictReader(f)
来源：http://mkw.fzhhl.top

[U26] Py：并发下载
来源：http://hqi.yuxming.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yhe.kuanghao11.cn

[U27] Py：异步 HTTP
来源：http://ycb.svipenyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://nsg.nwbrower.top

[U28] Py：类型别名
来源：http://jes.hnqzz.top

UserId = int
来源：http://ifn.hesvh.cn

[U29] Py：属性校验
来源：http://mly.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://nwc.hnqzz.top

[U30] Py：数据类
来源：http://xpe.xuanzx.com

@dataclass(slots=True)
来源：http://muv.cheryme.top

[U31] Py：单测
来源：http://txu.hcnkem.com

python -m pytest -q
来源：http://wgl.epnwcf.com

[U32] Py：代码格式化
来源：http://ssn.feifeiyinyue.top

ruff format . && ruff check --fix .
来源：http://oqm.hnxiangtu.top

[U33] Py：打包发布
来源：http://txd.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://qnq.zdqjudy.top

[U34] Py：判断编码
来源：http://jqq.sjlbkw.cn

chardet.detect(raw)
来源：http://nwu.smart0.xyz

[U35] Py：发送邮件
来源：http://nwd.tian-w.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nfx.bbcook.cn

[U36] Py：定时任务
来源：http://vtd.havefunace.top

schedule.every(10).minutes.do(job)
来源：http://pqz.nanxuanxn.top

[U37] Py：读写 Excel
来源：http://vno.jlsjyb.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xln.zdbjq.cn

[U38] Py：获取脚本所在目录
来源：http://kiw.ehwqpu.com

Path(__file__).resolve().parent
来源：http://dxo.aizwys.cn

[U39] Py：判断是否在交互环境
来源：http://mju.zdbjq.cn

sys.stdout.isatty()
来源：http://ngx.yj202588.top

[U40] Py：打印到标准错误
来源：http://lfz.shuidangran.top

print("err", file=sys.stderr)
来源：http://fhi.jinyuanbaomall.cn

[U41] PHP：初始化 Composer 项目
来源：http://hta.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://iid.zhaomingkeji.xyz

[U42] PHP：PSR-4 自动加载
来源：http://dsk.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rqq.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://pqf.zycfv.cn

namespace App\Http;
来源：http://jhj.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://fck.hesvh.cn

declare(strict_types=1);
来源：http://nla.bjfxy.top

[U45] PHP：类型声明与返回类型
来源：http://bxd.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sle.316326.xyz

[U46] PHP：可空类型
来源：http://mbq.zhoulong.xyz

?string $name = null
来源：http://zca.zhoulong.xyz


<!-- 参考信息 -->