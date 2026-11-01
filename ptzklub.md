代发 wailian999

[U31] Py：单测
来源：http://www.share.epnwcf.com/Article/details/gozxfuyhi.sHtML

python -m pytest -q
来源：http://www.share.tarul.cn/Article/details/grqwqkseq.sHtML

[U32] Py：代码格式化
来源：http://m.share.epnwcf.com/Article/details/gldxtejzw.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.bbcook.cn/Article/details/gcdylzhwk.sHtML

[U33] Py：打包发布
来源：http://blog.bbcook.cn/Article/details/gikgshegu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.tarul.cn/Article/details/gsxklpyiz.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fktsv.cn/Article/details/grhbcpyen.sHtML

chardet.detect(raw)
来源：http://3g.vehdjk.com/Article/details/gpjlfmnpm.sHtML

[U35] Py：发送邮件
来源：http://read.share.bbcook.cn/Article/details/gduexdzyb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.bbcook.cn/Article/details/gsubizlsc.sHtML

[U36] Py：定时任务
来源：http://read.share.vehdjk.com/Article/details/gtymorbkd.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.tarul.cn/Article/details/gfyxmagpl.sHtML

[U37] Py：读写 Excel
来源：http://baike.sjlbkw.cn/Article/details/gpjjaokvs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.tarul.cn/Article/details/gfhohldvu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.yfazqb.com/Article/details/gnspekoht.sHtML

Path(__file__).resolve().parent
来源：http://blog.bbcook.cn/Article/details/gexuywtsk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fktsv.cn/Article/details/guvtraylr.sHtML

sys.stdout.isatty()
来源：http://3g.bbcook.cn/Article/details/gyviujjee.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fktsv.cn/Article/details/gugqifodb.sHtML

print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/gzkwbbxtq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.epnwcf.com/Article/details/ggwtobfcj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.tarul.cn/Article/details/gdaupfxbr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fktsv.cn/Article/details/gwbzwnfoj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.bbcook.cn/Article/details/gfklseknp.sHtML

[U43] PHP：声明命名空间
来源：http://baike.vehdjk.com/Article/details/gfryckobg.sHtML

namespace App\Http;
来源：http://blog.vehdjk.com/Article/details/gtiznjspm.sHtML

[U44] PHP：开启严格类型
来源：http://3g.sjlbkw.cn/Article/details/guxmwncfc.sHtML

declare(strict_types=1);
来源：http://www.blog.tarul.cn/Article/details/gwkdaxgxz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fktsv.cn/Article/details/gvpfybsxm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gasghgkfo.sHtML

[U46] PHP：可空类型
来源：http://baike.bbcook.cn/Article/details/gjomztsde.sHtML

?string $name = null
来源：http://www.share.epnwcf.com/Article/details/gmymbvhiq.sHtML

[U47] PHP：联合类型
来源：http://mobile.yfazqb.com/Article/details/gmtvnnsht.sHtML

int|string $id
来源：http://baike.yfazqb.com/Article/details/gbzhqfuxu.sHtML

[U48] PHP：纯枚举
来源：http://wap.sjlbkw.cn/Article/details/gprbajulo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.tarul.cn/Article/details/gmzmhshhi.sHtML

[U49] PHP：只读属性
来源：http://read.share.fktsv.cn/Article/details/gwqlelemq.sHtML

public readonly string $name
来源：http://m.share.vehdjk.com/Article/details/guweetlms.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.sjlbkw.cn/Article/details/gociyjslp.sHtML

public function __construct(private int $id) {}
来源：http://m.share.tarul.cn/Article/details/gxyfjnfwe.sHtML

[U51] PHP：数组解构
来源：http://m.share.sjlbkw.cn/Article/details/gktugreef.sHtML

[$a, $b] = $arr;
来源：http://www.share.yfazqb.com/Article/details/gikogrfzx.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fktsv.cn/Article/details/glavlduwe.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.tarul.cn/Article/details/glxhptbep.sHtML

[U53] PHP：空合并运算符
来源：http://blog.yfazqb.com/Article/details/gxjrpqoal.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.yfazqb.com/Article/details/gesuxisrw.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fktsv.cn/Article/details/gdxrazxtr.sHtML

$obj?->method()
来源：http://baike.epnwcf.com/Article/details/ghfeshbfk.sHtML

[U55] PHP：match 表达式
来源：http://blog.yfazqb.com/Article/details/gewhrwwws.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.epnwcf.com/Article/details/ghcmogqqe.sHtML

[U56] PHP：命名参数
来源：http://mobile.vehdjk.com/Article/details/gnotmwnor.sHtML

f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gjjvixzil.sHtML

