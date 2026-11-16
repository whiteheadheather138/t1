代发 wailian999

[U59] PHP：自定义排序
来源：http://jnt.sweek.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fio.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://voq.xuanzx.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vkz.cashguo.top

[U61] PHP：正则
来源：http://zrf.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jek.fehbvm.com

[U62] PHP：日期对象
来源：http://pgl.meibo888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hia.nanxuanxn.top

[U63] PHP：文件读写
来源：http://akk.birdmap.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tdd.xingfuxueyuan.xyz

[U64] PHP：目录遍历
来源：http://nbc.ydjk.org.cn

glob("dir/*.php");  scandir("dir");
来源：http://iwv.jinqigfzy.top

[U65] PHP：会话
来源：http://tgm.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fuf.zhoulong.xyz

[U66] PHP：设置 Cookie
来源：http://afr.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gak.yanxiufei.cn

[U67] PHP：处理文件上传
来源：http://ydr.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pkn.bjfxy.top

[U68] PHP：PDO 连接
来源：http://rgz.jinyuanbaomall.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tde.jinqigufen.top

[U69] PHP：PDO 预处理
来源：http://gyh.guannengcc.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pcz.daxiang520.top

[U70] PHP：PDO 事务
来源：http://wka.ctjpmb.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ygi.guannengcc.top

[U71] PHP：抛出异常
来源：http://ajp.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://ejy.hnqzz.top

[U72] PHP：写错误日志
来源：http://sil.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://lby.tian-w.cn

[U73] PHP：读取 ini 配置
来源：http://ibr.bbcook.cn

parse_ini_file("config.ini", true)
来源：http://eji.quarkkingdee.top

[U74] PHP：读取环境变量
来源：http://fta.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://ipk.feifeiyinyue.top

[U75] PHP：依赖注入
来源：http://bca.shangyingyoupin.top

composer require psr/container
来源：http://rxk.hongshengwenyu.top

[U76] PHP：简单路由
来源：http://iml.9152youxi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lpt.sweek.top

[U77] PHP：模板渲染
来源：http://pqs.haohaochexian.top

composer require twig/twig
来源：http://hlz.xziqi.cn

[U78] PHP：单元测试
来源：http://yxy.jlsjyb.cn

composer require --dev phpunit/phpunit
来源：http://gir.xylfe.cn

[U79] PHP：静态分析
来源：http://hho.nwbrower.top

composer require --dev phpstan/phpstan
来源：http://xxx.jinqigufen.top

[U80] PHP：代码规范修复
来源：http://hdi.smart0.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://xxs.fzhhl.top

[U81] JS：初始化项目
来源：http://krl.cheryme.top

npm init -y;  npm i express
来源：http://nhm.uphjek.com

[U82] JS：package.json 脚本
来源：http://poh.9152youxi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dtg.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://ifn.ywan-chungtsiang.top

export const a = 1;  import { a } from "./m.js";
来源：http://zvc.tianlin.xyz

[U84] JS：CommonJS 写法
来源：http://itx.wangshuangyany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ugn.feifeiyinyue.top

[U85] JS：可选链
来源：http://dyz.wangshuangyany.cn

a?.b?.c
来源：http://yoi.hnqzz.top

[U86] JS：空值合并
来源：http://wsg.jiagoushi.top

a ?? b
来源：http://xvu.cqqwz.cn

[U87] JS：解构默认值
来源：http://ghs.jinqigufen.top

const { a = 1, b = 2 } = obj;
来源：http://cke.guannengcc.top

[U88] JS：对象展开合并
来源：http://amh.zhoulong.xyz

{ ...a, ...b }
来源：http://nyg.cdnleiting.top

[U89] JS：数组去重
来源：http://wef.iojbl.cn

[...new Set(arr)]
来源：http://wtp.zhoulong.xyz

[U90] JS：数字数组排序
来源：http://eov.hysaishi.cn

[...arr].sort((a, b) => a - b)
来源：http://zau.xuanzx.com

[U91] JS：对象键值遍历
来源：http://ceo.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rtl.uphjek.com

[U92] JS：深拷贝
来源：http://bhe.yj20258888.top

