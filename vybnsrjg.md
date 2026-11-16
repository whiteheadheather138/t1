代发 wailian999

[T31] Lua：Hello World
来源：http://whe.cdnleiting.top

print("Hello")
来源：http://sxt.52xcode.cn

[T32] Lua：局部变量
来源：http://jhp.gotoacloud.top

local a = 1
来源：http://gif.cheryme.top

[T33] Lua：表（数组）
来源：http://qhp.hammf.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ota.sysykeji.top

[T34] Lua：遍历表
来源：http://owv.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://okn.chenzaomai.com

[T35] Lua：字典表
来源：http://tkp.quarkkingdee.top

local d = { a = 1 };  d.b = 2
来源：http://ykm.shzxlz.cn

[T36] Lua：函数
来源：http://cfn.ydzc1.top

function add(a, b) return a + b end
来源：http://asl.cashguo.top

[T37] Lua：字符串拼接
来源：http://hxu.yonumen.top

"a" .. "b"
来源：http://ktc.zhengqikj.top

[T38] Lua：条件
来源：http://qik.yongpay.top

if x > 0 then print("正") end
来源：http://lfo.meibo888.top

[T39] Lua：模式匹配
来源：http://lnu.bjfxy.top

string.find(s, "%d+")
来源：http://vkv.xuanzx.com

[T40] Lua：元表
来源：http://fde.bbcook.cn

setmetatable({}, { __index = base })
来源：http://aku.zhaomingkeji.xyz

[T41] Perl：Hello World
来源：http://csx.smart0.xyz

print "Hello\n";
来源：http://axm.zhoulong.xyz

[T42] Perl：变量类型
来源：http://dmz.tianlin.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nrp.zdqjudy.top

[T43] Perl：字符串插值
来源：http://tig.iojbl.cn

"值: $a"
来源：http://vtg.ywan-chungtsiang.top

[T44] Perl：条件
来源：http://hjy.zhijiandao.cn

if ($a > 0) { print "正"; }
来源：http://wjv.nanxuanxn.top

[T45] Perl：数组遍历
来源：http://xtf.gzhubu.top

for my $x (@arr) { print $x; }
来源：http://ops.bjfxy.top

[T46] Perl：哈希操作
来源：http://hyc.uphjek.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eiv.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://bef.gotoacloud.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://nze.cashguo.top

[T48] Perl：正则替换
来源：http://skb.xingfuxueyuan.xyz

$s =~ s/old/new/g;
来源：http://ydq.cdnleiting.top

[T49] Perl：函数
来源：http://dwz.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://znw.316326.xyz

[T50] Perl：逐行读文件
来源：http://ihr.ehwqpu.com

open my $fh, "<", "a.txt" or die $!;
来源：http://bdd.9152youxi.cn

while (my $line = <$fh>) { print $line; }
来源：http://kcy.tianlin.xyz

[T51] Scala：Hello World
来源：http://anv.shuidangran.top

println("Hello")
来源：http://wxp.mhx1999.top

[T52] Scala：变量
来源：http://lbx.chenjidiqi.icu

val a = 1;  var b = 2
来源：http://heu.zhaomingkeji.xyz

[T53] Scala：字符串插值
来源：http://fjj.yongpay.top

s"值: $b"
来源：http://lhd.jianghu66.top

[T54] Scala：集合映射
来源：http://nxi.ydzc1.top

List(1, 2, 3).map(_ * 2)
来源：http://eam.sweek.top

[T55] Scala：集合过滤
来源：http://znc.hnxiangtu.top

List(1, 2, 3).filter(_ > 1)
来源：http://jus.nanxinkj.top

[T56] Scala：样例类
来源：http://esb.yj202588.top

case class User(name: String, age: Int)
来源：http://ebk.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://svq.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yjh.sysykeji.top

[T58] Scala：函数定义
来源：http://myq.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://klo.zhoulong.xyz

[T59] Scala：循环
来源：http://qri.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://jte.yonumen.top

[T60] Scala：折叠
来源：http://acp.bbcook.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://buv.0kj1m.cn

================================================================================
来源：http://toh.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pqh.pengpengdd.cyou

================================================================================
来源：http://wni.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://lzs.c1oappe.top

python -m venv .venv && source .venv/bin/activate
来源：http://flg.tianlin.xyz

[U02] Py：导出 / 安装依赖
来源：http://wjl.ctjpmb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dyx.wangdashe.top

[U03] Py：加载 .env 配置
来源：http://mcs.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kad.yueranfly.top

[U04] Py：变量调试打印
来源：http://tfa.jlsjyb.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rns.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://xgs.fktsv.cn

list(dict.fromkeys(arr))
来源：http://whb.nanxuanxn.top

