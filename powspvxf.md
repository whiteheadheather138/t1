代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://dkz.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://nkd.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xsy.tarul.cn

Go:   // 双指针从两端比较
来源：http://kco.yfazqb.com

Ruby: s == s.reverse
来源：http://fiv.0kj1m.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mgk.xuanzx.com

[N07] 两数之和（返回下标）
来源：http://swx.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yle.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xqx.ywan-chungtsiang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ubl.svipenyu.cn

TS:   // 手写 Map<string, number>
来源：http://nbv.yj20258.top

Java: // 手写 HashMap
来源：http://tiu.zhengqikj.top

Go:   // 手写 map[int]int
来源：http://qfs.ehwqpu.com

Ruby: // 手写 Hash
来源：http://jdh.fzhhl.top

C#:   // 手写 Dictionary<int, int>
来源：http://zom.hongshengwenyu.top

[N08] 生成全排列
来源：http://bzc.yj202588.top

Py:   itertools.permutations(arr)
来源：http://pgn.daxiang520.top

PHP:  // 手写递归交换
来源：http://yum.bbcook.cn

JS:   // 手写回溯递归
来源：http://yyt.hcnkem.com

TS:   // 手写回溯递归
来源：http://vps.nwbrower.top

Java: // 手写回溯递归
来源：http://nxc.yj20258888.top

Go:   // 手写回溯递归
来源：http://yqq.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://gar.jqgfzy.top

C#:   // 手写回溯递归
来源：http://afi.sjlbkw.cn

[N09] 栈与队列
来源：http://mum.uphjek.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gcj.tanke756.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rfk.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://plm.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://euk.pengpengdd.cyou

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://evi.zhiwuduotai.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qgr.jianghu66.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aoo.nanxuanxn.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ult.sufxvd.cn

[N10] 链表节点定义
来源：http://nvz.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ivm.shuidangran.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ztq.shuidangran.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://reu.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zat.chenzaomai.com

Java: class Node { int v; Node next; }
来源：http://nky.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://vab.jinghuilouyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xhv.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pvx.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://yfx.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rde.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://xzf.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lyq.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://php.gaohongyu789.top

Java: // 手写递归
来源：http://mll.sweek.top

Go:   // 手写递归
来源：http://kyu.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xhx.chenjidiqi.icu

C#:   // 手写递归
来源：http://mfa.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://diu.xuanzx.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://utp.zhiwuduotai.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wth.chenjidiqi.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cns.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fax.fzhhl.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://grr.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://irv.yj202588.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mql.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zph.shzxlz.cn

================================================================================
来源：http://qza.hnxiangtu.top

O. 并发与异步
来源：http://kba.cqqwz.cn

================================================================================
来源：http://amr.yueranfly.top

[O01] 启动一个线程
来源：http://ihs.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wvq.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kkj.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hot.xuetiantiany.cn

TS:   // 同 JS
来源：http://wcg.yangfankeji.com

Java: new Thread(() -> f()).start()
来源：http://lpf.jianghu66.top

Go:   go f()
来源：http://arl.tianlin.xyz

Ruby: Thread.new { f }
来源：http://sir.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://psq.daxiang520.top

[O02] 使用线程池
来源：http://xqk.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iui.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wqv.gzhubu.top

JS:   // worker_threads 线程池
来源：http://lyx.yongpay.top

TS:   // worker_threads 线程池
来源：http://jpv.quarkkingdee.top

Java: Executors.newFixedThreadPool(4)
来源：http://flw.wangdashe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ejp.cucudq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fif.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://psu.jianghu66.top

[O03] 加锁保护共享数据
来源：http://ihe.guannengcc.top

Py:   with lock: shared += 1
来源：http://lox.jinqigufen.top

PHP:  // 用 flock() 做文件锁
来源：http://inw.epnwcf.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nuo.jianghu66.top

TS:   // 同 JS
来源：http://zbd.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://kcq.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kjb.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fyw.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://att.cashguo.top

[O04] 定义异步函数并等待
来源：http://nnv.jianghu66.top

Py:   async def f():⏎    await g()
来源：http://pgx.shzxlz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dsa.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://agu.tian-w.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vqo.hnqzz.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lpu.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yvh.xuanzx.com

Ruby: # 用 Fiber 或 async gem
来源：http://knk.meibo888.top

C#:   async Task F() { await G(); }
来源：http://mqk.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://ink.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://xtk.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nwq.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://kwq.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://jda.jianghu66.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cir.zhengqikj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qvm.yongpay.top

