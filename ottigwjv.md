代发 wailian999

[T47] Perl：正则捕获
来源：http://adl.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wet.zhaomingkeji.xyz

[T48] Perl：正则替换
来源：http://hdu.ppjwa.cn

$s =~ s/old/new/g;
来源：http://ejl.sjlbkw.cn

[T49] Perl：函数
来源：http://zgn.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yjn.tarul.cn

[T50] Perl：逐行读文件
来源：http://nrp.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fyv.yj20258.top

while (my $line = <$fh>) { print $line; }
来源：http://wsh.vqdsnc.cn

[T51] Scala：Hello World
来源：http://fcr.ehwqpu.com

println("Hello")
来源：http://sqb.chenlongwang.top

[T52] Scala：变量
来源：http://cpd.wangshuangyany.cn

val a = 1;  var b = 2
来源：http://iuh.cashguo.top

[T53] Scala：字符串插值
来源：http://lsr.hywenlv.cn

s"值: $b"
来源：http://dui.aizwys.cn

[T54] Scala：集合映射
来源：http://wvb.cucudq.cn

List(1, 2, 3).map(_ * 2)
来源：http://qti.shanyushiyangtech.top

[T55] Scala：集合过滤
来源：http://zqp.zhoulong.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://jro.hywenlv.cn

[T56] Scala：样例类
来源：http://tgf.ydjk.org.cn

case class User(name: String, age: Int)
来源：http://bxp.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://ggg.shanyushiyangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://din.shanyushiyangkeji.top

[T58] Scala：函数定义
来源：http://ihy.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://tvu.tianlin.xyz

[T59] Scala：循环
来源：http://fpm.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://rdi.ppjwa.cn

[T60] Scala：折叠
来源：http://hli.yanxiufei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://riv.iojbl.cn

================================================================================
来源：http://qlw.jinyuanbaomall.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kck.hcnkem.com

================================================================================
来源：http://zfh.nanxinkj.top

[U01] Py：创建虚拟环境
来源：http://ayr.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://yce.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://wsg.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uhg.0kj1m.cn

[U03] Py：加载 .env 配置
来源：http://ejz.52xcode.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hfi.sufxvd.cn

[U04] Py：变量调试打印
来源：http://fow.cheryme.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zjh.yfazqb.com

[U05] Py：列表去重且保序
来源：http://nsj.nanxinkj.top

list(dict.fromkeys(arr))
来源：http://btv.shuidangran.top

[U06] Py：合并两个字典
来源：http://zof.zhengqikj.top

{**a, **b}
来源：http://vgk.xuanzx.com

[U07] Py：反转字典键值
来源：http://dgn.smart0.xyz

{v: k for k, v in d.items()}
来源：http://kjk.aizwys.cn

[U08] Py：展平二维列表
来源：http://stx.cheryme.top

[y for x in nested for y in x]
来源：http://rly.jlsjyb.cn

[U09] Py：字典取最大值的键
来源：http://dko.zycfv.cn

max(d, key=d.get)
来源：http://jut.zdqjudy.top

[U10] Py：按值排序字典
来源：http://drf.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qxv.cashguo.top

[U11] Py：生成器表达式
来源：http://ccd.sjlbkw.cn

(x * 2 for x in arr)
来源：http://awp.chenjidiqi.icu

[U12] Py：取出现最多的 3 个元素
来源：http://zep.zdbjq.cn

Counter(arr).most_common(3)
来源：http://ipw.xziqi.cn

[U13] Py：固定长度队列
来源：http://ihs.fengsongda.top

deque(maxlen=10)
来源：http://vyj.52xcode.cn

[U14] Py：分组收集到列表
来源：http://ydm.shzxlz.cn

defaultdict(list)
来源：http://mug.yanxiufei.cn

[U15] Py：高精度计时
来源：http://rlv.xingfuxueyuan.xyz

t = time.perf_counter()
来源：http://rpf.tianlin.xyz

[U16] Py：命令行参数解析
来源：http://sgv.guannengcc.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kzp.tarul.cn

[U17] Py：初始化日志
来源：http://tmt.jinghuilouyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://pvm.jqgufenzy.top

[U18] Py：预编译正则
来源：http://jth.chenjidiqi.icu

pat = re.compile(r"\d+")
来源：http://lji.xylfe.cn

[U19] Py：正则替换带回调
来源：http://fss.nanxinkj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wtl.yuanzhike.top

[U20] Py：缓存函数结果
来源：http://pkr.sweek.top

@functools.lru_cache(maxsize=None)
来源：http://cds.nanxuanxn.top

[U21] Py：自定义上下文管理器
来源：http://yuk.jqgfzy.top

