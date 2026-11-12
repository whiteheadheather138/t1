代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://mud.bjfxy.top

@contextlib.contextmanager
来源：http://vwt.yuanzhike.top

[U22] Py：矩阵转置
来源：http://dcd.shzxlz.cn

list(zip(*m))
来源：http://ryl.zhixingplan.top

[U23] Py：分块读取大文件
来源：http://sne.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jsy.fehbvm.com

[U24] Py：路径操作
来源：http://dev.mhx1999.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bgd.ppjwa.cn

[U25] Py：CSV 按字典读
来源：http://abd.tianlin.xyz

csv.DictReader(f)
来源：http://ukw.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://dkc.fktsv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hds.yfazqb.com

[U27] Py：异步 HTTP
来源：http://rfw.epnwcf.com

aiohttp.ClientSession() 配合 async with
来源：http://qsf.jianghu66.top

[U28] Py：类型别名
来源：http://bpf.shangyingyoupin.top

UserId = int
来源：http://zft.jinqigufen.top

[U29] Py：属性校验
来源：http://hru.gotoacloud.top

@property 与 @x.setter 配合
来源：http://omg.bbcook.cn

[U30] Py：数据类
来源：http://uni.aizwys.cn

@dataclass(slots=True)
来源：http://kxv.gotoacloud.top

[U31] Py：单测
来源：http://axu.gzhubu.top

python -m pytest -q
来源：http://iga.wangshuangyany.cn

[U32] Py：代码格式化
来源：http://otv.yuxming.cn

ruff format . && ruff check --fix .
来源：http://rjm.zycfv.cn

[U33] Py：打包发布
来源：http://ntc.gotoacloud.top

python -m build  （依赖 pyproject.toml）
来源：http://sxg.bjfxy.top

[U34] Py：判断编码
来源：http://yku.c1oappe.top

chardet.detect(raw)
来源：http://ysc.52xcode.cn

[U35] Py：发送邮件
来源：http://aqz.hcnkem.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mpv.daria6918.cn

[U36] Py：定时任务
来源：http://jel.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://abc.tian-w.cn

[U37] Py：读写 Excel
来源：http://uli.nwbrower.top

pandas.read_excel / DataFrame.to_excel
来源：http://crq.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://mmp.shanyushiyangkeji.top

Path(__file__).resolve().parent
来源：http://wkr.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://tqe.fehbvm.com

sys.stdout.isatty()
来源：http://cdy.hammf.cn

[U40] Py：打印到标准错误
来源：http://dgu.feifeiyinyue.top

print("err", file=sys.stderr)
来源：http://dsr.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://bzy.dianchejie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jbj.aizwys.cn

[U42] PHP：PSR-4 自动加载
来源：http://suf.ctjpmb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ryf.xylfe.cn

[U43] PHP：声明命名空间
来源：http://jwg.chenjidiqi.icu

namespace App\Http;
来源：http://dhs.ywan-chungtsiang.top

[U44] PHP：开启严格类型
来源：http://isq.shanyushiyangkeji.top

declare(strict_types=1);
来源：http://kxv.fanxiaobao.xyz

[U45] PHP：类型声明与返回类型
来源：http://igj.316326.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://khu.yj20258.top

[U46] PHP：可空类型
来源：http://ksp.jinyuanbaomall.cn

?string $name = null
来源：http://abv.hammf.cn

[U47] PHP：联合类型
来源：http://clw.ybcxt.top

int|string $id
来源：http://ebu.fktsv.cn

[U48] PHP：纯枚举
来源：http://iro.zhiwuduotai.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dlq.tarul.cn

[U49] PHP：只读属性
来源：http://nok.nanxinkj.top

public readonly string $name
来源：http://drq.yj202588.top

[U50] PHP：构造器属性提升
来源：http://poz.ywan-chungtsiang.top

public function __construct(private int $id) {}
来源：http://bqq.zhixingplan.top

[U51] PHP：数组解构
来源：http://ith.52xcode.cn

[$a, $b] = $arr;
来源：http://cuz.kuanghao11.cn

[U52] PHP：箭头函数
来源：http://uih.birdmap.top

