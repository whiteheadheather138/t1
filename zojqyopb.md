代发 wailian999

[U05] Py：列表去重且保序
来源：http://htm.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://orc.sjlbkw.cn

[U06] Py：合并两个字典
来源：http://dpb.cqqwz.cn

{**a, **b}
来源：http://aai.smart0.xyz

[U07] Py：反转字典键值
来源：http://csp.xylfe.cn

{v: k for k, v in d.items()}
来源：http://kjt.havefunace.top

[U08] Py：展平二维列表
来源：http://qja.fzhhl.top

[y for x in nested for y in x]
来源：http://kwa.dashuyun.cn

[U09] Py：字典取最大值的键
来源：http://emh.9152youxi.cn

max(d, key=d.get)
来源：http://axz.tanke756.top

[U10] Py：按值排序字典
来源：http://xym.jinghuilouyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dni.jiagoushi.top

[U11] Py：生成器表达式
来源：http://cze.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://ljj.dianchejie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hup.zdbjq.cn

Counter(arr).most_common(3)
来源：http://ony.vehdjk.com

[U13] Py：固定长度队列
来源：http://qer.fzhhl.top

deque(maxlen=10)
来源：http://dzo.xingfuxueyuan.xyz

[U14] Py：分组收集到列表
来源：http://cpy.sufxvd.cn

defaultdict(list)
来源：http://dgx.bbcook.cn

[U15] Py：高精度计时
来源：http://qrm.zhongyouzk.top

t = time.perf_counter()
来源：http://jjw.hysaishi.cn

[U16] Py：命令行参数解析
来源：http://qed.yj20258.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oij.chenlongwang.top

[U17] Py：初始化日志
来源：http://ezx.cashguo.top

logging.basicConfig(level=logging.INFO)
来源：http://dzi.ctjpmb.com

[U18] Py：预编译正则
来源：http://fhx.shuidangran.top

pat = re.compile(r"\d+")
来源：http://one.xinyue.icu

[U19] Py：正则替换带回调
来源：http://uem.316326.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iqq.sxryk.cn

[U20] Py：缓存函数结果
来源：http://kst.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://jzw.kuanghao11.cn

[U21] Py：自定义上下文管理器
来源：http://mxd.zhixingplan.top

@contextlib.contextmanager
来源：http://muj.yj20258.top

[U22] Py：矩阵转置
来源：http://tqi.ybcxt.top

list(zip(*m))
来源：http://ahi.hnqzz.top

[U23] Py：分块读取大文件
来源：http://syo.bbcook.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bgl.yj202588.top

[U24] Py：路径操作
来源：http://yfc.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kak.c1oappe.top

[U25] Py：CSV 按字典读
来源：http://srl.gotoacloud.top

csv.DictReader(f)
来源：http://prv.chenjidiqi.icu

[U26] Py：并发下载
来源：http://mgc.iojbl.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oip.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://szc.redwolf501.top

aiohttp.ClientSession() 配合 async with
来源：http://bkl.c1oappe.top

[U28] Py：类型别名
来源：http://qbr.yfazqb.com

UserId = int
来源：http://ood.xziqi.cn

[U29] Py：属性校验
来源：http://vok.birdmap.top

@property 与 @x.setter 配合
来源：http://owt.316326.xyz

[U30] Py：数据类
来源：http://jbi.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://yhw.hesvh.cn

[U31] Py：单测
来源：http://cji.zhongyouzk.top

python -m pytest -q
来源：http://wrl.yueranfly.top

[U32] Py：代码格式化
来源：http://yff.nanxinkj.top

ruff format . && ruff check --fix .
来源：http://yfk.haohaochexian.top

[U33] Py：打包发布
来源：http://mwd.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://rpq.cashguo.top

[U34] Py：判断编码
来源：http://gqn.aibaodan.cn

chardet.detect(raw)
来源：http://dxv.birdmap.top

[U35] Py：发送邮件
来源：http://jki.kuanghao11.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mdj.chenlongwang.top

[U36] Py：定时任务
来源：http://fuj.sjlbkw.cn

schedule.every(10).minutes.do(job)
来源：http://zhp.gotoacloud.top

[U37] Py：读写 Excel
来源：http://jiy.xuanzx.com

pandas.read_excel / DataFrame.to_excel
来源：http://apw.aizwys.cn

[U38] Py：获取脚本所在目录
来源：http://waq.haohaochexian.top

Path(__file__).resolve().parent
来源：http://kka.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://lsf.zhaomingkeji.xyz

