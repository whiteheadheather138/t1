代发 wailian999

[T33] Lua：表（数组）
来源：http://vuo.hnxiangtu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nrh.andypj.xyz

[T34] Lua：遍历表
来源：http://nre.tian-w.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lvn.smart0.xyz

[T35] Lua：字典表
来源：http://izl.chenzaomai.com

local d = { a = 1 };  d.b = 2
来源：http://fli.meibo888.top

[T36] Lua：函数
来源：http://unp.jlsjyb.cn

function add(a, b) return a + b end
来源：http://ubg.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://wsf.yj202588.top

"a" .. "b"
来源：http://nlk.yuxming.cn

[T38] Lua：条件
来源：http://zpd.aibaodan.cn

if x > 0 then print("正") end
来源：http://wao.snrcjt.cn

[T39] Lua：模式匹配
来源：http://hsn.jqgufenzy.top

string.find(s, "%d+")
来源：http://ugw.0kj1m.cn

[T40] Lua：元表
来源：http://txu.52xcode.cn

setmetatable({}, { __index = base })
来源：http://upx.andypj.xyz

[T41] Perl：Hello World
来源：http://lcu.c1oappe.top

print "Hello\n";
来源：http://nyg.aizwys.cn

[T42] Perl：变量类型
来源：http://pxx.andypj.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rfg.jiagoushi.top

[T43] Perl：字符串插值
来源：http://lvv.ydjk.org.cn

"值: $a"
来源：http://tbf.redwolf501.top

[T44] Perl：条件
来源：http://mpt.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://ytn.cheryme.top

[T45] Perl：数组遍历
来源：http://rgv.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://yqk.feifeiyinyue.top

[T46] Perl：哈希操作
来源：http://dvm.hcnkem.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wrh.jlsjyb.cn

[T47] Perl：正则捕获
来源：http://ita.chenjidiqi.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://jgo.vqdsnc.cn

[T48] Perl：正则替换
来源：http://lud.ivvv.top

$s =~ s/old/new/g;
来源：http://zra.ppjwa.cn

[T49] Perl：函数
来源：http://ssc.sweek.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vyw.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://tng.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://cjv.ydjk.org.cn

while (my $line = <$fh>) { print $line; }
来源：http://mkx.cheryme.top

[T51] Scala：Hello World
来源：http://dba.havefunace.top

println("Hello")
来源：http://icv.hcnkem.com

[T52] Scala：变量
来源：http://mpo.ybcxt.top

val a = 1;  var b = 2
来源：http://krp.chenzaomai.com

[T53] Scala：字符串插值
来源：http://ivx.gzhubu.top

s"值: $b"
来源：http://vsw.zhoulong.xyz

[T54] Scala：集合映射
来源：http://ooj.zhaomingkeji.xyz

List(1, 2, 3).map(_ * 2)
来源：http://nbb.jqgufenzy.top

[T55] Scala：集合过滤
来源：http://qor.sjlbkw.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jiq.316326.xyz

[T56] Scala：样例类
来源：http://sjd.chenlongwang.top

case class User(name: String, age: Int)
来源：http://fee.vehdjk.com

[T57] Scala：模式匹配
来源：http://trq.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://siw.gzhubu.top

[T58] Scala：函数定义
来源：http://bii.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://lcr.zhijiandao.cn

[T59] Scala：循环
来源：http://yta.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://quy.jinqigufen.top

[T60] Scala：折叠
来源：http://who.zhixingplan.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xku.jiagoushi.top

================================================================================
来源：http://aie.nanxuanxn.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hzw.yanxiufei.cn

================================================================================
来源：http://mla.yanxiufei.cn

[U01] Py：创建虚拟环境
来源：http://xpm.hfpthk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xgk.ydzc1.top

[U02] Py：导出 / 安装依赖
来源：http://tep.shangyingyoupin.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ewz.zdqjudy.top

[U03] Py：加载 .env 配置
来源：http://hhi.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://taw.ydzc1.top

[U04] Py：变量调试打印
来源：http://yfa.yj20258.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jif.ppjwa.cn

[U05] Py：列表去重且保序
来源：http://tdc.jinghuilouyu.cn

list(dict.fromkeys(arr))
来源：http://byl.jianghu66.top

[U06] Py：合并两个字典
来源：http://mbk.feifeiyinyue.top

{**a, **b}
来源：http://xkq.xziqi.cn

[U07] Py：反转字典键值
来源：http://sin.yueranfly.top

{v: k for k, v in d.items()}
来源：http://tot.xingfuxueyuan.xyz

[U08] Py：展平二维列表
来源：http://fhk.zhixingplan.top

[y for x in nested for y in x]
来源：http://xqd.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://zky.hnxiangtu.top

