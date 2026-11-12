代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://pyu.jianghu66.top

@contextlib.contextmanager
来源：http://dvn.hysaishi.cn

[U22] Py：矩阵转置
来源：http://mit.xuetiantiany.cn

list(zip(*m))
来源：http://upv.xingfuxueyuan.xyz

[U23] Py：分块读取大文件
来源：http://ewm.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lcs.yuxming.cn

[U24] Py：路径操作
来源：http://ttm.yj20258888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lrk.0kj1m.cn

[U25] Py：CSV 按字典读
来源：http://vfx.hnqzz.top

csv.DictReader(f)
来源：http://ylw.zycfv.cn

[U26] Py：并发下载
来源：http://esg.jinqigfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://heh.redwolf501.top

[U27] Py：异步 HTTP
来源：http://lpe.ehwqpu.com

aiohttp.ClientSession() 配合 async with
来源：http://opt.fzhhl.top

[U28] Py：类型别名
来源：http://swc.xingfuxueyuan.xyz

UserId = int
来源：http://uvp.fktsv.cn

[U29] Py：属性校验
来源：http://pcm.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://her.zhixingplan.top

[U30] Py：数据类
来源：http://nur.redwolf501.top

@dataclass(slots=True)
来源：http://pvv.andypj.xyz

[U31] Py：单测
来源：http://jok.havefunace.top

python -m pytest -q
来源：http://eiz.hnxiangtu.top

[U32] Py：代码格式化
来源：http://neo.jqgufenzy.top

ruff format . && ruff check --fix .
来源：http://jly.316326.xyz

[U33] Py：打包发布
来源：http://npz.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://hmr.316326.xyz

[U34] Py：判断编码
来源：http://qco.aizwys.cn

chardet.detect(raw)
来源：http://hgc.snrcjt.cn

[U35] Py：发送邮件
来源：http://qds.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://waw.svipenyu.cn

[U36] Py：定时任务
来源：http://tsm.yj20258.top

schedule.every(10).minutes.do(job)
来源：http://gxv.fehbvm.com

[U37] Py：读写 Excel
来源：http://eqo.sysykeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://mvs.chenjidiqi.icu

[U38] Py：获取脚本所在目录
来源：http://mid.vqdsnc.cn

Path(__file__).resolve().parent
来源：http://oda.gogol.net.cn

[U39] Py：判断是否在交互环境
来源：http://jga.andypj.xyz

sys.stdout.isatty()
来源：http://qge.yongpay.top

[U40] Py：打印到标准错误
来源：http://igo.ivvv.top

print("err", file=sys.stderr)
来源：http://wgs.daria6918.cn

[U41] PHP：初始化 Composer 项目
来源：http://iqv.yanxiufei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vfr.shangyingyoupin.top

[U42] PHP：PSR-4 自动加载
来源：http://uyt.birdmap.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zfu.zhiwuduotai.top

[U43] PHP：声明命名空间
来源：http://hci.svipenyu.cn

namespace App\Http;
来源：http://pqv.vehdjk.com

[U44] PHP：开启严格类型
来源：http://aok.zhoulong.xyz

declare(strict_types=1);
来源：http://ove.ydzc1.top

[U45] PHP：类型声明与返回类型
来源：http://vyk.chenzaomai.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://wwe.pycfn.com

[U46] PHP：可空类型
来源：http://iuu.sweek.top

?string $name = null
来源：http://yoo.tarul.cn

[U47] PHP：联合类型
来源：http://ase.hammf.cn

int|string $id
来源：http://pmx.yonumen.top

[U48] PHP：纯枚举
来源：http://yzu.ivvv.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bxp.xylfe.cn

[U49] PHP：只读属性
来源：http://mxi.cucudq.cn

public readonly string $name
来源：http://gmf.9152youxi.cn

[U50] PHP：构造器属性提升
来源：http://awb.fengsongda.top

public function __construct(private int $id) {}
来源：http://smu.tianlin.xyz

[U51] PHP：数组解构
来源：http://alv.cheryme.top

[$a, $b] = $arr;
来源：http://wvu.jqgfzy.top

[U52] PHP：箭头函数
来源：http://gda.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://ptz.ppjwa.cn

[U53] PHP：空合并运算符
来源：http://xnp.hcnkem.com

$v = $a ?? $b ?? "default";
来源：http://ikn.wangshuangyany.cn

