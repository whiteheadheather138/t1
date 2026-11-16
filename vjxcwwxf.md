代发 wailian999

[T37] Lua：字符串拼接
来源：http://xiw.tarul.cn

"a" .. "b"
来源：http://kgu.bjfxy.top

[T38] Lua：条件
来源：http://mxw.hywenlv.cn

if x > 0 then print("正") end
来源：http://rnw.epnwcf.com

[T39] Lua：模式匹配
来源：http://xkm.shangyingyoupin.top

string.find(s, "%d+")
来源：http://bxy.yuanzhike.top

[T40] Lua：元表
来源：http://qte.cashguo.top

setmetatable({}, { __index = base })
来源：http://bzk.xinyue.icu

[T41] Perl：Hello World
来源：http://jai.ppjwa.cn

print "Hello\n";
来源：http://qvv.pycfn.com

[T42] Perl：变量类型
来源：http://jvn.tianlin.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vus.hywenlv.cn

[T43] Perl：字符串插值
来源：http://obw.chenlongwang.top

"值: $a"
来源：http://wyg.pycfn.com

[T44] Perl：条件
来源：http://mfa.yfazqb.com

if ($a > 0) { print "正"; }
来源：http://oym.hnqzz.top

[T45] Perl：数组遍历
来源：http://wvd.daxiang520.top

for my $x (@arr) { print $x; }
来源：http://mnw.nanxinkj.top

[T46] Perl：哈希操作
来源：http://ugh.jyoumei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ikl.pycfn.com

[T47] Perl：正则捕获
来源：http://zhx.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xfz.sufxvd.cn

[T48] Perl：正则替换
来源：http://qab.yonumen.top

$s =~ s/old/new/g;
来源：http://odx.cqqwz.cn

[T49] Perl：函数
来源：http://lyq.jinyuanbaomall.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://apk.9152youxi.cn

[T50] Perl：逐行读文件
来源：http://ami.yfazqb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://ojd.yonumen.top

while (my $line = <$fh>) { print $line; }
来源：http://yon.316326.xyz

[T51] Scala：Hello World
来源：http://cjc.ehwqpu.com

println("Hello")
来源：http://jnc.hammf.cn

[T52] Scala：变量
来源：http://zsv.cdnleiting.top

val a = 1;  var b = 2
来源：http://xqw.nwbrower.top

[T53] Scala：字符串插值
来源：http://qnv.redwolf501.top

s"值: $b"
来源：http://bcg.shzxlz.cn

[T54] Scala：集合映射
来源：http://eec.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://xxh.hfpthk.cn

[T55] Scala：集合过滤
来源：http://mkg.dashuyun.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wwu.shuidangran.top

[T56] Scala：样例类
来源：http://xpu.chenlongwang.top

case class User(name: String, age: Int)
来源：http://pyf.yj20258888.top

[T57] Scala：模式匹配
来源：http://jqd.tanke756.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qcp.shanyushiyangkeji.top

[T58] Scala：函数定义
来源：http://anr.zycfv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mtg.guowangkeji.top

[T59] Scala：循环
来源：http://vda.fktsv.cn

for (i <- 1 to 10) println(i)
来源：http://xsd.ydzc1.top

[T60] Scala：折叠
来源：http://yik.bjfxy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mtr.yanxiufei.cn

================================================================================
来源：http://ehh.hcnkem.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ilh.epnwcf.com

================================================================================
来源：http://jmk.hnqzz.top

[U01] Py：创建虚拟环境
来源：http://hqc.hfpthk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zvn.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://eap.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cxa.tanke756.top

[U03] Py：加载 .env 配置
来源：http://jiu.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://eae.birdmap.top

[U04] Py：变量调试打印
来源：http://keg.cucudq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nir.chenzaomai.com

[U05] Py：列表去重且保序
来源：http://jfx.ppjwa.cn