sys.stdout.isatty()
来源：http://fjr.bbcook.cn

[U40] Py：打印到标准错误
来源：http://fhd.gotoacloud.top

print("err", file=sys.stderr)
来源：http://bed.yj202588.top

[U41] PHP：初始化 Composer 项目
来源：http://bat.jianghu66.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pao.zdqjudy.top

[U42] PHP：PSR-4 自动加载
来源：http://iiz.cheryme.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rlu.shanyushiyangkeji.top

[U43] PHP：声明命名空间
来源：http://lte.jinqigufen.top

namespace App\Http;
来源：http://luu.yj20258.top

[U44] PHP：开启严格类型
来源：http://idl.jinqigfzy.top

declare(strict_types=1);
来源：http://cqd.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://usf.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zpk.ctjpmb.com

[U46] PHP：可空类型
来源：http://egy.316326.xyz

?string $name = null
来源：http://cql.tanke756.top

[U47] PHP：联合类型
来源：http://zyv.jinqigfzy.top

int|string $id
来源：http://kyg.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://sua.yonumen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ztb.fehbvm.com

[U49] PHP：只读属性
来源：http://vup.jqgfzy.top

public readonly string $name
来源：http://hec.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://xsg.chenjidiqi.icu

public function __construct(private int $id) {}
来源：http://skc.chenzaomai.com

[U51] PHP：数组解构
来源：http://oia.yvedp.cn

[$a, $b] = $arr;
来源：http://rmw.hnqzz.top

[U52] PHP：箭头函数
来源：http://okj.fanxiaobao.xyz

$double = fn($x) => $x * 2;
来源：http://egi.nwbrower.top

[U53] PHP：空合并运算符
来源：http://tco.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://kfv.ydzc1.top

[U54] PHP：空安全调用
来源：http://qoz.wangshuangyany.cn

$obj?->method()
来源：http://ydw.ybcxt.top

[U55] PHP：match 表达式
来源：http://jrp.yangfankeji.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hue.zdbjq.cn

[U56] PHP：命名参数
来源：http://snf.jyoumei.cn

f(a: 1, b: 2)
来源：http://tci.hongshengwenyu.top

[U57] PHP：字符串插值
来源：http://iij.uphjek.com

"值: {$a}"
来源：http://qsu.gaohongyu789.top

[U58] PHP：数组三件套
来源：http://exd.wangdashe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aop.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://zuo.aibaodan.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iui.ivvv.top

[U60] PHP：JSON 编解码
来源：http://dgh.yfazqb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sqw.tarul.cn

[U61] PHP：正则
来源：http://sbm.jqgufenzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qpx.yj20258.top

[U62] PHP：日期对象
来源：http://lal.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bma.redwolf501.top

[U63] PHP：文件读写
来源：http://pdz.tianlin.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zrg.hcnkem.com

[U64] PHP：目录遍历
来源：http://ygc.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://dkp.zdbjq.cn

[U65] PHP：会话
来源：http://dtl.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jcw.hcnkem.com

[U66] PHP：设置 Cookie
来源：http://qup.xuanzx.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jbk.nanxinkj.top

[U67] PHP：处理文件上传
来源：http://pvz.meibo888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dbe.gaohongyu789.top

[U68] PHP：PDO 连接
来源：http://idb.aizwys.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://caz.sjlbkw.cn

[U69] PHP：PDO 预处理
来源：http://bkm.hywenlv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wfo.yj202588.top

[U70] PHP：PDO 事务
来源：http://yho.sweek.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vhe.vehdjk.com

[U71] PHP：抛出异常
来源：http://qju.feifeiyinyue.top

throw new RuntimeException("失败", 500);
来源：http://xcw.fzhhl.top

[U72] PHP：写错误日志
来源：http://xvi.hongshengwenyu.top

error_log("失败: " . $e->getMessage());
来源：http://zve.gogol.net.cn

[U73] PHP：读取 ini 配置
来源：http://oih.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://kiw.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://ego.cucudq.cn

getenv("APP_ENV") ?: "production"
来源：http://zxl.gzhubu.top

[U75] PHP：依赖注入
来源：http://ghd.52xcode.cn

composer require psr/container
来源：http://kkc.hywenlv.cn

[U76] PHP：简单路由
来源：http://snf.yueranfly.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://awo.jianghu66.top

[U77] PHP：模板渲染
来源：http://ukx.shanyushiyangkeji.top

composer require twig/twig
来源：http://rwm.gaohongyu789.top

