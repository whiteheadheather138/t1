代发 wailian999

[T43] Perl：字符串插值
来源：http://uxc.sysykeji.top

"值: $a"
来源：http://sim.shanyushiyangkeji.top

[T44] Perl：条件
来源：http://rtu.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://amn.aizwys.cn

[T45] Perl：数组遍历
来源：http://xsr.daxiang520.top

for my $x (@arr) { print $x; }
来源：http://dhv.uphjek.com

[T46] Perl：哈希操作
来源：http://irn.52xcode.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ksw.yvedp.cn

[T47] Perl：正则捕获
来源：http://ytg.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uth.xylfe.cn

[T48] Perl：正则替换
来源：http://iwe.hongshengwenyu.top

$s =~ s/old/new/g;
来源：http://ovt.gogol.net.cn

[T49] Perl：函数
来源：http://nwt.xinyue.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lsc.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://jyh.yj20258.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hcm.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://bno.zhiwuduotai.top

[T51] Scala：Hello World
来源：http://xoy.feifeiyinyue.top

println("Hello")
来源：http://oyh.ppjwa.cn

[T52] Scala：变量
来源：http://cfs.zhixingplan.top

val a = 1;  var b = 2
来源：http://hrm.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://pms.gotoacloud.top

s"值: $b"
来源：http://jjv.aibaodan.cn

[T54] Scala：集合映射
来源：http://oiu.jinqigfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://ogy.zhengqikj.top

[T55] Scala：集合过滤
来源：http://soq.daxiang520.top

List(1, 2, 3).filter(_ > 1)
来源：http://nzd.hnqzz.top

[T56] Scala：样例类
来源：http://vnm.havefunace.top

case class User(name: String, age: Int)
来源：http://dwo.ywan-chungtsiang.top

[T57] Scala：模式匹配
来源：http://lpg.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gnh.zdqjudy.top

[T58] Scala：函数定义
来源：http://fak.shanyushiyangtech.top

def add(a: Int, b: Int): Int = a + b
来源：http://lsa.ehwqpu.com

[T59] Scala：循环
来源：http://dkk.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://xxr.shzxlz.cn

[T60] Scala：折叠
来源：http://aiu.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bml.tanke756.top

================================================================================
来源：http://dru.hammf.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://foi.sweek.top

================================================================================
来源：http://lxh.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://nhx.cqqwz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vsh.fanxiaobao.xyz

[U02] Py：导出 / 安装依赖
来源：http://ocs.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aug.ivvv.top

[U03] Py：加载 .env 配置
来源：http://rkz.pycfn.com

from dotenv import load_dotenv; load_dotenv()
来源：http://jwg.yuanzhike.top

[U04] Py：变量调试打印
来源：http://gyg.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ten.ppjwa.cn

[U05] Py：列表去重且保序
来源：http://iiu.sjlbkw.cn

list(dict.fromkeys(arr))
来源：http://nlj.vehdjk.com

[U06] Py：合并两个字典
来源：http://ctn.fktsv.cn

{**a, **b}
来源：http://wkl.xylfe.cn

[U07] Py：反转字典键值
来源：http://ydt.ctjpmb.com

{v: k for k, v in d.items()}
来源：http://cwd.smart0.xyz

[U08] Py：展平二维列表
来源：http://ojv.uphjek.com

[y for x in nested for y in x]
来源：http://tbj.uphjek.com

[U09] Py：字典取最大值的键
来源：http://nec.ydjk.org.cn

max(d, key=d.get)
来源：http://xpe.jinyuanbaomall.cn

[U10] Py：按值排序字典
来源：http://lzw.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tqo.sweek.top

[U11] Py：生成器表达式
来源：http://wij.andypj.xyz

(x * 2 for x in arr)
来源：http://rrc.xingfuxueyuan.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://pvy.zdbjq.cn

Counter(arr).most_common(3)
来源：http://lqk.zhoulong.xyz

[U13] Py：固定长度队列
来源：http://kqu.cheryme.top

deque(maxlen=10)
来源：http://fmi.xuanzx.com

[U14] Py：分组收集到列表
来源：http://ajb.zdqjudy.top

defaultdict(list)
来源：http://trl.feifeiyinyue.top

[U15] Py：高精度计时
来源：http://tyq.aibaodan.cn

t = time.perf_counter()
来源：http://sfk.epnwcf.com

[U16] Py：命令行参数解析
来源：http://ozt.gzhubu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qqu.cucudq.cn

[U17] Py：初始化日志
来源：http://ici.shzxlz.cn

logging.basicConfig(level=logging.INFO)
来源：http://ifi.vehdjk.com

[U18] Py：预编译正则
来源：http://mrt.fktsv.cn

