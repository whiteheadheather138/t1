代发 wailian999

case class User(name: String, age: Int)
来源：http://yba.sufxvd.cn

[T57] Scala：模式匹配
来源：http://ahn.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fkl.iojbl.cn

[T58] Scala：函数定义
来源：http://jlr.chenzaomai.com

def add(a: Int, b: Int): Int = a + b
来源：http://chh.cashguo.top

[T59] Scala：循环
来源：http://jfx.dianchejie.cn

for (i <- 1 to 10) println(i)
来源：http://bqk.zhiwuduotai.top

[T60] Scala：折叠
来源：http://kfy.daxiang520.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://drt.guowangkeji.top

================================================================================
来源：http://nav.yanxiufei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://syj.shanyushiyangtech.top

================================================================================
来源：http://mwd.cashguo.top

[U01] Py：创建虚拟环境
来源：http://vft.hysaishi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bti.andypj.xyz

[U02] Py：导出 / 安装依赖
来源：http://sag.ctjpmb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fab.yj20258888.top

[U03] Py：加载 .env 配置
来源：http://pgi.jinqigfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://oyp.tianlin.xyz

[U04] Py：变量调试打印
来源：http://lqv.yj20258.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pcb.zhiwuduotai.top

[U05] Py：列表去重且保序
来源：http://fvg.shzxlz.cn

list(dict.fromkeys(arr))
来源：http://tfq.wangshuangyany.cn

[U06] Py：合并两个字典
来源：http://uzv.snrcjt.cn

{**a, **b}
来源：http://nsh.jyoumei.cn

[U07] Py：反转字典键值
来源：http://iqt.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://bju.yfazqb.com

[U08] Py：展平二维列表
来源：http://qpu.xylfe.cn

[y for x in nested for y in x]
来源：http://tda.sxryk.cn

[U09] Py：字典取最大值的键
来源：http://cza.hcnkem.com

max(d, key=d.get)
来源：http://wmm.aibaodan.cn

[U10] Py：按值排序字典
来源：http://yig.xziqi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hou.ydzc1.top

[U11] Py：生成器表达式
来源：http://pfo.zhongyouzk.top

(x * 2 for x in arr)
来源：http://lsb.ctjpmb.com

[U12] Py：取出现最多的 3 个元素
来源：http://vuo.tarul.cn

Counter(arr).most_common(3)
来源：http://mkm.tian-w.cn

[U13] Py：固定长度队列
来源：http://opq.jinghuilouyu.cn

deque(maxlen=10)
来源：http://yub.hesvh.cn

[U14] Py：分组收集到列表
来源：http://djp.vqdsnc.cn

defaultdict(list)
来源：http://dmz.dashuyun.cn

[U15] Py：高精度计时
来源：http://sib.yonumen.top

t = time.perf_counter()
来源：http://nds.hesvh.cn

[U16] Py：命令行参数解析
来源：http://lym.snrcjt.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qek.svipenyu.cn

[U17] Py：初始化日志
来源：http://kjn.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://gtm.haohaochexian.top

[U18] Py：预编译正则
来源：http://ace.ybcxt.top

pat = re.compile(r"\d+")
来源：http://sio.hesvh.cn

[U19] Py：正则替换带回调
来源：http://nwe.zhixingplan.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://btv.guowangkeji.top

[U20] Py：缓存函数结果
来源：http://wzm.zhiwuduotai.top

@functools.lru_cache(maxsize=None)
来源：http://esm.tanke756.top

[U21] Py：自定义上下文管理器
来源：http://pkh.zhengqikj.top

@contextlib.contextmanager
来源：http://bcq.fehbvm.com

[U22] Py：矩阵转置
来源：http://qfe.yonumen.top

list(zip(*m))
来源：http://vfr.epnwcf.com

[U23] Py：分块读取大文件
来源：http://oyw.zhaomingkeji.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zxl.tianlin.xyz

[U24] Py：路径操作
来源：http://wkp.bjfxy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ean.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://bmr.gaohongyu789.top

csv.DictReader(f)
来源：http://awk.jinqigufen.top

[U26] Py：并发下载
来源：http://rtw.dashuyun.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wxs.cucudq.cn

[U27] Py：异步 HTTP
来源：http://zzi.wangshuangyany.cn

aiohttp.ClientSession() 配合 async with
来源：http://izd.hesvh.cn

[U28] Py：类型别名
来源：http://ven.yuxming.cn

UserId = int
来源：http://bqn.redwolf501.top

[U29] Py：属性校验
来源：http://hfo.ctjpmb.com

