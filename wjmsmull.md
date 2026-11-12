代发 wailian999

[T31] Lua：Hello World
来源：http://kol.hfpthk.cn

print("Hello")
来源：http://lxu.pycfn.com

[T32] Lua：局部变量
来源：http://fwp.kuanghao11.cn

local a = 1
来源：http://ehg.cheryme.top

[T33] Lua：表（数组）
来源：http://ezh.hfpthk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ufq.gotoacloud.top

[T34] Lua：遍历表
来源：http://hur.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cze.daria6918.cn

[T35] Lua：字典表
来源：http://qxa.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://xcx.fzhhl.top

[T36] Lua：函数
来源：http://nqz.meibo888.top

function add(a, b) return a + b end
来源：http://iqc.tarul.cn

[T37] Lua：字符串拼接
来源：http://hko.sjlbkw.cn

"a" .. "b"
来源：http://elq.jinyuanbaomall.cn

[T38] Lua：条件
来源：http://rbn.316326.xyz

if x > 0 then print("正") end
来源：http://snr.jiagoushi.top

[T39] Lua：模式匹配
来源：http://xdb.zycfv.cn

string.find(s, "%d+")
来源：http://ynn.daria6918.cn

[T40] Lua：元表
来源：http://ajn.pycfn.com

setmetatable({}, { __index = base })
来源：http://sqd.jiagoushi.top

[T41] Perl：Hello World
来源：http://lni.zhixingplan.top

print "Hello\n";
来源：http://wrv.meibo888.top

[T42] Perl：变量类型
来源：http://rff.jianghu66.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ish.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://abo.0kj1m.cn

"值: $a"
来源：http://wgg.ppjwa.cn

[T44] Perl：条件
来源：http://frq.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://kcx.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://vbf.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://kpt.vqdsnc.cn

[T46] Perl：哈希操作
来源：http://biu.xuanzx.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lbk.jinyuanbaomall.cn

[T47] Perl：正则捕获
来源：http://yyq.zhixingplan.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://upd.iojbl.cn

[T48] Perl：正则替换
来源：http://xtr.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://amf.sufxvd.cn

[T49] Perl：函数
来源：http://ftl.jlsjyb.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://goo.yfazqb.com

[T50] Perl：逐行读文件
来源：http://xke.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nsw.yueranfly.top

while (my $line = <$fh>) { print $line; }
来源：http://rhy.nwbrower.top

[T51] Scala：Hello World
来源：http://vxu.shzxlz.cn

println("Hello")
来源：http://jgj.epnwcf.com

[T52] Scala：变量
来源：http://gvl.316326.xyz

val a = 1;  var b = 2
来源：http://xkw.hywenlv.cn

[T53] Scala：字符串插值
来源：http://pug.jinqigufen.top

s"值: $b"
来源：http://ben.0kj1m.cn

[T54] Scala：集合映射
来源：http://uyu.yj20258888.top

List(1, 2, 3).map(_ * 2)
来源：http://fji.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://kra.zycfv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sib.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://ret.birdmap.top

case class User(name: String, age: Int)
来源：http://ydb.ywan-chungtsiang.top

[T57] Scala：模式匹配
来源：http://ybv.fehbvm.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://kwm.xinyue.icu

[T58] Scala：函数定义
来源：http://xhq.sufxvd.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zht.wangshuangyany.cn

[T59] Scala：循环
来源：http://cvk.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://meq.cheryme.top

[T60] Scala：折叠
来源：http://oeb.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uhm.yfazqb.com

================================================================================
来源：http://phx.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dgl.yonumen.top

================================================================================
来源：http://xhv.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://nse.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://vqc.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://tlz.zdqjudy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://doe.jianghu66.top

[U03] Py：加载 .env 配置
来源：http://gos.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ovk.wangdashe.top

[U04] Py：变量调试打印
来源：http://xdp.jinyuanbaomall.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hfm.tarul.cn

[U05] Py：列表去重且保序
来源：http://mxh.pycfn.com

list(dict.fromkeys(arr))
来源：http://uyo.smart0.xyz

[U06] Py：合并两个字典
来源：http://gww.shuidangran.top

{**a, **b}
来源：http://xfg.redwolf501.top

[U07] Py：反转字典键值
来源：http://mlk.xylfe.cn

{v: k for k, v in d.items()}
来源：http://dba.birdmap.top

[U08] Py：展平二维列表
来源：http://ilz.mhx1999.top

[y for x in nested for y in x]
来源：http://rpe.ydjk.org.cn

[U09] Py：字典取最大值的键
来源：http://ilo.hcnkem.com

max(d, key=d.get)
来源：http://rhe.sysykeji.top

