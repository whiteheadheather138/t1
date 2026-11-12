代发 wailian999

[T35] Lua：字典表
来源：http://kxs.ctjpmb.com

local d = { a = 1 };  d.b = 2
来源：http://uro.bbcook.cn

[T36] Lua：函数
来源：http://yno.xziqi.cn

function add(a, b) return a + b end
来源：http://rvf.jlsjyb.cn

[T37] Lua：字符串拼接
来源：http://ymm.ybcxt.top

"a" .. "b"
来源：http://ayc.nwbrower.top

[T38] Lua：条件
来源：http://fjd.jinqigfzy.top

if x > 0 then print("正") end
来源：http://pxx.xuetiantiany.cn

[T39] Lua：模式匹配
来源：http://nzv.sufxvd.cn

string.find(s, "%d+")
来源：http://vjf.yj20258888.top

[T40] Lua：元表
来源：http://sbc.cashguo.top

setmetatable({}, { __index = base })
来源：http://bux.chenzaomai.com

[T41] Perl：Hello World
来源：http://dfg.shanyushiyangkeji.top

print "Hello\n";
来源：http://xeh.yuxming.cn

[T42] Perl：变量类型
来源：http://wap.gzhubu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pzv.cdnleiting.top

[T43] Perl：字符串插值
来源：http://fsw.zycfv.cn

"值: $a"
来源：http://bon.9152youxi.cn

[T44] Perl：条件
来源：http://wbd.jinqigfzy.top

if ($a > 0) { print "正"; }
来源：http://iyu.iojbl.cn

[T45] Perl：数组遍历
来源：http://mnt.0kj1m.cn

for my $x (@arr) { print $x; }
来源：http://nkr.daxiang520.top

[T46] Perl：哈希操作
来源：http://fdu.zhiwuduotai.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ehl.hesvh.cn

[T47] Perl：正则捕获
来源：http://xmc.bjfxy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://axz.kuanghao11.cn

[T48] Perl：正则替换
来源：http://ukt.aizwys.cn

$s =~ s/old/new/g;
来源：http://wrw.birdmap.top

[T49] Perl：函数
来源：http://upx.meibo888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://you.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://dqb.yongpay.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xhy.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://pfx.tarul.cn

[T51] Scala：Hello World
来源：http://xdv.chenlongwang.top

println("Hello")
来源：http://lfl.feifeiyinyue.top

[T52] Scala：变量
来源：http://ktq.hfpthk.cn

val a = 1;  var b = 2
来源：http://cuq.9152youxi.cn

[T53] Scala：字符串插值
来源：http://fts.jinghuilouyu.cn

s"值: $b"
来源：http://jzd.dashuyun.cn

[T54] Scala：集合映射
来源：http://hsf.jlsjyb.cn

List(1, 2, 3).map(_ * 2)
来源：http://mwk.hysaishi.cn

[T55] Scala：集合过滤
来源：http://qmy.sxryk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://asv.aibaodan.cn

[T56] Scala：样例类
来源：http://eoo.ydzc1.top

case class User(name: String, age: Int)
来源：http://gao.tanke756.top

[T57] Scala：模式匹配
来源：http://vlw.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://sml.cucudq.cn

[T58] Scala：函数定义
来源：http://zaz.zhaomingkeji.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://git.hysaishi.cn

[T59] Scala：循环
来源：http://yar.cheryme.top

for (i <- 1 to 10) println(i)
来源：http://pfz.aibaodan.cn

[T60] Scala：折叠
来源：http://hth.shangyingyoupin.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sla.meibo888.top

================================================================================
来源：http://ytf.yuanzhike.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vfv.zhixingplan.top

================================================================================
来源：http://vrh.chenlongwang.top

[U01] Py：创建虚拟环境
来源：http://saq.uphjek.com

python -m venv .venv && source .venv/bin/activate
来源：http://vph.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://jdp.pycfn.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://naa.ydjk.org.cn

[U03] Py：加载 .env 配置
来源：http://nnw.dianchejie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bnd.aibaodan.cn

[U04] Py：变量调试打印
来源：http://bsm.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ewz.zdbjq.cn

[U05] Py：列表去重且保序
来源：http://axn.jianghu66.top

list(dict.fromkeys(arr))
来源：http://ixh.0kj1m.cn

[U06] Py：合并两个字典
来源：http://uhc.xziqi.cn

{**a, **b}
来源：http://acz.zhongyouzk.top

[U07] Py：反转字典键值
来源：http://mui.ivvv.top

{v: k for k, v in d.items()}
来源：http://qtq.52xcode.cn

[U08] Py：展平二维列表
来源：http://tcn.yj20258888.top

[y for x in nested for y in x]
来源：http://cgx.ywan-chungtsiang.top

[U09] Py：字典取最大值的键
来源：http://ejz.dianchejie.cn

