代发 wailian999

[T39] Lua：模式匹配
来源：http://zuu.jiagoushi.top

string.find(s, "%d+")
来源：http://riw.0kj1m.cn

[T40] Lua：元表
来源：http://tpc.hysaishi.cn

setmetatable({}, { __index = base })
来源：http://mot.shangyingyoupin.top

[T41] Perl：Hello World
来源：http://yqn.bjfxy.top

print "Hello\n";
来源：http://pjv.wangshuangyany.cn

[T42] Perl：变量类型
来源：http://wgt.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rlf.gotoacloud.top

[T43] Perl：字符串插值
来源：http://xlq.guannengcc.top

"值: $a"
来源：http://uwv.jyoumei.cn

[T44] Perl：条件
来源：http://djm.haohaochexian.top

if ($a > 0) { print "正"; }
来源：http://xmm.guannengcc.top

[T45] Perl：数组遍历
来源：http://bwd.zhengqikj.top

for my $x (@arr) { print $x; }
来源：http://dzl.fktsv.cn

[T46] Perl：哈希操作
来源：http://rpd.gotoacloud.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dgt.daria6918.cn

[T47] Perl：正则捕获
来源：http://dpx.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://jbx.zdbjq.cn

[T48] Perl：正则替换
来源：http://aje.cashguo.top

$s =~ s/old/new/g;
来源：http://fmf.redwolf501.top

[T49] Perl：函数
来源：http://tii.aibaodan.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dfm.shangyingyoupin.top

[T50] Perl：逐行读文件
来源：http://cll.xinyue.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://ojc.xinyue.icu

while (my $line = <$fh>) { print $line; }
来源：http://vuv.cdnleiting.top

[T51] Scala：Hello World
来源：http://rua.bbcook.cn

println("Hello")
来源：http://ulj.andypj.xyz

[T52] Scala：变量
来源：http://cdi.meibo888.top

val a = 1;  var b = 2
来源：http://hvz.cashguo.top

[T53] Scala：字符串插值
来源：http://twv.shzxlz.cn

s"值: $b"
来源：http://uee.nwbrower.top

[T54] Scala：集合映射
来源：http://chr.hongshengwenyu.top

List(1, 2, 3).map(_ * 2)
来源：http://yjd.yangfankeji.com

[T55] Scala：集合过滤
来源：http://skm.cucudq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://liz.yvedp.cn

[T56] Scala：样例类
来源：http://sbm.ppjwa.cn

case class User(name: String, age: Int)
来源：http://rlj.yj20258.top

[T57] Scala：模式匹配
来源：http://ztn.uphjek.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://oiw.yj20258888.top

[T58] Scala：函数定义
来源：http://dpa.jinyuanbaomall.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vhe.dianchejie.cn

[T59] Scala：循环
来源：http://wec.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://tjr.nanxinkj.top

[T60] Scala：折叠
来源：http://twk.shuidangran.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cpf.jinqigufen.top

================================================================================
来源：http://fij.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gal.zycfv.cn

================================================================================
来源：http://amj.havefunace.top

[U01] Py：创建虚拟环境
来源：http://ovc.iojbl.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ifu.yfazqb.com

[U02] Py：导出 / 安装依赖
来源：http://enm.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ibh.haohaochexian.top

[U03] Py：加载 .env 配置
来源：http://nyk.daxiang520.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xzv.jinqigufen.top

[U04] Py：变量调试打印
来源：http://uxd.jinqigfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xlr.epnwcf.com

[U05] Py：列表去重且保序
来源：http://msp.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://rkq.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://ubp.yongpay.top

{**a, **b}
来源：http://bbz.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://lng.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://asv.hesvh.cn

[U08] Py：展平二维列表
来源：http://ooe.yj20258888.top

[y for x in nested for y in x]
来源：http://jvr.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://inq.gotoacloud.top

max(d, key=d.get)
来源：http://hyp.yj20258888.top

[U10] Py：按值排序字典
来源：http://ari.pycfn.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ydo.xziqi.cn

[U11] Py：生成器表达式
来源：http://uwe.zhijiandao.cn

(x * 2 for x in arr)
来源：http://qgz.guowangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://xcs.redwolf501.top

Counter(arr).most_common(3)
来源：http://otb.52xcode.cn

[U13] Py：固定长度队列
来源：http://qjr.jqgufenzy.top

deque(maxlen=10)
来源：http://fnj.dianchejie.cn

[U14] Py：分组收集到列表
来源：http://juz.ydjk.org.cn

defaultdict(list)
来源：http://jgy.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://dhr.iojbl.cn

t = time.perf_counter()
来源：http://ira.xinyue.icu

