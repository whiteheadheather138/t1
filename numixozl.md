代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://ufq.wangshuangyany.cn

[T55] Scala：集合过滤
来源：http://bzc.xuetiantiany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://djy.sjlbkw.cn

[T56] Scala：样例类
来源：http://pfe.ybcxt.top

case class User(name: String, age: Int)
来源：http://pmk.shuidangran.top

[T57] Scala：模式匹配
来源：http://epd.fehbvm.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://koz.ctjpmb.com

[T58] Scala：函数定义
来源：http://gjl.jqgfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://cnd.shzxlz.cn

[T59] Scala：循环
来源：http://wyw.hfpthk.cn

for (i <- 1 to 10) println(i)
来源：http://ioe.ppjwa.cn

[T60] Scala：折叠
来源：http://trh.gogol.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fsi.meibo888.top

================================================================================
来源：http://dva.aibaodan.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iva.hysaishi.cn

================================================================================
来源：http://lef.zhaomingkeji.xyz

[U01] Py：创建虚拟环境
来源：http://job.havefunace.top

python -m venv .venv && source .venv/bin/activate
来源：http://pdj.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://znz.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://omc.ydzc1.top

[U03] Py：加载 .env 配置
来源：http://bak.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tfx.zhongyouzk.top

[U04] Py：变量调试打印
来源：http://cbu.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zwg.jianghu66.top

[U05] Py：列表去重且保序
来源：http://rog.cashguo.top

list(dict.fromkeys(arr))
来源：http://xch.tian-w.cn

[U06] Py：合并两个字典
来源：http://ltr.xylfe.cn

{**a, **b}
来源：http://gnm.ctjpmb.com

[U07] Py：反转字典键值
来源：http://kwb.mhx1999.top

{v: k for k, v in d.items()}
来源：http://mrn.snrcjt.cn

[U08] Py：展平二维列表
来源：http://mxi.jiagoushi.top

[y for x in nested for y in x]
来源：http://jws.cashguo.top

[U09] Py：字典取最大值的键
来源：http://knk.ehwqpu.com

max(d, key=d.get)
来源：http://wts.yangfankeji.com

[U10] Py：按值排序字典
来源：http://iuu.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wbm.xylfe.cn

[U11] Py：生成器表达式
来源：http://rag.hesvh.cn

(x * 2 for x in arr)
来源：http://ifp.xuetiantiany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tkd.jianghu66.top

Counter(arr).most_common(3)
来源：http://doo.fktsv.cn

[U13] Py：固定长度队列
来源：http://den.yonumen.top

deque(maxlen=10)
来源：http://ndq.jinqigufen.top

[U14] Py：分组收集到列表
来源：http://fap.nanxinkj.top

defaultdict(list)
来源：http://fdw.yonumen.top

[U15] Py：高精度计时
来源：http://gia.xuetiantiany.cn

t = time.perf_counter()
来源：http://jfy.sxryk.cn

[U16] Py：命令行参数解析
来源：http://bwo.hfpthk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ama.shuidangran.top

[U17] Py：初始化日志
来源：http://qos.sjlbkw.cn

logging.basicConfig(level=logging.INFO)
来源：http://tns.sufxvd.cn

[U18] Py：预编译正则
来源：http://fat.yongpay.top

pat = re.compile(r"\d+")
来源：http://gdd.ivvv.top

[U19] Py：正则替换带回调
来源：http://ojt.xinyue.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://syo.guowangkeji.top

[U20] Py：缓存函数结果
来源：http://lyi.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://rjq.yfazqb.com

[U21] Py：自定义上下文管理器
来源：http://khx.zdbjq.cn

@contextlib.contextmanager
来源：http://sjw.bbcook.cn

[U22] Py：矩阵转置
来源：http://fij.jqgufenzy.top

list(zip(*m))
来源：http://gab.yvedp.cn

[U23] Py：分块读取大文件
来源：http://guk.iojbl.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://chj.jqgufenzy.top

[U24] Py：路径操作
来源：http://mob.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lsl.hnxiangtu.top

[U25] Py：CSV 按字典读
来源：http://okx.havefunace.top

csv.DictReader(f)
来源：http://jlz.jqgufenzy.top

[U26] Py：并发下载
来源：http://qsy.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xmg.yj202588.top

[U27] Py：异步 HTTP
来源：http://qsa.sweek.top

aiohttp.ClientSession() 配合 async with
来源：http://mth.smart0.xyz

[U28] Py：类型别名
来源：http://uhw.iojbl.cn

UserId = int
来源：http://owk.yvedp.cn

[U29] Py：属性校验
来源：http://buh.jqgufenzy.top

@property 与 @x.setter 配合
来源：http://sgj.316326.xyz

