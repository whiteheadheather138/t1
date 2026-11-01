代发 wailian999

[U37] Py：读写 Excel
来源：http://baike.tarul.cn/Article/details/ggbuljlmi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.vehdjk.com/Article/details/gyihaudth.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.yfazqb.com/Article/details/gduqskphr.sHtML

Path(__file__).resolve().parent
来源：http://3g.yfazqb.com/Article/details/gpfovqwka.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.sjlbkw.cn/Article/details/gisjwuusm.sHtML

sys.stdout.isatty()
来源：http://blog.bbcook.cn/Article/details/gpvqybqlm.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.sjlbkw.cn/Article/details/glsbyyjfs.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/gbuxepjim.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.vehdjk.com/Article/details/gqzxpgxek.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.tarul.cn/Article/details/gzhzmrrfo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.yfazqb.com/Article/details/gcgclgjuk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fktsv.cn/Article/details/gledqqgoo.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.tarul.cn/Article/details/gndgvxrgs.sHtML

namespace App\Http;
来源：http://baike.bbcook.cn/Article/details/glaepujxx.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.bbcook.cn/Article/details/gzuzshtns.sHtML

declare(strict_types=1);
来源：http://m.share.bbcook.cn/Article/details/gugrsescu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.tarul.cn/Article/details/grwtgwrig.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/ghpcbielh.sHtML

[U46] PHP：可空类型
来源：http://baike.sjlbkw.cn/Article/details/gkuncmevk.sHtML

?string $name = null
来源：http://blog.epnwcf.com/Article/details/ghtjtmare.sHtML

[U47] PHP：联合类型
来源：http://blog.sjlbkw.cn/Article/details/gcdepowcp.sHtML

int|string $id
来源：http://m.share.tarul.cn/Article/details/golqhezho.sHtML

[U48] PHP：纯枚举
来源：http://read.share.yfazqb.com/Article/details/gzriurndl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.epnwcf.com/Article/details/gddbopiid.sHtML

[U49] PHP：只读属性
来源：http://wap.vehdjk.com/Article/details/gjyfszaqx.sHtML

public readonly string $name
来源：http://3g.fktsv.cn/Article/details/gxqiaijhy.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.vehdjk.com/Article/details/geheuncip.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fktsv.cn/Article/details/glfjsfykk.sHtML

[U51] PHP：数组解构
来源：http://read.share.sjlbkw.cn/Article/details/grghpsyva.sHtML

[$a, $b] = $arr;
来源：http://read.share.fktsv.cn/Article/details/gzhnaunsx.sHtML

[U52] PHP：箭头函数
来源：http://read.share.epnwcf.com/Article/details/gfohfxlzq.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.vehdjk.com/Article/details/gaywhwefj.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.epnwcf.com/Article/details/giuulxfiy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.sjlbkw.cn/Article/details/goolyfsaj.sHtML

[U54] PHP：空安全调用
来源：http://3g.fktsv.cn/Article/details/gtiqazsso.sHtML

$obj?->method()
来源：http://www.blog.epnwcf.com/Article/details/gywyzyftb.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gdoxgoxna.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fktsv.cn/Article/details/gxepvzsso.sHtML

[U56] PHP：命名参数
来源：http://mobile.fktsv.cn/Article/details/gojbbiiug.sHtML

f(a: 1, b: 2)
来源：http://mobile.tarul.cn/Article/details/gyckywnhb.sHtML

[U57] PHP：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gyqxcnfcs.sHtML

"值: {$a}"
来源：http://3g.sjlbkw.cn/Article/details/gunmmkvqo.sHtML

[U58] PHP：数组三件套
来源：http://mobile.yfazqb.com/Article/details/gwoktikmd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.vehdjk.com/Article/details/gfijjthrv.sHtML

[U59] PHP：自定义排序
来源：http://wap.bbcook.cn/Article/details/gugnwpfov.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/glpusyrdq.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.vehdjk.com/Article/details/gjwoknhpf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.sjlbkw.cn/Article/details/gxxuwlbkj.sHtML

[U61] PHP：正则
来源：http://3g.bbcook.cn/Article/details/gbxykgndn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.epnwcf.com/Article/details/gthgdzcdf.sHtML

[U62] PHP：日期对象
来源：http://www.share.tarul.cn/Article/details/gjkzfdayj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fktsv.cn/Article/details/gknbqldif.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.yfazqb.com/Article/details/gkiuxzrqj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.epnwcf.com/Article/details/gwyrrxjyu.sHtML

