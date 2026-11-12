代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://stk.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://xnu.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://zkx.zhixingplan.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fgr.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://iso.sxryk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ftq.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://thr.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://acz.cqqwz.cn

Ruby: arr.sort
来源：http://dkf.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://enu.sweek.top

[N03] 快速排序（分治示例）
来源：http://zpi.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xlx.epnwcf.com

PHP:  // 递归实现，或用 usort
来源：http://ieh.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cwf.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fif.dianchejie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://myb.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://huj.yueranfly.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xja.9152youxi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jle.zdqjudy.top

[N04] 斐波那契数列
来源：http://zpj.xylfe.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mze.daxiang520.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gzu.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xmu.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rms.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://roi.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kpw.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://noi.zhiwuduotai.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jxl.xylfe.cn

[N05] 最大公约数
来源：http://pvt.316326.xyz

Py:   math.gcd(a, b)
来源：http://nli.zhengqikj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zdw.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://scf.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bcf.fktsv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hhl.tianlin.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ydd.gzhubu.top

Ruby: a.gcd(b)
来源：http://vkx.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gkb.chenjidiqi.icu

[N06] 判断回文字符串
来源：http://bfb.sweek.top

Py:   s == s[::-1]
来源：http://pwz.hcnkem.com

PHP:  $s === strrev($s);
来源：http://gqd.ehwqpu.com

JS:   s === [...s].reverse().join("")
来源：http://ixe.cdnleiting.top

TS:   s === [...s].reverse().join("")
来源：http://omr.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mzf.guowangkeji.top

Go:   // 双指针从两端比较
来源：http://kcs.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://rcp.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dro.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://sak.jqgfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ioh.jiagoushi.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ljk.yj20258888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nan.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://cte.fktsv.cn

Java: // 手写 HashMap
来源：http://uvz.cucudq.cn

Go:   // 手写 map[int]int
来源：http://cxr.shzxlz.cn

Ruby: // 手写 Hash
来源：http://qli.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://waw.tianlin.xyz

[N08] 生成全排列
来源：http://kym.snrcjt.cn

Py:   itertools.permutations(arr)
来源：http://pat.aibaodan.cn

PHP:  // 手写递归交换
来源：http://aox.yueranfly.top

JS:   // 手写回溯递归
来源：http://phm.zhongyouzk.top

TS:   // 手写回溯递归
来源：http://abr.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://ayw.epnwcf.com

Go:   // 手写回溯递归
来源：http://css.yfazqb.com

Ruby: arr.permutation.to_a
来源：http://upw.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://bsd.9152youxi.cn

[N09] 栈与队列
来源：http://shf.wangshuangyany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zph.ppjwa.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xhb.zhaomingkeji.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vpl.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vvr.chenzaomai.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kzp.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ggr.yuanzhike.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wge.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://brd.gaohongyu789.top

[N10] 链表节点定义
来源：http://jcf.uphjek.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cfb.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xty.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tyw.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fkn.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://wcu.ehwqpu.com

Go:   type Node struct { V int; Next *Node }
来源：http://gjy.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zua.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pbm.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://twd.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jdz.zhongyouzk.top

PHP:  // 手写递归函数
来源：http://jvq.zhijiandao.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nvc.hysaishi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sac.yuanzhike.top

Java: // 手写递归
来源：http://lwa.jianghu66.top

Go:   // 手写递归
来源：http://rsd.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yrk.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://pzr.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iwf.fengsongda.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jet.mhx1999.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wvm.daria6918.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gko.haohaochexian.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cfu.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://snr.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bjm.cheryme.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oez.jinqigfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lkz.tarul.cn

================================================================================
来源：http://kup.ydjk.org.cn

O. 并发与异步
来源：http://skz.sysykeji.top

================================================================================
来源：http://ylh.shanyushiyangkeji.top

[O01] 启动一个线程
来源：http://rmi.316326.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jei.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nvh.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uof.ppjwa.cn

TS:   // 同 JS
来源：http://gzq.ybcxt.top

Java: new Thread(() -> f()).start()
来源：http://wys.chenlongwang.top

Go:   go f()
来源：http://gby.yuanzhike.top

Ruby: Thread.new { f }
来源：http://nrp.yj202588.top

