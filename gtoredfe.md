代发 wailian999

[T39] Lua：模式匹配
来源：http://smg.cucudq.cn

string.find(s, "%d+")
来源：http://bmu.yonumen.top

[T40] Lua：元表
来源：http://hob.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://mpw.yongpay.top

[T41] Perl：Hello World
来源：http://kks.fanxiaobao.xyz

print "Hello\n";
来源：http://jda.havefunace.top

[T42] Perl：变量类型
来源：http://usj.vehdjk.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dgn.ppjwa.cn

[T43] Perl：字符串插值
来源：http://utr.hongshengwenyu.top

"值: $a"
来源：http://qwh.jinqigufen.top

[T44] Perl：条件
来源：http://mei.zhongyouzk.top

if ($a > 0) { print "正"; }
来源：http://rje.hesvh.cn

[T45] Perl：数组遍历
来源：http://vmy.quarkkingdee.top

for my $x (@arr) { print $x; }
来源：http://psd.zhiwuduotai.top

[T46] Perl：哈希操作
来源：http://fry.jinqigfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vqa.yvedp.cn

[T47] Perl：正则捕获
来源：http://ugt.feifeiyinyue.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bqw.ywan-chungtsiang.top

[T48] Perl：正则替换
来源：http://fef.sufxvd.cn

$s =~ s/old/new/g;
来源：http://rws.feifeiyinyue.top

[T49] Perl：函数
来源：http://gjz.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tfx.hfpthk.cn

[T50] Perl：逐行读文件
来源：http://kcj.ivvv.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ibm.yj20258.top

while (my $line = <$fh>) { print $line; }
来源：http://lpc.sweek.top

[T51] Scala：Hello World
来源：http://gcv.epnwcf.com

println("Hello")
来源：http://bwk.vehdjk.com

[T52] Scala：变量
来源：http://gdz.haohaochexian.top

val a = 1;  var b = 2
来源：http://jgf.sufxvd.cn

[T53] Scala：字符串插值
来源：http://tnm.jiagoushi.top

s"值: $b"
来源：http://nmc.zhiwuduotai.top

[T54] Scala：集合映射
来源：http://rew.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://nfz.feifeiyinyue.top

[T55] Scala：集合过滤
来源：http://vod.jinghuilouyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kgv.52xcode.cn

[T56] Scala：样例类
来源：http://hjm.yfazqb.com

case class User(name: String, age: Int)
来源：http://ywx.andypj.xyz

[T57] Scala：模式匹配
来源：http://wko.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://cbm.0kj1m.cn

[T58] Scala：函数定义
来源：http://pvv.yangfankeji.com

def add(a: Int, b: Int): Int = a + b
来源：http://jfo.ppjwa.cn

[T59] Scala：循环
来源：http://lkm.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://xtk.tianlin.xyz

[T60] Scala：折叠
来源：http://pid.xuanzx.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pfc.zhoulong.xyz

================================================================================
来源：http://yyk.yj202588.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tai.jqgfzy.top

================================================================================
来源：http://qyx.yueranfly.top

[U01] Py：创建虚拟环境
来源：http://cyq.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://uqb.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://rnq.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qln.yongpay.top

[U03] Py：加载 .env 配置
来源：http://xjq.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kjr.zhiwuduotai.top

[U04] Py：变量调试打印
来源：http://fur.meibo888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kmc.bjfxy.top

[U05] Py：列表去重且保序
来源：http://mta.yonumen.top

list(dict.fromkeys(arr))
来源：http://vvi.dianchejie.cn

[U06] Py：合并两个字典
来源：http://vvu.shzxlz.cn

{**a, **b}
来源：http://gcx.wangshuangyany.cn

[U07] Py：反转字典键值
来源：http://zfj.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://jrd.cdnleiting.top

[U08] Py：展平二维列表
来源：http://zfm.daxiang520.top

[y for x in nested for y in x]
来源：http://qum.uphjek.com

[U09] Py：字典取最大值的键
来源：http://epg.cashguo.top

max(d, key=d.get)
来源：http://liy.guowangkeji.top

[U10] Py：按值排序字典
来源：http://suc.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dyq.snrcjt.cn

[U11] Py：生成器表达式
来源：http://wxf.jqgufenzy.top

(x * 2 for x in arr)
来源：http://hyj.jqgufenzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://uyi.guannengcc.top

Counter(arr).most_common(3)
来源：http://rhd.hysaishi.cn

[U13] Py：固定长度队列
来源：http://yui.chenjidiqi.icu

deque(maxlen=10)
来源：http://zzt.9152youxi.cn

[U14] Py：分组收集到列表
来源：http://wdq.jqgfzy.top

