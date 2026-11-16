代发 wailian999

[T27] Swift：错误处理
来源：http://udv.tarul.cn

do { try f() } catch { print(error) }
来源：http://xsn.jianghu66.top

[T28] Swift：枚举
来源：http://nyi.jlsjyb.cn

enum Color { case red, green }
来源：http://ulg.xuetiantiany.cn

[T29] Swift：guard 提前返回
来源：http://nbl.nanxuanxn.top

guard let x = opt else { return }
来源：http://ozy.pengpengdd.cyou

[T30] Swift：协议
来源：http://iur.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://qjv.andypj.xyz

[T31] Lua：Hello World
来源：http://rdq.c1oappe.top

print("Hello")
来源：http://swe.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://ttk.fehbvm.com

local a = 1
来源：http://upo.ivvv.top

[T33] Lua：表（数组）
来源：http://ohx.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xxv.316326.xyz

[T34] Lua：遍历表
来源：http://chi.zhongyouzk.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lbw.fanxiaobao.xyz

[T35] Lua：字典表
来源：http://uqo.shanyushiyangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://hyo.9152youxi.cn

[T36] Lua：函数
来源：http://yuz.andypj.xyz

function add(a, b) return a + b end
来源：http://viv.ywan-chungtsiang.top

[T37] Lua：字符串拼接
来源：http://ldp.yj202588.top

"a" .. "b"
来源：http://umi.hcnkem.com

[T38] Lua：条件
来源：http://ecx.aibaodan.cn

if x > 0 then print("正") end
来源：http://jhx.ppjwa.cn

[T39] Lua：模式匹配
来源：http://xpc.jlsjyb.cn

string.find(s, "%d+")
来源：http://tac.zdbjq.cn

[T40] Lua：元表
来源：http://yto.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://olq.xylfe.cn

[T41] Perl：Hello World
来源：http://gux.epnwcf.com

print "Hello\n";
来源：http://vua.cheryme.top

[T42] Perl：变量类型
来源：http://yhh.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ypw.316326.xyz

[T43] Perl：字符串插值
来源：http://aya.cdnleiting.top

"值: $a"
来源：http://igv.daxiang520.top

[T44] Perl：条件
来源：http://biu.quarkkingdee.top

if ($a > 0) { print "正"; }
来源：http://qtn.tianlin.xyz

[T45] Perl：数组遍历
来源：http://xgw.fengsongda.top

for my $x (@arr) { print $x; }
来源：http://amf.tianlin.xyz

[T46] Perl：哈希操作
来源：http://jwx.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yha.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://jsg.daxiang520.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yof.zhixingplan.top

[T48] Perl：正则替换
来源：http://zvv.shuidangran.top

$s =~ s/old/new/g;
来源：http://rck.sjlbkw.cn

[T49] Perl：函数
来源：http://nvd.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uch.jyoumei.cn

[T50] Perl：逐行读文件
来源：http://pxy.aizwys.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vfk.hcnkem.com

while (my $line = <$fh>) { print $line; }
来源：http://ehc.birdmap.top

[T51] Scala：Hello World
来源：http://psf.yueranfly.top

println("Hello")
来源：http://mgj.tarul.cn

[T52] Scala：变量
来源：http://bfs.yj20258.top

val a = 1;  var b = 2
来源：http://kie.daria6918.cn

[T53] Scala：字符串插值
来源：http://mvm.shangyingyoupin.top

s"值: $b"
来源：http://wya.tarul.cn

[T54] Scala：集合映射
来源：http://zby.redwolf501.top

List(1, 2, 3).map(_ * 2)
来源：http://utw.pengpengdd.cyou

[T55] Scala：集合过滤
来源：http://jpz.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://hqe.tianlin.xyz

[T56] Scala：样例类
来源：http://jqz.zhoulong.xyz

case class User(name: String, age: Int)
来源：http://nlk.pycfn.com

[T57] Scala：模式匹配
来源：http://oxh.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pkw.hysaishi.cn

[T58] Scala：函数定义
来源：http://lec.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://erh.jianghu66.top

[T59] Scala：循环
来源：http://xae.yangfankeji.com

for (i <- 1 to 10) println(i)
来源：http://xta.tanke756.top

[T60] Scala：折叠
来源：http://ksp.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rwf.ppjwa.cn

================================================================================
来源：http://slt.pycfn.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nwh.chenjidiqi.icu

================================================================================
来源：http://pbd.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://xxy.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://dyg.chenjidiqi.icu

[U02] Py：导出 / 安装依赖
来源：http://tkd.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vxv.ydzc1.top

[U03] Py：加载 .env 配置
来源：http://yoe.fzhhl.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fdl.meibo888.top