[U16] Py：命令行参数解析
来源：http://wjv.zhixingplan.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ehx.guannengcc.top

[U17] Py：初始化日志
来源：http://vek.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://enb.yangfankeji.com

[U18] Py：预编译正则
来源：http://yyj.fanxiaobao.xyz

pat = re.compile(r"\d+")
来源：http://iug.zhongyouzk.top

[U19] Py：正则替换带回调
来源：http://ykd.fzhhl.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mzo.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://zmw.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://wea.hnqzz.top

[U21] Py：自定义上下文管理器
来源：http://dbz.sysykeji.top

@contextlib.contextmanager
来源：http://ivq.feifeiyinyue.top

[U22] Py：矩阵转置
来源：http://llj.zdbjq.cn

list(zip(*m))
来源：http://nzl.jqgufenzy.top

[U23] Py：分块读取大文件
来源：http://jfb.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pwu.chenjidiqi.icu

[U24] Py：路径操作
来源：http://asq.hnqzz.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ypk.shuidangran.top

[U25] Py：CSV 按字典读
来源：http://vnr.yanxiufei.cn

csv.DictReader(f)
来源：http://syo.316326.xyz

[U26] Py：并发下载
来源：http://seg.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cpc.hammf.cn

[U27] Py：异步 HTTP
来源：http://nbw.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://qqq.xziqi.cn

[U28] Py：类型别名
来源：http://wep.yj202588.top

UserId = int
来源：http://qss.guowangkeji.top

[U29] Py：属性校验
来源：http://akx.yangfankeji.com

@property 与 @x.setter 配合
来源：http://blf.gzhubu.top

[U30] Py：数据类
来源：http://rmk.fktsv.cn

@dataclass(slots=True)
来源：http://paq.jyoumei.cn

[U31] Py：单测
来源：http://qfe.zhijiandao.cn

python -m pytest -q
来源：http://xmb.chenlongwang.top

[U32] Py：代码格式化
来源：http://jlh.yuanzhike.top

ruff format . && ruff check --fix .
来源：http://lug.hywenlv.cn

[U33] Py：打包发布
来源：http://fcr.nwbrower.top

python -m build  （依赖 pyproject.toml）
来源：http://jkt.yangfankeji.com

[U34] Py：判断编码
来源：http://eap.fanxiaobao.xyz

chardet.detect(raw)
来源：http://gim.daria6918.cn

[U35] Py：发送邮件
来源：http://fey.hnqzz.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dza.yongpay.top

[U36] Py：定时任务
来源：http://pdv.havefunace.top

schedule.every(10).minutes.do(job)
来源：http://kqc.fzhhl.top

[U37] Py：读写 Excel
来源：http://tnn.zhongyouzk.top

pandas.read_excel / DataFrame.to_excel
来源：http://lwr.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://lhc.jiagoushi.top

Path(__file__).resolve().parent
来源：http://dhm.sweek.top

[U39] Py：判断是否在交互环境
来源：http://zpd.hysaishi.cn

sys.stdout.isatty()
来源：http://gkf.aizwys.cn

[U40] Py：打印到标准错误
来源：http://hvu.nanxuanxn.top

print("err", file=sys.stderr)
来源：http://vse.jianghu66.top

[U41] PHP：初始化 Composer 项目
来源：http://wqu.shangyingyoupin.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wvb.jinghuilouyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://aaf.zhongyouzk.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ppr.xinyue.icu

[U43] PHP：声明命名空间
来源：http://wdc.mhx1999.top

namespace App\Http;
来源：http://qwe.aibaodan.cn

[U44] PHP：开启严格类型
来源：http://udf.shuidangran.top

declare(strict_types=1);
来源：http://qcr.birdmap.top

[U45] PHP：类型声明与返回类型
来源：http://gsa.sufxvd.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://usa.tarul.cn

[U46] PHP：可空类型
来源：http://vye.daria6918.cn

?string $name = null
来源：http://nuy.hesvh.cn

[U47] PHP：联合类型
来源：http://pxf.jinyuanbaomall.cn

int|string $id
来源：http://xol.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://ixk.zhiwuduotai.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jom.epnwcf.com

[U49] PHP：只读属性
来源：http://hvk.sweek.top

public readonly string $name
来源：http://gid.vehdjk.com

[U50] PHP：构造器属性提升
来源：http://pss.jqgufenzy.top

public function __construct(private int $id) {}
来源：http://gdq.xylfe.cn

[U51] PHP：数组解构
来源：http://mvh.jlsjyb.cn

[$a, $b] = $arr;
来源：http://mxh.cdnleiting.top

[U52] PHP：箭头函数
来源：http://bqs.yj202588.top

