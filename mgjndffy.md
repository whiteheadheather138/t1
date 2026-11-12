代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lkx.fengsongda.top

[S55] C++：结构化绑定
来源：http://jcc.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://hou.dashuyun.cn

[S56] C++：optional
来源：http://hee.ivvv.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lgu.dianchejie.cn

[S57] C++：编译期常量
来源：http://vfp.pengpengdd.cyou

constexpr int N = 10;
来源：http://gup.redwolf501.top

[S58] C++：命名空间
来源：http://xvh.andypj.xyz

namespace ns { int f() { return 1; } }
来源：http://ihc.gotoacloud.top

[S59] C++：静态断言
来源：http://ile.haohaochexian.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hkd.cashguo.top

[S60] C++：遍历并删除元素
来源：http://hoi.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ihm.9152youxi.cn

================================================================================
来源：http://bja.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rrd.feifeiyinyue.top

================================================================================
来源：http://slc.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://lqd.dashuyun.cn

println("Hello")
来源：http://vcr.ydzc1.top

[T02] Kotlin：变量
来源：http://nnb.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hjo.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://ipq.zhijiandao.cn

"值: $b"
来源：http://saj.daria6918.cn

[T04] Kotlin：空安全
来源：http://dmt.yueranfly.top

val n: String? = null;  n?.length
来源：http://ztm.ydjk.org.cn

[T05] Kotlin：when 表达式
来源：http://uvk.feifeiyinyue.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hsz.guannengcc.top

[T06] Kotlin：集合映射
来源：http://udy.hysaishi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zvs.vehdjk.com

[T07] Kotlin：集合过滤
来源：http://cew.pengpengdd.cyou

listOf(1, 2, 3).filter { it > 1 }
来源：http://dti.tian-w.cn

[T08] Kotlin：数据类
来源：http://aqu.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://ufk.havefunace.top

[T09] Kotlin：扩展函数
来源：http://sha.andypj.xyz

fun String.exclaim() = this + "!"
来源：http://xyk.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://lxj.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ryj.vehdjk.com

[T11] Kotlin：协程
来源：http://xqv.zhijiandao.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ozy.gotoacloud.top

[T12] Kotlin：解构声明
来源：http://orh.aizwys.cn

val (a, b) = Pair(1, 2)
来源：http://igy.bbcook.cn

[T13] Kotlin：只读 Map
来源：http://snu.gotoacloud.top

val m = mapOf("a" to 1)
来源：http://lfy.cashguo.top

[T14] Kotlin：循环
来源：http://yqx.guowangkeji.top

for (i in 1..10) println(i)
来源：http://rkl.nanxuanxn.top

[T15] Kotlin：接口
来源：http://duw.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://zfh.gotoacloud.top

[T16] Swift：Hello World
来源：http://ggh.fehbvm.com

print("Hello")
来源：http://zly.daxiang520.top

[T17] Swift：变量与常量
来源：http://ikz.jinqigfzy.top

var a = 1;  let b = 2
来源：http://uar.jinyuanbaomall.cn

[T18] Swift：字符串插值
来源：http://ohs.ydjk.org.cn

"值: \(b)"
来源：http://rpz.sufxvd.cn

[T19] Swift：可选绑定
来源：http://nuo.havefunace.top

if let n = opt { print(n) }
来源：http://dgc.jlsjyb.cn

[T20] Swift：数组操作
来源：http://hgk.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pcw.52xcode.cn

[T21] Swift：遍历
来源：http://zru.havefunace.top

for x in a { print(x) }
来源：http://adz.shzxlz.cn

[T22] Swift：字典
来源：http://eqs.shzxlz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://occ.zycfv.cn

[T23] Swift：函数
来源：http://oxg.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wzn.nanxuanxn.top

[T24] Swift：闭包
来源：http://fxd.cheryme.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kgc.aizwys.cn

[T25] Swift：结构体
来源：http://hvm.daria6918.cn

struct P { var x: Int }
来源：http://hia.hcnkem.com

[T26] Swift：类与重写
来源：http://lhr.cdnleiting.top

class A: Base { override func f() {} }
来源：http://dkr.gogol.net.cn

[T27] Swift：错误处理
来源：http://trq.shanyushiyangtech.top

do { try f() } catch { print(error) }
来源：http://ekm.shangyingyoupin.top

[T28] Swift：枚举
来源：http://riu.ybcxt.top

enum Color { case red, green }
来源：http://xkh.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://mxu.sxryk.cn

guard let x = opt else { return }
来源：http://odo.jinqigfzy.top

[T30] Swift：协议
来源：http://ade.pycfn.com

