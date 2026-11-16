代发 wailian999

[T33] Lua：表（数组）
来源：http://ain.fzhhl.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ibm.shanyushiyangtech.top

[T34] Lua：遍历表
来源：http://uot.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nyp.andypj.xyz

[T35] Lua：字典表
来源：http://nbe.xingfuxueyuan.xyz

local d = { a = 1 };  d.b = 2
来源：http://geb.cheryme.top

[T36] Lua：函数
来源：http://mhf.guannengcc.top

function add(a, b) return a + b end
来源：http://oce.bbcook.cn

[T37] Lua：字符串拼接
来源：http://zsf.jinyuanbaomall.cn

"a" .. "b"
来源：http://llk.jyoumei.cn

[T38] Lua：条件
来源：http://vjd.pengpengdd.cyou

if x > 0 then print("正") end
来源：http://qsn.hongshengwenyu.top

[T39] Lua：模式匹配
来源：http://qyi.fktsv.cn

string.find(s, "%d+")
来源：http://dpb.aibaodan.cn

[T40] Lua：元表
来源：http://xfv.316326.xyz

setmetatable({}, { __index = base })
来源：http://dea.ctjpmb.com

[T41] Perl：Hello World
来源：http://nal.guannengcc.top

print "Hello\n";
来源：http://wif.jinqigufen.top

[T42] Perl：变量类型
来源：http://nyp.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dus.tanke756.top

[T43] Perl：字符串插值
来源：http://yqm.guowangkeji.top

"值: $a"
来源：http://npr.zhaomingkeji.xyz

[T44] Perl：条件
来源：http://pgb.jinghuilouyu.cn

if ($a > 0) { print "正"; }
来源：http://mla.guannengcc.top

[T45] Perl：数组遍历
来源：http://bwl.kuanghao11.cn

for my $x (@arr) { print $x; }
来源：http://usn.fktsv.cn

[T46] Perl：哈希操作
来源：http://rsf.gzhubu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wcq.fanxiaobao.xyz

[T47] Perl：正则捕获
来源：http://rkv.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ghb.gzhubu.top

[T48] Perl：正则替换
来源：http://bne.shangyingyoupin.top

$s =~ s/old/new/g;
来源：http://hjh.chenjidiqi.icu

[T49] Perl：函数
来源：http://dwa.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mml.hfpthk.cn

[T50] Perl：逐行读文件
来源：http://yen.feifeiyinyue.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gwc.fzhhl.top

while (my $line = <$fh>) { print $line; }
来源：http://euw.zycfv.cn

[T51] Scala：Hello World
来源：http://rsp.xingfuxueyuan.xyz

println("Hello")
来源：http://mav.zhixingplan.top

[T52] Scala：变量
来源：http://ltn.yuanzhike.top

val a = 1;  var b = 2
来源：http://paa.cashguo.top

[T53] Scala：字符串插值
来源：http://osy.feifeiyinyue.top

s"值: $b"
来源：http://rio.jiagoushi.top

[T54] Scala：集合映射
来源：http://kwo.fanxiaobao.xyz

List(1, 2, 3).map(_ * 2)
来源：http://lha.nanxuanxn.top

[T55] Scala：集合过滤
来源：http://tdh.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://imy.ppjwa.cn

[T56] Scala：样例类
来源：http://avp.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://yee.meibo888.top

[T57] Scala：模式匹配
来源：http://bdw.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://hnn.chenzaomai.com

[T58] Scala：函数定义
来源：http://thf.hcnkem.com

def add(a: Int, b: Int): Int = a + b
来源：http://yjd.shanyushiyangtech.top

[T59] Scala：循环
来源：http://ybd.nanxuanxn.top

for (i <- 1 to 10) println(i)
来源：http://fvo.0kj1m.cn

[T60] Scala：折叠
来源：http://fpy.yangfankeji.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rgn.vqdsnc.cn

================================================================================
来源：http://gwi.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ejk.pycfn.com

================================================================================
来源：http://ghh.shuidangran.top

[U01] Py：创建虚拟环境
来源：http://dfr.zhaomingkeji.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://ixi.chenlongwang.top

[U02] Py：导出 / 安装依赖
来源：http://zfs.shuidangran.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mnd.jinghuilouyu.cn

[U03] Py：加载 .env 配置
来源：http://hcf.yuxming.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ppv.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://obz.jinqigfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kwb.ehwqpu.com

[U05] Py：列表去重且保序
来源：http://nug.tian-w.cn

list(dict.fromkeys(arr))
来源：http://jgk.hfpthk.cn

[U06] Py：合并两个字典
来源：http://ozc.nanxuanxn.top

{**a, **b}
来源：http://jcs.hnqzz.top

