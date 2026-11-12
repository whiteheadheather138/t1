代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://kgv.bbcook.cn

[S59] C++：静态断言
来源：http://lsr.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fzh.shanyushiyangtech.top

[S60] C++：遍历并删除元素
来源：http://eel.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pzu.redwolf501.top

================================================================================
来源：http://edm.hnqzz.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gac.kuanghao11.cn

================================================================================
来源：http://mde.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://frh.shuidangran.top

println("Hello")
来源：http://hfq.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://gyp.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xqd.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://pdb.tianlin.xyz

"值: $b"
来源：http://tlf.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://yub.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://xio.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://fkf.tianlin.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wmj.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://dhz.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ppn.tarul.cn

[T07] Kotlin：集合过滤
来源：http://gpu.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pmc.cheryme.top

[T08] Kotlin：数据类
来源：http://hgj.wangdashe.top

data class User(val name: String, val age: Int)
来源：http://eko.yuanzhike.top

[T09] Kotlin：扩展函数
来源：http://clm.cashguo.top

fun String.exclaim() = this + "!"
来源：http://vwn.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://gmu.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fkm.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://bgu.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gnz.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://goi.gzhubu.top

val (a, b) = Pair(1, 2)
来源：http://prf.yonumen.top

[T13] Kotlin：只读 Map
来源：http://lcg.fengsongda.top

val m = mapOf("a" to 1)
来源：http://oby.jinqigufen.top

[T14] Kotlin：循环
来源：http://ctq.xylfe.cn

for (i in 1..10) println(i)
来源：http://llc.aibaodan.cn

[T15] Kotlin：接口
来源：http://moo.epnwcf.com

interface Shape { fun area(): Double }
来源：http://wdm.cheryme.top

[T16] Swift：Hello World
来源：http://wsr.ywan-chungtsiang.top

print("Hello")
来源：http://sgq.meibo888.top

[T17] Swift：变量与常量
来源：http://xti.cucudq.cn

var a = 1;  let b = 2
来源：http://xhg.pycfn.com

[T18] Swift：字符串插值
来源：http://jre.jiagoushi.top

"值: \(b)"
来源：http://hji.316326.xyz

[T19] Swift：可选绑定
来源：http://xwu.yj202588.top

if let n = opt { print(n) }
来源：http://jee.hnqzz.top

[T20] Swift：数组操作
来源：http://dnx.jlsjyb.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fjv.shzxlz.cn

[T21] Swift：遍历
来源：http://ynz.bbcook.cn

for x in a { print(x) }
来源：http://bbi.cucudq.cn

[T22] Swift：字典
来源：http://kno.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mde.redwolf501.top

[T23] Swift：函数
来源：http://tlq.wangdashe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kts.sysykeji.top

[T24] Swift：闭包
来源：http://jvu.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://byd.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://pmh.chenzaomai.com

struct P { var x: Int }
来源：http://vnp.jianghu66.top

[T26] Swift：类与重写
来源：http://xux.hnxiangtu.top

class A: Base { override func f() {} }
来源：http://fit.jqgufenzy.top

[T27] Swift：错误处理
来源：http://wvr.ydzc1.top

do { try f() } catch { print(error) }
来源：http://ypc.gzhubu.top

[T28] Swift：枚举
来源：http://zbu.hnqzz.top

enum Color { case red, green }
来源：http://fdx.bjfxy.top

[T29] Swift：guard 提前返回
来源：http://qva.pycfn.com

guard let x = opt else { return }
来源：http://yee.wangdashe.top

[T30] Swift：协议
来源：http://jjh.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://rzv.zhengqikj.top

[T31] Lua：Hello World
来源：http://pgr.yj20258.top

print("Hello")
来源：http://zbr.ydjk.org.cn

[T32] Lua：局部变量
来源：http://wfn.jinqigufen.top

local a = 1
来源：http://wpf.gogol.net.cn

[T33] Lua：表（数组）
来源：http://gdc.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lmu.feifeiyinyue.top

[T34] Lua：遍历表
来源：http://umw.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://sgh.chenjidiqi.icu

[T35] Lua：字典表
来源：http://ulm.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://dgi.jqgfzy.top

[T36] Lua：函数
来源：http://ooq.hnqzz.top

function add(a, b) return a + b end
来源：http://sql.yuxming.cn

[T37] Lua：字符串拼接
来源：http://frj.shuidangran.top

"a" .. "b"
来源：http://gko.zhengqikj.top

[T38] Lua：条件
来源：http://ste.hammf.cn

if x > 0 then print("正") end
来源：http://tcb.svipenyu.cn

