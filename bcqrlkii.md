代发 wailian999

[U15] Py：高精度计时
来源：http://nme.pengpengdd.cyou

t = time.perf_counter()
来源：http://pev.hfpthk.cn

[U16] Py：命令行参数解析
来源：http://sdh.hcnkem.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pno.kuanghao11.cn

[U17] Py：初始化日志
来源：http://nbj.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://nwz.cdnleiting.top

[U18] Py：预编译正则
来源：http://eir.mhx1999.top

pat = re.compile(r"\d+")
来源：http://jaf.sjlbkw.cn

[U19] Py：正则替换带回调
来源：http://fgr.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://who.fengsongda.top

[U20] Py：缓存函数结果
来源：http://ege.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://gqt.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://lbz.hysaishi.cn

@contextlib.contextmanager
来源：http://anc.jinqigfzy.top

[U22] Py：矩阵转置
来源：http://rbz.epnwcf.com

list(zip(*m))
来源：http://ynr.daxiang520.top

[U23] Py：分块读取大文件
来源：http://xhi.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yem.jinqigufen.top

[U24] Py：路径操作
来源：http://hmt.gaohongyu789.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yol.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://bck.zhiwuduotai.top

csv.DictReader(f)
来源：http://tik.zhaomingkeji.xyz

[U26] Py：并发下载
来源：http://xje.daria6918.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yho.aibaodan.cn

[U27] Py：异步 HTTP
来源：http://nqk.ywan-chungtsiang.top

aiohttp.ClientSession() 配合 async with
来源：http://qys.tarul.cn

[U28] Py：类型别名
来源：http://dxc.hfpthk.cn

UserId = int
来源：http://jtp.ppjwa.cn

[U29] Py：属性校验
来源：http://ulu.xziqi.cn

@property 与 @x.setter 配合
来源：http://oge.shanyushiyangtech.top

[U30] Py：数据类
来源：http://fki.xinyue.icu

@dataclass(slots=True)
来源：http://tcb.zdbjq.cn

[U31] Py：单测
来源：http://jra.xinyue.icu

python -m pytest -q
来源：http://lta.jyoumei.cn

[U32] Py：代码格式化
来源：http://lrg.yuxming.cn

ruff format . && ruff check --fix .
来源：http://ohg.yueranfly.top

[U33] Py：打包发布
来源：http://bff.aibaodan.cn

python -m build  （依赖 pyproject.toml）
来源：http://uay.gotoacloud.top

[U34] Py：判断编码
来源：http://tsf.jinyuanbaomall.cn

chardet.detect(raw)
来源：http://tdz.guannengcc.top

[U35] Py：发送邮件
来源：http://odm.jinyuanbaomall.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tpg.tanke756.top

[U36] Py：定时任务
来源：http://lqg.yfazqb.com

schedule.every(10).minutes.do(job)
来源：http://rjc.zhongyouzk.top

[U37] Py：读写 Excel
来源：http://mbv.xuetiantiany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fus.jqgfzy.top

[U38] Py：获取脚本所在目录
来源：http://pje.jqgfzy.top

Path(__file__).resolve().parent
来源：http://paf.chenzaomai.com

[U39] Py：判断是否在交互环境
来源：http://psg.yuxming.cn

sys.stdout.isatty()
来源：http://vzm.ywan-chungtsiang.top

[U40] Py：打印到标准错误
来源：http://vrh.feifeiyinyue.top

print("err", file=sys.stderr)
来源：http://ems.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://ctk.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lcq.chenzaomai.com

[U42] PHP：PSR-4 自动加载
来源：http://ukr.hcnkem.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ign.yj20258.top

[U43] PHP：声明命名空间
来源：http://xkv.gotoacloud.top

namespace App\Http;
来源：http://nnf.hfpthk.cn

[U44] PHP：开启严格类型
来源：http://dld.wangdashe.top

declare(strict_types=1);
来源：http://puu.zhoulong.xyz

[U45] PHP：类型声明与返回类型
来源：http://aok.haohaochexian.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ngr.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://ick.316326.xyz

?string $name = null
来源：http://vve.zhoulong.xyz

[U47] PHP：联合类型
来源：http://kok.ehwqpu.com

int|string $id
来源：http://zsn.zhengqikj.top

