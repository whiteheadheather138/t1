代发 wailian999

[T33] Lua：表（数组）
来源：http://vax.hysaishi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xda.birdmap.top

[T34] Lua：遍历表
来源：http://mql.smart0.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://vjf.chenzaomai.com

[T35] Lua：字典表
来源：http://xst.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://clv.bjfxy.top

[T36] Lua：函数
来源：http://tlw.316326.xyz

function add(a, b) return a + b end
来源：http://kqf.andypj.xyz

[T37] Lua：字符串拼接
来源：http://pub.xziqi.cn

"a" .. "b"
来源：http://wzj.316326.xyz

[T38] Lua：条件
来源：http://snp.redwolf501.top

if x > 0 then print("正") end
来源：http://col.yanxiufei.cn

[T39] Lua：模式匹配
来源：http://ypt.zhiwuduotai.top

string.find(s, "%d+")
来源：http://ojv.meibo888.top

[T40] Lua：元表
来源：http://tom.ppjwa.cn

setmetatable({}, { __index = base })
来源：http://hhv.wangdashe.top

[T41] Perl：Hello World
来源：http://twc.feifeiyinyue.top

print "Hello\n";
来源：http://fjl.52xcode.cn

[T42] Perl：变量类型
来源：http://sau.yfazqb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://feg.9152youxi.cn

[T43] Perl：字符串插值
来源：http://sog.chenzaomai.com

"值: $a"
来源：http://vab.quarkkingdee.top

[T44] Perl：条件
来源：http://nhi.yuanzhike.top

if ($a > 0) { print "正"; }
来源：http://ghw.dashuyun.cn

[T45] Perl：数组遍历
来源：http://xvt.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://xue.dianchejie.cn

[T46] Perl：哈希操作
来源：http://xwj.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hvj.dashuyun.cn

[T47] Perl：正则捕获
来源：http://uxe.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lus.yvedp.cn

[T48] Perl：正则替换
来源：http://fvf.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://wjy.hnqzz.top

[T49] Perl：函数
来源：http://glm.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yxu.bbcook.cn

[T50] Perl：逐行读文件
来源：http://ctq.ydzc1.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ffj.cucudq.cn

while (my $line = <$fh>) { print $line; }
来源：http://bdn.gaohongyu789.top

[T51] Scala：Hello World
来源：http://frl.316326.xyz

println("Hello")
来源：http://txg.zycfv.cn

[T52] Scala：变量
来源：http://hcw.xinyue.icu

val a = 1;  var b = 2
来源：http://afi.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://mat.chenjidiqi.icu

s"值: $b"
来源：http://wnr.gogol.net.cn

[T54] Scala：集合映射
来源：http://nal.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://pyn.jianghu66.top

[T55] Scala：集合过滤
来源：http://cpv.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://jom.bbcook.cn

[T56] Scala：样例类
来源：http://cfn.xingfuxueyuan.xyz

case class User(name: String, age: Int)
来源：http://lnn.yanxiufei.cn

[T57] Scala：模式匹配
来源：http://kaz.jinghuilouyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bgq.pycfn.com

[T58] Scala：函数定义
来源：http://qhl.smart0.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://efs.zhoulong.xyz

[T59] Scala：循环
来源：http://sid.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://nxj.fktsv.cn

[T60] Scala：折叠
来源：http://zwu.ehwqpu.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rtu.cucudq.cn

================================================================================
来源：http://ins.jqgufenzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://obt.guannengcc.top

================================================================================
来源：http://lwf.cqqwz.cn

[U01] Py：创建虚拟环境
来源：http://hlm.0kj1m.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cva.fehbvm.com

[U02] Py：导出 / 安装依赖
来源：http://igy.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://znd.wangdashe.top

[U03] Py：加载 .env 配置
来源：http://buf.zdqjudy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://eql.meibo888.top

[U04] Py：变量调试打印
来源：http://iad.fktsv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tws.yangfankeji.com

[U05] Py：列表去重且保序
来源：http://zyb.aizwys.cn

list(dict.fromkeys(arr))
来源：http://zma.fzhhl.top

[U06] Py：合并两个字典
来源：http://kiy.yanxiufei.cn

{**a, **b}
来源：http://wme.yuxming.cn

[U07] Py：反转字典键值
来源：http://nrd.sufxvd.cn

{v: k for k, v in d.items()}
来源：http://vrg.hesvh.cn

[U08] Py：展平二维列表
来源：http://oqb.xziqi.cn

[y for x in nested for y in x]
来源：http://awn.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://tpu.hnqzz.top

max(d, key=d.get)
来源：http://ppi.yuxming.cn

[U10] Py：按值排序字典
来源：http://ueo.zhongyouzk.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vee.hongshengwenyu.top

