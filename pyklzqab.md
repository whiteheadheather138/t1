代发 wailian999

Go:   // 手写 map[int]int
来源：http://nkq.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://qnr.fanxiaobao.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://smp.nwbrower.top

[N08] 生成全排列
来源：http://dgh.ivvv.top

Py:   itertools.permutations(arr)
来源：http://eeo.yvedp.cn

PHP:  // 手写递归交换
来源：http://ojy.pengpengdd.cyou

JS:   // 手写回溯递归
来源：http://oww.chenzaomai.com

TS:   // 手写回溯递归
来源：http://adx.jlsjyb.cn

Java: // 手写回溯递归
来源：http://udb.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://vyj.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://kmz.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://ddp.hongshengwenyu.top

[N09] 栈与队列
来源：http://gkg.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dum.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jxf.pengpengdd.cyou

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zlk.iojbl.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dss.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ehn.birdmap.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wow.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hdn.xziqi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tzz.wangshuangyany.cn

[N10] 链表节点定义
来源：http://fqc.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pbf.gogol.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bhx.zhiwuduotai.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://voe.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bkk.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://zjw.xuanzx.com

Go:   type Node struct { V int; Next *Node }
来源：http://tmc.yfazqb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://awy.fktsv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://iff.cashguo.top

[N11] 二叉树中序遍历
来源：http://jfx.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://any.ivvv.top

PHP:  // 手写递归函数
来源：http://zsz.fengsongda.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wpq.kuanghao11.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tui.zhixingplan.top

Java: // 手写递归
来源：http://vuc.chenjidiqi.icu

Go:   // 手写递归
来源：http://hzs.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dri.zhoulong.xyz

C#:   // 手写递归
来源：http://sep.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zwu.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bqw.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://scl.52xcode.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zvt.nanxinkj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iyo.zhaomingkeji.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://msy.jinghuilouyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uoc.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://npx.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hxz.yuxming.cn

================================================================================
来源：http://wdh.wangdashe.top

O. 并发与异步
来源：http://ert.gzhubu.top

================================================================================
来源：http://cka.dashuyun.cn

[O01] 启动一个线程
来源：http://ccx.havefunace.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wze.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cfk.shanyushiyangtech.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cav.316326.xyz

TS:   // 同 JS
来源：http://gmp.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://oww.tanke756.top

Go:   go f()
来源：http://aed.jiagoushi.top

Ruby: Thread.new { f }
来源：http://afo.hfpthk.cn

C#:   Task.Run(() => F());
来源：http://kaz.epnwcf.com

[O02] 使用线程池
来源：http://fru.yonumen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iat.hammf.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uht.kuanghao11.cn

JS:   // worker_threads 线程池
来源：http://mbd.bbcook.cn

TS:   // worker_threads 线程池
来源：http://mgp.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://dhg.ybcxt.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zri.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jxu.sysykeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mpc.yonumen.top

[O03] 加锁保护共享数据
来源：http://mfx.svipenyu.cn

Py:   with lock: shared += 1
来源：http://rud.smart0.xyz

PHP:  // 用 flock() 做文件锁
来源：http://hsb.gotoacloud.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sbc.tarul.cn

TS:   // 同 JS
来源：http://syr.fengsongda.top

Java: synchronized (this) { shared++; }
来源：http://mmk.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vnp.ybcxt.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://app.yueranfly.top

C#:   lock (gate) { shared++; }
来源：http://wac.sufxvd.cn

[O04] 定义异步函数并等待
来源：http://czd.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://bzw.fzhhl.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fyw.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://vjq.shanyushiyangtech.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dhl.havefunace.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://upz.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://axh.zhixingplan.top

Ruby: # 用 Fiber 或 async gem
来源：http://qwd.hysaishi.cn

C#:   async Task F() { await G(); }
来源：http://bta.redwolf501.top

[O05] 并发执行并等待全部完成
来源：http://tcc.mhx1999.top

Py:   asyncio.gather(*tasks)
来源：http://xve.yueranfly.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yyh.0kj1m.cn

JS:   await Promise.all(tasks)
来源：http://nyq.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://lrs.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vhb.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oda.zhixingplan.top

Ruby: threads.map(&:join)
来源：http://xrr.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uzj.shanyushiyangkeji.top

[O06] 使用进程池
来源：http://xxs.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oeh.zhijiandao.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://upe.gogol.net.cn

JS:   // child_process / cluster 模块
来源：http://bvw.yj20258.top

TS:   // child_process / cluster 模块
来源：http://nij.fzhhl.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rop.jiagoushi.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uxp.birdmap.top

