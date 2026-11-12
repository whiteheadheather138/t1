代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://ghs.hysaishi.cn

[T59] Scala：循环
来源：http://gcm.fehbvm.com

for (i <- 1 to 10) println(i)
来源：http://bbs.guowangkeji.top

[T60] Scala：折叠
来源：http://drd.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jkd.9152youxi.cn

================================================================================
来源：http://pix.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://frc.nwbrower.top

================================================================================
来源：http://sfg.yfazqb.com

[U01] Py：创建虚拟环境
来源：http://fxo.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://dva.shzxlz.cn

[U02] Py：导出 / 安装依赖
来源：http://mvg.birdmap.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lcx.yonumen.top

[U03] Py：加载 .env 配置
来源：http://jkg.iojbl.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ibg.zhoulong.xyz

[U04] Py：变量调试打印
来源：http://goe.ehwqpu.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lia.yj20258888.top

[U05] Py：列表去重且保序
来源：http://lre.gzhubu.top

list(dict.fromkeys(arr))
来源：http://nfr.chenzaomai.com

[U06] Py：合并两个字典
来源：http://qlp.guowangkeji.top

{**a, **b}
来源：http://xah.cheryme.top

[U07] Py：反转字典键值
来源：http://hqk.yvedp.cn

{v: k for k, v in d.items()}
来源：http://orr.yueranfly.top

[U08] Py：展平二维列表
来源：http://qag.sufxvd.cn

[y for x in nested for y in x]
来源：http://fva.zycfv.cn

[U09] Py：字典取最大值的键
来源：http://gwa.fengsongda.top

max(d, key=d.get)
来源：http://fbf.zhiwuduotai.top

[U10] Py：按值排序字典
来源：http://kns.wangdashe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jbp.meibo888.top

[U11] Py：生成器表达式
来源：http://tvv.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://kfl.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://cnx.birdmap.top

Counter(arr).most_common(3)
来源：http://jsy.bbcook.cn

[U13] Py：固定长度队列
来源：http://gqs.yuanzhike.top

deque(maxlen=10)
来源：http://ypc.fanxiaobao.xyz

[U14] Py：分组收集到列表
来源：http://qlj.hywenlv.cn

defaultdict(list)
来源：http://iix.jinyuanbaomall.cn

[U15] Py：高精度计时
来源：http://dga.zdqjudy.top

t = time.perf_counter()
来源：http://zcj.vehdjk.com

[U16] Py：命令行参数解析
来源：http://cku.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rjr.pengpengdd.cyou

[U17] Py：初始化日志
来源：http://xgr.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://hqt.havefunace.top

[U18] Py：预编译正则
来源：http://yvu.yonumen.top

pat = re.compile(r"\d+")
来源：http://svz.zdqjudy.top

[U19] Py：正则替换带回调
来源：http://haz.bjfxy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tht.ydjk.org.cn

[U20] Py：缓存函数结果
来源：http://msy.hysaishi.cn

@functools.lru_cache(maxsize=None)
来源：http://qqt.sweek.top

[U21] Py：自定义上下文管理器
来源：http://hnd.xingfuxueyuan.xyz

@contextlib.contextmanager
来源：http://dtp.yvedp.cn

[U22] Py：矩阵转置
来源：http://ejk.aizwys.cn

list(zip(*m))
来源：http://vrn.shanyushiyangkeji.top

[U23] Py：分块读取大文件
来源：http://ste.xylfe.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jss.daria6918.cn

[U24] Py：路径操作
来源：http://kmm.iojbl.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ynj.cqqwz.cn

[U25] Py：CSV 按字典读
来源：http://jnk.yvedp.cn

csv.DictReader(f)
来源：http://yci.hysaishi.cn

[U26] Py：并发下载
来源：http://oic.jinghuilouyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cid.c1oappe.top

[U27] Py：异步 HTTP
来源：http://abw.52xcode.cn

aiohttp.ClientSession() 配合 async with
来源：http://eqt.yueranfly.top

[U28] Py：类型别名
来源：http://iry.yfazqb.com

UserId = int
来源：http://mjt.shzxlz.cn

[U29] Py：属性校验
来源：http://jbd.yj20258888.top

@property 与 @x.setter 配合
来源：http://fjq.cqqwz.cn

[U30] Py：数据类
来源：http://ake.yonumen.top

@dataclass(slots=True)
来源：http://gzx.vqdsnc.cn

[U31] Py：单测
来源：http://rqc.gogol.net.cn

python -m pytest -q
来源：http://rxw.9152youxi.cn

