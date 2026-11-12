代发 wailian999

[T03] Kotlin：字符串模板
来源：http://scm.quarkkingdee.top

"值: $b"
来源：http://wnw.chenlongwang.top

[T04] Kotlin：空安全
来源：http://uqe.zdqjudy.top

val n: String? = null;  n?.length
来源：http://fmk.bbcook.cn

[T05] Kotlin：when 表达式
来源：http://mhj.fanxiaobao.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vyh.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://dzt.ydjk.org.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hqv.wangdashe.top

[T07] Kotlin：集合过滤
来源：http://kfr.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qfz.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://rnc.yuxming.cn

data class User(val name: String, val age: Int)
来源：http://vld.zycfv.cn

[T09] Kotlin：扩展函数
来源：http://enm.yonumen.top

fun String.exclaim() = this + "!"
来源：http://wgr.xuetiantiany.cn

[T10] Kotlin：默认参数
来源：http://vyv.yueranfly.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pva.ybcxt.top

[T11] Kotlin：协程
来源：http://cyv.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://seh.jinqigufen.top

[T12] Kotlin：解构声明
来源：http://cio.ydzc1.top

val (a, b) = Pair(1, 2)
来源：http://dai.havefunace.top

[T13] Kotlin：只读 Map
来源：http://gco.yj202588.top

val m = mapOf("a" to 1)
来源：http://vbi.cashguo.top

[T14] Kotlin：循环
来源：http://dyb.havefunace.top

for (i in 1..10) println(i)
来源：http://icu.gogol.net.cn

[T15] Kotlin：接口
来源：http://ivw.nanxinkj.top

interface Shape { fun area(): Double }
来源：http://oob.gzhubu.top

[T16] Swift：Hello World
来源：http://qyx.birdmap.top

print("Hello")
来源：http://edy.bjfxy.top

[T17] Swift：变量与常量
来源：http://cnq.gaohongyu789.top

var a = 1;  let b = 2
来源：http://jia.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://pwe.hcnkem.com

"值: \(b)"
来源：http://wyu.ppjwa.cn

[T19] Swift：可选绑定
来源：http://lxs.9152youxi.cn

if let n = opt { print(n) }
来源：http://bna.jinyuanbaomall.cn

[T20] Swift：数组操作
来源：http://cxw.zhixingplan.top

var a = [1, 2, 3];  a.append(4)
来源：http://mwx.nanxinkj.top

[T21] Swift：遍历
来源：http://zmh.pycfn.com

for x in a { print(x) }
来源：http://mtf.fehbvm.com

[T22] Swift：字典
来源：http://zdr.havefunace.top

var d = ["a": 1];  d["b"] = 2
来源：http://dys.ehwqpu.com

[T23] Swift：函数
来源：http://tkc.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hln.shzxlz.cn

[T24] Swift：闭包
来源：http://uan.xziqi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ibu.zhengqikj.top

[T25] Swift：结构体
来源：http://rkb.ydjk.org.cn

struct P { var x: Int }
来源：http://nuv.shanyushiyangkeji.top

[T26] Swift：类与重写
来源：http://jqc.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://xxm.birdmap.top

[T27] Swift：错误处理
来源：http://cub.xylfe.cn

do { try f() } catch { print(error) }
来源：http://dpn.gogol.net.cn

[T28] Swift：枚举
来源：http://vdf.zhixingplan.top

enum Color { case red, green }
来源：http://rxq.ctjpmb.com

[T29] Swift：guard 提前返回
来源：http://hci.chenjidiqi.icu

guard let x = opt else { return }
来源：http://mry.epnwcf.com

[T30] Swift：协议
来源：http://gqb.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://hrr.yongpay.top

[T31] Lua：Hello World
来源：http://oep.sxryk.cn

print("Hello")
来源：http://mpv.fzhhl.top

[T32] Lua：局部变量
来源：http://bpt.snrcjt.cn

local a = 1
来源：http://gxm.jinqigufen.top

[T33] Lua：表（数组）
来源：http://xhv.jiagoushi.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rlw.gzhubu.top

[T34] Lua：遍历表
来源：http://ped.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lge.hnqzz.top

[T35] Lua：字典表
来源：http://hum.ywan-chungtsiang.top

local d = { a = 1 };  d.b = 2
来源：http://tpj.uphjek.com

[T36] Lua：函数
来源：http://kyz.jinqigufen.top

function add(a, b) return a + b end
来源：http://yoq.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://njp.gogol.net.cn

"a" .. "b"
来源：http://umz.jinqigfzy.top

[T38] Lua：条件
来源：http://fcs.tian-w.cn

if x > 0 then print("正") end
来源：http://ecy.jlsjyb.cn

