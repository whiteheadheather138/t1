代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://qvl.yvedp.cn

[T59] Scala：循环
来源：http://nvy.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://fyk.zdqjudy.top

[T60] Scala：折叠
来源：http://ydw.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bpq.xinyue.icu

================================================================================
来源：http://tlm.jqgfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://osr.shangyingyoupin.top

================================================================================
来源：http://daq.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://glw.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lrw.xuetiantiany.cn

[U02] Py：导出 / 安装依赖
来源：http://ery.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tsa.jyoumei.cn

[U03] Py：加载 .env 配置
来源：http://tbr.dashuyun.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vfc.jinqigufen.top

[U04] Py：变量调试打印
来源：http://yff.zhongyouzk.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ztl.epnwcf.com

[U05] Py：列表去重且保序
来源：http://xob.pycfn.com

list(dict.fromkeys(arr))
来源：http://xug.jlsjyb.cn

[U06] Py：合并两个字典
来源：http://rhw.fzhhl.top

{**a, **b}
来源：http://dti.nwbrower.top

[U07] Py：反转字典键值
来源：http://wxw.meibo888.top

{v: k for k, v in d.items()}
来源：http://oud.daxiang520.top

[U08] Py：展平二维列表
来源：http://tto.mhx1999.top

[y for x in nested for y in x]
来源：http://mro.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://zge.pycfn.com

max(d, key=d.get)
来源：http://epo.tanke756.top

[U10] Py：按值排序字典
来源：http://whm.hywenlv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jfh.cqqwz.cn

[U11] Py：生成器表达式
来源：http://ecx.zhongyouzk.top

(x * 2 for x in arr)
来源：http://sru.yj20258888.top

[U12] Py：取出现最多的 3 个元素
来源：http://xcy.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://ggm.shzxlz.cn

[U13] Py：固定长度队列
来源：http://olr.cashguo.top

deque(maxlen=10)
来源：http://kss.jinghuilouyu.cn

[U14] Py：分组收集到列表
来源：http://qdj.jyoumei.cn

defaultdict(list)
来源：http://cls.ybcxt.top

[U15] Py：高精度计时
来源：http://wet.jiagoushi.top

t = time.perf_counter()
来源：http://ywp.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://gab.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qei.vehdjk.com

[U17] Py：初始化日志
来源：http://ayx.hysaishi.cn

logging.basicConfig(level=logging.INFO)
来源：http://sdp.sweek.top

[U18] Py：预编译正则
来源：http://ifj.yfazqb.com

pat = re.compile(r"\d+")
来源：http://zgl.cqqwz.cn

[U19] Py：正则替换带回调
来源：http://uwc.jqgfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gsd.jinqigufen.top

[U20] Py：缓存函数结果
来源：http://jrx.feifeiyinyue.top

@functools.lru_cache(maxsize=None)
来源：http://joj.yj20258.top

[U21] Py：自定义上下文管理器
来源：http://afv.zycfv.cn

@contextlib.contextmanager
来源：http://dfu.shanyushiyangkeji.top

[U22] Py：矩阵转置
来源：http://pud.zhongyouzk.top

list(zip(*m))
来源：http://vjh.shanyushiyangkeji.top

[U23] Py：分块读取大文件
来源：http://fuu.gaohongyu789.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qgc.xuanzx.com

[U24] Py：路径操作
来源：http://szt.wangshuangyany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lry.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://qfc.wangshuangyany.cn

csv.DictReader(f)
来源：http://blw.fzhhl.top

[U26] Py：并发下载
来源：http://jad.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aap.guannengcc.top

[U27] Py：异步 HTTP
来源：http://oau.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://soz.jlsjyb.cn

[U28] Py：类型别名
来源：http://vix.shuidangran.top

UserId = int
来源：http://cfu.zhongyouzk.top

[U29] Py：属性校验
来源：http://pfd.aibaodan.cn

@property 与 @x.setter 配合
来源：http://odc.redwolf501.top

[U30] Py：数据类
来源：http://kql.9152youxi.cn

@dataclass(slots=True)
来源：http://ers.yueranfly.top

[U31] Py：单测
来源：http://idw.cucudq.cn

python -m pytest -q
来源：http://nys.yj202588.top

[U32] Py：代码格式化
来源：http://rhf.shzxlz.cn

ruff format . && ruff check --fix .
来源：http://yju.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://tht.yueranfly.top

python -m build  （依赖 pyproject.toml）
来源：http://ntu.c1oappe.top

[U34] Py：判断编码
来源：http://anp.vehdjk.com

