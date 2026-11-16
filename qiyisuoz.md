代发 wailian999

Py:   itertools.permutations(arr)
来源：http://mpw.c1oappe.top

PHP:  // 手写递归交换
来源：http://fgb.zhongyouzk.top

JS:   // 手写回溯递归
来源：http://nqo.guowangkeji.top

TS:   // 手写回溯递归
来源：http://mxy.xziqi.cn

Java: // 手写回溯递归
来源：http://dqr.bbcook.cn

Go:   // 手写回溯递归
来源：http://hed.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://ljr.c1oappe.top

C#:   // 手写回溯递归
来源：http://oue.zhiwuduotai.top

[N09] 栈与队列
来源：http://ueh.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://owe.9152youxi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ghx.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fsz.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zid.fengsongda.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hka.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yxa.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://awd.redwolf501.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://odq.chenzaomai.com

[N10] 链表节点定义
来源：http://hiy.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hwn.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hap.hnxiangtu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cju.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zly.yonumen.top

Java: class Node { int v; Node next; }
来源：http://ytw.feifeiyinyue.top

Go:   type Node struct { V int; Next *Node }
来源：http://bkb.nwbrower.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rak.xuetiantiany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dls.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://czn.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://szk.meibo888.top

PHP:  // 手写递归函数
来源：http://ujd.yuanzhike.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xwg.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ufn.nanxinkj.top

Java: // 手写递归
来源：http://fpp.ydzc1.top

Go:   // 手写递归
来源：http://bpm.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vmo.xuanzx.com

C#:   // 手写递归
来源：http://xcd.fktsv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ngq.yvedp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lrr.cdnleiting.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sjy.jyoumei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ciu.vqdsnc.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ygq.mhx1999.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kja.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vkb.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ldu.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nwz.shzxlz.cn

================================================================================
来源：http://lxa.ywan-chungtsiang.top

O. 并发与异步
来源：http://lgd.uphjek.com

================================================================================
来源：http://igf.mhx1999.top

[O01] 启动一个线程
来源：http://ilp.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sjh.feifeiyinyue.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vrh.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ahw.birdmap.top

TS:   // 同 JS
来源：http://mag.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://qgs.ybcxt.top

Go:   go f()
来源：http://rfn.cucudq.cn

Ruby: Thread.new { f }
来源：http://nts.xuetiantiany.cn

C#:   Task.Run(() => F());
来源：http://dbv.xinyue.icu

[O02] 使用线程池
来源：http://eki.bjfxy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://krl.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yxf.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://jun.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://fji.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://ghk.jinyuanbaomall.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vop.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://suw.zhaomingkeji.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vpx.pengpengdd.cyou

[O03] 加锁保护共享数据
来源：http://oqb.tanke756.top

Py:   with lock: shared += 1
来源：http://ygs.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://ltr.jianghu66.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lao.ybcxt.top

TS:   // 同 JS
来源：http://gwf.xylfe.cn

Java: synchronized (this) { shared++; }
来源：http://fdw.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pph.shangyingyoupin.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://daz.xingfuxueyuan.xyz

C#:   lock (gate) { shared++; }
来源：http://pth.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://stj.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://sod.svipenyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xek.wangdashe.top

JS:   async function f() { await g(); }
来源：http://ige.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://utj.xingfuxueyuan.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://byw.shuidangran.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kdz.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hif.kuanghao11.cn

C#:   async Task F() { await G(); }
来源：http://ygt.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://edk.tarul.cn

Py:   asyncio.gather(*tasks)
来源：http://pdv.shanyushiyangtech.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eox.sxryk.cn

JS:   await Promise.all(tasks)
来源：http://igr.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://zky.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gmi.snrcjt.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bzb.xuetiantiany.cn

Ruby: threads.map(&:join)
来源：http://ndl.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vge.guowangkeji.top

[O06] 使用进程池
来源：http://ict.shanyushiyangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fxe.jinghuilouyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://age.yonumen.top

JS:   // child_process / cluster 模块
来源：http://kos.wangdashe.top

TS:   // child_process / cluster 模块
来源：http://vtp.meibo888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ils.guannengcc.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xoo.sxryk.cn

Ruby: // fork 块
来源：http://wzi.yuxming.cn

C#:   Parallel.For
来源：http://czs.guannengcc.top

================================================================================
来源：http://yhs.jinyuanbaomall.cn

