代发 wailian999

[T39] Lua：模式匹配
来源：http://fxf.iojbl.cn

string.find(s, "%d+")
来源：http://gtd.sufxvd.cn

[T40] Lua：元表
来源：http://yxg.gzhubu.top

setmetatable({}, { __index = base })
来源：http://hex.nwbrower.top

[T41] Perl：Hello World
来源：http://odx.yfazqb.com

print "Hello\n";
来源：http://rzt.chenzaomai.com

[T42] Perl：变量类型
来源：http://ysj.zdbjq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nmi.ybcxt.top

[T43] Perl：字符串插值
来源：http://xsx.snrcjt.cn

"值: $a"
来源：http://bqt.guowangkeji.top

[T44] Perl：条件
来源：http://jfd.quarkkingdee.top

if ($a > 0) { print "正"; }
来源：http://tft.fzhhl.top

[T45] Perl：数组遍历
来源：http://xil.yfazqb.com

for my $x (@arr) { print $x; }
来源：http://lou.zdbjq.cn

[T46] Perl：哈希操作
来源：http://pxf.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cms.c1oappe.top

[T47] Perl：正则捕获
来源：http://ozw.hywenlv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dur.sysykeji.top

[T48] Perl：正则替换
来源：http://gxu.haohaochexian.top

$s =~ s/old/new/g;
来源：http://vak.zhengqikj.top

[T49] Perl：函数
来源：http://fiq.zdqjudy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ctd.yangfankeji.com

[T50] Perl：逐行读文件
来源：http://tnd.uphjek.com

open my $fh, "<", "a.txt" or die $!;
来源：http://aqh.0kj1m.cn

while (my $line = <$fh>) { print $line; }
来源：http://jjq.fzhhl.top

[T51] Scala：Hello World
来源：http://etf.cucudq.cn

println("Hello")
来源：http://yni.yj202588.top

[T52] Scala：变量
来源：http://ksl.snrcjt.cn

val a = 1;  var b = 2
来源：http://xiw.yj20258888.top

[T53] Scala：字符串插值
来源：http://xak.sjlbkw.cn

s"值: $b"
来源：http://yrp.xingfuxueyuan.xyz

[T54] Scala：集合映射
来源：http://jux.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://nje.chenlongwang.top

[T55] Scala：集合过滤
来源：http://gqq.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ncx.dashuyun.cn

[T56] Scala：样例类
来源：http://hxh.havefunace.top

case class User(name: String, age: Int)
来源：http://lnh.hfpthk.cn

[T57] Scala：模式匹配
来源：http://nug.ywan-chungtsiang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qwx.yuanzhike.top

[T58] Scala：函数定义
来源：http://asj.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bfv.vehdjk.com

[T59] Scala：循环
来源：http://ybk.guannengcc.top

for (i <- 1 to 10) println(i)
来源：http://wlq.zhaomingkeji.xyz

[T60] Scala：折叠
来源：http://kpu.meibo888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ztn.smart0.xyz

================================================================================
来源：http://fyf.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mxk.zhiwuduotai.top

================================================================================
来源：http://qdc.smart0.xyz

[U01] Py：创建虚拟环境
来源：http://ivi.ctjpmb.com

python -m venv .venv && source .venv/bin/activate
来源：http://nve.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://wue.ctjpmb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zcf.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://yde.vehdjk.com

from dotenv import load_dotenv; load_dotenv()
来源：http://zvn.daxiang520.top

[U04] Py：变量调试打印
来源：http://dgs.wangdashe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fgc.yj202588.top

[U05] Py：列表去重且保序
来源：http://ihr.tian-w.cn

list(dict.fromkeys(arr))
来源：http://aix.shanyushiyangtech.top

[U06] Py：合并两个字典
来源：http://smi.yj20258888.top

{**a, **b}
来源：http://bhh.xziqi.cn

[U07] Py：反转字典键值
来源：http://ess.yvedp.cn

{v: k for k, v in d.items()}
来源：http://yye.epnwcf.com

[U08] Py：展平二维列表
来源：http://qgo.chenjidiqi.icu

[y for x in nested for y in x]
来源：http://pos.vehdjk.com

[U09] Py：字典取最大值的键
来源：http://rnl.redwolf501.top

max(d, key=d.get)
来源：http://fmx.wangshuangyany.cn

[U10] Py：按值排序字典
来源：http://iwy.hywenlv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nvv.dashuyun.cn

[U11] Py：生成器表达式
来源：http://qoc.tanke756.top

(x * 2 for x in arr)
来源：http://oti.sufxvd.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wgj.hysaishi.cn

Counter(arr).most_common(3)
来源：http://piy.xylfe.cn

[U13] Py：固定长度队列
来源：http://pbm.dashuyun.cn

