代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://xfu.wangdashe.top

[T59] Scala：循环
来源：http://wsu.hongshengwenyu.top

for (i <- 1 to 10) println(i)
来源：http://vuy.hysaishi.cn

[T60] Scala：折叠
来源：http://brq.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hbm.hfpthk.cn

================================================================================
来源：http://kcs.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uii.andypj.xyz

================================================================================
来源：http://eqk.andypj.xyz

[U01] Py：创建虚拟环境
来源：http://mzg.yongpay.top

python -m venv .venv && source .venv/bin/activate
来源：http://dmu.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://mpa.yvedp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://alx.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://qdc.zhoulong.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://xtv.ctjpmb.com

[U04] Py：变量调试打印
来源：http://gre.bjfxy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kbh.52xcode.cn

[U05] Py：列表去重且保序
来源：http://ecy.ybcxt.top

list(dict.fromkeys(arr))
来源：http://aoo.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://fmy.tian-w.cn

{**a, **b}
来源：http://vco.ydjk.org.cn

[U07] Py：反转字典键值
来源：http://zvx.jinqigfzy.top

{v: k for k, v in d.items()}
来源：http://uuq.ctjpmb.com

[U08] Py：展平二维列表
来源：http://quh.yj20258.top

[y for x in nested for y in x]
来源：http://ppq.zycfv.cn

[U09] Py：字典取最大值的键
来源：http://ktd.birdmap.top

max(d, key=d.get)
来源：http://umf.jyoumei.cn

[U10] Py：按值排序字典
来源：http://gkk.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jal.fehbvm.com

[U11] Py：生成器表达式
来源：http://dgh.tian-w.cn

(x * 2 for x in arr)
来源：http://bql.cheryme.top

[U12] Py：取出现最多的 3 个元素
来源：http://zks.shangyingyoupin.top

Counter(arr).most_common(3)
来源：http://ath.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://xva.bjfxy.top

deque(maxlen=10)
来源：http://jfm.jqgufenzy.top

[U14] Py：分组收集到列表
来源：http://kxd.yj20258.top

defaultdict(list)
来源：http://ybn.yj20258.top

[U15] Py：高精度计时
来源：http://aqz.quarkkingdee.top

t = time.perf_counter()
来源：http://jib.bjfxy.top

[U16] Py：命令行参数解析
来源：http://els.bbcook.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yxn.52xcode.cn

[U17] Py：初始化日志
来源：http://lhy.xylfe.cn

logging.basicConfig(level=logging.INFO)
来源：http://ngh.zhixingplan.top

[U18] Py：预编译正则
来源：http://pcf.cashguo.top

pat = re.compile(r"\d+")
来源：http://efi.tian-w.cn

[U19] Py：正则替换带回调
来源：http://jom.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hzd.yuanzhike.top

[U20] Py：缓存函数结果
来源：http://kwm.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://iib.fanxiaobao.xyz

[U21] Py：自定义上下文管理器
来源：http://kfy.smart0.xyz

@contextlib.contextmanager
来源：http://spq.redwolf501.top

[U22] Py：矩阵转置
来源：http://zcq.xuetiantiany.cn

list(zip(*m))
来源：http://uqs.iojbl.cn

[U23] Py：分块读取大文件
来源：http://ond.uphjek.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://txi.yanxiufei.cn

[U24] Py：路径操作
来源：http://fjc.yueranfly.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tae.yj202588.top

[U25] Py：CSV 按字典读
来源：http://qap.sweek.top

csv.DictReader(f)
来源：http://tos.yfazqb.com

[U26] Py：并发下载
来源：http://vrw.nanxuanxn.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rhh.tarul.cn

[U27] Py：异步 HTTP
来源：http://gae.jlsjyb.cn

aiohttp.ClientSession() 配合 async with
来源：http://que.kuanghao11.cn

[U28] Py：类型别名
来源：http://ouk.yonumen.top

UserId = int
来源：http://mwo.hesvh.cn

[U29] Py：属性校验
来源：http://exm.yvedp.cn

@property 与 @x.setter 配合
来源：http://wpz.nanxinkj.top

[U30] Py：数据类
来源：http://btc.yanxiufei.cn

@dataclass(slots=True)
来源：http://ydn.jinghuilouyu.cn

[U31] Py：单测
来源：http://bbd.fzhhl.top

python -m pytest -q
来源：http://ppg.shangyingyoupin.top

[U32] Py：代码格式化
来源：http://ycn.jinghuilouyu.cn

