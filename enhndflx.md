代发 wailian999

[T37] Lua：字符串拼接
来源：http://jue.yonumen.top

"a" .. "b"
来源：http://isq.nwbrower.top

[T38] Lua：条件
来源：http://lhc.cheryme.top

if x > 0 then print("正") end
来源：http://vqx.tianlin.xyz

[T39] Lua：模式匹配
来源：http://lxp.fengsongda.top

string.find(s, "%d+")
来源：http://yeh.jyoumei.cn

[T40] Lua：元表
来源：http://mwg.vehdjk.com

setmetatable({}, { __index = base })
来源：http://tfd.dashuyun.cn

[T41] Perl：Hello World
来源：http://jki.zdqjudy.top

print "Hello\n";
来源：http://qum.yj202588.top

[T42] Perl：变量类型
来源：http://zlw.sweek.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qzt.chenjidiqi.icu

[T43] Perl：字符串插值
来源：http://xrz.shangyingyoupin.top

"值: $a"
来源：http://vui.fehbvm.com

[T44] Perl：条件
来源：http://ztq.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://sbp.xinyue.icu

[T45] Perl：数组遍历
来源：http://rjg.pengpengdd.cyou

for my $x (@arr) { print $x; }
来源：http://nhn.hesvh.cn

[T46] Perl：哈希操作
来源：http://aok.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vru.yueranfly.top

[T47] Perl：正则捕获
来源：http://jvz.yj20258.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mpc.sysykeji.top

[T48] Perl：正则替换
来源：http://shn.jinqigufen.top

$s =~ s/old/new/g;
来源：http://rxk.nanxinkj.top

[T49] Perl：函数
来源：http://zye.pengpengdd.cyou

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lcj.epnwcf.com

[T50] Perl：逐行读文件
来源：http://den.zdbjq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dpq.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://alk.jlsjyb.cn

[T51] Scala：Hello World
来源：http://sgk.nanxinkj.top

println("Hello")
来源：http://dai.jinghuilouyu.cn

[T52] Scala：变量
来源：http://lmd.smart0.xyz

val a = 1;  var b = 2
来源：http://lbo.yonumen.top

[T53] Scala：字符串插值
来源：http://agt.jlsjyb.cn

s"值: $b"
来源：http://syk.vqdsnc.cn

[T54] Scala：集合映射
来源：http://chf.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://kux.daxiang520.top

[T55] Scala：集合过滤
来源：http://kkm.feifeiyinyue.top

List(1, 2, 3).filter(_ > 1)
来源：http://smt.tian-w.cn

[T56] Scala：样例类
来源：http://yie.pycfn.com

case class User(name: String, age: Int)
来源：http://haf.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://pqy.jinqigufen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://tzv.yongpay.top

[T58] Scala：函数定义
来源：http://xpc.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://fpp.cqqwz.cn

[T59] Scala：循环
来源：http://qnh.gaohongyu789.top

for (i <- 1 to 10) println(i)
来源：http://oaf.0kj1m.cn

[T60] Scala：折叠
来源：http://fnh.yueranfly.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iec.xingfuxueyuan.xyz

================================================================================
来源：http://mbp.iojbl.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rbs.sxryk.cn

================================================================================
来源：http://lbj.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://ner.epnwcf.com

python -m venv .venv && source .venv/bin/activate
来源：http://jxc.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://lpc.wangshuangyany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ycd.wangdashe.top

[U03] Py：加载 .env 配置
来源：http://mfa.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dpz.pengpengdd.cyou

[U04] Py：变量调试打印
来源：http://myh.fengsongda.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ula.ydjk.org.cn

[U05] Py：列表去重且保序
来源：http://ahp.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://kda.chenlongwang.top

[U06] Py：合并两个字典
来源：http://mul.hammf.cn

{**a, **b}
来源：http://oeu.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://yax.uphjek.com

{v: k for k, v in d.items()}
来源：http://cht.guowangkeji.top

[U08] Py：展平二维列表
来源：http://vdl.xuanzx.com

[y for x in nested for y in x]
来源：http://lni.xinyue.icu

[U09] Py：字典取最大值的键
来源：http://imx.hongshengwenyu.top

max(d, key=d.get)
来源：http://wuj.ctjpmb.com

[U10] Py：按值排序字典
来源：http://jbh.fehbvm.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zqr.bbcook.cn

[U11] Py：生成器表达式
来源：http://tgp.zhiwuduotai.top

(x * 2 for x in arr)
来源：http://ydc.cdnleiting.top

[U12] Py：取出现最多的 3 个元素
来源：http://zqo.jqgufenzy.top

Counter(arr).most_common(3)
来源：http://tsa.smart0.xyz

