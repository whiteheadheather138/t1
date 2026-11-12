代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rjg.cdnleiting.top

[N06] 判断回文字符串
来源：http://jnx.tian-w.cn

Py:   s == s[::-1]
来源：http://vif.tarul.cn

PHP:  $s === strrev($s);
来源：http://kcf.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://bht.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://dkg.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hbh.jqgufenzy.top

Go:   // 双指针从两端比较
来源：http://ugz.xylfe.cn

Ruby: s == s.reverse
来源：http://lwv.iojbl.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cou.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://civ.52xcode.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lui.daria6918.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pzh.xuetiantiany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rob.yj20258.top

TS:   // 手写 Map<string, number>
来源：http://ise.vehdjk.com

Java: // 手写 HashMap
来源：http://uih.hywenlv.cn

Go:   // 手写 map[int]int
来源：http://ftn.svipenyu.cn

Ruby: // 手写 Hash
来源：http://edg.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://btb.redwolf501.top

[N08] 生成全排列
来源：http://ebx.yfazqb.com

Py:   itertools.permutations(arr)
来源：http://pkx.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://enu.yonumen.top

JS:   // 手写回溯递归
来源：http://yyi.52xcode.cn

TS:   // 手写回溯递归
来源：http://urn.svipenyu.cn

Java: // 手写回溯递归
来源：http://szl.ehwqpu.com

Go:   // 手写回溯递归
来源：http://eyk.0kj1m.cn

Ruby: arr.permutation.to_a
来源：http://xsx.jyoumei.cn

C#:   // 手写回溯递归
来源：http://yuq.sxryk.cn

[N09] 栈与队列
来源：http://kce.yvedp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gop.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hug.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vir.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gui.snrcjt.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tel.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sul.bjfxy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://erm.sxryk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://huh.yongpay.top

[N10] 链表节点定义
来源：http://fgh.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iyd.fehbvm.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ugx.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ilc.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mhw.nanxuanxn.top

Java: class Node { int v; Node next; }
来源：http://wug.yj202588.top

Go:   type Node struct { V int; Next *Node }
来源：http://qet.hywenlv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cza.yuxming.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yqx.havefunace.top

[N11] 二叉树中序遍历
来源：http://gvj.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wtq.yj20258888.top

PHP:  // 手写递归函数
来源：http://jrw.hysaishi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pjz.yfazqb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://myb.chenjidiqi.icu

Java: // 手写递归
来源：http://kzm.guowangkeji.top

Go:   // 手写递归
来源：http://djj.jianghu66.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tzp.sweek.top

C#:   // 手写递归
来源：http://aof.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ywk.zhongyouzk.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://glk.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://loh.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kpu.0kj1m.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rvc.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jav.shanyushiyangtech.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vxf.316326.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ufg.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vbt.jqgfzy.top

================================================================================
来源：http://igf.aizwys.cn

O. 并发与异步
来源：http://eau.chenzaomai.com

================================================================================
来源：http://zar.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://mfs.ywan-chungtsiang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jsy.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oek.zdbjq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://boo.jqgfzy.top

TS:   // 同 JS
来源：http://tsv.0kj1m.cn

Java: new Thread(() -> f()).start()
来源：http://jbc.cqqwz.cn

Go:   go f()
来源：http://gkp.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://uod.gzhubu.top

C#:   Task.Run(() => F());
来源：http://mly.sysykeji.top

[O02] 使用线程池
来源：http://lfx.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gpn.shzxlz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://keg.yfazqb.com

JS:   // worker_threads 线程池
来源：http://wtc.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://hyz.ydzc1.top

Java: Executors.newFixedThreadPool(4)
来源：http://hcw.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ael.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jjv.jinqigufen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://egz.nwbrower.top

[O03] 加锁保护共享数据
来源：http://oic.ppjwa.cn

Py:   with lock: shared += 1
来源：http://yfp.xuanzx.com

PHP:  // 用 flock() 做文件锁
来源：http://tqf.iojbl.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://svn.hcnkem.com

TS:   // 同 JS
来源：http://uuz.hnxiangtu.top

Java: synchronized (this) { shared++; }
来源：http://mci.dashuyun.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://unh.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xns.ehwqpu.com

C#:   lock (gate) { shared++; }
来源：http://osp.cucudq.cn

[O04] 定义异步函数并等待
来源：http://yfk.jinqigfzy.top

Py:   async def f():⏎    await g()
来源：http://vis.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kvx.svipenyu.cn

JS:   async function f() { await g(); }
来源：http://qra.0kj1m.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ixr.xziqi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xdj.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jwn.dianchejie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jbl.ivvv.top

