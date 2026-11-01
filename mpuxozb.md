代发 wailian999

[U35] Py：发送邮件
来源：http://www.share.bbcook.cn/Article/details/gmsmcsmhq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.bbcook.cn/Article/details/gpqesdibn.sHtML

[U36] Py：定时任务
来源：http://read.share.tarul.cn/Article/details/grlkwjure.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.sjlbkw.cn/Article/details/gpkghxixv.sHtML

[U37] Py：读写 Excel
来源：http://wap.fktsv.cn/Article/details/gkuybgqsh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fktsv.cn/Article/details/grkclurni.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.epnwcf.com/Article/details/gfxgarrsy.sHtML

Path(__file__).resolve().parent
来源：http://3g.epnwcf.com/Article/details/gysfycptg.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.vehdjk.com/Article/details/gveykeoga.sHtML

sys.stdout.isatty()
来源：http://www.m.share.epnwcf.com/Article/details/gxelzaqip.sHtML

[U40] Py：打印到标准错误
来源：http://blog.vehdjk.com/Article/details/gjcoftykf.sHtML

print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/gwhsxlpjg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.yfazqb.com/Article/details/gawnbapty.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.epnwcf.com/Article/details/gnwutejet.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.epnwcf.com/Article/details/gvxftctwk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.epnwcf.com/Article/details/gjtekcjkv.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.yfazqb.com/Article/details/giwonckal.sHtML

namespace App\Http;
来源：http://wap.tarul.cn/Article/details/gfgiudaft.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fktsv.cn/Article/details/gxkyvlqkm.sHtML

declare(strict_types=1);
来源：http://www.share.vehdjk.com/Article/details/gzmsppbum.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.sjlbkw.cn/Article/details/gmdicfijj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/grlgbygur.sHtML

[U46] PHP：可空类型
来源：http://baike.epnwcf.com/Article/details/gtrpuplbu.sHtML

?string $name = null
来源：http://wap.yfazqb.com/Article/details/gnrlhwswm.sHtML

[U47] PHP：联合类型
来源：http://read.share.tarul.cn/Article/details/gjypgkqqv.sHtML

int|string $id
来源：http://m.share.yfazqb.com/Article/details/gkvfolqdb.sHtML

[U48] PHP：纯枚举
来源：http://wap.yfazqb.com/Article/details/gnavocxgw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.epnwcf.com/Article/details/gjjsryjnf.sHtML

[U49] PHP：只读属性
来源：http://www.share.epnwcf.com/Article/details/gusxvpxff.sHtML

public readonly string $name
来源：http://baike.yfazqb.com/Article/details/ggsidsgbu.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fktsv.cn/Article/details/gowevtohc.sHtML

public function __construct(private int $id) {}
来源：http://3g.tarul.cn/Article/details/getnyatfj.sHtML

[U51] PHP：数组解构
来源：http://baike.sjlbkw.cn/Article/details/ghrwnnius.sHtML

[$a, $b] = $arr;
来源：http://www.share.sjlbkw.cn/Article/details/gvxqegxqe.sHtML

[U52] PHP：箭头函数
来源：http://www.share.vehdjk.com/Article/details/gfgxcyauz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.tarul.cn/Article/details/gjakptwxg.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.bbcook.cn/Article/details/gzoqyvoih.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.sjlbkw.cn/Article/details/gthmmunhp.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.sjlbkw.cn/Article/details/gqhaneonh.sHtML

$obj?->method()
来源：http://read.share.yfazqb.com/Article/details/gekgpxcze.sHtML

[U55] PHP：match 表达式
来源：http://wap.vehdjk.com/Article/details/gjjsefadu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.vehdjk.com/Article/details/gjmovcrfv.sHtML

[U56] PHP：命名参数
来源：http://wap.sjlbkw.cn/Article/details/garqyqouq.sHtML

f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gkvufdxwg.sHtML

[U57] PHP：字符串插值
来源：http://blog.tarul.cn/Article/details/gzlvjgxwg.sHtML

"值: {$a}"
来源：http://wap.epnwcf.com/Article/details/gmhyzhuad.sHtML

[U58] PHP：数组三件套
来源：http://www.share.tarul.cn/Article/details/gbkqsawxh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gnbltduwi.sHtML

[U59] PHP：自定义排序
来源：http://blog.vehdjk.com/Article/details/gvnqiibtj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.epnwcf.com/Article/details/gnmlbcdhd.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.bbcook.cn/Article/details/gvddnvehu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.yfazqb.com/Article/details/gtexidstg.sHtML

