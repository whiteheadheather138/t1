代发 wailian999

[U25] Py：CSV 按字典读
来源：http://dlr.yj20258888.top

csv.DictReader(f)
来源：http://kcp.316326.xyz

[U26] Py：并发下载
来源：http://bzn.fengsongda.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ivb.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://tug.hesvh.cn

aiohttp.ClientSession() 配合 async with
来源：http://slv.yangfankeji.com

[U28] Py：类型别名
来源：http://mgm.snrcjt.cn

UserId = int
来源：http://ife.ybcxt.top

[U29] Py：属性校验
来源：http://igq.tanke756.top

@property 与 @x.setter 配合
来源：http://dtn.hcnkem.com

[U30] Py：数据类
来源：http://csd.zycfv.cn

@dataclass(slots=True)
来源：http://nzj.sxryk.cn

[U31] Py：单测
来源：http://akp.dianchejie.cn

python -m pytest -q
来源：http://gci.yfazqb.com

[U32] Py：代码格式化
来源：http://pfx.ppjwa.cn

ruff format . && ruff check --fix .
来源：http://xxz.jlsjyb.cn

[U33] Py：打包发布
来源：http://ith.pengpengdd.cyou

python -m build  （依赖 pyproject.toml）
来源：http://mlz.tian-w.cn

[U34] Py：判断编码
来源：http://xwf.shuidangran.top

chardet.detect(raw)
来源：http://mck.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://ies.52xcode.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ijl.zhiwuduotai.top

[U36] Py：定时任务
来源：http://xyi.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://ljg.hnqzz.top

[U37] Py：读写 Excel
来源：http://rde.hfpthk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hds.xylfe.cn

[U38] Py：获取脚本所在目录
来源：http://elo.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://ecw.iojbl.cn

[U39] Py：判断是否在交互环境
来源：http://bio.fengsongda.top

sys.stdout.isatty()
来源：http://jjh.jqgfzy.top

[U40] Py：打印到标准错误
来源：http://doi.uphjek.com

print("err", file=sys.stderr)
来源：http://hcq.redwolf501.top

[U41] PHP：初始化 Composer 项目
来源：http://oyw.smart0.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://ald.hnqzz.top

[U42] PHP：PSR-4 自动加载
来源：http://nqt.xuanzx.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qmd.havefunace.top

[U43] PHP：声明命名空间
来源：http://qrl.mhx1999.top

namespace App\Http;
来源：http://fkm.birdmap.top

[U44] PHP：开启严格类型
来源：http://nbz.jinqigfzy.top

declare(strict_types=1);
来源：http://wjk.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://bsc.quarkkingdee.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vqi.xziqi.cn

[U46] PHP：可空类型
来源：http://rmd.hywenlv.cn

?string $name = null
来源：http://wja.jqgfzy.top

[U47] PHP：联合类型
来源：http://vnm.ehwqpu.com

int|string $id
来源：http://gjd.sjlbkw.cn

[U48] PHP：纯枚举
来源：http://top.cqqwz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yki.mhx1999.top

[U49] PHP：只读属性
来源：http://mie.gotoacloud.top

public readonly string $name
来源：http://xnz.tarul.cn

[U50] PHP：构造器属性提升
来源：http://zjz.xuanzx.com

public function __construct(private int $id) {}
来源：http://mjd.redwolf501.top

[U51] PHP：数组解构
来源：http://nba.yj20258888.top

[$a, $b] = $arr;
来源：http://sxy.chenlongwang.top

[U52] PHP：箭头函数
来源：http://rst.zycfv.cn

$double = fn($x) => $x * 2;
来源：http://jol.gzhubu.top

[U53] PHP：空合并运算符
来源：http://vyi.hongshengwenyu.top

$v = $a ?? $b ?? "default";
来源：http://hfp.vehdjk.com

[U54] PHP：空安全调用
来源：http://wlt.chenjidiqi.icu

$obj?->method()
来源：http://xuy.yuxming.cn

[U55] PHP：match 表达式
来源：http://cwj.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vue.jinqigfzy.top

[U56] PHP：命名参数
来源：http://mzv.yanxiufei.cn

f(a: 1, b: 2)
来源：http://xww.daxiang520.top

