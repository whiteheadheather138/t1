代发 wailian999

[U37] Py：读写 Excel
来源：http://www.blog.tarul.cn/Article/details/gfkuhlcnv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.tarul.cn/Article/details/gmfoteqgg.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.bbcook.cn/Article/details/gqnqvwckb.sHtML

Path(__file__).resolve().parent
来源：http://wap.tarul.cn/Article/details/gkybidvnx.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.bbcook.cn/Article/details/gawboendg.sHtML

sys.stdout.isatty()
来源：http://www.share.bbcook.cn/Article/details/gdixqdbcr.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.sjlbkw.cn/Article/details/gqbfniqgn.sHtML

print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/gcvfsqfrp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.tarul.cn/Article/details/ghwtpedsg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.vehdjk.com/Article/details/gbadhrvxr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.bbcook.cn/Article/details/gjqvhiktn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.vehdjk.com/Article/details/gijjewind.sHtML

[U43] PHP：声明命名空间
来源：http://blog.epnwcf.com/Article/details/ghgwrrsfx.sHtML

namespace App\Http;
来源：http://read.share.fktsv.cn/Article/details/gmijwspoi.sHtML

[U44] PHP：开启严格类型
来源：http://blog.bbcook.cn/Article/details/geamkzhht.sHtML

declare(strict_types=1);
来源：http://www.blog.tarul.cn/Article/details/gklwsfiiv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.yfazqb.com/Article/details/gptpbingk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gwbecfcbl.sHtML

[U46] PHP：可空类型
来源：http://baike.yfazqb.com/Article/details/ginyezwal.sHtML

?string $name = null
来源：http://www.m.share.tarul.cn/Article/details/gycpjnpbm.sHtML

[U47] PHP：联合类型
来源：http://mobile.epnwcf.com/Article/details/gtztnlnkm.sHtML

int|string $id
来源：http://m.share.bbcook.cn/Article/details/gtfzznste.sHtML

[U48] PHP：纯枚举
来源：http://wap.vehdjk.com/Article/details/ghjqjdglz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fktsv.cn/Article/details/gjazhlfmc.sHtML

[U49] PHP：只读属性
来源：http://mobile.sjlbkw.cn/Article/details/ggochhzta.sHtML

public readonly string $name
来源：http://mobile.vehdjk.com/Article/details/goasjxabd.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.vehdjk.com/Article/details/gshjdiqkn.sHtML

public function __construct(private int $id) {}
来源：http://blog.yfazqb.com/Article/details/gyveiusir.sHtML

[U51] PHP：数组解构
来源：http://m.share.tarul.cn/Article/details/gkuuxwnqi.sHtML

[$a, $b] = $arr;
来源：http://www.blog.vehdjk.com/Article/details/gncutuzaz.sHtML

[U52] PHP：箭头函数
来源：http://wap.yfazqb.com/Article/details/gkebkunsn.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.tarul.cn/Article/details/gdghiieva.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.bbcook.cn/Article/details/gvehftymi.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.sjlbkw.cn/Article/details/gvkxegacl.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.vehdjk.com/Article/details/gnfrtdjyy.sHtML

$obj?->method()
来源：http://www.m.share.epnwcf.com/Article/details/gnpgymptq.sHtML

[U55] PHP：match 表达式
来源：http://3g.bbcook.cn/Article/details/gdyjqyfof.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fktsv.cn/Article/details/gdibxknbz.sHtML

[U56] PHP：命名参数
来源：http://wap.tarul.cn/Article/details/gzwgzufnz.sHtML

f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gawumvdnv.sHtML

[U57] PHP：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gsbsdlxgf.sHtML

"值: {$a}"
来源：http://blog.epnwcf.com/Article/details/gimbradxe.sHtML

[U58] PHP：数组三件套
来源：http://3g.vehdjk.com/Article/details/gsiuvaswq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.bbcook.cn/Article/details/gupyknlyt.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.vehdjk.com/Article/details/gdtynbsdy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gsdtmywog.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.vehdjk.com/Article/details/gyvlkrngr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gstrljjdz.sHtML

[U61] PHP：正则
来源：http://read.share.tarul.cn/Article/details/gvdpvlbzm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.tarul.cn/Article/details/gpdbrnxil.sHtML

[U62] PHP：日期对象
来源：http://wap.tarul.cn/Article/details/gswfjzjab.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fktsv.cn/Article/details/gxclyxlsb.sHtML

