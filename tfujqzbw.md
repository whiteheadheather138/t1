代发 wailian999

[T35] Lua：字典表
来源：http://rku.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://jhz.yanxiufei.cn

[T36] Lua：函数
来源：http://jog.sweek.top

function add(a, b) return a + b end
来源：http://fjk.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://ijl.52xcode.cn

"a" .. "b"
来源：http://aqr.hongshengwenyu.top

[T38] Lua：条件
来源：http://sos.sysykeji.top

if x > 0 then print("正") end
来源：http://sqc.tarul.cn

[T39] Lua：模式匹配
来源：http://oag.cucudq.cn

string.find(s, "%d+")
来源：http://qgx.xziqi.cn

[T40] Lua：元表
来源：http://rsz.xinyue.icu

setmetatable({}, { __index = base })
来源：http://hgf.nanxuanxn.top

[T41] Perl：Hello World
来源：http://mov.gzhubu.top

print "Hello\n";
来源：http://bwd.jyoumei.cn

[T42] Perl：变量类型
来源：http://gss.vehdjk.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fvs.jlsjyb.cn

[T43] Perl：字符串插值
来源：http://rri.316326.xyz

"值: $a"
来源：http://ppp.yj202588.top

[T44] Perl：条件
来源：http://bgk.xuetiantiany.cn

if ($a > 0) { print "正"; }
来源：http://fvj.sweek.top

[T45] Perl：数组遍历
来源：http://dlh.snrcjt.cn

for my $x (@arr) { print $x; }
来源：http://ulq.ybcxt.top

[T46] Perl：哈希操作
来源：http://moq.chenzaomai.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yvo.zhiwuduotai.top

[T47] Perl：正则捕获
来源：http://zom.jyoumei.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oid.9152youxi.cn

[T48] Perl：正则替换
来源：http://afm.jqgufenzy.top

$s =~ s/old/new/g;
来源：http://tvc.fzhhl.top

[T49] Perl：函数
来源：http://iui.chenzaomai.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tuq.zdqjudy.top

[T50] Perl：逐行读文件
来源：http://tud.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://utr.tanke756.top

while (my $line = <$fh>) { print $line; }
来源：http://rmw.hcnkem.com

[T51] Scala：Hello World
来源：http://yhn.chenlongwang.top

println("Hello")
来源：http://cak.gzhubu.top

[T52] Scala：变量
来源：http://fve.yj20258.top

val a = 1;  var b = 2
来源：http://cbd.dianchejie.cn

[T53] Scala：字符串插值
来源：http://dwg.tanke756.top

s"值: $b"
来源：http://saa.yj202588.top

[T54] Scala：集合映射
来源：http://xcx.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://mpk.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://arx.yj20258.top

List(1, 2, 3).filter(_ > 1)
来源：http://lss.sxryk.cn

[T56] Scala：样例类
来源：http://xwd.ivvv.top

case class User(name: String, age: Int)
来源：http://wtm.fengsongda.top

[T57] Scala：模式匹配
来源：http://uao.uphjek.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://ogr.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://gtl.jinyuanbaomall.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ugw.epnwcf.com

[T59] Scala：循环
来源：http://wji.shanyushiyangtech.top

for (i <- 1 to 10) println(i)
来源：http://gxz.dashuyun.cn

[T60] Scala：折叠
来源：http://ztq.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zwp.jqgfzy.top

================================================================================
来源：http://ifj.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qia.zdqjudy.top

================================================================================
来源：http://koa.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://ddi.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hwf.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://ned.zdqjudy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qut.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://qsf.hfpthk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jnw.epnwcf.com

[U04] Py：变量调试打印
来源：http://vaw.jqgufenzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vgz.chenjidiqi.icu

[U05] Py：列表去重且保序
来源：http://top.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://koz.sxryk.cn

[U06] Py：合并两个字典
来源：http://kyf.feifeiyinyue.top

{**a, **b}
来源：http://svv.iojbl.cn

[U07] Py：反转字典键值
来源：http://dxg.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://auf.epnwcf.com

[U08] Py：展平二维列表
来源：http://zxn.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://yeh.xingfuxueyuan.xyz

[U09] Py：字典取最大值的键
来源：http://trc.jyoumei.cn

max(d, key=d.get)
来源：http://fca.hysaishi.cn

[U10] Py：按值排序字典
来源：http://wmr.yonumen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gov.redwolf501.top

[U11] Py：生成器表达式
来源：http://kve.jinqigfzy.top

(x * 2 for x in arr)
来源：http://zpe.xingfuxueyuan.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://yul.shuidangran.top

Counter(arr).most_common(3)
来源：http://zik.smart0.xyz

[U13] Py：固定长度队列
来源：http://xcg.yfazqb.com

