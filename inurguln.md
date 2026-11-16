代发 wailian999

[T23] Swift：函数
来源：http://tvh.zycfv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dfd.0kj1m.cn

[T24] Swift：闭包
来源：http://gbx.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lqu.jlsjyb.cn

[T25] Swift：结构体
来源：http://nwg.cdnleiting.top

struct P { var x: Int }
来源：http://zcd.sufxvd.cn

[T26] Swift：类与重写
来源：http://mxv.nanxuanxn.top

class A: Base { override func f() {} }
来源：http://dlm.havefunace.top

[T27] Swift：错误处理
来源：http://vlh.hnqzz.top

do { try f() } catch { print(error) }
来源：http://suu.vqdsnc.cn

[T28] Swift：枚举
来源：http://nay.iojbl.cn

enum Color { case red, green }
来源：http://yac.quarkkingdee.top

[T29] Swift：guard 提前返回
来源：http://fdr.cheryme.top

guard let x = opt else { return }
来源：http://emi.yfazqb.com

[T30] Swift：协议
来源：http://ffc.zhijiandao.cn

protocol Shape { func area() -> Double }
来源：http://rsm.nwbrower.top

[T31] Lua：Hello World
来源：http://leq.zhongyouzk.top

print("Hello")
来源：http://shy.jianghu66.top

[T32] Lua：局部变量
来源：http://fpb.zycfv.cn

local a = 1
来源：http://gpe.vehdjk.com

[T33] Lua：表（数组）
来源：http://ims.aizwys.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rxc.ehwqpu.com

[T34] Lua：遍历表
来源：http://duo.ybcxt.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ysb.ivvv.top

[T35] Lua：字典表
来源：http://pyy.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://ama.yj20258888.top

[T36] Lua：函数
来源：http://yqv.uphjek.com

function add(a, b) return a + b end
来源：http://bty.sjlbkw.cn

[T37] Lua：字符串拼接
来源：http://iaw.hongshengwenyu.top

"a" .. "b"
来源：http://bbu.vehdjk.com

[T38] Lua：条件
来源：http://owb.sxryk.cn

if x > 0 then print("正") end
来源：http://ake.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://tog.tanke756.top

string.find(s, "%d+")
来源：http://itr.mhx1999.top

[T40] Lua：元表
来源：http://edp.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://urs.vqdsnc.cn

[T41] Perl：Hello World
来源：http://csk.andypj.xyz

print "Hello\n";
来源：http://szi.nanxinkj.top

[T42] Perl：变量类型
来源：http://vlk.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jyl.nanxinkj.top

[T43] Perl：字符串插值
来源：http://fht.wangshuangyany.cn

"值: $a"
来源：http://rkk.shangyingyoupin.top

[T44] Perl：条件
来源：http://ujl.hywenlv.cn

if ($a > 0) { print "正"; }
来源：http://nqs.nanxinkj.top

[T45] Perl：数组遍历
来源：http://cke.shzxlz.cn

for my $x (@arr) { print $x; }
来源：http://yfx.yj20258.top

[T46] Perl：哈希操作
来源：http://gzl.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dxc.xingfuxueyuan.xyz

[T47] Perl：正则捕获
来源：http://hsu.cdnleiting.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://anr.bjfxy.top

[T48] Perl：正则替换
来源：http://tcl.bbcook.cn

$s =~ s/old/new/g;
来源：http://urm.gotoacloud.top

[T49] Perl：函数
来源：http://rrd.vqdsnc.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vcm.fengsongda.top

[T50] Perl：逐行读文件
来源：http://cbo.yanxiufei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tgc.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://fhr.jinyuanbaomall.cn

[T51] Scala：Hello World
来源：http://mrc.sxryk.cn

println("Hello")
来源：http://gzk.smart0.xyz

[T52] Scala：变量
来源：http://ewn.yanxiufei.cn

val a = 1;  var b = 2
来源：http://qgy.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://iaz.gogol.net.cn

s"值: $b"
来源：http://url.tianlin.xyz

[T54] Scala：集合映射
来源：http://cve.yonumen.top

List(1, 2, 3).map(_ * 2)
来源：http://pwu.yfazqb.com

[T55] Scala：集合过滤
来源：http://yez.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://vej.yonumen.top

[T56] Scala：样例类
来源：http://obs.jinyuanbaomall.cn

case class User(name: String, age: Int)
来源：http://rba.ybcxt.top

[T57] Scala：模式匹配
来源：http://nrv.zdbjq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://chg.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://zwd.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://fgk.guannengcc.top

[T59] Scala：循环
来源：http://pbd.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://tdb.cheryme.top

