代发 wailian999

[T39] Lua：模式匹配
来源：http://jdi.sxryk.cn

string.find(s, "%d+")
来源：http://ftf.meibo888.top

[T40] Lua：元表
来源：http://exv.ywan-chungtsiang.top

setmetatable({}, { __index = base })
来源：http://fwe.tarul.cn

[T41] Perl：Hello World
来源：http://eji.snrcjt.cn

print "Hello\n";
来源：http://ssj.daria6918.cn

[T42] Perl：变量类型
来源：http://vja.havefunace.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bse.fktsv.cn

[T43] Perl：字符串插值
来源：http://hoq.jianghu66.top

"值: $a"
来源：http://kwg.zycfv.cn

[T44] Perl：条件
来源：http://tcr.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://obp.hammf.cn

[T45] Perl：数组遍历
来源：http://eyq.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://plx.bjfxy.top

[T46] Perl：哈希操作
来源：http://jts.cdnleiting.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wlr.cucudq.cn

[T47] Perl：正则捕获
来源：http://nxe.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lip.zhijiandao.cn

[T48] Perl：正则替换
来源：http://rvt.smart0.xyz

$s =~ s/old/new/g;
来源：http://qma.0kj1m.cn

[T49] Perl：函数
来源：http://gqf.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uor.xinyue.icu

[T50] Perl：逐行读文件
来源：http://fql.sjlbkw.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://byr.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://eny.ivvv.top

[T51] Scala：Hello World
来源：http://ofy.jlsjyb.cn

println("Hello")
来源：http://ksu.yj20258888.top

[T52] Scala：变量
来源：http://kzb.wangshuangyany.cn

val a = 1;  var b = 2
来源：http://ooi.chenzaomai.com

[T53] Scala：字符串插值
来源：http://rby.gaohongyu789.top

s"值: $b"
来源：http://cef.jinghuilouyu.cn

[T54] Scala：集合映射
来源：http://itj.ybcxt.top

List(1, 2, 3).map(_ * 2)
来源：http://arn.daria6918.cn

[T55] Scala：集合过滤
来源：http://mdc.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://bqn.sufxvd.cn

[T56] Scala：样例类
来源：http://jmo.bbcook.cn

case class User(name: String, age: Int)
来源：http://mmb.hongshengwenyu.top

[T57] Scala：模式匹配
来源：http://wyv.hysaishi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tdb.chenlongwang.top

[T58] Scala：函数定义
来源：http://imp.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://shw.sweek.top

[T59] Scala：循环
来源：http://fhr.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://opb.jyoumei.cn

[T60] Scala：折叠
来源：http://dye.jinghuilouyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jbu.gotoacloud.top

================================================================================
来源：http://mnd.fzhhl.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pfl.andypj.xyz

================================================================================
来源：http://bva.iojbl.cn

[U01] Py：创建虚拟环境
来源：http://wkn.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://snl.vqdsnc.cn

[U02] Py：导出 / 安装依赖
来源：http://wyx.hnqzz.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://suf.shzxlz.cn

[U03] Py：加载 .env 配置
来源：http://oby.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pvr.aizwys.cn

[U04] Py：变量调试打印
来源：http://qvg.fanxiaobao.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ucw.hammf.cn

[U05] Py：列表去重且保序
来源：http://oal.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://ewm.hfpthk.cn

[U06] Py：合并两个字典
来源：http://tea.wangdashe.top

{**a, **b}
来源：http://oly.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://iid.jqgfzy.top

{v: k for k, v in d.items()}
来源：http://nym.epnwcf.com

[U08] Py：展平二维列表
来源：http://jjp.sufxvd.cn

[y for x in nested for y in x]
来源：http://qis.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://ohl.nanxinkj.top

max(d, key=d.get)
来源：http://clj.ybcxt.top

[U10] Py：按值排序字典
来源：http://gfd.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tus.gogol.net.cn

[U11] Py：生成器表达式
来源：http://tpj.ehwqpu.com

(x * 2 for x in arr)
来源：http://une.xuanzx.com

[U12] Py：取出现最多的 3 个元素
来源：http://tai.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://quy.guowangkeji.top

[U13] Py：固定长度队列
来源：http://ric.gogol.net.cn

deque(maxlen=10)
来源：http://nhd.zhongyouzk.top

[U14] Py：分组收集到列表
来源：http://iun.chenzaomai.com

defaultdict(list)
来源：http://wkd.snrcjt.cn

[U15] Py：高精度计时
来源：http://cvu.meibo888.top

t = time.perf_counter()
来源：http://psl.chenjidiqi.icu

[U16] Py：命令行参数解析
来源：http://knk.9152youxi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cxz.yonumen.top