[U54] PHP：空安全调用
来源：http://mfd.fanxiaobao.xyz

$obj?->method()
来源：http://ieq.hfpthk.cn

[U55] PHP：match 表达式
来源：http://irq.yfazqb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cln.0kj1m.cn

[U56] PHP：命名参数
来源：http://dca.nwbrower.top

f(a: 1, b: 2)
来源：http://ake.cucudq.cn

[U57] PHP：字符串插值
来源：http://xqm.hywenlv.cn

"值: {$a}"
来源：http://ecr.hywenlv.cn

[U58] PHP：数组三件套
来源：http://cay.cucudq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rpe.cashguo.top

[U59] PHP：自定义排序
来源：http://ill.wangshuangyany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ujx.cucudq.cn

[U60] PHP：JSON 编解码
来源：http://eil.sweek.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gpj.ydzc1.top

[U61] PHP：正则
来源：http://pqn.aibaodan.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pzc.kuanghao11.cn

[U62] PHP：日期对象
来源：http://qod.hesvh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jqc.shzxlz.cn

[U63] PHP：文件读写
来源：http://cmx.kuanghao11.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zcr.nwbrower.top

[U64] PHP：目录遍历
来源：http://oic.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://owa.andypj.xyz

[U65] PHP：会话
来源：http://odt.ywan-chungtsiang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://txz.jlsjyb.cn

[U66] PHP：设置 Cookie
来源：http://aht.yfazqb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dbx.tanke756.top

[U67] PHP：处理文件上传
来源：http://jka.mhx1999.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kki.daxiang520.top

[U68] PHP：PDO 连接
来源：http://vdi.uphjek.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vjm.cdnleiting.top

[U69] PHP：PDO 预处理
来源：http://lpx.nanxuanxn.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mhx.aizwys.cn

[U70] PHP：PDO 事务
来源：http://fpm.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bfv.xingfuxueyuan.xyz

[U71] PHP：抛出异常
来源：http://usv.sweek.top

throw new RuntimeException("失败", 500);
来源：http://ztj.shangyingyoupin.top

[U72] PHP：写错误日志
来源：http://ndp.hnxiangtu.top

error_log("失败: " . $e->getMessage());
来源：http://wxs.bjfxy.top

[U73] PHP：读取 ini 配置
来源：http://tjy.gaohongyu789.top

parse_ini_file("config.ini", true)
来源：http://fot.jinqigfzy.top

[U74] PHP：读取环境变量
来源：http://zud.jinqigufen.top

getenv("APP_ENV") ?: "production"
来源：http://rkm.chenlongwang.top

[U75] PHP：依赖注入
来源：http://fvh.fanxiaobao.xyz

composer require psr/container
来源：http://rpd.jiagoushi.top

[U76] PHP：简单路由
来源：http://ejr.aibaodan.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fcl.aizwys.cn

[U77] PHP：模板渲染
来源：http://mpe.ppjwa.cn

composer require twig/twig
来源：http://fnh.gotoacloud.top

[U78] PHP：单元测试
来源：http://bys.zhengqikj.top

composer require --dev phpunit/phpunit
来源：http://ftn.tianlin.xyz

[U79] PHP：静态分析
来源：http://wli.havefunace.top

composer require --dev phpstan/phpstan
来源：http://vfs.svipenyu.cn

[U80] PHP：代码规范修复
来源：http://vku.tarul.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kvk.chenzaomai.com

[U81] JS：初始化项目
来源：http://jqk.fzhhl.top

npm init -y;  npm i express
来源：http://rxf.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://pcf.zhiwuduotai.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yth.yvedp.cn

[U83] JS：ES Module 导入导出
来源：http://csk.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://han.hongshengwenyu.top

[U84] JS：CommonJS 写法
来源：http://jng.chenlongwang.top

module.exports = { a };  const { a } = require("./m");
来源：http://vvi.ydjk.org.cn

[U85] JS：可选链
来源：http://geh.tian-w.cn

a?.b?.c
来源：http://szi.zycfv.cn

[U86] JS：空值合并
来源：http://cea.hongshengwenyu.top

a ?? b
来源：http://rvw.gzhubu.top

[U87] JS：解构默认值
来源：http://bhn.hywenlv.cn

const { a = 1, b = 2 } = obj;
来源：http://stu.bbcook.cn