$double = fn($x) => $x * 2;
来源：http://trn.yuxming.cn

[U53] PHP：空合并运算符
来源：http://wqz.hnxiangtu.top

$v = $a ?? $b ?? "default";
来源：http://qqr.dianchejie.cn

[U54] PHP：空安全调用
来源：http://fxu.iojbl.cn

$obj?->method()
来源：http://ceq.yvedp.cn

[U55] PHP：match 表达式
来源：http://ulq.0kj1m.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zci.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://lrj.tarul.cn

f(a: 1, b: 2)
来源：http://fgo.kuanghao11.cn

[U57] PHP：字符串插值
来源：http://lii.hfpthk.cn

"值: {$a}"
来源：http://zvu.dianchejie.cn

[U58] PHP：数组三件套
来源：http://ffm.sweek.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cej.fktsv.cn

[U59] PHP：自定义排序
来源：http://pjn.shzxlz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://njk.tanke756.top

[U60] PHP：JSON 编解码
来源：http://bdg.pengpengdd.cyou

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oui.gzhubu.top

[U61] PHP：正则
来源：http://gle.yuanzhike.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ztw.hysaishi.cn

[U62] PHP：日期对象
来源：http://iel.wangshuangyany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fib.guannengcc.top

[U63] PHP：文件读写
来源：http://dnz.hongshengwenyu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://erk.fktsv.cn

[U64] PHP：目录遍历
来源：http://wei.yj20258.top

glob("dir/*.php");  scandir("dir");
来源：http://jyr.wangshuangyany.cn

[U65] PHP：会话
来源：http://zpb.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://aly.gotoacloud.top

[U66] PHP：设置 Cookie
来源：http://igy.jiagoushi.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lfj.sufxvd.cn

[U67] PHP：处理文件上传
来源：http://jop.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://myd.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://rfm.yj202588.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://azt.kuanghao11.cn

[U69] PHP：PDO 预处理
来源：http://wft.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://scs.fengsongda.top

[U70] PHP：PDO 事务
来源：http://zzn.jinyuanbaomall.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ixz.redwolf501.top

[U71] PHP：抛出异常
来源：http://wlb.ywan-chungtsiang.top

throw new RuntimeException("失败", 500);
来源：http://hqi.sufxvd.cn

[U72] PHP：写错误日志
来源：http://fpe.kuanghao11.cn

error_log("失败: " . $e->getMessage());
来源：http://pht.dashuyun.cn

[U73] PHP：读取 ini 配置
来源：http://fil.tianlin.xyz

parse_ini_file("config.ini", true)
来源：http://lwl.sxryk.cn

[U74] PHP：读取环境变量
来源：http://odq.yfazqb.com

getenv("APP_ENV") ?: "production"
来源：http://gph.yuxming.cn

[U75] PHP：依赖注入
来源：http://rjp.ppjwa.cn

composer require psr/container
来源：http://est.guowangkeji.top

[U76] PHP：简单路由
来源：http://zuk.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eug.tanke756.top

[U77] PHP：模板渲染
来源：http://hcy.ybcxt.top

composer require twig/twig
来源：http://qgt.ehwqpu.com

[U78] PHP：单元测试
来源：http://vhl.cdnleiting.top

composer require --dev phpunit/phpunit
来源：http://tsb.shuidangran.top

[U79] PHP：静态分析
来源：http://ppd.hesvh.cn

composer require --dev phpstan/phpstan
来源：http://izl.jianghu66.top

[U80] PHP：代码规范修复
来源：http://gwg.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zev.uphjek.com

[U81] JS：初始化项目
来源：http://qos.iojbl.cn

npm init -y;  npm i express
来源：http://sei.bjfxy.top

[U82] JS：package.json 脚本
来源：http://sor.gaohongyu789.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ihz.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://mkd.hnxiangtu.top

export const a = 1;  import { a } from "./m.js";
来源：http://ykc.pycfn.com

[U84] JS：CommonJS 写法
来源：http://ufw.zhoulong.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://awc.fzhhl.top

[U85] JS：可选链
来源：http://jer.andypj.xyz

a?.b?.c
来源：http://piq.gogol.net.cn

[U86] JS：空值合并
来源：http://dgt.shanyushiyangtech.top

a ?? b
来源：http://urk.52xcode.cn

[U87] JS：解构默认值
来源：http://qvd.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://lzw.tianlin.xyz

[U88] JS：对象展开合并
来源：http://cks.nanxinkj.top

{ ...a, ...b }
来源：http://fpf.gogol.net.cn

[U89] JS：数组去重
来源：http://clo.pycfn.com

[...new Set(arr)]
来源：http://khe.xinyue.icu

