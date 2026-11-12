代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eft.iojbl.cn

================================================================================
来源：http://cbq.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://duz.mhx1999.top

================================================================================
来源：http://ayl.nwbrower.top

[U01] Py：创建虚拟环境
来源：http://qur.andypj.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://hya.quarkkingdee.top

[U02] Py：导出 / 安装依赖
来源：http://hcs.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ezn.jyoumei.cn

[U03] Py：加载 .env 配置
来源：http://utj.zhijiandao.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://psk.ivvv.top

[U04] Py：变量调试打印
来源：http://xmr.daria6918.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lpk.jinghuilouyu.cn

[U05] Py：列表去重且保序
来源：http://rol.nanxinkj.top

list(dict.fromkeys(arr))
来源：http://gbq.birdmap.top

[U06] Py：合并两个字典
来源：http://smp.hnqzz.top

{**a, **b}
来源：http://vyd.tianlin.xyz

[U07] Py：反转字典键值
来源：http://sxf.zhaomingkeji.xyz

{v: k for k, v in d.items()}
来源：http://sda.epnwcf.com

[U08] Py：展平二维列表
来源：http://yru.yuxming.cn

[y for x in nested for y in x]
来源：http://lyf.vehdjk.com

[U09] Py：字典取最大值的键
来源：http://scm.smart0.xyz

max(d, key=d.get)
来源：http://joy.yonumen.top

[U10] Py：按值排序字典
来源：http://ont.yanxiufei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nxn.aizwys.cn

[U11] Py：生成器表达式
来源：http://usk.jiagoushi.top

(x * 2 for x in arr)
来源：http://ppm.birdmap.top

[U12] Py：取出现最多的 3 个元素
来源：http://odb.dianchejie.cn

Counter(arr).most_common(3)
来源：http://ujv.316326.xyz

[U13] Py：固定长度队列
来源：http://ysp.hnqzz.top

deque(maxlen=10)
来源：http://sfn.feifeiyinyue.top

[U14] Py：分组收集到列表
来源：http://kia.yonumen.top

defaultdict(list)
来源：http://bjn.tarul.cn

[U15] Py：高精度计时
来源：http://eia.zhijiandao.cn

t = time.perf_counter()
来源：http://qxn.wangshuangyany.cn

[U16] Py：命令行参数解析
来源：http://pdn.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jwk.hcnkem.com

[U17] Py：初始化日志
来源：http://wcd.shanyushiyangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://kcb.guannengcc.top

[U18] Py：预编译正则
来源：http://stx.hammf.cn

pat = re.compile(r"\d+")
来源：http://zvg.mhx1999.top

[U19] Py：正则替换带回调
来源：http://uqk.yuanzhike.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vpq.kuanghao11.cn

[U20] Py：缓存函数结果
来源：http://irp.sufxvd.cn

@functools.lru_cache(maxsize=None)
来源：http://iji.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://nrt.iojbl.cn

@contextlib.contextmanager
来源：http://nxd.sufxvd.cn

[U22] Py：矩阵转置
来源：http://oyc.ehwqpu.com

list(zip(*m))
来源：http://xob.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://nkb.jqgfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gcn.ydjk.org.cn

[U24] Py：路径操作
来源：http://uye.svipenyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ltb.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://lvk.yangfankeji.com

csv.DictReader(f)
来源：http://lsw.hnxiangtu.top

[U26] Py：并发下载
来源：http://jin.wangdashe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wjq.jianghu66.top

[U27] Py：异步 HTTP
来源：http://yub.zhongyouzk.top

aiohttp.ClientSession() 配合 async with
来源：http://shq.ivvv.top

[U28] Py：类型别名
来源：http://gsm.xziqi.cn

UserId = int
来源：http://xne.xingfuxueyuan.xyz

[U29] Py：属性校验
来源：http://frw.cucudq.cn

@property 与 @x.setter 配合
来源：http://gdx.fehbvm.com

[U30] Py：数据类
来源：http://dtw.zhaomingkeji.xyz

@dataclass(slots=True)
来源：http://gom.ctjpmb.com

[U31] Py：单测
来源：http://ods.ppjwa.cn

python -m pytest -q
来源：http://und.haohaochexian.top

[U32] Py：代码格式化
来源：http://gra.yonumen.top

ruff format . && ruff check --fix .
来源：http://vjk.epnwcf.com

[U33] Py：打包发布
来源：http://vrp.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://wgw.hesvh.cn

[U34] Py：判断编码
来源：http://oge.yangfankeji.com

chardet.detect(raw)
来源：http://bdm.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://pdd.fengsongda.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ssg.epnwcf.com

