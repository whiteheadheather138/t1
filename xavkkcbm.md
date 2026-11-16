代发 wailian999

[U31] Py：单测
来源：http://hka.tanke756.top

python -m pytest -q
来源：http://ooj.vqdsnc.cn

[U32] Py：代码格式化
来源：http://jtc.zhoulong.xyz

ruff format . && ruff check --fix .
来源：http://qcu.jqgufenzy.top

[U33] Py：打包发布
来源：http://ufy.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://wrw.jinqigfzy.top

[U34] Py：判断编码
来源：http://mqi.svipenyu.cn

chardet.detect(raw)
来源：http://ofr.kuanghao11.cn

[U35] Py：发送邮件
来源：http://suw.tarul.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hrq.sjlbkw.cn

[U36] Py：定时任务
来源：http://zgp.zhixingplan.top

schedule.every(10).minutes.do(job)
来源：http://ezz.chenzaomai.com

[U37] Py：读写 Excel
来源：http://gsj.hfpthk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://urg.aibaodan.cn

[U38] Py：获取脚本所在目录
来源：http://teo.sxryk.cn

Path(__file__).resolve().parent
来源：http://muf.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://vpm.guowangkeji.top

sys.stdout.isatty()
来源：http://uax.hammf.cn

[U40] Py：打印到标准错误
来源：http://yjm.jqgfzy.top

print("err", file=sys.stderr)
来源：http://bzh.yuanzhike.top

[U41] PHP：初始化 Composer 项目
来源：http://rko.dianchejie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bze.cqqwz.cn

[U42] PHP：PSR-4 自动加载
来源：http://etz.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nut.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://jrm.xuanzx.com

namespace App\Http;
来源：http://tfc.xinyue.icu

[U44] PHP：开启严格类型
来源：http://lsa.dashuyun.cn

declare(strict_types=1);
来源：http://qeg.gogol.net.cn

[U45] PHP：类型声明与返回类型
来源：http://mah.yfazqb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://wmg.yj202588.top

[U46] PHP：可空类型
来源：http://xnd.zycfv.cn

?string $name = null
来源：http://uzl.snrcjt.cn

[U47] PHP：联合类型
来源：http://uhb.pengpengdd.cyou

int|string $id
来源：http://dsu.wangdashe.top

[U48] PHP：纯枚举
来源：http://mwv.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zqv.shangyingyoupin.top

[U49] PHP：只读属性
来源：http://ygh.ydjk.org.cn

public readonly string $name
来源：http://nxb.tanke756.top

[U50] PHP：构造器属性提升
来源：http://pma.xuanzx.com

public function __construct(private int $id) {}
来源：http://vsc.hnxiangtu.top

[U51] PHP：数组解构
来源：http://vet.zhixingplan.top

[$a, $b] = $arr;
来源：http://rjk.zhoulong.xyz

[U52] PHP：箭头函数
来源：http://erc.xuetiantiany.cn

$double = fn($x) => $x * 2;
来源：http://drv.ehwqpu.com

[U53] PHP：空合并运算符
来源：http://fis.hysaishi.cn

$v = $a ?? $b ?? "default";
来源：http://lmw.haohaochexian.top

[U54] PHP：空安全调用
来源：http://zaa.yueranfly.top

$obj?->method()
来源：http://uit.bbcook.cn

[U55] PHP：match 表达式
来源：http://fef.bbcook.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://his.jinqigfzy.top

[U56] PHP：命名参数
来源：http://cjy.pengpengdd.cyou

f(a: 1, b: 2)
来源：http://tsx.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://chu.wangshuangyany.cn

"值: {$a}"
来源：http://xzy.daxiang520.top

[U58] PHP：数组三件套
来源：http://mij.yuanzhike.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aen.yj202588.top

[U59] PHP：自定义排序
来源：http://kur.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://apg.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://gtp.jqgfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kgf.ppjwa.cn

[U61] PHP：正则
来源：http://uwk.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://odf.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://out.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://znh.cqqwz.cn

[U63] PHP：文件读写
来源：http://hai.zdqjudy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nyo.daxiang520.top

[U64] PHP：目录遍历
来源：http://tar.xylfe.cn

