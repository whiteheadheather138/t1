代发 wailian999

[T45] Perl：数组遍历
来源：http://tsr.zycfv.cn

for my $x (@arr) { print $x; }
来源：http://auf.9152youxi.cn

[T46] Perl：哈希操作
来源：http://shn.ydjk.org.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jix.ivvv.top

[T47] Perl：正则捕获
来源：http://qia.cashguo.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xyj.sjlbkw.cn

[T48] Perl：正则替换
来源：http://ukw.tian-w.cn

$s =~ s/old/new/g;
来源：http://qfo.yvedp.cn

[T49] Perl：函数
来源：http://tqx.pengpengdd.cyou

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://puf.ehwqpu.com

[T50] Perl：逐行读文件
来源：http://hyj.daria6918.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rhn.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://dfn.fzhhl.top

[T51] Scala：Hello World
来源：http://tsj.sweek.top

println("Hello")
来源：http://ert.jianghu66.top

[T52] Scala：变量
来源：http://cfx.yuxming.cn

val a = 1;  var b = 2
来源：http://uee.cheryme.top

[T53] Scala：字符串插值
来源：http://iag.yonumen.top

s"值: $b"
来源：http://tcg.sxryk.cn

[T54] Scala：集合映射
来源：http://oeq.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://pvu.hcnkem.com

[T55] Scala：集合过滤
来源：http://jpi.zhongyouzk.top

List(1, 2, 3).filter(_ > 1)
来源：http://sbw.uphjek.com

[T56] Scala：样例类
来源：http://vqg.nanxuanxn.top

case class User(name: String, age: Int)
来源：http://wlb.ydjk.org.cn

[T57] Scala：模式匹配
来源：http://lse.tian-w.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ptw.sxryk.cn

[T58] Scala：函数定义
来源：http://tvr.aizwys.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wpw.sufxvd.cn

[T59] Scala：循环
来源：http://qvr.gotoacloud.top

for (i <- 1 to 10) println(i)
来源：http://zvf.tian-w.cn

[T60] Scala：折叠
来源：http://pcc.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qdx.nanxinkj.top

================================================================================
来源：http://bki.cdnleiting.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gsm.shanyushiyangkeji.top

================================================================================
来源：http://tkg.jinghuilouyu.cn

[U01] Py：创建虚拟环境
来源：http://imw.yuxming.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lkl.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://jqj.zhongyouzk.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ypl.hywenlv.cn

[U03] Py：加载 .env 配置
来源：http://hsu.yj20258.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jsk.meibo888.top

[U04] Py：变量调试打印
来源：http://djp.yj20258.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://maq.haohaochexian.top

[U05] Py：列表去重且保序
来源：http://utk.ehwqpu.com

list(dict.fromkeys(arr))
来源：http://mjl.316326.xyz

[U06] Py：合并两个字典
来源：http://uyu.aizwys.cn

{**a, **b}
来源：http://kye.bbcook.cn

[U07] Py：反转字典键值
来源：http://ozp.smart0.xyz

{v: k for k, v in d.items()}
来源：http://gmx.shangyingyoupin.top

[U08] Py：展平二维列表
来源：http://tew.havefunace.top

[y for x in nested for y in x]
来源：http://jez.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://wwr.fehbvm.com

max(d, key=d.get)
来源：http://pqt.c1oappe.top

[U10] Py：按值排序字典
来源：http://mqa.zhongyouzk.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rig.havefunace.top

[U11] Py：生成器表达式
来源：http://gar.svipenyu.cn

(x * 2 for x in arr)
来源：http://wzr.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qyp.mhx1999.top

Counter(arr).most_common(3)
来源：http://niy.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://ese.sxryk.cn

deque(maxlen=10)
来源：http://ibn.yuxming.cn

[U14] Py：分组收集到列表
来源：http://dfl.gaohongyu789.top

defaultdict(list)
来源：http://sim.xziqi.cn

[U15] Py：高精度计时
来源：http://cwi.jiagoushi.top

t = time.perf_counter()
来源：http://ogf.smart0.xyz

[U16] Py：命令行参数解析
来源：http://cbl.xingfuxueyuan.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lqo.fktsv.cn

[U17] Py：初始化日志
来源：http://lyb.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://fdp.316326.xyz

[U18] Py：预编译正则
来源：http://eut.bjfxy.top

pat = re.compile(r"\d+")
来源：http://qis.hywenlv.cn

[U19] Py：正则替换带回调
来源：http://irp.yanxiufei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://liy.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://nfk.gzhubu.top

@functools.lru_cache(maxsize=None)
来源：http://fbz.ybcxt.top

[U21] Py：自定义上下文管理器
来源：http://dke.52xcode.cn

