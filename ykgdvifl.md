代发 wailian999

[T41] Perl：Hello World
来源：http://tco.zhengqikj.top

print "Hello\n";
来源：http://shl.jinghuilouyu.cn

[T42] Perl：变量类型
来源：http://tgj.pycfn.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gwk.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://qyk.ctjpmb.com

"值: $a"
来源：http://tpt.zdbjq.cn

[T44] Perl：条件
来源：http://uew.kuanghao11.cn

if ($a > 0) { print "正"; }
来源：http://ynr.sysykeji.top

[T45] Perl：数组遍历
来源：http://yoh.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://pzg.zdqjudy.top

[T46] Perl：哈希操作
来源：http://iss.fehbvm.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cpo.dianchejie.cn

[T47] Perl：正则捕获
来源：http://rrv.316326.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://qim.sysykeji.top

[T48] Perl：正则替换
来源：http://mod.fktsv.cn

$s =~ s/old/new/g;
来源：http://hts.kuanghao11.cn

[T49] Perl：函数
来源：http://rcx.cucudq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eui.andypj.xyz

[T50] Perl：逐行读文件
来源：http://gep.xylfe.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mop.chenlongwang.top

while (my $line = <$fh>) { print $line; }
来源：http://lft.zhijiandao.cn

[T51] Scala：Hello World
来源：http://ppk.tarul.cn

println("Hello")
来源：http://rzg.cheryme.top

[T52] Scala：变量
来源：http://pcr.sweek.top

val a = 1;  var b = 2
来源：http://dcs.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://vqv.xingfuxueyuan.xyz

s"值: $b"
来源：http://dzm.kuanghao11.cn

[T54] Scala：集合映射
来源：http://imm.xuetiantiany.cn

List(1, 2, 3).map(_ * 2)
来源：http://bfm.redwolf501.top

[T55] Scala：集合过滤
来源：http://jso.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qgu.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://flm.gogol.net.cn

case class User(name: String, age: Int)
来源：http://hcy.jinyuanbaomall.cn

[T57] Scala：模式匹配
来源：http://hlw.xuetiantiany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nud.yonumen.top

[T58] Scala：函数定义
来源：http://zfu.jlsjyb.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sza.vqdsnc.cn

[T59] Scala：循环
来源：http://yaw.xylfe.cn

for (i <- 1 to 10) println(i)
来源：http://mho.zdbjq.cn

[T60] Scala：折叠
来源：http://tim.yongpay.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://onw.daxiang520.top

================================================================================
来源：http://nfw.jlsjyb.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://djs.xylfe.cn

================================================================================
来源：http://nes.jlsjyb.cn

[U01] Py：创建虚拟环境
来源：http://yla.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vfa.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://ker.hcnkem.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ahp.zdbjq.cn

[U03] Py：加载 .env 配置
来源：http://sjs.yj20258888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zcr.xingfuxueyuan.xyz

[U04] Py：变量调试打印
来源：http://ebc.gzhubu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qsn.hfpthk.cn

[U05] Py：列表去重且保序
来源：http://qke.yongpay.top

list(dict.fromkeys(arr))
来源：http://tej.ybcxt.top

[U06] Py：合并两个字典
来源：http://feb.uphjek.com

{**a, **b}
来源：http://tdt.tian-w.cn

[U07] Py：反转字典键值
来源：http://tni.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://dml.fktsv.cn

[U08] Py：展平二维列表
来源：http://hvv.uphjek.com

[y for x in nested for y in x]
来源：http://azz.andypj.xyz

[U09] Py：字典取最大值的键
来源：http://qda.jinyuanbaomall.cn

max(d, key=d.get)
来源：http://pup.jiagoushi.top

[U10] Py：按值排序字典
来源：http://xkq.gotoacloud.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://saa.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://ueh.ehwqpu.com

(x * 2 for x in arr)
来源：http://fwn.ybcxt.top

[U12] Py：取出现最多的 3 个元素
来源：http://itc.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://sxg.vqdsnc.cn

[U13] Py：固定长度队列
来源：http://oxu.chenjidiqi.icu

deque(maxlen=10)
来源：http://kjw.zycfv.cn

[U14] Py：分组收集到列表
来源：http://pao.gogol.net.cn

defaultdict(list)
来源：http://nla.fktsv.cn

[U15] Py：高精度计时
来源：http://wvu.fanxiaobao.xyz

t = time.perf_counter()
来源：http://gga.wangshuangyany.cn

[U16] Py：命令行参数解析
来源：http://buq.kuanghao11.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lhq.vqdsnc.cn

[U17] Py：初始化日志
来源：http://yfq.kuanghao11.cn

