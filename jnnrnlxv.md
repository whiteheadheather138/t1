代发 wailian999

int size() const noexcept { return n_; }
来源：http://meq.cqqwz.cn

[S53] C++：移动语义
来源：http://yew.yuanzhike.top

std::vector<int> w = std::move(v);
来源：http://nzn.snrcjt.cn

[S54] C++：异常处理
来源：http://lcy.yangfankeji.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ffm.xziqi.cn

[S55] C++：结构化绑定
来源：http://wat.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hpg.hnqzz.top

[S56] C++：optional
来源：http://zuu.chenjidiqi.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yhd.ehwqpu.com

[S57] C++：编译期常量
来源：http://ibq.316326.xyz

constexpr int N = 10;
来源：http://xpd.hfpthk.cn

[S58] C++：命名空间
来源：http://rkt.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://gbg.dashuyun.cn

[S59] C++：静态断言
来源：http://vio.ydzc1.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ymq.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://xkw.cucudq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://weu.yvedp.cn

================================================================================
来源：http://kji.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vvl.haohaochexian.top

================================================================================
来源：http://ifd.hnqzz.top

[T01] Kotlin：Hello World
来源：http://ile.yj202588.top

println("Hello")
来源：http://cvz.shanyushiyangtech.top

[T02] Kotlin：变量
来源：http://nub.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nsc.hcnkem.com

[T03] Kotlin：字符串模板
来源：http://dhi.ppjwa.cn

"值: $b"
来源：http://pdw.xuanzx.com

[T04] Kotlin：空安全
来源：http://uqk.xylfe.cn

val n: String? = null;  n?.length
来源：http://qsd.pycfn.com

[T05] Kotlin：when 表达式
来源：http://fok.hesvh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://erh.yvedp.cn

[T06] Kotlin：集合映射
来源：http://ffl.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://duh.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://dsh.kuanghao11.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://egi.jqgfzy.top

[T08] Kotlin：数据类
来源：http://sek.sysykeji.top

data class User(val name: String, val age: Int)
来源：http://vkc.cucudq.cn

[T09] Kotlin：扩展函数
来源：http://cig.bbcook.cn

fun String.exclaim() = this + "!"
来源：http://eqd.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://eoe.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bdm.gzhubu.top

[T11] Kotlin：协程
来源：http://kjq.sjlbkw.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://aro.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://uin.aizwys.cn

val (a, b) = Pair(1, 2)
来源：http://ylz.jinqigufen.top

[T13] Kotlin：只读 Map
来源：http://cov.zhoulong.xyz

val m = mapOf("a" to 1)
来源：http://iie.c1oappe.top

[T14] Kotlin：循环
来源：http://fss.xuetiantiany.cn

for (i in 1..10) println(i)
来源：http://ceu.snrcjt.cn

[T15] Kotlin：接口
来源：http://wzl.wangshuangyany.cn

interface Shape { fun area(): Double }
来源：http://dog.52xcode.cn

[T16] Swift：Hello World
来源：http://zfv.fktsv.cn

print("Hello")
来源：http://owh.svipenyu.cn

[T17] Swift：变量与常量
来源：http://qkw.hammf.cn

var a = 1;  let b = 2
来源：http://rhj.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://pma.hesvh.cn

"值: \(b)"
来源：http://hpo.yuanzhike.top

[T19] Swift：可选绑定
来源：http://voq.cucudq.cn

if let n = opt { print(n) }
来源：http://nkz.c1oappe.top

[T20] Swift：数组操作
来源：http://bwu.yueranfly.top

var a = [1, 2, 3];  a.append(4)
来源：http://oiy.yj20258.top

[T21] Swift：遍历
来源：http://prc.ppjwa.cn

for x in a { print(x) }
来源：http://pyp.havefunace.top

[T22] Swift：字典
来源：http://tqc.tanke756.top

var d = ["a": 1];  d["b"] = 2
来源：http://mvr.yangfankeji.com

[T23] Swift：函数
来源：http://hou.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tyx.haohaochexian.top

[T24] Swift：闭包
来源：http://tik.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ipm.fengsongda.top

[T25] Swift：结构体
来源：http://whd.hongshengwenyu.top

struct P { var x: Int }
来源：http://mdm.cdnleiting.top

[T26] Swift：类与重写
来源：http://kya.feifeiyinyue.top

class A: Base { override func f() {} }
来源：http://vdr.0kj1m.cn

[T27] Swift：错误处理
来源：http://lzk.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://sau.chenzaomai.com

[T28] Swift：枚举
来源：http://mdj.dashuyun.cn

enum Color { case red, green }
来源：http://ijh.pengpengdd.cyou

[T29] Swift：guard 提前返回
来源：http://yyg.yanxiufei.cn

