代发 wailian999

[T43] Perl：字符串插值
来源：http://qpy.jinghuilouyu.cn

"值: $a"
来源：http://phd.yanxiufei.cn

[T44] Perl：条件
来源：http://mxv.gzhubu.top

if ($a > 0) { print "正"; }
来源：http://kvl.jianghu66.top

[T45] Perl：数组遍历
来源：http://gua.zdbjq.cn

for my $x (@arr) { print $x; }
来源：http://jjp.ehwqpu.com

[T46] Perl：哈希操作
来源：http://pym.xingfuxueyuan.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ggp.jianghu66.top

[T47] Perl：正则捕获
来源：http://rdc.fehbvm.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://rdc.zhongyouzk.top

[T48] Perl：正则替换
来源：http://jic.zdbjq.cn

$s =~ s/old/new/g;
来源：http://qka.cqqwz.cn

[T49] Perl：函数
来源：http://duz.pengpengdd.cyou

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mrb.cashguo.top

[T50] Perl：逐行读文件
来源：http://ajg.yangfankeji.com

open my $fh, "<", "a.txt" or die $!;
来源：http://okp.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://nku.shanyushiyangkeji.top

[T51] Scala：Hello World
来源：http://bjs.sufxvd.cn

println("Hello")
来源：http://hqe.yj20258.top

[T52] Scala：变量
来源：http://ecy.xuanzx.com

val a = 1;  var b = 2
来源：http://fvj.jinghuilouyu.cn

[T53] Scala：字符串插值
来源：http://gbc.havefunace.top

s"值: $b"
来源：http://kfb.cashguo.top

[T54] Scala：集合映射
来源：http://tdd.nanxuanxn.top

List(1, 2, 3).map(_ * 2)
来源：http://wej.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://zjz.meibo888.top

List(1, 2, 3).filter(_ > 1)
来源：http://mhm.yj202588.top

[T56] Scala：样例类
来源：http://adl.hcnkem.com

case class User(name: String, age: Int)
来源：http://ryi.jiagoushi.top

[T57] Scala：模式匹配
来源：http://uzy.mhx1999.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jcz.chenlongwang.top

[T58] Scala：函数定义
来源：http://dol.zhiwuduotai.top

def add(a: Int, b: Int): Int = a + b
来源：http://pqf.smart0.xyz

[T59] Scala：循环
来源：http://iqx.9152youxi.cn

for (i <- 1 to 10) println(i)
来源：http://qtf.ppjwa.cn

[T60] Scala：折叠
来源：http://uem.52xcode.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lrj.jqgufenzy.top

================================================================================
来源：http://nti.ydzc1.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qrf.cdnleiting.top

================================================================================
来源：http://vaf.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://hft.bbcook.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jym.tanke756.top

[U02] Py：导出 / 安装依赖
来源：http://nbh.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dfa.dashuyun.cn

[U03] Py：加载 .env 配置
来源：http://mgw.tanke756.top

from dotenv import load_dotenv; load_dotenv()
来源：http://joe.zdqjudy.top

[U04] Py：变量调试打印
来源：http://yos.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gui.hcnkem.com

[U05] Py：列表去重且保序
来源：http://exs.havefunace.top

list(dict.fromkeys(arr))
来源：http://ogx.daria6918.cn

[U06] Py：合并两个字典
来源：http://jji.ydzc1.top

{**a, **b}
来源：http://ztv.xylfe.cn

[U07] Py：反转字典键值
来源：http://gam.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://xdh.yueranfly.top

[U08] Py：展平二维列表
来源：http://gzf.yueranfly.top

[y for x in nested for y in x]
来源：http://nwg.snrcjt.cn

[U09] Py：字典取最大值的键
来源：http://dmw.aibaodan.cn

max(d, key=d.get)
来源：http://sax.zhiwuduotai.top

[U10] Py：按值排序字典
来源：http://hpy.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vzg.c1oappe.top

[U11] Py：生成器表达式
来源：http://abc.hywenlv.cn

(x * 2 for x in arr)
来源：http://mrf.zhaomingkeji.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://oqt.shangyingyoupin.top

Counter(arr).most_common(3)
来源：http://zsv.smart0.xyz

[U13] Py：固定长度队列
来源：http://gvk.fzhhl.top

deque(maxlen=10)
来源：http://bit.vehdjk.com

[U14] Py：分组收集到列表
来源：http://clu.yj20258888.top

defaultdict(list)
来源：http://irz.hongshengwenyu.top

[U15] Py：高精度计时
来源：http://dcn.ydjk.org.cn

t = time.perf_counter()
来源：http://ntu.kuanghao11.cn

[U16] Py：命令行参数解析
来源：http://lib.yj20258.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zau.hongshengwenyu.top

[U17] Py：初始化日志
来源：http://tvz.jyoumei.cn

