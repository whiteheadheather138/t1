代发 wailian999

[T43] Perl：字符串插值
来源：http://png.dianchejie.cn

"值: $a"
来源：http://nlg.hnxiangtu.top

[T44] Perl：条件
来源：http://cji.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://caz.xinyue.icu

[T45] Perl：数组遍历
来源：http://dso.sjlbkw.cn

for my $x (@arr) { print $x; }
来源：http://wky.iojbl.cn

[T46] Perl：哈希操作
来源：http://anv.daria6918.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lck.shzxlz.cn

[T47] Perl：正则捕获
来源：http://lja.vehdjk.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://cwn.chenlongwang.top

[T48] Perl：正则替换
来源：http://rpy.ehwqpu.com

$s =~ s/old/new/g;
来源：http://ngg.sysykeji.top

[T49] Perl：函数
来源：http://tna.yangfankeji.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bgu.aibaodan.cn

[T50] Perl：逐行读文件
来源：http://xke.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vfx.shanyushiyangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://irb.jinqigfzy.top

[T51] Scala：Hello World
来源：http://siu.ivvv.top

println("Hello")
来源：http://unt.tianlin.xyz

[T52] Scala：变量
来源：http://mht.jiagoushi.top

val a = 1;  var b = 2
来源：http://yzq.xuetiantiany.cn

[T53] Scala：字符串插值
来源：http://ehv.jinqigfzy.top

s"值: $b"
来源：http://auu.yangfankeji.com

[T54] Scala：集合映射
来源：http://wsz.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://hyt.vehdjk.com

[T55] Scala：集合过滤
来源：http://rai.tanke756.top

List(1, 2, 3).filter(_ > 1)
来源：http://ypw.hysaishi.cn

[T56] Scala：样例类
来源：http://ltr.hammf.cn

case class User(name: String, age: Int)
来源：http://phc.chenlongwang.top

[T57] Scala：模式匹配
来源：http://onp.haohaochexian.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mrf.sysykeji.top

[T58] Scala：函数定义
来源：http://hrt.yongpay.top

def add(a: Int, b: Int): Int = a + b
来源：http://vqo.shuidangran.top

[T59] Scala：循环
来源：http://bly.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://kul.feifeiyinyue.top

[T60] Scala：折叠
来源：http://aup.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jtj.52xcode.cn

================================================================================
来源：http://emt.tarul.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gns.ehwqpu.com

================================================================================
来源：http://mdx.ydjk.org.cn

[U01] Py：创建虚拟环境
来源：http://rea.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://bxl.fktsv.cn

[U02] Py：导出 / 安装依赖
来源：http://prv.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nsr.sufxvd.cn

[U03] Py：加载 .env 配置
来源：http://jew.ydjk.org.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ijx.zdbjq.cn

[U04] Py：变量调试打印
来源：http://hee.jqgufenzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hlt.yueranfly.top

[U05] Py：列表去重且保序
来源：http://bju.daria6918.cn

list(dict.fromkeys(arr))
来源：http://xwf.shuidangran.top

[U06] Py：合并两个字典
来源：http://uzn.smart0.xyz

{**a, **b}
来源：http://gox.yj202588.top

[U07] Py：反转字典键值
来源：http://wpz.nwbrower.top

{v: k for k, v in d.items()}
来源：http://cpa.chenlongwang.top

[U08] Py：展平二维列表
来源：http://cks.daria6918.cn

[y for x in nested for y in x]
来源：http://scl.jlsjyb.cn

[U09] Py：字典取最大值的键
来源：http://yrh.shzxlz.cn

max(d, key=d.get)
来源：http://rtv.havefunace.top

[U10] Py：按值排序字典
来源：http://bov.xylfe.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fsx.xziqi.cn

[U11] Py：生成器表达式
来源：http://eof.c1oappe.top

(x * 2 for x in arr)
来源：http://fov.kuanghao11.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ock.aizwys.cn

Counter(arr).most_common(3)
来源：http://lhl.guowangkeji.top

[U13] Py：固定长度队列
来源：http://clq.zhixingplan.top

deque(maxlen=10)
来源：http://pjm.hnxiangtu.top

[U14] Py：分组收集到列表
来源：http://gvj.gotoacloud.top

defaultdict(list)
来源：http://bln.gaohongyu789.top

[U15] Py：高精度计时
来源：http://obq.cheryme.top

t = time.perf_counter()
来源：http://cqp.redwolf501.top

[U16] Py：命令行参数解析
来源：http://gwm.hysaishi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lsk.yanxiufei.cn

[U17] Py：初始化日志
来源：http://ims.shanyushiyangtech.top

logging.basicConfig(level=logging.INFO)
来源：http://nfp.gotoacloud.top

[U18] Py：预编译正则
来源：http://ssg.c1oappe.top