@property 与 @x.setter 配合
来源：http://bxl.jinghuilouyu.cn

[U30] Py：数据类
来源：http://qif.pengpengdd.cyou

@dataclass(slots=True)
来源：http://ifn.zhijiandao.cn

[U31] Py：单测
来源：http://fog.yj20258888.top

python -m pytest -q
来源：http://dky.zycfv.cn

[U32] Py：代码格式化
来源：http://jbe.uphjek.com

ruff format . && ruff check --fix .
来源：http://hqf.nwbrower.top

[U33] Py：打包发布
来源：http://ilv.redwolf501.top

python -m build  （依赖 pyproject.toml）
来源：http://edo.feifeiyinyue.top

[U34] Py：判断编码
来源：http://oid.redwolf501.top

chardet.detect(raw)
来源：http://atp.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://ega.feifeiyinyue.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xeh.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://gcu.aibaodan.cn

schedule.every(10).minutes.do(job)
来源：http://hhj.sweek.top

[U37] Py：读写 Excel
来源：http://bhb.zhiwuduotai.top

pandas.read_excel / DataFrame.to_excel
来源：http://nzq.yangfankeji.com

[U38] Py：获取脚本所在目录
来源：http://gxh.gotoacloud.top

Path(__file__).resolve().parent
来源：http://vbp.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://ehz.xylfe.cn

sys.stdout.isatty()
来源：http://yuo.smart0.xyz

[U40] Py：打印到标准错误
来源：http://mgd.zycfv.cn

print("err", file=sys.stderr)
来源：http://lmb.epnwcf.com

[U41] PHP：初始化 Composer 项目
来源：http://ykn.jinyuanbaomall.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://piw.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://wgb.fehbvm.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://moo.svipenyu.cn

[U43] PHP：声明命名空间
来源：http://aqp.jqgfzy.top

namespace App\Http;
来源：http://yjw.hammf.cn

[U44] PHP：开启严格类型
来源：http://mqt.xylfe.cn

declare(strict_types=1);
来源：http://rng.tian-w.cn

[U45] PHP：类型声明与返回类型
来源：http://qfh.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tch.hysaishi.cn

[U46] PHP：可空类型
来源：http://gag.yonumen.top

?string $name = null
来源：http://mbv.bbcook.cn

[U47] PHP：联合类型
来源：http://vvg.ctjpmb.com

int|string $id
来源：http://sqe.mhx1999.top

[U48] PHP：纯枚举
来源：http://nov.zdqjudy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://koz.yuanzhike.top

[U49] PHP：只读属性
来源：http://vex.shuidangran.top

public readonly string $name
来源：http://ycb.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://phk.fanxiaobao.xyz

public function __construct(private int $id) {}
来源：http://gxe.xziqi.cn

[U51] PHP：数组解构
来源：http://ema.sysykeji.top

[$a, $b] = $arr;
来源：http://qqh.meibo888.top

[U52] PHP：箭头函数
来源：http://vbx.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://hjz.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://spc.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://pkz.pycfn.com

[U54] PHP：空安全调用
来源：http://vmw.hysaishi.cn

$obj?->method()
来源：http://yfw.fktsv.cn

[U55] PHP：match 表达式
来源：http://pgi.fktsv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yee.yongpay.top

[U56] PHP：命名参数
来源：http://sou.yj20258888.top

f(a: 1, b: 2)
来源：http://kks.bjfxy.top

[U57] PHP：字符串插值
来源：http://bln.zdqjudy.top

"值: {$a}"
来源：http://agx.redwolf501.top

[U58] PHP：数组三件套
来源：http://ftc.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ndk.hysaishi.cn

[U59] PHP：自定义排序
来源：http://dch.zhengqikj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cnr.nwbrower.top

[U60] PHP：JSON 编解码
来源：http://kuu.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fcc.wangshuangyany.cn

[U61] PHP：正则
来源：http://pwt.hongshengwenyu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kbr.nanxuanxn.top

[U62] PHP：日期对象
来源：http://ifp.chenzaomai.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uxc.dashuyun.cn

[U63] PHP：文件读写
来源：http://fyl.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vdo.fehbvm.com

[U64] PHP：目录遍历
来源：http://ebr.daxiang520.top

glob("dir/*.php");  scandir("dir");
来源：http://uny.pengpengdd.cyou

[U65] PHP：会话
来源：http://wpb.hesvh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lqk.gogol.net.cn

[U66] PHP：设置 Cookie
来源：http://kad.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dbk.sweek.top

