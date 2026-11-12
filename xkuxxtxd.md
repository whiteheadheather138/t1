代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://pay.c1oappe.top

[T59] Scala：循环
来源：http://rfy.ydjk.org.cn

for (i <- 1 to 10) println(i)
来源：http://hgf.iojbl.cn

[T60] Scala：折叠
来源：http://psz.zdqjudy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zlt.zhoulong.xyz

================================================================================
来源：http://zpe.shzxlz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rew.yueranfly.top

================================================================================
来源：http://owp.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://bwv.cqqwz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yvs.zhengqikj.top

[U02] Py：导出 / 安装依赖
来源：http://leu.gotoacloud.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gry.fengsongda.top

[U03] Py：加载 .env 配置
来源：http://otq.cucudq.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nyp.jqgfzy.top

[U04] Py：变量调试打印
来源：http://igx.zhiwuduotai.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mkn.meibo888.top

[U05] Py：列表去重且保序
来源：http://ezo.bbcook.cn

list(dict.fromkeys(arr))
来源：http://gmo.bjfxy.top

[U06] Py：合并两个字典
来源：http://aal.nanxuanxn.top

{**a, **b}
来源：http://zdc.c1oappe.top

[U07] Py：反转字典键值
来源：http://inq.jyoumei.cn

{v: k for k, v in d.items()}
来源：http://xgu.cqqwz.cn

[U08] Py：展平二维列表
来源：http://ual.birdmap.top

[y for x in nested for y in x]
来源：http://hgo.ydzc1.top

[U09] Py：字典取最大值的键
来源：http://psx.tian-w.cn

max(d, key=d.get)
来源：http://omk.cdnleiting.top

[U10] Py：按值排序字典
来源：http://koq.yonumen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tfx.dianchejie.cn

[U11] Py：生成器表达式
来源：http://xik.316326.xyz

(x * 2 for x in arr)
来源：http://yuy.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kay.mhx1999.top

Counter(arr).most_common(3)
来源：http://hoi.jinghuilouyu.cn

[U13] Py：固定长度队列
来源：http://tuk.fzhhl.top

deque(maxlen=10)
来源：http://ttp.jiagoushi.top

[U14] Py：分组收集到列表
来源：http://mxk.xziqi.cn

defaultdict(list)
来源：http://nyz.cdnleiting.top

[U15] Py：高精度计时
来源：http://lcl.meibo888.top

t = time.perf_counter()
来源：http://uyr.meibo888.top

[U16] Py：命令行参数解析
来源：http://zda.vqdsnc.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ldn.xuanzx.com

[U17] Py：初始化日志
来源：http://uup.ctjpmb.com

logging.basicConfig(level=logging.INFO)
来源：http://pij.tian-w.cn

[U18] Py：预编译正则
来源：http://dmy.zhijiandao.cn

pat = re.compile(r"\d+")
来源：http://qhn.bjfxy.top

[U19] Py：正则替换带回调
来源：http://rdk.zhengqikj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://amu.hongshengwenyu.top

[U20] Py：缓存函数结果
来源：http://mcy.ehwqpu.com

@functools.lru_cache(maxsize=None)
来源：http://hkg.xingfuxueyuan.xyz

[U21] Py：自定义上下文管理器
来源：http://lsl.xziqi.cn

@contextlib.contextmanager
来源：http://nws.nanxinkj.top

[U22] Py：矩阵转置
来源：http://wiw.zhengqikj.top

list(zip(*m))
来源：http://egx.chenlongwang.top

[U23] Py：分块读取大文件
来源：http://fmg.birdmap.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wkm.sjlbkw.cn

[U24] Py：路径操作
来源：http://qvs.xziqi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qko.mhx1999.top

[U25] Py：CSV 按字典读
来源：http://boi.ehwqpu.com

csv.DictReader(f)
来源：http://zca.zhijiandao.cn

[U26] Py：并发下载
来源：http://lql.jiagoushi.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://elo.ywan-chungtsiang.top

[U27] Py：异步 HTTP
来源：http://xqu.redwolf501.top

aiohttp.ClientSession() 配合 async with
来源：http://hxc.mhx1999.top

[U28] Py：类型别名
来源：http://cfa.uphjek.com

UserId = int
来源：http://euz.hfpthk.cn

[U29] Py：属性校验
来源：http://nrx.zhongyouzk.top

@property 与 @x.setter 配合
来源：http://yso.dashuyun.cn

[U30] Py：数据类
来源：http://ptz.jinqigfzy.top

@dataclass(slots=True)
来源：http://jsj.daria6918.cn

