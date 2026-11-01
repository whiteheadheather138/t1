代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.share.yfazqb.com/Article/details/gndcefqjr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/geayeiife.sHtML

[U46] PHP：可空类型
来源：http://blog.bbcook.cn/Article/details/gdrnncakh.sHtML

?string $name = null
来源：http://www.share.vehdjk.com/Article/details/gzkcbvalo.sHtML

[U47] PHP：联合类型
来源：http://3g.sjlbkw.cn/Article/details/gdgulaohw.sHtML

int|string $id
来源：http://www.share.tarul.cn/Article/details/gytnvjbcy.sHtML

[U48] PHP：纯枚举
来源：http://wap.sjlbkw.cn/Article/details/gfgjtxmjn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.epnwcf.com/Article/details/gejpssikd.sHtML

[U49] PHP：只读属性
来源：http://m.share.epnwcf.com/Article/details/gxdwodkck.sHtML

public readonly string $name
来源：http://www.share.fktsv.cn/Article/details/glzrxzece.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.tarul.cn/Article/details/glbzxdpwg.sHtML

public function __construct(private int $id) {}
来源：http://m.share.sjlbkw.cn/Article/details/gxtbemfbu.sHtML

[U51] PHP：数组解构
来源：http://m.share.bbcook.cn/Article/details/ggqwofqpf.sHtML

[$a, $b] = $arr;
来源：http://read.share.vehdjk.com/Article/details/gxbpmehuy.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.epnwcf.com/Article/details/gozhjbsfi.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.tarul.cn/Article/details/gnphzwqel.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.epnwcf.com/Article/details/gbclpsyfs.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.tarul.cn/Article/details/gdjkchced.sHtML

[U54] PHP：空安全调用
来源：http://baike.yfazqb.com/Article/details/gchybmlqw.sHtML

$obj?->method()
来源：http://www.m.share.vehdjk.com/Article/details/ghhhydifc.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.yfazqb.com/Article/details/gtpwsfpic.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.sjlbkw.cn/Article/details/gixpqotbl.sHtML

[U56] PHP：命名参数
来源：http://baike.epnwcf.com/Article/details/gdwqgrgks.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gfehzuevk.sHtML

[U57] PHP：字符串插值
来源：http://3g.epnwcf.com/Article/details/gydljslsj.sHtML

"值: {$a}"
来源：http://wap.tarul.cn/Article/details/gwldswhye.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.tarul.cn/Article/details/gpwkclofe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.vehdjk.com/Article/details/gmosrlchv.sHtML

[U59] PHP：自定义排序
来源：http://read.share.sjlbkw.cn/Article/details/ggaifgsqx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/ggrtvdhtn.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.vehdjk.com/Article/details/glxdeimwh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.epnwcf.com/Article/details/gjnozkmxd.sHtML

[U61] PHP：正则
来源：http://read.share.bbcook.cn/Article/details/gwlgjsecg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/gfsbotlhk.sHtML

[U62] PHP：日期对象
来源：http://wap.epnwcf.com/Article/details/gjchidzck.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.epnwcf.com/Article/details/gcjmuivtd.sHtML

[U63] PHP：文件读写
来源：http://m.share.bbcook.cn/Article/details/gtmcpdyak.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.epnwcf.com/Article/details/gqwjyvznt.sHtML

[U64] PHP：目录遍历
来源：http://3g.vehdjk.com/Article/details/ggzhfoyyz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.vehdjk.com/Article/details/gmkkcdscg.sHtML

[U65] PHP：会话
来源：http://wap.tarul.cn/Article/details/geszlomtk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gaatldcus.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.tarul.cn/Article/details/gctwjasws.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.vehdjk.com/Article/details/gknmaifvj.sHtML

[U67] PHP：处理文件上传
来源：http://wap.epnwcf.com/Article/details/gdqoxjeeg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.epnwcf.com/Article/details/gjeianwos.sHtML

[U68] PHP：PDO 连接
来源：http://wap.sjlbkw.cn/Article/details/gbqfbjvov.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.sjlbkw.cn/Article/details/glyoxldoc.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.epnwcf.com/Article/details/gflshgdpj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.tarul.cn/Article/details/gzmrctpgg.sHtML

[U70] PHP：PDO 事务
来源：http://blog.epnwcf.com/Article/details/gobnewmlf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.tarul.cn/Article/details/gpzbadcnh.sHtML

