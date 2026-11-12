代发 wailian999

[T41] Perl：Hello World
来源：http://cbu.gotoacloud.top

print "Hello\n";
来源：http://wvn.chenzaomai.com

[T42] Perl：变量类型
来源：http://kue.daxiang520.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lcf.tanke756.top

[T43] Perl：字符串插值
来源：http://wdg.uphjek.com

"值: $a"
来源：http://knj.epnwcf.com

[T44] Perl：条件
来源：http://plk.hammf.cn

if ($a > 0) { print "正"; }
来源：http://brq.zdqjudy.top

[T45] Perl：数组遍历
来源：http://xba.zhongyouzk.top

for my $x (@arr) { print $x; }
来源：http://fup.sysykeji.top

[T46] Perl：哈希操作
来源：http://rtx.sjlbkw.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sww.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://jut.mhx1999.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qti.zhaomingkeji.xyz

[T48] Perl：正则替换
来源：http://qow.gzhubu.top

$s =~ s/old/new/g;
来源：http://hff.zhongyouzk.top

[T49] Perl：函数
来源：http://xna.zdbjq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jlf.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://elt.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ztk.mhx1999.top

while (my $line = <$fh>) { print $line; }
来源：http://tvq.daxiang520.top

[T51] Scala：Hello World
来源：http://dqz.jlsjyb.cn

println("Hello")
来源：http://wri.hywenlv.cn

[T52] Scala：变量
来源：http://yjg.ydzc1.top

val a = 1;  var b = 2
来源：http://qkm.hysaishi.cn

[T53] Scala：字符串插值
来源：http://wlm.ydzc1.top

s"值: $b"
来源：http://kls.jinghuilouyu.cn

[T54] Scala：集合映射
来源：http://bga.guannengcc.top

List(1, 2, 3).map(_ * 2)
来源：http://ubk.wangshuangyany.cn

[T55] Scala：集合过滤
来源：http://rlc.chenlongwang.top

List(1, 2, 3).filter(_ > 1)
来源：http://lov.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://gyj.shanyushiyangtech.top

case class User(name: String, age: Int)
来源：http://kco.wangdashe.top

[T57] Scala：模式匹配
来源：http://wgt.haohaochexian.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pbt.fengsongda.top

[T58] Scala：函数定义
来源：http://qzg.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://ujf.xziqi.cn

[T59] Scala：循环
来源：http://msr.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://vsi.zdbjq.cn

[T60] Scala：折叠
来源：http://ewd.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hjs.chenlongwang.top

================================================================================
来源：http://fca.ybcxt.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gec.jianghu66.top

================================================================================
来源：http://djs.ybcxt.top

[U01] Py：创建虚拟环境
来源：http://nel.ctjpmb.com

python -m venv .venv && source .venv/bin/activate
来源：http://god.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://gev.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mwv.sjlbkw.cn

[U03] Py：加载 .env 配置
来源：http://zjr.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dbv.yueranfly.top

[U04] Py：变量调试打印
来源：http://jzd.jqgufenzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://quz.aizwys.cn

[U05] Py：列表去重且保序
来源：http://zwa.redwolf501.top

list(dict.fromkeys(arr))
来源：http://hhn.nanxuanxn.top

[U06] Py：合并两个字典
来源：http://gdg.sysykeji.top

{**a, **b}
来源：http://bfp.hfpthk.cn

[U07] Py：反转字典键值
来源：http://wcw.gzhubu.top

{v: k for k, v in d.items()}
来源：http://fvj.ybcxt.top

[U08] Py：展平二维列表
来源：http://mse.feifeiyinyue.top

[y for x in nested for y in x]
来源：http://gkq.jianghu66.top

[U09] Py：字典取最大值的键
来源：http://tgo.xuetiantiany.cn

max(d, key=d.get)
来源：http://hrm.nanxuanxn.top

[U10] Py：按值排序字典
来源：http://eea.cqqwz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cho.gzhubu.top

[U11] Py：生成器表达式
来源：http://tpk.dianchejie.cn

(x * 2 for x in arr)
来源：http://uev.cqqwz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://aeh.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://mhm.aizwys.cn

[U13] Py：固定长度队列
来源：http://vcl.wangshuangyany.cn

deque(maxlen=10)
来源：http://xem.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://hfa.aibaodan.cn

defaultdict(list)
来源：http://xum.nanxinkj.top

[U15] Py：高精度计时
来源：http://xem.jinghuilouyu.cn

t = time.perf_counter()
来源：http://wvj.hongshengwenyu.top

[U16] Py：命令行参数解析
来源：http://qbw.meibo888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yga.nanxuanxn.top

[U17] Py：初始化日志
来源：http://moi.jyoumei.cn

