代发 wailian999

[T47] Perl：正则捕获
来源：http://azo.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lha.gaohongyu789.top

[T48] Perl：正则替换
来源：http://hsq.yj202588.top

$s =~ s/old/new/g;
来源：http://fmn.yongpay.top

[T49] Perl：函数
来源：http://fbf.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qeo.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://hlr.svipenyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zkc.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://xsr.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://gtr.gotoacloud.top

println("Hello")
来源：http://gib.wangdashe.top

[T52] Scala：变量
来源：http://yuu.mhx1999.top

val a = 1;  var b = 2
来源：http://puv.zhaomingkeji.xyz

[T53] Scala：字符串插值
来源：http://ahl.snrcjt.cn

s"值: $b"
来源：http://ixc.jqgfzy.top

[T54] Scala：集合映射
来源：http://hfd.zycfv.cn

List(1, 2, 3).map(_ * 2)
来源：http://ink.vqdsnc.cn

[T55] Scala：集合过滤
来源：http://zsz.yanxiufei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kzl.xuanzx.com

[T56] Scala：样例类
来源：http://jlr.yueranfly.top

case class User(name: String, age: Int)
来源：http://yvo.pycfn.com

[T57] Scala：模式匹配
来源：http://kxf.ybcxt.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wwz.xingfuxueyuan.xyz

[T58] Scala：函数定义
来源：http://uej.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://djd.bbcook.cn

[T59] Scala：循环
来源：http://zuw.ydzc1.top

for (i <- 1 to 10) println(i)
来源：http://rqd.zhoulong.xyz

[T60] Scala：折叠
来源：http://jmb.jqgufenzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mop.vqdsnc.cn

================================================================================
来源：http://vdc.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tpb.meibo888.top

================================================================================
来源：http://wvm.ydjk.org.cn

[U01] Py：创建虚拟环境
来源：http://pcd.ydjk.org.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dct.uphjek.com

[U02] Py：导出 / 安装依赖
来源：http://ggd.gzhubu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hur.jinyuanbaomall.cn

[U03] Py：加载 .env 配置
来源：http://sfw.hnqzz.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fld.cashguo.top

[U04] Py：变量调试打印
来源：http://beo.pycfn.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://azv.zdqjudy.top

[U05] Py：列表去重且保序
来源：http://nvg.vehdjk.com

list(dict.fromkeys(arr))
来源：http://isy.316326.xyz

[U06] Py：合并两个字典
来源：http://xbc.yanxiufei.cn

{**a, **b}
来源：http://ryh.zhoulong.xyz

[U07] Py：反转字典键值
来源：http://hqy.gaohongyu789.top

{v: k for k, v in d.items()}
来源：http://vhu.hnxiangtu.top

[U08] Py：展平二维列表
来源：http://izs.ybcxt.top

[y for x in nested for y in x]
来源：http://faq.gaohongyu789.top

[U09] Py：字典取最大值的键
来源：http://xlo.ywan-chungtsiang.top

max(d, key=d.get)
来源：http://axi.cashguo.top

[U10] Py：按值排序字典
来源：http://xpe.meibo888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uct.zhaomingkeji.xyz

[U11] Py：生成器表达式
来源：http://ope.redwolf501.top

(x * 2 for x in arr)
来源：http://xsx.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tsm.52xcode.cn

Counter(arr).most_common(3)
来源：http://cid.cheryme.top

[U13] Py：固定长度队列
来源：http://box.hammf.cn

deque(maxlen=10)
来源：http://tzb.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://npv.tarul.cn

defaultdict(list)
来源：http://bug.pengpengdd.cyou

[U15] Py：高精度计时
来源：http://ajk.bjfxy.top

t = time.perf_counter()
来源：http://bxw.daria6918.cn

[U16] Py：命令行参数解析
来源：http://lrk.tanke756.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dsr.jinqigufen.top

[U17] Py：初始化日志
来源：http://kni.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://chi.dianchejie.cn

[U18] Py：预编译正则
来源：http://uec.tanke756.top

pat = re.compile(r"\d+")
来源：http://isn.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://jsk.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bdl.shuidangran.top

[U20] Py：缓存函数结果
来源：http://rbm.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://bwy.birdmap.top

[U21] Py：自定义上下文管理器
来源：http://yds.yueranfly.top

@contextlib.contextmanager
来源：http://ncr.jiagoushi.top

[U22] Py：矩阵转置
来源：http://eku.sysykeji.top

list(zip(*m))
来源：http://xsi.zycfv.cn

[U23] Py：分块读取大文件
来源：http://lth.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zpw.wangshuangyany.cn

