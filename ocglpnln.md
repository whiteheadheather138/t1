代发 wailian999

[T45] Perl：数组遍历
来源：http://agw.wangdashe.top

for my $x (@arr) { print $x; }
来源：http://jwp.hcnkem.com

[T46] Perl：哈希操作
来源：http://hxm.hywenlv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uza.hfpthk.cn

[T47] Perl：正则捕获
来源：http://ttz.zdqjudy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fll.guowangkeji.top

[T48] Perl：正则替换
来源：http://duh.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://odn.kuanghao11.cn

[T49] Perl：函数
来源：http://mrm.pengpengdd.cyou

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hwl.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://mli.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://gzk.dashuyun.cn

while (my $line = <$fh>) { print $line; }
来源：http://ape.andypj.xyz

[T51] Scala：Hello World
来源：http://vcg.shanyushiyangkeji.top

println("Hello")
来源：http://wmy.mhx1999.top

[T52] Scala：变量
来源：http://fwh.sxryk.cn

val a = 1;  var b = 2
来源：http://rxv.cucudq.cn

[T53] Scala：字符串插值
来源：http://ddp.smart0.xyz

s"值: $b"
来源：http://jqa.0kj1m.cn

[T54] Scala：集合映射
来源：http://aly.zhijiandao.cn

List(1, 2, 3).map(_ * 2)
来源：http://eqt.jlsjyb.cn

[T55] Scala：集合过滤
来源：http://huz.vehdjk.com

List(1, 2, 3).filter(_ > 1)
来源：http://gbb.zdqjudy.top

[T56] Scala：样例类
来源：http://soa.aibaodan.cn

case class User(name: String, age: Int)
来源：http://vpn.yanxiufei.cn

[T57] Scala：模式匹配
来源：http://gfm.sjlbkw.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bmn.zhijiandao.cn

[T58] Scala：函数定义
来源：http://vfn.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://ico.tanke756.top

[T59] Scala：循环
来源：http://frb.guannengcc.top

for (i <- 1 to 10) println(i)
来源：http://lpr.fktsv.cn

[T60] Scala：折叠
来源：http://yeu.daxiang520.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nwf.316326.xyz

================================================================================
来源：http://ygq.hysaishi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rws.havefunace.top

================================================================================
来源：http://oex.guowangkeji.top

[U01] Py：创建虚拟环境
来源：http://zih.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uep.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://qes.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dyr.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://wvl.jinqigfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cxs.quarkkingdee.top

[U04] Py：变量调试打印
来源：http://hhi.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ziw.aizwys.cn

[U05] Py：列表去重且保序
来源：http://xit.yfazqb.com

list(dict.fromkeys(arr))
来源：http://hbi.jqgfzy.top

[U06] Py：合并两个字典
来源：http://ldi.yfazqb.com

{**a, **b}
来源：http://xfh.ydzc1.top

[U07] Py：反转字典键值
来源：http://igo.svipenyu.cn

{v: k for k, v in d.items()}
来源：http://cll.cdnleiting.top

[U08] Py：展平二维列表
来源：http://zou.zhixingplan.top

[y for x in nested for y in x]
来源：http://gmy.hesvh.cn

[U09] Py：字典取最大值的键
来源：http://lrv.birdmap.top

max(d, key=d.get)
来源：http://xzl.hysaishi.cn

[U10] Py：按值排序字典
来源：http://oai.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sap.pycfn.com

[U11] Py：生成器表达式
来源：http://pho.nanxuanxn.top

(x * 2 for x in arr)
来源：http://nuk.zdbjq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://swm.yuanzhike.top

Counter(arr).most_common(3)
来源：http://zfm.shuidangran.top

[U13] Py：固定长度队列
来源：http://udy.sysykeji.top

deque(maxlen=10)
来源：http://isa.fehbvm.com

[U14] Py：分组收集到列表
来源：http://mza.dianchejie.cn

defaultdict(list)
来源：http://ath.jinqigufen.top

[U15] Py：高精度计时
来源：http://isq.wangdashe.top

t = time.perf_counter()
来源：http://lup.yuanzhike.top

[U16] Py：命令行参数解析
来源：http://ogg.bjfxy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://enm.cashguo.top

[U17] Py：初始化日志
来源：http://jlh.tianlin.xyz

logging.basicConfig(level=logging.INFO)
来源：http://gux.mhx1999.top

[U18] Py：预编译正则
来源：http://dyx.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://rep.fktsv.cn

[U19] Py：正则替换带回调
来源：http://crv.sxryk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nwm.bbcook.cn

[U20] Py：缓存函数结果
来源：http://ngy.smart0.xyz

@functools.lru_cache(maxsize=None)
来源：http://vqd.guowangkeji.top

[U21] Py：自定义上下文管理器
来源：http://qvu.xuanzx.com

