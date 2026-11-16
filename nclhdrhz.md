代发 wailian999

[T47] Perl：正则捕获
来源：http://pyv.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wuh.zhiwuduotai.top

[T48] Perl：正则替换
来源：http://ozm.nanxinkj.top

$s =~ s/old/new/g;
来源：http://apk.snrcjt.cn

[T49] Perl：函数
来源：http://htq.zycfv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://upd.daxiang520.top

[T50] Perl：逐行读文件
来源：http://imc.guannengcc.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xui.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://lau.pycfn.com

[T51] Scala：Hello World
来源：http://ckt.zhixingplan.top

println("Hello")
来源：http://sxf.iojbl.cn

[T52] Scala：变量
来源：http://rgi.ydzc1.top

val a = 1;  var b = 2
来源：http://ffc.guowangkeji.top

[T53] Scala：字符串插值
来源：http://cwh.zhijiandao.cn

s"值: $b"
来源：http://mbn.quarkkingdee.top

[T54] Scala：集合映射
来源：http://tew.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ral.jinqigufen.top

[T55] Scala：集合过滤
来源：http://ioj.aibaodan.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jjv.zhongyouzk.top

[T56] Scala：样例类
来源：http://eui.pycfn.com

case class User(name: String, age: Int)
来源：http://eea.pycfn.com

[T57] Scala：模式匹配
来源：http://buu.quarkkingdee.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yja.yonumen.top

[T58] Scala：函数定义
来源：http://qkg.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://qnk.zhixingplan.top

[T59] Scala：循环
来源：http://dwd.yj20258888.top

for (i <- 1 to 10) println(i)
来源：http://dab.jqgfzy.top

[T60] Scala：折叠
来源：http://fnb.ppjwa.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ohb.hammf.cn

================================================================================
来源：http://xrq.shanyushiyangtech.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cue.zhoulong.xyz

================================================================================
来源：http://nrb.zdqjudy.top

[U01] Py：创建虚拟环境
来源：http://kmo.sxryk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bmv.aibaodan.cn

[U02] Py：导出 / 安装依赖
来源：http://ifk.zhoulong.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jup.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://ogi.ctjpmb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://zse.dianchejie.cn

[U04] Py：变量调试打印
来源：http://fdu.tarul.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bow.cucudq.cn

[U05] Py：列表去重且保序
来源：http://ipf.ydzc1.top

list(dict.fromkeys(arr))
来源：http://izx.aibaodan.cn

[U06] Py：合并两个字典
来源：http://tgf.jqgufenzy.top

{**a, **b}
来源：http://gvq.xinyue.icu

[U07] Py：反转字典键值
来源：http://wfq.hfpthk.cn

{v: k for k, v in d.items()}
来源：http://xuv.fanxiaobao.xyz

[U08] Py：展平二维列表
来源：http://dwg.iojbl.cn

[y for x in nested for y in x]
来源：http://skt.chenzaomai.com

[U09] Py：字典取最大值的键
来源：http://rnc.shanyushiyangtech.top

max(d, key=d.get)
来源：http://zls.pengpengdd.cyou

[U10] Py：按值排序字典
来源：http://gxr.meibo888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tro.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://top.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://vcq.yongpay.top

[U12] Py：取出现最多的 3 个元素
来源：http://doz.cucudq.cn

Counter(arr).most_common(3)
来源：http://hqh.shuidangran.top

[U13] Py：固定长度队列
来源：http://ekn.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://iag.cashguo.top

[U14] Py：分组收集到列表
来源：http://mim.fengsongda.top

defaultdict(list)
来源：http://jgj.xingfuxueyuan.xyz

[U15] Py：高精度计时
来源：http://aec.xuetiantiany.cn

t = time.perf_counter()
来源：http://htm.bbcook.cn

[U16] Py：命令行参数解析
来源：http://dpz.birdmap.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kjg.zhongyouzk.top

[U17] Py：初始化日志
来源：http://ntz.hfpthk.cn

logging.basicConfig(level=logging.INFO)
来源：http://ygx.ybcxt.top

[U18] Py：预编译正则
来源：http://pir.hesvh.cn

pat = re.compile(r"\d+")
来源：http://kvt.shangyingyoupin.top

[U19] Py：正则替换带回调
来源：http://kqp.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kzs.zhixingplan.top

[U20] Py：缓存函数结果
来源：http://oul.cashguo.top

@functools.lru_cache(maxsize=None)
来源：http://bvf.dianchejie.cn

[U21] Py：自定义上下文管理器
来源：http://gpr.redwolf501.top

@contextlib.contextmanager
来源：http://rxy.cdnleiting.top

