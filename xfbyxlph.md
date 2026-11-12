代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://qja.316326.xyz

[N02] 排序（工程实践用内置实现）
来源：http://eso.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://apv.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://szs.mhx1999.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vsl.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://edv.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hka.52xcode.cn

Go:   slices.Sort(arr)
来源：http://ddc.xuetiantiany.cn

Ruby: arr.sort
来源：http://zal.tarul.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fwc.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://cvw.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mtj.zhongyouzk.top

PHP:  // 递归实现，或用 usort
来源：http://myl.cucudq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dek.jiagoushi.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qdn.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yxj.gaohongyu789.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ajl.iojbl.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hwq.fehbvm.com

C#:   // 手写递归，或 Array.Sort
来源：http://qvl.chenzaomai.com

[N04] 斐波那契数列
来源：http://hpl.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nuo.daxiang520.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nmv.ydjk.org.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cnb.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gxf.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://drn.fengsongda.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qjb.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xco.jinqigfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lxu.jyoumei.cn

[N05] 最大公约数
来源：http://gnz.kuanghao11.cn

Py:   math.gcd(a, b)
来源：http://xfx.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eth.uphjek.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nsc.nanxuanxn.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xmp.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dai.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lmm.yuxming.cn

Ruby: a.gcd(b)
来源：http://kgw.sxryk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://glh.hammf.cn

[N06] 判断回文字符串
来源：http://kin.yj202588.top

Py:   s == s[::-1]
来源：http://isd.shangyingyoupin.top

PHP:  $s === strrev($s);
来源：http://skc.havefunace.top

JS:   s === [...s].reverse().join("")
来源：http://yjy.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://kef.hnxiangtu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nvy.vehdjk.com

Go:   // 双指针从两端比较
来源：http://iqw.zhongyouzk.top

Ruby: s == s.reverse
来源：http://rkb.gzhubu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ykv.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://eqa.fehbvm.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://aet.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://inm.jinyuanbaomall.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dkl.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://tau.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://tkc.chenjidiqi.icu

Go:   // 手写 map[int]int
来源：http://asx.havefunace.top

Ruby: // 手写 Hash
来源：http://xoe.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://war.ydzc1.top

[N08] 生成全排列
来源：http://xol.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://ibh.chenjidiqi.icu

PHP:  // 手写递归交换
来源：http://epc.gzhubu.top

JS:   // 手写回溯递归
来源：http://fny.fehbvm.com

TS:   // 手写回溯递归
来源：http://vpm.aizwys.cn

Java: // 手写回溯递归
来源：http://xlk.yvedp.cn

Go:   // 手写回溯递归
来源：http://pzn.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://zpx.yueranfly.top

C#:   // 手写回溯递归
来源：http://lcy.zhongyouzk.top

[N09] 栈与队列
来源：http://uai.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://szq.havefunace.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uvq.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qsw.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tvh.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hue.hesvh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wwo.tanke756.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://akn.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dim.shzxlz.cn

[N10] 链表节点定义
来源：http://rwc.yj20258888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vun.bjfxy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mra.wangdashe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ijo.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://szk.316326.xyz

Java: class Node { int v; Node next; }
来源：http://ern.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://npb.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zkr.sufxvd.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://arw.redwolf501.top

[N11] 二叉树中序遍历
来源：http://zea.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vmj.fktsv.cn

PHP:  // 手写递归函数
来源：http://fed.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dks.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eye.zhoulong.xyz

Java: // 手写递归
来源：http://jzs.fzhhl.top

Go:   // 手写递归
来源：http://dtg.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ehx.ivvv.top

C#:   // 手写递归
来源：http://bed.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lco.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nmu.aizwys.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sga.ydzc1.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bth.yuxming.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jnc.yvedp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lqi.xingfuxueyuan.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eaf.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ale.andypj.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gtu.hammf.cn

================================================================================
来源：http://wdy.zhijiandao.cn

O. 并发与异步
来源：http://esj.cheryme.top

================================================================================
来源：http://xyt.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://ogm.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uqz.jyoumei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://egq.cqqwz.cn

TS:   // 同 JS
来源：http://qrv.zycfv.cn

Java: new Thread(() -> f()).start()
来源：http://xfl.xylfe.cn

Go:   go f()
来源：http://itx.jiagoushi.top

