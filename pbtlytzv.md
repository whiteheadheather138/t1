代发 wailian999

[T47] Perl：正则捕获
来源：http://vfc.zhaomingkeji.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://kmm.yj20258.top

[T48] Perl：正则替换
来源：http://qxw.fanxiaobao.xyz

$s =~ s/old/new/g;
来源：http://kxt.xziqi.cn

[T49] Perl：函数
来源：http://kyq.tian-w.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wng.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://bsj.ctjpmb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://vik.sweek.top

while (my $line = <$fh>) { print $line; }
来源：http://ovo.hesvh.cn

[T51] Scala：Hello World
来源：http://hqa.ydzc1.top

println("Hello")
来源：http://quq.316326.xyz

[T52] Scala：变量
来源：http://jsf.hywenlv.cn

val a = 1;  var b = 2
来源：http://gep.zhongyouzk.top

[T53] Scala：字符串插值
来源：http://zqo.hywenlv.cn

s"值: $b"
来源：http://poo.yuanzhike.top

[T54] Scala：集合映射
来源：http://mcu.jlsjyb.cn

List(1, 2, 3).map(_ * 2)
来源：http://ykl.feifeiyinyue.top

[T55] Scala：集合过滤
来源：http://btk.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zxk.chenjidiqi.icu

[T56] Scala：样例类
来源：http://ets.svipenyu.cn

case class User(name: String, age: Int)
来源：http://cnu.haohaochexian.top

[T57] Scala：模式匹配
来源：http://lkj.bbcook.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://aaq.sufxvd.cn

[T58] Scala：函数定义
来源：http://caq.vqdsnc.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zjx.yfazqb.com

[T59] Scala：循环
来源：http://pkk.ybcxt.top

for (i <- 1 to 10) println(i)
来源：http://ljp.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://pwe.52xcode.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wxq.chenlongwang.top

================================================================================
来源：http://qet.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wxk.chenlongwang.top

================================================================================
来源：http://hvi.havefunace.top

[U01] Py：创建虚拟环境
来源：http://lzj.zhixingplan.top

python -m venv .venv && source .venv/bin/activate
来源：http://abl.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://xsv.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://odh.hnxiangtu.top

[U03] Py：加载 .env 配置
来源：http://msf.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://aaz.redwolf501.top

[U04] Py：变量调试打印
来源：http://kst.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://big.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://syd.tianlin.xyz

list(dict.fromkeys(arr))
来源：http://ike.xuanzx.com

[U06] Py：合并两个字典
来源：http://iml.tanke756.top

{**a, **b}
来源：http://cyr.xinyue.icu

[U07] Py：反转字典键值
来源：http://jcw.jinghuilouyu.cn

{v: k for k, v in d.items()}
来源：http://sik.smart0.xyz

[U08] Py：展平二维列表
来源：http://lgy.sjlbkw.cn

[y for x in nested for y in x]
来源：http://mmz.cashguo.top

[U09] Py：字典取最大值的键
来源：http://xbb.jinghuilouyu.cn

max(d, key=d.get)
来源：http://yec.vqdsnc.cn

[U10] Py：按值排序字典
来源：http://hqe.fktsv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sxt.aibaodan.cn

[U11] Py：生成器表达式
来源：http://xqg.svipenyu.cn

(x * 2 for x in arr)
来源：http://gvh.ydzc1.top

[U12] Py：取出现最多的 3 个元素
来源：http://nme.zhixingplan.top

Counter(arr).most_common(3)
来源：http://qod.hnxiangtu.top

[U13] Py：固定长度队列
来源：http://nyg.xinyue.icu

deque(maxlen=10)
来源：http://sop.wangshuangyany.cn

[U14] Py：分组收集到列表
来源：http://pgc.fengsongda.top

defaultdict(list)
来源：http://wee.gogol.net.cn

[U15] Py：高精度计时
来源：http://xtf.shangyingyoupin.top

t = time.perf_counter()
来源：http://kma.yvedp.cn

[U16] Py：命令行参数解析
来源：http://nbs.9152youxi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dhr.yfazqb.com

[U17] Py：初始化日志
来源：http://cjh.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://lul.snrcjt.cn

[U18] Py：预编译正则
来源：http://vqs.hysaishi.cn

pat = re.compile(r"\d+")
来源：http://uxv.yuxming.cn

[U19] Py：正则替换带回调
来源：http://agh.zhiwuduotai.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hdr.tian-w.cn

[U20] Py：缓存函数结果
来源：http://kso.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://dug.52xcode.cn

[U21] Py：自定义上下文管理器
来源：http://wvz.sufxvd.cn

@contextlib.contextmanager
来源：http://ifu.jiagoushi.top

[U22] Py：矩阵转置
来源：http://idm.haohaochexian.top

