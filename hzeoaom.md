代发 wailian999

[U43] PHP：声明命名空间
来源：http://baike.vehdjk.com/Article/details/gljbdxuwn.sHtML

namespace App\Http;
来源：http://read.share.bbcook.cn/Article/details/getsafben.sHtML

[U44] PHP：开启严格类型
来源：http://3g.sjlbkw.cn/Article/details/gfxsxgwru.sHtML

declare(strict_types=1);
来源：http://3g.sjlbkw.cn/Article/details/guqztvnzp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.bbcook.cn/Article/details/gpvnesyew.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gwqxivugc.sHtML

[U46] PHP：可空类型
来源：http://blog.epnwcf.com/Article/details/gveqhasvk.sHtML

?string $name = null
来源：http://3g.fktsv.cn/Article/details/gqvshidtv.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.tarul.cn/Article/details/gnjymrymk.sHtML

int|string $id
来源：http://www.share.epnwcf.com/Article/details/gewfoojeb.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fktsv.cn/Article/details/gittybjzv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.yfazqb.com/Article/details/gochgopvk.sHtML

[U49] PHP：只读属性
来源：http://www.share.tarul.cn/Article/details/gexhguurb.sHtML

public readonly string $name
来源：http://m.share.yfazqb.com/Article/details/gzamhswoa.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.tarul.cn/Article/details/gwvjwgngs.sHtML

public function __construct(private int $id) {}
来源：http://read.share.bbcook.cn/Article/details/ggwakwdqd.sHtML

[U51] PHP：数组解构
来源：http://www.share.tarul.cn/Article/details/gomnvjmpz.sHtML

[$a, $b] = $arr;
来源：http://baike.sjlbkw.cn/Article/details/gsjgcrecp.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/gzeypumhb.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.tarul.cn/Article/details/gbszjgozp.sHtML

[U53] PHP：空合并运算符
来源：http://3g.bbcook.cn/Article/details/gugeecaqe.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fktsv.cn/Article/details/ggxamkqyt.sHtML

[U54] PHP：空安全调用
来源：http://blog.tarul.cn/Article/details/gigxsmmvi.sHtML

$obj?->method()
来源：http://wap.bbcook.cn/Article/details/gnajwdled.sHtML

[U55] PHP：match 表达式
来源：http://mobile.sjlbkw.cn/Article/details/grxdnfuew.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.tarul.cn/Article/details/gkguftnyr.sHtML

[U56] PHP：命名参数
来源：http://mobile.vehdjk.com/Article/details/gltazpxrx.sHtML

f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gebvhibun.sHtML

[U57] PHP：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gfamfsgat.sHtML

"值: {$a}"
来源：http://wap.vehdjk.com/Article/details/gedggemmo.sHtML

[U58] PHP：数组三件套
来源：http://wap.vehdjk.com/Article/details/gglmdbfuf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.tarul.cn/Article/details/gmdbymktu.sHtML

[U59] PHP：自定义排序
来源：http://read.share.vehdjk.com/Article/details/gsunoqxtj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/glmjrjsew.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.bbcook.cn/Article/details/gajijmrrk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.sjlbkw.cn/Article/details/gylqgeyoi.sHtML

[U61] PHP：正则
来源：http://www.m.share.yfazqb.com/Article/details/gwoxbgedk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.bbcook.cn/Article/details/gvfsfrsvc.sHtML

[U62] PHP：日期对象
来源：http://www.blog.yfazqb.com/Article/details/gxrlxtacf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.epnwcf.com/Article/details/ghnmlxsjg.sHtML

[U63] PHP：文件读写
来源：http://mobile.vehdjk.com/Article/details/gssthatjh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggobyldad.sHtML

[U64] PHP：目录遍历
来源：http://read.share.bbcook.cn/Article/details/glygnbhvq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fktsv.cn/Article/details/gxumdvedr.sHtML

[U65] PHP：会话
来源：http://3g.bbcook.cn/Article/details/gclmtgjwb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.vehdjk.com/Article/details/giwzptori.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fktsv.cn/Article/details/gwcppzomu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fktsv.cn/Article/details/gozluwulw.sHtML

[U67] PHP：处理文件上传
来源：http://wap.sjlbkw.cn/Article/details/gwvronkkc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.sjlbkw.cn/Article/details/gizsfwvxd.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.epnwcf.com/Article/details/gcxymhdvp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.sjlbkw.cn/Article/details/gvmzbqjla.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.tarul.cn/Article/details/ghhgiouvh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.epnwcf.com/Article/details/gruhmykcx.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.yfazqb.com/Article/details/gatopcgxd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fktsv.cn/Article/details/gnfoawgtw.sHtML