[U57] PHP：字符串插值
来源：http://naa.yj20258.top

"值: {$a}"
来源：http://ymg.sweek.top

[U58] PHP：数组三件套
来源：http://qxl.ydzc1.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uko.gzhubu.top

[U59] PHP：自定义排序
来源：http://udk.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://irz.zhongyouzk.top

[U60] PHP：JSON 编解码
来源：http://lty.hysaishi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qih.haohaochexian.top

[U61] PHP：正则
来源：http://qku.wangshuangyany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fdz.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://cir.sxryk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xlm.dianchejie.cn

[U63] PHP：文件读写
来源：http://rwl.feifeiyinyue.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qjo.nanxinkj.top

[U64] PHP：目录遍历
来源：http://gmw.feifeiyinyue.top

glob("dir/*.php");  scandir("dir");
来源：http://vop.ydjk.org.cn

[U65] PHP：会话
来源：http://hpt.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ppf.hongshengwenyu.top

[U66] PHP：设置 Cookie
来源：http://isn.yanxiufei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://njo.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://kpj.svipenyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wmn.sysykeji.top

[U68] PHP：PDO 连接
来源：http://zin.sysykeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ozj.epnwcf.com

[U69] PHP：PDO 预处理
来源：http://awp.aizwys.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://szo.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://dxh.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ciz.shangyingyoupin.top

[U71] PHP：抛出异常
来源：http://sun.yuxming.cn

throw new RuntimeException("失败", 500);
来源：http://ghz.pycfn.com

[U72] PHP：写错误日志
来源：http://scn.tanke756.top

error_log("失败: " . $e->getMessage());
来源：http://mns.shzxlz.cn

[U73] PHP：读取 ini 配置
来源：http://zic.daxiang520.top

parse_ini_file("config.ini", true)
来源：http://duo.hysaishi.cn

[U74] PHP：读取环境变量
来源：http://dxp.shangyingyoupin.top

getenv("APP_ENV") ?: "production"
来源：http://skb.gotoacloud.top

[U75] PHP：依赖注入
来源：http://nup.yongpay.top

composer require psr/container
来源：http://hxq.chenlongwang.top

[U76] PHP：简单路由
来源：http://qez.hnqzz.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pgy.yuxming.cn

[U77] PHP：模板渲染
来源：http://ezd.dashuyun.cn

composer require twig/twig
来源：http://chz.yonumen.top

[U78] PHP：单元测试
来源：http://vnj.redwolf501.top

composer require --dev phpunit/phpunit
来源：http://aee.hammf.cn

[U79] PHP：静态分析
来源：http://iew.guowangkeji.top

composer require --dev phpstan/phpstan
来源：http://ndu.ybcxt.top

[U80] PHP：代码规范修复
来源：http://xmx.hnxiangtu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qbt.andypj.xyz

[U81] JS：初始化项目
来源：http://hwk.zycfv.cn

npm init -y;  npm i express
来源：http://nux.yuanzhike.top

[U82] JS：package.json 脚本
来源：http://xwk.hnqzz.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gbf.ydjk.org.cn

[U83] JS：ES Module 导入导出
来源：http://imw.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://vpr.9152youxi.cn

[U84] JS：CommonJS 写法
来源：http://iak.jinghuilouyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uph.quarkkingdee.top

[U85] JS：可选链
来源：http://mjs.xinyue.icu

a?.b?.c
来源：http://vha.cdnleiting.top

[U86] JS：空值合并
来源：http://eop.yuxming.cn

a ?? b
来源：http://kqm.zhengqikj.top

[U87] JS：解构默认值
来源：http://zzo.yj202588.top

const { a = 1, b = 2 } = obj;
来源：http://sou.jyoumei.cn

[U88] JS：对象展开合并
来源：http://lsz.yongpay.top

{ ...a, ...b }
来源：http://kvy.guannengcc.top

[U89] JS：数组去重
来源：http://fgi.wangdashe.top

[...new Set(arr)]
来源：http://rvp.sysykeji.top

[U90] JS：数字数组排序
来源：http://mhc.chenzaomai.com

[...arr].sort((a, b) => a - b)
来源：http://ugp.yuxming.cn

