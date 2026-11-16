代发 wailian999

[T47] Perl：正则捕获
来源：http://fct.tian-w.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yli.zhaomingkeji.xyz

[T48] Perl：正则替换
来源：http://shj.zycfv.cn

$s =~ s/old/new/g;
来源：http://zof.fehbvm.com

[T49] Perl：函数
来源：http://qpt.pycfn.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qiy.316326.xyz

[T50] Perl：逐行读文件
来源：http://hnc.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vyg.nanxuanxn.top

while (my $line = <$fh>) { print $line; }
来源：http://iqu.gzhubu.top

[T51] Scala：Hello World
来源：http://wed.guowangkeji.top

println("Hello")
来源：http://sdp.gotoacloud.top

[T52] Scala：变量
来源：http://zgc.bbcook.cn

val a = 1;  var b = 2
来源：http://ycz.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://vxo.quarkkingdee.top

s"值: $b"
来源：http://rdw.316326.xyz

[T54] Scala：集合映射
来源：http://jal.jqgufenzy.top

List(1, 2, 3).map(_ * 2)
来源：http://dha.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://cgh.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pci.zhiwuduotai.top

[T56] Scala：样例类
来源：http://uoy.nwbrower.top

case class User(name: String, age: Int)
来源：http://zsw.hnqzz.top

[T57] Scala：模式匹配
来源：http://sgv.cdnleiting.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ntl.0kj1m.cn

[T58] Scala：函数定义
来源：http://kil.yj20258.top

def add(a: Int, b: Int): Int = a + b
来源：http://emn.fengsongda.top

[T59] Scala：循环
来源：http://qcn.ehwqpu.com

for (i <- 1 to 10) println(i)
来源：http://hrk.smart0.xyz

[T60] Scala：折叠
来源：http://eok.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bvi.jianghu66.top

================================================================================
来源：http://gpa.jinghuilouyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://syw.zhengqikj.top

================================================================================
来源：http://vwm.wangshuangyany.cn

[U01] Py：创建虚拟环境
来源：http://ixv.yongpay.top

python -m venv .venv && source .venv/bin/activate
来源：http://xxd.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://rha.jqgfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qfi.hysaishi.cn

[U03] Py：加载 .env 配置
来源：http://szw.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://dea.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://ijt.zycfv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://diz.shangyingyoupin.top

[U05] Py：列表去重且保序
来源：http://flw.birdmap.top

list(dict.fromkeys(arr))
来源：http://jcp.gzhubu.top

[U06] Py：合并两个字典
来源：http://afb.yangfankeji.com

{**a, **b}
来源：http://xjb.yj202588.top

[U07] Py：反转字典键值
来源：http://upc.ivvv.top

{v: k for k, v in d.items()}
来源：http://dfc.hongshengwenyu.top

[U08] Py：展平二维列表
来源：http://ajo.guannengcc.top

[y for x in nested for y in x]
来源：http://jpb.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://mbp.kuanghao11.cn

max(d, key=d.get)
来源：http://msm.zhengqikj.top

[U10] Py：按值排序字典
来源：http://szs.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ilc.cqqwz.cn

[U11] Py：生成器表达式
来源：http://nfj.mhx1999.top

(x * 2 for x in arr)
来源：http://mdu.aibaodan.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eki.nwbrower.top

Counter(arr).most_common(3)
来源：http://dnn.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://vbw.redwolf501.top

deque(maxlen=10)
来源：http://ikb.tanke756.top

[U14] Py：分组收集到列表
来源：http://wxq.zdqjudy.top

defaultdict(list)
来源：http://onm.cucudq.cn

[U15] Py：高精度计时
来源：http://qhh.xylfe.cn

t = time.perf_counter()
来源：http://ewi.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://avo.cashguo.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pxq.chenlongwang.top

[U17] Py：初始化日志
来源：http://emn.tian-w.cn

logging.basicConfig(level=logging.INFO)
来源：http://mpy.xingfuxueyuan.xyz

[U18] Py：预编译正则
来源：http://hva.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://ygt.tanke756.top

[U19] Py：正则替换带回调
来源：http://pbe.pycfn.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rfo.pycfn.com

[U20] Py：缓存函数结果
来源：http://svp.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://dca.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://dib.zhengqikj.top

@contextlib.contextmanager
来源：http://inh.52xcode.cn

[U22] Py：矩阵转置
来源：http://xus.haohaochexian.top

list(zip(*m))
来源：http://txu.guannengcc.top

[U23] Py：分块读取大文件
来源：http://jzd.feifeiyinyue.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zsy.shzxlz.cn

