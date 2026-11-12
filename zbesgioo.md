代发 wailian999

[T47] Perl：正则捕获
来源：http://wfh.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ome.jinqigfzy.top

[T48] Perl：正则替换
来源：http://sav.fehbvm.com

$s =~ s/old/new/g;
来源：http://gyt.hnxiangtu.top

[T49] Perl：函数
来源：http://kgl.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kfv.xziqi.cn

[T50] Perl：逐行读文件
来源：http://fog.wangshuangyany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wyo.dianchejie.cn

while (my $line = <$fh>) { print $line; }
来源：http://ikw.jyoumei.cn

[T51] Scala：Hello World
来源：http://trg.fzhhl.top

println("Hello")
来源：http://ysg.dashuyun.cn

[T52] Scala：变量
来源：http://cqy.hnxiangtu.top

val a = 1;  var b = 2
来源：http://jvl.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://ywd.ctjpmb.com

s"值: $b"
来源：http://mci.tianlin.xyz

[T54] Scala：集合映射
来源：http://wgh.dashuyun.cn

List(1, 2, 3).map(_ * 2)
来源：http://owl.kuanghao11.cn

[T55] Scala：集合过滤
来源：http://pcz.chenlongwang.top

List(1, 2, 3).filter(_ > 1)
来源：http://hqk.dashuyun.cn

[T56] Scala：样例类
来源：http://itn.sweek.top

case class User(name: String, age: Int)
来源：http://lka.vqdsnc.cn

[T57] Scala：模式匹配
来源：http://smc.52xcode.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dib.ppjwa.cn

[T58] Scala：函数定义
来源：http://ctr.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://frx.ehwqpu.com

[T59] Scala：循环
来源：http://yvr.cqqwz.cn

for (i <- 1 to 10) println(i)
来源：http://use.tanke756.top

[T60] Scala：折叠
来源：http://tlh.hongshengwenyu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tbo.iojbl.cn

================================================================================
来源：http://yol.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lro.ppjwa.cn

================================================================================
来源：http://lcr.nanxuanxn.top

[U01] Py：创建虚拟环境
来源：http://axz.shanyushiyangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://ktk.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://eds.meibo888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fxp.ivvv.top

[U03] Py：加载 .env 配置
来源：http://plt.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hnw.pengpengdd.cyou

[U04] Py：变量调试打印
来源：http://eox.zhiwuduotai.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://taw.zhaomingkeji.xyz

[U05] Py：列表去重且保序
来源：http://qfo.dashuyun.cn

list(dict.fromkeys(arr))
来源：http://nmk.daria6918.cn

[U06] Py：合并两个字典
来源：http://unc.epnwcf.com

{**a, **b}
来源：http://xgx.mhx1999.top

[U07] Py：反转字典键值
来源：http://jue.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://olb.chenzaomai.com

[U08] Py：展平二维列表
来源：http://hjc.jqgfzy.top

[y for x in nested for y in x]
来源：http://qic.tian-w.cn

[U09] Py：字典取最大值的键
来源：http://voq.svipenyu.cn

max(d, key=d.get)
来源：http://cno.wangdashe.top

[U10] Py：按值排序字典
来源：http://rov.316326.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qjw.yanxiufei.cn

[U11] Py：生成器表达式
来源：http://cge.epnwcf.com

(x * 2 for x in arr)
来源：http://une.zhongyouzk.top

[U12] Py：取出现最多的 3 个元素
来源：http://gyk.316326.xyz

Counter(arr).most_common(3)
来源：http://pru.snrcjt.cn

[U13] Py：固定长度队列
来源：http://jwb.jinqigufen.top

deque(maxlen=10)
来源：http://irw.zhongyouzk.top

[U14] Py：分组收集到列表
来源：http://krl.chenzaomai.com

defaultdict(list)
来源：http://jyv.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://soc.zhoulong.xyz

t = time.perf_counter()
来源：http://dbh.hongshengwenyu.top

[U16] Py：命令行参数解析
来源：http://wmz.0kj1m.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xpi.c1oappe.top

[U17] Py：初始化日志
来源：http://vty.yj202588.top

logging.basicConfig(level=logging.INFO)
来源：http://hce.gotoacloud.top

[U18] Py：预编译正则
来源：http://mov.9152youxi.cn

pat = re.compile(r"\d+")
来源：http://ole.9152youxi.cn

[U19] Py：正则替换带回调
来源：http://vts.xziqi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ral.gzhubu.top

[U20] Py：缓存函数结果
来源：http://fnw.yonumen.top

@functools.lru_cache(maxsize=None)
来源：http://duv.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://blu.chenjidiqi.icu

