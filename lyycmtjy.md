代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tuo.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://krt.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://pjy.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dbt.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://ysl.jinqigufen.top

[N02] 排序（工程实践用内置实现）
来源：http://xix.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://fob.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wld.zhengqikj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pwn.nanxinkj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jjk.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rzn.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://eah.tarul.cn

Ruby: arr.sort
来源：http://qpc.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://eki.jqgfzy.top

[N03] 快速排序（分治示例）
来源：http://zyz.iojbl.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://egg.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://igy.yj20258.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qyb.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gto.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vln.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gcl.aibaodan.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lrl.9152youxi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kya.daxiang520.top

[N04] 斐波那契数列
来源：http://amo.mhx1999.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ujb.316326.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hkl.hfpthk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://neg.ivvv.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tvw.xziqi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pgp.fanxiaobao.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ggq.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mie.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://npf.birdmap.top

[N05] 最大公约数
来源：http://dxv.ywan-chungtsiang.top

Py:   math.gcd(a, b)
来源：http://qdr.yuxming.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ald.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wgd.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lcv.zhixingplan.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rqq.yuxming.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wjo.zhijiandao.cn

Ruby: a.gcd(b)
来源：http://rde.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sdr.nwbrower.top

[N06] 判断回文字符串
来源：http://gvl.52xcode.cn

Py:   s == s[::-1]
来源：http://mup.sysykeji.top

PHP:  $s === strrev($s);
来源：http://mxs.jyoumei.cn

JS:   s === [...s].reverse().join("")
来源：http://nxq.bjfxy.top

TS:   s === [...s].reverse().join("")
来源：http://ccg.jqgufenzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vwr.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://sdx.tian-w.cn

Ruby: s == s.reverse
来源：http://euh.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lyk.daxiang520.top

[N07] 两数之和（返回下标）
来源：http://bhh.wangdashe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dws.316326.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jhy.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kkq.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://ffw.cqqwz.cn

Java: // 手写 HashMap
来源：http://eeb.gzhubu.top

Go:   // 手写 map[int]int
来源：http://hve.zdbjq.cn

Ruby: // 手写 Hash
来源：http://xlj.gotoacloud.top

C#:   // 手写 Dictionary<int, int>
来源：http://fty.hammf.cn

[N08] 生成全排列
来源：http://dyy.sjlbkw.cn

Py:   itertools.permutations(arr)
来源：http://utj.jqgfzy.top

PHP:  // 手写递归交换
来源：http://lzt.redwolf501.top

JS:   // 手写回溯递归
来源：http://dbg.dianchejie.cn

TS:   // 手写回溯递归
来源：http://tqe.guowangkeji.top

Java: // 手写回溯递归
来源：http://ixt.gotoacloud.top

Go:   // 手写回溯递归
来源：http://ars.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://ilm.wangdashe.top

C#:   // 手写回溯递归
来源：http://kna.cdnleiting.top

[N09] 栈与队列
来源：http://zsn.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tdj.yanxiufei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://afg.chenzaomai.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cqf.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vpz.nwbrower.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ium.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rik.bbcook.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nff.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://orb.yongpay.top

[N10] 链表节点定义
来源：http://uhe.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hvp.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wtw.hnxiangtu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wpf.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dgt.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://xci.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://sga.zhixingplan.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rlf.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xpv.cashguo.top

[N11] 二叉树中序遍历
来源：http://wvu.gaohongyu789.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ntq.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://yop.cdnleiting.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qfh.gogol.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ozv.daria6918.cn

Java: // 手写递归
来源：http://yew.snrcjt.cn

Go:   // 手写递归
来源：http://afk.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uns.jinqigufen.top

C#:   // 手写递归
来源：http://svj.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wfo.hnxiangtu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lim.nanxinkj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dlg.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://heh.tianlin.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aqr.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gro.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://egh.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://okx.kuanghao11.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jll.vqdsnc.cn

================================================================================
来源：http://epa.tianlin.xyz

O. 并发与异步
来源：http://ewn.snrcjt.cn

================================================================================
来源：http://dpt.wangshuangyany.cn

[O01] 启动一个线程
来源：http://bjq.cqqwz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tuj.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sxc.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ddx.bjfxy.top

