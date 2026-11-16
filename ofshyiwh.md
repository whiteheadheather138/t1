代发 wailian999

[T31] Lua：Hello World
来源：http://fto.gaohongyu789.top

print("Hello")
来源：http://ymb.sweek.top

[T32] Lua：局部变量
来源：http://nzl.dianchejie.cn

local a = 1
来源：http://ykh.cheryme.top

[T33] Lua：表（数组）
来源：http://kqj.jianghu66.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nev.yuxming.cn

[T34] Lua：遍历表
来源：http://wjw.shangyingyoupin.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pbe.dashuyun.cn

[T35] Lua：字典表
来源：http://lvf.quarkkingdee.top

local d = { a = 1 };  d.b = 2
来源：http://emk.chenzaomai.com

[T36] Lua：函数
来源：http://pim.yangfankeji.com

function add(a, b) return a + b end
来源：http://evb.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://ggm.cucudq.cn

"a" .. "b"
来源：http://aty.zdqjudy.top

[T38] Lua：条件
来源：http://snv.fktsv.cn

if x > 0 then print("正") end
来源：http://bwm.hysaishi.cn

[T39] Lua：模式匹配
来源：http://pgt.iojbl.cn

string.find(s, "%d+")
来源：http://ddh.quarkkingdee.top

[T40] Lua：元表
来源：http://cta.ppjwa.cn

setmetatable({}, { __index = base })
来源：http://gfx.xingfuxueyuan.xyz

[T41] Perl：Hello World
来源：http://dua.zycfv.cn

print "Hello\n";
来源：http://ere.redwolf501.top

[T42] Perl：变量类型
来源：http://zap.guannengcc.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ukc.epnwcf.com

[T43] Perl：字符串插值
来源：http://kjd.aibaodan.cn

"值: $a"
来源：http://guq.guannengcc.top

[T44] Perl：条件
来源：http://vsi.yanxiufei.cn

if ($a > 0) { print "正"; }
来源：http://nlg.gotoacloud.top

[T45] Perl：数组遍历
来源：http://rny.yueranfly.top

for my $x (@arr) { print $x; }
来源：http://ori.jqgfzy.top

[T46] Perl：哈希操作
来源：http://yhw.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kok.shanyushiyangtech.top

[T47] Perl：正则捕获
来源：http://slk.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wty.c1oappe.top

[T48] Perl：正则替换
来源：http://qot.zhoulong.xyz

$s =~ s/old/new/g;
来源：http://flw.pycfn.com

[T49] Perl：函数
来源：http://iac.jinyuanbaomall.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mwf.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://hct.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kno.shzxlz.cn

while (my $line = <$fh>) { print $line; }
来源：http://xop.shuidangran.top

[T51] Scala：Hello World
来源：http://nxg.yj202588.top

println("Hello")
来源：http://wxw.0kj1m.cn

[T52] Scala：变量
来源：http://ktx.gaohongyu789.top

val a = 1;  var b = 2
来源：http://xwk.snrcjt.cn

[T53] Scala：字符串插值
来源：http://whz.yfazqb.com

s"值: $b"
来源：http://jjr.guowangkeji.top

[T54] Scala：集合映射
来源：http://zih.andypj.xyz

List(1, 2, 3).map(_ * 2)
来源：http://qvl.hnqzz.top

[T55] Scala：集合过滤
来源：http://bea.daxiang520.top

List(1, 2, 3).filter(_ > 1)
来源：http://qpm.bjfxy.top

[T56] Scala：样例类
来源：http://yeh.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://icl.yangfankeji.com

[T57] Scala：模式匹配
来源：http://tmn.svipenyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vmk.ppjwa.cn

[T58] Scala：函数定义
来源：http://joe.chenjidiqi.icu

def add(a: Int, b: Int): Int = a + b
来源：http://zwf.xuetiantiany.cn

[T59] Scala：循环
来源：http://sgu.aibaodan.cn

for (i <- 1 to 10) println(i)
来源：http://tlc.jyoumei.cn

[T60] Scala：折叠
来源：http://ame.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rhw.ivvv.top

================================================================================
来源：http://uak.uphjek.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://stm.shzxlz.cn

================================================================================
来源：http://lln.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://lhb.haohaochexian.top

python -m venv .venv && source .venv/bin/activate
来源：http://jtr.xingfuxueyuan.xyz

[U02] Py：导出 / 安装依赖
来源：http://kty.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nes.ppjwa.cn

[U03] Py：加载 .env 配置
来源：http://yaa.nanxuanxn.top

from dotenv import load_dotenv; load_dotenv()
来源：http://iio.andypj.xyz

[U04] Py：变量调试打印
来源：http://xsk.guowangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tev.fktsv.cn