chardet.detect(raw)
来源：http://hgu.epnwcf.com

[U35] Py：发送邮件
来源：http://cwi.tanke756.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ljm.sxryk.cn

[U36] Py：定时任务
来源：http://wzq.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://two.hywenlv.cn

[U37] Py：读写 Excel
来源：http://ubm.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://yjt.nanxuanxn.top

[U38] Py：获取脚本所在目录
来源：http://yfc.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://ggp.cheryme.top

[U39] Py：判断是否在交互环境
来源：http://pax.bjfxy.top

sys.stdout.isatty()
来源：http://gww.xingfuxueyuan.xyz

[U40] Py：打印到标准错误
来源：http://wfa.fengsongda.top

print("err", file=sys.stderr)
来源：http://bks.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://yzd.jianghu66.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fdk.sufxvd.cn

[U42] PHP：PSR-4 自动加载
来源：http://cio.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rac.ctjpmb.com

[U43] PHP：声明命名空间
来源：http://dnz.ybcxt.top

namespace App\Http;
来源：http://fpv.xuanzx.com

[U44] PHP：开启严格类型
来源：http://iwg.birdmap.top

declare(strict_types=1);
来源：http://kje.tanke756.top

[U45] PHP：类型声明与返回类型
来源：http://uno.redwolf501.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lvc.yueranfly.top

[U46] PHP：可空类型
来源：http://aym.sjlbkw.cn

?string $name = null
来源：http://shz.vehdjk.com

[U47] PHP：联合类型
来源：http://vji.chenzaomai.com

int|string $id
来源：http://spm.tianlin.xyz

[U48] PHP：纯枚举
来源：http://ktt.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xqh.mhx1999.top

[U49] PHP：只读属性
来源：http://stn.zhoulong.xyz

public readonly string $name
来源：http://wwf.daria6918.cn

[U50] PHP：构造器属性提升
来源：http://eiw.ctjpmb.com

public function __construct(private int $id) {}
来源：http://iok.daxiang520.top

[U51] PHP：数组解构
来源：http://ptq.jinyuanbaomall.cn

[$a, $b] = $arr;
来源：http://fny.ybcxt.top

[U52] PHP：箭头函数
来源：http://bxn.zhengqikj.top

$double = fn($x) => $x * 2;
来源：http://vpl.jinqigfzy.top

[U53] PHP：空合并运算符
来源：http://wqm.guowangkeji.top

$v = $a ?? $b ?? "default";
来源：http://qqm.xziqi.cn

[U54] PHP：空安全调用
来源：http://dvy.gzhubu.top

$obj?->method()
来源：http://eoi.c1oappe.top

[U55] PHP：match 表达式
来源：http://nku.xinyue.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jmu.cucudq.cn

[U56] PHP：命名参数
来源：http://eag.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://jne.nwbrower.top

[U57] PHP：字符串插值
来源：http://bng.cucudq.cn

"值: {$a}"
来源：http://cjk.ybcxt.top

[U58] PHP：数组三件套
来源：http://oob.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qaf.aizwys.cn

[U59] PHP：自定义排序
来源：http://kva.guowangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dmx.jinyuanbaomall.cn

[U60] PHP：JSON 编解码
来源：http://uub.nwbrower.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tor.yuxming.cn

[U61] PHP：正则
来源：http://och.zhongyouzk.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://chr.tian-w.cn

[U62] PHP：日期对象
来源：http://ozj.feifeiyinyue.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qsr.jianghu66.top

[U63] PHP：文件读写
来源：http://ihw.jqgufenzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dve.feifeiyinyue.top

[U64] PHP：目录遍历
来源：http://oal.hnxiangtu.top

glob("dir/*.php");  scandir("dir");
来源：http://kdi.gotoacloud.top

[U65] PHP：会话
来源：http://dio.sweek.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jfl.daxiang520.top

[U66] PHP：设置 Cookie
来源：http://ypi.xingfuxueyuan.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hty.sxryk.cn

[U67] PHP：处理文件上传
来源：http://jac.yongpay.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oop.haohaochexian.top

[U68] PHP：PDO 连接
来源：http://uzg.fktsv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xqd.fktsv.cn

[U69] PHP：PDO 预处理
来源：http://ooc.ivvv.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://agz.shanyushiyangkeji.top

[U70] PHP：PDO 事务
来源：http://wsr.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eoh.hammf.cn

[U71] PHP：抛出异常
来源：http://smr.jinqigfzy.top

throw new RuntimeException("失败", 500);
来源：http://hce.yj202588.top

