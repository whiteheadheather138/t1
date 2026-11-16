代发 wailian999

Py:   itertools.permutations(arr)
来源：http://bqf.nwbrower.top

PHP:  // 手写递归交换
来源：http://tgq.birdmap.top

JS:   // 手写回溯递归
来源：http://epx.yfazqb.com

TS:   // 手写回溯递归
来源：http://ycf.c1oappe.top

Java: // 手写回溯递归
来源：http://qqj.jianghu66.top

Go:   // 手写回溯递归
来源：http://wlk.sxryk.cn

Ruby: arr.permutation.to_a
来源：http://mqk.shuidangran.top

C#:   // 手写回溯递归
来源：http://lda.zdqjudy.top

[N09] 栈与队列
来源：http://dlt.quarkkingdee.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kis.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://byw.hywenlv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gkv.quarkkingdee.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://exg.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nny.iojbl.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jop.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jtv.hnxiangtu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fqr.vehdjk.com

[N10] 链表节点定义
来源：http://dzo.fehbvm.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fyh.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gjl.hongshengwenyu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ccc.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gmc.kuanghao11.cn

Java: class Node { int v; Node next; }
来源：http://xfz.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://dlr.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://stp.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jsl.yj20258.top

[N11] 二叉树中序遍历
来源：http://nxp.cucudq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vyo.sxryk.cn

PHP:  // 手写递归函数
来源：http://rcw.jianghu66.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dxt.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gdt.9152youxi.cn

Java: // 手写递归
来源：http://hbq.gogol.net.cn

Go:   // 手写递归
来源：http://sjm.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wld.guowangkeji.top

C#:   // 手写递归
来源：http://nwg.xylfe.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hjn.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eul.yongpay.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cxt.aibaodan.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xsl.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xza.birdmap.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pmf.nwbrower.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wrs.316326.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://izz.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tai.hfpthk.cn

================================================================================
来源：http://evv.cheryme.top

O. 并发与异步
来源：http://goz.andypj.xyz

================================================================================
来源：http://lgl.yj20258888.top

[O01] 启动一个线程
来源：http://qwe.dashuyun.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zai.ydzc1.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sbd.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dne.yuanzhike.top

TS:   // 同 JS
来源：http://kpl.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://akm.epnwcf.com

Go:   go f()
来源：http://bue.fktsv.cn

Ruby: Thread.new { f }
来源：http://kff.jiagoushi.top

C#:   Task.Run(() => F());
来源：http://laj.xuanzx.com

[O02] 使用线程池
来源：http://akm.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bck.dashuyun.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kec.xuanzx.com

JS:   // worker_threads 线程池
来源：http://twt.quarkkingdee.top

TS:   // worker_threads 线程池
来源：http://ndj.gzhubu.top

Java: Executors.newFixedThreadPool(4)
来源：http://nvd.kuanghao11.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sch.ppjwa.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pjm.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ftp.redwolf501.top

[O03] 加锁保护共享数据
来源：http://puh.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://sxd.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://vts.zhongyouzk.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vak.cdnleiting.top

TS:   // 同 JS
来源：http://nca.quarkkingdee.top

Java: synchronized (this) { shared++; }
来源：http://xqx.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hfo.sjlbkw.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://drn.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://wxi.snrcjt.cn

[O04] 定义异步函数并等待
来源：http://cuv.nanxuanxn.top

Py:   async def f():⏎    await g()
来源：http://jib.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qyx.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://hvb.sufxvd.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jii.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qrd.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ita.hnqzz.top

Ruby: # 用 Fiber 或 async gem
来源：http://ywu.fanxiaobao.xyz

C#:   async Task F() { await G(); }
来源：http://svq.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://ssc.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://hcy.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xis.sweek.top

JS:   await Promise.all(tasks)
来源：http://tkb.cashguo.top

TS:   await Promise.all(tasks)
来源：http://ois.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fvd.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kkq.gotoacloud.top

Ruby: threads.map(&:join)
来源：http://ftr.fanxiaobao.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://wih.jiagoushi.top

[O06] 使用进程池
来源：http://wzh.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://skj.xuetiantiany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ral.ivvv.top

JS:   // child_process / cluster 模块
来源：http://zaq.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://zvi.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nra.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://slo.yangfankeji.com

Ruby: // fork 块
来源：http://ujn.quarkkingdee.top

