代发 wailian999

[U35] Py：发送邮件
来源：http://wap.bbcook.cn/Article/details/gykyzrfrc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.bbcook.cn/Article/details/gpgovcjxp.sHtML

[U36] Py：定时任务
来源：http://mobile.epnwcf.com/Article/details/ggtoogbbk.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.sjlbkw.cn/Article/details/goltlbvxa.sHtML

[U37] Py：读写 Excel
来源：http://m.share.yfazqb.com/Article/details/gawqxyrsq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.tarul.cn/Article/details/gywqslfpc.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.tarul.cn/Article/details/gxqnpebrf.sHtML

Path(__file__).resolve().parent
来源：http://mobile.sjlbkw.cn/Article/details/gscvbkncx.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.epnwcf.com/Article/details/gsjyxgpea.sHtML

sys.stdout.isatty()
来源：http://blog.fktsv.cn/Article/details/grhetgcsq.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.vehdjk.com/Article/details/gfmnnglsi.sHtML

print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/ghptdquqs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.bbcook.cn/Article/details/gsnxdbcar.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.tarul.cn/Article/details/gqfyafuvz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.yfazqb.com/Article/details/gogefgneb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.tarul.cn/Article/details/gyqpbtjdl.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fktsv.cn/Article/details/gpnvlagus.sHtML

namespace App\Http;
来源：http://baike.epnwcf.com/Article/details/gzrtxjglh.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.tarul.cn/Article/details/gwlwbjiph.sHtML

declare(strict_types=1);
来源：http://wap.sjlbkw.cn/Article/details/gxmssfkbg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.yfazqb.com/Article/details/gfxdarfai.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/ggnliwdgs.sHtML

[U46] PHP：可空类型
来源：http://3g.fktsv.cn/Article/details/gjacnubkl.sHtML

?string $name = null
来源：http://www.share.fktsv.cn/Article/details/gbkuziwxe.sHtML

[U47] PHP：联合类型
来源：http://baike.vehdjk.com/Article/details/gjkitizvx.sHtML

int|string $id
来源：http://www.share.sjlbkw.cn/Article/details/gtojlkhxv.sHtML

[U48] PHP：纯枚举
来源：http://3g.bbcook.cn/Article/details/gywhkfgoc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.vehdjk.com/Article/details/gtdtcaqxz.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.epnwcf.com/Article/details/gvonqkebk.sHtML

public readonly string $name
来源：http://m.share.fktsv.cn/Article/details/gnxiwiecp.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.tarul.cn/Article/details/gyhmipsvb.sHtML

public function __construct(private int $id) {}
来源：http://baike.epnwcf.com/Article/details/glgregqlq.sHtML

[U51] PHP：数组解构
来源：http://m.share.fktsv.cn/Article/details/gcpomwirr.sHtML

[$a, $b] = $arr;
来源：http://mobile.tarul.cn/Article/details/gykkzxrwi.sHtML

[U52] PHP：箭头函数
来源：http://mobile.vehdjk.com/Article/details/gpoiutggb.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.yfazqb.com/Article/details/gnfyinpow.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlckrarv.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.sjlbkw.cn/Article/details/ghaqscgjr.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.tarul.cn/Article/details/ggpcjhlev.sHtML

$obj?->method()
来源：http://wap.bbcook.cn/Article/details/gbwoqpwff.sHtML

[U55] PHP：match 表达式
来源：http://m.share.tarul.cn/Article/details/gcszlegna.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.yfazqb.com/Article/details/gshrlaybp.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhuuijbd.sHtML

f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/ggbbqsama.sHtML

[U57] PHP：字符串插值
来源：http://blog.vehdjk.com/Article/details/gbpeeayiv.sHtML

"值: {$a}"
来源：http://baike.tarul.cn/Article/details/ggtozuviv.sHtML

[U58] PHP：数组三件套
来源：http://3g.bbcook.cn/Article/details/gjrpfacps.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.tarul.cn/Article/details/gsqdbdodj.sHtML

[U59] PHP：自定义排序
来源：http://wap.tarul.cn/Article/details/gxfblxofg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/gprhhiewz.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.bbcook.cn/Article/details/gjuzpexxg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.epnwcf.com/Article/details/gtdwvjevr.sHtML

[U61] PHP：正则
来源：http://m.share.sjlbkw.cn/Article/details/ggfoebfpi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.epnwcf.com/Article/details/gxyhtauli.sHtML

