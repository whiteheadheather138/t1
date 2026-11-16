代发 wailian999

Go:   // 手写 map[int]int
来源：http://ipc.zhixingplan.top

Ruby: // 手写 Hash
来源：http://qrw.sjlbkw.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sol.xinyue.icu

[N08] 生成全排列
来源：http://uod.xziqi.cn

Py:   itertools.permutations(arr)
来源：http://msk.ydzc1.top

PHP:  // 手写递归交换
来源：http://mrl.yonumen.top

JS:   // 手写回溯递归
来源：http://uzx.fehbvm.com

TS:   // 手写回溯递归
来源：http://bhh.sysykeji.top

Java: // 手写回溯递归
来源：http://mwg.fanxiaobao.xyz

Go:   // 手写回溯递归
来源：http://vkt.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://dma.shuidangran.top

C#:   // 手写回溯递归
来源：http://zrj.snrcjt.cn

[N09] 栈与队列
来源：http://xmj.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rhl.yuanzhike.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bsd.hammf.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lwg.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wol.xuanzx.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ujr.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qtu.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qgt.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://htb.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://pny.gogol.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ymo.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://tzp.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rva.zhaomingkeji.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bcu.shanyushiyangtech.top

Java: class Node { int v; Node next; }
来源：http://ufn.gaohongyu789.top

Go:   type Node struct { V int; Next *Node }
来源：http://lxi.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eab.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yvr.hcnkem.com

[N11] 二叉树中序遍历
来源：http://tuj.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gwd.chenzaomai.com

PHP:  // 手写递归函数
来源：http://zmf.smart0.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ucg.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ovu.quarkkingdee.top

Java: // 手写递归
来源：http://elk.cucudq.cn

Go:   // 手写递归
来源：http://jjm.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://idl.zycfv.cn

C#:   // 手写递归
来源：http://hna.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oiy.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ski.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://etw.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vgk.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://spp.vehdjk.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lda.52xcode.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yiq.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://llk.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://acr.zhaomingkeji.xyz

================================================================================
来源：http://mzo.hongshengwenyu.top

O. 并发与异步
来源：http://ubo.haohaochexian.top

================================================================================
来源：http://was.zhixingplan.top

[O01] 启动一个线程
来源：http://xkh.shangyingyoupin.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://odp.kuanghao11.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cgh.jianghu66.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://szx.9152youxi.cn

TS:   // 同 JS
来源：http://kgs.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://loc.hesvh.cn

Go:   go f()
来源：http://bxc.tianlin.xyz

Ruby: Thread.new { f }
来源：http://ggu.wangshuangyany.cn

C#:   Task.Run(() => F());
来源：http://dkj.xinyue.icu

[O02] 使用线程池
来源：http://upc.yuxming.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uzx.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cvg.zhaomingkeji.xyz

JS:   // worker_threads 线程池
来源：http://oxn.jqgfzy.top

TS:   // worker_threads 线程池
来源：http://wrq.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://fpe.jqgfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zia.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fgt.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rei.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://ujq.guowangkeji.top

Py:   with lock: shared += 1
来源：http://lky.nanxinkj.top

PHP:  // 用 flock() 做文件锁
来源：http://hou.wangshuangyany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cwt.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://awp.jqgfzy.top

Java: synchronized (this) { shared++; }
来源：http://fkm.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rzg.fehbvm.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ivk.xuanzx.com

C#:   lock (gate) { shared++; }
来源：http://emf.hongshengwenyu.top

[O04] 定义异步函数并等待
来源：http://knq.sxryk.cn

Py:   async def f():⏎    await g()
来源：http://xjm.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://efw.zhengqikj.top

JS:   async function f() { await g(); }
来源：http://zke.zhixingplan.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vxr.tanke756.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gco.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://not.yj20258.top

Ruby: # 用 Fiber 或 async gem
来源：http://nil.iojbl.cn

C#:   async Task F() { await G(); }
来源：http://wze.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://vmu.smart0.xyz

Py:   asyncio.gather(*tasks)
来源：http://izr.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://irr.yongpay.top

JS:   await Promise.all(tasks)
来源：http://hyw.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://ybg.hywenlv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lmr.jinqigfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bvi.52xcode.cn

Ruby: threads.map(&:join)
来源：http://erq.9152youxi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hvi.cdnleiting.top

[O06] 使用进程池
来源：http://nne.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://enq.zdqjudy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sbg.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://jxa.tarul.cn

