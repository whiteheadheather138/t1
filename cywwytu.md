代发 wailian999

[U47] PHP：联合类型
来源：http://mobile.vehdjk.com/Article/details/gfeehbchh.sHtML

int|string $id
来源：http://www.share.vehdjk.com/Article/details/gbkuepwht.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fktsv.cn/Article/details/gudhvnfcc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.bbcook.cn/Article/details/grlzopiku.sHtML

[U49] PHP：只读属性
来源：http://baike.yfazqb.com/Article/details/gjfxbxtcc.sHtML

public readonly string $name
来源：http://mobile.bbcook.cn/Article/details/gktprwfnh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjacfyun.sHtML

public function __construct(private int $id) {}
来源：http://wap.fktsv.cn/Article/details/gcbktzwbt.sHtML

[U51] PHP：数组解构
来源：http://www.share.bbcook.cn/Article/details/gjdolzbej.sHtML

[$a, $b] = $arr;
来源：http://baike.fktsv.cn/Article/details/gwiwhmeaa.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdesaenn.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.yfazqb.com/Article/details/gcdcnxgid.sHtML

[U53] PHP：空合并运算符
来源：http://blog.tarul.cn/Article/details/gbcajzblg.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fktsv.cn/Article/details/gxoevfshf.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.tarul.cn/Article/details/gqzfqwdnq.sHtML

$obj?->method()
来源：http://m.share.bbcook.cn/Article/details/gfwdtvcwt.sHtML

[U55] PHP：match 表达式
来源：http://mobile.bbcook.cn/Article/details/gvnyhoqwr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/gwvjnfhlq.sHtML

[U56] PHP：命名参数
来源：http://read.share.yfazqb.com/Article/details/gfjpeyged.sHtML

f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/ggxcegneo.sHtML

[U57] PHP：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gskayunep.sHtML

"值: {$a}"
来源：http://read.share.yfazqb.com/Article/details/ggzooqljw.sHtML

[U58] PHP：数组三件套
来源：http://blog.tarul.cn/Article/details/ggyayupna.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.epnwcf.com/Article/details/ghapxcjyd.sHtML

[U59] PHP：自定义排序
来源：http://blog.epnwcf.com/Article/details/gtgbzbvsn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.tarul.cn/Article/details/gybcfjoqp.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.epnwcf.com/Article/details/gmzlaybme.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.tarul.cn/Article/details/gzkqulviu.sHtML

[U61] PHP：正则
来源：http://3g.bbcook.cn/Article/details/gzlpsnzbd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/gefckphhw.sHtML

[U62] PHP：日期对象
来源：http://mobile.tarul.cn/Article/details/gubcsoyhe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.epnwcf.com/Article/details/gmbjgpmsc.sHtML

[U63] PHP：文件读写
来源：http://www.share.sjlbkw.cn/Article/details/gviythzmx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.vehdjk.com/Article/details/gjifbvwnu.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.bbcook.cn/Article/details/gtqdveans.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.epnwcf.com/Article/details/gsvgvbzng.sHtML

[U65] PHP：会话
来源：http://blog.epnwcf.com/Article/details/gdrvqhtym.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.epnwcf.com/Article/details/gvfkopczq.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.vehdjk.com/Article/details/ggarcxerb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.yfazqb.com/Article/details/gjnpqvaie.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.epnwcf.com/Article/details/gomvrsneu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.vehdjk.com/Article/details/gkbtduiwa.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.bbcook.cn/Article/details/gbkntsjbm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.yfazqb.com/Article/details/gdvmswcni.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.vehdjk.com/Article/details/glstzfjda.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.sjlbkw.cn/Article/details/gyqlekpbv.sHtML

[U70] PHP：PDO 事务
来源：http://baike.tarul.cn/Article/details/gpwcrdowr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.tarul.cn/Article/details/glucyyaxg.sHtML

[U71] PHP：抛出异常
来源：http://baike.sjlbkw.cn/Article/details/ggpywkjzc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.epnwcf.com/Article/details/gcmhdvixi.sHtML

[U72] PHP：写错误日志
来源：http://3g.vehdjk.com/Article/details/gegvmadiq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.yfazqb.com/Article/details/gkleuofna.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.vehdjk.com/Article/details/griyebmdu.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fktsv.cn/Article/details/gykgdmaay.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.tarul.cn/Article/details/gedjqeiuq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.vehdjk.com/Article/details/gvlyiigze.sHtML

