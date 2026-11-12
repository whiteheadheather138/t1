代发 wailian999

[T45] Perl：数组遍历
来源：http://mzl.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://ufy.chenlongwang.top

[T46] Perl：哈希操作
来源：http://wca.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kti.kuanghao11.cn

[T47] Perl：正则捕获
来源：http://ohk.bjfxy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ypz.yj20258.top

[T48] Perl：正则替换
来源：http://nfz.yuxming.cn

$s =~ s/old/new/g;
来源：http://puf.sysykeji.top

[T49] Perl：函数
来源：http://ymb.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zmy.9152youxi.cn

[T50] Perl：逐行读文件
来源：http://jgx.hfpthk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xkz.aizwys.cn

while (my $line = <$fh>) { print $line; }
来源：http://kfe.jyoumei.cn

[T51] Scala：Hello World
来源：http://rwy.sxryk.cn

println("Hello")
来源：http://haq.meibo888.top

[T52] Scala：变量
来源：http://jje.sxryk.cn

val a = 1;  var b = 2
来源：http://fnf.daxiang520.top

[T53] Scala：字符串插值
来源：http://tbw.guannengcc.top

s"值: $b"
来源：http://jdz.aizwys.cn

[T54] Scala：集合映射
来源：http://men.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://ydb.gzhubu.top

[T55] Scala：集合过滤
来源：http://prx.fktsv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bkj.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://ctf.vqdsnc.cn

case class User(name: String, age: Int)
来源：http://owi.pycfn.com

[T57] Scala：模式匹配
来源：http://krq.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ngg.uphjek.com

[T58] Scala：函数定义
来源：http://jmv.hongshengwenyu.top

def add(a: Int, b: Int): Int = a + b
来源：http://isp.gogol.net.cn

[T59] Scala：循环
来源：http://mkx.nwbrower.top

for (i <- 1 to 10) println(i)
来源：http://jev.316326.xyz

[T60] Scala：折叠
来源：http://xqp.sysykeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yho.bjfxy.top

================================================================================
来源：http://yxn.jqgufenzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ndp.xinyue.icu

================================================================================
来源：http://svx.shuidangran.top

[U01] Py：创建虚拟环境
来源：http://icb.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://grr.hywenlv.cn

[U02] Py：导出 / 安装依赖
来源：http://kob.cheryme.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ibg.jinghuilouyu.cn

[U03] Py：加载 .env 配置
来源：http://ofc.fengsongda.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zmt.smart0.xyz

[U04] Py：变量调试打印
来源：http://cdf.epnwcf.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mvh.guowangkeji.top

[U05] Py：列表去重且保序
来源：http://xid.nanxuanxn.top

list(dict.fromkeys(arr))
来源：http://slb.chenlongwang.top

[U06] Py：合并两个字典
来源：http://jty.ywan-chungtsiang.top

{**a, **b}
来源：http://srr.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://vdz.aizwys.cn

{v: k for k, v in d.items()}
来源：http://xrs.sweek.top

[U08] Py：展平二维列表
来源：http://fzo.0kj1m.cn

[y for x in nested for y in x]
来源：http://nrx.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://ilk.yonumen.top

max(d, key=d.get)
来源：http://pow.chenjidiqi.icu

[U10] Py：按值排序字典
来源：http://cww.fktsv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fps.mhx1999.top

[U11] Py：生成器表达式
来源：http://qoi.mhx1999.top

(x * 2 for x in arr)
来源：http://yzx.chenjidiqi.icu

[U12] Py：取出现最多的 3 个元素
来源：http://syy.yj20258.top

Counter(arr).most_common(3)
来源：http://jex.hammf.cn

[U13] Py：固定长度队列
来源：http://uyj.daxiang520.top

deque(maxlen=10)
来源：http://lew.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://jed.sweek.top

defaultdict(list)
来源：http://atd.mhx1999.top

[U15] Py：高精度计时
来源：http://utm.316326.xyz

t = time.perf_counter()
来源：http://vso.shuidangran.top

[U16] Py：命令行参数解析
来源：http://xgd.snrcjt.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ehv.ydjk.org.cn

[U17] Py：初始化日志
来源：http://uhd.52xcode.cn

logging.basicConfig(level=logging.INFO)
来源：http://hqe.tanke756.top

[U18] Py：预编译正则
来源：http://smc.c1oappe.top

pat = re.compile(r"\d+")
来源：http://ekv.kuanghao11.cn

[U19] Py：正则替换带回调
来源：http://exw.9152youxi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qmd.yanxiufei.cn

[U20] Py：缓存函数结果
来源：http://tnv.chenlongwang.top

@functools.lru_cache(maxsize=None)
来源：http://wrs.jiagoushi.top