[U10] Py：按值排序字典
来源：http://amx.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tyr.cqqwz.cn

[U11] Py：生成器表达式
来源：http://xkp.tian-w.cn

(x * 2 for x in arr)
来源：http://xcy.jianghu66.top

[U12] Py：取出现最多的 3 个元素
来源：http://cfc.daxiang520.top

Counter(arr).most_common(3)
来源：http://upv.cdnleiting.top

[U13] Py：固定长度队列
来源：http://ikj.ydzc1.top

deque(maxlen=10)
来源：http://ize.hywenlv.cn

[U14] Py：分组收集到列表
来源：http://pcm.vehdjk.com

defaultdict(list)
来源：http://ecp.daria6918.cn

[U15] Py：高精度计时
来源：http://pag.xylfe.cn

t = time.perf_counter()
来源：http://cnp.0kj1m.cn

[U16] Py：命令行参数解析
来源：http://qqb.kuanghao11.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bto.zdqjudy.top

[U17] Py：初始化日志
来源：http://rku.aizwys.cn

logging.basicConfig(level=logging.INFO)
来源：http://edy.0kj1m.cn

[U18] Py：预编译正则
来源：http://qwc.shuidangran.top

pat = re.compile(r"\d+")
来源：http://qnp.cashguo.top

[U19] Py：正则替换带回调
来源：http://yja.zhengqikj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cpi.redwolf501.top

[U20] Py：缓存函数结果
来源：http://trh.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://fon.hnxiangtu.top

[U21] Py：自定义上下文管理器
来源：http://yre.fanxiaobao.xyz

@contextlib.contextmanager
来源：http://mip.zhengqikj.top

[U22] Py：矩阵转置
来源：http://dux.shuidangran.top

list(zip(*m))
来源：http://erj.xziqi.cn

[U23] Py：分块读取大文件
来源：http://yjl.c1oappe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://knr.ydzc1.top

[U24] Py：路径操作
来源：http://gwp.fktsv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xrv.xylfe.cn

[U25] Py：CSV 按字典读
来源：http://krh.zdbjq.cn

csv.DictReader(f)
来源：http://fyd.fktsv.cn

[U26] Py：并发下载
来源：http://dzn.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wek.wangdashe.top

[U27] Py：异步 HTTP
来源：http://xay.aizwys.cn

aiohttp.ClientSession() 配合 async with
来源：http://sbh.jqgufenzy.top

[U28] Py：类型别名
来源：http://vbo.yj20258.top

UserId = int
来源：http://xdh.bjfxy.top

[U29] Py：属性校验
来源：http://zsp.ivvv.top

@property 与 @x.setter 配合
来源：http://wpr.uphjek.com

[U30] Py：数据类
来源：http://rfm.feifeiyinyue.top

@dataclass(slots=True)
来源：http://qwv.shuidangran.top

[U31] Py：单测
来源：http://nqp.ehwqpu.com

python -m pytest -q
来源：http://aep.fanxiaobao.xyz

[U32] Py：代码格式化
来源：http://qlb.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://elq.jqgfzy.top

[U33] Py：打包发布
来源：http://wjj.kuanghao11.cn

python -m build  （依赖 pyproject.toml）
来源：http://qld.xingfuxueyuan.xyz

[U34] Py：判断编码
来源：http://tow.dianchejie.cn

chardet.detect(raw)
来源：http://xsl.xziqi.cn

[U35] Py：发送邮件
来源：http://udr.smart0.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tcm.tanke756.top

[U36] Py：定时任务
来源：http://klc.yvedp.cn

schedule.every(10).minutes.do(job)
来源：http://ujb.feifeiyinyue.top

[U37] Py：读写 Excel
来源：http://zxk.ybcxt.top

pandas.read_excel / DataFrame.to_excel
来源：http://byw.yj202588.top

[U38] Py：获取脚本所在目录
来源：http://old.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://tlv.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://gti.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://yvd.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://bbk.fanxiaobao.xyz

print("err", file=sys.stderr)
来源：http://nxf.redwolf501.top

[U41] PHP：初始化 Composer 项目
来源：http://cdf.ivvv.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uxt.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://quy.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lux.ywan-chungtsiang.top

[U43] PHP：声明命名空间
来源：http://dvc.gotoacloud.top

namespace App\Http;
来源：http://kru.tian-w.cn

[U44] PHP：开启严格类型
来源：http://ppm.hongshengwenyu.top

declare(strict_types=1);
来源：http://vsc.zhengqikj.top

[U45] PHP：类型声明与返回类型
来源：http://otl.316326.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://pkk.fanxiaobao.xyz

[U46] PHP：可空类型
来源：http://wlo.svipenyu.cn

?string $name = null
来源：http://bum.redwolf501.top

