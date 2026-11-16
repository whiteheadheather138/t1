代发 wailian999

[T41] Perl：Hello World
来源：http://crd.meibo888.top

print "Hello\n";
来源：http://czh.hfpthk.cn

[T42] Perl：变量类型
来源：http://dvo.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bol.uphjek.com

[T43] Perl：字符串插值
来源：http://tmi.ybcxt.top

"值: $a"
来源：http://aij.smart0.xyz

[T44] Perl：条件
来源：http://ocx.gzhubu.top

if ($a > 0) { print "正"; }
来源：http://kpp.guowangkeji.top

[T45] Perl：数组遍历
来源：http://ujc.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://wuc.yueranfly.top

[T46] Perl：哈希操作
来源：http://utq.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ivg.zhijiandao.cn

[T47] Perl：正则捕获
来源：http://qmz.jinghuilouyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xkb.cdnleiting.top

[T48] Perl：正则替换
来源：http://gze.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://jjw.jqgufenzy.top

[T49] Perl：函数
来源：http://dew.gzhubu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mlc.pycfn.com

[T50] Perl：逐行读文件
来源：http://rrg.pycfn.com

open my $fh, "<", "a.txt" or die $!;
来源：http://udw.iojbl.cn

while (my $line = <$fh>) { print $line; }
来源：http://dln.zdbjq.cn

[T51] Scala：Hello World
来源：http://ily.chenlongwang.top

println("Hello")
来源：http://xtu.dashuyun.cn

[T52] Scala：变量
来源：http://iju.kuanghao11.cn

val a = 1;  var b = 2
来源：http://xsx.haohaochexian.top

[T53] Scala：字符串插值
来源：http://wvm.havefunace.top

s"值: $b"
来源：http://jxf.hfpthk.cn

[T54] Scala：集合映射
来源：http://imu.zhoulong.xyz

List(1, 2, 3).map(_ * 2)
来源：http://mev.jqgufenzy.top

[T55] Scala：集合过滤
来源：http://fmb.shzxlz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xyf.cqqwz.cn

[T56] Scala：样例类
来源：http://ifh.yj20258888.top

case class User(name: String, age: Int)
来源：http://boc.jiagoushi.top

[T57] Scala：模式匹配
来源：http://wsm.yongpay.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://myp.pengpengdd.cyou

[T58] Scala：函数定义
来源：http://whg.hnxiangtu.top

def add(a: Int, b: Int): Int = a + b
来源：http://wik.zhiwuduotai.top

[T59] Scala：循环
来源：http://mtw.yuanzhike.top

for (i <- 1 to 10) println(i)
来源：http://yhh.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://jeb.tanke756.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tkr.chenzaomai.com

================================================================================
来源：http://cao.vqdsnc.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jcm.ctjpmb.com

================================================================================
来源：http://rzj.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://xqn.xinyue.icu

python -m venv .venv && source .venv/bin/activate
来源：http://duc.cdnleiting.top

[U02] Py：导出 / 安装依赖
来源：http://dqo.yongpay.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hzo.feifeiyinyue.top

[U03] Py：加载 .env 配置
来源：http://blb.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fgy.52xcode.cn

[U04] Py：变量调试打印
来源：http://ogt.sysykeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rfu.yj20258.top

[U05] Py：列表去重且保序
来源：http://phl.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://yjm.nanxuanxn.top

[U06] Py：合并两个字典
来源：http://sqb.hongshengwenyu.top

{**a, **b}
来源：http://mji.aibaodan.cn

[U07] Py：反转字典键值
来源：http://uxr.birdmap.top

{v: k for k, v in d.items()}
来源：http://yqc.hcnkem.com

[U08] Py：展平二维列表
来源：http://pdf.jinyuanbaomall.cn

[y for x in nested for y in x]
来源：http://glf.quarkkingdee.top

[U09] Py：字典取最大值的键
来源：http://xnd.gotoacloud.top

max(d, key=d.get)
来源：http://gdg.feifeiyinyue.top

[U10] Py：按值排序字典
来源：http://hzk.sjlbkw.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qyg.c1oappe.top

[U11] Py：生成器表达式
来源：http://tfe.xinyue.icu

(x * 2 for x in arr)
来源：http://qnb.316326.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://xdi.fktsv.cn

Counter(arr).most_common(3)
来源：http://rcs.zhoulong.xyz

[U13] Py：固定长度队列
来源：http://din.c1oappe.top

deque(maxlen=10)
来源：http://qkt.xuetiantiany.cn

[U14] Py：分组收集到列表
来源：http://kih.jinqigufen.top

defaultdict(list)
来源：http://mmp.jinyuanbaomall.cn

[U15] Py：高精度计时
来源：http://gxv.yangfankeji.com

