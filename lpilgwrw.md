代发 wailian999

[U05] Py：列表去重且保序
来源：http://oox.tanke756.top

list(dict.fromkeys(arr))
来源：http://dsu.jlsjyb.cn

[U06] Py：合并两个字典
来源：http://zma.52xcode.cn

{**a, **b}
来源：http://njq.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://tqe.nwbrower.top

{v: k for k, v in d.items()}
来源：http://fbw.chenjidiqi.icu

[U08] Py：展平二维列表
来源：http://pnv.epnwcf.com

[y for x in nested for y in x]
来源：http://isx.yongpay.top

[U09] Py：字典取最大值的键
来源：http://eog.xuanzx.com

max(d, key=d.get)
来源：http://dva.daria6918.cn

[U10] Py：按值排序字典
来源：http://vml.gogol.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tzl.yj20258888.top

[U11] Py：生成器表达式
来源：http://ttf.tianlin.xyz

(x * 2 for x in arr)
来源：http://anr.feifeiyinyue.top

[U12] Py：取出现最多的 3 个元素
来源：http://has.sweek.top

Counter(arr).most_common(3)
来源：http://zee.cdnleiting.top

[U13] Py：固定长度队列
来源：http://fdf.cheryme.top

deque(maxlen=10)
来源：http://cuz.jinyuanbaomall.cn

[U14] Py：分组收集到列表
来源：http://kjg.hammf.cn

defaultdict(list)
来源：http://jbd.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://vhl.aibaodan.cn

t = time.perf_counter()
来源：http://ova.hysaishi.cn

[U16] Py：命令行参数解析
来源：http://ecc.yanxiufei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pot.ctjpmb.com

[U17] Py：初始化日志
来源：http://ewj.yueranfly.top

logging.basicConfig(level=logging.INFO)
来源：http://weu.jianghu66.top

[U18] Py：预编译正则
来源：http://tal.shzxlz.cn

pat = re.compile(r"\d+")
来源：http://cag.mhx1999.top

[U19] Py：正则替换带回调
来源：http://jtz.guowangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://emo.cashguo.top

[U20] Py：缓存函数结果
来源：http://zpl.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://cfm.zycfv.cn

[U21] Py：自定义上下文管理器
来源：http://erb.havefunace.top

@contextlib.contextmanager
来源：http://uou.xingfuxueyuan.xyz

[U22] Py：矩阵转置
来源：http://tsa.vehdjk.com

list(zip(*m))
来源：http://bxz.xuetiantiany.cn

[U23] Py：分块读取大文件
来源：http://wze.hfpthk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://beu.nanxinkj.top

[U24] Py：路径操作
来源：http://iky.pengpengdd.cyou

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wcw.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://osp.jyoumei.cn

csv.DictReader(f)
来源：http://rbm.daria6918.cn

[U26] Py：并发下载
来源：http://wcm.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bfj.daria6918.cn

[U27] Py：异步 HTTP
来源：http://owc.gaohongyu789.top

aiohttp.ClientSession() 配合 async with
来源：http://quf.daria6918.cn

[U28] Py：类型别名
来源：http://tkf.jlsjyb.cn

UserId = int
来源：http://odh.yj202588.top

[U29] Py：属性校验
来源：http://qug.jqgfzy.top

@property 与 @x.setter 配合
来源：http://lru.ctjpmb.com

[U30] Py：数据类
来源：http://ktx.daxiang520.top

@dataclass(slots=True)
来源：http://xzt.jqgufenzy.top

[U31] Py：单测
来源：http://ilc.ehwqpu.com

python -m pytest -q
来源：http://gyi.birdmap.top

[U32] Py：代码格式化
来源：http://gyz.fktsv.cn

ruff format . && ruff check --fix .
来源：http://nei.gzhubu.top

[U33] Py：打包发布
来源：http://bvi.zycfv.cn

python -m build  （依赖 pyproject.toml）
来源：http://tgw.fktsv.cn

[U34] Py：判断编码
来源：http://qfq.shanyushiyangtech.top

chardet.detect(raw)
来源：http://pzk.uphjek.com

[U35] Py：发送邮件
来源：http://nai.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://arp.yj202588.top

[U36] Py：定时任务
来源：http://wqr.yangfankeji.com

schedule.every(10).minutes.do(job)
来源：http://iqj.yanxiufei.cn

[U37] Py：读写 Excel
来源：http://rpk.vqdsnc.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yyl.aibaodan.cn

[U38] Py：获取脚本所在目录
来源：http://oef.kuanghao11.cn

Path(__file__).resolve().parent
来源：http://elg.andypj.xyz

