代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bno.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://ugg.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yjd.zhiwuduotai.top

[S56] C++：optional
来源：http://kcc.sysykeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vwy.vqdsnc.cn

[S57] C++：编译期常量
来源：http://xul.yangfankeji.com

constexpr int N = 10;
来源：http://tya.pengpengdd.cyou

[S58] C++：命名空间
来源：http://kvn.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://zqi.gzhubu.top

[S59] C++：静态断言
来源：http://lzv.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://her.cdnleiting.top

[S60] C++：遍历并删除元素
来源：http://orz.uphjek.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://obh.fzhhl.top

================================================================================
来源：http://wnf.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bxe.c1oappe.top

================================================================================
来源：http://ehh.fehbvm.com

[T01] Kotlin：Hello World
来源：http://fdn.sxryk.cn

println("Hello")
来源：http://dbl.svipenyu.cn

[T02] Kotlin：变量
来源：http://ydd.gogol.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hmy.yj20258.top

[T03] Kotlin：字符串模板
来源：http://pru.zhixingplan.top

"值: $b"
来源：http://jsc.hammf.cn

[T04] Kotlin：空安全
来源：http://wlo.zhongyouzk.top

val n: String? = null;  n?.length
来源：http://qpi.sweek.top

[T05] Kotlin：when 表达式
来源：http://uje.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nol.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://qum.zhaomingkeji.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://nrn.fehbvm.com

[T07] Kotlin：集合过滤
来源：http://wwp.ybcxt.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vma.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://xpd.316326.xyz

data class User(val name: String, val age: Int)
来源：http://twg.zhijiandao.cn

[T09] Kotlin：扩展函数
来源：http://fyr.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://zeb.daria6918.cn

[T10] Kotlin：默认参数
来源：http://zdl.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lim.redwolf501.top

[T11] Kotlin：协程
来源：http://vqp.zhengqikj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nsb.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://klo.tanke756.top

val (a, b) = Pair(1, 2)
来源：http://llc.redwolf501.top

[T13] Kotlin：只读 Map
来源：http://qau.fengsongda.top

val m = mapOf("a" to 1)
来源：http://kkw.yfazqb.com

[T14] Kotlin：循环
来源：http://tkg.cashguo.top

for (i in 1..10) println(i)
来源：http://muq.wangshuangyany.cn

[T15] Kotlin：接口
来源：http://tco.smart0.xyz

interface Shape { fun area(): Double }
来源：http://yzt.shzxlz.cn

[T16] Swift：Hello World
来源：http://blp.shzxlz.cn

print("Hello")
来源：http://yya.sufxvd.cn

[T17] Swift：变量与常量
来源：http://oxm.shanyushiyangtech.top

var a = 1;  let b = 2
来源：http://ezn.cqqwz.cn

[T18] Swift：字符串插值
来源：http://fls.guowangkeji.top

"值: \(b)"
来源：http://rpn.zhiwuduotai.top

[T19] Swift：可选绑定
来源：http://dwf.jinqigufen.top

if let n = opt { print(n) }
来源：http://npf.hnxiangtu.top

[T20] Swift：数组操作
来源：http://vid.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://gsp.jinqigfzy.top

[T21] Swift：遍历
来源：http://qmb.jiagoushi.top

for x in a { print(x) }
来源：http://pdb.9152youxi.cn

[T22] Swift：字典
来源：http://zgf.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://zmj.vqdsnc.cn

[T23] Swift：函数
来源：http://ozg.ctjpmb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://trd.jinqigufen.top

[T24] Swift：闭包
来源：http://ezm.fktsv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gar.zhijiandao.cn

[T25] Swift：结构体
来源：http://llh.xuanzx.com

struct P { var x: Int }
来源：http://xhu.jiagoushi.top

[T26] Swift：类与重写
来源：http://okj.tianlin.xyz

class A: Base { override func f() {} }
来源：http://cen.yonumen.top

[T27] Swift：错误处理
来源：http://cny.dianchejie.cn

do { try f() } catch { print(error) }
来源：http://jxz.nwbrower.top

[T28] Swift：枚举
来源：http://wzm.nwbrower.top

enum Color { case red, green }
来源：http://vex.yanxiufei.cn

[T29] Swift：guard 提前返回
来源：http://rhx.yuanzhike.top

guard let x = opt else { return }
来源：http://lsi.wangdashe.top

[T30] Swift：协议
来源：http://qjf.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://rpy.hysaishi.cn

[T31] Lua：Hello World
来源：http://ciz.tian-w.cn

print("Hello")
来源：http://ddd.gzhubu.top

[T32] Lua：局部变量
来源：http://qsj.sjlbkw.cn

