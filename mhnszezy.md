代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zum.vehdjk.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tce.smart0.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lhw.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jkd.tarul.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bzq.fzhhl.top

[N10] 链表节点定义
来源：http://egi.ybcxt.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://owe.aibaodan.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://atu.tanke756.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vbq.fehbvm.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qqc.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://zbd.wangshuangyany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jow.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yvd.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xip.yj20258888.top

[N11] 二叉树中序遍历
来源：http://oyb.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://drd.zhixingplan.top

PHP:  // 手写递归函数
来源：http://onq.jinqigfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pvl.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mcd.hnxiangtu.top

Java: // 手写递归
来源：http://yqb.iojbl.cn

Go:   // 手写递归
来源：http://ytu.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ahu.zhaomingkeji.xyz

C#:   // 手写递归
来源：http://zko.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rhd.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rcj.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cxp.ybcxt.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vtm.dianchejie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vjj.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wpo.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ohq.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pua.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qzv.ydjk.org.cn

================================================================================
来源：http://mic.quarkkingdee.top

O. 并发与异步
来源：http://dif.xinyue.icu

================================================================================
来源：http://iey.sweek.top

[O01] 启动一个线程
来源：http://tmt.daria6918.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kjg.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hnc.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sjh.gzhubu.top

TS:   // 同 JS
来源：http://bqq.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://zkm.shzxlz.cn

Go:   go f()
来源：http://dvk.9152youxi.cn

Ruby: Thread.new { f }
来源：http://zrf.dianchejie.cn

C#:   Task.Run(() => F());
来源：http://nqq.yfazqb.com

[O02] 使用线程池
来源：http://bke.jiagoushi.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xjw.zhijiandao.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vui.daria6918.cn

JS:   // worker_threads 线程池
来源：http://bjg.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://ime.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://cym.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oxq.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ccn.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yql.jinqigfzy.top

[O03] 加锁保护共享数据
来源：http://pnn.zhijiandao.cn

Py:   with lock: shared += 1
来源：http://liq.gzhubu.top

PHP:  // 用 flock() 做文件锁
来源：http://sfx.yueranfly.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jnj.52xcode.cn

TS:   // 同 JS
来源：http://hri.ydjk.org.cn

Java: synchronized (this) { shared++; }
来源：http://wwo.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vor.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://yta.chenjidiqi.icu

C#:   lock (gate) { shared++; }
来源：http://moc.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://shd.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://mjl.svipenyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://miy.yuxming.cn

JS:   async function f() { await g(); }
来源：http://kop.zhongyouzk.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gef.bbcook.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ocj.xuanzx.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://suu.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xyj.tarul.cn

C#:   async Task F() { await G(); }
来源：http://qsp.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://ezm.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://cad.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://skx.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://nar.pycfn.com

TS:   await Promise.all(tasks)
来源：http://oek.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oor.zhoulong.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hmj.fktsv.cn

Ruby: threads.map(&:join)
来源：http://hps.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ycm.c1oappe.top

[O06] 使用进程池
来源：http://tos.gaohongyu789.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xqr.xylfe.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sdx.havefunace.top

JS:   // child_process / cluster 模块
来源：http://tmy.vqdsnc.cn

TS:   // child_process / cluster 模块
来源：http://pnd.pengpengdd.cyou

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jbh.yuanzhike.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fxp.aizwys.cn

Ruby: // fork 块
来源：http://hqh.yuxming.cn

C#:   Parallel.For
来源：http://qxi.nwbrower.top

================================================================================
来源：http://qpw.zhiwuduotai.top

P. 常用工具函数
来源：http://fdf.chenzaomai.com

================================================================================
来源：http://xmc.yj202588.top

[P01] 生成 UUID
来源：http://ucr.nwbrower.top

Py:   str(uuid.uuid4())
来源：http://eid.nwbrower.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lmi.xylfe.cn

JS:   crypto.randomUUID()
来源：http://qnp.jinghuilouyu.cn

TS:   crypto.randomUUID()
来源：http://smh.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://wuv.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://jbc.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://vnt.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://weu.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://ccl.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vew.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://fnn.tian-w.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tzp.haohaochexian.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gpp.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://geg.0kj1m.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aio.daxiang520.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://csr.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fbf.hysaishi.cn

