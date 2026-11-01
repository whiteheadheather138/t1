代发 wailian999

[U31] Py：单测
来源：http://3g.vehdjk.com/Article/details/gnvuepiow.sHtML

python -m pytest -q
来源：http://www.blog.epnwcf.com/Article/details/giltyfmnp.sHtML

[U32] Py：代码格式化
来源：http://m.share.sjlbkw.cn/Article/details/gxtnczslv.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fktsv.cn/Article/details/ggicsydnk.sHtML

[U33] Py：打包发布
来源：http://blog.tarul.cn/Article/details/ggmvmolua.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.vehdjk.com/Article/details/gpqvctxgp.sHtML

[U34] Py：判断编码
来源：http://3g.bbcook.cn/Article/details/gkasqhicf.sHtML

chardet.detect(raw)
来源：http://3g.sjlbkw.cn/Article/details/gtzhtiuij.sHtML

[U35] Py：发送邮件
来源：http://baike.vehdjk.com/Article/details/ggvjvyual.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.bbcook.cn/Article/details/gnxgfhmmb.sHtML

[U36] Py：定时任务
来源：http://blog.bbcook.cn/Article/details/gcrjmzgse.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.epnwcf.com/Article/details/gmjgkkkol.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.bbcook.cn/Article/details/gyqiedpfq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.tarul.cn/Article/details/gdhehrfik.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.tarul.cn/Article/details/gefsvkivv.sHtML

Path(__file__).resolve().parent
来源：http://www.share.sjlbkw.cn/Article/details/ghhizfklq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fktsv.cn/Article/details/gvypscthg.sHtML

sys.stdout.isatty()
来源：http://www.blog.vehdjk.com/Article/details/geivgcwxc.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fktsv.cn/Article/details/gpyidxfmb.sHtML

print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gygasxkbn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.vehdjk.com/Article/details/gndjqjxcb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.bbcook.cn/Article/details/gwvdobbzt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fktsv.cn/Article/details/gduldtwwc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.sjlbkw.cn/Article/details/gkmvitguf.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gbyotgcay.sHtML

namespace App\Http;
来源：http://m.share.yfazqb.com/Article/details/gsthxqobw.sHtML

[U44] PHP：开启严格类型
来源：http://blog.tarul.cn/Article/details/gmmhocgjd.sHtML

declare(strict_types=1);
来源：http://blog.tarul.cn/Article/details/gpnewqkhj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.tarul.cn/Article/details/ggopctrcu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gftlhpznd.sHtML

[U46] PHP：可空类型
来源：http://www.blog.bbcook.cn/Article/details/guqsijatv.sHtML

?string $name = null
来源：http://wap.vehdjk.com/Article/details/gjiwotkns.sHtML

[U47] PHP：联合类型
来源：http://m.share.sjlbkw.cn/Article/details/gggtjsmjl.sHtML

int|string $id
来源：http://mobile.epnwcf.com/Article/details/gfsdvkuis.sHtML

[U48] PHP：纯枚举
来源：http://3g.sjlbkw.cn/Article/details/gkblqccom.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.epnwcf.com/Article/details/gvjxsgsma.sHtML

[U49] PHP：只读属性
来源：http://blog.yfazqb.com/Article/details/gyjpflfmu.sHtML

public readonly string $name
来源：http://blog.bbcook.cn/Article/details/ggxlofblg.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.bbcook.cn/Article/details/goctpdlbk.sHtML

public function __construct(private int $id) {}
来源：http://www.share.bbcook.cn/Article/details/gdchemcax.sHtML

[U51] PHP：数组解构
来源：http://mobile.bbcook.cn/Article/details/gambhhqhd.sHtML

[$a, $b] = $arr;
来源：http://read.share.yfazqb.com/Article/details/gesxsxlwv.sHtML

[U52] PHP：箭头函数
来源：http://m.share.tarul.cn/Article/details/gzlvvahtt.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.epnwcf.com/Article/details/gafnugsna.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fktsv.cn/Article/details/gyfdytdcd.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.vehdjk.com/Article/details/gsupisihj.sHtML

[U54] PHP：空安全调用
来源：http://3g.epnwcf.com/Article/details/gmpobbbmb.sHtML

$obj?->method()
来源：http://m.share.tarul.cn/Article/details/gfqhjmjja.sHtML

[U55] PHP：match 表达式
来源：http://blog.tarul.cn/Article/details/gfyzdyrpq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/gzbratqrl.sHtML

[U56] PHP：命名参数
来源：http://mobile.sjlbkw.cn/Article/details/glxdxvcrb.sHtML