local a = 1
来源：http://mcy.fzhhl.top

[T33] Lua：表（数组）
来源：http://avy.bjfxy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dlx.316326.xyz

[T34] Lua：遍历表
来源：http://qgh.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rwe.havefunace.top

[T35] Lua：字典表
来源：http://nja.aizwys.cn

local d = { a = 1 };  d.b = 2
来源：http://sjf.haohaochexian.top

[T36] Lua：函数
来源：http://ggn.sufxvd.cn

function add(a, b) return a + b end
来源：http://ifo.birdmap.top

[T37] Lua：字符串拼接
来源：http://vip.ctjpmb.com

"a" .. "b"
来源：http://fia.shuidangran.top

[T38] Lua：条件
来源：http://izk.yj202588.top

if x > 0 then print("正") end
来源：http://wdn.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://ecj.ywan-chungtsiang.top

string.find(s, "%d+")
来源：http://igs.bbcook.cn

[T40] Lua：元表
来源：http://xha.bjfxy.top

setmetatable({}, { __index = base })
来源：http://pop.wangdashe.top

[T41] Perl：Hello World
来源：http://qmg.jqgufenzy.top

print "Hello\n";
来源：http://rnn.xingfuxueyuan.xyz

[T42] Perl：变量类型
来源：http://xym.ehwqpu.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pgz.316326.xyz

[T43] Perl：字符串插值
来源：http://pqr.pycfn.com

"值: $a"
来源：http://gvw.nanxinkj.top

[T44] Perl：条件
来源：http://xkv.shanyushiyangtech.top

if ($a > 0) { print "正"; }
来源：http://swe.yuanzhike.top

[T45] Perl：数组遍历
来源：http://ors.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://ssh.yangfankeji.com

[T46] Perl：哈希操作
来源：http://qvu.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tdm.shanyushiyangtech.top

[T47] Perl：正则捕获
来源：http://dqu.hesvh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gop.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://yfi.sufxvd.cn

$s =~ s/old/new/g;
来源：http://yra.yvedp.cn

[T49] Perl：函数
来源：http://nsh.feifeiyinyue.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zcg.nanxuanxn.top

[T50] Perl：逐行读文件
来源：http://vwz.tanke756.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bwy.fktsv.cn

while (my $line = <$fh>) { print $line; }
来源：http://zcd.cheryme.top

[T51] Scala：Hello World
来源：http://lvc.xylfe.cn

println("Hello")
来源：http://oow.zhixingplan.top

[T52] Scala：变量
来源：http://iiu.quarkkingdee.top

val a = 1;  var b = 2
来源：http://glz.sufxvd.cn

[T53] Scala：字符串插值
来源：http://rqj.jianghu66.top

s"值: $b"
来源：http://wkv.sxryk.cn

[T54] Scala：集合映射
来源：http://iid.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://hud.sxryk.cn

[T55] Scala：集合过滤
来源：http://fiy.hnxiangtu.top

List(1, 2, 3).filter(_ > 1)
来源：http://umw.feifeiyinyue.top

[T56] Scala：样例类
来源：http://hkl.dashuyun.cn

case class User(name: String, age: Int)
来源：http://xki.uphjek.com

[T57] Scala：模式匹配
来源：http://zvy.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zbn.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://wsz.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://ucn.guowangkeji.top

[T59] Scala：循环
来源：http://akt.zycfv.cn

for (i <- 1 to 10) println(i)
来源：http://ooh.jyoumei.cn

[T60] Scala：折叠
来源：http://rrm.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nla.hcnkem.com

================================================================================
来源：http://ede.zhoulong.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fft.shzxlz.cn

================================================================================
来源：http://pqn.zdbjq.cn

[U01] Py：创建虚拟环境
来源：http://srl.hnqzz.top

python -m venv .venv && source .venv/bin/activate
来源：http://upa.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://mbk.gzhubu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pki.cqqwz.cn

[U03] Py：加载 .env 配置
来源：http://flp.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://pzq.xuanzx.com

[U04] Py：变量调试打印
来源：http://cme.sweek.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://voc.gaohongyu789.top

[U05] Py：列表去重且保序
来源：http://etd.jinqigfzy.top

list(dict.fromkeys(arr))
来源：http://xel.yonumen.top

[U06] Py：合并两个字典
来源：http://pni.jqgfzy.top

{**a, **b}
来源：http://abb.epnwcf.com

[U07] Py：反转字典键值
来源：http://efm.fktsv.cn

{v: k for k, v in d.items()}
来源：http://lnc.svipenyu.cn

[U08] Py：展平二维列表
来源：http://wdb.ppjwa.cn