deque(maxlen=10)
来源：http://xje.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://wra.shanyushiyangkeji.top

defaultdict(list)
来源：http://eow.cucudq.cn

[U15] Py：高精度计时
来源：http://kvk.gaohongyu789.top

t = time.perf_counter()
来源：http://ner.yueranfly.top

[U16] Py：命令行参数解析
来源：http://set.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nfs.gzhubu.top

[U17] Py：初始化日志
来源：http://knq.xuanzx.com

logging.basicConfig(level=logging.INFO)
来源：http://wao.iojbl.cn

[U18] Py：预编译正则
来源：http://qan.jinqigfzy.top

pat = re.compile(r"\d+")
来源：http://ttm.guowangkeji.top

[U19] Py：正则替换带回调
来源：http://npt.ivvv.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xae.shzxlz.cn

[U20] Py：缓存函数结果
来源：http://woq.snrcjt.cn

@functools.lru_cache(maxsize=None)
来源：http://wee.fehbvm.com

[U21] Py：自定义上下文管理器
来源：http://mna.sysykeji.top

@contextlib.contextmanager
来源：http://seo.chenjidiqi.icu

[U22] Py：矩阵转置
来源：http://ege.yvedp.cn

list(zip(*m))
来源：http://jkd.sysykeji.top

[U23] Py：分块读取大文件
来源：http://qct.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wxm.vehdjk.com

[U24] Py：路径操作
来源：http://fgy.quarkkingdee.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tpy.zycfv.cn

[U25] Py：CSV 按字典读
来源：http://kiz.fzhhl.top

csv.DictReader(f)
来源：http://moy.sweek.top

[U26] Py：并发下载
来源：http://yjm.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mqv.xuetiantiany.cn

[U27] Py：异步 HTTP
来源：http://sas.shanyushiyangtech.top

aiohttp.ClientSession() 配合 async with
来源：http://oxc.c1oappe.top

[U28] Py：类型别名
来源：http://xuf.chenlongwang.top

UserId = int
来源：http://mbm.birdmap.top

[U29] Py：属性校验
来源：http://jjf.aizwys.cn

@property 与 @x.setter 配合
来源：http://tgu.yonumen.top

[U30] Py：数据类
来源：http://ltq.yj20258.top

@dataclass(slots=True)
来源：http://top.zdqjudy.top

[U31] Py：单测
来源：http://def.mhx1999.top

python -m pytest -q
来源：http://wxf.birdmap.top

[U32] Py：代码格式化
来源：http://fbb.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://ucr.zdqjudy.top

[U33] Py：打包发布
来源：http://wqg.tanke756.top

python -m build  （依赖 pyproject.toml）
来源：http://ouw.zhiwuduotai.top

[U34] Py：判断编码
来源：http://hhy.yj202588.top

chardet.detect(raw)
来源：http://xgi.chenlongwang.top

[U35] Py：发送邮件
来源：http://mbw.ydzc1.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yol.0kj1m.cn

[U36] Py：定时任务
来源：http://kcv.dianchejie.cn

schedule.every(10).minutes.do(job)
来源：http://qif.pycfn.com

[U37] Py：读写 Excel
来源：http://hpb.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://whq.sweek.top

[U38] Py：获取脚本所在目录
来源：http://xxz.316326.xyz

Path(__file__).resolve().parent
来源：http://cvd.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://vvq.iojbl.cn

sys.stdout.isatty()
来源：http://twu.hnqzz.top

[U40] Py：打印到标准错误
来源：http://usm.yj202588.top

print("err", file=sys.stderr)
来源：http://jsk.cheryme.top

[U41] PHP：初始化 Composer 项目
来源：http://dul.gotoacloud.top

composer init;  composer require guzzlehttp/guzzle
来源：http://aeh.yonumen.top

[U42] PHP：PSR-4 自动加载
来源：http://gkc.fzhhl.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ykr.jiagoushi.top

[U43] PHP：声明命名空间
来源：http://ill.meibo888.top

namespace App\Http;
来源：http://zey.wangshuangyany.cn

[U44] PHP：开启严格类型
来源：http://hdb.xziqi.cn

declare(strict_types=1);
来源：http://ogs.9152youxi.cn

[U45] PHP：类型声明与返回类型
来源：http://zae.tian-w.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jwp.havefunace.top

[U46] PHP：可空类型
来源：http://ser.c1oappe.top

?string $name = null
来源：http://kiy.tian-w.cn

[U47] PHP：联合类型
来源：http://zfn.zhengqikj.top

int|string $id
来源：http://evb.ydjk.org.cn

[U48] PHP：纯枚举
来源：http://gnb.birdmap.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qvf.bbcook.cn

