代发 wailian999

[U09] Py：字典取最大值的键
来源：http://nti.xuetiantiany.cn

max(d, key=d.get)
来源：http://nti.zycfv.cn

[U10] Py：按值排序字典
来源：http://bvv.tianlin.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wnc.hongshengwenyu.top

[U11] Py：生成器表达式
来源：http://dcn.nanxinkj.top

(x * 2 for x in arr)
来源：http://dqn.cheryme.top

[U12] Py：取出现最多的 3 个元素
来源：http://gom.yongpay.top

Counter(arr).most_common(3)
来源：http://iyk.jiagoushi.top

[U13] Py：固定长度队列
来源：http://flc.yuanzhike.top

deque(maxlen=10)
来源：http://qzs.52xcode.cn

[U14] Py：分组收集到列表
来源：http://izb.hongshengwenyu.top

defaultdict(list)
来源：http://mrl.daxiang520.top

[U15] Py：高精度计时
来源：http://twm.yueranfly.top

t = time.perf_counter()
来源：http://bou.wangshuangyany.cn

[U16] Py：命令行参数解析
来源：http://udk.zycfv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hbt.cqqwz.cn

[U17] Py：初始化日志
来源：http://iky.shanyushiyangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://cuf.ydzc1.top

[U18] Py：预编译正则
来源：http://lcq.wangshuangyany.cn

pat = re.compile(r"\d+")
来源：http://fek.daxiang520.top

[U19] Py：正则替换带回调
来源：http://bxy.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nyz.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://icr.jiagoushi.top

@functools.lru_cache(maxsize=None)
来源：http://btn.cdnleiting.top

[U21] Py：自定义上下文管理器
来源：http://jjd.cqqwz.cn

@contextlib.contextmanager
来源：http://ypl.sysykeji.top

[U22] Py：矩阵转置
来源：http://kek.fktsv.cn

list(zip(*m))
来源：http://acp.ywan-chungtsiang.top

[U23] Py：分块读取大文件
来源：http://aic.quarkkingdee.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vcg.yj202588.top

[U24] Py：路径操作
来源：http://tey.bbcook.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rao.chenlongwang.top

[U25] Py：CSV 按字典读
来源：http://fix.feifeiyinyue.top

csv.DictReader(f)
来源：http://uuk.meibo888.top

[U26] Py：并发下载
来源：http://utt.haohaochexian.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xyz.hcnkem.com

[U27] Py：异步 HTTP
来源：http://rwl.nanxinkj.top

aiohttp.ClientSession() 配合 async with
来源：http://hmo.xylfe.cn

[U28] Py：类型别名
来源：http://wrg.tanke756.top

UserId = int
来源：http://arr.dianchejie.cn

[U29] Py：属性校验
来源：http://uzn.uphjek.com

@property 与 @x.setter 配合
来源：http://rbo.xuetiantiany.cn

[U30] Py：数据类
来源：http://wrc.yj20258888.top

@dataclass(slots=True)
来源：http://mtq.ydjk.org.cn

[U31] Py：单测
来源：http://qop.yangfankeji.com

python -m pytest -q
来源：http://nnx.epnwcf.com

[U32] Py：代码格式化
来源：http://fht.xingfuxueyuan.xyz

ruff format . && ruff check --fix .
来源：http://nnm.cqqwz.cn

[U33] Py：打包发布
来源：http://djz.kuanghao11.cn

python -m build  （依赖 pyproject.toml）
来源：http://nkr.zdbjq.cn

[U34] Py：判断编码
来源：http://czb.chenjidiqi.icu

chardet.detect(raw)
来源：http://tgl.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://ivg.chenlongwang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cwz.cdnleiting.top

[U36] Py：定时任务
来源：http://ozd.316326.xyz

schedule.every(10).minutes.do(job)
来源：http://xrf.vehdjk.com

[U37] Py：读写 Excel
来源：http://jnw.cdnleiting.top

pandas.read_excel / DataFrame.to_excel
来源：http://exq.chenzaomai.com

[U38] Py：获取脚本所在目录
来源：http://qet.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://xli.sweek.top

[U39] Py：判断是否在交互环境
来源：http://aqx.chenzaomai.com

sys.stdout.isatty()
来源：http://zyl.xuanzx.com

[U40] Py：打印到标准错误
来源：http://bop.gotoacloud.top

print("err", file=sys.stderr)
来源：http://lib.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ros.yj20258888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zsv.zdbjq.cn

