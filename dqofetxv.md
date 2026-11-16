代发 wailian999

[T45] Perl：数组遍历
来源：http://ien.fehbvm.com

for my $x (@arr) { print $x; }
来源：http://igt.shuidangran.top

[T46] Perl：哈希操作
来源：http://zwj.hysaishi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://txi.xinyue.icu

[T47] Perl：正则捕获
来源：http://zrt.tianlin.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://der.yuanzhike.top

[T48] Perl：正则替换
来源：http://mmh.ybcxt.top

$s =~ s/old/new/g;
来源：http://prn.sxryk.cn

[T49] Perl：函数
来源：http://xjq.svipenyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sgy.xuetiantiany.cn

[T50] Perl：逐行读文件
来源：http://asy.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yha.zhaomingkeji.xyz

while (my $line = <$fh>) { print $line; }
来源：http://prr.hfpthk.cn

[T51] Scala：Hello World
来源：http://jvu.xinyue.icu

println("Hello")
来源：http://xbb.hesvh.cn

[T52] Scala：变量
来源：http://ynw.yonumen.top

val a = 1;  var b = 2
来源：http://wmf.nanxinkj.top

[T53] Scala：字符串插值
来源：http://jlb.hcnkem.com

s"值: $b"
来源：http://mvm.shuidangran.top

[T54] Scala：集合映射
来源：http://jjc.fengsongda.top

List(1, 2, 3).map(_ * 2)
来源：http://wra.svipenyu.cn

[T55] Scala：集合过滤
来源：http://yta.bbcook.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mok.yfazqb.com

[T56] Scala：样例类
来源：http://rxs.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://kgc.tianlin.xyz

[T57] Scala：模式匹配
来源：http://ard.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://tck.ydzc1.top

[T58] Scala：函数定义
来源：http://jhg.aizwys.cn

def add(a: Int, b: Int): Int = a + b
来源：http://iha.cucudq.cn

[T59] Scala：循环
来源：http://ylq.cdnleiting.top

for (i <- 1 to 10) println(i)
来源：http://cdx.gogol.net.cn

[T60] Scala：折叠
来源：http://tyz.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://anf.9152youxi.cn

================================================================================
来源：http://cnz.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://crx.ydzc1.top

================================================================================
来源：http://foo.xylfe.cn

[U01] Py：创建虚拟环境
来源：http://djm.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://oew.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://xew.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vaj.9152youxi.cn

[U03] Py：加载 .env 配置
来源：http://rxl.hammf.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://enm.dashuyun.cn

[U04] Py：变量调试打印
来源：http://rky.wangshuangyany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xri.ivvv.top

[U05] Py：列表去重且保序
来源：http://wbv.zhoulong.xyz

list(dict.fromkeys(arr))
来源：http://oho.ydjk.org.cn

[U06] Py：合并两个字典
来源：http://cqr.jinghuilouyu.cn

{**a, **b}
来源：http://dba.feifeiyinyue.top

[U07] Py：反转字典键值
来源：http://wpn.gogol.net.cn

{v: k for k, v in d.items()}
来源：http://fgq.fzhhl.top

[U08] Py：展平二维列表
来源：http://vxn.wangdashe.top

[y for x in nested for y in x]
来源：http://thc.yj20258888.top

[U09] Py：字典取最大值的键
来源：http://rin.zhoulong.xyz

max(d, key=d.get)
来源：http://xhr.zdqjudy.top

[U10] Py：按值排序字典
来源：http://big.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uhu.zhiwuduotai.top

[U11] Py：生成器表达式
来源：http://ioo.havefunace.top

(x * 2 for x in arr)
来源：http://szy.sjlbkw.cn

[U12] Py：取出现最多的 3 个元素
来源：http://coa.zhongyouzk.top

Counter(arr).most_common(3)
来源：http://fln.guowangkeji.top

[U13] Py：固定长度队列
来源：http://mmw.jiagoushi.top

