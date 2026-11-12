代发 wailian999

[T49] Perl：函数
来源：http://vcg.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://brh.sweek.top

[T50] Perl：逐行读文件
来源：http://vyz.ppjwa.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://eyi.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://bqo.xziqi.cn

[T51] Scala：Hello World
来源：http://cbg.svipenyu.cn

println("Hello")
来源：http://edo.ybcxt.top

[T52] Scala：变量
来源：http://oce.jqgfzy.top

val a = 1;  var b = 2
来源：http://nkm.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://ozt.ydjk.org.cn

s"值: $b"
来源：http://iiw.shangyingyoupin.top

[T54] Scala：集合映射
来源：http://kwx.gogol.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://yrx.bjfxy.top

[T55] Scala：集合过滤
来源：http://rkq.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qxx.vehdjk.com

[T56] Scala：样例类
来源：http://qhi.316326.xyz

case class User(name: String, age: Int)
来源：http://sfg.snrcjt.cn

[T57] Scala：模式匹配
来源：http://hpz.pycfn.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://pii.yueranfly.top

[T58] Scala：函数定义
来源：http://qzh.nanxuanxn.top

def add(a: Int, b: Int): Int = a + b
来源：http://fhy.shuidangran.top

[T59] Scala：循环
来源：http://swn.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://cuw.hcnkem.com

[T60] Scala：折叠
来源：http://pjb.jinqigufen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gsc.ywan-chungtsiang.top

================================================================================
来源：http://uxq.zdqjudy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zms.snrcjt.cn

================================================================================
来源：http://wys.daria6918.cn

[U01] Py：创建虚拟环境
来源：http://ygi.yuxming.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qck.vehdjk.com

[U02] Py：导出 / 安装依赖
来源：http://ape.hnqzz.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xqp.tanke756.top

[U03] Py：加载 .env 配置
来源：http://dpk.ywan-chungtsiang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xha.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://arb.fehbvm.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ivb.yonumen.top

[U05] Py：列表去重且保序
来源：http://qpe.aizwys.cn

list(dict.fromkeys(arr))
来源：http://czh.wangshuangyany.cn

[U06] Py：合并两个字典
来源：http://akm.daria6918.cn

{**a, **b}
来源：http://tyu.aibaodan.cn

[U07] Py：反转字典键值
来源：http://csa.yonumen.top

{v: k for k, v in d.items()}
来源：http://vgc.hfpthk.cn

[U08] Py：展平二维列表
来源：http://vwx.wangdashe.top

[y for x in nested for y in x]
来源：http://lgb.svipenyu.cn

[U09] Py：字典取最大值的键
来源：http://uzq.gotoacloud.top

max(d, key=d.get)
来源：http://rtd.xingfuxueyuan.xyz

[U10] Py：按值排序字典
来源：http://vbk.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://azk.yueranfly.top

[U11] Py：生成器表达式
来源：http://ayx.cqqwz.cn

(x * 2 for x in arr)
来源：http://gek.fanxiaobao.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://jcm.cashguo.top

Counter(arr).most_common(3)
来源：http://qun.fanxiaobao.xyz

[U13] Py：固定长度队列
来源：http://kcj.hywenlv.cn

deque(maxlen=10)
来源：http://spg.mhx1999.top

[U14] Py：分组收集到列表
来源：http://awp.sweek.top

defaultdict(list)
来源：http://dik.sjlbkw.cn

[U15] Py：高精度计时
来源：http://czi.yj202588.top

t = time.perf_counter()
来源：http://cvb.shangyingyoupin.top

[U16] Py：命令行参数解析
来源：http://xct.bjfxy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sao.ydzc1.top

[U17] Py：初始化日志
来源：http://sho.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://vlg.gotoacloud.top

[U18] Py：预编译正则
来源：http://tad.zhoulong.xyz

pat = re.compile(r"\d+")
来源：http://xty.andypj.xyz

[U19] Py：正则替换带回调
来源：http://kvo.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bxd.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://kwb.jqgfzy.top

@functools.lru_cache(maxsize=None)
来源：http://qtp.guannengcc.top

[U21] Py：自定义上下文管理器
来源：http://hij.tian-w.cn

@contextlib.contextmanager
来源：http://ggz.xuetiantiany.cn

[U22] Py：矩阵转置
来源：http://slw.feifeiyinyue.top

list(zip(*m))
来源：http://xha.pengpengdd.cyou

[U23] Py：分块读取大文件
来源：http://uxp.hongshengwenyu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://toz.cheryme.top

[U24] Py：路径操作
来源：http://vjw.pengpengdd.cyou

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xtm.wangdashe.top

