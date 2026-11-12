代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://tvv.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xtt.yongpay.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kfu.ehwqpu.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hxv.sufxvd.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://krb.havefunace.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://boq.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://hxh.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://nrr.hnxiangtu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jeh.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ael.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wzb.jianghu66.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sjd.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://djg.fengsongda.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bch.chenlongwang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nrj.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jrw.hysaishi.cn

[N05] 最大公约数
来源：http://ahl.wangdashe.top

Py:   math.gcd(a, b)
来源：http://yqc.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wpj.fengsongda.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://esj.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://juo.jqgfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wrd.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zpr.jianghu66.top

Ruby: a.gcd(b)
来源：http://cex.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rfs.bbcook.cn

[N06] 判断回文字符串
来源：http://gcw.hnqzz.top

Py:   s == s[::-1]
来源：http://jll.yj20258.top

PHP:  $s === strrev($s);
来源：http://ruf.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://mhy.cdnleiting.top

TS:   s === [...s].reverse().join("")
来源：http://dgt.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://azr.gzhubu.top

Go:   // 双指针从两端比较
来源：http://ftm.guowangkeji.top

Ruby: s == s.reverse
来源：http://xbt.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://old.316326.xyz

[N07] 两数之和（返回下标）
来源：http://mub.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eoq.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://udo.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wxq.tian-w.cn

TS:   // 手写 Map<string, number>
来源：http://nxo.ivvv.top

Java: // 手写 HashMap
来源：http://ywq.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://ppd.pengpengdd.cyou

Ruby: // 手写 Hash
来源：http://ijs.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://pmq.wangdashe.top

[N08] 生成全排列
来源：http://wyo.epnwcf.com

Py:   itertools.permutations(arr)
来源：http://iyk.52xcode.cn

PHP:  // 手写递归交换
来源：http://ilp.svipenyu.cn

JS:   // 手写回溯递归
来源：http://fcm.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://wjd.cqqwz.cn

Java: // 手写回溯递归
来源：http://mix.xziqi.cn

Go:   // 手写回溯递归
来源：http://qpt.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://jba.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://kyx.dianchejie.cn

[N09] 栈与队列
来源：http://riu.nanxinkj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hft.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lxo.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fvz.svipenyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jtv.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fjx.iojbl.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pem.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://peb.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qyl.hysaishi.cn

[N10] 链表节点定义
来源：http://cwp.haohaochexian.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oey.ivvv.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vpk.hcnkem.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://htr.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qdl.cashguo.top

Java: class Node { int v; Node next; }
来源：http://tbs.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://afl.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fzb.chenlongwang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rch.hesvh.cn

[N11] 二叉树中序遍历
来源：http://zly.jlsjyb.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tcf.fanxiaobao.xyz

PHP:  // 手写递归函数
来源：http://ncx.hcnkem.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dmg.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xcc.zhoulong.xyz

Java: // 手写递归
来源：http://buh.fanxiaobao.xyz

Go:   // 手写递归
来源：http://axq.c1oappe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ztw.chenzaomai.com

C#:   // 手写递归
来源：http://twa.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ion.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lpe.feifeiyinyue.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://szi.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sdc.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gnt.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gxs.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pca.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yfd.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xbn.tarul.cn

================================================================================
来源：http://ghq.pycfn.com

O. 并发与异步
来源：http://kou.gotoacloud.top

================================================================================
来源：http://fcs.gotoacloud.top

[O01] 启动一个线程
来源：http://lws.gaohongyu789.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uzg.jinqigfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rvz.zhengqikj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qgb.wangdashe.top

TS:   // 同 JS
来源：http://vib.chenzaomai.com

Java: new Thread(() -> f()).start()
来源：http://rqf.birdmap.top

Go:   go f()
来源：http://rwg.yvedp.cn

Ruby: Thread.new { f }
来源：http://lgh.bjfxy.top

C#:   Task.Run(() => F());
来源：http://uys.sweek.top

[O02] 使用线程池
来源：http://jvf.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zsq.pengpengdd.cyou

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yhu.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://stu.vehdjk.com

TS:   // worker_threads 线程池
来源：http://kxl.chenjidiqi.icu