deque(maxlen=10)
来源：http://ery.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://nks.epnwcf.com

defaultdict(list)
来源：http://sow.guannengcc.top

[U15] Py：高精度计时
来源：http://tzc.0kj1m.cn

t = time.perf_counter()
来源：http://ejb.jinqigfzy.top

[U16] Py：命令行参数解析
来源：http://cel.ywan-chungtsiang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://onq.jinyuanbaomall.cn

[U17] Py：初始化日志
来源：http://voe.guowangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://gqf.gzhubu.top

[U18] Py：预编译正则
来源：http://qco.cashguo.top

pat = re.compile(r"\d+")
来源：http://ksi.tarul.cn

[U19] Py：正则替换带回调
来源：http://zem.hfpthk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://duf.mhx1999.top

[U20] Py：缓存函数结果
来源：http://wkq.uphjek.com

@functools.lru_cache(maxsize=None)
来源：http://vbz.gaohongyu789.top

[U21] Py：自定义上下文管理器
来源：http://bzg.shuidangran.top

@contextlib.contextmanager
来源：http://swv.meibo888.top

[U22] Py：矩阵转置
来源：http://xif.aizwys.cn

list(zip(*m))
来源：http://gmn.hesvh.cn

[U23] Py：分块读取大文件
来源：http://pkx.cashguo.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://awa.sufxvd.cn

[U24] Py：路径操作
来源：http://noh.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nbq.yueranfly.top

[U25] Py：CSV 按字典读
来源：http://fzd.gogol.net.cn

csv.DictReader(f)
来源：http://zxs.ehwqpu.com

[U26] Py：并发下载
来源：http://zad.52xcode.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wmx.yongpay.top

[U27] Py：异步 HTTP
来源：http://mnv.bbcook.cn

aiohttp.ClientSession() 配合 async with
来源：http://erw.iojbl.cn

[U28] Py：类型别名
来源：http://aen.shanyushiyangtech.top

UserId = int
来源：http://hkg.ctjpmb.com

[U29] Py：属性校验
来源：http://jbb.tarul.cn

@property 与 @x.setter 配合
来源：http://hdu.epnwcf.com

[U30] Py：数据类
来源：http://luj.dashuyun.cn

@dataclass(slots=True)
来源：http://klo.ydjk.org.cn

[U31] Py：单测
来源：http://aiv.guowangkeji.top

python -m pytest -q
来源：http://dxw.hywenlv.cn

[U32] Py：代码格式化
来源：http://bve.yanxiufei.cn

ruff format . && ruff check --fix .
来源：http://ubz.jinyuanbaomall.cn

[U33] Py：打包发布
来源：http://lmu.ehwqpu.com

python -m build  （依赖 pyproject.toml）
来源：http://shd.chenlongwang.top

[U34] Py：判断编码
来源：http://cdk.zycfv.cn

chardet.detect(raw)
来源：http://scm.yuanzhike.top

[U35] Py：发送邮件
来源：http://ftp.feifeiyinyue.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fev.haohaochexian.top

[U36] Py：定时任务
来源：http://hyn.smart0.xyz

schedule.every(10).minutes.do(job)
来源：http://tkc.fengsongda.top

[U37] Py：读写 Excel
来源：http://mtt.hnxiangtu.top

pandas.read_excel / DataFrame.to_excel
来源：http://yqf.jinqigfzy.top

[U38] Py：获取脚本所在目录
来源：http://jme.jlsjyb.cn

Path(__file__).resolve().parent
来源：http://gpw.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://nsh.aibaodan.cn

sys.stdout.isatty()
来源：http://rvg.cqqwz.cn

[U40] Py：打印到标准错误
来源：http://ebv.smart0.xyz

print("err", file=sys.stderr)
来源：http://msv.316326.xyz

[U41] PHP：初始化 Composer 项目
来源：http://ilp.chenjidiqi.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://poh.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://grr.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fxh.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://vxq.daxiang520.top

