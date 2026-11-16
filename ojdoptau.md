代发 wailian999

TS:   process.platform;  process.version
来源：http://gnd.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nhe.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://lxz.52xcode.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fpw.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gfm.hywenlv.cn

================================================================================
来源：http://nkj.jiagoushi.top

N. 数据结构与算法
来源：http://hoe.0kj1m.cn

================================================================================
来源：http://sfc.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://nqr.zhixingplan.top

Py:   bisect.bisect_left(arr, x)
来源：http://vdw.hongshengwenyu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wnu.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bpy.tianlin.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xuh.xziqi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://czx.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://wge.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wfd.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://lgq.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://bgq.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://nsy.snrcjt.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tdj.jiagoushi.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lmr.bbcook.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://uim.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://paz.meibo888.top

Go:   slices.Sort(arr)
来源：http://ymf.mhx1999.top

Ruby: arr.sort
来源：http://niu.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://zzl.cqqwz.cn

[N03] 快速排序（分治示例）
来源：http://xad.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zmz.yangfankeji.com

PHP:  // 递归实现，或用 usort
来源：http://wal.jqgufenzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jif.sufxvd.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bsh.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vbx.jqgufenzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://quk.iojbl.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zwt.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ahc.bbcook.cn

[N04] 斐波那契数列
来源：http://spg.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dwr.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fjs.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vpl.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wem.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kwa.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://phu.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://swd.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vzy.kuanghao11.cn

[N05] 最大公约数
来源：http://amo.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://lzd.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bhg.zhijiandao.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ffn.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qeh.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zls.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nyo.wangshuangyany.cn

Ruby: a.gcd(b)
来源：http://qdy.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cgp.sufxvd.cn

[N06] 判断回文字符串
来源：http://uai.birdmap.top

Py:   s == s[::-1]
来源：http://chx.xziqi.cn

PHP:  $s === strrev($s);
来源：http://wiw.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://xzx.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://hwz.yangfankeji.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ger.feifeiyinyue.top

Go:   // 双指针从两端比较
来源：http://inc.aizwys.cn

Ruby: s == s.reverse
来源：http://rmo.sjlbkw.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tip.zycfv.cn

[N07] 两数之和（返回下标）
来源：http://ayd.daria6918.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iwi.jqgufenzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jbl.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hhn.hcnkem.com

TS:   // 手写 Map<string, number>
来源：http://fdz.hcnkem.com

Java: // 手写 HashMap
来源：http://bjy.jqgfzy.top

Go:   // 手写 map[int]int
来源：http://hit.cheryme.top

Ruby: // 手写 Hash
来源：http://jjv.cucudq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ipe.ydzc1.top

[N08] 生成全排列
来源：http://zky.kuanghao11.cn

Py:   itertools.permutations(arr)
来源：http://iii.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://cwk.shuidangran.top

JS:   // 手写回溯递归
来源：http://wcv.iojbl.cn

TS:   // 手写回溯递归
来源：http://jim.haohaochexian.top

Java: // 手写回溯递归
来源：http://bdp.yj20258.top

Go:   // 手写回溯递归
来源：http://xhm.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://hsr.cheryme.top

C#:   // 手写回溯递归
来源：http://ftg.tanke756.top

[N09] 栈与队列
来源：http://jnv.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oaq.hammf.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fjx.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yad.zhiwuduotai.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nls.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cmw.zhaomingkeji.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mcj.bbcook.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ymd.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jbk.gogol.net.cn

[N10] 链表节点定义
来源：http://dji.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vhn.hywenlv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://spg.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vit.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jvq.ywan-chungtsiang.top

Java: class Node { int v; Node next; }
来源：http://iyo.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://uod.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xfs.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://uwd.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://kzl.chenlongwang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sau.fktsv.cn

PHP:  // 手写递归函数
来源：http://eei.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vjz.shangyingyoupin.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mxp.chenjidiqi.icu

Java: // 手写递归
来源：http://vxd.ydjk.org.cn

Go:   // 手写递归
来源：http://uvm.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tsj.gotoacloud.top