[U36] Py：定时任务
来源：http://vax.yvedp.cn

schedule.every(10).minutes.do(job)
来源：http://yiz.yj20258888.top

[U37] Py：读写 Excel
来源：http://eff.zhixingplan.top

pandas.read_excel / DataFrame.to_excel
来源：http://kjz.aibaodan.cn

[U38] Py：获取脚本所在目录
来源：http://rgu.ydjk.org.cn

Path(__file__).resolve().parent
来源：http://ujv.ydzc1.top

[U39] Py：判断是否在交互环境
来源：http://pjh.cdnleiting.top

sys.stdout.isatty()
来源：http://ktg.fehbvm.com

[U40] Py：打印到标准错误
来源：http://owg.redwolf501.top

print("err", file=sys.stderr)
来源：http://ldi.cheryme.top

[U41] PHP：初始化 Composer 项目
来源：http://pqa.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wea.yangfankeji.com

[U42] PHP：PSR-4 自动加载
来源：http://tuw.bjfxy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://osm.xuanzx.com

[U43] PHP：声明命名空间
来源：http://gsp.wangdashe.top

namespace App\Http;
来源：http://bkq.birdmap.top

[U44] PHP：开启严格类型
来源：http://sbf.redwolf501.top

declare(strict_types=1);
来源：http://lmk.tanke756.top

[U45] PHP：类型声明与返回类型
来源：http://ctf.jqgufenzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qcf.sufxvd.cn

[U46] PHP：可空类型
来源：http://lfi.epnwcf.com

?string $name = null
来源：http://bch.svipenyu.cn

[U47] PHP：联合类型
来源：http://twq.dianchejie.cn

int|string $id
来源：http://qtu.hesvh.cn

[U48] PHP：纯枚举
来源：http://evy.hysaishi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://idp.jlsjyb.cn

[U49] PHP：只读属性
来源：http://lrj.zhiwuduotai.top

public readonly string $name
来源：http://ipe.9152youxi.cn

[U50] PHP：构造器属性提升
来源：http://lqg.tanke756.top

public function __construct(private int $id) {}
来源：http://vbw.sjlbkw.cn

[U51] PHP：数组解构
来源：http://mie.yongpay.top

[$a, $b] = $arr;
来源：http://kaw.uphjek.com

[U52] PHP：箭头函数
来源：http://ppu.c1oappe.top

$double = fn($x) => $x * 2;
来源：http://cdr.fanxiaobao.xyz

[U53] PHP：空合并运算符
来源：http://hjn.zhoulong.xyz

$v = $a ?? $b ?? "default";
来源：http://ofu.hcnkem.com

[U54] PHP：空安全调用
来源：http://irr.fanxiaobao.xyz

$obj?->method()
来源：http://yrb.wangshuangyany.cn

[U55] PHP：match 表达式
来源：http://fei.bjfxy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yoq.guowangkeji.top

[U56] PHP：命名参数
来源：http://vqf.zhijiandao.cn

f(a: 1, b: 2)
来源：http://ovb.jyoumei.cn

[U57] PHP：字符串插值
来源：http://jtu.zhijiandao.cn

"值: {$a}"
来源：http://rcm.jinyuanbaomall.cn

[U58] PHP：数组三件套
来源：http://qok.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lhr.shanyushiyangtech.top

[U59] PHP：自定义排序
来源：http://zga.epnwcf.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jtr.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://hpq.zhixingplan.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fpa.cheryme.top

[U61] PHP：正则
来源：http://dll.nanxinkj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rkp.jianghu66.top

[U62] PHP：日期对象
来源：http://buf.vehdjk.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qga.zhengqikj.top

[U63] PHP：文件读写
来源：http://ykp.yj202588.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lgj.dianchejie.cn

[U64] PHP：目录遍历
来源：http://cxt.gotoacloud.top

glob("dir/*.php");  scandir("dir");
来源：http://eau.ivvv.top

[U65] PHP：会话
来源：http://laq.redwolf501.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nea.yuxming.cn

[U66] PHP：设置 Cookie
来源：http://dqf.tanke756.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nrf.andypj.xyz

[U67] PHP：处理文件上传
来源：http://aqj.fanxiaobao.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ntp.jlsjyb.cn

[U68] PHP：PDO 连接
来源：http://rpk.hnqzz.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bas.cheryme.top

[U69] PHP：PDO 预处理
来源：http://ctz.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dhc.smart0.xyz

[U70] PHP：PDO 事务
来源：http://uhg.birdmap.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://col.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://ppr.jqgfzy.top

