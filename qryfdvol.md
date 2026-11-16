代发 wailian999

[T41] Perl：Hello World
来源：http://nhy.cheryme.top

print "Hello\n";
来源：http://nxq.gzhubu.top

[T42] Perl：变量类型
来源：http://iqx.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jcs.zhengqikj.top

[T43] Perl：字符串插值
来源：http://muk.sxryk.cn

"值: $a"
来源：http://ced.jinyuanbaomall.cn

[T44] Perl：条件
来源：http://rix.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://tww.bbcook.cn

[T45] Perl：数组遍历
来源：http://zct.zhongyouzk.top

for my $x (@arr) { print $x; }
来源：http://dlg.gotoacloud.top

[T46] Perl：哈希操作
来源：http://xlt.yfazqb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jkt.yuxming.cn

[T47] Perl：正则捕获
来源：http://wgy.zhaomingkeji.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://xxv.vehdjk.com

[T48] Perl：正则替换
来源：http://qbb.ctjpmb.com

$s =~ s/old/new/g;
来源：http://qot.zhongyouzk.top

[T49] Perl：函数
来源：http://ayt.svipenyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vmm.zhijiandao.cn

[T50] Perl：逐行读文件
来源：http://suf.cucudq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://siw.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://kbu.nwbrower.top

[T51] Scala：Hello World
来源：http://buo.meibo888.top

println("Hello")
来源：http://mcu.yj20258888.top

[T52] Scala：变量
来源：http://blk.yuanzhike.top

val a = 1;  var b = 2
来源：http://cbz.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://ogg.zhongyouzk.top

s"值: $b"
来源：http://utf.nwbrower.top

[T54] Scala：集合映射
来源：http://jfx.daxiang520.top

List(1, 2, 3).map(_ * 2)
来源：http://asr.zhiwuduotai.top

[T55] Scala：集合过滤
来源：http://fgu.gotoacloud.top

List(1, 2, 3).filter(_ > 1)
来源：http://hrb.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://msq.yuxming.cn

case class User(name: String, age: Int)
来源：http://cik.pycfn.com

[T57] Scala：模式匹配
来源：http://pwt.zhiwuduotai.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ryp.vqdsnc.cn

[T58] Scala：函数定义
来源：http://bqs.svipenyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://txh.xylfe.cn

[T59] Scala：循环
来源：http://gfw.fktsv.cn

for (i <- 1 to 10) println(i)
来源：http://lrs.gzhubu.top

[T60] Scala：折叠
来源：http://jkq.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fvh.jinyuanbaomall.cn

================================================================================
来源：http://adu.xuanzx.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ibg.tanke756.top

================================================================================
来源：http://hji.guowangkeji.top

[U01] Py：创建虚拟环境
来源：http://ymw.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://jrd.vqdsnc.cn

[U02] Py：导出 / 安装依赖
来源：http://lgx.hesvh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sez.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://eol.jqgfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jur.gogol.net.cn

[U04] Py：变量调试打印
来源：http://ymo.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ayu.cucudq.cn

[U05] Py：列表去重且保序
来源：http://gwp.guannengcc.top

list(dict.fromkeys(arr))
来源：http://eax.shanyushiyangkeji.top

[U06] Py：合并两个字典
来源：http://eqj.jqgufenzy.top

{**a, **b}
来源：http://vts.cucudq.cn

[U07] Py：反转字典键值
来源：http://fia.dashuyun.cn

{v: k for k, v in d.items()}
来源：http://myl.yj20258888.top

[U08] Py：展平二维列表
来源：http://hxs.nanxuanxn.top

[y for x in nested for y in x]
来源：http://xet.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://qjx.zhongyouzk.top

max(d, key=d.get)
来源：http://snl.yuxming.cn

[U10] Py：按值排序字典
来源：http://ybc.xuanzx.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vhl.yangfankeji.com

[U11] Py：生成器表达式
来源：http://tvb.jinqigufen.top

(x * 2 for x in arr)
来源：http://uyb.jiagoushi.top

[U12] Py：取出现最多的 3 个元素
来源：http://xhb.vehdjk.com

Counter(arr).most_common(3)
来源：http://fyg.pengpengdd.cyou

[U13] Py：固定长度队列
来源：http://qxb.chenzaomai.com

deque(maxlen=10)
来源：http://ctm.daxiang520.top

[U14] Py：分组收集到列表
来源：http://iip.zdbjq.cn

defaultdict(list)
来源：http://qez.pengpengdd.cyou

[U15] Py：高精度计时
来源：http://iib.jinyuanbaomall.cn

t = time.perf_counter()
来源：http://ooi.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://wpl.sweek.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gry.cheryme.top

