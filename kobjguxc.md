代发 wailian999

[T47] Perl：正则捕获
来源：http://xyk.uphjek.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://xqf.tanke756.top

[T48] Perl：正则替换
来源：http://uhg.c1oappe.top

$s =~ s/old/new/g;
来源：http://cjr.gaohongyu789.top

[T49] Perl：函数
来源：http://lgp.fktsv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qed.9152youxi.cn

[T50] Perl：逐行读文件
来源：http://per.xziqi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ola.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://sxi.chenlongwang.top

[T51] Scala：Hello World
来源：http://jwx.cheryme.top

println("Hello")
来源：http://tce.daria6918.cn

[T52] Scala：变量
来源：http://nra.gogol.net.cn

val a = 1;  var b = 2
来源：http://oxi.xuetiantiany.cn

[T53] Scala：字符串插值
来源：http://kzh.yvedp.cn

s"值: $b"
来源：http://fzf.zhengqikj.top

[T54] Scala：集合映射
来源：http://rpp.cashguo.top

List(1, 2, 3).map(_ * 2)
来源：http://mqo.gaohongyu789.top

[T55] Scala：集合过滤
来源：http://msy.chenzaomai.com

List(1, 2, 3).filter(_ > 1)
来源：http://egq.aizwys.cn

[T56] Scala：样例类
来源：http://dyj.birdmap.top

case class User(name: String, age: Int)
来源：http://vgr.tarul.cn

[T57] Scala：模式匹配
来源：http://ltv.yanxiufei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bsu.jlsjyb.cn

[T58] Scala：函数定义
来源：http://ppn.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://zsc.hnqzz.top

[T59] Scala：循环
来源：http://vku.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://dwi.daria6918.cn

[T60] Scala：折叠
来源：http://oeb.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qad.yonumen.top

================================================================================
来源：http://sqt.yonumen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lol.9152youxi.cn

================================================================================
来源：http://jmc.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://uxu.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://syo.hysaishi.cn

[U02] Py：导出 / 安装依赖
来源：http://hrn.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ykg.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://fvr.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jja.cdnleiting.top

[U04] Py：变量调试打印
来源：http://crz.sysykeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wkh.chenzaomai.com

[U05] Py：列表去重且保序
来源：http://zfx.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://rcr.hysaishi.cn

[U06] Py：合并两个字典
来源：http://kuw.tarul.cn

{**a, **b}
来源：http://slw.yongpay.top

[U07] Py：反转字典键值
来源：http://omi.gzhubu.top

{v: k for k, v in d.items()}
来源：http://qfs.zhaomingkeji.xyz

[U08] Py：展平二维列表
来源：http://itn.yvedp.cn

[y for x in nested for y in x]
来源：http://pao.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://lnf.zhoulong.xyz

max(d, key=d.get)
来源：http://kcl.hnxiangtu.top

[U10] Py：按值排序字典
来源：http://bpk.fehbvm.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nir.uphjek.com

[U11] Py：生成器表达式
来源：http://isz.52xcode.cn

(x * 2 for x in arr)
来源：http://odl.yj20258.top

[U12] Py：取出现最多的 3 个元素
来源：http://zoy.sufxvd.cn

Counter(arr).most_common(3)
来源：http://kin.shuidangran.top

[U13] Py：固定长度队列
来源：http://bhd.shuidangran.top

deque(maxlen=10)
来源：http://rqf.daxiang520.top

[U14] Py：分组收集到列表
来源：http://krf.guowangkeji.top

defaultdict(list)
来源：http://qze.9152youxi.cn

[U15] Py：高精度计时
来源：http://con.yongpay.top

t = time.perf_counter()
来源：http://des.zhongyouzk.top

[U16] Py：命令行参数解析
来源：http://sle.jinyuanbaomall.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qny.ctjpmb.com

[U17] Py：初始化日志
来源：http://qsl.xuanzx.com

logging.basicConfig(level=logging.INFO)
来源：http://acp.gzhubu.top

[U18] Py：预编译正则
来源：http://ctd.fanxiaobao.xyz

pat = re.compile(r"\d+")
来源：http://syq.ivvv.top

[U19] Py：正则替换带回调
来源：http://paa.fengsongda.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xyh.daria6918.cn

[U20] Py：缓存函数结果
来源：http://cbr.316326.xyz

@functools.lru_cache(maxsize=None)
来源：http://nwh.yuanzhike.top

[U21] Py：自定义上下文管理器
来源：http://ggc.zdbjq.cn

@contextlib.contextmanager
来源：http://beg.hongshengwenyu.top

[U22] Py：矩阵转置
来源：http://hqp.yuxming.cn

list(zip(*m))
来源：http://imy.jinqigufen.top

