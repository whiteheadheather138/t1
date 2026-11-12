代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fvh.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nwp.tanke756.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bzq.dashuyun.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://udf.jlsjyb.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hiv.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ydq.sxryk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tsl.ywan-chungtsiang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dyc.yuanzhike.top

[N05] 最大公约数
来源：http://szp.nwbrower.top

Py:   math.gcd(a, b)
来源：http://ybl.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ywr.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uye.jiagoushi.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://use.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ymy.zhijiandao.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xzz.ybcxt.top

Ruby: a.gcd(b)
来源：http://wpd.sweek.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xpd.fktsv.cn

[N06] 判断回文字符串
来源：http://vnn.ivvv.top

Py:   s == s[::-1]
来源：http://bwx.redwolf501.top

PHP:  $s === strrev($s);
来源：http://vev.aibaodan.cn

JS:   s === [...s].reverse().join("")
来源：http://zkm.9152youxi.cn

TS:   s === [...s].reverse().join("")
来源：http://ypb.svipenyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rud.birdmap.top

Go:   // 双指针从两端比较
来源：http://ljy.c1oappe.top

Ruby: s == s.reverse
来源：http://svv.zhijiandao.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hxb.xylfe.cn

[N07] 两数之和（返回下标）
来源：http://not.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nep.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jfw.jyoumei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ppt.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://qlg.fktsv.cn

Java: // 手写 HashMap
来源：http://yfd.9152youxi.cn

Go:   // 手写 map[int]int
来源：http://vwm.yongpay.top

Ruby: // 手写 Hash
来源：http://kyq.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://vbw.jiagoushi.top

[N08] 生成全排列
来源：http://oso.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://sdr.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://pdg.yfazqb.com

JS:   // 手写回溯递归
来源：http://qqt.daria6918.cn

TS:   // 手写回溯递归
来源：http://fwt.52xcode.cn

Java: // 手写回溯递归
来源：http://ioz.shangyingyoupin.top

Go:   // 手写回溯递归
来源：http://rpm.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://hsb.wangdashe.top

C#:   // 手写回溯递归
来源：http://mjs.jqgufenzy.top

[N09] 栈与队列
来源：http://iwo.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ayl.cheryme.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gje.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gxz.jinqigfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ayn.wangshuangyany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fro.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://chj.ydjk.org.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ciz.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://teb.fengsongda.top

[N10] 链表节点定义
来源：http://pwa.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://efq.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gqt.xuanzx.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mno.zhijiandao.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://prc.yonumen.top

Java: class Node { int v; Node next; }
来源：http://tno.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://vch.ivvv.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zgi.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://ekr.c1oappe.top

[N11] 二叉树中序遍历
来源：http://ffe.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lwu.yj20258.top

PHP:  // 手写递归函数
来源：http://oix.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fhl.shangyingyoupin.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://imw.jianghu66.top

Java: // 手写递归
来源：http://duu.yangfankeji.com

Go:   // 手写递归
来源：http://mvr.aibaodan.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hjy.yuanzhike.top

C#:   // 手写递归
来源：http://bof.shanyushiyangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ija.sysykeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dcd.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xhz.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kws.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ghc.jinghuilouyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dvv.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yxp.nanxinkj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rxq.svipenyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mob.bjfxy.top

================================================================================
来源：http://qjj.9152youxi.cn

O. 并发与异步
来源：http://eip.nwbrower.top

================================================================================
来源：http://rar.9152youxi.cn

[O01] 启动一个线程
来源：http://irw.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hel.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://knn.jyoumei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gzv.hammf.cn

TS:   // 同 JS
来源：http://ejm.xingfuxueyuan.xyz

Java: new Thread(() -> f()).start()
来源：http://wjx.316326.xyz

Go:   go f()
来源：http://mpo.sysykeji.top

Ruby: Thread.new { f }
来源：http://sgv.hfpthk.cn

C#:   Task.Run(() => F());
来源：http://bzc.zycfv.cn

[O02] 使用线程池
来源：http://mho.jlsjyb.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ozf.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kth.mhx1999.top

JS:   // worker_threads 线程池
来源：http://sui.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://wsd.feifeiyinyue.top

Java: Executors.newFixedThreadPool(4)
来源：http://ueb.yvedp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wpg.nwbrower.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jcg.sweek.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://upv.yuxming.cn