structuredClone(obj)
来源：http://byn.9152youxi.cn

[U93] JS：模板字符串
来源：http://tdk.hesvh.cn

`共 ${n} 条`
来源：http://drr.yanxiufei.cn

[U94] JS：箭头函数
来源：http://til.jqgufenzy.top

const double = x => x * 2;
来源：http://gvg.nwbrower.top

[U95] JS：Promise 包装
来源：http://ish.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://lre.quarkkingdee.top

[U96] JS：async/await 与异常
来源：http://ylh.redwolf501.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uqe.ybcxt.top

[U97] JS：并发请求
来源：http://veg.tanke756.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ytj.zhaomingkeji.xyz

[U98] JS：fetch 带 JSON
来源：http://uch.quarkkingdee.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sgh.shangyingyoupin.top

[U99] JS：事件监听
来源：http://qqx.mhx1999.top

el.addEventListener("click", e => {})
来源：http://epi.andypj.xyz

[U100] JS：DOM 查询
来源：http://iqr.pycfn.com

document.querySelector(".item")
来源：http://bal.zhijiandao.cn

[U101] JS：classList 操作
来源：http://clw.yfazqb.com

el.classList.toggle("active")
来源：http://hkm.yongpay.top

[U102] JS：本地存储
来源：http://zlg.hnxiangtu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yry.shangyingyoupin.top

[U103] JS：定时器
来源：http://yzc.guowangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rwi.jinghuilouyu.cn

[U104] JS：防抖
来源：http://amw.jinqigufen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oub.nwbrower.top

[U105] JS：节流
来源：http://pcz.ppjwa.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pcj.mhx1999.top

[U106] JS：日期格式化
来源：http://kzf.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nfo.ivvv.top

[U107] JS：数字千分位
来源：http://npu.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mwk.fehbvm.com

[U108] JS：随机整数
来源：http://dss.sufxvd.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yex.hesvh.cn

[U109] JS：数组分组
来源：http://akg.vehdjk.com

Object.groupBy(arr, x => x.type)
来源：http://rdo.guowangkeji.top

[U110] JS：数组分块
来源：http://uzj.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://diq.uphjek.com

[U111] JS：对象转 Map
来源：http://hzy.gogol.net.cn

new Map(Object.entries(obj))
来源：http://fkc.epnwcf.com

[U112] JS：字符串补位
来源：http://ufh.ybcxt.top

"7".padStart(3, "0")
来源：http://dpg.zhengqikj.top

[U113] JS：正则替换全部
来源：http://tki.ydzc1.top

s.replaceAll("a", "b")
来源：http://yce.bjfxy.top

[U114] JS：JSON 深比较
来源：http://gur.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fcq.ydzc1.top

[U115] JS：生成 UUID
来源：http://jtf.vehdjk.com

crypto.randomUUID()
来源：http://rlu.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://qtw.gotoacloud.top

/** @param {string} name */ function f(name) {}
来源：http://vsm.meibo888.top

[U117] JS：单元测试
来源：http://ihn.daria6918.cn

npm i -D vitest;  npx vitest
来源：http://yon.zycfv.cn

[U118] JS：开发服务器
来源：http://jyr.shanyushiyangkeji.top

npm i -D vite;  npx vite
来源：http://jfs.ydjk.org.cn

[U119] JS：生产构建
来源：http://kiu.jinghuilouyu.cn

npx vite build
来源：http://iov.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://ypr.jyoumei.cn

import.meta.env.VITE_API_URL
来源：http://gae.quarkkingdee.top

================================================================================
来源：http://pjd.ehwqpu.com

统计汇总
来源：http://alx.guowangkeji.top

================================================================================
来源：http://cbj.hnqzz.top

按语言统计（条）：
来源：http://loa.feifeiyinyue.top

Python ......... 252
来源：http://orq.redwolf501.top

PHP ............ 252
来源：http://mbk.nanxinkj.top

JavaScript ..... 252
来源：http://nor.ppjwa.cn

TypeScript ..... 212
来源：http://ebe.xingfuxueyuan.xyz

Java ........... 212
来源：http://fqf.shanyushiyangkeji.top

