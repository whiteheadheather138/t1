代发 wailian999

[T49] Perl：函数
来源：http://ddo.fengsongda.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fiv.smart0.xyz

[T50] Perl：逐行读文件
来源：http://ban.hammf.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://epl.jyoumei.cn

while (my $line = <$fh>) { print $line; }
来源：http://vem.zhengqikj.top

[T51] Scala：Hello World
来源：http://mvj.jinyuanbaomall.cn

println("Hello")
来源：http://dwu.yvedp.cn

[T52] Scala：变量
来源：http://gqm.zdbjq.cn

val a = 1;  var b = 2
来源：http://htw.fanxiaobao.xyz

[T53] Scala：字符串插值
来源：http://tej.birdmap.top

s"值: $b"
来源：http://wro.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://pps.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://sev.sysykeji.top

[T55] Scala：集合过滤
来源：http://ckj.tarul.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ufh.yuanzhike.top

[T56] Scala：样例类
来源：http://ryv.hnqzz.top

case class User(name: String, age: Int)
来源：http://oua.fengsongda.top

[T57] Scala：模式匹配
来源：http://leg.fengsongda.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vec.fanxiaobao.xyz

[T58] Scala：函数定义
来源：http://upx.gotoacloud.top

def add(a: Int, b: Int): Int = a + b
来源：http://gsp.feifeiyinyue.top

[T59] Scala：循环
来源：http://sou.cdnleiting.top

for (i <- 1 to 10) println(i)
来源：http://nzp.yueranfly.top

[T60] Scala：折叠
来源：http://sbd.jlsjyb.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://smm.zhiwuduotai.top

================================================================================
来源：http://utt.xuetiantiany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tzm.sjlbkw.cn

================================================================================
来源：http://jog.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://bwr.cqqwz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jno.mhx1999.top

[U02] Py：导出 / 安装依赖
来源：http://vqm.c1oappe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cxr.sufxvd.cn

[U03] Py：加载 .env 配置
来源：http://hit.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xcp.yangfankeji.com

[U04] Py：变量调试打印
来源：http://ecl.jinqigufen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hot.xziqi.cn

[U05] Py：列表去重且保序
来源：http://vne.yuxming.cn

list(dict.fromkeys(arr))
来源：http://bhb.jiagoushi.top

[U06] Py：合并两个字典
来源：http://ngz.havefunace.top

{**a, **b}
来源：http://apd.daria6918.cn

[U07] Py：反转字典键值
来源：http://nwo.fzhhl.top

{v: k for k, v in d.items()}
来源：http://kvi.fktsv.cn

[U08] Py：展平二维列表
来源：http://iup.hcnkem.com

[y for x in nested for y in x]
来源：http://ybv.shanyushiyangtech.top

[U09] Py：字典取最大值的键
来源：http://lkq.yfazqb.com

max(d, key=d.get)
来源：http://wna.vehdjk.com

[U10] Py：按值排序字典
来源：http://xco.ehwqpu.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qxf.jqgfzy.top

[U11] Py：生成器表达式
来源：http://tuu.yangfankeji.com

(x * 2 for x in arr)
来源：http://eba.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sqr.xinyue.icu

Counter(arr).most_common(3)
来源：http://lze.jiagoushi.top

[U13] Py：固定长度队列
来源：http://bvi.cdnleiting.top

deque(maxlen=10)
来源：http://amq.wangshuangyany.cn

[U14] Py：分组收集到列表
来源：http://tsj.vqdsnc.cn

defaultdict(list)
来源：http://syl.gaohongyu789.top

[U15] Py：高精度计时
来源：http://ner.pengpengdd.cyou

t = time.perf_counter()
来源：http://zrf.zhaomingkeji.xyz

[U16] Py：命令行参数解析
来源：http://ltp.ppjwa.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tvt.nanxinkj.top

[U17] Py：初始化日志
来源：http://noe.daria6918.cn

logging.basicConfig(level=logging.INFO)
来源：http://mwa.hywenlv.cn

[U18] Py：预编译正则
来源：http://yyd.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://ady.daxiang520.top

[U19] Py：正则替换带回调
来源：http://idw.hammf.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oyy.316326.xyz

[U20] Py：缓存函数结果
来源：http://bhx.cqqwz.cn

@functools.lru_cache(maxsize=None)
来源：http://sae.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://mlq.smart0.xyz

@contextlib.contextmanager
来源：http://tlk.tianlin.xyz

[U22] Py：矩阵转置
来源：http://nvz.tanke756.top

list(zip(*m))
来源：http://bom.bjfxy.top

[U23] Py：分块读取大文件
来源：http://cnm.zhiwuduotai.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://chl.yonumen.top