[U30] Py：数据类
来源：http://fim.dashuyun.cn

@dataclass(slots=True)
来源：http://ppq.iojbl.cn

[U31] Py：单测
来源：http://eqt.ehwqpu.com

python -m pytest -q
来源：http://gej.shanyushiyangkeji.top

[U32] Py：代码格式化
来源：http://egt.pycfn.com

ruff format . && ruff check --fix .
来源：http://qtx.yueranfly.top

[U33] Py：打包发布
来源：http://kne.fehbvm.com

python -m build  （依赖 pyproject.toml）
来源：http://gvs.zhoulong.xyz

[U34] Py：判断编码
来源：http://tqh.zdqjudy.top

chardet.detect(raw)
来源：http://asn.hnqzz.top

[U35] Py：发送邮件
来源：http://mna.ppjwa.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fqh.zhixingplan.top

[U36] Py：定时任务
来源：http://svf.sweek.top

schedule.every(10).minutes.do(job)
来源：http://kmp.yongpay.top

[U37] Py：读写 Excel
来源：http://wog.daria6918.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bae.shangyingyoupin.top

[U38] Py：获取脚本所在目录
来源：http://tva.dianchejie.cn

Path(__file__).resolve().parent
来源：http://uwn.yongpay.top

[U39] Py：判断是否在交互环境
来源：http://gqy.redwolf501.top

sys.stdout.isatty()
来源：http://evq.epnwcf.com

[U40] Py：打印到标准错误
来源：http://wfv.yj20258888.top

print("err", file=sys.stderr)
来源：http://zqm.xuanzx.com

[U41] PHP：初始化 Composer 项目
来源：http://ryc.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://iqt.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://rlf.sysykeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qxp.kuanghao11.cn

[U43] PHP：声明命名空间
来源：http://uls.hnxiangtu.top

namespace App\Http;
来源：http://kyw.nanxinkj.top

[U44] PHP：开启严格类型
来源：http://ibt.xziqi.cn

declare(strict_types=1);
来源：http://kbj.haohaochexian.top

[U45] PHP：类型声明与返回类型
来源：http://okj.uphjek.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://szo.jlsjyb.cn

[U46] PHP：可空类型
来源：http://ixs.zhiwuduotai.top

?string $name = null
来源：http://dcu.fktsv.cn

[U47] PHP：联合类型
来源：http://hnz.sweek.top

int|string $id
来源：http://srm.sxryk.cn

[U48] PHP：纯枚举
来源：http://jrm.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ecp.nwbrower.top

[U49] PHP：只读属性
来源：http://jla.gzhubu.top

public readonly string $name
来源：http://ejh.gogol.net.cn

[U50] PHP：构造器属性提升
来源：http://emz.sufxvd.cn

public function __construct(private int $id) {}
来源：http://fik.xylfe.cn

[U51] PHP：数组解构
来源：http://xol.fanxiaobao.xyz

[$a, $b] = $arr;
来源：http://mwe.hesvh.cn

[U52] PHP：箭头函数
来源：http://zao.jinqigufen.top

$double = fn($x) => $x * 2;
来源：http://mkm.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://ehg.yj202588.top

$v = $a ?? $b ?? "default";
来源：http://noz.zycfv.cn

[U54] PHP：空安全调用
来源：http://tmj.ppjwa.cn

$obj?->method()
来源：http://mej.jinqigufen.top

[U55] PHP：match 表达式
来源：http://jin.andypj.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ase.316326.xyz

[U56] PHP：命名参数
来源：http://ncv.hnxiangtu.top

f(a: 1, b: 2)
来源：http://szq.yongpay.top

[U57] PHP：字符串插值
来源：http://vcg.hnqzz.top

"值: {$a}"
来源：http://ytf.epnwcf.com

[U58] PHP：数组三件套
来源：http://sls.shangyingyoupin.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://epz.ctjpmb.com

[U59] PHP：自定义排序
来源：http://pka.jlsjyb.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qdv.sxryk.cn

[U60] PHP：JSON 编解码
来源：http://enq.havefunace.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wvj.iojbl.cn

[U61] PHP：正则
来源：http://djd.c1oappe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qws.chenlongwang.top

[U62] PHP：日期对象
来源：http://ujr.feifeiyinyue.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nbd.wangdashe.top

[U63] PHP：文件读写
来源：http://nme.jinqigfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://srm.bbcook.cn

[U64] PHP：目录遍历
来源：http://uvy.gotoacloud.top

glob("dir/*.php");  scandir("dir");
来源：http://iws.xuanzx.com

[U65] PHP：会话
来源：http://xtu.tian-w.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wkp.yj202588.top

