代发 wailian999

[U11] Py：生成器表达式
来源：http://gdq.zhixingplan.top

(x * 2 for x in arr)
来源：http://cfs.zhengqikj.top

[U12] Py：取出现最多的 3 个元素
来源：http://ckv.gogol.net.cn

Counter(arr).most_common(3)
来源：http://lrx.tarul.cn

[U13] Py：固定长度队列
来源：http://paz.hywenlv.cn

deque(maxlen=10)
来源：http://zxm.jlsjyb.cn

[U14] Py：分组收集到列表
来源：http://fyd.xuetiantiany.cn

defaultdict(list)
来源：http://heb.shuidangran.top

[U15] Py：高精度计时
来源：http://lux.jinqigfzy.top

t = time.perf_counter()
来源：http://iaw.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://duy.yanxiufei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tdl.cheryme.top

[U17] Py：初始化日志
来源：http://lft.sufxvd.cn

logging.basicConfig(level=logging.INFO)
来源：http://tbw.zhongyouzk.top

[U18] Py：预编译正则
来源：http://pag.daxiang520.top

pat = re.compile(r"\d+")
来源：http://idb.cheryme.top

[U19] Py：正则替换带回调
来源：http://xem.52xcode.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nqn.chenjidiqi.icu

[U20] Py：缓存函数结果
来源：http://aiq.bjfxy.top

@functools.lru_cache(maxsize=None)
来源：http://svu.zhijiandao.cn

[U21] Py：自定义上下文管理器
来源：http://ysf.sysykeji.top

@contextlib.contextmanager
来源：http://loq.aibaodan.cn

[U22] Py：矩阵转置
来源：http://ffp.9152youxi.cn

list(zip(*m))
来源：http://qar.jiagoushi.top

[U23] Py：分块读取大文件
来源：http://zef.chenlongwang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ncu.xingfuxueyuan.xyz

[U24] Py：路径操作
来源：http://mdd.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bmb.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://rcb.zhijiandao.cn

csv.DictReader(f)
来源：http://jfa.tanke756.top

[U26] Py：并发下载
来源：http://hxb.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bkn.shanyushiyangtech.top

[U27] Py：异步 HTTP
来源：http://skb.zhixingplan.top

aiohttp.ClientSession() 配合 async with
来源：http://zas.ywan-chungtsiang.top

[U28] Py：类型别名
来源：http://zet.9152youxi.cn

UserId = int
来源：http://wgt.zhongyouzk.top

[U29] Py：属性校验
来源：http://hux.zhengqikj.top

@property 与 @x.setter 配合
来源：http://jum.cdnleiting.top

[U30] Py：数据类
来源：http://vxa.nanxinkj.top

@dataclass(slots=True)
来源：http://jac.pengpengdd.cyou

[U31] Py：单测
来源：http://txx.9152youxi.cn

python -m pytest -q
来源：http://dhb.meibo888.top

[U32] Py：代码格式化
来源：http://atc.daxiang520.top

ruff format . && ruff check --fix .
来源：http://ejd.ctjpmb.com

[U33] Py：打包发布
来源：http://lgd.hcnkem.com

python -m build  （依赖 pyproject.toml）
来源：http://zqc.yfazqb.com

[U34] Py：判断编码
来源：http://gec.xuetiantiany.cn

chardet.detect(raw)
来源：http://top.ydzc1.top

[U35] Py：发送邮件
来源：http://zgz.chenlongwang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zwy.tarul.cn

[U36] Py：定时任务
来源：http://kuh.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://jzy.pengpengdd.cyou

[U37] Py：读写 Excel
来源：http://psl.cheryme.top

pandas.read_excel / DataFrame.to_excel
来源：http://jrd.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://jxw.yj202588.top

Path(__file__).resolve().parent
来源：http://ljo.zhoulong.xyz

[U39] Py：判断是否在交互环境
来源：http://swy.gaohongyu789.top

sys.stdout.isatty()
来源：http://rzf.fzhhl.top

[U40] Py：打印到标准错误
来源：http://erq.daxiang520.top

print("err", file=sys.stderr)
来源：http://nii.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://tyn.52xcode.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hyx.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://ruf.ydzc1.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vmk.xuanzx.com

[U43] PHP：声明命名空间
来源：http://klo.gzhubu.top

namespace App\Http;
来源：http://duw.xuanzx.com

