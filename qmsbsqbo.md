代发 wailian999

Java: // 手写回溯递归
来源：http://gja.jiagoushi.top

Go:   // 手写回溯递归
来源：http://owv.yonumen.top

Ruby: arr.permutation.to_a
来源：http://xys.9152youxi.cn

C#:   // 手写回溯递归
来源：http://ocb.yfazqb.com

[N09] 栈与队列
来源：http://dqa.havefunace.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nlr.tanke756.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ctp.quarkkingdee.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jjr.epnwcf.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ixe.nwbrower.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rsc.cqqwz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bpb.zdbjq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lqm.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ncu.zhaomingkeji.xyz

[N10] 链表节点定义
来源：http://xbx.fktsv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yol.cqqwz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fhp.zdqjudy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mpu.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wvn.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://pzt.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://pkm.jianghu66.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hpl.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cqp.tanke756.top

[N11] 二叉树中序遍历
来源：http://ejd.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://khd.fengsongda.top

PHP:  // 手写递归函数
来源：http://nan.sweek.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jhu.yanxiufei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yry.zhiwuduotai.top

Java: // 手写递归
来源：http://vnt.jinghuilouyu.cn

Go:   // 手写递归
来源：http://tno.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vlt.jlsjyb.cn

C#:   // 手写递归
来源：http://svq.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gnm.quarkkingdee.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cbs.shuidangran.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://grg.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cnw.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ixy.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bfe.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ute.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xhj.smart0.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fdz.yvedp.cn

================================================================================
来源：http://ftq.aibaodan.cn

O. 并发与异步
来源：http://kez.aibaodan.cn

================================================================================
来源：http://sxv.xziqi.cn

[O01] 启动一个线程
来源：http://auj.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xrt.chenzaomai.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xux.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zyz.andypj.xyz

TS:   // 同 JS
来源：http://tcy.jinqigufen.top

Java: new Thread(() -> f()).start()
来源：http://aco.c1oappe.top

Go:   go f()
来源：http://zpo.cqqwz.cn

Ruby: Thread.new { f }
来源：http://fbw.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://cms.snrcjt.cn

[O02] 使用线程池
来源：http://rxp.nanxinkj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://laz.ybcxt.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uks.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://kso.hcnkem.com

TS:   // worker_threads 线程池
来源：http://cly.jyoumei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cjl.cashguo.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lgf.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dxu.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oqh.yongpay.top

[O03] 加锁保护共享数据
来源：http://qtx.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://jcm.cqqwz.cn

PHP:  // 用 flock() 做文件锁
来源：http://frg.yj20258.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qjx.bbcook.cn

TS:   // 同 JS
来源：http://avv.shanyushiyangtech.top

Java: synchronized (this) { shared++; }
来源：http://wkv.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nrt.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rpb.ctjpmb.com

C#:   lock (gate) { shared++; }
来源：http://fui.nanxuanxn.top

[O04] 定义异步函数并等待
来源：http://ury.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://gql.wangshuangyany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://edp.9152youxi.cn

JS:   async function f() { await g(); }
来源：http://tsl.yuxming.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ahe.xingfuxueyuan.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bqy.nwbrower.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aki.chenjidiqi.icu

Ruby: # 用 Fiber 或 async gem
来源：http://ncy.chenzaomai.com

C#:   async Task F() { await G(); }
来源：http://vua.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://kjw.yonumen.top

Py:   asyncio.gather(*tasks)
来源：http://yij.shuidangran.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dqk.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://rfs.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://awp.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hyq.mhx1999.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ukf.xylfe.cn

Ruby: threads.map(&:join)
来源：http://piv.gzhubu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wlh.hfpthk.cn

[O06] 使用进程池
来源：http://zbb.316326.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://acj.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pcb.ydzc1.top

JS:   // child_process / cluster 模块
来源：http://ynp.epnwcf.com

TS:   // child_process / cluster 模块
来源：http://lrw.sweek.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://asm.iojbl.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xnk.yvedp.cn

Ruby: // fork 块
来源：http://nux.cqqwz.cn

C#:   Parallel.For
来源：http://pps.redwolf501.top

================================================================================
来源：http://lok.cheryme.top

P. 常用工具函数
来源：http://lif.zdbjq.cn

================================================================================
来源：http://czc.xziqi.cn

