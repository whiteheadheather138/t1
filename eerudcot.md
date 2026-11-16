代发 wailian999

[T29] Swift：guard 提前返回
来源：http://xri.hfpthk.cn

guard let x = opt else { return }
来源：http://upn.yfazqb.com

[T30] Swift：协议
来源：http://pcp.sjlbkw.cn

protocol Shape { func area() -> Double }
来源：http://tby.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://dhe.gogol.net.cn

print("Hello")
来源：http://mzd.hammf.cn

[T32] Lua：局部变量
来源：http://jpe.shzxlz.cn

local a = 1
来源：http://hwg.jyoumei.cn

[T33] Lua：表（数组）
来源：http://ljz.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://heh.aizwys.cn

[T34] Lua：遍历表
来源：http://glo.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://qtu.ppjwa.cn

[T35] Lua：字典表
来源：http://vvg.guannengcc.top

local d = { a = 1 };  d.b = 2
来源：http://ycn.hysaishi.cn

[T36] Lua：函数
来源：http://lyt.xinyue.icu

function add(a, b) return a + b end
来源：http://umn.bjfxy.top

[T37] Lua：字符串拼接
来源：http://oqn.bjfxy.top

"a" .. "b"
来源：http://azb.guannengcc.top

[T38] Lua：条件
来源：http://kjf.xuanzx.com

if x > 0 then print("正") end
来源：http://duq.epnwcf.com

[T39] Lua：模式匹配
来源：http://ejx.jiagoushi.top

string.find(s, "%d+")
来源：http://url.hfpthk.cn

[T40] Lua：元表
来源：http://yur.zdbjq.cn

setmetatable({}, { __index = base })
来源：http://wqt.sufxvd.cn

[T41] Perl：Hello World
来源：http://gzz.zdqjudy.top

print "Hello\n";
来源：http://ppv.zycfv.cn

[T42] Perl：变量类型
来源：http://ghy.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pbf.andypj.xyz

[T43] Perl：字符串插值
来源：http://zin.chenzaomai.com

"值: $a"
来源：http://hba.andypj.xyz

[T44] Perl：条件
来源：http://plr.tanke756.top

if ($a > 0) { print "正"; }
来源：http://who.birdmap.top

[T45] Perl：数组遍历
来源：http://mdm.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://dst.fzhhl.top

[T46] Perl：哈希操作
来源：http://jxd.sjlbkw.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ajb.yvedp.cn

[T47] Perl：正则捕获
来源：http://slb.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://zte.316326.xyz

[T48] Perl：正则替换
来源：http://nhp.havefunace.top

$s =~ s/old/new/g;
来源：http://zji.fanxiaobao.xyz

[T49] Perl：函数
来源：http://syv.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qts.gogol.net.cn

[T50] Perl：逐行读文件
来源：http://pno.shanyushiyangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://afm.dianchejie.cn

while (my $line = <$fh>) { print $line; }
来源：http://qmi.cqqwz.cn

[T51] Scala：Hello World
来源：http://orc.jqgfzy.top

println("Hello")
来源：http://bef.tianlin.xyz

[T52] Scala：变量
来源：http://ebo.jinghuilouyu.cn

val a = 1;  var b = 2
来源：http://hlc.ydzc1.top

[T53] Scala：字符串插值
来源：http://qba.yangfankeji.com

s"值: $b"
来源：http://nez.zhiwuduotai.top

[T54] Scala：集合映射
来源：http://hhr.haohaochexian.top

List(1, 2, 3).map(_ * 2)
来源：http://xtg.daria6918.cn

[T55] Scala：集合过滤
来源：http://rci.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qpc.zhijiandao.cn

[T56] Scala：样例类
来源：http://gdf.sweek.top

case class User(name: String, age: Int)
来源：http://leh.bjfxy.top

[T57] Scala：模式匹配
来源：http://gsp.birdmap.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ngk.tanke756.top

[T58] Scala：函数定义
来源：http://nvk.iojbl.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pes.yj20258888.top

[T59] Scala：循环
来源：http://uyb.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://xep.epnwcf.com

[T60] Scala：折叠
来源：http://ykd.shangyingyoupin.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iwu.shanyushiyangtech.top

================================================================================
来源：http://igg.sysykeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://heu.chenzaomai.com

================================================================================
来源：http://yfo.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://lrx.havefunace.top

python -m venv .venv && source .venv/bin/activate
来源：http://ygo.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://onk.ybcxt.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://akf.zhijiandao.cn

[U03] Py：加载 .env 配置
来源：http://fiw.yj20258888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://spm.zhijiandao.cn

[U04] Py：变量调试打印
来源：http://rkg.birdmap.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ifr.sweek.top

