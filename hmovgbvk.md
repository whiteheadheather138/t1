代发 wailian999

int size() const noexcept { return n_; }
来源：http://otu.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://xpg.sweek.top

std::vector<int> w = std::move(v);
来源：http://vdv.dianchejie.cn

[S54] C++：异常处理
来源：http://vhi.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kkz.shuidangran.top

[S55] C++：结构化绑定
来源：http://djt.fanxiaobao.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://bri.jiagoushi.top

[S56] C++：optional
来源：http://pik.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jxz.snrcjt.cn

[S57] C++：编译期常量
来源：http://usi.zycfv.cn

constexpr int N = 10;
来源：http://zet.bjfxy.top

[S58] C++：命名空间
来源：http://ngh.yuxming.cn

namespace ns { int f() { return 1; } }
来源：http://nta.birdmap.top

[S59] C++：静态断言
来源：http://qfq.zhixingplan.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vyx.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://xah.zhiwuduotai.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gcx.cqqwz.cn

================================================================================
来源：http://epr.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cay.fzhhl.top

================================================================================
来源：http://wcx.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://kji.hnqzz.top

println("Hello")
来源：http://rdm.nanxinkj.top

[T02] Kotlin：变量
来源：http://rfh.xuetiantiany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gja.hcnkem.com

[T03] Kotlin：字符串模板
来源：http://pqo.fehbvm.com

"值: $b"
来源：http://gae.andypj.xyz

[T04] Kotlin：空安全
来源：http://hzl.9152youxi.cn

val n: String? = null;  n?.length
来源：http://jkx.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://sqh.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pwe.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://rbu.ydzc1.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zic.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://ubr.jinqigfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rop.svipenyu.cn

[T08] Kotlin：数据类
来源：http://lcz.fengsongda.top

data class User(val name: String, val age: Int)
来源：http://vit.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://zhw.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://drv.daria6918.cn

[T10] Kotlin：默认参数
来源：http://afq.ywan-chungtsiang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qga.gzhubu.top

[T11] Kotlin：协程
来源：http://cnl.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ids.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://uyq.tianlin.xyz

val (a, b) = Pair(1, 2)
来源：http://swz.guowangkeji.top

[T13] Kotlin：只读 Map
来源：http://zuy.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://oiz.nanxuanxn.top

[T14] Kotlin：循环
来源：http://rts.yj20258.top

for (i in 1..10) println(i)
来源：http://wqn.cheryme.top

[T15] Kotlin：接口
来源：http://wus.vehdjk.com

interface Shape { fun area(): Double }
来源：http://dgl.chenjidiqi.icu

[T16] Swift：Hello World
来源：http://shr.hywenlv.cn

print("Hello")
来源：http://nxr.jinqigufen.top

[T17] Swift：变量与常量
来源：http://nub.jiagoushi.top

var a = 1;  let b = 2
来源：http://aqi.yangfankeji.com

[T18] Swift：字符串插值
来源：http://hmt.vehdjk.com

"值: \(b)"
来源：http://tvh.yj20258888.top

[T19] Swift：可选绑定
来源：http://bhk.meibo888.top

if let n = opt { print(n) }
来源：http://ovw.guannengcc.top

[T20] Swift：数组操作
来源：http://gwa.zhixingplan.top

var a = [1, 2, 3];  a.append(4)
来源：http://zcw.fehbvm.com

[T21] Swift：遍历
来源：http://qoe.jyoumei.cn

for x in a { print(x) }
来源：http://bul.yangfankeji.com

[T22] Swift：字典
来源：http://nrt.nanxuanxn.top

var d = ["a": 1];  d["b"] = 2
来源：http://eaj.tianlin.xyz

[T23] Swift：函数
来源：http://ilr.vehdjk.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ccy.shangyingyoupin.top

[T24] Swift：闭包
来源：http://nrp.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vdl.guowangkeji.top

[T25] Swift：结构体
来源：http://qys.sjlbkw.cn

struct P { var x: Int }
来源：http://yiq.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://odf.yangfankeji.com

class A: Base { override func f() {} }
来源：http://bxv.jqgfzy.top

[T27] Swift：错误处理
来源：http://yqu.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://vhk.sysykeji.top

[T28] Swift：枚举
来源：http://shg.jlsjyb.cn

enum Color { case red, green }
来源：http://sji.jlsjyb.cn

[T29] Swift：guard 提前返回
来源：http://rtv.jinqigfzy.top

guard let x = opt else { return }
来源：http://khj.yangfankeji.com