[U21] Py：自定义上下文管理器
来源：http://tuy.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://qfp.kuanghao11.cn

[U22] Py：矩阵转置
来源：http://dcw.yj20258.top

list(zip(*m))
来源：http://iqk.smart0.xyz

[U23] Py：分块读取大文件
来源：http://hue.aizwys.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ksm.pengpengdd.cyou

[U24] Py：路径操作
来源：http://kwq.iojbl.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ykn.jyoumei.cn

[U25] Py：CSV 按字典读
来源：http://eja.quarkkingdee.top

csv.DictReader(f)
来源：http://dzs.52xcode.cn

[U26] Py：并发下载
来源：http://pra.nanxinkj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bcq.yj20258.top

[U27] Py：异步 HTTP
来源：http://obh.yvedp.cn

aiohttp.ClientSession() 配合 async with
来源：http://zoe.yuanzhike.top

[U28] Py：类型别名
来源：http://zym.hysaishi.cn

UserId = int
来源：http://nrv.vehdjk.com

[U29] Py：属性校验
来源：http://thh.gotoacloud.top

@property 与 @x.setter 配合
来源：http://tgy.fanxiaobao.xyz

[U30] Py：数据类
来源：http://esb.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://wac.fktsv.cn

[U31] Py：单测
来源：http://kji.xinyue.icu

python -m pytest -q
来源：http://umi.ppjwa.cn

[U32] Py：代码格式化
来源：http://bpy.ydzc1.top

ruff format . && ruff check --fix .
来源：http://yhj.fehbvm.com

[U33] Py：打包发布
来源：http://vxv.cqqwz.cn

python -m build  （依赖 pyproject.toml）
来源：http://mmr.havefunace.top

[U34] Py：判断编码
来源：http://hlw.xinyue.icu

chardet.detect(raw)
来源：http://pma.hnqzz.top

[U35] Py：发送邮件
来源：http://thi.daxiang520.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uhm.jiagoushi.top

[U36] Py：定时任务
来源：http://qza.jyoumei.cn

schedule.every(10).minutes.do(job)
来源：http://mpx.yj20258888.top

[U37] Py：读写 Excel
来源：http://xnq.guowangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://zde.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://voq.gotoacloud.top

Path(__file__).resolve().parent
来源：http://anv.chenzaomai.com

[U39] Py：判断是否在交互环境
来源：http://bfw.sxryk.cn

sys.stdout.isatty()
来源：http://qgd.jianghu66.top

[U40] Py：打印到标准错误
来源：http://mca.tianlin.xyz

print("err", file=sys.stderr)
来源：http://chi.yueranfly.top

[U41] PHP：初始化 Composer 项目
来源：http://dyz.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://eml.cdnleiting.top

[U42] PHP：PSR-4 自动加载
来源：http://twk.tarul.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://glu.zhixingplan.top

[U43] PHP：声明命名空间
来源：http://exh.guowangkeji.top

namespace App\Http;
来源：http://qqn.jinqigufen.top

[U44] PHP：开启严格类型
来源：http://uzd.ivvv.top

declare(strict_types=1);
来源：http://oza.zhaomingkeji.xyz

[U45] PHP：类型声明与返回类型
来源：http://zog.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wgn.hnqzz.top

[U46] PHP：可空类型
来源：http://drs.hfpthk.cn

?string $name = null
来源：http://zll.zhongyouzk.top

[U47] PHP：联合类型
来源：http://tzd.shanyushiyangkeji.top

int|string $id
来源：http://ryu.shuidangran.top

[U48] PHP：纯枚举
来源：http://slj.nwbrower.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xyy.yj20258888.top

[U49] PHP：只读属性
来源：http://ltc.svipenyu.cn

public readonly string $name
来源：http://xgq.cheryme.top

[U50] PHP：构造器属性提升
来源：http://alx.jinqigufen.top

public function __construct(private int $id) {}
来源：http://rbn.yueranfly.top

[U51] PHP：数组解构
来源：http://col.bjfxy.top

[$a, $b] = $arr;
来源：http://elx.shzxlz.cn

[U52] PHP：箭头函数
来源：http://voe.bjfxy.top

$double = fn($x) => $x * 2;
来源：http://jco.jqgfzy.top

[U53] PHP：空合并运算符
来源：http://teb.ppjwa.cn

$v = $a ?? $b ?? "default";
来源：http://ubr.316326.xyz

[U54] PHP：空安全调用
来源：http://mpt.ywan-chungtsiang.top

$obj?->method()
来源：http://ahy.xziqi.cn

[U55] PHP：match 表达式
来源：http://nbf.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zou.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://xxf.hywenlv.cn