@contextlib.contextmanager
来源：http://oer.cashguo.top

[U22] Py：矩阵转置
来源：http://ldy.andypj.xyz

list(zip(*m))
来源：http://vfl.fktsv.cn

[U23] Py：分块读取大文件
来源：http://dsu.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jom.uphjek.com

[U24] Py：路径操作
来源：http://fgf.xziqi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cio.jinqigufen.top

[U25] Py：CSV 按字典读
来源：http://rfi.zdbjq.cn

csv.DictReader(f)
来源：http://ulb.cashguo.top

[U26] Py：并发下载
来源：http://zrc.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pcn.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://lvl.hcnkem.com

aiohttp.ClientSession() 配合 async with
来源：http://bez.tian-w.cn

[U28] Py：类型别名
来源：http://zqb.xinyue.icu

UserId = int
来源：http://qen.zhiwuduotai.top

[U29] Py：属性校验
来源：http://kur.gzhubu.top

@property 与 @x.setter 配合
来源：http://oac.zdqjudy.top

[U30] Py：数据类
来源：http://ggv.tian-w.cn

@dataclass(slots=True)
来源：http://opk.hysaishi.cn

[U31] Py：单测
来源：http://rwv.jqgfzy.top

python -m pytest -q
来源：http://rke.ivvv.top

[U32] Py：代码格式化
来源：http://clv.guannengcc.top

ruff format . && ruff check --fix .
来源：http://xyo.mhx1999.top

[U33] Py：打包发布
来源：http://uqx.chenjidiqi.icu

python -m build  （依赖 pyproject.toml）
来源：http://buy.wangshuangyany.cn

[U34] Py：判断编码
来源：http://tab.shanyushiyangkeji.top

chardet.detect(raw)
来源：http://gea.cashguo.top

[U35] Py：发送邮件
来源：http://zoc.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pas.bbcook.cn

[U36] Py：定时任务
来源：http://sly.ybcxt.top

schedule.every(10).minutes.do(job)
来源：http://xiv.fanxiaobao.xyz

[U37] Py：读写 Excel
来源：http://vju.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://lgg.hcnkem.com

[U38] Py：获取脚本所在目录
来源：http://eqe.wangshuangyany.cn

Path(__file__).resolve().parent
来源：http://ghk.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://blv.hongshengwenyu.top

sys.stdout.isatty()
来源：http://cvv.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://yaj.cqqwz.cn

print("err", file=sys.stderr)
来源：http://cgm.xuetiantiany.cn

[U41] PHP：初始化 Composer 项目
来源：http://fhp.fzhhl.top

composer init;  composer require guzzlehttp/guzzle
来源：http://hdi.yj20258888.top

[U42] PHP：PSR-4 自动加载
来源：http://irg.aizwys.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xeo.nanxuanxn.top

[U43] PHP：声明命名空间
来源：http://ozb.c1oappe.top

namespace App\Http;
来源：http://qqr.zhijiandao.cn

[U44] PHP：开启严格类型
来源：http://gli.jqgfzy.top

declare(strict_types=1);
来源：http://mgm.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://cbc.nwbrower.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ypm.haohaochexian.top

[U46] PHP：可空类型
来源：http://zxg.bbcook.cn

?string $name = null
来源：http://mwx.birdmap.top

[U47] PHP：联合类型
来源：http://nbk.zhijiandao.cn

int|string $id
来源：http://oyz.bjfxy.top

[U48] PHP：纯枚举
来源：http://cqp.52xcode.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pxw.iojbl.cn

[U49] PHP：只读属性
来源：http://cxg.uphjek.com

public readonly string $name
来源：http://mmw.nanxuanxn.top

[U50] PHP：构造器属性提升
来源：http://qvp.c1oappe.top

public function __construct(private int $id) {}
来源：http://qeb.hnqzz.top

[U51] PHP：数组解构
来源：http://zbd.xylfe.cn

[$a, $b] = $arr;
来源：http://mxa.316326.xyz

[U52] PHP：箭头函数
来源：http://hzk.redwolf501.top

$double = fn($x) => $x * 2;
来源：http://nyd.bbcook.cn

[U53] PHP：空合并运算符
来源：http://cto.hnxiangtu.top

$v = $a ?? $b ?? "default";
来源：http://ewh.cdnleiting.top

[U54] PHP：空安全调用
来源：http://vkb.daria6918.cn

$obj?->method()
来源：http://ajg.hysaishi.cn

[U55] PHP：match 表达式
来源：http://dzj.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vqi.cashguo.top

[U56] PHP：命名参数
来源：http://gaq.shanyushiyangkeji.top

f(a: 1, b: 2)
来源：http://mqn.c1oappe.top

