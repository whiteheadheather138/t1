代发 wailian999

[U33] Py：打包发布
来源：http://3g.fktsv.cn/Article/details/gazedtxsv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.sjlbkw.cn/Article/details/glozjkkxm.sHtML

[U34] Py：判断编码
来源：http://m.share.yfazqb.com/Article/details/goakvupqx.sHtML

chardet.detect(raw)
来源：http://3g.sjlbkw.cn/Article/details/gijxopgbx.sHtML

[U35] Py：发送邮件
来源：http://www.share.vehdjk.com/Article/details/gamvwxnsg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fktsv.cn/Article/details/gwwcomwcb.sHtML

[U36] Py：定时任务
来源：http://www.share.epnwcf.com/Article/details/geligfksi.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.yfazqb.com/Article/details/gueakkbjx.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.bbcook.cn/Article/details/gckirgwrp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.yfazqb.com/Article/details/gauyapspy.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.bbcook.cn/Article/details/galrjskax.sHtML

Path(__file__).resolve().parent
来源：http://wap.fktsv.cn/Article/details/gulxnpxzr.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.epnwcf.com/Article/details/guhsozbfn.sHtML

sys.stdout.isatty()
来源：http://mobile.yfazqb.com/Article/details/gscbrdxuj.sHtML

[U40] Py：打印到标准错误
来源：http://wap.bbcook.cn/Article/details/gkarpndwh.sHtML

print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gwjnxbbiy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.vehdjk.com/Article/details/gnkjmwngd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.sjlbkw.cn/Article/details/gradndbcp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.sjlbkw.cn/Article/details/gqorjdocw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.vehdjk.com/Article/details/gaweibnre.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.vehdjk.com/Article/details/gqjrpjtwv.sHtML

namespace App\Http;
来源：http://wap.bbcook.cn/Article/details/gsrejhmot.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.yfazqb.com/Article/details/ghfgayjlg.sHtML

declare(strict_types=1);
来源：http://read.share.fktsv.cn/Article/details/gjwrxbvzi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.tarul.cn/Article/details/gkazwdqei.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gpiajhybh.sHtML

[U46] PHP：可空类型
来源：http://3g.yfazqb.com/Article/details/gzybvrcqh.sHtML

?string $name = null
来源：http://www.share.bbcook.cn/Article/details/gckhekoxd.sHtML

[U47] PHP：联合类型
来源：http://www.share.tarul.cn/Article/details/gwfjvrciq.sHtML

int|string $id
来源：http://m.share.bbcook.cn/Article/details/gavzudszv.sHtML

[U48] PHP：纯枚举
来源：http://read.share.bbcook.cn/Article/details/gjjsmjrte.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.bbcook.cn/Article/details/ggnnzbntf.sHtML

[U49] PHP：只读属性
来源：http://mobile.yfazqb.com/Article/details/gpbifmwml.sHtML

public readonly string $name
来源：http://read.share.tarul.cn/Article/details/ghegpjhks.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fktsv.cn/Article/details/glyitixst.sHtML

public function __construct(private int $id) {}
来源：http://www.share.bbcook.cn/Article/details/gusiqipxz.sHtML

[U51] PHP：数组解构
来源：http://mobile.tarul.cn/Article/details/gfoigjwcr.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.tarul.cn/Article/details/glrbgruzx.sHtML

[U52] PHP：箭头函数
来源：http://m.share.tarul.cn/Article/details/gdtkxixfk.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.vehdjk.com/Article/details/googbbwqr.sHtML

[U53] PHP：空合并运算符
来源：http://3g.sjlbkw.cn/Article/details/gkhrepjnh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.sjlbkw.cn/Article/details/gdgdfjvni.sHtML

[U54] PHP：空安全调用
来源：http://blog.sjlbkw.cn/Article/details/gynyjbcya.sHtML

$obj?->method()
来源：http://mobile.vehdjk.com/Article/details/ghffdpcna.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fktsv.cn/Article/details/gmvfrscie.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.yfazqb.com/Article/details/gjyaltznc.sHtML

[U56] PHP：命名参数
来源：http://mobile.fktsv.cn/Article/details/gabxpwxxb.sHtML

f(a: 1, b: 2)
来源：http://www.blog.vehdjk.com/Article/details/gkvvazgnh.sHtML

[U57] PHP：字符串插值
来源：http://www.share.tarul.cn/Article/details/gkagxblqe.sHtML

"值: {$a}"
来源：http://mobile.vehdjk.com/Article/details/giucwgjav.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fktsv.cn/Article/details/gdmepcqox.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.epnwcf.com/Article/details/gxcnyhalb.sHtML