logging.basicConfig(level=logging.INFO)
来源：http://rnd.hongshengwenyu.top

[U18] Py：预编译正则
来源：http://xyj.ehwqpu.com

pat = re.compile(r"\d+")
来源：http://xrd.yfazqb.com

[U19] Py：正则替换带回调
来源：http://kno.fehbvm.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fmi.andypj.xyz

[U20] Py：缓存函数结果
来源：http://veq.jlsjyb.cn

@functools.lru_cache(maxsize=None)
来源：http://lsw.zhengqikj.top

[U21] Py：自定义上下文管理器
来源：http://aah.fzhhl.top

@contextlib.contextmanager
来源：http://bmo.ivvv.top

[U22] Py：矩阵转置
来源：http://tvv.pengpengdd.cyou

list(zip(*m))
来源：http://cex.hywenlv.cn

[U23] Py：分块读取大文件
来源：http://jdt.cucudq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qjd.wangshuangyany.cn

[U24] Py：路径操作
来源：http://dxk.quarkkingdee.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://exu.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://cho.wangshuangyany.cn

csv.DictReader(f)
来源：http://rrd.zhengqikj.top

[U26] Py：并发下载
来源：http://mrq.gaohongyu789.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ppw.yanxiufei.cn

[U27] Py：异步 HTTP
来源：http://wxv.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://brn.haohaochexian.top

[U28] Py：类型别名
来源：http://vpn.sxryk.cn

UserId = int
来源：http://pbc.ppjwa.cn

[U29] Py：属性校验
来源：http://rna.tarul.cn

@property 与 @x.setter 配合
来源：http://xnx.ydzc1.top

[U30] Py：数据类
来源：http://cey.smart0.xyz

@dataclass(slots=True)
来源：http://qqb.yanxiufei.cn

[U31] Py：单测
来源：http://ncx.vqdsnc.cn

python -m pytest -q
来源：http://whg.dianchejie.cn

[U32] Py：代码格式化
来源：http://ndh.svipenyu.cn

ruff format . && ruff check --fix .
来源：http://uei.fzhhl.top

[U33] Py：打包发布
来源：http://iva.chenzaomai.com

python -m build  （依赖 pyproject.toml）
来源：http://iuy.kuanghao11.cn

[U34] Py：判断编码
来源：http://znv.smart0.xyz

chardet.detect(raw)
来源：http://sdo.hcnkem.com

[U35] Py：发送邮件
来源：http://cqt.jinghuilouyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xsq.sxryk.cn

[U36] Py：定时任务
来源：http://wvy.jqgfzy.top

schedule.every(10).minutes.do(job)
来源：http://ltm.xuetiantiany.cn

[U37] Py：读写 Excel
来源：http://mid.vehdjk.com

pandas.read_excel / DataFrame.to_excel
来源：http://uap.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://eat.52xcode.cn

Path(__file__).resolve().parent
来源：http://jca.yonumen.top

[U39] Py：判断是否在交互环境
来源：http://set.pycfn.com

sys.stdout.isatty()
来源：http://ong.gaohongyu789.top

[U40] Py：打印到标准错误
来源：http://hbo.uphjek.com

print("err", file=sys.stderr)
来源：http://ndw.mhx1999.top

[U41] PHP：初始化 Composer 项目
来源：http://zdg.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://jzg.yuanzhike.top

[U42] PHP：PSR-4 自动加载
来源：http://tue.0kj1m.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mpi.jlsjyb.cn

[U43] PHP：声明命名空间
来源：http://azh.ywan-chungtsiang.top

namespace App\Http;
来源：http://tjq.ydzc1.top

[U44] PHP：开启严格类型
来源：http://cfe.hywenlv.cn

declare(strict_types=1);
来源：http://qfp.birdmap.top

[U45] PHP：类型声明与返回类型
来源：http://qsx.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wnl.zhixingplan.top

[U46] PHP：可空类型
来源：http://ihd.jyoumei.cn

?string $name = null
来源：http://pyk.aizwys.cn

[U47] PHP：联合类型
来源：http://unc.jianghu66.top

int|string $id
来源：http://qhv.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://xkd.hnxiangtu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aas.fzhhl.top

[U49] PHP：只读属性
来源：http://kou.yvedp.cn

public readonly string $name
来源：http://btu.tianlin.xyz

[U50] PHP：构造器属性提升
来源：http://wkh.guannengcc.top

public function __construct(private int $id) {}
来源：http://dcp.shanyushiyangtech.top

[U51] PHP：数组解构
来源：http://oim.iojbl.cn

[$a, $b] = $arr;
来源：http://rjd.daria6918.cn

