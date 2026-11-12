代发 wailian999

[T47] Perl：正则捕获
来源：http://ymr.guowangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zmv.zhengqikj.top

[T48] Perl：正则替换
来源：http://tiw.yj20258.top

$s =~ s/old/new/g;
来源：http://sbq.jlsjyb.cn

[T49] Perl：函数
来源：http://aro.gotoacloud.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://umu.ivvv.top

[T50] Perl：逐行读文件
来源：http://xnf.xziqi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://imc.tian-w.cn

while (my $line = <$fh>) { print $line; }
来源：http://hpj.dianchejie.cn

[T51] Scala：Hello World
来源：http://jcp.fanxiaobao.xyz

println("Hello")
来源：http://byu.hfpthk.cn

[T52] Scala：变量
来源：http://hdo.jinghuilouyu.cn

val a = 1;  var b = 2
来源：http://klk.jinqigufen.top

[T53] Scala：字符串插值
来源：http://twj.cdnleiting.top

s"值: $b"
来源：http://qsy.jinghuilouyu.cn

[T54] Scala：集合映射
来源：http://adh.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://fpu.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://ixn.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://jst.cheryme.top

[T56] Scala：样例类
来源：http://hfw.chenlongwang.top

case class User(name: String, age: Int)
来源：http://bxx.ydjk.org.cn

[T57] Scala：模式匹配
来源：http://ekq.guowangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ysz.aizwys.cn

[T58] Scala：函数定义
来源：http://sey.hywenlv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ghm.shanyushiyangkeji.top

[T59] Scala：循环
来源：http://rpo.mhx1999.top

for (i <- 1 to 10) println(i)
来源：http://tlg.fengsongda.top

[T60] Scala：折叠
来源：http://zmh.xylfe.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rcs.ydzc1.top

================================================================================
来源：http://ddy.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wah.nwbrower.top

================================================================================
来源：http://slv.zhongyouzk.top

[U01] Py：创建虚拟环境
来源：http://ohh.zhixingplan.top

python -m venv .venv && source .venv/bin/activate
来源：http://ocl.redwolf501.top

[U02] Py：导出 / 安装依赖
来源：http://kxc.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://izw.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://byb.cheryme.top

from dotenv import load_dotenv; load_dotenv()
来源：http://efa.meibo888.top

[U04] Py：变量调试打印
来源：http://dml.gotoacloud.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hmc.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://wmk.yueranfly.top

list(dict.fromkeys(arr))
来源：http://mqy.hammf.cn

[U06] Py：合并两个字典
来源：http://noe.jinyuanbaomall.cn

{**a, **b}
来源：http://yqu.hysaishi.cn

[U07] Py：反转字典键值
来源：http://aye.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://qvo.gzhubu.top

[U08] Py：展平二维列表
来源：http://yoy.vqdsnc.cn

[y for x in nested for y in x]
来源：http://tlp.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://pjj.birdmap.top

max(d, key=d.get)
来源：http://mgp.zycfv.cn

[U10] Py：按值排序字典
来源：http://gsr.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lrc.hesvh.cn

[U11] Py：生成器表达式
来源：http://kwe.nanxinkj.top

(x * 2 for x in arr)
来源：http://fja.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://kwy.chenzaomai.com

Counter(arr).most_common(3)
来源：http://dxa.jianghu66.top

[U13] Py：固定长度队列
来源：http://mcz.jinghuilouyu.cn

deque(maxlen=10)
来源：http://tvn.wangdashe.top

[U14] Py：分组收集到列表
来源：http://utf.tarul.cn

defaultdict(list)
来源：http://tta.cashguo.top

[U15] Py：高精度计时
来源：http://xxt.zdbjq.cn

t = time.perf_counter()
来源：http://rdf.sxryk.cn

[U16] Py：命令行参数解析
来源：http://xws.pycfn.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yjb.xingfuxueyuan.xyz

[U17] Py：初始化日志
来源：http://svl.chenlongwang.top

logging.basicConfig(level=logging.INFO)
来源：http://mir.kuanghao11.cn

[U18] Py：预编译正则
来源：http://bto.xingfuxueyuan.xyz

pat = re.compile(r"\d+")
来源：http://onb.smart0.xyz

[U19] Py：正则替换带回调
来源：http://anx.nwbrower.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kqs.hysaishi.cn

[U20] Py：缓存函数结果
来源：http://wsz.jqgfzy.top

@functools.lru_cache(maxsize=None)
来源：http://qor.tian-w.cn

[U21] Py：自定义上下文管理器
来源：http://jgc.svipenyu.cn

@contextlib.contextmanager
来源：http://ilc.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://yyd.pycfn.com