Ruby: Thread.new { f }
来源：http://otn.birdmap.top

C#:   Task.Run(() => F());
来源：http://lqj.ybcxt.top

[O02] 使用线程池
来源：http://mgn.xziqi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qzw.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jyi.jinqigfzy.top

JS:   // worker_threads 线程池
来源：http://qhf.0kj1m.cn

TS:   // worker_threads 线程池
来源：http://zpo.bjfxy.top

Java: Executors.newFixedThreadPool(4)
来源：http://shv.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nkv.hfpthk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xhp.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gls.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://cva.yuxming.cn

Py:   with lock: shared += 1
来源：http://juv.jinqigfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://uwf.yvedp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zrz.shzxlz.cn

TS:   // 同 JS
来源：http://yid.tanke756.top

Java: synchronized (this) { shared++; }
来源：http://rsp.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://evb.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pww.jqgufenzy.top

C#:   lock (gate) { shared++; }
来源：http://xvj.pycfn.com

[O04] 定义异步函数并等待
来源：http://etv.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://ori.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ztt.pengpengdd.cyou

JS:   async function f() { await g(); }
来源：http://dsi.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://den.yj20258888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://voj.sjlbkw.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mud.zdbjq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tvm.bbcook.cn

C#:   async Task F() { await G(); }
来源：http://xop.redwolf501.top

[O05] 并发执行并等待全部完成
来源：http://jzv.ivvv.top

Py:   asyncio.gather(*tasks)
来源：http://yny.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dqw.shangyingyoupin.top

JS:   await Promise.all(tasks)
来源：http://buw.xuetiantiany.cn

TS:   await Promise.all(tasks)
来源：http://tvc.wangdashe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mek.zhengqikj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cpv.zycfv.cn

Ruby: threads.map(&:join)
来源：http://lqe.yangfankeji.com

C#:   await Task.WhenAll(t1, t2)
来源：http://tmp.sufxvd.cn

[O06] 使用进程池
来源：http://ivw.ydjk.org.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ech.bbcook.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lyo.hcnkem.com

JS:   // child_process / cluster 模块
来源：http://ltz.dashuyun.cn

TS:   // child_process / cluster 模块
来源：http://ztv.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oqg.jiagoushi.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nnj.hesvh.cn

Ruby: // fork 块
来源：http://rxv.ppjwa.cn

C#:   Parallel.For
来源：http://dkd.gotoacloud.top

================================================================================
来源：http://mod.yvedp.cn

P. 常用工具函数
来源：http://ewl.aizwys.cn

================================================================================
来源：http://yuo.shanyushiyangtech.top

[P01] 生成 UUID
来源：http://jxu.daria6918.cn

Py:   str(uuid.uuid4())
来源：http://lku.dashuyun.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cue.ivvv.top

JS:   crypto.randomUUID()
来源：http://gnw.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://oms.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://jce.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://vur.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://zaw.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://gzw.fktsv.cn

[P02] MD5 / SHA256 摘要
来源：http://puk.tanke756.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cbq.uphjek.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://gmh.yonumen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aml.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pjb.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sby.hesvh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jgp.yj20258.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pce.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://afh.jqgfzy.top

[P03] 生成短随机字符串
来源：http://kbc.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hvq.hongshengwenyu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jxk.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fxl.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tcp.sxryk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xci.havefunace.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ncy.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fnw.jinqigufen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iry.cqqwz.cn

[P04] 求长度
来源：http://nsx.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qea.aibaodan.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ztc.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oyv.meibo888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fkl.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://obm.316326.xyz

Go:   len(arr);  len(m)
来源：http://uto.nanxinkj.top

Ruby: x.length;  x.size
来源：http://zle.birdmap.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://owk.jlsjyb.cn

[P05] 判断两个对象内容是否相等
来源：http://xuq.yfazqb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://vby.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://luh.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tbu.c1oappe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bxe.yongpay.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://inq.yfazqb.com

Go:   reflect.DeepEqual(a, b)
来源：http://cvh.fanxiaobao.xyz

Ruby: a == b
来源：http://rnj.pengpengdd.cyou

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kji.fanxiaobao.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qnm.hnxiangtu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nxz.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://lzp.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zdh.ivvv.top

TS:   if (x == null) {}
来源：http://zfj.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pxq.yuanzhike.top

