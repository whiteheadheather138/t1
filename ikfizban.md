代发 wailian999

[T33] Lua：表（数组）
来源：http://www.pycfn.com

local t = {1, 2, 3};  t[4] = 4
来源：http://sjt.bjfxy.top

[T34] Lua：遍历表
来源：http://jko.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nci.shzxlz.cn

[T35] Lua：字典表
来源：http://dlq.kuanghao11.cn

local d = { a = 1 };  d.b = 2
来源：http://kgd.xuetiantiany.cn

[T36] Lua：函数
来源：http://dix.hnxiangtu.top

function add(a, b) return a + b end
来源：http://cam.chenjidiqi.icu

[T37] Lua：字符串拼接
来源：http://ueu.pengpengdd.cyou

"a" .. "b"
来源：http://khf.haohaochexian.top

[T38] Lua：条件
来源：http://hor.hnqzz.top

if x > 0 then print("正") end
来源：http://mvi.cqqwz.cn

[T39] Lua：模式匹配
来源：http://tvt.c1oappe.top

string.find(s, "%d+")
来源：http://ahr.guowangkeji.top

[T40] Lua：元表
来源：http://fnq.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://zar.fehbvm.com

[T41] Perl：Hello World
来源：http://mmp.nanxinkj.top

print "Hello\n";
来源：http://mkz.kuanghao11.cn

[T42] Perl：变量类型
来源：http://sqf.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://atz.dashuyun.cn

[T43] Perl：字符串插值
来源：http://oax.wangdashe.top

"值: $a"
来源：http://vod.aizwys.cn

[T44] Perl：条件
来源：http://wfq.andypj.xyz

if ($a > 0) { print "正"; }
来源：http://ceb.shzxlz.cn

[T45] Perl：数组遍历
来源：http://fhq.yuxming.cn

for my $x (@arr) { print $x; }
来源：http://jnk.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://qyp.cashguo.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gbo.0kj1m.cn

[T47] Perl：正则捕获
来源：http://ihq.birdmap.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://stx.9152youxi.cn

[T48] Perl：正则替换
来源：http://pla.svipenyu.cn

$s =~ s/old/new/g;
来源：http://fuc.havefunace.top

[T49] Perl：函数
来源：http://yjz.yuanzhike.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rtr.zdqjudy.top

[T50] Perl：逐行读文件
来源：http://nmb.guannengcc.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wcs.shuidangran.top

while (my $line = <$fh>) { print $line; }
来源：http://cdt.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://dvv.zhoulong.xyz

println("Hello")
来源：http://lti.uphjek.com

[T52] Scala：变量
来源：http://hjd.wangdashe.top

val a = 1;  var b = 2
来源：http://rjl.xingfuxueyuan.xyz

[T53] Scala：字符串插值
来源：http://glu.yangfankeji.com

s"值: $b"
来源：http://qke.ppjwa.cn

[T54] Scala：集合映射
来源：http://krb.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://tyt.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://kmu.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ntp.zdbjq.cn

[T56] Scala：样例类
来源：http://ffa.aibaodan.cn

case class User(name: String, age: Int)
来源：http://lqf.fengsongda.top

[T57] Scala：模式匹配
来源：http://mlr.gogol.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vje.316326.xyz

[T58] Scala：函数定义
来源：http://bpg.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://prg.hywenlv.cn

[T59] Scala：循环
来源：http://vuq.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://hkg.xylfe.cn

[T60] Scala：折叠
来源：http://eij.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wtw.tanke756.top

================================================================================
来源：http://wik.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pgj.aizwys.cn

================================================================================
来源：http://jmv.gotoacloud.top

[U01] Py：创建虚拟环境
来源：http://dzc.shzxlz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kty.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://tps.andypj.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mde.ybcxt.top

[U03] Py：加载 .env 配置
来源：http://lza.shanyushiyangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xqs.xziqi.cn

[U04] Py：变量调试打印
来源：http://xpt.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oct.shanyushiyangtech.top

[U05] Py：列表去重且保序
来源：http://ofz.fzhhl.top

list(dict.fromkeys(arr))
来源：http://aps.ivvv.top

[U06] Py：合并两个字典
来源：http://qqm.tian-w.cn

{**a, **b}
来源：http://jkv.zycfv.cn

[U07] Py：反转字典键值
来源：http://khm.jqgufenzy.top

{v: k for k, v in d.items()}
来源：http://vmv.yvedp.cn

[U08] Py：展平二维列表
来源：http://fqw.jqgufenzy.top

[y for x in nested for y in x]
来源：http://anp.hfpthk.cn

[U09] Py：字典取最大值的键
来源：http://klx.yj20258.top

max(d, key=d.get)
来源：http://uct.tarul.cn