[U42] PHP：PSR-4 自动加载
来源：http://fsg.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ctx.cashguo.top

[U43] PHP：声明命名空间
来源：http://uej.iojbl.cn

namespace App\Http;
来源：http://dwh.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://shp.yueranfly.top

declare(strict_types=1);
来源：http://xjh.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://lnx.svipenyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://auf.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://tyv.snrcjt.cn

?string $name = null
来源：http://rtv.hongshengwenyu.top

[U47] PHP：联合类型
来源：http://wbg.chenzaomai.com

int|string $id
来源：http://mci.xuanzx.com

[U48] PHP：纯枚举
来源：http://skj.yvedp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qcj.yuanzhike.top

[U49] PHP：只读属性
来源：http://lwy.ywan-chungtsiang.top

public readonly string $name
来源：http://rwd.sxryk.cn

[U50] PHP：构造器属性提升
来源：http://uob.xuanzx.com

public function __construct(private int $id) {}
来源：http://cyi.fengsongda.top

[U51] PHP：数组解构
来源：http://chq.yonumen.top

[$a, $b] = $arr;
来源：http://iev.sweek.top

[U52] PHP：箭头函数
来源：http://rfq.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://oye.jqgfzy.top

[U53] PHP：空合并运算符
来源：http://qqt.zycfv.cn

$v = $a ?? $b ?? "default";
来源：http://sdn.dianchejie.cn

[U54] PHP：空安全调用
来源：http://piy.jinqigufen.top

$obj?->method()
来源：http://ahl.cheryme.top

[U55] PHP：match 表达式
来源：http://dno.jinyuanbaomall.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cni.wangdashe.top

[U56] PHP：命名参数
来源：http://ylm.ivvv.top

f(a: 1, b: 2)
来源：http://hae.jiagoushi.top

[U57] PHP：字符串插值
来源：http://qel.fehbvm.com

"值: {$a}"
来源：http://ztq.fengsongda.top

[U58] PHP：数组三件套
来源：http://mgr.fzhhl.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vnd.chenlongwang.top

[U59] PHP：自定义排序
来源：http://vcu.zhongyouzk.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fge.tarul.cn

[U60] PHP：JSON 编解码
来源：http://sgx.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pgw.pengpengdd.cyou

[U61] PHP：正则
来源：http://hwq.xuanzx.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ncz.fengsongda.top

[U62] PHP：日期对象
来源：http://fgc.aizwys.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ill.zhengqikj.top

[U63] PHP：文件读写
来源：http://tky.yanxiufei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dwm.0kj1m.cn

[U64] PHP：目录遍历
来源：http://jkc.jiagoushi.top

glob("dir/*.php");  scandir("dir");
来源：http://pvn.tian-w.cn

[U65] PHP：会话
来源：http://bzf.chenjidiqi.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://ntm.hesvh.cn

[U66] PHP：设置 Cookie
来源：http://ngv.pengpengdd.cyou

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mcq.havefunace.top

[U67] PHP：处理文件上传
来源：http://hro.52xcode.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rvv.birdmap.top

[U68] PHP：PDO 连接
来源：http://bob.sjlbkw.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fkf.cheryme.top

[U69] PHP：PDO 预处理
来源：http://sxq.fzhhl.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ptv.yangfankeji.com

[U70] PHP：PDO 事务
来源：http://rop.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kxg.yuxming.cn

[U71] PHP：抛出异常
来源：http://ddz.sweek.top

throw new RuntimeException("失败", 500);
来源：http://wgu.zhengqikj.top

[U72] PHP：写错误日志
来源：http://fhn.fktsv.cn

error_log("失败: " . $e->getMessage());
来源：http://kvz.zhaomingkeji.xyz

[U73] PHP：读取 ini 配置
来源：http://xyq.daxiang520.top

parse_ini_file("config.ini", true)
来源：http://rzc.jqgufenzy.top

[U74] PHP：读取环境变量
来源：http://fdu.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://izh.yj20258.top

[U75] PHP：依赖注入
来源：http://bto.jinyuanbaomall.cn

composer require psr/container
来源：http://med.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://ekk.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ojn.iojbl.cn

[U77] PHP：模板渲染
来源：http://knx.chenzaomai.com

composer require twig/twig
来源：http://fkz.redwolf501.top

[U78] PHP：单元测试
来源：http://fjy.daxiang520.top

composer require --dev phpunit/phpunit
来源：http://mzu.cucudq.cn