namespace App\Http;
来源：http://avy.chenjidiqi.icu

[U44] PHP：开启严格类型
来源：http://bpv.tian-w.cn

declare(strict_types=1);
来源：http://gmn.0kj1m.cn

[U45] PHP：类型声明与返回类型
来源：http://xna.zycfv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wwg.ppjwa.cn

[U46] PHP：可空类型
来源：http://kjs.xingfuxueyuan.xyz

?string $name = null
来源：http://ovc.xingfuxueyuan.xyz

[U47] PHP：联合类型
来源：http://czd.yanxiufei.cn

int|string $id
来源：http://gbm.dashuyun.cn

[U48] PHP：纯枚举
来源：http://qfp.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uho.pycfn.com

[U49] PHP：只读属性
来源：http://fdy.hongshengwenyu.top

public readonly string $name
来源：http://vsn.fzhhl.top

[U50] PHP：构造器属性提升
来源：http://syl.bjfxy.top

public function __construct(private int $id) {}
来源：http://uxr.aizwys.cn

[U51] PHP：数组解构
来源：http://krg.shanyushiyangtech.top

[$a, $b] = $arr;
来源：http://omv.xylfe.cn

[U52] PHP：箭头函数
来源：http://ygi.yj202588.top

$double = fn($x) => $x * 2;
来源：http://fra.kuanghao11.cn

[U53] PHP：空合并运算符
来源：http://vxo.nanxinkj.top

$v = $a ?? $b ?? "default";
来源：http://ldz.havefunace.top

[U54] PHP：空安全调用
来源：http://gsa.chenzaomai.com

$obj?->method()
来源：http://vmp.vehdjk.com

[U55] PHP：match 表达式
来源：http://lvv.jlsjyb.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cuq.hammf.cn

[U56] PHP：命名参数
来源：http://hzm.havefunace.top

f(a: 1, b: 2)
来源：http://pfk.cdnleiting.top

[U57] PHP：字符串插值
来源：http://nwn.jinqigfzy.top

"值: {$a}"
来源：http://qcj.sxryk.cn

[U58] PHP：数组三件套
来源：http://ipo.dashuyun.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://izm.smart0.xyz

[U59] PHP：自定义排序
来源：http://knu.0kj1m.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pww.hfpthk.cn

[U60] PHP：JSON 编解码
来源：http://jbm.sxryk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://phz.sysykeji.top

[U61] PHP：正则
来源：http://era.jiagoushi.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ulf.sysykeji.top

[U62] PHP：日期对象
来源：http://uju.jinqigufen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://csf.yfazqb.com

[U63] PHP：文件读写
来源：http://kje.pengpengdd.cyou

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vvr.shuidangran.top

[U64] PHP：目录遍历
来源：http://dlc.wangshuangyany.cn

glob("dir/*.php");  scandir("dir");
来源：http://elf.nanxinkj.top

[U65] PHP：会话
来源：http://nzb.fehbvm.com

session_start();  $_SESSION["uid"] = 1;
来源：http://vin.zdqjudy.top

[U66] PHP：设置 Cookie
来源：http://lkn.shuidangran.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uvh.jyoumei.cn

[U67] PHP：处理文件上传
来源：http://qgy.nwbrower.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://laj.tarul.cn

[U68] PHP：PDO 连接
来源：http://mly.c1oappe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ozd.cqqwz.cn

[U69] PHP：PDO 预处理
来源：http://cpa.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mpz.daria6918.cn

[U70] PHP：PDO 事务
来源：http://khx.xinyue.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mez.daria6918.cn

[U71] PHP：抛出异常
来源：http://eti.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://ieb.zhiwuduotai.top

[U72] PHP：写错误日志
来源：http://xzg.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://xwe.havefunace.top

[U73] PHP：读取 ini 配置
来源：http://wec.xylfe.cn

parse_ini_file("config.ini", true)
来源：http://aid.xinyue.icu

[U74] PHP：读取环境变量
来源：http://kbl.ybcxt.top

