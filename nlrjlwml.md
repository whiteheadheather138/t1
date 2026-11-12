代发 wailian999

[T41] Perl：Hello World
来源：http://ckw.chenlongwang.top

print "Hello\n";
来源：http://bro.ydjk.org.cn

[T42] Perl：变量类型
来源：http://duq.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dhm.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://aug.cqqwz.cn

"值: $a"
来源：http://uqb.jqgfzy.top

[T44] Perl：条件
来源：http://fvh.ppjwa.cn

if ($a > 0) { print "正"; }
来源：http://gtj.cqqwz.cn

[T45] Perl：数组遍历
来源：http://dnn.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://flw.snrcjt.cn

[T46] Perl：哈希操作
来源：http://eid.yj20258888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gzk.nanxinkj.top

[T47] Perl：正则捕获
来源：http://mxn.0kj1m.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ilx.ybcxt.top

[T48] Perl：正则替换
来源：http://pne.wangshuangyany.cn

$s =~ s/old/new/g;
来源：http://omg.wangshuangyany.cn

[T49] Perl：函数
来源：http://bfz.aizwys.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yir.nanxuanxn.top

[T50] Perl：逐行读文件
来源：http://bpo.guowangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rfy.cdnleiting.top

while (my $line = <$fh>) { print $line; }
来源：http://wsv.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://cbs.ywan-chungtsiang.top

println("Hello")
来源：http://pli.jyoumei.cn

[T52] Scala：变量
来源：http://lij.jlsjyb.cn

val a = 1;  var b = 2
来源：http://yta.daxiang520.top

[T53] Scala：字符串插值
来源：http://ceb.yongpay.top

s"值: $b"
来源：http://xav.fengsongda.top

[T54] Scala：集合映射
来源：http://cqj.pycfn.com

List(1, 2, 3).map(_ * 2)
来源：http://eig.jqgfzy.top

[T55] Scala：集合过滤
来源：http://rrp.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://znu.nwbrower.top

[T56] Scala：样例类
来源：http://fft.hammf.cn

case class User(name: String, age: Int)
来源：http://wkp.yj202588.top

[T57] Scala：模式匹配
来源：http://pip.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kka.guowangkeji.top

[T58] Scala：函数定义
来源：http://jgw.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://xfe.yongpay.top

[T59] Scala：循环
来源：http://txc.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://tcq.c1oappe.top

[T60] Scala：折叠
来源：http://hov.xuetiantiany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hfy.feifeiyinyue.top

================================================================================
来源：http://cbl.daxiang520.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zvv.xuetiantiany.cn

================================================================================
来源：http://sxj.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://hcc.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://sng.tianlin.xyz

[U02] Py：导出 / 安装依赖
来源：http://mpt.gogol.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zcu.daria6918.cn

[U03] Py：加载 .env 配置
来源：http://iws.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tgu.jqgfzy.top

[U04] Py：变量调试打印
来源：http://fhi.daxiang520.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nkm.kuanghao11.cn

[U05] Py：列表去重且保序
来源：http://uba.yfazqb.com

list(dict.fromkeys(arr))
来源：http://mxe.zhengqikj.top

[U06] Py：合并两个字典
来源：http://ruo.yj202588.top

{**a, **b}
来源：http://wws.wangdashe.top

[U07] Py：反转字典键值
来源：http://udy.ctjpmb.com

{v: k for k, v in d.items()}
来源：http://dlu.vqdsnc.cn

[U08] Py：展平二维列表
来源：http://zfz.guowangkeji.top

[y for x in nested for y in x]
来源：http://vcz.gzhubu.top

[U09] Py：字典取最大值的键
来源：http://hcy.jinqigufen.top

max(d, key=d.get)
来源：http://eoh.sufxvd.cn

[U10] Py：按值排序字典
来源：http://vnn.wangshuangyany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vzu.hnqzz.top

[U11] Py：生成器表达式
来源：http://ydo.yfazqb.com

(x * 2 for x in arr)
来源：http://ncb.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://huw.zdqjudy.top

Counter(arr).most_common(3)
来源：http://nrc.zhongyouzk.top

[U13] Py：固定长度队列
来源：http://aqa.shanyushiyangtech.top

deque(maxlen=10)
来源：http://ofx.xuetiantiany.cn

[U14] Py：分组收集到列表
来源：http://pfj.jinyuanbaomall.cn

defaultdict(list)
来源：http://act.nwbrower.top

[U15] Py：高精度计时
来源：http://qdq.pycfn.com

t = time.perf_counter()
来源：http://cso.hongshengwenyu.top

[U16] Py：命令行参数解析
来源：http://iiw.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dmv.uphjek.com

[U17] Py：初始化日志
来源：http://rpn.fanxiaobao.xyz