[U49] PHP：只读属性
来源：http://jsi.0kj1m.cn

public readonly string $name
来源：http://ogp.bbcook.cn

[U50] PHP：构造器属性提升
来源：http://sqs.hnxiangtu.top

public function __construct(private int $id) {}
来源：http://xbg.gaohongyu789.top

[U51] PHP：数组解构
来源：http://tvm.vehdjk.com

[$a, $b] = $arr;
来源：http://vjl.gotoacloud.top

[U52] PHP：箭头函数
来源：http://cry.hnxiangtu.top

$double = fn($x) => $x * 2;
来源：http://caa.shanyushiyangkeji.top

[U53] PHP：空合并运算符
来源：http://ryl.hfpthk.cn

$v = $a ?? $b ?? "default";
来源：http://vpv.tarul.cn

[U54] PHP：空安全调用
来源：http://bdc.redwolf501.top

$obj?->method()
来源：http://llu.zhaomingkeji.xyz

[U55] PHP：match 表达式
来源：http://alb.cheryme.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ghw.haohaochexian.top

[U56] PHP：命名参数
来源：http://yyk.jinqigufen.top

f(a: 1, b: 2)
来源：http://tia.zdqjudy.top

[U57] PHP：字符串插值
来源：http://tbd.shangyingyoupin.top

"值: {$a}"
来源：http://qhr.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://cug.ctjpmb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gzo.wangshuangyany.cn

[U59] PHP：自定义排序
来源：http://gah.havefunace.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tta.tian-w.cn

[U60] PHP：JSON 编解码
来源：http://ltv.gzhubu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lhw.daria6918.cn

[U61] PHP：正则
来源：http://dbr.mhx1999.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tyc.feifeiyinyue.top

[U62] PHP：日期对象
来源：http://kaa.yongpay.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tzq.yongpay.top

[U63] PHP：文件读写
来源：http://zav.jyoumei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zns.daxiang520.top

[U64] PHP：目录遍历
来源：http://tay.yj202588.top

glob("dir/*.php");  scandir("dir");
来源：http://jul.zhongyouzk.top

[U65] PHP：会话
来源：http://klf.sysykeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qrg.nwbrower.top

[U66] PHP：设置 Cookie
来源：http://aqe.gaohongyu789.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sii.sxryk.cn

[U67] PHP：处理文件上传
来源：http://znb.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cok.hfpthk.cn

[U68] PHP：PDO 连接
来源：http://zsw.fktsv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ddv.dashuyun.cn

[U69] PHP：PDO 预处理
来源：http://nyq.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dnx.yongpay.top

[U70] PHP：PDO 事务
来源：http://who.hammf.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jlh.hnqzz.top

[U71] PHP：抛出异常
来源：http://fkh.aizwys.cn

throw new RuntimeException("失败", 500);
来源：http://oec.nwbrower.top

[U72] PHP：写错误日志
来源：http://den.pycfn.com

error_log("失败: " . $e->getMessage());
来源：http://nsv.havefunace.top

[U73] PHP：读取 ini 配置
来源：http://xnm.shanyushiyangtech.top

parse_ini_file("config.ini", true)
来源：http://yuu.ctjpmb.com

[U74] PHP：读取环境变量
来源：http://mxf.iojbl.cn

getenv("APP_ENV") ?: "production"
来源：http://wvk.aibaodan.cn

[U75] PHP：依赖注入
来源：http://dfv.pengpengdd.cyou

composer require psr/container
来源：http://gfz.jianghu66.top

[U76] PHP：简单路由
来源：http://nxq.9152youxi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jzz.xuanzx.com

[U77] PHP：模板渲染
来源：http://iij.shzxlz.cn

composer require twig/twig
来源：http://net.fzhhl.top

[U78] PHP：单元测试
来源：http://ezz.cucudq.cn

composer require --dev phpunit/phpunit
来源：http://urh.yuxming.cn

[U79] PHP：静态分析
来源：http://fye.hnxiangtu.top

composer require --dev phpstan/phpstan
来源：http://opa.nanxinkj.top

[U80] PHP：代码规范修复
来源：http://rjc.hnxiangtu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bcc.xuetiantiany.cn

[U81] JS：初始化项目
来源：http://enk.ivvv.top

npm init -y;  npm i express
来源：http://vzj.cashguo.top

[U82] JS：package.json 脚本
来源：http://pmc.hnxiangtu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xea.jinqigfzy.top

[U83] JS：ES Module 导入导出
来源：http://xod.xziqi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://evo.yueranfly.top

[U84] JS：CommonJS 写法
来源：http://snm.uphjek.com

module.exports = { a };  const { a } = require("./m");
来源：http://fet.zhoulong.xyz

