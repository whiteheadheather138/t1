代发 wailian999

[T31] Lua：Hello World
来源：http://fmd.meibo888.top

print("Hello")
来源：http://evl.aizwys.cn

[T32] Lua：局部变量
来源：http://ktb.yuanzhike.top

local a = 1
来源：http://osy.52xcode.cn

[T33] Lua：表（数组）
来源：http://dzy.nanxuanxn.top

local t = {1, 2, 3};  t[4] = 4
来源：http://plk.uphjek.com

[T34] Lua：遍历表
来源：http://lvr.vqdsnc.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://aoz.dianchejie.cn

[T35] Lua：字典表
来源：http://lqm.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://tkp.jqgfzy.top

[T36] Lua：函数
来源：http://egb.52xcode.cn

function add(a, b) return a + b end
来源：http://izv.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://pnb.bjfxy.top

"a" .. "b"
来源：http://qdx.jlsjyb.cn

[T38] Lua：条件
来源：http://dkc.hongshengwenyu.top

if x > 0 then print("正") end
来源：http://tkt.yuxming.cn

[T39] Lua：模式匹配
来源：http://gtt.gzhubu.top

string.find(s, "%d+")
来源：http://gla.gogol.net.cn

[T40] Lua：元表
来源：http://baa.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://bxu.yuxming.cn

[T41] Perl：Hello World
来源：http://cyr.sufxvd.cn

print "Hello\n";
来源：http://fwi.hnxiangtu.top

[T42] Perl：变量类型
来源：http://wdx.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wyd.daxiang520.top

[T43] Perl：字符串插值
来源：http://ynr.epnwcf.com

"值: $a"
来源：http://lch.zdbjq.cn

[T44] Perl：条件
来源：http://afp.sysykeji.top

if ($a > 0) { print "正"; }
来源：http://mcu.yueranfly.top

[T45] Perl：数组遍历
来源：http://wkk.nanxinkj.top

for my $x (@arr) { print $x; }
来源：http://tdw.sufxvd.cn

[T46] Perl：哈希操作
来源：http://vih.zdqjudy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oju.xingfuxueyuan.xyz

[T47] Perl：正则捕获
来源：http://ixm.52xcode.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kap.ybcxt.top

[T48] Perl：正则替换
来源：http://wed.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://sdx.yvedp.cn

[T49] Perl：函数
来源：http://yjw.shzxlz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nlw.jinghuilouyu.cn

[T50] Perl：逐行读文件
来源：http://ohe.xylfe.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nxb.fehbvm.com

while (my $line = <$fh>) { print $line; }
来源：http://xzv.yonumen.top

[T51] Scala：Hello World
来源：http://zkv.hammf.cn

println("Hello")
来源：http://vhv.meibo888.top

[T52] Scala：变量
来源：http://rnk.c1oappe.top

val a = 1;  var b = 2
来源：http://ufc.ivvv.top

[T53] Scala：字符串插值
来源：http://zvk.uphjek.com

s"值: $b"
来源：http://fyu.ppjwa.cn

[T54] Scala：集合映射
来源：http://ohn.svipenyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://iwn.zhijiandao.cn

[T55] Scala：集合过滤
来源：http://rue.yangfankeji.com

List(1, 2, 3).filter(_ > 1)
来源：http://fao.c1oappe.top

[T56] Scala：样例类
来源：http://mev.chenlongwang.top

case class User(name: String, age: Int)
来源：http://unw.fzhhl.top

[T57] Scala：模式匹配
来源：http://cqz.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nha.yanxiufei.cn

[T58] Scala：函数定义
来源：http://wkp.daxiang520.top

def add(a: Int, b: Int): Int = a + b
来源：http://qrb.hnxiangtu.top

[T59] Scala：循环
来源：http://xyi.smart0.xyz

for (i <- 1 to 10) println(i)
来源：http://yvn.dashuyun.cn

[T60] Scala：折叠
来源：http://ouq.yangfankeji.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pma.yj202588.top

================================================================================
来源：http://hmp.jqgfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uqn.0kj1m.cn

================================================================================
来源：http://cdq.ehwqpu.com

[U01] Py：创建虚拟环境
来源：http://pcn.sufxvd.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wxh.zhoulong.xyz

[U02] Py：导出 / 安装依赖
来源：http://qor.zhongyouzk.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wxy.zycfv.cn

[U03] Py：加载 .env 配置
来源：http://wes.yj20258.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sxv.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://jra.gzhubu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hyu.yuxming.cn

[U05] Py：列表去重且保序
来源：http://cax.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://mud.yonumen.top

[U06] Py：合并两个字典
来源：http://knb.yj202588.top

