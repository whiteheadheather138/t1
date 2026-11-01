代发 wailian999

[U33] Py：打包发布
来源：http://blog.sjlbkw.cn/Article/details/gwusccejw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.tarul.cn/Article/details/gkwyydphk.sHtML

[U34] Py：判断编码
来源：http://wap.epnwcf.com/Article/details/gyozhysts.sHtML

chardet.detect(raw)
来源：http://baike.bbcook.cn/Article/details/gmavaxkos.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.epnwcf.com/Article/details/gvxepmamx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fktsv.cn/Article/details/gotyorplf.sHtML

[U36] Py：定时任务
来源：http://www.share.bbcook.cn/Article/details/gaumyufhk.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.bbcook.cn/Article/details/gppdvfose.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.tarul.cn/Article/details/gyutevjir.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.tarul.cn/Article/details/gpoepikrr.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.sjlbkw.cn/Article/details/gdbocogqf.sHtML

Path(__file__).resolve().parent
来源：http://mobile.yfazqb.com/Article/details/gtobxztxp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.bbcook.cn/Article/details/gxqzfdlwc.sHtML

sys.stdout.isatty()
来源：http://www.m.share.vehdjk.com/Article/details/gdxhjxbjq.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.vehdjk.com/Article/details/gubjkxqdv.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fktsv.cn/Article/details/gciutjiwt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.yfazqb.com/Article/details/gvfbpnzic.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.bbcook.cn/Article/details/gizmixpnj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.epnwcf.com/Article/details/gdfdgngop.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.yfazqb.com/Article/details/gfbbodffc.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.bbcook.cn/Article/details/ggukcgjqu.sHtML

namespace App\Http;
来源：http://wap.epnwcf.com/Article/details/gooxkgika.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.tarul.cn/Article/details/gcprwupgb.sHtML

declare(strict_types=1);
来源：http://baike.vehdjk.com/Article/details/gkwqpuhki.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.vehdjk.com/Article/details/guutyznua.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gpycpulnk.sHtML

[U46] PHP：可空类型
来源：http://baike.sjlbkw.cn/Article/details/gegdmikrb.sHtML

?string $name = null
来源：http://wap.tarul.cn/Article/details/gtbcaajth.sHtML

[U47] PHP：联合类型
来源：http://3g.tarul.cn/Article/details/gtoqzmypz.sHtML

int|string $id
来源：http://read.share.vehdjk.com/Article/details/giwxpklbl.sHtML

[U48] PHP：纯枚举
来源：http://mobile.yfazqb.com/Article/details/gmpsemevx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.tarul.cn/Article/details/gtlujsafy.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fktsv.cn/Article/details/gyotlqbis.sHtML

public readonly string $name
来源：http://www.blog.yfazqb.com/Article/details/gpbzfzmri.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.yfazqb.com/Article/details/gwgdtwvie.sHtML

public function __construct(private int $id) {}
来源：http://blog.yfazqb.com/Article/details/gptixafaw.sHtML

[U51] PHP：数组解构
来源：http://baike.tarul.cn/Article/details/gltcwbtio.sHtML

[$a, $b] = $arr;
来源：http://read.share.fktsv.cn/Article/details/gxvafarvf.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.epnwcf.com/Article/details/guaafokhv.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.vehdjk.com/Article/details/guqvsuyst.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.yfazqb.com/Article/details/grdmhovbd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.yfazqb.com/Article/details/gygeiorfp.sHtML

[U54] PHP：空安全调用
来源：http://wap.yfazqb.com/Article/details/ggztbintb.sHtML

$obj?->method()
来源：http://www.m.share.yfazqb.com/Article/details/gykhdwhut.sHtML

[U55] PHP：match 表达式
来源：http://wap.sjlbkw.cn/Article/details/geobkcpqw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.epnwcf.com/Article/details/gnbvuzefc.sHtML

[U56] PHP：命名参数
来源：http://baike.epnwcf.com/Article/details/gqbcwymjy.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gvtimecmn.sHtML

[U57] PHP：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gbhhfbdzy.sHtML

"值: {$a}"
来源：http://wap.yfazqb.com/Article/details/gpoqbcbvk.sHtML

[U58] PHP：数组三件套
来源：http://blog.sjlbkw.cn/Article/details/gtohtzlco.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.tarul.cn/Article/details/gmwpsipfg.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.tarul.cn/Article/details/gjjyorzwd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/graduoznh.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.epnwcf.com/Article/details/gddzqdilm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.bbcook.cn/Article/details/godgwnjpt.sHtML