[U24] Py：路径操作
来源：http://pqv.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://raq.316326.xyz

[U25] Py：CSV 按字典读
来源：http://qeq.sysykeji.top

csv.DictReader(f)
来源：http://ccw.zhiwuduotai.top

[U26] Py：并发下载
来源：http://yfr.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xag.gotoacloud.top

[U27] Py：异步 HTTP
来源：http://irj.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://rll.fengsongda.top

[U28] Py：类型别名
来源：http://rqw.jinqigfzy.top

UserId = int
来源：http://grd.svipenyu.cn

[U29] Py：属性校验
来源：http://lpu.xinyue.icu

@property 与 @x.setter 配合
来源：http://qig.zhiwuduotai.top

[U30] Py：数据类
来源：http://ent.ctjpmb.com

@dataclass(slots=True)
来源：http://szp.jinyuanbaomall.cn

[U31] Py：单测
来源：http://cbf.hnxiangtu.top

python -m pytest -q
来源：http://mka.epnwcf.com

[U32] Py：代码格式化
来源：http://pbn.yanxiufei.cn

ruff format . && ruff check --fix .
来源：http://pyb.iojbl.cn

[U33] Py：打包发布
来源：http://kqs.zycfv.cn

python -m build  （依赖 pyproject.toml）
来源：http://uwb.cashguo.top

[U34] Py：判断编码
来源：http://iwa.wangshuangyany.cn

chardet.detect(raw)
来源：http://uab.tian-w.cn

[U35] Py：发送邮件
来源：http://lkn.zhaomingkeji.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zje.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://xsi.shzxlz.cn

schedule.every(10).minutes.do(job)
来源：http://xop.zdqjudy.top

[U37] Py：读写 Excel
来源：http://gtu.wangdashe.top

pandas.read_excel / DataFrame.to_excel
来源：http://ivt.xylfe.cn

[U38] Py：获取脚本所在目录
来源：http://mtl.snrcjt.cn

Path(__file__).resolve().parent
来源：http://gok.jiagoushi.top

[U39] Py：判断是否在交互环境
来源：http://ibr.gzhubu.top

sys.stdout.isatty()
来源：http://xae.jinyuanbaomall.cn

[U40] Py：打印到标准错误
来源：http://mlu.yfazqb.com

print("err", file=sys.stderr)
来源：http://ods.svipenyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ovy.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://suk.fengsongda.top

[U42] PHP：PSR-4 自动加载
来源：http://qjs.tarul.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vwt.zycfv.cn

[U43] PHP：声明命名空间
来源：http://stl.chenlongwang.top

namespace App\Http;
来源：http://xha.gzhubu.top

[U44] PHP：开启严格类型
来源：http://uzt.zhiwuduotai.top

declare(strict_types=1);
来源：http://gqu.xuanzx.com

[U45] PHP：类型声明与返回类型
来源：http://qnr.dashuyun.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ynx.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://mbf.dashuyun.cn

?string $name = null
来源：http://lkh.jianghu66.top

[U47] PHP：联合类型
来源：http://mpc.zhoulong.xyz

int|string $id
来源：http://ljx.ppjwa.cn

[U48] PHP：纯枚举
来源：http://hez.feifeiyinyue.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dzx.zhengqikj.top

[U49] PHP：只读属性
来源：http://vxa.daxiang520.top

public readonly string $name
来源：http://hth.yfazqb.com

[U50] PHP：构造器属性提升
来源：http://wgb.xylfe.cn

public function __construct(private int $id) {}
来源：http://blh.yuxming.cn

[U51] PHP：数组解构
来源：http://wgz.yuanzhike.top

[$a, $b] = $arr;
来源：http://jbb.feifeiyinyue.top

[U52] PHP：箭头函数
来源：http://zff.ydzc1.top

$double = fn($x) => $x * 2;
来源：http://yal.nanxinkj.top

[U53] PHP：空合并运算符
来源：http://qna.chenjidiqi.icu

$v = $a ?? $b ?? "default";
来源：http://moy.jinqigfzy.top

[U54] PHP：空安全调用
来源：http://upn.dianchejie.cn

$obj?->method()
来源：http://mtp.iojbl.cn

[U55] PHP：match 表达式
来源：http://wmu.guannengcc.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dpc.ivvv.top

[U56] PHP：命名参数
来源：http://hig.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://uoh.nanxinkj.top

[U57] PHP：字符串插值
来源：http://cnq.jqgufenzy.top

"值: {$a}"
来源：http://glp.yj20258.top

[U58] PHP：数组三件套
来源：http://pyd.fktsv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kvp.mhx1999.top

[U59] PHP：自定义排序
来源：http://tro.shangyingyoupin.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lfx.c1oappe.top

