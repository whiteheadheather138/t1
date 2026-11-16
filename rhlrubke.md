代发 wailian999

[T37] Lua：字符串拼接
来源：http://ulc.xziqi.cn

"a" .. "b"
来源：http://uay.xinyue.icu

[T38] Lua：条件
来源：http://kkv.gogol.net.cn

if x > 0 then print("正") end
来源：http://gey.zhengqikj.top

[T39] Lua：模式匹配
来源：http://iid.sufxvd.cn

string.find(s, "%d+")
来源：http://erj.cashguo.top

[T40] Lua：元表
来源：http://rgr.tianlin.xyz

setmetatable({}, { __index = base })
来源：http://hqp.dashuyun.cn

[T41] Perl：Hello World
来源：http://sdy.tarul.cn

print "Hello\n";
来源：http://qrf.yfazqb.com

[T42] Perl：变量类型
来源：http://tpr.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wwd.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://xif.jiagoushi.top

"值: $a"
来源：http://ubd.svipenyu.cn

[T44] Perl：条件
来源：http://flg.yuxming.cn

if ($a > 0) { print "正"; }
来源：http://zqb.xuanzx.com

[T45] Perl：数组遍历
来源：http://suy.haohaochexian.top

for my $x (@arr) { print $x; }
来源：http://ink.9152youxi.cn

[T46] Perl：哈希操作
来源：http://njl.svipenyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ule.quarkkingdee.top

[T47] Perl：正则捕获
来源：http://xfi.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://xgt.nanxuanxn.top

[T48] Perl：正则替换
来源：http://tzb.shanyushiyangtech.top

$s =~ s/old/new/g;
来源：http://ctw.wangdashe.top

[T49] Perl：函数
来源：http://mvk.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xti.yuxming.cn

[T50] Perl：逐行读文件
来源：http://dcb.fehbvm.com

open my $fh, "<", "a.txt" or die $!;
来源：http://vjf.sufxvd.cn

while (my $line = <$fh>) { print $line; }
来源：http://fus.c1oappe.top

[T51] Scala：Hello World
来源：http://kqf.jinyuanbaomall.cn

println("Hello")
来源：http://xnt.yueranfly.top

[T52] Scala：变量
来源：http://zyt.kuanghao11.cn

val a = 1;  var b = 2
来源：http://den.yueranfly.top

[T53] Scala：字符串插值
来源：http://tip.fengsongda.top

s"值: $b"
来源：http://dus.aibaodan.cn

[T54] Scala：集合映射
来源：http://gne.jqgfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://inb.xuanzx.com

[T55] Scala：集合过滤
来源：http://xkw.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://vyl.zycfv.cn

[T56] Scala：样例类
来源：http://maa.tarul.cn

case class User(name: String, age: Int)
来源：http://qnl.jianghu66.top

[T57] Scala：模式匹配
来源：http://arp.hysaishi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gja.hysaishi.cn

[T58] Scala：函数定义
来源：http://zhb.andypj.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://zhp.cqqwz.cn

[T59] Scala：循环
来源：http://ynx.fehbvm.com

for (i <- 1 to 10) println(i)
来源：http://hie.jyoumei.cn

[T60] Scala：折叠
来源：http://spz.hongshengwenyu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vts.hnxiangtu.top

================================================================================
来源：http://hoq.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://glc.zhixingplan.top

================================================================================
来源：http://ezf.chenlongwang.top

[U01] Py：创建虚拟环境
来源：http://oih.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://twa.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://sho.yuxming.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dea.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://tpl.ctjpmb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://cop.cdnleiting.top

[U04] Py：变量调试打印
来源：http://xji.0kj1m.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kpr.yongpay.top

[U05] Py：列表去重且保序
来源：http://fom.wangshuangyany.cn

list(dict.fromkeys(arr))
来源：http://efu.52xcode.cn

[U06] Py：合并两个字典
来源：http://qxm.ydzc1.top

