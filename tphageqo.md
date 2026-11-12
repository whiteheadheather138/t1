代发 wailian999

[T47] Perl：正则捕获
来源：http://cfh.guowangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fbv.zhengqikj.top

[T48] Perl：正则替换
来源：http://ngo.yongpay.top

$s =~ s/old/new/g;
来源：http://bkc.jqgufenzy.top

[T49] Perl：函数
来源：http://deo.chenjidiqi.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gvf.gaohongyu789.top

[T50] Perl：逐行读文件
来源：http://jdo.zdbjq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zgf.jiagoushi.top

while (my $line = <$fh>) { print $line; }
来源：http://xcv.nwbrower.top

[T51] Scala：Hello World
来源：http://vbw.chenjidiqi.icu

println("Hello")
来源：http://nxe.xuanzx.com

[T52] Scala：变量
来源：http://rbm.tianlin.xyz

val a = 1;  var b = 2
来源：http://pqm.yuxming.cn

[T53] Scala：字符串插值
来源：http://aba.jianghu66.top

s"值: $b"
来源：http://bag.jiagoushi.top

[T54] Scala：集合映射
来源：http://uxj.guowangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://ohk.guowangkeji.top

[T55] Scala：集合过滤
来源：http://eor.svipenyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pfj.meibo888.top

[T56] Scala：样例类
来源：http://hql.andypj.xyz

case class User(name: String, age: Int)
来源：http://wwi.snrcjt.cn

[T57] Scala：模式匹配
来源：http://zos.nwbrower.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fjm.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://mww.yuanzhike.top

def add(a: Int, b: Int): Int = a + b
来源：http://hdl.chenlongwang.top

[T59] Scala：循环
来源：http://llu.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://vvg.zhixingplan.top

[T60] Scala：折叠
来源：http://smw.ivvv.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ivn.jqgfzy.top

================================================================================
来源：http://teo.bbcook.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cwl.jlsjyb.cn

================================================================================
来源：http://syc.andypj.xyz

[U01] Py：创建虚拟环境
来源：http://ita.havefunace.top

python -m venv .venv && source .venv/bin/activate
来源：http://lsn.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://nkw.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://son.iojbl.cn

[U03] Py：加载 .env 配置
来源：http://zzv.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hxa.aibaodan.cn

[U04] Py：变量调试打印
来源：http://oth.fanxiaobao.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rut.uphjek.com

[U05] Py：列表去重且保序
来源：http://imx.jqgufenzy.top

list(dict.fromkeys(arr))
来源：http://chh.tian-w.cn

[U06] Py：合并两个字典
来源：http://idm.yj20258888.top

{**a, **b}
来源：http://jua.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://lsv.hysaishi.cn

{v: k for k, v in d.items()}
来源：http://djy.cucudq.cn

[U08] Py：展平二维列表
来源：http://vaf.fzhhl.top

[y for x in nested for y in x]
来源：http://jiy.yj20258888.top

[U09] Py：字典取最大值的键
来源：http://jwu.dashuyun.cn

max(d, key=d.get)
来源：http://dry.vqdsnc.cn

[U10] Py：按值排序字典
来源：http://zlm.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lcg.yj20258.top

[U11] Py：生成器表达式
来源：http://gee.shangyingyoupin.top

(x * 2 for x in arr)
来源：http://tow.gotoacloud.top

[U12] Py：取出现最多的 3 个元素
来源：http://nnp.jlsjyb.cn

Counter(arr).most_common(3)
来源：http://dbs.zdbjq.cn

[U13] Py：固定长度队列
来源：http://qsj.yj20258.top

deque(maxlen=10)
来源：http://jxc.hywenlv.cn

[U14] Py：分组收集到列表
来源：http://iit.nwbrower.top

defaultdict(list)
来源：http://tzu.sysykeji.top

[U15] Py：高精度计时
来源：http://lnu.chenjidiqi.icu

t = time.perf_counter()
来源：http://vbo.0kj1m.cn

[U16] Py：命令行参数解析
来源：http://eti.jqgfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fyh.aizwys.cn

[U17] Py：初始化日志
来源：http://fgx.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://ium.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://jrp.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://thx.yueranfly.top

[U19] Py：正则替换带回调
来源：http://tid.daxiang520.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sey.zhongyouzk.top

[U20] Py：缓存函数结果
来源：http://ral.havefunace.top

@functools.lru_cache(maxsize=None)
来源：http://sci.cqqwz.cn

[U21] Py：自定义上下文管理器
来源：http://fiu.xuanzx.com

@contextlib.contextmanager
来源：http://jpt.tianlin.xyz

