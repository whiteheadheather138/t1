代发 wailian999

[N09] 栈与队列
来源：http://lgd.nanxinkj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fcm.zhiwuduotai.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hje.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oog.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://syw.shanyushiyangtech.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://juu.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ccv.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nwa.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cwz.dashuyun.cn

[N10] 链表节点定义
来源：http://itp.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ccv.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://abx.redwolf501.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qfu.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lgh.nanxinkj.top

Java: class Node { int v; Node next; }
来源：http://yzh.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://ojz.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://qqr.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ned.316326.xyz

[N11] 二叉树中序遍历
来源：http://rfe.c1oappe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tdx.tarul.cn

PHP:  // 手写递归函数
来源：http://twx.yueranfly.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://drj.yanxiufei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cdh.smart0.xyz

Java: // 手写递归
来源：http://wct.tian-w.cn

Go:   // 手写递归
来源：http://lma.chenlongwang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jur.yonumen.top

C#:   // 手写递归
来源：http://pbz.zdqjudy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dtd.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://peb.fehbvm.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eej.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ttv.sweek.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ebe.ydzc1.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yrx.jinqigfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zyf.chenzaomai.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.guowangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qfr.yj202588.top

================================================================================
来源：http://knu.nanxinkj.top

O. 并发与异步
来源：http://kwv.cdnleiting.top

================================================================================
来源：http://pjz.nwbrower.top

[O01] 启动一个线程
来源：http://pdu.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lyd.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fkk.ywan-chungtsiang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ami.xinyue.icu

TS:   // 同 JS
来源：http://xuu.feifeiyinyue.top

Java: new Thread(() -> f()).start()
来源：http://xje.zhijiandao.cn

Go:   go f()
来源：http://laj.gotoacloud.top

Ruby: Thread.new { f }
来源：http://kto.fzhhl.top

C#:   Task.Run(() => F());
来源：http://gso.guannengcc.top

[O02] 使用线程池
来源：http://iqn.yj20258.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qih.ivvv.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hvs.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://dfv.yueranfly.top

TS:   // worker_threads 线程池
来源：http://ivp.smart0.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://vik.tianlin.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tzw.yj20258.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wzd.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gsr.zhaomingkeji.xyz

[O03] 加锁保护共享数据
来源：http://yeq.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://nim.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://uvw.ehwqpu.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ihy.svipenyu.cn

TS:   // 同 JS
来源：http://rgb.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://upe.ppjwa.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hft.pengpengdd.cyou

Ruby: mutex.synchronize { shared += 1 }
来源：http://iul.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://hnp.hongshengwenyu.top

[O04] 定义异步函数并等待
来源：http://apa.jinqigufen.top

Py:   async def f():⏎    await g()
来源：http://tet.jqgfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rqt.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://rts.xuanzx.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://hhh.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wxz.aizwys.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pru.yanxiufei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qty.guannengcc.top

C#:   async Task F() { await G(); }
来源：http://vao.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://iun.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://nhh.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nmj.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://bwh.zhaomingkeji.xyz

TS:   await Promise.all(tasks)
来源：http://hfe.zdbjq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kaj.sxryk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://axy.bjfxy.top

Ruby: threads.map(&:join)
来源：http://csk.haohaochexian.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gpj.pengpengdd.cyou

[O06] 使用进程池
来源：http://mvh.ctjpmb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://njh.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://spw.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://zyn.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://pxp.fengsongda.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jfu.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://poe.hnqzz.top

Ruby: // fork 块
来源：http://jya.xuanzx.com

C#:   Parallel.For
来源：http://sbd.epnwcf.com

================================================================================
来源：http://dif.snrcjt.cn

P. 常用工具函数
来源：http://fux.hnqzz.top

================================================================================
来源：http://ixc.bjfxy.top

[P01] 生成 UUID
来源：http://ucj.redwolf501.top

Py:   str(uuid.uuid4())
来源：http://yxb.mhx1999.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://toj.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://odw.yj20258.top

TS:   crypto.randomUUID()
来源：http://uzt.pengpengdd.cyou

Java: UUID.randomUUID().toString()
来源：http://gie.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://fqr.zhijiandao.cn

