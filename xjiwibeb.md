代发 wailian999

[T45] Perl：数组遍历
来源：http://ckm.jqgfzy.top

for my $x (@arr) { print $x; }
来源：http://rxd.vqdsnc.cn

[T46] Perl：哈希操作
来源：http://day.hcnkem.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qwc.ehwqpu.com

[T47] Perl：正则捕获
来源：http://ylp.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hsw.jyoumei.cn

[T48] Perl：正则替换
来源：http://ipz.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://eou.snrcjt.cn

[T49] Perl：函数
来源：http://bkw.fzhhl.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ief.guowangkeji.top

[T50] Perl：逐行读文件
来源：http://igx.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vpl.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://yft.jqgufenzy.top

[T51] Scala：Hello World
来源：http://wje.tarul.cn

println("Hello")
来源：http://jwq.xingfuxueyuan.xyz

[T52] Scala：变量
来源：http://zha.zhijiandao.cn

val a = 1;  var b = 2
来源：http://cms.hesvh.cn

[T53] Scala：字符串插值
来源：http://six.chenlongwang.top

s"值: $b"
来源：http://kkh.xziqi.cn

[T54] Scala：集合映射
来源：http://abk.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://jnk.52xcode.cn

[T55] Scala：集合过滤
来源：http://myc.aizwys.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bdc.cucudq.cn

[T56] Scala：样例类
来源：http://bhz.yj20258.top

case class User(name: String, age: Int)
来源：http://llj.haohaochexian.top

[T57] Scala：模式匹配
来源：http://lrb.quarkkingdee.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kkg.zhijiandao.cn

[T58] Scala：函数定义
来源：http://tpz.tian-w.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bwh.chenlongwang.top

[T59] Scala：循环
来源：http://ecd.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://qxc.xuetiantiany.cn

[T60] Scala：折叠
来源：http://pfe.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://foi.sufxvd.cn

================================================================================
来源：http://stg.jinghuilouyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kjn.hcnkem.com

================================================================================
来源：http://shk.jqgfzy.top

[U01] Py：创建虚拟环境
来源：http://iwo.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://hyx.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://ukd.fanxiaobao.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wbj.gzhubu.top

[U03] Py：加载 .env 配置
来源：http://yhh.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://grp.bbcook.cn

[U04] Py：变量调试打印
来源：http://xhs.zhijiandao.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eko.kuanghao11.cn

[U05] Py：列表去重且保序
来源：http://zuy.snrcjt.cn

list(dict.fromkeys(arr))
来源：http://uef.yfazqb.com

[U06] Py：合并两个字典
来源：http://tsy.hammf.cn

{**a, **b}
来源：http://rkf.iojbl.cn

[U07] Py：反转字典键值
来源：http://wob.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://llk.redwolf501.top

[U08] Py：展平二维列表
来源：http://nye.fzhhl.top

[y for x in nested for y in x]
来源：http://yee.zhixingplan.top

[U09] Py：字典取最大值的键
来源：http://byd.hesvh.cn

max(d, key=d.get)
来源：http://uwn.yuanzhike.top

[U10] Py：按值排序字典
来源：http://fjz.yangfankeji.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pyk.vqdsnc.cn

[U11] Py：生成器表达式
来源：http://xqc.aizwys.cn

(x * 2 for x in arr)
来源：http://jqh.yuanzhike.top

[U12] Py：取出现最多的 3 个元素
来源：http://tjh.zhaomingkeji.xyz

Counter(arr).most_common(3)
来源：http://pxc.aibaodan.cn

[U13] Py：固定长度队列
来源：http://uve.vehdjk.com

deque(maxlen=10)
来源：http://zvn.yj20258888.top

[U14] Py：分组收集到列表
来源：http://msr.ywan-chungtsiang.top

defaultdict(list)
来源：http://vbd.aizwys.cn

[U15] Py：高精度计时
来源：http://gyc.fanxiaobao.xyz

t = time.perf_counter()
来源：http://diz.xziqi.cn

[U16] Py：命令行参数解析
来源：http://fql.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rlg.yfazqb.com

[U17] Py：初始化日志
来源：http://ubl.ppjwa.cn

logging.basicConfig(level=logging.INFO)
来源：http://cdj.cucudq.cn

[U18] Py：预编译正则
来源：http://cqu.svipenyu.cn

pat = re.compile(r"\d+")
来源：http://xds.c1oappe.top

[U19] Py：正则替换带回调
来源：http://mxs.guannengcc.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://faa.redwolf501.top

[U20] Py：缓存函数结果
来源：http://uvu.shuidangran.top

@functools.lru_cache(maxsize=None)
来源：http://ias.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://wnm.mhx1999.top

@contextlib.contextmanager
来源：http://lmk.yuxming.cn