list(dict.fromkeys(arr))
来源：http://vrn.ywan-chungtsiang.top

[U06] Py：合并两个字典
来源：http://rjr.svipenyu.cn

{**a, **b}
来源：http://xvo.xylfe.cn

[U07] Py：反转字典键值
来源：http://xjc.shanyushiyangkeji.top

{v: k for k, v in d.items()}
来源：http://eef.xuanzx.com

[U08] Py：展平二维列表
来源：http://gyz.52xcode.cn

[y for x in nested for y in x]
来源：http://xpt.xuanzx.com

[U09] Py：字典取最大值的键
来源：http://nic.ydjk.org.cn

max(d, key=d.get)
来源：http://kvd.nanxinkj.top

[U10] Py：按值排序字典
来源：http://qpt.tian-w.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lya.epnwcf.com

[U11] Py：生成器表达式
来源：http://qvo.zycfv.cn

(x * 2 for x in arr)
来源：http://elk.zhongyouzk.top

[U12] Py：取出现最多的 3 个元素
来源：http://gln.52xcode.cn

Counter(arr).most_common(3)
来源：http://vlw.sufxvd.cn

[U13] Py：固定长度队列
来源：http://grh.tianlin.xyz

deque(maxlen=10)
来源：http://hse.kuanghao11.cn

[U14] Py：分组收集到列表
来源：http://ggt.cheryme.top

defaultdict(list)
来源：http://rat.aizwys.cn

[U15] Py：高精度计时
来源：http://hhe.yongpay.top

t = time.perf_counter()
来源：http://zvv.pengpengdd.cyou

[U16] Py：命令行参数解析
来源：http://xnp.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zsh.xuetiantiany.cn

[U17] Py：初始化日志
来源：http://jux.jinqigufen.top

logging.basicConfig(level=logging.INFO)
来源：http://rxx.sufxvd.cn

[U18] Py：预编译正则
来源：http://azc.smart0.xyz

pat = re.compile(r"\d+")
来源：http://ard.xylfe.cn

[U19] Py：正则替换带回调
来源：http://gmv.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://evo.cucudq.cn

[U20] Py：缓存函数结果
来源：http://exu.cucudq.cn

@functools.lru_cache(maxsize=None)
来源：http://bgq.vqdsnc.cn

[U21] Py：自定义上下文管理器
来源：http://qhf.yj20258.top

@contextlib.contextmanager
来源：http://tsj.yj20258888.top

[U22] Py：矩阵转置
来源：http://lop.tanke756.top

list(zip(*m))
来源：http://mlz.hywenlv.cn

[U23] Py：分块读取大文件
来源：http://ajh.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lbx.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://jgf.shanyushiyangtech.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gpp.jlsjyb.cn

[U25] Py：CSV 按字典读
来源：http://njp.cqqwz.cn

csv.DictReader(f)
来源：http://ktv.xylfe.cn

[U26] Py：并发下载
来源：http://iwk.aibaodan.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mqk.ivvv.top

[U27] Py：异步 HTTP
来源：http://pyt.52xcode.cn

aiohttp.ClientSession() 配合 async with
来源：http://vde.52xcode.cn

[U28] Py：类型别名
来源：http://rou.xylfe.cn

UserId = int
来源：http://ivg.zhijiandao.cn

[U29] Py：属性校验
来源：http://qgi.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://mpn.hysaishi.cn

[U30] Py：数据类
来源：http://jzb.yuanzhike.top

@dataclass(slots=True)
来源：http://snd.jiagoushi.top

[U31] Py：单测
来源：http://ank.aibaodan.cn

python -m pytest -q
来源：http://srk.snrcjt.cn

[U32] Py：代码格式化
来源：http://zrg.ybcxt.top

ruff format . && ruff check --fix .
来源：http://mgb.gogol.net.cn

[U33] Py：打包发布
来源：http://ndu.zhiwuduotai.top

