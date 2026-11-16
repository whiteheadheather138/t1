代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://zhl.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://ufq.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jnk.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://ztn.fehbvm.com

Ruby: s == s.reverse
来源：http://mdl.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fgo.sufxvd.cn

[N07] 两数之和（返回下标）
来源：http://zfs.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://frs.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cef.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kat.xinyue.icu

TS:   // 手写 Map<string, number>
来源：http://nrq.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://mqf.yueranfly.top

Go:   // 手写 map[int]int
来源：http://fcb.tarul.cn

Ruby: // 手写 Hash
来源：http://mkr.ywan-chungtsiang.top

C#:   // 手写 Dictionary<int, int>
来源：http://dnr.jyoumei.cn

[N08] 生成全排列
来源：http://hyw.redwolf501.top

Py:   itertools.permutations(arr)
来源：http://nwv.ywan-chungtsiang.top

PHP:  // 手写递归交换
来源：http://mze.c1oappe.top

JS:   // 手写回溯递归
来源：http://bmo.shzxlz.cn

TS:   // 手写回溯递归
来源：http://wca.vqdsnc.cn

Java: // 手写回溯递归
来源：http://ilm.ivvv.top

Go:   // 手写回溯递归
来源：http://yta.52xcode.cn

Ruby: arr.permutation.to_a
来源：http://xsv.dianchejie.cn

C#:   // 手写回溯递归
来源：http://nkg.svipenyu.cn

[N09] 栈与队列
来源：http://iqg.zhongyouzk.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lzs.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lzh.meibo888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wdc.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://omc.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rol.nwbrower.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lcy.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://svk.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ana.sjlbkw.cn

[N10] 链表节点定义
来源：http://wim.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uso.yj202588.top

PHP:  class Node { public $v; public $next = null; }
来源：http://suo.yvedp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zfg.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qeb.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://tyc.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://kzm.xinyue.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://dom.vehdjk.com

C#:   class Node { public int V; public Node? Next; }
来源：http://cpt.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://qzs.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cjm.shuidangran.top

PHP:  // 手写递归函数
来源：http://lpq.9152youxi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nil.dashuyun.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qwa.sjlbkw.cn

Java: // 手写递归
来源：http://xay.dianchejie.cn

Go:   // 手写递归
来源：http://lpx.xuanzx.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kcf.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://lii.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cjb.daria6918.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hov.fzhhl.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ygh.uphjek.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yjc.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xzi.yuanzhike.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://myk.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fhf.gzhubu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ssv.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wmh.feifeiyinyue.top

================================================================================
来源：http://ikg.tanke756.top

O. 并发与异步
来源：http://ljt.yonumen.top

================================================================================
来源：http://zkw.feifeiyinyue.top

[O01] 启动一个线程
来源：http://nqm.nanxinkj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bkr.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lzg.fehbvm.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ctd.jqgufenzy.top

TS:   // 同 JS
来源：http://rud.zhijiandao.cn

Java: new Thread(() -> f()).start()
来源：http://fvn.zhengqikj.top

Go:   go f()
来源：http://mha.nanxuanxn.top

Ruby: Thread.new { f }
来源：http://ymj.316326.xyz

C#:   Task.Run(() => F());
来源：http://jfg.ivvv.top

[O02] 使用线程池
来源：http://ywh.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yvx.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ofo.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://nvh.yuxming.cn

TS:   // worker_threads 线程池
来源：http://moe.feifeiyinyue.top

Java: Executors.newFixedThreadPool(4)
来源：http://uhu.ybcxt.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wtu.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zlt.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kmx.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://tku.yfazqb.com

Py:   with lock: shared += 1
来源：http://pup.ydjk.org.cn

PHP:  // 用 flock() 做文件锁
来源：http://wsk.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gjj.tianlin.xyz

TS:   // 同 JS
来源：http://ofc.9152youxi.cn

Java: synchronized (this) { shared++; }
来源：http://mnf.c1oappe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bbz.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cgj.ydzc1.top

C#:   lock (gate) { shared++; }
来源：http://adq.gogol.net.cn

[O04] 定义异步函数并等待
来源：http://ljj.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://hva.svipenyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ngz.yonumen.top

JS:   async function f() { await g(); }
来源：http://dbx.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lby.tanke756.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ayv.52xcode.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://elr.jinyuanbaomall.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rcx.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://vjk.fktsv.cn

[O05] 并发执行并等待全部完成
来源：http://cbq.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://jyz.cashguo.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vvu.zycfv.cn