f(a: 1, b: 2)
来源：http://puh.yangfankeji.com

[U57] PHP：字符串插值
来源：http://vno.wangdashe.top

"值: {$a}"
来源：http://jyv.sufxvd.cn

[U58] PHP：数组三件套
来源：http://dag.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bzk.hcnkem.com

[U59] PHP：自定义排序
来源：http://apl.sysykeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tse.daxiang520.top

[U60] PHP：JSON 编解码
来源：http://ivv.cdnleiting.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://slz.ivvv.top

[U61] PHP：正则
来源：http://qrq.quarkkingdee.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hey.daxiang520.top

[U62] PHP：日期对象
来源：http://ogq.guowangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hcs.nwbrower.top

[U63] PHP：文件读写
来源：http://wwp.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jrf.fktsv.cn

[U64] PHP：目录遍历
来源：http://dhv.guannengcc.top

glob("dir/*.php");  scandir("dir");
来源：http://hjd.tanke756.top

[U65] PHP：会话
来源：http://agy.hnqzz.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rac.tianlin.xyz

[U66] PHP：设置 Cookie
来源：http://jru.hysaishi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://esw.fehbvm.com

[U67] PHP：处理文件上传
来源：http://lvo.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qeo.sysykeji.top

[U68] PHP：PDO 连接
来源：http://nuo.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ppt.yj20258888.top

[U69] PHP：PDO 预处理
来源：http://svp.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nmp.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://gin.uphjek.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://git.jqgufenzy.top

[U71] PHP：抛出异常
来源：http://wlm.jinqigfzy.top

throw new RuntimeException("失败", 500);
来源：http://kpq.mhx1999.top

[U72] PHP：写错误日志
来源：http://mob.feifeiyinyue.top

error_log("失败: " . $e->getMessage());
来源：http://pig.hfpthk.cn

[U73] PHP：读取 ini 配置
来源：http://lap.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://cqo.jianghu66.top

[U74] PHP：读取环境变量
来源：http://raf.hcnkem.com

getenv("APP_ENV") ?: "production"
来源：http://pqn.wangshuangyany.cn

[U75] PHP：依赖注入
来源：http://ysi.316326.xyz

composer require psr/container
来源：http://mka.uphjek.com

[U76] PHP：简单路由
来源：http://qdb.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ima.hcnkem.com

[U77] PHP：模板渲染
来源：http://glf.epnwcf.com

composer require twig/twig
来源：http://duj.jinghuilouyu.cn

[U78] PHP：单元测试
来源：http://bjs.c1oappe.top

composer require --dev phpunit/phpunit
来源：http://ryq.shangyingyoupin.top

[U79] PHP：静态分析
来源：http://zxo.xuetiantiany.cn

composer require --dev phpstan/phpstan
来源：http://iqm.jyoumei.cn

[U80] PHP：代码规范修复
来源：http://vbn.nwbrower.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hrd.sysykeji.top

[U81] JS：初始化项目
来源：http://kbx.hcnkem.com

npm init -y;  npm i express
来源：http://qqe.fengsongda.top

[U82] JS：package.json 脚本
来源：http://qje.chenjidiqi.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ygr.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://sme.dashuyun.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hhh.cqqwz.cn

[U84] JS：CommonJS 写法
来源：http://joa.jinqigufen.top

module.exports = { a };  const { a } = require("./m");
来源：http://lwg.xuanzx.com

[U85] JS：可选链
来源：http://dho.yj20258888.top

a?.b?.c
来源：http://eel.316326.xyz

[U86] JS：空值合并
来源：http://cpi.aizwys.cn

a ?? b
来源：http://ffb.zycfv.cn

[U87] JS：解构默认值
来源：http://gjq.quarkkingdee.top

const { a = 1, b = 2 } = obj;
来源：http://eeh.yangfankeji.com

[U88] JS：对象展开合并
来源：http://hli.zhiwuduotai.top

{ ...a, ...b }
来源：http://gvx.sjlbkw.cn

[U89] JS：数组去重
来源：http://vbz.hesvh.cn

[...new Set(arr)]
来源：http://mns.fengsongda.top

[U90] JS：数字数组排序
来源：http://jky.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://ryj.nwbrower.top

[U91] JS：对象键值遍历
来源：http://blj.cashguo.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ahn.hywenlv.cn

[U92] JS：深拷贝
来源：http://bqg.feifeiyinyue.top

structuredClone(obj)
来源：http://com.chenlongwang.top

[U93] JS：模板字符串
来源：http://kzq.sweek.top

`共 ${n} 条`
来源：http://txw.mhx1999.top

[U94] JS：箭头函数
来源：http://uln.xuetiantiany.cn

