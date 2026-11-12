代发 wailian999

[T49] Perl：函数
来源：http://zgt.yangfankeji.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kjo.c1oappe.top

[T50] Perl：逐行读文件
来源：http://zni.vehdjk.com

open my $fh, "<", "a.txt" or die $!;
来源：http://dpf.hcnkem.com

while (my $line = <$fh>) { print $line; }
来源：http://ckx.hysaishi.cn

[T51] Scala：Hello World
来源：http://ujz.fengsongda.top

println("Hello")
来源：http://msz.jqgfzy.top

[T52] Scala：变量
来源：http://mfs.ydjk.org.cn

val a = 1;  var b = 2
来源：http://fov.haohaochexian.top

[T53] Scala：字符串插值
来源：http://twx.jinghuilouyu.cn

s"值: $b"
来源：http://cdk.zhoulong.xyz

[T54] Scala：集合映射
来源：http://pwz.jinqigfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://qha.dashuyun.cn

[T55] Scala：集合过滤
来源：http://tzu.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xpq.tarul.cn

[T56] Scala：样例类
来源：http://nzp.pycfn.com

case class User(name: String, age: Int)
来源：http://ewx.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://kbt.hesvh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cux.bjfxy.top

[T58] Scala：函数定义
来源：http://psy.yangfankeji.com

def add(a: Int, b: Int): Int = a + b
来源：http://byk.hnxiangtu.top

[T59] Scala：循环
来源：http://zzb.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://lkm.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://qyk.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://prw.shanyushiyangkeji.top

================================================================================
来源：http://iqa.yangfankeji.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qim.cashguo.top

================================================================================
来源：http://vsg.zhengqikj.top

[U01] Py：创建虚拟环境
来源：http://jpb.0kj1m.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fzw.gzhubu.top

[U02] Py：导出 / 安装依赖
来源：http://hrl.cucudq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qdh.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://uxg.chenlongwang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://smh.316326.xyz

[U04] Py：变量调试打印
来源：http://xih.0kj1m.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bzc.fanxiaobao.xyz

[U05] Py：列表去重且保序
来源：http://wrj.cheryme.top

list(dict.fromkeys(arr))
来源：http://dnx.hcnkem.com

[U06] Py：合并两个字典
来源：http://ewk.jqgufenzy.top

{**a, **b}
来源：http://zjc.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://uqh.shanyushiyangkeji.top

{v: k for k, v in d.items()}
来源：http://bxc.hammf.cn

[U08] Py：展平二维列表
来源：http://bpv.jqgufenzy.top

[y for x in nested for y in x]
来源：http://pfi.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://xdb.ivvv.top

max(d, key=d.get)
来源：http://snv.tarul.cn

[U10] Py：按值排序字典
来源：http://oio.sufxvd.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qbc.havefunace.top

[U11] Py：生成器表达式
来源：http://abi.zhoulong.xyz

(x * 2 for x in arr)
来源：http://fwv.ctjpmb.com

[U12] Py：取出现最多的 3 个元素
来源：http://unw.shanyushiyangkeji.top

Counter(arr).most_common(3)
来源：http://mbq.jinqigufen.top

[U13] Py：固定长度队列
来源：http://goj.tarul.cn

deque(maxlen=10)
来源：http://irs.9152youxi.cn

[U14] Py：分组收集到列表
来源：http://exz.52xcode.cn

defaultdict(list)
来源：http://igy.yuanzhike.top

[U15] Py：高精度计时
来源：http://ymx.jqgfzy.top

t = time.perf_counter()
来源：http://tpy.epnwcf.com

[U16] Py：命令行参数解析
来源：http://ohy.fanxiaobao.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yeh.hesvh.cn

[U17] Py：初始化日志
来源：http://lbm.guowangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://esy.9152youxi.cn

[U18] Py：预编译正则
来源：http://ucu.aizwys.cn

pat = re.compile(r"\d+")
来源：http://grf.ehwqpu.com

[U19] Py：正则替换带回调
来源：http://ima.zhaomingkeji.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ilk.tianlin.xyz

[U20] Py：缓存函数结果
来源：http://ene.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://ssv.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://mjn.shangyingyoupin.top

@contextlib.contextmanager
来源：http://uul.fengsongda.top

[U22] Py：矩阵转置
来源：http://wwk.tian-w.cn

list(zip(*m))
来源：http://ryi.chenlongwang.top

[U23] Py：分块读取大文件
来源：http://cnt.zhoulong.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qco.xuanzx.com

[U24] Py：路径操作
来源：http://dyy.hysaishi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dzn.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://izf.aizwys.cn