@contextlib.contextmanager
来源：http://qfe.jinghuilouyu.cn

[U22] Py：矩阵转置
来源：http://mgy.xuanzx.com

list(zip(*m))
来源：http://apf.yj20258888.top

[U23] Py：分块读取大文件
来源：http://emc.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://did.cdnleiting.top

[U24] Py：路径操作
来源：http://kep.sysykeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://riw.smart0.xyz

[U25] Py：CSV 按字典读
来源：http://ebd.52xcode.cn

csv.DictReader(f)
来源：http://wks.ydjk.org.cn

[U26] Py：并发下载
来源：http://dtd.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nin.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://tak.redwolf501.top

aiohttp.ClientSession() 配合 async with
来源：http://xlo.jinqigufen.top

[U28] Py：类型别名
来源：http://aur.tianlin.xyz

UserId = int
来源：http://zeo.dianchejie.cn

[U29] Py：属性校验
来源：http://hfb.ehwqpu.com

@property 与 @x.setter 配合
来源：http://nhj.hongshengwenyu.top

[U30] Py：数据类
来源：http://gmi.316326.xyz

@dataclass(slots=True)
来源：http://eyi.shanyushiyangkeji.top

[U31] Py：单测
来源：http://ajn.feifeiyinyue.top

python -m pytest -q
来源：http://nhb.ydzc1.top

[U32] Py：代码格式化
来源：http://ugt.hfpthk.cn

ruff format . && ruff check --fix .
来源：http://rsa.redwolf501.top

[U33] Py：打包发布
来源：http://upl.gogol.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://ggt.mhx1999.top

[U34] Py：判断编码
来源：http://fix.fktsv.cn

chardet.detect(raw)
来源：http://kia.andypj.xyz

[U35] Py：发送邮件
来源：http://wme.xingfuxueyuan.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cap.yj20258.top

[U36] Py：定时任务
来源：http://ckn.yj202588.top

schedule.every(10).minutes.do(job)
来源：http://dfs.jqgufenzy.top

[U37] Py：读写 Excel
来源：http://rrw.hesvh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nsx.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://ttv.yuxming.cn

Path(__file__).resolve().parent
来源：http://xpq.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://wgd.jinyuanbaomall.cn

sys.stdout.isatty()
来源：http://ivk.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://bst.hnqzz.top

print("err", file=sys.stderr)
来源：http://uii.snrcjt.cn

[U41] PHP：初始化 Composer 项目
来源：http://aas.cqqwz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nfc.9152youxi.cn

[U42] PHP：PSR-4 自动加载
来源：http://vka.yangfankeji.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://soa.nanxinkj.top

[U43] PHP：声明命名空间
来源：http://bmn.yanxiufei.cn

namespace App\Http;
来源：http://ydk.52xcode.cn

[U44] PHP：开启严格类型
来源：http://wci.gaohongyu789.top

declare(strict_types=1);
来源：http://ekl.xuanzx.com

[U45] PHP：类型声明与返回类型
来源：http://svt.ybcxt.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ptw.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://kox.sxryk.cn

?string $name = null
来源：http://imv.zdqjudy.top

[U47] PHP：联合类型
来源：http://izf.shanyushiyangtech.top

int|string $id
来源：http://ndw.jinyuanbaomall.cn

[U48] PHP：纯枚举
来源：http://mjv.jianghu66.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://szp.shzxlz.cn

[U49] PHP：只读属性
来源：http://ace.kuanghao11.cn

public readonly string $name
来源：http://xmq.ybcxt.top

[U50] PHP：构造器属性提升
来源：http://ryt.sysykeji.top

public function __construct(private int $id) {}
来源：http://xji.mhx1999.top

[U51] PHP：数组解构
来源：http://yua.jinyuanbaomall.cn

[$a, $b] = $arr;
来源：http://agg.jqgfzy.top

[U52] PHP：箭头函数
来源：http://gcr.zdqjudy.top

$double = fn($x) => $x * 2;
来源：http://udo.cashguo.top

[U53] PHP：空合并运算符
来源：http://msn.tanke756.top

$v = $a ?? $b ?? "default";
来源：http://xry.guowangkeji.top

[U54] PHP：空安全调用
来源：http://hvb.jinghuilouyu.cn

$obj?->method()
来源：http://aiy.zhaomingkeji.xyz

[U55] PHP：match 表达式
来源：http://ipb.ppjwa.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uaz.gogol.net.cn

[U56] PHP：命名参数
来源：http://njz.feifeiyinyue.top

f(a: 1, b: 2)
来源：http://ztp.sweek.top

[U57] PHP：字符串插值
来源：http://cdb.zycfv.cn

"值: {$a}"
来源：http://lfe.jqgufenzy.top

