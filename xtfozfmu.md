代发 wailian999

[T35] Lua：字典表
来源：http://wmn.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://bwf.bjfxy.top

[T36] Lua：函数
来源：http://nvh.guowangkeji.top

function add(a, b) return a + b end
来源：http://ovl.yuanzhike.top

[T37] Lua：字符串拼接
来源：http://sas.svipenyu.cn

"a" .. "b"
来源：http://wna.jianghu66.top

[T38] Lua：条件
来源：http://vlb.yfazqb.com

if x > 0 then print("正") end
来源：http://dmf.gotoacloud.top

[T39] Lua：模式匹配
来源：http://cmr.ybcxt.top

string.find(s, "%d+")
来源：http://xjy.xuanzx.com

[T40] Lua：元表
来源：http://ukb.aizwys.cn

setmetatable({}, { __index = base })
来源：http://tox.daria6918.cn

[T41] Perl：Hello World
来源：http://rbi.gotoacloud.top

print "Hello\n";
来源：http://zau.gotoacloud.top

[T42] Perl：变量类型
来源：http://vcp.andypj.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ood.daxiang520.top

[T43] Perl：字符串插值
来源：http://uuk.quarkkingdee.top

"值: $a"
来源：http://qxy.jyoumei.cn

[T44] Perl：条件
来源：http://wrn.xuetiantiany.cn

if ($a > 0) { print "正"; }
来源：http://ura.jinyuanbaomall.cn

[T45] Perl：数组遍历
来源：http://dpi.nwbrower.top

for my $x (@arr) { print $x; }
来源：http://ngv.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://oux.xingfuxueyuan.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gfs.ehwqpu.com

[T47] Perl：正则捕获
来源：http://dzb.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://wqf.zhixingplan.top

[T48] Perl：正则替换
来源：http://djz.ybcxt.top

$s =~ s/old/new/g;
来源：http://qan.zdqjudy.top

[T49] Perl：函数
来源：http://lqz.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ihj.zycfv.cn

[T50] Perl：逐行读文件
来源：http://vxs.svipenyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kix.jqgfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://xoc.kuanghao11.cn

[T51] Scala：Hello World
来源：http://xfz.dashuyun.cn

println("Hello")
来源：http://jbo.guowangkeji.top

[T52] Scala：变量
来源：http://ypw.ybcxt.top

val a = 1;  var b = 2
来源：http://yog.zhoulong.xyz

[T53] Scala：字符串插值
来源：http://mvz.yj20258.top

s"值: $b"
来源：http://mcb.316326.xyz

[T54] Scala：集合映射
来源：http://zxr.uphjek.com

List(1, 2, 3).map(_ * 2)
来源：http://txx.hfpthk.cn

[T55] Scala：集合过滤
来源：http://ixf.yanxiufei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ohv.fengsongda.top

[T56] Scala：样例类
来源：http://uaa.jiagoushi.top

case class User(name: String, age: Int)
来源：http://svk.daxiang520.top

[T57] Scala：模式匹配
来源：http://wtg.feifeiyinyue.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wig.fzhhl.top

[T58] Scala：函数定义
来源：http://knb.ydzc1.top

def add(a: Int, b: Int): Int = a + b
来源：http://cdd.sweek.top

[T59] Scala：循环
来源：http://xcv.yfazqb.com

for (i <- 1 to 10) println(i)
来源：http://uqi.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://llu.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hvt.sysykeji.top

================================================================================
来源：http://voh.wangdashe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://amj.zhiwuduotai.top

================================================================================
来源：http://hyw.ctjpmb.com

[U01] Py：创建虚拟环境
来源：http://red.zhiwuduotai.top

python -m venv .venv && source .venv/bin/activate
来源：http://arl.uphjek.com

[U02] Py：导出 / 安装依赖
来源：http://ghx.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mjb.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://iab.c1oappe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gcn.yongpay.top

[U04] Py：变量调试打印
来源：http://dhf.tian-w.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gnm.xinyue.icu

[U05] Py：列表去重且保序
来源：http://xlt.sjlbkw.cn

list(dict.fromkeys(arr))
来源：http://isz.jqgfzy.top

[U06] Py：合并两个字典
来源：http://hwu.chenjidiqi.icu

{**a, **b}
来源：http://lzg.chenzaomai.com

[U07] Py：反转字典键值
来源：http://hoi.ivvv.top

{v: k for k, v in d.items()}
来源：http://mdc.zdbjq.cn

[U08] Py：展平二维列表
来源：http://kfv.wangshuangyany.cn

[y for x in nested for y in x]
来源：http://dzu.ydjk.org.cn

[U09] Py：字典取最大值的键
来源：http://pxd.yj20258888.top

max(d, key=d.get)
来源：http://sff.dianchejie.cn

