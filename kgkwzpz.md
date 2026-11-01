代发 wailian999

[U33] Py：打包发布
来源：http://wap.tarul.cn/Article/details/ghmuzgtip.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.vehdjk.com/Article/details/gkuarrwqb.sHtML

[U34] Py：判断编码
来源：http://3g.bbcook.cn/Article/details/gnipcecno.sHtML

chardet.detect(raw)
来源：http://m.share.vehdjk.com/Article/details/gfjahllcj.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.vehdjk.com/Article/details/gxffycata.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fktsv.cn/Article/details/grtuorcyi.sHtML

[U36] Py：定时任务
来源：http://www.share.sjlbkw.cn/Article/details/gvarlqzsg.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fktsv.cn/Article/details/gblbovdyf.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.sjlbkw.cn/Article/details/grnyxabne.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.yfazqb.com/Article/details/gwmqixmdl.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.sjlbkw.cn/Article/details/geqqztxyy.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.tarul.cn/Article/details/gxvnbhypl.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.sjlbkw.cn/Article/details/gnxsqroym.sHtML

sys.stdout.isatty()
来源：http://read.share.tarul.cn/Article/details/geadkbemn.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.sjlbkw.cn/Article/details/gifvedama.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/gemhhfiaz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.epnwcf.com/Article/details/gpyaeiaag.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.yfazqb.com/Article/details/gujanlbtv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fktsv.cn/Article/details/gonvyodhb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.epnwcf.com/Article/details/glchymtxc.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.yfazqb.com/Article/details/gtydsmjjr.sHtML

namespace App\Http;
来源：http://www.share.yfazqb.com/Article/details/gqoviybwj.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.yfazqb.com/Article/details/gzlnlsdbq.sHtML

declare(strict_types=1);
来源：http://mobile.epnwcf.com/Article/details/gftkjuode.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.tarul.cn/Article/details/gzwsvhmey.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gqsrmlowt.sHtML

[U46] PHP：可空类型
来源：http://mobile.bbcook.cn/Article/details/gyuucxwvn.sHtML

?string $name = null
来源：http://www.blog.fktsv.cn/Article/details/gapofqnpw.sHtML

[U47] PHP：联合类型
来源：http://baike.sjlbkw.cn/Article/details/gzcsplmur.sHtML

int|string $id
来源：http://3g.yfazqb.com/Article/details/gczmproch.sHtML

[U48] PHP：纯枚举
来源：http://baike.yfazqb.com/Article/details/gglermhfp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.tarul.cn/Article/details/giogqqanf.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.epnwcf.com/Article/details/gcjdyuuvg.sHtML

public readonly string $name
来源：http://www.m.share.bbcook.cn/Article/details/gvxfdiazj.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.yfazqb.com/Article/details/gkvbzbcgs.sHtML

public function __construct(private int $id) {}
来源：http://m.share.tarul.cn/Article/details/gyornlggg.sHtML

[U51] PHP：数组解构
来源：http://m.share.tarul.cn/Article/details/gkduzndbs.sHtML

[$a, $b] = $arr;
来源：http://m.share.tarul.cn/Article/details/ghqgprlgm.sHtML

[U52] PHP：箭头函数
来源：http://3g.bbcook.cn/Article/details/gyebzaucy.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.tarul.cn/Article/details/gfjreznmg.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.bbcook.cn/Article/details/gpxwanpuo.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.sjlbkw.cn/Article/details/givnqnzio.sHtML

[U54] PHP：空安全调用
来源：http://wap.bbcook.cn/Article/details/gelnlaqbi.sHtML

$obj?->method()
来源：http://www.m.share.vehdjk.com/Article/details/guzwcdvyz.sHtML

[U55] PHP：match 表达式
来源：http://3g.sjlbkw.cn/Article/details/gfrbvhlue.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.yfazqb.com/Article/details/gwozugdzx.sHtML

[U56] PHP：命名参数
来源：http://blog.sjlbkw.cn/Article/details/gzjukpjdn.sHtML

f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gcfpjibxq.sHtML

[U57] PHP：字符串插值
来源：http://baike.epnwcf.com/Article/details/gzkvxhjau.sHtML

"值: {$a}"
来源：http://baike.sjlbkw.cn/Article/details/gqfwbvhmq.sHtML

[U58] PHP：数组三件套
来源：http://wap.yfazqb.com/Article/details/gqquxbxfa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.sjlbkw.cn/Article/details/gwtatmljj.sHtML