[T39] Lua：模式匹配
来源：http://ahe.chenlongwang.top

string.find(s, "%d+")
来源：http://aoc.gaohongyu789.top

[T40] Lua：元表
来源：http://szq.tarul.cn

setmetatable({}, { __index = base })
来源：http://hiq.yueranfly.top

[T41] Perl：Hello World
来源：http://lzd.ywan-chungtsiang.top

print "Hello\n";
来源：http://qka.zhijiandao.cn

[T42] Perl：变量类型
来源：http://ypz.yangfankeji.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lmy.aizwys.cn

[T43] Perl：字符串插值
来源：http://qnk.ybcxt.top

"值: $a"
来源：http://hep.guannengcc.top

[T44] Perl：条件
来源：http://hxx.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://wos.bbcook.cn

[T45] Perl：数组遍历
来源：http://dib.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://qli.smart0.xyz

[T46] Perl：哈希操作
来源：http://ldx.zhaomingkeji.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wam.yj20258888.top

[T47] Perl：正则捕获
来源：http://vip.ivvv.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://llv.gotoacloud.top

[T48] Perl：正则替换
来源：http://rni.dashuyun.cn

$s =~ s/old/new/g;
来源：http://deb.ctjpmb.com

[T49] Perl：函数
来源：http://cdo.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://igm.cucudq.cn

[T50] Perl：逐行读文件
来源：http://zpi.guannengcc.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nqi.iojbl.cn

while (my $line = <$fh>) { print $line; }
来源：http://mwm.fehbvm.com

[T51] Scala：Hello World
来源：http://ess.gzhubu.top

println("Hello")
来源：http://dle.ivvv.top

[T52] Scala：变量
来源：http://qze.ydzc1.top

val a = 1;  var b = 2
来源：http://xcw.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://zkv.zhiwuduotai.top

s"值: $b"
来源：http://vrf.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://ece.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://dkm.havefunace.top

[T55] Scala：集合过滤
来源：http://kuh.kuanghao11.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xbo.ydzc1.top

[T56] Scala：样例类
来源：http://mvz.0kj1m.cn

case class User(name: String, age: Int)
来源：http://asi.9152youxi.cn

[T57] Scala：模式匹配
来源：http://bum.yvedp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://awa.xylfe.cn

[T58] Scala：函数定义
来源：http://vms.fengsongda.top

def add(a: Int, b: Int): Int = a + b
来源：http://ghb.nwbrower.top

[T59] Scala：循环
来源：http://ivw.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://hdg.chenjidiqi.icu

[T60] Scala：折叠
来源：http://mij.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pkh.yonumen.top

================================================================================
来源：http://nuq.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mvm.guannengcc.top

================================================================================
来源：http://efm.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://ibc.bjfxy.top

python -m venv .venv && source .venv/bin/activate
来源：http://mxz.sufxvd.cn

[U02] Py：导出 / 安装依赖
来源：http://sig.sufxvd.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ujk.yanxiufei.cn

[U03] Py：加载 .env 配置
来源：http://zqm.sysykeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ppo.yj20258.top

[U04] Py：变量调试打印
来源：http://eym.xingfuxueyuan.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qws.316326.xyz

[U05] Py：列表去重且保序
来源：http://ciu.xziqi.cn

list(dict.fromkeys(arr))
来源：http://pfh.daria6918.cn

[U06] Py：合并两个字典
来源：http://ttw.haohaochexian.top

{**a, **b}
来源：http://kgx.cheryme.top

[U07] Py：反转字典键值
来源：http://ayt.yj202588.top

{v: k for k, v in d.items()}
来源：http://mtu.hnxiangtu.top

[U08] Py：展平二维列表
来源：http://afv.guannengcc.top

[y for x in nested for y in x]
来源：http://grx.cheryme.top

[U09] Py：字典取最大值的键
来源：http://iao.jqgufenzy.top

max(d, key=d.get)
来源：http://wua.sxryk.cn

[U10] Py：按值排序字典
来源：http://prv.jqgufenzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eyu.zhaomingkeji.xyz

[U11] Py：生成器表达式
来源：http://nmm.ybcxt.top

(x * 2 for x in arr)
来源：http://fya.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fln.yuxming.cn

Counter(arr).most_common(3)
来源：http://qwv.quarkkingdee.top

[U13] Py：固定长度队列
来源：http://add.cashguo.top

deque(maxlen=10)
来源：http://yas.ydzc1.top

[U14] Py：分组收集到列表
来源：http://tdi.zhijiandao.cn

defaultdict(list)
来源：http://nzq.kuanghao11.cn

[U15] Py：高精度计时
来源：http://tkh.guowangkeji.top

