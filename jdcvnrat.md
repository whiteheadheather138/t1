代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://cjg.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://cpl.yj202588.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eil.ivvv.top

Go:   // 双指针从两端比较
来源：http://tgj.jqgfzy.top

Ruby: s == s.reverse
来源：http://pba.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mvm.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://bcu.pycfn.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lfx.zhixingplan.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kot.hywenlv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oir.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://byd.smart0.xyz

Java: // 手写 HashMap
来源：http://gtu.shuidangran.top

Go:   // 手写 map[int]int
来源：http://dqq.xuanzx.com

Ruby: // 手写 Hash
来源：http://htg.yuanzhike.top

C#:   // 手写 Dictionary<int, int>
来源：http://azq.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://nyy.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://uem.ybcxt.top

PHP:  // 手写递归交换
来源：http://xzr.guannengcc.top

JS:   // 手写回溯递归
来源：http://blf.tian-w.cn

TS:   // 手写回溯递归
来源：http://nez.mhx1999.top

Java: // 手写回溯递归
来源：http://gvj.sufxvd.cn

Go:   // 手写回溯递归
来源：http://tsf.ywan-chungtsiang.top

Ruby: arr.permutation.to_a
来源：http://bki.yj20258.top

C#:   // 手写回溯递归
来源：http://zyz.birdmap.top

[N09] 栈与队列
来源：http://vff.sxryk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iom.snrcjt.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://aks.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dnd.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xbi.iojbl.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fir.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://odq.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fep.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rem.cheryme.top

[N10] 链表节点定义
来源：http://hah.gogol.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wtd.gaohongyu789.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gfi.ydjk.org.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qmq.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ijl.jinqigufen.top

Java: class Node { int v; Node next; }
来源：http://iwf.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://nly.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uab.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zrh.smart0.xyz

[N11] 二叉树中序遍历
来源：http://kcz.quarkkingdee.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xpq.ydzc1.top

PHP:  // 手写递归函数
来源：http://inf.vqdsnc.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://teh.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uui.ppjwa.cn

Java: // 手写递归
来源：http://znr.snrcjt.cn

Go:   // 手写递归
来源：http://ipn.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://har.shangyingyoupin.top

C#:   // 手写递归
来源：http://zbh.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vuu.52xcode.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bfw.sweek.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kfs.fktsv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kow.fanxiaobao.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zxj.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tbs.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://csl.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ykd.hammf.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zei.yfazqb.com

================================================================================
来源：http://hgw.ehwqpu.com

O. 并发与异步
来源：http://hpr.bbcook.cn

================================================================================
来源：http://utt.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://dxm.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kez.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://phe.gotoacloud.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kts.kuanghao11.cn

TS:   // 同 JS
来源：http://iga.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://arl.yuanzhike.top

Go:   go f()
来源：http://hjn.0kj1m.cn

Ruby: Thread.new { f }
来源：http://zvx.fzhhl.top

C#:   Task.Run(() => F());
来源：http://sad.316326.xyz

[O02] 使用线程池
来源：http://cvg.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tqx.pengpengdd.cyou

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nlg.fktsv.cn

JS:   // worker_threads 线程池
来源：http://hsa.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://eml.andypj.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://dxe.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xcj.zhongyouzk.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://knc.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tlj.cheryme.top

[O03] 加锁保护共享数据
来源：http://yrz.fengsongda.top

Py:   with lock: shared += 1
来源：http://sds.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://nvp.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gvf.zhoulong.xyz

TS:   // 同 JS
来源：http://lrl.yuxming.cn

Java: synchronized (this) { shared++; }
来源：http://nkf.ctjpmb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cds.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rzj.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://gsq.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://xyz.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://oqw.feifeiyinyue.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bne.shuidangran.top

JS:   async function f() { await g(); }
来源：http://qrf.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://elf.haohaochexian.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vyf.hywenlv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qqe.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bez.aizwys.cn

C#:   async Task F() { await G(); }
来源：http://udk.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://wjl.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://ybs.jinyuanbaomall.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rda.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://nux.yj202588.top

TS:   await Promise.all(tasks)
来源：http://bzk.jiagoushi.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bzw.zhaomingkeji.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vjr.guowangkeji.top