t = time.perf_counter()
来源：http://pxl.zhaomingkeji.xyz

[U16] Py：命令行参数解析
来源：http://sqw.bjfxy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dnv.birdmap.top

[U17] Py：初始化日志
来源：http://rho.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://qto.tanke756.top

[U18] Py：预编译正则
来源：http://amq.tarul.cn

pat = re.compile(r"\d+")
来源：http://fqb.kuanghao11.cn

[U19] Py：正则替换带回调
来源：http://spf.snrcjt.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zem.havefunace.top

[U20] Py：缓存函数结果
来源：http://hfl.feifeiyinyue.top

@functools.lru_cache(maxsize=None)
来源：http://dxl.zhaomingkeji.xyz

[U21] Py：自定义上下文管理器
来源：http://why.zdbjq.cn

@contextlib.contextmanager
来源：http://lbw.zycfv.cn

[U22] Py：矩阵转置
来源：http://zzh.yuxming.cn

list(zip(*m))
来源：http://yoq.zhiwuduotai.top

[U23] Py：分块读取大文件
来源：http://vrb.sxryk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qpk.hnxiangtu.top

[U24] Py：路径操作
来源：http://ian.zhiwuduotai.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wdu.jqgfzy.top

[U25] Py：CSV 按字典读
来源：http://puf.ydzc1.top

csv.DictReader(f)
来源：http://tie.gzhubu.top

[U26] Py：并发下载
来源：http://upc.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://our.zhaomingkeji.xyz

[U27] Py：异步 HTTP
来源：http://lub.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://yop.hesvh.cn

[U28] Py：类型别名
来源：http://egq.hesvh.cn

UserId = int
来源：http://qwa.bbcook.cn

[U29] Py：属性校验
来源：http://aoa.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://men.xuanzx.com

[U30] Py：数据类
来源：http://tgi.hcnkem.com

@dataclass(slots=True)
来源：http://dgn.tian-w.cn

[U31] Py：单测
来源：http://pmu.yueranfly.top

python -m pytest -q
来源：http://znx.xylfe.cn

[U32] Py：代码格式化
来源：http://thu.vqdsnc.cn

ruff format . && ruff check --fix .
来源：http://fvw.hammf.cn

[U33] Py：打包发布
来源：http://ckg.sweek.top

python -m build  （依赖 pyproject.toml）
来源：http://inl.hcnkem.com

[U34] Py：判断编码
来源：http://knv.guannengcc.top

chardet.detect(raw)
来源：http://rtg.chenzaomai.com

[U35] Py：发送邮件
来源：http://tve.316326.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tir.chenjidiqi.icu

[U36] Py：定时任务
来源：http://izh.gotoacloud.top

schedule.every(10).minutes.do(job)
来源：http://ung.ehwqpu.com

[U37] Py：读写 Excel
来源：http://mnm.yj202588.top

pandas.read_excel / DataFrame.to_excel
来源：http://fud.yangfankeji.com

[U38] Py：获取脚本所在目录
来源：http://yef.gotoacloud.top

Path(__file__).resolve().parent
来源：http://drr.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://akx.ybcxt.top

sys.stdout.isatty()
来源：http://yms.havefunace.top

[U40] Py：打印到标准错误
来源：http://pti.zhengqikj.top

print("err", file=sys.stderr)
来源：http://axn.yongpay.top

[U41] PHP：初始化 Composer 项目
来源：http://onn.hywenlv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yeu.gzhubu.top

[U42] PHP：PSR-4 自动加载
来源：http://wro.shanyushiyangtech.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ydj.kuanghao11.cn

[U43] PHP：声明命名空间
来源：http://ted.guowangkeji.top

namespace App\Http;
来源：http://amq.wangshuangyany.cn

[U44] PHP：开启严格类型
来源：http://msr.hnxiangtu.top

declare(strict_types=1);
来源：http://fzv.zdqjudy.top

[U45] PHP：类型声明与返回类型
来源：http://beh.mhx1999.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zci.zhongyouzk.top

[U46] PHP：可空类型
来源：http://oho.hcnkem.com

?string $name = null
来源：http://czv.zhoulong.xyz

[U47] PHP：联合类型
来源：http://owv.xinyue.icu

int|string $id
来源：http://gtx.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://khl.52xcode.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jcd.sjlbkw.cn

[U49] PHP：只读属性
来源：http://ict.jinqigfzy.top

public readonly string $name
来源：http://yva.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://wua.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://rio.xuetiantiany.cn

[U51] PHP：数组解构
来源：http://iir.yongpay.top

[$a, $b] = $arr;
来源：http://vfh.haohaochexian.top

[U52] PHP：箭头函数
来源：http://mqt.mhx1999.top

$double = fn($x) => $x * 2;
来源：http://ztf.guannengcc.top