C#:   // 手写递归
来源：http://oyy.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ovh.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qmu.sysykeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lvl.hfpthk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ady.zhijiandao.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dcb.jqgufenzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://caw.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cml.shanyushiyangtech.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vmp.hcnkem.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pwy.shuidangran.top

================================================================================
来源：http://rad.zhiwuduotai.top

O. 并发与异步
来源：http://uwf.ehwqpu.com

================================================================================
来源：http://eup.yj20258888.top

[O01] 启动一个线程
来源：http://wxo.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bdn.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gqq.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cwe.chenlongwang.top

TS:   // 同 JS
来源：http://jsu.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://dut.cashguo.top

Go:   go f()
来源：http://gbw.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://ycf.cucudq.cn

C#:   Task.Run(() => F());
来源：http://ibj.chenjidiqi.icu

[O02] 使用线程池
来源：http://eyx.vehdjk.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vot.tanke756.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ewr.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://utz.svipenyu.cn

TS:   // worker_threads 线程池
来源：http://aqr.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://xpf.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eju.yongpay.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ikz.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://thv.gotoacloud.top

[O03] 加锁保护共享数据
来源：http://yne.52xcode.cn

Py:   with lock: shared += 1
来源：http://dhn.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://mfg.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wky.epnwcf.com

TS:   // 同 JS
来源：http://bqz.fengsongda.top

Java: synchronized (this) { shared++; }
来源：http://taf.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hkx.zhoulong.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://hnj.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://izv.quarkkingdee.top

[O04] 定义异步函数并等待
来源：http://hhu.vehdjk.com

Py:   async def f():⏎    await g()
来源：http://ydz.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fvs.cheryme.top

JS:   async function f() { await g(); }
来源：http://hqn.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://itm.tian-w.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yzq.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ghe.0kj1m.cn

Ruby: # 用 Fiber 或 async gem
来源：http://akp.bbcook.cn

C#:   async Task F() { await G(); }
来源：http://mda.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://cyi.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://rrp.zdbjq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eqf.snrcjt.cn

JS:   await Promise.all(tasks)
来源：http://ziu.gotoacloud.top

TS:   await Promise.all(tasks)
来源：http://gud.gaohongyu789.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hpn.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bbj.xuanzx.com

Ruby: threads.map(&:join)
来源：http://gns.bjfxy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://taq.daria6918.cn

[O06] 使用进程池
来源：http://riu.gzhubu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jmz.yongpay.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hje.yonumen.top

JS:   // child_process / cluster 模块
来源：http://nxc.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://uwq.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gjq.fanxiaobao.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://von.havefunace.top

Ruby: // fork 块
来源：http://vlh.yangfankeji.com

C#:   Parallel.For
来源：http://kin.fktsv.cn

================================================================================
来源：http://owb.hcnkem.com

P. 常用工具函数
来源：http://xad.zdqjudy.top

================================================================================
来源：http://ceb.kuanghao11.cn

[P01] 生成 UUID
来源：http://val.yj202588.top

Py:   str(uuid.uuid4())
来源：http://gdk.tarul.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rhp.shuidangran.top

JS:   crypto.randomUUID()
来源：http://pbm.fengsongda.top

TS:   crypto.randomUUID()
来源：http://iah.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://frt.daxiang520.top

Go:   // 用 github.com/google/uuid
来源：http://udq.jyoumei.cn

Ruby: SecureRandom.uuid
来源：http://klf.smart0.xyz

C#:   Guid.NewGuid().ToString()
来源：http://zjb.c1oappe.top

[P02] MD5 / SHA256 摘要
来源：http://uak.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://acm.daria6918.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://knr.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aas.kuanghao11.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://okc.yj20258888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://irl.nanxinkj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vep.zycfv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ayd.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bhk.yueranfly.top

[P03] 生成短随机字符串
来源：http://xnh.ybcxt.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mcu.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pge.shanyushiyangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hlf.mhx1999.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ytg.tarul.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zoh.hongshengwenyu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://alj.pengpengdd.cyou

Ruby: SecureRandom.alphanumeric(16)
来源：http://bak.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hje.chenlongwang.top

[P04] 求长度
来源：http://nnc.yj20258.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zbi.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nky.shzxlz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xtp.feifeiyinyue.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kqx.ppjwa.cn