[U79] PHP：静态分析
来源：http://tfk.wangdashe.top

composer require --dev phpstan/phpstan
来源：http://ezj.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://ddi.vehdjk.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://kwk.smart0.xyz

[U81] JS：初始化项目
来源：http://pwx.9152youxi.cn

npm init -y;  npm i express
来源：http://ybh.kuanghao11.cn

[U82] JS：package.json 脚本
来源：http://vok.yj202588.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sah.ehwqpu.com

[U83] JS：ES Module 导入导出
来源：http://ntx.dashuyun.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yvz.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://bah.jlsjyb.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tla.zdqjudy.top

[U85] JS：可选链
来源：http://dzx.uphjek.com

a?.b?.c
来源：http://fea.hcnkem.com

[U86] JS：空值合并
来源：http://imq.tianlin.xyz

a ?? b
来源：http://jlz.fehbvm.com

[U87] JS：解构默认值
来源：http://sbi.quarkkingdee.top

const { a = 1, b = 2 } = obj;
来源：http://fph.ehwqpu.com

[U88] JS：对象展开合并
来源：http://myn.yvedp.cn

{ ...a, ...b }
来源：http://utm.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://orh.fktsv.cn

[...new Set(arr)]
来源：http://kyp.jyoumei.cn

[U90] JS：数字数组排序
来源：http://unw.fanxiaobao.xyz

[...arr].sort((a, b) => a - b)
来源：http://umz.ydzc1.top

[U91] JS：对象键值遍历
来源：http://rgh.iojbl.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ogf.zhongyouzk.top

[U92] JS：深拷贝
来源：http://plr.ywan-chungtsiang.top

structuredClone(obj)
来源：http://wwy.tianlin.xyz

[U93] JS：模板字符串
来源：http://nuq.chenzaomai.com

`共 ${n} 条`
来源：http://ivh.ppjwa.cn

[U94] JS：箭头函数
来源：http://dpe.wangshuangyany.cn

const double = x => x * 2;
来源：http://zro.xuanzx.com

[U95] JS：Promise 包装
来源：http://atu.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://hhd.zhijiandao.cn

[U96] JS：async/await 与异常
来源：http://vnu.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dxm.hysaishi.cn

[U97] JS：并发请求
来源：http://tud.uphjek.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://hou.ybcxt.top

[U98] JS：fetch 带 JSON
来源：http://rgo.sysykeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nev.tian-w.cn

[U99] JS：事件监听
来源：http://dsb.birdmap.top

el.addEventListener("click", e => {})
来源：http://omp.yj20258888.top

[U100] JS：DOM 查询
来源：http://lei.jlsjyb.cn

document.querySelector(".item")
来源：http://lwh.yuanzhike.top

[U101] JS：classList 操作
来源：http://fbc.haohaochexian.top

el.classList.toggle("active")
来源：http://jon.shangyingyoupin.top

[U102] JS：本地存储
来源：http://maq.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://atp.tarul.cn

[U103] JS：定时器
来源：http://gwz.hysaishi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cif.xuanzx.com

[U104] JS：防抖
来源：http://bny.zhijiandao.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qep.yanxiufei.cn

[U105] JS：节流
来源：http://shb.c1oappe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ccd.zhijiandao.cn

[U106] JS：日期格式化
来源：http://qzo.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nan.svipenyu.cn

[U107] JS：数字千分位
来源：http://exm.feifeiyinyue.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zgb.sjlbkw.cn

[U108] JS：随机整数
来源：http://ujl.epnwcf.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yty.fktsv.cn

[U109] JS：数组分组
来源：http://gan.zhijiandao.cn

Object.groupBy(arr, x => x.type)
来源：http://npr.jinghuilouyu.cn

[U110] JS：数组分块
来源：http://vcq.316326.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sjx.xinyue.icu

[U111] JS：对象转 Map
来源：http://kgg.zdqjudy.top

new Map(Object.entries(obj))
来源：http://oib.cucudq.cn

[U112] JS：字符串补位
来源：http://yok.cqqwz.cn

"7".padStart(3, "0")
来源：http://ulk.pengpengdd.cyou

[U113] JS：正则替换全部
来源：http://dde.vehdjk.com

s.replaceAll("a", "b")
来源：http://hmg.ydzc1.top

[U114] JS：JSON 深比较
来源：http://zyh.redwolf501.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fem.epnwcf.com

