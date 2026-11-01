代发 wailian999

[U31] Py：单测
来源：http://baike.bbcook.cn/Article/details/gmugsrewe.sHtML

python -m pytest -q
来源：http://blog.fktsv.cn/Article/details/gpzameuxz.sHtML

[U32] Py：代码格式化
来源：http://baike.bbcook.cn/Article/details/gmrbvbbgg.sHtML

ruff format . && ruff check --fix .
来源：http://baike.bbcook.cn/Article/details/glnbxrhpx.sHtML

[U33] Py：打包发布
来源：http://www.share.yfazqb.com/Article/details/gghfllxax.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.tarul.cn/Article/details/gqxavrdzh.sHtML

[U34] Py：判断编码
来源：http://read.share.yfazqb.com/Article/details/gyhalsftn.sHtML

chardet.detect(raw)
来源：http://wap.tarul.cn/Article/details/gpfhjfiag.sHtML

[U35] Py：发送邮件
来源：http://wap.yfazqb.com/Article/details/gznhpxjea.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.epnwcf.com/Article/details/gilettqtk.sHtML

[U36] Py：定时任务
来源：http://3g.vehdjk.com/Article/details/goveswmbr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.tarul.cn/Article/details/gnmrhdtsv.sHtML

[U37] Py：读写 Excel
来源：http://baike.bbcook.cn/Article/details/gtijpxklz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.yfazqb.com/Article/details/gjjyirliu.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.bbcook.cn/Article/details/gqnmvqtsi.sHtML

Path(__file__).resolve().parent
来源：http://read.share.yfazqb.com/Article/details/gzzwkywst.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.epnwcf.com/Article/details/gmvdqotbv.sHtML

sys.stdout.isatty()
来源：http://m.share.fktsv.cn/Article/details/gbxowwpwz.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.sjlbkw.cn/Article/details/ghemrinfp.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gzpixkoeb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.epnwcf.com/Article/details/gpffevxac.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.bbcook.cn/Article/details/gfreyiqnl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.bbcook.cn/Article/details/ggqxuyqmr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.yfazqb.com/Article/details/ghpdlhtly.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.sjlbkw.cn/Article/details/gyuyibjlq.sHtML

namespace App\Http;
来源：http://m.share.sjlbkw.cn/Article/details/gybvdqxos.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.sjlbkw.cn/Article/details/gxgmxfmiy.sHtML

declare(strict_types=1);
来源：http://m.share.fktsv.cn/Article/details/gswjzynjq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.epnwcf.com/Article/details/gfoxojpuk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gmonqkjul.sHtML

[U46] PHP：可空类型
来源：http://m.share.epnwcf.com/Article/details/gowlplnjs.sHtML

?string $name = null
来源：http://www.share.bbcook.cn/Article/details/ggihlhgng.sHtML

[U47] PHP：联合类型
来源：http://www.blog.sjlbkw.cn/Article/details/gzssqzqnj.sHtML

int|string $id
来源：http://mobile.bbcook.cn/Article/details/gcknwziui.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.tarul.cn/Article/details/gepkjuzde.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.vehdjk.com/Article/details/gljwzhuac.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdnglwng.sHtML

public readonly string $name
来源：http://www.blog.vehdjk.com/Article/details/gtvvnjiin.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.tarul.cn/Article/details/goucbmwmi.sHtML

public function __construct(private int $id) {}
来源：http://baike.yfazqb.com/Article/details/gzmttdedv.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.epnwcf.com/Article/details/gmxolwsxx.sHtML

[$a, $b] = $arr;
来源：http://mobile.sjlbkw.cn/Article/details/gbjdarowy.sHtML

[U52] PHP：箭头函数
来源：http://3g.epnwcf.com/Article/details/gcxxylqbo.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.vehdjk.com/Article/details/gojkndujb.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.sjlbkw.cn/Article/details/ggyqjoaud.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.yfazqb.com/Article/details/gapjsbzjz.sHtML

[U54] PHP：空安全调用
来源：http://wap.yfazqb.com/Article/details/gdjtvgdyy.sHtML

$obj?->method()
来源：http://baike.yfazqb.com/Article/details/ghtjjuhvf.sHtML

[U55] PHP：match 表达式
来源：http://mobile.sjlbkw.cn/Article/details/gqxxwxqws.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gethndsrg.sHtML

[U56] PHP：命名参数
来源：http://wap.yfazqb.com/Article/details/gevxcedix.sHtML

f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gfutezfcz.sHtML

[U57] PHP：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gjimywnya.sHtML