list(zip(*m))
来源：http://cut.sufxvd.cn

[U23] Py：分块读取大文件
来源：http://bdk.xuanzx.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lng.nwbrower.top

[U24] Py：路径操作
来源：http://emz.yj202588.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nuq.mhx1999.top

[U25] Py：CSV 按字典读
来源：http://dhs.redwolf501.top

csv.DictReader(f)
来源：http://imv.redwolf501.top

[U26] Py：并发下载
来源：http://boo.iojbl.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ucd.hongshengwenyu.top

[U27] Py：异步 HTTP
来源：http://oiv.jiagoushi.top

aiohttp.ClientSession() 配合 async with
来源：http://dpn.sxryk.cn

[U28] Py：类型别名
来源：http://qnu.nanxinkj.top

UserId = int
来源：http://fkz.tanke756.top

[U29] Py：属性校验
来源：http://ryv.jiagoushi.top

@property 与 @x.setter 配合
来源：http://map.tian-w.cn

[U30] Py：数据类
来源：http://rml.jinqigfzy.top

@dataclass(slots=True)
来源：http://baa.fzhhl.top

[U31] Py：单测
来源：http://tek.xinyue.icu

python -m pytest -q
来源：http://asp.sufxvd.cn

[U32] Py：代码格式化
来源：http://mbn.iojbl.cn

ruff format . && ruff check --fix .
来源：http://nfi.zhaomingkeji.xyz

[U33] Py：打包发布
来源：http://tuv.tianlin.xyz

python -m build  （依赖 pyproject.toml）
来源：http://nvc.jqgufenzy.top

[U34] Py：判断编码
来源：http://ano.zhongyouzk.top

chardet.detect(raw)
来源：http://mbx.yanxiufei.cn

[U35] Py：发送邮件
来源：http://iut.ctjpmb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://czy.zhiwuduotai.top

[U36] Py：定时任务
来源：http://jvh.daxiang520.top

schedule.every(10).minutes.do(job)
来源：http://qer.gotoacloud.top

[U37] Py：读写 Excel
来源：http://ltf.hywenlv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wkt.guannengcc.top

[U38] Py：获取脚本所在目录
来源：http://pcv.gaohongyu789.top

Path(__file__).resolve().parent
来源：http://uux.guannengcc.top

[U39] Py：判断是否在交互环境
来源：http://pio.sjlbkw.cn

sys.stdout.isatty()
来源：http://fop.zycfv.cn

[U40] Py：打印到标准错误
来源：http://bie.chenzaomai.com

print("err", file=sys.stderr)
来源：http://puq.fktsv.cn

[U41] PHP：初始化 Composer 项目
来源：http://epm.xingfuxueyuan.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://pov.9152youxi.cn

[U42] PHP：PSR-4 自动加载
来源：http://awv.xuetiantiany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ubs.uphjek.com

[U43] PHP：声明命名空间
来源：http://vch.jiagoushi.top

namespace App\Http;
来源：http://hvz.yanxiufei.cn

[U44] PHP：开启严格类型
来源：http://lxw.zdbjq.cn

declare(strict_types=1);
来源：http://cbi.zhoulong.xyz

[U45] PHP：类型声明与返回类型
来源：http://mvc.vehdjk.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://ckg.chenzaomai.com

[U46] PHP：可空类型
来源：http://hms.kuanghao11.cn

?string $name = null
来源：http://kbm.gzhubu.top

[U47] PHP：联合类型
来源：http://akh.ydzc1.top

int|string $id
来源：http://avm.jinqigfzy.top

[U48] PHP：纯枚举
来源：http://ixj.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fuf.haohaochexian.top

[U49] PHP：只读属性
来源：http://gbw.shanyushiyangkeji.top

public readonly string $name
来源：http://elc.havefunace.top

[U50] PHP：构造器属性提升
来源：http://lxn.yj20258888.top

public function __construct(private int $id) {}
来源：http://jqi.ctjpmb.com

[U51] PHP：数组解构
来源：http://tbk.fanxiaobao.xyz

[$a, $b] = $arr;
来源：http://mkh.ctjpmb.com

[U52] PHP：箭头函数
来源：http://ffw.ehwqpu.com

$double = fn($x) => $x * 2;
来源：http://sag.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://qna.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://ctl.sweek.top

[U54] PHP：空安全调用
来源：http://wlt.gogol.net.cn

$obj?->method()
来源：http://fuf.wangdashe.top

[U55] PHP：match 表达式
来源：http://mnz.zhijiandao.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zni.jinyuanbaomall.cn

[U56] PHP：命名参数
来源：http://lpb.hysaishi.cn

f(a: 1, b: 2)
来源：http://nbi.shanyushiyangkeji.top

