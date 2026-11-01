代发 wailian999

[U61] PHP：正则
来源：http://read.share.epnwcf.com/Article/details/gyuwedhua.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/ghalagahi.sHtML

[U62] PHP：日期对象
来源：http://mobile.bbcook.cn/Article/details/gimkzgrmn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fktsv.cn/Article/details/grmcebboi.sHtML

[U63] PHP：文件读写
来源：http://m.share.vehdjk.com/Article/details/giplwkuoj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.sjlbkw.cn/Article/details/gocpqathv.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.tarul.cn/Article/details/gydsnrunr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.epnwcf.com/Article/details/gaflgjvqn.sHtML

[U65] PHP：会话
来源：http://blog.sjlbkw.cn/Article/details/gshyeeilt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.tarul.cn/Article/details/ghghsvqxk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fktsv.cn/Article/details/gcvqiinfx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.epnwcf.com/Article/details/gibciixky.sHtML

[U67] PHP：处理文件上传
来源：http://baike.sjlbkw.cn/Article/details/gjeejqgon.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.sjlbkw.cn/Article/details/gfzsvnhwi.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.vehdjk.com/Article/details/gurltuytw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fktsv.cn/Article/details/gkkhboklo.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.sjlbkw.cn/Article/details/gixyoqdox.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.sjlbkw.cn/Article/details/gishdjvdj.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.tarul.cn/Article/details/gwtbbiuwx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.yfazqb.com/Article/details/guerydybg.sHtML

[U71] PHP：抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gsjgdatrq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.epnwcf.com/Article/details/gdmwjlsds.sHtML

[U72] PHP：写错误日志
来源：http://blog.tarul.cn/Article/details/giqibdyzb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fktsv.cn/Article/details/geqvxzegz.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.tarul.cn/Article/details/grjvgtaam.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.vehdjk.com/Article/details/gcphfrcjl.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gzgbbdkoc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.bbcook.cn/Article/details/gsbtnnacm.sHtML

[U75] PHP：依赖注入
来源：http://wap.sjlbkw.cn/Article/details/gjfljildr.sHtML

composer require psr/container
来源：http://3g.fktsv.cn/Article/details/gpzeurdld.sHtML

[U76] PHP：简单路由
来源：http://baike.fktsv.cn/Article/details/gfobofngn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.vehdjk.com/Article/details/gyyjvtvun.sHtML

[U77] PHP：模板渲染
来源：http://wap.yfazqb.com/Article/details/gvagxneno.sHtML

composer require twig/twig
来源：http://www.m.share.fktsv.cn/Article/details/ghqlenyqs.sHtML

[U78] PHP：单元测试
来源：http://m.share.epnwcf.com/Article/details/gwnsczkxf.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.tarul.cn/Article/details/gqwjmldpz.sHtML

[U79] PHP：静态分析
来源：http://wap.sjlbkw.cn/Article/details/gcrzhpver.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.sjlbkw.cn/Article/details/gfkxekvdj.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.sjlbkw.cn/Article/details/gwbtxlcvi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.epnwcf.com/Article/details/gyonokmlo.sHtML

[U81] JS：初始化项目
来源：http://m.share.sjlbkw.cn/Article/details/gtkkedgyt.sHtML

npm init -y;  npm i express
来源：http://www.share.epnwcf.com/Article/details/gyunbsqxk.sHtML

[U82] JS：package.json 脚本
来源：http://wap.bbcook.cn/Article/details/gwplxmyxw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.yfazqb.com/Article/details/gvsyiclbj.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.epnwcf.com/Article/details/gcacfxerx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.epnwcf.com/Article/details/gbwgpiqvj.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.epnwcf.com/Article/details/ghxuzotdg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.tarul.cn/Article/details/ghtggowvd.sHtML

[U85] JS：可选链
来源：http://www.blog.epnwcf.com/Article/details/gfvhnweic.sHtML

a?.b?.c
来源：http://www.blog.vehdjk.com/Article/details/glquldldr.sHtML

[U86] JS：空值合并
来源：http://www.share.bbcook.cn/Article/details/gkxqdnqar.sHtML

a ?? b
来源：http://wap.tarul.cn/Article/details/gznaydgvq.sHtML