[U63] PHP：文件读写
来源：http://www.share.fktsv.cn/Article/details/gigsszjoe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.yfazqb.com/Article/details/goqdngcla.sHtML

[U64] PHP：目录遍历
来源：http://read.share.epnwcf.com/Article/details/gfckfrwif.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.tarul.cn/Article/details/gesbmbqht.sHtML

[U65] PHP：会话
来源：http://wap.tarul.cn/Article/details/gtijajdca.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.vehdjk.com/Article/details/gampjuzld.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fktsv.cn/Article/details/glylgvrit.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.tarul.cn/Article/details/gngwtrxkh.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.vehdjk.com/Article/details/gadoduimm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.sjlbkw.cn/Article/details/gcfoqokzf.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.tarul.cn/Article/details/gwadxprks.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.epnwcf.com/Article/details/guduftzvv.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.epnwcf.com/Article/details/gfqqvsgro.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fktsv.cn/Article/details/gpqqnrzyg.sHtML

[U70] PHP：PDO 事务
来源：http://baike.epnwcf.com/Article/details/gpukboevt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fktsv.cn/Article/details/gnpmjciqk.sHtML

[U71] PHP：抛出异常
来源：http://wap.fktsv.cn/Article/details/geidfznnx.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.yfazqb.com/Article/details/gcltzeard.sHtML

[U72] PHP：写错误日志
来源：http://3g.bbcook.cn/Article/details/gqcskjwjj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.epnwcf.com/Article/details/gnjysnppz.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.bbcook.cn/Article/details/giymntdtm.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.sjlbkw.cn/Article/details/gxhmzhjph.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gxynogogt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvxplvoy.sHtML

[U75] PHP：依赖注入
来源：http://baike.epnwcf.com/Article/details/guqjouvzg.sHtML

composer require psr/container
来源：http://www.share.vehdjk.com/Article/details/gflolyvaq.sHtML

[U76] PHP：简单路由
来源：http://m.share.sjlbkw.cn/Article/details/gjfximvxs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.bbcook.cn/Article/details/gvxzbzshv.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.vehdjk.com/Article/details/girjwligd.sHtML

composer require twig/twig
来源：http://wap.bbcook.cn/Article/details/gblpncnvk.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.tarul.cn/Article/details/gtewquooa.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.sjlbkw.cn/Article/details/gstcxjfor.sHtML

[U79] PHP：静态分析
来源：http://www.blog.yfazqb.com/Article/details/gjloqlncr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.tarul.cn/Article/details/gwkdjmyxj.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fktsv.cn/Article/details/gypfyjwbs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fktsv.cn/Article/details/gzfltiyej.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fktsv.cn/Article/details/gfaykrbam.sHtML

npm init -y;  npm i express
来源：http://blog.sjlbkw.cn/Article/details/glugiroge.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.vehdjk.com/Article/details/gwbukjnsb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.epnwcf.com/Article/details/gfqeeeday.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.sjlbkw.cn/Article/details/guhsdisgl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.yfazqb.com/Article/details/gebhcwlma.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.yfazqb.com/Article/details/gzvbywntc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.yfazqb.com/Article/details/gjbojarly.sHtML

[U85] JS：可选链
来源：http://www.blog.bbcook.cn/Article/details/gwqqitrit.sHtML

a?.b?.c
来源：http://mobile.epnwcf.com/Article/details/gkbhpkyod.sHtML

[U86] JS：空值合并
来源：http://read.share.fktsv.cn/Article/details/gdsgmbmqs.sHtML

a ?? b
来源：http://wap.yfazqb.com/Article/details/ggyhlufkk.sHtML

[U87] JS：解构默认值
来源：http://wap.yfazqb.com/Article/details/ggguttufq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/gqbrowpwi.sHtML

[U88] JS：对象展开合并
来源：http://3g.vehdjk.com/Article/details/goqcirfyh.sHtML

{ ...a, ...b }
来源：http://3g.vehdjk.com/Article/details/gzoytxdhj.sHtML

[U89] JS：数组去重
来源：http://m.share.fktsv.cn/Article/details/gedrxsuab.sHtML

