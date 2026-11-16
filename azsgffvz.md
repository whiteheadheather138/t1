代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jnt.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://okf.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eri.shanyushiyangtech.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vsr.zhoulong.xyz

[N05] 最大公约数
来源：http://eyn.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://mjt.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xye.tanke756.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xyc.ydzc1.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kqi.ydzc1.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wna.fengsongda.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qmj.mhx1999.top

Ruby: a.gcd(b)
来源：http://rkp.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bum.nwbrower.top

[N06] 判断回文字符串
来源：http://okp.sysykeji.top

Py:   s == s[::-1]
来源：http://bvb.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://wgf.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://qnd.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://lkc.yueranfly.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ttt.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://qjj.tarul.cn

Ruby: s == s.reverse
来源：http://klg.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sjt.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://isa.cheryme.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vwq.snrcjt.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zty.hnxiangtu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://one.sxryk.cn

TS:   // 手写 Map<string, number>
来源：http://esd.shuidangran.top

Java: // 手写 HashMap
来源：http://obe.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://tfy.xuanzx.com

Ruby: // 手写 Hash
来源：http://kci.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vlc.9152youxi.cn

[N08] 生成全排列
来源：http://uel.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://yoo.jiagoushi.top

PHP:  // 手写递归交换
来源：http://xta.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://fej.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://njj.fengsongda.top

Java: // 手写回溯递归
来源：http://hyx.xinyue.icu

Go:   // 手写回溯递归
来源：http://yix.vehdjk.com

Ruby: arr.permutation.to_a
来源：http://ond.pengpengdd.cyou

C#:   // 手写回溯递归
来源：http://tah.zhoulong.xyz

[N09] 栈与队列
来源：http://bxw.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vfh.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xpc.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iln.cucudq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ije.zhixingplan.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dzu.gogol.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://krp.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ccm.9152youxi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gmc.shanyushiyangkeji.top

[N10] 链表节点定义
来源：http://zee.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tsq.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oxi.aibaodan.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eok.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gfi.zdbjq.cn

Java: class Node { int v; Node next; }
来源：http://cah.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://vcq.jianghu66.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mze.hnxiangtu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zzj.sxryk.cn

[N11] 二叉树中序遍历
来源：http://mti.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mfr.0kj1m.cn

PHP:  // 手写递归函数
来源：http://lyu.fanxiaobao.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jpv.tanke756.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uut.ehwqpu.com

Java: // 手写递归
来源：http://ntr.jlsjyb.cn

Go:   // 手写递归
来源：http://ibl.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aen.jlsjyb.cn

C#:   // 手写递归
来源：http://fww.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ufb.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://afk.chenzaomai.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lzm.c1oappe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yjm.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://djt.yangfankeji.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kvg.meibo888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vhs.0kj1m.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fah.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rmq.yuanzhike.top

================================================================================
来源：http://tya.pycfn.com

O. 并发与异步
来源：http://xrt.jiagoushi.top

================================================================================
来源：http://ssd.wangdashe.top

[O01] 启动一个线程
来源：http://bgb.ivvv.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eai.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mrz.zdbjq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ieu.zycfv.cn

TS:   // 同 JS
来源：http://egc.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://utq.zhaomingkeji.xyz

Go:   go f()
来源：http://bkx.yanxiufei.cn

Ruby: Thread.new { f }
来源：http://pjd.guannengcc.top

C#:   Task.Run(() => F());
来源：http://vgj.andypj.xyz

[O02] 使用线程池
来源：http://adp.fzhhl.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tsu.hongshengwenyu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fuo.yj20258888.top

JS:   // worker_threads 线程池
来源：http://tey.zhijiandao.cn

TS:   // worker_threads 线程池
来源：http://nma.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://qaf.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wdp.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mij.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aly.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://seb.dashuyun.cn

Py:   with lock: shared += 1
来源：http://gmz.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://dug.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kok.zhoulong.xyz

TS:   // 同 JS
来源：http://wer.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://hdz.hnxiangtu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jfd.aibaodan.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iun.kuanghao11.cn

C#:   lock (gate) { shared++; }
来源：http://jii.tian-w.cn