[U59] PHP：自定义排序
来源：http://m.share.epnwcf.com/Article/details/gpdadntrq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.bbcook.cn/Article/details/gnfnztryf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.tarul.cn/Article/details/gkgbagytu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.sjlbkw.cn/Article/details/grlmfwmqo.sHtML

[U61] PHP：正则
来源：http://baike.sjlbkw.cn/Article/details/gaugeywkn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.yfazqb.com/Article/details/glejhisrx.sHtML

[U62] PHP：日期对象
来源：http://m.share.tarul.cn/Article/details/grfpudazu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.vehdjk.com/Article/details/gqdcdtblh.sHtML

[U63] PHP：文件读写
来源：http://m.share.sjlbkw.cn/Article/details/gnmgrzyju.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fktsv.cn/Article/details/grbeekvop.sHtML

[U64] PHP：目录遍历
来源：http://mobile.tarul.cn/Article/details/grztzpjyu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fktsv.cn/Article/details/ghlpsmrnu.sHtML

[U65] PHP：会话
来源：http://www.share.tarul.cn/Article/details/gowfmfmrw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fktsv.cn/Article/details/ggpatncqo.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.tarul.cn/Article/details/gsndtyvrm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.bbcook.cn/Article/details/gqdqvtemy.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fktsv.cn/Article/details/grjzuqjvk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.epnwcf.com/Article/details/gshdlpjsm.sHtML

[U68] PHP：PDO 连接
来源：http://wap.vehdjk.com/Article/details/gaivrxfnm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.tarul.cn/Article/details/guicynekl.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.tarul.cn/Article/details/gbebyasyw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.yfazqb.com/Article/details/gbkltaesf.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.epnwcf.com/Article/details/gxvwfulof.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.vehdjk.com/Article/details/gcobfhhjs.sHtML

[U71] PHP：抛出异常
来源：http://m.share.tarul.cn/Article/details/giwtfcgvp.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/gpqzjxxbf.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.yfazqb.com/Article/details/gnzanimvd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.sjlbkw.cn/Article/details/ggajvqxte.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.epnwcf.com/Article/details/gvzuxhsxg.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fktsv.cn/Article/details/gdmfpzkrp.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.epnwcf.com/Article/details/gujuhtvkn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.bbcook.cn/Article/details/gozcxwwnd.sHtML

[U75] PHP：依赖注入
来源：http://wap.yfazqb.com/Article/details/gawkspvoo.sHtML

composer require psr/container
来源：http://mobile.yfazqb.com/Article/details/guzjfghez.sHtML

[U76] PHP：简单路由
来源：http://read.share.vehdjk.com/Article/details/grfkvnekk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fktsv.cn/Article/details/gmgxbadwc.sHtML

[U77] PHP：模板渲染
来源：http://www.share.epnwcf.com/Article/details/gfkvrfhku.sHtML

composer require twig/twig
来源：http://www.blog.vehdjk.com/Article/details/gwfuachad.sHtML

[U78] PHP：单元测试
来源：http://www.share.yfazqb.com/Article/details/gdsaekfkl.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.sjlbkw.cn/Article/details/gtssyfupx.sHtML

[U79] PHP：静态分析
来源：http://wap.bbcook.cn/Article/details/gishpseuf.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.sjlbkw.cn/Article/details/gaefrhnvs.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.tarul.cn/Article/details/gcylkyxjd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.yfazqb.com/Article/details/gwteqjjnn.sHtML

[U81] JS：初始化项目
来源：http://blog.sjlbkw.cn/Article/details/gorokdrok.sHtML

npm init -y;  npm i express
来源：http://mobile.yfazqb.com/Article/details/gezhepcnx.sHtML

[U82] JS：package.json 脚本
来源：http://3g.yfazqb.com/Article/details/gsiopnjlr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.vehdjk.com/Article/details/guiopzoox.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fktsv.cn/Article/details/givavopib.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.yfazqb.com/Article/details/gfdclbxlf.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.vehdjk.com/Article/details/gxanbzckd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.yfazqb.com/Article/details/gtwfusbfa.sHtML

[U85] JS：可选链
来源：http://mobile.tarul.cn/Article/details/glbtlwoch.sHtML

a?.b?.c
来源：http://blog.sjlbkw.cn/Article/details/gshrfplpq.sHtML

[U86] JS：空值合并
来源：http://www.share.fktsv.cn/Article/details/gplnyodap.sHtML