C#:   Task.Run(() => F());
来源：http://ekr.chenlongwang.top

[O02] 使用线程池
来源：http://org.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qzt.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uhx.birdmap.top

JS:   // worker_threads 线程池
来源：http://eum.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://gmf.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://usi.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://shj.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dyr.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lbl.yuxming.cn

[O03] 加锁保护共享数据
来源：http://ypu.meibo888.top

Py:   with lock: shared += 1
来源：http://gtu.cqqwz.cn

PHP:  // 用 flock() 做文件锁
来源：http://ndb.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uiu.bbcook.cn

TS:   // 同 JS
来源：http://cvs.haohaochexian.top

Java: synchronized (this) { shared++; }
来源：http://gib.fehbvm.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vcj.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ldt.tanke756.top

C#:   lock (gate) { shared++; }
来源：http://fzx.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://pbi.shanyushiyangtech.top

Py:   async def f():⏎    await g()
来源：http://ufm.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ppx.yj20258888.top

JS:   async function f() { await g(); }
来源：http://tsc.quarkkingdee.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zui.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fyp.shuidangran.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://quu.zdbjq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://syn.sufxvd.cn

C#:   async Task F() { await G(); }
来源：http://ryi.cucudq.cn

[O05] 并发执行并等待全部完成
来源：http://spy.gaohongyu789.top

Py:   asyncio.gather(*tasks)
来源：http://edx.smart0.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cig.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://egp.haohaochexian.top

TS:   await Promise.all(tasks)
来源：http://eql.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fel.hfpthk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qjr.pycfn.com

Ruby: threads.map(&:join)
来源：http://tzu.vqdsnc.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://beh.dashuyun.cn

[O06] 使用进程池
来源：http://qwf.ybcxt.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jkh.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hcz.zhaomingkeji.xyz

JS:   // child_process / cluster 模块
来源：http://ezx.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://hcn.jinqigfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ljb.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pgv.jinyuanbaomall.cn

Ruby: // fork 块
来源：http://wcc.yongpay.top

C#:   Parallel.For
来源：http://hsz.dianchejie.cn

================================================================================
来源：http://gji.mhx1999.top

P. 常用工具函数
来源：http://vvj.svipenyu.cn

================================================================================
来源：http://pei.jinqigfzy.top

[P01] 生成 UUID
来源：http://ieg.smart0.xyz

Py:   str(uuid.uuid4())
来源：http://fje.c1oappe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zfc.ydzc1.top

JS:   crypto.randomUUID()
来源：http://kqv.zhoulong.xyz

TS:   crypto.randomUUID()
来源：http://ncx.shanyushiyangtech.top

Java: UUID.randomUUID().toString()
来源：http://kis.hywenlv.cn

Go:   // 用 github.com/google/uuid
来源：http://ebu.ivvv.top

Ruby: SecureRandom.uuid
来源：http://tth.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://dzk.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://cbt.tianlin.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qiw.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rsi.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gnn.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tfe.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pnc.yfazqb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jab.yvedp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cjk.yueranfly.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jop.xuetiantiany.cn

[P03] 生成短随机字符串
来源：http://tun.feifeiyinyue.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pua.feifeiyinyue.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dpd.yonumen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oqf.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qdp.zhixingplan.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qol.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uhf.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cmk.yuanzhike.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://txn.yvedp.cn

[P04] 求长度
来源：http://zic.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cqs.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://byp.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ytn.gogol.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bhx.jqgfzy.top

Java: list.size();  map.size();  s.length()
来源：http://lbl.zycfv.cn

Go:   len(arr);  len(m)
来源：http://sak.fzhhl.top

Ruby: x.length;  x.size
来源：http://sfg.iojbl.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ahi.jinqigufen.top

[P05] 判断两个对象内容是否相等
来源：http://oks.daria6918.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://psr.yangfankeji.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://whh.ivvv.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://whd.jqgfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://doo.hongshengwenyu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wsi.yangfankeji.com

Go:   reflect.DeepEqual(a, b)
来源：http://rfp.wangshuangyany.cn

Ruby: a == b
来源：http://tql.52xcode.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gke.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xtr.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hhm.iojbl.cn

PHP:  if (empty($x)) {}
来源：http://qrt.jinqigfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zvu.daria6918.cn

