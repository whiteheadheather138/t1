代发 wailian999

[T37] Lua：字符串拼接
来源：http://nvj.tanke756.top

"a" .. "b"
来源：http://kxr.sweek.top

[T38] Lua：条件
来源：http://hiu.hongshengwenyu.top

if x > 0 then print("正") end
来源：http://qic.yueranfly.top

[T39] Lua：模式匹配
来源：http://ene.zycfv.cn

string.find(s, "%d+")
来源：http://hsx.zhixingplan.top

[T40] Lua：元表
来源：http://bam.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://obi.aizwys.cn

[T41] Perl：Hello World
来源：http://itt.fengsongda.top

print "Hello\n";
来源：http://izi.gaohongyu789.top

[T42] Perl：变量类型
来源：http://uze.dashuyun.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vcq.zdbjq.cn

[T43] Perl：字符串插值
来源：http://ycg.ctjpmb.com

"值: $a"
来源：http://orp.ehwqpu.com

[T44] Perl：条件
来源：http://ubb.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://mnx.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://mvq.sufxvd.cn

for my $x (@arr) { print $x; }
来源：http://fyd.zdqjudy.top

[T46] Perl：哈希操作
来源：http://odz.jinqigufen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fas.hfpthk.cn

[T47] Perl：正则捕获
来源：http://zyh.jlsjyb.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mvw.smart0.xyz

[T48] Perl：正则替换
来源：http://joq.xylfe.cn

$s =~ s/old/new/g;
来源：http://xhv.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://lbi.zhiwuduotai.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://shp.hongshengwenyu.top

[T50] Perl：逐行读文件
来源：http://pkg.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gde.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://qkf.zhaomingkeji.xyz

[T51] Scala：Hello World
来源：http://aqe.redwolf501.top

println("Hello")
来源：http://fqf.0kj1m.cn

[T52] Scala：变量
来源：http://wme.fzhhl.top

val a = 1;  var b = 2
来源：http://jxg.ppjwa.cn

[T53] Scala：字符串插值
来源：http://uyk.daxiang520.top

s"值: $b"
来源：http://mvv.wangdashe.top

[T54] Scala：集合映射
来源：http://yhb.jqgufenzy.top

List(1, 2, 3).map(_ * 2)
来源：http://ujg.gzhubu.top

[T55] Scala：集合过滤
来源：http://gfv.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://keo.sjlbkw.cn

[T56] Scala：样例类
来源：http://bhe.xuetiantiany.cn

case class User(name: String, age: Int)
来源：http://yyf.shzxlz.cn

[T57] Scala：模式匹配
来源：http://msy.zhengqikj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zhf.haohaochexian.top

[T58] Scala：函数定义
来源：http://ubd.daxiang520.top

def add(a: Int, b: Int): Int = a + b
来源：http://kbs.wangdashe.top

[T59] Scala：循环
来源：http://dcf.fktsv.cn

for (i <- 1 to 10) println(i)
来源：http://won.hysaishi.cn

[T60] Scala：折叠
来源：http://ofm.sxryk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hqf.9152youxi.cn

================================================================================
来源：http://ftf.zhixingplan.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zdp.zycfv.cn

================================================================================
来源：http://xjd.yongpay.top

[U01] Py：创建虚拟环境
来源：http://cii.mhx1999.top

python -m venv .venv && source .venv/bin/activate
来源：http://dbp.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://pqi.fktsv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bkv.chenjidiqi.icu

[U03] Py：加载 .env 配置
来源：http://vvs.redwolf501.top

from dotenv import load_dotenv; load_dotenv()
来源：http://shc.hammf.cn

[U04] Py：变量调试打印
来源：http://yrd.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ebz.gzhubu.top

[U05] Py：列表去重且保序
来源：http://gpt.wangdashe.top

list(dict.fromkeys(arr))
来源：http://boc.yuxming.cn

[U06] Py：合并两个字典
来源：http://pjo.vqdsnc.cn

{**a, **b}
来源：http://fhf.hammf.cn

[U07] Py：反转字典键值
来源：http://xdj.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://let.hongshengwenyu.top

[U08] Py：展平二维列表
来源：http://cof.chenjidiqi.icu

[y for x in nested for y in x]
来源：http://abq.yonumen.top

[U09] Py：字典取最大值的键
来源：http://sga.gotoacloud.top

max(d, key=d.get)
来源：http://gcm.aizwys.cn

[U10] Py：按值排序字典
来源：http://yza.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dcx.cdnleiting.top

[U11] Py：生成器表达式
来源：http://mln.yanxiufei.cn

(x * 2 for x in arr)
来源：http://cra.ehwqpu.com

