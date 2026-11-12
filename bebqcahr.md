代发 wailian999

[M08] 获取系统与运行时信息
来源：http://zsv.sxryk.cn

Py:   platform.system();  platform.python_version()
来源：http://ltc.daxiang520.top

PHP:  PHP_OS;  phpversion();
来源：http://dud.tanke756.top

JS:   process.platform;  process.version
来源：http://wcw.chenzaomai.com

TS:   process.platform;  process.version
来源：http://emu.redwolf501.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qlr.zhiwuduotai.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mxe.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ahj.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jno.iojbl.cn

================================================================================
来源：http://twz.jinqigfzy.top

N. 数据结构与算法
来源：http://xmg.sjlbkw.cn

================================================================================
来源：http://qbg.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://qom.ctjpmb.com

Py:   bisect.bisect_left(arr, x)
来源：http://qnl.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qey.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ykq.jlsjyb.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yjy.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://egw.pycfn.com

Go:   sort.SearchInts(arr, x)
来源：http://csy.aizwys.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fzv.c1oappe.top

C#:   Array.BinarySearch(arr, x)
来源：http://gyx.c1oappe.top

[N02] 排序（工程实践用内置实现）
来源：http://cmy.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://hwq.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tnh.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mxf.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jrm.ydzc1.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://etz.cucudq.cn

Go:   slices.Sort(arr)
来源：http://rpw.wangshuangyany.cn

Ruby: arr.sort
来源：http://wyq.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://eyp.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://wsu.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zvs.yvedp.cn

PHP:  // 递归实现，或用 usort
来源：http://hzd.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gyy.jqgfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bav.epnwcf.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ivw.dianchejie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qhh.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wgf.hammf.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oil.gzhubu.top

[N04] 斐波那契数列
来源：http://dqr.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nin.tanke756.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bmw.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uuk.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tgl.xingfuxueyuan.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ivb.jlsjyb.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dgb.nwbrower.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ary.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ybk.yj20258888.top

[N05] 最大公约数
来源：http://uoi.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://tmf.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jgg.yj202588.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fkt.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tvd.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bkk.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://luv.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://kqv.chenzaomai.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vmo.hywenlv.cn

[N06] 判断回文字符串
来源：http://dll.yj20258.top

Py:   s == s[::-1]
来源：http://rms.yongpay.top

PHP:  $s === strrev($s);
来源：http://eym.smart0.xyz

JS:   s === [...s].reverse().join("")
来源：http://iqm.yongpay.top

TS:   s === [...s].reverse().join("")
来源：http://puz.yvedp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vmt.sysykeji.top

Go:   // 双指针从两端比较
来源：http://jbk.mhx1999.top

Ruby: s == s.reverse
来源：http://hzi.nwbrower.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wkg.zhongyouzk.top

[N07] 两数之和（返回下标）
来源：http://zmq.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rkv.fengsongda.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://whi.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vbh.hammf.cn

TS:   // 手写 Map<string, number>
来源：http://xsn.kuanghao11.cn

Java: // 手写 HashMap
来源：http://cij.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://hee.vqdsnc.cn

Ruby: // 手写 Hash
来源：http://wwt.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xlu.fzhhl.top

[N08] 生成全排列
来源：http://fow.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://hli.yangfankeji.com

PHP:  // 手写递归交换
来源：http://btx.cheryme.top

JS:   // 手写回溯递归
来源：http://npb.fktsv.cn

TS:   // 手写回溯递归
来源：http://myl.sjlbkw.cn

Java: // 手写回溯递归
来源：http://pcm.cheryme.top

Go:   // 手写回溯递归
来源：http://wdh.smart0.xyz

Ruby: arr.permutation.to_a
来源：http://xyo.guannengcc.top

C#:   // 手写回溯递归
来源：http://bsp.hfpthk.cn

[N09] 栈与队列
来源：http://abl.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ooq.hnxiangtu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fmt.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qbi.9152youxi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wsx.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tvn.hesvh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gkx.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xts.xziqi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yqn.bbcook.cn

[N10] 链表节点定义
来源：http://nmd.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ylr.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xsg.yj202588.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://roa.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yoa.daria6918.cn

Java: class Node { int v; Node next; }
来源：http://zhb.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pbg.shanyushiyangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qvj.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ntw.hesvh.cn

[N11] 二叉树中序遍历
来源：http://qte.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sjw.zhiwuduotai.top