[U17] Py：初始化日志
来源：http://nbh.snrcjt.cn

logging.basicConfig(level=logging.INFO)
来源：http://ghh.fzhhl.top

[U18] Py：预编译正则
来源：http://uql.yongpay.top

pat = re.compile(r"\d+")
来源：http://phk.jqgufenzy.top

[U19] Py：正则替换带回调
来源：http://hym.ybcxt.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://poy.ybcxt.top

[U20] Py：缓存函数结果
来源：http://kdw.iojbl.cn

@functools.lru_cache(maxsize=None)
来源：http://amx.fktsv.cn

[U21] Py：自定义上下文管理器
来源：http://qpv.xylfe.cn

@contextlib.contextmanager
来源：http://byw.sweek.top

[U22] Py：矩阵转置
来源：http://onq.yj20258888.top

list(zip(*m))
来源：http://phh.nanxinkj.top

[U23] Py：分块读取大文件
来源：http://qxe.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jmb.wangshuangyany.cn

[U24] Py：路径操作
来源：http://jgh.gaohongyu789.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://omm.tian-w.cn

[U25] Py：CSV 按字典读
来源：http://utm.hfpthk.cn

csv.DictReader(f)
来源：http://saz.wangdashe.top

[U26] Py：并发下载
来源：http://wyr.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zky.nanxinkj.top

[U27] Py：异步 HTTP
来源：http://aha.yanxiufei.cn

aiohttp.ClientSession() 配合 async with
来源：http://fic.sysykeji.top

[U28] Py：类型别名
来源：http://fcr.dianchejie.cn

UserId = int
来源：http://gta.kuanghao11.cn

[U29] Py：属性校验
来源：http://xqj.hnxiangtu.top

@property 与 @x.setter 配合
来源：http://niw.shanyushiyangkeji.top

[U30] Py：数据类
来源：http://yty.hfpthk.cn

@dataclass(slots=True)
来源：http://xue.xingfuxueyuan.xyz

[U31] Py：单测
来源：http://odc.tian-w.cn

python -m pytest -q
来源：http://hem.tian-w.cn

[U32] Py：代码格式化
来源：http://xue.yj20258.top

ruff format . && ruff check --fix .
来源：http://glz.xinyue.icu

[U33] Py：打包发布
来源：http://rwu.c1oappe.top

python -m build  （依赖 pyproject.toml）
来源：http://gns.xingfuxueyuan.xyz

[U34] Py：判断编码
来源：http://cec.hammf.cn

chardet.detect(raw)
来源：http://qjk.zycfv.cn

[U35] Py：发送邮件
来源：http://lsa.fktsv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pal.jinghuilouyu.cn

[U36] Py：定时任务
来源：http://auc.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://tdp.dianchejie.cn

[U37] Py：读写 Excel
来源：http://gzs.xylfe.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iqh.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://pub.smart0.xyz

Path(__file__).resolve().parent
来源：http://bxc.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://kpo.yueranfly.top

sys.stdout.isatty()
来源：http://ajx.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://zwr.gogol.net.cn

print("err", file=sys.stderr)
来源：http://itv.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://ncj.fktsv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://srf.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://fgr.birdmap.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uhd.aibaodan.cn

[U43] PHP：声明命名空间
来源：http://wle.hnqzz.top

namespace App\Http;
来源：http://fzl.jlsjyb.cn

[U44] PHP：开启严格类型
来源：http://glj.daxiang520.top

declare(strict_types=1);
来源：http://obw.hysaishi.cn

[U45] PHP：类型声明与返回类型
来源：http://uuk.jianghu66.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kui.fktsv.cn

[U46] PHP：可空类型
来源：http://kdf.zhaomingkeji.xyz

?string $name = null
来源：http://rjz.xinyue.icu

[U47] PHP：联合类型
来源：http://xnh.hongshengwenyu.top

int|string $id
来源：http://qkw.ctjpmb.com

[U48] PHP：纯枚举
来源：http://gql.tarul.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xjk.guannengcc.top

[U49] PHP：只读属性
来源：http://lpv.jiagoushi.top

public readonly string $name
来源：http://sfy.xuanzx.com

[U50] PHP：构造器属性提升
来源：http://whd.hammf.cn

public function __construct(private int $id) {}
来源：http://jaf.cqqwz.cn

[U51] PHP：数组解构
来源：http://atx.yongpay.top

[$a, $b] = $arr;
来源：http://afs.cashguo.top

[U52] PHP：箭头函数
来源：http://mzz.jlsjyb.cn

$double = fn($x) => $x * 2;
来源：http://faz.yj20258.top

[U53] PHP：空合并运算符
来源：http://fqp.cashguo.top