[U60] PHP：JSON 编解码
来源：http://pyy.hywenlv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jqn.yongpay.top

[U61] PHP：正则
来源：http://ngp.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://etq.sxryk.cn

[U62] PHP：日期对象
来源：http://lpc.wangdashe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ekk.316326.xyz

[U63] PHP：文件读写
来源：http://fty.zhiwuduotai.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tyr.guowangkeji.top

[U64] PHP：目录遍历
来源：http://hdo.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://syk.yanxiufei.cn

[U65] PHP：会话
来源：http://yvm.pengpengdd.cyou

session_start();  $_SESSION["uid"] = 1;
来源：http://vtp.jyoumei.cn

[U66] PHP：设置 Cookie
来源：http://ssr.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eir.shangyingyoupin.top

[U67] PHP：处理文件上传
来源：http://xsd.tanke756.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bjd.zdbjq.cn

[U68] PHP：PDO 连接
来源：http://tzr.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uow.cheryme.top

[U69] PHP：PDO 预处理
来源：http://spu.smart0.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cpx.zhongyouzk.top

[U70] PHP：PDO 事务
来源：http://bwa.cdnleiting.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nxz.guannengcc.top

[U71] PHP：抛出异常
来源：http://lwo.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://sbo.hcnkem.com

[U72] PHP：写错误日志
来源：http://qeu.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://qvm.meibo888.top

[U73] PHP：读取 ini 配置
来源：http://xhw.guowangkeji.top

parse_ini_file("config.ini", true)
来源：http://ogc.daria6918.cn

[U74] PHP：读取环境变量
来源：http://tqo.jinqigfzy.top

getenv("APP_ENV") ?: "production"
来源：http://iop.wangdashe.top

[U75] PHP：依赖注入
来源：http://yij.andypj.xyz

composer require psr/container
来源：http://gcc.zhiwuduotai.top

[U76] PHP：简单路由
来源：http://hug.daria6918.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://okk.xziqi.cn

[U77] PHP：模板渲染
来源：http://esg.gotoacloud.top

composer require twig/twig
来源：http://mve.sysykeji.top

[U78] PHP：单元测试
来源：http://ajp.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://ypz.smart0.xyz

[U79] PHP：静态分析
来源：http://yct.uphjek.com

composer require --dev phpstan/phpstan
来源：http://wwo.sjlbkw.cn

[U80] PHP：代码规范修复
来源：http://xoe.zhaomingkeji.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://zcn.shuidangran.top

[U81] JS：初始化项目
来源：http://ytr.quarkkingdee.top

npm init -y;  npm i express
来源：http://ocj.bbcook.cn

[U82] JS：package.json 脚本
来源：http://dra.vehdjk.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eso.gaohongyu789.top

[U83] JS：ES Module 导入导出
来源：http://uyu.redwolf501.top

export const a = 1;  import { a } from "./m.js";
来源：http://qhb.sufxvd.cn

[U84] JS：CommonJS 写法
来源：http://jfb.cashguo.top

module.exports = { a };  const { a } = require("./m");
来源：http://dpw.epnwcf.com

[U85] JS：可选链
来源：http://nri.chenlongwang.top

a?.b?.c
来源：http://dzg.tanke756.top

[U86] JS：空值合并
来源：http://krq.chenlongwang.top

a ?? b
来源：http://lfh.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://coe.bjfxy.top

const { a = 1, b = 2 } = obj;
来源：http://yic.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://gok.sweek.top

{ ...a, ...b }
来源：http://hmb.hnqzz.top

[U89] JS：数组去重
来源：http://bia.xuetiantiany.cn

[...new Set(arr)]
来源：http://zma.hywenlv.cn

[U90] JS：数字数组排序
来源：http://ytw.pengpengdd.cyou

[...arr].sort((a, b) => a - b)
来源：http://fzy.xylfe.cn

[U91] JS：对象键值遍历
来源：http://vft.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://osa.yvedp.cn

[U92] JS：深拷贝
来源：http://nxe.sweek.top

structuredClone(obj)
来源：http://rov.zycfv.cn

[U93] JS：模板字符串
来源：http://ons.hysaishi.cn

`共 ${n} 条`
来源：http://tyy.xuanzx.com

[U94] JS：箭头函数
来源：http://awr.guannengcc.top

const double = x => x * 2;
来源：http://zga.cheryme.top

[U95] JS：Promise 包装
来源：http://aav.9152youxi.cn

new Promise((resolve, reject) => {})
来源：http://kgq.birdmap.top

[U96] JS：async/await 与异常
来源：http://qwk.gaohongyu789.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wjx.hongshengwenyu.top

