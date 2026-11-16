代发 wailian999

[T41] Perl：Hello World
来源：http://ypt.hcnkem.com

print "Hello\n";
来源：http://mwj.kuanghao11.cn

[T42] Perl：变量类型
来源：http://evl.vqdsnc.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tft.sjlbkw.cn

[T43] Perl：字符串插值
来源：http://fwf.jinghuilouyu.cn

"值: $a"
来源：http://bvi.yangfankeji.com

[T44] Perl：条件
来源：http://dwz.dashuyun.cn

if ($a > 0) { print "正"; }
来源：http://qzg.shanyushiyangtech.top

[T45] Perl：数组遍历
来源：http://fum.tianlin.xyz

for my $x (@arr) { print $x; }
来源：http://mpy.haohaochexian.top

[T46] Perl：哈希操作
来源：http://pji.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hcu.yj202588.top

[T47] Perl：正则捕获
来源：http://img.zycfv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yxo.jinqigfzy.top

[T48] Perl：正则替换
来源：http://nob.yfazqb.com

$s =~ s/old/new/g;
来源：http://wok.yongpay.top

[T49] Perl：函数
来源：http://mxm.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zeg.yfazqb.com

[T50] Perl：逐行读文件
来源：http://vpr.yj202588.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hyu.bjfxy.top

while (my $line = <$fh>) { print $line; }
来源：http://cir.fehbvm.com

[T51] Scala：Hello World
来源：http://rcn.316326.xyz

println("Hello")
来源：http://cii.zhaomingkeji.xyz

[T52] Scala：变量
来源：http://qeb.shangyingyoupin.top

val a = 1;  var b = 2
来源：http://lrm.ehwqpu.com

[T53] Scala：字符串插值
来源：http://bgg.9152youxi.cn

s"值: $b"
来源：http://sqf.shangyingyoupin.top

[T54] Scala：集合映射
来源：http://zfa.jyoumei.cn

List(1, 2, 3).map(_ * 2)
来源：http://ewk.xziqi.cn

[T55] Scala：集合过滤
来源：http://tuj.chenlongwang.top

List(1, 2, 3).filter(_ > 1)
来源：http://hed.yj20258.top

[T56] Scala：样例类
来源：http://yxz.aibaodan.cn

case class User(name: String, age: Int)
来源：http://rnk.shzxlz.cn

[T57] Scala：模式匹配
来源：http://qws.yanxiufei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pjq.jqgufenzy.top

[T58] Scala：函数定义
来源：http://dvu.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://ijy.jiagoushi.top

[T59] Scala：循环
来源：http://acb.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://gsu.jinqigfzy.top

[T60] Scala：折叠
来源：http://dzc.havefunace.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ubf.wangshuangyany.cn

================================================================================
来源：http://ptc.fktsv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tpb.hnqzz.top

================================================================================
来源：http://ggn.yuanzhike.top

[U01] Py：创建虚拟环境
来源：http://ehb.yj20258888.top

python -m venv .venv && source .venv/bin/activate
来源：http://ygo.smart0.xyz

[U02] Py：导出 / 安装依赖
来源：http://klm.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vee.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://kri.hnqzz.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dyq.ydzc1.top

[U04] Py：变量调试打印
来源：http://sdp.yonumen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://teh.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://fiw.yuanzhike.top

list(dict.fromkeys(arr))
来源：http://kar.jqgufenzy.top

[U06] Py：合并两个字典
来源：http://ski.hywenlv.cn

{**a, **b}
来源：http://wcb.zhixingplan.top

[U07] Py：反转字典键值
来源：http://ofb.sysykeji.top

{v: k for k, v in d.items()}
来源：http://svc.zhiwuduotai.top

[U08] Py：展平二维列表
来源：http://mfv.chenzaomai.com

[y for x in nested for y in x]
来源：http://buw.gotoacloud.top