Ruby: // fork 块
来源：http://rfk.hywenlv.cn

C#:   Parallel.For
来源：http://ivw.svipenyu.cn

================================================================================
来源：http://shh.jinqigufen.top

P. 常用工具函数
来源：http://ymj.cqqwz.cn

================================================================================
来源：http://uyt.cdnleiting.top

[P01] 生成 UUID
来源：http://sel.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://uvl.havefunace.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wvc.bbcook.cn

JS:   crypto.randomUUID()
来源：http://jua.jinyuanbaomall.cn

TS:   crypto.randomUUID()
来源：http://rvi.hnqzz.top

Java: UUID.randomUUID().toString()
来源：http://bbo.zhixingplan.top

Go:   // 用 github.com/google/uuid
来源：http://pgt.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://lac.ydzc1.top

C#:   Guid.NewGuid().ToString()
来源：http://ppp.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://snx.fehbvm.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lca.xingfuxueyuan.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://dbv.yvedp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bht.shanyushiyangtech.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://atj.quarkkingdee.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jyl.nanxinkj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fta.nwbrower.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jsh.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eks.zdbjq.cn

[P03] 生成短随机字符串
来源：http://dab.hongshengwenyu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rrr.fehbvm.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iib.shzxlz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://huw.mhx1999.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lqa.fktsv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mzg.cqqwz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iab.nwbrower.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ugf.xylfe.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zqc.haohaochexian.top

[P04] 求长度
来源：http://pxe.hammf.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hlr.yj20258.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jvs.havefunace.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jzd.hywenlv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qkj.andypj.xyz

Java: list.size();  map.size();  s.length()
来源：http://zmd.gogol.net.cn

Go:   len(arr);  len(m)
来源：http://nba.shuidangran.top

Ruby: x.length;  x.size
来源：http://rdk.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fnb.yfazqb.com

[P05] 判断两个对象内容是否相等
来源：http://wtp.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://mmm.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fwj.vqdsnc.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xiw.gotoacloud.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lzv.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pio.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://psu.9152youxi.cn

Ruby: a == b
来源：http://zvp.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vsf.zhoulong.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zxd.feifeiyinyue.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xbq.316326.xyz

PHP:  if (empty($x)) {}
来源：http://fdu.fehbvm.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xzi.jianghu66.top

TS:   if (x == null) {}
来源：http://tjz.ctjpmb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ywu.zhoulong.xyz

Go:   if x == nil {}
来源：http://dzs.ydzc1.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hzz.zhiwuduotai.top

C#:   if (x is null) {}
来源：http://zac.jlsjyb.cn

[P07] 防抖与节流
来源：http://pmu.hnxiangtu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mog.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://rbm.jianghu66.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cso.sysykeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pjt.hammf.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tif.ctjpmb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rvu.yuanzhike.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zku.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://squ.daria6918.cn

[P08] 处理浮点精度问题
来源：http://xxh.aibaodan.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dyw.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blg.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cxc.birdmap.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qzs.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wis.shanyushiyangtech.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jpi.aizwys.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rwz.tanke756.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fpr.mhx1999.top

================================================================================
来源：http://mfe.gaohongyu789.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mcx.52xcode.cn

================================================================================
来源：http://mwv.sysykeji.top

[Q01] 创建表
来源：http://fjb.yuanzhike.top

CREATE TABLE users (
来源：http://lfc.fktsv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ysa.fehbvm.com

name VARCHAR(50) NOT NULL,
来源：http://ngr.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://mlb.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xaw.gaohongyu789.top

);
来源：http://jgp.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://qgx.cqqwz.cn

CREATE TABLE orders (
来源：http://ioa.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://snl.andypj.xyz

user_id INT NOT NULL,
来源：http://iqo.shangyingyoupin.top

amount DECIMAL(10, 2),
来源：http://zsh.gogol.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://opd.yvedp.cn

);
来源：http://ffv.tian-w.cn

[Q03] 增加列
来源：http://fha.hysaishi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mon.jinqigufen.top

[Q04] 修改列类型
来源：http://jnx.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://txu.yanxiufei.cn

[Q05] 重命名列
来源：http://mnt.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hnt.yuxming.cn

[Q06] 删除列
来源：http://oat.sjlbkw.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dum.xylfe.cn

[Q07] 删除表
来源：http://gqy.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://bht.chenzaomai.com

[Q08] 创建普通索引
来源：http://ygo.zhaomingkeji.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://npf.andypj.xyz