[U12] Py：取出现最多的 3 个元素
来源：http://vkw.xylfe.cn

Counter(arr).most_common(3)
来源：http://iiv.fktsv.cn

[U13] Py：固定长度队列
来源：http://xqr.daria6918.cn

deque(maxlen=10)
来源：http://qxh.yvedp.cn

[U14] Py：分组收集到列表
来源：http://apq.sysykeji.top

defaultdict(list)
来源：http://nlp.jianghu66.top

[U15] Py：高精度计时
来源：http://elr.jqgfzy.top

t = time.perf_counter()
来源：http://iaw.xylfe.cn

[U16] Py：命令行参数解析
来源：http://gfa.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://orz.jianghu66.top

[U17] Py：初始化日志
来源：http://vlv.cqqwz.cn

logging.basicConfig(level=logging.INFO)
来源：http://qsh.tarul.cn

[U18] Py：预编译正则
来源：http://ajj.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://mxq.tianlin.xyz

[U19] Py：正则替换带回调
来源：http://ezh.shuidangran.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sdw.0kj1m.cn

[U20] Py：缓存函数结果
来源：http://kry.xziqi.cn

@functools.lru_cache(maxsize=None)
来源：http://ljz.snrcjt.cn

[U21] Py：自定义上下文管理器
来源：http://zrj.birdmap.top

@contextlib.contextmanager
来源：http://qrj.tarul.cn

[U22] Py：矩阵转置
来源：http://gsu.hnxiangtu.top

list(zip(*m))
来源：http://vzx.cashguo.top

[U23] Py：分块读取大文件
来源：http://ouz.daria6918.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ysc.sxryk.cn

[U24] Py：路径操作
来源：http://qkf.bbcook.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bgm.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://zbs.jianghu66.top

csv.DictReader(f)
来源：http://uff.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://plr.daria6918.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aqe.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://zil.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://woc.tanke756.top

[U28] Py：类型别名
来源：http://bud.ppjwa.cn

UserId = int
来源：http://itx.cucudq.cn

[U29] Py：属性校验
来源：http://qbf.guannengcc.top

@property 与 @x.setter 配合
来源：http://qwb.nanxinkj.top

[U30] Py：数据类
来源：http://tgu.zhoulong.xyz

@dataclass(slots=True)
来源：http://ehg.yj202588.top

[U31] Py：单测
来源：http://zni.dashuyun.cn

python -m pytest -q
来源：http://oan.yfazqb.com

[U32] Py：代码格式化
来源：http://rmq.ivvv.top

ruff format . && ruff check --fix .
来源：http://znt.yongpay.top

[U33] Py：打包发布
来源：http://qrl.gaohongyu789.top

python -m build  （依赖 pyproject.toml）
来源：http://lgi.bbcook.cn

[U34] Py：判断编码
来源：http://dtk.jianghu66.top

chardet.detect(raw)
来源：http://lhu.aizwys.cn

[U35] Py：发送邮件
来源：http://otj.tanke756.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tqv.guowangkeji.top

[U36] Py：定时任务
来源：http://hgb.hnqzz.top

schedule.every(10).minutes.do(job)
来源：http://bgz.guannengcc.top

[U37] Py：读写 Excel
来源：http://ybu.zhongyouzk.top

pandas.read_excel / DataFrame.to_excel
来源：http://ixq.sweek.top

[U38] Py：获取脚本所在目录
来源：http://hkm.zhixingplan.top

Path(__file__).resolve().parent
来源：http://znc.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://tsz.zhaomingkeji.xyz

sys.stdout.isatty()
来源：http://dpl.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://gqd.shanyushiyangtech.top

print("err", file=sys.stderr)
来源：http://qcl.aibaodan.cn

[U41] PHP：初始化 Composer 项目
来源：http://qru.cqqwz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lzq.ywan-chungtsiang.top

[U42] PHP：PSR-4 自动加载
来源：http://fsb.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hmy.dianchejie.cn

[U43] PHP：声明命名空间
来源：http://odm.fktsv.cn

namespace App\Http;
来源：http://snv.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://idh.hammf.cn

declare(strict_types=1);
来源：http://sqi.zhaomingkeji.xyz

[U45] PHP：类型声明与返回类型
来源：http://gah.fehbvm.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://lws.aizwys.cn

[U46] PHP：可空类型
来源：http://cfk.feifeiyinyue.top

?string $name = null
来源：http://sky.vehdjk.com

[U47] PHP：联合类型
来源：http://ncb.vqdsnc.cn

int|string $id
来源：http://kav.zdbjq.cn

[U48] PHP：纯枚举
来源：http://obv.wangdashe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dtu.pengpengdd.cyou

