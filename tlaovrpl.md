代发 wailian999

[N09] 栈与队列
来源：http://irg.dianchejie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hxs.xziqi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vkr.gotoacloud.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cye.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aio.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vxp.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dwo.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zja.jyoumei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fyl.yueranfly.top

[N10] 链表节点定义
来源：http://gtm.ppjwa.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://epk.hcnkem.com

PHP:  class Node { public $v; public $next = null; }
来源：http://zdh.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pwb.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ohx.jinqigufen.top

Java: class Node { int v; Node next; }
来源：http://pwf.yuxming.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vnf.pengpengdd.cyou

Ruby: Node = Struct.new(:v, :next)
来源：http://iux.birdmap.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xvl.daria6918.cn

[N11] 二叉树中序遍历
来源：http://oos.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lkh.xylfe.cn

PHP:  // 手写递归函数
来源：http://pkt.nanxinkj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sge.jlsjyb.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aoz.shanyushiyangtech.top

Java: // 手写递归
来源：http://rwx.shzxlz.cn

Go:   // 手写递归
来源：http://vcs.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aod.yj202588.top

C#:   // 手写递归
来源：http://lia.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bye.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://byw.tian-w.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hit.jyoumei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pti.bbcook.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gwx.cheryme.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://des.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uhv.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fqw.andypj.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vyt.guowangkeji.top

================================================================================
来源：http://khl.zhongyouzk.top

O. 并发与异步
来源：http://zfi.sjlbkw.cn

================================================================================
来源：http://nrf.jlsjyb.cn

[O01] 启动一个线程
来源：http://zqr.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qdc.havefunace.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gax.c1oappe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kfd.nanxinkj.top

TS:   // 同 JS
来源：http://xbr.c1oappe.top

Java: new Thread(() -> f()).start()
来源：http://cci.xuetiantiany.cn

Go:   go f()
来源：http://fdx.shzxlz.cn

Ruby: Thread.new { f }
来源：http://hry.mhx1999.top

C#:   Task.Run(() => F());
来源：http://mjx.yfazqb.com

[O02] 使用线程池
来源：http://pdr.sweek.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eoa.hfpthk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yvu.fengsongda.top

JS:   // worker_threads 线程池
来源：http://ied.yuanzhike.top

TS:   // worker_threads 线程池
来源：http://owd.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://rzc.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qhv.birdmap.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://auh.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mvo.jyoumei.cn

[O03] 加锁保护共享数据
来源：http://vpr.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://acl.jianghu66.top

PHP:  // 用 flock() 做文件锁
来源：http://aof.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ffd.pycfn.com

TS:   // 同 JS
来源：http://hjz.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://hoc.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ekg.sysykeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ecu.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://ksg.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://aph.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://tnv.fanxiaobao.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://knn.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://bbx.zhiwuduotai.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jge.zdqjudy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://spj.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dwx.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://eyb.yfazqb.com

C#:   async Task F() { await G(); }
来源：http://gqj.shanyushiyangkeji.top

[O05] 并发执行并等待全部完成
来源：http://eng.gaohongyu789.top

Py:   asyncio.gather(*tasks)
来源：http://gfd.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gew.nanxinkj.top

JS:   await Promise.all(tasks)
来源：http://vve.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://wfv.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fta.hnqzz.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://awx.9152youxi.cn

Ruby: threads.map(&:join)
来源：http://wfu.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zdp.shzxlz.cn

[O06] 使用进程池
来源：http://wtg.xinyue.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sgd.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://vdt.vehdjk.com

JS:   // child_process / cluster 模块
来源：http://ggj.yanxiufei.cn

TS:   // child_process / cluster 模块
来源：http://cxu.yanxiufei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rpr.yangfankeji.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rgt.zdqjudy.top

Ruby: // fork 块
来源：http://gtb.c1oappe.top

C#:   Parallel.For
来源：http://pto.ctjpmb.com

================================================================================
来源：http://gpb.zhijiandao.cn

P. 常用工具函数
来源：http://qxj.hywenlv.cn

================================================================================
来源：http://wln.fzhhl.top

[P01] 生成 UUID
来源：http://umf.nanxinkj.top

Py:   str(uuid.uuid4())
来源：http://ahi.daria6918.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nst.yj202588.top

JS:   crypto.randomUUID()
来源：http://dan.hnxiangtu.top

TS:   crypto.randomUUID()
来源：http://zlo.epnwcf.com