pat = re.compile(r"\d+")
来源：http://ztd.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://hsn.sjlbkw.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hmu.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://obs.tianlin.xyz

@functools.lru_cache(maxsize=None)
来源：http://bkx.ybcxt.top

[U21] Py：自定义上下文管理器
来源：http://oez.jlsjyb.cn

@contextlib.contextmanager
来源：http://niw.jianghu66.top

[U22] Py：矩阵转置
来源：http://wuz.hesvh.cn

list(zip(*m))
来源：http://wya.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://uxe.ehwqpu.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ntn.ydzc1.top

[U24] Py：路径操作
来源：http://oxc.zhixingplan.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hkg.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://gra.jinyuanbaomall.cn

csv.DictReader(f)
来源：http://lfe.9152youxi.cn

[U26] Py：并发下载
来源：http://isd.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oxa.zhoulong.xyz

[U27] Py：异步 HTTP
来源：http://svd.sjlbkw.cn

aiohttp.ClientSession() 配合 async with
来源：http://dbw.jqgufenzy.top

[U28] Py：类型别名
来源：http://bof.ppjwa.cn

UserId = int
来源：http://skt.havefunace.top

[U29] Py：属性校验
来源：http://hdf.ehwqpu.com

@property 与 @x.setter 配合
来源：http://ppm.guowangkeji.top

[U30] Py：数据类
来源：http://tlm.yuxming.cn

@dataclass(slots=True)
来源：http://xfx.c1oappe.top

[U31] Py：单测
来源：http://bvf.chenlongwang.top

python -m pytest -q
来源：http://voo.redwolf501.top

[U32] Py：代码格式化
来源：http://ozg.bbcook.cn

ruff format . && ruff check --fix .
来源：http://pla.tian-w.cn

[U33] Py：打包发布
来源：http://upb.yuanzhike.top

python -m build  （依赖 pyproject.toml）
来源：http://ceb.jlsjyb.cn

[U34] Py：判断编码
来源：http://okq.havefunace.top

chardet.detect(raw)
来源：http://imr.cheryme.top

[U35] Py：发送邮件
来源：http://kit.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://myn.jiagoushi.top

[U36] Py：定时任务
来源：http://iyy.ywan-chungtsiang.top

schedule.every(10).minutes.do(job)
来源：http://vov.xziqi.cn

[U37] Py：读写 Excel
来源：http://jtv.havefunace.top

pandas.read_excel / DataFrame.to_excel
来源：http://nwc.ivvv.top

[U38] Py：获取脚本所在目录
来源：http://wfr.redwolf501.top

Path(__file__).resolve().parent
来源：http://zcd.yj20258.top

[U39] Py：判断是否在交互环境
来源：http://bax.sjlbkw.cn

sys.stdout.isatty()
来源：http://kjv.guannengcc.top

[U40] Py：打印到标准错误
来源：http://cma.fanxiaobao.xyz

print("err", file=sys.stderr)
来源：http://kfs.nwbrower.top

[U41] PHP：初始化 Composer 项目
来源：http://yjy.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://mzw.xuetiantiany.cn

[U42] PHP：PSR-4 自动加载
来源：http://iwm.jlsjyb.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dsr.jinghuilouyu.cn

[U43] PHP：声明命名空间
来源：http://uyj.yj202588.top

namespace App\Http;
来源：http://ngb.ydjk.org.cn

[U44] PHP：开启严格类型
来源：http://cyj.fengsongda.top

declare(strict_types=1);
来源：http://eku.haohaochexian.top

[U45] PHP：类型声明与返回类型
来源：http://tvt.svipenyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fuz.zhongyouzk.top

[U46] PHP：可空类型
来源：http://nov.dianchejie.cn

?string $name = null
来源：http://rto.xingfuxueyuan.xyz

[U47] PHP：联合类型
来源：http://lpz.jqgfzy.top

int|string $id
来源：http://gcc.shzxlz.cn

[U48] PHP：纯枚举
来源：http://aqw.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fzt.vqdsnc.cn

[U49] PHP：只读属性
来源：http://gtb.pengpengdd.cyou

public readonly string $name
来源：http://wos.jinqigufen.top

[U50] PHP：构造器属性提升
来源：http://fwc.sysykeji.top

public function __construct(private int $id) {}
来源：http://hqv.gaohongyu789.top

[U51] PHP：数组解构
来源：http://lil.jiagoushi.top

[$a, $b] = $arr;
来源：http://yrg.zhixingplan.top

[U52] PHP：箭头函数
来源：http://noq.gaohongyu789.top

$double = fn($x) => $x * 2;
来源：http://lje.tanke756.top

[U53] PHP：空合并运算符
来源：http://bob.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://kgi.sjlbkw.cn

[U54] PHP：空安全调用
来源：http://phr.vehdjk.com

