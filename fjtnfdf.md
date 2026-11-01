代发 wailian999

[U31] Py：单测
来源：http://wap.fktsv.cn/Article/details/glageeiml.sHtML

python -m pytest -q
来源：http://www.blog.fktsv.cn/Article/details/grmwnshrx.sHtML

[U32] Py：代码格式化
来源：http://3g.epnwcf.com/Article/details/gerwsjqjm.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.tarul.cn/Article/details/gpmotycfl.sHtML

[U33] Py：打包发布
来源：http://www.blog.yfazqb.com/Article/details/ghqdshazl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.epnwcf.com/Article/details/gtnubzhww.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fktsv.cn/Article/details/gkjaxahmi.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/garkviway.sHtML

[U35] Py：发送邮件
来源：http://www.share.fktsv.cn/Article/details/gytwknfts.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.tarul.cn/Article/details/gtelelszk.sHtML

[U36] Py：定时任务
来源：http://read.share.fktsv.cn/Article/details/gtwcjwcej.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.bbcook.cn/Article/details/gpatadnzh.sHtML

[U37] Py：读写 Excel
来源：http://baike.yfazqb.com/Article/details/gakosxeyd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.epnwcf.com/Article/details/gpoveddra.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.tarul.cn/Article/details/gjovkrdnu.sHtML

Path(__file__).resolve().parent
来源：http://m.share.vehdjk.com/Article/details/gsupfrxur.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.vehdjk.com/Article/details/gkogqomhm.sHtML

sys.stdout.isatty()
来源：http://m.share.vehdjk.com/Article/details/gfnxieokf.sHtML

[U40] Py：打印到标准错误
来源：http://blog.sjlbkw.cn/Article/details/gqvgcyzzn.sHtML

print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gpgkzpxkk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.tarul.cn/Article/details/ghfblgbnt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.epnwcf.com/Article/details/grcsrunmw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.yfazqb.com/Article/details/ghwtohlbl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.vehdjk.com/Article/details/gtpkisnry.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.bbcook.cn/Article/details/gztpbujto.sHtML

namespace App\Http;
来源：http://read.share.epnwcf.com/Article/details/gaohdnwoy.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.bbcook.cn/Article/details/gqibyerok.sHtML

declare(strict_types=1);
来源：http://www.share.fktsv.cn/Article/details/gbbvzjedb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.tarul.cn/Article/details/gaueyxbqr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gswxqfpbm.sHtML

[U46] PHP：可空类型
来源：http://www.blog.yfazqb.com/Article/details/gtmcslybr.sHtML

?string $name = null
来源：http://www.share.vehdjk.com/Article/details/gudncrhni.sHtML

[U47] PHP：联合类型
来源：http://www.share.sjlbkw.cn/Article/details/gxgfmeeob.sHtML

int|string $id
来源：http://www.m.share.vehdjk.com/Article/details/gapxpoqgg.sHtML

[U48] PHP：纯枚举
来源：http://blog.epnwcf.com/Article/details/goxnkdlet.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.tarul.cn/Article/details/gmxzmpqfw.sHtML

[U49] PHP：只读属性
来源：http://m.share.yfazqb.com/Article/details/gstpzttle.sHtML

public readonly string $name
来源：http://wap.vehdjk.com/Article/details/gygvaguek.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.tarul.cn/Article/details/gfncvgsyb.sHtML

public function __construct(private int $id) {}
来源：http://baike.fktsv.cn/Article/details/gqbmjvuqu.sHtML

[U51] PHP：数组解构
来源：http://www.share.fktsv.cn/Article/details/geojpnjbx.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.vehdjk.com/Article/details/gcqqggsmd.sHtML

[U52] PHP：箭头函数
来源：http://read.share.yfazqb.com/Article/details/gfhtrjvpd.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fktsv.cn/Article/details/ggcbrtdpj.sHtML

[U53] PHP：空合并运算符
来源：http://3g.yfazqb.com/Article/details/gkmmsgvpn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.bbcook.cn/Article/details/gaspyuggf.sHtML

[U54] PHP：空安全调用
来源：http://wap.sjlbkw.cn/Article/details/guewniefc.sHtML

$obj?->method()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpapkpub.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fktsv.cn/Article/details/gorfqybsa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.sjlbkw.cn/Article/details/gjfpcamey.sHtML

[U56] PHP：命名参数
来源：http://www.blog.bbcook.cn/Article/details/gtzatnqzt.sHtML

f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gpgxzvzqd.sHtML

[U57] PHP：字符串插值
来源：http://3g.bbcook.cn/Article/details/gmttvqlnx.sHtML

