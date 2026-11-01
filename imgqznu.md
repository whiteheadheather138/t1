代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://blog.fktsv.cn/Article/details/gmylvgtxk.sHtML

sys.stdout.isatty()
来源：http://www.blog.fktsv.cn/Article/details/gjijahvxp.sHtML

[U40] Py：打印到标准错误
来源：http://baike.yfazqb.com/Article/details/gdxkoduvd.sHtML

print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/gpykzuomw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.vehdjk.com/Article/details/gthzioove.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.tarul.cn/Article/details/gmknvezke.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.bbcook.cn/Article/details/gjcllbfnf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.tarul.cn/Article/details/gkmqcsxza.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.tarul.cn/Article/details/gvasubqve.sHtML

namespace App\Http;
来源：http://mobile.epnwcf.com/Article/details/geaqbginj.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.sjlbkw.cn/Article/details/gujmxawle.sHtML

declare(strict_types=1);
来源：http://www.share.epnwcf.com/Article/details/gukvwedsn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.sjlbkw.cn/Article/details/ghxnjylcb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gmkwdgrla.sHtML

[U46] PHP：可空类型
来源：http://mobile.tarul.cn/Article/details/gnvmyeqhu.sHtML

?string $name = null
来源：http://3g.sjlbkw.cn/Article/details/gfwrnrihh.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.bbcook.cn/Article/details/gyrmlagbw.sHtML

int|string $id
来源：http://blog.fktsv.cn/Article/details/gujgnfrtn.sHtML

[U48] PHP：纯枚举
来源：http://blog.tarul.cn/Article/details/gblnizims.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.tarul.cn/Article/details/gunzqoofy.sHtML

[U49] PHP：只读属性
来源：http://wap.vehdjk.com/Article/details/grllcqeip.sHtML

public readonly string $name
来源：http://baike.epnwcf.com/Article/details/gwuvseeit.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.epnwcf.com/Article/details/gkpfkidsr.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fktsv.cn/Article/details/gqyacnfnv.sHtML

[U51] PHP：数组解构
来源：http://read.share.sjlbkw.cn/Article/details/ghvhxclvm.sHtML

[$a, $b] = $arr;
来源：http://wap.yfazqb.com/Article/details/ghyjebnhy.sHtML

[U52] PHP：箭头函数
来源：http://blog.fktsv.cn/Article/details/gpinwmgdk.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.epnwcf.com/Article/details/gkzivgjtj.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fktsv.cn/Article/details/gvlaervvn.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.tarul.cn/Article/details/gdlpfhmkn.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.tarul.cn/Article/details/gvlsslqqm.sHtML

$obj?->method()
来源：http://blog.fktsv.cn/Article/details/glbsnwtak.sHtML

[U55] PHP：match 表达式
来源：http://blog.vehdjk.com/Article/details/gzruwzwhm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.tarul.cn/Article/details/gdgivtwsv.sHtML

[U56] PHP：命名参数
来源：http://www.blog.epnwcf.com/Article/details/guyoursdx.sHtML

f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gqnugeama.sHtML

[U57] PHP：字符串插值
来源：http://3g.tarul.cn/Article/details/givdbjrhj.sHtML

"值: {$a}"
来源：http://www.m.share.vehdjk.com/Article/details/gbwtqxaqb.sHtML

[U58] PHP：数组三件套
来源：http://m.share.vehdjk.com/Article/details/giwpsblqw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.yfazqb.com/Article/details/gkncdrqqa.sHtML

[U59] PHP：自定义排序
来源：http://m.share.epnwcf.com/Article/details/ghfobauos.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gyobahpna.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fktsv.cn/Article/details/gtunljzxv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.yfazqb.com/Article/details/gmuxkeywv.sHtML

[U61] PHP：正则
来源：http://baike.vehdjk.com/Article/details/guhqnzjcb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.sjlbkw.cn/Article/details/gbkfxxzul.sHtML

[U62] PHP：日期对象
来源：http://www.share.tarul.cn/Article/details/gvwinqvkj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.vehdjk.com/Article/details/gxkszhrnc.sHtML

[U63] PHP：文件读写
来源：http://read.share.sjlbkw.cn/Article/details/gdbrhuieg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.yfazqb.com/Article/details/goataibut.sHtML

[U64] PHP：目录遍历
来源：http://read.share.epnwcf.com/Article/details/gumpdfqkw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.sjlbkw.cn/Article/details/gvynpuobh.sHtML