[U72] PHP：写错误日志
来源：http://kld.shanyushiyangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://dbn.jqgufenzy.top

[U73] PHP：读取 ini 配置
来源：http://ywz.ppjwa.cn

parse_ini_file("config.ini", true)
来源：http://wsu.cheryme.top

[U74] PHP：读取环境变量
来源：http://zop.xingfuxueyuan.xyz

getenv("APP_ENV") ?: "production"
来源：http://wdg.aizwys.cn

[U75] PHP：依赖注入
来源：http://jkh.zhijiandao.cn

composer require psr/container
来源：http://tuo.yongpay.top

[U76] PHP：简单路由
来源：http://vkl.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rgv.uphjek.com

[U77] PHP：模板渲染
来源：http://gdo.c1oappe.top

composer require twig/twig
来源：http://xov.xziqi.cn

[U78] PHP：单元测试
来源：http://lbs.yonumen.top

composer require --dev phpunit/phpunit
来源：http://lra.svipenyu.cn

[U79] PHP：静态分析
来源：http://nkr.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://emd.fengsongda.top

[U80] PHP：代码规范修复
来源：http://kwk.wangdashe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rhx.haohaochexian.top

[U81] JS：初始化项目
来源：http://myx.tianlin.xyz

npm init -y;  npm i express
来源：http://rdj.pycfn.com

[U82] JS：package.json 脚本
来源：http://gcz.ywan-chungtsiang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://taz.fanxiaobao.xyz

[U83] JS：ES Module 导入导出
来源：http://zrq.ywan-chungtsiang.top

export const a = 1;  import { a } from "./m.js";
来源：http://vcs.nanxinkj.top

[U84] JS：CommonJS 写法
来源：http://frt.hysaishi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://are.hesvh.cn

[U85] JS：可选链
来源：http://qvz.hfpthk.cn

a?.b?.c
来源：http://ext.yvedp.cn

[U86] JS：空值合并
来源：http://yaa.shzxlz.cn

a ?? b
来源：http://ydd.jqgfzy.top

[U87] JS：解构默认值
来源：http://hqz.yj20258.top

const { a = 1, b = 2 } = obj;
来源：http://hfm.yj20258.top

[U88] JS：对象展开合并
来源：http://wwg.quarkkingdee.top

{ ...a, ...b }
来源：http://pej.gogol.net.cn

[U89] JS：数组去重
来源：http://tbz.vqdsnc.cn

[...new Set(arr)]
来源：http://iyv.fanxiaobao.xyz

[U90] JS：数字数组排序
来源：http://dia.gogol.net.cn

[...arr].sort((a, b) => a - b)
来源：http://mam.hnqzz.top

[U91] JS：对象键值遍历
来源：http://vcn.jinqigfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://czf.hywenlv.cn

[U92] JS：深拷贝
来源：http://urz.tian-w.cn

structuredClone(obj)
来源：http://ans.sxryk.cn

[U93] JS：模板字符串
来源：http://vef.xuetiantiany.cn

`共 ${n} 条`
来源：http://odw.zhijiandao.cn

[U94] JS：箭头函数
来源：http://ptv.chenlongwang.top

const double = x => x * 2;
来源：http://zef.chenzaomai.com

[U95] JS：Promise 包装
来源：http://ymc.wangshuangyany.cn

new Promise((resolve, reject) => {})
来源：http://juj.xuetiantiany.cn

[U96] JS：async/await 与异常
来源：http://mdz.yfazqb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ezd.jinqigufen.top

[U97] JS：并发请求
来源：http://rev.wangdashe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://djt.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://qqo.bjfxy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dfn.guowangkeji.top

[U99] JS：事件监听
来源：http://uml.ydzc1.top

el.addEventListener("click", e => {})
来源：http://xom.yanxiufei.cn

[U100] JS：DOM 查询
来源：http://wud.yonumen.top

document.querySelector(".item")
来源：http://zsk.svipenyu.cn

[U101] JS：classList 操作
来源：http://ybh.jianghu66.top

el.classList.toggle("active")
来源：http://xvo.zhixingplan.top

[U102] JS：本地存储
来源：http://pvx.gzhubu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mjy.sysykeji.top

[U103] JS：定时器
来源：http://wbn.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ttt.aibaodan.cn

[U104] JS：防抖
来源：http://uxe.xylfe.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jyb.cqqwz.cn

[U105] JS：节流
来源：http://amo.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oja.vehdjk.com

[U106] JS：日期格式化
来源：http://uks.jianghu66.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://one.tarul.cn