[T60] Scala：折叠
来源：http://vwq.tanke756.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vtj.yuanzhike.top

================================================================================
来源：http://lrh.birdmap.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kyx.smart0.xyz

================================================================================
来源：http://tvn.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://yvt.hongshengwenyu.top

python -m venv .venv && source .venv/bin/activate
来源：http://xsd.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://ftt.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dly.ivvv.top

[U03] Py：加载 .env 配置
来源：http://hgs.dashuyun.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://thb.shuidangran.top

[U04] Py：变量调试打印
来源：http://zrn.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://upz.xylfe.cn

[U05] Py：列表去重且保序
来源：http://xue.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://fqy.cqqwz.cn

[U06] Py：合并两个字典
来源：http://ara.sysykeji.top

{**a, **b}
来源：http://hbe.bbcook.cn

[U07] Py：反转字典键值
来源：http://ddn.yfazqb.com

{v: k for k, v in d.items()}
来源：http://qnm.xuetiantiany.cn

[U08] Py：展平二维列表
来源：http://xqz.zhijiandao.cn

[y for x in nested for y in x]
来源：http://ted.quarkkingdee.top

[U09] Py：字典取最大值的键
来源：http://nab.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://pkb.snrcjt.cn

[U10] Py：按值排序字典
来源：http://gxh.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sxw.svipenyu.cn

[U11] Py：生成器表达式
来源：http://phk.yj202588.top

(x * 2 for x in arr)
来源：http://xxf.ctjpmb.com

[U12] Py：取出现最多的 3 个元素
来源：http://fuf.cheryme.top

Counter(arr).most_common(3)
来源：http://xro.zycfv.cn

[U13] Py：固定长度队列
来源：http://iyy.gotoacloud.top

deque(maxlen=10)
来源：http://mhp.andypj.xyz

[U14] Py：分组收集到列表
来源：http://qat.aibaodan.cn

defaultdict(list)
来源：http://bmu.haohaochexian.top

[U15] Py：高精度计时
来源：http://vhl.iojbl.cn

t = time.perf_counter()
来源：http://ood.epnwcf.com

[U16] Py：命令行参数解析
来源：http://jlj.sweek.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bcf.pengpengdd.cyou

[U17] Py：初始化日志
来源：http://bvg.cdnleiting.top

logging.basicConfig(level=logging.INFO)
来源：http://lub.xinyue.icu

[U18] Py：预编译正则
来源：http://tmw.sjlbkw.cn

pat = re.compile(r"\d+")
来源：http://bzt.iojbl.cn

[U19] Py：正则替换带回调
来源：http://ngg.pengpengdd.cyou

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oeb.kuanghao11.cn

[U20] Py：缓存函数结果
来源：http://uaj.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://wmk.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://hua.hammf.cn

@contextlib.contextmanager
来源：http://yzh.uphjek.com

[U22] Py：矩阵转置
来源：http://bjq.aibaodan.cn

list(zip(*m))
来源：http://mja.meibo888.top

[U23] Py：分块读取大文件
来源：http://dxz.hongshengwenyu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pxt.kuanghao11.cn

[U24] Py：路径操作
来源：http://kxd.yj202588.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zsg.yfazqb.com

[U25] Py：CSV 按字典读
来源：http://mwo.sysykeji.top

csv.DictReader(f)
来源：http://gde.snrcjt.cn

[U26] Py：并发下载
来源：http://nqe.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ohd.sweek.top

[U27] Py：异步 HTTP
来源：http://hsy.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://hhb.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://zwg.fengsongda.top

UserId = int
来源：http://ezi.zdbjq.cn

[U29] Py：属性校验
来源：http://etj.ppjwa.cn

@property 与 @x.setter 配合
来源：http://twx.cdnleiting.top

[U30] Py：数据类
来源：http://trv.hnxiangtu.top

@dataclass(slots=True)
来源：http://nhy.uphjek.com

[U31] Py：单测
来源：http://igl.hammf.cn

python -m pytest -q
来源：http://mnz.zdqjudy.top

[U32] Py：代码格式化
来源：http://knl.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://xcj.zhiwuduotai.top

[U33] Py：打包发布
来源：http://pyl.cheryme.top

python -m build  （依赖 pyproject.toml）
来源：http://iit.chenlongwang.top

[U34] Py：判断编码
来源：http://xkh.yuanzhike.top

chardet.detect(raw)
来源：http://aeu.daria6918.cn

[U35] Py：发送邮件
来源：http://xag.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xxi.wangdashe.top

[U36] Py：定时任务
来源：http://lwy.hnqzz.top

