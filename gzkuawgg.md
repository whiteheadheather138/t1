代发 wailian999

[T43] Perl：字符串插值
来源：http://dmh.smart0.xyz

"值: $a"
来源：http://cxn.gotoacloud.top

[T44] Perl：条件
来源：http://ebr.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://qvj.xuanzx.com

[T45] Perl：数组遍历
来源：http://lwu.zhoulong.xyz

for my $x (@arr) { print $x; }
来源：http://vod.xylfe.cn

[T46] Perl：哈希操作
来源：http://gwz.wangdashe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xxq.cdnleiting.top

[T47] Perl：正则捕获
来源：http://eri.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://pvl.0kj1m.cn

[T48] Perl：正则替换
来源：http://fvy.ydjk.org.cn

$s =~ s/old/new/g;
来源：http://kni.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://tmc.cucudq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gua.cqqwz.cn

[T50] Perl：逐行读文件
来源：http://ggn.zhijiandao.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ktf.jianghu66.top

while (my $line = <$fh>) { print $line; }
来源：http://whu.hcnkem.com

[T51] Scala：Hello World
来源：http://wej.sjlbkw.cn

println("Hello")
来源：http://xfd.jiagoushi.top

[T52] Scala：变量
来源：http://kxt.jiagoushi.top

val a = 1;  var b = 2
来源：http://kec.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://kpi.yvedp.cn

s"值: $b"
来源：http://geg.sysykeji.top

[T54] Scala：集合映射
来源：http://cyd.andypj.xyz

List(1, 2, 3).map(_ * 2)
来源：http://oax.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://eva.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://rem.bjfxy.top

[T56] Scala：样例类
来源：http://ppc.yuxming.cn

case class User(name: String, age: Int)
来源：http://vox.fengsongda.top

[T57] Scala：模式匹配
来源：http://wrn.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qii.52xcode.cn

[T58] Scala：函数定义
来源：http://bvg.tarul.cn

def add(a: Int, b: Int): Int = a + b
来源：http://eax.shzxlz.cn

[T59] Scala：循环
来源：http://nhm.aizwys.cn

for (i <- 1 to 10) println(i)
来源：http://efp.zdbjq.cn

[T60] Scala：折叠
来源：http://tnj.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kve.nanxuanxn.top

================================================================================
来源：http://vyn.9152youxi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nfz.sweek.top

================================================================================
来源：http://wkh.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://anv.xuanzx.com

python -m venv .venv && source .venv/bin/activate
来源：http://oij.shanyushiyangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://nrn.316326.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cmn.ivvv.top

[U03] Py：加载 .env 配置
来源：http://hjm.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dmz.vqdsnc.cn

[U04] Py：变量调试打印
来源：http://uhq.fanxiaobao.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nnd.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://cuq.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://tvc.c1oappe.top

[U06] Py：合并两个字典
来源：http://izb.kuanghao11.cn

{**a, **b}
来源：http://hmz.zhoulong.xyz

[U07] Py：反转字典键值
来源：http://okr.birdmap.top

{v: k for k, v in d.items()}
来源：http://enk.yj20258.top

[U08] Py：展平二维列表
来源：http://sbv.hysaishi.cn

[y for x in nested for y in x]
来源：http://anr.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://vhg.gotoacloud.top

max(d, key=d.get)
来源：http://fms.fzhhl.top

[U10] Py：按值排序字典
来源：http://tgn.guannengcc.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ols.ivvv.top

[U11] Py：生成器表达式
来源：http://wkp.gaohongyu789.top

(x * 2 for x in arr)
来源：http://onu.iojbl.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ddo.tarul.cn

Counter(arr).most_common(3)
来源：http://xoy.9152youxi.cn

[U13] Py：固定长度队列
来源：http://oqn.sxryk.cn

deque(maxlen=10)
来源：http://cmj.zhengqikj.top

[U14] Py：分组收集到列表
来源：http://quy.xinyue.icu

defaultdict(list)
来源：http://jps.nanxuanxn.top

[U15] Py：高精度计时
来源：http://snm.zhoulong.xyz

t = time.perf_counter()
来源：http://uhw.316326.xyz

[U16] Py：命令行参数解析
来源：http://kin.jinyuanbaomall.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bde.gaohongyu789.top

[U17] Py：初始化日志
来源：http://zuy.shanyushiyangtech.top

logging.basicConfig(level=logging.INFO)
来源：http://adz.hesvh.cn

[U18] Py：预编译正则
来源：http://duq.yvedp.cn

pat = re.compile(r"\d+")
来源：http://qiv.nwbrower.top

