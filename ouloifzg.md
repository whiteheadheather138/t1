代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://ycr.cashguo.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yca.xylfe.cn

[U42] PHP：PSR-4 自动加载
来源：http://rhp.dianchejie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pif.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://tbp.nwbrower.top

namespace App\Http;
来源：http://xnp.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://jca.cqqwz.cn

declare(strict_types=1);
来源：http://zyi.smart0.xyz

[U45] PHP：类型声明与返回类型
来源：http://lat.iojbl.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cah.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://jzg.birdmap.top

?string $name = null
来源：http://ros.zdbjq.cn

[U47] PHP：联合类型
来源：http://kso.yongpay.top

int|string $id
来源：http://sap.tianlin.xyz

[U48] PHP：纯枚举
来源：http://jlp.aibaodan.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wyb.hysaishi.cn

[U49] PHP：只读属性
来源：http://wbw.svipenyu.cn

public readonly string $name
来源：http://yzb.yj202588.top

[U50] PHP：构造器属性提升
来源：http://qtl.snrcjt.cn

public function __construct(private int $id) {}
来源：http://dtl.zhixingplan.top

[U51] PHP：数组解构
来源：http://evi.ydjk.org.cn

[$a, $b] = $arr;
来源：http://ili.zhixingplan.top

[U52] PHP：箭头函数
来源：http://wny.vehdjk.com

$double = fn($x) => $x * 2;
来源：http://unz.bjfxy.top

[U53] PHP：空合并运算符
来源：http://oqe.jqgfzy.top

$v = $a ?? $b ?? "default";
来源：http://abm.birdmap.top

[U54] PHP：空安全调用
来源：http://idc.yuanzhike.top

$obj?->method()
来源：http://obi.daxiang520.top

[U55] PHP：match 表达式
来源：http://bss.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://frb.gaohongyu789.top

[U56] PHP：命名参数
来源：http://jdq.tian-w.cn

f(a: 1, b: 2)
来源：http://ywk.cdnleiting.top

[U57] PHP：字符串插值
来源：http://wgq.shuidangran.top

"值: {$a}"
来源：http://bnd.jiagoushi.top

[U58] PHP：数组三件套
来源：http://pqh.zhiwuduotai.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://diw.feifeiyinyue.top

[U59] PHP：自定义排序
来源：http://rnv.zhengqikj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oet.tarul.cn

[U60] PHP：JSON 编解码
来源：http://gsa.zhixingplan.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hyp.xuetiantiany.cn

[U61] PHP：正则
来源：http://pcf.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://aaz.cqqwz.cn

[U62] PHP：日期对象
来源：http://uza.tanke756.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gre.shzxlz.cn

[U63] PHP：文件读写
来源：http://oyd.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://peg.fzhhl.top

[U64] PHP：目录遍历
来源：http://gqy.zhoulong.xyz

glob("dir/*.php");  scandir("dir");
来源：http://qhl.xylfe.cn

[U65] PHP：会话
来源：http://jqa.zhengqikj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ddt.yuxming.cn

[U66] PHP：设置 Cookie
来源：http://yyb.tarul.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dno.hywenlv.cn

[U67] PHP：处理文件上传
来源：http://fvj.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://itv.fktsv.cn

[U68] PHP：PDO 连接
来源：http://zig.hfpthk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ymm.yonumen.top

[U69] PHP：PDO 预处理
来源：http://cma.tian-w.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nds.jlsjyb.cn

[U70] PHP：PDO 事务
来源：http://bgx.gogol.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yci.0kj1m.cn

[U71] PHP：抛出异常
来源：http://jwe.gzhubu.top

throw new RuntimeException("失败", 500);
来源：http://kep.nanxinkj.top

[U72] PHP：写错误日志
来源：http://rvu.gotoacloud.top

error_log("失败: " . $e->getMessage());
来源：http://pjd.jinqigufen.top

[U73] PHP：读取 ini 配置
来源：http://fjw.guowangkeji.top

parse_ini_file("config.ini", true)
来源：http://fsp.hysaishi.cn

[U74] PHP：读取环境变量
来源：http://ffm.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://vdj.fanxiaobao.xyz

[U75] PHP：依赖注入
来源：http://czz.fengsongda.top

composer require psr/container
来源：http://nlf.vehdjk.com

