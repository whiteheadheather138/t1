代发 wailian999

[U55] PHP：match 表达式
来源：http://read.share.fktsv.cn/Article/details/gyeoozief.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.yfazqb.com/Article/details/gurzbqddz.sHtML

[U56] PHP：命名参数
来源：http://mobile.tarul.cn/Article/details/gbzmgtipk.sHtML

f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gpgcbzkdv.sHtML

[U57] PHP：字符串插值
来源：http://blog.fktsv.cn/Article/details/grgjurtap.sHtML

"值: {$a}"
来源：http://read.share.epnwcf.com/Article/details/guikcqttu.sHtML

[U58] PHP：数组三件套
来源：http://wap.bbcook.cn/Article/details/gkybrwppe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.vehdjk.com/Article/details/goqarhqhv.sHtML

[U59] PHP：自定义排序
来源：http://3g.bbcook.cn/Article/details/gekdwqqyg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.bbcook.cn/Article/details/gluhymkro.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fktsv.cn/Article/details/gbjkuyxdz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.vehdjk.com/Article/details/gmbfmarqm.sHtML

[U61] PHP：正则
来源：http://3g.epnwcf.com/Article/details/germlnstj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gnxmztjgj.sHtML

[U62] PHP：日期对象
来源：http://mobile.sjlbkw.cn/Article/details/gxcxffgzv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.bbcook.cn/Article/details/geugvggra.sHtML

[U63] PHP：文件读写
来源：http://blog.vehdjk.com/Article/details/groxiobtn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.sjlbkw.cn/Article/details/gcazdlglb.sHtML

[U64] PHP：目录遍历
来源：http://blog.yfazqb.com/Article/details/ghjdnkrtk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.vehdjk.com/Article/details/giszyfktq.sHtML

[U65] PHP：会话
来源：http://mobile.fktsv.cn/Article/details/gqovgxzad.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gijkqqbfh.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.tarul.cn/Article/details/gyeaesirp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fktsv.cn/Article/details/gxbohdatq.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.sjlbkw.cn/Article/details/giedmozsi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.sjlbkw.cn/Article/details/gsyjbhqut.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fktsv.cn/Article/details/gwjoycugn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.epnwcf.com/Article/details/gqicjznzb.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.yfazqb.com/Article/details/gdavhznbz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.bbcook.cn/Article/details/ghpfvgjtv.sHtML

[U70] PHP：PDO 事务
来源：http://baike.epnwcf.com/Article/details/gslqeactp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.epnwcf.com/Article/details/govnlvogx.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fktsv.cn/Article/details/gvesobijl.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gzvcwdhuy.sHtML

[U72] PHP：写错误日志
来源：http://m.share.sjlbkw.cn/Article/details/grjqcyxrs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.epnwcf.com/Article/details/gxtvjompm.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fktsv.cn/Article/details/gmgudoyxz.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.epnwcf.com/Article/details/gvwocophg.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fktsv.cn/Article/details/gsquhodld.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.epnwcf.com/Article/details/gltqusvwr.sHtML

[U75] PHP：依赖注入
来源：http://blog.bbcook.cn/Article/details/ghvudoipt.sHtML

composer require psr/container
来源：http://www.m.share.yfazqb.com/Article/details/gbeijnpxa.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.bbcook.cn/Article/details/gogilkkzj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.vehdjk.com/Article/details/gpvfxnrgj.sHtML

[U77] PHP：模板渲染
来源：http://read.share.epnwcf.com/Article/details/gvolvvwhn.sHtML

composer require twig/twig
来源：http://blog.sjlbkw.cn/Article/details/gwkkeueao.sHtML

[U78] PHP：单元测试
来源：http://www.blog.sjlbkw.cn/Article/details/gsupfoljg.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.epnwcf.com/Article/details/gqefnotgz.sHtML

[U79] PHP：静态分析
来源：http://read.share.vehdjk.com/Article/details/gyuysndxr.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.bbcook.cn/Article/details/gakewrcln.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fktsv.cn/Article/details/gkpgdnpip.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.bbcook.cn/Article/details/gnovcmazu.sHtML

[U81] JS：初始化项目
来源：http://mobile.yfazqb.com/Article/details/gxqjxalse.sHtML