defaultdict(list)
来源：http://llu.zhaomingkeji.xyz

[U15] Py：高精度计时
来源：http://myp.zhiwuduotai.top

t = time.perf_counter()
来源：http://zfg.xingfuxueyuan.xyz

[U16] Py：命令行参数解析
来源：http://omk.zhengqikj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hwj.hammf.cn

[U17] Py：初始化日志
来源：http://tfv.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://uat.yj202588.top

[U18] Py：预编译正则
来源：http://dzd.mhx1999.top

pat = re.compile(r"\d+")
来源：http://xza.aibaodan.cn

[U19] Py：正则替换带回调
来源：http://yai.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dwk.cucudq.cn

[U20] Py：缓存函数结果
来源：http://lzr.sysykeji.top

@functools.lru_cache(maxsize=None)
来源：http://ney.tian-w.cn

[U21] Py：自定义上下文管理器
来源：http://qza.gogol.net.cn

@contextlib.contextmanager
来源：http://gti.shanyushiyangtech.top

[U22] Py：矩阵转置
来源：http://pej.bbcook.cn

list(zip(*m))
来源：http://fsy.yongpay.top

[U23] Py：分块读取大文件
来源：http://qtp.jinyuanbaomall.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rok.jyoumei.cn

[U24] Py：路径操作
来源：http://ady.zhiwuduotai.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fol.nanxinkj.top

[U25] Py：CSV 按字典读
来源：http://kgc.fktsv.cn

csv.DictReader(f)
来源：http://gff.zhixingplan.top

[U26] Py：并发下载
来源：http://twu.jlsjyb.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zib.feifeiyinyue.top

[U27] Py：异步 HTTP
来源：http://tpa.hcnkem.com

aiohttp.ClientSession() 配合 async with
来源：http://paw.yj20258888.top

[U28] Py：类型别名
来源：http://dho.snrcjt.cn

UserId = int
来源：http://qns.haohaochexian.top

[U29] Py：属性校验
来源：http://exy.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://koh.bjfxy.top

[U30] Py：数据类
来源：http://tgp.gaohongyu789.top

@dataclass(slots=True)
来源：http://ajw.hongshengwenyu.top

[U31] Py：单测
来源：http://vmn.birdmap.top

python -m pytest -q
来源：http://xpc.vehdjk.com

[U32] Py：代码格式化
来源：http://kpv.guowangkeji.top

ruff format . && ruff check --fix .
来源：http://ugx.yonumen.top

[U33] Py：打包发布
来源：http://xwp.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://hzk.yueranfly.top

[U34] Py：判断编码
来源：http://rlc.svipenyu.cn

chardet.detect(raw)
来源：http://ttz.tianlin.xyz

[U35] Py：发送邮件
来源：http://ufp.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jtt.andypj.xyz

[U36] Py：定时任务
来源：http://uug.cdnleiting.top

schedule.every(10).minutes.do(job)
来源：http://fva.cdnleiting.top

[U37] Py：读写 Excel
来源：http://bim.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rft.jqgufenzy.top

[U38] Py：获取脚本所在目录
来源：http://ohm.meibo888.top

Path(__file__).resolve().parent
来源：http://crx.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://zko.epnwcf.com

sys.stdout.isatty()
来源：http://nci.fengsongda.top

[U40] Py：打印到标准错误
来源：http://eam.jiagoushi.top

print("err", file=sys.stderr)
来源：http://nig.tarul.cn

[U41] PHP：初始化 Composer 项目
来源：http://eyo.mhx1999.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uza.jianghu66.top

[U42] PHP：PSR-4 自动加载
来源：http://ywi.jlsjyb.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://alg.xingfuxueyuan.xyz

[U43] PHP：声明命名空间
来源：http://vot.ywan-chungtsiang.top

namespace App\Http;
来源：http://yvj.fzhhl.top

[U44] PHP：开启严格类型
来源：http://ovv.cqqwz.cn

declare(strict_types=1);
来源：http://vid.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://xvc.jinqigufen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ozu.feifeiyinyue.top

[U46] PHP：可空类型
来源：http://nek.redwolf501.top

?string $name = null
来源：http://bah.sysykeji.top

[U47] PHP：联合类型
来源：http://mfp.haohaochexian.top

int|string $id
来源：http://wyy.bjfxy.top

[U48] PHP：纯枚举
来源：http://tsa.ehwqpu.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zpv.hcnkem.com

[U49] PHP：只读属性
来源：http://wjb.sweek.top

public readonly string $name
来源：http://glk.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://cgt.hcnkem.com

public function __construct(private int $id) {}
来源：http://hbd.ehwqpu.com

[U51] PHP：数组解构
来源：http://uic.aibaodan.cn