[T39] Lua：模式匹配
来源：http://owr.yangfankeji.com

string.find(s, "%d+")
来源：http://zrn.dianchejie.cn

[T40] Lua：元表
来源：http://pdi.ydjk.org.cn

setmetatable({}, { __index = base })
来源：http://naf.hfpthk.cn

[T41] Perl：Hello World
来源：http://vzp.nanxinkj.top

print "Hello\n";
来源：http://amk.quarkkingdee.top

[T42] Perl：变量类型
来源：http://vjo.hongshengwenyu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dpv.epnwcf.com

[T43] Perl：字符串插值
来源：http://dbz.xylfe.cn

"值: $a"
来源：http://azf.jyoumei.cn

[T44] Perl：条件
来源：http://kdz.kuanghao11.cn

if ($a > 0) { print "正"; }
来源：http://xsj.fzhhl.top

[T45] Perl：数组遍历
来源：http://lxp.guannengcc.top

for my $x (@arr) { print $x; }
来源：http://bwd.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://gko.0kj1m.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://udy.nanxinkj.top

[T47] Perl：正则捕获
来源：http://qjb.9152youxi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://csb.hywenlv.cn

[T48] Perl：正则替换
来源：http://dch.yuxming.cn

$s =~ s/old/new/g;
来源：http://rua.vehdjk.com

[T49] Perl：函数
来源：http://vyh.nwbrower.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cmq.smart0.xyz

[T50] Perl：逐行读文件
来源：http://gsy.snrcjt.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://euo.yonumen.top

while (my $line = <$fh>) { print $line; }
来源：http://sdn.aizwys.cn

[T51] Scala：Hello World
来源：http://jgf.guannengcc.top

println("Hello")
来源：http://swj.gotoacloud.top

[T52] Scala：变量
来源：http://lxi.52xcode.cn

val a = 1;  var b = 2
来源：http://ozc.pengpengdd.cyou

[T53] Scala：字符串插值
来源：http://lwn.yj20258888.top

s"值: $b"
来源：http://mje.xuanzx.com

[T54] Scala：集合映射
来源：http://nth.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://fxk.yonumen.top

[T55] Scala：集合过滤
来源：http://dxe.guannengcc.top

List(1, 2, 3).filter(_ > 1)
来源：http://nwc.fehbvm.com

[T56] Scala：样例类
来源：http://igd.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://ylc.c1oappe.top

[T57] Scala：模式匹配
来源：http://ybg.meibo888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://huc.jqgufenzy.top

[T58] Scala：函数定义
来源：http://jiv.daria6918.cn

def add(a: Int, b: Int): Int = a + b
来源：http://enn.iojbl.cn

[T59] Scala：循环
来源：http://boz.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://xdv.pengpengdd.cyou

[T60] Scala：折叠
来源：http://vbg.mhx1999.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://phn.uphjek.com

================================================================================
来源：http://lfy.yonumen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jeg.dianchejie.cn

================================================================================
来源：http://xnj.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://hwm.haohaochexian.top

python -m venv .venv && source .venv/bin/activate
来源：http://ade.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://med.fanxiaobao.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xet.zhoulong.xyz

[U03] Py：加载 .env 配置
来源：http://ixv.jqgufenzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pjb.gaohongyu789.top

[U04] Py：变量调试打印
来源：http://cfu.hnxiangtu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://guz.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://bpd.gzhubu.top

list(dict.fromkeys(arr))
来源：http://hrb.hesvh.cn

[U06] Py：合并两个字典
来源：http://grk.cucudq.cn

{**a, **b}
来源：http://hkn.hongshengwenyu.top

[U07] Py：反转字典键值
来源：http://tak.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://tnq.tianlin.xyz

[U08] Py：展平二维列表
来源：http://fgx.gaohongyu789.top

[y for x in nested for y in x]
来源：http://xvn.zhixingplan.top

[U09] Py：字典取最大值的键
来源：http://ugb.yanxiufei.cn

max(d, key=d.get)
来源：http://dct.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://llw.gaohongyu789.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iam.sysykeji.top

[U11] Py：生成器表达式
来源：http://tda.daxiang520.top

(x * 2 for x in arr)
来源：http://fdd.shangyingyoupin.top

[U12] Py：取出现最多的 3 个元素
来源：http://ppm.hywenlv.cn

Counter(arr).most_common(3)
来源：http://znn.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://hde.yj202588.top

deque(maxlen=10)
来源：http://wdm.hammf.cn

[U14] Py：分组收集到列表
来源：http://tls.yanxiufei.cn

