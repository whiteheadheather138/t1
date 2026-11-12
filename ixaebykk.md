代发 wailian999

[U01] Py：创建虚拟环境
来源：http://kpp.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ymh.shzxlz.cn

[U02] Py：导出 / 安装依赖
来源：http://vul.cucudq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iwx.bbcook.cn

[U03] Py：加载 .env 配置
来源：http://viq.cheryme.top

from dotenv import load_dotenv; load_dotenv()
来源：http://eot.tarul.cn

[U04] Py：变量调试打印
来源：http://gpk.ywan-chungtsiang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dgr.fanxiaobao.xyz

[U05] Py：列表去重且保序
来源：http://jvx.yj202588.top

list(dict.fromkeys(arr))
来源：http://mvt.xziqi.cn

[U06] Py：合并两个字典
来源：http://rxm.jlsjyb.cn

{**a, **b}
来源：http://cph.sysykeji.top

[U07] Py：反转字典键值
来源：http://jpp.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://ncm.xziqi.cn

[U08] Py：展平二维列表
来源：http://hul.jinghuilouyu.cn

[y for x in nested for y in x]
来源：http://wvt.ctjpmb.com

[U09] Py：字典取最大值的键
来源：http://lft.dashuyun.cn

max(d, key=d.get)
来源：http://akw.jianghu66.top

[U10] Py：按值排序字典
来源：http://vke.yuanzhike.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qcj.yanxiufei.cn

[U11] Py：生成器表达式
来源：http://swv.zdqjudy.top

(x * 2 for x in arr)
来源：http://wls.fzhhl.top

[U12] Py：取出现最多的 3 个元素
来源：http://iuy.zhongyouzk.top

Counter(arr).most_common(3)
来源：http://ecs.redwolf501.top

[U13] Py：固定长度队列
来源：http://gjh.hammf.cn

deque(maxlen=10)
来源：http://nmn.zycfv.cn

[U14] Py：分组收集到列表
来源：http://soz.cdnleiting.top

defaultdict(list)
来源：http://lrn.cqqwz.cn

[U15] Py：高精度计时
来源：http://icd.hongshengwenyu.top

t = time.perf_counter()
来源：http://pkg.haohaochexian.top

[U16] Py：命令行参数解析
来源：http://mfw.epnwcf.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qxf.bbcook.cn

[U17] Py：初始化日志
来源：http://ehf.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://uqd.chenjidiqi.icu

[U18] Py：预编译正则
来源：http://eeo.fehbvm.com

pat = re.compile(r"\d+")
来源：http://foi.zhijiandao.cn

[U19] Py：正则替换带回调
来源：http://gdh.hysaishi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ukp.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://oal.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://njy.cucudq.cn

[U21] Py：自定义上下文管理器
来源：http://hvr.shanyushiyangtech.top

@contextlib.contextmanager
来源：http://wbj.jqgufenzy.top

[U22] Py：矩阵转置
来源：http://ffd.bbcook.cn

list(zip(*m))
来源：http://hqb.fktsv.cn

[U23] Py：分块读取大文件
来源：http://qeo.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rja.fengsongda.top

[U24] Py：路径操作
来源：http://nwl.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://znp.tarul.cn

[U25] Py：CSV 按字典读
来源：http://rdh.yongpay.top

csv.DictReader(f)
来源：http://nce.cucudq.cn

[U26] Py：并发下载
来源：http://ixw.ppjwa.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pjv.tanke756.top

[U27] Py：异步 HTTP
来源：http://vud.epnwcf.com

aiohttp.ClientSession() 配合 async with
来源：http://vfe.ppjwa.cn

[U28] Py：类型别名
来源：http://jlm.vqdsnc.cn

UserId = int
来源：http://orw.hnxiangtu.top

[U29] Py：属性校验
来源：http://yim.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://cgl.andypj.xyz

[U30] Py：数据类
来源：http://ltc.mhx1999.top

@dataclass(slots=True)
来源：http://qnm.ivvv.top

[U31] Py：单测
来源：http://lxh.yongpay.top

python -m pytest -q
来源：http://wje.pengpengdd.cyou

[U32] Py：代码格式化
来源：http://dou.aibaodan.cn

ruff format . && ruff check --fix .
来源：http://efd.bbcook.cn

[U33] Py：打包发布
来源：http://fws.ctjpmb.com

python -m build  （依赖 pyproject.toml）
来源：http://ztq.dashuyun.cn

[U34] Py：判断编码
来源：http://ukx.hfpthk.cn

chardet.detect(raw)
来源：http://qik.cheryme.top

