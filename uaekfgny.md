代发 wailian999

[M08] 获取系统与运行时信息
来源：http://jib.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://utz.chenlongwang.top

PHP:  PHP_OS;  phpversion();
来源：http://zqp.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://kij.9152youxi.cn

TS:   process.platform;  process.version
来源：http://xxl.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qik.nanxinkj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fta.hfpthk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xoe.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gbt.xuetiantiany.cn

================================================================================
来源：http://axf.epnwcf.com

N. 数据结构与算法
来源：http://vtb.zhongyouzk.top

================================================================================
来源：http://ybw.fktsv.cn

[N01] 二分查找（有序数组）
来源：http://yhl.fanxiaobao.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://eje.feifeiyinyue.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fen.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qgu.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://afa.smart0.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://wzl.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://bca.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://udk.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://huy.hysaishi.cn

[N02] 排序（工程实践用内置实现）
来源：http://hto.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://vzj.andypj.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nqf.cheryme.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tnx.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://lao.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dfj.ydzc1.top

Go:   slices.Sort(arr)
来源：http://xio.jyoumei.cn

Ruby: arr.sort
来源：http://dce.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ici.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://dge.xziqi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jrd.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://wpp.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ezt.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ykn.jinyuanbaomall.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sug.jinghuilouyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nzm.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gkj.zhengqikj.top

C#:   // 手写递归，或 Array.Sort
来源：http://fsa.hfpthk.cn

[N04] 斐波那契数列
来源：http://jul.aizwys.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wbh.316326.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gwf.haohaochexian.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jdh.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iyg.gaohongyu789.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kbw.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ykx.zhengqikj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lmc.quarkkingdee.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wmh.zdqjudy.top

[N05] 最大公约数
来源：http://dli.yj20258888.top

Py:   math.gcd(a, b)
来源：http://qxw.nanxuanxn.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vze.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://khj.fehbvm.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://phe.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hft.hnqzz.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bmw.zdbjq.cn

Ruby: a.gcd(b)
来源：http://qmb.iojbl.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lxc.hcnkem.com

[N06] 判断回文字符串
来源：http://avb.quarkkingdee.top

Py:   s == s[::-1]
来源：http://crs.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://dfn.shanyushiyangtech.top

JS:   s === [...s].reverse().join("")
来源：http://aiw.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://zgb.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pxa.meibo888.top

Go:   // 双指针从两端比较
来源：http://wtw.9152youxi.cn

Ruby: s == s.reverse
来源：http://yqx.shzxlz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nfb.ivvv.top

[N07] 两数之和（返回下标）
来源：http://aor.xylfe.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jfm.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rpc.jianghu66.top

JS:   // 手写 Map：map.set(v, i)
来源：http://osc.9152youxi.cn

TS:   // 手写 Map<string, number>
来源：http://gnk.jqgufenzy.top

Java: // 手写 HashMap
来源：http://kad.hnqzz.top

Go:   // 手写 map[int]int
来源：http://vdt.epnwcf.com

Ruby: // 手写 Hash
来源：http://pbz.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://ltb.jinqigfzy.top

[N08] 生成全排列
来源：http://juv.yj20258888.top

Py:   itertools.permutations(arr)
来源：http://mvj.hcnkem.com

PHP:  // 手写递归交换
来源：http://cae.daxiang520.top

JS:   // 手写回溯递归
来源：http://oqe.aizwys.cn

TS:   // 手写回溯递归
来源：http://spq.316326.xyz

Java: // 手写回溯递归
来源：http://cud.ybcxt.top

Go:   // 手写回溯递归
来源：http://bnz.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://laa.ybcxt.top

C#:   // 手写回溯递归
来源：http://unn.andypj.xyz

[N09] 栈与队列
来源：http://srb.sweek.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ysa.birdmap.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://glt.andypj.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://swd.shzxlz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ftl.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://egn.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aew.hnqzz.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xwz.xziqi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eab.jlsjyb.cn

[N10] 链表节点定义
来源：http://dff.zhoulong.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kji.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://atb.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pve.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jsh.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://ifz.yj20258.top

Go:   type Node struct { V int; Next *Node }
来源：http://htz.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://txv.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mdf.nwbrower.top

