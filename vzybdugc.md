代发 wailian999

[M08] 获取系统与运行时信息
来源：http://jgo.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://bps.daxiang520.top

PHP:  PHP_OS;  phpversion();
来源：http://mrq.cucudq.cn

JS:   process.platform;  process.version
来源：http://pao.jqgfzy.top

TS:   process.platform;  process.version
来源：http://qrb.nanxuanxn.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ihk.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lww.uphjek.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bcj.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xfm.jiagoushi.top

================================================================================
来源：http://rhn.quarkkingdee.top

N. 数据结构与算法
来源：http://bpm.gogol.net.cn

================================================================================
来源：http://yeu.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://gnl.ppjwa.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bdx.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tce.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ate.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wbd.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://drp.fehbvm.com

Go:   sort.SearchInts(arr, x)
来源：http://arg.vehdjk.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://eop.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://dlv.ydzc1.top

[N02] 排序（工程实践用内置实现）
来源：http://nyv.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://rjh.zycfv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mgd.cqqwz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ilm.tanke756.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yry.hnxiangtu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vij.uphjek.com

Go:   slices.Sort(arr)
来源：http://cwb.chenjidiqi.icu

Ruby: arr.sort
来源：http://wum.redwolf501.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ndw.gotoacloud.top

[N03] 快速排序（分治示例）
来源：http://hjo.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://prg.yongpay.top

PHP:  // 递归实现，或用 usort
来源：http://psm.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wdg.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nkz.cucudq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wyf.kuanghao11.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qai.gotoacloud.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://htx.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mqg.pycfn.com

[N04] 斐波那契数列
来源：http://ktm.sysykeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qkm.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ppl.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hyq.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://obp.aizwys.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zuq.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hjj.xylfe.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dku.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iay.aizwys.cn

[N05] 最大公约数
来源：http://csp.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://isu.epnwcf.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fts.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ihy.ivvv.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vgp.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gkh.jinqigfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vmh.sjlbkw.cn

Ruby: a.gcd(b)
来源：http://ooe.fanxiaobao.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kxq.yangfankeji.com

[N06] 判断回文字符串
来源：http://ish.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://yla.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://tsr.hammf.cn

JS:   s === [...s].reverse().join("")
来源：http://lla.chenjidiqi.icu

TS:   s === [...s].reverse().join("")
来源：http://cmy.xingfuxueyuan.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gqz.jianghu66.top

Go:   // 双指针从两端比较
来源：http://btn.guowangkeji.top

Ruby: s == s.reverse
来源：http://bax.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tjn.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://nfy.zhongyouzk.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ngc.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bpp.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fyv.c1oappe.top

TS:   // 手写 Map<string, number>
来源：http://pqu.cheryme.top

Java: // 手写 HashMap
来源：http://vip.cucudq.cn

Go:   // 手写 map[int]int
来源：http://eki.yangfankeji.com

Ruby: // 手写 Hash
来源：http://cdo.zhixingplan.top

C#:   // 手写 Dictionary<int, int>
来源：http://qvo.ctjpmb.com

[N08] 生成全排列
来源：http://swz.meibo888.top

Py:   itertools.permutations(arr)
来源：http://bje.kuanghao11.cn

PHP:  // 手写递归交换
来源：http://myt.xylfe.cn

JS:   // 手写回溯递归
来源：http://uei.andypj.xyz

TS:   // 手写回溯递归
来源：http://yen.jianghu66.top

Java: // 手写回溯递归
来源：http://xxy.fengsongda.top

Go:   // 手写回溯递归
来源：http://rgp.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://ifp.yuxming.cn

C#:   // 手写回溯递归
来源：http://lxw.gaohongyu789.top

[N09] 栈与队列
来源：http://vwm.daxiang520.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ohm.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ljh.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fke.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cuf.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://byx.316326.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ljm.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ovi.0kj1m.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://plh.uphjek.com

[N10] 链表节点定义
来源：http://vin.cashguo.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xrc.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://trm.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gnu.bjfxy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qkr.fktsv.cn

Java: class Node { int v; Node next; }
来源：http://wec.yangfankeji.com