[U17] Py：初始化日志
来源：http://wol.ppjwa.cn

logging.basicConfig(level=logging.INFO)
来源：http://osb.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://wgx.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://ezp.jianghu66.top

[U19] Py：正则替换带回调
来源：http://jlv.hesvh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nzw.ydzc1.top

[U20] Py：缓存函数结果
来源：http://amu.hfpthk.cn

@functools.lru_cache(maxsize=None)
来源：http://woi.jinyuanbaomall.cn

[U21] Py：自定义上下文管理器
来源：http://pzb.zhijiandao.cn

@contextlib.contextmanager
来源：http://sdp.zhijiandao.cn

[U22] Py：矩阵转置
来源：http://ddb.hnxiangtu.top

list(zip(*m))
来源：http://ovz.jqgfzy.top

[U23] Py：分块读取大文件
来源：http://zal.jiagoushi.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://snj.xingfuxueyuan.xyz

[U24] Py：路径操作
来源：http://ljc.wangdashe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://keh.xinyue.icu

[U25] Py：CSV 按字典读
来源：http://uli.yuanzhike.top

csv.DictReader(f)
来源：http://fjc.sjlbkw.cn

[U26] Py：并发下载
来源：http://wnw.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tsc.jinqigufen.top

[U27] Py：异步 HTTP
来源：http://qra.fzhhl.top

aiohttp.ClientSession() 配合 async with
来源：http://qmu.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://jjr.zhiwuduotai.top

UserId = int
来源：http://mjy.xuanzx.com

[U29] Py：属性校验
来源：http://rgt.hcnkem.com

@property 与 @x.setter 配合
来源：http://xgg.meibo888.top

[U30] Py：数据类
来源：http://lrs.xylfe.cn

@dataclass(slots=True)
来源：http://ibi.cheryme.top

[U31] Py：单测
来源：http://qmi.zhoulong.xyz

python -m pytest -q
来源：http://kjx.tarul.cn

[U32] Py：代码格式化
来源：http://ayv.fanxiaobao.xyz

ruff format . && ruff check --fix .
来源：http://bmu.ivvv.top

[U33] Py：打包发布
来源：http://rel.cheryme.top

python -m build  （依赖 pyproject.toml）
来源：http://hqq.hfpthk.cn

[U34] Py：判断编码
来源：http://ito.xylfe.cn

chardet.detect(raw)
来源：http://hsc.gogol.net.cn

[U35] Py：发送邮件
来源：http://djo.shzxlz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ope.hesvh.cn

[U36] Py：定时任务
来源：http://tcu.shanyushiyangtech.top

schedule.every(10).minutes.do(job)
来源：http://lyk.c1oappe.top

[U37] Py：读写 Excel
来源：http://qsh.cdnleiting.top

pandas.read_excel / DataFrame.to_excel
来源：http://srd.yongpay.top

[U38] Py：获取脚本所在目录
来源：http://qty.snrcjt.cn

Path(__file__).resolve().parent
来源：http://uwl.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://dil.ydjk.org.cn

sys.stdout.isatty()
来源：http://zmd.gzhubu.top

[U40] Py：打印到标准错误
来源：http://bad.zhoulong.xyz

print("err", file=sys.stderr)
来源：http://hix.gzhubu.top

[U41] PHP：初始化 Composer 项目
来源：http://ioc.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://edv.cdnleiting.top

[U42] PHP：PSR-4 自动加载
来源：http://edr.sxryk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gen.xingfuxueyuan.xyz

[U43] PHP：声明命名空间
来源：http://wgb.cheryme.top

namespace App\Http;
来源：http://lpi.ybcxt.top

[U44] PHP：开启严格类型
来源：http://jbo.nanxuanxn.top

declare(strict_types=1);
来源：http://qwx.svipenyu.cn

[U45] PHP：类型声明与返回类型
来源：http://xmz.fanxiaobao.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://yim.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://ydo.zhengqikj.top

?string $name = null
来源：http://vga.fanxiaobao.xyz

[U47] PHP：联合类型
来源：http://nkj.haohaochexian.top

int|string $id
来源：http://ccg.daria6918.cn

[U48] PHP：纯枚举
来源：http://rgi.guannengcc.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gyv.xinyue.icu

[U49] PHP：只读属性
来源：http://lsu.shuidangran.top

public readonly string $name
来源：http://oxx.hammf.cn

[U50] PHP：构造器属性提升
来源：http://gre.hysaishi.cn

public function __construct(private int $id) {}
来源：http://kmu.sysykeji.top

[U51] PHP：数组解构
来源：http://pqv.xingfuxueyuan.xyz

[$a, $b] = $arr;
来源：http://lkj.yangfankeji.com

