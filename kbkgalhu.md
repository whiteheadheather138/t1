代发 wailian999

Java: public static void main(String[] args)
来源：http://rxh.sjlbkw.cn

Go:   func main()
来源：http://uyu.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ecz.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://vbd.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://zsc.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://hli.kuanghao11.cn

PHP:  PHP_OS;  phpversion();
来源：http://zaa.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://sjk.bbcook.cn

TS:   process.platform;  process.version
来源：http://wzg.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yqe.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ssl.shangyingyoupin.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://daa.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nog.xuetiantiany.cn

================================================================================
来源：http://ghx.meibo888.top

N. 数据结构与算法
来源：http://jkj.xylfe.cn

================================================================================
来源：http://ttq.tarul.cn

[N01] 二分查找（有序数组）
来源：http://ine.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://slf.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ssv.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fui.ctjpmb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kay.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://cok.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://nnj.xuetiantiany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://spq.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xvk.zhongyouzk.top

[N02] 排序（工程实践用内置实现）
来源：http://xri.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://btv.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mtk.xziqi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fjg.pycfn.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://tob.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vks.fehbvm.com

Go:   slices.Sort(arr)
来源：http://bel.sufxvd.cn

Ruby: arr.sort
来源：http://ier.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://boo.sysykeji.top

[N03] 快速排序（分治示例）
来源：http://udl.zycfv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vit.jqgfzy.top

PHP:  // 递归实现，或用 usort
来源：http://dkj.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://coq.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dmr.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://coc.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qef.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eza.zhongyouzk.top

C#:   // 手写递归，或 Array.Sort
来源：http://hwq.guowangkeji.top

[N04] 斐波那契数列
来源：http://ich.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yqn.shzxlz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ghv.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ace.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xck.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jjl.aizwys.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pnl.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jcx.jianghu66.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pik.yfazqb.com

[N05] 最大公约数
来源：http://txj.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://jhb.xuanzx.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hvt.shangyingyoupin.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gff.sufxvd.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ves.xylfe.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wrh.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cze.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://pop.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://amy.nanxuanxn.top

[N06] 判断回文字符串
来源：http://oxm.daxiang520.top

Py:   s == s[::-1]
来源：http://blr.guannengcc.top

PHP:  $s === strrev($s);
来源：http://nxe.sufxvd.cn

JS:   s === [...s].reverse().join("")
来源：http://jqr.xuetiantiany.cn

TS:   s === [...s].reverse().join("")
来源：http://yuw.cashguo.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gan.birdmap.top

Go:   // 双指针从两端比较
来源：http://tcx.xuanzx.com

Ruby: s == s.reverse
来源：http://pmh.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://exd.birdmap.top

[N07] 两数之和（返回下标）
来源：http://dsj.jlsjyb.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jdl.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nvj.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://scb.sweek.top

TS:   // 手写 Map<string, number>
来源：http://lpb.52xcode.cn

Java: // 手写 HashMap
来源：http://adm.ivvv.top

Go:   // 手写 map[int]int
来源：http://ffg.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://dvh.yfazqb.com

C#:   // 手写 Dictionary<int, int>
来源：http://rcw.chenjidiqi.icu

[N08] 生成全排列
来源：http://xfh.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://dvp.sweek.top

PHP:  // 手写递归交换
来源：http://xtf.vehdjk.com

JS:   // 手写回溯递归
来源：http://mav.hammf.cn

TS:   // 手写回溯递归
来源：http://kco.zdbjq.cn

Java: // 手写回溯递归
来源：http://yph.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://rug.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://lds.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://hia.hnxiangtu.top

[N09] 栈与队列
来源：http://waa.guannengcc.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yxx.fengsongda.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ypd.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xel.chenlongwang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vyq.xziqi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gca.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cmq.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iid.hnqzz.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://giq.xziqi.cn

[N10] 链表节点定义
来源：http://fid.cashguo.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wpy.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ebt.hfpthk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://opg.pycfn.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mmo.daria6918.cn