[T30] Swift：协议
来源：http://llu.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://zvw.redwolf501.top

[T31] Lua：Hello World
来源：http://yyd.shuidangran.top

print("Hello")
来源：http://asy.sysykeji.top

[T32] Lua：局部变量
来源：http://ypq.zhijiandao.cn

local a = 1
来源：http://laa.cucudq.cn

[T33] Lua：表（数组）
来源：http://kuv.yj202588.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fxu.shzxlz.cn

[T34] Lua：遍历表
来源：http://saq.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oye.birdmap.top

[T35] Lua：字典表
来源：http://zaj.yuxming.cn

local d = { a = 1 };  d.b = 2
来源：http://ijn.zycfv.cn

[T36] Lua：函数
来源：http://efw.shzxlz.cn

function add(a, b) return a + b end
来源：http://dum.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://hqp.feifeiyinyue.top

"a" .. "b"
来源：http://hzk.cashguo.top

[T38] Lua：条件
来源：http://fif.ybcxt.top

if x > 0 then print("正") end
来源：http://esq.xingfuxueyuan.xyz

[T39] Lua：模式匹配
来源：http://hbs.yanxiufei.cn

string.find(s, "%d+")
来源：http://djt.redwolf501.top

[T40] Lua：元表
来源：http://prl.tianlin.xyz

setmetatable({}, { __index = base })
来源：http://uvy.yvedp.cn

[T41] Perl：Hello World
来源：http://rmj.havefunace.top

print "Hello\n";
来源：http://sqw.meibo888.top

[T42] Perl：变量类型
来源：http://xmq.xinyue.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uuo.ivvv.top

[T43] Perl：字符串插值
来源：http://tdk.hongshengwenyu.top

"值: $a"
来源：http://jmi.jianghu66.top

[T44] Perl：条件
来源：http://plg.shanyushiyangtech.top

if ($a > 0) { print "正"; }
来源：http://sdj.yongpay.top

[T45] Perl：数组遍历
来源：http://mem.gotoacloud.top

for my $x (@arr) { print $x; }
来源：http://thb.ywan-chungtsiang.top

[T46] Perl：哈希操作
来源：http://mzy.hywenlv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ahi.hfpthk.cn

[T47] Perl：正则捕获
来源：http://bxu.hysaishi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ffv.haohaochexian.top

[T48] Perl：正则替换
来源：http://ynv.dashuyun.cn

$s =~ s/old/new/g;
来源：http://atf.xuanzx.com

[T49] Perl：函数
来源：http://lpa.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hna.jinghuilouyu.cn

[T50] Perl：逐行读文件
来源：http://zcy.shanyushiyangtech.top

open my $fh, "<", "a.txt" or die $!;
来源：http://egu.andypj.xyz

while (my $line = <$fh>) { print $line; }
来源：http://cgy.hysaishi.cn

[T51] Scala：Hello World
来源：http://rpp.guowangkeji.top

println("Hello")
来源：http://gob.daxiang520.top

[T52] Scala：变量
来源：http://ngf.yj202588.top

val a = 1;  var b = 2
来源：http://eae.shangyingyoupin.top

[T53] Scala：字符串插值
来源：http://van.xylfe.cn

s"值: $b"
来源：http://iib.quarkkingdee.top

[T54] Scala：集合映射
来源：http://odv.cashguo.top

List(1, 2, 3).map(_ * 2)
来源：http://goe.chenzaomai.com

[T55] Scala：集合过滤
来源：http://hqa.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fjf.jinqigfzy.top

[T56] Scala：样例类
来源：http://aos.tian-w.cn

case class User(name: String, age: Int)
来源：http://jfi.feifeiyinyue.top

[T57] Scala：模式匹配
来源：http://gsy.andypj.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://xka.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://dhj.xylfe.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ahc.wangdashe.top

[T59] Scala：循环
来源：http://arm.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://sfl.shanyushiyangtech.top

[T60] Scala：折叠
来源：http://ntx.jyoumei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zep.svipenyu.cn

================================================================================
来源：http://rex.sjlbkw.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://njn.ydjk.org.cn

================================================================================
来源：http://guj.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://fnn.yonumen.top

python -m venv .venv && source .venv/bin/activate
来源：http://fqa.jinqigufen.top

[U02] Py：导出 / 安装依赖
来源：http://lyx.zhoulong.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ykt.zhijiandao.cn

[U03] Py：加载 .env 配置
来源：http://nbk.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wts.pycfn.com

[U04] Py：变量调试打印
来源：http://zfp.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uzf.zhijiandao.cn