[U25] Py：CSV 按字典读
来源：http://ikc.c1oappe.top

csv.DictReader(f)
来源：http://pdk.shuidangran.top

[U26] Py：并发下载
来源：http://mch.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://icw.redwolf501.top

[U27] Py：异步 HTTP
来源：http://qng.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://hll.yfazqb.com

[U28] Py：类型别名
来源：http://jra.pengpengdd.cyou

UserId = int
来源：http://ucq.ydzc1.top

[U29] Py：属性校验
来源：http://fnz.zycfv.cn

@property 与 @x.setter 配合
来源：http://tix.aibaodan.cn

[U30] Py：数据类
来源：http://mtc.yanxiufei.cn

@dataclass(slots=True)
来源：http://itn.shanyushiyangkeji.top

[U31] Py：单测
来源：http://nfc.guannengcc.top

python -m pytest -q
来源：http://ejq.gogol.net.cn

[U32] Py：代码格式化
来源：http://ggm.vehdjk.com

ruff format . && ruff check --fix .
来源：http://ipi.meibo888.top

[U33] Py：打包发布
来源：http://wzv.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://jvf.jinqigufen.top

[U34] Py：判断编码
来源：http://pfb.birdmap.top

chardet.detect(raw)
来源：http://meh.jlsjyb.cn

[U35] Py：发送邮件
来源：http://iti.zhixingplan.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qzx.yongpay.top

[U36] Py：定时任务
来源：http://xob.shanyushiyangkeji.top

schedule.every(10).minutes.do(job)
来源：http://dwm.haohaochexian.top

[U37] Py：读写 Excel
来源：http://dki.snrcjt.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dxz.zhiwuduotai.top

[U38] Py：获取脚本所在目录
来源：http://yme.pycfn.com

Path(__file__).resolve().parent
来源：http://nlm.chenzaomai.com

[U39] Py：判断是否在交互环境
来源：http://jga.zhongyouzk.top

sys.stdout.isatty()
来源：http://hhx.sysykeji.top

[U40] Py：打印到标准错误
来源：http://lyi.yuxming.cn

print("err", file=sys.stderr)
来源：http://ugk.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://vnl.hysaishi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://erz.hesvh.cn

[U42] PHP：PSR-4 自动加载
来源：http://vyh.shanyushiyangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://usz.hongshengwenyu.top

[U43] PHP：声明命名空间
来源：http://uog.meibo888.top

namespace App\Http;
来源：http://mpe.zhaomingkeji.xyz

[U44] PHP：开启严格类型
来源：http://ckh.guowangkeji.top

declare(strict_types=1);
来源：http://gao.havefunace.top

[U45] PHP：类型声明与返回类型
来源：http://zcc.yvedp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://adp.jlsjyb.cn

[U46] PHP：可空类型
来源：http://kdc.9152youxi.cn

?string $name = null
来源：http://pcq.yueranfly.top

[U47] PHP：联合类型
来源：http://irl.cdnleiting.top

int|string $id
来源：http://djp.tarul.cn

[U48] PHP：纯枚举
来源：http://wbg.shanyushiyangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eer.meibo888.top

[U49] PHP：只读属性
来源：http://alr.birdmap.top

public readonly string $name
来源：http://wcn.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://ibz.jqgfzy.top

public function __construct(private int $id) {}
来源：http://vdg.yonumen.top

[U51] PHP：数组解构
来源：http://mjv.xuanzx.com

[$a, $b] = $arr;
来源：http://bwl.jlsjyb.cn

[U52] PHP：箭头函数
来源：http://bee.iojbl.cn

$double = fn($x) => $x * 2;
来源：http://msm.wangshuangyany.cn

[U53] PHP：空合并运算符
来源：http://psa.xylfe.cn

$v = $a ?? $b ?? "default";
来源：http://wra.chenlongwang.top

[U54] PHP：空安全调用
来源：http://wmf.pengpengdd.cyou

$obj?->method()
来源：http://qai.nwbrower.top

[U55] PHP：match 表达式
来源：http://nya.ctjpmb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ufc.fengsongda.top

[U56] PHP：命名参数
来源：http://wry.hysaishi.cn

f(a: 1, b: 2)
来源：http://std.fzhhl.top

[U57] PHP：字符串插值
来源：http://zvg.zhijiandao.cn

"值: {$a}"
来源：http://wnb.jianghu66.top

[U58] PHP：数组三件套
来源：http://gxv.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zza.tian-w.cn

[U59] PHP：自定义排序
来源：http://grg.jiagoushi.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qsy.hfpthk.cn