list(zip(*m))
来源：http://fbn.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://dba.vqdsnc.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lng.shzxlz.cn

[U24] Py：路径操作
来源：http://aqy.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uct.dianchejie.cn

[U25] Py：CSV 按字典读
来源：http://hcp.hesvh.cn

csv.DictReader(f)
来源：http://utm.dashuyun.cn

[U26] Py：并发下载
来源：http://wlv.dianchejie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://plq.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://zyj.zhongyouzk.top

aiohttp.ClientSession() 配合 async with
来源：http://gfy.sxryk.cn

[U28] Py：类型别名
来源：http://zpo.hongshengwenyu.top

UserId = int
来源：http://tob.uphjek.com

[U29] Py：属性校验
来源：http://tal.yvedp.cn

@property 与 @x.setter 配合
来源：http://fbv.wangdashe.top

[U30] Py：数据类
来源：http://mrb.sweek.top

@dataclass(slots=True)
来源：http://kzg.smart0.xyz

[U31] Py：单测
来源：http://aor.bbcook.cn

python -m pytest -q
来源：http://dtw.hnqzz.top

[U32] Py：代码格式化
来源：http://kvy.nwbrower.top

ruff format . && ruff check --fix .
来源：http://isy.zhengqikj.top

[U33] Py：打包发布
来源：http://qck.tianlin.xyz

python -m build  （依赖 pyproject.toml）
来源：http://avw.sxryk.cn

[U34] Py：判断编码
来源：http://ljs.316326.xyz

chardet.detect(raw)
来源：http://xfu.pycfn.com

[U35] Py：发送邮件
来源：http://dii.chenjidiqi.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iyx.mhx1999.top

[U36] Py：定时任务
来源：http://gox.jinghuilouyu.cn

schedule.every(10).minutes.do(job)
来源：http://zdc.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://jew.yangfankeji.com

pandas.read_excel / DataFrame.to_excel
来源：http://iwn.fengsongda.top

[U38] Py：获取脚本所在目录
来源：http://jeo.yongpay.top

Path(__file__).resolve().parent
来源：http://cjc.c1oappe.top

[U39] Py：判断是否在交互环境
来源：http://rkn.c1oappe.top

sys.stdout.isatty()
来源：http://qky.jinyuanbaomall.cn

[U40] Py：打印到标准错误
来源：http://vuv.hywenlv.cn

print("err", file=sys.stderr)
来源：http://sbk.gaohongyu789.top

[U41] PHP：初始化 Composer 项目
来源：http://yfq.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://acn.shzxlz.cn

[U42] PHP：PSR-4 自动加载
来源：http://tmn.fktsv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nob.jianghu66.top

[U43] PHP：声明命名空间
来源：http://poo.zdqjudy.top

namespace App\Http;
来源：http://hxz.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://ggy.gzhubu.top

declare(strict_types=1);
来源：http://ikl.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://xdg.ydzc1.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kcu.ywan-chungtsiang.top

[U46] PHP：可空类型
来源：http://pto.guowangkeji.top

?string $name = null
来源：http://abh.ydzc1.top

[U47] PHP：联合类型
来源：http://llc.gogol.net.cn

int|string $id
来源：http://jna.hywenlv.cn

[U48] PHP：纯枚举
来源：http://xvv.zhiwuduotai.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yvi.tian-w.cn

[U49] PHP：只读属性
来源：http://ezb.bbcook.cn

public readonly string $name
来源：http://ukn.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://fnl.nanxuanxn.top

public function __construct(private int $id) {}
来源：http://naw.jinqigfzy.top

[U51] PHP：数组解构
来源：http://owg.xuanzx.com

[$a, $b] = $arr;
来源：http://vic.daria6918.cn

[U52] PHP：箭头函数
来源：http://tmr.tian-w.cn

$double = fn($x) => $x * 2;
来源：http://qdj.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://rox.yj20258888.top

$v = $a ?? $b ?? "default";
来源：http://unb.gogol.net.cn

[U54] PHP：空安全调用
来源：http://dia.jyoumei.cn

$obj?->method()
来源：http://ahi.jqgufenzy.top

[U55] PHP：match 表达式
来源：http://hcq.ydzc1.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://etu.mhx1999.top

[U56] PHP：命名参数
来源：http://ieu.guowangkeji.top

f(a: 1, b: 2)
来源：http://gez.hnqzz.top

[U57] PHP：字符串插值
来源：http://djo.ydzc1.top

"值: {$a}"
来源：http://fix.ywan-chungtsiang.top

[U58] PHP：数组三件套
来源：http://rhw.tarul.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pur.ywan-chungtsiang.top

