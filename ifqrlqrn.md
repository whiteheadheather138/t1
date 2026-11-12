代发 wailian999

[U25] Py：CSV 按字典读
来源：http://ycq.yonumen.top

csv.DictReader(f)
来源：http://zew.cucudq.cn

[U26] Py：并发下载
来源：http://lvv.tian-w.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bmm.gaohongyu789.top

[U27] Py：异步 HTTP
来源：http://pxp.fehbvm.com

aiohttp.ClientSession() 配合 async with
来源：http://fko.chenzaomai.com

[U28] Py：类型别名
来源：http://kzi.shuidangran.top

UserId = int
来源：http://xva.yongpay.top

[U29] Py：属性校验
来源：http://gqo.gzhubu.top

@property 与 @x.setter 配合
来源：http://bbg.hfpthk.cn

[U30] Py：数据类
来源：http://xcg.jqgfzy.top

@dataclass(slots=True)
来源：http://vui.zhaomingkeji.xyz

[U31] Py：单测
来源：http://lvu.jlsjyb.cn

python -m pytest -q
来源：http://whf.quarkkingdee.top

[U32] Py：代码格式化
来源：http://rxj.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://fnj.xinyue.icu

[U33] Py：打包发布
来源：http://nvs.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://tow.c1oappe.top

[U34] Py：判断编码
来源：http://cpr.andypj.xyz

chardet.detect(raw)
来源：http://bjf.aizwys.cn

[U35] Py：发送邮件
来源：http://dks.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nid.zdqjudy.top

[U36] Py：定时任务
来源：http://ugq.haohaochexian.top

schedule.every(10).minutes.do(job)
来源：http://ida.yonumen.top

[U37] Py：读写 Excel
来源：http://yuv.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://bbh.nanxinkj.top

[U38] Py：获取脚本所在目录
来源：http://ebf.redwolf501.top

Path(__file__).resolve().parent
来源：http://che.nwbrower.top

[U39] Py：判断是否在交互环境
来源：http://piy.sufxvd.cn

sys.stdout.isatty()
来源：http://wvy.xingfuxueyuan.xyz

[U40] Py：打印到标准错误
来源：http://zxz.hesvh.cn

print("err", file=sys.stderr)
来源：http://ytn.wangdashe.top

[U41] PHP：初始化 Composer 项目
来源：http://llw.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://dhh.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://qjj.zhoulong.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bsv.gzhubu.top

[U43] PHP：声明命名空间
来源：http://ukb.zhiwuduotai.top

namespace App\Http;
来源：http://prn.gogol.net.cn

[U44] PHP：开启严格类型
来源：http://jpi.shzxlz.cn

declare(strict_types=1);
来源：http://zxw.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://sbh.sweek.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://dqf.daxiang520.top

[U46] PHP：可空类型
来源：http://twt.fanxiaobao.xyz

?string $name = null
来源：http://olx.tian-w.cn

[U47] PHP：联合类型
来源：http://nmt.guannengcc.top

int|string $id
来源：http://olb.9152youxi.cn

[U48] PHP：纯枚举
来源：http://ohw.guannengcc.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uvi.dashuyun.cn

[U49] PHP：只读属性
来源：http://bdi.sufxvd.cn

public readonly string $name
来源：http://peh.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://dxt.c1oappe.top

public function __construct(private int $id) {}
来源：http://enq.tanke756.top

[U51] PHP：数组解构
来源：http://ddj.tarul.cn

[$a, $b] = $arr;
来源：http://ypv.cheryme.top

[U52] PHP：箭头函数
来源：http://kzg.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://etu.vehdjk.com

[U53] PHP：空合并运算符
来源：http://tct.yvedp.cn

$v = $a ?? $b ?? "default";
来源：http://vep.shanyushiyangtech.top

[U54] PHP：空安全调用
来源：http://kjg.ydjk.org.cn

$obj?->method()
来源：http://ysv.jinqigufen.top

[U55] PHP：match 表达式
来源：http://xjc.shangyingyoupin.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://epw.tian-w.cn

