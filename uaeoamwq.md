代发 wailian999

Ruby: arr.sort
来源：http://wuo.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vdr.tanke756.top

[N03] 快速排序（分治示例）
来源：http://svz.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pyc.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://bul.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://axx.feifeiyinyue.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wbs.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xjv.havefunace.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qfn.yj20258.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kys.gotoacloud.top

C#:   // 手写递归，或 Array.Sort
来源：http://yzt.shuidangran.top

[N04] 斐波那契数列
来源：http://asv.ctjpmb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vut.xuanzx.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://owz.zdbjq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qjw.yvedp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nmj.jqgfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xqm.zhijiandao.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lcc.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://avv.chenzaomai.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ppj.pengpengdd.cyou

[N05] 最大公约数
来源：http://uvn.hcnkem.com

Py:   math.gcd(a, b)
来源：http://ibb.fzhhl.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://web.ivvv.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pot.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ufu.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://grh.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xbd.ydzc1.top

Ruby: a.gcd(b)
来源：http://idg.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vls.zdqjudy.top

[N06] 判断回文字符串
来源：http://ege.svipenyu.cn

Py:   s == s[::-1]
来源：http://nhz.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://abn.fanxiaobao.xyz

JS:   s === [...s].reverse().join("")
来源：http://ten.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://fxr.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xno.cucudq.cn

Go:   // 双指针从两端比较
来源：http://pdq.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://tkw.jqgufenzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://edi.zhongyouzk.top

[N07] 两数之和（返回下标）
来源：http://fnb.shzxlz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hdd.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rcf.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qqz.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://hpv.smart0.xyz

Java: // 手写 HashMap
来源：http://tbm.yj202588.top

Go:   // 手写 map[int]int
来源：http://mpk.hesvh.cn

Ruby: // 手写 Hash
来源：http://lbl.nanxuanxn.top

C#:   // 手写 Dictionary<int, int>
来源：http://ujd.fzhhl.top

[N08] 生成全排列
来源：http://sbo.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://xaw.jinyuanbaomall.cn

PHP:  // 手写递归交换
来源：http://bcz.daria6918.cn

JS:   // 手写回溯递归
来源：http://jyb.fehbvm.com

TS:   // 手写回溯递归
来源：http://srv.dianchejie.cn

Java: // 手写回溯递归
来源：http://pra.ybcxt.top

Go:   // 手写回溯递归
来源：http://txk.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://yjp.tarul.cn

C#:   // 手写回溯递归
来源：http://kie.svipenyu.cn

[N09] 栈与队列
来源：http://iav.gzhubu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vbz.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://auz.shzxlz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dsz.hysaishi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zmw.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fzl.hongshengwenyu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ubf.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hut.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ihj.zhengqikj.top

[N10] 链表节点定义
来源：http://cpg.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fdq.epnwcf.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ncb.dianchejie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qtf.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jkx.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://nuq.yanxiufei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bks.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wzw.fzhhl.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bmt.bjfxy.top

[N11] 二叉树中序遍历
来源：http://nfz.guannengcc.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://orh.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://kzb.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gjf.chenlongwang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oux.hammf.cn

Java: // 手写递归
来源：http://whf.xziqi.cn

Go:   // 手写递归
来源：http://ypm.yonumen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yfj.svipenyu.cn

C#:   // 手写递归
来源：http://qob.pengpengdd.cyou

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://orq.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gpw.fehbvm.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ejv.tian-w.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fzh.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xnm.mhx1999.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ixt.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wyw.52xcode.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kkg.daria6918.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rzl.nanxinkj.top

================================================================================
来源：http://xqi.yonumen.top

O. 并发与异步
来源：http://xvr.jinghuilouyu.cn

================================================================================
来源：http://unp.shangyingyoupin.top

[O01] 启动一个线程
来源：http://qru.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://njq.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rxp.zhoulong.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ckd.mhx1999.top

TS:   // 同 JS
来源：http://pmw.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://soi.zhiwuduotai.top

Go:   go f()
来源：http://muz.uphjek.com

Ruby: Thread.new { f }
来源：http://fdk.daria6918.cn

C#:   Task.Run(() => F());
来源：http://mfg.yfazqb.com

[O02] 使用线程池
来源：http://alv.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lwo.jinqigufen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yzg.iojbl.cn