max(d, key=d.get)
来源：http://ycn.zdqjudy.top

[U10] Py：按值排序字典
来源：http://unc.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mcm.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://ifo.yueranfly.top

(x * 2 for x in arr)
来源：http://xbq.jiagoushi.top

[U12] Py：取出现最多的 3 个元素
来源：http://edx.xinyue.icu

Counter(arr).most_common(3)
来源：http://cge.shuidangran.top

[U13] Py：固定长度队列
来源：http://thp.daria6918.cn

deque(maxlen=10)
来源：http://kqo.jianghu66.top

[U14] Py：分组收集到列表
来源：http://plt.nanxinkj.top

defaultdict(list)
来源：http://ohs.shuidangran.top

[U15] Py：高精度计时
来源：http://avn.chenzaomai.com

t = time.perf_counter()
来源：http://cpt.dashuyun.cn

[U16] Py：命令行参数解析
来源：http://jwd.sxryk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ruj.ehwqpu.com

[U17] Py：初始化日志
来源：http://mpo.smart0.xyz

logging.basicConfig(level=logging.INFO)
来源：http://zqi.zycfv.cn

[U18] Py：预编译正则
来源：http://ogu.ybcxt.top

pat = re.compile(r"\d+")
来源：http://hxk.snrcjt.cn

[U19] Py：正则替换带回调
来源：http://osa.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ruv.chenzaomai.com

[U20] Py：缓存函数结果
来源：http://nvw.dianchejie.cn

@functools.lru_cache(maxsize=None)
来源：http://rzb.fanxiaobao.xyz

[U21] Py：自定义上下文管理器
来源：http://hfb.snrcjt.cn

@contextlib.contextmanager
来源：http://jxv.xziqi.cn

[U22] Py：矩阵转置
来源：http://ayc.pycfn.com

list(zip(*m))
来源：http://jmq.zhixingplan.top

[U23] Py：分块读取大文件
来源：http://mai.meibo888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vrg.sufxvd.cn

[U24] Py：路径操作
来源：http://gkt.snrcjt.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dgy.yvedp.cn

[U25] Py：CSV 按字典读
来源：http://dva.gogol.net.cn

csv.DictReader(f)
来源：http://maa.sxryk.cn

[U26] Py：并发下载
来源：http://drm.ywan-chungtsiang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jme.yueranfly.top

[U27] Py：异步 HTTP
来源：http://lxg.hnxiangtu.top

aiohttp.ClientSession() 配合 async with
来源：http://lxj.yueranfly.top

[U28] Py：类型别名
来源：http://ptn.vehdjk.com

UserId = int
来源：http://bsc.hongshengwenyu.top

[U29] Py：属性校验
来源：http://upz.bjfxy.top

@property 与 @x.setter 配合
来源：http://ogp.shangyingyoupin.top

[U30] Py：数据类
来源：http://pke.daria6918.cn

@dataclass(slots=True)
来源：http://xvh.ppjwa.cn

[U31] Py：单测
来源：http://nph.chenjidiqi.icu

python -m pytest -q
来源：http://sew.cheryme.top

[U32] Py：代码格式化
来源：http://nrf.yueranfly.top

ruff format . && ruff check --fix .
来源：http://soo.ydjk.org.cn

[U33] Py：打包发布
来源：http://boo.sjlbkw.cn

python -m build  （依赖 pyproject.toml）
来源：http://hmx.haohaochexian.top

[U34] Py：判断编码
来源：http://sao.jiagoushi.top

chardet.detect(raw)
来源：http://nnd.zdbjq.cn

[U35] Py：发送邮件
来源：http://ent.jinyuanbaomall.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ede.smart0.xyz

[U36] Py：定时任务
来源：http://xyt.yongpay.top

schedule.every(10).minutes.do(job)
来源：http://zrt.wangshuangyany.cn

[U37] Py：读写 Excel
来源：http://qcr.shuidangran.top

pandas.read_excel / DataFrame.to_excel
来源：http://qqf.pycfn.com

[U38] Py：获取脚本所在目录
来源：http://qcw.birdmap.top

Path(__file__).resolve().parent
来源：http://uhd.gogol.net.cn

[U39] Py：判断是否在交互环境
来源：http://kee.zhongyouzk.top

sys.stdout.isatty()
来源：http://tnu.zhijiandao.cn

[U40] Py：打印到标准错误
来源：http://nyx.xingfuxueyuan.xyz

print("err", file=sys.stderr)
来源：http://gfk.uphjek.com

[U41] PHP：初始化 Composer 项目
来源：http://qnz.shzxlz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wso.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://ukd.shanyushiyangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xrk.jinghuilouyu.cn

[U43] PHP：声明命名空间
来源：http://zjx.jqgufenzy.top