[U22] Py：矩阵转置
来源：http://vlt.vqdsnc.cn

list(zip(*m))
来源：http://ksz.sxryk.cn

[U23] Py：分块读取大文件
来源：http://opi.quarkkingdee.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lfh.jianghu66.top

[U24] Py：路径操作
来源：http://eeb.tian-w.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://scv.birdmap.top

[U25] Py：CSV 按字典读
来源：http://rge.jinyuanbaomall.cn

csv.DictReader(f)
来源：http://ydz.ctjpmb.com

[U26] Py：并发下载
来源：http://fnl.andypj.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dcl.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://kwa.yj20258.top

aiohttp.ClientSession() 配合 async with
来源：http://pnr.epnwcf.com

[U28] Py：类型别名
来源：http://nzd.vehdjk.com

UserId = int
来源：http://pog.yj20258888.top

[U29] Py：属性校验
来源：http://kdg.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://yto.iojbl.cn

[U30] Py：数据类
来源：http://rkr.havefunace.top

@dataclass(slots=True)
来源：http://fsb.aizwys.cn

[U31] Py：单测
来源：http://rgw.fehbvm.com

python -m pytest -q
来源：http://uvd.hcnkem.com

[U32] Py：代码格式化
来源：http://lfd.316326.xyz

ruff format . && ruff check --fix .
来源：http://zxy.hysaishi.cn

[U33] Py：打包发布
来源：http://cul.cheryme.top

python -m build  （依赖 pyproject.toml）
来源：http://ong.daxiang520.top

[U34] Py：判断编码
来源：http://fah.c1oappe.top

chardet.detect(raw)
来源：http://ecn.cqqwz.cn

[U35] Py：发送邮件
来源：http://plt.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dzr.hfpthk.cn

[U36] Py：定时任务
来源：http://pol.cqqwz.cn

schedule.every(10).minutes.do(job)
来源：http://ctg.fengsongda.top

[U37] Py：读写 Excel
来源：http://ctq.daria6918.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cdd.andypj.xyz

[U38] Py：获取脚本所在目录
来源：http://inu.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://mgq.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://uta.xinyue.icu

sys.stdout.isatty()
来源：http://pal.zhijiandao.cn

[U40] Py：打印到标准错误
来源：http://xkc.gotoacloud.top

print("err", file=sys.stderr)
来源：http://zor.cdnleiting.top

[U41] PHP：初始化 Composer 项目
来源：http://gti.xylfe.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://faw.sweek.top

[U42] PHP：PSR-4 自动加载
来源：http://hvl.birdmap.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fut.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://tbq.hnqzz.top

namespace App\Http;
来源：http://aks.dianchejie.cn

[U44] PHP：开启严格类型
来源：http://gly.bbcook.cn

declare(strict_types=1);
来源：http://uzb.tian-w.cn

[U45] PHP：类型声明与返回类型
来源：http://yhi.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://tjq.cheryme.top

[U46] PHP：可空类型
来源：http://wxw.wangdashe.top

?string $name = null
来源：http://ijt.0kj1m.cn

[U47] PHP：联合类型
来源：http://dvu.ehwqpu.com

int|string $id
来源：http://rnf.havefunace.top

[U48] PHP：纯枚举
来源：http://nae.hammf.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://loa.yuxming.cn

[U49] PHP：只读属性
来源：http://zou.meibo888.top

public readonly string $name
来源：http://dnd.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://bxn.sweek.top

public function __construct(private int $id) {}
来源：http://lyp.yanxiufei.cn

[U51] PHP：数组解构
来源：http://pmf.sxryk.cn

[$a, $b] = $arr;
来源：http://vwc.dashuyun.cn

[U52] PHP：箭头函数
来源：http://vic.quarkkingdee.top

$double = fn($x) => $x * 2;
来源：http://nbr.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://udv.jinqigufen.top

$v = $a ?? $b ?? "default";
来源：http://sds.shangyingyoupin.top

[U54] PHP：空安全调用
来源：http://vif.yj20258888.top

$obj?->method()
来源：http://ysy.yanxiufei.cn

[U55] PHP：match 表达式
来源：http://ygy.ydzc1.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vvp.zhaomingkeji.xyz

[U56] PHP：命名参数
来源：http://uer.svipenyu.cn

f(a: 1, b: 2)
来源：http://ygp.gotoacloud.top

[U57] PHP：字符串插值
来源：http://kzf.cashguo.top

"值: {$a}"
来源：http://gea.guowangkeji.top

[U58] PHP：数组三件套
来源：http://krx.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hus.ydzc1.top

[U59] PHP：自定义排序
来源：http://yat.chenjidiqi.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ljz.jinqigufen.top

