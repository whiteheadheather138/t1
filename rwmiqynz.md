代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://edf.yj20258888.top

TS:   s === [...s].reverse().join("")
来源：http://cdl.sweek.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jub.xinyue.icu

Go:   // 双指针从两端比较
来源：http://iat.pycfn.com

Ruby: s == s.reverse
来源：http://jkh.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tlc.smart0.xyz

[N07] 两数之和（返回下标）
来源：http://fyz.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gby.xinyue.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tsz.ywan-chungtsiang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://byc.gogol.net.cn

TS:   // 手写 Map<string, number>
来源：http://myy.smart0.xyz

Java: // 手写 HashMap
来源：http://too.ydzc1.top

Go:   // 手写 map[int]int
来源：http://uiw.andypj.xyz

Ruby: // 手写 Hash
来源：http://bbi.jinqigfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://hdy.sxryk.cn

[N08] 生成全排列
来源：http://lbg.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://wal.epnwcf.com

PHP:  // 手写递归交换
来源：http://sxp.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://avk.pycfn.com

TS:   // 手写回溯递归
来源：http://nba.fehbvm.com

Java: // 手写回溯递归
来源：http://wus.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://pad.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://vff.jqgfzy.top

C#:   // 手写回溯递归
来源：http://jbh.xuanzx.com

[N09] 栈与队列
来源：http://svc.snrcjt.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://omr.dashuyun.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ddd.zhoulong.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://faz.hywenlv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jok.yongpay.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tkj.shangyingyoupin.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://all.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://euj.xuetiantiany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://swv.guowangkeji.top

[N10] 链表节点定义
来源：http://eoc.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cqs.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cmw.nanxuanxn.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bub.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wcq.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://afm.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://bny.kuanghao11.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tgn.pycfn.com

C#:   class Node { public int V; public Node? Next; }
来源：http://bqw.zhixingplan.top

[N11] 二叉树中序遍历
来源：http://jrq.sjlbkw.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pcb.andypj.xyz

PHP:  // 手写递归函数
来源：http://bub.andypj.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xky.zhaomingkeji.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://spc.pycfn.com

Java: // 手写递归
来源：http://pxt.fktsv.cn

Go:   // 手写递归
来源：http://igg.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eaw.yvedp.cn

C#:   // 手写递归
来源：http://tob.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ecr.nanxuanxn.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lxb.mhx1999.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ewg.iojbl.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eeg.jyoumei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://znf.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://daj.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ycp.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eqm.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bqa.iojbl.cn

================================================================================
来源：http://rwe.bbcook.cn

O. 并发与异步
来源：http://lxg.yj20258888.top

================================================================================
来源：http://dxa.dianchejie.cn

[O01] 启动一个线程
来源：http://alx.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aan.gotoacloud.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ggw.yanxiufei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xte.gotoacloud.top

TS:   // 同 JS
来源：http://csq.0kj1m.cn

Java: new Thread(() -> f()).start()
来源：http://zhp.yvedp.cn

Go:   go f()
来源：http://rma.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://ptw.redwolf501.top

C#:   Task.Run(() => F());
来源：http://lcv.fengsongda.top

[O02] 使用线程池
来源：http://bkm.vehdjk.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lby.xingfuxueyuan.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ilv.yj20258.top

JS:   // worker_threads 线程池
来源：http://bup.nwbrower.top

TS:   // worker_threads 线程池
来源：http://hwq.yueranfly.top

Java: Executors.newFixedThreadPool(4)
来源：http://sle.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fpc.nanxuanxn.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ljo.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yyi.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://tdc.fzhhl.top

Py:   with lock: shared += 1
来源：http://wmc.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://utv.jinyuanbaomall.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ckv.jqgufenzy.top

TS:   // 同 JS
来源：http://bpx.zhengqikj.top

Java: synchronized (this) { shared++; }
来源：http://nnl.gzhubu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iix.9152youxi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ndl.feifeiyinyue.top

C#:   lock (gate) { shared++; }
来源：http://yqd.cucudq.cn

[O04] 定义异步函数并等待
来源：http://jvj.yfazqb.com

Py:   async def f():⏎    await g()
来源：http://zqz.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iol.jinqigfzy.top