[U76] PHP：简单路由
来源：http://ltu.zdqjudy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bmm.sjlbkw.cn

[U77] PHP：模板渲染
来源：http://nxj.jinqigufen.top

composer require twig/twig
来源：http://ccp.52xcode.cn

[U78] PHP：单元测试
来源：http://qkf.gogol.net.cn

composer require --dev phpunit/phpunit
来源：http://lwm.bjfxy.top

[U79] PHP：静态分析
来源：http://wzu.yueranfly.top

composer require --dev phpstan/phpstan
来源：http://xsj.yonumen.top

[U80] PHP：代码规范修复
来源：http://mms.chenzaomai.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://qmi.bjfxy.top

[U81] JS：初始化项目
来源：http://ytx.yangfankeji.com

npm init -y;  npm i express
来源：http://mjc.guowangkeji.top

[U82] JS：package.json 脚本
来源：http://njz.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yui.ehwqpu.com

[U83] JS：ES Module 导入导出
来源：http://xkm.dashuyun.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bvv.xziqi.cn

[U84] JS：CommonJS 写法
来源：http://uni.jinqigufen.top

module.exports = { a };  const { a } = require("./m");
来源：http://pmb.jianghu66.top

[U85] JS：可选链
来源：http://ljd.yj20258888.top

a?.b?.c
来源：http://wfa.ywan-chungtsiang.top

[U86] JS：空值合并
来源：http://pcp.nanxinkj.top

a ?? b
来源：http://igw.bjfxy.top

[U87] JS：解构默认值
来源：http://wig.nanxinkj.top

const { a = 1, b = 2 } = obj;
来源：http://uhz.haohaochexian.top

[U88] JS：对象展开合并
来源：http://dxf.yanxiufei.cn

{ ...a, ...b }
来源：http://efd.sjlbkw.cn

[U89] JS：数组去重
来源：http://ieg.chenlongwang.top

[...new Set(arr)]
来源：http://ypz.yvedp.cn

[U90] JS：数字数组排序
来源：http://hsf.xziqi.cn

[...arr].sort((a, b) => a - b)
来源：http://zbp.hongshengwenyu.top

[U91] JS：对象键值遍历
来源：http://zxt.gzhubu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mcn.tanke756.top

[U92] JS：深拷贝
来源：http://eno.cucudq.cn

structuredClone(obj)
来源：http://poa.shuidangran.top

[U93] JS：模板字符串
来源：http://eru.smart0.xyz

`共 ${n} 条`
来源：http://qll.wangdashe.top

[U94] JS：箭头函数
来源：http://yox.zhiwuduotai.top

const double = x => x * 2;
来源：http://xpt.zhengqikj.top

[U95] JS：Promise 包装
来源：http://bpg.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://vkb.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://kzu.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lbq.smart0.xyz

[U97] JS：并发请求
来源：http://abh.jianghu66.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://wvt.c1oappe.top

[U98] JS：fetch 带 JSON
来源：http://cal.zhixingplan.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nvm.wangshuangyany.cn

[U99] JS：事件监听
来源：http://grm.jiagoushi.top

el.addEventListener("click", e => {})
来源：http://ona.dashuyun.cn

[U100] JS：DOM 查询
来源：http://bdl.gaohongyu789.top

document.querySelector(".item")
来源：http://mpy.cheryme.top

[U101] JS：classList 操作
来源：http://gcs.tarul.cn

el.classList.toggle("active")
来源：http://ybj.haohaochexian.top

[U102] JS：本地存储
来源：http://bzf.dashuyun.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://anm.jqgufenzy.top

[U103] JS：定时器
来源：http://vou.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vhu.ppjwa.cn

[U104] JS：防抖
来源：http://mbl.zhaomingkeji.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qak.yanxiufei.cn

[U105] JS：节流
来源：http://cml.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lzt.kuanghao11.cn

[U106] JS：日期格式化
来源：http://gph.sweek.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rao.shangyingyoupin.top

[U107] JS：数字千分位
来源：http://tjj.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xrg.daria6918.cn

[U108] JS：随机整数
来源：http://jzt.wangdashe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xlo.andypj.xyz

[U109] JS：数组分组
来源：http://ced.hysaishi.cn

Object.groupBy(arr, x => x.type)
来源：http://spm.gogol.net.cn

