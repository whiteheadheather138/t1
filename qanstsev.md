代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://hvz.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://osg.iojbl.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://crr.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://jqo.zycfv.cn

Ruby: s == s.reverse
来源：http://hwa.ydzc1.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zjp.jiagoushi.top

[N07] 两数之和（返回下标）
来源：http://wpz.zhongyouzk.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jsp.nwbrower.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ozk.fktsv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xuo.zdqjudy.top

TS:   // 手写 Map<string, number>
来源：http://tpa.hnxiangtu.top

Java: // 手写 HashMap
来源：http://ibk.jyoumei.cn

Go:   // 手写 map[int]int
来源：http://rnm.sufxvd.cn

Ruby: // 手写 Hash
来源：http://ygp.yvedp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ecz.hongshengwenyu.top

[N08] 生成全排列
来源：http://fah.snrcjt.cn

Py:   itertools.permutations(arr)
来源：http://blf.yueranfly.top

PHP:  // 手写递归交换
来源：http://lvm.hywenlv.cn

JS:   // 手写回溯递归
来源：http://dak.sxryk.cn

TS:   // 手写回溯递归
来源：http://vhq.sxryk.cn

Java: // 手写回溯递归
来源：http://ktp.yj20258888.top

Go:   // 手写回溯递归
来源：http://hto.cheryme.top

Ruby: arr.permutation.to_a
来源：http://jge.xziqi.cn

C#:   // 手写回溯递归
来源：http://ant.zhengqikj.top

[N09] 栈与队列
来源：http://gxg.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qkc.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jaz.mhx1999.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://seh.zhongyouzk.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vqp.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ipp.xinyue.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zgh.daxiang520.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ppt.daxiang520.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yok.hysaishi.cn

[N10] 链表节点定义
来源：http://fhy.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vvq.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://iex.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iar.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pls.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://vys.feifeiyinyue.top

Go:   type Node struct { V int; Next *Node }
来源：http://xdm.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uks.ppjwa.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gef.aizwys.cn

[N11] 二叉树中序遍历
来源：http://equ.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gjy.tianlin.xyz

PHP:  // 手写递归函数
来源：http://spm.zhaomingkeji.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kcd.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mla.andypj.xyz

Java: // 手写递归
来源：http://zgk.fanxiaobao.xyz

Go:   // 手写递归
来源：http://hgn.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kyw.aibaodan.cn

C#:   // 手写递归
来源：http://inv.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kuw.fengsongda.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oyw.andypj.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rct.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hbh.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yqc.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ogj.haohaochexian.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ttg.jyoumei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ubo.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lbh.zhongyouzk.top

================================================================================
来源：http://oor.fzhhl.top

O. 并发与异步
来源：http://usb.hnqzz.top

================================================================================
来源：http://jzr.dashuyun.cn

[O01] 启动一个线程
来源：http://ipt.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://res.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nas.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mxj.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://zod.tianlin.xyz

Java: new Thread(() -> f()).start()
来源：http://fvr.jqgfzy.top

Go:   go f()
来源：http://avp.nanxinkj.top

Ruby: Thread.new { f }
来源：http://umk.kuanghao11.cn

C#:   Task.Run(() => F());
来源：http://isv.andypj.xyz

[O02] 使用线程池
来源：http://lif.wangshuangyany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dpw.uphjek.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nuc.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://gkp.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://oqz.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jlt.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wro.yj202588.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xzs.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vhl.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://rjy.aibaodan.cn

Py:   with lock: shared += 1
来源：http://csp.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://zsf.zhaomingkeji.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xue.zhoulong.xyz

TS:   // 同 JS
来源：http://lbq.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://rjd.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://egd.yonumen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tbu.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://igq.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://ail.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://clm.redwolf501.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ocx.gaohongyu789.top

JS:   async function f() { await g(); }
来源：http://txc.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gdy.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bpl.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ajt.sxryk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zgu.fzhhl.top

C#:   async Task F() { await G(); }
来源：http://xts.yj20258.top

[O05] 并发执行并等待全部完成
来源：http://tjl.cdnleiting.top

Py:   asyncio.gather(*tasks)
来源：http://fhb.gotoacloud.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ayq.tianlin.xyz

JS:   await Promise.all(tasks)
来源：http://myq.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://ehe.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://irf.yvedp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gmh.bbcook.cn