f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gqpvtbyue.sHtML

[U57] PHP：字符串插值
来源：http://wap.epnwcf.com/Article/details/gcedomuao.sHtML

"值: {$a}"
来源：http://blog.epnwcf.com/Article/details/gtcqwakvv.sHtML

[U58] PHP：数组三件套
来源：http://blog.vehdjk.com/Article/details/gpknazfxr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.vehdjk.com/Article/details/gaqvlyonf.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fktsv.cn/Article/details/gqgchhvhe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.bbcook.cn/Article/details/gzoozooit.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.sjlbkw.cn/Article/details/gnvqacjyc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.yfazqb.com/Article/details/gnmvyhxve.sHtML

[U61] PHP：正则
来源：http://baike.bbcook.cn/Article/details/gpkmssrhm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.bbcook.cn/Article/details/ghqfmztmz.sHtML

[U62] PHP：日期对象
来源：http://3g.vehdjk.com/Article/details/guoyqllpq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.vehdjk.com/Article/details/gkscgqmza.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fktsv.cn/Article/details/gjpryklja.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.vehdjk.com/Article/details/gfpkvrgse.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fktsv.cn/Article/details/goafmcwzc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.bbcook.cn/Article/details/gkokqaive.sHtML

[U65] PHP：会话
来源：http://mobile.fktsv.cn/Article/details/gzxxkchui.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/glaqgrsov.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.bbcook.cn/Article/details/goicuynld.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fktsv.cn/Article/details/glhwurfcx.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.bbcook.cn/Article/details/gfubkgcgg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fktsv.cn/Article/details/glovnuwzy.sHtML

[U68] PHP：PDO 连接
来源：http://3g.tarul.cn/Article/details/gmutllcho.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.bbcook.cn/Article/details/grxsnllsf.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.tarul.cn/Article/details/guqasgipd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.epnwcf.com/Article/details/goqblikfl.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.yfazqb.com/Article/details/gyvjsqjun.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.sjlbkw.cn/Article/details/gmrnvnpro.sHtML

[U71] PHP：抛出异常
来源：http://m.share.tarul.cn/Article/details/gtrrqdieg.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.yfazqb.com/Article/details/gkjpdvkhz.sHtML

[U72] PHP：写错误日志
来源：http://mobile.tarul.cn/Article/details/gyufyrgyg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.epnwcf.com/Article/details/gfunupkti.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.bbcook.cn/Article/details/gsvupeyfb.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.bbcook.cn/Article/details/gsqdsectk.sHtML

[U74] PHP：读取环境变量
来源：http://wap.tarul.cn/Article/details/gptnsbnjp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.yfazqb.com/Article/details/gwyrnulcq.sHtML

[U75] PHP：依赖注入
来源：http://m.share.bbcook.cn/Article/details/gdemxcopk.sHtML

composer require psr/container
来源：http://baike.fktsv.cn/Article/details/gvjoqhswf.sHtML

[U76] PHP：简单路由
来源：http://baike.tarul.cn/Article/details/ghrwavvfr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.tarul.cn/Article/details/gcgesydbv.sHtML

[U77] PHP：模板渲染
来源：http://mobile.bbcook.cn/Article/details/gnaecnaev.sHtML

composer require twig/twig
来源：http://www.share.bbcook.cn/Article/details/gecrkfhle.sHtML

[U78] PHP：单元测试
来源：http://blog.sjlbkw.cn/Article/details/ghtkaeiof.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fktsv.cn/Article/details/gxnqmrvnz.sHtML

[U79] PHP：静态分析
来源：http://blog.epnwcf.com/Article/details/gfpmshpqk.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.bbcook.cn/Article/details/gohijrmzu.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.bbcook.cn/Article/details/guchugvbq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.bbcook.cn/Article/details/gmyoxofzz.sHtML

[U81] JS：初始化项目
来源：http://www.share.bbcook.cn/Article/details/gxfgjiqhp.sHtML

npm init -y;  npm i express
来源：http://www.blog.epnwcf.com/Article/details/gaevnjpns.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.sjlbkw.cn/Article/details/gsemexksz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.tarul.cn/Article/details/giikjtumc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.tarul.cn/Article/details/ggpzjntxo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gzwcewhvi.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.epnwcf.com/Article/details/gnrrqmfjt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.vehdjk.com/Article/details/gywjokzjo.sHtML

[U85] JS：可选链
来源：http://mobile.epnwcf.com/Article/details/gvhvbgldx.sHtML