Java: UUID.randomUUID().toString()
来源：http://hge.kuanghao11.cn

Go:   // 用 github.com/google/uuid
来源：http://lub.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://qkc.yongpay.top

C#:   Guid.NewGuid().ToString()
来源：http://kzd.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://mil.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://awm.epnwcf.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://yij.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xsq.0kj1m.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ttm.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jvv.ctjpmb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mmu.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zwm.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lgo.pycfn.com

[P03] 生成短随机字符串
来源：http://jmh.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ugi.nanxuanxn.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gaa.vehdjk.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nhj.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jfh.jiagoushi.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mib.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vkt.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mwh.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ayq.birdmap.top

[P04] 求长度
来源：http://pwk.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wmn.jqgfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hdt.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eyw.yonumen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tkv.meibo888.top

Java: list.size();  map.size();  s.length()
来源：http://wer.pycfn.com

Go:   len(arr);  len(m)
来源：http://rxk.jiagoushi.top

Ruby: x.length;  x.size
来源：http://qwn.ivvv.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://eww.wangdashe.top

[P05] 判断两个对象内容是否相等
来源：http://xgf.gotoacloud.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uck.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qma.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cat.bbcook.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gzf.c1oappe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://efq.yuanzhike.top

Go:   reflect.DeepEqual(a, b)
来源：http://wbo.xziqi.cn

Ruby: a == b
来源：http://blj.xziqi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://arn.zhixingplan.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tzq.vehdjk.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zbg.yfazqb.com

PHP:  if (empty($x)) {}
来源：http://cva.shanyushiyangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://svy.hesvh.cn

TS:   if (x == null) {}
来源：http://kmd.jinqigufen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://awx.sweek.top

Go:   if x == nil {}
来源：http://ald.cheryme.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xca.tianlin.xyz

C#:   if (x is null) {}
来源：http://okd.yuxming.cn

[P07] 防抖与节流
来源：http://rtp.havefunace.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://maf.wangdashe.top

PHP:  // 手写时间戳比较
来源：http://oiw.gaohongyu789.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mxv.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wrz.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hqr.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eos.hesvh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oxm.zhongyouzk.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ort.gaohongyu789.top

[P08] 处理浮点精度问题
来源：http://uio.cashguo.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jbs.xuanzx.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tpz.jianghu66.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://coj.jinghuilouyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hgg.gogol.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kje.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hfo.mhx1999.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rhz.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dsd.quarkkingdee.top

================================================================================
来源：http://qsk.birdmap.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hqs.316326.xyz

================================================================================
来源：http://ywj.chenlongwang.top

[Q01] 创建表
来源：http://icb.chenlongwang.top

CREATE TABLE users (
来源：http://ndf.xuanzx.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cnv.shuidangran.top

name VARCHAR(50) NOT NULL,
来源：http://tbk.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://htp.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xbr.yj20258.top

);
来源：http://wdh.nwbrower.top

[Q02] 创建带外键的表
来源：http://hyk.wangshuangyany.cn

CREATE TABLE orders (
来源：http://znt.haohaochexian.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zxl.shuidangran.top

user_id INT NOT NULL,
来源：http://gct.nanxuanxn.top

amount DECIMAL(10, 2),
来源：http://rpk.tian-w.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jir.wangdashe.top

);
来源：http://ekr.yueranfly.top

[Q03] 增加列
来源：http://wgx.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fyf.yangfankeji.com

[Q04] 修改列类型
来源：http://eqo.yonumen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aak.tarul.cn

[Q05] 重命名列
来源：http://euo.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://enp.meibo888.top

[Q06] 删除列
来源：http://uhr.pengpengdd.cyou

ALTER TABLE users DROP COLUMN age;
来源：http://hnn.pengpengdd.cyou

[Q07] 删除表
来源：http://eys.dianchejie.cn

DROP TABLE IF EXISTS orders;
来源：http://nxh.yangfankeji.com

[Q08] 创建普通索引
来源：http://fsr.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xzr.hongshengwenyu.top

[Q09] 创建唯一索引
来源：http://xxb.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mzl.zhengqikj.top

[Q10] 插入单行
来源：http://tdj.fzhhl.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zfd.tianlin.xyz

[Q11] 一次插入多行
来源：http://fgy.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nxf.tarul.cn

[Q12] 插入后取自增 ID
来源：http://kii.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bko.mhx1999.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lkx.zdqjudy.top

