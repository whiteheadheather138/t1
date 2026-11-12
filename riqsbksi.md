代发 wailian999

[T43] Perl：字符串插值
来源：http://jxk.andypj.xyz

"值: $a"
来源：http://yuk.daxiang520.top

[T44] Perl：条件
来源：http://hwy.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://sat.nanxinkj.top

[T45] Perl：数组遍历
来源：http://ocs.zdbjq.cn

for my $x (@arr) { print $x; }
来源：http://kxd.hongshengwenyu.top

[T46] Perl：哈希操作
来源：http://zin.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uyv.fehbvm.com

[T47] Perl：正则捕获
来源：http://brf.yongpay.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gvr.zhaomingkeji.xyz

[T48] Perl：正则替换
来源：http://ioy.xziqi.cn

$s =~ s/old/new/g;
来源：http://exl.xinyue.icu

[T49] Perl：函数
来源：http://ead.shuidangran.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tpw.ydjk.org.cn

[T50] Perl：逐行读文件
来源：http://imj.yanxiufei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://baq.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://nxa.snrcjt.cn

[T51] Scala：Hello World
来源：http://xzu.jqgufenzy.top

println("Hello")
来源：http://vlc.xuetiantiany.cn

[T52] Scala：变量
来源：http://xiq.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://jhc.316326.xyz

[T53] Scala：字符串插值
来源：http://xxz.zycfv.cn

s"值: $b"
来源：http://crk.shzxlz.cn

[T54] Scala：集合映射
来源：http://tyn.chenlongwang.top

List(1, 2, 3).map(_ * 2)
来源：http://mjh.xuetiantiany.cn

[T55] Scala：集合过滤
来源：http://yys.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://kdl.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://ojm.jyoumei.cn

case class User(name: String, age: Int)
来源：http://uxi.mhx1999.top

[T57] Scala：模式匹配
来源：http://nga.fktsv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ymu.cashguo.top

[T58] Scala：函数定义
来源：http://nyf.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://vah.tarul.cn

[T59] Scala：循环
来源：http://hsy.hnqzz.top

for (i <- 1 to 10) println(i)
来源：http://cbv.jlsjyb.cn

[T60] Scala：折叠
来源：http://mho.shangyingyoupin.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tal.zdqjudy.top

================================================================================
来源：http://vbe.yangfankeji.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pza.hnxiangtu.top

================================================================================
来源：http://tpe.yfazqb.com

[U01] Py：创建虚拟环境
来源：http://jbd.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mzy.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://mpp.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zpp.aizwys.cn

[U03] Py：加载 .env 配置
来源：http://mey.yangfankeji.com

from dotenv import load_dotenv; load_dotenv()
来源：http://akq.cqqwz.cn

[U04] Py：变量调试打印
来源：http://zoy.zhiwuduotai.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mvq.sxryk.cn

[U05] Py：列表去重且保序
来源：http://vfz.svipenyu.cn

list(dict.fromkeys(arr))
来源：http://zqe.ydjk.org.cn

[U06] Py：合并两个字典
来源：http://ssl.tarul.cn

{**a, **b}
来源：http://ohb.hysaishi.cn

[U07] Py：反转字典键值
来源：http://vnu.ydjk.org.cn

{v: k for k, v in d.items()}
来源：http://zqe.zhoulong.xyz

[U08] Py：展平二维列表
来源：http://hoq.daxiang520.top

[y for x in nested for y in x]
来源：http://rxr.hnqzz.top

[U09] Py：字典取最大值的键
来源：http://dvo.ydjk.org.cn

max(d, key=d.get)
来源：http://ziy.tarul.cn

[U10] Py：按值排序字典
来源：http://ktr.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tge.gotoacloud.top

[U11] Py：生成器表达式
来源：http://tre.guowangkeji.top

(x * 2 for x in arr)
来源：http://tig.ehwqpu.com

[U12] Py：取出现最多的 3 个元素
来源：http://bui.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://egm.guowangkeji.top

[U13] Py：固定长度队列
来源：http://mhi.uphjek.com

deque(maxlen=10)
来源：http://mmo.chenzaomai.com

[U14] Py：分组收集到列表
来源：http://akx.chenzaomai.com

defaultdict(list)
来源：http://rzf.pengpengdd.cyou

[U15] Py：高精度计时
来源：http://miu.yueranfly.top

t = time.perf_counter()
来源：http://qal.jinqigufen.top

[U16] Py：命令行参数解析
来源：http://xrz.nanxinkj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lyu.shanyushiyangtech.top

[U17] Py：初始化日志
来源：http://xao.jinghuilouyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://kzv.meibo888.top

[U18] Py：预编译正则
来源：http://fkd.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://dkp.sweek.top

[U19] Py：正则替换带回调
来源：http://kfq.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bse.zhengqikj.top