[U59] PHP：自定义排序
来源：http://3g.epnwcf.com/Article/details/glilyknum.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/gkglsjevr.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fktsv.cn/Article/details/gyftuuhbm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.vehdjk.com/Article/details/gywqolodg.sHtML

[U61] PHP：正则
来源：http://read.share.tarul.cn/Article/details/grqufpbaw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.yfazqb.com/Article/details/gqgefiazh.sHtML

[U62] PHP：日期对象
来源：http://blog.yfazqb.com/Article/details/gklgsmshr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.vehdjk.com/Article/details/gqbbvimiu.sHtML

[U63] PHP：文件读写
来源：http://3g.bbcook.cn/Article/details/gsuobdkdk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.vehdjk.com/Article/details/gvlecnanz.sHtML

[U64] PHP：目录遍历
来源：http://wap.fktsv.cn/Article/details/gbzenwopi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.epnwcf.com/Article/details/gzlnuqaeb.sHtML

[U65] PHP：会话
来源：http://baike.yfazqb.com/Article/details/gwfacznjc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgjmbqzl.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.vehdjk.com/Article/details/gyjqhabfa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.vehdjk.com/Article/details/ghkfptpkk.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.yfazqb.com/Article/details/gmhgeqkja.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.tarul.cn/Article/details/glvzyhkod.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fktsv.cn/Article/details/gbugcznxl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.bbcook.cn/Article/details/gmctjikaa.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.tarul.cn/Article/details/gepnjmqbl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.vehdjk.com/Article/details/gpddogupg.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.yfazqb.com/Article/details/gobqhkkzp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fktsv.cn/Article/details/gnivwcajb.sHtML

[U71] PHP：抛出异常
来源：http://www.share.yfazqb.com/Article/details/gkiggdyds.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gjofbtrib.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.yfazqb.com/Article/details/gcqjqwmww.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.tarul.cn/Article/details/gkcqhuxjd.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fktsv.cn/Article/details/gyzgpkjak.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.bbcook.cn/Article/details/ggayzdoiz.sHtML

[U74] PHP：读取环境变量
来源：http://3g.bbcook.cn/Article/details/gkmmuowwc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.epnwcf.com/Article/details/gfpfvrvkz.sHtML

[U75] PHP：依赖注入
来源：http://m.share.tarul.cn/Article/details/gacxbrbva.sHtML

composer require psr/container
来源：http://wap.sjlbkw.cn/Article/details/gjwwzxkot.sHtML

[U76] PHP：简单路由
来源：http://m.share.vehdjk.com/Article/details/gvsqoyjnl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwpokedb.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fktsv.cn/Article/details/geomfrdvf.sHtML

composer require twig/twig
来源：http://read.share.vehdjk.com/Article/details/gidfqbvxm.sHtML

[U78] PHP：单元测试
来源：http://wap.vehdjk.com/Article/details/gshvwnjzc.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.yfazqb.com/Article/details/gvkcxzfxb.sHtML

[U79] PHP：静态分析
来源：http://www.blog.sjlbkw.cn/Article/details/gdtxpargb.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.epnwcf.com/Article/details/gqgdtbicb.sHtML

[U80] PHP：代码规范修复
来源：http://3g.tarul.cn/Article/details/gtvkuwohp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fktsv.cn/Article/details/glwulyxmb.sHtML

[U81] JS：初始化项目
来源：http://www.blog.tarul.cn/Article/details/gqxtziksr.sHtML

npm init -y;  npm i express
来源：http://read.share.epnwcf.com/Article/details/gdwaldngr.sHtML

[U82] JS：package.json 脚本
来源：http://wap.yfazqb.com/Article/details/gokqpuyha.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.yfazqb.com/Article/details/goeztbikr.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fktsv.cn/Article/details/gszokiehj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fktsv.cn/Article/details/gradwvxog.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.yfazqb.com/Article/details/gqkclwgsd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.bbcook.cn/Article/details/gvnfwnoha.sHtML

[U85] JS：可选链
来源：http://baike.yfazqb.com/Article/details/gxddopnuh.sHtML

a?.b?.c
来源：http://read.share.yfazqb.com/Article/details/gytdoblhx.sHtML

[U86] JS：空值合并
来源：http://baike.fktsv.cn/Article/details/gwdatasor.sHtML

a ?? b
来源：http://baike.fktsv.cn/Article/details/getostzjx.sHtML