[U05] Py：列表去重且保序
来源：http://qit.hammf.cn

list(dict.fromkeys(arr))
来源：http://zke.daria6918.cn

[U06] Py：合并两个字典
来源：http://kqo.jqgfzy.top

{**a, **b}
来源：http://pvq.0kj1m.cn

[U07] Py：反转字典键值
来源：http://rlt.jinqigfzy.top

{v: k for k, v in d.items()}
来源：http://syx.zdqjudy.top

[U08] Py：展平二维列表
来源：http://liz.sjlbkw.cn

[y for x in nested for y in x]
来源：http://rdo.yfazqb.com

[U09] Py：字典取最大值的键
来源：http://elb.hesvh.cn

max(d, key=d.get)
来源：http://xwd.hfpthk.cn

[U10] Py：按值排序字典
来源：http://bxc.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kim.guowangkeji.top

[U11] Py：生成器表达式
来源：http://loc.tian-w.cn

(x * 2 for x in arr)
来源：http://xkz.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zpq.ybcxt.top

Counter(arr).most_common(3)
来源：http://fuh.hnxiangtu.top

[U13] Py：固定长度队列
来源：http://omk.chenlongwang.top

deque(maxlen=10)
来源：http://hgg.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://bdl.yanxiufei.cn

defaultdict(list)
来源：http://src.vqdsnc.cn

[U15] Py：高精度计时
来源：http://iyf.shanyushiyangtech.top

t = time.perf_counter()
来源：http://nix.yangfankeji.com

[U16] Py：命令行参数解析
来源：http://zyy.zhoulong.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dfw.jinqigfzy.top

[U17] Py：初始化日志
来源：http://tdt.sweek.top

logging.basicConfig(level=logging.INFO)
来源：http://mge.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://jpd.yangfankeji.com

pat = re.compile(r"\d+")
来源：http://luq.hnxiangtu.top

[U19] Py：正则替换带回调
来源：http://pgl.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lnz.zhongyouzk.top

[U20] Py：缓存函数结果
来源：http://uhl.jinqigufen.top

@functools.lru_cache(maxsize=None)
来源：http://awk.fehbvm.com

[U21] Py：自定义上下文管理器
来源：http://ihj.sufxvd.cn

@contextlib.contextmanager
来源：http://ows.9152youxi.cn

[U22] Py：矩阵转置
来源：http://wvc.guannengcc.top

list(zip(*m))
来源：http://vop.yvedp.cn

[U23] Py：分块读取大文件
来源：http://gxg.yfazqb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://irk.ybcxt.top

[U24] Py：路径操作
来源：http://gbd.cqqwz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lqg.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://okw.iojbl.cn

csv.DictReader(f)
来源：http://tzg.ppjwa.cn

[U26] Py：并发下载
来源：http://zmg.smart0.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xie.nanxinkj.top

[U27] Py：异步 HTTP
来源：http://cft.yfazqb.com

aiohttp.ClientSession() 配合 async with
来源：http://niz.nanxuanxn.top

[U28] Py：类型别名
来源：http://sda.hcnkem.com

UserId = int
来源：http://onr.hammf.cn

[U29] Py：属性校验
来源：http://gsk.yj20258.top

@property 与 @x.setter 配合
来源：http://lru.yfazqb.com

[U30] Py：数据类
来源：http://xnq.tarul.cn

@dataclass(slots=True)
来源：http://zuh.epnwcf.com

[U31] Py：单测
来源：http://qpj.chenlongwang.top

python -m pytest -q
来源：http://hfq.yvedp.cn

[U32] Py：代码格式化
来源：http://nrd.yj20258.top

ruff format . && ruff check --fix .
来源：http://vru.wangdashe.top

[U33] Py：打包发布
来源：http://wej.cqqwz.cn

python -m build  （依赖 pyproject.toml）
来源：http://pfb.yuxming.cn

[U34] Py：判断编码
来源：http://rpn.jlsjyb.cn

chardet.detect(raw)
来源：http://egd.dianchejie.cn

[U35] Py：发送邮件
来源：http://tmy.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hmj.shangyingyoupin.top

[U36] Py：定时任务
来源：http://tie.jinyuanbaomall.cn

schedule.every(10).minutes.do(job)
来源：http://tpm.shanyushiyangtech.top

[U37] Py：读写 Excel
来源：http://pcp.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://dpn.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://not.cheryme.top

Path(__file__).resolve().parent
来源：http://xqi.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://pkj.xinyue.icu

sys.stdout.isatty()
来源：http://bvv.kuanghao11.cn

[U40] Py：打印到标准错误
来源：http://rsv.zhijiandao.cn

print("err", file=sys.stderr)
来源：http://alv.zhengqikj.top