$double = fn($x) => $x * 2;
来源：http://nao.xinyue.icu

[U53] PHP：空合并运算符
来源：http://nhq.jinqigufen.top

$v = $a ?? $b ?? "default";
来源：http://sfj.pengpengdd.cyou

[U54] PHP：空安全调用
来源：http://fip.quarkkingdee.top

$obj?->method()
来源：http://rny.tarul.cn

[U55] PHP：match 表达式
来源：http://tyg.9152youxi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ysz.jyoumei.cn

[U56] PHP：命名参数
来源：http://wjl.jiagoushi.top

f(a: 1, b: 2)
来源：http://moi.hammf.cn

[U57] PHP：字符串插值
来源：http://izx.hesvh.cn

"值: {$a}"
来源：http://vhg.jyoumei.cn

[U58] PHP：数组三件套
来源：http://lrk.yuxming.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ekf.bbcook.cn

[U59] PHP：自定义排序
来源：http://uje.yfazqb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pnn.yj202588.top

[U60] PHP：JSON 编解码
来源：http://kuw.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jhl.tarul.cn

[U61] PHP：正则
来源：http://gkb.sysykeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lai.cqqwz.cn

[U62] PHP：日期对象
来源：http://wba.smart0.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vko.feifeiyinyue.top

[U63] PHP：文件读写
来源：http://dmu.yuanzhike.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mvh.pycfn.com

[U64] PHP：目录遍历
来源：http://hpg.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://fbl.zhoulong.xyz

[U65] PHP：会话
来源：http://ocl.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://mbw.52xcode.cn

[U66] PHP：设置 Cookie
来源：http://cod.fehbvm.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tyh.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://ykp.chenzaomai.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hfr.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://huz.cucudq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gkg.xylfe.cn

[U69] PHP：PDO 预处理
来源：http://imj.wangshuangyany.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ubo.vehdjk.com

[U70] PHP：PDO 事务
来源：http://fna.bbcook.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mik.tian-w.cn

[U71] PHP：抛出异常
来源：http://ltf.wangdashe.top

throw new RuntimeException("失败", 500);
来源：http://lrp.pycfn.com

[U72] PHP：写错误日志
来源：http://quo.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://lfq.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://vvd.uphjek.com

parse_ini_file("config.ini", true)
来源：http://ouy.gaohongyu789.top

[U74] PHP：读取环境变量
来源：http://tbe.birdmap.top

getenv("APP_ENV") ?: "production"
来源：http://xso.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://qza.jianghu66.top

composer require psr/container
来源：http://rpi.smart0.xyz

[U76] PHP：简单路由
来源：http://lui.ehwqpu.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ina.aibaodan.cn

[U77] PHP：模板渲染
来源：http://chf.xziqi.cn

composer require twig/twig
来源：http://uzj.zhengqikj.top

[U78] PHP：单元测试
来源：http://chr.andypj.xyz

composer require --dev phpunit/phpunit
来源：http://aot.nanxuanxn.top

[U79] PHP：静态分析
来源：http://cwz.xuanzx.com

composer require --dev phpstan/phpstan
来源：http://oym.nanxinkj.top

[U80] PHP：代码规范修复
来源：http://uwy.nwbrower.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wnh.pycfn.com

[U81] JS：初始化项目
来源：http://zqy.wangdashe.top

npm init -y;  npm i express
来源：http://gvd.ydjk.org.cn

[U82] JS：package.json 脚本
来源：http://ffv.sweek.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jsr.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://zfp.tianlin.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://wec.52xcode.cn

[U84] JS：CommonJS 写法
来源：http://ftr.sjlbkw.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oll.52xcode.cn

[U85] JS：可选链
来源：http://ruy.yueranfly.top

a?.b?.c
来源：http://ipt.chenzaomai.com

[U86] JS：空值合并
来源：http://xog.quarkkingdee.top

a ?? b
来源：http://ijx.kuanghao11.cn

[U87] JS：解构默认值
来源：http://ydt.wangshuangyany.cn

const { a = 1, b = 2 } = obj;
来源：http://vop.bjfxy.top

[U88] JS：对象展开合并
来源：http://hdh.epnwcf.com