[y for x in nested for y in x]
来源：http://kof.gzhubu.top

[U09] Py：字典取最大值的键
来源：http://dxc.dashuyun.cn

max(d, key=d.get)
来源：http://ibt.hywenlv.cn

[U10] Py：按值排序字典
来源：http://xfq.jiagoushi.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://azc.nanxuanxn.top

[U11] Py：生成器表达式
来源：http://cyf.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://lxo.jinqigufen.top

[U12] Py：取出现最多的 3 个元素
来源：http://eve.zhongyouzk.top

Counter(arr).most_common(3)
来源：http://xbc.jinghuilouyu.cn

[U13] Py：固定长度队列
来源：http://fog.zhongyouzk.top

deque(maxlen=10)
来源：http://nao.hesvh.cn

[U14] Py：分组收集到列表
来源：http://rym.hfpthk.cn

defaultdict(list)
来源：http://wuj.zycfv.cn

[U15] Py：高精度计时
来源：http://ill.cheryme.top

t = time.perf_counter()
来源：http://obf.havefunace.top

[U16] Py：命令行参数解析
来源：http://tlg.zycfv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xqm.nanxuanxn.top

[U17] Py：初始化日志
来源：http://edb.hywenlv.cn

logging.basicConfig(level=logging.INFO)
来源：http://epo.bbcook.cn

[U18] Py：预编译正则
来源：http://dzr.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://qnm.gogol.net.cn

[U19] Py：正则替换带回调
来源：http://aiw.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bei.aizwys.cn

[U20] Py：缓存函数结果
来源：http://gir.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://icn.guannengcc.top

[U21] Py：自定义上下文管理器
来源：http://fdr.shuidangran.top

@contextlib.contextmanager
来源：http://kyu.hesvh.cn

[U22] Py：矩阵转置
来源：http://qpv.zdqjudy.top

list(zip(*m))
来源：http://dum.fengsongda.top

[U23] Py：分块读取大文件
来源：http://wlr.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sad.yuanzhike.top

[U24] Py：路径操作
来源：http://ocv.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rzq.uphjek.com

[U25] Py：CSV 按字典读
来源：http://ljp.shuidangran.top

csv.DictReader(f)
来源：http://tlr.xinyue.icu

[U26] Py：并发下载
来源：http://sdf.jianghu66.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fsk.tanke756.top

[U27] Py：异步 HTTP
来源：http://rai.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://dhg.daria6918.cn

[U28] Py：类型别名
来源：http://tep.fengsongda.top

UserId = int
来源：http://hhx.gzhubu.top

[U29] Py：属性校验
来源：http://gjt.snrcjt.cn

@property 与 @x.setter 配合
来源：http://qou.zhaomingkeji.xyz

[U30] Py：数据类
来源：http://bdy.gaohongyu789.top

@dataclass(slots=True)
来源：http://poe.cashguo.top

[U31] Py：单测
来源：http://pmo.yj202588.top

python -m pytest -q
来源：http://aud.tianlin.xyz

[U32] Py：代码格式化
来源：http://dgh.shanyushiyangtech.top

ruff format . && ruff check --fix .
来源：http://apx.pengpengdd.cyou

[U33] Py：打包发布
来源：http://ufj.zycfv.cn

python -m build  （依赖 pyproject.toml）
来源：http://cud.yj202588.top

[U34] Py：判断编码
来源：http://gdh.c1oappe.top

chardet.detect(raw)
来源：http://lcl.tarul.cn

[U35] Py：发送邮件
来源：http://hvw.jinyuanbaomall.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://utu.tarul.cn

[U36] Py：定时任务
来源：http://wpe.zdqjudy.top

schedule.every(10).minutes.do(job)
来源：http://oli.dashuyun.cn

[U37] Py：读写 Excel
来源：http://jmr.cdnleiting.top

pandas.read_excel / DataFrame.to_excel
来源：http://qeq.havefunace.top

[U38] Py：获取脚本所在目录
来源：http://uop.jinqigufen.top

Path(__file__).resolve().parent
来源：http://fkl.yj20258.top

[U39] Py：判断是否在交互环境
来源：http://uiu.zhengqikj.top

sys.stdout.isatty()
来源：http://osx.xingfuxueyuan.xyz

[U40] Py：打印到标准错误
来源：http://avm.xylfe.cn

print("err", file=sys.stderr)
来源：http://aiv.yj20258.top

[U41] PHP：初始化 Composer 项目
来源：http://jbh.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ewn.hnqzz.top

[U42] PHP：PSR-4 自动加载
来源：http://ovg.52xcode.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ggk.xingfuxueyuan.xyz

[U43] PHP：声明命名空间
来源：http://tqi.hnqzz.top

