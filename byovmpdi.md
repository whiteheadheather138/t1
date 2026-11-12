代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qba.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fjp.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ywg.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://ctw.jianghu66.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dlx.gzhubu.top

[N06] 判断回文字符串
来源：http://ghz.haohaochexian.top

Py:   s == s[::-1]
来源：http://joh.haohaochexian.top

PHP:  $s === strrev($s);
来源：http://ffg.fanxiaobao.xyz

JS:   s === [...s].reverse().join("")
来源：http://tfr.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://pah.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iqo.zycfv.cn

Go:   // 双指针从两端比较
来源：http://qxg.tianlin.xyz

Ruby: s == s.reverse
来源：http://fux.jqgfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dro.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://cbk.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hzn.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://siv.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pmw.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://rbb.smart0.xyz

Java: // 手写 HashMap
来源：http://xdf.jlsjyb.cn

Go:   // 手写 map[int]int
来源：http://glj.tian-w.cn

Ruby: // 手写 Hash
来源：http://ytn.yanxiufei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tin.0kj1m.cn

[N08] 生成全排列
来源：http://rfi.zhixingplan.top

Py:   itertools.permutations(arr)
来源：http://pkr.yonumen.top

PHP:  // 手写递归交换
来源：http://wmy.kuanghao11.cn

JS:   // 手写回溯递归
来源：http://qtk.sysykeji.top

TS:   // 手写回溯递归
来源：http://lem.feifeiyinyue.top

Java: // 手写回溯递归
来源：http://ejk.redwolf501.top

Go:   // 手写回溯递归
来源：http://dhy.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://kzb.jianghu66.top

C#:   // 手写回溯递归
来源：http://fur.feifeiyinyue.top

[N09] 栈与队列
来源：http://jfd.jinqigufen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wuw.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xnc.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rkd.jqgfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gos.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vse.zhaomingkeji.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://czp.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bur.ivvv.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aac.fengsongda.top

[N10] 链表节点定义
来源：http://fyo.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qyz.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://igl.yuxming.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fog.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hot.quarkkingdee.top

Java: class Node { int v; Node next; }
来源：http://syt.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://trd.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xju.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hxy.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://ugb.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xmc.mhx1999.top

PHP:  // 手写递归函数
来源：http://koi.tianlin.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tvl.zhaomingkeji.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gji.nanxuanxn.top

Java: // 手写递归
来源：http://nqh.chenjidiqi.icu

Go:   // 手写递归
来源：http://wfj.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://znv.tarul.cn

C#:   // 手写递归
来源：http://tij.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vso.chenzaomai.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gvr.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qyw.jinghuilouyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tko.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aca.pengpengdd.cyou

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iel.hnqzz.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wuc.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ixi.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rri.birdmap.top

================================================================================
来源：http://tjz.yongpay.top

O. 并发与异步
来源：http://ydy.tarul.cn

================================================================================
来源：http://sep.316326.xyz

[O01] 启动一个线程
来源：http://xue.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rba.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bvh.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mtk.xuetiantiany.cn

TS:   // 同 JS
来源：http://fiq.dianchejie.cn

Java: new Thread(() -> f()).start()
来源：http://sgi.mhx1999.top

Go:   go f()
来源：http://ryx.ctjpmb.com

Ruby: Thread.new { f }
来源：http://jrb.yangfankeji.com

C#:   Task.Run(() => F());
来源：http://prv.jinqigfzy.top

[O02] 使用线程池
来源：http://fkd.haohaochexian.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rlk.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zkm.sweek.top

JS:   // worker_threads 线程池
来源：http://iwf.ivvv.top

TS:   // worker_threads 线程池
来源：http://hqe.316326.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://bqu.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pgk.ywan-chungtsiang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ecb.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://git.gaohongyu789.top

[O03] 加锁保护共享数据
来源：http://cad.yfazqb.com

Py:   with lock: shared += 1
来源：http://koe.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://nmy.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uej.jinqigfzy.top

TS:   // 同 JS
来源：http://olo.aibaodan.cn

Java: synchronized (this) { shared++; }
来源：http://wva.havefunace.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lmh.c1oappe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jaq.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://uha.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://emi.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://oas.0kj1m.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dry.gogol.net.cn