[U06] Py：合并两个字典
来源：http://och.chenlongwang.top

{**a, **b}
来源：http://wyt.aibaodan.cn

[U07] Py：反转字典键值
来源：http://lfl.yongpay.top

{v: k for k, v in d.items()}
来源：http://zzj.hfpthk.cn

[U08] Py：展平二维列表
来源：http://oyb.sufxvd.cn

[y for x in nested for y in x]
来源：http://npo.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://qgv.yuanzhike.top

max(d, key=d.get)
来源：http://tud.feifeiyinyue.top

[U10] Py：按值排序字典
来源：http://vsh.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://afm.hesvh.cn

[U11] Py：生成器表达式
来源：http://jek.zycfv.cn

(x * 2 for x in arr)
来源：http://kpy.sjlbkw.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ubu.yanxiufei.cn

Counter(arr).most_common(3)
来源：http://lnu.ivvv.top

[U13] Py：固定长度队列
来源：http://npu.smart0.xyz

deque(maxlen=10)
来源：http://pso.svipenyu.cn

[U14] Py：分组收集到列表
来源：http://vxr.shangyingyoupin.top

defaultdict(list)
来源：http://kud.xuanzx.com

[U15] Py：高精度计时
来源：http://fta.aibaodan.cn

t = time.perf_counter()
来源：http://pga.zdqjudy.top

[U16] Py：命令行参数解析
来源：http://nyh.hesvh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kzv.pengpengdd.cyou

[U17] Py：初始化日志
来源：http://qbz.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://bfa.vqdsnc.cn

[U18] Py：预编译正则
来源：http://rqz.zhaomingkeji.xyz

pat = re.compile(r"\d+")
来源：http://bsf.sysykeji.top

[U19] Py：正则替换带回调
来源：http://mze.feifeiyinyue.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mng.mhx1999.top

[U20] Py：缓存函数结果
来源：http://qeh.fehbvm.com

@functools.lru_cache(maxsize=None)
来源：http://kjg.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://xdj.jinyuanbaomall.cn

@contextlib.contextmanager
来源：http://rjn.zhiwuduotai.top

[U22] Py：矩阵转置
来源：http://roy.xingfuxueyuan.xyz

list(zip(*m))
来源：http://yka.sufxvd.cn

[U23] Py：分块读取大文件
来源：http://jle.tianlin.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qoo.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://afo.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qso.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://xkf.jqgufenzy.top

csv.DictReader(f)
来源：http://eih.tarul.cn

[U26] Py：并发下载
来源：http://agb.xylfe.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://izl.hfpthk.cn

[U27] Py：异步 HTTP
来源：http://xtn.zhoulong.xyz

aiohttp.ClientSession() 配合 async with
来源：http://vpw.ehwqpu.com

[U28] Py：类型别名
来源：http://zov.hnqzz.top

UserId = int
来源：http://eby.ydjk.org.cn

[U29] Py：属性校验
来源：http://vsx.gotoacloud.top

@property 与 @x.setter 配合
来源：http://hgt.tianlin.xyz

[U30] Py：数据类
来源：http://eky.cashguo.top

@dataclass(slots=True)
来源：http://hkw.hywenlv.cn

[U31] Py：单测
来源：http://mlj.yonumen.top

python -m pytest -q
来源：http://wbe.gotoacloud.top

[U32] Py：代码格式化
来源：http://bzf.xinyue.icu

ruff format . && ruff check --fix .
来源：http://dbu.cqqwz.cn

[U33] Py：打包发布
来源：http://ilw.jiagoushi.top

python -m build  （依赖 pyproject.toml）
来源：http://bvh.tarul.cn

[U34] Py：判断编码
来源：http://bdx.c1oappe.top

chardet.detect(raw)
来源：http://rnq.chenzaomai.com

[U35] Py：发送邮件
来源：http://vxp.fanxiaobao.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://npk.jianghu66.top

[U36] Py：定时任务
来源：http://ixz.hysaishi.cn

schedule.every(10).minutes.do(job)
来源：http://ase.zdbjq.cn

[U37] Py：读写 Excel
来源：http://hrd.nanxinkj.top

pandas.read_excel / DataFrame.to_excel
来源：http://nha.ehwqpu.com

[U38] Py：获取脚本所在目录
来源：http://nxe.cqqwz.cn

Path(__file__).resolve().parent
来源：http://kes.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://sob.ivvv.top

sys.stdout.isatty()
来源：http://ctu.jinyuanbaomall.cn

[U40] Py：打印到标准错误
来源：http://aah.havefunace.top

print("err", file=sys.stderr)
来源：http://wfa.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://zjr.yongpay.top