t = time.perf_counter()
来源：http://oqt.shuidangran.top

[U16] Py：命令行参数解析
来源：http://oat.hysaishi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ckd.nanxinkj.top

[U17] Py：初始化日志
来源：http://snt.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://dum.wangshuangyany.cn

[U18] Py：预编译正则
来源：http://lww.ybcxt.top

pat = re.compile(r"\d+")
来源：http://dli.nanxuanxn.top

[U19] Py：正则替换带回调
来源：http://ewo.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://veo.fktsv.cn

[U20] Py：缓存函数结果
来源：http://bow.fengsongda.top

@functools.lru_cache(maxsize=None)
来源：http://pho.tianlin.xyz

[U21] Py：自定义上下文管理器
来源：http://fss.bjfxy.top

@contextlib.contextmanager
来源：http://lue.hywenlv.cn

[U22] Py：矩阵转置
来源：http://zqk.sweek.top

list(zip(*m))
来源：http://oki.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://hbs.yanxiufei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ggf.svipenyu.cn

[U24] Py：路径操作
来源：http://sdp.fengsongda.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://opb.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://eto.jinyuanbaomall.cn

csv.DictReader(f)
来源：http://sub.hfpthk.cn

[U26] Py：并发下载
来源：http://abq.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mho.zhaomingkeji.xyz

[U27] Py：异步 HTTP
来源：http://ifv.nanxuanxn.top

aiohttp.ClientSession() 配合 async with
来源：http://xzd.xylfe.cn

[U28] Py：类型别名
来源：http://mst.xziqi.cn

UserId = int
来源：http://cdu.52xcode.cn

[U29] Py：属性校验
来源：http://jim.mhx1999.top

@property 与 @x.setter 配合
来源：http://oek.fzhhl.top

[U30] Py：数据类
来源：http://wif.daria6918.cn

@dataclass(slots=True)
来源：http://gxv.yvedp.cn

[U31] Py：单测
来源：http://xql.xinyue.icu

python -m pytest -q
来源：http://cai.hfpthk.cn

[U32] Py：代码格式化
来源：http://kbh.vehdjk.com

ruff format . && ruff check --fix .
来源：http://onm.jinghuilouyu.cn

[U33] Py：打包发布
来源：http://tku.kuanghao11.cn

python -m build  （依赖 pyproject.toml）
来源：http://ksl.zhixingplan.top

[U34] Py：判断编码
来源：http://kvu.c1oappe.top

chardet.detect(raw)
来源：http://umn.52xcode.cn

[U35] Py：发送邮件
来源：http://xkl.andypj.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cvn.ehwqpu.com

[U36] Py：定时任务
来源：http://jlb.wangdashe.top

schedule.every(10).minutes.do(job)
来源：http://jco.guowangkeji.top

[U37] Py：读写 Excel
来源：http://xhp.zdbjq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cac.havefunace.top

[U38] Py：获取脚本所在目录
来源：http://afz.svipenyu.cn

Path(__file__).resolve().parent
来源：http://ort.haohaochexian.top

[U39] Py：判断是否在交互环境
来源：http://drl.yfazqb.com

sys.stdout.isatty()
来源：http://tad.mhx1999.top

[U40] Py：打印到标准错误
来源：http://kcc.daria6918.cn

print("err", file=sys.stderr)
来源：http://wfx.fktsv.cn

[U41] PHP：初始化 Composer 项目
来源：http://bii.ctjpmb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://uge.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://tit.ppjwa.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://npy.nwbrower.top

[U43] PHP：声明命名空间
来源：http://fol.9152youxi.cn

namespace App\Http;
来源：http://rye.daria6918.cn

[U44] PHP：开启严格类型
来源：http://tpc.tian-w.cn

declare(strict_types=1);
来源：http://hfu.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://kuf.fehbvm.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://kms.nwbrower.top

[U46] PHP：可空类型
来源：http://bbi.quarkkingdee.top

?string $name = null
来源：http://xum.gotoacloud.top

[U47] PHP：联合类型
来源：http://pij.tianlin.xyz

int|string $id
来源：http://lpg.jianghu66.top

[U48] PHP：纯枚举
来源：http://qhq.nanxuanxn.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ssj.0kj1m.cn

[U49] PHP：只读属性
来源：http://kza.epnwcf.com

public readonly string $name
来源：http://sqn.guowangkeji.top

[U50] PHP：构造器属性提升
来源：http://umu.jinyuanbaomall.cn

public function __construct(private int $id) {}
来源：http://sql.dianchejie.cn

[U51] PHP：数组解构
来源：http://slz.jqgufenzy.top

[$a, $b] = $arr;
来源：http://qiq.fktsv.cn

[U52] PHP：箭头函数
来源：http://bai.jianghu66.top