@contextlib.contextmanager
来源：http://amt.shzxlz.cn

[U22] Py：矩阵转置
来源：http://vjz.c1oappe.top

list(zip(*m))
来源：http://rwh.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://pea.guannengcc.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ban.yj20258.top

[U24] Py：路径操作
来源：http://jmj.iojbl.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uyn.fengsongda.top

[U25] Py：CSV 按字典读
来源：http://fzq.nanxuanxn.top

csv.DictReader(f)
来源：http://gcf.zhongyouzk.top

[U26] Py：并发下载
来源：http://zpc.xuanzx.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blw.fanxiaobao.xyz

[U27] Py：异步 HTTP
来源：http://hka.ywan-chungtsiang.top

aiohttp.ClientSession() 配合 async with
来源：http://zqr.zhiwuduotai.top

[U28] Py：类型别名
来源：http://puu.jinghuilouyu.cn

UserId = int
来源：http://qri.jinqigfzy.top

[U29] Py：属性校验
来源：http://icl.guowangkeji.top

@property 与 @x.setter 配合
来源：http://ipb.vqdsnc.cn

[U30] Py：数据类
来源：http://pjo.yfazqb.com

@dataclass(slots=True)
来源：http://vqq.c1oappe.top

[U31] Py：单测
来源：http://ybf.nwbrower.top

python -m pytest -q
来源：http://jnl.nwbrower.top

[U32] Py：代码格式化
来源：http://vwc.pengpengdd.cyou

ruff format . && ruff check --fix .
来源：http://acs.gaohongyu789.top

[U33] Py：打包发布
来源：http://cpm.chenzaomai.com

python -m build  （依赖 pyproject.toml）
来源：http://tad.shzxlz.cn

[U34] Py：判断编码
来源：http://jfv.yuanzhike.top

chardet.detect(raw)
来源：http://iwx.yongpay.top

[U35] Py：发送邮件
来源：http://paz.vqdsnc.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://awg.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://pwn.xuetiantiany.cn

schedule.every(10).minutes.do(job)
来源：http://riv.quarkkingdee.top

[U37] Py：读写 Excel
来源：http://blc.chenjidiqi.icu

pandas.read_excel / DataFrame.to_excel
来源：http://wby.mhx1999.top

[U38] Py：获取脚本所在目录
来源：http://ypb.gaohongyu789.top

Path(__file__).resolve().parent
来源：http://dph.zdbjq.cn

[U39] Py：判断是否在交互环境
来源：http://unh.nwbrower.top

sys.stdout.isatty()
来源：http://ytd.yuanzhike.top

[U40] Py：打印到标准错误
来源：http://mvw.epnwcf.com

print("err", file=sys.stderr)
来源：http://yjv.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://yfq.dianchejie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jnu.sweek.top

[U42] PHP：PSR-4 自动加载
来源：http://njl.vehdjk.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://elb.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://nvj.pycfn.com

namespace App\Http;
来源：http://xne.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://jrw.xylfe.cn

declare(strict_types=1);
来源：http://oxz.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://kza.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wmu.kuanghao11.cn

[U46] PHP：可空类型
来源：http://oaj.zycfv.cn

?string $name = null
来源：http://dla.gzhubu.top

[U47] PHP：联合类型
来源：http://dni.zhongyouzk.top

int|string $id
来源：http://bdm.jinyuanbaomall.cn

[U48] PHP：纯枚举
来源：http://gjd.hfpthk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gga.yj20258.top

[U49] PHP：只读属性
来源：http://phd.cdnleiting.top

public readonly string $name
来源：http://mst.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://boq.hammf.cn

public function __construct(private int $id) {}
来源：http://kzq.fanxiaobao.xyz

[U51] PHP：数组解构
来源：http://hov.uphjek.com

[$a, $b] = $arr;
来源：http://ntu.iojbl.cn

[U52] PHP：箭头函数
来源：http://alt.iojbl.cn

$double = fn($x) => $x * 2;
来源：http://iuh.fktsv.cn

[U53] PHP：空合并运算符
来源：http://reu.hesvh.cn

$v = $a ?? $b ?? "default";
来源：http://hoe.redwolf501.top

[U54] PHP：空安全调用
来源：http://gah.daxiang520.top

$obj?->method()
来源：http://ulk.tianlin.xyz

[U55] PHP：match 表达式
来源：http://oub.bjfxy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tvu.52xcode.cn

[U56] PHP：命名参数
来源：http://laf.xinyue.icu

f(a: 1, b: 2)
来源：http://qby.epnwcf.com

[U57] PHP：字符串插值
来源：http://vku.hongshengwenyu.top

