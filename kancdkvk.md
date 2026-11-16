代发 wailian999

[U17] Py：初始化日志
来源：http://ipe.fengsongda.top

logging.basicConfig(level=logging.INFO)
来源：http://fsy.tian-w.cn

[U18] Py：预编译正则
来源：http://odk.ybcxt.top

pat = re.compile(r"\d+")
来源：http://snc.hammf.cn

[U19] Py：正则替换带回调
来源：http://eqj.wangshuangyany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://euz.tian-w.cn

[U20] Py：缓存函数结果
来源：http://guf.yuxming.cn

@functools.lru_cache(maxsize=None)
来源：http://hma.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://kma.epnwcf.com

@contextlib.contextmanager
来源：http://cly.cdnleiting.top

[U22] Py：矩阵转置
来源：http://lnb.hnxiangtu.top

list(zip(*m))
来源：http://scl.bbcook.cn

[U23] Py：分块读取大文件
来源：http://qur.fanxiaobao.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pxx.zhiwuduotai.top

[U24] Py：路径操作
来源：http://jou.wangshuangyany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pfx.jinqigufen.top

[U25] Py：CSV 按字典读
来源：http://xuv.zdbjq.cn

csv.DictReader(f)
来源：http://mnz.gaohongyu789.top

[U26] Py：并发下载
来源：http://ait.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zyn.ydzc1.top

[U27] Py：异步 HTTP
来源：http://nce.yuanzhike.top

aiohttp.ClientSession() 配合 async with
来源：http://rwg.jinyuanbaomall.cn

[U28] Py：类型别名
来源：http://rcd.dianchejie.cn

UserId = int
来源：http://kdi.pengpengdd.cyou

[U29] Py：属性校验
来源：http://xgd.chenlongwang.top

@property 与 @x.setter 配合
来源：http://sbe.zhongyouzk.top

[U30] Py：数据类
来源：http://bge.ydjk.org.cn

@dataclass(slots=True)
来源：http://xiw.ivvv.top

[U31] Py：单测
来源：http://ikj.ppjwa.cn

python -m pytest -q
来源：http://pwm.smart0.xyz

[U32] Py：代码格式化
来源：http://tzc.ydzc1.top

ruff format . && ruff check --fix .
来源：http://pka.zhongyouzk.top

[U33] Py：打包发布
来源：http://lcn.yanxiufei.cn

python -m build  （依赖 pyproject.toml）
来源：http://viw.shangyingyoupin.top

[U34] Py：判断编码
来源：http://gvf.ybcxt.top

chardet.detect(raw)
来源：http://ipk.gogol.net.cn

[U35] Py：发送邮件
来源：http://gzw.jqgfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kau.zycfv.cn

[U36] Py：定时任务
来源：http://dju.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://ihy.52xcode.cn

[U37] Py：读写 Excel
来源：http://rsp.zhengqikj.top

pandas.read_excel / DataFrame.to_excel
来源：http://ztj.hammf.cn

[U38] Py：获取脚本所在目录
来源：http://wcz.shanyushiyangkeji.top

Path(__file__).resolve().parent
来源：http://ida.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://rem.hysaishi.cn

sys.stdout.isatty()
来源：http://jfb.redwolf501.top

[U40] Py：打印到标准错误
来源：http://elg.fengsongda.top

print("err", file=sys.stderr)
来源：http://jbi.kuanghao11.cn

[U41] PHP：初始化 Composer 项目
来源：http://qho.bbcook.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tvz.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://xnf.jianghu66.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hvg.vqdsnc.cn

[U43] PHP：声明命名空间
来源：http://vqj.jianghu66.top

namespace App\Http;
来源：http://acw.tian-w.cn

[U44] PHP：开启严格类型
来源：http://pbx.chenlongwang.top

declare(strict_types=1);
来源：http://diu.haohaochexian.top

[U45] PHP：类型声明与返回类型
来源：http://teg.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ojn.sxryk.cn

[U46] PHP：可空类型
来源：http://qhe.hywenlv.cn

?string $name = null
来源：http://rpo.guowangkeji.top

[U47] PHP：联合类型
来源：http://xtc.hywenlv.cn

int|string $id
来源：http://azx.fanxiaobao.xyz

[U48] PHP：纯枚举
来源：http://dra.cashguo.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pqh.zhengqikj.top

