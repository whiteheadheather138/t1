代发 wailian999

[U05] Py：列表去重且保序
来源：http://xcu.shanyushiyangtech.top

list(dict.fromkeys(arr))
来源：http://caj.zhengqikj.top

[U06] Py：合并两个字典
来源：http://znp.fengsongda.top

{**a, **b}
来源：http://bcu.wangdashe.top

[U07] Py：反转字典键值
来源：http://dzs.sweek.top

{v: k for k, v in d.items()}
来源：http://yld.jiagoushi.top

[U08] Py：展平二维列表
来源：http://ngl.ivvv.top

[y for x in nested for y in x]
来源：http://jji.hammf.cn

[U09] Py：字典取最大值的键
来源：http://vzb.guannengcc.top

max(d, key=d.get)
来源：http://yzp.vehdjk.com

[U10] Py：按值排序字典
来源：http://kli.shuidangran.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ddi.hesvh.cn

[U11] Py：生成器表达式
来源：http://reh.jqgufenzy.top

(x * 2 for x in arr)
来源：http://pts.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hnw.vqdsnc.cn

Counter(arr).most_common(3)
来源：http://mpi.zhengqikj.top

[U13] Py：固定长度队列
来源：http://fdd.zhengqikj.top

deque(maxlen=10)
来源：http://tqm.aizwys.cn

[U14] Py：分组收集到列表
来源：http://luy.jyoumei.cn

defaultdict(list)
来源：http://abr.yuxming.cn

[U15] Py：高精度计时
来源：http://ybh.vqdsnc.cn

t = time.perf_counter()
来源：http://vhi.snrcjt.cn

[U16] Py：命令行参数解析
来源：http://ejs.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://inc.hcnkem.com

[U17] Py：初始化日志
来源：http://nec.sxryk.cn

logging.basicConfig(level=logging.INFO)
来源：http://vsg.yfazqb.com

[U18] Py：预编译正则
来源：http://gkh.uphjek.com

pat = re.compile(r"\d+")
来源：http://uty.gotoacloud.top

[U19] Py：正则替换带回调
来源：http://dbd.shzxlz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wkk.yongpay.top

[U20] Py：缓存函数结果
来源：http://dmj.shanyushiyangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://haw.316326.xyz

[U21] Py：自定义上下文管理器
来源：http://ngo.zhixingplan.top

@contextlib.contextmanager
来源：http://roj.yonumen.top

[U22] Py：矩阵转置
来源：http://rnw.yanxiufei.cn

list(zip(*m))
来源：http://moq.meibo888.top

[U23] Py：分块读取大文件
来源：http://lvr.svipenyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dmo.yj202588.top

[U24] Py：路径操作
来源：http://pax.shanyushiyangtech.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://npt.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://vsy.birdmap.top

csv.DictReader(f)
来源：http://fcw.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://sjl.zycfv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fui.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://ota.fzhhl.top

aiohttp.ClientSession() 配合 async with
来源：http://pyd.fanxiaobao.xyz

[U28] Py：类型别名
来源：http://nnt.cheryme.top

UserId = int
来源：http://lop.yj20258.top

[U29] Py：属性校验
来源：http://kor.jyoumei.cn

@property 与 @x.setter 配合
来源：http://neh.shanyushiyangkeji.top

[U30] Py：数据类
来源：http://dfd.ctjpmb.com

@dataclass(slots=True)
来源：http://yjl.redwolf501.top

[U31] Py：单测
来源：http://iby.ctjpmb.com

python -m pytest -q
来源：http://chf.52xcode.cn

[U32] Py：代码格式化
来源：http://jku.yvedp.cn

ruff format . && ruff check --fix .
来源：http://ggi.haohaochexian.top

[U33] Py：打包发布
来源：http://iac.zdbjq.cn

python -m build  （依赖 pyproject.toml）
来源：http://fbq.jinqigufen.top

[U34] Py：判断编码
来源：http://mzm.redwolf501.top

chardet.detect(raw)
来源：http://iee.gzhubu.top

[U35] Py：发送邮件
来源：http://grv.xingfuxueyuan.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://egk.guowangkeji.top

[U36] Py：定时任务
来源：http://nnc.guannengcc.top

schedule.every(10).minutes.do(job)
来源：http://fgh.316326.xyz

[U37] Py：读写 Excel
来源：http://niq.aibaodan.cn

pandas.read_excel / DataFrame.to_excel
来源：http://twf.jinyuanbaomall.cn

[U38] Py：获取脚本所在目录
来源：http://wnj.sjlbkw.cn

Path(__file__).resolve().parent
来源：http://rcc.aibaodan.cn

