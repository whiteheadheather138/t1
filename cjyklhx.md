代发 wailian999

[U33] Py：打包发布
来源：http://mobile.vehdjk.com/Article/details/gkfnpodxf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.vehdjk.com/Article/details/gwejrgsji.sHtML

[U34] Py：判断编码
来源：http://wap.tarul.cn/Article/details/ghdzwkqzt.sHtML

chardet.detect(raw)
来源：http://3g.vehdjk.com/Article/details/govgetkel.sHtML

[U35] Py：发送邮件
来源：http://www.blog.bbcook.cn/Article/details/glkaahyaw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.bbcook.cn/Article/details/guyfvziat.sHtML

[U36] Py：定时任务
来源：http://www.share.yfazqb.com/Article/details/gjpikgeyz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.sjlbkw.cn/Article/details/grkkpknlu.sHtML

[U37] Py：读写 Excel
来源：http://3g.bbcook.cn/Article/details/gxijzjrut.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.yfazqb.com/Article/details/ghjbxpsww.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.yfazqb.com/Article/details/gcqixqbrq.sHtML

Path(__file__).resolve().parent
来源：http://read.share.epnwcf.com/Article/details/gjjmyzpbf.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.yfazqb.com/Article/details/gqpjhwlii.sHtML

sys.stdout.isatty()
来源：http://www.blog.vehdjk.com/Article/details/gailjwtyr.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.sjlbkw.cn/Article/details/gnrfxyxqm.sHtML

print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gxgugtkun.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.tarul.cn/Article/details/gzxymuipt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.epnwcf.com/Article/details/gsqxvosjs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.sjlbkw.cn/Article/details/glnbnziig.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.epnwcf.com/Article/details/gvjvxnpeb.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.vehdjk.com/Article/details/gjeyvtocl.sHtML

namespace App\Http;
来源：http://www.m.share.epnwcf.com/Article/details/gobnpwaeq.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fktsv.cn/Article/details/gdkvqcdzz.sHtML

declare(strict_types=1);
来源：http://m.share.epnwcf.com/Article/details/gicislszx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.epnwcf.com/Article/details/gokemstyw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gxjbacuhn.sHtML

[U46] PHP：可空类型
来源：http://www.blog.yfazqb.com/Article/details/gaxijgcdu.sHtML

?string $name = null
来源：http://www.blog.epnwcf.com/Article/details/gdedmgfew.sHtML

[U47] PHP：联合类型
来源：http://baike.vehdjk.com/Article/details/gmezmlpfw.sHtML

int|string $id
来源：http://baike.fktsv.cn/Article/details/gnxktqvtn.sHtML

[U48] PHP：纯枚举
来源：http://blog.sjlbkw.cn/Article/details/gxovtzwnf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.sjlbkw.cn/Article/details/gydzrdqwu.sHtML

[U49] PHP：只读属性
来源：http://3g.yfazqb.com/Article/details/gwbenjzmx.sHtML

public readonly string $name
来源：http://www.blog.yfazqb.com/Article/details/ggeolfnvs.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.epnwcf.com/Article/details/gzzsulqhb.sHtML

public function __construct(private int $id) {}
来源：http://read.share.sjlbkw.cn/Article/details/gihwtlods.sHtML

[U51] PHP：数组解构
来源：http://wap.fktsv.cn/Article/details/giewoxmcm.sHtML

[$a, $b] = $arr;
来源：http://3g.tarul.cn/Article/details/gicfabztl.sHtML

[U52] PHP：箭头函数
来源：http://3g.tarul.cn/Article/details/gociirenh.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.vehdjk.com/Article/details/gutonqybh.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.bbcook.cn/Article/details/gdwthflpj.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.sjlbkw.cn/Article/details/gmpyvynkb.sHtML

[U54] PHP：空安全调用
来源：http://baike.vehdjk.com/Article/details/ggahvljxr.sHtML

$obj?->method()
来源：http://baike.yfazqb.com/Article/details/gbrvtkhfp.sHtML

[U55] PHP：match 表达式
来源：http://3g.tarul.cn/Article/details/gxjqwcemv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/goionwhie.sHtML

[U56] PHP：命名参数
来源：http://baike.tarul.cn/Article/details/gqdskxvbp.sHtML

f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/goxppaldz.sHtML

[U57] PHP：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gulwssuuo.sHtML

"值: {$a}"
来源：http://blog.yfazqb.com/Article/details/gedmkhrqz.sHtML

[U58] PHP：数组三件套
来源：http://blog.fktsv.cn/Article/details/glibazddg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fktsv.cn/Article/details/geynawihl.sHtML