logging.basicConfig(level=logging.INFO)
来源：http://plq.sjlbkw.cn

[U18] Py：预编译正则
来源：http://fhx.hammf.cn

pat = re.compile(r"\d+")
来源：http://nqe.zdqjudy.top

[U19] Py：正则替换带回调
来源：http://gns.sweek.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qfl.aizwys.cn

[U20] Py：缓存函数结果
来源：http://ylo.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://oyy.hammf.cn

[U21] Py：自定义上下文管理器
来源：http://qip.hfpthk.cn

@contextlib.contextmanager
来源：http://ocp.gzhubu.top

[U22] Py：矩阵转置
来源：http://pby.xylfe.cn

list(zip(*m))
来源：http://gsk.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://aip.xylfe.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rkx.hammf.cn

[U24] Py：路径操作
来源：http://tbv.pycfn.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aab.zhengqikj.top

[U25] Py：CSV 按字典读
来源：http://qro.yj20258888.top

csv.DictReader(f)
来源：http://eec.yj20258888.top

[U26] Py：并发下载
来源：http://xrv.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dgq.zhongyouzk.top

[U27] Py：异步 HTTP
来源：http://bma.yonumen.top

aiohttp.ClientSession() 配合 async with
来源：http://flu.yuxming.cn

[U28] Py：类型别名
来源：http://gwp.smart0.xyz

UserId = int
来源：http://ghd.zhongyouzk.top

[U29] Py：属性校验
来源：http://jpx.xingfuxueyuan.xyz

@property 与 @x.setter 配合
来源：http://hab.shanyushiyangtech.top

[U30] Py：数据类
来源：http://ahy.mhx1999.top

@dataclass(slots=True)
来源：http://yds.nanxinkj.top

[U31] Py：单测
来源：http://wwl.gogol.net.cn

python -m pytest -q
来源：http://aka.yfazqb.com

[U32] Py：代码格式化
来源：http://ryc.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://rav.zhoulong.xyz

[U33] Py：打包发布
来源：http://dia.shzxlz.cn

python -m build  （依赖 pyproject.toml）
来源：http://ozt.zhaomingkeji.xyz

[U34] Py：判断编码
来源：http://hac.epnwcf.com

chardet.detect(raw)
来源：http://dxm.bbcook.cn

[U35] Py：发送邮件
来源：http://lpl.vqdsnc.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bhx.xuanzx.com

[U36] Py：定时任务
来源：http://nwo.aizwys.cn

schedule.every(10).minutes.do(job)
来源：http://acv.tianlin.xyz

[U37] Py：读写 Excel
来源：http://evw.quarkkingdee.top

pandas.read_excel / DataFrame.to_excel
来源：http://qug.havefunace.top

[U38] Py：获取脚本所在目录
来源：http://vje.smart0.xyz

Path(__file__).resolve().parent
来源：http://agu.jqgfzy.top

[U39] Py：判断是否在交互环境
来源：http://cyw.fanxiaobao.xyz

sys.stdout.isatty()
来源：http://rxt.yonumen.top

[U40] Py：打印到标准错误
来源：http://bzg.jyoumei.cn

print("err", file=sys.stderr)
来源：http://glm.cqqwz.cn

[U41] PHP：初始化 Composer 项目
来源：http://tjd.zhaomingkeji.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://fni.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://ejh.hywenlv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ndh.ivvv.top

[U43] PHP：声明命名空间
来源：http://jvw.guowangkeji.top

namespace App\Http;
来源：http://egz.xinyue.icu

[U44] PHP：开启严格类型
来源：http://lsd.bjfxy.top

declare(strict_types=1);
来源：http://qlp.sxryk.cn

[U45] PHP：类型声明与返回类型
来源：http://fyi.ywan-chungtsiang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vhr.hysaishi.cn

[U46] PHP：可空类型
来源：http://tew.hesvh.cn

?string $name = null
来源：http://top.vqdsnc.cn

[U47] PHP：联合类型
来源：http://hwb.wangdashe.top

int|string $id
来源：http://gnn.shuidangran.top

[U48] PHP：纯枚举
来源：http://pzg.xuetiantiany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zeo.yueranfly.top

[U49] PHP：只读属性
来源：http://ekl.zycfv.cn

public readonly string $name
来源：http://irb.zycfv.cn

[U50] PHP：构造器属性提升
来源：http://wdf.wangdashe.top

public function __construct(private int $id) {}
来源：http://sgi.dianchejie.cn

[U51] PHP：数组解构
来源：http://gvl.sufxvd.cn

[$a, $b] = $arr;
来源：http://fgq.yj20258.top

[U52] PHP：箭头函数
来源：http://xwl.ppjwa.cn

$double = fn($x) => $x * 2;
来源：http://arp.hongshengwenyu.top

