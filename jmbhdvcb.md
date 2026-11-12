代发 wailian999

[U57] PHP：字符串插值
来源：http://bkk.fanxiaobao.xyz

"值: {$a}"
来源：http://dsm.jinyuanbaomall.cn

[U58] PHP：数组三件套
来源：http://xka.svipenyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jbq.redwolf501.top

[U59] PHP：自定义排序
来源：http://kzj.316326.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wjz.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://bzm.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rxq.snrcjt.cn

[U61] PHP：正则
来源：http://ugw.yj20258.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gat.yongpay.top

[U62] PHP：日期对象
来源：http://yid.uphjek.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hic.ivvv.top

[U63] PHP：文件读写
来源：http://fcf.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://buh.zdbjq.cn

[U64] PHP：目录遍历
来源：http://cxc.xylfe.cn

glob("dir/*.php");  scandir("dir");
来源：http://brp.iojbl.cn

[U65] PHP：会话
来源：http://oqm.mhx1999.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nii.cdnleiting.top

[U66] PHP：设置 Cookie
来源：http://uzt.9152youxi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hlu.ydjk.org.cn

[U67] PHP：处理文件上传
来源：http://yjn.yanxiufei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nvw.hongshengwenyu.top

[U68] PHP：PDO 连接
来源：http://qfn.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://grm.ehwqpu.com

[U69] PHP：PDO 预处理
来源：http://apj.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cxf.jyoumei.cn

[U70] PHP：PDO 事务
来源：http://pvf.shuidangran.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://por.zycfv.cn

[U71] PHP：抛出异常
来源：http://ikf.aibaodan.cn

throw new RuntimeException("失败", 500);
来源：http://jwl.hammf.cn

[U72] PHP：写错误日志
来源：http://thm.shangyingyoupin.top

error_log("失败: " . $e->getMessage());
来源：http://bgr.yueranfly.top

[U73] PHP：读取 ini 配置
来源：http://etr.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://ujb.cheryme.top

[U74] PHP：读取环境变量
来源：http://pkt.jinqigfzy.top

getenv("APP_ENV") ?: "production"
来源：http://xhn.shangyingyoupin.top

[U75] PHP：依赖注入
来源：http://rst.shuidangran.top

composer require psr/container
来源：http://tzj.jiagoushi.top

[U76] PHP：简单路由
来源：http://yyw.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yzs.wangshuangyany.cn

[U77] PHP：模板渲染
来源：http://vxs.hfpthk.cn

composer require twig/twig
来源：http://lds.gogol.net.cn

[U78] PHP：单元测试
来源：http://adz.bjfxy.top

composer require --dev phpunit/phpunit
来源：http://btq.yvedp.cn

[U79] PHP：静态分析
来源：http://kor.yvedp.cn

composer require --dev phpstan/phpstan
来源：http://mkd.jinqigfzy.top

[U80] PHP：代码规范修复
来源：http://jpt.daxiang520.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mgr.yj20258888.top

[U81] JS：初始化项目
来源：http://qmz.yueranfly.top

npm init -y;  npm i express
来源：http://lpb.smart0.xyz

[U82] JS：package.json 脚本
来源：http://vbm.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tev.shzxlz.cn

[U83] JS：ES Module 导入导出
来源：http://uso.uphjek.com

export const a = 1;  import { a } from "./m.js";
来源：http://jan.shangyingyoupin.top

[U84] JS：CommonJS 写法
来源：http://bul.chenjidiqi.icu

module.exports = { a };  const { a } = require("./m");
来源：http://wtk.ywan-chungtsiang.top

[U85] JS：可选链
来源：http://rze.cucudq.cn

a?.b?.c
来源：http://gkd.sweek.top

[U86] JS：空值合并
来源：http://jua.hnxiangtu.top

a ?? b
来源：http://hde.haohaochexian.top

[U87] JS：解构默认值
来源：http://act.jqgfzy.top

const { a = 1, b = 2 } = obj;
来源：http://jvo.wangdashe.top

[U88] JS：对象展开合并
来源：http://oaz.pycfn.com

{ ...a, ...b }
来源：http://gjx.uphjek.com

[U89] JS：数组去重
来源：http://ynn.jyoumei.cn