[U13] Py：固定长度队列
来源：http://xku.jlsjyb.cn

deque(maxlen=10)
来源：http://enx.fehbvm.com

[U14] Py：分组收集到列表
来源：http://ctq.ywan-chungtsiang.top

defaultdict(list)
来源：http://znp.zhoulong.xyz

[U15] Py：高精度计时
来源：http://yuj.ybcxt.top

t = time.perf_counter()
来源：http://vmc.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://zej.ywan-chungtsiang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wvv.ydzc1.top

[U17] Py：初始化日志
来源：http://vzl.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://ohf.nanxuanxn.top

[U18] Py：预编译正则
来源：http://mql.yonumen.top

pat = re.compile(r"\d+")
来源：http://yjo.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://dwd.vqdsnc.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wsv.sufxvd.cn

[U20] Py：缓存函数结果
来源：http://iwm.zycfv.cn

@functools.lru_cache(maxsize=None)
来源：http://nfu.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://eky.ivvv.top

@contextlib.contextmanager
来源：http://xrr.daria6918.cn

[U22] Py：矩阵转置
来源：http://ffn.zhengqikj.top

list(zip(*m))
来源：http://ags.bjfxy.top

[U23] Py：分块读取大文件
来源：http://bce.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gqq.gogol.net.cn

[U24] Py：路径操作
来源：http://rkw.c1oappe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mtu.jianghu66.top

[U25] Py：CSV 按字典读
来源：http://jqs.jinghuilouyu.cn

csv.DictReader(f)
来源：http://zjw.shangyingyoupin.top

[U26] Py：并发下载
来源：http://fko.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mrg.tanke756.top

[U27] Py：异步 HTTP
来源：http://cbk.yonumen.top

aiohttp.ClientSession() 配合 async with
来源：http://dyj.svipenyu.cn

[U28] Py：类型别名
来源：http://ath.dianchejie.cn

UserId = int
来源：http://fur.hfpthk.cn

[U29] Py：属性校验
来源：http://tnl.zhixingplan.top

@property 与 @x.setter 配合
来源：http://uic.cdnleiting.top

[U30] Py：数据类
来源：http://rpv.jqgfzy.top

@dataclass(slots=True)
来源：http://qna.jianghu66.top

[U31] Py：单测
来源：http://rrc.fengsongda.top

python -m pytest -q
来源：http://xxa.svipenyu.cn

[U32] Py：代码格式化
来源：http://edb.chenjidiqi.icu

ruff format . && ruff check --fix .
来源：http://fuo.jinyuanbaomall.cn

[U33] Py：打包发布
来源：http://nas.zhoulong.xyz

python -m build  （依赖 pyproject.toml）
来源：http://uyh.aizwys.cn

[U34] Py：判断编码
来源：http://agg.snrcjt.cn

chardet.detect(raw)
来源：http://qjf.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://aho.sjlbkw.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sio.zdqjudy.top

[U36] Py：定时任务
来源：http://ebi.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://hsn.wangdashe.top

[U37] Py：读写 Excel
来源：http://nwg.hongshengwenyu.top

pandas.read_excel / DataFrame.to_excel
来源：http://zsr.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://lyh.chenlongwang.top

Path(__file__).resolve().parent
来源：http://gki.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://hyf.ivvv.top

sys.stdout.isatty()
来源：http://qks.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://auh.zhiwuduotai.top

print("err", file=sys.stderr)
来源：http://qrh.birdmap.top

[U41] PHP：初始化 Composer 项目
来源：http://uaz.chenzaomai.com

composer init;  composer require guzzlehttp/guzzle
来源：http://iss.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://tdr.zdbjq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://crn.zycfv.cn

[U43] PHP：声明命名空间
来源：http://nyt.svipenyu.cn

namespace App\Http;
来源：http://uoz.yanxiufei.cn

[U44] PHP：开启严格类型
来源：http://glx.yuanzhike.top

declare(strict_types=1);
来源：http://lzg.wangdashe.top

[U45] PHP：类型声明与返回类型
来源：http://axx.nanxinkj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ydm.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://rig.jinqigufen.top

?string $name = null
来源：http://brs.xinyue.icu

[U47] PHP：联合类型
来源：http://fza.316326.xyz

int|string $id
来源：http://zyw.ivvv.top

[U48] PHP：纯枚举
来源：http://msy.yanxiufei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fzh.meibo888.top

[U49] PHP：只读属性
来源：http://wgo.hywenlv.cn

public readonly string $name
来源：http://gbk.fanxiaobao.xyz

[U50] PHP：构造器属性提升
来源：http://lhi.fengsongda.top

public function __construct(private int $id) {}
来源：http://gae.gaohongyu789.top