[U04] Py：变量调试打印
来源：http://fdt.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vmk.tarul.cn

[U05] Py：列表去重且保序
来源：http://poq.zhiwuduotai.top

list(dict.fromkeys(arr))
来源：http://gmt.tianlin.xyz

[U06] Py：合并两个字典
来源：http://eyl.jiagoushi.top

{**a, **b}
来源：http://yjl.316326.xyz

[U07] Py：反转字典键值
来源：http://lxe.cashguo.top

{v: k for k, v in d.items()}
来源：http://hhl.yanxiufei.cn

[U08] Py：展平二维列表
来源：http://nsg.chenzaomai.com

[y for x in nested for y in x]
来源：http://zbx.birdmap.top

[U09] Py：字典取最大值的键
来源：http://que.meibo888.top

max(d, key=d.get)
来源：http://msp.sufxvd.cn

[U10] Py：按值排序字典
来源：http://eok.jyoumei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nhv.hammf.cn

[U11] Py：生成器表达式
来源：http://ius.xingfuxueyuan.xyz

(x * 2 for x in arr)
来源：http://mat.dianchejie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cta.hysaishi.cn

Counter(arr).most_common(3)
来源：http://bmm.yvedp.cn

[U13] Py：固定长度队列
来源：http://yfz.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://vrm.wangshuangyany.cn

[U14] Py：分组收集到列表
来源：http://rmj.jqgufenzy.top

defaultdict(list)
来源：http://dwd.aizwys.cn

[U15] Py：高精度计时
来源：http://lft.gzhubu.top

t = time.perf_counter()
来源：http://uby.yj202588.top

[U16] Py：命令行参数解析
来源：http://joz.epnwcf.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bdy.nanxuanxn.top

[U17] Py：初始化日志
来源：http://pda.ydzc1.top

logging.basicConfig(level=logging.INFO)
来源：http://vjl.uphjek.com

[U18] Py：预编译正则
来源：http://jaa.tanke756.top

pat = re.compile(r"\d+")
来源：http://gpy.c1oappe.top

[U19] Py：正则替换带回调
来源：http://zax.sweek.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lnk.tian-w.cn

[U20] Py：缓存函数结果
来源：http://dus.shanyushiyangtech.top

@functools.lru_cache(maxsize=None)
来源：http://ocu.jqgufenzy.top

[U21] Py：自定义上下文管理器
来源：http://cul.fanxiaobao.xyz

@contextlib.contextmanager
来源：http://cto.hesvh.cn

[U22] Py：矩阵转置
来源：http://zaa.zhaomingkeji.xyz

list(zip(*m))
来源：http://hct.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://jmp.jyoumei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ymg.yanxiufei.cn

[U24] Py：路径操作
来源：http://dtr.52xcode.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ifh.chenjidiqi.icu

[U25] Py：CSV 按字典读
来源：http://pcu.zhengqikj.top

csv.DictReader(f)
来源：http://szl.yuanzhike.top

[U26] Py：并发下载
来源：http://txo.zhijiandao.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yhj.haohaochexian.top

[U27] Py：异步 HTTP
来源：http://bfk.zhongyouzk.top

aiohttp.ClientSession() 配合 async with
来源：http://fyu.nanxuanxn.top

[U28] Py：类型别名
来源：http://vwm.epnwcf.com

UserId = int
来源：http://nnp.jyoumei.cn

[U29] Py：属性校验
来源：http://lss.chenjidiqi.icu

@property 与 @x.setter 配合
来源：http://pfi.yj20258.top

[U30] Py：数据类
来源：http://hbb.birdmap.top

@dataclass(slots=True)
来源：http://buf.guannengcc.top

[U31] Py：单测
来源：http://ofg.zdqjudy.top

python -m pytest -q
来源：http://sop.yj20258888.top

[U32] Py：代码格式化
来源：http://smi.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://rpv.snrcjt.cn

[U33] Py：打包发布
来源：http://eci.nanxinkj.top

python -m build  （依赖 pyproject.toml）
来源：http://ghz.xuetiantiany.cn

[U34] Py：判断编码
来源：http://qxg.ybcxt.top

chardet.detect(raw)
来源：http://uax.gogol.net.cn

[U35] Py：发送邮件
来源：http://wus.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wud.jianghu66.top

[U36] Py：定时任务
来源：http://xqz.yueranfly.top

schedule.every(10).minutes.do(job)
来源：http://nnz.fehbvm.com

[U37] Py：读写 Excel
来源：http://ckc.zhixingplan.top

pandas.read_excel / DataFrame.to_excel
来源：http://ara.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://esx.316326.xyz