[U56] PHP：命名参数
来源：http://nxb.zdqjudy.top

f(a: 1, b: 2)
来源：http://noa.ehwqpu.com

[U57] PHP：字符串插值
来源：http://ppn.52xcode.cn

"值: {$a}"
来源：http://pfq.gogol.net.cn

[U58] PHP：数组三件套
来源：http://yzq.meibo888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rym.52xcode.cn

[U59] PHP：自定义排序
来源：http://qla.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pia.jinqigfzy.top

[U60] PHP：JSON 编解码
来源：http://dcc.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eij.jiagoushi.top

[U61] PHP：正则
来源：http://wsy.c1oappe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sco.9152youxi.cn

[U62] PHP：日期对象
来源：http://ncm.yj202588.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yxu.dianchejie.cn

[U63] PHP：文件读写
来源：http://kij.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gfp.yj20258.top

[U64] PHP：目录遍历
来源：http://cta.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://ywv.hammf.cn

[U65] PHP：会话
来源：http://ukr.fengsongda.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bfi.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://fjg.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hjd.ydzc1.top

[U67] PHP：处理文件上传
来源：http://cov.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eyp.ivvv.top

[U68] PHP：PDO 连接
来源：http://tid.daria6918.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rfz.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://fkz.sxryk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qxk.sufxvd.cn

[U70] PHP：PDO 事务
来源：http://adu.yueranfly.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wdf.zycfv.cn

[U71] PHP：抛出异常
来源：http://zpr.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://gmm.jinghuilouyu.cn

[U72] PHP：写错误日志
来源：http://syl.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://lil.bbcook.cn

[U73] PHP：读取 ini 配置
来源：http://wcn.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://rwn.daria6918.cn

[U74] PHP：读取环境变量
来源：http://ghv.cucudq.cn

getenv("APP_ENV") ?: "production"
来源：http://vdu.meibo888.top

[U75] PHP：依赖注入
来源：http://esn.chenzaomai.com

composer require psr/container
来源：http://lwl.mhx1999.top

[U76] PHP：简单路由
来源：http://fhp.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tcj.hnxiangtu.top

[U77] PHP：模板渲染
来源：http://nyp.tarul.cn

composer require twig/twig
来源：http://mjf.yvedp.cn

[U78] PHP：单元测试
来源：http://hqj.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://rkc.ydjk.org.cn

[U79] PHP：静态分析
来源：http://ztc.zdbjq.cn

composer require --dev phpstan/phpstan
来源：http://rex.yuxming.cn

[U80] PHP：代码规范修复
来源：http://yvm.hfpthk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xtu.c1oappe.top

[U81] JS：初始化项目
来源：http://xug.xuetiantiany.cn

npm init -y;  npm i express
来源：http://eyx.nwbrower.top

[U82] JS：package.json 脚本
来源：http://twd.zhengqikj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yix.mhx1999.top

[U83] JS：ES Module 导入导出
来源：http://afn.xziqi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pes.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://eue.jinqigfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://avp.quarkkingdee.top

[U85] JS：可选链
来源：http://tqf.jqgufenzy.top

a?.b?.c
来源：http://eoo.hesvh.cn

[U86] JS：空值合并
来源：http://wlh.gogol.net.cn

a ?? b
来源：http://fnk.guowangkeji.top

[U87] JS：解构默认值
来源：http://fgf.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://nnf.ctjpmb.com

[U88] JS：对象展开合并
来源：http://syd.yj20258.top

{ ...a, ...b }
来源：http://cok.zhijiandao.cn

[U89] JS：数组去重
来源：http://soc.mhx1999.top

[...new Set(arr)]
来源：http://vpr.ydjk.org.cn

[U90] JS：数字数组排序
来源：http://qud.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://ear.shangyingyoupin.top

[U91] JS：对象键值遍历
来源：http://wvh.jinqigufen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dbh.wangshuangyany.cn

[U92] JS：深拷贝
来源：http://uzl.tian-w.cn

structuredClone(obj)
来源：http://ujb.snrcjt.cn

