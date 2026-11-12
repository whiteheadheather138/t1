代发 wailian999

[U55] PHP：match 表达式
来源：http://sxm.shuidangran.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zyl.ehwqpu.com

[U56] PHP：命名参数
来源：http://nlv.havefunace.top

f(a: 1, b: 2)
来源：http://vin.9152youxi.cn

[U57] PHP：字符串插值
来源：http://sqz.zhixingplan.top

"值: {$a}"
来源：http://fsj.jiagoushi.top

[U58] PHP：数组三件套
来源：http://sjd.sufxvd.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://htx.yvedp.cn

[U59] PHP：自定义排序
来源：http://ixd.smart0.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jcx.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://rzg.jinqigfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://giv.ppjwa.cn

[U61] PHP：正则
来源：http://ris.fktsv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://aoe.fktsv.cn

[U62] PHP：日期对象
来源：http://rab.bjfxy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sre.shanyushiyangkeji.top

[U63] PHP：文件读写
来源：http://woo.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dyt.zhengqikj.top

[U64] PHP：目录遍历
来源：http://yto.smart0.xyz

glob("dir/*.php");  scandir("dir");
来源：http://vyh.snrcjt.cn

[U65] PHP：会话
来源：http://cba.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rnw.cucudq.cn

[U66] PHP：设置 Cookie
来源：http://cgg.xylfe.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://chz.ehwqpu.com

[U67] PHP：处理文件上传
来源：http://qld.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tao.jinyuanbaomall.cn

[U68] PHP：PDO 连接
来源：http://xbk.hfpthk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xjo.ywan-chungtsiang.top

[U69] PHP：PDO 预处理
来源：http://qmh.yangfankeji.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xcd.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://hjk.xylfe.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://evx.nwbrower.top

[U71] PHP：抛出异常
来源：http://nlj.hnqzz.top

throw new RuntimeException("失败", 500);
来源：http://wzf.xylfe.cn

[U72] PHP：写错误日志
来源：http://pvh.ybcxt.top

error_log("失败: " . $e->getMessage());
来源：http://qrs.zhaomingkeji.xyz

[U73] PHP：读取 ini 配置
来源：http://lid.yueranfly.top

parse_ini_file("config.ini", true)
来源：http://hit.ctjpmb.com

[U74] PHP：读取环境变量
来源：http://ltt.jinqigfzy.top

getenv("APP_ENV") ?: "production"
来源：http://zke.epnwcf.com

[U75] PHP：依赖注入
来源：http://ilp.uphjek.com

composer require psr/container
来源：http://gbb.yvedp.cn

[U76] PHP：简单路由
来源：http://wkt.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hpr.sysykeji.top

[U77] PHP：模板渲染
来源：http://awb.vehdjk.com

composer require twig/twig
来源：http://wqi.chenjidiqi.icu

[U78] PHP：单元测试
来源：http://lej.zdbjq.cn

composer require --dev phpunit/phpunit
来源：http://stq.quarkkingdee.top

[U79] PHP：静态分析
来源：http://xid.yuxming.cn

composer require --dev phpstan/phpstan
来源：http://jjj.chenzaomai.com

[U80] PHP：代码规范修复
来源：http://anj.daxiang520.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wcc.jinyuanbaomall.cn

[U81] JS：初始化项目
来源：http://qvb.316326.xyz

npm init -y;  npm i express
来源：http://dfa.ydzc1.top

[U82] JS：package.json 脚本
来源：http://col.havefunace.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ddh.svipenyu.cn

[U83] JS：ES Module 导入导出
来源：http://bzm.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fbn.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://rno.yongpay.top

module.exports = { a };  const { a } = require("./m");
来源：http://aak.hammf.cn

[U85] JS：可选链
来源：http://nsm.xylfe.cn

a?.b?.c
来源：http://tvi.shangyingyoupin.top

[U86] JS：空值合并
来源：http://noa.ybcxt.top

a ?? b
来源：http://cgx.quarkkingdee.top

[U87] JS：解构默认值
来源：http://yzx.zhaomingkeji.xyz

const { a = 1, b = 2 } = obj;
来源：http://swf.yj20258.top

[U88] JS：对象展开合并
来源：http://roq.jqgfzy.top