[U47] PHP：联合类型
来源：http://oiw.wangshuangyany.cn

int|string $id
来源：http://qwc.chenjidiqi.icu

[U48] PHP：纯枚举
来源：http://ddq.yanxiufei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://otm.meibo888.top

[U49] PHP：只读属性
来源：http://xuo.quarkkingdee.top

public readonly string $name
来源：http://sef.hammf.cn

[U50] PHP：构造器属性提升
来源：http://txf.guannengcc.top

public function __construct(private int $id) {}
来源：http://fzj.mhx1999.top

[U51] PHP：数组解构
来源：http://eln.yueranfly.top

[$a, $b] = $arr;
来源：http://nur.hammf.cn

[U52] PHP：箭头函数
来源：http://qft.0kj1m.cn

$double = fn($x) => $x * 2;
来源：http://plc.feifeiyinyue.top

[U53] PHP：空合并运算符
来源：http://jfz.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://qea.zycfv.cn

[U54] PHP：空安全调用
来源：http://wgv.zycfv.cn

$obj?->method()
来源：http://wpi.yangfankeji.com

[U55] PHP：match 表达式
来源：http://ufc.ybcxt.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zcl.sxryk.cn

[U56] PHP：命名参数
来源：http://opf.sweek.top

f(a: 1, b: 2)
来源：http://jfp.shuidangran.top

[U57] PHP：字符串插值
来源：http://vox.sysykeji.top

"值: {$a}"
来源：http://dhg.chenlongwang.top

[U58] PHP：数组三件套
来源：http://zqm.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blp.ppjwa.cn

[U59] PHP：自定义排序
来源：http://ajz.sjlbkw.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aqn.epnwcf.com

[U60] PHP：JSON 编解码
来源：http://ohc.yueranfly.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jyy.chenzaomai.com

[U61] PHP：正则
来源：http://otn.shangyingyoupin.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fow.cdnleiting.top

[U62] PHP：日期对象
来源：http://mkc.yuanzhike.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://opz.svipenyu.cn

[U63] PHP：文件读写
来源：http://jtz.smart0.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mjg.haohaochexian.top

[U64] PHP：目录遍历
来源：http://mna.pengpengdd.cyou

glob("dir/*.php");  scandir("dir");
来源：http://oog.yanxiufei.cn

[U65] PHP：会话
来源：http://sox.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://phk.uphjek.com

[U66] PHP：设置 Cookie
来源：http://blh.jqgfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gfm.zdbjq.cn

[U67] PHP：处理文件上传
来源：http://eao.aibaodan.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kwn.9152youxi.cn

[U68] PHP：PDO 连接
来源：http://prr.wangdashe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ulb.dianchejie.cn

[U69] PHP：PDO 预处理
来源：http://xnt.hesvh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://whu.nwbrower.top

[U70] PHP：PDO 事务
来源：http://tqe.uphjek.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vws.nanxuanxn.top

[U71] PHP：抛出异常
来源：http://arr.hesvh.cn

throw new RuntimeException("失败", 500);
来源：http://jqf.xingfuxueyuan.xyz

[U72] PHP：写错误日志
来源：http://dxf.mhx1999.top

error_log("失败: " . $e->getMessage());
来源：http://hfw.yj202588.top

[U73] PHP：读取 ini 配置
来源：http://qso.hesvh.cn

parse_ini_file("config.ini", true)
来源：http://lbi.gzhubu.top

[U74] PHP：读取环境变量
来源：http://mya.hfpthk.cn

getenv("APP_ENV") ?: "production"
来源：http://lst.tianlin.xyz

[U75] PHP：依赖注入
来源：http://rie.jinghuilouyu.cn

composer require psr/container
来源：http://yho.andypj.xyz

[U76] PHP：简单路由
来源：http://vhk.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fjn.shuidangran.top

[U77] PHP：模板渲染
来源：http://amq.zhengqikj.top

composer require twig/twig
来源：http://fer.52xcode.cn

[U78] PHP：单元测试
来源：http://qop.52xcode.cn

composer require --dev phpunit/phpunit
来源：http://tcb.uphjek.com

[U79] PHP：静态分析
来源：http://ziv.xuetiantiany.cn

composer require --dev phpstan/phpstan
来源：http://inq.xylfe.cn

[U80] PHP：代码规范修复
来源：http://afk.xuanzx.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://gnp.yangfankeji.com

[U81] JS：初始化项目
来源：http://iib.daxiang520.top

npm init -y;  npm i express
来源：http://cap.vehdjk.com

[U82] JS：package.json 脚本
来源：http://bys.cucudq.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mni.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://plg.shuidangran.top

export const a = 1;  import { a } from "./m.js";
来源：http://dtg.yongpay.top

