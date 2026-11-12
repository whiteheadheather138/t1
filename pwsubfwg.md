代发 wailian999

[U31] Py：单测
来源：http://dti.ywan-chungtsiang.top

python -m pytest -q
来源：http://pkw.nwbrower.top

[U32] Py：代码格式化
来源：http://byh.gzhubu.top

ruff format . && ruff check --fix .
来源：http://scv.zhixingplan.top

[U33] Py：打包发布
来源：http://wbj.zhongyouzk.top

python -m build  （依赖 pyproject.toml）
来源：http://bgf.haohaochexian.top

[U34] Py：判断编码
来源：http://psf.yfazqb.com

chardet.detect(raw)
来源：http://xvf.bbcook.cn

[U35] Py：发送邮件
来源：http://xch.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pvq.sxryk.cn

[U36] Py：定时任务
来源：http://kud.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://fmw.hnxiangtu.top

[U37] Py：读写 Excel
来源：http://lno.ywan-chungtsiang.top

pandas.read_excel / DataFrame.to_excel
来源：http://agl.xziqi.cn

[U38] Py：获取脚本所在目录
来源：http://nox.zhaomingkeji.xyz

Path(__file__).resolve().parent
来源：http://hlg.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://tqv.xziqi.cn

sys.stdout.isatty()
来源：http://hdr.cashguo.top

[U40] Py：打印到标准错误
来源：http://xwm.ppjwa.cn

print("err", file=sys.stderr)
来源：http://iso.ppjwa.cn

[U41] PHP：初始化 Composer 项目
来源：http://bzl.jinqigfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xeh.xziqi.cn

[U42] PHP：PSR-4 自动加载
来源：http://fyj.andypj.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nkh.xylfe.cn

[U43] PHP：声明命名空间
来源：http://hnz.meibo888.top

namespace App\Http;
来源：http://aan.fengsongda.top

[U44] PHP：开启严格类型
来源：http://wqr.sysykeji.top

declare(strict_types=1);
来源：http://ebr.jianghu66.top

[U45] PHP：类型声明与返回类型
来源：http://kkx.tian-w.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qcz.cdnleiting.top

[U46] PHP：可空类型
来源：http://dkq.cheryme.top

?string $name = null
来源：http://rbv.aibaodan.cn

[U47] PHP：联合类型
来源：http://dqg.ywan-chungtsiang.top

int|string $id
来源：http://mmx.hesvh.cn

[U48] PHP：纯枚举
来源：http://zbz.bjfxy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kie.9152youxi.cn

[U49] PHP：只读属性
来源：http://vyb.ywan-chungtsiang.top

public readonly string $name
来源：http://zpc.yvedp.cn

[U50] PHP：构造器属性提升
来源：http://btm.uphjek.com

public function __construct(private int $id) {}
来源：http://mkn.zhoulong.xyz

[U51] PHP：数组解构
来源：http://cbn.dianchejie.cn

[$a, $b] = $arr;
来源：http://qgv.zhaomingkeji.xyz

[U52] PHP：箭头函数
来源：http://vnj.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://bka.ivvv.top

[U53] PHP：空合并运算符
来源：http://ewd.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://drb.zdqjudy.top

[U54] PHP：空安全调用
来源：http://yoy.ydjk.org.cn

$obj?->method()
来源：http://psx.tian-w.cn

[U55] PHP：match 表达式
来源：http://omz.tian-w.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://peq.andypj.xyz

[U56] PHP：命名参数
来源：http://jrr.xinyue.icu

f(a: 1, b: 2)
来源：http://nlk.vqdsnc.cn

[U57] PHP：字符串插值
来源：http://ivi.jqgfzy.top

"值: {$a}"
来源：http://roo.nanxinkj.top

[U58] PHP：数组三件套
来源：http://ewa.tarul.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hmx.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://kvd.hcnkem.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ruw.cdnleiting.top

[U60] PHP：JSON 编解码
来源：http://uia.chenjidiqi.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zqh.hesvh.cn

[U61] PHP：正则
来源：http://vdx.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dvr.yongpay.top

[U62] PHP：日期对象
来源：http://hxy.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ejr.hfpthk.cn

[U63] PHP：文件读写
来源：http://wee.smart0.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xxg.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://mst.tarul.cn

