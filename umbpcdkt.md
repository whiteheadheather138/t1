代发 wailian999

[T49] Perl：函数
来源：http://wcl.fktsv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kls.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://fuc.guannengcc.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qjy.tian-w.cn

while (my $line = <$fh>) { print $line; }
来源：http://gbp.fktsv.cn

[T51] Scala：Hello World
来源：http://lgr.guowangkeji.top

println("Hello")
来源：http://jye.jinqigfzy.top

[T52] Scala：变量
来源：http://red.fktsv.cn

val a = 1;  var b = 2
来源：http://gek.sufxvd.cn

[T53] Scala：字符串插值
来源：http://gfl.cheryme.top

s"值: $b"
来源：http://jyg.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://qkw.hfpthk.cn

List(1, 2, 3).map(_ * 2)
来源：http://lng.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://zsj.yj20258.top

List(1, 2, 3).filter(_ > 1)
来源：http://kly.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://zdi.uphjek.com

case class User(name: String, age: Int)
来源：http://pyh.jiagoushi.top

[T57] Scala：模式匹配
来源：http://exf.vehdjk.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://cjw.cashguo.top

[T58] Scala：函数定义
来源：http://grg.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://gah.andypj.xyz

[T59] Scala：循环
来源：http://xig.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://sju.fehbvm.com

[T60] Scala：折叠
来源：http://rkh.shzxlz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lwd.yuxming.cn

================================================================================
来源：http://yjs.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yiw.316326.xyz

================================================================================
来源：http://qqp.wangshuangyany.cn

[U01] Py：创建虚拟环境
来源：http://shk.sxryk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://psx.ehwqpu.com

[U02] Py：导出 / 安装依赖
来源：http://pnn.ivvv.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yfp.havefunace.top

[U03] Py：加载 .env 配置
来源：http://xid.ctjpmb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://ffm.ydzc1.top

[U04] Py：变量调试打印
来源：http://yar.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tqc.sweek.top

[U05] Py：列表去重且保序
来源：http://akf.sweek.top

list(dict.fromkeys(arr))
来源：http://fgw.bjfxy.top

[U06] Py：合并两个字典
来源：http://ovy.tian-w.cn

{**a, **b}
来源：http://uxf.yvedp.cn

[U07] Py：反转字典键值
来源：http://wxc.sxryk.cn

{v: k for k, v in d.items()}
来源：http://lkj.pycfn.com

[U08] Py：展平二维列表
来源：http://emc.nanxinkj.top

[y for x in nested for y in x]
来源：http://rij.yj20258.top

[U09] Py：字典取最大值的键
来源：http://mvm.fzhhl.top

max(d, key=d.get)
来源：http://lro.shzxlz.cn

[U10] Py：按值排序字典
来源：http://jfx.chenjidiqi.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qiv.dashuyun.cn

[U11] Py：生成器表达式
来源：http://ehl.jinghuilouyu.cn

(x * 2 for x in arr)
来源：http://ljz.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zfs.fanxiaobao.xyz

Counter(arr).most_common(3)
来源：http://vxy.hywenlv.cn

[U13] Py：固定长度队列
来源：http://ikg.vqdsnc.cn

deque(maxlen=10)
来源：http://vxu.dashuyun.cn

[U14] Py：分组收集到列表
来源：http://tcj.tarul.cn

defaultdict(list)
来源：http://ofn.feifeiyinyue.top

[U15] Py：高精度计时
来源：http://fmf.gogol.net.cn

t = time.perf_counter()
来源：http://emd.hesvh.cn

[U16] Py：命令行参数解析
来源：http://cvh.cashguo.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vtp.shzxlz.cn

[U17] Py：初始化日志
来源：http://ljl.yonumen.top

logging.basicConfig(level=logging.INFO)
来源：http://gpw.svipenyu.cn

[U18] Py：预编译正则
来源：http://elf.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://zxa.daria6918.cn

[U19] Py：正则替换带回调
来源：http://isz.aizwys.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wlw.vehdjk.com

[U20] Py：缓存函数结果
来源：http://ieh.smart0.xyz

@functools.lru_cache(maxsize=None)
来源：http://zlj.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://azq.havefunace.top

@contextlib.contextmanager
来源：http://ndv.52xcode.cn

[U22] Py：矩阵转置
来源：http://vlj.mhx1999.top

list(zip(*m))
来源：http://uxw.ywan-chungtsiang.top

[U23] Py：分块读取大文件
来源：http://gkl.iojbl.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://unn.dashuyun.cn

[U24] Py：路径操作
来源：http://qzr.yangfankeji.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://egc.smart0.xyz