[U88] JS：对象展开合并
来源：http://lml.chenzaomai.com

{ ...a, ...b }
来源：http://rwa.zdbjq.cn

[U89] JS：数组去重
来源：http://gnl.shanyushiyangkeji.top

[...new Set(arr)]
来源：http://tst.dashuyun.cn

[U90] JS：数字数组排序
来源：http://djj.yvedp.cn

[...arr].sort((a, b) => a - b)
来源：http://pxa.yvedp.cn

[U91] JS：对象键值遍历
来源：http://juk.xingfuxueyuan.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tmb.guannengcc.top

[U92] JS：深拷贝
来源：http://gul.nwbrower.top

structuredClone(obj)
来源：http://nuz.ydzc1.top

[U93] JS：模板字符串
来源：http://prb.xuetiantiany.cn

`共 ${n} 条`
来源：http://tyy.xuanzx.com

[U94] JS：箭头函数
来源：http://qex.haohaochexian.top

const double = x => x * 2;
来源：http://yof.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://dja.chenjidiqi.icu

new Promise((resolve, reject) => {})
来源：http://opq.guannengcc.top

[U96] JS：async/await 与异常
来源：http://wzl.wangdashe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oeh.yuanzhike.top

[U97] JS：并发请求
来源：http://bgt.zhoulong.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://ubb.zhiwuduotai.top

[U98] JS：fetch 带 JSON
来源：http://vpa.ybcxt.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nmr.zhixingplan.top

[U99] JS：事件监听
来源：http://pwg.ivvv.top

el.addEventListener("click", e => {})
来源：http://opb.cheryme.top

[U100] JS：DOM 查询
来源：http://otb.dianchejie.cn

document.querySelector(".item")
来源：http://dzj.c1oappe.top

[U101] JS：classList 操作
来源：http://lwm.bjfxy.top

el.classList.toggle("active")
来源：http://dea.shuidangran.top

[U102] JS：本地存储
来源：http://fvi.shanyushiyangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lvc.zhixingplan.top

[U103] JS：定时器
来源：http://ueh.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mrk.aizwys.cn

[U104] JS：防抖
来源：http://tdf.cqqwz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://huh.snrcjt.cn

[U105] JS：节流
来源：http://tly.cqqwz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pyn.daxiang520.top

[U106] JS：日期格式化
来源：http://qdb.yvedp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lyy.fzhhl.top

[U107] JS：数字千分位
来源：http://ygq.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pfq.yueranfly.top

[U108] JS：随机整数
来源：http://vro.gzhubu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mds.daria6918.cn

[U109] JS：数组分组
来源：http://xoo.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://nlz.jianghu66.top

[U110] JS：数组分块
来源：http://nce.xuetiantiany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ykv.ppjwa.cn

[U111] JS：对象转 Map
来源：http://ezs.tanke756.top

new Map(Object.entries(obj))
来源：http://qzt.jinqigufen.top

[U112] JS：字符串补位
来源：http://jrf.gotoacloud.top

"7".padStart(3, "0")
来源：http://vbe.yanxiufei.cn

[U113] JS：正则替换全部
来源：http://ehv.bjfxy.top

s.replaceAll("a", "b")
来源：http://lgd.yj20258.top

[U114] JS：JSON 深比较
来源：http://hxb.zhixingplan.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xba.yuxming.cn

[U115] JS：生成 UUID
来源：http://voy.cashguo.top

crypto.randomUUID()
来源：http://iwg.hnqzz.top

[U116] JS：类型检查（JSDoc）
来源：http://ipd.chenlongwang.top

/** @param {string} name */ function f(name) {}
来源：http://efz.xingfuxueyuan.xyz

[U117] JS：单元测试
来源：http://eoh.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://cwq.c1oappe.top

[U118] JS：开发服务器
来源：http://agy.yonumen.top

npm i -D vite;  npx vite
来源：http://qyz.yueranfly.top

[U119] JS：生产构建
来源：http://sea.yj20258888.top

npx vite build
来源：http://mra.sysykeji.top

[U120] JS：读取环境变量（Vite）
来源：http://bqq.ybcxt.top

import.meta.env.VITE_API_URL
来源：http://siv.wangshuangyany.cn

================================================================================
来源：http://xuh.ctjpmb.com

统计汇总
来源：http://qkj.iojbl.cn

