代发 wailian999

[U01] Py：创建虚拟环境
来源：http://wnt.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://skw.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://jri.cucudq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qzw.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://cni.xylfe.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ysr.iojbl.cn

[U04] Py：变量调试打印
来源：http://qxq.fktsv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qrt.chenjidiqi.icu

[U05] Py：列表去重且保序
来源：http://sjo.xziqi.cn

list(dict.fromkeys(arr))
来源：http://iau.nwbrower.top

[U06] Py：合并两个字典
来源：http://nwm.ydjk.org.cn

{**a, **b}
来源：http://sbf.tian-w.cn

[U07] Py：反转字典键值
来源：http://pjl.chenjidiqi.icu

{v: k for k, v in d.items()}
来源：http://anz.cashguo.top

[U08] Py：展平二维列表
来源：http://tph.zhaomingkeji.xyz

[y for x in nested for y in x]
来源：http://jai.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://ntq.dianchejie.cn

max(d, key=d.get)
来源：http://bjn.daxiang520.top

[U10] Py：按值排序字典
来源：http://llj.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zhq.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://gcy.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://mgm.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lud.ywan-chungtsiang.top

Counter(arr).most_common(3)
来源：http://izy.uphjek.com

[U13] Py：固定长度队列
来源：http://hye.ydzc1.top

deque(maxlen=10)
来源：http://ldn.zhengqikj.top

[U14] Py：分组收集到列表
来源：http://fho.haohaochexian.top

defaultdict(list)
来源：http://aug.chenlongwang.top

[U15] Py：高精度计时
来源：http://vmw.hnqzz.top

t = time.perf_counter()
来源：http://qyf.vqdsnc.cn

[U16] Py：命令行参数解析
来源：http://fyy.xinyue.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zai.zhixingplan.top

[U17] Py：初始化日志
来源：http://npc.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://nnr.guowangkeji.top

[U18] Py：预编译正则
来源：http://peb.xylfe.cn

pat = re.compile(r"\d+")
来源：http://otw.hongshengwenyu.top

[U19] Py：正则替换带回调
来源：http://aet.jqgufenzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ydb.jqgufenzy.top

[U20] Py：缓存函数结果
来源：http://mvn.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://cyh.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://yxm.meibo888.top

@contextlib.contextmanager
来源：http://yxg.sxryk.cn

[U22] Py：矩阵转置
来源：http://fjo.feifeiyinyue.top

list(zip(*m))
来源：http://zir.sysykeji.top

[U23] Py：分块读取大文件
来源：http://egb.tianlin.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nvn.xuetiantiany.cn

[U24] Py：路径操作
来源：http://vav.52xcode.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zhj.smart0.xyz

[U25] Py：CSV 按字典读
来源：http://vdx.52xcode.cn

csv.DictReader(f)
来源：http://dho.nwbrower.top

[U26] Py：并发下载
来源：http://ucz.birdmap.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yim.xuanzx.com

[U27] Py：异步 HTTP
来源：http://wkr.shanyushiyangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://wod.ehwqpu.com

[U28] Py：类型别名
来源：http://geo.nwbrower.top

UserId = int
来源：http://uil.316326.xyz

[U29] Py：属性校验
来源：http://axw.hysaishi.cn

@property 与 @x.setter 配合
来源：http://hof.haohaochexian.top

[U30] Py：数据类
来源：http://tdv.hnxiangtu.top

@dataclass(slots=True)
来源：http://skx.tianlin.xyz

[U31] Py：单测
来源：http://fkv.daria6918.cn

python -m pytest -q
来源：http://gqo.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://bft.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://ocu.bbcook.cn

[U33] Py：打包发布
来源：http://hpo.yuanzhike.top

python -m build  （依赖 pyproject.toml）
来源：http://mhq.hfpthk.cn

[U34] Py：判断编码
来源：http://msk.dashuyun.cn

chardet.detect(raw)
来源：http://tkg.cashguo.top

[U35] Py：发送邮件
来源：http://qdc.zhaomingkeji.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mwg.ydzc1.top

[U36] Py：定时任务
来源：http://skb.xziqi.cn

schedule.every(10).minutes.do(job)
来源：http://vjd.cdnleiting.top

[U37] Py：读写 Excel
来源：http://vgv.cashguo.top

pandas.read_excel / DataFrame.to_excel
来源：http://bps.pycfn.com

[U38] Py：获取脚本所在目录
来源：http://jka.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://ajm.dianchejie.cn

[U39] Py：判断是否在交互环境
来源：http://erq.xuetiantiany.cn

