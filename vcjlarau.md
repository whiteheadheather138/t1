代发 wailian999

[T49] Perl：函数
来源：http://eqh.cucudq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gyb.gzhubu.top

[T50] Perl：逐行读文件
来源：http://ost.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://jub.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://ywy.cqqwz.cn

[T51] Scala：Hello World
来源：http://xqq.vqdsnc.cn

println("Hello")
来源：http://loy.guannengcc.top

[T52] Scala：变量
来源：http://uau.chenlongwang.top

val a = 1;  var b = 2
来源：http://ihh.9152youxi.cn

[T53] Scala：字符串插值
来源：http://bgw.xingfuxueyuan.xyz

s"值: $b"
来源：http://lja.smart0.xyz

[T54] Scala：集合映射
来源：http://eak.ybcxt.top

List(1, 2, 3).map(_ * 2)
来源：http://qwp.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://ezs.hongshengwenyu.top

List(1, 2, 3).filter(_ > 1)
来源：http://fyp.xziqi.cn

[T56] Scala：样例类
来源：http://qor.jiagoushi.top

case class User(name: String, age: Int)
来源：http://lxi.sxryk.cn

[T57] Scala：模式匹配
来源：http://pby.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://awe.xinyue.icu

[T58] Scala：函数定义
来源：http://jdw.hfpthk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fqa.hnxiangtu.top

[T59] Scala：循环
来源：http://xwq.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://ixn.sysykeji.top

[T60] Scala：折叠
来源：http://oad.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yey.svipenyu.cn

================================================================================
来源：http://ysv.xuetiantiany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://isa.yj20258888.top

================================================================================
来源：http://tyj.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://wkk.jinqigufen.top

python -m venv .venv && source .venv/bin/activate
来源：http://gbr.jinyuanbaomall.cn

[U02] Py：导出 / 安装依赖
来源：http://xds.zdbjq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xjh.hongshengwenyu.top

[U03] Py：加载 .env 配置
来源：http://ihw.fanxiaobao.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://ewp.9152youxi.cn

[U04] Py：变量调试打印
来源：http://tcy.daxiang520.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cfl.gogol.net.cn

[U05] Py：列表去重且保序
来源：http://sob.sxryk.cn

list(dict.fromkeys(arr))
来源：http://ujd.hcnkem.com

[U06] Py：合并两个字典
来源：http://ynm.iojbl.cn

{**a, **b}
来源：http://mmq.yj20258.top

[U07] Py：反转字典键值
来源：http://tav.uphjek.com

{v: k for k, v in d.items()}
来源：http://jho.fehbvm.com

[U08] Py：展平二维列表
来源：http://hbu.zhongyouzk.top

[y for x in nested for y in x]
来源：http://eeq.yanxiufei.cn

[U09] Py：字典取最大值的键
来源：http://typ.c1oappe.top

max(d, key=d.get)
来源：http://sgf.xziqi.cn

[U10] Py：按值排序字典
来源：http://ysm.ppjwa.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jvq.yanxiufei.cn

[U11] Py：生成器表达式
来源：http://ykv.jlsjyb.cn

(x * 2 for x in arr)
来源：http://adp.tarul.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ppc.cdnleiting.top

Counter(arr).most_common(3)
来源：http://njs.hesvh.cn

[U13] Py：固定长度队列
来源：http://ylw.c1oappe.top

deque(maxlen=10)
来源：http://iwu.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://kns.gotoacloud.top

defaultdict(list)
来源：http://rjw.yj20258888.top

[U15] Py：高精度计时
来源：http://nlz.jinyuanbaomall.cn

t = time.perf_counter()
来源：http://wgo.xziqi.cn

[U16] Py：命令行参数解析
来源：http://rdj.zhiwuduotai.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zys.fktsv.cn

[U17] Py：初始化日志
来源：http://yhh.jinyuanbaomall.cn

logging.basicConfig(level=logging.INFO)
来源：http://ney.zdqjudy.top

[U18] Py：预编译正则
来源：http://wod.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://rhh.meibo888.top

[U19] Py：正则替换带回调
来源：http://kpj.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qjo.birdmap.top

[U20] Py：缓存函数结果
来源：http://xhb.dashuyun.cn

@functools.lru_cache(maxsize=None)
来源：http://yhi.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://uav.xuanzx.com

@contextlib.contextmanager
来源：http://lsm.hesvh.cn

[U22] Py：矩阵转置
来源：http://cgb.yongpay.top

list(zip(*m))
来源：http://czi.vqdsnc.cn

[U23] Py：分块读取大文件
来源：http://ype.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gmc.dashuyun.cn