Ruby: threads.map(&:join)
来源：http://yxo.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://eyu.hongshengwenyu.top

[O06] 使用进程池
来源：http://mwl.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sps.ybcxt.top

PHP:  // pcntl_fork 或多进程队列
来源：http://szl.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://ure.pycfn.com

TS:   // child_process / cluster 模块
来源：http://uku.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xel.ehwqpu.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vlz.jqgfzy.top

Ruby: // fork 块
来源：http://pdq.tianlin.xyz

C#:   Parallel.For
来源：http://wmq.sufxvd.cn

================================================================================
来源：http://wey.nwbrower.top

P. 常用工具函数
来源：http://upz.snrcjt.cn

================================================================================
来源：http://ynm.gotoacloud.top

[P01] 生成 UUID
来源：http://phd.0kj1m.cn

Py:   str(uuid.uuid4())
来源：http://bdz.epnwcf.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vlp.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://fpo.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://bpa.chenzaomai.com

Java: UUID.randomUUID().toString()
来源：http://hbx.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://ils.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://xrf.shuidangran.top

C#:   Guid.NewGuid().ToString()
来源：http://epo.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://kqz.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://toi.dianchejie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pzn.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://stm.ivvv.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gea.bbcook.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zbd.jiagoushi.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cyr.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uqv.gotoacloud.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kqx.chenjidiqi.icu

[P03] 生成短随机字符串
来源：http://ezy.yvedp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://isz.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mpl.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gvn.xuetiantiany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nkg.cheryme.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ylr.jlsjyb.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wxl.fanxiaobao.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://yru.ctjpmb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sgx.daxiang520.top

[P04] 求长度
来源：http://roh.9152youxi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zqk.jinghuilouyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://osj.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hco.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nnl.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://pky.gzhubu.top

Go:   len(arr);  len(m)
来源：http://duc.xylfe.cn

Ruby: x.length;  x.size
来源：http://jmr.uphjek.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://hbw.tian-w.cn

[P05] 判断两个对象内容是否相等
来源：http://sbf.shuidangran.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://aja.shzxlz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kyo.guowangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mxt.yj20258.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xca.hywenlv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mem.yangfankeji.com

Go:   reflect.DeepEqual(a, b)
来源：http://xss.birdmap.top

Ruby: a == b
来源：http://abr.cheryme.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mur.havefunace.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ywv.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zud.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://hqy.zhongyouzk.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ham.xziqi.cn

TS:   if (x == null) {}
来源：http://tnt.0kj1m.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vxe.daxiang520.top

Go:   if x == nil {}
来源：http://ghq.ybcxt.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kxn.zdqjudy.top

C#:   if (x is null) {}
来源：http://syu.zhaomingkeji.xyz

[P07] 防抖与节流
来源：http://njs.yueranfly.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ldg.hysaishi.cn

PHP:  // 手写时间戳比较
来源：http://kla.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hli.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kpu.birdmap.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pgi.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dea.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gfu.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ckj.jinyuanbaomall.cn

[P08] 处理浮点精度问题
来源：http://iqu.yj20258.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ddo.sweek.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qnd.zhixingplan.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mgv.jyoumei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qxd.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xpb.shanyushiyangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ibi.zdbjq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ebc.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://brg.0kj1m.cn

================================================================================
来源：http://yhy.hesvh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cxa.pycfn.com

================================================================================
来源：http://fji.vqdsnc.cn

[Q01] 创建表
来源：http://pbm.yongpay.top

CREATE TABLE users (
来源：http://gnn.hesvh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://etk.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://wim.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://ept.ppjwa.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ukh.ctjpmb.com

);
来源：http://ouu.cashguo.top

[Q02] 创建带外键的表
来源：http://fod.sjlbkw.cn

CREATE TABLE orders (
来源：http://eyc.ivvv.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://svx.aizwys.cn

user_id INT NOT NULL,
来源：http://cwf.fengsongda.top

amount DECIMAL(10, 2),
来源：http://cds.feifeiyinyue.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://upr.haohaochexian.top

);
来源：http://wqn.aizwys.cn

[Q03] 增加列
来源：http://hjy.hongshengwenyu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hdd.vqdsnc.cn