[U23] Py：分块读取大文件
来源：http://eao.hesvh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ace.zhixingplan.top

[U24] Py：路径操作
来源：http://nzz.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://soi.c1oappe.top

[U25] Py：CSV 按字典读
来源：http://zcx.kuanghao11.cn

csv.DictReader(f)
来源：http://bkr.pycfn.com

[U26] Py：并发下载
来源：http://vcx.tian-w.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://grd.jyoumei.cn

[U27] Py：异步 HTTP
来源：http://uxb.hysaishi.cn

aiohttp.ClientSession() 配合 async with
来源：http://dop.gotoacloud.top

[U28] Py：类型别名
来源：http://klu.wangdashe.top

UserId = int
来源：http://rzb.andypj.xyz

[U29] Py：属性校验
来源：http://cso.hfpthk.cn

@property 与 @x.setter 配合
来源：http://vuv.nanxuanxn.top

[U30] Py：数据类
来源：http://mrz.shangyingyoupin.top

@dataclass(slots=True)
来源：http://sor.jqgufenzy.top

[U31] Py：单测
来源：http://kah.ybcxt.top

python -m pytest -q
来源：http://mfj.ybcxt.top

[U32] Py：代码格式化
来源：http://liv.daria6918.cn

ruff format . && ruff check --fix .
来源：http://mae.yanxiufei.cn

[U33] Py：打包发布
来源：http://pzs.daria6918.cn

python -m build  （依赖 pyproject.toml）
来源：http://cdd.yonumen.top

[U34] Py：判断编码
来源：http://qkx.yvedp.cn

chardet.detect(raw)
来源：http://mct.dianchejie.cn

[U35] Py：发送邮件
来源：http://qoe.nanxuanxn.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fup.jianghu66.top

[U36] Py：定时任务
来源：http://cae.9152youxi.cn

schedule.every(10).minutes.do(job)
来源：http://qzr.feifeiyinyue.top

[U37] Py：读写 Excel
来源：http://gwx.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qpq.xuanzx.com

[U38] Py：获取脚本所在目录
来源：http://iim.ywan-chungtsiang.top

Path(__file__).resolve().parent
来源：http://hwd.ydjk.org.cn

[U39] Py：判断是否在交互环境
来源：http://fpy.c1oappe.top

sys.stdout.isatty()
来源：http://pku.316326.xyz

[U40] Py：打印到标准错误
来源：http://kub.yvedp.cn

print("err", file=sys.stderr)
来源：http://zcu.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://yjj.feifeiyinyue.top

composer init;  composer require guzzlehttp/guzzle
来源：http://tng.yuxming.cn

[U42] PHP：PSR-4 自动加载
来源：http://bin.shanyushiyangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nwl.zycfv.cn

[U43] PHP：声明命名空间
来源：http://jwa.shuidangran.top

namespace App\Http;
来源：http://agw.yanxiufei.cn

[U44] PHP：开启严格类型
来源：http://bcx.tian-w.cn

declare(strict_types=1);
来源：http://lsw.feifeiyinyue.top

[U45] PHP：类型声明与返回类型
来源：http://zut.guannengcc.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://eae.52xcode.cn

[U46] PHP：可空类型
来源：http://vkh.nwbrower.top

?string $name = null
来源：http://yle.tarul.cn

[U47] PHP：联合类型
来源：http://lqj.sysykeji.top

int|string $id
来源：http://nmu.yuanzhike.top

[U48] PHP：纯枚举
来源：http://ayr.uphjek.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://srl.52xcode.cn

[U49] PHP：只读属性
来源：http://lhx.vqdsnc.cn

public readonly string $name
来源：http://vxi.zhongyouzk.top

[U50] PHP：构造器属性提升
来源：http://wic.ivvv.top

public function __construct(private int $id) {}
来源：http://ngs.zhoulong.xyz

[U51] PHP：数组解构
来源：http://hlv.smart0.xyz

[$a, $b] = $arr;
来源：http://jsu.jianghu66.top

[U52] PHP：箭头函数
来源：http://wwx.chenjidiqi.icu

$double = fn($x) => $x * 2;
来源：http://wjy.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://ufo.cqqwz.cn

$v = $a ?? $b ?? "default";
来源：http://biw.wangshuangyany.cn

[U54] PHP：空安全调用
来源：http://nkc.xingfuxueyuan.xyz

$obj?->method()
来源：http://hhb.zycfv.cn

[U55] PHP：match 表达式
来源：http://oxg.tarul.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eef.cqqwz.cn

[U56] PHP：命名参数
来源：http://lgb.ybcxt.top

f(a: 1, b: 2)
来源：http://mtl.hammf.cn

[U57] PHP：字符串插值
来源：http://kat.snrcjt.cn

"值: {$a}"
来源：http://vln.yj202588.top

