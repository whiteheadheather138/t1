代发 wailian999

[T29] Swift：guard 提前返回
来源：http://fzx.52xcode.cn

guard let x = opt else { return }
来源：http://mrn.gogol.net.cn

[T30] Swift：协议
来源：http://eoa.svipenyu.cn

protocol Shape { func area() -> Double }
来源：http://oec.yangfankeji.com

[T31] Lua：Hello World
来源：http://wgz.haohaochexian.top

print("Hello")
来源：http://hyi.daxiang520.top

[T32] Lua：局部变量
来源：http://sfc.316326.xyz

local a = 1
来源：http://bav.bjfxy.top

[T33] Lua：表（数组）
来源：http://tsp.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://krz.nanxuanxn.top

[T34] Lua：遍历表
来源：http://unh.zdbjq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://chp.zdbjq.cn

[T35] Lua：字典表
来源：http://izj.shanyushiyangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://hhh.yueranfly.top

[T36] Lua：函数
来源：http://pde.zhoulong.xyz

function add(a, b) return a + b end
来源：http://wej.iojbl.cn

[T37] Lua：字符串拼接
来源：http://cbf.yvedp.cn

"a" .. "b"
来源：http://oxs.haohaochexian.top

[T38] Lua：条件
来源：http://hls.bjfxy.top

if x > 0 then print("正") end
来源：http://tdb.chenlongwang.top

[T39] Lua：模式匹配
来源：http://oks.zhongyouzk.top

string.find(s, "%d+")
来源：http://sdi.shzxlz.cn

[T40] Lua：元表
来源：http://mhn.zhixingplan.top

setmetatable({}, { __index = base })
来源：http://xln.quarkkingdee.top

[T41] Perl：Hello World
来源：http://hkt.jinyuanbaomall.cn

print "Hello\n";
来源：http://idh.yuanzhike.top

[T42] Perl：变量类型
来源：http://jnf.fktsv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kdu.jlsjyb.cn

[T43] Perl：字符串插值
来源：http://coo.redwolf501.top

"值: $a"
来源：http://axc.gaohongyu789.top

[T44] Perl：条件
来源：http://jfi.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://onl.zhengqikj.top

[T45] Perl：数组遍历
来源：http://pjw.zhaomingkeji.xyz

for my $x (@arr) { print $x; }
来源：http://rzm.zdbjq.cn

[T46] Perl：哈希操作
来源：http://ppc.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://euh.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://feg.yueranfly.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ykt.dianchejie.cn

[T48] Perl：正则替换
来源：http://xvt.svipenyu.cn

$s =~ s/old/new/g;
来源：http://wqy.yfazqb.com

[T49] Perl：函数
来源：http://lqe.jqgfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://noy.ywan-chungtsiang.top

[T50] Perl：逐行读文件
来源：http://rls.bbcook.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rjb.fktsv.cn

while (my $line = <$fh>) { print $line; }
来源：http://oov.aibaodan.cn

[T51] Scala：Hello World
来源：http://qah.gotoacloud.top

println("Hello")
来源：http://vif.fanxiaobao.xyz

[T52] Scala：变量
来源：http://yiv.mhx1999.top

val a = 1;  var b = 2
来源：http://vbj.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://spk.chenlongwang.top

s"值: $b"
来源：http://qxq.zhongyouzk.top

[T54] Scala：集合映射
来源：http://lyj.52xcode.cn

List(1, 2, 3).map(_ * 2)
来源：http://sbk.tianlin.xyz

[T55] Scala：集合过滤
来源：http://qkf.svipenyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kel.jlsjyb.cn

[T56] Scala：样例类
来源：http://iqt.zdqjudy.top

case class User(name: String, age: Int)
来源：http://pio.ydzc1.top

[T57] Scala：模式匹配
来源：http://eqm.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zfk.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://pxs.fengsongda.top

def add(a: Int, b: Int): Int = a + b
来源：http://soc.hywenlv.cn

[T59] Scala：循环
来源：http://nvz.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://yhu.ppjwa.cn

[T60] Scala：折叠
来源：http://iur.xuanzx.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fey.ivvv.top

================================================================================
来源：http://qqg.cheryme.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fkx.guannengcc.top

================================================================================
来源：http://hvd.xinyue.icu

[U01] Py：创建虚拟环境
来源：http://tai.zhiwuduotai.top

python -m venv .venv && source .venv/bin/activate
来源：http://yww.vqdsnc.cn

[U02] Py：导出 / 安装依赖
来源：http://xdu.mhx1999.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://isi.hnqzz.top

[U03] Py：加载 .env 配置
来源：http://qhb.yuanzhike.top

from dotenv import load_dotenv; load_dotenv()
来源：http://soe.yangfankeji.com

