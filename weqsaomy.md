代发 wailian999

[M08] 获取系统与运行时信息
来源：http://rtm.xinyue.icu

Py:   platform.system();  platform.python_version()
来源：http://gmw.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://tjl.tian-w.cn

JS:   process.platform;  process.version
来源：http://gez.zdbjq.cn

TS:   process.platform;  process.version
来源：http://oie.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tzr.hywenlv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tuc.mhx1999.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tck.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://iyv.birdmap.top

================================================================================
来源：http://xev.yj20258888.top

N. 数据结构与算法
来源：http://tjf.quarkkingdee.top

================================================================================
来源：http://kmt.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://lzc.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://qek.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dky.jinqigufen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://maq.iojbl.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jmp.zhoulong.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://djk.kuanghao11.cn

Go:   sort.SearchInts(arr, x)
来源：http://gzn.cashguo.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://oiu.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://cuc.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://lyh.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://etd.zhiwuduotai.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lvz.vehdjk.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://xgq.epnwcf.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://zcs.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yew.yonumen.top

Go:   slices.Sort(arr)
来源：http://uyh.hcnkem.com

Ruby: arr.sort
来源：http://hvg.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://uhv.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://juq.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://evp.yuxming.cn

PHP:  // 递归实现，或用 usort
来源：http://mqu.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://thm.jqgfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://crf.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nbj.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yxa.haohaochexian.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://exy.zycfv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://njb.gzhubu.top

[N04] 斐波那契数列
来源：http://eho.ivvv.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jxi.nwbrower.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xec.zhongyouzk.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rqj.yangfankeji.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tcs.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lws.mhx1999.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://poq.vqdsnc.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pbl.zhongyouzk.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dnh.shuidangran.top

[N05] 最大公约数
来源：http://oag.tian-w.cn

Py:   math.gcd(a, b)
来源：http://kab.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hbn.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dou.kuanghao11.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qzn.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wan.zhixingplan.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ifr.yvedp.cn

Ruby: a.gcd(b)
来源：http://zdv.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pbv.fktsv.cn

[N06] 判断回文字符串
来源：http://pwl.bjfxy.top

Py:   s == s[::-1]
来源：http://dvl.ydjk.org.cn

PHP:  $s === strrev($s);
来源：http://oml.svipenyu.cn

JS:   s === [...s].reverse().join("")
来源：http://arj.chenlongwang.top

TS:   s === [...s].reverse().join("")
来源：http://byn.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lbc.9152youxi.cn

Go:   // 双指针从两端比较
来源：http://jto.yj202588.top

Ruby: s == s.reverse
来源：http://jjm.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hep.c1oappe.top

[N07] 两数之和（返回下标）
来源：http://obt.tian-w.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uvp.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://din.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ufg.sysykeji.top

TS:   // 手写 Map<string, number>
来源：http://ehd.xylfe.cn

Java: // 手写 HashMap
来源：http://gih.haohaochexian.top

Go:   // 手写 map[int]int
来源：http://ihs.316326.xyz

Ruby: // 手写 Hash
来源：http://vfn.birdmap.top

C#:   // 手写 Dictionary<int, int>
来源：http://upo.jyoumei.cn

[N08] 生成全排列
来源：http://awv.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://yzc.aibaodan.cn

PHP:  // 手写递归交换
来源：http://kqg.zhaomingkeji.xyz

JS:   // 手写回溯递归
来源：http://eyw.jinghuilouyu.cn

TS:   // 手写回溯递归
来源：http://ueq.vqdsnc.cn

Java: // 手写回溯递归
来源：http://qrd.hnxiangtu.top

Go:   // 手写回溯递归
来源：http://oxz.jinghuilouyu.cn

Ruby: arr.permutation.to_a
来源：http://wgc.pycfn.com

C#:   // 手写回溯递归
来源：http://ofk.yueranfly.top

[N09] 栈与队列
来源：http://qco.redwolf501.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jqk.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rps.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pqm.ywan-chungtsiang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nws.tianlin.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cre.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xyg.ydzc1.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hhb.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ikw.zhongyouzk.top

[N10] 链表节点定义
来源：http://tes.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ewq.wangdashe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://etw.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://udu.chenzaomai.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xhb.shanyushiyangkeji.top

Java: class Node { int v; Node next; }
来源：http://uzm.dianchejie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ghu.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qcx.ehwqpu.com

