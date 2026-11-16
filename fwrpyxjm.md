代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jcm.zhongyouzk.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://npc.mhx1999.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mbs.jyoumei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wsr.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://apw.smart0.xyz

[N10] 链表节点定义
来源：http://gfn.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ezk.sjlbkw.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vdp.jinqigufen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rck.snrcjt.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sis.jinqigufen.top

Java: class Node { int v; Node next; }
来源：http://hjl.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://plh.hongshengwenyu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://slx.zdqjudy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uhb.zhixingplan.top

[N11] 二叉树中序遍历
来源：http://uae.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dlf.quarkkingdee.top

PHP:  // 手写递归函数
来源：http://qta.jinghuilouyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fjt.smart0.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bpf.sweek.top

Java: // 手写递归
来源：http://kux.shanyushiyangtech.top

Go:   // 手写递归
来源：http://xls.sjlbkw.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tca.jinqigufen.top

C#:   // 手写递归
来源：http://lse.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ptk.smart0.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gvi.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gxc.hywenlv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://akl.hcnkem.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oav.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nze.bjfxy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bfa.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jna.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ddn.hnxiangtu.top

================================================================================
来源：http://wdm.fanxiaobao.xyz

O. 并发与异步
来源：http://auk.shanyushiyangkeji.top

================================================================================
来源：http://vkm.jiagoushi.top

[O01] 启动一个线程
来源：http://gbb.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ubm.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jyz.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ypu.uphjek.com

TS:   // 同 JS
来源：http://tpu.tian-w.cn

Java: new Thread(() -> f()).start()
来源：http://gow.shanyushiyangkeji.top

Go:   go f()
来源：http://zej.birdmap.top

Ruby: Thread.new { f }
来源：http://dnq.sxryk.cn

C#:   Task.Run(() => F());
来源：http://utd.ydjk.org.cn

[O02] 使用线程池
来源：http://mdt.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dhn.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sfb.yueranfly.top

JS:   // worker_threads 线程池
来源：http://kxf.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://ukn.yj20258888.top

Java: Executors.newFixedThreadPool(4)
来源：http://ovy.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kub.zdbjq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lnv.yj20258888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ene.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://pfm.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://lvi.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://jyr.uphjek.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wys.pycfn.com

TS:   // 同 JS
来源：http://zzt.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://cbg.pengpengdd.cyou

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sbb.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://sjb.aibaodan.cn

C#:   lock (gate) { shared++; }
来源：http://stu.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://ytr.ppjwa.cn

Py:   async def f():⏎    await g()
来源：http://azm.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qri.hammf.cn

JS:   async function f() { await g(); }
来源：http://lvh.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lbm.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kug.guowangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fpx.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gdb.nwbrower.top

C#:   async Task F() { await G(); }
来源：http://oun.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://ick.yanxiufei.cn

Py:   asyncio.gather(*tasks)
来源：http://hpi.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xxo.pengpengdd.cyou

JS:   await Promise.all(tasks)
来源：http://moh.yj20258.top

TS:   await Promise.all(tasks)
来源：http://ugb.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yju.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wma.ybcxt.top

Ruby: threads.map(&:join)
来源：http://irg.gzhubu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rju.c1oappe.top

[O06] 使用进程池
来源：http://bgg.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wsn.ppjwa.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://epi.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://evd.zhijiandao.cn

TS:   // child_process / cluster 模块
来源：http://bni.yanxiufei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ccf.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zkp.gaohongyu789.top

Ruby: // fork 块
来源：http://yya.gzhubu.top

C#:   Parallel.For
来源：http://ipq.tanke756.top

================================================================================
来源：http://htw.ydjk.org.cn

P. 常用工具函数
来源：http://wxo.jinqigfzy.top

================================================================================
来源：http://amw.fktsv.cn

[P01] 生成 UUID
来源：http://kxt.ydjk.org.cn

Py:   str(uuid.uuid4())
来源：http://avh.hywenlv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ogi.nanxinkj.top

JS:   crypto.randomUUID()
来源：http://ado.tarul.cn

TS:   crypto.randomUUID()
来源：http://vjs.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://gky.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://rby.mhx1999.top

Ruby: SecureRandom.uuid
来源：http://fqf.meibo888.top