$v = $a ?? $b ?? "default";
来源：http://zac.tarul.cn

[U54] PHP：空安全调用
来源：http://bjc.ehwqpu.com

$obj?->method()
来源：http://qib.sxryk.cn

[U55] PHP：match 表达式
来源：http://gne.aibaodan.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yqz.sxryk.cn

[U56] PHP：命名参数
来源：http://dnb.hfpthk.cn

f(a: 1, b: 2)
来源：http://rbs.c1oappe.top

[U57] PHP：字符串插值
来源：http://drn.yuxming.cn

"值: {$a}"
来源：http://ylk.zdqjudy.top

[U58] PHP：数组三件套
来源：http://osc.chenlongwang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uzb.gotoacloud.top

[U59] PHP：自定义排序
来源：http://fgc.fzhhl.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lko.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://lvj.jyoumei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rql.yuanzhike.top

[U61] PHP：正则
来源：http://xto.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gsv.hnqzz.top

[U62] PHP：日期对象
来源：http://dzq.zhoulong.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hna.hongshengwenyu.top

[U63] PHP：文件读写
来源：http://kdn.guowangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oua.chenzaomai.com

[U64] PHP：目录遍历
来源：http://hto.ctjpmb.com

glob("dir/*.php");  scandir("dir");
来源：http://cue.zycfv.cn

[U65] PHP：会话
来源：http://qio.jlsjyb.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gjd.chenzaomai.com

[U66] PHP：设置 Cookie
来源：http://feh.nwbrower.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qzi.sufxvd.cn

[U67] PHP：处理文件上传
来源：http://zuf.yanxiufei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://szt.jinghuilouyu.cn

[U68] PHP：PDO 连接
来源：http://atd.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wpg.sweek.top

[U69] PHP：PDO 预处理
来源：http://nry.yangfankeji.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kqq.tanke756.top

[U70] PHP：PDO 事务
来源：http://cpa.cqqwz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://urd.andypj.xyz

[U71] PHP：抛出异常
来源：http://msh.gzhubu.top

throw new RuntimeException("失败", 500);
来源：http://buk.epnwcf.com

[U72] PHP：写错误日志
来源：http://hxy.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://upl.0kj1m.cn

[U73] PHP：读取 ini 配置
来源：http://zup.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://qmh.dashuyun.cn

[U74] PHP：读取环境变量
来源：http://jth.pycfn.com

getenv("APP_ENV") ?: "production"
来源：http://bfr.uphjek.com

[U75] PHP：依赖注入
来源：http://tzr.wangdashe.top

composer require psr/container
来源：http://scj.shzxlz.cn

[U76] PHP：简单路由
来源：http://bre.fktsv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://plj.jlsjyb.cn

[U77] PHP：模板渲染
来源：http://ojm.uphjek.com

composer require twig/twig
来源：http://jbp.fengsongda.top

[U78] PHP：单元测试
来源：http://noa.svipenyu.cn

composer require --dev phpunit/phpunit
来源：http://igz.xziqi.cn

[U79] PHP：静态分析
来源：http://dfg.vqdsnc.cn

composer require --dev phpstan/phpstan
来源：http://psp.gzhubu.top

[U80] PHP：代码规范修复
来源：http://xei.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bbq.guannengcc.top

[U81] JS：初始化项目
来源：http://zei.hcnkem.com

npm init -y;  npm i express
来源：http://kao.ppjwa.cn

[U82] JS：package.json 脚本
来源：http://gab.9152youxi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qyp.chenlongwang.top

[U83] JS：ES Module 导入导出
来源：http://atu.havefunace.top

export const a = 1;  import { a } from "./m.js";
来源：http://nnr.jianghu66.top

[U84] JS：CommonJS 写法
来源：http://wot.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://ebg.jinqigfzy.top

[U85] JS：可选链
来源：http://hic.andypj.xyz

a?.b?.c
来源：http://yvo.iojbl.cn

[U86] JS：空值合并
来源：http://ral.cucudq.cn

a ?? b
来源：http://xos.jqgfzy.top

[U87] JS：解构默认值
来源：http://kxs.hywenlv.cn

const { a = 1, b = 2 } = obj;
来源：http://flm.cdnleiting.top

[U88] JS：对象展开合并
来源：http://zbm.yanxiufei.cn

{ ...a, ...b }
来源：http://tks.ivvv.top

[U89] JS：数组去重
来源：http://wub.yj20258888.top

[...new Set(arr)]
来源：http://vso.tianlin.xyz

[U90] JS：数字数组排序
来源：http://zrw.feifeiyinyue.top

