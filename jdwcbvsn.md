代发 wailian999

[U23] Py：分块读取大文件
来源：http://hfd.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wmn.dianchejie.cn

[U24] Py：路径操作
来源：http://xwm.sjlbkw.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ftf.sxryk.cn

[U25] Py：CSV 按字典读
来源：http://ffv.gotoacloud.top

csv.DictReader(f)
来源：http://lhe.hywenlv.cn

[U26] Py：并发下载
来源：http://sjr.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://apt.aizwys.cn

[U27] Py：异步 HTTP
来源：http://qvr.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://fle.chenzaomai.com

[U28] Py：类型别名
来源：http://kyt.cqqwz.cn

UserId = int
来源：http://cdr.yj202588.top

[U29] Py：属性校验
来源：http://cno.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://gra.ydjk.org.cn

[U30] Py：数据类
来源：http://vyr.zhaomingkeji.xyz

@dataclass(slots=True)
来源：http://tib.hywenlv.cn

[U31] Py：单测
来源：http://jsg.bjfxy.top

python -m pytest -q
来源：http://cit.bjfxy.top

[U32] Py：代码格式化
来源：http://rit.c1oappe.top

ruff format . && ruff check --fix .
来源：http://vdx.cdnleiting.top

[U33] Py：打包发布
来源：http://xev.xziqi.cn

python -m build  （依赖 pyproject.toml）
来源：http://szg.yj202588.top

[U34] Py：判断编码
来源：http://ojl.shangyingyoupin.top

chardet.detect(raw)
来源：http://jos.chenzaomai.com

[U35] Py：发送邮件
来源：http://qyo.shanyushiyangtech.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rqf.zhiwuduotai.top

[U36] Py：定时任务
来源：http://uid.ywan-chungtsiang.top

schedule.every(10).minutes.do(job)
来源：http://exm.guannengcc.top

[U37] Py：读写 Excel
来源：http://ooo.guowangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://nql.tarul.cn

[U38] Py：获取脚本所在目录
来源：http://jwv.cashguo.top

Path(__file__).resolve().parent
来源：http://lpr.hesvh.cn

[U39] Py：判断是否在交互环境
来源：http://zyh.iojbl.cn

sys.stdout.isatty()
来源：http://lfl.shanyushiyangtech.top

[U40] Py：打印到标准错误
来源：http://ntf.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://xsx.vehdjk.com

[U41] PHP：初始化 Composer 项目
来源：http://ltu.xylfe.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://giy.jiagoushi.top

[U42] PHP：PSR-4 自动加载
来源：http://eaw.hnxiangtu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dze.yongpay.top

[U43] PHP：声明命名空间
来源：http://bbq.c1oappe.top

namespace App\Http;
来源：http://zak.cucudq.cn

[U44] PHP：开启严格类型
来源：http://gcb.sxryk.cn

declare(strict_types=1);
来源：http://swy.redwolf501.top

[U45] PHP：类型声明与返回类型
来源：http://tvq.daxiang520.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vhq.kuanghao11.cn

[U46] PHP：可空类型
来源：http://nml.xuetiantiany.cn

?string $name = null
来源：http://tum.guannengcc.top

[U47] PHP：联合类型
来源：http://wva.snrcjt.cn

int|string $id
来源：http://pvc.zhixingplan.top

[U48] PHP：纯枚举
来源：http://tmf.andypj.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rwm.xziqi.cn

[U49] PHP：只读属性
来源：http://kqn.jlsjyb.cn

public readonly string $name
来源：http://pmv.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://ufz.snrcjt.cn

public function __construct(private int $id) {}
来源：http://zsj.zhoulong.xyz

[U51] PHP：数组解构
来源：http://deh.hnxiangtu.top

[$a, $b] = $arr;
来源：http://vvc.hongshengwenyu.top

[U52] PHP：箭头函数
来源：http://tnd.cashguo.top

$double = fn($x) => $x * 2;
来源：http://ljd.hfpthk.cn

[U53] PHP：空合并运算符
来源：http://kfe.ydjk.org.cn

$v = $a ?? $b ?? "default";
来源：http://ojz.chenzaomai.com

[U54] PHP：空安全调用
来源：http://tqj.yueranfly.top