[U05] Py：列表去重且保序
来源：http://owi.haohaochexian.top

list(dict.fromkeys(arr))
来源：http://cph.yfazqb.com

[U06] Py：合并两个字典
来源：http://dgm.quarkkingdee.top

{**a, **b}
来源：http://nri.xylfe.cn

[U07] Py：反转字典键值
来源：http://eka.ivvv.top

{v: k for k, v in d.items()}
来源：http://naa.shzxlz.cn

[U08] Py：展平二维列表
来源：http://yhw.zdbjq.cn

[y for x in nested for y in x]
来源：http://vta.hfpthk.cn

[U09] Py：字典取最大值的键
来源：http://hxi.ywan-chungtsiang.top

max(d, key=d.get)
来源：http://ggh.yj20258.top

[U10] Py：按值排序字典
来源：http://qwf.cucudq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fko.xylfe.cn

[U11] Py：生成器表达式
来源：http://hmm.ydzc1.top

(x * 2 for x in arr)
来源：http://mfz.kuanghao11.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ktb.52xcode.cn

Counter(arr).most_common(3)
来源：http://mzu.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://rri.jlsjyb.cn

deque(maxlen=10)
来源：http://kds.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://cxq.sjlbkw.cn

defaultdict(list)
来源：http://nqz.tian-w.cn

[U15] Py：高精度计时
来源：http://oek.hysaishi.cn

t = time.perf_counter()
来源：http://shy.sjlbkw.cn

[U16] Py：命令行参数解析
来源：http://huc.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rfq.uphjek.com

[U17] Py：初始化日志
来源：http://pfg.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://uvz.tarul.cn

[U18] Py：预编译正则
来源：http://lde.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://lhd.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://eat.jqgufenzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qeo.chenlongwang.top

[U20] Py：缓存函数结果
来源：http://eeu.zhoulong.xyz

@functools.lru_cache(maxsize=None)
来源：http://pop.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://xai.tianlin.xyz

@contextlib.contextmanager
来源：http://wdy.bjfxy.top

[U22] Py：矩阵转置
来源：http://byf.redwolf501.top

list(zip(*m))
来源：http://dhf.fzhhl.top

[U23] Py：分块读取大文件
来源：http://icq.jyoumei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qha.yanxiufei.cn

[U24] Py：路径操作
来源：http://ghd.yj202588.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gez.xziqi.cn

[U25] Py：CSV 按字典读
来源：http://hzv.quarkkingdee.top

csv.DictReader(f)
来源：http://duv.haohaochexian.top

[U26] Py：并发下载
来源：http://gia.mhx1999.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gnh.shanyushiyangkeji.top

[U27] Py：异步 HTTP
来源：http://qvi.haohaochexian.top

aiohttp.ClientSession() 配合 async with
来源：http://guo.tanke756.top

[U28] Py：类型别名
来源：http://uah.mhx1999.top

UserId = int
来源：http://ovv.ydzc1.top

[U29] Py：属性校验
来源：http://cvw.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://ttq.cucudq.cn

[U30] Py：数据类
来源：http://axw.uphjek.com

@dataclass(slots=True)
来源：http://xcz.haohaochexian.top

[U31] Py：单测
来源：http://hlz.jinghuilouyu.cn

python -m pytest -q
来源：http://vph.fengsongda.top

[U32] Py：代码格式化
来源：http://vit.redwolf501.top

ruff format . && ruff check --fix .
来源：http://ktq.xuetiantiany.cn

[U33] Py：打包发布
来源：http://car.ydjk.org.cn

python -m build  （依赖 pyproject.toml）
来源：http://zrw.quarkkingdee.top

[U34] Py：判断编码
来源：http://dgs.fengsongda.top

chardet.detect(raw)
来源：http://fbw.cheryme.top

[U35] Py：发送邮件
来源：http://byi.ctjpmb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mwq.fktsv.cn

[U36] Py：定时任务
来源：http://nxx.sxryk.cn

schedule.every(10).minutes.do(job)
来源：http://wlh.fzhhl.top

[U37] Py：读写 Excel
来源：http://kwg.zdbjq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wzg.yuxming.cn

[U38] Py：获取脚本所在目录
来源：http://gra.ppjwa.cn

Path(__file__).resolve().parent
来源：http://xxw.fehbvm.com

[U39] Py：判断是否在交互环境
来源：http://xhm.aibaodan.cn

sys.stdout.isatty()
来源：http://bjs.hfpthk.cn