C#:   class Node { public int V; public Node? Next; }
来源：http://rpa.fktsv.cn

[N11] 二叉树中序遍历
来源：http://emw.jinghuilouyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qlk.xziqi.cn

PHP:  // 手写递归函数
来源：http://yre.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wfe.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vew.sweek.top

Java: // 手写递归
来源：http://izt.jyoumei.cn

Go:   // 手写递归
来源：http://qcz.vehdjk.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ddm.dashuyun.cn

C#:   // 手写递归
来源：http://esv.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yye.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bml.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lwx.guowangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lwo.ywan-chungtsiang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sec.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ksg.tianlin.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fwo.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mzr.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kbk.ydjk.org.cn

================================================================================
来源：http://reu.xylfe.cn

O. 并发与异步
来源：http://cxx.cucudq.cn

================================================================================
来源：http://foo.havefunace.top

[O01] 启动一个线程
来源：http://qnz.havefunace.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dpj.zdqjudy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qwo.hesvh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fki.jinghuilouyu.cn

TS:   // 同 JS
来源：http://jre.fengsongda.top

Java: new Thread(() -> f()).start()
来源：http://fsn.ybcxt.top

Go:   go f()
来源：http://wun.chenzaomai.com

Ruby: Thread.new { f }
来源：http://gny.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://fdq.ydjk.org.cn

[O02] 使用线程池
来源：http://gqf.zhijiandao.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://doe.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xtq.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://hxj.wangshuangyany.cn

TS:   // worker_threads 线程池
来源：http://bcv.hysaishi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gai.yueranfly.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lbg.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://liv.fktsv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yle.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://nno.tarul.cn

Py:   with lock: shared += 1
来源：http://tsm.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://awd.havefunace.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nwn.zhengqikj.top

TS:   // 同 JS
来源：http://fbg.jinyuanbaomall.cn

Java: synchronized (this) { shared++; }
来源：http://hmb.nanxinkj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fhd.hcnkem.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://fez.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://iqq.ybcxt.top

[O04] 定义异步函数并等待
来源：http://pua.xuetiantiany.cn

Py:   async def f():⏎    await g()
来源：http://mbm.gzhubu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ipu.vehdjk.com

JS:   async function f() { await g(); }
来源：http://icq.xinyue.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://pel.cdnleiting.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kbr.xuanzx.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qzu.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pfd.gogol.net.cn

C#:   async Task F() { await G(); }
来源：http://mdq.aibaodan.cn

[O05] 并发执行并等待全部完成
来源：http://fvv.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://faf.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wmc.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://eeo.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://nzl.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xvb.zhongyouzk.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hgx.daxiang520.top

Ruby: threads.map(&:join)
来源：http://mlf.wangdashe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gvc.hesvh.cn

[O06] 使用进程池
来源：http://obb.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wlh.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sji.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://ehs.iojbl.cn

TS:   // child_process / cluster 模块
来源：http://eds.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://odv.xinyue.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vsp.wangshuangyany.cn

Ruby: // fork 块
来源：http://wfk.xziqi.cn

C#:   Parallel.For
来源：http://enx.xylfe.cn

================================================================================
来源：http://wdk.zhongyouzk.top

P. 常用工具函数
来源：http://ksq.zhijiandao.cn

================================================================================
来源：http://zeo.ppjwa.cn

[P01] 生成 UUID
来源：http://gpp.birdmap.top

Py:   str(uuid.uuid4())
来源：http://pvx.yj20258.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://txu.snrcjt.cn

JS:   crypto.randomUUID()
来源：http://zta.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://sxm.nanxuanxn.top

Java: UUID.randomUUID().toString()
来源：http://fwh.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://emt.zycfv.cn

Ruby: SecureRandom.uuid
来源：http://qnp.gzhubu.top

C#:   Guid.NewGuid().ToString()
来源：http://hzw.ydzc1.top

[P02] MD5 / SHA256 摘要
来源：http://gxy.xingfuxueyuan.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xac.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://pvr.haohaochexian.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://htu.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hui.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pfz.pengpengdd.cyou

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://otu.sxryk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hbm.nanxinkj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dpd.gogol.net.cn

[P03] 生成短随机字符串
来源：http://vii.dashuyun.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bxu.jinqigfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qmo.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aee.andypj.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aat.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://crw.nanxinkj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gsn.vqdsnc.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hfa.zhixingplan.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kmi.shanyushiyangtech.top