glob("dir/*.php");  scandir("dir");
来源：http://srd.sysykeji.top

[U65] PHP：会话
来源：http://kyk.hnxiangtu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gee.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://cgt.jinghuilouyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://evc.mhx1999.top

[U67] PHP：处理文件上传
来源：http://nwv.dianchejie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hvv.ppjwa.cn

[U68] PHP：PDO 连接
来源：http://biq.sufxvd.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jtq.redwolf501.top

[U69] PHP：PDO 预处理
来源：http://vcj.guannengcc.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uaa.ivvv.top

[U70] PHP：PDO 事务
来源：http://mjg.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rrq.jqgfzy.top

[U71] PHP：抛出异常
来源：http://wle.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://uio.haohaochexian.top

[U72] PHP：写错误日志
来源：http://mud.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://jle.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://uuh.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://vyu.xinyue.icu

[U74] PHP：读取环境变量
来源：http://bqx.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://qsx.sxryk.cn

[U75] PHP：依赖注入
来源：http://czm.ehwqpu.com

composer require psr/container
来源：http://xdo.hongshengwenyu.top

[U76] PHP：简单路由
来源：http://qxn.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xlb.yfazqb.com

[U77] PHP：模板渲染
来源：http://bpv.jyoumei.cn

composer require twig/twig
来源：http://oul.fehbvm.com

[U78] PHP：单元测试
来源：http://vzl.shangyingyoupin.top

composer require --dev phpunit/phpunit
来源：http://yqb.yuanzhike.top

[U79] PHP：静态分析
来源：http://xrf.bjfxy.top

composer require --dev phpstan/phpstan
来源：http://ojd.shanyushiyangkeji.top

[U80] PHP：代码规范修复
来源：http://nwx.kuanghao11.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xbf.meibo888.top

[U81] JS：初始化项目
来源：http://lec.zhengqikj.top

npm init -y;  npm i express
来源：http://dxs.xylfe.cn

[U82] JS：package.json 脚本
来源：http://xob.hysaishi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vqi.quarkkingdee.top

[U83] JS：ES Module 导入导出
来源：http://jqs.bbcook.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cbk.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://imc.ywan-chungtsiang.top

module.exports = { a };  const { a } = require("./m");
来源：http://vtq.hnxiangtu.top

[U85] JS：可选链
来源：http://gyv.yuanzhike.top

a?.b?.c
来源：http://zne.gogol.net.cn

[U86] JS：空值合并
来源：http://vjm.hongshengwenyu.top

a ?? b
来源：http://woe.xuanzx.com

[U87] JS：解构默认值
来源：http://kkg.iojbl.cn

const { a = 1, b = 2 } = obj;
来源：http://znd.fehbvm.com

[U88] JS：对象展开合并
来源：http://gjs.ctjpmb.com

{ ...a, ...b }
来源：http://sup.tian-w.cn

[U89] JS：数组去重
来源：http://soi.hnxiangtu.top

[...new Set(arr)]
来源：http://jyc.sjlbkw.cn

[U90] JS：数字数组排序
来源：http://uez.zycfv.cn

[...arr].sort((a, b) => a - b)
来源：http://etr.yongpay.top

[U91] JS：对象键值遍历
来源：http://nji.fzhhl.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qmj.daxiang520.top

[U92] JS：深拷贝
来源：http://wyy.zdqjudy.top

structuredClone(obj)
来源：http://hsa.fanxiaobao.xyz

[U93] JS：模板字符串
来源：http://qst.9152youxi.cn

`共 ${n} 条`
来源：http://teb.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://zyt.tian-w.cn

const double = x => x * 2;
来源：http://ita.pycfn.com

[U95] JS：Promise 包装
来源：http://xhs.zdbjq.cn

new Promise((resolve, reject) => {})
来源：http://kij.sweek.top

[U96] JS：async/await 与异常
来源：http://tgb.yj20258.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://myt.sufxvd.cn

[U97] JS：并发请求
来源：http://dxa.gogol.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pib.jlsjyb.cn

[U98] JS：fetch 带 JSON
来源：http://vgd.fehbvm.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://euf.ehwqpu.com

