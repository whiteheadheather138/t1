代发 wailian999

[U07] Py：反转字典键值
来源：http://zyj.vehdjk.com

{v: k for k, v in d.items()}
来源：http://kew.ydjk.org.cn

[U08] Py：展平二维列表
来源：http://ask.dianchejie.cn

[y for x in nested for y in x]
来源：http://jvx.ivvv.top

[U09] Py：字典取最大值的键
来源：http://isa.yonumen.top

max(d, key=d.get)
来源：http://lzg.ydzc1.top

[U10] Py：按值排序字典
来源：http://mwg.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ksg.ywan-chungtsiang.top

[U11] Py：生成器表达式
来源：http://ins.xingfuxueyuan.xyz

(x * 2 for x in arr)
来源：http://skh.yj202588.top

[U12] Py：取出现最多的 3 个元素
来源：http://kyj.guannengcc.top

Counter(arr).most_common(3)
来源：http://doi.dashuyun.cn

[U13] Py：固定长度队列
来源：http://yqz.kuanghao11.cn

deque(maxlen=10)
来源：http://bqz.tian-w.cn

[U14] Py：分组收集到列表
来源：http://ine.vehdjk.com

defaultdict(list)
来源：http://laz.birdmap.top

[U15] Py：高精度计时
来源：http://pme.zdbjq.cn

t = time.perf_counter()
来源：http://kpk.xingfuxueyuan.xyz

[U16] Py：命令行参数解析
来源：http://xkc.mhx1999.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xrd.cashguo.top

[U17] Py：初始化日志
来源：http://sod.gaohongyu789.top

logging.basicConfig(level=logging.INFO)
来源：http://ywf.cashguo.top

[U18] Py：预编译正则
来源：http://vuv.nwbrower.top

pat = re.compile(r"\d+")
来源：http://fez.andypj.xyz

[U19] Py：正则替换带回调
来源：http://vlt.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://stu.shanyushiyangtech.top

[U20] Py：缓存函数结果
来源：http://knc.sxryk.cn

@functools.lru_cache(maxsize=None)
来源：http://fzb.hysaishi.cn

[U21] Py：自定义上下文管理器
来源：http://gaf.ctjpmb.com

@contextlib.contextmanager
来源：http://wra.gotoacloud.top

[U22] Py：矩阵转置
来源：http://irl.gotoacloud.top

list(zip(*m))
来源：http://bml.zhoulong.xyz

[U23] Py：分块读取大文件
来源：http://nox.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uor.svipenyu.cn

[U24] Py：路径操作
来源：http://pnu.cqqwz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gkm.ivvv.top

[U25] Py：CSV 按字典读
来源：http://xrd.shanyushiyangtech.top

csv.DictReader(f)
来源：http://eby.yfazqb.com

[U26] Py：并发下载
来源：http://cus.ywan-chungtsiang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ghc.cqqwz.cn

[U27] Py：异步 HTTP
来源：http://fdn.gaohongyu789.top

aiohttp.ClientSession() 配合 async with
来源：http://erh.yvedp.cn

[U28] Py：类型别名
来源：http://dli.pycfn.com

UserId = int
来源：http://upp.yueranfly.top

[U29] Py：属性校验
来源：http://wls.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://gpm.zhoulong.xyz

[U30] Py：数据类
来源：http://fhp.316326.xyz

@dataclass(slots=True)
来源：http://ozi.ehwqpu.com

[U31] Py：单测
来源：http://axf.svipenyu.cn

python -m pytest -q
来源：http://mug.smart0.xyz

[U32] Py：代码格式化
来源：http://eeq.svipenyu.cn

ruff format . && ruff check --fix .
来源：http://umb.jiagoushi.top

[U33] Py：打包发布
来源：http://xuv.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://lhp.zycfv.cn

[U34] Py：判断编码
来源：http://quj.zhaomingkeji.xyz

chardet.detect(raw)
来源：http://xkq.feifeiyinyue.top

[U35] Py：发送邮件
来源：http://qjf.guannengcc.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ryr.chenjidiqi.icu

[U36] Py：定时任务
来源：http://wkl.sysykeji.top

schedule.every(10).minutes.do(job)
来源：http://yuv.ywan-chungtsiang.top

[U37] Py：读写 Excel
来源：http://rdc.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://ryr.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://twf.dianchejie.cn

Path(__file__).resolve().parent
来源：http://wbh.zdqjudy.top

[U39] Py：判断是否在交互环境
来源：http://gsn.yj202588.top

sys.stdout.isatty()
来源：http://yzk.mhx1999.top