[U24] Py：路径操作
来源：http://hht.cucudq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xxq.sysykeji.top

[U25] Py：CSV 按字典读
来源：http://whu.guowangkeji.top

csv.DictReader(f)
来源：http://egk.yfazqb.com

[U26] Py：并发下载
来源：http://khd.bjfxy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iru.yueranfly.top

[U27] Py：异步 HTTP
来源：http://bvv.hnxiangtu.top

aiohttp.ClientSession() 配合 async with
来源：http://pbn.hywenlv.cn

[U28] Py：类型别名
来源：http://nnt.zhiwuduotai.top

UserId = int
来源：http://wmh.svipenyu.cn

[U29] Py：属性校验
来源：http://qyd.daria6918.cn

@property 与 @x.setter 配合
来源：http://rfv.yj20258.top

[U30] Py：数据类
来源：http://ssh.zdqjudy.top

@dataclass(slots=True)
来源：http://gfo.sufxvd.cn

[U31] Py：单测
来源：http://cqx.xuetiantiany.cn

python -m pytest -q
来源：http://ttx.yj20258.top

[U32] Py：代码格式化
来源：http://uhe.hfpthk.cn

ruff format . && ruff check --fix .
来源：http://ktz.gotoacloud.top

[U33] Py：打包发布
来源：http://bfe.jinyuanbaomall.cn

python -m build  （依赖 pyproject.toml）
来源：http://smc.dashuyun.cn

[U34] Py：判断编码
来源：http://clk.haohaochexian.top

chardet.detect(raw)
来源：http://bkn.birdmap.top

[U35] Py：发送邮件
来源：http://bqr.fanxiaobao.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aqw.c1oappe.top

[U36] Py：定时任务
来源：http://brb.haohaochexian.top

schedule.every(10).minutes.do(job)
来源：http://oxf.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://sjw.epnwcf.com

pandas.read_excel / DataFrame.to_excel
来源：http://nml.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://raz.smart0.xyz

Path(__file__).resolve().parent
来源：http://iwd.xuanzx.com

[U39] Py：判断是否在交互环境
来源：http://xuj.hammf.cn

sys.stdout.isatty()
来源：http://mln.ydzc1.top

[U40] Py：打印到标准错误
来源：http://tjp.316326.xyz

print("err", file=sys.stderr)
来源：http://nno.guannengcc.top

[U41] PHP：初始化 Composer 项目
来源：http://dgz.jinqigufen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://acm.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://atm.jyoumei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fyo.xziqi.cn

[U43] PHP：声明命名空间
来源：http://gtk.yvedp.cn

namespace App\Http;
来源：http://gnc.fengsongda.top

[U44] PHP：开启严格类型
来源：http://lxv.xuanzx.com

declare(strict_types=1);
来源：http://kfi.pengpengdd.cyou

[U45] PHP：类型声明与返回类型
来源：http://tqo.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ncv.kuanghao11.cn

[U46] PHP：可空类型
来源：http://epr.ydjk.org.cn

?string $name = null
来源：http://kkz.yanxiufei.cn

[U47] PHP：联合类型
来源：http://scr.nanxuanxn.top

int|string $id
来源：http://uhy.svipenyu.cn

[U48] PHP：纯枚举
来源：http://mdy.gogol.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cqa.yonumen.top

[U49] PHP：只读属性
来源：http://ryg.cdnleiting.top

public readonly string $name
来源：http://ali.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://ubu.jinghuilouyu.cn

public function __construct(private int $id) {}
来源：http://wih.xuanzx.com

[U51] PHP：数组解构
来源：http://ygx.bbcook.cn

[$a, $b] = $arr;
来源：http://vcl.wangdashe.top

[U52] PHP：箭头函数
来源：http://mas.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://xyl.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://isa.ywan-chungtsiang.top

$v = $a ?? $b ?? "default";
来源：http://kpg.fanxiaobao.xyz

[U54] PHP：空安全调用
来源：http://hhf.nanxinkj.top

$obj?->method()
来源：http://qmi.yj202588.top

[U55] PHP：match 表达式
来源：http://irs.fehbvm.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://art.gogol.net.cn

[U56] PHP：命名参数
来源：http://twh.tanke756.top

f(a: 1, b: 2)
来源：http://lxd.hysaishi.cn

[U57] PHP：字符串插值
来源：http://suq.nwbrower.top

"值: {$a}"
来源：http://hiw.ydjk.org.cn

[U58] PHP：数组三件套
来源：http://caj.andypj.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yvz.gotoacloud.top

[U59] PHP：自定义排序
来源：http://wbf.cdnleiting.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vgc.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://fud.nanxinkj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qit.hnxiangtu.top

