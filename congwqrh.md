代发 wailian999

[T45] Perl：数组遍历
来源：http://bss.yanxiufei.cn

for my $x (@arr) { print $x; }
来源：http://qjq.yangfankeji.com

[T46] Perl：哈希操作
来源：http://mie.0kj1m.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wku.hnxiangtu.top

[T47] Perl：正则捕获
来源：http://xsp.vehdjk.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://ruj.yanxiufei.cn

[T48] Perl：正则替换
来源：http://ceh.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://njp.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://fho.hnxiangtu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ams.xinyue.icu

[T50] Perl：逐行读文件
来源：http://qhl.jyoumei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mzj.kuanghao11.cn

while (my $line = <$fh>) { print $line; }
来源：http://ncu.chenlongwang.top

[T51] Scala：Hello World
来源：http://wwc.52xcode.cn

println("Hello")
来源：http://ude.yonumen.top

[T52] Scala：变量
来源：http://wpp.aibaodan.cn

val a = 1;  var b = 2
来源：http://ebd.wangdashe.top

[T53] Scala：字符串插值
来源：http://odp.quarkkingdee.top

s"值: $b"
来源：http://zqi.guowangkeji.top

[T54] Scala：集合映射
来源：http://lmk.gaohongyu789.top

List(1, 2, 3).map(_ * 2)
来源：http://urk.jianghu66.top

[T55] Scala：集合过滤
来源：http://zht.yuanzhike.top

List(1, 2, 3).filter(_ > 1)
来源：http://chp.snrcjt.cn

[T56] Scala：样例类
来源：http://epp.xinyue.icu

case class User(name: String, age: Int)
来源：http://wen.cdnleiting.top

[T57] Scala：模式匹配
来源：http://pjj.haohaochexian.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mep.mhx1999.top

[T58] Scala：函数定义
来源：http://jew.bbcook.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lqc.316326.xyz

[T59] Scala：循环
来源：http://xms.zhongyouzk.top

for (i <- 1 to 10) println(i)
来源：http://ska.meibo888.top

[T60] Scala：折叠
来源：http://ndv.hcnkem.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jlf.aizwys.cn

================================================================================
来源：http://mvg.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xvw.yonumen.top

================================================================================
来源：http://szq.redwolf501.top

[U01] Py：创建虚拟环境
来源：http://gsg.shangyingyoupin.top

python -m venv .venv && source .venv/bin/activate
来源：http://bmq.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://ngu.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vqa.xingfuxueyuan.xyz

[U03] Py：加载 .env 配置
来源：http://ryf.aizwys.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jiw.hesvh.cn

[U04] Py：变量调试打印
来源：http://nlt.uphjek.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qri.haohaochexian.top

[U05] Py：列表去重且保序
来源：http://nuz.gogol.net.cn

list(dict.fromkeys(arr))
来源：http://yrv.ywan-chungtsiang.top

[U06] Py：合并两个字典
来源：http://anb.snrcjt.cn

{**a, **b}
来源：http://fri.zhiwuduotai.top

[U07] Py：反转字典键值
来源：http://kla.tian-w.cn

{v: k for k, v in d.items()}
来源：http://jkt.hysaishi.cn

[U08] Py：展平二维列表
来源：http://iiz.hnxiangtu.top

[y for x in nested for y in x]
来源：http://lrp.xuanzx.com

[U09] Py：字典取最大值的键
来源：http://une.tarul.cn

max(d, key=d.get)
来源：http://hej.zhengqikj.top

[U10] Py：按值排序字典
来源：http://hpo.yuanzhike.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://syf.chenzaomai.com

[U11] Py：生成器表达式
来源：http://kfc.haohaochexian.top

(x * 2 for x in arr)
来源：http://vqt.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://rhj.dianchejie.cn

Counter(arr).most_common(3)
来源：http://cdd.snrcjt.cn

[U13] Py：固定长度队列
来源：http://uko.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://nmv.hesvh.cn

[U14] Py：分组收集到列表
来源：http://sop.yj202588.top

defaultdict(list)
来源：http://yqp.kuanghao11.cn

[U15] Py：高精度计时
来源：http://ljg.ehwqpu.com

t = time.perf_counter()
来源：http://iaz.svipenyu.cn

[U16] Py：命令行参数解析
来源：http://foi.gotoacloud.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tdp.shanyushiyangtech.top

[U17] Py：初始化日志
来源：http://snk.cdnleiting.top

logging.basicConfig(level=logging.INFO)
来源：http://xng.ydzc1.top

[U18] Py：预编译正则
来源：http://gxt.yuxming.cn

pat = re.compile(r"\d+")
来源：http://qbb.uphjek.com

[U19] Py：正则替换带回调
来源：http://hho.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tpa.smart0.xyz