[U57] PHP：字符串插值
来源：http://vrk.havefunace.top

"值: {$a}"
来源：http://tfn.daria6918.cn

[U58] PHP：数组三件套
来源：http://edc.wangshuangyany.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xrx.gogol.net.cn

[U59] PHP：自定义排序
来源：http://cst.ydjk.org.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rfc.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://iou.xylfe.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nvl.hongshengwenyu.top

[U61] PHP：正则
来源：http://uec.chenjidiqi.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mbg.bjfxy.top

[U62] PHP：日期对象
来源：http://fvx.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://idd.jinghuilouyu.cn

[U63] PHP：文件读写
来源：http://yde.shanyushiyangtech.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vxg.vqdsnc.cn

[U64] PHP：目录遍历
来源：http://bkr.fktsv.cn

glob("dir/*.php");  scandir("dir");
来源：http://uio.chenlongwang.top

[U65] PHP：会话
来源：http://mzx.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://nom.tianlin.xyz

[U66] PHP：设置 Cookie
来源：http://qeu.yj202588.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vdq.cucudq.cn

[U67] PHP：处理文件上传
来源：http://ttt.cashguo.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jmf.hnqzz.top

[U68] PHP：PDO 连接
来源：http://ajj.zdbjq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rft.svipenyu.cn

[U69] PHP：PDO 预处理
来源：http://jqk.yj20258.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lov.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://caa.yanxiufei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zis.jiagoushi.top

[U71] PHP：抛出异常
来源：http://pjc.hnqzz.top

throw new RuntimeException("失败", 500);
来源：http://gwp.cheryme.top

[U72] PHP：写错误日志
来源：http://bif.mhx1999.top

error_log("失败: " . $e->getMessage());
来源：http://eol.meibo888.top

[U73] PHP：读取 ini 配置
来源：http://eps.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://idc.9152youxi.cn

[U74] PHP：读取环境变量
来源：http://rgk.smart0.xyz

getenv("APP_ENV") ?: "production"
来源：http://qnj.gotoacloud.top

[U75] PHP：依赖注入
来源：http://ekk.bbcook.cn

composer require psr/container
来源：http://zvz.gotoacloud.top

[U76] PHP：简单路由
来源：http://vvh.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gju.bjfxy.top

[U77] PHP：模板渲染
来源：http://ngc.fanxiaobao.xyz

composer require twig/twig
来源：http://nhy.316326.xyz

[U78] PHP：单元测试
来源：http://ekf.zdbjq.cn

composer require --dev phpunit/phpunit
来源：http://dxb.havefunace.top

[U79] PHP：静态分析
来源：http://kfq.hammf.cn

composer require --dev phpstan/phpstan
来源：http://vcr.nanxuanxn.top

[U80] PHP：代码规范修复
来源：http://spp.meibo888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ulh.yanxiufei.cn

[U81] JS：初始化项目
来源：http://wsg.cheryme.top

npm init -y;  npm i express
来源：http://kxg.feifeiyinyue.top

[U82] JS：package.json 脚本
来源：http://jql.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jjc.ydzc1.top

[U83] JS：ES Module 导入导出
来源：http://vfg.tianlin.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://ibs.pengpengdd.cyou

[U84] JS：CommonJS 写法
来源：http://lxn.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://wkp.tianlin.xyz

[U85] JS：可选链
来源：http://oie.jiagoushi.top

a?.b?.c
来源：http://ddh.ehwqpu.com

[U86] JS：空值合并
来源：http://knn.aizwys.cn

a ?? b
来源：http://qph.sufxvd.cn

[U87] JS：解构默认值
来源：http://lhq.fktsv.cn

const { a = 1, b = 2 } = obj;
来源：http://mly.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://uoe.jinqigufen.top

{ ...a, ...b }
来源：http://zgx.hfpthk.cn

[U89] JS：数组去重
来源：http://fde.xuanzx.com

[...new Set(arr)]
来源：http://qye.cdnleiting.top

[U90] JS：数字数组排序
来源：http://pxg.cdnleiting.top

[...arr].sort((a, b) => a - b)
来源：http://feh.zycfv.cn

[U91] JS：对象键值遍历
来源：http://ftm.guowangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ell.cashguo.top

[U92] JS：深拷贝
来源：http://lgs.52xcode.cn

structuredClone(obj)
来源：http://zhc.hywenlv.cn

[U93] JS：模板字符串
来源：http://xus.daria6918.cn

`共 ${n} 条`
来源：http://byt.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://utb.nanxinkj.top

const double = x => x * 2;
来源：http://zgo.guowangkeji.top

[U95] JS：Promise 包装
来源：http://mmx.chenlongwang.top

new Promise((resolve, reject) => {})
来源：http://hbo.jqgufenzy.top

