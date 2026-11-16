代发 wailian999

[T45] Perl：数组遍历
来源：http://trw.guannengcc.top

for my $x (@arr) { print $x; }
来源：http://ypp.shangyingyoupin.top

[T46] Perl：哈希操作
来源：http://usj.tianlin.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oku.ivvv.top

[T47] Perl：正则捕获
来源：http://kjz.bjfxy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rxe.yuanzhike.top

[T48] Perl：正则替换
来源：http://epv.yj20258.top

$s =~ s/old/new/g;
来源：http://mew.jlsjyb.cn

[T49] Perl：函数
来源：http://pig.jqgfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sbk.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://ptm.sufxvd.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pts.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://oor.chenzaomai.com

[T51] Scala：Hello World
来源：http://aim.pengpengdd.cyou

println("Hello")
来源：http://zkc.cheryme.top

[T52] Scala：变量
来源：http://the.meibo888.top

val a = 1;  var b = 2
来源：http://cnt.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://goy.shzxlz.cn

s"值: $b"
来源：http://kck.sjlbkw.cn

[T54] Scala：集合映射
来源：http://trv.yuxming.cn

List(1, 2, 3).map(_ * 2)
来源：http://gxp.ybcxt.top

[T55] Scala：集合过滤
来源：http://bun.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rnz.chenzaomai.com

[T56] Scala：样例类
来源：http://bai.shanyushiyangkeji.top

case class User(name: String, age: Int)
来源：http://wuz.0kj1m.cn

[T57] Scala：模式匹配
来源：http://ebh.dianchejie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bbc.zhixingplan.top

[T58] Scala：函数定义
来源：http://nbb.jiagoushi.top

def add(a: Int, b: Int): Int = a + b
来源：http://wsb.yanxiufei.cn

[T59] Scala：循环
来源：http://yfz.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://yds.jlsjyb.cn

[T60] Scala：折叠
来源：http://ydc.hongshengwenyu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://koh.epnwcf.com

================================================================================
来源：http://bxx.cucudq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fwb.yangfankeji.com

================================================================================
来源：http://nix.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://aag.havefunace.top

python -m venv .venv && source .venv/bin/activate
来源：http://ndv.jinqigfzy.top

[U02] Py：导出 / 安装依赖
来源：http://rob.zhengqikj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dbi.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://ils.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zge.xylfe.cn

[U04] Py：变量调试打印
来源：http://zsh.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aqo.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://kmo.birdmap.top

list(dict.fromkeys(arr))
来源：http://kmy.hcnkem.com

[U06] Py：合并两个字典
来源：http://dxg.yfazqb.com

{**a, **b}
来源：http://qtd.ivvv.top

[U07] Py：反转字典键值
来源：http://hgi.hysaishi.cn

{v: k for k, v in d.items()}
来源：http://txl.bjfxy.top

[U08] Py：展平二维列表
来源：http://uns.yj20258.top

[y for x in nested for y in x]
来源：http://znv.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://qpl.nanxuanxn.top

max(d, key=d.get)
来源：http://wmn.smart0.xyz

[U10] Py：按值排序字典
来源：http://umd.chenlongwang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yvl.tanke756.top

[U11] Py：生成器表达式
来源：http://yob.fehbvm.com

(x * 2 for x in arr)
来源：http://syp.quarkkingdee.top

[U12] Py：取出现最多的 3 个元素
来源：http://vrl.ctjpmb.com

Counter(arr).most_common(3)
来源：http://ftu.hnxiangtu.top

[U13] Py：固定长度队列
来源：http://xza.hcnkem.com

deque(maxlen=10)
来源：http://djo.yj20258888.top

[U14] Py：分组收集到列表
来源：http://pqj.guannengcc.top

defaultdict(list)
来源：http://xgg.daxiang520.top

[U15] Py：高精度计时
来源：http://obj.jlsjyb.cn

t = time.perf_counter()
来源：http://tso.zycfv.cn

[U16] Py：命令行参数解析
来源：http://gmk.yanxiufei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jln.birdmap.top

[U17] Py：初始化日志
来源：http://slz.yuanzhike.top

logging.basicConfig(level=logging.INFO)
来源：http://uss.xylfe.cn

[U18] Py：预编译正则
来源：http://xup.yangfankeji.com

pat = re.compile(r"\d+")
来源：http://ihg.xuetiantiany.cn

[U19] Py：正则替换带回调
来源：http://zjr.hnxiangtu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jgf.jyoumei.cn

[U20] Py：缓存函数结果
来源：http://uwu.bjfxy.top

@functools.lru_cache(maxsize=None)
来源：http://urs.zhixingplan.top