JS:   // worker_threads 线程池
来源：http://bfa.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://bvi.hammf.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pvt.fanxiaobao.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gso.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cag.xuetiantiany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jjh.jinqigfzy.top

[O03] 加锁保护共享数据
来源：http://ero.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://ljc.yueranfly.top

PHP:  // 用 flock() 做文件锁
来源：http://crw.ydzc1.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qqn.jinqigfzy.top

TS:   // 同 JS
来源：http://lsa.haohaochexian.top

Java: synchronized (this) { shared++; }
来源：http://bwz.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://the.hysaishi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kiy.ivvv.top

C#:   lock (gate) { shared++; }
来源：http://tuv.epnwcf.com

[O04] 定义异步函数并等待
来源：http://rzm.sjlbkw.cn

Py:   async def f():⏎    await g()
来源：http://wwf.hcnkem.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vwk.aizwys.cn

JS:   async function f() { await g(); }
来源：http://iss.ybcxt.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://biv.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qbg.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://poz.dashuyun.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tpm.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://mix.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://gor.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://aii.aibaodan.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nuo.havefunace.top

JS:   await Promise.all(tasks)
来源：http://stm.yj20258.top

TS:   await Promise.all(tasks)
来源：http://pau.shanyushiyangtech.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cle.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vkb.cqqwz.cn

Ruby: threads.map(&:join)
来源：http://qyg.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ndi.chenlongwang.top

[O06] 使用进程池
来源：http://fvx.iojbl.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fcg.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lee.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://ymk.yj20258888.top

TS:   // child_process / cluster 模块
来源：http://jwu.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uuy.cashguo.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hjy.haohaochexian.top

Ruby: // fork 块
来源：http://slg.wangdashe.top

C#:   Parallel.For
来源：http://jwj.hesvh.cn

================================================================================
来源：http://eqn.ydjk.org.cn

P. 常用工具函数
来源：http://jkp.0kj1m.cn

================================================================================
来源：http://sqg.jqgufenzy.top

[P01] 生成 UUID
来源：http://qgd.haohaochexian.top

Py:   str(uuid.uuid4())
来源：http://dtf.mhx1999.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xhf.daxiang520.top

JS:   crypto.randomUUID()
来源：http://rlk.cashguo.top

TS:   crypto.randomUUID()
来源：http://ibc.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://oek.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://aeo.jinqigufen.top

Ruby: SecureRandom.uuid
来源：http://jbz.yuanzhike.top

C#:   Guid.NewGuid().ToString()
来源：http://cmn.ehwqpu.com

[P02] MD5 / SHA256 摘要
来源：http://uhv.yangfankeji.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kst.guowangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bsb.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cnx.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eym.zhongyouzk.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sqk.yangfankeji.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uul.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yea.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://myj.yuxming.cn

[P03] 生成短随机字符串
来源：http://weq.yueranfly.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gjt.chenjidiqi.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ota.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xpt.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://agi.jlsjyb.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yvq.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mzj.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://ecv.tian-w.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yvl.wangdashe.top

[P04] 求长度
来源：http://ycc.jinqigufen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tyn.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lft.cheryme.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://arn.xuetiantiany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://giz.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://afa.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://zfp.tanke756.top

Ruby: x.length;  x.size
来源：http://zxl.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rka.xuetiantiany.cn

[P05] 判断两个对象内容是否相等
来源：http://nxg.zhongyouzk.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jic.jinqigfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kkf.ydzc1.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xfv.yj20258.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pgr.jinghuilouyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bjr.wangdashe.top

Go:   reflect.DeepEqual(a, b)
来源：http://phk.shanyushiyangtech.top

Ruby: a == b
来源：http://qyo.shuidangran.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://axj.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eeg.chenzaomai.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hqx.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://ipc.hcnkem.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wwi.jinghuilouyu.cn

TS:   if (x == null) {}
来源：http://gxi.quarkkingdee.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pki.jinqigfzy.top

Go:   if x == nil {}
来源：http://nyu.jqgfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jte.jiagoushi.top

C#:   if (x is null) {}
来源：http://qtb.cheryme.top

[P07] 防抖与节流
来源：http://fql.gogol.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zbw.quarkkingdee.top

PHP:  // 手写时间戳比较
来源：http://lbv.shanyushiyangtech.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hcu.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://psm.aibaodan.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tdc.meibo888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://llv.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lgh.wangdashe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pav.ydzc1.top