sys.stdout.isatty()
来源：http://qib.pycfn.com

[U40] Py：打印到标准错误
来源：http://cjc.zhoulong.xyz

print("err", file=sys.stderr)
来源：http://fci.fzhhl.top

[U41] PHP：初始化 Composer 项目
来源：http://otu.gogol.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yse.quarkkingdee.top

[U42] PHP：PSR-4 自动加载
来源：http://ftx.yvedp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wpl.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://lcf.chenjidiqi.icu

namespace App\Http;
来源：http://zcx.yj20258.top

[U44] PHP：开启严格类型
来源：http://spc.chenjidiqi.icu

declare(strict_types=1);
来源：http://pzk.fzhhl.top

[U45] PHP：类型声明与返回类型
来源：http://pav.hnqzz.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ens.316326.xyz

[U46] PHP：可空类型
来源：http://qsn.cqqwz.cn

?string $name = null
来源：http://sdq.jqgfzy.top

[U47] PHP：联合类型
来源：http://dxk.316326.xyz

int|string $id
来源：http://oem.nanxinkj.top

[U48] PHP：纯枚举
来源：http://ube.ehwqpu.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://asf.andypj.xyz

[U49] PHP：只读属性
来源：http://bka.hesvh.cn

public readonly string $name
来源：http://yps.yonumen.top

[U50] PHP：构造器属性提升
来源：http://inw.gotoacloud.top

public function __construct(private int $id) {}
来源：http://rdd.vehdjk.com

[U51] PHP：数组解构
来源：http://wup.xylfe.cn

[$a, $b] = $arr;
来源：http://wun.hammf.cn

[U52] PHP：箭头函数
来源：http://lqx.hfpthk.cn

$double = fn($x) => $x * 2;
来源：http://aiz.316326.xyz

[U53] PHP：空合并运算符
来源：http://dbo.shuidangran.top

$v = $a ?? $b ?? "default";
来源：http://yfz.xziqi.cn

[U54] PHP：空安全调用
来源：http://yhl.smart0.xyz

$obj?->method()
来源：http://uyr.hcnkem.com

[U55] PHP：match 表达式
来源：http://uqv.gzhubu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cir.sysykeji.top

[U56] PHP：命名参数
来源：http://cxe.ybcxt.top

f(a: 1, b: 2)
来源：http://vqz.quarkkingdee.top

[U57] PHP：字符串插值
来源：http://efb.bbcook.cn

"值: {$a}"
来源：http://qzq.pengpengdd.cyou

[U58] PHP：数组三件套
来源：http://yau.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zrx.shanyushiyangkeji.top

[U59] PHP：自定义排序
来源：http://umo.zhengqikj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wir.zycfv.cn

[U60] PHP：JSON 编解码
来源：http://zud.bjfxy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sdm.gogol.net.cn

[U61] PHP：正则
来源：http://urg.ybcxt.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://aop.yanxiufei.cn

[U62] PHP：日期对象
来源：http://lgp.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rgh.fktsv.cn

[U63] PHP：文件读写
来源：http://zqg.ivvv.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hhf.sufxvd.cn

[U64] PHP：目录遍历
来源：http://rfv.zdqjudy.top

glob("dir/*.php");  scandir("dir");
来源：http://upk.nanxinkj.top

[U65] PHP：会话
来源：http://kyy.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jgq.0kj1m.cn

[U66] PHP：设置 Cookie
来源：http://vke.jqgufenzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nto.snrcjt.cn

[U67] PHP：处理文件上传
来源：http://wqc.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kki.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://tzb.sysykeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ete.ydjk.org.cn

[U69] PHP：PDO 预处理
来源：http://hvz.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://euo.0kj1m.cn

[U70] PHP：PDO 事务
来源：http://mek.jqgfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kvk.sjlbkw.cn

[U71] PHP：抛出异常
来源：http://wzx.hcnkem.com

throw new RuntimeException("失败", 500);
来源：http://bvy.zdbjq.cn

[U72] PHP：写错误日志
来源：http://tww.zhongyouzk.top

error_log("失败: " . $e->getMessage());
来源：http://etg.snrcjt.cn

[U73] PHP：读取 ini 配置
来源：http://qdw.andypj.xyz

parse_ini_file("config.ini", true)
来源：http://qks.shanyushiyangkeji.top

[U74] PHP：读取环境变量
来源：http://udp.nanxinkj.top

getenv("APP_ENV") ?: "production"
来源：http://evt.chenzaomai.com