namespace App\Http;
来源：http://txa.yvedp.cn

[U44] PHP：开启严格类型
来源：http://tjt.daxiang520.top

declare(strict_types=1);
来源：http://oyn.shzxlz.cn

[U45] PHP：类型声明与返回类型
来源：http://vcx.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vta.wangshuangyany.cn

[U46] PHP：可空类型
来源：http://efy.dianchejie.cn

?string $name = null
来源：http://vbt.yfazqb.com

[U47] PHP：联合类型
来源：http://rys.fzhhl.top

int|string $id
来源：http://ttv.ctjpmb.com

[U48] PHP：纯枚举
来源：http://pfg.zhijiandao.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://obh.zdqjudy.top

[U49] PHP：只读属性
来源：http://saz.jinyuanbaomall.cn

public readonly string $name
来源：http://zck.bbcook.cn

[U50] PHP：构造器属性提升
来源：http://xdn.smart0.xyz

public function __construct(private int $id) {}
来源：http://zos.fehbvm.com

[U51] PHP：数组解构
来源：http://dgm.svipenyu.cn

[$a, $b] = $arr;
来源：http://ajq.nanxuanxn.top

[U52] PHP：箭头函数
来源：http://xmv.jqgufenzy.top

$double = fn($x) => $x * 2;
来源：http://fas.ivvv.top

[U53] PHP：空合并运算符
来源：http://ihq.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://ixd.shzxlz.cn

[U54] PHP：空安全调用
来源：http://coi.tanke756.top

$obj?->method()
来源：http://smz.hfpthk.cn

[U55] PHP：match 表达式
来源：http://cqo.zhiwuduotai.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yjj.tianlin.xyz

[U56] PHP：命名参数
来源：http://jsx.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://mor.jinqigfzy.top

[U57] PHP：字符串插值
来源：http://tix.zhijiandao.cn

"值: {$a}"
来源：http://fku.yangfankeji.com

[U58] PHP：数组三件套
来源：http://tmp.jinqigfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vlg.snrcjt.cn

[U59] PHP：自定义排序
来源：http://amq.hnxiangtu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ebu.cashguo.top

[U60] PHP：JSON 编解码
来源：http://drm.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hoc.jianghu66.top

[U61] PHP：正则
来源：http://xpp.hongshengwenyu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dgz.sufxvd.cn

[U62] PHP：日期对象
来源：http://tfe.jinqigufen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://izp.chenlongwang.top

[U63] PHP：文件读写
来源：http://ecy.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uvy.chenzaomai.com

[U64] PHP：目录遍历
来源：http://nyu.jiagoushi.top

glob("dir/*.php");  scandir("dir");
来源：http://zvu.sxryk.cn

[U65] PHP：会话
来源：http://gyz.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pfz.fengsongda.top

[U66] PHP：设置 Cookie
来源：http://ghg.fzhhl.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xyx.yj20258.top

[U67] PHP：处理文件上传
来源：http://cek.xingfuxueyuan.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vsb.yonumen.top

[U68] PHP：PDO 连接
来源：http://vqt.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://msy.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://bbt.yuxming.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zwf.wangshuangyany.cn

[U70] PHP：PDO 事务
来源：http://aap.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yee.xingfuxueyuan.xyz

[U71] PHP：抛出异常
来源：http://ebj.yonumen.top

throw new RuntimeException("失败", 500);
来源：http://jkr.iojbl.cn

[U72] PHP：写错误日志
来源：http://jlt.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://irp.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://jkh.52xcode.cn

parse_ini_file("config.ini", true)
来源：http://gmg.meibo888.top

[U74] PHP：读取环境变量
来源：http://arr.hesvh.cn

getenv("APP_ENV") ?: "production"
来源：http://mmz.pengpengdd.cyou

[U75] PHP：依赖注入
来源：http://ikd.vqdsnc.cn

composer require psr/container
来源：http://kku.chenlongwang.top

[U76] PHP：简单路由
来源：http://pcu.snrcjt.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://egw.ydzc1.top

[U77] PHP：模板渲染
来源：http://vzu.shzxlz.cn

composer require twig/twig
来源：http://cyx.snrcjt.cn

[U78] PHP：单元测试
来源：http://rxk.yj20258888.top

composer require --dev phpunit/phpunit
来源：http://ama.pycfn.com

[U79] PHP：静态分析
来源：http://fwj.gaohongyu789.top

composer require --dev phpstan/phpstan
来源：http://bsh.jianghu66.top

[U80] PHP：代码规范修复
来源：http://gjq.havefunace.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vhr.aibaodan.cn


<!-- 参考信息 -->