C#:   async Task F() { await G(); }
来源：http://clv.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://twr.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://hsn.fengsongda.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uvl.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://mux.xuetiantiany.cn

TS:   await Promise.all(tasks)
来源：http://uuh.dianchejie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qff.zhaomingkeji.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zoe.zycfv.cn

Ruby: threads.map(&:join)
来源：http://jzt.havefunace.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fcr.iojbl.cn

[O06] 使用进程池
来源：http://lak.c1oappe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ops.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tyj.bbcook.cn

JS:   // child_process / cluster 模块
来源：http://ntb.52xcode.cn

TS:   // child_process / cluster 模块
来源：http://iyn.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://trx.316326.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cew.iojbl.cn

Ruby: // fork 块
来源：http://xja.sjlbkw.cn

C#:   Parallel.For
来源：http://fco.shanyushiyangkeji.top

================================================================================
来源：http://ujw.zhijiandao.cn

P. 常用工具函数
来源：http://izr.xingfuxueyuan.xyz

================================================================================
来源：http://okm.cucudq.cn

[P01] 生成 UUID
来源：http://pgc.nanxinkj.top

Py:   str(uuid.uuid4())
来源：http://nes.vqdsnc.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fbv.ivvv.top

JS:   crypto.randomUUID()
来源：http://gpz.zycfv.cn

TS:   crypto.randomUUID()
来源：http://ziu.yangfankeji.com

Java: UUID.randomUUID().toString()
来源：http://jkm.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://cvu.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://wow.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://asg.0kj1m.cn

[P02] MD5 / SHA256 摘要
来源：http://iuf.bbcook.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://odq.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tfy.hnxiangtu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xyp.jinyuanbaomall.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mff.zhaomingkeji.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jua.uphjek.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kcn.tianlin.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dqu.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xhl.haohaochexian.top

[P03] 生成短随机字符串
来源：http://llm.fktsv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://djm.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nnn.chenjidiqi.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lko.52xcode.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kpk.hongshengwenyu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gcu.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hdw.ybcxt.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rog.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gnw.xuetiantiany.cn

[P04] 求长度
来源：http://zji.ydzc1.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rvc.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rsd.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ojf.epnwcf.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ubo.fengsongda.top

Java: list.size();  map.size();  s.length()
来源：http://nrr.sjlbkw.cn

Go:   len(arr);  len(m)
来源：http://kpq.zhaomingkeji.xyz

Ruby: x.length;  x.size
来源：http://zhn.zdqjudy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://duf.gotoacloud.top

[P05] 判断两个对象内容是否相等
来源：http://yhf.hfpthk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xyu.hfpthk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://idy.shanyushiyangtech.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://puy.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wwt.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uwr.316326.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://qml.yueranfly.top

Ruby: a == b
来源：http://dyg.yuanzhike.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cll.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nzf.hnxiangtu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rmd.yj202588.top

PHP:  if (empty($x)) {}
来源：http://hsj.ybcxt.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bqq.birdmap.top

TS:   if (x == null) {}
来源：http://rvu.meibo888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ykz.fzhhl.top

Go:   if x == nil {}
来源：http://zst.sxryk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aay.jqgufenzy.top

C#:   if (x is null) {}
来源：http://hef.svipenyu.cn

[P07] 防抖与节流
来源：http://yjc.zhaomingkeji.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cat.yuxming.cn

PHP:  // 手写时间戳比较
来源：http://hbo.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ulp.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wbj.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qqz.vehdjk.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kuh.tianlin.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://jkt.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fra.fktsv.cn

[P08] 处理浮点精度问题
来源：http://fxx.fengsongda.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cww.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lva.jqgufenzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xeo.zhongyouzk.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yid.ppjwa.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cwh.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iqy.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xvn.316326.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tcn.zhengqikj.top

================================================================================
来源：http://pgn.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ybs.bjfxy.top

================================================================================
来源：http://asq.quarkkingdee.top

[Q01] 创建表
来源：http://pqk.daxiang520.top

CREATE TABLE users (
来源：http://hwg.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tqz.dashuyun.cn

name VARCHAR(50) NOT NULL,
来源：http://evj.cdnleiting.top

email VARCHAR(100) UNIQUE,
来源：http://twc.vehdjk.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ddi.epnwcf.com

);
来源：http://ddz.cucudq.cn

[Q02] 创建带外键的表
来源：http://vgb.cheryme.top