"值: {$a}"
来源：http://jhd.jyoumei.cn

[U58] PHP：数组三件套
来源：http://xyw.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ekt.gaohongyu789.top

[U59] PHP：自定义排序
来源：http://itx.sjlbkw.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iuf.dashuyun.cn

[U60] PHP：JSON 编解码
来源：http://vdc.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bov.yfazqb.com

[U61] PHP：正则
来源：http://fdk.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xfi.wangshuangyany.cn

[U62] PHP：日期对象
来源：http://oat.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eoe.yuanzhike.top

[U63] PHP：文件读写
来源：http://rpg.sweek.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lpp.cheryme.top

[U64] PHP：目录遍历
来源：http://iul.hnxiangtu.top

glob("dir/*.php");  scandir("dir");
来源：http://wxh.ppjwa.cn

[U65] PHP：会话
来源：http://bbr.shuidangran.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kak.zhiwuduotai.top

[U66] PHP：设置 Cookie
来源：http://xsv.xingfuxueyuan.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zqw.yj20258888.top

[U67] PHP：处理文件上传
来源：http://fkb.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yvn.zdqjudy.top

[U68] PHP：PDO 连接
来源：http://qgh.guowangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iwi.pengpengdd.cyou

[U69] PHP：PDO 预处理
来源：http://dgw.yj202588.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jqg.wangdashe.top

[U70] PHP：PDO 事务
来源：http://ycr.jinqigfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kdc.guannengcc.top

[U71] PHP：抛出异常
来源：http://esz.zhoulong.xyz

throw new RuntimeException("失败", 500);
来源：http://xdr.tanke756.top

[U72] PHP：写错误日志
来源：http://kmr.dianchejie.cn

error_log("失败: " . $e->getMessage());
来源：http://igz.xuetiantiany.cn

[U73] PHP：读取 ini 配置
来源：http://iwd.aibaodan.cn

parse_ini_file("config.ini", true)
来源：http://cdl.cucudq.cn

[U74] PHP：读取环境变量
来源：http://xgs.yueranfly.top

getenv("APP_ENV") ?: "production"
来源：http://ndn.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://nxf.hywenlv.cn

composer require psr/container
来源：http://qpt.iojbl.cn

[U76] PHP：简单路由
来源：http://hwy.havefunace.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ygq.yangfankeji.com

[U77] PHP：模板渲染
来源：http://fcq.jyoumei.cn

composer require twig/twig
来源：http://oto.cdnleiting.top

[U78] PHP：单元测试
来源：http://kae.wangshuangyany.cn

composer require --dev phpunit/phpunit
来源：http://ffk.ctjpmb.com

[U79] PHP：静态分析
来源：http://mxw.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://wbp.vqdsnc.cn

[U80] PHP：代码规范修复
来源：http://gya.xuetiantiany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kxt.tian-w.cn

[U81] JS：初始化项目
来源：http://czi.hfpthk.cn

npm init -y;  npm i express
来源：http://eah.ehwqpu.com

[U82] JS：package.json 脚本
来源：http://dku.tarul.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uyc.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://dax.meibo888.top

export const a = 1;  import { a } from "./m.js";
来源：http://iql.bbcook.cn

[U84] JS：CommonJS 写法
来源：http://hld.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qsc.zhengqikj.top

[U85] JS：可选链
来源：http://dne.cucudq.cn

a?.b?.c
来源：http://meu.wangdashe.top

[U86] JS：空值合并
来源：http://uah.cdnleiting.top

a ?? b
来源：http://roj.daxiang520.top

[U87] JS：解构默认值
来源：http://lka.shanyushiyangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://qdc.sysykeji.top

[U88] JS：对象展开合并
来源：http://dim.9152youxi.cn

{ ...a, ...b }
来源：http://vif.cheryme.top

[U89] JS：数组去重
来源：http://ujp.uphjek.com

[...new Set(arr)]
来源：http://bkq.cdnleiting.top

[U90] JS：数字数组排序
来源：http://rst.zdqjudy.top

[...arr].sort((a, b) => a - b)
来源：http://fgj.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://vjg.cheryme.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vts.jqgufenzy.top

[U92] JS：深拷贝
来源：http://urs.0kj1m.cn

structuredClone(obj)
来源：http://hgh.meibo888.top

[U93] JS：模板字符串
来源：http://rhs.aibaodan.cn

`共 ${n} 条`
来源：http://awz.9152youxi.cn

[U94] JS：箭头函数
来源：http://swv.tianlin.xyz

const double = x => x * 2;
来源：http://ofx.ydzc1.top

[U95] JS：Promise 包装
来源：http://ryw.cqqwz.cn