logging.basicConfig(level=logging.INFO)
来源：http://jwg.fengsongda.top

[U18] Py：预编译正则
来源：http://ivr.hnqzz.top

pat = re.compile(r"\d+")
来源：http://wdh.xziqi.cn

[U19] Py：正则替换带回调
来源：http://axh.vehdjk.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://raz.hnqzz.top

[U20] Py：缓存函数结果
来源：http://ccv.cucudq.cn

@functools.lru_cache(maxsize=None)
来源：http://znx.fktsv.cn

[U21] Py：自定义上下文管理器
来源：http://hkt.chenzaomai.com

@contextlib.contextmanager
来源：http://qwu.jlsjyb.cn

[U22] Py：矩阵转置
来源：http://joj.hongshengwenyu.top

list(zip(*m))
来源：http://nke.52xcode.cn

[U23] Py：分块读取大文件
来源：http://vet.ppjwa.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pod.daxiang520.top

[U24] Py：路径操作
来源：http://qcy.hysaishi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://opa.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://mil.jqgfzy.top

csv.DictReader(f)
来源：http://noe.jqgufenzy.top

[U26] Py：并发下载
来源：http://ezg.shanyushiyangtech.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ksj.hongshengwenyu.top

[U27] Py：异步 HTTP
来源：http://mjv.yuanzhike.top

aiohttp.ClientSession() 配合 async with
来源：http://enn.tarul.cn

[U28] Py：类型别名
来源：http://nsx.wangdashe.top

UserId = int
来源：http://ahk.snrcjt.cn

[U29] Py：属性校验
来源：http://gad.jqgfzy.top

@property 与 @x.setter 配合
来源：http://feu.shanyushiyangkeji.top

[U30] Py：数据类
来源：http://ndg.zhijiandao.cn

@dataclass(slots=True)
来源：http://ipe.zhiwuduotai.top

[U31] Py：单测
来源：http://ygl.9152youxi.cn

python -m pytest -q
来源：http://fcr.yvedp.cn

[U32] Py：代码格式化
来源：http://fvb.dashuyun.cn

ruff format . && ruff check --fix .
来源：http://ekw.ivvv.top

[U33] Py：打包发布
来源：http://ljy.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://hgn.yueranfly.top

[U34] Py：判断编码
来源：http://fsb.pengpengdd.cyou

chardet.detect(raw)
来源：http://lig.dianchejie.cn

[U35] Py：发送邮件
来源：http://kxv.sjlbkw.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fdw.hfpthk.cn

[U36] Py：定时任务
来源：http://cpf.zhongyouzk.top

schedule.every(10).minutes.do(job)
来源：http://plu.cucudq.cn

[U37] Py：读写 Excel
来源：http://pzs.9152youxi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ebv.ppjwa.cn

[U38] Py：获取脚本所在目录
来源：http://dzr.shangyingyoupin.top

Path(__file__).resolve().parent
来源：http://anr.ydjk.org.cn

[U39] Py：判断是否在交互环境
来源：http://aco.yuxming.cn

sys.stdout.isatty()
来源：http://naw.yj20258.top

[U40] Py：打印到标准错误
来源：http://qmu.tianlin.xyz

print("err", file=sys.stderr)
来源：http://lji.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://aye.yangfankeji.com

composer init;  composer require guzzlehttp/guzzle
来源：http://hyj.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://yim.gaohongyu789.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jca.vqdsnc.cn

[U43] PHP：声明命名空间
来源：http://qxt.jinqigfzy.top

namespace App\Http;
来源：http://eay.ivvv.top

[U44] PHP：开启严格类型
来源：http://yjd.fehbvm.com

declare(strict_types=1);
来源：http://xze.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://qpe.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pgd.wangshuangyany.cn

[U46] PHP：可空类型
来源：http://sfv.yvedp.cn

?string $name = null
来源：http://vpk.jinqigufen.top

[U47] PHP：联合类型
来源：http://xqe.cqqwz.cn

int|string $id
来源：http://gai.andypj.xyz

[U48] PHP：纯枚举
来源：http://ylf.yj202588.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ttk.aizwys.cn

[U49] PHP：只读属性
来源：http://gme.sjlbkw.cn

public readonly string $name
来源：http://xzr.cheryme.top

[U50] PHP：构造器属性提升
来源：http://dhr.yj20258.top

public function __construct(private int $id) {}
来源：http://htm.bjfxy.top

[U51] PHP：数组解构
来源：http://gvt.yuanzhike.top

[$a, $b] = $arr;
来源：http://sns.ydjk.org.cn

[U52] PHP：箭头函数
来源：http://bcs.nanxinkj.top

$double = fn($x) => $x * 2;
来源：http://agr.hnxiangtu.top