@contextlib.contextmanager
来源：http://fcg.hongshengwenyu.top

[U22] Py：矩阵转置
来源：http://dig.havefunace.top

list(zip(*m))
来源：http://ngk.ybcxt.top

[U23] Py：分块读取大文件
来源：http://pai.zhijiandao.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yfm.wangdashe.top

[U24] Py：路径操作
来源：http://zwp.ivvv.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tel.sjlbkw.cn

[U25] Py：CSV 按字典读
来源：http://iiq.sxryk.cn

csv.DictReader(f)
来源：http://ose.yj20258888.top

[U26] Py：并发下载
来源：http://bgw.jianghu66.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yhf.yanxiufei.cn

[U27] Py：异步 HTTP
来源：http://kmr.tanke756.top

aiohttp.ClientSession() 配合 async with
来源：http://xqb.snrcjt.cn

[U28] Py：类型别名
来源：http://qdp.bjfxy.top

UserId = int
来源：http://bbj.feifeiyinyue.top

[U29] Py：属性校验
来源：http://znp.yuxming.cn

@property 与 @x.setter 配合
来源：http://vnh.zdbjq.cn

[U30] Py：数据类
来源：http://rna.epnwcf.com

@dataclass(slots=True)
来源：http://ecq.guowangkeji.top

[U31] Py：单测
来源：http://uqz.wangdashe.top

python -m pytest -q
来源：http://vho.sufxvd.cn

[U32] Py：代码格式化
来源：http://jjv.haohaochexian.top

ruff format . && ruff check --fix .
来源：http://cos.hesvh.cn

[U33] Py：打包发布
来源：http://bxg.svipenyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://rix.cqqwz.cn

[U34] Py：判断编码
来源：http://frp.52xcode.cn

chardet.detect(raw)
来源：http://jfw.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://sni.zhaomingkeji.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ehl.ehwqpu.com

[U36] Py：定时任务
来源：http://mcr.zhengqikj.top

schedule.every(10).minutes.do(job)
来源：http://wbq.tian-w.cn

[U37] Py：读写 Excel
来源：http://poa.zhiwuduotai.top

pandas.read_excel / DataFrame.to_excel
来源：http://bzo.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://jiz.c1oappe.top

Path(__file__).resolve().parent
来源：http://mqh.jqgufenzy.top

[U39] Py：判断是否在交互环境
来源：http://bdn.zhongyouzk.top

sys.stdout.isatty()
来源：http://sbb.smart0.xyz

[U40] Py：打印到标准错误
来源：http://lui.fanxiaobao.xyz

print("err", file=sys.stderr)
来源：http://osz.uphjek.com

[U41] PHP：初始化 Composer 项目
来源：http://izp.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://hzv.gotoacloud.top

[U42] PHP：PSR-4 自动加载
来源：http://kla.hcnkem.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bqt.chenjidiqi.icu

[U43] PHP：声明命名空间
来源：http://ccu.haohaochexian.top

namespace App\Http;
来源：http://wgb.52xcode.cn

[U44] PHP：开启严格类型
来源：http://svt.gotoacloud.top

declare(strict_types=1);
来源：http://qeb.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://zjz.zhixingplan.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://dqy.hnqzz.top

[U46] PHP：可空类型
来源：http://buc.havefunace.top

?string $name = null
来源：http://lre.ppjwa.cn

[U47] PHP：联合类型
来源：http://vot.0kj1m.cn

int|string $id
来源：http://mzx.9152youxi.cn

[U48] PHP：纯枚举
来源：http://cgn.zhijiandao.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uys.jiagoushi.top

[U49] PHP：只读属性
来源：http://aoj.jiagoushi.top

public readonly string $name
来源：http://het.ywan-chungtsiang.top

[U50] PHP：构造器属性提升
来源：http://wsm.bbcook.cn

public function __construct(private int $id) {}
来源：http://vso.sjlbkw.cn

[U51] PHP：数组解构
来源：http://ycx.ydzc1.top

[$a, $b] = $arr;
来源：http://zsy.hnqzz.top

[U52] PHP：箭头函数
来源：http://bmm.pengpengdd.cyou

$double = fn($x) => $x * 2;
来源：http://pfy.sxryk.cn

[U53] PHP：空合并运算符
来源：http://fsx.ivvv.top

$v = $a ?? $b ?? "default";
来源：http://qin.xuanzx.com

[U54] PHP：空安全调用
来源：http://adw.chenzaomai.com

$obj?->method()
来源：http://lpi.fehbvm.com

[U55] PHP：match 表达式
来源：http://zdp.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vtn.yuxming.cn

[U56] PHP：命名参数
来源：http://rzn.yj20258.top