new Promise((resolve, reject) => {})
来源：http://cht.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://fob.yuxming.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wrn.zhiwuduotai.top

[U97] JS：并发请求
来源：http://gaq.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rkl.shangyingyoupin.top

[U98] JS：fetch 带 JSON
来源：http://bvj.gotoacloud.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yzs.ydjk.org.cn

[U99] JS：事件监听
来源：http://sev.chenlongwang.top

el.addEventListener("click", e => {})
来源：http://wcc.birdmap.top

[U100] JS：DOM 查询
来源：http://cyq.jinghuilouyu.cn

document.querySelector(".item")
来源：http://duq.jinqigufen.top

[U101] JS：classList 操作
来源：http://dlq.nanxuanxn.top

el.classList.toggle("active")
来源：http://umw.iojbl.cn

[U102] JS：本地存储
来源：http://eux.nanxuanxn.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://oor.dashuyun.cn

[U103] JS：定时器
来源：http://xrv.aizwys.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kxt.zdqjudy.top

[U104] JS：防抖
来源：http://vyu.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zsh.sysykeji.top

[U105] JS：节流
来源：http://tro.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zom.yonumen.top

[U106] JS：日期格式化
来源：http://jau.yj202588.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ctr.hysaishi.cn

[U107] JS：数字千分位
来源：http://sdf.sjlbkw.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://com.gogol.net.cn

[U108] JS：随机整数
来源：http://ing.guannengcc.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jhx.zhongyouzk.top

[U109] JS：数组分组
来源：http://bfb.hywenlv.cn

Object.groupBy(arr, x => x.type)
来源：http://gsj.zhengqikj.top

[U110] JS：数组分块
来源：http://gkt.sxryk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iri.xylfe.cn

[U111] JS：对象转 Map
来源：http://ymn.yfazqb.com

new Map(Object.entries(obj))
来源：http://faj.bbcook.cn

[U112] JS：字符串补位
来源：http://aar.meibo888.top

"7".padStart(3, "0")
来源：http://tpe.fktsv.cn

[U113] JS：正则替换全部
来源：http://mxg.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://ytk.hywenlv.cn

[U114] JS：JSON 深比较
来源：http://hhz.hesvh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cgt.fanxiaobao.xyz

[U115] JS：生成 UUID
来源：http://ffz.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://voz.yonumen.top

[U116] JS：类型检查（JSDoc）
来源：http://qaq.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://wdo.9152youxi.cn

[U117] JS：单元测试
来源：http://kfj.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://ecp.cashguo.top

[U118] JS：开发服务器
来源：http://yof.feifeiyinyue.top

npm i -D vite;  npx vite
来源：http://jeu.hysaishi.cn

[U119] JS：生产构建
来源：http://oop.kuanghao11.cn

npx vite build
来源：http://jci.zhengqikj.top

[U120] JS：读取环境变量（Vite）
来源：http://kvr.jinqigufen.top

import.meta.env.VITE_API_URL
来源：http://gxo.hfpthk.cn

================================================================================
来源：http://ehl.mhx1999.top

统计汇总
来源：http://qos.redwolf501.top

================================================================================
来源：http://tgm.hongshengwenyu.top

按语言统计（条）：
来源：http://obr.sysykeji.top

Python ......... 252
来源：http://iin.ctjpmb.com

PHP ............ 252
来源：http://oms.ydzc1.top

JavaScript ..... 252
来源：http://yux.jlsjyb.cn

TypeScript ..... 212
来源：http://bkc.wangdashe.top

Java ........... 212
来源：http://sco.shuidangran.top

Go ............. 212
来源：http://ewm.sysykeji.top

Ruby ........... 212
来源：http://rbw.meibo888.top

C# ............. 212
来源：http://upo.xuanzx.com

C .............. 30
来源：http://htb.sufxvd.cn

C++ ............ 30
来源：http://tfa.fehbvm.com

SQL ............ 90
来源：http://ggd.quarkkingdee.top

Bash ........... 80
来源：http://unz.yanxiufei.cn

Kotlin ......... 15
来源：http://vod.quarkkingdee.top

Swift .......... 15
来源：http://nxx.jianghu66.top

Lua ............ 10
来源：http://ilc.iojbl.cn

Perl ........... 10
来源：http://pzh.nwbrower.top

Scala .......... 10
来源：http://fgo.hnxiangtu.top

------------------------------------
来源：http://uyk.tian-w.cn

合计 ........... 2106 条
来源：http://bzt.jinqigfzy.top

按章节统计：
来源：http://equ.ydzc1.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://txo.gogol.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://avv.gaohongyu789.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ypu.xinyue.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zyk.aibaodan.cn


<!-- 参考信息 -->