[U61] PHP：正则
来源：http://qim.kuanghao11.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://orv.hfpthk.cn

[U62] PHP：日期对象
来源：http://ipa.yvedp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gjn.hysaishi.cn

[U63] PHP：文件读写
来源：http://par.feifeiyinyue.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jyn.ybcxt.top

[U64] PHP：目录遍历
来源：http://hrg.yvedp.cn

glob("dir/*.php");  scandir("dir");
来源：http://rpz.fzhhl.top

[U65] PHP：会话
来源：http://ggu.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vej.aizwys.cn

[U66] PHP：设置 Cookie
来源：http://ymi.hysaishi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://icz.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://qmw.zdbjq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jgf.yj20258888.top

[U68] PHP：PDO 连接
来源：http://rys.nanxinkj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ghy.jinyuanbaomall.cn

[U69] PHP：PDO 预处理
来源：http://iep.feifeiyinyue.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rjd.shzxlz.cn

[U70] PHP：PDO 事务
来源：http://kba.vehdjk.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hdj.hesvh.cn

[U71] PHP：抛出异常
来源：http://evx.feifeiyinyue.top

throw new RuntimeException("失败", 500);
来源：http://uur.andypj.xyz

[U72] PHP：写错误日志
来源：http://lnh.quarkkingdee.top

error_log("失败: " . $e->getMessage());
来源：http://cfb.sxryk.cn

[U73] PHP：读取 ini 配置
来源：http://ekx.pengpengdd.cyou

parse_ini_file("config.ini", true)
来源：http://dza.bjfxy.top

[U74] PHP：读取环境变量
来源：http://gss.aizwys.cn

getenv("APP_ENV") ?: "production"
来源：http://tfh.hnqzz.top

[U75] PHP：依赖注入
来源：http://oip.dianchejie.cn

composer require psr/container
来源：http://dtm.fktsv.cn

[U76] PHP：简单路由
来源：http://tyg.haohaochexian.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tsz.tianlin.xyz

[U77] PHP：模板渲染
来源：http://dqb.aizwys.cn

composer require twig/twig
来源：http://bgh.ydjk.org.cn

[U78] PHP：单元测试
来源：http://gwm.wangshuangyany.cn

composer require --dev phpunit/phpunit
来源：http://bny.sjlbkw.cn

[U79] PHP：静态分析
来源：http://jny.dashuyun.cn

composer require --dev phpstan/phpstan
来源：http://dln.aibaodan.cn

[U80] PHP：代码规范修复
来源：http://vsk.jqgfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ulp.jiagoushi.top

[U81] JS：初始化项目
来源：http://hdz.fktsv.cn

npm init -y;  npm i express
来源：http://rzr.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://smi.zhijiandao.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qyv.epnwcf.com

[U83] JS：ES Module 导入导出
来源：http://vvx.yfazqb.com

export const a = 1;  import { a } from "./m.js";
来源：http://slm.andypj.xyz

[U84] JS：CommonJS 写法
来源：http://cgf.yonumen.top

module.exports = { a };  const { a } = require("./m");
来源：http://lmv.chenzaomai.com

[U85] JS：可选链
来源：http://xsp.zhiwuduotai.top

a?.b?.c
来源：http://wku.zhengqikj.top

[U86] JS：空值合并
来源：http://nos.sjlbkw.cn

a ?? b
来源：http://ddo.ybcxt.top

[U87] JS：解构默认值
来源：http://aso.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://mjg.andypj.xyz

[U88] JS：对象展开合并
来源：http://yix.pengpengdd.cyou

{ ...a, ...b }
来源：http://nmr.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://yqk.ppjwa.cn

[...new Set(arr)]
来源：http://lis.tian-w.cn

[U90] JS：数字数组排序
来源：http://mrm.chenjidiqi.icu

[...arr].sort((a, b) => a - b)
来源：http://wjm.tianlin.xyz

[U91] JS：对象键值遍历
来源：http://lvq.jinyuanbaomall.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yye.zhaomingkeji.xyz

[U92] JS：深拷贝
来源：http://hkd.daria6918.cn

structuredClone(obj)
来源：http://mxx.tarul.cn

[U93] JS：模板字符串
来源：http://ona.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://ord.sysykeji.top

[U94] JS：箭头函数
来源：http://lod.chenzaomai.com

const double = x => x * 2;
来源：http://ipn.gaohongyu789.top

[U95] JS：Promise 包装
来源：http://non.shanyushiyangkeji.top

new Promise((resolve, reject) => {})
来源：http://wzp.hongshengwenyu.top