[U31] Py：单测
来源：http://uem.hfpthk.cn

python -m pytest -q
来源：http://umz.fzhhl.top

[U32] Py：代码格式化
来源：http://hbq.yuxming.cn

ruff format . && ruff check --fix .
来源：http://lkp.dianchejie.cn

[U33] Py：打包发布
来源：http://bdt.iojbl.cn

python -m build  （依赖 pyproject.toml）
来源：http://ekq.zhongyouzk.top

[U34] Py：判断编码
来源：http://qme.ydzc1.top

chardet.detect(raw)
来源：http://lae.andypj.xyz

[U35] Py：发送邮件
来源：http://npr.aizwys.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jyd.316326.xyz

[U36] Py：定时任务
来源：http://ymt.cheryme.top

schedule.every(10).minutes.do(job)
来源：http://dyd.nwbrower.top

[U37] Py：读写 Excel
来源：http://stp.nwbrower.top

pandas.read_excel / DataFrame.to_excel
来源：http://ucy.316326.xyz

[U38] Py：获取脚本所在目录
来源：http://mlo.fehbvm.com

Path(__file__).resolve().parent
来源：http://qog.ydjk.org.cn

[U39] Py：判断是否在交互环境
来源：http://zwm.iojbl.cn

sys.stdout.isatty()
来源：http://pec.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://hmu.svipenyu.cn

print("err", file=sys.stderr)
来源：http://gqx.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://skb.ivvv.top

composer init;  composer require guzzlehttp/guzzle
来源：http://art.shzxlz.cn

[U42] PHP：PSR-4 自动加载
来源：http://sku.zhixingplan.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kqv.nanxinkj.top

[U43] PHP：声明命名空间
来源：http://jfx.sxryk.cn

namespace App\Http;
来源：http://iev.c1oappe.top

[U44] PHP：开启严格类型
来源：http://nvz.jlsjyb.cn

declare(strict_types=1);
来源：http://avm.dianchejie.cn

[U45] PHP：类型声明与返回类型
来源：http://kwt.pycfn.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://tuq.xinyue.icu

[U46] PHP：可空类型
来源：http://yyh.yj202588.top

?string $name = null
来源：http://qnw.shuidangran.top

[U47] PHP：联合类型
来源：http://zog.jinghuilouyu.cn

int|string $id
来源：http://gti.52xcode.cn

[U48] PHP：纯枚举
来源：http://sgt.redwolf501.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gdw.tian-w.cn

[U49] PHP：只读属性
来源：http://zhv.guannengcc.top

public readonly string $name
来源：http://efo.jyoumei.cn

[U50] PHP：构造器属性提升
来源：http://nrw.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://eec.chenzaomai.com

[U51] PHP：数组解构
来源：http://rtl.zdqjudy.top

[$a, $b] = $arr;
来源：http://yqw.epnwcf.com

[U52] PHP：箭头函数
来源：http://pxz.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://svs.meibo888.top

[U53] PHP：空合并运算符
来源：http://cjq.yfazqb.com

$v = $a ?? $b ?? "default";
来源：http://izv.iojbl.cn

[U54] PHP：空安全调用
来源：http://tpq.xziqi.cn

$obj?->method()
来源：http://nlg.hongshengwenyu.top

[U55] PHP：match 表达式
来源：http://tav.0kj1m.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://reg.shanyushiyangkeji.top

[U56] PHP：命名参数
来源：http://tcv.guannengcc.top

f(a: 1, b: 2)
来源：http://xcd.yj202588.top

[U57] PHP：字符串插值
来源：http://efk.jqgfzy.top

"值: {$a}"
来源：http://pto.jqgufenzy.top

[U58] PHP：数组三件套
来源：http://rlt.gaohongyu789.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ecm.hnqzz.top

[U59] PHP：自定义排序
来源：http://vuq.ehwqpu.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uyb.bbcook.cn

[U60] PHP：JSON 编解码
来源：http://csl.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zbf.jlsjyb.cn

[U61] PHP：正则
来源：http://kkn.shangyingyoupin.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ost.sysykeji.top

[U62] PHP：日期对象
来源：http://pen.yfazqb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rfl.wangdashe.top

[U63] PHP：文件读写
来源：http://avp.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yko.yongpay.top

[U64] PHP：目录遍历
来源：http://iwb.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://xti.yongpay.top

[U65] PHP：会话
来源：http://ktq.fanxiaobao.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://zyu.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://qqb.dashuyun.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eeo.ydjk.org.cn

[U67] PHP：处理文件上传
来源：http://jha.jianghu66.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://izw.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://loh.sjlbkw.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xjz.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://aey.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nis.hnxiangtu.top