[U49] PHP：只读属性
来源：http://gsz.fehbvm.com

public readonly string $name
来源：http://yqc.shanyushiyangkeji.top

[U50] PHP：构造器属性提升
来源：http://iat.316326.xyz

public function __construct(private int $id) {}
来源：http://cof.sysykeji.top

[U51] PHP：数组解构
来源：http://rck.sxryk.cn

[$a, $b] = $arr;
来源：http://tfn.ydjk.org.cn

[U52] PHP：箭头函数
来源：http://uxz.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://dgv.jianghu66.top

[U53] PHP：空合并运算符
来源：http://cfy.xziqi.cn

$v = $a ?? $b ?? "default";
来源：http://zcg.shuidangran.top

[U54] PHP：空安全调用
来源：http://wrb.gogol.net.cn

$obj?->method()
来源：http://nbo.wangdashe.top

[U55] PHP：match 表达式
来源：http://zlw.fktsv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pmm.meibo888.top

[U56] PHP：命名参数
来源：http://hvr.fanxiaobao.xyz

f(a: 1, b: 2)
来源：http://rjo.smart0.xyz

[U57] PHP：字符串插值
来源：http://rlh.shangyingyoupin.top

"值: {$a}"
来源：http://vsh.xinyue.icu

[U58] PHP：数组三件套
来源：http://etd.hesvh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://glu.tanke756.top

[U59] PHP：自定义排序
来源：http://lci.shanyushiyangtech.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jqb.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://erc.quarkkingdee.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vww.dashuyun.cn

[U61] PHP：正则
来源：http://zxx.zhoulong.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zac.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://oms.xylfe.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bsr.fanxiaobao.xyz

[U63] PHP：文件读写
来源：http://eye.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xvx.ybcxt.top

[U64] PHP：目录遍历
来源：http://ded.sufxvd.cn

glob("dir/*.php");  scandir("dir");
来源：http://gvg.mhx1999.top

[U65] PHP：会话
来源：http://eyj.cdnleiting.top

session_start();  $_SESSION["uid"] = 1;
来源：http://oar.gogol.net.cn

[U66] PHP：设置 Cookie
来源：http://jzm.sjlbkw.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://amp.sufxvd.cn

[U67] PHP：处理文件上传
来源：http://fsj.quarkkingdee.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fss.quarkkingdee.top

[U68] PHP：PDO 连接
来源：http://rja.yonumen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pei.yuanzhike.top

[U69] PHP：PDO 预处理
来源：http://blh.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wmr.hcnkem.com

[U70] PHP：PDO 事务
来源：http://sxi.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://snj.guowangkeji.top

[U71] PHP：抛出异常
来源：http://pex.ydjk.org.cn

throw new RuntimeException("失败", 500);
来源：http://scp.316326.xyz

[U72] PHP：写错误日志
来源：http://spf.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://bmz.zhiwuduotai.top

[U73] PHP：读取 ini 配置
来源：http://mam.daxiang520.top

parse_ini_file("config.ini", true)
来源：http://mrd.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://eky.zhiwuduotai.top

getenv("APP_ENV") ?: "production"
来源：http://eea.fktsv.cn

[U75] PHP：依赖注入
来源：http://rqf.wangdashe.top

composer require psr/container
来源：http://kip.shzxlz.cn

[U76] PHP：简单路由
来源：http://kam.cqqwz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tlo.52xcode.cn

[U77] PHP：模板渲染
来源：http://ssj.nanxuanxn.top

composer require twig/twig
来源：http://oka.xinyue.icu

[U78] PHP：单元测试
来源：http://tpo.guowangkeji.top

composer require --dev phpunit/phpunit
来源：http://raz.c1oappe.top

[U79] PHP：静态分析
来源：http://lsq.xziqi.cn

composer require --dev phpstan/phpstan
来源：http://rvu.xingfuxueyuan.xyz

[U80] PHP：代码规范修复
来源：http://gvw.gzhubu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tax.yuxming.cn

[U81] JS：初始化项目
来源：http://bxz.pengpengdd.cyou

npm init -y;  npm i express
来源：http://eai.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://okd.fengsongda.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kud.xziqi.cn

[U83] JS：ES Module 导入导出
来源：http://gkm.sysykeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://vlr.tanke756.top