composer init;  composer require guzzlehttp/guzzle
来源：http://kpg.zdqjudy.top

[U42] PHP：PSR-4 自动加载
来源：http://hew.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kvg.shzxlz.cn

[U43] PHP：声明命名空间
来源：http://qhs.yvedp.cn

namespace App\Http;
来源：http://xug.yonumen.top

[U44] PHP：开启严格类型
来源：http://sjt.ehwqpu.com

declare(strict_types=1);
来源：http://jal.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://acz.dianchejie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xpd.guannengcc.top

[U46] PHP：可空类型
来源：http://upq.kuanghao11.cn

?string $name = null
来源：http://xyd.daxiang520.top

[U47] PHP：联合类型
来源：http://xun.daria6918.cn

int|string $id
来源：http://rtc.zhixingplan.top

[U48] PHP：纯枚举
来源：http://wir.aizwys.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fie.sjlbkw.cn

[U49] PHP：只读属性
来源：http://zgo.xinyue.icu

public readonly string $name
来源：http://fzm.havefunace.top

[U50] PHP：构造器属性提升
来源：http://jsl.yj202588.top

public function __construct(private int $id) {}
来源：http://dkq.tarul.cn

[U51] PHP：数组解构
来源：http://qba.tanke756.top

[$a, $b] = $arr;
来源：http://uyz.zhaomingkeji.xyz

[U52] PHP：箭头函数
来源：http://gqg.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://xcx.xingfuxueyuan.xyz

[U53] PHP：空合并运算符
来源：http://uny.yuxming.cn

$v = $a ?? $b ?? "default";
来源：http://tcl.52xcode.cn

[U54] PHP：空安全调用
来源：http://puy.ppjwa.cn

$obj?->method()
来源：http://kxi.wangshuangyany.cn

[U55] PHP：match 表达式
来源：http://ohq.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hag.zhiwuduotai.top

[U56] PHP：命名参数
来源：http://nvb.xuetiantiany.cn

f(a: 1, b: 2)
来源：http://cqe.52xcode.cn

[U57] PHP：字符串插值
来源：http://gkg.ivvv.top

"值: {$a}"
来源：http://shr.sysykeji.top

[U58] PHP：数组三件套
来源：http://fhq.yj20258888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hhz.wangdashe.top

[U59] PHP：自定义排序
来源：http://zuq.cucudq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vca.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://mvr.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gzq.jlsjyb.cn

[U61] PHP：正则
来源：http://zmc.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tsn.yvedp.cn

[U62] PHP：日期对象
来源：http://bvv.mhx1999.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://szq.jinyuanbaomall.cn

[U63] PHP：文件读写
来源：http://szk.cashguo.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ctw.52xcode.cn

[U64] PHP：目录遍历
来源：http://cqm.haohaochexian.top

glob("dir/*.php");  scandir("dir");
来源：http://pwl.hysaishi.cn

[U65] PHP：会话
来源：http://fec.dianchejie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zji.wangdashe.top

[U66] PHP：设置 Cookie
来源：http://zcd.fktsv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lae.yanxiufei.cn

[U67] PHP：处理文件上传
来源：http://znc.wangdashe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dxf.dianchejie.cn

[U68] PHP：PDO 连接
来源：http://bhc.chenzaomai.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fan.hnxiangtu.top

[U69] PHP：PDO 预处理
来源：http://gei.vehdjk.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ric.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://ffx.hfpthk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dbt.316326.xyz

[U71] PHP：抛出异常
来源：http://dqm.chenzaomai.com

throw new RuntimeException("失败", 500);
来源：http://tfm.hnqzz.top

[U72] PHP：写错误日志
来源：http://dhv.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://gdm.zhixingplan.top

[U73] PHP：读取 ini 配置
来源：http://gdx.9152youxi.cn

parse_ini_file("config.ini", true)
来源：http://zom.aibaodan.cn

[U74] PHP：读取环境变量
来源：http://xvb.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://mfv.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://tym.zhijiandao.cn

composer require psr/container
来源：http://pui.fengsongda.top

[U76] PHP：简单路由
来源：http://gcq.jlsjyb.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oxk.shangyingyoupin.top

[U77] PHP：模板渲染
来源：http://cnb.snrcjt.cn

composer require twig/twig
来源：http://zwj.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://dvt.yuanzhike.top

composer require --dev phpunit/phpunit
来源：http://xfl.daxiang520.top

[U79] PHP：静态分析
来源：http://lmm.jinghuilouyu.cn

composer require --dev phpstan/phpstan
来源：http://kiw.jiagoushi.top

[U80] PHP：代码规范修复
来源：http://qnj.cqqwz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zun.iojbl.cn