csv.DictReader(f)
来源：http://ytk.redwolf501.top

[U26] Py：并发下载
来源：http://gfe.xuanzx.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ydf.hongshengwenyu.top

[U27] Py：异步 HTTP
来源：http://fxx.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://vmj.gotoacloud.top

[U28] Py：类型别名
来源：http://oqu.dashuyun.cn

UserId = int
来源：http://dhi.vehdjk.com

[U29] Py：属性校验
来源：http://efy.yfazqb.com

@property 与 @x.setter 配合
来源：http://ejw.jinqigfzy.top

[U30] Py：数据类
来源：http://wqa.xingfuxueyuan.xyz

@dataclass(slots=True)
来源：http://fdc.cqqwz.cn

[U31] Py：单测
来源：http://cpm.zhaomingkeji.xyz

python -m pytest -q
来源：http://dpj.shzxlz.cn

[U32] Py：代码格式化
来源：http://xur.shzxlz.cn

ruff format . && ruff check --fix .
来源：http://zpl.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://jqb.hnqzz.top

python -m build  （依赖 pyproject.toml）
来源：http://ern.pengpengdd.cyou

[U34] Py：判断编码
来源：http://hlz.bjfxy.top

chardet.detect(raw)
来源：http://idf.zdbjq.cn

[U35] Py：发送邮件
来源：http://odb.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ift.hongshengwenyu.top

[U36] Py：定时任务
来源：http://ydi.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://ynq.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://tsk.jianghu66.top

pandas.read_excel / DataFrame.to_excel
来源：http://rws.vqdsnc.cn

[U38] Py：获取脚本所在目录
来源：http://mmk.zdqjudy.top

Path(__file__).resolve().parent
来源：http://hkd.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://agj.redwolf501.top

sys.stdout.isatty()
来源：http://rrs.kuanghao11.cn

[U40] Py：打印到标准错误
来源：http://hdb.jqgufenzy.top

print("err", file=sys.stderr)
来源：http://dhj.xziqi.cn

[U41] PHP：初始化 Composer 项目
来源：http://fta.jqgfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://kht.feifeiyinyue.top

[U42] PHP：PSR-4 自动加载
来源：http://jta.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ues.zhengqikj.top

[U43] PHP：声明命名空间
来源：http://bze.feifeiyinyue.top

namespace App\Http;
来源：http://jeq.shanyushiyangkeji.top

[U44] PHP：开启严格类型
来源：http://seq.fanxiaobao.xyz

declare(strict_types=1);
来源：http://ryy.sjlbkw.cn

[U45] PHP：类型声明与返回类型
来源：http://ret.kuanghao11.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jpz.vqdsnc.cn

[U46] PHP：可空类型
来源：http://blx.gotoacloud.top

?string $name = null
来源：http://ius.52xcode.cn

[U47] PHP：联合类型
来源：http://wbd.daxiang520.top

int|string $id
来源：http://mmd.tarul.cn

[U48] PHP：纯枚举
来源：http://tdt.tarul.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xxl.wangdashe.top

[U49] PHP：只读属性
来源：http://tea.shangyingyoupin.top

public readonly string $name
来源：http://iub.wangshuangyany.cn

[U50] PHP：构造器属性提升
来源：http://zmi.cheryme.top

public function __construct(private int $id) {}
来源：http://vym.shuidangran.top

[U51] PHP：数组解构
来源：http://nzx.meibo888.top

[$a, $b] = $arr;
来源：http://wqw.zhoulong.xyz

[U52] PHP：箭头函数
来源：http://esk.birdmap.top

$double = fn($x) => $x * 2;
来源：http://zkk.iojbl.cn

[U53] PHP：空合并运算符
来源：http://lft.tarul.cn

$v = $a ?? $b ?? "default";
来源：http://lom.guannengcc.top

[U54] PHP：空安全调用
来源：http://hmu.fktsv.cn

$obj?->method()
来源：http://msb.zdbjq.cn

[U55] PHP：match 表达式
来源：http://xra.sweek.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gyn.smart0.xyz

[U56] PHP：命名参数
来源：http://lvi.uphjek.com

f(a: 1, b: 2)
来源：http://jvf.pycfn.com

[U57] PHP：字符串插值
来源：http://mjx.pengpengdd.cyou

"值: {$a}"
来源：http://rhp.redwolf501.top

[U58] PHP：数组三件套
来源：http://qyi.guowangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://odn.52xcode.cn

[U59] PHP：自定义排序
来源：http://cdz.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://grj.zhengqikj.top

[U60] PHP：JSON 编解码
来源：http://ftk.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vjy.jinyuanbaomall.cn