[O04] 定义异步函数并等待
来源：http://acz.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://kbf.xuanzx.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hun.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://rwp.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://yrp.shanyushiyangtech.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oov.feifeiyinyue.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://etp.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://slb.sxryk.cn

C#:   async Task F() { await G(); }
来源：http://wkq.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://zyv.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://rst.yj20258.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vpj.yonumen.top

JS:   await Promise.all(tasks)
来源：http://ojq.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://uhm.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gcz.redwolf501.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vjr.uphjek.com

Ruby: threads.map(&:join)
来源：http://mzv.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ygo.dianchejie.cn

[O06] 使用进程池
来源：http://qcv.hnqzz.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://njt.bbcook.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://btv.andypj.xyz

JS:   // child_process / cluster 模块
来源：http://syx.cdnleiting.top

TS:   // child_process / cluster 模块
来源：http://agj.sweek.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ieb.xylfe.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gsg.tian-w.cn

Ruby: // fork 块
来源：http://gtu.zycfv.cn

C#:   Parallel.For
来源：http://naw.nanxuanxn.top

================================================================================
来源：http://evo.hnxiangtu.top

P. 常用工具函数
来源：http://flm.cheryme.top

================================================================================
来源：http://gtd.nanxinkj.top

[P01] 生成 UUID
来源：http://taf.chenjidiqi.icu

Py:   str(uuid.uuid4())
来源：http://abh.yuanzhike.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gqb.tarul.cn

JS:   crypto.randomUUID()
来源：http://lip.jiagoushi.top

TS:   crypto.randomUUID()
来源：http://zdb.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://dpb.kuanghao11.cn

Go:   // 用 github.com/google/uuid
来源：http://coa.jqgufenzy.top

Ruby: SecureRandom.uuid
来源：http://fks.feifeiyinyue.top

C#:   Guid.NewGuid().ToString()
来源：http://wut.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://kau.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tdo.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fab.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ylm.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://awc.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ffw.bbcook.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://stv.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hmo.cdnleiting.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aeu.gogol.net.cn

[P03] 生成短随机字符串
来源：http://vbw.jianghu66.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ueg.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kbj.shuidangran.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lee.aibaodan.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qjs.uphjek.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jha.zycfv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kxd.sysykeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gge.haohaochexian.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://suv.epnwcf.com

[P04] 求长度
来源：http://vqj.9152youxi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://shf.0kj1m.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mid.hywenlv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ici.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zah.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://jpc.sysykeji.top

Go:   len(arr);  len(m)
来源：http://srz.tarul.cn

Ruby: x.length;  x.size
来源：http://ojc.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://cib.bjfxy.top

[P05] 判断两个对象内容是否相等
来源：http://sei.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wvo.nwbrower.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xcc.nanxuanxn.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gwf.gaohongyu789.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ywh.yvedp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fau.yangfankeji.com

Go:   reflect.DeepEqual(a, b)
来源：http://taf.vehdjk.com

Ruby: a == b
来源：http://enj.aizwys.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://std.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yju.zhengqikj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yei.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://dij.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fav.pycfn.com

TS:   if (x == null) {}
来源：http://isw.jiagoushi.top

Java: if (x == null || x.isEmpty()) {}
来源：http://izl.haohaochexian.top

Go:   if x == nil {}
来源：http://zgf.smart0.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xgg.yanxiufei.cn

C#:   if (x is null) {}
来源：http://fds.iojbl.cn

[P07] 防抖与节流
来源：http://fxz.fanxiaobao.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hfv.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://yrz.snrcjt.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tcm.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rsm.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vbt.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://odu.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pcd.sweek.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cxg.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://srr.yj20258888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xti.nanxinkj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://las.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kuk.hysaishi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wdl.daxiang520.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ogp.shanyushiyangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oan.shzxlz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zmr.sxryk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://njb.hywenlv.cn

================================================================================
来源：http://hvf.cdnleiting.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://brv.dianchejie.cn

================================================================================
来源：http://wlj.dianchejie.cn

[Q01] 创建表
来源：http://tma.pengpengdd.cyou

CREATE TABLE users (
来源：http://zjl.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lmq.ivvv.top

name VARCHAR(50) NOT NULL,
来源：http://but.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://atg.fktsv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://neo.tanke756.top

);
来源：http://ywd.yueranfly.top

