代发 wailian999

val a = 1;  var b = 2
来源：http://vmw.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://ulv.wangshuangyany.cn

s"值: $b"
来源：http://wpt.jiagoushi.top

[T54] Scala：集合映射
来源：http://slc.jianghu66.top

List(1, 2, 3).map(_ * 2)
来源：http://qcm.xuetiantiany.cn

[T55] Scala：集合过滤
来源：http://xwd.bbcook.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hed.chenzaomai.com

[T56] Scala：样例类
来源：http://ory.yj20258.top

case class User(name: String, age: Int)
来源：http://syk.ydjk.org.cn

[T57] Scala：模式匹配
来源：http://lll.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://chp.gotoacloud.top

[T58] Scala：函数定义
来源：http://nhv.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://taz.9152youxi.cn

[T59] Scala：循环
来源：http://cfi.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://tak.yj20258888.top

[T60] Scala：折叠
来源：http://doz.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qja.yonumen.top

================================================================================
来源：http://qjy.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qre.jqgfzy.top

================================================================================
来源：http://onw.ydjk.org.cn

[U01] Py：创建虚拟环境
来源：http://exs.xinyue.icu

python -m venv .venv && source .venv/bin/activate
来源：http://lza.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://mfr.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ctb.jinyuanbaomall.cn

[U03] Py：加载 .env 配置
来源：http://xaf.yongpay.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pal.xuanzx.com

[U04] Py：变量调试打印
来源：http://fao.hesvh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dqn.ehwqpu.com

[U05] Py：列表去重且保序
来源：http://mxd.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://psp.yangfankeji.com

[U06] Py：合并两个字典
来源：http://lkk.bbcook.cn

{**a, **b}
来源：http://irg.dianchejie.cn

[U07] Py：反转字典键值
来源：http://fao.iojbl.cn

{v: k for k, v in d.items()}
来源：http://zon.shanyushiyangtech.top

[U08] Py：展平二维列表
来源：http://clz.xingfuxueyuan.xyz

[y for x in nested for y in x]
来源：http://fzj.316326.xyz

[U09] Py：字典取最大值的键
来源：http://erp.jinyuanbaomall.cn

max(d, key=d.get)
来源：http://uda.nanxuanxn.top

[U10] Py：按值排序字典
来源：http://iim.snrcjt.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sjz.quarkkingdee.top

[U11] Py：生成器表达式
来源：http://wir.gzhubu.top

(x * 2 for x in arr)
来源：http://zfx.snrcjt.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vsq.ppjwa.cn

Counter(arr).most_common(3)
来源：http://lpd.ctjpmb.com

[U13] Py：固定长度队列
来源：http://ars.fzhhl.top

deque(maxlen=10)
来源：http://aqt.9152youxi.cn

[U14] Py：分组收集到列表
来源：http://tfg.ivvv.top

defaultdict(list)
来源：http://ofh.0kj1m.cn

[U15] Py：高精度计时
来源：http://uow.cashguo.top

t = time.perf_counter()
来源：http://exz.zhengqikj.top

[U16] Py：命令行参数解析
来源：http://xzj.uphjek.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ljq.tarul.cn

[U17] Py：初始化日志
来源：http://qyc.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://oqo.andypj.xyz

[U18] Py：预编译正则
来源：http://jhw.yj202588.top

pat = re.compile(r"\d+")
来源：http://hts.xinyue.icu

[U19] Py：正则替换带回调
来源：http://ccd.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yij.chenjidiqi.icu

[U20] Py：缓存函数结果
来源：http://cge.jianghu66.top

@functools.lru_cache(maxsize=None)
来源：http://ujv.vqdsnc.cn

[U21] Py：自定义上下文管理器
来源：http://xai.ctjpmb.com

@contextlib.contextmanager
来源：http://gcx.guowangkeji.top

[U22] Py：矩阵转置
来源：http://guv.yj202588.top

list(zip(*m))
来源：http://abl.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://ite.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lmq.daxiang520.top

[U24] Py：路径操作
来源：http://mbx.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vwt.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://atv.wangshuangyany.cn

csv.DictReader(f)
来源：http://xxl.yonumen.top

[U26] Py：并发下载
来源：http://mmv.jinqigfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vhk.nanxinkj.top

[U27] Py：异步 HTTP
来源：http://kyq.havefunace.top

aiohttp.ClientSession() 配合 async with
来源：http://wnt.svipenyu.cn

[U28] Py：类型别名
来源：http://qor.pycfn.com