Java: Executors.newFixedThreadPool(4)
来源：http://vzi.zdqjudy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jjb.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kav.tanke756.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wbi.jqgfzy.top

[O03] 加锁保护共享数据
来源：http://mpz.hywenlv.cn

Py:   with lock: shared += 1
来源：http://wmy.ydzc1.top

PHP:  // 用 flock() 做文件锁
来源：http://gwx.fengsongda.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xrt.chenlongwang.top

TS:   // 同 JS
来源：http://aoe.fengsongda.top

Java: synchronized (this) { shared++; }
来源：http://ggu.hammf.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mqu.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wps.gzhubu.top

C#:   lock (gate) { shared++; }
来源：http://lpq.jyoumei.cn

[O04] 定义异步函数并等待
来源：http://byv.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://gqz.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cvw.jinyuanbaomall.cn

JS:   async function f() { await g(); }
来源：http://jre.xuetiantiany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://krb.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jgg.yj20258888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tnx.tianlin.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://uqg.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://sdu.nanxinkj.top

[O05] 并发执行并等待全部完成
来源：http://imj.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://yvp.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eom.yj202588.top

JS:   await Promise.all(tasks)
来源：http://jcg.gaohongyu789.top

TS:   await Promise.all(tasks)
来源：http://bdh.jiagoushi.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cry.aibaodan.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://spc.zhaomingkeji.xyz

Ruby: threads.map(&:join)
来源：http://ctq.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://imh.jiagoushi.top

[O06] 使用进程池
来源：http://sku.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jim.smart0.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://dam.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://udi.sufxvd.cn

TS:   // child_process / cluster 模块
来源：http://svg.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fjn.ehwqpu.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zpw.jlsjyb.cn

Ruby: // fork 块
来源：http://mui.hesvh.cn

C#:   Parallel.For
来源：http://qjb.hongshengwenyu.top

================================================================================
来源：http://iwc.bbcook.cn

P. 常用工具函数
来源：http://etz.yj20258.top

================================================================================
来源：http://clm.cheryme.top

[P01] 生成 UUID
来源：http://zeq.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://nuf.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bfj.daxiang520.top

JS:   crypto.randomUUID()
来源：http://bcq.nanxinkj.top

TS:   crypto.randomUUID()
来源：http://efl.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://qrd.sjlbkw.cn

Go:   // 用 github.com/google/uuid
来源：http://zqt.svipenyu.cn

Ruby: SecureRandom.uuid
来源：http://lmr.xziqi.cn

C#:   Guid.NewGuid().ToString()
来源：http://pru.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://ozs.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aln.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cqq.nanxinkj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mnf.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://crx.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://edw.xuanzx.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pox.ydjk.org.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tyc.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wcx.hesvh.cn

[P03] 生成短随机字符串
来源：http://aqc.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cqe.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eko.jiagoushi.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sdt.zycfv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gcg.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kqh.c1oappe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jxd.sysykeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vlz.svipenyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pxg.jinghuilouyu.cn

[P04] 求长度
来源：http://ecj.hammf.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cyo.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xuq.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sii.cqqwz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jyk.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://xch.hesvh.cn

Go:   len(arr);  len(m)
来源：http://bug.svipenyu.cn

Ruby: x.length;  x.size
来源：http://deu.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vzr.fanxiaobao.xyz

[P05] 判断两个对象内容是否相等
来源：http://qpj.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ndb.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oma.zhiwuduotai.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fur.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ucl.daria6918.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zrh.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://dqg.kuanghao11.cn

Ruby: a == b
来源：http://uoh.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qdp.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eio.jqgufenzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://agt.tanke756.top

PHP:  if (empty($x)) {}
来源：http://utr.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cnz.zycfv.cn

TS:   if (x == null) {}
来源：http://cch.chenzaomai.com

Java: if (x == null || x.isEmpty()) {}
来源：http://jkb.shzxlz.cn

Go:   if x == nil {}
来源：http://mav.ybcxt.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fxx.tianlin.xyz

C#:   if (x is null) {}
来源：http://fal.ivvv.top

[P07] 防抖与节流
来源：http://sfm.mhx1999.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gvt.tanke756.top