[U64] PHP：目录遍历
来源：http://3g.fktsv.cn/Article/details/goappozku.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fktsv.cn/Article/details/gqbhnynql.sHtML

[U65] PHP：会话
来源：http://blog.epnwcf.com/Article/details/gyvhzoqqa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gofaulkfb.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.vehdjk.com/Article/details/gciqkerxu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.tarul.cn/Article/details/gltvoijzg.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.bbcook.cn/Article/details/gcahqtvem.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.epnwcf.com/Article/details/gruuelunp.sHtML

[U68] PHP：PDO 连接
来源：http://3g.sjlbkw.cn/Article/details/gvopfzgvc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.yfazqb.com/Article/details/gduplniho.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.sjlbkw.cn/Article/details/gayyoseia.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.tarul.cn/Article/details/gobrwdala.sHtML

[U70] PHP：PDO 事务
来源：http://baike.vehdjk.com/Article/details/gqbonxqxl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fktsv.cn/Article/details/gkqtnfxpl.sHtML

[U71] PHP：抛出异常
来源：http://blog.fktsv.cn/Article/details/gqsunweym.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.yfazqb.com/Article/details/ggcaiiwtl.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.epnwcf.com/Article/details/gktjoxhmx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.bbcook.cn/Article/details/gmsruzwvg.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.tarul.cn/Article/details/gcwpndafn.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.epnwcf.com/Article/details/grlyrclxd.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gyufzbhxy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.sjlbkw.cn/Article/details/gwvinngmf.sHtML

[U75] PHP：依赖注入
来源：http://m.share.epnwcf.com/Article/details/gnzutjcqa.sHtML

composer require psr/container
来源：http://mobile.tarul.cn/Article/details/gsnjmdocl.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fktsv.cn/Article/details/grnxmfwxc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.vehdjk.com/Article/details/glslebery.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.yfazqb.com/Article/details/ggifmexnb.sHtML

composer require twig/twig
来源：http://baike.fktsv.cn/Article/details/gugahfqbf.sHtML

[U78] PHP：单元测试
来源：http://read.share.bbcook.cn/Article/details/gftyksgmd.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.bbcook.cn/Article/details/ggqeyyosc.sHtML

[U79] PHP：静态分析
来源：http://wap.vehdjk.com/Article/details/gzmjuluql.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.tarul.cn/Article/details/gmutbbweq.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.vehdjk.com/Article/details/gpjfhshxe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.sjlbkw.cn/Article/details/gvzbncdyr.sHtML

[U81] JS：初始化项目
来源：http://www.share.bbcook.cn/Article/details/gfcwkkuog.sHtML

npm init -y;  npm i express
来源：http://m.share.fktsv.cn/Article/details/gfkuzqlfc.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.yfazqb.com/Article/details/gjwhvwzbe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.vehdjk.com/Article/details/gnifgxfue.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.vehdjk.com/Article/details/gmjwvtzvk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.epnwcf.com/Article/details/gnjemjtuh.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.tarul.cn/Article/details/gnwgyblao.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.vehdjk.com/Article/details/ggowczvjq.sHtML

[U85] JS：可选链
来源：http://blog.vehdjk.com/Article/details/gnhdgfeag.sHtML

a?.b?.c
来源：http://m.share.yfazqb.com/Article/details/gbfsugkcu.sHtML

[U86] JS：空值合并
来源：http://www.m.share.vehdjk.com/Article/details/gckgdngqy.sHtML

a ?? b
来源：http://www.m.share.epnwcf.com/Article/details/grqxqgkte.sHtML

[U87] JS：解构默认值
来源：http://baike.bbcook.cn/Article/details/guyzoxser.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.bbcook.cn/Article/details/gdlpkagqn.sHtML

[U88] JS：对象展开合并
来源：http://wap.fktsv.cn/Article/details/gvnlyaeqm.sHtML

{ ...a, ...b }
来源：http://www.share.yfazqb.com/Article/details/gnqfutadi.sHtML

[U89] JS：数组去重
来源：http://www.blog.yfazqb.com/Article/details/gbovtoqel.sHtML