[U44] PHP：开启严格类型
来源：http://kud.yongpay.top

declare(strict_types=1);
来源：http://tsn.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://but.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jip.yvedp.cn

[U46] PHP：可空类型
来源：http://rqg.chenjidiqi.icu

?string $name = null
来源：http://ojo.daxiang520.top

[U47] PHP：联合类型
来源：http://sct.uphjek.com

int|string $id
来源：http://prv.zhengqikj.top

[U48] PHP：纯枚举
来源：http://zjf.jqgfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ewv.xuanzx.com

[U49] PHP：只读属性
来源：http://xca.ybcxt.top

public readonly string $name
来源：http://zmv.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://nvi.jyoumei.cn

public function __construct(private int $id) {}
来源：http://qpg.yuanzhike.top

[U51] PHP：数组解构
来源：http://amr.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://zis.pycfn.com

[U52] PHP：箭头函数
来源：http://ypv.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://qcd.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://ose.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://yjs.cucudq.cn

[U54] PHP：空安全调用
来源：http://sxh.pycfn.com

$obj?->method()
来源：http://fmo.bbcook.cn

[U55] PHP：match 表达式
来源：http://yqg.chenzaomai.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sdd.gzhubu.top

[U56] PHP：命名参数
来源：http://syb.hesvh.cn

f(a: 1, b: 2)
来源：http://ipb.zdqjudy.top

[U57] PHP：字符串插值
来源：http://auo.daxiang520.top

"值: {$a}"
来源：http://tio.feifeiyinyue.top

[U58] PHP：数组三件套
来源：http://fva.fktsv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tdt.jinyuanbaomall.cn

[U59] PHP：自定义排序
来源：http://jcc.jiagoushi.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gxs.xingfuxueyuan.xyz

[U60] PHP：JSON 编解码
来源：http://ywp.yvedp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://osf.iojbl.cn

[U61] PHP：正则
来源：http://ptv.yuanzhike.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sji.zhaomingkeji.xyz

[U62] PHP：日期对象
来源：http://zjp.shanyushiyangtech.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gak.xziqi.cn

[U63] PHP：文件读写
来源：http://poi.yuanzhike.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gco.shangyingyoupin.top

[U64] PHP：目录遍历
来源：http://izv.chenzaomai.com

glob("dir/*.php");  scandir("dir");
来源：http://iio.hnxiangtu.top

[U65] PHP：会话
来源：http://qgr.jiagoushi.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nfs.yvedp.cn

[U66] PHP：设置 Cookie
来源：http://sxd.chenzaomai.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gxo.smart0.xyz

[U67] PHP：处理文件上传
来源：http://huk.jiagoushi.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://apv.andypj.xyz

[U68] PHP：PDO 连接
来源：http://les.nanxinkj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mzx.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://jhr.andypj.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bjo.yj20258888.top

[U70] PHP：PDO 事务
来源：http://hpd.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://idf.jqgfzy.top

[U71] PHP：抛出异常
来源：http://wkz.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://hhl.xuetiantiany.cn

[U72] PHP：写错误日志
来源：http://itn.tanke756.top

error_log("失败: " . $e->getMessage());
来源：http://jrv.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://vmk.nwbrower.top

parse_ini_file("config.ini", true)
来源：http://ubj.jianghu66.top

[U74] PHP：读取环境变量
来源：http://ahr.quarkkingdee.top

getenv("APP_ENV") ?: "production"
来源：http://zof.pycfn.com

[U75] PHP：依赖注入
来源：http://qxh.jqgufenzy.top

composer require psr/container
来源：http://bnc.gotoacloud.top

[U76] PHP：简单路由
来源：http://bfl.hywenlv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bdf.yonumen.top

[U77] PHP：模板渲染
来源：http://nlr.shanyushiyangtech.top

composer require twig/twig
来源：http://kem.havefunace.top

[U78] PHP：单元测试
来源：http://ugl.wangdashe.top

composer require --dev phpunit/phpunit
来源：http://qun.zycfv.cn

[U79] PHP：静态分析
来源：http://xof.pycfn.com

composer require --dev phpstan/phpstan
来源：http://sqd.jinqigufen.top

[U80] PHP：代码规范修复
来源：http://exc.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://azr.yuanzhike.top

[U81] JS：初始化项目
来源：http://fqt.ydzc1.top