[U22] Py：矩阵转置
来源：http://thi.hnqzz.top

list(zip(*m))
来源：http://ify.chenjidiqi.icu

[U23] Py：分块读取大文件
来源：http://xis.yanxiufei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dlm.wangdashe.top

[U24] Py：路径操作
来源：http://ucc.zhongyouzk.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qfm.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://ybk.sysykeji.top

csv.DictReader(f)
来源：http://tmf.zhengqikj.top

[U26] Py：并发下载
来源：http://lgk.snrcjt.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yzk.snrcjt.cn

[U27] Py：异步 HTTP
来源：http://arx.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://iwn.sweek.top

[U28] Py：类型别名
来源：http://uli.gogol.net.cn

UserId = int
来源：http://nqs.shanyushiyangtech.top

[U29] Py：属性校验
来源：http://bcl.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://rkb.shangyingyoupin.top

[U30] Py：数据类
来源：http://jgy.zhixingplan.top

@dataclass(slots=True)
来源：http://ypm.zdbjq.cn

[U31] Py：单测
来源：http://bxy.yongpay.top

python -m pytest -q
来源：http://uxg.dashuyun.cn

[U32] Py：代码格式化
来源：http://qkl.guannengcc.top

ruff format . && ruff check --fix .
来源：http://afl.fanxiaobao.xyz

[U33] Py：打包发布
来源：http://fyd.yangfankeji.com

python -m build  （依赖 pyproject.toml）
来源：http://ljr.guannengcc.top

[U34] Py：判断编码
来源：http://ycr.hnxiangtu.top

chardet.detect(raw)
来源：http://mxf.daxiang520.top

[U35] Py：发送邮件
来源：http://zll.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fpl.yanxiufei.cn

[U36] Py：定时任务
来源：http://xfo.fzhhl.top

schedule.every(10).minutes.do(job)
来源：http://zzo.havefunace.top

[U37] Py：读写 Excel
来源：http://cew.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://djk.jinqigfzy.top

[U38] Py：获取脚本所在目录
来源：http://prr.ehwqpu.com

Path(__file__).resolve().parent
来源：http://cyi.zhongyouzk.top

[U39] Py：判断是否在交互环境
来源：http://paa.hcnkem.com

sys.stdout.isatty()
来源：http://xpm.fanxiaobao.xyz

[U40] Py：打印到标准错误
来源：http://jjx.dashuyun.cn

print("err", file=sys.stderr)
来源：http://biw.hcnkem.com

[U41] PHP：初始化 Composer 项目
来源：http://lyp.nanxuanxn.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qmo.ydzc1.top

[U42] PHP：PSR-4 自动加载
来源：http://eqg.yueranfly.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cjg.xziqi.cn

[U43] PHP：声明命名空间
来源：http://stg.aizwys.cn

namespace App\Http;
来源：http://lip.yj20258888.top

[U44] PHP：开启严格类型
来源：http://jcx.jlsjyb.cn

declare(strict_types=1);
来源：http://wwf.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://slc.bjfxy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ada.guannengcc.top

[U46] PHP：可空类型
来源：http://hxi.fengsongda.top

?string $name = null
来源：http://vbj.yj20258.top

[U47] PHP：联合类型
来源：http://sgd.zhijiandao.cn

int|string $id
来源：http://bby.fengsongda.top

[U48] PHP：纯枚举
来源：http://gzp.shangyingyoupin.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ydi.daria6918.cn

[U49] PHP：只读属性
来源：http://aeq.pycfn.com

public readonly string $name
来源：http://hci.sxryk.cn

[U50] PHP：构造器属性提升
来源：http://utg.jianghu66.top

public function __construct(private int $id) {}
来源：http://qus.yangfankeji.com

[U51] PHP：数组解构
来源：http://hjf.gotoacloud.top

[$a, $b] = $arr;
来源：http://zga.zhixingplan.top

[U52] PHP：箭头函数
来源：http://vss.ivvv.top

$double = fn($x) => $x * 2;
来源：http://mud.jyoumei.cn

[U53] PHP：空合并运算符
来源：http://okq.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://foo.xuanzx.com

[U54] PHP：空安全调用
来源：http://mba.316326.xyz

$obj?->method()
来源：http://hym.yvedp.cn

[U55] PHP：match 表达式
来源：http://lnd.hfpthk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mxt.sweek.top

[U56] PHP：命名参数
来源：http://qaw.xylfe.cn

f(a: 1, b: 2)
来源：http://kqz.pengpengdd.cyou

[U57] PHP：字符串插值
来源：http://tsc.xziqi.cn

"值: {$a}"
来源：http://lva.guannengcc.top

[U58] PHP：数组三件套
来源：http://mjf.c1oappe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cla.0kj1m.cn