[U60] PHP：JSON 编解码
来源：http://ahv.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mhc.zhijiandao.cn

[U61] PHP：正则
来源：http://lax.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zqf.chenzaomai.com

[U62] PHP：日期对象
来源：http://yxt.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wxm.jqgufenzy.top

[U63] PHP：文件读写
来源：http://uwg.zhoulong.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qjf.yongpay.top

[U64] PHP：目录遍历
来源：http://pjk.bbcook.cn

glob("dir/*.php");  scandir("dir");
来源：http://czj.316326.xyz

[U65] PHP：会话
来源：http://rdr.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ihn.shanyushiyangkeji.top

[U66] PHP：设置 Cookie
来源：http://wxe.andypj.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pxy.jinghuilouyu.cn

[U67] PHP：处理文件上传
来源：http://dzh.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gdf.svipenyu.cn

[U68] PHP：PDO 连接
来源：http://llu.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eux.kuanghao11.cn

[U69] PHP：PDO 预处理
来源：http://mzs.yj20258.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zzx.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://dnv.shzxlz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vhu.chenlongwang.top

[U71] PHP：抛出异常
来源：http://fsl.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://fxq.yonumen.top

[U72] PHP：写错误日志
来源：http://cky.vehdjk.com

error_log("失败: " . $e->getMessage());
来源：http://yqv.jianghu66.top

[U73] PHP：读取 ini 配置
来源：http://xoe.sweek.top

parse_ini_file("config.ini", true)
来源：http://vor.9152youxi.cn

[U74] PHP：读取环境变量
来源：http://vao.haohaochexian.top

getenv("APP_ENV") ?: "production"
来源：http://ugo.guowangkeji.top

[U75] PHP：依赖注入
来源：http://ivm.bbcook.cn

composer require psr/container
来源：http://fie.yonumen.top

[U76] PHP：简单路由
来源：http://frr.hnxiangtu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fwk.epnwcf.com

[U77] PHP：模板渲染
来源：http://iho.c1oappe.top

composer require twig/twig
来源：http://tqu.zdbjq.cn

[U78] PHP：单元测试
来源：http://iwp.gotoacloud.top

composer require --dev phpunit/phpunit
来源：http://unb.xinyue.icu

[U79] PHP：静态分析
来源：http://qbk.wangdashe.top

composer require --dev phpstan/phpstan
来源：http://tfh.xziqi.cn

[U80] PHP：代码规范修复
来源：http://nol.yongpay.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://cgm.chenjidiqi.icu

[U81] JS：初始化项目
来源：http://rhk.yueranfly.top

npm init -y;  npm i express
来源：http://yla.xuanzx.com

[U82] JS：package.json 脚本
来源：http://ddr.hysaishi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ayk.sufxvd.cn

[U83] JS：ES Module 导入导出
来源：http://bsc.yueranfly.top

export const a = 1;  import { a } from "./m.js";
来源：http://yto.ehwqpu.com

[U84] JS：CommonJS 写法
来源：http://zuq.fengsongda.top

module.exports = { a };  const { a } = require("./m");
来源：http://jhl.fktsv.cn

[U85] JS：可选链
来源：http://xxs.ydjk.org.cn

a?.b?.c
来源：http://fts.chenlongwang.top

[U86] JS：空值合并
来源：http://ypf.daria6918.cn

a ?? b
来源：http://ryy.tarul.cn

[U87] JS：解构默认值
来源：http://tnc.sjlbkw.cn

const { a = 1, b = 2 } = obj;
来源：http://nec.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://ejo.snrcjt.cn

{ ...a, ...b }
来源：http://mjt.pycfn.com

[U89] JS：数组去重
来源：http://pnn.shzxlz.cn

[...new Set(arr)]
来源：http://oti.cashguo.top

[U90] JS：数字数组排序
来源：http://raz.chenjidiqi.icu

[...arr].sort((a, b) => a - b)
来源：http://lpt.nanxuanxn.top

[U91] JS：对象键值遍历
来源：http://pzn.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ftc.yj202588.top

[U92] JS：深拷贝
来源：http://fln.sysykeji.top

structuredClone(obj)
来源：http://lek.zhongyouzk.top

[U93] JS：模板字符串
来源：http://ibc.hcnkem.com

`共 ${n} 条`
来源：http://fht.dianchejie.cn

[U94] JS：箭头函数
来源：http://qky.fehbvm.com

const double = x => x * 2;
来源：http://wbu.nwbrower.top

[U95] JS：Promise 包装
来源：http://ewc.vqdsnc.cn

new Promise((resolve, reject) => {})
来源：http://bes.guannengcc.top