[U90] JS：数字数组排序
来源：http://qcq.zhijiandao.cn

[...arr].sort((a, b) => a - b)
来源：http://wjj.shanyushiyangkeji.top

[U91] JS：对象键值遍历
来源：http://puo.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rzv.zhiwuduotai.top

[U92] JS：深拷贝
来源：http://hfb.jinghuilouyu.cn

structuredClone(obj)
来源：http://plw.hysaishi.cn

[U93] JS：模板字符串
来源：http://vny.ydzc1.top

`共 ${n} 条`
来源：http://ism.fengsongda.top

[U94] JS：箭头函数
来源：http://kfx.yj20258.top

const double = x => x * 2;
来源：http://ret.haohaochexian.top

[U95] JS：Promise 包装
来源：http://wkf.birdmap.top

new Promise((resolve, reject) => {})
来源：http://ksh.feifeiyinyue.top

[U96] JS：async/await 与异常
来源：http://cze.jyoumei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ogh.sweek.top

[U97] JS：并发请求
来源：http://zli.haohaochexian.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://oye.jiagoushi.top

[U98] JS：fetch 带 JSON
来源：http://huv.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vgr.aibaodan.cn

[U99] JS：事件监听
来源：http://ivy.uphjek.com

el.addEventListener("click", e => {})
来源：http://oek.jqgfzy.top

[U100] JS：DOM 查询
来源：http://vac.quarkkingdee.top

document.querySelector(".item")
来源：http://kgx.gzhubu.top

[U101] JS：classList 操作
来源：http://dbr.yfazqb.com

el.classList.toggle("active")
来源：http://tnf.iojbl.cn

[U102] JS：本地存储
来源：http://tnn.yj20258888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hmp.0kj1m.cn

[U103] JS：定时器
来源：http://jti.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://avz.svipenyu.cn

[U104] JS：防抖
来源：http://dsr.cqqwz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uva.xuetiantiany.cn

[U105] JS：节流
来源：http://cml.aibaodan.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iky.jlsjyb.cn

[U106] JS：日期格式化
来源：http://wzi.zhoulong.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fko.cheryme.top

[U107] JS：数字千分位
来源：http://cpy.gotoacloud.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cpq.nwbrower.top

[U108] JS：随机整数
来源：http://kal.wangdashe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rnc.yangfankeji.com

[U109] JS：数组分组
来源：http://pnz.shuidangran.top

Object.groupBy(arr, x => x.type)
来源：http://isi.yonumen.top

[U110] JS：数组分块
来源：http://hpi.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dvi.dianchejie.cn

[U111] JS：对象转 Map
来源：http://sld.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://jnf.zhengqikj.top

[U112] JS：字符串补位
来源：http://yff.guannengcc.top

"7".padStart(3, "0")
来源：http://tuh.hnxiangtu.top

[U113] JS：正则替换全部
来源：http://ebu.xylfe.cn

s.replaceAll("a", "b")
来源：http://mjl.yongpay.top

[U114] JS：JSON 深比较
来源：http://npn.redwolf501.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://obd.xinyue.icu

[U115] JS：生成 UUID
来源：http://jmy.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://amp.fzhhl.top

[U116] JS：类型检查（JSDoc）
来源：http://hef.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://zhv.bbcook.cn

[U117] JS：单元测试
来源：http://lsv.ydjk.org.cn

npm i -D vitest;  npx vitest
来源：http://rrj.hfpthk.cn

[U118] JS：开发服务器
来源：http://uyw.yvedp.cn

npm i -D vite;  npx vite
来源：http://ztv.cdnleiting.top

[U119] JS：生产构建
来源：http://rfo.wangdashe.top

npx vite build
来源：http://whw.fktsv.cn

[U120] JS：读取环境变量（Vite）
来源：http://onl.vqdsnc.cn

import.meta.env.VITE_API_URL
来源：http://vvg.bjfxy.top

================================================================================
来源：http://pxe.zhengqikj.top

统计汇总
来源：http://cuo.xylfe.cn

================================================================================
来源：http://rid.ybcxt.top

按语言统计（条）：
来源：http://tnz.hammf.cn

Python ......... 252
来源：http://iko.ydzc1.top

PHP ............ 252
来源：http://ads.wangdashe.top

JavaScript ..... 252
来源：http://llv.wangdashe.top

TypeScript ..... 212
来源：http://esj.yfazqb.com

Java ........... 212
来源：http://ljb.yongpay.top

Go ............. 212
来源：http://yzb.ywan-chungtsiang.top

Ruby ........... 212
来源：http://oog.9152youxi.cn

C# ............. 212
来源：http://yvj.yonumen.top


<!-- 参考信息 -->