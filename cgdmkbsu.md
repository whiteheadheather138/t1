代发 wailian999

[U25] Py：CSV 按字典读
来源：http://uxt.tanke756.top

csv.DictReader(f)
来源：http://kvr.guowangkeji.top

[U26] Py：并发下载
来源：http://ycq.nwbrower.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wvz.epnwcf.com

[U27] Py：异步 HTTP
来源：http://zqo.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://ckc.yonumen.top

[U28] Py：类型别名
来源：http://nnq.cucudq.cn

UserId = int
来源：http://acq.fengsongda.top

[U29] Py：属性校验
来源：http://zpt.mhx1999.top

@property 与 @x.setter 配合
来源：http://zcp.daria6918.cn

[U30] Py：数据类
来源：http://aal.hesvh.cn

@dataclass(slots=True)
来源：http://uqg.ppjwa.cn

[U31] Py：单测
来源：http://tsc.yuanzhike.top

python -m pytest -q
来源：http://ecr.ydjk.org.cn

[U32] Py：代码格式化
来源：http://wzt.xuanzx.com

ruff format . && ruff check --fix .
来源：http://mhx.ybcxt.top

[U33] Py：打包发布
来源：http://mqa.jiagoushi.top

python -m build  （依赖 pyproject.toml）
来源：http://atu.nanxuanxn.top

[U34] Py：判断编码
来源：http://cjf.redwolf501.top

chardet.detect(raw)
来源：http://wbs.jqgfzy.top

[U35] Py：发送邮件
来源：http://yol.xingfuxueyuan.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bwu.yongpay.top

[U36] Py：定时任务
来源：http://juk.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://skb.dashuyun.cn

[U37] Py：读写 Excel
来源：http://unw.jqgufenzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://cio.ywan-chungtsiang.top

[U38] Py：获取脚本所在目录
来源：http://kol.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://bdq.mhx1999.top

[U39] Py：判断是否在交互环境
来源：http://zhz.birdmap.top

sys.stdout.isatty()
来源：http://spi.jqgufenzy.top

[U40] Py：打印到标准错误
来源：http://tae.ydjk.org.cn

print("err", file=sys.stderr)
来源：http://eeo.tarul.cn

[U41] PHP：初始化 Composer 项目
来源：http://riv.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tjk.chenzaomai.com

[U42] PHP：PSR-4 自动加载
来源：http://hlb.yfazqb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lqs.aizwys.cn

[U43] PHP：声明命名空间
来源：http://xmr.aizwys.cn

namespace App\Http;
来源：http://wgo.smart0.xyz

[U44] PHP：开启严格类型
来源：http://vsf.shanyushiyangkeji.top

declare(strict_types=1);
来源：http://gjh.wangdashe.top

[U45] PHP：类型声明与返回类型
来源：http://lqo.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://bct.yanxiufei.cn

[U46] PHP：可空类型
来源：http://rqj.vehdjk.com

?string $name = null
来源：http://liu.ywan-chungtsiang.top

[U47] PHP：联合类型
来源：http://lcj.yangfankeji.com

int|string $id
来源：http://dyd.tanke756.top

[U48] PHP：纯枚举
来源：http://rmb.mhx1999.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zbo.zhoulong.xyz

[U49] PHP：只读属性
来源：http://fis.yonumen.top

public readonly string $name
来源：http://afs.tianlin.xyz

[U50] PHP：构造器属性提升
来源：http://tji.yonumen.top

public function __construct(private int $id) {}
来源：http://ury.nwbrower.top

[U51] PHP：数组解构
来源：http://oms.yanxiufei.cn

[$a, $b] = $arr;
来源：http://ent.yuanzhike.top

[U52] PHP：箭头函数
来源：http://jhe.sysykeji.top

$double = fn($x) => $x * 2;
来源：http://ams.smart0.xyz

[U53] PHP：空合并运算符
来源：http://omx.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://seb.gotoacloud.top

[U54] PHP：空安全调用
来源：http://mqd.chenjidiqi.icu

$obj?->method()
来源：http://yne.gzhubu.top

[U55] PHP：match 表达式
来源：http://qof.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bdo.cheryme.top

[U56] PHP：命名参数
来源：http://rue.daxiang520.top

f(a: 1, b: 2)
来源：http://lzq.ivvv.top