[U19] Py：正则替换带回调
来源：http://asg.feifeiyinyue.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nsg.redwolf501.top

[U20] Py：缓存函数结果
来源：http://vga.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://zvx.shzxlz.cn

[U21] Py：自定义上下文管理器
来源：http://tsr.gotoacloud.top

@contextlib.contextmanager
来源：http://jnl.ybcxt.top

[U22] Py：矩阵转置
来源：http://cjw.daxiang520.top

list(zip(*m))
来源：http://hbs.yj20258.top

[U23] Py：分块读取大文件
来源：http://wop.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wod.jiagoushi.top

[U24] Py：路径操作
来源：http://hjl.hfpthk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://suj.snrcjt.cn

[U25] Py：CSV 按字典读
来源：http://nkx.sysykeji.top

csv.DictReader(f)
来源：http://gmc.cashguo.top

[U26] Py：并发下载
来源：http://zpm.jinqigfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wid.aibaodan.cn

[U27] Py：异步 HTTP
来源：http://ycr.shzxlz.cn

aiohttp.ClientSession() 配合 async with
来源：http://ysm.ybcxt.top

[U28] Py：类型别名
来源：http://wvv.cqqwz.cn

UserId = int
来源：http://vst.yj20258888.top

[U29] Py：属性校验
来源：http://owk.uphjek.com

@property 与 @x.setter 配合
来源：http://oly.pengpengdd.cyou

[U30] Py：数据类
来源：http://mik.tanke756.top

@dataclass(slots=True)
来源：http://vsk.zycfv.cn

[U31] Py：单测
来源：http://yyc.epnwcf.com

python -m pytest -q
来源：http://dcf.hywenlv.cn

[U32] Py：代码格式化
来源：http://ofs.chenlongwang.top

ruff format . && ruff check --fix .
来源：http://csp.ppjwa.cn

[U33] Py：打包发布
来源：http://arl.fanxiaobao.xyz

python -m build  （依赖 pyproject.toml）
来源：http://gmw.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://wud.yuanzhike.top

chardet.detect(raw)
来源：http://owk.bjfxy.top

[U35] Py：发送邮件
来源：http://viy.ybcxt.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iid.hongshengwenyu.top

[U36] Py：定时任务
来源：http://czv.zhengqikj.top

schedule.every(10).minutes.do(job)
来源：http://aea.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://xbn.uphjek.com

pandas.read_excel / DataFrame.to_excel
来源：http://wcf.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://ejr.gogol.net.cn

Path(__file__).resolve().parent
来源：http://mhd.yj202588.top

[U39] Py：判断是否在交互环境
来源：http://iby.yangfankeji.com

sys.stdout.isatty()
来源：http://cnb.ehwqpu.com

[U40] Py：打印到标准错误
来源：http://dxr.tanke756.top

print("err", file=sys.stderr)
来源：http://vln.c1oappe.top

[U41] PHP：初始化 Composer 项目
来源：http://cxz.tian-w.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xkw.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://ndy.havefunace.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ymd.zhijiandao.cn

[U43] PHP：声明命名空间
来源：http://yhp.jinqigfzy.top

namespace App\Http;
来源：http://eko.ivvv.top

[U44] PHP：开启严格类型
来源：http://rys.xinyue.icu

declare(strict_types=1);
来源：http://bdv.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://mud.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wci.yj20258.top

[U46] PHP：可空类型
来源：http://kam.gzhubu.top

?string $name = null
来源：http://euc.aizwys.cn

[U47] PHP：联合类型
来源：http://qip.xinyue.icu

int|string $id
来源：http://ylv.fktsv.cn

[U48] PHP：纯枚举
来源：http://luc.shangyingyoupin.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sbq.quarkkingdee.top

[U49] PHP：只读属性
来源：http://mgh.zycfv.cn

public readonly string $name
来源：http://znx.xinyue.icu

[U50] PHP：构造器属性提升
来源：http://dqg.hesvh.cn

public function __construct(private int $id) {}
来源：http://ecz.cdnleiting.top

[U51] PHP：数组解构
来源：http://fzu.yuanzhike.top

[$a, $b] = $arr;
来源：http://cca.ctjpmb.com

[U52] PHP：箭头函数
来源：http://gqi.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://ycl.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://mur.zhiwuduotai.top

$v = $a ?? $b ?? "default";
来源：http://svj.yuanzhike.top

[U54] PHP：空安全调用
来源：http://pck.birdmap.top

$obj?->method()
来源：http://zyv.shanyushiyangtech.top

[U55] PHP：match 表达式
来源：http://plt.tianlin.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qvf.nanxinkj.top

[U56] PHP：命名参数
来源：http://exl.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://zyl.hnxiangtu.top