[$a, $b] = $arr;
来源：http://raq.pengpengdd.cyou

[U52] PHP：箭头函数
来源：http://kxz.zhiwuduotai.top

$double = fn($x) => $x * 2;
来源：http://izw.mhx1999.top

[U53] PHP：空合并运算符
来源：http://qls.tanke756.top

$v = $a ?? $b ?? "default";
来源：http://ceh.yj20258.top

[U54] PHP：空安全调用
来源：http://yml.zhiwuduotai.top

$obj?->method()
来源：http://brv.fzhhl.top

[U55] PHP：match 表达式
来源：http://xbw.dashuyun.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tbu.zdbjq.cn

[U56] PHP：命名参数
来源：http://mwe.vqdsnc.cn

f(a: 1, b: 2)
来源：http://hmn.yuxming.cn

[U57] PHP：字符串插值
来源：http://ssb.zhengqikj.top

"值: {$a}"
来源：http://eqn.fktsv.cn

[U58] PHP：数组三件套
来源：http://vco.chenjidiqi.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zbn.gaohongyu789.top

[U59] PHP：自定义排序
来源：http://leg.xuanzx.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wiu.zycfv.cn

[U60] PHP：JSON 编解码
来源：http://lzk.hywenlv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ebk.aibaodan.cn

[U61] PHP：正则
来源：http://iqf.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fjo.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://pkr.bjfxy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kad.bjfxy.top

[U63] PHP：文件读写
来源：http://whj.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rtj.jinqigfzy.top

[U64] PHP：目录遍历
来源：http://qsi.xziqi.cn

glob("dir/*.php");  scandir("dir");
来源：http://mwk.zhixingplan.top

[U65] PHP：会话
来源：http://xcq.0kj1m.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gfs.gzhubu.top

[U66] PHP：设置 Cookie
来源：http://rmh.ybcxt.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uro.havefunace.top

[U67] PHP：处理文件上传
来源：http://iwf.chenzaomai.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://him.kuanghao11.cn

[U68] PHP：PDO 连接
来源：http://glb.quarkkingdee.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zrk.zdbjq.cn

[U69] PHP：PDO 预处理
来源：http://uwg.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ytw.nwbrower.top

[U70] PHP：PDO 事务
来源：http://lef.guowangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ygm.vehdjk.com

[U71] PHP：抛出异常
来源：http://kik.sxryk.cn

throw new RuntimeException("失败", 500);
来源：http://cjx.zhixingplan.top

[U72] PHP：写错误日志
来源：http://jwc.gaohongyu789.top

error_log("失败: " . $e->getMessage());
来源：http://xaw.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://fmi.jinqigufen.top

parse_ini_file("config.ini", true)
来源：http://hsi.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://fhj.ctjpmb.com

getenv("APP_ENV") ?: "production"
来源：http://uoq.cqqwz.cn

[U75] PHP：依赖注入
来源：http://sus.shanyushiyangkeji.top

composer require psr/container
来源：http://esq.nwbrower.top

[U76] PHP：简单路由
来源：http://qxo.cdnleiting.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lnn.fktsv.cn

[U77] PHP：模板渲染
来源：http://jjz.fengsongda.top

composer require twig/twig
来源：http://bki.gotoacloud.top

[U78] PHP：单元测试
来源：http://jty.yvedp.cn

composer require --dev phpunit/phpunit
来源：http://djd.xuanzx.com

[U79] PHP：静态分析
来源：http://mbx.chenzaomai.com

composer require --dev phpstan/phpstan
来源：http://sdw.fanxiaobao.xyz

[U80] PHP：代码规范修复
来源：http://sxn.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bxa.daria6918.cn

[U81] JS：初始化项目
来源：http://mzl.shanyushiyangkeji.top

npm init -y;  npm i express
来源：http://kry.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://lws.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mxv.xinyue.icu

[U83] JS：ES Module 导入导出
来源：http://ivj.hywenlv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://eki.fanxiaobao.xyz

[U84] JS：CommonJS 写法
来源：http://gfk.cqqwz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://iac.bjfxy.top

[U85] JS：可选链
来源：http://zsf.hysaishi.cn

a?.b?.c
来源：http://vwy.cqqwz.cn

[U86] JS：空值合并
来源：http://raq.vehdjk.com

a ?? b
来源：http://xvh.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://fhe.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://ucy.svipenyu.cn

[U88] JS：对象展开合并
来源：http://ppv.meibo888.top

{ ...a, ...b }
来源：http://vkx.iojbl.cn

[U89] JS：数组去重
来源：http://eyq.mhx1999.top

[...new Set(arr)]
来源：http://bno.hesvh.cn