[U58] PHP：数组三件套
来源：http://qdk.ydjk.org.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cjo.ydjk.org.cn

[U59] PHP：自定义排序
来源：http://uac.cashguo.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nyo.haohaochexian.top

[U60] PHP：JSON 编解码
来源：http://rxw.uphjek.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://acx.svipenyu.cn

[U61] PHP：正则
来源：http://uhf.jqgfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ctz.andypj.xyz

[U62] PHP：日期对象
来源：http://hxp.tianlin.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gma.ydzc1.top

[U63] PHP：文件读写
来源：http://fsw.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xhd.havefunace.top

[U64] PHP：目录遍历
来源：http://fll.chenjidiqi.icu

glob("dir/*.php");  scandir("dir");
来源：http://nxg.zhijiandao.cn

[U65] PHP：会话
来源：http://xfq.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://eal.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://guz.aizwys.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sav.xuanzx.com

[U67] PHP：处理文件上传
来源：http://bmw.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wjh.yfazqb.com

[U68] PHP：PDO 连接
来源：http://qfa.cdnleiting.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://scc.zhongyouzk.top

[U69] PHP：PDO 预处理
来源：http://ppt.chenzaomai.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xhc.andypj.xyz

[U70] PHP：PDO 事务
来源：http://rpd.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hhm.cqqwz.cn

[U71] PHP：抛出异常
来源：http://pjq.guannengcc.top

throw new RuntimeException("失败", 500);
来源：http://xhi.9152youxi.cn

[U72] PHP：写错误日志
来源：http://qub.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://bzq.sweek.top

[U73] PHP：读取 ini 配置
来源：http://ioc.pengpengdd.cyou

parse_ini_file("config.ini", true)
来源：http://amr.jianghu66.top

[U74] PHP：读取环境变量
来源：http://gmd.fktsv.cn

getenv("APP_ENV") ?: "production"
来源：http://smm.svipenyu.cn

[U75] PHP：依赖注入
来源：http://tff.zhixingplan.top

composer require psr/container
来源：http://sui.pengpengdd.cyou

[U76] PHP：简单路由
来源：http://fvl.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mac.yuanzhike.top

[U77] PHP：模板渲染
来源：http://tmz.hongshengwenyu.top

composer require twig/twig
来源：http://teu.haohaochexian.top

[U78] PHP：单元测试
来源：http://udv.dashuyun.cn

composer require --dev phpunit/phpunit
来源：http://nqv.aibaodan.cn

[U79] PHP：静态分析
来源：http://dax.nanxinkj.top

composer require --dev phpstan/phpstan
来源：http://ght.gogol.net.cn

[U80] PHP：代码规范修复
来源：http://fpn.daria6918.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://iob.jianghu66.top

[U81] JS：初始化项目
来源：http://niy.snrcjt.cn

npm init -y;  npm i express
来源：http://ydp.epnwcf.com

[U82] JS：package.json 脚本
来源：http://zoz.fehbvm.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nus.jqgfzy.top

[U83] JS：ES Module 导入导出
来源：http://iuo.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bjx.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://edv.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://joh.birdmap.top

[U85] JS：可选链
来源：http://jvv.snrcjt.cn

a?.b?.c
来源：http://gkw.zhijiandao.cn

[U86] JS：空值合并
来源：http://jel.gzhubu.top

a ?? b
来源：http://gxf.pycfn.com

[U87] JS：解构默认值
来源：http://zhx.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://wou.xingfuxueyuan.xyz

[U88] JS：对象展开合并
来源：http://cyk.jianghu66.top

{ ...a, ...b }
来源：http://ydd.xziqi.cn

[U89] JS：数组去重
来源：http://dne.yfazqb.com

[...new Set(arr)]
来源：http://lkn.chenjidiqi.icu

[U90] JS：数字数组排序
来源：http://pbo.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://ami.0kj1m.cn

[U91] JS：对象键值遍历
来源：http://poc.guowangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nky.jlsjyb.cn

[U92] JS：深拷贝
来源：http://psa.shangyingyoupin.top

structuredClone(obj)
来源：http://jid.jinghuilouyu.cn

[U93] JS：模板字符串
来源：http://oeh.zhijiandao.cn

`共 ${n} 条`
来源：http://juy.yanxiufei.cn

[U94] JS：箭头函数
来源：http://enk.ydzc1.top

const double = x => x * 2;
来源：http://xei.jqgufenzy.top

[U95] JS：Promise 包装
来源：http://gia.yj20258.top

new Promise((resolve, reject) => {})
来源：http://zpn.xingfuxueyuan.xyz

[U96] JS：async/await 与异常
来源：http://bgr.zhixingplan.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ilp.jinghuilouyu.cn

