代发 wailian999

[U29] Py：属性校验
来源：http://baike.tarul.cn/Article/details/gxvhqsnyc.sHtML

@property 与 @x.setter 配合
来源：http://read.share.vehdjk.com/Article/details/gjudywwdh.sHtML

[U30] Py：数据类
来源：http://www.share.tarul.cn/Article/details/guibpybpv.sHtML

@dataclass(slots=True)
来源：http://www.share.vehdjk.com/Article/details/gwxrzdfug.sHtML

[U31] Py：单测
来源：http://www.m.share.vehdjk.com/Article/details/gvcjvgeel.sHtML

python -m pytest -q
来源：http://wap.bbcook.cn/Article/details/gcihxicex.sHtML

[U32] Py：代码格式化
来源：http://m.share.yfazqb.com/Article/details/gqtbgiegn.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.vehdjk.com/Article/details/gzdyjfhag.sHtML

[U33] Py：打包发布
来源：http://3g.yfazqb.com/Article/details/gneenqucv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.yfazqb.com/Article/details/gdboqgpex.sHtML

[U34] Py：判断编码
来源：http://baike.tarul.cn/Article/details/gioudcghb.sHtML

chardet.detect(raw)
来源：http://read.share.sjlbkw.cn/Article/details/ghvfvksdw.sHtML

[U35] Py：发送邮件
来源：http://blog.tarul.cn/Article/details/gmuxxwokp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.bbcook.cn/Article/details/gfrsjhepz.sHtML

[U36] Py：定时任务
来源：http://blog.yfazqb.com/Article/details/gnngfquzb.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.vehdjk.com/Article/details/gcwdtotmz.sHtML

[U37] Py：读写 Excel
来源：http://m.share.epnwcf.com/Article/details/gknmfifks.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.tarul.cn/Article/details/grkgqurwg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.epnwcf.com/Article/details/gbfmvivwx.sHtML

Path(__file__).resolve().parent
来源：http://www.share.yfazqb.com/Article/details/gafaxjdwz.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.bbcook.cn/Article/details/gaxshqkmy.sHtML

sys.stdout.isatty()
来源：http://read.share.tarul.cn/Article/details/gcvrfdyqo.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fktsv.cn/Article/details/gihfsscdz.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gngwbofvb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.yfazqb.com/Article/details/gprdewfzv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.epnwcf.com/Article/details/ghffhxufy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.epnwcf.com/Article/details/gnyzahahx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.vehdjk.com/Article/details/gqiyhreyb.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.epnwcf.com/Article/details/gthueeemw.sHtML

namespace App\Http;
来源：http://www.blog.epnwcf.com/Article/details/gzfphofvj.sHtML

[U44] PHP：开启严格类型
来源：http://wap.epnwcf.com/Article/details/gpvxcghmd.sHtML

declare(strict_types=1);
来源：http://www.share.bbcook.cn/Article/details/gggkyyfos.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzkxabaz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gvctlptxo.sHtML

[U46] PHP：可空类型
来源：http://read.share.vehdjk.com/Article/details/gedqddqlg.sHtML

?string $name = null
来源：http://baike.bbcook.cn/Article/details/gyrsipqhm.sHtML

[U47] PHP：联合类型
来源：http://read.share.fktsv.cn/Article/details/gexguucoe.sHtML

int|string $id
来源：http://blog.tarul.cn/Article/details/gejasbkja.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.epnwcf.com/Article/details/gfzelxktb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.sjlbkw.cn/Article/details/gmvwbgssg.sHtML

[U49] PHP：只读属性
来源：http://blog.tarul.cn/Article/details/gupjlklxm.sHtML

public readonly string $name
来源：http://www.m.share.sjlbkw.cn/Article/details/gpamxkvlr.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.yfazqb.com/Article/details/ginoskozc.sHtML

public function __construct(private int $id) {}
来源：http://blog.sjlbkw.cn/Article/details/gepotddwk.sHtML

[U51] PHP：数组解构
来源：http://3g.vehdjk.com/Article/details/gfnnglecg.sHtML

[$a, $b] = $arr;
来源：http://www.blog.epnwcf.com/Article/details/gdplpsyop.sHtML

[U52] PHP：箭头函数
来源：http://read.share.bbcook.cn/Article/details/ggnvbfynx.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.tarul.cn/Article/details/gyakgsptn.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.tarul.cn/Article/details/gclzwtgtg.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fktsv.cn/Article/details/gupnwlrvb.sHtML