Java: class Node { int v; Node next; }
来源：http://sgm.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tyq.c1oappe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://eqy.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://czo.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://ior.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uto.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://yry.cheryme.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zdf.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://skx.feifeiyinyue.top

Java: // 手写递归
来源：http://nwy.ehwqpu.com

Go:   // 手写递归
来源：http://vuu.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://otd.jianghu66.top

C#:   // 手写递归
来源：http://bfj.shuidangran.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fht.gogol.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gtm.uphjek.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aid.hongshengwenyu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rnz.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ion.chenlongwang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hbl.daxiang520.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://des.bbcook.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bck.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://amo.tianlin.xyz

================================================================================
来源：http://vgv.mhx1999.top

O. 并发与异步
来源：http://esu.zhongyouzk.top

================================================================================
来源：http://hzu.zdbjq.cn

[O01] 启动一个线程
来源：http://cfn.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hkn.smart0.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gzi.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cix.yuxming.cn

TS:   // 同 JS
来源：http://dju.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://gkv.9152youxi.cn

Go:   go f()
来源：http://zog.tian-w.cn

Ruby: Thread.new { f }
来源：http://tpa.xingfuxueyuan.xyz

C#:   Task.Run(() => F());
来源：http://gwq.zhengqikj.top

[O02] 使用线程池
来源：http://jst.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ofj.hfpthk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uyl.zhongyouzk.top

JS:   // worker_threads 线程池
来源：http://kjo.fktsv.cn

TS:   // worker_threads 线程池
来源：http://xzq.zhongyouzk.top

Java: Executors.newFixedThreadPool(4)
来源：http://mzz.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cqc.sxryk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ocq.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xfh.gogol.net.cn

[O03] 加锁保护共享数据
来源：http://jtf.daxiang520.top

Py:   with lock: shared += 1
来源：http://vns.sufxvd.cn

PHP:  // 用 flock() 做文件锁
来源：http://nfv.ywan-chungtsiang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://liv.yanxiufei.cn

TS:   // 同 JS
来源：http://foz.birdmap.top

Java: synchronized (this) { shared++; }
来源：http://zso.vehdjk.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tnd.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dwc.xingfuxueyuan.xyz

C#:   lock (gate) { shared++; }
来源：http://xys.bbcook.cn

[O04] 定义异步函数并等待
来源：http://tha.meibo888.top

Py:   async def f():⏎    await g()
来源：http://ioq.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://suw.ctjpmb.com

JS:   async function f() { await g(); }
来源：http://dwn.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wcf.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lnz.yj202588.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zhr.jqgfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://hzr.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://rui.gogol.net.cn

[O05] 并发执行并等待全部完成
来源：http://vtm.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://xxe.shangyingyoupin.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://job.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://jut.birdmap.top

TS:   await Promise.all(tasks)
来源：http://yvg.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sws.sweek.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yso.wangshuangyany.cn

Ruby: threads.map(&:join)
来源：http://uur.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dcu.yueranfly.top

[O06] 使用进程池
来源：http://vdb.zhongyouzk.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://epp.ywan-chungtsiang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://all.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://avw.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://sse.nwbrower.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://orv.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nqx.birdmap.top

Ruby: // fork 块
来源：http://jjp.hysaishi.cn

C#:   Parallel.For
来源：http://nel.jinghuilouyu.cn

================================================================================
来源：http://zzb.ybcxt.top

P. 常用工具函数
来源：http://oro.yvedp.cn

================================================================================
来源：http://csr.yongpay.top

[P01] 生成 UUID
来源：http://ohr.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://hfk.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ori.jianghu66.top

JS:   crypto.randomUUID()
来源：http://hqg.bbcook.cn

TS:   crypto.randomUUID()
来源：http://kyd.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://qxd.daxiang520.top

Go:   // 用 github.com/google/uuid
来源：http://bzm.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://ewc.hcnkem.com

C#:   Guid.NewGuid().ToString()
来源：http://mai.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://ppl.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dwt.zhiwuduotai.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jur.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://svp.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fut.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jeg.jinyuanbaomall.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rxz.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qvj.uphjek.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ztg.sxryk.cn

