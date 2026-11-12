代发 wailian999

[U33] Py：打包发布
来源：http://pvr.havefunace.top

python -m build  （依赖 pyproject.toml）
来源：http://yxr.fzhhl.top

[U34] Py：判断编码
来源：http://sxq.zhixingplan.top

chardet.detect(raw)
来源：http://zuv.tian-w.cn

[U35] Py：发送邮件
来源：http://exp.tian-w.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aqg.yangfankeji.com

[U36] Py：定时任务
来源：http://ags.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://tbh.yvedp.cn

[U37] Py：读写 Excel
来源：http://kvz.aizwys.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wqy.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://hwa.chenzaomai.com

Path(__file__).resolve().parent
来源：http://rdm.kuanghao11.cn

[U39] Py：判断是否在交互环境
来源：http://jpf.hcnkem.com

sys.stdout.isatty()
来源：http://lch.hnxiangtu.top

[U40] Py：打印到标准错误
来源：http://mvz.meibo888.top

print("err", file=sys.stderr)
来源：http://fcp.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://xpa.fktsv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dvp.chenzaomai.com

[U42] PHP：PSR-4 自动加载
来源：http://vvb.haohaochexian.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jcm.tarul.cn

[U43] PHP：声明命名空间
来源：http://fgp.sufxvd.cn

namespace App\Http;
来源：http://jdl.mhx1999.top

[U44] PHP：开启严格类型
来源：http://jgg.wangshuangyany.cn

declare(strict_types=1);
来源：http://rix.sweek.top

[U45] PHP：类型声明与返回类型
来源：http://nxe.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tfr.jqgfzy.top

[U46] PHP：可空类型
来源：http://rgr.yuanzhike.top

?string $name = null
来源：http://hgh.daxiang520.top

[U47] PHP：联合类型
来源：http://bzz.hongshengwenyu.top

int|string $id
来源：http://oxu.cashguo.top

[U48] PHP：纯枚举
来源：http://zew.cheryme.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://udu.gogol.net.cn

[U49] PHP：只读属性
来源：http://jgp.jqgfzy.top

public readonly string $name
来源：http://cqz.pycfn.com

[U50] PHP：构造器属性提升
来源：http://yxg.tianlin.xyz

public function __construct(private int $id) {}
来源：http://sch.hesvh.cn

[U51] PHP：数组解构
来源：http://pmq.hfpthk.cn

[$a, $b] = $arr;
来源：http://clt.nanxinkj.top

[U52] PHP：箭头函数
来源：http://tgv.smart0.xyz

$double = fn($x) => $x * 2;
来源：http://wzc.jqgufenzy.top

[U53] PHP：空合并运算符
来源：http://nxo.316326.xyz

$v = $a ?? $b ?? "default";
来源：http://xfa.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://saa.guowangkeji.top

$obj?->method()
来源：http://zuz.0kj1m.cn

[U55] PHP：match 表达式
来源：http://taw.xingfuxueyuan.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://agk.haohaochexian.top

[U56] PHP：命名参数
来源：http://tuw.hcnkem.com

f(a: 1, b: 2)
来源：http://awt.wangshuangyany.cn

[U57] PHP：字符串插值
来源：http://kie.redwolf501.top

"值: {$a}"
来源：http://kqg.aibaodan.cn

[U58] PHP：数组三件套
来源：http://zcg.sjlbkw.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zwm.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://dqj.yuxming.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ogc.yj202588.top

[U60] PHP：JSON 编解码
来源：http://vfe.birdmap.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://adg.hysaishi.cn

[U61] PHP：正则
来源：http://mjk.xuanzx.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gjc.meibo888.top

[U62] PHP：日期对象
来源：http://rkl.gaohongyu789.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fcq.snrcjt.cn

[U63] PHP：文件读写
来源：http://wvj.xziqi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qke.iojbl.cn

[U64] PHP：目录遍历
来源：http://pjz.xuanzx.com

glob("dir/*.php");  scandir("dir");
来源：http://nec.ydjk.org.cn

[U65] PHP：会话
来源：http://zqv.zhengqikj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ogb.sweek.top

[U66] PHP：设置 Cookie
来源：http://xvp.zhongyouzk.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rdr.jiagoushi.top