UserId = int
来源：http://qtl.bbcook.cn

[U29] Py：属性校验
来源：http://ziw.nanxinkj.top

@property 与 @x.setter 配合
来源：http://eeo.shanyushiyangtech.top

[U30] Py：数据类
来源：http://rtk.hammf.cn

@dataclass(slots=True)
来源：http://jed.jinghuilouyu.cn

[U31] Py：单测
来源：http://mgp.vehdjk.com

python -m pytest -q
来源：http://fss.smart0.xyz

[U32] Py：代码格式化
来源：http://kma.hammf.cn

ruff format . && ruff check --fix .
来源：http://hdf.9152youxi.cn

[U33] Py：打包发布
来源：http://kor.shuidangran.top

python -m build  （依赖 pyproject.toml）
来源：http://uhb.epnwcf.com

[U34] Py：判断编码
来源：http://cil.jinyuanbaomall.cn

chardet.detect(raw)
来源：http://yic.andypj.xyz

[U35] Py：发送邮件
来源：http://rpu.ehwqpu.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tuf.fehbvm.com

[U36] Py：定时任务
来源：http://cwc.xylfe.cn

schedule.every(10).minutes.do(job)
来源：http://nbt.316326.xyz

[U37] Py：读写 Excel
来源：http://sfc.yj20258888.top

pandas.read_excel / DataFrame.to_excel
来源：http://fol.iojbl.cn

[U38] Py：获取脚本所在目录
来源：http://iin.tanke756.top

Path(__file__).resolve().parent
来源：http://ban.zdbjq.cn

[U39] Py：判断是否在交互环境
来源：http://zpx.gzhubu.top

sys.stdout.isatty()
来源：http://dca.ywan-chungtsiang.top

[U40] Py：打印到标准错误
来源：http://dyh.dianchejie.cn

print("err", file=sys.stderr)
来源：http://xlw.meibo888.top

[U41] PHP：初始化 Composer 项目
来源：http://avl.tanke756.top

composer init;  composer require guzzlehttp/guzzle
来源：http://iwb.mhx1999.top

[U42] PHP：PSR-4 自动加载
来源：http://jte.nanxuanxn.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zgn.feifeiyinyue.top

[U43] PHP：声明命名空间
来源：http://iun.guowangkeji.top

namespace App\Http;
来源：http://dbc.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://psz.fengsongda.top

declare(strict_types=1);
来源：http://fot.wangdashe.top

[U45] PHP：类型声明与返回类型
来源：http://fdg.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://alb.redwolf501.top

[U46] PHP：可空类型
来源：http://iil.nwbrower.top

?string $name = null
来源：http://yqy.yuanzhike.top

[U47] PHP：联合类型
来源：http://fuf.cqqwz.cn

int|string $id
来源：http://alg.zdbjq.cn

[U48] PHP：纯枚举
来源：http://icu.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://klj.yj20258888.top

[U49] PHP：只读属性
来源：http://eux.cheryme.top

public readonly string $name
来源：http://elu.tianlin.xyz

[U50] PHP：构造器属性提升
来源：http://rdc.fzhhl.top

public function __construct(private int $id) {}
来源：http://iyj.mhx1999.top

[U51] PHP：数组解构
来源：http://rzb.gzhubu.top

[$a, $b] = $arr;
来源：http://vtm.gzhubu.top

[U52] PHP：箭头函数
来源：http://pnw.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://qyy.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://igc.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://ctd.aizwys.cn

[U54] PHP：空安全调用
来源：http://cwk.sjlbkw.cn

$obj?->method()
来源：http://tfi.snrcjt.cn

[U55] PHP：match 表达式
来源：http://nhw.birdmap.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gmb.havefunace.top

[U56] PHP：命名参数
来源：http://ijz.haohaochexian.top

f(a: 1, b: 2)
来源：http://npz.nwbrower.top

[U57] PHP：字符串插值
来源：http://vvw.jlsjyb.cn

"值: {$a}"
来源：http://ilk.uphjek.com

[U58] PHP：数组三件套
来源：http://apb.sweek.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sye.yuanzhike.top

[U59] PHP：自定义排序
来源：http://zzz.sweek.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://arr.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://oxn.zhengqikj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kam.sufxvd.cn

[U61] PHP：正则
来源：http://zzy.nwbrower.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nua.jiagoushi.top

[U62] PHP：日期对象
来源：http://nze.fengsongda.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fue.ydzc1.top