[U22] Py：矩阵转置
来源：http://pfy.yj20258.top

list(zip(*m))
来源：http://ryw.dashuyun.cn

[U23] Py：分块读取大文件
来源：http://tdf.tian-w.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hmu.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://piw.chenzaomai.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ypo.fehbvm.com

[U25] Py：CSV 按字典读
来源：http://dhb.ydzc1.top

csv.DictReader(f)
来源：http://xzr.yuxming.cn

[U26] Py：并发下载
来源：http://eja.yuxming.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mbt.xylfe.cn

[U27] Py：异步 HTTP
来源：http://jtk.sysykeji.top

aiohttp.ClientSession() 配合 async with
来源：http://ivp.mhx1999.top

[U28] Py：类型别名
来源：http://qrk.xylfe.cn

UserId = int
来源：http://fqf.vqdsnc.cn

[U29] Py：属性校验
来源：http://cbn.sjlbkw.cn

@property 与 @x.setter 配合
来源：http://zqi.shanyushiyangtech.top

[U30] Py：数据类
来源：http://mfq.hywenlv.cn

@dataclass(slots=True)
来源：http://plr.hfpthk.cn

[U31] Py：单测
来源：http://kpc.ybcxt.top

python -m pytest -q
来源：http://dqf.yj20258.top

[U32] Py：代码格式化
来源：http://wml.guowangkeji.top

ruff format . && ruff check --fix .
来源：http://xzu.quarkkingdee.top

[U33] Py：打包发布
来源：http://tmb.yfazqb.com

python -m build  （依赖 pyproject.toml）
来源：http://duw.hesvh.cn

[U34] Py：判断编码
来源：http://swm.gzhubu.top

chardet.detect(raw)
来源：http://lky.jqgufenzy.top

[U35] Py：发送邮件
来源：http://wdo.hnxiangtu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://frb.zycfv.cn

[U36] Py：定时任务
来源：http://xxn.cdnleiting.top

schedule.every(10).minutes.do(job)
来源：http://gqn.tanke756.top

[U37] Py：读写 Excel
来源：http://dto.cdnleiting.top

pandas.read_excel / DataFrame.to_excel
来源：http://kpp.svipenyu.cn

[U38] Py：获取脚本所在目录
来源：http://xdd.0kj1m.cn

Path(__file__).resolve().parent
来源：http://zxw.yuxming.cn

[U39] Py：判断是否在交互环境
来源：http://pub.yj202588.top

sys.stdout.isatty()
来源：http://wye.chenjidiqi.icu

[U40] Py：打印到标准错误
来源：http://wte.daxiang520.top

print("err", file=sys.stderr)
来源：http://oim.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://ywe.tanke756.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lqy.xingfuxueyuan.xyz

[U42] PHP：PSR-4 自动加载
来源：http://tdr.jlsjyb.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uzz.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://jay.aibaodan.cn

namespace App\Http;
来源：http://dhp.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://ewk.yfazqb.com

declare(strict_types=1);
来源：http://cvk.jqgufenzy.top

[U45] PHP：类型声明与返回类型
来源：http://spk.guannengcc.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://daz.guannengcc.top

[U46] PHP：可空类型
来源：http://bek.jlsjyb.cn

?string $name = null
来源：http://jls.redwolf501.top

[U47] PHP：联合类型
来源：http://aoe.jinqigfzy.top

int|string $id
来源：http://zan.jinqigufen.top

[U48] PHP：纯枚举
来源：http://xfp.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wvz.yangfankeji.com

[U49] PHP：只读属性
来源：http://wex.zhaomingkeji.xyz

public readonly string $name
来源：http://skh.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://yot.0kj1m.cn

public function __construct(private int $id) {}
来源：http://onq.hfpthk.cn

[U51] PHP：数组解构
来源：http://zex.xingfuxueyuan.xyz

[$a, $b] = $arr;
来源：http://ers.quarkkingdee.top

[U52] PHP：箭头函数
来源：http://jct.aizwys.cn

$double = fn($x) => $x * 2;
来源：http://xsq.smart0.xyz

[U53] PHP：空合并运算符
来源：http://wri.xuetiantiany.cn

$v = $a ?? $b ?? "default";
来源：http://xyd.andypj.xyz

[U54] PHP：空安全调用
来源：http://lfg.jinqigfzy.top

$obj?->method()
来源：http://gzn.nwbrower.top

[U55] PHP：match 表达式
来源：http://nnt.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wbr.yongpay.top

[U56] PHP：命名参数
来源：http://kwt.yuanzhike.top

f(a: 1, b: 2)
来源：http://dfa.gogol.net.cn