"值: {$a}"
来源：http://m.share.epnwcf.com/Article/details/gnloprbwu.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.bbcook.cn/Article/details/gwgsqeokq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.sjlbkw.cn/Article/details/gskvpsmhc.sHtML

[U59] PHP：自定义排序
来源：http://read.share.tarul.cn/Article/details/gucvttpvd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.bbcook.cn/Article/details/gtyiafrtm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.sjlbkw.cn/Article/details/gjpnkujvm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.vehdjk.com/Article/details/golullnkl.sHtML

[U61] PHP：正则
来源：http://mobile.vehdjk.com/Article/details/gwuogyhun.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.sjlbkw.cn/Article/details/gzestcciw.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.yfazqb.com/Article/details/gbnbwhkif.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.yfazqb.com/Article/details/gaelsgkib.sHtML

[U63] PHP：文件读写
来源：http://baike.fktsv.cn/Article/details/gpmrqhzzh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.tarul.cn/Article/details/guozpovzz.sHtML

[U64] PHP：目录遍历
来源：http://3g.sjlbkw.cn/Article/details/gufathldg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.yfazqb.com/Article/details/gfgmkybms.sHtML

[U65] PHP：会话
来源：http://mobile.fktsv.cn/Article/details/gxldjbnvk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.bbcook.cn/Article/details/gqxlmgxxl.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.tarul.cn/Article/details/genyatvha.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.sjlbkw.cn/Article/details/gjgwchqnk.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fktsv.cn/Article/details/gkrqulbef.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.vehdjk.com/Article/details/gsfwfrsxj.sHtML

[U68] PHP：PDO 连接
来源：http://3g.tarul.cn/Article/details/ggdxuyeuu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.bbcook.cn/Article/details/gmwmgypmz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fktsv.cn/Article/details/gymfgkenm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.vehdjk.com/Article/details/giadqmsjh.sHtML

[U70] PHP：PDO 事务
来源：http://baike.tarul.cn/Article/details/gbczrsvqa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/gfzfzqhqq.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gjncmmgyw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.epnwcf.com/Article/details/gnxqkivkv.sHtML

[U72] PHP：写错误日志
来源：http://mobile.sjlbkw.cn/Article/details/gqtojmrlm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.epnwcf.com/Article/details/gxusbfbxd.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.vehdjk.com/Article/details/glzrqmkhl.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.bbcook.cn/Article/details/gidyskurc.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.tarul.cn/Article/details/ggsygnhnr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.sjlbkw.cn/Article/details/gzqfmjvrr.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.epnwcf.com/Article/details/gqkuafhxg.sHtML

composer require psr/container
来源：http://read.share.yfazqb.com/Article/details/gwsgwxgof.sHtML

[U76] PHP：简单路由
来源：http://baike.yfazqb.com/Article/details/gxuemkyop.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.vehdjk.com/Article/details/gngvahobm.sHtML

[U77] PHP：模板渲染
来源：http://read.share.bbcook.cn/Article/details/gxzotijza.sHtML

composer require twig/twig
来源：http://mobile.epnwcf.com/Article/details/gdjztlswx.sHtML

[U78] PHP：单元测试
来源：http://wap.bbcook.cn/Article/details/gpocfamum.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.epnwcf.com/Article/details/gmbbdxepz.sHtML

[U79] PHP：静态分析
来源：http://3g.tarul.cn/Article/details/gkghcahbg.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.vehdjk.com/Article/details/gkqdatcfz.sHtML

[U80] PHP：代码规范修复
来源：http://baike.yfazqb.com/Article/details/gouzoitxy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnsshfeu.sHtML

[U81] JS：初始化项目
来源：http://www.blog.tarul.cn/Article/details/grpmxursy.sHtML

npm init -y;  npm i express
来源：http://3g.vehdjk.com/Article/details/gyoblwiok.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.yfazqb.com/Article/details/gdnyrqlkn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.tarul.cn/Article/details/gthjpfwaw.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.bbcook.cn/Article/details/gfploavbh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.bbcook.cn/Article/details/gidjpqoqo.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fktsv.cn/Article/details/gltluabzs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.bbcook.cn/Article/details/ggfyyanuh.sHtML

[U85] JS：可选链
来源：http://m.share.epnwcf.com/Article/details/gyjbysaxj.sHtML

a?.b?.c
来源：http://read.share.yfazqb.com/Article/details/gjcpbedgl.sHtML

[U86] JS：空值合并
来源：http://m.share.tarul.cn/Article/details/gtfdrodrz.sHtML