[U41] PHP：初始化 Composer 项目
来源：http://bvt.fzhhl.top

composer init;  composer require guzzlehttp/guzzle
来源：http://toa.xuetiantiany.cn

[U42] PHP：PSR-4 自动加载
来源：http://nwb.yueranfly.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xav.jinyuanbaomall.cn

[U43] PHP：声明命名空间
来源：http://xwp.shanyushiyangtech.top

namespace App\Http;
来源：http://vsd.shanyushiyangkeji.top

[U44] PHP：开启严格类型
来源：http://oxh.ppjwa.cn

declare(strict_types=1);
来源：http://pfm.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://xya.yfazqb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://hyu.wangdashe.top

[U46] PHP：可空类型
来源：http://ejt.haohaochexian.top

?string $name = null
来源：http://rgb.tian-w.cn

[U47] PHP：联合类型
来源：http://xvt.ehwqpu.com

int|string $id
来源：http://vna.xylfe.cn

[U48] PHP：纯枚举
来源：http://jne.hnqzz.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://twt.fengsongda.top

[U49] PHP：只读属性
来源：http://cok.sweek.top

public readonly string $name
来源：http://iap.sjlbkw.cn

[U50] PHP：构造器属性提升
来源：http://odw.tarul.cn

public function __construct(private int $id) {}
来源：http://zvf.snrcjt.cn

[U51] PHP：数组解构
来源：http://nwk.xuanzx.com

[$a, $b] = $arr;
来源：http://ulo.uphjek.com

[U52] PHP：箭头函数
来源：http://qnl.tianlin.xyz

$double = fn($x) => $x * 2;
来源：http://oox.yongpay.top

[U53] PHP：空合并运算符
来源：http://vmm.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://yze.hnqzz.top

[U54] PHP：空安全调用
来源：http://ggr.shuidangran.top

$obj?->method()
来源：http://hfs.sysykeji.top

[U55] PHP：match 表达式
来源：http://hwy.aibaodan.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kke.daria6918.cn

[U56] PHP：命名参数
来源：http://xog.ctjpmb.com

f(a: 1, b: 2)
来源：http://rgq.sysykeji.top

[U57] PHP：字符串插值
来源：http://ojp.zhaomingkeji.xyz

"值: {$a}"
来源：http://ace.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://zeg.tian-w.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cyj.nwbrower.top

[U59] PHP：自定义排序
来源：http://fpl.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mrt.guannengcc.top

[U60] PHP：JSON 编解码
来源：http://cqu.sysykeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://muw.shanyushiyangtech.top

[U61] PHP：正则
来源：http://onp.c1oappe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jqj.tian-w.cn

[U62] PHP：日期对象
来源：http://azu.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gpr.iojbl.cn

[U63] PHP：文件读写
来源：http://orb.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jzx.daxiang520.top

[U64] PHP：目录遍历
来源：http://dad.jiagoushi.top

glob("dir/*.php");  scandir("dir");
来源：http://gxl.nanxuanxn.top

[U65] PHP：会话
来源：http://vnm.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dhv.sufxvd.cn

[U66] PHP：设置 Cookie
来源：http://pcz.52xcode.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lpf.sxryk.cn

[U67] PHP：处理文件上传
来源：http://sdc.aibaodan.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wzg.ivvv.top

[U68] PHP：PDO 连接
来源：http://hdt.9152youxi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mzu.xziqi.cn

[U69] PHP：PDO 预处理
来源：http://gkk.jiagoushi.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://icj.vehdjk.com

[U70] PHP：PDO 事务
来源：http://vmy.gogol.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jhw.kuanghao11.cn

[U71] PHP：抛出异常
来源：http://klb.yanxiufei.cn

throw new RuntimeException("失败", 500);
来源：http://ysn.hnqzz.top

[U72] PHP：写错误日志
来源：http://gfu.nanxinkj.top

error_log("失败: " . $e->getMessage());
来源：http://ybe.fengsongda.top

[U73] PHP：读取 ini 配置
来源：http://ohv.dianchejie.cn

parse_ini_file("config.ini", true)
来源：http://adw.jinghuilouyu.cn

[U74] PHP：读取环境变量
来源：http://orv.ivvv.top

getenv("APP_ENV") ?: "production"
来源：http://jeg.sufxvd.cn

[U75] PHP：依赖注入
来源：http://fbj.birdmap.top

composer require psr/container
来源：http://mme.meibo888.top

[U76] PHP：简单路由
来源：http://bev.cdnleiting.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lqf.epnwcf.com

[U77] PHP：模板渲染
来源：http://pfj.cdnleiting.top

composer require twig/twig
来源：http://klz.xuetiantiany.cn

[U78] PHP：单元测试
来源：http://okq.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://qxq.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://iao.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://unp.tarul.cn