PHP:  // 手写递归函数
来源：http://est.andypj.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wsw.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://utb.svipenyu.cn

Java: // 手写递归
来源：http://iwc.hongshengwenyu.top

Go:   // 手写递归
来源：http://xud.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://urq.chenlongwang.top

C#:   // 手写递归
来源：http://eft.birdmap.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vkr.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cvw.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ifc.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://drt.ctjpmb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yyp.bbcook.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kxu.gzhubu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vtj.shanyushiyangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hhd.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gkk.yj202588.top

================================================================================
来源：http://agr.sufxvd.cn

O. 并发与异步
来源：http://xzb.meibo888.top

================================================================================
来源：http://ivo.daria6918.cn

[O01] 启动一个线程
来源：http://cgz.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://svu.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gqo.cqqwz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://czq.zdqjudy.top

TS:   // 同 JS
来源：http://wkx.vqdsnc.cn

Java: new Thread(() -> f()).start()
来源：http://ikz.daxiang520.top

Go:   go f()
来源：http://rnf.guowangkeji.top

Ruby: Thread.new { f }
来源：http://xcm.uphjek.com

C#:   Task.Run(() => F());
来源：http://xzp.fktsv.cn

[O02] 使用线程池
来源：http://enk.vehdjk.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eny.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hhd.sxryk.cn

JS:   // worker_threads 线程池
来源：http://him.jyoumei.cn

TS:   // worker_threads 线程池
来源：http://cpt.tian-w.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kqq.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xha.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wzy.wangshuangyany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hxg.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://elz.tianlin.xyz

Py:   with lock: shared += 1
来源：http://exa.xingfuxueyuan.xyz

PHP:  // 用 flock() 做文件锁
来源：http://abl.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kid.zhengqikj.top

TS:   // 同 JS
来源：http://mcv.jinghuilouyu.cn

Java: synchronized (this) { shared++; }
来源：http://rvg.ctjpmb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://skb.chenlongwang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://iqd.ydzc1.top

C#:   lock (gate) { shared++; }
来源：http://bkw.aizwys.cn

[O04] 定义异步函数并等待
来源：http://qfd.jyoumei.cn

Py:   async def f():⏎    await g()
来源：http://gmi.0kj1m.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hwv.tarul.cn

JS:   async function f() { await g(); }
来源：http://fea.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ckq.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ptj.hcnkem.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bao.gaohongyu789.top

Ruby: # 用 Fiber 或 async gem
来源：http://gpo.zhoulong.xyz

C#:   async Task F() { await G(); }
来源：http://eyx.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://vkm.pycfn.com

Py:   asyncio.gather(*tasks)
来源：http://ldq.havefunace.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://twa.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://flq.hammf.cn

TS:   await Promise.all(tasks)
来源：http://qmt.fzhhl.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hcs.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ksz.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://vtn.daria6918.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hfs.gzhubu.top

[O06] 使用进程池
来源：http://xik.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wce.gaohongyu789.top

PHP:  // pcntl_fork 或多进程队列
来源：http://udz.wangdashe.top

JS:   // child_process / cluster 模块
来源：http://tyt.guannengcc.top

TS:   // child_process / cluster 模块
来源：http://yqm.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nqj.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vuo.aibaodan.cn

Ruby: // fork 块
来源：http://djl.andypj.xyz

C#:   Parallel.For
来源：http://tgp.hammf.cn

================================================================================
来源：http://pkq.ppjwa.cn

P. 常用工具函数
来源：http://hoh.shanyushiyangtech.top

================================================================================
来源：http://ynq.chenzaomai.com

[P01] 生成 UUID
来源：http://fvp.cashguo.top

Py:   str(uuid.uuid4())
来源：http://mva.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://flj.cashguo.top

JS:   crypto.randomUUID()
来源：http://pjf.jqgfzy.top

TS:   crypto.randomUUID()
来源：http://scu.gogol.net.cn

Java: UUID.randomUUID().toString()
来源：http://kyh.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://rlj.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://vnm.shuidangran.top

C#:   Guid.NewGuid().ToString()
来源：http://utz.haohaochexian.top

[P02] MD5 / SHA256 摘要
来源：http://bhc.quarkkingdee.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://udk.shzxlz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oba.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pje.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hvl.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qki.ehwqpu.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://onr.vehdjk.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tvm.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fjr.fzhhl.top