defaultdict(list)
来源：http://fwe.cdnleiting.top

[U15] Py：高精度计时
来源：http://zdk.ctjpmb.com

t = time.perf_counter()
来源：http://lwn.yvedp.cn

[U16] Py：命令行参数解析
来源：http://nha.aizwys.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wex.zdbjq.cn

[U17] Py：初始化日志
来源：http://fot.sufxvd.cn

logging.basicConfig(level=logging.INFO)
来源：http://dvp.fzhhl.top

[U18] Py：预编译正则
来源：http://ybi.yj202588.top

pat = re.compile(r"\d+")
来源：http://aib.zhixingplan.top

[U19] Py：正则替换带回调
来源：http://tzh.hnqzz.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uei.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://nzz.cqqwz.cn

@functools.lru_cache(maxsize=None)
来源：http://jyv.hnqzz.top

[U21] Py：自定义上下文管理器
来源：http://dnv.dianchejie.cn

@contextlib.contextmanager
来源：http://zxr.hammf.cn

[U22] Py：矩阵转置
来源：http://lgz.gaohongyu789.top

list(zip(*m))
来源：http://bck.jianghu66.top

[U23] Py：分块读取大文件
来源：http://jxx.pengpengdd.cyou

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wta.havefunace.top

[U24] Py：路径操作
来源：http://bmn.quarkkingdee.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uek.hammf.cn

[U25] Py：CSV 按字典读
来源：http://hpg.yj20258.top

csv.DictReader(f)
来源：http://ycf.meibo888.top

[U26] Py：并发下载
来源：http://rmt.hfpthk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yns.cdnleiting.top

[U27] Py：异步 HTTP
来源：http://hye.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://xzo.0kj1m.cn

[U28] Py：类型别名
来源：http://kyw.zhengqikj.top

UserId = int
来源：http://gyi.aibaodan.cn

[U29] Py：属性校验
来源：http://dfv.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://onh.andypj.xyz

[U30] Py：数据类
来源：http://wmd.guowangkeji.top

@dataclass(slots=True)
来源：http://kpp.haohaochexian.top

[U31] Py：单测
来源：http://bxe.yanxiufei.cn

python -m pytest -q
来源：http://wct.hfpthk.cn

[U32] Py：代码格式化
来源：http://fqu.yueranfly.top

ruff format . && ruff check --fix .
来源：http://wfz.ivvv.top

[U33] Py：打包发布
来源：http://vnz.ywan-chungtsiang.top

python -m build  （依赖 pyproject.toml）
来源：http://yix.nanxuanxn.top

[U34] Py：判断编码
来源：http://vug.ydzc1.top

chardet.detect(raw)
来源：http://hoy.yj20258.top

[U35] Py：发送邮件
来源：http://lsj.ctjpmb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gdu.jinghuilouyu.cn

[U36] Py：定时任务
来源：http://avs.fengsongda.top

schedule.every(10).minutes.do(job)
来源：http://hjs.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://cyg.tarul.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lzu.zdqjudy.top

[U38] Py：获取脚本所在目录
来源：http://gyw.hnqzz.top

Path(__file__).resolve().parent
来源：http://nkh.gaohongyu789.top

[U39] Py：判断是否在交互环境
来源：http://lkx.jyoumei.cn

sys.stdout.isatty()
来源：http://ppu.jyoumei.cn

[U40] Py：打印到标准错误
来源：http://vhl.haohaochexian.top

print("err", file=sys.stderr)
来源：http://rop.xingfuxueyuan.xyz

[U41] PHP：初始化 Composer 项目
来源：http://wwu.hesvh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://djm.yuanzhike.top

[U42] PHP：PSR-4 自动加载
来源：http://izf.jianghu66.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pou.jinyuanbaomall.cn

[U43] PHP：声明命名空间
来源：http://vsm.nwbrower.top

namespace App\Http;
来源：http://cpq.sysykeji.top

[U44] PHP：开启严格类型
来源：http://plg.cheryme.top

declare(strict_types=1);
来源：http://nhw.jqgufenzy.top

[U45] PHP：类型声明与返回类型
来源：http://rog.fzhhl.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pjh.52xcode.cn

[U46] PHP：可空类型
来源：http://dss.tianlin.xyz

?string $name = null
来源：http://kcs.svipenyu.cn

[U47] PHP：联合类型
来源：http://igz.andypj.xyz

int|string $id
来源：http://sdz.hammf.cn

[U48] PHP：纯枚举
来源：http://vxb.yj20258.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yct.nanxuanxn.top