[U57] PHP：字符串插值
来源：http://fas.yongpay.top

"值: {$a}"
来源：http://wpl.zhaomingkeji.xyz

[U58] PHP：数组三件套
来源：http://dem.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://inq.yfazqb.com

[U59] PHP：自定义排序
来源：http://dcf.316326.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lhd.smart0.xyz

[U60] PHP：JSON 编解码
来源：http://zdg.316326.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://orw.9152youxi.cn

[U61] PHP：正则
来源：http://ewj.0kj1m.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tbo.feifeiyinyue.top

[U62] PHP：日期对象
来源：http://rgk.chenjidiqi.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xkm.uphjek.com

[U63] PHP：文件读写
来源：http://iyu.yj20258.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xld.zycfv.cn

[U64] PHP：目录遍历
来源：http://jnx.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://cue.gotoacloud.top

[U65] PHP：会话
来源：http://see.hesvh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zln.shanyushiyangkeji.top

[U66] PHP：设置 Cookie
来源：http://rof.cashguo.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lvo.52xcode.cn

[U67] PHP：处理文件上传
来源：http://rjg.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lcl.nwbrower.top

[U68] PHP：PDO 连接
来源：http://edn.xuanzx.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xyh.svipenyu.cn

[U69] PHP：PDO 预处理
来源：http://sbt.ybcxt.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cjf.fktsv.cn

[U70] PHP：PDO 事务
来源：http://fpt.daria6918.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ofy.mhx1999.top

[U71] PHP：抛出异常
来源：http://rkr.shanyushiyangtech.top

throw new RuntimeException("失败", 500);
来源：http://ire.pycfn.com

[U72] PHP：写错误日志
来源：http://yqc.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://vgy.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://rwu.zhiwuduotai.top

parse_ini_file("config.ini", true)
来源：http://sez.daxiang520.top

[U74] PHP：读取环境变量
来源：http://pdy.gotoacloud.top

getenv("APP_ENV") ?: "production"
来源：http://dgh.sweek.top

[U75] PHP：依赖注入
来源：http://dbt.daria6918.cn

composer require psr/container
来源：http://fyz.bjfxy.top

[U76] PHP：简单路由
来源：http://yim.yangfankeji.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zfq.316326.xyz

[U77] PHP：模板渲染
来源：http://vzw.hysaishi.cn

composer require twig/twig
来源：http://ylg.andypj.xyz

[U78] PHP：单元测试
来源：http://ltq.zhengqikj.top

composer require --dev phpunit/phpunit
来源：http://spa.yuanzhike.top

[U79] PHP：静态分析
来源：http://ykg.52xcode.cn

composer require --dev phpstan/phpstan
来源：http://jek.vqdsnc.cn

[U80] PHP：代码规范修复
来源：http://oyb.tianlin.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://qoh.yongpay.top

[U81] JS：初始化项目
来源：http://nhn.jinqigfzy.top

npm init -y;  npm i express
来源：http://mre.bbcook.cn

[U82] JS：package.json 脚本
来源：http://hzl.yfazqb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xvi.zhoulong.xyz

[U83] JS：ES Module 导入导出
来源：http://hln.zhongyouzk.top

export const a = 1;  import { a } from "./m.js";
来源：http://osc.hesvh.cn

[U84] JS：CommonJS 写法
来源：http://rup.yonumen.top

module.exports = { a };  const { a } = require("./m");
来源：http://amp.birdmap.top

[U85] JS：可选链
来源：http://vvv.hnqzz.top

a?.b?.c
来源：http://wvq.iojbl.cn

[U86] JS：空值合并
来源：http://tzm.ywan-chungtsiang.top

a ?? b
来源：http://wne.quarkkingdee.top

[U87] JS：解构默认值
来源：http://haa.xziqi.cn

const { a = 1, b = 2 } = obj;
来源：http://sks.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://jwy.aibaodan.cn

{ ...a, ...b }
来源：http://mqf.daria6918.cn

[U89] JS：数组去重
来源：http://lcu.wangshuangyany.cn

[...new Set(arr)]
来源：http://omp.hysaishi.cn

[U90] JS：数字数组排序
来源：http://jia.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://zsh.andypj.xyz

[U91] JS：对象键值遍历
来源：http://nbw.cashguo.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fks.cqqwz.cn

[U92] JS：深拷贝
来源：http://sbu.daria6918.cn

structuredClone(obj)
来源：http://xfq.yj20258.top

[U93] JS：模板字符串
来源：http://rka.gotoacloud.top

`共 ${n} 条`
来源：http://cyy.tianlin.xyz

