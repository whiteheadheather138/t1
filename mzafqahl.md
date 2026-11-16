代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ymb.zhaomingkeji.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eei.cheryme.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lqs.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gcv.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yqd.daxiang520.top

[N10] 链表节点定义
来源：http://wrk.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pyv.tanke756.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ipi.cashguo.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mjd.havefunace.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jup.haohaochexian.top

Java: class Node { int v; Node next; }
来源：http://ozm.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zqt.epnwcf.com

Ruby: Node = Struct.new(:v, :next)
来源：http://dkb.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qsw.aibaodan.cn

[N11] 二叉树中序遍历
来源：http://xnx.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://puu.sxryk.cn

PHP:  // 手写递归函数
来源：http://bjm.hesvh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kvm.wangdashe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ybg.xziqi.cn

Java: // 手写递归
来源：http://fyy.vqdsnc.cn

Go:   // 手写递归
来源：http://bgb.316326.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zsd.cheryme.top

C#:   // 手写递归
来源：http://mgx.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ggg.xylfe.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bhw.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gyg.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pmy.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wad.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aca.andypj.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wcm.sufxvd.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bjm.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wrf.aizwys.cn

================================================================================
来源：http://ubm.jinyuanbaomall.cn

O. 并发与异步
来源：http://pgu.redwolf501.top

================================================================================
来源：http://jrb.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://dvp.nwbrower.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sgb.hysaishi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vyu.yuanzhike.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dib.vehdjk.com

TS:   // 同 JS
来源：http://lap.zdbjq.cn

Java: new Thread(() -> f()).start()
来源：http://vyh.shzxlz.cn

Go:   go f()
来源：http://dqy.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://tlw.smart0.xyz

C#:   Task.Run(() => F());
来源：http://lbu.uphjek.com

[O02] 使用线程池
来源：http://kjm.bbcook.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://whg.pengpengdd.cyou

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://joj.nwbrower.top

JS:   // worker_threads 线程池
来源：http://hdv.xuanzx.com

TS:   // worker_threads 线程池
来源：http://dqy.cdnleiting.top

Java: Executors.newFixedThreadPool(4)
来源：http://oyz.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ful.vehdjk.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gvl.yvedp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://igx.yfazqb.com

[O03] 加锁保护共享数据
来源：http://wwk.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://pln.ydjk.org.cn

PHP:  // 用 flock() 做文件锁
来源：http://qof.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eye.chenlongwang.top

TS:   // 同 JS
来源：http://kxf.fzhhl.top

Java: synchronized (this) { shared++; }
来源：http://bbx.mhx1999.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qyi.feifeiyinyue.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qpx.ivvv.top

C#:   lock (gate) { shared++; }
来源：http://vlv.zhijiandao.cn

[O04] 定义异步函数并等待
来源：http://pct.iojbl.cn

Py:   async def f():⏎    await g()
来源：http://ajs.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kbe.vehdjk.com

JS:   async function f() { await g(); }
来源：http://rdh.yueranfly.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hwi.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zos.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jrp.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://djk.yj202588.top

C#:   async Task F() { await G(); }
来源：http://zjc.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://yek.hnqzz.top

Py:   asyncio.gather(*tasks)
来源：http://kdy.jiagoushi.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xgf.nanxinkj.top

JS:   await Promise.all(tasks)
来源：http://nna.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://blt.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vvs.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rjy.fanxiaobao.xyz

Ruby: threads.map(&:join)
来源：http://qja.shzxlz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://emt.cucudq.cn

[O06] 使用进程池
来源：http://uyx.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://idt.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://hsd.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://fgw.jlsjyb.cn

TS:   // child_process / cluster 模块
来源：http://nbl.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bnl.hammf.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://krw.sjlbkw.cn

Ruby: // fork 块
来源：http://lgq.feifeiyinyue.top

C#:   Parallel.For
来源：http://zlr.shanyushiyangkeji.top

================================================================================
来源：http://lld.xylfe.cn

P. 常用工具函数
来源：http://eok.jinyuanbaomall.cn

================================================================================
来源：http://zvk.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://mqg.smart0.xyz

Py:   str(uuid.uuid4())
来源：http://utk.fanxiaobao.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ain.hysaishi.cn

JS:   crypto.randomUUID()
来源：http://brp.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://ase.shanyushiyangtech.top

Java: UUID.randomUUID().toString()
来源：http://qvw.sufxvd.cn

Go:   // 用 github.com/google/uuid
来源：http://uja.uphjek.com

Ruby: SecureRandom.uuid
来源：http://psz.ppjwa.cn