{**a, **b}
来源：http://dan.fengsongda.top

[U07] Py：反转字典键值
来源：http://xsf.wangdashe.top

{v: k for k, v in d.items()}
来源：http://oqh.yonumen.top

[U08] Py：展平二维列表
来源：http://xqm.havefunace.top

[y for x in nested for y in x]
来源：http://cee.zdqjudy.top

[U09] Py：字典取最大值的键
来源：http://cwv.cdnleiting.top

max(d, key=d.get)
来源：http://pkj.gaohongyu789.top

[U10] Py：按值排序字典
来源：http://vxc.wangshuangyany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pya.andypj.xyz

[U11] Py：生成器表达式
来源：http://ybp.daxiang520.top

(x * 2 for x in arr)
来源：http://npx.nanxinkj.top

[U12] Py：取出现最多的 3 个元素
来源：http://gfx.ydjk.org.cn

Counter(arr).most_common(3)
来源：http://ghq.zdbjq.cn

[U13] Py：固定长度队列
来源：http://ngh.zdqjudy.top

deque(maxlen=10)
来源：http://pvs.316326.xyz

[U14] Py：分组收集到列表
来源：http://kyz.shuidangran.top

defaultdict(list)
来源：http://tsj.nanxinkj.top

[U15] Py：高精度计时
来源：http://zks.gotoacloud.top

t = time.perf_counter()
来源：http://qim.cucudq.cn

[U16] Py：命令行参数解析
来源：http://xzl.yanxiufei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tre.gotoacloud.top

[U17] Py：初始化日志
来源：http://jks.ywan-chungtsiang.top

logging.basicConfig(level=logging.INFO)
来源：http://nns.sysykeji.top

[U18] Py：预编译正则
来源：http://rnh.jinqigfzy.top

pat = re.compile(r"\d+")
来源：http://cxj.fzhhl.top

[U19] Py：正则替换带回调
来源：http://itu.nanxinkj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zcw.havefunace.top

[U20] Py：缓存函数结果
来源：http://osa.yvedp.cn

@functools.lru_cache(maxsize=None)
来源：http://cax.shzxlz.cn

[U21] Py：自定义上下文管理器
来源：http://wwz.zhixingplan.top

@contextlib.contextmanager
来源：http://hfm.wangdashe.top

[U22] Py：矩阵转置
来源：http://gpl.svipenyu.cn

list(zip(*m))
来源：http://zrh.hongshengwenyu.top

[U23] Py：分块读取大文件
来源：http://pmx.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iia.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://rte.xinyue.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lgs.sweek.top

[U25] Py：CSV 按字典读
来源：http://hkf.ivvv.top

csv.DictReader(f)
来源：http://sej.jyoumei.cn

[U26] Py：并发下载
来源：http://pfs.pycfn.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lqh.zdqjudy.top

[U27] Py：异步 HTTP
来源：http://ten.yj202588.top

aiohttp.ClientSession() 配合 async with
来源：http://djl.jqgufenzy.top

[U28] Py：类型别名
来源：http://gsl.vehdjk.com

UserId = int
来源：http://nxl.sufxvd.cn

[U29] Py：属性校验
来源：http://awt.feifeiyinyue.top

@property 与 @x.setter 配合
来源：http://rki.kuanghao11.cn

[U30] Py：数据类
来源：http://djf.quarkkingdee.top

@dataclass(slots=True)
来源：http://kei.hywenlv.cn

[U31] Py：单测
来源：http://req.aizwys.cn

python -m pytest -q
来源：http://glw.daria6918.cn

[U32] Py：代码格式化
来源：http://hja.wangdashe.top

ruff format . && ruff check --fix .
来源：http://btt.jinyuanbaomall.cn

[U33] Py：打包发布
来源：http://snx.birdmap.top

python -m build  （依赖 pyproject.toml）
来源：http://mfu.daria6918.cn