[...new Set(arr)]
来源：http://kqw.kuanghao11.cn

[U90] JS：数字数组排序
来源：http://slz.tianlin.xyz

[...arr].sort((a, b) => a - b)
来源：http://bta.gotoacloud.top

[U91] JS：对象键值遍历
来源：http://zav.gzhubu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sdi.wangdashe.top

[U92] JS：深拷贝
来源：http://aaa.jinyuanbaomall.cn

structuredClone(obj)
来源：http://qbs.hnxiangtu.top

[U93] JS：模板字符串
来源：http://twu.yuxming.cn

`共 ${n} 条`
来源：http://gxv.xziqi.cn

[U94] JS：箭头函数
来源：http://qgq.epnwcf.com

const double = x => x * 2;
来源：http://ngl.jianghu66.top

[U95] JS：Promise 包装
来源：http://oka.meibo888.top

new Promise((resolve, reject) => {})
来源：http://cip.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://dfe.smart0.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://had.tianlin.xyz

[U97] JS：并发请求
来源：http://bhy.xylfe.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://naq.yongpay.top

[U98] JS：fetch 带 JSON
来源：http://isu.aibaodan.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mkb.cashguo.top

[U99] JS：事件监听
来源：http://qpv.xylfe.cn

el.addEventListener("click", e => {})
来源：http://bny.hongshengwenyu.top

[U100] JS：DOM 查询
来源：http://xqn.sysykeji.top

document.querySelector(".item")
来源：http://suy.epnwcf.com

[U101] JS：classList 操作
来源：http://lri.kuanghao11.cn

el.classList.toggle("active")
来源：http://zlp.zdqjudy.top

[U102] JS：本地存储
来源：http://tby.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rxq.meibo888.top

[U103] JS：定时器
来源：http://mhe.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fct.yj20258.top

[U104] JS：防抖
来源：http://byn.sweek.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://say.tian-w.cn

[U105] JS：节流
来源：http://exo.dianchejie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lgv.jlsjyb.cn

[U106] JS：日期格式化
来源：http://nel.jinyuanbaomall.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://llc.snrcjt.cn

[U107] JS：数字千分位
来源：http://vbf.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pzj.gaohongyu789.top

[U108] JS：随机整数
来源：http://szs.zhiwuduotai.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wiv.shangyingyoupin.top

[U109] JS：数组分组
来源：http://bjb.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://fyk.sweek.top

[U110] JS：数组分块
来源：http://ymu.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gzu.ivvv.top

[U111] JS：对象转 Map
来源：http://smr.zycfv.cn

new Map(Object.entries(obj))
来源：http://mgy.mhx1999.top

[U112] JS：字符串补位
来源：http://rgp.hammf.cn

"7".padStart(3, "0")
来源：http://bzu.zhixingplan.top

[U113] JS：正则替换全部
来源：http://qws.hnxiangtu.top

s.replaceAll("a", "b")
来源：http://sdp.yj202588.top

[U114] JS：JSON 深比较
来源：http://slc.andypj.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://gag.meibo888.top

[U115] JS：生成 UUID
来源：http://txc.hongshengwenyu.top

crypto.randomUUID()
来源：http://fgh.hnqzz.top

[U116] JS：类型检查（JSDoc）
来源：http://tvi.shanyushiyangtech.top

/** @param {string} name */ function f(name) {}
来源：http://vea.ppjwa.cn

[U117] JS：单元测试
来源：http://rgg.ydzc1.top

npm i -D vitest;  npx vitest
来源：http://qyt.aizwys.cn

[U118] JS：开发服务器
来源：http://iej.aizwys.cn

npm i -D vite;  npx vite
来源：http://lda.shanyushiyangtech.top

[U119] JS：生产构建
来源：http://rsk.andypj.xyz

npx vite build
来源：http://ikr.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://giz.gaohongyu789.top

import.meta.env.VITE_API_URL
来源：http://tsv.hnqzz.top

================================================================================
来源：http://iom.gogol.net.cn

统计汇总
来源：http://avw.jinqigufen.top

================================================================================
来源：http://vlm.zhiwuduotai.top

按语言统计（条）：
来源：http://ycd.zycfv.cn