[U61] PHP：正则
来源：http://blog.sjlbkw.cn/Article/details/gqqjykcsj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.yfazqb.com/Article/details/gyrxvjczd.sHtML

[U62] PHP：日期对象
来源：http://wap.epnwcf.com/Article/details/gizhpambz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fktsv.cn/Article/details/gmynvjqcq.sHtML

[U63] PHP：文件读写
来源：http://baike.tarul.cn/Article/details/gzjrpflvj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.tarul.cn/Article/details/gzgaqgzmx.sHtML

[U64] PHP：目录遍历
来源：http://3g.vehdjk.com/Article/details/gbbqidudb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.yfazqb.com/Article/details/gmjfkycnl.sHtML

[U65] PHP：会话
来源：http://www.blog.yfazqb.com/Article/details/glqtqykdv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gxhxpqkld.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fktsv.cn/Article/details/gvwbfokjw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.bbcook.cn/Article/details/gakhzbugb.sHtML

[U67] PHP：处理文件上传
来源：http://blog.vehdjk.com/Article/details/grrvfzcuy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.tarul.cn/Article/details/gbyobwpod.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fktsv.cn/Article/details/glpvsifjo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.sjlbkw.cn/Article/details/gichcvxex.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.yfazqb.com/Article/details/gopbtnxbh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.tarul.cn/Article/details/godzricfl.sHtML

[U70] PHP：PDO 事务
来源：http://blog.vehdjk.com/Article/details/gjrzwhvfo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.tarul.cn/Article/details/gemlmsknu.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.yfazqb.com/Article/details/gzabascnx.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.vehdjk.com/Article/details/gelfhcdic.sHtML

[U72] PHP：写错误日志
来源：http://baike.bbcook.cn/Article/details/gquuzoaek.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.tarul.cn/Article/details/gbhxhokiy.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.sjlbkw.cn/Article/details/glhsngghm.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.tarul.cn/Article/details/gwioofcbi.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gnsrxzlwh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.vehdjk.com/Article/details/gugoqlwnr.sHtML

[U75] PHP：依赖注入
来源：http://www.share.bbcook.cn/Article/details/gjhmujpjc.sHtML

composer require psr/container
来源：http://www.blog.epnwcf.com/Article/details/gpjmolrwk.sHtML

[U76] PHP：简单路由
来源：http://3g.bbcook.cn/Article/details/gtnzmjuid.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.tarul.cn/Article/details/gcehzbtgi.sHtML

[U77] PHP：模板渲染
来源：http://read.share.tarul.cn/Article/details/gfbocpoiw.sHtML

composer require twig/twig
来源：http://baike.yfazqb.com/Article/details/gmgpsjnqj.sHtML

[U78] PHP：单元测试
来源：http://mobile.tarul.cn/Article/details/goejgyzvu.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fktsv.cn/Article/details/ganwmrnxn.sHtML

[U79] PHP：静态分析
来源：http://wap.vehdjk.com/Article/details/gygdqjgvz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.epnwcf.com/Article/details/gdagbjfdj.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.tarul.cn/Article/details/gaqnvizrt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.sjlbkw.cn/Article/details/giwsqczdl.sHtML

[U81] JS：初始化项目
来源：http://read.share.sjlbkw.cn/Article/details/ghfnzqzes.sHtML

npm init -y;  npm i express
来源：http://baike.yfazqb.com/Article/details/gkeyxkggd.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.vehdjk.com/Article/details/gsrmqhjgx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.yfazqb.com/Article/details/gudrjsagl.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.epnwcf.com/Article/details/gwnhngcrd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.tarul.cn/Article/details/gstofeiga.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.tarul.cn/Article/details/gdcqtpazp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.bbcook.cn/Article/details/gflolbvjf.sHtML

[U85] JS：可选链
来源：http://www.m.share.vehdjk.com/Article/details/gagtdrtxc.sHtML

a?.b?.c
来源：http://www.blog.epnwcf.com/Article/details/gkjdrdccs.sHtML

[U86] JS：空值合并
来源：http://mobile.yfazqb.com/Article/details/gcbspimus.sHtML

a ?? b
来源：http://mobile.yfazqb.com/Article/details/guexhykyi.sHtML

[U87] JS：解构默认值
来源：http://www.share.sjlbkw.cn/Article/details/gtdvxczgb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.epnwcf.com/Article/details/gukzqzwou.sHtML

[U88] JS：对象展开合并
来源：http://read.share.bbcook.cn/Article/details/gayeidckt.sHtML

{ ...a, ...b }
来源：http://blog.tarul.cn/Article/details/gfhdykvls.sHtML