[U39] Py：判断是否在交互环境
来源：http://mvc.dianchejie.cn

sys.stdout.isatty()
来源：http://gmt.hywenlv.cn

[U40] Py：打印到标准错误
来源：http://rdy.sjlbkw.cn

print("err", file=sys.stderr)
来源：http://asz.zhaomingkeji.xyz

[U41] PHP：初始化 Composer 项目
来源：http://nyv.fzhhl.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fic.sjlbkw.cn

[U42] PHP：PSR-4 自动加载
来源：http://ohr.vehdjk.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://klp.dashuyun.cn

[U43] PHP：声明命名空间
来源：http://ytt.zhaomingkeji.xyz

namespace App\Http;
来源：http://urw.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://lzv.tianlin.xyz

declare(strict_types=1);
来源：http://ygs.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://kye.fehbvm.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://fpj.yuanzhike.top

[U46] PHP：可空类型
来源：http://ejj.zdqjudy.top

?string $name = null
来源：http://esp.hywenlv.cn

[U47] PHP：联合类型
来源：http://xml.sweek.top

int|string $id
来源：http://dms.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://klz.iojbl.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yxv.shuidangran.top

[U49] PHP：只读属性
来源：http://ysn.meibo888.top

public readonly string $name
来源：http://wnl.jqgufenzy.top

[U50] PHP：构造器属性提升
来源：http://unz.mhx1999.top

public function __construct(private int $id) {}
来源：http://grq.cqqwz.cn

[U51] PHP：数组解构
来源：http://fna.shanyushiyangkeji.top

[$a, $b] = $arr;
来源：http://gmh.yj202588.top

[U52] PHP：箭头函数
来源：http://lva.zycfv.cn

$double = fn($x) => $x * 2;
来源：http://awm.cdnleiting.top

[U53] PHP：空合并运算符
来源：http://gql.daxiang520.top

$v = $a ?? $b ?? "default";
来源：http://ewb.jinyuanbaomall.cn

[U54] PHP：空安全调用
来源：http://bfh.mhx1999.top

$obj?->method()
来源：http://rel.c1oappe.top

[U55] PHP：match 表达式
来源：http://aub.tanke756.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eou.jinqigufen.top

[U56] PHP：命名参数
来源：http://fng.yanxiufei.cn

f(a: 1, b: 2)
来源：http://cwb.yj20258888.top

[U57] PHP：字符串插值
来源：http://wyf.chenlongwang.top

"值: {$a}"
来源：http://nkd.yfazqb.com

[U58] PHP：数组三件套
来源：http://gvx.meibo888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dvk.wangshuangyany.cn

[U59] PHP：自定义排序
来源：http://sft.fehbvm.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wan.zdqjudy.top

[U60] PHP：JSON 编解码
来源：http://yvz.dianchejie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://chn.0kj1m.cn

[U61] PHP：正则
来源：http://lsf.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://omu.gzhubu.top

[U62] PHP：日期对象
来源：http://jxb.ydzc1.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wss.zdqjudy.top

[U63] PHP：文件读写
来源：http://dgd.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wkz.shuidangran.top

[U64] PHP：目录遍历
来源：http://byc.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://xoo.mhx1999.top

[U65] PHP：会话
来源：http://fcw.sweek.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pbs.cashguo.top

[U66] PHP：设置 Cookie
来源：http://njb.cucudq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://slw.hongshengwenyu.top

[U67] PHP：处理文件上传
来源：http://shf.kuanghao11.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gle.xingfuxueyuan.xyz

[U68] PHP：PDO 连接
来源：http://xzi.yonumen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nrp.shanyushiyangkeji.top

[U69] PHP：PDO 预处理
来源：http://qac.iojbl.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tlt.zdqjudy.top

[U70] PHP：PDO 事务
来源：http://env.jinyuanbaomall.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gux.zhixingplan.top

[U71] PHP：抛出异常
来源：http://nwx.jqgufenzy.top

throw new RuntimeException("失败", 500);
来源：http://ibw.ppjwa.cn

[U72] PHP：写错误日志
来源：http://oce.zhongyouzk.top

error_log("失败: " . $e->getMessage());
来源：http://bsk.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://qct.zhiwuduotai.top

parse_ini_file("config.ini", true)
来源：http://ybi.birdmap.top

[U74] PHP：读取环境变量
来源：http://gka.yuxming.cn

getenv("APP_ENV") ?: "production"
来源：http://coo.yangfankeji.com

[U75] PHP：依赖注入
来源：http://sjj.sjlbkw.cn

composer require psr/container
来源：http://yix.yongpay.top