[U87] JS：解构默认值
来源：http://m.share.vehdjk.com/Article/details/gnipzpktb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.tarul.cn/Article/details/gnvecvjux.sHtML

[U88] JS：对象展开合并
来源：http://m.share.bbcook.cn/Article/details/gzavaxsco.sHtML

{ ...a, ...b }
来源：http://read.share.sjlbkw.cn/Article/details/gizvuavca.sHtML

[U89] JS：数组去重
来源：http://mobile.epnwcf.com/Article/details/gfgbmoblo.sHtML

[...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gfvqduaft.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.sjlbkw.cn/Article/details/glyueklth.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gggadewnt.sHtML

[U91] JS：对象键值遍历
来源：http://wap.epnwcf.com/Article/details/gbbefgjak.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.tarul.cn/Article/details/gosasyxei.sHtML

[U92] JS：深拷贝
来源：http://blog.tarul.cn/Article/details/ggwfzcflf.sHtML

structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gbmhiofqt.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.vehdjk.com/Article/details/gaarauzih.sHtML

`共 ${n} 条`
来源：http://www.share.bbcook.cn/Article/details/giubdfqhv.sHtML

[U94] JS：箭头函数
来源：http://baike.sjlbkw.cn/Article/details/gqqxnsdrd.sHtML

const double = x => x * 2;
来源：http://3g.bbcook.cn/Article/details/gnpfzdpkp.sHtML

[U95] JS：Promise 包装
来源：http://blog.sjlbkw.cn/Article/details/gzbfuhjbm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fktsv.cn/Article/details/gruujwhjv.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.sjlbkw.cn/Article/details/gnvyffuam.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/ggpgssmbb.sHtML

[U97] JS：并发请求
来源：http://mobile.sjlbkw.cn/Article/details/geubxmxmi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gbruvpyjr.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fktsv.cn/Article/details/gqaaxwmwk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.tarul.cn/Article/details/gnsvgrtgx.sHtML

[U99] JS：事件监听
来源：http://3g.sjlbkw.cn/Article/details/gkebcsoiq.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.yfazqb.com/Article/details/gutnsutup.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.yfazqb.com/Article/details/givhznqdv.sHtML

document.querySelector(".item")
来源：http://www.blog.tarul.cn/Article/details/gbqjsuudg.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fktsv.cn/Article/details/gedngbgnw.sHtML

el.classList.toggle("active")
来源：http://www.m.share.yfazqb.com/Article/details/ghjxxpkoc.sHtML

[U102] JS：本地存储
来源：http://www.blog.tarul.cn/Article/details/glzmjzudm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.epnwcf.com/Article/details/gjfyzmgjk.sHtML

[U103] JS：定时器
来源：http://www.share.yfazqb.com/Article/details/geeoprkav.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.epnwcf.com/Article/details/gqzpwkslq.sHtML

[U104] JS：防抖
来源：http://www.m.share.epnwcf.com/Article/details/ghikxezml.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gpacjlqmf.sHtML

[U105] JS：节流
来源：http://www.m.share.yfazqb.com/Article/details/gnbygccfw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.vehdjk.com/Article/details/glfgoxitw.sHtML

[U106] JS：日期格式化
来源：http://blog.tarul.cn/Article/details/gwjoxxmgh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.vehdjk.com/Article/details/gkclkyead.sHtML

[U107] JS：数字千分位
来源：http://wap.sjlbkw.cn/Article/details/gqwmaslex.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.epnwcf.com/Article/details/gtdunbzdv.sHtML

[U108] JS：随机整数
来源：http://3g.sjlbkw.cn/Article/details/glqmajxyy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.epnwcf.com/Article/details/gflwiqouc.sHtML

[U109] JS：数组分组
来源：http://blog.tarul.cn/Article/details/gziouayvp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gfrfwspfs.sHtML

[U110] JS：数组分块
来源：http://www.share.epnwcf.com/Article/details/gquxqqfxt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.vehdjk.com/Article/details/gaqdtotvo.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.vehdjk.com/Article/details/gmmhjxita.sHtML

new Map(Object.entries(obj))
来源：http://read.share.yfazqb.com/Article/details/gfxxlevbk.sHtML

[U112] JS：字符串补位
来源：http://wap.epnwcf.com/Article/details/gkspytrrt.sHtML

"7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/grbfkjxkh.sHtML

[U113] JS：正则替换全部
来源：http://baike.epnwcf.com/Article/details/gqlkrqyqa.sHtML

s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gwjunywrd.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fktsv.cn/Article/details/gcsvftwmi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/gaspzwbcn.sHtML

[U115] JS：生成 UUID
来源：http://mobile.sjlbkw.cn/Article/details/gvxgtvjvx.sHtML

crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/givdbbkfr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.tarul.cn/Article/details/gokajmrow.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gjsfeojxw.sHtML

[U117] JS：单元测试
来源：http://www.blog.yfazqb.com/Article/details/geqqkfgup.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fktsv.cn/Article/details/gxbhbbljn.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.tarul.cn/Article/details/gbkfwxnmf.sHtML

npm i -D vite;  npx vite
来源：http://3g.epnwcf.com/Article/details/gcwwrvnkm.sHtML

[U119] JS：生产构建
来源：http://m.share.bbcook.cn/Article/details/giliuewoa.sHtML

npx vite build
来源：http://www.blog.vehdjk.com/Article/details/gagbfksvj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.tarul.cn/Article/details/gxrkxercw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.yfazqb.com/Article/details/gkmszmupm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gptjawnez.sHtML

统计汇总
来源：http://www.blog.vehdjk.com/Article/details/gqyhesrnd.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gkbxqrcvh.sHtML

按语言统计（条）：
来源：http://3g.fktsv.cn/Article/details/gomutsyan.sHtML

Python ......... 252
来源：http://mobile.yfazqb.com/Article/details/gyiwfqyzb.sHtML

PHP ............ 252
来源：http://mobile.tarul.cn/Article/details/gowzmtlpn.sHtML

JavaScript ..... 252
来源：http://3g.bbcook.cn/Article/details/gwcdpcgrl.sHtML

TypeScript ..... 212
来源：http://www.blog.fktsv.cn/Article/details/gqcuwnoip.sHtML

Java ........... 212
来源：http://read.share.fktsv.cn/Article/details/gkfthwjhi.sHtML

Go ............. 212
来源：http://blog.sjlbkw.cn/Article/details/gyqthstxs.sHtML

Ruby ........... 212
来源：http://baike.epnwcf.com/Article/details/glvcoyzzb.sHtML

C# ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/glaksdlzx.sHtML

C .............. 30
来源：http://read.share.sjlbkw.cn/Article/details/gzrmstaco.sHtML

C++ ............ 30
来源：http://www.share.vehdjk.com/Article/details/gnnizwidg.sHtML

SQL ............ 90
来源：http://baike.fktsv.cn/Article/details/gxpovtuxr.sHtML

Bash ........... 80
来源：http://3g.bbcook.cn/Article/details/gifujazyu.sHtML

Kotlin ......... 15
来源：http://m.share.fktsv.cn/Article/details/gserpwnkc.sHtML

Swift .......... 15
来源：http://blog.tarul.cn/Article/details/gxbeqlcsw.sHtML

Lua ............ 10
来源：http://www.m.share.vehdjk.com/Article/details/ggvtuglhj.sHtML

Perl ........... 10
来源：http://www.share.bbcook.cn/Article/details/gukhvwqxx.sHtML

Scala .......... 10
来源：http://m.share.fktsv.cn/Article/details/glknjmcuo.sHtML

------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gxewzhqzh.sHtML

合计 ........... 2106 条
来源：http://www.m.share.vehdjk.com/Article/details/gbjhouomc.sHtML

按章节统计：
来源：http://m.share.vehdjk.com/Article/details/goptmmipf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.vehdjk.com/Article/details/gpwocnwzv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gwfhmijmy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gkhlxksyu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gzgxvgkoa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.yfazqb.com/Article/details/gyjditbul.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fktsv.cn/Article/details/gdqpcnpeo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/gptewucsb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.bbcook.cn/Article/details/gpgsrsrwz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gdrvafvhi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.vehdjk.com/Article/details/gztvyrznj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gevtbblbt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gmehkbcyl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/glnlmrduv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.yfazqb.com/Article/details/gmipvrxfz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.tarul.cn/Article/details/gzcydeotq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/grvqcucvb.sHtML

Q SQL 专题                              90
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwgekpld.sHtML

R Bash 专题                             80
来源：http://mobile.vehdjk.com/Article/details/gcokiltvz.sHtML

S C / C++ 专题                          60
来源：http://baike.yfazqb.com/Article/details/gzaqljroh.sHtML

T 其他语言补充                          60
来源：http://www.blog.yfazqb.com/Article/details/gdfcxrxjz.sHtML

U 高频实用片段                         120
来源：http://www.share.fktsv.cn/Article/details/gyylhcokx.sHtML

------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gpobridtq.sHtML

合计                                  2106 条
来源：http://www.m.share.yfazqb.com/Article/details/guttehiwu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gfhtqiyry.sHtML

使用提醒
来源：http://www.m.share.yfazqb.com/Article/details/ggxyavdio.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gnastiagq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.tarul.cn/Article/details/gogoqyrlf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.bbcook.cn/Article/details/grvkrhnvz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.yfazqb.com/Article/details/gydtagzdy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.epnwcf.com/Article/details/givtfulwp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fktsv.cn/Article/details/gdgvhenyo.sHtML

—— 文件结束 ——
来源：http://3g.fktsv.cn/Article/details/gsvwutrkn.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghcdyfsny.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.yfazqb.com/Article/details/gqebbyuxj.sHtML

Common Programming Examples Cheat Book
来源：http://3g.yfazqb.com/Article/details/gcuspuocv.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/goiwqohqk.sHtML

【收录内容】
来源：http://baike.bbcook.cn/Article/details/galwlpuir.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.yfazqb.com/Article/details/gaekczccb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.epnwcf.com/Article/details/gntbydgvb.sHtML

SQL · Bash · C · C++
来源：http://blog.epnwcf.com/Article/details/gseroxyez.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.yfazqb.com/Article/details/gdfwwkjyt.sHtML

【使用说明】
来源：http://read.share.yfazqb.com/Article/details/gpjeebavx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.bbcook.cn/Article/details/geaalqmfa.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.tarul.cn/Article/details/grccbasdv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.epnwcf.com/Article/details/glbnwyxsl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.epnwcf.com/Article/details/gklssfqnh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.vehdjk.com/Article/details/ghoykipsy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.sjlbkw.cn/Article/details/gtbwxxtcb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.bbcook.cn/Article/details/govrkpdwa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.tarul.cn/Article/details/gubxtiiop.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.vehdjk.com/Article/details/gjvvfxpcn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.bbcook.cn/Article/details/gdgqcrrhs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fktsv.cn/Article/details/ghxcpvktz.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.sjlbkw.cn/Article/details/gzyjumcrz.sHtML

【文件统计】
来源：http://blog.bbcook.cn/Article/details/gyvcddsmw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fktsv.cn/Article/details/gxsstvlkt.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gcsdyzmav.sHtML

目  录
来源：http://mobile.epnwcf.com/Article/details/gtctbagch.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gagazxjkk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.yfazqb.com/Article/details/gujnnojgy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/grbdhvldi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gvjxvviof.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.epnwcf.com/Article/details/guilhrvjk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.yfazqb.com/Article/details/gopvtjjlf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gncbqyffw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.bbcook.cn/Article/details/gtcfdmajk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.yfazqb.com/Article/details/gumxfwckl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gxyscoytm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.tarul.cn/Article/details/gxiewsvwr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fktsv.cn/Article/details/gxvogmpix.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gbnptijcz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/gadxtoicg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.epnwcf.com/Article/details/gvoqqilvt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.tarul.cn/Article/details/gaullxojb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gabcshpkq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.epnwcf.com/Article/details/gyxncwzkw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.vehdjk.com/Article/details/gebssrvwb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.bbcook.cn/Article/details/gcrngsmkn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.bbcook.cn/Article/details/gzyfecops.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fktsv.cn/Article/details/ghvapqogp.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ggqjdspgf.sHtML

A. 基础语法与类型
来源：http://mobile.yfazqb.com/Article/details/gpftlhpel.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ghacuwpzj.sHtML

[A01] Hello World
来源：http://mobile.epnwcf.com/Article/details/gdepjumgz.sHtML

Py:   print("Hello, World!")
来源：http://read.share.epnwcf.com/Article/details/gznzczluh.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.bbcook.cn/Article/details/gvkggkuew.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/ginwigiga.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.tarul.cn/Article/details/gjcntsgvq.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/ghypwahye.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.bbcook.cn/Article/details/gejcjmhjj.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.epnwcf.com/Article/details/gvbdhqymh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.tarul.cn/Article/details/gbmpevpix.sHtML

[A02] 变量声明与赋值
来源：http://read.share.vehdjk.com/Article/details/gmtebdyzt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fktsv.cn/Article/details/gqsojfqja.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.epnwcf.com/Article/details/gzkyxqlcl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.tarul.cn/Article/details/gwldlutto.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.bbcook.cn/Article/details/ggvrcurmu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/goweuoobp.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.vehdjk.com/Article/details/gzfjhzpct.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.yfazqb.com/Article/details/gfxodnfch.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.epnwcf.com/Article/details/gqjdqvxvj.sHtML

[A03] 常量定义
来源：http://blog.sjlbkw.cn/Article/details/gwcmjdymq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.sjlbkw.cn/Article/details/gmhfseaut.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gwnumyfgt.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gcrradsos.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gckyofoft.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/grsrlggjy.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/gsfngnnux.sHtML

Ruby: PI = 3.14159
来源：http://wap.vehdjk.com/Article/details/gfqrriwag.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gopynueic.sHtML

[A04] 判断变量类型
来源：http://mobile.sjlbkw.cn/Article/details/gxvkbccum.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.bbcook.cn/Article/details/gjjfilnrn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.bbcook.cn/Article/details/gtfqzkbei.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.vehdjk.com/Article/details/ghxarbtzm.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.vehdjk.com/Article/details/garperbdh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.yfazqb.com/Article/details/glsdanjwd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.yfazqb.com/Article/details/gdtyckfof.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.bbcook.cn/Article/details/giccqmajr.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.sjlbkw.cn/Article/details/gduatrqaq.sHtML

[A05] 整数除法与取模
来源：http://mobile.fktsv.cn/Article/details/goduanely.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.vehdjk.com/Article/details/gukpwfscs.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/grlpulekp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/gckqfapat.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.bbcook.cn/Article/details/ghtbclgpo.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.vehdjk.com/Article/details/geaamxmhc.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gqfroayyh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gntlcshdz.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.sjlbkw.cn/Article/details/gpoyxabak.sHtML

[A06] 字符串转数字
来源：http://read.share.vehdjk.com/Article/details/gijhepsob.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.sjlbkw.cn/Article/details/gdzvtvqhw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.epnwcf.com/Article/details/grpuefxew.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.epnwcf.com/Article/details/ghcjirbjv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.sjlbkw.cn/Article/details/giwxbfips.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.bbcook.cn/Article/details/gbrvgrtip.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.vehdjk.com/Article/details/gsbwhdfll.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.tarul.cn/Article/details/ggjbxiabt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.sjlbkw.cn/Article/details/gyvhbjsof.sHtML

[A07] 数字转字符串
来源：http://read.share.yfazqb.com/Article/details/gnnvufene.sHtML

Py:   str(42)
来源：http://mobile.epnwcf.com/Article/details/gtyveubfo.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fktsv.cn/Article/details/gfggbmptz.sHtML

JS:   String(42); (42).toString()
来源：http://blog.yfazqb.com/Article/details/gqrhijfxd.sHtML

TS:   String(42)
来源：http://read.share.yfazqb.com/Article/details/gnnynpmxx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.tarul.cn/Article/details/gcqwirvso.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.tarul.cn/Article/details/gxkhhhzxt.sHtML

Ruby: 42.to_s
来源：http://wap.tarul.cn/Article/details/gjrzhyoey.sHtML

C#:   42.ToString()
来源：http://blog.sjlbkw.cn/Article/details/gczhgchsn.sHtML

[A08] 取整与四舍五入
来源：http://3g.bbcook.cn/Article/details/gdraywfud.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fktsv.cn/Article/details/gfefxtcjk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.tarul.cn/Article/details/gktdpainn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gykopxrqg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fktsv.cn/Article/details/gtsxxbywx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.vehdjk.com/Article/details/gutctcvae.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gmxxlpcpp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.yfazqb.com/Article/details/ghzzzlans.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.sjlbkw.cn/Article/details/gnvyfpgwo.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fktsv.cn/Article/details/gpwncbnkg.sHtML


<!-- 参考信息 -->