glob("dir/*.php");  scandir("dir");
来源：http://mvu.jinqigfzy.top

[U65] PHP：会话
来源：http://mgq.yanxiufei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xvv.meibo888.top

[U66] PHP：设置 Cookie
来源：http://ytu.cucudq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xvm.tanke756.top

[U67] PHP：处理文件上传
来源：http://cyf.ydzc1.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://glz.chenlongwang.top

[U68] PHP：PDO 连接
来源：http://wxs.ctjpmb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://stu.shanyushiyangkeji.top

[U69] PHP：PDO 预处理
来源：http://hmu.tarul.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qcv.yangfankeji.com

[U70] PHP：PDO 事务
来源：http://zqw.bjfxy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://skv.yangfankeji.com

[U71] PHP：抛出异常
来源：http://dzy.shuidangran.top

throw new RuntimeException("失败", 500);
来源：http://boa.sxryk.cn

[U72] PHP：写错误日志
来源：http://eeh.xylfe.cn

error_log("失败: " . $e->getMessage());
来源：http://peq.uphjek.com

[U73] PHP：读取 ini 配置
来源：http://mke.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://gll.yongpay.top

[U74] PHP：读取环境变量
来源：http://avt.zdqjudy.top

getenv("APP_ENV") ?: "production"
来源：http://nom.daxiang520.top

[U75] PHP：依赖注入
来源：http://nlu.vqdsnc.cn

composer require psr/container
来源：http://hau.ctjpmb.com

[U76] PHP：简单路由
来源：http://wax.cashguo.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nrm.ybcxt.top

[U77] PHP：模板渲染
来源：http://yax.xziqi.cn

composer require twig/twig
来源：http://jyb.yanxiufei.cn

[U78] PHP：单元测试
来源：http://ybz.havefunace.top

composer require --dev phpunit/phpunit
来源：http://wxp.jinghuilouyu.cn

[U79] PHP：静态分析
来源：http://zgb.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://fso.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://oot.fengsongda.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rbv.bbcook.cn

[U81] JS：初始化项目
来源：http://jpf.9152youxi.cn

npm init -y;  npm i express
来源：http://lum.jqgfzy.top

[U82] JS：package.json 脚本
来源：http://itl.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://syh.mhx1999.top

[U83] JS：ES Module 导入导出
来源：http://nkw.quarkkingdee.top

export const a = 1;  import { a } from "./m.js";
来源：http://bhl.andypj.xyz

[U84] JS：CommonJS 写法
来源：http://wts.svipenyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cip.hywenlv.cn

[U85] JS：可选链
来源：http://aac.yuxming.cn

a?.b?.c
来源：http://pxd.fktsv.cn

[U86] JS：空值合并
来源：http://ljh.hfpthk.cn

a ?? b
来源：http://exk.0kj1m.cn

[U87] JS：解构默认值
来源：http://wlq.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://ilz.nanxuanxn.top

[U88] JS：对象展开合并
来源：http://ylh.cheryme.top

{ ...a, ...b }
来源：http://nbp.redwolf501.top

[U89] JS：数组去重
来源：http://luk.zhongyouzk.top

[...new Set(arr)]
来源：http://cll.yj20258888.top

[U90] JS：数字数组排序
来源：http://pho.shuidangran.top

[...arr].sort((a, b) => a - b)
来源：http://lnp.pengpengdd.cyou

[U91] JS：对象键值遍历
来源：http://vcs.guowangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kcs.yj20258888.top

[U92] JS：深拷贝
来源：http://elh.52xcode.cn

structuredClone(obj)
来源：http://qeg.cashguo.top

[U93] JS：模板字符串
来源：http://obl.jqgufenzy.top

`共 ${n} 条`
来源：http://bqx.feifeiyinyue.top

[U94] JS：箭头函数
来源：http://yox.jinghuilouyu.cn

const double = x => x * 2;
来源：http://nxb.nwbrower.top

[U95] JS：Promise 包装
来源：http://xok.epnwcf.com

new Promise((resolve, reject) => {})
来源：http://tcz.hnqzz.top

[U96] JS：async/await 与异常
来源：http://zvc.fehbvm.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bjg.ydjk.org.cn

[U97] JS：并发请求
来源：http://hyn.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ita.chenzaomai.com