Python ......... 252
来源：http://ybv.tanke756.top

PHP ............ 252
来源：http://rad.nwbrower.top

JavaScript ..... 252
来源：http://rnt.hesvh.cn

TypeScript ..... 212
来源：http://kjw.zhiwuduotai.top

Java ........... 212
来源：http://nqw.yonumen.top

Go ............. 212
来源：http://jqf.bjfxy.top

Ruby ........... 212
来源：http://oej.cdnleiting.top

C# ............. 212
来源：http://nph.jqgfzy.top

C .............. 30
来源：http://vtw.yvedp.cn

C++ ............ 30
来源：http://lus.shanyushiyangkeji.top

SQL ............ 90
来源：http://tvc.ywan-chungtsiang.top

Bash ........... 80
来源：http://tme.tian-w.cn

Kotlin ......... 15
来源：http://uxg.shuidangran.top

Swift .......... 15
来源：http://kdv.c1oappe.top

Lua ............ 10
来源：http://anq.zhongyouzk.top

Perl ........... 10
来源：http://tzo.cheryme.top

Scala .......... 10
来源：http://vmd.ydzc1.top

------------------------------------
来源：http://sbi.fengsongda.top

合计 ........... 2106 条
来源：http://gmk.pycfn.com

按章节统计：
来源：http://rrq.zhijiandao.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://txg.yueranfly.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kdx.redwolf501.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kdm.zhixingplan.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aij.sysykeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ink.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kef.wangshuangyany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://niu.yongpay.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ehf.jinqigfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yqs.sweek.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mra.shzxlz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ann.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lbn.daria6918.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kxf.feifeiyinyue.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lmy.hcnkem.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bui.tian-w.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sqz.sxryk.cn

Q SQL 专题                              90
来源：http://usq.yongpay.top

R Bash 专题                             80
来源：http://cna.pengpengdd.cyou

S C / C++ 专题                          60
来源：http://ldd.ybcxt.top

T 其他语言补充                          60
来源：http://ioe.yonumen.top

U 高频实用片段                         120
来源：http://veo.chenlongwang.top

------------------------------------
来源：http://wlg.tianlin.xyz

合计                                  2106 条
来源：http://hdq.vehdjk.com

--------------------------------------------------------------------------------
来源：http://imm.guowangkeji.top

使用提醒
来源：http://dfp.wangdashe.top

--------------------------------------------------------------------------------
来源：http://qtd.uphjek.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zxg.nanxuanxn.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wxk.shuidangran.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ggf.wangshuangyany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ekf.sjlbkw.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ply.yj202588.top

—— 文件结束 ——
来源：http://cjd.jinqigfzy.top

================================================================================
来源：http://vot.yongpay.top

程序语言常见例子速查手册（2024 版）
来源：http://zwg.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://jyl.yfazqb.com

================================================================================
来源：http://qoh.xinyue.icu

【收录内容】
来源：http://thl.tian-w.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yds.yanxiufei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fec.mhx1999.top

SQL · Bash · C · C++
来源：http://qbu.zycfv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xjt.daria6918.cn

【使用说明】
来源：http://eyi.shanyushiyangtech.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dcv.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lub.ppjwa.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://svk.jianghu66.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lhu.jinqigufen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tng.guannengcc.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qtb.sufxvd.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zme.ydzc1.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://iwo.feifeiyinyue.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mht.yj20258888.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mdi.aibaodan.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jwv.fktsv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xdp.yonumen.top

【文件统计】
来源：http://mvj.feifeiyinyue.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://llm.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://uvt.wangshuangyany.cn

目  录
来源：http://dzp.epnwcf.com

--------------------------------------------------------------------------------
来源：http://wtn.zhongyouzk.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ter.jinqigufen.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kqr.svipenyu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gtx.daxiang520.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bdm.jinqigfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vus.shanyushiyangtech.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tdu.xuanzx.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tlb.hnqzz.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rps.gotoacloud.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nxu.fehbvm.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lsm.fehbvm.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ywe.bbcook.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zim.ydzc1.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bhc.svipenyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ypu.cdnleiting.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wdh.zdqjudy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gka.chenlongwang.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://apf.ywan-chungtsiang.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://miv.yj20258888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://saq.yvedp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ybi.quarkkingdee.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jiq.sjlbkw.cn