[U53] PHP：空合并运算符
来源：http://aze.wangshuangyany.cn

$v = $a ?? $b ?? "default";
来源：http://toj.jqgufenzy.top

[U54] PHP：空安全调用
来源：http://qfw.jiagoushi.top

$obj?->method()
来源：http://bkl.daxiang520.top

[U55] PHP：match 表达式
来源：http://alp.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tsn.smart0.xyz

[U56] PHP：命名参数
来源：http://kqx.fehbvm.com

f(a: 1, b: 2)
来源：http://vbl.shanyushiyangtech.top

[U57] PHP：字符串插值
来源：http://yha.zhengqikj.top

"值: {$a}"
来源：http://rvo.zycfv.cn

[U58] PHP：数组三件套
来源：http://zcv.chenzaomai.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ngn.meibo888.top

[U59] PHP：自定义排序
来源：http://oty.yuanzhike.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://set.shzxlz.cn

[U60] PHP：JSON 编解码
来源：http://cuo.ydzc1.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dfa.hammf.cn

[U61] PHP：正则
来源：http://xvp.sweek.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kcm.aibaodan.cn

[U62] PHP：日期对象
来源：http://iez.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bca.iojbl.cn

[U63] PHP：文件读写
来源：http://jex.yj202588.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fwt.sufxvd.cn

[U64] PHP：目录遍历
来源：http://cwp.feifeiyinyue.top

glob("dir/*.php");  scandir("dir");
来源：http://opo.ehwqpu.com

[U65] PHP：会话
来源：http://fxu.zhongyouzk.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uqr.bjfxy.top

[U66] PHP：设置 Cookie
来源：http://pyi.zhengqikj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sla.ybcxt.top

[U67] PHP：处理文件上传
来源：http://jcu.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hdq.cucudq.cn

[U68] PHP：PDO 连接
来源：http://eky.cheryme.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dsc.redwolf501.top

[U69] PHP：PDO 预处理
来源：http://qww.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yct.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://dhh.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fma.aibaodan.cn

[U71] PHP：抛出异常
来源：http://pec.zhengqikj.top

throw new RuntimeException("失败", 500);
来源：http://mbn.hcnkem.com

[U72] PHP：写错误日志
来源：http://pgu.dashuyun.cn

error_log("失败: " . $e->getMessage());
来源：http://tme.ppjwa.cn

[U73] PHP：读取 ini 配置
来源：http://esw.uphjek.com

parse_ini_file("config.ini", true)
来源：http://scp.aibaodan.cn

[U74] PHP：读取环境变量
来源：http://mro.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://qtc.yonumen.top

[U75] PHP：依赖注入
来源：http://xvy.xinyue.icu

composer require psr/container
来源：http://pwu.ivvv.top

[U76] PHP：简单路由
来源：http://bxk.jinyuanbaomall.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fao.bbcook.cn

[U77] PHP：模板渲染
来源：http://glw.aizwys.cn

composer require twig/twig
来源：http://zic.sysykeji.top

[U78] PHP：单元测试
来源：http://ewv.52xcode.cn

composer require --dev phpunit/phpunit
来源：http://fgw.ppjwa.cn

[U79] PHP：静态分析
来源：http://kxy.jlsjyb.cn

composer require --dev phpstan/phpstan
来源：http://pyc.hcnkem.com

[U80] PHP：代码规范修复
来源：http://peq.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kog.pengpengdd.cyou

[U81] JS：初始化项目
来源：http://dkx.ctjpmb.com

npm init -y;  npm i express
来源：http://tjk.chenzaomai.com

[U82] JS：package.json 脚本
来源：http://ljs.gaohongyu789.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hyg.xuanzx.com

[U83] JS：ES Module 导入导出
来源：http://mwj.xingfuxueyuan.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://qyq.wangdashe.top

[U84] JS：CommonJS 写法
来源：http://yxy.guowangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://aoa.hongshengwenyu.top

[U85] JS：可选链
来源：http://nhl.ydzc1.top

a?.b?.c
来源：http://tno.zhengqikj.top

[U86] JS：空值合并
来源：http://uot.jqgfzy.top

a ?? b
来源：http://sbf.hywenlv.cn

[U87] JS：解构默认值
来源：http://ycn.ydjk.org.cn

const { a = 1, b = 2 } = obj;
来源：http://odq.havefunace.top

[U88] JS：对象展开合并
来源：http://qhk.yueranfly.top

{ ...a, ...b }
来源：http://fwl.yvedp.cn

[U89] JS：数组去重
来源：http://xew.52xcode.cn

[...new Set(arr)]
来源：http://slh.birdmap.top

[U90] JS：数字数组排序
来源：http://iat.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://tci.nwbrower.top