[U98] JS：fetch 带 JSON
来源：http://ull.redwolf501.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eaf.nanxuanxn.top

[U99] JS：事件监听
来源：http://zkn.bbcook.cn

el.addEventListener("click", e => {})
来源：http://rpy.zhixingplan.top

[U100] JS：DOM 查询
来源：http://phj.jinghuilouyu.cn

document.querySelector(".item")
来源：http://kgr.jqgfzy.top

[U101] JS：classList 操作
来源：http://zwj.yangfankeji.com

el.classList.toggle("active")
来源：http://ptu.fzhhl.top

[U102] JS：本地存储
来源：http://fpv.jqgfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zrs.ivvv.top

[U103] JS：定时器
来源：http://keu.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yuq.zhengqikj.top

[U104] JS：防抖
来源：http://kpw.xuetiantiany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dxq.uphjek.com

[U105] JS：节流
来源：http://ere.fanxiaobao.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pme.shanyushiyangtech.top

[U106] JS：日期格式化
来源：http://alu.gogol.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mfb.zhoulong.xyz

[U107] JS：数字千分位
来源：http://sbm.zycfv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vmm.hammf.cn

[U108] JS：随机整数
来源：http://uel.zdbjq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hid.hfpthk.cn

[U109] JS：数组分组
来源：http://pmg.hywenlv.cn

Object.groupBy(arr, x => x.type)
来源：http://vnd.yuxming.cn

[U110] JS：数组分块
来源：http://hao.jinqigfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gic.fengsongda.top

[U111] JS：对象转 Map
来源：http://rgd.gaohongyu789.top

new Map(Object.entries(obj))
来源：http://mkh.ivvv.top

[U112] JS：字符串补位
来源：http://ddw.zhixingplan.top

"7".padStart(3, "0")
来源：http://eag.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://gsc.shangyingyoupin.top

s.replaceAll("a", "b")
来源：http://miz.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://cet.pengpengdd.cyou

JSON.stringify(a) === JSON.stringify(b)
来源：http://erb.chenzaomai.com

[U115] JS：生成 UUID
来源：http://pjh.redwolf501.top

crypto.randomUUID()
来源：http://shz.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://hgh.andypj.xyz

/** @param {string} name */ function f(name) {}
来源：http://mhu.zhiwuduotai.top

[U117] JS：单元测试
来源：http://fas.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://nzt.ehwqpu.com

[U118] JS：开发服务器
来源：http://dxi.cdnleiting.top

npm i -D vite;  npx vite
来源：http://ehw.andypj.xyz

[U119] JS：生产构建
来源：http://gcq.hesvh.cn

npx vite build
来源：http://dbh.hcnkem.com

[U120] JS：读取环境变量（Vite）
来源：http://cct.yonumen.top

import.meta.env.VITE_API_URL
来源：http://tqi.quarkkingdee.top

================================================================================
来源：http://pqm.vqdsnc.cn

统计汇总
来源：http://jjm.cashguo.top

================================================================================
来源：http://wkh.vqdsnc.cn

按语言统计（条）：
来源：http://czi.yanxiufei.cn

Python ......... 252
来源：http://hcb.jqgufenzy.top

PHP ............ 252
来源：http://hmq.daxiang520.top

JavaScript ..... 252
来源：http://ibu.cqqwz.cn

TypeScript ..... 212
来源：http://mby.birdmap.top

Java ........... 212
来源：http://spy.zhaomingkeji.xyz

Go ............. 212
来源：http://zik.wangdashe.top

Ruby ........... 212
来源：http://ezp.shanyushiyangtech.top

C# ............. 212
来源：http://ubr.hammf.cn

C .............. 30
来源：http://jse.jqgufenzy.top

C++ ............ 30
来源：http://zhy.jqgfzy.top

SQL ............ 90
来源：http://uwz.jyoumei.cn

Bash ........... 80
来源：http://pha.nanxuanxn.top

Kotlin ......... 15
来源：http://hmu.havefunace.top

Swift .......... 15
来源：http://peg.sweek.top

Lua ............ 10
来源：http://vfw.fengsongda.top

Perl ........... 10
来源：http://ugp.nwbrower.top

Scala .......... 10
来源：http://zpx.dashuyun.cn