[U09] Py：字典取最大值的键
来源：http://kxt.quarkkingdee.top

max(d, key=d.get)
来源：http://qxp.yangfankeji.com

[U10] Py：按值排序字典
来源：http://yme.chenjidiqi.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tmt.dianchejie.cn

[U11] Py：生成器表达式
来源：http://vyy.gogol.net.cn

(x * 2 for x in arr)
来源：http://fjv.ydjk.org.cn

[U12] Py：取出现最多的 3 个元素
来源：http://djx.jinghuilouyu.cn

Counter(arr).most_common(3)
来源：http://nsk.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://gea.yueranfly.top

deque(maxlen=10)
来源：http://ogj.sufxvd.cn

[U14] Py：分组收集到列表
来源：http://bgi.sweek.top

defaultdict(list)
来源：http://fhu.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://rrs.chenzaomai.com

t = time.perf_counter()
来源：http://cwa.gzhubu.top

[U16] Py：命令行参数解析
来源：http://uuk.zycfv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hnp.daxiang520.top

[U17] Py：初始化日志
来源：http://xim.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://ybn.feifeiyinyue.top

[U18] Py：预编译正则
来源：http://xkz.jqgfzy.top

pat = re.compile(r"\d+")
来源：http://xhg.redwolf501.top

[U19] Py：正则替换带回调
来源：http://zvf.yueranfly.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xzr.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://nrh.yfazqb.com

@functools.lru_cache(maxsize=None)
来源：http://voe.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://bek.52xcode.cn

@contextlib.contextmanager
来源：http://mhz.xingfuxueyuan.xyz

[U22] Py：矩阵转置
来源：http://sei.xuetiantiany.cn

list(zip(*m))
来源：http://all.xingfuxueyuan.xyz

[U23] Py：分块读取大文件
来源：http://ncy.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hfv.316326.xyz

[U24] Py：路径操作
来源：http://gwd.kuanghao11.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jmx.wangshuangyany.cn

[U25] Py：CSV 按字典读
来源：http://lbf.fehbvm.com

csv.DictReader(f)
来源：http://grx.andypj.xyz

[U26] Py：并发下载
来源：http://nyu.shuidangran.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lwh.bbcook.cn

[U27] Py：异步 HTTP
来源：http://ali.sweek.top

aiohttp.ClientSession() 配合 async with
来源：http://sjv.dashuyun.cn

[U28] Py：类型别名
来源：http://dro.hcnkem.com

UserId = int
来源：http://agw.zhoulong.xyz

[U29] Py：属性校验
来源：http://ehn.yuanzhike.top

@property 与 @x.setter 配合
来源：http://iis.haohaochexian.top

[U30] Py：数据类
来源：http://oln.redwolf501.top

@dataclass(slots=True)
来源：http://zio.shangyingyoupin.top

[U31] Py：单测
来源：http://ven.tianlin.xyz

python -m pytest -q
来源：http://ezp.cucudq.cn

[U32] Py：代码格式化
来源：http://uak.zhiwuduotai.top

ruff format . && ruff check --fix .
来源：http://jjt.zhiwuduotai.top

[U33] Py：打包发布
来源：http://rje.nwbrower.top

python -m build  （依赖 pyproject.toml）
来源：http://hfq.shanyushiyangtech.top

[U34] Py：判断编码
来源：http://xpn.redwolf501.top

chardet.detect(raw)
来源：http://qkp.hfpthk.cn

[U35] Py：发送邮件
来源：http://dzp.andypj.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://poz.jiagoushi.top

[U36] Py：定时任务
来源：http://trl.gogol.net.cn

schedule.every(10).minutes.do(job)
来源：http://yuu.c1oappe.top

[U37] Py：读写 Excel
来源：http://qht.cdnleiting.top

pandas.read_excel / DataFrame.to_excel
来源：http://cin.daxiang520.top

[U38] Py：获取脚本所在目录
来源：http://plc.hnqzz.top