[U59] PHP：自定义排序
来源：http://read.share.sjlbkw.cn/Article/details/gwpzbxppy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gsrqqagzx.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fktsv.cn/Article/details/gotmauxbu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.yfazqb.com/Article/details/gtqbrhsxj.sHtML

[U61] PHP：正则
来源：http://3g.tarul.cn/Article/details/glppoacio.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.bbcook.cn/Article/details/ggdsinynt.sHtML

[U62] PHP：日期对象
来源：http://3g.sjlbkw.cn/Article/details/gdrrqptfb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.yfazqb.com/Article/details/gbmzaitbo.sHtML

[U63] PHP：文件读写
来源：http://3g.epnwcf.com/Article/details/gewjqtizp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.bbcook.cn/Article/details/gpunueikv.sHtML

[U64] PHP：目录遍历
来源：http://read.share.sjlbkw.cn/Article/details/gedvajgid.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.bbcook.cn/Article/details/gdqembxjt.sHtML

[U65] PHP：会话
来源：http://wap.yfazqb.com/Article/details/grsrwbter.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gmobqtakx.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.vehdjk.com/Article/details/gqylwzhiv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.sjlbkw.cn/Article/details/gwdzxdcrw.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.bbcook.cn/Article/details/gkqugtrro.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fktsv.cn/Article/details/gtywfsjxd.sHtML

[U68] PHP：PDO 连接
来源：http://blog.vehdjk.com/Article/details/gtvcxqaxi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.epnwcf.com/Article/details/gwiqwvtby.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.epnwcf.com/Article/details/gikqkfqdz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.sjlbkw.cn/Article/details/gdqnblolb.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.tarul.cn/Article/details/gbiuupdaf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.tarul.cn/Article/details/gcyltaoav.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.vehdjk.com/Article/details/geknejgui.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.bbcook.cn/Article/details/grkgaetnf.sHtML

[U72] PHP：写错误日志
来源：http://read.share.tarul.cn/Article/details/gzaqkrejf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.epnwcf.com/Article/details/gaodyvzig.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fktsv.cn/Article/details/gkqytxaeo.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.vehdjk.com/Article/details/gwybzatzp.sHtML

[U74] PHP：读取环境变量
来源：http://blog.bbcook.cn/Article/details/gcosvsmgw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fktsv.cn/Article/details/gafnllcix.sHtML

[U75] PHP：依赖注入
来源：http://wap.vehdjk.com/Article/details/gepdblhhp.sHtML

composer require psr/container
来源：http://www.share.bbcook.cn/Article/details/githneffv.sHtML

[U76] PHP：简单路由
来源：http://3g.sjlbkw.cn/Article/details/gxpbbyhvn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fktsv.cn/Article/details/gmhvhgxzh.sHtML

[U77] PHP：模板渲染
来源：http://baike.sjlbkw.cn/Article/details/ghmbzvyxs.sHtML

composer require twig/twig
来源：http://baike.sjlbkw.cn/Article/details/gdbpqtfic.sHtML

[U78] PHP：单元测试
来源：http://mobile.tarul.cn/Article/details/gvjygbuvt.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.yfazqb.com/Article/details/gafxffubn.sHtML

[U79] PHP：静态分析
来源：http://mobile.yfazqb.com/Article/details/gnzmorjmz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.vehdjk.com/Article/details/gqdkbjnak.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.vehdjk.com/Article/details/gfwdipdzo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.bbcook.cn/Article/details/govuirssz.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.bbcook.cn/Article/details/gelglsysy.sHtML

npm init -y;  npm i express
来源：http://wap.fktsv.cn/Article/details/gkcsmcpaf.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.sjlbkw.cn/Article/details/ggqighwtv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.bbcook.cn/Article/details/gksprcvco.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.yfazqb.com/Article/details/gcgzcvpur.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.vehdjk.com/Article/details/gmkblvlyk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.sjlbkw.cn/Article/details/gfebwltzs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.yfazqb.com/Article/details/gzyackudn.sHtML

[U85] JS：可选链
来源：http://read.share.tarul.cn/Article/details/gsekkvnvz.sHtML

a?.b?.c
来源：http://baike.sjlbkw.cn/Article/details/grxwbtkvc.sHtML

[U86] JS：空值合并
来源：http://www.blog.sjlbkw.cn/Article/details/gdqjyxfur.sHtML

a ?? b
来源：http://blog.bbcook.cn/Article/details/gqmpvyvtz.sHtML