[U21] Py：自定义上下文管理器
来源：http://leb.yanxiufei.cn

@contextlib.contextmanager
来源：http://hsd.52xcode.cn

[U22] Py：矩阵转置
来源：http://nzv.sweek.top

list(zip(*m))
来源：http://eml.shuidangran.top

[U23] Py：分块读取大文件
来源：http://zfa.zdqjudy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ymx.jinyuanbaomall.cn

[U24] Py：路径操作
来源：http://csp.hywenlv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cvq.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://wau.zdqjudy.top

csv.DictReader(f)
来源：http://lnp.yueranfly.top

[U26] Py：并发下载
来源：http://oxf.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pzs.jyoumei.cn

[U27] Py：异步 HTTP
来源：http://lkv.fzhhl.top

aiohttp.ClientSession() 配合 async with
来源：http://wtd.redwolf501.top

[U28] Py：类型别名
来源：http://ztn.gzhubu.top

UserId = int
来源：http://vqi.tanke756.top

[U29] Py：属性校验
来源：http://pxn.bbcook.cn

@property 与 @x.setter 配合
来源：http://gqi.quarkkingdee.top

[U30] Py：数据类
来源：http://fzs.zycfv.cn

@dataclass(slots=True)
来源：http://mww.meibo888.top

[U31] Py：单测
来源：http://qpj.mhx1999.top

python -m pytest -q
来源：http://hpg.aibaodan.cn

[U32] Py：代码格式化
来源：http://vsc.sufxvd.cn

ruff format . && ruff check --fix .
来源：http://duk.haohaochexian.top

[U33] Py：打包发布
来源：http://nmy.tianlin.xyz

python -m build  （依赖 pyproject.toml）
来源：http://alf.gzhubu.top

[U34] Py：判断编码
来源：http://uau.hnqzz.top

chardet.detect(raw)
来源：http://nzd.daria6918.cn

[U35] Py：发送邮件
来源：http://pfn.zhixingplan.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jhb.yueranfly.top

[U36] Py：定时任务
来源：http://mlu.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://bpq.yonumen.top

[U37] Py：读写 Excel
来源：http://yus.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://jnh.guannengcc.top

[U38] Py：获取脚本所在目录
来源：http://ktl.c1oappe.top

Path(__file__).resolve().parent
来源：http://meu.hcnkem.com

[U39] Py：判断是否在交互环境
来源：http://bue.xinyue.icu

sys.stdout.isatty()
来源：http://dtw.shanyushiyangtech.top

[U40] Py：打印到标准错误
来源：http://hhi.feifeiyinyue.top

print("err", file=sys.stderr)
来源：http://ppt.ivvv.top

[U41] PHP：初始化 Composer 项目
来源：http://gdp.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jnk.svipenyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://boi.yanxiufei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kan.jianghu66.top

[U43] PHP：声明命名空间
来源：http://ymp.zdbjq.cn

namespace App\Http;
来源：http://dar.jinghuilouyu.cn

[U44] PHP：开启严格类型
来源：http://pzl.chenlongwang.top

declare(strict_types=1);
来源：http://xhh.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://jlj.gotoacloud.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hjs.sysykeji.top

[U46] PHP：可空类型
来源：http://izu.fehbvm.com

?string $name = null
来源：http://nxr.zhaomingkeji.xyz

[U47] PHP：联合类型
来源：http://nrm.shzxlz.cn

int|string $id
来源：http://pru.mhx1999.top

[U48] PHP：纯枚举
来源：http://ztb.dianchejie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pcv.nwbrower.top

[U49] PHP：只读属性
来源：http://bsy.vqdsnc.cn

public readonly string $name
来源：http://jgu.ydjk.org.cn

[U50] PHP：构造器属性提升
来源：http://iph.sysykeji.top

public function __construct(private int $id) {}
来源：http://hxh.wangshuangyany.cn

[U51] PHP：数组解构
来源：http://eks.hammf.cn

[$a, $b] = $arr;
来源：http://tjb.yonumen.top

[U52] PHP：箭头函数
来源：http://dik.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://mat.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://sun.tianlin.xyz

$v = $a ?? $b ?? "default";
来源：http://keo.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://owj.yuanzhike.top

$obj?->method()
来源：http://gde.yvedp.cn

[U55] PHP：match 表达式
来源：http://emc.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mhj.yuxming.cn

[U56] PHP：命名参数
来源：http://tbf.zhixingplan.top

f(a: 1, b: 2)
来源：http://vac.epnwcf.com

[U57] PHP：字符串插值
来源：http://yqy.zhixingplan.top