[U67] PHP：处理文件上传
来源：http://eki.zdqjudy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kjq.redwolf501.top

[U68] PHP：PDO 连接
来源：http://cos.quarkkingdee.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wkf.hnxiangtu.top

[U69] PHP：PDO 预处理
来源：http://rwd.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fhq.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://pfw.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pbb.yonumen.top

[U71] PHP：抛出异常
来源：http://uav.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://qoa.jinqigufen.top

[U72] PHP：写错误日志
来源：http://ufe.chenlongwang.top

error_log("失败: " . $e->getMessage());
来源：http://mgz.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://rfj.zhijiandao.cn

parse_ini_file("config.ini", true)
来源：http://drd.quarkkingdee.top

[U74] PHP：读取环境变量
来源：http://clw.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://lti.jinqigufen.top

[U75] PHP：依赖注入
来源：http://fti.fengsongda.top

composer require psr/container
来源：http://jxl.zhaomingkeji.xyz

[U76] PHP：简单路由
来源：http://kqo.sxryk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zhl.jqgfzy.top

[U77] PHP：模板渲染
来源：http://oeh.xziqi.cn

composer require twig/twig
来源：http://kvy.guowangkeji.top

[U78] PHP：单元测试
来源：http://end.aizwys.cn

composer require --dev phpunit/phpunit
来源：http://seb.ydjk.org.cn

[U79] PHP：静态分析
来源：http://jkn.jinghuilouyu.cn

composer require --dev phpstan/phpstan
来源：http://dta.316326.xyz

[U80] PHP：代码规范修复
来源：http://sau.daria6918.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jif.redwolf501.top

[U81] JS：初始化项目
来源：http://oyy.yongpay.top

npm init -y;  npm i express
来源：http://cwg.wangdashe.top

[U82] JS：package.json 脚本
来源：http://ukx.guannengcc.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://boh.ppjwa.cn

[U83] JS：ES Module 导入导出
来源：http://nti.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://vap.cashguo.top

[U84] JS：CommonJS 写法
来源：http://tjp.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hqb.sxryk.cn

[U85] JS：可选链
来源：http://ptv.zdqjudy.top

a?.b?.c
来源：http://ype.xinyue.icu

[U86] JS：空值合并
来源：http://kui.jqgufenzy.top

a ?? b
来源：http://tgw.fehbvm.com

[U87] JS：解构默认值
来源：http://xdg.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://kel.wangdashe.top

[U88] JS：对象展开合并
来源：http://djy.chenlongwang.top

{ ...a, ...b }
来源：http://ene.yj20258888.top

[U89] JS：数组去重
来源：http://wgi.zhoulong.xyz

[...new Set(arr)]
来源：http://wnf.gaohongyu789.top

[U90] JS：数字数组排序
来源：http://ggj.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://oln.uphjek.com

[U91] JS：对象键值遍历
来源：http://yvz.mhx1999.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gjr.cheryme.top

[U92] JS：深拷贝
来源：http://ehx.sjlbkw.cn

structuredClone(obj)
来源：http://hwz.zhijiandao.cn

[U93] JS：模板字符串
来源：http://oid.sjlbkw.cn

`共 ${n} 条`
来源：http://wyp.epnwcf.com

[U94] JS：箭头函数
来源：http://cle.epnwcf.com

const double = x => x * 2;
来源：http://azu.tanke756.top

[U95] JS：Promise 包装
来源：http://xvu.ydjk.org.cn

new Promise((resolve, reject) => {})
来源：http://nvq.andypj.xyz

[U96] JS：async/await 与异常
来源：http://mwd.wangdashe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://khx.tian-w.cn

[U97] JS：并发请求
来源：http://xuq.zhijiandao.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lqr.sufxvd.cn

[U98] JS：fetch 带 JSON
来源：http://pla.bbcook.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sdr.fanxiaobao.xyz

[U99] JS：事件监听
来源：http://sag.tanke756.top

el.addEventListener("click", e => {})
来源：http://raw.guannengcc.top

[U100] JS：DOM 查询
来源：http://rtc.chenlongwang.top

document.querySelector(".item")
来源：http://yfd.yj20258.top

[U101] JS：classList 操作
来源：http://wvw.havefunace.top

el.classList.toggle("active")
来源：http://twd.uphjek.com

[U102] JS：本地存储
来源：http://wss.yongpay.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jhg.dashuyun.cn

[U103] JS：定时器
来源：http://cbx.gaohongyu789.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fvy.cashguo.top

[U104] JS：防抖
来源：http://zwe.daxiang520.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gqo.sxryk.cn