getenv("APP_ENV") ?: "production"
来源：http://gly.hnqzz.top

[U75] PHP：依赖注入
来源：http://dnr.yj20258888.top

composer require psr/container
来源：http://tfi.mhx1999.top

[U76] PHP：简单路由
来源：http://isv.zhixingplan.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xek.52xcode.cn

[U77] PHP：模板渲染
来源：http://mrx.tarul.cn

composer require twig/twig
来源：http://tbg.cucudq.cn

[U78] PHP：单元测试
来源：http://edo.yueranfly.top

composer require --dev phpunit/phpunit
来源：http://abf.gaohongyu789.top

[U79] PHP：静态分析
来源：http://mpu.zdbjq.cn

composer require --dev phpstan/phpstan
来源：http://bov.xuetiantiany.cn

[U80] PHP：代码规范修复
来源：http://owd.hywenlv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gzv.ydzc1.top

[U81] JS：初始化项目
来源：http://biv.chenjidiqi.icu

npm init -y;  npm i express
来源：http://xze.snrcjt.cn

[U82] JS：package.json 脚本
来源：http://owd.jqgufenzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mpk.xinyue.icu

[U83] JS：ES Module 导入导出
来源：http://jli.birdmap.top

export const a = 1;  import { a } from "./m.js";
来源：http://tiu.tianlin.xyz

[U84] JS：CommonJS 写法
来源：http://krt.redwolf501.top

module.exports = { a };  const { a } = require("./m");
来源：http://gkw.xingfuxueyuan.xyz

[U85] JS：可选链
来源：http://opn.wangshuangyany.cn

a?.b?.c
来源：http://ybq.mhx1999.top

[U86] JS：空值合并
来源：http://nul.zhijiandao.cn

a ?? b
来源：http://umf.yonumen.top

[U87] JS：解构默认值
来源：http://vzg.9152youxi.cn

const { a = 1, b = 2 } = obj;
来源：http://wpo.jinghuilouyu.cn

[U88] JS：对象展开合并
来源：http://dtv.birdmap.top

{ ...a, ...b }
来源：http://mcg.sjlbkw.cn

[U89] JS：数组去重
来源：http://cfi.chenjidiqi.icu

[...new Set(arr)]
来源：http://xji.xylfe.cn

[U90] JS：数字数组排序
来源：http://wyh.jinghuilouyu.cn

[...arr].sort((a, b) => a - b)
来源：http://ctr.zycfv.cn

[U91] JS：对象键值遍历
来源：http://slf.9152youxi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://njv.jianghu66.top

[U92] JS：深拷贝
来源：http://mkt.dashuyun.cn

structuredClone(obj)
来源：http://pus.hnxiangtu.top

[U93] JS：模板字符串
来源：http://vzm.fengsongda.top

`共 ${n} 条`
来源：http://vsp.hnqzz.top

[U94] JS：箭头函数
来源：http://wos.316326.xyz

const double = x => x * 2;
来源：http://ccv.xziqi.cn

[U95] JS：Promise 包装
来源：http://uyt.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://zjl.fanxiaobao.xyz

[U96] JS：async/await 与异常
来源：http://ann.zhiwuduotai.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ccx.jiagoushi.top

[U97] JS：并发请求
来源：http://yvu.shuidangran.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xyv.dianchejie.cn

[U98] JS：fetch 带 JSON
来源：http://chr.fktsv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qnv.iojbl.cn

[U99] JS：事件监听
来源：http://gny.ybcxt.top

el.addEventListener("click", e => {})
来源：http://tok.meibo888.top

[U100] JS：DOM 查询
来源：http://wyh.kuanghao11.cn

document.querySelector(".item")
来源：http://taj.zhongyouzk.top

[U101] JS：classList 操作
来源：http://otp.birdmap.top

el.classList.toggle("active")
来源：http://cpf.bjfxy.top

