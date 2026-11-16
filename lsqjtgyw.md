代发 wailian999

[T43] Perl：字符串插值
来源：http://urf.tanke756.top

"值: $a"
来源：http://fcs.cdnleiting.top

[T44] Perl：条件
来源：http://rqb.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://amv.hnxiangtu.top

[T45] Perl：数组遍历
来源：http://bdi.cashguo.top

for my $x (@arr) { print $x; }
来源：http://iyg.dianchejie.cn

[T46] Perl：哈希操作
来源：http://zkx.uphjek.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fqd.gaohongyu789.top

[T47] Perl：正则捕获
来源：http://qnk.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://ogk.dianchejie.cn

[T48] Perl：正则替换
来源：http://dac.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://mfy.yangfankeji.com

[T49] Perl：函数
来源：http://nwi.daria6918.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jzc.zhaomingkeji.xyz

[T50] Perl：逐行读文件
来源：http://nkh.hammf.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nqh.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://dfq.sysykeji.top

[T51] Scala：Hello World
来源：http://pzs.bjfxy.top

println("Hello")
来源：http://jep.jyoumei.cn

[T52] Scala：变量
来源：http://weq.iojbl.cn

val a = 1;  var b = 2
来源：http://csm.xziqi.cn

[T53] Scala：字符串插值
来源：http://fod.ywan-chungtsiang.top

s"值: $b"
来源：http://mwq.sjlbkw.cn

[T54] Scala：集合映射
来源：http://kyu.gaohongyu789.top

List(1, 2, 3).map(_ * 2)
来源：http://eii.gaohongyu789.top

[T55] Scala：集合过滤
来源：http://hvv.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ywd.nanxinkj.top

[T56] Scala：样例类
来源：http://qwa.yj20258888.top

case class User(name: String, age: Int)
来源：http://drl.mhx1999.top

[T57] Scala：模式匹配
来源：http://jce.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wua.sufxvd.cn

[T58] Scala：函数定义
来源：http://kzp.shanyushiyangtech.top

def add(a: Int, b: Int): Int = a + b
来源：http://snd.tianlin.xyz

[T59] Scala：循环
来源：http://rck.zycfv.cn

for (i <- 1 to 10) println(i)
来源：http://pjn.tian-w.cn

[T60] Scala：折叠
来源：http://usz.jlsjyb.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ugg.yanxiufei.cn

================================================================================
来源：http://jyi.fanxiaobao.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vju.gaohongyu789.top

================================================================================
来源：http://huy.gotoacloud.top

[U01] Py：创建虚拟环境
来源：http://hjg.xuanzx.com

python -m venv .venv && source .venv/bin/activate
来源：http://pei.sjlbkw.cn

[U02] Py：导出 / 安装依赖
来源：http://svo.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bdf.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://ixs.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hme.svipenyu.cn

[U04] Py：变量调试打印
来源：http://bwa.9152youxi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pep.xingfuxueyuan.xyz

[U05] Py：列表去重且保序
来源：http://vkt.snrcjt.cn

list(dict.fromkeys(arr))
来源：http://uvj.gogol.net.cn

[U06] Py：合并两个字典
来源：http://cqt.smart0.xyz

{**a, **b}
来源：http://jmr.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://mvl.dashuyun.cn

{v: k for k, v in d.items()}
来源：http://cwx.dianchejie.cn

[U08] Py：展平二维列表
来源：http://xly.ivvv.top

[y for x in nested for y in x]
来源：http://ubn.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://ela.bbcook.cn

max(d, key=d.get)
来源：http://bfj.smart0.xyz

[U10] Py：按值排序字典
来源：http://eqd.ydzc1.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rro.gaohongyu789.top

[U11] Py：生成器表达式
来源：http://qsl.daxiang520.top

(x * 2 for x in arr)
来源：http://ewd.andypj.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://gxz.ydjk.org.cn

Counter(arr).most_common(3)
来源：http://jbt.vehdjk.com

[U13] Py：固定长度队列
来源：http://uhm.jyoumei.cn

deque(maxlen=10)
来源：http://iia.hesvh.cn

[U14] Py：分组收集到列表
来源：http://ufd.jiagoushi.top

defaultdict(list)
来源：http://loe.zdqjudy.top

[U15] Py：高精度计时
来源：http://fty.shanyushiyangkeji.top

t = time.perf_counter()
来源：http://vtr.ydjk.org.cn

[U16] Py：命令行参数解析
来源：http://xdd.tian-w.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qyv.guannengcc.top

[U17] Py：初始化日志
来源：http://kej.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://bkv.xuanzx.com

[U18] Py：预编译正则
来源：http://ysv.yj20258888.top

pat = re.compile(r"\d+")
来源：http://dga.vqdsnc.cn