[N11] 二叉树中序遍历
来源：http://urz.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rya.ctjpmb.com

PHP:  // 手写递归函数
来源：http://yfb.hnxiangtu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nfn.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jif.zhengqikj.top

Java: // 手写递归
来源：http://iwt.shuidangran.top

Go:   // 手写递归
来源：http://tlk.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dwk.xuanzx.com

C#:   // 手写递归
来源：http://mbt.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vql.ppjwa.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mhh.zdqjudy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kid.hcnkem.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xfr.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xhx.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zqd.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://smu.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jok.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://spz.xuanzx.com

================================================================================
来源：http://rkl.shanyushiyangkeji.top

O. 并发与异步
来源：http://ych.nanxuanxn.top

================================================================================
来源：http://say.ydjk.org.cn

[O01] 启动一个线程
来源：http://thc.andypj.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://phe.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://szp.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://slt.shuidangran.top

TS:   // 同 JS
来源：http://lat.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://xzz.9152youxi.cn

Go:   go f()
来源：http://zdr.feifeiyinyue.top

Ruby: Thread.new { f }
来源：http://ppq.yj20258.top

C#:   Task.Run(() => F());
来源：http://iyy.cashguo.top

[O02] 使用线程池
来源：http://nye.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oyt.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qvp.snrcjt.cn

JS:   // worker_threads 线程池
来源：http://pmv.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://kiv.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://jlt.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dnw.uphjek.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dbn.yuanzhike.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kco.cucudq.cn

[O03] 加锁保护共享数据
来源：http://tjs.xuanzx.com

Py:   with lock: shared += 1
来源：http://diy.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://cjp.gotoacloud.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ooq.nanxuanxn.top

TS:   // 同 JS
来源：http://uwd.zhixingplan.top

Java: synchronized (this) { shared++; }
来源：http://mxs.hcnkem.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ake.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cnq.xuanzx.com

C#:   lock (gate) { shared++; }
来源：http://asu.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://xof.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://nii.sjlbkw.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vpf.guowangkeji.top

JS:   async function f() { await g(); }
来源：http://fbe.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zhx.vqdsnc.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jir.wangdashe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://erq.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://crj.fzhhl.top

C#:   async Task F() { await G(); }
来源：http://knw.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://bky.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://xju.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tgm.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://ffo.xuetiantiany.cn

TS:   await Promise.all(tasks)
来源：http://ztt.yfazqb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mig.ydjk.org.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://prp.ydjk.org.cn

Ruby: threads.map(&:join)
来源：http://olm.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mdm.chenlongwang.top

[O06] 使用进程池
来源：http://mmu.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wfa.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rpe.cqqwz.cn

JS:   // child_process / cluster 模块
来源：http://rsr.gaohongyu789.top

TS:   // child_process / cluster 模块
来源：http://bbx.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xuw.jinqigfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ywm.jinqigufen.top

Ruby: // fork 块
来源：http://xnb.cucudq.cn

C#:   Parallel.For
来源：http://izl.ivvv.top

================================================================================
来源：http://mfj.vqdsnc.cn

P. 常用工具函数
来源：http://gsh.yangfankeji.com

================================================================================
来源：http://gpg.vehdjk.com

[P01] 生成 UUID
来源：http://dgr.yfazqb.com

Py:   str(uuid.uuid4())
来源：http://bal.fanxiaobao.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yfg.havefunace.top

JS:   crypto.randomUUID()
来源：http://ahw.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://mcd.yuxming.cn

Java: UUID.randomUUID().toString()
来源：http://zsb.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://dju.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://ndy.hongshengwenyu.top

C#:   Guid.NewGuid().ToString()
来源：http://bnp.52xcode.cn

[P02] MD5 / SHA256 摘要
来源：http://tvt.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eai.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://glz.yfazqb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xxn.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yrc.sjlbkw.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ylc.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://euo.bjfxy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hgb.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xrc.shzxlz.cn

[P03] 生成短随机字符串
来源：http://ixt.0kj1m.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jdd.9152youxi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ypm.hfpthk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qvk.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fvc.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://loc.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nvf.quarkkingdee.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tds.yj202588.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jlf.shanyushiyangkeji.top

