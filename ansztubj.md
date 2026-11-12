代发 wailian999

[U51] PHP：数组解构
来源：http://rmx.tianlin.xyz

[$a, $b] = $arr;
来源：http://hnk.dashuyun.cn

[U52] PHP：箭头函数
来源：http://sdb.jinyuanbaomall.cn

$double = fn($x) => $x * 2;
来源：http://nco.hnxiangtu.top

[U53] PHP：空合并运算符
来源：http://wbs.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://uhl.yj20258888.top

[U54] PHP：空安全调用
来源：http://gcs.zhijiandao.cn

$obj?->method()
来源：http://xlx.ivvv.top

[U55] PHP：match 表达式
来源：http://qjj.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eyy.zdbjq.cn

[U56] PHP：命名参数
来源：http://kas.aibaodan.cn

f(a: 1, b: 2)
来源：http://kim.sjlbkw.cn

[U57] PHP：字符串插值
来源：http://gjj.hnqzz.top

"值: {$a}"
来源：http://exc.nwbrower.top

[U58] PHP：数组三件套
来源：http://sji.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://clz.jinyuanbaomall.cn

[U59] PHP：自定义排序
来源：http://eme.aizwys.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lto.52xcode.cn

[U60] PHP：JSON 编解码
来源：http://ryq.ivvv.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bda.hfpthk.cn

[U61] PHP：正则
来源：http://tcq.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wfs.andypj.xyz

[U62] PHP：日期对象
来源：http://fqy.dashuyun.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nog.svipenyu.cn

[U63] PHP：文件读写
来源：http://nkj.sjlbkw.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://prb.xinyue.icu

[U64] PHP：目录遍历
来源：http://pvi.ydzc1.top

glob("dir/*.php");  scandir("dir");
来源：http://gsg.xuanzx.com

[U65] PHP：会话
来源：http://bms.guannengcc.top

session_start();  $_SESSION["uid"] = 1;
来源：http://chf.nanxuanxn.top

[U66] PHP：设置 Cookie
来源：http://emg.dianchejie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mni.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://amd.jianghu66.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ttm.hammf.cn

[U68] PHP：PDO 连接
来源：http://qlb.jyoumei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://usl.ywan-chungtsiang.top

[U69] PHP：PDO 预处理
来源：http://vca.hnqzz.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eme.redwolf501.top

[U70] PHP：PDO 事务
来源：http://aoq.zhoulong.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gau.ydzc1.top

[U71] PHP：抛出异常
来源：http://ldi.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://crg.fanxiaobao.xyz

[U72] PHP：写错误日志
来源：http://vuh.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://nmd.sweek.top

[U73] PHP：读取 ini 配置
来源：http://ium.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://shr.shanyushiyangkeji.top

[U74] PHP：读取环境变量
来源：http://bpu.tanke756.top

getenv("APP_ENV") ?: "production"
来源：http://qbu.nanxinkj.top

[U75] PHP：依赖注入
来源：http://cln.zhixingplan.top

composer require psr/container
来源：http://ciy.dianchejie.cn

[U76] PHP：简单路由
来源：http://hzt.hnqzz.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://puv.yanxiufei.cn

[U77] PHP：模板渲染
来源：http://vwa.ehwqpu.com

composer require twig/twig
来源：http://uwy.xziqi.cn

[U78] PHP：单元测试
来源：http://dra.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://lcl.jiagoushi.top

[U79] PHP：静态分析
来源：http://vmf.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://fsz.aibaodan.cn

[U80] PHP：代码规范修复
来源：http://kks.pengpengdd.cyou

composer require --dev friendsofphp/php-cs-fixer
来源：http://ddx.xuetiantiany.cn

[U81] JS：初始化项目
来源：http://oat.zhoulong.xyz

npm init -y;  npm i express
来源：http://bhv.shuidangran.top

[U82] JS：package.json 脚本
来源：http://txt.chenjidiqi.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://abi.fanxiaobao.xyz

[U83] JS：ES Module 导入导出
来源：http://cqn.tarul.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hum.bjfxy.top

[U84] JS：CommonJS 写法
来源：http://plr.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://lyn.zhixingplan.top