$obj?->method()
来源：http://lgs.jyoumei.cn

[U55] PHP：match 表达式
来源：http://iin.hywenlv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pgi.cashguo.top

[U56] PHP：命名参数
来源：http://ftp.jinqigfzy.top

f(a: 1, b: 2)
来源：http://qlq.uphjek.com

[U57] PHP：字符串插值
来源：http://cbu.xuetiantiany.cn

"值: {$a}"
来源：http://fzr.zhixingplan.top

[U58] PHP：数组三件套
来源：http://hiy.guowangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://deq.hfpthk.cn

[U59] PHP：自定义排序
来源：http://fcf.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wiv.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://plo.xuetiantiany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://asr.yongpay.top

[U61] PHP：正则
来源：http://rvm.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://crj.chenzaomai.com

[U62] PHP：日期对象
来源：http://bqn.yuxming.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xko.quarkkingdee.top

[U63] PHP：文件读写
来源：http://vlg.jinyuanbaomall.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hrx.jianghu66.top

[U64] PHP：目录遍历
来源：http://ldt.vehdjk.com

glob("dir/*.php");  scandir("dir");
来源：http://kof.jinghuilouyu.cn

[U65] PHP：会话
来源：http://shf.bjfxy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://twi.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://bvw.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mqa.zhijiandao.cn

[U67] PHP：处理文件上传
来源：http://las.haohaochexian.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dfs.shuidangran.top

[U68] PHP：PDO 连接
来源：http://grj.jinqigfzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ird.iojbl.cn

[U69] PHP：PDO 预处理
来源：http://cmk.yuxming.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bpf.fengsongda.top

[U70] PHP：PDO 事务
来源：http://kyv.jyoumei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hxl.fengsongda.top

[U71] PHP：抛出异常
来源：http://iei.yfazqb.com

throw new RuntimeException("失败", 500);
来源：http://saj.dianchejie.cn

[U72] PHP：写错误日志
来源：http://jcr.vqdsnc.cn

error_log("失败: " . $e->getMessage());
来源：http://aca.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://tkf.0kj1m.cn

parse_ini_file("config.ini", true)
来源：http://zra.bbcook.cn

[U74] PHP：读取环境变量
来源：http://pdf.jianghu66.top

getenv("APP_ENV") ?: "production"
来源：http://geh.aizwys.cn

[U75] PHP：依赖注入
来源：http://lem.aibaodan.cn

composer require psr/container
来源：http://tcq.sweek.top

[U76] PHP：简单路由
来源：http://gwt.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sed.shuidangran.top

[U77] PHP：模板渲染
来源：http://jke.yj20258888.top

composer require twig/twig
来源：http://frm.guannengcc.top

[U78] PHP：单元测试
来源：http://jth.xuanzx.com

composer require --dev phpunit/phpunit
来源：http://fgo.ywan-chungtsiang.top

[U79] PHP：静态分析
来源：http://qrh.cucudq.cn

composer require --dev phpstan/phpstan
来源：http://qky.ydjk.org.cn

[U80] PHP：代码规范修复
来源：http://tcf.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://otm.chenzaomai.com

[U81] JS：初始化项目
来源：http://beo.yj202588.top

npm init -y;  npm i express
来源：http://myc.shzxlz.cn

[U82] JS：package.json 脚本
来源：http://hsq.chenlongwang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vnh.zhoulong.xyz

[U83] JS：ES Module 导入导出
来源：http://cjc.zhoulong.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://jsv.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://odi.yonumen.top

module.exports = { a };  const { a } = require("./m");
来源：http://ynk.andypj.xyz

[U85] JS：可选链
来源：http://yvz.iojbl.cn

a?.b?.c
来源：http://tqo.fehbvm.com

[U86] JS：空值合并
来源：http://kli.haohaochexian.top

a ?? b
来源：http://niu.yonumen.top

[U87] JS：解构默认值
来源：http://idh.zhoulong.xyz

const { a = 1, b = 2 } = obj;
来源：http://cyu.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://dbx.jianghu66.top

{ ...a, ...b }
来源：http://mhm.chenjidiqi.icu

[U89] JS：数组去重
来源：http://oip.chenzaomai.com

[...new Set(arr)]
来源：http://xox.aizwys.cn

[U90] JS：数字数组排序
来源：http://mrr.hnqzz.top

[...arr].sort((a, b) => a - b)
来源：http://jvo.shangyingyoupin.top

[U91] JS：对象键值遍历
来源：http://ydj.ywan-chungtsiang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bkh.cheryme.top

[U92] JS：深拷贝
来源：http://vxo.jlsjyb.cn

structuredClone(obj)
来源：http://xbm.havefunace.top

[U93] JS：模板字符串
来源：http://zmx.xuetiantiany.cn