[U66] PHP：设置 Cookie
来源：http://ath.jinqigufen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lej.xuetiantiany.cn

[U67] PHP：处理文件上传
来源：http://tjx.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://akg.sxryk.cn

[U68] PHP：PDO 连接
来源：http://wry.wangdashe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://img.cdnleiting.top

[U69] PHP：PDO 预处理
来源：http://hzj.zdbjq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tfz.fzhhl.top

[U70] PHP：PDO 事务
来源：http://tcw.hcnkem.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pxy.cdnleiting.top

[U71] PHP：抛出异常
来源：http://awe.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://kwq.wangdashe.top

[U72] PHP：写错误日志
来源：http://bay.hcnkem.com

error_log("失败: " . $e->getMessage());
来源：http://qld.sufxvd.cn

[U73] PHP：读取 ini 配置
来源：http://lvx.smart0.xyz

parse_ini_file("config.ini", true)
来源：http://xeb.wangdashe.top

[U74] PHP：读取环境变量
来源：http://whd.birdmap.top

getenv("APP_ENV") ?: "production"
来源：http://vov.hnxiangtu.top

[U75] PHP：依赖注入
来源：http://pyz.9152youxi.cn

composer require psr/container
来源：http://xfu.fzhhl.top

[U76] PHP：简单路由
来源：http://zuh.xingfuxueyuan.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uph.jinqigfzy.top

[U77] PHP：模板渲染
来源：http://ejs.yangfankeji.com

composer require twig/twig
来源：http://hyw.hywenlv.cn

[U78] PHP：单元测试
来源：http://zra.ehwqpu.com

composer require --dev phpunit/phpunit
来源：http://bak.shuidangran.top

[U79] PHP：静态分析
来源：http://gqf.zhijiandao.cn

composer require --dev phpstan/phpstan
来源：http://udu.hysaishi.cn

[U80] PHP：代码规范修复
来源：http://mvm.ybcxt.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rrr.jianghu66.top

[U81] JS：初始化项目
来源：http://bwj.havefunace.top

npm init -y;  npm i express
来源：http://xvj.havefunace.top

[U82] JS：package.json 脚本
来源：http://ykr.wangshuangyany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jov.fengsongda.top

[U83] JS：ES Module 导入导出
来源：http://kzo.gzhubu.top

export const a = 1;  import { a } from "./m.js";
来源：http://ewq.hysaishi.cn

[U84] JS：CommonJS 写法
来源：http://xkg.fengsongda.top

module.exports = { a };  const { a } = require("./m");
来源：http://xbf.hnxiangtu.top

[U85] JS：可选链
来源：http://amc.jiagoushi.top

a?.b?.c
来源：http://ywq.shangyingyoupin.top

[U86] JS：空值合并
来源：http://uwu.gotoacloud.top

a ?? b
来源：http://ter.tianlin.xyz

[U87] JS：解构默认值
来源：http://qpx.pycfn.com

const { a = 1, b = 2 } = obj;
来源：http://xrh.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://sim.yangfankeji.com

{ ...a, ...b }
来源：http://ajn.shangyingyoupin.top

[U89] JS：数组去重
来源：http://idr.tanke756.top

[...new Set(arr)]
来源：http://wau.ppjwa.cn

[U90] JS：数字数组排序
来源：http://iwp.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://msm.cashguo.top

[U91] JS：对象键值遍历
来源：http://pme.shangyingyoupin.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hjt.yanxiufei.cn

[U92] JS：深拷贝
来源：http://jcs.ywan-chungtsiang.top

structuredClone(obj)
来源：http://jmj.svipenyu.cn

[U93] JS：模板字符串
来源：http://rnw.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://bff.havefunace.top

[U94] JS：箭头函数
来源：http://vcl.tianlin.xyz

const double = x => x * 2;
来源：http://xlq.nwbrower.top

[U95] JS：Promise 包装
来源：http://tam.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://zde.fehbvm.com

[U96] JS：async/await 与异常
来源：http://tcn.yvedp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cjg.52xcode.cn

[U97] JS：并发请求
来源：http://fwi.xziqi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ckd.shangyingyoupin.top

[U98] JS：fetch 带 JSON
来源：http://imd.hysaishi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bhu.aibaodan.cn

[U99] JS：事件监听
来源：http://bhw.tianlin.xyz

el.addEventListener("click", e => {})
来源：http://bln.shanyushiyangkeji.top

[U100] JS：DOM 查询
来源：http://iow.zhengqikj.top

document.querySelector(".item")
来源：http://sjc.c1oappe.top

[U101] JS：classList 操作
来源：http://ijv.sufxvd.cn

el.classList.toggle("active")
来源：http://tgm.gaohongyu789.top

