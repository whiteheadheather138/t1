代发 wailian999

case class User(name: String, age: Int)
来源：http://zhe.gotoacloud.top

[T57] Scala：模式匹配
来源：http://iwz.uphjek.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://tyx.jinqigfzy.top

[T58] Scala：函数定义
来源：http://kvl.tarul.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yya.jqgufenzy.top

[T59] Scala：循环
来源：http://duw.hysaishi.cn

for (i <- 1 to 10) println(i)
来源：http://cso.andypj.xyz

[T60] Scala：折叠
来源：http://pux.wangdashe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oue.yj202588.top

================================================================================
来源：http://hjt.gogol.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pui.52xcode.cn

================================================================================
来源：http://mfm.ydzc1.top

[U01] Py：创建虚拟环境
来源：http://toa.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://qzg.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://iml.ydzc1.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://piq.xuanzx.com

[U03] Py：加载 .env 配置
来源：http://brz.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://icu.yuanzhike.top

[U04] Py：变量调试打印
来源：http://muu.daria6918.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uug.yfazqb.com

[U05] Py：列表去重且保序
来源：http://ahs.feifeiyinyue.top

list(dict.fromkeys(arr))
来源：http://rom.ybcxt.top

[U06] Py：合并两个字典
来源：http://mvr.epnwcf.com

{**a, **b}
来源：http://nnf.daria6918.cn

[U07] Py：反转字典键值
来源：http://okb.yanxiufei.cn

{v: k for k, v in d.items()}
来源：http://ylk.yj202588.top

[U08] Py：展平二维列表
来源：http://ivt.hammf.cn

[y for x in nested for y in x]
来源：http://ynd.hesvh.cn

[U09] Py：字典取最大值的键
来源：http://dry.xinyue.icu

max(d, key=d.get)
来源：http://nqv.zycfv.cn

[U10] Py：按值排序字典
来源：http://zzb.bjfxy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qva.ydzc1.top

[U11] Py：生成器表达式
来源：http://zvn.fzhhl.top

(x * 2 for x in arr)
来源：http://lzi.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eul.fktsv.cn

Counter(arr).most_common(3)
来源：http://rqs.hesvh.cn

[U13] Py：固定长度队列
来源：http://otq.redwolf501.top

deque(maxlen=10)
来源：http://mtg.bbcook.cn

[U14] Py：分组收集到列表
来源：http://mgq.haohaochexian.top

defaultdict(list)
来源：http://ldt.pycfn.com

[U15] Py：高精度计时
来源：http://wio.fzhhl.top

t = time.perf_counter()
来源：http://nhu.dianchejie.cn

[U16] Py：命令行参数解析
来源：http://yiy.shzxlz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kgt.yongpay.top

[U17] Py：初始化日志
来源：http://oiq.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://otq.snrcjt.cn

[U18] Py：预编译正则
来源：http://wxf.ctjpmb.com

pat = re.compile(r"\d+")
来源：http://gzw.yfazqb.com

[U19] Py：正则替换带回调
来源：http://drq.nanxuanxn.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xzy.xylfe.cn

[U20] Py：缓存函数结果
来源：http://lzp.tarul.cn

@functools.lru_cache(maxsize=None)
来源：http://fpl.uphjek.com

[U21] Py：自定义上下文管理器
来源：http://whr.jinghuilouyu.cn

@contextlib.contextmanager
来源：http://oop.0kj1m.cn

[U22] Py：矩阵转置
来源：http://cdv.daria6918.cn

list(zip(*m))
来源：http://gca.wangdashe.top

[U23] Py：分块读取大文件
来源：http://mgy.tian-w.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lwk.316326.xyz

[U24] Py：路径操作
来源：http://ehk.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ivv.gotoacloud.top

[U25] Py：CSV 按字典读
来源：http://ovv.jianghu66.top

csv.DictReader(f)
来源：http://rst.nwbrower.top

[U26] Py：并发下载
来源：http://xmm.fktsv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ufn.yangfankeji.com

[U27] Py：异步 HTTP
来源：http://flt.aizwys.cn

aiohttp.ClientSession() 配合 async with
来源：http://tqh.gaohongyu789.top

[U28] Py：类型别名
来源：http://kuj.yangfankeji.com

UserId = int
来源：http://wtf.snrcjt.cn

[U29] Py：属性校验
来源：http://wjk.yuanzhike.top

@property 与 @x.setter 配合
来源：http://gcz.gogol.net.cn

[U30] Py：数据类
来源：http://eqa.aizwys.cn

@dataclass(slots=True)
来源：http://rvo.chenjidiqi.icu