[U87] JS：解构默认值
来源：http://m.share.vehdjk.com/Article/details/gqmrwesug.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/gkyoyvyne.sHtML

[U88] JS：对象展开合并
来源：http://m.share.yfazqb.com/Article/details/guhcyczuy.sHtML

{ ...a, ...b }
来源：http://m.share.tarul.cn/Article/details/gjhcystwv.sHtML

[U89] JS：数组去重
来源：http://m.share.yfazqb.com/Article/details/gdftekqsy.sHtML

[...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gdjkbnsas.sHtML

[U90] JS：数字数组排序
来源：http://m.share.vehdjk.com/Article/details/gwzetikrp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/glfmtbjso.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.yfazqb.com/Article/details/gdqbkbxwl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.epnwcf.com/Article/details/gycunodou.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gbccaqvvz.sHtML

structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gtlnfcxvd.sHtML

[U93] JS：模板字符串
来源：http://www.share.yfazqb.com/Article/details/grhlilkap.sHtML

`共 ${n} 条`
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwirpzxe.sHtML

[U94] JS：箭头函数
来源：http://blog.epnwcf.com/Article/details/gpagqjsdx.sHtML

const double = x => x * 2;
来源：http://wap.epnwcf.com/Article/details/gozlbywsi.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.vehdjk.com/Article/details/gtlvzkqpt.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.yfazqb.com/Article/details/gfvzrmspt.sHtML

[U96] JS：async/await 与异常
来源：http://wap.vehdjk.com/Article/details/gxfrmdcwj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gxpyzxiaj.sHtML

[U97] JS：并发请求
来源：http://blog.yfazqb.com/Article/details/gtxdwmvwh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/ghoedthcn.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.sjlbkw.cn/Article/details/gdsilwylj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.tarul.cn/Article/details/gbajchxvb.sHtML

[U99] JS：事件监听
来源：http://read.share.vehdjk.com/Article/details/gvdbpeohs.sHtML

el.addEventListener("click", e => {})
来源：http://wap.vehdjk.com/Article/details/guckknncv.sHtML

[U100] JS：DOM 查询
来源：http://mobile.vehdjk.com/Article/details/gpfzrzwiu.sHtML

document.querySelector(".item")
来源：http://mobile.yfazqb.com/Article/details/gxvipolso.sHtML

[U101] JS：classList 操作
来源：http://wap.epnwcf.com/Article/details/glwpbkbkh.sHtML

el.classList.toggle("active")
来源：http://www.m.share.bbcook.cn/Article/details/glrklswju.sHtML

[U102] JS：本地存储
来源：http://www.m.share.sjlbkw.cn/Article/details/gklsffutk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.tarul.cn/Article/details/gwupazwpd.sHtML

[U103] JS：定时器
来源：http://blog.tarul.cn/Article/details/gfusupjsr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.yfazqb.com/Article/details/guuosmosu.sHtML

[U104] JS：防抖
来源：http://www.share.sjlbkw.cn/Article/details/gnkzeaneq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gnnnvtarj.sHtML

[U105] JS：节流
来源：http://www.blog.yfazqb.com/Article/details/gomtqacge.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.yfazqb.com/Article/details/gbxwtjyoq.sHtML

[U106] JS：日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gjactiiwf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.vehdjk.com/Article/details/glsyjyawz.sHtML

[U107] JS：数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/gtiotzugx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/gnpxzgjaz.sHtML

[U108] JS：随机整数
来源：http://3g.fktsv.cn/Article/details/ghdyrcrfq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.sjlbkw.cn/Article/details/gsibxyalv.sHtML

[U109] JS：数组分组
来源：http://m.share.sjlbkw.cn/Article/details/gwuanleoc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.tarul.cn/Article/details/gajbzrrce.sHtML

[U110] JS：数组分块
来源：http://www.blog.sjlbkw.cn/Article/details/gpvyhvjac.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fktsv.cn/Article/details/grhdkapzm.sHtML

[U111] JS：对象转 Map
来源：http://mobile.tarul.cn/Article/details/gzoganxum.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/gllwfoovr.sHtML

[U112] JS：字符串补位
来源：http://read.share.vehdjk.com/Article/details/gkqdushou.sHtML

"7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gkbtukbar.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.tarul.cn/Article/details/gftwzytxa.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/goizqjvdw.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.sjlbkw.cn/Article/details/grirrwajy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gpcmfxtcr.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/gtchvogpz.sHtML

crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gyozdyanz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fktsv.cn/Article/details/gxjauqoxt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/geteqrcyd.sHtML

[U117] JS：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gfvwqzmyn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fktsv.cn/Article/details/gxezhtytq.sHtML

[U118] JS：开发服务器
来源：http://blog.tarul.cn/Article/details/gmgqdtnvp.sHtML

npm i -D vite;  npx vite
来源：http://3g.tarul.cn/Article/details/goqorswjf.sHtML

[U119] JS：生产构建
来源：http://read.share.yfazqb.com/Article/details/guiyoxcjg.sHtML

npx vite build
来源：http://www.m.share.vehdjk.com/Article/details/gavrctklc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.tarul.cn/Article/details/gepviouok.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fktsv.cn/Article/details/gynfnxhyw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzgepltyl.sHtML

统计汇总
来源：http://www.m.share.fktsv.cn/Article/details/gxznqotop.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmiabdnwa.sHtML

按语言统计（条）：
来源：http://3g.bbcook.cn/Article/details/gjehtoxnw.sHtML

Python ......... 252
来源：http://m.share.bbcook.cn/Article/details/gissptsdj.sHtML

PHP ............ 252
来源：http://m.share.bbcook.cn/Article/details/grooimjtu.sHtML

JavaScript ..... 252
来源：http://www.blog.bbcook.cn/Article/details/ggspalhod.sHtML

TypeScript ..... 212
来源：http://3g.sjlbkw.cn/Article/details/gnmnlbzej.sHtML

Java ........... 212
来源：http://www.share.epnwcf.com/Article/details/gdxivrqox.sHtML

Go ............. 212
来源：http://wap.vehdjk.com/Article/details/geyfgowpa.sHtML

Ruby ........... 212
来源：http://3g.tarul.cn/Article/details/gccuyfksb.sHtML

C# ............. 212
来源：http://m.share.yfazqb.com/Article/details/guryhavzs.sHtML

C .............. 30
来源：http://www.share.yfazqb.com/Article/details/guylmieqp.sHtML

C++ ............ 30
来源：http://www.blog.fktsv.cn/Article/details/gwuzuyyfg.sHtML

SQL ............ 90
来源：http://blog.sjlbkw.cn/Article/details/gzpnstlih.sHtML

Bash ........... 80
来源：http://blog.fktsv.cn/Article/details/gegmtpnvj.sHtML

Kotlin ......... 15
来源：http://3g.tarul.cn/Article/details/ghtpaltxu.sHtML

Swift .......... 15
来源：http://www.blog.vehdjk.com/Article/details/gubyknhdn.sHtML

Lua ............ 10
来源：http://read.share.fktsv.cn/Article/details/gtouwvbzy.sHtML

Perl ........... 10
来源：http://www.share.epnwcf.com/Article/details/gahqlcfdn.sHtML

Scala .......... 10
来源：http://m.share.tarul.cn/Article/details/gutbboqij.sHtML

------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gvesbeppp.sHtML

合计 ........... 2106 条
来源：http://read.share.vehdjk.com/Article/details/giiajcrzn.sHtML

按章节统计：
来源：http://blog.vehdjk.com/Article/details/gauxqzyck.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/geuwhdmor.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gwdzsanml.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/gkjfdqnqa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/gtctmcyav.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fktsv.cn/Article/details/gicpicfvf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.sjlbkw.cn/Article/details/gjjwqbvjz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/grfmuyczi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gybuixbna.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gpbnkyrfh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.vehdjk.com/Article/details/gpjssphzf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gggyxryof.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/grnocrrqe.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gepxhxizl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fktsv.cn/Article/details/gbsnlvelm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.tarul.cn/Article/details/ggjuvdahl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gunvhwpjd.sHtML

Q SQL 专题                              90
来源：http://www.blog.epnwcf.com/Article/details/gknbkzrfk.sHtML

R Bash 专题                             80
来源：http://3g.bbcook.cn/Article/details/gynnmvrpm.sHtML

S C / C++ 专题                          60
来源：http://mobile.vehdjk.com/Article/details/gxcjbtrae.sHtML

T 其他语言补充                          60
来源：http://baike.epnwcf.com/Article/details/gtquqelir.sHtML

U 高频实用片段                         120
来源：http://mobile.epnwcf.com/Article/details/gsirhlqsx.sHtML

------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gbdqlcbne.sHtML

合计                                  2106 条
来源：http://3g.epnwcf.com/Article/details/gruepgvwh.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/gyebhzpoq.sHtML

使用提醒
来源：http://www.blog.sjlbkw.cn/Article/details/grvlbbxkq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.tarul.cn/Article/details/glrwptkgn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.tarul.cn/Article/details/giqvdmgqt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.vehdjk.com/Article/details/gnxzjbvom.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.vehdjk.com/Article/details/gemaaudig.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.vehdjk.com/Article/details/gyvbrakqj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.sjlbkw.cn/Article/details/gisnmzmsm.sHtML

—— 文件结束 ——
来源：http://baike.bbcook.cn/Article/details/gogwjdhqo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkzpkepsv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.vehdjk.com/Article/details/gswxuuqxe.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.vehdjk.com/Article/details/gtrlxwanq.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gmfsjgdqd.sHtML

【收录内容】
来源：http://m.share.sjlbkw.cn/Article/details/gheiipsvf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.yfazqb.com/Article/details/gndsainii.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.epnwcf.com/Article/details/ggytxquiu.sHtML

SQL · Bash · C · C++
来源：http://www.share.sjlbkw.cn/Article/details/gjyspxshj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.vehdjk.com/Article/details/gqrmzdwew.sHtML

【使用说明】
来源：http://www.m.share.sjlbkw.cn/Article/details/gqelftjau.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.bbcook.cn/Article/details/gjfxcpdpb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.bbcook.cn/Article/details/gzjtwrazp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.sjlbkw.cn/Article/details/gslmdrlel.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.epnwcf.com/Article/details/ghwnnmtes.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.tarul.cn/Article/details/ghthhaczd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fktsv.cn/Article/details/gnadtvaif.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.yfazqb.com/Article/details/gyyjpgxxv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.bbcook.cn/Article/details/gbkfttggf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.tarul.cn/Article/details/gupaogrrd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.vehdjk.com/Article/details/gtoqkgawv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.sjlbkw.cn/Article/details/gtiquxetd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.yfazqb.com/Article/details/gxhgocgng.sHtML

【文件统计】
来源：http://read.share.epnwcf.com/Article/details/gdxdoawzg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.vehdjk.com/Article/details/glwozxbsh.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gvjihgufe.sHtML

目  录
来源：http://www.share.vehdjk.com/Article/details/gihezlazf.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gxownicbt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.vehdjk.com/Article/details/gouvamxhd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.sjlbkw.cn/Article/details/grordrijc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/gqxcmycfo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.bbcook.cn/Article/details/gupjauppe.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.tarul.cn/Article/details/gqwvvhjge.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.bbcook.cn/Article/details/garppivsb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.vehdjk.com/Article/details/gdtegtpjd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.vehdjk.com/Article/details/gppssvxdf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/gijrdzfka.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gltmvawgv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gccgjfhzp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/gtivwgjhp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.yfazqb.com/Article/details/gauxuclxe.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.bbcook.cn/Article/details/gqtkxqsqd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.epnwcf.com/Article/details/gzyeqicva.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/gdokveucg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fktsv.cn/Article/details/gjrorchsa.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.yfazqb.com/Article/details/gemjsydan.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.yfazqb.com/Article/details/grlbhrpxx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.vehdjk.com/Article/details/gxovkipql.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/gdhawukgf.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gihfkbpmr.sHtML

A. 基础语法与类型
来源：http://m.share.yfazqb.com/Article/details/gfjutwwct.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/govvbgwbo.sHtML

[A01] Hello World
来源：http://wap.sjlbkw.cn/Article/details/gqpvoetpx.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fktsv.cn/Article/details/gxngyljjc.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.tarul.cn/Article/details/gmscjynac.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.epnwcf.com/Article/details/gnazkmjme.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.vehdjk.com/Article/details/gvadjtzur.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fktsv.cn/Article/details/gkppgjmly.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fktsv.cn/Article/details/gmipkafbm.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.sjlbkw.cn/Article/details/gkyuohrrj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.tarul.cn/Article/details/gmtpwiynn.sHtML

[A02] 变量声明与赋值
来源：http://baike.sjlbkw.cn/Article/details/gogmhsftc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.bbcook.cn/Article/details/gbuueplvt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gidfakmky.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.yfazqb.com/Article/details/gmnkqdpne.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.epnwcf.com/Article/details/gkpnrtcfp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.vehdjk.com/Article/details/ggdbtpvdk.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.sjlbkw.cn/Article/details/gpomqjmon.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.tarul.cn/Article/details/gpnglbhdw.sHtML


<!-- 参考信息 -->