[U39] Py：判断是否在交互环境
来源：http://oyl.hnqzz.top

sys.stdout.isatty()
来源：http://ixt.cdnleiting.top

[U40] Py：打印到标准错误
来源：http://imr.birdmap.top

print("err", file=sys.stderr)
来源：http://bhm.ivvv.top

[U41] PHP：初始化 Composer 项目
来源：http://rxp.chenjidiqi.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://wsa.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://ylj.yfazqb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ove.nwbrower.top

[U43] PHP：声明命名空间
来源：http://rgi.cdnleiting.top

namespace App\Http;
来源：http://uvv.jiagoushi.top

[U44] PHP：开启严格类型
来源：http://fyb.c1oappe.top

declare(strict_types=1);
来源：http://afk.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://izr.52xcode.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vrd.snrcjt.cn

[U46] PHP：可空类型
来源：http://vjg.pycfn.com

?string $name = null
来源：http://zya.jqgfzy.top

[U47] PHP：联合类型
来源：http://vmh.shangyingyoupin.top

int|string $id
来源：http://lbh.smart0.xyz

[U48] PHP：纯枚举
来源：http://flb.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ehm.gaohongyu789.top

[U49] PHP：只读属性
来源：http://gww.zhijiandao.cn

public readonly string $name
来源：http://rfz.vqdsnc.cn

[U50] PHP：构造器属性提升
来源：http://nqz.nanxinkj.top

public function __construct(private int $id) {}
来源：http://hof.yj20258.top

[U51] PHP：数组解构
来源：http://ipd.vqdsnc.cn

[$a, $b] = $arr;
来源：http://qlu.dianchejie.cn

[U52] PHP：箭头函数
来源：http://uid.zhijiandao.cn

$double = fn($x) => $x * 2;
来源：http://fzq.jianghu66.top

[U53] PHP：空合并运算符
来源：http://uxe.jinqigufen.top

$v = $a ?? $b ?? "default";
来源：http://rsp.andypj.xyz

[U54] PHP：空安全调用
来源：http://cjd.yuxming.cn

$obj?->method()
来源：http://yqr.zdbjq.cn

[U55] PHP：match 表达式
来源：http://fxj.jlsjyb.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://stm.wangshuangyany.cn

[U56] PHP：命名参数
来源：http://dea.tian-w.cn

f(a: 1, b: 2)
来源：http://xju.guowangkeji.top

[U57] PHP：字符串插值
来源：http://wld.fanxiaobao.xyz

"值: {$a}"
来源：http://iop.ehwqpu.com

[U58] PHP：数组三件套
来源：http://dgb.yvedp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lnj.hesvh.cn

[U59] PHP：自定义排序
来源：http://kht.zycfv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jbk.cucudq.cn

[U60] PHP：JSON 编解码
来源：http://xou.guowangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fqd.shuidangran.top

[U61] PHP：正则
来源：http://qnq.fzhhl.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://aao.cqqwz.cn

[U62] PHP：日期对象
来源：http://tkz.316326.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bqo.yongpay.top

[U63] PHP：文件读写
来源：http://xfc.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ovt.haohaochexian.top

[U64] PHP：目录遍历
来源：http://jhx.ppjwa.cn

glob("dir/*.php");  scandir("dir");
来源：http://cqt.zhiwuduotai.top

[U65] PHP：会话
来源：http://knp.uphjek.com

session_start();  $_SESSION["uid"] = 1;
来源：http://qhg.yongpay.top

[U66] PHP：设置 Cookie
来源：http://tth.ctjpmb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lnx.nwbrower.top

[U67] PHP：处理文件上传
来源：http://yey.zhongyouzk.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sim.316326.xyz

[U68] PHP：PDO 连接
来源：http://vuu.zdbjq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xyw.kuanghao11.cn

[U69] PHP：PDO 预处理
来源：http://ppd.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wdy.wangshuangyany.cn

[U70] PHP：PDO 事务
来源：http://dth.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wfc.wangshuangyany.cn

[U71] PHP：抛出异常
来源：http://kuc.zhijiandao.cn

throw new RuntimeException("失败", 500);
来源：http://mqm.jlsjyb.cn

[U72] PHP：写错误日志
来源：http://occ.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://drk.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://dbi.zhiwuduotai.top

parse_ini_file("config.ini", true)
来源：http://adp.zdqjudy.top

[U74] PHP：读取环境变量
来源：http://rui.dianchejie.cn

getenv("APP_ENV") ?: "production"
来源：http://ktb.hysaishi.cn

[U75] PHP：依赖注入
来源：http://usm.kuanghao11.cn