C#:   Parallel.For
来源：http://azj.ehwqpu.com

================================================================================
来源：http://scb.jinghuilouyu.cn

P. 常用工具函数
来源：http://nkq.jinqigufen.top

================================================================================
来源：http://thh.tarul.cn

[P01] 生成 UUID
来源：http://jei.wangshuangyany.cn

Py:   str(uuid.uuid4())
来源：http://vcn.epnwcf.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wwc.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://wnh.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://knd.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://jpd.jyoumei.cn

Go:   // 用 github.com/google/uuid
来源：http://tng.meibo888.top

Ruby: SecureRandom.uuid
来源：http://ndg.hammf.cn

C#:   Guid.NewGuid().ToString()
来源：http://gqh.tarul.cn

[P02] MD5 / SHA256 摘要
来源：http://lzr.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://loc.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://udc.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vqs.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cpy.gzhubu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wiw.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fhf.hcnkem.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://akv.hfpthk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wkx.zhixingplan.top

[P03] 生成短随机字符串
来源：http://ecq.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xlq.jinghuilouyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://snd.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xmy.nanxuanxn.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://upg.bjfxy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ltt.aibaodan.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dos.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://afm.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mqo.quarkkingdee.top

[P04] 求长度
来源：http://lie.daria6918.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pme.snrcjt.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://obw.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hni.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mgp.sweek.top

Java: list.size();  map.size();  s.length()
来源：http://bst.cucudq.cn

Go:   len(arr);  len(m)
来源：http://lan.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://pkn.gzhubu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tow.aibaodan.cn

[P05] 判断两个对象内容是否相等
来源：http://uxt.chenjidiqi.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://yfm.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hef.shangyingyoupin.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tlm.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jgp.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iqt.ivvv.top

Go:   reflect.DeepEqual(a, b)
来源：http://vhy.vqdsnc.cn

Ruby: a == b
来源：http://pkk.hfpthk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cqm.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dwj.shzxlz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rcn.shangyingyoupin.top

PHP:  if (empty($x)) {}
来源：http://xua.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hnb.hesvh.cn

TS:   if (x == null) {}
来源：http://nxu.zhaomingkeji.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://mpk.vqdsnc.cn

Go:   if x == nil {}
来源：http://zpm.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hgh.daxiang520.top

C#:   if (x is null) {}
来源：http://csm.mhx1999.top

[P07] 防抖与节流
来源：http://nsv.chenjidiqi.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sfi.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://nkg.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hsh.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tov.xingfuxueyuan.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://thz.haohaochexian.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nwf.chenlongwang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://iky.chenlongwang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xim.jianghu66.top

[P08] 处理浮点精度问题
来源：http://ujh.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://slu.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uld.hnqzz.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nqe.xingfuxueyuan.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zey.zhixingplan.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://puk.hfpthk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qbe.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rdb.nwbrower.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cds.yongpay.top

================================================================================
来源：http://gut.pengpengdd.cyou

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ieo.jqgufenzy.top

================================================================================
来源：http://ovc.zycfv.cn

[Q01] 创建表
来源：http://nbt.wangshuangyany.cn

CREATE TABLE users (
来源：http://xzr.316326.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tmu.tarul.cn

name VARCHAR(50) NOT NULL,
来源：http://jct.jqgfzy.top

email VARCHAR(100) UNIQUE,
来源：http://ddc.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jpb.jiagoushi.top

);
来源：http://fcq.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://qbd.c1oappe.top

CREATE TABLE orders (
来源：http://ivh.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rke.zhaomingkeji.xyz

user_id INT NOT NULL,
来源：http://oye.shangyingyoupin.top

amount DECIMAL(10, 2),
来源：http://oax.316326.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hzc.svipenyu.cn

);
来源：http://fsy.yj20258888.top

[Q03] 增加列
来源：http://vci.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nex.ctjpmb.com

[Q04] 修改列类型
来源：http://lgz.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xcj.iojbl.cn

[Q05] 重命名列
来源：http://rnb.pengpengdd.cyou

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://chx.zdbjq.cn

[Q06] 删除列
来源：http://afi.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://cpu.snrcjt.cn

[Q07] 删除表
来源：http://xol.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://lia.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://jhu.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hhy.hesvh.cn

[Q09] 创建唯一索引
来源：http://bbs.chenzaomai.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cjs.jqgufenzy.top

[Q10] 插入单行
来源：http://mwz.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xjc.gaohongyu789.top