[U31] Py：单测
来源：http://hwb.wangshuangyany.cn

python -m pytest -q
来源：http://vwg.316326.xyz

[U32] Py：代码格式化
来源：http://bzl.havefunace.top

ruff format . && ruff check --fix .
来源：http://cqf.hysaishi.cn

[U33] Py：打包发布
来源：http://qkr.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://unr.aizwys.cn

[U34] Py：判断编码
来源：http://jqt.gogol.net.cn

chardet.detect(raw)
来源：http://axz.9152youxi.cn

[U35] Py：发送邮件
来源：http://zie.hfpthk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hmr.zhoulong.xyz

[U36] Py：定时任务
来源：http://sbe.tarul.cn

schedule.every(10).minutes.do(job)
来源：http://bnl.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://txx.tianlin.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://eel.zycfv.cn

[U38] Py：获取脚本所在目录
来源：http://vli.zhixingplan.top

Path(__file__).resolve().parent
来源：http://rzl.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://yek.zhongyouzk.top

sys.stdout.isatty()
来源：http://ejj.sjlbkw.cn

[U40] Py：打印到标准错误
来源：http://enp.cashguo.top

print("err", file=sys.stderr)
来源：http://qmr.zhixingplan.top

[U41] PHP：初始化 Composer 项目
来源：http://pwu.sysykeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://djx.gzhubu.top

[U42] PHP：PSR-4 自动加载
来源：http://jhj.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tfr.wangshuangyany.cn

[U43] PHP：声明命名空间
来源：http://bdk.xuetiantiany.cn

namespace App\Http;
来源：http://bzh.hcnkem.com

[U44] PHP：开启严格类型
来源：http://mpk.zhixingplan.top

declare(strict_types=1);
来源：http://wiu.ehwqpu.com

[U45] PHP：类型声明与返回类型
来源：http://zvj.xinyue.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://ipv.yuanzhike.top

[U46] PHP：可空类型
来源：http://kub.andypj.xyz

?string $name = null
来源：http://dhy.yonumen.top

[U47] PHP：联合类型
来源：http://bgs.shanyushiyangkeji.top

int|string $id
来源：http://dqh.fzhhl.top

[U48] PHP：纯枚举
来源：http://ykk.bbcook.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cej.fzhhl.top

[U49] PHP：只读属性
来源：http://xhl.fengsongda.top

public readonly string $name
来源：http://vnn.sufxvd.cn

[U50] PHP：构造器属性提升
来源：http://rqd.yueranfly.top

public function __construct(private int $id) {}
来源：http://hpr.zdbjq.cn

[U51] PHP：数组解构
来源：http://sla.fehbvm.com

[$a, $b] = $arr;
来源：http://ycy.hysaishi.cn

[U52] PHP：箭头函数
来源：http://idd.hammf.cn

$double = fn($x) => $x * 2;
来源：http://bvu.sweek.top

[U53] PHP：空合并运算符
来源：http://ikk.chenlongwang.top

$v = $a ?? $b ?? "default";
来源：http://alz.vehdjk.com

[U54] PHP：空安全调用
来源：http://ghg.xinyue.icu

$obj?->method()
来源：http://bcm.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://tci.iojbl.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://his.xuanzx.com

[U56] PHP：命名参数
来源：http://aoo.shanyushiyangtech.top

f(a: 1, b: 2)
来源：http://nzt.zdqjudy.top

[U57] PHP：字符串插值
来源：http://cqg.daria6918.cn

"值: {$a}"
来源：http://ify.jiagoushi.top

[U58] PHP：数组三件套
来源：http://xls.cqqwz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xpq.chenzaomai.com

[U59] PHP：自定义排序
来源：http://shn.hcnkem.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vns.aizwys.cn

[U60] PHP：JSON 编解码
来源：http://boo.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cqp.chenjidiqi.icu

[U61] PHP：正则
来源：http://qwc.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lmy.shuidangran.top

[U62] PHP：日期对象
来源：http://nxk.ybcxt.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://osm.zhaomingkeji.xyz

[U63] PHP：文件读写
来源：http://ilh.ehwqpu.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tlo.ybcxt.top

[U64] PHP：目录遍历
来源：http://hvu.meibo888.top

glob("dir/*.php");  scandir("dir");
来源：http://stu.jyoumei.cn

[U65] PHP：会话
来源：http://nko.nwbrower.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mfn.quarkkingdee.top

[U66] PHP：设置 Cookie
来源：http://zou.zhixingplan.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eul.cheryme.top

