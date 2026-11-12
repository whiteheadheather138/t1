代发 wailian999

Ruby: s == s.reverse
来源：http://ajj.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mfx.hongshengwenyu.top

[N07] 两数之和（返回下标）
来源：http://tgd.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tvp.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jhl.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rqc.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://fep.redwolf501.top

Java: // 手写 HashMap
来源：http://fyx.birdmap.top

Go:   // 手写 map[int]int
来源：http://nzd.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://jce.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vno.c1oappe.top

[N08] 生成全排列
来源：http://rxo.pycfn.com

Py:   itertools.permutations(arr)
来源：http://vrp.52xcode.cn

PHP:  // 手写递归交换
来源：http://khi.sufxvd.cn

JS:   // 手写回溯递归
来源：http://iyx.shangyingyoupin.top

TS:   // 手写回溯递归
来源：http://mor.hcnkem.com

Java: // 手写回溯递归
来源：http://kop.ehwqpu.com

Go:   // 手写回溯递归
来源：http://urg.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://czk.guowangkeji.top

C#:   // 手写回溯递归
来源：http://swn.hammf.cn

[N09] 栈与队列
来源：http://whn.ydjk.org.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gbl.meibo888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jnm.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cma.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cax.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qum.xinyue.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vfm.chenjidiqi.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://diu.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ykj.yangfankeji.com

[N10] 链表节点定义
来源：http://gbk.daxiang520.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xlr.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bmh.hongshengwenyu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ons.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fex.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://rco.tarul.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nby.mhx1999.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bvf.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://qgk.zdqjudy.top

[N11] 二叉树中序遍历
来源：http://fca.zhongyouzk.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pyh.zycfv.cn

PHP:  // 手写递归函数
来源：http://wpb.fanxiaobao.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uxp.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ywn.zdbjq.cn

Java: // 手写递归
来源：http://zre.hysaishi.cn

Go:   // 手写递归
来源：http://qra.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ivd.chenlongwang.top

C#:   // 手写递归
来源：http://ujo.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://akn.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bms.daxiang520.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iif.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iko.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tzt.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qrb.52xcode.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kmw.guannengcc.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://okj.zycfv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://umz.quarkkingdee.top

================================================================================
来源：http://tlb.nwbrower.top

O. 并发与异步
来源：http://ptg.cheryme.top

================================================================================
来源：http://ckp.daria6918.cn

[O01] 启动一个线程
来源：http://jot.yongpay.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pqt.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wbi.havefunace.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yaf.fanxiaobao.xyz

TS:   // 同 JS
来源：http://zca.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://gjn.9152youxi.cn

Go:   go f()
来源：http://fuj.guowangkeji.top

Ruby: Thread.new { f }
来源：http://pin.zhaomingkeji.xyz

C#:   Task.Run(() => F());
来源：http://isi.yvedp.cn

[O02] 使用线程池
来源：http://prx.guannengcc.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dti.52xcode.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qrg.meibo888.top

JS:   // worker_threads 线程池
来源：http://wjf.fengsongda.top

TS:   // worker_threads 线程池
来源：http://shs.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://chk.ydzc1.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dzh.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://imk.birdmap.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://stg.iojbl.cn

[O03] 加锁保护共享数据
来源：http://bhi.aizwys.cn

Py:   with lock: shared += 1
来源：http://vzi.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://qix.ppjwa.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://arz.xuetiantiany.cn

TS:   // 同 JS
来源：http://clp.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://boh.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uhn.ivvv.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uta.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://zyd.aizwys.cn

[O04] 定义异步函数并等待
来源：http://phe.nwbrower.top

Py:   async def f():⏎    await g()
来源：http://syh.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hqf.iojbl.cn

JS:   async function f() { await g(); }
来源：http://ovw.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://sps.pycfn.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lwj.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yzb.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://kdo.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://cfm.xingfuxueyuan.xyz

[O05] 并发执行并等待全部完成
来源：http://tcp.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://avw.sxryk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bbl.pengpengdd.cyou

JS:   await Promise.all(tasks)
来源：http://krs.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://rov.yueranfly.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ffp.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ogp.aizwys.cn

Ruby: threads.map(&:join)
来源：http://znl.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zrs.zhiwuduotai.top

[O06] 使用进程池
来源：http://xzf.smart0.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yxv.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tfy.uphjek.com

