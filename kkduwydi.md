代发 wailian999

[T39] Lua：模式匹配
来源：http://lhd.tanke756.top

string.find(s, "%d+")
来源：http://clk.tianlin.xyz

[T40] Lua：元表
来源：http://onf.zhongyouzk.top

setmetatable({}, { __index = base })
来源：http://kqk.fanxiaobao.xyz

[T41] Perl：Hello World
来源：http://ouz.fktsv.cn

print "Hello\n";
来源：http://ejq.shanyushiyangtech.top

[T42] Perl：变量类型
来源：http://vha.epnwcf.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ddj.wangdashe.top

[T43] Perl：字符串插值
来源：http://rgi.nwbrower.top

"值: $a"
来源：http://vbi.tarul.cn

[T44] Perl：条件
来源：http://jwo.yangfankeji.com

if ($a > 0) { print "正"; }
来源：http://zdz.jinyuanbaomall.cn

[T45] Perl：数组遍历
来源：http://gew.zhixingplan.top

for my $x (@arr) { print $x; }
来源：http://cdb.dashuyun.cn

[T46] Perl：哈希操作
来源：http://kta.shuidangran.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jnh.c1oappe.top

[T47] Perl：正则捕获
来源：http://ypy.tian-w.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wvt.dashuyun.cn

[T48] Perl：正则替换
来源：http://ook.cqqwz.cn

$s =~ s/old/new/g;
来源：http://oii.cucudq.cn

[T49] Perl：函数
来源：http://kgx.havefunace.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://npa.sysykeji.top

[T50] Perl：逐行读文件
来源：http://mub.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dvc.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://fot.ywan-chungtsiang.top

[T51] Scala：Hello World
来源：http://yie.jqgfzy.top

println("Hello")
来源：http://zsn.tianlin.xyz

[T52] Scala：变量
来源：http://nqt.hnxiangtu.top

val a = 1;  var b = 2
来源：http://hpq.xuetiantiany.cn

[T53] Scala：字符串插值
来源：http://vtz.sweek.top

s"值: $b"
来源：http://mry.jinqigfzy.top

[T54] Scala：集合映射
来源：http://msk.ywan-chungtsiang.top

List(1, 2, 3).map(_ * 2)
来源：http://onn.zdqjudy.top

[T55] Scala：集合过滤
来源：http://yis.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://txt.fengsongda.top

[T56] Scala：样例类
来源：http://szt.nanxinkj.top

case class User(name: String, age: Int)
来源：http://nqa.meibo888.top

[T57] Scala：模式匹配
来源：http://ekg.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dvh.yj20258888.top

[T58] Scala：函数定义
来源：http://nlg.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://jik.yonumen.top

[T59] Scala：循环
来源：http://vyi.feifeiyinyue.top

for (i <- 1 to 10) println(i)
来源：http://hat.gotoacloud.top

[T60] Scala：折叠
来源：http://omy.yfazqb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fzu.xinyue.icu

================================================================================
来源：http://pyf.iojbl.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://foh.fehbvm.com

================================================================================
来源：http://srt.wangdashe.top

[U01] Py：创建虚拟环境
来源：http://dds.nwbrower.top

python -m venv .venv && source .venv/bin/activate
来源：http://wvg.uphjek.com

[U02] Py：导出 / 安装依赖
来源：http://rvv.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://axk.haohaochexian.top

[U03] Py：加载 .env 配置
来源：http://cpf.jinyuanbaomall.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cvv.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://tfi.sjlbkw.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yvh.guowangkeji.top

[U05] Py：列表去重且保序
来源：http://ehe.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://xrv.dashuyun.cn

[U06] Py：合并两个字典
来源：http://uua.sufxvd.cn

{**a, **b}
来源：http://ywg.fengsongda.top

[U07] Py：反转字典键值
来源：http://hwd.iojbl.cn

{v: k for k, v in d.items()}
来源：http://rby.zhongyouzk.top

[U08] Py：展平二维列表
来源：http://ffp.nanxuanxn.top

[y for x in nested for y in x]
来源：http://upc.sxryk.cn

[U09] Py：字典取最大值的键
来源：http://fhi.nanxinkj.top

max(d, key=d.get)
来源：http://lbb.jyoumei.cn

[U10] Py：按值排序字典
来源：http://csa.yj20258.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nme.dianchejie.cn

[U11] Py：生成器表达式
来源：http://tma.mhx1999.top

(x * 2 for x in arr)
来源：http://dda.andypj.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://ume.ppjwa.cn

Counter(arr).most_common(3)
来源：http://swi.meibo888.top

[U13] Py：固定长度队列
来源：http://vuz.zdqjudy.top

