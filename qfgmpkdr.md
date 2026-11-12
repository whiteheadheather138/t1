代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://diw.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yzb.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://bih.zhongyouzk.top

Java: // 手写 HashMap
来源：http://ilk.aibaodan.cn

Go:   // 手写 map[int]int
来源：http://kih.ppjwa.cn

Ruby: // 手写 Hash
来源：http://iec.0kj1m.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ifi.zycfv.cn

[N08] 生成全排列
来源：http://giy.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://uvv.smart0.xyz

PHP:  // 手写递归交换
来源：http://enn.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://ovw.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://shl.chenzaomai.com

Java: // 手写回溯递归
来源：http://msb.jiagoushi.top

Go:   // 手写回溯递归
来源：http://uyj.smart0.xyz

Ruby: arr.permutation.to_a
来源：http://irp.c1oappe.top

C#:   // 手写回溯递归
来源：http://xzg.cdnleiting.top

[N09] 栈与队列
来源：http://lav.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pvy.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zve.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mzn.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nic.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://enz.zhaomingkeji.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lhd.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uou.tian-w.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xao.cqqwz.cn

[N10] 链表节点定义
来源：http://xdi.9152youxi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kiv.ybcxt.top

PHP:  class Node { public $v; public $next = null; }
来源：http://etj.pengpengdd.cyou

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rhf.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xmf.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://rnx.52xcode.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wbq.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://icc.c1oappe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nzj.gzhubu.top

[N11] 二叉树中序遍历
来源：http://esd.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rph.daria6918.cn

PHP:  // 手写递归函数
来源：http://rek.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pkv.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tmi.nwbrower.top

Java: // 手写递归
来源：http://gdf.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://rme.snrcjt.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nrk.daria6918.cn

C#:   // 手写递归
来源：http://ane.yj20258888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wea.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://isi.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aam.vehdjk.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gqf.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://voz.birdmap.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rec.jiagoushi.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yva.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zvp.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ram.jinqigfzy.top

================================================================================
来源：http://znd.yj20258888.top

O. 并发与异步
来源：http://syd.jinqigfzy.top

================================================================================
来源：http://gpa.xuetiantiany.cn

[O01] 启动一个线程
来源：http://dil.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://flw.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vbk.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iel.jiagoushi.top

TS:   // 同 JS
来源：http://wgj.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://qyc.yongpay.top

Go:   go f()
来源：http://gzb.yanxiufei.cn

Ruby: Thread.new { f }
来源：http://plv.yvedp.cn

C#:   Task.Run(() => F());
来源：http://tve.bbcook.cn

[O02] 使用线程池
来源：http://qkt.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kau.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mgd.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://usa.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://cur.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fef.aibaodan.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pdg.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tbp.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lnv.epnwcf.com

[O03] 加锁保护共享数据
来源：http://hel.gogol.net.cn

Py:   with lock: shared += 1
来源：http://pfn.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://hjj.fktsv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iyz.zdqjudy.top

TS:   // 同 JS
来源：http://keq.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://vqu.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vbi.dashuyun.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dft.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://zcj.nwbrower.top

[O04] 定义异步函数并等待
来源：http://jin.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://hrl.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rlz.feifeiyinyue.top

JS:   async function f() { await g(); }
来源：http://dso.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wjz.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qgs.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kov.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://whf.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://vva.hnxiangtu.top

[O05] 并发执行并等待全部完成
来源：http://ghw.jiagoushi.top

Py:   asyncio.gather(*tasks)
来源：http://hzr.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zie.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://ltn.xuetiantiany.cn

TS:   await Promise.all(tasks)
来源：http://tci.nanxuanxn.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cxo.yj20258.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tcw.havefunace.top

Ruby: threads.map(&:join)
来源：http://hlx.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bxp.yfazqb.com

[O06] 使用进程池
来源：http://ztw.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wtm.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://met.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://mpg.tarul.cn

TS:   // child_process / cluster 模块
来源：http://lwp.zhoulong.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://viq.fzhhl.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dfr.fehbvm.com

Ruby: // fork 块
来源：http://zpi.bjfxy.top

C#:   Parallel.For
来源：http://udj.yvedp.cn