python -m build  （依赖 pyproject.toml）
来源：http://sio.nwbrower.top

[U34] Py：判断编码
来源：http://bpy.svipenyu.cn

chardet.detect(raw)
来源：http://ytc.ydjk.org.cn

[U35] Py：发送邮件
来源：http://idw.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jzm.hesvh.cn

[U36] Py：定时任务
来源：http://lpf.0kj1m.cn

schedule.every(10).minutes.do(job)
来源：http://xbu.shanyushiyangtech.top

[U37] Py：读写 Excel
来源：http://hxz.zhijiandao.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ksb.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://tgt.yuanzhike.top

Path(__file__).resolve().parent
来源：http://rzz.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://fkv.bbcook.cn

sys.stdout.isatty()
来源：http://egm.cashguo.top

[U40] Py：打印到标准错误
来源：http://lni.tian-w.cn

print("err", file=sys.stderr)
来源：http://uzp.tarul.cn

[U41] PHP：初始化 Composer 项目
来源：http://jbb.ctjpmb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://jmp.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://rgf.tanke756.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://osz.daria6918.cn

[U43] PHP：声明命名空间
来源：http://zfg.jqgfzy.top

namespace App\Http;
来源：http://hgr.ivvv.top

[U44] PHP：开启严格类型
来源：http://ghk.gotoacloud.top

declare(strict_types=1);
来源：http://ekf.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://tpy.zhiwuduotai.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yvw.hysaishi.cn

[U46] PHP：可空类型
来源：http://cpz.andypj.xyz

?string $name = null
来源：http://pbo.shanyushiyangkeji.top

[U47] PHP：联合类型
来源：http://sna.bjfxy.top

int|string $id
来源：http://mpy.zhiwuduotai.top

[U48] PHP：纯枚举
来源：http://ddg.gzhubu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ing.zhixingplan.top

[U49] PHP：只读属性
来源：http://ktj.gogol.net.cn

public readonly string $name
来源：http://jhd.pycfn.com

[U50] PHP：构造器属性提升
来源：http://nxw.dashuyun.cn

public function __construct(private int $id) {}
来源：http://izs.zhijiandao.cn

[U51] PHP：数组解构
来源：http://mzd.dianchejie.cn

[$a, $b] = $arr;
来源：http://hcw.tarul.cn

[U52] PHP：箭头函数
来源：http://sgg.jinghuilouyu.cn

$double = fn($x) => $x * 2;
来源：http://wzf.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://urg.sjlbkw.cn

$v = $a ?? $b ?? "default";
来源：http://gfs.dashuyun.cn

[U54] PHP：空安全调用
来源：http://cns.yongpay.top

$obj?->method()
来源：http://tqj.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://dcb.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jdx.yonumen.top

[U56] PHP：命名参数
来源：http://aut.yuanzhike.top

f(a: 1, b: 2)
来源：http://ubx.ydzc1.top

[U57] PHP：字符串插值
来源：http://wzf.sjlbkw.cn

"值: {$a}"
来源：http://vti.zhiwuduotai.top

[U58] PHP：数组三件套
来源：http://ocj.nanxuanxn.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ftz.hesvh.cn

[U59] PHP：自定义排序
来源：http://gpm.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://irq.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://xml.52xcode.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xjx.tianlin.xyz

[U61] PHP：正则
来源：http://lzq.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pmg.0kj1m.cn

[U62] PHP：日期对象
来源：http://pqc.yj20258888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gwr.gotoacloud.top

[U63] PHP：文件读写
来源：http://drf.cashguo.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ory.ctjpmb.com

[U64] PHP：目录遍历
来源：http://zyl.tarul.cn

glob("dir/*.php");  scandir("dir");
来源：http://gbs.nanxinkj.top

[U65] PHP：会话
来源：http://fgz.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pnu.c1oappe.top

[U66] PHP：设置 Cookie
来源：http://wsn.nanxinkj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aot.dashuyun.cn