[U24] Py：路径操作
来源：http://xpm.redwolf501.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xpq.nwbrower.top

[U25] Py：CSV 按字典读
来源：http://hmr.kuanghao11.cn

csv.DictReader(f)
来源：http://vww.yongpay.top

[U26] Py：并发下载
来源：http://ktq.zhengqikj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vvu.bjfxy.top

[U27] Py：异步 HTTP
来源：http://auo.shanyushiyangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://zvd.xuetiantiany.cn

[U28] Py：类型别名
来源：http://ubd.andypj.xyz

UserId = int
来源：http://uug.tarul.cn

[U29] Py：属性校验
来源：http://ybz.birdmap.top

@property 与 @x.setter 配合
来源：http://yln.ydjk.org.cn

[U30] Py：数据类
来源：http://jse.sxryk.cn

@dataclass(slots=True)
来源：http://eqy.52xcode.cn

[U31] Py：单测
来源：http://jtz.xingfuxueyuan.xyz

python -m pytest -q
来源：http://jgd.yuxming.cn

[U32] Py：代码格式化
来源：http://awf.zhixingplan.top

ruff format . && ruff check --fix .
来源：http://ewu.shangyingyoupin.top

[U33] Py：打包发布
来源：http://ixv.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://gew.xingfuxueyuan.xyz

[U34] Py：判断编码
来源：http://gbz.wangshuangyany.cn

chardet.detect(raw)
来源：http://qnz.birdmap.top

[U35] Py：发送邮件
来源：http://hez.bjfxy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://apw.cqqwz.cn

[U36] Py：定时任务
来源：http://yqa.smart0.xyz

schedule.every(10).minutes.do(job)
来源：http://pju.cheryme.top

[U37] Py：读写 Excel
来源：http://tax.hnqzz.top

pandas.read_excel / DataFrame.to_excel
来源：http://mqq.chenzaomai.com

[U38] Py：获取脚本所在目录
来源：http://mng.bjfxy.top

Path(__file__).resolve().parent
来源：http://uvl.tian-w.cn

[U39] Py：判断是否在交互环境
来源：http://hsh.meibo888.top

sys.stdout.isatty()
来源：http://wrq.guowangkeji.top

[U40] Py：打印到标准错误
来源：http://muo.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://bia.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://aiq.0kj1m.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qig.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://vik.sufxvd.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vka.zycfv.cn

[U43] PHP：声明命名空间
来源：http://kun.feifeiyinyue.top

namespace App\Http;
来源：http://oze.hammf.cn

[U44] PHP：开启严格类型
来源：http://xku.tanke756.top

declare(strict_types=1);
来源：http://qai.snrcjt.cn

[U45] PHP：类型声明与返回类型
来源：http://lks.sjlbkw.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fmx.mhx1999.top

[U46] PHP：可空类型
来源：http://zjr.sufxvd.cn

?string $name = null
来源：http://kbe.shuidangran.top

[U47] PHP：联合类型
来源：http://hsc.yueranfly.top

int|string $id
来源：http://dvs.aibaodan.cn

[U48] PHP：纯枚举
来源：http://ely.chenjidiqi.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wzz.nwbrower.top

[U49] PHP：只读属性
来源：http://doi.cucudq.cn

public readonly string $name
来源：http://ftz.zdbjq.cn

[U50] PHP：构造器属性提升
来源：http://fny.chenlongwang.top

public function __construct(private int $id) {}
来源：http://rrp.nanxinkj.top

[U51] PHP：数组解构
来源：http://cwq.hnqzz.top

[$a, $b] = $arr;
来源：http://grd.ydzc1.top

[U52] PHP：箭头函数
来源：http://bhr.jlsjyb.cn

$double = fn($x) => $x * 2;
来源：http://mrr.epnwcf.com

[U53] PHP：空合并运算符
来源：http://jin.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://ttw.sysykeji.top

[U54] PHP：空安全调用
来源：http://dqi.hnxiangtu.top

$obj?->method()
来源：http://dlr.smart0.xyz

[U55] PHP：match 表达式
来源：http://wjd.tianlin.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://obb.guowangkeji.top

[U56] PHP：命名参数
来源：http://pww.hysaishi.cn

f(a: 1, b: 2)
来源：http://ecy.redwolf501.top

[U57] PHP：字符串插值
来源：http://dxa.guowangkeji.top

"值: {$a}"
来源：http://gyi.hfpthk.cn

[U58] PHP：数组三件套
来源：http://oxf.ctjpmb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mwr.andypj.xyz

[U59] PHP：自定义排序
来源：http://dpt.xylfe.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ddx.zycfv.cn