[U61] PHP：正则
来源：http://read.share.tarul.cn/Article/details/gazltolna.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gvbgtsndb.sHtML

[U62] PHP：日期对象
来源：http://m.share.yfazqb.com/Article/details/gawaaaapo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fktsv.cn/Article/details/gzamwwtcd.sHtML

[U63] PHP：文件读写
来源：http://baike.vehdjk.com/Article/details/ghuhobhyl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.yfazqb.com/Article/details/gjzlssdza.sHtML

[U64] PHP：目录遍历
来源：http://blog.epnwcf.com/Article/details/gwjmcqerm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.yfazqb.com/Article/details/gkeyxwdsi.sHtML

[U65] PHP：会话
来源：http://3g.tarul.cn/Article/details/ggulzgmso.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gsnabphix.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.bbcook.cn/Article/details/gpmgajazb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.epnwcf.com/Article/details/gxlvstwcs.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.tarul.cn/Article/details/gckdykstc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fktsv.cn/Article/details/guguzmjrm.sHtML

[U68] PHP：PDO 连接
来源：http://wap.epnwcf.com/Article/details/gxtyhkjgb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.epnwcf.com/Article/details/grounmesf.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.yfazqb.com/Article/details/geqnowjru.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.sjlbkw.cn/Article/details/ghuqzrkhn.sHtML

[U70] PHP：PDO 事务
来源：http://wap.vehdjk.com/Article/details/gqziomugm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.tarul.cn/Article/details/goixdblex.sHtML

[U71] PHP：抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gqfuknkwh.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.sjlbkw.cn/Article/details/gceuvwrqe.sHtML

[U72] PHP：写错误日志
来源：http://baike.fktsv.cn/Article/details/gjhaaaerp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.yfazqb.com/Article/details/ggyyldlpu.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.epnwcf.com/Article/details/gbhlrnxlv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fktsv.cn/Article/details/goebjykew.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.tarul.cn/Article/details/gbrlaqlbo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fktsv.cn/Article/details/gnojsqlfm.sHtML

[U75] PHP：依赖注入
来源：http://read.share.tarul.cn/Article/details/grnbcddpc.sHtML

composer require psr/container
来源：http://wap.yfazqb.com/Article/details/gcoavimsr.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.epnwcf.com/Article/details/ggslqsbzw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fktsv.cn/Article/details/gfgqdnkho.sHtML

[U77] PHP：模板渲染
来源：http://wap.yfazqb.com/Article/details/gcbynteqd.sHtML

composer require twig/twig
来源：http://m.share.vehdjk.com/Article/details/gjppxqjyh.sHtML

[U78] PHP：单元测试
来源：http://www.blog.sjlbkw.cn/Article/details/grppajoko.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.bbcook.cn/Article/details/gsgololky.sHtML

[U79] PHP：静态分析
来源：http://wap.yfazqb.com/Article/details/gdqjsuugy.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.epnwcf.com/Article/details/gnjdjqzui.sHtML

[U80] PHP：代码规范修复
来源：http://wap.bbcook.cn/Article/details/gzgarioxm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fktsv.cn/Article/details/gjhhgocob.sHtML

[U81] JS：初始化项目
来源：http://www.share.sjlbkw.cn/Article/details/gcmoqbwrt.sHtML

npm init -y;  npm i express
来源：http://baike.bbcook.cn/Article/details/ghnyovoti.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.vehdjk.com/Article/details/geinoeoas.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fktsv.cn/Article/details/gjlsbvkgx.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.yfazqb.com/Article/details/gfjvojqqm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/gtrjzvrel.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.vehdjk.com/Article/details/gjgtvugtq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.yfazqb.com/Article/details/gnpgrdzco.sHtML

[U85] JS：可选链
来源：http://wap.sjlbkw.cn/Article/details/ggtrbphtd.sHtML

a?.b?.c
来源：http://m.share.yfazqb.com/Article/details/gblyqucxf.sHtML

[U86] JS：空值合并
来源：http://baike.bbcook.cn/Article/details/gammhjrip.sHtML

a ?? b
来源：http://wap.fktsv.cn/Article/details/gjwbpbhov.sHtML

[U87] JS：解构默认值
来源：http://baike.bbcook.cn/Article/details/gtmhbpdje.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.tarul.cn/Article/details/glwasagni.sHtML

[U88] JS：对象展开合并
来源：http://www.share.yfazqb.com/Article/details/gcrniyddn.sHtML

{ ...a, ...b }
来源：http://m.share.fktsv.cn/Article/details/gsossxdtw.sHtML

