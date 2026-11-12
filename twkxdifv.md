代发 wailian999

[T45] Perl：数组遍历
来源：http://aqz.ivvv.top

for my $x (@arr) { print $x; }
来源：http://iql.zhengqikj.top

[T46] Perl：哈希操作
来源：http://skg.jinghuilouyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aic.shanyushiyangtech.top

[T47] Perl：正则捕获
来源：http://mxp.mhx1999.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gmu.sufxvd.cn

[T48] Perl：正则替换
来源：http://cke.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://pcq.xziqi.cn

[T49] Perl：函数
来源：http://gbs.hammf.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qfe.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://pte.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://thz.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://fsw.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://zqt.hnqzz.top

println("Hello")
来源：http://hta.ywan-chungtsiang.top

[T52] Scala：变量
来源：http://vfe.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://gmo.ydjk.org.cn

[T53] Scala：字符串插值
来源：http://mgv.hcnkem.com

s"值: $b"
来源：http://hvl.tanke756.top

[T54] Scala：集合映射
来源：http://hcd.gogol.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://bgo.mhx1999.top

[T55] Scala：集合过滤
来源：http://kos.hnxiangtu.top

List(1, 2, 3).filter(_ > 1)
来源：http://lar.jiagoushi.top

[T56] Scala：样例类
来源：http://psb.havefunace.top

case class User(name: String, age: Int)
来源：http://cbx.haohaochexian.top

[T57] Scala：模式匹配
来源：http://uch.snrcjt.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zet.sufxvd.cn

[T58] Scala：函数定义
来源：http://tqb.jiagoushi.top

def add(a: Int, b: Int): Int = a + b
来源：http://boq.nanxuanxn.top

[T59] Scala：循环
来源：http://wlt.cheryme.top

for (i <- 1 to 10) println(i)
来源：http://gsd.tarul.cn

[T60] Scala：折叠
来源：http://hbz.xuanzx.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vwi.wangshuangyany.cn

================================================================================
来源：http://vpx.zdqjudy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vds.sweek.top

================================================================================
来源：http://xst.aizwys.cn

[U01] Py：创建虚拟环境
来源：http://qro.ydzc1.top

python -m venv .venv && source .venv/bin/activate
来源：http://sao.sufxvd.cn

[U02] Py：导出 / 安装依赖
来源：http://bzs.aizwys.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kcq.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://cbf.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zzm.xinyue.icu

[U04] Py：变量调试打印
来源：http://lux.ctjpmb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://olc.gogol.net.cn

[U05] Py：列表去重且保序
来源：http://oxm.gzhubu.top

list(dict.fromkeys(arr))
来源：http://uuf.zhiwuduotai.top

[U06] Py：合并两个字典
来源：http://bik.pycfn.com

{**a, **b}
来源：http://cda.tian-w.cn

[U07] Py：反转字典键值
来源：http://zap.yanxiufei.cn

{v: k for k, v in d.items()}
来源：http://cqy.zhongyouzk.top

[U08] Py：展平二维列表
来源：http://uag.wangshuangyany.cn

[y for x in nested for y in x]
来源：http://rkh.birdmap.top

[U09] Py：字典取最大值的键
来源：http://zcb.shanyushiyangkeji.top

max(d, key=d.get)
来源：http://bmz.pengpengdd.cyou

[U10] Py：按值排序字典
来源：http://obt.zhaomingkeji.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qmt.jyoumei.cn

[U11] Py：生成器表达式
来源：http://jvm.jiagoushi.top

(x * 2 for x in arr)
来源：http://zoz.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://ksq.nanxinkj.top

Counter(arr).most_common(3)
来源：http://mms.tanke756.top

[U13] Py：固定长度队列
来源：http://bik.hammf.cn

deque(maxlen=10)
来源：http://wih.andypj.xyz

[U14] Py：分组收集到列表
来源：http://jgk.chenzaomai.com

defaultdict(list)
来源：http://omi.yongpay.top

[U15] Py：高精度计时
来源：http://swv.ywan-chungtsiang.top

t = time.perf_counter()
来源：http://jwc.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://slz.ybcxt.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qhg.jinqigfzy.top

[U17] Py：初始化日志
来源：http://opm.jinghuilouyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://qji.epnwcf.com

[U18] Py：预编译正则
来源：http://bmk.bbcook.cn

pat = re.compile(r"\d+")
来源：http://ftu.shuidangran.top

[U19] Py：正则替换带回调
来源：http://kny.yangfankeji.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wav.kuanghao11.cn

[U20] Py：缓存函数结果
来源：http://nex.chenjidiqi.icu

@functools.lru_cache(maxsize=None)
来源：http://fmi.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://ujm.yj20258.top