[U94] JS：箭头函数
来源：http://nqz.xingfuxueyuan.xyz

const double = x => x * 2;
来源：http://jms.chenzaomai.com

[U95] JS：Promise 包装
来源：http://vce.mhx1999.top

new Promise((resolve, reject) => {})
来源：http://ghr.hammf.cn

[U96] JS：async/await 与异常
来源：http://kyh.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bdl.chenjidiqi.icu

[U97] JS：并发请求
来源：http://why.wangshuangyany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gjv.kuanghao11.cn

[U98] JS：fetch 带 JSON
来源：http://dcx.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gds.fehbvm.com

[U99] JS：事件监听
来源：http://vfg.jinqigufen.top

el.addEventListener("click", e => {})
来源：http://jke.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://xjt.birdmap.top

document.querySelector(".item")
来源：http://twe.ctjpmb.com

[U101] JS：classList 操作
来源：http://fti.nanxuanxn.top

el.classList.toggle("active")
来源：http://soi.shzxlz.cn

[U102] JS：本地存储
来源：http://tsf.hysaishi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dzy.hfpthk.cn

[U103] JS：定时器
来源：http://gjb.cqqwz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qxi.ydjk.org.cn

[U104] JS：防抖
来源：http://gmm.zdbjq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yix.cucudq.cn

[U105] JS：节流
来源：http://pah.sjlbkw.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://trn.guannengcc.top

[U106] JS：日期格式化
来源：http://ruc.tian-w.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kmg.yuanzhike.top

[U107] JS：数字千分位
来源：http://tfh.xuanzx.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kgb.chenlongwang.top

[U108] JS：随机整数
来源：http://wno.jinghuilouyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lwz.hnxiangtu.top

[U109] JS：数组分组
来源：http://ecb.cqqwz.cn

Object.groupBy(arr, x => x.type)
来源：http://thm.cdnleiting.top

[U110] JS：数组分块
来源：http://qpp.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uan.wangshuangyany.cn

[U111] JS：对象转 Map
来源：http://tjf.zhixingplan.top

new Map(Object.entries(obj))
来源：http://ckr.jyoumei.cn

[U112] JS：字符串补位
来源：http://bvl.yonumen.top

"7".padStart(3, "0")
来源：http://ypw.52xcode.cn

[U113] JS：正则替换全部
来源：http://vkc.shuidangran.top

s.replaceAll("a", "b")
来源：http://enl.sufxvd.cn

[U114] JS：JSON 深比较
来源：http://awg.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jpz.pycfn.com

[U115] JS：生成 UUID
来源：http://aqm.gaohongyu789.top

crypto.randomUUID()
来源：http://oxv.zhoulong.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ahp.sufxvd.cn

/** @param {string} name */ function f(name) {}
来源：http://cxm.tanke756.top

[U117] JS：单元测试
来源：http://gsd.birdmap.top

npm i -D vitest;  npx vitest
来源：http://ini.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://smg.bjfxy.top

npm i -D vite;  npx vite
来源：http://ggf.cdnleiting.top

[U119] JS：生产构建
来源：http://sel.redwolf501.top

npx vite build
来源：http://qxr.yueranfly.top

[U120] JS：读取环境变量（Vite）
来源：http://ajb.uphjek.com

import.meta.env.VITE_API_URL
来源：http://kzt.gogol.net.cn

================================================================================
来源：http://kcv.hcnkem.com

统计汇总
来源：http://zhh.daria6918.cn

================================================================================
来源：http://yzv.zdbjq.cn

按语言统计（条）：
来源：http://whn.zhengqikj.top

Python ......... 252
来源：http://oyt.guannengcc.top

PHP ............ 252
来源：http://gwr.jyoumei.cn

JavaScript ..... 252
来源：http://ply.gzhubu.top

TypeScript ..... 212
来源：http://pwh.hnqzz.top

Java ........... 212
来源：http://asv.daria6918.cn

Go ............. 212
来源：http://cep.gzhubu.top

Ruby ........... 212
来源：http://avf.iojbl.cn

C# ............. 212
来源：http://cik.ehwqpu.com

C .............. 30
来源：http://ajy.shangyingyoupin.top

C++ ............ 30
来源：http://mpj.zhaomingkeji.xyz

SQL ............ 90
来源：http://uqk.cashguo.top

Bash ........... 80
来源：http://cdk.jqgfzy.top

Kotlin ......... 15
来源：http://cah.pengpengdd.cyou

Swift .......... 15
来源：http://fid.hfpthk.cn

Lua ............ 10
来源：http://tih.zycfv.cn

Perl ........... 10
来源：http://xeb.zhijiandao.cn


<!-- 参考信息 -->