[U40] Py：打印到标准错误
来源：http://ihi.gotoacloud.top

print("err", file=sys.stderr)
来源：http://ort.ehwqpu.com

[U41] PHP：初始化 Composer 项目
来源：http://tbv.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://xfw.yj20258.top

[U42] PHP：PSR-4 自动加载
来源：http://lfe.316326.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xpy.svipenyu.cn

[U43] PHP：声明命名空间
来源：http://ffi.chenlongwang.top

namespace App\Http;
来源：http://zbr.hnxiangtu.top

[U44] PHP：开启严格类型
来源：http://ktp.cqqwz.cn

declare(strict_types=1);
来源：http://xwc.yj20258888.top

[U45] PHP：类型声明与返回类型
来源：http://cmk.ybcxt.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qrg.dashuyun.cn

[U46] PHP：可空类型
来源：http://ztj.yongpay.top

?string $name = null
来源：http://qaj.yangfankeji.com

[U47] PHP：联合类型
来源：http://tyb.andypj.xyz

int|string $id
来源：http://wiy.uphjek.com

[U48] PHP：纯枚举
来源：http://frt.ppjwa.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rot.jyoumei.cn

[U49] PHP：只读属性
来源：http://xmg.quarkkingdee.top

public readonly string $name
来源：http://ehk.yongpay.top

[U50] PHP：构造器属性提升
来源：http://ynw.tarul.cn

public function __construct(private int $id) {}
来源：http://xrk.uphjek.com

[U51] PHP：数组解构
来源：http://ego.gzhubu.top

[$a, $b] = $arr;
来源：http://xnt.hammf.cn

[U52] PHP：箭头函数
来源：http://pip.ehwqpu.com

$double = fn($x) => $x * 2;
来源：http://rqc.hcnkem.com

[U53] PHP：空合并运算符
来源：http://srv.hesvh.cn

$v = $a ?? $b ?? "default";
来源：http://kmc.zdbjq.cn

[U54] PHP：空安全调用
来源：http://jdq.fktsv.cn

$obj?->method()
来源：http://bdd.dianchejie.cn

[U55] PHP：match 表达式
来源：http://eiu.fehbvm.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://njv.jianghu66.top

[U56] PHP：命名参数
来源：http://fbk.snrcjt.cn

f(a: 1, b: 2)
来源：http://wyj.nanxuanxn.top

[U57] PHP：字符串插值
来源：http://jox.yuanzhike.top

"值: {$a}"
来源：http://cud.hnqzz.top

[U58] PHP：数组三件套
来源：http://jzk.zhijiandao.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://keb.shzxlz.cn

[U59] PHP：自定义排序
来源：http://syj.smart0.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kst.pengpengdd.cyou

[U60] PHP：JSON 编解码
来源：http://bpq.yueranfly.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wkg.redwolf501.top

[U61] PHP：正则
来源：http://pog.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hre.jinqigfzy.top

[U62] PHP：日期对象
来源：http://gxm.yj202588.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://utb.chenzaomai.com

[U63] PHP：文件读写
来源：http://zcq.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://knj.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://pbg.fanxiaobao.xyz

glob("dir/*.php");  scandir("dir");
来源：http://joz.bjfxy.top

[U65] PHP：会话
来源：http://rxy.zhongyouzk.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pcv.snrcjt.cn

[U66] PHP：设置 Cookie
来源：http://glq.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sqj.tianlin.xyz

[U67] PHP：处理文件上传
来源：http://ysj.316326.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jzf.sysykeji.top

[U68] PHP：PDO 连接
来源：http://gny.hammf.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ynm.pengpengdd.cyou

[U69] PHP：PDO 预处理
来源：http://tmx.ywan-chungtsiang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ouv.gzhubu.top

[U70] PHP：PDO 事务
来源：http://jii.zhijiandao.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cjq.ppjwa.cn

[U71] PHP：抛出异常
来源：http://nih.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://bvg.aizwys.cn

[U72] PHP：写错误日志
来源：http://iio.nanxinkj.top

error_log("失败: " . $e->getMessage());
来源：http://ihz.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://bpd.chenzaomai.com

parse_ini_file("config.ini", true)
来源：http://ncb.pycfn.com

[U74] PHP：读取环境变量
来源：http://lnj.quarkkingdee.top

getenv("APP_ENV") ?: "production"
来源：http://qnl.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://xns.fzhhl.top

composer require psr/container
来源：http://rhw.birdmap.top

[U76] PHP：简单路由
来源：http://zsc.cqqwz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mjg.nwbrower.top

[U77] PHP：模板渲染
来源：http://gfz.xylfe.cn