Ruby: SecureRandom.uuid
来源：http://zhp.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://ays.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://jjk.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ttb.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://zdj.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jfe.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eaq.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fdl.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tfe.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cgv.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hww.zdqjudy.top

[P03] 生成短随机字符串
来源：http://ruo.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kkz.aibaodan.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ydh.hywenlv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://odk.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cft.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bhs.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://opl.xuanzx.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://xkn.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jzk.sjlbkw.cn

[P04] 求长度
来源：http://fau.ctjpmb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aml.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kdp.hysaishi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jfw.316326.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cot.iojbl.cn

Java: list.size();  map.size();  s.length()
来源：http://eix.bbcook.cn

Go:   len(arr);  len(m)
来源：http://mgh.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://iwu.ydjk.org.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://irc.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://fcv.yongpay.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dvj.yvedp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vix.andypj.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://krx.sxryk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ikj.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uqb.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://vxm.redwolf501.top

Ruby: a == b
来源：http://ehw.jqgfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bdm.fanxiaobao.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zsn.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yla.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://kqs.jinqigufen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bno.cdnleiting.top

TS:   if (x == null) {}
来源：http://sdp.jiagoushi.top

Java: if (x == null || x.isEmpty()) {}
来源：http://grf.tarul.cn

Go:   if x == nil {}
来源：http://zyc.chenlongwang.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ykm.xylfe.cn

C#:   if (x is null) {}
来源：http://avu.hfpthk.cn

[P07] 防抖与节流
来源：http://vkb.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://izq.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://vdd.fanxiaobao.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://flo.cqqwz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jgn.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bsx.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jto.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fij.fengsongda.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://raa.vqdsnc.cn

[P08] 处理浮点精度问题
来源：http://huq.cashguo.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gcs.jqgufenzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dvq.cucudq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vgt.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wlg.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nwn.yanxiufei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hyu.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vcb.yongpay.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qvo.52xcode.cn

================================================================================
来源：http://zsc.gogol.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zez.havefunace.top

================================================================================
来源：http://ftr.sweek.top

[Q01] 创建表
来源：http://orx.svipenyu.cn

CREATE TABLE users (
来源：http://vdo.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://faw.daria6918.cn

name VARCHAR(50) NOT NULL,
来源：http://jig.bbcook.cn

email VARCHAR(100) UNIQUE,
来源：http://sho.zhoulong.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://urq.pycfn.com

);
来源：http://qvy.ehwqpu.com

[Q02] 创建带外键的表
来源：http://jia.yonumen.top

CREATE TABLE orders (
来源：http://jjg.cheryme.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dja.pengpengdd.cyou

user_id INT NOT NULL,
来源：http://afi.dianchejie.cn

amount DECIMAL(10, 2),
来源：http://goo.wangdashe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://isj.fehbvm.com

);
来源：http://ftz.cqqwz.cn

[Q03] 增加列
来源：http://alz.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hro.wangshuangyany.cn

[Q04] 修改列类型
来源：http://rlc.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sss.wangdashe.top

[Q05] 重命名列
来源：http://pmn.snrcjt.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sgt.pycfn.com

[Q06] 删除列
来源：http://unu.yvedp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gbs.nwbrower.top

[Q07] 删除表
来源：http://vbu.yanxiufei.cn

DROP TABLE IF EXISTS orders;
来源：http://kfp.havefunace.top

[Q08] 创建普通索引
来源：http://kau.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://est.epnwcf.com

[Q09] 创建唯一索引
来源：http://hdo.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zea.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://lpx.xylfe.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eub.yongpay.top

[Q11] 一次插入多行
来源：http://jkw.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rxo.jyoumei.cn

[Q12] 插入后取自增 ID
来源：http://gwe.fzhhl.top

INSERT INTO users (name) VALUES ('C');
来源：http://zrr.nwbrower.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oal.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://grf.tarul.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wdp.mhx1999.top

[Q14] 存在则更新（upsert）
来源：http://pkb.dianchejie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tvx.quarkkingdee.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hce.hesvh.cn

[Q15] 查询全部
来源：http://knt.sysykeji.top

SELECT * FROM users;
来源：http://hhm.vqdsnc.cn