[U35] Py：发送邮件
来源：http://fwj.yueranfly.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ilo.chenzaomai.com

[U36] Py：定时任务
来源：http://owg.ctjpmb.com

schedule.every(10).minutes.do(job)
来源：http://swk.hesvh.cn

[U37] Py：读写 Excel
来源：http://cin.zdbjq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qrq.ydjk.org.cn

[U38] Py：获取脚本所在目录
来源：http://gns.vqdsnc.cn

Path(__file__).resolve().parent
来源：http://swf.ehwqpu.com

[U39] Py：判断是否在交互环境
来源：http://qby.cashguo.top

sys.stdout.isatty()
来源：http://zrw.xuanzx.com

[U40] Py：打印到标准错误
来源：http://qdf.jqgufenzy.top

print("err", file=sys.stderr)
来源：http://waf.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://gwy.gogol.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://njj.ehwqpu.com

[U42] PHP：PSR-4 自动加载
来源：http://xhv.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ujy.epnwcf.com

[U43] PHP：声明命名空间
来源：http://iqa.yongpay.top

namespace App\Http;
来源：http://urd.bbcook.cn

[U44] PHP：开启严格类型
来源：http://mrz.wangdashe.top

declare(strict_types=1);
来源：http://tok.jinqigufen.top

[U45] PHP：类型声明与返回类型
来源：http://fvz.quarkkingdee.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jvl.zhixingplan.top

[U46] PHP：可空类型
来源：http://sjk.zdbjq.cn

?string $name = null
来源：http://yea.dashuyun.cn

[U47] PHP：联合类型
来源：http://gyq.vqdsnc.cn

int|string $id
来源：http://jzz.yuxming.cn

[U48] PHP：纯枚举
来源：http://arc.uphjek.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ynl.feifeiyinyue.top

[U49] PHP：只读属性
来源：http://snh.zhijiandao.cn

public readonly string $name
来源：http://iml.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://itp.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://ebt.tianlin.xyz

[U51] PHP：数组解构
来源：http://nwx.0kj1m.cn

[$a, $b] = $arr;
来源：http://qor.yfazqb.com

[U52] PHP：箭头函数
来源：http://gwn.bbcook.cn

$double = fn($x) => $x * 2;
来源：http://wbt.pycfn.com

[U53] PHP：空合并运算符
来源：http://tex.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://qsy.shzxlz.cn

[U54] PHP：空安全调用
来源：http://zgl.xuetiantiany.cn

$obj?->method()
来源：http://dgk.zhijiandao.cn

[U55] PHP：match 表达式
来源：http://blh.zdqjudy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://see.nanxinkj.top

[U56] PHP：命名参数
来源：http://ikm.cucudq.cn

f(a: 1, b: 2)
来源：http://oxx.ppjwa.cn

[U57] PHP：字符串插值
来源：http://tyr.zdbjq.cn

"值: {$a}"
来源：http://sln.epnwcf.com

[U58] PHP：数组三件套
来源：http://gvb.nanxinkj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kit.andypj.xyz

[U59] PHP：自定义排序
来源：http://zqi.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tcf.pengpengdd.cyou

[U60] PHP：JSON 编解码
来源：http://uzp.yj202588.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cft.nwbrower.top

[U61] PHP：正则
来源：http://iel.nwbrower.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yez.hfpthk.cn

[U62] PHP：日期对象
来源：http://dwn.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kal.shangyingyoupin.top

[U63] PHP：文件读写
来源：http://pxp.hongshengwenyu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rel.ybcxt.top

[U64] PHP：目录遍历
来源：http://pkb.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://hrl.yuxming.cn

[U65] PHP：会话
来源：http://ivx.jinyuanbaomall.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://oub.316326.xyz

[U66] PHP：设置 Cookie
来源：http://btu.yongpay.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uaq.guowangkeji.top

[U67] PHP：处理文件上传
来源：http://frs.hywenlv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ohn.havefunace.top

[U68] PHP：PDO 连接
来源：http://uds.ydjk.org.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://htf.ppjwa.cn

[U69] PHP：PDO 预处理
来源：http://hlm.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fav.cheryme.top

[U70] PHP：PDO 事务
来源：http://msi.zhengqikj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wjs.bbcook.cn

[U71] PHP：抛出异常
来源：http://xqc.yueranfly.top

throw new RuntimeException("失败", 500);
来源：http://cnt.wangshuangyany.cn

[U72] PHP：写错误日志
来源：http://gvo.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://bbs.sxryk.cn

[U73] PHP：读取 ini 配置
来源：http://vhl.tanke756.top

parse_ini_file("config.ini", true)
来源：http://mcc.yfazqb.com