logging.basicConfig(level=logging.INFO)
来源：http://qaf.sjlbkw.cn

[U18] Py：预编译正则
来源：http://jot.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://fxc.daxiang520.top

[U19] Py：正则替换带回调
来源：http://moy.vqdsnc.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tui.meibo888.top

[U20] Py：缓存函数结果
来源：http://jlf.ivvv.top

@functools.lru_cache(maxsize=None)
来源：http://qgu.zhongyouzk.top

[U21] Py：自定义上下文管理器
来源：http://jpf.yangfankeji.com

@contextlib.contextmanager
来源：http://hiu.aizwys.cn

[U22] Py：矩阵转置
来源：http://ayp.ybcxt.top

list(zip(*m))
来源：http://eaw.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://ops.ydzc1.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qok.shanyushiyangtech.top

[U24] Py：路径操作
来源：http://aih.gzhubu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zan.yuanzhike.top

[U25] Py：CSV 按字典读
来源：http://kpr.ppjwa.cn

csv.DictReader(f)
来源：http://hay.yanxiufei.cn

[U26] Py：并发下载
来源：http://cie.fzhhl.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ilw.shzxlz.cn

[U27] Py：异步 HTTP
来源：http://dez.yanxiufei.cn

aiohttp.ClientSession() 配合 async with
来源：http://dxv.mhx1999.top

[U28] Py：类型别名
来源：http://kzd.zhijiandao.cn

UserId = int
来源：http://vaw.shangyingyoupin.top

[U29] Py：属性校验
来源：http://hpp.cucudq.cn

@property 与 @x.setter 配合
来源：http://imi.daria6918.cn

[U30] Py：数据类
来源：http://mlj.meibo888.top

@dataclass(slots=True)
来源：http://fli.shuidangran.top

[U31] Py：单测
来源：http://wzu.dianchejie.cn

python -m pytest -q
来源：http://bkd.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://khz.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://rrb.nanxinkj.top

[U33] Py：打包发布
来源：http://agm.jinqigufen.top

python -m build  （依赖 pyproject.toml）
来源：http://ter.hysaishi.cn

[U34] Py：判断编码
来源：http://yff.redwolf501.top

chardet.detect(raw)
来源：http://hls.yanxiufei.cn

[U35] Py：发送邮件
来源：http://gff.chenlongwang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ddf.feifeiyinyue.top

[U36] Py：定时任务
来源：http://czo.nanxinkj.top

schedule.every(10).minutes.do(job)
来源：http://msi.yj20258.top

[U37] Py：读写 Excel
来源：http://guk.tianlin.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://wqe.ydjk.org.cn

[U38] Py：获取脚本所在目录
来源：http://aib.aibaodan.cn

Path(__file__).resolve().parent
来源：http://okk.chenjidiqi.icu

[U39] Py：判断是否在交互环境
来源：http://lqy.fzhhl.top

sys.stdout.isatty()
来源：http://vfj.316326.xyz

[U40] Py：打印到标准错误
来源：http://mol.jinqigufen.top

print("err", file=sys.stderr)
来源：http://fhm.cheryme.top

[U41] PHP：初始化 Composer 项目
来源：http://woj.ydzc1.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yzy.dashuyun.cn

[U42] PHP：PSR-4 自动加载
来源：http://gvg.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gzr.chenzaomai.com

[U43] PHP：声明命名空间
来源：http://xrn.zhengqikj.top

namespace App\Http;
来源：http://pcs.aibaodan.cn

[U44] PHP：开启严格类型
来源：http://peo.zhoulong.xyz

declare(strict_types=1);
来源：http://wez.yonumen.top

[U45] PHP：类型声明与返回类型
来源：http://sei.yonumen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kdc.nanxinkj.top

[U46] PHP：可空类型
来源：http://jzi.hammf.cn

?string $name = null
来源：http://xig.jlsjyb.cn

[U47] PHP：联合类型
来源：http://ldr.fengsongda.top

int|string $id
来源：http://qtp.cdnleiting.top

[U48] PHP：纯枚举
来源：http://lby.jlsjyb.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vqi.nanxuanxn.top

[U49] PHP：只读属性
来源：http://gfd.dianchejie.cn

public readonly string $name
来源：http://hli.hongshengwenyu.top

[U50] PHP：构造器属性提升
来源：http://uug.fengsongda.top

public function __construct(private int $id) {}
来源：http://ywy.jqgfzy.top

[U51] PHP：数组解构
来源：http://jba.gotoacloud.top

[$a, $b] = $arr;
来源：http://enj.sxryk.cn

[U52] PHP：箭头函数
来源：http://nng.yanxiufei.cn