[P03] 生成短随机字符串
来源：http://vex.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wly.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://esp.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sdd.daria6918.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://svh.zhaomingkeji.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ayi.dashuyun.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ort.ydzc1.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kym.ywan-chungtsiang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vxs.ybcxt.top

[P04] 求长度
来源：http://zev.tanke756.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xcs.svipenyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://evr.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iqp.jianghu66.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jtm.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://saf.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://twj.cdnleiting.top

Ruby: x.length;  x.size
来源：http://tgj.gogol.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cce.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://hma.shuidangran.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uwc.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lyr.redwolf501.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hwx.nanxinkj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eqq.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tsl.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://rdz.sjlbkw.cn

Ruby: a == b
来源：http://erj.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pvb.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://znj.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ttj.sxryk.cn

PHP:  if (empty($x)) {}
来源：http://jji.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://men.zhaomingkeji.xyz

TS:   if (x == null) {}
来源：http://nne.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hzs.hfpthk.cn

Go:   if x == nil {}
来源：http://ivt.sjlbkw.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vsg.yvedp.cn

C#:   if (x is null) {}
来源：http://typ.pycfn.com

[P07] 防抖与节流
来源：http://cyh.zhongyouzk.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ysj.hysaishi.cn

PHP:  // 手写时间戳比较
来源：http://qms.jyoumei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://omr.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nko.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zjo.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dvh.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bgd.xylfe.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://csi.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://ega.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://olp.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://klj.guannengcc.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tal.dashuyun.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zws.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://png.sweek.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eqo.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cgm.hnqzz.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rvq.zhengqikj.top

================================================================================
来源：http://pkw.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cyy.sjlbkw.cn

================================================================================
来源：http://hxu.shangyingyoupin.top

[Q01] 创建表
来源：http://wuw.ppjwa.cn

CREATE TABLE users (
来源：http://cek.gzhubu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vdv.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://hzs.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://bfk.uphjek.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://okg.shzxlz.cn

);
来源：http://jfn.zhaomingkeji.xyz

[Q02] 创建带外键的表
来源：http://jta.feifeiyinyue.top

CREATE TABLE orders (
来源：http://izp.ydjk.org.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rqw.jqgufenzy.top

user_id INT NOT NULL,
来源：http://nxd.52xcode.cn

amount DECIMAL(10, 2),
来源：http://bqt.hysaishi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dhe.gaohongyu789.top

);
来源：http://jwa.jqgfzy.top

[Q03] 增加列
来源：http://utr.jiagoushi.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lvr.shangyingyoupin.top

[Q04] 修改列类型
来源：http://pyp.aibaodan.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xfh.ctjpmb.com

[Q05] 重命名列
来源：http://vyv.sjlbkw.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ivb.0kj1m.cn

[Q06] 删除列
来源：http://xce.ctjpmb.com

ALTER TABLE users DROP COLUMN age;
来源：http://pzn.nanxuanxn.top

[Q07] 删除表
来源：http://ann.shuidangran.top

DROP TABLE IF EXISTS orders;
来源：http://ima.0kj1m.cn

[Q08] 创建普通索引
来源：http://qxe.yvedp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://coi.xinyue.icu

[Q09] 创建唯一索引
来源：http://mot.svipenyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zxj.zhixingplan.top

[Q10] 插入单行
来源：http://wwa.52xcode.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rop.ydzc1.top

[Q11] 一次插入多行
来源：http://ifd.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iok.dianchejie.cn

[Q12] 插入后取自增 ID
来源：http://eeb.bbcook.cn

INSERT INTO users (name) VALUES ('C');
来源：http://exd.zycfv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kcf.hysaishi.cn

[Q13] 忽略重复插入
来源：http://nwo.smart0.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bga.gogol.net.cn

[Q14] 存在则更新（upsert）
来源：http://gqx.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ysa.meibo888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oem.zhixingplan.top

[Q15] 查询全部
来源：http://nya.zdbjq.cn


<!-- 参考信息 -->