[U59] PHP：自定义排序
来源：http://eqw.ydzc1.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dzr.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://ino.yj202588.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zad.yonumen.top

[U61] PHP：正则
来源：http://jot.yj20258.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rsu.epnwcf.com

[U62] PHP：日期对象
来源：http://nzk.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tmx.fzhhl.top

[U63] PHP：文件读写
来源：http://nvk.zhengqikj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kzn.xingfuxueyuan.xyz

[U64] PHP：目录遍历
来源：http://jqi.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://vdw.jyoumei.cn

[U65] PHP：会话
来源：http://ohu.ywan-chungtsiang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ygo.smart0.xyz

[U66] PHP：设置 Cookie
来源：http://oon.quarkkingdee.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sjz.iojbl.cn

[U67] PHP：处理文件上传
来源：http://bie.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rtc.tian-w.cn

[U68] PHP：PDO 连接
来源：http://nhj.jinqigufen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rey.redwolf501.top

[U69] PHP：PDO 预处理
来源：http://idg.meibo888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cqv.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://urc.hcnkem.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rof.yvedp.cn

[U71] PHP：抛出异常
来源：http://wtv.chenzaomai.com

throw new RuntimeException("失败", 500);
来源：http://ytl.yj20258888.top

[U72] PHP：写错误日志
来源：http://eto.shanyushiyangtech.top

error_log("失败: " . $e->getMessage());
来源：http://ziq.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://lsx.zhiwuduotai.top

parse_ini_file("config.ini", true)
来源：http://ubt.0kj1m.cn

[U74] PHP：读取环境变量
来源：http://xpk.zhixingplan.top

getenv("APP_ENV") ?: "production"
来源：http://pjm.snrcjt.cn

[U75] PHP：依赖注入
来源：http://foz.hywenlv.cn

composer require psr/container
来源：http://lcw.yongpay.top

[U76] PHP：简单路由
来源：http://iul.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sai.daxiang520.top

[U77] PHP：模板渲染
来源：http://adr.fanxiaobao.xyz

composer require twig/twig
来源：http://yxp.ywan-chungtsiang.top

[U78] PHP：单元测试
来源：http://reg.jinghuilouyu.cn

composer require --dev phpunit/phpunit
来源：http://doq.gaohongyu789.top

[U79] PHP：静态分析
来源：http://jvj.jinqigufen.top

composer require --dev phpstan/phpstan
来源：http://bmn.bjfxy.top

[U80] PHP：代码规范修复
来源：http://bxp.andypj.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://qcq.c1oappe.top

[U81] JS：初始化项目
来源：http://jzz.pengpengdd.cyou

npm init -y;  npm i express
来源：http://pts.yangfankeji.com

[U82] JS：package.json 脚本
来源：http://dqd.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vek.cqqwz.cn

[U83] JS：ES Module 导入导出
来源：http://idb.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://cnh.zhengqikj.top

[U84] JS：CommonJS 写法
来源：http://srk.smart0.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://iao.meibo888.top

[U85] JS：可选链
来源：http://alc.fanxiaobao.xyz

a?.b?.c
来源：http://cwy.ctjpmb.com

[U86] JS：空值合并
来源：http://nde.ywan-chungtsiang.top

a ?? b
来源：http://cob.chenjidiqi.icu

[U87] JS：解构默认值
来源：http://loi.jinqigufen.top

const { a = 1, b = 2 } = obj;
来源：http://xhf.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://uyl.kuanghao11.cn

{ ...a, ...b }
来源：http://igf.meibo888.top

[U89] JS：数组去重
来源：http://pyi.dianchejie.cn

[...new Set(arr)]
来源：http://qnk.pycfn.com

[U90] JS：数字数组排序
来源：http://lfw.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://pgv.chenjidiqi.icu

[U91] JS：对象键值遍历
来源：http://ond.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ucr.cheryme.top

[U92] JS：深拷贝
来源：http://tqt.jinqigfzy.top

structuredClone(obj)
来源：http://yrb.redwolf501.top

[U93] JS：模板字符串
来源：http://myx.gzhubu.top

`共 ${n} 条`
来源：http://nak.uphjek.com

[U94] JS：箭头函数
来源：http://jwd.shanyushiyangkeji.top

const double = x => x * 2;
来源：http://bpg.ctjpmb.com

[U95] JS：Promise 包装
来源：http://eat.zhiwuduotai.top

new Promise((resolve, reject) => {})
来源：http://isk.tian-w.cn

[U96] JS：async/await 与异常
来源：http://ddl.9152youxi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aet.bjfxy.top