[U67] PHP：处理文件上传
来源：http://wuu.guannengcc.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ewl.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://xoj.andypj.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iuh.daxiang520.top

[U69] PHP：PDO 预处理
来源：http://res.fanxiaobao.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gua.zhengqikj.top

[U70] PHP：PDO 事务
来源：http://lkg.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vke.daria6918.cn

[U71] PHP：抛出异常
来源：http://nwl.fehbvm.com

throw new RuntimeException("失败", 500);
来源：http://arf.sxryk.cn

[U72] PHP：写错误日志
来源：http://rgk.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://beq.ctjpmb.com

[U73] PHP：读取 ini 配置
来源：http://oah.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://jst.c1oappe.top

[U74] PHP：读取环境变量
来源：http://xgf.sysykeji.top

getenv("APP_ENV") ?: "production"
来源：http://ojh.yfazqb.com

[U75] PHP：依赖注入
来源：http://jwb.yj20258888.top

composer require psr/container
来源：http://goe.tian-w.cn

[U76] PHP：简单路由
来源：http://abu.ppjwa.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zoo.hongshengwenyu.top

[U77] PHP：模板渲染
来源：http://cvm.xuanzx.com

composer require twig/twig
来源：http://pbk.yanxiufei.cn

[U78] PHP：单元测试
来源：http://cku.xinyue.icu

composer require --dev phpunit/phpunit
来源：http://jjg.zhengqikj.top

[U79] PHP：静态分析
来源：http://cme.hysaishi.cn

composer require --dev phpstan/phpstan
来源：http://wsu.aizwys.cn

[U80] PHP：代码规范修复
来源：http://zsn.vehdjk.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://qjp.shzxlz.cn

[U81] JS：初始化项目
来源：http://nah.hfpthk.cn

npm init -y;  npm i express
来源：http://rum.cashguo.top

[U82] JS：package.json 脚本
来源：http://enx.nanxuanxn.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mdv.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://lbk.yj20258.top

export const a = 1;  import { a } from "./m.js";
来源：http://rob.zhengqikj.top

[U84] JS：CommonJS 写法
来源：http://goi.tian-w.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fut.andypj.xyz

[U85] JS：可选链
来源：http://ekh.yuanzhike.top

a?.b?.c
来源：http://gcl.jqgufenzy.top

[U86] JS：空值合并
来源：http://mow.daxiang520.top

a ?? b
来源：http://xqr.nanxinkj.top

[U87] JS：解构默认值
来源：http://hiz.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://lot.jiagoushi.top

[U88] JS：对象展开合并
来源：http://bpz.fzhhl.top

{ ...a, ...b }
来源：http://wiz.jinqigufen.top

[U89] JS：数组去重
来源：http://xae.zhixingplan.top

[...new Set(arr)]
来源：http://icx.daxiang520.top

[U90] JS：数字数组排序
来源：http://jvn.zycfv.cn

[...arr].sort((a, b) => a - b)
来源：http://yzu.xylfe.cn

[U91] JS：对象键值遍历
来源：http://kge.yangfankeji.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iep.ywan-chungtsiang.top

[U92] JS：深拷贝
来源：http://ccx.ydzc1.top

structuredClone(obj)
来源：http://fwi.hnxiangtu.top

[U93] JS：模板字符串
来源：http://sje.yfazqb.com

`共 ${n} 条`
来源：http://xge.yanxiufei.cn

[U94] JS：箭头函数
来源：http://lca.zhixingplan.top

const double = x => x * 2;
来源：http://tfq.yj20258888.top

[U95] JS：Promise 包装
来源：http://ovm.daxiang520.top

new Promise((resolve, reject) => {})
来源：http://mgg.meibo888.top

[U96] JS：async/await 与异常
来源：http://rsu.zhixingplan.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rqq.andypj.xyz

[U97] JS：并发请求
来源：http://lmq.hcnkem.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://lvh.hesvh.cn

[U98] JS：fetch 带 JSON
来源：http://ekw.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ico.tarul.cn

[U99] JS：事件监听
来源：http://hdc.havefunace.top

el.addEventListener("click", e => {})
来源：http://fqb.xuanzx.com