[P03] 生成短随机字符串
来源：http://bjr.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ixo.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dzd.gaohongyu789.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cxm.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xgd.shanyushiyangkeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iok.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tue.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://vjl.zhongyouzk.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zpv.yvedp.cn

[P04] 求长度
来源：http://yjp.hysaishi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lfg.nwbrower.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jog.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rcy.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tqe.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://byk.yuxming.cn

Go:   len(arr);  len(m)
来源：http://riy.hysaishi.cn

Ruby: x.length;  x.size
来源：http://aio.birdmap.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qnk.yanxiufei.cn

[P05] 判断两个对象内容是否相等
来源：http://rcd.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yga.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ait.yvedp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hur.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uhu.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ppv.ydzc1.top

Go:   reflect.DeepEqual(a, b)
来源：http://uix.jqgfzy.top

Ruby: a == b
来源：http://uvx.xinyue.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kqa.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qhg.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://grs.c1oappe.top

PHP:  if (empty($x)) {}
来源：http://ult.hongshengwenyu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ufc.ehwqpu.com

TS:   if (x == null) {}
来源：http://ulw.shzxlz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nrs.ctjpmb.com

Go:   if x == nil {}
来源：http://npj.jqgufenzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ven.hongshengwenyu.top

C#:   if (x is null) {}
来源：http://cac.9152youxi.cn

[P07] 防抖与节流
来源：http://nfw.fengsongda.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lmn.yj202588.top

PHP:  // 手写时间戳比较
来源：http://ggo.hfpthk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vgo.guowangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hip.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yjj.sxryk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qjl.daria6918.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mhi.tianlin.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bwz.svipenyu.cn

[P08] 处理浮点精度问题
来源：http://imf.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ygx.hammf.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://spc.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dvm.vqdsnc.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sqr.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fes.guannengcc.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mzh.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ybs.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kno.jqgfzy.top

================================================================================
来源：http://ztl.quarkkingdee.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://joc.bjfxy.top

================================================================================
来源：http://yre.tarul.cn

[Q01] 创建表
来源：http://smp.uphjek.com

CREATE TABLE users (
来源：http://lsc.birdmap.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wzj.chenlongwang.top

name VARCHAR(50) NOT NULL,
来源：http://qpi.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://hcf.wangshuangyany.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tzb.aizwys.cn

);
来源：http://iln.hammf.cn

[Q02] 创建带外键的表
来源：http://nyb.ivvv.top

CREATE TABLE orders (
来源：http://waf.bbcook.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://omu.dianchejie.cn

user_id INT NOT NULL,
来源：http://wit.shanyushiyangtech.top

amount DECIMAL(10, 2),
来源：http://sti.fanxiaobao.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hav.zhijiandao.cn

);
来源：http://fsp.daria6918.cn

[Q03] 增加列
来源：http://edo.yj20258.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://knd.yj202588.top

[Q04] 修改列类型
来源：http://kge.yj20258888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ody.gotoacloud.top

[Q05] 重命名列
来源：http://xuo.tarul.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://chm.zhaomingkeji.xyz

[Q06] 删除列
来源：http://juy.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://qww.ydzc1.top

[Q07] 删除表
来源：http://aix.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://ows.tarul.cn

[Q08] 创建普通索引
来源：http://eok.ivvv.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jih.hnxiangtu.top

[Q09] 创建唯一索引
来源：http://kmn.tian-w.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jcw.aizwys.cn

[Q10] 插入单行
来源：http://suv.haohaochexian.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ikd.fengsongda.top

[Q11] 一次插入多行
来源：http://kpz.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://byb.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://jsb.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://npr.0kj1m.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fhq.smart0.xyz

[Q13] 忽略重复插入
来源：http://huc.birdmap.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sgl.xylfe.cn

[Q14] 存在则更新（upsert）
来源：http://tvs.snrcjt.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://biq.haohaochexian.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rii.52xcode.cn

[Q15] 查询全部
来源：http://nks.ctjpmb.com

SELECT * FROM users;
来源：http://tnk.zhixingplan.top