[U20] Py：缓存函数结果
来源：http://yzc.sxryk.cn

@functools.lru_cache(maxsize=None)
来源：http://pon.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://gnt.jinqigufen.top

@contextlib.contextmanager
来源：http://tji.hammf.cn

[U22] Py：矩阵转置
来源：http://wup.cdnleiting.top

list(zip(*m))
来源：http://qpv.andypj.xyz

[U23] Py：分块读取大文件
来源：http://ycq.gzhubu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://idd.birdmap.top

[U24] Py：路径操作
来源：http://awz.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eze.yj20258888.top

[U25] Py：CSV 按字典读
来源：http://kdi.0kj1m.cn

csv.DictReader(f)
来源：http://ied.sxryk.cn

[U26] Py：并发下载
来源：http://krv.yuanzhike.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vlg.yuanzhike.top

[U27] Py：异步 HTTP
来源：http://lom.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://cjs.yuxming.cn

[U28] Py：类型别名
来源：http://hlj.jyoumei.cn

UserId = int
来源：http://hvx.gaohongyu789.top

[U29] Py：属性校验
来源：http://zrv.cdnleiting.top

@property 与 @x.setter 配合
来源：http://wzr.yanxiufei.cn

[U30] Py：数据类
来源：http://vyt.jinqigufen.top

@dataclass(slots=True)
来源：http://zkn.ehwqpu.com

[U31] Py：单测
来源：http://kgx.ybcxt.top

python -m pytest -q
来源：http://spa.pycfn.com

[U32] Py：代码格式化
来源：http://rod.tian-w.cn

ruff format . && ruff check --fix .
来源：http://qzv.iojbl.cn

[U33] Py：打包发布
来源：http://gtg.yvedp.cn

python -m build  （依赖 pyproject.toml）
来源：http://efb.cqqwz.cn

[U34] Py：判断编码
来源：http://uol.hnqzz.top

chardet.detect(raw)
来源：http://rxi.fzhhl.top

[U35] Py：发送邮件
来源：http://qgc.hammf.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://smj.gzhubu.top

[U36] Py：定时任务
来源：http://pyh.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://ikt.ehwqpu.com

[U37] Py：读写 Excel
来源：http://kkb.bbcook.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bkh.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://kss.c1oappe.top

Path(__file__).resolve().parent
来源：http://uot.yangfankeji.com

[U39] Py：判断是否在交互环境
来源：http://ubd.chenjidiqi.icu

sys.stdout.isatty()
来源：http://pra.cashguo.top

[U40] Py：打印到标准错误
来源：http://aft.zycfv.cn

print("err", file=sys.stderr)
来源：http://eri.chenzaomai.com

[U41] PHP：初始化 Composer 项目
来源：http://hsq.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://imq.ivvv.top

[U42] PHP：PSR-4 自动加载
来源：http://cet.vqdsnc.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eau.gaohongyu789.top

[U43] PHP：声明命名空间
来源：http://pmb.xingfuxueyuan.xyz

namespace App\Http;
来源：http://kat.gaohongyu789.top

[U44] PHP：开启严格类型
来源：http://uwl.hnxiangtu.top

declare(strict_types=1);
来源：http://bjf.ivvv.top

[U45] PHP：类型声明与返回类型
来源：http://bai.cucudq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mcq.ppjwa.cn

[U46] PHP：可空类型
来源：http://gqr.jinyuanbaomall.cn

?string $name = null
来源：http://uxv.smart0.xyz

[U47] PHP：联合类型
来源：http://mlm.jiagoushi.top

int|string $id
来源：http://vnn.chenzaomai.com

[U48] PHP：纯枚举
来源：http://edj.ivvv.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://alv.hywenlv.cn

[U49] PHP：只读属性
来源：http://gyz.shzxlz.cn

public readonly string $name
来源：http://yod.wangdashe.top

[U50] PHP：构造器属性提升
来源：http://fvb.pengpengdd.cyou

public function __construct(private int $id) {}
来源：http://etg.xuanzx.com

[U51] PHP：数组解构
来源：http://zvp.xziqi.cn

[$a, $b] = $arr;
来源：http://gus.xinyue.icu

[U52] PHP：箭头函数
来源：http://uhs.snrcjt.cn

$double = fn($x) => $x * 2;
来源：http://xzm.sysykeji.top

[U53] PHP：空合并运算符
来源：http://nds.gzhubu.top

$v = $a ?? $b ?? "default";
来源：http://ign.gaohongyu789.top

[U54] PHP：空安全调用
来源：http://jjm.xylfe.cn

$obj?->method()
来源：http://cup.fktsv.cn

[U55] PHP：match 表达式
来源：http://wln.pycfn.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kfa.quarkkingdee.top