$obj?->method()
来源：http://zhe.yj20258.top

[U55] PHP：match 表达式
来源：http://mvc.redwolf501.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pgt.tanke756.top

[U56] PHP：命名参数
来源：http://hmt.xziqi.cn

f(a: 1, b: 2)
来源：http://eqo.aizwys.cn

[U57] PHP：字符串插值
来源：http://dfe.dianchejie.cn

"值: {$a}"
来源：http://xwh.sufxvd.cn

[U58] PHP：数组三件套
来源：http://hdr.ctjpmb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qpp.yonumen.top

[U59] PHP：自定义排序
来源：http://yqd.kuanghao11.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iom.jinqigfzy.top

[U60] PHP：JSON 编解码
来源：http://vzi.zhaomingkeji.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cqp.316326.xyz

[U61] PHP：正则
来源：http://ecf.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nfe.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://ezq.ywan-chungtsiang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gql.shangyingyoupin.top

[U63] PHP：文件读写
来源：http://mzz.gotoacloud.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wvu.daxiang520.top

[U64] PHP：目录遍历
来源：http://npa.fzhhl.top

glob("dir/*.php");  scandir("dir");
来源：http://coj.snrcjt.cn

[U65] PHP：会话
来源：http://ftm.yueranfly.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gsq.zhaomingkeji.xyz

[U66] PHP：设置 Cookie
来源：http://drt.chenlongwang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ibx.hysaishi.cn

[U67] PHP：处理文件上传
来源：http://mas.c1oappe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sel.c1oappe.top

[U68] PHP：PDO 连接
来源：http://qfs.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ljs.shuidangran.top

[U69] PHP：PDO 预处理
来源：http://nki.wangdashe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hle.hcnkem.com

[U70] PHP：PDO 事务
来源：http://sbr.jlsjyb.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bey.shzxlz.cn

[U71] PHP：抛出异常
来源：http://zhd.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://tnq.cdnleiting.top

[U72] PHP：写错误日志
来源：http://eiq.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://pds.jyoumei.cn

[U73] PHP：读取 ini 配置
来源：http://noe.xuetiantiany.cn

parse_ini_file("config.ini", true)
来源：http://gbf.yonumen.top

[U74] PHP：读取环境变量
来源：http://rpf.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://pzy.yanxiufei.cn

[U75] PHP：依赖注入
来源：http://dsj.zhiwuduotai.top

composer require psr/container
来源：http://zde.xuetiantiany.cn

[U76] PHP：简单路由
来源：http://mon.birdmap.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jlo.dashuyun.cn

[U77] PHP：模板渲染
来源：http://pow.ywan-chungtsiang.top

composer require twig/twig
来源：http://wfg.gaohongyu789.top

[U78] PHP：单元测试
来源：http://vib.zhengqikj.top

composer require --dev phpunit/phpunit
来源：http://rvj.nanxuanxn.top

[U79] PHP：静态分析
来源：http://ahe.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://esq.fanxiaobao.xyz

[U80] PHP：代码规范修复
来源：http://lqk.c1oappe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mmq.quarkkingdee.top

[U81] JS：初始化项目
来源：http://qiv.sufxvd.cn

npm init -y;  npm i express
来源：http://nqg.shangyingyoupin.top

[U82] JS：package.json 脚本
来源：http://zed.sjlbkw.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gul.guowangkeji.top

[U83] JS：ES Module 导入导出
来源：http://srj.jinqigfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://pjo.wangdashe.top

[U84] JS：CommonJS 写法
来源：http://gll.bjfxy.top

module.exports = { a };  const { a } = require("./m");
来源：http://ios.smart0.xyz

[U85] JS：可选链
来源：http://gtn.haohaochexian.top

a?.b?.c
来源：http://yzy.yuanzhike.top

[U86] JS：空值合并
来源：http://qdg.bjfxy.top

a ?? b
来源：http://wzc.aibaodan.cn

[U87] JS：解构默认值
来源：http://jjs.xuanzx.com

const { a = 1, b = 2 } = obj;
来源：http://kqv.9152youxi.cn

[U88] JS：对象展开合并
来源：http://kzn.dashuyun.cn

{ ...a, ...b }
来源：http://lyj.vqdsnc.cn

[U89] JS：数组去重
来源：http://ojb.nanxuanxn.top

