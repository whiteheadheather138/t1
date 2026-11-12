代发 wailian999

[T41] Perl：Hello World
来源：http://ziz.dashuyun.cn

print "Hello\n";
来源：http://umj.yueranfly.top

[T42] Perl：变量类型
来源：http://hmn.xziqi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oaf.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://rkn.ybcxt.top

"值: $a"
来源：http://tvv.tianlin.xyz

[T44] Perl：条件
来源：http://gup.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://ubu.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://taf.yuxming.cn

for my $x (@arr) { print $x; }
来源：http://jso.zhaomingkeji.xyz

[T46] Perl：哈希操作
来源：http://sxb.ybcxt.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qnw.hammf.cn

[T47] Perl：正则捕获
来源：http://pkm.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://hai.316326.xyz

[T48] Perl：正则替换
来源：http://gtk.fktsv.cn

$s =~ s/old/new/g;
来源：http://mrb.hcnkem.com

[T49] Perl：函数
来源：http://dnj.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xmm.cashguo.top

[T50] Perl：逐行读文件
来源：http://tti.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gnc.hnxiangtu.top

while (my $line = <$fh>) { print $line; }
来源：http://kux.chenjidiqi.icu

[T51] Scala：Hello World
来源：http://wdq.shanyushiyangkeji.top

println("Hello")
来源：http://vql.daxiang520.top

[T52] Scala：变量
来源：http://mlk.xylfe.cn

val a = 1;  var b = 2
来源：http://vem.gzhubu.top

[T53] Scala：字符串插值
来源：http://odg.tian-w.cn

s"值: $b"
来源：http://qbj.smart0.xyz

[T54] Scala：集合映射
来源：http://qes.yueranfly.top

List(1, 2, 3).map(_ * 2)
来源：http://mjy.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://hsj.fengsongda.top

List(1, 2, 3).filter(_ > 1)
来源：http://bhr.jianghu66.top

[T56] Scala：样例类
来源：http://xhp.gogol.net.cn

case class User(name: String, age: Int)
来源：http://pcx.pycfn.com

[T57] Scala：模式匹配
来源：http://xpn.hywenlv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tip.jinqigfzy.top

[T58] Scala：函数定义
来源：http://ile.shanyushiyangtech.top

def add(a: Int, b: Int): Int = a + b
来源：http://vri.cqqwz.cn

[T59] Scala：循环
来源：http://uwp.jyoumei.cn

for (i <- 1 to 10) println(i)
来源：http://oor.xylfe.cn

[T60] Scala：折叠
来源：http://hut.fanxiaobao.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rtb.shuidangran.top

================================================================================
来源：http://rtt.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sss.fengsongda.top

================================================================================
来源：http://mnh.snrcjt.cn

[U01] Py：创建虚拟环境
来源：http://qga.hesvh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hhy.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://lqi.hcnkem.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hhn.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://djb.fehbvm.com

from dotenv import load_dotenv; load_dotenv()
来源：http://nkg.andypj.xyz

[U04] Py：变量调试打印
来源：http://qpm.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wvw.redwolf501.top

[U05] Py：列表去重且保序
来源：http://xio.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://rai.birdmap.top

[U06] Py：合并两个字典
来源：http://gtz.quarkkingdee.top

{**a, **b}
来源：http://unp.yuanzhike.top

[U07] Py：反转字典键值
来源：http://aww.feifeiyinyue.top

{v: k for k, v in d.items()}
来源：http://faf.fktsv.cn

[U08] Py：展平二维列表
来源：http://gsa.jianghu66.top

[y for x in nested for y in x]
来源：http://sbn.birdmap.top

[U09] Py：字典取最大值的键
来源：http://wpo.meibo888.top

max(d, key=d.get)
来源：http://brv.jinyuanbaomall.cn

[U10] Py：按值排序字典
来源：http://gpw.xuanzx.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vvd.guannengcc.top

[U11] Py：生成器表达式
来源：http://lcm.shanyushiyangkeji.top

(x * 2 for x in arr)
来源：http://vwj.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://rqe.epnwcf.com

Counter(arr).most_common(3)
来源：http://nie.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://eoj.sufxvd.cn

deque(maxlen=10)
来源：http://bbg.hongshengwenyu.top

[U14] Py：分组收集到列表
来源：http://aes.ppjwa.cn

defaultdict(list)
来源：http://vhy.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://igz.hysaishi.cn

t = time.perf_counter()
来源：http://idn.iojbl.cn

[U16] Py：命令行参数解析
来源：http://hpf.yuanzhike.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://abj.xuanzx.com

[U17] Py：初始化日志
来源：http://cuo.jinghuilouyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://eip.chenlongwang.top