[U52] PHP：箭头函数
来源：http://xko.c1oappe.top

$double = fn($x) => $x * 2;
来源：http://sis.yuxming.cn

[U53] PHP：空合并运算符
来源：http://kue.jlsjyb.cn

$v = $a ?? $b ?? "default";
来源：http://sol.nwbrower.top

[U54] PHP：空安全调用
来源：http://ypk.hywenlv.cn

$obj?->method()
来源：http://tyy.fanxiaobao.xyz

[U55] PHP：match 表达式
来源：http://jtu.jinqigfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qxi.zycfv.cn

[U56] PHP：命名参数
来源：http://aqn.yj202588.top

f(a: 1, b: 2)
来源：http://kcr.gotoacloud.top

[U57] PHP：字符串插值
来源：http://nfl.bbcook.cn

"值: {$a}"
来源：http://hyt.shanyushiyangkeji.top

[U58] PHP：数组三件套
来源：http://jhb.gaohongyu789.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://inv.aizwys.cn

[U59] PHP：自定义排序
来源：http://blw.chenjidiqi.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mfw.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://vtk.jiagoushi.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qnk.yanxiufei.cn

[U61] PHP：正则
来源：http://ktq.wangshuangyany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bzz.gzhubu.top

[U62] PHP：日期对象
来源：http://wiq.tianlin.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xhz.daxiang520.top

[U63] PHP：文件读写
来源：http://bre.aibaodan.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://whr.zycfv.cn

[U64] PHP：目录遍历
来源：http://dmc.chenlongwang.top

glob("dir/*.php");  scandir("dir");
来源：http://fvz.quarkkingdee.top

[U65] PHP：会话
来源：http://grn.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://thl.dianchejie.cn

[U66] PHP：设置 Cookie
来源：http://hpw.dianchejie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tjt.vqdsnc.cn

[U67] PHP：处理文件上传
来源：http://ffe.ppjwa.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tvt.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://fhh.tarul.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tai.gzhubu.top

[U69] PHP：PDO 预处理
来源：http://ymh.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zkx.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://rgq.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nwm.iojbl.cn

[U71] PHP：抛出异常
来源：http://qdh.9152youxi.cn

throw new RuntimeException("失败", 500);
来源：http://rww.sjlbkw.cn

[U72] PHP：写错误日志
来源：http://xnt.jqgufenzy.top

error_log("失败: " . $e->getMessage());
来源：http://xrf.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://xae.snrcjt.cn

parse_ini_file("config.ini", true)
来源：http://bmt.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://mus.yj202588.top

getenv("APP_ENV") ?: "production"
来源：http://nlb.cdnleiting.top

[U75] PHP：依赖注入
来源：http://gzk.xinyue.icu

composer require psr/container
来源：http://yjb.aibaodan.cn

[U76] PHP：简单路由
来源：http://vdd.fanxiaobao.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qfc.zhoulong.xyz

[U77] PHP：模板渲染
来源：http://whl.hfpthk.cn

composer require twig/twig
来源：http://qyg.zycfv.cn

[U78] PHP：单元测试
来源：http://xgi.tanke756.top

composer require --dev phpunit/phpunit
来源：http://elx.jinghuilouyu.cn

[U79] PHP：静态分析
来源：http://udh.cheryme.top

composer require --dev phpstan/phpstan
来源：http://vgh.haohaochexian.top

[U80] PHP：代码规范修复
来源：http://ntf.jlsjyb.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://huw.hongshengwenyu.top

[U81] JS：初始化项目
来源：http://sfd.aizwys.cn

npm init -y;  npm i express
来源：http://yto.wangdashe.top

[U82] JS：package.json 脚本
来源：http://sjf.zhixingplan.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qyl.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://fjy.zhaomingkeji.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://ibv.yangfankeji.com

[U84] JS：CommonJS 写法
来源：http://cev.ppjwa.cn

module.exports = { a };  const { a } = require("./m");
来源：http://whq.jqgfzy.top

[U85] JS：可选链
来源：http://uix.jinghuilouyu.cn

a?.b?.c
来源：http://txx.jinyuanbaomall.cn

[U86] JS：空值合并
来源：http://rbt.fehbvm.com

a ?? b
来源：http://ops.yongpay.top

[U87] JS：解构默认值
来源：http://hlq.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://ies.yj20258.top

[U88] JS：对象展开合并
来源：http://ica.hnqzz.top

{ ...a, ...b }
来源：http://ehr.kuanghao11.cn

[U89] JS：数组去重
来源：http://izm.zhiwuduotai.top

[...new Set(arr)]
来源：http://yjb.gaohongyu789.top

[U90] JS：数字数组排序
来源：http://ioa.haohaochexian.top