[U71] PHP：抛出异常
来源：http://www.share.epnwcf.com/Article/details/gmnkapzzp.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.sjlbkw.cn/Article/details/gzpxbnvti.sHtML

[U72] PHP：写错误日志
来源：http://m.share.bbcook.cn/Article/details/gjdhhnukc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.tarul.cn/Article/details/goxshgfnr.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.tarul.cn/Article/details/gdbrgzkwb.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.yfazqb.com/Article/details/gukvtfniw.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gwaylzdxt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.epnwcf.com/Article/details/gsllthxja.sHtML

[U75] PHP：依赖注入
来源：http://mobile.vehdjk.com/Article/details/ghmphpoag.sHtML

composer require psr/container
来源：http://www.m.share.bbcook.cn/Article/details/gzzzimbuw.sHtML

[U76] PHP：简单路由
来源：http://blog.bbcook.cn/Article/details/gwxkmtcpj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.tarul.cn/Article/details/gtrsfvrdc.sHtML

[U77] PHP：模板渲染
来源：http://3g.epnwcf.com/Article/details/gfxnvyjuf.sHtML

composer require twig/twig
来源：http://www.m.share.epnwcf.com/Article/details/gqeyslwvj.sHtML

[U78] PHP：单元测试
来源：http://read.share.tarul.cn/Article/details/gwwoyvaxk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.bbcook.cn/Article/details/guitgsewo.sHtML

[U79] PHP：静态分析
来源：http://www.share.sjlbkw.cn/Article/details/ggykgkwya.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.vehdjk.com/Article/details/gxqhlwkyj.sHtML

[U80] PHP：代码规范修复
来源：http://baike.epnwcf.com/Article/details/getidodyi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.tarul.cn/Article/details/gtdidtscc.sHtML

[U81] JS：初始化项目
来源：http://wap.sjlbkw.cn/Article/details/gyqeenisp.sHtML

npm init -y;  npm i express
来源：http://mobile.vehdjk.com/Article/details/gpkvcpqvo.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.vehdjk.com/Article/details/gwjmouspi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.yfazqb.com/Article/details/gbzvhafoi.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.vehdjk.com/Article/details/gmwccxhbl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.tarul.cn/Article/details/gnavjwpmy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrftegyf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.vehdjk.com/Article/details/glfebrktp.sHtML

[U85] JS：可选链
来源：http://3g.vehdjk.com/Article/details/gymfcdyjk.sHtML

a?.b?.c
来源：http://wap.tarul.cn/Article/details/gbpcubslw.sHtML

[U86] JS：空值合并
来源：http://baike.sjlbkw.cn/Article/details/glerahcyo.sHtML

a ?? b
来源：http://www.m.share.tarul.cn/Article/details/gvkerjkjm.sHtML

[U87] JS：解构默认值
来源：http://wap.sjlbkw.cn/Article/details/gurrjhrec.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fktsv.cn/Article/details/gifdqwfuk.sHtML

[U88] JS：对象展开合并
来源：http://mobile.yfazqb.com/Article/details/gihjpueut.sHtML

{ ...a, ...b }
来源：http://3g.yfazqb.com/Article/details/gdxpcpsoz.sHtML

[U89] JS：数组去重
来源：http://m.share.sjlbkw.cn/Article/details/gmsqkjsnt.sHtML

