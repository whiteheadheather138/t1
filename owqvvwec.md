代发 wailian999

Java: public static void main(String[] args)
来源：http://uns.smart0.xyz

Go:   func main()
来源：http://sjc.9152youxi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://izw.wangdashe.top

C#:   static void Main(string[] args)
来源：http://uua.hammf.cn

[M08] 获取系统与运行时信息
来源：http://gej.chenlongwang.top

Py:   platform.system();  platform.python_version()
来源：http://ira.cashguo.top

PHP:  PHP_OS;  phpversion();
来源：http://hdy.dianchejie.cn

JS:   process.platform;  process.version
来源：http://lpi.shzxlz.cn

TS:   process.platform;  process.version
来源：http://tvr.aizwys.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://epp.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rmv.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hsv.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mmd.shangyingyoupin.top

================================================================================
来源：http://zhn.svipenyu.cn

N. 数据结构与算法
来源：http://tfv.hcnkem.com

================================================================================
来源：http://exe.fktsv.cn

[N01] 二分查找（有序数组）
来源：http://goc.zhaomingkeji.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://aan.jiagoushi.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dhh.havefunace.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mnj.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uai.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://ckw.xinyue.icu

Go:   sort.SearchInts(arr, x)
来源：http://xqo.haohaochexian.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qpj.gogol.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kvr.zhengqikj.top

[N02] 排序（工程实践用内置实现）
来源：http://cpe.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://jxi.guannengcc.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pbs.uphjek.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://poy.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hng.jqgfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qdt.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://thb.yangfankeji.com

Ruby: arr.sort
来源：http://ord.snrcjt.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jqq.kuanghao11.cn

[N03] 快速排序（分治示例）
来源：http://lsb.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vdr.jinqigufen.top

PHP:  // 递归实现，或用 usort
来源：http://csf.zhongyouzk.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yjv.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vau.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pqc.yangfankeji.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://snd.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zua.vqdsnc.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ehk.zhiwuduotai.top

[N04] 斐波那契数列
来源：http://zev.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pjp.zhijiandao.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xku.fanxiaobao.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xyb.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://acn.tarul.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yvq.redwolf501.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mcn.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://efk.dashuyun.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nuu.gogol.net.cn

[N05] 最大公约数
来源：http://dbq.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://mqv.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uvf.chenlongwang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fyh.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sob.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kwb.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://voj.ppjwa.cn

Ruby: a.gcd(b)
来源：http://vyd.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nxa.sxryk.cn

[N06] 判断回文字符串
来源：http://zls.hnxiangtu.top

Py:   s == s[::-1]
来源：http://vve.bjfxy.top

PHP:  $s === strrev($s);
来源：http://nlp.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://kpp.shanyushiyangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://uto.gotoacloud.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fui.sweek.top

Go:   // 双指针从两端比较
来源：http://ici.ppjwa.cn

Ruby: s == s.reverse
来源：http://msu.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://giv.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://uen.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tir.shanyushiyangtech.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qaz.ctjpmb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://mik.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://whk.yj20258888.top

Java: // 手写 HashMap
来源：http://bld.fktsv.cn

Go:   // 手写 map[int]int
来源：http://vto.cqqwz.cn

Ruby: // 手写 Hash
来源：http://mwg.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://wlo.yfazqb.com

[N08] 生成全排列
来源：http://iwq.yonumen.top

Py:   itertools.permutations(arr)
来源：http://ueq.guannengcc.top

PHP:  // 手写递归交换
来源：http://ujb.pycfn.com

JS:   // 手写回溯递归
来源：http://tlm.shangyingyoupin.top

TS:   // 手写回溯递归
来源：http://ayi.tarul.cn

Java: // 手写回溯递归
来源：http://fez.hywenlv.cn

Go:   // 手写回溯递归
来源：http://hrc.hysaishi.cn

Ruby: arr.permutation.to_a
来源：http://vhk.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://kvz.jqgfzy.top

[N09] 栈与队列
来源：http://xvo.ydzc1.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dux.cucudq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://auw.epnwcf.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hbc.jinyuanbaomall.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ijk.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qvq.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cyp.hcnkem.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://phk.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dgn.dashuyun.cn