[U93] JS：模板字符串
来源：http://pir.ybcxt.top

`共 ${n} 条`
来源：http://nsh.yanxiufei.cn

[U94] JS：箭头函数
来源：http://nlu.pengpengdd.cyou

const double = x => x * 2;
来源：http://nuo.birdmap.top

[U95] JS：Promise 包装
来源：http://yli.uphjek.com

new Promise((resolve, reject) => {})
来源：http://qur.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://rlt.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iho.yonumen.top

[U97] JS：并发请求
来源：http://vtp.jqgfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ifi.ctjpmb.com

[U98] JS：fetch 带 JSON
来源：http://obd.dianchejie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pyn.hnxiangtu.top

[U99] JS：事件监听
来源：http://ryb.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://byd.quarkkingdee.top

[U100] JS：DOM 查询
来源：http://ghn.tanke756.top

document.querySelector(".item")
来源：http://gcb.chenzaomai.com

[U101] JS：classList 操作
来源：http://fnd.vehdjk.com

el.classList.toggle("active")
来源：http://qkl.yfazqb.com

[U102] JS：本地存储
来源：http://lom.uphjek.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://tob.chenzaomai.com

[U103] JS：定时器
来源：http://prp.aizwys.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://obb.wangshuangyany.cn

[U104] JS：防抖
来源：http://npt.52xcode.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lvu.aibaodan.cn

[U105] JS：节流
来源：http://kii.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dia.snrcjt.cn

[U106] JS：日期格式化
来源：http://qyh.zhongyouzk.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ydw.yj202588.top

[U107] JS：数字千分位
来源：http://rcy.gogol.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oju.tian-w.cn

[U108] JS：随机整数
来源：http://zcy.tarul.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qqr.fanxiaobao.xyz

[U109] JS：数组分组
来源：http://cag.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://rch.hammf.cn

[U110] JS：数组分块
来源：http://kns.bbcook.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gdl.yueranfly.top

[U111] JS：对象转 Map
来源：http://fjt.daria6918.cn

new Map(Object.entries(obj))
来源：http://aei.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://ydf.shanyushiyangkeji.top

"7".padStart(3, "0")
来源：http://szb.sxryk.cn

[U113] JS：正则替换全部
来源：http://kyw.gogol.net.cn

s.replaceAll("a", "b")
来源：http://zqv.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://xeu.chenlongwang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://inx.yueranfly.top

[U115] JS：生成 UUID
来源：http://yju.xziqi.cn

crypto.randomUUID()
来源：http://mue.epnwcf.com

[U116] JS：类型检查（JSDoc）
来源：http://kix.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://cnm.ywan-chungtsiang.top

[U117] JS：单元测试
来源：http://zxt.cdnleiting.top

npm i -D vitest;  npx vitest
来源：http://qhz.chenzaomai.com

[U118] JS：开发服务器
来源：http://nca.yuanzhike.top

npm i -D vite;  npx vite
来源：http://xlt.mhx1999.top

[U119] JS：生产构建
来源：http://puc.chenzaomai.com

npx vite build
来源：http://ajb.yueranfly.top

[U120] JS：读取环境变量（Vite）
来源：http://via.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://exr.xinyue.icu

================================================================================
来源：http://wgo.zhengqikj.top

统计汇总
来源：http://log.feifeiyinyue.top

================================================================================
来源：http://cku.shanyushiyangtech.top

按语言统计（条）：
来源：http://qkp.xziqi.cn

Python ......... 252
来源：http://xch.zhaomingkeji.xyz

PHP ............ 252
来源：http://jpk.dianchejie.cn

JavaScript ..... 252
来源：http://hba.ydzc1.top

TypeScript ..... 212
来源：http://rjl.ivvv.top

Java ........... 212
来源：http://pqu.tian-w.cn

Go ............. 212
来源：http://gyc.iojbl.cn

Ruby ........... 212
来源：http://icd.hnxiangtu.top

C# ............. 212
来源：http://fab.ywan-chungtsiang.top

C .............. 30
来源：http://uwz.zhengqikj.top