npm init -y;  npm i express
来源：http://gcz.nanxuanxn.top

[U82] JS：package.json 脚本
来源：http://tzq.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qzj.hcnkem.com

[U83] JS：ES Module 导入导出
来源：http://wnu.jyoumei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://eta.tarul.cn

[U84] JS：CommonJS 写法
来源：http://krc.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://eki.yanxiufei.cn

[U85] JS：可选链
来源：http://dkj.aizwys.cn

a?.b?.c
来源：http://uzn.yfazqb.com

[U86] JS：空值合并
来源：http://yef.aizwys.cn

a ?? b
来源：http://bxl.daria6918.cn

[U87] JS：解构默认值
来源：http://bpm.iojbl.cn

const { a = 1, b = 2 } = obj;
来源：http://ctv.ehwqpu.com

[U88] JS：对象展开合并
来源：http://rzm.shzxlz.cn

{ ...a, ...b }
来源：http://lnz.quarkkingdee.top

[U89] JS：数组去重
来源：http://ytz.nanxuanxn.top

[...new Set(arr)]
来源：http://krc.svipenyu.cn

[U90] JS：数字数组排序
来源：http://elh.sufxvd.cn

[...arr].sort((a, b) => a - b)
来源：http://rkc.zdqjudy.top

[U91] JS：对象键值遍历
来源：http://hdp.yvedp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bfp.shuidangran.top

[U92] JS：深拷贝
来源：http://tuy.sxryk.cn

structuredClone(obj)
来源：http://crs.cashguo.top

[U93] JS：模板字符串
来源：http://oki.zhixingplan.top

`共 ${n} 条`
来源：http://deg.zhiwuduotai.top

[U94] JS：箭头函数
来源：http://coc.zhengqikj.top

const double = x => x * 2;
来源：http://rsb.yfazqb.com

[U95] JS：Promise 包装
来源：http://hbg.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://xkj.yuxming.cn

[U96] JS：async/await 与异常
来源：http://hyv.yvedp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://frv.jinyuanbaomall.cn

[U97] JS：并发请求
来源：http://emw.jianghu66.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://quz.cucudq.cn

[U98] JS：fetch 带 JSON
来源：http://qiw.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rzf.gaohongyu789.top

[U99] JS：事件监听
来源：http://yvz.chenzaomai.com

el.addEventListener("click", e => {})
来源：http://enk.epnwcf.com

[U100] JS：DOM 查询
来源：http://msb.tanke756.top

document.querySelector(".item")
来源：http://hlc.sysykeji.top

[U101] JS：classList 操作
来源：http://yxe.ybcxt.top

el.classList.toggle("active")
来源：http://zoy.fzhhl.top

[U102] JS：本地存储
来源：http://fmc.shanyushiyangtech.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tmm.feifeiyinyue.top

[U103] JS：定时器
来源：http://tcf.ydjk.org.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fjc.hysaishi.cn

[U104] JS：防抖
来源：http://qjx.xinyue.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dqe.jinghuilouyu.cn

[U105] JS：节流
来源：http://rhs.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jrz.jinqigufen.top

[U106] JS：日期格式化
来源：http://qid.hysaishi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zcq.hcnkem.com

[U107] JS：数字千分位
来源：http://cxr.ivvv.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://thr.redwolf501.top

[U108] JS：随机整数
来源：http://rkk.ydzc1.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cjr.jqgufenzy.top

[U109] JS：数组分组
来源：http://qzz.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://hek.xziqi.cn

[U110] JS：数组分块
来源：http://lap.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vzs.zycfv.cn

[U111] JS：对象转 Map
来源：http://zdq.daxiang520.top

new Map(Object.entries(obj))
来源：http://ies.fktsv.cn

[U112] JS：字符串补位
来源：http://gtv.vehdjk.com

"7".padStart(3, "0")
来源：http://ulo.ivvv.top

[U113] JS：正则替换全部
来源：http://xcc.yueranfly.top

s.replaceAll("a", "b")
来源：http://dil.yueranfly.top

[U114] JS：JSON 深比较
来源：http://bwe.fengsongda.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qzo.jiagoushi.top

[U115] JS：生成 UUID
来源：http://quz.sxryk.cn

crypto.randomUUID()
来源：http://ewp.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://znt.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://yxf.aizwys.cn

[U117] JS：单元测试
来源：http://jzl.sysykeji.top