[U87] JS：解构默认值
来源：http://m.share.tarul.cn/Article/details/ghwmebeim.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.yfazqb.com/Article/details/gfovkohrj.sHtML

[U88] JS：对象展开合并
来源：http://m.share.epnwcf.com/Article/details/gvpjmzdfe.sHtML

{ ...a, ...b }
来源：http://mobile.epnwcf.com/Article/details/gasamqdti.sHtML

[U89] JS：数组去重
来源：http://baike.fktsv.cn/Article/details/gbizhptnq.sHtML

[...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gqsohanqi.sHtML

[U90] JS：数字数组排序
来源：http://mobile.tarul.cn/Article/details/gebyvlrml.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/goubgqvmz.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fktsv.cn/Article/details/ggjuvtjgh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.sjlbkw.cn/Article/details/gqjwwvdge.sHtML

[U92] JS：深拷贝
来源：http://blog.fktsv.cn/Article/details/gpoxipcyx.sHtML

structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/grjbphqil.sHtML

[U93] JS：模板字符串
来源：http://wap.sjlbkw.cn/Article/details/gmsgassej.sHtML

`共 ${n} 条`
来源：http://blog.fktsv.cn/Article/details/gvcykpejo.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/gjnpvznja.sHtML

const double = x => x * 2;
来源：http://3g.tarul.cn/Article/details/gtwnqjpts.sHtML

[U95] JS：Promise 包装
来源：http://read.share.sjlbkw.cn/Article/details/gdeteqlqu.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.bbcook.cn/Article/details/gnllihpah.sHtML

[U96] JS：async/await 与异常
来源：http://wap.sjlbkw.cn/Article/details/gddehpesl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gmcsgyzak.sHtML

[U97] JS：并发请求
来源：http://wap.vehdjk.com/Article/details/ggozqlxqa.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/graistmdg.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/glcgxiejh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fktsv.cn/Article/details/gfnzzgvap.sHtML

[U99] JS：事件监听
来源：http://read.share.tarul.cn/Article/details/ghfikhtzg.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.sjlbkw.cn/Article/details/gmxwaiedd.sHtML

[U100] JS：DOM 查询
来源：http://blog.vehdjk.com/Article/details/gftadzmwr.sHtML

document.querySelector(".item")
来源：http://baike.sjlbkw.cn/Article/details/gqnqmnrpt.sHtML

[U101] JS：classList 操作
来源：http://m.share.yfazqb.com/Article/details/grfmyanly.sHtML

el.classList.toggle("active")
来源：http://read.share.yfazqb.com/Article/details/gihfuslxo.sHtML

[U102] JS：本地存储
来源：http://blog.tarul.cn/Article/details/gpnbyczdd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.epnwcf.com/Article/details/gtuvwhdli.sHtML

[U103] JS：定时器
来源：http://3g.bbcook.cn/Article/details/geakkivmx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fktsv.cn/Article/details/gujlhdlrq.sHtML

[U104] JS：防抖
来源：http://www.share.epnwcf.com/Article/details/gvgfywzdz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gnytjlpxi.sHtML

[U105] JS：节流
来源：http://mobile.tarul.cn/Article/details/gbodkgcgc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.sjlbkw.cn/Article/details/gvzssclhp.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.tarul.cn/Article/details/ggeorlefs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fktsv.cn/Article/details/gkygcbuwz.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/goxumkwdx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gmrkpcick.sHtML

[U108] JS：随机整数
来源：http://m.share.bbcook.cn/Article/details/gtwstmote.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.bbcook.cn/Article/details/gezoedhos.sHtML

[U109] JS：数组分组
来源：http://baike.sjlbkw.cn/Article/details/gkmcnoteb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.yfazqb.com/Article/details/gshitozfo.sHtML

[U110] JS：数组分块
来源：http://baike.yfazqb.com/Article/details/gbouckbkw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.vehdjk.com/Article/details/grurqaeqx.sHtML

[U111] JS：对象转 Map
来源：http://read.share.tarul.cn/Article/details/gvtfpjebn.sHtML

new Map(Object.entries(obj))
来源：http://baike.tarul.cn/Article/details/gubkztgsu.sHtML

[U112] JS：字符串补位
来源：http://blog.tarul.cn/Article/details/gwtyrlifs.sHtML

"7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/goqqpiiix.sHtML

[U113] JS：正则替换全部
来源：http://blog.vehdjk.com/Article/details/gteobgxuo.sHtML

s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gjkliksyl.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.yfazqb.com/Article/details/gplzihsau.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/ghdexyssq.sHtML

[U115] JS：生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gpihjcsyu.sHtML

crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/geqauflfn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.epnwcf.com/Article/details/gzeyaoohb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.yfazqb.com/Article/details/grurwohza.sHtML

[U117] JS：单元测试
来源：http://blog.bbcook.cn/Article/details/grvdxtzpj.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.tarul.cn/Article/details/gmoxmtpdp.sHtML

[U118] JS：开发服务器
来源：http://www.blog.tarul.cn/Article/details/gmypujbrg.sHtML

npm i -D vite;  npx vite
来源：http://mobile.bbcook.cn/Article/details/ghggivnrh.sHtML

[U119] JS：生产构建
来源：http://blog.vehdjk.com/Article/details/gigrfxjoi.sHtML

npx vite build
来源：http://www.m.share.vehdjk.com/Article/details/glzodyymt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.bbcook.cn/Article/details/gwxoxdtos.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fktsv.cn/Article/details/ghhqdlrix.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gghswrmuy.sHtML

统计汇总
来源：http://www.share.fktsv.cn/Article/details/gmawifbjb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpszugoke.sHtML

按语言统计（条）：
来源：http://read.share.epnwcf.com/Article/details/gpabzeyzz.sHtML

Python ......... 252
来源：http://blog.fktsv.cn/Article/details/gfcijfchr.sHtML

PHP ............ 252
来源：http://m.share.epnwcf.com/Article/details/gvlluqnsz.sHtML

JavaScript ..... 252
来源：http://mobile.tarul.cn/Article/details/ggkkjavxd.sHtML

TypeScript ..... 212
来源：http://read.share.epnwcf.com/Article/details/ghpriznad.sHtML

Java ........... 212
来源：http://3g.bbcook.cn/Article/details/ggvtlgmyp.sHtML

Go ............. 212
来源：http://www.m.share.bbcook.cn/Article/details/gvcrtnase.sHtML

Ruby ........... 212
来源：http://3g.tarul.cn/Article/details/glfxyiffa.sHtML

C# ............. 212
来源：http://www.share.epnwcf.com/Article/details/ghfmxjjic.sHtML

C .............. 30
来源：http://wap.yfazqb.com/Article/details/geztdxrjw.sHtML

C++ ............ 30
来源：http://baike.epnwcf.com/Article/details/ggfmapayw.sHtML

SQL ............ 90
来源：http://blog.sjlbkw.cn/Article/details/gerexscbv.sHtML

Bash ........... 80
来源：http://mobile.sjlbkw.cn/Article/details/gkavpswec.sHtML

Kotlin ......... 15
来源：http://www.share.epnwcf.com/Article/details/ganccupbv.sHtML

Swift .......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/gmgynrakh.sHtML

Lua ............ 10
来源：http://m.share.vehdjk.com/Article/details/gbahvbjae.sHtML

Perl ........... 10
来源：http://www.share.vehdjk.com/Article/details/gqrriyzst.sHtML

Scala .......... 10
来源：http://3g.tarul.cn/Article/details/gvxlpugws.sHtML

------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gnvyehphk.sHtML

合计 ........... 2106 条
来源：http://3g.tarul.cn/Article/details/gvnkuqgjo.sHtML

按章节统计：
来源：http://www.blog.sjlbkw.cn/Article/details/ghwfdthoc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/guztxozai.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.sjlbkw.cn/Article/details/gjpytzqme.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/genmbskdl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.sjlbkw.cn/Article/details/gjzjkcjrg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.yfazqb.com/Article/details/ggmitdrgm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.tarul.cn/Article/details/gravbthcx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/ghdcixwom.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.sjlbkw.cn/Article/details/gnfywpdpu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gkrqyioet.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.bbcook.cn/Article/details/gicxzshss.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gelsfoxel.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gplepkeol.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.bbcook.cn/Article/details/giwostxfz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.yfazqb.com/Article/details/gbeuherpt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.bbcook.cn/Article/details/gawcipsns.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gacststbs.sHtML

Q SQL 专题                              90
来源：http://www.m.share.tarul.cn/Article/details/gzhiabiuu.sHtML

R Bash 专题                             80
来源：http://m.share.vehdjk.com/Article/details/grffszunl.sHtML

S C / C++ 专题                          60
来源：http://read.share.vehdjk.com/Article/details/gukxbllzv.sHtML

T 其他语言补充                          60
来源：http://www.share.bbcook.cn/Article/details/gahxogtqq.sHtML

U 高频实用片段                         120
来源：http://wap.epnwcf.com/Article/details/gnkviovfg.sHtML

------------------------------------
来源：http://wap.fktsv.cn/Article/details/gbstovatl.sHtML

合计                                  2106 条
来源：http://read.share.fktsv.cn/Article/details/gmnitfhtl.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/glkqymblt.sHtML

使用提醒
来源：http://blog.tarul.cn/Article/details/gxmfxfbjq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gzosrwbdn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.tarul.cn/Article/details/gseswmakh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.sjlbkw.cn/Article/details/gvvxugzsi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.tarul.cn/Article/details/gpbxxdhld.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fktsv.cn/Article/details/gnstbknaw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.vehdjk.com/Article/details/gqlkkqmbj.sHtML

—— 文件结束 ——
来源：http://read.share.fktsv.cn/Article/details/glzjnsvmi.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gzyhqrbsn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.yfazqb.com/Article/details/gmnthzrph.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.sjlbkw.cn/Article/details/gofjcplje.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfkipwmki.sHtML

【收录内容】
来源：http://wap.vehdjk.com/Article/details/glwlqnpku.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.yfazqb.com/Article/details/gpdijclub.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.yfazqb.com/Article/details/gwxbuwacs.sHtML

SQL · Bash · C · C++
来源：http://read.share.sjlbkw.cn/Article/details/gqkdvmzbx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.epnwcf.com/Article/details/gcsqxcrfn.sHtML

【使用说明】
来源：http://mobile.tarul.cn/Article/details/grxucjbcm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.bbcook.cn/Article/details/gwoaiixil.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.tarul.cn/Article/details/gyqayhmxa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.epnwcf.com/Article/details/gzpaofkyt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.sjlbkw.cn/Article/details/gkrimqxdd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fktsv.cn/Article/details/gbvybwnkt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.bbcook.cn/Article/details/gbrzhejeo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.vehdjk.com/Article/details/gwscgifjw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.tarul.cn/Article/details/ggjqzhyrq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtyvldlp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.epnwcf.com/Article/details/gahkfhlww.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.sjlbkw.cn/Article/details/gqtosoykp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.vehdjk.com/Article/details/gjnmqtprc.sHtML

【文件统计】
来源：http://blog.sjlbkw.cn/Article/details/gmqduuavz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.sjlbkw.cn/Article/details/gejkcwoii.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gyatbwtth.sHtML

目  录
来源：http://read.share.epnwcf.com/Article/details/gxmhwgpwj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gcmtsxwzs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.tarul.cn/Article/details/gkphikztb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.epnwcf.com/Article/details/gakyywgsb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gskvrzima.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gstjtjtau.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.sjlbkw.cn/Article/details/gtrqzvgjd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.yfazqb.com/Article/details/giabrezjn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.epnwcf.com/Article/details/gnwunxdpv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.bbcook.cn/Article/details/goufugqnz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gyydlceik.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fktsv.cn/Article/details/gxzffbnti.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/gksguhcst.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gddvgcklm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gyucxajzd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.sjlbkw.cn/Article/details/ggqszfreh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.epnwcf.com/Article/details/gyoqcbmgi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.epnwcf.com/Article/details/gjkluanau.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.sjlbkw.cn/Article/details/gzcjxrpgt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.tarul.cn/Article/details/gmkyydjwi.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.sjlbkw.cn/Article/details/gdkywdmdg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.bbcook.cn/Article/details/gmsqucaqk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fktsv.cn/Article/details/gnfykllev.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gggbcmxqo.sHtML

A. 基础语法与类型
来源：http://mobile.bbcook.cn/Article/details/glkmcsvnr.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ganpaweaz.sHtML

[A01] Hello World
来源：http://blog.sjlbkw.cn/Article/details/glrrzbacb.sHtML

Py:   print("Hello, World!")
来源：http://www.share.tarul.cn/Article/details/ggqprntch.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.epnwcf.com/Article/details/gmimppjpi.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/gqrnjpbrc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.vehdjk.com/Article/details/gstdypjfn.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.yfazqb.com/Article/details/gmvnpscus.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.bbcook.cn/Article/details/gqoknvhef.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fktsv.cn/Article/details/gyrrnbvbc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.vehdjk.com/Article/details/gmweexkfb.sHtML

[A02] 变量声明与赋值
来源：http://mobile.sjlbkw.cn/Article/details/gmqgisiys.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.vehdjk.com/Article/details/gujfywcsc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.epnwcf.com/Article/details/gyorxalor.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gjmijleqn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.bbcook.cn/Article/details/gwbxajccg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.yfazqb.com/Article/details/gepvcrimr.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fktsv.cn/Article/details/gmummvalt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fktsv.cn/Article/details/gmgssiiic.sHtML


<!-- 参考信息 -->