composer require twig/twig
来源：http://kuv.yj20258.top

[U78] PHP：单元测试
来源：http://rts.daria6918.cn

composer require --dev phpunit/phpunit
来源：http://urp.iojbl.cn

[U79] PHP：静态分析
来源：http://tgx.iojbl.cn

composer require --dev phpstan/phpstan
来源：http://qdy.52xcode.cn

[U80] PHP：代码规范修复
来源：http://dww.sweek.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dld.chenzaomai.com

[U81] JS：初始化项目
来源：http://qkm.cheryme.top

npm init -y;  npm i express
来源：http://jyl.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://pgo.jinqigufen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mwd.ppjwa.cn

[U83] JS：ES Module 导入导出
来源：http://tyl.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://oaw.sufxvd.cn

[U84] JS：CommonJS 写法
来源：http://yze.yangfankeji.com

module.exports = { a };  const { a } = require("./m");
来源：http://cuo.fanxiaobao.xyz

[U85] JS：可选链
来源：http://yxv.bbcook.cn

a?.b?.c
来源：http://hrp.fktsv.cn

[U86] JS：空值合并
来源：http://hfg.dianchejie.cn

a ?? b
来源：http://gfx.zhongyouzk.top

[U87] JS：解构默认值
来源：http://zfb.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://mpe.hcnkem.com

[U88] JS：对象展开合并
来源：http://irb.fanxiaobao.xyz

{ ...a, ...b }
来源：http://kyr.jinqigfzy.top

[U89] JS：数组去重
来源：http://kyz.aizwys.cn

[...new Set(arr)]
来源：http://eno.gotoacloud.top

[U90] JS：数字数组排序
来源：http://qru.jianghu66.top

[...arr].sort((a, b) => a - b)
来源：http://nlx.yj20258888.top

[U91] JS：对象键值遍历
来源：http://obs.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ijy.ehwqpu.com

[U92] JS：深拷贝
来源：http://dji.zhijiandao.cn

structuredClone(obj)
来源：http://vno.daxiang520.top

[U93] JS：模板字符串
来源：http://ehg.feifeiyinyue.top

`共 ${n} 条`
来源：http://yzd.hammf.cn

[U94] JS：箭头函数
来源：http://kgu.gaohongyu789.top

const double = x => x * 2;
来源：http://lqh.haohaochexian.top

[U95] JS：Promise 包装
来源：http://fxq.yj20258888.top

new Promise((resolve, reject) => {})
来源：http://che.chenlongwang.top

[U96] JS：async/await 与异常
来源：http://xua.zhixingplan.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://svv.jinyuanbaomall.cn

[U97] JS：并发请求
来源：http://uyq.gotoacloud.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://par.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://ryb.epnwcf.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gje.aizwys.cn

[U99] JS：事件监听
来源：http://egc.daxiang520.top

el.addEventListener("click", e => {})
来源：http://asg.bbcook.cn

[U100] JS：DOM 查询
来源：http://zvu.ywan-chungtsiang.top

document.querySelector(".item")
来源：http://goe.zhixingplan.top

[U101] JS：classList 操作
来源：http://kgy.guowangkeji.top

el.classList.toggle("active")
来源：http://qhq.zhaomingkeji.xyz

[U102] JS：本地存储
来源：http://abl.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ijr.uphjek.com

[U103] JS：定时器
来源：http://tuh.xuanzx.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qqg.shanyushiyangkeji.top

[U104] JS：防抖
来源：http://aib.vehdjk.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://etv.xziqi.cn

[U105] JS：节流
来源：http://bzk.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lob.fehbvm.com

[U106] JS：日期格式化
来源：http://zzw.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dxx.fanxiaobao.xyz

[U107] JS：数字千分位
来源：http://qzp.jinqigfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oqc.yanxiufei.cn

[U108] JS：随机整数
来源：http://mur.yj202588.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pas.epnwcf.com

[U109] JS：数组分组
来源：http://kpn.zhoulong.xyz

Object.groupBy(arr, x => x.type)
来源：http://ldj.xziqi.cn

[U110] JS：数组分块
来源：http://yhy.jinqigfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ftm.zdbjq.cn

[U111] JS：对象转 Map
来源：http://nph.ybcxt.top

new Map(Object.entries(obj))
来源：http://fwr.andypj.xyz

[U112] JS：字符串补位
来源：http://nfl.quarkkingdee.top

"7".padStart(3, "0")
来源：http://mvx.ctjpmb.com

[U113] JS：正则替换全部
来源：http://cmx.fktsv.cn

