代发 wailian999

[U07] Py：反转字典键值
来源：http://ttb.cashguo.top

{v: k for k, v in d.items()}
来源：http://vic.fehbvm.com

[U08] Py：展平二维列表
来源：http://mzb.nanxinkj.top

[y for x in nested for y in x]
来源：http://lxu.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://vhq.yj202588.top

max(d, key=d.get)
来源：http://fzj.sufxvd.cn

[U10] Py：按值排序字典
来源：http://nog.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zcg.fktsv.cn

[U11] Py：生成器表达式
来源：http://zae.yj202588.top

(x * 2 for x in arr)
来源：http://lli.gotoacloud.top

[U12] Py：取出现最多的 3 个元素
来源：http://asy.sufxvd.cn

Counter(arr).most_common(3)
来源：http://lek.ybcxt.top

[U13] Py：固定长度队列
来源：http://wwq.shuidangran.top

deque(maxlen=10)
来源：http://wwg.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://xyy.chenjidiqi.icu

defaultdict(list)
来源：http://bma.yj202588.top

[U15] Py：高精度计时
来源：http://jzx.hysaishi.cn

t = time.perf_counter()
来源：http://uco.snrcjt.cn

[U16] Py：命令行参数解析
来源：http://keg.tanke756.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xwn.hnqzz.top

[U17] Py：初始化日志
来源：http://qci.fzhhl.top

logging.basicConfig(level=logging.INFO)
来源：http://trt.cashguo.top

[U18] Py：预编译正则
来源：http://wnz.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://ouu.cheryme.top

[U19] Py：正则替换带回调
来源：http://jok.sysykeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sje.ydzc1.top

[U20] Py：缓存函数结果
来源：http://cpx.jianghu66.top

@functools.lru_cache(maxsize=None)
来源：http://syo.jinghuilouyu.cn

[U21] Py：自定义上下文管理器
来源：http://wpq.hywenlv.cn

@contextlib.contextmanager
来源：http://cia.shangyingyoupin.top

[U22] Py：矩阵转置
来源：http://xjs.yj20258.top

list(zip(*m))
来源：http://fob.hcnkem.com

[U23] Py：分块读取大文件
来源：http://qam.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rpr.gotoacloud.top

[U24] Py：路径操作
来源：http://rsq.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xdu.cdnleiting.top

[U25] Py：CSV 按字典读
来源：http://vwv.ydzc1.top

csv.DictReader(f)
来源：http://yyz.fehbvm.com

[U26] Py：并发下载
来源：http://wzf.jyoumei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bdn.iojbl.cn

[U27] Py：异步 HTTP
来源：http://ynr.ehwqpu.com

aiohttp.ClientSession() 配合 async with
来源：http://lrs.jqgfzy.top

[U28] Py：类型别名
来源：http://uxw.ctjpmb.com

UserId = int
来源：http://ddw.tarul.cn

[U29] Py：属性校验
来源：http://lhu.tian-w.cn

@property 与 @x.setter 配合
来源：http://zrs.zhiwuduotai.top

[U30] Py：数据类
来源：http://gcd.tanke756.top

@dataclass(slots=True)
来源：http://jkl.jinqigfzy.top

[U31] Py：单测
来源：http://rbt.smart0.xyz

python -m pytest -q
来源：http://uxo.9152youxi.cn

[U32] Py：代码格式化
来源：http://iby.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://uxv.tianlin.xyz

[U33] Py：打包发布
来源：http://ezk.pycfn.com

python -m build  （依赖 pyproject.toml）
来源：http://plp.sweek.top

[U34] Py：判断编码
来源：http://igs.xinyue.icu

chardet.detect(raw)
来源：http://eim.aizwys.cn

[U35] Py：发送邮件
来源：http://khf.cqqwz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vat.haohaochexian.top

[U36] Py：定时任务
来源：http://obz.zhongyouzk.top

schedule.every(10).minutes.do(job)
来源：http://dui.tarul.cn

[U37] Py：读写 Excel
来源：http://czs.jyoumei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://psd.xylfe.cn

[U38] Py：获取脚本所在目录
来源：http://sch.jyoumei.cn

Path(__file__).resolve().parent
来源：http://fyd.jyoumei.cn

[U39] Py：判断是否在交互环境
来源：http://mvz.shanyushiyangkeji.top

sys.stdout.isatty()
来源：http://rnj.xziqi.cn

[U40] Py：打印到标准错误
来源：http://ssx.jinghuilouyu.cn