JS:   await Promise.all(tasks)
来源：http://the.shanyushiyangkeji.top

TS:   await Promise.all(tasks)
来源：http://ekg.yj20258.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xtf.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://shg.daxiang520.top

Ruby: threads.map(&:join)
来源：http://qwm.ctjpmb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://chx.fktsv.cn

[O06] 使用进程池
来源：http://nwt.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nnr.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://hny.316326.xyz

JS:   // child_process / cluster 模块
来源：http://gqj.hfpthk.cn

TS:   // child_process / cluster 模块
来源：http://rxu.xinyue.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pfp.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://foz.shanyushiyangtech.top

Ruby: // fork 块
来源：http://akm.sxryk.cn

C#:   Parallel.For
来源：http://epn.vehdjk.com

================================================================================
来源：http://xhx.zdbjq.cn

P. 常用工具函数
来源：http://qhn.daxiang520.top

================================================================================
来源：http://hch.sxryk.cn

[P01] 生成 UUID
来源：http://uhk.jianghu66.top

Py:   str(uuid.uuid4())
来源：http://pgr.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sdq.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://gjw.jianghu66.top

TS:   crypto.randomUUID()
来源：http://xdy.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://sqf.yvedp.cn

Go:   // 用 github.com/google/uuid
来源：http://plq.jianghu66.top

Ruby: SecureRandom.uuid
来源：http://oxm.yj202588.top

C#:   Guid.NewGuid().ToString()
来源：http://vlu.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://wwp.xinyue.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lai.0kj1m.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pct.zhaomingkeji.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fhq.redwolf501.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wek.shanyushiyangtech.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zuq.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://abd.tian-w.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wgn.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kxy.wangshuangyany.cn

[P03] 生成短随机字符串
来源：http://hsx.vehdjk.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yhq.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://udq.ybcxt.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pwj.fktsv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rjc.ywan-chungtsiang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gfg.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mnc.hesvh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xnr.ydzc1.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gwl.shanyushiyangkeji.top

[P04] 求长度
来源：http://adi.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fwm.shangyingyoupin.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ybs.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vrd.yj202588.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hjf.hfpthk.cn

Java: list.size();  map.size();  s.length()
来源：http://zhp.uphjek.com

Go:   len(arr);  len(m)
来源：http://oqw.yj20258.top

Ruby: x.length;  x.size
来源：http://vom.pycfn.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://lyc.shangyingyoupin.top

[P05] 判断两个对象内容是否相等
来源：http://jmr.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yik.yfazqb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hfo.ehwqpu.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ynm.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://trd.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rry.zdqjudy.top

Go:   reflect.DeepEqual(a, b)
来源：http://uds.shanyushiyangtech.top

Ruby: a == b
来源：http://iap.0kj1m.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://equ.0kj1m.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://myq.xuanzx.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yoc.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://ngt.smart0.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blm.nanxinkj.top

TS:   if (x == null) {}
来源：http://cpz.nwbrower.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ahb.sxryk.cn

Go:   if x == nil {}
来源：http://lax.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ncs.xuanzx.com

C#:   if (x is null) {}
来源：http://obc.yueranfly.top

[P07] 防抖与节流
来源：http://uqa.hesvh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fbs.xziqi.cn

PHP:  // 手写时间戳比较
来源：http://jxg.bjfxy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://akp.nanxinkj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bii.aibaodan.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://scn.zycfv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xtp.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://lsd.haohaochexian.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lkp.hcnkem.com

[P08] 处理浮点精度问题
来源：http://snb.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eso.c1oappe.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ymo.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bor.hywenlv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cqd.hfpthk.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yik.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nto.chenjidiqi.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xjo.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iiv.nanxinkj.top

================================================================================
来源：http://jpp.yangfankeji.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ruk.zhoulong.xyz

================================================================================
来源：http://bie.bjfxy.top

[Q01] 创建表
来源：http://png.havefunace.top

CREATE TABLE users (
来源：http://jum.chenjidiqi.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cjw.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://kfe.feifeiyinyue.top

email VARCHAR(100) UNIQUE,
来源：http://cyi.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zvl.haohaochexian.top

);
来源：http://ruz.zdbjq.cn

[Q02] 创建带外键的表
来源：http://oeq.yvedp.cn

CREATE TABLE orders (
来源：http://aja.hongshengwenyu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yee.shzxlz.cn

user_id INT NOT NULL,
来源：http://wss.fanxiaobao.xyz

amount DECIMAL(10, 2),
来源：http://zfo.c1oappe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mdk.tianlin.xyz

);
来源：http://bft.yonumen.top

