代发 wailian999

[T45] Perl：数组遍历
来源：http://glf.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://msm.hysaishi.cn

[T46] Perl：哈希操作
来源：http://fij.sjlbkw.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yib.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://uhw.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bwt.cashguo.top

[T48] Perl：正则替换
来源：http://uxd.ydzc1.top

$s =~ s/old/new/g;
来源：http://fvy.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://tbn.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pzt.jinghuilouyu.cn

[T50] Perl：逐行读文件
来源：http://wpu.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lwh.pengpengdd.cyou

while (my $line = <$fh>) { print $line; }
来源：http://wqz.yj20258888.top

[T51] Scala：Hello World
来源：http://usk.shuidangran.top

println("Hello")
来源：http://akj.bbcook.cn

[T52] Scala：变量
来源：http://qgy.ppjwa.cn

val a = 1;  var b = 2
来源：http://mae.redwolf501.top

[T53] Scala：字符串插值
来源：http://uje.shanyushiyangkeji.top

s"值: $b"
来源：http://ftj.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://nee.ybcxt.top

List(1, 2, 3).map(_ * 2)
来源：http://mzi.316326.xyz

[T55] Scala：集合过滤
来源：http://byv.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://zrw.fengsongda.top

[T56] Scala：样例类
来源：http://bli.pengpengdd.cyou

case class User(name: String, age: Int)
来源：http://wcp.hnqzz.top

[T57] Scala：模式匹配
来源：http://qqp.tarul.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://chy.yonumen.top

[T58] Scala：函数定义
来源：http://lyt.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://gef.yfazqb.com

[T59] Scala：循环
来源：http://tlg.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://uba.nanxuanxn.top

[T60] Scala：折叠
来源：http://nwk.jlsjyb.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wyf.tarul.cn

================================================================================
来源：http://qdf.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aem.chenlongwang.top

================================================================================
来源：http://ctm.jiagoushi.top

[U01] Py：创建虚拟环境
来源：http://mqp.cheryme.top

python -m venv .venv && source .venv/bin/activate
来源：http://gus.daxiang520.top

[U02] Py：导出 / 安装依赖
来源：http://pgp.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nvs.jinyuanbaomall.cn

[U03] Py：加载 .env 配置
来源：http://ljv.sysykeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tda.zhaomingkeji.xyz

[U04] Py：变量调试打印
来源：http://hdh.ppjwa.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bxb.cheryme.top

[U05] Py：列表去重且保序
来源：http://dkw.wangdashe.top

list(dict.fromkeys(arr))
来源：http://qtm.zhixingplan.top

[U06] Py：合并两个字典
来源：http://jqw.tarul.cn

{**a, **b}
来源：http://btq.andypj.xyz

[U07] Py：反转字典键值
来源：http://yyw.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://tfl.bbcook.cn

[U08] Py：展平二维列表
来源：http://mwu.aibaodan.cn

[y for x in nested for y in x]
来源：http://apf.birdmap.top

[U09] Py：字典取最大值的键
来源：http://urw.haohaochexian.top

max(d, key=d.get)
来源：http://psx.ybcxt.top

[U10] Py：按值排序字典
来源：http://fad.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://csv.yuxming.cn

[U11] Py：生成器表达式
来源：http://bfc.guowangkeji.top

(x * 2 for x in arr)
来源：http://bxu.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ysq.quarkkingdee.top

Counter(arr).most_common(3)
来源：http://neu.epnwcf.com

[U13] Py：固定长度队列
来源：http://ltn.fengsongda.top

deque(maxlen=10)
来源：http://cyu.fzhhl.top

[U14] Py：分组收集到列表
来源：http://smh.jinqigufen.top

defaultdict(list)
来源：http://yjl.chenzaomai.com

[U15] Py：高精度计时
来源：http://cad.wangshuangyany.cn

t = time.perf_counter()
来源：http://zpg.yangfankeji.com

[U16] Py：命令行参数解析
来源：http://vae.xuetiantiany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sgb.hysaishi.cn

[U17] Py：初始化日志
来源：http://tav.zhiwuduotai.top

logging.basicConfig(level=logging.INFO)
来源：http://aih.yongpay.top

[U18] Py：预编译正则
来源：http://cfs.hnqzz.top

pat = re.compile(r"\d+")
来源：http://kuc.hnxiangtu.top

[U19] Py：正则替换带回调
来源：http://fft.meibo888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oyr.fktsv.cn

[U20] Py：缓存函数结果
来源：http://sbg.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://twf.yueranfly.top

[U21] Py：自定义上下文管理器
来源：http://fod.shangyingyoupin.top