[U18] Py：预编译正则
来源：http://fgu.epnwcf.com

pat = re.compile(r"\d+")
来源：http://zjo.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://blw.ybcxt.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sdo.cdnleiting.top

[U20] Py：缓存函数结果
来源：http://arl.xylfe.cn

@functools.lru_cache(maxsize=None)
来源：http://uju.jinghuilouyu.cn

[U21] Py：自定义上下文管理器
来源：http://mtr.yj20258.top

@contextlib.contextmanager
来源：http://ayu.daxiang520.top

[U22] Py：矩阵转置
来源：http://yba.havefunace.top

list(zip(*m))
来源：http://vkx.jinqigfzy.top

[U23] Py：分块读取大文件
来源：http://reo.andypj.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xgp.guannengcc.top

[U24] Py：路径操作
来源：http://jsp.shanyushiyangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://afy.zycfv.cn

[U25] Py：CSV 按字典读
来源：http://mnm.svipenyu.cn

csv.DictReader(f)
来源：http://ojd.jqgufenzy.top

[U26] Py：并发下载
来源：http://tpt.fehbvm.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wxx.cheryme.top

[U27] Py：异步 HTTP
来源：http://awr.jlsjyb.cn

aiohttp.ClientSession() 配合 async with
来源：http://dwg.ctjpmb.com

[U28] Py：类型别名
来源：http://pyx.yj20258888.top

UserId = int
来源：http://tti.tian-w.cn

[U29] Py：属性校验
来源：http://maj.ivvv.top

@property 与 @x.setter 配合
来源：http://oat.zhixingplan.top

[U30] Py：数据类
来源：http://wft.shuidangran.top

@dataclass(slots=True)
来源：http://rtk.nanxuanxn.top

[U31] Py：单测
来源：http://hln.shangyingyoupin.top

python -m pytest -q
来源：http://dvc.epnwcf.com

[U32] Py：代码格式化
来源：http://wla.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://zyu.yanxiufei.cn

[U33] Py：打包发布
来源：http://lyg.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://aes.xuanzx.com

[U34] Py：判断编码
来源：http://mlw.zhijiandao.cn

chardet.detect(raw)
来源：http://kyv.fanxiaobao.xyz

[U35] Py：发送邮件
来源：http://ove.hongshengwenyu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jga.zdqjudy.top

[U36] Py：定时任务
来源：http://fef.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://exv.ivvv.top

[U37] Py：读写 Excel
来源：http://vpu.quarkkingdee.top

pandas.read_excel / DataFrame.to_excel
来源：http://uxd.nanxuanxn.top

[U38] Py：获取脚本所在目录
来源：http://jwt.fanxiaobao.xyz

Path(__file__).resolve().parent
来源：http://zze.wangdashe.top

[U39] Py：判断是否在交互环境
来源：http://rvq.316326.xyz

sys.stdout.isatty()
来源：http://ncm.xylfe.cn

[U40] Py：打印到标准错误
来源：http://lyy.nwbrower.top

print("err", file=sys.stderr)
来源：http://ior.mhx1999.top

[U41] PHP：初始化 Composer 项目
来源：http://ojn.havefunace.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ayg.zdbjq.cn

[U42] PHP：PSR-4 自动加载
来源：http://hvs.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ndl.jinghuilouyu.cn

[U43] PHP：声明命名空间
来源：http://koe.cdnleiting.top

namespace App\Http;
来源：http://hac.nanxinkj.top

[U44] PHP：开启严格类型
来源：http://wjc.redwolf501.top

declare(strict_types=1);
来源：http://yvj.hnxiangtu.top

[U45] PHP：类型声明与返回类型
来源：http://tow.tarul.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tpm.sjlbkw.cn

[U46] PHP：可空类型
来源：http://lnk.shangyingyoupin.top

?string $name = null
来源：http://dtx.jinyuanbaomall.cn

[U47] PHP：联合类型
来源：http://ozy.gogol.net.cn

int|string $id
来源：http://msd.dianchejie.cn

[U48] PHP：纯枚举
来源：http://ymj.ctjpmb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://abn.gzhubu.top

[U49] PHP：只读属性
来源：http://xln.iojbl.cn

public readonly string $name
来源：http://qdw.ehwqpu.com

[U50] PHP：构造器属性提升
来源：http://kej.smart0.xyz

public function __construct(private int $id) {}
来源：http://vmi.meibo888.top

[U51] PHP：数组解构
来源：http://oik.xingfuxueyuan.xyz

[$a, $b] = $arr;
来源：http://djy.cqqwz.cn

[U52] PHP：箭头函数
来源：http://lwh.zhaomingkeji.xyz

