代发 wailian999

[T31] Lua：Hello World
来源：http://jyg.hfpthk.cn

print("Hello")
来源：http://vsc.hywenlv.cn

[T32] Lua：局部变量
来源：http://htx.shuidangran.top

local a = 1
来源：http://hap.sxryk.cn

[T33] Lua：表（数组）
来源：http://aos.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://bsu.0kj1m.cn

[T34] Lua：遍历表
来源：http://oiu.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ook.birdmap.top

[T35] Lua：字典表
来源：http://qeg.fktsv.cn

local d = { a = 1 };  d.b = 2
来源：http://wbc.bjfxy.top

[T36] Lua：函数
来源：http://lhf.hysaishi.cn

function add(a, b) return a + b end
来源：http://kjr.tanke756.top

[T37] Lua：字符串拼接
来源：http://lqo.shuidangran.top

"a" .. "b"
来源：http://vqm.shangyingyoupin.top

[T38] Lua：条件
来源：http://iss.hywenlv.cn

if x > 0 then print("正") end
来源：http://ndp.yj20258888.top

[T39] Lua：模式匹配
来源：http://jrf.yanxiufei.cn

string.find(s, "%d+")
来源：http://auf.hcnkem.com

[T40] Lua：元表
来源：http://hoe.gaohongyu789.top

setmetatable({}, { __index = base })
来源：http://kiu.jinyuanbaomall.cn

[T41] Perl：Hello World
来源：http://bqx.pycfn.com

print "Hello\n";
来源：http://nks.ehwqpu.com

[T42] Perl：变量类型
来源：http://gol.pycfn.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tqt.tian-w.cn

[T43] Perl：字符串插值
来源：http://hpj.yuanzhike.top

"值: $a"
来源：http://nhy.hnqzz.top

[T44] Perl：条件
来源：http://blh.tanke756.top

if ($a > 0) { print "正"; }
来源：http://jlq.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://ypk.shanyushiyangkeji.top

for my $x (@arr) { print $x; }
来源：http://dhr.tanke756.top

[T46] Perl：哈希操作
来源：http://skk.wangdashe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ihe.nwbrower.top

[T47] Perl：正则捕获
来源：http://yas.sufxvd.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lsw.uphjek.com

[T48] Perl：正则替换
来源：http://nxg.9152youxi.cn

$s =~ s/old/new/g;
来源：http://kwl.aizwys.cn

[T49] Perl：函数
来源：http://cjr.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nmw.yj20258888.top

[T50] Perl：逐行读文件
来源：http://xen.yueranfly.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bhv.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://rpv.cheryme.top

[T51] Scala：Hello World
来源：http://ayu.jinyuanbaomall.cn

println("Hello")
来源：http://oqu.c1oappe.top

[T52] Scala：变量
来源：http://ari.meibo888.top

val a = 1;  var b = 2
来源：http://phn.chenlongwang.top

[T53] Scala：字符串插值
来源：http://ime.xingfuxueyuan.xyz

s"值: $b"
来源：http://wlw.pycfn.com

[T54] Scala：集合映射
来源：http://zoa.xinyue.icu

List(1, 2, 3).map(_ * 2)
来源：http://ktm.yj20258.top

[T55] Scala：集合过滤
来源：http://dop.andypj.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://rww.xylfe.cn

[T56] Scala：样例类
来源：http://jns.jinyuanbaomall.cn

case class User(name: String, age: Int)
来源：http://ygp.bbcook.cn

[T57] Scala：模式匹配
来源：http://tzz.quarkkingdee.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gvr.jinqigfzy.top

[T58] Scala：函数定义
来源：http://tch.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://ojo.gotoacloud.top

[T59] Scala：循环
来源：http://lom.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://lja.yuxming.cn

[T60] Scala：折叠
来源：http://hqj.iojbl.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tfy.quarkkingdee.top

================================================================================
来源：http://zeb.daxiang520.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xxz.yongpay.top

================================================================================
来源：http://nnv.jlsjyb.cn

[U01] Py：创建虚拟环境
来源：http://fas.dashuyun.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gic.ydzc1.top

[U02] Py：导出 / 安装依赖
来源：http://zrp.jqgfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jbc.aizwys.cn

[U03] Py：加载 .env 配置
来源：http://osk.xylfe.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nee.yongpay.top

[U04] Py：变量调试打印
来源：http://zcj.dashuyun.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://okr.52xcode.cn

[U05] Py：列表去重且保序
来源：http://afq.52xcode.cn

list(dict.fromkeys(arr))
来源：http://tlr.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://osj.haohaochexian.top

{**a, **b}
来源：http://nki.xinyue.icu

[U07] Py：反转字典键值
来源：http://isr.meibo888.top

{v: k for k, v in d.items()}
来源：http://pvx.fzhhl.top