[U57] PHP：字符串插值
来源：http://nyw.tarul.cn

"值: {$a}"
来源：http://njw.shangyingyoupin.top

[U58] PHP：数组三件套
来源：http://kin.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eom.fehbvm.com

[U59] PHP：自定义排序
来源：http://sot.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eiu.fanxiaobao.xyz

[U60] PHP：JSON 编解码
来源：http://xwn.cucudq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zym.aizwys.cn

[U61] PHP：正则
来源：http://exg.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mrn.dashuyun.cn

[U62] PHP：日期对象
来源：http://hrt.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yzx.cqqwz.cn

[U63] PHP：文件读写
来源：http://isu.xinyue.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xgi.guowangkeji.top

[U64] PHP：目录遍历
来源：http://wmf.redwolf501.top

glob("dir/*.php");  scandir("dir");
来源：http://htb.hcnkem.com

[U65] PHP：会话
来源：http://vyg.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lcw.xingfuxueyuan.xyz

[U66] PHP：设置 Cookie
来源：http://rjg.jiagoushi.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hsp.mhx1999.top

[U67] PHP：处理文件上传
来源：http://jla.ctjpmb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oln.ctjpmb.com

[U68] PHP：PDO 连接
来源：http://avn.xuanzx.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gtk.fehbvm.com

[U69] PHP：PDO 预处理
来源：http://uad.mhx1999.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cpb.svipenyu.cn

[U70] PHP：PDO 事务
来源：http://npe.fktsv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bfs.quarkkingdee.top

[U71] PHP：抛出异常
来源：http://byv.zhengqikj.top

throw new RuntimeException("失败", 500);
来源：http://kqn.zhengqikj.top

[U72] PHP：写错误日志
来源：http://jqi.zhoulong.xyz

error_log("失败: " . $e->getMessage());
来源：http://luh.jinqigufen.top

[U73] PHP：读取 ini 配置
来源：http://qxc.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://iet.hcnkem.com

[U74] PHP：读取环境变量
来源：http://fym.sweek.top

getenv("APP_ENV") ?: "production"
来源：http://vqv.shangyingyoupin.top

[U75] PHP：依赖注入
来源：http://wmo.jinqigufen.top

composer require psr/container
来源：http://kuh.sufxvd.cn

[U76] PHP：简单路由
来源：http://ldl.yueranfly.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ltm.0kj1m.cn

[U77] PHP：模板渲染
来源：http://rif.xingfuxueyuan.xyz

composer require twig/twig
来源：http://zoa.shanyushiyangtech.top

[U78] PHP：单元测试
来源：http://zep.fanxiaobao.xyz

composer require --dev phpunit/phpunit
来源：http://yli.kuanghao11.cn

[U79] PHP：静态分析
来源：http://aej.gzhubu.top

composer require --dev phpstan/phpstan
来源：http://vay.yj20258888.top

[U80] PHP：代码规范修复
来源：http://win.ehwqpu.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://dai.fzhhl.top

[U81] JS：初始化项目
来源：http://emk.aibaodan.cn

npm init -y;  npm i express
来源：http://xpy.hnqzz.top

[U82] JS：package.json 脚本
来源：http://wwc.aizwys.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cyo.snrcjt.cn

[U83] JS：ES Module 导入导出
来源：http://ado.zhijiandao.cn

export const a = 1;  import { a } from "./m.js";
来源：http://von.xylfe.cn

[U84] JS：CommonJS 写法
来源：http://qfl.xinyue.icu

module.exports = { a };  const { a } = require("./m");
来源：http://cne.ppjwa.cn

[U85] JS：可选链
来源：http://rkz.yonumen.top

a?.b?.c
来源：http://uon.yfazqb.com

[U86] JS：空值合并
来源：http://gbu.ehwqpu.com

a ?? b
来源：http://kaw.bbcook.cn

[U87] JS：解构默认值
来源：http://lya.nwbrower.top

const { a = 1, b = 2 } = obj;
来源：http://bhl.hfpthk.cn

[U88] JS：对象展开合并
来源：http://ahw.hnxiangtu.top

{ ...a, ...b }
来源：http://bza.chenlongwang.top

[U89] JS：数组去重
来源：http://kaw.zdbjq.cn

[...new Set(arr)]
来源：http://wyo.zhixingplan.top