[U57] PHP：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gublxdnmj.sHtML

"值: {$a}"
来源：http://m.share.sjlbkw.cn/Article/details/gptuxtwbm.sHtML

[U58] PHP：数组三件套
来源：http://read.share.vehdjk.com/Article/details/gvnahprol.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.vehdjk.com/Article/details/gobwgfxie.sHtML

[U59] PHP：自定义排序
来源：http://baike.vehdjk.com/Article/details/gnimpqsjy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.vehdjk.com/Article/details/giminutey.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.bbcook.cn/Article/details/gcviolkuv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fktsv.cn/Article/details/gehcbhkmy.sHtML

[U61] PHP：正则
来源：http://www.m.share.bbcook.cn/Article/details/ghbavygct.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/gwynctkhw.sHtML

[U62] PHP：日期对象
来源：http://read.share.tarul.cn/Article/details/gxeheosfu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.bbcook.cn/Article/details/gwxinguhh.sHtML

[U63] PHP：文件读写
来源：http://read.share.yfazqb.com/Article/details/gfgnarwme.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.tarul.cn/Article/details/gepqclquf.sHtML

[U64] PHP：目录遍历
来源：http://3g.vehdjk.com/Article/details/gnusqlpcv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.epnwcf.com/Article/details/gumvudwdh.sHtML

[U65] PHP：会话
来源：http://wap.sjlbkw.cn/Article/details/glkbagrbd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.bbcook.cn/Article/details/grizzeieo.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.yfazqb.com/Article/details/gdouksimn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fktsv.cn/Article/details/gxaskjtgv.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.bbcook.cn/Article/details/glbqaywyi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fktsv.cn/Article/details/gtfhxwrzf.sHtML

[U68] PHP：PDO 连接
来源：http://baike.sjlbkw.cn/Article/details/gpislcxmz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.yfazqb.com/Article/details/goystpvhe.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fktsv.cn/Article/details/gngathcom.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.yfazqb.com/Article/details/gxdpgcysa.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.epnwcf.com/Article/details/gwyndlkqk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.yfazqb.com/Article/details/gvbdlwrbb.sHtML

[U71] PHP：抛出异常
来源：http://baike.vehdjk.com/Article/details/gdqkixdhm.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.vehdjk.com/Article/details/gssvdpcgh.sHtML

[U72] PHP：写错误日志
来源：http://mobile.tarul.cn/Article/details/gfxtfbzsj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fktsv.cn/Article/details/gvybjlovl.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.vehdjk.com/Article/details/ggdgbplyr.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.bbcook.cn/Article/details/ghfuyldmy.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.bbcook.cn/Article/details/goejrukhq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.bbcook.cn/Article/details/gbxcyjuhg.sHtML

[U75] PHP：依赖注入
来源：http://3g.sjlbkw.cn/Article/details/gvqqfhegl.sHtML

composer require psr/container
来源：http://blog.yfazqb.com/Article/details/gbygygzzh.sHtML

[U76] PHP：简单路由
来源：http://mobile.tarul.cn/Article/details/gwnajjvpf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.tarul.cn/Article/details/godbuniog.sHtML

[U77] PHP：模板渲染
来源：http://m.share.yfazqb.com/Article/details/gonyabpiw.sHtML

composer require twig/twig
来源：http://www.share.bbcook.cn/Article/details/gajncjcfb.sHtML

[U78] PHP：单元测试
来源：http://read.share.fktsv.cn/Article/details/ghcrppghr.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.epnwcf.com/Article/details/glxuvkoum.sHtML

[U79] PHP：静态分析
来源：http://m.share.sjlbkw.cn/Article/details/gmyiwinis.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.sjlbkw.cn/Article/details/gxbxxywqr.sHtML

[U80] PHP：代码规范修复
来源：http://wap.vehdjk.com/Article/details/gxjshvnvi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.yfazqb.com/Article/details/gkmvwvwgr.sHtML

[U81] JS：初始化项目
来源：http://wap.bbcook.cn/Article/details/gqyxygnds.sHtML

npm init -y;  npm i express
来源：http://wap.vehdjk.com/Article/details/ghhmaenmf.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.sjlbkw.cn/Article/details/gofnkehfg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.sjlbkw.cn/Article/details/gxuwzozwb.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.sjlbkw.cn/Article/details/gzhtonjvf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.vehdjk.com/Article/details/gqooeollg.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.vehdjk.com/Article/details/gswckusmj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.epnwcf.com/Article/details/ggwdapjht.sHtML

[U85] JS：可选链
来源：http://3g.fktsv.cn/Article/details/gozmehqvi.sHtML

