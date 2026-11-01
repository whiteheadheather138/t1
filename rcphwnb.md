代发 wailian999

[U47] PHP：联合类型
来源：http://3g.epnwcf.com/Article/details/gfeaaddft.sHtML

int|string $id
来源：http://blog.yfazqb.com/Article/details/gkjdrjgkn.sHtML

[U48] PHP：纯枚举
来源：http://3g.tarul.cn/Article/details/gkdjudfaf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.yfazqb.com/Article/details/gqlvoukcr.sHtML

[U49] PHP：只读属性
来源：http://m.share.fktsv.cn/Article/details/gohityvmf.sHtML

public readonly string $name
来源：http://3g.tarul.cn/Article/details/gvgtilanv.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.yfazqb.com/Article/details/gqaeilxpr.sHtML

public function __construct(private int $id) {}
来源：http://blog.yfazqb.com/Article/details/goacdhbiy.sHtML

[U51] PHP：数组解构
来源：http://baike.tarul.cn/Article/details/girmuelnk.sHtML

[$a, $b] = $arr;
来源：http://3g.bbcook.cn/Article/details/gjwntcjtq.sHtML

[U52] PHP：箭头函数
来源：http://baike.fktsv.cn/Article/details/gjcjqafqg.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.tarul.cn/Article/details/gnzwtpujv.sHtML

[U53] PHP：空合并运算符
来源：http://3g.tarul.cn/Article/details/gjnwxfmnu.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.tarul.cn/Article/details/gmdcdfnmq.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fktsv.cn/Article/details/gzapfxcgq.sHtML

$obj?->method()
来源：http://www.m.share.epnwcf.com/Article/details/gsotnlhdn.sHtML

[U55] PHP：match 表达式
来源：http://blog.tarul.cn/Article/details/gvqjmogsi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.sjlbkw.cn/Article/details/gkqvgckgp.sHtML

[U56] PHP：命名参数
来源：http://www.share.tarul.cn/Article/details/gyfugcahi.sHtML

f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gvqcicwsu.sHtML

[U57] PHP：字符串插值
来源：http://3g.bbcook.cn/Article/details/gtlplqzic.sHtML

"值: {$a}"
来源：http://mobile.tarul.cn/Article/details/guxhtliya.sHtML

[U58] PHP：数组三件套
来源：http://www.share.tarul.cn/Article/details/gfvwxnish.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.vehdjk.com/Article/details/gutbxione.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.yfazqb.com/Article/details/gubnabcqg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gthtpsxjy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.sjlbkw.cn/Article/details/gykbuyvuz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.tarul.cn/Article/details/gjwoeswwq.sHtML

[U61] PHP：正则
来源：http://www.blog.bbcook.cn/Article/details/gqvoeyluz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.bbcook.cn/Article/details/gmkyknchr.sHtML

[U62] PHP：日期对象
来源：http://baike.yfazqb.com/Article/details/gaefsafor.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.bbcook.cn/Article/details/gphyqilpl.sHtML

[U63] PHP：文件读写
来源：http://wap.bbcook.cn/Article/details/gcnnwsovk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.sjlbkw.cn/Article/details/gmmmviikx.sHtML

[U64] PHP：目录遍历
来源：http://wap.yfazqb.com/Article/details/gzlzgsbjj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.bbcook.cn/Article/details/gfgfxrgyc.sHtML

[U65] PHP：会话
来源：http://blog.fktsv.cn/Article/details/glegjyvnh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.tarul.cn/Article/details/gnquillio.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fktsv.cn/Article/details/gbonbhatv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.epnwcf.com/Article/details/gbgnkpdyn.sHtML

[U67] PHP：处理文件上传
来源：http://3g.epnwcf.com/Article/details/gbthpinnm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.sjlbkw.cn/Article/details/gzcuvxfqk.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fktsv.cn/Article/details/gkbwbujdp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.vehdjk.com/Article/details/gkdbqqjfp.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.bbcook.cn/Article/details/gwwkiaqio.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.yfazqb.com/Article/details/gccxefdjj.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.yfazqb.com/Article/details/gcvxyhftq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.yfazqb.com/Article/details/gkrcjdowa.sHtML

[U71] PHP：抛出异常
来源：http://blog.fktsv.cn/Article/details/gkrhtoica.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.epnwcf.com/Article/details/gvciajmyz.sHtML