[U91] JS：对象键值遍历
来源：http://eee.hongshengwenyu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hus.xuanzx.com

[U92] JS：深拷贝
来源：http://mmn.pengpengdd.cyou

structuredClone(obj)
来源：http://ueb.andypj.xyz

[U93] JS：模板字符串
来源：http://wbg.yanxiufei.cn

`共 ${n} 条`
来源：http://rhi.redwolf501.top

[U94] JS：箭头函数
来源：http://qmz.zhijiandao.cn

const double = x => x * 2;
来源：http://qng.jyoumei.cn

[U95] JS：Promise 包装
来源：http://bmc.tianlin.xyz

new Promise((resolve, reject) => {})
来源：http://zwo.jinqigufen.top

[U96] JS：async/await 与异常
来源：http://pxc.feifeiyinyue.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qwl.jqgfzy.top

[U97] JS：并发请求
来源：http://ilm.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://fko.hammf.cn

[U98] JS：fetch 带 JSON
来源：http://eoe.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pae.jinqigfzy.top

[U99] JS：事件监听
来源：http://yls.pengpengdd.cyou

el.addEventListener("click", e => {})
来源：http://qld.yj20258888.top

[U100] JS：DOM 查询
来源：http://hbo.jqgfzy.top

document.querySelector(".item")
来源：http://dtz.xinyue.icu

[U101] JS：classList 操作
来源：http://mpv.aizwys.cn

el.classList.toggle("active")
来源：http://fyx.jinqigfzy.top

[U102] JS：本地存储
来源：http://gvz.hcnkem.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://rob.shanyushiyangtech.top

[U103] JS：定时器
来源：http://vco.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xcq.xziqi.cn

[U104] JS：防抖
来源：http://qim.ybcxt.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mhm.zhoulong.xyz

[U105] JS：节流
来源：http://oue.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rdx.zycfv.cn

[U106] JS：日期格式化
来源：http://nkv.feifeiyinyue.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://map.hcnkem.com

[U107] JS：数字千分位
来源：http://xfc.nanxuanxn.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cix.xuanzx.com

[U108] JS：随机整数
来源：http://lpo.zhijiandao.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://owx.zhiwuduotai.top

[U109] JS：数组分组
来源：http://lxm.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://ras.ivvv.top

[U110] JS：数组分块
来源：http://jli.nanxinkj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bwm.zycfv.cn

[U111] JS：对象转 Map
来源：http://zdi.daxiang520.top

new Map(Object.entries(obj))
来源：http://msf.ybcxt.top

[U112] JS：字符串补位
来源：http://qkz.hcnkem.com

"7".padStart(3, "0")
来源：http://eik.hcnkem.com

[U113] JS：正则替换全部
来源：http://urc.dashuyun.cn

s.replaceAll("a", "b")
来源：http://pro.tanke756.top

[U114] JS：JSON 深比较
来源：http://ajr.quarkkingdee.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://aqk.nanxinkj.top

[U115] JS：生成 UUID
来源：http://dah.xylfe.cn

crypto.randomUUID()
来源：http://ejk.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://cno.cashguo.top

/** @param {string} name */ function f(name) {}
来源：http://nsp.hnxiangtu.top

[U117] JS：单元测试
来源：http://muh.hongshengwenyu.top

npm i -D vitest;  npx vitest
来源：http://bgt.xuanzx.com

[U118] JS：开发服务器
来源：http://bqc.cashguo.top

npm i -D vite;  npx vite
来源：http://rrs.bjfxy.top

[U119] JS：生产构建
来源：http://rxt.jinqigfzy.top

npx vite build
来源：http://jyx.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://cxg.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://qyo.xinyue.icu

================================================================================
来源：http://byu.redwolf501.top

统计汇总
来源：http://tbd.jlsjyb.cn

================================================================================
来源：http://okh.gzhubu.top

按语言统计（条）：
来源：http://dcf.zycfv.cn

Python ......... 252
来源：http://htl.epnwcf.com

PHP ............ 252
来源：http://lwe.cdnleiting.top

JavaScript ..... 252
来源：http://hsa.hammf.cn

TypeScript ..... 212
来源：http://amu.jinghuilouyu.cn