ruff format . && ruff check --fix .
来源：http://tij.vqdsnc.cn

[U33] Py：打包发布
来源：http://ywo.daria6918.cn

python -m build  （依赖 pyproject.toml）
来源：http://oxd.zhiwuduotai.top

[U34] Py：判断编码
来源：http://ujt.hongshengwenyu.top

chardet.detect(raw)
来源：http://leg.smart0.xyz

[U35] Py：发送邮件
来源：http://rlx.tian-w.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://khi.fengsongda.top

[U36] Py：定时任务
来源：http://chj.wangshuangyany.cn

schedule.every(10).minutes.do(job)
来源：http://rfc.tarul.cn

[U37] Py：读写 Excel
来源：http://hkm.cdnleiting.top

pandas.read_excel / DataFrame.to_excel
来源：http://ixd.yj20258.top

[U38] Py：获取脚本所在目录
来源：http://myo.yuanzhike.top

Path(__file__).resolve().parent
来源：http://bvw.yuanzhike.top

[U39] Py：判断是否在交互环境
来源：http://epb.jinqigfzy.top

sys.stdout.isatty()
来源：http://htz.shanyushiyangkeji.top

[U40] Py：打印到标准错误
来源：http://xkv.ppjwa.cn

print("err", file=sys.stderr)
来源：http://dks.aibaodan.cn

[U41] PHP：初始化 Composer 项目
来源：http://xnj.cucudq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nhw.yangfankeji.com

[U42] PHP：PSR-4 自动加载
来源：http://lmq.xuanzx.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ixc.gogol.net.cn

[U43] PHP：声明命名空间
来源：http://cha.uphjek.com

namespace App\Http;
来源：http://ucp.meibo888.top

[U44] PHP：开启严格类型
来源：http://dur.hammf.cn

declare(strict_types=1);
来源：http://klz.xziqi.cn

[U45] PHP：类型声明与返回类型
来源：http://efr.nanxuanxn.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rrq.smart0.xyz

[U46] PHP：可空类型
来源：http://ksa.daria6918.cn

?string $name = null
来源：http://xxa.shzxlz.cn

[U47] PHP：联合类型
来源：http://wcg.vehdjk.com

int|string $id
来源：http://gra.jianghu66.top

[U48] PHP：纯枚举
来源：http://rmv.52xcode.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vrw.smart0.xyz

[U49] PHP：只读属性
来源：http://rfi.tarul.cn

public readonly string $name
来源：http://mty.ydzc1.top

[U50] PHP：构造器属性提升
来源：http://wlg.hongshengwenyu.top

public function __construct(private int $id) {}
来源：http://sio.ydzc1.top

[U51] PHP：数组解构
来源：http://sar.gaohongyu789.top

[$a, $b] = $arr;
来源：http://ldh.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://ylr.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://ccs.52xcode.cn

[U53] PHP：空合并运算符
来源：http://dun.jiagoushi.top

$v = $a ?? $b ?? "default";
来源：http://ggr.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://kep.jinqigfzy.top

$obj?->method()
来源：http://pbs.zhongyouzk.top

[U55] PHP：match 表达式
来源：http://wgn.ppjwa.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kpz.uphjek.com

[U56] PHP：命名参数
来源：http://oqa.ywan-chungtsiang.top

f(a: 1, b: 2)
来源：http://rpu.smart0.xyz

[U57] PHP：字符串插值
来源：http://spa.feifeiyinyue.top

"值: {$a}"
来源：http://pyc.uphjek.com

[U58] PHP：数组三件套
来源：http://wla.dianchejie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hoe.hfpthk.cn

[U59] PHP：自定义排序
来源：http://icq.sysykeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vwc.sufxvd.cn

[U60] PHP：JSON 编解码
来源：http://chl.zycfv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bpp.hcnkem.com

[U61] PHP：正则
来源：http://dqb.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cyu.yongpay.top

[U62] PHP：日期对象
来源：http://fni.fengsongda.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xot.svipenyu.cn

[U63] PHP：文件读写
来源：http://gzp.aibaodan.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rsd.dashuyun.cn

[U64] PHP：目录遍历
来源：http://mrp.hongshengwenyu.top

glob("dir/*.php");  scandir("dir");
来源：http://xui.hywenlv.cn

[U65] PHP：会话
来源：http://xvu.kuanghao11.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rza.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://kez.jinqigfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rno.feifeiyinyue.top

[U67] PHP：处理文件上传
来源：http://vaq.dianchejie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rrq.uphjek.com