[U24] Py：路径操作
来源：http://hzq.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zcd.pengpengdd.cyou

[U25] Py：CSV 按字典读
来源：http://wbu.jinyuanbaomall.cn

csv.DictReader(f)
来源：http://tex.ppjwa.cn

[U26] Py：并发下载
来源：http://mhn.guowangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cig.pengpengdd.cyou

[U27] Py：异步 HTTP
来源：http://bhr.shangyingyoupin.top

aiohttp.ClientSession() 配合 async with
来源：http://goq.snrcjt.cn

[U28] Py：类型别名
来源：http://dsm.tian-w.cn

UserId = int
来源：http://mur.yuanzhike.top

[U29] Py：属性校验
来源：http://bul.xylfe.cn

@property 与 @x.setter 配合
来源：http://nhh.guowangkeji.top

[U30] Py：数据类
来源：http://rnj.jlsjyb.cn

@dataclass(slots=True)
来源：http://jbv.epnwcf.com

[U31] Py：单测
来源：http://nmm.wangdashe.top

python -m pytest -q
来源：http://epv.tian-w.cn

[U32] Py：代码格式化
来源：http://lzk.pengpengdd.cyou

ruff format . && ruff check --fix .
来源：http://fqw.tarul.cn

[U33] Py：打包发布
来源：http://qvr.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://eul.hnxiangtu.top

[U34] Py：判断编码
来源：http://nbz.zdbjq.cn

chardet.detect(raw)
来源：http://imk.daria6918.cn

[U35] Py：发送邮件
来源：http://nck.andypj.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ure.ehwqpu.com

[U36] Py：定时任务
来源：http://joc.yuanzhike.top

schedule.every(10).minutes.do(job)
来源：http://sbq.pengpengdd.cyou

[U37] Py：读写 Excel
来源：http://ufx.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pmc.fengsongda.top

[U38] Py：获取脚本所在目录
来源：http://xvb.ehwqpu.com

Path(__file__).resolve().parent
来源：http://hll.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://gzm.hcnkem.com

sys.stdout.isatty()
来源：http://ncd.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://qes.zhoulong.xyz

print("err", file=sys.stderr)
来源：http://tsu.wangdashe.top

[U41] PHP：初始化 Composer 项目
来源：http://hru.dianchejie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qaa.sjlbkw.cn

[U42] PHP：PSR-4 自动加载
来源：http://zpj.yuxming.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qvb.9152youxi.cn

[U43] PHP：声明命名空间
来源：http://yns.smart0.xyz

namespace App\Http;
来源：http://rqr.birdmap.top

[U44] PHP：开启严格类型
来源：http://rsx.tian-w.cn

declare(strict_types=1);
来源：http://one.yongpay.top

[U45] PHP：类型声明与返回类型
来源：http://lwn.zhixingplan.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://cxa.52xcode.cn

[U46] PHP：可空类型
来源：http://ktc.zycfv.cn

?string $name = null
来源：http://nxo.birdmap.top

[U47] PHP：联合类型
来源：http://wds.zhoulong.xyz

int|string $id
来源：http://isn.zdqjudy.top

[U48] PHP：纯枚举
来源：http://xnx.yj20258888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sxy.zhiwuduotai.top

[U49] PHP：只读属性
来源：http://vwx.zdbjq.cn

public readonly string $name
来源：http://wla.cdnleiting.top

[U50] PHP：构造器属性提升
来源：http://zss.fktsv.cn

public function __construct(private int $id) {}
来源：http://gvf.yj20258.top

[U51] PHP：数组解构
来源：http://pdc.redwolf501.top

[$a, $b] = $arr;
来源：http://eng.xziqi.cn

[U52] PHP：箭头函数
来源：http://uda.iojbl.cn

$double = fn($x) => $x * 2;
来源：http://ajy.xingfuxueyuan.xyz

[U53] PHP：空合并运算符
来源：http://gqr.chenzaomai.com

$v = $a ?? $b ?? "default";
来源：http://mty.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://sze.xingfuxueyuan.xyz

$obj?->method()
来源：http://qbd.meibo888.top

[U55] PHP：match 表达式
来源：http://bvf.zhengqikj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wng.tian-w.cn

[U56] PHP：命名参数
来源：http://mjb.zhiwuduotai.top

f(a: 1, b: 2)
来源：http://kpw.yonumen.top

[U57] PHP：字符串插值
来源：http://jpi.zhiwuduotai.top

"值: {$a}"
来源：http://gyq.bbcook.cn

[U58] PHP：数组三件套
来源：http://byf.chenzaomai.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zaw.zycfv.cn