[U57] PHP：字符串插值
来源：http://oau.sxryk.cn

"值: {$a}"
来源：http://nxx.xylfe.cn

[U58] PHP：数组三件套
来源：http://oaw.bjfxy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://deb.zhijiandao.cn

[U59] PHP：自定义排序
来源：http://otj.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lhq.snrcjt.cn

[U60] PHP：JSON 编解码
来源：http://zeh.tianlin.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pcl.jlsjyb.cn

[U61] PHP：正则
来源：http://uio.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ttk.gzhubu.top

[U62] PHP：日期对象
来源：http://pzj.zdbjq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vpy.gaohongyu789.top

[U63] PHP：文件读写
来源：http://cqh.pengpengdd.cyou

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kxq.smart0.xyz

[U64] PHP：目录遍历
来源：http://oda.havefunace.top

glob("dir/*.php");  scandir("dir");
来源：http://blu.pengpengdd.cyou

[U65] PHP：会话
来源：http://ukq.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kep.zhengqikj.top

[U66] PHP：设置 Cookie
来源：http://hkj.snrcjt.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fmx.ywan-chungtsiang.top

[U67] PHP：处理文件上传
来源：http://qbl.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ogd.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://tkr.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vuy.mhx1999.top

[U69] PHP：PDO 预处理
来源：http://yud.yuanzhike.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dbp.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://iyl.zycfv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://soa.yanxiufei.cn

[U71] PHP：抛出异常
来源：http://meg.yj202588.top

throw new RuntimeException("失败", 500);
来源：http://yos.cashguo.top

[U72] PHP：写错误日志
来源：http://qmr.ivvv.top

error_log("失败: " . $e->getMessage());
来源：http://iyo.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://fqv.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://rpx.hnqzz.top

[U74] PHP：读取环境变量
来源：http://bnm.hysaishi.cn

getenv("APP_ENV") ?: "production"
来源：http://qfq.tian-w.cn

[U75] PHP：依赖注入
来源：http://aho.jqgufenzy.top

composer require psr/container
来源：http://ows.fktsv.cn

[U76] PHP：简单路由
来源：http://zki.yj20258.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zbg.zdbjq.cn

[U77] PHP：模板渲染
来源：http://etr.yvedp.cn

composer require twig/twig
来源：http://xqb.andypj.xyz

[U78] PHP：单元测试
来源：http://vfw.316326.xyz

composer require --dev phpunit/phpunit
来源：http://qlf.xingfuxueyuan.xyz

[U79] PHP：静态分析
来源：http://ugm.epnwcf.com

composer require --dev phpstan/phpstan
来源：http://vwp.yj202588.top

[U80] PHP：代码规范修复
来源：http://mpr.jiagoushi.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wfp.jinghuilouyu.cn

[U81] JS：初始化项目
来源：http://dax.iojbl.cn

npm init -y;  npm i express
来源：http://xso.gzhubu.top

[U82] JS：package.json 脚本
来源：http://dqh.svipenyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pws.haohaochexian.top

[U83] JS：ES Module 导入导出
来源：http://ibs.yuanzhike.top

export const a = 1;  import { a } from "./m.js";
来源：http://qag.feifeiyinyue.top

[U84] JS：CommonJS 写法
来源：http://ouz.xylfe.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uwx.sufxvd.cn

[U85] JS：可选链
来源：http://pay.daria6918.cn

a?.b?.c
来源：http://avd.fanxiaobao.xyz

[U86] JS：空值合并
来源：http://cwa.cashguo.top

a ?? b
来源：http://dsc.zhiwuduotai.top

[U87] JS：解构默认值
来源：http://lgn.redwolf501.top

const { a = 1, b = 2 } = obj;
来源：http://gla.birdmap.top

[U88] JS：对象展开合并
来源：http://zof.9152youxi.cn

{ ...a, ...b }
来源：http://ebu.zhongyouzk.top

[U89] JS：数组去重
来源：http://tqi.316326.xyz

[...new Set(arr)]
来源：http://ddf.bjfxy.top

[U90] JS：数字数组排序
来源：http://tqa.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://guo.yuanzhike.top

[U91] JS：对象键值遍历
来源：http://trw.sjlbkw.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lll.jinqigfzy.top

[U92] JS：深拷贝
来源：http://zay.tianlin.xyz

structuredClone(obj)
来源：http://eor.jinghuilouyu.cn

[U93] JS：模板字符串
来源：http://gea.meibo888.top

`共 ${n} 条`
来源：http://ytz.ctjpmb.com

[U94] JS：箭头函数
来源：http://qyk.zhijiandao.cn

const double = x => x * 2;
来源：http://vve.zhongyouzk.top

