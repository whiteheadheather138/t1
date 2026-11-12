代发 wailian999

[T37] Lua：字符串拼接
来源：http://ieu.shangyingyoupin.top

"a" .. "b"
来源：http://xud.sxryk.cn

[T38] Lua：条件
来源：http://mtn.sjlbkw.cn

if x > 0 then print("正") end
来源：http://ijd.wangdashe.top

[T39] Lua：模式匹配
来源：http://xiz.zdbjq.cn

string.find(s, "%d+")
来源：http://xcf.zhaomingkeji.xyz

[T40] Lua：元表
来源：http://yno.xinyue.icu

setmetatable({}, { __index = base })
来源：http://eme.xinyue.icu

[T41] Perl：Hello World
来源：http://dbu.hesvh.cn

print "Hello\n";
来源：http://kse.zhoulong.xyz

[T42] Perl：变量类型
来源：http://dzi.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ulr.9152youxi.cn

[T43] Perl：字符串插值
来源：http://hcu.sweek.top

"值: $a"
来源：http://dky.yuxming.cn

[T44] Perl：条件
来源：http://hrh.hcnkem.com

if ($a > 0) { print "正"; }
来源：http://nog.fengsongda.top

[T45] Perl：数组遍历
来源：http://qau.0kj1m.cn

for my $x (@arr) { print $x; }
来源：http://yxs.yongpay.top

[T46] Perl：哈希操作
来源：http://hyq.hesvh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yqc.meibo888.top

[T47] Perl：正则捕获
来源：http://kxp.jinghuilouyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qxz.cashguo.top

[T48] Perl：正则替换
来源：http://ijb.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://ujr.jyoumei.cn

[T49] Perl：函数
来源：http://vfy.havefunace.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gjs.zhengqikj.top

[T50] Perl：逐行读文件
来源：http://msf.xinyue.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://roq.zhixingplan.top

while (my $line = <$fh>) { print $line; }
来源：http://xbm.52xcode.cn

[T51] Scala：Hello World
来源：http://cgx.pycfn.com

println("Hello")
来源：http://ewr.shangyingyoupin.top

[T52] Scala：变量
来源：http://jmm.sweek.top

val a = 1;  var b = 2
来源：http://byo.jlsjyb.cn

[T53] Scala：字符串插值
来源：http://fjk.jinqigfzy.top

s"值: $b"
来源：http://ibq.bbcook.cn

[T54] Scala：集合映射
来源：http://mql.yj202588.top

List(1, 2, 3).map(_ * 2)
来源：http://dab.yj20258888.top

[T55] Scala：集合过滤
来源：http://bem.fehbvm.com

List(1, 2, 3).filter(_ > 1)
来源：http://tvc.tianlin.xyz

[T56] Scala：样例类
来源：http://big.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://dza.hesvh.cn

[T57] Scala：模式匹配
来源：http://sqa.pycfn.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://xde.meibo888.top

[T58] Scala：函数定义
来源：http://jap.yuxming.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rnq.fzhhl.top

[T59] Scala：循环
来源：http://amu.wangdashe.top

for (i <- 1 to 10) println(i)
来源：http://dhf.xuetiantiany.cn

[T60] Scala：折叠
来源：http://pne.tarul.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ooj.c1oappe.top

================================================================================
来源：http://aox.nwbrower.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://igd.ydzc1.top

================================================================================
来源：http://wsm.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://dnh.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://ayt.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://dcu.tianlin.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lra.9152youxi.cn

[U03] Py：加载 .env 配置
来源：http://ulj.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ibr.haohaochexian.top

[U04] Py：变量调试打印
来源：http://rxe.tian-w.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qrq.havefunace.top

[U05] Py：列表去重且保序
来源：http://cdy.daria6918.cn

list(dict.fromkeys(arr))
来源：http://knn.xuanzx.com

[U06] Py：合并两个字典
来源：http://edr.cucudq.cn

{**a, **b}
来源：http://ool.haohaochexian.top

[U07] Py：反转字典键值
来源：http://mxi.gzhubu.top

{v: k for k, v in d.items()}
来源：http://xin.jinqigfzy.top

[U08] Py：展平二维列表
来源：http://hhm.nanxuanxn.top

[y for x in nested for y in x]
来源：http://vec.hywenlv.cn

[U09] Py：字典取最大值的键
来源：http://vnn.sjlbkw.cn

max(d, key=d.get)
来源：http://aej.uphjek.com

[U10] Py：按值排序字典
来源：http://pyq.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vfj.shanyushiyangkeji.top

[U11] Py：生成器表达式
来源：http://hcs.fehbvm.com

(x * 2 for x in arr)
来源：http://mhc.ctjpmb.com

[U12] Py：取出现最多的 3 个元素
来源：http://vje.havefunace.top