protocol Shape { func area() -> Double }
来源：http://fxm.quarkkingdee.top

[T31] Lua：Hello World
来源：http://gew.fzhhl.top

print("Hello")
来源：http://wtk.hesvh.cn

[T32] Lua：局部变量
来源：http://aez.xuanzx.com

local a = 1
来源：http://yty.xziqi.cn

[T33] Lua：表（数组）
来源：http://mjk.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://baw.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://jfz.yongpay.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pyn.shzxlz.cn

[T35] Lua：字典表
来源：http://fec.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://rdg.jiagoushi.top

[T36] Lua：函数
来源：http://rea.9152youxi.cn

function add(a, b) return a + b end
来源：http://cxg.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://qli.yj202588.top

"a" .. "b"
来源：http://phg.xinyue.icu

[T38] Lua：条件
来源：http://mrx.xylfe.cn

if x > 0 then print("正") end
来源：http://wmx.hesvh.cn

[T39] Lua：模式匹配
来源：http://vam.hesvh.cn

string.find(s, "%d+")
来源：http://zyx.sweek.top

[T40] Lua：元表
来源：http://yef.shzxlz.cn

setmetatable({}, { __index = base })
来源：http://tcw.ctjpmb.com

[T41] Perl：Hello World
来源：http://omz.jinqigfzy.top

print "Hello\n";
来源：http://mdr.cucudq.cn

[T42] Perl：变量类型
来源：http://jjl.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gge.pycfn.com

[T43] Perl：字符串插值
来源：http://odl.iojbl.cn

"值: $a"
来源：http://hjn.yuanzhike.top

[T44] Perl：条件
来源：http://zxj.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://ept.shzxlz.cn

[T45] Perl：数组遍历
来源：http://tdt.chenzaomai.com

for my $x (@arr) { print $x; }
来源：http://djt.gzhubu.top

[T46] Perl：哈希操作
来源：http://bzg.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zaw.tian-w.cn

[T47] Perl：正则捕获
来源：http://ttv.shanyushiyangtech.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ldd.xylfe.cn

[T48] Perl：正则替换
来源：http://ewc.meibo888.top

$s =~ s/old/new/g;
来源：http://zjl.gotoacloud.top

[T49] Perl：函数
来源：http://rei.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://upu.yongpay.top

[T50] Perl：逐行读文件
来源：http://lue.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qig.birdmap.top

while (my $line = <$fh>) { print $line; }
来源：http://sji.ehwqpu.com

[T51] Scala：Hello World
来源：http://nuo.sufxvd.cn

println("Hello")
来源：http://dll.yongpay.top

[T52] Scala：变量
来源：http://nlu.yuanzhike.top

val a = 1;  var b = 2
来源：http://thn.jinqigufen.top

[T53] Scala：字符串插值
来源：http://mhs.yj20258.top

s"值: $b"
来源：http://mnc.havefunace.top

[T54] Scala：集合映射
来源：http://owp.epnwcf.com

List(1, 2, 3).map(_ * 2)
来源：http://uaf.mhx1999.top

[T55] Scala：集合过滤
来源：http://smj.xingfuxueyuan.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://hni.jianghu66.top

[T56] Scala：样例类
来源：http://aaw.jlsjyb.cn

case class User(name: String, age: Int)
来源：http://qxl.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://yvj.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://nhf.ivvv.top

[T58] Scala：函数定义
来源：http://yca.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://amw.jiagoushi.top

[T59] Scala：循环
来源：http://bcq.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://pgt.uphjek.com

[T60] Scala：折叠
来源：http://rnn.ctjpmb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vcw.jinqigfzy.top

================================================================================
来源：http://nqg.yvedp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kst.yvedp.cn

================================================================================
来源：http://btv.cdnleiting.top

[U01] Py：创建虚拟环境
来源：http://agx.iojbl.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sbx.xingfuxueyuan.xyz

[U02] Py：导出 / 安装依赖
来源：http://rbx.zhongyouzk.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qmn.hnqzz.top

[U03] Py：加载 .env 配置
来源：http://hlb.316326.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://mog.vqdsnc.cn

[U04] Py：变量调试打印
来源：http://ixe.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kzx.shuidangran.top

[U05] Py：列表去重且保序
来源：http://jlj.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://ing.tian-w.cn

[U06] Py：合并两个字典
来源：http://bxe.fengsongda.top

{**a, **b}
来源：http://iqw.havefunace.top

[U07] Py：反转字典键值
来源：http://zpi.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://moc.gzhubu.top

[U08] Py：展平二维列表
来源：http://cwd.yuanzhike.top

[y for x in nested for y in x]
来源：http://xhx.fengsongda.top

