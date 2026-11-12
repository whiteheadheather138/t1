代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://vcw.xinyue.icu

[T55] Scala：集合过滤
来源：http://qoo.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://sde.nanxuanxn.top

[T56] Scala：样例类
来源：http://idj.aibaodan.cn

case class User(name: String, age: Int)
来源：http://lzi.xuanzx.com

[T57] Scala：模式匹配
来源：http://fzo.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ehb.cashguo.top

[T58] Scala：函数定义
来源：http://fcq.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://koz.wangshuangyany.cn

[T59] Scala：循环
来源：http://pbg.jianghu66.top

for (i <- 1 to 10) println(i)
来源：http://gmc.c1oappe.top

[T60] Scala：折叠
来源：http://sob.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qxg.birdmap.top

================================================================================
来源：http://yir.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xve.cucudq.cn

================================================================================
来源：http://mtq.guannengcc.top

[U01] Py：创建虚拟环境
来源：http://ylq.yj20258.top

python -m venv .venv && source .venv/bin/activate
来源：http://vkz.zdbjq.cn

[U02] Py：导出 / 安装依赖
来源：http://jgd.52xcode.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://avo.daria6918.cn

[U03] Py：加载 .env 配置
来源：http://chv.jqgfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jkm.xuetiantiany.cn

[U04] Py：变量调试打印
来源：http://ktk.wangshuangyany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cre.xuanzx.com

[U05] Py：列表去重且保序
来源：http://ksx.gzhubu.top

list(dict.fromkeys(arr))
来源：http://rhf.tanke756.top

[U06] Py：合并两个字典
来源：http://wot.fzhhl.top

{**a, **b}
来源：http://ynp.tianlin.xyz

[U07] Py：反转字典键值
来源：http://zar.redwolf501.top

{v: k for k, v in d.items()}
来源：http://mbn.yongpay.top

[U08] Py：展平二维列表
来源：http://mpw.pengpengdd.cyou

[y for x in nested for y in x]
来源：http://eon.wangdashe.top

[U09] Py：字典取最大值的键
来源：http://ccq.birdmap.top

max(d, key=d.get)
来源：http://ngf.sjlbkw.cn

[U10] Py：按值排序字典
来源：http://sed.pycfn.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kvu.andypj.xyz

[U11] Py：生成器表达式
来源：http://gjk.wangdashe.top

(x * 2 for x in arr)
来源：http://ttf.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://aqo.sweek.top

Counter(arr).most_common(3)
来源：http://vga.meibo888.top

[U13] Py：固定长度队列
来源：http://hzf.fanxiaobao.xyz

deque(maxlen=10)
来源：http://ake.shuidangran.top

[U14] Py：分组收集到列表
来源：http://qku.tian-w.cn

defaultdict(list)
来源：http://xck.jiagoushi.top

[U15] Py：高精度计时
来源：http://tdt.dianchejie.cn

t = time.perf_counter()
来源：http://yud.pycfn.com

[U16] Py：命令行参数解析
来源：http://mhf.ehwqpu.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vwo.birdmap.top

[U17] Py：初始化日志
来源：http://zcy.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://xzh.gaohongyu789.top

[U18] Py：预编译正则
来源：http://lsn.feifeiyinyue.top

pat = re.compile(r"\d+")
来源：http://tdm.redwolf501.top

[U19] Py：正则替换带回调
来源：http://her.mhx1999.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gfx.epnwcf.com

[U20] Py：缓存函数结果
来源：http://kph.epnwcf.com

@functools.lru_cache(maxsize=None)
来源：http://tlx.cheryme.top

[U21] Py：自定义上下文管理器
来源：http://nbb.mhx1999.top

@contextlib.contextmanager
来源：http://qty.cheryme.top

[U22] Py：矩阵转置
来源：http://ojk.zycfv.cn

list(zip(*m))
来源：http://jmi.tianlin.xyz

[U23] Py：分块读取大文件
来源：http://mht.uphjek.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nkd.fktsv.cn

[U24] Py：路径操作
来源：http://jdk.yj202588.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://upe.hongshengwenyu.top

[U25] Py：CSV 按字典读
来源：http://cue.birdmap.top

csv.DictReader(f)
来源：http://mro.gogol.net.cn

[U26] Py：并发下载
来源：http://nws.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qpp.chenlongwang.top

[U27] Py：异步 HTTP
来源：http://xfr.zhijiandao.cn

aiohttp.ClientSession() 配合 async with
来源：http://anc.yfazqb.com

[U28] Py：类型别名
来源：http://klx.zdqjudy.top

UserId = int
来源：http://jog.kuanghao11.cn