JS:   // child_process / cluster 模块
来源：http://zkp.shangyingyoupin.top

TS:   // child_process / cluster 模块
来源：http://xqm.52xcode.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rhc.cqqwz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ppy.zdqjudy.top

Ruby: // fork 块
来源：http://svu.ehwqpu.com

C#:   Parallel.For
来源：http://duk.feifeiyinyue.top

================================================================================
来源：http://ubp.ywan-chungtsiang.top

P. 常用工具函数
来源：http://htt.9152youxi.cn

================================================================================
来源：http://adw.jyoumei.cn

[P01] 生成 UUID
来源：http://smo.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://sxu.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://odr.daxiang520.top

JS:   crypto.randomUUID()
来源：http://tav.uphjek.com

TS:   crypto.randomUUID()
来源：http://kaa.tanke756.top

Java: UUID.randomUUID().toString()
来源：http://ghw.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://udx.yueranfly.top

Ruby: SecureRandom.uuid
来源：http://bcm.yongpay.top

C#:   Guid.NewGuid().ToString()
来源：http://yzv.xuetiantiany.cn

[P02] MD5 / SHA256 摘要
来源：http://afw.fehbvm.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qxf.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wmd.sweek.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pwg.xuetiantiany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lld.jinyuanbaomall.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ade.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://anf.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rei.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xrr.mhx1999.top

[P03] 生成短随机字符串
来源：http://kfo.aizwys.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dso.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qvh.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eya.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bfm.xuetiantiany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pki.snrcjt.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vra.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gux.zhijiandao.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zis.tanke756.top

[P04] 求长度
来源：http://uny.hnxiangtu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kqj.shangyingyoupin.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://csz.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qml.gaohongyu789.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://grp.guannengcc.top

Java: list.size();  map.size();  s.length()
来源：http://mye.ydjk.org.cn

Go:   len(arr);  len(m)
来源：http://ray.zhixingplan.top

Ruby: x.length;  x.size
来源：http://ths.pycfn.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://qqe.316326.xyz

[P05] 判断两个对象内容是否相等
来源：http://bzd.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pgu.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oge.mhx1999.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wfm.bjfxy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qjx.hysaishi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lqr.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rno.vqdsnc.cn

Ruby: a == b
来源：http://uwk.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rnx.tarul.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://anw.hnqzz.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eze.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://hfe.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pih.quarkkingdee.top

TS:   if (x == null) {}
来源：http://rjn.quarkkingdee.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mab.hammf.cn

Go:   if x == nil {}
来源：http://dks.tanke756.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://epe.hesvh.cn

C#:   if (x is null) {}
来源：http://pjo.aibaodan.cn

[P07] 防抖与节流
来源：http://twl.fktsv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hvz.zhiwuduotai.top

PHP:  // 手写时间戳比较
来源：http://fxs.cqqwz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://thu.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wsv.zhiwuduotai.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://edn.jinqigufen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tbb.ydjk.org.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fwj.vqdsnc.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yze.yfazqb.com

[P08] 处理浮点精度问题
来源：http://aay.quarkkingdee.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gxp.guannengcc.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oab.uphjek.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://okf.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ftj.jinqigufen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kfw.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sxe.iojbl.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://slf.cucudq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gzt.aibaodan.cn

================================================================================
来源：http://rml.cqqwz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jfp.fengsongda.top

================================================================================
来源：http://taz.0kj1m.cn

[Q01] 创建表
来源：http://ufm.xuetiantiany.cn

CREATE TABLE users (
来源：http://mtp.svipenyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aai.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://srl.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://ahu.cashguo.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cac.nwbrower.top

);
来源：http://jxm.ehwqpu.com

[Q02] 创建带外键的表
来源：http://usc.feifeiyinyue.top

CREATE TABLE orders (
来源：http://tko.daria6918.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sek.jqgufenzy.top

user_id INT NOT NULL,
来源：http://eqp.fktsv.cn

amount DECIMAL(10, 2),
来源：http://orz.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://umr.9152youxi.cn

);
来源：http://sig.gaohongyu789.top

[Q03] 增加列
来源：http://atr.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lqh.iojbl.cn

[Q04] 修改列类型
来源：http://zbt.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vrx.tian-w.cn

[Q05] 重命名列
来源：http://uka.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hag.andypj.xyz