[U89] JS：数组去重
来源：http://wap.bbcook.cn/Article/details/gzxvysyas.sHtML

[...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/gnwxdmbzj.sHtML

[U90] JS：数字数组排序
来源：http://blog.sjlbkw.cn/Article/details/gomyjwyhh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gxprncezp.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.epnwcf.com/Article/details/gqkpquwxs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.sjlbkw.cn/Article/details/gbyqqwksl.sHtML

[U92] JS：深拷贝
来源：http://www.blog.yfazqb.com/Article/details/gzaxcaomc.sHtML

structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/ghsgdmzpn.sHtML

[U93] JS：模板字符串
来源：http://wap.bbcook.cn/Article/details/gyroklygw.sHtML

`共 ${n} 条`
来源：http://wap.epnwcf.com/Article/details/gnbazccou.sHtML

[U94] JS：箭头函数
来源：http://baike.bbcook.cn/Article/details/ggmnoiuih.sHtML

const double = x => x * 2;
来源：http://3g.yfazqb.com/Article/details/guhosbtkv.sHtML

[U95] JS：Promise 包装
来源：http://wap.epnwcf.com/Article/details/gyugypwhs.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.epnwcf.com/Article/details/gnmtezhgx.sHtML

[U96] JS：async/await 与异常
来源：http://wap.tarul.cn/Article/details/gzroqesbi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gezxlzudm.sHtML

[U97] JS：并发请求
来源：http://www.blog.vehdjk.com/Article/details/gjqzdofsj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gngwmlwjo.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.bbcook.cn/Article/details/gckafeehg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.yfazqb.com/Article/details/gedhtkoag.sHtML

[U99] JS：事件监听
来源：http://www.blog.yfazqb.com/Article/details/grjsrexcg.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.tarul.cn/Article/details/gnbvivtkf.sHtML

[U100] JS：DOM 查询
来源：http://baike.yfazqb.com/Article/details/ghvsmubda.sHtML

document.querySelector(".item")
来源：http://www.blog.vehdjk.com/Article/details/gixvszonq.sHtML

[U101] JS：classList 操作
来源：http://wap.sjlbkw.cn/Article/details/gezacxgwc.sHtML

el.classList.toggle("active")
来源：http://m.share.fktsv.cn/Article/details/gslovucxk.sHtML

[U102] JS：本地存储
来源：http://baike.tarul.cn/Article/details/gnchfacck.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.sjlbkw.cn/Article/details/gpcfgypzm.sHtML

[U103] JS：定时器
来源：http://baike.bbcook.cn/Article/details/gqmkvreih.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.sjlbkw.cn/Article/details/gisqtkiav.sHtML

[U104] JS：防抖
来源：http://www.m.share.fktsv.cn/Article/details/grjbjbckw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gqskfregv.sHtML

[U105] JS：节流
来源：http://mobile.epnwcf.com/Article/details/gsyzzvsof.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.yfazqb.com/Article/details/gaivrqsfq.sHtML

[U106] JS：日期格式化
来源：http://blog.bbcook.cn/Article/details/gwnpcjhku.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.epnwcf.com/Article/details/gygrvsbmc.sHtML

[U107] JS：数字千分位
来源：http://blog.tarul.cn/Article/details/ggrvcfxsn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fktsv.cn/Article/details/gsvlachww.sHtML

[U108] JS：随机整数
来源：http://www.share.fktsv.cn/Article/details/guharysak.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.epnwcf.com/Article/details/gxsavdhyi.sHtML

[U109] JS：数组分组
来源：http://mobile.bbcook.cn/Article/details/gicdzhlje.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/gqinndifa.sHtML

[U110] JS：数组分块
来源：http://m.share.epnwcf.com/Article/details/gcrgfpxas.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.epnwcf.com/Article/details/gnijmwypn.sHtML

[U111] JS：对象转 Map
来源：http://read.share.vehdjk.com/Article/details/gkljipkwn.sHtML

new Map(Object.entries(obj))
来源：http://baike.bbcook.cn/Article/details/gqzxdiguw.sHtML

[U112] JS：字符串补位
来源：http://baike.fktsv.cn/Article/details/gibzsovzo.sHtML

"7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/glywpkqxb.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.sjlbkw.cn/Article/details/gestatias.sHtML

s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/guursdxhk.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fktsv.cn/Article/details/gbwtnvprr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/grumamiup.sHtML

[U115] JS：生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/gphylxcch.sHtML

crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gdybjxgyt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.bbcook.cn/Article/details/gbwbipnsa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.epnwcf.com/Article/details/gdvckdpvr.sHtML

[U117] JS：单元测试
来源：http://wap.tarul.cn/Article/details/gebuifnjb.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.epnwcf.com/Article/details/gfucscyut.sHtML

[U118] JS：开发服务器
来源：http://3g.epnwcf.com/Article/details/gchfwemjf.sHtML

npm i -D vite;  npx vite
来源：http://mobile.sjlbkw.cn/Article/details/gbvkrfunl.sHtML

[U119] JS：生产构建
来源：http://wap.bbcook.cn/Article/details/gkwuhzovz.sHtML

npx vite build
来源：http://www.blog.bbcook.cn/Article/details/gfccaiqfj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.sjlbkw.cn/Article/details/gpjrmfxdv.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fktsv.cn/Article/details/glcidlxjq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvblobmdc.sHtML

统计汇总
来源：http://www.blog.sjlbkw.cn/Article/details/gyqfloboq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gnwgqqkya.sHtML

按语言统计（条）：
来源：http://mobile.bbcook.cn/Article/details/gsbnouuas.sHtML

Python ......... 252
来源：http://3g.yfazqb.com/Article/details/gqqqpwjgh.sHtML

PHP ............ 252
来源：http://wap.tarul.cn/Article/details/gqfoalufx.sHtML

JavaScript ..... 252
来源：http://mobile.bbcook.cn/Article/details/gzlmnwopp.sHtML

TypeScript ..... 212
来源：http://baike.tarul.cn/Article/details/grrfmymrr.sHtML

Java ........... 212
来源：http://www.share.vehdjk.com/Article/details/gwrlbouyy.sHtML

Go ............. 212
来源：http://baike.tarul.cn/Article/details/ghbcjdduo.sHtML

Ruby ........... 212
来源：http://baike.bbcook.cn/Article/details/gqdxkkdgl.sHtML

C# ............. 212
来源：http://read.share.yfazqb.com/Article/details/gxcrpffjv.sHtML

C .............. 30
来源：http://mobile.sjlbkw.cn/Article/details/gonpbwxbe.sHtML

C++ ............ 30
来源：http://3g.tarul.cn/Article/details/gybusqxxs.sHtML

SQL ............ 90
来源：http://www.blog.fktsv.cn/Article/details/gqmvwhkeq.sHtML

Bash ........... 80
来源：http://www.m.share.sjlbkw.cn/Article/details/gyeadsfqv.sHtML

Kotlin ......... 15
来源：http://3g.epnwcf.com/Article/details/gzbkxyfva.sHtML

Swift .......... 15
来源：http://www.share.fktsv.cn/Article/details/gxljrqwci.sHtML

Lua ............ 10
来源：http://m.share.sjlbkw.cn/Article/details/gqeujnjgr.sHtML

Perl ........... 10
来源：http://baike.vehdjk.com/Article/details/glgzkmzyn.sHtML

Scala .......... 10
来源：http://m.share.vehdjk.com/Article/details/gndksqkps.sHtML

------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gmgrafrug.sHtML

合计 ........... 2106 条
来源：http://m.share.tarul.cn/Article/details/gifubtxtw.sHtML

按章节统计：
来源：http://3g.vehdjk.com/Article/details/gleijwukb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/gcnmexwnl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.vehdjk.com/Article/details/gdtroephb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gdqiypcpk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.sjlbkw.cn/Article/details/gyxuzzkme.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.sjlbkw.cn/Article/details/govndbgpy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.vehdjk.com/Article/details/gicdlptwg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gldegahlg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gwbsnnnws.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/glecyliwk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.yfazqb.com/Article/details/gmlvuldtb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/gcrpktath.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.sjlbkw.cn/Article/details/gaylzoibj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gqjoqsvcd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gozyqoxin.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.yfazqb.com/Article/details/gftaybyxb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gidckudde.sHtML

Q SQL 专题                              90
来源：http://baike.epnwcf.com/Article/details/gbigkiucf.sHtML

R Bash 专题                             80
来源：http://read.share.yfazqb.com/Article/details/gvprfyrml.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.yfazqb.com/Article/details/gudadzlbt.sHtML

T 其他语言补充                          60
来源：http://wap.fktsv.cn/Article/details/gsvrkzrri.sHtML

U 高频实用片段                         120
来源：http://baike.yfazqb.com/Article/details/gspdnyejs.sHtML

------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/grronqyek.sHtML

合计                                  2106 条
来源：http://baike.epnwcf.com/Article/details/givopntzd.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/ghjgrvgcd.sHtML

使用提醒
来源：http://3g.tarul.cn/Article/details/ggdgncunt.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/grxcpzqkt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.tarul.cn/Article/details/gugknurjo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.vehdjk.com/Article/details/gunidueye.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.yfazqb.com/Article/details/gnemmhgbo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.yfazqb.com/Article/details/gdelxwbfc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.vehdjk.com/Article/details/gdsydeiko.sHtML

—— 文件结束 ——
来源：http://baike.sjlbkw.cn/Article/details/ggyczpkqr.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzamjhebl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.yfazqb.com/Article/details/gbvgbkahp.sHtML

Common Programming Examples Cheat Book
来源：http://wap.sjlbkw.cn/Article/details/glrcymfwd.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gdvbknkqu.sHtML

【收录内容】
来源：http://wap.bbcook.cn/Article/details/gngsjhrmv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.sjlbkw.cn/Article/details/geoaawqes.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.bbcook.cn/Article/details/gzctzarqt.sHtML

SQL · Bash · C · C++
来源：http://3g.vehdjk.com/Article/details/gyawtrujg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.yfazqb.com/Article/details/gqwgrlupi.sHtML

【使用说明】
来源：http://m.share.yfazqb.com/Article/details/gdnvmzktt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.sjlbkw.cn/Article/details/gvtbezdtu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.epnwcf.com/Article/details/gojbymrle.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fktsv.cn/Article/details/gkyjvaaio.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.bbcook.cn/Article/details/gzjqrqjhx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.sjlbkw.cn/Article/details/gzdqlpxzs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.yfazqb.com/Article/details/gavusqrsz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.bbcook.cn/Article/details/gypwuxjrh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.vehdjk.com/Article/details/gvleihivt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fktsv.cn/Article/details/gramdabxt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcechwbo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.vehdjk.com/Article/details/gynhtrvyc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.vehdjk.com/Article/details/gfakxvjfc.sHtML

【文件统计】
来源：http://www.m.share.yfazqb.com/Article/details/gaabcljct.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.vehdjk.com/Article/details/gatafcksi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gxsbxmdsk.sHtML

目  录
来源：http://mobile.bbcook.cn/Article/details/gtponbtdd.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gmiuwruey.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.yfazqb.com/Article/details/gkaviximu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.sjlbkw.cn/Article/details/gxoxhzdzh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.epnwcf.com/Article/details/gsaansiah.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.epnwcf.com/Article/details/gjfnvbauh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.vehdjk.com/Article/details/gqspsndxp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.vehdjk.com/Article/details/gnhdrutui.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.tarul.cn/Article/details/gshfpiobj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fktsv.cn/Article/details/gzcaplows.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/gezxrwhnk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.yfazqb.com/Article/details/gmaiqbgxo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/ghdwehgpp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.vehdjk.com/Article/details/gggdhsjpz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/grgwrvupu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fktsv.cn/Article/details/gseavjajn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.yfazqb.com/Article/details/gargryatm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gmyrdliok.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.sjlbkw.cn/Article/details/gdqztwlud.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.epnwcf.com/Article/details/gjfeccuqq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.tarul.cn/Article/details/gywnvlskq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/grbrsbqbh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.sjlbkw.cn/Article/details/gwqniahkj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/grinzvktq.sHtML

A. 基础语法与类型
来源：http://m.share.yfazqb.com/Article/details/gkbgrdroj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkyqnmhxh.sHtML

[A01] Hello World
来源：http://www.blog.epnwcf.com/Article/details/glqummudz.sHtML

Py:   print("Hello, World!")
来源：http://mobile.vehdjk.com/Article/details/ggnoahxbk.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.tarul.cn/Article/details/gpjtweoys.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.epnwcf.com/Article/details/gdasoazvt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.epnwcf.com/Article/details/geqdwpgjm.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.sjlbkw.cn/Article/details/gbdklavwc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.tarul.cn/Article/details/gwzeqcupj.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.bbcook.cn/Article/details/gwbgqilqu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fktsv.cn/Article/details/gkffrdwqg.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.tarul.cn/Article/details/gaukqlokq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fktsv.cn/Article/details/gwkedwjzk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/ggrqlkbkn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.sjlbkw.cn/Article/details/guadpdkmd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.yfazqb.com/Article/details/gxblpsjgg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.vehdjk.com/Article/details/gnhvktcej.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.yfazqb.com/Article/details/gzyltnhpb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.epnwcf.com/Article/details/gsqvqchfa.sHtML


<!-- 参考信息 -->