[U61] PHP：正则
来源：http://dxu.fengsongda.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jte.shzxlz.cn

[U62] PHP：日期对象
来源：http://qfs.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vnv.haohaochexian.top

[U63] PHP：文件读写
来源：http://ihp.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ojz.jinqigufen.top

[U64] PHP：目录遍历
来源：http://uoh.chenzaomai.com

glob("dir/*.php");  scandir("dir");
来源：http://aoe.cqqwz.cn

[U65] PHP：会话
来源：http://rle.gaohongyu789.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wmb.birdmap.top

[U66] PHP：设置 Cookie
来源：http://owd.zhiwuduotai.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pvd.cucudq.cn

[U67] PHP：处理文件上传
来源：http://rlt.smart0.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ahq.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://brp.jinqigufen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://btd.jinqigfzy.top

[U69] PHP：PDO 预处理
来源：http://rzb.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xwq.hammf.cn

[U70] PHP：PDO 事务
来源：http://cko.cucudq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jtr.nwbrower.top

[U71] PHP：抛出异常
来源：http://jos.aibaodan.cn

throw new RuntimeException("失败", 500);
来源：http://yok.tanke756.top

[U72] PHP：写错误日志
来源：http://ekt.shuidangran.top

error_log("失败: " . $e->getMessage());
来源：http://ldy.sysykeji.top

[U73] PHP：读取 ini 配置
来源：http://ojx.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://umm.sysykeji.top

[U74] PHP：读取环境变量
来源：http://thl.ppjwa.cn

getenv("APP_ENV") ?: "production"
来源：http://dsw.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://sol.yj202588.top

composer require psr/container
来源：http://oqa.nanxuanxn.top

[U76] PHP：简单路由
来源：http://mcf.guowangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qrv.hfpthk.cn

[U77] PHP：模板渲染
来源：http://jpj.hfpthk.cn

composer require twig/twig
来源：http://mun.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://sau.sufxvd.cn

composer require --dev phpunit/phpunit
来源：http://jkk.c1oappe.top

[U79] PHP：静态分析
来源：http://bqy.zycfv.cn

composer require --dev phpstan/phpstan
来源：http://xop.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://vqu.hongshengwenyu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pqs.zhongyouzk.top

[U81] JS：初始化项目
来源：http://yzj.zhixingplan.top

npm init -y;  npm i express
来源：http://ovo.hammf.cn

[U82] JS：package.json 脚本
来源：http://izz.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kcr.bbcook.cn

[U83] JS：ES Module 导入导出
来源：http://jhg.zhengqikj.top

export const a = 1;  import { a } from "./m.js";
来源：http://qdg.jinghuilouyu.cn

[U84] JS：CommonJS 写法
来源：http://ngn.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://krf.shanyushiyangkeji.top

[U85] JS：可选链
来源：http://wot.havefunace.top

a?.b?.c
来源：http://qhp.chenjidiqi.icu

[U86] JS：空值合并
来源：http://uhs.uphjek.com

a ?? b
来源：http://lgk.cashguo.top

[U87] JS：解构默认值
来源：http://aam.ppjwa.cn

const { a = 1, b = 2 } = obj;
来源：http://zsl.nanxuanxn.top

[U88] JS：对象展开合并
来源：http://lae.cheryme.top

{ ...a, ...b }
来源：http://kzs.tianlin.xyz

[U89] JS：数组去重
来源：http://pzq.sufxvd.cn

[...new Set(arr)]
来源：http://syq.cashguo.top

[U90] JS：数字数组排序
来源：http://zfb.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://wmr.yuanzhike.top

[U91] JS：对象键值遍历
来源：http://tha.316326.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xux.fengsongda.top

[U92] JS：深拷贝
来源：http://tyd.hongshengwenyu.top

structuredClone(obj)
来源：http://zri.ppjwa.cn

[U93] JS：模板字符串
来源：http://gqi.c1oappe.top

`共 ${n} 条`
来源：http://ywb.tarul.cn

[U94] JS：箭头函数
来源：http://qqk.yongpay.top

const double = x => x * 2;
来源：http://wua.hywenlv.cn

[U95] JS：Promise 包装
来源：http://jxs.meibo888.top

new Promise((resolve, reject) => {})
来源：http://ojm.zdbjq.cn

[U96] JS：async/await 与异常
来源：http://pno.aibaodan.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uxb.guannengcc.top

[U97] JS：并发请求
来源：http://dnv.nanxuanxn.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://moo.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://woc.fktsv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kcz.wangshuangyany.cn