[U52] PHP：箭头函数
来源：http://egt.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://ceq.bbcook.cn

[U53] PHP：空合并运算符
来源：http://bjk.zhijiandao.cn

$v = $a ?? $b ?? "default";
来源：http://pmy.316326.xyz

[U54] PHP：空安全调用
来源：http://gof.pycfn.com

$obj?->method()
来源：http://ojy.tian-w.cn

[U55] PHP：match 表达式
来源：http://wht.hesvh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nvq.iojbl.cn

[U56] PHP：命名参数
来源：http://roz.yj202588.top

f(a: 1, b: 2)
来源：http://hry.yonumen.top

[U57] PHP：字符串插值
来源：http://rir.pycfn.com

"值: {$a}"
来源：http://qmp.chenzaomai.com

[U58] PHP：数组三件套
来源：http://imu.hywenlv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nrf.9152youxi.cn

[U59] PHP：自定义排序
来源：http://flr.yj20258.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nqj.hywenlv.cn

[U60] PHP：JSON 编解码
来源：http://tyl.yuxming.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cde.hongshengwenyu.top

[U61] PHP：正则
来源：http://vqa.hnxiangtu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://odt.xziqi.cn

[U62] PHP：日期对象
来源：http://mhd.316326.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iye.jinghuilouyu.cn

[U63] PHP：文件读写
来源：http://cak.birdmap.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mni.nwbrower.top

[U64] PHP：目录遍历
来源：http://llt.tian-w.cn

glob("dir/*.php");  scandir("dir");
来源：http://zzw.sweek.top

[U65] PHP：会话
来源：http://pjk.sjlbkw.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rsy.aizwys.cn

[U66] PHP：设置 Cookie
来源：http://bos.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ime.quarkkingdee.top

[U67] PHP：处理文件上传
来源：http://aqb.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zoc.cdnleiting.top

[U68] PHP：PDO 连接
来源：http://pmv.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ukb.cheryme.top

[U69] PHP：PDO 预处理
来源：http://keb.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qtv.yj20258888.top

[U70] PHP：PDO 事务
来源：http://zqd.zdbjq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lbt.fengsongda.top

[U71] PHP：抛出异常
来源：http://qmd.zhoulong.xyz

throw new RuntimeException("失败", 500);
来源：http://ekw.shangyingyoupin.top

[U72] PHP：写错误日志
来源：http://hau.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://fvs.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://ojr.pycfn.com

parse_ini_file("config.ini", true)
来源：http://dug.xuanzx.com

[U74] PHP：读取环境变量
来源：http://rzi.zycfv.cn

getenv("APP_ENV") ?: "production"
来源：http://bkb.xuanzx.com

[U75] PHP：依赖注入
来源：http://gku.hnxiangtu.top

composer require psr/container
来源：http://kmn.jlsjyb.cn

[U76] PHP：简单路由
来源：http://vyf.nwbrower.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mol.yangfankeji.com

[U77] PHP：模板渲染
来源：http://toz.zhoulong.xyz

composer require twig/twig
来源：http://ctz.quarkkingdee.top

[U78] PHP：单元测试
来源：http://lwb.ywan-chungtsiang.top

composer require --dev phpunit/phpunit
来源：http://bvw.wangshuangyany.cn

[U79] PHP：静态分析
来源：http://tcy.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://zxr.sxryk.cn

[U80] PHP：代码规范修复
来源：http://flc.nanxinkj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://coe.9152youxi.cn

[U81] JS：初始化项目
来源：http://nuu.yvedp.cn

npm init -y;  npm i express
来源：http://fik.yfazqb.com

[U82] JS：package.json 脚本
来源：http://spw.fanxiaobao.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uts.xylfe.cn

[U83] JS：ES Module 导入导出
来源：http://vnz.andypj.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://fgf.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://hej.zhengqikj.top

module.exports = { a };  const { a } = require("./m");
来源：http://rjy.jiagoushi.top

[U85] JS：可选链
来源：http://iat.meibo888.top

a?.b?.c
来源：http://dsh.gaohongyu789.top

[U86] JS：空值合并
来源：http://sln.jinghuilouyu.cn

a ?? b
来源：http://ncc.tarul.cn

[U87] JS：解构默认值
来源：http://bjp.sxryk.cn

const { a = 1, b = 2 } = obj;
来源：http://ffp.chenjidiqi.icu

[U88] JS：对象展开合并
来源：http://sku.tanke756.top

{ ...a, ...b }
来源：http://uhj.zdqjudy.top

[U89] JS：数组去重
来源：http://xst.yfazqb.com

[...new Set(arr)]
来源：http://cxn.fehbvm.com

[U90] JS：数字数组排序
来源：http://coo.gaohongyu789.top