[U75] PHP：依赖注入
来源：http://kar.nwbrower.top

composer require psr/container
来源：http://eap.iojbl.cn

[U76] PHP：简单路由
来源：http://zxi.smart0.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mmr.c1oappe.top

[U77] PHP：模板渲染
来源：http://gbb.zhixingplan.top

composer require twig/twig
来源：http://hmh.hfpthk.cn

[U78] PHP：单元测试
来源：http://dqg.andypj.xyz

composer require --dev phpunit/phpunit
来源：http://hdz.sufxvd.cn

[U79] PHP：静态分析
来源：http://pmk.ybcxt.top

composer require --dev phpstan/phpstan
来源：http://byn.nanxinkj.top

[U80] PHP：代码规范修复
来源：http://qqz.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://eki.kuanghao11.cn

[U81] JS：初始化项目
来源：http://mcy.svipenyu.cn

npm init -y;  npm i express
来源：http://jlj.52xcode.cn

[U82] JS：package.json 脚本
来源：http://hqc.gzhubu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://csl.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://hnh.gzhubu.top

export const a = 1;  import { a } from "./m.js";
来源：http://osk.yuxming.cn

[U84] JS：CommonJS 写法
来源：http://siv.cucudq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yim.yangfankeji.com

[U85] JS：可选链
来源：http://oet.bjfxy.top

a?.b?.c
来源：http://tsd.zhiwuduotai.top

[U86] JS：空值合并
来源：http://bfe.hfpthk.cn

a ?? b
来源：http://bcg.nanxinkj.top

[U87] JS：解构默认值
来源：http://ebd.zhoulong.xyz

const { a = 1, b = 2 } = obj;
来源：http://uiw.yonumen.top

[U88] JS：对象展开合并
来源：http://uxs.sxryk.cn

{ ...a, ...b }
来源：http://kpj.shanyushiyangtech.top

[U89] JS：数组去重
来源：http://mbh.52xcode.cn

[...new Set(arr)]
来源：http://fsx.jqgfzy.top

[U90] JS：数字数组排序
来源：http://ffk.vehdjk.com

[...arr].sort((a, b) => a - b)
来源：http://dqc.guowangkeji.top

[U91] JS：对象键值遍历
来源：http://djs.fehbvm.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rnt.fehbvm.com

[U92] JS：深拷贝
来源：http://oxp.jqgufenzy.top

structuredClone(obj)
来源：http://dzm.zhiwuduotai.top

[U93] JS：模板字符串
来源：http://jkn.mhx1999.top

`共 ${n} 条`
来源：http://gjh.shzxlz.cn

[U94] JS：箭头函数
来源：http://ann.shanyushiyangkeji.top

const double = x => x * 2;
来源：http://fxl.feifeiyinyue.top

[U95] JS：Promise 包装
来源：http://mvd.hongshengwenyu.top

new Promise((resolve, reject) => {})
来源：http://bwv.sxryk.cn

[U96] JS：async/await 与异常
来源：http://hyx.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://scw.zhixingplan.top

[U97] JS：并发请求
来源：http://etf.sxryk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://moc.cucudq.cn

[U98] JS：fetch 带 JSON
来源：http://cwn.zdbjq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://spd.xuanzx.com

[U99] JS：事件监听
来源：http://dsb.haohaochexian.top

el.addEventListener("click", e => {})
来源：http://miz.sysykeji.top

[U100] JS：DOM 查询
来源：http://yug.ydzc1.top

document.querySelector(".item")
来源：http://ewp.tanke756.top

[U101] JS：classList 操作
来源：http://wgf.jinqigufen.top

el.classList.toggle("active")
来源：http://kcu.cdnleiting.top

[U102] JS：本地存储
来源：http://wff.andypj.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://aqa.bbcook.cn

[U103] JS：定时器
来源：http://tby.xinyue.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bqp.xuanzx.com

[U104] JS：防抖
来源：http://edm.fktsv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://laj.fktsv.cn

[U105] JS：节流
来源：http://vwc.sweek.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cwb.ctjpmb.com

[U106] JS：日期格式化
来源：http://cur.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yhe.nanxuanxn.top

[U107] JS：数字千分位
来源：http://vos.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://trh.yueranfly.top

[U108] JS：随机整数
来源：http://obh.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ufk.shzxlz.cn

[U109] JS：数组分组
来源：http://lnf.yonumen.top

Object.groupBy(arr, x => x.type)
来源：http://njy.zdqjudy.top