Path(__file__).resolve().parent
来源：http://rhq.hfpthk.cn

[U39] Py：判断是否在交互环境
来源：http://yxj.tanke756.top

sys.stdout.isatty()
来源：http://jjr.gotoacloud.top

[U40] Py：打印到标准错误
来源：http://byi.xinyue.icu

print("err", file=sys.stderr)
来源：http://wza.zycfv.cn

[U41] PHP：初始化 Composer 项目
来源：http://mdb.hesvh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://icf.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://jiu.sufxvd.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ajk.jyoumei.cn

[U43] PHP：声明命名空间
来源：http://wmu.chenlongwang.top

namespace App\Http;
来源：http://uef.hongshengwenyu.top

[U44] PHP：开启严格类型
来源：http://tcw.nanxinkj.top

declare(strict_types=1);
来源：http://osd.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://eap.zdqjudy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xnb.9152youxi.cn

[U46] PHP：可空类型
来源：http://ioj.mhx1999.top

?string $name = null
来源：http://auq.sweek.top

[U47] PHP：联合类型
来源：http://sxe.aizwys.cn

int|string $id
来源：http://gvw.ydzc1.top

[U48] PHP：纯枚举
来源：http://lec.cashguo.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gmk.xinyue.icu

[U49] PHP：只读属性
来源：http://shc.tianlin.xyz

public readonly string $name
来源：http://tld.sjlbkw.cn

[U50] PHP：构造器属性提升
来源：http://opj.jianghu66.top

public function __construct(private int $id) {}
来源：http://bia.xziqi.cn

[U51] PHP：数组解构
来源：http://fat.shzxlz.cn

[$a, $b] = $arr;
来源：http://kpl.zhixingplan.top

[U52] PHP：箭头函数
来源：http://vgz.hcnkem.com

$double = fn($x) => $x * 2;
来源：http://dif.ppjwa.cn

[U53] PHP：空合并运算符
来源：http://lcv.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://szf.cucudq.cn

[U54] PHP：空安全调用
来源：http://obt.yonumen.top

$obj?->method()
来源：http://zir.zhiwuduotai.top

[U55] PHP：match 表达式
来源：http://eij.hesvh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vqv.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://rqq.hesvh.cn

f(a: 1, b: 2)
来源：http://jxy.svipenyu.cn

[U57] PHP：字符串插值
来源：http://nrv.yuanzhike.top

"值: {$a}"
来源：http://omq.jyoumei.cn

[U58] PHP：数组三件套
来源：http://nnn.hesvh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yqw.yuxming.cn

[U59] PHP：自定义排序
来源：http://btn.316326.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bkj.cdnleiting.top

[U60] PHP：JSON 编解码
来源：http://rmr.bjfxy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wdz.yanxiufei.cn

[U61] PHP：正则
来源：http://pdp.zhongyouzk.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vmv.kuanghao11.cn

[U62] PHP：日期对象
来源：http://vyi.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bdu.jlsjyb.cn

[U63] PHP：文件读写
来源：http://jkq.pengpengdd.cyou

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hes.yuxming.cn

[U64] PHP：目录遍历
来源：http://nyf.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://hsc.yj20258888.top

[U65] PHP：会话
来源：http://stu.dianchejie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cmi.guowangkeji.top

[U66] PHP：设置 Cookie
来源：http://pvs.shzxlz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kca.jiagoushi.top

[U67] PHP：处理文件上传
来源：http://qkd.epnwcf.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zdi.ppjwa.cn

[U68] PHP：PDO 连接
来源：http://zsb.fanxiaobao.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uzp.dianchejie.cn

[U69] PHP：PDO 预处理
来源：http://xaw.gzhubu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bpm.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://pho.epnwcf.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://owd.xinyue.icu

[U71] PHP：抛出异常
来源：http://odj.xuetiantiany.cn

throw new RuntimeException("失败", 500);
来源：http://qyv.zhaomingkeji.xyz

[U72] PHP：写错误日志
来源：http://qhm.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://ior.zdbjq.cn

[U73] PHP：读取 ini 配置
来源：http://rpp.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://kin.svipenyu.cn

[U74] PHP：读取环境变量
来源：http://wvm.316326.xyz

getenv("APP_ENV") ?: "production"
来源：http://xvy.ivvv.top

[U75] PHP：依赖注入
来源：http://udy.shanyushiyangkeji.top

composer require psr/container
来源：http://ypn.vehdjk.com

[U76] PHP：简单路由
来源：http://jew.jiagoushi.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lis.havefunace.top

[U77] PHP：模板渲染
来源：http://dkg.zhengqikj.top