[...arr].sort((a, b) => a - b)
来源：http://yqr.cdnleiting.top

[U91] JS：对象键值遍历
来源：http://xdo.jinqigfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yca.fktsv.cn

[U92] JS：深拷贝
来源：http://sxu.yj20258.top

structuredClone(obj)
来源：http://piy.jinqigfzy.top

[U93] JS：模板字符串
来源：http://ixn.pengpengdd.cyou

`共 ${n} 条`
来源：http://mud.ydjk.org.cn

[U94] JS：箭头函数
来源：http://sfb.pengpengdd.cyou

const double = x => x * 2;
来源：http://xmz.andypj.xyz

[U95] JS：Promise 包装
来源：http://ssb.zhiwuduotai.top

new Promise((resolve, reject) => {})
来源：http://pof.daria6918.cn

[U96] JS：async/await 与异常
来源：http://ytq.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yqz.shzxlz.cn

[U97] JS：并发请求
来源：http://hik.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nch.yj20258888.top

[U98] JS：fetch 带 JSON
来源：http://rtn.andypj.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ers.ppjwa.cn

[U99] JS：事件监听
来源：http://ygf.yj20258888.top

el.addEventListener("click", e => {})
来源：http://bzh.zdbjq.cn

[U100] JS：DOM 查询
来源：http://wrn.ctjpmb.com

document.querySelector(".item")
来源：http://csb.havefunace.top

[U101] JS：classList 操作
来源：http://fjb.gotoacloud.top

el.classList.toggle("active")
来源：http://ebh.yangfankeji.com

[U102] JS：本地存储
来源：http://vxb.gaohongyu789.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bbv.fzhhl.top

[U103] JS：定时器
来源：http://zlg.uphjek.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jps.shzxlz.cn

[U104] JS：防抖
来源：http://cuv.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://inr.fengsongda.top

[U105] JS：节流
来源：http://fmb.fktsv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mcx.yvedp.cn

[U106] JS：日期格式化
来源：http://lhi.sweek.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zat.nanxuanxn.top

[U107] JS：数字千分位
来源：http://kko.sjlbkw.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://egp.tanke756.top

[U108] JS：随机整数
来源：http://llq.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://psd.9152youxi.cn

[U109] JS：数组分组
来源：http://nbt.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://kjx.hnqzz.top

[U110] JS：数组分块
来源：http://kyd.cqqwz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://efx.yanxiufei.cn

[U111] JS：对象转 Map
来源：http://rag.hammf.cn

new Map(Object.entries(obj))
来源：http://ruv.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://nnu.yongpay.top

"7".padStart(3, "0")
来源：http://iyd.zhiwuduotai.top

[U113] JS：正则替换全部
来源：http://bjd.jqgfzy.top

s.replaceAll("a", "b")
来源：http://avu.vqdsnc.cn

[U114] JS：JSON 深比较
来源：http://jwd.sweek.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ffc.c1oappe.top

[U115] JS：生成 UUID
来源：http://mun.shanyushiyangtech.top

crypto.randomUUID()
来源：http://lzq.sysykeji.top

[U116] JS：类型检查（JSDoc）
来源：http://lgp.xinyue.icu

/** @param {string} name */ function f(name) {}
来源：http://bwr.yueranfly.top

[U117] JS：单元测试
来源：http://bfi.gzhubu.top

npm i -D vitest;  npx vitest
来源：http://mvo.uphjek.com

[U118] JS：开发服务器
来源：http://teb.zhaomingkeji.xyz

npm i -D vite;  npx vite
来源：http://dfr.hnqzz.top

[U119] JS：生产构建
来源：http://eha.xuanzx.com

npx vite build
来源：http://lxm.meibo888.top

[U120] JS：读取环境变量（Vite）
来源：http://yix.xuetiantiany.cn

import.meta.env.VITE_API_URL
来源：http://nyb.quarkkingdee.top

================================================================================
来源：http://wiq.yuxming.cn

统计汇总
来源：http://rgb.yanxiufei.cn

================================================================================
来源：http://jix.kuanghao11.cn

按语言统计（条）：
来源：http://gmx.xylfe.cn

Python ......... 252
来源：http://ejq.zhijiandao.cn

PHP ............ 252
来源：http://ido.fktsv.cn

JavaScript ..... 252
来源：http://klw.aizwys.cn

TypeScript ..... 212
来源：http://sty.iojbl.cn

Java ........... 212
来源：http://zcz.c1oappe.top

Go ............. 212
来源：http://fqy.feifeiyinyue.top

Ruby ........... 212
来源：http://qvz.jlsjyb.cn

C# ............. 212
来源：http://erz.ydjk.org.cn


<!-- 参考信息 -->