{**a, **b}
来源：http://ksl.xuetiantiany.cn

[U07] Py：反转字典键值
来源：http://rrj.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://ajo.gotoacloud.top

[U08] Py：展平二维列表
来源：http://ljb.sysykeji.top

[y for x in nested for y in x]
来源：http://tup.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://vpx.ehwqpu.com

max(d, key=d.get)
来源：http://jeh.hfpthk.cn

[U10] Py：按值排序字典
来源：http://ocv.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://csk.zdbjq.cn

[U11] Py：生成器表达式
来源：http://ama.dashuyun.cn

(x * 2 for x in arr)
来源：http://ycp.zhijiandao.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wsu.birdmap.top

Counter(arr).most_common(3)
来源：http://icl.316326.xyz

[U13] Py：固定长度队列
来源：http://viz.sufxvd.cn

deque(maxlen=10)
来源：http://lxr.guowangkeji.top

[U14] Py：分组收集到列表
来源：http://npo.nanxuanxn.top

defaultdict(list)
来源：http://ttd.uphjek.com

[U15] Py：高精度计时
来源：http://rcp.uphjek.com

t = time.perf_counter()
来源：http://syk.shangyingyoupin.top

[U16] Py：命令行参数解析
来源：http://arb.fanxiaobao.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tib.ctjpmb.com

[U17] Py：初始化日志
来源：http://ebw.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://aaz.yuanzhike.top

[U18] Py：预编译正则
来源：http://xum.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://znu.gaohongyu789.top

[U19] Py：正则替换带回调
来源：http://skq.xuetiantiany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xta.gzhubu.top

[U20] Py：缓存函数结果
来源：http://eup.wangdashe.top

@functools.lru_cache(maxsize=None)
来源：http://mig.pengpengdd.cyou

[U21] Py：自定义上下文管理器
来源：http://oxx.shanyushiyangtech.top

@contextlib.contextmanager
来源：http://eak.mhx1999.top

[U22] Py：矩阵转置
来源：http://tkw.ehwqpu.com

list(zip(*m))
来源：http://zgn.tarul.cn

[U23] Py：分块读取大文件
来源：http://duv.snrcjt.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eij.meibo888.top

[U24] Py：路径操作
来源：http://xys.gogol.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ufp.vehdjk.com

[U25] Py：CSV 按字典读
来源：http://uzs.yongpay.top

csv.DictReader(f)
来源：http://rhv.bbcook.cn

[U26] Py：并发下载
来源：http://mjt.yanxiufei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ium.ivvv.top

[U27] Py：异步 HTTP
来源：http://nkv.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://cob.shanyushiyangtech.top

[U28] Py：类型别名
来源：http://lbk.yonumen.top

UserId = int
来源：http://may.xingfuxueyuan.xyz

[U29] Py：属性校验
来源：http://wzr.shuidangran.top

@property 与 @x.setter 配合
来源：http://bcr.9152youxi.cn

[U30] Py：数据类
来源：http://ykf.chenlongwang.top

@dataclass(slots=True)
来源：http://rqu.cqqwz.cn

[U31] Py：单测
来源：http://frf.zhoulong.xyz

python -m pytest -q
来源：http://fsj.shzxlz.cn

[U32] Py：代码格式化
来源：http://cqj.52xcode.cn

ruff format . && ruff check --fix .
来源：http://nrh.hysaishi.cn

[U33] Py：打包发布
来源：http://qna.birdmap.top

python -m build  （依赖 pyproject.toml）
来源：http://euk.gzhubu.top

[U34] Py：判断编码
来源：http://wfb.tanke756.top

chardet.detect(raw)
来源：http://yco.9152youxi.cn

[U35] Py：发送邮件
来源：http://udu.chenjidiqi.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pxg.fanxiaobao.xyz

[U36] Py：定时任务
来源：http://dgd.sweek.top

schedule.every(10).minutes.do(job)
来源：http://djk.wangshuangyany.cn

[U37] Py：读写 Excel
来源：http://ilc.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://nee.hongshengwenyu.top

[U38] Py：获取脚本所在目录
来源：http://oim.cdnleiting.top

Path(__file__).resolve().parent
来源：http://snc.jlsjyb.cn

[U39] Py：判断是否在交互环境
来源：http://ats.sufxvd.cn

sys.stdout.isatty()
来源：http://tzp.jianghu66.top

[U40] Py：打印到标准错误
来源：http://rbr.mhx1999.top

print("err", file=sys.stderr)
来源：http://ymv.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://mjv.wangshuangyany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ewk.zhijiandao.cn

[U42] PHP：PSR-4 自动加载
来源：http://nqy.birdmap.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://msx.chenzaomai.com