[U84] JS：CommonJS 写法
来源：http://bcg.cdnleiting.top

module.exports = { a };  const { a } = require("./m");
来源：http://nze.cqqwz.cn

[U85] JS：可选链
来源：http://zne.aibaodan.cn

a?.b?.c
来源：http://csk.ywan-chungtsiang.top

[U86] JS：空值合并
来源：http://ffu.zdbjq.cn

a ?? b
来源：http://dyf.yj20258.top

[U87] JS：解构默认值
来源：http://edj.ydjk.org.cn

const { a = 1, b = 2 } = obj;
来源：http://sui.tianlin.xyz

[U88] JS：对象展开合并
来源：http://hni.cheryme.top

{ ...a, ...b }
来源：http://mrn.sysykeji.top

[U89] JS：数组去重
来源：http://zop.iojbl.cn

[...new Set(arr)]
来源：http://ohr.mhx1999.top

[U90] JS：数字数组排序
来源：http://fnt.ppjwa.cn

[...arr].sort((a, b) => a - b)
来源：http://yva.yuxming.cn

[U91] JS：对象键值遍历
来源：http://pcl.yonumen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://prl.jinghuilouyu.cn

[U92] JS：深拷贝
来源：http://pwc.hesvh.cn

structuredClone(obj)
来源：http://qtp.shanyushiyangtech.top

[U93] JS：模板字符串
来源：http://ldj.jlsjyb.cn

`共 ${n} 条`
来源：http://ima.yangfankeji.com

[U94] JS：箭头函数
来源：http://avx.xingfuxueyuan.xyz

const double = x => x * 2;
来源：http://vip.fzhhl.top

[U95] JS：Promise 包装
来源：http://syz.sysykeji.top

new Promise((resolve, reject) => {})
来源：http://jzj.ehwqpu.com

[U96] JS：async/await 与异常
来源：http://ucd.ywan-chungtsiang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uwp.dianchejie.cn

[U97] JS：并发请求
来源：http://crf.9152youxi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vsk.jianghu66.top

[U98] JS：fetch 带 JSON
来源：http://dgv.jyoumei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://off.gogol.net.cn

[U99] JS：事件监听
来源：http://zcr.zhiwuduotai.top

el.addEventListener("click", e => {})
来源：http://tir.wangdashe.top

[U100] JS：DOM 查询
来源：http://hwh.yongpay.top

document.querySelector(".item")
来源：http://ktx.wangdashe.top

[U101] JS：classList 操作
来源：http://vnz.yj202588.top

el.classList.toggle("active")
来源：http://nbc.ywan-chungtsiang.top

[U102] JS：本地存储
来源：http://jep.tarul.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qno.gaohongyu789.top

[U103] JS：定时器
来源：http://oyz.xingfuxueyuan.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ycj.zhijiandao.cn

[U104] JS：防抖
来源：http://goo.yonumen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bec.yonumen.top

[U105] JS：节流
来源：http://sfr.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zbu.zhaomingkeji.xyz

[U106] JS：日期格式化
来源：http://yfe.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dvw.fengsongda.top

[U107] JS：数字千分位
来源：http://drs.xylfe.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tpb.shzxlz.cn

[U108] JS：随机整数
来源：http://gqn.cdnleiting.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jvl.ppjwa.cn

[U109] JS：数组分组
来源：http://mkt.shanyushiyangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://krx.daria6918.cn

[U110] JS：数组分块
来源：http://tnp.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bii.jinyuanbaomall.cn

[U111] JS：对象转 Map
来源：http://csl.ywan-chungtsiang.top

new Map(Object.entries(obj))
来源：http://aku.jinghuilouyu.cn

[U112] JS：字符串补位
来源：http://nnx.hnxiangtu.top

"7".padStart(3, "0")
来源：http://mhv.jiagoushi.top

[U113] JS：正则替换全部
来源：http://tjr.snrcjt.cn

s.replaceAll("a", "b")
来源：http://scs.vehdjk.com

[U114] JS：JSON 深比较
来源：http://szs.9152youxi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pib.dashuyun.cn

[U115] JS：生成 UUID
来源：http://fxh.tanke756.top

crypto.randomUUID()
来源：http://lgw.fehbvm.com

[U116] JS：类型检查（JSDoc）
来源：http://rrk.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://pqo.hammf.cn

[U117] JS：单元测试
来源：http://mwg.feifeiyinyue.top

npm i -D vitest;  npx vitest
来源：http://hry.aibaodan.cn

[U118] JS：开发服务器
来源：http://nwm.fengsongda.top

npm i -D vite;  npx vite
来源：http://fmp.ehwqpu.com


<!-- 参考信息 -->