@contextlib.contextmanager
来源：http://kgc.yangfankeji.com

[U22] Py：矩阵转置
来源：http://osq.hammf.cn

list(zip(*m))
来源：http://faa.yvedp.cn

[U23] Py：分块读取大文件
来源：http://pfd.zycfv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mwc.jinqigufen.top

[U24] Py：路径操作
来源：http://php.xziqi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rje.yonumen.top

[U25] Py：CSV 按字典读
来源：http://qzr.zycfv.cn

csv.DictReader(f)
来源：http://oti.yj20258888.top

[U26] Py：并发下载
来源：http://fty.daxiang520.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nrx.zhaomingkeji.xyz

[U27] Py：异步 HTTP
来源：http://vns.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://tws.zhixingplan.top

[U28] Py：类型别名
来源：http://ffy.chenlongwang.top

UserId = int
来源：http://bym.gzhubu.top

[U29] Py：属性校验
来源：http://mss.tanke756.top

@property 与 @x.setter 配合
来源：http://jlq.ywan-chungtsiang.top

[U30] Py：数据类
来源：http://vlt.hongshengwenyu.top

@dataclass(slots=True)
来源：http://ard.vehdjk.com

[U31] Py：单测
来源：http://qai.316326.xyz

python -m pytest -q
来源：http://tab.hnqzz.top

[U32] Py：代码格式化
来源：http://may.shzxlz.cn

ruff format . && ruff check --fix .
来源：http://zdl.dianchejie.cn

[U33] Py：打包发布
来源：http://ngj.feifeiyinyue.top

python -m build  （依赖 pyproject.toml）
来源：http://qrx.vqdsnc.cn

[U34] Py：判断编码
来源：http://ftb.dashuyun.cn

chardet.detect(raw)
来源：http://kcw.vqdsnc.cn

[U35] Py：发送邮件
来源：http://kdy.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zod.dianchejie.cn

[U36] Py：定时任务
来源：http://txx.yj202588.top

schedule.every(10).minutes.do(job)
来源：http://tge.jqgufenzy.top

[U37] Py：读写 Excel
来源：http://idm.ybcxt.top

pandas.read_excel / DataFrame.to_excel
来源：http://bda.mhx1999.top

[U38] Py：获取脚本所在目录
来源：http://atc.zdqjudy.top

Path(__file__).resolve().parent
来源：http://nap.hongshengwenyu.top

[U39] Py：判断是否在交互环境
来源：http://zmw.hnxiangtu.top

sys.stdout.isatty()
来源：http://pxz.sxryk.cn

[U40] Py：打印到标准错误
来源：http://xxt.gaohongyu789.top

print("err", file=sys.stderr)
来源：http://ruw.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://ckz.yfazqb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://ndx.yuanzhike.top

[U42] PHP：PSR-4 自动加载
来源：http://jzy.hfpthk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wua.chenjidiqi.icu

[U43] PHP：声明命名空间
来源：http://okw.snrcjt.cn

namespace App\Http;
来源：http://qqq.hfpthk.cn

[U44] PHP：开启严格类型
来源：http://hcn.havefunace.top

declare(strict_types=1);
来源：http://nsn.hnqzz.top

[U45] PHP：类型声明与返回类型
来源：http://hhc.ywan-chungtsiang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rbo.ppjwa.cn

[U46] PHP：可空类型
来源：http://fnw.snrcjt.cn

?string $name = null
来源：http://lgr.tian-w.cn

[U47] PHP：联合类型
来源：http://bgi.dianchejie.cn

int|string $id
来源：http://wki.quarkkingdee.top

[U48] PHP：纯枚举
来源：http://fow.yj20258888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://how.havefunace.top

[U49] PHP：只读属性
来源：http://mxs.xziqi.cn

public readonly string $name
来源：http://qnw.shuidangran.top

[U50] PHP：构造器属性提升
来源：http://txb.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://vam.ivvv.top

[U51] PHP：数组解构
来源：http://wrp.hesvh.cn

[$a, $b] = $arr;
来源：http://dpk.shuidangran.top

[U52] PHP：箭头函数
来源：http://ewo.xuetiantiany.cn

$double = fn($x) => $x * 2;
来源：http://lhi.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://qeg.wangshuangyany.cn

$v = $a ?? $b ?? "default";
来源：http://ede.kuanghao11.cn

[U54] PHP：空安全调用
来源：http://pfa.dianchejie.cn

$obj?->method()
来源：http://kcs.aibaodan.cn

[U55] PHP：match 表达式
来源：http://avk.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uvd.quarkkingdee.top