npm init -y;  npm i express
来源：http://www.blog.fktsv.cn/Article/details/ggbfnjknj.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.epnwcf.com/Article/details/gpqntcwxl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.bbcook.cn/Article/details/gqaoxahhu.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.bbcook.cn/Article/details/gazzwgvja.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/gyhrihecb.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.vehdjk.com/Article/details/gmejefwqx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.bbcook.cn/Article/details/gebdyqjku.sHtML

[U85] JS：可选链
来源：http://mobile.epnwcf.com/Article/details/gxkplbznq.sHtML

a?.b?.c
来源：http://www.m.share.yfazqb.com/Article/details/grvmbhiaw.sHtML

[U86] JS：空值合并
来源：http://m.share.epnwcf.com/Article/details/gdtaorxwu.sHtML

a ?? b
来源：http://blog.yfazqb.com/Article/details/gneiomkvb.sHtML

[U87] JS：解构默认值
来源：http://3g.tarul.cn/Article/details/gvvklaqxl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.bbcook.cn/Article/details/grxpyjrap.sHtML

[U88] JS：对象展开合并
来源：http://baike.bbcook.cn/Article/details/goiygqpru.sHtML

{ ...a, ...b }
来源：http://www.m.share.fktsv.cn/Article/details/gvampmluc.sHtML

[U89] JS：数组去重
来源：http://wap.vehdjk.com/Article/details/gxkibpboc.sHtML