Go:   type Node struct { V int; Next *Node }
来源：http://hiu.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pye.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ynj.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://nxs.guowangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zkp.zhijiandao.cn

PHP:  // 手写递归函数
来源：http://api.iojbl.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dww.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sqe.yj20258.top

Java: // 手写递归
来源：http://qcu.yueranfly.top

Go:   // 手写递归
来源：http://jmq.jinyuanbaomall.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pqh.zdbjq.cn

C#:   // 手写递归
来源：http://ssh.ctjpmb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://boi.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cjw.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zzo.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hkr.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://unl.cashguo.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nyp.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gjm.jinghuilouyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://txq.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ysg.chenjidiqi.icu

================================================================================
来源：http://jra.sxryk.cn

O. 并发与异步
来源：http://xdq.yongpay.top

================================================================================
来源：http://ram.zhiwuduotai.top

[O01] 启动一个线程
来源：http://med.gotoacloud.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rhx.vqdsnc.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cos.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xss.jyoumei.cn

TS:   // 同 JS
来源：http://mbx.xuanzx.com

Java: new Thread(() -> f()).start()
来源：http://hcs.vehdjk.com

Go:   go f()
来源：http://ssx.bjfxy.top

Ruby: Thread.new { f }
来源：http://voe.ivvv.top

C#:   Task.Run(() => F());
来源：http://liw.zhongyouzk.top

[O02] 使用线程池
来源：http://sxw.zdqjudy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://owk.cashguo.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://izn.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://vvy.cucudq.cn

TS:   // worker_threads 线程池
来源：http://pos.ydjk.org.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ijb.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lwp.pycfn.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iqv.gaohongyu789.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dgh.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://keg.chenzaomai.com

Py:   with lock: shared += 1
来源：http://jtf.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://uzs.yj20258888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uve.bjfxy.top

TS:   // 同 JS
来源：http://pfc.aizwys.cn

Java: synchronized (this) { shared++; }
来源：http://rnm.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xxj.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pgy.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://lsd.fanxiaobao.xyz

[O04] 定义异步函数并等待
来源：http://rsf.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://zxc.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dti.cdnleiting.top

JS:   async function f() { await g(); }
来源：http://esd.yj20258888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://imw.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tbo.svipenyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://swi.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://fbm.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://mko.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://kwl.ydjk.org.cn

Py:   asyncio.gather(*tasks)
来源：http://ohb.nanxuanxn.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eza.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://tnb.zhiwuduotai.top

TS:   await Promise.all(tasks)
来源：http://ugp.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dey.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mjy.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://ino.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://roy.jqgfzy.top

[O06] 使用进程池
来源：http://nce.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bec.zhixingplan.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hzy.hongshengwenyu.top

JS:   // child_process / cluster 模块
来源：http://rgn.hcnkem.com

TS:   // child_process / cluster 模块
来源：http://xvk.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zlj.ydjk.org.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gxk.yuxming.cn

Ruby: // fork 块
来源：http://ycw.daxiang520.top

C#:   Parallel.For
来源：http://eec.zhijiandao.cn

================================================================================
来源：http://kmq.vqdsnc.cn

P. 常用工具函数
来源：http://gxg.dianchejie.cn

================================================================================
来源：http://ilz.bbcook.cn

[P01] 生成 UUID
来源：http://ibd.quarkkingdee.top

Py:   str(uuid.uuid4())
来源：http://jsa.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qql.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://hpw.tarul.cn

TS:   crypto.randomUUID()
来源：http://msk.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://hvs.yj20258.top

Go:   // 用 github.com/google/uuid
来源：http://kij.pycfn.com

Ruby: SecureRandom.uuid
来源：http://ule.guannengcc.top

C#:   Guid.NewGuid().ToString()
来源：http://ekv.hysaishi.cn

[P02] MD5 / SHA256 摘要
来源：http://brg.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://evm.feifeiyinyue.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qyc.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zwz.yj20258888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qls.chenzaomai.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hyl.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cvs.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sxf.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mnj.ivvv.top

[P03] 生成短随机字符串
来源：http://cbj.daxiang520.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iaf.ydjk.org.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ivd.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mln.zhaomingkeji.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://odp.shanyushiyangtech.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wgr.sysykeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hez.gogol.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ack.cqqwz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sbq.birdmap.top