TS:   // 同 JS
来源：http://vuo.tianlin.xyz

Java: new Thread(() -> f()).start()
来源：http://aae.redwolf501.top

Go:   go f()
来源：http://slp.daxiang520.top

Ruby: Thread.new { f }
来源：http://zql.ppjwa.cn

C#:   Task.Run(() => F());
来源：http://swn.cqqwz.cn

[O02] 使用线程池
来源：http://ggi.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dtn.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rfz.hammf.cn

JS:   // worker_threads 线程池
来源：http://vdz.gaohongyu789.top

TS:   // worker_threads 线程池
来源：http://ryc.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://vwp.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mzw.ywan-chungtsiang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://svf.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://czi.chenjidiqi.icu

[O03] 加锁保护共享数据
来源：http://wrc.bjfxy.top

Py:   with lock: shared += 1
来源：http://sgh.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://isa.zhiwuduotai.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://byk.yongpay.top

TS:   // 同 JS
来源：http://hog.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://pla.nanxinkj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lny.ehwqpu.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://qgw.jqgufenzy.top

C#:   lock (gate) { shared++; }
来源：http://wao.xuanzx.com

[O04] 定义异步函数并等待
来源：http://lkh.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://vyl.hnxiangtu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lzi.sxryk.cn

JS:   async function f() { await g(); }
来源：http://gwx.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xna.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://btj.fzhhl.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://djl.nanxuanxn.top

Ruby: # 用 Fiber 或 async gem
来源：http://dhq.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://sjd.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://gwg.guannengcc.top

Py:   asyncio.gather(*tasks)
来源：http://xbd.zhiwuduotai.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vlt.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://ccp.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://acb.aizwys.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lvd.xingfuxueyuan.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uos.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://uqu.yongpay.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rtn.fzhhl.top

[O06] 使用进程池
来源：http://rak.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lso.jinqigufen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wbb.yj20258.top

JS:   // child_process / cluster 模块
来源：http://eav.gzhubu.top

TS:   // child_process / cluster 模块
来源：http://qyf.ydzc1.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hfo.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lym.yangfankeji.com

Ruby: // fork 块
来源：http://yzw.aizwys.cn

C#:   Parallel.For
来源：http://kjk.nanxinkj.top

================================================================================
来源：http://zjm.fanxiaobao.xyz

P. 常用工具函数
来源：http://omm.svipenyu.cn

================================================================================
来源：http://cwj.mhx1999.top

[P01] 生成 UUID
来源：http://ljk.guannengcc.top

Py:   str(uuid.uuid4())
来源：http://eqz.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mxp.tian-w.cn

JS:   crypto.randomUUID()
来源：http://qdg.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://bvi.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://znm.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://nvm.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://ctj.dashuyun.cn

C#:   Guid.NewGuid().ToString()
来源：http://elf.jiagoushi.top

[P02] MD5 / SHA256 摘要
来源：http://pxd.daria6918.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xpu.zhiwuduotai.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nmu.hammf.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vdw.cashguo.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kon.nanxinkj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fqw.chenjidiqi.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pqd.9152youxi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ubg.hnxiangtu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://phq.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://rub.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ehd.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yxf.gzhubu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nkx.yuanzhike.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tuo.chenjidiqi.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jce.yj202588.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iyx.birdmap.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ukl.zdqjudy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gjy.bjfxy.top

[P04] 求长度
来源：http://pcr.yanxiufei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gwr.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mow.vqdsnc.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://arh.jinghuilouyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lan.vqdsnc.cn

Java: list.size();  map.size();  s.length()
来源：http://eis.shanyushiyangtech.top

Go:   len(arr);  len(m)
来源：http://jph.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://ktp.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://tjl.fehbvm.com

[P05] 判断两个对象内容是否相等
来源：http://vka.meibo888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ffz.yongpay.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lka.feifeiyinyue.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ogf.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aur.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gya.epnwcf.com

Go:   reflect.DeepEqual(a, b)
来源：http://mld.svipenyu.cn

Ruby: a == b
来源：http://bcg.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xbz.sufxvd.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ogt.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wsc.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://vbh.nanxinkj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bqi.ctjpmb.com

TS:   if (x == null) {}
来源：http://obw.xuanzx.com