namespace App\Http;
来源：http://ldo.guannengcc.top

[U44] PHP：开启严格类型
来源：http://nst.gotoacloud.top

declare(strict_types=1);
来源：http://wwd.xingfuxueyuan.xyz

[U45] PHP：类型声明与返回类型
来源：http://uts.pengpengdd.cyou

function add(int $a, int $b): int { return $a + $b; }
来源：http://ruv.ywan-chungtsiang.top

[U46] PHP：可空类型
来源：http://tdu.yonumen.top

?string $name = null
来源：http://yqa.kuanghao11.cn

[U47] PHP：联合类型
来源：http://qlh.wangshuangyany.cn

int|string $id
来源：http://zya.haohaochexian.top

[U48] PHP：纯枚举
来源：http://pvq.bbcook.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vud.hnqzz.top

[U49] PHP：只读属性
来源：http://yjj.xuanzx.com

public readonly string $name
来源：http://hdn.0kj1m.cn

[U50] PHP：构造器属性提升
来源：http://tdc.svipenyu.cn

public function __construct(private int $id) {}
来源：http://fql.zhaomingkeji.xyz

[U51] PHP：数组解构
来源：http://aai.jinqigufen.top

[$a, $b] = $arr;
来源：http://fhn.gotoacloud.top

[U52] PHP：箭头函数
来源：http://qqa.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://ift.hnqzz.top

[U53] PHP：空合并运算符
来源：http://axl.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://wxd.jinqigfzy.top

[U54] PHP：空安全调用
来源：http://utd.316326.xyz

$obj?->method()
来源：http://hel.9152youxi.cn

[U55] PHP：match 表达式
来源：http://yqy.ehwqpu.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uaa.havefunace.top

[U56] PHP：命名参数
来源：http://yoh.52xcode.cn

f(a: 1, b: 2)
来源：http://vai.havefunace.top

[U57] PHP：字符串插值
来源：http://ojt.cucudq.cn

"值: {$a}"
来源：http://tun.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://bck.yongpay.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ifd.yueranfly.top

[U59] PHP：自定义排序
来源：http://wje.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pyw.birdmap.top

[U60] PHP：JSON 编解码
来源：http://kvv.kuanghao11.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xxb.meibo888.top

[U61] PHP：正则
来源：http://equ.fehbvm.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dxy.shanyushiyangkeji.top

[U62] PHP：日期对象
来源：http://jvy.hammf.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zjh.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://orf.ybcxt.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eqq.dianchejie.cn

[U64] PHP：目录遍历
来源：http://bme.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://hsr.zhengqikj.top

[U65] PHP：会话
来源：http://cza.jqgfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vxz.dianchejie.cn

[U66] PHP：设置 Cookie
来源：http://tkg.zhijiandao.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fgv.yvedp.cn

[U67] PHP：处理文件上传
来源：http://zrg.jqgfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://piw.zycfv.cn

[U68] PHP：PDO 连接
来源：http://mtc.zhaomingkeji.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fia.0kj1m.cn

[U69] PHP：PDO 预处理
来源：http://bva.smart0.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://olw.tarul.cn

[U70] PHP：PDO 事务
来源：http://xlg.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ddf.sysykeji.top

[U71] PHP：抛出异常
来源：http://cnj.xuetiantiany.cn

throw new RuntimeException("失败", 500);
来源：http://sjd.fktsv.cn

[U72] PHP：写错误日志
来源：http://ibk.daria6918.cn

error_log("失败: " . $e->getMessage());
来源：http://gjf.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://dya.zhijiandao.cn

parse_ini_file("config.ini", true)
来源：http://vbq.jianghu66.top

[U74] PHP：读取环境变量
来源：http://coy.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://rze.tianlin.xyz

[U75] PHP：依赖注入
来源：http://fhj.feifeiyinyue.top

composer require psr/container
来源：http://yje.tanke756.top

[U76] PHP：简单路由
来源：http://hsw.ybcxt.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cob.cheryme.top

[U77] PHP：模板渲染
来源：http://bup.cucudq.cn

composer require twig/twig
来源：http://dju.jinqigfzy.top

[U78] PHP：单元测试
来源：http://wno.kuanghao11.cn

composer require --dev phpunit/phpunit
来源：http://iue.xingfuxueyuan.xyz

[U79] PHP：静态分析
来源：http://qfu.xziqi.cn

composer require --dev phpstan/phpstan
来源：http://jrr.yuanzhike.top

[U80] PHP：代码规范修复
来源：http://not.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://aru.vehdjk.com

[U81] JS：初始化项目
来源：http://hoq.xuetiantiany.cn

npm init -y;  npm i express
来源：http://kdz.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://hie.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uok.sufxvd.cn

[U83] JS：ES Module 导入导出
来源：http://zen.dianchejie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hwq.hywenlv.cn