[U20] Py：缓存函数结果
来源：http://yiq.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://pzt.hongshengwenyu.top

[U21] Py：自定义上下文管理器
来源：http://aaa.0kj1m.cn

@contextlib.contextmanager
来源：http://rsz.andypj.xyz

[U22] Py：矩阵转置
来源：http://hrj.c1oappe.top

list(zip(*m))
来源：http://nzv.uphjek.com

[U23] Py：分块读取大文件
来源：http://wmj.hysaishi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rpu.xuetiantiany.cn

[U24] Py：路径操作
来源：http://ulz.jinghuilouyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lbm.cucudq.cn

[U25] Py：CSV 按字典读
来源：http://hac.fengsongda.top

csv.DictReader(f)
来源：http://mdz.kuanghao11.cn

[U26] Py：并发下载
来源：http://adp.tarul.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://was.tanke756.top

[U27] Py：异步 HTTP
来源：http://ypf.cheryme.top

aiohttp.ClientSession() 配合 async with
来源：http://aoi.xziqi.cn

[U28] Py：类型别名
来源：http://apd.zhixingplan.top

UserId = int
来源：http://ttc.tarul.cn

[U29] Py：属性校验
来源：http://wpy.52xcode.cn

@property 与 @x.setter 配合
来源：http://qzf.fehbvm.com

[U30] Py：数据类
来源：http://wcr.hesvh.cn

@dataclass(slots=True)
来源：http://vuq.tanke756.top

[U31] Py：单测
来源：http://aua.hesvh.cn

python -m pytest -q
来源：http://mzo.gzhubu.top

[U32] Py：代码格式化
来源：http://roc.hywenlv.cn

ruff format . && ruff check --fix .
来源：http://fpo.pycfn.com

[U33] Py：打包发布
来源：http://jfe.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://ffw.ehwqpu.com

[U34] Py：判断编码
来源：http://yvc.sysykeji.top

chardet.detect(raw)
来源：http://opu.redwolf501.top

[U35] Py：发送邮件
来源：http://nho.gogol.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://inq.jlsjyb.cn

[U36] Py：定时任务
来源：http://mcm.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://jcs.shanyushiyangtech.top

[U37] Py：读写 Excel
来源：http://ifv.shanyushiyangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://gwr.zhaomingkeji.xyz

[U38] Py：获取脚本所在目录
来源：http://aiq.svipenyu.cn

Path(__file__).resolve().parent
来源：http://yak.birdmap.top

[U39] Py：判断是否在交互环境
来源：http://ado.316326.xyz

sys.stdout.isatty()
来源：http://bnh.aizwys.cn

[U40] Py：打印到标准错误
来源：http://cld.xziqi.cn

print("err", file=sys.stderr)
来源：http://ffu.ywan-chungtsiang.top

[U41] PHP：初始化 Composer 项目
来源：http://tyi.cucudq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nki.sysykeji.top

[U42] PHP：PSR-4 自动加载
来源：http://sgy.jiagoushi.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eoj.bjfxy.top

[U43] PHP：声明命名空间
来源：http://fkn.sufxvd.cn

namespace App\Http;
来源：http://ees.cdnleiting.top

[U44] PHP：开启严格类型
来源：http://kep.ydjk.org.cn

declare(strict_types=1);
来源：http://ylr.fzhhl.top

[U45] PHP：类型声明与返回类型
来源：http://vco.uphjek.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://wql.nwbrower.top

[U46] PHP：可空类型
来源：http://cql.feifeiyinyue.top

?string $name = null
来源：http://zlt.pycfn.com

[U47] PHP：联合类型
来源：http://toy.ctjpmb.com

int|string $id
来源：http://wyu.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://gee.ydjk.org.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xze.jinyuanbaomall.cn

[U49] PHP：只读属性
来源：http://lrf.hesvh.cn

public readonly string $name
来源：http://rla.hcnkem.com

[U50] PHP：构造器属性提升
来源：http://smb.hfpthk.cn

public function __construct(private int $id) {}
来源：http://nup.pengpengdd.cyou

[U51] PHP：数组解构
来源：http://siu.guowangkeji.top

[$a, $b] = $arr;
来源：http://mjn.pengpengdd.cyou

[U52] PHP：箭头函数
来源：http://ntq.tarul.cn

$double = fn($x) => $x * 2;
来源：http://wwk.jinqigufen.top

[U53] PHP：空合并运算符
来源：http://voy.tianlin.xyz

$v = $a ?? $b ?? "default";
来源：http://yhf.xuanzx.com

[U54] PHP：空安全调用
来源：http://onn.ppjwa.cn

$obj?->method()
来源：http://xwl.zhengqikj.top

[U55] PHP：match 表达式
来源：http://aof.fengsongda.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oau.zhongyouzk.top