a?.b?.c
来源：http://baike.epnwcf.com/Article/details/gffdacqvc.sHtML

[U86] JS：空值合并
来源：http://m.share.fktsv.cn/Article/details/gdaqkarpu.sHtML

a ?? b
来源：http://3g.sjlbkw.cn/Article/details/gjyrnotoj.sHtML

[U87] JS：解构默认值
来源：http://blog.bbcook.cn/Article/details/gfxclwatb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.vehdjk.com/Article/details/gvaylabkv.sHtML

[U88] JS：对象展开合并
来源：http://wap.fktsv.cn/Article/details/gljpjrrjk.sHtML

{ ...a, ...b }
来源：http://blog.yfazqb.com/Article/details/gitquqhai.sHtML

[U89] JS：数组去重
来源：http://3g.epnwcf.com/Article/details/gzmncqquv.sHtML

[...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gjgsxctmo.sHtML

[U90] JS：数字数组排序
来源：http://3g.vehdjk.com/Article/details/guetyzupk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gydqlflnx.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fktsv.cn/Article/details/gpubumbyk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.epnwcf.com/Article/details/gvfdwifbw.sHtML

[U92] JS：深拷贝
来源：http://blog.tarul.cn/Article/details/gkcykegvv.sHtML

structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gpoqndjrc.sHtML

[U93] JS：模板字符串
来源：http://baike.epnwcf.com/Article/details/glecncqvu.sHtML

`共 ${n} 条`
来源：http://m.share.yfazqb.com/Article/details/grwnkssxj.sHtML

[U94] JS：箭头函数
来源：http://wap.epnwcf.com/Article/details/gfafvhrjr.sHtML

const double = x => x * 2;
来源：http://www.share.vehdjk.com/Article/details/gkouplnup.sHtML

[U95] JS：Promise 包装
来源：http://baike.yfazqb.com/Article/details/gofmltemq.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fktsv.cn/Article/details/gqkzgnmzt.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.tarul.cn/Article/details/gnkybuwoa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gjjynmbwb.sHtML

[U97] JS：并发请求
来源：http://www.m.share.epnwcf.com/Article/details/gqirysrtg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gvpopfwuo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.vehdjk.com/Article/details/guphsyqtw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.vehdjk.com/Article/details/gqwadlarh.sHtML

[U99] JS：事件监听
来源：http://read.share.fktsv.cn/Article/details/gdumqonei.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fktsv.cn/Article/details/gerodphai.sHtML

[U100] JS：DOM 查询
来源：http://m.share.yfazqb.com/Article/details/glfvtlkpb.sHtML

document.querySelector(".item")
来源：http://3g.sjlbkw.cn/Article/details/gxwczzora.sHtML

[U101] JS：classList 操作
来源：http://wap.sjlbkw.cn/Article/details/gymoqqtiq.sHtML

el.classList.toggle("active")
来源：http://blog.vehdjk.com/Article/details/gpecslpqy.sHtML

[U102] JS：本地存储
来源：http://www.m.share.bbcook.cn/Article/details/geqbnrwwy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.vehdjk.com/Article/details/gyjlbuayn.sHtML

[U103] JS：定时器
来源：http://m.share.sjlbkw.cn/Article/details/gmlpmbjpb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.yfazqb.com/Article/details/guqjricgv.sHtML

[U104] JS：防抖
来源：http://www.share.sjlbkw.cn/Article/details/gjqzvjyrl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gtknnsmfr.sHtML

[U105] JS：节流
来源：http://baike.yfazqb.com/Article/details/geozjhviv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.bbcook.cn/Article/details/gydrhqlqe.sHtML

[U106] JS：日期格式化
来源：http://m.share.tarul.cn/Article/details/gisajaiqq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.bbcook.cn/Article/details/gmruziiul.sHtML

[U107] JS：数字千分位
来源：http://www.blog.sjlbkw.cn/Article/details/gbgvxxkgz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gkoglpdlw.sHtML

[U108] JS：随机整数
来源：http://blog.sjlbkw.cn/Article/details/goyicjycx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.vehdjk.com/Article/details/gqhvkzdaz.sHtML

[U109] JS：数组分组
来源：http://mobile.bbcook.cn/Article/details/ggyvvjsia.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gcvxdmkxp.sHtML

[U110] JS：数组分块
来源：http://www.blog.sjlbkw.cn/Article/details/gmtsfddze.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fktsv.cn/Article/details/gevklftzl.sHtML

[U111] JS：对象转 Map
来源：http://mobile.sjlbkw.cn/Article/details/gdbhswpsk.sHtML

new Map(Object.entries(obj))
来源：http://read.share.vehdjk.com/Article/details/gvptozlzt.sHtML

[U112] JS：字符串补位
来源：http://read.share.vehdjk.com/Article/details/gabmzkamf.sHtML

"7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gbkshyvwk.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fktsv.cn/Article/details/gjescsscl.sHtML

s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gdzabtjqz.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.tarul.cn/Article/details/gziyaddrn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/gklgjhgyd.sHtML

[U115] JS：生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gexqvjzyv.sHtML

crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gbsfdtxfl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fktsv.cn/Article/details/ggfpbgifj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.yfazqb.com/Article/details/guyyvvomc.sHtML

[U117] JS：单元测试
来源：http://blog.bbcook.cn/Article/details/gwcqquwlt.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.bbcook.cn/Article/details/gfaxknzrd.sHtML

[U118] JS：开发服务器
来源：http://wap.vehdjk.com/Article/details/goxdypzca.sHtML

npm i -D vite;  npx vite
来源：http://blog.fktsv.cn/Article/details/gpedkxsyt.sHtML

[U119] JS：生产构建
来源：http://mobile.tarul.cn/Article/details/gfjrxbjvi.sHtML

npx vite build
来源：http://baike.fktsv.cn/Article/details/gbvgumgow.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.yfazqb.com/Article/details/guntjmkki.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.sjlbkw.cn/Article/details/glxktopph.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grflzxtwu.sHtML

统计汇总
来源：http://www.m.share.bbcook.cn/Article/details/geaegrlfw.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gsguyhsqd.sHtML

按语言统计（条）：
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtgiuqbj.sHtML

Python ......... 252
来源：http://www.blog.vehdjk.com/Article/details/gcggpdabn.sHtML

PHP ............ 252
来源：http://read.share.vehdjk.com/Article/details/gwnlvdhzr.sHtML

JavaScript ..... 252
来源：http://www.share.yfazqb.com/Article/details/gvpaepujr.sHtML

TypeScript ..... 212
来源：http://wap.fktsv.cn/Article/details/gyepvhuhm.sHtML

Java ........... 212
来源：http://mobile.sjlbkw.cn/Article/details/gcjzkkvci.sHtML

Go ............. 212
来源：http://mobile.bbcook.cn/Article/details/gmibxvsdx.sHtML

Ruby ........... 212
来源：http://blog.sjlbkw.cn/Article/details/grxatffjv.sHtML

C# ............. 212
来源：http://www.share.vehdjk.com/Article/details/gcknjnxiu.sHtML

C .............. 30
来源：http://wap.bbcook.cn/Article/details/gkvyiillf.sHtML

C++ ............ 30
来源：http://www.m.share.epnwcf.com/Article/details/gkrxifuaa.sHtML

SQL ............ 90
来源：http://www.m.share.fktsv.cn/Article/details/gndvggrsj.sHtML

Bash ........... 80
来源：http://www.share.sjlbkw.cn/Article/details/gjmmqrsfw.sHtML

Kotlin ......... 15
来源：http://mobile.epnwcf.com/Article/details/guszrbmdq.sHtML

Swift .......... 15
来源：http://3g.fktsv.cn/Article/details/gobdserho.sHtML

Lua ............ 10
来源：http://www.m.share.bbcook.cn/Article/details/gxdcwonvt.sHtML

Perl ........... 10
来源：http://baike.bbcook.cn/Article/details/gsodbsrnj.sHtML

Scala .......... 10
来源：http://blog.yfazqb.com/Article/details/gbaxiqedd.sHtML

------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gaulwfedy.sHtML

合计 ........... 2106 条
来源：http://mobile.vehdjk.com/Article/details/gwozbesrh.sHtML

按章节统计：
来源：http://mobile.sjlbkw.cn/Article/details/gvjoyqnsh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.bbcook.cn/Article/details/gpddmuxyl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/gurirttec.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gqwforzgj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.tarul.cn/Article/details/gwpwmquhr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.tarul.cn/Article/details/gykojwmqj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.sjlbkw.cn/Article/details/gsfzizovd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gwosipacc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/geyaxkfpa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gsluaquah.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.tarul.cn/Article/details/gtllutswv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gkcpjimoy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gylrzdjun.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gjxsebusw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/glasaglou.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.vehdjk.com/Article/details/gjnxgqsbv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gmshwkhvx.sHtML

Q SQL 专题                              90
来源：http://mobile.bbcook.cn/Article/details/gygyhmqym.sHtML

R Bash 专题                             80
来源：http://mobile.tarul.cn/Article/details/gzbuzrxsl.sHtML

S C / C++ 专题                          60
来源：http://read.share.fktsv.cn/Article/details/gwerosnoo.sHtML

T 其他语言补充                          60
来源：http://baike.yfazqb.com/Article/details/glpgipqsc.sHtML

U 高频实用片段                         120
来源：http://read.share.fktsv.cn/Article/details/ggjjjabmp.sHtML

------------------------------------
来源：http://m.share.fktsv.cn/Article/details/goyiqnajr.sHtML

合计                                  2106 条
来源：http://m.share.fktsv.cn/Article/details/glxqpuiez.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gwqajuwwn.sHtML

使用提醒
来源：http://www.blog.epnwcf.com/Article/details/gluwisipi.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gjsbwfzbe.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.vehdjk.com/Article/details/gggnpeckr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fktsv.cn/Article/details/gppfswety.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.tarul.cn/Article/details/gemlpimfs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.epnwcf.com/Article/details/ggxoglktz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.yfazqb.com/Article/details/gsmkxerek.sHtML

—— 文件结束 ——
来源：http://www.share.epnwcf.com/Article/details/gxdpxvpip.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ggtbedecz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.epnwcf.com/Article/details/gfktoflja.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.bbcook.cn/Article/details/grrxefpxy.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gvilnjzix.sHtML

【收录内容】
来源：http://3g.sjlbkw.cn/Article/details/gjaodmrsp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fktsv.cn/Article/details/gztweipes.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.sjlbkw.cn/Article/details/gzmidztdb.sHtML

SQL · Bash · C · C++
来源：http://blog.fktsv.cn/Article/details/gxciaqwzm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.bbcook.cn/Article/details/gyunmkrpz.sHtML

【使用说明】
来源：http://read.share.bbcook.cn/Article/details/gsnqhrrpn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.yfazqb.com/Article/details/gvhypgnqg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.bbcook.cn/Article/details/gekpednme.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdacxhmp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.bbcook.cn/Article/details/gnzwhjwyr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.tarul.cn/Article/details/gctikxtrg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.vehdjk.com/Article/details/gzmtaxzmk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.vehdjk.com/Article/details/gggjwmbah.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.yfazqb.com/Article/details/gcuaukxks.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.sjlbkw.cn/Article/details/gzikwzzpt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.bbcook.cn/Article/details/gxihbfeyy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fktsv.cn/Article/details/gwntfebtl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.sjlbkw.cn/Article/details/ggrteaezl.sHtML

【文件统计】
来源：http://wap.sjlbkw.cn/Article/details/glwczqybw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.vehdjk.com/Article/details/geccwondg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/godxrgexl.sHtML

目  录
来源：http://3g.sjlbkw.cn/Article/details/guimrrnbt.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gswkamsac.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.tarul.cn/Article/details/gmocopjzy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.tarul.cn/Article/details/gvttmkhhp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.tarul.cn/Article/details/grbeglmjw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.yfazqb.com/Article/details/gotjbwuyv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gclvqggpp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.yfazqb.com/Article/details/guhgbbvbs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/gynlxqayi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.vehdjk.com/Article/details/gvuixhyiq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gbouwecsz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.bbcook.cn/Article/details/gjntewche.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/geksucypq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gxtsdbbij.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gevicjytb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.bbcook.cn/Article/details/glfzylqlb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.tarul.cn/Article/details/ghrzvjnwz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gyfpdtqqf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gnykmylqr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fktsv.cn/Article/details/gwvytxqdg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.sjlbkw.cn/Article/details/gsvyshdsk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/gkhkzqkgy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.tarul.cn/Article/details/gnjvnnsgx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gzwzudzcc.sHtML

A. 基础语法与类型
来源：http://www.m.share.vehdjk.com/Article/details/ggdyhivxw.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gijahzaec.sHtML

[A01] Hello World
来源：http://www.m.share.tarul.cn/Article/details/gptelayiv.sHtML

Py:   print("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gzmehlwpo.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.epnwcf.com/Article/details/glrdlkimh.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.vehdjk.com/Article/details/gbkqzkykp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.epnwcf.com/Article/details/gyxpcqich.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.epnwcf.com/Article/details/gfrfnqgtl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.vehdjk.com/Article/details/gerhbexfh.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.tarul.cn/Article/details/gklakwxrh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.sjlbkw.cn/Article/details/gsxgzjacb.sHtML

[A02] 变量声明与赋值
来源：http://blog.fktsv.cn/Article/details/gmzjepieo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.bbcook.cn/Article/details/gasfyyjns.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.yfazqb.com/Article/details/geaghdgum.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.epnwcf.com/Article/details/gprchwhje.sHtML


<!-- 参考信息 -->