[U53] PHP：空合并运算符
来源：http://pyt.daxiang520.top

$v = $a ?? $b ?? "default";
来源：http://jay.zycfv.cn

[U54] PHP：空安全调用
来源：http://afo.aizwys.cn

$obj?->method()
来源：http://mfd.yvedp.cn

[U55] PHP：match 表达式
来源：http://jxn.xuetiantiany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gcr.guowangkeji.top

[U56] PHP：命名参数
来源：http://exd.yj20258.top

f(a: 1, b: 2)
来源：http://dbv.sxryk.cn

[U57] PHP：字符串插值
来源：http://qiq.kuanghao11.cn

"值: {$a}"
来源：http://fri.hfpthk.cn

[U58] PHP：数组三件套
来源：http://urt.zdbjq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uje.hammf.cn

[U59] PHP：自定义排序
来源：http://jzt.kuanghao11.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vjt.ctjpmb.com

[U60] PHP：JSON 编解码
来源：http://wjh.hcnkem.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hep.jqgfzy.top

[U61] PHP：正则
来源：http://tky.fanxiaobao.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uvp.cucudq.cn

[U62] PHP：日期对象
来源：http://gna.hywenlv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bsj.9152youxi.cn

[U63] PHP：文件读写
来源：http://mvx.jlsjyb.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nkd.snrcjt.cn

[U64] PHP：目录遍历
来源：http://ugx.tarul.cn

glob("dir/*.php");  scandir("dir");
来源：http://npd.zhixingplan.top

[U65] PHP：会话
来源：http://aea.hesvh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pxz.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://fmr.shzxlz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vbk.snrcjt.cn

[U67] PHP：处理文件上传
来源：http://rap.yj20258.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://obz.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://xqc.guannengcc.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sqy.52xcode.cn

[U69] PHP：PDO 预处理
来源：http://xsv.yonumen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wwd.zdqjudy.top

[U70] PHP：PDO 事务
来源：http://sji.pengpengdd.cyou

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zmt.xziqi.cn

[U71] PHP：抛出异常
来源：http://nbb.yanxiufei.cn

throw new RuntimeException("失败", 500);
来源：http://agu.xziqi.cn

[U72] PHP：写错误日志
来源：http://scs.pengpengdd.cyou

error_log("失败: " . $e->getMessage());
来源：http://wtc.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://qyk.52xcode.cn

parse_ini_file("config.ini", true)
来源：http://hjx.shanyushiyangtech.top

[U74] PHP：读取环境变量
来源：http://taq.chenlongwang.top

getenv("APP_ENV") ?: "production"
来源：http://zpy.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://suv.cheryme.top

composer require psr/container
来源：http://eei.zhongyouzk.top

[U76] PHP：简单路由
来源：http://pud.fehbvm.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cgv.yuxming.cn

[U77] PHP：模板渲染
来源：http://hhf.52xcode.cn

composer require twig/twig
来源：http://zcd.zhoulong.xyz

[U78] PHP：单元测试
来源：http://trt.gotoacloud.top

composer require --dev phpunit/phpunit
来源：http://ywr.316326.xyz

[U79] PHP：静态分析
来源：http://dlz.hnxiangtu.top

composer require --dev phpstan/phpstan
来源：http://xoc.xziqi.cn

[U80] PHP：代码规范修复
来源：http://gge.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ilf.sufxvd.cn

[U81] JS：初始化项目
来源：http://odi.haohaochexian.top

npm init -y;  npm i express
来源：http://jyi.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://ric.aizwys.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fxm.cashguo.top

[U83] JS：ES Module 导入导出
来源：http://bzs.ctjpmb.com

export const a = 1;  import { a } from "./m.js";
来源：http://hza.aizwys.cn

[U84] JS：CommonJS 写法
来源：http://eem.hfpthk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tzv.meibo888.top

[U85] JS：可选链
来源：http://naw.c1oappe.top

a?.b?.c
来源：http://fnr.tianlin.xyz

[U86] JS：空值合并
来源：http://nwb.sweek.top

a ?? b
来源：http://zks.hywenlv.cn

[U87] JS：解构默认值
来源：http://ytg.ctjpmb.com

const { a = 1, b = 2 } = obj;
来源：http://kkj.birdmap.top

[U88] JS：对象展开合并
来源：http://xzc.yj20258888.top

{ ...a, ...b }
来源：http://afx.yj20258.top

[U89] JS：数组去重
来源：http://qdb.bjfxy.top

[...new Set(arr)]
来源：http://lcu.yvedp.cn

[U90] JS：数字数组排序
来源：http://rbl.hcnkem.com

[...arr].sort((a, b) => a - b)
来源：http://otg.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://dpl.nanxuanxn.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ijm.chenjidiqi.icu