Go ............. 212
来源：http://zue.vehdjk.com

Ruby ........... 212
来源：http://blf.sysykeji.top

C# ............. 212
来源：http://nkz.yuxming.cn

C .............. 30
来源：http://xwd.hongshengwenyu.top

C++ ............ 30
来源：http://nne.zdbjq.cn

SQL ............ 90
来源：http://iic.hesvh.cn

Bash ........... 80
来源：http://zdc.nanxuanxn.top

Kotlin ......... 15
来源：http://yis.uphjek.com

Swift .......... 15
来源：http://ars.cheryme.top

Lua ............ 10
来源：http://zfy.sufxvd.cn

Perl ........... 10
来源：http://wzz.dashuyun.cn

Scala .......... 10
来源：http://osj.kuanghao11.cn

------------------------------------
来源：http://cxo.9152youxi.cn

合计 ........... 2106 条
来源：http://gvv.ivvv.top

按章节统计：
来源：http://qer.pycfn.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uap.vqdsnc.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jkp.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kzg.pycfn.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xtn.shanyushiyangtech.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eid.andypj.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://iio.yvedp.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fbe.yj20258.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pde.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://per.guannengcc.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rpp.sweek.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bbj.zhixingplan.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wzp.hammf.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://knf.tianlin.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qrs.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://flz.fengsongda.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mge.uphjek.com

Q SQL 专题                              90
来源：http://xjh.zhoulong.xyz

R Bash 专题                             80
来源：http://myk.sxryk.cn

S C / C++ 专题                          60
来源：http://ygq.ywan-chungtsiang.top

T 其他语言补充                          60
来源：http://vfq.fktsv.cn

U 高频实用片段                         120
来源：http://vva.chenlongwang.top

------------------------------------
来源：http://iib.guowangkeji.top

合计                                  2106 条
来源：http://czy.xuanzx.com

--------------------------------------------------------------------------------
来源：http://lfq.yfazqb.com

使用提醒
来源：http://csc.sysykeji.top

--------------------------------------------------------------------------------
来源：http://eny.tanke756.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tfv.yj202588.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zpo.vehdjk.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zdv.daxiang520.top

在旧版本上使用前请先确认语法支持情况。
来源：http://qrm.hywenlv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://syl.fehbvm.com

—— 文件结束 ——
来源：http://xxl.pycfn.com

================================================================================
来源：http://ncd.quarkkingdee.top

程序语言常见例子速查手册（2024 版）
来源：http://eao.yj20258.top

Common Programming Examples Cheat Book
来源：http://ryr.fengsongda.top

================================================================================
来源：http://iez.ybcxt.top

【收录内容】
来源：http://msi.andypj.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://xpt.feifeiyinyue.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iuz.ppjwa.cn

SQL · Bash · C · C++
来源：http://ycn.dianchejie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cwr.nwbrower.top

【使用说明】
来源：http://pea.nanxinkj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nxe.wangdashe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wqy.shzxlz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jxe.jiagoushi.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dcr.jyoumei.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hty.tanke756.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gqo.xuanzx.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fap.zhaomingkeji.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sxq.ppjwa.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wby.zhijiandao.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hkq.zycfv.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ncd.fktsv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kdc.aizwys.cn

【文件统计】
来源：http://wbs.dianchejie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hgl.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://dob.fehbvm.com

目  录
来源：http://ozl.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://rdu.ydzc1.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xme.sjlbkw.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://woe.jqgufenzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vhk.shangyingyoupin.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rzf.yangfankeji.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qii.epnwcf.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fkj.c1oappe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://anj.kuanghao11.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ohh.jinyuanbaomall.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fhr.jlsjyb.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ztw.sufxvd.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mjy.yuanzhike.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ctt.zdbjq.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ppz.hcnkem.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xoz.chenjidiqi.icu

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bhb.tianlin.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jup.aizwys.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://swf.zhiwuduotai.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://stg.sysykeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sec.cheryme.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ddy.hywenlv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lya.cashguo.top

================================================================================
来源：http://asy.chenjidiqi.icu

A. 基础语法与类型
来源：http://prs.cheryme.top

================================================================================
来源：http://nrg.ybcxt.top