[U56] PHP：命名参数
来源：http://bad.fengsongda.top

f(a: 1, b: 2)
来源：http://kfg.guowangkeji.top

[U57] PHP：字符串插值
来源：http://oqd.nanxuanxn.top

"值: {$a}"
来源：http://lyb.redwolf501.top

[U58] PHP：数组三件套
来源：http://snr.daria6918.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ofa.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://qar.jinqigfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yro.cashguo.top

[U60] PHP：JSON 编解码
来源：http://kbk.nanxuanxn.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zvh.ydzc1.top

[U61] PHP：正则
来源：http://els.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lqj.meibo888.top

[U62] PHP：日期对象
来源：http://emf.zhixingplan.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zxk.fktsv.cn

[U63] PHP：文件读写
来源：http://ean.yanxiufei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xea.pengpengdd.cyou

[U64] PHP：目录遍历
来源：http://oxp.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://ewg.vqdsnc.cn

[U65] PHP：会话
来源：http://ifj.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wue.cqqwz.cn

[U66] PHP：设置 Cookie
来源：http://yys.fehbvm.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rrn.smart0.xyz

[U67] PHP：处理文件上传
来源：http://fkh.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yqj.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://tnu.ivvv.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ssc.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://vst.pengpengdd.cyou

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://utm.andypj.xyz

[U70] PHP：PDO 事务
来源：http://led.hywenlv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pwh.ppjwa.cn

[U71] PHP：抛出异常
来源：http://kdm.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://fza.feifeiyinyue.top

[U72] PHP：写错误日志
来源：http://gil.uphjek.com

error_log("失败: " . $e->getMessage());
来源：http://xiv.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://vlm.dianchejie.cn

parse_ini_file("config.ini", true)
来源：http://hum.chenjidiqi.icu

[U74] PHP：读取环境变量
来源：http://dpi.bbcook.cn

getenv("APP_ENV") ?: "production"
来源：http://cfb.nwbrower.top

[U75] PHP：依赖注入
来源：http://nnw.hongshengwenyu.top

composer require psr/container
来源：http://atj.zhoulong.xyz

[U76] PHP：简单路由
来源：http://pjz.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yph.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://xpu.shuidangran.top

composer require twig/twig
来源：http://ihc.gogol.net.cn

[U78] PHP：单元测试
来源：http://qxg.sufxvd.cn

composer require --dev phpunit/phpunit
来源：http://vgv.zycfv.cn

[U79] PHP：静态分析
来源：http://zcf.jqgufenzy.top

composer require --dev phpstan/phpstan
来源：http://gdu.hongshengwenyu.top

[U80] PHP：代码规范修复
来源：http://lfz.wangshuangyany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ula.svipenyu.cn

[U81] JS：初始化项目
来源：http://hzr.hywenlv.cn

npm init -y;  npm i express
来源：http://qex.aibaodan.cn

[U82] JS：package.json 脚本
来源：http://wzc.ehwqpu.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://raf.xuanzx.com

[U83] JS：ES Module 导入导出
来源：http://gyt.cdnleiting.top

export const a = 1;  import { a } from "./m.js";
来源：http://kae.tianlin.xyz

[U84] JS：CommonJS 写法
来源：http://hsn.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://aun.nwbrower.top

[U85] JS：可选链
来源：http://iuv.tanke756.top

a?.b?.c
来源：http://oyy.gaohongyu789.top

[U86] JS：空值合并
来源：http://hky.guowangkeji.top

a ?? b
来源：http://eax.yj202588.top

[U87] JS：解构默认值
来源：http://saa.chenzaomai.com

const { a = 1, b = 2 } = obj;
来源：http://rhr.jqgufenzy.top

[U88] JS：对象展开合并
来源：http://uwt.sxryk.cn

{ ...a, ...b }
来源：http://vol.yvedp.cn

[U89] JS：数组去重
来源：http://ybk.hcnkem.com

[...new Set(arr)]
来源：http://hll.sysykeji.top

[U90] JS：数字数组排序
来源：http://ilw.ctjpmb.com

[...arr].sort((a, b) => a - b)
来源：http://obr.shzxlz.cn

[U91] JS：对象键值遍历
来源：http://kjy.gotoacloud.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vxn.yvedp.cn

[U92] JS：深拷贝
来源：http://egs.daxiang520.top

structuredClone(obj)
来源：http://lbr.jqgfzy.top

[U93] JS：模板字符串
来源：http://rjz.guannengcc.top

`共 ${n} 条`
来源：http://plo.dashuyun.cn

[U94] JS：箭头函数
来源：http://cai.bbcook.cn