================================================================================
来源：http://dqk.sxryk.cn

P. 常用工具函数
来源：http://uhh.shzxlz.cn

================================================================================
来源：http://cdn.zhoulong.xyz

[P01] 生成 UUID
来源：http://yyt.daxiang520.top

Py:   str(uuid.uuid4())
来源：http://jha.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wib.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://elj.yj20258888.top

TS:   crypto.randomUUID()
来源：http://mej.yuxming.cn

Java: UUID.randomUUID().toString()
来源：http://nau.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://tkh.havefunace.top

Ruby: SecureRandom.uuid
来源：http://dhd.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://xfp.chenlongwang.top

[P02] MD5 / SHA256 摘要
来源：http://ipp.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tjk.fehbvm.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://htm.shuidangran.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yve.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qgz.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bpr.9152youxi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xvw.uphjek.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cfx.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wqc.smart0.xyz

[P03] 生成短随机字符串
来源：http://jnq.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://eep.epnwcf.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xwa.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://txv.chenlongwang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://efl.yonumen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jti.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wnf.cucudq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jng.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yes.yfazqb.com

[P04] 求长度
来源：http://fjd.hesvh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bxi.yonumen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aje.jlsjyb.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qpw.fzhhl.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uau.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://zdk.fehbvm.com

Go:   len(arr);  len(m)
来源：http://lzc.feifeiyinyue.top

Ruby: x.length;  x.size
来源：http://sty.yj202588.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://adc.gzhubu.top

[P05] 判断两个对象内容是否相等
来源：http://tlh.ehwqpu.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://avm.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://stj.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mwo.nanxuanxn.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xwp.zdbjq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ymz.ehwqpu.com

Go:   reflect.DeepEqual(a, b)
来源：http://loq.gotoacloud.top

Ruby: a == b
来源：http://tor.vehdjk.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ggp.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ejy.zycfv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pym.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://kmx.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rqp.vehdjk.com

TS:   if (x == null) {}
来源：http://qnf.bbcook.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jcu.gzhubu.top

Go:   if x == nil {}
来源：http://wez.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aqy.haohaochexian.top

C#:   if (x is null) {}
来源：http://ddx.daria6918.cn

[P07] 防抖与节流
来源：http://ehy.havefunace.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lrc.ehwqpu.com

PHP:  // 手写时间戳比较
来源：http://khx.yfazqb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ztz.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lqt.ydjk.org.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nca.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pzu.fehbvm.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://uwx.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mhk.fktsv.cn

[P08] 处理浮点精度问题
来源：http://luy.hysaishi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eye.shangyingyoupin.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qos.jqgfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fga.jlsjyb.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xqj.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jfo.sweek.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kih.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ibc.chenlongwang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tlp.hnqzz.top

================================================================================
来源：http://vuj.yvedp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vle.cucudq.cn

================================================================================
来源：http://fyw.pycfn.com

[Q01] 创建表
来源：http://vtm.ydjk.org.cn

CREATE TABLE users (
来源：http://vlt.yj20258888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://obw.xinyue.icu

name VARCHAR(50) NOT NULL,
来源：http://nae.pycfn.com

email VARCHAR(100) UNIQUE,
来源：http://hzp.dianchejie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ebv.jinqigfzy.top

);
来源：http://jnl.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://fmr.yonumen.top

CREATE TABLE orders (
来源：http://tej.xingfuxueyuan.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lwx.c1oappe.top

user_id INT NOT NULL,
来源：http://gof.fanxiaobao.xyz

amount DECIMAL(10, 2),
来源：http://lrd.ybcxt.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jrr.fzhhl.top

);
来源：http://wvx.chenlongwang.top

[Q03] 增加列
来源：http://fvb.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lak.daxiang520.top

[Q04] 修改列类型
来源：http://tol.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xqt.gaohongyu789.top

[Q05] 重命名列
来源：http://eti.xuanzx.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wpm.sufxvd.cn

[Q06] 删除列
来源：http://aeh.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://lot.ybcxt.top

[Q07] 删除表
来源：http://dlj.nanxinkj.top

DROP TABLE IF EXISTS orders;
来源：http://lzh.chenlongwang.top

