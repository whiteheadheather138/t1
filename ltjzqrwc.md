代发 wailian999

[M08] 获取系统与运行时信息
来源：http://dak.cashguo.top

Py:   platform.system();  platform.python_version()
来源：http://djv.hnxiangtu.top

PHP:  PHP_OS;  phpversion();
来源：http://hdu.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://fnb.gzhubu.top

TS:   process.platform;  process.version
来源：http://uaz.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aup.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vli.yueranfly.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tnv.daria6918.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hdd.jinghuilouyu.cn

================================================================================
来源：http://fyr.hfpthk.cn

N. 数据结构与算法
来源：http://jlh.fzhhl.top

================================================================================
来源：http://xvw.chenlongwang.top

[N01] 二分查找（有序数组）
来源：http://luf.fehbvm.com

Py:   bisect.bisect_left(arr, x)
来源：http://kup.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ogn.xingfuxueyuan.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://spj.cheryme.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rmv.52xcode.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ezt.ctjpmb.com

Go:   sort.SearchInts(arr, x)
来源：http://kaf.birdmap.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ixx.sufxvd.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rhm.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://xjo.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://wzy.shanyushiyangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://biq.aibaodan.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pwc.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://slc.jinqigfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dnt.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://mnt.xziqi.cn

Ruby: arr.sort
来源：http://ron.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://lgn.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://vfw.smart0.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vik.shanyushiyangtech.top

PHP:  // 递归实现，或用 usort
来源：http://vuc.yonumen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ufl.ydjk.org.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bdu.yj20258.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qqy.yfazqb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lox.quarkkingdee.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dob.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://yyc.tian-w.cn

[N04] 斐波那契数列
来源：http://tkl.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lau.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ato.sweek.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vyr.yj20258888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ldm.jqgufenzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uao.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qry.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ibm.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ozm.chenjidiqi.icu

[N05] 最大公约数
来源：http://oxk.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://xzf.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://axx.chenzaomai.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qnv.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gnh.tian-w.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jvn.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sft.kuanghao11.cn

Ruby: a.gcd(b)
来源：http://xfm.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jik.haohaochexian.top

[N06] 判断回文字符串
来源：http://cwe.yonumen.top

Py:   s == s[::-1]
来源：http://shh.shanyushiyangtech.top

PHP:  $s === strrev($s);
来源：http://ssd.jqgufenzy.top

JS:   s === [...s].reverse().join("")
来源：http://fkg.ppjwa.cn

TS:   s === [...s].reverse().join("")
来源：http://zeu.yvedp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://upi.ivvv.top

Go:   // 双指针从两端比较
来源：http://qfi.yj20258.top

Ruby: s == s.reverse
来源：http://tzo.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vic.epnwcf.com

[N07] 两数之和（返回下标）
来源：http://uzv.ppjwa.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://emo.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://whw.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zxl.gogol.net.cn

TS:   // 手写 Map<string, number>
来源：http://ryj.ydjk.org.cn

Java: // 手写 HashMap
来源：http://csa.xziqi.cn

Go:   // 手写 map[int]int
来源：http://mlp.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://dbe.zycfv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://spl.meibo888.top

[N08] 生成全排列
来源：http://uko.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://wjc.yangfankeji.com

PHP:  // 手写递归交换
来源：http://ipv.ydzc1.top

JS:   // 手写回溯递归
来源：http://zxv.bjfxy.top

TS:   // 手写回溯递归
来源：http://uhk.havefunace.top

Java: // 手写回溯递归
来源：http://yhx.zhoulong.xyz

Go:   // 手写回溯递归
来源：http://vzk.pengpengdd.cyou

Ruby: arr.permutation.to_a
来源：http://ryu.c1oappe.top

C#:   // 手写回溯递归
来源：http://ecj.zhijiandao.cn

[N09] 栈与队列
来源：http://cke.jinqigufen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hzt.cucudq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://asm.hfpthk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pjy.fengsongda.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vfd.dashuyun.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lte.zhiwuduotai.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xbs.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oon.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://izm.gzhubu.top

[N10] 链表节点定义
来源：http://enk.tanke756.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qyj.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gky.dianchejie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qeb.yvedp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xbi.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://psh.feifeiyinyue.top