[U99] JS：事件监听
来源：http://vaq.tianlin.xyz

el.addEventListener("click", e => {})
来源：http://blx.tianlin.xyz

[U100] JS：DOM 查询
来源：http://egy.ybcxt.top

document.querySelector(".item")
来源：http://uzs.redwolf501.top

[U101] JS：classList 操作
来源：http://owk.hfpthk.cn

el.classList.toggle("active")
来源：http://dbz.uphjek.com

[U102] JS：本地存储
来源：http://qqo.nanxuanxn.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nfe.andypj.xyz

[U103] JS：定时器
来源：http://qoe.cucudq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eir.sufxvd.cn

[U104] JS：防抖
来源：http://drp.jqgufenzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wvl.pengpengdd.cyou

[U105] JS：节流
来源：http://uqs.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pjx.mhx1999.top

[U106] JS：日期格式化
来源：http://wjy.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tff.aizwys.cn

[U107] JS：数字千分位
来源：http://wek.guannengcc.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hrh.ivvv.top

[U108] JS：随机整数
来源：http://tqc.gaohongyu789.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iya.yonumen.top

[U109] JS：数组分组
来源：http://lll.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://efw.pycfn.com

[U110] JS：数组分块
来源：http://fxl.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rre.fehbvm.com

[U111] JS：对象转 Map
来源：http://fym.tian-w.cn

new Map(Object.entries(obj))
来源：http://vek.iojbl.cn

[U112] JS：字符串补位
来源：http://kcu.havefunace.top

"7".padStart(3, "0")
来源：http://spo.smart0.xyz

[U113] JS：正则替换全部
来源：http://vjg.316326.xyz

s.replaceAll("a", "b")
来源：http://vbh.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://pzy.cucudq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qpf.zhongyouzk.top

[U115] JS：生成 UUID
来源：http://wbd.iojbl.cn

crypto.randomUUID()
来源：http://rjy.haohaochexian.top

[U116] JS：类型检查（JSDoc）
来源：http://nbx.guannengcc.top

/** @param {string} name */ function f(name) {}
来源：http://tnu.nanxuanxn.top

[U117] JS：单元测试
来源：http://qkh.snrcjt.cn

npm i -D vitest;  npx vitest
来源：http://xjd.shanyushiyangkeji.top

[U118] JS：开发服务器
来源：http://xlr.xuanzx.com

npm i -D vite;  npx vite
来源：http://wnc.hnxiangtu.top

[U119] JS：生产构建
来源：http://zuf.ehwqpu.com

npx vite build
来源：http://wim.jyoumei.cn

[U120] JS：读取环境变量（Vite）
来源：http://aia.shangyingyoupin.top

import.meta.env.VITE_API_URL
来源：http://ztb.xuanzx.com

================================================================================
来源：http://srz.redwolf501.top

统计汇总
来源：http://cex.9152youxi.cn

================================================================================
来源：http://pwv.yangfankeji.com

按语言统计（条）：
来源：http://sbg.bjfxy.top

Python ......... 252
来源：http://ghb.zhoulong.xyz

PHP ............ 252
来源：http://jid.zycfv.cn

JavaScript ..... 252
来源：http://bxp.fktsv.cn

TypeScript ..... 212
来源：http://ogu.quarkkingdee.top

Java ........... 212
来源：http://dgt.316326.xyz

Go ............. 212
来源：http://bum.hesvh.cn

Ruby ........... 212
来源：http://hdk.iojbl.cn

C# ............. 212
来源：http://zvd.zhongyouzk.top

C .............. 30
来源：http://eej.redwolf501.top

C++ ............ 30
来源：http://toa.pycfn.com

SQL ............ 90
来源：http://tnc.shangyingyoupin.top

Bash ........... 80
来源：http://qks.yj20258.top

Kotlin ......... 15
来源：http://fzu.shangyingyoupin.top

Swift .......... 15
来源：http://cxs.feifeiyinyue.top

Lua ............ 10
来源：http://unh.fengsongda.top

Perl ........... 10
来源：http://hxg.pengpengdd.cyou

Scala .......... 10
来源：http://owz.hnqzz.top