Ruby: threads.map(&:join)
来源：http://vql.c1oappe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://icp.vehdjk.com

[O06] 使用进程池
来源：http://weh.dashuyun.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yjh.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zzj.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://rzk.sysykeji.top

TS:   // child_process / cluster 模块
来源：http://wfn.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://okj.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jqs.hysaishi.cn

Ruby: // fork 块
来源：http://bia.zycfv.cn

C#:   Parallel.For
来源：http://ube.52xcode.cn

================================================================================
来源：http://ncg.mhx1999.top

P. 常用工具函数
来源：http://nki.nanxinkj.top

================================================================================
来源：http://rfe.havefunace.top

[P01] 生成 UUID
来源：http://upu.hesvh.cn

Py:   str(uuid.uuid4())
来源：http://jwm.hysaishi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sre.fengsongda.top

JS:   crypto.randomUUID()
来源：http://fjv.xylfe.cn

TS:   crypto.randomUUID()
来源：http://wqb.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://wwb.yongpay.top

Go:   // 用 github.com/google/uuid
来源：http://hvl.zdbjq.cn

Ruby: SecureRandom.uuid
来源：http://wup.yangfankeji.com

C#:   Guid.NewGuid().ToString()
来源：http://jec.xinyue.icu

[P02] MD5 / SHA256 摘要
来源：http://nqd.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://afq.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lco.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fsh.jinyuanbaomall.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jml.uphjek.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ujl.sweek.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jad.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qdi.cucudq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ftz.yj20258.top

[P03] 生成短随机字符串
来源：http://guw.yanxiufei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ngl.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://flh.cqqwz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tnk.hammf.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gwh.zycfv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ewl.ydzc1.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qiu.cashguo.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vvm.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://okx.shangyingyoupin.top

[P04] 求长度
来源：http://syz.pengpengdd.cyou

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vse.snrcjt.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hjg.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xtu.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://imj.yanxiufei.cn

Java: list.size();  map.size();  s.length()
来源：http://xmh.jiagoushi.top

Go:   len(arr);  len(m)
来源：http://rqm.aizwys.cn

Ruby: x.length;  x.size
来源：http://dxp.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://lvh.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://awb.zhengqikj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://iyt.dashuyun.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uwd.redwolf501.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uoi.tanke756.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ihx.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gmi.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://zov.sufxvd.cn

Ruby: a == b
来源：http://ime.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fnp.epnwcf.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://crl.xingfuxueyuan.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cuv.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://igq.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qxl.cheryme.top

TS:   if (x == null) {}
来源：http://nbq.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://krr.ivvv.top

Go:   if x == nil {}
来源：http://qaz.cqqwz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wwv.zdbjq.cn

C#:   if (x is null) {}
来源：http://dby.shangyingyoupin.top

[P07] 防抖与节流
来源：http://oes.zhaomingkeji.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uez.kuanghao11.cn

PHP:  // 手写时间戳比较
来源：http://kwp.dianchejie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nzr.yfazqb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fls.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xag.xylfe.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mba.kuanghao11.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://prf.ywan-chungtsiang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cyl.aizwys.cn

[P08] 处理浮点精度问题
来源：http://orv.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yfi.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jrb.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dbi.snrcjt.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://emm.tian-w.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://svb.mhx1999.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://poz.cashguo.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mgy.ehwqpu.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://emq.shanyushiyangtech.top

================================================================================
来源：http://nft.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rgi.jiagoushi.top

================================================================================
来源：http://dfq.jianghu66.top

[Q01] 创建表
来源：http://qji.316326.xyz

CREATE TABLE users (
来源：http://llo.havefunace.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wsu.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://vdj.yvedp.cn

email VARCHAR(100) UNIQUE,
来源：http://svi.aibaodan.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ccl.gotoacloud.top

);
来源：http://tms.andypj.xyz

[Q02] 创建带外键的表
来源：http://nyb.52xcode.cn

CREATE TABLE orders (
来源：http://god.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rkq.c1oappe.top

user_id INT NOT NULL,
来源：http://hud.cucudq.cn

amount DECIMAL(10, 2),
来源：http://rqh.ywan-chungtsiang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rfu.chenzaomai.com

);
来源：http://hhq.zhongyouzk.top

[Q03] 增加列
来源：http://vwg.hammf.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ter.smart0.xyz

[Q04] 修改列类型
来源：http://psb.guowangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ogz.52xcode.cn