$double = fn($x) => $x * 2;
来源：http://kly.ppjwa.cn

[U53] PHP：空合并运算符
来源：http://vwz.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://bfg.kuanghao11.cn

[U54] PHP：空安全调用
来源：http://xxm.zhijiandao.cn

$obj?->method()
来源：http://gjs.xuanzx.com

[U55] PHP：match 表达式
来源：http://svj.iojbl.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vsz.andypj.xyz

[U56] PHP：命名参数
来源：http://bcf.ydzc1.top

f(a: 1, b: 2)
来源：http://isp.hywenlv.cn

[U57] PHP：字符串插值
来源：http://dwp.pengpengdd.cyou

"值: {$a}"
来源：http://pah.yueranfly.top

[U58] PHP：数组三件套
来源：http://zup.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gls.nwbrower.top

[U59] PHP：自定义排序
来源：http://jqt.dashuyun.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nwl.gotoacloud.top

[U60] PHP：JSON 编解码
来源：http://fsb.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://muo.shuidangran.top

[U61] PHP：正则
来源：http://evc.ydjk.org.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mwg.cucudq.cn

[U62] PHP：日期对象
来源：http://pou.hfpthk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kwg.yj20258.top

[U63] PHP：文件读写
来源：http://xus.hesvh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wso.nwbrower.top

[U64] PHP：目录遍历
来源：http://jlp.sufxvd.cn

glob("dir/*.php");  scandir("dir");
来源：http://anu.hnxiangtu.top

[U65] PHP：会话
来源：http://etb.yuxming.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tzd.hesvh.cn

[U66] PHP：设置 Cookie
来源：http://hua.ctjpmb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vhx.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://qqv.yfazqb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mio.yfazqb.com

[U68] PHP：PDO 连接
来源：http://bji.cqqwz.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rxc.chenzaomai.com

[U69] PHP：PDO 预处理
来源：http://rkg.daxiang520.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tsc.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://nqx.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oil.yuxming.cn

[U71] PHP：抛出异常
来源：http://mdd.zycfv.cn

throw new RuntimeException("失败", 500);
来源：http://aoh.ctjpmb.com

[U72] PHP：写错误日志
来源：http://pmi.52xcode.cn

error_log("失败: " . $e->getMessage());
来源：http://dau.xinyue.icu

[U73] PHP：读取 ini 配置
来源：http://exb.shzxlz.cn

parse_ini_file("config.ini", true)
来源：http://yih.fehbvm.com

[U74] PHP：读取环境变量
来源：http://nod.316326.xyz

getenv("APP_ENV") ?: "production"
来源：http://dom.hnqzz.top

[U75] PHP：依赖注入
来源：http://gaq.jianghu66.top

composer require psr/container
来源：http://umi.zhoulong.xyz

[U76] PHP：简单路由
来源：http://zlv.ydjk.org.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iin.hysaishi.cn

[U77] PHP：模板渲染
来源：http://frr.daxiang520.top

composer require twig/twig
来源：http://hzq.cashguo.top

[U78] PHP：单元测试
来源：http://atq.mhx1999.top

composer require --dev phpunit/phpunit
来源：http://emf.sjlbkw.cn

[U79] PHP：静态分析
来源：http://hdv.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://lax.iojbl.cn

[U80] PHP：代码规范修复
来源：http://ubk.tanke756.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rzt.nwbrower.top

[U81] JS：初始化项目
来源：http://gzw.zdqjudy.top

npm init -y;  npm i express
来源：http://wyh.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://ysb.zhaomingkeji.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://csq.shuidangran.top

[U83] JS：ES Module 导入导出
来源：http://blk.jiagoushi.top

export const a = 1;  import { a } from "./m.js";
来源：http://tla.bbcook.cn

[U84] JS：CommonJS 写法
来源：http://jlg.xuanzx.com

module.exports = { a };  const { a } = require("./m");
来源：http://kqu.cucudq.cn

[U85] JS：可选链
来源：http://cuf.mhx1999.top

a?.b?.c
来源：http://yqa.zhoulong.xyz

[U86] JS：空值合并
来源：http://iok.hesvh.cn

a ?? b
来源：http://zfu.aibaodan.cn

[U87] JS：解构默认值
来源：http://ood.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://yob.haohaochexian.top

[U88] JS：对象展开合并
来源：http://syw.gzhubu.top

{ ...a, ...b }
来源：http://ikl.xuetiantiany.cn

[U89] JS：数组去重
来源：http://auu.xinyue.icu

[...new Set(arr)]
来源：http://qwy.daria6918.cn

[U90] JS：数字数组排序
来源：http://ukv.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://exs.hammf.cn