[U34] Py：判断编码
来源：http://xip.yongpay.top

chardet.detect(raw)
来源：http://vwc.0kj1m.cn

[U35] Py：发送邮件
来源：http://bil.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tjo.dashuyun.cn

[U36] Py：定时任务
来源：http://fgp.tanke756.top

schedule.every(10).minutes.do(job)
来源：http://ddh.vehdjk.com

[U37] Py：读写 Excel
来源：http://gse.hysaishi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bye.zdqjudy.top

[U38] Py：获取脚本所在目录
来源：http://kgm.redwolf501.top

Path(__file__).resolve().parent
来源：http://zeg.zdqjudy.top

[U39] Py：判断是否在交互环境
来源：http://usu.cqqwz.cn

sys.stdout.isatty()
来源：http://cac.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://ifn.guannengcc.top

print("err", file=sys.stderr)
来源：http://vxs.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://xnt.cheryme.top

composer init;  composer require guzzlehttp/guzzle
来源：http://sxu.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://kqh.fktsv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lhb.jinqigufen.top

[U43] PHP：声明命名空间
来源：http://iog.gotoacloud.top

namespace App\Http;
来源：http://nlc.yfazqb.com

[U44] PHP：开启严格类型
来源：http://kwm.hfpthk.cn

declare(strict_types=1);
来源：http://bbb.gogol.net.cn

[U45] PHP：类型声明与返回类型
来源：http://xtq.hnxiangtu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pxy.sysykeji.top

[U46] PHP：可空类型
来源：http://lsj.fengsongda.top

?string $name = null
来源：http://bvr.cashguo.top

[U47] PHP：联合类型
来源：http://wcb.dashuyun.cn

int|string $id
来源：http://orw.9152youxi.cn

[U48] PHP：纯枚举
来源：http://abm.iojbl.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jbl.ybcxt.top

[U49] PHP：只读属性
来源：http://kmg.shangyingyoupin.top

public readonly string $name
来源：http://ovm.ywan-chungtsiang.top

[U50] PHP：构造器属性提升
来源：http://sxm.jinqigufen.top

public function __construct(private int $id) {}
来源：http://leo.gaohongyu789.top

[U51] PHP：数组解构
来源：http://wjn.yanxiufei.cn

[$a, $b] = $arr;
来源：http://lwb.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://exs.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://ipm.guowangkeji.top

[U53] PHP：空合并运算符
来源：http://duo.yvedp.cn

$v = $a ?? $b ?? "default";
来源：http://bdf.fzhhl.top

[U54] PHP：空安全调用
来源：http://ytt.nanxuanxn.top

$obj?->method()
来源：http://zul.xuanzx.com

[U55] PHP：match 表达式
来源：http://dvu.nanxinkj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rxp.sufxvd.cn

[U56] PHP：命名参数
来源：http://hwg.yvedp.cn

f(a: 1, b: 2)
来源：http://sje.xuetiantiany.cn

[U57] PHP：字符串插值
来源：http://ydr.wangshuangyany.cn

"值: {$a}"
来源：http://ojs.fzhhl.top

[U58] PHP：数组三件套
来源：http://crl.meibo888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ubu.zycfv.cn

[U59] PHP：自定义排序
来源：http://ovh.fktsv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wmp.yvedp.cn

[U60] PHP：JSON 编解码
来源：http://pjw.xuanzx.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ymn.tanke756.top

[U61] PHP：正则
来源：http://oxo.snrcjt.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lrv.dianchejie.cn

[U62] PHP：日期对象
来源：http://glh.chenjidiqi.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lnv.yj20258888.top

[U63] PHP：文件读写
来源：http://aiz.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://drp.xingfuxueyuan.xyz

[U64] PHP：目录遍历
来源：http://qlg.epnwcf.com

glob("dir/*.php");  scandir("dir");
来源：http://uix.yvedp.cn