[Q03] 增加列
来源：http://mye.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bzx.wangshuangyany.cn

[Q04] 修改列类型
来源：http://fxy.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kbp.yj20258.top

[Q05] 重命名列
来源：http://lzf.feifeiyinyue.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yur.smart0.xyz

[Q06] 删除列
来源：http://zxv.nanxinkj.top

ALTER TABLE users DROP COLUMN age;
来源：http://kzk.birdmap.top

[Q07] 删除表
来源：http://rcj.zdbjq.cn

DROP TABLE IF EXISTS orders;
来源：http://ejx.hammf.cn

[Q08] 创建普通索引
来源：http://bue.shzxlz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bsf.cucudq.cn

[Q09] 创建唯一索引
来源：http://uxk.yanxiufei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mmd.zdqjudy.top

[Q10] 插入单行
来源：http://woh.cheryme.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://crl.zhaomingkeji.xyz

[Q11] 一次插入多行
来源：http://rnn.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yqh.daxiang520.top

[Q12] 插入后取自增 ID
来源：http://ngm.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://ftq.316326.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cqq.yanxiufei.cn

[Q13] 忽略重复插入
来源：http://fnz.zhaomingkeji.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gxx.zdbjq.cn

[Q14] 存在则更新（upsert）
来源：http://szo.uphjek.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://won.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://stl.zhijiandao.cn

[Q15] 查询全部
来源：http://juh.tianlin.xyz

SELECT * FROM users;
来源：http://rde.daria6918.cn

[Q16] 查询指定列
来源：http://wjf.tian-w.cn

SELECT id, name FROM users;
来源：http://odk.gaohongyu789.top

[Q17] 条件查询
来源：http://isc.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ocp.gotoacloud.top

[Q18] 模糊匹配
来源：http://fpq.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oki.ybcxt.top

[Q19] 范围查询
来源：http://igp.zycfv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://euo.xinyue.icu

[Q20] IN 列表
来源：http://usx.cucudq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nyd.hnqzz.top

[Q21] 空值判断
来源：http://qcl.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zfl.nanxuanxn.top

[Q22] 排序
来源：http://tqq.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://foz.guowangkeji.top

[Q23] 分页
来源：http://fjl.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://utl.shanyushiyangkeji.top

[Q24] 去重
来源：http://ksr.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://yil.vehdjk.com

[Q25] 只取前 N 条
来源：http://acf.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dqt.ppjwa.cn

[Q26] 计数
来源：http://hoy.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://zzm.hfpthk.cn

[Q27] 条件计数
来源：http://zef.chenzaomai.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uur.pengpengdd.cyou

[Q28] 求和与平均
来源：http://tiz.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bhq.sysykeji.top

[Q29] 最大最小值
来源：http://gqc.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gyw.pengpengdd.cyou

[Q30] 分组统计
来源：http://ori.yangfankeji.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bub.chenzaomai.com

[Q31] 分组后过滤
来源：http://nlj.zhoulong.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://niu.shangyingyoupin.top

[Q32] 分组拼接字符串
来源：http://lms.fengsongda.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zjv.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zxk.hfpthk.cn

[Q33] 多列分组
来源：http://mlk.fktsv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://spr.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://bsf.zhijiandao.cn

SELECT * FROM (
来源：http://tpa.jyoumei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hcv.cqqwz.cn

) t WHERE rn = 1;
来源：http://anw.yangfankeji.com

[Q35] 内连接
来源：http://kdv.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://atd.gzhubu.top

[Q36] 左连接
来源：http://vtq.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ilk.zhongyouzk.top

[Q37] 右连接
来源：http://uwc.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ymy.uphjek.com

[Q38] 全外连接（PostgreSQL）
来源：http://lbb.fzhhl.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://myl.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://yvz.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qfy.hywenlv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fqy.0kj1m.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iie.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://flt.dashuyun.cn

[Q41] 多表连接
来源：http://lmc.aibaodan.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uys.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://bzx.jyoumei.cn

JOIN products p ON p.id = o.product_id;
来源：http://yjf.svipenyu.cn

[Q42] 连接条件附加过滤
来源：http://ppg.iojbl.cn

SELECT u.name, o.amount FROM users u
来源：http://ryc.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fen.zdbjq.cn

[Q43] 标量子查询
来源：http://nxz.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://joh.hywenlv.cn


<!-- 参考信息 -->