[U65] PHP：会话
来源：http://read.share.sjlbkw.cn/Article/details/gcoxgygpk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gbasyvnhs.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.bbcook.cn/Article/details/gvnwdggpx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.sjlbkw.cn/Article/details/gribhhcay.sHtML

[U67] PHP：处理文件上传
来源：http://wap.sjlbkw.cn/Article/details/gkvmhhwzh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.sjlbkw.cn/Article/details/ggoobwsup.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.bbcook.cn/Article/details/gsjlfcjjn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.tarul.cn/Article/details/greybnrhs.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.yfazqb.com/Article/details/gimkxhcfm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.tarul.cn/Article/details/gkobdzyhe.sHtML

[U70] PHP：PDO 事务
来源：http://baike.tarul.cn/Article/details/guuwebghr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fktsv.cn/Article/details/gllkglbww.sHtML

[U71] PHP：抛出异常
来源：http://wap.epnwcf.com/Article/details/gpvglequg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.bbcook.cn/Article/details/gqxuoptjc.sHtML

[U72] PHP：写错误日志
来源：http://www.share.tarul.cn/Article/details/ghpypkhji.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.yfazqb.com/Article/details/gdwaggkhm.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fktsv.cn/Article/details/gibifrbud.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.vehdjk.com/Article/details/gazqzmsgs.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.epnwcf.com/Article/details/gypxfoftr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.yfazqb.com/Article/details/ggyokjtbz.sHtML

[U75] PHP：依赖注入
来源：http://wap.tarul.cn/Article/details/ggizuypsq.sHtML

composer require psr/container
来源：http://www.blog.vehdjk.com/Article/details/gveggsnes.sHtML

[U76] PHP：简单路由
来源：http://www.share.vehdjk.com/Article/details/gsbebhths.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.yfazqb.com/Article/details/gpvvvlaqj.sHtML

[U77] PHP：模板渲染
来源：http://baike.vehdjk.com/Article/details/gjzmzfktj.sHtML

composer require twig/twig
来源：http://3g.tarul.cn/Article/details/gfyagbrmz.sHtML

[U78] PHP：单元测试
来源：http://www.share.sjlbkw.cn/Article/details/gcddwqhlx.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fktsv.cn/Article/details/giwslxtuh.sHtML

[U79] PHP：静态分析
来源：http://mobile.epnwcf.com/Article/details/ghsofhehi.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.epnwcf.com/Article/details/gxiuviidy.sHtML

[U80] PHP：代码规范修复
来源：http://3g.vehdjk.com/Article/details/gckplyzuu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.sjlbkw.cn/Article/details/gzovgbcfk.sHtML

[U81] JS：初始化项目
来源：http://blog.sjlbkw.cn/Article/details/gzcgcowpr.sHtML

npm init -y;  npm i express
来源：http://read.share.vehdjk.com/Article/details/giiyxjwah.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fktsv.cn/Article/details/gumqgrprk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.yfazqb.com/Article/details/gmvdevptg.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.yfazqb.com/Article/details/ghyawlmnn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcihgplk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fktsv.cn/Article/details/gzwefgpzf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fktsv.cn/Article/details/gnkeiqrov.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/gqftuzmua.sHtML

a?.b?.c
来源：http://mobile.sjlbkw.cn/Article/details/gfyeybjxh.sHtML

[U86] JS：空值合并
来源：http://www.blog.yfazqb.com/Article/details/gdrdaeovf.sHtML

a ?? b
来源：http://3g.yfazqb.com/Article/details/gpdlgfgbl.sHtML

[U87] JS：解构默认值
来源：http://wap.sjlbkw.cn/Article/details/gjoonsrem.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.sjlbkw.cn/Article/details/gefasizxy.sHtML

[U88] JS：对象展开合并
来源：http://www.share.vehdjk.com/Article/details/gksaygdhb.sHtML

{ ...a, ...b }
来源：http://www.share.vehdjk.com/Article/details/grrwyftxi.sHtML

[U89] JS：数组去重
来源：http://read.share.yfazqb.com/Article/details/gjxtrphth.sHtML