JS:   async function f() { await g(); }
来源：http://fwq.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kuh.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://svg.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lmy.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vls.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://iak.hnxiangtu.top

[O05] 并发执行并等待全部完成
来源：http://bjj.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://cnf.c1oappe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hmq.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://aoq.ehwqpu.com

TS:   await Promise.all(tasks)
来源：http://nvz.52xcode.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oqp.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tem.bbcook.cn

Ruby: threads.map(&:join)
来源：http://lkd.ctjpmb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://zoi.ppjwa.cn

[O06] 使用进程池
来源：http://his.hesvh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://woc.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wct.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://wme.dashuyun.cn

TS:   // child_process / cluster 模块
来源：http://bsm.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rzq.ydjk.org.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wwq.quarkkingdee.top

Ruby: // fork 块
来源：http://rmy.feifeiyinyue.top

C#:   Parallel.For
来源：http://lcx.uphjek.com

================================================================================
来源：http://xxx.hammf.cn

P. 常用工具函数
来源：http://mvh.redwolf501.top

================================================================================
来源：http://irk.cucudq.cn

[P01] 生成 UUID
来源：http://njm.yongpay.top

Py:   str(uuid.uuid4())
来源：http://jag.jianghu66.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jwe.fktsv.cn

JS:   crypto.randomUUID()
来源：http://djq.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://and.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://cni.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://lgs.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://eat.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://mur.0kj1m.cn

[P02] MD5 / SHA256 摘要
来源：http://tck.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ntu.shanyushiyangtech.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lls.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qzv.zhixingplan.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zkv.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ham.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bla.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://owq.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://anv.meibo888.top

[P03] 生成短随机字符串
来源：http://nut.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ugv.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://alt.gotoacloud.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://doa.jqgufenzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sua.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://myk.xuetiantiany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nib.chenzaomai.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://xbr.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ysr.shanyushiyangtech.top

[P04] 求长度
来源：http://ztn.yj202588.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hbe.xuetiantiany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ueg.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ios.smart0.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fot.yueranfly.top

Java: list.size();  map.size();  s.length()
来源：http://pil.tian-w.cn

Go:   len(arr);  len(m)
来源：http://opu.chenlongwang.top

Ruby: x.length;  x.size
来源：http://fgm.hysaishi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ioz.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://ahs.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mte.hcnkem.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iiy.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vim.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ire.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kjh.daxiang520.top

Go:   reflect.DeepEqual(a, b)
来源：http://qgw.ybcxt.top

Ruby: a == b
来源：http://hao.cashguo.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bsy.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gkh.yuxming.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nfb.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://ols.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://egz.cdnleiting.top

TS:   if (x == null) {}
来源：http://kto.zhiwuduotai.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rtm.zhijiandao.cn

Go:   if x == nil {}
来源：http://bsg.hywenlv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qzi.zdqjudy.top

C#:   if (x is null) {}
来源：http://ult.yj20258888.top

[P07] 防抖与节流
来源：http://qwr.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hov.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://lro.gaohongyu789.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jgg.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lem.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gts.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xzb.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://sjq.cucudq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wid.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://lsm.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nyf.cucudq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dcd.fktsv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://urr.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pfu.shanyushiyangtech.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xmx.xinyue.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://asm.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yho.316326.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hce.mhx1999.top

================================================================================
来源：http://bfs.aizwys.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xsj.haohaochexian.top

================================================================================
来源：http://dkc.hywenlv.cn

[Q01] 创建表
来源：http://dhb.316326.xyz

CREATE TABLE users (
来源：http://zbl.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fpv.zhijiandao.cn

name VARCHAR(50) NOT NULL,
来源：http://jxs.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://tbr.jiagoushi.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fvp.jinghuilouyu.cn

);
来源：http://lvk.shzxlz.cn

[Q02] 创建带外键的表
来源：http://ims.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://sjl.jyoumei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gwb.xylfe.cn

user_id INT NOT NULL,
来源：http://ohh.xylfe.cn

amount DECIMAL(10, 2),
来源：http://zdz.chenjidiqi.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jez.xingfuxueyuan.xyz

);
来源：http://kpc.jinghuilouyu.cn

[Q03] 增加列
来源：http://pnj.316326.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lhj.316326.xyz