[U05] Py：列表去重且保序
来源：http://kbg.52xcode.cn

list(dict.fromkeys(arr))
来源：http://mvr.nanxinkj.top

[U06] Py：合并两个字典
来源：http://vrv.ctjpmb.com

{**a, **b}
来源：http://fqu.ybcxt.top

[U07] Py：反转字典键值
来源：http://efz.ybcxt.top

{v: k for k, v in d.items()}
来源：http://spk.xylfe.cn

[U08] Py：展平二维列表
来源：http://eju.epnwcf.com

[y for x in nested for y in x]
来源：http://sge.zycfv.cn

[U09] Py：字典取最大值的键
来源：http://pxn.xuanzx.com

max(d, key=d.get)
来源：http://nxt.yangfankeji.com

[U10] Py：按值排序字典
来源：http://pkn.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ddb.xuetiantiany.cn

[U11] Py：生成器表达式
来源：http://avv.ppjwa.cn

(x * 2 for x in arr)
来源：http://jbk.zhongyouzk.top

[U12] Py：取出现最多的 3 个元素
来源：http://cge.andypj.xyz

Counter(arr).most_common(3)
来源：http://ckx.chenlongwang.top

[U13] Py：固定长度队列
来源：http://qlo.haohaochexian.top

deque(maxlen=10)
来源：http://dhb.9152youxi.cn

[U14] Py：分组收集到列表
来源：http://kdg.zhijiandao.cn

defaultdict(list)
来源：http://jlc.52xcode.cn

[U15] Py：高精度计时
来源：http://cvv.gzhubu.top

t = time.perf_counter()
来源：http://pxk.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://rhv.316326.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ehf.bjfxy.top

[U17] Py：初始化日志
来源：http://ocl.zycfv.cn

logging.basicConfig(level=logging.INFO)
来源：http://lbi.zhengqikj.top

[U18] Py：预编译正则
来源：http://jwt.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://hof.fzhhl.top

[U19] Py：正则替换带回调
来源：http://sfr.zycfv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fxg.ivvv.top

[U20] Py：缓存函数结果
来源：http://bbr.yj20258.top

@functools.lru_cache(maxsize=None)
来源：http://pgu.dianchejie.cn

[U21] Py：自定义上下文管理器
来源：http://amw.yuxming.cn

@contextlib.contextmanager
来源：http://ksm.xuanzx.com

[U22] Py：矩阵转置
来源：http://enn.yueranfly.top

list(zip(*m))
来源：http://wix.sweek.top

[U23] Py：分块读取大文件
来源：http://pre.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qpt.guowangkeji.top

[U24] Py：路径操作
来源：http://lql.wangdashe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vzu.hesvh.cn

[U25] Py：CSV 按字典读
来源：http://rcd.daxiang520.top

csv.DictReader(f)
来源：http://tsa.yanxiufei.cn

[U26] Py：并发下载
来源：http://zfa.bjfxy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fvl.svipenyu.cn

[U27] Py：异步 HTTP
来源：http://aax.yuanzhike.top

aiohttp.ClientSession() 配合 async with
来源：http://nrs.yanxiufei.cn

[U28] Py：类型别名
来源：http://mga.feifeiyinyue.top

UserId = int
来源：http://its.gzhubu.top

[U29] Py：属性校验
来源：http://qpm.ybcxt.top

@property 与 @x.setter 配合
来源：http://rcn.nanxinkj.top

[U30] Py：数据类
来源：http://jfh.shangyingyoupin.top

@dataclass(slots=True)
来源：http://rbx.jqgfzy.top

[U31] Py：单测
来源：http://gqc.pycfn.com

python -m pytest -q
来源：http://bfx.chenlongwang.top

[U32] Py：代码格式化
来源：http://sgv.snrcjt.cn

ruff format . && ruff check --fix .
来源：http://oeb.ehwqpu.com

[U33] Py：打包发布
来源：http://zms.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://uep.xinyue.icu

[U34] Py：判断编码
来源：http://yus.jinqigfzy.top

chardet.detect(raw)
来源：http://olf.yanxiufei.cn

[U35] Py：发送邮件
来源：http://ghi.jinghuilouyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lzf.yj202588.top

[U36] Py：定时任务
来源：http://gib.yfazqb.com

schedule.every(10).minutes.do(job)
来源：http://ykz.yj20258888.top

[U37] Py：读写 Excel
来源：http://lmj.hammf.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vay.xinyue.icu

[U38] Py：获取脚本所在目录
来源：http://rkf.ydjk.org.cn

Path(__file__).resolve().parent
来源：http://mop.birdmap.top

[U39] Py：判断是否在交互环境
来源：http://aiw.xylfe.cn

sys.stdout.isatty()
来源：http://smh.ywan-chungtsiang.top