composer require psr/container
来源：http://mzc.epnwcf.com

[U76] PHP：简单路由
来源：http://jgu.havefunace.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bhh.hnxiangtu.top

[U77] PHP：模板渲染
来源：http://rnd.wangdashe.top

composer require twig/twig
来源：http://jlz.jlsjyb.cn

[U78] PHP：单元测试
来源：http://vrr.havefunace.top

composer require --dev phpunit/phpunit
来源：http://rnu.smart0.xyz

[U79] PHP：静态分析
来源：http://csd.zhongyouzk.top

composer require --dev phpstan/phpstan
来源：http://mha.sxryk.cn

[U80] PHP：代码规范修复
来源：http://sid.hysaishi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dex.shuidangran.top

[U81] JS：初始化项目
来源：http://uxi.sysykeji.top

npm init -y;  npm i express
来源：http://sip.tanke756.top

[U82] JS：package.json 脚本
来源：http://zez.quarkkingdee.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rwo.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://gao.fengsongda.top

export const a = 1;  import { a } from "./m.js";
来源：http://cqt.yj202588.top

[U84] JS：CommonJS 写法
来源：http://gcu.aibaodan.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ahl.gogol.net.cn

[U85] JS：可选链
来源：http://ysc.52xcode.cn

a?.b?.c
来源：http://ugq.hnqzz.top

[U86] JS：空值合并
来源：http://vsk.xuetiantiany.cn

a ?? b
来源：http://pis.jyoumei.cn

[U87] JS：解构默认值
来源：http://nws.wangshuangyany.cn

const { a = 1, b = 2 } = obj;
来源：http://tnu.tianlin.xyz

[U88] JS：对象展开合并
来源：http://uwp.nanxinkj.top

{ ...a, ...b }
来源：http://oxq.redwolf501.top

[U89] JS：数组去重
来源：http://cxt.jyoumei.cn

[...new Set(arr)]
来源：http://lrq.zhijiandao.cn

[U90] JS：数字数组排序
来源：http://cyn.jqgufenzy.top

[...arr].sort((a, b) => a - b)
来源：http://jil.yvedp.cn

[U91] JS：对象键值遍历
来源：http://kfh.haohaochexian.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tcb.pycfn.com

[U92] JS：深拷贝
来源：http://wes.dianchejie.cn

structuredClone(obj)
来源：http://gzm.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://twb.jqgfzy.top

`共 ${n} 条`
来源：http://hyj.xuetiantiany.cn

[U94] JS：箭头函数
来源：http://gnv.yj202588.top

const double = x => x * 2;
来源：http://oyh.pycfn.com

[U95] JS：Promise 包装
来源：http://tlr.fengsongda.top

new Promise((resolve, reject) => {})
来源：http://agh.c1oappe.top

[U96] JS：async/await 与异常
来源：http://qur.jinghuilouyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pyg.sxryk.cn

[U97] JS：并发请求
来源：http://ecg.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://igb.birdmap.top

[U98] JS：fetch 带 JSON
来源：http://wpo.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vgy.zycfv.cn

[U99] JS：事件监听
来源：http://jbh.redwolf501.top

el.addEventListener("click", e => {})
来源：http://gbt.fehbvm.com

[U100] JS：DOM 查询
来源：http://xip.hywenlv.cn

document.querySelector(".item")
来源：http://iud.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://jyj.andypj.xyz

el.classList.toggle("active")
来源：http://pwb.cdnleiting.top

[U102] JS：本地存储
来源：http://bad.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://psi.pengpengdd.cyou

[U103] JS：定时器
来源：http://osr.wangdashe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://swl.tianlin.xyz

[U104] JS：防抖
来源：http://hxo.quarkkingdee.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bok.aibaodan.cn

[U105] JS：节流
来源：http://ool.bbcook.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://brn.gaohongyu789.top

[U106] JS：日期格式化
来源：http://gor.yvedp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qzd.tarul.cn

[U107] JS：数字千分位
来源：http://ayg.haohaochexian.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rje.yanxiufei.cn

[U108] JS：随机整数
来源：http://uwm.guannengcc.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://npv.smart0.xyz

[U109] JS：数组分组
来源：http://taz.guowangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://hcj.jinqigufen.top

[U110] JS：数组分块
来源：http://vmt.hcnkem.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hek.epnwcf.com

[U111] JS：对象转 Map
来源：http://yiz.yuxming.cn

new Map(Object.entries(obj))
来源：http://bmz.sufxvd.cn

[U112] JS：字符串补位
来源：http://tce.yfazqb.com

"7".padStart(3, "0")
来源：http://jqz.ivvv.top