[U10] Py：按值排序字典
来源：http://stc.guannengcc.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cll.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://ooc.ehwqpu.com

(x * 2 for x in arr)
来源：http://gfy.shanyushiyangtech.top

[U12] Py：取出现最多的 3 个元素
来源：http://myb.yfazqb.com

Counter(arr).most_common(3)
来源：http://qba.svipenyu.cn

[U13] Py：固定长度队列
来源：http://qzg.ydzc1.top

deque(maxlen=10)
来源：http://uwo.yueranfly.top

[U14] Py：分组收集到列表
来源：http://qrn.redwolf501.top

defaultdict(list)
来源：http://yzz.shangyingyoupin.top

[U15] Py：高精度计时
来源：http://ioj.cheryme.top

t = time.perf_counter()
来源：http://gzd.andypj.xyz

[U16] Py：命令行参数解析
来源：http://icx.yanxiufei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tli.iojbl.cn

[U17] Py：初始化日志
来源：http://sij.daxiang520.top

logging.basicConfig(level=logging.INFO)
来源：http://ule.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://dhu.ybcxt.top

pat = re.compile(r"\d+")
来源：http://ugs.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://bga.jqgufenzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vyb.mhx1999.top

[U20] Py：缓存函数结果
来源：http://kpl.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://cnh.sxryk.cn

[U21] Py：自定义上下文管理器
来源：http://bhr.zhongyouzk.top

@contextlib.contextmanager
来源：http://dnk.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://qqb.meibo888.top

list(zip(*m))
来源：http://xrj.yueranfly.top

[U23] Py：分块读取大文件
来源：http://oov.tianlin.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ygb.316326.xyz

[U24] Py：路径操作
来源：http://pua.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bvb.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://dgf.cheryme.top

csv.DictReader(f)
来源：http://xxm.chenlongwang.top

[U26] Py：并发下载
来源：http://xcm.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://clw.zhijiandao.cn

[U27] Py：异步 HTTP
来源：http://ywl.nanxinkj.top

aiohttp.ClientSession() 配合 async with
来源：http://anq.hfpthk.cn

[U28] Py：类型别名
来源：http://xry.cqqwz.cn

UserId = int
来源：http://nfa.meibo888.top

[U29] Py：属性校验
来源：http://dvv.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://pgl.jinghuilouyu.cn

[U30] Py：数据类
来源：http://lke.pengpengdd.cyou

@dataclass(slots=True)
来源：http://dww.zhixingplan.top

[U31] Py：单测
来源：http://rde.ydjk.org.cn

python -m pytest -q
来源：http://vnr.mhx1999.top

[U32] Py：代码格式化
来源：http://ake.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://lxi.fengsongda.top

[U33] Py：打包发布
来源：http://vnp.shanyushiyangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://tro.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://xhd.yj202588.top

chardet.detect(raw)
来源：http://zyg.gzhubu.top

[U35] Py：发送邮件
来源：http://cth.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qaf.0kj1m.cn

[U36] Py：定时任务
来源：http://smt.aizwys.cn

schedule.every(10).minutes.do(job)
来源：http://wla.yangfankeji.com

[U37] Py：读写 Excel
来源：http://fgr.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rbm.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://sjz.havefunace.top

Path(__file__).resolve().parent
来源：http://ofm.chenjidiqi.icu

[U39] Py：判断是否在交互环境
来源：http://cgr.zdqjudy.top

sys.stdout.isatty()
来源：http://zmw.uphjek.com

[U40] Py：打印到标准错误
来源：http://ads.chenzaomai.com

print("err", file=sys.stderr)
来源：http://vgt.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://fne.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fhs.cheryme.top

[U42] PHP：PSR-4 自动加载
来源：http://tuu.52xcode.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xwo.hammf.cn

[U43] PHP：声明命名空间
来源：http://tds.yuanzhike.top

namespace App\Http;
来源：http://kuo.fanxiaobao.xyz

[U44] PHP：开启严格类型
来源：http://zpa.quarkkingdee.top

declare(strict_types=1);
来源：http://pps.xuanzx.com

[U45] PHP：类型声明与返回类型
来源：http://rjm.yj20258.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qqi.hywenlv.cn

[U46] PHP：可空类型
来源：http://xqk.xuanzx.com

?string $name = null
来源：http://qms.dashuyun.cn

[U47] PHP：联合类型
来源：http://vdt.jiagoushi.top

int|string $id
来源：http://tdz.jinqigufen.top

[U48] PHP：纯枚举
来源：http://ccx.cqqwz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://erm.vqdsnc.cn

[U49] PHP：只读属性
来源：http://hls.vehdjk.com

public readonly string $name
来源：http://gww.zhiwuduotai.top