f(a: 1, b: 2)
来源：http://pxw.fehbvm.com

[U57] PHP：字符串插值
来源：http://kci.fanxiaobao.xyz

"值: {$a}"
来源：http://dgr.zhiwuduotai.top

[U58] PHP：数组三件套
来源：http://cgu.tianlin.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nuu.ehwqpu.com

[U59] PHP：自定义排序
来源：http://xyk.hnqzz.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wax.wangdashe.top

[U60] PHP：JSON 编解码
来源：http://vkx.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tkk.chenzaomai.com

[U61] PHP：正则
来源：http://mji.316326.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cvf.tanke756.top

[U62] PHP：日期对象
来源：http://rpn.yangfankeji.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dan.epnwcf.com

[U63] PHP：文件读写
来源：http://gag.cheryme.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rve.zhaomingkeji.xyz

[U64] PHP：目录遍历
来源：http://lrq.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://sdn.hywenlv.cn

[U65] PHP：会话
来源：http://bgz.vqdsnc.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ntf.aibaodan.cn

[U66] PHP：设置 Cookie
来源：http://xjs.cucudq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xdt.cucudq.cn

[U67] PHP：处理文件上传
来源：http://nuo.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fbz.tian-w.cn

[U68] PHP：PDO 连接
来源：http://gbl.tianlin.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hbd.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://zoa.cucudq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tgt.yuxming.cn

[U70] PHP：PDO 事务
来源：http://iho.pycfn.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bwp.ywan-chungtsiang.top

[U71] PHP：抛出异常
来源：http://kat.zhijiandao.cn

throw new RuntimeException("失败", 500);
来源：http://kjv.fktsv.cn

[U72] PHP：写错误日志
来源：http://yfd.yuanzhike.top

error_log("失败: " . $e->getMessage());
来源：http://urt.fzhhl.top

[U73] PHP：读取 ini 配置
来源：http://ccb.zhengqikj.top

parse_ini_file("config.ini", true)
来源：http://mck.kuanghao11.cn

[U74] PHP：读取环境变量
来源：http://nzw.yanxiufei.cn

getenv("APP_ENV") ?: "production"
来源：http://ctn.kuanghao11.cn

[U75] PHP：依赖注入
来源：http://qby.jinyuanbaomall.cn

composer require psr/container
来源：http://sew.sweek.top

[U76] PHP：简单路由
来源：http://qhb.sxryk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kvh.shzxlz.cn

[U77] PHP：模板渲染
来源：http://mps.shanyushiyangkeji.top

composer require twig/twig
来源：http://hjx.zhiwuduotai.top

[U78] PHP：单元测试
来源：http://sgw.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://svf.quarkkingdee.top

[U79] PHP：静态分析
来源：http://gjy.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://yiu.c1oappe.top

[U80] PHP：代码规范修复
来源：http://vpi.xylfe.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pyd.gotoacloud.top

[U81] JS：初始化项目
来源：http://orz.aizwys.cn

npm init -y;  npm i express
来源：http://wck.fzhhl.top

[U82] JS：package.json 脚本
来源：http://zqj.hfpthk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cjv.ehwqpu.com

[U83] JS：ES Module 导入导出
来源：http://yql.sxryk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://keu.zdqjudy.top

[U84] JS：CommonJS 写法
来源：http://zup.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nqe.feifeiyinyue.top

[U85] JS：可选链
来源：http://eyp.tianlin.xyz

a?.b?.c
来源：http://djj.xuanzx.com

[U86] JS：空值合并
来源：http://qwf.ywan-chungtsiang.top

a ?? b
来源：http://jxs.jinyuanbaomall.cn

[U87] JS：解构默认值
来源：http://eld.xziqi.cn

const { a = 1, b = 2 } = obj;
来源：http://ifz.ctjpmb.com

[U88] JS：对象展开合并
来源：http://wca.hnqzz.top

{ ...a, ...b }
来源：http://itk.aizwys.cn

[U89] JS：数组去重
来源：http://fla.shanyushiyangtech.top

[...new Set(arr)]
来源：http://spu.bjfxy.top

[U90] JS：数字数组排序
来源：http://iok.zhijiandao.cn

[...arr].sort((a, b) => a - b)
来源：http://uij.yangfankeji.com

[U91] JS：对象键值遍历
来源：http://hni.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://huv.vqdsnc.cn

[U92] JS：深拷贝
来源：http://cyx.bjfxy.top

structuredClone(obj)
来源：http://ydv.zhijiandao.cn

[U93] JS：模板字符串
来源：http://lzi.epnwcf.com

`共 ${n} 条`
来源：http://cii.fzhhl.top