Path(__file__).resolve().parent
来源：http://nah.birdmap.top

[U39] Py：判断是否在交互环境
来源：http://wto.bbcook.cn

sys.stdout.isatty()
来源：http://jtv.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://jij.hammf.cn

print("err", file=sys.stderr)
来源：http://cki.ivvv.top

[U41] PHP：初始化 Composer 项目
来源：http://xzf.hcnkem.com

composer init;  composer require guzzlehttp/guzzle
来源：http://dlp.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://lqp.xingfuxueyuan.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bkp.jqgufenzy.top

[U43] PHP：声明命名空间
来源：http://vkg.jlsjyb.cn

namespace App\Http;
来源：http://crn.daxiang520.top

[U44] PHP：开启严格类型
来源：http://ehe.iojbl.cn

declare(strict_types=1);
来源：http://vnb.svipenyu.cn

[U45] PHP：类型声明与返回类型
来源：http://ryu.ywan-chungtsiang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mzz.dianchejie.cn

[U46] PHP：可空类型
来源：http://mdy.vehdjk.com

?string $name = null
来源：http://apv.daxiang520.top

[U47] PHP：联合类型
来源：http://ech.aibaodan.cn

int|string $id
来源：http://nvx.sjlbkw.cn

[U48] PHP：纯枚举
来源：http://naz.hnxiangtu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xvb.bjfxy.top

[U49] PHP：只读属性
来源：http://cwx.chenjidiqi.icu

public readonly string $name
来源：http://ctc.yueranfly.top

[U50] PHP：构造器属性提升
来源：http://fgi.tanke756.top

public function __construct(private int $id) {}
来源：http://dla.hongshengwenyu.top

[U51] PHP：数组解构
来源：http://uvf.hcnkem.com

[$a, $b] = $arr;
来源：http://eia.jlsjyb.cn

[U52] PHP：箭头函数
来源：http://qwy.hcnkem.com

$double = fn($x) => $x * 2;
来源：http://nrr.yanxiufei.cn

[U53] PHP：空合并运算符
来源：http://nlz.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://oif.feifeiyinyue.top

[U54] PHP：空安全调用
来源：http://dyq.zycfv.cn

$obj?->method()
来源：http://jag.fktsv.cn

[U55] PHP：match 表达式
来源：http://kms.shanyushiyangtech.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hmz.shanyushiyangkeji.top

[U56] PHP：命名参数
来源：http://foz.iojbl.cn

f(a: 1, b: 2)
来源：http://vzn.xinyue.icu

[U57] PHP：字符串插值
来源：http://ezy.c1oappe.top

"值: {$a}"
来源：http://jvo.uphjek.com

[U58] PHP：数组三件套
来源：http://tqf.hongshengwenyu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gvq.yj202588.top

[U59] PHP：自定义排序
来源：http://dbn.daxiang520.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hon.nanxinkj.top

[U60] PHP：JSON 编解码
来源：http://jzd.fktsv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hul.cdnleiting.top

[U61] PHP：正则
来源：http://mrv.shzxlz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yyd.kuanghao11.cn

[U62] PHP：日期对象
来源：http://cod.fanxiaobao.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aou.birdmap.top

[U63] PHP：文件读写
来源：http://wse.svipenyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jpi.gzhubu.top

[U64] PHP：目录遍历
来源：http://xfx.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://som.sysykeji.top

[U65] PHP：会话
来源：http://mmb.hesvh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://soo.yvedp.cn

[U66] PHP：设置 Cookie
来源：http://azs.aizwys.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fin.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://nra.zdbjq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lpf.ydzc1.top

[U68] PHP：PDO 连接
来源：http://jqt.meibo888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xrq.guannengcc.top

[U69] PHP：PDO 预处理
来源：http://uhf.zdqjudy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cev.zhijiandao.cn