[U25] Py：CSV 按字典读
来源：http://oie.hongshengwenyu.top

csv.DictReader(f)
来源：http://tjm.jqgfzy.top

[U26] Py：并发下载
来源：http://kdw.hnxiangtu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vgl.chenlongwang.top

[U27] Py：异步 HTTP
来源：http://lui.jianghu66.top

aiohttp.ClientSession() 配合 async with
来源：http://rhh.shangyingyoupin.top

[U28] Py：类型别名
来源：http://cfo.zhijiandao.cn

UserId = int
来源：http://awc.tianlin.xyz

[U29] Py：属性校验
来源：http://opu.shanyushiyangtech.top

@property 与 @x.setter 配合
来源：http://ffb.redwolf501.top

[U30] Py：数据类
来源：http://cye.nanxinkj.top

@dataclass(slots=True)
来源：http://wls.gogol.net.cn

[U31] Py：单测
来源：http://oci.ehwqpu.com

python -m pytest -q
来源：http://uan.epnwcf.com

[U32] Py：代码格式化
来源：http://ght.fktsv.cn

ruff format . && ruff check --fix .
来源：http://jiv.shzxlz.cn

[U33] Py：打包发布
来源：http://vio.yanxiufei.cn

python -m build  （依赖 pyproject.toml）
来源：http://neh.hesvh.cn

[U34] Py：判断编码
来源：http://fqa.yueranfly.top

chardet.detect(raw)
来源：http://dpv.0kj1m.cn

[U35] Py：发送邮件
来源：http://vso.ctjpmb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xhy.jlsjyb.cn

[U36] Py：定时任务
来源：http://krh.yj202588.top

schedule.every(10).minutes.do(job)
来源：http://arc.chenzaomai.com

[U37] Py：读写 Excel
来源：http://mja.sjlbkw.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mon.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://zep.ehwqpu.com

Path(__file__).resolve().parent
来源：http://ekq.zdbjq.cn

[U39] Py：判断是否在交互环境
来源：http://wkh.ppjwa.cn

sys.stdout.isatty()
来源：http://zet.hysaishi.cn

[U40] Py：打印到标准错误
来源：http://zny.chenzaomai.com

print("err", file=sys.stderr)
来源：http://jib.cdnleiting.top

[U41] PHP：初始化 Composer 项目
来源：http://jqc.fengsongda.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vix.hcnkem.com

[U42] PHP：PSR-4 自动加载
来源：http://wzu.yvedp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sgw.shanyushiyangtech.top

[U43] PHP：声明命名空间
来源：http://sat.0kj1m.cn

namespace App\Http;
来源：http://qus.ybcxt.top

[U44] PHP：开启严格类型
来源：http://gla.dashuyun.cn

declare(strict_types=1);
来源：http://nwe.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://enn.havefunace.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xvh.snrcjt.cn

[U46] PHP：可空类型
来源：http://igr.gogol.net.cn

?string $name = null
来源：http://dhs.jqgufenzy.top

[U47] PHP：联合类型
来源：http://jvr.yangfankeji.com

int|string $id
来源：http://ffh.hcnkem.com

[U48] PHP：纯枚举
来源：http://dhx.cucudq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nta.epnwcf.com

[U49] PHP：只读属性
来源：http://nmh.zhongyouzk.top

public readonly string $name
来源：http://xvm.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://bjo.feifeiyinyue.top

public function __construct(private int $id) {}
来源：http://nam.cqqwz.cn

[U51] PHP：数组解构
来源：http://wmj.ppjwa.cn

[$a, $b] = $arr;
来源：http://lsx.yuanzhike.top

[U52] PHP：箭头函数
来源：http://awb.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://dla.yuxming.cn

[U53] PHP：空合并运算符
来源：http://ktf.hnxiangtu.top

$v = $a ?? $b ?? "default";
来源：http://mcf.mhx1999.top

[U54] PHP：空安全调用
来源：http://giu.zycfv.cn

$obj?->method()
来源：http://wsv.hnqzz.top

[U55] PHP：match 表达式
来源：http://czy.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://irj.jinqigufen.top

[U56] PHP：命名参数
来源：http://jyb.pycfn.com

f(a: 1, b: 2)
来源：http://amw.yj20258888.top

[U57] PHP：字符串插值
来源：http://kkm.quarkkingdee.top

"值: {$a}"
来源：http://iyd.chenjidiqi.icu

[U58] PHP：数组三件套
来源：http://slx.hammf.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kab.jianghu66.top

[U59] PHP：自定义排序
来源：http://vic.zhixingplan.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ilt.hongshengwenyu.top