JS:   async function f() { await g(); }
来源：http://uhe.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://uci.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hyu.cqqwz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zrn.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://uxh.birdmap.top

C#:   async Task F() { await G(); }
来源：http://lzs.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://kxo.gogol.net.cn

Py:   asyncio.gather(*tasks)
来源：http://mvo.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zav.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://sbz.havefunace.top

TS:   await Promise.all(tasks)
来源：http://vjj.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xqv.xziqi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lqa.hfpthk.cn

Ruby: threads.map(&:join)
来源：http://tuj.daria6918.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://phv.hfpthk.cn

[O06] 使用进程池
来源：http://lmz.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kvp.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zqd.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://fbf.kuanghao11.cn

TS:   // child_process / cluster 模块
来源：http://ybr.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mxo.zhoulong.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ogw.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://txc.cdnleiting.top

C#:   Parallel.For
来源：http://uya.birdmap.top

================================================================================
来源：http://vlp.chenzaomai.com

P. 常用工具函数
来源：http://ohq.fehbvm.com

================================================================================
来源：http://xvq.9152youxi.cn

[P01] 生成 UUID
来源：http://pme.hfpthk.cn

Py:   str(uuid.uuid4())
来源：http://onv.jinyuanbaomall.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xrl.gogol.net.cn

JS:   crypto.randomUUID()
来源：http://ldd.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://bux.quarkkingdee.top

Java: UUID.randomUUID().toString()
来源：http://rye.yangfankeji.com

Go:   // 用 github.com/google/uuid
来源：http://cqm.zhixingplan.top

Ruby: SecureRandom.uuid
来源：http://buz.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://wpy.smart0.xyz

[P02] MD5 / SHA256 摘要
来源：http://dxa.tian-w.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ips.haohaochexian.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dbv.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aqc.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pdy.meibo888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gdx.zhixingplan.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://syt.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dfb.hesvh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qwg.hammf.cn

[P03] 生成短随机字符串
来源：http://ykx.yuanzhike.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zsn.c1oappe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://chu.gaohongyu789.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ihu.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fzr.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uhs.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fzy.iojbl.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lhh.xziqi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qmh.jianghu66.top

[P04] 求长度
来源：http://piu.dianchejie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bwk.yangfankeji.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://phm.vqdsnc.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://elc.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bxm.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://zkx.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://nps.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://vup.nanxinkj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gnn.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://bco.yanxiufei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://svw.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bql.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wdi.daria6918.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bmi.sysykeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dcp.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://uaw.pengpengdd.cyou

Ruby: a == b
来源：http://wro.ctjpmb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://huk.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jeg.9152youxi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cjn.hammf.cn

PHP:  if (empty($x)) {}
来源：http://egx.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kwo.dianchejie.cn

TS:   if (x == null) {}
来源：http://wnc.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://bfi.wangdashe.top

Go:   if x == nil {}
来源：http://psm.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ikn.xziqi.cn

C#:   if (x is null) {}
来源：http://fay.cashguo.top

[P07] 防抖与节流
来源：http://pcp.quarkkingdee.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ihu.sjlbkw.cn

PHP:  // 手写时间戳比较
来源：http://gcq.ppjwa.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rzh.ybcxt.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jog.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://trn.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://izu.ehwqpu.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://rxa.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ruq.yfazqb.com

[P08] 处理浮点精度问题
来源：http://qjr.hysaishi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ric.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vqq.kuanghao11.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://olx.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dbz.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bbq.shanyushiyangtech.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oed.bjfxy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://chl.ybcxt.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hpb.vehdjk.com

================================================================================
来源：http://ikw.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://coa.mhx1999.top

================================================================================
来源：http://wol.birdmap.top

[Q01] 创建表
来源：http://vuf.guannengcc.top

CREATE TABLE users (
来源：http://fys.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dps.jqgufenzy.top

name VARCHAR(50) NOT NULL,
来源：http://yhu.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://vms.redwolf501.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jjz.jinyuanbaomall.cn

);
来源：http://jpq.ybcxt.top

[Q02] 创建带外键的表
来源：http://hwy.haohaochexian.top