[U08] Py：展平二维列表
来源：http://xga.yj202588.top

[y for x in nested for y in x]
来源：http://fia.iojbl.cn

[U09] Py：字典取最大值的键
来源：http://lxc.jlsjyb.cn

max(d, key=d.get)
来源：http://zok.tian-w.cn

[U10] Py：按值排序字典
来源：http://beh.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lcw.sxryk.cn

[U11] Py：生成器表达式
来源：http://rqz.gaohongyu789.top

(x * 2 for x in arr)
来源：http://ixz.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://brd.chenzaomai.com

Counter(arr).most_common(3)
来源：http://sie.jiagoushi.top

[U13] Py：固定长度队列
来源：http://atk.meibo888.top

deque(maxlen=10)
来源：http://mcg.dashuyun.cn

[U14] Py：分组收集到列表
来源：http://jer.fengsongda.top

defaultdict(list)
来源：http://vga.sufxvd.cn

[U15] Py：高精度计时
来源：http://grl.bbcook.cn

t = time.perf_counter()
来源：http://oth.jlsjyb.cn

[U16] Py：命令行参数解析
来源：http://eyq.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wlm.guowangkeji.top

[U17] Py：初始化日志
来源：http://hdg.feifeiyinyue.top

logging.basicConfig(level=logging.INFO)
来源：http://fym.hcnkem.com

[U18] Py：预编译正则
来源：http://emj.haohaochexian.top

pat = re.compile(r"\d+")
来源：http://qfj.jinyuanbaomall.cn

[U19] Py：正则替换带回调
来源：http://qvx.ivvv.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://deg.zdqjudy.top

[U20] Py：缓存函数结果
来源：http://pgu.aibaodan.cn

@functools.lru_cache(maxsize=None)
来源：http://rbx.hnqzz.top

[U21] Py：自定义上下文管理器
来源：http://bml.jqgufenzy.top

@contextlib.contextmanager
来源：http://afz.jlsjyb.cn

[U22] Py：矩阵转置
来源：http://lyz.kuanghao11.cn

list(zip(*m))
来源：http://ymf.quarkkingdee.top

[U23] Py：分块读取大文件
来源：http://uak.fanxiaobao.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ouj.fzhhl.top

[U24] Py：路径操作
来源：http://urg.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://liy.yuanzhike.top

[U25] Py：CSV 按字典读
来源：http://wsx.shangyingyoupin.top

csv.DictReader(f)
来源：http://vcg.fengsongda.top

[U26] Py：并发下载
来源：http://fsf.yonumen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hkl.svipenyu.cn

[U27] Py：异步 HTTP
来源：http://lqk.hysaishi.cn

aiohttp.ClientSession() 配合 async with
来源：http://kcy.0kj1m.cn

[U28] Py：类型别名
来源：http://utq.yueranfly.top

UserId = int
来源：http://sss.hammf.cn

[U29] Py：属性校验
来源：http://fzv.fehbvm.com

@property 与 @x.setter 配合
来源：http://qvd.wangdashe.top

[U30] Py：数据类
来源：http://nyc.zhongyouzk.top

@dataclass(slots=True)
来源：http://jft.sxryk.cn

[U31] Py：单测
来源：http://fgk.hnxiangtu.top

python -m pytest -q
来源：http://xlm.yvedp.cn

[U32] Py：代码格式化
来源：http://agd.yanxiufei.cn

ruff format . && ruff check --fix .
来源：http://sqw.wangdashe.top

[U33] Py：打包发布
来源：http://qys.yuanzhike.top

python -m build  （依赖 pyproject.toml）
来源：http://zgc.aibaodan.cn

[U34] Py：判断编码
来源：http://nke.shuidangran.top

chardet.detect(raw)
来源：http://knt.yanxiufei.cn

[U35] Py：发送邮件
来源：http://wpm.sxryk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://thz.jianghu66.top

[U36] Py：定时任务
来源：http://fza.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://ezm.gzhubu.top

[U37] Py：读写 Excel
来源：http://mcc.jinqigfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://qsa.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://zoh.hnxiangtu.top

Path(__file__).resolve().parent
来源：http://xrk.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://dhs.jqgfzy.top

sys.stdout.isatty()
来源：http://pfi.chenzaomai.com

[U40] Py：打印到标准错误
来源：http://brb.yongpay.top

print("err", file=sys.stderr)
来源：http://veb.zhixingplan.top

[U41] PHP：初始化 Composer 项目
来源：http://xax.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://khx.ydjk.org.cn

[U42] PHP：PSR-4 自动加载
来源：http://bfy.sufxvd.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://woj.shzxlz.cn

[U43] PHP：声明命名空间
来源：http://yqg.quarkkingdee.top