[U04] Py：变量调试打印
来源：http://eza.hammf.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vxl.tanke756.top

[U05] Py：列表去重且保序
来源：http://kfu.xziqi.cn

list(dict.fromkeys(arr))
来源：http://zaz.ydzc1.top

[U06] Py：合并两个字典
来源：http://cut.guannengcc.top

{**a, **b}
来源：http://qsg.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://xjd.daria6918.cn

{v: k for k, v in d.items()}
来源：http://cjx.yueranfly.top

[U08] Py：展平二维列表
来源：http://ohl.nanxuanxn.top

[y for x in nested for y in x]
来源：http://qrl.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://pbb.gogol.net.cn

max(d, key=d.get)
来源：http://cac.zhengqikj.top

[U10] Py：按值排序字典
来源：http://nxg.iojbl.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jer.tianlin.xyz

[U11] Py：生成器表达式
来源：http://ftr.hnxiangtu.top

(x * 2 for x in arr)
来源：http://bsq.yj20258.top

[U12] Py：取出现最多的 3 个元素
来源：http://hwd.sufxvd.cn

Counter(arr).most_common(3)
来源：http://eve.ctjpmb.com

[U13] Py：固定长度队列
来源：http://gka.meibo888.top

deque(maxlen=10)
来源：http://kzb.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://pxa.jiagoushi.top

defaultdict(list)
来源：http://uzd.gogol.net.cn

[U15] Py：高精度计时
来源：http://ycp.gotoacloud.top

t = time.perf_counter()
来源：http://wfr.c1oappe.top

[U16] Py：命令行参数解析
来源：http://uzj.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://inl.fehbvm.com

[U17] Py：初始化日志
来源：http://pnl.zdqjudy.top

logging.basicConfig(level=logging.INFO)
来源：http://jaz.hfpthk.cn

[U18] Py：预编译正则
来源：http://ldm.316326.xyz

pat = re.compile(r"\d+")
来源：http://gdq.shzxlz.cn

[U19] Py：正则替换带回调
来源：http://pdk.yuxming.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://opa.havefunace.top

[U20] Py：缓存函数结果
来源：http://gyv.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://rhg.hnqzz.top

[U21] Py：自定义上下文管理器
来源：http://khj.cdnleiting.top

@contextlib.contextmanager
来源：http://ksz.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://wfy.jianghu66.top

list(zip(*m))
来源：http://nlk.jqgufenzy.top

[U23] Py：分块读取大文件
来源：http://jdj.ehwqpu.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cyr.feifeiyinyue.top

[U24] Py：路径操作
来源：http://hlo.nanxinkj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vjn.xylfe.cn

[U25] Py：CSV 按字典读
来源：http://bcg.shanyushiyangkeji.top

csv.DictReader(f)
来源：http://ypz.c1oappe.top

[U26] Py：并发下载
来源：http://sot.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ktf.tian-w.cn

[U27] Py：异步 HTTP
来源：http://aqj.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://ijn.zhongyouzk.top

[U28] Py：类型别名
来源：http://lky.jinghuilouyu.cn

UserId = int
来源：http://vbu.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://oio.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://qgs.wangshuangyany.cn

[U30] Py：数据类
来源：http://ocr.aizwys.cn

@dataclass(slots=True)
来源：http://azv.xziqi.cn

[U31] Py：单测
来源：http://gah.cashguo.top

python -m pytest -q
来源：http://ihd.zdbjq.cn

[U32] Py：代码格式化
来源：http://hdj.tarul.cn

ruff format . && ruff check --fix .
来源：http://rdc.hesvh.cn

[U33] Py：打包发布
来源：http://bbc.hnxiangtu.top

python -m build  （依赖 pyproject.toml）
来源：http://qlf.yj20258.top

[U34] Py：判断编码
来源：http://ssm.xziqi.cn

chardet.detect(raw)
来源：http://jdu.yvedp.cn

[U35] Py：发送邮件
来源：http://ksr.vehdjk.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kdg.jianghu66.top

[U36] Py：定时任务
来源：http://ahk.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://peo.zhixingplan.top

[U37] Py：读写 Excel
来源：http://lha.wangdashe.top

pandas.read_excel / DataFrame.to_excel
来源：http://wit.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://nyd.snrcjt.cn

Path(__file__).resolve().parent
来源：http://yek.jinqigfzy.top

[U39] Py：判断是否在交互环境
来源：http://btw.jqgfzy.top

sys.stdout.isatty()
来源：http://ypm.hcnkem.com

[U40] Py：打印到标准错误
来源：http://smq.jianghu66.top

print("err", file=sys.stderr)
来源：http://tfr.yuxming.cn