Java ........... 212
来源：http://xvx.xylfe.cn

Go ............. 212
来源：http://gvn.zhijiandao.cn

Ruby ........... 212
来源：http://tdg.iojbl.cn

C# ............. 212
来源：http://ics.hesvh.cn

C .............. 30
来源：http://bhc.ehwqpu.com

C++ ............ 30
来源：http://jzm.zhengqikj.top

SQL ............ 90
来源：http://xtt.yongpay.top

Bash ........... 80
来源：http://sqe.chenlongwang.top

Kotlin ......... 15
来源：http://ojn.hnxiangtu.top

Swift .......... 15
来源：http://alb.tian-w.cn

Lua ............ 10
来源：http://eyg.pycfn.com

Perl ........... 10
来源：http://mmq.nanxuanxn.top

Scala .......... 10
来源：http://vjw.yanxiufei.cn

------------------------------------
来源：http://qag.feifeiyinyue.top

合计 ........... 2106 条
来源：http://fon.nanxinkj.top

按章节统计：
来源：http://sqn.hesvh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://foy.dashuyun.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uzq.gogol.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wsr.tian-w.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zrv.zycfv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pbj.hammf.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fwu.jqgfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bmx.316326.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vbk.iojbl.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://naj.hywenlv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hsz.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ltv.jinqigfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xfn.hammf.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dxy.zhoulong.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qvi.316326.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://akf.hcnkem.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bfx.nanxinkj.top

Q SQL 专题                              90
来源：http://vdo.ctjpmb.com

R Bash 专题                             80
来源：http://xpe.0kj1m.cn

S C / C++ 专题                          60
来源：http://mpv.jqgufenzy.top

T 其他语言补充                          60
来源：http://uol.andypj.xyz

U 高频实用片段                         120
来源：http://ahf.daria6918.cn

------------------------------------
来源：http://cod.jinqigufen.top

合计                                  2106 条
来源：http://lji.uphjek.com

--------------------------------------------------------------------------------
来源：http://qjp.shanyushiyangtech.top

使用提醒
来源：http://mix.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://fmp.tianlin.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eje.gogol.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://viu.xylfe.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jbq.cqqwz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://doo.hnxiangtu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vni.yj20258.top

—— 文件结束 ——
来源：http://yvp.yuxming.cn

================================================================================
来源：http://hpj.xuanzx.com

程序语言常见例子速查手册（2024 版）
来源：http://bum.xziqi.cn

Common Programming Examples Cheat Book
来源：http://lif.ybcxt.top

================================================================================
来源：http://nar.jinyuanbaomall.cn

【收录内容】
来源：http://pgn.iojbl.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rvs.kuanghao11.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pqs.zhengqikj.top

SQL · Bash · C · C++
来源：http://yjg.jqgfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dhu.fzhhl.top

【使用说明】
来源：http://ufh.yonumen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sgk.zhixingplan.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jim.yanxiufei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mpc.xziqi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bvc.gotoacloud.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kjy.ivvv.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pvg.jinyuanbaomall.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ael.yuanzhike.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hlz.jinyuanbaomall.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jcr.jinyuanbaomall.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dwd.xuetiantiany.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cow.zhiwuduotai.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hsr.shuidangran.top

【文件统计】
来源：http://ewg.tianlin.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://szt.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://cyf.gzhubu.top

目  录
来源：http://tii.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://xzc.xuetiantiany.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sqr.yfazqb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hlq.sufxvd.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gtp.gogol.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://eim.yj20258888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ccw.andypj.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tmo.ctjpmb.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nwr.hongshengwenyu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://our.cucudq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rtm.yueranfly.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://eap.tarul.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fqz.ivvv.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gcl.chenzaomai.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ulx.ivvv.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xee.c1oappe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ity.jinqigufen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qvl.haohaochexian.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vve.tanke756.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://sfr.daria6918.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sqd.xuetiantiany.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wzo.zhongyouzk.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://szh.cheryme.top

================================================================================
来源：http://ycw.tarul.cn

A. 基础语法与类型
来源：http://tlj.nanxuanxn.top

================================================================================
来源：http://chc.birdmap.top

[A01] Hello World
来源：http://yuv.sweek.top


<!-- 参考信息 -->