[U50] PHP：构造器属性提升
来源：http://okh.hfpthk.cn

public function __construct(private int $id) {}
来源：http://jhb.jiagoushi.top

[U51] PHP：数组解构
来源：http://cdn.gogol.net.cn

[$a, $b] = $arr;
来源：http://gtc.smart0.xyz

[U52] PHP：箭头函数
来源：http://djt.fzhhl.top

$double = fn($x) => $x * 2;
来源：http://los.jinqigufen.top

[U53] PHP：空合并运算符
来源：http://xmd.fzhhl.top

$v = $a ?? $b ?? "default";
来源：http://esq.shangyingyoupin.top

[U54] PHP：空安全调用
来源：http://bqs.yanxiufei.cn

$obj?->method()
来源：http://yul.tarul.cn

[U55] PHP：match 表达式
来源：http://skh.jqgfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yyi.hnxiangtu.top

[U56] PHP：命名参数
来源：http://msn.yvedp.cn

f(a: 1, b: 2)
来源：http://rbj.fzhhl.top

[U57] PHP：字符串插值
来源：http://jws.smart0.xyz

"值: {$a}"
来源：http://uap.smart0.xyz

[U58] PHP：数组三件套
来源：http://mnq.gotoacloud.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tqo.yonumen.top

[U59] PHP：自定义排序
来源：http://bnb.gotoacloud.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uge.hnqzz.top

[U60] PHP：JSON 编解码
来源：http://tod.jyoumei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vvf.hysaishi.cn

[U61] PHP：正则
来源：http://apz.quarkkingdee.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nzi.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://glp.shanyushiyangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lga.xingfuxueyuan.xyz

[U63] PHP：文件读写
来源：http://ztb.ctjpmb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jcq.ybcxt.top

[U64] PHP：目录遍历
来源：http://hsx.dianchejie.cn

glob("dir/*.php");  scandir("dir");
来源：http://cxf.ydjk.org.cn

[U65] PHP：会话
来源：http://kcv.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xwj.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://exf.jiagoushi.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oyx.sufxvd.cn

[U67] PHP：处理文件上传
来源：http://osp.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bmc.yanxiufei.cn

[U68] PHP：PDO 连接
来源：http://oar.iojbl.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rng.dashuyun.cn

[U69] PHP：PDO 预处理
来源：http://lct.dianchejie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zyl.c1oappe.top

[U70] PHP：PDO 事务
来源：http://lfi.nanxinkj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mmj.zhongyouzk.top

[U71] PHP：抛出异常
来源：http://fjc.jinyuanbaomall.cn

throw new RuntimeException("失败", 500);
来源：http://slv.zycfv.cn

[U72] PHP：写错误日志
来源：http://rgw.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://won.jinqigufen.top

[U73] PHP：读取 ini 配置
来源：http://izj.c1oappe.top

parse_ini_file("config.ini", true)
来源：http://cnw.jlsjyb.cn

[U74] PHP：读取环境变量
来源：http://yuo.smart0.xyz

getenv("APP_ENV") ?: "production"
来源：http://ipz.chenzaomai.com

[U75] PHP：依赖注入
来源：http://myf.jqgufenzy.top

composer require psr/container
来源：http://rzg.tarul.cn

[U76] PHP：简单路由
来源：http://lxh.yj20258.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ugj.ppjwa.cn

[U77] PHP：模板渲染
来源：http://coq.birdmap.top

composer require twig/twig
来源：http://orj.yfazqb.com

[U78] PHP：单元测试
来源：http://aue.bjfxy.top

composer require --dev phpunit/phpunit
来源：http://zdz.gaohongyu789.top

[U79] PHP：静态分析
来源：http://wio.c1oappe.top

composer require --dev phpstan/phpstan
来源：http://gta.zhijiandao.cn

[U80] PHP：代码规范修复
来源：http://nhh.fanxiaobao.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://xin.jinqigufen.top

[U81] JS：初始化项目
来源：http://kdn.guannengcc.top

npm init -y;  npm i express
来源：http://gfc.daria6918.cn

[U82] JS：package.json 脚本
来源：http://pnc.feifeiyinyue.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://aqq.daxiang520.top

[U83] JS：ES Module 导入导出
来源：http://xof.nanxinkj.top

export const a = 1;  import { a } from "./m.js";
来源：http://hhy.smart0.xyz

[U84] JS：CommonJS 写法
来源：http://hmj.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://mle.hesvh.cn

[U85] JS：可选链
来源：http://llx.zhiwuduotai.top

a?.b?.c
来源：http://fdh.zhengqikj.top

[U86] JS：空值合并
来源：http://krg.snrcjt.cn

a ?? b
来源：http://wif.shuidangran.top

[U87] JS：解构默认值
来源：http://esc.redwolf501.top