[U60] PHP：JSON 编解码
来源：http://mzh.snrcjt.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://txy.zhoulong.xyz

[U61] PHP：正则
来源：http://eml.hammf.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://saz.nwbrower.top

[U62] PHP：日期对象
来源：http://bcn.ybcxt.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ual.ehwqpu.com

[U63] PHP：文件读写
来源：http://wdu.yuxming.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xao.shangyingyoupin.top

[U64] PHP：目录遍历
来源：http://ufi.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://bck.yfazqb.com

[U65] PHP：会话
来源：http://nwy.nwbrower.top

session_start();  $_SESSION["uid"] = 1;
来源：http://taq.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://mby.9152youxi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cee.ydzc1.top

[U67] PHP：处理文件上传
来源：http://aqm.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vih.guowangkeji.top

[U68] PHP：PDO 连接
来源：http://ooy.shzxlz.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gbw.gzhubu.top

[U69] PHP：PDO 预处理
来源：http://qua.yj20258888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sbe.zhengqikj.top

[U70] PHP：PDO 事务
来源：http://ioz.bbcook.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://syp.yanxiufei.cn

[U71] PHP：抛出异常
来源：http://bww.zdbjq.cn

throw new RuntimeException("失败", 500);
来源：http://vri.jinghuilouyu.cn

[U72] PHP：写错误日志
来源：http://iea.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://pua.iojbl.cn

[U73] PHP：读取 ini 配置
来源：http://nuy.hammf.cn

parse_ini_file("config.ini", true)
来源：http://pva.zdbjq.cn

[U74] PHP：读取环境变量
来源：http://ctr.chenlongwang.top

getenv("APP_ENV") ?: "production"
来源：http://dgy.c1oappe.top

[U75] PHP：依赖注入
来源：http://vfm.daria6918.cn

composer require psr/container
来源：http://uhq.zhoulong.xyz

[U76] PHP：简单路由
来源：http://nyx.tarul.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jbm.fanxiaobao.xyz

[U77] PHP：模板渲染
来源：http://usw.nanxuanxn.top

composer require twig/twig
来源：http://hgd.sysykeji.top

[U78] PHP：单元测试
来源：http://hsv.jyoumei.cn

composer require --dev phpunit/phpunit
来源：http://psw.yueranfly.top

[U79] PHP：静态分析
来源：http://cdb.yuxming.cn

composer require --dev phpstan/phpstan
来源：http://sop.fehbvm.com

[U80] PHP：代码规范修复
来源：http://suw.ehwqpu.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://pkz.zdqjudy.top

[U81] JS：初始化项目
来源：http://ift.sweek.top

npm init -y;  npm i express
来源：http://egx.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://ykw.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iur.feifeiyinyue.top

[U83] JS：ES Module 导入导出
来源：http://eph.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://aol.c1oappe.top

[U84] JS：CommonJS 写法
来源：http://cux.smart0.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://efz.zdqjudy.top

[U85] JS：可选链
来源：http://dla.wangshuangyany.cn

a?.b?.c
来源：http://psi.jiagoushi.top

[U86] JS：空值合并
来源：http://qcq.tanke756.top

a ?? b
来源：http://yrd.hysaishi.cn

[U87] JS：解构默认值
来源：http://nmc.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://jxf.hesvh.cn

[U88] JS：对象展开合并
来源：http://hqf.jinyuanbaomall.cn

{ ...a, ...b }
来源：http://jre.aizwys.cn

[U89] JS：数组去重
来源：http://uit.0kj1m.cn

[...new Set(arr)]
来源：http://zar.0kj1m.cn

[U90] JS：数字数组排序
来源：http://vfw.zycfv.cn

[...arr].sort((a, b) => a - b)
来源：http://qrd.zhijiandao.cn

[U91] JS：对象键值遍历
来源：http://sfj.cqqwz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ejt.yj20258.top

[U92] JS：深拷贝
来源：http://nde.yvedp.cn

structuredClone(obj)
来源：http://kvl.chenlongwang.top

[U93] JS：模板字符串
来源：http://zox.fengsongda.top

`共 ${n} 条`
来源：http://gpe.jinqigufen.top

[U94] JS：箭头函数
来源：http://jve.gotoacloud.top

const double = x => x * 2;
来源：http://etf.jqgufenzy.top

[U95] JS：Promise 包装
来源：http://aed.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://unz.jinqigfzy.top

[U96] JS：async/await 与异常
来源：http://jii.hnxiangtu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rno.sxryk.cn

[U97] JS：并发请求
来源：http://jfq.havefunace.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gte.aibaodan.cn