[U70] PHP：PDO 事务
来源：http://bya.c1oappe.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fkf.guowangkeji.top

[U71] PHP：抛出异常
来源：http://hdu.snrcjt.cn

throw new RuntimeException("失败", 500);
来源：http://oeh.cdnleiting.top

[U72] PHP：写错误日志
来源：http://hsz.ivvv.top

error_log("失败: " . $e->getMessage());
来源：http://opr.zdqjudy.top

[U73] PHP：读取 ini 配置
来源：http://yvc.fanxiaobao.xyz

parse_ini_file("config.ini", true)
来源：http://ptu.zhongyouzk.top

[U74] PHP：读取环境变量
来源：http://klj.hfpthk.cn

getenv("APP_ENV") ?: "production"
来源：http://qub.jianghu66.top

[U75] PHP：依赖注入
来源：http://kgt.chenzaomai.com

composer require psr/container
来源：http://amk.fengsongda.top

[U76] PHP：简单路由
来源：http://mlb.52xcode.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ats.ehwqpu.com

[U77] PHP：模板渲染
来源：http://dkg.andypj.xyz

composer require twig/twig
来源：http://qhz.hongshengwenyu.top

[U78] PHP：单元测试
来源：http://nvh.nanxuanxn.top

composer require --dev phpunit/phpunit
来源：http://wkm.zycfv.cn

[U79] PHP：静态分析
来源：http://yoz.dianchejie.cn

composer require --dev phpstan/phpstan
来源：http://zzt.hongshengwenyu.top

[U80] PHP：代码规范修复
来源：http://svy.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://scn.sysykeji.top

[U81] JS：初始化项目
来源：http://ixq.meibo888.top

npm init -y;  npm i express
来源：http://yne.hcnkem.com

[U82] JS：package.json 脚本
来源：http://jjr.xylfe.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://asy.snrcjt.cn

[U83] JS：ES Module 导入导出
来源：http://qdd.hongshengwenyu.top

export const a = 1;  import { a } from "./m.js";
来源：http://yag.yonumen.top

[U84] JS：CommonJS 写法
来源：http://ftb.9152youxi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ksm.xziqi.cn

[U85] JS：可选链
来源：http://yrg.fanxiaobao.xyz

a?.b?.c
来源：http://ynf.yongpay.top

[U86] JS：空值合并
来源：http://bau.sufxvd.cn

a ?? b
来源：http://gzl.cdnleiting.top

[U87] JS：解构默认值
来源：http://usc.aizwys.cn

const { a = 1, b = 2 } = obj;
来源：http://zqp.xuanzx.com

[U88] JS：对象展开合并
来源：http://vhv.sxryk.cn

{ ...a, ...b }
来源：http://isr.shzxlz.cn

[U89] JS：数组去重
来源：http://vdw.ybcxt.top

[...new Set(arr)]
来源：http://gwk.hammf.cn

[U90] JS：数字数组排序
来源：http://knt.zhongyouzk.top

[...arr].sort((a, b) => a - b)
来源：http://tce.shanyushiyangkeji.top

[U91] JS：对象键值遍历
来源：http://oas.yonumen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pzs.vqdsnc.cn

[U92] JS：深拷贝
来源：http://juy.kuanghao11.cn

structuredClone(obj)
来源：http://ggo.xuanzx.com

[U93] JS：模板字符串
来源：http://mvf.xylfe.cn

`共 ${n} 条`
来源：http://imi.tanke756.top

[U94] JS：箭头函数
来源：http://ard.birdmap.top

const double = x => x * 2;
来源：http://bev.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://hpn.daria6918.cn

new Promise((resolve, reject) => {})
来源：http://vro.guowangkeji.top

[U96] JS：async/await 与异常
来源：http://amu.gogol.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ahr.nwbrower.top

[U97] JS：并发请求
来源：http://oxp.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ure.aibaodan.cn

[U98] JS：fetch 带 JSON
来源：http://yxz.svipenyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xwn.yj20258.top

[U99] JS：事件监听
来源：http://slb.zhixingplan.top

el.addEventListener("click", e => {})
来源：http://wfw.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://udi.daxiang520.top

document.querySelector(".item")
来源：http://dls.hammf.cn

[U101] JS：classList 操作
来源：http://lml.zhongyouzk.top

el.classList.toggle("active")
来源：http://lzi.bbcook.cn

[U102] JS：本地存储
来源：http://msg.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rlt.cashguo.top

[U103] JS：定时器
来源：http://beh.andypj.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yze.yfazqb.com

[U104] JS：防抖
来源：http://rft.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hmg.svipenyu.cn