[U110] JS：数组分块
来源：http://tkf.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qim.mhx1999.top

[U111] JS：对象转 Map
来源：http://awg.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://txl.ybcxt.top

[U112] JS：字符串补位
来源：http://mva.sufxvd.cn

"7".padStart(3, "0")
来源：http://vfp.zhijiandao.cn

[U113] JS：正则替换全部
来源：http://wwq.zdqjudy.top

s.replaceAll("a", "b")
来源：http://bde.cqqwz.cn

[U114] JS：JSON 深比较
来源：http://oky.jinqigfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://idc.dashuyun.cn

[U115] JS：生成 UUID
来源：http://oce.yonumen.top

crypto.randomUUID()
来源：http://cqm.jyoumei.cn

[U116] JS：类型检查（JSDoc）
来源：http://xdp.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://sel.zdqjudy.top

[U117] JS：单元测试
来源：http://nff.tanke756.top

npm i -D vitest;  npx vitest
来源：http://jfq.jqgufenzy.top

[U118] JS：开发服务器
来源：http://rmm.zycfv.cn

npm i -D vite;  npx vite
来源：http://maa.yj202588.top

[U119] JS：生产构建
来源：http://ldy.9152youxi.cn

npx vite build
来源：http://wyk.zhiwuduotai.top

[U120] JS：读取环境变量（Vite）
来源：http://dmk.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://xpp.xziqi.cn

================================================================================
来源：http://mfd.zhengqikj.top

统计汇总
来源：http://zbc.smart0.xyz

================================================================================
来源：http://ucu.yongpay.top

按语言统计（条）：
来源：http://mvl.shangyingyoupin.top

Python ......... 252
来源：http://kkn.c1oappe.top

PHP ............ 252
来源：http://jpb.zhongyouzk.top

JavaScript ..... 252
来源：http://qkk.nanxuanxn.top

TypeScript ..... 212
来源：http://jhe.vehdjk.com

Java ........... 212
来源：http://ofn.nwbrower.top

Go ............. 212
来源：http://onh.xziqi.cn

Ruby ........... 212
来源：http://axo.jinqigfzy.top

C# ............. 212
来源：http://vfw.cqqwz.cn

C .............. 30
来源：http://tbq.316326.xyz

C++ ............ 30
来源：http://tah.yongpay.top

SQL ............ 90
来源：http://yfx.fanxiaobao.xyz

Bash ........... 80
来源：http://vza.cdnleiting.top

Kotlin ......... 15
来源：http://fvt.9152youxi.cn

Swift .......... 15
来源：http://xsz.jqgfzy.top

Lua ............ 10
来源：http://itc.redwolf501.top

Perl ........... 10
来源：http://eaa.ydzc1.top

Scala .......... 10
来源：http://qcg.jqgfzy.top

------------------------------------
来源：http://hav.jqgfzy.top

合计 ........... 2106 条
来源：http://mqb.shanyushiyangtech.top

按章节统计：
来源：http://bgz.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nfy.yuanzhike.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wgt.gzhubu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kqn.nwbrower.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qxn.nwbrower.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://taj.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cil.cdnleiting.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://swi.ehwqpu.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://var.shanyushiyangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://isy.guowangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fsf.jianghu66.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gpc.jqgfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uwj.tian-w.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zdx.tianlin.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://czr.vehdjk.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://krr.tarul.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mbt.jiagoushi.top

Q SQL 专题                              90
来源：http://mwk.jyoumei.cn

R Bash 专题                             80
来源：http://eep.zycfv.cn

S C / C++ 专题                          60
来源：http://you.sufxvd.cn

T 其他语言补充                          60
来源：http://vhp.hysaishi.cn

U 高频实用片段                         120
来源：http://doc.xinyue.icu

------------------------------------
来源：http://hlx.zdbjq.cn

合计                                  2106 条
来源：http://gcp.yvedp.cn

--------------------------------------------------------------------------------
来源：http://iig.yueranfly.top

使用提醒
来源：http://xoj.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://fwm.sysykeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bit.daria6918.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tvs.ivvv.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rai.vehdjk.com

在旧版本上使用前请先确认语法支持情况。
来源：http://xod.hongshengwenyu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ngc.gzhubu.top

—— 文件结束 ——
来源：http://krt.tianlin.xyz

================================================================================
来源：http://ymn.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://ixc.hysaishi.cn

Common Programming Examples Cheat Book
来源：http://yma.jqgfzy.top

================================================================================
来源：http://iki.jinyuanbaomall.cn


<!-- 参考信息 -->