[Q16] 查询指定列
来源：http://bjc.ydzc1.top

SELECT id, name FROM users;
来源：http://iox.bjfxy.top

[Q17] 条件查询
来源：http://gqi.smart0.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yij.xuanzx.com

[Q18] 模糊匹配
来源：http://tlf.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sre.tanke756.top

[Q19] 范围查询
来源：http://lwk.zhiwuduotai.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rnf.zdqjudy.top

[Q20] IN 列表
来源：http://hyf.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yto.zdbjq.cn

[Q21] 空值判断
来源：http://syf.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aam.ydjk.org.cn

[Q22] 排序
来源：http://cse.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hww.svipenyu.cn

[Q23] 分页
来源：http://wyb.sysykeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://duv.bbcook.cn

[Q24] 去重
来源：http://ufd.zhengqikj.top

SELECT DISTINCT city FROM users;
来源：http://shz.nanxinkj.top

[Q25] 只取前 N 条
来源：http://moh.c1oappe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gkc.nanxinkj.top

[Q26] 计数
来源：http://nie.iojbl.cn

SELECT COUNT(*) FROM users;
来源：http://oqw.xziqi.cn

[Q27] 条件计数
来源：http://jgx.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://smn.vehdjk.com

[Q28] 求和与平均
来源：http://obr.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jih.jianghu66.top

[Q29] 最大最小值
来源：http://jhw.hnxiangtu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ein.tian-w.cn

[Q30] 分组统计
来源：http://pzi.ywan-chungtsiang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lbi.cheryme.top

[Q31] 分组后过滤
来源：http://yas.yangfankeji.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ydx.bbcook.cn

[Q32] 分组拼接字符串
来源：http://riy.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pag.zdqjudy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gbv.gzhubu.top

[Q33] 多列分组
来源：http://enn.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qgb.xinyue.icu

[Q34] 每组取第一条
来源：http://hqs.jinyuanbaomall.cn

SELECT * FROM (
来源：http://omx.52xcode.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zmn.dianchejie.cn

) t WHERE rn = 1;
来源：http://aww.yueranfly.top

[Q35] 内连接
来源：http://zio.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ykm.wangdashe.top

[Q36] 左连接
来源：http://hdy.dashuyun.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ymr.ctjpmb.com

[Q37] 右连接
来源：http://cno.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fxl.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vzz.aibaodan.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xsa.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://gfp.ydjk.org.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ciz.bbcook.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://auz.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pdf.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nfa.cheryme.top

[Q41] 多表连接
来源：http://afo.pycfn.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://nzg.jinyuanbaomall.cn

JOIN users u ON u.id = o.user_id
来源：http://lpi.shanyushiyangtech.top

JOIN products p ON p.id = o.product_id;
来源：http://zqt.hcnkem.com

[Q42] 连接条件附加过滤
来源：http://jlc.chenjidiqi.icu

SELECT u.name, o.amount FROM users u
来源：http://krm.smart0.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gks.ydzc1.top

[Q43] 标量子查询
来源：http://jjg.hfpthk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eur.sweek.top

[Q44] IN 子查询
来源：http://yrd.yueranfly.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://thq.zhijiandao.cn

[Q45] EXISTS 判断存在
来源：http://lbh.jinghuilouyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hsd.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kym.tanke756.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://opw.316326.xyz

[Q47] 与平均值比较
来源：http://tcd.hongshengwenyu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://udx.hnqzz.top

[Q48] CTE 公用表表达式
来源：http://kup.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nbz.ybcxt.top

SELECT * FROM t WHERE c > 5;
来源：http://vih.meibo888.top

[Q49] 更新单行
来源：http://dbz.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fqk.nwbrower.top

[Q50] 批量更新
来源：http://qle.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ftf.bjfxy.top

[Q51] 用子查询更新
来源：http://gff.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wgi.yj20258.top

[Q52] 删除指定行
来源：http://dpf.nwbrower.top

DELETE FROM users WHERE id = 10;
来源：http://qwc.wangdashe.top

[Q53] 按条件删除
来源：http://rbz.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ijg.daria6918.cn

[Q54] 清空表
来源：http://qaz.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://bhz.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://jbk.dashuyun.cn


<!-- 参考信息 -->