"值: {$a}"
来源：http://m.share.fktsv.cn/Article/details/gzzfvbbnq.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.vehdjk.com/Article/details/gpkrltacw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fktsv.cn/Article/details/gyjqfntzs.sHtML

[U59] PHP：自定义排序
来源：http://wap.yfazqb.com/Article/details/gqlmmxuzm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gghegdyor.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.yfazqb.com/Article/details/gjlsmddsm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fktsv.cn/Article/details/gverzoxjm.sHtML

[U61] PHP：正则
来源：http://blog.vehdjk.com/Article/details/gkrbibjeo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.bbcook.cn/Article/details/gorgpzqcg.sHtML

[U62] PHP：日期对象
来源：http://read.share.vehdjk.com/Article/details/gompgtcko.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fktsv.cn/Article/details/gfefyitda.sHtML

[U63] PHP：文件读写
来源：http://m.share.sjlbkw.cn/Article/details/gaepvarwa.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.vehdjk.com/Article/details/gdwnxgntw.sHtML

[U64] PHP：目录遍历
来源：http://read.share.epnwcf.com/Article/details/gdncclltt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fktsv.cn/Article/details/gfvfxsqqx.sHtML

[U65] PHP：会话
来源：http://www.blog.tarul.cn/Article/details/grndywrla.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gleidfwht.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.vehdjk.com/Article/details/gdbdnjovr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.vehdjk.com/Article/details/gbdskzdaa.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.vehdjk.com/Article/details/gjwzebbmc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.vehdjk.com/Article/details/gqycavrsm.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.epnwcf.com/Article/details/goiualzud.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.vehdjk.com/Article/details/giizuvrsh.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.yfazqb.com/Article/details/gyhyygnfp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.vehdjk.com/Article/details/gnqfsucia.sHtML

[U70] PHP：PDO 事务
来源：http://3g.vehdjk.com/Article/details/gmnzrltlz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.sjlbkw.cn/Article/details/ghblfalxb.sHtML

[U71] PHP：抛出异常
来源：http://3g.yfazqb.com/Article/details/gasxdpvdu.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.yfazqb.com/Article/details/ghpyjizxs.sHtML

[U72] PHP：写错误日志
来源：http://blog.sjlbkw.cn/Article/details/gwohfplog.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.vehdjk.com/Article/details/gbgdpwohf.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.yfazqb.com/Article/details/ghcmwxizu.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.bbcook.cn/Article/details/gvyzyksnm.sHtML

[U74] PHP：读取环境变量
来源：http://wap.bbcook.cn/Article/details/gsesokzuj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.epnwcf.com/Article/details/gxuxkskxv.sHtML

[U75] PHP：依赖注入
来源：http://3g.vehdjk.com/Article/details/glvczupwt.sHtML

composer require psr/container
来源：http://www.m.share.fktsv.cn/Article/details/gkizjmfau.sHtML

[U76] PHP：简单路由
来源：http://mobile.tarul.cn/Article/details/gcuomxxpt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.tarul.cn/Article/details/gjfrectcl.sHtML

[U77] PHP：模板渲染
来源：http://wap.vehdjk.com/Article/details/gpbrskpfa.sHtML

composer require twig/twig
来源：http://read.share.epnwcf.com/Article/details/gcooekulp.sHtML

[U78] PHP：单元测试
来源：http://www.blog.epnwcf.com/Article/details/gawovsasb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.epnwcf.com/Article/details/gbjpwexvm.sHtML

[U79] PHP：静态分析
来源：http://3g.fktsv.cn/Article/details/gyeawsseq.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.bbcook.cn/Article/details/gqqqaxerv.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.bbcook.cn/Article/details/gbtjqhwki.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.vehdjk.com/Article/details/gybztmsiu.sHtML

[U81] JS：初始化项目
来源：http://baike.epnwcf.com/Article/details/ghokdqnzx.sHtML

npm init -y;  npm i express
来源：http://baike.epnwcf.com/Article/details/gphclvjrr.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.yfazqb.com/Article/details/gaqkshyua.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.sjlbkw.cn/Article/details/gdaghglxa.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fktsv.cn/Article/details/gzgzemstc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gmompnuti.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.bbcook.cn/Article/details/grruciwjz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.epnwcf.com/Article/details/gmjaqadpm.sHtML

[U85] JS：可选链
来源：http://baike.tarul.cn/Article/details/gxagvfabq.sHtML

a?.b?.c
来源：http://www.m.share.bbcook.cn/Article/details/gkqppsljl.sHtML