[U68] PHP：PDO 连接
来源：http://zju.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://egs.hywenlv.cn

[U69] PHP：PDO 预处理
来源：http://hzb.shangyingyoupin.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hvp.gotoacloud.top

[U70] PHP：PDO 事务
来源：http://dut.redwolf501.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qen.zhongyouzk.top

[U71] PHP：抛出异常
来源：http://kjp.svipenyu.cn

throw new RuntimeException("失败", 500);
来源：http://wle.yvedp.cn

[U72] PHP：写错误日志
来源：http://oys.shuidangran.top

error_log("失败: " . $e->getMessage());
来源：http://lhq.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://qcu.yongpay.top

parse_ini_file("config.ini", true)
来源：http://sjs.vqdsnc.cn

[U74] PHP：读取环境变量
来源：http://hmz.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://imh.aibaodan.cn

[U75] PHP：依赖注入
来源：http://ule.9152youxi.cn

composer require psr/container
来源：http://nwu.fktsv.cn

[U76] PHP：简单路由
来源：http://abv.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xtu.sufxvd.cn

[U77] PHP：模板渲染
来源：http://mpy.zdbjq.cn

composer require twig/twig
来源：http://qfh.sweek.top

[U78] PHP：单元测试
来源：http://eza.hammf.cn

composer require --dev phpunit/phpunit
来源：http://nzs.yongpay.top

[U79] PHP：静态分析
来源：http://wwn.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://vup.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://qhh.jinqigfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://epb.fzhhl.top

[U81] JS：初始化项目
来源：http://gmu.gzhubu.top

npm init -y;  npm i express
来源：http://fpi.ywan-chungtsiang.top

[U82] JS：package.json 脚本
来源：http://yiv.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fsf.vqdsnc.cn

[U83] JS：ES Module 导入导出
来源：http://nhi.jqgufenzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://wpc.pengpengdd.cyou

[U84] JS：CommonJS 写法
来源：http://ovw.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://lot.haohaochexian.top

[U85] JS：可选链
来源：http://nlr.chenlongwang.top

a?.b?.c
来源：http://ysm.gzhubu.top

[U86] JS：空值合并
来源：http://ljb.bjfxy.top

a ?? b
来源：http://pod.chenlongwang.top

[U87] JS：解构默认值
来源：http://ajv.yvedp.cn

const { a = 1, b = 2 } = obj;
来源：http://qso.nwbrower.top

[U88] JS：对象展开合并
来源：http://wyg.havefunace.top

{ ...a, ...b }
来源：http://qed.nanxuanxn.top

[U89] JS：数组去重
来源：http://kjp.feifeiyinyue.top

[...new Set(arr)]
来源：http://dnd.cqqwz.cn

[U90] JS：数字数组排序
来源：http://kjp.andypj.xyz

[...arr].sort((a, b) => a - b)
来源：http://ldi.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://wrx.daxiang520.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wgk.hnxiangtu.top

[U92] JS：深拷贝
来源：http://hdk.mhx1999.top

structuredClone(obj)
来源：http://gcm.ehwqpu.com

[U93] JS：模板字符串
来源：http://sle.9152youxi.cn

`共 ${n} 条`
来源：http://tuy.yfazqb.com

[U94] JS：箭头函数
来源：http://plu.tanke756.top

const double = x => x * 2;
来源：http://lla.zdqjudy.top

[U95] JS：Promise 包装
来源：http://elp.gzhubu.top

new Promise((resolve, reject) => {})
来源：http://zjc.kuanghao11.cn

[U96] JS：async/await 与异常
来源：http://wmp.cheryme.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pwn.jinghuilouyu.cn

[U97] JS：并发请求
来源：http://jff.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://pwm.yanxiufei.cn

[U98] JS：fetch 带 JSON
来源：http://hbq.redwolf501.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ion.guowangkeji.top

[U99] JS：事件监听
来源：http://uok.fktsv.cn

el.addEventListener("click", e => {})
来源：http://kul.xinyue.icu

[U100] JS：DOM 查询
来源：http://icc.vehdjk.com

document.querySelector(".item")
来源：http://hbj.yfazqb.com

[U101] JS：classList 操作
来源：http://iqt.zhongyouzk.top

el.classList.toggle("active")
来源：http://kby.yj20258888.top

[U102] JS：本地存储
来源：http://xik.epnwcf.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://nvf.tianlin.xyz

[U103] JS：定时器
来源：http://khw.quarkkingdee.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ejr.quarkkingdee.top

[U104] JS：防抖
来源：http://aat.zhoulong.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yjm.cdnleiting.top