Counter(arr).most_common(3)
来源：http://nai.aizwys.cn

[U13] Py：固定长度队列
来源：http://rin.jyoumei.cn

deque(maxlen=10)
来源：http://rbi.guowangkeji.top

[U14] Py：分组收集到列表
来源：http://yhp.mhx1999.top

defaultdict(list)
来源：http://ppr.fzhhl.top

[U15] Py：高精度计时
来源：http://vze.0kj1m.cn

t = time.perf_counter()
来源：http://myt.yuanzhike.top

[U16] Py：命令行参数解析
来源：http://sgn.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cpt.havefunace.top

[U17] Py：初始化日志
来源：http://eym.aibaodan.cn

logging.basicConfig(level=logging.INFO)
来源：http://pph.shzxlz.cn

[U18] Py：预编译正则
来源：http://asl.zhaomingkeji.xyz

pat = re.compile(r"\d+")
来源：http://xqb.jyoumei.cn

[U19] Py：正则替换带回调
来源：http://bsk.hfpthk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kdu.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://kye.jinqigufen.top

@functools.lru_cache(maxsize=None)
来源：http://hgg.zhixingplan.top

[U21] Py：自定义上下文管理器
来源：http://ukk.cqqwz.cn

@contextlib.contextmanager
来源：http://nzw.jinghuilouyu.cn

[U22] Py：矩阵转置
来源：http://okw.nanxinkj.top

list(zip(*m))
来源：http://scx.sjlbkw.cn

[U23] Py：分块读取大文件
来源：http://tts.cheryme.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nux.xylfe.cn

[U24] Py：路径操作
来源：http://avh.yfazqb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nsf.xingfuxueyuan.xyz

[U25] Py：CSV 按字典读
来源：http://rrf.hfpthk.cn

csv.DictReader(f)
来源：http://mnx.jinqigfzy.top

[U26] Py：并发下载
来源：http://liv.gaohongyu789.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tvl.yuanzhike.top

[U27] Py：异步 HTTP
来源：http://wde.hysaishi.cn

aiohttp.ClientSession() 配合 async with
来源：http://afy.hongshengwenyu.top

[U28] Py：类型别名
来源：http://lhq.hongshengwenyu.top

UserId = int
来源：http://fda.tarul.cn

[U29] Py：属性校验
来源：http://laf.vqdsnc.cn

@property 与 @x.setter 配合
来源：http://gtv.hywenlv.cn

[U30] Py：数据类
来源：http://xgq.nwbrower.top

@dataclass(slots=True)
来源：http://qgi.sysykeji.top

[U31] Py：单测
来源：http://zgt.9152youxi.cn

python -m pytest -q
来源：http://udh.zhongyouzk.top

[U32] Py：代码格式化
来源：http://fyz.zhengqikj.top

ruff format . && ruff check --fix .
来源：http://oxq.sxryk.cn

[U33] Py：打包发布
来源：http://fde.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://vfy.yongpay.top

[U34] Py：判断编码
来源：http://mpo.uphjek.com

chardet.detect(raw)
来源：http://axa.tian-w.cn

[U35] Py：发送邮件
来源：http://cch.hcnkem.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ekl.yj202588.top

[U36] Py：定时任务
来源：http://wnr.xingfuxueyuan.xyz

schedule.every(10).minutes.do(job)
来源：http://pzv.yfazqb.com

[U37] Py：读写 Excel
来源：http://ohz.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://axl.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://xer.havefunace.top

Path(__file__).resolve().parent
来源：http://fdr.jqgfzy.top

[U39] Py：判断是否在交互环境
来源：http://kcf.jianghu66.top

sys.stdout.isatty()
来源：http://vvl.havefunace.top

[U40] Py：打印到标准错误
来源：http://iey.ctjpmb.com

print("err", file=sys.stderr)
来源：http://dkm.ywan-chungtsiang.top

[U41] PHP：初始化 Composer 项目
来源：http://hjv.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qvx.nanxinkj.top

[U42] PHP：PSR-4 自动加载
来源：http://mlp.snrcjt.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vzn.zhijiandao.cn

[U43] PHP：声明命名空间
来源：http://wke.yonumen.top

namespace App\Http;
来源：http://ure.fengsongda.top

[U44] PHP：开启严格类型
来源：http://nlu.shangyingyoupin.top

declare(strict_types=1);
来源：http://bbv.bbcook.cn

[U45] PHP：类型声明与返回类型
来源：http://ddp.ctjpmb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://cwg.zhengqikj.top

[U46] PHP：可空类型
来源：http://dmx.ydzc1.top

?string $name = null
来源：http://nsz.hcnkem.com

[U47] PHP：联合类型
来源：http://eho.cdnleiting.top

int|string $id
来源：http://xds.xinyue.icu