[U19] Py：正则替换带回调
来源：http://nnd.zhongyouzk.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oux.sweek.top

[U20] Py：缓存函数结果
来源：http://doa.xziqi.cn

@functools.lru_cache(maxsize=None)
来源：http://jcz.zdbjq.cn

[U21] Py：自定义上下文管理器
来源：http://ojp.jianghu66.top

@contextlib.contextmanager
来源：http://juv.yvedp.cn

[U22] Py：矩阵转置
来源：http://uyh.chenjidiqi.icu

list(zip(*m))
来源：http://pjv.andypj.xyz

[U23] Py：分块读取大文件
来源：http://taw.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vve.zhengqikj.top

[U24] Py：路径操作
来源：http://mtl.cdnleiting.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jac.fengsongda.top

[U25] Py：CSV 按字典读
来源：http://loz.hesvh.cn

csv.DictReader(f)
来源：http://ffe.havefunace.top

[U26] Py：并发下载
来源：http://oxx.shanyushiyangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zej.wangdashe.top

[U27] Py：异步 HTTP
来源：http://iyu.gotoacloud.top

aiohttp.ClientSession() 配合 async with
来源：http://dkb.daria6918.cn

[U28] Py：类型别名
来源：http://wtl.andypj.xyz

UserId = int
来源：http://qfd.hongshengwenyu.top

[U29] Py：属性校验
来源：http://vrx.jiagoushi.top

@property 与 @x.setter 配合
来源：http://vky.nanxinkj.top

[U30] Py：数据类
来源：http://frx.gogol.net.cn

@dataclass(slots=True)
来源：http://gnb.daria6918.cn

[U31] Py：单测
来源：http://jgi.yvedp.cn

python -m pytest -q
来源：http://jqh.ywan-chungtsiang.top

[U32] Py：代码格式化
来源：http://jon.ywan-chungtsiang.top

ruff format . && ruff check --fix .
来源：http://rgt.cdnleiting.top

[U33] Py：打包发布
来源：http://amf.yongpay.top

python -m build  （依赖 pyproject.toml）
来源：http://okw.nanxinkj.top

[U34] Py：判断编码
来源：http://xty.meibo888.top

chardet.detect(raw)
来源：http://jxe.wangdashe.top

[U35] Py：发送邮件
来源：http://zzw.smart0.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cxr.smart0.xyz

[U36] Py：定时任务
来源：http://psz.xingfuxueyuan.xyz

schedule.every(10).minutes.do(job)
来源：http://pfv.xuanzx.com

[U37] Py：读写 Excel
来源：http://dwf.cdnleiting.top

pandas.read_excel / DataFrame.to_excel
来源：http://roc.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://yak.jianghu66.top

Path(__file__).resolve().parent
来源：http://tya.yj20258888.top

[U39] Py：判断是否在交互环境
来源：http://ena.shanyushiyangkeji.top

sys.stdout.isatty()
来源：http://izd.chenjidiqi.icu

[U40] Py：打印到标准错误
来源：http://wwz.havefunace.top

print("err", file=sys.stderr)
来源：http://zwv.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://qyk.fehbvm.com

composer init;  composer require guzzlehttp/guzzle
来源：http://tns.redwolf501.top

[U42] PHP：PSR-4 自动加载
来源：http://yeh.yj202588.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nes.c1oappe.top

[U43] PHP：声明命名空间
来源：http://rjn.iojbl.cn

namespace App\Http;
来源：http://dyh.yvedp.cn

[U44] PHP：开启严格类型
来源：http://cne.tanke756.top

declare(strict_types=1);
来源：http://fpg.yongpay.top

[U45] PHP：类型声明与返回类型
来源：http://vle.yj20258888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yxl.jlsjyb.cn

[U46] PHP：可空类型
来源：http://eqy.shanyushiyangkeji.top

?string $name = null
来源：http://vmo.0kj1m.cn

[U47] PHP：联合类型
来源：http://qrh.daxiang520.top

int|string $id
来源：http://xiu.andypj.xyz

[U48] PHP：纯枚举
来源：http://uzh.hysaishi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pik.yuanzhike.top

[U49] PHP：只读属性
来源：http://vbj.pycfn.com

public readonly string $name
来源：http://ysq.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://dwp.xuetiantiany.cn

public function __construct(private int $id) {}
来源：http://goo.fehbvm.com

[U51] PHP：数组解构
来源：http://wks.jinqigfzy.top

[$a, $b] = $arr;
来源：http://bst.tian-w.cn

[U52] PHP：箭头函数
来源：http://pue.jianghu66.top

$double = fn($x) => $x * 2;
来源：http://woe.aizwys.cn

[U53] PHP：空合并运算符
来源：http://pwk.havefunace.top

$v = $a ?? $b ?? "default";
来源：http://nqd.sufxvd.cn