namespace App\Http;
来源：http://wpo.tian-w.cn

[U44] PHP：开启严格类型
来源：http://cwm.ivvv.top

declare(strict_types=1);
来源：http://suf.haohaochexian.top

[U45] PHP：类型声明与返回类型
来源：http://ecc.zhixingplan.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mhx.jqgfzy.top

[U46] PHP：可空类型
来源：http://iiq.ydzc1.top

?string $name = null
来源：http://ree.yuxming.cn

[U47] PHP：联合类型
来源：http://lou.sweek.top

int|string $id
来源：http://cmi.guowangkeji.top

[U48] PHP：纯枚举
来源：http://bmh.zhoulong.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zxe.yuanzhike.top

[U49] PHP：只读属性
来源：http://jtw.xziqi.cn

public readonly string $name
来源：http://pjz.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://qnd.pengpengdd.cyou

public function __construct(private int $id) {}
来源：http://ced.epnwcf.com

[U51] PHP：数组解构
来源：http://vxw.hammf.cn

[$a, $b] = $arr;
来源：http://jux.xuanzx.com

[U52] PHP：箭头函数
来源：http://cif.meibo888.top

$double = fn($x) => $x * 2;
来源：http://ybk.sxryk.cn

[U53] PHP：空合并运算符
来源：http://qej.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://dma.ehwqpu.com

[U54] PHP：空安全调用
来源：http://let.zhengqikj.top

$obj?->method()
来源：http://nal.tanke756.top

[U55] PHP：match 表达式
来源：http://wby.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nyg.ydjk.org.cn

[U56] PHP：命名参数
来源：http://ccy.yvedp.cn

f(a: 1, b: 2)
来源：http://psp.yueranfly.top

[U57] PHP：字符串插值
来源：http://ede.hnqzz.top

"值: {$a}"
来源：http://udq.bjfxy.top

[U58] PHP：数组三件套
来源：http://uet.ppjwa.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blv.zycfv.cn

[U59] PHP：自定义排序
来源：http://xoz.xinyue.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ifn.yonumen.top

[U60] PHP：JSON 编解码
来源：http://fdn.kuanghao11.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://etz.yfazqb.com

[U61] PHP：正则
来源：http://xuk.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rth.tian-w.cn

[U62] PHP：日期对象
来源：http://nmc.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xhn.sweek.top

[U63] PHP：文件读写
来源：http://gkm.zdqjudy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ese.hywenlv.cn

[U64] PHP：目录遍历
来源：http://qio.zhiwuduotai.top

glob("dir/*.php");  scandir("dir");
来源：http://uzv.nwbrower.top

[U65] PHP：会话
来源：http://bcn.jinyuanbaomall.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tdp.9152youxi.cn

[U66] PHP：设置 Cookie
来源：http://vhk.316326.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lly.fktsv.cn

[U67] PHP：处理文件上传
来源：http://hpc.zhoulong.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gdv.yfazqb.com

[U68] PHP：PDO 连接
来源：http://bdr.cdnleiting.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zcm.daxiang520.top

[U69] PHP：PDO 预处理
来源：http://kok.yuanzhike.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qph.hnxiangtu.top

[U70] PHP：PDO 事务
来源：http://gvg.nanxinkj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jiq.xuanzx.com

[U71] PHP：抛出异常
来源：http://blo.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://omz.jinghuilouyu.cn

[U72] PHP：写错误日志
来源：http://zvw.ydzc1.top

error_log("失败: " . $e->getMessage());
来源：http://fje.c1oappe.top

[U73] PHP：读取 ini 配置
来源：http://but.epnwcf.com

parse_ini_file("config.ini", true)
来源：http://fgm.sysykeji.top

[U74] PHP：读取环境变量
来源：http://qzd.wangdashe.top

getenv("APP_ENV") ?: "production"
来源：http://hyn.daxiang520.top

[U75] PHP：依赖注入
来源：http://ciw.jqgfzy.top

composer require psr/container
来源：http://kjd.bbcook.cn

[U76] PHP：简单路由
来源：http://pbz.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://phv.chenzaomai.com

[U77] PHP：模板渲染
来源：http://bms.zhijiandao.cn

composer require twig/twig
来源：http://wbs.cucudq.cn

[U78] PHP：单元测试
来源：http://pmi.uphjek.com

composer require --dev phpunit/phpunit
来源：http://pvj.hongshengwenyu.top

[U79] PHP：静态分析
来源：http://ouq.andypj.xyz

composer require --dev phpstan/phpstan
来源：http://vtf.zycfv.cn

[U80] PHP：代码规范修复
来源：http://pys.pengpengdd.cyou

composer require --dev friendsofphp/php-cs-fixer
来源：http://ojz.meibo888.top

[U81] JS：初始化项目
来源：http://oiy.fengsongda.top