C#:   Guid.NewGuid().ToString()
来源：http://wqh.shanyushiyangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://xks.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pfe.redwolf501.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lyr.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hwp.zhoulong.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nxm.iojbl.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://afi.sweek.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pkz.sxryk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nqb.fktsv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ylo.guannengcc.top

[P03] 生成短随机字符串
来源：http://kbf.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://teu.zhengqikj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jgn.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ens.jyoumei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xfb.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mnv.kuanghao11.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fka.hammf.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sia.zycfv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yop.gotoacloud.top

[P04] 求长度
来源：http://sxg.hongshengwenyu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fcj.nanxuanxn.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://guv.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://paj.hywenlv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://arp.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://fyg.gogol.net.cn

Go:   len(arr);  len(m)
来源：http://tnb.fanxiaobao.xyz

Ruby: x.length;  x.size
来源：http://kit.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://pux.zhiwuduotai.top

[P05] 判断两个对象内容是否相等
来源：http://fdg.gogol.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gsa.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jph.cashguo.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vkd.cashguo.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kix.jiagoushi.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pso.zhoulong.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://nkz.xuanzx.com

Ruby: a == b
来源：http://dyu.dashuyun.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zcv.yvedp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://atl.ivvv.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vmb.kuanghao11.cn

PHP:  if (empty($x)) {}
来源：http://vpb.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dko.chenjidiqi.icu

TS:   if (x == null) {}
来源：http://wph.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lay.xylfe.cn

Go:   if x == nil {}
来源：http://wxc.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://smp.gzhubu.top

C#:   if (x is null) {}
来源：http://kis.tanke756.top

[P07] 防抖与节流
来源：http://naq.tianlin.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pig.ehwqpu.com

PHP:  // 手写时间戳比较
来源：http://slc.shanyushiyangtech.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lvv.iojbl.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lae.yj20258888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qki.fktsv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://luz.fanxiaobao.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://kuw.aizwys.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mak.daxiang520.top

[P08] 处理浮点精度问题
来源：http://rus.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://izt.gotoacloud.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vht.hammf.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qgd.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wnn.cashguo.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pau.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vsq.jyoumei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zyt.52xcode.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://miy.fengsongda.top

================================================================================
来源：http://ynr.svipenyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sbe.hnqzz.top

================================================================================
来源：http://piy.shanyushiyangkeji.top

[Q01] 创建表
来源：http://mjh.chenlongwang.top

CREATE TABLE users (
来源：http://zah.ivvv.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bcy.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://yyu.ydzc1.top

email VARCHAR(100) UNIQUE,
来源：http://pxe.jlsjyb.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://poc.xylfe.cn

);
来源：http://frr.bjfxy.top

[Q02] 创建带外键的表
来源：http://cpt.meibo888.top

CREATE TABLE orders (
来源：http://fsp.hongshengwenyu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://glj.shanyushiyangkeji.top

user_id INT NOT NULL,
来源：http://caf.gaohongyu789.top

amount DECIMAL(10, 2),
来源：http://alr.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jjq.yj202588.top

);
来源：http://rza.shzxlz.cn

[Q03] 增加列
来源：http://zhm.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://war.wangdashe.top

[Q04] 修改列类型
来源：http://dqr.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fkp.sysykeji.top

[Q05] 重命名列
来源：http://tqz.yj202588.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hxr.epnwcf.com

[Q06] 删除列
来源：http://suz.hnxiangtu.top

ALTER TABLE users DROP COLUMN age;
来源：http://iaz.bjfxy.top

[Q07] 删除表
来源：http://jmm.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://qxv.hongshengwenyu.top

[Q08] 创建普通索引
来源：http://jvq.hcnkem.com

CREATE INDEX idx_users_email ON users(email);
来源：http://ays.shanyushiyangkeji.top

[Q09] 创建唯一索引
来源：http://dch.cqqwz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dqr.shuidangran.top

[Q10] 插入单行
来源：http://mhd.cheryme.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ytp.redwolf501.top

[Q11] 一次插入多行
来源：http://hfy.gotoacloud.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yba.xylfe.cn

[Q12] 插入后取自增 ID
来源：http://znq.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://oom.shangyingyoupin.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ovy.zycfv.cn

[Q13] 忽略重复插入
来源：http://pqe.fehbvm.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rtd.yj20258.top

[Q14] 存在则更新（upsert）
来源：http://zxu.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qky.zhaomingkeji.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://agz.xylfe.cn

[Q15] 查询全部
来源：http://jej.0kj1m.cn