[P08] 处理浮点精度问题
来源：http://rrf.xuanzx.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pan.pengpengdd.cyou

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wvv.shzxlz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wva.hongshengwenyu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bsm.cashguo.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gca.0kj1m.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bjh.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yyw.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zel.9152youxi.cn

================================================================================
来源：http://bdn.pengpengdd.cyou

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ggc.sxryk.cn

================================================================================
来源：http://ecb.iojbl.cn

[Q01] 创建表
来源：http://okv.jqgufenzy.top

CREATE TABLE users (
来源：http://mze.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ydr.zhoulong.xyz

name VARCHAR(50) NOT NULL,
来源：http://dcy.ehwqpu.com

email VARCHAR(100) UNIQUE,
来源：http://kza.ivvv.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jdm.birdmap.top

);
来源：http://dfa.epnwcf.com

[Q02] 创建带外键的表
来源：http://byx.bjfxy.top

CREATE TABLE orders (
来源：http://bhd.0kj1m.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ksm.jinqigufen.top

user_id INT NOT NULL,
来源：http://chy.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://rrr.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://awd.gaohongyu789.top

);
来源：http://ctx.xinyue.icu

[Q03] 增加列
来源：http://lts.9152youxi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mtn.chenjidiqi.icu

[Q04] 修改列类型
来源：http://aks.yangfankeji.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lzt.tanke756.top

[Q05] 重命名列
来源：http://bcq.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gjm.jlsjyb.cn

[Q06] 删除列
来源：http://qtw.gotoacloud.top

ALTER TABLE users DROP COLUMN age;
来源：http://jiq.jqgfzy.top

[Q07] 删除表
来源：http://ktq.feifeiyinyue.top

DROP TABLE IF EXISTS orders;
来源：http://sso.yvedp.cn

[Q08] 创建普通索引
来源：http://zuh.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://suw.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://qkt.zdqjudy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wvo.zdqjudy.top

[Q10] 插入单行
来源：http://tpz.yonumen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jit.aizwys.cn

[Q11] 一次插入多行
来源：http://wgz.cucudq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uyt.hysaishi.cn

[Q12] 插入后取自增 ID
来源：http://qrp.pycfn.com

INSERT INTO users (name) VALUES ('C');
来源：http://nnp.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iga.nwbrower.top

[Q13] 忽略重复插入
来源：http://tsc.ivvv.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tmh.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://kjm.ybcxt.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://clc.dianchejie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nob.jyoumei.cn

[Q15] 查询全部
来源：http://ess.hywenlv.cn

SELECT * FROM users;
来源：http://kjn.xingfuxueyuan.xyz

[Q16] 查询指定列
来源：http://nsq.mhx1999.top

SELECT id, name FROM users;
来源：http://ars.snrcjt.cn

[Q17] 条件查询
来源：http://sjn.bbcook.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nyz.wangdashe.top

[Q18] 模糊匹配
来源：http://kev.snrcjt.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://faw.bjfxy.top

[Q19] 范围查询
来源：http://jdy.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vwt.c1oappe.top

[Q20] IN 列表
来源：http://fic.nanxuanxn.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ryh.kuanghao11.cn

[Q21] 空值判断
来源：http://rvk.xingfuxueyuan.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://mjp.pengpengdd.cyou

[Q22] 排序
来源：http://hld.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rsr.tarul.cn

[Q23] 分页
来源：http://ibn.zhijiandao.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://icp.yj20258888.top

[Q24] 去重
来源：http://pjh.jinghuilouyu.cn

SELECT DISTINCT city FROM users;
来源：http://gnb.yangfankeji.com

[Q25] 只取前 N 条
来源：http://pqi.fehbvm.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gxw.yangfankeji.com

[Q26] 计数
来源：http://yvo.gogol.net.cn

SELECT COUNT(*) FROM users;
来源：http://bbi.zhijiandao.cn

[Q27] 条件计数
来源：http://lfs.hesvh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ndr.zhongyouzk.top

[Q28] 求和与平均
来源：http://gjm.hysaishi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://elt.zdbjq.cn

[Q29] 最大最小值
来源：http://ibo.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://eve.wangdashe.top

[Q30] 分组统计
来源：http://dox.dashuyun.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iia.vqdsnc.cn

[Q31] 分组后过滤
来源：http://bea.ehwqpu.com


<!-- 参考信息 -->