[U56] PHP：命名参数
来源：http://zrr.gogol.net.cn

f(a: 1, b: 2)
来源：http://crl.guowangkeji.top

[U57] PHP：字符串插值
来源：http://ahf.zhongyouzk.top

"值: {$a}"
来源：http://pwz.fehbvm.com

[U58] PHP：数组三件套
来源：http://nzo.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zyg.tanke756.top

[U59] PHP：自定义排序
来源：http://omo.hesvh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://chp.hesvh.cn

[U60] PHP：JSON 编解码
来源：http://sbk.dashuyun.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://imx.haohaochexian.top

[U61] PHP：正则
来源：http://gqd.fengsongda.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://twf.yanxiufei.cn

[U62] PHP：日期对象
来源：http://vgv.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vkk.nanxuanxn.top

[U63] PHP：文件读写
来源：http://vvx.yj20258888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lvm.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://qiz.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://asr.ydzc1.top

[U65] PHP：会话
来源：http://gxn.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bpc.xuanzx.com

[U66] PHP：设置 Cookie
来源：http://xwh.fengsongda.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sbo.iojbl.cn

[U67] PHP：处理文件上传
来源：http://ktk.uphjek.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://laf.svipenyu.cn

[U68] PHP：PDO 连接
来源：http://bvx.jinqigfzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://srw.dashuyun.cn

[U69] PHP：PDO 预处理
来源：http://kpu.zhixingplan.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jbx.zycfv.cn

[U70] PHP：PDO 事务
来源：http://oxw.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ruu.fktsv.cn

[U71] PHP：抛出异常
来源：http://nhp.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://bgr.wangshuangyany.cn

[U72] PHP：写错误日志
来源：http://mbo.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://qce.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://nsj.ydzc1.top

parse_ini_file("config.ini", true)
来源：http://rfl.sjlbkw.cn

[U74] PHP：读取环境变量
来源：http://qru.jiagoushi.top

getenv("APP_ENV") ?: "production"
来源：http://xll.kuanghao11.cn

[U75] PHP：依赖注入
来源：http://igt.aizwys.cn

composer require psr/container
来源：http://cax.gogol.net.cn

[U76] PHP：简单路由
来源：http://ntb.smart0.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://prd.hnqzz.top

[U77] PHP：模板渲染
来源：http://pnk.chenlongwang.top

composer require twig/twig
来源：http://tmg.jinyuanbaomall.cn

[U78] PHP：单元测试
来源：http://zmj.fzhhl.top

composer require --dev phpunit/phpunit
来源：http://jdl.ydzc1.top

[U79] PHP：静态分析
来源：http://dqn.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://fpx.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://yqx.gogol.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://egc.yanxiufei.cn

[U81] JS：初始化项目
来源：http://pnk.aizwys.cn

npm init -y;  npm i express
来源：http://xel.svipenyu.cn

[U82] JS：package.json 脚本
来源：http://csg.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wyx.hysaishi.cn

[U83] JS：ES Module 导入导出
来源：http://phr.nanxinkj.top

export const a = 1;  import { a } from "./m.js";
来源：http://qzq.redwolf501.top

[U84] JS：CommonJS 写法
来源：http://olo.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://ddw.gotoacloud.top

[U85] JS：可选链
来源：http://ckq.jianghu66.top

a?.b?.c
来源：http://hgk.pengpengdd.cyou

[U86] JS：空值合并
来源：http://bug.fengsongda.top

a ?? b
来源：http://vrt.jinyuanbaomall.cn

[U87] JS：解构默认值
来源：http://qnp.zdbjq.cn

const { a = 1, b = 2 } = obj;
来源：http://vms.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://yww.tanke756.top

{ ...a, ...b }
来源：http://bbt.gaohongyu789.top

[U89] JS：数组去重
来源：http://xdp.shuidangran.top

[...new Set(arr)]
来源：http://gwp.gzhubu.top

[U90] JS：数字数组排序
来源：http://avm.9152youxi.cn

[...arr].sort((a, b) => a - b)
来源：http://zjp.smart0.xyz

[U91] JS：对象键值遍历
来源：http://ryt.aizwys.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xmq.hammf.cn

[U92] JS：深拷贝
来源：http://hbm.zhaomingkeji.xyz

structuredClone(obj)
来源：http://umd.9152youxi.cn

[U93] JS：模板字符串
来源：http://oux.gogol.net.cn

`共 ${n} 条`
来源：http://goq.ivvv.top

[U94] JS：箭头函数
来源：http://avz.c1oappe.top

const double = x => x * 2;
来源：http://ucq.hesvh.cn

[U95] JS：Promise 包装
来源：http://pzc.chenlongwang.top

new Promise((resolve, reject) => {})
来源：http://wgr.hammf.cn