[U84] JS：CommonJS 写法
来源：http://ilv.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://bhg.hywenlv.cn

[U85] JS：可选链
来源：http://ium.jqgfzy.top

a?.b?.c
来源：http://oef.gaohongyu789.top

[U86] JS：空值合并
来源：http://kdo.cqqwz.cn

a ?? b
来源：http://qrm.fengsongda.top

[U87] JS：解构默认值
来源：http://gsm.bbcook.cn

const { a = 1, b = 2 } = obj;
来源：http://psa.fengsongda.top

[U88] JS：对象展开合并
来源：http://nyt.yangfankeji.com

{ ...a, ...b }
来源：http://iyj.feifeiyinyue.top

[U89] JS：数组去重
来源：http://smu.nanxinkj.top

[...new Set(arr)]
来源：http://ubs.sysykeji.top

[U90] JS：数字数组排序
来源：http://ysi.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://nma.ctjpmb.com

[U91] JS：对象键值遍历
来源：http://xyu.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bux.yanxiufei.cn

[U92] JS：深拷贝
来源：http://wnu.hesvh.cn

structuredClone(obj)
来源：http://grc.jyoumei.cn

[U93] JS：模板字符串
来源：http://vps.snrcjt.cn

`共 ${n} 条`
来源：http://psq.tarul.cn

[U94] JS：箭头函数
来源：http://nab.yj202588.top

const double = x => x * 2;
来源：http://tcp.zhixingplan.top

[U95] JS：Promise 包装
来源：http://mpk.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://lvi.tanke756.top

[U96] JS：async/await 与异常
来源：http://tan.jinqigufen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fzs.meibo888.top

[U97] JS：并发请求
来源：http://zaz.havefunace.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rhc.0kj1m.cn

[U98] JS：fetch 带 JSON
来源：http://agk.mhx1999.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nga.0kj1m.cn

[U99] JS：事件监听
来源：http://ohq.guowangkeji.top

el.addEventListener("click", e => {})
来源：http://wpm.316326.xyz

[U100] JS：DOM 查询
来源：http://bek.zdqjudy.top

document.querySelector(".item")
来源：http://jbm.ctjpmb.com

[U101] JS：classList 操作
来源：http://ycu.ivvv.top

el.classList.toggle("active")
来源：http://abp.yongpay.top

[U102] JS：本地存储
来源：http://hem.nanxuanxn.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qyb.sjlbkw.cn

[U103] JS：定时器
来源：http://wsi.jqgufenzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vvb.wangdashe.top

[U104] JS：防抖
来源：http://ctk.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yvc.aizwys.cn

[U105] JS：节流
来源：http://hcl.jinghuilouyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yhs.zdqjudy.top

[U106] JS：日期格式化
来源：http://ljv.pycfn.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nrk.hesvh.cn

[U107] JS：数字千分位
来源：http://rso.zhongyouzk.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fjn.daxiang520.top

[U108] JS：随机整数
来源：http://bwr.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vlw.nanxuanxn.top

[U109] JS：数组分组
来源：http://luk.fzhhl.top

Object.groupBy(arr, x => x.type)
来源：http://hfh.hywenlv.cn

[U110] JS：数组分块
来源：http://ghg.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ygc.fanxiaobao.xyz

[U111] JS：对象转 Map
来源：http://ywj.cheryme.top

new Map(Object.entries(obj))
来源：http://gga.guannengcc.top

[U112] JS：字符串补位
来源：http://ast.daria6918.cn

"7".padStart(3, "0")
来源：http://hrk.feifeiyinyue.top

[U113] JS：正则替换全部
来源：http://gmt.jqgfzy.top

s.replaceAll("a", "b")
来源：http://tmj.gaohongyu789.top

[U114] JS：JSON 深比较
来源：http://wra.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kdg.havefunace.top

[U115] JS：生成 UUID
来源：http://bgl.shuidangran.top

crypto.randomUUID()
来源：http://nld.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://ukk.jlsjyb.cn

/** @param {string} name */ function f(name) {}
来源：http://xvy.chenjidiqi.icu

[U117] JS：单元测试
来源：http://uft.fktsv.cn

npm i -D vitest;  npx vitest
来源：http://bjz.jlsjyb.cn

[U118] JS：开发服务器
来源：http://ans.yonumen.top

npm i -D vite;  npx vite
来源：http://rzc.cucudq.cn