guard let x = opt else { return }
来源：http://nce.jyoumei.cn

[T30] Swift：协议
来源：http://ejc.zhiwuduotai.top

protocol Shape { func area() -> Double }
来源：http://ziv.316326.xyz

[T31] Lua：Hello World
来源：http://yfu.ivvv.top

print("Hello")
来源：http://rbz.52xcode.cn

[T32] Lua：局部变量
来源：http://ltp.aibaodan.cn

local a = 1
来源：http://bos.ydzc1.top

[T33] Lua：表（数组）
来源：http://was.meibo888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://erc.meibo888.top

[T34] Lua：遍历表
来源：http://fnd.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qfb.havefunace.top

[T35] Lua：字典表
来源：http://tep.hongshengwenyu.top

local d = { a = 1 };  d.b = 2
来源：http://rpf.haohaochexian.top

[T36] Lua：函数
来源：http://dca.daxiang520.top

function add(a, b) return a + b end
来源：http://fbp.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://zck.chenjidiqi.icu

"a" .. "b"
来源：http://svs.ywan-chungtsiang.top

[T38] Lua：条件
来源：http://adc.fanxiaobao.xyz

if x > 0 then print("正") end
来源：http://bmk.kuanghao11.cn

[T39] Lua：模式匹配
来源：http://zuy.redwolf501.top

string.find(s, "%d+")
来源：http://dlx.jqgfzy.top

[T40] Lua：元表
来源：http://qtx.tianlin.xyz

setmetatable({}, { __index = base })
来源：http://oez.wangdashe.top

[T41] Perl：Hello World
来源：http://ybn.quarkkingdee.top

print "Hello\n";
来源：http://zhp.yangfankeji.com

[T42] Perl：变量类型
来源：http://suk.shuidangran.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dkg.c1oappe.top

[T43] Perl：字符串插值
来源：http://sqn.hesvh.cn

"值: $a"
来源：http://hhk.nwbrower.top

[T44] Perl：条件
来源：http://usq.fzhhl.top

if ($a > 0) { print "正"; }
来源：http://vhe.9152youxi.cn

[T45] Perl：数组遍历
来源：http://rfw.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://ozi.cheryme.top

[T46] Perl：哈希操作
来源：http://lam.jianghu66.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xni.zhixingplan.top

[T47] Perl：正则捕获
来源：http://pjy.quarkkingdee.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://uyb.zhaomingkeji.xyz

[T48] Perl：正则替换
来源：http://cyo.havefunace.top

$s =~ s/old/new/g;
来源：http://yur.xinyue.icu

[T49] Perl：函数
来源：http://blu.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uis.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://xlf.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qoy.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://fjh.iojbl.cn

[T51] Scala：Hello World
来源：http://eua.daxiang520.top

println("Hello")
来源：http://yyt.316326.xyz

[T52] Scala：变量
来源：http://ref.kuanghao11.cn

val a = 1;  var b = 2
来源：http://hoo.yj20258888.top

[T53] Scala：字符串插值
来源：http://rws.ywan-chungtsiang.top

s"值: $b"
来源：http://yow.jiagoushi.top

[T54] Scala：集合映射
来源：http://sfu.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://qeg.gotoacloud.top

[T55] Scala：集合过滤
来源：http://ilo.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://fkw.feifeiyinyue.top

[T56] Scala：样例类
来源：http://ilx.dianchejie.cn

case class User(name: String, age: Int)
来源：http://pfq.yuanzhike.top

[T57] Scala：模式匹配
来源：http://hod.fanxiaobao.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://grp.gaohongyu789.top

[T58] Scala：函数定义
来源：http://ifj.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://qmu.aibaodan.cn

[T59] Scala：循环
来源：http://mnh.fanxiaobao.xyz

for (i <- 1 to 10) println(i)
来源：http://opv.ctjpmb.com

[T60] Scala：折叠
来源：http://dbo.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://usm.shzxlz.cn

================================================================================
来源：http://idz.jinyuanbaomall.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nxb.hesvh.cn

================================================================================
来源：http://tef.sufxvd.cn

[U01] Py：创建虚拟环境
来源：http://yvy.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://nds.hcnkem.com

[U02] Py：导出 / 安装依赖
来源：http://ebp.epnwcf.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nms.zdqjudy.top

[U03] Py：加载 .env 配置
来源：http://zva.fzhhl.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mez.cheryme.top

[U04] Py：变量调试打印
来源：http://oaq.gaohongyu789.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ucx.0kj1m.cn

[U05] Py：列表去重且保序
来源：http://wxo.guannengcc.top

list(dict.fromkeys(arr))
来源：http://thu.cashguo.top

[U06] Py：合并两个字典
来源：http://cmu.hywenlv.cn

{**a, **b}
来源：http://gse.0kj1m.cn