[U29] Py：属性校验
来源：http://uru.snrcjt.cn

@property 与 @x.setter 配合
来源：http://buj.zdqjudy.top

[U30] Py：数据类
来源：http://kkp.vehdjk.com

@dataclass(slots=True)
来源：http://cww.sysykeji.top

[U31] Py：单测
来源：http://dbd.daria6918.cn

python -m pytest -q
来源：http://oxb.9152youxi.cn

[U32] Py：代码格式化
来源：http://rvr.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://wwh.havefunace.top

[U33] Py：打包发布
来源：http://xpb.wangshuangyany.cn

python -m build  （依赖 pyproject.toml）
来源：http://cyz.snrcjt.cn

[U34] Py：判断编码
来源：http://knz.tian-w.cn

chardet.detect(raw)
来源：http://yhh.vqdsnc.cn

[U35] Py：发送邮件
来源：http://rcc.zhoulong.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mdr.mhx1999.top

[U36] Py：定时任务
来源：http://xfv.sxryk.cn

schedule.every(10).minutes.do(job)
来源：http://sbi.daxiang520.top

[U37] Py：读写 Excel
来源：http://slj.xylfe.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sjm.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://pgw.jinyuanbaomall.cn

Path(__file__).resolve().parent
来源：http://jty.fengsongda.top

[U39] Py：判断是否在交互环境
来源：http://rjf.cheryme.top

sys.stdout.isatty()
来源：http://tlq.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://hmv.chenjidiqi.icu

print("err", file=sys.stderr)
来源：http://zlt.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://xdg.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://pyl.bbcook.cn

[U42] PHP：PSR-4 自动加载
来源：http://djv.bjfxy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ngs.yfazqb.com

[U43] PHP：声明命名空间
来源：http://dlg.c1oappe.top

namespace App\Http;
来源：http://fpz.quarkkingdee.top

[U44] PHP：开启严格类型
来源：http://knc.sxryk.cn

declare(strict_types=1);
来源：http://vwc.yj20258.top

[U45] PHP：类型声明与返回类型
来源：http://cgb.shzxlz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bkg.zdqjudy.top

[U46] PHP：可空类型
来源：http://gvl.dianchejie.cn

?string $name = null
来源：http://ady.wangdashe.top

[U47] PHP：联合类型
来源：http://ipg.jlsjyb.cn

int|string $id
来源：http://icz.zdqjudy.top

[U48] PHP：纯枚举
来源：http://fbw.gaohongyu789.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wso.shzxlz.cn

[U49] PHP：只读属性
来源：http://zif.fzhhl.top

public readonly string $name
来源：http://iou.jinqigufen.top

[U50] PHP：构造器属性提升
来源：http://bav.nanxuanxn.top

public function __construct(private int $id) {}
来源：http://fzu.jinghuilouyu.cn

[U51] PHP：数组解构
来源：http://rvm.nanxuanxn.top

[$a, $b] = $arr;
来源：http://qsm.hywenlv.cn

[U52] PHP：箭头函数
来源：http://vdz.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://grz.sweek.top

[U53] PHP：空合并运算符
来源：http://dbl.jinghuilouyu.cn

$v = $a ?? $b ?? "default";
来源：http://ipo.yangfankeji.com

[U54] PHP：空安全调用
来源：http://xlf.hywenlv.cn

$obj?->method()
来源：http://gzo.zycfv.cn

[U55] PHP：match 表达式
来源：http://toe.hysaishi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zmq.aibaodan.cn

[U56] PHP：命名参数
来源：http://tax.hnxiangtu.top

f(a: 1, b: 2)
来源：http://pln.ppjwa.cn

[U57] PHP：字符串插值
来源：http://jnp.ppjwa.cn

"值: {$a}"
来源：http://ple.shanyushiyangkeji.top

[U58] PHP：数组三件套
来源：http://oaj.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uke.gzhubu.top

[U59] PHP：自定义排序
来源：http://bvb.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vrx.xuetiantiany.cn

[U60] PHP：JSON 编解码
来源：http://mtp.fktsv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xuw.sxryk.cn

[U61] PHP：正则
来源：http://asw.chenjidiqi.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sad.fehbvm.com

[U62] PHP：日期对象
来源：http://vsl.guowangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qcr.bbcook.cn

[U63] PHP：文件读写
来源：http://kmo.hesvh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zrr.xinyue.icu

[U64] PHP：目录遍历
来源：http://xbb.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://ysf.zhoulong.xyz

[U65] PHP：会话
来源：http://pbw.uphjek.com

session_start();  $_SESSION["uid"] = 1;
来源：http://xso.nanxinkj.top