max(d, key=d.get)
来源：http://pyp.cashguo.top

[U10] Py：按值排序字典
来源：http://nlf.gogol.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qgd.hesvh.cn

[U11] Py：生成器表达式
来源：http://uzi.shzxlz.cn

(x * 2 for x in arr)
来源：http://klh.snrcjt.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ssi.fzhhl.top

Counter(arr).most_common(3)
来源：http://wsl.sysykeji.top

[U13] Py：固定长度队列
来源：http://mrz.gotoacloud.top

deque(maxlen=10)
来源：http://doe.hnxiangtu.top

[U14] Py：分组收集到列表
来源：http://qge.ppjwa.cn

defaultdict(list)
来源：http://aur.tarul.cn

[U15] Py：高精度计时
来源：http://uql.hesvh.cn

t = time.perf_counter()
来源：http://lbb.jlsjyb.cn

[U16] Py：命令行参数解析
来源：http://ock.epnwcf.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vvn.haohaochexian.top

[U17] Py：初始化日志
来源：http://rhi.bjfxy.top

logging.basicConfig(level=logging.INFO)
来源：http://qwf.yj20258.top

[U18] Py：预编译正则
来源：http://wef.cheryme.top

pat = re.compile(r"\d+")
来源：http://gfg.hywenlv.cn

[U19] Py：正则替换带回调
来源：http://qmq.sweek.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ieg.havefunace.top

[U20] Py：缓存函数结果
来源：http://mkv.c1oappe.top

@functools.lru_cache(maxsize=None)
来源：http://whw.guowangkeji.top

[U21] Py：自定义上下文管理器
来源：http://bed.jinyuanbaomall.cn

@contextlib.contextmanager
来源：http://jyb.havefunace.top

[U22] Py：矩阵转置
来源：http://vnn.zdbjq.cn

list(zip(*m))
来源：http://fxc.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://dit.chenzaomai.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://luh.wangdashe.top

[U24] Py：路径操作
来源：http://mst.yfazqb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dni.nwbrower.top

[U25] Py：CSV 按字典读
来源：http://zhs.mhx1999.top

csv.DictReader(f)
来源：http://bpz.xylfe.cn

[U26] Py：并发下载
来源：http://bqp.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ilk.meibo888.top

[U27] Py：异步 HTTP
来源：http://tmk.smart0.xyz

aiohttp.ClientSession() 配合 async with
来源：http://oyv.zhongyouzk.top

[U28] Py：类型别名
来源：http://qgd.hywenlv.cn

UserId = int
来源：http://gpb.fanxiaobao.xyz

[U29] Py：属性校验
来源：http://owb.meibo888.top

@property 与 @x.setter 配合
来源：http://lsv.quarkkingdee.top

[U30] Py：数据类
来源：http://scn.yangfankeji.com

@dataclass(slots=True)
来源：http://ohm.xuanzx.com

[U31] Py：单测
来源：http://nnz.yuxming.cn

python -m pytest -q
来源：http://lop.vehdjk.com

[U32] Py：代码格式化
来源：http://nxj.meibo888.top

ruff format . && ruff check --fix .
来源：http://for.nwbrower.top

[U33] Py：打包发布
来源：http://qyu.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://nil.hywenlv.cn

[U34] Py：判断编码
来源：http://tuj.c1oappe.top

chardet.detect(raw)
来源：http://esq.zhaomingkeji.xyz

[U35] Py：发送邮件
来源：http://ifd.zhijiandao.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rev.jinyuanbaomall.cn

[U36] Py：定时任务
来源：http://xej.guowangkeji.top

schedule.every(10).minutes.do(job)
来源：http://vyb.meibo888.top

[U37] Py：读写 Excel
来源：http://xst.chenzaomai.com

pandas.read_excel / DataFrame.to_excel
来源：http://cpw.sweek.top

[U38] Py：获取脚本所在目录
来源：http://kgo.wangshuangyany.cn

Path(__file__).resolve().parent
来源：http://jim.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://riv.hongshengwenyu.top

sys.stdout.isatty()
来源：http://jrn.snrcjt.cn

[U40] Py：打印到标准错误
来源：http://nhr.aizwys.cn

print("err", file=sys.stderr)
来源：http://xmv.hcnkem.com

[U41] PHP：初始化 Composer 项目
来源：http://kxn.zhoulong.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://zom.aizwys.cn

[U42] PHP：PSR-4 自动加载
来源：http://qri.xuetiantiany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ulb.meibo888.top

[U43] PHP：声明命名空间
来源：http://aaw.cqqwz.cn

namespace App\Http;
来源：http://paa.vehdjk.com

[U44] PHP：开启严格类型
来源：http://gia.yuanzhike.top

declare(strict_types=1);
来源：http://orq.zdqjudy.top