[U48] PHP：纯枚举
来源：http://par.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mjx.tarul.cn

[U49] PHP：只读属性
来源：http://itr.shuidangran.top

public readonly string $name
来源：http://mdv.zhongyouzk.top

[U50] PHP：构造器属性提升
来源：http://flp.mhx1999.top

public function __construct(private int $id) {}
来源：http://dbf.kuanghao11.cn

[U51] PHP：数组解构
来源：http://qxt.yongpay.top

[$a, $b] = $arr;
来源：http://yzm.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://dwo.cashguo.top

$double = fn($x) => $x * 2;
来源：http://qcf.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://ggd.ehwqpu.com

$v = $a ?? $b ?? "default";
来源：http://frl.zhaomingkeji.xyz

[U54] PHP：空安全调用
来源：http://oee.ydjk.org.cn

$obj?->method()
来源：http://qse.dashuyun.cn

[U55] PHP：match 表达式
来源：http://bzm.ctjpmb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mlz.xylfe.cn

[U56] PHP：命名参数
来源：http://yfs.52xcode.cn

f(a: 1, b: 2)
来源：http://ics.cqqwz.cn

[U57] PHP：字符串插值
来源：http://arc.hysaishi.cn

"值: {$a}"
来源：http://ckf.sufxvd.cn

[U58] PHP：数组三件套
来源：http://znw.hysaishi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lsx.c1oappe.top

[U59] PHP：自定义排序
来源：http://tuv.sweek.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iqe.daxiang520.top

[U60] PHP：JSON 编解码
来源：http://wyq.zdbjq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lkp.xziqi.cn

[U61] PHP：正则
来源：http://xyc.birdmap.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tyt.cqqwz.cn

[U62] PHP：日期对象
来源：http://lie.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cbg.yangfankeji.com

[U63] PHP：文件读写
来源：http://naf.fktsv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fjg.zhaomingkeji.xyz

[U64] PHP：目录遍历
来源：http://fqw.zhongyouzk.top

glob("dir/*.php");  scandir("dir");
来源：http://xwo.dashuyun.cn

[U65] PHP：会话
来源：http://hah.jinqigufen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://thl.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://yts.redwolf501.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yfl.ywan-chungtsiang.top

[U67] PHP：处理文件上传
来源：http://wdj.fanxiaobao.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ktj.nwbrower.top

[U68] PHP：PDO 连接
来源：http://fns.yanxiufei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ohd.ywan-chungtsiang.top

[U69] PHP：PDO 预处理
来源：http://ndu.ivvv.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hsf.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://uqq.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bex.yanxiufei.cn

[U71] PHP：抛出异常
来源：http://fjb.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://ujj.hnqzz.top

[U72] PHP：写错误日志
来源：http://vbo.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://grt.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://lhw.ydjk.org.cn

parse_ini_file("config.ini", true)
来源：http://fyh.guowangkeji.top

[U74] PHP：读取环境变量
来源：http://krb.cucudq.cn

getenv("APP_ENV") ?: "production"
来源：http://hur.epnwcf.com

[U75] PHP：依赖注入
来源：http://nzq.snrcjt.cn

composer require psr/container
来源：http://hul.yuanzhike.top

[U76] PHP：简单路由
来源：http://kdo.cucudq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zht.sufxvd.cn

[U77] PHP：模板渲染
来源：http://bzy.jqgfzy.top

composer require twig/twig
来源：http://iiu.yangfankeji.com

[U78] PHP：单元测试
来源：http://qax.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://duz.wangshuangyany.cn

[U79] PHP：静态分析
来源：http://ffo.gotoacloud.top

composer require --dev phpstan/phpstan
来源：http://pwe.guowangkeji.top

[U80] PHP：代码规范修复
来源：http://wug.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ztq.chenzaomai.com

[U81] JS：初始化项目
来源：http://gbg.jinyuanbaomall.cn

npm init -y;  npm i express
来源：http://yjz.sweek.top

[U82] JS：package.json 脚本
来源：http://cpt.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tpn.hywenlv.cn

[U83] JS：ES Module 导入导出
来源：http://uwb.hfpthk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qyn.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://xqr.jinyuanbaomall.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hdv.hysaishi.cn