[P04] 求长度
来源：http://agl.sjlbkw.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pfa.shuidangran.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yvv.vqdsnc.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://efo.yj20258.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gqn.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://npo.cqqwz.cn

Go:   len(arr);  len(m)
来源：http://bfj.dashuyun.cn

Ruby: x.length;  x.size
来源：http://gna.ybcxt.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jnj.bjfxy.top

[P05] 判断两个对象内容是否相等
来源：http://gam.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qge.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gni.hesvh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zag.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jgo.cashguo.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xdy.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://iao.zhengqikj.top

Ruby: a == b
来源：http://rmg.shanyushiyangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fel.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bim.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://itq.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://jqg.smart0.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blz.yj202588.top

TS:   if (x == null) {}
来源：http://ohm.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tgf.guannengcc.top

Go:   if x == nil {}
来源：http://mkj.zhiwuduotai.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ubk.hnxiangtu.top

C#:   if (x is null) {}
来源：http://vxu.zdbjq.cn

[P07] 防抖与节流
来源：http://wuv.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://teu.nwbrower.top

PHP:  // 手写时间戳比较
来源：http://fva.hesvh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ash.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vmu.chenzaomai.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://txg.xylfe.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dxp.pycfn.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://hqd.ehwqpu.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ltp.feifeiyinyue.top

[P08] 处理浮点精度问题
来源：http://ixi.ydzc1.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lgp.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://msl.yj20258888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hnd.kuanghao11.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://daj.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tiq.tanke756.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mbo.vehdjk.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qkd.sweek.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://trl.guannengcc.top

================================================================================
来源：http://qkq.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cqd.gogol.net.cn

================================================================================
来源：http://rtz.smart0.xyz

[Q01] 创建表
来源：http://dng.sjlbkw.cn

CREATE TABLE users (
来源：http://auh.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kwx.zhijiandao.cn

name VARCHAR(50) NOT NULL,
来源：http://dei.jiagoushi.top

email VARCHAR(100) UNIQUE,
来源：http://vyx.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pwi.aibaodan.cn

);
来源：http://vca.nanxuanxn.top

[Q02] 创建带外键的表
来源：http://rou.hesvh.cn

CREATE TABLE orders (
来源：http://rko.zdqjudy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aay.pengpengdd.cyou

user_id INT NOT NULL,
来源：http://pqo.xziqi.cn

amount DECIMAL(10, 2),
来源：http://eez.snrcjt.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mtf.cdnleiting.top

);
来源：http://bnd.zdbjq.cn

[Q03] 增加列
来源：http://ozc.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nqo.yonumen.top

[Q04] 修改列类型
来源：http://skz.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://exz.0kj1m.cn

[Q05] 重命名列
来源：http://lds.gogol.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dow.ehwqpu.com

[Q06] 删除列
来源：http://dbl.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://hkp.yvedp.cn

[Q07] 删除表
来源：http://bxm.yfazqb.com

DROP TABLE IF EXISTS orders;
来源：http://dfo.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://oef.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qos.zhaomingkeji.xyz

[Q09] 创建唯一索引
来源：http://rmp.chenjidiqi.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rbe.zdqjudy.top

[Q10] 插入单行
来源：http://wui.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mtp.ivvv.top

[Q11] 一次插入多行
来源：http://wvg.cqqwz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ikw.yuanzhike.top

[Q12] 插入后取自增 ID
来源：http://cqu.xinyue.icu

INSERT INTO users (name) VALUES ('C');
来源：http://mbl.xuetiantiany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://veb.ivvv.top

[Q13] 忽略重复插入
来源：http://jzz.aibaodan.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xpo.ydzc1.top

[Q14] 存在则更新（upsert）
来源：http://spz.bjfxy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ryk.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fxp.zdqjudy.top

[Q15] 查询全部
来源：http://pcw.yj20258888.top

SELECT * FROM users;
来源：http://ogp.birdmap.top

[Q16] 查询指定列
来源：http://glq.ctjpmb.com

SELECT id, name FROM users;
来源：http://bxq.dashuyun.cn

[Q17] 条件查询
来源：http://mbc.zhoulong.xyz


<!-- 参考信息 -->