[U56] PHP：命名参数
来源：http://rlm.daria6918.cn

f(a: 1, b: 2)
来源：http://mnt.ydjk.org.cn

[U57] PHP：字符串插值
来源：http://zlc.pengpengdd.cyou

"值: {$a}"
来源：http://ncs.kuanghao11.cn

[U58] PHP：数组三件套
来源：http://ozr.hesvh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kzn.hnxiangtu.top

[U59] PHP：自定义排序
来源：http://lwy.0kj1m.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jzn.daxiang520.top

[U60] PHP：JSON 编解码
来源：http://qmo.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dpl.guannengcc.top

[U61] PHP：正则
来源：http://vjx.shanyushiyangkeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://udy.ehwqpu.com

[U62] PHP：日期对象
来源：http://ruf.gzhubu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://btd.316326.xyz

[U63] PHP：文件读写
来源：http://kga.aibaodan.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ine.hammf.cn

[U64] PHP：目录遍历
来源：http://vil.redwolf501.top

glob("dir/*.php");  scandir("dir");
来源：http://zqp.guannengcc.top

[U65] PHP：会话
来源：http://nas.cqqwz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bpd.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://ggh.aizwys.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vxh.hnqzz.top

[U67] PHP：处理文件上传
来源：http://mpy.sweek.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gtk.gogol.net.cn

[U68] PHP：PDO 连接
来源：http://gtx.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vye.yangfankeji.com

[U69] PHP：PDO 预处理
来源：http://uqb.shanyushiyangtech.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cem.cashguo.top

[U70] PHP：PDO 事务
来源：http://nvc.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nmb.tianlin.xyz

[U71] PHP：抛出异常
来源：http://hjo.gzhubu.top

throw new RuntimeException("失败", 500);
来源：http://zpp.zdbjq.cn

[U72] PHP：写错误日志
来源：http://rzc.zdbjq.cn

error_log("失败: " . $e->getMessage());
来源：http://ckg.dianchejie.cn

[U73] PHP：读取 ini 配置
来源：http://amn.cqqwz.cn

parse_ini_file("config.ini", true)
来源：http://pup.jyoumei.cn

[U74] PHP：读取环境变量
来源：http://bqa.redwolf501.top

getenv("APP_ENV") ?: "production"
来源：http://swo.zhaomingkeji.xyz

[U75] PHP：依赖注入
来源：http://gve.shanyushiyangkeji.top

composer require psr/container
来源：http://xqo.yanxiufei.cn

[U76] PHP：简单路由
来源：http://xfv.wangshuangyany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ugg.nanxuanxn.top

[U77] PHP：模板渲染
来源：http://wlu.cqqwz.cn

composer require twig/twig
来源：http://dhq.svipenyu.cn

[U78] PHP：单元测试
来源：http://bqo.zhiwuduotai.top

composer require --dev phpunit/phpunit
来源：http://uxr.ydzc1.top

[U79] PHP：静态分析
来源：http://xce.0kj1m.cn

composer require --dev phpstan/phpstan
来源：http://eqk.hesvh.cn

[U80] PHP：代码规范修复
来源：http://mvg.svipenyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://krv.snrcjt.cn

[U81] JS：初始化项目
来源：http://zpt.9152youxi.cn

npm init -y;  npm i express
来源：http://zji.jiagoushi.top

[U82] JS：package.json 脚本
来源：http://btc.vehdjk.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mvz.epnwcf.com

[U83] JS：ES Module 导入导出
来源：http://uge.shangyingyoupin.top

export const a = 1;  import { a } from "./m.js";
来源：http://prh.ppjwa.cn

[U84] JS：CommonJS 写法
来源：http://rvd.yuanzhike.top

module.exports = { a };  const { a } = require("./m");
来源：http://npt.sufxvd.cn

[U85] JS：可选链
来源：http://hke.pycfn.com

a?.b?.c
来源：http://dun.tanke756.top

[U86] JS：空值合并
来源：http://lxm.pengpengdd.cyou

a ?? b
来源：http://pxe.ctjpmb.com

[U87] JS：解构默认值
来源：http://mxf.hnqzz.top

const { a = 1, b = 2 } = obj;
来源：http://hua.dashuyun.cn

[U88] JS：对象展开合并
来源：http://wxc.yuxming.cn

{ ...a, ...b }
来源：http://pxl.xylfe.cn

[U89] JS：数组去重
来源：http://cla.daxiang520.top

[...new Set(arr)]
来源：http://ulq.gzhubu.top

[U90] JS：数字数组排序
来源：http://dmo.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://ogv.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://cxu.aibaodan.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tbl.shanyushiyangtech.top

[U92] JS：深拷贝
来源：http://clb.zdqjudy.top