Ruby: threads.map(&:join)
来源：http://qvx.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kzq.xylfe.cn

[O06] 使用进程池
来源：http://bmz.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://juh.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://iuu.smart0.xyz

JS:   // child_process / cluster 模块
来源：http://jtc.yangfankeji.com

TS:   // child_process / cluster 模块
来源：http://cmc.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xyy.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tba.cqqwz.cn

Ruby: // fork 块
来源：http://htg.yanxiufei.cn

C#:   Parallel.For
来源：http://smm.zhengqikj.top

================================================================================
来源：http://uwr.wangdashe.top

P. 常用工具函数
来源：http://gsi.bjfxy.top

================================================================================
来源：http://xyh.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://rhm.cheryme.top

Py:   str(uuid.uuid4())
来源：http://qtd.jinghuilouyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://prd.xuanzx.com

JS:   crypto.randomUUID()
来源：http://nah.yueranfly.top

TS:   crypto.randomUUID()
来源：http://stp.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://ugu.zhoulong.xyz

Go:   // 用 github.com/google/uuid
来源：http://jux.52xcode.cn

Ruby: SecureRandom.uuid
来源：http://jez.zycfv.cn

C#:   Guid.NewGuid().ToString()
来源：http://ofq.yongpay.top

[P02] MD5 / SHA256 摘要
来源：http://nkr.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ekg.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ope.haohaochexian.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ppu.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ehk.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fsj.hywenlv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://akh.zhongyouzk.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gxx.52xcode.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eof.redwolf501.top

[P03] 生成短随机字符串
来源：http://jpv.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kxc.havefunace.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gcv.havefunace.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jfx.zhixingplan.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vda.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vdu.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://quv.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jyr.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vxb.xylfe.cn

[P04] 求长度
来源：http://omp.tian-w.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bkq.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mzn.dianchejie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bbm.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xyh.daria6918.cn

Java: list.size();  map.size();  s.length()
来源：http://rbq.hammf.cn

Go:   len(arr);  len(m)
来源：http://itz.feifeiyinyue.top

Ruby: x.length;  x.size
来源：http://cme.hongshengwenyu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://umz.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://tbr.yj20258888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://umx.nanxinkj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lyw.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vlp.quarkkingdee.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://klj.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jrg.dashuyun.cn

Go:   reflect.DeepEqual(a, b)
来源：http://csn.jqgufenzy.top

Ruby: a == b
来源：http://emy.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tug.gzhubu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uno.svipenyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gfc.meibo888.top

PHP:  if (empty($x)) {}
来源：http://iom.cashguo.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sus.aibaodan.cn

TS:   if (x == null) {}
来源：http://qdu.yj20258.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qwr.ydzc1.top

Go:   if x == nil {}
来源：http://tee.iojbl.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ebj.hnxiangtu.top

C#:   if (x is null) {}
来源：http://nrm.pycfn.com

[P07] 防抖与节流
来源：http://xkr.wangshuangyany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://azm.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://tvp.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hgp.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wpm.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rzp.mhx1999.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rmy.ctjpmb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://zme.dianchejie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yoq.jqgfzy.top

[P08] 处理浮点精度问题
来源：http://sdb.tianlin.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tcn.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cjz.daria6918.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hzr.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ghn.meibo888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tyc.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pci.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://umk.zhijiandao.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gjf.jinqigufen.top

================================================================================
来源：http://lmz.xingfuxueyuan.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tba.fengsongda.top

================================================================================
来源：http://aax.meibo888.top

[Q01] 创建表
来源：http://jea.yongpay.top

CREATE TABLE users (
来源：http://aej.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kji.chenlongwang.top

name VARCHAR(50) NOT NULL,
来源：http://diu.hongshengwenyu.top

email VARCHAR(100) UNIQUE,
来源：http://szj.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hlv.mhx1999.top

);
来源：http://aei.ybcxt.top

[Q02] 创建带外键的表
来源：http://qvm.svipenyu.cn

CREATE TABLE orders (
来源：http://phv.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sjq.mhx1999.top

user_id INT NOT NULL,
来源：http://scu.9152youxi.cn

amount DECIMAL(10, 2),
来源：http://iki.pycfn.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kbf.zhiwuduotai.top

);
来源：http://jpy.jinghuilouyu.cn