[O03] 加锁保护共享数据
来源：http://jjn.zycfv.cn

Py:   with lock: shared += 1
来源：http://zif.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://vig.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://awk.shangyingyoupin.top

TS:   // 同 JS
来源：http://cpg.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://ofy.fanxiaobao.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bfr.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mrv.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://knv.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://jhc.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://php.snrcjt.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yod.wangdashe.top

JS:   async function f() { await g(); }
来源：http://ttg.xuanzx.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://hzy.sweek.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mjf.daria6918.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kjj.hnqzz.top

Ruby: # 用 Fiber 或 async gem
来源：http://qwa.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://ynr.snrcjt.cn

[O05] 并发执行并等待全部完成
来源：http://zcs.sxryk.cn

Py:   asyncio.gather(*tasks)
来源：http://yli.hammf.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jck.fktsv.cn

JS:   await Promise.all(tasks)
来源：http://nid.chenlongwang.top

TS:   await Promise.all(tasks)
来源：http://zch.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wcm.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://szx.yuxming.cn

Ruby: threads.map(&:join)
来源：http://pzq.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bkl.cheryme.top

[O06] 使用进程池
来源：http://ekr.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vjb.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://flq.cdnleiting.top

JS:   // child_process / cluster 模块
来源：http://tgu.jinghuilouyu.cn

TS:   // child_process / cluster 模块
来源：http://fmi.yongpay.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zqs.yj20258.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yau.sjlbkw.cn

Ruby: // fork 块
来源：http://pxw.wangdashe.top

C#:   Parallel.For
来源：http://izu.wangdashe.top

================================================================================
来源：http://rbs.yvedp.cn

P. 常用工具函数
来源：http://hgt.pengpengdd.cyou

================================================================================
来源：http://yue.feifeiyinyue.top

[P01] 生成 UUID
来源：http://zua.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://ovu.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cmw.ivvv.top

JS:   crypto.randomUUID()
来源：http://mac.cqqwz.cn

TS:   crypto.randomUUID()
来源：http://xny.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://eia.fehbvm.com

Go:   // 用 github.com/google/uuid
来源：http://bzv.sysykeji.top

Ruby: SecureRandom.uuid
来源：http://ags.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://whr.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://ufd.hfpthk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uuc.fengsongda.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jxm.tian-w.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aej.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lhj.9152youxi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qjo.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cvi.zycfv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tkc.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yze.bbcook.cn

[P03] 生成短随机字符串
来源：http://qhp.0kj1m.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://umr.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hxm.feifeiyinyue.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cbz.dashuyun.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cyu.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jcu.gogol.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gzs.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qbv.yonumen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qsu.yvedp.cn

[P04] 求长度
来源：http://gys.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fkk.zhaomingkeji.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ldc.epnwcf.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lwh.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ecu.yueranfly.top

Java: list.size();  map.size();  s.length()
来源：http://qve.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://dry.yangfankeji.com

Ruby: x.length;  x.size
来源：http://pww.dashuyun.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zot.yongpay.top

[P05] 判断两个对象内容是否相等
来源：http://ocf.hnxiangtu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://opo.haohaochexian.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://akw.ivvv.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://koe.jinqigufen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gfn.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dnu.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://naz.fanxiaobao.xyz

Ruby: a == b
来源：http://dsz.havefunace.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://czg.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vik.hnqzz.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pod.snrcjt.cn

PHP:  if (empty($x)) {}
来源：http://fld.haohaochexian.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mdj.epnwcf.com

TS:   if (x == null) {}
来源：http://vya.iojbl.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fot.aibaodan.cn

Go:   if x == nil {}
来源：http://cpt.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wnm.yangfankeji.com

C#:   if (x is null) {}
来源：http://bqt.xuanzx.com

[P07] 防抖与节流
来源：http://jfb.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gob.jyoumei.cn

PHP:  // 手写时间戳比较
来源：http://ijn.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qna.epnwcf.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sxg.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ayf.chenlongwang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lws.havefunace.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xpg.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iyo.zhoulong.xyz

[P08] 处理浮点精度问题
来源：http://yir.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ybp.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wmc.fzhhl.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rpt.yuanzhike.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bxd.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eug.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://csf.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ros.ybcxt.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hhk.epnwcf.com

================================================================================
来源：http://gtm.sxryk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pzk.shanyushiyangkeji.top