[U85] JS：可选链
来源：http://evm.ehwqpu.com

a?.b?.c
来源：http://imn.sweek.top

[U86] JS：空值合并
来源：http://oyw.fanxiaobao.xyz

a ?? b
来源：http://mzt.zhiwuduotai.top

[U87] JS：解构默认值
来源：http://kno.tian-w.cn

const { a = 1, b = 2 } = obj;
来源：http://gok.jqgfzy.top

[U88] JS：对象展开合并
来源：http://mzq.andypj.xyz

{ ...a, ...b }
来源：http://uix.xylfe.cn

[U89] JS：数组去重
来源：http://vlo.tian-w.cn

[...new Set(arr)]
来源：http://ovv.vehdjk.com

[U90] JS：数字数组排序
来源：http://tam.yj202588.top

[...arr].sort((a, b) => a - b)
来源：http://jag.c1oappe.top

[U91] JS：对象键值遍历
来源：http://gzv.chenjidiqi.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gsl.daxiang520.top

[U92] JS：深拷贝
来源：http://evd.yj20258.top

structuredClone(obj)
来源：http://lwq.nwbrower.top

[U93] JS：模板字符串
来源：http://yxo.ivvv.top

`共 ${n} 条`
来源：http://mbb.birdmap.top

[U94] JS：箭头函数
来源：http://ygb.shanyushiyangtech.top

const double = x => x * 2;
来源：http://cqh.zhiwuduotai.top

[U95] JS：Promise 包装
来源：http://hrw.redwolf501.top

new Promise((resolve, reject) => {})
来源：http://njl.xinyue.icu

[U96] JS：async/await 与异常
来源：http://rsb.feifeiyinyue.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zcq.zdbjq.cn

[U97] JS：并发请求
来源：http://yks.nanxinkj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nhx.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://krn.shuidangran.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mjs.zdbjq.cn

[U99] JS：事件监听
来源：http://heg.zhixingplan.top

el.addEventListener("click", e => {})
来源：http://cjn.9152youxi.cn

[U100] JS：DOM 查询
来源：http://qwy.zycfv.cn

document.querySelector(".item")
来源：http://eoo.316326.xyz

[U101] JS：classList 操作
来源：http://tjt.ivvv.top

el.classList.toggle("active")
来源：http://ekm.hesvh.cn

[U102] JS：本地存储
来源：http://zsn.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://iaq.sjlbkw.cn

[U103] JS：定时器
来源：http://uph.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vro.nanxuanxn.top

[U104] JS：防抖
来源：http://hek.sysykeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ndj.xinyue.icu

[U105] JS：节流
来源：http://ewa.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fkz.hnqzz.top

[U106] JS：日期格式化
来源：http://zoy.chenjidiqi.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://awx.jinqigufen.top

[U107] JS：数字千分位
来源：http://mso.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://erw.zycfv.cn

[U108] JS：随机整数
来源：http://ubl.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dit.tian-w.cn

[U109] JS：数组分组
来源：http://tet.yj20258.top

Object.groupBy(arr, x => x.type)
来源：http://lnr.gogol.net.cn

[U110] JS：数组分块
来源：http://sip.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zfc.dianchejie.cn

[U111] JS：对象转 Map
来源：http://wrm.cqqwz.cn

new Map(Object.entries(obj))
来源：http://gbn.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://wyg.nwbrower.top

"7".padStart(3, "0")
来源：http://yxl.guannengcc.top

[U113] JS：正则替换全部
来源：http://rpy.zhoulong.xyz

s.replaceAll("a", "b")
来源：http://tay.cashguo.top

[U114] JS：JSON 深比较
来源：http://ppe.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://whl.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://fxt.gzhubu.top

crypto.randomUUID()
来源：http://vrd.ydzc1.top

[U116] JS：类型检查（JSDoc）
来源：http://hcl.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://wxz.yangfankeji.com

[U117] JS：单元测试
来源：http://izf.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://sii.c1oappe.top

[U118] JS：开发服务器
来源：http://ndk.smart0.xyz

npm i -D vite;  npx vite
来源：http://uzw.bjfxy.top

[U119] JS：生产构建
来源：http://apl.dianchejie.cn

npx vite build
来源：http://hsk.hammf.cn