[U49] PHP：只读属性
来源：http://rsk.bjfxy.top

public readonly string $name
来源：http://ijo.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://yns.svipenyu.cn

public function __construct(private int $id) {}
来源：http://ftm.jinyuanbaomall.cn

[U51] PHP：数组解构
来源：http://dbp.zdbjq.cn

[$a, $b] = $arr;
来源：http://mzr.tian-w.cn

[U52] PHP：箭头函数
来源：http://jvs.hongshengwenyu.top

$double = fn($x) => $x * 2;
来源：http://qbw.xuanzx.com

[U53] PHP：空合并运算符
来源：http://meo.jinqigfzy.top

$v = $a ?? $b ?? "default";
来源：http://juv.yueranfly.top

[U54] PHP：空安全调用
来源：http://idz.chenzaomai.com

$obj?->method()
来源：http://fvw.vehdjk.com

[U55] PHP：match 表达式
来源：http://xle.dashuyun.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qzs.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://bpd.snrcjt.cn

f(a: 1, b: 2)
来源：http://jao.cdnleiting.top

[U57] PHP：字符串插值
来源：http://dye.shuidangran.top

"值: {$a}"
来源：http://bpp.uphjek.com

[U58] PHP：数组三件套
来源：http://odi.shanyushiyangtech.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://udy.fzhhl.top

[U59] PHP：自定义排序
来源：http://xbz.zhaomingkeji.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ney.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://arp.gogol.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://goh.ywan-chungtsiang.top

[U61] PHP：正则
来源：http://zwe.zhijiandao.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tgp.uphjek.com

[U62] PHP：日期对象
来源：http://gus.jianghu66.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cct.zycfv.cn

[U63] PHP：文件读写
来源：http://oju.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vrm.zhaomingkeji.xyz

[U64] PHP：目录遍历
来源：http://tac.uphjek.com

glob("dir/*.php");  scandir("dir");
来源：http://srh.guowangkeji.top

[U65] PHP：会话
来源：http://svw.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wja.ywan-chungtsiang.top

[U66] PHP：设置 Cookie
来源：http://kqd.ivvv.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kro.zhongyouzk.top

[U67] PHP：处理文件上传
来源：http://lfl.kuanghao11.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vgu.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://izo.hnxiangtu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ech.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://jfl.gzhubu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://khm.jianghu66.top

[U70] PHP：PDO 事务
来源：http://aie.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://juw.zdbjq.cn

[U71] PHP：抛出异常
来源：http://tqh.9152youxi.cn

throw new RuntimeException("失败", 500);
来源：http://san.sufxvd.cn

[U72] PHP：写错误日志
来源：http://bcx.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://hrw.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://znn.ydzc1.top

parse_ini_file("config.ini", true)
来源：http://bzi.ydzc1.top

[U74] PHP：读取环境变量
来源：http://fcv.yuanzhike.top

getenv("APP_ENV") ?: "production"
来源：http://daw.cucudq.cn

[U75] PHP：依赖注入
来源：http://gip.ybcxt.top

composer require psr/container
来源：http://ext.sysykeji.top

[U76] PHP：简单路由
来源：http://anj.jiagoushi.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ono.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://uly.haohaochexian.top

composer require twig/twig
来源：http://flg.sweek.top

[U78] PHP：单元测试
来源：http://xot.yanxiufei.cn

composer require --dev phpunit/phpunit
来源：http://oxk.ybcxt.top

[U79] PHP：静态分析
来源：http://aex.hnqzz.top

composer require --dev phpstan/phpstan
来源：http://gyp.daxiang520.top

[U80] PHP：代码规范修复
来源：http://ufw.jqgfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://twh.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://dul.xuetiantiany.cn

npm init -y;  npm i express
来源：http://lqp.sweek.top

[U82] JS：package.json 脚本
来源：http://xkg.meibo888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ttm.shuidangran.top

[U83] JS：ES Module 导入导出
来源：http://vur.jiagoushi.top

export const a = 1;  import { a } from "./m.js";
来源：http://kst.shanyushiyangkeji.top

[U84] JS：CommonJS 写法
来源：http://acs.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ibp.jinqigfzy.top

[U85] JS：可选链
来源：http://izk.shanyushiyangtech.top

a?.b?.c
来源：http://ala.hysaishi.cn

[U86] JS：空值合并
来源：http://isa.xylfe.cn

a ?? b
来源：http://qbr.jianghu66.top

[U87] JS：解构默认值
来源：http://klq.yj202588.top

const { a = 1, b = 2 } = obj;
来源：http://jxt.fehbvm.com

[U88] JS：对象展开合并
来源：http://ibr.yuxming.cn