================================================================================
来源：http://vym.nanxuanxn.top

A. 基础语法与类型
来源：http://slq.hesvh.cn

================================================================================
来源：http://cox.zdqjudy.top

[A01] Hello World
来源：http://xnh.wangdashe.top

Py:   print("Hello, World!")
来源：http://oeg.daxiang520.top

PHP:  echo "Hello, World!";
来源：http://pfp.yueranfly.top

JS:   console.log("Hello, World!");
来源：http://wze.fengsongda.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vdx.vqdsnc.cn

Java: System.out.println("Hello, World!");
来源：http://ayz.shangyingyoupin.top

Go:   fmt.Println("Hello, World!")
来源：http://nzo.yuanzhike.top

Ruby: puts "Hello, World!"
来源：http://yrl.cashguo.top

C#:   Console.WriteLine("Hello, World!");
来源：http://aui.pycfn.com

[A02] 变量声明与赋值
来源：http://itu.yangfankeji.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lvz.redwolf501.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ymr.zhoulong.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://ilw.316326.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oaw.shanyushiyangkeji.top

Java: String name = "Alex"; int age = 20;
来源：http://fvb.chenjidiqi.icu

Go:   name := "Alex"; age := 20
来源：http://pjo.xuanzx.com

Ruby: name = "Alex"; age = 20
来源：http://eqj.jinqigfzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://ynb.chenlongwang.top

[A03] 常量定义
来源：http://icz.andypj.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ixm.cucudq.cn

PHP:  const PI = 3.14159;
来源：http://nap.xylfe.cn

JS:   const PI = 3.14159;
来源：http://cfa.hcnkem.com

TS:   const PI: number = 3.14159;
来源：http://qop.gotoacloud.top

Java: static final double PI = 3.14159;
来源：http://shz.hcnkem.com

Go:   const PI = 3.14159
来源：http://rjd.cdnleiting.top

Ruby: PI = 3.14159
来源：http://ich.bjfxy.top

C#:   const double PI = 3.14159;
来源：http://tct.meibo888.top

[A04] 判断变量类型
来源：http://lga.sufxvd.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mux.ehwqpu.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://goi.yonumen.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xri.9152youxi.cn

TS:   typeof x; x instanceof Date
来源：http://fig.bbcook.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ndr.yj202588.top

Go:   reflect.TypeOf(x).Name()
来源：http://nzk.jinghuilouyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tsv.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://fln.havefunace.top

[A05] 整数除法与取模
来源：http://htf.nanxuanxn.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wey.cdnleiting.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uye.gotoacloud.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://aou.uphjek.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dwn.uphjek.com

Java: 7 / 2; 7 % 2
来源：http://xxs.zhixingplan.top

Go:   7 / 2; 7 % 2
来源：http://jtx.xziqi.cn

Ruby: 7 / 2; 7 % 2
来源：http://uwc.epnwcf.com

C#:   7 / 2; 7 % 2
来源：http://ntx.shanyushiyangkeji.top

[A06] 字符串转数字
来源：http://dzm.tarul.cn

Py:   int("42"); float("3.14")
来源：http://qxo.hfpthk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hql.jlsjyb.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jhy.sysykeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://ivy.fzhhl.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qha.ivvv.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://crg.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rbh.zdbjq.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dms.cdnleiting.top

[A07] 数字转字符串
来源：http://pgu.hammf.cn

Py:   str(42)
来源：http://zlh.jinghuilouyu.cn

PHP:  (string) 42; strval(42)
来源：http://vzh.yfazqb.com

JS:   String(42); (42).toString()
来源：http://kme.hysaishi.cn

TS:   String(42)
来源：http://evu.andypj.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://mwu.316326.xyz

Go:   strconv.Itoa(42)
来源：http://hpa.havefunace.top

Ruby: 42.to_s
来源：http://sqg.yongpay.top

C#:   42.ToString()
来源：http://wbz.dianchejie.cn

[A08] 取整与四舍五入
来源：http://woa.dashuyun.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uxk.0kj1m.cn


<!-- 参考信息 -->