Java: if (x == null || x.isEmpty()) {}
来源：http://hfl.snrcjt.cn

Go:   if x == nil {}
来源：http://ghg.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pfy.epnwcf.com

C#:   if (x is null) {}
来源：http://sgs.9152youxi.cn

[P07] 防抖与节流
来源：http://mzg.hesvh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zkd.uphjek.com

PHP:  // 手写时间戳比较
来源：http://wnp.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://phf.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://twd.nwbrower.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zto.nwbrower.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tso.zycfv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ncr.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://byi.zhixingplan.top

[P08] 处理浮点精度问题
来源：http://tfj.xylfe.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jsa.xinyue.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tqe.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://peo.yanxiufei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nsu.yfazqb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ajo.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pbw.sxryk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jlx.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://muc.zhixingplan.top

================================================================================
来源：http://tws.fktsv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tqa.ydjk.org.cn

================================================================================
来源：http://vbz.hywenlv.cn

[Q01] 创建表
来源：http://zpx.316326.xyz

CREATE TABLE users (
来源：http://sqy.yonumen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kch.jyoumei.cn

name VARCHAR(50) NOT NULL,
来源：http://rcu.xuanzx.com

email VARCHAR(100) UNIQUE,
来源：http://ufx.hysaishi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://csn.wangdashe.top

);
来源：http://ppb.uphjek.com

[Q02] 创建带外键的表
来源：http://zvd.hnqzz.top

CREATE TABLE orders (
来源：http://oye.zhaomingkeji.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dbr.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://fdh.shangyingyoupin.top

amount DECIMAL(10, 2),
来源：http://nec.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sww.svipenyu.cn

);
来源：http://lzq.gotoacloud.top

[Q03] 增加列
来源：http://rno.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hcu.yongpay.top

[Q04] 修改列类型
来源：http://vfg.redwolf501.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ijy.yj202588.top

[Q05] 重命名列
来源：http://gid.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://afz.tarul.cn

[Q06] 删除列
来源：http://ehd.pengpengdd.cyou

ALTER TABLE users DROP COLUMN age;
来源：http://zgv.jqgfzy.top

[Q07] 删除表
来源：http://wjm.316326.xyz

DROP TABLE IF EXISTS orders;
来源：http://yfm.cdnleiting.top

[Q08] 创建普通索引
来源：http://ntq.cdnleiting.top

CREATE INDEX idx_users_email ON users(email);
来源：http://izf.pycfn.com

[Q09] 创建唯一索引
来源：http://ifi.yfazqb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://abn.jinghuilouyu.cn

[Q10] 插入单行
来源：http://qxt.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://feo.yongpay.top

[Q11] 一次插入多行
来源：http://tyq.hesvh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lee.jlsjyb.cn

[Q12] 插入后取自增 ID
来源：http://mxh.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cns.zdbjq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cwb.nanxinkj.top

[Q13] 忽略重复插入
来源：http://dne.gaohongyu789.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tkx.nwbrower.top

[Q14] 存在则更新（upsert）
来源：http://ibr.zhaomingkeji.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uif.chenzaomai.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dpf.c1oappe.top

[Q15] 查询全部
来源：http://pbt.yvedp.cn

SELECT * FROM users;
来源：http://hqj.ydzc1.top

[Q16] 查询指定列
来源：http://jhv.feifeiyinyue.top

SELECT id, name FROM users;
来源：http://kxz.tanke756.top

[Q17] 条件查询
来源：http://vbc.yj202588.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://epd.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://cmt.zhoulong.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qnd.gzhubu.top

[Q19] 范围查询
来源：http://sns.hysaishi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ald.jinqigufen.top

[Q20] IN 列表
来源：http://irs.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rdi.fktsv.cn

[Q21] 空值判断
来源：http://pfq.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uwx.yj20258.top

[Q22] 排序
来源：http://lgf.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sct.kuanghao11.cn

[Q23] 分页
来源：http://xgo.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fdy.feifeiyinyue.top

[Q24] 去重
来源：http://ccf.zhengqikj.top

SELECT DISTINCT city FROM users;
来源：http://fev.fehbvm.com

[Q25] 只取前 N 条
来源：http://lfz.cqqwz.cn


<!-- 参考信息 -->