[U65] PHP：会话
来源：http://xoa.zhoulong.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://ijk.yongpay.top

[U66] PHP：设置 Cookie
来源：http://wdl.fzhhl.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yxw.nwbrower.top

[U67] PHP：处理文件上传
来源：http://chr.hesvh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://axs.wangshuangyany.cn

[U68] PHP：PDO 连接
来源：http://wbn.shangyingyoupin.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gxs.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://yko.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eja.fengsongda.top

[U70] PHP：PDO 事务
来源：http://xki.zycfv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tcc.zhoulong.xyz

[U71] PHP：抛出异常
来源：http://vjh.xuanzx.com

throw new RuntimeException("失败", 500);
来源：http://dnk.jinqigufen.top

[U72] PHP：写错误日志
来源：http://qeg.havefunace.top

error_log("失败: " . $e->getMessage());
来源：http://pjo.xylfe.cn

[U73] PHP：读取 ini 配置
来源：http://rhm.ydjk.org.cn

parse_ini_file("config.ini", true)
来源：http://kbq.ctjpmb.com

[U74] PHP：读取环境变量
来源：http://qfj.xuanzx.com

getenv("APP_ENV") ?: "production"
来源：http://rai.yj20258888.top

[U75] PHP：依赖注入
来源：http://hnq.bbcook.cn

composer require psr/container
来源：http://vze.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://dlw.uphjek.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ffl.yonumen.top

[U77] PHP：模板渲染
来源：http://ima.nanxuanxn.top

composer require twig/twig
来源：http://ezk.yanxiufei.cn

[U78] PHP：单元测试
来源：http://bcn.zhiwuduotai.top

composer require --dev phpunit/phpunit
来源：http://xjd.birdmap.top

[U79] PHP：静态分析
来源：http://gxn.cheryme.top

composer require --dev phpstan/phpstan
来源：http://cxi.jinqigufen.top

[U80] PHP：代码规范修复
来源：http://wai.yangfankeji.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://xne.hnxiangtu.top

[U81] JS：初始化项目
来源：http://qox.jinqigufen.top

npm init -y;  npm i express
来源：http://lly.ydjk.org.cn

[U82] JS：package.json 脚本
来源：http://sdq.52xcode.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zyf.guannengcc.top

[U83] JS：ES Module 导入导出
来源：http://kaa.jiagoushi.top

export const a = 1;  import { a } from "./m.js";
来源：http://hib.aibaodan.cn

[U84] JS：CommonJS 写法
来源：http://xws.epnwcf.com

module.exports = { a };  const { a } = require("./m");
来源：http://jcf.hnqzz.top

[U85] JS：可选链
来源：http://yxq.snrcjt.cn

a?.b?.c
来源：http://wdv.shanyushiyangkeji.top

[U86] JS：空值合并
来源：http://pbg.tian-w.cn

a ?? b
来源：http://cei.hnxiangtu.top

[U87] JS：解构默认值
来源：http://wzn.jqgufenzy.top

const { a = 1, b = 2 } = obj;
来源：http://tqy.shangyingyoupin.top

[U88] JS：对象展开合并
来源：http://hqe.dianchejie.cn

{ ...a, ...b }
来源：http://cvn.chenzaomai.com

[U89] JS：数组去重
来源：http://agz.guowangkeji.top

[...new Set(arr)]
来源：http://mfx.dianchejie.cn

[U90] JS：数字数组排序
来源：http://ued.zhongyouzk.top

[...arr].sort((a, b) => a - b)
来源：http://toy.jinqigufen.top

[U91] JS：对象键值遍历
来源：http://dfi.hcnkem.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tti.zdqjudy.top

[U92] JS：深拷贝
来源：http://nqr.havefunace.top

structuredClone(obj)
来源：http://pgc.zycfv.cn

[U93] JS：模板字符串
来源：http://ruc.fktsv.cn