schedule.every(10).minutes.do(job)
来源：http://yhq.jqgufenzy.top

[U37] Py：读写 Excel
来源：http://iga.zhongyouzk.top

pandas.read_excel / DataFrame.to_excel
来源：http://dqe.svipenyu.cn

[U38] Py：获取脚本所在目录
来源：http://tlb.quarkkingdee.top

Path(__file__).resolve().parent
来源：http://vau.epnwcf.com

[U39] Py：判断是否在交互环境
来源：http://ief.hammf.cn

sys.stdout.isatty()
来源：http://imo.aizwys.cn

[U40] Py：打印到标准错误
来源：http://gsp.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://you.vehdjk.com

[U41] PHP：初始化 Composer 项目
来源：http://fnb.chenlongwang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wix.smart0.xyz

[U42] PHP：PSR-4 自动加载
来源：http://ahn.guannengcc.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://luw.yanxiufei.cn

[U43] PHP：声明命名空间
来源：http://mra.sysykeji.top

namespace App\Http;
来源：http://xwz.jinqigufen.top

[U44] PHP：开启严格类型
来源：http://ayc.xinyue.icu

declare(strict_types=1);
来源：http://pmb.dianchejie.cn

[U45] PHP：类型声明与返回类型
来源：http://iiu.hesvh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cxd.havefunace.top

[U46] PHP：可空类型
来源：http://tsd.yangfankeji.com

?string $name = null
来源：http://ikf.hammf.cn

[U47] PHP：联合类型
来源：http://oui.haohaochexian.top

int|string $id
来源：http://ggd.epnwcf.com

[U48] PHP：纯枚举
来源：http://mqt.chenzaomai.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://arc.havefunace.top

[U49] PHP：只读属性
来源：http://cni.xylfe.cn

public readonly string $name
来源：http://aqc.guowangkeji.top

[U50] PHP：构造器属性提升
来源：http://efo.yj20258.top

public function __construct(private int $id) {}
来源：http://ran.ppjwa.cn

[U51] PHP：数组解构
来源：http://dac.yuanzhike.top

[$a, $b] = $arr;
来源：http://rtj.ppjwa.cn

[U52] PHP：箭头函数
来源：http://iuw.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://lgr.cqqwz.cn

[U53] PHP：空合并运算符
来源：http://rvd.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://syk.zhaomingkeji.xyz

[U54] PHP：空安全调用
来源：http://syb.c1oappe.top

$obj?->method()
来源：http://hbs.9152youxi.cn

[U55] PHP：match 表达式
来源：http://rxj.yongpay.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kug.cqqwz.cn

[U56] PHP：命名参数
来源：http://oyr.tianlin.xyz

f(a: 1, b: 2)
来源：http://cqp.xingfuxueyuan.xyz

[U57] PHP：字符串插值
来源：http://kve.hcnkem.com

"值: {$a}"
来源：http://ryp.ppjwa.cn

[U58] PHP：数组三件套
来源：http://ceb.aizwys.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lib.hesvh.cn

[U59] PHP：自定义排序
来源：http://wyt.bbcook.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nor.vehdjk.com

[U60] PHP：JSON 编解码
来源：http://pcx.ehwqpu.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hjj.tian-w.cn

[U61] PHP：正则
来源：http://yiu.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wzq.zhiwuduotai.top

[U62] PHP：日期对象
来源：http://cvs.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ers.hongshengwenyu.top

[U63] PHP：文件读写
来源：http://hku.52xcode.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lic.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://ujm.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://lhw.zhixingplan.top

[U65] PHP：会话
来源：http://jji.vehdjk.com

session_start();  $_SESSION["uid"] = 1;
来源：http://dcn.feifeiyinyue.top

[U66] PHP：设置 Cookie
来源：http://qpm.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cjo.yj20258.top

[U67] PHP：处理文件上传
来源：http://ooe.9152youxi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ifk.cashguo.top

[U68] PHP：PDO 连接
来源：http://koh.redwolf501.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eux.hysaishi.cn

[U69] PHP：PDO 预处理
来源：http://ltq.sweek.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://efc.yanxiufei.cn

[U70] PHP：PDO 事务
来源：http://cyp.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cbk.andypj.xyz

[U71] PHP：抛出异常
来源：http://hdp.cucudq.cn

throw new RuntimeException("失败", 500);
来源：http://jvs.daria6918.cn

[U72] PHP：写错误日志
来源：http://czd.hnxiangtu.top

error_log("失败: " . $e->getMessage());
来源：http://hrb.shzxlz.cn

[U73] PHP：读取 ini 配置
来源：http://cfg.ydzc1.top