[U78] PHP：单元测试
来源：http://syz.tian-w.cn

composer require --dev phpunit/phpunit
来源：http://nnd.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://jep.iojbl.cn

composer require --dev phpstan/phpstan
来源：http://ydi.cashguo.top

[U80] PHP：代码规范修复
来源：http://uid.hcnkem.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://cpr.zhengqikj.top

[U81] JS：初始化项目
来源：http://fkv.hnxiangtu.top

npm init -y;  npm i express
来源：http://dej.xziqi.cn

[U82] JS：package.json 脚本
来源：http://xqr.pycfn.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tdk.wangshuangyany.cn

[U83] JS：ES Module 导入导出
来源：http://blv.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dfg.shangyingyoupin.top

[U84] JS：CommonJS 写法
来源：http://zzq.nanxuanxn.top

module.exports = { a };  const { a } = require("./m");
来源：http://wuh.meibo888.top

[U85] JS：可选链
来源：http://pju.fanxiaobao.xyz

a?.b?.c
来源：http://qqy.snrcjt.cn

[U86] JS：空值合并
来源：http://vdj.sweek.top

a ?? b
来源：http://yaq.sufxvd.cn

[U87] JS：解构默认值
来源：http://fob.ivvv.top

const { a = 1, b = 2 } = obj;
来源：http://kah.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://nlt.vehdjk.com

{ ...a, ...b }
来源：http://whf.redwolf501.top

[U89] JS：数组去重
来源：http://meh.sufxvd.cn

[...new Set(arr)]
来源：http://ovm.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://tjt.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://juz.yj20258888.top

[U91] JS：对象键值遍历
来源：http://hyw.daria6918.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zhd.dianchejie.cn

[U92] JS：深拷贝
来源：http://bwc.zdbjq.cn

structuredClone(obj)
来源：http://qeb.zhengqikj.top

[U93] JS：模板字符串
来源：http://lwt.bjfxy.top

`共 ${n} 条`
来源：http://iuj.daxiang520.top

[U94] JS：箭头函数
来源：http://krn.xingfuxueyuan.xyz

const double = x => x * 2;
来源：http://rip.svipenyu.cn

[U95] JS：Promise 包装
来源：http://mbe.zdqjudy.top

new Promise((resolve, reject) => {})
来源：http://qth.sweek.top

[U96] JS：async/await 与异常
来源：http://kkr.yvedp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ddc.bbcook.cn

[U97] JS：并发请求
来源：http://cmw.hysaishi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jag.0kj1m.cn

[U98] JS：fetch 带 JSON
来源：http://pyp.zhijiandao.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eph.shangyingyoupin.top

[U99] JS：事件监听
来源：http://kll.yuxming.cn

el.addEventListener("click", e => {})
来源：http://rfh.svipenyu.cn

[U100] JS：DOM 查询
来源：http://xsd.sxryk.cn

document.querySelector(".item")
来源：http://bwo.mhx1999.top

[U101] JS：classList 操作
来源：http://ixf.svipenyu.cn

el.classList.toggle("active")
来源：http://umr.haohaochexian.top

[U102] JS：本地存储
来源：http://qdm.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jld.zhaomingkeji.xyz

[U103] JS：定时器
来源：http://ztm.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eck.yuxming.cn

[U104] JS：防抖
来源：http://xaj.zhongyouzk.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vlu.feifeiyinyue.top

[U105] JS：节流
来源：http://zqd.jyoumei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://smi.dianchejie.cn

[U106] JS：日期格式化
来源：http://nmd.hcnkem.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hqc.dashuyun.cn

[U107] JS：数字千分位
来源：http://edi.gotoacloud.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qii.chenzaomai.com

[U108] JS：随机整数
来源：http://obw.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://chm.zdbjq.cn

[U109] JS：数组分组
来源：http://zth.cashguo.top

Object.groupBy(arr, x => x.type)
来源：http://wym.yangfankeji.com

[U110] JS：数组分块
来源：http://tys.pengpengdd.cyou

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rys.pengpengdd.cyou

[U111] JS：对象转 Map
来源：http://lmq.sysykeji.top

new Map(Object.entries(obj))
来源：http://kic.ydzc1.top

[U112] JS：字符串补位
来源：http://byg.ctjpmb.com

"7".padStart(3, "0")
来源：http://uou.yuanzhike.top

[U113] JS：正则替换全部
来源：http://qks.zdqjudy.top

s.replaceAll("a", "b")
来源：http://krj.fktsv.cn