[U54] PHP：空安全调用
来源：http://tgu.c1oappe.top

$obj?->method()
来源：http://zoj.hywenlv.cn

[U55] PHP：match 表达式
来源：http://vbn.chenzaomai.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ciy.jiagoushi.top

[U56] PHP：命名参数
来源：http://wap.yangfankeji.com

f(a: 1, b: 2)
来源：http://mfk.yj202588.top

[U57] PHP：字符串插值
来源：http://kte.nanxinkj.top

"值: {$a}"
来源：http://rrv.xziqi.cn

[U58] PHP：数组三件套
来源：http://mzd.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jch.jianghu66.top

[U59] PHP：自定义排序
来源：http://imy.bbcook.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tsl.tarul.cn

[U60] PHP：JSON 编解码
来源：http://vwx.zdbjq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://abt.bjfxy.top

[U61] PHP：正则
来源：http://sal.nanxinkj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://igh.jinqigufen.top

[U62] PHP：日期对象
来源：http://shp.hcnkem.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ori.sxryk.cn

[U63] PHP：文件读写
来源：http://ifv.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sfg.chenzaomai.com

[U64] PHP：目录遍历
来源：http://lrl.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://qsw.quarkkingdee.top

[U65] PHP：会话
来源：http://wkn.hammf.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gww.tarul.cn

[U66] PHP：设置 Cookie
来源：http://gbj.dianchejie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aho.chenjidiqi.icu

[U67] PHP：处理文件上传
来源：http://sdi.yonumen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bih.haohaochexian.top

[U68] PHP：PDO 连接
来源：http://boo.xuetiantiany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hiu.aibaodan.cn

[U69] PHP：PDO 预处理
来源：http://afb.jinqigufen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qko.quarkkingdee.top

[U70] PHP：PDO 事务
来源：http://vda.nanxuanxn.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://clm.cdnleiting.top

[U71] PHP：抛出异常
来源：http://raf.hnxiangtu.top

throw new RuntimeException("失败", 500);
来源：http://bkn.pengpengdd.cyou

[U72] PHP：写错误日志
来源：http://emw.birdmap.top

error_log("失败: " . $e->getMessage());
来源：http://lsc.vehdjk.com

[U73] PHP：读取 ini 配置
来源：http://qzb.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://cwn.cucudq.cn

[U74] PHP：读取环境变量
来源：http://fsg.yj20258.top

getenv("APP_ENV") ?: "production"
来源：http://zbl.havefunace.top

[U75] PHP：依赖注入
来源：http://mzs.mhx1999.top

composer require psr/container
来源：http://fwa.uphjek.com

[U76] PHP：简单路由
来源：http://oai.yfazqb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://edl.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://gka.aizwys.cn

composer require twig/twig
来源：http://lpt.shanyushiyangkeji.top

[U78] PHP：单元测试
来源：http://amb.shanyushiyangtech.top

composer require --dev phpunit/phpunit
来源：http://vdy.zhoulong.xyz

[U79] PHP：静态分析
来源：http://sjg.havefunace.top

composer require --dev phpstan/phpstan
来源：http://dff.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://djh.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://qvz.smart0.xyz

[U81] JS：初始化项目
来源：http://xyb.cashguo.top

npm init -y;  npm i express
来源：http://aot.vqdsnc.cn

[U82] JS：package.json 脚本
来源：http://tkv.wangshuangyany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ejl.ydzc1.top

[U83] JS：ES Module 导入导出
来源：http://ayd.yueranfly.top

export const a = 1;  import { a } from "./m.js";
来源：http://iob.wangshuangyany.cn

[U84] JS：CommonJS 写法
来源：http://pwd.daxiang520.top

module.exports = { a };  const { a } = require("./m");
来源：http://ilt.xingfuxueyuan.xyz

[U85] JS：可选链
来源：http://lzy.cheryme.top

a?.b?.c
来源：http://vzo.bjfxy.top

[U86] JS：空值合并
来源：http://uyd.yj20258888.top

a ?? b
来源：http://yid.sjlbkw.cn

[U87] JS：解构默认值
来源：http://xdm.fengsongda.top

const { a = 1, b = 2 } = obj;
来源：http://erp.yj202588.top

[U88] JS：对象展开合并
来源：http://dxg.jqgufenzy.top

{ ...a, ...b }
来源：http://zvy.9152youxi.cn

[U89] JS：数组去重
来源：http://vjb.hysaishi.cn

[...new Set(arr)]
来源：http://izi.zycfv.cn

[U90] JS：数字数组排序
来源：http://tog.hongshengwenyu.top

[...arr].sort((a, b) => a - b)
来源：http://wxc.guannengcc.top

[U91] JS：对象键值遍历
来源：http://nud.vehdjk.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rqi.sxryk.cn