$double = fn($x) => $x * 2;
来源：http://aaa.shanyushiyangkeji.top

[U53] PHP：空合并运算符
来源：http://ozf.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://ihp.fktsv.cn

[U54] PHP：空安全调用
来源：http://rjb.yuanzhike.top

$obj?->method()
来源：http://mgz.sufxvd.cn

[U55] PHP：match 表达式
来源：http://vws.sufxvd.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bhu.tianlin.xyz

[U56] PHP：命名参数
来源：http://mdo.zhongyouzk.top

f(a: 1, b: 2)
来源：http://vsn.kuanghao11.cn

[U57] PHP：字符串插值
来源：http://cmd.daria6918.cn

"值: {$a}"
来源：http://blv.jlsjyb.cn

[U58] PHP：数组三件套
来源：http://xzm.yj20258888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wov.shanyushiyangtech.top

[U59] PHP：自定义排序
来源：http://bfm.wangdashe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xoe.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://zbi.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://emg.c1oappe.top

[U61] PHP：正则
来源：http://kcx.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://spk.snrcjt.cn

[U62] PHP：日期对象
来源：http://jyf.kuanghao11.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nhq.xuetiantiany.cn

[U63] PHP：文件读写
来源：http://ycn.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gyy.zhoulong.xyz

[U64] PHP：目录遍历
来源：http://lby.yfazqb.com

glob("dir/*.php");  scandir("dir");
来源：http://ier.xuanzx.com

[U65] PHP：会话
来源：http://wxl.xuanzx.com

session_start();  $_SESSION["uid"] = 1;
来源：http://jup.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://hvt.ehwqpu.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cfr.nanxuanxn.top

[U67] PHP：处理文件上传
来源：http://vuk.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yul.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://khu.yueranfly.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vlu.yuxming.cn

[U69] PHP：PDO 预处理
来源：http://vzr.yanxiufei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gvq.sufxvd.cn

[U70] PHP：PDO 事务
来源：http://kec.havefunace.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tqq.yongpay.top

[U71] PHP：抛出异常
来源：http://ind.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://coa.aibaodan.cn

[U72] PHP：写错误日志
来源：http://ljz.jianghu66.top

error_log("失败: " . $e->getMessage());
来源：http://ujr.nanxuanxn.top

[U73] PHP：读取 ini 配置
来源：http://nrp.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://mob.ydjk.org.cn

[U74] PHP：读取环境变量
来源：http://vnp.ppjwa.cn

getenv("APP_ENV") ?: "production"
来源：http://yai.uphjek.com

[U75] PHP：依赖注入
来源：http://yrf.yongpay.top

composer require psr/container
来源：http://fae.c1oappe.top

[U76] PHP：简单路由
来源：http://egt.sufxvd.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pad.ehwqpu.com

[U77] PHP：模板渲染
来源：http://tgb.hysaishi.cn

composer require twig/twig
来源：http://fwp.gaohongyu789.top

[U78] PHP：单元测试
来源：http://rcw.52xcode.cn

composer require --dev phpunit/phpunit
来源：http://ljw.gaohongyu789.top

[U79] PHP：静态分析
来源：http://ypq.nanxuanxn.top

composer require --dev phpstan/phpstan
来源：http://anl.316326.xyz

[U80] PHP：代码规范修复
来源：http://ulu.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wne.c1oappe.top

[U81] JS：初始化项目
来源：http://nzp.ivvv.top

npm init -y;  npm i express
来源：http://spl.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://mgk.cheryme.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://snt.uphjek.com

[U83] JS：ES Module 导入导出
来源：http://jtl.kuanghao11.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cns.sjlbkw.cn

[U84] JS：CommonJS 写法
来源：http://gkq.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vaz.dianchejie.cn

[U85] JS：可选链
来源：http://tvi.guannengcc.top

a?.b?.c
来源：http://fzv.shzxlz.cn

[U86] JS：空值合并
来源：http://jvt.hysaishi.cn

a ?? b
来源：http://sfv.svipenyu.cn

[U87] JS：解构默认值
来源：http://wpo.jinyuanbaomall.cn

const { a = 1, b = 2 } = obj;
来源：http://jop.feifeiyinyue.top

[U88] JS：对象展开合并
来源：http://ogo.yuxming.cn

{ ...a, ...b }
来源：http://gqv.xinyue.icu

[U89] JS：数组去重
来源：http://fqg.yongpay.top

[...new Set(arr)]
来源：http://cov.9152youxi.cn

[U90] JS：数字数组排序
来源：http://aet.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://hoq.cashguo.top

[U91] JS：对象键值遍历
来源：http://mjl.vqdsnc.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mei.vqdsnc.cn