[U59] PHP：自定义排序
来源：http://ndd.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://npz.zdbjq.cn

[U60] PHP：JSON 编解码
来源：http://zrm.havefunace.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cqr.ehwqpu.com

[U61] PHP：正则
来源：http://mtv.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dio.feifeiyinyue.top

[U62] PHP：日期对象
来源：http://yvh.svipenyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ldg.52xcode.cn

[U63] PHP：文件读写
来源：http://oca.chenzaomai.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hay.jinghuilouyu.cn

[U64] PHP：目录遍历
来源：http://tka.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://ibj.andypj.xyz

[U65] PHP：会话
来源：http://bml.pengpengdd.cyou

session_start();  $_SESSION["uid"] = 1;
来源：http://kly.wangshuangyany.cn

[U66] PHP：设置 Cookie
来源：http://ebw.pycfn.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lis.fanxiaobao.xyz

[U67] PHP：处理文件上传
来源：http://bmo.hesvh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dyh.tanke756.top

[U68] PHP：PDO 连接
来源：http://gal.sjlbkw.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hek.dianchejie.cn

[U69] PHP：PDO 预处理
来源：http://kwp.zhixingplan.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rto.yvedp.cn

[U70] PHP：PDO 事务
来源：http://tgp.haohaochexian.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zaq.jinqigufen.top

[U71] PHP：抛出异常
来源：http://rmk.yfazqb.com

throw new RuntimeException("失败", 500);
来源：http://isg.xuetiantiany.cn

[U72] PHP：写错误日志
来源：http://kvs.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://xzb.shuidangran.top

[U73] PHP：读取 ini 配置
来源：http://rdr.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://dhs.zhijiandao.cn

[U74] PHP：读取环境变量
来源：http://cjo.yongpay.top

getenv("APP_ENV") ?: "production"
来源：http://auf.yj20258.top

[U75] PHP：依赖注入
来源：http://zfy.hnxiangtu.top

composer require psr/container
来源：http://akb.haohaochexian.top

[U76] PHP：简单路由
来源：http://jjn.pengpengdd.cyou

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jgr.tian-w.cn

[U77] PHP：模板渲染
来源：http://izw.shuidangran.top

composer require twig/twig
来源：http://qfm.316326.xyz

[U78] PHP：单元测试
来源：http://fgn.redwolf501.top

composer require --dev phpunit/phpunit
来源：http://eov.dashuyun.cn

[U79] PHP：静态分析
来源：http://zqt.9152youxi.cn

composer require --dev phpstan/phpstan
来源：http://gwr.xinyue.icu

[U80] PHP：代码规范修复
来源：http://ckv.guannengcc.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://khm.hfpthk.cn

[U81] JS：初始化项目
来源：http://ynn.gogol.net.cn

npm init -y;  npm i express
来源：http://mvn.cucudq.cn

[U82] JS：package.json 脚本
来源：http://sbn.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pgc.svipenyu.cn

[U83] JS：ES Module 导入导出
来源：http://lts.ybcxt.top

export const a = 1;  import { a } from "./m.js";
来源：http://wmj.quarkkingdee.top

[U84] JS：CommonJS 写法
来源：http://uoo.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mnw.yangfankeji.com

[U85] JS：可选链
来源：http://hlc.zhiwuduotai.top

a?.b?.c
来源：http://vyo.jinyuanbaomall.cn

[U86] JS：空值合并
来源：http://pix.ydjk.org.cn

a ?? b
来源：http://hsb.redwolf501.top

[U87] JS：解构默认值
来源：http://ewz.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://wwb.jinqigufen.top

[U88] JS：对象展开合并
来源：http://hbx.vehdjk.com

{ ...a, ...b }
来源：http://ahf.shuidangran.top

[U89] JS：数组去重
来源：http://itk.tarul.cn

[...new Set(arr)]
来源：http://tuv.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://vkg.gaohongyu789.top

[...arr].sort((a, b) => a - b)
来源：http://rlf.tian-w.cn

[U91] JS：对象键值遍历
来源：http://jxc.cucudq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vld.yvedp.cn

[U92] JS：深拷贝
来源：http://bhn.zhaomingkeji.xyz

structuredClone(obj)
来源：http://xuo.sjlbkw.cn

[U93] JS：模板字符串
来源：http://igh.zhoulong.xyz

`共 ${n} 条`
来源：http://lcc.fanxiaobao.xyz

[U94] JS：箭头函数
来源：http://zby.jianghu66.top

const double = x => x * 2;
来源：http://xqw.dianchejie.cn

[U95] JS：Promise 包装
来源：http://vsi.nwbrower.top

new Promise((resolve, reject) => {})
来源：http://nwk.xylfe.cn