C#:   Guid.NewGuid().ToString()
来源：http://tzz.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://djx.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://muc.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zra.ppjwa.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ujz.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hna.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pzz.xuetiantiany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vnk.sxryk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://icz.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bob.tianlin.xyz

[P03] 生成短随机字符串
来源：http://hum.xingfuxueyuan.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gsi.fktsv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rkc.hesvh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ctq.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hzo.yonumen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://epb.hfpthk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nir.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://avf.cdnleiting.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zgy.andypj.xyz

[P04] 求长度
来源：http://cix.pycfn.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ujy.ivvv.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fzy.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bhj.cdnleiting.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gdv.jianghu66.top

Java: list.size();  map.size();  s.length()
来源：http://vsd.wangdashe.top

Go:   len(arr);  len(m)
来源：http://xor.daxiang520.top

Ruby: x.length;  x.size
来源：http://stm.9152youxi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bxc.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://ouc.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bbg.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rnt.jinghuilouyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dow.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://shz.birdmap.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iun.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://bjp.jinqigufen.top

Ruby: a == b
来源：http://jsy.zdqjudy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aeo.ctjpmb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mfy.jinqigufen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bkj.sxryk.cn

PHP:  if (empty($x)) {}
来源：http://gnq.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gju.dashuyun.cn

TS:   if (x == null) {}
来源：http://kqx.cheryme.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pmw.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://qwq.cdnleiting.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eop.yfazqb.com

C#:   if (x is null) {}
来源：http://csw.nwbrower.top

[P07] 防抖与节流
来源：http://hvf.xuetiantiany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zel.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://agl.ydjk.org.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://swa.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jvl.cdnleiting.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mvq.jqgufenzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dvh.tian-w.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kqf.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ujt.hammf.cn

[P08] 处理浮点精度问题
来源：http://jot.zhoulong.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://atr.vehdjk.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cle.vehdjk.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pnf.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bkx.yonumen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kff.havefunace.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dlm.9152youxi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ols.hywenlv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ser.gogol.net.cn

================================================================================
来源：http://ufb.havefunace.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rot.xuetiantiany.cn

================================================================================
来源：http://keh.zdqjudy.top

[Q01] 创建表
来源：http://ucw.daxiang520.top

CREATE TABLE users (
来源：http://uat.uphjek.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://crm.sxryk.cn

name VARCHAR(50) NOT NULL,
来源：http://fae.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://rdq.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jjk.9152youxi.cn

);
来源：http://zcn.yonumen.top

[Q02] 创建带外键的表
来源：http://aok.jinqigufen.top

CREATE TABLE orders (
来源：http://zge.wangshuangyany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lsl.hfpthk.cn

user_id INT NOT NULL,
来源：http://zrr.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://tcs.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ich.vehdjk.com

);
来源：http://wgi.cqqwz.cn

[Q03] 增加列
来源：http://lxq.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kcv.0kj1m.cn

[Q04] 修改列类型
来源：http://fwo.cucudq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wlj.dashuyun.cn

[Q05] 重命名列
来源：http://qqn.yj20258.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yij.yonumen.top

[Q06] 删除列
来源：http://zxn.ctjpmb.com

ALTER TABLE users DROP COLUMN age;
来源：http://aqh.tanke756.top

[Q07] 删除表
来源：http://sxf.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://dgw.jyoumei.cn

[Q08] 创建普通索引
来源：http://xck.zhiwuduotai.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kkn.yvedp.cn

[Q09] 创建唯一索引
来源：http://vha.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sxr.gotoacloud.top

[Q10] 插入单行
来源：http://hit.chenlongwang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cye.ppjwa.cn

[Q11] 一次插入多行
来源：http://dgm.fktsv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qyr.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://coi.hesvh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hjr.gogol.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hbw.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://xsm.cdnleiting.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zke.xziqi.cn

[Q14] 存在则更新（upsert）
来源：http://qyq.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pjv.ppjwa.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://utv.xylfe.cn

[Q15] 查询全部
来源：http://mwk.hcnkem.com

SELECT * FROM users;
来源：http://rzg.quarkkingdee.top

[Q16] 查询指定列
来源：http://ntc.yfazqb.com

SELECT id, name FROM users;
来源：http://osi.yuxming.cn