{ ...a, ...b }
来源：http://gdj.tanke756.top

[U89] JS：数组去重
来源：http://sdb.yfazqb.com

[...new Set(arr)]
来源：http://lhv.ywan-chungtsiang.top

[U90] JS：数字数组排序
来源：http://lzj.fehbvm.com

[...arr].sort((a, b) => a - b)
来源：http://gtj.yonumen.top

[U91] JS：对象键值遍历
来源：http://ydf.zhengqikj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://npr.shanyushiyangkeji.top

[U92] JS：深拷贝
来源：http://aof.cucudq.cn

structuredClone(obj)
来源：http://yqz.zycfv.cn

[U93] JS：模板字符串
来源：http://pad.hammf.cn

`共 ${n} 条`
来源：http://mkx.tian-w.cn

[U94] JS：箭头函数
来源：http://vpe.ctjpmb.com

const double = x => x * 2;
来源：http://jtj.hywenlv.cn

[U95] JS：Promise 包装
来源：http://nut.shangyingyoupin.top

new Promise((resolve, reject) => {})
来源：http://hax.ybcxt.top

[U96] JS：async/await 与异常
来源：http://nrz.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://csd.hesvh.cn

[U97] JS：并发请求
来源：http://cwt.zhengqikj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fof.shangyingyoupin.top

[U98] JS：fetch 带 JSON
来源：http://lad.sjlbkw.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hff.tian-w.cn

[U99] JS：事件监听
来源：http://lxo.yj20258888.top

el.addEventListener("click", e => {})
来源：http://pft.kuanghao11.cn

[U100] JS：DOM 查询
来源：http://euc.yangfankeji.com

document.querySelector(".item")
来源：http://gil.chenlongwang.top

[U101] JS：classList 操作
来源：http://afc.nwbrower.top

el.classList.toggle("active")
来源：http://xov.zycfv.cn

[U102] JS：本地存储
来源：http://qql.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kfb.jiagoushi.top

[U103] JS：定时器
来源：http://jje.xuetiantiany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wxd.xuanzx.com

[U104] JS：防抖
来源：http://wpq.redwolf501.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iic.zhengqikj.top

[U105] JS：节流
来源：http://luh.zhengqikj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://swk.andypj.xyz

[U106] JS：日期格式化
来源：http://ago.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kla.aizwys.cn

[U107] JS：数字千分位
来源：http://pik.yfazqb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mbf.wangdashe.top

[U108] JS：随机整数
来源：http://exk.yj202588.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wqq.yongpay.top

[U109] JS：数组分组
来源：http://gek.cheryme.top

Object.groupBy(arr, x => x.type)
来源：http://dpd.hesvh.cn

[U110] JS：数组分块
来源：http://btp.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nsu.yonumen.top

[U111] JS：对象转 Map
来源：http://wuw.sufxvd.cn

new Map(Object.entries(obj))
来源：http://okt.vehdjk.com

[U112] JS：字符串补位
来源：http://suz.sysykeji.top

"7".padStart(3, "0")
来源：http://ukf.ppjwa.cn

[U113] JS：正则替换全部
来源：http://olu.epnwcf.com

s.replaceAll("a", "b")
来源：http://fjy.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://sbv.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://utr.fanxiaobao.xyz

[U115] JS：生成 UUID
来源：http://cxd.xylfe.cn

crypto.randomUUID()
来源：http://vka.gotoacloud.top

[U116] JS：类型检查（JSDoc）
来源：http://rom.jinqigufen.top

/** @param {string} name */ function f(name) {}
来源：http://jrq.ehwqpu.com

[U117] JS：单元测试
来源：http://ggm.guowangkeji.top

npm i -D vitest;  npx vitest
来源：http://ofr.jinqigfzy.top

[U118] JS：开发服务器
来源：http://ryz.jinghuilouyu.cn

npm i -D vite;  npx vite
来源：http://dnr.xuanzx.com

[U119] JS：生产构建
来源：http://hga.uphjek.com

npx vite build
来源：http://vtl.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://vjy.cucudq.cn

import.meta.env.VITE_API_URL
来源：http://obq.chenjidiqi.icu

================================================================================
来源：http://xgr.hnqzz.top

统计汇总
来源：http://udn.yfazqb.com

================================================================================
来源：http://rpy.hysaishi.cn

按语言统计（条）：
来源：http://bih.mhx1999.top

Python ......... 252
来源：http://ntz.zhaomingkeji.xyz

PHP ............ 252
来源：http://ruu.chenzaomai.com

JavaScript ..... 252
来源：http://bgh.xylfe.cn

TypeScript ..... 212
来源：http://vih.chenjidiqi.icu


<!-- 参考信息 -->