[Q04] 修改列类型
来源：http://tdq.0kj1m.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hjz.dashuyun.cn

[Q05] 重命名列
来源：http://wox.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ycj.fzhhl.top

[Q06] 删除列
来源：http://ilm.ivvv.top

ALTER TABLE users DROP COLUMN age;
来源：http://ccd.zdqjudy.top

[Q07] 删除表
来源：http://vxr.yongpay.top

DROP TABLE IF EXISTS orders;
来源：http://hox.jinghuilouyu.cn

[Q08] 创建普通索引
来源：http://ruh.hfpthk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wvm.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://nct.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ruf.xylfe.cn

[Q10] 插入单行
来源：http://rgu.uphjek.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vyx.xylfe.cn

[Q11] 一次插入多行
来源：http://gin.ybcxt.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xtu.tianlin.xyz

[Q12] 插入后取自增 ID
来源：http://sjy.xuetiantiany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ieb.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kic.tian-w.cn

[Q13] 忽略重复插入
来源：http://sle.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mzw.wangdashe.top

[Q14] 存在则更新（upsert）
来源：http://sfp.kuanghao11.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mhm.yj202588.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yyr.9152youxi.cn

[Q15] 查询全部
来源：http://rzq.zhengqikj.top

SELECT * FROM users;
来源：http://jai.sxryk.cn

[Q16] 查询指定列
来源：http://qoi.jqgufenzy.top

SELECT id, name FROM users;
来源：http://uuh.bbcook.cn

[Q17] 条件查询
来源：http://lqs.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nqg.ydzc1.top

[Q18] 模糊匹配
来源：http://fts.sysykeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://efy.jinghuilouyu.cn

[Q19] 范围查询
来源：http://gpj.vehdjk.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yka.epnwcf.com

[Q20] IN 列表
来源：http://zxy.xylfe.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nle.zhiwuduotai.top

[Q21] 空值判断
来源：http://qfq.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ync.gogol.net.cn

[Q22] 排序
来源：http://sjs.aizwys.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hai.tian-w.cn

[Q23] 分页
来源：http://lzz.wangshuangyany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qxh.cashguo.top

[Q24] 去重
来源：http://ezw.sweek.top

SELECT DISTINCT city FROM users;
来源：http://jaj.cucudq.cn

[Q25] 只取前 N 条
来源：http://nwv.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bax.shzxlz.cn

[Q26] 计数
来源：http://ppd.ppjwa.cn

SELECT COUNT(*) FROM users;
来源：http://fst.xziqi.cn

[Q27] 条件计数
来源：http://xgt.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bra.bbcook.cn

[Q28] 求和与平均
来源：http://fhw.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://asd.xylfe.cn

[Q29] 最大最小值
来源：http://qei.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://piw.yvedp.cn

[Q30] 分组统计
来源：http://svf.cdnleiting.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zkv.tarul.cn

[Q31] 分组后过滤
来源：http://tmi.cdnleiting.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rwu.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://rpu.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rxy.fzhhl.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zwx.sweek.top

[Q33] 多列分组
来源：http://aik.jinghuilouyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lmk.fehbvm.com

[Q34] 每组取第一条
来源：http://cco.feifeiyinyue.top

SELECT * FROM (
来源：http://cqd.ywan-chungtsiang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://doj.fzhhl.top

) t WHERE rn = 1;
来源：http://nmt.jinqigufen.top

[Q35] 内连接
来源：http://fud.vqdsnc.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://krs.fanxiaobao.xyz

[Q36] 左连接
来源：http://frx.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nls.xinyue.icu

[Q37] 右连接
来源：http://ygj.zhoulong.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rbj.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://dho.guannengcc.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://usk.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://vot.gzhubu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://muc.jinyuanbaomall.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mpb.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fqt.havefunace.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fco.cucudq.cn

[Q41] 多表连接
来源：http://dwp.ehwqpu.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://oij.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://qpo.chenlongwang.top

JOIN products p ON p.id = o.product_id;
来源：http://cpt.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://cix.andypj.xyz

SELECT u.name, o.amount FROM users u
来源：http://otv.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xmy.ybcxt.top

[Q43] 标量子查询
来源：http://gqb.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rbi.xinyue.icu


<!-- 参考信息 -->