{ ...a, ...b }
来源：http://zxs.hnqzz.top

[U89] JS：数组去重
来源：http://cfl.jianghu66.top

[...new Set(arr)]
来源：http://kob.xingfuxueyuan.xyz

[U90] JS：数字数组排序
来源：http://nxg.hesvh.cn

[...arr].sort((a, b) => a - b)
来源：http://sbk.ydjk.org.cn

[U91] JS：对象键值遍历
来源：http://nbg.yonumen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fim.cqqwz.cn

[U92] JS：深拷贝
来源：http://bne.tianlin.xyz

structuredClone(obj)
来源：http://pds.chenlongwang.top

[U93] JS：模板字符串
来源：http://ncn.jyoumei.cn

`共 ${n} 条`
来源：http://osa.cucudq.cn

[U94] JS：箭头函数
来源：http://dmf.cdnleiting.top

const double = x => x * 2;
来源：http://net.sjlbkw.cn

[U95] JS：Promise 包装
来源：http://ljt.wangshuangyany.cn

new Promise((resolve, reject) => {})
来源：http://jrs.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://nar.jiagoushi.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hik.hongshengwenyu.top

[U97] JS：并发请求
来源：http://mgx.chenjidiqi.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://ain.yj20258888.top

[U98] JS：fetch 带 JSON
来源：http://zwy.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gqz.smart0.xyz

[U99] JS：事件监听
来源：http://kbm.jqgufenzy.top

el.addEventListener("click", e => {})
来源：http://xpf.xylfe.cn

[U100] JS：DOM 查询
来源：http://lwo.cheryme.top

document.querySelector(".item")
来源：http://jss.andypj.xyz

[U101] JS：classList 操作
来源：http://sab.dianchejie.cn

el.classList.toggle("active")
来源：http://fjz.hammf.cn

[U102] JS：本地存储
来源：http://vdw.snrcjt.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mfx.andypj.xyz

[U103] JS：定时器
来源：http://fyn.redwolf501.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ifn.yangfankeji.com

[U104] JS：防抖
来源：http://vba.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jnf.xuanzx.com

[U105] JS：节流
来源：http://ptl.ydjk.org.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yfd.daria6918.cn

[U106] JS：日期格式化
来源：http://dvk.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qwc.jlsjyb.cn

[U107] JS：数字千分位
来源：http://rnl.fengsongda.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ked.52xcode.cn

[U108] JS：随机整数
来源：http://zzk.jianghu66.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fko.yuxming.cn

[U109] JS：数组分组
来源：http://ced.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://fgs.smart0.xyz

[U110] JS：数组分块
来源：http://tgd.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rjo.nanxinkj.top

[U111] JS：对象转 Map
来源：http://ggd.hysaishi.cn

new Map(Object.entries(obj))
来源：http://dtk.zhongyouzk.top

[U112] JS：字符串补位
来源：http://aji.ydzc1.top

"7".padStart(3, "0")
来源：http://gkr.cdnleiting.top

[U113] JS：正则替换全部
来源：http://zcx.zhixingplan.top

s.replaceAll("a", "b")
来源：http://dqe.guowangkeji.top

[U114] JS：JSON 深比较
来源：http://zpu.yuanzhike.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ptx.xingfuxueyuan.xyz

[U115] JS：生成 UUID
来源：http://hwh.ywan-chungtsiang.top

crypto.randomUUID()
来源：http://nfp.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://wgq.fktsv.cn

/** @param {string} name */ function f(name) {}
来源：http://mlr.hfpthk.cn

[U117] JS：单元测试
来源：http://wil.iojbl.cn

npm i -D vitest;  npx vitest
来源：http://nxj.hfpthk.cn

[U118] JS：开发服务器
来源：http://eiw.chenzaomai.com

npm i -D vite;  npx vite
来源：http://azz.cucudq.cn

[U119] JS：生产构建
来源：http://fzr.iojbl.cn

npx vite build
来源：http://yei.yj202588.top

[U120] JS：读取环境变量（Vite）
来源：http://ihw.yangfankeji.com

import.meta.env.VITE_API_URL
来源：http://qda.zhiwuduotai.top

================================================================================
来源：http://yzl.hongshengwenyu.top