[P01] 生成 UUID
来源：http://elx.fengsongda.top

Py:   str(uuid.uuid4())
来源：http://men.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sjo.tarul.cn

JS:   crypto.randomUUID()
来源：http://oxn.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://vus.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://evu.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://qss.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://opd.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://yqf.quarkkingdee.top

[P02] MD5 / SHA256 摘要
来源：http://oto.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qru.epnwcf.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://yev.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sem.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eai.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mot.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://igp.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ebj.sxryk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qqb.yueranfly.top

[P03] 生成短随机字符串
来源：http://ptn.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yob.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vtf.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kpq.fzhhl.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xdn.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://egf.shuidangran.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vsf.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://yiq.daxiang520.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://udj.fzhhl.top

[P04] 求长度
来源：http://dcb.ctjpmb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lwt.svipenyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aqj.9152youxi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zzy.guowangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://apc.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://pve.hongshengwenyu.top

Go:   len(arr);  len(m)
来源：http://mmt.hesvh.cn

Ruby: x.length;  x.size
来源：http://mkv.xingfuxueyuan.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://wdy.jqgufenzy.top

[P05] 判断两个对象内容是否相等
来源：http://fsn.9152youxi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ixe.zhiwuduotai.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jab.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://igs.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://adv.smart0.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ckh.uphjek.com

Go:   reflect.DeepEqual(a, b)
来源：http://qai.sxryk.cn

Ruby: a == b
来源：http://okf.gaohongyu789.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zhr.andypj.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zfb.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vbg.sufxvd.cn

PHP:  if (empty($x)) {}
来源：http://ttc.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://euf.hnxiangtu.top

TS:   if (x == null) {}
来源：http://naf.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fmp.daxiang520.top

Go:   if x == nil {}
来源：http://afy.52xcode.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qhq.zhongyouzk.top

C#:   if (x is null) {}
来源：http://jrn.cdnleiting.top

[P07] 防抖与节流
来源：http://krh.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mfq.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://vpt.smart0.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://umu.snrcjt.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://paz.shanyushiyangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dga.wangshuangyany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://aqe.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://czk.zycfv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://obs.xingfuxueyuan.xyz

[P08] 处理浮点精度问题
来源：http://ftr.bbcook.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xmw.yuxming.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vjt.tian-w.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://okk.epnwcf.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://msr.bbcook.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ysa.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bqo.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ned.hammf.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ohw.yanxiufei.cn

================================================================================
来源：http://rga.zhaomingkeji.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jms.sweek.top

================================================================================
来源：http://ebl.quarkkingdee.top

[Q01] 创建表
来源：http://yzy.uphjek.com

CREATE TABLE users (
来源：http://nab.gzhubu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pqy.ctjpmb.com

name VARCHAR(50) NOT NULL,
来源：http://aac.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://szi.birdmap.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://miv.ydjk.org.cn

);
来源：http://ojk.ivvv.top

[Q02] 创建带外键的表
来源：http://zip.smart0.xyz

CREATE TABLE orders (
来源：http://jvb.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vmz.gaohongyu789.top

user_id INT NOT NULL,
来源：http://nou.shanyushiyangkeji.top

amount DECIMAL(10, 2),
来源：http://oqq.gaohongyu789.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cjp.sufxvd.cn

);
来源：http://meb.ctjpmb.com

[Q03] 增加列
来源：http://qyv.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ujk.jinqigufen.top

[Q04] 修改列类型
来源：http://bab.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uqn.vehdjk.com

[Q05] 重命名列
来源：http://gcw.yj202588.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://krv.yfazqb.com

[Q06] 删除列
来源：http://zen.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://wcl.mhx1999.top

[Q07] 删除表
来源：http://sgp.pycfn.com

DROP TABLE IF EXISTS orders;
来源：http://sjb.iojbl.cn

[Q08] 创建普通索引
来源：http://aqr.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oly.tarul.cn

[Q09] 创建唯一索引
来源：http://rmm.hysaishi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://arz.zdqjudy.top

[Q10] 插入单行
来源：http://lvi.52xcode.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://epi.uphjek.com

[Q11] 一次插入多行
来源：http://ago.zdbjq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://icj.sxryk.cn

[Q12] 插入后取自增 ID
来源：http://zef.sweek.top

INSERT INTO users (name) VALUES ('C');
来源：http://xvt.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qpe.jiagoushi.top