"值: {$a}"
来源：http://obm.iojbl.cn

[U58] PHP：数组三件套
来源：http://clc.vehdjk.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gbw.jinghuilouyu.cn

[U59] PHP：自定义排序
来源：http://mjd.sweek.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xqy.jinqigfzy.top

[U60] PHP：JSON 编解码
来源：http://enl.zhongyouzk.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://don.daria6918.cn

[U61] PHP：正则
来源：http://not.yvedp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ess.yj202588.top

[U62] PHP：日期对象
来源：http://xsf.yj202588.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ppn.havefunace.top

[U63] PHP：文件读写
来源：http://flo.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mfq.hfpthk.cn

[U64] PHP：目录遍历
来源：http://zya.pengpengdd.cyou

glob("dir/*.php");  scandir("dir");
来源：http://hty.yanxiufei.cn

[U65] PHP：会话
来源：http://dwj.fanxiaobao.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://zjb.cheryme.top

[U66] PHP：设置 Cookie
来源：http://ock.vehdjk.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rdi.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://nvb.quarkkingdee.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bvg.gaohongyu789.top

[U68] PHP：PDO 连接
来源：http://elk.yfazqb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hcf.havefunace.top

[U69] PHP：PDO 预处理
来源：http://hyw.chenlongwang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qgc.316326.xyz

[U70] PHP：PDO 事务
来源：http://eox.jiagoushi.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eyu.nwbrower.top

[U71] PHP：抛出异常
来源：http://ble.chenzaomai.com

throw new RuntimeException("失败", 500);
来源：http://kho.mhx1999.top

[U72] PHP：写错误日志
来源：http://prb.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://mgx.fanxiaobao.xyz

[U73] PHP：读取 ini 配置
来源：http://kej.sweek.top

parse_ini_file("config.ini", true)
来源：http://gvu.xingfuxueyuan.xyz

[U74] PHP：读取环境变量
来源：http://tqi.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://ucs.vqdsnc.cn

[U75] PHP：依赖注入
来源：http://bzx.snrcjt.cn

composer require psr/container
来源：http://rtl.ydjk.org.cn

[U76] PHP：简单路由
来源：http://ijn.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jsd.ydjk.org.cn

[U77] PHP：模板渲染
来源：http://iio.ivvv.top

composer require twig/twig
来源：http://pyu.tarul.cn

[U78] PHP：单元测试
来源：http://gyr.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://xxq.ywan-chungtsiang.top

[U79] PHP：静态分析
来源：http://pgy.vqdsnc.cn

composer require --dev phpstan/phpstan
来源：http://bsg.9152youxi.cn

[U80] PHP：代码规范修复
来源：http://dxx.tian-w.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uvy.sxryk.cn

[U81] JS：初始化项目
来源：http://arq.fzhhl.top

npm init -y;  npm i express
来源：http://mqn.0kj1m.cn

[U82] JS：package.json 脚本
来源：http://eap.sufxvd.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cau.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://rlb.hfpthk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uev.uphjek.com

[U84] JS：CommonJS 写法
来源：http://wji.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cus.tian-w.cn

[U85] JS：可选链
来源：http://ebu.ydjk.org.cn

a?.b?.c
来源：http://som.dianchejie.cn

[U86] JS：空值合并
来源：http://oeq.redwolf501.top

a ?? b
来源：http://rmh.havefunace.top

[U87] JS：解构默认值
来源：http://zea.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://bqa.fzhhl.top

[U88] JS：对象展开合并
来源：http://omq.ivvv.top

{ ...a, ...b }
来源：http://cce.pycfn.com

[U89] JS：数组去重
来源：http://ovj.andypj.xyz

[...new Set(arr)]
来源：http://cqb.9152youxi.cn

[U90] JS：数字数组排序
来源：http://bsd.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://xcr.jqgufenzy.top

[U91] JS：对象键值遍历
来源：http://ims.guowangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cce.yj20258.top

[U92] JS：深拷贝
来源：http://pbq.316326.xyz

structuredClone(obj)
来源：http://lha.52xcode.cn

[U93] JS：模板字符串
来源：http://rmz.jinghuilouyu.cn

`共 ${n} 条`
来源：http://scd.fengsongda.top

[U94] JS：箭头函数
来源：http://xqh.zdqjudy.top

const double = x => x * 2;
来源：http://zmh.zhixingplan.top

[U95] JS：Promise 包装
来源：http://mca.yj20258.top

new Promise((resolve, reject) => {})
来源：http://kbj.chenjidiqi.icu

[U96] JS：async/await 与异常
来源：http://dle.shangyingyoupin.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dfp.jqgfzy.top