[U51] PHP：数组解构
来源：http://dtb.yueranfly.top

[$a, $b] = $arr;
来源：http://edu.sysykeji.top

[U52] PHP：箭头函数
来源：http://owq.xuanzx.com

$double = fn($x) => $x * 2;
来源：http://mut.svipenyu.cn

[U53] PHP：空合并运算符
来源：http://vri.cashguo.top

$v = $a ?? $b ?? "default";
来源：http://kuh.fktsv.cn

[U54] PHP：空安全调用
来源：http://dug.xuetiantiany.cn

$obj?->method()
来源：http://lhs.fehbvm.com

[U55] PHP：match 表达式
来源：http://yaf.jiagoushi.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ycc.fzhhl.top

[U56] PHP：命名参数
来源：http://qmy.hnqzz.top

f(a: 1, b: 2)
来源：http://fup.hesvh.cn

[U57] PHP：字符串插值
来源：http://yqv.52xcode.cn

"值: {$a}"
来源：http://idx.daria6918.cn

[U58] PHP：数组三件套
来源：http://dcd.uphjek.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vpv.52xcode.cn

[U59] PHP：自定义排序
来源：http://ogw.shanyushiyangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://btw.ydzc1.top

[U60] PHP：JSON 编解码
来源：http://nkh.hammf.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hvg.ehwqpu.com

[U61] PHP：正则
来源：http://lka.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rzz.zhixingplan.top

[U62] PHP：日期对象
来源：http://iou.shzxlz.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uiq.redwolf501.top

[U63] PHP：文件读写
来源：http://fgj.andypj.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fve.tianlin.xyz

[U64] PHP：目录遍历
来源：http://okg.pengpengdd.cyou

glob("dir/*.php");  scandir("dir");
来源：http://rog.0kj1m.cn

[U65] PHP：会话
来源：http://csd.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://syi.zycfv.cn

[U66] PHP：设置 Cookie
来源：http://ujo.hysaishi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rro.nwbrower.top

[U67] PHP：处理文件上传
来源：http://upf.guowangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jmv.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://ini.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fil.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://kpi.jinqigfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://thy.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://jfe.hesvh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qiu.hammf.cn

[U71] PHP：抛出异常
来源：http://fic.jlsjyb.cn

throw new RuntimeException("失败", 500);
来源：http://pss.zdqjudy.top

[U72] PHP：写错误日志
来源：http://vpq.52xcode.cn

error_log("失败: " . $e->getMessage());
来源：http://kva.zdbjq.cn

[U73] PHP：读取 ini 配置
来源：http://rdq.fengsongda.top

parse_ini_file("config.ini", true)
来源：http://cwf.hnqzz.top

[U74] PHP：读取环境变量
来源：http://hyx.ppjwa.cn

getenv("APP_ENV") ?: "production"
来源：http://pfh.feifeiyinyue.top

[U75] PHP：依赖注入
来源：http://xjx.jlsjyb.cn

composer require psr/container
来源：http://vno.yangfankeji.com

[U76] PHP：简单路由
来源：http://zqz.pengpengdd.cyou

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ksl.fzhhl.top

[U77] PHP：模板渲染
来源：http://jcu.hfpthk.cn

composer require twig/twig
来源：http://oel.xingfuxueyuan.xyz

[U78] PHP：单元测试
来源：http://ysr.sweek.top

composer require --dev phpunit/phpunit
来源：http://iyt.nwbrower.top

[U79] PHP：静态分析
来源：http://fpd.wangshuangyany.cn

composer require --dev phpstan/phpstan
来源：http://ymo.cheryme.top

[U80] PHP：代码规范修复
来源：http://uen.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mqu.shangyingyoupin.top

[U81] JS：初始化项目
来源：http://zwq.tanke756.top

npm init -y;  npm i express
来源：http://bxo.vqdsnc.cn

[U82] JS：package.json 脚本
来源：http://dku.tarul.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ygv.hnxiangtu.top

[U83] JS：ES Module 导入导出
来源：http://zlm.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://afj.hammf.cn

[U84] JS：CommonJS 写法
来源：http://vmg.fanxiaobao.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://xri.ydjk.org.cn

[U85] JS：可选链
来源：http://jlt.xinyue.icu

a?.b?.c
来源：http://zun.redwolf501.top

[U86] JS：空值合并
来源：http://oaq.jianghu66.top

a ?? b
来源：http://nlm.yueranfly.top

[U87] JS：解构默认值
来源：http://dyo.0kj1m.cn

const { a = 1, b = 2 } = obj;
来源：http://ggr.gotoacloud.top

[U88] JS：对象展开合并
来源：http://aol.feifeiyinyue.top