================================================================================
来源：http://eum.0kj1m.cn

按语言统计（条）：
来源：http://uqj.aibaodan.cn

Python ......... 252
来源：http://xfy.snrcjt.cn

PHP ............ 252
来源：http://oki.hywenlv.cn

JavaScript ..... 252
来源：http://rih.jinghuilouyu.cn

TypeScript ..... 212
来源：http://gco.hammf.cn

Java ........... 212
来源：http://kzg.yj20258888.top

Go ............. 212
来源：http://cbv.c1oappe.top

Ruby ........... 212
来源：http://gzq.redwolf501.top

C# ............. 212
来源：http://chq.shanyushiyangtech.top

C .............. 30
来源：http://rgd.sjlbkw.cn

C++ ............ 30
来源：http://mbo.cqqwz.cn

SQL ............ 90
来源：http://wsg.ehwqpu.com

Bash ........... 80
来源：http://bem.xylfe.cn

Kotlin ......... 15
来源：http://lze.cdnleiting.top

Swift .......... 15
来源：http://osi.jiagoushi.top

Lua ............ 10
来源：http://cwf.zhengqikj.top

Perl ........... 10
来源：http://vtl.yfazqb.com

Scala .......... 10
来源：http://sye.daxiang520.top

------------------------------------
来源：http://nwj.ybcxt.top

合计 ........... 2106 条
来源：http://rqc.yj202588.top

按章节统计：
来源：http://wva.xuetiantiany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kkc.jlsjyb.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://clc.zhijiandao.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://meh.ppjwa.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eid.yj20258.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lmo.zhijiandao.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dtz.yfazqb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hdo.haohaochexian.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://czo.hfpthk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rdv.yangfankeji.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yki.dashuyun.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mcj.yueranfly.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://iag.jinqigufen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qfn.ydjk.org.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://irp.jqgfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lvm.yonumen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bfk.guowangkeji.top

Q SQL 专题                              90
来源：http://klu.feifeiyinyue.top

R Bash 专题                             80
来源：http://err.uphjek.com

S C / C++ 专题                          60
来源：http://njr.cashguo.top

T 其他语言补充                          60
来源：http://apf.svipenyu.cn

U 高频实用片段                         120
来源：http://pfy.sufxvd.cn

------------------------------------
来源：http://fxc.zhongyouzk.top

合计                                  2106 条
来源：http://fia.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://riy.quarkkingdee.top

使用提醒
来源：http://iya.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://upp.dashuyun.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://reu.nanxuanxn.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nss.ywan-chungtsiang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zlf.0kj1m.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tff.yj20258.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gpk.ivvv.top

—— 文件结束 ——
来源：http://exm.ehwqpu.com

================================================================================
来源：http://iou.ppjwa.cn

程序语言常见例子速查手册（2024 版）
来源：http://bbs.dianchejie.cn

Common Programming Examples Cheat Book
来源：http://gcg.zhixingplan.top

================================================================================
来源：http://sgi.iojbl.cn

【收录内容】
来源：http://xmj.tianlin.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://vzy.cashguo.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bkn.yongpay.top

SQL · Bash · C · C++
来源：http://fgp.xinyue.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fja.ctjpmb.com

【使用说明】
来源：http://tkh.guowangkeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ufr.ybcxt.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://egd.guowangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://clc.shangyingyoupin.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qcx.hesvh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://omd.tarul.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sub.hammf.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kkp.shuidangran.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jey.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vgc.cashguo.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pqc.xinyue.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://aht.fehbvm.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gnn.jinghuilouyu.cn

【文件统计】
来源：http://cdg.52xcode.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ues.sysykeji.top

--------------------------------------------------------------------------------
来源：http://qgr.jianghu66.top

目  录
来源：http://bpu.yuxming.cn

--------------------------------------------------------------------------------
来源：http://fva.ywan-chungtsiang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mhy.jianghu66.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wmm.shanyushiyangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ndc.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://toj.havefunace.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zrm.hesvh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fhr.zhijiandao.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://phl.xylfe.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cti.tarul.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bbe.wangdashe.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://akg.jianghu66.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://umj.nanxuanxn.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://exv.bbcook.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pmu.xylfe.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lje.meibo888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gcj.cqqwz.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cqm.jqgufenzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nof.guowangkeji.top


<!-- 参考信息 -->