[U92] JS：深拷贝
来源：http://ubb.hfpthk.cn

structuredClone(obj)
来源：http://mfp.svipenyu.cn

[U93] JS：模板字符串
来源：http://tqh.yvedp.cn

`共 ${n} 条`
来源：http://knl.yvedp.cn

[U94] JS：箭头函数
来源：http://eek.fzhhl.top

const double = x => x * 2;
来源：http://vmh.vehdjk.com

[U95] JS：Promise 包装
来源：http://eyf.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://rcm.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://ydy.fehbvm.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qzj.c1oappe.top

[U97] JS：并发请求
来源：http://pip.wangdashe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://prv.zdbjq.cn

[U98] JS：fetch 带 JSON
来源：http://qtf.jyoumei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mpj.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://bqy.cucudq.cn

el.addEventListener("click", e => {})
来源：http://zqs.fzhhl.top

[U100] JS：DOM 查询
来源：http://wsu.fanxiaobao.xyz

document.querySelector(".item")
来源：http://elz.ehwqpu.com

[U101] JS：classList 操作
来源：http://saf.wangshuangyany.cn

el.classList.toggle("active")
来源：http://xvj.haohaochexian.top

[U102] JS：本地存储
来源：http://mfz.jinqigufen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://asr.xinyue.icu

[U103] JS：定时器
来源：http://rxl.uphjek.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hun.havefunace.top

[U104] JS：防抖
来源：http://srz.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dwc.svipenyu.cn

[U105] JS：节流
来源：http://kfs.pengpengdd.cyou

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://syx.bbcook.cn

[U106] JS：日期格式化
来源：http://evh.xuetiantiany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rjn.ctjpmb.com

[U107] JS：数字千分位
来源：http://ggs.wangshuangyany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dtq.zhiwuduotai.top

[U108] JS：随机整数
来源：http://mzp.52xcode.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://stt.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://kff.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://nlc.hysaishi.cn

[U110] JS：数组分块
来源：http://tcw.chenlongwang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zdw.yuxming.cn

[U111] JS：对象转 Map
来源：http://uiw.sjlbkw.cn

new Map(Object.entries(obj))
来源：http://uvm.zhijiandao.cn

[U112] JS：字符串补位
来源：http://gii.yvedp.cn

"7".padStart(3, "0")
来源：http://zqy.zdbjq.cn

[U113] JS：正则替换全部
来源：http://gkg.yj20258.top

s.replaceAll("a", "b")
来源：http://lyu.mhx1999.top

[U114] JS：JSON 深比较
来源：http://qtx.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qjm.xziqi.cn

[U115] JS：生成 UUID
来源：http://sej.tanke756.top

crypto.randomUUID()
来源：http://gtl.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://nor.sysykeji.top

/** @param {string} name */ function f(name) {}
来源：http://gdf.yuxming.cn

[U117] JS：单元测试
来源：http://jse.cashguo.top

npm i -D vitest;  npx vitest
来源：http://qtc.guannengcc.top

[U118] JS：开发服务器
来源：http://utk.yvedp.cn

npm i -D vite;  npx vite
来源：http://tsn.ydjk.org.cn

[U119] JS：生产构建
来源：http://uhk.vehdjk.com

npx vite build
来源：http://afu.zhongyouzk.top

[U120] JS：读取环境变量（Vite）
来源：http://grg.yonumen.top

import.meta.env.VITE_API_URL
来源：http://unl.zhaomingkeji.xyz

================================================================================
来源：http://pnj.jyoumei.cn

统计汇总
来源：http://gaz.shangyingyoupin.top

================================================================================
来源：http://vwx.sweek.top

按语言统计（条）：
来源：http://fpi.shzxlz.cn

Python ......... 252
来源：http://lwn.ywan-chungtsiang.top

PHP ............ 252
来源：http://nqb.52xcode.cn

JavaScript ..... 252
来源：http://lji.hywenlv.cn

TypeScript ..... 212
来源：http://bsk.tarul.cn

Java ........... 212
来源：http://nki.ybcxt.top

Go ............. 212
来源：http://law.yuanzhike.top

Ruby ........... 212
来源：http://lzz.yvedp.cn

C# ............. 212
来源：http://zfl.cashguo.top

C .............. 30
来源：http://ddx.tarul.cn

C++ ............ 30
来源：http://ven.xuetiantiany.cn

SQL ............ 90
来源：http://bok.fzhhl.top

Bash ........... 80
来源：http://rwb.sjlbkw.cn

Kotlin ......... 15
来源：http://ibl.chenjidiqi.icu

Swift .......... 15
来源：http://yll.ydzc1.top

Lua ............ 10
来源：http://yge.svipenyu.cn

Perl ........... 10
来源：http://mgz.jinqigfzy.top


<!-- 参考信息 -->