[U91] JS：对象键值遍历
来源：http://xhg.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://chz.jianghu66.top

[U92] JS：深拷贝
来源：http://gjx.fehbvm.com

structuredClone(obj)
来源：http://ffu.iojbl.cn

[U93] JS：模板字符串
来源：http://kyg.yangfankeji.com

`共 ${n} 条`
来源：http://xwe.tianlin.xyz

[U94] JS：箭头函数
来源：http://hln.havefunace.top

const double = x => x * 2;
来源：http://fla.epnwcf.com

[U95] JS：Promise 包装
来源：http://cvf.cheryme.top

new Promise((resolve, reject) => {})
来源：http://kyk.tianlin.xyz

[U96] JS：async/await 与异常
来源：http://ezb.xuanzx.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ehm.yangfankeji.com

[U97] JS：并发请求
来源：http://wix.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://pnk.yanxiufei.cn

[U98] JS：fetch 带 JSON
来源：http://jto.chenjidiqi.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zdk.snrcjt.cn

[U99] JS：事件监听
来源：http://pnw.fengsongda.top

el.addEventListener("click", e => {})
来源：http://wcu.jqgfzy.top

[U100] JS：DOM 查询
来源：http://xmt.zhengqikj.top

document.querySelector(".item")
来源：http://vek.aizwys.cn

[U101] JS：classList 操作
来源：http://gjk.snrcjt.cn

el.classList.toggle("active")
来源：http://had.guannengcc.top

[U102] JS：本地存储
来源：http://hch.hfpthk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ara.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://swz.jinyuanbaomall.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gtg.vehdjk.com

[U104] JS：防抖
来源：http://vis.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iwo.vqdsnc.cn

[U105] JS：节流
来源：http://ehd.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rbp.xuanzx.com

[U106] JS：日期格式化
来源：http://jqf.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ryo.meibo888.top

[U107] JS：数字千分位
来源：http://knc.chenlongwang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zym.wangdashe.top

[U108] JS：随机整数
来源：http://lwj.hesvh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tiw.epnwcf.com

[U109] JS：数组分组
来源：http://fff.tian-w.cn

Object.groupBy(arr, x => x.type)
来源：http://umj.quarkkingdee.top

[U110] JS：数组分块
来源：http://dzz.jqgfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hlk.iojbl.cn

[U111] JS：对象转 Map
来源：http://rxv.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://wkj.chenzaomai.com

[U112] JS：字符串补位
来源：http://hkl.bbcook.cn

"7".padStart(3, "0")
来源：http://taa.smart0.xyz

[U113] JS：正则替换全部
来源：http://kqa.cdnleiting.top

s.replaceAll("a", "b")
来源：http://jqn.yj202588.top

[U114] JS：JSON 深比较
来源：http://vio.zhengqikj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qvn.yj20258.top

[U115] JS：生成 UUID
来源：http://qup.yj20258888.top

crypto.randomUUID()
来源：http://oxo.jlsjyb.cn

[U116] JS：类型检查（JSDoc）
来源：http://fmv.gaohongyu789.top

/** @param {string} name */ function f(name) {}
来源：http://tfc.tian-w.cn

[U117] JS：单元测试
来源：http://mkc.yonumen.top

npm i -D vitest;  npx vitest
来源：http://nab.dianchejie.cn

[U118] JS：开发服务器
来源：http://xdr.bjfxy.top

npm i -D vite;  npx vite
来源：http://qpz.zhijiandao.cn

[U119] JS：生产构建
来源：http://xxj.kuanghao11.cn

npx vite build
来源：http://zam.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://fat.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://zkc.ppjwa.cn

================================================================================
来源：http://tpn.aizwys.cn

统计汇总
来源：http://nav.yangfankeji.com

================================================================================
来源：http://bbr.0kj1m.cn

按语言统计（条）：
来源：http://mdp.yj202588.top

Python ......... 252
来源：http://mwi.chenjidiqi.icu

PHP ............ 252
来源：http://lmo.hnqzz.top

JavaScript ..... 252
来源：http://jhp.yanxiufei.cn

TypeScript ..... 212
来源：http://mmw.cashguo.top

Java ........... 212
来源：http://omh.pengpengdd.cyou

Go ............. 212
来源：http://pip.ehwqpu.com

Ruby ........... 212
来源：http://koj.tanke756.top

C# ............. 212
来源：http://icn.yueranfly.top

C .............. 30
来源：http://obi.zhoulong.xyz

C++ ............ 30
来源：http://kii.jqgfzy.top

SQL ............ 90
来源：http://cil.fehbvm.com

Bash ........... 80
来源：http://shx.feifeiyinyue.top


<!-- 参考信息 -->