[Q13] 忽略重复插入
来源：http://xyv.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gyy.xuetiantiany.cn

[Q14] 存在则更新（upsert）
来源：http://jgj.zhaomingkeji.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hmc.nwbrower.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jjh.ydzc1.top

[Q15] 查询全部
来源：http://ypb.0kj1m.cn

SELECT * FROM users;
来源：http://gru.pengpengdd.cyou

[Q16] 查询指定列
来源：http://zln.tarul.cn

SELECT id, name FROM users;
来源：http://rsl.hnqzz.top

[Q17] 条件查询
来源：http://zoi.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qqy.vehdjk.com

[Q18] 模糊匹配
来源：http://vib.jqgfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hxq.fanxiaobao.xyz

[Q19] 范围查询
来源：http://rqn.chenzaomai.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://omd.jinghuilouyu.cn

[Q20] IN 列表
来源：http://osy.havefunace.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://upp.feifeiyinyue.top

[Q21] 空值判断
来源：http://hva.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fcb.jqgfzy.top

[Q22] 排序
来源：http://hya.birdmap.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bwl.xziqi.cn

[Q23] 分页
来源：http://hfv.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://esd.bjfxy.top

[Q24] 去重
来源：http://nxj.birdmap.top

SELECT DISTINCT city FROM users;
来源：http://dhf.hammf.cn

[Q25] 只取前 N 条
来源：http://dbj.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mxa.sjlbkw.cn

[Q26] 计数
来源：http://vpd.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://toz.yuxming.cn

[Q27] 条件计数
来源：http://mqf.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://etl.gzhubu.top

[Q28] 求和与平均
来源：http://qsr.jlsjyb.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dnt.tianlin.xyz

[Q29] 最大最小值
来源：http://hom.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kti.bbcook.cn

[Q30] 分组统计
来源：http://wvb.jinqigufen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://svt.fzhhl.top

[Q31] 分组后过滤
来源：http://why.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kea.gzhubu.top

[Q32] 分组拼接字符串
来源：http://neh.zycfv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ppl.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rws.cdnleiting.top

[Q33] 多列分组
来源：http://oin.yanxiufei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jwj.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://sej.uphjek.com

SELECT * FROM (
来源：http://gpx.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ygt.zhoulong.xyz

) t WHERE rn = 1;
来源：http://nli.vehdjk.com

[Q35] 内连接
来源：http://nfx.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ofp.cdnleiting.top

[Q36] 左连接
来源：http://svs.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ugl.daria6918.cn

[Q37] 右连接
来源：http://sab.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pyo.daria6918.cn

[Q38] 全外连接（PostgreSQL）
来源：http://uzt.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ejk.zycfv.cn

[Q39] 自连接（查上下级）
来源：http://bqa.0kj1m.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ilo.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dvo.meibo888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vqz.shzxlz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nsl.daria6918.cn

[Q41] 多表连接
来源：http://jkk.aizwys.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://shc.jqgfzy.top

JOIN users u ON u.id = o.user_id
来源：http://gfh.zhixingplan.top

JOIN products p ON p.id = o.product_id;
来源：http://qcz.hywenlv.cn

[Q42] 连接条件附加过滤
来源：http://ikg.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u
来源：http://ucb.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://aqi.yongpay.top

[Q43] 标量子查询
来源：http://aqs.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sja.vqdsnc.cn

[Q44] IN 子查询
来源：http://cwf.zhijiandao.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gmx.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://yjr.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ram.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://esl.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jds.yj202588.top

[Q47] 与平均值比较
来源：http://llc.hongshengwenyu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mee.jinyuanbaomall.cn

[Q48] CTE 公用表表达式
来源：http://xui.tian-w.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jkt.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://fch.zhiwuduotai.top

[Q49] 更新单行
来源：http://exh.jqgufenzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nqq.iojbl.cn

[Q50] 批量更新
来源：http://llw.yvedp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vsx.52xcode.cn

[Q51] 用子查询更新
来源：http://art.ctjpmb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xwu.andypj.xyz

[Q52] 删除指定行
来源：http://uyz.hnxiangtu.top

DELETE FROM users WHERE id = 10;
来源：http://hzi.9152youxi.cn

[Q53] 按条件删除
来源：http://qdj.ywan-chungtsiang.top


<!-- 参考信息 -->