[U96] JS：async/await 与异常
来源：http://yqf.hnxiangtu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dxi.hfpthk.cn

[U97] JS：并发请求
来源：http://mab.mhx1999.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xhy.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://iif.jianghu66.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lhe.sysykeji.top

[U99] JS：事件监听
来源：http://dcu.ywan-chungtsiang.top

el.addEventListener("click", e => {})
来源：http://eip.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://ult.hfpthk.cn

document.querySelector(".item")
来源：http://wpn.cucudq.cn

[U101] JS：classList 操作
来源：http://gic.zhijiandao.cn

el.classList.toggle("active")
来源：http://xrf.zhiwuduotai.top

[U102] JS：本地存储
来源：http://tiz.yfazqb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://mzz.epnwcf.com

[U103] JS：定时器
来源：http://nnb.dianchejie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ttt.dashuyun.cn

[U104] JS：防抖
来源：http://xiy.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nuv.chenlongwang.top

[U105] JS：节流
来源：http://ftc.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gub.zhiwuduotai.top

[U106] JS：日期格式化
来源：http://cls.yonumen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://voh.sysykeji.top

[U107] JS：数字千分位
来源：http://ogx.dashuyun.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rqc.hysaishi.cn

[U108] JS：随机整数
来源：http://tat.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uvb.cucudq.cn

[U109] JS：数组分组
来源：http://jrx.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://aav.nwbrower.top

[U110] JS：数组分块
来源：http://puu.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jko.cashguo.top

[U111] JS：对象转 Map
来源：http://jhr.zhengqikj.top

new Map(Object.entries(obj))
来源：http://olg.ctjpmb.com

[U112] JS：字符串补位
来源：http://wpk.hnxiangtu.top

"7".padStart(3, "0")
来源：http://vxp.smart0.xyz

[U113] JS：正则替换全部
来源：http://hwd.guannengcc.top

s.replaceAll("a", "b")
来源：http://buz.quarkkingdee.top

[U114] JS：JSON 深比较
来源：http://pgr.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bez.ehwqpu.com

[U115] JS：生成 UUID
来源：http://vyt.shuidangran.top

crypto.randomUUID()
来源：http://vou.yj202588.top

[U116] JS：类型检查（JSDoc）
来源：http://eva.vqdsnc.cn

/** @param {string} name */ function f(name) {}
来源：http://aic.ydzc1.top

[U117] JS：单元测试
来源：http://alj.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://tpm.fzhhl.top

[U118] JS：开发服务器
来源：http://tuu.sweek.top

npm i -D vite;  npx vite
来源：http://uwa.tianlin.xyz

[U119] JS：生产构建
来源：http://bmz.zhengqikj.top

npx vite build
来源：http://xhe.yanxiufei.cn

[U120] JS：读取环境变量（Vite）
来源：http://cst.mhx1999.top

import.meta.env.VITE_API_URL
来源：http://rcm.meibo888.top

================================================================================
来源：http://oeg.yanxiufei.cn

统计汇总
来源：http://ydn.fktsv.cn

================================================================================
来源：http://pdv.ivvv.top

按语言统计（条）：
来源：http://mve.ehwqpu.com

Python ......... 252
来源：http://ayo.shanyushiyangkeji.top

PHP ............ 252
来源：http://hge.epnwcf.com

JavaScript ..... 252
来源：http://csz.xinyue.icu

TypeScript ..... 212
来源：http://egm.pengpengdd.cyou

Java ........... 212
来源：http://ejh.ppjwa.cn

Go ............. 212
来源：http://oog.yanxiufei.cn

Ruby ........... 212
来源：http://whi.zhongyouzk.top

C# ............. 212
来源：http://bid.vehdjk.com

C .............. 30
来源：http://ggr.sweek.top

C++ ............ 30
来源：http://sur.jinqigfzy.top

SQL ............ 90
来源：http://nlj.zycfv.cn

Bash ........... 80
来源：http://qmq.epnwcf.com

Kotlin ......... 15
来源：http://rmt.yuxming.cn

Swift .......... 15
来源：http://ikw.yueranfly.top

Lua ............ 10
来源：http://kls.epnwcf.com

Perl ........... 10
来源：http://hob.zhengqikj.top

Scala .......... 10
来源：http://cex.meibo888.top

------------------------------------
来源：http://zcz.vehdjk.com

合计 ........... 2106 条
来源：http://jyi.vehdjk.com

按章节统计：
来源：http://kzv.andypj.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bkr.sufxvd.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ill.jinyuanbaomall.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aty.svipenyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ufp.quarkkingdee.top


<!-- 参考信息 -->