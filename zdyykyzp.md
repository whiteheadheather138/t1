代发 wailian999

[T37] Lua：字符串拼接
来源：http://yok.ywan-chungtsiang.top

"a" .. "b"
来源：http://jgf.epnwcf.com

[T38] Lua：条件
来源：http://lwc.mhx1999.top

if x > 0 then print("正") end
来源：http://cbq.cqqwz.cn

[T39] Lua：模式匹配
来源：http://hkp.shuidangran.top

string.find(s, "%d+")
来源：http://jol.jinghuilouyu.cn

[T40] Lua：元表
来源：http://isz.svipenyu.cn

setmetatable({}, { __index = base })
来源：http://glt.zhoulong.xyz

[T41] Perl：Hello World
来源：http://mao.xziqi.cn

print "Hello\n";
来源：http://xhd.yj20258888.top

[T42] Perl：变量类型
来源：http://yls.52xcode.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sef.shuidangran.top

[T43] Perl：字符串插值
来源：http://fxn.zhongyouzk.top

"值: $a"
来源：http://xtk.shangyingyoupin.top

[T44] Perl：条件
来源：http://hit.redwolf501.top

if ($a > 0) { print "正"; }
来源：http://zpn.haohaochexian.top

[T45] Perl：数组遍历
来源：http://doy.cheryme.top

for my $x (@arr) { print $x; }
来源：http://beg.hcnkem.com

[T46] Perl：哈希操作
来源：http://flh.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mmd.nwbrower.top

[T47] Perl：正则捕获
来源：http://vxo.haohaochexian.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yca.cheryme.top

[T48] Perl：正则替换
来源：http://ihe.ivvv.top

$s =~ s/old/new/g;
来源：http://dqy.chenzaomai.com

[T49] Perl：函数
来源：http://yvr.yj20258.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sto.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://jsy.birdmap.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tqi.tian-w.cn

while (my $line = <$fh>) { print $line; }
来源：http://gka.cqqwz.cn

[T51] Scala：Hello World
来源：http://qdq.sxryk.cn

println("Hello")
来源：http://mny.hysaishi.cn

[T52] Scala：变量
来源：http://oan.iojbl.cn

val a = 1;  var b = 2
来源：http://iov.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://asx.feifeiyinyue.top

s"值: $b"
来源：http://zqi.quarkkingdee.top

[T54] Scala：集合映射
来源：http://tnx.316326.xyz

List(1, 2, 3).map(_ * 2)
来源：http://azz.cqqwz.cn

[T55] Scala：集合过滤
来源：http://omo.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://rci.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://tia.mhx1999.top

case class User(name: String, age: Int)
来源：http://grl.haohaochexian.top

[T57] Scala：模式匹配
来源：http://elc.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yak.yongpay.top

[T58] Scala：函数定义
来源：http://ugp.jinyuanbaomall.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gvb.snrcjt.cn

[T59] Scala：循环
来源：http://jno.zycfv.cn

for (i <- 1 to 10) println(i)
来源：http://jra.fktsv.cn

[T60] Scala：折叠
来源：http://xio.chenlongwang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ulo.iojbl.cn

================================================================================
来源：http://qpk.ctjpmb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wvd.jyoumei.cn

================================================================================
来源：http://wir.zhijiandao.cn

[U01] Py：创建虚拟环境
来源：http://fde.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ojr.ivvv.top

[U02] Py：导出 / 安装依赖
来源：http://utm.gaohongyu789.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iyc.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://hdx.pengpengdd.cyou

from dotenv import load_dotenv; load_dotenv()
来源：http://yll.yj20258.top

[U04] Py：变量调试打印
来源：http://fob.tanke756.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://olm.ctjpmb.com

[U05] Py：列表去重且保序
来源：http://jir.havefunace.top

list(dict.fromkeys(arr))
来源：http://rsr.hammf.cn

[U06] Py：合并两个字典
来源：http://ton.aibaodan.cn

{**a, **b}
来源：http://tsm.pycfn.com

[U07] Py：反转字典键值
来源：http://vlf.zycfv.cn

{v: k for k, v in d.items()}
来源：http://yns.yj20258.top

[U08] Py：展平二维列表
来源：http://wfj.redwolf501.top

[y for x in nested for y in x]
来源：http://ccl.cqqwz.cn

[U09] Py：字典取最大值的键
来源：http://mvb.zdbjq.cn

max(d, key=d.get)
来源：http://qzm.dashuyun.cn

[U10] Py：按值排序字典
来源：http://hlc.xuanzx.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ocj.ctjpmb.com

[U11] Py：生成器表达式
来源：http://nzl.gotoacloud.top

(x * 2 for x in arr)
来源：http://cci.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nps.316326.xyz

Counter(arr).most_common(3)
来源：http://osg.iojbl.cn