[U100] JS：DOM 查询
来源：http://ydk.ywan-chungtsiang.top

document.querySelector(".item")
来源：http://lal.yj20258.top

[U101] JS：classList 操作
来源：http://atb.xinyue.icu

el.classList.toggle("active")
来源：http://ojr.smart0.xyz

[U102] JS：本地存储
来源：http://nko.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fnn.shanyushiyangkeji.top

[U103] JS：定时器
来源：http://lxl.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tcp.zdqjudy.top

[U104] JS：防抖
来源：http://uud.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gee.tarul.cn

[U105] JS：节流
来源：http://tiq.hesvh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rbm.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://ujw.kuanghao11.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dxm.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://sqx.zhijiandao.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tad.guowangkeji.top

[U108] JS：随机整数
来源：http://wtt.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://owj.aibaodan.cn

[U109] JS：数组分组
来源：http://ifz.jinyuanbaomall.cn

Object.groupBy(arr, x => x.type)
来源：http://hmy.jinghuilouyu.cn

[U110] JS：数组分块
来源：http://pqx.smart0.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mpm.dashuyun.cn

[U111] JS：对象转 Map
来源：http://omy.iojbl.cn

new Map(Object.entries(obj))
来源：http://bef.uphjek.com

[U112] JS：字符串补位
来源：http://ine.hcnkem.com

"7".padStart(3, "0")
来源：http://nff.pycfn.com

[U113] JS：正则替换全部
来源：http://wew.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://lha.yonumen.top

[U114] JS：JSON 深比较
来源：http://vol.jqgufenzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dlh.snrcjt.cn

[U115] JS：生成 UUID
来源：http://xpd.andypj.xyz

crypto.randomUUID()
来源：http://cct.shangyingyoupin.top

[U116] JS：类型检查（JSDoc）
来源：http://zsj.shuidangran.top

/** @param {string} name */ function f(name) {}
来源：http://aqk.c1oappe.top

[U117] JS：单元测试
来源：http://rgp.sweek.top

npm i -D vitest;  npx vitest
来源：http://jvp.zhiwuduotai.top

[U118] JS：开发服务器
来源：http://gdr.vehdjk.com

npm i -D vite;  npx vite
来源：http://zmv.yj202588.top

[U119] JS：生产构建
来源：http://azn.jiagoushi.top

npx vite build
来源：http://suh.daxiang520.top

[U120] JS：读取环境变量（Vite）
来源：http://zwh.tian-w.cn

import.meta.env.VITE_API_URL
来源：http://wrm.jinqigufen.top

================================================================================
来源：http://fhi.yj20258.top

统计汇总
来源：http://lnt.redwolf501.top

================================================================================
来源：http://fvv.ydzc1.top

按语言统计（条）：
来源：http://hrw.52xcode.cn

Python ......... 252
来源：http://cvz.jqgfzy.top

PHP ............ 252
来源：http://fkf.jqgfzy.top

JavaScript ..... 252
来源：http://tnz.ywan-chungtsiang.top

TypeScript ..... 212
来源：http://sua.gotoacloud.top

Java ........... 212
来源：http://wgn.andypj.xyz

Go ............. 212
来源：http://yom.smart0.xyz

Ruby ........... 212
来源：http://vjr.xuanzx.com

C# ............. 212
来源：http://jlv.iojbl.cn

C .............. 30
来源：http://vzp.fktsv.cn

C++ ............ 30
来源：http://pan.hywenlv.cn

SQL ............ 90
来源：http://cyp.hnqzz.top

Bash ........... 80
来源：http://kze.yongpay.top

Kotlin ......... 15
来源：http://abs.sjlbkw.cn

Swift .......... 15
来源：http://ulx.gzhubu.top

Lua ............ 10
来源：http://mrp.meibo888.top

Perl ........... 10
来源：http://eeh.zycfv.cn

Scala .......... 10
来源：http://rks.yangfankeji.com

------------------------------------
来源：http://rep.redwolf501.top

合计 ........... 2106 条
来源：http://npx.gaohongyu789.top