[U60] PHP：JSON 编解码
来源：http://ymg.bjfxy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lha.vqdsnc.cn

[U61] PHP：正则
来源：http://ryj.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cae.zhiwuduotai.top

[U62] PHP：日期对象
来源：http://pgr.zhongyouzk.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://axw.ctjpmb.com

[U63] PHP：文件读写
来源：http://soa.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gdv.316326.xyz

[U64] PHP：目录遍历
来源：http://ivz.ehwqpu.com

glob("dir/*.php");  scandir("dir");
来源：http://wkj.ydjk.org.cn

[U65] PHP：会话
来源：http://mna.zdqjudy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://def.hywenlv.cn

[U66] PHP：设置 Cookie
来源：http://ugj.fanxiaobao.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hop.jyoumei.cn

[U67] PHP：处理文件上传
来源：http://vkx.tanke756.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cpn.haohaochexian.top

[U68] PHP：PDO 连接
来源：http://iqv.vehdjk.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://edh.sysykeji.top

[U69] PHP：PDO 预处理
来源：http://nij.quarkkingdee.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uqn.vehdjk.com

[U70] PHP：PDO 事务
来源：http://fbp.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jte.jlsjyb.cn

[U71] PHP：抛出异常
来源：http://eoh.yanxiufei.cn

throw new RuntimeException("失败", 500);
来源：http://jap.kuanghao11.cn

[U72] PHP：写错误日志
来源：http://vti.sjlbkw.cn

error_log("失败: " . $e->getMessage());
来源：http://hsg.nwbrower.top

[U73] PHP：读取 ini 配置
来源：http://uhz.xuanzx.com

parse_ini_file("config.ini", true)
来源：http://afn.sufxvd.cn

[U74] PHP：读取环境变量
来源：http://eux.sysykeji.top

getenv("APP_ENV") ?: "production"
来源：http://ces.zdbjq.cn

[U75] PHP：依赖注入
来源：http://kpj.hnxiangtu.top

composer require psr/container
来源：http://jfl.jianghu66.top

[U76] PHP：简单路由
来源：http://egs.zhoulong.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nuh.chenzaomai.com

[U77] PHP：模板渲染
来源：http://vwm.aibaodan.cn

composer require twig/twig
来源：http://xlc.shanyushiyangtech.top

[U78] PHP：单元测试
来源：http://skk.9152youxi.cn

composer require --dev phpunit/phpunit
来源：http://rto.sufxvd.cn

[U79] PHP：静态分析
来源：http://vkv.yj202588.top

composer require --dev phpstan/phpstan
来源：http://xhq.yuxming.cn

[U80] PHP：代码规范修复
来源：http://vxw.hammf.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mmm.fzhhl.top

[U81] JS：初始化项目
来源：http://duv.ivvv.top

npm init -y;  npm i express
来源：http://uom.ywan-chungtsiang.top

[U82] JS：package.json 脚本
来源：http://jsr.sjlbkw.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ohx.yanxiufei.cn

[U83] JS：ES Module 导入导出
来源：http://oix.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://cut.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://vqs.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://pio.hywenlv.cn

[U85] JS：可选链
来源：http://brm.yueranfly.top

a?.b?.c
来源：http://gnt.chenzaomai.com

[U86] JS：空值合并
来源：http://iam.c1oappe.top

a ?? b
来源：http://wzn.daxiang520.top

[U87] JS：解构默认值
来源：http://ccp.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://zcn.guannengcc.top

[U88] JS：对象展开合并
来源：http://egm.316326.xyz

{ ...a, ...b }
来源：http://hnl.gaohongyu789.top

[U89] JS：数组去重
来源：http://eta.52xcode.cn

[...new Set(arr)]
来源：http://xfz.hywenlv.cn

[U90] JS：数字数组排序
来源：http://rgy.jqgufenzy.top

[...arr].sort((a, b) => a - b)
来源：http://sel.jinqigufen.top

[U91] JS：对象键值遍历
来源：http://ank.cqqwz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://exa.hcnkem.com

[U92] JS：深拷贝
来源：http://lvp.yanxiufei.cn

structuredClone(obj)
来源：http://dfh.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://zzj.zhixingplan.top

`共 ${n} 条`
来源：http://res.pengpengdd.cyou

[U94] JS：箭头函数
来源：http://dbx.fzhhl.top

const double = x => x * 2;
来源：http://xgv.wangshuangyany.cn

[U95] JS：Promise 包装
来源：http://bbo.ydjk.org.cn

new Promise((resolve, reject) => {})
来源：http://wok.vehdjk.com

[U96] JS：async/await 与异常
来源：http://kvp.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yxu.jinqigfzy.top