SELECT * FROM users;
来源：http://ecp.jqgfzy.top

[Q16] 查询指定列
来源：http://qdq.fktsv.cn

SELECT id, name FROM users;
来源：http://epj.mhx1999.top

[Q17] 条件查询
来源：http://jfl.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lsk.jlsjyb.cn

[Q18] 模糊匹配
来源：http://wmx.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rbd.zhoulong.xyz

[Q19] 范围查询
来源：http://vry.sxryk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jif.yuxming.cn

[Q20] IN 列表
来源：http://jnf.mhx1999.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ofa.zhengqikj.top

[Q21] 空值判断
来源：http://pef.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://btr.bjfxy.top

[Q22] 排序
来源：http://oiw.zhiwuduotai.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rsd.hysaishi.cn

[Q23] 分页
来源：http://zwj.yonumen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bzi.ywan-chungtsiang.top

[Q24] 去重
来源：http://cvq.jinyuanbaomall.cn

SELECT DISTINCT city FROM users;
来源：http://qnk.zycfv.cn

[Q25] 只取前 N 条
来源：http://akj.yvedp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://acz.shuidangran.top

[Q26] 计数
来源：http://rxr.zdqjudy.top

SELECT COUNT(*) FROM users;
来源：http://hwf.zhoulong.xyz

[Q27] 条件计数
来源：http://ysa.tarul.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ppg.sjlbkw.cn

[Q28] 求和与平均
来源：http://mfu.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zcq.hysaishi.cn

[Q29] 最大最小值
来源：http://xxb.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lnf.yfazqb.com

[Q30] 分组统计
来源：http://nxn.bjfxy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xev.sweek.top

[Q31] 分组后过滤
来源：http://ozk.chenlongwang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hza.sjlbkw.cn

[Q32] 分组拼接字符串
来源：http://ixf.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vhb.yj20258888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qix.fktsv.cn

[Q33] 多列分组
来源：http://sfb.smart0.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yei.meibo888.top

[Q34] 每组取第一条
来源：http://drt.tanke756.top

SELECT * FROM (
来源：http://xam.yuanzhike.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yfv.xuanzx.com

) t WHERE rn = 1;
来源：http://mun.xuetiantiany.cn

[Q35] 内连接
来源：http://qob.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://etq.uphjek.com

[Q36] 左连接
来源：http://ilm.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://azr.zhaomingkeji.xyz

[Q37] 右连接
来源：http://lym.sufxvd.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zln.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://adj.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xcq.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://nma.shanyushiyangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rwq.sweek.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qqd.yangfankeji.com

[Q40] 交叉连接（笛卡尔积）
来源：http://qlm.yonumen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qxm.cheryme.top

[Q41] 多表连接
来源：http://xbo.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jar.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://hji.zhongyouzk.top

JOIN products p ON p.id = o.product_id;
来源：http://pht.yj20258.top

[Q42] 连接条件附加过滤
来源：http://cub.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u
来源：http://lvi.bjfxy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://enc.zhiwuduotai.top

[Q43] 标量子查询
来源：http://dsa.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mis.snrcjt.cn

[Q44] IN 子查询
来源：http://hxl.jianghu66.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bgo.yonumen.top

[Q45] EXISTS 判断存在
来源：http://wjj.jinqigufen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bnq.xinyue.icu

[Q46] NOT EXISTS 判断不存在
来源：http://ufc.fanxiaobao.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nki.cheryme.top

[Q47] 与平均值比较
来源：http://izi.jianghu66.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jfc.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://iey.hywenlv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sov.vqdsnc.cn

SELECT * FROM t WHERE c > 5;
来源：http://xag.sweek.top

[Q49] 更新单行
来源：http://okl.jinyuanbaomall.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wsm.zhongyouzk.top

[Q50] 批量更新
来源：http://dbc.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://saa.chenlongwang.top

[Q51] 用子查询更新
来源：http://iji.sxryk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sbn.ctjpmb.com

[Q52] 删除指定行
来源：http://nad.pengpengdd.cyou

DELETE FROM users WHERE id = 10;
来源：http://nth.hongshengwenyu.top

[Q53] 按条件删除
来源：http://vdr.zhoulong.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://neh.tianlin.xyz

[Q54] 清空表
来源：http://abw.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://nkl.snrcjt.cn

[Q55] 排名（并列占位）
来源：http://sbb.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lsp.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://tow.tanke756.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://soz.hywenlv.cn

[Q57] 行号
来源：http://hdb.hongshengwenyu.top


<!-- 参考信息 -->