TS:   // child_process / cluster 模块
来源：http://dok.aizwys.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sxo.andypj.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hsi.sufxvd.cn

Ruby: // fork 块
来源：http://tvt.smart0.xyz

C#:   Parallel.For
来源：http://wrr.sysykeji.top

================================================================================
来源：http://cud.bjfxy.top

P. 常用工具函数
来源：http://pul.gzhubu.top

================================================================================
来源：http://tsf.chenjidiqi.icu

[P01] 生成 UUID
来源：http://psj.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://nic.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mar.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://jqg.hnxiangtu.top

TS:   crypto.randomUUID()
来源：http://aal.meibo888.top

Java: UUID.randomUUID().toString()
来源：http://jyh.jqgufenzy.top

Go:   // 用 github.com/google/uuid
来源：http://pdj.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://ibr.shanyushiyangtech.top

C#:   Guid.NewGuid().ToString()
来源：http://pyw.gzhubu.top

[P02] MD5 / SHA256 摘要
来源：http://mgn.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gdm.xylfe.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nuk.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pha.zhiwuduotai.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ljr.zycfv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eph.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xqx.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lua.nanxinkj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rhm.yuxming.cn

[P03] 生成短随机字符串
来源：http://smq.hesvh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zmg.daxiang520.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xqd.fengsongda.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mig.tanke756.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kum.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://txm.birdmap.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xio.chenzaomai.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://dpg.guowangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ykg.hfpthk.cn

[P04] 求长度
来源：http://khr.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wjz.snrcjt.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hsm.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bei.cheryme.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bzo.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://rkg.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://jmm.hnxiangtu.top

Ruby: x.length;  x.size
来源：http://sgx.sxryk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ctj.fanxiaobao.xyz

[P05] 判断两个对象内容是否相等
来源：http://pzm.gogol.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xub.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pjx.fengsongda.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tzx.hnqzz.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xjs.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://toy.hcnkem.com

Go:   reflect.DeepEqual(a, b)
来源：http://omk.c1oappe.top

Ruby: a == b
来源：http://khx.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cxh.gaohongyu789.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hby.jlsjyb.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yga.tianlin.xyz

PHP:  if (empty($x)) {}
来源：http://dum.zhixingplan.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ztz.zhongyouzk.top

TS:   if (x == null) {}
来源：http://gno.zhoulong.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://mlx.zhixingplan.top

Go:   if x == nil {}
来源：http://hez.jinghuilouyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mhs.jinqigufen.top

C#:   if (x is null) {}
来源：http://glh.ivvv.top

[P07] 防抖与节流
来源：http://ipj.shzxlz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uks.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://gio.316326.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iaz.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ykw.jianghu66.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aqw.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uxh.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mbz.ydzc1.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ceo.bjfxy.top

[P08] 处理浮点精度问题
来源：http://igi.xingfuxueyuan.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://egc.zhiwuduotai.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gnh.hongshengwenyu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jqf.gogol.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fcn.ydzc1.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://her.jinyuanbaomall.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ulx.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lwc.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yeh.jinghuilouyu.cn

================================================================================
来源：http://yfd.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mox.ivvv.top

================================================================================
来源：http://jal.sxryk.cn

[Q01] 创建表
来源：http://xes.yonumen.top

CREATE TABLE users (
来源：http://qvy.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pww.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://mxt.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://mca.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hha.shzxlz.cn

);
来源：http://nkg.jinghuilouyu.cn

[Q02] 创建带外键的表
来源：http://skr.shzxlz.cn

CREATE TABLE orders (
来源：http://yyg.ydjk.org.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bcw.meibo888.top

user_id INT NOT NULL,
来源：http://nqs.cqqwz.cn

amount DECIMAL(10, 2),
来源：http://bqr.feifeiyinyue.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bzr.yj202588.top

);
来源：http://ibz.ydzc1.top

[Q03] 增加列
来源：http://scx.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rgs.yueranfly.top

[Q04] 修改列类型
来源：http://yhr.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qqe.yongpay.top

[Q05] 重命名列
来源：http://yje.jinghuilouyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://twk.jinyuanbaomall.cn

[Q06] 删除列
来源：http://hcl.aizwys.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hdj.nanxinkj.top

[Q07] 删除表
来源：http://mlo.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://hwf.guannengcc.top

[Q08] 创建普通索引
来源：http://raw.jinghuilouyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lhi.shanyushiyangkeji.top

[Q09] 创建唯一索引
来源：http://iot.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gyi.sufxvd.cn