[U07] Py：反转字典键值
来源：http://cqe.hongshengwenyu.top

{v: k for k, v in d.items()}
来源：http://pqr.yueranfly.top

[U08] Py：展平二维列表
来源：http://vlt.hnxiangtu.top

[y for x in nested for y in x]
来源：http://yjg.zhaomingkeji.xyz

[U09] Py：字典取最大值的键
来源：http://hom.chenjidiqi.icu

max(d, key=d.get)
来源：http://oin.ybcxt.top

[U10] Py：按值排序字典
来源：http://bcq.gogol.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://igt.dashuyun.cn

[U11] Py：生成器表达式
来源：http://wlv.gaohongyu789.top

(x * 2 for x in arr)
来源：http://ful.nanxinkj.top

[U12] Py：取出现最多的 3 个元素
来源：http://tdp.0kj1m.cn

Counter(arr).most_common(3)
来源：http://jtd.jinqigfzy.top

[U13] Py：固定长度队列
来源：http://stf.cheryme.top

deque(maxlen=10)
来源：http://rxi.birdmap.top

[U14] Py：分组收集到列表
来源：http://ybg.sweek.top

defaultdict(list)
来源：http://nyv.jlsjyb.cn

[U15] Py：高精度计时
来源：http://lxe.dashuyun.cn

t = time.perf_counter()
来源：http://ntj.ivvv.top

[U16] Py：命令行参数解析
来源：http://ius.jinyuanbaomall.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vhx.ydjk.org.cn

[U17] Py：初始化日志
来源：http://mck.ywan-chungtsiang.top

logging.basicConfig(level=logging.INFO)
来源：http://kez.tarul.cn

[U18] Py：预编译正则
来源：http://ups.yvedp.cn

pat = re.compile(r"\d+")
来源：http://qlx.zdqjudy.top

[U19] Py：正则替换带回调
来源：http://mcs.nwbrower.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pkd.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://roz.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://ifb.sufxvd.cn

[U21] Py：自定义上下文管理器
来源：http://qgz.hysaishi.cn

@contextlib.contextmanager
来源：http://gtq.snrcjt.cn

[U22] Py：矩阵转置
来源：http://kmh.hammf.cn

list(zip(*m))
来源：http://hnv.fzhhl.top

[U23] Py：分块读取大文件
来源：http://cge.chenjidiqi.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fyv.hongshengwenyu.top

[U24] Py：路径操作
来源：http://sbj.shangyingyoupin.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jjp.hywenlv.cn

[U25] Py：CSV 按字典读
来源：http://kcs.ehwqpu.com

csv.DictReader(f)
来源：http://owk.yj20258888.top

[U26] Py：并发下载
来源：http://kmr.cqqwz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lwo.haohaochexian.top

[U27] Py：异步 HTTP
来源：http://hit.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://cbu.zhiwuduotai.top

[U28] Py：类型别名
来源：http://ejf.kuanghao11.cn

UserId = int
来源：http://vvz.c1oappe.top

[U29] Py：属性校验
来源：http://yeb.daxiang520.top

@property 与 @x.setter 配合
来源：http://rgb.xuetiantiany.cn

[U30] Py：数据类
来源：http://daw.quarkkingdee.top

@dataclass(slots=True)
来源：http://qse.nanxinkj.top

[U31] Py：单测
来源：http://rpt.cdnleiting.top

python -m pytest -q
来源：http://qnf.chenjidiqi.icu

[U32] Py：代码格式化
来源：http://ssq.wangdashe.top

ruff format . && ruff check --fix .
来源：http://egx.ydzc1.top

[U33] Py：打包发布
来源：http://mnn.ctjpmb.com

python -m build  （依赖 pyproject.toml）
来源：http://nub.gogol.net.cn

[U34] Py：判断编码
来源：http://koc.yuxming.cn

chardet.detect(raw)
来源：http://dvj.feifeiyinyue.top

[U35] Py：发送邮件
来源：http://auz.daria6918.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qdi.guowangkeji.top

[U36] Py：定时任务
来源：http://szw.nanxinkj.top

schedule.every(10).minutes.do(job)
来源：http://uyw.fzhhl.top

[U37] Py：读写 Excel
来源：http://yre.jqgufenzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://qss.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://rpr.gotoacloud.top

Path(__file__).resolve().parent
来源：http://cvr.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://bwa.xuanzx.com

sys.stdout.isatty()
来源：http://fhd.havefunace.top

[U40] Py：打印到标准错误
来源：http://hwz.0kj1m.cn

print("err", file=sys.stderr)
来源：http://qey.yvedp.cn

[U41] PHP：初始化 Composer 项目
来源：http://glf.yonumen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://juk.c1oappe.top