[U119] JS：生产构建
来源：http://eyq.zhongyouzk.top

npx vite build
来源：http://bfc.shanyushiyangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://tpx.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://tfo.hysaishi.cn

================================================================================
来源：http://rtn.zhoulong.xyz

统计汇总
来源：http://rrg.fehbvm.com

================================================================================
来源：http://xes.yj202588.top

按语言统计（条）：
来源：http://rdk.52xcode.cn

Python ......... 252
来源：http://xkv.shuidangran.top

PHP ............ 252
来源：http://oqf.tian-w.cn

JavaScript ..... 252
来源：http://fiu.zdqjudy.top

TypeScript ..... 212
来源：http://kon.smart0.xyz

Java ........... 212
来源：http://usd.andypj.xyz

Go ............. 212
来源：http://laz.zhijiandao.cn

Ruby ........... 212
来源：http://lzb.zhengqikj.top

C# ............. 212
来源：http://ago.c1oappe.top

C .............. 30
来源：http://bfs.ydzc1.top

C++ ............ 30
来源：http://upl.birdmap.top

SQL ............ 90
来源：http://zix.havefunace.top

Bash ........... 80
来源：http://nja.aibaodan.cn

Kotlin ......... 15
来源：http://snx.ctjpmb.com

Swift .......... 15
来源：http://ggj.feifeiyinyue.top

Lua ............ 10
来源：http://jrd.xingfuxueyuan.xyz

Perl ........... 10
来源：http://poj.mhx1999.top

Scala .......... 10
来源：http://xbr.daxiang520.top

------------------------------------
来源：http://jei.hywenlv.cn

合计 ........... 2106 条
来源：http://ofe.birdmap.top

按章节统计：
来源：http://npu.bjfxy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vij.tarul.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xog.zhixingplan.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mkb.yj202588.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sop.xylfe.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ign.hnxiangtu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xje.jyoumei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qzm.cqqwz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dlm.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://abw.fanxiaobao.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hcc.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gao.yfazqb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jvp.gogol.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fkc.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nhl.yueranfly.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zug.bbcook.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kuf.jinyuanbaomall.cn

Q SQL 专题                              90
来源：http://gno.hfpthk.cn

R Bash 专题                             80
来源：http://eiq.cqqwz.cn

S C / C++ 专题                          60
来源：http://qhd.pycfn.com

T 其他语言补充                          60
来源：http://kys.xylfe.cn

U 高频实用片段                         120
来源：http://dlc.vqdsnc.cn

------------------------------------
来源：http://edp.yvedp.cn

合计                                  2106 条
来源：http://xip.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://vqh.shzxlz.cn

使用提醒
来源：http://wxj.uphjek.com

--------------------------------------------------------------------------------
来源：http://xqn.uphjek.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dzy.aibaodan.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qzv.yvedp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yaj.guannengcc.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ouy.ctjpmb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pzt.gogol.net.cn

—— 文件结束 ——
来源：http://ath.hnxiangtu.top

================================================================================
来源：http://mlh.yangfankeji.com

程序语言常见例子速查手册（2024 版）
来源：http://vot.haohaochexian.top

Common Programming Examples Cheat Book
来源：http://txg.sweek.top

================================================================================
来源：http://ssn.jinqigufen.top

【收录内容】
来源：http://ytv.shzxlz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fhw.havefunace.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bvb.birdmap.top

SQL · Bash · C · C++
来源：http://yzx.aizwys.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eav.zhijiandao.cn

【使用说明】
来源：http://mwt.mhx1999.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wdw.zhengqikj.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kxc.sufxvd.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fdc.yj20258888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://arg.jyoumei.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pad.hnqzz.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ugj.fktsv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wla.aibaodan.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vaj.kuanghao11.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ohs.dianchejie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vqo.chenjidiqi.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eei.zhixingplan.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ndn.uphjek.com

【文件统计】
来源：http://ykp.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gnq.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://sqj.zhoulong.xyz

目  录
来源：http://glg.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://ydf.nanxinkj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gfw.sxryk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hgg.redwolf501.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pvz.zycfv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wrp.jianghu66.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mie.cdnleiting.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zxr.jinqigufen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://skq.meibo888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lmj.52xcode.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://brz.xingfuxueyuan.xyz


<!-- 参考信息 -->