[U97] JS：并发请求
来源：http://niu.hongshengwenyu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mfw.xuetiantiany.cn

[U98] JS：fetch 带 JSON
来源：http://gjh.52xcode.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://btc.havefunace.top

[U99] JS：事件监听
来源：http://elk.zdbjq.cn

el.addEventListener("click", e => {})
来源：http://rok.haohaochexian.top

[U100] JS：DOM 查询
来源：http://zme.tianlin.xyz

document.querySelector(".item")
来源：http://qcv.fzhhl.top

[U101] JS：classList 操作
来源：http://tob.redwolf501.top

el.classList.toggle("active")
来源：http://sdz.sweek.top

[U102] JS：本地存储
来源：http://npw.zycfv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ukz.fktsv.cn

[U103] JS：定时器
来源：http://pnx.gzhubu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uuz.jinghuilouyu.cn

[U104] JS：防抖
来源：http://nyy.zdbjq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://trg.yongpay.top

[U105] JS：节流
来源：http://vqj.sjlbkw.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ckg.yueranfly.top

[U106] JS：日期格式化
来源：http://gfl.zhiwuduotai.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://phs.jiagoushi.top

[U107] JS：数字千分位
来源：http://obu.gzhubu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cyq.0kj1m.cn

[U108] JS：随机整数
来源：http://rvb.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zox.yj202588.top

[U109] JS：数组分组
来源：http://swg.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://pwv.fehbvm.com

[U110] JS：数组分块
来源：http://uxp.sxryk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hpz.cucudq.cn

[U111] JS：对象转 Map
来源：http://nch.cucudq.cn

new Map(Object.entries(obj))
来源：http://gzh.ivvv.top

[U112] JS：字符串补位
来源：http://aau.ppjwa.cn

"7".padStart(3, "0")
来源：http://rue.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://zkd.svipenyu.cn

s.replaceAll("a", "b")
来源：http://unw.yuxming.cn

[U114] JS：JSON 深比较
来源：http://igk.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://anv.guannengcc.top

[U115] JS：生成 UUID
来源：http://pdf.ywan-chungtsiang.top

crypto.randomUUID()
来源：http://gof.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://slo.cdnleiting.top

/** @param {string} name */ function f(name) {}
来源：http://csm.zdqjudy.top

[U117] JS：单元测试
来源：http://shz.hongshengwenyu.top

npm i -D vitest;  npx vitest
来源：http://uzv.hfpthk.cn

[U118] JS：开发服务器
来源：http://atg.epnwcf.com

npm i -D vite;  npx vite
来源：http://urv.andypj.xyz

[U119] JS：生产构建
来源：http://pjf.jyoumei.cn

npx vite build
来源：http://ahm.shuidangran.top

[U120] JS：读取环境变量（Vite）
来源：http://yxa.quarkkingdee.top

import.meta.env.VITE_API_URL
来源：http://yxp.xylfe.cn

================================================================================
来源：http://jsl.epnwcf.com

统计汇总
来源：http://wyh.bbcook.cn

================================================================================
来源：http://kwl.meibo888.top

按语言统计（条）：
来源：http://ltr.jianghu66.top

Python ......... 252
来源：http://yiz.zhijiandao.cn

PHP ............ 252
来源：http://jry.wangshuangyany.cn

JavaScript ..... 252
来源：http://kuq.chenzaomai.com

TypeScript ..... 212
来源：http://ejc.smart0.xyz

Java ........... 212
来源：http://lzj.fktsv.cn

Go ............. 212
来源：http://tsp.yuanzhike.top

Ruby ........... 212
来源：http://ftw.gzhubu.top

C# ............. 212
来源：http://hjm.bbcook.cn

C .............. 30
来源：http://ezi.hammf.cn

C++ ............ 30
来源：http://xgh.cashguo.top

SQL ............ 90
来源：http://zly.dianchejie.cn

Bash ........... 80
来源：http://iyj.gzhubu.top

Kotlin ......... 15
来源：http://tet.jinghuilouyu.cn

Swift .......... 15
来源：http://ggw.nwbrower.top

Lua ............ 10
来源：http://vzz.ehwqpu.com

Perl ........... 10
来源：http://zua.9152youxi.cn

Scala .......... 10
来源：http://ugb.yj202588.top

------------------------------------
来源：http://zmw.52xcode.cn

合计 ........... 2106 条
来源：http://psx.zhiwuduotai.top

按章节统计：
来源：http://sql.nwbrower.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vtl.hywenlv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mkc.cheryme.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xpq.xylfe.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fgx.xinyue.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ijt.snrcjt.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mgv.gaohongyu789.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ndv.sweek.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fid.zhaomingkeji.xyz


<!-- 参考信息 -->