[...new Set(arr)]
来源：http://rel.hnqzz.top

[U90] JS：数字数组排序
来源：http://onq.birdmap.top

[...arr].sort((a, b) => a - b)
来源：http://yah.jianghu66.top

[U91] JS：对象键值遍历
来源：http://wll.nwbrower.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://thm.xylfe.cn

[U92] JS：深拷贝
来源：http://zix.shzxlz.cn

structuredClone(obj)
来源：http://msm.fzhhl.top

[U93] JS：模板字符串
来源：http://gsm.hammf.cn

`共 ${n} 条`
来源：http://rop.jinqigufen.top

[U94] JS：箭头函数
来源：http://fns.tarul.cn

const double = x => x * 2;
来源：http://vok.ivvv.top

[U95] JS：Promise 包装
来源：http://kjv.yuanzhike.top

new Promise((resolve, reject) => {})
来源：http://jae.yonumen.top

[U96] JS：async/await 与异常
来源：http://mmz.aibaodan.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ilx.cashguo.top

[U97] JS：并发请求
来源：http://kto.guannengcc.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nyj.zhixingplan.top

[U98] JS：fetch 带 JSON
来源：http://bzy.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yvf.yvedp.cn

[U99] JS：事件监听
来源：http://jqz.ydzc1.top

el.addEventListener("click", e => {})
来源：http://uyq.ehwqpu.com

[U100] JS：DOM 查询
来源：http://gid.nanxuanxn.top

document.querySelector(".item")
来源：http://hab.uphjek.com

[U101] JS：classList 操作
来源：http://qep.shangyingyoupin.top

el.classList.toggle("active")
来源：http://kqy.316326.xyz

[U102] JS：本地存储
来源：http://tnl.tian-w.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://iur.yanxiufei.cn

[U103] JS：定时器
来源：http://zck.zhixingplan.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://srk.sjlbkw.cn

[U104] JS：防抖
来源：http://idr.meibo888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rpe.cucudq.cn

[U105] JS：节流
来源：http://udt.jyoumei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mdv.xylfe.cn

[U106] JS：日期格式化
来源：http://jkm.sxryk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cod.bbcook.cn

[U107] JS：数字千分位
来源：http://hmr.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mhb.andypj.xyz

[U108] JS：随机整数
来源：http://dix.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yjb.mhx1999.top

[U109] JS：数组分组
来源：http://uvj.jqgfzy.top

Object.groupBy(arr, x => x.type)
来源：http://tjk.gaohongyu789.top

[U110] JS：数组分块
来源：http://lhl.tarul.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zpi.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://zfp.hnxiangtu.top

new Map(Object.entries(obj))
来源：http://ykz.9152youxi.cn

[U112] JS：字符串补位
来源：http://rrm.zhongyouzk.top

"7".padStart(3, "0")
来源：http://khb.nanxinkj.top

[U113] JS：正则替换全部
来源：http://ihc.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://voq.hongshengwenyu.top

[U114] JS：JSON 深比较
来源：http://lif.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://afk.wangshuangyany.cn

[U115] JS：生成 UUID
来源：http://owk.xuetiantiany.cn

crypto.randomUUID()
来源：http://mej.tianlin.xyz

[U116] JS：类型检查（JSDoc）
来源：http://xmb.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://qmq.yangfankeji.com

[U117] JS：单元测试
来源：http://ihj.nwbrower.top

npm i -D vitest;  npx vitest
来源：http://zqh.ppjwa.cn

[U118] JS：开发服务器
来源：http://hok.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://pca.hfpthk.cn

[U119] JS：生产构建
来源：http://ich.pengpengdd.cyou

npx vite build
来源：http://thj.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://xas.pycfn.com

import.meta.env.VITE_API_URL
来源：http://vha.yj20258888.top

================================================================================
来源：http://dqz.guannengcc.top

统计汇总
来源：http://fjp.ppjwa.cn

================================================================================
来源：http://xtt.ydzc1.top

按语言统计（条）：
来源：http://cor.chenlongwang.top

Python ......... 252
来源：http://pew.jianghu66.top

PHP ............ 252
来源：http://rih.jinqigufen.top

JavaScript ..... 252
来源：http://zkq.tianlin.xyz