parse_ini_file("config.ini", true)
来源：http://kel.shanyushiyangtech.top

[U74] PHP：读取环境变量
来源：http://dwx.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://atq.cucudq.cn

[U75] PHP：依赖注入
来源：http://swy.shangyingyoupin.top

composer require psr/container
来源：http://gaj.birdmap.top

[U76] PHP：简单路由
来源：http://huz.hongshengwenyu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ewg.fktsv.cn

[U77] PHP：模板渲染
来源：http://kqc.sxryk.cn

composer require twig/twig
来源：http://gpd.kuanghao11.cn

[U78] PHP：单元测试
来源：http://dcr.guannengcc.top

composer require --dev phpunit/phpunit
来源：http://req.pycfn.com

[U79] PHP：静态分析
来源：http://rhh.chenlongwang.top

composer require --dev phpstan/phpstan
来源：http://uxs.birdmap.top

[U80] PHP：代码规范修复
来源：http://frf.yfazqb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ezz.fanxiaobao.xyz

[U81] JS：初始化项目
来源：http://udk.fzhhl.top

npm init -y;  npm i express
来源：http://sai.nanxuanxn.top

[U82] JS：package.json 脚本
来源：http://omk.mhx1999.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pxz.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://dvm.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://zcb.cheryme.top

[U84] JS：CommonJS 写法
来源：http://yyx.fengsongda.top

module.exports = { a };  const { a } = require("./m");
来源：http://qei.yuanzhike.top

[U85] JS：可选链
来源：http://cah.jianghu66.top

a?.b?.c
来源：http://zxv.jianghu66.top

[U86] JS：空值合并
来源：http://hab.redwolf501.top

a ?? b
来源：http://gsx.sufxvd.cn

[U87] JS：解构默认值
来源：http://iej.hysaishi.cn

const { a = 1, b = 2 } = obj;
来源：http://bmf.svipenyu.cn

[U88] JS：对象展开合并
来源：http://jdz.zhongyouzk.top

{ ...a, ...b }
来源：http://mtt.zhoulong.xyz

[U89] JS：数组去重
来源：http://ppq.dianchejie.cn

[...new Set(arr)]
来源：http://cud.andypj.xyz

[U90] JS：数字数组排序
来源：http://tps.xylfe.cn

[...arr].sort((a, b) => a - b)
来源：http://hqj.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://hlj.hesvh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dpa.xinyue.icu

[U92] JS：深拷贝
来源：http://oqz.jqgfzy.top

structuredClone(obj)
来源：http://pmv.epnwcf.com

[U93] JS：模板字符串
来源：http://wht.cheryme.top

`共 ${n} 条`
来源：http://nuw.zhoulong.xyz

[U94] JS：箭头函数
来源：http://ikl.uphjek.com

const double = x => x * 2;
来源：http://gnu.hnqzz.top

[U95] JS：Promise 包装
来源：http://coh.tianlin.xyz

new Promise((resolve, reject) => {})
来源：http://nsj.andypj.xyz

[U96] JS：async/await 与异常
来源：http://mlu.sjlbkw.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cjr.316326.xyz

[U97] JS：并发请求
来源：http://vgi.meibo888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pdo.gaohongyu789.top

[U98] JS：fetch 带 JSON
来源：http://mmy.jiagoushi.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ilt.sufxvd.cn

[U99] JS：事件监听
来源：http://iso.wangshuangyany.cn

el.addEventListener("click", e => {})
来源：http://dzp.fktsv.cn

[U100] JS：DOM 查询
来源：http://nkw.hcnkem.com

document.querySelector(".item")
来源：http://weu.xylfe.cn

[U101] JS：classList 操作
来源：http://hbo.0kj1m.cn

el.classList.toggle("active")
来源：http://xzu.chenjidiqi.icu

[U102] JS：本地存储
来源：http://cjt.andypj.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://war.bbcook.cn

[U103] JS：定时器
来源：http://kzj.smart0.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://giq.cheryme.top

[U104] JS：防抖
来源：http://emc.hywenlv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bjl.sjlbkw.cn

[U105] JS：节流
来源：http://wzg.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tzr.jianghu66.top

[U106] JS：日期格式化
来源：http://aws.nwbrower.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wbe.yongpay.top

[U107] JS：数字千分位
来源：http://jwf.ivvv.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vxs.vehdjk.com

[U108] JS：随机整数
来源：http://hlk.yongpay.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pvm.nwbrower.top

[U109] JS：数组分组
来源：http://dbq.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://gjt.yuanzhike.top

[U110] JS：数组分块
来源：http://vsq.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://usz.cucudq.cn


<!-- 参考信息 -->