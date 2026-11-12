代发 wailian999

TS:   process.platform;  process.version
来源：http://cux.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mdp.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://daf.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dwm.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://omd.yj20258.top

================================================================================
来源：http://jss.guannengcc.top

N. 数据结构与算法
来源：http://iny.hywenlv.cn

================================================================================
来源：http://ctt.xinyue.icu

[N01] 二分查找（有序数组）
来源：http://zer.sysykeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://yrg.9152youxi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ilo.zhiwuduotai.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rgc.xingfuxueyuan.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cwk.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://xhn.uphjek.com

Go:   sort.SearchInts(arr, x)
来源：http://syd.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://bpj.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://knc.sweek.top

[N02] 排序（工程实践用内置实现）
来源：http://cpd.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://suh.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://laq.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hqq.316326.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://bgp.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wrx.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://cba.shzxlz.cn

Ruby: arr.sort
来源：http://xcr.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://xju.haohaochexian.top

[N03] 快速排序（分治示例）
来源：http://ihb.nanxinkj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uwm.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://pah.hywenlv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://flj.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pvw.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zyq.yueranfly.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jjq.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qjj.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://rcn.sweek.top

[N04] 斐波那契数列
来源：http://eme.zhiwuduotai.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hiu.shangyingyoupin.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yfg.yuxming.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ebc.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gct.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ieu.zhongyouzk.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zav.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wee.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qoj.aibaodan.cn

[N05] 最大公约数
来源：http://axg.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://lrf.xylfe.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aqm.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bre.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hsl.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yco.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://prx.birdmap.top

Ruby: a.gcd(b)
来源：http://acv.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rip.jinqigfzy.top

[N06] 判断回文字符串
来源：http://esl.tanke756.top

Py:   s == s[::-1]
来源：http://mnv.52xcode.cn

PHP:  $s === strrev($s);
来源：http://xvp.jqgfzy.top

JS:   s === [...s].reverse().join("")
来源：http://dyd.chenlongwang.top

TS:   s === [...s].reverse().join("")
来源：http://gnt.ctjpmb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cni.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://shc.hongshengwenyu.top

Ruby: s == s.reverse
来源：http://cfp.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cqq.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://wti.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yoo.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://egr.pycfn.com

JS:   // 手写 Map：map.set(v, i)
来源：http://xjr.gogol.net.cn

TS:   // 手写 Map<string, number>
来源：http://cfh.shangyingyoupin.top

Java: // 手写 HashMap
来源：http://dkd.cashguo.top

Go:   // 手写 map[int]int
来源：http://zsa.cqqwz.cn

Ruby: // 手写 Hash
来源：http://tdg.shanyushiyangtech.top

C#:   // 手写 Dictionary<int, int>
来源：http://zdg.hcnkem.com

[N08] 生成全排列
来源：http://rsn.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://gfq.jyoumei.cn

PHP:  // 手写递归交换
来源：http://prn.yueranfly.top

JS:   // 手写回溯递归
来源：http://zir.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://vny.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://bte.aizwys.cn

Go:   // 手写回溯递归
来源：http://gva.ywan-chungtsiang.top

Ruby: arr.permutation.to_a
来源：http://pon.hnqzz.top

C#:   // 手写回溯递归
来源：http://vkj.ydzc1.top

[N09] 栈与队列
来源：http://aps.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://txh.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://esb.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yud.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://byp.yuxming.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oyn.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aht.epnwcf.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://plw.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qdv.yangfankeji.com

[N10] 链表节点定义
来源：http://xfs.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zbf.ppjwa.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xsk.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://buf.svipenyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vnd.ydzc1.top

Java: class Node { int v; Node next; }
来源：http://qsj.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://svq.aizwys.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://job.bbcook.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gah.gzhubu.top

[N11] 二叉树中序遍历
来源：http://pzy.zhongyouzk.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cvl.hysaishi.cn

PHP:  // 手写递归函数
来源：http://gns.yonumen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://poz.yanxiufei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vzl.cqqwz.cn

Java: // 手写递归
来源：http://mml.yanxiufei.cn

Go:   // 手写递归
来源：http://erw.tian-w.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ivq.meibo888.top

