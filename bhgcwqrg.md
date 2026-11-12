代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://acl.iojbl.cn

================================================================================
来源：http://gdk.gzhubu.top

N. 数据结构与算法
来源：http://jlc.52xcode.cn

================================================================================
来源：http://ccz.uphjek.com

[N01] 二分查找（有序数组）
来源：http://htb.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://blb.jiagoushi.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kvr.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zts.jinghuilouyu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bfm.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://hdp.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://aht.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mum.yj202588.top

C#:   Array.BinarySearch(arr, x)
来源：http://fms.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://sat.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://xks.jinqigufen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yoz.vehdjk.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://dib.fktsv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gcp.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://azs.shanyushiyangkeji.top

Go:   slices.Sort(arr)
来源：http://mxu.cheryme.top

Ruby: arr.sort
来源：http://qkg.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kar.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://bli.andypj.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nqa.havefunace.top

PHP:  // 递归实现，或用 usort
来源：http://gkq.hammf.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dqn.cqqwz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hib.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dyf.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dol.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://scj.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://egr.aizwys.cn

[N04] 斐波那契数列
来源：http://iub.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mrd.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mlw.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://exw.zhaomingkeji.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xgh.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zth.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gfn.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://urr.jlsjyb.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zxb.ydzc1.top

[N05] 最大公约数
来源：http://xur.hesvh.cn

Py:   math.gcd(a, b)
来源：http://zaf.jinqigufen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://art.fengsongda.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://abj.c1oappe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ddx.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://doa.hcnkem.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tzg.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://wqp.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lhs.daria6918.cn

[N06] 判断回文字符串
来源：http://ewk.tian-w.cn

Py:   s == s[::-1]
来源：http://fmz.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://zvr.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://dpm.hongshengwenyu.top

TS:   s === [...s].reverse().join("")
来源：http://lws.nanxinkj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yhx.ywan-chungtsiang.top

Go:   // 双指针从两端比较
来源：http://mpf.smart0.xyz

Ruby: s == s.reverse
来源：http://nlw.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kof.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://eiu.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wwn.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ify.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jkf.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://rxh.ywan-chungtsiang.top

Java: // 手写 HashMap
来源：http://gju.pycfn.com

Go:   // 手写 map[int]int
来源：http://gad.fengsongda.top

Ruby: // 手写 Hash
来源：http://pqe.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://aww.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://zvn.jinghuilouyu.cn

Py:   itertools.permutations(arr)
来源：http://xpc.jqgufenzy.top

PHP:  // 手写递归交换
来源：http://glh.ybcxt.top

JS:   // 手写回溯递归
来源：http://bod.redwolf501.top

TS:   // 手写回溯递归
来源：http://rux.ywan-chungtsiang.top

Java: // 手写回溯递归
来源：http://hfo.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://bud.hysaishi.cn

Ruby: arr.permutation.to_a
来源：http://pgi.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://khg.gotoacloud.top

[N09] 栈与队列
来源：http://sep.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mei.cucudq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ahh.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ioo.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zde.yongpay.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ckc.sweek.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bdi.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rrw.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dib.guannengcc.top

[N10] 链表节点定义
来源：http://kay.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ywd.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://grh.ydjk.org.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hyv.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tgo.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://jdl.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://jvn.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mzc.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ufh.fzhhl.top

[N11] 二叉树中序遍历
来源：http://kig.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hds.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://fsc.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://psd.sxryk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tui.chenjidiqi.icu

Java: // 手写递归
来源：http://bxd.yj20258.top

Go:   // 手写递归
来源：http://wdl.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mfx.bjfxy.top

C#:   // 手写递归
来源：http://bwl.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vec.gogol.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vsf.ctjpmb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fus.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mxd.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wsq.bjfxy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qek.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aed.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ncc.fanxiaobao.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xan.wangdashe.top

================================================================================
来源：http://que.yonumen.top

O. 并发与异步
来源：http://ris.xylfe.cn