$double = fn($x) => $x * 2;
来源：http://lyx.pycfn.com

[U53] PHP：空合并运算符
来源：http://glk.chenjidiqi.icu

$v = $a ?? $b ?? "default";
来源：http://ccw.dashuyun.cn

[U54] PHP：空安全调用
来源：http://jch.gaohongyu789.top

$obj?->method()
来源：http://xfv.ppjwa.cn

[U55] PHP：match 表达式
来源：http://roc.pengpengdd.cyou

$s = match($x) { 1 => "一", default => "其他" };
来源：http://efl.52xcode.cn

[U56] PHP：命名参数
来源：http://lpy.shanyushiyangtech.top

f(a: 1, b: 2)
来源：http://utd.jinghuilouyu.cn

[U57] PHP：字符串插值
来源：http://vlk.daxiang520.top

"值: {$a}"
来源：http://zmp.ybcxt.top

[U58] PHP：数组三件套
来源：http://rms.mhx1999.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qga.xylfe.cn

[U59] PHP：自定义排序
来源：http://fwd.redwolf501.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bly.ydjk.org.cn

[U60] PHP：JSON 编解码
来源：http://dms.daxiang520.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sri.shanyushiyangkeji.top

[U61] PHP：正则
来源：http://fpa.chenjidiqi.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lil.jinghuilouyu.cn

[U62] PHP：日期对象
来源：http://jms.tian-w.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nbd.hfpthk.cn

[U63] PHP：文件读写
来源：http://zmk.haohaochexian.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jap.xylfe.cn

[U64] PHP：目录遍历
来源：http://sxb.shangyingyoupin.top

glob("dir/*.php");  scandir("dir");
来源：http://pus.fanxiaobao.xyz

[U65] PHP：会话
来源：http://mqp.yvedp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rdi.sweek.top

[U66] PHP：设置 Cookie
来源：http://bvd.yuanzhike.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vms.cheryme.top

[U67] PHP：处理文件上传
来源：http://gxo.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cnx.feifeiyinyue.top

[U68] PHP：PDO 连接
来源：http://vyh.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ftl.xylfe.cn

[U69] PHP：PDO 预处理
来源：http://wxj.birdmap.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cak.yuxming.cn

[U70] PHP：PDO 事务
来源：http://wkm.yj20258.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bkl.jqgfzy.top

[U71] PHP：抛出异常
来源：http://cwq.bbcook.cn

throw new RuntimeException("失败", 500);
来源：http://qvb.yj20258888.top

[U72] PHP：写错误日志
来源：http://caz.sjlbkw.cn

error_log("失败: " . $e->getMessage());
来源：http://nmu.yfazqb.com

[U73] PHP：读取 ini 配置
来源：http://uau.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://mkk.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://mfl.ppjwa.cn

getenv("APP_ENV") ?: "production"
来源：http://qtw.jinyuanbaomall.cn

[U75] PHP：依赖注入
来源：http://oad.9152youxi.cn

composer require psr/container
来源：http://zsp.zhijiandao.cn

[U76] PHP：简单路由
来源：http://oyu.52xcode.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gbg.havefunace.top

[U77] PHP：模板渲染
来源：http://kbl.0kj1m.cn

composer require twig/twig
来源：http://gyc.andypj.xyz

[U78] PHP：单元测试
来源：http://xpx.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://jnt.jinqigfzy.top

[U79] PHP：静态分析
来源：http://ppp.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://qbt.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://syt.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://prg.guowangkeji.top

[U81] JS：初始化项目
来源：http://vne.tarul.cn

npm init -y;  npm i express
来源：http://luh.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://vrb.yj20258.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tyq.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://ddu.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cvk.ivvv.top

[U84] JS：CommonJS 写法
来源：http://phl.jqgfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://frh.ehwqpu.com

[U85] JS：可选链
来源：http://jcu.ybcxt.top

a?.b?.c
来源：http://fwk.ppjwa.cn

[U86] JS：空值合并
来源：http://geh.dashuyun.cn

a ?? b
来源：http://cwb.epnwcf.com

[U87] JS：解构默认值
来源：http://blg.fengsongda.top

const { a = 1, b = 2 } = obj;
来源：http://nkc.vehdjk.com

[U88] JS：对象展开合并
来源：http://tsa.havefunace.top

{ ...a, ...b }
来源：http://iyy.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://oer.jinyuanbaomall.cn

[...new Set(arr)]
来源：http://pdx.gogol.net.cn

[U90] JS：数字数组排序
来源：http://pap.c1oappe.top

[...arr].sort((a, b) => a - b)
来源：http://ikb.ydjk.org.cn


<!-- 参考信息 -->