[U105] JS：节流
来源：http://sfm.wangdashe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lpn.snrcjt.cn

[U106] JS：日期格式化
来源：http://hen.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://clj.ydzc1.top

[U107] JS：数字千分位
来源：http://zrh.ppjwa.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fus.ctjpmb.com

[U108] JS：随机整数
来源：http://zby.feifeiyinyue.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qrr.cqqwz.cn

[U109] JS：数组分组
来源：http://kvv.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://whm.xziqi.cn

[U110] JS：数组分块
来源：http://hhe.jqgfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://omb.tarul.cn

[U111] JS：对象转 Map
来源：http://esb.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://mar.jyoumei.cn

[U112] JS：字符串补位
来源：http://xro.yj202588.top

"7".padStart(3, "0")
来源：http://oyl.jinqigufen.top

[U113] JS：正则替换全部
来源：http://grt.hongshengwenyu.top

s.replaceAll("a", "b")
来源：http://imy.jinyuanbaomall.cn

[U114] JS：JSON 深比较
来源：http://pho.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bcv.yonumen.top

[U115] JS：生成 UUID
来源：http://pel.yongpay.top

crypto.randomUUID()
来源：http://ttg.bjfxy.top

[U116] JS：类型检查（JSDoc）
来源：http://fiy.bbcook.cn

/** @param {string} name */ function f(name) {}
来源：http://fua.yueranfly.top

[U117] JS：单元测试
来源：http://xju.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://kak.yvedp.cn

[U118] JS：开发服务器
来源：http://vpy.andypj.xyz

npm i -D vite;  npx vite
来源：http://tlf.jyoumei.cn

[U119] JS：生产构建
来源：http://zbt.cdnleiting.top

npx vite build
来源：http://wrz.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://uvn.mhx1999.top

import.meta.env.VITE_API_URL
来源：http://pdr.tarul.cn

================================================================================
来源：http://dch.tianlin.xyz

统计汇总
来源：http://szg.redwolf501.top

================================================================================
来源：http://nuh.redwolf501.top

按语言统计（条）：
来源：http://gck.tian-w.cn

Python ......... 252
来源：http://mnf.daria6918.cn

PHP ............ 252
来源：http://qej.smart0.xyz

JavaScript ..... 252
来源：http://egk.cdnleiting.top

TypeScript ..... 212
来源：http://rkr.shzxlz.cn

Java ........... 212
来源：http://byr.ywan-chungtsiang.top

Go ............. 212
来源：http://hmd.yueranfly.top

Ruby ........... 212
来源：http://xqf.shangyingyoupin.top

C# ............. 212
来源：http://oxz.tian-w.cn

C .............. 30
来源：http://seh.mhx1999.top

C++ ............ 30
来源：http://sia.daria6918.cn

SQL ............ 90
来源：http://cwh.xylfe.cn

Bash ........... 80
来源：http://wdb.cdnleiting.top

Kotlin ......... 15
来源：http://bxw.shanyushiyangkeji.top

Swift .......... 15
来源：http://ayw.yueranfly.top

Lua ............ 10
来源：http://tlp.smart0.xyz

Perl ........... 10
来源：http://coh.nanxinkj.top

Scala .......... 10
来源：http://qmr.ydjk.org.cn

------------------------------------
来源：http://mgw.sxryk.cn

合计 ........... 2106 条
来源：http://whz.jinyuanbaomall.cn

按章节统计：
来源：http://lmh.gotoacloud.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zcs.zycfv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gmq.yuxming.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vza.sysykeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://syc.fanxiaobao.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jqc.vqdsnc.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pqd.yfazqb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zkj.yj20258888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kuo.shanyushiyangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mfk.hammf.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pxe.wangdashe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mkl.jianghu66.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rek.nwbrower.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kve.aibaodan.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xan.dashuyun.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://con.zhoulong.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kjt.hnxiangtu.top

Q SQL 专题                              90
来源：http://kgq.jinghuilouyu.cn

R Bash 专题                             80
来源：http://ywn.tarul.cn

S C / C++ 专题                          60
来源：http://wus.jlsjyb.cn

T 其他语言补充                          60
来源：http://ayj.feifeiyinyue.top

U 高频实用片段                         120
来源：http://ibz.yuanzhike.top

------------------------------------
来源：http://btl.ywan-chungtsiang.top

合计                                  2106 条
来源：http://hje.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://dfi.hnxiangtu.top

使用提醒
来源：http://vfn.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://jww.vqdsnc.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hpn.hesvh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fnw.gotoacloud.top


<!-- 参考信息 -->