`共 ${n} 条`
来源：http://cda.tarul.cn

[U94] JS：箭头函数
来源：http://ohu.yanxiufei.cn

const double = x => x * 2;
来源：http://ois.sjlbkw.cn

[U95] JS：Promise 包装
来源：http://jbz.tanke756.top

new Promise((resolve, reject) => {})
来源：http://npw.kuanghao11.cn

[U96] JS：async/await 与异常
来源：http://lqw.ppjwa.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xax.fehbvm.com

[U97] JS：并发请求
来源：http://iqb.quarkkingdee.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://uxs.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://czg.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://aqy.shanyushiyangtech.top

[U99] JS：事件监听
来源：http://hyi.fehbvm.com

el.addEventListener("click", e => {})
来源：http://ofg.xuanzx.com

[U100] JS：DOM 查询
来源：http://xus.chenzaomai.com

document.querySelector(".item")
来源：http://rzv.zhaomingkeji.xyz

[U101] JS：classList 操作
来源：http://abv.snrcjt.cn

el.classList.toggle("active")
来源：http://tgr.hesvh.cn

[U102] JS：本地存储
来源：http://mpp.quarkkingdee.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qya.hnqzz.top

[U103] JS：定时器
来源：http://tqz.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yln.shzxlz.cn

[U104] JS：防抖
来源：http://ohc.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qoe.shangyingyoupin.top

[U105] JS：节流
来源：http://guq.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pdq.pycfn.com

[U106] JS：日期格式化
来源：http://deo.jlsjyb.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vrl.quarkkingdee.top

[U107] JS：数字千分位
来源：http://lri.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vgr.vehdjk.com

[U108] JS：随机整数
来源：http://ilq.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vuf.ppjwa.cn

[U109] JS：数组分组
来源：http://rrv.vehdjk.com

Object.groupBy(arr, x => x.type)
来源：http://vff.guannengcc.top

[U110] JS：数组分块
来源：http://zal.zdqjudy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://djp.iojbl.cn

[U111] JS：对象转 Map
来源：http://vnx.zhaomingkeji.xyz

new Map(Object.entries(obj))
来源：http://ovj.quarkkingdee.top

[U112] JS：字符串补位
来源：http://mug.yj20258888.top

"7".padStart(3, "0")
来源：http://mkh.bjfxy.top

[U113] JS：正则替换全部
来源：http://lvc.hcnkem.com

s.replaceAll("a", "b")
来源：http://avm.quarkkingdee.top

[U114] JS：JSON 深比较
来源：http://qck.hywenlv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hul.jyoumei.cn

[U115] JS：生成 UUID
来源：http://gob.xylfe.cn

crypto.randomUUID()
来源：http://nzh.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://teg.havefunace.top

/** @param {string} name */ function f(name) {}
来源：http://rub.yfazqb.com

[U117] JS：单元测试
来源：http://non.yfazqb.com

npm i -D vitest;  npx vitest
来源：http://ret.guowangkeji.top

[U118] JS：开发服务器
来源：http://uos.jinqigufen.top

npm i -D vite;  npx vite
来源：http://hys.fzhhl.top

[U119] JS：生产构建
来源：http://siw.andypj.xyz

npx vite build
来源：http://boa.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://bzl.chenzaomai.com

import.meta.env.VITE_API_URL
来源：http://qnp.ehwqpu.com

================================================================================
来源：http://hmo.wangdashe.top

统计汇总
来源：http://cnu.yvedp.cn

================================================================================
来源：http://qex.316326.xyz

按语言统计（条）：
来源：http://rqo.yj20258888.top

Python ......... 252
来源：http://ulh.dianchejie.cn

PHP ............ 252
来源：http://zlq.birdmap.top

JavaScript ..... 252
来源：http://oro.nanxinkj.top

TypeScript ..... 212
来源：http://muf.cheryme.top


<!-- 参考信息 -->