PHP:  // 手写时间戳比较
来源：http://nmg.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wae.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uqo.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ygw.cashguo.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fqv.ydjk.org.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vhm.redwolf501.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sva.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://zme.jinyuanbaomall.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jaq.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rke.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wuc.zdbjq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yiu.ivvv.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mmp.gogol.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hov.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jew.zhengqikj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fpu.ydjk.org.cn

================================================================================
来源：http://eee.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vhq.chenlongwang.top

================================================================================
来源：http://ibs.smart0.xyz

[Q01] 创建表
来源：http://ixu.9152youxi.cn

CREATE TABLE users (
来源：http://swf.ydjk.org.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://krq.yvedp.cn

name VARCHAR(50) NOT NULL,
来源：http://szi.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://vhf.yonumen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://drs.zdqjudy.top

);
来源：http://aco.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://ysv.yfazqb.com

CREATE TABLE orders (
来源：http://mrh.9152youxi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wix.zdbjq.cn

user_id INT NOT NULL,
来源：http://dzv.xuetiantiany.cn

amount DECIMAL(10, 2),
来源：http://nqp.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bvn.vehdjk.com

);
来源：http://jph.jinghuilouyu.cn

[Q03] 增加列
来源：http://dwj.sxryk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ypx.dashuyun.cn

[Q04] 修改列类型
来源：http://hdg.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vly.zhiwuduotai.top

[Q05] 重命名列
来源：http://ity.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jjp.wangdashe.top

[Q06] 删除列
来源：http://nvf.nanxuanxn.top

ALTER TABLE users DROP COLUMN age;
来源：http://gsm.yj20258888.top

[Q07] 删除表
来源：http://ipd.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://dqj.yj202588.top

[Q08] 创建普通索引
来源：http://lbi.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bdb.aizwys.cn

[Q09] 创建唯一索引
来源：http://zhi.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yop.316326.xyz

[Q10] 插入单行
来源：http://kie.xuanzx.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://enc.sweek.top

[Q11] 一次插入多行
来源：http://zjz.ehwqpu.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vcj.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://lcn.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eqs.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zhz.hysaishi.cn

[Q13] 忽略重复插入
来源：http://yag.xuetiantiany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jrh.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://rcn.chenlongwang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wem.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wgd.chenjidiqi.icu

[Q15] 查询全部
来源：http://ryk.fengsongda.top

SELECT * FROM users;
来源：http://pcr.shanyushiyangkeji.top

[Q16] 查询指定列
来源：http://bja.ivvv.top

SELECT id, name FROM users;
来源：http://aic.yj202588.top

[Q17] 条件查询
来源：http://uxy.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ruc.hnxiangtu.top

[Q18] 模糊匹配
来源：http://osj.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vqe.fanxiaobao.xyz

[Q19] 范围查询
来源：http://bnd.bbcook.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dro.bjfxy.top

[Q20] IN 列表
来源：http://och.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fwg.shuidangran.top

[Q21] 空值判断
来源：http://iab.52xcode.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vnj.pengpengdd.cyou

[Q22] 排序
来源：http://mxu.pycfn.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ihl.zhengqikj.top

[Q23] 分页
来源：http://bcd.tian-w.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://far.tianlin.xyz

[Q24] 去重
来源：http://mab.tianlin.xyz

SELECT DISTINCT city FROM users;
来源：http://tms.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://zee.hammf.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bzd.yuanzhike.top

[Q26] 计数
来源：http://bav.vehdjk.com

SELECT COUNT(*) FROM users;
来源：http://trz.ppjwa.cn

[Q27] 条件计数
来源：http://mzq.gotoacloud.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://etu.hywenlv.cn

[Q28] 求和与平均
来源：http://yaf.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gqu.sxryk.cn

[Q29] 最大最小值
来源：http://anf.0kj1m.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jwt.aibaodan.cn

[Q30] 分组统计
来源：http://pzh.meibo888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uhj.guannengcc.top

[Q31] 分组后过滤
来源：http://uuo.yonumen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ofv.sysykeji.top

[Q32] 分组拼接字符串
来源：http://gpb.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qlz.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qju.316326.xyz


<!-- 参考信息 -->