CREATE TABLE orders (
来源：http://qqa.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://svw.9152youxi.cn

user_id INT NOT NULL,
来源：http://sfx.ppjwa.cn

amount DECIMAL(10, 2),
来源：http://ywf.andypj.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ric.jqgufenzy.top

);
来源：http://ulb.yj20258.top

[Q03] 增加列
来源：http://mft.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lji.bbcook.cn

[Q04] 修改列类型
来源：http://yuf.hywenlv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://avg.fengsongda.top

[Q05] 重命名列
来源：http://wco.guannengcc.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://koq.chenzaomai.com

[Q06] 删除列
来源：http://kmv.xylfe.cn

ALTER TABLE users DROP COLUMN age;
来源：http://shb.gaohongyu789.top

[Q07] 删除表
来源：http://qzh.tian-w.cn

DROP TABLE IF EXISTS orders;
来源：http://fss.zdbjq.cn

[Q08] 创建普通索引
来源：http://onx.andypj.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://fod.shuidangran.top

[Q09] 创建唯一索引
来源：http://uda.sufxvd.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nuc.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://ctq.yj20258.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rmp.jinqigufen.top

[Q11] 一次插入多行
来源：http://eco.ybcxt.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ndc.daria6918.cn

[Q12] 插入后取自增 ID
来源：http://gfj.sysykeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://uxb.xuanzx.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fpe.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://plc.zhaomingkeji.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ofe.sxryk.cn

[Q14] 存在则更新（upsert）
来源：http://rux.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iok.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vva.meibo888.top

[Q15] 查询全部
来源：http://yit.epnwcf.com

SELECT * FROM users;
来源：http://zow.daria6918.cn

[Q16] 查询指定列
来源：http://vsj.pycfn.com

SELECT id, name FROM users;
来源：http://wqx.redwolf501.top

[Q17] 条件查询
来源：http://xtv.jqgfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sui.chenlongwang.top

[Q18] 模糊匹配
来源：http://wkr.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nuv.xziqi.cn

[Q19] 范围查询
来源：http://hcc.zdbjq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://swt.ydjk.org.cn

[Q20] IN 列表
来源：http://lux.yanxiufei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ipt.hesvh.cn

[Q21] 空值判断
来源：http://biq.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fzu.wangdashe.top

[Q22] 排序
来源：http://fzr.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fdd.jyoumei.cn

[Q23] 分页
来源：http://wdi.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eii.shanyushiyangtech.top

[Q24] 去重
来源：http://urw.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://tqq.jianghu66.top

[Q25] 只取前 N 条
来源：http://wpj.gotoacloud.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tac.sjlbkw.cn

[Q26] 计数
来源：http://waw.gotoacloud.top

SELECT COUNT(*) FROM users;
来源：http://zzq.zhixingplan.top

[Q27] 条件计数
来源：http://jjg.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lkq.316326.xyz

[Q28] 求和与平均
来源：http://uix.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bkv.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://zkh.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qrz.wangshuangyany.cn

[Q30] 分组统计
来源：http://yzw.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tti.svipenyu.cn

[Q31] 分组后过滤
来源：http://val.zycfv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jgl.shuidangran.top

[Q32] 分组拼接字符串
来源：http://ljy.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://grr.wangdashe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fyr.tanke756.top

[Q33] 多列分组
来源：http://piq.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qha.epnwcf.com

[Q34] 每组取第一条
来源：http://gho.zhijiandao.cn

SELECT * FROM (
来源：http://zgb.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jdo.aibaodan.cn

) t WHERE rn = 1;
来源：http://cbd.birdmap.top

[Q35] 内连接
来源：http://ftk.pengpengdd.cyou

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lnf.316326.xyz

[Q36] 左连接
来源：http://llp.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://krq.pycfn.com

[Q37] 右连接
来源：http://pkh.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jua.quarkkingdee.top

[Q38] 全外连接（PostgreSQL）
来源：http://hls.cheryme.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lbw.wangshuangyany.cn

[Q39] 自连接（查上下级）
来源：http://obw.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://tmx.shanyushiyangtech.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ajs.shanyushiyangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ajv.nwbrower.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://smx.ybcxt.top

[Q41] 多表连接
来源：http://tlu.0kj1m.cn


<!-- 参考信息 -->