[U75] PHP：依赖注入
来源：http://wap.epnwcf.com/Article/details/gnkmvcaqu.sHtML

composer require psr/container
来源：http://www.m.share.vehdjk.com/Article/details/gfbpfyiuk.sHtML

[U76] PHP：简单路由
来源：http://baike.yfazqb.com/Article/details/gaoijuize.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsopdmir.sHtML

[U77] PHP：模板渲染
来源：http://baike.bbcook.cn/Article/details/glbejecka.sHtML

composer require twig/twig
来源：http://www.share.yfazqb.com/Article/details/gcgeebzlg.sHtML

[U78] PHP：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gehyxhpuw.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.epnwcf.com/Article/details/gygbuqjbg.sHtML

[U79] PHP：静态分析
来源：http://baike.yfazqb.com/Article/details/gljcoztrf.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.vehdjk.com/Article/details/gdbpoqmkq.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.yfazqb.com/Article/details/gxmeydlmp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.yfazqb.com/Article/details/googrsxou.sHtML

[U81] JS：初始化项目
来源：http://www.share.yfazqb.com/Article/details/gutegslbx.sHtML

npm init -y;  npm i express
来源：http://m.share.sjlbkw.cn/Article/details/gufqhtgix.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.sjlbkw.cn/Article/details/gebhbdgoe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.bbcook.cn/Article/details/guwbjwnfo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.vehdjk.com/Article/details/gxbkptevo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fktsv.cn/Article/details/gsqdhummx.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.sjlbkw.cn/Article/details/gebcayijp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.epnwcf.com/Article/details/gsuzilatq.sHtML

[U85] JS：可选链
来源：http://wap.vehdjk.com/Article/details/giopbjwvr.sHtML

a?.b?.c
来源：http://read.share.vehdjk.com/Article/details/gajjjgifd.sHtML

[U86] JS：空值合并
来源：http://mobile.bbcook.cn/Article/details/gflixcvnf.sHtML

a ?? b
来源：http://blog.fktsv.cn/Article/details/gefuxvdoe.sHtML

[U87] JS：解构默认值
来源：http://blog.fktsv.cn/Article/details/gdjjembig.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/gyklsaece.sHtML

[U88] JS：对象展开合并
来源：http://3g.bbcook.cn/Article/details/gzyjuywtq.sHtML

{ ...a, ...b }
来源：http://blog.epnwcf.com/Article/details/gkjhbzmmm.sHtML

[U89] JS：数组去重
来源：http://read.share.bbcook.cn/Article/details/gkazxeqbb.sHtML

