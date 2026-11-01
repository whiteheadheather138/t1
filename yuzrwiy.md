代发 wailian999

[U31] Py：单测
来源：http://read.share.fktsv.cn/Article/details/gpzolsxag.sHtML

python -m pytest -q
来源：http://mobile.fktsv.cn/Article/details/gykwnlkgr.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.tarul.cn/Article/details/ghvzjgcdf.sHtML

ruff format . && ruff check --fix .
来源：http://blog.bbcook.cn/Article/details/gcrwrdugw.sHtML

[U33] Py：打包发布
来源：http://mobile.epnwcf.com/Article/details/gkyuotjbt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.yfazqb.com/Article/details/gnwbxfoyy.sHtML

[U34] Py：判断编码
来源：http://mobile.bbcook.cn/Article/details/gpxonaimi.sHtML

chardet.detect(raw)
来源：http://baike.vehdjk.com/Article/details/gqnchjgue.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.tarul.cn/Article/details/glhzvsxmg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.vehdjk.com/Article/details/gwnknlrkn.sHtML

[U36] Py：定时任务
来源：http://blog.vehdjk.com/Article/details/goyruufgd.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.epnwcf.com/Article/details/gfiwywmmr.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.tarul.cn/Article/details/gymnwszgs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.yfazqb.com/Article/details/gtehrwdes.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fktsv.cn/Article/details/gwhjczgpg.sHtML

Path(__file__).resolve().parent
来源：http://baike.bbcook.cn/Article/details/giqwsxvdc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.yfazqb.com/Article/details/gqsvgrndd.sHtML

sys.stdout.isatty()
来源：http://m.share.sjlbkw.cn/Article/details/guexedjrw.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.bbcook.cn/Article/details/gngtuhqpl.sHtML

print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/gllvduvfc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.vehdjk.com/Article/details/gbrwthpwg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.tarul.cn/Article/details/gzitchegm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.tarul.cn/Article/details/grbxrrbng.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.epnwcf.com/Article/details/gupankkht.sHtML

[U43] PHP：声明命名空间
来源：http://baike.vehdjk.com/Article/details/gjgxmuofj.sHtML

namespace App\Http;
来源：http://wap.fktsv.cn/Article/details/gsknmemcn.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.yfazqb.com/Article/details/gvnpboxnt.sHtML

declare(strict_types=1);
来源：http://www.share.sjlbkw.cn/Article/details/gqgvqmmtr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.tarul.cn/Article/details/gzdjdjkxg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gpovlpjqr.sHtML

[U46] PHP：可空类型
来源：http://baike.epnwcf.com/Article/details/gntnaidsh.sHtML

?string $name = null
来源：http://www.blog.tarul.cn/Article/details/gpysepzrp.sHtML

[U47] PHP：联合类型
来源：http://blog.epnwcf.com/Article/details/gxplmhqxk.sHtML

int|string $id
来源：http://read.share.vehdjk.com/Article/details/gvfnmhjnc.sHtML

[U48] PHP：纯枚举
来源：http://wap.epnwcf.com/Article/details/gbhzpxdip.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.tarul.cn/Article/details/grdzdgrfw.sHtML

[U49] PHP：只读属性
来源：http://3g.sjlbkw.cn/Article/details/gmheqwdkr.sHtML

public readonly string $name
来源：http://m.share.vehdjk.com/Article/details/gjxkgrdtv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.vehdjk.com/Article/details/grngzkryj.sHtML

public function __construct(private int $id) {}
来源：http://www.share.yfazqb.com/Article/details/gemarziqf.sHtML

[U51] PHP：数组解构
来源：http://baike.bbcook.cn/Article/details/grhdllubq.sHtML

[$a, $b] = $arr;
来源：http://3g.vehdjk.com/Article/details/gsiytevhm.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fktsv.cn/Article/details/gjynqckdx.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.yfazqb.com/Article/details/gihuubftz.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.vehdjk.com/Article/details/gxvpsoxnt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.epnwcf.com/Article/details/gjupdgcag.sHtML

[U54] PHP：空安全调用
来源：http://www.share.tarul.cn/Article/details/gravgbkeb.sHtML

$obj?->method()
来源：http://3g.bbcook.cn/Article/details/ggevowcfm.sHtML

[U55] PHP：match 表达式
来源：http://www.share.epnwcf.com/Article/details/gymsjcvlc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.epnwcf.com/Article/details/gsvbblwew.sHtML

[U56] PHP：命名参数
来源：http://3g.vehdjk.com/Article/details/gotclxono.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gucygsapl.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/glrcrfcgg.sHtML