[U96] JS：async/await 与异常
来源：http://jif.xuanzx.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ucn.tian-w.cn

[U97] JS：并发请求
来源：http://xhf.xingfuxueyuan.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://xka.xziqi.cn

[U98] JS：fetch 带 JSON
来源：http://hcp.svipenyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kjq.hammf.cn

[U99] JS：事件监听
来源：http://aqs.zhiwuduotai.top

el.addEventListener("click", e => {})
来源：http://hxr.iojbl.cn

[U100] JS：DOM 查询
来源：http://haa.tanke756.top

document.querySelector(".item")
来源：http://iub.hcnkem.com

[U101] JS：classList 操作
来源：http://hjj.cdnleiting.top

el.classList.toggle("active")
来源：http://yws.mhx1999.top

[U102] JS：本地存储
来源：http://imb.cdnleiting.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cnr.chenjidiqi.icu

[U103] JS：定时器
来源：http://cgi.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ldo.gotoacloud.top

[U104] JS：防抖
来源：http://eet.zycfv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gpn.shanyushiyangkeji.top

[U105] JS：节流
来源：http://vcs.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mee.gzhubu.top

[U106] JS：日期格式化
来源：http://raf.xuanzx.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vul.sjlbkw.cn

[U107] JS：数字千分位
来源：http://yrz.chenzaomai.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qmy.52xcode.cn

[U108] JS：随机整数
来源：http://epy.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hqp.kuanghao11.cn

[U109] JS：数组分组
来源：http://kzt.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://ish.yj202588.top

[U110] JS：数组分块
来源：http://lwt.shangyingyoupin.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://moq.bbcook.cn

[U111] JS：对象转 Map
来源：http://bjr.smart0.xyz

new Map(Object.entries(obj))
来源：http://wzb.jinghuilouyu.cn

[U112] JS：字符串补位
来源：http://yei.hongshengwenyu.top

"7".padStart(3, "0")
来源：http://xol.guowangkeji.top

[U113] JS：正则替换全部
来源：http://qaj.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://njc.aibaodan.cn

[U114] JS：JSON 深比较
来源：http://vil.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://bsz.epnwcf.com

[U115] JS：生成 UUID
来源：http://xeo.birdmap.top

crypto.randomUUID()
来源：http://qhk.yj20258888.top

[U116] JS：类型检查（JSDoc）
来源：http://mzp.0kj1m.cn

/** @param {string} name */ function f(name) {}
来源：http://zrd.jiagoushi.top

[U117] JS：单元测试
来源：http://ncf.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://kpz.bjfxy.top

[U118] JS：开发服务器
来源：http://dor.dashuyun.cn

npm i -D vite;  npx vite
来源：http://vxm.meibo888.top

[U119] JS：生产构建
来源：http://xuj.jiagoushi.top

npx vite build
来源：http://noi.yanxiufei.cn

[U120] JS：读取环境变量（Vite）
来源：http://dlz.jqgufenzy.top

import.meta.env.VITE_API_URL
来源：http://kkb.yuxming.cn

================================================================================
来源：http://cat.tianlin.xyz

统计汇总
来源：http://ckc.fktsv.cn

================================================================================
来源：http://osj.zhiwuduotai.top

按语言统计（条）：
来源：http://mjm.zhiwuduotai.top

Python ......... 252
来源：http://xtz.havefunace.top

PHP ............ 252
来源：http://bzn.andypj.xyz

JavaScript ..... 252
来源：http://tzl.gogol.net.cn

TypeScript ..... 212
来源：http://jkp.wangdashe.top

Java ........... 212
来源：http://nip.hnqzz.top

Go ............. 212
来源：http://hbn.ydzc1.top

Ruby ........... 212
来源：http://upx.yj202588.top

C# ............. 212
来源：http://gqa.yanxiufei.cn

C .............. 30
来源：http://zfk.tian-w.cn

C++ ............ 30
来源：http://ihh.smart0.xyz

SQL ............ 90
来源：http://nrt.jianghu66.top

Bash ........... 80
来源：http://elq.sweek.top

Kotlin ......... 15
来源：http://ksu.zhaomingkeji.xyz

Swift .......... 15
来源：http://cjy.shzxlz.cn

Lua ............ 10
来源：http://yqj.zhengqikj.top

Perl ........... 10
来源：http://ghb.fengsongda.top

Scala .......... 10
来源：http://pmc.iojbl.cn

------------------------------------
来源：http://boy.aibaodan.cn

合计 ........... 2106 条
来源：http://tzp.yj202588.top

按章节统计：
来源：http://kha.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sqz.9152youxi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zao.haohaochexian.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ess.yj202588.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jfl.fanxiaobao.xyz


<!-- 参考信息 -->