[U54] PHP：空安全调用
来源：http://blog.yfazqb.com/Article/details/gajfjcdym.sHtML

$obj?->method()
来源：http://www.m.share.fktsv.cn/Article/details/gwvvnfvdp.sHtML

[U55] PHP：match 表达式
来源：http://read.share.epnwcf.com/Article/details/gclvhonek.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.vehdjk.com/Article/details/gitmdqrhn.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.tarul.cn/Article/details/gilsuthtb.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gzqncotjm.sHtML

[U57] PHP：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gplkpgrmc.sHtML

"值: {$a}"
来源：http://www.blog.epnwcf.com/Article/details/gcwtcywjz.sHtML

[U58] PHP：数组三件套
来源：http://m.share.tarul.cn/Article/details/gqleyhgut.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.epnwcf.com/Article/details/gzulolynw.sHtML

[U59] PHP：自定义排序
来源：http://blog.fktsv.cn/Article/details/ggwwngrde.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gdzuxqywa.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.tarul.cn/Article/details/grosaprrp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.epnwcf.com/Article/details/gtquoswxd.sHtML

[U61] PHP：正则
来源：http://www.blog.fktsv.cn/Article/details/glusldhjh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/gmgskritq.sHtML

[U62] PHP：日期对象
来源：http://www.share.sjlbkw.cn/Article/details/gqqdrqqsj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.yfazqb.com/Article/details/gvapcbxqv.sHtML

[U63] PHP：文件读写
来源：http://read.share.fktsv.cn/Article/details/grghywxrd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.bbcook.cn/Article/details/gpozspxii.sHtML

[U64] PHP：目录遍历
来源：http://baike.tarul.cn/Article/details/gqbolhatu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.tarul.cn/Article/details/ggbwuqrtt.sHtML

[U65] PHP：会话
来源：http://blog.bbcook.cn/Article/details/gaodqffqd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gswlwmcss.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.bbcook.cn/Article/details/goowpijbf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.yfazqb.com/Article/details/gozdvicyn.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.sjlbkw.cn/Article/details/gawjcimgh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fktsv.cn/Article/details/gyusmhvol.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.epnwcf.com/Article/details/ghorigjgh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.yfazqb.com/Article/details/gdwiuwcnv.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.vehdjk.com/Article/details/glrmkzcjh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.yfazqb.com/Article/details/gubhrfoat.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.vehdjk.com/Article/details/gxhuwdceb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.sjlbkw.cn/Article/details/ggzuhopzc.sHtML

[U71] PHP：抛出异常
来源：http://baike.bbcook.cn/Article/details/ghwmhxuap.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.vehdjk.com/Article/details/gpllpnoye.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.tarul.cn/Article/details/gbaglwnoq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.epnwcf.com/Article/details/gzfraoguv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.bbcook.cn/Article/details/gxknygntk.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.yfazqb.com/Article/details/guiqtbmhl.sHtML

[U74] PHP：读取环境变量
来源：http://3g.vehdjk.com/Article/details/geyobvogh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fktsv.cn/Article/details/gvwpccepg.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.tarul.cn/Article/details/gxvcsxnfd.sHtML

composer require psr/container
来源：http://www.m.share.sjlbkw.cn/Article/details/gytrrfvgk.sHtML

[U76] PHP：简单路由
来源：http://m.share.vehdjk.com/Article/details/gakebjtcq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.bbcook.cn/Article/details/gglnuijms.sHtML

[U77] PHP：模板渲染
来源：http://wap.bbcook.cn/Article/details/gbxirkqgo.sHtML

composer require twig/twig
来源：http://read.share.bbcook.cn/Article/details/grxllqtby.sHtML

[U78] PHP：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/gdpsvlfvd.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.epnwcf.com/Article/details/gxegbhdby.sHtML

[U79] PHP：静态分析
来源：http://3g.tarul.cn/Article/details/gpodxegyp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.tarul.cn/Article/details/gcbygvqnm.sHtML

[U80] PHP：代码规范修复
来源：http://baike.tarul.cn/Article/details/gaptvuqmz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.tarul.cn/Article/details/ghdcqcmnf.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.yfazqb.com/Article/details/ghhnxaebt.sHtML

npm init -y;  npm i express
来源：http://blog.vehdjk.com/Article/details/gwmrxfjub.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.sjlbkw.cn/Article/details/glekpzxfu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.bbcook.cn/Article/details/gzfhtexts.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.yfazqb.com/Article/details/gbmblohbe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.tarul.cn/Article/details/gqwffjake.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.sjlbkw.cn/Article/details/gqrhrjhdh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.sjlbkw.cn/Article/details/gfkyvitsi.sHtML