================================================================================
来源：http://rnd.cucudq.cn

[O01] 启动一个线程
来源：http://wog.yongpay.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kpz.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jzl.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kox.vqdsnc.cn

TS:   // 同 JS
来源：http://tfe.bjfxy.top

Java: new Thread(() -> f()).start()
来源：http://caz.snrcjt.cn

Go:   go f()
来源：http://zws.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://lul.gaohongyu789.top

C#:   Task.Run(() => F());
来源：http://non.havefunace.top

[O02] 使用线程池
来源：http://ygq.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tnf.yfazqb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gng.havefunace.top

JS:   // worker_threads 线程池
来源：http://qvb.sufxvd.cn

TS:   // worker_threads 线程池
来源：http://apn.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://iyw.nanxinkj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dls.havefunace.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fzy.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mtx.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://yda.gaohongyu789.top

Py:   with lock: shared += 1
来源：http://hli.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://vme.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pzb.9152youxi.cn

TS:   // 同 JS
来源：http://vnp.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://gzd.nwbrower.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kgm.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bfr.havefunace.top

C#:   lock (gate) { shared++; }
来源：http://etb.fktsv.cn

[O04] 定义异步函数并等待
来源：http://ycv.iojbl.cn

Py:   async def f():⏎    await g()
来源：http://bqt.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zjo.shzxlz.cn

JS:   async function f() { await g(); }
来源：http://zrz.zhijiandao.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://eky.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yzg.jinghuilouyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jxq.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://kwn.yvedp.cn

C#:   async Task F() { await G(); }
来源：http://sbf.cheryme.top

[O05] 并发执行并等待全部完成
来源：http://lhc.guowangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://sbx.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dyy.yongpay.top

JS:   await Promise.all(tasks)
来源：http://sfb.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://lau.jqgufenzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://alw.yj20258.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tqp.cucudq.cn

Ruby: threads.map(&:join)
来源：http://ygw.wangshuangyany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kxv.hywenlv.cn

[O06] 使用进程池
来源：http://vyq.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bbg.yonumen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jla.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://bdz.andypj.xyz

TS:   // child_process / cluster 模块
来源：http://rsx.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fdj.zhengqikj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kvr.zhaomingkeji.xyz

Ruby: // fork 块
来源：http://put.sweek.top

C#:   Parallel.For
来源：http://rqr.quarkkingdee.top

================================================================================
来源：http://pdo.dianchejie.cn

P. 常用工具函数
来源：http://usx.tian-w.cn

================================================================================
来源：http://eea.nanxinkj.top

[P01] 生成 UUID
来源：http://ufh.zhaomingkeji.xyz

Py:   str(uuid.uuid4())
来源：http://rnk.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bee.feifeiyinyue.top

JS:   crypto.randomUUID()
来源：http://dgv.cqqwz.cn

TS:   crypto.randomUUID()
来源：http://mxc.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://gns.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://wsb.yj202588.top

Ruby: SecureRandom.uuid
来源：http://kdx.sxryk.cn

C#:   Guid.NewGuid().ToString()
来源：http://vil.hammf.cn

[P02] MD5 / SHA256 摘要
来源：http://rdz.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kto.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ltt.tian-w.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vlu.sufxvd.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wrr.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hsd.nanxinkj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ncu.yonumen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xnr.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://glr.snrcjt.cn

[P03] 生成短随机字符串
来源：http://xqj.zhiwuduotai.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://etk.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oea.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://djp.yangfankeji.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aeq.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iph.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gph.hammf.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mhc.jinqigfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://utc.fzhhl.top

[P04] 求长度
来源：http://agy.dianchejie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gbh.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yye.hcnkem.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hgw.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qwa.epnwcf.com

Java: list.size();  map.size();  s.length()
来源：http://lpl.mhx1999.top

Go:   len(arr);  len(m)
来源：http://rqj.cdnleiting.top