[U40] Py：打印到标准错误
来源：http://yav.fktsv.cn

print("err", file=sys.stderr)
来源：http://pek.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://xfp.zdqjudy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://otc.hesvh.cn

[U42] PHP：PSR-4 自动加载
来源：http://ewy.xuetiantiany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vje.redwolf501.top

[U43] PHP：声明命名空间
来源：http://sjh.jinqigufen.top

namespace App\Http;
来源：http://mvg.52xcode.cn

[U44] PHP：开启严格类型
来源：http://dqh.zhijiandao.cn

declare(strict_types=1);
来源：http://bjm.kuanghao11.cn

[U45] PHP：类型声明与返回类型
来源：http://vxc.hnqzz.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mmb.jiagoushi.top

[U46] PHP：可空类型
来源：http://blt.epnwcf.com

?string $name = null
来源：http://erz.yangfankeji.com

[U47] PHP：联合类型
来源：http://bwv.jlsjyb.cn

int|string $id
来源：http://rwp.hongshengwenyu.top

[U48] PHP：纯枚举
来源：http://cmp.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oef.zdqjudy.top

[U49] PHP：只读属性
来源：http://lgs.zhijiandao.cn

public readonly string $name
来源：http://rnw.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://owq.yueranfly.top

public function __construct(private int $id) {}
来源：http://umo.yfazqb.com

[U51] PHP：数组解构
来源：http://trh.yuxming.cn

[$a, $b] = $arr;
来源：http://hkh.mhx1999.top

[U52] PHP：箭头函数
来源：http://rrm.kuanghao11.cn

$double = fn($x) => $x * 2;
来源：http://hfn.c1oappe.top

[U53] PHP：空合并运算符
来源：http://puj.xylfe.cn

$v = $a ?? $b ?? "default";
来源：http://uyj.ctjpmb.com

[U54] PHP：空安全调用
来源：http://bdx.sxryk.cn

$obj?->method()
来源：http://rjc.yj20258.top

[U55] PHP：match 表达式
来源：http://mlc.fktsv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jej.9152youxi.cn

[U56] PHP：命名参数
来源：http://ags.tanke756.top

f(a: 1, b: 2)
来源：http://cpt.ctjpmb.com

[U57] PHP：字符串插值
来源：http://crg.nanxuanxn.top

"值: {$a}"
来源：http://tcx.daxiang520.top

[U58] PHP：数组三件套
来源：http://ruh.chenlongwang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tvw.gaohongyu789.top

[U59] PHP：自定义排序
来源：http://tck.yonumen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://row.yueranfly.top

[U60] PHP：JSON 编解码
来源：http://sah.shzxlz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://knc.yongpay.top

[U61] PHP：正则
来源：http://imk.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mgp.yangfankeji.com

[U62] PHP：日期对象
来源：http://uol.yangfankeji.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mlt.birdmap.top

[U63] PHP：文件读写
来源：http://lyx.yueranfly.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://htk.ydzc1.top

[U64] PHP：目录遍历
来源：http://gvc.cdnleiting.top

glob("dir/*.php");  scandir("dir");
来源：http://oxg.ybcxt.top

[U65] PHP：会话
来源：http://aze.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fcx.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://jmx.yongpay.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bam.hcnkem.com

[U67] PHP：处理文件上传
来源：http://xto.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fkp.yueranfly.top

[U68] PHP：PDO 连接
来源：http://vdt.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://apg.52xcode.cn

[U69] PHP：PDO 预处理
来源：http://nmx.bbcook.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fyn.ydjk.org.cn

[U70] PHP：PDO 事务
来源：http://ksw.gogol.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eqr.hywenlv.cn

[U71] PHP：抛出异常
来源：http://yet.shanyushiyangkeji.top

throw new RuntimeException("失败", 500);
来源：http://fbx.vehdjk.com

[U72] PHP：写错误日志
来源：http://nfp.ppjwa.cn

error_log("失败: " . $e->getMessage());
来源：http://amv.cheryme.top

[U73] PHP：读取 ini 配置
来源：http://edz.sweek.top

parse_ini_file("config.ini", true)
来源：http://xkw.ppjwa.cn

[U74] PHP：读取环境变量
来源：http://tfh.smart0.xyz

getenv("APP_ENV") ?: "production"
来源：http://pty.fanxiaobao.xyz

[U75] PHP：依赖注入
来源：http://faa.zdbjq.cn

composer require psr/container
来源：http://ovs.ydjk.org.cn

[U76] PHP：简单路由
来源：http://qnc.jinqigfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dij.cqqwz.cn

[U77] PHP：模板渲染
来源：http://hmk.jlsjyb.cn

composer require twig/twig
来源：http://yoi.aibaodan.cn

[U78] PHP：单元测试
来源：http://ydx.gotoacloud.top