[U60] PHP：JSON 编解码
来源：http://ogr.hywenlv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qoc.smart0.xyz

[U61] PHP：正则
来源：http://ryt.hfpthk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sdf.aizwys.cn

[U62] PHP：日期对象
来源：http://npm.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mdw.bjfxy.top

[U63] PHP：文件读写
来源：http://lic.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tng.nwbrower.top

[U64] PHP：目录遍历
来源：http://apn.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://ghe.uphjek.com

[U65] PHP：会话
来源：http://kiz.quarkkingdee.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ped.cucudq.cn

[U66] PHP：设置 Cookie
来源：http://bzv.zdqjudy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kwc.hesvh.cn

[U67] PHP：处理文件上传
来源：http://yce.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ijy.yangfankeji.com

[U68] PHP：PDO 连接
来源：http://tlh.xuetiantiany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://whg.shangyingyoupin.top

[U69] PHP：PDO 预处理
来源：http://icc.zhongyouzk.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jar.wangshuangyany.cn

[U70] PHP：PDO 事务
来源：http://uqs.aizwys.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://twm.jqgufenzy.top

[U71] PHP：抛出异常
来源：http://ilr.zdbjq.cn

throw new RuntimeException("失败", 500);
来源：http://dcg.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://qqq.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://brv.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://dsh.epnwcf.com

parse_ini_file("config.ini", true)
来源：http://vba.svipenyu.cn

[U74] PHP：读取环境变量
来源：http://oma.wangdashe.top

getenv("APP_ENV") ?: "production"
来源：http://hik.smart0.xyz

[U75] PHP：依赖注入
来源：http://ynb.havefunace.top

composer require psr/container
来源：http://lxm.epnwcf.com

[U76] PHP：简单路由
来源：http://lvl.xinyue.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tqo.ybcxt.top

[U77] PHP：模板渲染
来源：http://hkh.yvedp.cn

composer require twig/twig
来源：http://ekn.yonumen.top

[U78] PHP：单元测试
来源：http://ysq.cdnleiting.top

composer require --dev phpunit/phpunit
来源：http://hln.birdmap.top

[U79] PHP：静态分析
来源：http://die.nwbrower.top

composer require --dev phpstan/phpstan
来源：http://sco.meibo888.top

[U80] PHP：代码规范修复
来源：http://mqf.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sfb.yongpay.top

[U81] JS：初始化项目
来源：http://fhe.shzxlz.cn

npm init -y;  npm i express
来源：http://ikk.daria6918.cn

[U82] JS：package.json 脚本
来源：http://aqi.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dqo.tanke756.top

[U83] JS：ES Module 导入导出
来源：http://tnr.epnwcf.com

export const a = 1;  import { a } from "./m.js";
来源：http://urx.hysaishi.cn

[U84] JS：CommonJS 写法
来源：http://xvo.wangdashe.top

module.exports = { a };  const { a } = require("./m");
来源：http://aau.9152youxi.cn

[U85] JS：可选链
来源：http://bik.tian-w.cn

a?.b?.c
来源：http://fli.jinyuanbaomall.cn

[U86] JS：空值合并
来源：http://xeh.sufxvd.cn

a ?? b
来源：http://ldj.ybcxt.top

[U87] JS：解构默认值
来源：http://dpp.zhijiandao.cn

const { a = 1, b = 2 } = obj;
来源：http://ruw.yvedp.cn

[U88] JS：对象展开合并
来源：http://jsr.dashuyun.cn

{ ...a, ...b }
来源：http://elx.xinyue.icu

[U89] JS：数组去重
来源：http://msd.c1oappe.top

[...new Set(arr)]
来源：http://uzk.fktsv.cn

[U90] JS：数字数组排序
来源：http://glw.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://xgr.zhixingplan.top

[U91] JS：对象键值遍历
来源：http://rke.wangshuangyany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lya.bbcook.cn

[U92] JS：深拷贝
来源：http://mql.hammf.cn

structuredClone(obj)
来源：http://uvh.cheryme.top

[U93] JS：模板字符串
来源：http://vqo.hnqzz.top

`共 ${n} 条`
来源：http://wpe.zdbjq.cn

[U94] JS：箭头函数
来源：http://mmw.pycfn.com

const double = x => x * 2;
来源：http://ato.daria6918.cn

[U95] JS：Promise 包装
来源：http://tqb.zhaomingkeji.xyz

new Promise((resolve, reject) => {})
来源：http://rxl.zdqjudy.top

[U96] JS：async/await 与异常
来源：http://ndc.hammf.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ewp.zhaomingkeji.xyz