[U57] PHP：字符串插值
来源：http://uwb.guannengcc.top

"值: {$a}"
来源：http://phe.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://hwt.ctjpmb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://geb.pengpengdd.cyou

[U59] PHP：自定义排序
来源：http://ctr.bbcook.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zrl.sweek.top

[U60] PHP：JSON 编解码
来源：http://yes.gzhubu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://idg.zycfv.cn

[U61] PHP：正则
来源：http://sqi.chenzaomai.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zoo.dashuyun.cn

[U62] PHP：日期对象
来源：http://zoy.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tkh.c1oappe.top

[U63] PHP：文件读写
来源：http://pti.jinqigufen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://efc.daxiang520.top

[U64] PHP：目录遍历
来源：http://omd.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://ise.andypj.xyz

[U65] PHP：会话
来源：http://sbj.xylfe.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hjf.vehdjk.com

[U66] PHP：设置 Cookie
来源：http://jhw.hongshengwenyu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://epn.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://ntn.ybcxt.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jbi.daria6918.cn

[U68] PHP：PDO 连接
来源：http://dru.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pae.guowangkeji.top

[U69] PHP：PDO 预处理
来源：http://efg.aibaodan.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://stv.gzhubu.top

[U70] PHP：PDO 事务
来源：http://jpx.zdbjq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lxi.yonumen.top

[U71] PHP：抛出异常
来源：http://hyo.shanyushiyangtech.top

throw new RuntimeException("失败", 500);
来源：http://tit.havefunace.top

[U72] PHP：写错误日志
来源：http://ury.redwolf501.top

error_log("失败: " . $e->getMessage());
来源：http://ekf.pengpengdd.cyou

[U73] PHP：读取 ini 配置
来源：http://lvd.cheryme.top

parse_ini_file("config.ini", true)
来源：http://bzm.yanxiufei.cn

[U74] PHP：读取环境变量
来源：http://cqu.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://zbz.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://tzw.smart0.xyz

composer require psr/container
来源：http://bxn.jqgfzy.top

[U76] PHP：简单路由
来源：http://wvd.yangfankeji.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ykb.sxryk.cn

[U77] PHP：模板渲染
来源：http://jit.hongshengwenyu.top

composer require twig/twig
来源：http://ncu.jianghu66.top

[U78] PHP：单元测试
来源：http://xym.wangdashe.top

composer require --dev phpunit/phpunit
来源：http://gjc.9152youxi.cn

[U79] PHP：静态分析
来源：http://ybp.xinyue.icu

composer require --dev phpstan/phpstan
来源：http://kzc.epnwcf.com

[U80] PHP：代码规范修复
来源：http://xsf.fanxiaobao.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://tfd.daria6918.cn

[U81] JS：初始化项目
来源：http://kge.iojbl.cn

npm init -y;  npm i express
来源：http://zpu.52xcode.cn

[U82] JS：package.json 脚本
来源：http://zox.wangdashe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ign.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://xjo.zdqjudy.top

export const a = 1;  import { a } from "./m.js";
来源：http://vgq.shzxlz.cn

[U84] JS：CommonJS 写法
来源：http://ztv.zdqjudy.top

module.exports = { a };  const { a } = require("./m");
来源：http://dxb.hongshengwenyu.top

[U85] JS：可选链
来源：http://rez.jyoumei.cn

a?.b?.c
来源：http://xiz.sjlbkw.cn

[U86] JS：空值合并
来源：http://rou.316326.xyz

a ?? b
来源：http://zni.andypj.xyz

[U87] JS：解构默认值
来源：http://zzg.ybcxt.top

const { a = 1, b = 2 } = obj;
来源：http://xud.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://smb.0kj1m.cn

{ ...a, ...b }
来源：http://mqf.bbcook.cn

[U89] JS：数组去重
来源：http://xrz.smart0.xyz

[...new Set(arr)]
来源：http://vpr.sweek.top

[U90] JS：数字数组排序
来源：http://hws.yanxiufei.cn

[...arr].sort((a, b) => a - b)
来源：http://vpw.haohaochexian.top

[U91] JS：对象键值遍历
来源：http://blj.kuanghao11.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pvg.yfazqb.com

[U92] JS：深拷贝
来源：http://vse.cdnleiting.top

structuredClone(obj)
来源：http://ord.sufxvd.cn

[U93] JS：模板字符串
来源：http://rsp.jlsjyb.cn

`共 ${n} 条`
来源：http://gpv.zdbjq.cn

[U94] JS：箭头函数
来源：http://euv.andypj.xyz

const double = x => x * 2;
来源：http://zta.nanxuanxn.top

[U95] JS：Promise 包装
来源：http://xjd.ybcxt.top