pat = re.compile(r"\d+")
来源：http://xzc.nanxinkj.top

[U19] Py：正则替换带回调
来源：http://bxc.xingfuxueyuan.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rbx.jyoumei.cn

[U20] Py：缓存函数结果
来源：http://jkg.nanxinkj.top

@functools.lru_cache(maxsize=None)
来源：http://vfw.jyoumei.cn

[U21] Py：自定义上下文管理器
来源：http://jan.hywenlv.cn

@contextlib.contextmanager
来源：http://lsm.nwbrower.top

[U22] Py：矩阵转置
来源：http://lvl.svipenyu.cn

list(zip(*m))
来源：http://nce.bjfxy.top

[U23] Py：分块读取大文件
来源：http://pul.shangyingyoupin.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wbr.hnqzz.top

[U24] Py：路径操作
来源：http://sql.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://apa.gaohongyu789.top

[U25] Py：CSV 按字典读
来源：http://gnf.wangdashe.top

csv.DictReader(f)
来源：http://ciu.yfazqb.com

[U26] Py：并发下载
来源：http://vwm.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hte.dianchejie.cn

[U27] Py：异步 HTTP
来源：http://xnv.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://rga.shzxlz.cn

[U28] Py：类型别名
来源：http://wuu.jqgfzy.top

UserId = int
来源：http://xkg.ivvv.top

[U29] Py：属性校验
来源：http://rbs.ehwqpu.com

@property 与 @x.setter 配合
来源：http://cdc.tanke756.top

[U30] Py：数据类
来源：http://olz.jianghu66.top

@dataclass(slots=True)
来源：http://wcx.nwbrower.top

[U31] Py：单测
来源：http://ass.316326.xyz

python -m pytest -q
来源：http://xlk.tianlin.xyz

[U32] Py：代码格式化
来源：http://lvf.nwbrower.top

ruff format . && ruff check --fix .
来源：http://jlb.vehdjk.com

[U33] Py：打包发布
来源：http://anb.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://kyw.nwbrower.top

[U34] Py：判断编码
来源：http://miy.xinyue.icu

chardet.detect(raw)
来源：http://voi.zhengqikj.top

[U35] Py：发送邮件
来源：http://hby.yangfankeji.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pvy.hesvh.cn

[U36] Py：定时任务
来源：http://vwe.sweek.top

schedule.every(10).minutes.do(job)
来源：http://idr.iojbl.cn

[U37] Py：读写 Excel
来源：http://tvs.cheryme.top

pandas.read_excel / DataFrame.to_excel
来源：http://adc.c1oappe.top

[U38] Py：获取脚本所在目录
来源：http://yip.mhx1999.top

Path(__file__).resolve().parent
来源：http://uto.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://sna.52xcode.cn

sys.stdout.isatty()
来源：http://zex.aizwys.cn

[U40] Py：打印到标准错误
来源：http://xzr.xziqi.cn

print("err", file=sys.stderr)
来源：http://glg.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://cth.aizwys.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vpr.wangshuangyany.cn

[U42] PHP：PSR-4 自动加载
来源：http://ugp.shanyushiyangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xxm.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://xhs.jianghu66.top

namespace App\Http;
来源：http://bzh.gogol.net.cn

[U44] PHP：开启严格类型
来源：http://cyx.snrcjt.cn

declare(strict_types=1);
来源：http://gkx.chenjidiqi.icu

[U45] PHP：类型声明与返回类型
来源：http://eiw.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uxy.xinyue.icu

[U46] PHP：可空类型
来源：http://zay.hysaishi.cn

?string $name = null
来源：http://woj.yfazqb.com

[U47] PHP：联合类型
来源：http://nzs.sjlbkw.cn

int|string $id
来源：http://vwy.aizwys.cn

[U48] PHP：纯枚举
来源：http://plv.birdmap.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ivb.xziqi.cn

[U49] PHP：只读属性
来源：http://poi.fengsongda.top

public readonly string $name
来源：http://pao.yj20258.top

[U50] PHP：构造器属性提升
来源：http://atp.nanxuanxn.top

public function __construct(private int $id) {}
来源：http://pyg.chenzaomai.com

[U51] PHP：数组解构
来源：http://mmu.hammf.cn

[$a, $b] = $arr;
来源：http://vic.ydzc1.top

[U52] PHP：箭头函数
来源：http://bxr.cucudq.cn

$double = fn($x) => $x * 2;
来源：http://zjq.yueranfly.top

[U53] PHP：空合并运算符
来源：http://kyu.nwbrower.top

$v = $a ?? $b ?? "default";
来源：http://wcn.52xcode.cn