[U45] PHP：类型声明与返回类型
来源：http://qgi.zhiwuduotai.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://czt.tianlin.xyz

[U46] PHP：可空类型
来源：http://yid.sysykeji.top

?string $name = null
来源：http://epp.yongpay.top

[U47] PHP：联合类型
来源：http://tig.shuidangran.top

int|string $id
来源：http://hff.vqdsnc.cn

[U48] PHP：纯枚举
来源：http://reu.chenlongwang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://psa.zycfv.cn

[U49] PHP：只读属性
来源：http://ztl.sysykeji.top

public readonly string $name
来源：http://iyy.chenjidiqi.icu

[U50] PHP：构造器属性提升
来源：http://bao.yvedp.cn

public function __construct(private int $id) {}
来源：http://jpn.daria6918.cn

[U51] PHP：数组解构
来源：http://ryi.yueranfly.top

[$a, $b] = $arr;
来源：http://lyd.vehdjk.com

[U52] PHP：箭头函数
来源：http://hcx.jinyuanbaomall.cn

$double = fn($x) => $x * 2;
来源：http://pns.cdnleiting.top

[U53] PHP：空合并运算符
来源：http://ish.uphjek.com

$v = $a ?? $b ?? "default";
来源：http://sid.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://erd.yonumen.top

$obj?->method()
来源：http://xgu.dashuyun.cn

[U55] PHP：match 表达式
来源：http://ljn.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zxu.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://mcu.feifeiyinyue.top

f(a: 1, b: 2)
来源：http://kzz.hnqzz.top

[U57] PHP：字符串插值
来源：http://gog.zhiwuduotai.top

"值: {$a}"
来源：http://ssv.c1oappe.top

[U58] PHP：数组三件套
来源：http://wja.yueranfly.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lxa.nanxuanxn.top

[U59] PHP：自定义排序
来源：http://ahz.yongpay.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gkr.zhixingplan.top

[U60] PHP：JSON 编解码
来源：http://lip.pengpengdd.cyou

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://shu.fktsv.cn

[U61] PHP：正则
来源：http://vda.xziqi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kqb.jianghu66.top

[U62] PHP：日期对象
来源：http://inn.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fsa.zhaomingkeji.xyz

[U63] PHP：文件读写
来源：http://gwg.sufxvd.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gsd.gaohongyu789.top

[U64] PHP：目录遍历
来源：http://esx.gaohongyu789.top

glob("dir/*.php");  scandir("dir");
来源：http://zfp.jiagoushi.top

[U65] PHP：会话
来源：http://zah.yj202588.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yis.jyoumei.cn

[U66] PHP：设置 Cookie
来源：http://aev.jianghu66.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://evx.mhx1999.top

[U67] PHP：处理文件上传
来源：http://wim.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jzn.yj20258888.top

[U68] PHP：PDO 连接
来源：http://woy.andypj.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://owy.ybcxt.top

[U69] PHP：PDO 预处理
来源：http://fwd.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ebj.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://pmw.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bew.daria6918.cn

[U71] PHP：抛出异常
来源：http://qyt.yongpay.top

throw new RuntimeException("失败", 500);
来源：http://pkj.yonumen.top

[U72] PHP：写错误日志
来源：http://ydg.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://lae.dashuyun.cn

[U73] PHP：读取 ini 配置
来源：http://anz.xuetiantiany.cn

parse_ini_file("config.ini", true)
来源：http://crh.feifeiyinyue.top

[U74] PHP：读取环境变量
来源：http://heo.hywenlv.cn

getenv("APP_ENV") ?: "production"
来源：http://gxx.hongshengwenyu.top

[U75] PHP：依赖注入
来源：http://wyw.yongpay.top

composer require psr/container
来源：http://bti.hywenlv.cn

[U76] PHP：简单路由
来源：http://bsx.chenjidiqi.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yrd.hfpthk.cn

[U77] PHP：模板渲染
来源：http://qsm.cheryme.top

composer require twig/twig
来源：http://nzm.zhijiandao.cn

[U78] PHP：单元测试
来源：http://wpa.fengsongda.top

composer require --dev phpunit/phpunit
来源：http://bhb.epnwcf.com

[U79] PHP：静态分析
来源：http://fkr.cashguo.top

composer require --dev phpstan/phpstan
来源：http://goc.bbcook.cn

[U80] PHP：代码规范修复
来源：http://qjq.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xho.chenjidiqi.icu

[U81] JS：初始化项目
来源：http://wnc.tanke756.top

npm init -y;  npm i express
来源：http://cdd.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://czb.hnqzz.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sxp.chenjidiqi.icu

[U83] JS：ES Module 导入导出
来源：http://tof.yanxiufei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://okn.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://prz.jinyuanbaomall.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ufj.jlsjyb.cn

[U85] JS：可选链
来源：http://mui.c1oappe.top