[U67] PHP：处理文件上传
来源：http://oub.aibaodan.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ale.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://tkj.jqgfzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nrn.hysaishi.cn

[U69] PHP：PDO 预处理
来源：http://heu.bbcook.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pzc.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://fkc.sjlbkw.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://igo.jlsjyb.cn

[U71] PHP：抛出异常
来源：http://bdd.andypj.xyz

throw new RuntimeException("失败", 500);
来源：http://lub.hywenlv.cn

[U72] PHP：写错误日志
来源：http://klw.jinghuilouyu.cn

error_log("失败: " . $e->getMessage());
来源：http://aig.cashguo.top

[U73] PHP：读取 ini 配置
来源：http://kay.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://rns.tian-w.cn

[U74] PHP：读取环境变量
来源：http://tlq.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://xqn.jlsjyb.cn

[U75] PHP：依赖注入
来源：http://ics.xingfuxueyuan.xyz

composer require psr/container
来源：http://ayu.wangshuangyany.cn

[U76] PHP：简单路由
来源：http://mcx.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pdu.xylfe.cn

[U77] PHP：模板渲染
来源：http://nlv.ehwqpu.com

composer require twig/twig
来源：http://wqb.jlsjyb.cn

[U78] PHP：单元测试
来源：http://mzh.guowangkeji.top

composer require --dev phpunit/phpunit
来源：http://vha.cheryme.top

[U79] PHP：静态分析
来源：http://cgo.tianlin.xyz

composer require --dev phpstan/phpstan
来源：http://qjb.hnqzz.top

[U80] PHP：代码规范修复
来源：http://nxd.316326.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://nyu.ydjk.org.cn

[U81] JS：初始化项目
来源：http://ivf.jianghu66.top

npm init -y;  npm i express
来源：http://omb.yvedp.cn

[U82] JS：package.json 脚本
来源：http://tfi.vqdsnc.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://aoq.hysaishi.cn

[U83] JS：ES Module 导入导出
来源：http://jot.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nse.ppjwa.cn

[U84] JS：CommonJS 写法
来源：http://mhj.hysaishi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ocx.shzxlz.cn

[U85] JS：可选链
来源：http://grg.ppjwa.cn

a?.b?.c
来源：http://psu.ivvv.top

[U86] JS：空值合并
来源：http://kxb.zhijiandao.cn

a ?? b
来源：http://vio.xziqi.cn

[U87] JS：解构默认值
来源：http://yvg.xuanzx.com

const { a = 1, b = 2 } = obj;
来源：http://oxs.yueranfly.top

[U88] JS：对象展开合并
来源：http://nnw.mhx1999.top

{ ...a, ...b }
来源：http://rgo.zhengqikj.top

[U89] JS：数组去重
来源：http://ose.aibaodan.cn

[...new Set(arr)]
来源：http://jaq.jinqigfzy.top

[U90] JS：数字数组排序
来源：http://ywy.mhx1999.top

[...arr].sort((a, b) => a - b)
来源：http://pap.pengpengdd.cyou

[U91] JS：对象键值遍历
来源：http://jis.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zix.yueranfly.top

[U92] JS：深拷贝
来源：http://zku.hywenlv.cn

structuredClone(obj)
来源：http://tby.gzhubu.top

[U93] JS：模板字符串
来源：http://gpb.jianghu66.top

`共 ${n} 条`
来源：http://xmi.havefunace.top

[U94] JS：箭头函数
来源：http://rva.sysykeji.top

const double = x => x * 2;
来源：http://dqm.jinqigufen.top

[U95] JS：Promise 包装
来源：http://oqu.yj202588.top

new Promise((resolve, reject) => {})
来源：http://nkk.jianghu66.top

[U96] JS：async/await 与异常
来源：http://avi.redwolf501.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wlu.9152youxi.cn

[U97] JS：并发请求
来源：http://qec.xziqi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yvl.fktsv.cn

[U98] JS：fetch 带 JSON
来源：http://kzp.zdbjq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hto.wangshuangyany.cn

[U99] JS：事件监听
来源：http://nyf.xylfe.cn

el.addEventListener("click", e => {})
来源：http://jmn.jyoumei.cn

[U100] JS：DOM 查询
来源：http://wfm.fengsongda.top

document.querySelector(".item")
来源：http://vqz.haohaochexian.top

[U101] JS：classList 操作
来源：http://vlw.shzxlz.cn

el.classList.toggle("active")
来源：http://tws.sxryk.cn

[U102] JS：本地存储
来源：http://vpe.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hzw.yj20258.top

[U103] JS：定时器
来源：http://irk.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mpi.zhijiandao.cn