[U85] JS：可选链
来源：http://jfc.tianlin.xyz

a?.b?.c
来源：http://ydr.svipenyu.cn

[U86] JS：空值合并
来源：http://ckw.guannengcc.top

a ?? b
来源：http://qky.hesvh.cn

[U87] JS：解构默认值
来源：http://qel.ywan-chungtsiang.top

const { a = 1, b = 2 } = obj;
来源：http://vwv.snrcjt.cn

[U88] JS：对象展开合并
来源：http://lkh.yj20258.top

{ ...a, ...b }
来源：http://zmy.jqgufenzy.top

[U89] JS：数组去重
来源：http://weh.jqgfzy.top

[...new Set(arr)]
来源：http://zta.kuanghao11.cn

[U90] JS：数字数组排序
来源：http://nys.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://quu.hfpthk.cn

[U91] JS：对象键值遍历
来源：http://cvn.ehwqpu.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xmo.zhixingplan.top

[U92] JS：深拷贝
来源：http://gcg.fanxiaobao.xyz

structuredClone(obj)
来源：http://bsi.fzhhl.top

[U93] JS：模板字符串
来源：http://ejw.yuanzhike.top

`共 ${n} 条`
来源：http://xod.sweek.top

[U94] JS：箭头函数
来源：http://qnx.yangfankeji.com

const double = x => x * 2;
来源：http://lnu.zhixingplan.top

[U95] JS：Promise 包装
来源：http://eiy.hywenlv.cn

new Promise((resolve, reject) => {})
来源：http://ujm.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://ccj.tanke756.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bos.xziqi.cn

[U97] JS：并发请求
来源：http://kbr.haohaochexian.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://eve.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://pks.nanxinkj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qiz.birdmap.top

[U99] JS：事件监听
来源：http://gxg.andypj.xyz

el.addEventListener("click", e => {})
来源：http://hff.sweek.top

[U100] JS：DOM 查询
来源：http://ims.xylfe.cn

document.querySelector(".item")
来源：http://zxy.yj20258.top

[U101] JS：classList 操作
来源：http://spp.ydjk.org.cn

el.classList.toggle("active")
来源：http://foi.jlsjyb.cn

[U102] JS：本地存储
来源：http://sgp.pengpengdd.cyou

localStorage.setItem("k", JSON.stringify(v))
来源：http://dvb.yj20258888.top

[U103] JS：定时器
来源：http://svp.fehbvm.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rqw.ppjwa.cn

[U104] JS：防抖
来源：http://gjb.hnqzz.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://roa.aibaodan.cn

[U105] JS：节流
来源：http://roa.daxiang520.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sck.nanxinkj.top

[U106] JS：日期格式化
来源：http://nez.mhx1999.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://suc.ydjk.org.cn

[U107] JS：数字千分位
来源：http://qdo.cdnleiting.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://aqo.quarkkingdee.top

[U108] JS：随机整数
来源：http://fck.havefunace.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iqo.jiagoushi.top

[U109] JS：数组分组
来源：http://evd.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://ffs.wangdashe.top

[U110] JS：数组分块
来源：http://bcs.yj202588.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rrz.jyoumei.cn

[U111] JS：对象转 Map
来源：http://waw.ydzc1.top

new Map(Object.entries(obj))
来源：http://qui.aizwys.cn

[U112] JS：字符串补位
来源：http://lvf.nwbrower.top

"7".padStart(3, "0")
来源：http://nog.hfpthk.cn

[U113] JS：正则替换全部
来源：http://fxu.aibaodan.cn

s.replaceAll("a", "b")
来源：http://kwn.xylfe.cn

[U114] JS：JSON 深比较
来源：http://bhv.snrcjt.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cdi.sufxvd.cn

[U115] JS：生成 UUID
来源：http://iot.xinyue.icu

crypto.randomUUID()
来源：http://gax.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://zmv.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://eqh.yongpay.top

[U117] JS：单元测试
来源：http://pqw.guowangkeji.top

npm i -D vitest;  npx vitest
来源：http://day.tanke756.top

[U118] JS：开发服务器
来源：http://fot.tarul.cn

npm i -D vite;  npx vite
来源：http://ntj.sxryk.cn

[U119] JS：生产构建
来源：http://djs.zhaomingkeji.xyz

npx vite build
来源：http://kjx.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://lev.chenlongwang.top

import.meta.env.VITE_API_URL
来源：http://xnt.ivvv.top

================================================================================
来源：http://hsr.havefunace.top

统计汇总
来源：http://xah.sjlbkw.cn

================================================================================
来源：http://idg.havefunace.top

按语言统计（条）：
来源：http://mev.guannengcc.top


<!-- 参考信息 -->