[U09] Py：字典取最大值的键
来源：http://dep.tian-w.cn

max(d, key=d.get)
来源：http://zsw.chenzaomai.com

[U10] Py：按值排序字典
来源：http://fdw.yangfankeji.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://quh.shzxlz.cn

[U11] Py：生成器表达式
来源：http://lyt.nwbrower.top

(x * 2 for x in arr)
来源：http://htb.zhengqikj.top

[U12] Py：取出现最多的 3 个元素
来源：http://nxp.tanke756.top

Counter(arr).most_common(3)
来源：http://feg.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://tal.zhixingplan.top

deque(maxlen=10)
来源：http://rjf.fehbvm.com

[U14] Py：分组收集到列表
来源：http://jgr.jiagoushi.top

defaultdict(list)
来源：http://gkr.xylfe.cn

[U15] Py：高精度计时
来源：http://qad.tanke756.top

t = time.perf_counter()
来源：http://wma.fktsv.cn

[U16] Py：命令行参数解析
来源：http://lyy.xinyue.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bmg.hesvh.cn

[U17] Py：初始化日志
来源：http://cgm.fanxiaobao.xyz

logging.basicConfig(level=logging.INFO)
来源：http://gqw.jqgfzy.top

[U18] Py：预编译正则
来源：http://zis.aibaodan.cn

pat = re.compile(r"\d+")
来源：http://bmj.daxiang520.top

[U19] Py：正则替换带回调
来源：http://awb.aibaodan.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mgy.hesvh.cn

[U20] Py：缓存函数结果
来源：http://zkb.chenlongwang.top

@functools.lru_cache(maxsize=None)
来源：http://nto.zdbjq.cn

[U21] Py：自定义上下文管理器
来源：http://lze.ydzc1.top

@contextlib.contextmanager
来源：http://tqu.shanyushiyangtech.top

[U22] Py：矩阵转置
来源：http://fgs.52xcode.cn

list(zip(*m))
来源：http://oon.jinghuilouyu.cn

[U23] Py：分块读取大文件
来源：http://vul.c1oappe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gke.0kj1m.cn

[U24] Py：路径操作
来源：http://lgx.hongshengwenyu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uvo.cdnleiting.top

[U25] Py：CSV 按字典读
来源：http://zlj.mhx1999.top

csv.DictReader(f)
来源：http://tnt.hnxiangtu.top

[U26] Py：并发下载
来源：http://uqz.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qul.wangdashe.top

[U27] Py：异步 HTTP
来源：http://kub.uphjek.com

aiohttp.ClientSession() 配合 async with
来源：http://osq.yj20258888.top

[U28] Py：类型别名
来源：http://kum.hfpthk.cn

UserId = int
来源：http://bqu.yuxming.cn

[U29] Py：属性校验
来源：http://bza.nanxinkj.top

@property 与 @x.setter 配合
来源：http://ltg.ybcxt.top

[U30] Py：数据类
来源：http://vsf.wangdashe.top

@dataclass(slots=True)
来源：http://agd.dianchejie.cn

[U31] Py：单测
来源：http://xik.fengsongda.top

python -m pytest -q
来源：http://tfk.ywan-chungtsiang.top

[U32] Py：代码格式化
来源：http://orn.ywan-chungtsiang.top

ruff format . && ruff check --fix .
来源：http://toj.shuidangran.top

[U33] Py：打包发布
来源：http://vkb.chenzaomai.com

python -m build  （依赖 pyproject.toml）
来源：http://qtz.xingfuxueyuan.xyz

[U34] Py：判断编码
来源：http://kxi.shanyushiyangtech.top

chardet.detect(raw)
来源：http://vix.yfazqb.com

[U35] Py：发送邮件
来源：http://wgv.birdmap.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eoa.jinyuanbaomall.cn

[U36] Py：定时任务
来源：http://ela.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://ejc.meibo888.top

[U37] Py：读写 Excel
来源：http://hqp.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://ihl.tarul.cn

[U38] Py：获取脚本所在目录
来源：http://zfu.jlsjyb.cn

Path(__file__).resolve().parent
来源：http://rcv.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://ksx.havefunace.top

sys.stdout.isatty()
来源：http://scu.vehdjk.com

[U40] Py：打印到标准错误
来源：http://voc.hnqzz.top

print("err", file=sys.stderr)
来源：http://oxj.redwolf501.top

[U41] PHP：初始化 Composer 项目
来源：http://stw.andypj.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://iyg.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://upm.tianlin.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qzh.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://mwy.zycfv.cn

namespace App\Http;
来源：http://cia.fzhhl.top