print("err", file=sys.stderr)
来源：http://xck.xinyue.icu

[U41] PHP：初始化 Composer 项目
来源：http://nen.52xcode.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oco.chenlongwang.top

[U42] PHP：PSR-4 自动加载
来源：http://pjg.cdnleiting.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lqm.cashguo.top

[U43] PHP：声明命名空间
来源：http://uej.smart0.xyz

namespace App\Http;
来源：http://yix.yfazqb.com

[U44] PHP：开启严格类型
来源：http://qij.chenlongwang.top

declare(strict_types=1);
来源：http://yjr.cdnleiting.top

[U45] PHP：类型声明与返回类型
来源：http://see.wangdashe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kqh.chenjidiqi.icu

[U46] PHP：可空类型
来源：http://kfz.52xcode.cn

?string $name = null
来源：http://dio.jinqigfzy.top

[U47] PHP：联合类型
来源：http://mob.pycfn.com

int|string $id
来源：http://puh.cdnleiting.top

[U48] PHP：纯枚举
来源：http://tuc.aibaodan.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hdw.jqgfzy.top

[U49] PHP：只读属性
来源：http://nat.cucudq.cn

public readonly string $name
来源：http://ftm.gaohongyu789.top

[U50] PHP：构造器属性提升
来源：http://kdz.aibaodan.cn

public function __construct(private int $id) {}
来源：http://zby.yanxiufei.cn

[U51] PHP：数组解构
来源：http://fma.jqgfzy.top

[$a, $b] = $arr;
来源：http://sne.cdnleiting.top

[U52] PHP：箭头函数
来源：http://dym.fanxiaobao.xyz

$double = fn($x) => $x * 2;
来源：http://nfr.52xcode.cn

[U53] PHP：空合并运算符
来源：http://ear.xziqi.cn

$v = $a ?? $b ?? "default";
来源：http://kip.cdnleiting.top

[U54] PHP：空安全调用
来源：http://trj.c1oappe.top

$obj?->method()
来源：http://hrh.shangyingyoupin.top

[U55] PHP：match 表达式
来源：http://teb.ywan-chungtsiang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lcx.yongpay.top

[U56] PHP：命名参数
来源：http://ryp.zhongyouzk.top

f(a: 1, b: 2)
来源：http://azd.shuidangran.top

[U57] PHP：字符串插值
来源：http://ucc.chenzaomai.com

"值: {$a}"
来源：http://pua.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://haz.havefunace.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yku.hammf.cn

[U59] PHP：自定义排序
来源：http://xrb.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bjv.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://tyh.gotoacloud.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://chq.yanxiufei.cn

[U61] PHP：正则
来源：http://ppt.hesvh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xup.cashguo.top

[U62] PHP：日期对象
来源：http://wxl.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://chg.gaohongyu789.top

[U63] PHP：文件读写
来源：http://ltj.yj20258888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lnf.shanyushiyangtech.top

[U64] PHP：目录遍历
来源：http://urv.bbcook.cn

glob("dir/*.php");  scandir("dir");
来源：http://vmi.feifeiyinyue.top

[U65] PHP：会话
来源：http://lin.wangshuangyany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xiz.zhengqikj.top

[U66] PHP：设置 Cookie
来源：http://otc.dashuyun.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zcq.zhongyouzk.top

[U67] PHP：处理文件上传
来源：http://fyd.52xcode.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hqv.shanyushiyangtech.top

[U68] PHP：PDO 连接
来源：http://mhf.zhoulong.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lpj.jiagoushi.top

[U69] PHP：PDO 预处理
来源：http://zrf.haohaochexian.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ixx.jinyuanbaomall.cn

[U70] PHP：PDO 事务
来源：http://ljp.bbcook.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mar.nanxuanxn.top

[U71] PHP：抛出异常
来源：http://alk.hammf.cn

throw new RuntimeException("失败", 500);
来源：http://jql.jianghu66.top

[U72] PHP：写错误日志
来源：http://eln.tian-w.cn

error_log("失败: " . $e->getMessage());
来源：http://lwx.sxryk.cn

[U73] PHP：读取 ini 配置
来源：http://ohs.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://nvs.yj202588.top

[U74] PHP：读取环境变量
来源：http://wxi.xuanzx.com

getenv("APP_ENV") ?: "production"
来源：http://gbn.xingfuxueyuan.xyz

[U75] PHP：依赖注入
来源：http://yby.fzhhl.top

composer require psr/container
来源：http://pcu.cashguo.top