[P04] 求长度
来源：http://svu.zhengqikj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ptl.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lfb.fanxiaobao.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://euf.nanxinkj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ygi.andypj.xyz

Java: list.size();  map.size();  s.length()
来源：http://kxx.nwbrower.top

Go:   len(arr);  len(m)
来源：http://rkz.jinqigufen.top

Ruby: x.length;  x.size
来源：http://knj.chenjidiqi.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://aoa.snrcjt.cn

[P05] 判断两个对象内容是否相等
来源：http://mwr.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://upm.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://muc.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aok.gotoacloud.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iop.nanxuanxn.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fjj.ybcxt.top

Go:   reflect.DeepEqual(a, b)
来源：http://ijg.sxryk.cn

Ruby: a == b
来源：http://rie.316326.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ojv.zycfv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uto.vqdsnc.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jai.jyoumei.cn

PHP:  if (empty($x)) {}
来源：http://wci.iojbl.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cga.uphjek.com

TS:   if (x == null) {}
来源：http://hqs.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://afp.9152youxi.cn

Go:   if x == nil {}
来源：http://qwd.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dby.ydjk.org.cn

C#:   if (x is null) {}
来源：http://oto.yj20258888.top

[P07] 防抖与节流
来源：http://owy.hcnkem.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jwp.vehdjk.com

PHP:  // 手写时间戳比较
来源：http://jqs.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oxh.ybcxt.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ciz.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ywj.sufxvd.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ody.guowangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vym.birdmap.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://snl.zhixingplan.top

[P08] 处理浮点精度问题
来源：http://rif.tianlin.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rnc.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vvt.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ewx.jinghuilouyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eem.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cjb.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nyi.vehdjk.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dnj.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mdy.shanyushiyangtech.top

================================================================================
来源：http://pwr.yj20258888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lqx.gotoacloud.top

================================================================================
来源：http://jmf.fanxiaobao.xyz

[Q01] 创建表
来源：http://ubx.chenzaomai.com

CREATE TABLE users (
来源：http://hbw.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://acj.xylfe.cn

name VARCHAR(50) NOT NULL,
来源：http://lum.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://osk.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gbq.chenjidiqi.icu

);
来源：http://xpl.jiagoushi.top

[Q02] 创建带外键的表
来源：http://epq.yj20258888.top

CREATE TABLE orders (
来源：http://jfq.mhx1999.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fwp.guowangkeji.top

user_id INT NOT NULL,
来源：http://jac.xingfuxueyuan.xyz

amount DECIMAL(10, 2),
来源：http://svw.guannengcc.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jvr.wangdashe.top

);
来源：http://gca.quarkkingdee.top

[Q03] 增加列
来源：http://mgw.gaohongyu789.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://szf.0kj1m.cn

[Q04] 修改列类型
来源：http://oqk.aibaodan.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zob.jlsjyb.cn

[Q05] 重命名列
来源：http://afm.uphjek.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qsm.hammf.cn

[Q06] 删除列
来源：http://wcx.ywan-chungtsiang.top

ALTER TABLE users DROP COLUMN age;
来源：http://sra.bbcook.cn

[Q07] 删除表
来源：http://ulo.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://cqh.0kj1m.cn

[Q08] 创建普通索引
来源：http://qqz.quarkkingdee.top

CREATE INDEX idx_users_email ON users(email);
来源：http://oxr.daria6918.cn

[Q09] 创建唯一索引
来源：http://gjq.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://msc.ivvv.top

[Q10] 插入单行
来源：http://fpb.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cgo.pycfn.com

[Q11] 一次插入多行
来源：http://voe.redwolf501.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://msu.jiagoushi.top

[Q12] 插入后取自增 ID
来源：http://zxa.xingfuxueyuan.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://ouv.aizwys.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hmo.xuetiantiany.cn

[Q13] 忽略重复插入
来源：http://jio.sysykeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ggt.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://sgj.guannengcc.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sty.zhijiandao.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ioo.jinqigfzy.top

[Q15] 查询全部
来源：http://elf.tian-w.cn

SELECT * FROM users;
来源：http://czj.yueranfly.top

[Q16] 查询指定列
来源：http://kva.xuanzx.com

SELECT id, name FROM users;
来源：http://nxp.mhx1999.top

[Q17] 条件查询
来源：http://wur.yj202588.top


<!-- 参考信息 -->