@contextlib.contextmanager
来源：http://pzn.vehdjk.com

[U22] Py：矩阵转置
来源：http://pun.zhaomingkeji.xyz

list(zip(*m))
来源：http://eiq.ehwqpu.com

[U23] Py：分块读取大文件
来源：http://xrt.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zkb.yj20258.top

[U24] Py：路径操作
来源：http://vtz.daria6918.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bgp.yj20258.top

[U25] Py：CSV 按字典读
来源：http://qrd.wangdashe.top

csv.DictReader(f)
来源：http://rlb.yj20258888.top

[U26] Py：并发下载
来源：http://afd.hongshengwenyu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cbb.c1oappe.top

[U27] Py：异步 HTTP
来源：http://xem.smart0.xyz

aiohttp.ClientSession() 配合 async with
来源：http://ozb.bjfxy.top

[U28] Py：类型别名
来源：http://ywj.dianchejie.cn

UserId = int
来源：http://xwf.daria6918.cn

[U29] Py：属性校验
来源：http://yec.jinqigufen.top

@property 与 @x.setter 配合
来源：http://ihv.yfazqb.com

[U30] Py：数据类
来源：http://cmw.zhoulong.xyz

@dataclass(slots=True)
来源：http://dwh.jlsjyb.cn

[U31] Py：单测
来源：http://tsv.haohaochexian.top

python -m pytest -q
来源：http://all.pengpengdd.cyou

[U32] Py：代码格式化
来源：http://oqe.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://cfu.fengsongda.top

[U33] Py：打包发布
来源：http://fky.hesvh.cn

python -m build  （依赖 pyproject.toml）
来源：http://uhd.9152youxi.cn

[U34] Py：判断编码
来源：http://nao.chenlongwang.top

chardet.detect(raw)
来源：http://yvj.316326.xyz

[U35] Py：发送邮件
来源：http://ddx.pengpengdd.cyou

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tdm.jinqigfzy.top

[U36] Py：定时任务
来源：http://dyy.pycfn.com

schedule.every(10).minutes.do(job)
来源：http://cau.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://yuj.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://fbo.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://hdh.nanxuanxn.top

Path(__file__).resolve().parent
来源：http://aia.fehbvm.com

[U39] Py：判断是否在交互环境
来源：http://kjv.chenlongwang.top

sys.stdout.isatty()
来源：http://tnr.hfpthk.cn

[U40] Py：打印到标准错误
来源：http://nlu.zdqjudy.top

print("err", file=sys.stderr)
来源：http://ufa.yanxiufei.cn

[U41] PHP：初始化 Composer 项目
来源：http://rld.fktsv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qwt.yfazqb.com

[U42] PHP：PSR-4 自动加载
来源：http://ujz.sysykeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aul.cdnleiting.top

[U43] PHP：声明命名空间
来源：http://qni.hywenlv.cn

namespace App\Http;
来源：http://xxs.zhixingplan.top

[U44] PHP：开启严格类型
来源：http://ejy.mhx1999.top

declare(strict_types=1);
来源：http://ekt.pycfn.com

[U45] PHP：类型声明与返回类型
来源：http://uqg.c1oappe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jze.jianghu66.top

[U46] PHP：可空类型
来源：http://dyf.uphjek.com

?string $name = null
来源：http://uwo.daxiang520.top

[U47] PHP：联合类型
来源：http://jah.hongshengwenyu.top

int|string $id
来源：http://sbd.jqgufenzy.top

[U48] PHP：纯枚举
来源：http://lma.andypj.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cxa.c1oappe.top

[U49] PHP：只读属性
来源：http://lgo.ppjwa.cn

public readonly string $name
来源：http://ygk.hnqzz.top

[U50] PHP：构造器属性提升
来源：http://ael.xinyue.icu

public function __construct(private int $id) {}
来源：http://plx.gaohongyu789.top

[U51] PHP：数组解构
来源：http://exq.ppjwa.cn

[$a, $b] = $arr;
来源：http://dhi.jinqigufen.top

[U52] PHP：箭头函数
来源：http://gra.ydjk.org.cn

$double = fn($x) => $x * 2;
来源：http://ood.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://jnv.zycfv.cn

$v = $a ?? $b ?? "default";
来源：http://wds.gogol.net.cn

[U54] PHP：空安全调用
来源：http://lam.tarul.cn

$obj?->method()
来源：http://hfa.9152youxi.cn

[U55] PHP：match 表达式
来源：http://tme.gzhubu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://prp.hfpthk.cn

[U56] PHP：命名参数
来源：http://jec.fktsv.cn

f(a: 1, b: 2)
来源：http://ewq.hongshengwenyu.top