[U62] PHP：日期对象
来源：http://3g.vehdjk.com/Article/details/gasbufcov.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.yfazqb.com/Article/details/ghksyxzah.sHtML

[U63] PHP：文件读写
来源：http://www.blog.bbcook.cn/Article/details/gosubsutz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.tarul.cn/Article/details/getalsmxu.sHtML

[U64] PHP：目录遍历
来源：http://wap.epnwcf.com/Article/details/gsmlmmtrk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.yfazqb.com/Article/details/geuuuutyb.sHtML

[U65] PHP：会话
来源：http://www.share.epnwcf.com/Article/details/gjcsfwvlj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gwvdzjgqs.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.vehdjk.com/Article/details/gezojewkh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.sjlbkw.cn/Article/details/gjyxloapq.sHtML

[U67] PHP：处理文件上传
来源：http://blog.epnwcf.com/Article/details/gmhmoidxp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.epnwcf.com/Article/details/glebeqwkc.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fktsv.cn/Article/details/gezeqwzjw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.epnwcf.com/Article/details/gbaiptsfn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmoiselo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.sjlbkw.cn/Article/details/gamyuzqbc.sHtML

[U70] PHP：PDO 事务
来源：http://3g.sjlbkw.cn/Article/details/gmdxmargx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.bbcook.cn/Article/details/gfanjnvii.sHtML

[U71] PHP：抛出异常
来源：http://blog.epnwcf.com/Article/details/gwmovtvcd.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.tarul.cn/Article/details/gkvwzyhkb.sHtML

[U72] PHP：写错误日志
来源：http://wap.yfazqb.com/Article/details/gqtdnygbg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fktsv.cn/Article/details/gmdfkauue.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.tarul.cn/Article/details/gmeixmflb.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.epnwcf.com/Article/details/ghvyihzmg.sHtML

[U74] PHP：读取环境变量
来源：http://blog.epnwcf.com/Article/details/gurnkwzca.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfairuru.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.epnwcf.com/Article/details/ganstqpwp.sHtML

composer require psr/container
来源：http://m.share.tarul.cn/Article/details/gjsddjgin.sHtML

[U76] PHP：简单路由
来源：http://mobile.epnwcf.com/Article/details/gmduvwbsa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.sjlbkw.cn/Article/details/gdymadtks.sHtML

[U77] PHP：模板渲染
来源：http://read.share.yfazqb.com/Article/details/gedhrzwik.sHtML

composer require twig/twig
来源：http://www.blog.epnwcf.com/Article/details/gfzhiacjp.sHtML

[U78] PHP：单元测试
来源：http://www.blog.epnwcf.com/Article/details/gswpunlyz.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.yfazqb.com/Article/details/gaygwnkhd.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.tarul.cn/Article/details/grzyjnmmb.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.yfazqb.com/Article/details/gpdkkyphp.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.vehdjk.com/Article/details/gbehnjfwq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.bbcook.cn/Article/details/gsbfbjgeg.sHtML

[U81] JS：初始化项目
来源：http://read.share.vehdjk.com/Article/details/gztjxtawq.sHtML

npm init -y;  npm i express
来源：http://m.share.epnwcf.com/Article/details/gziugbato.sHtML

[U82] JS：package.json 脚本
来源：http://3g.epnwcf.com/Article/details/gggjsskyj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.epnwcf.com/Article/details/gvvrxjeso.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.bbcook.cn/Article/details/gbsezwmls.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.epnwcf.com/Article/details/gfzofticz.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.vehdjk.com/Article/details/gaisakdoc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.bbcook.cn/Article/details/gkvbzkprr.sHtML

[U85] JS：可选链
来源：http://blog.yfazqb.com/Article/details/gjsiffeke.sHtML

a?.b?.c
来源：http://m.share.vehdjk.com/Article/details/gwmbaejvc.sHtML

[U86] JS：空值合并
来源：http://m.share.yfazqb.com/Article/details/gezyqiome.sHtML

a ?? b
来源：http://www.blog.vehdjk.com/Article/details/gwovrjcpk.sHtML

[U87] JS：解构默认值
来源：http://m.share.sjlbkw.cn/Article/details/gkvxeqvay.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.yfazqb.com/Article/details/gqcppmapn.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fktsv.cn/Article/details/gxevwvbtg.sHtML

{ ...a, ...b }
来源：http://read.share.tarul.cn/Article/details/gukgyjvwu.sHtML

[U89] JS：数组去重
来源：http://blog.tarul.cn/Article/details/gqovtqpia.sHtML