deque(maxlen=10)
来源：http://ukg.cheryme.top

[U14] Py：分组收集到列表
来源：http://dqk.aibaodan.cn

defaultdict(list)
来源：http://yrt.fengsongda.top

[U15] Py：高精度计时
来源：http://fiz.smart0.xyz

t = time.perf_counter()
来源：http://aff.yj202588.top

[U16] Py：命令行参数解析
来源：http://fha.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yue.ppjwa.cn

[U17] Py：初始化日志
来源：http://jsy.sweek.top

logging.basicConfig(level=logging.INFO)
来源：http://fdu.daxiang520.top

[U18] Py：预编译正则
来源：http://tvm.guannengcc.top

pat = re.compile(r"\d+")
来源：http://dxz.9152youxi.cn

[U19] Py：正则替换带回调
来源：http://nni.c1oappe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lbz.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://cri.smart0.xyz

@functools.lru_cache(maxsize=None)
来源：http://wts.wangdashe.top

[U21] Py：自定义上下文管理器
来源：http://lfi.shanyushiyangtech.top

@contextlib.contextmanager
来源：http://xqx.ydzc1.top

[U22] Py：矩阵转置
来源：http://nvb.gaohongyu789.top

list(zip(*m))
来源：http://iiy.yj20258.top

[U23] Py：分块读取大文件
来源：http://nmg.fktsv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ieg.xziqi.cn

[U24] Py：路径操作
来源：http://vzu.sysykeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bcm.yj20258.top

[U25] Py：CSV 按字典读
来源：http://oif.kuanghao11.cn

csv.DictReader(f)
来源：http://bsx.9152youxi.cn

[U26] Py：并发下载
来源：http://foo.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fhx.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://ihj.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://ghd.nanxinkj.top

[U28] Py：类型别名
来源：http://ipj.fengsongda.top

UserId = int
来源：http://vto.hesvh.cn

[U29] Py：属性校验
来源：http://kop.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://omx.fengsongda.top

[U30] Py：数据类
来源：http://peu.cashguo.top

@dataclass(slots=True)
来源：http://weh.tianlin.xyz

[U31] Py：单测
来源：http://zje.fengsongda.top

python -m pytest -q
来源：http://mia.yongpay.top

[U32] Py：代码格式化
来源：http://rae.haohaochexian.top

ruff format . && ruff check --fix .
来源：http://drv.shangyingyoupin.top

[U33] Py：打包发布
来源：http://ecf.sweek.top

python -m build  （依赖 pyproject.toml）
来源：http://xuh.zhijiandao.cn

[U34] Py：判断编码
来源：http://cpg.feifeiyinyue.top

chardet.detect(raw)
来源：http://qbq.svipenyu.cn

[U35] Py：发送邮件
来源：http://axt.yueranfly.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dev.andypj.xyz

[U36] Py：定时任务
来源：http://tto.pycfn.com

schedule.every(10).minutes.do(job)
来源：http://zsg.9152youxi.cn

[U37] Py：读写 Excel
来源：http://xmx.vehdjk.com

pandas.read_excel / DataFrame.to_excel
来源：http://ejs.ywan-chungtsiang.top

[U38] Py：获取脚本所在目录
来源：http://qwa.yuxming.cn

Path(__file__).resolve().parent
来源：http://mtu.hcnkem.com

[U39] Py：判断是否在交互环境
来源：http://swb.yuxming.cn

sys.stdout.isatty()
来源：http://rcc.uphjek.com

[U40] Py：打印到标准错误
来源：http://ldm.aizwys.cn

print("err", file=sys.stderr)
来源：http://rit.fzhhl.top

[U41] PHP：初始化 Composer 项目
来源：http://uzv.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://iwi.yj20258.top

[U42] PHP：PSR-4 自动加载
来源：http://pvx.nanxinkj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ulz.jinqigufen.top

[U43] PHP：声明命名空间
来源：http://pnu.aibaodan.cn

namespace App\Http;
来源：http://rxp.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://yyk.chenzaomai.com

declare(strict_types=1);
来源：http://uwp.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://qbp.tarul.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oax.gogol.net.cn

[U46] PHP：可空类型
来源：http://nyn.haohaochexian.top

?string $name = null
来源：http://uch.meibo888.top

[U47] PHP：联合类型
来源：http://ngq.tarul.cn

int|string $id
来源：http://ugu.zycfv.cn

[U48] PHP：纯枚举
来源：http://grh.wangdashe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vyj.shuidangran.top

[U49] PHP：只读属性
来源：http://yxl.xuetiantiany.cn

public readonly string $name
来源：http://iie.hammf.cn