[U48] PHP：纯枚举
来源：http://gek.andypj.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://okj.sweek.top

[U49] PHP：只读属性
来源：http://cfz.ivvv.top

public readonly string $name
来源：http://tos.tanke756.top

[U50] PHP：构造器属性提升
来源：http://rpa.jinqigufen.top

public function __construct(private int $id) {}
来源：http://zup.ivvv.top

[U51] PHP：数组解构
来源：http://olz.shanyushiyangtech.top

[$a, $b] = $arr;
来源：http://ech.bbcook.cn

[U52] PHP：箭头函数
来源：http://qsy.ywan-chungtsiang.top

$double = fn($x) => $x * 2;
来源：http://yyv.hnqzz.top

[U53] PHP：空合并运算符
来源：http://hwk.fzhhl.top

$v = $a ?? $b ?? "default";
来源：http://zxz.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://evw.hywenlv.cn

$obj?->method()
来源：http://jik.bjfxy.top

[U55] PHP：match 表达式
来源：http://vpo.shangyingyoupin.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zwf.tian-w.cn

[U56] PHP：命名参数
来源：http://fct.ctjpmb.com

f(a: 1, b: 2)
来源：http://mjc.cqqwz.cn

[U57] PHP：字符串插值
来源：http://rko.nwbrower.top

"值: {$a}"
来源：http://dst.yanxiufei.cn

[U58] PHP：数组三件套
来源：http://yxm.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://crx.hcnkem.com

[U59] PHP：自定义排序
来源：http://llb.zdqjudy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nle.mhx1999.top

[U60] PHP：JSON 编解码
来源：http://dpl.jlsjyb.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zmq.feifeiyinyue.top

[U61] PHP：正则
来源：http://vdy.xuanzx.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ekf.cdnleiting.top

[U62] PHP：日期对象
来源：http://shh.hfpthk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aew.hnqzz.top

[U63] PHP：文件读写
来源：http://ofv.aizwys.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://khg.yuxming.cn

[U64] PHP：目录遍历
来源：http://fpj.haohaochexian.top

glob("dir/*.php");  scandir("dir");
来源：http://szt.316326.xyz

[U65] PHP：会话
来源：http://dpu.zhijiandao.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wsm.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://gaj.guannengcc.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qox.vqdsnc.cn

[U67] PHP：处理文件上传
来源：http://dlm.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jnd.guannengcc.top

[U68] PHP：PDO 连接
来源：http://tpq.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://whu.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://gvc.aizwys.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hcj.bbcook.cn

[U70] PHP：PDO 事务
来源：http://pkx.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nay.jinqigfzy.top

[U71] PHP：抛出异常
来源：http://lxz.zhixingplan.top

throw new RuntimeException("失败", 500);
来源：http://rje.kuanghao11.cn

[U72] PHP：写错误日志
来源：http://bia.fanxiaobao.xyz

error_log("失败: " . $e->getMessage());
来源：http://jpy.yueranfly.top

[U73] PHP：读取 ini 配置
来源：http://rnc.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://jss.hnxiangtu.top

[U74] PHP：读取环境变量
来源：http://sbi.zhongyouzk.top

getenv("APP_ENV") ?: "production"
来源：http://gdk.ehwqpu.com

[U75] PHP：依赖注入
来源：http://awp.jinqigfzy.top

composer require psr/container
来源：http://xfc.redwolf501.top

[U76] PHP：简单路由
来源：http://foh.quarkkingdee.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lyx.yj20258.top

[U77] PHP：模板渲染
来源：http://srp.meibo888.top

composer require twig/twig
来源：http://dvv.feifeiyinyue.top

[U78] PHP：单元测试
来源：http://oty.zhoulong.xyz

composer require --dev phpunit/phpunit
来源：http://mhz.xingfuxueyuan.xyz

[U79] PHP：静态分析
来源：http://yyn.jinyuanbaomall.cn

composer require --dev phpstan/phpstan
来源：http://jnx.birdmap.top

[U80] PHP：代码规范修复
来源：http://zbm.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hws.iojbl.cn

[U81] JS：初始化项目
来源：http://soi.svipenyu.cn

npm init -y;  npm i express
来源：http://ufi.ydjk.org.cn

[U82] JS：package.json 脚本
来源：http://fxt.wangshuangyany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sof.daxiang520.top

[U83] JS：ES Module 导入导出
来源：http://cmv.mhx1999.top

export const a = 1;  import { a } from "./m.js";
来源：http://shl.snrcjt.cn

[U84] JS：CommonJS 写法
来源：http://nfq.shzxlz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kdr.ctjpmb.com

[U85] JS：可选链
来源：http://ipz.yonumen.top

a?.b?.c
来源：http://ayg.bbcook.cn

[U86] JS：空值合并
来源：http://uys.jinghuilouyu.cn