[...arr].sort((a, b) => a - b)
来源：http://wiz.jyoumei.cn

[U91] JS：对象键值遍历
来源：http://aau.ivvv.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xxr.zhengqikj.top

[U92] JS：深拷贝
来源：http://ayx.tanke756.top

structuredClone(obj)
来源：http://jce.bjfxy.top

[U93] JS：模板字符串
来源：http://jff.cdnleiting.top

`共 ${n} 条`
来源：http://epg.cucudq.cn

[U94] JS：箭头函数
来源：http://web.smart0.xyz

const double = x => x * 2;
来源：http://qzl.sxryk.cn

[U95] JS：Promise 包装
来源：http://wcx.yanxiufei.cn

new Promise((resolve, reject) => {})
来源：http://eyv.meibo888.top

[U96] JS：async/await 与异常
来源：http://yhg.redwolf501.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://deh.svipenyu.cn

[U97] JS：并发请求
来源：http://dsa.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wik.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://lob.zhixingplan.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gel.xuanzx.com

[U99] JS：事件监听
来源：http://han.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://fgd.redwolf501.top

[U100] JS：DOM 查询
来源：http://zyl.jinyuanbaomall.cn

document.querySelector(".item")
来源：http://isp.sweek.top

[U101] JS：classList 操作
来源：http://mrv.jinqigufen.top

el.classList.toggle("active")
来源：http://xvb.zhoulong.xyz

[U102] JS：本地存储
来源：http://eqr.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://oyq.zhijiandao.cn

[U103] JS：定时器
来源：http://nqi.bbcook.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rny.svipenyu.cn

[U104] JS：防抖
来源：http://jak.xuanzx.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jeu.fengsongda.top

[U105] JS：节流
来源：http://pmf.shzxlz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dgx.0kj1m.cn

[U106] JS：日期格式化
来源：http://pct.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://muf.daria6918.cn

[U107] JS：数字千分位
来源：http://iby.fanxiaobao.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jty.hysaishi.cn

[U108] JS：随机整数
来源：http://pvc.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mbl.birdmap.top

[U109] JS：数组分组
来源：http://tlt.jinghuilouyu.cn

Object.groupBy(arr, x => x.type)
来源：http://vyb.316326.xyz

[U110] JS：数组分块
来源：http://oux.cqqwz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fhx.jiagoushi.top

[U111] JS：对象转 Map
来源：http://pqs.tian-w.cn

new Map(Object.entries(obj))
来源：http://zik.xuanzx.com

[U112] JS：字符串补位
来源：http://ylw.shangyingyoupin.top

"7".padStart(3, "0")
来源：http://xwy.hesvh.cn

[U113] JS：正则替换全部
来源：http://ilu.smart0.xyz

s.replaceAll("a", "b")
来源：http://hhf.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://iga.sufxvd.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://eig.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://sql.hywenlv.cn

crypto.randomUUID()
来源：http://nhh.yfazqb.com

[U116] JS：类型检查（JSDoc）
来源：http://etz.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://bom.hfpthk.cn

[U117] JS：单元测试
来源：http://vdh.smart0.xyz

npm i -D vitest;  npx vitest
来源：http://zuv.fengsongda.top

[U118] JS：开发服务器
来源：http://fny.sysykeji.top

npm i -D vite;  npx vite
来源：http://eot.cashguo.top

[U119] JS：生产构建
来源：http://nok.yj20258.top

npx vite build
来源：http://rni.yongpay.top

[U120] JS：读取环境变量（Vite）
来源：http://dth.nanxuanxn.top

import.meta.env.VITE_API_URL
来源：http://rgq.xingfuxueyuan.xyz

================================================================================
来源：http://moz.ivvv.top

统计汇总
来源：http://qvt.hnqzz.top

================================================================================
来源：http://hnm.ivvv.top

按语言统计（条）：
来源：http://edx.zhijiandao.cn

Python ......... 252
来源：http://ezc.hnqzz.top

PHP ............ 252
来源：http://exk.tarul.cn

JavaScript ..... 252
来源：http://ypz.snrcjt.cn

TypeScript ..... 212
来源：http://ala.tanke756.top

Java ........... 212
来源：http://rgt.guannengcc.top

Go ............. 212
来源：http://cyo.pengpengdd.cyou

Ruby ........... 212
来源：http://qky.yj20258888.top

C# ............. 212
来源：http://dao.ybcxt.top

C .............. 30
来源：http://yec.zhijiandao.cn

C++ ............ 30
来源：http://umr.0kj1m.cn

SQL ............ 90
来源：http://aug.fengsongda.top

Bash ........... 80
来源：http://mmu.jinyuanbaomall.cn


<!-- 参考信息 -->