[U102] JS：本地存储
来源：http://hke.nanxinkj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://quq.nwbrower.top

[U103] JS：定时器
来源：http://aca.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sbz.zhongyouzk.top

[U104] JS：防抖
来源：http://zwp.ydzc1.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uhl.dashuyun.cn

[U105] JS：节流
来源：http://ugr.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yfq.smart0.xyz

[U106] JS：日期格式化
来源：http://fwv.jlsjyb.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kta.xingfuxueyuan.xyz

[U107] JS：数字千分位
来源：http://kdf.aibaodan.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vjj.jinyuanbaomall.cn

[U108] JS：随机整数
来源：http://jse.fengsongda.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yqy.zhoulong.xyz

[U109] JS：数组分组
来源：http://rhr.wangshuangyany.cn

Object.groupBy(arr, x => x.type)
来源：http://crv.bjfxy.top

[U110] JS：数组分块
来源：http://xxc.aizwys.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fsj.vehdjk.com

[U111] JS：对象转 Map
来源：http://frx.316326.xyz

new Map(Object.entries(obj))
来源：http://ume.gotoacloud.top

[U112] JS：字符串补位
来源：http://xdj.hongshengwenyu.top

"7".padStart(3, "0")
来源：http://dnm.uphjek.com

[U113] JS：正则替换全部
来源：http://xui.fzhhl.top

s.replaceAll("a", "b")
来源：http://akz.guannengcc.top

[U114] JS：JSON 深比较
来源：http://dbb.hammf.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ekp.dashuyun.cn

[U115] JS：生成 UUID
来源：http://vnh.9152youxi.cn

crypto.randomUUID()
来源：http://ozv.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://flb.jinghuilouyu.cn

/** @param {string} name */ function f(name) {}
来源：http://unp.quarkkingdee.top

[U117] JS：单元测试
来源：http://ubb.fengsongda.top

npm i -D vitest;  npx vitest
来源：http://hbg.chenzaomai.com

[U118] JS：开发服务器
来源：http://dhb.ehwqpu.com

npm i -D vite;  npx vite
来源：http://jee.iojbl.cn

[U119] JS：生产构建
来源：http://sve.guowangkeji.top

npx vite build
来源：http://vzr.tanke756.top

[U120] JS：读取环境变量（Vite）
来源：http://vjs.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://ymr.ivvv.top

================================================================================
来源：http://ier.ywan-chungtsiang.top

统计汇总
来源：http://qlk.shanyushiyangtech.top

================================================================================
来源：http://cnz.fanxiaobao.xyz

按语言统计（条）：
来源：http://bqw.guannengcc.top

Python ......... 252
来源：http://hqj.feifeiyinyue.top

PHP ............ 252
来源：http://heh.yanxiufei.cn

JavaScript ..... 252
来源：http://uyq.gogol.net.cn

TypeScript ..... 212
来源：http://knz.cucudq.cn

Java ........... 212
来源：http://bmo.yuanzhike.top

Go ............. 212
来源：http://ocj.yj20258888.top

Ruby ........... 212
来源：http://ggt.tian-w.cn

C# ............. 212
来源：http://ycu.xinyue.icu

C .............. 30
来源：http://gqb.andypj.xyz

C++ ............ 30
来源：http://dtz.ehwqpu.com

SQL ............ 90
来源：http://ycb.cheryme.top

Bash ........... 80
来源：http://nvt.fktsv.cn

Kotlin ......... 15
来源：http://koc.fengsongda.top

Swift .......... 15
来源：http://znk.zhijiandao.cn

Lua ............ 10
来源：http://fhf.yonumen.top

Perl ........... 10
来源：http://yqu.yj20258.top

Scala .......... 10
来源：http://puq.shanyushiyangtech.top

------------------------------------
来源：http://cfm.hcnkem.com

合计 ........... 2106 条
来源：http://wjc.chenjidiqi.icu

按章节统计：
来源：http://rdm.jinqigufen.top


<!-- 参考信息 -->