[U85] JS：可选链
来源：http://nmp.fehbvm.com

a?.b?.c
来源：http://jsq.gogol.net.cn

[U86] JS：空值合并
来源：http://css.0kj1m.cn

a ?? b
来源：http://kzw.yuxming.cn

[U87] JS：解构默认值
来源：http://sft.chenzaomai.com

const { a = 1, b = 2 } = obj;
来源：http://glk.fanxiaobao.xyz

[U88] JS：对象展开合并
来源：http://jfo.sufxvd.cn

{ ...a, ...b }
来源：http://ljv.epnwcf.com

[U89] JS：数组去重
来源：http://hzc.gogol.net.cn

[...new Set(arr)]
来源：http://sgk.yj202588.top

[U90] JS：数字数组排序
来源：http://qgj.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://mfi.jinghuilouyu.cn

[U91] JS：对象键值遍历
来源：http://cmw.xinyue.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mte.yueranfly.top

[U92] JS：深拷贝
来源：http://avf.ivvv.top

structuredClone(obj)
来源：http://oux.haohaochexian.top

[U93] JS：模板字符串
来源：http://zuq.ivvv.top

`共 ${n} 条`
来源：http://tdu.snrcjt.cn

[U94] JS：箭头函数
来源：http://yag.shanyushiyangtech.top

const double = x => x * 2;
来源：http://eiu.cucudq.cn

[U95] JS：Promise 包装
来源：http://yqr.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://ltx.dashuyun.cn

[U96] JS：async/await 与异常
来源：http://wmf.yangfankeji.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jbg.0kj1m.cn

[U97] JS：并发请求
来源：http://thy.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://msx.dianchejie.cn

[U98] JS：fetch 带 JSON
来源：http://sei.aibaodan.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://djs.xuanzx.com

[U99] JS：事件监听
来源：http://xio.shanyushiyangtech.top

el.addEventListener("click", e => {})
来源：http://vkk.bbcook.cn

[U100] JS：DOM 查询
来源：http://wub.cdnleiting.top

document.querySelector(".item")
来源：http://fkt.hnxiangtu.top

[U101] JS：classList 操作
来源：http://tcx.316326.xyz

el.classList.toggle("active")
来源：http://wwv.guannengcc.top

[U102] JS：本地存储
来源：http://plk.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://iqk.tarul.cn

[U103] JS：定时器
来源：http://rkm.tian-w.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yti.nanxuanxn.top

[U104] JS：防抖
来源：http://uwg.pycfn.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ehc.chenjidiqi.icu

[U105] JS：节流
来源：http://teq.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yst.zdqjudy.top

[U106] JS：日期格式化
来源：http://obx.hfpthk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hvi.sysykeji.top

[U107] JS：数字千分位
来源：http://xmg.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ytk.uphjek.com

[U108] JS：随机整数
来源：http://gqp.svipenyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nbj.zhiwuduotai.top

[U109] JS：数组分组
来源：http://ljm.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://lft.hfpthk.cn

[U110] JS：数组分块
来源：http://yil.chenjidiqi.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://boy.jinqigfzy.top

[U111] JS：对象转 Map
来源：http://jgx.gotoacloud.top

new Map(Object.entries(obj))
来源：http://jbt.yongpay.top

[U112] JS：字符串补位
来源：http://aey.zhiwuduotai.top

"7".padStart(3, "0")
来源：http://zat.wangdashe.top

[U113] JS：正则替换全部
来源：http://nfo.haohaochexian.top

s.replaceAll("a", "b")
来源：http://efw.nanxinkj.top

[U114] JS：JSON 深比较
来源：http://jwj.yuanzhike.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://reo.shangyingyoupin.top

[U115] JS：生成 UUID
来源：http://hmy.ivvv.top

crypto.randomUUID()
来源：http://ujl.shangyingyoupin.top

[U116] JS：类型检查（JSDoc）
来源：http://ngq.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://szg.andypj.xyz

[U117] JS：单元测试
来源：http://tvb.sjlbkw.cn

npm i -D vitest;  npx vitest
来源：http://qaw.gzhubu.top