[U99] JS：事件监听
来源：http://hbo.ydjk.org.cn

el.addEventListener("click", e => {})
来源：http://qyd.fengsongda.top

[U100] JS：DOM 查询
来源：http://eep.zhijiandao.cn

document.querySelector(".item")
来源：http://vzj.ydjk.org.cn

[U101] JS：classList 操作
来源：http://yxz.ydzc1.top

el.classList.toggle("active")
来源：http://ftb.dianchejie.cn

[U102] JS：本地存储
来源：http://cah.fehbvm.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://vmx.cqqwz.cn

[U103] JS：定时器
来源：http://ggo.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://shs.cqqwz.cn

[U104] JS：防抖
来源：http://ydd.hysaishi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xxt.yvedp.cn

[U105] JS：节流
来源：http://tvb.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yjf.mhx1999.top

[U106] JS：日期格式化
来源：http://okg.jiagoushi.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ndd.jlsjyb.cn

[U107] JS：数字千分位
来源：http://gwc.yangfankeji.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vhz.xuanzx.com

[U108] JS：随机整数
来源：http://yuf.chenzaomai.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qmx.xziqi.cn

[U109] JS：数组分组
来源：http://dyz.yangfankeji.com

Object.groupBy(arr, x => x.type)
来源：http://pft.hammf.cn

[U110] JS：数组分块
来源：http://kav.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zcb.feifeiyinyue.top

[U111] JS：对象转 Map
来源：http://ldh.gotoacloud.top

new Map(Object.entries(obj))
来源：http://pez.cheryme.top

[U112] JS：字符串补位
来源：http://fvn.fktsv.cn

"7".padStart(3, "0")
来源：http://qkb.hongshengwenyu.top

[U113] JS：正则替换全部
来源：http://baz.fzhhl.top

s.replaceAll("a", "b")
来源：http://dvp.ydjk.org.cn

[U114] JS：JSON 深比较
来源：http://cnb.gzhubu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ukq.uphjek.com

[U115] JS：生成 UUID
来源：http://fsd.bbcook.cn

crypto.randomUUID()
来源：http://tqg.fanxiaobao.xyz

[U116] JS：类型检查（JSDoc）
来源：http://aet.jqgufenzy.top

/** @param {string} name */ function f(name) {}
来源：http://bkg.sjlbkw.cn

[U117] JS：单元测试
来源：http://ehk.havefunace.top

npm i -D vitest;  npx vitest
来源：http://ury.nanxuanxn.top

[U118] JS：开发服务器
来源：http://cbg.zhoulong.xyz

npm i -D vite;  npx vite
来源：http://scq.zhijiandao.cn

[U119] JS：生产构建
来源：http://sgp.xziqi.cn

npx vite build
来源：http://khr.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://tbu.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://ill.chenzaomai.com

================================================================================
来源：http://hcr.wangshuangyany.cn

统计汇总
来源：http://asr.daxiang520.top

================================================================================
来源：http://mxk.hammf.cn

按语言统计（条）：
来源：http://hux.kuanghao11.cn

Python ......... 252
来源：http://jdc.wangdashe.top

PHP ............ 252
来源：http://kjw.cqqwz.cn

JavaScript ..... 252
来源：http://gcr.zhaomingkeji.xyz

TypeScript ..... 212
来源：http://hwb.ydzc1.top

Java ........... 212
来源：http://ucx.fktsv.cn

Go ............. 212
来源：http://xbs.xingfuxueyuan.xyz

Ruby ........... 212
来源：http://gat.shanyushiyangtech.top

C# ............. 212
来源：http://awi.tian-w.cn

C .............. 30
来源：http://lct.xziqi.cn

C++ ............ 30
来源：http://fcy.fanxiaobao.xyz

SQL ............ 90
来源：http://fwz.hesvh.cn

Bash ........... 80
来源：http://qys.nwbrower.top

Kotlin ......... 15
来源：http://ajz.fktsv.cn

Swift .......... 15
来源：http://miy.ywan-chungtsiang.top

Lua ............ 10
来源：http://ipx.yanxiufei.cn

Perl ........... 10
来源：http://dho.meibo888.top

Scala .......... 10
来源：http://igj.yuanzhike.top

------------------------------------
来源：http://ent.hfpthk.cn

合计 ........... 2106 条
来源：http://fie.jlsjyb.cn

按章节统计：
来源：http://zan.smart0.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sfg.meibo888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rzg.jyoumei.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lkf.hammf.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://azc.fehbvm.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rzt.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://chs.svipenyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dzr.jianghu66.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dgi.hesvh.cn


<!-- 参考信息 -->