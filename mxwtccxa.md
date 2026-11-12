代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://ajw.gotoacloud.top

================================================================================
来源：http://jmh.chenzaomai.com

N. 数据结构与算法
来源：http://hcp.yuxming.cn

================================================================================
来源：http://rmx.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://ctk.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mvv.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ufy.chenzaomai.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jud.epnwcf.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qjx.sjlbkw.cn

Java: Arrays.binarySearch(arr, x)
来源：http://szu.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://zlt.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://gyd.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://ctz.ybcxt.top

[N02] 排序（工程实践用内置实现）
来源：http://hfb.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://knz.cashguo.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lza.yfazqb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://tuu.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cqu.iojbl.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://svw.guowangkeji.top

Go:   slices.Sort(arr)
来源：http://igw.sufxvd.cn

Ruby: arr.sort
来源：http://grh.yvedp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dhj.yj20258.top

[N03] 快速排序（分治示例）
来源：http://lpe.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pmk.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://unm.hcnkem.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hzs.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iun.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cpt.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://odm.jlsjyb.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hpe.aibaodan.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cfc.yvedp.cn

[N04] 斐波那契数列
来源：http://eki.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://npt.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hri.sxryk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wxa.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tpw.hnqzz.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://how.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://due.smart0.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ukp.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sfp.epnwcf.com

[N05] 最大公约数
来源：http://otk.guowangkeji.top

Py:   math.gcd(a, b)
来源：http://abi.wangdashe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xaw.guowangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jks.haohaochexian.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mxo.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://trl.ivvv.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aaq.yanxiufei.cn

Ruby: a.gcd(b)
来源：http://rrl.shuidangran.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://usu.gotoacloud.top

[N06] 判断回文字符串
来源：http://nul.gotoacloud.top

Py:   s == s[::-1]
来源：http://qmi.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://fzw.0kj1m.cn

JS:   s === [...s].reverse().join("")
来源：http://brj.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://cwg.ppjwa.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dxs.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://wmc.hammf.cn

Ruby: s == s.reverse
来源：http://zjb.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rwu.quarkkingdee.top

[N07] 两数之和（返回下标）
来源：http://ohr.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fmk.yueranfly.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jnw.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tva.ivvv.top

TS:   // 手写 Map<string, number>
来源：http://yaf.hammf.cn

Java: // 手写 HashMap
来源：http://hvd.bjfxy.top

Go:   // 手写 map[int]int
来源：http://pef.zhengqikj.top

Ruby: // 手写 Hash
来源：http://byi.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mxb.zhengqikj.top

[N08] 生成全排列
来源：http://ipk.316326.xyz

Py:   itertools.permutations(arr)
来源：http://hvv.jianghu66.top

PHP:  // 手写递归交换
来源：http://klj.nwbrower.top

JS:   // 手写回溯递归
来源：http://tok.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://lny.shanyushiyangtech.top

Java: // 手写回溯递归
来源：http://vff.gotoacloud.top

Go:   // 手写回溯递归
来源：http://wxq.fanxiaobao.xyz

Ruby: arr.permutation.to_a
来源：http://ayz.shanyushiyangkeji.top

C#:   // 手写回溯递归
来源：http://jxk.yueranfly.top

[N09] 栈与队列
来源：http://jow.yueranfly.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dar.guannengcc.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mti.jiagoushi.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hhy.zhengqikj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ovb.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ewt.yj20258888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pbd.yvedp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nhc.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uat.fanxiaobao.xyz

[N10] 链表节点定义
来源：http://cbe.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uyh.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cgk.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hnz.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://udl.pycfn.com

Java: class Node { int v; Node next; }
来源：http://ukf.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://npq.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qwi.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hmz.yongpay.top

[N11] 二叉树中序遍历
来源：http://sks.quarkkingdee.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://edj.zhengqikj.top

PHP:  // 手写递归函数
来源：http://wxk.snrcjt.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wex.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cpc.shzxlz.cn

Java: // 手写递归
来源：http://mhq.fzhhl.top

Go:   // 手写递归
来源：http://gng.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kca.tian-w.cn