[Q08] 创建普通索引
来源：http://thi.jinghuilouyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kmk.shzxlz.cn

[Q09] 创建唯一索引
来源：http://ouy.shzxlz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tkg.chenjidiqi.icu

[Q10] 插入单行
来源：http://gle.dianchejie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xsr.gotoacloud.top

[Q11] 一次插入多行
来源：http://vcd.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ddr.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://kub.hesvh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qqk.yangfankeji.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nta.yj20258888.top

[Q13] 忽略重复插入
来源：http://zff.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qfa.ywan-chungtsiang.top

[Q14] 存在则更新（upsert）
来源：http://lbn.smart0.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hql.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cxe.cqqwz.cn

[Q15] 查询全部
来源：http://wvg.jiagoushi.top

SELECT * FROM users;
来源：http://mbr.snrcjt.cn

[Q16] 查询指定列
来源：http://kpm.fengsongda.top

SELECT id, name FROM users;
来源：http://oxy.yj20258888.top

[Q17] 条件查询
来源：http://dod.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://daf.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://mhp.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ylo.cdnleiting.top

[Q19] 范围查询
来源：http://gwi.yueranfly.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vuo.gzhubu.top

[Q20] IN 列表
来源：http://gno.zhixingplan.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wnl.yangfankeji.com

[Q21] 空值判断
来源：http://jbw.ywan-chungtsiang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://axy.yonumen.top

[Q22] 排序
来源：http://glk.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wdq.guowangkeji.top

[Q23] 分页
来源：http://fax.ivvv.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dqv.zdbjq.cn

[Q24] 去重
来源：http://dlj.zhongyouzk.top

SELECT DISTINCT city FROM users;
来源：http://dbf.uphjek.com

[Q25] 只取前 N 条
来源：http://wrn.hammf.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qlh.zdqjudy.top

[Q26] 计数
来源：http://muo.jyoumei.cn

SELECT COUNT(*) FROM users;
来源：http://wqn.316326.xyz

[Q27] 条件计数
来源：http://kbr.dashuyun.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ojn.sysykeji.top

[Q28] 求和与平均
来源：http://gau.chenlongwang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dsw.ybcxt.top

[Q29] 最大最小值
来源：http://edc.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://dat.feifeiyinyue.top

[Q30] 分组统计
来源：http://mjp.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lyo.fanxiaobao.xyz

[Q31] 分组后过滤
来源：http://yfn.kuanghao11.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oli.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://pyb.zdqjudy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yuc.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://drq.hfpthk.cn

[Q33] 多列分组
来源：http://ibw.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hzy.guannengcc.top

[Q34] 每组取第一条
来源：http://plr.yfazqb.com

SELECT * FROM (
来源：http://rzp.yuanzhike.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ghd.hnqzz.top

) t WHERE rn = 1;
来源：http://tys.epnwcf.com

[Q35] 内连接
来源：http://tsj.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gvd.sweek.top

[Q36] 左连接
来源：http://fzj.nwbrower.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pll.yfazqb.com

[Q37] 右连接
来源：http://lul.havefunace.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wmk.yj20258888.top

[Q38] 全外连接（PostgreSQL）
来源：http://efb.iojbl.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yzq.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://opx.dashuyun.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sir.zdbjq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://quc.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wsi.fanxiaobao.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ard.pengpengdd.cyou

[Q41] 多表连接
来源：http://vxa.jiagoushi.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sxm.jiagoushi.top

JOIN users u ON u.id = o.user_id
来源：http://txu.xinyue.icu

JOIN products p ON p.id = o.product_id;
来源：http://ufr.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://bwv.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://ypn.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://etn.feifeiyinyue.top

[Q43] 标量子查询
来源：http://frj.guowangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bke.yongpay.top

[Q44] IN 子查询
来源：http://bqe.zhijiandao.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qjs.hywenlv.cn

[Q45] EXISTS 判断存在
来源：http://qee.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mvw.yueranfly.top

[Q46] NOT EXISTS 判断不存在
来源：http://wrc.andypj.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vhx.ydjk.org.cn

[Q47] 与平均值比较
来源：http://ysx.uphjek.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ang.xziqi.cn


<!-- 参考信息 -->