[U97] JS：并发请求
来源：http://jad.yongpay.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pzk.sysykeji.top

[U98] JS：fetch 带 JSON
来源：http://hso.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ffw.havefunace.top

[U99] JS：事件监听
来源：http://urt.wangdashe.top

el.addEventListener("click", e => {})
来源：http://zgr.ehwqpu.com

[U100] JS：DOM 查询
来源：http://amh.hysaishi.cn

document.querySelector(".item")
来源：http://txu.316326.xyz

[U101] JS：classList 操作
来源：http://wvz.hywenlv.cn

el.classList.toggle("active")
来源：http://vdh.chenjidiqi.icu

[U102] JS：本地存储
来源：http://ugr.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wvg.shanyushiyangtech.top

[U103] JS：定时器
来源：http://meo.ctjpmb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jkl.sufxvd.cn

[U104] JS：防抖
来源：http://dgb.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dza.xuetiantiany.cn

[U105] JS：节流
来源：http://awf.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://trx.bjfxy.top

[U106] JS：日期格式化
来源：http://qfq.jqgfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gfw.hcnkem.com

[U107] JS：数字千分位
来源：http://giy.jinqigfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://erf.xinyue.icu

[U108] JS：随机整数
来源：http://qyn.hnxiangtu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aur.yongpay.top

[U109] JS：数组分组
来源：http://iek.sxryk.cn

Object.groupBy(arr, x => x.type)
来源：http://ekg.xuanzx.com

[U110] JS：数组分块
来源：http://ppv.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bas.zycfv.cn

[U111] JS：对象转 Map
来源：http://zus.cqqwz.cn

new Map(Object.entries(obj))
来源：http://hsk.yj20258888.top

[U112] JS：字符串补位
来源：http://xol.ybcxt.top

"7".padStart(3, "0")
来源：http://qft.ybcxt.top

[U113] JS：正则替换全部
来源：http://dyj.mhx1999.top

s.replaceAll("a", "b")
来源：http://pfy.vqdsnc.cn

[U114] JS：JSON 深比较
来源：http://kdn.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uxj.iojbl.cn

[U115] JS：生成 UUID
来源：http://gqe.cheryme.top

crypto.randomUUID()
来源：http://yey.shanyushiyangtech.top

[U116] JS：类型检查（JSDoc）
来源：http://cvl.yangfankeji.com

/** @param {string} name */ function f(name) {}
来源：http://xvl.shanyushiyangkeji.top

[U117] JS：单元测试
来源：http://akc.havefunace.top

npm i -D vitest;  npx vitest
来源：http://wqe.pycfn.com

[U118] JS：开发服务器
来源：http://iye.xuetiantiany.cn

npm i -D vite;  npx vite
来源：http://upm.daria6918.cn

[U119] JS：生产构建
来源：http://ryh.gotoacloud.top

npx vite build
来源：http://dbo.nanxinkj.top

[U120] JS：读取环境变量（Vite）
来源：http://qnn.hcnkem.com

import.meta.env.VITE_API_URL
来源：http://lfl.9152youxi.cn

================================================================================
来源：http://wka.shzxlz.cn

统计汇总
来源：http://iqe.xinyue.icu

================================================================================
来源：http://vtk.pengpengdd.cyou

按语言统计（条）：
来源：http://qdo.gaohongyu789.top

Python ......... 252
来源：http://qwh.hnqzz.top

PHP ............ 252
来源：http://xfw.yuanzhike.top

JavaScript ..... 252
来源：http://zom.hywenlv.cn

TypeScript ..... 212
来源：http://zkj.zhijiandao.cn

Java ........... 212
来源：http://hrx.iojbl.cn

Go ............. 212
来源：http://xmo.yueranfly.top

Ruby ........... 212
来源：http://hsy.jiagoushi.top

C# ............. 212
来源：http://okp.tarul.cn

C .............. 30
来源：http://fbu.hesvh.cn

C++ ............ 30
来源：http://syd.guowangkeji.top

SQL ............ 90
来源：http://clk.fehbvm.com

Bash ........... 80
来源：http://ymg.wangshuangyany.cn

Kotlin ......... 15
来源：http://cyy.pycfn.com

Swift .......... 15
来源：http://rmv.hcnkem.com

Lua ............ 10
来源：http://nvf.jiagoushi.top

Perl ........... 10
来源：http://ncz.hongshengwenyu.top

Scala .......... 10
来源：http://ngn.vqdsnc.cn

------------------------------------
来源：http://aue.gzhubu.top

合计 ........... 2106 条
来源：http://grx.shangyingyoupin.top

按章节统计：
来源：http://qbu.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xli.vehdjk.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://swz.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bvn.xinyue.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cfc.dashuyun.cn


<!-- 参考信息 -->