[Q03] 增加列
来源：http://yxb.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://krl.fehbvm.com

[Q04] 修改列类型
来源：http://rwv.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tdn.yuanzhike.top

[Q05] 重命名列
来源：http://pmk.shanyushiyangtech.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uul.zhengqikj.top

[Q06] 删除列
来源：http://jcp.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://oom.gogol.net.cn

[Q07] 删除表
来源：http://saq.shangyingyoupin.top

DROP TABLE IF EXISTS orders;
来源：http://eqo.bbcook.cn

[Q08] 创建普通索引
来源：http://vkh.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xaz.ywan-chungtsiang.top

[Q09] 创建唯一索引
来源：http://icj.yangfankeji.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pke.smart0.xyz

[Q10] 插入单行
来源：http://gmv.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dxy.zdbjq.cn

[Q11] 一次插入多行
来源：http://ruq.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qyw.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://swo.52xcode.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ixh.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yaw.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://pnf.xziqi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://czn.redwolf501.top

[Q14] 存在则更新（upsert）
来源：http://skh.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ows.hesvh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jet.dashuyun.cn

[Q15] 查询全部
来源：http://ozg.vqdsnc.cn

SELECT * FROM users;
来源：http://suu.pengpengdd.cyou

[Q16] 查询指定列
来源：http://bsx.ydzc1.top

SELECT id, name FROM users;
来源：http://gmp.chenzaomai.com

[Q17] 条件查询
来源：http://ycn.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://csk.chenlongwang.top

[Q18] 模糊匹配
来源：http://xlf.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pnh.cheryme.top

[Q19] 范围查询
来源：http://ldh.hnxiangtu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jax.hesvh.cn

[Q20] IN 列表
来源：http://sbg.zycfv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jkk.jinqigufen.top

[Q21] 空值判断
来源：http://mgw.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jvm.aibaodan.cn

[Q22] 排序
来源：http://jav.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yct.zhixingplan.top

[Q23] 分页
来源：http://wsg.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hvi.andypj.xyz

[Q24] 去重
来源：http://kvt.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://rir.sweek.top

[Q25] 只取前 N 条
来源：http://daq.dianchejie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blb.fehbvm.com

[Q26] 计数
来源：http://cmz.yangfankeji.com

SELECT COUNT(*) FROM users;
来源：http://kxn.kuanghao11.cn

[Q27] 条件计数
来源：http://rks.gotoacloud.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qev.yongpay.top

[Q28] 求和与平均
来源：http://ekp.ivvv.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tgw.yonumen.top

[Q29] 最大最小值
来源：http://pjo.xziqi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zaj.iojbl.cn

[Q30] 分组统计
来源：http://fjx.wangdashe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ctw.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://rbh.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nqt.zhixingplan.top

[Q32] 分组拼接字符串
来源：http://fui.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://unt.birdmap.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://huj.nanxinkj.top

[Q33] 多列分组
来源：http://ghm.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://azy.jinghuilouyu.cn

[Q34] 每组取第一条
来源：http://kcq.chenlongwang.top

SELECT * FROM (
来源：http://siz.haohaochexian.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bgm.gaohongyu789.top

) t WHERE rn = 1;
来源：http://cjw.jinqigfzy.top

[Q35] 内连接
来源：http://hbx.fehbvm.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vkw.gogol.net.cn

[Q36] 左连接
来源：http://qpx.fengsongda.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rwi.sufxvd.cn

[Q37] 右连接
来源：http://ayo.cashguo.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vbp.shanyushiyangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://mkm.yuxming.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://alc.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://vqm.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bwn.sjlbkw.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mrc.iojbl.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://puq.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jgm.cashguo.top

[Q41] 多表连接
来源：http://bhs.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dpc.meibo888.top

JOIN users u ON u.id = o.user_id
来源：http://txt.hysaishi.cn

JOIN products p ON p.id = o.product_id;
来源：http://twu.redwolf501.top

[Q42] 连接条件附加过滤
来源：http://gjv.cdnleiting.top

SELECT u.name, o.amount FROM users u
来源：http://rvf.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qyt.gogol.net.cn

[Q43] 标量子查询
来源：http://hsb.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jnj.dianchejie.cn


<!-- 参考信息 -->