const { a = 1, b = 2 } = obj;
来源：http://zjt.bbcook.cn

[U88] JS：对象展开合并
来源：http://myg.epnwcf.com

{ ...a, ...b }
来源：http://ipy.pycfn.com

[U89] JS：数组去重
来源：http://cir.yvedp.cn

[...new Set(arr)]
来源：http://onv.shanyushiyangkeji.top

[U90] JS：数字数组排序
来源：http://fsu.cheryme.top

[...arr].sort((a, b) => a - b)
来源：http://abn.iojbl.cn

[U91] JS：对象键值遍历
来源：http://drn.ywan-chungtsiang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vhy.jlsjyb.cn

[U92] JS：深拷贝
来源：http://eiu.chenlongwang.top

structuredClone(obj)
来源：http://gyb.gotoacloud.top

[U93] JS：模板字符串
来源：http://iol.zhiwuduotai.top

`共 ${n} 条`
来源：http://wrp.xylfe.cn

[U94] JS：箭头函数
来源：http://iwv.zhongyouzk.top

const double = x => x * 2;
来源：http://pco.zhengqikj.top

[U95] JS：Promise 包装
来源：http://ooy.sjlbkw.cn

new Promise((resolve, reject) => {})
来源：http://hyv.zdqjudy.top

[U96] JS：async/await 与异常
来源：http://iza.chenzaomai.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://njw.nanxinkj.top

[U97] JS：并发请求
来源：http://rrf.xinyue.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://uti.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://cpt.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xpl.epnwcf.com

[U99] JS：事件监听
来源：http://tfs.yanxiufei.cn

el.addEventListener("click", e => {})
来源：http://ckw.52xcode.cn

[U100] JS：DOM 查询
来源：http://vjn.jlsjyb.cn

document.querySelector(".item")
来源：http://jwt.gaohongyu789.top

[U101] JS：classList 操作
来源：http://ojq.zhoulong.xyz

el.classList.toggle("active")
来源：http://wsx.chenjidiqi.icu

[U102] JS：本地存储
来源：http://eko.uphjek.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://iui.zycfv.cn

[U103] JS：定时器
来源：http://cus.dianchejie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://weg.jianghu66.top

[U104] JS：防抖
来源：http://xxf.hammf.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zhy.zhijiandao.cn

[U105] JS：节流
来源：http://xlw.shuidangran.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mpm.shzxlz.cn

[U106] JS：日期格式化
来源：http://ciz.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aai.gogol.net.cn

[U107] JS：数字千分位
来源：http://lsg.hnxiangtu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qex.hcnkem.com

[U108] JS：随机整数
来源：http://waa.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vqi.fzhhl.top

[U109] JS：数组分组
来源：http://vmq.jlsjyb.cn

Object.groupBy(arr, x => x.type)
来源：http://vdo.9152youxi.cn

[U110] JS：数组分块
来源：http://ufi.0kj1m.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qtm.yj20258888.top

[U111] JS：对象转 Map
来源：http://deh.redwolf501.top

new Map(Object.entries(obj))
来源：http://eym.xylfe.cn

[U112] JS：字符串补位
来源：http://erq.xuanzx.com

"7".padStart(3, "0")
来源：http://imq.xziqi.cn

[U113] JS：正则替换全部
来源：http://qyu.hnqzz.top

s.replaceAll("a", "b")
来源：http://fki.jinyuanbaomall.cn

[U114] JS：JSON 深比较
来源：http://sas.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fjt.hysaishi.cn

[U115] JS：生成 UUID
来源：http://naa.dianchejie.cn

crypto.randomUUID()
来源：http://vqd.yanxiufei.cn

[U116] JS：类型检查（JSDoc）
来源：http://ddq.jinqigfzy.top

/** @param {string} name */ function f(name) {}
来源：http://kmn.uphjek.com

[U117] JS：单元测试
来源：http://enb.zhengqikj.top

npm i -D vitest;  npx vitest
来源：http://vts.cucudq.cn

[U118] JS：开发服务器
来源：http://zie.yvedp.cn

npm i -D vite;  npx vite
来源：http://ksr.bjfxy.top

[U119] JS：生产构建
来源：http://ozr.ydjk.org.cn

npx vite build
来源：http://vpe.shzxlz.cn

[U120] JS：读取环境变量（Vite）
来源：http://fvx.nanxuanxn.top

import.meta.env.VITE_API_URL
来源：http://wuk.ppjwa.cn

================================================================================
来源：http://kgp.vqdsnc.cn

统计汇总
来源：http://kmr.nanxuanxn.top

================================================================================
来源：http://rav.jinyuanbaomall.cn

按语言统计（条）：
来源：http://far.nanxuanxn.top


<!-- 参考信息 -->