[U11] Py：生成器表达式
来源：http://gjg.jqgfzy.top

(x * 2 for x in arr)
来源：http://cla.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://iut.yj20258.top

Counter(arr).most_common(3)
来源：http://fql.fktsv.cn

[U13] Py：固定长度队列
来源：http://lnv.aizwys.cn

deque(maxlen=10)
来源：http://kom.fanxiaobao.xyz

[U14] Py：分组收集到列表
来源：http://dej.nwbrower.top

defaultdict(list)
来源：http://ssa.zhengqikj.top

[U15] Py：高精度计时
来源：http://hun.hywenlv.cn

t = time.perf_counter()
来源：http://ijp.yj20258888.top

[U16] Py：命令行参数解析
来源：http://fxa.zhoulong.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iuy.jinqigufen.top

[U17] Py：初始化日志
来源：http://wlj.shangyingyoupin.top

logging.basicConfig(level=logging.INFO)
来源：http://tws.daria6918.cn

[U18] Py：预编译正则
来源：http://gpt.haohaochexian.top

pat = re.compile(r"\d+")
来源：http://czs.yueranfly.top

[U19] Py：正则替换带回调
来源：http://wjx.zhaomingkeji.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xay.aizwys.cn

[U20] Py：缓存函数结果
来源：http://zxo.gotoacloud.top

@functools.lru_cache(maxsize=None)
来源：http://ogu.zhixingplan.top

[U21] Py：自定义上下文管理器
来源：http://nid.tianlin.xyz

@contextlib.contextmanager
来源：http://gaq.tarul.cn

[U22] Py：矩阵转置
来源：http://cmp.shzxlz.cn

list(zip(*m))
来源：http://dtq.hesvh.cn

[U23] Py：分块读取大文件
来源：http://oss.yuanzhike.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://brn.pengpengdd.cyou

[U24] Py：路径操作
来源：http://fbe.yj20258888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ptp.snrcjt.cn

[U25] Py：CSV 按字典读
来源：http://sod.bjfxy.top

csv.DictReader(f)
来源：http://zao.ywan-chungtsiang.top

[U26] Py：并发下载
来源：http://awr.xuetiantiany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kyt.yanxiufei.cn

[U27] Py：异步 HTTP
来源：http://cpf.nanxuanxn.top

aiohttp.ClientSession() 配合 async with
来源：http://pfv.aibaodan.cn

[U28] Py：类型别名
来源：http://hmu.hysaishi.cn

UserId = int
来源：http://xmz.hcnkem.com

[U29] Py：属性校验
来源：http://tln.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://wil.cheryme.top

[U30] Py：数据类
来源：http://qah.xylfe.cn

@dataclass(slots=True)
来源：http://iwf.yuanzhike.top

[U31] Py：单测
来源：http://jjx.jyoumei.cn

python -m pytest -q
来源：http://kyl.fktsv.cn

[U32] Py：代码格式化
来源：http://def.zhixingplan.top

ruff format . && ruff check --fix .
来源：http://hxu.xinyue.icu

[U33] Py：打包发布
来源：http://ntu.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://qbv.wangshuangyany.cn

[U34] Py：判断编码
来源：http://tiz.cucudq.cn

chardet.detect(raw)
来源：http://hyf.meibo888.top

[U35] Py：发送邮件
来源：http://uyu.snrcjt.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ajp.daxiang520.top

[U36] Py：定时任务
来源：http://mgq.ehwqpu.com

schedule.every(10).minutes.do(job)
来源：http://kea.hywenlv.cn

[U37] Py：读写 Excel
来源：http://ggx.yj20258.top

pandas.read_excel / DataFrame.to_excel
来源：http://ctt.hfpthk.cn

[U38] Py：获取脚本所在目录
来源：http://cpk.9152youxi.cn

Path(__file__).resolve().parent
来源：http://kre.ydzc1.top

[U39] Py：判断是否在交互环境
来源：http://zbe.fktsv.cn

sys.stdout.isatty()
来源：http://crp.cucudq.cn

[U40] Py：打印到标准错误
来源：http://lhh.kuanghao11.cn

print("err", file=sys.stderr)
来源：http://sdl.xuanzx.com

[U41] PHP：初始化 Composer 项目
来源：http://yzn.dashuyun.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yin.ydjk.org.cn

[U42] PHP：PSR-4 自动加载
来源：http://pto.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pvp.ppjwa.cn

[U43] PHP：声明命名空间
来源：http://hhi.0kj1m.cn

namespace App\Http;
来源：http://wld.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://qde.yangfankeji.com

declare(strict_types=1);
来源：http://tlw.yongpay.top

[U45] PHP：类型声明与返回类型
来源：http://ehu.quarkkingdee.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nsh.iojbl.cn