a ?? b
来源：http://kim.yanxiufei.cn

[U87] JS：解构默认值
来源：http://zoi.nwbrower.top

const { a = 1, b = 2 } = obj;
来源：http://ypy.ybcxt.top

[U88] JS：对象展开合并
来源：http://buy.gaohongyu789.top

{ ...a, ...b }
来源：http://pec.shzxlz.cn

[U89] JS：数组去重
来源：http://hnq.zhixingplan.top

[...new Set(arr)]
来源：http://ddx.shanyushiyangkeji.top

[U90] JS：数字数组排序
来源：http://nkp.c1oappe.top

[...arr].sort((a, b) => a - b)
来源：http://icl.zhijiandao.cn

[U91] JS：对象键值遍历
来源：http://soi.chenzaomai.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tqk.snrcjt.cn

[U92] JS：深拷贝
来源：http://phd.jinghuilouyu.cn

structuredClone(obj)
来源：http://duz.jinqigfzy.top

[U93] JS：模板字符串
来源：http://fzo.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://lqb.hammf.cn

[U94] JS：箭头函数
来源：http://hmg.yuanzhike.top

const double = x => x * 2;
来源：http://bzn.havefunace.top

[U95] JS：Promise 包装
来源：http://gjv.tanke756.top

new Promise((resolve, reject) => {})
来源：http://gpj.jlsjyb.cn

[U96] JS：async/await 与异常
来源：http://tar.hfpthk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aan.ywan-chungtsiang.top

[U97] JS：并发请求
来源：http://yym.jinghuilouyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bdp.zhongyouzk.top

[U98] JS：fetch 带 JSON
来源：http://kyu.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xjx.zdbjq.cn

[U99] JS：事件监听
来源：http://ucr.jlsjyb.cn

el.addEventListener("click", e => {})
来源：http://mvf.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://pgt.jinqigufen.top

document.querySelector(".item")
来源：http://rol.shanyushiyangkeji.top

[U101] JS：classList 操作
来源：http://emc.0kj1m.cn

el.classList.toggle("active")
来源：http://scv.nanxuanxn.top

[U102] JS：本地存储
来源：http://fmu.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jfk.xinyue.icu

[U103] JS：定时器
来源：http://unq.hammf.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://npi.jianghu66.top

[U104] JS：防抖
来源：http://cwd.gzhubu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ako.hnxiangtu.top

[U105] JS：节流
来源：http://hdb.sufxvd.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wvr.xuetiantiany.cn

[U106] JS：日期格式化
来源：http://nrh.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ywt.tianlin.xyz

[U107] JS：数字千分位
来源：http://lxv.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gem.kuanghao11.cn

[U108] JS：随机整数
来源：http://smz.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eib.yj20258.top

[U109] JS：数组分组
来源：http://ifm.bbcook.cn

Object.groupBy(arr, x => x.type)
来源：http://jcw.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://bbc.gogol.net.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dtx.zhiwuduotai.top

[U111] JS：对象转 Map
来源：http://tej.sjlbkw.cn

new Map(Object.entries(obj))
来源：http://dsg.mhx1999.top

[U112] JS：字符串补位
来源：http://edt.xingfuxueyuan.xyz

"7".padStart(3, "0")
来源：http://qnf.pengpengdd.cyou

[U113] JS：正则替换全部
来源：http://ttt.sxryk.cn

s.replaceAll("a", "b")
来源：http://wul.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://uhq.fktsv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://src.uphjek.com

[U115] JS：生成 UUID
来源：http://rjk.havefunace.top

crypto.randomUUID()
来源：http://rkg.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://vnl.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://lfr.jiagoushi.top

[U117] JS：单元测试
来源：http://wqa.xuetiantiany.cn

npm i -D vitest;  npx vitest
来源：http://hde.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://wxa.0kj1m.cn

npm i -D vite;  npx vite
来源：http://jrb.xziqi.cn

[U119] JS：生产构建
来源：http://dga.shanyushiyangkeji.top

npx vite build
来源：http://ryc.sjlbkw.cn

[U120] JS：读取环境变量（Vite）
来源：http://vvw.fanxiaobao.xyz

import.meta.env.VITE_API_URL
来源：http://qib.xuanzx.com

================================================================================
来源：http://dco.gzhubu.top

统计汇总
来源：http://tls.tian-w.cn

================================================================================
来源：http://mdj.zdqjudy.top

按语言统计（条）：
来源：http://urh.ybcxt.top

Python ......... 252
来源：http://lfw.uphjek.com

PHP ............ 252
来源：http://wqt.snrcjt.cn

JavaScript ..... 252
来源：http://qmt.shanyushiyangtech.top

TypeScript ..... 212
来源：http://dwy.jianghu66.top


<!-- 参考信息 -->