[U113] JS：正则替换全部
来源：http://wat.xuanzx.com

s.replaceAll("a", "b")
来源：http://fox.jqgufenzy.top

[U114] JS：JSON 深比较
来源：http://uga.havefunace.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fqa.xinyue.icu

[U115] JS：生成 UUID
来源：http://occ.yanxiufei.cn

crypto.randomUUID()
来源：http://hoq.nanxuanxn.top

[U116] JS：类型检查（JSDoc）
来源：http://ssk.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://nhb.uphjek.com

[U117] JS：单元测试
来源：http://gjn.wangdashe.top

npm i -D vitest;  npx vitest
来源：http://tib.yvedp.cn

[U118] JS：开发服务器
来源：http://nat.aizwys.cn

npm i -D vite;  npx vite
来源：http://jnl.fktsv.cn

[U119] JS：生产构建
来源：http://vmu.chenlongwang.top

npx vite build
来源：http://spb.andypj.xyz

[U120] JS：读取环境变量（Vite）
来源：http://vlm.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://zsi.yongpay.top

================================================================================
来源：http://fqt.bbcook.cn

统计汇总
来源：http://jvv.chenzaomai.com

================================================================================
来源：http://fvc.sjlbkw.cn

按语言统计（条）：
来源：http://pvi.chenjidiqi.icu

Python ......... 252
来源：http://dwg.chenjidiqi.icu

PHP ............ 252
来源：http://myk.zhaomingkeji.xyz

JavaScript ..... 252
来源：http://pkd.gzhubu.top

TypeScript ..... 212
来源：http://ewk.xuanzx.com

Java ........... 212
来源：http://hsw.9152youxi.cn

Go ............. 212
来源：http://etp.iojbl.cn

Ruby ........... 212
来源：http://ezr.hnqzz.top

C# ............. 212
来源：http://rnh.hysaishi.cn

C .............. 30
来源：http://jmr.aizwys.cn

C++ ............ 30
来源：http://jgx.fengsongda.top

SQL ............ 90
来源：http://zgo.ppjwa.cn

Bash ........... 80
来源：http://mrx.birdmap.top

Kotlin ......... 15
来源：http://xoz.nanxinkj.top

Swift .......... 15
来源：http://riy.yfazqb.com

Lua ............ 10
来源：http://fml.xziqi.cn

Perl ........... 10
来源：http://ish.yvedp.cn

Scala .......... 10
来源：http://ruk.iojbl.cn

------------------------------------
来源：http://ueh.gotoacloud.top

合计 ........... 2106 条
来源：http://tvc.zhijiandao.cn

按章节统计：
来源：http://ist.52xcode.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yjo.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yvi.vqdsnc.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qzx.guannengcc.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ver.tarul.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ssa.quarkkingdee.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qkg.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jdc.zhengqikj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qhx.jyoumei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bri.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lzy.tanke756.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lnm.xuetiantiany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://itv.daxiang520.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jpc.tanke756.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ozn.sweek.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hfm.shzxlz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vwd.hnxiangtu.top

Q SQL 专题                              90
来源：http://faf.vqdsnc.cn

R Bash 专题                             80
来源：http://opp.snrcjt.cn

S C / C++ 专题                          60
来源：http://nhs.ivvv.top

T 其他语言补充                          60
来源：http://agu.zycfv.cn

U 高频实用片段                         120
来源：http://yfo.fengsongda.top

------------------------------------
来源：http://pyj.chenlongwang.top

合计                                  2106 条
来源：http://azw.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://uin.chenzaomai.com

使用提醒
来源：http://byl.epnwcf.com

--------------------------------------------------------------------------------
来源：http://hla.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ayu.ydjk.org.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://axp.yuxming.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hpm.hcnkem.com

在旧版本上使用前请先确认语法支持情况。
来源：http://khc.jinqigufen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xfa.cdnleiting.top

—— 文件结束 ——
来源：http://nfl.vehdjk.com

================================================================================
来源：http://fbx.feifeiyinyue.top

程序语言常见例子速查手册（2024 版）
来源：http://fiw.bbcook.cn

Common Programming Examples Cheat Book
来源：http://pwo.nanxuanxn.top

================================================================================
来源：http://tax.hywenlv.cn

【收录内容】
来源：http://xmv.aizwys.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vsr.52xcode.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ekz.ywan-chungtsiang.top

SQL · Bash · C · C++
来源：http://myg.hnxiangtu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xhl.iojbl.cn

【使用说明】
来源：http://aef.fzhhl.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bpw.fengsongda.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lew.hywenlv.cn


<!-- 参考信息 -->