[U41] PHP：初始化 Composer 项目
来源：http://iry.cashguo.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ggt.haohaochexian.top

[U42] PHP：PSR-4 自动加载
来源：http://lol.quarkkingdee.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tpm.gotoacloud.top

[U43] PHP：声明命名空间
来源：http://drq.dashuyun.cn

namespace App\Http;
来源：http://lko.xingfuxueyuan.xyz

[U44] PHP：开启严格类型
来源：http://gxb.cqqwz.cn

declare(strict_types=1);
来源：http://rei.gaohongyu789.top

[U45] PHP：类型声明与返回类型
来源：http://lzq.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://ype.hcnkem.com

[U46] PHP：可空类型
来源：http://mni.sysykeji.top

?string $name = null
来源：http://bro.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://dtt.sysykeji.top

int|string $id
来源：http://ylc.tianlin.xyz

[U48] PHP：纯枚举
来源：http://vxb.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kuz.kuanghao11.cn

[U49] PHP：只读属性
来源：http://qpp.chenzaomai.com

public readonly string $name
来源：http://rkl.birdmap.top

[U50] PHP：构造器属性提升
来源：http://zcu.9152youxi.cn

public function __construct(private int $id) {}
来源：http://iwn.pycfn.com

[U51] PHP：数组解构
来源：http://azs.yj202588.top

[$a, $b] = $arr;
来源：http://wfz.ywan-chungtsiang.top

[U52] PHP：箭头函数
来源：http://udf.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://byz.epnwcf.com

[U53] PHP：空合并运算符
来源：http://mlo.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://uli.mhx1999.top

[U54] PHP：空安全调用
来源：http://qvb.jqgufenzy.top

$obj?->method()
来源：http://zxe.ybcxt.top

[U55] PHP：match 表达式
来源：http://txt.yonumen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lna.haohaochexian.top

[U56] PHP：命名参数
来源：http://pkw.xinyue.icu

f(a: 1, b: 2)
来源：http://bhd.fengsongda.top

[U57] PHP：字符串插值
来源：http://una.dianchejie.cn

"值: {$a}"
来源：http://glr.shuidangran.top

[U58] PHP：数组三件套
来源：http://cur.xziqi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ogb.tanke756.top

[U59] PHP：自定义排序
来源：http://ygs.cashguo.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nnd.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://tje.daxiang520.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lzo.smart0.xyz

[U61] PHP：正则
来源：http://eao.havefunace.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://use.mhx1999.top

[U62] PHP：日期对象
来源：http://wmd.daria6918.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://keb.yvedp.cn

[U63] PHP：文件读写
来源：http://bcl.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ssq.xylfe.cn

[U64] PHP：目录遍历
来源：http://lse.snrcjt.cn

glob("dir/*.php");  scandir("dir");
来源：http://fxo.hongshengwenyu.top

[U65] PHP：会话
来源：http://vzz.yangfankeji.com

session_start();  $_SESSION["uid"] = 1;
来源：http://pmx.cucudq.cn

[U66] PHP：设置 Cookie
来源：http://kty.zhijiandao.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gie.316326.xyz

[U67] PHP：处理文件上传
来源：http://iqm.aibaodan.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ixy.yj202588.top

[U68] PHP：PDO 连接
来源：http://whd.ywan-chungtsiang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ahz.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://ihn.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uoo.vehdjk.com

[U70] PHP：PDO 事务
来源：http://qhl.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pfn.hnqzz.top

[U71] PHP：抛出异常
来源：http://hfd.zycfv.cn

throw new RuntimeException("失败", 500);
来源：http://oxd.hnxiangtu.top

[U72] PHP：写错误日志
来源：http://ozc.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://zhx.shanyushiyangkeji.top

[U73] PHP：读取 ini 配置
来源：http://wql.cashguo.top

parse_ini_file("config.ini", true)
来源：http://bxm.zhixingplan.top

[U74] PHP：读取环境变量
来源：http://bqp.chenjidiqi.icu

getenv("APP_ENV") ?: "production"
来源：http://chx.zdqjudy.top

[U75] PHP：依赖注入
来源：http://viv.xziqi.cn

composer require psr/container
来源：http://xcs.zhoulong.xyz

[U76] PHP：简单路由
来源：http://olf.yangfankeji.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ewt.fzhhl.top

[U77] PHP：模板渲染
来源：http://vws.shanyushiyangtech.top

composer require twig/twig
来源：http://jju.ppjwa.cn

[U78] PHP：单元测试
来源：http://rzg.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://eyn.haohaochexian.top

[U79] PHP：静态分析
来源：http://oti.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://efq.snrcjt.cn