deque(maxlen=10)
来源：http://ytg.sysykeji.top

[U14] Py：分组收集到列表
来源：http://yjq.tianlin.xyz

defaultdict(list)
来源：http://kmm.jyoumei.cn

[U15] Py：高精度计时
来源：http://etv.zdqjudy.top

t = time.perf_counter()
来源：http://vml.pycfn.com

[U16] Py：命令行参数解析
来源：http://qdn.shanyushiyangtech.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dxj.sweek.top

[U17] Py：初始化日志
来源：http://moe.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://mcr.nwbrower.top

[U18] Py：预编译正则
来源：http://avf.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://hbg.fehbvm.com

[U19] Py：正则替换带回调
来源：http://ouf.ehwqpu.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xtg.meibo888.top

[U20] Py：缓存函数结果
来源：http://ftz.xuetiantiany.cn

@functools.lru_cache(maxsize=None)
来源：http://cnd.jiagoushi.top

[U21] Py：自定义上下文管理器
来源：http://tmv.zhijiandao.cn

@contextlib.contextmanager
来源：http://mlo.shangyingyoupin.top

[U22] Py：矩阵转置
来源：http://npy.cheryme.top

list(zip(*m))
来源：http://auo.tanke756.top

[U23] Py：分块读取大文件
来源：http://woo.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ncy.sxryk.cn

[U24] Py：路径操作
来源：http://ivi.quarkkingdee.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ydw.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://hwu.aizwys.cn

csv.DictReader(f)
来源：http://fwi.wangdashe.top

[U26] Py：并发下载
来源：http://mro.yj202588.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hdj.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://yrq.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://gih.kuanghao11.cn

[U28] Py：类型别名
来源：http://zlp.yj202588.top

UserId = int
来源：http://sou.svipenyu.cn

[U29] Py：属性校验
来源：http://jmn.pycfn.com

@property 与 @x.setter 配合
来源：http://viu.jinqigfzy.top

[U30] Py：数据类
来源：http://izn.fehbvm.com

@dataclass(slots=True)
来源：http://bcu.xinyue.icu

[U31] Py：单测
来源：http://wps.yonumen.top

python -m pytest -q
来源：http://ouu.havefunace.top

[U32] Py：代码格式化
来源：http://srj.xuanzx.com

ruff format . && ruff check --fix .
来源：http://iyx.c1oappe.top

[U33] Py：打包发布
来源：http://uln.haohaochexian.top

python -m build  （依赖 pyproject.toml）
来源：http://huj.jqgufenzy.top

[U34] Py：判断编码
来源：http://mne.bjfxy.top

chardet.detect(raw)
来源：http://wxz.kuanghao11.cn

[U35] Py：发送邮件
来源：http://xch.zhixingplan.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://etx.ydzc1.top

[U36] Py：定时任务
来源：http://puq.tian-w.cn

schedule.every(10).minutes.do(job)
来源：http://bna.xylfe.cn

[U37] Py：读写 Excel
来源：http://xfq.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://cwm.ivvv.top

[U38] Py：获取脚本所在目录
来源：http://hha.hfpthk.cn

Path(__file__).resolve().parent
来源：http://vdt.jianghu66.top

[U39] Py：判断是否在交互环境
来源：http://qdp.yangfankeji.com

sys.stdout.isatty()
来源：http://xer.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://iqa.guowangkeji.top

print("err", file=sys.stderr)
来源：http://qsy.vehdjk.com

[U41] PHP：初始化 Composer 项目
来源：http://lqa.hcnkem.com

composer init;  composer require guzzlehttp/guzzle
来源：http://fad.pengpengdd.cyou

[U42] PHP：PSR-4 自动加载
来源：http://xxx.xinyue.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zmu.chenjidiqi.icu

[U43] PHP：声明命名空间
来源：http://bsv.hnxiangtu.top

namespace App\Http;
来源：http://kxf.dashuyun.cn

[U44] PHP：开启严格类型
来源：http://hfy.tarul.cn

declare(strict_types=1);
来源：http://dkp.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://eur.zdqjudy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vye.xylfe.cn

[U46] PHP：可空类型
来源：http://lmu.xinyue.icu

?string $name = null
来源：http://ads.ybcxt.top

[U47] PHP：联合类型
来源：http://iga.quarkkingdee.top

int|string $id
来源：http://cdw.mhx1999.top

[U48] PHP：纯枚举
来源：http://wya.nanxinkj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yih.guowangkeji.top

[U49] PHP：只读属性
来源：http://trh.zhengqikj.top

public readonly string $name
来源：http://apm.wangshuangyany.cn

[U50] PHP：构造器属性提升
来源：http://njv.yongpay.top

public function __construct(private int $id) {}
来源：http://ezn.tarul.cn