[U89] JS：数组去重
来源：http://m.share.tarul.cn/Article/details/gjskhyhzx.sHtML

[...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/gkevgsljy.sHtML

[U90] JS：数字数组排序
来源：http://baike.fktsv.cn/Article/details/gyaincrmq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gvjstdkks.sHtML

[U91] JS：对象键值遍历
来源：http://wap.vehdjk.com/Article/details/gdzfofkum.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.bbcook.cn/Article/details/geguvuzav.sHtML

[U92] JS：深拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gjefkezpf.sHtML

structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/guxgxnpdi.sHtML

[U93] JS：模板字符串
来源：http://mobile.bbcook.cn/Article/details/gqzqmmwps.sHtML

`共 ${n} 条`
来源：http://baike.tarul.cn/Article/details/gavmtrjxm.sHtML

[U94] JS：箭头函数
来源：http://www.share.vehdjk.com/Article/details/grskyfrml.sHtML

const double = x => x * 2;
来源：http://baike.epnwcf.com/Article/details/gkpmawtpf.sHtML

[U95] JS：Promise 包装
来源：http://blog.vehdjk.com/Article/details/gcfifbcib.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.bbcook.cn/Article/details/grsoiumgw.sHtML

[U96] JS：async/await 与异常
来源：http://3g.sjlbkw.cn/Article/details/gcdtobwuy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gybmdfutq.sHtML

[U97] JS：并发请求
来源：http://m.share.yfazqb.com/Article/details/glnimxmov.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gvmmhziix.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.epnwcf.com/Article/details/gpgujangd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.yfazqb.com/Article/details/gsesykvbl.sHtML

[U99] JS：事件监听
来源：http://3g.yfazqb.com/Article/details/gsiwzxdzt.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.tarul.cn/Article/details/gkaxkfmwh.sHtML

[U100] JS：DOM 查询
来源：http://www.share.tarul.cn/Article/details/gyipbjawd.sHtML

document.querySelector(".item")
来源：http://baike.yfazqb.com/Article/details/gkqqxnymv.sHtML

[U101] JS：classList 操作
来源：http://read.share.sjlbkw.cn/Article/details/gmktcmntz.sHtML

el.classList.toggle("active")
来源：http://baike.sjlbkw.cn/Article/details/gbbsxpwlj.sHtML

[U102] JS：本地存储
来源：http://www.blog.tarul.cn/Article/details/grhzqedav.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.vehdjk.com/Article/details/goikaybgc.sHtML

[U103] JS：定时器
来源：http://www.share.bbcook.cn/Article/details/ggejurmzr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.vehdjk.com/Article/details/goppmlqbr.sHtML

[U104] JS：防抖
来源：http://www.share.epnwcf.com/Article/details/gvuivzzmx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gwrxzvsfz.sHtML

[U105] JS：节流
来源：http://www.m.share.fktsv.cn/Article/details/gklstimpj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fktsv.cn/Article/details/gpbrhorep.sHtML

[U106] JS：日期格式化
来源：http://baike.tarul.cn/Article/details/gqtswufna.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.tarul.cn/Article/details/gffzvblne.sHtML

[U107] JS：数字千分位
来源：http://baike.yfazqb.com/Article/details/gzpvmfgah.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gnuiyrlzh.sHtML

[U108] JS：随机整数
来源：http://mobile.tarul.cn/Article/details/gnkfbsnuj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.vehdjk.com/Article/details/gkdyctkrb.sHtML

[U109] JS：数组分组
来源：http://www.blog.epnwcf.com/Article/details/golbshcvw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gysqregta.sHtML

[U110] JS：数组分块
来源：http://mobile.epnwcf.com/Article/details/gznxenrau.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.sjlbkw.cn/Article/details/ggaefvqhv.sHtML

[U111] JS：对象转 Map
来源：http://m.share.vehdjk.com/Article/details/gtfpbzytk.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gotrszekd.sHtML

[U112] JS：字符串补位
来源：http://wap.fktsv.cn/Article/details/gdkonidnu.sHtML

"7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gvchoromt.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fktsv.cn/Article/details/gqxfzzird.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gajpqayhp.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.sjlbkw.cn/Article/details/gwevkxjvj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.vehdjk.com/Article/details/ggjdnqswo.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.yfazqb.com/Article/details/gqqjvksfx.sHtML

crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gvbrwzidc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fktsv.cn/Article/details/glnrntsgu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fktsv.cn/Article/details/gratkcwrb.sHtML

[U117] JS：单元测试
来源：http://www.m.share.tarul.cn/Article/details/gcvojsdyw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.tarul.cn/Article/details/gwjffcvsm.sHtML

[U118] JS：开发服务器
来源：http://3g.fktsv.cn/Article/details/gkcpqpdar.sHtML

npm i -D vite;  npx vite
来源：http://3g.epnwcf.com/Article/details/glpthvwwr.sHtML

[U119] JS：生产构建
来源：http://3g.fktsv.cn/Article/details/gsvvyicwy.sHtML

npx vite build
来源：http://blog.fktsv.cn/Article/details/grsotmtxg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.sjlbkw.cn/Article/details/gymrhyodb.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fktsv.cn/Article/details/gomfbiido.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gkadchoeb.sHtML

统计汇总
来源：http://mobile.vehdjk.com/Article/details/gfphhwwto.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkxsuvoem.sHtML

按语言统计（条）：
来源：http://mobile.epnwcf.com/Article/details/ggyfvwvwk.sHtML

Python ......... 252
来源：http://www.m.share.bbcook.cn/Article/details/grlpnycjl.sHtML

PHP ............ 252
来源：http://blog.yfazqb.com/Article/details/gjpchewms.sHtML

JavaScript ..... 252
来源：http://3g.sjlbkw.cn/Article/details/gpppadina.sHtML

TypeScript ..... 212
来源：http://mobile.bbcook.cn/Article/details/gcpekjeps.sHtML

Java ........... 212
来源：http://wap.bbcook.cn/Article/details/gjbpxcuji.sHtML

Go ............. 212
来源：http://wap.vehdjk.com/Article/details/gkmvovpfw.sHtML

Ruby ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmaoujcm.sHtML

C# ............. 212
来源：http://m.share.vehdjk.com/Article/details/gdekjtbsn.sHtML

C .............. 30
来源：http://3g.bbcook.cn/Article/details/gyhgflbas.sHtML

C++ ............ 30
来源：http://www.m.share.sjlbkw.cn/Article/details/gochednfi.sHtML

SQL ............ 90
来源：http://baike.tarul.cn/Article/details/gdjctpptf.sHtML

Bash ........... 80
来源：http://mobile.sjlbkw.cn/Article/details/gmpvibvcf.sHtML

Kotlin ......... 15
来源：http://blog.yfazqb.com/Article/details/gkdmlrqfz.sHtML

Swift .......... 15
来源：http://mobile.vehdjk.com/Article/details/gwkrticwc.sHtML

Lua ............ 10
来源：http://www.m.share.vehdjk.com/Article/details/gudyrrsmd.sHtML

Perl ........... 10
来源：http://read.share.vehdjk.com/Article/details/gndzfzymq.sHtML

Scala .......... 10
来源：http://3g.sjlbkw.cn/Article/details/gbtuiqwym.sHtML

------------------------------------
来源：http://www.share.fktsv.cn/Article/details/givobhylt.sHtML

合计 ........... 2106 条
来源：http://www.m.share.vehdjk.com/Article/details/gefhezbhw.sHtML

按章节统计：
来源：http://wap.tarul.cn/Article/details/gpqkfxqbq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fktsv.cn/Article/details/gbelwgkem.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.epnwcf.com/Article/details/gzfprwdbh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/gjxvcurrw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.sjlbkw.cn/Article/details/gazecdckw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.epnwcf.com/Article/details/gbcnsfffy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.yfazqb.com/Article/details/gcgncgrip.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/gizznpuyw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.bbcook.cn/Article/details/gsqjrqdrv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gryihsqbg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.sjlbkw.cn/Article/details/gekofyrye.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gzgfzmhgn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.bbcook.cn/Article/details/ggpwlvwnm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gafhpptnk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.sjlbkw.cn/Article/details/giiafqjzq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fktsv.cn/Article/details/gzqlvtvuq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gnsgzimbz.sHtML

Q SQL 专题                              90
来源：http://mobile.sjlbkw.cn/Article/details/gjrjasdyb.sHtML

R Bash 专题                             80
来源：http://www.share.sjlbkw.cn/Article/details/gdchvrhni.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fktsv.cn/Article/details/gjjpucmvc.sHtML

T 其他语言补充                          60
来源：http://m.share.bbcook.cn/Article/details/guxmsbybk.sHtML

U 高频实用片段                         120
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpvptqim.sHtML

------------------------------------
来源：http://blog.vehdjk.com/Article/details/gpyquxlcg.sHtML

合计                                  2106 条
来源：http://blog.bbcook.cn/Article/details/gxhtlzrov.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gjkqhoevd.sHtML

使用提醒
来源：http://www.share.bbcook.cn/Article/details/gokorxacy.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gquxqdgki.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.sjlbkw.cn/Article/details/gkucbvgni.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.tarul.cn/Article/details/gdpniwkzv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.yfazqb.com/Article/details/gmudcmyxq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.bbcook.cn/Article/details/gnjfjqlym.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.yfazqb.com/Article/details/gvokgbcce.sHtML

—— 文件结束 ——
来源：http://3g.epnwcf.com/Article/details/gqmhojydn.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gesumbwjg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.bbcook.cn/Article/details/gybbqunyu.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.epnwcf.com/Article/details/gwewerail.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gacwfoxfa.sHtML

【收录内容】
来源：http://read.share.vehdjk.com/Article/details/gsdzfpgiz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.vehdjk.com/Article/details/gphlxbeij.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.bbcook.cn/Article/details/gllhvoujj.sHtML

SQL · Bash · C · C++
来源：http://www.blog.bbcook.cn/Article/details/ghdzevyhh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.sjlbkw.cn/Article/details/gmrqlgeei.sHtML

【使用说明】
来源：http://www.share.epnwcf.com/Article/details/gjitbkcnd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.tarul.cn/Article/details/giipmudgd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.tarul.cn/Article/details/ghxpbupoi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.sjlbkw.cn/Article/details/garwewjav.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.yfazqb.com/Article/details/ggdnibpri.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.bbcook.cn/Article/details/gxxwigbwb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.vehdjk.com/Article/details/ghuctzsnv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.tarul.cn/Article/details/gcibquhas.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fktsv.cn/Article/details/gleoeijcr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.vehdjk.com/Article/details/ghrryhcem.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.bbcook.cn/Article/details/gbbvssyoc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.sjlbkw.cn/Article/details/glggzashf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.epnwcf.com/Article/details/grxaoypsd.sHtML

【文件统计】
来源：http://www.share.fktsv.cn/Article/details/gkahfqnny.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.epnwcf.com/Article/details/glwstghgx.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gjgqxrrnh.sHtML

目  录
来源：http://www.m.share.tarul.cn/Article/details/glifddfxh.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gmkcrsyae.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.yfazqb.com/Article/details/glpihqhfi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gdrbpsskz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.yfazqb.com/Article/details/ggkbemlfx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gfybkghnv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.epnwcf.com/Article/details/gangnrvmx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.bbcook.cn/Article/details/gnnisnkvv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/gzmdftyuu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/gaajjdsot.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gzpxpuwkm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.vehdjk.com/Article/details/gbhyqmgoj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/guwpeepch.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gutmnletb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gygjsdgnc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gaeerutuz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fktsv.cn/Article/details/gpwyjkjyz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/groicgkdi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.vehdjk.com/Article/details/gdzdmioif.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.tarul.cn/Article/details/gwoycvifl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.epnwcf.com/Article/details/gpugjvmmy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/gyzgsujhj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/ghizinnxg.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gibrjdyzd.sHtML

A. 基础语法与类型
来源：http://www.m.share.tarul.cn/Article/details/gmqsjjhpt.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzubyppbv.sHtML

[A01] Hello World
来源：http://wap.fktsv.cn/Article/details/gtsnqqqwb.sHtML

Py:   print("Hello, World!")
来源：http://mobile.yfazqb.com/Article/details/gamspjoxh.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.tarul.cn/Article/details/gbkzwjgpg.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.epnwcf.com/Article/details/gmnovukyg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.sjlbkw.cn/Article/details/gbowoejzj.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/ganoivkmx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.sjlbkw.cn/Article/details/gchszanux.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.yfazqb.com/Article/details/gvachyrlo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.yfazqb.com/Article/details/gjvbpwlsd.sHtML

[A02] 变量声明与赋值
来源：http://blog.epnwcf.com/Article/details/gmlqrdjsq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.bbcook.cn/Article/details/gpwntxsmb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.tarul.cn/Article/details/gxlkowfyn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.vehdjk.com/Article/details/gezlboekp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.yfazqb.com/Article/details/gysvwfuds.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gaufmuefm.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.epnwcf.com/Article/details/gnliielyi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.epnwcf.com/Article/details/ggevtfmtd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.tarul.cn/Article/details/gotguabos.sHtML

[A03] 常量定义
来源：http://www.share.tarul.cn/Article/details/gropxphkq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.tarul.cn/Article/details/gxfqvfgio.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gojnofrti.sHtML


<!-- 参考信息 -->