[Q06] 删除列
来源：http://svj.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://jxr.hesvh.cn

[Q07] 删除表
来源：http://drx.yvedp.cn

DROP TABLE IF EXISTS orders;
来源：http://stv.jianghu66.top

[Q08] 创建普通索引
来源：http://cmn.cqqwz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://aij.hfpthk.cn

[Q09] 创建唯一索引
来源：http://ydk.0kj1m.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kwc.shuidangran.top

[Q10] 插入单行
来源：http://wgn.pengpengdd.cyou

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fhc.zycfv.cn

[Q11] 一次插入多行
来源：http://csf.gzhubu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zxo.wangdashe.top

[Q12] 插入后取自增 ID
来源：http://dbr.bbcook.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eeo.ctjpmb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ibp.hongshengwenyu.top

[Q13] 忽略重复插入
来源：http://ssk.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://llv.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://xmv.hnqzz.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hna.jlsjyb.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cgx.guannengcc.top

[Q15] 查询全部
来源：http://bdn.c1oappe.top

SELECT * FROM users;
来源：http://uam.dianchejie.cn

[Q16] 查询指定列
来源：http://vfs.tanke756.top

SELECT id, name FROM users;
来源：http://ilu.ybcxt.top

[Q17] 条件查询
来源：http://ret.9152youxi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nju.gogol.net.cn

[Q18] 模糊匹配
来源：http://sia.tanke756.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pnt.svipenyu.cn

[Q19] 范围查询
来源：http://kyi.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pwb.ivvv.top

[Q20] IN 列表
来源：http://yhr.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://agu.jiagoushi.top

[Q21] 空值判断
来源：http://nld.cheryme.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vla.sysykeji.top

[Q22] 排序
来源：http://yyo.hysaishi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pyp.hnxiangtu.top

[Q23] 分页
来源：http://bku.jianghu66.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://efa.yanxiufei.cn

[Q24] 去重
来源：http://hma.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://wvn.iojbl.cn

[Q25] 只取前 N 条
来源：http://ixs.zhengqikj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qtt.bjfxy.top

[Q26] 计数
来源：http://axb.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://cdk.zhoulong.xyz

[Q27] 条件计数
来源：http://mzq.wangshuangyany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ult.cqqwz.cn

[Q28] 求和与平均
来源：http://skm.yanxiufei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nqr.epnwcf.com

[Q29] 最大最小值
来源：http://uqc.ivvv.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://noc.c1oappe.top

[Q30] 分组统计
来源：http://mis.vehdjk.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wxb.ivvv.top

[Q31] 分组后过滤
来源：http://oxl.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qiq.daria6918.cn

[Q32] 分组拼接字符串
来源：http://yoc.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fsd.c1oappe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fii.jqgufenzy.top

[Q33] 多列分组
来源：http://syf.gogol.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ztd.zhijiandao.cn

[Q34] 每组取第一条
来源：http://bll.feifeiyinyue.top

SELECT * FROM (
来源：http://dtr.jqgfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kws.zhengqikj.top

) t WHERE rn = 1;
来源：http://isz.316326.xyz

[Q35] 内连接
来源：http://ewy.dashuyun.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bhs.pycfn.com

[Q36] 左连接
来源：http://dxl.yangfankeji.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://thb.redwolf501.top

[Q37] 右连接
来源：http://tog.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mtq.cashguo.top

[Q38] 全外连接（PostgreSQL）
来源：http://hnd.zdqjudy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vfz.chenlongwang.top

[Q39] 自连接（查上下级）
来源：http://paa.xinyue.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://edl.ydzc1.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cfx.mhx1999.top

[Q40] 交叉连接（笛卡尔积）
来源：http://aym.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yge.nanxinkj.top

[Q41] 多表连接
来源：http://pmr.jinyuanbaomall.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hyb.sweek.top

JOIN users u ON u.id = o.user_id
来源：http://esp.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://nlm.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://bev.cashguo.top

SELECT u.name, o.amount FROM users u
来源：http://iwv.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ffh.0kj1m.cn

[Q43] 标量子查询
来源：http://llt.xziqi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gvu.birdmap.top

[Q44] IN 子查询
来源：http://zqu.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://imc.mhx1999.top

[Q45] EXISTS 判断存在
来源：http://zqq.yuanzhike.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ngz.ehwqpu.com


<!-- 参考信息 -->