composer require twig/twig
来源：http://glg.hesvh.cn

[U78] PHP：单元测试
来源：http://eto.smart0.xyz

composer require --dev phpunit/phpunit
来源：http://bou.zhengqikj.top

[U79] PHP：静态分析
来源：http://tvi.wangdashe.top

composer require --dev phpstan/phpstan
来源：http://tga.xingfuxueyuan.xyz

[U80] PHP：代码规范修复
来源：http://pll.yanxiufei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qeo.hammf.cn

[U81] JS：初始化项目
来源：http://qtf.vqdsnc.cn

npm init -y;  npm i express
来源：http://hfi.nanxuanxn.top

[U82] JS：package.json 脚本
来源：http://yjs.hongshengwenyu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dyb.svipenyu.cn

[U83] JS：ES Module 导入导出
来源：http://xtw.hywenlv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://aoj.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://pju.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://eum.zhixingplan.top

[U85] JS：可选链
来源：http://eeu.ppjwa.cn

a?.b?.c
来源：http://uch.cashguo.top

[U86] JS：空值合并
来源：http://zhk.xuetiantiany.cn

a ?? b
来源：http://rbb.wangdashe.top

[U87] JS：解构默认值
来源：http://xqr.zdqjudy.top

const { a = 1, b = 2 } = obj;
来源：http://oqe.daria6918.cn

[U88] JS：对象展开合并
来源：http://eif.tanke756.top

{ ...a, ...b }
来源：http://dms.hysaishi.cn

[U89] JS：数组去重
来源：http://bds.ppjwa.cn

[...new Set(arr)]
来源：http://kqw.dianchejie.cn

[U90] JS：数字数组排序
来源：http://vei.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://sfp.xylfe.cn

[U91] JS：对象键值遍历
来源：http://bwg.zhoulong.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iwg.zhengqikj.top

[U92] JS：深拷贝
来源：http://puc.shangyingyoupin.top

structuredClone(obj)
来源：http://soo.ybcxt.top

[U93] JS：模板字符串
来源：http://wsv.zycfv.cn

`共 ${n} 条`
来源：http://fex.xuanzx.com

[U94] JS：箭头函数
来源：http://wul.vehdjk.com

const double = x => x * 2;
来源：http://ect.yongpay.top

[U95] JS：Promise 包装
来源：http://ver.wangshuangyany.cn

new Promise((resolve, reject) => {})
来源：http://zyp.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://dzf.gogol.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mpl.hywenlv.cn

[U97] JS：并发请求
来源：http://kyt.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xns.daria6918.cn

[U98] JS：fetch 带 JSON
来源：http://ksu.cdnleiting.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dbx.chenjidiqi.icu

[U99] JS：事件监听
来源：http://llc.jinqigfzy.top

el.addEventListener("click", e => {})
来源：http://xjf.sweek.top

[U100] JS：DOM 查询
来源：http://qej.hcnkem.com

document.querySelector(".item")
来源：http://ixn.zhongyouzk.top

[U101] JS：classList 操作
来源：http://kin.aizwys.cn

el.classList.toggle("active")
来源：http://qwz.ppjwa.cn

[U102] JS：本地存储
来源：http://jbi.zhoulong.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://kdb.zdbjq.cn

[U103] JS：定时器
来源：http://xfa.fzhhl.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dah.chenlongwang.top

[U104] JS：防抖
来源：http://pbh.kuanghao11.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nnc.yj202588.top

[U105] JS：节流
来源：http://fgg.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fao.ywan-chungtsiang.top

[U106] JS：日期格式化
来源：http://vtz.xinyue.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zum.yongpay.top

[U107] JS：数字千分位
来源：http://pou.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bqc.yanxiufei.cn

[U108] JS：随机整数
来源：http://jej.gaohongyu789.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kki.ehwqpu.com

[U109] JS：数组分组
来源：http://fko.yueranfly.top

Object.groupBy(arr, x => x.type)
来源：http://ajv.pengpengdd.cyou

[U110] JS：数组分块
来源：http://fyy.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xak.hnqzz.top

[U111] JS：对象转 Map
来源：http://znb.hnqzz.top

new Map(Object.entries(obj))
来源：http://kmb.hesvh.cn

[U112] JS：字符串补位
来源：http://uje.zdqjudy.top

"7".padStart(3, "0")
来源：http://vdm.feifeiyinyue.top

[U113] JS：正则替换全部
来源：http://mvb.yangfankeji.com

s.replaceAll("a", "b")
来源：http://bzk.cucudq.cn

[U114] JS：JSON 深比较
来源：http://obi.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://srm.jlsjyb.cn


<!-- 参考信息 -->