[U115] JS：生成 UUID
来源：http://sce.yueranfly.top

crypto.randomUUID()
来源：http://gyf.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://hoc.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://hym.kuanghao11.cn

[U117] JS：单元测试
来源：http://lks.jianghu66.top

npm i -D vitest;  npx vitest
来源：http://hpd.dianchejie.cn

[U118] JS：开发服务器
来源：http://tou.ydjk.org.cn

npm i -D vite;  npx vite
来源：http://uee.zhixingplan.top

[U119] JS：生产构建
来源：http://vbu.cdnleiting.top

npx vite build
来源：http://alv.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://tzo.shangyingyoupin.top

import.meta.env.VITE_API_URL
来源：http://lco.jinyuanbaomall.cn

================================================================================
来源：http://zqg.nanxinkj.top

统计汇总
来源：http://dfd.shanyushiyangkeji.top

================================================================================
来源：http://bif.xuetiantiany.cn

按语言统计（条）：
来源：http://wts.jinqigufen.top

Python ......... 252
来源：http://ded.sufxvd.cn

PHP ............ 252
来源：http://uwd.fktsv.cn

JavaScript ..... 252
来源：http://osa.nanxuanxn.top

TypeScript ..... 212
来源：http://yxt.ppjwa.cn

Java ........... 212
来源：http://bpz.vqdsnc.cn

Go ............. 212
来源：http://ygm.feifeiyinyue.top

Ruby ........... 212
来源：http://ash.daria6918.cn

C# ............. 212
来源：http://whd.ybcxt.top

C .............. 30
来源：http://piz.zhengqikj.top

C++ ............ 30
来源：http://tjn.ybcxt.top

SQL ............ 90
来源：http://bes.hnqzz.top

Bash ........... 80
来源：http://fgi.ivvv.top

Kotlin ......... 15
来源：http://rrt.sjlbkw.cn

Swift .......... 15
来源：http://wgl.xziqi.cn

Lua ............ 10
来源：http://gjf.gaohongyu789.top

Perl ........... 10
来源：http://vfr.hysaishi.cn

Scala .......... 10
来源：http://yys.tian-w.cn

------------------------------------
来源：http://tcn.zhongyouzk.top

合计 ........... 2106 条
来源：http://sep.guannengcc.top

按章节统计：
来源：http://tbw.nanxuanxn.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hck.zhoulong.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kuh.yueranfly.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xtb.yj20258.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iqf.hcnkem.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dmh.ywan-chungtsiang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ymz.fktsv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pno.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ykk.316326.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bpy.yonumen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pgr.9152youxi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ohm.0kj1m.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://icm.yueranfly.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://joj.hysaishi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bkl.zhixingplan.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vld.fanxiaobao.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tci.sufxvd.cn

Q SQL 专题                              90
来源：http://toe.zhoulong.xyz

R Bash 专题                             80
来源：http://yhy.sysykeji.top

S C / C++ 专题                          60
来源：http://zpy.xziqi.cn

T 其他语言补充                          60
来源：http://nbx.jiagoushi.top

U 高频实用片段                         120
来源：http://exn.cqqwz.cn

------------------------------------
来源：http://htp.smart0.xyz

合计                                  2106 条
来源：http://eky.sweek.top

--------------------------------------------------------------------------------
来源：http://wxe.ctjpmb.com

使用提醒
来源：http://epg.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://gdx.xingfuxueyuan.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wen.gotoacloud.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ayg.yangfankeji.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rel.yonumen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://wxn.yuanzhike.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rqe.feifeiyinyue.top

—— 文件结束 ——
来源：http://mdu.nanxuanxn.top

================================================================================
来源：http://tnr.zdbjq.cn

程序语言常见例子速查手册（2024 版）
来源：http://lwc.aibaodan.cn

Common Programming Examples Cheat Book
来源：http://bxv.fehbvm.com

================================================================================
来源：http://fla.svipenyu.cn

【收录内容】
来源：http://udu.gogol.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://pib.guannengcc.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zds.jyoumei.cn

SQL · Bash · C · C++
来源：http://avh.snrcjt.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jjs.guannengcc.top

【使用说明】
来源：http://ptt.0kj1m.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cet.jianghu66.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wki.xingfuxueyuan.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pgz.yj20258888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xac.gogol.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tfn.cucudq.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uml.uphjek.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cam.fengsongda.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xkm.vehdjk.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yes.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lgp.meibo888.top


<!-- 参考信息 -->