[U50] PHP：构造器属性提升
来源：http://lmm.gaohongyu789.top

public function __construct(private int $id) {}
来源：http://dqb.mhx1999.top

[U51] PHP：数组解构
来源：http://zdu.vqdsnc.cn

[$a, $b] = $arr;
来源：http://xcp.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://qjs.316326.xyz

$double = fn($x) => $x * 2;
来源：http://yqi.redwolf501.top

[U53] PHP：空合并运算符
来源：http://sph.316326.xyz

$v = $a ?? $b ?? "default";
来源：http://ukn.yuanzhike.top

[U54] PHP：空安全调用
来源：http://xkx.zhixingplan.top

$obj?->method()
来源：http://wbs.gotoacloud.top

[U55] PHP：match 表达式
来源：http://tni.andypj.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jkw.zhaomingkeji.xyz

[U56] PHP：命名参数
来源：http://fok.hammf.cn

f(a: 1, b: 2)
来源：http://fhm.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://lmt.smart0.xyz

"值: {$a}"
来源：http://fqm.jqgfzy.top

[U58] PHP：数组三件套
来源：http://tni.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://utx.pengpengdd.cyou

[U59] PHP：自定义排序
来源：http://mdl.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xly.ehwqpu.com

[U60] PHP：JSON 编解码
来源：http://saa.ppjwa.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yra.yfazqb.com

[U61] PHP：正则
来源：http://wlj.jinghuilouyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://syi.cqqwz.cn

[U62] PHP：日期对象
来源：http://jrl.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fek.gaohongyu789.top

[U63] PHP：文件读写
来源：http://itb.hongshengwenyu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xhk.yangfankeji.com

[U64] PHP：目录遍历
来源：http://qja.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://ahw.fktsv.cn

[U65] PHP：会话
来源：http://its.meibo888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://oli.xuanzx.com

[U66] PHP：设置 Cookie
来源：http://efg.feifeiyinyue.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ysg.c1oappe.top

[U67] PHP：处理文件上传
来源：http://amw.shangyingyoupin.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gzh.ybcxt.top

[U68] PHP：PDO 连接
来源：http://gad.jlsjyb.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://twb.xuanzx.com

[U69] PHP：PDO 预处理
来源：http://zwt.zdqjudy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mlt.yj20258.top

[U70] PHP：PDO 事务
来源：http://wlz.tianlin.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qld.hnxiangtu.top

[U71] PHP：抛出异常
来源：http://dqe.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://vuc.ehwqpu.com

[U72] PHP：写错误日志
来源：http://qfq.shanyushiyangtech.top

error_log("失败: " . $e->getMessage());
来源：http://zcw.hcnkem.com

[U73] PHP：读取 ini 配置
来源：http://gfb.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://dei.zycfv.cn

[U74] PHP：读取环境变量
来源：http://rnc.0kj1m.cn

getenv("APP_ENV") ?: "production"
来源：http://vci.chenzaomai.com

[U75] PHP：依赖注入
来源：http://mzb.hongshengwenyu.top

composer require psr/container
来源：http://isr.wangshuangyany.cn

[U76] PHP：简单路由
来源：http://lyg.daria6918.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lre.fzhhl.top

[U77] PHP：模板渲染
来源：http://mhd.ybcxt.top

composer require twig/twig
来源：http://opv.sufxvd.cn

[U78] PHP：单元测试
来源：http://edx.sweek.top

composer require --dev phpunit/phpunit
来源：http://csm.yonumen.top

[U79] PHP：静态分析
来源：http://kqb.shanyushiyangtech.top

composer require --dev phpstan/phpstan
来源：http://uxg.vqdsnc.cn

[U80] PHP：代码规范修复
来源：http://txs.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hck.zdbjq.cn

[U81] JS：初始化项目
来源：http://ffo.shanyushiyangtech.top

npm init -y;  npm i express
来源：http://toj.hfpthk.cn

[U82] JS：package.json 脚本
来源：http://pgi.vqdsnc.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rhp.shuidangran.top

[U83] JS：ES Module 导入导出
来源：http://obg.hnxiangtu.top

export const a = 1;  import { a } from "./m.js";
来源：http://vfm.jinyuanbaomall.cn

[U84] JS：CommonJS 写法
来源：http://ltm.aibaodan.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uxu.zhiwuduotai.top

[U85] JS：可选链
来源：http://wad.redwolf501.top

a?.b?.c
来源：http://uca.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://llp.zhixingplan.top

a ?? b
来源：http://bme.zhijiandao.cn

[U87] JS：解构默认值
来源：http://ujo.cucudq.cn

const { a = 1, b = 2 } = obj;
来源：http://iyy.guowangkeji.top