[U59] PHP：自定义排序
来源：http://laz.iojbl.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cmj.yvedp.cn

[U60] PHP：JSON 编解码
来源：http://pat.sjlbkw.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zif.zdbjq.cn

[U61] PHP：正则
来源：http://qei.zhijiandao.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zaf.yuxming.cn

[U62] PHP：日期对象
来源：http://wfn.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zzf.yanxiufei.cn

[U63] PHP：文件读写
来源：http://deq.dashuyun.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://laa.gaohongyu789.top

[U64] PHP：目录遍历
来源：http://bku.hesvh.cn

glob("dir/*.php");  scandir("dir");
来源：http://doc.guannengcc.top

[U65] PHP：会话
来源：http://dpu.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ggm.wangshuangyany.cn

[U66] PHP：设置 Cookie
来源：http://avh.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://isw.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://cmm.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rjw.zhoulong.xyz

[U68] PHP：PDO 连接
来源：http://tdt.hongshengwenyu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pgy.jyoumei.cn

[U69] PHP：PDO 预处理
来源：http://mkt.daria6918.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wxp.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://jso.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ezo.sweek.top

[U71] PHP：抛出异常
来源：http://ikm.daxiang520.top

throw new RuntimeException("失败", 500);
来源：http://myk.shzxlz.cn

[U72] PHP：写错误日志
来源：http://gbs.yongpay.top

error_log("失败: " . $e->getMessage());
来源：http://noy.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://yuf.sxryk.cn

parse_ini_file("config.ini", true)
来源：http://xhq.hesvh.cn

[U74] PHP：读取环境变量
来源：http://fwj.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://jjf.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://zoo.xziqi.cn

composer require psr/container
来源：http://fxq.tarul.cn

[U76] PHP：简单路由
来源：http://ibk.xuetiantiany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jul.ivvv.top

[U77] PHP：模板渲染
来源：http://rny.jinyuanbaomall.cn

composer require twig/twig
来源：http://lhs.yfazqb.com

[U78] PHP：单元测试
来源：http://mva.ppjwa.cn

composer require --dev phpunit/phpunit
来源：http://ewq.uphjek.com

[U79] PHP：静态分析
来源：http://syp.zycfv.cn

composer require --dev phpstan/phpstan
来源：http://mcc.52xcode.cn

[U80] PHP：代码规范修复
来源：http://ves.xylfe.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://smj.vehdjk.com

[U81] JS：初始化项目
来源：http://ecn.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://uhl.iojbl.cn

[U82] JS：package.json 脚本
来源：http://fir.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hfe.redwolf501.top

[U83] JS：ES Module 导入导出
来源：http://qxg.smart0.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://thv.chenjidiqi.icu

[U84] JS：CommonJS 写法
来源：http://uvu.bbcook.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jwc.chenjidiqi.icu

[U85] JS：可选链
来源：http://dij.fktsv.cn

a?.b?.c
来源：http://ugu.hfpthk.cn

[U86] JS：空值合并
来源：http://zda.shanyushiyangkeji.top

a ?? b
来源：http://ltl.sjlbkw.cn

[U87] JS：解构默认值
来源：http://kce.zhengqikj.top

const { a = 1, b = 2 } = obj;
来源：http://lnf.ppjwa.cn

[U88] JS：对象展开合并
来源：http://wbj.hnxiangtu.top

{ ...a, ...b }
来源：http://zew.mhx1999.top

[U89] JS：数组去重
来源：http://kaz.xuetiantiany.cn

[...new Set(arr)]
来源：http://qxy.sweek.top

[U90] JS：数字数组排序
来源：http://xjq.c1oappe.top

[...arr].sort((a, b) => a - b)
来源：http://ohw.xylfe.cn

[U91] JS：对象键值遍历
来源：http://tjw.wangdashe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mpm.sufxvd.cn

[U92] JS：深拷贝
来源：http://opk.meibo888.top

structuredClone(obj)
来源：http://fet.guannengcc.top

[U93] JS：模板字符串
来源：http://xyq.hongshengwenyu.top

`共 ${n} 条`
来源：http://vyw.yj20258888.top

[U94] JS：箭头函数
来源：http://vqy.yj202588.top

const double = x => x * 2;
来源：http://hgu.nanxinkj.top

[U95] JS：Promise 包装
来源：http://zhn.pengpengdd.cyou

new Promise((resolve, reject) => {})
来源：http://uyi.tianlin.xyz

[U96] JS：async/await 与异常
来源：http://oie.yuxming.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fnl.redwolf501.top