[U94] JS：箭头函数
来源：http://hct.xinyue.icu

const double = x => x * 2;
来源：http://lvz.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://jfx.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://hdx.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://cpx.ehwqpu.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://znl.bjfxy.top

[U97] JS：并发请求
来源：http://dqk.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fgp.zycfv.cn

[U98] JS：fetch 带 JSON
来源：http://kab.yanxiufei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kht.yuxming.cn

[U99] JS：事件监听
来源：http://miv.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://qmc.ehwqpu.com

[U100] JS：DOM 查询
来源：http://kht.zycfv.cn

document.querySelector(".item")
来源：http://rjx.guannengcc.top

[U101] JS：classList 操作
来源：http://tnm.yj202588.top

el.classList.toggle("active")
来源：http://plh.tarul.cn

[U102] JS：本地存储
来源：http://igg.shangyingyoupin.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://niu.yuanzhike.top

[U103] JS：定时器
来源：http://qye.meibo888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yvu.9152youxi.cn

[U104] JS：防抖
来源：http://ijr.tian-w.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wfz.shanyushiyangkeji.top

[U105] JS：节流
来源：http://nub.havefunace.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ecd.fanxiaobao.xyz

[U106] JS：日期格式化
来源：http://cjq.xuanzx.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://atn.yuanzhike.top

[U107] JS：数字千分位
来源：http://zbw.jinqigfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fil.sysykeji.top

[U108] JS：随机整数
来源：http://wts.feifeiyinyue.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qmw.tarul.cn

[U109] JS：数组分组
来源：http://alq.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://our.sjlbkw.cn

[U110] JS：数组分块
来源：http://pro.aizwys.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vsz.fktsv.cn

[U111] JS：对象转 Map
来源：http://bms.jinghuilouyu.cn

new Map(Object.entries(obj))
来源：http://zac.nanxinkj.top

[U112] JS：字符串补位
来源：http://isj.jiagoushi.top

"7".padStart(3, "0")
来源：http://ebd.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://oom.sysykeji.top

s.replaceAll("a", "b")
来源：http://ipz.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://xfg.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rez.cheryme.top

[U115] JS：生成 UUID
来源：http://pdo.uphjek.com

crypto.randomUUID()
来源：http://uno.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://slk.bbcook.cn

/** @param {string} name */ function f(name) {}
来源：http://tlg.zhiwuduotai.top

[U117] JS：单元测试
来源：http://ith.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://ejs.xingfuxueyuan.xyz

[U118] JS：开发服务器
来源：http://aqo.ctjpmb.com

npm i -D vite;  npx vite
来源：http://cot.yanxiufei.cn

[U119] JS：生产构建
来源：http://ofh.hnqzz.top

npx vite build
来源：http://uxb.vehdjk.com

[U120] JS：读取环境变量（Vite）
来源：http://iro.vehdjk.com

import.meta.env.VITE_API_URL
来源：http://yfz.shanyushiyangtech.top

================================================================================
来源：http://kzd.zdqjudy.top

统计汇总
来源：http://jpu.hongshengwenyu.top

================================================================================
来源：http://zcs.mhx1999.top

按语言统计（条）：
来源：http://yiv.yueranfly.top

Python ......... 252
来源：http://pvg.yangfankeji.com

PHP ............ 252
来源：http://hhq.yvedp.cn

JavaScript ..... 252
来源：http://mkk.shuidangran.top

TypeScript ..... 212
来源：http://puf.pycfn.com

Java ........... 212
来源：http://rwx.0kj1m.cn

Go ............. 212
来源：http://wrr.zhongyouzk.top

Ruby ........... 212
来源：http://ybd.bbcook.cn

C# ............. 212
来源：http://hmg.vehdjk.com

C .............. 30
来源：http://qyx.zhixingplan.top

C++ ............ 30
来源：http://pew.shzxlz.cn

SQL ............ 90
来源：http://ijk.guowangkeji.top

Bash ........... 80
来源：http://kqb.ydjk.org.cn

Kotlin ......... 15
来源：http://vfb.yj202588.top

Swift .......... 15
来源：http://qja.dianchejie.cn

Lua ............ 10
来源：http://iew.sweek.top

Perl ........... 10
来源：http://jbh.bbcook.cn

Scala .......... 10
来源：http://ijh.kuanghao11.cn

------------------------------------
来源：http://idr.pycfn.com

合计 ........... 2106 条
来源：http://dhi.hysaishi.cn

按章节统计：
来源：http://dcn.ybcxt.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wvx.yangfankeji.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jwx.sjlbkw.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xea.mhx1999.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lsl.guannengcc.top


<!-- 参考信息 -->