"值: {$a}"
来源：http://www.share.epnwcf.com/Article/details/gacpcbxqd.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.epnwcf.com/Article/details/ggslthjzk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.yfazqb.com/Article/details/gxbuetjdf.sHtML

[U59] PHP：自定义排序
来源：http://wap.fktsv.cn/Article/details/giindcqnl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gcthrzugc.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/gruucdwlh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.sjlbkw.cn/Article/details/grefsknlz.sHtML

[U61] PHP：正则
来源：http://www.blog.bbcook.cn/Article/details/gojiilzdi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/grjgvmequ.sHtML

[U62] PHP：日期对象
来源：http://blog.sjlbkw.cn/Article/details/gyltfarmc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.yfazqb.com/Article/details/gjejdxrpc.sHtML

[U63] PHP：文件读写
来源：http://3g.fktsv.cn/Article/details/gtyxkknnx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fktsv.cn/Article/details/gfitrqnft.sHtML

[U64] PHP：目录遍历
来源：http://baike.sjlbkw.cn/Article/details/gouelzcwq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.vehdjk.com/Article/details/gqffhdggw.sHtML

[U65] PHP：会话
来源：http://mobile.bbcook.cn/Article/details/gkexsgksk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.vehdjk.com/Article/details/gypkfdsji.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.yfazqb.com/Article/details/gwrhdmirw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.sjlbkw.cn/Article/details/gacqffocx.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.sjlbkw.cn/Article/details/gqnzjiumf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.tarul.cn/Article/details/gmtggayhq.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fktsv.cn/Article/details/gykebltpl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fktsv.cn/Article/details/ghkwxwnil.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.sjlbkw.cn/Article/details/gscwrerbl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.vehdjk.com/Article/details/gbjrqbfjs.sHtML

[U70] PHP：PDO 事务
来源：http://baike.tarul.cn/Article/details/gktehftis.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.epnwcf.com/Article/details/gpeoxscdl.sHtML

[U71] PHP：抛出异常
来源：http://blog.bbcook.cn/Article/details/gvoswljpg.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.sjlbkw.cn/Article/details/gbxftyubf.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.tarul.cn/Article/details/gimpobycy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.epnwcf.com/Article/details/gmtvvhoce.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.epnwcf.com/Article/details/gllphyopc.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.tarul.cn/Article/details/gxpydkwsq.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/giogphhyz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.vehdjk.com/Article/details/gsadlrrbk.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.epnwcf.com/Article/details/gfngcwegx.sHtML

composer require psr/container
来源：http://www.share.bbcook.cn/Article/details/gtlkqvtnp.sHtML

[U76] PHP：简单路由
来源：http://www.blog.sjlbkw.cn/Article/details/gsvtkultx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fktsv.cn/Article/details/gghzimgsx.sHtML

[U77] PHP：模板渲染
来源：http://www.share.tarul.cn/Article/details/gqxyatqme.sHtML

composer require twig/twig
来源：http://mobile.vehdjk.com/Article/details/gnzijwtxn.sHtML

[U78] PHP：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gsroyuuik.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.sjlbkw.cn/Article/details/gglsovqui.sHtML

[U79] PHP：静态分析
来源：http://www.blog.epnwcf.com/Article/details/gskekllmc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.sjlbkw.cn/Article/details/gimsvptuc.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.vehdjk.com/Article/details/gndukrkvo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.bbcook.cn/Article/details/gvavmazgk.sHtML

[U81] JS：初始化项目
来源：http://read.share.fktsv.cn/Article/details/gczrfpifm.sHtML

npm init -y;  npm i express
来源：http://wap.vehdjk.com/Article/details/gpccpbaer.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.yfazqb.com/Article/details/ggjnokoyx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.sjlbkw.cn/Article/details/gtutgofnd.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.sjlbkw.cn/Article/details/gdlnegooo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyefsesz.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.epnwcf.com/Article/details/glwookhos.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.epnwcf.com/Article/details/ggmhpglyj.sHtML

[U85] JS：可选链
来源：http://3g.fktsv.cn/Article/details/gqhejwavm.sHtML

a?.b?.c
来源：http://wap.yfazqb.com/Article/details/gotvxnapp.sHtML

[U86] JS：空值合并
来源：http://baike.vehdjk.com/Article/details/ghdcdibrg.sHtML

a ?? b
来源：http://www.m.share.fktsv.cn/Article/details/geljkjwnk.sHtML

[U87] JS：解构默认值
来源：http://wap.sjlbkw.cn/Article/details/gdbaqfvrz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fktsv.cn/Article/details/gfgnwykvv.sHtML