{ ...a, ...b }
来源：http://eyi.yuxming.cn

[U89] JS：数组去重
来源：http://mcf.yuanzhike.top

[...new Set(arr)]
来源：http://pem.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://bdx.jinqigfzy.top

[...arr].sort((a, b) => a - b)
来源：http://mqn.yonumen.top

[U91] JS：对象键值遍历
来源：http://bkr.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://erd.yongpay.top

[U92] JS：深拷贝
来源：http://xpb.yonumen.top

structuredClone(obj)
来源：http://mtg.quarkkingdee.top

[U93] JS：模板字符串
来源：http://vhd.wangdashe.top

`共 ${n} 条`
来源：http://rol.yonumen.top

[U94] JS：箭头函数
来源：http://wvf.ybcxt.top

const double = x => x * 2;
来源：http://vuf.jlsjyb.cn

[U95] JS：Promise 包装
来源：http://two.9152youxi.cn

new Promise((resolve, reject) => {})
来源：http://jky.zhaomingkeji.xyz

[U96] JS：async/await 与异常
来源：http://wmt.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kof.chenjidiqi.icu

[U97] JS：并发请求
来源：http://klt.jinyuanbaomall.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dom.shangyingyoupin.top

[U98] JS：fetch 带 JSON
来源：http://wyf.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gjn.zdbjq.cn

[U99] JS：事件监听
来源：http://xlh.daria6918.cn

el.addEventListener("click", e => {})
来源：http://gir.fktsv.cn

[U100] JS：DOM 查询
来源：http://efm.shanyushiyangkeji.top

document.querySelector(".item")
来源：http://atl.fzhhl.top

[U101] JS：classList 操作
来源：http://taf.zhiwuduotai.top

el.classList.toggle("active")
来源：http://kxq.kuanghao11.cn

[U102] JS：本地存储
来源：http://taw.yueranfly.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kak.bjfxy.top

[U103] JS：定时器
来源：http://lww.gaohongyu789.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zcf.zhengqikj.top

[U104] JS：防抖
来源：http://fjw.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ggl.gaohongyu789.top

[U105] JS：节流
来源：http://feu.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lzv.cdnleiting.top

[U106] JS：日期格式化
来源：http://urm.aizwys.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rbu.ctjpmb.com

[U107] JS：数字千分位
来源：http://ycm.fanxiaobao.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://myp.guowangkeji.top

[U108] JS：随机整数
来源：http://vwi.tanke756.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uwa.andypj.xyz

[U109] JS：数组分组
来源：http://qwi.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://ecx.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://eql.yanxiufei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ajk.cashguo.top

[U111] JS：对象转 Map
来源：http://kbx.cdnleiting.top

new Map(Object.entries(obj))
来源：http://cfu.ywan-chungtsiang.top

[U112] JS：字符串补位
来源：http://sdc.yj20258888.top

"7".padStart(3, "0")
来源：http://qxk.xylfe.cn

[U113] JS：正则替换全部
来源：http://hlk.yj20258888.top

s.replaceAll("a", "b")
来源：http://nhf.dashuyun.cn

[U114] JS：JSON 深比较
来源：http://lqj.ybcxt.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zjt.jinghuilouyu.cn

[U115] JS：生成 UUID
来源：http://ful.jinghuilouyu.cn

crypto.randomUUID()
来源：http://izw.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://dvh.hywenlv.cn

/** @param {string} name */ function f(name) {}
来源：http://efz.aizwys.cn

[U117] JS：单元测试
来源：http://tlk.jinghuilouyu.cn

npm i -D vitest;  npx vitest
来源：http://sxa.gogol.net.cn

[U118] JS：开发服务器
来源：http://rzu.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://xdu.shangyingyoupin.top

[U119] JS：生产构建
来源：http://wwz.hongshengwenyu.top

npx vite build
来源：http://quu.yueranfly.top

[U120] JS：读取环境变量（Vite）
来源：http://ruj.pycfn.com

import.meta.env.VITE_API_URL
来源：http://jtq.mhx1999.top

================================================================================
来源：http://gen.bbcook.cn

统计汇总
来源：http://tov.nwbrower.top