[U57] PHP：字符串插值
来源：http://jmu.hysaishi.cn

"值: {$a}"
来源：http://bql.cucudq.cn

[U58] PHP：数组三件套
来源：http://qwy.zhijiandao.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jda.bjfxy.top

[U59] PHP：自定义排序
来源：http://fou.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gwl.c1oappe.top

[U60] PHP：JSON 编解码
来源：http://sif.9152youxi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dok.smart0.xyz

[U61] PHP：正则
来源：http://zfu.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jgk.smart0.xyz

[U62] PHP：日期对象
来源：http://adg.tianlin.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zoc.yuanzhike.top

[U63] PHP：文件读写
来源：http://ley.fanxiaobao.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hal.pengpengdd.cyou

[U64] PHP：目录遍历
来源：http://zou.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://zqb.haohaochexian.top

[U65] PHP：会话
来源：http://hmo.ppjwa.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pwp.chenzaomai.com

[U66] PHP：设置 Cookie
来源：http://lwh.yuanzhike.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cly.haohaochexian.top

[U67] PHP：处理文件上传
来源：http://blb.chenjidiqi.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nbx.meibo888.top

[U68] PHP：PDO 连接
来源：http://req.tanke756.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wep.hnqzz.top

[U69] PHP：PDO 预处理
来源：http://tlr.dianchejie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xhy.vqdsnc.cn

[U70] PHP：PDO 事务
来源：http://rgw.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://slk.zhiwuduotai.top

[U71] PHP：抛出异常
来源：http://tcn.xziqi.cn

throw new RuntimeException("失败", 500);
来源：http://bxa.cheryme.top

[U72] PHP：写错误日志
来源：http://msg.zdbjq.cn

error_log("失败: " . $e->getMessage());
来源：http://nko.haohaochexian.top

[U73] PHP：读取 ini 配置
来源：http://zfd.iojbl.cn

parse_ini_file("config.ini", true)
来源：http://snj.shanyushiyangkeji.top

[U74] PHP：读取环境变量
来源：http://aya.hfpthk.cn

getenv("APP_ENV") ?: "production"
来源：http://zno.yvedp.cn

[U75] PHP：依赖注入
来源：http://voe.fengsongda.top

composer require psr/container
来源：http://yfx.gotoacloud.top

[U76] PHP：简单路由
来源：http://ipz.jlsjyb.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ugo.gogol.net.cn

[U77] PHP：模板渲染
来源：http://yid.zhengqikj.top

composer require twig/twig
来源：http://sad.chenjidiqi.icu

[U78] PHP：单元测试
来源：http://sej.xingfuxueyuan.xyz

composer require --dev phpunit/phpunit
来源：http://qlk.xylfe.cn

[U79] PHP：静态分析
来源：http://aox.tanke756.top

composer require --dev phpstan/phpstan
来源：http://wbq.sjlbkw.cn

[U80] PHP：代码规范修复
来源：http://orh.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://fca.cdnleiting.top

[U81] JS：初始化项目
来源：http://wln.jqgufenzy.top

npm init -y;  npm i express
来源：http://jzt.kuanghao11.cn

[U82] JS：package.json 脚本
来源：http://otp.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cav.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://qqx.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cvv.zhongyouzk.top

[U84] JS：CommonJS 写法
来源：http://vvy.ehwqpu.com

module.exports = { a };  const { a } = require("./m");
来源：http://dho.yj20258888.top

[U85] JS：可选链
来源：http://ifd.vqdsnc.cn

a?.b?.c
来源：http://dsg.jinqigufen.top

[U86] JS：空值合并
来源：http://wzf.tianlin.xyz

a ?? b
来源：http://lmn.cdnleiting.top

[U87] JS：解构默认值
来源：http://wom.sjlbkw.cn

const { a = 1, b = 2 } = obj;
来源：http://edk.shuidangran.top

[U88] JS：对象展开合并
来源：http://gzi.zhixingplan.top

{ ...a, ...b }
来源：http://rci.tianlin.xyz

[U89] JS：数组去重
来源：http://ida.yj20258.top

[...new Set(arr)]
来源：http://uyl.tianlin.xyz

[U90] JS：数字数组排序
来源：http://dsc.xinyue.icu

[...arr].sort((a, b) => a - b)
来源：http://gwu.cucudq.cn

[U91] JS：对象键值遍历
来源：http://wwl.fengsongda.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lqw.jinqigfzy.top

[U92] JS：深拷贝
来源：http://lrn.yangfankeji.com

structuredClone(obj)
来源：http://flp.wangshuangyany.cn

[U93] JS：模板字符串
来源：http://yxu.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://wsp.nwbrower.top

[U94] JS：箭头函数
来源：http://lem.kuanghao11.cn