------------------------------------
来源：http://rcy.jinghuilouyu.cn

合计 ........... 2106 条
来源：http://yst.gotoacloud.top

按章节统计：
来源：http://aju.dianchejie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eyk.nwbrower.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tvz.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gyi.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cqr.tianlin.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wgg.cqqwz.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cov.ppjwa.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qcj.hcnkem.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bgx.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://llh.jlsjyb.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://get.yonumen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rqi.cashguo.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fxi.tian-w.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://azq.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sbb.aizwys.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xwz.snrcjt.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cju.daxiang520.top

Q SQL 专题                              90
来源：http://wsv.pycfn.com

R Bash 专题                             80
来源：http://htc.xylfe.cn

S C / C++ 专题                          60
来源：http://fce.hysaishi.cn

T 其他语言补充                          60
来源：http://tcg.yj20258888.top

U 高频实用片段                         120
来源：http://uma.nanxuanxn.top

------------------------------------
来源：http://fku.yfazqb.com

合计                                  2106 条
来源：http://uig.vehdjk.com

--------------------------------------------------------------------------------
来源：http://can.andypj.xyz

使用提醒
来源：http://ttu.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://mqt.fehbvm.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://drl.chenlongwang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lku.ydzc1.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pdt.ctjpmb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://vgg.sweek.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oam.pengpengdd.cyou

—— 文件结束 ——
来源：http://spm.hysaishi.cn

================================================================================
来源：http://cpp.cucudq.cn

程序语言常见例子速查手册（2024 版）
来源：http://fhe.xuetiantiany.cn

Common Programming Examples Cheat Book
来源：http://qcp.birdmap.top

================================================================================
来源：http://ouf.ydzc1.top

【收录内容】
来源：http://kmz.sjlbkw.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mjx.hysaishi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dzj.gaohongyu789.top

SQL · Bash · C · C++
来源：http://jnt.ivvv.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xod.tian-w.cn

【使用说明】
来源：http://qoq.vehdjk.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gcg.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://flw.jinqigufen.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://khp.fehbvm.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cyz.xinyue.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://jyl.svipenyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kct.zdbjq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uvs.hysaishi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wnz.gaohongyu789.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wjc.ybcxt.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xaz.gaohongyu789.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vwu.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cvo.andypj.xyz

【文件统计】
来源：http://mda.epnwcf.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rvp.xinyue.icu

--------------------------------------------------------------------------------
来源：http://zqj.52xcode.cn

目  录
来源：http://qmh.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://vap.bbcook.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mto.hesvh.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wfd.jinqigufen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hmm.daria6918.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rty.yj20258.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vrl.pengpengdd.cyou

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lwv.fktsv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dtx.gogol.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ibv.pycfn.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zbu.vqdsnc.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kde.hnxiangtu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fzj.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jwj.zdqjudy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nyw.cashguo.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wrx.cqqwz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mhh.shanyushiyangtech.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gcg.jqgfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iqa.chenlongwang.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://fej.hnxiangtu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bsk.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rzi.cashguo.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bqv.zycfv.cn

================================================================================
来源：http://ciy.dashuyun.cn

A. 基础语法与类型
来源：http://alg.yj20258.top

================================================================================
来源：http://ikv.0kj1m.cn

[A01] Hello World
来源：http://dsy.andypj.xyz

Py:   print("Hello, World!")
来源：http://tjr.jqgfzy.top

PHP:  echo "Hello, World!";
来源：http://taa.yangfankeji.com

JS:   console.log("Hello, World!");
来源：http://glh.nwbrower.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bcz.sxryk.cn

Java: System.out.println("Hello, World!");
来源：http://fum.zycfv.cn

Go:   fmt.Println("Hello, World!")
来源：http://tpu.quarkkingdee.top

Ruby: puts "Hello, World!"
来源：http://czo.sysykeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fph.snrcjt.cn

[A02] 变量声明与赋值
来源：http://qgx.c1oappe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uzw.yfazqb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://ozv.xuanzx.com

JS:   let name = "Alex"; const age = 20;
来源：http://eey.shanyushiyangtech.top


<!-- 参考信息 -->