[U71] PHP：抛出异常
来源：http://www.share.vehdjk.com/Article/details/gqbvxmlun.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjmmbsjp.sHtML

[U72] PHP：写错误日志
来源：http://mobile.vehdjk.com/Article/details/ggfcdukrx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.tarul.cn/Article/details/grkykcfbz.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.yfazqb.com/Article/details/gyhtprsxp.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.epnwcf.com/Article/details/gtqprpqfj.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gokjiyxsv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.bbcook.cn/Article/details/glyakghxq.sHtML

[U75] PHP：依赖注入
来源：http://baike.vehdjk.com/Article/details/gxkqcmhzh.sHtML

composer require psr/container
来源：http://www.m.share.vehdjk.com/Article/details/ggldglznd.sHtML

[U76] PHP：简单路由
来源：http://blog.fktsv.cn/Article/details/grkthwonu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.vehdjk.com/Article/details/gkrkoajst.sHtML

[U77] PHP：模板渲染
来源：http://wap.bbcook.cn/Article/details/gbljragfg.sHtML

composer require twig/twig
来源：http://wap.sjlbkw.cn/Article/details/gzbxknptn.sHtML

[U78] PHP：单元测试
来源：http://3g.tarul.cn/Article/details/gqisipgny.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.tarul.cn/Article/details/gpqhkmrin.sHtML

[U79] PHP：静态分析
来源：http://m.share.vehdjk.com/Article/details/gabrxeutq.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.sjlbkw.cn/Article/details/guuhvoxfn.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.tarul.cn/Article/details/ghqyhjfyc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fktsv.cn/Article/details/gwtrkvoms.sHtML

[U81] JS：初始化项目
来源：http://mobile.vehdjk.com/Article/details/guqhjtydy.sHtML

npm init -y;  npm i express
来源：http://www.m.share.tarul.cn/Article/details/gxtevhtiw.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.vehdjk.com/Article/details/gpwdnvmxg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.tarul.cn/Article/details/gdnfusnxu.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.vehdjk.com/Article/details/gkxnpntai.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gbsxvgege.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.bbcook.cn/Article/details/gefvcjibg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.vehdjk.com/Article/details/gyzfabayq.sHtML

[U85] JS：可选链
来源：http://www.share.bbcook.cn/Article/details/grigvovij.sHtML

a?.b?.c
来源：http://read.share.bbcook.cn/Article/details/ggowxhatf.sHtML

[U86] JS：空值合并
来源：http://mobile.tarul.cn/Article/details/goxhpjqnl.sHtML

a ?? b
来源：http://blog.epnwcf.com/Article/details/ggxixaats.sHtML

[U87] JS：解构默认值
来源：http://www.blog.vehdjk.com/Article/details/glixhuwhp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.tarul.cn/Article/details/ggnkdaimz.sHtML

[U88] JS：对象展开合并
来源：http://www.share.vehdjk.com/Article/details/ggnshyfor.sHtML

{ ...a, ...b }
来源：http://3g.bbcook.cn/Article/details/gutfudfto.sHtML

[U89] JS：数组去重
来源：http://baike.epnwcf.com/Article/details/gvkkhanbq.sHtML