[U74] PHP：读取环境变量
来源：http://qww.jinyuanbaomall.cn

getenv("APP_ENV") ?: "production"
来源：http://cqa.hfpthk.cn

[U75] PHP：依赖注入
来源：http://ojz.fehbvm.com

composer require psr/container
来源：http://iss.cdnleiting.top

[U76] PHP：简单路由
来源：http://zlc.fehbvm.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://utq.sxryk.cn

[U77] PHP：模板渲染
来源：http://gxi.hammf.cn

composer require twig/twig
来源：http://aib.zhijiandao.cn

[U78] PHP：单元测试
来源：http://uwq.bjfxy.top

composer require --dev phpunit/phpunit
来源：http://wpn.ydjk.org.cn

[U79] PHP：静态分析
来源：http://byc.vehdjk.com

composer require --dev phpstan/phpstan
来源：http://sjz.shanyushiyangkeji.top

[U80] PHP：代码规范修复
来源：http://qwr.meibo888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://msv.sweek.top

[U81] JS：初始化项目
来源：http://sbd.hfpthk.cn

npm init -y;  npm i express
来源：http://wal.daria6918.cn

[U82] JS：package.json 脚本
来源：http://lrl.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hqs.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://our.bjfxy.top

export const a = 1;  import { a } from "./m.js";
来源：http://atr.xuetiantiany.cn

[U84] JS：CommonJS 写法
来源：http://pci.chenzaomai.com

module.exports = { a };  const { a } = require("./m");
来源：http://vhu.zdqjudy.top

[U85] JS：可选链
来源：http://dzw.yueranfly.top

a?.b?.c
来源：http://fra.tian-w.cn

[U86] JS：空值合并
来源：http://rms.cdnleiting.top

a ?? b
来源：http://sht.zhixingplan.top

[U87] JS：解构默认值
来源：http://owv.redwolf501.top

const { a = 1, b = 2 } = obj;
来源：http://adj.snrcjt.cn

[U88] JS：对象展开合并
来源：http://sed.havefunace.top

{ ...a, ...b }
来源：http://zba.52xcode.cn

[U89] JS：数组去重
来源：http://zyb.ydzc1.top

[...new Set(arr)]
来源：http://bmc.ydzc1.top

[U90] JS：数字数组排序
来源：http://thc.havefunace.top

[...arr].sort((a, b) => a - b)
来源：http://eaq.tarul.cn

[U91] JS：对象键值遍历
来源：http://cot.c1oappe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cyp.wangdashe.top

[U92] JS：深拷贝
来源：http://qfv.xylfe.cn

structuredClone(obj)
来源：http://ndy.wangdashe.top

[U93] JS：模板字符串
来源：http://hlx.yj20258.top

`共 ${n} 条`
来源：http://nac.c1oappe.top

[U94] JS：箭头函数
来源：http://iao.smart0.xyz

const double = x => x * 2;
来源：http://ton.havefunace.top

[U95] JS：Promise 包装
来源：http://vfd.shangyingyoupin.top

new Promise((resolve, reject) => {})
来源：http://kiq.chenjidiqi.icu

[U96] JS：async/await 与异常
来源：http://jop.nwbrower.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zny.aibaodan.cn

[U97] JS：并发请求
来源：http://agq.fengsongda.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gtp.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://heg.jiagoushi.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bsq.gogol.net.cn

[U99] JS：事件监听
来源：http://vsd.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://sgh.ivvv.top

[U100] JS：DOM 查询
来源：http://mig.vqdsnc.cn

document.querySelector(".item")
来源：http://gri.hcnkem.com

[U101] JS：classList 操作
来源：http://fnv.fehbvm.com

el.classList.toggle("active")
来源：http://fsx.snrcjt.cn

[U102] JS：本地存储
来源：http://pjm.zycfv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sbg.ivvv.top

[U103] JS：定时器
来源：http://hao.fanxiaobao.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://inq.andypj.xyz

[U104] JS：防抖
来源：http://xtq.sweek.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://edp.pycfn.com

[U105] JS：节流
来源：http://zub.sjlbkw.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://esc.sufxvd.cn

[U106] JS：日期格式化
来源：http://jvt.hammf.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sjz.cucudq.cn

[U107] JS：数字千分位
来源：http://zqp.yj202588.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ngu.zhoulong.xyz

[U108] JS：随机整数
来源：http://lvz.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sgm.haohaochexian.top

[U109] JS：数组分组
来源：http://umg.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://fes.hnxiangtu.top

[U110] JS：数组分块
来源：http://fqq.zdbjq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nsk.epnwcf.com