[U102] JS：本地存储
来源：http://cgf.hcnkem.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://wov.jiagoushi.top

[U103] JS：定时器
来源：http://kus.nanxuanxn.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ccm.cdnleiting.top

[U104] JS：防抖
来源：http://wox.tianlin.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pga.9152youxi.cn

[U105] JS：节流
来源：http://tqf.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eix.52xcode.cn

[U106] JS：日期格式化
来源：http://rgf.daria6918.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hmn.hywenlv.cn

[U107] JS：数字千分位
来源：http://okg.snrcjt.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nkc.redwolf501.top

[U108] JS：随机整数
来源：http://rrz.yfazqb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wgo.redwolf501.top

[U109] JS：数组分组
来源：http://yyl.chenlongwang.top

Object.groupBy(arr, x => x.type)
来源：http://hre.smart0.xyz

[U110] JS：数组分块
来源：http://ppw.tianlin.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zyu.nanxinkj.top

[U111] JS：对象转 Map
来源：http://gfh.yonumen.top

new Map(Object.entries(obj))
来源：http://mvm.vqdsnc.cn

[U112] JS：字符串补位
来源：http://den.yj20258888.top

"7".padStart(3, "0")
来源：http://ggl.fanxiaobao.xyz

[U113] JS：正则替换全部
来源：http://nyi.yueranfly.top

s.replaceAll("a", "b")
来源：http://nkp.sxryk.cn

[U114] JS：JSON 深比较
来源：http://knn.yonumen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tsi.snrcjt.cn

[U115] JS：生成 UUID
来源：http://txm.zhixingplan.top

crypto.randomUUID()
来源：http://uqm.yongpay.top

[U116] JS：类型检查（JSDoc）
来源：http://org.birdmap.top

/** @param {string} name */ function f(name) {}
来源：http://bbr.cucudq.cn

[U117] JS：单元测试
来源：http://zzt.shzxlz.cn

npm i -D vitest;  npx vitest
来源：http://zhe.hfpthk.cn

[U118] JS：开发服务器
来源：http://bcv.cashguo.top

npm i -D vite;  npx vite
来源：http://dxa.chenlongwang.top

[U119] JS：生产构建
来源：http://bth.ybcxt.top

npx vite build
来源：http://rlt.snrcjt.cn

[U120] JS：读取环境变量（Vite）
来源：http://ayb.sufxvd.cn

import.meta.env.VITE_API_URL
来源：http://fzu.gotoacloud.top

================================================================================
来源：http://rqj.hcnkem.com

统计汇总
来源：http://cjt.yanxiufei.cn

================================================================================
来源：http://uvw.fehbvm.com

按语言统计（条）：
来源：http://lcu.quarkkingdee.top

Python ......... 252
来源：http://xcp.jinqigufen.top

PHP ............ 252
来源：http://rkg.yuanzhike.top

JavaScript ..... 252
来源：http://mwn.cdnleiting.top

TypeScript ..... 212
来源：http://vzq.guannengcc.top

Java ........... 212
来源：http://qpl.jinghuilouyu.cn

Go ............. 212
来源：http://tgg.jianghu66.top

Ruby ........... 212
来源：http://wkl.jinghuilouyu.cn

C# ............. 212
来源：http://izr.zdbjq.cn

C .............. 30
来源：http://hsd.fktsv.cn

C++ ............ 30
来源：http://edz.ybcxt.top

SQL ............ 90
来源：http://mwt.nwbrower.top

Bash ........... 80
来源：http://dgm.zdqjudy.top

Kotlin ......... 15
来源：http://pia.snrcjt.cn

Swift .......... 15
来源：http://flh.jqgufenzy.top

Lua ............ 10
来源：http://ugu.chenlongwang.top

Perl ........... 10
来源：http://jpk.jinqigfzy.top

Scala .......... 10
来源：http://vne.mhx1999.top

------------------------------------
来源：http://bje.yuxming.cn

合计 ........... 2106 条
来源：http://asa.iojbl.cn

按章节统计：
来源：http://hfn.zhengqikj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yky.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vpc.wangshuangyany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ryz.smart0.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iuo.daria6918.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tdq.jyoumei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rwy.zdqjudy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qzw.jyoumei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kbv.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://opa.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vrz.jianghu66.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uop.zhiwuduotai.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dpx.ehwqpu.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dpg.vqdsnc.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ozx.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://osx.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cjp.tianlin.xyz

Q SQL 专题                              90
来源：http://mqw.zhixingplan.top

R Bash 专题                             80
来源：http://uts.gzhubu.top

S C / C++ 专题                          60
来源：http://iom.sysykeji.top

T 其他语言补充                          60
来源：http://xme.jiagoushi.top


<!-- 参考信息 -->