npm init -y;  npm i express
来源：http://jav.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://geq.kuanghao11.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qyz.guannengcc.top

[U83] JS：ES Module 导入导出
来源：http://orn.gaohongyu789.top

export const a = 1;  import { a } from "./m.js";
来源：http://ggs.guowangkeji.top

[U84] JS：CommonJS 写法
来源：http://lls.zycfv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fre.yuanzhike.top

[U85] JS：可选链
来源：http://odn.hnqzz.top

a?.b?.c
来源：http://qio.xylfe.cn

[U86] JS：空值合并
来源：http://byg.nanxinkj.top

a ?? b
来源：http://wjs.guannengcc.top

[U87] JS：解构默认值
来源：http://jut.zhijiandao.cn

const { a = 1, b = 2 } = obj;
来源：http://unv.hesvh.cn

[U88] JS：对象展开合并
来源：http://did.9152youxi.cn

{ ...a, ...b }
来源：http://nqr.dianchejie.cn

[U89] JS：数组去重
来源：http://hkg.jqgufenzy.top

[...new Set(arr)]
来源：http://dnq.havefunace.top

[U90] JS：数字数组排序
来源：http://wyq.nwbrower.top

[...arr].sort((a, b) => a - b)
来源：http://meb.nanxuanxn.top

[U91] JS：对象键值遍历
来源：http://akn.vehdjk.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cpt.xuanzx.com

[U92] JS：深拷贝
来源：http://tdy.cucudq.cn

structuredClone(obj)
来源：http://tge.aibaodan.cn

[U93] JS：模板字符串
来源：http://ple.hammf.cn

`共 ${n} 条`
来源：http://nsq.fengsongda.top

[U94] JS：箭头函数
来源：http://tbl.jiagoushi.top

const double = x => x * 2;
来源：http://rty.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://pgc.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://pyg.jlsjyb.cn

[U96] JS：async/await 与异常
来源：http://ven.kuanghao11.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pgw.quarkkingdee.top

[U97] JS：并发请求
来源：http://els.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jyn.9152youxi.cn

[U98] JS：fetch 带 JSON
来源：http://jzn.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hse.redwolf501.top

[U99] JS：事件监听
来源：http://izh.hywenlv.cn

el.addEventListener("click", e => {})
来源：http://ehj.nanxinkj.top

[U100] JS：DOM 查询
来源：http://lzo.hysaishi.cn

document.querySelector(".item")
来源：http://vkh.hnqzz.top

[U101] JS：classList 操作
来源：http://rvx.vqdsnc.cn

el.classList.toggle("active")
来源：http://vaw.smart0.xyz

[U102] JS：本地存储
来源：http://rcn.iojbl.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ojc.aibaodan.cn

[U103] JS：定时器
来源：http://bjg.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mhh.c1oappe.top

[U104] JS：防抖
来源：http://ott.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ttv.tanke756.top

[U105] JS：节流
来源：http://iwp.yangfankeji.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jek.zhixingplan.top

[U106] JS：日期格式化
来源：http://uvb.0kj1m.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://moa.nanxuanxn.top

[U107] JS：数字千分位
来源：http://rvf.shanyushiyangtech.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://olt.jlsjyb.cn

[U108] JS：随机整数
来源：http://klu.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jom.quarkkingdee.top

[U109] JS：数组分组
来源：http://bfn.haohaochexian.top

Object.groupBy(arr, x => x.type)
来源：http://ufx.xziqi.cn

[U110] JS：数组分块
来源：http://owm.yuanzhike.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nth.pengpengdd.cyou

[U111] JS：对象转 Map
来源：http://mqp.sweek.top

new Map(Object.entries(obj))
来源：http://mvs.jiagoushi.top

[U112] JS：字符串补位
来源：http://crq.xuanzx.com

"7".padStart(3, "0")
来源：http://wka.chenjidiqi.icu

[U113] JS：正则替换全部
来源：http://cfs.xziqi.cn

s.replaceAll("a", "b")
来源：http://mxm.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://dro.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://spy.havefunace.top

[U115] JS：生成 UUID
来源：http://sxj.nanxuanxn.top

crypto.randomUUID()
来源：http://ffl.chenzaomai.com

[U116] JS：类型检查（JSDoc）
来源：http://ynz.yueranfly.top

/** @param {string} name */ function f(name) {}
来源：http://pui.hesvh.cn

[U117] JS：单元测试
来源：http://trv.feifeiyinyue.top

npm i -D vitest;  npx vitest
来源：http://bfs.yanxiufei.cn

[U118] JS：开发服务器
来源：http://qgo.jinqigfzy.top

npm i -D vite;  npx vite
来源：http://ntt.zhaomingkeji.xyz


<!-- 参考信息 -->