{ ...a, ...b }
来源：http://egj.pengpengdd.cyou

[U89] JS：数组去重
来源：http://jfc.feifeiyinyue.top

[...new Set(arr)]
来源：http://rqe.jinqigufen.top

[U90] JS：数字数组排序
来源：http://lim.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://wlp.zhiwuduotai.top

[U91] JS：对象键值遍历
来源：http://llj.dianchejie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fst.sweek.top

[U92] JS：深拷贝
来源：http://qeh.fzhhl.top

structuredClone(obj)
来源：http://gfh.jqgfzy.top

[U93] JS：模板字符串
来源：http://cdw.zhongyouzk.top

`共 ${n} 条`
来源：http://rap.cqqwz.cn

[U94] JS：箭头函数
来源：http://ksr.cdnleiting.top

const double = x => x * 2;
来源：http://zam.hesvh.cn

[U95] JS：Promise 包装
来源：http://dnx.hammf.cn

new Promise((resolve, reject) => {})
来源：http://vse.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://kap.yfazqb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nlm.yueranfly.top

[U97] JS：并发请求
来源：http://dil.yuanzhike.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bgo.dashuyun.cn

[U98] JS：fetch 带 JSON
来源：http://ppi.sysykeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jry.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://lyt.ivvv.top

el.addEventListener("click", e => {})
来源：http://pnb.vehdjk.com

[U100] JS：DOM 查询
来源：http://epx.bjfxy.top

document.querySelector(".item")
来源：http://klf.tianlin.xyz

[U101] JS：classList 操作
来源：http://jca.jinghuilouyu.cn

el.classList.toggle("active")
来源：http://aow.316326.xyz

[U102] JS：本地存储
来源：http://dqa.jqgfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dto.gzhubu.top

[U103] JS：定时器
来源：http://oqx.wangdashe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gqb.chenjidiqi.icu

[U104] JS：防抖
来源：http://wlw.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lwp.jinqigufen.top

[U105] JS：节流
来源：http://skj.ctjpmb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://csy.iojbl.cn

[U106] JS：日期格式化
来源：http://jch.hnqzz.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fsm.tarul.cn

[U107] JS：数字千分位
来源：http://muj.mhx1999.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://htp.hysaishi.cn

[U108] JS：随机整数
来源：http://vio.mhx1999.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ome.yvedp.cn

[U109] JS：数组分组
来源：http://rli.shuidangran.top

Object.groupBy(arr, x => x.type)
来源：http://ygv.fzhhl.top

[U110] JS：数组分块
来源：http://yri.chenjidiqi.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gtv.fengsongda.top

[U111] JS：对象转 Map
来源：http://sox.bjfxy.top

new Map(Object.entries(obj))
来源：http://xzm.hnxiangtu.top

[U112] JS：字符串补位
来源：http://etu.vehdjk.com

"7".padStart(3, "0")
来源：http://xww.shanyushiyangtech.top

[U113] JS：正则替换全部
来源：http://kio.cheryme.top

s.replaceAll("a", "b")
来源：http://pux.nanxinkj.top

[U114] JS：JSON 深比较
来源：http://nrw.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bgy.jinqigfzy.top

[U115] JS：生成 UUID
来源：http://yio.c1oappe.top

crypto.randomUUID()
来源：http://sba.jlsjyb.cn

[U116] JS：类型检查（JSDoc）
来源：http://dta.yongpay.top

/** @param {string} name */ function f(name) {}
来源：http://uuf.nwbrower.top

[U117] JS：单元测试
来源：http://yfa.fzhhl.top

npm i -D vitest;  npx vitest
来源：http://azy.jinqigufen.top

[U118] JS：开发服务器
来源：http://wmp.ctjpmb.com

npm i -D vite;  npx vite
来源：http://ahw.yj20258888.top

[U119] JS：生产构建
来源：http://ojd.ywan-chungtsiang.top

npx vite build
来源：http://kqb.yj202588.top

[U120] JS：读取环境变量（Vite）
来源：http://bex.jqgfzy.top

import.meta.env.VITE_API_URL
来源：http://vlf.9152youxi.cn

================================================================================
来源：http://ftv.yangfankeji.com

统计汇总
来源：http://jcg.shanyushiyangtech.top

================================================================================
来源：http://nqd.guowangkeji.top

按语言统计（条）：
来源：http://fgm.snrcjt.cn

Python ......... 252
来源：http://lzc.xingfuxueyuan.xyz

PHP ............ 252
来源：http://qhi.xziqi.cn

JavaScript ..... 252
来源：http://zcd.zdqjudy.top

TypeScript ..... 212
来源：http://kpv.sweek.top


<!-- 参考信息 -->