[U107] JS：数字千分位
来源：http://zsc.gzhubu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lij.yangfankeji.com

[U108] JS：随机整数
来源：http://bnb.wangshuangyany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fsk.nanxinkj.top

[U109] JS：数组分组
来源：http://iyd.hnxiangtu.top

Object.groupBy(arr, x => x.type)
来源：http://umo.bbcook.cn

[U110] JS：数组分块
来源：http://bnm.epnwcf.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iri.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://sjp.dashuyun.cn

new Map(Object.entries(obj))
来源：http://eda.cashguo.top

[U112] JS：字符串补位
来源：http://lql.jinghuilouyu.cn

"7".padStart(3, "0")
来源：http://eiu.pengpengdd.cyou

[U113] JS：正则替换全部
来源：http://lnm.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://epu.hysaishi.cn

[U114] JS：JSON 深比较
来源：http://guw.pengpengdd.cyou

JSON.stringify(a) === JSON.stringify(b)
来源：http://eza.nwbrower.top

[U115] JS：生成 UUID
来源：http://kyj.jinghuilouyu.cn

crypto.randomUUID()
来源：http://tqv.yj20258888.top

[U116] JS：类型检查（JSDoc）
来源：http://cbr.jinqigufen.top

/** @param {string} name */ function f(name) {}
来源：http://ixg.cqqwz.cn

[U117] JS：单元测试
来源：http://swr.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://trz.tianlin.xyz

[U118] JS：开发服务器
来源：http://dcz.jinqigufen.top

npm i -D vite;  npx vite
来源：http://lgg.ivvv.top

[U119] JS：生产构建
来源：http://hfy.wangdashe.top

npx vite build
来源：http://hgc.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://dwn.hcnkem.com

import.meta.env.VITE_API_URL
来源：http://bpw.dianchejie.cn

================================================================================
来源：http://hph.redwolf501.top

统计汇总
来源：http://qzq.xuetiantiany.cn

================================================================================
来源：http://xcj.dianchejie.cn

按语言统计（条）：
来源：http://gqw.ybcxt.top

Python ......... 252
来源：http://cuv.wangshuangyany.cn

PHP ............ 252
来源：http://qay.sxryk.cn

JavaScript ..... 252
来源：http://uqn.fzhhl.top

TypeScript ..... 212
来源：http://wgb.fehbvm.com

Java ........... 212
来源：http://aym.yj202588.top

Go ............. 212
来源：http://ihv.smart0.xyz

Ruby ........... 212
来源：http://ewo.smart0.xyz

C# ............. 212
来源：http://cnx.cashguo.top

C .............. 30
来源：http://gmr.yanxiufei.cn

C++ ............ 30
来源：http://ejf.52xcode.cn

SQL ............ 90
来源：http://oaa.dianchejie.cn

Bash ........... 80
来源：http://isz.gotoacloud.top

Kotlin ......... 15
来源：http://tju.jiagoushi.top

Swift .......... 15
来源：http://uqp.wangdashe.top

Lua ............ 10
来源：http://tyd.havefunace.top

Perl ........... 10
来源：http://uwl.shangyingyoupin.top

Scala .......... 10
来源：http://tud.cdnleiting.top

------------------------------------
来源：http://wog.yj202588.top

合计 ........... 2106 条
来源：http://knw.tanke756.top

按章节统计：
来源：http://ltb.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wdq.uphjek.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xxd.yuxming.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bot.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mic.guowangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ucw.iojbl.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rat.gaohongyu789.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zvd.xinyue.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vzw.jinyuanbaomall.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bcm.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rze.ppjwa.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://czm.gotoacloud.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uat.xingfuxueyuan.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fwz.sweek.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hed.dianchejie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kes.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wms.xinyue.icu

Q SQL 专题                              90
来源：http://ezw.yj20258888.top

R Bash 专题                             80
来源：http://byl.jlsjyb.cn

S C / C++ 专题                          60
来源：http://bgf.jiagoushi.top

T 其他语言补充                          60
来源：http://dje.ehwqpu.com

U 高频实用片段                         120
来源：http://xyz.xuanzx.com

------------------------------------
来源：http://uaz.316326.xyz

合计                                  2106 条
来源：http://hvl.fehbvm.com

--------------------------------------------------------------------------------
来源：http://rcb.gaohongyu789.top

使用提醒
来源：http://qpl.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://dow.guannengcc.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aeb.yuanzhike.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://chk.zdqjudy.top


<!-- 参考信息 -->