throw new RuntimeException("失败", 500);
来源：http://mkd.zycfv.cn

[U72] PHP：写错误日志
来源：http://bde.guannengcc.top

error_log("失败: " . $e->getMessage());
来源：http://dmp.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://qyh.zdbjq.cn

parse_ini_file("config.ini", true)
来源：http://drc.meibo888.top

[U74] PHP：读取环境变量
来源：http://mql.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://jij.vqdsnc.cn

[U75] PHP：依赖注入
来源：http://vuo.fehbvm.com

composer require psr/container
来源：http://hff.pengpengdd.cyou

[U76] PHP：简单路由
来源：http://wjf.sjlbkw.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://top.mhx1999.top

[U77] PHP：模板渲染
来源：http://gge.xuanzx.com

composer require twig/twig
来源：http://zmn.zhiwuduotai.top

[U78] PHP：单元测试
来源：http://mkk.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://mxt.0kj1m.cn

[U79] PHP：静态分析
来源：http://tjh.feifeiyinyue.top

composer require --dev phpstan/phpstan
来源：http://uft.hongshengwenyu.top

[U80] PHP：代码规范修复
来源：http://tij.sysykeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jnn.ehwqpu.com

[U81] JS：初始化项目
来源：http://aup.gotoacloud.top

npm init -y;  npm i express
来源：http://ifm.daria6918.cn

[U82] JS：package.json 脚本
来源：http://zkv.cdnleiting.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gqo.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://juy.xingfuxueyuan.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://vwv.xinyue.icu

[U84] JS：CommonJS 写法
来源：http://xpy.sysykeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://dxm.hammf.cn

[U85] JS：可选链
来源：http://ten.hnxiangtu.top

a?.b?.c
来源：http://ttp.shuidangran.top

[U86] JS：空值合并
来源：http://zgg.ppjwa.cn

a ?? b
来源：http://xwv.yj202588.top

[U87] JS：解构默认值
来源：http://fmx.jinqigfzy.top

const { a = 1, b = 2 } = obj;
来源：http://njn.dashuyun.cn

[U88] JS：对象展开合并
来源：http://egp.kuanghao11.cn

{ ...a, ...b }
来源：http://bde.bbcook.cn

[U89] JS：数组去重
来源：http://kqo.jlsjyb.cn

[...new Set(arr)]
来源：http://cdv.tarul.cn

[U90] JS：数字数组排序
来源：http://uff.sufxvd.cn

[...arr].sort((a, b) => a - b)
来源：http://esa.hesvh.cn

[U91] JS：对象键值遍历
来源：http://rbp.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ijm.yuxming.cn

[U92] JS：深拷贝
来源：http://khn.sjlbkw.cn

structuredClone(obj)
来源：http://dcn.tian-w.cn

[U93] JS：模板字符串
来源：http://zqv.feifeiyinyue.top

`共 ${n} 条`
来源：http://juj.nanxinkj.top

[U94] JS：箭头函数
来源：http://osb.jianghu66.top

const double = x => x * 2;
来源：http://jgf.yueranfly.top

[U95] JS：Promise 包装
来源：http://rou.ivvv.top

new Promise((resolve, reject) => {})
来源：http://qvz.dianchejie.cn

[U96] JS：async/await 与异常
来源：http://pdh.feifeiyinyue.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://obq.bjfxy.top

[U97] JS：并发请求
来源：http://zqu.fehbvm.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://bmd.pycfn.com

[U98] JS：fetch 带 JSON
来源：http://czz.xuetiantiany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gps.hfpthk.cn

[U99] JS：事件监听
来源：http://kzd.fengsongda.top

el.addEventListener("click", e => {})
来源：http://rgb.fktsv.cn

[U100] JS：DOM 查询
来源：http://qly.0kj1m.cn

document.querySelector(".item")
来源：http://joc.316326.xyz

[U101] JS：classList 操作
来源：http://ckh.cqqwz.cn

el.classList.toggle("active")
来源：http://rel.vqdsnc.cn

[U102] JS：本地存储
来源：http://gpl.zycfv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://aen.svipenyu.cn

[U103] JS：定时器
来源：http://zex.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bhc.yvedp.cn

[U104] JS：防抖
来源：http://zwx.mhx1999.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vom.jinyuanbaomall.cn

[U105] JS：节流
来源：http://vct.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xtk.yanxiufei.cn

[U106] JS：日期格式化
来源：http://pwg.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sbv.sweek.top

[U107] JS：数字千分位
来源：http://mcm.mhx1999.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yoj.bjfxy.top

[U108] JS：随机整数
来源：http://whh.aizwys.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xao.haohaochexian.top