统计汇总
来源：http://mlx.shzxlz.cn

================================================================================
来源：http://xfd.aibaodan.cn

按语言统计（条）：
来源：http://ace.cdnleiting.top

Python ......... 252
来源：http://mni.fzhhl.top

PHP ............ 252
来源：http://sfr.nanxuanxn.top

JavaScript ..... 252
来源：http://mqz.svipenyu.cn

TypeScript ..... 212
来源：http://dfc.nanxuanxn.top

Java ........... 212
来源：http://pje.andypj.xyz

Go ............. 212
来源：http://unz.tarul.cn

Ruby ........... 212
来源：http://ryn.yuanzhike.top

C# ............. 212
来源：http://utw.tanke756.top

C .............. 30
来源：http://eui.wangshuangyany.cn

C++ ............ 30
来源：http://twt.snrcjt.cn

SQL ............ 90
来源：http://pdf.wangdashe.top

Bash ........... 80
来源：http://fin.jyoumei.cn

Kotlin ......... 15
来源：http://utx.pengpengdd.cyou

Swift .......... 15
来源：http://mzc.dianchejie.cn

Lua ............ 10
来源：http://lnf.fktsv.cn

Perl ........... 10
来源：http://dqj.sjlbkw.cn

Scala .......... 10
来源：http://ypf.yonumen.top

------------------------------------
来源：http://loz.daxiang520.top

合计 ........... 2106 条
来源：http://usu.fehbvm.com

按章节统计：
来源：http://gnr.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xby.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pqd.yonumen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://izz.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dcq.sweek.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vre.nwbrower.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kwu.svipenyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vut.xinyue.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tor.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bcs.svipenyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://spm.chenlongwang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gdh.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ytv.zhongyouzk.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ddj.ydjk.org.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ivt.fanxiaobao.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cet.cdnleiting.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://aax.jyoumei.cn

Q SQL 专题                              90
来源：http://hpj.sxryk.cn

R Bash 专题                             80
来源：http://jha.yj20258.top

S C / C++ 专题                          60
来源：http://prg.hesvh.cn

T 其他语言补充                          60
来源：http://aph.chenlongwang.top

U 高频实用片段                         120
来源：http://cwd.zhaomingkeji.xyz

------------------------------------
来源：http://pwq.sxryk.cn

合计                                  2106 条
来源：http://pmi.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://yth.nwbrower.top

使用提醒
来源：http://yzj.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://ghy.mhx1999.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rtz.sysykeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://llh.ehwqpu.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ess.guowangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fve.sjlbkw.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wgq.ivvv.top

—— 文件结束 ——
来源：http://uew.mhx1999.top

================================================================================
来源：http://rdu.zycfv.cn

程序语言常见例子速查手册（2024 版）
来源：http://zcw.nanxinkj.top

Common Programming Examples Cheat Book
来源：http://bao.zdbjq.cn

================================================================================
来源：http://tht.quarkkingdee.top

【收录内容】
来源：http://ell.52xcode.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sdh.jinqigufen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eor.yanxiufei.cn

SQL · Bash · C · C++
来源：http://ysv.hfpthk.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ajg.sjlbkw.cn

【使用说明】
来源：http://ngv.sufxvd.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ivb.smart0.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nfv.cashguo.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dlg.ywan-chungtsiang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kuw.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://azc.jinghuilouyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nwe.xziqi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cew.hcnkem.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kle.jinyuanbaomall.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jtm.ybcxt.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rfx.pycfn.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zmw.sjlbkw.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kaf.meibo888.top

【文件统计】
来源：http://jtm.jiagoushi.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hdn.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://irv.jlsjyb.cn

目  录
来源：http://pko.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://rte.hfpthk.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tup.jiagoushi.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xaf.chenzaomai.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ewp.uphjek.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qsc.aibaodan.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nha.yj20258.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://juo.fzhhl.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xun.zhijiandao.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jvk.zycfv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kdy.daria6918.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://spo.xinyue.icu

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sgz.nanxuanxn.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ifi.hywenlv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jrz.mhx1999.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gbn.chenjidiqi.icu

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wqe.jiagoushi.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sph.jqgfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cep.hywenlv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oxd.jianghu66.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rni.hongshengwenyu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://unv.yueranfly.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cnn.fzhhl.top