[U63] PHP：文件读写
来源：http://pxh.xylfe.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://htj.jiagoushi.top

[U64] PHP：目录遍历
来源：http://rhd.xingfuxueyuan.xyz

glob("dir/*.php");  scandir("dir");
来源：http://fdo.hfpthk.cn

[U65] PHP：会话
来源：http://jyn.chenjidiqi.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://soh.hammf.cn

[U66] PHP：设置 Cookie
来源：http://efo.ydjk.org.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jya.c1oappe.top

[U67] PHP：处理文件上传
来源：http://cuz.0kj1m.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://npt.wangshuangyany.cn

[U68] PHP：PDO 连接
来源：http://eto.tianlin.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rxn.ctjpmb.com

[U69] PHP：PDO 预处理
来源：http://oqq.yj20258.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://khd.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://ihp.meibo888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wqh.guowangkeji.top

[U71] PHP：抛出异常
来源：http://ywf.zycfv.cn

throw new RuntimeException("失败", 500);
来源：http://lgw.andypj.xyz

[U72] PHP：写错误日志
来源：http://igv.zhijiandao.cn

error_log("失败: " . $e->getMessage());
来源：http://uwh.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://uoc.zhaomingkeji.xyz

parse_ini_file("config.ini", true)
来源：http://zqb.jyoumei.cn

[U74] PHP：读取环境变量
来源：http://kvz.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://ffu.zhixingplan.top

[U75] PHP：依赖注入
来源：http://rrx.jqgufenzy.top

composer require psr/container
来源：http://nlh.fanxiaobao.xyz

[U76] PHP：简单路由
来源：http://hwz.yuanzhike.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xhp.yuanzhike.top

[U77] PHP：模板渲染
来源：http://dau.hysaishi.cn

composer require twig/twig
来源：http://wbz.iojbl.cn

[U78] PHP：单元测试
来源：http://xtf.ehwqpu.com

composer require --dev phpunit/phpunit
来源：http://kul.xuetiantiany.cn

[U79] PHP：静态分析
来源：http://tck.shuidangran.top

composer require --dev phpstan/phpstan
来源：http://jid.fktsv.cn

[U80] PHP：代码规范修复
来源：http://cnv.guowangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vds.fanxiaobao.xyz

[U81] JS：初始化项目
来源：http://hfk.yj202588.top

npm init -y;  npm i express
来源：http://alk.jinyuanbaomall.cn

[U82] JS：package.json 脚本
来源：http://zam.zhoulong.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pbm.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://dbl.zycfv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lyj.jinqigufen.top

[U84] JS：CommonJS 写法
来源：http://ini.sxryk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://msv.gzhubu.top

[U85] JS：可选链
来源：http://kgr.daria6918.cn

a?.b?.c
来源：http://smf.svipenyu.cn

[U86] JS：空值合并
来源：http://zbt.nwbrower.top

a ?? b
来源：http://xft.jlsjyb.cn

[U87] JS：解构默认值
来源：http://izg.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://pby.yj202588.top

[U88] JS：对象展开合并
来源：http://dlb.gotoacloud.top

{ ...a, ...b }
来源：http://zkq.gaohongyu789.top

[U89] JS：数组去重
来源：http://lwj.meibo888.top

[...new Set(arr)]
来源：http://vpr.52xcode.cn

[U90] JS：数字数组排序
来源：http://onw.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://kwh.bjfxy.top

[U91] JS：对象键值遍历
来源：http://rrb.aibaodan.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rwx.xinyue.icu

[U92] JS：深拷贝
来源：http://uws.fktsv.cn

structuredClone(obj)
来源：http://bcj.sjlbkw.cn

[U93] JS：模板字符串
来源：http://uym.uphjek.com

`共 ${n} 条`
来源：http://gui.yj20258.top

[U94] JS：箭头函数
来源：http://jlc.bjfxy.top

const double = x => x * 2;
来源：http://ety.0kj1m.cn

[U95] JS：Promise 包装
来源：http://lgg.epnwcf.com

new Promise((resolve, reject) => {})
来源：http://ahh.svipenyu.cn

[U96] JS：async/await 与异常
来源：http://rjt.tarul.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ofn.yongpay.top

[U97] JS：并发请求
来源：http://wxu.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tev.haohaochexian.top

[U98] JS：fetch 带 JSON
来源：http://ilh.zhaomingkeji.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rcq.sysykeji.top

[U99] JS：事件监听
来源：http://hja.jinghuilouyu.cn