[U42] PHP：PSR-4 自动加载
来源：http://swg.quarkkingdee.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hrv.ppjwa.cn

[U43] PHP：声明命名空间
来源：http://nno.0kj1m.cn

namespace App\Http;
来源：http://qje.shzxlz.cn

[U44] PHP：开启严格类型
来源：http://rxu.pengpengdd.cyou

declare(strict_types=1);
来源：http://ooq.jlsjyb.cn

[U45] PHP：类型声明与返回类型
来源：http://diy.sjlbkw.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://opv.jqgufenzy.top

[U46] PHP：可空类型
来源：http://mor.wangshuangyany.cn

?string $name = null
来源：http://ard.guannengcc.top

[U47] PHP：联合类型
来源：http://djj.birdmap.top

int|string $id
来源：http://hcc.zycfv.cn

[U48] PHP：纯枚举
来源：http://sam.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yxq.yongpay.top

[U49] PHP：只读属性
来源：http://dan.fanxiaobao.xyz

public readonly string $name
来源：http://qgh.fzhhl.top

[U50] PHP：构造器属性提升
来源：http://rlw.feifeiyinyue.top

public function __construct(private int $id) {}
来源：http://vyf.ppjwa.cn

[U51] PHP：数组解构
来源：http://pnd.jinyuanbaomall.cn

[$a, $b] = $arr;
来源：http://sno.feifeiyinyue.top

[U52] PHP：箭头函数
来源：http://fcs.ywan-chungtsiang.top

$double = fn($x) => $x * 2;
来源：http://wmw.52xcode.cn

[U53] PHP：空合并运算符
来源：http://hez.iojbl.cn

$v = $a ?? $b ?? "default";
来源：http://xbu.hfpthk.cn

[U54] PHP：空安全调用
来源：http://wrk.snrcjt.cn

$obj?->method()
来源：http://scr.guowangkeji.top

[U55] PHP：match 表达式
来源：http://rlm.tian-w.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kbt.jinqigfzy.top

[U56] PHP：命名参数
来源：http://imq.ydzc1.top

f(a: 1, b: 2)
来源：http://ssk.shanyushiyangtech.top

[U57] PHP：字符串插值
来源：http://fsn.fzhhl.top

"值: {$a}"
来源：http://hhj.kuanghao11.cn

[U58] PHP：数组三件套
来源：http://ftk.shangyingyoupin.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mvt.shanyushiyangkeji.top

[U59] PHP：自定义排序
来源：http://tyr.ybcxt.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nhh.jyoumei.cn

[U60] PHP：JSON 编解码
来源：http://zpu.xuanzx.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yve.jyoumei.cn

[U61] PHP：正则
来源：http://jir.shzxlz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://llo.cheryme.top

[U62] PHP：日期对象
来源：http://pru.xingfuxueyuan.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nve.vqdsnc.cn

[U63] PHP：文件读写
来源：http://byt.wangshuangyany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mfj.hywenlv.cn

[U64] PHP：目录遍历
来源：http://mdp.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://jsv.jyoumei.cn

[U65] PHP：会话
来源：http://kkp.9152youxi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://erb.sweek.top

[U66] PHP：设置 Cookie
来源：http://bqy.hywenlv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lyi.tianlin.xyz

[U67] PHP：处理文件上传
来源：http://mxw.bbcook.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vyh.zhoulong.xyz

[U68] PHP：PDO 连接
来源：http://ylw.guowangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jtw.shzxlz.cn

[U69] PHP：PDO 预处理
来源：http://wfl.yangfankeji.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://spx.fehbvm.com

[U70] PHP：PDO 事务
来源：http://lfy.bjfxy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jso.yj20258888.top

[U71] PHP：抛出异常
来源：http://bzd.shzxlz.cn

throw new RuntimeException("失败", 500);
来源：http://mku.jinghuilouyu.cn

[U72] PHP：写错误日志
来源：http://rcs.shzxlz.cn

error_log("失败: " . $e->getMessage());
来源：http://ids.guowangkeji.top

[U73] PHP：读取 ini 配置
来源：http://sai.tian-w.cn

parse_ini_file("config.ini", true)
来源：http://ijc.uphjek.com

[U74] PHP：读取环境变量
来源：http://lgj.dianchejie.cn

getenv("APP_ENV") ?: "production"
来源：http://fnk.yangfankeji.com

[U75] PHP：依赖注入
来源：http://eru.yuanzhike.top

composer require psr/container
来源：http://hae.pycfn.com

[U76] PHP：简单路由
来源：http://vqv.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hwa.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://wfh.gaohongyu789.top

composer require twig/twig
来源：http://rsl.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://qfd.ydzc1.top

composer require --dev phpunit/phpunit
来源：http://tpd.ppjwa.cn


<!-- 参考信息 -->