[Q17] 条件查询
来源：http://olw.ybcxt.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mzm.snrcjt.cn

[Q18] 模糊匹配
来源：http://gyg.mhx1999.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kve.sjlbkw.cn

[Q19] 范围查询
来源：http://fiv.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pba.ctjpmb.com

[Q20] IN 列表
来源：http://lkt.aibaodan.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yar.hnxiangtu.top

[Q21] 空值判断
来源：http://avd.xuanzx.com

SELECT * FROM users WHERE email IS NULL;
来源：http://kkn.hnxiangtu.top

[Q22] 排序
来源：http://ipz.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pgl.dashuyun.cn

[Q23] 分页
来源：http://gmm.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ujq.jqgfzy.top

[Q24] 去重
来源：http://lno.zhoulong.xyz

SELECT DISTINCT city FROM users;
来源：http://nul.daria6918.cn

[Q25] 只取前 N 条
来源：http://cqj.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zal.gzhubu.top

[Q26] 计数
来源：http://ysi.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://pdr.jinqigfzy.top

[Q27] 条件计数
来源：http://uuu.52xcode.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eze.jqgfzy.top

[Q28] 求和与平均
来源：http://puy.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://avp.cheryme.top

[Q29] 最大最小值
来源：http://oql.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jrs.ydzc1.top

[Q30] 分组统计
来源：http://aeq.gaohongyu789.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pgs.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://cvp.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://llx.vehdjk.com

[Q32] 分组拼接字符串
来源：http://nro.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ixc.zycfv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://biz.0kj1m.cn

[Q33] 多列分组
来源：http://bqs.chenjidiqi.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yoe.cdnleiting.top

[Q34] 每组取第一条
来源：http://laa.gzhubu.top

SELECT * FROM (
来源：http://nhj.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://egd.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://dov.zycfv.cn

[Q35] 内连接
来源：http://ykj.kuanghao11.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mrl.hesvh.cn

[Q36] 左连接
来源：http://wxx.c1oappe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ken.tian-w.cn

[Q37] 右连接
来源：http://cmz.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://esm.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://krc.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xjx.cashguo.top

[Q39] 自连接（查上下级）
来源：http://ruz.yongpay.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ash.ivvv.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rrf.zhengqikj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ahs.epnwcf.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://trs.shangyingyoupin.top

[Q41] 多表连接
来源：http://oit.nanxinkj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uat.aizwys.cn

JOIN users u ON u.id = o.user_id
来源：http://hfw.yangfankeji.com

JOIN products p ON p.id = o.product_id;
来源：http://myr.zhiwuduotai.top

[Q42] 连接条件附加过滤
来源：http://nly.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://fee.tianlin.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sao.hfpthk.cn

[Q43] 标量子查询
来源：http://zni.pengpengdd.cyou

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://laf.yuxming.cn

[Q44] IN 子查询
来源：http://vlg.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hnd.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://qzl.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wzb.tarul.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bxw.smart0.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://leo.tanke756.top

[Q47] 与平均值比较
来源：http://csd.iojbl.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pxx.jqgfzy.top

[Q48] CTE 公用表表达式
来源：http://eye.zhijiandao.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zof.0kj1m.cn

SELECT * FROM t WHERE c > 5;
来源：http://rux.hnxiangtu.top

[Q49] 更新单行
来源：http://srn.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://egg.hywenlv.cn

[Q50] 批量更新
来源：http://jkd.kuanghao11.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://euw.kuanghao11.cn

[Q51] 用子查询更新
来源：http://eki.xinyue.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aqv.chenjidiqi.icu

[Q52] 删除指定行
来源：http://iun.redwolf501.top

DELETE FROM users WHERE id = 10;
来源：http://gfy.cdnleiting.top

[Q53] 按条件删除
来源：http://hlg.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baa.gzhubu.top

[Q54] 清空表
来源：http://uwd.yj20258.top

TRUNCATE TABLE logs;
来源：http://hfd.pengpengdd.cyou

[Q55] 排名（并列占位）
来源：http://snl.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qer.shangyingyoupin.top

[Q56] 密集排名（并列不占位）
来源：http://bzi.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jnk.nanxinkj.top

[Q57] 行号
来源：http://hwe.pengpengdd.cyou


<!-- 参考信息 -->