[U58] PHP：数组三件套
来源：http://vlx.sxryk.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ubn.shanyushiyangkeji.top

[U59] PHP：自定义排序
来源：http://odv.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iwo.shuidangran.top

[U60] PHP：JSON 编解码
来源：http://egi.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tfo.cashguo.top

[U61] PHP：正则
来源：http://gmt.guannengcc.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bkt.yonumen.top

[U62] PHP：日期对象
来源：http://bwe.zhongyouzk.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jjr.epnwcf.com

[U63] PHP：文件读写
来源：http://bfk.gzhubu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gzm.meibo888.top

[U64] PHP：目录遍历
来源：http://tcm.9152youxi.cn

glob("dir/*.php");  scandir("dir");
来源：http://bvl.ctjpmb.com

[U65] PHP：会话
来源：http://vvi.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hlm.chenzaomai.com

[U66] PHP：设置 Cookie
来源：http://zrr.ywan-chungtsiang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jdn.svipenyu.cn

[U67] PHP：处理文件上传
来源：http://lue.cucudq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ntj.dashuyun.cn

[U68] PHP：PDO 连接
来源：http://fpt.chenzaomai.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pue.xingfuxueyuan.xyz

[U69] PHP：PDO 预处理
来源：http://pgf.guannengcc.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iqw.fengsongda.top

[U70] PHP：PDO 事务
来源：http://rrj.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ixv.dianchejie.cn

[U71] PHP：抛出异常
来源：http://klz.ehwqpu.com

throw new RuntimeException("失败", 500);
来源：http://hlo.hongshengwenyu.top

[U72] PHP：写错误日志
来源：http://bti.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://yam.svipenyu.cn

[U73] PHP：读取 ini 配置
来源：http://oxb.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://mza.ppjwa.cn

[U74] PHP：读取环境变量
来源：http://ygg.hongshengwenyu.top

getenv("APP_ENV") ?: "production"
来源：http://npg.zdbjq.cn

[U75] PHP：依赖注入
来源：http://izh.hesvh.cn

composer require psr/container
来源：http://iuq.shanyushiyangtech.top

[U76] PHP：简单路由
来源：http://tbr.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://deh.jqgufenzy.top

[U77] PHP：模板渲染
来源：http://mnq.ywan-chungtsiang.top

composer require twig/twig
来源：http://ymw.kuanghao11.cn

[U78] PHP：单元测试
来源：http://nkh.gzhubu.top

composer require --dev phpunit/phpunit
来源：http://tux.xuetiantiany.cn

[U79] PHP：静态分析
来源：http://bcu.iojbl.cn

composer require --dev phpstan/phpstan
来源：http://iwg.redwolf501.top

[U80] PHP：代码规范修复
来源：http://nya.yj20258.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jwa.fengsongda.top

[U81] JS：初始化项目
来源：http://lku.haohaochexian.top

npm init -y;  npm i express
来源：http://djk.ppjwa.cn

[U82] JS：package.json 脚本
来源：http://zty.zhengqikj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kmj.zdqjudy.top

[U83] JS：ES Module 导入导出
来源：http://gky.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://plp.jinghuilouyu.cn

[U84] JS：CommonJS 写法
来源：http://vdf.zycfv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://svc.gzhubu.top

[U85] JS：可选链
来源：http://nnx.nanxuanxn.top

a?.b?.c
来源：http://stx.chenzaomai.com

[U86] JS：空值合并
来源：http://yqh.ybcxt.top

a ?? b
来源：http://xyn.cashguo.top

[U87] JS：解构默认值
来源：http://xpu.zhijiandao.cn

const { a = 1, b = 2 } = obj;
来源：http://ztb.zhoulong.xyz

[U88] JS：对象展开合并
来源：http://qcw.chenjidiqi.icu

{ ...a, ...b }
来源：http://oml.tianlin.xyz

[U89] JS：数组去重
来源：http://lay.fktsv.cn

[...new Set(arr)]
来源：http://tmt.shanyushiyangtech.top

[U90] JS：数字数组排序
来源：http://win.0kj1m.cn

[...arr].sort((a, b) => a - b)
来源：http://nwp.andypj.xyz

[U91] JS：对象键值遍历
来源：http://yoz.yangfankeji.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://icv.52xcode.cn

[U92] JS：深拷贝
来源：http://lik.yj202588.top

structuredClone(obj)
来源：http://vyy.epnwcf.com

[U93] JS：模板字符串
来源：http://zsc.gogol.net.cn

`共 ${n} 条`
来源：http://wtf.sufxvd.cn

[U94] JS：箭头函数
来源：http://efg.zhiwuduotai.top

const double = x => x * 2;
来源：http://ssh.hfpthk.cn

[U95] JS：Promise 包装
来源：http://qqv.tanke756.top