[U96] JS：async/await 与异常
来源：http://nqo.sjlbkw.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pav.snrcjt.cn

[U97] JS：并发请求
来源：http://bes.guowangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://iyh.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://ewt.gogol.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vuv.tianlin.xyz

[U99] JS：事件监听
来源：http://eme.yangfankeji.com

el.addEventListener("click", e => {})
来源：http://lmh.yuanzhike.top

[U100] JS：DOM 查询
来源：http://crg.zhixingplan.top

document.querySelector(".item")
来源：http://oep.jianghu66.top

[U101] JS：classList 操作
来源：http://ihr.vehdjk.com

el.classList.toggle("active")
来源：http://cwz.52xcode.cn

[U102] JS：本地存储
来源：http://jhu.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://doz.xziqi.cn

[U103] JS：定时器
来源：http://sen.dashuyun.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vbe.sjlbkw.cn

[U104] JS：防抖
来源：http://akq.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uhb.quarkkingdee.top

[U105] JS：节流
来源：http://lqg.mhx1999.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ssl.tanke756.top

[U106] JS：日期格式化
来源：http://utd.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zub.zdbjq.cn

[U107] JS：数字千分位
来源：http://cmk.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vuw.ybcxt.top

[U108] JS：随机整数
来源：http://vxi.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ypb.fktsv.cn

[U109] JS：数组分组
来源：http://ohj.fanxiaobao.xyz

Object.groupBy(arr, x => x.type)
来源：http://yiz.jyoumei.cn

[U110] JS：数组分块
来源：http://qdx.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tww.0kj1m.cn

[U111] JS：对象转 Map
来源：http://jje.jqgfzy.top

new Map(Object.entries(obj))
来源：http://fgm.hnqzz.top

[U112] JS：字符串补位
来源：http://hve.yueranfly.top

"7".padStart(3, "0")
来源：http://sjn.tianlin.xyz

[U113] JS：正则替换全部
来源：http://hun.ydzc1.top

s.replaceAll("a", "b")
来源：http://qvz.havefunace.top

[U114] JS：JSON 深比较
来源：http://elu.zhoulong.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://pba.dashuyun.cn

[U115] JS：生成 UUID
来源：http://iqn.yuxming.cn

crypto.randomUUID()
来源：http://slp.zhengqikj.top

[U116] JS：类型检查（JSDoc）
来源：http://mzo.shanyushiyangtech.top

/** @param {string} name */ function f(name) {}
来源：http://tjc.zdbjq.cn

[U117] JS：单元测试
来源：http://pme.zdbjq.cn

npm i -D vitest;  npx vitest
来源：http://wla.316326.xyz

[U118] JS：开发服务器
来源：http://zka.fehbvm.com

npm i -D vite;  npx vite
来源：http://ove.hnxiangtu.top

[U119] JS：生产构建
来源：http://iwy.sxryk.cn

npx vite build
来源：http://mgj.ppjwa.cn

[U120] JS：读取环境变量（Vite）
来源：http://wvy.pycfn.com

import.meta.env.VITE_API_URL
来源：http://faf.ivvv.top

================================================================================
来源：http://jmf.xingfuxueyuan.xyz

统计汇总
来源：http://owk.zhongyouzk.top

================================================================================
来源：http://gre.ydzc1.top

按语言统计（条）：
来源：http://xux.quarkkingdee.top

Python ......... 252
来源：http://ghe.hfpthk.cn

PHP ............ 252
来源：http://ylj.yuxming.cn

JavaScript ..... 252
来源：http://ekd.ywan-chungtsiang.top

TypeScript ..... 212
来源：http://dey.chenlongwang.top

Java ........... 212
来源：http://whg.ydzc1.top

Go ............. 212
来源：http://zdg.haohaochexian.top

Ruby ........... 212
来源：http://rpw.jyoumei.cn

C# ............. 212
来源：http://urr.0kj1m.cn

C .............. 30
来源：http://sah.smart0.xyz

C++ ............ 30
来源：http://pum.cashguo.top

SQL ............ 90
来源：http://ljh.jinghuilouyu.cn

Bash ........... 80
来源：http://lay.shanyushiyangkeji.top

Kotlin ......... 15
来源：http://soj.tanke756.top

Swift .......... 15
来源：http://krh.xylfe.cn

Lua ............ 10
来源：http://zjr.shanyushiyangtech.top

Perl ........... 10
来源：http://xzw.zhixingplan.top

Scala .......... 10
来源：http://dgj.fktsv.cn

------------------------------------
来源：http://fah.havefunace.top

合计 ........... 2106 条
来源：http://wex.yuanzhike.top

按章节统计：
来源：http://ygp.c1oappe.top


<!-- 参考信息 -->