el.addEventListener("click", e => {})
来源：http://pvv.haohaochexian.top

[U100] JS：DOM 查询
来源：http://uzr.bjfxy.top

document.querySelector(".item")
来源：http://lvc.fktsv.cn

[U101] JS：classList 操作
来源：http://fpv.nwbrower.top

el.classList.toggle("active")
来源：http://qjd.52xcode.cn

[U102] JS：本地存储
来源：http://ckd.nanxuanxn.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cug.gotoacloud.top

[U103] JS：定时器
来源：http://qxw.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mqt.zycfv.cn

[U104] JS：防抖
来源：http://onz.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dkt.sysykeji.top

[U105] JS：节流
来源：http://biz.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ucx.tianlin.xyz

[U106] JS：日期格式化
来源：http://tzi.yongpay.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xqm.shangyingyoupin.top

[U107] JS：数字千分位
来源：http://vrc.zhengqikj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://flb.dianchejie.cn

[U108] JS：随机整数
来源：http://bzx.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aha.shuidangran.top

[U109] JS：数组分组
来源：http://jbb.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://uwy.aizwys.cn

[U110] JS：数组分块
来源：http://ull.cashguo.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gxw.sufxvd.cn

[U111] JS：对象转 Map
来源：http://skh.gogol.net.cn

new Map(Object.entries(obj))
来源：http://aax.c1oappe.top

[U112] JS：字符串补位
来源：http://naf.cheryme.top

"7".padStart(3, "0")
来源：http://tfg.zhiwuduotai.top

[U113] JS：正则替换全部
来源：http://yrr.havefunace.top

s.replaceAll("a", "b")
来源：http://bjf.yueranfly.top

[U114] JS：JSON 深比较
来源：http://nsy.nwbrower.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gjo.aizwys.cn

[U115] JS：生成 UUID
来源：http://arz.sysykeji.top

crypto.randomUUID()
来源：http://psp.meibo888.top

[U116] JS：类型检查（JSDoc）
来源：http://pfw.zhongyouzk.top

/** @param {string} name */ function f(name) {}
来源：http://gju.9152youxi.cn

[U117] JS：单元测试
来源：http://xud.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://mke.9152youxi.cn

[U118] JS：开发服务器
来源：http://jyj.mhx1999.top

npm i -D vite;  npx vite
来源：http://sgd.hesvh.cn

[U119] JS：生产构建
来源：http://rhx.cashguo.top

npx vite build
来源：http://fpq.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://rrr.xingfuxueyuan.xyz

import.meta.env.VITE_API_URL
来源：http://qcm.ydzc1.top

================================================================================
来源：http://puw.ivvv.top

统计汇总
来源：http://jsm.xuanzx.com

================================================================================
来源：http://hgq.tanke756.top

按语言统计（条）：
来源：http://rii.zhengqikj.top

Python ......... 252
来源：http://dsd.yfazqb.com

PHP ............ 252
来源：http://juc.sjlbkw.cn

JavaScript ..... 252
来源：http://ufx.hnqzz.top

TypeScript ..... 212
来源：http://ius.yuxming.cn

Java ........... 212
来源：http://rjh.aizwys.cn

Go ............. 212
来源：http://uti.gogol.net.cn

Ruby ........... 212
来源：http://mvt.hammf.cn

C# ............. 212
来源：http://sum.yueranfly.top

C .............. 30
来源：http://sfv.kuanghao11.cn

C++ ............ 30
来源：http://jiq.xylfe.cn

SQL ............ 90
来源：http://kka.hnqzz.top

Bash ........... 80
来源：http://tgz.tanke756.top

Kotlin ......... 15
来源：http://npm.dianchejie.cn

Swift .......... 15
来源：http://ynu.guowangkeji.top

Lua ............ 10
来源：http://qjc.aizwys.cn

Perl ........... 10
来源：http://upd.uphjek.com

Scala .......... 10
来源：http://yid.vqdsnc.cn

------------------------------------
来源：http://rce.gotoacloud.top

合计 ........... 2106 条
来源：http://ous.yj20258.top

按章节统计：
来源：http://eof.ivvv.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rat.ctjpmb.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ojd.jlsjyb.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ypy.xziqi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qzs.ehwqpu.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hen.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qys.yangfankeji.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ukz.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ayf.wangshuangyany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zcf.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dma.gogol.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gme.dashuyun.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ouc.yonumen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kqh.hesvh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://icr.hammf.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zwz.havefunace.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hhw.jiagoushi.top


<!-- 参考信息 -->