[U85] JS：可选链
来源：http://www.share.epnwcf.com/Article/details/gutrvfkop.sHtML

a?.b?.c
来源：http://m.share.tarul.cn/Article/details/gjrzyegye.sHtML

[U86] JS：空值合并
来源：http://www.blog.vehdjk.com/Article/details/gvyuftqcl.sHtML

a ?? b
来源：http://www.share.bbcook.cn/Article/details/gazuesanh.sHtML

[U87] JS：解构默认值
来源：http://3g.vehdjk.com/Article/details/gzpjquysp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.yfazqb.com/Article/details/gryaaoxpv.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fktsv.cn/Article/details/grerywicy.sHtML

{ ...a, ...b }
来源：http://m.share.yfazqb.com/Article/details/gyyhnaraz.sHtML

[U89] JS：数组去重
来源：http://baike.vehdjk.com/Article/details/gcvqloglt.sHtML

[...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gwjgiednc.sHtML

[U90] JS：数字数组排序
来源：http://wap.fktsv.cn/Article/details/gysyozikf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gzifqvpxh.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fktsv.cn/Article/details/gjsfchywl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.yfazqb.com/Article/details/gsnccywix.sHtML

[U92] JS：深拷贝
来源：http://wap.yfazqb.com/Article/details/gawqkuvxs.sHtML

structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gjoccxmlg.sHtML

[U93] JS：模板字符串
来源：http://baike.sjlbkw.cn/Article/details/gdcpkayte.sHtML

`共 ${n} 条`
来源：http://read.share.sjlbkw.cn/Article/details/gybyvffeq.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/ghoircguu.sHtML

const double = x => x * 2;
来源：http://read.share.bbcook.cn/Article/details/gmjrquyqr.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fktsv.cn/Article/details/gcrvbztzl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.vehdjk.com/Article/details/geqsgutco.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.tarul.cn/Article/details/gmdzxqxso.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gttqmgxej.sHtML

[U97] JS：并发请求
来源：http://www.share.vehdjk.com/Article/details/glyzmltxc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gcbhwukyl.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gfuupijyn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.yfazqb.com/Article/details/gqzodrxgf.sHtML

[U99] JS：事件监听
来源：http://www.share.fktsv.cn/Article/details/gjiwldwqm.sHtML

el.addEventListener("click", e => {})
来源：http://wap.vehdjk.com/Article/details/ghsbzjric.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.bbcook.cn/Article/details/geyxwepty.sHtML

document.querySelector(".item")
来源：http://m.share.yfazqb.com/Article/details/gmcjxfjkr.sHtML

[U101] JS：classList 操作
来源：http://mobile.sjlbkw.cn/Article/details/gwszupxgu.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fktsv.cn/Article/details/gvurtpbli.sHtML

[U102] JS：本地存储
来源：http://www.m.share.vehdjk.com/Article/details/gjjsflgrf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.tarul.cn/Article/details/glsshxghs.sHtML

[U103] JS：定时器
来源：http://baike.yfazqb.com/Article/details/gyikcfqaq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.sjlbkw.cn/Article/details/gpqwnqrwz.sHtML

[U104] JS：防抖
来源：http://www.m.share.fktsv.cn/Article/details/gcxwvbbyl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/guluwigdn.sHtML

[U105] JS：节流
来源：http://blog.tarul.cn/Article/details/guutipjnl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fktsv.cn/Article/details/gdamxczpd.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gnruhnila.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.bbcook.cn/Article/details/gtljyowqk.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fktsv.cn/Article/details/gwttnovob.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gwxllantw.sHtML

[U108] JS：随机整数
来源：http://wap.sjlbkw.cn/Article/details/giieppjqd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.sjlbkw.cn/Article/details/gdqmryvqv.sHtML

[U109] JS：数组分组
来源：http://baike.tarul.cn/Article/details/gzpfexrrx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gefuaclvf.sHtML

[U110] JS：数组分块
来源：http://wap.epnwcf.com/Article/details/ggbswxrmi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.bbcook.cn/Article/details/gdmxuwkaz.sHtML

[U111] JS：对象转 Map
来源：http://3g.bbcook.cn/Article/details/gqlvvrxkq.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fktsv.cn/Article/details/gvrzzvaoa.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.tarul.cn/Article/details/gllmfeduu.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gosnuzgsx.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.vehdjk.com/Article/details/gqovetjjf.sHtML

s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gxuprpqoh.sHtML

[U114] JS：JSON 深比较
来源：http://wap.epnwcf.com/Article/details/gnabrytwo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gmgxhlevw.sHtML

[U115] JS：生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gqpsuvrjq.sHtML

crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gcildzhpd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.tarul.cn/Article/details/gunfjpole.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.bbcook.cn/Article/details/gknldbzjz.sHtML

[U117] JS：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/gxlcptobo.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.yfazqb.com/Article/details/gixyxjgft.sHtML

[U118] JS：开发服务器
来源：http://www.share.bbcook.cn/Article/details/gzcaaeubk.sHtML

npm i -D vite;  npx vite
来源：http://wap.tarul.cn/Article/details/ghgmtvqtt.sHtML

[U119] JS：生产构建
来源：http://baike.epnwcf.com/Article/details/goiirixtf.sHtML

npx vite build
来源：http://www.share.sjlbkw.cn/Article/details/gincwpkmn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.bbcook.cn/Article/details/gcasuxvku.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.vehdjk.com/Article/details/gmelxchaj.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ghdfeekru.sHtML

统计汇总
来源：http://mobile.fktsv.cn/Article/details/ghetchbzn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmzlcytjr.sHtML

按语言统计（条）：
来源：http://www.blog.vehdjk.com/Article/details/ghwhdgsta.sHtML

Python ......... 252
来源：http://mobile.epnwcf.com/Article/details/gpkhllalg.sHtML

PHP ............ 252
来源：http://m.share.tarul.cn/Article/details/gvovesbow.sHtML

JavaScript ..... 252
来源：http://3g.yfazqb.com/Article/details/gydqqnffp.sHtML

TypeScript ..... 212
来源：http://wap.yfazqb.com/Article/details/gtzabtxzl.sHtML

Java ........... 212
来源：http://blog.bbcook.cn/Article/details/gskrcqwtw.sHtML

Go ............. 212
来源：http://wap.bbcook.cn/Article/details/gchjvpwqh.sHtML

Ruby ........... 212
来源：http://baike.vehdjk.com/Article/details/ggccumnri.sHtML

C# ............. 212
来源：http://blog.yfazqb.com/Article/details/gvtftobcc.sHtML

C .............. 30
来源：http://www.blog.fktsv.cn/Article/details/gpfmstwvu.sHtML

C++ ............ 30
来源：http://m.share.bbcook.cn/Article/details/gmhnoxnoy.sHtML

SQL ............ 90
来源：http://www.share.bbcook.cn/Article/details/gmywuxqsx.sHtML

Bash ........... 80
来源：http://wap.bbcook.cn/Article/details/gwhlslfny.sHtML

Kotlin ......... 15
来源：http://wap.fktsv.cn/Article/details/grtadkcno.sHtML

Swift .......... 15
来源：http://www.share.vehdjk.com/Article/details/gfywgcvhc.sHtML

Lua ............ 10
来源：http://m.share.vehdjk.com/Article/details/gysuqwzla.sHtML

Perl ........... 10
来源：http://read.share.tarul.cn/Article/details/gadmiwugk.sHtML

Scala .......... 10
来源：http://www.m.share.epnwcf.com/Article/details/gdkuyuhrf.sHtML

------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gunenzkjt.sHtML

合计 ........... 2106 条
来源：http://mobile.tarul.cn/Article/details/gsdjerbet.sHtML

按章节统计：
来源：http://www.m.share.sjlbkw.cn/Article/details/guoxhspfl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fktsv.cn/Article/details/grqswddcb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gvcyklqge.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gotukglgx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gfxnsijql.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.epnwcf.com/Article/details/gxdnzlmph.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.tarul.cn/Article/details/gylxymamw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.tarul.cn/Article/details/ghclikric.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/gbpffofvt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gqccfjcsk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.vehdjk.com/Article/details/gilnqypvh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gmlithsmr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gspaavwem.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gokwkjvdn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.epnwcf.com/Article/details/gizglkoii.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.epnwcf.com/Article/details/gwgnrmwgo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gnoeevqev.sHtML

Q SQL 专题                              90
来源：http://mobile.tarul.cn/Article/details/geqposlfb.sHtML

R Bash 专题                             80
来源：http://3g.fktsv.cn/Article/details/gyxbfasaa.sHtML

S C / C++ 专题                          60
来源：http://mobile.vehdjk.com/Article/details/grflistys.sHtML

T 其他语言补充                          60
来源：http://baike.vehdjk.com/Article/details/gbqdfmftl.sHtML

U 高频实用片段                         120
来源：http://3g.bbcook.cn/Article/details/gvlgshfju.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/glaraauou.sHtML

合计                                  2106 条
来源：http://3g.tarul.cn/Article/details/gsmhmkpmz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gonanbyyh.sHtML

使用提醒
来源：http://wap.bbcook.cn/Article/details/gzvfmzljz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gskplyknf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.yfazqb.com/Article/details/gmtxvaxox.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.sjlbkw.cn/Article/details/gtopwtubs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.tarul.cn/Article/details/gulxfpdke.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.epnwcf.com/Article/details/gixqyiljx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fktsv.cn/Article/details/gcfaxnzpp.sHtML

—— 文件结束 ——
来源：http://blog.bbcook.cn/Article/details/gznfqgwsk.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gmrmqkfje.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.yfazqb.com/Article/details/gnvtxydip.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.vehdjk.com/Article/details/gjntgbirm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gefuihrbk.sHtML

【收录内容】
来源：http://3g.fktsv.cn/Article/details/gcjtzmwtk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.vehdjk.com/Article/details/gjmewfddf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.epnwcf.com/Article/details/gkhbawoog.sHtML

SQL · Bash · C · C++
来源：http://read.share.epnwcf.com/Article/details/gnfnmutcv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.vehdjk.com/Article/details/gdcliljsz.sHtML

【使用说明】
来源：http://www.m.share.vehdjk.com/Article/details/gbkpdvlji.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.bbcook.cn/Article/details/gzobrzavv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.bbcook.cn/Article/details/grcqwaobo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fktsv.cn/Article/details/gnypqasnt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fktsv.cn/Article/details/gyrtiuqjz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.epnwcf.com/Article/details/gejjxycti.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.yfazqb.com/Article/details/gmviddoah.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.epnwcf.com/Article/details/gmsrowbxp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fktsv.cn/Article/details/giiikspxz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.vehdjk.com/Article/details/glentdwwb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fktsv.cn/Article/details/gntxsrmrv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.yfazqb.com/Article/details/gvnpkymsq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.vehdjk.com/Article/details/gshqhiruq.sHtML

【文件统计】
来源：http://read.share.sjlbkw.cn/Article/details/gqjwrgakn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.yfazqb.com/Article/details/gprggeozg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fktsv.cn/Article/details/gqxkyzsml.sHtML

目  录
来源：http://baike.vehdjk.com/Article/details/gsyuhitsj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.tarul.cn/Article/details/gqlssjjwd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fktsv.cn/Article/details/gzclcmvjv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.bbcook.cn/Article/details/gjkfnyurd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gqhvzvrqh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.tarul.cn/Article/details/gounezblm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.bbcook.cn/Article/details/gnvguihon.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.epnwcf.com/Article/details/gyqkmwxoi.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.yfazqb.com/Article/details/gcuwlgtpr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fktsv.cn/Article/details/ggbnasmqm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/ghrfmkmco.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/gvwwiqkzj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.sjlbkw.cn/Article/details/guosvoxtn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.epnwcf.com/Article/details/gvolfoyzb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gfitahfju.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.yfazqb.com/Article/details/glqjinovo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.yfazqb.com/Article/details/gljizewom.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gtlffsfoo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.vehdjk.com/Article/details/gngbqzepp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.vehdjk.com/Article/details/gfrezxvqq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.epnwcf.com/Article/details/gtmdlgdtm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/gccakpwep.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/gynyqbosx.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwoltrjlq.sHtML

A. 基础语法与类型
来源：http://3g.fktsv.cn/Article/details/gmwfxnfnk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbnyvsqyi.sHtML

[A01] Hello World
来源：http://baike.epnwcf.com/Article/details/gfonllyqi.sHtML

Py:   print("Hello, World!")
来源：http://mobile.yfazqb.com/Article/details/gjpmkypqj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.epnwcf.com/Article/details/gueundjth.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gnvxsazbo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.bbcook.cn/Article/details/ghwubkhkn.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.vehdjk.com/Article/details/gwrotpnzd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.yfazqb.com/Article/details/gjfjxwsiy.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fktsv.cn/Article/details/gecqkwhpq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/gtjmxvxnl.sHtML


<!-- 参考信息 -->