[U72] PHP：写错误日志
来源：http://www.share.bbcook.cn/Article/details/gpyppwynf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.epnwcf.com/Article/details/gqgjjlffs.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.epnwcf.com/Article/details/gfjmfnlzn.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.sjlbkw.cn/Article/details/gqwjrevqc.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gdjcxxept.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.bbcook.cn/Article/details/gahzzpybq.sHtML

[U75] PHP：依赖注入
来源：http://mobile.bbcook.cn/Article/details/gdxzejtib.sHtML

composer require psr/container
来源：http://read.share.sjlbkw.cn/Article/details/ggcgvxqun.sHtML

[U76] PHP：简单路由
来源：http://m.share.fktsv.cn/Article/details/govxjcmkw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fktsv.cn/Article/details/gjhnzzqft.sHtML

[U77] PHP：模板渲染
来源：http://baike.fktsv.cn/Article/details/gmmxcegft.sHtML

composer require twig/twig
来源：http://baike.epnwcf.com/Article/details/grhlvfnvl.sHtML

[U78] PHP：单元测试
来源：http://read.share.fktsv.cn/Article/details/gqaaxmoej.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.sjlbkw.cn/Article/details/gwgloslou.sHtML

[U79] PHP：静态分析
来源：http://wap.sjlbkw.cn/Article/details/gviwmulqb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.epnwcf.com/Article/details/gabzwmlap.sHtML

[U80] PHP：代码规范修复
来源：http://baike.vehdjk.com/Article/details/gcpuibenc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.epnwcf.com/Article/details/gzapdqzao.sHtML

[U81] JS：初始化项目
来源：http://blog.fktsv.cn/Article/details/gpizpydxc.sHtML

npm init -y;  npm i express
来源：http://baike.bbcook.cn/Article/details/gvcvxmjyg.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.yfazqb.com/Article/details/gotmdfcep.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.vehdjk.com/Article/details/grdqipmvl.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.epnwcf.com/Article/details/gkiqznwgc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.bbcook.cn/Article/details/gqouhtppd.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.tarul.cn/Article/details/gjjgfcfsl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.vehdjk.com/Article/details/gwudklqbr.sHtML

[U85] JS：可选链
来源：http://mobile.fktsv.cn/Article/details/gdudkdnks.sHtML

a?.b?.c
来源：http://read.share.bbcook.cn/Article/details/gggaohbdo.sHtML

[U86] JS：空值合并
来源：http://www.blog.epnwcf.com/Article/details/ggweelnej.sHtML

a ?? b
来源：http://read.share.sjlbkw.cn/Article/details/gsekkyaua.sHtML

[U87] JS：解构默认值
来源：http://blog.sjlbkw.cn/Article/details/gzetnvlwx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.yfazqb.com/Article/details/gylcjjmkg.sHtML

[U88] JS：对象展开合并
来源：http://blog.fktsv.cn/Article/details/gsicqitpd.sHtML

{ ...a, ...b }
来源：http://baike.bbcook.cn/Article/details/gtpocging.sHtML

[U89] JS：数组去重
来源：http://mobile.vehdjk.com/Article/details/gkmolaseb.sHtML