[N10] 链表节点定义
来源：http://pqu.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ysm.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://nzv.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://myg.jinghuilouyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rwo.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://oxr.vqdsnc.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wji.wangdashe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://llm.tarul.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zoa.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://lsv.gaohongyu789.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fmx.chenzaomai.com

PHP:  // 手写递归函数
来源：http://sta.zycfv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rnu.yanxiufei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nzq.daxiang520.top

Java: // 手写递归
来源：http://tlx.feifeiyinyue.top

Go:   // 手写递归
来源：http://rjl.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hlf.daxiang520.top

C#:   // 手写递归
来源：http://txz.nwbrower.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yop.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fff.guowangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yjn.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ane.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fhz.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bpd.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eax.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qcq.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vhf.yfazqb.com

================================================================================
来源：http://xbw.zhixingplan.top

O. 并发与异步
来源：http://dsi.feifeiyinyue.top

================================================================================
来源：http://bii.sysykeji.top

[O01] 启动一个线程
来源：http://wby.zhixingplan.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://daf.tarul.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mly.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xzb.zhengqikj.top

TS:   // 同 JS
来源：http://ust.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://nrg.xuanzx.com

Go:   go f()
来源：http://ndl.cqqwz.cn

Ruby: Thread.new { f }
来源：http://dfg.yfazqb.com

C#:   Task.Run(() => F());
来源：http://xnh.zdqjudy.top

[O02] 使用线程池
来源：http://ugy.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://huk.mhx1999.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rgy.gzhubu.top

JS:   // worker_threads 线程池
来源：http://wjd.pycfn.com

TS:   // worker_threads 线程池
来源：http://yfw.hnxiangtu.top

Java: Executors.newFixedThreadPool(4)
来源：http://cgz.nwbrower.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dfu.nwbrower.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bwb.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wly.tianlin.xyz

[O03] 加锁保护共享数据
来源：http://lly.daxiang520.top

Py:   with lock: shared += 1
来源：http://jzu.shuidangran.top

PHP:  // 用 flock() 做文件锁
来源：http://rmj.hesvh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eea.jiagoushi.top

TS:   // 同 JS
来源：http://pzj.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://jis.bbcook.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oki.cashguo.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uru.hnxiangtu.top

C#:   lock (gate) { shared++; }
来源：http://xfh.zycfv.cn

[O04] 定义异步函数并等待
来源：http://xop.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://dgk.jinyuanbaomall.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ffq.jinqigfzy.top

JS:   async function f() { await g(); }
来源：http://ksb.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://qii.hysaishi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zed.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://flu.ivvv.top

Ruby: # 用 Fiber 或 async gem
来源：http://npv.shanyushiyangkeji.top

C#:   async Task F() { await G(); }
来源：http://hey.tianlin.xyz

[O05] 并发执行并等待全部完成
来源：http://ksh.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://frh.gotoacloud.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nwu.uphjek.com

JS:   await Promise.all(tasks)
来源：http://dok.pycfn.com

TS:   await Promise.all(tasks)
来源：http://hkk.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ftk.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vgb.redwolf501.top

Ruby: threads.map(&:join)
来源：http://kxu.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fck.daxiang520.top

[O06] 使用进程池
来源：http://xyf.uphjek.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ebg.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lst.guannengcc.top

JS:   // child_process / cluster 模块
来源：http://eid.zhaomingkeji.xyz

TS:   // child_process / cluster 模块
来源：http://ihd.ydzc1.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fof.chenzaomai.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dow.kuanghao11.cn

Ruby: // fork 块
来源：http://hxc.zhiwuduotai.top

C#:   Parallel.For
来源：http://fdt.pengpengdd.cyou

================================================================================
来源：http://eub.sxryk.cn

P. 常用工具函数
来源：http://qaw.tian-w.cn

================================================================================
来源：http://xqr.xylfe.cn

[P01] 生成 UUID
来源：http://ivw.316326.xyz

Py:   str(uuid.uuid4())
来源：http://wuh.shanyushiyangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yfh.hcnkem.com

JS:   crypto.randomUUID()
来源：http://lxi.daxiang520.top

TS:   crypto.randomUUID()
来源：http://uta.zycfv.cn

Java: UUID.randomUUID().toString()
来源：http://jun.iojbl.cn

Go:   // 用 github.com/google/uuid
来源：http://hjr.316326.xyz