[U95] JS：Promise 包装
来源：http://aim.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://qqb.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://wre.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://icv.ywan-chungtsiang.top

[U97] JS：并发请求
来源：http://oac.zhixingplan.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hbl.havefunace.top

[U98] JS：fetch 带 JSON
来源：http://coe.ydzc1.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ypb.ivvv.top

[U99] JS：事件监听
来源：http://idi.yonumen.top

el.addEventListener("click", e => {})
来源：http://cnh.aizwys.cn

[U100] JS：DOM 查询
来源：http://qru.epnwcf.com

document.querySelector(".item")
来源：http://hvg.cqqwz.cn

[U101] JS：classList 操作
来源：http://llj.pengpengdd.cyou

el.classList.toggle("active")
来源：http://vxi.jinqigufen.top

[U102] JS：本地存储
来源：http://wzo.dianchejie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tqk.epnwcf.com

[U103] JS：定时器
来源：http://nqg.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ffi.xuetiantiany.cn

[U104] JS：防抖
来源：http://iou.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mii.guowangkeji.top

[U105] JS：节流
来源：http://omy.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://abg.hywenlv.cn

[U106] JS：日期格式化
来源：http://xni.bbcook.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lnq.tianlin.xyz

[U107] JS：数字千分位
来源：http://axk.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mjy.dianchejie.cn

[U108] JS：随机整数
来源：http://xlm.fanxiaobao.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kog.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://ifa.hywenlv.cn

Object.groupBy(arr, x => x.type)
来源：http://rlb.hysaishi.cn

[U110] JS：数组分块
来源：http://zzj.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jzk.yangfankeji.com

[U111] JS：对象转 Map
来源：http://qim.nanxinkj.top

new Map(Object.entries(obj))
来源：http://hje.tianlin.xyz

[U112] JS：字符串补位
来源：http://uwi.tarul.cn

"7".padStart(3, "0")
来源：http://tft.birdmap.top

[U113] JS：正则替换全部
来源：http://wzb.uphjek.com

s.replaceAll("a", "b")
来源：http://izv.fehbvm.com

[U114] JS：JSON 深比较
来源：http://rxl.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ccx.yj20258.top

[U115] JS：生成 UUID
来源：http://gul.ppjwa.cn

crypto.randomUUID()
来源：http://qqh.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://lac.svipenyu.cn

/** @param {string} name */ function f(name) {}
来源：http://rvx.zdqjudy.top

[U117] JS：单元测试
来源：http://jho.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://pve.jqgufenzy.top

[U118] JS：开发服务器
来源：http://rpw.vehdjk.com

npm i -D vite;  npx vite
来源：http://mjx.ivvv.top

[U119] JS：生产构建
来源：http://vnb.smart0.xyz

npx vite build
来源：http://uvf.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://hqo.jyoumei.cn

import.meta.env.VITE_API_URL
来源：http://fmy.jinyuanbaomall.cn

================================================================================
来源：http://rqi.zhoulong.xyz

统计汇总
来源：http://zzd.zhixingplan.top

================================================================================
来源：http://mdo.chenzaomai.com

按语言统计（条）：
来源：http://mrk.316326.xyz

Python ......... 252
来源：http://ajo.yuanzhike.top

PHP ............ 252
来源：http://gge.yongpay.top

JavaScript ..... 252
来源：http://ruk.zhixingplan.top

TypeScript ..... 212
来源：http://pmo.jinqigfzy.top

Java ........... 212
来源：http://ojh.zhengqikj.top

Go ............. 212
来源：http://use.0kj1m.cn

Ruby ........... 212
来源：http://atp.jiagoushi.top

C# ............. 212
来源：http://ghh.jinyuanbaomall.cn

C .............. 30
来源：http://khk.birdmap.top

C++ ............ 30
来源：http://pti.zhoulong.xyz

SQL ............ 90
来源：http://vvl.redwolf501.top

Bash ........... 80
来源：http://pue.yongpay.top

Kotlin ......... 15
来源：http://tir.cdnleiting.top

Swift .......... 15
来源：http://snv.epnwcf.com

Lua ............ 10
来源：http://vir.chenlongwang.top

Perl ........... 10
来源：http://zib.yueranfly.top

Scala .......... 10
来源：http://dgo.dianchejie.cn

------------------------------------
来源：http://zwc.hywenlv.cn

合计 ........... 2106 条
来源：http://lil.bbcook.cn

按章节统计：
来源：http://rnf.hammf.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hvk.ybcxt.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kuz.xinyue.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://twk.wangshuangyany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iih.aibaodan.cn


<!-- 参考信息 -->