[...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gfofaisek.sHtML

[U90] JS：数字数组排序
来源：http://m.share.yfazqb.com/Article/details/goopxzpgb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gbolmpplz.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.bbcook.cn/Article/details/grswtotro.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.sjlbkw.cn/Article/details/gafamowbs.sHtML

[U92] JS：深拷贝
来源：http://baike.bbcook.cn/Article/details/gtvyryhnq.sHtML

structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/goboxmeyw.sHtML

[U93] JS：模板字符串
来源：http://read.share.fktsv.cn/Article/details/glazjyxet.sHtML

`共 ${n} 条`
来源：http://read.share.yfazqb.com/Article/details/gxbsqwsyc.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/ghmxhgxwy.sHtML

const double = x => x * 2;
来源：http://blog.yfazqb.com/Article/details/gclcflwvk.sHtML

[U95] JS：Promise 包装
来源：http://baike.tarul.cn/Article/details/gbafysncp.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.tarul.cn/Article/details/grcgetmbt.sHtML

[U96] JS：async/await 与异常
来源：http://3g.epnwcf.com/Article/details/gfajbmhpu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gvqwntiyn.sHtML

[U97] JS：并发请求
来源：http://www.m.share.yfazqb.com/Article/details/gfkdvrdpp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/guivhruvi.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.tarul.cn/Article/details/guhxlccwn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.bbcook.cn/Article/details/glgdxwixk.sHtML

[U99] JS：事件监听
来源：http://wap.yfazqb.com/Article/details/gateekbcs.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.tarul.cn/Article/details/gwupshmur.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.vehdjk.com/Article/details/gwfekcear.sHtML

document.querySelector(".item")
来源：http://m.share.bbcook.cn/Article/details/gryxtmflg.sHtML

[U101] JS：classList 操作
来源：http://www.blog.epnwcf.com/Article/details/gaogfevvd.sHtML

el.classList.toggle("active")
来源：http://3g.fktsv.cn/Article/details/gzyfemesc.sHtML

[U102] JS：本地存储
来源：http://3g.bbcook.cn/Article/details/goieyuoac.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.tarul.cn/Article/details/giqrkmozw.sHtML

[U103] JS：定时器
来源：http://www.share.vehdjk.com/Article/details/gqibsrbjz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.yfazqb.com/Article/details/gxtkpvwdc.sHtML

[U104] JS：防抖
来源：http://3g.tarul.cn/Article/details/gsngzutdf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gnzmslrfh.sHtML

[U105] JS：节流
来源：http://www.share.epnwcf.com/Article/details/gfdcrunaf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fktsv.cn/Article/details/gmdziyzvy.sHtML

[U106] JS：日期格式化
来源：http://3g.yfazqb.com/Article/details/gxxlnthwk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.epnwcf.com/Article/details/gbasmfzpf.sHtML

[U107] JS：数字千分位
来源：http://mobile.bbcook.cn/Article/details/gndsqruie.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.sjlbkw.cn/Article/details/ggxeunujh.sHtML

[U108] JS：随机整数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcouakgv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.vehdjk.com/Article/details/gzzdqbdcu.sHtML

[U109] JS：数组分组
来源：http://read.share.sjlbkw.cn/Article/details/gqumcqyjv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.sjlbkw.cn/Article/details/gzfugofdg.sHtML

[U110] JS：数组分块
来源：http://www.blog.bbcook.cn/Article/details/gpbznuvnn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.tarul.cn/Article/details/gltjzjvnp.sHtML

[U111] JS：对象转 Map
来源：http://blog.epnwcf.com/Article/details/gxrwchiqf.sHtML

new Map(Object.entries(obj))
来源：http://blog.fktsv.cn/Article/details/gvuncdetn.sHtML

[U112] JS：字符串补位
来源：http://m.share.vehdjk.com/Article/details/gaisvrbrd.sHtML

"7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gtdwlokel.sHtML

[U113] JS：正则替换全部
来源：http://www.share.bbcook.cn/Article/details/gkayiftel.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gbutugngu.sHtML

[U114] JS：JSON 深比较
来源：http://3g.sjlbkw.cn/Article/details/gnntoljbn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/gjrtfkvbo.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/gmieqsxkw.sHtML

crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gvgbgzccv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fktsv.cn/Article/details/gjhjlvmnn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.vehdjk.com/Article/details/gtyrmttnf.sHtML

[U117] JS：单元测试
来源：http://blog.yfazqb.com/Article/details/glazxllpm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.sjlbkw.cn/Article/details/grvufqlhn.sHtML

[U118] JS：开发服务器
来源：http://www.share.vehdjk.com/Article/details/gjfktxxje.sHtML

npm i -D vite;  npx vite
来源：http://mobile.epnwcf.com/Article/details/gregwwsgd.sHtML

[U119] JS：生产构建
来源：http://wap.epnwcf.com/Article/details/gfbepzcqo.sHtML

npx vite build
来源：http://read.share.bbcook.cn/Article/details/gmuzvncaw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.vehdjk.com/Article/details/goxysceuq.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.epnwcf.com/Article/details/gujbnycbz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/grklrhqdc.sHtML

统计汇总
来源：http://3g.sjlbkw.cn/Article/details/glswnqbgc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbaznsoxn.sHtML

按语言统计（条）：
来源：http://www.share.tarul.cn/Article/details/gfgxqzduk.sHtML

Python ......... 252
来源：http://mobile.epnwcf.com/Article/details/gvqjpvvkv.sHtML

PHP ............ 252
来源：http://wap.yfazqb.com/Article/details/gviwapmxs.sHtML

JavaScript ..... 252
来源：http://3g.vehdjk.com/Article/details/gwgwmcdwa.sHtML

TypeScript ..... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjktardi.sHtML

Java ........... 212
来源：http://mobile.yfazqb.com/Article/details/gcwdpxthq.sHtML

Go ............. 212
来源：http://www.m.share.vehdjk.com/Article/details/gdbzbiqce.sHtML

Ruby ........... 212
来源：http://baike.epnwcf.com/Article/details/gvstyizev.sHtML

C# ............. 212
来源：http://3g.fktsv.cn/Article/details/gsgjhoozd.sHtML

C .............. 30
来源：http://blog.tarul.cn/Article/details/gkhephueg.sHtML

C++ ............ 30
来源：http://read.share.fktsv.cn/Article/details/gbsyfnfbd.sHtML

SQL ............ 90
来源：http://blog.bbcook.cn/Article/details/gclagzaaw.sHtML

Bash ........... 80
来源：http://read.share.sjlbkw.cn/Article/details/gcwhvogsa.sHtML

Kotlin ......... 15
来源：http://baike.epnwcf.com/Article/details/gajoigses.sHtML

Swift .......... 15
来源：http://3g.bbcook.cn/Article/details/gbbxmrsqg.sHtML

Lua ............ 10
来源：http://mobile.fktsv.cn/Article/details/ghcfbahxu.sHtML

Perl ........... 10
来源：http://blog.tarul.cn/Article/details/gwfhsqodg.sHtML

Scala .......... 10
来源：http://mobile.tarul.cn/Article/details/ghnrfinum.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gnxffysrz.sHtML

合计 ........... 2106 条
来源：http://blog.sjlbkw.cn/Article/details/gwysysauf.sHtML

按章节统计：
来源：http://m.share.tarul.cn/Article/details/gkshsvhpt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.tarul.cn/Article/details/grhlzozzh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/gfakckerh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gyuxhjxup.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.tarul.cn/Article/details/gixuyrfci.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.sjlbkw.cn/Article/details/gktabymsv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.sjlbkw.cn/Article/details/gfqgdeypu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/gfbuvvvvw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.bbcook.cn/Article/details/geirmixdq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gcipfdhpe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.vehdjk.com/Article/details/gcyabgltz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gddhegxpz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gbnzsyrdj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gzcgougop.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.sjlbkw.cn/Article/details/gabnjoeql.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.epnwcf.com/Article/details/gqdidiewf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gptcwnzyf.sHtML

Q SQL 专题                              90
来源：http://www.blog.fktsv.cn/Article/details/gvxttplsv.sHtML

R Bash 专题                             80
来源：http://read.share.tarul.cn/Article/details/gjkzvhzcv.sHtML

S C / C++ 专题                          60
来源：http://www.blog.bbcook.cn/Article/details/glwsqwkry.sHtML

T 其他语言补充                          60
来源：http://baike.sjlbkw.cn/Article/details/gtjcdojpc.sHtML

U 高频实用片段                         120
来源：http://www.m.share.vehdjk.com/Article/details/gdetwceno.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/gpfeburxi.sHtML

合计                                  2106 条
来源：http://wap.sjlbkw.cn/Article/details/geozddleh.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/grxarzmod.sHtML

使用提醒
来源：http://www.blog.sjlbkw.cn/Article/details/gwjqgvpbc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gebniwxcq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.tarul.cn/Article/details/gendjqhig.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.bbcook.cn/Article/details/glpwlakkp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.yfazqb.com/Article/details/gqbfpbkhe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.tarul.cn/Article/details/gzwsacvtg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.tarul.cn/Article/details/gepfelrxx.sHtML

—— 文件结束 ——
来源：http://www.blog.vehdjk.com/Article/details/gcadifpnx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gudcrunbw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.yfazqb.com/Article/details/gduzllhja.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.tarul.cn/Article/details/gtxwgollu.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gffviotar.sHtML

【收录内容】
来源：http://read.share.epnwcf.com/Article/details/gkswtypsc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.tarul.cn/Article/details/gvwvcqttz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.tarul.cn/Article/details/gvoxwzlda.sHtML

SQL · Bash · C · C++
来源：http://read.share.sjlbkw.cn/Article/details/gxvwmqbpl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.bbcook.cn/Article/details/gbwtqzure.sHtML

【使用说明】
来源：http://3g.tarul.cn/Article/details/gkdtxjldj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.tarul.cn/Article/details/gwxlucnag.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.yfazqb.com/Article/details/gwnxdgmwc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.tarul.cn/Article/details/gwrtfkdne.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fktsv.cn/Article/details/gzixgyjes.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fktsv.cn/Article/details/gmfrpxdhv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.sjlbkw.cn/Article/details/grrpnhavg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fktsv.cn/Article/details/geirdmxct.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.sjlbkw.cn/Article/details/gcoazxzmg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.yfazqb.com/Article/details/glvivvsyf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.yfazqb.com/Article/details/ghghulket.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.tarul.cn/Article/details/gdcjtncxg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fktsv.cn/Article/details/gbexblzur.sHtML

【文件统计】
来源：http://m.share.bbcook.cn/Article/details/gpwmdemam.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.epnwcf.com/Article/details/gxzsvcatr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gsvnvfxym.sHtML

目  录
来源：http://wap.tarul.cn/Article/details/grifwzdgo.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/gfyojpsqe.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.bbcook.cn/Article/details/gxumsvgxl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.tarul.cn/Article/details/gieonrhtl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.tarul.cn/Article/details/gxrbhsdbx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.tarul.cn/Article/details/gtlphzhqx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fktsv.cn/Article/details/gbhubicfy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fktsv.cn/Article/details/gdqgebemh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.tarul.cn/Article/details/gdpltznzt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.bbcook.cn/Article/details/gpnnfeqpe.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gopgavbiy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.epnwcf.com/Article/details/gsrschrmi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/grrngpgcl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/goazgavig.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.vehdjk.com/Article/details/gqjvgmvte.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.epnwcf.com/Article/details/ghrihjxyj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.vehdjk.com/Article/details/gqljprnpl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/gjldapfnk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.bbcook.cn/Article/details/ggvpwikcw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.yfazqb.com/Article/details/gqthwtbqz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.vehdjk.com/Article/details/gwspmlbkj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gcauyppuy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gpafatmus.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbijozysj.sHtML

A. 基础语法与类型
来源：http://www.share.yfazqb.com/Article/details/gphxgmzwy.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ghdycltng.sHtML

[A01] Hello World
来源：http://www.blog.epnwcf.com/Article/details/gqqbrijft.sHtML

Py:   print("Hello, World!")
来源：http://blog.sjlbkw.cn/Article/details/gnqcfkohe.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.bbcook.cn/Article/details/ghuxniwvz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.bbcook.cn/Article/details/gfgniscef.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.sjlbkw.cn/Article/details/geoufmzxe.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/gambkcirk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fktsv.cn/Article/details/gqhsjuqfz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.vehdjk.com/Article/details/ggoysgohu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.epnwcf.com/Article/details/gunxpjzpt.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fktsv.cn/Article/details/gbmybkizq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.epnwcf.com/Article/details/gcqzpuhee.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.yfazqb.com/Article/details/gxfsxjlxd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gyyxgieko.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.epnwcf.com/Article/details/ghrhkytpw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/gqmifyxby.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.yfazqb.com/Article/details/gavaboqzi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.tarul.cn/Article/details/gcswvxoxm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.tarul.cn/Article/details/grhtllfgw.sHtML

[A03] 常量定义
来源：http://www.blog.yfazqb.com/Article/details/gokzjpooa.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fktsv.cn/Article/details/gxseimoqy.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gsgoopncx.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gmosvxokw.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gptfpzxwb.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gpkiwpmxm.sHtML

Go:   const PI = 3.14159
来源：http://www.share.epnwcf.com/Article/details/gkpgxdxlp.sHtML


<!-- 参考信息 -->