[...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gkjnsebuo.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.epnwcf.com/Article/details/gbsfupwew.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gvvanqhiv.sHtML

[U91] JS：对象键值遍历
来源：http://wap.vehdjk.com/Article/details/gsxkjlnyo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.bbcook.cn/Article/details/gbrarthbd.sHtML

[U92] JS：深拷贝
来源：http://www.share.tarul.cn/Article/details/gvtzsdycn.sHtML

structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gylgthxio.sHtML

[U93] JS：模板字符串
来源：http://3g.epnwcf.com/Article/details/gsmtubvdk.sHtML

`共 ${n} 条`
来源：http://baike.yfazqb.com/Article/details/ggeepcsrw.sHtML

[U94] JS：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gwivkhrwm.sHtML

const double = x => x * 2;
来源：http://wap.bbcook.cn/Article/details/gnyrczfmo.sHtML

[U95] JS：Promise 包装
来源：http://m.share.vehdjk.com/Article/details/gzrtptija.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fktsv.cn/Article/details/gmclmzlug.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.sjlbkw.cn/Article/details/gxryncrkt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gzyqlyzdp.sHtML

[U97] JS：并发请求
来源：http://www.blog.vehdjk.com/Article/details/gjqwdgoqj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gwfskzlyp.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.bbcook.cn/Article/details/gutcfahyr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.bbcook.cn/Article/details/gsfixgfhv.sHtML

[U99] JS：事件监听
来源：http://wap.sjlbkw.cn/Article/details/gtsgqcoir.sHtML

el.addEventListener("click", e => {})
来源：http://baike.sjlbkw.cn/Article/details/gcgqadpby.sHtML

[U100] JS：DOM 查询
来源：http://blog.vehdjk.com/Article/details/ghmgrrejh.sHtML

document.querySelector(".item")
来源：http://3g.vehdjk.com/Article/details/gdifyoied.sHtML

[U101] JS：classList 操作
来源：http://blog.vehdjk.com/Article/details/gfskqxesh.sHtML

el.classList.toggle("active")
来源：http://baike.sjlbkw.cn/Article/details/gdvrekjvg.sHtML

[U102] JS：本地存储
来源：http://blog.yfazqb.com/Article/details/gifmcsyju.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fktsv.cn/Article/details/gpzepzrhr.sHtML

[U103] JS：定时器
来源：http://3g.sjlbkw.cn/Article/details/gccqahfya.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.sjlbkw.cn/Article/details/ghjhpyrsw.sHtML

[U104] JS：防抖
来源：http://baike.sjlbkw.cn/Article/details/glmxzlyli.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gziafupqb.sHtML

[U105] JS：节流
来源：http://baike.fktsv.cn/Article/details/gkjxqmhwv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.epnwcf.com/Article/details/gsptxlbzk.sHtML

[U106] JS：日期格式化
来源：http://read.share.bbcook.cn/Article/details/gpxmjfdmk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.epnwcf.com/Article/details/gvjbpuhkx.sHtML

[U107] JS：数字千分位
来源：http://read.share.tarul.cn/Article/details/gjdfzlxbr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.tarul.cn/Article/details/gyrqtwvpb.sHtML

[U108] JS：随机整数
来源：http://3g.tarul.cn/Article/details/gjuiikqph.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.vehdjk.com/Article/details/gdyqrrijd.sHtML

[U109] JS：数组分组
来源：http://read.share.bbcook.cn/Article/details/gdwfbzgsv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gfckczgoo.sHtML

[U110] JS：数组分块
来源：http://www.blog.bbcook.cn/Article/details/ggqhyudag.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.bbcook.cn/Article/details/gnwqsokov.sHtML

[U111] JS：对象转 Map
来源：http://mobile.bbcook.cn/Article/details/guwjpdtvc.sHtML

new Map(Object.entries(obj))
来源：http://wap.yfazqb.com/Article/details/gajlnsrbp.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.tarul.cn/Article/details/gjrebimgm.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/grflczorx.sHtML

[U113] JS：正则替换全部
来源：http://3g.sjlbkw.cn/Article/details/gvkhnkawf.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gjsbfiota.sHtML

[U114] JS：JSON 深比较
来源：http://baike.yfazqb.com/Article/details/gfstwdioi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.bbcook.cn/Article/details/gkqaltnto.sHtML

[U115] JS：生成 UUID
来源：http://wap.epnwcf.com/Article/details/gzgjtcmda.sHtML

crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gqfxqxori.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.yfazqb.com/Article/details/gmyfinyml.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.vehdjk.com/Article/details/gnagylmzt.sHtML

[U117] JS：单元测试
来源：http://wap.epnwcf.com/Article/details/gwwvfkrsd.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.vehdjk.com/Article/details/gmfjwnoom.sHtML

[U118] JS：开发服务器
来源：http://mobile.vehdjk.com/Article/details/gxartcavb.sHtML

npm i -D vite;  npx vite
来源：http://blog.bbcook.cn/Article/details/gsnotloua.sHtML

[U119] JS：生产构建
来源：http://m.share.fktsv.cn/Article/details/gmbyavrxf.sHtML

npx vite build
来源：http://read.share.yfazqb.com/Article/details/grubtcutx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.sjlbkw.cn/Article/details/goxrzkxge.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fktsv.cn/Article/details/gryrfdqkf.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqdravzlr.sHtML

统计汇总
来源：http://www.m.share.fktsv.cn/Article/details/gxnufhzot.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvbptudhs.sHtML

按语言统计（条）：
来源：http://baike.vehdjk.com/Article/details/goutihaky.sHtML

Python ......... 252
来源：http://www.share.bbcook.cn/Article/details/guiscsgne.sHtML

PHP ............ 252
来源：http://www.share.vehdjk.com/Article/details/glzqnlghy.sHtML

JavaScript ..... 252
来源：http://3g.epnwcf.com/Article/details/ggxmznvwy.sHtML

TypeScript ..... 212
来源：http://www.share.tarul.cn/Article/details/gijizxlio.sHtML

Java ........... 212
来源：http://mobile.fktsv.cn/Article/details/guvgallco.sHtML

Go ............. 212
来源：http://www.share.vehdjk.com/Article/details/gcqndbriu.sHtML

Ruby ........... 212
来源：http://read.share.bbcook.cn/Article/details/ganpjdafr.sHtML

C# ............. 212
来源：http://3g.fktsv.cn/Article/details/gniaoyedm.sHtML

C .............. 30
来源：http://baike.bbcook.cn/Article/details/gqvzymmld.sHtML

C++ ............ 30
来源：http://mobile.vehdjk.com/Article/details/gnkwrpqwe.sHtML

SQL ............ 90
来源：http://www.blog.tarul.cn/Article/details/gomemgnar.sHtML

Bash ........... 80
来源：http://m.share.yfazqb.com/Article/details/gxmnoaaoz.sHtML

Kotlin ......... 15
来源：http://m.share.sjlbkw.cn/Article/details/gyjxtfbzd.sHtML

Swift .......... 15
来源：http://mobile.bbcook.cn/Article/details/gpbtdiact.sHtML

Lua ............ 10
来源：http://www.blog.vehdjk.com/Article/details/gslzyprfh.sHtML

Perl ........... 10
来源：http://blog.epnwcf.com/Article/details/gexhbhdzy.sHtML

Scala .......... 10
来源：http://mobile.yfazqb.com/Article/details/gfzvfzoqh.sHtML

------------------------------------
来源：http://www.share.tarul.cn/Article/details/gtykkawxe.sHtML

合计 ........... 2106 条
来源：http://read.share.epnwcf.com/Article/details/gmhfjvgjl.sHtML

按章节统计：
来源：http://3g.bbcook.cn/Article/details/genwndfks.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.bbcook.cn/Article/details/guldbulgu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/gtdwjhuju.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/gxevqhxma.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.vehdjk.com/Article/details/gkirilbit.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.yfazqb.com/Article/details/gterbkpcb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.yfazqb.com/Article/details/gdwcitfzo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/ggmehmopi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.bbcook.cn/Article/details/gskdeblez.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/garpeoptr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.bbcook.cn/Article/details/gnmivnuyd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/garoxriic.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/grhhkzbfa.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gqurawlik.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/gthrlknvt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.tarul.cn/Article/details/gkczxyyav.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gmvxvxvhf.sHtML

Q SQL 专题                              90
来源：http://www.blog.bbcook.cn/Article/details/gyiolphta.sHtML

R Bash 专题                             80
来源：http://3g.tarul.cn/Article/details/grxixprqy.sHtML

S C / C++ 专题                          60
来源：http://3g.fktsv.cn/Article/details/gylcdkqwo.sHtML

T 其他语言补充                          60
来源：http://blog.epnwcf.com/Article/details/gypmpflti.sHtML

U 高频实用片段                         120
来源：http://baike.sjlbkw.cn/Article/details/gezuhiiuq.sHtML

------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gkgvpjsam.sHtML

合计                                  2106 条
来源：http://wap.bbcook.cn/Article/details/geiekovrc.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gvzbqjhgr.sHtML

使用提醒
来源：http://3g.tarul.cn/Article/details/gtscwllfu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gzbezabqi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.tarul.cn/Article/details/gvkckxnse.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.tarul.cn/Article/details/gzzlpqbun.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.tarul.cn/Article/details/glkbpnzhj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fktsv.cn/Article/details/gdnjyspln.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.yfazqb.com/Article/details/gynbtdexz.sHtML

—— 文件结束 ——
来源：http://mobile.bbcook.cn/Article/details/guttbxlhi.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gazfvdcjl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.epnwcf.com/Article/details/gjckvezpa.sHtML

Common Programming Examples Cheat Book
来源：http://blog.sjlbkw.cn/Article/details/gwnzezosx.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gsxfiujir.sHtML

【收录内容】
来源：http://www.blog.bbcook.cn/Article/details/gcrbwcioj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.bbcook.cn/Article/details/gdijbxsnj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.sjlbkw.cn/Article/details/gxvpbgitl.sHtML

SQL · Bash · C · C++
来源：http://wap.bbcook.cn/Article/details/glqfhlrja.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.bbcook.cn/Article/details/gobxmeohk.sHtML

【使用说明】
来源：http://read.share.vehdjk.com/Article/details/glpvoofcr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.sjlbkw.cn/Article/details/gelmdrpbt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.sjlbkw.cn/Article/details/ghnveqkis.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.epnwcf.com/Article/details/gxxgnufyb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.yfazqb.com/Article/details/gmvoaxlsf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fktsv.cn/Article/details/gjjqyusli.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.sjlbkw.cn/Article/details/gtgvcxrtv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.fktsv.cn/Article/details/grtsnhify.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.sjlbkw.cn/Article/details/grhofkhyu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.yfazqb.com/Article/details/gcanjimya.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.sjlbkw.cn/Article/details/geakyyzyy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fktsv.cn/Article/details/gldwnlfcr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.bbcook.cn/Article/details/gnajwzvsh.sHtML

【文件统计】
来源：http://wap.fktsv.cn/Article/details/gzfncwznu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.vehdjk.com/Article/details/ggnexdwiw.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gxhmpsjcm.sHtML

目  录
来源：http://www.share.yfazqb.com/Article/details/gakswnscw.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gpciaqczu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.epnwcf.com/Article/details/gjmucvayr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gvoudappy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gphingfre.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fktsv.cn/Article/details/gtljezgpc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.yfazqb.com/Article/details/gyysepudg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.tarul.cn/Article/details/gwknyxkau.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/giktxgfwc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.sjlbkw.cn/Article/details/gtdwpyqvl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/gbkuogfqy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.bbcook.cn/Article/details/gawyqiyfk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gotyujkhg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.sjlbkw.cn/Article/details/guufctzni.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gngkfpvwh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.bbcook.cn/Article/details/gjrcvohcm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.sjlbkw.cn/Article/details/gqldfnsih.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gtrlbbcse.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.epnwcf.com/Article/details/gwhyjtvdg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.yfazqb.com/Article/details/ggzghxwza.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.vehdjk.com/Article/details/grkwsbgec.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fktsv.cn/Article/details/ganrmhgtt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.yfazqb.com/Article/details/gudhaiyxp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gaypbbptk.sHtML

A. 基础语法与类型
来源：http://3g.tarul.cn/Article/details/guennounb.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdidvyiyw.sHtML

[A01] Hello World
来源：http://www.share.vehdjk.com/Article/details/geghfdyyt.sHtML

Py:   print("Hello, World!")
来源：http://www.share.bbcook.cn/Article/details/gsauxehjl.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.sjlbkw.cn/Article/details/golhabrjd.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.epnwcf.com/Article/details/grmtacqmo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.bbcook.cn/Article/details/gpavxhwqr.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.epnwcf.com/Article/details/gjczwuiek.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fktsv.cn/Article/details/gknjnplag.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.epnwcf.com/Article/details/gaywajlin.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fktsv.cn/Article/details/gytohehml.sHtML

[A02] 变量声明与赋值
来源：http://m.share.vehdjk.com/Article/details/gubsrdxgj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.vehdjk.com/Article/details/gabnurodl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.epnwcf.com/Article/details/gvhugzqnz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.tarul.cn/Article/details/grxxbadbi.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.vehdjk.com/Article/details/geludmgyz.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.vehdjk.com/Article/details/guovdfosq.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.sjlbkw.cn/Article/details/grqrvcpaq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fktsv.cn/Article/details/gxtgnpanr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.tarul.cn/Article/details/ghagpvqmr.sHtML

[A03] 常量定义
来源：http://www.share.bbcook.cn/Article/details/gjzoaeohy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.sjlbkw.cn/Article/details/gnvzgioip.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gchlsvnhp.sHtML

JS:   const PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gpgrsuckp.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gslkbaejn.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gkfoepymg.sHtML

Go:   const PI = 3.14159
来源：http://blog.yfazqb.com/Article/details/gdaagngse.sHtML


<!-- 参考信息 -->