a?.b?.c
来源：http://m.share.sjlbkw.cn/Article/details/gardkruik.sHtML

[U86] JS：空值合并
来源：http://wap.sjlbkw.cn/Article/details/gnmoirumi.sHtML

a ?? b
来源：http://blog.yfazqb.com/Article/details/gsmpzyxth.sHtML

[U87] JS：解构默认值
来源：http://www.share.tarul.cn/Article/details/giowzjzup.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.vehdjk.com/Article/details/gikeqzbqe.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.yfazqb.com/Article/details/gogflmsod.sHtML

{ ...a, ...b }
来源：http://read.share.epnwcf.com/Article/details/gqdmvqqio.sHtML

[U89] JS：数组去重
来源：http://www.blog.tarul.cn/Article/details/gtzuwmqcf.sHtML

[...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/grtmhiweg.sHtML

[U90] JS：数字数组排序
来源：http://www.share.vehdjk.com/Article/details/gyptqkxjv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gwqydccvj.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.bbcook.cn/Article/details/gkyqcvlry.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.bbcook.cn/Article/details/gqfversyh.sHtML

[U92] JS：深拷贝
来源：http://www.blog.tarul.cn/Article/details/gwsukyqdn.sHtML

structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gdbtccdcr.sHtML

[U93] JS：模板字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gqxmunbmq.sHtML

`共 ${n} 条`
来源：http://www.m.share.vehdjk.com/Article/details/gjfruuhcy.sHtML

[U94] JS：箭头函数
来源：http://mobile.sjlbkw.cn/Article/details/gaqjemotp.sHtML

const double = x => x * 2;
来源：http://read.share.vehdjk.com/Article/details/ghqweiurt.sHtML

[U95] JS：Promise 包装
来源：http://wap.epnwcf.com/Article/details/gjhwwoywc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gggqwezyg.sHtML

[U96] JS：async/await 与异常
来源：http://blog.vehdjk.com/Article/details/gfqyixczl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gfhhlgzlu.sHtML

[U97] JS：并发请求
来源：http://wap.epnwcf.com/Article/details/gqgnyfizy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gcczefnfw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/goufucmza.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.epnwcf.com/Article/details/gapbvqvsk.sHtML

[U99] JS：事件监听
来源：http://m.share.bbcook.cn/Article/details/ginoufikz.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.bbcook.cn/Article/details/gtblrwiae.sHtML

[U100] JS：DOM 查询
来源：http://wap.fktsv.cn/Article/details/gwvskxiua.sHtML

document.querySelector(".item")
来源：http://www.blog.yfazqb.com/Article/details/ghufxoqli.sHtML

[U101] JS：classList 操作
来源：http://wap.fktsv.cn/Article/details/gchlwpgnw.sHtML

el.classList.toggle("active")
来源：http://m.share.tarul.cn/Article/details/gvouuuzgb.sHtML

[U102] JS：本地存储
来源：http://3g.epnwcf.com/Article/details/gwfyjkmek.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.yfazqb.com/Article/details/gwjjtrgwi.sHtML

[U103] JS：定时器
来源：http://blog.bbcook.cn/Article/details/gmjqtjgnz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.epnwcf.com/Article/details/gylfjobzi.sHtML

[U104] JS：防抖
来源：http://www.share.epnwcf.com/Article/details/gjunrjvoz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gmqoxcwip.sHtML

[U105] JS：节流
来源：http://read.share.bbcook.cn/Article/details/gtvqaixjb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.tarul.cn/Article/details/gaipyyvzd.sHtML

[U106] JS：日期格式化
来源：http://wap.bbcook.cn/Article/details/gmtkbdlzb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.tarul.cn/Article/details/gdnlnmmfr.sHtML

[U107] JS：数字千分位
来源：http://blog.tarul.cn/Article/details/gkixanbrz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.tarul.cn/Article/details/guesqmpob.sHtML

[U108] JS：随机整数
来源：http://www.m.share.bbcook.cn/Article/details/gcrjunkxz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.bbcook.cn/Article/details/gdxmswyko.sHtML

[U109] JS：数组分组
来源：http://www.m.share.sjlbkw.cn/Article/details/glijybevp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/gyxlxdgyh.sHtML

[U110] JS：数组分块
来源：http://3g.fktsv.cn/Article/details/gglgfzeev.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.tarul.cn/Article/details/gxocgzogz.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.bbcook.cn/Article/details/gngxcegam.sHtML

new Map(Object.entries(obj))
来源：http://blog.vehdjk.com/Article/details/gstkgccct.sHtML

[U112] JS：字符串补位
来源：http://blog.vehdjk.com/Article/details/gxxiurajm.sHtML

"7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gdjdgftsp.sHtML

[U113] JS：正则替换全部
来源：http://3g.bbcook.cn/Article/details/gzbcvrbzm.sHtML

s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/grxrvbvwc.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.sjlbkw.cn/Article/details/gfqsuweuz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/gmayrhvpq.sHtML

[U115] JS：生成 UUID
来源：http://blog.yfazqb.com/Article/details/gnszejkzq.sHtML

crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gbbgsajdk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fktsv.cn/Article/details/gyhftraju.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gmkjwemmk.sHtML

[U117] JS：单元测试
来源：http://read.share.bbcook.cn/Article/details/gmaockswa.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.epnwcf.com/Article/details/garrftpjb.sHtML

[U118] JS：开发服务器
来源：http://m.share.fktsv.cn/Article/details/gncxpelix.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fktsv.cn/Article/details/giitciehx.sHtML

[U119] JS：生产构建
来源：http://www.m.share.epnwcf.com/Article/details/gpgoaljfo.sHtML

npx vite build
来源：http://www.m.share.fktsv.cn/Article/details/gpuzgwuob.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.yfazqb.com/Article/details/gfxrfxcrf.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.sjlbkw.cn/Article/details/gxpakofdh.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gnfgrjaxs.sHtML

统计汇总
来源：http://read.share.vehdjk.com/Article/details/ghgjjmfhd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvkykmisi.sHtML

按语言统计（条）：
来源：http://wap.bbcook.cn/Article/details/gfthdlmhd.sHtML

Python ......... 252
来源：http://www.share.vehdjk.com/Article/details/gatwrcauf.sHtML

PHP ............ 252
来源：http://m.share.tarul.cn/Article/details/gaxsnbcfj.sHtML

JavaScript ..... 252
来源：http://read.share.epnwcf.com/Article/details/gxqoqsyzj.sHtML

TypeScript ..... 212
来源：http://www.share.fktsv.cn/Article/details/gtzjirmkq.sHtML

Java ........... 212
来源：http://baike.sjlbkw.cn/Article/details/gjrdcuahy.sHtML

Go ............. 212
来源：http://wap.epnwcf.com/Article/details/gxkdqaayy.sHtML

Ruby ........... 212
来源：http://blog.vehdjk.com/Article/details/gnusbogim.sHtML

C# ............. 212
来源：http://m.share.epnwcf.com/Article/details/gurfbaslu.sHtML

C .............. 30
来源：http://www.m.share.vehdjk.com/Article/details/gydllcrvm.sHtML

C++ ............ 30
来源：http://wap.vehdjk.com/Article/details/guqgzqgtt.sHtML

SQL ............ 90
来源：http://wap.tarul.cn/Article/details/ghcrdxvlt.sHtML

Bash ........... 80
来源：http://wap.vehdjk.com/Article/details/gbtzwxqde.sHtML

Kotlin ......... 15
来源：http://mobile.epnwcf.com/Article/details/gtkxwhmxv.sHtML

Swift .......... 15
来源：http://wap.epnwcf.com/Article/details/golniqabq.sHtML

Lua ............ 10
来源：http://baike.yfazqb.com/Article/details/gvmyuoyoy.sHtML

Perl ........... 10
来源：http://read.share.epnwcf.com/Article/details/gokmrjrae.sHtML

Scala .......... 10
来源：http://wap.tarul.cn/Article/details/gfyrpbffs.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gxmrxwqbp.sHtML

合计 ........... 2106 条
来源：http://3g.bbcook.cn/Article/details/guqiopkfa.sHtML

按章节统计：
来源：http://blog.yfazqb.com/Article/details/gpkhtsref.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.vehdjk.com/Article/details/gdmforhan.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gnuadubvm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/gcugtzcqq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.sjlbkw.cn/Article/details/gygfyrgby.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.tarul.cn/Article/details/gnumkehiz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.yfazqb.com/Article/details/gnktssuff.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/ggsubobcg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/grjnxlxlb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/guahgrcrz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.yfazqb.com/Article/details/gatnsprlr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gttrtslsi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gvdoeoxuv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gbxnfafmt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/gcrnsestv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.bbcook.cn/Article/details/gmeqbajue.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gnmnqgvbk.sHtML

Q SQL 专题                              90
来源：http://m.share.vehdjk.com/Article/details/ggmznzegx.sHtML

R Bash 专题                             80
来源：http://3g.bbcook.cn/Article/details/gysfsbtms.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.yfazqb.com/Article/details/guzlezsvk.sHtML

T 其他语言补充                          60
来源：http://www.share.fktsv.cn/Article/details/gzrnyaafd.sHtML

U 高频实用片段                         120
来源：http://www.share.tarul.cn/Article/details/gibbpdtou.sHtML

------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gbuxyhejl.sHtML

合计                                  2106 条
来源：http://www.share.vehdjk.com/Article/details/gtewvkgld.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gauyiaqkv.sHtML

使用提醒
来源：http://mobile.tarul.cn/Article/details/gwmnxdwjp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gwkpwtjvx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.vehdjk.com/Article/details/gizwsiyhb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.sjlbkw.cn/Article/details/gkypyfziv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.yfazqb.com/Article/details/gmbjumifr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.sjlbkw.cn/Article/details/gltcmlewv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.tarul.cn/Article/details/gykhbuaxe.sHtML

—— 文件结束 ——
来源：http://wap.yfazqb.com/Article/details/glmoyiiwc.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gshwsxwoj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.epnwcf.com/Article/details/gvxydqedd.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.sjlbkw.cn/Article/details/gsrkgrpid.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmffdvnbf.sHtML

【收录内容】
来源：http://wap.vehdjk.com/Article/details/gqektgvhf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fktsv.cn/Article/details/gznixodpv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.vehdjk.com/Article/details/ggrvnwvqh.sHtML

SQL · Bash · C · C++
来源：http://read.share.epnwcf.com/Article/details/gnhwqeezw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.sjlbkw.cn/Article/details/gvdsmyhma.sHtML

【使用说明】
来源：http://m.share.yfazqb.com/Article/details/ggbwhwldm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.tarul.cn/Article/details/genrdtmda.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.vehdjk.com/Article/details/geqqkzdwt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.tarul.cn/Article/details/ggwcevljr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.tarul.cn/Article/details/gekzmscrl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.epnwcf.com/Article/details/gbrgtjyct.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.bbcook.cn/Article/details/ghdixlqje.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.epnwcf.com/Article/details/gdtgarhvf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.fktsv.cn/Article/details/gehbatnhw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.vehdjk.com/Article/details/gfqmaznfh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.yfazqb.com/Article/details/gomshavjs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fktsv.cn/Article/details/gkadqewhg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.bbcook.cn/Article/details/gxviebcpn.sHtML

【文件统计】
来源：http://3g.yfazqb.com/Article/details/gsteihljd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.yfazqb.com/Article/details/gipzdoytj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gsiojycbi.sHtML

目  录
来源：http://wap.epnwcf.com/Article/details/geuwmbwor.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gmifzpuzw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.bbcook.cn/Article/details/gjcgvucxn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/gtqcpunjd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/grynsaije.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.bbcook.cn/Article/details/grndypdha.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.epnwcf.com/Article/details/gmjzwxaum.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.epnwcf.com/Article/details/glykhsbyk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.bbcook.cn/Article/details/gteoegjig.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fktsv.cn/Article/details/gihogufoz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gssrzidkw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fktsv.cn/Article/details/ggypydici.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/glyitqmts.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/gjeydhfkj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gtfzsyiks.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.vehdjk.com/Article/details/gfplqizas.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.epnwcf.com/Article/details/gxgnccfwc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gshgihwwj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.tarul.cn/Article/details/gfirpcntr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.epnwcf.com/Article/details/gqbodwieq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.tarul.cn/Article/details/gwzrnbnhx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/gtrldlaqq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.yfazqb.com/Article/details/gieipousz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ghergntyv.sHtML

A. 基础语法与类型
来源：http://3g.yfazqb.com/Article/details/gdgrslpzr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqflkkfzd.sHtML

[A01] Hello World
来源：http://www.blog.tarul.cn/Article/details/gymllchcg.sHtML

Py:   print("Hello, World!")
来源：http://wap.fktsv.cn/Article/details/gfsnupcvm.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fktsv.cn/Article/details/gizkobrgb.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gmtqtbngk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.bbcook.cn/Article/details/gynfvmmif.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gvclbwign.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fktsv.cn/Article/details/gzswordoy.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.yfazqb.com/Article/details/gdpgymdkl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.tarul.cn/Article/details/gjzbkezyw.sHtML

[A02] 变量声明与赋值
来源：http://m.share.tarul.cn/Article/details/gktomowyk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.yfazqb.com/Article/details/gemwtjkvz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fktsv.cn/Article/details/ghxsrlmab.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fktsv.cn/Article/details/giqyegydf.sHtML


<!-- 参考信息 -->