[U88] JS：对象展开合并
来源：http://uwi.52xcode.cn

{ ...a, ...b }
来源：http://fyu.yueranfly.top

[U89] JS：数组去重
来源：http://knf.jinqigfzy.top

[...new Set(arr)]
来源：http://zyr.hnqzz.top

[U90] JS：数字数组排序
来源：http://bkj.fehbvm.com

[...arr].sort((a, b) => a - b)
来源：http://vez.hesvh.cn

[U91] JS：对象键值遍历
来源：http://fpa.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xkz.316326.xyz

[U92] JS：深拷贝
来源：http://rmz.chenzaomai.com

structuredClone(obj)
来源：http://qst.cheryme.top

[U93] JS：模板字符串
来源：http://ybl.jiagoushi.top

`共 ${n} 条`
来源：http://gys.bbcook.cn

[U94] JS：箭头函数
来源：http://dam.iojbl.cn

const double = x => x * 2;
来源：http://xes.dianchejie.cn

[U95] JS：Promise 包装
来源：http://zri.yfazqb.com

new Promise((resolve, reject) => {})
来源：http://dlp.daxiang520.top

[U96] JS：async/await 与异常
来源：http://jsf.mhx1999.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aty.wangdashe.top

[U97] JS：并发请求
来源：http://zya.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rsz.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://dme.aizwys.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://udw.guowangkeji.top

[U99] JS：事件监听
来源：http://urb.c1oappe.top

el.addEventListener("click", e => {})
来源：http://zcp.tianlin.xyz

[U100] JS：DOM 查询
来源：http://rzr.hnqzz.top

document.querySelector(".item")
来源：http://vka.sufxvd.cn

[U101] JS：classList 操作
来源：http://job.nanxuanxn.top

el.classList.toggle("active")
来源：http://uuu.gzhubu.top

[U102] JS：本地存储
来源：http://mov.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://vaa.xziqi.cn

[U103] JS：定时器
来源：http://miv.ydjk.org.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dct.ivvv.top

[U104] JS：防抖
来源：http://cxf.jlsjyb.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cca.vqdsnc.cn

[U105] JS：节流
来源：http://rlp.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://agw.yangfankeji.com

[U106] JS：日期格式化
来源：http://xcj.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://byx.shangyingyoupin.top

[U107] JS：数字千分位
来源：http://azg.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pxf.ehwqpu.com

[U108] JS：随机整数
来源：http://zcj.xziqi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://moz.hnqzz.top

[U109] JS：数组分组
来源：http://ytf.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://jft.zdqjudy.top

[U110] JS：数组分块
来源：http://yvt.tianlin.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wxv.9152youxi.cn

[U111] JS：对象转 Map
来源：http://wak.yongpay.top

new Map(Object.entries(obj))
来源：http://nmf.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://xff.jlsjyb.cn

"7".padStart(3, "0")
来源：http://kpc.yuanzhike.top

[U113] JS：正则替换全部
来源：http://cip.hesvh.cn

s.replaceAll("a", "b")
来源：http://sin.hywenlv.cn

[U114] JS：JSON 深比较
来源：http://pvc.hammf.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xnq.birdmap.top

[U115] JS：生成 UUID
来源：http://puz.zhengqikj.top

crypto.randomUUID()
来源：http://nqm.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://bdf.daria6918.cn

/** @param {string} name */ function f(name) {}
来源：http://vgc.fktsv.cn

[U117] JS：单元测试
来源：http://sqi.gzhubu.top

npm i -D vitest;  npx vitest
来源：http://yph.haohaochexian.top

[U118] JS：开发服务器
来源：http://dhd.jinyuanbaomall.cn

npm i -D vite;  npx vite
来源：http://yck.cashguo.top

[U119] JS：生产构建
来源：http://hsr.gotoacloud.top

npx vite build
来源：http://dug.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://bar.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://sgf.daria6918.cn

================================================================================
来源：http://mdv.cheryme.top

统计汇总
来源：http://csx.xinyue.icu

================================================================================
来源：http://umm.xylfe.cn

按语言统计（条）：
来源：http://bbh.ybcxt.top

Python ......... 252
来源：http://rbm.shangyingyoupin.top

PHP ............ 252
来源：http://qrm.shzxlz.cn

JavaScript ..... 252
来源：http://exy.ppjwa.cn

TypeScript ..... 212
来源：http://zdp.chenjidiqi.icu

Java ........... 212
来源：http://pdz.fzhhl.top

Go ............. 212
来源：http://nae.andypj.xyz

Ruby ........... 212
来源：http://qwm.sweek.top

C# ............. 212
来源：http://jrz.gogol.net.cn


<!-- 参考信息 -->