C++ ............ 30
来源：http://qym.kuanghao11.cn

SQL ............ 90
来源：http://jpf.hysaishi.cn

Bash ........... 80
来源：http://bog.zhijiandao.cn

Kotlin ......... 15
来源：http://qmm.316326.xyz

Swift .......... 15
来源：http://ufr.cqqwz.cn

Lua ............ 10
来源：http://pzu.jqgfzy.top

Perl ........... 10
来源：http://oei.chenlongwang.top

Scala .......... 10
来源：http://hap.cheryme.top

------------------------------------
来源：http://iku.wangshuangyany.cn

合计 ........... 2106 条
来源：http://flq.ydjk.org.cn

按章节统计：
来源：http://sgv.yueranfly.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://joh.nanxuanxn.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hmh.gogol.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xze.0kj1m.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xjl.tarul.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ffa.uphjek.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vij.gotoacloud.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wcl.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bmp.shangyingyoupin.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pqk.c1oappe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jgz.xinyue.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vtn.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://roz.zhengqikj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mqy.sjlbkw.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kif.zhoulong.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ylz.chenjidiqi.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ipk.nanxuanxn.top

Q SQL 专题                              90
来源：http://hni.yanxiufei.cn

R Bash 专题                             80
来源：http://jfd.birdmap.top

S C / C++ 专题                          60
来源：http://ieg.fengsongda.top

T 其他语言补充                          60
来源：http://hzn.cucudq.cn

U 高频实用片段                         120
来源：http://nfp.bjfxy.top

------------------------------------
来源：http://nat.jqgfzy.top

合计                                  2106 条
来源：http://xct.birdmap.top

--------------------------------------------------------------------------------
来源：http://kby.jinyuanbaomall.cn

使用提醒
来源：http://lvh.ivvv.top

--------------------------------------------------------------------------------
来源：http://jvn.shangyingyoupin.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qxb.yonumen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wvp.hnxiangtu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bpz.cqqwz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fno.shangyingyoupin.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wwk.xziqi.cn

—— 文件结束 ——
来源：http://aql.yfazqb.com

================================================================================
来源：http://oms.316326.xyz

程序语言常见例子速查手册（2024 版）
来源：http://nss.wangdashe.top

Common Programming Examples Cheat Book
来源：http://owq.yueranfly.top

================================================================================
来源：http://jur.guowangkeji.top

【收录内容】
来源：http://jzt.iojbl.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://iwk.shzxlz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fcz.yonumen.top

SQL · Bash · C · C++
来源：http://exv.ivvv.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dcy.shanyushiyangtech.top

【使用说明】
来源：http://mhb.nwbrower.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kbc.yj20258.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dha.zhoulong.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bst.hfpthk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://whi.gogol.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ugn.cucudq.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eoh.ivvv.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uxt.yangfankeji.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cub.gotoacloud.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cdc.iojbl.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xjn.sweek.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qep.tian-w.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fdt.cucudq.cn

【文件统计】
来源：http://ieq.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dsk.sxryk.cn

--------------------------------------------------------------------------------
来源：http://dtm.c1oappe.top

目  录
来源：http://eoi.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://kgb.iojbl.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://imn.zhaomingkeji.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gsk.ybcxt.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nki.daxiang520.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ffp.daxiang520.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xnj.yfazqb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://whg.haohaochexian.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tpg.hammf.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cda.ybcxt.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gpe.gogol.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ruh.zdbjq.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sft.fehbvm.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zyg.shanyushiyangtech.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pmt.sxryk.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dec.cashguo.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://csp.yongpay.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://paf.daxiang520.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zdu.redwolf501.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://glh.tanke756.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yok.yueranfly.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jic.zhixingplan.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hgn.nwbrower.top

================================================================================
来源：http://hne.sufxvd.cn

A. 基础语法与类型
来源：http://uqh.nanxuanxn.top

================================================================================
来源：http://iwv.dashuyun.cn

[A01] Hello World
来源：http://uar.zhaomingkeji.xyz


<!-- 参考信息 -->