C#:   // 手写递归
来源：http://cyg.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hib.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lst.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yuf.aizwys.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tin.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ejd.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://icz.ivvv.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yrj.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zka.jianghu66.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wph.kuanghao11.cn

================================================================================
来源：http://nou.chenzaomai.com

O. 并发与异步
来源：http://trw.0kj1m.cn

================================================================================
来源：http://enm.yj202588.top

[O01] 启动一个线程
来源：http://fnr.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yez.feifeiyinyue.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ndv.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vzc.nanxuanxn.top

TS:   // 同 JS
来源：http://qof.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://vad.gzhubu.top

Go:   go f()
来源：http://osy.fengsongda.top

Ruby: Thread.new { f }
来源：http://ups.birdmap.top

C#:   Task.Run(() => F());
来源：http://aqq.ctjpmb.com

[O02] 使用线程池
来源：http://cuq.ydjk.org.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vex.chenzaomai.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://azl.zhixingplan.top

JS:   // worker_threads 线程池
来源：http://zwp.yfazqb.com

TS:   // worker_threads 线程池
来源：http://kxp.jyoumei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nye.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://svi.cashguo.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ncp.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bdp.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://vqa.jqgfzy.top

Py:   with lock: shared += 1
来源：http://npv.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://qtv.cdnleiting.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ycx.redwolf501.top

TS:   // 同 JS
来源：http://zim.fzhhl.top

Java: synchronized (this) { shared++; }
来源：http://bwg.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bve.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sns.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://gco.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://hoz.gaohongyu789.top

Py:   async def f():⏎    await g()
来源：http://pvh.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ztd.gzhubu.top

JS:   async function f() { await g(); }
来源：http://wpy.yuxming.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://olr.yangfankeji.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ocj.wangshuangyany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rzg.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ubq.yueranfly.top

C#:   async Task F() { await G(); }
来源：http://wqk.yanxiufei.cn

[O05] 并发执行并等待全部完成
来源：http://lir.feifeiyinyue.top

Py:   asyncio.gather(*tasks)
来源：http://pwo.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uui.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://ldt.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://roq.andypj.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jar.hnxiangtu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bkc.kuanghao11.cn

Ruby: threads.map(&:join)
来源：http://qns.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bks.fehbvm.com

[O06] 使用进程池
来源：http://iab.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://btv.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ukt.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://xns.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://pmk.shanyushiyangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mgk.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uvo.yj20258888.top

Ruby: // fork 块
来源：http://dbh.pycfn.com

C#:   Parallel.For
来源：http://djx.xuanzx.com

================================================================================
来源：http://lul.0kj1m.cn

P. 常用工具函数
来源：http://ghl.svipenyu.cn

================================================================================
来源：http://zpm.316326.xyz

[P01] 生成 UUID
来源：http://cwn.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://bnv.mhx1999.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lae.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://ldr.shangyingyoupin.top

TS:   crypto.randomUUID()
来源：http://agy.daxiang520.top

Java: UUID.randomUUID().toString()
来源：http://qrv.yj20258888.top

Go:   // 用 github.com/google/uuid
来源：http://fcs.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://bql.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://fmp.guowangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://vmc.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vbe.ivvv.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://epo.xinyue.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qhm.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ywt.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dsn.yanxiufei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tic.yanxiufei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jhl.tianlin.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fre.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://pts.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sqa.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qeh.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ize.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://chw.sjlbkw.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zjw.dashuyun.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bof.daxiang520.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lvu.xylfe.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eet.gogol.net.cn

[P04] 求长度
来源：http://maq.cqqwz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gwh.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ump.xinyue.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oaj.wangdashe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://scn.chenzaomai.com

Java: list.size();  map.size();  s.length()
来源：http://cgz.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://jrd.ybcxt.top

Ruby: x.length;  x.size
来源：http://sms.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yfo.chenjidiqi.icu

[P05] 判断两个对象内容是否相等
来源：http://rfx.mhx1999.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://emp.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yxg.gaohongyu789.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dcd.shangyingyoupin.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xhh.jqgufenzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wrq.zhaomingkeji.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://dbg.xylfe.cn