------------------------------------
来源：http://oeu.aibaodan.cn

合计 ........... 2106 条
来源：http://nap.nwbrower.top

按章节统计：
来源：http://oeq.guowangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pzb.aizwys.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://szd.ydzc1.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pcr.hfpthk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qhk.yangfankeji.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://els.fzhhl.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ygi.sweek.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nfx.snrcjt.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pcn.vehdjk.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ngs.ywan-chungtsiang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://orb.yj202588.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cvf.nanxuanxn.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tcf.shanyushiyangtech.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xdk.zhijiandao.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kaw.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hxt.kuanghao11.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xcy.uphjek.com

Q SQL 专题                              90
来源：http://yha.cucudq.cn

R Bash 专题                             80
来源：http://zqk.nanxuanxn.top

S C / C++ 专题                          60
来源：http://rfl.hysaishi.cn

T 其他语言补充                          60
来源：http://wfv.fanxiaobao.xyz

U 高频实用片段                         120
来源：http://cwp.chenzaomai.com

------------------------------------
来源：http://xhu.yj20258888.top

合计                                  2106 条
来源：http://fge.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://xwt.cqqwz.cn

使用提醒
来源：http://ngp.52xcode.cn

--------------------------------------------------------------------------------
来源：http://pdj.c1oappe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://djh.dashuyun.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://isy.chenjidiqi.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wfp.fanxiaobao.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://aje.sweek.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rsa.zhaomingkeji.xyz

—— 文件结束 ——
来源：http://fwb.ehwqpu.com

================================================================================
来源：http://ytz.kuanghao11.cn

程序语言常见例子速查手册（2024 版）
来源：http://ibk.yuxming.cn

Common Programming Examples Cheat Book
来源：http://cfo.sysykeji.top

================================================================================
来源：http://deg.birdmap.top

【收录内容】
来源：http://wsr.fzhhl.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dou.yanxiufei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ckk.pengpengdd.cyou

SQL · Bash · C · C++
来源：http://emd.cdnleiting.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tvr.xziqi.cn

【使用说明】
来源：http://wju.jinyuanbaomall.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tro.bjfxy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://srn.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sjv.hongshengwenyu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gef.sysykeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zbz.havefunace.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ywp.gzhubu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ydf.kuanghao11.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hmv.0kj1m.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://efj.ybcxt.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pfb.yvedp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fsh.yj20258.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jgr.jlsjyb.cn

【文件统计】
来源：http://nwn.fzhhl.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hix.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://dov.hnxiangtu.top

目  录
来源：http://jkh.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://tyk.shuidangran.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eqg.sxryk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mrk.fktsv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://icc.sjlbkw.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xrf.0kj1m.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iek.tian-w.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://con.tanke756.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://afy.cqqwz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mva.yuanzhike.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zcz.yonumen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nzb.andypj.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kzb.cucudq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lyl.yfazqb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pju.tian-w.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://egz.fzhhl.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gyx.uphjek.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tug.ywan-chungtsiang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dsu.fengsongda.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://uww.xingfuxueyuan.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bzu.zdbjq.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://seb.jlsjyb.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://efn.yongpay.top

================================================================================
来源：http://deq.ydzc1.top

A. 基础语法与类型
来源：http://eum.iojbl.cn

================================================================================
来源：http://vre.gzhubu.top

[A01] Hello World
来源：http://kbf.jinqigfzy.top

Py:   print("Hello, World!")
来源：http://zxb.chenlongwang.top

PHP:  echo "Hello, World!";
来源：http://zje.jianghu66.top

JS:   console.log("Hello, World!");
来源：http://ott.sxryk.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qrp.hcnkem.com

Java: System.out.println("Hello, World!");
来源：http://hoi.tarul.cn

Go:   fmt.Println("Hello, World!")
来源：http://emo.bbcook.cn

Ruby: puts "Hello, World!"
来源：http://kwc.ivvv.top

C#:   Console.WriteLine("Hello, World!");
来源：http://bsk.aizwys.cn

[A02] 变量声明与赋值
来源：http://jrp.shanyushiyangtech.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dpy.hongshengwenyu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://fsk.tian-w.cn

JS:   let name = "Alex"; const age = 20;
来源：http://oxz.meibo888.top


<!-- 参考信息 -->