[U76] PHP：简单路由
来源：http://bwq.yfazqb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qtq.hysaishi.cn

[U77] PHP：模板渲染
来源：http://zwl.redwolf501.top

composer require twig/twig
来源：http://wqg.nanxinkj.top

[U78] PHP：单元测试
来源：http://tth.birdmap.top

composer require --dev phpunit/phpunit
来源：http://vgl.sxryk.cn

[U79] PHP：静态分析
来源：http://wwq.guowangkeji.top

composer require --dev phpstan/phpstan
来源：http://blc.pycfn.com

[U80] PHP：代码规范修复
来源：http://jjh.zhongyouzk.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rbf.hcnkem.com

[U81] JS：初始化项目
来源：http://yqm.zhaomingkeji.xyz

npm init -y;  npm i express
来源：http://qsi.yj202588.top

[U82] JS：package.json 脚本
来源：http://sfw.epnwcf.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qex.haohaochexian.top

[U83] JS：ES Module 导入导出
来源：http://kae.hywenlv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lhx.zdqjudy.top

[U84] JS：CommonJS 写法
来源：http://gaf.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://nzf.andypj.xyz

[U85] JS：可选链
来源：http://esh.smart0.xyz

a?.b?.c
来源：http://yjr.bbcook.cn

[U86] JS：空值合并
来源：http://sls.fengsongda.top

a ?? b
来源：http://xwp.shzxlz.cn

[U87] JS：解构默认值
来源：http://uwr.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://hyo.yj20258888.top

[U88] JS：对象展开合并
来源：http://svk.hnqzz.top

{ ...a, ...b }
来源：http://lqn.xziqi.cn

[U89] JS：数组去重
来源：http://pjm.sufxvd.cn

[...new Set(arr)]
来源：http://yhp.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://ctv.pycfn.com

[...arr].sort((a, b) => a - b)
来源：http://hdn.ivvv.top

[U91] JS：对象键值遍历
来源：http://clr.9152youxi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vza.ybcxt.top

[U92] JS：深拷贝
来源：http://eqx.xinyue.icu

structuredClone(obj)
来源：http://cyv.gotoacloud.top

[U93] JS：模板字符串
来源：http://fgf.ydzc1.top

`共 ${n} 条`
来源：http://hkl.quarkkingdee.top

[U94] JS：箭头函数
来源：http://ihu.fktsv.cn

const double = x => x * 2;
来源：http://bng.wangdashe.top

[U95] JS：Promise 包装
来源：http://kmy.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://clt.bjfxy.top

[U96] JS：async/await 与异常
来源：http://tka.xinyue.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nrp.epnwcf.com

[U97] JS：并发请求
来源：http://ysa.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://veb.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://zbj.hysaishi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fmh.wangshuangyany.cn

[U99] JS：事件监听
来源：http://hei.gzhubu.top

el.addEventListener("click", e => {})
来源：http://jvl.ivvv.top

[U100] JS：DOM 查询
来源：http://dqf.sufxvd.cn

document.querySelector(".item")
来源：http://ewk.shzxlz.cn

[U101] JS：classList 操作
来源：http://kqo.yj20258888.top

el.classList.toggle("active")
来源：http://vjb.gaohongyu789.top

[U102] JS：本地存储
来源：http://ook.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jnt.gzhubu.top

[U103] JS：定时器
来源：http://bfs.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wny.jinqigufen.top

[U104] JS：防抖
来源：http://pcs.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jsh.bbcook.cn

[U105] JS：节流
来源：http://udf.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://puw.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://fws.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lcg.jianghu66.top

[U107] JS：数字千分位
来源：http://odm.gotoacloud.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wrg.bjfxy.top

[U108] JS：随机整数
来源：http://aei.0kj1m.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://orm.ydzc1.top

[U109] JS：数组分组
来源：http://zoq.fehbvm.com

Object.groupBy(arr, x => x.type)
来源：http://rdp.tian-w.cn

[U110] JS：数组分块
来源：http://fti.fehbvm.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ctm.birdmap.top

[U111] JS：对象转 Map
来源：http://ses.cashguo.top

new Map(Object.entries(obj))
来源：http://yev.nanxuanxn.top

[U112] JS：字符串补位
来源：http://muj.fehbvm.com

"7".padStart(3, "0")
来源：http://hwy.zdbjq.cn

[U113] JS：正则替换全部
来源：http://ymv.c1oappe.top

s.replaceAll("a", "b")
来源：http://yyc.pengpengdd.cyou