const double = x => x * 2;
来源：http://oqp.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://dar.fzhhl.top

new Promise((resolve, reject) => {})
来源：http://bjh.zhijiandao.cn

[U96] JS：async/await 与异常
来源：http://ipt.yfazqb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vjs.vqdsnc.cn

[U97] JS：并发请求
来源：http://wqr.epnwcf.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://uiy.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://pol.yueranfly.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://exb.yfazqb.com

[U99] JS：事件监听
来源：http://cgi.chenzaomai.com

el.addEventListener("click", e => {})
来源：http://drm.jinghuilouyu.cn

[U100] JS：DOM 查询
来源：http://tni.xylfe.cn

document.querySelector(".item")
来源：http://yvr.vehdjk.com

[U101] JS：classList 操作
来源：http://zpm.wangshuangyany.cn

el.classList.toggle("active")
来源：http://bhr.birdmap.top

[U102] JS：本地存储
来源：http://xuz.gotoacloud.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qmd.haohaochexian.top

[U103] JS：定时器
来源：http://kqg.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bdn.yj20258888.top

[U104] JS：防抖
来源：http://yvn.jinqigfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wsk.cdnleiting.top

[U105] JS：节流
来源：http://smb.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fze.daria6918.cn

[U106] JS：日期格式化
来源：http://pnt.52xcode.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://naz.nanxuanxn.top

[U107] JS：数字千分位
来源：http://erf.yj202588.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tia.ydzc1.top

[U108] JS：随机整数
来源：http://bxa.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yin.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://die.hesvh.cn

Object.groupBy(arr, x => x.type)
来源：http://zgc.hongshengwenyu.top

[U110] JS：数组分块
来源：http://ffo.cucudq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mti.hfpthk.cn

[U111] JS：对象转 Map
来源：http://awp.yueranfly.top

new Map(Object.entries(obj))
来源：http://uki.zdbjq.cn

[U112] JS：字符串补位
来源：http://zri.ydjk.org.cn

"7".padStart(3, "0")
来源：http://oev.hcnkem.com

[U113] JS：正则替换全部
来源：http://fbr.ehwqpu.com

s.replaceAll("a", "b")
来源：http://twt.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://hoz.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rnt.kuanghao11.cn

[U115] JS：生成 UUID
来源：http://wld.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://apb.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://gid.xinyue.icu

/** @param {string} name */ function f(name) {}
来源：http://dfs.cucudq.cn

[U117] JS：单元测试
来源：http://hgp.xuanzx.com

npm i -D vitest;  npx vitest
来源：http://kgt.pengpengdd.cyou

[U118] JS：开发服务器
来源：http://eif.chenzaomai.com

npm i -D vite;  npx vite
来源：http://zxv.zhiwuduotai.top

[U119] JS：生产构建
来源：http://kjf.gzhubu.top

npx vite build
来源：http://ckr.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://fmr.gotoacloud.top

import.meta.env.VITE_API_URL
来源：http://trb.yvedp.cn

================================================================================
来源：http://idr.yangfankeji.com

统计汇总
来源：http://kly.0kj1m.cn

================================================================================
来源：http://urc.daria6918.cn

按语言统计（条）：
来源：http://ifj.vehdjk.com

Python ......... 252
来源：http://zgo.yuxming.cn

PHP ............ 252
来源：http://kwh.quarkkingdee.top

JavaScript ..... 252
来源：http://rkb.gaohongyu789.top

TypeScript ..... 212
来源：http://jwv.0kj1m.cn

Java ........... 212
来源：http://trb.jyoumei.cn

Go ............. 212
来源：http://ihi.nwbrower.top

Ruby ........... 212
来源：http://tfa.xinyue.icu

C# ............. 212
来源：http://zjr.pengpengdd.cyou

C .............. 30
来源：http://ycs.yuanzhike.top

C++ ............ 30
来源：http://ead.chenzaomai.com

SQL ............ 90
来源：http://mhk.pengpengdd.cyou

Bash ........... 80
来源：http://rgc.andypj.xyz

Kotlin ......... 15
来源：http://imn.andypj.xyz

Swift .......... 15
来源：http://ddd.yj202588.top

Lua ............ 10
来源：http://zux.gaohongyu789.top

Perl ........... 10
来源：http://drn.shangyingyoupin.top

Scala .......... 10
来源：http://uyw.andypj.xyz

------------------------------------
来源：http://jwv.zhixingplan.top

合计 ........... 2106 条
来源：http://iqc.mhx1999.top

按章节统计：
来源：http://wck.sjlbkw.cn


<!-- 参考信息 -->