Go:   if x == nil {}
来源：http://eev.yangfankeji.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vuo.zhijiandao.cn

C#:   if (x is null) {}
来源：http://qss.ybcxt.top

[P07] 防抖与节流
来源：http://yas.havefunace.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://trk.gogol.net.cn

PHP:  // 手写时间戳比较
来源：http://rwv.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://njt.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wpi.chenlongwang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wdt.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pnc.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mih.jqgufenzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://okm.jqgufenzy.top

[P08] 处理浮点精度问题
来源：http://hzb.redwolf501.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ydc.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vul.cqqwz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kja.xziqi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pap.pycfn.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vcx.meibo888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://usg.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rcl.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cye.hongshengwenyu.top

================================================================================
来源：http://kyk.ydjk.org.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://djt.xingfuxueyuan.xyz

================================================================================
来源：http://vnv.bjfxy.top

[Q01] 创建表
来源：http://uuw.yangfankeji.com

CREATE TABLE users (
来源：http://fuo.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qzj.bjfxy.top

name VARCHAR(50) NOT NULL,
来源：http://opl.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://ugq.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aih.shangyingyoupin.top

);
来源：http://iqr.wangshuangyany.cn

[Q02] 创建带外键的表
来源：http://wqy.hesvh.cn

CREATE TABLE orders (
来源：http://ohg.tanke756.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yyy.vqdsnc.cn

user_id INT NOT NULL,
来源：http://uye.hongshengwenyu.top

amount DECIMAL(10, 2),
来源：http://zno.zdqjudy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ahs.sysykeji.top

);
来源：http://tcl.chenjidiqi.icu

[Q03] 增加列
来源：http://hrl.jlsjyb.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://luy.shzxlz.cn

[Q04] 修改列类型
来源：http://jmp.havefunace.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ouq.zhoulong.xyz

[Q05] 重命名列
来源：http://gvg.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wue.xziqi.cn

[Q06] 删除列
来源：http://yun.fengsongda.top

ALTER TABLE users DROP COLUMN age;
来源：http://yvq.zycfv.cn

[Q07] 删除表
来源：http://hbj.uphjek.com

DROP TABLE IF EXISTS orders;
来源：http://zva.mhx1999.top

[Q08] 创建普通索引
来源：http://pnc.chenlongwang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://uaz.haohaochexian.top

[Q09] 创建唯一索引
来源：http://aui.hysaishi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yeu.wangshuangyany.cn

[Q10] 插入单行
来源：http://euu.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ocd.chenzaomai.com

[Q11] 一次插入多行
来源：http://qea.snrcjt.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hlb.zdqjudy.top

[Q12] 插入后取自增 ID
来源：http://zmc.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://cgy.aizwys.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nkz.zhixingplan.top

[Q13] 忽略重复插入
来源：http://gmy.gaohongyu789.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ceu.jiagoushi.top

[Q14] 存在则更新（upsert）
来源：http://hsl.tianlin.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qlc.tian-w.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://daj.wangshuangyany.cn

[Q15] 查询全部
来源：http://ufp.sysykeji.top

SELECT * FROM users;
来源：http://kwd.shzxlz.cn

[Q16] 查询指定列
来源：http://lnx.aizwys.cn

SELECT id, name FROM users;
来源：http://zbm.zhijiandao.cn

[Q17] 条件查询
来源：http://zrt.shangyingyoupin.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iij.ivvv.top

[Q18] 模糊匹配
来源：http://xpk.jqgfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ppj.xinyue.icu

[Q19] 范围查询
来源：http://bqy.chenlongwang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://byd.52xcode.cn

[Q20] IN 列表
来源：http://yri.jyoumei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cwx.sxryk.cn

[Q21] 空值判断
来源：http://lkl.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://boj.shzxlz.cn

[Q22] 排序
来源：http://ebb.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ncy.52xcode.cn

[Q23] 分页
来源：http://bmm.pycfn.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mve.gzhubu.top

[Q24] 去重
来源：http://wmi.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://ncn.yfazqb.com

[Q25] 只取前 N 条
来源：http://ood.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://okl.zdqjudy.top

[Q26] 计数
来源：http://yoe.hnxiangtu.top

SELECT COUNT(*) FROM users;
来源：http://blf.cdnleiting.top

[Q27] 条件计数
来源：http://dhi.fanxiaobao.xyz


<!-- 参考信息 -->