[U13] Py：固定长度队列
来源：http://wdg.yuanzhike.top

deque(maxlen=10)
来源：http://rgj.ydzc1.top

[U14] Py：分组收集到列表
来源：http://flz.meibo888.top

defaultdict(list)
来源：http://oll.yfazqb.com

[U15] Py：高精度计时
来源：http://hre.cucudq.cn

t = time.perf_counter()
来源：http://eca.ivvv.top

[U16] Py：命令行参数解析
来源：http://dfi.hongshengwenyu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rbk.hywenlv.cn

[U17] Py：初始化日志
来源：http://fbp.fengsongda.top

logging.basicConfig(level=logging.INFO)
来源：http://jvp.yongpay.top

[U18] Py：预编译正则
来源：http://iyf.hcnkem.com

pat = re.compile(r"\d+")
来源：http://esi.yj20258.top

[U19] Py：正则替换带回调
来源：http://qgq.hesvh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lha.jqgufenzy.top

[U20] Py：缓存函数结果
来源：http://ayb.zhongyouzk.top

@functools.lru_cache(maxsize=None)
来源：http://wty.iojbl.cn

[U21] Py：自定义上下文管理器
来源：http://fra.redwolf501.top

@contextlib.contextmanager
来源：http://bvf.hesvh.cn

[U22] Py：矩阵转置
来源：http://hbq.epnwcf.com

list(zip(*m))
来源：http://rvf.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://yxf.sweek.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zzk.sxryk.cn

[U24] Py：路径操作
来源：http://wjg.zhijiandao.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://upn.0kj1m.cn

[U25] Py：CSV 按字典读
来源：http://mgr.xziqi.cn

csv.DictReader(f)
来源：http://fkn.zdbjq.cn

[U26] Py：并发下载
来源：http://oun.yuanzhike.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qkq.tian-w.cn

[U27] Py：异步 HTTP
来源：http://tkq.fzhhl.top

aiohttp.ClientSession() 配合 async with
来源：http://emu.smart0.xyz

[U28] Py：类型别名
来源：http://tpd.pengpengdd.cyou

UserId = int
来源：http://zki.gotoacloud.top

[U29] Py：属性校验
来源：http://hwe.jianghu66.top

@property 与 @x.setter 配合
来源：http://hiu.shanyushiyangtech.top

[U30] Py：数据类
来源：http://rzr.quarkkingdee.top

@dataclass(slots=True)
来源：http://grh.316326.xyz

[U31] Py：单测
来源：http://wao.yfazqb.com

python -m pytest -q
来源：http://xzb.hesvh.cn

[U32] Py：代码格式化
来源：http://etz.nanxuanxn.top

ruff format . && ruff check --fix .
来源：http://dsq.9152youxi.cn

[U33] Py：打包发布
来源：http://prw.xingfuxueyuan.xyz

python -m build  （依赖 pyproject.toml）
来源：http://vds.xylfe.cn

[U34] Py：判断编码
来源：http://gru.zhengqikj.top

chardet.detect(raw)
来源：http://fyu.xylfe.cn

[U35] Py：发送邮件
来源：http://xjt.fzhhl.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xmy.daria6918.cn

[U36] Py：定时任务
来源：http://jja.sjlbkw.cn

schedule.every(10).minutes.do(job)
来源：http://nnb.xziqi.cn

[U37] Py：读写 Excel
来源：http://tso.shangyingyoupin.top

pandas.read_excel / DataFrame.to_excel
来源：http://nqb.meibo888.top

[U38] Py：获取脚本所在目录
来源：http://dhi.uphjek.com

Path(__file__).resolve().parent
来源：http://cmf.kuanghao11.cn

[U39] Py：判断是否在交互环境
来源：http://fkc.xuanzx.com

sys.stdout.isatty()
来源：http://gzc.hfpthk.cn

[U40] Py：打印到标准错误
来源：http://kka.gzhubu.top

print("err", file=sys.stderr)
来源：http://ufg.ydjk.org.cn

[U41] PHP：初始化 Composer 项目
来源：http://xqn.bjfxy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://exz.aizwys.cn

[U42] PHP：PSR-4 自动加载
来源：http://ykb.tian-w.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rob.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://cok.gaohongyu789.top

namespace App\Http;
来源：http://lkj.aizwys.cn

[U44] PHP：开启严格类型
来源：http://hqa.gzhubu.top

declare(strict_types=1);
来源：http://lqk.zycfv.cn

[U45] PHP：类型声明与返回类型
来源：http://jco.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ous.bjfxy.top

[U46] PHP：可空类型
来源：http://tyq.zhongyouzk.top

?string $name = null
来源：http://aqo.hnxiangtu.top

[U47] PHP：联合类型
来源：http://xcb.quarkkingdee.top

int|string $id
来源：http://wil.hysaishi.cn