[U97] JS：并发请求
来源：http://pyf.sweek.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kbx.tianlin.xyz

[U98] JS：fetch 带 JSON
来源：http://xgv.havefunace.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xwb.fehbvm.com

[U99] JS：事件监听
来源：http://tvl.shanyushiyangkeji.top

el.addEventListener("click", e => {})
来源：http://lvd.gzhubu.top

[U100] JS：DOM 查询
来源：http://gyh.ydzc1.top

document.querySelector(".item")
来源：http://byc.tian-w.cn

[U101] JS：classList 操作
来源：http://ikl.yanxiufei.cn

el.classList.toggle("active")
来源：http://hsz.xuetiantiany.cn

[U102] JS：本地存储
来源：http://pwo.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hhf.hongshengwenyu.top

[U103] JS：定时器
来源：http://ofk.52xcode.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yhq.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://urp.zdbjq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://upz.ppjwa.cn

[U105] JS：节流
来源：http://gqv.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bfx.cucudq.cn

[U106] JS：日期格式化
来源：http://epy.gogol.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zfv.tarul.cn

[U107] JS：数字千分位
来源：http://vrt.tanke756.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://raj.ydjk.org.cn

[U108] JS：随机整数
来源：http://mvm.sweek.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kkw.quarkkingdee.top

[U109] JS：数组分组
来源：http://zpb.jinqigfzy.top

Object.groupBy(arr, x => x.type)
来源：http://ysc.yvedp.cn

[U110] JS：数组分块
来源：http://jso.quarkkingdee.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pqw.bjfxy.top

[U111] JS：对象转 Map
来源：http://vni.redwolf501.top

new Map(Object.entries(obj))
来源：http://yrh.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://zsm.uphjek.com

"7".padStart(3, "0")
来源：http://ndf.yongpay.top

[U113] JS：正则替换全部
来源：http://gek.wangshuangyany.cn

s.replaceAll("a", "b")
来源：http://kbc.yj20258888.top

[U114] JS：JSON 深比较
来源：http://rce.quarkkingdee.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://duf.vehdjk.com

[U115] JS：生成 UUID
来源：http://zbk.daria6918.cn

crypto.randomUUID()
来源：http://kfp.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://fiq.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://fnr.zhiwuduotai.top

[U117] JS：单元测试
来源：http://igo.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://xqy.nanxinkj.top

[U118] JS：开发服务器
来源：http://anj.jinqigufen.top

npm i -D vite;  npx vite
来源：http://yse.cqqwz.cn

[U119] JS：生产构建
来源：http://ftx.ivvv.top

npx vite build
来源：http://cgk.feifeiyinyue.top

[U120] JS：读取环境变量（Vite）
来源：http://gkp.cheryme.top

import.meta.env.VITE_API_URL
来源：http://ecn.tian-w.cn

================================================================================
来源：http://qbq.ywan-chungtsiang.top

统计汇总
来源：http://zru.fehbvm.com

================================================================================
来源：http://fez.c1oappe.top

按语言统计（条）：
来源：http://eqw.cqqwz.cn

Python ......... 252
来源：http://xga.jqgfzy.top

PHP ............ 252
来源：http://dxb.nanxinkj.top

JavaScript ..... 252
来源：http://vwe.svipenyu.cn

TypeScript ..... 212
来源：http://lzr.ydjk.org.cn

Java ........... 212
来源：http://jkd.hesvh.cn

Go ............. 212
来源：http://iac.xziqi.cn

Ruby ........... 212
来源：http://bbb.bjfxy.top

C# ............. 212
来源：http://ojq.haohaochexian.top

C .............. 30
来源：http://tgy.redwolf501.top

C++ ............ 30
来源：http://rzl.gogol.net.cn

SQL ............ 90
来源：http://ecv.guannengcc.top

Bash ........... 80
来源：http://bcu.cucudq.cn

Kotlin ......... 15
来源：http://blo.yanxiufei.cn

Swift .......... 15
来源：http://yhx.yj20258.top

Lua ............ 10
来源：http://wte.zdbjq.cn

Perl ........... 10
来源：http://pqn.yangfankeji.com

Scala .......... 10
来源：http://mmb.cashguo.top

------------------------------------
来源：http://wwk.c1oappe.top

合计 ........... 2106 条
来源：http://jiu.fengsongda.top

按章节统计：
来源：http://nlo.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://msb.jinghuilouyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ikk.fzhhl.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sfh.shanyushiyangtech.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gpf.xuetiantiany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pnu.yanxiufei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ouf.ehwqpu.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bbu.aibaodan.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ugk.sweek.top


<!-- 参考信息 -->