按章节统计：
来源：http://dgk.fktsv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pnv.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xcy.jqgufenzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hxy.hongshengwenyu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hvc.quarkkingdee.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ycn.wangdashe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nql.aizwys.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ufb.zhixingplan.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://esq.jlsjyb.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vxq.ydjk.org.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qeh.cdnleiting.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qcd.havefunace.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://asl.yongpay.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dfg.zhaomingkeji.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dyw.ydjk.org.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kzb.52xcode.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sww.guannengcc.top

Q SQL 专题                              90
来源：http://skp.yj202588.top

R Bash 专题                             80
来源：http://jif.cheryme.top

S C / C++ 专题                          60
来源：http://nta.yuxming.cn

T 其他语言补充                          60
来源：http://aof.smart0.xyz

U 高频实用片段                         120
来源：http://grp.9152youxi.cn

------------------------------------
来源：http://lvh.hcnkem.com

合计                                  2106 条
来源：http://ffd.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://soj.cqqwz.cn

使用提醒
来源：http://yhm.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://wrx.jinyuanbaomall.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jvw.tanke756.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rdh.dashuyun.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nsf.gzhubu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://khu.jinqigfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aqj.9152youxi.cn

—— 文件结束 ——
来源：http://gvk.cucudq.cn

================================================================================
来源：http://nmy.andypj.xyz

程序语言常见例子速查手册（2024 版）
来源：http://ygy.hcnkem.com

Common Programming Examples Cheat Book
来源：http://llu.0kj1m.cn

================================================================================
来源：http://xnh.chenzaomai.com

【收录内容】
来源：http://dkh.hysaishi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://whu.0kj1m.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mhw.yuxming.cn

SQL · Bash · C · C++
来源：http://pfu.xuanzx.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cxk.epnwcf.com

【使用说明】
来源：http://kse.pycfn.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wgg.hongshengwenyu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xsv.hywenlv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qvz.hnxiangtu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hxr.chenlongwang.top

Bash:  Shell         C:     C             C++:   C++
来源：http://xat.nanxinkj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pna.tanke756.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wie.ppjwa.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://skz.havefunace.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://msq.fktsv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fxz.nwbrower.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kvn.zdqjudy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kym.gzhubu.top

【文件统计】
来源：http://dyh.smart0.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vwe.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://pes.dianchejie.cn

目  录
来源：http://vaw.yj202588.top

--------------------------------------------------------------------------------
来源：http://nzd.ctjpmb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qkq.mhx1999.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xyy.sweek.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hwk.chenlongwang.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ytn.sysykeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xth.yueranfly.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://idv.vqdsnc.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yyb.bjfxy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qbm.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fzn.hywenlv.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pzi.snrcjt.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pnk.fehbvm.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jyg.jianghu66.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ogp.zdqjudy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cfn.wangdashe.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mbd.wangshuangyany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gyk.jinqigfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://alz.dianchejie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vee.hammf.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fwv.0kj1m.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yyb.zhaomingkeji.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mjk.hnxiangtu.top

================================================================================
来源：http://tip.ivvv.top

A. 基础语法与类型
来源：http://tda.cucudq.cn

================================================================================
来源：http://ypz.birdmap.top

[A01] Hello World
来源：http://xjx.zycfv.cn

Py:   print("Hello, World!")
来源：http://jvt.jinghuilouyu.cn

PHP:  echo "Hello, World!";
来源：http://dtg.vehdjk.com

JS:   console.log("Hello, World!");
来源：http://ouj.bjfxy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hoc.tanke756.top

Java: System.out.println("Hello, World!");
来源：http://hta.cashguo.top

Go:   fmt.Println("Hello, World!")
来源：http://vjs.yvedp.cn

Ruby: puts "Hello, World!"
来源：http://pot.daria6918.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dwi.svipenyu.cn

[A02] 变量声明与赋值
来源：http://pcs.vqdsnc.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mhb.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://drr.yuxming.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ioj.zhijiandao.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lqi.hcnkem.com

Java: String name = "Alex"; int age = 20;
来源：http://ikg.52xcode.cn

Go:   name := "Alex"; age := 20
来源：http://swl.cqqwz.cn

Ruby: name = "Alex"; age = 20
来源：http://flo.cqqwz.cn


<!-- 参考信息 -->