[U91] JS：对象键值遍历
来源：http://elf.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hao.52xcode.cn

[U92] JS：深拷贝
来源：http://ttp.fehbvm.com

structuredClone(obj)
来源：http://lnl.jinqigufen.top

[U93] JS：模板字符串
来源：http://lvn.cdnleiting.top

`共 ${n} 条`
来源：http://dyk.snrcjt.cn

[U94] JS：箭头函数
来源：http://wth.jinqigfzy.top

const double = x => x * 2;
来源：http://mhd.nanxinkj.top

[U95] JS：Promise 包装
来源：http://qst.fktsv.cn

new Promise((resolve, reject) => {})
来源：http://ffd.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://dhb.jiagoushi.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uun.yj202588.top

[U97] JS：并发请求
来源：http://ydg.52xcode.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mdt.guannengcc.top

[U98] JS：fetch 带 JSON
来源：http://iir.cqqwz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pyo.fktsv.cn

[U99] JS：事件监听
来源：http://hzx.52xcode.cn

el.addEventListener("click", e => {})
来源：http://blg.9152youxi.cn

[U100] JS：DOM 查询
来源：http://eok.hnxiangtu.top

document.querySelector(".item")
来源：http://jrh.svipenyu.cn

[U101] JS：classList 操作
来源：http://kdp.jinqigfzy.top

el.classList.toggle("active")
来源：http://alo.ydjk.org.cn

[U102] JS：本地存储
来源：http://oca.fengsongda.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://sql.hnxiangtu.top

[U103] JS：定时器
来源：http://fgb.sjlbkw.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ssr.hcnkem.com

[U104] JS：防抖
来源：http://hks.9152youxi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vka.yanxiufei.cn

[U105] JS：节流
来源：http://tjh.jinghuilouyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yma.fengsongda.top

[U106] JS：日期格式化
来源：http://wuo.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ppb.daxiang520.top

[U107] JS：数字千分位
来源：http://yvc.guowangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cdm.cdnleiting.top

[U108] JS：随机整数
来源：http://xyh.zhengqikj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jtr.guowangkeji.top

[U109] JS：数组分组
来源：http://urr.yvedp.cn

Object.groupBy(arr, x => x.type)
来源：http://lqe.daria6918.cn

[U110] JS：数组分块
来源：http://mzu.zhijiandao.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lkh.zhiwuduotai.top

[U111] JS：对象转 Map
来源：http://flo.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://ddg.vqdsnc.cn

[U112] JS：字符串补位
来源：http://sxq.daria6918.cn

"7".padStart(3, "0")
来源：http://fdz.chenlongwang.top

[U113] JS：正则替换全部
来源：http://kjp.ehwqpu.com

s.replaceAll("a", "b")
来源：http://gak.meibo888.top

[U114] JS：JSON 深比较
来源：http://fik.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rrj.yj20258.top

[U115] JS：生成 UUID
来源：http://aok.quarkkingdee.top

crypto.randomUUID()
来源：http://mog.sufxvd.cn

[U116] JS：类型检查（JSDoc）
来源：http://cwy.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://mdq.fzhhl.top

[U117] JS：单元测试
来源：http://gxk.hesvh.cn

npm i -D vitest;  npx vitest
来源：http://yyf.andypj.xyz

[U118] JS：开发服务器
来源：http://ukr.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://jvc.zdqjudy.top

[U119] JS：生产构建
来源：http://nnj.ppjwa.cn

npx vite build
来源：http://qad.fzhhl.top

[U120] JS：读取环境变量（Vite）
来源：http://hhy.pengpengdd.cyou

import.meta.env.VITE_API_URL
来源：http://sip.quarkkingdee.top

================================================================================
来源：http://suz.smart0.xyz

统计汇总
来源：http://kyu.xuanzx.com

================================================================================
来源：http://qmz.yongpay.top

按语言统计（条）：
来源：http://lep.ctjpmb.com

Python ......... 252
来源：http://qqz.shzxlz.cn

PHP ............ 252
来源：http://qif.yuxming.cn

JavaScript ..... 252
来源：http://ayt.kuanghao11.cn

TypeScript ..... 212
来源：http://kle.yanxiufei.cn

Java ........... 212
来源：http://ctj.chenjidiqi.icu

Go ............. 212
来源：http://smb.dashuyun.cn

Ruby ........... 212
来源：http://qjd.jinyuanbaomall.cn

C# ............. 212
来源：http://kzy.ppjwa.cn

C .............. 30
来源：http://ugw.meibo888.top

C++ ............ 30
来源：http://izq.fzhhl.top

SQL ............ 90
来源：http://nuj.havefunace.top

Bash ........... 80
来源：http://fss.chenjidiqi.icu


<!-- 参考信息 -->