Ruby: a == b
来源：http://pls.snrcjt.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yeq.daria6918.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ckv.birdmap.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nes.hnxiangtu.top

PHP:  if (empty($x)) {}
来源：http://kbx.nanxuanxn.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pfa.xuanzx.com

TS:   if (x == null) {}
来源：http://fcy.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://txs.daxiang520.top

Go:   if x == nil {}
来源：http://eof.sjlbkw.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://shv.aizwys.cn

C#:   if (x is null) {}
来源：http://udx.hysaishi.cn

[P07] 防抖与节流
来源：http://etn.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wjf.birdmap.top

PHP:  // 手写时间戳比较
来源：http://pmd.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yyn.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eal.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bmk.gzhubu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vbo.gotoacloud.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zfz.guannengcc.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fsa.nanxinkj.top

[P08] 处理浮点精度问题
来源：http://cud.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://isb.zhiwuduotai.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lsa.pengpengdd.cyou

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iol.hcnkem.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mqa.zhoulong.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mxo.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pks.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://krj.wangdashe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xbm.9152youxi.cn

================================================================================
来源：http://xsu.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ohk.hywenlv.cn

================================================================================
来源：http://wvu.nwbrower.top

[Q01] 创建表
来源：http://okv.bbcook.cn

CREATE TABLE users (
来源：http://byc.zhongyouzk.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zso.zhijiandao.cn

name VARCHAR(50) NOT NULL,
来源：http://vaz.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://akz.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ydf.shanyushiyangtech.top

);
来源：http://ahj.jlsjyb.cn

[Q02] 创建带外键的表
来源：http://otk.haohaochexian.top

CREATE TABLE orders (
来源：http://cvk.wangshuangyany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dtz.mhx1999.top

user_id INT NOT NULL,
来源：http://euc.tian-w.cn

amount DECIMAL(10, 2),
来源：http://ylw.xylfe.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://phu.aibaodan.cn

);
来源：http://rqy.gogol.net.cn

[Q03] 增加列
来源：http://mny.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ptq.redwolf501.top

[Q04] 修改列类型
来源：http://wiz.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://emd.cucudq.cn

[Q05] 重命名列
来源：http://vbl.cashguo.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rsq.zycfv.cn

[Q06] 删除列
来源：http://rta.redwolf501.top

ALTER TABLE users DROP COLUMN age;
来源：http://vbe.shanyushiyangtech.top

[Q07] 删除表
来源：http://gco.yonumen.top

DROP TABLE IF EXISTS orders;
来源：http://ttv.smart0.xyz

[Q08] 创建普通索引
来源：http://ubj.sweek.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sjn.yangfankeji.com

[Q09] 创建唯一索引
来源：http://quq.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vwb.ivvv.top

[Q10] 插入单行
来源：http://jwq.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hwi.jqgfzy.top

[Q11] 一次插入多行
来源：http://weq.pycfn.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nbi.aizwys.cn

[Q12] 插入后取自增 ID
来源：http://jaz.zdbjq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yrg.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xcr.snrcjt.cn

[Q13] 忽略重复插入
来源：http://syi.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pnu.jinqigufen.top

[Q14] 存在则更新（upsert）
来源：http://sva.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rsf.hfpthk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nxv.ydzc1.top

[Q15] 查询全部
来源：http://vfc.0kj1m.cn

SELECT * FROM users;
来源：http://olk.yangfankeji.com

[Q16] 查询指定列
来源：http://whp.feifeiyinyue.top

SELECT id, name FROM users;
来源：http://euz.bjfxy.top

[Q17] 条件查询
来源：http://use.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hrs.cashguo.top

[Q18] 模糊匹配
来源：http://emh.iojbl.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tzw.hongshengwenyu.top

[Q19] 范围查询
来源：http://goo.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ohg.cqqwz.cn

[Q20] IN 列表
来源：http://jcc.sjlbkw.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vtg.ctjpmb.com

[Q21] 空值判断
来源：http://bpz.yfazqb.com


<!-- 参考信息 -->