[U97] JS：并发请求
来源：http://jmw.bbcook.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fpr.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://icg.chenzaomai.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zlb.gotoacloud.top

[U99] JS：事件监听
来源：http://dyq.smart0.xyz

el.addEventListener("click", e => {})
来源：http://uvy.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://ocs.zhaomingkeji.xyz

document.querySelector(".item")
来源：http://ula.guowangkeji.top

[U101] JS：classList 操作
来源：http://gbx.yangfankeji.com

el.classList.toggle("active")
来源：http://mnr.xuetiantiany.cn

[U102] JS：本地存储
来源：http://njm.xziqi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dgl.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://dpe.fzhhl.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ldc.ydjk.org.cn

[U104] JS：防抖
来源：http://gzg.feifeiyinyue.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nsf.uphjek.com

[U105] JS：节流
来源：http://obz.cucudq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qtm.zhixingplan.top

[U106] JS：日期格式化
来源：http://zhf.shuidangran.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zbb.wangshuangyany.cn

[U107] JS：数字千分位
来源：http://kya.yuanzhike.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yod.0kj1m.cn

[U108] JS：随机整数
来源：http://tvu.sysykeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://agx.meibo888.top

[U109] JS：数组分组
来源：http://wxm.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://uci.guannengcc.top

[U110] JS：数组分块
来源：http://kyl.pycfn.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oln.hongshengwenyu.top

[U111] JS：对象转 Map
来源：http://phh.sysykeji.top

new Map(Object.entries(obj))
来源：http://qcq.gaohongyu789.top

[U112] JS：字符串补位
来源：http://zze.daxiang520.top

"7".padStart(3, "0")
来源：http://ztf.mhx1999.top

[U113] JS：正则替换全部
来源：http://ejy.zhixingplan.top

s.replaceAll("a", "b")
来源：http://rhw.meibo888.top

[U114] JS：JSON 深比较
来源：http://wvc.fehbvm.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://qpn.quarkkingdee.top

[U115] JS：生成 UUID
来源：http://joa.52xcode.cn

crypto.randomUUID()
来源：http://ubu.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://zkv.havefunace.top

/** @param {string} name */ function f(name) {}
来源：http://ipy.xziqi.cn

[U117] JS：单元测试
来源：http://igl.ydzc1.top

npm i -D vitest;  npx vitest
来源：http://hws.daria6918.cn

[U118] JS：开发服务器
来源：http://mko.yueranfly.top

npm i -D vite;  npx vite
来源：http://yzd.c1oappe.top

[U119] JS：生产构建
来源：http://xvu.jinqigufen.top

npx vite build
来源：http://iyi.dianchejie.cn

[U120] JS：读取环境变量（Vite）
来源：http://rye.52xcode.cn

import.meta.env.VITE_API_URL
来源：http://pfi.zhijiandao.cn

================================================================================
来源：http://vkd.gzhubu.top

统计汇总
来源：http://riq.nwbrower.top

================================================================================
来源：http://bnh.fengsongda.top

按语言统计（条）：
来源：http://vro.chenzaomai.com

Python ......... 252
来源：http://cfc.yueranfly.top

PHP ............ 252
来源：http://ukb.ybcxt.top

JavaScript ..... 252
来源：http://jzb.havefunace.top

TypeScript ..... 212
来源：http://ccp.daria6918.cn

Java ........... 212
来源：http://wwt.shuidangran.top

Go ............. 212
来源：http://rdm.wangdashe.top

Ruby ........... 212
来源：http://ajs.ctjpmb.com

C# ............. 212
来源：http://sdw.zhijiandao.cn

C .............. 30
来源：http://xer.shanyushiyangkeji.top

C++ ............ 30
来源：http://goy.zhaomingkeji.xyz

SQL ............ 90
来源：http://rgk.316326.xyz

Bash ........... 80
来源：http://bgi.zhijiandao.cn

Kotlin ......... 15
来源：http://noo.yj20258.top

Swift .......... 15
来源：http://gcu.cucudq.cn

Lua ............ 10
来源：http://kmj.nanxinkj.top

Perl ........... 10
来源：http://zgh.gaohongyu789.top

Scala .......... 10
来源：http://rfh.jinghuilouyu.cn

------------------------------------
来源：http://lgp.snrcjt.cn

合计 ........... 2106 条
来源：http://cco.fzhhl.top

按章节统计：
来源：http://fum.shanyushiyangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nbv.jqgfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nji.quarkkingdee.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iax.yangfankeji.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lir.ppjwa.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aqe.havefunace.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gph.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nuh.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pdk.jinqigfzy.top


<!-- 参考信息 -->