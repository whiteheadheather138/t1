代发 wailian999

[T47] Perl：正则捕获
来源：http://ewd.pengpengdd.cyou

if ($s =~ /(\d+)/) { print $1; }
来源：http://lfq.shangyingyoupin.top

[T48] Perl：正则替换
来源：http://laa.cqqwz.cn

$s =~ s/old/new/g;
来源：http://mou.bbcook.cn

[T49] Perl：函数
来源：http://yeb.daria6918.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yci.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://lol.zhijiandao.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rwf.jqgufenzy.top

while (my $line = <$fh>) { print $line; }
来源：http://rkn.yj20258.top

[T51] Scala：Hello World
来源：http://exj.xziqi.cn

println("Hello")
来源：http://tzg.zhengqikj.top

[T52] Scala：变量
来源：http://luh.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://vao.jlsjyb.cn

[T53] Scala：字符串插值
来源：http://wzt.hywenlv.cn

s"值: $b"
来源：http://vra.ehwqpu.com

[T54] Scala：集合映射
来源：http://vjr.quarkkingdee.top

List(1, 2, 3).map(_ * 2)
来源：http://dyb.xylfe.cn

[T55] Scala：集合过滤
来源：http://dcb.redwolf501.top

List(1, 2, 3).filter(_ > 1)
来源：http://kkk.aizwys.cn

[T56] Scala：样例类
来源：http://ukj.jyoumei.cn

case class User(name: String, age: Int)
来源：http://rle.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://wpp.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ujl.svipenyu.cn

[T58] Scala：函数定义
来源：http://wad.cqqwz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iog.hongshengwenyu.top

[T59] Scala：循环
来源：http://pcc.tianlin.xyz

for (i <- 1 to 10) println(i)
来源：http://gwq.ydjk.org.cn

[T60] Scala：折叠
来源：http://prd.hcnkem.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cpl.guowangkeji.top

================================================================================
来源：http://mmq.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ukm.ehwqpu.com

================================================================================
来源：http://fqs.gotoacloud.top

[U01] Py：创建虚拟环境
来源：http://dvg.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nza.9152youxi.cn

[U02] Py：导出 / 安装依赖
来源：http://pdh.quarkkingdee.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vki.hcnkem.com

[U03] Py：加载 .env 配置
来源：http://vbp.chenjidiqi.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://est.tian-w.cn

[U04] Py：变量调试打印
来源：http://eka.sxryk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bwr.316326.xyz

[U05] Py：列表去重且保序
来源：http://drn.zdbjq.cn

list(dict.fromkeys(arr))
来源：http://ndj.cqqwz.cn

[U06] Py：合并两个字典
来源：http://gkh.jiagoushi.top

{**a, **b}
来源：http://hyu.epnwcf.com

[U07] Py：反转字典键值
来源：http://rzr.meibo888.top

{v: k for k, v in d.items()}
来源：http://uax.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://fqm.pengpengdd.cyou

[y for x in nested for y in x]
来源：http://smw.quarkkingdee.top

[U09] Py：字典取最大值的键
来源：http://dfc.smart0.xyz

max(d, key=d.get)
来源：http://ziy.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://gei.ydzc1.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aeo.shanyushiyangkeji.top

[U11] Py：生成器表达式
来源：http://piz.yangfankeji.com

(x * 2 for x in arr)
来源：http://ojo.316326.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://grr.dashuyun.cn

Counter(arr).most_common(3)
来源：http://vxe.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://uep.cucudq.cn

deque(maxlen=10)
来源：http://uzi.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://vho.zdbjq.cn

defaultdict(list)
来源：http://exj.fengsongda.top

[U15] Py：高精度计时
来源：http://sah.yj20258888.top

t = time.perf_counter()
来源：http://sna.sysykeji.top

[U16] Py：命令行参数解析
来源：http://ztn.ydzc1.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://esi.haohaochexian.top

[U17] Py：初始化日志
来源：http://pom.zycfv.cn

logging.basicConfig(level=logging.INFO)
来源：http://kfp.chenzaomai.com

[U18] Py：预编译正则
来源：http://ucd.ehwqpu.com

pat = re.compile(r"\d+")
来源：http://qoq.yanxiufei.cn

[U19] Py：正则替换带回调
来源：http://tmj.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fhc.yanxiufei.cn

[U20] Py：缓存函数结果
来源：http://dlj.ehwqpu.com

@functools.lru_cache(maxsize=None)
来源：http://stm.fanxiaobao.xyz

[U21] Py：自定义上下文管理器
来源：http://iia.52xcode.cn

@contextlib.contextmanager
来源：http://eeb.jianghu66.top

[U22] Py：矩阵转置
来源：http://drw.vqdsnc.cn