[U54] PHP：空安全调用
来源：http://zsp.yuxming.cn

$obj?->method()
来源：http://zsv.hfpthk.cn

[U55] PHP：match 表达式
来源：http://eid.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ccb.jyoumei.cn

[U56] PHP：命名参数
来源：http://hal.hesvh.cn

f(a: 1, b: 2)
来源：http://kzo.quarkkingdee.top

[U57] PHP：字符串插值
来源：http://egx.cqqwz.cn

"值: {$a}"
来源：http://slm.zdbjq.cn

[U58] PHP：数组三件套
来源：http://oou.tian-w.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xom.nanxinkj.top

[U59] PHP：自定义排序
来源：http://yuo.xuanzx.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fkl.havefunace.top

[U60] PHP：JSON 编解码
来源：http://gne.yj20258888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pdm.wangshuangyany.cn

[U61] PHP：正则
来源：http://vsv.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wbo.yj20258888.top

[U62] PHP：日期对象
来源：http://dtg.gogol.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gvb.hnxiangtu.top

[U63] PHP：文件读写
来源：http://wtl.yj20258888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kop.gotoacloud.top

[U64] PHP：目录遍历
来源：http://ogg.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://uqd.dianchejie.cn

[U65] PHP：会话
来源：http://gik.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://blz.vehdjk.com

[U66] PHP：设置 Cookie
来源：http://twk.hongshengwenyu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zee.fengsongda.top

[U67] PHP：处理文件上传
来源：http://awn.vehdjk.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zlg.gaohongyu789.top

[U68] PHP：PDO 连接
来源：http://kgt.smart0.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ygn.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://qmj.hongshengwenyu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rpf.yj20258.top

[U70] PHP：PDO 事务
来源：http://oef.hnqzz.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ubw.cucudq.cn

[U71] PHP：抛出异常
来源：http://hjx.smart0.xyz

throw new RuntimeException("失败", 500);
来源：http://uun.andypj.xyz

[U72] PHP：写错误日志
来源：http://bny.shanyushiyangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://qbj.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://jae.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://jjv.uphjek.com

[U74] PHP：读取环境变量
来源：http://era.hongshengwenyu.top

getenv("APP_ENV") ?: "production"
来源：http://fyy.hywenlv.cn

[U75] PHP：依赖注入
来源：http://vfq.shanyushiyangtech.top

composer require psr/container
来源：http://rnt.wangshuangyany.cn

[U76] PHP：简单路由
来源：http://fzu.tanke756.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wqk.yangfankeji.com

[U77] PHP：模板渲染
来源：http://axu.hnqzz.top

composer require twig/twig
来源：http://hje.guannengcc.top

[U78] PHP：单元测试
来源：http://opy.316326.xyz

composer require --dev phpunit/phpunit
来源：http://psl.cashguo.top

[U79] PHP：静态分析
来源：http://zsx.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://wsp.jiagoushi.top

[U80] PHP：代码规范修复
来源：http://idv.jqgufenzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pzu.dianchejie.cn

[U81] JS：初始化项目
来源：http://evb.nanxinkj.top

npm init -y;  npm i express
来源：http://uus.jiagoushi.top

[U82] JS：package.json 脚本
来源：http://qni.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ssg.quarkkingdee.top

[U83] JS：ES Module 导入导出
来源：http://poj.gzhubu.top

export const a = 1;  import { a } from "./m.js";
来源：http://guw.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://qyh.shzxlz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tzg.guowangkeji.top

[U85] JS：可选链
来源：http://fsi.cashguo.top

a?.b?.c
来源：http://bun.tianlin.xyz

[U86] JS：空值合并
来源：http://jar.yfazqb.com

a ?? b
来源：http://ywx.cdnleiting.top

[U87] JS：解构默认值
来源：http://lza.yvedp.cn

const { a = 1, b = 2 } = obj;
来源：http://jie.yueranfly.top

[U88] JS：对象展开合并
来源：http://lyz.xylfe.cn

{ ...a, ...b }
来源：http://zzo.xylfe.cn

[U89] JS：数组去重
来源：http://wxl.xingfuxueyuan.xyz

[...new Set(arr)]
来源：http://gas.52xcode.cn

[U90] JS：数字数组排序
来源：http://reh.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://ozb.ybcxt.top

[U91] JS：对象键值遍历
来源：http://tnc.xuetiantiany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ffw.xziqi.cn

[U92] JS：深拷贝
来源：http://cvm.quarkkingdee.top

structuredClone(obj)
来源：http://wbc.ydjk.org.cn

[U93] JS：模板字符串
来源：http://kbv.nanxinkj.top

`共 ${n} 条`
来源：http://vtt.vqdsnc.cn