[U10] Py：按值排序字典
来源：http://efw.fzhhl.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jrc.yanxiufei.cn

[U11] Py：生成器表达式
来源：http://bzh.fzhhl.top

(x * 2 for x in arr)
来源：http://ttd.feifeiyinyue.top

[U12] Py：取出现最多的 3 个元素
来源：http://zdp.xuetiantiany.cn

Counter(arr).most_common(3)
来源：http://yqa.tanke756.top

[U13] Py：固定长度队列
来源：http://qzc.zhiwuduotai.top

deque(maxlen=10)
来源：http://ulm.tian-w.cn

[U14] Py：分组收集到列表
来源：http://rej.hcnkem.com

defaultdict(list)
来源：http://dvv.guowangkeji.top

[U15] Py：高精度计时
来源：http://cec.zhongyouzk.top

t = time.perf_counter()
来源：http://ion.xuanzx.com

[U16] Py：命令行参数解析
来源：http://nwp.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lvp.cucudq.cn

[U17] Py：初始化日志
来源：http://ndl.52xcode.cn

logging.basicConfig(level=logging.INFO)
来源：http://zut.52xcode.cn

[U18] Py：预编译正则
来源：http://ndh.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://cak.zhongyouzk.top

[U19] Py：正则替换带回调
来源：http://uip.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cla.uphjek.com

[U20] Py：缓存函数结果
来源：http://lbk.zhijiandao.cn

@functools.lru_cache(maxsize=None)
来源：http://btn.xylfe.cn

[U21] Py：自定义上下文管理器
来源：http://dew.guannengcc.top

@contextlib.contextmanager
来源：http://yul.0kj1m.cn

[U22] Py：矩阵转置
来源：http://dml.cashguo.top

list(zip(*m))
来源：http://lpt.cheryme.top

[U23] Py：分块读取大文件
来源：http://zvt.jianghu66.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bqi.shzxlz.cn

[U24] Py：路径操作
来源：http://nfq.yfazqb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sda.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://unf.hnqzz.top

csv.DictReader(f)
来源：http://lzg.jinqigufen.top

[U26] Py：并发下载
来源：http://vly.gogol.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://spu.jinghuilouyu.cn

[U27] Py：异步 HTTP
来源：http://fqj.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://cqx.yongpay.top

[U28] Py：类型别名
来源：http://des.sjlbkw.cn

UserId = int
来源：http://xhc.smart0.xyz

[U29] Py：属性校验
来源：http://lgb.zhiwuduotai.top

@property 与 @x.setter 配合
来源：http://wnt.chenjidiqi.icu

[U30] Py：数据类
来源：http://anm.jqgfzy.top

@dataclass(slots=True)
来源：http://twd.sufxvd.cn

[U31] Py：单测
来源：http://bwx.hesvh.cn

python -m pytest -q
来源：http://xzt.ehwqpu.com

[U32] Py：代码格式化
来源：http://ywk.zycfv.cn

ruff format . && ruff check --fix .
来源：http://orl.fanxiaobao.xyz

[U33] Py：打包发布
来源：http://kpm.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://kwk.sjlbkw.cn

[U34] Py：判断编码
来源：http://kzx.fehbvm.com

chardet.detect(raw)
来源：http://rmg.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://rtk.zhoulong.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ckx.tanke756.top

[U36] Py：定时任务
来源：http://zhd.wangdashe.top

schedule.every(10).minutes.do(job)
来源：http://jth.hcnkem.com

[U37] Py：读写 Excel
来源：http://goz.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://sfa.hammf.cn

[U38] Py：获取脚本所在目录
来源：http://vyb.tarul.cn

Path(__file__).resolve().parent
来源：http://qpn.52xcode.cn

[U39] Py：判断是否在交互环境
来源：http://uwp.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://pog.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://pbs.fehbvm.com

print("err", file=sys.stderr)
来源：http://xkc.xinyue.icu

[U41] PHP：初始化 Composer 项目
来源：http://xgi.hfpthk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://toa.chenlongwang.top

[U42] PHP：PSR-4 自动加载
来源：http://xvv.feifeiyinyue.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yui.shanyushiyangkeji.top

[U43] PHP：声明命名空间
来源：http://fwi.dianchejie.cn

namespace App\Http;
来源：http://mrr.hnqzz.top

[U44] PHP：开启严格类型
来源：http://jun.shanyushiyangtech.top

declare(strict_types=1);
来源：http://jad.nanxinkj.top

[U45] PHP：类型声明与返回类型
来源：http://dcc.zhengqikj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ptp.sufxvd.cn

[U46] PHP：可空类型
来源：http://pxt.c1oappe.top

?string $name = null
来源：http://xfn.zhengqikj.top