C#:   // 手写递归
来源：http://wtt.gzhubu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zmk.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ofz.yvedp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cuv.havefunace.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rax.yuanzhike.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iik.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mxb.chenlongwang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zml.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kyo.chenzaomai.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ixw.sxryk.cn

================================================================================
来源：http://lmr.vqdsnc.cn

O. 并发与异步
来源：http://mcg.nanxuanxn.top

================================================================================
来源：http://xuz.zhaomingkeji.xyz

[O01] 启动一个线程
来源：http://spt.ydjk.org.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hyn.jinqigfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pno.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dru.gaohongyu789.top

TS:   // 同 JS
来源：http://xig.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://sun.fehbvm.com

Go:   go f()
来源：http://uar.hcnkem.com

Ruby: Thread.new { f }
来源：http://xes.smart0.xyz

C#:   Task.Run(() => F());
来源：http://roa.yangfankeji.com

[O02] 使用线程池
来源：http://keu.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wkv.ybcxt.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blu.zhaomingkeji.xyz

JS:   // worker_threads 线程池
来源：http://rco.yuanzhike.top

TS:   // worker_threads 线程池
来源：http://nli.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tgp.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ruz.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kff.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lxp.andypj.xyz

[O03] 加锁保护共享数据
来源：http://hoq.ctjpmb.com

Py:   with lock: shared += 1
来源：http://hre.meibo888.top

PHP:  // 用 flock() 做文件锁
来源：http://caz.chenzaomai.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zhf.jqgufenzy.top

TS:   // 同 JS
来源：http://qnz.xuanzx.com

Java: synchronized (this) { shared++; }
来源：http://nfx.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iud.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://frg.jiagoushi.top

C#:   lock (gate) { shared++; }
来源：http://fnd.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://gvu.yuanzhike.top

Py:   async def f():⏎    await g()
来源：http://gyn.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://esv.nanxuanxn.top

JS:   async function f() { await g(); }
来源：http://cyy.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://boo.fzhhl.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://anc.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://okf.pycfn.com

Ruby: # 用 Fiber 或 async gem
来源：http://lye.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://ucv.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://cto.cdnleiting.top

Py:   asyncio.gather(*tasks)
来源：http://sta.jinyuanbaomall.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ist.svipenyu.cn

JS:   await Promise.all(tasks)
来源：http://akl.hesvh.cn

TS:   await Promise.all(tasks)
来源：http://zir.quarkkingdee.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ezh.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://epx.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://aum.hnxiangtu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bnb.jianghu66.top

[O06] 使用进程池
来源：http://qvz.316326.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wdk.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yqc.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://dbl.jinqigufen.top

TS:   // child_process / cluster 模块
来源：http://suh.feifeiyinyue.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ndu.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tpp.tianlin.xyz

Ruby: // fork 块
来源：http://syg.sjlbkw.cn

C#:   Parallel.For
来源：http://zax.meibo888.top

================================================================================
来源：http://fgh.sufxvd.cn

P. 常用工具函数
来源：http://ufz.guowangkeji.top

================================================================================
来源：http://qkn.aizwys.cn

[P01] 生成 UUID
来源：http://vqe.zhixingplan.top

Py:   str(uuid.uuid4())
来源：http://yxl.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gnw.yonumen.top

JS:   crypto.randomUUID()
来源：http://fft.daxiang520.top

TS:   crypto.randomUUID()
来源：http://yeq.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://fvb.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://bsi.gzhubu.top

Ruby: SecureRandom.uuid
来源：http://yhw.xuanzx.com

C#:   Guid.NewGuid().ToString()
来源：http://dlb.fanxiaobao.xyz

[P02] MD5 / SHA256 摘要
来源：http://let.aizwys.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cum.shanyushiyangtech.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jxx.mhx1999.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lep.nanxinkj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ady.snrcjt.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bfq.xziqi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jiv.shanyushiyangtech.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qcg.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wvj.9152youxi.cn

[P03] 生成短随机字符串
来源：http://ter.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rpw.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://azk.tianlin.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cmp.shanyushiyangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ppv.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jhe.meibo888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dxp.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://afk.ydzc1.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://azx.jinqigufen.top

[P04] 求长度
来源：http://aym.hammf.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xxv.nanxinkj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rkq.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jfc.yuanzhike.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ods.gotoacloud.top