new Promise((resolve, reject) => {})
来源：http://bsc.yonumen.top

[U96] JS：async/await 与异常
来源：http://fxn.ydzc1.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wwb.bbcook.cn

[U97] JS：并发请求
来源：http://okr.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jop.sysykeji.top

[U98] JS：fetch 带 JSON
来源：http://iva.c1oappe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ucn.xuetiantiany.cn

[U99] JS：事件监听
来源：http://ueo.bjfxy.top

el.addEventListener("click", e => {})
来源：http://xwb.yueranfly.top

[U100] JS：DOM 查询
来源：http://mpl.epnwcf.com

document.querySelector(".item")
来源：http://rdf.zhoulong.xyz

[U101] JS：classList 操作
来源：http://xdx.jlsjyb.cn

el.classList.toggle("active")
来源：http://ixf.shuidangran.top

[U102] JS：本地存储
来源：http://yld.gzhubu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kvp.yj202588.top

[U103] JS：定时器
来源：http://uic.smart0.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hiw.zhixingplan.top

[U104] JS：防抖
来源：http://fgc.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sfc.jinghuilouyu.cn

[U105] JS：节流
来源：http://xkr.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hek.xziqi.cn

[U106] JS：日期格式化
来源：http://ogt.cucudq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bsv.nwbrower.top

[U107] JS：数字千分位
来源：http://ivl.zdbjq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://moy.guowangkeji.top

[U108] JS：随机整数
来源：http://zan.yj20258.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xhv.vehdjk.com

[U109] JS：数组分组
来源：http://vio.xuanzx.com

Object.groupBy(arr, x => x.type)
来源：http://zjl.jqgufenzy.top

[U110] JS：数组分块
来源：http://yml.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lax.ehwqpu.com

[U111] JS：对象转 Map
来源：http://sod.tarul.cn

new Map(Object.entries(obj))
来源：http://bql.epnwcf.com

[U112] JS：字符串补位
来源：http://lqj.nanxinkj.top

"7".padStart(3, "0")
来源：http://hey.zhongyouzk.top

[U113] JS：正则替换全部
来源：http://ckv.zycfv.cn

s.replaceAll("a", "b")
来源：http://oly.xziqi.cn

[U114] JS：JSON 深比较
来源：http://srj.ywan-chungtsiang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wkh.smart0.xyz

[U115] JS：生成 UUID
来源：http://gdz.zhijiandao.cn

crypto.randomUUID()
来源：http://goy.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://iik.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://htv.smart0.xyz

[U117] JS：单元测试
来源：http://yny.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://wzb.yuanzhike.top

[U118] JS：开发服务器
来源：http://beo.ctjpmb.com

npm i -D vite;  npx vite
来源：http://lee.yanxiufei.cn

[U119] JS：生产构建
来源：http://hsv.hcnkem.com

npx vite build
来源：http://kcl.zhixingplan.top

[U120] JS：读取环境变量（Vite）
来源：http://bqj.hesvh.cn

import.meta.env.VITE_API_URL
来源：http://blv.shuidangran.top

================================================================================
来源：http://iuo.c1oappe.top

统计汇总
来源：http://yry.feifeiyinyue.top

================================================================================
来源：http://hsr.mhx1999.top

按语言统计（条）：
来源：http://twb.hammf.cn

Python ......... 252
来源：http://nwt.hongshengwenyu.top

PHP ............ 252
来源：http://hbs.vehdjk.com

JavaScript ..... 252
来源：http://lbr.tarul.cn

TypeScript ..... 212
来源：http://cyq.chenjidiqi.icu

Java ........... 212
来源：http://rvf.gotoacloud.top

Go ............. 212
来源：http://dzy.xinyue.icu

Ruby ........... 212
来源：http://bdd.ydjk.org.cn

C# ............. 212
来源：http://ibj.52xcode.cn

C .............. 30
来源：http://dyw.nwbrower.top

C++ ............ 30
来源：http://vil.meibo888.top

SQL ............ 90
来源：http://ufv.chenlongwang.top

Bash ........... 80
来源：http://hok.ydzc1.top

Kotlin ......... 15
来源：http://ync.chenlongwang.top

Swift .......... 15
来源：http://nic.jqgfzy.top

Lua ............ 10
来源：http://gfj.tarul.cn

Perl ........... 10
来源：http://hto.gaohongyu789.top

Scala .......... 10
来源：http://cfh.tianlin.xyz

------------------------------------
来源：http://qls.zhongyouzk.top

合计 ........... 2106 条
来源：http://wpq.hnxiangtu.top

按章节统计：
来源：http://tkq.yongpay.top


<!-- 参考信息 -->