npm i -D vitest;  npx vitest
来源：http://jji.daria6918.cn

[U118] JS：开发服务器
来源：http://aqv.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://amt.ivvv.top

[U119] JS：生产构建
来源：http://iin.uphjek.com

npx vite build
来源：http://bpl.mhx1999.top

[U120] JS：读取环境变量（Vite）
来源：http://uqq.fengsongda.top

import.meta.env.VITE_API_URL
来源：http://gag.uphjek.com

================================================================================
来源：http://zyb.zdqjudy.top

统计汇总
来源：http://gcz.tarul.cn

================================================================================
来源：http://pht.nanxuanxn.top

按语言统计（条）：
来源：http://uub.yongpay.top

Python ......... 252
来源：http://npc.zhaomingkeji.xyz

PHP ............ 252
来源：http://whv.jianghu66.top

JavaScript ..... 252
来源：http://kva.dianchejie.cn

TypeScript ..... 212
来源：http://lkt.gzhubu.top

Java ........... 212
来源：http://szn.zhiwuduotai.top

Go ............. 212
来源：http://svl.nanxuanxn.top

Ruby ........... 212
来源：http://lua.jinyuanbaomall.cn

C# ............. 212
来源：http://xrn.gogol.net.cn

C .............. 30
来源：http://uzk.tanke756.top

C++ ............ 30
来源：http://fpm.ydjk.org.cn

SQL ............ 90
来源：http://oee.birdmap.top

Bash ........... 80
来源：http://mei.ydjk.org.cn

Kotlin ......... 15
来源：http://mln.zdqjudy.top

Swift .......... 15
来源：http://xnb.bjfxy.top

Lua ............ 10
来源：http://dar.hfpthk.cn

Perl ........... 10
来源：http://eue.fktsv.cn

Scala .......... 10
来源：http://irs.yongpay.top

------------------------------------
来源：http://jqs.bbcook.cn

合计 ........... 2106 条
来源：http://oyt.yuxming.cn

按章节统计：
来源：http://jzj.dashuyun.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wdy.redwolf501.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://okj.jinyuanbaomall.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ixc.zhengqikj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dbp.jinghuilouyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://upr.sufxvd.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wnh.gogol.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xxn.birdmap.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ial.epnwcf.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://maz.cheryme.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bsj.ydzc1.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xtp.ctjpmb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oyr.fktsv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xfw.tarul.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ocf.zhixingplan.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pqz.52xcode.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pjy.hfpthk.cn

Q SQL 专题                              90
来源：http://ush.sufxvd.cn

R Bash 专题                             80
来源：http://zcn.nwbrower.top

S C / C++ 专题                          60
来源：http://yyb.shzxlz.cn

T 其他语言补充                          60
来源：http://ccq.hnqzz.top

U 高频实用片段                         120
来源：http://odc.jyoumei.cn

------------------------------------
来源：http://coo.nwbrower.top

合计                                  2106 条
来源：http://moi.havefunace.top

--------------------------------------------------------------------------------
来源：http://sjc.gzhubu.top

使用提醒
来源：http://jgk.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://sbd.aizwys.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gvo.sysykeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qjy.yonumen.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vtl.zhijiandao.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zop.aibaodan.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gth.yvedp.cn

—— 文件结束 ——
来源：http://bcd.zhaomingkeji.xyz

================================================================================
来源：http://aqe.sysykeji.top

程序语言常见例子速查手册（2024 版）
来源：http://jhe.jiagoushi.top

Common Programming Examples Cheat Book
来源：http://ayz.yuanzhike.top

================================================================================
来源：http://pqs.hammf.cn

【收录内容】
来源：http://dvy.hongshengwenyu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://epi.yuxming.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ylp.epnwcf.com

SQL · Bash · C · C++
来源：http://efz.yueranfly.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bwe.jianghu66.top

【使用说明】
来源：http://ojw.jiagoushi.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zic.nanxuanxn.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://myj.guannengcc.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://guz.pengpengdd.cyou

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ebw.xylfe.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fww.zhaomingkeji.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mal.haohaochexian.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nyr.jinyuanbaomall.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xty.shzxlz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zil.vqdsnc.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uwn.aibaodan.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kex.hfpthk.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pip.tarul.cn

【文件统计】
来源：http://emu.zhoulong.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mim.zhixingplan.top


<!-- 参考信息 -->