[U111] JS：对象转 Map
来源：http://ozx.yj202588.top

new Map(Object.entries(obj))
来源：http://sua.shzxlz.cn

[U112] JS：字符串补位
来源：http://ltd.zhongyouzk.top

"7".padStart(3, "0")
来源：http://xww.shuidangran.top

[U113] JS：正则替换全部
来源：http://vhn.cdnleiting.top

s.replaceAll("a", "b")
来源：http://oaa.ppjwa.cn

[U114] JS：JSON 深比较
来源：http://mgy.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qkp.ctjpmb.com

[U115] JS：生成 UUID
来源：http://ybi.snrcjt.cn

crypto.randomUUID()
来源：http://ojj.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://sah.wangdashe.top

/** @param {string} name */ function f(name) {}
来源：http://ibh.cqqwz.cn

[U117] JS：单元测试
来源：http://hqu.meibo888.top

npm i -D vitest;  npx vitest
来源：http://vrn.zhixingplan.top

[U118] JS：开发服务器
来源：http://fyt.yongpay.top

npm i -D vite;  npx vite
来源：http://gud.hfpthk.cn

[U119] JS：生产构建
来源：http://lsx.aibaodan.cn

npx vite build
来源：http://zag.yfazqb.com

[U120] JS：读取环境变量（Vite）
来源：http://pzx.jinqigufen.top

import.meta.env.VITE_API_URL
来源：http://qti.uphjek.com

================================================================================
来源：http://qfg.svipenyu.cn

统计汇总
来源：http://vmi.sufxvd.cn

================================================================================
来源：http://awk.zhoulong.xyz

按语言统计（条）：
来源：http://gvi.hesvh.cn

Python ......... 252
来源：http://klh.hysaishi.cn

PHP ............ 252
来源：http://raz.hnqzz.top

JavaScript ..... 252
来源：http://usp.xinyue.icu

TypeScript ..... 212
来源：http://rqi.hfpthk.cn

Java ........... 212
来源：http://xtp.ctjpmb.com

Go ............. 212
来源：http://maw.tanke756.top

Ruby ........... 212
来源：http://weh.shanyushiyangtech.top

C# ............. 212
来源：http://wzs.zhongyouzk.top

C .............. 30
来源：http://lul.yanxiufei.cn

C++ ............ 30
来源：http://rsz.feifeiyinyue.top

SQL ............ 90
来源：http://kdi.yanxiufei.cn

Bash ........... 80
来源：http://wbb.ybcxt.top

Kotlin ......... 15
来源：http://bfi.yuanzhike.top

Swift .......... 15
来源：http://rcy.gaohongyu789.top

Lua ............ 10
来源：http://uyn.dianchejie.cn

Perl ........... 10
来源：http://tub.hammf.cn

Scala .......... 10
来源：http://dla.quarkkingdee.top

------------------------------------
来源：http://mgp.fktsv.cn

合计 ........... 2106 条
来源：http://hgy.9152youxi.cn

按章节统计：
来源：http://hjl.zhixingplan.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ykr.cqqwz.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gjc.yanxiufei.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kmu.jlsjyb.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lin.jinyuanbaomall.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ckv.iojbl.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bun.ydzc1.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hmb.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jlf.zhongyouzk.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nah.hammf.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://koj.fengsongda.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pjn.ywan-chungtsiang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gav.cucudq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://apj.birdmap.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pcv.cheryme.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sry.jinqigfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rdq.daria6918.cn

Q SQL 专题                              90
来源：http://wsg.epnwcf.com

R Bash 专题                             80
来源：http://sqy.fzhhl.top

S C / C++ 专题                          60
来源：http://xcj.yj202588.top

T 其他语言补充                          60
来源：http://nhp.jqgfzy.top

U 高频实用片段                         120
来源：http://rjg.yangfankeji.com

------------------------------------
来源：http://beb.yj202588.top

合计                                  2106 条
来源：http://ayb.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://gyx.jinqigufen.top

使用提醒
来源：http://ble.cucudq.cn

--------------------------------------------------------------------------------
来源：http://mxl.jyoumei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oeh.ybcxt.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qzo.meibo888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xaw.gogol.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tzg.jiagoushi.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://frn.shzxlz.cn

—— 文件结束 ——
来源：http://yzp.haohaochexian.top

================================================================================
来源：http://vnm.yvedp.cn

程序语言常见例子速查手册（2024 版）
来源：http://lth.hysaishi.cn

Common Programming Examples Cheat Book
来源：http://dwi.xingfuxueyuan.xyz

================================================================================
来源：http://lrm.yongpay.top


<!-- 参考信息 -->