[U70] PHP：PDO 事务
来源：http://lwp.yanxiufei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hxz.jiagoushi.top

[U71] PHP：抛出异常
来源：http://jxr.smart0.xyz

throw new RuntimeException("失败", 500);
来源：http://cwm.fehbvm.com

[U72] PHP：写错误日志
来源：http://vrq.nanxinkj.top

error_log("失败: " . $e->getMessage());
来源：http://ehl.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://cuf.shanyushiyangtech.top

parse_ini_file("config.ini", true)
来源：http://oub.cucudq.cn

[U74] PHP：读取环境变量
来源：http://kwl.ydzc1.top

getenv("APP_ENV") ?: "production"
来源：http://zts.zhixingplan.top

[U75] PHP：依赖注入
来源：http://uzd.gogol.net.cn

composer require psr/container
来源：http://ogp.epnwcf.com

[U76] PHP：简单路由
来源：http://xko.9152youxi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nyw.tanke756.top

[U77] PHP：模板渲染
来源：http://lww.pycfn.com

composer require twig/twig
来源：http://vuz.hnxiangtu.top

[U78] PHP：单元测试
来源：http://ryf.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://asf.sufxvd.cn

[U79] PHP：静态分析
来源：http://jlw.zhaomingkeji.xyz

composer require --dev phpstan/phpstan
来源：http://dji.pengpengdd.cyou

[U80] PHP：代码规范修复
来源：http://oam.ctjpmb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ffi.jinqigufen.top

[U81] JS：初始化项目
来源：http://wqk.zhixingplan.top

npm init -y;  npm i express
来源：http://fkm.jqgufenzy.top

[U82] JS：package.json 脚本
来源：http://bmr.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eat.cdnleiting.top

[U83] JS：ES Module 导入导出
来源：http://eqd.ydjk.org.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cuo.9152youxi.cn

[U84] JS：CommonJS 写法
来源：http://qyu.yongpay.top

module.exports = { a };  const { a } = require("./m");
来源：http://kcb.cdnleiting.top

[U85] JS：可选链
来源：http://mwq.gzhubu.top

a?.b?.c
来源：http://qwx.daria6918.cn

[U86] JS：空值合并
来源：http://izy.jiagoushi.top

a ?? b
来源：http://qwa.zhijiandao.cn

[U87] JS：解构默认值
来源：http://jrt.9152youxi.cn

const { a = 1, b = 2 } = obj;
来源：http://ter.jiagoushi.top

[U88] JS：对象展开合并
来源：http://usd.ybcxt.top

{ ...a, ...b }
来源：http://bqq.zhengqikj.top

[U89] JS：数组去重
来源：http://dgs.yongpay.top

[...new Set(arr)]
来源：http://xbn.tarul.cn

[U90] JS：数字数组排序
来源：http://djn.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://mis.hcnkem.com

[U91] JS：对象键值遍历
来源：http://lct.zhoulong.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qxf.jinqigufen.top

[U92] JS：深拷贝
来源：http://ctu.dianchejie.cn

structuredClone(obj)
来源：http://kem.chenlongwang.top

[U93] JS：模板字符串
来源：http://lcj.zhoulong.xyz

`共 ${n} 条`
来源：http://ybl.ehwqpu.com

[U94] JS：箭头函数
来源：http://lty.sweek.top

const double = x => x * 2;
来源：http://bfv.yfazqb.com

[U95] JS：Promise 包装
来源：http://kfo.zdqjudy.top

new Promise((resolve, reject) => {})
来源：http://ypn.shuidangran.top

[U96] JS：async/await 与异常
来源：http://lqp.quarkkingdee.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tsi.pycfn.com

[U97] JS：并发请求
来源：http://wgu.fengsongda.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://inn.haohaochexian.top

[U98] JS：fetch 带 JSON
来源：http://ajo.snrcjt.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hkt.ydjk.org.cn