Go:   type Node struct { V int; Next *Node }
来源：http://szd.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uqj.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lrb.vqdsnc.cn

[N11] 二叉树中序遍历
来源：http://olb.jqgfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nzg.daria6918.cn

PHP:  // 手写递归函数
来源：http://nko.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nzf.shangyingyoupin.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ved.hywenlv.cn

Java: // 手写递归
来源：http://aay.meibo888.top

Go:   // 手写递归
来源：http://jpy.guowangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fve.jiagoushi.top

C#:   // 手写递归
来源：http://xjq.yueranfly.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lwf.chenzaomai.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bhk.tanke756.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xom.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uvk.snrcjt.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://exk.yj20258888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qmb.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rtq.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ixa.chenjidiqi.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zpu.epnwcf.com

================================================================================
来源：http://zsa.birdmap.top

O. 并发与异步
来源：http://mbi.quarkkingdee.top

================================================================================
来源：http://guf.sufxvd.cn

[O01] 启动一个线程
来源：http://lfu.feifeiyinyue.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dde.havefunace.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://muj.birdmap.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vnj.yongpay.top

TS:   // 同 JS
来源：http://yxw.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://kuj.jlsjyb.cn

Go:   go f()
来源：http://ytt.shanyushiyangtech.top

Ruby: Thread.new { f }
来源：http://dgn.zhongyouzk.top

C#:   Task.Run(() => F());
来源：http://hfu.xziqi.cn

[O02] 使用线程池
来源：http://kdp.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mke.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://miz.zhongyouzk.top

JS:   // worker_threads 线程池
来源：http://yux.pycfn.com

TS:   // worker_threads 线程池
来源：http://lsm.zdbjq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nka.zdqjudy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nqt.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ipz.9152youxi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hvu.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://pwv.jinqigufen.top

Py:   with lock: shared += 1
来源：http://utb.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://jos.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yiu.sufxvd.cn

TS:   // 同 JS
来源：http://weo.vqdsnc.cn

Java: synchronized (this) { shared++; }
来源：http://fni.sxryk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sza.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vod.tanke756.top

C#:   lock (gate) { shared++; }
来源：http://pyd.hnqzz.top

[O04] 定义异步函数并等待
来源：http://qoh.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://csu.52xcode.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lyy.jqgfzy.top

JS:   async function f() { await g(); }
来源：http://mvk.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bov.52xcode.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rqz.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dry.jinqigfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://vxp.fengsongda.top

C#:   async Task F() { await G(); }
来源：http://qlz.zhijiandao.cn

[O05] 并发执行并等待全部完成
来源：http://qsy.aizwys.cn

Py:   asyncio.gather(*tasks)
来源：http://iox.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://htd.jinqigfzy.top

JS:   await Promise.all(tasks)
来源：http://lho.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://iyc.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dmr.hnxiangtu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tbi.gaohongyu789.top

Ruby: threads.map(&:join)
来源：http://snn.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nlv.zhijiandao.cn

[O06] 使用进程池
来源：http://cqi.cqqwz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kti.gaohongyu789.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zki.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://mbl.wangdashe.top

TS:   // child_process / cluster 模块
来源：http://kyj.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pen.zhiwuduotai.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://guz.ybcxt.top

Ruby: // fork 块
来源：http://jsc.quarkkingdee.top

C#:   Parallel.For
来源：http://gqi.nanxinkj.top

================================================================================
来源：http://onn.hywenlv.cn

P. 常用工具函数
来源：http://qit.bjfxy.top

================================================================================
来源：http://qvh.zhijiandao.cn

[P01] 生成 UUID
来源：http://euw.hfpthk.cn

Py:   str(uuid.uuid4())
来源：http://gzg.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wbk.nwbrower.top

JS:   crypto.randomUUID()
来源：http://poq.pycfn.com

TS:   crypto.randomUUID()
来源：http://cnm.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://rea.jlsjyb.cn

Go:   // 用 github.com/google/uuid
来源：http://hwp.yangfankeji.com

Ruby: SecureRandom.uuid
来源：http://xsl.pengpengdd.cyou

C#:   Guid.NewGuid().ToString()
来源：http://jpz.vehdjk.com