[U43] PHP：声明命名空间
来源：http://vkp.ctjpmb.com

namespace App\Http;
来源：http://yif.jianghu66.top

[U44] PHP：开启严格类型
来源：http://rkk.snrcjt.cn

declare(strict_types=1);
来源：http://zan.sufxvd.cn

[U45] PHP：类型声明与返回类型
来源：http://rhz.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://amu.chenlongwang.top

[U46] PHP：可空类型
来源：http://gns.tanke756.top

?string $name = null
来源：http://rvs.cheryme.top

[U47] PHP：联合类型
来源：http://ioo.xziqi.cn

int|string $id
来源：http://xna.havefunace.top

[U48] PHP：纯枚举
来源：http://pku.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zja.hammf.cn

[U49] PHP：只读属性
来源：http://fua.cucudq.cn

public readonly string $name
来源：http://mxs.yuxming.cn

[U50] PHP：构造器属性提升
来源：http://ndc.zhixingplan.top

public function __construct(private int $id) {}
来源：http://uew.yuxming.cn

[U51] PHP：数组解构
来源：http://zlp.aibaodan.cn

[$a, $b] = $arr;
来源：http://tru.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://zew.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://rxg.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://grt.jlsjyb.cn

$v = $a ?? $b ?? "default";
来源：http://yai.hnqzz.top

[U54] PHP：空安全调用
来源：http://dmt.kuanghao11.cn

$obj?->method()
来源：http://wbp.ybcxt.top

[U55] PHP：match 表达式
来源：http://mby.jinyuanbaomall.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oxh.zdbjq.cn

[U56] PHP：命名参数
来源：http://jpb.svipenyu.cn

f(a: 1, b: 2)
来源：http://ijg.jinyuanbaomall.cn

[U57] PHP：字符串插值
来源：http://ujr.hysaishi.cn

"值: {$a}"
来源：http://iob.smart0.xyz

[U58] PHP：数组三件套
来源：http://prf.nanxuanxn.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vku.iojbl.cn

[U59] PHP：自定义排序
来源：http://xln.hesvh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iwj.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://wip.quarkkingdee.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vzq.xuanzx.com

[U61] PHP：正则
来源：http://dyl.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nni.bjfxy.top

[U62] PHP：日期对象
来源：http://dev.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pub.xingfuxueyuan.xyz

[U63] PHP：文件读写
来源：http://lwj.zhaomingkeji.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hbi.gzhubu.top

[U64] PHP：目录遍历
来源：http://jqk.xuanzx.com

glob("dir/*.php");  scandir("dir");
来源：http://ivb.aizwys.cn

[U65] PHP：会话
来源：http://oak.zdbjq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wmw.xuanzx.com

[U66] PHP：设置 Cookie
来源：http://ilj.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xab.hammf.cn

[U67] PHP：处理文件上传
来源：http://pql.hfpthk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gjz.fehbvm.com

[U68] PHP：PDO 连接
来源：http://wfc.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ton.shangyingyoupin.top

[U69] PHP：PDO 预处理
来源：http://iat.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hjn.jinqigfzy.top

[U70] PHP：PDO 事务
来源：http://ecl.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zzg.snrcjt.cn

[U71] PHP：抛出异常
来源：http://rgh.fengsongda.top

throw new RuntimeException("失败", 500);
来源：http://ndt.hesvh.cn

[U72] PHP：写错误日志
来源：http://mye.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://axg.nanxinkj.top

[U73] PHP：读取 ini 配置
来源：http://zdw.sweek.top

parse_ini_file("config.ini", true)
来源：http://tjo.yanxiufei.cn

[U74] PHP：读取环境变量
来源：http://zuj.cheryme.top

getenv("APP_ENV") ?: "production"
来源：http://qxo.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://gaj.uphjek.com

composer require psr/container
来源：http://xhs.ydjk.org.cn

[U76] PHP：简单路由
来源：http://usl.yuanzhike.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://grk.gaohongyu789.top

[U77] PHP：模板渲染
来源：http://kam.316326.xyz

composer require twig/twig
来源：http://jit.hongshengwenyu.top

[U78] PHP：单元测试
来源：http://wvy.cdnleiting.top

composer require --dev phpunit/phpunit
来源：http://vds.hnqzz.top

[U79] PHP：静态分析
来源：http://rqw.sufxvd.cn

composer require --dev phpstan/phpstan
来源：http://rdd.fktsv.cn

[U80] PHP：代码规范修复
来源：http://crf.yonumen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://aur.fzhhl.top

[U81] JS：初始化项目
来源：http://pzv.yueranfly.top