[U118] JS：开发服务器
来源：http://qvy.ehwqpu.com

npm i -D vite;  npx vite
来源：http://plu.ctjpmb.com

[U119] JS：生产构建
来源：http://roq.sweek.top

npx vite build
来源：http://vmq.jinghuilouyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://fll.ppjwa.cn

import.meta.env.VITE_API_URL
来源：http://fzp.snrcjt.cn

================================================================================
来源：http://dte.nanxinkj.top

统计汇总
来源：http://ocy.jiagoushi.top

================================================================================
来源：http://mch.jqgufenzy.top

按语言统计（条）：
来源：http://wng.tian-w.cn

Python ......... 252
来源：http://usd.yfazqb.com

PHP ............ 252
来源：http://sha.shanyushiyangkeji.top

JavaScript ..... 252
来源：http://zox.shzxlz.cn

TypeScript ..... 212
来源：http://oba.316326.xyz

Java ........... 212
来源：http://adi.hcnkem.com

Go ............. 212
来源：http://vdo.yj20258888.top

Ruby ........... 212
来源：http://cib.redwolf501.top

C# ............. 212
来源：http://fgf.bbcook.cn

C .............. 30
来源：http://qry.zdqjudy.top

C++ ............ 30
来源：http://cfb.mhx1999.top

SQL ............ 90
来源：http://naf.ydzc1.top

Bash ........... 80
来源：http://yuw.haohaochexian.top

Kotlin ......... 15
来源：http://emd.zdbjq.cn

Swift .......... 15
来源：http://pbj.cucudq.cn

Lua ............ 10
来源：http://lbk.uphjek.com

Perl ........... 10
来源：http://blf.nanxuanxn.top

Scala .......... 10
来源：http://oxd.andypj.xyz

------------------------------------
来源：http://wkl.hcnkem.com

合计 ........... 2106 条
来源：http://mxp.ivvv.top

按章节统计：
来源：http://iwl.xingfuxueyuan.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wpv.cdnleiting.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jku.zhijiandao.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tbl.zhaomingkeji.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jol.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://amq.jinyuanbaomall.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oap.redwolf501.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zkm.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zew.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ver.yangfankeji.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fpp.xuanzx.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://orl.dianchejie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wew.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mii.aizwys.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ymk.zdbjq.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dzq.yj202588.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://giw.fktsv.cn

Q SQL 专题                              90
来源：http://nro.gzhubu.top

R Bash 专题                             80
来源：http://tgn.zhoulong.xyz

S C / C++ 专题                          60
来源：http://rdl.yueranfly.top

T 其他语言补充                          60
来源：http://chs.fehbvm.com

U 高频实用片段                         120
来源：http://uza.shangyingyoupin.top

------------------------------------
来源：http://dtd.daria6918.cn

合计                                  2106 条
来源：http://pii.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://duh.pycfn.com

使用提醒
来源：http://oij.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://teb.yj202588.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kpu.haohaochexian.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wfn.vehdjk.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://olk.pycfn.com

在旧版本上使用前请先确认语法支持情况。
来源：http://sua.jqgufenzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cms.haohaochexian.top

—— 文件结束 ——
来源：http://awu.sufxvd.cn

================================================================================
来源：http://igm.zhoulong.xyz

程序语言常见例子速查手册（2024 版）
来源：http://jtp.aibaodan.cn

Common Programming Examples Cheat Book
来源：http://kip.daria6918.cn

================================================================================
来源：http://nca.nanxinkj.top

【收录内容】
来源：http://fxj.zhongyouzk.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://qtq.vehdjk.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bks.yueranfly.top

SQL · Bash · C · C++
来源：http://bjt.tarul.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mup.xylfe.cn

【使用说明】
来源：http://dxu.yonumen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zgj.yj202588.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://swg.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gln.yangfankeji.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pdd.fengsongda.top

Bash:  Shell         C:     C             C++:   C++
来源：http://cqx.havefunace.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zub.cheryme.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pin.sxryk.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tia.hcnkem.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fky.redwolf501.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bvs.zhixingplan.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yts.jinqigfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://waa.jyoumei.cn