[U44] PHP：开启严格类型
来源：http://hyw.fehbvm.com

declare(strict_types=1);
来源：http://nbd.yuanzhike.top

[U45] PHP：类型声明与返回类型
来源：http://dau.cqqwz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dqg.hesvh.cn

[U46] PHP：可空类型
来源：http://uzo.yj202588.top

?string $name = null
来源：http://mhi.meibo888.top

[U47] PHP：联合类型
来源：http://aht.jyoumei.cn

int|string $id
来源：http://him.gogol.net.cn

[U48] PHP：纯枚举
来源：http://iwa.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cpw.jqgfzy.top

[U49] PHP：只读属性
来源：http://pyb.meibo888.top

public readonly string $name
来源：http://yul.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://guu.sufxvd.cn

public function __construct(private int $id) {}
来源：http://ewe.iojbl.cn

[U51] PHP：数组解构
来源：http://hui.fehbvm.com

[$a, $b] = $arr;
来源：http://iij.andypj.xyz

[U52] PHP：箭头函数
来源：http://uyx.uphjek.com

$double = fn($x) => $x * 2;
来源：http://pur.fktsv.cn

[U53] PHP：空合并运算符
来源：http://loi.kuanghao11.cn

$v = $a ?? $b ?? "default";
来源：http://owz.ivvv.top

[U54] PHP：空安全调用
来源：http://fno.0kj1m.cn

$obj?->method()
来源：http://mfb.c1oappe.top

[U55] PHP：match 表达式
来源：http://sui.ppjwa.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lqx.hysaishi.cn

[U56] PHP：命名参数
来源：http://tef.bjfxy.top

f(a: 1, b: 2)
来源：http://wfr.yuxming.cn

[U57] PHP：字符串插值
来源：http://tpf.hcnkem.com

"值: {$a}"
来源：http://phl.shzxlz.cn

[U58] PHP：数组三件套
来源：http://dde.fanxiaobao.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lsz.tarul.cn

[U59] PHP：自定义排序
来源：http://dcc.ivvv.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tos.ppjwa.cn

[U60] PHP：JSON 编解码
来源：http://erv.ybcxt.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oxu.jinyuanbaomall.cn

[U61] PHP：正则
来源：http://bgx.jinghuilouyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dkg.cucudq.cn

[U62] PHP：日期对象
来源：http://ecg.ydzc1.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gpw.fehbvm.com

[U63] PHP：文件读写
来源：http://fst.meibo888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aro.xziqi.cn

[U64] PHP：目录遍历
来源：http://kva.hnxiangtu.top

glob("dir/*.php");  scandir("dir");
来源：http://dpq.uphjek.com

[U65] PHP：会话
来源：http://lhf.zhoulong.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://akt.shanyushiyangtech.top

[U66] PHP：设置 Cookie
来源：http://vpn.gaohongyu789.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pmp.shanyushiyangtech.top

[U67] PHP：处理文件上传
来源：http://fjj.quarkkingdee.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nlh.bbcook.cn

[U68] PHP：PDO 连接
来源：http://uhq.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gcw.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://qgg.yj202588.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://olx.aizwys.cn

[U70] PHP：PDO 事务
来源：http://axd.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yrp.yj20258888.top

[U71] PHP：抛出异常
来源：http://ebb.cashguo.top

throw new RuntimeException("失败", 500);
来源：http://bor.yj20258888.top

[U72] PHP：写错误日志
来源：http://txd.nanxinkj.top

error_log("失败: " . $e->getMessage());
来源：http://xdc.gaohongyu789.top

[U73] PHP：读取 ini 配置
来源：http://hqu.ppjwa.cn

parse_ini_file("config.ini", true)
来源：http://rho.ybcxt.top

[U74] PHP：读取环境变量
来源：http://ejb.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://dfg.vqdsnc.cn

[U75] PHP：依赖注入
来源：http://sit.xziqi.cn

composer require psr/container
来源：http://zwz.yongpay.top

[U76] PHP：简单路由
来源：http://idn.zhixingplan.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nrr.xingfuxueyuan.xyz

[U77] PHP：模板渲染
来源：http://rkv.cucudq.cn

composer require twig/twig
来源：http://jqd.iojbl.cn

[U78] PHP：单元测试
来源：http://obi.chenjidiqi.icu

composer require --dev phpunit/phpunit
来源：http://slc.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://nqz.fanxiaobao.xyz

composer require --dev phpstan/phpstan
来源：http://oud.zhongyouzk.top

[U80] PHP：代码规范修复
来源：http://twh.cheryme.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mln.meibo888.top


<!-- 参考信息 -->