[...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gdmwscfme.sHtML

[U90] JS：数字数组排序
来源：http://www.share.bbcook.cn/Article/details/grhrgbqve.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gawrscsaa.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.bbcook.cn/Article/details/gvqsnknia.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.tarul.cn/Article/details/gpvugxetr.sHtML

[U92] JS：深拷贝
来源：http://mobile.epnwcf.com/Article/details/ghlepfrta.sHtML

structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/gyrddglki.sHtML

[U93] JS：模板字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gyfxshbxy.sHtML

`共 ${n} 条`
来源：http://m.share.vehdjk.com/Article/details/ggdlueqwa.sHtML

[U94] JS：箭头函数
来源：http://baike.vehdjk.com/Article/details/geeeahnvp.sHtML

const double = x => x * 2;
来源：http://read.share.vehdjk.com/Article/details/gfakfgxvm.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.vehdjk.com/Article/details/gdbcgupos.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.tarul.cn/Article/details/gqgfzalsx.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fktsv.cn/Article/details/gibzgckyb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gmgyoxfgm.sHtML

[U97] JS：并发请求
来源：http://www.blog.sjlbkw.cn/Article/details/glerrwnyf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/ghqlhmeos.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.epnwcf.com/Article/details/glgpqubul.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fktsv.cn/Article/details/gyjzwjwob.sHtML

[U99] JS：事件监听
来源：http://www.share.sjlbkw.cn/Article/details/geayqcrhu.sHtML

el.addEventListener("click", e => {})
来源：http://blog.vehdjk.com/Article/details/guafflzxi.sHtML

[U100] JS：DOM 查询
来源：http://mobile.yfazqb.com/Article/details/ggcwuqhgr.sHtML

document.querySelector(".item")
来源：http://blog.epnwcf.com/Article/details/gbuvaujhp.sHtML

[U101] JS：classList 操作
来源：http://3g.bbcook.cn/Article/details/gaebfvuce.sHtML

el.classList.toggle("active")
来源：http://www.m.share.yfazqb.com/Article/details/gchrbayta.sHtML

[U102] JS：本地存储
来源：http://baike.vehdjk.com/Article/details/gnnxiivcz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fktsv.cn/Article/details/gxpvyixpp.sHtML

[U103] JS：定时器
来源：http://mobile.tarul.cn/Article/details/gojxmcdzo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.sjlbkw.cn/Article/details/gajvpkxkj.sHtML

[U104] JS：防抖
来源：http://baike.bbcook.cn/Article/details/gbtzcifvd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/glixgqmoo.sHtML

[U105] JS：节流
来源：http://3g.yfazqb.com/Article/details/gctbsadtw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.bbcook.cn/Article/details/gjlvbpfvv.sHtML

[U106] JS：日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gyftbnkei.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.bbcook.cn/Article/details/gthnqtrrz.sHtML

[U107] JS：数字千分位
来源：http://www.blog.vehdjk.com/Article/details/gjkvzohhb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.epnwcf.com/Article/details/ghwxmyjbc.sHtML

[U108] JS：随机整数
来源：http://baike.fktsv.cn/Article/details/gtqglnrsc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fktsv.cn/Article/details/gjotmjqes.sHtML

[U109] JS：数组分组
来源：http://wap.vehdjk.com/Article/details/gshdmbgpf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/gnfwuakaf.sHtML

[U110] JS：数组分块
来源：http://blog.vehdjk.com/Article/details/gcrnjyabe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.epnwcf.com/Article/details/gpawhjlfj.sHtML

[U111] JS：对象转 Map
来源：http://blog.sjlbkw.cn/Article/details/grncmkrbl.sHtML

new Map(Object.entries(obj))
来源：http://blog.bbcook.cn/Article/details/geeyvfuif.sHtML

[U112] JS：字符串补位
来源：http://mobile.vehdjk.com/Article/details/gpoinwygu.sHtML

"7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gdsufjgtg.sHtML

[U113] JS：正则替换全部
来源：http://blog.sjlbkw.cn/Article/details/gjkfqncqz.sHtML

s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/glplveblw.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.vehdjk.com/Article/details/gdtdilidi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gkmmxtiyj.sHtML

[U115] JS：生成 UUID
来源：http://3g.vehdjk.com/Article/details/grgwikpbr.sHtML

crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gcearwhtx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.epnwcf.com/Article/details/ggaoamkwo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.bbcook.cn/Article/details/ggsinpyps.sHtML

[U117] JS：单元测试
来源：http://mobile.yfazqb.com/Article/details/gzdrjepuy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.vehdjk.com/Article/details/gqtjlvbso.sHtML

[U118] JS：开发服务器
来源：http://m.share.vehdjk.com/Article/details/grqvqpwdw.sHtML

npm i -D vite;  npx vite
来源：http://wap.epnwcf.com/Article/details/ghoqiqqfz.sHtML

[U119] JS：生产构建
来源：http://www.m.share.bbcook.cn/Article/details/gxufbqmms.sHtML

npx vite build
来源：http://mobile.vehdjk.com/Article/details/gilcelfsv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fktsv.cn/Article/details/gqwrdghls.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.yfazqb.com/Article/details/ghiixkfvt.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gptpahcgu.sHtML

统计汇总
来源：http://read.share.vehdjk.com/Article/details/gduxandki.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gsteowmmd.sHtML

按语言统计（条）：
来源：http://3g.vehdjk.com/Article/details/gmzphtzts.sHtML

Python ......... 252
来源：http://baike.fktsv.cn/Article/details/gixywloqn.sHtML

PHP ............ 252
来源：http://mobile.fktsv.cn/Article/details/gxorusyht.sHtML

JavaScript ..... 252
来源：http://m.share.epnwcf.com/Article/details/grepzjswk.sHtML

TypeScript ..... 212
来源：http://mobile.epnwcf.com/Article/details/gqhwndwyu.sHtML

Java ........... 212
来源：http://baike.epnwcf.com/Article/details/gsdhrsjqz.sHtML

Go ............. 212
来源：http://www.blog.epnwcf.com/Article/details/geooxkfqe.sHtML

Ruby ........... 212
来源：http://wap.sjlbkw.cn/Article/details/gaqypomln.sHtML

C# ............. 212
来源：http://3g.fktsv.cn/Article/details/gpfkymchp.sHtML

C .............. 30
来源：http://blog.bbcook.cn/Article/details/giixctekq.sHtML

C++ ............ 30
来源：http://blog.tarul.cn/Article/details/gcmnsqnmw.sHtML

SQL ............ 90
来源：http://read.share.tarul.cn/Article/details/gdfaqanca.sHtML

Bash ........... 80
来源：http://www.m.share.vehdjk.com/Article/details/gmmntaymh.sHtML

Kotlin ......... 15
来源：http://www.blog.fktsv.cn/Article/details/gnqpayeux.sHtML

Swift .......... 15
来源：http://3g.sjlbkw.cn/Article/details/gjvvzccnh.sHtML

Lua ............ 10
来源：http://mobile.vehdjk.com/Article/details/greaenbtr.sHtML

Perl ........... 10
来源：http://m.share.fktsv.cn/Article/details/gxnlbdtjd.sHtML

Scala .......... 10
来源：http://www.share.sjlbkw.cn/Article/details/gyogrvkpe.sHtML

------------------------------------
来源：http://3g.bbcook.cn/Article/details/gcazlkuln.sHtML

合计 ........... 2106 条
来源：http://mobile.bbcook.cn/Article/details/gfyjzrjzd.sHtML

按章节统计：
来源：http://www.share.bbcook.cn/Article/details/gsksayywz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.epnwcf.com/Article/details/gknfwejny.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/guoegmtyo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/gymjpssgi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/gdhjaxtxt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fktsv.cn/Article/details/ghtqceouf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.tarul.cn/Article/details/gdwraoxge.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/gcbamypay.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/gndofprcw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/guklrnotn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.yfazqb.com/Article/details/gwrnmeqio.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gwpbqainc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gbwypxnyn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gchsqzszi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.tarul.cn/Article/details/gzlethmlq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.vehdjk.com/Article/details/gmjptehah.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gmrkxjkpi.sHtML

Q SQL 专题                              90
来源：http://3g.epnwcf.com/Article/details/gjbbvnfyq.sHtML

R Bash 专题                             80
来源：http://wap.sjlbkw.cn/Article/details/ggpgnnwwn.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.sjlbkw.cn/Article/details/gkismfqpb.sHtML

T 其他语言补充                          60
来源：http://3g.sjlbkw.cn/Article/details/gjdojlyls.sHtML

U 高频实用片段                         120
来源：http://mobile.yfazqb.com/Article/details/gouqkoaia.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gyoumgjye.sHtML

合计                                  2106 条
来源：http://blog.epnwcf.com/Article/details/gxhcvlwzy.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gdvufqmyg.sHtML

使用提醒
来源：http://m.share.vehdjk.com/Article/details/gprezjcgv.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gmeuyqsnr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.vehdjk.com/Article/details/gbqpjvpfc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.bbcook.cn/Article/details/gvrcdygqc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.yfazqb.com/Article/details/guopkqvnm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.yfazqb.com/Article/details/gljmaecxc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.yfazqb.com/Article/details/givwicuqf.sHtML

—— 文件结束 ——
来源：http://www.m.share.yfazqb.com/Article/details/gvdzldizy.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/goycwtmcj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.tarul.cn/Article/details/gnwnnooof.sHtML

Common Programming Examples Cheat Book
来源：http://baike.tarul.cn/Article/details/gabgqvpov.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdsuiwyeq.sHtML

【收录内容】
来源：http://blog.tarul.cn/Article/details/gicwzcvlw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.epnwcf.com/Article/details/ggfuzeojv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.yfazqb.com/Article/details/glvvrzbfm.sHtML

SQL · Bash · C · C++
来源：http://www.share.yfazqb.com/Article/details/gjkcwoyiv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.yfazqb.com/Article/details/gdcqamykh.sHtML

【使用说明】
来源：http://www.blog.vehdjk.com/Article/details/grugzchrf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.vehdjk.com/Article/details/glxegwntz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.epnwcf.com/Article/details/gesmzthxn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.sjlbkw.cn/Article/details/gviwsirkl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.epnwcf.com/Article/details/grthtvyhe.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.tarul.cn/Article/details/grxhoxsqm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fktsv.cn/Article/details/gnnqqjhgq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.vehdjk.com/Article/details/gbgivdbry.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.epnwcf.com/Article/details/gcgkqcwmi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.epnwcf.com/Article/details/gblanudqi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.epnwcf.com/Article/details/gxyuotbwe.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.yfazqb.com/Article/details/gyvbjyezn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.tarul.cn/Article/details/ggdwmmlhi.sHtML

【文件统计】
来源：http://www.m.share.tarul.cn/Article/details/ggxlqjrog.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.yfazqb.com/Article/details/gjqhapfaj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/gdpseuamd.sHtML

目  录
来源：http://wap.bbcook.cn/Article/details/gnkkdebtu.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gxttrymwp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/goyaezdby.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/glcmggetf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fktsv.cn/Article/details/godgmojpd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.vehdjk.com/Article/details/gmvvpgdmz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.tarul.cn/Article/details/gcwunpbsw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.bbcook.cn/Article/details/gzjolviij.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gkkruifrg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/gocrflzwe.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/ggboqsxmy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fktsv.cn/Article/details/gnewhzgke.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/gmgjwganl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gjmmkcxau.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gjykprjxj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.bbcook.cn/Article/details/gntyihbom.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fktsv.cn/Article/details/gieksfnzt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gipnliwpe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.bbcook.cn/Article/details/gufskvxnk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.epnwcf.com/Article/details/glnbhmntp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.yfazqb.com/Article/details/gqjpyksvo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/gupfsdwga.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.yfazqb.com/Article/details/gtioiqraf.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gcxghkdvx.sHtML

A. 基础语法与类型
来源：http://wap.sjlbkw.cn/Article/details/gibrteydq.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjxnjclem.sHtML

[A01] Hello World
来源：http://blog.bbcook.cn/Article/details/ggdfwjusl.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.epnwcf.com/Article/details/gdovfcqdp.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fktsv.cn/Article/details/gfqjykujd.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/gwrapmsab.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.yfazqb.com/Article/details/gtjepwbse.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/glhhcvris.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fktsv.cn/Article/details/gpumaoqqn.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.yfazqb.com/Article/details/ghgbspztf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.tarul.cn/Article/details/gswebdqnq.sHtML

[A02] 变量声明与赋值
来源：http://m.share.vehdjk.com/Article/details/gbaujhfhm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.epnwcf.com/Article/details/grtvtgwxp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.vehdjk.com/Article/details/gfuhrstww.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.bbcook.cn/Article/details/gowvrzxkd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fktsv.cn/Article/details/gfbhpkjjz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fktsv.cn/Article/details/gbthqciiz.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.epnwcf.com/Article/details/gcdjohjmj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.bbcook.cn/Article/details/gqeqaoxbq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.tarul.cn/Article/details/goohzmhba.sHtML

[A03] 常量定义
来源：http://baike.sjlbkw.cn/Article/details/gamuukqsr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.vehdjk.com/Article/details/gxaaouzep.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gaoifrinh.sHtML


<!-- 参考信息 -->