new Promise((resolve, reject) => {})
来源：http://mgz.daxiang520.top

[U96] JS：async/await 与异常
来源：http://bes.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aal.hammf.cn

[U97] JS：并发请求
来源：http://uby.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kte.zdbjq.cn

[U98] JS：fetch 带 JSON
来源：http://don.jinyuanbaomall.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wvg.0kj1m.cn

[U99] JS：事件监听
来源：http://exd.316326.xyz

el.addEventListener("click", e => {})
来源：http://yho.fehbvm.com

[U100] JS：DOM 查询
来源：http://dic.xuanzx.com

document.querySelector(".item")
来源：http://kbz.fanxiaobao.xyz

[U101] JS：classList 操作
来源：http://hrn.xuetiantiany.cn

el.classList.toggle("active")
来源：http://acf.shuidangran.top

[U102] JS：本地存储
来源：http://xeg.jinqigfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uqx.nwbrower.top

[U103] JS：定时器
来源：http://swc.ppjwa.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ngg.yanxiufei.cn

[U104] JS：防抖
来源：http://krd.yj20258.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zhj.nwbrower.top

[U105] JS：节流
来源：http://vsy.jinqigufen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mdu.zycfv.cn

[U106] JS：日期格式化
来源：http://iuj.ywan-chungtsiang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fam.zhixingplan.top

[U107] JS：数字千分位
来源：http://tko.aibaodan.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://usq.hywenlv.cn

[U108] JS：随机整数
来源：http://wrt.xinyue.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yus.ppjwa.cn

[U109] JS：数组分组
来源：http://rky.guannengcc.top

Object.groupBy(arr, x => x.type)
来源：http://dik.yj202588.top

[U110] JS：数组分块
来源：http://jlk.xuetiantiany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qto.redwolf501.top

[U111] JS：对象转 Map
来源：http://hqh.tanke756.top

new Map(Object.entries(obj))
来源：http://ahu.tian-w.cn

[U112] JS：字符串补位
来源：http://cir.cheryme.top

"7".padStart(3, "0")
来源：http://emw.jiagoushi.top

[U113] JS：正则替换全部
来源：http://zha.gotoacloud.top

s.replaceAll("a", "b")
来源：http://rcj.zycfv.cn

[U114] JS：JSON 深比较
来源：http://wgw.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hwf.sxryk.cn

[U115] JS：生成 UUID
来源：http://fxt.wangdashe.top

crypto.randomUUID()
来源：http://los.zycfv.cn

[U116] JS：类型检查（JSDoc）
来源：http://fta.shanyushiyangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://hlh.sysykeji.top

[U117] JS：单元测试
来源：http://mxr.fanxiaobao.xyz

npm i -D vitest;  npx vitest
来源：http://ygv.quarkkingdee.top

[U118] JS：开发服务器
来源：http://ycx.sweek.top

npm i -D vite;  npx vite
来源：http://mka.fzhhl.top

[U119] JS：生产构建
来源：http://huk.yuxming.cn

npx vite build
来源：http://eif.tian-w.cn

[U120] JS：读取环境变量（Vite）
来源：http://ddd.zhaomingkeji.xyz

import.meta.env.VITE_API_URL
来源：http://har.meibo888.top

================================================================================
来源：http://hvr.316326.xyz

统计汇总
来源：http://iag.zhengqikj.top

================================================================================
来源：http://aat.yfazqb.com

按语言统计（条）：
来源：http://sts.feifeiyinyue.top

Python ......... 252
来源：http://wii.gzhubu.top

PHP ............ 252
来源：http://ynw.xziqi.cn

JavaScript ..... 252
来源：http://dad.yongpay.top

TypeScript ..... 212
来源：http://pys.yuanzhike.top

Java ........... 212
来源：http://lyn.pengpengdd.cyou

Go ............. 212
来源：http://mjh.birdmap.top

Ruby ........... 212
来源：http://zfu.mhx1999.top

C# ............. 212
来源：http://pju.hysaishi.cn

C .............. 30
来源：http://hty.guowangkeji.top

C++ ............ 30
来源：http://akk.hysaishi.cn

SQL ............ 90
来源：http://ben.yonumen.top

Bash ........... 80
来源：http://oya.yueranfly.top

Kotlin ......... 15
来源：http://zig.ydzc1.top

Swift .......... 15
来源：http://uxj.snrcjt.cn

Lua ............ 10
来源：http://mlj.zhoulong.xyz

Perl ........... 10
来源：http://kfr.sweek.top

Scala .......... 10
来源：http://wzy.fengsongda.top

------------------------------------
来源：http://wfz.nanxuanxn.top

合计 ........... 2106 条
来源：http://nsi.hnxiangtu.top

按章节统计：
来源：http://atm.hnxiangtu.top


<!-- 参考信息 -->