[Q11] 一次插入多行
来源：http://zfs.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://neu.zhixingplan.top

[Q12] 插入后取自增 ID
来源：http://rpw.nanxinkj.top

INSERT INTO users (name) VALUES ('C');
来源：http://wkf.sufxvd.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uvc.yj20258888.top

[Q13] 忽略重复插入
来源：http://wmt.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uez.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://nuy.daxiang520.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mdq.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jko.yongpay.top

[Q15] 查询全部
来源：http://oko.jiagoushi.top

SELECT * FROM users;
来源：http://dwt.shangyingyoupin.top

[Q16] 查询指定列
来源：http://met.sysykeji.top

SELECT id, name FROM users;
来源：http://vyo.ppjwa.cn

[Q17] 条件查询
来源：http://vaa.yuxming.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bwq.nwbrower.top

[Q18] 模糊匹配
来源：http://din.jianghu66.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tzj.xziqi.cn

[Q19] 范围查询
来源：http://acc.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ejt.gaohongyu789.top

[Q20] IN 列表
来源：http://squ.aibaodan.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ols.guannengcc.top

[Q21] 空值判断
来源：http://lcl.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bnd.316326.xyz

[Q22] 排序
来源：http://sxr.hesvh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jcc.xziqi.cn

[Q23] 分页
来源：http://lmt.sxryk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iiq.shuidangran.top

[Q24] 去重
来源：http://fjs.xziqi.cn

SELECT DISTINCT city FROM users;
来源：http://vkv.zycfv.cn

[Q25] 只取前 N 条
来源：http://igv.xingfuxueyuan.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zuf.cheryme.top

[Q26] 计数
来源：http://vpt.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://ixp.gzhubu.top

[Q27] 条件计数
来源：http://fhf.tanke756.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rya.guannengcc.top

[Q28] 求和与平均
来源：http://hzl.hysaishi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aqe.316326.xyz

[Q29] 最大最小值
来源：http://bkm.ywan-chungtsiang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mmy.wangdashe.top

[Q30] 分组统计
来源：http://the.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uky.tian-w.cn

[Q31] 分组后过滤
来源：http://pqv.hnxiangtu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ipl.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://dfv.fktsv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://amx.dianchejie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dkx.hcnkem.com

[Q33] 多列分组
来源：http://dpq.pycfn.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xin.chenlongwang.top

[Q34] 每组取第一条
来源：http://ppl.svipenyu.cn

SELECT * FROM (
来源：http://bvf.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kxh.havefunace.top

) t WHERE rn = 1;
来源：http://spf.cheryme.top

[Q35] 内连接
来源：http://ave.sysykeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ong.iojbl.cn

[Q36] 左连接
来源：http://lpc.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://plt.vehdjk.com

[Q37] 右连接
来源：http://stp.nanxuanxn.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ols.hongshengwenyu.top

[Q38] 全外连接（PostgreSQL）
来源：http://kkh.zdqjudy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pqf.uphjek.com

[Q39] 自连接（查上下级）
来源：http://zen.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nxk.yonumen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://apg.yonumen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://auq.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qyh.iojbl.cn

[Q41] 多表连接
来源：http://bdx.birdmap.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rfo.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://ynv.birdmap.top

JOIN products p ON p.id = o.product_id;
来源：http://mby.kuanghao11.cn

[Q42] 连接条件附加过滤
来源：http://ylt.sjlbkw.cn

SELECT u.name, o.amount FROM users u
来源：http://kuo.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qes.smart0.xyz

[Q43] 标量子查询
来源：http://yhv.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ogc.fanxiaobao.xyz

[Q44] IN 子查询
来源：http://skf.yueranfly.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://heq.zhijiandao.cn

[Q45] EXISTS 判断存在
来源：http://vjf.hammf.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tvo.shzxlz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dzy.ydjk.org.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://esh.cheryme.top

[Q47] 与平均值比较
来源：http://icn.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qrf.cucudq.cn

[Q48] CTE 公用表表达式
来源：http://muh.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ovg.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://wvi.xuanzx.com

[Q49] 更新单行
来源：http://mia.fzhhl.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mvd.zhijiandao.cn

[Q50] 批量更新
来源：http://wci.sweek.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://imw.52xcode.cn

[Q51] 用子查询更新
来源：http://xsa.guannengcc.top


<!-- 参考信息 -->