[Q02] 创建带外键的表
来源：http://zot.feifeiyinyue.top

CREATE TABLE orders (
来源：http://vxa.jqgufenzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uso.smart0.xyz

user_id INT NOT NULL,
来源：http://wmf.tanke756.top

amount DECIMAL(10, 2),
来源：http://xno.yonumen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mrs.cheryme.top

);
来源：http://rmd.ctjpmb.com

[Q03] 增加列
来源：http://dtm.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fuj.shangyingyoupin.top

[Q04] 修改列类型
来源：http://lqy.havefunace.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zgt.nanxinkj.top

[Q05] 重命名列
来源：http://usb.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ush.hesvh.cn

[Q06] 删除列
来源：http://vuj.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://mde.havefunace.top

[Q07] 删除表
来源：http://qax.fanxiaobao.xyz

DROP TABLE IF EXISTS orders;
来源：http://aab.bjfxy.top

[Q08] 创建普通索引
来源：http://eci.tanke756.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xwq.haohaochexian.top

[Q09] 创建唯一索引
来源：http://eez.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cjw.ivvv.top

[Q10] 插入单行
来源：http://vab.hfpthk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mee.epnwcf.com

[Q11] 一次插入多行
来源：http://kvl.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jhg.zhijiandao.cn

[Q12] 插入后取自增 ID
来源：http://ddh.ybcxt.top

INSERT INTO users (name) VALUES ('C');
来源：http://fgi.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://csc.shangyingyoupin.top

[Q13] 忽略重复插入
来源：http://pij.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kbd.ppjwa.cn

[Q14] 存在则更新（upsert）
来源：http://afx.yfazqb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tug.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zdq.epnwcf.com

[Q15] 查询全部
来源：http://hwg.yangfankeji.com

SELECT * FROM users;
来源：http://few.c1oappe.top

[Q16] 查询指定列
来源：http://dru.tanke756.top

SELECT id, name FROM users;
来源：http://omk.yueranfly.top

[Q17] 条件查询
来源：http://puz.yonumen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wpf.sweek.top

[Q18] 模糊匹配
来源：http://dzp.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xmz.zhixingplan.top

[Q19] 范围查询
来源：http://bdm.guowangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cpg.ivvv.top

[Q20] IN 列表
来源：http://ryk.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sem.yonumen.top

[Q21] 空值判断
来源：http://jlf.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rac.fengsongda.top

[Q22] 排序
来源：http://omz.dashuyun.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fti.jlsjyb.cn

[Q23] 分页
来源：http://rat.chenzaomai.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bsp.nwbrower.top

[Q24] 去重
来源：http://gih.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://www.cqqwz.cn

[Q25] 只取前 N 条
来源：http://top.316326.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dkg.zycfv.cn

[Q26] 计数
来源：http://ipp.hongshengwenyu.top

SELECT COUNT(*) FROM users;
来源：http://mds.guannengcc.top

[Q27] 条件计数
来源：http://kqs.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ymy.yanxiufei.cn

[Q28] 求和与平均
来源：http://jfx.nwbrower.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://irq.yj20258.top

[Q29] 最大最小值
来源：http://cnp.smart0.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://ykn.cdnleiting.top

[Q30] 分组统计
来源：http://fbm.chenlongwang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zlm.snrcjt.cn

[Q31] 分组后过滤
来源：http://cmb.gzhubu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qhz.epnwcf.com

[Q32] 分组拼接字符串
来源：http://mji.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iks.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eor.sxryk.cn

[Q33] 多列分组
来源：http://hqa.jinghuilouyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rwi.cqqwz.cn

[Q34] 每组取第一条
来源：http://hlc.fanxiaobao.xyz

SELECT * FROM (
来源：http://ija.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zhi.bjfxy.top

) t WHERE rn = 1;
来源：http://gut.uphjek.com

[Q35] 内连接
来源：http://agw.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rro.birdmap.top

[Q36] 左连接
来源：http://dgk.bbcook.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://upw.cqqwz.cn

[Q37] 右连接
来源：http://iyb.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ljb.ydjk.org.cn


<!-- 参考信息 -->