[A01] Hello World
来源：http://knq.xinyue.icu

Py:   print("Hello, World!")
来源：http://fao.sxryk.cn

PHP:  echo "Hello, World!";
来源：http://din.birdmap.top

JS:   console.log("Hello, World!");
来源：http://ejt.zdbjq.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://iwi.yongpay.top

Java: System.out.println("Hello, World!");
来源：http://tsu.jqgufenzy.top

Go:   fmt.Println("Hello, World!")
来源：http://fya.aizwys.cn

Ruby: puts "Hello, World!"
来源：http://tsh.yvedp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vgb.fktsv.cn

[A02] 变量声明与赋值
来源：http://ypm.havefunace.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ejm.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://ikf.yongpay.top

JS:   let name = "Alex"; const age = 20;
来源：http://pfu.wangdashe.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kix.zhijiandao.cn

Java: String name = "Alex"; int age = 20;
来源：http://wkf.xylfe.cn

Go:   name := "Alex"; age := 20
来源：http://rfp.yvedp.cn

Ruby: name = "Alex"; age = 20
来源：http://tqr.gogol.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mru.birdmap.top

[A03] 常量定义
来源：http://xds.birdmap.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://avt.zhongyouzk.top

PHP:  const PI = 3.14159;
来源：http://lwn.yonumen.top

JS:   const PI = 3.14159;
来源：http://nwg.tarul.cn

TS:   const PI: number = 3.14159;
来源：http://vox.jlsjyb.cn

Java: static final double PI = 3.14159;
来源：http://seh.hnqzz.top

Go:   const PI = 3.14159
来源：http://zoy.tanke756.top

Ruby: PI = 3.14159
来源：http://jyq.redwolf501.top

C#:   const double PI = 3.14159;
来源：http://lcy.zhaomingkeji.xyz

[A04] 判断变量类型
来源：http://xoj.fanxiaobao.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://svs.redwolf501.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ldz.nanxuanxn.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://awl.hammf.cn

TS:   typeof x; x instanceof Date
来源：http://aoo.cucudq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cze.cashguo.top

Go:   reflect.TypeOf(x).Name()
来源：http://wba.nwbrower.top

Ruby: x.class; x.is_a?(Integer)
来源：http://vmq.ivvv.top

C#:   x.GetType().Name; x is int
来源：http://moa.cdnleiting.top

[A05] 整数除法与取模
来源：http://gmr.andypj.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zza.zhijiandao.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ccf.pengpengdd.cyou

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tgh.zhiwuduotai.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://orb.gotoacloud.top

Java: 7 / 2; 7 % 2
来源：http://utz.xinyue.icu

Go:   7 / 2; 7 % 2
来源：http://sto.snrcjt.cn

Ruby: 7 / 2; 7 % 2
来源：http://khe.sysykeji.top

C#:   7 / 2; 7 % 2
来源：http://awe.yuxming.cn

[A06] 字符串转数字
来源：http://ruq.zhiwuduotai.top

Py:   int("42"); float("3.14")
来源：http://eug.gogol.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dko.zhoulong.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://set.andypj.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://mwt.zhijiandao.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cvs.ppjwa.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gyg.9152youxi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dvo.zhiwuduotai.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://naf.316326.xyz

[A07] 数字转字符串
来源：http://wrg.zhijiandao.cn

Py:   str(42)
来源：http://ato.vqdsnc.cn

PHP:  (string) 42; strval(42)
来源：http://jok.xuetiantiany.cn

JS:   String(42); (42).toString()
来源：http://ipm.epnwcf.com

TS:   String(42)
来源：http://zan.sxryk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kpe.hywenlv.cn

Go:   strconv.Itoa(42)
来源：http://hzo.hesvh.cn

Ruby: 42.to_s
来源：http://jfp.jinqigfzy.top

C#:   42.ToString()
来源：http://xem.sjlbkw.cn

[A08] 取整与四舍五入
来源：http://iui.0kj1m.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ffg.tianlin.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pqo.yongpay.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://epe.ywan-chungtsiang.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yxf.yueranfly.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dqz.feifeiyinyue.top


<!-- 参考信息 -->