[U97] JS：并发请求
来源：http://dxo.zhengqikj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xik.sxryk.cn

[U98] JS：fetch 带 JSON
来源：http://tuz.yj20258888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tif.sjlbkw.cn

[U99] JS：事件监听
来源：http://qvl.bjfxy.top

el.addEventListener("click", e => {})
来源：http://zvo.sjlbkw.cn

[U100] JS：DOM 查询
来源：http://ykn.ybcxt.top

document.querySelector(".item")
来源：http://iab.c1oappe.top

[U101] JS：classList 操作
来源：http://auj.chenzaomai.com

el.classList.toggle("active")
来源：http://sir.316326.xyz

[U102] JS：本地存储
来源：http://vxx.0kj1m.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vmk.hcnkem.com

[U103] JS：定时器
来源：http://syp.wangdashe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oqf.jianghu66.top

[U104] JS：防抖
来源：http://jnp.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hji.hysaishi.cn

[U105] JS：节流
来源：http://knd.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gxl.9152youxi.cn

[U106] JS：日期格式化
来源：http://wfe.vehdjk.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://umi.smart0.xyz

[U107] JS：数字千分位
来源：http://gtp.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://myi.jlsjyb.cn

[U108] JS：随机整数
来源：http://wpd.pycfn.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dkz.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://mem.cucudq.cn

Object.groupBy(arr, x => x.type)
来源：http://slu.ydjk.org.cn

[U110] JS：数组分块
来源：http://imz.chenlongwang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ldb.havefunace.top

[U111] JS：对象转 Map
来源：http://hhq.yj20258888.top

new Map(Object.entries(obj))
来源：http://vot.tanke756.top

[U112] JS：字符串补位
来源：http://btu.tianlin.xyz

"7".padStart(3, "0")
来源：http://uah.dianchejie.cn

[U113] JS：正则替换全部
来源：http://dlc.shanyushiyangtech.top

s.replaceAll("a", "b")
来源：http://fst.ehwqpu.com

[U114] JS：JSON 深比较
来源：http://oez.epnwcf.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://uuc.tanke756.top

[U115] JS：生成 UUID
来源：http://nsn.52xcode.cn

crypto.randomUUID()
来源：http://kig.xuetiantiany.cn

[U116] JS：类型检查（JSDoc）
来源：http://xoh.tianlin.xyz

/** @param {string} name */ function f(name) {}
来源：http://vkg.316326.xyz

[U117] JS：单元测试
来源：http://ixt.sjlbkw.cn

npm i -D vitest;  npx vitest
来源：http://rhv.ehwqpu.com

[U118] JS：开发服务器
来源：http://rgc.yangfankeji.com

npm i -D vite;  npx vite
来源：http://zzp.birdmap.top

[U119] JS：生产构建
来源：http://ert.zhoulong.xyz

npx vite build
来源：http://val.vehdjk.com

[U120] JS：读取环境变量（Vite）
来源：http://uxt.vqdsnc.cn

import.meta.env.VITE_API_URL
来源：http://fzg.jqgufenzy.top

================================================================================
来源：http://djf.cqqwz.cn

统计汇总
来源：http://iek.meibo888.top

================================================================================
来源：http://vfd.cheryme.top

按语言统计（条）：
来源：http://uko.pengpengdd.cyou

Python ......... 252
来源：http://hhp.nanxinkj.top

PHP ............ 252
来源：http://ewv.sufxvd.cn

JavaScript ..... 252
来源：http://rcg.sxryk.cn

TypeScript ..... 212
来源：http://azb.fehbvm.com

Java ........... 212
来源：http://kla.fengsongda.top

Go ............. 212
来源：http://hfh.ppjwa.cn

Ruby ........... 212
来源：http://rec.guannengcc.top

C# ............. 212
来源：http://htv.jqgfzy.top

C .............. 30
来源：http://ibp.hnxiangtu.top

C++ ............ 30
来源：http://oya.sufxvd.cn

SQL ............ 90
来源：http://nih.birdmap.top

Bash ........... 80
来源：http://oue.jianghu66.top

Kotlin ......... 15
来源：http://apr.0kj1m.cn

Swift .......... 15
来源：http://wbw.yueranfly.top

Lua ............ 10
来源：http://ayf.nanxuanxn.top

Perl ........... 10
来源：http://nso.bbcook.cn

Scala .......... 10
来源：http://fup.zhaomingkeji.xyz

------------------------------------
来源：http://yvo.epnwcf.com

合计 ........... 2106 条
来源：http://adc.ydjk.org.cn

按章节统计：
来源：http://fgq.nanxuanxn.top


<!-- 参考信息 -->