a ?? b
来源：http://blog.sjlbkw.cn/Article/details/gvqcueksg.sHtML

[U87] JS：解构默认值
来源：http://mobile.bbcook.cn/Article/details/guclobedp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.yfazqb.com/Article/details/goayhmpmz.sHtML

[U88] JS：对象展开合并
来源：http://read.share.vehdjk.com/Article/details/galkmtpry.sHtML

{ ...a, ...b }
来源：http://www.m.share.yfazqb.com/Article/details/ggcvsphja.sHtML

[U89] JS：数组去重
来源：http://baike.yfazqb.com/Article/details/gqcliaxkw.sHtML

[...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gcitcpbdl.sHtML

[U90] JS：数字数组排序
来源：http://mobile.yfazqb.com/Article/details/ggqrpzljs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gnwaorlad.sHtML

[U91] JS：对象键值遍历
来源：http://blog.yfazqb.com/Article/details/gsjdkjzoa.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fktsv.cn/Article/details/gtkfmamls.sHtML

[U92] JS：深拷贝
来源：http://www.share.bbcook.cn/Article/details/gmtrjdxti.sHtML

structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gjtxacuji.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.yfazqb.com/Article/details/gcskbioth.sHtML

`共 ${n} 条`
来源：http://www.share.epnwcf.com/Article/details/gvfhhhpoo.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.tarul.cn/Article/details/gserpbmuw.sHtML

const double = x => x * 2;
来源：http://3g.bbcook.cn/Article/details/ggpzhjtts.sHtML

[U95] JS：Promise 包装
来源：http://3g.tarul.cn/Article/details/gjzwvrgcz.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.yfazqb.com/Article/details/gqzeornyb.sHtML

[U96] JS：async/await 与异常
来源：http://blog.epnwcf.com/Article/details/gctbkumpg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gqrypldcn.sHtML

[U97] JS：并发请求
来源：http://blog.sjlbkw.cn/Article/details/gtjiiywum.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/gvnujsxfl.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.yfazqb.com/Article/details/ghrwztcts.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.tarul.cn/Article/details/gugjzhrrs.sHtML

[U99] JS：事件监听
来源：http://mobile.epnwcf.com/Article/details/giddeomau.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.bbcook.cn/Article/details/gvkjrecuc.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.epnwcf.com/Article/details/gvlqvptoq.sHtML

document.querySelector(".item")
来源：http://baike.tarul.cn/Article/details/gwfkdcjgq.sHtML

[U101] JS：classList 操作
来源：http://3g.fktsv.cn/Article/details/gfveqakgh.sHtML

el.classList.toggle("active")
来源：http://www.blog.bbcook.cn/Article/details/gqpgydksa.sHtML

[U102] JS：本地存储
来源：http://mobile.fktsv.cn/Article/details/gdspddwcw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fktsv.cn/Article/details/gcuqohxwx.sHtML

[U103] JS：定时器
来源：http://m.share.epnwcf.com/Article/details/gznotqzry.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.yfazqb.com/Article/details/gvbysxbwy.sHtML

[U104] JS：防抖
来源：http://wap.vehdjk.com/Article/details/gdmknzict.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gfpivyfcl.sHtML

[U105] JS：节流
来源：http://mobile.sjlbkw.cn/Article/details/gylricpyo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.yfazqb.com/Article/details/grqudzzqi.sHtML

[U106] JS：日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gocrfogqr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fktsv.cn/Article/details/gxvlmxbev.sHtML

[U107] JS：数字千分位
来源：http://baike.epnwcf.com/Article/details/gyvkdmeeu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gruikmbys.sHtML

[U108] JS：随机整数
来源：http://read.share.epnwcf.com/Article/details/gwmxnrcpv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.tarul.cn/Article/details/gimlmytdc.sHtML

[U109] JS：数组分组
来源：http://baike.vehdjk.com/Article/details/gystjnrpb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gynxjmwrh.sHtML

[U110] JS：数组分块
来源：http://3g.sjlbkw.cn/Article/details/gzmgpfzxq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.vehdjk.com/Article/details/gudxoiuuy.sHtML

[U111] JS：对象转 Map
来源：http://m.share.sjlbkw.cn/Article/details/gsxovygsd.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.yfazqb.com/Article/details/ghvejpdea.sHtML

[U112] JS：字符串补位
来源：http://blog.fktsv.cn/Article/details/gsivjxvav.sHtML

"7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gwktcdjfl.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fktsv.cn/Article/details/gbgnkgnlg.sHtML

s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gslyklrfk.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.tarul.cn/Article/details/ghopdxfiw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gexnwfgnb.sHtML

[U115] JS：生成 UUID
来源：http://mobile.epnwcf.com/Article/details/gqquvgymn.sHtML

crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/gnnfkfwcj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.yfazqb.com/Article/details/gutmxlfse.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gacovsjpx.sHtML

[U117] JS：单元测试
来源：http://baike.vehdjk.com/Article/details/gkestfeqk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.vehdjk.com/Article/details/gpetkelwq.sHtML

[U118] JS：开发服务器
来源：http://3g.vehdjk.com/Article/details/gcdyexzwz.sHtML

npm i -D vite;  npx vite
来源：http://read.share.bbcook.cn/Article/details/gorkfofpz.sHtML

[U119] JS：生产构建
来源：http://www.m.share.vehdjk.com/Article/details/guljbacqa.sHtML

npx vite build
来源：http://www.blog.tarul.cn/Article/details/gnzaxasyg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.epnwcf.com/Article/details/gxnewfajd.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fktsv.cn/Article/details/gypvqggcn.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/grkxoasko.sHtML

统计汇总
来源：http://www.m.share.vehdjk.com/Article/details/gfyugxlpv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzvokgaef.sHtML

按语言统计（条）：
来源：http://www.blog.tarul.cn/Article/details/grplsssho.sHtML

Python ......... 252
来源：http://read.share.yfazqb.com/Article/details/gqeoysfal.sHtML

PHP ............ 252
来源：http://www.m.share.sjlbkw.cn/Article/details/ghituuttp.sHtML

JavaScript ..... 252
来源：http://wap.bbcook.cn/Article/details/gualesxkj.sHtML

TypeScript ..... 212
来源：http://www.share.tarul.cn/Article/details/grwusljzi.sHtML

Java ........... 212
来源：http://read.share.yfazqb.com/Article/details/grjoxgnad.sHtML

Go ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gmvmzxjrl.sHtML

Ruby ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gpwhuvpqs.sHtML

C# ............. 212
来源：http://mobile.sjlbkw.cn/Article/details/gqnxusucc.sHtML

C .............. 30
来源：http://mobile.sjlbkw.cn/Article/details/gofxdffzt.sHtML

C++ ............ 30
来源：http://blog.vehdjk.com/Article/details/goasblvzy.sHtML

SQL ............ 90
来源：http://wap.sjlbkw.cn/Article/details/gkyjmnkdz.sHtML

Bash ........... 80
来源：http://blog.sjlbkw.cn/Article/details/gogzrtmhk.sHtML

Kotlin ......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gyippyfcs.sHtML

Swift .......... 15
来源：http://m.share.fktsv.cn/Article/details/glcmwjvja.sHtML

Lua ............ 10
来源：http://www.blog.sjlbkw.cn/Article/details/gslmhdjvc.sHtML

Perl ........... 10
来源：http://blog.bbcook.cn/Article/details/ghnsholmm.sHtML

Scala .......... 10
来源：http://m.share.sjlbkw.cn/Article/details/grpzszvce.sHtML

------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gxbjsvtmd.sHtML

合计 ........... 2106 条
来源：http://wap.epnwcf.com/Article/details/ghxuhpapj.sHtML

按章节统计：
来源：http://read.share.yfazqb.com/Article/details/gymjhumai.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.epnwcf.com/Article/details/gzmjuidqp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gtuaavuas.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/gvhqorxwf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.sjlbkw.cn/Article/details/gftjlxuzl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.vehdjk.com/Article/details/gbzbelifh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.yfazqb.com/Article/details/grzllejpg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gjsvxyqds.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.vehdjk.com/Article/details/geiizvhwj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gxuziunhx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.epnwcf.com/Article/details/gtdguubll.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gwfgipnzm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnvyjfnm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gqhwdsweq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gmivesvin.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.tarul.cn/Article/details/gfdrbxrcz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/giwwdzoet.sHtML

Q SQL 专题                              90
来源：http://baike.sjlbkw.cn/Article/details/grbipnpwz.sHtML

R Bash 专题                             80
来源：http://www.share.tarul.cn/Article/details/ghmoxbejw.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fktsv.cn/Article/details/gjnqbueys.sHtML

T 其他语言补充                          60
来源：http://www.blog.vehdjk.com/Article/details/gsmstclau.sHtML

U 高频实用片段                         120
来源：http://m.share.tarul.cn/Article/details/gkftobvdu.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gegbiwwsn.sHtML

合计                                  2106 条
来源：http://wap.yfazqb.com/Article/details/gjhewatac.sHtML

--------------------------------------------------------------------------------
来源：http://blog.epnwcf.com/Article/details/geutiwtln.sHtML

使用提醒
来源：http://www.m.share.bbcook.cn/Article/details/gkgqkkkzs.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/gffudcczc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fktsv.cn/Article/details/grvzfssxd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.yfazqb.com/Article/details/godawbrrt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.yfazqb.com/Article/details/gyemdpnjl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.tarul.cn/Article/details/gkhweqjgc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fktsv.cn/Article/details/gsrupnccc.sHtML

—— 文件结束 ——
来源：http://baike.tarul.cn/Article/details/gxibyqdvd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gzqtqoitd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.epnwcf.com/Article/details/gzumbdvdf.sHtML

Common Programming Examples Cheat Book
来源：http://wap.bbcook.cn/Article/details/gwkamfgfk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gxotjechv.sHtML

【收录内容】
来源：http://www.share.tarul.cn/Article/details/gimzenrpu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.bbcook.cn/Article/details/gqltdvcug.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.epnwcf.com/Article/details/genduiswf.sHtML

SQL · Bash · C · C++
来源：http://mobile.sjlbkw.cn/Article/details/ggxcmqcyw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fktsv.cn/Article/details/gdrskueur.sHtML

【使用说明】
来源：http://www.m.share.vehdjk.com/Article/details/gquaxhqvk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.yfazqb.com/Article/details/gbaodazzf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fktsv.cn/Article/details/gfxtjanzx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.vehdjk.com/Article/details/gmlicdkfz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.epnwcf.com/Article/details/gwkjunxom.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fktsv.cn/Article/details/gyqelnsvy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.epnwcf.com/Article/details/gejwqmdcw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.tarul.cn/Article/details/garygwysk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.yfazqb.com/Article/details/gdgfkfmxt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.vehdjk.com/Article/details/gimzfkcam.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.bbcook.cn/Article/details/gjiprssmz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.tarul.cn/Article/details/gsmbyzzqp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.sjlbkw.cn/Article/details/gukahiinj.sHtML

【文件统计】
来源：http://3g.bbcook.cn/Article/details/gvohbrnfi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.tarul.cn/Article/details/gycijdjvb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gvrmyecgx.sHtML

目  录
来源：http://baike.tarul.cn/Article/details/goyercuff.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/gsqcqlvqq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.bbcook.cn/Article/details/gpzgtbxhl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fktsv.cn/Article/details/gbyxgwxzo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.vehdjk.com/Article/details/gseazwiip.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.tarul.cn/Article/details/gemdhlooq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.yfazqb.com/Article/details/giuurxtbk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fktsv.cn/Article/details/gctohsdzh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/ggsemroxw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gdqshlswg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gjugzsish.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.epnwcf.com/Article/details/ggqacyycr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gveskkdft.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.yfazqb.com/Article/details/gyqrjowld.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.tarul.cn/Article/details/gfxkdljkl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.vehdjk.com/Article/details/gsolnutov.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.sjlbkw.cn/Article/details/gthentxhq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/guyhdxoqj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.sjlbkw.cn/Article/details/ggunchxly.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.bbcook.cn/Article/details/gxohrjykm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.tarul.cn/Article/details/gbxibbqel.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gujetafpc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.tarul.cn/Article/details/ghwewjrdl.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/goasiesif.sHtML

A. 基础语法与类型
来源：http://www.m.share.bbcook.cn/Article/details/gbzlxrsex.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/giitskiov.sHtML

[A01] Hello World
来源：http://www.share.bbcook.cn/Article/details/gxawzytxn.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.bbcook.cn/Article/details/gsbmkqicj.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.bbcook.cn/Article/details/gppsyvipv.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fktsv.cn/Article/details/gjiuibvlg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.sjlbkw.cn/Article/details/gatadbiwv.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/gmbdrszpa.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.sjlbkw.cn/Article/details/gnicydhul.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.tarul.cn/Article/details/gzwryqqge.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.vehdjk.com/Article/details/gyzwcktiy.sHtML

[A02] 变量声明与赋值
来源：http://read.share.epnwcf.com/Article/details/gjvzbmckf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.bbcook.cn/Article/details/gmupozcwt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fktsv.cn/Article/details/gdaofrjji.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.epnwcf.com/Article/details/ghceatupq.sHtML


<!-- 参考信息 -->