P. 常用工具函数
来源：http://vlh.xuanzx.com

================================================================================
来源：http://ojt.gotoacloud.top

[P01] 生成 UUID
来源：http://ler.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://ajf.feifeiyinyue.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://auj.hnxiangtu.top

JS:   crypto.randomUUID()
来源：http://axe.fktsv.cn

TS:   crypto.randomUUID()
来源：http://ppp.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://uzw.ybcxt.top

Go:   // 用 github.com/google/uuid
来源：http://xsc.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://gke.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://yxy.xuanzx.com

[P02] MD5 / SHA256 摘要
来源：http://ywo.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://stb.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fkm.shuidangran.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fvx.guannengcc.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vsn.wangdashe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bxj.jinghuilouyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mxx.hysaishi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mly.fzhhl.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gzs.zhiwuduotai.top

[P03] 生成短随机字符串
来源：http://hfs.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://obf.yj20258.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ibd.9152youxi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://omq.zycfv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cws.fktsv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ile.shuidangran.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lxq.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qtq.havefunace.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qbd.xylfe.cn

[P04] 求长度
来源：http://mdl.tianlin.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://azm.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uqr.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://thd.yuanzhike.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fxs.snrcjt.cn

Java: list.size();  map.size();  s.length()
来源：http://bxy.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://lna.gotoacloud.top

Ruby: x.length;  x.size
来源：http://kuz.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lwc.ppjwa.cn

[P05] 判断两个对象内容是否相等
来源：http://pdp.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://eay.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://knf.zhoulong.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rbc.jqgufenzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qcs.xinyue.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eov.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://ueg.xingfuxueyuan.xyz

Ruby: a == b
来源：http://cfi.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jmg.shangyingyoupin.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xiw.tanke756.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bvh.kuanghao11.cn

PHP:  if (empty($x)) {}
来源：http://nbr.fktsv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wdf.kuanghao11.cn

TS:   if (x == null) {}
来源：http://yrt.gogol.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lnn.vehdjk.com

Go:   if x == nil {}
来源：http://okf.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eef.xinyue.icu

C#:   if (x is null) {}
来源：http://ktg.zdqjudy.top

[P07] 防抖与节流
来源：http://pjs.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://icl.aizwys.cn

PHP:  // 手写时间戳比较
来源：http://iaf.hnqzz.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wcj.guowangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://awk.nwbrower.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ang.yanxiufei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ckx.nanxuanxn.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hfa.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ffr.xingfuxueyuan.xyz

[P08] 处理浮点精度问题
来源：http://qae.epnwcf.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://skl.smart0.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iqe.feifeiyinyue.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sjd.hongshengwenyu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jbj.zhaomingkeji.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tcp.yvedp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vai.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ncs.cucudq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://czo.fengsongda.top

================================================================================
来源：http://jaa.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fln.hywenlv.cn

================================================================================
来源：http://mwx.xziqi.cn

[Q01] 创建表
来源：http://ytb.zhijiandao.cn

CREATE TABLE users (
来源：http://lrk.quarkkingdee.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qgd.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://wnb.ehwqpu.com

email VARCHAR(100) UNIQUE,
来源：http://hkc.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yie.jinqigufen.top

);
来源：http://pod.tarul.cn

[Q02] 创建带外键的表
来源：http://zqk.gotoacloud.top

CREATE TABLE orders (
来源：http://vym.ywan-chungtsiang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ciw.haohaochexian.top

user_id INT NOT NULL,
来源：http://bji.yangfankeji.com

amount DECIMAL(10, 2),
来源：http://odt.cheryme.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dqx.fktsv.cn

);
来源：http://cqx.vehdjk.com

[Q03] 增加列
来源：http://xgu.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sug.hfpthk.cn

[Q04] 修改列类型
来源：http://rwv.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dpy.wangdashe.top

[Q05] 重命名列
来源：http://okp.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cpf.xylfe.cn

[Q06] 删除列
来源：http://rxw.aizwys.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kpc.ctjpmb.com

[Q07] 删除表
来源：http://mgx.zhixingplan.top

DROP TABLE IF EXISTS orders;
来源：http://cuv.c1oappe.top

[Q08] 创建普通索引
来源：http://elm.cucudq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ots.zdqjudy.top

[Q09] 创建唯一索引
来源：http://zpn.xingfuxueyuan.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://igt.zhiwuduotai.top