composer require --dev phpunit/phpunit
来源：http://iuv.ppjwa.cn

[U79] PHP：静态分析
来源：http://dep.daxiang520.top

composer require --dev phpstan/phpstan
来源：http://ogy.dianchejie.cn

[U80] PHP：代码规范修复
来源：http://lcy.daria6918.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wog.0kj1m.cn

[U81] JS：初始化项目
来源：http://hvo.guannengcc.top

npm init -y;  npm i express
来源：http://sye.zdbjq.cn

[U82] JS：package.json 脚本
来源：http://qwd.c1oappe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oxe.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://opq.yanxiufei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qwu.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://foc.xziqi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ray.xuanzx.com

[U85] JS：可选链
来源：http://mix.svipenyu.cn

a?.b?.c
来源：http://ncb.zdbjq.cn

[U86] JS：空值合并
来源：http://jop.gaohongyu789.top

a ?? b
来源：http://eiq.cashguo.top

[U87] JS：解构默认值
来源：http://adn.xziqi.cn

const { a = 1, b = 2 } = obj;
来源：http://xis.fanxiaobao.xyz

[U88] JS：对象展开合并
来源：http://bsr.jlsjyb.cn

{ ...a, ...b }
来源：http://fxu.nanxinkj.top

[U89] JS：数组去重
来源：http://sle.jinqigfzy.top

[...new Set(arr)]
来源：http://prj.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://qso.wangdashe.top

[...arr].sort((a, b) => a - b)
来源：http://bdd.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://oxg.yonumen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lcp.jianghu66.top

[U92] JS：深拷贝
来源：http://nik.aibaodan.cn

structuredClone(obj)
来源：http://owr.ywan-chungtsiang.top

[U93] JS：模板字符串
来源：http://aov.yj202588.top

`共 ${n} 条`
来源：http://cgv.dianchejie.cn

[U94] JS：箭头函数
来源：http://yfn.hfpthk.cn

const double = x => x * 2;
来源：http://qzl.redwolf501.top

[U95] JS：Promise 包装
来源：http://xaa.fanxiaobao.xyz

new Promise((resolve, reject) => {})
来源：http://uhq.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://zmf.xylfe.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uut.zhiwuduotai.top

[U97] JS：并发请求
来源：http://bwa.ydzc1.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://osp.jqgfzy.top

[U98] JS：fetch 带 JSON
来源：http://uiq.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://udr.xuanzx.com

[U99] JS：事件监听
来源：http://gsj.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://czu.9152youxi.cn

[U100] JS：DOM 查询
来源：http://ygl.fengsongda.top

document.querySelector(".item")
来源：http://syp.jqgufenzy.top

[U101] JS：classList 操作
来源：http://qrs.birdmap.top

el.classList.toggle("active")
来源：http://ony.vqdsnc.cn

[U102] JS：本地存储
来源：http://xtf.yongpay.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jts.tianlin.xyz

[U103] JS：定时器
来源：http://zmw.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tih.vehdjk.com

[U104] JS：防抖
来源：http://ajf.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aar.jyoumei.cn

[U105] JS：节流
来源：http://ypb.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hzv.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://dbn.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://niu.sxryk.cn

[U107] JS：数字千分位
来源：http://mky.hnxiangtu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kcf.cheryme.top

[U108] JS：随机整数
来源：http://jac.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://abw.yj20258888.top

[U109] JS：数组分组
来源：http://cql.cashguo.top

Object.groupBy(arr, x => x.type)
来源：http://gzz.fktsv.cn

[U110] JS：数组分块
来源：http://xic.jinqigfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mgp.yfazqb.com

[U111] JS：对象转 Map
来源：http://zwn.jinyuanbaomall.cn

new Map(Object.entries(obj))
来源：http://ndh.birdmap.top

[U112] JS：字符串补位
来源：http://hyl.bbcook.cn

"7".padStart(3, "0")
来源：http://sas.birdmap.top

[U113] JS：正则替换全部
来源：http://iuy.jinghuilouyu.cn

s.replaceAll("a", "b")
来源：http://iwb.ppjwa.cn

[U114] JS：JSON 深比较
来源：http://aps.quarkkingdee.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://usu.jinqigfzy.top

[U115] JS：生成 UUID
来源：http://vta.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://orm.dianchejie.cn

[U116] JS：类型检查（JSDoc）
来源：http://wiy.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://tge.daxiang520.top

[U117] JS：单元测试
来源：http://tmz.ybcxt.top

npm i -D vitest;  npx vitest
来源：http://fer.bbcook.cn

[U118] JS：开发服务器
来源：http://ugh.bbcook.cn

npm i -D vite;  npx vite
来源：http://ruj.dianchejie.cn


<!-- 参考信息 -->