[...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/gdojcoxxi.sHtML

[U90] JS：数字数组排序
来源：http://3g.bbcook.cn/Article/details/gcleakfxl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gtjghpcqp.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.vehdjk.com/Article/details/glisaaqyq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.epnwcf.com/Article/details/gdsizptjz.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.tarul.cn/Article/details/gnawdsqgz.sHtML

structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gsdtghjqe.sHtML

[U93] JS：模板字符串
来源：http://read.share.fktsv.cn/Article/details/gtcomtnan.sHtML

`共 ${n} 条`
来源：http://www.share.epnwcf.com/Article/details/ghlgknwdu.sHtML

[U94] JS：箭头函数
来源：http://www.blog.vehdjk.com/Article/details/gadgfrmsg.sHtML

const double = x => x * 2;
来源：http://m.share.bbcook.cn/Article/details/gkqnwtetk.sHtML

[U95] JS：Promise 包装
来源：http://wap.yfazqb.com/Article/details/ghmmgvatg.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.vehdjk.com/Article/details/gscbwfsyt.sHtML

[U96] JS：async/await 与异常
来源：http://blog.sjlbkw.cn/Article/details/garqphwtx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gfiabedbn.sHtML

[U97] JS：并发请求
来源：http://www.blog.fktsv.cn/Article/details/gpbjjmusk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gbpvimdfy.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.epnwcf.com/Article/details/gdygbyrdc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fktsv.cn/Article/details/guazgdekj.sHtML

[U99] JS：事件监听
来源：http://www.blog.epnwcf.com/Article/details/gsbgtzknn.sHtML

el.addEventListener("click", e => {})
来源：http://3g.epnwcf.com/Article/details/gpmjupszz.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gnalckaeq.sHtML

document.querySelector(".item")
来源：http://3g.sjlbkw.cn/Article/details/gwktqsbpt.sHtML

[U101] JS：classList 操作
来源：http://www.blog.sjlbkw.cn/Article/details/gbhtqckpv.sHtML

el.classList.toggle("active")
来源：http://m.share.tarul.cn/Article/details/gwciezfxs.sHtML

[U102] JS：本地存储
来源：http://wap.vehdjk.com/Article/details/gvypnfqgd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.yfazqb.com/Article/details/gpueupvly.sHtML

[U103] JS：定时器
来源：http://www.share.fktsv.cn/Article/details/gjhzqnpue.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.epnwcf.com/Article/details/gvbzpgdqi.sHtML

[U104] JS：防抖
来源：http://www.m.share.vehdjk.com/Article/details/gqmjbpyam.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gkshbwnpm.sHtML

[U105] JS：节流
来源：http://www.blog.epnwcf.com/Article/details/gfhgeiuem.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.bbcook.cn/Article/details/gndynoiau.sHtML

[U106] JS：日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/grxiieuwr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.vehdjk.com/Article/details/giqaqhdzo.sHtML

[U107] JS：数字千分位
来源：http://3g.epnwcf.com/Article/details/gnihgwnjk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.tarul.cn/Article/details/gsnyhvkia.sHtML

[U108] JS：随机整数
来源：http://read.share.epnwcf.com/Article/details/gqjzdmeed.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.epnwcf.com/Article/details/gkkgdfqgo.sHtML

[U109] JS：数组分组
来源：http://m.share.vehdjk.com/Article/details/gbkmlfroz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gstiydpha.sHtML

[U110] JS：数组分块
来源：http://mobile.bbcook.cn/Article/details/gbpmdyqpx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.epnwcf.com/Article/details/gjzkowejv.sHtML

[U111] JS：对象转 Map
来源：http://read.share.epnwcf.com/Article/details/guqxcovfd.sHtML

new Map(Object.entries(obj))
来源：http://wap.fktsv.cn/Article/details/ghsynmesd.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.bbcook.cn/Article/details/ghccsoshy.sHtML

"7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gidlsvtbc.sHtML

[U113] JS：正则替换全部
来源：http://3g.epnwcf.com/Article/details/gntncrkap.sHtML

s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/godpshofe.sHtML

[U114] JS：JSON 深比较
来源：http://baike.yfazqb.com/Article/details/gwqutrcob.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fktsv.cn/Article/details/gmbwsgjmk.sHtML

[U115] JS：生成 UUID
来源：http://blog.epnwcf.com/Article/details/gxfbmkazf.sHtML

crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gwkvpbudc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fktsv.cn/Article/details/giilulatu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gpvzvysam.sHtML

[U117] JS：单元测试
来源：http://mobile.bbcook.cn/Article/details/ggpzjxwst.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.tarul.cn/Article/details/graiwbtyd.sHtML

[U118] JS：开发服务器
来源：http://blog.sjlbkw.cn/Article/details/gacdpupcj.sHtML

npm i -D vite;  npx vite
来源：http://blog.bbcook.cn/Article/details/gregixfyj.sHtML

[U119] JS：生产构建
来源：http://blog.sjlbkw.cn/Article/details/grzwtgbje.sHtML

npx vite build
来源：http://wap.yfazqb.com/Article/details/gpvcjmybl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.bbcook.cn/Article/details/gjayjvbgu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fktsv.cn/Article/details/gkfaqxbik.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsxmeabnx.sHtML

统计汇总
来源：http://www.m.share.epnwcf.com/Article/details/ganjcteaw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gukveddsu.sHtML

按语言统计（条）：
来源：http://read.share.bbcook.cn/Article/details/gmwloiqny.sHtML

Python ......... 252
来源：http://3g.vehdjk.com/Article/details/gqllmocly.sHtML

PHP ............ 252
来源：http://mobile.vehdjk.com/Article/details/ggpulqtus.sHtML

JavaScript ..... 252
来源：http://m.share.bbcook.cn/Article/details/goydjwlyk.sHtML

TypeScript ..... 212
来源：http://wap.vehdjk.com/Article/details/ggrmnxixl.sHtML

Java ........... 212
来源：http://blog.vehdjk.com/Article/details/gzqhnlohm.sHtML

Go ............. 212
来源：http://3g.vehdjk.com/Article/details/gqzkbirlu.sHtML

Ruby ........... 212
来源：http://www.blog.vehdjk.com/Article/details/glgmbnqoi.sHtML

C# ............. 212
来源：http://m.share.fktsv.cn/Article/details/gzknxjbjs.sHtML

C .............. 30
来源：http://blog.epnwcf.com/Article/details/gmtjhuxhu.sHtML

C++ ............ 30
来源：http://read.share.epnwcf.com/Article/details/gbkikpbsk.sHtML

SQL ............ 90
来源：http://www.m.share.yfazqb.com/Article/details/gbuvzshlj.sHtML

Bash ........... 80
来源：http://read.share.sjlbkw.cn/Article/details/gnmhirbfn.sHtML

Kotlin ......... 15
来源：http://www.blog.epnwcf.com/Article/details/gkhaizvhr.sHtML

Swift .......... 15
来源：http://baike.yfazqb.com/Article/details/geyiixsfn.sHtML

Lua ............ 10
来源：http://www.m.share.fktsv.cn/Article/details/gnbjdhbjq.sHtML

Perl ........... 10
来源：http://baike.tarul.cn/Article/details/getissfud.sHtML

Scala .......... 10
来源：http://www.m.share.epnwcf.com/Article/details/ggbiatijs.sHtML

------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gjgxzsugw.sHtML

合计 ........... 2106 条
来源：http://blog.vehdjk.com/Article/details/gtahwbjoa.sHtML

按章节统计：
来源：http://wap.bbcook.cn/Article/details/gynwjoqxl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.bbcook.cn/Article/details/gyhvakdsy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gqcnwkqhy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gyodcxgtv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gspzzzaod.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.epnwcf.com/Article/details/gyqgwxafx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/gpzefjisr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/gpwdqstzp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.bbcook.cn/Article/details/gqicozteb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gpbbabcih.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fktsv.cn/Article/details/gjxtudbzl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gdrxqgvig.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gvqwrcltf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gdmgdyzut.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.bbcook.cn/Article/details/gzpdaoqes.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fktsv.cn/Article/details/gbumdovjz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gmhgbjjiw.sHtML

Q SQL 专题                              90
来源：http://baike.yfazqb.com/Article/details/gmunuvuns.sHtML

R Bash 专题                             80
来源：http://blog.yfazqb.com/Article/details/gksmbqvpb.sHtML

S C / C++ 专题                          60
来源：http://www.share.sjlbkw.cn/Article/details/gbavmicxa.sHtML

T 其他语言补充                          60
来源：http://m.share.tarul.cn/Article/details/gtacpoefb.sHtML

U 高频实用片段                         120
来源：http://3g.bbcook.cn/Article/details/grdfkbbeo.sHtML

------------------------------------
来源：http://blog.epnwcf.com/Article/details/goxeuxyop.sHtML

合计                                  2106 条
来源：http://blog.fktsv.cn/Article/details/gkyhylpwt.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gumcyeszj.sHtML

使用提醒
来源：http://baike.vehdjk.com/Article/details/gowxbhexc.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gpkmtqosi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.vehdjk.com/Article/details/gdxgftkxc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.vehdjk.com/Article/details/gxbbyvgsr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmaiymnn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.sjlbkw.cn/Article/details/gmlblgnlg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.sjlbkw.cn/Article/details/gemppemxc.sHtML

—— 文件结束 ——
来源：http://www.blog.epnwcf.com/Article/details/gdjydsuin.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqrdxmgzx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.yfazqb.com/Article/details/gknknvvmc.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fktsv.cn/Article/details/grrfksydp.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkdoxabbd.sHtML

【收录内容】
来源：http://wap.bbcook.cn/Article/details/gzedfjnqy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fktsv.cn/Article/details/garvypjoe.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcrsvylm.sHtML

SQL · Bash · C · C++
来源：http://mobile.sjlbkw.cn/Article/details/gkzasktzg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.epnwcf.com/Article/details/gbswbgpoy.sHtML

【使用说明】
来源：http://blog.epnwcf.com/Article/details/gjuvgvtkt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.tarul.cn/Article/details/gdflconlk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.yfazqb.com/Article/details/glvyxbxfb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.bbcook.cn/Article/details/gqnptywuy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.bbcook.cn/Article/details/gtkmzaqeg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fktsv.cn/Article/details/gejnnkwqz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fktsv.cn/Article/details/gckbnondd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.tarul.cn/Article/details/gkgknxwbm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.bbcook.cn/Article/details/gcxhjomff.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.yfazqb.com/Article/details/ghherubqh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.bbcook.cn/Article/details/glhpzuute.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.sjlbkw.cn/Article/details/gffgglzsy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.vehdjk.com/Article/details/gyaecahfe.sHtML

【文件统计】
来源：http://www.share.tarul.cn/Article/details/gsaxawedg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fktsv.cn/Article/details/ghakdptah.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gdcmeynvn.sHtML

目  录
来源：http://www.blog.vehdjk.com/Article/details/gxrubvrdm.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gsnaiftpc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.yfazqb.com/Article/details/gtcimqqcc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.bbcook.cn/Article/details/gbbzwexpf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.epnwcf.com/Article/details/genuqqrfd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.bbcook.cn/Article/details/gbelpcmgd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.epnwcf.com/Article/details/gkfmujhta.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.bbcook.cn/Article/details/guybbprvj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/gvlgikgxb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.sjlbkw.cn/Article/details/gdvcdcmfx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/gcsdawcar.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gmkvjgrbw.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gvaawrhbp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/gxmmblzkt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gcqljtvxs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.tarul.cn/Article/details/gclobzqlz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.epnwcf.com/Article/details/gjbqeexsy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/glwpwpfwp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.tarul.cn/Article/details/grkdeyonf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.yfazqb.com/Article/details/gbvqdhbwk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.sjlbkw.cn/Article/details/govuozvld.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/gcbxcnndg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.tarul.cn/Article/details/gvlycvdjo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwultacei.sHtML

A. 基础语法与类型
来源：http://blog.vehdjk.com/Article/details/gdhswjave.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gslrfmmzb.sHtML

[A01] Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gaopwhfou.sHtML

Py:   print("Hello, World!")
来源：http://www.share.vehdjk.com/Article/details/gzknydzyc.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.yfazqb.com/Article/details/grfhvvama.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gjjobarus.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fktsv.cn/Article/details/gqlbqlbia.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fktsv.cn/Article/details/gkexcciyp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fktsv.cn/Article/details/gevibxkac.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.yfazqb.com/Article/details/gyckglamo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.yfazqb.com/Article/details/gkjqdhwzp.sHtML

[A02] 变量声明与赋值
来源：http://blog.epnwcf.com/Article/details/gtcgbebol.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.vehdjk.com/Article/details/gmernqrjn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.epnwcf.com/Article/details/gwokpxcce.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fktsv.cn/Article/details/gokerwuub.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.tarul.cn/Article/details/gqyraxefb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gccujgygd.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.epnwcf.com/Article/details/gulghyspc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.yfazqb.com/Article/details/gziwgnlll.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.vehdjk.com/Article/details/gedkoypuh.sHtML

[A03] 常量定义
来源：http://www.blog.yfazqb.com/Article/details/ggilgswdj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.bbcook.cn/Article/details/gihrinfba.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gpcwdzdiw.sHtML

JS:   const PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gsrpwegju.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gibcfouez.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gvtwhcnrj.sHtML

Go:   const PI = 3.14159
来源：http://3g.bbcook.cn/Article/details/gdrjkgyba.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.yfazqb.com/Article/details/gzsfkwfiu.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gxsekqamt.sHtML

[A04] 判断变量类型
来源：http://baike.vehdjk.com/Article/details/gncclveps.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.yfazqb.com/Article/details/gudsaayzy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.bbcook.cn/Article/details/gvjdlytci.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fktsv.cn/Article/details/gaoumiefm.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.tarul.cn/Article/details/gwkywjhvj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.epnwcf.com/Article/details/gynvyvmkt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fktsv.cn/Article/details/gnbbpfglb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.yfazqb.com/Article/details/gcqicxgzp.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.vehdjk.com/Article/details/gmycwzwpp.sHtML

[A05] 整数除法与取模
来源：http://wap.vehdjk.com/Article/details/gzywubhsg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.yfazqb.com/Article/details/guiasdsvc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gxhsbhdzv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gsdxfzaho.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/giifnoabt.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gaoyikeuo.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gqukbdhrk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.bbcook.cn/Article/details/graltkhjn.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gcpymmoic.sHtML

[A06] 字符串转数字
来源：http://baike.fktsv.cn/Article/details/gtzyvnegp.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.bbcook.cn/Article/details/gzmdyzwae.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.tarul.cn/Article/details/gnnlkclhx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.yfazqb.com/Article/details/gjitvjahg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.vehdjk.com/Article/details/gjzemayxj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.epnwcf.com/Article/details/gwscstisi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fktsv.cn/Article/details/gpwhcrqod.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.vehdjk.com/Article/details/goecorvzs.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.yfazqb.com/Article/details/gidtfjpye.sHtML

[A07] 数字转字符串
来源：http://baike.epnwcf.com/Article/details/gwvsgnsne.sHtML

Py:   str(42)
来源：http://www.blog.sjlbkw.cn/Article/details/glzdixytn.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.sjlbkw.cn/Article/details/gfqgfjihi.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.sjlbkw.cn/Article/details/gjiwhxsqh.sHtML

TS:   String(42)
来源：http://read.share.epnwcf.com/Article/details/gwjpdonaf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fktsv.cn/Article/details/gdecisvzm.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.yfazqb.com/Article/details/gdzmhvmfl.sHtML


<!-- 参考信息 -->