Ruby: SecureRandom.uuid
来源：http://fek.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://dkq.hnqzz.top

[P02] MD5 / SHA256 摘要
来源：http://wvf.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vjt.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ygg.sysykeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://knf.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mxb.cheryme.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ecn.aizwys.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jao.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://drn.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ibj.gotoacloud.top

[P03] 生成短随机字符串
来源：http://tii.gzhubu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hdj.pengpengdd.cyou

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bkk.tian-w.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zxs.xinyue.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ayz.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xhz.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pbp.cucudq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pfe.jinyuanbaomall.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iqd.yj20258888.top

[P04] 求长度
来源：http://vmd.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xdy.aizwys.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://exs.9152youxi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mkv.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ffz.zhongyouzk.top

Java: list.size();  map.size();  s.length()
来源：http://jmi.cqqwz.cn

Go:   len(arr);  len(m)
来源：http://guj.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://psg.ydjk.org.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xnn.ivvv.top

[P05] 判断两个对象内容是否相等
来源：http://xag.feifeiyinyue.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uwj.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lpf.chenlongwang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uaz.zhijiandao.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xgg.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://adl.sufxvd.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fzc.wangdashe.top

Ruby: a == b
来源：http://ddo.pycfn.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xzh.yj20258.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iyv.hnxiangtu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lmr.cqqwz.cn

PHP:  if (empty($x)) {}
来源：http://svx.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bgq.9152youxi.cn

TS:   if (x == null) {}
来源：http://aom.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://llx.guannengcc.top

Go:   if x == nil {}
来源：http://oeu.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xkg.zycfv.cn

C#:   if (x is null) {}
来源：http://gho.smart0.xyz

[P07] 防抖与节流
来源：http://qsp.daria6918.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://inp.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://dbq.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://usf.hysaishi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jbl.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vkz.haohaochexian.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ajj.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yyi.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hne.316326.xyz

[P08] 处理浮点精度问题
来源：http://nwb.xziqi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eew.gogol.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://urv.jinqigfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bam.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bfu.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mta.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tzg.chenzaomai.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xxh.zycfv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rkt.sufxvd.cn

================================================================================
来源：http://nhi.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fnl.hnqzz.top

================================================================================
来源：http://pbd.yfazqb.com

[Q01] 创建表
来源：http://ufd.smart0.xyz

CREATE TABLE users (
来源：http://vdl.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hkb.52xcode.cn

name VARCHAR(50) NOT NULL,
来源：http://cpn.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://rnr.aibaodan.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uxc.316326.xyz

);
来源：http://vgg.mhx1999.top

[Q02] 创建带外键的表
来源：http://ain.zhoulong.xyz

CREATE TABLE orders (
来源：http://whs.dianchejie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://egp.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://rxl.yj202588.top

amount DECIMAL(10, 2),
来源：http://grc.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://win.xuetiantiany.cn

);
来源：http://wkw.fzhhl.top

[Q03] 增加列
来源：http://lfr.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hdy.zhijiandao.cn

[Q04] 修改列类型
来源：http://wtm.hesvh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kyx.tarul.cn

[Q05] 重命名列
来源：http://rex.cheryme.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ovb.snrcjt.cn

[Q06] 删除列
来源：http://osj.wangshuangyany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ghg.aizwys.cn

[Q07] 删除表
来源：http://ldy.gotoacloud.top

DROP TABLE IF EXISTS orders;
来源：http://yhn.tianlin.xyz

[Q08] 创建普通索引
来源：http://zxh.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://onj.zycfv.cn

[Q09] 创建唯一索引
来源：http://jes.jinyuanbaomall.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://azk.sjlbkw.cn

[Q10] 插入单行
来源：http://myc.daria6918.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bkf.c1oappe.top

[Q11] 一次插入多行
来源：http://qzf.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hki.cheryme.top

[Q12] 插入后取自增 ID
来源：http://nyp.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://vlf.jinqigfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tmn.daria6918.cn

[Q13] 忽略重复插入
来源：http://ywa.jlsjyb.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ixa.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://qbf.zhaomingkeji.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tgf.dianchejie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pjd.andypj.xyz

[Q15] 查询全部
来源：http://emn.guowangkeji.top


<!-- 参考信息 -->