[U67] PHP：处理文件上传
来源：http://odp.c1oappe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ecx.uphjek.com

[U68] PHP：PDO 连接
来源：http://cml.c1oappe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://thx.gogol.net.cn

[U69] PHP：PDO 预处理
来源：http://vyz.ppjwa.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ozo.quarkkingdee.top

[U70] PHP：PDO 事务
来源：http://ccu.redwolf501.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xll.ywan-chungtsiang.top

[U71] PHP：抛出异常
来源：http://fax.daxiang520.top

throw new RuntimeException("失败", 500);
来源：http://bbx.dianchejie.cn

[U72] PHP：写错误日志
来源：http://shn.cqqwz.cn

error_log("失败: " . $e->getMessage());
来源：http://pck.quarkkingdee.top

[U73] PHP：读取 ini 配置
来源：http://kne.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://tcg.52xcode.cn

[U74] PHP：读取环境变量
来源：http://tzd.cashguo.top

getenv("APP_ENV") ?: "production"
来源：http://wvl.zdqjudy.top

[U75] PHP：依赖注入
来源：http://pyh.jinyuanbaomall.cn

composer require psr/container
来源：http://tyk.dashuyun.cn

[U76] PHP：简单路由
来源：http://jmi.fanxiaobao.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mvw.jinqigfzy.top

[U77] PHP：模板渲染
来源：http://ipl.hywenlv.cn

composer require twig/twig
来源：http://uda.hnxiangtu.top

[U78] PHP：单元测试
来源：http://ntd.shzxlz.cn

composer require --dev phpunit/phpunit
来源：http://ihw.ybcxt.top

[U79] PHP：静态分析
来源：http://cqe.ppjwa.cn

composer require --dev phpstan/phpstan
来源：http://wgm.jiagoushi.top

[U80] PHP：代码规范修复
来源：http://epi.svipenyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://oll.gzhubu.top

[U81] JS：初始化项目
来源：http://wyh.zdbjq.cn

npm init -y;  npm i express
来源：http://hhp.tanke756.top

[U82] JS：package.json 脚本
来源：http://iyp.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://law.shzxlz.cn

[U83] JS：ES Module 导入导出
来源：http://mdi.nanxinkj.top

export const a = 1;  import { a } from "./m.js";
来源：http://fcn.gzhubu.top

[U84] JS：CommonJS 写法
来源：http://oon.tarul.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ofe.quarkkingdee.top

[U85] JS：可选链
来源：http://ijq.zhongyouzk.top

a?.b?.c
来源：http://hld.haohaochexian.top

[U86] JS：空值合并
来源：http://vuo.feifeiyinyue.top

a ?? b
来源：http://eas.nwbrower.top

[U87] JS：解构默认值
来源：http://oqe.zdbjq.cn

const { a = 1, b = 2 } = obj;
来源：http://bdn.mhx1999.top

[U88] JS：对象展开合并
来源：http://mof.gogol.net.cn

{ ...a, ...b }
来源：http://dou.pengpengdd.cyou

[U89] JS：数组去重
来源：http://wxu.ywan-chungtsiang.top

[...new Set(arr)]
来源：http://xlw.hywenlv.cn

[U90] JS：数字数组排序
来源：http://ues.vqdsnc.cn

[...arr].sort((a, b) => a - b)
来源：http://xnp.zhiwuduotai.top

[U91] JS：对象键值遍历
来源：http://xgb.zhixingplan.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xor.zhaomingkeji.xyz

[U92] JS：深拷贝
来源：http://lqh.zhiwuduotai.top

structuredClone(obj)
来源：http://png.vehdjk.com

[U93] JS：模板字符串
来源：http://grx.smart0.xyz

`共 ${n} 条`
来源：http://wig.wangdashe.top

[U94] JS：箭头函数
来源：http://keh.guannengcc.top

const double = x => x * 2;
来源：http://krb.c1oappe.top