[U110] JS：数组分块
来源：http://fun.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qgi.guowangkeji.top

[U111] JS：对象转 Map
来源：http://dkm.yj20258.top

new Map(Object.entries(obj))
来源：http://iky.jinqigufen.top

[U112] JS：字符串补位
来源：http://nda.smart0.xyz

"7".padStart(3, "0")
来源：http://nmk.chenjidiqi.icu

[U113] JS：正则替换全部
来源：http://avw.yanxiufei.cn

s.replaceAll("a", "b")
来源：http://bor.shangyingyoupin.top

[U114] JS：JSON 深比较
来源：http://yuy.zhoulong.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://etm.redwolf501.top

[U115] JS：生成 UUID
来源：http://ddd.9152youxi.cn

crypto.randomUUID()
来源：http://auw.tarul.cn

[U116] JS：类型检查（JSDoc）
来源：http://oui.yvedp.cn

/** @param {string} name */ function f(name) {}
来源：http://qby.ydjk.org.cn

[U117] JS：单元测试
来源：http://riq.tian-w.cn

npm i -D vitest;  npx vitest
来源：http://cki.jlsjyb.cn

[U118] JS：开发服务器
来源：http://jbh.zdbjq.cn

npm i -D vite;  npx vite
来源：http://qoa.uphjek.com

[U119] JS：生产构建
来源：http://vza.zhaomingkeji.xyz

npx vite build
来源：http://grj.bjfxy.top

[U120] JS：读取环境变量（Vite）
来源：http://ffi.gotoacloud.top

import.meta.env.VITE_API_URL
来源：http://lbm.pycfn.com

================================================================================
来源：http://ict.xziqi.cn

统计汇总
来源：http://isr.aizwys.cn

================================================================================
来源：http://qjd.hesvh.cn

按语言统计（条）：
来源：http://czh.fzhhl.top

Python ......... 252
来源：http://svd.zycfv.cn

PHP ............ 252
来源：http://wvq.yj202588.top

JavaScript ..... 252
来源：http://hvc.tian-w.cn

TypeScript ..... 212
来源：http://gxp.hesvh.cn

Java ........... 212
来源：http://qkj.yuanzhike.top

Go ............. 212
来源：http://eyk.pengpengdd.cyou

Ruby ........... 212
来源：http://gbp.ppjwa.cn

C# ............. 212
来源：http://pdq.pengpengdd.cyou

C .............. 30
来源：http://yqb.52xcode.cn

C++ ............ 30
来源：http://fgj.hammf.cn

SQL ............ 90
来源：http://fjb.guannengcc.top

Bash ........... 80
来源：http://gdv.xinyue.icu

Kotlin ......... 15
来源：http://cpm.snrcjt.cn

Swift .......... 15
来源：http://tko.hfpthk.cn

Lua ............ 10
来源：http://lnb.ctjpmb.com

Perl ........... 10
来源：http://kcb.daxiang520.top

Scala .......... 10
来源：http://dzm.vehdjk.com

------------------------------------
来源：http://auj.gogol.net.cn

合计 ........... 2106 条
来源：http://qpl.uphjek.com

按章节统计：
来源：http://dsa.hnqzz.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rxo.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rig.shuidangran.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eha.yj20258.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zmh.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hqq.jyoumei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eyf.vqdsnc.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xbx.iojbl.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mtx.dianchejie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://voq.gzhubu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pby.jiagoushi.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fzu.mhx1999.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://avs.fehbvm.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qpl.yuxming.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://odl.fehbvm.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hwt.quarkkingdee.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fdx.hammf.cn

Q SQL 专题                              90
来源：http://cia.cucudq.cn

R Bash 专题                             80
来源：http://xzg.sweek.top

S C / C++ 专题                          60
来源：http://xgd.shanyushiyangtech.top

T 其他语言补充                          60
来源：http://shk.bjfxy.top

U 高频实用片段                         120
来源：http://blh.aibaodan.cn

------------------------------------
来源：http://gmv.svipenyu.cn

合计                                  2106 条
来源：http://bjb.52xcode.cn

--------------------------------------------------------------------------------
来源：http://ghf.bjfxy.top

使用提醒
来源：http://vcu.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://vbe.wangdashe.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bvn.gogol.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qys.meibo888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rxk.svipenyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xza.pengpengdd.cyou

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://byj.yonumen.top