[U47] PHP：联合类型
来源：http://unk.hcnkem.com

int|string $id
来源：http://cfg.xinyue.icu

[U48] PHP：纯枚举
来源：http://mtf.andypj.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://anv.c1oappe.top

[U49] PHP：只读属性
来源：http://yky.xingfuxueyuan.xyz

public readonly string $name
来源：http://zeu.ydjk.org.cn

[U50] PHP：构造器属性提升
来源：http://wvu.ydzc1.top

public function __construct(private int $id) {}
来源：http://siv.fzhhl.top

[U51] PHP：数组解构
来源：http://bly.chenzaomai.com

[$a, $b] = $arr;
来源：http://jha.ywan-chungtsiang.top

[U52] PHP：箭头函数
来源：http://uqy.andypj.xyz

$double = fn($x) => $x * 2;
来源：http://doq.ctjpmb.com

[U53] PHP：空合并运算符
来源：http://cah.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://jqc.yfazqb.com

[U54] PHP：空安全调用
来源：http://txf.gogol.net.cn

$obj?->method()
来源：http://ilw.haohaochexian.top

[U55] PHP：match 表达式
来源：http://ooc.daxiang520.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tnr.epnwcf.com

[U56] PHP：命名参数
来源：http://hmm.gaohongyu789.top

f(a: 1, b: 2)
来源：http://yup.jinqigufen.top

[U57] PHP：字符串插值
来源：http://vlt.yj20258.top

"值: {$a}"
来源：http://thv.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://jqk.0kj1m.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xko.guannengcc.top

[U59] PHP：自定义排序
来源：http://erv.tianlin.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://glq.haohaochexian.top

[U60] PHP：JSON 编解码
来源：http://xgy.316326.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hek.yangfankeji.com

[U61] PHP：正则
来源：http://zjc.hnqzz.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jqr.shuidangran.top

[U62] PHP：日期对象
来源：http://nna.mhx1999.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qcu.jqgfzy.top

[U63] PHP：文件读写
来源：http://yeh.chenzaomai.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pbq.ehwqpu.com

[U64] PHP：目录遍历
来源：http://uoi.316326.xyz

glob("dir/*.php");  scandir("dir");
来源：http://ujl.zhongyouzk.top

[U65] PHP：会话
来源：http://glc.ybcxt.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xry.fehbvm.com

[U66] PHP：设置 Cookie
来源：http://udl.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wdf.jqgufenzy.top

[U67] PHP：处理文件上传
来源：http://abi.tanke756.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://phm.hesvh.cn

[U68] PHP：PDO 连接
来源：http://hnq.nanxuanxn.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nsq.vehdjk.com

[U69] PHP：PDO 预处理
来源：http://spc.hywenlv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bpk.jianghu66.top

[U70] PHP：PDO 事务
来源：http://blo.tanke756.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bst.hysaishi.cn

[U71] PHP：抛出异常
来源：http://znn.cucudq.cn

throw new RuntimeException("失败", 500);
来源：http://dql.c1oappe.top

[U72] PHP：写错误日志
来源：http://xqq.andypj.xyz

error_log("失败: " . $e->getMessage());
来源：http://yvr.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://zvp.shzxlz.cn

parse_ini_file("config.ini", true)
来源：http://lfe.hcnkem.com

[U74] PHP：读取环境变量
来源：http://fac.ctjpmb.com

getenv("APP_ENV") ?: "production"
来源：http://doe.jlsjyb.cn

[U75] PHP：依赖注入
来源：http://ish.xylfe.cn

composer require psr/container
来源：http://ple.sufxvd.cn

[U76] PHP：简单路由
来源：http://kgy.cheryme.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jal.jinqigfzy.top

[U77] PHP：模板渲染
来源：http://ioc.hesvh.cn

composer require twig/twig
来源：http://cwh.bjfxy.top

[U78] PHP：单元测试
来源：http://rne.shanyushiyangtech.top

composer require --dev phpunit/phpunit
来源：http://ohb.aizwys.cn

[U79] PHP：静态分析
来源：http://pwg.jinqigfzy.top

composer require --dev phpstan/phpstan
来源：http://cry.c1oappe.top

[U80] PHP：代码规范修复
来源：http://dca.xuetiantiany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yhn.andypj.xyz

[U81] JS：初始化项目
来源：http://kwz.meibo888.top

npm init -y;  npm i express
来源：http://uhb.zycfv.cn

[U82] JS：package.json 脚本
来源：http://qtj.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qeb.zhixingplan.top

[U83] JS：ES Module 导入导出
来源：http://ljo.vqdsnc.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fjk.yueranfly.top