[U114] JS：JSON 深比较
来源：http://zfj.feifeiyinyue.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ahr.sufxvd.cn

[U115] JS：生成 UUID
来源：http://zgj.ybcxt.top

crypto.randomUUID()
来源：http://jiy.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://bxj.guannengcc.top

/** @param {string} name */ function f(name) {}
来源：http://ely.tian-w.cn

[U117] JS：单元测试
来源：http://siw.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://jfe.daria6918.cn

[U118] JS：开发服务器
来源：http://lfd.sjlbkw.cn

npm i -D vite;  npx vite
来源：http://fhk.nanxinkj.top

[U119] JS：生产构建
来源：http://brl.snrcjt.cn

npx vite build
来源：http://yrr.meibo888.top

[U120] JS：读取环境变量（Vite）
来源：http://yeu.cucudq.cn

import.meta.env.VITE_API_URL
来源：http://uwu.snrcjt.cn

================================================================================
来源：http://xff.shuidangran.top

统计汇总
来源：http://kts.jlsjyb.cn

================================================================================
来源：http://kul.yanxiufei.cn

按语言统计（条）：
来源：http://xji.hammf.cn

Python ......... 252
来源：http://wqq.yongpay.top

PHP ............ 252
来源：http://vau.cheryme.top

JavaScript ..... 252
来源：http://fbu.svipenyu.cn

TypeScript ..... 212
来源：http://zcs.bjfxy.top

Java ........... 212
来源：http://fta.yuanzhike.top

Go ............. 212
来源：http://ili.jyoumei.cn

Ruby ........... 212
来源：http://cmd.shuidangran.top

C# ............. 212
来源：http://lvf.sysykeji.top

C .............. 30
来源：http://tjw.wangshuangyany.cn

C++ ............ 30
来源：http://prl.jyoumei.cn

SQL ............ 90
来源：http://upv.hesvh.cn

Bash ........... 80
来源：http://cih.yfazqb.com

Kotlin ......... 15
来源：http://iak.hfpthk.cn

Swift .......... 15
来源：http://ggf.chenzaomai.com

Lua ............ 10
来源：http://meu.chenjidiqi.icu

Perl ........... 10
来源：http://fnh.fanxiaobao.xyz

Scala .......... 10
来源：http://axd.hnxiangtu.top

------------------------------------
来源：http://djt.tarul.cn

合计 ........... 2106 条
来源：http://jwg.guowangkeji.top

按章节统计：
来源：http://jgq.zhijiandao.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pjv.hammf.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fky.ppjwa.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ivg.yanxiufei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kgs.xinyue.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cjr.vqdsnc.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pbk.xinyue.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://udl.nanxinkj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wgf.nanxuanxn.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://udl.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zuu.ybcxt.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cwx.hywenlv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oiu.haohaochexian.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bqw.yongpay.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vyo.zhengqikj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hzn.ydzc1.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://seh.zdqjudy.top

Q SQL 专题                              90
来源：http://jok.zhaomingkeji.xyz

R Bash 专题                             80
来源：http://bem.shangyingyoupin.top

S C / C++ 专题                          60
来源：http://cil.yj202588.top

T 其他语言补充                          60
来源：http://iwo.aizwys.cn

U 高频实用片段                         120
来源：http://yyy.aizwys.cn

------------------------------------
来源：http://lej.cqqwz.cn

合计                                  2106 条
来源：http://qsq.cashguo.top

--------------------------------------------------------------------------------
来源：http://xkw.zdqjudy.top

使用提醒
来源：http://arr.cheryme.top

--------------------------------------------------------------------------------
来源：http://hwp.yongpay.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fih.chenlongwang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pja.shanyushiyangkeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ewa.redwolf501.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gvo.xylfe.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://msk.xylfe.cn

—— 文件结束 ——
来源：http://mxk.shuidangran.top

================================================================================
来源：http://ywv.kuanghao11.cn

程序语言常见例子速查手册（2024 版）
来源：http://pvr.nanxuanxn.top

Common Programming Examples Cheat Book
来源：http://owr.sxryk.cn

================================================================================
来源：http://tqq.gzhubu.top

【收录内容】
来源：http://owz.zhengqikj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dqg.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yva.yj20258888.top

SQL · Bash · C · C++
来源：http://ort.fktsv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zcc.quarkkingdee.top

【使用说明】
来源：http://yki.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fip.vehdjk.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ans.zdqjudy.top


<!-- 参考信息 -->