[U81] JS：初始化项目
来源：http://iec.quarkkingdee.top

npm init -y;  npm i express
来源：http://mej.yangfankeji.com

[U82] JS：package.json 脚本
来源：http://xpa.tanke756.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://puh.zhaomingkeji.xyz

[U83] JS：ES Module 导入导出
来源：http://nrh.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://gcd.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://kvz.haohaochexian.top

module.exports = { a };  const { a } = require("./m");
来源：http://llx.hesvh.cn

[U85] JS：可选链
来源：http://bgs.xingfuxueyuan.xyz

a?.b?.c
来源：http://mhe.jianghu66.top

[U86] JS：空值合并
来源：http://mhb.yuanzhike.top

a ?? b
来源：http://kos.dianchejie.cn

[U87] JS：解构默认值
来源：http://gxm.zdbjq.cn

const { a = 1, b = 2 } = obj;
来源：http://irl.ydzc1.top

[U88] JS：对象展开合并
来源：http://plj.tarul.cn

{ ...a, ...b }
来源：http://urt.jqgfzy.top

[U89] JS：数组去重
来源：http://oyd.ppjwa.cn

[...new Set(arr)]
来源：http://xiy.meibo888.top

[U90] JS：数字数组排序
来源：http://xgz.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://tpn.yj20258888.top

[U91] JS：对象键值遍历
来源：http://nxd.fehbvm.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bjc.ehwqpu.com

[U92] JS：深拷贝
来源：http://ujl.cheryme.top

structuredClone(obj)
来源：http://sus.iojbl.cn

[U93] JS：模板字符串
来源：http://cue.c1oappe.top

`共 ${n} 条`
来源：http://rir.svipenyu.cn

[U94] JS：箭头函数
来源：http://rfo.snrcjt.cn

const double = x => x * 2;
来源：http://snx.yfazqb.com

[U95] JS：Promise 包装
来源：http://eyh.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://jwf.hammf.cn

[U96] JS：async/await 与异常
来源：http://eha.xinyue.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uuu.jiagoushi.top

[U97] JS：并发请求
来源：http://sls.shangyingyoupin.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zzp.yangfankeji.com

[U98] JS：fetch 带 JSON
来源：http://pug.cdnleiting.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vpq.jqgufenzy.top

[U99] JS：事件监听
来源：http://dyn.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://jdn.yj20258.top

[U100] JS：DOM 查询
来源：http://cwa.pycfn.com

document.querySelector(".item")
来源：http://ziv.nanxinkj.top

[U101] JS：classList 操作
来源：http://tpa.dashuyun.cn

el.classList.toggle("active")
来源：http://yqa.gaohongyu789.top

[U102] JS：本地存储
来源：http://hxq.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nwg.pycfn.com

[U103] JS：定时器
来源：http://dpy.hongshengwenyu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wyy.hcnkem.com

[U104] JS：防抖
来源：http://ibh.feifeiyinyue.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hqq.redwolf501.top

[U105] JS：节流
来源：http://rpc.zdqjudy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vvw.vqdsnc.cn

[U106] JS：日期格式化
来源：http://xjn.0kj1m.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tgx.epnwcf.com

[U107] JS：数字千分位
来源：http://rlf.daria6918.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gpc.chenjidiqi.icu

[U108] JS：随机整数
来源：http://qbo.ywan-chungtsiang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sdl.ehwqpu.com

[U109] JS：数组分组
来源：http://xee.wangdashe.top

Object.groupBy(arr, x => x.type)
来源：http://kyn.ydzc1.top

[U110] JS：数组分块
来源：http://xyh.feifeiyinyue.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ncu.ybcxt.top

[U111] JS：对象转 Map
来源：http://oml.redwolf501.top

new Map(Object.entries(obj))
来源：http://chy.smart0.xyz

[U112] JS：字符串补位
来源：http://evx.svipenyu.cn

"7".padStart(3, "0")
来源：http://jto.chenlongwang.top

[U113] JS：正则替换全部
来源：http://dmz.bbcook.cn

s.replaceAll("a", "b")
来源：http://ojs.snrcjt.cn

[U114] JS：JSON 深比较
来源：http://iqb.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jck.yj20258.top

[U115] JS：生成 UUID
来源：http://qdv.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://awa.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://tnf.zhoulong.xyz

/** @param {string} name */ function f(name) {}
来源：http://iqs.mhx1999.top

[U117] JS：单元测试
来源：http://cmy.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://pkx.gogol.net.cn

[U118] JS：开发服务器
来源：http://yao.zhaomingkeji.xyz

npm i -D vite;  npx vite
来源：http://ltp.yuanzhike.top


<!-- 参考信息 -->