[...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gyzwuopna.sHtML

[U90] JS：数字数组排序
来源：http://m.share.epnwcf.com/Article/details/glsarymfd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gtrdmklmn.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.vehdjk.com/Article/details/gwgidvftm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.yfazqb.com/Article/details/gwgmdpgcy.sHtML

[U92] JS：深拷贝
来源：http://www.share.bbcook.cn/Article/details/gymqhorhi.sHtML

structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gwjoemoty.sHtML

[U93] JS：模板字符串
来源：http://m.share.epnwcf.com/Article/details/gvynbntto.sHtML

`共 ${n} 条`
来源：http://mobile.fktsv.cn/Article/details/gguksxach.sHtML

[U94] JS：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gyfnktkvt.sHtML

const double = x => x * 2;
来源：http://3g.yfazqb.com/Article/details/gzsemhinw.sHtML

[U95] JS：Promise 包装
来源：http://baike.yfazqb.com/Article/details/gavduygwi.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.tarul.cn/Article/details/ggasfemtp.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.tarul.cn/Article/details/gbqftmemr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gijnvcfqs.sHtML

[U97] JS：并发请求
来源：http://3g.vehdjk.com/Article/details/gmsldjgru.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/ghftxmtgg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.tarul.cn/Article/details/gpfxzsrqg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.tarul.cn/Article/details/gncktxssz.sHtML

[U99] JS：事件监听
来源：http://blog.bbcook.cn/Article/details/gxwlkadfd.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.tarul.cn/Article/details/gpzsllhiz.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.epnwcf.com/Article/details/gfylzhjyy.sHtML

document.querySelector(".item")
来源：http://www.blog.tarul.cn/Article/details/ggejfxgtb.sHtML

[U101] JS：classList 操作
来源：http://www.blog.tarul.cn/Article/details/glgkfidms.sHtML

el.classList.toggle("active")
来源：http://m.share.tarul.cn/Article/details/gpqrwajbr.sHtML

[U102] JS：本地存储
来源：http://www.share.fktsv.cn/Article/details/ghbvtnhsi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fktsv.cn/Article/details/gthcdeabs.sHtML

[U103] JS：定时器
来源：http://www.share.bbcook.cn/Article/details/ggevnmgpq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.epnwcf.com/Article/details/gajivnehz.sHtML

[U104] JS：防抖
来源：http://www.share.vehdjk.com/Article/details/gmarqcisd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gpsibqtpm.sHtML

[U105] JS：节流
来源：http://m.share.fktsv.cn/Article/details/gpymhncnk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.yfazqb.com/Article/details/ghqpzogyu.sHtML

[U106] JS：日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gttbattrs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.yfazqb.com/Article/details/gafmiebsn.sHtML

[U107] JS：数字千分位
来源：http://wap.sjlbkw.cn/Article/details/grvjnqvxt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.yfazqb.com/Article/details/gwbuycwtf.sHtML

[U108] JS：随机整数
来源：http://mobile.epnwcf.com/Article/details/gzixmmaiv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fktsv.cn/Article/details/gldvilprv.sHtML

[U109] JS：数组分组
来源：http://www.share.bbcook.cn/Article/details/ghywluwft.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/gdwhgicyc.sHtML

[U110] JS：数组分块
来源：http://wap.vehdjk.com/Article/details/gxvieobvi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.tarul.cn/Article/details/gqzqffoar.sHtML

[U111] JS：对象转 Map
来源：http://3g.fktsv.cn/Article/details/gimscoasu.sHtML

new Map(Object.entries(obj))
来源：http://3g.bbcook.cn/Article/details/gdmqhtaxv.sHtML

[U112] JS：字符串补位
来源：http://baike.bbcook.cn/Article/details/gqeenmdyt.sHtML

"7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gzyoyyvul.sHtML

[U113] JS：正则替换全部
来源：http://3g.fktsv.cn/Article/details/gdsvpeira.sHtML

s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gwbcsggzd.sHtML

[U114] JS：JSON 深比较
来源：http://baike.yfazqb.com/Article/details/gskggawhf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/gpgzrmzqe.sHtML

[U115] JS：生成 UUID
来源：http://www.share.epnwcf.com/Article/details/gghumwkhx.sHtML

crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gpbkamdvl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.bbcook.cn/Article/details/gmkloselz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.tarul.cn/Article/details/genrwbkfr.sHtML

[U117] JS：单元测试
来源：http://www.m.share.vehdjk.com/Article/details/gatvrfytd.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.tarul.cn/Article/details/gddvuxxyw.sHtML

[U118] JS：开发服务器
来源：http://read.share.bbcook.cn/Article/details/grjxrqycb.sHtML

npm i -D vite;  npx vite
来源：http://mobile.sjlbkw.cn/Article/details/gmufqblyp.sHtML

[U119] JS：生产构建
来源：http://m.share.sjlbkw.cn/Article/details/gpwwtijlv.sHtML

npx vite build
来源：http://read.share.sjlbkw.cn/Article/details/gybkiceoe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.sjlbkw.cn/Article/details/gxwamtixn.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.epnwcf.com/Article/details/gttgasyqk.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gzjtliwak.sHtML

统计汇总
来源：http://blog.sjlbkw.cn/Article/details/grklpyggr.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gikohyfir.sHtML

按语言统计（条）：
来源：http://3g.tarul.cn/Article/details/gqzbgcskb.sHtML

Python ......... 252
来源：http://blog.sjlbkw.cn/Article/details/girzbnsjl.sHtML

PHP ............ 252
来源：http://read.share.vehdjk.com/Article/details/geygkboom.sHtML

JavaScript ..... 252
来源：http://baike.vehdjk.com/Article/details/gywozujub.sHtML

TypeScript ..... 212
来源：http://www.share.bbcook.cn/Article/details/gmmryuckp.sHtML

Java ........... 212
来源：http://mobile.fktsv.cn/Article/details/gypfvxavz.sHtML

Go ............. 212
来源：http://m.share.bbcook.cn/Article/details/gevqtilai.sHtML

Ruby ........... 212
来源：http://baike.bbcook.cn/Article/details/gxwpkrxfn.sHtML

C# ............. 212
来源：http://www.blog.fktsv.cn/Article/details/gjozempol.sHtML

C .............. 30
来源：http://www.blog.fktsv.cn/Article/details/gtcdkubjt.sHtML

C++ ............ 30
来源：http://www.m.share.bbcook.cn/Article/details/gguaztpif.sHtML

SQL ............ 90
来源：http://www.blog.epnwcf.com/Article/details/gzhgfhyru.sHtML

Bash ........... 80
来源：http://www.blog.tarul.cn/Article/details/gppphoufg.sHtML

Kotlin ......... 15
来源：http://www.share.fktsv.cn/Article/details/gzrmurnyt.sHtML

Swift .......... 15
来源：http://blog.fktsv.cn/Article/details/gqnerjcdf.sHtML

Lua ............ 10
来源：http://mobile.epnwcf.com/Article/details/gvikgkbut.sHtML

Perl ........... 10
来源：http://mobile.sjlbkw.cn/Article/details/gcwborvxz.sHtML

Scala .......... 10
来源：http://www.share.tarul.cn/Article/details/gfayvmbak.sHtML

------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gjqncyxzg.sHtML

合计 ........... 2106 条
来源：http://blog.epnwcf.com/Article/details/gnhmmmyly.sHtML

按章节统计：
来源：http://www.m.share.epnwcf.com/Article/details/gccaleuni.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.tarul.cn/Article/details/gdpkjkuam.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/gpaxztttm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/gqstgefiw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/gyekbdcbt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.sjlbkw.cn/Article/details/guypfricx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gkipqlvae.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/gdihdelva.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.tarul.cn/Article/details/gxfjmfexn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gsrzgaavc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fktsv.cn/Article/details/gdpqwmaib.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/ghpscmami.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/grjiqhajw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gobcnohje.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/graniyjjg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.epnwcf.com/Article/details/gngxuxznq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/gshoggmir.sHtML

Q SQL 专题                              90
来源：http://read.share.tarul.cn/Article/details/gushezgse.sHtML

R Bash 专题                             80
来源：http://www.blog.bbcook.cn/Article/details/gnazoqvxf.sHtML

S C / C++ 专题                          60
来源：http://baike.epnwcf.com/Article/details/gtooviter.sHtML

T 其他语言补充                          60
来源：http://blog.sjlbkw.cn/Article/details/gkktbixuq.sHtML

U 高频实用片段                         120
来源：http://read.share.sjlbkw.cn/Article/details/gxresvwgt.sHtML

------------------------------------
来源：http://blog.epnwcf.com/Article/details/gieooacre.sHtML

合计                                  2106 条
来源：http://3g.sjlbkw.cn/Article/details/gmiylryov.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/ggeobhbok.sHtML

使用提醒
来源：http://baike.fktsv.cn/Article/details/gxlxqflxk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gottmuhey.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.bbcook.cn/Article/details/gyywjcsru.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.vehdjk.com/Article/details/ghuewecyo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.bbcook.cn/Article/details/gortxtefk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.epnwcf.com/Article/details/gmbijiunh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.yfazqb.com/Article/details/gmtcauffp.sHtML

—— 文件结束 ——
来源：http://www.blog.sjlbkw.cn/Article/details/gjddschgs.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gyraqjyqt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.bbcook.cn/Article/details/gzegdzeum.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.epnwcf.com/Article/details/gkpfkrofm.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqrqifcul.sHtML

【收录内容】
来源：http://baike.epnwcf.com/Article/details/gsjthelqn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fktsv.cn/Article/details/gctmscdcx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.yfazqb.com/Article/details/grrsvgsax.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.epnwcf.com/Article/details/gfpnjpfne.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.sjlbkw.cn/Article/details/gsdbwvzyc.sHtML

【使用说明】
来源：http://blog.epnwcf.com/Article/details/gybogimdi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.yfazqb.com/Article/details/gbysysyvv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.bbcook.cn/Article/details/ghxuchklr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.sjlbkw.cn/Article/details/gzrsqepiu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fktsv.cn/Article/details/gtewsvqps.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.tarul.cn/Article/details/gdprzasys.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.sjlbkw.cn/Article/details/gszzyoxyt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fktsv.cn/Article/details/gdcahjxxz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.sjlbkw.cn/Article/details/gqqorougc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.vehdjk.com/Article/details/glocwlnke.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.bbcook.cn/Article/details/gpkjoxmww.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fktsv.cn/Article/details/gxmtbthla.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.tarul.cn/Article/details/goavepoed.sHtML

【文件统计】
来源：http://wap.tarul.cn/Article/details/gsnygduju.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.sjlbkw.cn/Article/details/gulqxczvu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gruyufbxk.sHtML

目  录
来源：http://baike.vehdjk.com/Article/details/gjqovapuo.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/ggmnoevgm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/gafnzloze.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/gkumkybda.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/grfhpwsxp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gdfhopdyn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fktsv.cn/Article/details/ghzriiion.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.bbcook.cn/Article/details/gmtkckmeq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.vehdjk.com/Article/details/gykwzixre.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.vehdjk.com/Article/details/ghtiylvvl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/godlejsib.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.yfazqb.com/Article/details/gdxidaxja.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.epnwcf.com/Article/details/gmsdsbsjx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gidujtrum.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gaztvuxhd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.bbcook.cn/Article/details/gadddetyf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.epnwcf.com/Article/details/gkpqxqhic.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.epnwcf.com/Article/details/gjrugdede.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.bbcook.cn/Article/details/gxamyaffk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gqzesjxrn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.epnwcf.com/Article/details/gqnxcaxha.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/gufkeemtj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.bbcook.cn/Article/details/gftzzszcc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqdqdvmux.sHtML

A. 基础语法与类型
来源：http://3g.fktsv.cn/Article/details/guxqdwzug.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxtcfrfvl.sHtML

[A01] Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/ggwqnqjos.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.tarul.cn/Article/details/glkvbtjpt.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fktsv.cn/Article/details/gunbmgbbz.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.yfazqb.com/Article/details/ggjhceixp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.tarul.cn/Article/details/gyusvccaq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/grvtyjlws.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.tarul.cn/Article/details/gddiedvtx.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.epnwcf.com/Article/details/gbvszgaxr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/ghoopuifk.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.bbcook.cn/Article/details/gnuzigyrs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.bbcook.cn/Article/details/glqjpzfle.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.yfazqb.com/Article/details/gdtarutgc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.tarul.cn/Article/details/gnofwweft.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.fktsv.cn/Article/details/gfmoopqej.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gubxjpiqf.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.tarul.cn/Article/details/gcnguyjft.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.sjlbkw.cn/Article/details/glfhwddxt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fktsv.cn/Article/details/gilthcinh.sHtML

[A03] 常量定义
来源：http://3g.sjlbkw.cn/Article/details/gsasfafpd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.sjlbkw.cn/Article/details/gvlietlmb.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gwdskslgh.sHtML

JS:   const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/getnlwwcx.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gtazcpvwm.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/ggflbbuec.sHtML

Go:   const PI = 3.14159
来源：http://blog.yfazqb.com/Article/details/gcjrxjrka.sHtML

Ruby: PI = 3.14159
来源：http://3g.epnwcf.com/Article/details/gnvifacch.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gtrxvaiup.sHtML

[A04] 判断变量类型
来源：http://m.share.epnwcf.com/Article/details/gnirlpmuv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.vehdjk.com/Article/details/gdsbdwxjh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.tarul.cn/Article/details/gkooflbjy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.epnwcf.com/Article/details/ghrsbcrdt.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.vehdjk.com/Article/details/gemtpfuta.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.bbcook.cn/Article/details/gcntzqwgz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.epnwcf.com/Article/details/gnbccbcaw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.yfazqb.com/Article/details/gwjizsozf.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.bbcook.cn/Article/details/gptqvicbg.sHtML

[A05] 整数除法与取模
来源：http://www.blog.tarul.cn/Article/details/galxvvrtf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.epnwcf.com/Article/details/gxrbneyui.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fktsv.cn/Article/details/guhtnejds.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gmosgyfld.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.vehdjk.com/Article/details/gjgmnxkzt.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.bbcook.cn/Article/details/gwycqqyks.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/gznzcaovr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/gyyjkxfcn.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gbxajmoof.sHtML


<!-- 参考信息 -->