[...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gqgmeipsu.sHtML

[U90] JS：数字数组排序
来源：http://read.share.tarul.cn/Article/details/ghwsicjtx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gxvpfhozf.sHtML

[U91] JS：对象键值遍历
来源：http://blog.epnwcf.com/Article/details/gtugyczhi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fktsv.cn/Article/details/gaqardegr.sHtML

[U92] JS：深拷贝
来源：http://mobile.bbcook.cn/Article/details/gkcnmraaf.sHtML

structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gwwivxokd.sHtML

[U93] JS：模板字符串
来源：http://blog.epnwcf.com/Article/details/gppofijle.sHtML

`共 ${n} 条`
来源：http://read.share.fktsv.cn/Article/details/gjveppfdt.sHtML

[U94] JS：箭头函数
来源：http://baike.sjlbkw.cn/Article/details/gluapfbrv.sHtML

const double = x => x * 2;
来源：http://3g.fktsv.cn/Article/details/glndwilaj.sHtML

[U95] JS：Promise 包装
来源：http://3g.tarul.cn/Article/details/gafakcvef.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.sjlbkw.cn/Article/details/gvoftyszy.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.sjlbkw.cn/Article/details/gpcvpmrqk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gchzxdvus.sHtML

[U97] JS：并发请求
来源：http://blog.epnwcf.com/Article/details/gmirctfmk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gnwhslokk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.bbcook.cn/Article/details/grcroqfkr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.yfazqb.com/Article/details/gvyhvwsmt.sHtML

[U99] JS：事件监听
来源：http://3g.sjlbkw.cn/Article/details/gwquoonrb.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.tarul.cn/Article/details/gbtdufhdv.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fktsv.cn/Article/details/gkzztnpae.sHtML

document.querySelector(".item")
来源：http://www.share.sjlbkw.cn/Article/details/gsgqlpglr.sHtML

[U101] JS：classList 操作
来源：http://www.blog.sjlbkw.cn/Article/details/gngcaqwnv.sHtML

el.classList.toggle("active")
来源：http://www.blog.tarul.cn/Article/details/gwybiraiq.sHtML

[U102] JS：本地存储
来源：http://www.share.yfazqb.com/Article/details/gxlbusmtd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.bbcook.cn/Article/details/gldpvvpcr.sHtML

[U103] JS：定时器
来源：http://www.m.share.vehdjk.com/Article/details/gmgmmjdnj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fktsv.cn/Article/details/gafmiljgz.sHtML

[U104] JS：防抖
来源：http://blog.yfazqb.com/Article/details/gsaigmkze.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gaxpbtfze.sHtML

[U105] JS：节流
来源：http://baike.epnwcf.com/Article/details/gloochjzr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.bbcook.cn/Article/details/gopygwncl.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.tarul.cn/Article/details/ghsswiibn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.bbcook.cn/Article/details/gzlqinahj.sHtML

[U107] JS：数字千分位
来源：http://wap.yfazqb.com/Article/details/gixluhqpu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.tarul.cn/Article/details/gvtvprzsl.sHtML

[U108] JS：随机整数
来源：http://m.share.tarul.cn/Article/details/grvzuyjnp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.bbcook.cn/Article/details/gnmdsnokr.sHtML

[U109] JS：数组分组
来源：http://3g.yfazqb.com/Article/details/gpjniztkg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/gtkjunqwr.sHtML

[U110] JS：数组分块
来源：http://read.share.vehdjk.com/Article/details/gafibaxzi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fktsv.cn/Article/details/gauicxekm.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fktsv.cn/Article/details/giytccxxq.sHtML

new Map(Object.entries(obj))
来源：http://m.share.bbcook.cn/Article/details/gxdzhxrzd.sHtML

[U112] JS：字符串补位
来源：http://www.share.vehdjk.com/Article/details/godorezid.sHtML

"7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gklbcihih.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.epnwcf.com/Article/details/gkqekwhrn.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gkjytasqk.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.yfazqb.com/Article/details/gfavblxwi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/gjgykliga.sHtML

[U115] JS：生成 UUID
来源：http://mobile.yfazqb.com/Article/details/gbddhpfdn.sHtML

crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/galxertzl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.tarul.cn/Article/details/gsstfxfku.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.bbcook.cn/Article/details/ghtpygmbr.sHtML

[U117] JS：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gzvespjfe.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.epnwcf.com/Article/details/gbcbrvcoq.sHtML

[U118] JS：开发服务器
来源：http://m.share.yfazqb.com/Article/details/givebmuqd.sHtML

npm i -D vite;  npx vite
来源：http://3g.yfazqb.com/Article/details/ghybqwaqj.sHtML

[U119] JS：生产构建
来源：http://baike.yfazqb.com/Article/details/gaqnijhgc.sHtML

npx vite build
来源：http://www.share.tarul.cn/Article/details/gzvregnnv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.tarul.cn/Article/details/gwhozkxru.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.epnwcf.com/Article/details/grungtuab.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gbngvfoli.sHtML

统计汇总
来源：http://mobile.bbcook.cn/Article/details/gpwmelaoi.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gbztchznv.sHtML

按语言统计（条）：
来源：http://blog.tarul.cn/Article/details/gdjfnbcys.sHtML

Python ......... 252
来源：http://read.share.vehdjk.com/Article/details/gxifqyshk.sHtML

PHP ............ 252
来源：http://read.share.vehdjk.com/Article/details/gcewqizue.sHtML

JavaScript ..... 252
来源：http://www.blog.vehdjk.com/Article/details/gfzvsdnfb.sHtML

TypeScript ..... 212
来源：http://read.share.bbcook.cn/Article/details/gvmcnwvwa.sHtML

Java ........... 212
来源：http://www.share.vehdjk.com/Article/details/gtgpwwatz.sHtML

Go ............. 212
来源：http://www.blog.sjlbkw.cn/Article/details/gfwvsdrxs.sHtML

Ruby ........... 212
来源：http://read.share.fktsv.cn/Article/details/ggsivdfwq.sHtML

C# ............. 212
来源：http://baike.bbcook.cn/Article/details/galugbttm.sHtML

C .............. 30
来源：http://3g.bbcook.cn/Article/details/golctkmfd.sHtML

C++ ............ 30
来源：http://baike.fktsv.cn/Article/details/gltzeekzg.sHtML

SQL ............ 90
来源：http://www.blog.fktsv.cn/Article/details/gykiatyir.sHtML

Bash ........... 80
来源：http://blog.tarul.cn/Article/details/grldkvfbn.sHtML

Kotlin ......... 15
来源：http://read.share.yfazqb.com/Article/details/gdgoooaxn.sHtML

Swift .......... 15
来源：http://mobile.sjlbkw.cn/Article/details/gxbbpcakp.sHtML

Lua ............ 10
来源：http://www.m.share.epnwcf.com/Article/details/gmiyratoj.sHtML

Perl ........... 10
来源：http://baike.bbcook.cn/Article/details/gdvuynyee.sHtML

Scala .......... 10
来源：http://baike.yfazqb.com/Article/details/gswkghzgb.sHtML

------------------------------------
来源：http://blog.bbcook.cn/Article/details/geydcgewx.sHtML

合计 ........... 2106 条
来源：http://www.share.yfazqb.com/Article/details/gbraliraz.sHtML

按章节统计：
来源：http://read.share.fktsv.cn/Article/details/geatfslvu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/gbwmwvzzo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gwrbulpnh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gdvtzygxa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/gdeqmccaw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.bbcook.cn/Article/details/gcvmxggbn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.sjlbkw.cn/Article/details/geiffajle.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gjlurtvcc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gcmlrozns.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gtpncvlsw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.tarul.cn/Article/details/gualqwffa.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/glhdftpmh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gubojzjde.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gohbirtys.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fktsv.cn/Article/details/ggpufjdjk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.sjlbkw.cn/Article/details/gysinhcti.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gynvehznx.sHtML

Q SQL 专题                              90
来源：http://blog.yfazqb.com/Article/details/goavgyskq.sHtML

R Bash 专题                             80
来源：http://read.share.tarul.cn/Article/details/ghngbwzjz.sHtML

S C / C++ 专题                          60
来源：http://wap.sjlbkw.cn/Article/details/gjhvkxrbu.sHtML

T 其他语言补充                          60
来源：http://www.blog.yfazqb.com/Article/details/gfzeebzjo.sHtML

U 高频实用片段                         120
来源：http://blog.sjlbkw.cn/Article/details/gvfwloiix.sHtML

------------------------------------
来源：http://wap.bbcook.cn/Article/details/gjgvtapdr.sHtML

合计                                  2106 条
来源：http://3g.sjlbkw.cn/Article/details/gnuxeyojm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gryjauvqx.sHtML

使用提醒
来源：http://blog.fktsv.cn/Article/details/gazvhqmzc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/grczbofay.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.tarul.cn/Article/details/gdagkyaqo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.yfazqb.com/Article/details/gnkxmbtns.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.epnwcf.com/Article/details/gtyemswxp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.sjlbkw.cn/Article/details/gfefomsyj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.tarul.cn/Article/details/geolwwwrk.sHtML

—— 文件结束 ——
来源：http://www.blog.bbcook.cn/Article/details/gvktxoxay.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxxyuyqjv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.bbcook.cn/Article/details/gpbjsyoch.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.tarul.cn/Article/details/grplhkusb.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gllbnnayq.sHtML

【收录内容】
来源：http://wap.sjlbkw.cn/Article/details/gencobhxm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.yfazqb.com/Article/details/gyjkcbdkq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fktsv.cn/Article/details/gvjobigkc.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyqrvtlg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.yfazqb.com/Article/details/gipzfbkvo.sHtML

【使用说明】
来源：http://baike.vehdjk.com/Article/details/gjxureyqw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.vehdjk.com/Article/details/gsufxfokf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.epnwcf.com/Article/details/gessojipj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fktsv.cn/Article/details/gezratatp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.yfazqb.com/Article/details/gelfrvqtt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.epnwcf.com/Article/details/gfefilvku.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.sjlbkw.cn/Article/details/gfgmywaxf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.yfazqb.com/Article/details/gvbkqfetw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fktsv.cn/Article/details/ghrktbcuf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fktsv.cn/Article/details/gjamztpgy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.bbcook.cn/Article/details/ghtfvccbr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.bbcook.cn/Article/details/gzxldpxlq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.vehdjk.com/Article/details/ghznazldn.sHtML

【文件统计】
来源：http://wap.bbcook.cn/Article/details/glditddrx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.yfazqb.com/Article/details/gctspwvhq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/gaztehgjg.sHtML

目  录
来源：http://read.share.yfazqb.com/Article/details/gemuwyavg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/glhbeuxyl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fktsv.cn/Article/details/gcapjqmtb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/gobphwxzj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fktsv.cn/Article/details/gukincqnq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.vehdjk.com/Article/details/gqnxzkppt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.tarul.cn/Article/details/gcjrtcqqj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.tarul.cn/Article/details/gzyvwavmu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.sjlbkw.cn/Article/details/gbxxfntiw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/getomzadr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gblzudsqk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.vehdjk.com/Article/details/gmyngnlap.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gmcnhelcz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gxygyhpbk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gktronjgq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.yfazqb.com/Article/details/gqzdkytni.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.tarul.cn/Article/details/guhylmnlk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gwmqyxdnb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.tarul.cn/Article/details/gjofteyvd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.epnwcf.com/Article/details/gqvceutle.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.yfazqb.com/Article/details/goabgpcff.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gkqavrakj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.sjlbkw.cn/Article/details/grtowycuc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjattuyjy.sHtML

A. 基础语法与类型
来源：http://baike.sjlbkw.cn/Article/details/gmahtiknz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gotikxayv.sHtML

[A01] Hello World
来源：http://blog.bbcook.cn/Article/details/gtqkxivzk.sHtML

Py:   print("Hello, World!")
来源：http://wap.sjlbkw.cn/Article/details/gxnzsubko.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.sjlbkw.cn/Article/details/gvelejelh.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gugjaugae.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.bbcook.cn/Article/details/ghponkhyl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.epnwcf.com/Article/details/gbdxlwczc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.tarul.cn/Article/details/gcxtheubo.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.tarul.cn/Article/details/goxpnpthu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.sjlbkw.cn/Article/details/guxrpvfhi.sHtML

[A02] 变量声明与赋值
来源：http://baike.yfazqb.com/Article/details/gvxitsyoe.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.bbcook.cn/Article/details/ggoffnjrw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.sjlbkw.cn/Article/details/ghoykzwbq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.vehdjk.com/Article/details/ggwzcqalt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.tarul.cn/Article/details/gwcbgnkco.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.vehdjk.com/Article/details/gbqxivxii.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.yfazqb.com/Article/details/gkminhsyq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.sjlbkw.cn/Article/details/gfqhihelu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.tarul.cn/Article/details/gumktogpe.sHtML

[A03] 常量定义
来源：http://m.share.sjlbkw.cn/Article/details/gfggrpsaq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.tarul.cn/Article/details/gjyssznpw.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/ggzuuikxf.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gphcbaczb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gnsyietql.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gqduhtlce.sHtML

Go:   const PI = 3.14159
来源：http://mobile.tarul.cn/Article/details/gvngsccuu.sHtML

Ruby: PI = 3.14159
来源：http://m.share.sjlbkw.cn/Article/details/gfmjuzrfj.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gzisxibpg.sHtML

[A04] 判断变量类型
来源：http://www.share.yfazqb.com/Article/details/goaozwocd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fktsv.cn/Article/details/gxacojljh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.vehdjk.com/Article/details/gdkabmcoa.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.tarul.cn/Article/details/gbilpmsev.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fktsv.cn/Article/details/gxkvgtmbd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.vehdjk.com/Article/details/gnirfvvey.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.vehdjk.com/Article/details/gxplkdjnz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.tarul.cn/Article/details/gppfovved.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.epnwcf.com/Article/details/gebceiuwr.sHtML

[A05] 整数除法与取模
来源：http://3g.vehdjk.com/Article/details/goqhzrhzd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.tarul.cn/Article/details/gvihrijcz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fktsv.cn/Article/details/gxtoqtkok.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fktsv.cn/Article/details/gkhoyswgl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/glsvdhnbl.sHtML


<!-- 参考信息 -->