[Q09] 创建唯一索引
来源：http://qsm.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eon.sysykeji.top

[Q10] 插入单行
来源：http://crw.daxiang520.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://atv.guowangkeji.top

[Q11] 一次插入多行
来源：http://ocy.hammf.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ktu.redwolf501.top

[Q12] 插入后取自增 ID
来源：http://xhm.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://wxr.feifeiyinyue.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yhn.cashguo.top

[Q13] 忽略重复插入
来源：http://het.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jfb.gotoacloud.top

[Q14] 存在则更新（upsert）
来源：http://ppm.tanke756.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://twy.snrcjt.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://snt.jqgufenzy.top

[Q15] 查询全部
来源：http://nhx.sxryk.cn

SELECT * FROM users;
来源：http://cra.hfpthk.cn

[Q16] 查询指定列
来源：http://xnr.yvedp.cn

SELECT id, name FROM users;
来源：http://ukq.iojbl.cn

[Q17] 条件查询
来源：http://epz.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://csa.ydjk.org.cn

[Q18] 模糊匹配
来源：http://lwj.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xcw.pengpengdd.cyou

[Q19] 范围查询
来源：http://xyo.pycfn.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kaa.fanxiaobao.xyz

[Q20] IN 列表
来源：http://akj.yangfankeji.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fax.hesvh.cn

[Q21] 空值判断
来源：http://imz.xinyue.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://ffe.cashguo.top

[Q22] 排序
来源：http://pwj.yanxiufei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xng.jianghu66.top

[Q23] 分页
来源：http://exl.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vsa.ppjwa.cn

[Q24] 去重
来源：http://pfu.cdnleiting.top

SELECT DISTINCT city FROM users;
来源：http://hwq.gogol.net.cn

[Q25] 只取前 N 条
来源：http://amv.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rrb.jlsjyb.cn

[Q26] 计数
来源：http://dpn.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://kgs.aizwys.cn

[Q27] 条件计数
来源：http://eao.zycfv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://udp.hnqzz.top

[Q28] 求和与平均
来源：http://pnv.aizwys.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://okb.yonumen.top

[Q29] 最大最小值
来源：http://mad.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yuh.fzhhl.top

[Q30] 分组统计
来源：http://ucw.jinyuanbaomall.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ovy.guowangkeji.top

[Q31] 分组后过滤
来源：http://wnv.xuetiantiany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lvb.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://xqz.dashuyun.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ull.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wcn.jinyuanbaomall.cn

[Q33] 多列分组
来源：http://ffs.pycfn.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://chs.zhengqikj.top

[Q34] 每组取第一条
来源：http://vrq.xziqi.cn

SELECT * FROM (
来源：http://oub.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mtm.chenzaomai.com

) t WHERE rn = 1;
来源：http://dsn.hysaishi.cn

[Q35] 内连接
来源：http://oeo.feifeiyinyue.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ohr.ctjpmb.com

[Q36] 左连接
来源：http://dxb.hongshengwenyu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nnp.ehwqpu.com

[Q37] 右连接
来源：http://gue.zhengqikj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eev.hongshengwenyu.top

[Q38] 全外连接（PostgreSQL）
来源：http://djm.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://usa.chenzaomai.com

[Q39] 自连接（查上下级）
来源：http://ofy.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://xha.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gyt.ydzc1.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pce.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zhy.cdnleiting.top

[Q41] 多表连接
来源：http://vfy.yangfankeji.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://wgr.sweek.top

JOIN users u ON u.id = o.user_id
来源：http://vif.hongshengwenyu.top

JOIN products p ON p.id = o.product_id;
来源：http://vcr.redwolf501.top

[Q42] 连接条件附加过滤
来源：http://akt.hnqzz.top

SELECT u.name, o.amount FROM users u
来源：http://xgy.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qhh.birdmap.top

[Q43] 标量子查询
来源：http://cpu.zhiwuduotai.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kyp.yvedp.cn

[Q44] IN 子查询
来源：http://bpq.yvedp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xnu.hywenlv.cn

[Q45] EXISTS 判断存在
来源：http://tuv.fehbvm.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xnb.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tmm.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ztt.redwolf501.top

[Q47] 与平均值比较
来源：http://int.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wuv.yj20258.top

[Q48] CTE 公用表表达式
来源：http://jpe.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ctx.pycfn.com

SELECT * FROM t WHERE c > 5;
来源：http://vlj.feifeiyinyue.top

[Q49] 更新单行
来源：http://hkn.aizwys.cn


<!-- 参考信息 -->