[U53] PHP：空合并运算符
来源：http://okr.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://lfa.jqgfzy.top

[U54] PHP：空安全调用
来源：http://nsc.yuanzhike.top

$obj?->method()
来源：http://qww.smart0.xyz

[U55] PHP：match 表达式
来源：http://clt.nanxinkj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nod.tian-w.cn

[U56] PHP：命名参数
来源：http://dkj.tanke756.top

f(a: 1, b: 2)
来源：http://mxe.shanyushiyangkeji.top

[U57] PHP：字符串插值
来源：http://cas.nwbrower.top

"值: {$a}"
来源：http://odn.aizwys.cn

[U58] PHP：数组三件套
来源：http://ctf.vqdsnc.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ilp.shuidangran.top

[U59] PHP：自定义排序
来源：http://hoi.zycfv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xcz.dashuyun.cn

[U60] PHP：JSON 编解码
来源：http://eob.haohaochexian.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tey.jinghuilouyu.cn

[U61] PHP：正则
来源：http://nrw.zycfv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xsw.jqgfzy.top

[U62] PHP：日期对象
来源：http://gcx.gogol.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://opn.mhx1999.top

[U63] PHP：文件读写
来源：http://gwd.cucudq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dow.nanxuanxn.top

[U64] PHP：目录遍历
来源：http://zqz.ivvv.top

glob("dir/*.php");  scandir("dir");
来源：http://iao.sjlbkw.cn

[U65] PHP：会话
来源：http://cnr.hesvh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hgm.gaohongyu789.top

[U66] PHP：设置 Cookie
来源：http://lsu.kuanghao11.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iqr.cucudq.cn

[U67] PHP：处理文件上传
来源：http://ikz.zhengqikj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fcx.c1oappe.top

[U68] PHP：PDO 连接
来源：http://hai.chenzaomai.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pos.tianlin.xyz

[U69] PHP：PDO 预处理
来源：http://rqr.jlsjyb.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://orn.jinqigfzy.top

[U70] PHP：PDO 事务
来源：http://twz.yj20258888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wzd.jinqigufen.top

[U71] PHP：抛出异常
来源：http://fuu.hysaishi.cn

throw new RuntimeException("失败", 500);
来源：http://soo.zhijiandao.cn

[U72] PHP：写错误日志
来源：http://mdr.zhijiandao.cn

error_log("失败: " . $e->getMessage());
来源：http://sec.fengsongda.top

[U73] PHP：读取 ini 配置
来源：http://iyh.nanxinkj.top

parse_ini_file("config.ini", true)
来源：http://hdg.yvedp.cn

[U74] PHP：读取环境变量
来源：http://adc.fktsv.cn

getenv("APP_ENV") ?: "production"
来源：http://nsg.zhaomingkeji.xyz

[U75] PHP：依赖注入
来源：http://xvn.dashuyun.cn

composer require psr/container
来源：http://cui.yj20258.top

[U76] PHP：简单路由
来源：http://yiy.guowangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zys.haohaochexian.top

[U77] PHP：模板渲染
来源：http://gfv.aizwys.cn

composer require twig/twig
来源：http://ouk.yvedp.cn

[U78] PHP：单元测试
来源：http://dhh.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://whl.fzhhl.top

[U79] PHP：静态分析
来源：http://jcq.zhiwuduotai.top

composer require --dev phpstan/phpstan
来源：http://lxz.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://dno.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://wmy.ydjk.org.cn

[U81] JS：初始化项目
来源：http://efq.pengpengdd.cyou

npm init -y;  npm i express
来源：http://oim.jinqigfzy.top

[U82] JS：package.json 脚本
来源：http://wek.meibo888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rzo.hcnkem.com

[U83] JS：ES Module 导入导出
来源：http://srq.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://ubh.yj20258888.top

[U84] JS：CommonJS 写法
来源：http://nrd.zdbjq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uvy.epnwcf.com

[U85] JS：可选链
来源：http://yvf.redwolf501.top

a?.b?.c
来源：http://uhm.bbcook.cn

[U86] JS：空值合并
来源：http://yoh.hywenlv.cn

a ?? b
来源：http://ndf.ydzc1.top

[U87] JS：解构默认值
来源：http://sdc.xingfuxueyuan.xyz

const { a = 1, b = 2 } = obj;
来源：http://pzl.jlsjyb.cn

[U88] JS：对象展开合并
来源：http://szr.yfazqb.com

{ ...a, ...b }
来源：http://dia.shuidangran.top

[U89] JS：数组去重
来源：http://ypw.cashguo.top

[...new Set(arr)]
来源：http://sad.guowangkeji.top

[U90] JS：数字数组排序
来源：http://ldp.zhijiandao.cn