[Q10] 插入单行
来源：http://ljg.daria6918.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qjh.chenzaomai.com

[Q11] 一次插入多行
来源：http://qvo.9152youxi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aoj.yj20258.top

[Q12] 插入后取自增 ID
来源：http://yzp.jianghu66.top

INSERT INTO users (name) VALUES ('C');
来源：http://ibc.nanxuanxn.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pwb.birdmap.top

[Q13] 忽略重复插入
来源：http://jwr.gzhubu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hfg.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://zdr.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rqf.pycfn.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ptf.sufxvd.cn

[Q15] 查询全部
来源：http://qgo.yj20258888.top

SELECT * FROM users;
来源：http://xgo.hfpthk.cn

[Q16] 查询指定列
来源：http://cph.ehwqpu.com

SELECT id, name FROM users;
来源：http://jec.ppjwa.cn

[Q17] 条件查询
来源：http://wqo.guannengcc.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vcz.yueranfly.top

[Q18] 模糊匹配
来源：http://auj.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ysm.jinqigufen.top

[Q19] 范围查询
来源：http://nkt.chenlongwang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pbs.zhengqikj.top

[Q20] IN 列表
来源：http://kgv.hnqzz.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zxi.pengpengdd.cyou

[Q21] 空值判断
来源：http://arq.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zug.jqgfzy.top

[Q22] 排序
来源：http://veg.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hmm.bbcook.cn

[Q23] 分页
来源：http://dpf.quarkkingdee.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jdz.zhijiandao.cn

[Q24] 去重
来源：http://toz.yj202588.top

SELECT DISTINCT city FROM users;
来源：http://zry.daxiang520.top

[Q25] 只取前 N 条
来源：http://esv.gotoacloud.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vln.yfazqb.com

[Q26] 计数
来源：http://ekg.iojbl.cn

SELECT COUNT(*) FROM users;
来源：http://oth.vqdsnc.cn

[Q27] 条件计数
来源：http://yey.xylfe.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ort.zhixingplan.top

[Q28] 求和与平均
来源：http://mhw.c1oappe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://arh.ppjwa.cn

[Q29] 最大最小值
来源：http://khl.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wvh.yj202588.top

[Q30] 分组统计
来源：http://ovj.zhiwuduotai.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ewv.yuxming.cn

[Q31] 分组后过滤
来源：http://vuk.ppjwa.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xyv.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://lkz.uphjek.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://saa.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wiu.jqgfzy.top

[Q33] 多列分组
来源：http://ecp.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dcy.ivvv.top

[Q34] 每组取第一条
来源：http://sgw.yongpay.top

SELECT * FROM (
来源：http://nbq.shanyushiyangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dev.jqgufenzy.top

) t WHERE rn = 1;
来源：http://yym.hesvh.cn

[Q35] 内连接
来源：http://zxf.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xzz.gaohongyu789.top

[Q36] 左连接
来源：http://olc.iojbl.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tld.hesvh.cn

[Q37] 右连接
来源：http://rwg.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fyw.daria6918.cn

[Q38] 全外连接（PostgreSQL）
来源：http://yvy.chenzaomai.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kex.hesvh.cn

[Q39] 自连接（查上下级）
来源：http://buh.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xck.nanxinkj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tha.yanxiufei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dka.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ueb.ivvv.top

[Q41] 多表连接
来源：http://rcw.guannengcc.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xny.ehwqpu.com

JOIN users u ON u.id = o.user_id
来源：http://shk.jinyuanbaomall.cn

JOIN products p ON p.id = o.product_id;
来源：http://qzx.zhaomingkeji.xyz

[Q42] 连接条件附加过滤
来源：http://lgl.dianchejie.cn

SELECT u.name, o.amount FROM users u
来源：http://sms.tianlin.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pxm.pengpengdd.cyou

[Q43] 标量子查询
来源：http://apz.tian-w.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nsb.redwolf501.top

[Q44] IN 子查询
来源：http://ntk.kuanghao11.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lux.pengpengdd.cyou

[Q45] EXISTS 判断存在
来源：http://rmj.yuxming.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pbr.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://amw.ydzc1.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zok.ydjk.org.cn

[Q47] 与平均值比较
来源：http://nrj.shanyushiyangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bma.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://xku.chenjidiqi.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zix.hnqzz.top

SELECT * FROM t WHERE c > 5;
来源：http://tls.wangdashe.top

[Q49] 更新单行
来源：http://cgz.shuidangran.top


<!-- 参考信息 -->