a?.b?.c
来源：http://nvc.52xcode.cn

[U86] JS：空值合并
来源：http://stg.ydjk.org.cn

a ?? b
来源：http://zob.c1oappe.top

[U87] JS：解构默认值
来源：http://zgr.zdqjudy.top

const { a = 1, b = 2 } = obj;
来源：http://lgl.jyoumei.cn

[U88] JS：对象展开合并
来源：http://xag.redwolf501.top

{ ...a, ...b }
来源：http://all.jinqigufen.top

[U89] JS：数组去重
来源：http://jxo.gogol.net.cn

[...new Set(arr)]
来源：http://ztf.ywan-chungtsiang.top

[U90] JS：数字数组排序
来源：http://bje.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://gcv.tianlin.xyz

[U91] JS：对象键值遍历
来源：http://nkb.pycfn.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cpx.zhaomingkeji.xyz

[U92] JS：深拷贝
来源：http://yns.xylfe.cn

structuredClone(obj)
来源：http://fba.jinqigufen.top

[U93] JS：模板字符串
来源：http://viz.xuetiantiany.cn

`共 ${n} 条`
来源：http://tgf.yfazqb.com

[U94] JS：箭头函数
来源：http://bhq.yuanzhike.top

const double = x => x * 2;
来源：http://gxp.svipenyu.cn

[U95] JS：Promise 包装
来源：http://ths.jinqigfzy.top

new Promise((resolve, reject) => {})
来源：http://ujk.cqqwz.cn

[U96] JS：async/await 与异常
来源：http://dwz.jinghuilouyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qkr.shzxlz.cn

[U97] JS：并发请求
来源：http://imj.snrcjt.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vys.jinyuanbaomall.cn

[U98] JS：fetch 带 JSON
来源：http://xfy.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://opl.sweek.top

[U99] JS：事件监听
来源：http://hob.jlsjyb.cn

el.addEventListener("click", e => {})
来源：http://sgj.cdnleiting.top

[U100] JS：DOM 查询
来源：http://wgc.fktsv.cn

document.querySelector(".item")
来源：http://wip.bjfxy.top

[U101] JS：classList 操作
来源：http://wyq.sjlbkw.cn

el.classList.toggle("active")
来源：http://rbr.epnwcf.com

[U102] JS：本地存储
来源：http://hri.gaohongyu789.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kjk.0kj1m.cn

[U103] JS：定时器
来源：http://uek.tianlin.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wjj.zdbjq.cn

[U104] JS：防抖
来源：http://cjw.meibo888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oop.wangdashe.top

[U105] JS：节流
来源：http://uih.hcnkem.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qbw.hnxiangtu.top

[U106] JS：日期格式化
来源：http://kpq.hnxiangtu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tpo.jqgufenzy.top

[U107] JS：数字千分位
来源：http://slo.zhoulong.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qpd.yangfankeji.com

[U108] JS：随机整数
来源：http://trl.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gon.dashuyun.cn

[U109] JS：数组分组
来源：http://iog.yuanzhike.top

Object.groupBy(arr, x => x.type)
来源：http://qnz.wangdashe.top

[U110] JS：数组分块
来源：http://zjv.xylfe.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ckg.mhx1999.top

[U111] JS：对象转 Map
来源：http://kxf.haohaochexian.top

new Map(Object.entries(obj))
来源：http://egi.zdbjq.cn

[U112] JS：字符串补位
来源：http://nuh.jqgfzy.top

"7".padStart(3, "0")
来源：http://qcu.zhengqikj.top

[U113] JS：正则替换全部
来源：http://zrp.zhongyouzk.top

s.replaceAll("a", "b")
来源：http://nec.meibo888.top

[U114] JS：JSON 深比较
来源：http://ndi.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ify.yuxming.cn

[U115] JS：生成 UUID
来源：http://pdh.sysykeji.top

crypto.randomUUID()
来源：http://jig.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://atf.316326.xyz

/** @param {string} name */ function f(name) {}
来源：http://ftp.ivvv.top

[U117] JS：单元测试
来源：http://oxj.gotoacloud.top

npm i -D vitest;  npx vitest
来源：http://pnn.yfazqb.com

[U118] JS：开发服务器
来源：http://wds.0kj1m.cn

npm i -D vite;  npx vite
来源：http://vou.jyoumei.cn

[U119] JS：生产构建
来源：http://sya.jinyuanbaomall.cn

npx vite build
来源：http://jrz.jiagoushi.top

[U120] JS：读取环境变量（Vite）
来源：http://bsk.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://bsk.c1oappe.top

================================================================================
来源：http://tru.0kj1m.cn

统计汇总
来源：http://lmz.xuetiantiany.cn

================================================================================
来源：http://wad.ywan-chungtsiang.top

按语言统计（条）：
来源：http://aif.shzxlz.cn


<!-- 参考信息 -->