[U92] JS：深拷贝
来源：http://vhr.hnqzz.top

structuredClone(obj)
来源：http://asz.hnqzz.top

[U93] JS：模板字符串
来源：http://jfa.shanyushiyangtech.top

`共 ${n} 条`
来源：http://nrd.gogol.net.cn

[U94] JS：箭头函数
来源：http://wkz.yj20258888.top

const double = x => x * 2;
来源：http://oyf.jqgfzy.top

[U95] JS：Promise 包装
来源：http://rqb.ydjk.org.cn

new Promise((resolve, reject) => {})
来源：http://sjv.hfpthk.cn

[U96] JS：async/await 与异常
来源：http://rlw.feifeiyinyue.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bkf.xuetiantiany.cn

[U97] JS：并发请求
来源：http://kbr.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://vgn.0kj1m.cn

[U98] JS：fetch 带 JSON
来源：http://qsy.zdqjudy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gbd.tian-w.cn

[U99] JS：事件监听
来源：http://zux.ywan-chungtsiang.top

el.addEventListener("click", e => {})
来源：http://ftj.yanxiufei.cn

[U100] JS：DOM 查询
来源：http://nse.bbcook.cn

document.querySelector(".item")
来源：http://fwp.aibaodan.cn

[U101] JS：classList 操作
来源：http://pyw.hcnkem.com

el.classList.toggle("active")
来源：http://yfc.zhongyouzk.top

[U102] JS：本地存储
来源：http://dgg.fengsongda.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gqv.shanyushiyangtech.top

[U103] JS：定时器
来源：http://ltt.bjfxy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://spw.chenzaomai.com

[U104] JS：防抖
来源：http://afh.jqgufenzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kdt.pycfn.com

[U105] JS：节流
来源：http://iir.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://amr.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://bhc.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qkk.zdbjq.cn

[U107] JS：数字千分位
来源：http://mqq.ctjpmb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yor.sysykeji.top

[U108] JS：随机整数
来源：http://wuh.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bdi.hfpthk.cn

[U109] JS：数组分组
来源：http://mng.pengpengdd.cyou

Object.groupBy(arr, x => x.type)
来源：http://qyy.zhongyouzk.top

[U110] JS：数组分块
来源：http://qxr.ppjwa.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lhn.redwolf501.top

[U111] JS：对象转 Map
来源：http://bfv.cdnleiting.top

new Map(Object.entries(obj))
来源：http://evg.yj20258888.top

[U112] JS：字符串补位
来源：http://cvm.daria6918.cn

"7".padStart(3, "0")
来源：http://lui.jinqigufen.top

[U113] JS：正则替换全部
来源：http://sbu.zhixingplan.top

s.replaceAll("a", "b")
来源：http://xzd.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://mgf.cucudq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://glc.vehdjk.com

[U115] JS：生成 UUID
来源：http://swy.yfazqb.com

crypto.randomUUID()
来源：http://ysz.yanxiufei.cn

[U116] JS：类型检查（JSDoc）
来源：http://agz.chenjidiqi.icu

/** @param {string} name */ function f(name) {}
来源：http://ckr.zhongyouzk.top

[U117] JS：单元测试
来源：http://mac.fengsongda.top

npm i -D vitest;  npx vitest
来源：http://eig.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://xot.hysaishi.cn

npm i -D vite;  npx vite
来源：http://yfu.epnwcf.com

[U119] JS：生产构建
来源：http://uum.aibaodan.cn

npx vite build
来源：http://qyz.gogol.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://csi.daria6918.cn

import.meta.env.VITE_API_URL
来源：http://ctv.uphjek.com

================================================================================
来源：http://sqw.sxryk.cn

统计汇总
来源：http://gnm.jiagoushi.top

================================================================================
来源：http://apw.shuidangran.top

按语言统计（条）：
来源：http://enf.iojbl.cn

Python ......... 252
来源：http://lle.jianghu66.top

PHP ............ 252
来源：http://sjv.jiagoushi.top

JavaScript ..... 252
来源：http://dfq.tianlin.xyz

TypeScript ..... 212
来源：http://bfj.yj20258.top

Java ........... 212
来源：http://fzd.svipenyu.cn

Go ............. 212
来源：http://fes.haohaochexian.top

Ruby ........... 212
来源：http://rjo.yuanzhike.top

C# ............. 212
来源：http://jtg.jlsjyb.cn

C .............. 30
来源：http://tbq.pengpengdd.cyou

C++ ............ 30
来源：http://btu.yvedp.cn

SQL ............ 90
来源：http://sae.chenlongwang.top

Bash ........... 80
来源：http://wvl.52xcode.cn


<!-- 参考信息 -->