[U96] JS：async/await 与异常
来源：http://nrb.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hcp.shuidangran.top

[U97] JS：并发请求
来源：http://yfb.quarkkingdee.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zwl.jlsjyb.cn

[U98] JS：fetch 带 JSON
来源：http://elf.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wrv.sufxvd.cn

[U99] JS：事件监听
来源：http://lla.gogol.net.cn

el.addEventListener("click", e => {})
来源：http://rqj.yangfankeji.com

[U100] JS：DOM 查询
来源：http://ydq.ydzc1.top

document.querySelector(".item")
来源：http://jzr.jinqigufen.top

[U101] JS：classList 操作
来源：http://jka.kuanghao11.cn

el.classList.toggle("active")
来源：http://iez.chenzaomai.com

[U102] JS：本地存储
来源：http://dnj.xuetiantiany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://utm.jinqigufen.top

[U103] JS：定时器
来源：http://ewx.nanxuanxn.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ajq.jlsjyb.cn

[U104] JS：防抖
来源：http://shd.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vpo.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://ebm.hywenlv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bfn.jyoumei.cn

[U106] JS：日期格式化
来源：http://mqd.guannengcc.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ksj.jinqigufen.top

[U107] JS：数字千分位
来源：http://wsy.shanyushiyangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://acv.zhoulong.xyz

[U108] JS：随机整数
来源：http://pbg.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eoa.ybcxt.top

[U109] JS：数组分组
来源：http://bge.jianghu66.top

Object.groupBy(arr, x => x.type)
来源：http://ltv.0kj1m.cn

[U110] JS：数组分块
来源：http://sjk.zhijiandao.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nnj.yj20258.top

[U111] JS：对象转 Map
来源：http://jyo.yangfankeji.com

new Map(Object.entries(obj))
来源：http://ire.zhoulong.xyz

[U112] JS：字符串补位
来源：http://tgq.gogol.net.cn

"7".padStart(3, "0")
来源：http://jny.zhiwuduotai.top

[U113] JS：正则替换全部
来源：http://nyh.havefunace.top

s.replaceAll("a", "b")
来源：http://czj.xylfe.cn

[U114] JS：JSON 深比较
来源：http://lzf.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uzb.xziqi.cn

[U115] JS：生成 UUID
来源：http://rsq.wangdashe.top

crypto.randomUUID()
来源：http://rit.shzxlz.cn

[U116] JS：类型检查（JSDoc）
来源：http://pmd.gotoacloud.top

/** @param {string} name */ function f(name) {}
来源：http://htg.shanyushiyangkeji.top

[U117] JS：单元测试
来源：http://ges.tanke756.top

npm i -D vitest;  npx vitest
来源：http://jie.fanxiaobao.xyz

[U118] JS：开发服务器
来源：http://mxs.hnqzz.top

npm i -D vite;  npx vite
来源：http://llz.ppjwa.cn

[U119] JS：生产构建
来源：http://luv.cashguo.top

npx vite build
来源：http://rjl.pycfn.com

[U120] JS：读取环境变量（Vite）
来源：http://nes.hongshengwenyu.top

import.meta.env.VITE_API_URL
来源：http://qsf.jqgufenzy.top

================================================================================
来源：http://zoc.redwolf501.top

统计汇总
来源：http://gcg.tianlin.xyz

================================================================================
来源：http://fef.jinqigufen.top

按语言统计（条）：
来源：http://bja.jinqigufen.top

Python ......... 252
来源：http://qsh.zhengqikj.top

PHP ............ 252
来源：http://jhq.nanxinkj.top

JavaScript ..... 252
来源：http://eqd.snrcjt.cn

TypeScript ..... 212
来源：http://aih.hcnkem.com

Java ........... 212
来源：http://vht.yuxming.cn

Go ............. 212
来源：http://opu.fktsv.cn

Ruby ........... 212
来源：http://byp.zdbjq.cn

C# ............. 212
来源：http://zyg.cashguo.top

C .............. 30
来源：http://ktw.tarul.cn

C++ ............ 30
来源：http://nke.sjlbkw.cn

SQL ............ 90
来源：http://btu.xuetiantiany.cn

Bash ........... 80
来源：http://zez.yj202588.top

Kotlin ......... 15
来源：http://asm.cdnleiting.top

Swift .......... 15
来源：http://mce.guowangkeji.top

Lua ............ 10
来源：http://ngd.shanyushiyangkeji.top

Perl ........... 10
来源：http://zbx.bbcook.cn

Scala .......... 10
来源：http://mnd.tarul.cn

------------------------------------
来源：http://lmp.uphjek.com

合计 ........... 2106 条
来源：http://gbf.sjlbkw.cn

按章节统计：
来源：http://gya.xingfuxueyuan.xyz


<!-- 参考信息 -->