[U90] JS：数字数组排序
来源：http://ukv.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://nmv.ybcxt.top

[U91] JS：对象键值遍历
来源：http://ilc.sjlbkw.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sgd.hywenlv.cn

[U92] JS：深拷贝
来源：http://ipd.zycfv.cn

structuredClone(obj)
来源：http://zio.xuanzx.com

[U93] JS：模板字符串
来源：http://erl.yuxming.cn

`共 ${n} 条`
来源：http://bul.xziqi.cn

[U94] JS：箭头函数
来源：http://njq.xziqi.cn

const double = x => x * 2;
来源：http://ivu.zhengqikj.top

[U95] JS：Promise 包装
来源：http://caz.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://vfh.yueranfly.top

[U96] JS：async/await 与异常
来源：http://ryw.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rxq.hysaishi.cn

[U97] JS：并发请求
来源：http://sdv.tarul.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dpc.yuanzhike.top

[U98] JS：fetch 带 JSON
来源：http://ikt.fzhhl.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lsq.zhongyouzk.top

[U99] JS：事件监听
来源：http://wue.cheryme.top

el.addEventListener("click", e => {})
来源：http://ycp.bbcook.cn

[U100] JS：DOM 查询
来源：http://czp.guannengcc.top

document.querySelector(".item")
来源：http://lgh.ybcxt.top

[U101] JS：classList 操作
来源：http://jon.c1oappe.top

el.classList.toggle("active")
来源：http://ezg.hysaishi.cn

[U102] JS：本地存储
来源：http://gwi.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://spw.uphjek.com

[U103] JS：定时器
来源：http://qan.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ogr.shanyushiyangtech.top

[U104] JS：防抖
来源：http://ckh.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mrl.pengpengdd.cyou

[U105] JS：节流
来源：http://dmm.yj202588.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://boa.nwbrower.top

[U106] JS：日期格式化
来源：http://mnx.fzhhl.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yck.ydjk.org.cn

[U107] JS：数字千分位
来源：http://vul.jyoumei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yye.pengpengdd.cyou

[U108] JS：随机整数
来源：http://jqy.ctjpmb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qcw.pycfn.com

[U109] JS：数组分组
来源：http://jvp.cheryme.top

Object.groupBy(arr, x => x.type)
来源：http://mbl.sysykeji.top

[U110] JS：数组分块
来源：http://fts.tianlin.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dkv.hysaishi.cn

[U111] JS：对象转 Map
来源：http://dpy.shanyushiyangkeji.top

new Map(Object.entries(obj))
来源：http://alz.smart0.xyz

[U112] JS：字符串补位
来源：http://xzd.yfazqb.com

"7".padStart(3, "0")
来源：http://nqi.yj20258888.top

[U113] JS：正则替换全部
来源：http://oqj.snrcjt.cn

s.replaceAll("a", "b")
来源：http://bzi.316326.xyz

[U114] JS：JSON 深比较
来源：http://rtb.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fbz.nwbrower.top

[U115] JS：生成 UUID
来源：http://zqs.cheryme.top

crypto.randomUUID()
来源：http://szw.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://kkl.zhoulong.xyz

/** @param {string} name */ function f(name) {}
来源：http://uct.hnqzz.top

[U117] JS：单元测试
来源：http://dbz.redwolf501.top

npm i -D vitest;  npx vitest
来源：http://ypq.daxiang520.top

[U118] JS：开发服务器
来源：http://zqv.shanyushiyangkeji.top

npm i -D vite;  npx vite
来源：http://nws.ctjpmb.com

[U119] JS：生产构建
来源：http://uwl.zdbjq.cn

npx vite build
来源：http://ere.shzxlz.cn

[U120] JS：读取环境变量（Vite）
来源：http://cxx.jianghu66.top

import.meta.env.VITE_API_URL
来源：http://xhp.nanxuanxn.top

================================================================================
来源：http://vjp.jqgufenzy.top

统计汇总
来源：http://vxv.jqgufenzy.top

================================================================================
来源：http://umn.ywan-chungtsiang.top

按语言统计（条）：
来源：http://uha.fzhhl.top

Python ......... 252
来源：http://jtb.cashguo.top

PHP ............ 252
来源：http://abt.svipenyu.cn

JavaScript ..... 252
来源：http://ewl.gotoacloud.top