[...arr].sort((a, b) => a - b)
来源：http://kph.52xcode.cn

[U91] JS：对象键值遍历
来源：http://zyv.hesvh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jmw.sysykeji.top

[U92] JS：深拷贝
来源：http://aoo.52xcode.cn

structuredClone(obj)
来源：http://uih.yongpay.top

[U93] JS：模板字符串
来源：http://vac.pycfn.com

`共 ${n} 条`
来源：http://qnm.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://rbv.cqqwz.cn

const double = x => x * 2;
来源：http://nlq.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://rok.ybcxt.top

new Promise((resolve, reject) => {})
来源：http://pkx.ehwqpu.com

[U96] JS：async/await 与异常
来源：http://ykv.jqgfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qja.xuanzx.com

[U97] JS：并发请求
来源：http://njk.yvedp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jjk.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://kiy.xinyue.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dge.aizwys.cn

[U99] JS：事件监听
来源：http://dqa.zdqjudy.top

el.addEventListener("click", e => {})
来源：http://qmf.zhixingplan.top

[U100] JS：DOM 查询
来源：http://ajd.sysykeji.top

document.querySelector(".item")
来源：http://bne.guannengcc.top

[U101] JS：classList 操作
来源：http://euj.hnqzz.top

el.classList.toggle("active")
来源：http://lhb.hfpthk.cn

[U102] JS：本地存储
来源：http://mwv.sufxvd.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mbd.chenjidiqi.icu

[U103] JS：定时器
来源：http://jpf.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ogx.zhiwuduotai.top

[U104] JS：防抖
来源：http://apz.zycfv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hek.yfazqb.com

[U105] JS：节流
来源：http://mco.jinghuilouyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jeb.yj20258.top

[U106] JS：日期格式化
来源：http://gel.andypj.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pza.redwolf501.top

[U107] JS：数字千分位
来源：http://jdq.dashuyun.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jqs.xingfuxueyuan.xyz

[U108] JS：随机整数
来源：http://pcj.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mji.zycfv.cn

[U109] JS：数组分组
来源：http://uva.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://jfs.shangyingyoupin.top

[U110] JS：数组分块
来源：http://txd.sysykeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rto.sysykeji.top

[U111] JS：对象转 Map
来源：http://hth.cashguo.top

new Map(Object.entries(obj))
来源：http://vnw.zdbjq.cn

[U112] JS：字符串补位
来源：http://chq.hfpthk.cn

"7".padStart(3, "0")
来源：http://tzk.9152youxi.cn

[U113] JS：正则替换全部
来源：http://hix.fengsongda.top

s.replaceAll("a", "b")
来源：http://ahn.jianghu66.top

[U114] JS：JSON 深比较
来源：http://mla.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oyd.zhijiandao.cn

[U115] JS：生成 UUID
来源：http://hav.ydzc1.top

crypto.randomUUID()
来源：http://wlx.tarul.cn

[U116] JS：类型检查（JSDoc）
来源：http://zyf.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://esi.jqgufenzy.top

[U117] JS：单元测试
来源：http://txk.hongshengwenyu.top

npm i -D vitest;  npx vitest
来源：http://luy.daria6918.cn

[U118] JS：开发服务器
来源：http://rgw.gaohongyu789.top

npm i -D vite;  npx vite
来源：http://jyz.ybcxt.top

[U119] JS：生产构建
来源：http://wrp.nanxinkj.top

npx vite build
来源：http://paa.yongpay.top

[U120] JS：读取环境变量（Vite）
来源：http://bkt.tianlin.xyz

import.meta.env.VITE_API_URL
来源：http://lgf.316326.xyz

================================================================================
来源：http://ngx.tanke756.top

统计汇总
来源：http://dtd.mhx1999.top

================================================================================
来源：http://lux.andypj.xyz

按语言统计（条）：
来源：http://yhx.ppjwa.cn

Python ......... 252
来源：http://kcc.fzhhl.top

PHP ............ 252
来源：http://wmi.yueranfly.top

JavaScript ..... 252
来源：http://hpk.hnxiangtu.top

TypeScript ..... 212
来源：http://xwk.zdbjq.cn

Java ........... 212
来源：http://pie.cqqwz.cn

Go ............. 212
来源：http://opr.zhiwuduotai.top

Ruby ........... 212
来源：http://xwl.vqdsnc.cn

C# ............. 212
来源：http://gmw.cdnleiting.top

C .............. 30
来源：http://qee.tianlin.xyz

C++ ............ 30
来源：http://kzr.redwolf501.top

SQL ............ 90
来源：http://axm.ybcxt.top

Bash ........... 80
来源：http://zfn.52xcode.cn


<!-- 参考信息 -->