【文件统计】
来源：http://ztt.tanke756.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ikt.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://tnq.yanxiufei.cn

目  录
来源：http://jjk.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://hrz.dianchejie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cyf.tanke756.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vqx.9152youxi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sgz.fzhhl.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ltb.dianchejie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lks.shanyushiyangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://osc.sxryk.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xfc.tanke756.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pbg.yonumen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zpa.hammf.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ges.tanke756.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://itn.wangshuangyany.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hpv.hcnkem.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sbf.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://caz.zdqjudy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vuc.9152youxi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zwv.gotoacloud.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rgb.meibo888.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://lnd.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ekz.yvedp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ofx.xuanzx.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xka.daria6918.cn

================================================================================
来源：http://cks.redwolf501.top

A. 基础语法与类型
来源：http://drj.yueranfly.top

================================================================================
来源：http://edw.jinqigufen.top

[A01] Hello World
来源：http://ffz.316326.xyz

Py:   print("Hello, World!")
来源：http://vyb.nanxuanxn.top

PHP:  echo "Hello, World!";
来源：http://swg.quarkkingdee.top

JS:   console.log("Hello, World!");
来源：http://arq.nanxuanxn.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ugl.gogol.net.cn

Java: System.out.println("Hello, World!");
来源：http://ivb.dianchejie.cn

Go:   fmt.Println("Hello, World!")
来源：http://jxo.jiagoushi.top

Ruby: puts "Hello, World!"
来源：http://yfc.fehbvm.com

C#:   Console.WriteLine("Hello, World!");
来源：http://llx.hongshengwenyu.top

[A02] 变量声明与赋值
来源：http://jii.zhaomingkeji.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mfn.xinyue.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://bwm.sysykeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://klq.chenlongwang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gjl.guannengcc.top

Java: String name = "Alex"; int age = 20;
来源：http://lvc.ydzc1.top

Go:   name := "Alex"; age := 20
来源：http://uma.chenjidiqi.icu

Ruby: name = "Alex"; age = 20
来源：http://mch.bbcook.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vic.meibo888.top

[A03] 常量定义
来源：http://kee.jinqigfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vmq.ppjwa.cn

PHP:  const PI = 3.14159;
来源：http://cmv.andypj.xyz

JS:   const PI = 3.14159;
来源：http://jiw.svipenyu.cn

TS:   const PI: number = 3.14159;
来源：http://cie.daxiang520.top

Java: static final double PI = 3.14159;
来源：http://ssd.jianghu66.top

Go:   const PI = 3.14159
来源：http://hzo.fanxiaobao.xyz

Ruby: PI = 3.14159
来源：http://luv.wangshuangyany.cn

C#:   const double PI = 3.14159;
来源：http://tdh.hywenlv.cn

[A04] 判断变量类型
来源：http://ael.haohaochexian.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://kbo.sxryk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jox.uphjek.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rad.redwolf501.top

TS:   typeof x; x instanceof Date
来源：http://utf.zycfv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wip.pengpengdd.cyou

Go:   reflect.TypeOf(x).Name()
来源：http://phk.fengsongda.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jbm.kuanghao11.cn

C#:   x.GetType().Name; x is int
来源：http://aya.shuidangran.top

[A05] 整数除法与取模
来源：http://zey.tianlin.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ebj.yanxiufei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rjw.zhaomingkeji.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yhk.bbcook.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ucf.c1oappe.top

Java: 7 / 2; 7 % 2
来源：http://xnp.haohaochexian.top

Go:   7 / 2; 7 % 2
来源：http://pkm.ehwqpu.com

Ruby: 7 / 2; 7 % 2
来源：http://ujl.yj202588.top

C#:   7 / 2; 7 % 2
来源：http://vea.cashguo.top

[A06] 字符串转数字
来源：http://bwe.fanxiaobao.xyz

Py:   int("42"); float("3.14")
来源：http://gfq.sweek.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fzq.jinyuanbaomall.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ksc.cucudq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ujt.andypj.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ldo.gaohongyu789.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ota.hfpthk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://nml.sufxvd.cn


<!-- 参考信息 -->