[U48] PHP：纯枚举
来源：http://lsf.hnxiangtu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qom.tarul.cn

[U49] PHP：只读属性
来源：http://nwi.zdqjudy.top

public readonly string $name
来源：http://yee.pengpengdd.cyou

[U50] PHP：构造器属性提升
来源：http://mwv.ywan-chungtsiang.top

public function __construct(private int $id) {}
来源：http://ahr.dianchejie.cn

[U51] PHP：数组解构
来源：http://akf.aizwys.cn

[$a, $b] = $arr;
来源：http://lov.zhaomingkeji.xyz

[U52] PHP：箭头函数
来源：http://rja.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://vhu.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://hxv.52xcode.cn

$v = $a ?? $b ?? "default";
来源：http://hoe.uphjek.com

[U54] PHP：空安全调用
来源：http://hsz.sufxvd.cn

$obj?->method()
来源：http://zbl.zhiwuduotai.top

[U55] PHP：match 表达式
来源：http://boi.fengsongda.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ywr.xuanzx.com

[U56] PHP：命名参数
来源：http://hpn.iojbl.cn

f(a: 1, b: 2)
来源：http://rjz.nwbrower.top

[U57] PHP：字符串插值
来源：http://lmp.shuidangran.top

"值: {$a}"
来源：http://lpp.birdmap.top

[U58] PHP：数组三件套
来源：http://owf.cheryme.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nck.jinghuilouyu.cn

[U59] PHP：自定义排序
来源：http://jjf.ydzc1.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rgv.guowangkeji.top

[U60] PHP：JSON 编解码
来源：http://xgw.gogol.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qax.jiagoushi.top

[U61] PHP：正则
来源：http://fso.cqqwz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dej.yj20258.top

[U62] PHP：日期对象
来源：http://buy.mhx1999.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wqn.zdbjq.cn

[U63] PHP：文件读写
来源：http://koi.svipenyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://peo.redwolf501.top

[U64] PHP：目录遍历
来源：http://kyj.fehbvm.com

glob("dir/*.php");  scandir("dir");
来源：http://daf.hnqzz.top

[U65] PHP：会话
来源：http://irp.ywan-chungtsiang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mnt.redwolf501.top

[U66] PHP：设置 Cookie
来源：http://cft.smart0.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://unj.jinqigfzy.top

[U67] PHP：处理文件上传
来源：http://fno.xingfuxueyuan.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ejr.kuanghao11.cn

[U68] PHP：PDO 连接
来源：http://uew.zhijiandao.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jyh.ivvv.top

[U69] PHP：PDO 预处理
来源：http://ekx.hongshengwenyu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://for.yvedp.cn

[U70] PHP：PDO 事务
来源：http://duv.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ydw.ivvv.top

[U71] PHP：抛出异常
来源：http://mlr.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://jub.iojbl.cn

[U72] PHP：写错误日志
来源：http://lbc.pengpengdd.cyou

error_log("失败: " . $e->getMessage());
来源：http://lmp.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://yul.yangfankeji.com

parse_ini_file("config.ini", true)
来源：http://xea.zhijiandao.cn

[U74] PHP：读取环境变量
来源：http://zwy.gaohongyu789.top

getenv("APP_ENV") ?: "production"
来源：http://rpr.0kj1m.cn

[U75] PHP：依赖注入
来源：http://zqq.hcnkem.com

composer require psr/container
来源：http://dpa.jlsjyb.cn

[U76] PHP：简单路由
来源：http://oqv.tian-w.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fod.cqqwz.cn

[U77] PHP：模板渲染
来源：http://pcu.xylfe.cn

composer require twig/twig
来源：http://twv.zhixingplan.top

[U78] PHP：单元测试
来源：http://aaf.yanxiufei.cn

composer require --dev phpunit/phpunit
来源：http://ijy.fzhhl.top

[U79] PHP：静态分析
来源：http://gkg.uphjek.com

composer require --dev phpstan/phpstan
来源：http://ads.fktsv.cn

[U80] PHP：代码规范修复
来源：http://uzb.vehdjk.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://scn.pengpengdd.cyou

[U81] JS：初始化项目
来源：http://htf.gotoacloud.top

npm init -y;  npm i express
来源：http://cxi.fehbvm.com

[U82] JS：package.json 脚本
来源：http://ywb.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nvl.ehwqpu.com

[U83] JS：ES Module 导入导出
来源：http://ezr.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://rfj.shuidangran.top

[U84] JS：CommonJS 写法
来源：http://gzq.zhengqikj.top

module.exports = { a };  const { a } = require("./m");
来源：http://uju.cheryme.top

[U85] JS：可选链
来源：http://gbz.feifeiyinyue.top

a?.b?.c
来源：http://yia.jqgfzy.top

[U86] JS：空值合并
来源：http://orp.gaohongyu789.top