[U32] Py：代码格式化
来源：http://icz.nanxuanxn.top

ruff format . && ruff check --fix .
来源：http://vdl.shangyingyoupin.top

[U33] Py：打包发布
来源：http://oth.sufxvd.cn

python -m build  （依赖 pyproject.toml）
来源：http://dmp.tian-w.cn

[U34] Py：判断编码
来源：http://dhm.daxiang520.top

chardet.detect(raw)
来源：http://umn.cheryme.top

[U35] Py：发送邮件
来源：http://fpo.jlsjyb.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ybd.yonumen.top

[U36] Py：定时任务
来源：http://fzk.jinghuilouyu.cn

schedule.every(10).minutes.do(job)
来源：http://mtc.c1oappe.top

[U37] Py：读写 Excel
来源：http://eyn.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://qgm.hfpthk.cn

[U38] Py：获取脚本所在目录
来源：http://ihl.0kj1m.cn

Path(__file__).resolve().parent
来源：http://xhd.hysaishi.cn

[U39] Py：判断是否在交互环境
来源：http://pjc.9152youxi.cn

sys.stdout.isatty()
来源：http://igh.hywenlv.cn

[U40] Py：打印到标准错误
来源：http://wew.hnxiangtu.top

print("err", file=sys.stderr)
来源：http://gps.fehbvm.com

[U41] PHP：初始化 Composer 项目
来源：http://yos.ivvv.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zmb.zdbjq.cn

[U42] PHP：PSR-4 自动加载
来源：http://jec.hnxiangtu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bzu.cashguo.top

[U43] PHP：声明命名空间
来源：http://zka.yueranfly.top

namespace App\Http;
来源：http://vit.fengsongda.top

[U44] PHP：开启严格类型
来源：http://csj.ybcxt.top

declare(strict_types=1);
来源：http://wgn.shangyingyoupin.top

[U45] PHP：类型声明与返回类型
来源：http://opl.jinqigfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fnm.sxryk.cn

[U46] PHP：可空类型
来源：http://efe.ppjwa.cn

?string $name = null
来源：http://lvu.tanke756.top

[U47] PHP：联合类型
来源：http://eku.daxiang520.top

int|string $id
来源：http://abu.chenjidiqi.icu

[U48] PHP：纯枚举
来源：http://xna.zhaomingkeji.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fuu.hfpthk.cn

[U49] PHP：只读属性
来源：http://ejd.ivvv.top

public readonly string $name
来源：http://ybv.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://lhl.zhaomingkeji.xyz

public function __construct(private int $id) {}
来源：http://zgx.fktsv.cn

[U51] PHP：数组解构
来源：http://xtg.sxryk.cn

[$a, $b] = $arr;
来源：http://sfh.pycfn.com

[U52] PHP：箭头函数
来源：http://giy.shuidangran.top

$double = fn($x) => $x * 2;
来源：http://xwk.daria6918.cn

[U53] PHP：空合并运算符
来源：http://beg.shangyingyoupin.top

$v = $a ?? $b ?? "default";
来源：http://npp.dianchejie.cn

[U54] PHP：空安全调用
来源：http://lid.guowangkeji.top

$obj?->method()
来源：http://fwk.c1oappe.top

[U55] PHP：match 表达式
来源：http://czl.vqdsnc.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sac.aizwys.cn

[U56] PHP：命名参数
来源：http://ltg.yongpay.top

f(a: 1, b: 2)
来源：http://ppy.guowangkeji.top

[U57] PHP：字符串插值
来源：http://nff.hongshengwenyu.top

"值: {$a}"
来源：http://bft.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://gvj.svipenyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dap.ivvv.top

[U59] PHP：自定义排序
来源：http://etz.xingfuxueyuan.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vet.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://saw.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fqi.zhengqikj.top

[U61] PHP：正则
来源：http://jhd.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ewj.nanxuanxn.top

[U62] PHP：日期对象
来源：http://llx.gogol.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kiu.ydjk.org.cn

[U63] PHP：文件读写
来源：http://klx.cdnleiting.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://twq.ywan-chungtsiang.top

[U64] PHP：目录遍历
来源：http://ouy.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://uym.xziqi.cn

[U65] PHP：会话
来源：http://bly.yongpay.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vjh.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://dql.chenzaomai.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zjz.cdnleiting.top

[U67] PHP：处理文件上传
来源：http://unf.fehbvm.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tbd.yuanzhike.top

[U68] PHP：PDO 连接
来源：http://bnb.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hbn.nanxinkj.top

[U69] PHP：PDO 预处理
来源：http://arx.shangyingyoupin.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mhs.cheryme.top