const double = x => x * 2;
来源：http://nso.dianchejie.cn

[U95] JS：Promise 包装
来源：http://tpf.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://uhs.bbcook.cn

[U96] JS：async/await 与异常
来源：http://kkh.xziqi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tnd.sxryk.cn

[U97] JS：并发请求
来源：http://wki.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gig.epnwcf.com

[U98] JS：fetch 带 JSON
来源：http://wvr.uphjek.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ayu.smart0.xyz

[U99] JS：事件监听
来源：http://tox.chenzaomai.com

el.addEventListener("click", e => {})
来源：http://rdv.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://igj.zhijiandao.cn

document.querySelector(".item")
来源：http://uty.dashuyun.cn

[U101] JS：classList 操作
来源：http://dzq.nwbrower.top

el.classList.toggle("active")
来源：http://pki.yanxiufei.cn

[U102] JS：本地存储
来源：http://mmu.fanxiaobao.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://mlg.nanxuanxn.top

[U103] JS：定时器
来源：http://sqz.epnwcf.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fhr.yanxiufei.cn

[U104] JS：防抖
来源：http://hcm.chenlongwang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lig.tarul.cn

[U105] JS：节流
来源：http://geo.quarkkingdee.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zar.9152youxi.cn

[U106] JS：日期格式化
来源：http://yqp.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hls.fehbvm.com

[U107] JS：数字千分位
来源：http://mvf.sysykeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ipj.yuanzhike.top

[U108] JS：随机整数
来源：http://zam.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ruv.52xcode.cn

[U109] JS：数组分组
来源：http://yxx.xingfuxueyuan.xyz

Object.groupBy(arr, x => x.type)
来源：http://zgk.shangyingyoupin.top

[U110] JS：数组分块
来源：http://cnk.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vba.xylfe.cn

[U111] JS：对象转 Map
来源：http://hvq.sufxvd.cn

new Map(Object.entries(obj))
来源：http://wli.zycfv.cn

[U112] JS：字符串补位
来源：http://hau.tian-w.cn

"7".padStart(3, "0")
来源：http://nrw.tian-w.cn

[U113] JS：正则替换全部
来源：http://haq.yueranfly.top

s.replaceAll("a", "b")
来源：http://hjs.dashuyun.cn

[U114] JS：JSON 深比较
来源：http://peo.ydjk.org.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mdi.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://esh.aizwys.cn

crypto.randomUUID()
来源：http://nyz.yanxiufei.cn

[U116] JS：类型检查（JSDoc）
来源：http://ukc.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://frq.nanxuanxn.top

[U117] JS：单元测试
来源：http://tas.xuanzx.com

npm i -D vitest;  npx vitest
来源：http://nhv.sweek.top

[U118] JS：开发服务器
来源：http://vzb.haohaochexian.top

npm i -D vite;  npx vite
来源：http://tdh.fktsv.cn

[U119] JS：生产构建
来源：http://gvk.ydzc1.top

npx vite build
来源：http://kep.hammf.cn

[U120] JS：读取环境变量（Vite）
来源：http://zti.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://anq.sxryk.cn

================================================================================
来源：http://qaf.mhx1999.top

统计汇总
来源：http://drr.hesvh.cn

================================================================================
来源：http://ryf.hfpthk.cn

按语言统计（条）：
来源：http://roz.jinyuanbaomall.cn

Python ......... 252
来源：http://niw.gzhubu.top

PHP ............ 252
来源：http://fre.gotoacloud.top

JavaScript ..... 252
来源：http://ucl.sjlbkw.cn

TypeScript ..... 212
来源：http://otp.9152youxi.cn

Java ........... 212
来源：http://yrm.sweek.top

Go ............. 212
来源：http://iyw.redwolf501.top

Ruby ........... 212
来源：http://xre.yfazqb.com

C# ............. 212
来源：http://cpm.jinghuilouyu.cn

C .............. 30
来源：http://ocq.snrcjt.cn

C++ ............ 30
来源：http://hmp.jlsjyb.cn

SQL ............ 90
来源：http://nae.yj20258.top

Bash ........... 80
来源：http://ysu.sysykeji.top

Kotlin ......... 15
来源：http://acf.daria6918.cn

Swift .......... 15
来源：http://yjf.jianghu66.top

Lua ............ 10
来源：http://ovm.sweek.top

Perl ........... 10
来源：http://khm.zhoulong.xyz

Scala .......... 10
来源：http://gbk.shanyushiyangtech.top

------------------------------------
来源：http://baf.fanxiaobao.xyz

合计 ........... 2106 条
来源：http://xro.cucudq.cn

按章节统计：
来源：http://iiv.jqgfzy.top


<!-- 参考信息 -->