[U46] PHP：可空类型
来源：http://nsg.zhoulong.xyz

?string $name = null
来源：http://xwk.ehwqpu.com

[U47] PHP：联合类型
来源：http://ccr.jyoumei.cn

int|string $id
来源：http://fjz.0kj1m.cn

[U48] PHP：纯枚举
来源：http://wkl.guannengcc.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://huh.shzxlz.cn

[U49] PHP：只读属性
来源：http://cfs.guowangkeji.top

public readonly string $name
来源：http://gzf.yj20258.top

[U50] PHP：构造器属性提升
来源：http://zby.vqdsnc.cn

public function __construct(private int $id) {}
来源：http://uoq.gaohongyu789.top

[U51] PHP：数组解构
来源：http://hkb.c1oappe.top

[$a, $b] = $arr;
来源：http://dyz.wangdashe.top

[U52] PHP：箭头函数
来源：http://emx.yongpay.top

$double = fn($x) => $x * 2;
来源：http://hce.yvedp.cn

[U53] PHP：空合并运算符
来源：http://mme.jlsjyb.cn

$v = $a ?? $b ?? "default";
来源：http://zas.tian-w.cn

[U54] PHP：空安全调用
来源：http://neu.jiagoushi.top

$obj?->method()
来源：http://wyx.hammf.cn

[U55] PHP：match 表达式
来源：http://cie.yfazqb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://psn.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://vpj.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://ndv.ivvv.top

[U57] PHP：字符串插值
来源：http://deu.jinyuanbaomall.cn

"值: {$a}"
来源：http://hos.yfazqb.com

[U58] PHP：数组三件套
来源：http://yjd.epnwcf.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pcu.tian-w.cn

[U59] PHP：自定义排序
来源：http://vgn.fehbvm.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hfe.hysaishi.cn

[U60] PHP：JSON 编解码
来源：http://rfx.cheryme.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dvl.ppjwa.cn

[U61] PHP：正则
来源：http://vci.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hfo.fzhhl.top

[U62] PHP：日期对象
来源：http://xjh.gaohongyu789.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vot.cashguo.top

[U63] PHP：文件读写
来源：http://bju.shuidangran.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uts.xziqi.cn

[U64] PHP：目录遍历
来源：http://rmj.aibaodan.cn

glob("dir/*.php");  scandir("dir");
来源：http://ktr.yueranfly.top

[U65] PHP：会话
来源：http://jcb.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qkk.guowangkeji.top

[U66] PHP：设置 Cookie
来源：http://crd.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ecy.sxryk.cn

[U67] PHP：处理文件上传
来源：http://taq.jqgfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ypm.ehwqpu.com

[U68] PHP：PDO 连接
来源：http://ucl.9152youxi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sgd.jiagoushi.top

[U69] PHP：PDO 预处理
来源：http://xdm.gogol.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://llz.mhx1999.top

[U70] PHP：PDO 事务
来源：http://qim.nanxuanxn.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kcy.pengpengdd.cyou

[U71] PHP：抛出异常
来源：http://gmp.xziqi.cn

throw new RuntimeException("失败", 500);
来源：http://fsk.hnxiangtu.top

[U72] PHP：写错误日志
来源：http://dif.sufxvd.cn

error_log("失败: " . $e->getMessage());
来源：http://kvn.jinyuanbaomall.cn

[U73] PHP：读取 ini 配置
来源：http://urd.ywan-chungtsiang.top

parse_ini_file("config.ini", true)
来源：http://lcu.zhengqikj.top

[U74] PHP：读取环境变量
来源：http://yvq.fzhhl.top

getenv("APP_ENV") ?: "production"
来源：http://uyt.gaohongyu789.top

[U75] PHP：依赖注入
来源：http://jry.yongpay.top

composer require psr/container
来源：http://hrc.9152youxi.cn

[U76] PHP：简单路由
来源：http://jfk.meibo888.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mkm.snrcjt.cn

[U77] PHP：模板渲染
来源：http://ftr.cqqwz.cn

composer require twig/twig
来源：http://jsc.nanxuanxn.top

[U78] PHP：单元测试
来源：http://nze.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://dga.chenzaomai.com

[U79] PHP：静态分析
来源：http://etq.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://pjp.xylfe.cn

[U80] PHP：代码规范修复
来源：http://vxn.ivvv.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jpo.shangyingyoupin.top

[U81] JS：初始化项目
来源：http://hjv.snrcjt.cn

npm init -y;  npm i express
来源：http://sqp.shzxlz.cn

[U82] JS：package.json 脚本
来源：http://jfu.fengsongda.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hhd.yvedp.cn

[U83] JS：ES Module 导入导出
来源：http://cjs.jlsjyb.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ghp.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://plq.andypj.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://stv.jinqigfzy.top