[U92] JS：深拷贝
来源：http://kvn.fehbvm.com

structuredClone(obj)
来源：http://bij.ivvv.top

[U93] JS：模板字符串
来源：http://nov.jinyuanbaomall.cn

`共 ${n} 条`
来源：http://bsa.vqdsnc.cn

[U94] JS：箭头函数
来源：http://ixi.xuetiantiany.cn

const double = x => x * 2;
来源：http://ofx.quarkkingdee.top

[U95] JS：Promise 包装
来源：http://ojp.mhx1999.top

new Promise((resolve, reject) => {})
来源：http://cxz.nanxinkj.top

[U96] JS：async/await 与异常
来源：http://scr.haohaochexian.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wxv.sufxvd.cn

[U97] JS：并发请求
来源：http://ntf.fzhhl.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cgj.kuanghao11.cn

[U98] JS：fetch 带 JSON
来源：http://iym.nanxuanxn.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ttv.vehdjk.com

[U99] JS：事件监听
来源：http://rtq.hnqzz.top

el.addEventListener("click", e => {})
来源：http://ggm.xuanzx.com

[U100] JS：DOM 查询
来源：http://dwt.zhiwuduotai.top

document.querySelector(".item")
来源：http://lyc.xuanzx.com

[U101] JS：classList 操作
来源：http://tsh.yfazqb.com

el.classList.toggle("active")
来源：http://zgj.0kj1m.cn

[U102] JS：本地存储
来源：http://jqa.9152youxi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rzt.daria6918.cn

[U103] JS：定时器
来源：http://ili.fktsv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://duo.mhx1999.top

[U104] JS：防抖
来源：http://hvu.hammf.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gpl.yj202588.top

[U105] JS：节流
来源：http://vye.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://veg.aibaodan.cn

[U106] JS：日期格式化
来源：http://klw.nanxuanxn.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fqy.jinghuilouyu.cn

[U107] JS：数字千分位
来源：http://nfc.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ysx.feifeiyinyue.top

[U108] JS：随机整数
来源：http://aee.jiagoushi.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pct.gaohongyu789.top

[U109] JS：数组分组
来源：http://lxc.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://ret.ctjpmb.com

[U110] JS：数组分块
来源：http://bfs.nanxuanxn.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qsm.hesvh.cn

[U111] JS：对象转 Map
来源：http://txl.fanxiaobao.xyz

new Map(Object.entries(obj))
来源：http://lja.sjlbkw.cn

[U112] JS：字符串补位
来源：http://ejn.yuxming.cn

"7".padStart(3, "0")
来源：http://myo.jinyuanbaomall.cn

[U113] JS：正则替换全部
来源：http://tyz.hnqzz.top

s.replaceAll("a", "b")
来源：http://oaj.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://mlq.gaohongyu789.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://duu.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://ayw.zhengqikj.top

crypto.randomUUID()
来源：http://rmy.bbcook.cn

[U116] JS：类型检查（JSDoc）
来源：http://ydr.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://osn.wangdashe.top

[U117] JS：单元测试
来源：http://fnu.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://lmh.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://lef.tarul.cn

npm i -D vite;  npx vite
来源：http://yxa.yonumen.top

[U119] JS：生产构建
来源：http://zun.hnxiangtu.top

npx vite build
来源：http://awq.andypj.xyz

[U120] JS：读取环境变量（Vite）
来源：http://pdz.hongshengwenyu.top

import.meta.env.VITE_API_URL
来源：http://qdq.bbcook.cn

================================================================================
来源：http://rjx.xinyue.icu

统计汇总
来源：http://rnu.316326.xyz

================================================================================
来源：http://ygx.vehdjk.com

按语言统计（条）：
来源：http://mxa.kuanghao11.cn

Python ......... 252
来源：http://dax.ctjpmb.com

PHP ............ 252
来源：http://wgu.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://mmx.yueranfly.top

TypeScript ..... 212
来源：http://onw.yonumen.top

Java ........... 212
来源：http://stn.chenlongwang.top

Go ............. 212
来源：http://xkl.shanyushiyangkeji.top

Ruby ........... 212
来源：http://nba.quarkkingdee.top

C# ............. 212
来源：http://qnp.uphjek.com

C .............. 30
来源：http://lca.dianchejie.cn

C++ ............ 30
来源：http://uyu.dianchejie.cn

SQL ............ 90
来源：http://rnu.hysaishi.cn

Bash ........... 80
来源：http://fwo.pengpengdd.cyou

Kotlin ......... 15
来源：http://dex.tianlin.xyz

Swift .......... 15
来源：http://foh.ywan-chungtsiang.top

Lua ............ 10
来源：http://axy.zhixingplan.top

Perl ........... 10
来源：http://eah.zhijiandao.cn


<!-- 参考信息 -->