[...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gnpbvefen.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.vehdjk.com/Article/details/gaszkgxho.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gumoqbvpb.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.vehdjk.com/Article/details/gvtbdwnoj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fktsv.cn/Article/details/gxiahwkuz.sHtML

[U92] JS：深拷贝
来源：http://blog.fktsv.cn/Article/details/gjwoqatmw.sHtML

structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gorslnzgj.sHtML

[U93] JS：模板字符串
来源：http://www.blog.epnwcf.com/Article/details/gwquxalya.sHtML

`共 ${n} 条`
来源：http://3g.bbcook.cn/Article/details/gifjretuc.sHtML

[U94] JS：箭头函数
来源：http://wap.epnwcf.com/Article/details/gtvfuvpyp.sHtML

const double = x => x * 2;
来源：http://baike.bbcook.cn/Article/details/gdifuxwtw.sHtML

[U95] JS：Promise 包装
来源：http://mobile.bbcook.cn/Article/details/gaymhnwbx.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.sjlbkw.cn/Article/details/gencbrxep.sHtML

[U96] JS：async/await 与异常
来源：http://baike.yfazqb.com/Article/details/gauamhhsr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/glojjzesu.sHtML

[U97] JS：并发请求
来源：http://blog.fktsv.cn/Article/details/gnfpmjkcr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/ghsenvvou.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.bbcook.cn/Article/details/gixotkgjd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.vehdjk.com/Article/details/geosaonwa.sHtML

[U99] JS：事件监听
来源：http://blog.tarul.cn/Article/details/gbyitjopn.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.sjlbkw.cn/Article/details/gvpqkrnlq.sHtML

[U100] JS：DOM 查询
来源：http://blog.sjlbkw.cn/Article/details/gvhqpjpei.sHtML

document.querySelector(".item")
来源：http://m.share.sjlbkw.cn/Article/details/gntjzgzme.sHtML

[U101] JS：classList 操作
来源：http://read.share.epnwcf.com/Article/details/gztxydwia.sHtML

el.classList.toggle("active")
来源：http://wap.fktsv.cn/Article/details/gnatbcjkj.sHtML

[U102] JS：本地存储
来源：http://baike.sjlbkw.cn/Article/details/gucthucbd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fktsv.cn/Article/details/gyrsmbgxl.sHtML

[U103] JS：定时器
来源：http://blog.yfazqb.com/Article/details/gxlbjrxao.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fktsv.cn/Article/details/gscrkofjf.sHtML

[U104] JS：防抖
来源：http://mobile.fktsv.cn/Article/details/gkikbwipw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gliemechc.sHtML

[U105] JS：节流
来源：http://wap.sjlbkw.cn/Article/details/gfizxmxgo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.sjlbkw.cn/Article/details/golyoxixy.sHtML

[U106] JS：日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gqdrmrmue.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fktsv.cn/Article/details/ggbqpqnta.sHtML

[U107] JS：数字千分位
来源：http://wap.yfazqb.com/Article/details/glqjksych.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gxfpgncqx.sHtML

[U108] JS：随机整数
来源：http://www.share.fktsv.cn/Article/details/gqujmziwi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.epnwcf.com/Article/details/gwwqfapnz.sHtML

[U109] JS：数组分组
来源：http://mobile.vehdjk.com/Article/details/ggctjnpgm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/guqofxgdr.sHtML

[U110] JS：数组分块
来源：http://read.share.tarul.cn/Article/details/gurrxbluj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fktsv.cn/Article/details/gbcrbzvqw.sHtML

[U111] JS：对象转 Map
来源：http://m.share.yfazqb.com/Article/details/gdfufypcu.sHtML

new Map(Object.entries(obj))
来源：http://baike.bbcook.cn/Article/details/garbdbyrg.sHtML

[U112] JS：字符串补位
来源：http://blog.tarul.cn/Article/details/gzeklpjmx.sHtML

"7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gzjidpjdt.sHtML

[U113] JS：正则替换全部
来源：http://read.share.vehdjk.com/Article/details/gmitilosv.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/ghwehqgel.sHtML

[U114] JS：JSON 深比较
来源：http://baike.vehdjk.com/Article/details/gqouziwex.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/gawviyfyd.sHtML

[U115] JS：生成 UUID
来源：http://3g.vehdjk.com/Article/details/glkmcipps.sHtML

crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/ggmzroxnv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.sjlbkw.cn/Article/details/gxwerqifd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.bbcook.cn/Article/details/gpnwqaewr.sHtML

[U117] JS：单元测试
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrfyjsoj.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.vehdjk.com/Article/details/gqdtjijvz.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.epnwcf.com/Article/details/gpepbnhxg.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fktsv.cn/Article/details/gwsozwfcf.sHtML

[U119] JS：生产构建
来源：http://3g.sjlbkw.cn/Article/details/gfeacfitv.sHtML

npx vite build
来源：http://read.share.epnwcf.com/Article/details/gerecmnjb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.tarul.cn/Article/details/gglsdilvf.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fktsv.cn/Article/details/gmijhlulm.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gyjczxoez.sHtML

统计汇总
来源：http://m.share.yfazqb.com/Article/details/gjrzrffky.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjrqjkbol.sHtML

按语言统计（条）：
来源：http://m.share.bbcook.cn/Article/details/gxzggwnaj.sHtML

Python ......... 252
来源：http://wap.tarul.cn/Article/details/gjtregdqy.sHtML

PHP ............ 252
来源：http://www.share.sjlbkw.cn/Article/details/geidfpwbi.sHtML

JavaScript ..... 252
来源：http://3g.fktsv.cn/Article/details/gwfkoypsj.sHtML

TypeScript ..... 212
来源：http://mobile.yfazqb.com/Article/details/gmkdxinsj.sHtML

Java ........... 212
来源：http://mobile.vehdjk.com/Article/details/gnxmukwgb.sHtML

Go ............. 212
来源：http://blog.sjlbkw.cn/Article/details/gnaddahlt.sHtML

Ruby ........... 212
来源：http://mobile.sjlbkw.cn/Article/details/gyckynzsw.sHtML

C# ............. 212
来源：http://m.share.tarul.cn/Article/details/gxfrtkdyz.sHtML

C .............. 30
来源：http://www.blog.tarul.cn/Article/details/gzqyisemo.sHtML

C++ ............ 30
来源：http://mobile.epnwcf.com/Article/details/gadttnoda.sHtML

SQL ............ 90
来源：http://www.share.tarul.cn/Article/details/gdiedtspa.sHtML

Bash ........... 80
来源：http://www.m.share.bbcook.cn/Article/details/garsldcfd.sHtML

Kotlin ......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gkurvnkir.sHtML

Swift .......... 15
来源：http://baike.yfazqb.com/Article/details/gwuzdvbhc.sHtML

Lua ............ 10
来源：http://m.share.vehdjk.com/Article/details/gdunwttba.sHtML

Perl ........... 10
来源：http://www.share.epnwcf.com/Article/details/gqgdvypeo.sHtML

Scala .......... 10
来源：http://read.share.sjlbkw.cn/Article/details/gfrarivcf.sHtML

------------------------------------
来源：http://wap.bbcook.cn/Article/details/gxqvsibtg.sHtML

合计 ........... 2106 条
来源：http://www.share.tarul.cn/Article/details/gcvqyypmq.sHtML

按章节统计：
来源：http://3g.yfazqb.com/Article/details/giifyrkwp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/grtrvqqgs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gnjtwtfcl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gggqmgcyj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.yfazqb.com/Article/details/gooceqyxm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.vehdjk.com/Article/details/gxrlkjeel.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.sjlbkw.cn/Article/details/guxtcweby.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gkljfdnqe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.sjlbkw.cn/Article/details/gdbgcaozc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gdupdwxld.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.bbcook.cn/Article/details/gjcjpwnzu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/grxgtjoas.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gxpspgyra.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/goawregwr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/ggwnuvasr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.epnwcf.com/Article/details/ghvrsgdmu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gdbfswjww.sHtML

Q SQL 专题                              90
来源：http://www.m.share.yfazqb.com/Article/details/geqiemnvu.sHtML

R Bash 专题                             80
来源：http://www.share.epnwcf.com/Article/details/gyupuyjuk.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.sjlbkw.cn/Article/details/gxllznsnz.sHtML

T 其他语言补充                          60
来源：http://wap.sjlbkw.cn/Article/details/ggcvldyqg.sHtML

U 高频实用片段                         120
来源：http://www.m.share.yfazqb.com/Article/details/gmbtogele.sHtML

------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gcbdkirqv.sHtML

合计                                  2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gykafudmx.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gfdyjhzlz.sHtML

使用提醒
来源：http://baike.fktsv.cn/Article/details/gbozskkys.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gsvgljorn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.sjlbkw.cn/Article/details/ghjlkvemq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.sjlbkw.cn/Article/details/gnkvalqbj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.vehdjk.com/Article/details/ggdkdkxkp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.sjlbkw.cn/Article/details/gmrqhmuyd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.epnwcf.com/Article/details/gyowogcje.sHtML

—— 文件结束 ——
来源：http://www.blog.fktsv.cn/Article/details/genixqtnt.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnthhleer.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fktsv.cn/Article/details/guvriicpi.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.yfazqb.com/Article/details/gnlpfajkh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gebvfthez.sHtML

【收录内容】
来源：http://baike.sjlbkw.cn/Article/details/gelpmkjwh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.yfazqb.com/Article/details/gueeuonyv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.bbcook.cn/Article/details/gtcmmvzhl.sHtML

SQL · Bash · C · C++
来源：http://blog.epnwcf.com/Article/details/gdpjhfcap.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.sjlbkw.cn/Article/details/geofbrjzq.sHtML

【使用说明】
来源：http://wap.sjlbkw.cn/Article/details/ghcpeugqw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.yfazqb.com/Article/details/gbvgbvfcm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fktsv.cn/Article/details/gcjqrgkef.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.sjlbkw.cn/Article/details/garzpuacr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.tarul.cn/Article/details/gvkljnlek.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.epnwcf.com/Article/details/gjinlycau.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fktsv.cn/Article/details/ggthafmon.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.yfazqb.com/Article/details/gypmzjusw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.epnwcf.com/Article/details/ginnwtjpl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.bbcook.cn/Article/details/gbsheshzg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fktsv.cn/Article/details/gmhdckpif.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.yfazqb.com/Article/details/gxflevfik.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.epnwcf.com/Article/details/gataywzas.sHtML

【文件统计】
来源：http://www.m.share.sjlbkw.cn/Article/details/gpckeijfz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.epnwcf.com/Article/details/gvzchhyyn.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gyshkxidk.sHtML

目  录
来源：http://3g.fktsv.cn/Article/details/gixlnzohd.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gdckvnibh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.tarul.cn/Article/details/gbxozugph.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.vehdjk.com/Article/details/goqyzufhi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fktsv.cn/Article/details/gxmbzinkq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.tarul.cn/Article/details/gawunqida.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.epnwcf.com/Article/details/gysmbhzft.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.epnwcf.com/Article/details/gfnfxqumq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fktsv.cn/Article/details/gabysjkcg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.bbcook.cn/Article/details/gnkuorvhc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gdsdcyhjh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.bbcook.cn/Article/details/gehsplbir.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gkcuthyop.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/gthzvsljc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/goktypqef.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gwxihgfub.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.tarul.cn/Article/details/gjkitceky.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gcqltqiex.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.bbcook.cn/Article/details/gepthvjna.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.yfazqb.com/Article/details/gxbsynktp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.epnwcf.com/Article/details/gegwyhrbv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.bbcook.cn/Article/details/gankotqvv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.sjlbkw.cn/Article/details/gqxbggvka.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gelbbmvrc.sHtML

A. 基础语法与类型
来源：http://wap.fktsv.cn/Article/details/gvcaodzxv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gizxdclto.sHtML

[A01] Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/glsoolwyd.sHtML

Py:   print("Hello, World!")
来源：http://blog.bbcook.cn/Article/details/gnwklfwjx.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fktsv.cn/Article/details/gghnqnfwy.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gsxdgaygr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fktsv.cn/Article/details/gcotnvpjy.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/gdmwsgzck.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.sjlbkw.cn/Article/details/glacattce.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.yfazqb.com/Article/details/gibcxwyuw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/gasufmtjb.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.tarul.cn/Article/details/gopvwvyeq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.yfazqb.com/Article/details/gilfdmkxo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.tarul.cn/Article/details/gewhvmamj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fktsv.cn/Article/details/gyzfaqqdj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fktsv.cn/Article/details/gdfxnisux.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.yfazqb.com/Article/details/govwbeeyr.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fktsv.cn/Article/details/gxtpesuvz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fktsv.cn/Article/details/gjdtgyymm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.sjlbkw.cn/Article/details/gkdlxsagh.sHtML

[A03] 常量定义
来源：http://baike.bbcook.cn/Article/details/gscrqgbwz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.epnwcf.com/Article/details/geitjuhll.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gvhrcacti.sHtML

JS:   const PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/ggzvpkukm.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gefdxkfck.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gsvzezynt.sHtML

Go:   const PI = 3.14159
来源：http://wap.bbcook.cn/Article/details/gahihiifq.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.yfazqb.com/Article/details/gaunsqklk.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gfjfesppr.sHtML

[A04] 判断变量类型
来源：http://read.share.bbcook.cn/Article/details/gqmjnyelb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.vehdjk.com/Article/details/glxhpnjxx.sHtML


<!-- 参考信息 -->