[U109] JS：数组分组
来源：http://iyf.ybcxt.top

Object.groupBy(arr, x => x.type)
来源：http://ize.zhixingplan.top

[U110] JS：数组分块
来源：http://xrw.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ikn.pengpengdd.cyou

[U111] JS：对象转 Map
来源：http://urq.fktsv.cn

new Map(Object.entries(obj))
来源：http://kpx.ehwqpu.com

[U112] JS：字符串补位
来源：http://sho.uphjek.com

"7".padStart(3, "0")
来源：http://fzz.zhiwuduotai.top

[U113] JS：正则替换全部
来源：http://csx.shuidangran.top

s.replaceAll("a", "b")
来源：http://enc.xylfe.cn

[U114] JS：JSON 深比较
来源：http://xeq.gaohongyu789.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://epd.xylfe.cn

[U115] JS：生成 UUID
来源：http://vkn.havefunace.top

crypto.randomUUID()
来源：http://srj.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://ttx.daria6918.cn

/** @param {string} name */ function f(name) {}
来源：http://cvh.yuanzhike.top

[U117] JS：单元测试
来源：http://bee.sysykeji.top

npm i -D vitest;  npx vitest
来源：http://dxm.guowangkeji.top

[U118] JS：开发服务器
来源：http://zoo.yueranfly.top

npm i -D vite;  npx vite
来源：http://hkr.zhengqikj.top

[U119] JS：生产构建
来源：http://mzt.iojbl.cn

npx vite build
来源：http://dxg.ybcxt.top

[U120] JS：读取环境变量（Vite）
来源：http://yoc.gogol.net.cn

import.meta.env.VITE_API_URL
来源：http://zwu.zhiwuduotai.top

================================================================================
来源：http://cak.0kj1m.cn

统计汇总
来源：http://nlc.zhoulong.xyz

================================================================================
来源：http://xwd.tianlin.xyz

按语言统计（条）：
来源：http://ebd.ivvv.top

Python ......... 252
来源：http://hax.kuanghao11.cn

PHP ............ 252
来源：http://axj.pengpengdd.cyou

JavaScript ..... 252
来源：http://izj.jlsjyb.cn

TypeScript ..... 212
来源：http://aif.fzhhl.top

Java ........... 212
来源：http://umn.tian-w.cn

Go ............. 212
来源：http://xln.zycfv.cn

Ruby ........... 212
来源：http://qbv.yj20258.top

C# ............. 212
来源：http://syw.nwbrower.top

C .............. 30
来源：http://ibp.dianchejie.cn

C++ ............ 30
来源：http://gbx.sweek.top

SQL ............ 90
来源：http://kfq.xylfe.cn

Bash ........... 80
来源：http://vvk.hcnkem.com

Kotlin ......... 15
来源：http://yyw.jianghu66.top

Swift .......... 15
来源：http://msr.nanxinkj.top

Lua ............ 10
来源：http://dyt.hongshengwenyu.top

Perl ........... 10
来源：http://koe.vehdjk.com

Scala .......... 10
来源：http://avl.fanxiaobao.xyz

------------------------------------
来源：http://gff.yueranfly.top

合计 ........... 2106 条
来源：http://klz.dashuyun.cn

按章节统计：
来源：http://zkc.chenlongwang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://adn.aibaodan.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zqw.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cwv.xingfuxueyuan.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://opy.zhongyouzk.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gab.ivvv.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uye.ybcxt.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://prw.zhengqikj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kly.guannengcc.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://deu.jinqigfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nme.c1oappe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://awg.ppjwa.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qzr.guowangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dtc.yonumen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ojt.yueranfly.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kas.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jav.xingfuxueyuan.xyz

Q SQL 专题                              90
来源：http://kkh.sxryk.cn

R Bash 专题                             80
来源：http://lue.ivvv.top

S C / C++ 专题                          60
来源：http://svc.xylfe.cn

T 其他语言补充                          60
来源：http://ttw.zhiwuduotai.top

U 高频实用片段                         120
来源：http://unc.hcnkem.com

------------------------------------
来源：http://mra.ydzc1.top

合计                                  2106 条
来源：http://ihr.xylfe.cn

--------------------------------------------------------------------------------
来源：http://msz.sxryk.cn

使用提醒
来源：http://mlo.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://wzc.mhx1999.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kdt.jinghuilouyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://osm.ppjwa.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ccm.yj20258888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://maa.zycfv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qux.xuetiantiany.cn

—— 文件结束 ——
来源：http://xxj.chenjidiqi.icu


<!-- 参考信息 -->