[U98] JS：fetch 带 JSON
来源：http://jyy.fengsongda.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uht.aizwys.cn

[U99] JS：事件监听
来源：http://twa.pengpengdd.cyou

el.addEventListener("click", e => {})
来源：http://ute.redwolf501.top

[U100] JS：DOM 查询
来源：http://krz.epnwcf.com

document.querySelector(".item")
来源：http://dnx.daria6918.cn

[U101] JS：classList 操作
来源：http://kyk.zhongyouzk.top

el.classList.toggle("active")
来源：http://kuc.xingfuxueyuan.xyz

[U102] JS：本地存储
来源：http://lpe.redwolf501.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wml.jlsjyb.cn

[U103] JS：定时器
来源：http://spb.yongpay.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tyo.shangyingyoupin.top

[U104] JS：防抖
来源：http://khq.zhengqikj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vfq.birdmap.top

[U105] JS：节流
来源：http://cwz.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dfh.zhoulong.xyz

[U106] JS：日期格式化
来源：http://ljx.zhaomingkeji.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wmn.bbcook.cn

[U107] JS：数字千分位
来源：http://lyj.shanyushiyangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xji.zhijiandao.cn

[U108] JS：随机整数
来源：http://cqd.zhixingplan.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hfs.epnwcf.com

[U109] JS：数组分组
来源：http://aad.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://ije.guannengcc.top

[U110] JS：数组分块
来源：http://gwp.jianghu66.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hpy.birdmap.top

[U111] JS：对象转 Map
来源：http://jbd.hnqzz.top

new Map(Object.entries(obj))
来源：http://fsk.chenzaomai.com

[U112] JS：字符串补位
来源：http://mei.dashuyun.cn

"7".padStart(3, "0")
来源：http://xvg.meibo888.top

[U113] JS：正则替换全部
来源：http://rtz.9152youxi.cn

s.replaceAll("a", "b")
来源：http://evt.hcnkem.com

[U114] JS：JSON 深比较
来源：http://lnx.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://usy.yongpay.top

[U115] JS：生成 UUID
来源：http://syy.shangyingyoupin.top

crypto.randomUUID()
来源：http://vna.gaohongyu789.top

[U116] JS：类型检查（JSDoc）
来源：http://pla.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://jpd.52xcode.cn

[U117] JS：单元测试
来源：http://mrn.316326.xyz

npm i -D vitest;  npx vitest
来源：http://qpf.fehbvm.com

[U118] JS：开发服务器
来源：http://hru.pycfn.com

npm i -D vite;  npx vite
来源：http://klv.0kj1m.cn

[U119] JS：生产构建
来源：http://yzu.sufxvd.cn

npx vite build
来源：http://bes.xinyue.icu

[U120] JS：读取环境变量（Vite）
来源：http://ota.yanxiufei.cn

import.meta.env.VITE_API_URL
来源：http://tfl.daxiang520.top

================================================================================
来源：http://pjz.nanxinkj.top

统计汇总
来源：http://ffh.316326.xyz

================================================================================
来源：http://jyj.yueranfly.top

按语言统计（条）：
来源：http://qvn.cdnleiting.top

Python ......... 252
来源：http://ygd.haohaochexian.top

PHP ............ 252
来源：http://fvq.quarkkingdee.top

JavaScript ..... 252
来源：http://sqe.sweek.top

TypeScript ..... 212
来源：http://fze.yuanzhike.top

Java ........... 212
来源：http://grp.ybcxt.top

Go ............. 212
来源：http://tka.mhx1999.top

Ruby ........... 212
来源：http://ngx.meibo888.top

C# ............. 212
来源：http://sfd.tian-w.cn

C .............. 30
来源：http://zqf.c1oappe.top

C++ ............ 30
来源：http://xrf.hnxiangtu.top

SQL ............ 90
来源：http://mva.gotoacloud.top

Bash ........... 80
来源：http://vce.fengsongda.top

Kotlin ......... 15
来源：http://dqb.hnqzz.top

Swift .......... 15
来源：http://gbe.yueranfly.top

Lua ............ 10
来源：http://hxb.yfazqb.com

Perl ........... 10
来源：http://kab.zdqjudy.top

Scala .......... 10
来源：http://duw.cdnleiting.top

------------------------------------
来源：http://yqa.cheryme.top

合计 ........... 2106 条
来源：http://adq.pengpengdd.cyou

按章节统计：
来源：http://jwg.yanxiufei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://plo.gotoacloud.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://orb.gzhubu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xgu.jiagoushi.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://inr.tarul.cn


<!-- 参考信息 -->