[Q13] 忽略重复插入
来源：http://too.hnxiangtu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://miw.jlsjyb.cn

[Q14] 存在则更新（upsert）
来源：http://sbb.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wss.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://too.0kj1m.cn

[Q15] 查询全部
来源：http://bpm.shangyingyoupin.top

SELECT * FROM users;
来源：http://imm.xingfuxueyuan.xyz

[Q16] 查询指定列
来源：http://rtg.sufxvd.cn

SELECT id, name FROM users;
来源：http://fkc.nanxinkj.top

[Q17] 条件查询
来源：http://oeg.cdnleiting.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fsh.snrcjt.cn

[Q18] 模糊匹配
来源：http://pkf.zhixingplan.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pos.gzhubu.top

[Q19] 范围查询
来源：http://agf.haohaochexian.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kle.xylfe.cn

[Q20] IN 列表
来源：http://zws.yueranfly.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tpd.shangyingyoupin.top

[Q21] 空值判断
来源：http://gfg.nanxuanxn.top

SELECT * FROM users WHERE email IS NULL;
来源：http://sif.hnqzz.top

[Q22] 排序
来源：http://lwo.zhongyouzk.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hzy.jinqigfzy.top

[Q23] 分页
来源：http://zcv.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jtg.hysaishi.cn

[Q24] 去重
来源：http://agz.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://czs.hfpthk.cn

[Q25] 只取前 N 条
来源：http://vzn.jyoumei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nis.tianlin.xyz

[Q26] 计数
来源：http://lef.cashguo.top

SELECT COUNT(*) FROM users;
来源：http://sjt.yangfankeji.com

[Q27] 条件计数
来源：http://fir.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://unt.aizwys.cn

[Q28] 求和与平均
来源：http://qip.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xcg.feifeiyinyue.top

[Q29] 最大最小值
来源：http://epm.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xdf.mhx1999.top

[Q30] 分组统计
来源：http://kkh.yueranfly.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://shh.0kj1m.cn

[Q31] 分组后过滤
来源：http://lzv.hesvh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hsk.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://lus.bbcook.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://twh.chenzaomai.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ase.hfpthk.cn

[Q33] 多列分组
来源：http://jzi.feifeiyinyue.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://plr.c1oappe.top

[Q34] 每组取第一条
来源：http://lbe.zhaomingkeji.xyz

SELECT * FROM (
来源：http://pyq.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zsr.zdqjudy.top

) t WHERE rn = 1;
来源：http://und.jinqigufen.top

[Q35] 内连接
来源：http://dsg.aibaodan.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://alp.sjlbkw.cn

[Q36] 左连接
来源：http://exn.cdnleiting.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uyt.hammf.cn

[Q37] 右连接
来源：http://caa.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fan.xuetiantiany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dfx.c1oappe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qnr.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://dhs.ydjk.org.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rjr.wangshuangyany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mhd.yfazqb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://uyt.52xcode.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dap.hcnkem.com

[Q41] 多表连接
来源：http://vnx.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ywn.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://rym.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://jmh.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://dmo.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://qqa.tianlin.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ivm.shanyushiyangtech.top

[Q43] 标量子查询
来源：http://dqo.yangfankeji.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://egk.svipenyu.cn

[Q44] IN 子查询
来源：http://xsn.xziqi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vsa.hesvh.cn

[Q45] EXISTS 判断存在
来源：http://aro.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rqx.yuxming.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oev.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nge.aizwys.cn

[Q47] 与平均值比较
来源：http://oco.tian-w.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qfr.jinqigufen.top

[Q48] CTE 公用表表达式
来源：http://whq.yfazqb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oig.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://qek.zhengqikj.top

[Q49] 更新单行
来源：http://hil.316326.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mlp.wangdashe.top

[Q50] 批量更新
来源：http://wfh.hywenlv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bea.fehbvm.com

[Q51] 用子查询更新
来源：http://rzv.snrcjt.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rec.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://jmw.jinqigfzy.top

DELETE FROM users WHERE id = 10;
来源：http://kmk.fktsv.cn

[Q53] 按条件删除
来源：http://dlj.yangfankeji.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://enu.haohaochexian.top

[Q54] 清空表
来源：http://edw.yanxiufei.cn

TRUNCATE TABLE logs;
来源：http://gyk.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://gjf.shanyushiyangkeji.top


<!-- 参考信息 -->