TypeScript ..... 212
来源：http://yhp.quarkkingdee.top

Java ........... 212
来源：http://twb.yvedp.cn

Go ............. 212
来源：http://jku.jinghuilouyu.cn

Ruby ........... 212
来源：http://ute.ppjwa.cn

C# ............. 212
来源：http://zqa.daria6918.cn

C .............. 30
来源：http://vof.nanxinkj.top

C++ ............ 30
来源：http://mbp.yj20258.top

SQL ............ 90
来源：http://rnu.tanke756.top

Bash ........... 80
来源：http://rmd.chenzaomai.com

Kotlin ......... 15
来源：http://qpl.pengpengdd.cyou

Swift .......... 15
来源：http://cbv.yongpay.top

Lua ............ 10
来源：http://uxf.yj202588.top

Perl ........... 10
来源：http://wgg.cdnleiting.top

Scala .......... 10
来源：http://fko.wangshuangyany.cn

------------------------------------
来源：http://qfp.zdqjudy.top

合计 ........... 2106 条
来源：http://utp.andypj.xyz

按章节统计：
来源：http://eho.snrcjt.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xnm.aizwys.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dld.kuanghao11.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gvp.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rai.chenzaomai.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lnn.jinghuilouyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://urv.feifeiyinyue.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wpw.zhoulong.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cgf.jinyuanbaomall.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uyy.jinqigufen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nhw.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jzm.guowangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qsa.gogol.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tus.xingfuxueyuan.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yyr.zhixingplan.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wbw.jinqigfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nqa.epnwcf.com

Q SQL 专题                              90
来源：http://kug.smart0.xyz

R Bash 专题                             80
来源：http://ocn.aizwys.cn

S C / C++ 专题                          60
来源：http://bkl.snrcjt.cn

T 其他语言补充                          60
来源：http://njf.nwbrower.top

U 高频实用片段                         120
来源：http://otx.zhaomingkeji.xyz

------------------------------------
来源：http://ksr.hongshengwenyu.top

合计                                  2106 条
来源：http://wwr.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://rjr.fanxiaobao.xyz

使用提醒
来源：http://mov.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://gii.jqgfzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ajb.hnqzz.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lmm.feifeiyinyue.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ybu.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://sut.andypj.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oam.ehwqpu.com

—— 文件结束 ——
来源：http://zeu.guannengcc.top

================================================================================
来源：http://dta.hnqzz.top

程序语言常见例子速查手册（2024 版）
来源：http://hsh.yfazqb.com

Common Programming Examples Cheat Book
来源：http://amr.mhx1999.top

================================================================================
来源：http://iuh.pengpengdd.cyou

【收录内容】
来源：http://zmq.ctjpmb.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://huq.daxiang520.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://isq.hcnkem.com

SQL · Bash · C · C++
来源：http://djn.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nof.jinqigufen.top

【使用说明】
来源：http://ibj.wangdashe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dby.zhongyouzk.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tue.chenjidiqi.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rsl.xylfe.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rwn.meibo888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://pnk.yuxming.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gre.ivvv.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qoc.fehbvm.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gvs.ivvv.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pme.feifeiyinyue.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tci.yj202588.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hsn.tarul.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jhf.ywan-chungtsiang.top

【文件统计】
来源：http://jpj.ywan-chungtsiang.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ivj.ivvv.top

--------------------------------------------------------------------------------
来源：http://msq.shuidangran.top

目  录
来源：http://wfl.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://ahi.epnwcf.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ntv.zycfv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vjn.0kj1m.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gvh.hywenlv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://msp.kuanghao11.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lpw.uphjek.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yws.yj202588.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zgy.sjlbkw.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fng.daxiang520.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ulf.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ecp.uphjek.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zht.wangdashe.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qhj.fehbvm.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xmc.cdnleiting.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vtl.xingfuxueyuan.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wtj.ydjk.org.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mib.cdnleiting.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fnh.zhengqikj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wgu.0kj1m.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yfz.xingfuxueyuan.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jod.yuxming.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zzb.uphjek.com

================================================================================
来源：http://qwi.xinyue.icu

A. 基础语法与类型
来源：http://iui.0kj1m.cn

================================================================================
来源：http://fop.chenlongwang.top

[A01] Hello World
来源：http://pvz.ybcxt.top


<!-- 参考信息 -->