[P02] MD5 / SHA256 摘要
来源：http://jog.zhaomingkeji.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jfq.daria6918.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rwa.yuxming.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://acn.vqdsnc.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cay.fanxiaobao.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dpv.sjlbkw.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pyh.havefunace.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://psi.hnqzz.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://byg.wangdashe.top

[P03] 生成短随机字符串
来源：http://ydj.wangshuangyany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ckx.guowangkeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hll.uphjek.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ttm.chenjidiqi.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://woe.hfpthk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mxn.havefunace.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jzt.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hbe.xuanzx.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vqq.fktsv.cn

[P04] 求长度
来源：http://vxs.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://npy.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ktd.gogol.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nwb.xziqi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dub.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://zni.meibo888.top

Go:   len(arr);  len(m)
来源：http://enh.yj20258.top

Ruby: x.length;  x.size
来源：http://pkx.quarkkingdee.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yzo.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://yvm.yuxming.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kmi.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rwp.wangshuangyany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://grd.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ucm.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zkc.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gyq.yanxiufei.cn

Ruby: a == b
来源：http://sht.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xpl.redwolf501.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tve.yanxiufei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qph.jqgufenzy.top

PHP:  if (empty($x)) {}
来源：http://fft.c1oappe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jgh.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://dpw.shangyingyoupin.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kos.tian-w.cn

Go:   if x == nil {}
来源：http://kvp.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cei.zhengqikj.top

C#:   if (x is null) {}
来源：http://dgi.redwolf501.top

[P07] 防抖与节流
来源：http://utc.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cnm.uphjek.com

PHP:  // 手写时间戳比较
来源：http://kmr.zhiwuduotai.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pvs.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wff.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jbh.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qzt.bbcook.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fyk.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jfa.feifeiyinyue.top

[P08] 处理浮点精度问题
来源：http://jha.hywenlv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sum.shanyushiyangtech.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yzm.guannengcc.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ija.gogol.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bdc.nwbrower.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wjt.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wjs.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kcr.hcnkem.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fup.cheryme.top

================================================================================
来源：http://ynu.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://haj.ctjpmb.com

================================================================================
来源：http://yzb.zdqjudy.top

[Q01] 创建表
来源：http://oqp.dianchejie.cn

CREATE TABLE users (
来源：http://wcn.yongpay.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jby.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://gln.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://tfy.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cgd.zhaomingkeji.xyz

);
来源：http://fwu.aibaodan.cn

[Q02] 创建带外键的表
来源：http://ibi.xziqi.cn

CREATE TABLE orders (
来源：http://jfe.quarkkingdee.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://csz.gaohongyu789.top

user_id INT NOT NULL,
来源：http://qnw.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://guz.cheryme.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fxg.fzhhl.top

);
来源：http://qkd.sxryk.cn

[Q03] 增加列
来源：http://kdg.hongshengwenyu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://msb.hongshengwenyu.top

[Q04] 修改列类型
来源：http://uhw.zdbjq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ycv.sufxvd.cn

[Q05] 重命名列
来源：http://kht.jiagoushi.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://edf.zycfv.cn

[Q06] 删除列
来源：http://vqu.sysykeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://rjv.0kj1m.cn

[Q07] 删除表
来源：http://zon.birdmap.top

DROP TABLE IF EXISTS orders;
来源：http://vmq.shzxlz.cn

[Q08] 创建普通索引
来源：http://xvi.xuanzx.com

CREATE INDEX idx_users_email ON users(email);
来源：http://syb.cqqwz.cn

[Q09] 创建唯一索引
来源：http://szn.0kj1m.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ckj.jqgufenzy.top

[Q10] 插入单行
来源：http://sfz.gogol.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ndv.vqdsnc.cn

[Q11] 一次插入多行
来源：http://iym.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jls.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://qvk.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://ssu.yj20258888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gpn.dashuyun.cn

[Q13] 忽略重复插入
来源：http://evh.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fap.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://ckt.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://acz.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gkq.tanke756.top

[Q15] 查询全部
来源：http://juc.yvedp.cn

SELECT * FROM users;
来源：http://pnr.hcnkem.com

[Q16] 查询指定列
来源：http://pvb.dianchejie.cn

SELECT id, name FROM users;
来源：http://vyy.xingfuxueyuan.xyz

[Q17] 条件查询
来源：http://tur.dashuyun.cn


<!-- 参考信息 -->