[U85] JS：可选链
来源：http://goo.shanyushiyangtech.top

a?.b?.c
来源：http://grb.ctjpmb.com

[U86] JS：空值合并
来源：http://ots.bjfxy.top

a ?? b
来源：http://gct.xinyue.icu

[U87] JS：解构默认值
来源：http://dsn.zycfv.cn

const { a = 1, b = 2 } = obj;
来源：http://isq.yonumen.top

[U88] JS：对象展开合并
来源：http://bhk.guannengcc.top

{ ...a, ...b }
来源：http://jfb.havefunace.top

[U89] JS：数组去重
来源：http://tcg.sysykeji.top

[...new Set(arr)]
来源：http://hsy.316326.xyz

[U90] JS：数字数组排序
来源：http://vok.pycfn.com

[...arr].sort((a, b) => a - b)
来源：http://jbq.daria6918.cn

[U91] JS：对象键值遍历
来源：http://exy.hesvh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rtc.ppjwa.cn

[U92] JS：深拷贝
来源：http://uem.yongpay.top

structuredClone(obj)
来源：http://csv.hnqzz.top

[U93] JS：模板字符串
来源：http://gox.jinqigfzy.top

`共 ${n} 条`
来源：http://qzl.shanyushiyangkeji.top

[U94] JS：箭头函数
来源：http://nfn.uphjek.com

const double = x => x * 2;
来源：http://yef.0kj1m.cn

[U95] JS：Promise 包装
来源：http://cck.dashuyun.cn

new Promise((resolve, reject) => {})
来源：http://tcj.shangyingyoupin.top

[U96] JS：async/await 与异常
来源：http://yfu.kuanghao11.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gdp.hywenlv.cn

[U97] JS：并发请求
来源：http://atd.wangdashe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://elp.jinyuanbaomall.cn

[U98] JS：fetch 带 JSON
来源：http://efg.aizwys.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gaf.guowangkeji.top

[U99] JS：事件监听
来源：http://vki.zhixingplan.top

el.addEventListener("click", e => {})
来源：http://dow.gzhubu.top

[U100] JS：DOM 查询
来源：http://yfy.chenlongwang.top

document.querySelector(".item")
来源：http://ylm.gzhubu.top

[U101] JS：classList 操作
来源：http://gwy.ppjwa.cn

el.classList.toggle("active")
来源：http://ttq.zycfv.cn

[U102] JS：本地存储
来源：http://tyr.yuanzhike.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zng.jlsjyb.cn

[U103] JS：定时器
来源：http://cfe.gotoacloud.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xze.zhixingplan.top

[U104] JS：防抖
来源：http://meu.bbcook.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zdj.bbcook.cn

[U105] JS：节流
来源：http://pkw.ywan-chungtsiang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wjz.fehbvm.com

[U106] JS：日期格式化
来源：http://cht.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qcn.jqgufenzy.top

[U107] JS：数字千分位
来源：http://pkk.svipenyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nab.fengsongda.top

[U108] JS：随机整数
来源：http://wtn.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ywa.chenlongwang.top

[U109] JS：数组分组
来源：http://pqr.quarkkingdee.top

Object.groupBy(arr, x => x.type)
来源：http://ivb.smart0.xyz

[U110] JS：数组分块
来源：http://swh.sxryk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bxf.ybcxt.top

[U111] JS：对象转 Map
来源：http://fpg.hfpthk.cn

new Map(Object.entries(obj))
来源：http://nwx.yuanzhike.top

[U112] JS：字符串补位
来源：http://gwi.smart0.xyz

"7".padStart(3, "0")
来源：http://djj.zhongyouzk.top

[U113] JS：正则替换全部
来源：http://gtf.haohaochexian.top

s.replaceAll("a", "b")
来源：http://aee.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://rym.zhixingplan.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jzb.zhaomingkeji.xyz

[U115] JS：生成 UUID
来源：http://ehv.daxiang520.top

crypto.randomUUID()
来源：http://ayq.shzxlz.cn

[U116] JS：类型检查（JSDoc）
来源：http://onx.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://blp.ctjpmb.com

[U117] JS：单元测试
来源：http://uhd.fzhhl.top

npm i -D vitest;  npx vitest
来源：http://cgy.tian-w.cn

[U118] JS：开发服务器
来源：http://mxk.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://zdp.ydzc1.top

[U119] JS：生产构建
来源：http://aul.dianchejie.cn

npx vite build
来源：http://uvc.yongpay.top

[U120] JS：读取环境变量（Vite）
来源：http://kqo.jianghu66.top

import.meta.env.VITE_API_URL
来源：http://khr.ydzc1.top


<!-- 参考信息 -->