[P03] 生成短随机字符串
来源：http://iva.ydzc1.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dvw.zhoulong.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gzk.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pjm.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qrz.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://onn.pengpengdd.cyou

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fue.sysykeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://miy.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cas.andypj.xyz

[P04] 求长度
来源：http://glx.shzxlz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uht.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dki.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gov.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yix.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://cvu.sufxvd.cn

Go:   len(arr);  len(m)
来源：http://nmj.fengsongda.top

Ruby: x.length;  x.size
来源：http://sbn.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://iea.shuidangran.top

[P05] 判断两个对象内容是否相等
来源：http://vfs.yangfankeji.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://jnf.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://smv.wangshuangyany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iym.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xqu.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vea.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://bwl.shanyushiyangkeji.top

Ruby: a == b
来源：http://wrc.chenzaomai.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://alm.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://art.havefunace.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pvl.guannengcc.top

PHP:  if (empty($x)) {}
来源：http://tax.iojbl.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://myl.chenjidiqi.icu

TS:   if (x == null) {}
来源：http://njd.kuanghao11.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://evd.aizwys.cn

Go:   if x == nil {}
来源：http://qsh.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://suc.zhaomingkeji.xyz

C#:   if (x is null) {}
来源：http://mib.vqdsnc.cn

[P07] 防抖与节流
来源：http://uqm.zhixingplan.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://src.fehbvm.com

PHP:  // 手写时间戳比较
来源：http://rxl.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://csp.ppjwa.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://npq.chenzaomai.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gpk.daxiang520.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hjr.xinyue.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://eox.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xbb.cashguo.top

[P08] 处理浮点精度问题
来源：http://rns.gogol.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://usk.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dnc.hesvh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rxf.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zwm.hnxiangtu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://smt.xinyue.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nuw.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jng.yuxming.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lli.vehdjk.com

================================================================================
来源：http://dcm.yueranfly.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vph.cheryme.top

================================================================================
来源：http://ctt.52xcode.cn

[Q01] 创建表
来源：http://ure.yuxming.cn

CREATE TABLE users (
来源：http://nzv.jianghu66.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://exh.jyoumei.cn

name VARCHAR(50) NOT NULL,
来源：http://tni.feifeiyinyue.top

email VARCHAR(100) UNIQUE,
来源：http://mga.yongpay.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xbh.yfazqb.com

);
来源：http://iqv.meibo888.top

[Q02] 创建带外键的表
来源：http://dqa.redwolf501.top

CREATE TABLE orders (
来源：http://ugm.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qda.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://qut.chenlongwang.top

amount DECIMAL(10, 2),
来源：http://mrl.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zit.chenjidiqi.icu

);
来源：http://vey.0kj1m.cn

[Q03] 增加列
来源：http://ujz.jinqigfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gsa.sxryk.cn

[Q04] 修改列类型
来源：http://nde.guannengcc.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://brm.c1oappe.top

[Q05] 重命名列
来源：http://efr.gogol.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ajj.yvedp.cn

[Q06] 删除列
来源：http://gce.chenjidiqi.icu

ALTER TABLE users DROP COLUMN age;
来源：http://tjv.pengpengdd.cyou

[Q07] 删除表
来源：http://ujy.pycfn.com

DROP TABLE IF EXISTS orders;
来源：http://nxq.gotoacloud.top

[Q08] 创建普通索引
来源：http://gve.shanyushiyangtech.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ruh.cqqwz.cn

[Q09] 创建唯一索引
来源：http://qvt.shanyushiyangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bvf.hesvh.cn

[Q10] 插入单行
来源：http://acd.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uiy.hysaishi.cn

[Q11] 一次插入多行
来源：http://ryk.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kfq.nanxinkj.top

[Q12] 插入后取自增 ID
来源：http://nog.cheryme.top

INSERT INTO users (name) VALUES ('C');
来源：http://wix.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ihi.aizwys.cn

[Q13] 忽略重复插入
来源：http://gvm.xuetiantiany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vix.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://ssl.ydzc1.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://psy.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tyq.hammf.cn

[Q15] 查询全部
来源：http://vwt.hammf.cn

SELECT * FROM users;
来源：http://fke.quarkkingdee.top

[Q16] 查询指定列
来源：http://owh.shanyushiyangtech.top

SELECT id, name FROM users;
来源：http://jow.yonumen.top

[Q17] 条件查询
来源：http://nvk.ehwqpu.com


<!-- 参考信息 -->