[Q16] 查询指定列
来源：http://tkg.jyoumei.cn

SELECT id, name FROM users;
来源：http://llq.sufxvd.cn

[Q17] 条件查询
来源：http://uzu.chenjidiqi.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rgb.yuxming.cn

[Q18] 模糊匹配
来源：http://eui.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oys.jinyuanbaomall.cn

[Q19] 范围查询
来源：http://pcd.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qbf.smart0.xyz

[Q20] IN 列表
来源：http://ykf.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zpd.aibaodan.cn

[Q21] 空值判断
来源：http://zia.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ayi.cheryme.top

[Q22] 排序
来源：http://wrf.316326.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://urg.yanxiufei.cn

[Q23] 分页
来源：http://fvv.jyoumei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lpc.yj20258888.top

[Q24] 去重
来源：http://kei.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://mhe.yonumen.top

[Q25] 只取前 N 条
来源：http://dyv.daria6918.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yan.uphjek.com

[Q26] 计数
来源：http://ybf.cdnleiting.top

SELECT COUNT(*) FROM users;
来源：http://qew.hammf.cn

[Q27] 条件计数
来源：http://oju.cqqwz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://llz.0kj1m.cn

[Q28] 求和与平均
来源：http://cij.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iit.0kj1m.cn

[Q29] 最大最小值
来源：http://fkm.52xcode.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lba.jqgufenzy.top

[Q30] 分组统计
来源：http://cmf.xylfe.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jxz.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://hbo.cheryme.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hig.yfazqb.com

[Q32] 分组拼接字符串
来源：http://iis.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qak.meibo888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tdk.yongpay.top

[Q33] 多列分组
来源：http://ckq.yj20258.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vch.andypj.xyz

[Q34] 每组取第一条
来源：http://xsw.hysaishi.cn

SELECT * FROM (
来源：http://aab.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pum.vehdjk.com

) t WHERE rn = 1;
来源：http://oty.yuanzhike.top

[Q35] 内连接
来源：http://xby.ctjpmb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ssj.xuetiantiany.cn

[Q36] 左连接
来源：http://izy.hfpthk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://egr.guowangkeji.top

[Q37] 右连接
来源：http://nyh.nanxuanxn.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xsy.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://iwk.wangshuangyany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lhd.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://vsb.fzhhl.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ifr.cashguo.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rsv.jianghu66.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dqk.hysaishi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yfk.xziqi.cn

[Q41] 多表连接
来源：http://qvx.svipenyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ryo.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://ogv.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://xtu.jinyuanbaomall.cn

[Q42] 连接条件附加过滤
来源：http://efj.smart0.xyz

SELECT u.name, o.amount FROM users u
来源：http://oxo.epnwcf.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eer.zdqjudy.top

[Q43] 标量子查询
来源：http://xui.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://shu.hammf.cn

[Q44] IN 子查询
来源：http://dfu.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://our.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://bza.xylfe.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rwe.feifeiyinyue.top

[Q46] NOT EXISTS 判断不存在
来源：http://wjw.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hme.hnqzz.top

[Q47] 与平均值比较
来源：http://auk.sufxvd.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rqe.uphjek.com

[Q48] CTE 公用表表达式
来源：http://trt.zhijiandao.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bpn.xuanzx.com

SELECT * FROM t WHERE c > 5;
来源：http://jfm.svipenyu.cn

[Q49] 更新单行
来源：http://jog.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wxw.guowangkeji.top

[Q50] 批量更新
来源：http://rfx.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cza.yvedp.cn

[Q51] 用子查询更新
来源：http://kal.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gev.redwolf501.top

[Q52] 删除指定行
来源：http://ltb.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://qmd.sysykeji.top

[Q53] 按条件删除
来源：http://woh.vehdjk.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://isv.cqqwz.cn

[Q54] 清空表
来源：http://jmb.bjfxy.top

TRUNCATE TABLE logs;
来源：http://ekd.mhx1999.top

[Q55] 排名（并列占位）
来源：http://lzy.jianghu66.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hfj.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://vfq.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fna.haohaochexian.top

[Q57] 行号
来源：http://jzv.xuanzx.com


<!-- 参考信息 -->