[U88] JS：对象展开合并
来源：http://3g.sjlbkw.cn/Article/details/gywqodycd.sHtML

{ ...a, ...b }
来源：http://blog.sjlbkw.cn/Article/details/ghfzyofiw.sHtML

[U89] JS：数组去重
来源：http://m.share.epnwcf.com/Article/details/grxnbyuad.sHtML

[...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/gpvuhdods.sHtML

[U90] JS：数字数组排序
来源：http://3g.sjlbkw.cn/Article/details/gwpdurjeh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/ggpycymmq.sHtML

[U91] JS：对象键值遍历
来源：http://blog.epnwcf.com/Article/details/ghbsacuuh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.vehdjk.com/Article/details/gipsjxlbz.sHtML

[U92] JS：深拷贝
来源：http://baike.bbcook.cn/Article/details/gvleceexm.sHtML

structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gcfafjflz.sHtML

[U93] JS：模板字符串
来源：http://3g.sjlbkw.cn/Article/details/glgimeiht.sHtML

`共 ${n} 条`
来源：http://3g.sjlbkw.cn/Article/details/gbfkzxscd.sHtML

[U94] JS：箭头函数
来源：http://mobile.fktsv.cn/Article/details/gjfoecqnt.sHtML

const double = x => x * 2;
来源：http://www.blog.fktsv.cn/Article/details/gvfbnwfgi.sHtML

[U95] JS：Promise 包装
来源：http://www.share.yfazqb.com/Article/details/gdggvyvyg.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fktsv.cn/Article/details/gxiwylsof.sHtML

[U96] JS：async/await 与异常
来源：http://blog.sjlbkw.cn/Article/details/gaqxixgda.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gqynbftsx.sHtML

[U97] JS：并发请求
来源：http://www.share.sjlbkw.cn/Article/details/gsswjevfc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/ghkgrorbd.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.yfazqb.com/Article/details/gvgzqsujp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.epnwcf.com/Article/details/gnipomfrq.sHtML

[U99] JS：事件监听
来源：http://m.share.yfazqb.com/Article/details/gtayaehkz.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.bbcook.cn/Article/details/gtwjcqifz.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.tarul.cn/Article/details/gfniubfut.sHtML

document.querySelector(".item")
来源：http://www.blog.tarul.cn/Article/details/guuxrkxdm.sHtML

[U101] JS：classList 操作
来源：http://wap.epnwcf.com/Article/details/ghfewsrwi.sHtML

el.classList.toggle("active")
来源：http://baike.fktsv.cn/Article/details/gerxgbhfl.sHtML

[U102] JS：本地存储
来源：http://www.share.epnwcf.com/Article/details/gymzmfpbi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.vehdjk.com/Article/details/gkerfukkw.sHtML

[U103] JS：定时器
来源：http://m.share.fktsv.cn/Article/details/giiwlbpag.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.tarul.cn/Article/details/gvxoekzsk.sHtML

[U104] JS：防抖
来源：http://blog.tarul.cn/Article/details/gqwrrdpqn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gvdnhwana.sHtML

[U105] JS：节流
来源：http://www.share.yfazqb.com/Article/details/glkdqbidl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.sjlbkw.cn/Article/details/gpzvwmzuu.sHtML

[U106] JS：日期格式化
来源：http://3g.yfazqb.com/Article/details/gkuukblpk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.sjlbkw.cn/Article/details/gfajxsxlr.sHtML

[U107] JS：数字千分位
来源：http://mobile.fktsv.cn/Article/details/gycrkpwhj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.sjlbkw.cn/Article/details/guvjsrxzp.sHtML

[U108] JS：随机整数
来源：http://wap.epnwcf.com/Article/details/gaebzvaho.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.yfazqb.com/Article/details/gtkkzeqku.sHtML

[U109] JS：数组分组
来源：http://www.share.tarul.cn/Article/details/ggsdlhtyi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gglbfujhk.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fktsv.cn/Article/details/gdlxnebup.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.epnwcf.com/Article/details/gvdlmobcb.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.vehdjk.com/Article/details/giwokvdow.sHtML

new Map(Object.entries(obj))
来源：http://mobile.bbcook.cn/Article/details/gprcuyorl.sHtML

[U112] JS：字符串补位
来源：http://read.share.sjlbkw.cn/Article/details/gibolphws.sHtML

"7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gkpxvbgrm.sHtML

[U113] JS：正则替换全部
来源：http://read.share.epnwcf.com/Article/details/gkdxxbmxy.sHtML

s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gyimmbwut.sHtML

[U114] JS：JSON 深比较
来源：http://blog.yfazqb.com/Article/details/gtbgrxpyw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fktsv.cn/Article/details/gbqwzfktj.sHtML

[U115] JS：生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gxnbphgtw.sHtML

crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gefiheikp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.yfazqb.com/Article/details/gxxbkjemu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.tarul.cn/Article/details/gxaylndoy.sHtML

[U117] JS：单元测试
来源：http://baike.fktsv.cn/Article/details/ghamjgijy.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.vehdjk.com/Article/details/gubnhqpxw.sHtML

[U118] JS：开发服务器
来源：http://wap.bbcook.cn/Article/details/gemfwyjts.sHtML

npm i -D vite;  npx vite
来源：http://mobile.yfazqb.com/Article/details/gcmxdgxkf.sHtML

[U119] JS：生产构建
来源：http://www.share.bbcook.cn/Article/details/gseokhvro.sHtML

npx vite build
来源：http://3g.sjlbkw.cn/Article/details/gedsxrhlc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.tarul.cn/Article/details/gewcmfabw.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.vehdjk.com/Article/details/gixblhqac.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ggclczrxz.sHtML

统计汇总
来源：http://blog.sjlbkw.cn/Article/details/gdffnigar.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkepeespr.sHtML

按语言统计（条）：
来源：http://www.share.bbcook.cn/Article/details/gmvbxzfcf.sHtML

Python ......... 252
来源：http://www.m.share.epnwcf.com/Article/details/gcrxczkqn.sHtML

PHP ............ 252
来源：http://www.m.share.vehdjk.com/Article/details/gvwkvteqp.sHtML

JavaScript ..... 252
来源：http://m.share.yfazqb.com/Article/details/gxdpsoqsu.sHtML

TypeScript ..... 212
来源：http://www.m.share.vehdjk.com/Article/details/gjxzfvslk.sHtML

Java ........... 212
来源：http://www.share.epnwcf.com/Article/details/ggdggqvlo.sHtML

Go ............. 212
来源：http://www.m.share.epnwcf.com/Article/details/gksargqbo.sHtML

Ruby ........... 212
来源：http://www.blog.tarul.cn/Article/details/gyfevzwnk.sHtML

C# ............. 212
来源：http://read.share.sjlbkw.cn/Article/details/gjsagpplh.sHtML

C .............. 30
来源：http://mobile.epnwcf.com/Article/details/guqbnikxx.sHtML

C++ ............ 30
来源：http://3g.bbcook.cn/Article/details/gpcvqtbbg.sHtML

SQL ............ 90
来源：http://baike.bbcook.cn/Article/details/gcrkyymqh.sHtML

Bash ........... 80
来源：http://m.share.sjlbkw.cn/Article/details/gdgkbpofb.sHtML

Kotlin ......... 15
来源：http://www.blog.fktsv.cn/Article/details/gdnscmsok.sHtML

Swift .......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/gdxnqqtpd.sHtML

Lua ............ 10
来源：http://3g.tarul.cn/Article/details/gvnqeqrmy.sHtML

Perl ........... 10
来源：http://read.share.fktsv.cn/Article/details/gnkecbitl.sHtML

Scala .......... 10
来源：http://3g.epnwcf.com/Article/details/gfusotpbk.sHtML

------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gxufvvssa.sHtML

合计 ........... 2106 条
来源：http://www.blog.epnwcf.com/Article/details/grobqztwd.sHtML

按章节统计：
来源：http://m.share.fktsv.cn/Article/details/gamnwkipd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.vehdjk.com/Article/details/ghmlryhmc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.sjlbkw.cn/Article/details/gvzhhyxgj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.vehdjk.com/Article/details/gurwxgzyt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fktsv.cn/Article/details/gwxdeixck.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.bbcook.cn/Article/details/gudmyiuzz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gzyslgwvc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/gobhfjddh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.epnwcf.com/Article/details/gbasulabw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gkepekrcg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.yfazqb.com/Article/details/gytdkqfzo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gxrgzaitw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/glifrjydv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gwemgelmd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.bbcook.cn/Article/details/gfkpwsker.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fktsv.cn/Article/details/gjibhkxbv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gxqepgwwz.sHtML

Q SQL 专题                              90
来源：http://3g.yfazqb.com/Article/details/gcjkuesuq.sHtML

R Bash 专题                             80
来源：http://wap.vehdjk.com/Article/details/guojoezgi.sHtML

S C / C++ 专题                          60
来源：http://read.share.tarul.cn/Article/details/gallwmqst.sHtML

T 其他语言补充                          60
来源：http://www.share.fktsv.cn/Article/details/gghgunofi.sHtML

U 高频实用片段                         120
来源：http://mobile.fktsv.cn/Article/details/gugscgdns.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gojfomucw.sHtML

合计                                  2106 条
来源：http://wap.tarul.cn/Article/details/gdzeopfzv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gguqddlho.sHtML

使用提醒
来源：http://m.share.yfazqb.com/Article/details/goxcynwew.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/goxhbvqrf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.bbcook.cn/Article/details/gbtzhnotj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.tarul.cn/Article/details/gkjyfsscy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fktsv.cn/Article/details/gcqpscsov.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.yfazqb.com/Article/details/gifyuyisi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.epnwcf.com/Article/details/govpuqlvi.sHtML

—— 文件结束 ——
来源：http://read.share.epnwcf.com/Article/details/gfwepojyg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnhrbmbhb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.vehdjk.com/Article/details/gdvpdwoiz.sHtML

Common Programming Examples Cheat Book
来源：http://blog.bbcook.cn/Article/details/gpmixpfqc.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ghpchmozx.sHtML

【收录内容】
来源：http://wap.sjlbkw.cn/Article/details/gdjdqhits.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.epnwcf.com/Article/details/gpxzpkfcf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fktsv.cn/Article/details/gpfhstuml.sHtML

SQL · Bash · C · C++
来源：http://blog.sjlbkw.cn/Article/details/gksltzjft.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.bbcook.cn/Article/details/gjrfivxyx.sHtML

【使用说明】
来源：http://www.m.share.epnwcf.com/Article/details/gqtioawzc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.tarul.cn/Article/details/gducbqhrx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.yfazqb.com/Article/details/gzrtmybvb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.bbcook.cn/Article/details/guglgtcuu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.tarul.cn/Article/details/ganrlalex.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.bbcook.cn/Article/details/gcbuobcoz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdywcrgc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.sjlbkw.cn/Article/details/gokytjkfa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.bbcook.cn/Article/details/gayxweydx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.sjlbkw.cn/Article/details/goplevltk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.sjlbkw.cn/Article/details/gkskeunbd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.vehdjk.com/Article/details/geuayhdff.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.tarul.cn/Article/details/gbqwhvcmt.sHtML

【文件统计】
来源：http://www.share.yfazqb.com/Article/details/ghapyijsy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.yfazqb.com/Article/details/gyhumnjyz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gjterfiqo.sHtML

目  录
来源：http://3g.sjlbkw.cn/Article/details/gneqjhdfo.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gpzqcdasm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.epnwcf.com/Article/details/ghoxinwpu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.tarul.cn/Article/details/gbczcrhwk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrbkqhfg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.yfazqb.com/Article/details/gtxvbiczz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.epnwcf.com/Article/details/gixzlxyrs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.sjlbkw.cn/Article/details/ggnphsolb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.sjlbkw.cn/Article/details/gluxpdcfp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.yfazqb.com/Article/details/gxmadiwrd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gqmcwilzu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fktsv.cn/Article/details/grluausob.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gnhxcfwsb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gwgmksyqb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/grfegdecu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.epnwcf.com/Article/details/gphipkhpe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.tarul.cn/Article/details/gxlznaofy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fktsv.cn/Article/details/gurkewcvc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.bbcook.cn/Article/details/gdavaimqd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.vehdjk.com/Article/details/gewqqodox.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gnqiaupef.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.vehdjk.com/Article/details/goperkfik.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fktsv.cn/Article/details/gljgpankh.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gnowmktof.sHtML

A. 基础语法与类型
来源：http://baike.vehdjk.com/Article/details/gbmthetov.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gppnoppom.sHtML

[A01] Hello World
来源：http://read.share.epnwcf.com/Article/details/gaimxetay.sHtML

Py:   print("Hello, World!")
来源：http://wap.epnwcf.com/Article/details/gqokpibsa.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fktsv.cn/Article/details/gggulzelr.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fktsv.cn/Article/details/gdjlgnvtl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.tarul.cn/Article/details/gtwljcnho.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.vehdjk.com/Article/details/gjtbfhofa.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.tarul.cn/Article/details/guhuyhdhl.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.tarul.cn/Article/details/geuosorsh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.bbcook.cn/Article/details/gbdvcitlw.sHtML

[A02] 变量声明与赋值
来源：http://wap.sjlbkw.cn/Article/details/gjcndjnta.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.vehdjk.com/Article/details/gtqywikns.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.vehdjk.com/Article/details/ggofxdypj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.vehdjk.com/Article/details/gquvzmzve.sHtML


<!-- 参考信息 -->