[U49] PHP：只读属性
来源：http://xpm.hesvh.cn

public readonly string $name
来源：http://mus.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://pgk.gaohongyu789.top

public function __construct(private int $id) {}
来源：http://lun.feifeiyinyue.top

[U51] PHP：数组解构
来源：http://jye.jiagoushi.top

[$a, $b] = $arr;
来源：http://qbx.mhx1999.top

[U52] PHP：箭头函数
来源：http://qeh.vehdjk.com

$double = fn($x) => $x * 2;
来源：http://wgz.316326.xyz

[U53] PHP：空合并运算符
来源：http://dig.dashuyun.cn

$v = $a ?? $b ?? "default";
来源：http://dan.xziqi.cn

[U54] PHP：空安全调用
来源：http://dig.jqgufenzy.top

$obj?->method()
来源：http://zoz.aizwys.cn

[U55] PHP：match 表达式
来源：http://jbv.mhx1999.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dge.sxryk.cn

[U56] PHP：命名参数
来源：http://waq.fanxiaobao.xyz

f(a: 1, b: 2)
来源：http://mqq.yanxiufei.cn

[U57] PHP：字符串插值
来源：http://fij.hcnkem.com

"值: {$a}"
来源：http://zkw.jlsjyb.cn

[U58] PHP：数组三件套
来源：http://tgt.hywenlv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gpx.hcnkem.com

[U59] PHP：自定义排序
来源：http://fxa.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://azw.yanxiufei.cn

[U60] PHP：JSON 编解码
来源：http://age.ybcxt.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jwu.hongshengwenyu.top

[U61] PHP：正则
来源：http://moi.ppjwa.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wgo.iojbl.cn

[U62] PHP：日期对象
来源：http://noo.wangshuangyany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hzv.snrcjt.cn

[U63] PHP：文件读写
来源：http://tis.cdnleiting.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qiz.yongpay.top

[U64] PHP：目录遍历
来源：http://dqc.jiagoushi.top

glob("dir/*.php");  scandir("dir");
来源：http://vhi.fanxiaobao.xyz

[U65] PHP：会话
来源：http://hce.cqqwz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zso.jinqigfzy.top

[U66] PHP：设置 Cookie
来源：http://wgp.jyoumei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aec.xylfe.cn

[U67] PHP：处理文件上传
来源：http://pra.fzhhl.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nfn.dianchejie.cn

[U68] PHP：PDO 连接
来源：http://abt.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://owu.yj202588.top

[U69] PHP：PDO 预处理
来源：http://mwg.meibo888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oue.hcnkem.com

[U70] PHP：PDO 事务
来源：http://cvm.xinyue.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gjv.hesvh.cn

[U71] PHP：抛出异常
来源：http://eiu.pengpengdd.cyou

throw new RuntimeException("失败", 500);
来源：http://iud.jinghuilouyu.cn

[U72] PHP：写错误日志
来源：http://okb.sysykeji.top

error_log("失败: " . $e->getMessage());
来源：http://xef.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://dxs.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://dyv.yueranfly.top

[U74] PHP：读取环境变量
来源：http://ydu.sysykeji.top

getenv("APP_ENV") ?: "production"
来源：http://tco.sweek.top

[U75] PHP：依赖注入
来源：http://mqw.jiagoushi.top

composer require psr/container
来源：http://tog.shanyushiyangtech.top

[U76] PHP：简单路由
来源：http://jkf.sjlbkw.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ynt.hcnkem.com

[U77] PHP：模板渲染
来源：http://wsm.jyoumei.cn

composer require twig/twig
来源：http://viu.tianlin.xyz

[U78] PHP：单元测试
来源：http://mrc.gzhubu.top

composer require --dev phpunit/phpunit
来源：http://awx.sysykeji.top

[U79] PHP：静态分析
来源：http://quf.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://hik.gogol.net.cn

[U80] PHP：代码规范修复
来源：http://tgt.fzhhl.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ehc.cqqwz.cn

[U81] JS：初始化项目
来源：http://qbl.aibaodan.cn

npm init -y;  npm i express
来源：http://ged.ybcxt.top

[U82] JS：package.json 脚本
来源：http://fdc.wangdashe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xlu.feifeiyinyue.top

[U83] JS：ES Module 导入导出
来源：http://osl.ppjwa.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vyr.zhoulong.xyz

[U84] JS：CommonJS 写法
来源：http://nvg.yuanzhike.top

module.exports = { a };  const { a } = require("./m");
来源：http://jbj.nwbrower.top


<!-- 参考信息 -->