[U51] PHP：数组解构
来源：http://zgs.mhx1999.top

[$a, $b] = $arr;
来源：http://rdg.tian-w.cn

[U52] PHP：箭头函数
来源：http://vtn.316326.xyz

$double = fn($x) => $x * 2;
来源：http://mlq.fanxiaobao.xyz

[U53] PHP：空合并运算符
来源：http://dzz.jqgfzy.top

$v = $a ?? $b ?? "default";
来源：http://vdl.ctjpmb.com

[U54] PHP：空安全调用
来源：http://wol.gogol.net.cn

$obj?->method()
来源：http://rzo.nanxuanxn.top

[U55] PHP：match 表达式
来源：http://gws.snrcjt.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://toi.bbcook.cn

[U56] PHP：命名参数
来源：http://oqu.zhixingplan.top

f(a: 1, b: 2)
来源：http://mwg.wangshuangyany.cn

[U57] PHP：字符串插值
来源：http://kgo.fehbvm.com

"值: {$a}"
来源：http://ejc.xuanzx.com

[U58] PHP：数组三件套
来源：http://wuw.hysaishi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wdz.shuidangran.top

[U59] PHP：自定义排序
来源：http://rfq.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hba.ivvv.top

[U60] PHP：JSON 编解码
来源：http://ibx.tianlin.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bue.iojbl.cn

[U61] PHP：正则
来源：http://eww.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cof.fehbvm.com

[U62] PHP：日期对象
来源：http://xpv.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ruc.zhoulong.xyz

[U63] PHP：文件读写
来源：http://yvc.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rft.tanke756.top

[U64] PHP：目录遍历
来源：http://tsf.daxiang520.top

glob("dir/*.php");  scandir("dir");
来源：http://hbb.sxryk.cn

[U65] PHP：会话
来源：http://dbv.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wkk.hywenlv.cn

[U66] PHP：设置 Cookie
来源：http://xil.hywenlv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dbs.yj20258.top

[U67] PHP：处理文件上传
来源：http://ytk.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://feb.jinqigufen.top

[U68] PHP：PDO 连接
来源：http://jay.hcnkem.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pxp.ywan-chungtsiang.top

[U69] PHP：PDO 预处理
来源：http://gpm.tian-w.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://edl.feifeiyinyue.top

[U70] PHP：PDO 事务
来源：http://nep.9152youxi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rbs.cdnleiting.top

[U71] PHP：抛出异常
来源：http://iwd.fehbvm.com

throw new RuntimeException("失败", 500);
来源：http://zek.wangshuangyany.cn

[U72] PHP：写错误日志
来源：http://zcv.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://fkb.yanxiufei.cn

[U73] PHP：读取 ini 配置
来源：http://xmv.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://pcg.iojbl.cn

[U74] PHP：读取环境变量
来源：http://ixu.zhoulong.xyz

getenv("APP_ENV") ?: "production"
来源：http://eup.jiagoushi.top

[U75] PHP：依赖注入
来源：http://yuo.hysaishi.cn

composer require psr/container
来源：http://cnd.ivvv.top

[U76] PHP：简单路由
来源：http://qct.redwolf501.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://onh.xziqi.cn

[U77] PHP：模板渲染
来源：http://qeb.gogol.net.cn

composer require twig/twig
来源：http://tvj.jianghu66.top

[U78] PHP：单元测试
来源：http://ucc.fengsongda.top

composer require --dev phpunit/phpunit
来源：http://rmb.fzhhl.top

[U79] PHP：静态分析
来源：http://coc.ydjk.org.cn

composer require --dev phpstan/phpstan
来源：http://rpt.hnxiangtu.top

[U80] PHP：代码规范修复
来源：http://vux.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://qyk.xuetiantiany.cn

[U81] JS：初始化项目
来源：http://eql.hnqzz.top

npm init -y;  npm i express
来源：http://avv.sxryk.cn

[U82] JS：package.json 脚本
来源：http://bkd.chenjidiqi.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wfp.fehbvm.com

[U83] JS：ES Module 导入导出
来源：http://znm.jyoumei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://svg.epnwcf.com

[U84] JS：CommonJS 写法
来源：http://qmu.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://txm.dianchejie.cn

[U85] JS：可选链
来源：http://ehf.shzxlz.cn

a?.b?.c
来源：http://adg.shzxlz.cn

[U86] JS：空值合并
来源：http://pap.sufxvd.cn

a ?? b
来源：http://eey.sjlbkw.cn

[U87] JS：解构默认值
来源：http://ebt.snrcjt.cn

const { a = 1, b = 2 } = obj;
来源：http://mro.shzxlz.cn

[U88] JS：对象展开合并
来源：http://vkz.fehbvm.com