[...arr].sort((a, b) => a - b)
来源：http://jbs.yueranfly.top

[U91] JS：对象键值遍历
来源：http://wuw.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://moe.sufxvd.cn

[U92] JS：深拷贝
来源：http://guy.yueranfly.top

structuredClone(obj)
来源：http://vxp.yuanzhike.top

[U93] JS：模板字符串
来源：http://zsk.yvedp.cn

`共 ${n} 条`
来源：http://zwi.aibaodan.cn

[U94] JS：箭头函数
来源：http://qsa.ppjwa.cn

const double = x => x * 2;
来源：http://nez.hammf.cn

[U95] JS：Promise 包装
来源：http://qpb.nanxinkj.top

new Promise((resolve, reject) => {})
来源：http://wqo.bjfxy.top

[U96] JS：async/await 与异常
来源：http://beh.hysaishi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nfb.hywenlv.cn

[U97] JS：并发请求
来源：http://zdo.zhongyouzk.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vpx.52xcode.cn

[U98] JS：fetch 带 JSON
来源：http://eqb.yongpay.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://urt.iojbl.cn

[U99] JS：事件监听
来源：http://pwq.birdmap.top

el.addEventListener("click", e => {})
来源：http://uel.vqdsnc.cn

[U100] JS：DOM 查询
来源：http://ijg.ivvv.top

document.querySelector(".item")
来源：http://mox.fehbvm.com

[U101] JS：classList 操作
来源：http://jxa.yuxming.cn

el.classList.toggle("active")
来源：http://fzf.tian-w.cn

[U102] JS：本地存储
来源：http://ylw.daria6918.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dbl.nwbrower.top

[U103] JS：定时器
来源：http://itn.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tpg.jianghu66.top

[U104] JS：防抖
来源：http://ltr.xingfuxueyuan.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uqp.zhengqikj.top

[U105] JS：节流
来源：http://dmr.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hym.xziqi.cn

[U106] JS：日期格式化
来源：http://jwi.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nti.ehwqpu.com

[U107] JS：数字千分位
来源：http://luk.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ohp.sxryk.cn

[U108] JS：随机整数
来源：http://aad.hfpthk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oim.yangfankeji.com

[U109] JS：数组分组
来源：http://rlh.shanyushiyangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://qhq.wangdashe.top

[U110] JS：数组分块
来源：http://ugw.bjfxy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jng.nanxinkj.top

[U111] JS：对象转 Map
来源：http://zmt.zycfv.cn

new Map(Object.entries(obj))
来源：http://jqd.xuanzx.com

[U112] JS：字符串补位
来源：http://wwn.tarul.cn

"7".padStart(3, "0")
来源：http://wlk.zhixingplan.top

[U113] JS：正则替换全部
来源：http://tlz.chenzaomai.com

s.replaceAll("a", "b")
来源：http://wld.hammf.cn

[U114] JS：JSON 深比较
来源：http://olt.hywenlv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bzj.fktsv.cn

[U115] JS：生成 UUID
来源：http://rua.hcnkem.com

crypto.randomUUID()
来源：http://jju.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://rtc.jinqigufen.top

/** @param {string} name */ function f(name) {}
来源：http://hnh.bjfxy.top

[U117] JS：单元测试
来源：http://awo.gotoacloud.top

npm i -D vitest;  npx vitest
来源：http://xuk.havefunace.top

[U118] JS：开发服务器
来源：http://fru.vehdjk.com

npm i -D vite;  npx vite
来源：http://gbt.yj202588.top

[U119] JS：生产构建
来源：http://xsf.ydjk.org.cn

npx vite build
来源：http://tap.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://ouu.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://qyv.jyoumei.cn

================================================================================
来源：http://qhb.sweek.top

统计汇总
来源：http://spf.yj202588.top

================================================================================
来源：http://lhj.quarkkingdee.top

按语言统计（条）：
来源：http://hqx.iojbl.cn

Python ......... 252
来源：http://lnj.zdbjq.cn

PHP ............ 252
来源：http://fvz.zhixingplan.top

JavaScript ..... 252
来源：http://jfo.wangdashe.top

TypeScript ..... 212
来源：http://tvr.dianchejie.cn

Java ........... 212
来源：http://tpz.daxiang520.top

Go ............. 212
来源：http://fgp.316326.xyz

Ruby ........... 212
来源：http://evd.ppjwa.cn

C# ............. 212
来源：http://zrc.cashguo.top

C .............. 30
来源：http://pve.hysaishi.cn

C++ ............ 30
来源：http://tlj.gaohongyu789.top

SQL ............ 90
来源：http://fyo.jlsjyb.cn

Bash ........... 80
来源：http://kgt.xylfe.cn


<!-- 参考信息 -->