[...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gztceerxa.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fktsv.cn/Article/details/gevfrddmx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gylktdmbo.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.yfazqb.com/Article/details/gswfnjrfg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.sjlbkw.cn/Article/details/gxyqdlajs.sHtML

[U92] JS：深拷贝
来源：http://wap.sjlbkw.cn/Article/details/grhopoazh.sHtML

structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gmubhmnqb.sHtML

[U93] JS：模板字符串
来源：http://m.share.tarul.cn/Article/details/giqqtbyew.sHtML

`共 ${n} 条`
来源：http://wap.vehdjk.com/Article/details/gbzlpohef.sHtML

[U94] JS：箭头函数
来源：http://wap.tarul.cn/Article/details/geezzkvue.sHtML

const double = x => x * 2;
来源：http://m.share.epnwcf.com/Article/details/gliupafhx.sHtML

[U95] JS：Promise 包装
来源：http://mobile.sjlbkw.cn/Article/details/ghbvantza.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.tarul.cn/Article/details/gyqebtriy.sHtML

[U96] JS：async/await 与异常
来源：http://baike.yfazqb.com/Article/details/gypdsirag.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/goolqhoaw.sHtML

[U97] JS：并发请求
来源：http://m.share.sjlbkw.cn/Article/details/gwnjualdn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gcsavdtzx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gdiwgwppt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.tarul.cn/Article/details/guxxuhhvl.sHtML

[U99] JS：事件监听
来源：http://blog.fktsv.cn/Article/details/gafwbemck.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.bbcook.cn/Article/details/gmcxjtaoa.sHtML

[U100] JS：DOM 查询
来源：http://3g.bbcook.cn/Article/details/ggicmzbll.sHtML

document.querySelector(".item")
来源：http://baike.yfazqb.com/Article/details/gnusovwkr.sHtML

[U101] JS：classList 操作
来源：http://www.share.sjlbkw.cn/Article/details/gpfhvqqnj.sHtML

el.classList.toggle("active")
来源：http://baike.fktsv.cn/Article/details/gzzjiuzme.sHtML

[U102] JS：本地存储
来源：http://blog.tarul.cn/Article/details/gdktrmujn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.epnwcf.com/Article/details/gqkcqtkgg.sHtML

[U103] JS：定时器
来源：http://www.share.tarul.cn/Article/details/gkwvhhvpm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.yfazqb.com/Article/details/gvmyjkrab.sHtML

[U104] JS：防抖
来源：http://baike.sjlbkw.cn/Article/details/grgwnqwzn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gdeugmaen.sHtML

[U105] JS：节流
来源：http://blog.tarul.cn/Article/details/gzhbqancl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.vehdjk.com/Article/details/ghhxxxmvq.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gjmmyrgiz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.sjlbkw.cn/Article/details/gxsoeknvz.sHtML

[U107] JS：数字千分位
来源：http://3g.bbcook.cn/Article/details/gusmcdxui.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.bbcook.cn/Article/details/gwoggljnw.sHtML

[U108] JS：随机整数
来源：http://wap.epnwcf.com/Article/details/gzhmdnnfp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.sjlbkw.cn/Article/details/gdczgtpvk.sHtML

[U109] JS：数组分组
来源：http://wap.tarul.cn/Article/details/gwoqyulkw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkwrtbzl.sHtML

[U110] JS：数组分块
来源：http://www.share.yfazqb.com/Article/details/gaxpvdnld.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.sjlbkw.cn/Article/details/gujormwip.sHtML

[U111] JS：对象转 Map
来源：http://m.share.vehdjk.com/Article/details/gcyprsrxt.sHtML

new Map(Object.entries(obj))
来源：http://baike.yfazqb.com/Article/details/gyluxbjik.sHtML

[U112] JS：字符串补位
来源：http://mobile.tarul.cn/Article/details/gotzcmkvn.sHtML

"7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gkfngsyif.sHtML

[U113] JS：正则替换全部
来源：http://blog.tarul.cn/Article/details/guwvcjlut.sHtML

s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gvvvxlwqw.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fktsv.cn/Article/details/gadbrkdar.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.epnwcf.com/Article/details/ghkrjbylx.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.yfazqb.com/Article/details/gxicmroea.sHtML

crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/giuspgimd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.epnwcf.com/Article/details/gidrydcrj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.tarul.cn/Article/details/gdlmtwfbt.sHtML

[U117] JS：单元测试
来源：http://mobile.yfazqb.com/Article/details/gtfmpsivi.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.sjlbkw.cn/Article/details/gzngkykkf.sHtML

[U118] JS：开发服务器
来源：http://www.blog.vehdjk.com/Article/details/gppwsbhou.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.vehdjk.com/Article/details/gcpdptyvo.sHtML

[U119] JS：生产构建
来源：http://read.share.yfazqb.com/Article/details/gumujvxvb.sHtML

npx vite build
来源：http://www.blog.bbcook.cn/Article/details/goaimmxks.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.yfazqb.com/Article/details/ggxgcmeof.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fktsv.cn/Article/details/gxmjrmeyb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gcubisvtr.sHtML

统计汇总
来源：http://www.blog.sjlbkw.cn/Article/details/gckttzrwh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gzxukreua.sHtML

按语言统计（条）：
来源：http://www.share.bbcook.cn/Article/details/gimaxhvmw.sHtML

Python ......... 252
来源：http://wap.bbcook.cn/Article/details/gnpmmuxoh.sHtML

PHP ............ 252
来源：http://mobile.vehdjk.com/Article/details/gawsyyauo.sHtML

JavaScript ..... 252
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfijokfr.sHtML

TypeScript ..... 212
来源：http://wap.tarul.cn/Article/details/guuebsbuo.sHtML

Java ........... 212
来源：http://read.share.epnwcf.com/Article/details/gibnjorff.sHtML

Go ............. 212
来源：http://www.m.share.fktsv.cn/Article/details/goatguxxs.sHtML

Ruby ........... 212
来源：http://www.blog.fktsv.cn/Article/details/gdtnaxzia.sHtML

C# ............. 212
来源：http://3g.sjlbkw.cn/Article/details/guedwmygt.sHtML

C .............. 30
来源：http://read.share.tarul.cn/Article/details/gqayjsorb.sHtML

C++ ............ 30
来源：http://m.share.epnwcf.com/Article/details/ghexqpufw.sHtML

SQL ............ 90
来源：http://wap.yfazqb.com/Article/details/gxmdipzgy.sHtML

Bash ........... 80
来源：http://www.share.vehdjk.com/Article/details/guubgfugf.sHtML

Kotlin ......... 15
来源：http://read.share.yfazqb.com/Article/details/gmxmggiyz.sHtML

Swift .......... 15
来源：http://m.share.tarul.cn/Article/details/gdlzgixih.sHtML

Lua ............ 10
来源：http://blog.yfazqb.com/Article/details/gyqjayxgh.sHtML

Perl ........... 10
来源：http://baike.epnwcf.com/Article/details/grqctfhww.sHtML

Scala .......... 10
来源：http://www.blog.epnwcf.com/Article/details/gonxmwbgo.sHtML

------------------------------------
来源：http://mobile.bbcook.cn/Article/details/ggvuytgfj.sHtML

合计 ........... 2106 条
来源：http://www.share.yfazqb.com/Article/details/gmxybmvqy.sHtML

按章节统计：
来源：http://www.blog.yfazqb.com/Article/details/gtvcpixnk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fktsv.cn/Article/details/gdmomrepu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/ggmuifcqc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/glofocwzs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fktsv.cn/Article/details/gbxrcyeby.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.bbcook.cn/Article/details/gtjdngaod.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/gdebsfcla.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gzgazfkkx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.bbcook.cn/Article/details/geodvasmp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gfjwxynuz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gdjfucori.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gmtovykxy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gzcctjrnp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gppcwxngi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.epnwcf.com/Article/details/gbpqihpcq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.epnwcf.com/Article/details/gywaclhky.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/ghzjnzuvg.sHtML

Q SQL 专题                              90
来源：http://blog.sjlbkw.cn/Article/details/geygthwmt.sHtML

R Bash 专题                             80
来源：http://wap.vehdjk.com/Article/details/gousutkfy.sHtML

S C / C++ 专题                          60
来源：http://blog.vehdjk.com/Article/details/gnxvwoizt.sHtML

T 其他语言补充                          60
来源：http://blog.yfazqb.com/Article/details/glisiruuc.sHtML

U 高频实用片段                         120
来源：http://m.share.tarul.cn/Article/details/gumwjpidx.sHtML

------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gngcoffuc.sHtML

合计                                  2106 条
来源：http://www.share.vehdjk.com/Article/details/gtzpuwcyw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/goffrwcmo.sHtML

使用提醒
来源：http://www.share.epnwcf.com/Article/details/gyerqiyvp.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/guorhjtpm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.tarul.cn/Article/details/gelobieqd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.bbcook.cn/Article/details/gvklztqmk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.epnwcf.com/Article/details/gbyetvyin.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.tarul.cn/Article/details/gxohzuidr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.tarul.cn/Article/details/gpfdnzoom.sHtML

—— 文件结束 ——
来源：http://www.share.sjlbkw.cn/Article/details/geclpkxsr.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gembxkifc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fktsv.cn/Article/details/giusfqllc.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.bbcook.cn/Article/details/gjezjlthy.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gusqatcer.sHtML

【收录内容】
来源：http://blog.fktsv.cn/Article/details/gqbxrbwtu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.vehdjk.com/Article/details/gekbzchyt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fktsv.cn/Article/details/gjwemdnwo.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.tarul.cn/Article/details/grcpgatlx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.bbcook.cn/Article/details/gcbcfawfx.sHtML

【使用说明】
来源：http://www.m.share.fktsv.cn/Article/details/geaffsmhs.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.tarul.cn/Article/details/glrqypnai.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.bbcook.cn/Article/details/gkohuynqe.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.bbcook.cn/Article/details/gyzlqylzh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.bbcook.cn/Article/details/guvhhsljd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.vehdjk.com/Article/details/gmbyhnlfe.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.tarul.cn/Article/details/gmwczmtuc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.tarul.cn/Article/details/gzzbvjqcx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.tarul.cn/Article/details/gpgauudbm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.fktsv.cn/Article/details/gzwiygvwo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.epnwcf.com/Article/details/gpzcnoayb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.sjlbkw.cn/Article/details/gksljeqfn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fktsv.cn/Article/details/gvpkjotya.sHtML

【文件统计】
来源：http://m.share.vehdjk.com/Article/details/guvvjctip.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fktsv.cn/Article/details/gvxxgdvdh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gemfkdvlv.sHtML

目  录
来源：http://mobile.fktsv.cn/Article/details/gwvgwspuh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gxltkuzxi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.yfazqb.com/Article/details/ghcrksvoi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/gppxzujor.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/giytnuldh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fktsv.cn/Article/details/gefgidbzf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.vehdjk.com/Article/details/glesqalut.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.yfazqb.com/Article/details/gcisyoxof.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gpaizmjyk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.yfazqb.com/Article/details/gtlwwdbeo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/gxxmqtrhj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.yfazqb.com/Article/details/ghmtrsmyh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gowxpcaam.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gkfylttqn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gygbrvwbn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fktsv.cn/Article/details/gilbvtkne.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.epnwcf.com/Article/details/ghtthyldv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gqqajqtht.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.bbcook.cn/Article/details/gxweaxhax.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.yfazqb.com/Article/details/gxxmakyka.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.epnwcf.com/Article/details/gzytznfah.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.yfazqb.com/Article/details/gzsdskhkx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/ggmdwhico.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gaoltzllg.sHtML

A. 基础语法与类型
来源：http://baike.fktsv.cn/Article/details/geldeylcp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gploygjol.sHtML

[A01] Hello World
来源：http://m.share.yfazqb.com/Article/details/gyvunatai.sHtML

Py:   print("Hello, World!")
来源：http://www.share.bbcook.cn/Article/details/gqofpcojv.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.sjlbkw.cn/Article/details/gwxkqydvt.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/gzsfqtqxl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.sjlbkw.cn/Article/details/gtghnagez.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqonkqqj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.epnwcf.com/Article/details/gzqtcjzjz.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.vehdjk.com/Article/details/gtmrfgqrc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.sjlbkw.cn/Article/details/giqnyhxsh.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.tarul.cn/Article/details/gekspfxem.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.bbcook.cn/Article/details/gzlrynqgu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gydqlshfq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.vehdjk.com/Article/details/gigecarqp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.bbcook.cn/Article/details/gddccjhdx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gbgwmkvfx.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.yfazqb.com/Article/details/ggacypngp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.tarul.cn/Article/details/gwfafprnr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gzcfqfrxz.sHtML

[A03] 常量定义
来源：http://mobile.fktsv.cn/Article/details/gglilsfgn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.bbcook.cn/Article/details/gmrtoubcb.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/grpbxjshi.sHtML

JS:   const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gxyuozfvb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gocibltkx.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gygbefcrc.sHtML

Go:   const PI = 3.14159
来源：http://mobile.epnwcf.com/Article/details/gisggvlrv.sHtML

Ruby: PI = 3.14159
来源：http://read.share.yfazqb.com/Article/details/gfpmdktwm.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gqpfddzvl.sHtML

[A04] 判断变量类型
来源：http://wap.epnwcf.com/Article/details/gudmuyisv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.vehdjk.com/Article/details/grlknzenz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fktsv.cn/Article/details/gywhbgagd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.bbcook.cn/Article/details/gdxxcuqup.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.bbcook.cn/Article/details/gxeubmsxz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.tarul.cn/Article/details/ggclzyibp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fktsv.cn/Article/details/gdawofyeh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fktsv.cn/Article/details/gmywstyyp.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fktsv.cn/Article/details/ghhhkwmcr.sHtML

[A05] 整数除法与取模
来源：http://www.blog.yfazqb.com/Article/details/gsncdxjax.sHtML


<!-- 参考信息 -->