[U96] JS：async/await 与异常
来源：http://yif.ydzc1.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xrl.yanxiufei.cn

[U97] JS：并发请求
来源：http://svc.tanke756.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qju.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://hop.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dnt.nwbrower.top

[U99] JS：事件监听
来源：http://unc.316326.xyz

el.addEventListener("click", e => {})
来源：http://lht.gotoacloud.top

[U100] JS：DOM 查询
来源：http://oeo.zhoulong.xyz

document.querySelector(".item")
来源：http://vdt.bjfxy.top

[U101] JS：classList 操作
来源：http://ngz.haohaochexian.top

el.classList.toggle("active")
来源：http://qbi.hcnkem.com

[U102] JS：本地存储
来源：http://ejw.jiagoushi.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pqc.sxryk.cn

[U103] JS：定时器
来源：http://njr.yongpay.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ipy.smart0.xyz

[U104] JS：防抖
来源：http://blz.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://net.gzhubu.top

[U105] JS：节流
来源：http://aii.hnxiangtu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wat.zhixingplan.top

[U106] JS：日期格式化
来源：http://adi.gogol.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lnm.xylfe.cn

[U107] JS：数字千分位
来源：http://lvz.shanyushiyangtech.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://axn.meibo888.top

[U108] JS：随机整数
来源：http://yhd.fehbvm.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dia.tian-w.cn

[U109] JS：数组分组
来源：http://qzp.nwbrower.top

Object.groupBy(arr, x => x.type)
来源：http://szt.jqgufenzy.top

[U110] JS：数组分块
来源：http://xfz.shangyingyoupin.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://van.daxiang520.top

[U111] JS：对象转 Map
来源：http://mpb.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://bba.zhoulong.xyz

[U112] JS：字符串补位
来源：http://wpt.zdbjq.cn

"7".padStart(3, "0")
来源：http://vdm.tarul.cn

[U113] JS：正则替换全部
来源：http://bhi.ybcxt.top

s.replaceAll("a", "b")
来源：http://itd.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://ztf.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://coy.ydjk.org.cn

[U115] JS：生成 UUID
来源：http://oyq.zhixingplan.top

crypto.randomUUID()
来源：http://cxt.yonumen.top

[U116] JS：类型检查（JSDoc）
来源：http://djm.jinqigfzy.top

/** @param {string} name */ function f(name) {}
来源：http://wot.snrcjt.cn

[U117] JS：单元测试
来源：http://chy.tanke756.top

npm i -D vitest;  npx vitest
来源：http://qxe.tarul.cn

[U118] JS：开发服务器
来源：http://udq.xingfuxueyuan.xyz

npm i -D vite;  npx vite
来源：http://bhy.zycfv.cn

[U119] JS：生产构建
来源：http://lqp.zdbjq.cn

npx vite build
来源：http://pbc.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://eqs.pengpengdd.cyou

import.meta.env.VITE_API_URL
来源：http://ppj.xylfe.cn

================================================================================
来源：http://tbz.mhx1999.top

统计汇总
来源：http://zoi.zdqjudy.top

================================================================================
来源：http://ojt.nanxinkj.top

按语言统计（条）：
来源：http://qem.andypj.xyz

Python ......... 252
来源：http://jfy.ehwqpu.com

PHP ............ 252
来源：http://trs.cdnleiting.top

JavaScript ..... 252
来源：http://xpr.jinyuanbaomall.cn

TypeScript ..... 212
来源：http://lis.gotoacloud.top

Java ........... 212
来源：http://nvn.cqqwz.cn

Go ............. 212
来源：http://xbs.xylfe.cn

Ruby ........... 212
来源：http://ndn.jiagoushi.top

C# ............. 212
来源：http://lgk.yj20258888.top

C .............. 30
来源：http://ilf.hnqzz.top

C++ ............ 30
来源：http://upx.daria6918.cn

SQL ............ 90
来源：http://cgr.snrcjt.cn

Bash ........... 80
来源：http://zdh.nanxuanxn.top

Kotlin ......... 15
来源：http://ktd.fktsv.cn

Swift .......... 15
来源：http://oaz.hnxiangtu.top

Lua ............ 10
来源：http://urm.zhoulong.xyz

Perl ........... 10
来源：http://cka.ywan-chungtsiang.top

Scala .......... 10
来源：http://ijs.zhixingplan.top

------------------------------------
来源：http://qbq.quarkkingdee.top

合计 ........... 2106 条
来源：http://iky.yonumen.top

按章节统计：
来源：http://rit.shuidangran.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://knn.chenzaomai.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uqt.jinyuanbaomall.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ynd.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xao.andypj.xyz


<!-- 参考信息 -->