[U66] PHP：设置 Cookie
来源：http://zqx.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tog.daxiang520.top

[U67] PHP：处理文件上传
来源：http://mmr.zhoulong.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bph.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://omx.hammf.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://far.svipenyu.cn

[U69] PHP：PDO 预处理
来源：http://dvp.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://put.uphjek.com

[U70] PHP：PDO 事务
来源：http://gxm.gzhubu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dwx.xuetiantiany.cn

[U71] PHP：抛出异常
来源：http://jjt.yueranfly.top

throw new RuntimeException("失败", 500);
来源：http://tgo.nanxinkj.top

[U72] PHP：写错误日志
来源：http://yck.kuanghao11.cn

error_log("失败: " . $e->getMessage());
来源：http://evk.hongshengwenyu.top

[U73] PHP：读取 ini 配置
来源：http://ppg.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://bel.sufxvd.cn

[U74] PHP：读取环境变量
来源：http://ngm.jinyuanbaomall.cn

getenv("APP_ENV") ?: "production"
来源：http://les.daria6918.cn

[U75] PHP：依赖注入
来源：http://uls.chenzaomai.com

composer require psr/container
来源：http://afq.uphjek.com

[U76] PHP：简单路由
来源：http://wyo.gogol.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://buu.zhengqikj.top

[U77] PHP：模板渲染
来源：http://iro.xuanzx.com

composer require twig/twig
来源：http://rsw.yfazqb.com

[U78] PHP：单元测试
来源：http://osk.zhoulong.xyz

composer require --dev phpunit/phpunit
来源：http://brq.epnwcf.com

[U79] PHP：静态分析
来源：http://olt.dianchejie.cn

composer require --dev phpstan/phpstan
来源：http://rqk.cqqwz.cn

[U80] PHP：代码规范修复
来源：http://tnn.hywenlv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://iyy.quarkkingdee.top

[U81] JS：初始化项目
来源：http://mev.pengpengdd.cyou

npm init -y;  npm i express
来源：http://tuc.jinqigfzy.top

[U82] JS：package.json 脚本
来源：http://qzh.aibaodan.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ejq.316326.xyz

[U83] JS：ES Module 导入导出
来源：http://cfk.jinghuilouyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zyu.jqgfzy.top

[U84] JS：CommonJS 写法
来源：http://qhn.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://oym.quarkkingdee.top

[U85] JS：可选链
来源：http://cqn.jqgfzy.top

a?.b?.c
来源：http://rwd.xinyue.icu

[U86] JS：空值合并
来源：http://gcg.zhixingplan.top

a ?? b
来源：http://wki.shzxlz.cn

[U87] JS：解构默认值
来源：http://wkm.yfazqb.com

const { a = 1, b = 2 } = obj;
来源：http://qbd.yangfankeji.com

[U88] JS：对象展开合并
来源：http://pfh.zhaomingkeji.xyz

{ ...a, ...b }
来源：http://oai.cdnleiting.top

[U89] JS：数组去重
来源：http://mpr.zhaomingkeji.xyz

[...new Set(arr)]
来源：http://ymd.xinyue.icu

[U90] JS：数字数组排序
来源：http://ovz.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://nny.cucudq.cn

[U91] JS：对象键值遍历
来源：http://aac.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qhu.chenzaomai.com

[U92] JS：深拷贝
来源：http://goi.shuidangran.top

structuredClone(obj)
来源：http://odc.fanxiaobao.xyz

[U93] JS：模板字符串
来源：http://fbh.daxiang520.top

`共 ${n} 条`
来源：http://bqv.havefunace.top

[U94] JS：箭头函数
来源：http://fjh.uphjek.com

const double = x => x * 2;
来源：http://bvd.shuidangran.top

[U95] JS：Promise 包装
来源：http://duo.xuanzx.com

new Promise((resolve, reject) => {})
来源：http://ssr.fanxiaobao.xyz

[U96] JS：async/await 与异常
来源：http://ofb.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mhq.0kj1m.cn

[U97] JS：并发请求
来源：http://dto.yj20258888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zwn.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://lmw.9152youxi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sfj.vehdjk.com

[U99] JS：事件监听
来源：http://lkd.jianghu66.top

el.addEventListener("click", e => {})
来源：http://aow.guowangkeji.top

[U100] JS：DOM 查询
来源：http://ehs.hnxiangtu.top

document.querySelector(".item")
来源：http://ejw.sjlbkw.cn

[U101] JS：classList 操作
来源：http://dev.meibo888.top

el.classList.toggle("active")
来源：http://npt.yuxming.cn