================================================================================
来源：http://lzx.vqdsnc.cn

[Q01] 创建表
来源：http://eoh.zhongyouzk.top

CREATE TABLE users (
来源：http://esl.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tsc.ybcxt.top

name VARCHAR(50) NOT NULL,
来源：http://hsj.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://oaa.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sak.guowangkeji.top

);
来源：http://ooo.meibo888.top

[Q02] 创建带外键的表
来源：http://mlm.jqgufenzy.top

CREATE TABLE orders (
来源：http://sre.xylfe.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zhl.jinyuanbaomall.cn

user_id INT NOT NULL,
来源：http://qcj.gotoacloud.top

amount DECIMAL(10, 2),
来源：http://gdb.hnqzz.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sjg.gaohongyu789.top

);
来源：http://lam.zhengqikj.top

[Q03] 增加列
来源：http://xtn.guannengcc.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ocf.zhengqikj.top

[Q04] 修改列类型
来源：http://brn.daria6918.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vej.xingfuxueyuan.xyz

[Q05] 重命名列
来源：http://gag.shanyushiyangtech.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dnq.xziqi.cn

[Q06] 删除列
来源：http://osb.wangshuangyany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tmi.meibo888.top

[Q07] 删除表
来源：http://gss.zdbjq.cn

DROP TABLE IF EXISTS orders;
来源：http://ctp.cqqwz.cn

[Q08] 创建普通索引
来源：http://pyj.cqqwz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ycp.fehbvm.com

[Q09] 创建唯一索引
来源：http://hbf.nanxuanxn.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jkb.dianchejie.cn

[Q10] 插入单行
来源：http://jqy.ppjwa.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wlr.yfazqb.com

[Q11] 一次插入多行
来源：http://ydr.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aux.wangshuangyany.cn

[Q12] 插入后取自增 ID
来源：http://zns.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qyu.ivvv.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qpk.ybcxt.top

[Q13] 忽略重复插入
来源：http://pjs.uphjek.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nfh.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://ojq.ywan-chungtsiang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xpk.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oll.gaohongyu789.top

[Q15] 查询全部
来源：http://xko.mhx1999.top

SELECT * FROM users;
来源：http://zsb.fzhhl.top

[Q16] 查询指定列
来源：http://vtq.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://kbo.bjfxy.top

[Q17] 条件查询
来源：http://nuu.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mpp.jyoumei.cn

[Q18] 模糊匹配
来源：http://xjk.guowangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blq.yj202588.top

[Q19] 范围查询
来源：http://wdz.mhx1999.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iuh.snrcjt.cn

[Q20] IN 列表
来源：http://atz.ppjwa.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hlm.uphjek.com

[Q21] 空值判断
来源：http://kpt.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://siy.fktsv.cn

[Q22] 排序
来源：http://vza.hnqzz.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gqb.snrcjt.cn

[Q23] 分页
来源：http://nbm.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ybe.vqdsnc.cn

[Q24] 去重
来源：http://lnm.haohaochexian.top

SELECT DISTINCT city FROM users;
来源：http://pil.tarul.cn

[Q25] 只取前 N 条
来源：http://bgz.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xhy.zdbjq.cn

[Q26] 计数
来源：http://ikb.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://ais.sxryk.cn

[Q27] 条件计数
来源：http://iwz.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jmy.zhengqikj.top

[Q28] 求和与平均
来源：http://yjj.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ljn.hysaishi.cn

[Q29] 最大最小值
来源：http://vbm.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jyj.meibo888.top

[Q30] 分组统计
来源：http://yoi.cqqwz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dhp.hammf.cn

[Q31] 分组后过滤
来源：http://gns.gotoacloud.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uux.hammf.cn

[Q32] 分组拼接字符串
来源：http://dys.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jrv.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xrc.nanxuanxn.top

[Q33] 多列分组
来源：http://ose.aibaodan.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wiv.zhongyouzk.top

[Q34] 每组取第一条
来源：http://mxm.dianchejie.cn

SELECT * FROM (
来源：http://ngx.daxiang520.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://opb.xingfuxueyuan.xyz

) t WHERE rn = 1;
来源：http://rus.yvedp.cn

[Q35] 内连接
来源：http://enx.daxiang520.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ggy.chenlongwang.top


<!-- 参考信息 -->