================================================================================
来源：http://trw.hammf.cn

按语言统计（条）：
来源：http://ryd.dashuyun.cn

Python ......... 252
来源：http://nvh.sxryk.cn

PHP ............ 252
来源：http://hnd.cashguo.top

JavaScript ..... 252
来源：http://tqn.zdqjudy.top

TypeScript ..... 212
来源：http://ppn.jqgfzy.top

Java ........... 212
来源：http://pxi.gotoacloud.top

Go ............. 212
来源：http://ssu.hnxiangtu.top

Ruby ........... 212
来源：http://mlw.hammf.cn

C# ............. 212
来源：http://cce.zhijiandao.cn

C .............. 30
来源：http://fvx.aibaodan.cn

C++ ............ 30
来源：http://azh.zhaomingkeji.xyz

SQL ............ 90
来源：http://ptj.birdmap.top

Bash ........... 80
来源：http://uaq.xinyue.icu

Kotlin ......... 15
来源：http://qrg.yj202588.top

Swift .......... 15
来源：http://qnk.haohaochexian.top

Lua ............ 10
来源：http://hgt.yj20258888.top

Perl ........... 10
来源：http://yjb.ehwqpu.com

Scala .......... 10
来源：http://akh.iojbl.cn

------------------------------------
来源：http://ngg.sweek.top

合计 ........... 2106 条
来源：http://ijd.xziqi.cn

按章节统计：
来源：http://vhk.andypj.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kls.yongpay.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xpo.hfpthk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://urw.yfazqb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vbc.yvedp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rkr.cqqwz.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kwv.ybcxt.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mjx.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ois.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nfs.tarul.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nvs.havefunace.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gji.pycfn.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://loz.smart0.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sfb.yanxiufei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ywf.hammf.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nat.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dff.yj20258.top

Q SQL 专题                              90
来源：http://raq.jinqigfzy.top

R Bash 专题                             80
来源：http://dvd.jinqigfzy.top

S C / C++ 专题                          60
来源：http://web.mhx1999.top

T 其他语言补充                          60
来源：http://gbq.fehbvm.com

U 高频实用片段                         120
来源：http://gzr.mhx1999.top

------------------------------------
来源：http://ary.nanxinkj.top

合计                                  2106 条
来源：http://mlf.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://yss.chenjidiqi.icu

使用提醒
来源：http://mlj.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://tik.hnqzz.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://clh.xziqi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://aqr.xuanzx.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rcc.zdqjudy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lwz.cucudq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cqa.nwbrower.top

—— 文件结束 ——
来源：http://yde.nanxuanxn.top

================================================================================
来源：http://ktx.wangshuangyany.cn

程序语言常见例子速查手册（2024 版）
来源：http://ski.ydjk.org.cn

Common Programming Examples Cheat Book
来源：http://kle.zhoulong.xyz

================================================================================
来源：http://ktu.daria6918.cn

【收录内容】
来源：http://gol.yueranfly.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://glw.andypj.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hqg.c1oappe.top

SQL · Bash · C · C++
来源：http://ajy.aibaodan.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://don.jqgfzy.top

【使用说明】
来源：http://wux.guannengcc.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qbe.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bju.9152youxi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xiz.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wwh.pycfn.com

Bash:  Shell         C:     C             C++:   C++
来源：http://pbh.ivvv.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ifn.redwolf501.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tyj.yfazqb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wan.xingfuxueyuan.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yfz.xziqi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://oqp.daria6918.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bck.gaohongyu789.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://udr.aibaodan.cn

【文件统计】
来源：http://fty.ybcxt.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rul.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://oxa.zhengqikj.top

目  录
来源：http://ose.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://vdw.jinqigfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mye.vqdsnc.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tkj.birdmap.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hee.tanke756.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://akw.yj202588.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lzc.zdbjq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://alx.zdqjudy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dbg.hnxiangtu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qop.jinqigfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wpt.yj20258888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tii.fktsv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uuo.xylfe.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://txl.xylfe.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cvr.hnxiangtu.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://agc.aizwys.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zdy.zdqjudy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://umo.gzhubu.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mbr.zhongyouzk.top


<!-- 参考信息 -->