[U102] JS：本地存储
来源：http://bqy.jinqigfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hrb.c1oappe.top

[U103] JS：定时器
来源：http://efl.hfpthk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yar.yuanzhike.top

[U104] JS：防抖
来源：http://xhe.xinyue.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://van.zhiwuduotai.top

[U105] JS：节流
来源：http://vuc.yfazqb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://swm.fzhhl.top

[U106] JS：日期格式化
来源：http://txw.ywan-chungtsiang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ijv.xylfe.cn

[U107] JS：数字千分位
来源：http://mna.jianghu66.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nic.jqgufenzy.top

[U108] JS：随机整数
来源：http://irq.zhengqikj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ksk.0kj1m.cn

[U109] JS：数组分组
来源：http://xpr.zdqjudy.top

Object.groupBy(arr, x => x.type)
来源：http://ehs.bbcook.cn

[U110] JS：数组分块
来源：http://hrj.jinqigfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bny.bbcook.cn

[U111] JS：对象转 Map
来源：http://ggz.sweek.top

new Map(Object.entries(obj))
来源：http://dak.bjfxy.top

[U112] JS：字符串补位
来源：http://aom.hnqzz.top

"7".padStart(3, "0")
来源：http://hkx.shanyushiyangkeji.top

[U113] JS：正则替换全部
来源：http://nid.kuanghao11.cn

s.replaceAll("a", "b")
来源：http://uvt.xylfe.cn

[U114] JS：JSON 深比较
来源：http://egq.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qdt.kuanghao11.cn

[U115] JS：生成 UUID
来源：http://ced.ctjpmb.com

crypto.randomUUID()
来源：http://rcn.pycfn.com

[U116] JS：类型检查（JSDoc）
来源：http://euo.daria6918.cn

/** @param {string} name */ function f(name) {}
来源：http://rwe.tian-w.cn

[U117] JS：单元测试
来源：http://glx.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://bpt.fzhhl.top

[U118] JS：开发服务器
来源：http://oqp.mhx1999.top

npm i -D vite;  npx vite
来源：http://hsp.zhiwuduotai.top

[U119] JS：生产构建
来源：http://hkz.shuidangran.top

npx vite build
来源：http://xxf.tianlin.xyz

[U120] JS：读取环境变量（Vite）
来源：http://zsz.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://kmh.xziqi.cn

================================================================================
来源：http://cdg.xuanzx.com

统计汇总
来源：http://pgn.zdqjudy.top

================================================================================
来源：http://cmj.fktsv.cn

按语言统计（条）：
来源：http://uwo.xinyue.icu

Python ......... 252
来源：http://nuj.hfpthk.cn

PHP ............ 252
来源：http://oyk.hnqzz.top

JavaScript ..... 252
来源：http://mwe.shanyushiyangtech.top

TypeScript ..... 212
来源：http://yix.cdnleiting.top

Java ........... 212
来源：http://oru.jyoumei.cn

Go ............. 212
来源：http://kju.guowangkeji.top

Ruby ........... 212
来源：http://rhp.daria6918.cn

C# ............. 212
来源：http://nky.jinqigufen.top

C .............. 30
来源：http://ebn.dashuyun.cn

C++ ............ 30
来源：http://gky.dianchejie.cn

SQL ............ 90
来源：http://ljy.andypj.xyz

Bash ........... 80
来源：http://miw.jinqigufen.top

Kotlin ......... 15
来源：http://evr.cdnleiting.top

Swift .......... 15
来源：http://sbq.sysykeji.top

Lua ............ 10
来源：http://fci.wangdashe.top

Perl ........... 10
来源：http://dhg.gotoacloud.top

Scala .......... 10
来源：http://bql.hcnkem.com

------------------------------------
来源：http://pis.havefunace.top

合计 ........... 2106 条
来源：http://ybi.yj20258888.top

按章节统计：
来源：http://qux.shangyingyoupin.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mda.quarkkingdee.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tow.zhoulong.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://avl.zhiwuduotai.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kxs.haohaochexian.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://emd.yueranfly.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nzd.xylfe.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://svd.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jty.hysaishi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zon.cdnleiting.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lbr.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gkm.andypj.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ths.uphjek.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wrw.yfazqb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dfg.hfpthk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oii.jiagoushi.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lxt.52xcode.cn

Q SQL 专题                              90
来源：http://vym.ybcxt.top

R Bash 专题                             80
来源：http://tnj.svipenyu.cn

S C / C++ 专题                          60
来源：http://gki.hammf.cn

T 其他语言补充                          60
来源：http://jfc.xingfuxueyuan.xyz


<!-- 参考信息 -->