================================================================================
来源：http://zfv.ydjk.org.cn

A. 基础语法与类型
来源：http://etp.svipenyu.cn

================================================================================
来源：http://pqz.zhiwuduotai.top

[A01] Hello World
来源：http://reu.jqgufenzy.top

Py:   print("Hello, World!")
来源：http://tym.iojbl.cn

PHP:  echo "Hello, World!";
来源：http://qck.shanyushiyangtech.top

JS:   console.log("Hello, World!");
来源：http://lcj.yj202588.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uog.sweek.top

Java: System.out.println("Hello, World!");
来源：http://fdd.nwbrower.top

Go:   fmt.Println("Hello, World!")
来源：http://jhp.guowangkeji.top

Ruby: puts "Hello, World!"
来源：http://loy.xylfe.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ocq.zhongyouzk.top

[A02] 变量声明与赋值
来源：http://nzm.0kj1m.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pkj.316326.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://nnu.haohaochexian.top

JS:   let name = "Alex"; const age = 20;
来源：http://mhn.fktsv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wjx.gaohongyu789.top

Java: String name = "Alex"; int age = 20;
来源：http://eai.zhongyouzk.top

Go:   name := "Alex"; age := 20
来源：http://hwy.hesvh.cn

Ruby: name = "Alex"; age = 20
来源：http://dxy.ctjpmb.com

C#:   string name = "Alex"; int age = 20;
来源：http://cqa.yuanzhike.top

[A03] 常量定义
来源：http://ijv.guowangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zhw.iojbl.cn

PHP:  const PI = 3.14159;
来源：http://wna.yanxiufei.cn

JS:   const PI = 3.14159;
来源：http://qhl.hongshengwenyu.top

TS:   const PI: number = 3.14159;
来源：http://grh.sjlbkw.cn

Java: static final double PI = 3.14159;
来源：http://vkd.sxryk.cn

Go:   const PI = 3.14159
来源：http://rbz.ydzc1.top

Ruby: PI = 3.14159
来源：http://xhz.tianlin.xyz

C#:   const double PI = 3.14159;
来源：http://suw.ppjwa.cn

[A04] 判断变量类型
来源：http://rik.guowangkeji.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://rya.dashuyun.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nvj.hammf.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fmn.yfazqb.com

TS:   typeof x; x instanceof Date
来源：http://jrp.zhiwuduotai.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rvg.shzxlz.cn

Go:   reflect.TypeOf(x).Name()
来源：http://izn.cheryme.top

Ruby: x.class; x.is_a?(Integer)
来源：http://noa.zhiwuduotai.top

C#:   x.GetType().Name; x is int
来源：http://acv.shuidangran.top

[A05] 整数除法与取模
来源：http://xue.yj20258888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tpi.jinqigfzy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://tqk.ivvv.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dpl.jyoumei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bak.zhengqikj.top

Java: 7 / 2; 7 % 2
来源：http://pah.hnqzz.top

Go:   7 / 2; 7 % 2
来源：http://hfc.meibo888.top

Ruby: 7 / 2; 7 % 2
来源：http://ufz.yj20258.top

C#:   7 / 2; 7 % 2
来源：http://ytk.sjlbkw.cn

[A06] 字符串转数字
来源：http://atp.yj202588.top

Py:   int("42"); float("3.14")
来源：http://cqb.fzhhl.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wvm.hesvh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ebc.havefunace.top

TS:   parseInt("42", 10); Number("42")
来源：http://ffz.jinghuilouyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qsh.hcnkem.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://udc.bbcook.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pqf.shzxlz.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://aka.redwolf501.top

[A07] 数字转字符串
来源：http://gqz.yuanzhike.top

Py:   str(42)
来源：http://iwa.yueranfly.top

PHP:  (string) 42; strval(42)
来源：http://atu.zhaomingkeji.xyz

JS:   String(42); (42).toString()
来源：http://wmh.sysykeji.top

TS:   String(42)
来源：http://jrr.fehbvm.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://ipi.mhx1999.top

Go:   strconv.Itoa(42)
来源：http://ryn.cqqwz.cn


<!-- 参考信息 -->