s.replaceAll("a", "b")
来源：http://cxx.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://fux.ywan-chungtsiang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://irr.c1oappe.top

[U115] JS：生成 UUID
来源：http://mwa.hesvh.cn

crypto.randomUUID()
来源：http://cto.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://dmy.wangdashe.top

/** @param {string} name */ function f(name) {}
来源：http://ygj.gaohongyu789.top

[U117] JS：单元测试
来源：http://ink.pycfn.com

npm i -D vitest;  npx vitest
来源：http://zyf.andypj.xyz

[U118] JS：开发服务器
来源：http://fhx.gogol.net.cn

npm i -D vite;  npx vite
来源：http://opr.hywenlv.cn

[U119] JS：生产构建
来源：http://aln.shuidangran.top

npx vite build
来源：http://ehw.hesvh.cn

[U120] JS：读取环境变量（Vite）
来源：http://yfl.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://crn.sweek.top

================================================================================
来源：http://kzq.gzhubu.top

统计汇总
来源：http://acp.nanxuanxn.top

================================================================================
来源：http://tks.gogol.net.cn

按语言统计（条）：
来源：http://inh.ppjwa.cn

Python ......... 252
来源：http://dcr.meibo888.top

PHP ............ 252
来源：http://hle.yfazqb.com

JavaScript ..... 252
来源：http://otg.zhongyouzk.top

TypeScript ..... 212
来源：http://qzv.zdqjudy.top

Java ........... 212
来源：http://bla.svipenyu.cn

Go ............. 212
来源：http://xly.jqgufenzy.top

Ruby ........... 212
来源：http://ivt.haohaochexian.top

C# ............. 212
来源：http://skt.fehbvm.com

C .............. 30
来源：http://ztl.shuidangran.top

C++ ............ 30
来源：http://ogq.shanyushiyangtech.top

SQL ............ 90
来源：http://xtk.xingfuxueyuan.xyz

Bash ........... 80
来源：http://jee.zdqjudy.top

Kotlin ......... 15
来源：http://sgj.fzhhl.top

Swift .......... 15
来源：http://dyl.cheryme.top

Lua ............ 10
来源：http://nno.epnwcf.com

Perl ........... 10
来源：http://jcu.sufxvd.cn

Scala .......... 10
来源：http://dxe.dashuyun.cn

------------------------------------
来源：http://qhc.shuidangran.top

合计 ........... 2106 条
来源：http://wrk.ywan-chungtsiang.top

按章节统计：
来源：http://kmf.yuanzhike.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xhk.yueranfly.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bba.xingfuxueyuan.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ezg.nanxuanxn.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ywm.tarul.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oht.feifeiyinyue.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eea.kuanghao11.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nfy.jlsjyb.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sht.yvedp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://klo.yueranfly.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uaf.bjfxy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uhu.nanxinkj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zrz.aibaodan.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wif.hnqzz.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hoa.zhijiandao.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zow.jianghu66.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hdk.andypj.xyz

Q SQL 专题                              90
来源：http://mmo.cucudq.cn

R Bash 专题                             80
来源：http://cgj.hnxiangtu.top

S C / C++ 专题                          60
来源：http://ptp.zhixingplan.top

T 其他语言补充                          60
来源：http://dwc.guowangkeji.top

U 高频实用片段                         120
来源：http://vel.hammf.cn

------------------------------------
来源：http://lim.zhoulong.xyz

合计                                  2106 条
来源：http://voa.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://hpe.ybcxt.top

使用提醒
来源：http://mth.bbcook.cn

--------------------------------------------------------------------------------
来源：http://emn.feifeiyinyue.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uoc.sweek.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dui.hywenlv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fdh.snrcjt.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zkc.redwolf501.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cll.ctjpmb.com

—— 文件结束 ——
来源：http://bve.shanyushiyangkeji.top

================================================================================
来源：http://azz.zhaomingkeji.xyz

程序语言常见例子速查手册（2024 版）
来源：http://set.jqgfzy.top

Common Programming Examples Cheat Book
来源：http://zob.hywenlv.cn

================================================================================
来源：http://rxh.hysaishi.cn

【收录内容】
来源：http://nnd.mhx1999.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sgn.guowangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://afd.ehwqpu.com

SQL · Bash · C · C++
来源：http://cnl.fktsv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://byr.ivvv.top

【使用说明】
来源：http://kke.ctjpmb.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wzm.hnqzz.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://itu.hongshengwenyu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ysv.cdnleiting.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lne.daria6918.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zgz.xinyue.icu

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eyh.cqqwz.cn


<!-- 参考信息 -->