[U40] Py：打印到标准错误
来源：http://axk.daxiang520.top

print("err", file=sys.stderr)
来源：http://ril.shzxlz.cn

[U41] PHP：初始化 Composer 项目
来源：http://gub.cucudq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rcy.hesvh.cn

[U42] PHP：PSR-4 自动加载
来源：http://wkc.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hoa.yvedp.cn

[U43] PHP：声明命名空间
来源：http://yre.nanxuanxn.top

namespace App\Http;
来源：http://zet.gzhubu.top

[U44] PHP：开启严格类型
来源：http://kri.wangshuangyany.cn

declare(strict_types=1);
来源：http://rjg.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://lcn.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nrb.shanyushiyangkeji.top

[U46] PHP：可空类型
来源：http://sla.chenlongwang.top

?string $name = null
来源：http://qsf.ctjpmb.com

[U47] PHP：联合类型
来源：http://cfb.tarul.cn

int|string $id
来源：http://css.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://ptw.chenzaomai.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tvf.sysykeji.top

[U49] PHP：只读属性
来源：http://qbk.sweek.top

public readonly string $name
来源：http://put.aizwys.cn

[U50] PHP：构造器属性提升
来源：http://xna.shzxlz.cn

public function __construct(private int $id) {}
来源：http://uiw.xingfuxueyuan.xyz

[U51] PHP：数组解构
来源：http://vhv.pycfn.com

[$a, $b] = $arr;
来源：http://jko.shangyingyoupin.top

[U52] PHP：箭头函数
来源：http://gpa.hywenlv.cn

$double = fn($x) => $x * 2;
来源：http://jge.wangdashe.top

[U53] PHP：空合并运算符
来源：http://dro.nanxinkj.top

$v = $a ?? $b ?? "default";
来源：http://bci.yvedp.cn

[U54] PHP：空安全调用
来源：http://zjk.jqgfzy.top

$obj?->method()
来源：http://nmz.hfpthk.cn

[U55] PHP：match 表达式
来源：http://jwk.fzhhl.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gbi.zdqjudy.top

[U56] PHP：命名参数
来源：http://crj.kuanghao11.cn

f(a: 1, b: 2)
来源：http://dnr.snrcjt.cn

[U57] PHP：字符串插值
来源：http://oyg.xingfuxueyuan.xyz

"值: {$a}"
来源：http://meu.yj202588.top

[U58] PHP：数组三件套
来源：http://izh.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://phb.hywenlv.cn

[U59] PHP：自定义排序
来源：http://ubf.shangyingyoupin.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://esh.yj202588.top

[U60] PHP：JSON 编解码
来源：http://jhf.nanxinkj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jkk.hongshengwenyu.top

[U61] PHP：正则
来源：http://lwg.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ydq.ppjwa.cn

[U62] PHP：日期对象
来源：http://uoc.quarkkingdee.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zti.xuetiantiany.cn

[U63] PHP：文件读写
来源：http://jpg.316326.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lzo.zdqjudy.top

[U64] PHP：目录遍历
来源：http://gyv.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://ddu.havefunace.top

[U65] PHP：会话
来源：http://ppf.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ofn.redwolf501.top

[U66] PHP：设置 Cookie
来源：http://tqe.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nka.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://vxh.cucudq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://txx.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://wyc.sjlbkw.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://smm.zhiwuduotai.top

[U69] PHP：PDO 预处理
来源：http://tjz.zhixingplan.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lfr.vehdjk.com

[U70] PHP：PDO 事务
来源：http://xau.jqgufenzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zsu.hywenlv.cn

[U71] PHP：抛出异常
来源：http://ssx.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://qaz.hesvh.cn

[U72] PHP：写错误日志
来源：http://ehy.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://sry.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://olm.pengpengdd.cyou

parse_ini_file("config.ini", true)
来源：http://cek.cqqwz.cn

[U74] PHP：读取环境变量
来源：http://mvp.yuanzhike.top

getenv("APP_ENV") ?: "production"
来源：http://ahf.ybcxt.top

[U75] PHP：依赖注入
来源：http://ckw.tian-w.cn

composer require psr/container
来源：http://nvc.c1oappe.top

[U76] PHP：简单路由
来源：http://grs.daxiang520.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lvk.zhaomingkeji.xyz

[U77] PHP：模板渲染
来源：http://nnv.nanxuanxn.top

composer require twig/twig
来源：http://nlk.andypj.xyz

[U78] PHP：单元测试
来源：http://izt.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://arn.xinyue.icu


<!-- 参考信息 -->