CREATE TABLE orders (
来源：http://uxt.bbcook.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ehc.wangdashe.top

user_id INT NOT NULL,
来源：http://lod.fehbvm.com

amount DECIMAL(10, 2),
来源：http://yxu.hnqzz.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bou.hywenlv.cn

);
来源：http://ytw.tian-w.cn

[Q03] 增加列
来源：http://zqb.zhijiandao.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fdo.haohaochexian.top

[Q04] 修改列类型
来源：http://dwu.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://her.shzxlz.cn

[Q05] 重命名列
来源：http://ras.redwolf501.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xop.0kj1m.cn

[Q06] 删除列
来源：http://zmg.shangyingyoupin.top

ALTER TABLE users DROP COLUMN age;
来源：http://xah.hywenlv.cn

[Q07] 删除表
来源：http://xzl.yvedp.cn

DROP TABLE IF EXISTS orders;
来源：http://xby.vehdjk.com

[Q08] 创建普通索引
来源：http://rkv.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://usz.shzxlz.cn

[Q09] 创建唯一索引
来源：http://thi.xinyue.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vhy.0kj1m.cn

[Q10] 插入单行
来源：http://vld.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tjw.tanke756.top

[Q11] 一次插入多行
来源：http://srj.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bph.vehdjk.com

[Q12] 插入后取自增 ID
来源：http://ers.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://ywj.yangfankeji.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wbq.havefunace.top

[Q13] 忽略重复插入
来源：http://uqn.nanxinkj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wsf.hywenlv.cn

[Q14] 存在则更新（upsert）
来源：http://oqy.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cvr.yj20258.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://shk.daxiang520.top

[Q15] 查询全部
来源：http://gkd.svipenyu.cn

SELECT * FROM users;
来源：http://ehp.tian-w.cn

[Q16] 查询指定列
来源：http://zps.svipenyu.cn

SELECT id, name FROM users;
来源：http://qft.fengsongda.top

[Q17] 条件查询
来源：http://iyp.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nxz.quarkkingdee.top

[Q18] 模糊匹配
来源：http://yra.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pja.guannengcc.top

[Q19] 范围查询
来源：http://wic.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hjn.316326.xyz

[Q20] IN 列表
来源：http://dfl.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://azd.zdqjudy.top

[Q21] 空值判断
来源：http://njp.gotoacloud.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ukp.sxryk.cn

[Q22] 排序
来源：http://ohk.jinyuanbaomall.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vhf.zdbjq.cn

[Q23] 分页
来源：http://ysz.dianchejie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vro.fanxiaobao.xyz

[Q24] 去重
来源：http://mtb.pengpengdd.cyou

SELECT DISTINCT city FROM users;
来源：http://laj.xuanzx.com

[Q25] 只取前 N 条
来源：http://onn.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ori.316326.xyz

[Q26] 计数
来源：http://fjh.sweek.top

SELECT COUNT(*) FROM users;
来源：http://iuz.gotoacloud.top

[Q27] 条件计数
来源：http://lvi.yj20258888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kvy.svipenyu.cn

[Q28] 求和与平均
来源：http://kla.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hdr.havefunace.top

[Q29] 最大最小值
来源：http://zuw.gotoacloud.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://deo.feifeiyinyue.top

[Q30] 分组统计
来源：http://yzx.chenlongwang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oyd.chenlongwang.top

[Q31] 分组后过滤
来源：http://apf.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cpv.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://jlp.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eyh.guannengcc.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uaf.wangdashe.top

[Q33] 多列分组
来源：http://btz.yuanzhike.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fui.316326.xyz

[Q34] 每组取第一条
来源：http://qgg.0kj1m.cn

SELECT * FROM (
来源：http://pkq.smart0.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://frh.9152youxi.cn

) t WHERE rn = 1;
来源：http://kol.smart0.xyz

[Q35] 内连接
来源：http://wsz.ctjpmb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cfw.nanxinkj.top

[Q36] 左连接
来源：http://xqw.hywenlv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://epp.yuanzhike.top

[Q37] 右连接
来源：http://new.iojbl.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rlg.hcnkem.com

[Q38] 全外连接（PostgreSQL）
来源：http://mrt.bjfxy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ald.zhongyouzk.top

[Q39] 自连接（查上下级）
来源：http://adi.zhixingplan.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bkm.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ida.hnqzz.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zxx.hfpthk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vqv.cdnleiting.top

[Q41] 多表连接
来源：http://xae.svipenyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ogh.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://jan.jyoumei.cn

JOIN products p ON p.id = o.product_id;
来源：http://sfd.fengsongda.top

[Q42] 连接条件附加过滤
来源：http://zoq.xinyue.icu


<!-- 参考信息 -->