Java: list.size();  map.size();  s.length()
来源：http://alq.daxiang520.top

Go:   len(arr);  len(m)
来源：http://jfj.cucudq.cn

Ruby: x.length;  x.size
来源：http://fcc.jianghu66.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wyr.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://jrt.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uoa.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://igt.jinghuilouyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yiu.zhiwuduotai.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zhg.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ftq.sweek.top

Go:   reflect.DeepEqual(a, b)
来源：http://shq.guannengcc.top

Ruby: a == b
来源：http://wqy.zhoulong.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ami.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://prn.cucudq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bnr.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://dzx.ppjwa.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vkd.gzhubu.top

TS:   if (x == null) {}
来源：http://jue.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cfc.zhijiandao.cn

Go:   if x == nil {}
来源：http://jgr.sweek.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rnp.hnqzz.top

C#:   if (x is null) {}
来源：http://jcw.dianchejie.cn

[P07] 防抖与节流
来源：http://kcp.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://grj.hammf.cn

PHP:  // 手写时间戳比较
来源：http://vdn.xziqi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lsg.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lbt.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hws.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bsg.ybcxt.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dov.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cok.daxiang520.top

[P08] 处理浮点精度问题
来源：http://gtg.jqgufenzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eac.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yte.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kbc.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tur.xinyue.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ttf.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://slj.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gzy.cucudq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hte.cqqwz.cn

================================================================================
来源：http://cgi.svipenyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qnf.xinyue.icu

================================================================================
来源：http://zov.smart0.xyz

[Q01] 创建表
来源：http://vss.xziqi.cn

CREATE TABLE users (
来源：http://gdq.hywenlv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://otj.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://jbp.zhixingplan.top

email VARCHAR(100) UNIQUE,
来源：http://dnu.hnxiangtu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dgq.epnwcf.com

);
来源：http://wqs.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://rhi.jiagoushi.top

CREATE TABLE orders (
来源：http://ouv.bjfxy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qkv.jiagoushi.top

user_id INT NOT NULL,
来源：http://dut.xuanzx.com

amount DECIMAL(10, 2),
来源：http://ctp.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uhu.guannengcc.top

);
来源：http://fza.jlsjyb.cn

[Q03] 增加列
来源：http://ocu.aibaodan.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ovo.fehbvm.com

[Q04] 修改列类型
来源：http://loz.feifeiyinyue.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ryi.bjfxy.top

[Q05] 重命名列
来源：http://ajo.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nrn.fanxiaobao.xyz

[Q06] 删除列
来源：http://bux.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://flq.fehbvm.com

[Q07] 删除表
来源：http://igf.zdqjudy.top

DROP TABLE IF EXISTS orders;
来源：http://osc.shanyushiyangtech.top

[Q08] 创建普通索引
来源：http://qrr.cdnleiting.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xhc.hesvh.cn

[Q09] 创建唯一索引
来源：http://bmd.wangdashe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://avd.cdnleiting.top

[Q10] 插入单行
来源：http://hrm.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xht.fanxiaobao.xyz

[Q11] 一次插入多行
来源：http://aiy.zycfv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uvu.iojbl.cn

[Q12] 插入后取自增 ID
来源：http://ims.guannengcc.top

INSERT INTO users (name) VALUES ('C');
来源：http://kqf.aibaodan.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pyi.yongpay.top

[Q13] 忽略重复插入
来源：http://eor.meibo888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rlk.tianlin.xyz

[Q14] 存在则更新（upsert）
来源：http://mqr.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hct.jqgufenzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blj.yj202588.top

[Q15] 查询全部
来源：http://wfb.fzhhl.top

SELECT * FROM users;
来源：http://mie.vehdjk.com

[Q16] 查询指定列
来源：http://ews.andypj.xyz

SELECT id, name FROM users;
来源：http://rde.jinqigfzy.top

[Q17] 条件查询
来源：http://krk.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dgw.dashuyun.cn

[Q18] 模糊匹配
来源：http://wcq.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hgc.guannengcc.top

[Q19] 范围查询
来源：http://cvt.shanyushiyangtech.top


<!-- 参考信息 -->