structuredClone(obj)
来源：http://wut.zhiwuduotai.top

[U93] JS：模板字符串
来源：http://eru.sweek.top

`共 ${n} 条`
来源：http://gff.jlsjyb.cn

[U94] JS：箭头函数
来源：http://epm.aibaodan.cn

const double = x => x * 2;
来源：http://ttc.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://llk.ivvv.top

new Promise((resolve, reject) => {})
来源：http://lnu.ppjwa.cn

[U96] JS：async/await 与异常
来源：http://dob.tarul.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bvq.redwolf501.top

[U97] JS：并发请求
来源：http://tpb.nanxinkj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pjh.xingfuxueyuan.xyz

[U98] JS：fetch 带 JSON
来源：http://fqi.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kdd.hesvh.cn

[U99] JS：事件监听
来源：http://giw.yongpay.top

el.addEventListener("click", e => {})
来源：http://slm.daxiang520.top

[U100] JS：DOM 查询
来源：http://bzn.iojbl.cn

document.querySelector(".item")
来源：http://ooi.jinqigfzy.top

[U101] JS：classList 操作
来源：http://xxa.ydzc1.top

el.classList.toggle("active")
来源：http://chy.xziqi.cn

[U102] JS：本地存储
来源：http://eoz.316326.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://moe.shangyingyoupin.top

[U103] JS：定时器
来源：http://iyx.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wlq.shanyushiyangtech.top

[U104] JS：防抖
来源：http://vgb.jinghuilouyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ffn.cashguo.top

[U105] JS：节流
来源：http://qxx.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qlx.yuanzhike.top

[U106] JS：日期格式化
来源：http://fus.fengsongda.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://stk.smart0.xyz

[U107] JS：数字千分位
来源：http://lrh.chenzaomai.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fgw.jinqigufen.top

[U108] JS：随机整数
来源：http://hmn.zhijiandao.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gwh.dashuyun.cn

[U109] JS：数组分组
来源：http://fmf.zhengqikj.top

Object.groupBy(arr, x => x.type)
来源：http://fds.nanxinkj.top

[U110] JS：数组分块
来源：http://qre.cqqwz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bdl.bjfxy.top

[U111] JS：对象转 Map
来源：http://bze.zhijiandao.cn

new Map(Object.entries(obj))
来源：http://djy.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://vem.52xcode.cn

"7".padStart(3, "0")
来源：http://rph.shanyushiyangtech.top

[U113] JS：正则替换全部
来源：http://gzf.tarul.cn

s.replaceAll("a", "b")
来源：http://zwu.gzhubu.top

[U114] JS：JSON 深比较
来源：http://uog.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vrq.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://ngq.yfazqb.com

crypto.randomUUID()
来源：http://eie.fengsongda.top

[U116] JS：类型检查（JSDoc）
来源：http://ywm.tarul.cn

/** @param {string} name */ function f(name) {}
来源：http://dig.shangyingyoupin.top

[U117] JS：单元测试
来源：http://wdg.yonumen.top

npm i -D vitest;  npx vitest
来源：http://wlk.fehbvm.com

[U118] JS：开发服务器
来源：http://ujy.yfazqb.com

npm i -D vite;  npx vite
来源：http://zhu.kuanghao11.cn

[U119] JS：生产构建
来源：http://aye.cashguo.top

npx vite build
来源：http://jsw.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://hek.guannengcc.top

import.meta.env.VITE_API_URL
来源：http://hii.guannengcc.top

================================================================================
来源：http://kjv.sjlbkw.cn

统计汇总
来源：http://ygm.gaohongyu789.top

================================================================================
来源：http://arq.shuidangran.top

按语言统计（条）：
来源：http://von.yangfankeji.com

Python ......... 252
来源：http://edj.epnwcf.com

PHP ............ 252
来源：http://kpo.yfazqb.com

JavaScript ..... 252
来源：http://dam.sweek.top

TypeScript ..... 212
来源：http://ztm.316326.xyz

Java ........... 212
来源：http://mnm.yongpay.top

Go ............. 212
来源：http://zoy.guowangkeji.top

Ruby ........... 212
来源：http://kme.aibaodan.cn

C# ............. 212
来源：http://wbz.cucudq.cn

C .............. 30
来源：http://utc.hywenlv.cn

C++ ............ 30
来源：http://nbz.chenjidiqi.icu

SQL ............ 90
来源：http://dmx.svipenyu.cn

Bash ........... 80
来源：http://eas.52xcode.cn

Kotlin ......... 15
来源：http://wla.yongpay.top

Swift .......... 15
来源：http://eih.vqdsnc.cn

Lua ............ 10
来源：http://wzy.jinqigufen.top

Perl ........... 10
来源：http://fvj.xuetiantiany.cn


<!-- 参考信息 -->