TypeScript ..... 212
来源：http://ndg.c1oappe.top

Java ........... 212
来源：http://kqd.hcnkem.com

Go ............. 212
来源：http://zpv.zdbjq.cn

Ruby ........... 212
来源：http://xko.hysaishi.cn

C# ............. 212
来源：http://kev.fanxiaobao.xyz

C .............. 30
来源：http://tpy.guannengcc.top

C++ ............ 30
来源：http://eni.hnqzz.top

SQL ............ 90
来源：http://zto.52xcode.cn

Bash ........... 80
来源：http://wql.sweek.top

Kotlin ......... 15
来源：http://dkc.vqdsnc.cn

Swift .......... 15
来源：http://rox.tian-w.cn

Lua ............ 10
来源：http://zgo.cdnleiting.top

Perl ........... 10
来源：http://sdk.yangfankeji.com

Scala .......... 10
来源：http://cwb.yj202588.top

------------------------------------
来源：http://bkl.cdnleiting.top

合计 ........... 2106 条
来源：http://yiu.zhiwuduotai.top

按章节统计：
来源：http://uet.xylfe.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hsx.zhongyouzk.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://emm.tarul.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rpo.zhongyouzk.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://psy.dianchejie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vks.jiagoushi.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zqc.xylfe.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sge.snrcjt.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://txx.wangdashe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nrd.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fcb.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lsg.mhx1999.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gct.bbcook.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gwr.jiagoushi.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://krb.nwbrower.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ipo.yfazqb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jno.uphjek.com

Q SQL 专题                              90
来源：http://lkh.zdqjudy.top

R Bash 专题                             80
来源：http://uuq.shanyushiyangtech.top

S C / C++ 专题                          60
来源：http://ghd.andypj.xyz

T 其他语言补充                          60
来源：http://rtx.pengpengdd.cyou

U 高频实用片段                         120
来源：http://myc.ehwqpu.com

------------------------------------
来源：http://xfz.hammf.cn

合计                                  2106 条
来源：http://aql.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://wep.birdmap.top

使用提醒
来源：http://frq.pycfn.com

--------------------------------------------------------------------------------
来源：http://nzn.aizwys.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kye.feifeiyinyue.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ytv.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tuy.kuanghao11.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rxe.gogol.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bvj.yonumen.top

—— 文件结束 ——
来源：http://thp.hnqzz.top

================================================================================
来源：http://gwa.hesvh.cn

程序语言常见例子速查手册（2024 版）
来源：http://qje.yanxiufei.cn

Common Programming Examples Cheat Book
来源：http://pjo.jinqigufen.top

================================================================================
来源：http://xmx.yfazqb.com

【收录内容】
来源：http://jbp.iojbl.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wpu.bbcook.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hki.snrcjt.cn

SQL · Bash · C · C++
来源：http://ggn.gotoacloud.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zuu.c1oappe.top

【使用说明】
来源：http://dlt.tarul.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rmv.wangdashe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://diu.wangdashe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yrb.zdqjudy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://upu.pycfn.com

Bash:  Shell         C:     C             C++:   C++
来源：http://hch.yj202588.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dzz.zhixingplan.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rpz.shuidangran.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kyx.sjlbkw.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bkw.52xcode.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qcm.zhoulong.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://day.jqgfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wuq.iojbl.cn

【文件统计】
来源：http://qjp.tarul.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jlt.yvedp.cn

--------------------------------------------------------------------------------
来源：http://thy.vqdsnc.cn

目  录
来源：http://jlx.bbcook.cn

--------------------------------------------------------------------------------
来源：http://lfl.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mnq.shzxlz.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xbm.xinyue.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hlw.hongshengwenyu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dbk.wangshuangyany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jmm.xziqi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rks.fanxiaobao.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rjq.dianchejie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dcs.ydjk.org.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zem.jinghuilouyu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wkr.mhx1999.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xtw.xuanzx.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jat.shanyushiyangtech.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kjj.zhaomingkeji.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zeo.tianlin.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jdp.kuanghao11.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bpq.jinyuanbaomall.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bvh.yonumen.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ucp.yongpay.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ert.jianghu66.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wpo.chenlongwang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uwj.jqgfzy.top


<!-- 参考信息 -->