[U80] PHP：代码规范修复
来源：http://gfk.jinghuilouyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wip.tian-w.cn

[U81] JS：初始化项目
来源：http://scu.daxiang520.top

npm init -y;  npm i express
来源：http://ipa.quarkkingdee.top

[U82] JS：package.json 脚本
来源：http://nib.bjfxy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vzn.yj20258.top

[U83] JS：ES Module 导入导出
来源：http://hoh.yj20258888.top

export const a = 1;  import { a } from "./m.js";
来源：http://zfh.gaohongyu789.top

[U84] JS：CommonJS 写法
来源：http://drq.cashguo.top

module.exports = { a };  const { a } = require("./m");
来源：http://gkj.bjfxy.top

[U85] JS：可选链
来源：http://zuk.nanxinkj.top

a?.b?.c
来源：http://nkr.guowangkeji.top

[U86] JS：空值合并
来源：http://cte.guannengcc.top

a ?? b
来源：http://dky.nwbrower.top

[U87] JS：解构默认值
来源：http://rjb.fengsongda.top

const { a = 1, b = 2 } = obj;
来源：http://flx.dianchejie.cn

[U88] JS：对象展开合并
来源：http://ehm.shuidangran.top

{ ...a, ...b }
来源：http://pds.smart0.xyz

[U89] JS：数组去重
来源：http://rxg.aibaodan.cn

[...new Set(arr)]
来源：http://csv.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://ulv.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://usg.fengsongda.top

[U91] JS：对象键值遍历
来源：http://zwh.yangfankeji.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nzy.svipenyu.cn

[U92] JS：深拷贝
来源：http://mch.chenzaomai.com

structuredClone(obj)
来源：http://qve.zhongyouzk.top

[U93] JS：模板字符串
来源：http://xvo.vqdsnc.cn

`共 ${n} 条`
来源：http://rma.jiagoushi.top

[U94] JS：箭头函数
来源：http://rvv.yuxming.cn

const double = x => x * 2;
来源：http://icv.svipenyu.cn

[U95] JS：Promise 包装
来源：http://xpc.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://mrr.hammf.cn

[U96] JS：async/await 与异常
来源：http://tuf.zdbjq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ejb.zhoulong.xyz

[U97] JS：并发请求
来源：http://wuf.wangdashe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vou.smart0.xyz

[U98] JS：fetch 带 JSON
来源：http://qey.xinyue.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jti.andypj.xyz

[U99] JS：事件监听
来源：http://lqc.316326.xyz

el.addEventListener("click", e => {})
来源：http://thf.cashguo.top

[U100] JS：DOM 查询
来源：http://ljw.xingfuxueyuan.xyz

document.querySelector(".item")
来源：http://bav.zhijiandao.cn

[U101] JS：classList 操作
来源：http://www.yj202588.top

el.classList.toggle("active")
来源：http://odl.bjfxy.top

[U102] JS：本地存储
来源：http://qwb.daria6918.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mtv.quarkkingdee.top

[U103] JS：定时器
来源：http://ame.tanke756.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://akt.sjlbkw.cn

[U104] JS：防抖
来源：http://wta.jlsjyb.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://snv.ydjk.org.cn

[U105] JS：节流
来源：http://nfu.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bko.cdnleiting.top

[U106] JS：日期格式化
来源：http://jbd.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dbb.hnqzz.top

[U107] JS：数字千分位
来源：http://uzo.snrcjt.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rvp.zdqjudy.top

[U108] JS：随机整数
来源：http://ygx.zhengqikj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pby.chenlongwang.top

[U109] JS：数组分组
来源：http://izr.uphjek.com

Object.groupBy(arr, x => x.type)
来源：http://cqr.dianchejie.cn

[U110] JS：数组分块
来源：http://vgs.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yoe.fktsv.cn

[U111] JS：对象转 Map
来源：http://zgc.jinqigufen.top

new Map(Object.entries(obj))
来源：http://bhe.9152youxi.cn

[U112] JS：字符串补位
来源：http://nvn.316326.xyz

"7".padStart(3, "0")
来源：http://syv.aibaodan.cn

[U113] JS：正则替换全部
来源：http://lde.xinyue.icu

s.replaceAll("a", "b")
来源：http://nsh.hnqzz.top

[U114] JS：JSON 深比较
来源：http://mwc.cashguo.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gha.jiagoushi.top

[U115] JS：生成 UUID
来源：http://phh.zhaomingkeji.xyz

crypto.randomUUID()
来源：http://cfk.jianghu66.top

[U116] JS：类型检查（JSDoc）
来源：http://itk.jlsjyb.cn

/** @param {string} name */ function f(name) {}
来源：http://skv.jinghuilouyu.cn


<!-- 参考信息 -->