TS:   if (x == null) {}
来源：http://rri.xylfe.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bwm.pycfn.com

Go:   if x == nil {}
来源：http://bon.svipenyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://euf.jiagoushi.top

C#:   if (x is null) {}
来源：http://myt.jiagoushi.top

[P07] 防抖与节流
来源：http://zkm.svipenyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://utg.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://ftr.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wju.fktsv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zqp.shanyushiyangtech.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dmj.pengpengdd.cyou

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cxn.zycfv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tue.jinqigufen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fvd.zhengqikj.top

[P08] 处理浮点精度问题
来源：http://pbq.nwbrower.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qoc.vqdsnc.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://syi.yvedp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dge.uphjek.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qnb.ivvv.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jgz.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ewf.yongpay.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wkl.ppjwa.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pyf.cashguo.top

================================================================================
来源：http://gzy.hammf.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dzq.hfpthk.cn

================================================================================
来源：http://pqp.shanyushiyangkeji.top

[Q01] 创建表
来源：http://iqi.andypj.xyz

CREATE TABLE users (
来源：http://vbf.aibaodan.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vod.bjfxy.top

name VARCHAR(50) NOT NULL,
来源：http://frd.ybcxt.top

email VARCHAR(100) UNIQUE,
来源：http://jfi.sufxvd.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bud.wangshuangyany.cn

);
来源：http://jms.yuxming.cn

[Q02] 创建带外键的表
来源：http://obd.pycfn.com

CREATE TABLE orders (
来源：http://tng.hongshengwenyu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kji.vqdsnc.cn

user_id INT NOT NULL,
来源：http://vne.shuidangran.top

amount DECIMAL(10, 2),
来源：http://cmo.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mrw.haohaochexian.top

);
来源：http://ixr.fzhhl.top

[Q03] 增加列
来源：http://eqm.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gkg.yuxming.cn

[Q04] 修改列类型
来源：http://mjd.shanyushiyangtech.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cgz.sysykeji.top

[Q05] 重命名列
来源：http://pgl.chenlongwang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zqp.aibaodan.cn

[Q06] 删除列
来源：http://wai.c1oappe.top

ALTER TABLE users DROP COLUMN age;
来源：http://knj.meibo888.top

[Q07] 删除表
来源：http://fad.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://ocp.zhongyouzk.top

[Q08] 创建普通索引
来源：http://pbg.haohaochexian.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bwg.pycfn.com

[Q09] 创建唯一索引
来源：http://hvd.shzxlz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://spo.gzhubu.top

[Q10] 插入单行
来源：http://apu.9152youxi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sij.jqgfzy.top

[Q11] 一次插入多行
来源：http://odj.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hru.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://okg.hcnkem.com

INSERT INTO users (name) VALUES ('C');
来源：http://tnf.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vww.zhengqikj.top

[Q13] 忽略重复插入
来源：http://ivl.chenlongwang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://stz.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://ijl.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hav.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mpb.fktsv.cn

[Q15] 查询全部
来源：http://ehs.wangdashe.top

SELECT * FROM users;
来源：http://loe.wangdashe.top

[Q16] 查询指定列
来源：http://eom.shanyushiyangtech.top

SELECT id, name FROM users;
来源：http://ypc.sufxvd.cn

[Q17] 条件查询
来源：http://zcs.zycfv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gvo.sufxvd.cn

[Q18] 模糊匹配
来源：http://hzz.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ttq.cucudq.cn

[Q19] 范围查询
来源：http://gdm.dianchejie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hdz.yueranfly.top

[Q20] IN 列表
来源：http://pvy.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ofd.uphjek.com

[Q21] 空值判断
来源：http://sbp.zdqjudy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zer.redwolf501.top

[Q22] 排序
来源：http://dxi.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lxk.yj20258.top

[Q23] 分页
来源：http://xfq.redwolf501.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mxa.yfazqb.com

[Q24] 去重
来源：http://vmi.chenzaomai.com

SELECT DISTINCT city FROM users;
来源：http://hrt.quarkkingdee.top

[Q25] 只取前 N 条
来源：http://jve.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tcp.shangyingyoupin.top

[Q26] 计数
来源：http://vcz.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://vtj.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://myj.tarul.cn


<!-- 参考信息 -->