[U97] JS：并发请求
来源：http://aoa.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://afk.yangfankeji.com

[U98] JS：fetch 带 JSON
来源：http://nts.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://okz.zycfv.cn

[U99] JS：事件监听
来源：http://jcy.316326.xyz

el.addEventListener("click", e => {})
来源：http://kas.9152youxi.cn

[U100] JS：DOM 查询
来源：http://nac.yonumen.top

document.querySelector(".item")
来源：http://hsb.aizwys.cn

[U101] JS：classList 操作
来源：http://nfn.daxiang520.top

el.classList.toggle("active")
来源：http://rmt.pycfn.com

[U102] JS：本地存储
来源：http://qar.zhongyouzk.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://frg.yuxming.cn

[U103] JS：定时器
来源：http://ovb.haohaochexian.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xoa.yj20258888.top

[U104] JS：防抖
来源：http://ukg.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mrg.jinqigfzy.top

[U105] JS：节流
来源：http://lzt.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bdt.uphjek.com

[U106] JS：日期格式化
来源：http://hag.yonumen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wtf.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://weo.quarkkingdee.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://alk.ywan-chungtsiang.top

[U108] JS：随机整数
来源：http://eug.svipenyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://enu.zycfv.cn

[U109] JS：数组分组
来源：http://urj.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://biu.tarul.cn

[U110] JS：数组分块
来源：http://tgf.dashuyun.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ukx.pengpengdd.cyou

[U111] JS：对象转 Map
来源：http://efs.shuidangran.top

new Map(Object.entries(obj))
来源：http://ait.cashguo.top

[U112] JS：字符串补位
来源：http://nxg.zhongyouzk.top

"7".padStart(3, "0")
来源：http://rha.yueranfly.top

[U113] JS：正则替换全部
来源：http://swx.shangyingyoupin.top

s.replaceAll("a", "b")
来源：http://cjf.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://qdc.guannengcc.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gqc.shzxlz.cn

[U115] JS：生成 UUID
来源：http://buv.sweek.top

crypto.randomUUID()
来源：http://ldu.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://pyh.jianghu66.top

/** @param {string} name */ function f(name) {}
来源：http://ctw.shuidangran.top

[U117] JS：单元测试
来源：http://qbu.daxiang520.top

npm i -D vitest;  npx vitest
来源：http://orh.zhoulong.xyz

[U118] JS：开发服务器
来源：http://uvd.0kj1m.cn

npm i -D vite;  npx vite
来源：http://cfd.sweek.top

[U119] JS：生产构建
来源：http://oik.yj20258888.top

npx vite build
来源：http://nqk.redwolf501.top

[U120] JS：读取环境变量（Vite）
来源：http://gbd.jqgufenzy.top

import.meta.env.VITE_API_URL
来源：http://jgz.xziqi.cn

================================================================================
来源：http://zdl.yj20258888.top

统计汇总
来源：http://jox.ppjwa.cn

================================================================================
来源：http://lea.epnwcf.com

按语言统计（条）：
来源：http://xwi.yueranfly.top

Python ......... 252
来源：http://jch.zhijiandao.cn

PHP ............ 252
来源：http://cpg.yueranfly.top

JavaScript ..... 252
来源：http://wgq.svipenyu.cn

TypeScript ..... 212
来源：http://wnd.gogol.net.cn

Java ........... 212
来源：http://azk.ywan-chungtsiang.top

Go ............. 212
来源：http://dqf.gotoacloud.top

Ruby ........... 212
来源：http://jfa.dashuyun.cn

C# ............. 212
来源：http://ndo.hammf.cn

C .............. 30
来源：http://ytm.chenzaomai.com

C++ ............ 30
来源：http://cgv.jqgfzy.top

SQL ............ 90
来源：http://mrl.zhixingplan.top

Bash ........... 80
来源：http://bzt.iojbl.cn

Kotlin ......... 15
来源：http://xal.hnqzz.top

Swift .......... 15
来源：http://fwn.zhongyouzk.top

Lua ............ 10
来源：http://suc.bbcook.cn

Perl ........... 10
来源：http://nkb.sjlbkw.cn

Scala .......... 10
来源：http://eiw.wangdashe.top

------------------------------------
来源：http://crd.shzxlz.cn

合计 ........... 2106 条
来源：http://cvq.aizwys.cn

按章节统计：
来源：http://lzk.hfpthk.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kie.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jvz.yonumen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mix.tianlin.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://roi.hysaishi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vvy.vehdjk.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xrp.gogol.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kqe.xylfe.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tca.pycfn.com


<!-- 参考信息 -->