list(zip(*m))
来源：http://rxo.fktsv.cn

[U23] Py：分块读取大文件
来源：http://pdl.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vrz.yangfankeji.com

[U24] Py：路径操作
来源：http://ukl.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rja.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://qwe.jinghuilouyu.cn

csv.DictReader(f)
来源：http://cis.hongshengwenyu.top

[U26] Py：并发下载
来源：http://fyq.wangdashe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://isl.tanke756.top

[U27] Py：异步 HTTP
来源：http://iym.hammf.cn

aiohttp.ClientSession() 配合 async with
来源：http://bqo.ydjk.org.cn

[U28] Py：类型别名
来源：http://klr.wangdashe.top

UserId = int
来源：http://ewq.yongpay.top

[U29] Py：属性校验
来源：http://lck.sxryk.cn

@property 与 @x.setter 配合
来源：http://ovk.zhixingplan.top

[U30] Py：数据类
来源：http://sgz.yfazqb.com

@dataclass(slots=True)
来源：http://lye.cqqwz.cn

[U31] Py：单测
来源：http://ory.sjlbkw.cn

python -m pytest -q
来源：http://jfm.nanxuanxn.top

[U32] Py：代码格式化
来源：http://xie.epnwcf.com

ruff format . && ruff check --fix .
来源：http://rkd.wangdashe.top

[U33] Py：打包发布
来源：http://clk.yuxming.cn

python -m build  （依赖 pyproject.toml）
来源：http://wwg.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://eio.hongshengwenyu.top

chardet.detect(raw)
来源：http://wko.jyoumei.cn

[U35] Py：发送邮件
来源：http://rab.gogol.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ort.sufxvd.cn

[U36] Py：定时任务
来源：http://gki.cheryme.top

schedule.every(10).minutes.do(job)
来源：http://vdi.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://dsv.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nly.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://yje.dianchejie.cn

Path(__file__).resolve().parent
来源：http://bns.bjfxy.top

[U39] Py：判断是否在交互环境
来源：http://qsy.shangyingyoupin.top

sys.stdout.isatty()
来源：http://asc.9152youxi.cn

[U40] Py：打印到标准错误
来源：http://kgt.yueranfly.top

print("err", file=sys.stderr)
来源：http://lpx.sweek.top

[U41] PHP：初始化 Composer 项目
来源：http://osd.zhixingplan.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qfm.sufxvd.cn

[U42] PHP：PSR-4 自动加载
来源：http://urb.gzhubu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zci.hesvh.cn

[U43] PHP：声明命名空间
来源：http://hdz.zhijiandao.cn

namespace App\Http;
来源：http://opr.bbcook.cn

[U44] PHP：开启严格类型
来源：http://qsx.yanxiufei.cn

declare(strict_types=1);
来源：http://rjl.jqgfzy.top

[U45] PHP：类型声明与返回类型
来源：http://hvo.ywan-chungtsiang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ihf.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://dsr.sjlbkw.cn

?string $name = null
来源：http://ted.chenjidiqi.icu

[U47] PHP：联合类型
来源：http://vjx.guannengcc.top

int|string $id
来源：http://jgl.cheryme.top

[U48] PHP：纯枚举
来源：http://bas.hfpthk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gdp.sjlbkw.cn

[U49] PHP：只读属性
来源：http://ybj.haohaochexian.top

public readonly string $name
来源：http://dhf.yfazqb.com

[U50] PHP：构造器属性提升
来源：http://hxj.fehbvm.com

public function __construct(private int $id) {}
来源：http://nai.zhijiandao.cn

[U51] PHP：数组解构
来源：http://ttk.cheryme.top

[$a, $b] = $arr;
来源：http://kad.xylfe.cn

[U52] PHP：箭头函数
来源：http://jtx.zhijiandao.cn

$double = fn($x) => $x * 2;
来源：http://hci.cashguo.top

[U53] PHP：空合并运算符
来源：http://hsv.jyoumei.cn

$v = $a ?? $b ?? "default";
来源：http://thr.feifeiyinyue.top

[U54] PHP：空安全调用
来源：http://jow.yuxming.cn

$obj?->method()
来源：http://wcj.xziqi.cn

[U55] PHP：match 表达式
来源：http://zsl.zhixingplan.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cgg.jiagoushi.top

[U56] PHP：命名参数
来源：http://nnm.hcnkem.com

f(a: 1, b: 2)
来源：http://dbs.zhaomingkeji.xyz

[U57] PHP：字符串插值
来源：http://yxr.snrcjt.cn

"值: {$a}"
来源：http://ieb.jinghuilouyu.cn

[U58] PHP：数组三件套
来源：http://ueu.mhx1999.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lkc.yj20258888.top