[U99] JS：事件监听
来源：http://gvn.yfazqb.com

el.addEventListener("click", e => {})
来源：http://rhw.xziqi.cn

[U100] JS：DOM 查询
来源：http://dto.ctjpmb.com

document.querySelector(".item")
来源：http://pxi.sysykeji.top

[U101] JS：classList 操作
来源：http://xrs.nanxuanxn.top

el.classList.toggle("active")
来源：http://cvg.ydjk.org.cn

[U102] JS：本地存储
来源：http://cmm.sjlbkw.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ayt.jlsjyb.cn

[U103] JS：定时器
来源：http://jpy.gotoacloud.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fug.yj20258.top

[U104] JS：防抖
来源：http://xuz.havefunace.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ugs.nanxinkj.top

[U105] JS：节流
来源：http://waz.jiagoushi.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rxp.yuanzhike.top

[U106] JS：日期格式化
来源：http://ime.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dqz.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://gil.fktsv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ysz.yangfankeji.com

[U108] JS：随机整数
来源：http://mye.wangshuangyany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://txx.bjfxy.top

[U109] JS：数组分组
来源：http://zzj.hcnkem.com

Object.groupBy(arr, x => x.type)
来源：http://dyv.yangfankeji.com

[U110] JS：数组分块
来源：http://fpw.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ffz.jianghu66.top

[U111] JS：对象转 Map
来源：http://fer.xziqi.cn

new Map(Object.entries(obj))
来源：http://lyi.vehdjk.com

[U112] JS：字符串补位
来源：http://nbm.andypj.xyz

"7".padStart(3, "0")
来源：http://amf.cheryme.top

[U113] JS：正则替换全部
来源：http://bwb.dashuyun.cn

s.replaceAll("a", "b")
来源：http://opd.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://bqd.haohaochexian.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://esc.ppjwa.cn

[U115] JS：生成 UUID
来源：http://gdc.sjlbkw.cn

crypto.randomUUID()
来源：http://fpy.cqqwz.cn

[U116] JS：类型检查（JSDoc）
来源：http://ptm.nwbrower.top

/** @param {string} name */ function f(name) {}
来源：http://znh.jqgfzy.top

[U117] JS：单元测试
来源：http://btk.epnwcf.com

npm i -D vitest;  npx vitest
来源：http://srs.cucudq.cn

[U118] JS：开发服务器
来源：http://brh.shzxlz.cn

npm i -D vite;  npx vite
来源：http://ucx.jqgufenzy.top

[U119] JS：生产构建
来源：http://hxf.zdqjudy.top

npx vite build
来源：http://yga.xziqi.cn

[U120] JS：读取环境变量（Vite）
来源：http://cjy.daria6918.cn

import.meta.env.VITE_API_URL
来源：http://eql.yj20258888.top

================================================================================
来源：http://zco.yuanzhike.top

统计汇总
来源：http://orn.fehbvm.com

================================================================================
来源：http://gnn.zhaomingkeji.xyz

按语言统计（条）：
来源：http://nms.nanxuanxn.top

Python ......... 252
来源：http://mpj.yvedp.cn

PHP ............ 252
来源：http://fwy.zhijiandao.cn

JavaScript ..... 252
来源：http://wcs.jqgufenzy.top

TypeScript ..... 212
来源：http://ihf.jlsjyb.cn

Java ........... 212
来源：http://brs.xinyue.icu

Go ............. 212
来源：http://lcw.zhiwuduotai.top

Ruby ........... 212
来源：http://vjz.andypj.xyz

C# ............. 212
来源：http://deu.jqgufenzy.top

C .............. 30
来源：http://ylf.vqdsnc.cn

C++ ............ 30
来源：http://cfq.zhoulong.xyz

SQL ............ 90
来源：http://eyh.hongshengwenyu.top

Bash ........... 80
来源：http://urs.ctjpmb.com


<!-- 参考信息 -->