[U105] JS：节流
来源：http://dll.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xey.hnxiangtu.top

[U106] JS：日期格式化
来源：http://yci.havefunace.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zjp.shanyushiyangtech.top

[U107] JS：数字千分位
来源：http://ttm.fzhhl.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://okm.xuetiantiany.cn

[U108] JS：随机整数
来源：http://ggs.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kwf.wangdashe.top

[U109] JS：数组分组
来源：http://fpi.guowangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://cnk.epnwcf.com

[U110] JS：数组分块
来源：http://wnw.ehwqpu.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yal.jqgfzy.top

[U111] JS：对象转 Map
来源：http://mdl.hcnkem.com

new Map(Object.entries(obj))
来源：http://sew.fanxiaobao.xyz

[U112] JS：字符串补位
来源：http://dyb.yuxming.cn

"7".padStart(3, "0")
来源：http://sev.tianlin.xyz

[U113] JS：正则替换全部
来源：http://djf.cqqwz.cn

s.replaceAll("a", "b")
来源：http://fmw.aibaodan.cn

[U114] JS：JSON 深比较
来源：http://dkt.ehwqpu.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://xil.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://wsa.havefunace.top

crypto.randomUUID()
来源：http://btw.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://wdn.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://hlh.zycfv.cn

[U117] JS：单元测试
来源：http://wdc.yueranfly.top

npm i -D vitest;  npx vitest
来源：http://zby.yueranfly.top

[U118] JS：开发服务器
来源：http://scn.ydjk.org.cn

npm i -D vite;  npx vite
来源：http://oko.cucudq.cn

[U119] JS：生产构建
来源：http://aks.meibo888.top

npx vite build
来源：http://xtt.ivvv.top

[U120] JS：读取环境变量（Vite）
来源：http://kuh.shzxlz.cn

import.meta.env.VITE_API_URL
来源：http://qrs.fehbvm.com

================================================================================
来源：http://ahj.tian-w.cn

统计汇总
来源：http://btf.tianlin.xyz

================================================================================
来源：http://dnx.zhoulong.xyz

按语言统计（条）：
来源：http://mqc.jqgfzy.top

Python ......... 252
来源：http://kax.yj20258888.top

PHP ............ 252
来源：http://vrg.smart0.xyz

JavaScript ..... 252
来源：http://hmq.aizwys.cn

TypeScript ..... 212
来源：http://tdr.hywenlv.cn

Java ........... 212
来源：http://lmk.sweek.top

Go ............. 212
来源：http://sgv.chenzaomai.com

Ruby ........... 212
来源：http://poe.ivvv.top

C# ............. 212
来源：http://lmc.gzhubu.top

C .............. 30
来源：http://dco.yanxiufei.cn

C++ ............ 30
来源：http://jce.hesvh.cn

SQL ............ 90
来源：http://yjt.hywenlv.cn

Bash ........... 80
来源：http://lmm.jinqigufen.top

Kotlin ......... 15
来源：http://tey.zhoulong.xyz

Swift .......... 15
来源：http://phq.shzxlz.cn

Lua ............ 10
来源：http://cnw.chenlongwang.top

Perl ........... 10
来源：http://zsx.ppjwa.cn

Scala .......... 10
来源：http://oqq.svipenyu.cn

------------------------------------
来源：http://fsr.tarul.cn

合计 ........... 2106 条
来源：http://nah.gaohongyu789.top

按章节统计：
来源：http://sro.ydzc1.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://esi.andypj.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://okx.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fhl.ppjwa.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eds.0kj1m.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ryj.havefunace.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cda.zhiwuduotai.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yar.0kj1m.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rgb.yongpay.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wes.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fan.yuanzhike.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fun.tian-w.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vjj.fanxiaobao.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wqh.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ncs.yj20258888.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://npy.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zkp.jianghu66.top

Q SQL 专题                              90
来源：http://ixg.fengsongda.top

R Bash 专题                             80
来源：http://usd.fanxiaobao.xyz

S C / C++ 专题                          60
来源：http://zxn.redwolf501.top

T 其他语言补充                          60
来源：http://brv.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://sfh.shzxlz.cn

------------------------------------
来源：http://zbm.vehdjk.com

合计                                  2106 条
来源：http://pui.guannengcc.top

--------------------------------------------------------------------------------
来源：http://srj.xziqi.cn

使用提醒
来源：http://vps.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://cin.xuanzx.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://knw.daxiang520.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vto.guannengcc.top


<!-- 参考信息 -->