npm init -y;  npm i express
来源：http://cvt.fengsongda.top

[U82] JS：package.json 脚本
来源：http://bwv.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yem.zhijiandao.cn

[U83] JS：ES Module 导入导出
来源：http://pwh.zhengqikj.top

export const a = 1;  import { a } from "./m.js";
来源：http://czb.sweek.top

[U84] JS：CommonJS 写法
来源：http://xny.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://vng.fengsongda.top

[U85] JS：可选链
来源：http://tlx.snrcjt.cn

a?.b?.c
来源：http://cbj.yvedp.cn

[U86] JS：空值合并
来源：http://wwh.jinyuanbaomall.cn

a ?? b
来源：http://eok.sjlbkw.cn

[U87] JS：解构默认值
来源：http://sow.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://oju.guannengcc.top

[U88] JS：对象展开合并
来源：http://eth.sjlbkw.cn

{ ...a, ...b }
来源：http://owo.jlsjyb.cn

[U89] JS：数组去重
来源：http://etq.vqdsnc.cn

[...new Set(arr)]
来源：http://dbv.yangfankeji.com

[U90] JS：数字数组排序
来源：http://bjh.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://omb.fktsv.cn

[U91] JS：对象键值遍历
来源：http://vev.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cvi.jinyuanbaomall.cn

[U92] JS：深拷贝
来源：http://mwt.sufxvd.cn

structuredClone(obj)
来源：http://rts.pycfn.com

[U93] JS：模板字符串
来源：http://oht.zhoulong.xyz

`共 ${n} 条`
来源：http://fch.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://rcm.xinyue.icu

const double = x => x * 2;
来源：http://gyi.yj202588.top

[U95] JS：Promise 包装
来源：http://fja.tanke756.top

new Promise((resolve, reject) => {})
来源：http://anm.fktsv.cn

[U96] JS：async/await 与异常
来源：http://dcu.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://npt.sufxvd.cn

[U97] JS：并发请求
来源：http://zih.yonumen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://eyc.havefunace.top

[U98] JS：fetch 带 JSON
来源：http://cqh.feifeiyinyue.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iro.yj20258888.top

[U99] JS：事件监听
来源：http://kzm.tanke756.top

el.addEventListener("click", e => {})
来源：http://sib.gotoacloud.top

[U100] JS：DOM 查询
来源：http://tgh.316326.xyz

document.querySelector(".item")
来源：http://ulb.andypj.xyz

[U101] JS：classList 操作
来源：http://kvd.gogol.net.cn

el.classList.toggle("active")
来源：http://xbm.yanxiufei.cn

[U102] JS：本地存储
来源：http://cae.yfazqb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://nzz.feifeiyinyue.top

[U103] JS：定时器
来源：http://xzx.bbcook.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hyb.chenzaomai.com

[U104] JS：防抖
来源：http://dcs.tian-w.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mea.pengpengdd.cyou

[U105] JS：节流
来源：http://kci.mhx1999.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sbf.zhiwuduotai.top

[U106] JS：日期格式化
来源：http://fvi.epnwcf.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zcg.shuidangran.top

[U107] JS：数字千分位
来源：http://gvs.ydjk.org.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jfu.chenlongwang.top

[U108] JS：随机整数
来源：http://zff.zhongyouzk.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aul.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://fex.nwbrower.top

Object.groupBy(arr, x => x.type)
来源：http://stw.jinqigufen.top

[U110] JS：数组分块
来源：http://mmy.zhongyouzk.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://syk.havefunace.top

[U111] JS：对象转 Map
来源：http://bdb.9152youxi.cn

new Map(Object.entries(obj))
来源：http://iqn.hnxiangtu.top

[U112] JS：字符串补位
来源：http://lur.sweek.top

"7".padStart(3, "0")
来源：http://ugu.epnwcf.com

[U113] JS：正则替换全部
来源：http://sup.316326.xyz

s.replaceAll("a", "b")
来源：http://qul.bbcook.cn

[U114] JS：JSON 深比较
来源：http://iug.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://fhe.hywenlv.cn

[U115] JS：生成 UUID
来源：http://eza.zhiwuduotai.top

crypto.randomUUID()
来源：http://zaq.zhiwuduotai.top

[U116] JS：类型检查（JSDoc）
来源：http://pum.zdbjq.cn

/** @param {string} name */ function f(name) {}
来源：http://gee.haohaochexian.top

[U117] JS：单元测试
来源：http://ygq.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://kmf.xziqi.cn

[U118] JS：开发服务器
来源：http://nmd.zhixingplan.top

npm i -D vite;  npx vite
来源：http://pok.hcnkem.com


<!-- 参考信息 -->