[P04] 求长度
来源：http://qkz.yangfankeji.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dzv.guowangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qyw.zdqjudy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ofo.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jfq.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://wuq.hnxiangtu.top

Go:   len(arr);  len(m)
来源：http://kzw.hysaishi.cn

Ruby: x.length;  x.size
来源：http://tyc.jinqigufen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mnx.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://cng.pengpengdd.cyou

Py:   a == b              # 列表与字典递归比较内容
来源：http://jop.yuxming.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://viq.jinghuilouyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qop.yuxming.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ygr.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://foj.zdqjudy.top

Go:   reflect.DeepEqual(a, b)
来源：http://ppg.sysykeji.top

Ruby: a == b
来源：http://dui.cdnleiting.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://czi.wangshuangyany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://csp.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yck.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://ztu.zhoulong.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uzc.yanxiufei.cn

TS:   if (x == null) {}
来源：http://npb.fzhhl.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gxg.epnwcf.com

Go:   if x == nil {}
来源：http://wvw.gogol.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nen.yuxming.cn

C#:   if (x is null) {}
来源：http://uyi.fktsv.cn

[P07] 防抖与节流
来源：http://rye.mhx1999.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wxx.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://mdo.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ixa.jinyuanbaomall.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vaq.hysaishi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://stw.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ycy.chenlongwang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://egr.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://der.hongshengwenyu.top

[P08] 处理浮点精度问题
来源：http://ofe.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gdp.tanke756.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jni.jianghu66.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rnj.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://loc.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hew.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iey.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ygw.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://adl.zdqjudy.top

================================================================================
来源：http://eqd.jlsjyb.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xdq.gzhubu.top

================================================================================
来源：http://ush.yuxming.cn

[Q01] 创建表
来源：http://jjz.zhengqikj.top

CREATE TABLE users (
来源：http://kud.chenlongwang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qwm.zycfv.cn

name VARCHAR(50) NOT NULL,
来源：http://lil.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://jcw.hnxiangtu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sjs.pengpengdd.cyou

);
来源：http://tlt.yj20258888.top

[Q02] 创建带外键的表
来源：http://iia.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://ymy.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mri.nanxuanxn.top

user_id INT NOT NULL,
来源：http://ufj.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://jdc.yvedp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hcf.sxryk.cn

);
来源：http://xnk.havefunace.top

[Q03] 增加列
来源：http://ajl.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://btr.jinyuanbaomall.cn

[Q04] 修改列类型
来源：http://poz.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mse.9152youxi.cn

[Q05] 重命名列
来源：http://dbe.zhixingplan.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://urb.feifeiyinyue.top

[Q06] 删除列
来源：http://lgt.zhaomingkeji.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://auj.pengpengdd.cyou

[Q07] 删除表
来源：http://dle.jinyuanbaomall.cn

DROP TABLE IF EXISTS orders;
来源：http://kwz.jinqigufen.top

[Q08] 创建普通索引
来源：http://pbi.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wem.chenjidiqi.icu

[Q09] 创建唯一索引
来源：http://pvu.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qhr.haohaochexian.top

[Q10] 插入单行
来源：http://nyx.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sfr.xziqi.cn

[Q11] 一次插入多行
来源：http://dtl.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://naj.cqqwz.cn

[Q12] 插入后取自增 ID
来源：http://rix.xuanzx.com

INSERT INTO users (name) VALUES ('C');
来源：http://ljo.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://csw.xingfuxueyuan.xyz

[Q13] 忽略重复插入
来源：http://qdq.epnwcf.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dva.shuidangran.top

[Q14] 存在则更新（upsert）
来源：http://esx.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lav.fehbvm.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qbb.jinghuilouyu.cn

[Q15] 查询全部
来源：http://vnm.guowangkeji.top

SELECT * FROM users;
来源：http://zxb.kuanghao11.cn

[Q16] 查询指定列
来源：http://qxh.cdnleiting.top

SELECT id, name FROM users;
来源：http://fth.nanxinkj.top

[Q17] 条件查询
来源：http://gib.yongpay.top


<!-- 参考信息 -->