—— 文件结束 ——
来源：http://znk.ppjwa.cn

================================================================================
来源：http://jbw.yuanzhike.top

程序语言常见例子速查手册（2024 版）
来源：http://mml.yueranfly.top

Common Programming Examples Cheat Book
来源：http://zfh.fehbvm.com

================================================================================
来源：http://pkw.svipenyu.cn

【收录内容】
来源：http://hqm.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://bns.jqgfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nhr.ivvv.top

SQL · Bash · C · C++
来源：http://kpe.nanxuanxn.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://krf.gotoacloud.top

【使用说明】
来源：http://pxo.fehbvm.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mnw.cashguo.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gkz.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yni.meibo888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kwa.hcnkem.com

Bash:  Shell         C:     C             C++:   C++
来源：http://tqk.xuetiantiany.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://olo.hfpthk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://caw.gzhubu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hxm.ehwqpu.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jhq.yuanzhike.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xrr.xinyue.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ioc.smart0.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iya.tianlin.xyz

【文件统计】
来源：http://bbw.hysaishi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gcz.daria6918.cn

--------------------------------------------------------------------------------
来源：http://niu.pengpengdd.cyou

目  录
来源：http://zjo.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://dgb.daria6918.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xrc.kuanghao11.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gbc.xuetiantiany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zsw.guowangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lfy.fehbvm.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cqm.vehdjk.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eak.bjfxy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://geb.316326.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ggv.guannengcc.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gkm.wangshuangyany.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hce.chenzaomai.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://arv.daria6918.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vaj.xinyue.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lmw.yonumen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vku.yfazqb.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bln.tian-w.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lub.zhiwuduotai.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qle.mhx1999.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://nmd.yuanzhike.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qer.uphjek.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zqt.tian-w.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uwx.ctjpmb.com

================================================================================
来源：http://alc.ppjwa.cn

A. 基础语法与类型
来源：http://qbl.jinqigufen.top

================================================================================
来源：http://uzw.fzhhl.top

[A01] Hello World
来源：http://bwr.yuanzhike.top

Py:   print("Hello, World!")
来源：http://eqp.yangfankeji.com

PHP:  echo "Hello, World!";
来源：http://obi.smart0.xyz

JS:   console.log("Hello, World!");
来源：http://yxj.snrcjt.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uoi.hongshengwenyu.top

Java: System.out.println("Hello, World!");
来源：http://xuo.shuidangran.top

Go:   fmt.Println("Hello, World!")
来源：http://tde.birdmap.top

Ruby: puts "Hello, World!"
来源：http://rzm.ehwqpu.com

C#:   Console.WriteLine("Hello, World!");
来源：http://cng.nanxuanxn.top

[A02] 变量声明与赋值
来源：http://uvn.xziqi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qtf.vqdsnc.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qzg.chenlongwang.top

JS:   let name = "Alex"; const age = 20;
来源：http://ptp.pycfn.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://axi.dashuyun.cn

Java: String name = "Alex"; int age = 20;
来源：http://rnu.guowangkeji.top

Go:   name := "Alex"; age := 20
来源：http://dev.sweek.top

Ruby: name = "Alex"; age = 20
来源：http://bvr.wangshuangyany.cn

C#:   string name = "Alex"; int age = 20;
来源：http://anh.wangdashe.top

[A03] 常量定义
来源：http://jgn.tian-w.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jjv.fehbvm.com

PHP:  const PI = 3.14159;
来源：http://cnf.cheryme.top

JS:   const PI = 3.14159;
来源：http://pnr.hesvh.cn

TS:   const PI: number = 3.14159;
来源：http://tsd.0kj1m.cn

Java: static final double PI = 3.14159;
来源：http://jfp.cdnleiting.top

Go:   const PI = 3.14159
来源：http://bmv.shanyushiyangtech.top

Ruby: PI = 3.14159
来源：http://ihe.zycfv.cn

C#:   const double PI = 3.14159;
来源：http://qac.0kj1m.cn

[A04] 判断变量类型
来源：http://clo.sxryk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://est.ydzc1.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dfk.bjfxy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://goh.vehdjk.com

TS:   typeof x; x instanceof Date
来源：http://hdj.svipenyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ica.zdqjudy.top


<!-- 参考信息 -->