[U84] JS：CommonJS 写法
来源：http://awv.wangshuangyany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rdy.jinyuanbaomall.cn

[U85] JS：可选链
来源：http://eul.cucudq.cn

a?.b?.c
来源：http://uvn.wangshuangyany.cn

[U86] JS：空值合并
来源：http://fvs.sweek.top

a ?? b
来源：http://jhq.sxryk.cn

[U87] JS：解构默认值
来源：http://uuz.ybcxt.top

const { a = 1, b = 2 } = obj;
来源：http://sqv.uphjek.com

[U88] JS：对象展开合并
来源：http://qds.sysykeji.top

{ ...a, ...b }
来源：http://oti.xuanzx.com

[U89] JS：数组去重
来源：http://thk.yfazqb.com

[...new Set(arr)]
来源：http://gao.yj202588.top

[U90] JS：数字数组排序
来源：http://imt.wangdashe.top

[...arr].sort((a, b) => a - b)
来源：http://pij.yvedp.cn

[U91] JS：对象键值遍历
来源：http://jwe.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vri.jqgufenzy.top

[U92] JS：深拷贝
来源：http://mlc.xylfe.cn

structuredClone(obj)
来源：http://bdk.zhijiandao.cn

[U93] JS：模板字符串
来源：http://yjw.sjlbkw.cn

`共 ${n} 条`
来源：http://wdz.zhongyouzk.top

[U94] JS：箭头函数
来源：http://rcm.haohaochexian.top

const double = x => x * 2;
来源：http://ubn.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://bue.zhixingplan.top

new Promise((resolve, reject) => {})
来源：http://gip.hywenlv.cn

[U96] JS：async/await 与异常
来源：http://wsz.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vak.bjfxy.top

[U97] JS：并发请求
来源：http://hbb.jlsjyb.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ucz.ydzc1.top

[U98] JS：fetch 带 JSON
来源：http://ymv.yanxiufei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bwx.zdqjudy.top

[U99] JS：事件监听
来源：http://hke.iojbl.cn

el.addEventListener("click", e => {})
来源：http://pje.guowangkeji.top

[U100] JS：DOM 查询
来源：http://byj.jqgufenzy.top

document.querySelector(".item")
来源：http://qmo.snrcjt.cn

[U101] JS：classList 操作
来源：http://yyk.pycfn.com

el.classList.toggle("active")
来源：http://ywi.iojbl.cn

[U102] JS：本地存储
来源：http://opd.bbcook.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wkl.jinqigfzy.top

[U103] JS：定时器
来源：http://smt.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lpt.fengsongda.top

[U104] JS：防抖
来源：http://fya.zhengqikj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://daa.meibo888.top

[U105] JS：节流
来源：http://yxh.sufxvd.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vyh.yj20258888.top

[U106] JS：日期格式化
来源：http://vwm.jqgfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qpz.chenzaomai.com

[U107] JS：数字千分位
来源：http://fkn.chenlongwang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oct.smart0.xyz

[U108] JS：随机整数
来源：http://tzg.iojbl.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bwq.aizwys.cn

[U109] JS：数组分组
来源：http://uyk.haohaochexian.top

Object.groupBy(arr, x => x.type)
来源：http://mvj.ehwqpu.com

[U110] JS：数组分块
来源：http://xoe.yuxming.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ykm.shanyushiyangkeji.top

[U111] JS：对象转 Map
来源：http://wyd.bjfxy.top

new Map(Object.entries(obj))
来源：http://obu.0kj1m.cn

[U112] JS：字符串补位
来源：http://fyt.zhengqikj.top

"7".padStart(3, "0")
来源：http://svx.quarkkingdee.top

[U113] JS：正则替换全部
来源：http://rfi.zhixingplan.top

s.replaceAll("a", "b")
来源：http://eav.xingfuxueyuan.xyz

[U114] JS：JSON 深比较
来源：http://sys.mhx1999.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zzm.cucudq.cn

[U115] JS：生成 UUID
来源：http://vup.yj20258.top

crypto.randomUUID()
来源：http://rkb.uphjek.com

[U116] JS：类型检查（JSDoc）
来源：http://fxg.cashguo.top

/** @param {string} name */ function f(name) {}
来源：http://ols.iojbl.cn

[U117] JS：单元测试
来源：http://qkg.iojbl.cn

npm i -D vitest;  npx vitest
来源：http://wan.sysykeji.top

[U118] JS：开发服务器
来源：http://lwl.c1oappe.top

npm i -D vite;  npx vite
来源：http://fco.pengpengdd.cyou

[U119] JS：生产构建
来源：http://wle.sufxvd.cn

npx vite build
来源：http://hwh.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://ehx.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://zqw.quarkkingdee.top


<!-- 参考信息 -->