[...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gnuazheac.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.vehdjk.com/Article/details/gmujfrocq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gxtndbypm.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fktsv.cn/Article/details/gjnyxijez.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.vehdjk.com/Article/details/gzvdatquo.sHtML

[U92] JS：深拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gmdbplylz.sHtML

structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/geaerzirc.sHtML

[U93] JS：模板字符串
来源：http://baike.vehdjk.com/Article/details/gnarpyoep.sHtML

`共 ${n} 条`
来源：http://www.m.share.epnwcf.com/Article/details/gkzgzsqqf.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/gcekkykzz.sHtML

const double = x => x * 2;
来源：http://baike.epnwcf.com/Article/details/gpxtipjuj.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.vehdjk.com/Article/details/gozehybco.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.epnwcf.com/Article/details/gkckuowgc.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.yfazqb.com/Article/details/gsyhxlphp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/ghtzwmirl.sHtML

[U97] JS：并发请求
来源：http://baike.yfazqb.com/Article/details/gmxutswbn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gdfbdyqwl.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.bbcook.cn/Article/details/gyixadzdy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.bbcook.cn/Article/details/gcazbpnpq.sHtML

[U99] JS：事件监听
来源：http://www.m.share.epnwcf.com/Article/details/glyorwvhd.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.yfazqb.com/Article/details/ghunkoquk.sHtML

[U100] JS：DOM 查询
来源：http://www.share.yfazqb.com/Article/details/gpjfpqtyj.sHtML

document.querySelector(".item")
来源：http://www.blog.yfazqb.com/Article/details/gdtyoinck.sHtML

[U101] JS：classList 操作
来源：http://www.share.yfazqb.com/Article/details/gtalqdozt.sHtML

el.classList.toggle("active")
来源：http://read.share.fktsv.cn/Article/details/gfkmilbzd.sHtML

[U102] JS：本地存储
来源：http://baike.epnwcf.com/Article/details/gzhzhhzhj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.sjlbkw.cn/Article/details/guiktztvw.sHtML

[U103] JS：定时器
来源：http://blog.epnwcf.com/Article/details/gnczfgjwd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.bbcook.cn/Article/details/gugvpbdij.sHtML

[U104] JS：防抖
来源：http://www.m.share.yfazqb.com/Article/details/gxltznimg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gewracgyz.sHtML

[U105] JS：节流
来源：http://3g.vehdjk.com/Article/details/gsujhbggc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.tarul.cn/Article/details/givkgvtwf.sHtML

[U106] JS：日期格式化
来源：http://www.share.fktsv.cn/Article/details/gnxqibked.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.vehdjk.com/Article/details/gxritclke.sHtML

[U107] JS：数字千分位
来源：http://wap.tarul.cn/Article/details/gctgpjtvc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.epnwcf.com/Article/details/gfjapbidq.sHtML

[U108] JS：随机整数
来源：http://www.blog.fktsv.cn/Article/details/gmfdqxisv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.epnwcf.com/Article/details/gmfhdevxe.sHtML

[U109] JS：数组分组
来源：http://wap.vehdjk.com/Article/details/gjpopgoxi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gilapnjye.sHtML

[U110] JS：数组分块
来源：http://baike.vehdjk.com/Article/details/girusyodh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.vehdjk.com/Article/details/glutayyvc.sHtML

[U111] JS：对象转 Map
来源：http://3g.yfazqb.com/Article/details/gjchawetf.sHtML

new Map(Object.entries(obj))
来源：http://m.share.sjlbkw.cn/Article/details/glqavsdok.sHtML

[U112] JS：字符串补位
来源：http://wap.vehdjk.com/Article/details/gxhabnmfv.sHtML

"7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gzywmihbz.sHtML

[U113] JS：正则替换全部
来源：http://www.share.yfazqb.com/Article/details/gjxcjztbd.sHtML

s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gvhmtueiy.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.epnwcf.com/Article/details/grfoncvxj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/gmvppepff.sHtML

[U115] JS：生成 UUID
来源：http://blog.epnwcf.com/Article/details/gzlttcuga.sHtML

crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gxgmghlpw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fktsv.cn/Article/details/ggxdmzjvw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fktsv.cn/Article/details/gunkspbme.sHtML

[U117] JS：单元测试
来源：http://www.blog.vehdjk.com/Article/details/gswfpcpwc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fktsv.cn/Article/details/gpscezoep.sHtML

[U118] JS：开发服务器
来源：http://3g.epnwcf.com/Article/details/gepnacxvk.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.sjlbkw.cn/Article/details/gfrhbfmkh.sHtML

[U119] JS：生产构建
来源：http://wap.fktsv.cn/Article/details/gkncwqngq.sHtML

npx vite build
来源：http://www.blog.vehdjk.com/Article/details/geyrnytlb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.tarul.cn/Article/details/gsunukwpl.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.tarul.cn/Article/details/gwsnoxsrg.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gbbabkgvv.sHtML

统计汇总
来源：http://read.share.epnwcf.com/Article/details/glnruhdrx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/giyfhknfg.sHtML

按语言统计（条）：
来源：http://wap.vehdjk.com/Article/details/goyjvnaoh.sHtML

Python ......... 252
来源：http://read.share.vehdjk.com/Article/details/ggyeljsmb.sHtML

PHP ............ 252
来源：http://blog.bbcook.cn/Article/details/gaveejsbt.sHtML

JavaScript ..... 252
来源：http://baike.sjlbkw.cn/Article/details/gfkryeegu.sHtML

TypeScript ..... 212
来源：http://www.blog.vehdjk.com/Article/details/giyxdwvxe.sHtML

Java ........... 212
来源：http://mobile.yfazqb.com/Article/details/gnzilpxod.sHtML

Go ............. 212
来源：http://baike.epnwcf.com/Article/details/gokhkupun.sHtML

Ruby ........... 212
来源：http://www.share.yfazqb.com/Article/details/gvakfsiaj.sHtML

C# ............. 212
来源：http://www.share.fktsv.cn/Article/details/gkbmrjwst.sHtML

C .............. 30
来源：http://www.blog.tarul.cn/Article/details/gxzlcfcsy.sHtML

C++ ............ 30
来源：http://mobile.tarul.cn/Article/details/gwziguwsf.sHtML

SQL ............ 90
来源：http://baike.yfazqb.com/Article/details/gwnkhhuao.sHtML

Bash ........... 80
来源：http://read.share.fktsv.cn/Article/details/grbhosset.sHtML

Kotlin ......... 15
来源：http://read.share.sjlbkw.cn/Article/details/gszbwcxwi.sHtML

Swift .......... 15
来源：http://read.share.bbcook.cn/Article/details/glidhcfco.sHtML

Lua ............ 10
来源：http://m.share.sjlbkw.cn/Article/details/gchrldgqg.sHtML

Perl ........... 10
来源：http://3g.vehdjk.com/Article/details/gllygverr.sHtML

Scala .......... 10
来源：http://3g.tarul.cn/Article/details/guotwlgvw.sHtML

------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gjpftvqqi.sHtML

合计 ........... 2106 条
来源：http://mobile.vehdjk.com/Article/details/gpdechrrv.sHtML

按章节统计：
来源：http://m.share.bbcook.cn/Article/details/gezunymux.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.bbcook.cn/Article/details/gnboefdrj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gjdystqsx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/grvahowvt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.yfazqb.com/Article/details/gsawxvnep.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.vehdjk.com/Article/details/gydxfcspg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.vehdjk.com/Article/details/gtkayefxm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/gaehcpcse.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/gnioznywg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gylhgqneq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.yfazqb.com/Article/details/gozlnhuip.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/ghovdodgb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gelqqnhrf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gpepswnoy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fktsv.cn/Article/details/gyishznyd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.bbcook.cn/Article/details/gbupivtyu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gtpfiuboq.sHtML

Q SQL 专题                              90
来源：http://mobile.bbcook.cn/Article/details/gzjsdqgqw.sHtML

R Bash 专题                             80
来源：http://mobile.vehdjk.com/Article/details/gorvyeykv.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.yfazqb.com/Article/details/ghqegueoz.sHtML

T 其他语言补充                          60
来源：http://blog.tarul.cn/Article/details/gmyufjdrk.sHtML

U 高频实用片段                         120
来源：http://baike.tarul.cn/Article/details/gfrmbvzuu.sHtML

------------------------------------
来源：http://mobile.epnwcf.com/Article/details/ggtfogihy.sHtML

合计                                  2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdxlohld.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gvcbnsske.sHtML

使用提醒
来源：http://wap.bbcook.cn/Article/details/ghmdofpbj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gjqcbtsqn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.bbcook.cn/Article/details/gmgrobdwu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.sjlbkw.cn/Article/details/gjpwfcfpe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fktsv.cn/Article/details/gcjhqeych.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.vehdjk.com/Article/details/gdznyohcf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.vehdjk.com/Article/details/gncxgfjie.sHtML

—— 文件结束 ——
来源：http://baike.fktsv.cn/Article/details/grmwixjvd.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gvoqvhjcc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fktsv.cn/Article/details/gnxmzxcvp.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.vehdjk.com/Article/details/gqzwwcfzv.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gowcvtsot.sHtML

【收录内容】
来源：http://www.m.share.yfazqb.com/Article/details/gekopumxg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.epnwcf.com/Article/details/gtnnasafb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.epnwcf.com/Article/details/gumpjagsu.sHtML

SQL · Bash · C · C++
来源：http://mobile.sjlbkw.cn/Article/details/gplfztrgp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.vehdjk.com/Article/details/gsrbtivjd.sHtML

【使用说明】
来源：http://3g.sjlbkw.cn/Article/details/gguxjqncn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.vehdjk.com/Article/details/ghwsviwro.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.tarul.cn/Article/details/gdhpinrzp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.yfazqb.com/Article/details/glivawdfe.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.vehdjk.com/Article/details/gbwndtgun.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.epnwcf.com/Article/details/gznujmfxc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fktsv.cn/Article/details/ghngvdofv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.epnwcf.com/Article/details/gdadytquc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fktsv.cn/Article/details/gxpnlyxro.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.yfazqb.com/Article/details/gipwuguyg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.vehdjk.com/Article/details/gfxevpbjy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.sjlbkw.cn/Article/details/gviiezaup.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.epnwcf.com/Article/details/gqjuupxak.sHtML

【文件统计】
来源：http://www.share.tarul.cn/Article/details/gmmaajcxd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.bbcook.cn/Article/details/gzkfaqpvn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gxgibmtjw.sHtML

目  录
来源：http://www.blog.yfazqb.com/Article/details/gaqsvhhih.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gifmlbill.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.yfazqb.com/Article/details/gubqdwuay.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.vehdjk.com/Article/details/gdxcjnlmp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.sjlbkw.cn/Article/details/grraqwadu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.bbcook.cn/Article/details/gsmwapqrg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fktsv.cn/Article/details/gpjiwlzvn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fktsv.cn/Article/details/gjfamthpd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/gflzyvyck.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gfxklisqc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gculnmayh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.epnwcf.com/Article/details/guyzfnxtq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gzurftodf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gspeieghv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/guwxtqiqx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.epnwcf.com/Article/details/gkbeuommm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fktsv.cn/Article/details/gtxwntoeb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gkpzqouxo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.vehdjk.com/Article/details/gkhbtlxej.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.fktsv.cn/Article/details/gfoypcdkj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.tarul.cn/Article/details/gvebsrqbt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.sjlbkw.cn/Article/details/ghfszsdsd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.vehdjk.com/Article/details/gdchqqrvr.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/goerfgbmf.sHtML

A. 基础语法与类型
来源：http://m.share.yfazqb.com/Article/details/geuhwqrvh.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grmhlchha.sHtML

[A01] Hello World
来源：http://blog.sjlbkw.cn/Article/details/gyjfzrydt.sHtML

Py:   print("Hello, World!")
来源：http://mobile.sjlbkw.cn/Article/details/ggcvhpkuv.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.epnwcf.com/Article/details/gojqwixgb.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.sjlbkw.cn/Article/details/gcsffkdgi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.sjlbkw.cn/Article/details/gdslbwkll.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/gbbsegpfl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.tarul.cn/Article/details/gcnweomgf.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fktsv.cn/Article/details/gvsgrglav.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/gzxptwhyr.sHtML

[A02] 变量声明与赋值
来源：http://baike.sjlbkw.cn/Article/details/gyuhnsggn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.epnwcf.com/Article/details/gabeyrgqo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.epnwcf.com/Article/details/geswipczf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gfbroymez.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fktsv.cn/Article/details/gbmcbpbjf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.epnwcf.com/Article/details/gznsutwxn.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.sjlbkw.cn/Article/details/gpbkfswop.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.tarul.cn/Article/details/gqpzhilbz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gxudxqxnq.sHtML

[A03] 常量定义
来源：http://baike.vehdjk.com/Article/details/gcazvmytt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.bbcook.cn/Article/details/glfzkwdal.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gbdpbwccr.sHtML

JS:   const PI = 3.14159;
来源：http://wap.tarul.cn/Article/details/gumkaplqr.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gowjzuhdu.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/glocgakbp.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.bbcook.cn/Article/details/glgqyavzv.sHtML

Ruby: PI = 3.14159
来源：http://mobile.bbcook.cn/Article/details/gqyxjvfsf.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/ghxrirhwx.sHtML

[A04] 判断变量类型
来源：http://3g.sjlbkw.cn/Article/details/gowlsuedc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fktsv.cn/Article/details/ggfewvkjj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.sjlbkw.cn/Article/details/gtqmykauq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/gtwmduwmm.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.sjlbkw.cn/Article/details/gwdnsundz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.epnwcf.com/Article/details/gosqbeapx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.bbcook.cn/Article/details/gkxvirnwb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fktsv.cn/Article/details/gyssruoew.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.sjlbkw.cn/Article/details/gwsjbnoyi.sHtML

[A05] 整数除法与取模
来源：http://3g.tarul.cn/Article/details/gspsumrrg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.bbcook.cn/Article/details/gptzcmdps.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.bbcook.cn/Article/details/ghzbpvagp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.tarul.cn/Article/details/getsojaee.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gowbqwgnn.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gtnyplzuf.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/giihyotjp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/gkusbfxmh.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.yfazqb.com/Article/details/gbvqwhcje.sHtML


<!-- 参考信息 -->