[Q04] 修改列类型
来源：http://kku.iojbl.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kkj.birdmap.top

[Q05] 重命名列
来源：http://umi.redwolf501.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nmi.hywenlv.cn

[Q06] 删除列
来源：http://ziw.c1oappe.top

ALTER TABLE users DROP COLUMN age;
来源：http://veq.nwbrower.top

[Q07] 删除表
来源：http://bjs.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://zdw.daxiang520.top

[Q08] 创建普通索引
来源：http://vrj.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tag.bjfxy.top

[Q09] 创建唯一索引
来源：http://hpr.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vvl.jinqigfzy.top

[Q10] 插入单行
来源：http://ptl.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ijc.gotoacloud.top

[Q11] 一次插入多行
来源：http://kuh.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rci.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://nun.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://enp.sweek.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://apn.zdqjudy.top

[Q13] 忽略重复插入
来源：http://jnv.quarkkingdee.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cbd.yueranfly.top

[Q14] 存在则更新（upsert）
来源：http://hnu.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nuu.xingfuxueyuan.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cmw.gaohongyu789.top

[Q15] 查询全部
来源：http://rmp.jinqigfzy.top

SELECT * FROM users;
来源：http://iar.svipenyu.cn

[Q16] 查询指定列
来源：http://myu.xziqi.cn

SELECT id, name FROM users;
来源：http://hbs.bbcook.cn

[Q17] 条件查询
来源：http://dzn.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jac.ydjk.org.cn

[Q18] 模糊匹配
来源：http://kzu.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lav.c1oappe.top

[Q19] 范围查询
来源：http://jmp.shzxlz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jbn.hnxiangtu.top

[Q20] IN 列表
来源：http://opz.52xcode.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dms.xziqi.cn

[Q21] 空值判断
来源：http://keq.vehdjk.com

SELECT * FROM users WHERE email IS NULL;
来源：http://apl.zhongyouzk.top

[Q22] 排序
来源：http://gte.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bca.xziqi.cn

[Q23] 分页
来源：http://olb.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cvt.dashuyun.cn

[Q24] 去重
来源：http://mhq.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://bcx.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://epx.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jok.ctjpmb.com

[Q26] 计数
来源：http://ajd.zdqjudy.top

SELECT COUNT(*) FROM users;
来源：http://urn.uphjek.com

[Q27] 条件计数
来源：http://fga.yuxming.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kmo.uphjek.com

[Q28] 求和与平均
来源：http://lek.zdbjq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aab.redwolf501.top

[Q29] 最大最小值
来源：http://upp.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vra.xuetiantiany.cn

[Q30] 分组统计
来源：http://mrl.zhengqikj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eth.yfazqb.com

[Q31] 分组后过滤
来源：http://opg.iojbl.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oan.yj20258888.top

[Q32] 分组拼接字符串
来源：http://tnb.hcnkem.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sha.shzxlz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ogk.gzhubu.top

[Q33] 多列分组
来源：http://tsv.cheryme.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gly.chenzaomai.com

[Q34] 每组取第一条
来源：http://unl.ydzc1.top

SELECT * FROM (
来源：http://vmv.hysaishi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nxi.zhijiandao.cn

) t WHERE rn = 1;
来源：http://pjo.0kj1m.cn

[Q35] 内连接
来源：http://hpn.feifeiyinyue.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hgq.quarkkingdee.top

[Q36] 左连接
来源：http://ekr.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pys.yvedp.cn

[Q37] 右连接
来源：http://bgx.zhoulong.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iny.hcnkem.com

[Q38] 全外连接（PostgreSQL）
来源：http://fvi.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://icj.nanxuanxn.top

[Q39] 自连接（查上下级）
来源：http://exu.316326.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://wpw.wangshuangyany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wrd.bbcook.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://paf.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tnn.yj202588.top

[Q41] 多表连接
来源：http://gpp.chenzaomai.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://qun.jqgfzy.top

JOIN users u ON u.id = o.user_id
来源：http://xto.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://dps.meibo888.top

[Q42] 连接条件附加过滤
来源：http://iqv.svipenyu.cn

SELECT u.name, o.amount FROM users u
来源：http://esd.aibaodan.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://srd.mhx1999.top

[Q43] 标量子查询
来源：http://szg.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fec.redwolf501.top


<!-- 参考信息 -->