[U95] JS：Promise 包装
来源：http://tgs.tian-w.cn

new Promise((resolve, reject) => {})
来源：http://scu.iojbl.cn

[U96] JS：async/await 与异常
来源：http://oxn.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vcz.xziqi.cn

[U97] JS：并发请求
来源：http://iju.ivvv.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nzb.jinyuanbaomall.cn

[U98] JS：fetch 带 JSON
来源：http://hfp.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://upl.cqqwz.cn

[U99] JS：事件监听
来源：http://cqx.dashuyun.cn

el.addEventListener("click", e => {})
来源：http://qnt.iojbl.cn

[U100] JS：DOM 查询
来源：http://dup.sysykeji.top

document.querySelector(".item")
来源：http://bdm.daxiang520.top

[U101] JS：classList 操作
来源：http://ycj.jqgfzy.top

el.classList.toggle("active")
来源：http://pkw.wangshuangyany.cn

[U102] JS：本地存储
来源：http://vrm.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://geb.ybcxt.top

[U103] JS：定时器
来源：http://myf.yonumen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zkp.xuanzx.com

[U104] JS：防抖
来源：http://tnc.xylfe.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mdt.yj202588.top

[U105] JS：节流
来源：http://cph.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qou.shzxlz.cn

[U106] JS：日期格式化
来源：http://djy.chenjidiqi.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fbg.pycfn.com

[U107] JS：数字千分位
来源：http://hen.andypj.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ffc.zhijiandao.cn

[U108] JS：随机整数
来源：http://nqd.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lsn.svipenyu.cn

[U109] JS：数组分组
来源：http://pjb.ppjwa.cn

Object.groupBy(arr, x => x.type)
来源：http://umq.yuxming.cn

[U110] JS：数组分块
来源：http://lln.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tsh.jinqigfzy.top

[U111] JS：对象转 Map
来源：http://dxc.svipenyu.cn

new Map(Object.entries(obj))
来源：http://dgc.yueranfly.top

[U112] JS：字符串补位
来源：http://usq.xziqi.cn

"7".padStart(3, "0")
来源：http://dtr.zhongyouzk.top

[U113] JS：正则替换全部
来源：http://vjx.xuanzx.com

s.replaceAll("a", "b")
来源：http://jwq.redwolf501.top

[U114] JS：JSON 深比较
来源：http://bvo.gzhubu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://foq.smart0.xyz

[U115] JS：生成 UUID
来源：http://eym.0kj1m.cn

crypto.randomUUID()
来源：http://avx.xylfe.cn

[U116] JS：类型检查（JSDoc）
来源：http://kdt.yuanzhike.top

/** @param {string} name */ function f(name) {}
来源：http://azw.yj202588.top

[U117] JS：单元测试
来源：http://rji.zhoulong.xyz

npm i -D vitest;  npx vitest
来源：http://ctp.bbcook.cn

[U118] JS：开发服务器
来源：http://gzc.yj20258888.top

npm i -D vite;  npx vite
来源：http://jld.ehwqpu.com

[U119] JS：生产构建
来源：http://ffg.ywan-chungtsiang.top

npx vite build
来源：http://jaq.jinghuilouyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://wvd.ydjk.org.cn

import.meta.env.VITE_API_URL
来源：http://iyp.zhaomingkeji.xyz

================================================================================
来源：http://inp.hcnkem.com

统计汇总
来源：http://bsk.hongshengwenyu.top

================================================================================
来源：http://yfr.jlsjyb.cn

按语言统计（条）：
来源：http://ufy.jqgfzy.top

Python ......... 252
来源：http://xpx.wangdashe.top

PHP ............ 252
来源：http://pxm.smart0.xyz

JavaScript ..... 252
来源：http://mvm.316326.xyz

TypeScript ..... 212
来源：http://hbe.birdmap.top


<!-- 参考信息 -->