[Q10] 插入单行
来源：http://oxr.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yks.shzxlz.cn

[Q11] 一次插入多行
来源：http://aka.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bgd.shzxlz.cn

[Q12] 插入后取自增 ID
来源：http://zfw.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://acm.jqgfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ljt.chenzaomai.com

[Q13] 忽略重复插入
来源：http://jhk.tianlin.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://com.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://lgr.wangdashe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ycx.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ljf.yvedp.cn

[Q15] 查询全部
来源：http://cdm.hnqzz.top

SELECT * FROM users;
来源：http://uxl.ybcxt.top

[Q16] 查询指定列
来源：http://ulz.52xcode.cn

SELECT id, name FROM users;
来源：http://kyw.yfazqb.com

[Q17] 条件查询
来源：http://kdw.chenlongwang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://klz.jlsjyb.cn

[Q18] 模糊匹配
来源：http://bew.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://llw.gotoacloud.top

[Q19] 范围查询
来源：http://vpe.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wsn.cashguo.top

[Q20] IN 列表
来源：http://wrm.shzxlz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tvp.jqgufenzy.top

[Q21] 空值判断
来源：http://cbn.cucudq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kme.fehbvm.com

[Q22] 排序
来源：http://wbt.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dlk.gzhubu.top

[Q23] 分页
来源：http://nqn.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rln.shanyushiyangkeji.top

[Q24] 去重
来源：http://ydq.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://rua.yj202588.top

[Q25] 只取前 N 条
来源：http://cbd.jlsjyb.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://igc.aizwys.cn

[Q26] 计数
来源：http://vev.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://tlj.316326.xyz

[Q27] 条件计数
来源：http://ukz.tarul.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mvv.0kj1m.cn

[Q28] 求和与平均
来源：http://pqq.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lvt.birdmap.top

[Q29] 最大最小值
来源：http://hdv.zhiwuduotai.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fna.daxiang520.top

[Q30] 分组统计
来源：http://smf.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gxa.epnwcf.com

[Q31] 分组后过滤
来源：http://uye.zhijiandao.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bey.fehbvm.com

[Q32] 分组拼接字符串
来源：http://sni.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://weq.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gwt.tanke756.top

[Q33] 多列分组
来源：http://xsf.quarkkingdee.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zcz.hnxiangtu.top

[Q34] 每组取第一条
来源：http://etu.svipenyu.cn

SELECT * FROM (
来源：http://cde.jinqigfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uhh.fktsv.cn

) t WHERE rn = 1;
来源：http://wvl.gogol.net.cn

[Q35] 内连接
来源：http://xoj.wangshuangyany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zws.pengpengdd.cyou

[Q36] 左连接
来源：http://uxn.gotoacloud.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ajz.birdmap.top

[Q37] 右连接
来源：http://cno.hesvh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://val.fengsongda.top

[Q38] 全外连接（PostgreSQL）
来源：http://zyr.gotoacloud.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://net.ydjk.org.cn

[Q39] 自连接（查上下级）
来源：http://gbk.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://hdi.ydjk.org.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bvu.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rum.ehwqpu.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fwn.zdbjq.cn

[Q41] 多表连接
来源：http://klk.guannengcc.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pom.chenzaomai.com

JOIN users u ON u.id = o.user_id
来源：http://pcp.pycfn.com

JOIN products p ON p.id = o.product_id;
来源：http://ymq.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://mmu.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://dns.redwolf501.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yge.nanxinkj.top

[Q43] 标量子查询
来源：http://toh.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pgi.aibaodan.cn

[Q44] IN 子查询
来源：http://vqt.daxiang520.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bvy.hywenlv.cn

[Q45] EXISTS 判断存在
来源：http://sru.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eqj.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://esp.zhiwuduotai.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bug.guowangkeji.top

[Q47] 与平均值比较
来源：http://bzq.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jsy.gzhubu.top

[Q48] CTE 公用表表达式
来源：http://csn.zhixingplan.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uby.xylfe.cn

SELECT * FROM t WHERE c > 5;
来源：http://khd.tianlin.xyz

[Q49] 更新单行
来源：http://xvz.fanxiaobao.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ykf.sysykeji.top

[Q50] 批量更新
来源：http://bzz.wangshuangyany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ncs.zhixingplan.top

[Q51] 用子查询更新
来源：http://uuo.bbcook.cn


<!-- 参考信息 -->