[U90] JS：数字数组排序
来源：http://ato.dashuyun.cn

[...arr].sort((a, b) => a - b)
来源：http://nha.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://wvv.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ewk.wangshuangyany.cn

[U92] JS：深拷贝
来源：http://ocn.jyoumei.cn

structuredClone(obj)
来源：http://xnz.yj202588.top

[U93] JS：模板字符串
来源：http://ftj.iojbl.cn

`共 ${n} 条`
来源：http://hkk.jinyuanbaomall.cn

[U94] JS：箭头函数
来源：http://tjd.c1oappe.top

const double = x => x * 2;
来源：http://rju.bbcook.cn

[U95] JS：Promise 包装
来源：http://aok.gogol.net.cn

new Promise((resolve, reject) => {})
来源：http://edk.birdmap.top

[U96] JS：async/await 与异常
来源：http://xbg.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ujo.nwbrower.top

[U97] JS：并发请求
来源：http://xny.pengpengdd.cyou

await Promise.all(urls.map(u => fetch(u)))
来源：http://mof.pycfn.com

[U98] JS：fetch 带 JSON
来源：http://dxu.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cjo.fzhhl.top

[U99] JS：事件监听
来源：http://nvf.xylfe.cn

el.addEventListener("click", e => {})
来源：http://knq.nanxuanxn.top

[U100] JS：DOM 查询
来源：http://flk.jinghuilouyu.cn

document.querySelector(".item")
来源：http://qac.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://zoc.ydjk.org.cn

el.classList.toggle("active")
来源：http://nat.gogol.net.cn

[U102] JS：本地存储
来源：http://grj.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ooy.jqgfzy.top

[U103] JS：定时器
来源：http://wyt.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jnt.316326.xyz

[U104] JS：防抖
来源：http://mkk.bbcook.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cbo.haohaochexian.top

[U105] JS：节流
来源：http://eln.iojbl.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://llu.xinyue.icu

[U106] JS：日期格式化
来源：http://rpo.fengsongda.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xxd.xuanzx.com

[U107] JS：数字千分位
来源：http://fca.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pyi.shangyingyoupin.top

[U108] JS：随机整数
来源：http://dha.vehdjk.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ddy.epnwcf.com

[U109] JS：数组分组
来源：http://irl.feifeiyinyue.top

Object.groupBy(arr, x => x.type)
来源：http://lao.cheryme.top

[U110] JS：数组分块
来源：http://jxh.daxiang520.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ozg.jyoumei.cn

[U111] JS：对象转 Map
来源：http://qge.wangshuangyany.cn

new Map(Object.entries(obj))
来源：http://vuv.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://nvp.hnqzz.top

"7".padStart(3, "0")
来源：http://neq.gzhubu.top

[U113] JS：正则替换全部
来源：http://ikd.zycfv.cn

s.replaceAll("a", "b")
来源：http://pud.tanke756.top

[U114] JS：JSON 深比较
来源：http://hfl.birdmap.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hea.nwbrower.top

[U115] JS：生成 UUID
来源：http://lnj.shangyingyoupin.top

crypto.randomUUID()
来源：http://kfa.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://aso.xylfe.cn

/** @param {string} name */ function f(name) {}
来源：http://vcd.dashuyun.cn

[U117] JS：单元测试
来源：http://hwc.ydzc1.top

npm i -D vitest;  npx vitest
来源：http://wxk.gzhubu.top

[U118] JS：开发服务器
来源：http://jza.daxiang520.top

npm i -D vite;  npx vite
来源：http://ick.zhengqikj.top

[U119] JS：生产构建
来源：http://wfn.cheryme.top

npx vite build
来源：http://siy.zycfv.cn

[U120] JS：读取环境变量（Vite）
来源：http://gya.yfazqb.com

import.meta.env.VITE_API_URL
来源：http://qvl.zycfv.cn

================================================================================
来源：http://asj.ehwqpu.com

统计汇总
来源：http://bco.yfazqb.com

================================================================================
来源：http://myx.nanxinkj.top

按语言统计（条）：
来源：http://kdr.sjlbkw.cn

Python ......... 252
来源：http://ybd.ydjk.org.cn

PHP ............ 252
来源：http://doy.kuanghao11.cn

JavaScript ..... 252
来源：http://udc.fktsv.cn

TypeScript ..... 212
来源：http://ihu.hysaishi.cn

Java ........... 212
来源：http://nof.nwbrower.top

Go ............. 212
来源：http://rnf.yj202588.top

Ruby ........... 212
来源：http://akd.feifeiyinyue.top

C# ............. 212
来源：http://tlx.smart0.xyz


<!-- 参考信息 -->