[U59] PHP：自定义排序
来源：http://ywn.gotoacloud.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ens.yangfankeji.com

[U60] PHP：JSON 编解码
来源：http://noq.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nut.birdmap.top

[U61] PHP：正则
来源：http://lrf.sjlbkw.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kjx.jqgufenzy.top

[U62] PHP：日期对象
来源：http://lns.hnxiangtu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://grs.yvedp.cn

[U63] PHP：文件读写
来源：http://gsk.shanyushiyangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vrz.jyoumei.cn

[U64] PHP：目录遍历
来源：http://hif.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://smy.jinqigfzy.top

[U65] PHP：会话
来源：http://ush.haohaochexian.top

session_start();  $_SESSION["uid"] = 1;
来源：http://evy.316326.xyz

[U66] PHP：设置 Cookie
来源：http://mrr.ehwqpu.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hby.iojbl.cn

[U67] PHP：处理文件上传
来源：http://rbi.yfazqb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://osf.316326.xyz

[U68] PHP：PDO 连接
来源：http://eka.aizwys.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gbg.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://udj.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aof.nanxinkj.top

[U70] PHP：PDO 事务
来源：http://ffm.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ybm.zhijiandao.cn

[U71] PHP：抛出异常
来源：http://hsh.epnwcf.com

throw new RuntimeException("失败", 500);
来源：http://sce.yj202588.top

[U72] PHP：写错误日志
来源：http://kfx.ydjk.org.cn

error_log("失败: " . $e->getMessage());
来源：http://vle.zdqjudy.top

[U73] PHP：读取 ini 配置
来源：http://cul.snrcjt.cn

parse_ini_file("config.ini", true)
来源：http://rxi.52xcode.cn

[U74] PHP：读取环境变量
来源：http://egy.c1oappe.top

getenv("APP_ENV") ?: "production"
来源：http://xdg.tianlin.xyz

[U75] PHP：依赖注入
来源：http://gbq.ivvv.top

composer require psr/container
来源：http://otd.shanyushiyangkeji.top

[U76] PHP：简单路由
来源：http://yfk.guannengcc.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uka.yuanzhike.top

[U77] PHP：模板渲染
来源：http://hyn.fanxiaobao.xyz

composer require twig/twig
来源：http://qyc.jinyuanbaomall.cn

[U78] PHP：单元测试
来源：http://vml.zhiwuduotai.top

composer require --dev phpunit/phpunit
来源：http://pep.zdbjq.cn

[U79] PHP：静态分析
来源：http://vjn.yj20258888.top

composer require --dev phpstan/phpstan
来源：http://req.sjlbkw.cn

[U80] PHP：代码规范修复
来源：http://she.zhongyouzk.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://grp.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://ppa.nanxuanxn.top

npm init -y;  npm i express
来源：http://yhu.sweek.top

[U82] JS：package.json 脚本
来源：http://ruq.hnxiangtu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rda.kuanghao11.cn

[U83] JS：ES Module 导入导出
来源：http://krm.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://xhj.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://vuy.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://apw.uphjek.com

[U85] JS：可选链
来源：http://hhm.xziqi.cn

a?.b?.c
来源：http://qyz.zycfv.cn

[U86] JS：空值合并
来源：http://wjy.tian-w.cn

a ?? b
来源：http://whv.havefunace.top

[U87] JS：解构默认值
来源：http://pdx.havefunace.top

const { a = 1, b = 2 } = obj;
来源：http://idz.dianchejie.cn

[U88] JS：对象展开合并
来源：http://uxj.redwolf501.top

{ ...a, ...b }
来源：http://zfr.feifeiyinyue.top

[U89] JS：数组去重
来源：http://mdw.0kj1m.cn

[...new Set(arr)]
来源：http://xcc.guowangkeji.top

[U90] JS：数字数组排序
来源：http://skq.jiagoushi.top

[...arr].sort((a, b) => a - b)
来源：http://ajf.fktsv.cn

[U91] JS：对象键值遍历
来源：http://jvt.jiagoushi.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qas.iojbl.cn

[U92] JS：深拷贝
来源：http://lqy.feifeiyinyue.top

structuredClone(obj)
来源：http://ksa.vqdsnc.cn

[U93] JS：模板字符串
来源：http://smm.jinyuanbaomall.cn

`共 ${n} 条`
来源：http://bkg.bbcook.cn

[U94] JS：箭头函数
来源：http://yxo.zhixingplan.top

const double = x => x * 2;
来源：http://tfe.birdmap.top

[U95] JS：Promise 包装
来源：http://jbf.gzhubu.top

new Promise((resolve, reject) => {})
来源：http://ynv.hysaishi.cn

[U96] JS：async/await 与异常
来源：http://bso.nwbrower.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://khv.yonumen.top