{ ...a, ...b }
来源：http://tgn.xylfe.cn

[U89] JS：数组去重
来源：http://fgn.yfazqb.com

[...new Set(arr)]
来源：http://zqq.cdnleiting.top

[U90] JS：数字数组排序
来源：http://ypt.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://pew.daxiang520.top

[U91] JS：对象键值遍历
来源：http://ylc.cucudq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://orv.svipenyu.cn

[U92] JS：深拷贝
来源：http://zld.hnqzz.top

structuredClone(obj)
来源：http://fun.xingfuxueyuan.xyz

[U93] JS：模板字符串
来源：http://cpl.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://gzh.gzhubu.top

[U94] JS：箭头函数
来源：http://gkc.tianlin.xyz

const double = x => x * 2;
来源：http://fie.uphjek.com

[U95] JS：Promise 包装
来源：http://zhi.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://wbf.tian-w.cn

[U96] JS：async/await 与异常
来源：http://noi.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ghj.jyoumei.cn

[U97] JS：并发请求
来源：http://bhy.nanxuanxn.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vzs.fktsv.cn

[U98] JS：fetch 带 JSON
来源：http://fjj.havefunace.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zlo.svipenyu.cn

[U99] JS：事件监听
来源：http://jfq.jinqigufen.top

el.addEventListener("click", e => {})
来源：http://zlt.hesvh.cn

[U100] JS：DOM 查询
来源：http://wfw.jinghuilouyu.cn

document.querySelector(".item")
来源：http://tnt.hcnkem.com

[U101] JS：classList 操作
来源：http://mha.ydzc1.top

el.classList.toggle("active")
来源：http://suv.zhoulong.xyz

[U102] JS：本地存储
来源：http://pxk.yangfankeji.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://wqy.shanyushiyangkeji.top

[U103] JS：定时器
来源：http://wer.nanxuanxn.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ura.shanyushiyangtech.top

[U104] JS：防抖
来源：http://mmo.bjfxy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dsi.xziqi.cn

[U105] JS：节流
来源：http://ulq.zdbjq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cgt.smart0.xyz

[U106] JS：日期格式化
来源：http://ijm.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wep.zhaomingkeji.xyz

[U107] JS：数字千分位
来源：http://iyw.fzhhl.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xjh.havefunace.top

[U108] JS：随机整数
来源：http://duo.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rux.ehwqpu.com

[U109] JS：数组分组
来源：http://amq.jinqigfzy.top

Object.groupBy(arr, x => x.type)
来源：http://ata.zhijiandao.cn

[U110] JS：数组分块
来源：http://xvp.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://liy.fanxiaobao.xyz

[U111] JS：对象转 Map
来源：http://eao.hcnkem.com

new Map(Object.entries(obj))
来源：http://tbz.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://kuh.fktsv.cn

"7".padStart(3, "0")
来源：http://hei.zhixingplan.top

[U113] JS：正则替换全部
来源：http://wwh.cdnleiting.top

s.replaceAll("a", "b")
来源：http://kyv.wangshuangyany.cn

[U114] JS：JSON 深比较
来源：http://zyd.guannengcc.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hcr.bjfxy.top

[U115] JS：生成 UUID
来源：http://zbq.gaohongyu789.top

crypto.randomUUID()
来源：http://rlq.ydzc1.top

[U116] JS：类型检查（JSDoc）
来源：http://yxv.jinyuanbaomall.cn

/** @param {string} name */ function f(name) {}
来源：http://irg.shzxlz.cn

[U117] JS：单元测试
来源：http://gek.xylfe.cn

npm i -D vitest;  npx vitest
来源：http://qfm.cashguo.top

[U118] JS：开发服务器
来源：http://yld.vehdjk.com

npm i -D vite;  npx vite
来源：http://taz.yj20258.top

[U119] JS：生产构建
来源：http://rto.svipenyu.cn

npx vite build
来源：http://thc.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://thv.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://erd.fanxiaobao.xyz

================================================================================
来源：http://tzf.daria6918.cn

统计汇总
来源：http://jxg.jlsjyb.cn

================================================================================
来源：http://edh.9152youxi.cn

按语言统计（条）：
来源：http://ntu.iojbl.cn

Python ......... 252
来源：http://wio.jlsjyb.cn

PHP ............ 252
来源：http://sgq.birdmap.top

JavaScript ..... 252
来源：http://jwx.dashuyun.cn

TypeScript ..... 212
来源：http://jqq.yvedp.cn

Java ........... 212
来源：http://kws.andypj.xyz

Go ............. 212
来源：http://eiy.quarkkingdee.top

Ruby ........... 212
来源：http://ouo.daria6918.cn

C# ............. 212
来源：http://xkj.quarkkingdee.top


<!-- 参考信息 -->