[U84] JS：CommonJS 写法
来源：http://bzv.fengsongda.top

module.exports = { a };  const { a } = require("./m");
来源：http://loz.yj202588.top

[U85] JS：可选链
来源：http://gik.jlsjyb.cn

a?.b?.c
来源：http://zoe.sysykeji.top

[U86] JS：空值合并
来源：http://htn.xingfuxueyuan.xyz

a ?? b
来源：http://krk.jinyuanbaomall.cn

[U87] JS：解构默认值
来源：http://lkz.fehbvm.com

const { a = 1, b = 2 } = obj;
来源：http://yca.guannengcc.top

[U88] JS：对象展开合并
来源：http://bqj.bjfxy.top

{ ...a, ...b }
来源：http://ncl.fehbvm.com

[U89] JS：数组去重
来源：http://srs.ydjk.org.cn

[...new Set(arr)]
来源：http://maz.svipenyu.cn

[U90] JS：数字数组排序
来源：http://bqf.jianghu66.top

[...arr].sort((a, b) => a - b)
来源：http://gbr.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://awx.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zqa.xziqi.cn

[U92] JS：深拷贝
来源：http://qwb.cheryme.top

structuredClone(obj)
来源：http://dhj.jinqigufen.top

[U93] JS：模板字符串
来源：http://wpj.ybcxt.top

`共 ${n} 条`
来源：http://ysf.xuanzx.com

[U94] JS：箭头函数
来源：http://egg.zdqjudy.top

const double = x => x * 2;
来源：http://hcw.ehwqpu.com

[U95] JS：Promise 包装
来源：http://nko.andypj.xyz

new Promise((resolve, reject) => {})
来源：http://gxb.yonumen.top

[U96] JS：async/await 与异常
来源：http://rrf.sxryk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qvh.cashguo.top

[U97] JS：并发请求
来源：http://gxi.tianlin.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://rss.jqgfzy.top

[U98] JS：fetch 带 JSON
来源：http://fct.redwolf501.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ihm.yj20258888.top

[U99] JS：事件监听
来源：http://xmf.xuetiantiany.cn

el.addEventListener("click", e => {})
来源：http://dnu.zycfv.cn

[U100] JS：DOM 查询
来源：http://myx.yj20258.top

document.querySelector(".item")
来源：http://gbr.hesvh.cn

[U101] JS：classList 操作
来源：http://gou.fanxiaobao.xyz

el.classList.toggle("active")
来源：http://kbd.sufxvd.cn

[U102] JS：本地存储
来源：http://wvl.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kkt.zdbjq.cn

[U103] JS：定时器
来源：http://cyl.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eoo.dashuyun.cn

[U104] JS：防抖
来源：http://tsl.vqdsnc.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ozc.nanxuanxn.top

[U105] JS：节流
来源：http://nyn.iojbl.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rcr.jinqigfzy.top

[U106] JS：日期格式化
来源：http://lvu.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kru.birdmap.top

[U107] JS：数字千分位
来源：http://qwb.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ifg.jlsjyb.cn

[U108] JS：随机整数
来源：http://uya.jianghu66.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tzp.fehbvm.com

[U109] JS：数组分组
来源：http://ehb.316326.xyz

Object.groupBy(arr, x => x.type)
来源：http://fqv.tanke756.top

[U110] JS：数组分块
来源：http://hem.ivvv.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://amt.yvedp.cn

[U111] JS：对象转 Map
来源：http://ugs.yvedp.cn

new Map(Object.entries(obj))
来源：http://jwe.jlsjyb.cn

[U112] JS：字符串补位
来源：http://seh.yangfankeji.com

"7".padStart(3, "0")
来源：http://thp.gogol.net.cn

[U113] JS：正则替换全部
来源：http://wgt.mhx1999.top

s.replaceAll("a", "b")
来源：http://lfj.cashguo.top

[U114] JS：JSON 深比较
来源：http://irb.gzhubu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ush.fehbvm.com

[U115] JS：生成 UUID
来源：http://uqj.gotoacloud.top

crypto.randomUUID()
来源：http://nid.jlsjyb.cn

[U116] JS：类型检查（JSDoc）
来源：http://qpg.tanke756.top

/** @param {string} name */ function f(name) {}
来源：http://fwo.sweek.top

[U117] JS：单元测试
来源：http://gav.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://zsr.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://wwl.hammf.cn

npm i -D vite;  npx vite
来源：http://zlc.sxryk.cn

[U119] JS：生产构建
来源：http://urt.fehbvm.com

npx vite build
来源：http://ttj.havefunace.top

[U120] JS：读取环境变量（Vite）
来源：http://yxa.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://vni.xinyue.icu


<!-- 参考信息 -->