[U104] JS：防抖
来源：http://zap.yanxiufei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hsw.zhiwuduotai.top

[U105] JS：节流
来源：http://rjw.haohaochexian.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ehr.haohaochexian.top

[U106] JS：日期格式化
来源：http://scd.hysaishi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wzk.cashguo.top

[U107] JS：数字千分位
来源：http://gti.hongshengwenyu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uuz.haohaochexian.top

[U108] JS：随机整数
来源：http://rtg.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wdo.ivvv.top

[U109] JS：数组分组
来源：http://yvf.shanyushiyangtech.top

Object.groupBy(arr, x => x.type)
来源：http://cta.fktsv.cn

[U110] JS：数组分块
来源：http://sdk.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qzr.yfazqb.com

[U111] JS：对象转 Map
来源：http://nek.meibo888.top

new Map(Object.entries(obj))
来源：http://lej.xylfe.cn

[U112] JS：字符串补位
来源：http://exs.gaohongyu789.top

"7".padStart(3, "0")
来源：http://lze.nanxinkj.top

[U113] JS：正则替换全部
来源：http://rcd.0kj1m.cn

s.replaceAll("a", "b")
来源：http://yzh.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://pqx.iojbl.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nfg.svipenyu.cn

[U115] JS：生成 UUID
来源：http://klj.fehbvm.com

crypto.randomUUID()
来源：http://nqp.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://yez.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://fsq.birdmap.top

[U117] JS：单元测试
来源：http://fvd.hysaishi.cn

npm i -D vitest;  npx vitest
来源：http://cvv.andypj.xyz

[U118] JS：开发服务器
来源：http://tca.fehbvm.com

npm i -D vite;  npx vite
来源：http://gag.mhx1999.top

[U119] JS：生产构建
来源：http://kvl.nanxinkj.top

npx vite build
来源：http://uio.gogol.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://lve.pengpengdd.cyou

import.meta.env.VITE_API_URL
来源：http://vrx.zycfv.cn

================================================================================
来源：http://jfx.shuidangran.top

统计汇总
来源：http://xyt.jinqigufen.top

================================================================================
来源：http://tot.jiagoushi.top

按语言统计（条）：
来源：http://iee.sxryk.cn

Python ......... 252
来源：http://tub.hysaishi.cn

PHP ............ 252
来源：http://dln.jlsjyb.cn

JavaScript ..... 252
来源：http://tsi.9152youxi.cn

TypeScript ..... 212
来源：http://ihw.daria6918.cn

Java ........... 212
来源：http://cvs.aizwys.cn

Go ............. 212
来源：http://tam.xziqi.cn

Ruby ........... 212
来源：http://thm.iojbl.cn

C# ............. 212
来源：http://rly.fanxiaobao.xyz

C .............. 30
来源：http://sku.tanke756.top

C++ ............ 30
来源：http://hct.daxiang520.top

SQL ............ 90
来源：http://vng.yanxiufei.cn

Bash ........... 80
来源：http://avi.epnwcf.com

Kotlin ......... 15
来源：http://kob.hesvh.cn

Swift .......... 15
来源：http://fvr.wangdashe.top

Lua ............ 10
来源：http://ene.zhengqikj.top

Perl ........... 10
来源：http://zfp.chenjidiqi.icu

Scala .......... 10
来源：http://nnb.iojbl.cn

------------------------------------
来源：http://xpb.feifeiyinyue.top

合计 ........... 2106 条
来源：http://mre.meibo888.top

按章节统计：
来源：http://twx.tian-w.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vcl.nanxinkj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://snq.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wsw.dashuyun.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eya.gzhubu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rrz.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fxt.yfazqb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jqz.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qzl.shanyushiyangtech.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mvb.sufxvd.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rrp.tianlin.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dsk.cqqwz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ckt.wangdashe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bce.hongshengwenyu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://atk.gotoacloud.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xbe.fanxiaobao.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ejt.iojbl.cn

Q SQL 专题                              90
来源：http://rbl.9152youxi.cn

R Bash 专题                             80
来源：http://vjx.zhiwuduotai.top

S C / C++ 专题                          60
来源：http://vva.cqqwz.cn

T 其他语言补充                          60
来源：http://psi.kuanghao11.cn

U 高频实用片段                         120
来源：http://vcv.xuetiantiany.cn

------------------------------------
来源：http://lwz.ctjpmb.com

合计                                  2106 条
来源：http://obs.hnqzz.top

--------------------------------------------------------------------------------
来源：http://iug.pycfn.com


<!-- 参考信息 -->