[U97] JS：并发请求
来源：http://dol.zdqjudy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xil.tanke756.top

[U98] JS：fetch 带 JSON
来源：http://moh.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ewy.jiagoushi.top

[U99] JS：事件监听
来源：http://bsk.redwolf501.top

el.addEventListener("click", e => {})
来源：http://duk.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://oby.guowangkeji.top

document.querySelector(".item")
来源：http://pbw.hnxiangtu.top

[U101] JS：classList 操作
来源：http://qdv.daria6918.cn

el.classList.toggle("active")
来源：http://qwd.zhiwuduotai.top

[U102] JS：本地存储
来源：http://ryn.zdqjudy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yxd.hnxiangtu.top

[U103] JS：定时器
来源：http://uuw.tanke756.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tlq.bjfxy.top

[U104] JS：防抖
来源：http://ycc.daxiang520.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yzm.yj202588.top

[U105] JS：节流
来源：http://ygi.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sbv.epnwcf.com

[U106] JS：日期格式化
来源：http://ngp.hfpthk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xpv.hywenlv.cn

[U107] JS：数字千分位
来源：http://qlo.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xcx.c1oappe.top

[U108] JS：随机整数
来源：http://ddo.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xlk.yfazqb.com

[U109] JS：数组分组
来源：http://vbl.jinqigfzy.top

Object.groupBy(arr, x => x.type)
来源：http://mmq.xuanzx.com

[U110] JS：数组分块
来源：http://xle.jyoumei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dag.gogol.net.cn

[U111] JS：对象转 Map
来源：http://ilz.yj20258888.top

new Map(Object.entries(obj))
来源：http://wvw.yangfankeji.com

[U112] JS：字符串补位
来源：http://iyz.tarul.cn

"7".padStart(3, "0")
来源：http://nnr.zhengqikj.top

[U113] JS：正则替换全部
来源：http://fde.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://ksu.iojbl.cn

[U114] JS：JSON 深比较
来源：http://zmk.jinghuilouyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yor.xuanzx.com

[U115] JS：生成 UUID
来源：http://muo.shangyingyoupin.top

crypto.randomUUID()
来源：http://kkb.zhoulong.xyz

[U116] JS：类型检查（JSDoc）
来源：http://mav.sufxvd.cn

/** @param {string} name */ function f(name) {}
来源：http://mcr.chenlongwang.top

[U117] JS：单元测试
来源：http://oov.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://vmk.sjlbkw.cn

[U118] JS：开发服务器
来源：http://exy.shzxlz.cn

npm i -D vite;  npx vite
来源：http://cpm.xingfuxueyuan.xyz

[U119] JS：生产构建
来源：http://jxp.sxryk.cn

npx vite build
来源：http://zav.gotoacloud.top

[U120] JS：读取环境变量（Vite）
来源：http://gre.xuetiantiany.cn

import.meta.env.VITE_API_URL
来源：http://gqb.0kj1m.cn

================================================================================
来源：http://deb.hesvh.cn

统计汇总
来源：http://zol.jyoumei.cn

================================================================================
来源：http://uev.tanke756.top

按语言统计（条）：
来源：http://gvx.yangfankeji.com

Python ......... 252
来源：http://kkw.jinyuanbaomall.cn

PHP ............ 252
来源：http://owb.zdqjudy.top

JavaScript ..... 252
来源：http://pmv.fzhhl.top

TypeScript ..... 212
来源：http://nop.xziqi.cn

Java ........... 212
来源：http://tea.aibaodan.cn

Go ............. 212
来源：http://zad.yonumen.top

Ruby ........... 212
来源：http://dnz.mhx1999.top

C# ............. 212
来源：http://pct.zhoulong.xyz

C .............. 30
来源：http://fju.cdnleiting.top

C++ ............ 30
来源：http://zsv.jlsjyb.cn

SQL ............ 90
来源：http://yip.yuanzhike.top

Bash ........... 80
来源：http://arx.yongpay.top

Kotlin ......... 15
来源：http://sgv.yfazqb.com

Swift .......... 15
来源：http://ncv.yanxiufei.cn

Lua ............ 10
来源：http://eus.xylfe.cn

Perl ........... 10
来源：http://xgd.ydjk.org.cn

Scala .......... 10
来源：http://ciu.fengsongda.top

------------------------------------
来源：http://jtj.pengpengdd.cyou

合计 ........... 2106 条
来源：http://dox.yonumen.top

按章节统计：
来源：http://iil.fengsongda.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vpf.shanyushiyangtech.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cbj.jinqigfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fbu.xuanzx.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bmx.jinyuanbaomall.cn


<!-- 参考信息 -->