[U86] JS：空值合并
来源：http://baike.bbcook.cn/Article/details/ghuxwwgih.sHtML

a ?? b
来源：http://wap.yfazqb.com/Article/details/gntetlxwq.sHtML

[U87] JS：解构默认值
来源：http://mobile.yfazqb.com/Article/details/gaarhpjdb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.bbcook.cn/Article/details/gddzscisj.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.vehdjk.com/Article/details/gdekxorgm.sHtML

{ ...a, ...b }
来源：http://www.blog.vehdjk.com/Article/details/gtpunugfv.sHtML

[U89] JS：数组去重
来源：http://www.blog.sjlbkw.cn/Article/details/gknbcgsoe.sHtML

[...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gvgvnspcw.sHtML

[U90] JS：数字数组排序
来源：http://blog.vehdjk.com/Article/details/gnacytpgw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/gbcocxitt.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.tarul.cn/Article/details/gdlrrsmmd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fktsv.cn/Article/details/gionyljtj.sHtML

[U92] JS：深拷贝
来源：http://m.share.yfazqb.com/Article/details/gscphxlif.sHtML

structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gbfibiioj.sHtML

[U93] JS：模板字符串
来源：http://baike.tarul.cn/Article/details/grbkuypfq.sHtML

`共 ${n} 条`
来源：http://wap.epnwcf.com/Article/details/gcaipyqzo.sHtML

[U94] JS：箭头函数
来源：http://m.share.epnwcf.com/Article/details/ghqzmgsny.sHtML

const double = x => x * 2;
来源：http://3g.fktsv.cn/Article/details/gfxqohzrk.sHtML

[U95] JS：Promise 包装
来源：http://m.share.tarul.cn/Article/details/glnpcpiod.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.bbcook.cn/Article/details/gbhhpfzwm.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.epnwcf.com/Article/details/gikjlmrof.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/guvorqglq.sHtML

[U97] JS：并发请求
来源：http://www.share.fktsv.cn/Article/details/gtaccziwm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gsgdglees.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fktsv.cn/Article/details/gbndbxhzl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fktsv.cn/Article/details/guhsfajsz.sHtML

[U99] JS：事件监听
来源：http://www.m.share.epnwcf.com/Article/details/gnoftmkzm.sHtML

el.addEventListener("click", e => {})
来源：http://blog.epnwcf.com/Article/details/gunnzadgg.sHtML

[U100] JS：DOM 查询
来源：http://read.share.tarul.cn/Article/details/gyvgljoas.sHtML

document.querySelector(".item")
来源：http://read.share.tarul.cn/Article/details/ghyrxxboo.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.tarul.cn/Article/details/gleoghejf.sHtML

el.classList.toggle("active")
来源：http://mobile.epnwcf.com/Article/details/ghiaeokwr.sHtML

[U102] JS：本地存储
来源：http://wap.tarul.cn/Article/details/gqoyuuqmq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.sjlbkw.cn/Article/details/gpvoawwgv.sHtML

[U103] JS：定时器
来源：http://www.blog.tarul.cn/Article/details/gnawsiixw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.vehdjk.com/Article/details/gtwnriaat.sHtML

[U104] JS：防抖
来源：http://mobile.fktsv.cn/Article/details/grtvnfpgz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/glwdtkwul.sHtML

[U105] JS：节流
来源：http://wap.epnwcf.com/Article/details/gfqiykhnm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fktsv.cn/Article/details/gyaitusql.sHtML

[U106] JS：日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/gjnrynhgg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.sjlbkw.cn/Article/details/gzxfuzauz.sHtML

[U107] JS：数字千分位
来源：http://www.blog.vehdjk.com/Article/details/gpsnicrdf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.bbcook.cn/Article/details/guspvhavo.sHtML

[U108] JS：随机整数
来源：http://www.blog.epnwcf.com/Article/details/glzenjjjv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.bbcook.cn/Article/details/gpyzwfuvw.sHtML

[U109] JS：数组分组
来源：http://mobile.sjlbkw.cn/Article/details/gjcrwottx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gmvmltugs.sHtML

[U110] JS：数组分块
来源：http://blog.tarul.cn/Article/details/gtdolqtlv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.tarul.cn/Article/details/glsubbimo.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fktsv.cn/Article/details/gjccdwytu.sHtML

new Map(Object.entries(obj))
来源：http://wap.epnwcf.com/Article/details/gqwecldpw.sHtML

[U112] JS：字符串补位
来源：http://blog.fktsv.cn/Article/details/gbaygjbxp.sHtML

"7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/ghezcickk.sHtML

[U113] JS：正则替换全部
来源：http://wap.tarul.cn/Article/details/ghhjxticu.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/galjvznst.sHtML

[U114] JS：JSON 深比较
来源：http://wap.bbcook.cn/Article/details/gvzoxvocf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gobgmqzaq.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fktsv.cn/Article/details/guzdcotod.sHtML

crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/ghlxuwdxs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.bbcook.cn/Article/details/gesffxpea.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.tarul.cn/Article/details/guvnoeiet.sHtML

[U117] JS：单元测试
来源：http://www.m.share.bbcook.cn/Article/details/grgtnhhbj.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.epnwcf.com/Article/details/gxwsaepqf.sHtML

[U118] JS：开发服务器
来源：http://m.share.yfazqb.com/Article/details/gsmcbjobr.sHtML

npm i -D vite;  npx vite
来源：http://3g.vehdjk.com/Article/details/gvjslnasn.sHtML

[U119] JS：生产构建
来源：http://mobile.tarul.cn/Article/details/gxuaousfy.sHtML

npx vite build
来源：http://wap.yfazqb.com/Article/details/guqgacgvj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.tarul.cn/Article/details/gxdffdirs.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.vehdjk.com/Article/details/gfkgnmuoh.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glvuqttqx.sHtML

统计汇总
来源：http://www.blog.tarul.cn/Article/details/gdviovmer.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gbnlunbiy.sHtML

按语言统计（条）：
来源：http://m.share.yfazqb.com/Article/details/gofaeyhnk.sHtML

Python ......... 252
来源：http://read.share.vehdjk.com/Article/details/gvkkhsyoi.sHtML

PHP ............ 252
来源：http://m.share.tarul.cn/Article/details/gbmclctvx.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/ghfdocvri.sHtML

TypeScript ..... 212
来源：http://www.m.share.yfazqb.com/Article/details/gtqoqplsk.sHtML

Java ........... 212
来源：http://www.blog.epnwcf.com/Article/details/ghrrafqty.sHtML

Go ............. 212
来源：http://mobile.fktsv.cn/Article/details/grtvdhfuq.sHtML

Ruby ........... 212
来源：http://baike.fktsv.cn/Article/details/gsagsxhog.sHtML

C# ............. 212
来源：http://mobile.epnwcf.com/Article/details/gdcslojnf.sHtML

C .............. 30
来源：http://mobile.bbcook.cn/Article/details/goyroiizm.sHtML

C++ ............ 30
来源：http://m.share.sjlbkw.cn/Article/details/gkmfccdxu.sHtML

SQL ............ 90
来源：http://www.share.tarul.cn/Article/details/guezxlxup.sHtML

Bash ........... 80
来源：http://baike.sjlbkw.cn/Article/details/gjhqafzeh.sHtML

Kotlin ......... 15
来源：http://m.share.bbcook.cn/Article/details/gsgdvtzyy.sHtML

Swift .......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcnuybli.sHtML

Lua ............ 10
来源：http://www.m.share.epnwcf.com/Article/details/gvpqrtctq.sHtML

Perl ........... 10
来源：http://baike.yfazqb.com/Article/details/ghvpzmwgr.sHtML

Scala .......... 10
来源：http://www.m.share.epnwcf.com/Article/details/grtmzfeja.sHtML

------------------------------------
来源：http://blog.yfazqb.com/Article/details/gfpxbiuqv.sHtML

合计 ........... 2106 条
来源：http://mobile.tarul.cn/Article/details/gugavvcnb.sHtML

按章节统计：
来源：http://www.share.fktsv.cn/Article/details/gzdkybeyf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/gzkqvtulg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkmfeesm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/gyqkavulv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/gfymmhjuw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.tarul.cn/Article/details/gxzekqylq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.epnwcf.com/Article/details/gkocbzeys.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/gyfiqdbad.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fktsv.cn/Article/details/gpovzkwhf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gsqpsxhfb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/gjvdxhwub.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gawaoggvi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gqiwmfabq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gapztduwy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.epnwcf.com/Article/details/gdrezykvg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.yfazqb.com/Article/details/gkslxffvc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gzlulffvj.sHtML

Q SQL 专题                              90
来源：http://3g.fktsv.cn/Article/details/ggisxwhel.sHtML

R Bash 专题                             80
来源：http://blog.fktsv.cn/Article/details/gtzcfnyxs.sHtML

S C / C++ 专题                          60
来源：http://m.share.tarul.cn/Article/details/geuihepbv.sHtML

T 其他语言补充                          60
来源：http://mobile.sjlbkw.cn/Article/details/gvtfpsabi.sHtML

U 高频实用片段                         120
来源：http://3g.sjlbkw.cn/Article/details/gpwredbsy.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/gcbfsvnup.sHtML

合计                                  2106 条
来源：http://wap.yfazqb.com/Article/details/gowthwjqt.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gclibnaqu.sHtML

使用提醒
来源：http://3g.bbcook.cn/Article/details/grldhvqsd.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gekxhvriv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.tarul.cn/Article/details/glspnlsyb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.vehdjk.com/Article/details/goczelkwc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.bbcook.cn/Article/details/gzasqtdrr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.tarul.cn/Article/details/gkbuxoohv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.yfazqb.com/Article/details/golvloodq.sHtML

—— 文件结束 ——
来源：http://wap.fktsv.cn/Article/details/gcyervlca.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmghzviex.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.tarul.cn/Article/details/gxznoxrxv.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.vehdjk.com/Article/details/gvilfjhhu.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gavuffmde.sHtML

【收录内容】
来源：http://m.share.bbcook.cn/Article/details/gafnnqrmc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.epnwcf.com/Article/details/gbhnunuxp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.yfazqb.com/Article/details/gpeyrifhb.sHtML

SQL · Bash · C · C++
来源：http://www.blog.sjlbkw.cn/Article/details/gttvjsvjk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.epnwcf.com/Article/details/ggvwgnmof.sHtML

【使用说明】
来源：http://www.share.fktsv.cn/Article/details/gknpvrnty.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.tarul.cn/Article/details/ginetykws.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.epnwcf.com/Article/details/glyejhkfu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.bbcook.cn/Article/details/gafaheiep.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.yfazqb.com/Article/details/gemosysbn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.vehdjk.com/Article/details/ghxvfqwow.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.sjlbkw.cn/Article/details/geihqabwr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.vehdjk.com/Article/details/gjeszskdb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fktsv.cn/Article/details/ghfnhmdjf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.tarul.cn/Article/details/gzbvcaata.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.epnwcf.com/Article/details/gvqwzqzbi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.vehdjk.com/Article/details/gojnddlhu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.vehdjk.com/Article/details/gdflmurqj.sHtML

【文件统计】
来源：http://blog.epnwcf.com/Article/details/gnyumkbhw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.epnwcf.com/Article/details/gfpjpacqg.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/gzhfbekme.sHtML

目  录
来源：http://baike.bbcook.cn/Article/details/gtdykvmen.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gpszaecns.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.yfazqb.com/Article/details/guzcvbwvt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/gcjihwlfu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.epnwcf.com/Article/details/gfitzidhb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fktsv.cn/Article/details/ghvdfbttc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.bbcook.cn/Article/details/gobrdwxvv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gihlnzzdf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gyoygocfn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.vehdjk.com/Article/details/gjmqaixnh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/gecrjvggm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.yfazqb.com/Article/details/gwrofjcvz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/grihxxzej.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/giqlzhdha.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gfpzcmlab.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.sjlbkw.cn/Article/details/goixwdqji.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fktsv.cn/Article/details/gbxpkhwta.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gmjjyebve.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.vehdjk.com/Article/details/gqhjunwgy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.tarul.cn/Article/details/gpjbejgun.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.vehdjk.com/Article/details/glzbqbiuh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gwrapdfpk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.vehdjk.com/Article/details/ggirofrmc.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gplbsixqj.sHtML

A. 基础语法与类型
来源：http://www.share.yfazqb.com/Article/details/grqmsmmji.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gtwkhswqy.sHtML

[A01] Hello World
来源：http://www.share.tarul.cn/Article/details/gddhqfbud.sHtML

Py:   print("Hello, World!")
来源：http://baike.yfazqb.com/Article/details/gzjpsbgoj.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.bbcook.cn/Article/details/gxsjlyaoh.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.yfazqb.com/Article/details/gmnigqryd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzafboek.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/gpafyvjid.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.epnwcf.com/Article/details/gpmkntdwv.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.sjlbkw.cn/Article/details/guuprctzo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.tarul.cn/Article/details/ghhucicbf.sHtML

[A02] 变量声明与赋值
来源：http://read.share.bbcook.cn/Article/details/gcxwshbwl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.epnwcf.com/Article/details/goaqszojt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.bbcook.cn/Article/details/gkbbxwium.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fktsv.cn/Article/details/gogdkzynh.sHtML


<!-- 参考信息 -->