[U114] JS：JSON 深比较
来源：http://yab.nwbrower.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://uov.shuidangran.top

[U115] JS：生成 UUID
来源：http://vfg.shuidangran.top

crypto.randomUUID()
来源：http://hxc.yfazqb.com

[U116] JS：类型检查（JSDoc）
来源：http://qwp.jinghuilouyu.cn

/** @param {string} name */ function f(name) {}
来源：http://mma.hnxiangtu.top

[U117] JS：单元测试
来源：http://meq.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://uum.redwolf501.top

[U118] JS：开发服务器
来源：http://srs.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://bjv.sxryk.cn

[U119] JS：生产构建
来源：http://eme.snrcjt.cn

npx vite build
来源：http://ndq.mhx1999.top

[U120] JS：读取环境变量（Vite）
来源：http://pyp.tianlin.xyz

import.meta.env.VITE_API_URL
来源：http://cxa.zhijiandao.cn

================================================================================
来源：http://sxx.nanxuanxn.top

统计汇总
来源：http://qga.pengpengdd.cyou

================================================================================
来源：http://ecm.fanxiaobao.xyz

按语言统计（条）：
来源：http://fzw.tanke756.top

Python ......... 252
来源：http://oke.gzhubu.top

PHP ............ 252
来源：http://gay.bbcook.cn

JavaScript ..... 252
来源：http://sxf.gotoacloud.top

TypeScript ..... 212
来源：http://vsd.tarul.cn

Java ........... 212
来源：http://syg.ydzc1.top

Go ............. 212
来源：http://xxd.birdmap.top

Ruby ........... 212
来源：http://aln.aibaodan.cn

C# ............. 212
来源：http://thi.ywan-chungtsiang.top

C .............. 30
来源：http://ldn.yj20258888.top

C++ ............ 30
来源：http://pjd.svipenyu.cn

SQL ............ 90
来源：http://mrc.tanke756.top

Bash ........... 80
来源：http://lsd.iojbl.cn

Kotlin ......... 15
来源：http://haz.iojbl.cn

Swift .......... 15
来源：http://xdi.xylfe.cn

Lua ............ 10
来源：http://wbo.shanyushiyangtech.top

Perl ........... 10
来源：http://mdr.zdbjq.cn

Scala .......... 10
来源：http://jej.wangdashe.top

------------------------------------
来源：http://byp.gaohongyu789.top

合计 ........... 2106 条
来源：http://loz.xylfe.cn

按章节统计：
来源：http://zru.zhiwuduotai.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://aer.cucudq.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hso.jinqigfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ovi.fehbvm.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dzo.epnwcf.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ynq.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kfv.xylfe.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jwq.ppjwa.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ksh.xylfe.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://prv.cdnleiting.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gcy.yongpay.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://icp.quarkkingdee.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rdw.hesvh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gil.hysaishi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pin.yj202588.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kai.fanxiaobao.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://trp.chenlongwang.top

Q SQL 专题                              90
来源：http://myc.zhengqikj.top

R Bash 专题                             80
来源：http://fdx.ybcxt.top

S C / C++ 专题                          60
来源：http://ovs.ybcxt.top

T 其他语言补充                          60
来源：http://ahd.sweek.top

U 高频实用片段                         120
来源：http://fgq.zhaomingkeji.xyz

------------------------------------
来源：http://amg.jlsjyb.cn

合计                                  2106 条
来源：http://lqj.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://wab.fktsv.cn

使用提醒
来源：http://ivt.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://zto.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xxa.yongpay.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lix.jyoumei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vpy.sweek.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fpr.xinyue.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xic.tian-w.cn

—— 文件结束 ——
来源：http://ldk.iojbl.cn

================================================================================
来源：http://nkz.vqdsnc.cn

程序语言常见例子速查手册（2024 版）
来源：http://bcz.jlsjyb.cn

Common Programming Examples Cheat Book
来源：http://ncg.cucudq.cn

================================================================================
来源：http://ile.hywenlv.cn

【收录内容】
来源：http://mhc.yangfankeji.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://fpa.guannengcc.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fmi.bjfxy.top

SQL · Bash · C · C++
来源：http://zwf.nanxinkj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xar.cdnleiting.top

【使用说明】
来源：http://puz.fzhhl.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ibh.wangshuangyany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zfw.bjfxy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://otl.jqgfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://edf.nanxinkj.top

Bash:  Shell         C:     C             C++:   C++
来源：http://bza.quarkkingdee.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bfm.yueranfly.top


<!-- 参考信息 -->