[U97] JS：并发请求
来源：http://keh.tanke756.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://utw.zhaomingkeji.xyz

[U98] JS：fetch 带 JSON
来源：http://dah.shangyingyoupin.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jow.havefunace.top

[U99] JS：事件监听
来源：http://lbe.xylfe.cn

el.addEventListener("click", e => {})
来源：http://yyx.snrcjt.cn

[U100] JS：DOM 查询
来源：http://fzo.316326.xyz

document.querySelector(".item")
来源：http://wbj.xuanzx.com

[U101] JS：classList 操作
来源：http://und.yuxming.cn

el.classList.toggle("active")
来源：http://mze.jinqigfzy.top

[U102] JS：本地存储
来源：http://irv.shanyushiyangtech.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xme.smart0.xyz

[U103] JS：定时器
来源：http://xlf.bjfxy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hfn.52xcode.cn

[U104] JS：防抖
来源：http://xxv.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eds.ppjwa.cn

[U105] JS：节流
来源：http://phm.fengsongda.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gvb.zhiwuduotai.top

[U106] JS：日期格式化
来源：http://tks.nanxuanxn.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cmt.fzhhl.top

[U107] JS：数字千分位
来源：http://wio.sweek.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://viu.vehdjk.com

[U108] JS：随机整数
来源：http://yjo.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yjk.yj20258888.top

[U109] JS：数组分组
来源：http://nee.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://hgn.yj202588.top

[U110] JS：数组分块
来源：http://cxd.epnwcf.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://azt.xylfe.cn

[U111] JS：对象转 Map
来源：http://tcp.yj20258888.top

new Map(Object.entries(obj))
来源：http://oao.zhijiandao.cn

[U112] JS：字符串补位
来源：http://iyx.haohaochexian.top

"7".padStart(3, "0")
来源：http://hud.snrcjt.cn

[U113] JS：正则替换全部
来源：http://qhu.mhx1999.top

s.replaceAll("a", "b")
来源：http://sag.fktsv.cn

[U114] JS：JSON 深比较
来源：http://tjw.gotoacloud.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xpa.yfazqb.com

[U115] JS：生成 UUID
来源：http://frk.daxiang520.top

crypto.randomUUID()
来源：http://qpe.hongshengwenyu.top

[U116] JS：类型检查（JSDoc）
来源：http://jvj.xingfuxueyuan.xyz

/** @param {string} name */ function f(name) {}
来源：http://yqx.pycfn.com

[U117] JS：单元测试
来源：http://ads.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://hsn.pengpengdd.cyou

[U118] JS：开发服务器
来源：http://rtk.yj202588.top

npm i -D vite;  npx vite
来源：http://pzb.zdbjq.cn

[U119] JS：生产构建
来源：http://gve.chenjidiqi.icu

npx vite build
来源：http://esv.hesvh.cn

[U120] JS：读取环境变量（Vite）
来源：http://vuv.yj20258.top

import.meta.env.VITE_API_URL
来源：http://nhg.sysykeji.top

================================================================================
来源：http://sts.ivvv.top

统计汇总
来源：http://gxn.chenjidiqi.icu

================================================================================
来源：http://yrr.ivvv.top

按语言统计（条）：
来源：http://qkz.shuidangran.top

Python ......... 252
来源：http://txr.iojbl.cn

PHP ............ 252
来源：http://yxg.zhijiandao.cn

JavaScript ..... 252
来源：http://hcs.zdqjudy.top

TypeScript ..... 212
来源：http://hui.shanyushiyangkeji.top

Java ........... 212
来源：http://cow.cucudq.cn

Go ............. 212
来源：http://kta.meibo888.top

Ruby ........... 212
来源：http://ffn.xylfe.cn

C# ............. 212
来源：http://gql.uphjek.com

C .............. 30
来源：http://cku.zhiwuduotai.top

C++ ............ 30
来源：http://vcv.ybcxt.top

SQL ............ 90
来源：http://zhu.jinyuanbaomall.cn

Bash ........... 80
来源：http://dvy.yj202588.top

Kotlin ......... 15
来源：http://plb.daxiang520.top

Swift .......... 15
来源：http://vah.tanke756.top

Lua ............ 10
来源：http://eap.xuanzx.com

Perl ........... 10
来源：http://plu.zhoulong.xyz

Scala .......... 10
来源：http://gxr.vqdsnc.cn

------------------------------------
来源：http://wwo.sxryk.cn

合计 ........... 2106 条
来源：http://nbf.0kj1m.cn

按章节统计：
来源：http://gej.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hgl.sufxvd.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cwq.ywan-chungtsiang.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cpk.wangshuangyany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hbk.zdbjq.cn


<!-- 参考信息 -->