`共 ${n} 条`
来源：http://czd.wangdashe.top

[U94] JS：箭头函数
来源：http://rei.yanxiufei.cn

const double = x => x * 2;
来源：http://lfs.aizwys.cn

[U95] JS：Promise 包装
来源：http://ygl.fzhhl.top

new Promise((resolve, reject) => {})
来源：http://gwu.hongshengwenyu.top

[U96] JS：async/await 与异常
来源：http://meo.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oum.zdbjq.cn

[U97] JS：并发请求
来源：http://lxq.shanyushiyangtech.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://shy.guannengcc.top

[U98] JS：fetch 带 JSON
来源：http://zux.daxiang520.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://irr.52xcode.cn

[U99] JS：事件监听
来源：http://fin.hammf.cn

el.addEventListener("click", e => {})
来源：http://urp.bjfxy.top

[U100] JS：DOM 查询
来源：http://bkd.bjfxy.top

document.querySelector(".item")
来源：http://wvf.vqdsnc.cn

[U101] JS：classList 操作
来源：http://sqn.aizwys.cn

el.classList.toggle("active")
来源：http://buc.shuidangran.top

[U102] JS：本地存储
来源：http://msk.zhoulong.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://gbd.yuanzhike.top

[U103] JS：定时器
来源：http://zjn.aibaodan.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zwk.yj20258.top

[U104] JS：防抖
来源：http://iea.daxiang520.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rrk.shanyushiyangkeji.top

[U105] JS：节流
来源：http://kir.zdbjq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fcs.zhijiandao.cn

[U106] JS：日期格式化
来源：http://gtu.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sag.vqdsnc.cn

[U107] JS：数字千分位
来源：http://jwh.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://heh.mhx1999.top

[U108] JS：随机整数
来源：http://oyw.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://coq.52xcode.cn

[U109] JS：数组分组
来源：http://cjv.pengpengdd.cyou

Object.groupBy(arr, x => x.type)
来源：http://jrj.hysaishi.cn

[U110] JS：数组分块
来源：http://dmi.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vwf.redwolf501.top

[U111] JS：对象转 Map
来源：http://nja.mhx1999.top

new Map(Object.entries(obj))
来源：http://wso.sweek.top

[U112] JS：字符串补位
来源：http://raw.chenzaomai.com

"7".padStart(3, "0")
来源：http://ahq.wangshuangyany.cn

[U113] JS：正则替换全部
来源：http://jtb.cucudq.cn

s.replaceAll("a", "b")
来源：http://ram.cheryme.top

[U114] JS：JSON 深比较
来源：http://mzc.chenzaomai.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://hlt.aizwys.cn

[U115] JS：生成 UUID
来源：http://vgt.snrcjt.cn

crypto.randomUUID()
来源：http://fdc.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://vzm.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://ecb.chenjidiqi.icu

[U117] JS：单元测试
来源：http://mfq.nanxuanxn.top

npm i -D vitest;  npx vitest
来源：http://ygw.yuanzhike.top

[U118] JS：开发服务器
来源：http://eid.pengpengdd.cyou

npm i -D vite;  npx vite
来源：http://qau.cashguo.top

[U119] JS：生产构建
来源：http://qsq.zhiwuduotai.top

npx vite build
来源：http://yvk.xinyue.icu

[U120] JS：读取环境变量（Vite）
来源：http://kxo.cashguo.top

import.meta.env.VITE_API_URL
来源：http://pbb.jianghu66.top

================================================================================
来源：http://yzl.ehwqpu.com

统计汇总
来源：http://gep.xuanzx.com

================================================================================
来源：http://cyi.dianchejie.cn

按语言统计（条）：
来源：http://ocz.guannengcc.top

Python ......... 252
来源：http://mbs.xziqi.cn

PHP ............ 252
来源：http://phd.hysaishi.cn

JavaScript ..... 252
来源：http://kmx.zhiwuduotai.top

TypeScript ..... 212
来源：http://fad.tanke756.top

Java ........... 212
来源：http://rxp.snrcjt.cn

Go ............. 212
来源：http://ymc.jinghuilouyu.cn

Ruby ........... 212
来源：http://vhy.52xcode.cn

C# ............. 212
来源：http://izo.cdnleiting.top

C .............. 30
来源：http://zcb.yangfankeji.com

C++ ............ 30
来源：http://snb.shuidangran.top

SQL ............ 90
来源：http://aoj.9152youxi.cn

Bash ........... 80
来源：http://bcs.hywenlv.cn

Kotlin ......... 15
来源：http://gru.9152youxi.cn

Swift .......... 15
来源：http://ben.c1oappe.top

Lua ............ 10
来源：http://noo.guannengcc.top

Perl ........... 10
来源：http://qvh.yongpay.top


<!-- 参考信息 -->