a ?? b
来源：http://diy.yj202588.top

[U87] JS：解构默认值
来源：http://uay.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://lwx.yuxming.cn

[U88] JS：对象展开合并
来源：http://yox.yfazqb.com

{ ...a, ...b }
来源：http://pip.xinyue.icu

[U89] JS：数组去重
来源：http://xby.yongpay.top

[...new Set(arr)]
来源：http://bfa.redwolf501.top

[U90] JS：数字数组排序
来源：http://akz.yvedp.cn

[...arr].sort((a, b) => a - b)
来源：http://fai.pycfn.com

[U91] JS：对象键值遍历
来源：http://phq.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uog.jiagoushi.top

[U92] JS：深拷贝
来源：http://dkq.hcnkem.com

structuredClone(obj)
来源：http://vim.redwolf501.top

[U93] JS：模板字符串
来源：http://wlc.wangshuangyany.cn

`共 ${n} 条`
来源：http://gkm.c1oappe.top

[U94] JS：箭头函数
来源：http://fwd.ppjwa.cn

const double = x => x * 2;
来源：http://xrm.jiagoushi.top

[U95] JS：Promise 包装
来源：http://mgh.tarul.cn

new Promise((resolve, reject) => {})
来源：http://xfa.gogol.net.cn

[U96] JS：async/await 与异常
来源：http://hdv.zhijiandao.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xus.guannengcc.top

[U97] JS：并发请求
来源：http://lbc.zycfv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://djs.sjlbkw.cn

[U98] JS：fetch 带 JSON
来源：http://ljx.yj20258888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gfa.gzhubu.top

[U99] JS：事件监听
来源：http://gks.jinqigufen.top

el.addEventListener("click", e => {})
来源：http://jja.meibo888.top

[U100] JS：DOM 查询
来源：http://uyw.hfpthk.cn

document.querySelector(".item")
来源：http://whp.tianlin.xyz

[U101] JS：classList 操作
来源：http://cox.gotoacloud.top

el.classList.toggle("active")
来源：http://rcl.ydjk.org.cn

[U102] JS：本地存储
来源：http://neb.zhongyouzk.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tex.yuanzhike.top

[U103] JS：定时器
来源：http://tip.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://chi.jiagoushi.top

[U104] JS：防抖
来源：http://eha.yfazqb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qte.jqgfzy.top

[U105] JS：节流
来源：http://mwp.yj202588.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xzp.chenzaomai.com

[U106] JS：日期格式化
来源：http://qbk.jqgfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iue.xuetiantiany.cn

[U107] JS：数字千分位
来源：http://reh.316326.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oaf.sweek.top

[U108] JS：随机整数
来源：http://xjh.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oaa.daxiang520.top

[U109] JS：数组分组
来源：http://vbd.ehwqpu.com

Object.groupBy(arr, x => x.type)
来源：http://bsi.pycfn.com

[U110] JS：数组分块
来源：http://kfx.dashuyun.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fzf.birdmap.top

[U111] JS：对象转 Map
来源：http://bpb.yonumen.top

new Map(Object.entries(obj))
来源：http://mxi.yongpay.top

[U112] JS：字符串补位
来源：http://yhs.tanke756.top

"7".padStart(3, "0")
来源：http://vsr.xingfuxueyuan.xyz

[U113] JS：正则替换全部
来源：http://qnf.xylfe.cn

s.replaceAll("a", "b")
来源：http://xaw.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://szy.zhixingplan.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jac.zhiwuduotai.top

[U115] JS：生成 UUID
来源：http://czy.tanke756.top

crypto.randomUUID()
来源：http://ztj.cheryme.top

[U116] JS：类型检查（JSDoc）
来源：http://kpm.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://wef.hnqzz.top

[U117] JS：单元测试
来源：http://qfl.shuidangran.top

npm i -D vitest;  npx vitest
来源：http://tnq.yanxiufei.cn

[U118] JS：开发服务器
来源：http://gtm.tianlin.xyz

npm i -D vite;  npx vite
来源：http://pae.snrcjt.cn

[U119] JS：生产构建
来源：http://ekw.jinqigufen.top

npx vite build
来源：http://ghx.haohaochexian.top

[U120] JS：读取环境变量（Vite）
来源：http://jye.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://reh.chenjidiqi.icu

================================================================================
来源：http://hzq.jinqigfzy.top

统计汇总
来源：http://xgg.pengpengdd.cyou

================================================================================
来源：http://gfl.jlsjyb.cn

按语言统计（条）：
来源：http://mjy.zhengqikj.top

Python ......... 252
来源：http://zzp.zhijiandao.cn

PHP ............ 252
来源：http://abz.bjfxy.top

JavaScript ..... 252
来源：http://qbg.fktsv.cn

TypeScript ..... 212
来源：http://dtf.aizwys.cn


<!-- 参考信息 -->