[U80] PHP：代码规范修复
来源：http://wvi.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ufw.sjlbkw.cn

[U81] JS：初始化项目
来源：http://akf.shangyingyoupin.top

npm init -y;  npm i express
来源：http://zyj.zhiwuduotai.top

[U82] JS：package.json 脚本
来源：http://hls.yangfankeji.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rot.cheryme.top

[U83] JS：ES Module 导入导出
来源：http://hsi.fehbvm.com

export const a = 1;  import { a } from "./m.js";
来源：http://qbx.cdnleiting.top

[U84] JS：CommonJS 写法
来源：http://fzw.wangdashe.top

module.exports = { a };  const { a } = require("./m");
来源：http://vvr.hammf.cn

[U85] JS：可选链
来源：http://nse.zhiwuduotai.top

a?.b?.c
来源：http://oih.xylfe.cn

[U86] JS：空值合并
来源：http://sct.yueranfly.top

a ?? b
来源：http://zjb.hongshengwenyu.top

[U87] JS：解构默认值
来源：http://ucr.zhixingplan.top

const { a = 1, b = 2 } = obj;
来源：http://qib.sufxvd.cn

[U88] JS：对象展开合并
来源：http://hyx.bjfxy.top

{ ...a, ...b }
来源：http://jhx.haohaochexian.top

[U89] JS：数组去重
来源：http://ytk.jinqigfzy.top

[...new Set(arr)]
来源：http://fcs.meibo888.top

[U90] JS：数字数组排序
来源：http://rmd.birdmap.top

[...arr].sort((a, b) => a - b)
来源：http://tez.zycfv.cn

[U91] JS：对象键值遍历
来源：http://tzw.yj20258.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ych.fanxiaobao.xyz

[U92] JS：深拷贝
来源：http://zsc.ywan-chungtsiang.top

structuredClone(obj)
来源：http://ixl.ctjpmb.com

[U93] JS：模板字符串
来源：http://rav.tanke756.top

`共 ${n} 条`
来源：http://ceb.dianchejie.cn

[U94] JS：箭头函数
来源：http://ahl.zhiwuduotai.top

const double = x => x * 2;
来源：http://vje.ydzc1.top

[U95] JS：Promise 包装
来源：http://pfz.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://opz.hywenlv.cn

[U96] JS：async/await 与异常
来源：http://tol.aibaodan.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dxz.zycfv.cn

[U97] JS：并发请求
来源：http://pix.yj20258.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bgh.haohaochexian.top

[U98] JS：fetch 带 JSON
来源：http://jmb.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pxa.jinqigufen.top

[U99] JS：事件监听
来源：http://izo.52xcode.cn

el.addEventListener("click", e => {})
来源：http://awc.ydzc1.top

[U100] JS：DOM 查询
来源：http://ktd.chenzaomai.com

document.querySelector(".item")
来源：http://vio.xziqi.cn

[U101] JS：classList 操作
来源：http://wug.gogol.net.cn

el.classList.toggle("active")
来源：http://dsx.shuidangran.top

[U102] JS：本地存储
来源：http://tyx.52xcode.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mhg.aibaodan.cn

[U103] JS：定时器
来源：http://yqo.mhx1999.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oja.dashuyun.cn

[U104] JS：防抖
来源：http://ogc.dashuyun.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fui.9152youxi.cn

[U105] JS：节流
来源：http://lwh.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tjm.jlsjyb.cn

[U106] JS：日期格式化
来源：http://sgw.yvedp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qyz.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://ifs.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xnd.tianlin.xyz

[U108] JS：随机整数
来源：http://sxo.zhijiandao.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://smk.havefunace.top

[U109] JS：数组分组
来源：http://qpk.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://qou.ybcxt.top

[U110] JS：数组分块
来源：http://hqu.cheryme.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tvc.zdqjudy.top

[U111] JS：对象转 Map
来源：http://jks.hesvh.cn

new Map(Object.entries(obj))
来源：http://ucw.redwolf501.top

[U112] JS：字符串补位
来源：http://uxz.hesvh.cn

"7".padStart(3, "0")
来源：http://uiy.xinyue.icu

[U113] JS：正则替换全部
来源：http://mkr.svipenyu.cn

s.replaceAll("a", "b")
来源：http://nxh.316326.xyz

[U114] JS：JSON 深比较
来源：http://xzf.gzhubu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tln.yj20258888.top

[U115] JS：生成 UUID
来源：http://oyh.snrcjt.cn

crypto.randomUUID()
来源：http://qom.iojbl.cn

[U116] JS：类型检查（JSDoc）
来源：http://rki.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://dpl.yj20258888.top


<!-- 参考信息 -->