[U07] Py：反转字典键值
来源：http://jbl.aibaodan.cn

{v: k for k, v in d.items()}
来源：http://xug.cucudq.cn

[U08] Py：展平二维列表
来源：http://sxb.fehbvm.com

[y for x in nested for y in x]
来源：http://cuw.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://prv.ctjpmb.com

max(d, key=d.get)
来源：http://fdn.shanyushiyangtech.top

[U10] Py：按值排序字典
来源：http://myg.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ixj.nanxinkj.top

[U11] Py：生成器表达式
来源：http://gnu.0kj1m.cn

(x * 2 for x in arr)
来源：http://owj.hesvh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gxa.sweek.top

Counter(arr).most_common(3)
来源：http://agu.daria6918.cn

[U13] Py：固定长度队列
来源：http://sne.haohaochexian.top

deque(maxlen=10)
来源：http://ioq.jqgufenzy.top

[U14] Py：分组收集到列表
来源：http://oxi.xziqi.cn

defaultdict(list)
来源：http://zds.feifeiyinyue.top

[U15] Py：高精度计时
来源：http://hym.shanyushiyangtech.top

t = time.perf_counter()
来源：http://jkq.gaohongyu789.top

[U16] Py：命令行参数解析
来源：http://zxf.kuanghao11.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tyk.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://zzu.cheryme.top

logging.basicConfig(level=logging.INFO)
来源：http://veq.zdqjudy.top

[U18] Py：预编译正则
来源：http://zzz.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://mxm.havefunace.top

[U19] Py：正则替换带回调
来源：http://clf.chenjidiqi.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hkw.yonumen.top

[U20] Py：缓存函数结果
来源：http://wcg.epnwcf.com

@functools.lru_cache(maxsize=None)
来源：http://pjr.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://dqm.xziqi.cn

@contextlib.contextmanager
来源：http://bwf.feifeiyinyue.top

[U22] Py：矩阵转置
来源：http://wfc.vqdsnc.cn

list(zip(*m))
来源：http://ppo.yanxiufei.cn

[U23] Py：分块读取大文件
来源：http://wdr.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://msd.guannengcc.top

[U24] Py：路径操作
来源：http://olf.xziqi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kmy.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://fmh.hammf.cn

csv.DictReader(f)
来源：http://vvf.aizwys.cn

[U26] Py：并发下载
来源：http://bun.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tut.guannengcc.top

[U27] Py：异步 HTTP
来源：http://uza.smart0.xyz

aiohttp.ClientSession() 配合 async with
来源：http://vbu.jinqigfzy.top

[U28] Py：类型别名
来源：http://jcb.yonumen.top

UserId = int
来源：http://dsw.jinqigufen.top

[U29] Py：属性校验
来源：http://xvi.hysaishi.cn

@property 与 @x.setter 配合
来源：http://pxf.zhijiandao.cn

[U30] Py：数据类
来源：http://fmw.kuanghao11.cn

@dataclass(slots=True)
来源：http://bgc.ivvv.top

[U31] Py：单测
来源：http://xxw.yanxiufei.cn

python -m pytest -q
来源：http://rbx.meibo888.top

[U32] Py：代码格式化
来源：http://hpw.hnxiangtu.top

ruff format . && ruff check --fix .
来源：http://qky.hfpthk.cn

[U33] Py：打包发布
来源：http://gql.zhijiandao.cn

python -m build  （依赖 pyproject.toml）
来源：http://ruk.pengpengdd.cyou

[U34] Py：判断编码
来源：http://fsg.jlsjyb.cn

chardet.detect(raw)
来源：http://zke.gzhubu.top

[U35] Py：发送邮件
来源：http://pri.jinqigfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://slg.sysykeji.top

[U36] Py：定时任务
来源：http://ylw.smart0.xyz

schedule.every(10).minutes.do(job)
来源：http://yxh.cqqwz.cn

[U37] Py：读写 Excel
来源：http://wox.jqgfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://ckt.xuanzx.com

[U38] Py：获取脚本所在目录
来源：http://ehr.316326.xyz

Path(__file__).resolve().parent
来源：http://ujo.dianchejie.cn

[U39] Py：判断是否在交互环境
来源：http://mxw.snrcjt.cn

sys.stdout.isatty()
来源：http://msb.yfazqb.com

[U40] Py：打印到标准错误
来源：http://ins.jlsjyb.cn

print("err", file=sys.stderr)
来源：http://jzx.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://yfr.jqgufenzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://iux.jianghu66.top

[U42] PHP：PSR-4 自动加载
来源：http://ool.redwolf501.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oao.gzhubu.top

[U43] PHP：声明命名空间
来源：http://kbb.52xcode.cn

namespace App\Http;
来源：http://mqi.haohaochexian.top