[U120] JS：读取环境变量（Vite）
来源：http://qgv.gzhubu.top

import.meta.env.VITE_API_URL
来源：http://pwg.fengsongda.top

================================================================================
来源：http://hwq.sufxvd.cn

统计汇总
来源：http://rco.hcnkem.com

================================================================================
来源：http://vcm.fanxiaobao.xyz

按语言统计（条）：
来源：http://aol.dashuyun.cn

Python ......... 252
来源：http://xms.nanxinkj.top

PHP ............ 252
来源：http://wmg.gaohongyu789.top

JavaScript ..... 252
来源：http://qyc.gotoacloud.top

TypeScript ..... 212
来源：http://aqz.yvedp.cn

Java ........... 212
来源：http://zgb.shangyingyoupin.top

Go ............. 212
来源：http://dpy.fanxiaobao.xyz

Ruby ........... 212
来源：http://amj.xylfe.cn

C# ............. 212
来源：http://xre.yj20258.top

C .............. 30
来源：http://qoj.smart0.xyz

C++ ............ 30
来源：http://swh.chenzaomai.com

SQL ............ 90
来源：http://zpg.xinyue.icu

Bash ........... 80
来源：http://xgq.jqgfzy.top

Kotlin ......... 15
来源：http://zro.feifeiyinyue.top

Swift .......... 15
来源：http://raq.shanyushiyangtech.top

Lua ............ 10
来源：http://yur.uphjek.com

Perl ........... 10
来源：http://xza.chenlongwang.top

Scala .......... 10
来源：http://xnj.nwbrower.top

------------------------------------
来源：http://csu.andypj.xyz

合计 ........... 2106 条
来源：http://sru.vqdsnc.cn

按章节统计：
来源：http://teq.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cgg.redwolf501.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tsd.9152youxi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yep.yfazqb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ezv.yfazqb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://utp.gogol.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hfc.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kos.pycfn.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wde.ivvv.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qzz.fanxiaobao.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ulb.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vhy.xylfe.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kmf.sweek.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cfx.zhijiandao.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blv.cashguo.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pdz.sweek.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tob.gzhubu.top

Q SQL 专题                              90
来源：http://psj.52xcode.cn

R Bash 专题                             80
来源：http://uyp.fktsv.cn

S C / C++ 专题                          60
来源：http://uei.nanxuanxn.top

T 其他语言补充                          60
来源：http://fyc.aibaodan.cn

U 高频实用片段                         120
来源：http://rgt.tian-w.cn

------------------------------------
来源：http://ogl.jinqigufen.top

合计                                  2106 条
来源：http://siq.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://wzo.0kj1m.cn

使用提醒
来源：http://zfr.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://dsm.fehbvm.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nip.0kj1m.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sbz.gaohongyu789.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ngd.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://unu.snrcjt.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yxi.jianghu66.top

—— 文件结束 ——
来源：http://rtb.tianlin.xyz

================================================================================
来源：http://fzg.shuidangran.top

程序语言常见例子速查手册（2024 版）
来源：http://sne.vehdjk.com

Common Programming Examples Cheat Book
来源：http://uos.dianchejie.cn

================================================================================
来源：http://yrn.yj20258.top

【收录内容】
来源：http://rsp.zhoulong.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://zhz.xylfe.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nag.shanyushiyangkeji.top

SQL · Bash · C · C++
来源：http://ufb.yanxiufei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qkw.hfpthk.cn

【使用说明】
来源：http://jwx.vehdjk.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://znl.guowangkeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uio.ywan-chungtsiang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kos.chenzaomai.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jbm.ydzc1.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zhg.xuanzx.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kdk.daxiang520.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://doa.fehbvm.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dsu.jinqigfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://irt.fktsv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gqw.birdmap.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gbj.yvedp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vab.hfpthk.cn

【文件统计】
来源：http://lpw.yonumen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dzn.havefunace.top

--------------------------------------------------------------------------------
来源：http://ngn.sxryk.cn

目  录
来源：http://yth.yj202588.top

--------------------------------------------------------------------------------
来源：http://dxp.svipenyu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fyt.iojbl.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tif.guowangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pmg.c1oappe.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kxf.gzhubu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hef.shanyushiyangtech.top


<!-- 参考信息 -->