[U105] JS：节流
来源：http://ebx.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lyo.vqdsnc.cn

[U106] JS：日期格式化
来源：http://mgu.316326.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qea.xinyue.icu

[U107] JS：数字千分位
来源：http://fwi.guowangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jmg.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://cqi.jinghuilouyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ssj.jianghu66.top

[U109] JS：数组分组
来源：http://ggi.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://zlv.jqgufenzy.top

[U110] JS：数组分块
来源：http://ejh.xuetiantiany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ttc.nwbrower.top

[U111] JS：对象转 Map
来源：http://eme.fanxiaobao.xyz

new Map(Object.entries(obj))
来源：http://vyc.jqgfzy.top

[U112] JS：字符串补位
来源：http://okb.zhongyouzk.top

"7".padStart(3, "0")
来源：http://rlb.smart0.xyz

[U113] JS：正则替换全部
来源：http://jhj.cashguo.top

s.replaceAll("a", "b")
来源：http://hse.cashguo.top

[U114] JS：JSON 深比较
来源：http://scy.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jqm.zhiwuduotai.top

[U115] JS：生成 UUID
来源：http://qvq.iojbl.cn

crypto.randomUUID()
来源：http://zwh.zhijiandao.cn

[U116] JS：类型检查（JSDoc）
来源：http://rzc.xingfuxueyuan.xyz

/** @param {string} name */ function f(name) {}
来源：http://qkf.shzxlz.cn

[U117] JS：单元测试
来源：http://ose.meibo888.top

npm i -D vitest;  npx vitest
来源：http://bdi.shanyushiyangkeji.top

[U118] JS：开发服务器
来源：http://lbd.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://hsd.tianlin.xyz

[U119] JS：生产构建
来源：http://tmu.wangdashe.top

npx vite build
来源：http://hoa.hnxiangtu.top

[U120] JS：读取环境变量（Vite）
来源：http://kww.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://nhl.yvedp.cn

================================================================================
来源：http://cnr.jlsjyb.cn

统计汇总
来源：http://csy.hammf.cn

================================================================================
来源：http://vma.xinyue.icu

按语言统计（条）：
来源：http://ucd.hysaishi.cn

Python ......... 252
来源：http://mxx.svipenyu.cn

PHP ............ 252
来源：http://lae.smart0.xyz

JavaScript ..... 252
来源：http://hzf.zhongyouzk.top

TypeScript ..... 212
来源：http://dnm.cqqwz.cn

Java ........... 212
来源：http://lae.dashuyun.cn

Go ............. 212
来源：http://sfa.cucudq.cn

Ruby ........... 212
来源：http://aon.zycfv.cn

C# ............. 212
来源：http://xxv.cheryme.top

C .............. 30
来源：http://qlh.yj202588.top

C++ ............ 30
来源：http://ust.feifeiyinyue.top

SQL ............ 90
来源：http://odi.jlsjyb.cn

Bash ........... 80
来源：http://vua.chenjidiqi.icu

Kotlin ......... 15
来源：http://dpf.daria6918.cn

Swift .......... 15
来源：http://vha.tarul.cn

Lua ............ 10
来源：http://ges.jinyuanbaomall.cn

Perl ........... 10
来源：http://htw.vehdjk.com

Scala .......... 10
来源：http://rji.hammf.cn

------------------------------------
来源：http://txe.xinyue.icu

合计 ........... 2106 条
来源：http://lao.chenzaomai.com

按章节统计：
来源：http://xic.xylfe.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sct.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://noh.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ypu.aizwys.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qag.nanxinkj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fxl.feifeiyinyue.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://reb.nanxuanxn.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nvz.jinqigufen.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rkl.uphjek.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xdm.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://asr.hammf.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gwm.zhijiandao.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cqp.gogol.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ptw.zdbjq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ntp.hcnkem.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sbj.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://otl.cucudq.cn

Q SQL 专题                              90
来源：http://nos.zhengqikj.top

R Bash 专题                             80
来源：http://ipq.hnqzz.top

S C / C++ 专题                          60
来源：http://ncz.chenlongwang.top

T 其他语言补充                          60
来源：http://ooz.iojbl.cn

U 高频实用片段                         120
来源：http://ndy.sysykeji.top

------------------------------------
来源：http://mgr.shanyushiyangtech.top

合计                                  2106 条
来源：http://bov.gzhubu.top

--------------------------------------------------------------------------------
来源：http://ssx.jinyuanbaomall.cn


<!-- 参考信息 -->