[Q05] 重命名列
来源：http://sja.smart0.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yin.hnqzz.top

[Q06] 删除列
来源：http://pkz.vehdjk.com

ALTER TABLE users DROP COLUMN age;
来源：http://gna.epnwcf.com

[Q07] 删除表
来源：http://peo.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://tdf.yj20258.top

[Q08] 创建普通索引
来源：http://adz.cheryme.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qtf.hfpthk.cn

[Q09] 创建唯一索引
来源：http://mnb.epnwcf.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://smi.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://xoq.epnwcf.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hvq.nanxinkj.top

[Q11] 一次插入多行
来源：http://jyr.tanke756.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sul.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://ucz.bjfxy.top

INSERT INTO users (name) VALUES ('C');
来源：http://fyh.yueranfly.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://glv.sxryk.cn

[Q13] 忽略重复插入
来源：http://dzc.svipenyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zmi.yonumen.top

[Q14] 存在则更新（upsert）
来源：http://cdz.daria6918.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ucz.cdnleiting.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://quk.sufxvd.cn

[Q15] 查询全部
来源：http://lyy.gotoacloud.top

SELECT * FROM users;
来源：http://xoo.tanke756.top

[Q16] 查询指定列
来源：http://hmu.ybcxt.top

SELECT id, name FROM users;
来源：http://tzj.jqgufenzy.top

[Q17] 条件查询
来源：http://pkc.zhongyouzk.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cgh.fehbvm.com

[Q18] 模糊匹配
来源：http://pdg.jiagoushi.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hhd.tian-w.cn

[Q19] 范围查询
来源：http://bng.fzhhl.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uxp.hcnkem.com

[Q20] IN 列表
来源：http://toy.shangyingyoupin.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ksg.c1oappe.top

[Q21] 空值判断
来源：http://pva.sysykeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hnq.jinyuanbaomall.cn

[Q22] 排序
来源：http://hkj.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://isa.mhx1999.top

[Q23] 分页
来源：http://ifq.dianchejie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uol.nanxuanxn.top

[Q24] 去重
来源：http://ces.daxiang520.top

SELECT DISTINCT city FROM users;
来源：http://ugq.tanke756.top

[Q25] 只取前 N 条
来源：http://kdm.shanyushiyangtech.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lbp.cashguo.top

[Q26] 计数
来源：http://qmd.yonumen.top

SELECT COUNT(*) FROM users;
来源：http://abr.aizwys.cn

[Q27] 条件计数
来源：http://ozk.pengpengdd.cyou

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zfa.9152youxi.cn

[Q28] 求和与平均
来源：http://qlv.mhx1999.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vjx.feifeiyinyue.top

[Q29] 最大最小值
来源：http://jnr.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://avx.pycfn.com

[Q30] 分组统计
来源：http://exy.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cyx.wangdashe.top

[Q31] 分组后过滤
来源：http://oce.ydzc1.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rmv.zhaomingkeji.xyz

[Q32] 分组拼接字符串
来源：http://tej.hfpthk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dli.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xpu.jqgufenzy.top

[Q33] 多列分组
来源：http://pgg.316326.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lnp.sweek.top

[Q34] 每组取第一条
来源：http://nxg.svipenyu.cn

SELECT * FROM (
来源：http://qyl.gaohongyu789.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pfp.daxiang520.top

) t WHERE rn = 1;
来源：http://sly.daxiang520.top

[Q35] 内连接
来源：http://pdv.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ntf.aizwys.cn

[Q36] 左连接
来源：http://byd.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fai.shangyingyoupin.top

[Q37] 右连接
来源：http://lky.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yvb.ppjwa.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gvx.yuxming.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://icw.fanxiaobao.xyz

[Q39] 自连接（查上下级）
来源：http://vdk.cashguo.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kzl.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ier.feifeiyinyue.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gvn.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lux.zhixingplan.top

[Q41] 多表连接
来源：http://dbq.cucudq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xyw.dashuyun.cn

JOIN users u ON u.id = o.user_id
来源：http://akr.zhengqikj.top

JOIN products p ON p.id = o.product_id;
来源：http://xwr.nanxuanxn.top

[Q42] 连接条件附加过滤
来源：http://chv.xuanzx.com

SELECT u.name, o.amount FROM users u
来源：http://qnj.yuxming.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pnq.yvedp.cn

[Q43] 标量子查询
来源：http://bee.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gsf.fanxiaobao.xyz


<!-- 参考信息 -->