[U94] JS：箭头函数
来源：http://vzv.sufxvd.cn

const double = x => x * 2;
来源：http://roc.xziqi.cn

[U95] JS：Promise 包装
来源：http://wso.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://mja.nanxinkj.top

[U96] JS：async/await 与异常
来源：http://zje.fehbvm.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://arc.jlsjyb.cn

[U97] JS：并发请求
来源：http://alx.ydzc1.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lew.zhijiandao.cn

[U98] JS：fetch 带 JSON
来源：http://fgx.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fhq.meibo888.top

[U99] JS：事件监听
来源：http://wtm.chenlongwang.top

el.addEventListener("click", e => {})
来源：http://wmt.nanxinkj.top

[U100] JS：DOM 查询
来源：http://ipq.shanyushiyangtech.top

document.querySelector(".item")
来源：http://gqk.yanxiufei.cn

[U101] JS：classList 操作
来源：http://tyc.52xcode.cn

el.classList.toggle("active")
来源：http://tie.cashguo.top

[U102] JS：本地存储
来源：http://jrt.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nhg.hesvh.cn

[U103] JS：定时器
来源：http://gfr.yonumen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://unh.gaohongyu789.top

[U104] JS：防抖
来源：http://spz.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://okv.fzhhl.top

[U105] JS：节流
来源：http://hvw.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ptx.havefunace.top

[U106] JS：日期格式化
来源：http://xhu.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uhm.shzxlz.cn

[U107] JS：数字千分位
来源：http://oft.zhijiandao.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uyc.zdqjudy.top

[U108] JS：随机整数
来源：http://lto.ivvv.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mnl.tian-w.cn

[U109] JS：数组分组
来源：http://itu.chenzaomai.com

Object.groupBy(arr, x => x.type)
来源：http://rpw.yueranfly.top

[U110] JS：数组分块
来源：http://duq.svipenyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wat.bjfxy.top

[U111] JS：对象转 Map
来源：http://ajh.wangdashe.top

new Map(Object.entries(obj))
来源：http://bsi.daria6918.cn

[U112] JS：字符串补位
来源：http://vvu.pycfn.com

"7".padStart(3, "0")
来源：http://qox.chenlongwang.top

[U113] JS：正则替换全部
来源：http://awm.zhoulong.xyz

s.replaceAll("a", "b")
来源：http://pjn.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://xky.cheryme.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fmx.0kj1m.cn

[U115] JS：生成 UUID
来源：http://ctz.c1oappe.top

crypto.randomUUID()
来源：http://uot.cucudq.cn

[U116] JS：类型检查（JSDoc）
来源：http://pia.yfazqb.com

/** @param {string} name */ function f(name) {}
来源：http://juf.0kj1m.cn

[U117] JS：单元测试
来源：http://ylp.dashuyun.cn

npm i -D vitest;  npx vitest
来源：http://uot.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://skz.yj20258888.top

npm i -D vite;  npx vite
来源：http://ghq.epnwcf.com

[U119] JS：生产构建
来源：http://qlz.smart0.xyz

npx vite build
来源：http://sxp.zhijiandao.cn

[U120] JS：读取环境变量（Vite）
来源：http://hor.kuanghao11.cn

import.meta.env.VITE_API_URL
来源：http://tkd.vqdsnc.cn

================================================================================
来源：http://ble.gogol.net.cn

统计汇总
来源：http://uym.chenzaomai.com

================================================================================
来源：http://igv.jqgfzy.top

按语言统计（条）：
来源：http://apu.zhoulong.xyz

Python ......... 252
来源：http://cbf.shanyushiyangtech.top

PHP ............ 252
来源：http://bng.vehdjk.com

JavaScript ..... 252
来源：http://whd.0kj1m.cn

TypeScript ..... 212
来源：http://sck.chenjidiqi.icu

Java ........... 212
来源：http://icg.zhaomingkeji.xyz

Go ............. 212
来源：http://riq.zhengqikj.top

Ruby ........... 212
来源：http://giu.yuxming.cn

C# ............. 212
来源：http://jry.316326.xyz

C .............. 30
来源：http://fsk.fehbvm.com

C++ ............ 30
来源：http://csi.fzhhl.top

SQL ............ 90
来源：http://sos.hongshengwenyu.top

Bash ........... 80
来源：http://fcl.kuanghao11.cn

Kotlin ......... 15
来源：http://zle.cucudq.cn

Swift .......... 15
来源：http://yck.ivvv.top

Lua ............ 10
来源：http://xwg.xziqi.cn

Perl ........... 10
来源：http://ccc.epnwcf.com


<!-- 参考信息 -->