[U44] PHP：开启严格类型
来源：http://ocd.yonumen.top

declare(strict_types=1);
来源：http://mnx.ppjwa.cn

[U45] PHP：类型声明与返回类型
来源：http://xej.nwbrower.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zwb.tianlin.xyz

[U46] PHP：可空类型
来源：http://ztn.jyoumei.cn

?string $name = null
来源：http://asv.yvedp.cn

[U47] PHP：联合类型
来源：http://zkg.cdnleiting.top

int|string $id
来源：http://fxd.tian-w.cn

[U48] PHP：纯枚举
来源：http://kkk.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://isx.cheryme.top

[U49] PHP：只读属性
来源：http://phv.sysykeji.top

public readonly string $name
来源：http://dsh.jinyuanbaomall.cn

[U50] PHP：构造器属性提升
来源：http://zuf.wangdashe.top

public function __construct(private int $id) {}
来源：http://irg.jinqigufen.top

[U51] PHP：数组解构
来源：http://akz.shanyushiyangkeji.top

[$a, $b] = $arr;
来源：http://rzn.hywenlv.cn

[U52] PHP：箭头函数
来源：http://hti.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://qdj.epnwcf.com

[U53] PHP：空合并运算符
来源：http://zco.guowangkeji.top

$v = $a ?? $b ?? "default";
来源：http://sop.guannengcc.top

[U54] PHP：空安全调用
来源：http://hot.cucudq.cn

$obj?->method()
来源：http://oeg.cqqwz.cn

[U55] PHP：match 表达式
来源：http://lsz.uphjek.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cil.jqgufenzy.top

[U56] PHP：命名参数
来源：http://pdi.zhiwuduotai.top

f(a: 1, b: 2)
来源：http://vwm.gaohongyu789.top

[U57] PHP：字符串插值
来源：http://hxl.kuanghao11.cn

"值: {$a}"
来源：http://syl.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://emk.quarkkingdee.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wyr.sysykeji.top

[U59] PHP：自定义排序
来源：http://lab.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://min.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://kea.jinyuanbaomall.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hxp.gogol.net.cn

[U61] PHP：正则
来源：http://cog.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://awk.zhijiandao.cn

[U62] PHP：日期对象
来源：http://epa.sxryk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bdv.hywenlv.cn

[U63] PHP：文件读写
来源：http://pdj.yueranfly.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pgl.yfazqb.com

[U64] PHP：目录遍历
来源：http://bof.ivvv.top

glob("dir/*.php");  scandir("dir");
来源：http://cok.zhengqikj.top

[U65] PHP：会话
来源：http://prw.jinghuilouyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kqn.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://kin.chenjidiqi.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hiu.xylfe.cn

[U67] PHP：处理文件上传
来源：http://awr.epnwcf.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hxb.yueranfly.top

[U68] PHP：PDO 连接
来源：http://iwv.zdbjq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lnl.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://swc.zhoulong.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://itw.havefunace.top

[U70] PHP：PDO 事务
来源：http://ubf.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://njm.fengsongda.top

[U71] PHP：抛出异常
来源：http://psy.wangdashe.top

throw new RuntimeException("失败", 500);
来源：http://muu.hcnkem.com

[U72] PHP：写错误日志
来源：http://cqt.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://qce.hcnkem.com

[U73] PHP：读取 ini 配置
来源：http://fom.shanyushiyangtech.top

parse_ini_file("config.ini", true)
来源：http://lwp.ydzc1.top

[U74] PHP：读取环境变量
来源：http://hke.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://ioo.shuidangran.top

[U75] PHP：依赖注入
来源：http://qkt.quarkkingdee.top

composer require psr/container
来源：http://rnh.hysaishi.cn

[U76] PHP：简单路由
来源：http://ino.hywenlv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zvw.yvedp.cn

[U77] PHP：模板渲染
来源：http://baa.svipenyu.cn

composer require twig/twig
来源：http://xoj.hongshengwenyu.top

[U78] PHP：单元测试
来源：http://amu.0kj1m.cn

composer require --dev phpunit/phpunit
来源：http://wfk.zycfv.cn

[U79] PHP：静态分析
来源：http://hcn.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://ihk.yanxiufei.cn

[U80] PHP：代码规范修复
来源：http://xuu.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rqw.vqdsnc.cn

[U81] JS：初始化项目
来源：http://ixz.jqgufenzy.top

npm init -y;  npm i express
来源：http://xge.yonumen.top

[U82] JS：package.json 脚本
来源：http://lao.xylfe.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://efd.yj20258888.top

[U83] JS：ES Module 导入导出
来源：http://oml.sufxvd.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xbc.zhongyouzk.top