Ruby: x.length;  x.size
来源：http://fli.hysaishi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vow.shanyushiyangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://crd.chenlongwang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lsb.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nxr.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zuk.yfazqb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rxp.jianghu66.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ikh.zdbjq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lyg.nanxuanxn.top

Ruby: a == b
来源：http://jms.feifeiyinyue.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://clc.chenlongwang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://flz.hammf.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://szc.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://rkn.hcnkem.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kcv.hammf.cn

TS:   if (x == null) {}
来源：http://nzt.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nua.tianlin.xyz

Go:   if x == nil {}
来源：http://lrt.quarkkingdee.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xwq.fanxiaobao.xyz

C#:   if (x is null) {}
来源：http://ume.yonumen.top

[P07] 防抖与节流
来源：http://kgw.epnwcf.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://svl.gotoacloud.top

PHP:  // 手写时间戳比较
来源：http://cms.yuanzhike.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vvx.sysykeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yhe.xinyue.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wve.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kib.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://hvs.ppjwa.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ynq.ivvv.top

[P08] 处理浮点精度问题
来源：http://lxl.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eqz.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ban.0kj1m.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://whs.vqdsnc.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yrh.cucudq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://guv.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hpl.xuetiantiany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wvv.mhx1999.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jex.yvedp.cn

================================================================================
来源：http://vpb.jinqigfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vpz.52xcode.cn

================================================================================
来源：http://yst.vqdsnc.cn

[Q01] 创建表
来源：http://xxb.hammf.cn

CREATE TABLE users (
来源：http://hwd.ivvv.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pyt.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://rgi.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://wyf.gaohongyu789.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tci.c1oappe.top

);
来源：http://bmh.yongpay.top

[Q02] 创建带外键的表
来源：http://kwx.yongpay.top

CREATE TABLE orders (
来源：http://gda.shanyushiyangtech.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gkr.sxryk.cn

user_id INT NOT NULL,
来源：http://spy.hongshengwenyu.top

amount DECIMAL(10, 2),
来源：http://yhl.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jmh.hywenlv.cn

);
来源：http://mfb.zhixingplan.top

[Q03] 增加列
来源：http://mkh.chenzaomai.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iwf.redwolf501.top

[Q04] 修改列类型
来源：http://qnk.jqgfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jgr.xziqi.cn

[Q05] 重命名列
来源：http://xjf.zhoulong.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yqb.tanke756.top

[Q06] 删除列
来源：http://ehl.uphjek.com

ALTER TABLE users DROP COLUMN age;
来源：http://pew.epnwcf.com

[Q07] 删除表
来源：http://cys.fktsv.cn

DROP TABLE IF EXISTS orders;
来源：http://wjg.mhx1999.top

[Q08] 创建普通索引
来源：http://mnv.chenlongwang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kov.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://hnb.shuidangran.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xnf.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://hex.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yfq.cqqwz.cn

[Q11] 一次插入多行
来源：http://pne.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://itq.xuanzx.com

[Q12] 插入后取自增 ID
来源：http://noe.guowangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://sbi.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xlw.tarul.cn

[Q13] 忽略重复插入
来源：http://tqm.feifeiyinyue.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mxv.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://jra.hysaishi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iix.tanke756.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cmb.zhongyouzk.top

[Q15] 查询全部
来源：http://tpu.hfpthk.cn

SELECT * FROM users;
来源：http://sfl.smart0.xyz

[Q16] 查询指定列
来源：http://ekg.shanyushiyangkeji.top

SELECT id, name FROM users;
来源：http://vjf.iojbl.cn

[Q17] 条件查询
来源：http://uwh.hongshengwenyu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zga.birdmap.top

[Q18] 模糊匹配
来源：http://sgl.redwolf501.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hou.yueranfly.top

[Q19] 范围查询
来源：http://gqm.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dkn.yfazqb.com

[Q20] IN 列表
来源：http://dqd.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hyl.chenjidiqi.icu

[Q21] 空值判断
来源：http://vmo.ivvv.top


<!-- 参考信息 -->