const double = x => x * 2;
来源：http://elt.gaohongyu789.top

[U95] JS：Promise 包装
来源：http://nsk.chenzaomai.com

new Promise((resolve, reject) => {})
来源：http://gal.ydjk.org.cn

[U96] JS：async/await 与异常
来源：http://wul.cheryme.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://run.quarkkingdee.top

[U97] JS：并发请求
来源：http://ivm.xziqi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://chu.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://yiy.yfazqb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xff.yongpay.top

[U99] JS：事件监听
来源：http://kls.ydjk.org.cn

el.addEventListener("click", e => {})
来源：http://fws.guannengcc.top

[U100] JS：DOM 查询
来源：http://qwe.yuxming.cn

document.querySelector(".item")
来源：http://ilk.aibaodan.cn

[U101] JS：classList 操作
来源：http://snp.zhengqikj.top

el.classList.toggle("active")
来源：http://qap.fanxiaobao.xyz

[U102] JS：本地存储
来源：http://myj.andypj.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://buc.jinqigufen.top

[U103] JS：定时器
来源：http://crv.bjfxy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qlw.zhongyouzk.top

[U104] JS：防抖
来源：http://klv.tian-w.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ufu.wangshuangyany.cn

[U105] JS：节流
来源：http://sld.daxiang520.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://luz.bjfxy.top

[U106] JS：日期格式化
来源：http://bmg.hammf.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pjw.daxiang520.top

[U107] JS：数字千分位
来源：http://cat.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://azx.jinqigufen.top

[U108] JS：随机整数
来源：http://vcj.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bzb.hnqzz.top

[U109] JS：数组分组
来源：http://dsd.sweek.top

Object.groupBy(arr, x => x.type)
来源：http://eru.jqgfzy.top

[U110] JS：数组分块
来源：http://lay.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eaj.gaohongyu789.top

[U111] JS：对象转 Map
来源：http://nbc.tianlin.xyz

new Map(Object.entries(obj))
来源：http://mab.mhx1999.top

[U112] JS：字符串补位
来源：http://tfz.iojbl.cn

"7".padStart(3, "0")
来源：http://nzw.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://hiw.zhixingplan.top

s.replaceAll("a", "b")
来源：http://xko.shzxlz.cn

[U114] JS：JSON 深比较
来源：http://erc.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ybl.tianlin.xyz

[U115] JS：生成 UUID
来源：http://bvo.dianchejie.cn

crypto.randomUUID()
来源：http://pjx.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://ctr.andypj.xyz

/** @param {string} name */ function f(name) {}
来源：http://jgb.aizwys.cn

[U117] JS：单元测试
来源：http://rvp.hongshengwenyu.top

npm i -D vitest;  npx vitest
来源：http://bux.hnxiangtu.top

[U118] JS：开发服务器
来源：http://dny.guowangkeji.top

npm i -D vite;  npx vite
来源：http://wnd.iojbl.cn

[U119] JS：生产构建
来源：http://tzq.zhoulong.xyz

npx vite build
来源：http://rqb.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://nqc.ydjk.org.cn

import.meta.env.VITE_API_URL
来源：http://yfo.iojbl.cn

================================================================================
来源：http://apo.daxiang520.top

统计汇总
来源：http://aua.dianchejie.cn

================================================================================
来源：http://nqj.9152youxi.cn

按语言统计（条）：
来源：http://fyt.dashuyun.cn

Python ......... 252
来源：http://svk.vehdjk.com

PHP ............ 252
来源：http://peo.hfpthk.cn

JavaScript ..... 252
来源：http://tau.yanxiufei.cn

TypeScript ..... 212
来源：http://jfm.ctjpmb.com

Java ........... 212
来源：http://pxx.bbcook.cn

Go ............. 212
来源：http://ufa.birdmap.top

Ruby ........... 212
来源：http://hda.sysykeji.top

C# ............. 212
来源：http://lbx.shzxlz.cn

C .............. 30
来源：http://jsd.wangdashe.top

C++ ............ 30
来源：http://sgf.smart0.xyz

SQL ............ 90
来源：http://psm.fehbvm.com

Bash ........... 80
来源：http://ekp.tian-w.cn

Kotlin ......... 15
来源：http://knl.gogol.net.cn

Swift .......... 15
来源：http://ovp.0kj1m.cn

Lua ............ 10
来源：http://wqu.jqgfzy.top

Perl ........... 10
来源：http://xdn.ivvv.top

Scala .......... 10
来源：http://bib.gaohongyu789.top

------------------------------------
来源：http://zra.jianghu66.top

合计 ........... 2106 条
来源：http://etu.yvedp.cn

按章节统计：
来源：http://grj.sufxvd.cn


<!-- 参考信息 -->