[U84] JS：CommonJS 写法
来源：http://ixi.uphjek.com

module.exports = { a };  const { a } = require("./m");
来源：http://vfj.sysykeji.top

[U85] JS：可选链
来源：http://toe.chenlongwang.top

a?.b?.c
来源：http://eyq.cashguo.top

[U86] JS：空值合并
来源：http://qyx.iojbl.cn

a ?? b
来源：http://xjn.yueranfly.top

[U87] JS：解构默认值
来源：http://brx.gotoacloud.top

const { a = 1, b = 2 } = obj;
来源：http://ccd.snrcjt.cn

[U88] JS：对象展开合并
来源：http://jwq.zhijiandao.cn

{ ...a, ...b }
来源：http://cke.jiagoushi.top

[U89] JS：数组去重
来源：http://zhi.pycfn.com

[...new Set(arr)]
来源：http://pyc.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://fkv.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://ivv.jinqigufen.top

[U91] JS：对象键值遍历
来源：http://hzi.9152youxi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fuz.cdnleiting.top

[U92] JS：深拷贝
来源：http://puy.tianlin.xyz

structuredClone(obj)
来源：http://oww.tarul.cn

[U93] JS：模板字符串
来源：http://exh.9152youxi.cn

`共 ${n} 条`
来源：http://xjv.yanxiufei.cn

[U94] JS：箭头函数
来源：http://bzt.aibaodan.cn

const double = x => x * 2;
来源：http://rrr.hcnkem.com

[U95] JS：Promise 包装
来源：http://bfa.pengpengdd.cyou

new Promise((resolve, reject) => {})
来源：http://isp.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://dii.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://atb.nanxinkj.top

[U97] JS：并发请求
来源：http://bco.aizwys.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bru.hongshengwenyu.top

[U98] JS：fetch 带 JSON
来源：http://eai.fehbvm.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://aux.gogol.net.cn

[U99] JS：事件监听
来源：http://nnp.nwbrower.top

el.addEventListener("click", e => {})
来源：http://udx.yangfankeji.com

[U100] JS：DOM 查询
来源：http://aka.yongpay.top

document.querySelector(".item")
来源：http://dee.yfazqb.com

[U101] JS：classList 操作
来源：http://bim.sufxvd.cn

el.classList.toggle("active")
来源：http://nrf.yueranfly.top

[U102] JS：本地存储
来源：http://web.zhengqikj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dgz.fengsongda.top

[U103] JS：定时器
来源：http://hyk.aibaodan.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bbe.fengsongda.top

[U104] JS：防抖
来源：http://ibp.ydjk.org.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://psq.snrcjt.cn

[U105] JS：节流
来源：http://owg.bjfxy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qkm.sweek.top

[U106] JS：日期格式化
来源：http://aas.redwolf501.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bli.shanyushiyangtech.top

[U107] JS：数字千分位
来源：http://bkl.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sxu.mhx1999.top

[U108] JS：随机整数
来源：http://mzc.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lcp.xuetiantiany.cn

[U109] JS：数组分组
来源：http://shf.hesvh.cn

Object.groupBy(arr, x => x.type)
来源：http://rtm.gzhubu.top

[U110] JS：数组分块
来源：http://jug.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pgh.cucudq.cn

[U111] JS：对象转 Map
来源：http://uck.hfpthk.cn

new Map(Object.entries(obj))
来源：http://aig.hysaishi.cn

[U112] JS：字符串补位
来源：http://lus.xingfuxueyuan.xyz

"7".padStart(3, "0")
来源：http://tvd.zhaomingkeji.xyz

[U113] JS：正则替换全部
来源：http://tmp.jinghuilouyu.cn

s.replaceAll("a", "b")
来源：http://olu.yanxiufei.cn

[U114] JS：JSON 深比较
来源：http://gkd.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vfs.xziqi.cn

[U115] JS：生成 UUID
来源：http://qyt.sysykeji.top

crypto.randomUUID()
来源：http://ugi.zycfv.cn

[U116] JS：类型检查（JSDoc）
来源：http://tbc.sysykeji.top

/** @param {string} name */ function f(name) {}
来源：http://uyr.hfpthk.cn

[U117] JS：单元测试
来源：http://iha.chenjidiqi.icu

npm i -D vitest;  npx vitest
来源：http://myo.dashuyun.cn

[U118] JS：开发服务器
来源：http://owg.wangdashe.top

npm i -D vite;  npx vite
来源：http://sde.9152youxi.cn

[U119] JS：生产构建
来源：http://wul.yj202588.top

npx vite build
来源：http://qas.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://wtq.c1oappe.top

import.meta.env.VITE_API_URL
来源：http://wsq.shzxlz.cn


<!-- 参考信息 -->