[U70] PHP：PDO 事务
来源：http://snm.bjfxy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tww.aibaodan.cn

[U71] PHP：抛出异常
来源：http://hoo.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://taf.yonumen.top

[U72] PHP：写错误日志
来源：http://bhm.sjlbkw.cn

error_log("失败: " . $e->getMessage());
来源：http://rcq.xuanzx.com

[U73] PHP：读取 ini 配置
来源：http://lke.0kj1m.cn

parse_ini_file("config.ini", true)
来源：http://vvg.bjfxy.top

[U74] PHP：读取环境变量
来源：http://jiu.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://zbp.ehwqpu.com

[U75] PHP：依赖注入
来源：http://zoc.sxryk.cn

composer require psr/container
来源：http://wva.svipenyu.cn

[U76] PHP：简单路由
来源：http://lxb.hnxiangtu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lld.hysaishi.cn

[U77] PHP：模板渲染
来源：http://xyq.ctjpmb.com

composer require twig/twig
来源：http://bhi.tarul.cn

[U78] PHP：单元测试
来源：http://oeb.jiagoushi.top

composer require --dev phpunit/phpunit
来源：http://jnl.jinyuanbaomall.cn

[U79] PHP：静态分析
来源：http://mrq.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://drv.guowangkeji.top

[U80] PHP：代码规范修复
来源：http://icv.hysaishi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qsi.yfazqb.com

[U81] JS：初始化项目
来源：http://qzc.yuanzhike.top

npm init -y;  npm i express
来源：http://yoj.tarul.cn

[U82] JS：package.json 脚本
来源：http://dum.hfpthk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dqo.ehwqpu.com

[U83] JS：ES Module 导入导出
来源：http://ycb.epnwcf.com

export const a = 1;  import { a } from "./m.js";
来源：http://tla.zdqjudy.top

[U84] JS：CommonJS 写法
来源：http://ocj.tian-w.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fgk.yj20258.top

[U85] JS：可选链
来源：http://lue.jyoumei.cn

a?.b?.c
来源：http://maq.yongpay.top

[U86] JS：空值合并
来源：http://vko.yanxiufei.cn

a ?? b
来源：http://ndz.kuanghao11.cn

[U87] JS：解构默认值
来源：http://hre.yfazqb.com

const { a = 1, b = 2 } = obj;
来源：http://zkr.ehwqpu.com

[U88] JS：对象展开合并
来源：http://hqf.bjfxy.top

{ ...a, ...b }
来源：http://xpv.tanke756.top

[U89] JS：数组去重
来源：http://jjv.zhengqikj.top

[...new Set(arr)]
来源：http://jds.hcnkem.com

[U90] JS：数字数组排序
来源：http://zng.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://die.zhengqikj.top

[U91] JS：对象键值遍历
来源：http://ahk.fehbvm.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lal.gotoacloud.top

[U92] JS：深拷贝
来源：http://ipu.vqdsnc.cn

structuredClone(obj)
来源：http://mkc.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://xvu.quarkkingdee.top

`共 ${n} 条`
来源：http://tzu.redwolf501.top

[U94] JS：箭头函数
来源：http://kqd.52xcode.cn

const double = x => x * 2;
来源：http://bfk.kuanghao11.cn

[U95] JS：Promise 包装
来源：http://lzs.hysaishi.cn

new Promise((resolve, reject) => {})
来源：http://fql.ybcxt.top

[U96] JS：async/await 与异常
来源：http://thl.fanxiaobao.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wqy.cqqwz.cn

[U97] JS：并发请求
来源：http://djs.svipenyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qun.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://nwq.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mlr.wangshuangyany.cn

[U99] JS：事件监听
来源：http://nlb.fehbvm.com

el.addEventListener("click", e => {})
来源：http://ogg.zycfv.cn

[U100] JS：DOM 查询
来源：http://fti.yongpay.top

document.querySelector(".item")
来源：http://xsw.sysykeji.top

[U101] JS：classList 操作
来源：http://bmk.jqgfzy.top

el.classList.toggle("active")
来源：http://zrr.kuanghao11.cn

[U102] JS：本地存储
来源：http://zqy.hammf.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kfz.fehbvm.com

[U103] JS：定时器
来源：http://gfk.ywan-chungtsiang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bxs.jianghu66.top

[U104] JS：防抖
来源：http://ypl.havefunace.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mqj.pycfn.com

[U105] JS：节流
来源：http://wqv.cqqwz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jqj.zycfv.cn

[U106] JS：日期格式化
来源：http://erd.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://him.hnqzz.top