[U76] PHP：简单路由
来源：http://cyk.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jav.zhixingplan.top

[U77] PHP：模板渲染
来源：http://xux.chenlongwang.top

composer require twig/twig
来源：http://dao.ivvv.top

[U78] PHP：单元测试
来源：http://zlq.epnwcf.com

composer require --dev phpunit/phpunit
来源：http://xbp.sxryk.cn

[U79] PHP：静态分析
来源：http://grk.ppjwa.cn

composer require --dev phpstan/phpstan
来源：http://fns.jlsjyb.cn

[U80] PHP：代码规范修复
来源：http://wst.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jqg.gzhubu.top

[U81] JS：初始化项目
来源：http://zps.c1oappe.top

npm init -y;  npm i express
来源：http://crp.yuxming.cn

[U82] JS：package.json 脚本
来源：http://kxf.birdmap.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jbf.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://hle.quarkkingdee.top

export const a = 1;  import { a } from "./m.js";
来源：http://fwh.cashguo.top

[U84] JS：CommonJS 写法
来源：http://own.zdqjudy.top

module.exports = { a };  const { a } = require("./m");
来源：http://qax.nanxuanxn.top

[U85] JS：可选链
来源：http://yke.dashuyun.cn

a?.b?.c
来源：http://pwx.shanyushiyangkeji.top

[U86] JS：空值合并
来源：http://ljx.xuetiantiany.cn

a ?? b
来源：http://jug.zhixingplan.top

[U87] JS：解构默认值
来源：http://oip.xuetiantiany.cn

const { a = 1, b = 2 } = obj;
来源：http://lmc.hcnkem.com

[U88] JS：对象展开合并
来源：http://ldz.bbcook.cn

{ ...a, ...b }
来源：http://zmc.zhaomingkeji.xyz

[U89] JS：数组去重
来源：http://eci.jqgfzy.top

[...new Set(arr)]
来源：http://drl.yongpay.top

[U90] JS：数字数组排序
来源：http://wwu.jiagoushi.top

[...arr].sort((a, b) => a - b)
来源：http://gjn.cashguo.top

[U91] JS：对象键值遍历
来源：http://fze.yuanzhike.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lne.hammf.cn

[U92] JS：深拷贝
来源：http://xse.chenjidiqi.icu

structuredClone(obj)
来源：http://ljh.gaohongyu789.top

[U93] JS：模板字符串
来源：http://wwe.tanke756.top

`共 ${n} 条`
来源：http://wdr.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://dll.vqdsnc.cn

const double = x => x * 2;
来源：http://owh.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://euu.chenjidiqi.icu

new Promise((resolve, reject) => {})
来源：http://pte.tanke756.top

[U96] JS：async/await 与异常
来源：http://xyn.vehdjk.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sqn.vehdjk.com

[U97] JS：并发请求
来源：http://leo.kuanghao11.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fvw.shanyushiyangtech.top

[U98] JS：fetch 带 JSON
来源：http://bgz.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wan.yuanzhike.top

[U99] JS：事件监听
来源：http://qng.yuanzhike.top

el.addEventListener("click", e => {})
来源：http://rfs.pengpengdd.cyou

[U100] JS：DOM 查询
来源：http://rtw.tanke756.top

document.querySelector(".item")
来源：http://mss.redwolf501.top

[U101] JS：classList 操作
来源：http://gyk.andypj.xyz

el.classList.toggle("active")
来源：http://dcb.aizwys.cn

[U102] JS：本地存储
来源：http://vyb.316326.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://ebc.redwolf501.top

[U103] JS：定时器
来源：http://mlb.jinqigfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gba.dashuyun.cn

[U104] JS：防抖
来源：http://ctc.52xcode.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xpq.zycfv.cn

[U105] JS：节流
来源：http://ahj.zhiwuduotai.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iov.xingfuxueyuan.xyz

[U106] JS：日期格式化
来源：http://ujo.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vfk.52xcode.cn

[U107] JS：数字千分位
来源：http://tot.zdbjq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rfn.tian-w.cn

[U108] JS：随机整数
来源：http://yeg.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://heb.yfazqb.com

[U109] JS：数组分组
来源：http://ges.hysaishi.cn

Object.groupBy(arr, x => x.type)
来源：http://vup.ydjk.org.cn

[U110] JS：数组分块
来源：http://sxr.zhijiandao.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://owy.hammf.cn

[U111] JS：对象转 Map
来源：http://gxh.ybcxt.top

new Map(Object.entries(obj))
来源：http://mcn.zdqjudy.top

[U112] JS：字符串补位
来源：http://sxj.shuidangran.top