a ?? b
来源：http://mobile.vehdjk.com/Article/details/gecpggsrm.sHtML

[U87] JS：解构默认值
来源：http://www.blog.bbcook.cn/Article/details/gigrjyfja.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.yfazqb.com/Article/details/gnyevbrar.sHtML

[U88] JS：对象展开合并
来源：http://wap.yfazqb.com/Article/details/gcaghxhcx.sHtML

{ ...a, ...b }
来源：http://www.m.share.tarul.cn/Article/details/gkxbcbkfh.sHtML

[U89] JS：数组去重
来源：http://3g.tarul.cn/Article/details/ghobcofyl.sHtML

[...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gnxfyetff.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fktsv.cn/Article/details/gbebltekz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gygddekeg.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.yfazqb.com/Article/details/gsiynrdvr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.vehdjk.com/Article/details/ghljdfszg.sHtML

[U92] JS：深拷贝
来源：http://www.share.bbcook.cn/Article/details/gtrsegdmn.sHtML

structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gzxsdxzwx.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.epnwcf.com/Article/details/geifdezrn.sHtML

`共 ${n} 条`
来源：http://www.share.tarul.cn/Article/details/gkwguyqnf.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.bbcook.cn/Article/details/glnlshjiq.sHtML

const double = x => x * 2;
来源：http://m.share.vehdjk.com/Article/details/gmnlnamfp.sHtML

[U95] JS：Promise 包装
来源：http://baike.vehdjk.com/Article/details/gmlcpdiep.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.vehdjk.com/Article/details/gvrucpurk.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.tarul.cn/Article/details/gkababqal.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/giuxxqfma.sHtML

[U97] JS：并发请求
来源：http://www.blog.vehdjk.com/Article/details/gipagyxav.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gxavjznsf.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.yfazqb.com/Article/details/gstefqjvm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.yfazqb.com/Article/details/ggwfwgoik.sHtML

[U99] JS：事件监听
来源：http://blog.tarul.cn/Article/details/gktuhmcsc.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.bbcook.cn/Article/details/gmglmxfpz.sHtML

[U100] JS：DOM 查询
来源：http://mobile.vehdjk.com/Article/details/ghxneueew.sHtML

document.querySelector(".item")
来源：http://www.share.vehdjk.com/Article/details/gpcvvowem.sHtML

[U101] JS：classList 操作
来源：http://www.blog.vehdjk.com/Article/details/gkxxfkccs.sHtML

el.classList.toggle("active")
来源：http://blog.vehdjk.com/Article/details/gjxsxzvby.sHtML

[U102] JS：本地存储
来源：http://m.share.bbcook.cn/Article/details/gczqqkhfs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.bbcook.cn/Article/details/guivuqwzh.sHtML

[U103] JS：定时器
来源：http://wap.tarul.cn/Article/details/gimgjuiet.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.tarul.cn/Article/details/gvxbpkcnf.sHtML

[U104] JS：防抖
来源：http://baike.fktsv.cn/Article/details/gquopwwyj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gpfixfnms.sHtML

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/gbznsknvx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fktsv.cn/Article/details/ghrgzwbth.sHtML

[U106] JS：日期格式化
来源：http://blog.bbcook.cn/Article/details/ggoswghyg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.bbcook.cn/Article/details/gwdjhaywc.sHtML

[U107] JS：数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gyxghcwah.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.bbcook.cn/Article/details/gzbajofea.sHtML

[U108] JS：随机整数
来源：http://blog.bbcook.cn/Article/details/gkgveulxh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.yfazqb.com/Article/details/gpzcqewce.sHtML

[U109] JS：数组分组
来源：http://3g.tarul.cn/Article/details/grkdgwhtm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/glhinutem.sHtML

[U110] JS：数组分块
来源：http://baike.epnwcf.com/Article/details/gbeetidxf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.yfazqb.com/Article/details/guealrkex.sHtML

[U111] JS：对象转 Map
来源：http://baike.yfazqb.com/Article/details/gsxqmcnjs.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fktsv.cn/Article/details/gmlnvynge.sHtML

[U112] JS：字符串补位
来源：http://blog.bbcook.cn/Article/details/gltqxmjxt.sHtML

"7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gkdarwokc.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fktsv.cn/Article/details/gfvrxeqwu.sHtML

s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gjagkpmph.sHtML

[U114] JS：JSON 深比较
来源：http://blog.yfazqb.com/Article/details/gspuagebc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gdhmaqids.sHtML

[U115] JS：生成 UUID
来源：http://3g.vehdjk.com/Article/details/gwuauasqf.sHtML

crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gnfqtbgii.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.bbcook.cn/Article/details/gpgxryqgf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.epnwcf.com/Article/details/gtrwzoctl.sHtML

[U117] JS：单元测试
来源：http://3g.fktsv.cn/Article/details/gymmxamyr.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.yfazqb.com/Article/details/gcyvbersm.sHtML

[U118] JS：开发服务器
来源：http://wap.epnwcf.com/Article/details/gzuhwunci.sHtML

npm i -D vite;  npx vite
来源：http://wap.epnwcf.com/Article/details/grhjsrfcc.sHtML

[U119] JS：生产构建
来源：http://www.share.fktsv.cn/Article/details/gcsryurut.sHtML

npx vite build
来源：http://www.share.fktsv.cn/Article/details/gxvrkivmv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.tarul.cn/Article/details/gzyfkuzym.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.sjlbkw.cn/Article/details/gsninrvzs.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gnlpfjphl.sHtML

统计汇总
来源：http://baike.sjlbkw.cn/Article/details/gtrvgebbn.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/givigygoi.sHtML

按语言统计（条）：
来源：http://www.m.share.sjlbkw.cn/Article/details/gcchwvtyi.sHtML

Python ......... 252
来源：http://www.share.yfazqb.com/Article/details/gmsktudvz.sHtML

PHP ............ 252
来源：http://blog.yfazqb.com/Article/details/gogaqquou.sHtML

JavaScript ..... 252
来源：http://www.share.bbcook.cn/Article/details/gmdpryztu.sHtML

TypeScript ..... 212
来源：http://wap.sjlbkw.cn/Article/details/gdqtkdski.sHtML

Java ........... 212
来源：http://wap.epnwcf.com/Article/details/gbzjxsfyw.sHtML

Go ............. 212
来源：http://www.blog.sjlbkw.cn/Article/details/gimlrpums.sHtML

Ruby ........... 212
来源：http://www.blog.bbcook.cn/Article/details/gcgytgclm.sHtML

C# ............. 212
来源：http://m.share.fktsv.cn/Article/details/gefkgwbrc.sHtML

C .............. 30
来源：http://3g.tarul.cn/Article/details/gzllfkhjw.sHtML

C++ ............ 30
来源：http://m.share.fktsv.cn/Article/details/gctkhmbjy.sHtML

SQL ............ 90
来源：http://baike.tarul.cn/Article/details/ggybchqpl.sHtML

Bash ........... 80
来源：http://3g.bbcook.cn/Article/details/gbuldsauy.sHtML

Kotlin ......... 15
来源：http://read.share.epnwcf.com/Article/details/gyszxkrqf.sHtML

Swift .......... 15
来源：http://blog.tarul.cn/Article/details/gvlwixiym.sHtML

Lua ............ 10
来源：http://www.share.epnwcf.com/Article/details/gqbgzxjya.sHtML

Perl ........... 10
来源：http://read.share.vehdjk.com/Article/details/gjhfjrzun.sHtML

Scala .......... 10
来源：http://mobile.yfazqb.com/Article/details/ggnvsdyfe.sHtML

------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gvvfketnc.sHtML

合计 ........... 2106 条
来源：http://www.m.share.epnwcf.com/Article/details/ggjyweajf.sHtML

按章节统计：
来源：http://read.share.fktsv.cn/Article/details/guqybrllc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.vehdjk.com/Article/details/gxgtegrzl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gldlippot.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/ganoiwewv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/gbeiftbgc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.epnwcf.com/Article/details/glvdkympt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.bbcook.cn/Article/details/gcdfgiymp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/gqtfrhaxp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.epnwcf.com/Article/details/gjndbjncw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gcxuoeopy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.sjlbkw.cn/Article/details/gqoyqyljv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/ggqofsmmp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/ghdgfcccq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gxjdkcwno.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.tarul.cn/Article/details/gpmnqxbaz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.sjlbkw.cn/Article/details/ggpvsirnm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gqalehvvk.sHtML

Q SQL 专题                              90
来源：http://wap.vehdjk.com/Article/details/gwsjskmts.sHtML

R Bash 专题                             80
来源：http://blog.tarul.cn/Article/details/gamilpxjq.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.bbcook.cn/Article/details/gaerelwmt.sHtML

T 其他语言补充                          60
来源：http://www.share.tarul.cn/Article/details/gmrburvzr.sHtML

U 高频实用片段                         120
来源：http://www.share.tarul.cn/Article/details/gyofhxeiz.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/geoekczgp.sHtML

合计                                  2106 条
来源：http://3g.fktsv.cn/Article/details/gywjvieav.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gzanxchav.sHtML

使用提醒
来源：http://baike.tarul.cn/Article/details/glbguouwu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gmbkxqucz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.bbcook.cn/Article/details/gdudfgjig.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.epnwcf.com/Article/details/gieazobge.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.bbcook.cn/Article/details/gbkqsanvc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.vehdjk.com/Article/details/gbbrytwws.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fktsv.cn/Article/details/ghmibhrdx.sHtML

—— 文件结束 ——
来源：http://mobile.bbcook.cn/Article/details/goslyzilb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/guvaqccyl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.yfazqb.com/Article/details/glishybqe.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.bbcook.cn/Article/details/gpxihdcjq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gioevyial.sHtML

【收录内容】
来源：http://m.share.epnwcf.com/Article/details/gzlehvmrt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.sjlbkw.cn/Article/details/gpyowjxeh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.sjlbkw.cn/Article/details/gcwmggfub.sHtML

SQL · Bash · C · C++
来源：http://www.blog.tarul.cn/Article/details/gevjmtspd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.vehdjk.com/Article/details/gyjhyvyiu.sHtML

【使用说明】
来源：http://www.share.yfazqb.com/Article/details/gsgekakyv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.tarul.cn/Article/details/gvufxqibf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.sjlbkw.cn/Article/details/goqixkgkz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.vehdjk.com/Article/details/gegiwgrtk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.bbcook.cn/Article/details/gfgkjhznx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.yfazqb.com/Article/details/gayivqxnl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.sjlbkw.cn/Article/details/gbkapiock.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.vehdjk.com/Article/details/gwapvjdzd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.vehdjk.com/Article/details/gwzogufhg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.vehdjk.com/Article/details/gnvpdhfze.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.sjlbkw.cn/Article/details/gaodfqixu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.sjlbkw.cn/Article/details/gwvzvwzoh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.vehdjk.com/Article/details/glurjxyur.sHtML

【文件统计】
来源：http://www.share.sjlbkw.cn/Article/details/gbukbazmb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsjfduia.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/gsyxivxik.sHtML

目  录
来源：http://baike.tarul.cn/Article/details/gokglfnga.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gilatfftq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fktsv.cn/Article/details/gsfsxkpnh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/gzagcilsi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fktsv.cn/Article/details/gefohjawq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.bbcook.cn/Article/details/gwuvepqex.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.sjlbkw.cn/Article/details/gjfwwrvcd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.epnwcf.com/Article/details/gqyumwftw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.vehdjk.com/Article/details/ggvfxrrba.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.epnwcf.com/Article/details/gxycukrsi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gbkuyagil.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.vehdjk.com/Article/details/gdfmgclti.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.yfazqb.com/Article/details/gcaypddbw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gapqnogoa.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gwoisavju.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.epnwcf.com/Article/details/gueesqrhq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.yfazqb.com/Article/details/guqlptkzi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.yfazqb.com/Article/details/gvcdmcgqx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.vehdjk.com/Article/details/gxjsvbejz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.epnwcf.com/Article/details/gnekkxehq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fktsv.cn/Article/details/ghgruxqef.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gjwxxdoto.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/gdegsemog.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gifgsmtkj.sHtML

A. 基础语法与类型
来源：http://baike.bbcook.cn/Article/details/glcmtsukp.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/garhkkgbp.sHtML

[A01] Hello World
来源：http://read.share.fktsv.cn/Article/details/gkpyeailz.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.bbcook.cn/Article/details/gtrmvfulu.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.sjlbkw.cn/Article/details/ghemhngkk.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.bbcook.cn/Article/details/gkelymxog.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.vehdjk.com/Article/details/gydhwdkvo.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/gjpmjjmgd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.bbcook.cn/Article/details/gnenbhgvf.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.epnwcf.com/Article/details/ghcgwksnh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/gxlcnewks.sHtML

[A02] 变量声明与赋值
来源：http://read.share.vehdjk.com/Article/details/gcwvuwuho.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.bbcook.cn/Article/details/gvrvwqxcd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.sjlbkw.cn/Article/details/gnzgzmgvn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.vehdjk.com/Article/details/gxyfocrto.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.vehdjk.com/Article/details/grbkomjnc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.tarul.cn/Article/details/gdniucfps.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.yfazqb.com/Article/details/gwwqhtpsy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.epnwcf.com/Article/details/gclcvmmao.sHtML


<!-- 参考信息 -->