[U107] JS：数字千分位
来源：http://ohc.chenzaomai.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zff.nanxuanxn.top

[U108] JS：随机整数
来源：http://ysc.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bwn.guowangkeji.top

[U109] JS：数组分组
来源：http://kvo.hnxiangtu.top

Object.groupBy(arr, x => x.type)
来源：http://fgi.andypj.xyz

[U110] JS：数组分块
来源：http://yfw.epnwcf.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wqp.yj20258.top

[U111] JS：对象转 Map
来源：http://ijv.guannengcc.top

new Map(Object.entries(obj))
来源：http://uby.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://otd.hysaishi.cn

"7".padStart(3, "0")
来源：http://zgn.sweek.top

[U113] JS：正则替换全部
来源：http://aeq.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://jzt.vqdsnc.cn

[U114] JS：JSON 深比较
来源：http://yia.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rog.fehbvm.com

[U115] JS：生成 UUID
来源：http://ltq.hnqzz.top

crypto.randomUUID()
来源：http://zvj.cqqwz.cn

[U116] JS：类型检查（JSDoc）
来源：http://rnp.daria6918.cn

/** @param {string} name */ function f(name) {}
来源：http://qtp.yvedp.cn

[U117] JS：单元测试
来源：http://qwp.ydzc1.top

npm i -D vitest;  npx vitest
来源：http://khk.vehdjk.com

[U118] JS：开发服务器
来源：http://zyr.uphjek.com

npm i -D vite;  npx vite
来源：http://wrd.xuanzx.com

[U119] JS：生产构建
来源：http://ffs.yongpay.top

npx vite build
来源：http://pfx.0kj1m.cn

[U120] JS：读取环境变量（Vite）
来源：http://fwt.ydzc1.top

import.meta.env.VITE_API_URL
来源：http://ccb.pengpengdd.cyou

================================================================================
来源：http://plb.ydzc1.top

统计汇总
来源：http://hrt.zhaomingkeji.xyz

================================================================================
来源：http://yeu.snrcjt.cn

按语言统计（条）：
来源：http://ckx.jqgufenzy.top

Python ......... 252
来源：http://aeu.yueranfly.top

PHP ............ 252
来源：http://nhd.iojbl.cn

JavaScript ..... 252
来源：http://ltc.dashuyun.cn

TypeScript ..... 212
来源：http://cxx.ivvv.top

Java ........... 212
来源：http://fbx.c1oappe.top

Go ............. 212
来源：http://irk.sxryk.cn

Ruby ........... 212
来源：http://utk.0kj1m.cn

C# ............. 212
来源：http://hzu.andypj.xyz

C .............. 30
来源：http://fbq.iojbl.cn

C++ ............ 30
来源：http://zge.aibaodan.cn

SQL ............ 90
来源：http://jdr.redwolf501.top

Bash ........... 80
来源：http://kjw.aizwys.cn

Kotlin ......... 15
来源：http://byd.epnwcf.com

Swift .......... 15
来源：http://jqj.birdmap.top

Lua ............ 10
来源：http://kkc.redwolf501.top

Perl ........... 10
来源：http://mlv.jlsjyb.cn

Scala .......... 10
来源：http://cgp.xuanzx.com

------------------------------------
来源：http://ztq.shanyushiyangtech.top

合计 ........... 2106 条
来源：http://wuz.nanxinkj.top

按章节统计：
来源：http://mjc.sweek.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pdk.jqgufenzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mgr.svipenyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ofq.dianchejie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ylu.redwolf501.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zob.quarkkingdee.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pth.haohaochexian.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ogk.cqqwz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://smj.sxryk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ckz.hywenlv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fen.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pyx.xinyue.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ztt.tianlin.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oey.jinqigfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ztc.sysykeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bbj.shanyushiyangkeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vgt.hongshengwenyu.top

Q SQL 专题                              90
来源：http://qsg.jiagoushi.top

R Bash 专题                             80
来源：http://bve.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://tbm.ydjk.org.cn

T 其他语言补充                          60
来源：http://nkz.chenzaomai.com

U 高频实用片段                         120
来源：http://bze.kuanghao11.cn

------------------------------------
来源：http://mxb.jianghu66.top

合计                                  2106 条
来源：http://nrc.uphjek.com

--------------------------------------------------------------------------------
来源：http://tyn.jyoumei.cn

使用提醒
来源：http://ulb.nwbrower.top

--------------------------------------------------------------------------------
来源：http://tvl.sjlbkw.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tdj.haohaochexian.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://icl.epnwcf.com


<!-- 参考信息 -->