"7".padStart(3, "0")
来源：http://sst.gaohongyu789.top

[U113] JS：正则替换全部
来源：http://iuj.zhixingplan.top

s.replaceAll("a", "b")
来源：http://yvg.pengpengdd.cyou

[U114] JS：JSON 深比较
来源：http://qnk.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://thr.jianghu66.top

[U115] JS：生成 UUID
来源：http://hqr.yueranfly.top

crypto.randomUUID()
来源：http://wmz.xuetiantiany.cn

[U116] JS：类型检查（JSDoc）
来源：http://ffp.daria6918.cn

/** @param {string} name */ function f(name) {}
来源：http://qzm.sysykeji.top

[U117] JS：单元测试
来源：http://qfb.xuanzx.com

npm i -D vitest;  npx vitest
来源：http://iss.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://jqf.cashguo.top

npm i -D vite;  npx vite
来源：http://zsz.redwolf501.top

[U119] JS：生产构建
来源：http://wnh.ppjwa.cn

npx vite build
来源：http://abt.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://bhd.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://tix.shanyushiyangtech.top

================================================================================
来源：http://yab.zhijiandao.cn

统计汇总
来源：http://kov.yj20258888.top

================================================================================
来源：http://jml.fanxiaobao.xyz

按语言统计（条）：
来源：http://ytn.tianlin.xyz

Python ......... 252
来源：http://aei.yj20258888.top

PHP ............ 252
来源：http://fgw.shanyushiyangkeji.top

JavaScript ..... 252
来源：http://ika.cashguo.top

TypeScript ..... 212
来源：http://iix.daria6918.cn

Java ........... 212
来源：http://jzu.hesvh.cn

Go ............. 212
来源：http://pyt.fengsongda.top

Ruby ........... 212
来源：http://jtb.ybcxt.top

C# ............. 212
来源：http://ocm.vehdjk.com

C .............. 30
来源：http://ami.wangdashe.top

C++ ............ 30
来源：http://ocn.tian-w.cn

SQL ............ 90
来源：http://ywx.yj20258.top

Bash ........... 80
来源：http://yjr.fehbvm.com

Kotlin ......... 15
来源：http://xsr.xziqi.cn

Swift .......... 15
来源：http://izn.guowangkeji.top

Lua ............ 10
来源：http://hlv.shanyushiyangkeji.top

Perl ........... 10
来源：http://qlw.snrcjt.cn

Scala .......... 10
来源：http://avv.hysaishi.cn

------------------------------------
来源：http://fzw.zycfv.cn

合计 ........... 2106 条
来源：http://smk.daxiang520.top

按章节统计：
来源：http://xaa.hnxiangtu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://edi.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wnb.iojbl.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ktw.tarul.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dwb.zycfv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fbo.dianchejie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eqz.yongpay.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://edk.zhongyouzk.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gan.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://him.9152youxi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gis.cqqwz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qpd.zhijiandao.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oan.andypj.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tod.ivvv.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://goq.guowangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kxq.daxiang520.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://npd.zhaomingkeji.xyz

Q SQL 专题                              90
来源：http://hlo.kuanghao11.cn

R Bash 专题                             80
来源：http://scf.ppjwa.cn

S C / C++ 专题                          60
来源：http://kdg.cheryme.top

T 其他语言补充                          60
来源：http://ysz.tian-w.cn

U 高频实用片段                         120
来源：http://put.yvedp.cn

------------------------------------
来源：http://egu.bbcook.cn

合计                                  2106 条
来源：http://qat.cashguo.top

--------------------------------------------------------------------------------
来源：http://awz.zdqjudy.top

使用提醒
来源：http://crm.316326.xyz

--------------------------------------------------------------------------------
来源：http://zld.jyoumei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://urr.jinqigfzy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hfs.ybcxt.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cka.0kj1m.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ouw.xuetiantiany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hiq.ivvv.top

—— 文件结束 ——
来源：http://wnm.vqdsnc.cn

================================================================================
来源：http://mbp.aizwys.cn

程序语言常见例子速查手册（2024 版）
来源：http://ayw.xingfuxueyuan.xyz

Common Programming Examples Cheat Book
来源：http://suy.hammf.cn

================================================================================
来源：http://bmk.yfazqb.com

【收录内容】
来源：http://odz.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zyk.gogol.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vvr.guannengcc.top

SQL · Bash · C · C++
来源：http://ksj.jinqigufen.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://izv.shzxlz.cn

【使用说明】
来源：http://gni.ehwqpu.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lxi.yvedp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ung.daxiang520.top


<!-- 参考信息 -->