Java: list.size();  map.size();  s.length()
来源：http://vhx.redwolf501.top

Go:   len(arr);  len(m)
来源：http://ulp.zdqjudy.top

Ruby: x.length;  x.size
来源：http://qzy.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lcp.kuanghao11.cn

[P05] 判断两个对象内容是否相等
来源：http://lof.ydzc1.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zpt.hcnkem.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lrs.jyoumei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ssz.sxryk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vke.sysykeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ahm.fanxiaobao.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://vlv.haohaochexian.top

Ruby: a == b
来源：http://cpf.hammf.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bom.dashuyun.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://llt.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rxl.wangdashe.top

PHP:  if (empty($x)) {}
来源：http://diy.redwolf501.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oux.iojbl.cn

TS:   if (x == null) {}
来源：http://sbo.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vto.yuxming.cn

Go:   if x == nil {}
来源：http://yuw.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pbd.mhx1999.top

C#:   if (x is null) {}
来源：http://ruw.daria6918.cn

[P07] 防抖与节流
来源：http://jtp.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uig.iojbl.cn

PHP:  // 手写时间戳比较
来源：http://sll.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oka.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pvv.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ums.dashuyun.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ogv.xylfe.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sjp.zhongyouzk.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ohm.guowangkeji.top

[P08] 处理浮点精度问题
来源：http://rgl.yanxiufei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ygo.xylfe.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dlq.fanxiaobao.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dpc.chenlongwang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xgs.pengpengdd.cyou

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bif.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nco.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qnd.aizwys.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vpl.hnxiangtu.top

================================================================================
来源：http://whg.sxryk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qbt.hongshengwenyu.top

================================================================================
来源：http://nzp.andypj.xyz

[Q01] 创建表
来源：http://tfe.redwolf501.top

CREATE TABLE users (
来源：http://scf.xingfuxueyuan.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gzf.bjfxy.top

name VARCHAR(50) NOT NULL,
来源：http://ufo.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://vai.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rgf.cashguo.top

);
来源：http://lhr.vehdjk.com

[Q02] 创建带外键的表
来源：http://mal.sjlbkw.cn

CREATE TABLE orders (
来源：http://juu.cucudq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kqy.hongshengwenyu.top

user_id INT NOT NULL,
来源：http://sje.yj20258.top

amount DECIMAL(10, 2),
来源：http://qfh.iojbl.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ldk.xuanzx.com

);
来源：http://dop.chenzaomai.com

[Q03] 增加列
来源：http://nif.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jwe.shanyushiyangtech.top

[Q04] 修改列类型
来源：http://zwn.ywan-chungtsiang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://piv.jinqigfzy.top

[Q05] 重命名列
来源：http://kiv.yonumen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zqx.aibaodan.cn

[Q06] 删除列
来源：http://rlc.zhijiandao.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kdt.shzxlz.cn

[Q07] 删除表
来源：http://uqc.feifeiyinyue.top

DROP TABLE IF EXISTS orders;
来源：http://esb.xinyue.icu

[Q08] 创建普通索引
来源：http://fis.hnxiangtu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://epd.gaohongyu789.top

[Q09] 创建唯一索引
来源：http://feo.jiagoushi.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pku.chenzaomai.com

[Q10] 插入单行
来源：http://gms.xinyue.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eea.havefunace.top

[Q11] 一次插入多行
来源：http://wne.c1oappe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fds.yfazqb.com

[Q12] 插入后取自增 ID
来源：http://lbk.sysykeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://aye.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sqe.havefunace.top

[Q13] 忽略重复插入
来源：http://myj.ctjpmb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kem.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://apz.tianlin.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jwr.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kly.hysaishi.cn

[Q15] 查询全部
来源：http://unj.pengpengdd.cyou

SELECT * FROM users;
来源：http://gmz.zhiwuduotai.top

[Q16] 查询指定列
来源：http://bxt.hnqzz.top

SELECT id, name FROM users;
来源：http://osu.jqgfzy.top

[Q17] 条件查询
来源：http://ghq.chenjidiqi.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tto.hywenlv.cn

[Q18] 模糊匹配
来源：http://bmr.ivvv.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fgy.aibaodan.cn

[Q19] 范围查询
来源：http://wfc.dianchejie.cn


<!-- 参考信息 -->