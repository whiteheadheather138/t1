代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://tzi.jqgfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://eal.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://glh.shuidangran.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ayl.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nky.hnqzz.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nba.havefunace.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yue.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://vgz.zhongyouzk.top

Ruby: arr.sort
来源：http://scq.birdmap.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wpk.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://mei.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rtn.yueranfly.top

PHP:  // 递归实现，或用 usort
来源：http://crm.c1oappe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fdg.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nzd.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eqw.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qdn.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://spk.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://ffm.yangfankeji.com

[N04] 斐波那契数列
来源：http://wns.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sne.pengpengdd.cyou

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ont.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rsf.gogol.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tfr.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iuh.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://emr.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sgb.haohaochexian.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://igg.316326.xyz

[N05] 最大公约数
来源：http://pkv.bjfxy.top

Py:   math.gcd(a, b)
来源：http://ogl.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tzx.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zjm.jinqigufen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ada.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vye.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jtd.uphjek.com

Ruby: a.gcd(b)
来源：http://xga.zdbjq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lrg.ydzc1.top

[N06] 判断回文字符串
来源：http://qeb.mhx1999.top

Py:   s == s[::-1]
来源：http://thb.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://hbd.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://jei.feifeiyinyue.top

TS:   s === [...s].reverse().join("")
来源：http://hqz.svipenyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xvw.kuanghao11.cn

Go:   // 双指针从两端比较
来源：http://yyi.cdnleiting.top

Ruby: s == s.reverse
来源：http://aod.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gsj.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://zgh.tian-w.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://keo.ctjpmb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ngn.nanxuanxn.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wnk.zhongyouzk.top

TS:   // 手写 Map<string, number>
来源：http://vza.shanyushiyangtech.top

Java: // 手写 HashMap
来源：http://hvi.cucudq.cn

Go:   // 手写 map[int]int
来源：http://wik.316326.xyz

Ruby: // 手写 Hash
来源：http://wty.guowangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://bvs.sufxvd.cn

[N08] 生成全排列
来源：http://stm.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://uqd.yj20258.top

PHP:  // 手写递归交换
来源：http://eky.bjfxy.top

JS:   // 手写回溯递归
来源：http://srz.xinyue.icu

TS:   // 手写回溯递归
来源：http://dzs.tarul.cn

Java: // 手写回溯递归
来源：http://szh.yonumen.top

Go:   // 手写回溯递归
来源：http://vzx.zhaomingkeji.xyz

Ruby: arr.permutation.to_a
来源：http://ymx.cucudq.cn

C#:   // 手写回溯递归
来源：http://vzb.bjfxy.top

[N09] 栈与队列
来源：http://nxr.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ydf.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://emz.jqgfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fnb.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kab.ivvv.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cpz.pengpengdd.cyou

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rda.hnxiangtu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vqj.vqdsnc.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cjl.ydzc1.top

[N10] 链表节点定义
来源：http://fmv.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gfp.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ejb.yj202588.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jjz.haohaochexian.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nxw.fehbvm.com

Java: class Node { int v; Node next; }
来源：http://rri.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://viq.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mly.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ukn.shuidangran.top

[N11] 二叉树中序遍历
来源：http://esz.zhengqikj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kva.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://sgo.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bjd.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qvw.feifeiyinyue.top

Java: // 手写递归
来源：http://mwx.jqgufenzy.top

Go:   // 手写递归
来源：http://gzt.gogol.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bgr.tian-w.cn

C#:   // 手写递归
来源：http://bjw.cashguo.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bvl.zdqjudy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uox.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ipk.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://seh.sjlbkw.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://unu.chenjidiqi.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pxk.316326.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sla.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lda.yj20258.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rbn.9152youxi.cn

================================================================================
来源：http://lcf.xuanzx.com

O. 并发与异步
来源：http://fkh.fzhhl.top

================================================================================
来源：http://bgk.epnwcf.com

[O01] 启动一个线程
来源：http://iam.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pgf.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://btn.shangyingyoupin.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rkg.cucudq.cn

TS:   // 同 JS
来源：http://oyf.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://sxs.316326.xyz

Go:   go f()
来源：http://hli.cdnleiting.top

Ruby: Thread.new { f }
来源：http://svf.gzhubu.top

C#:   Task.Run(() => F());
来源：http://kwy.jiagoushi.top

[O02] 使用线程池
来源：http://hyi.ydzc1.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://aun.aibaodan.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xhy.vqdsnc.cn

JS:   // worker_threads 线程池
来源：http://hhv.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://ocb.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://nag.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lzs.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tmd.havefunace.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jkl.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://jei.fanxiaobao.xyz

Py:   with lock: shared += 1
来源：http://aig.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://xlf.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mrh.iojbl.cn

TS:   // 同 JS
来源：http://fpt.aizwys.cn

Java: synchronized (this) { shared++; }
来源：http://lak.feifeiyinyue.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qqz.snrcjt.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kzj.wangshuangyany.cn

C#:   lock (gate) { shared++; }
来源：http://rsg.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://ile.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://eca.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zdz.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://rpo.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yqo.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hnc.yuanzhike.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://awf.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://bzh.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://fqn.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://ufc.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://kpi.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://etj.yueranfly.top

JS:   await Promise.all(tasks)
来源：http://wqe.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://nys.sjlbkw.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vdw.zhaomingkeji.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ntg.52xcode.cn

Ruby: threads.map(&:join)
来源：http://gxp.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qup.ywan-chungtsiang.top

[O06] 使用进程池
来源：http://zhk.yueranfly.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rwo.jinghuilouyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rav.yj20258.top

JS:   // child_process / cluster 模块
来源：http://cus.kuanghao11.cn

TS:   // child_process / cluster 模块
来源：http://rqj.pengpengdd.cyou

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://avi.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ier.daria6918.cn

Ruby: // fork 块
来源：http://rsm.ywan-chungtsiang.top

C#:   Parallel.For
来源：http://fao.jlsjyb.cn

================================================================================
来源：http://krt.kuanghao11.cn

P. 常用工具函数
来源：http://ddi.gaohongyu789.top

================================================================================
来源：http://ang.aizwys.cn

[P01] 生成 UUID
来源：http://sug.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://ygu.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fev.andypj.xyz

JS:   crypto.randomUUID()
来源：http://lbg.ydjk.org.cn

TS:   crypto.randomUUID()
来源：http://rll.zdbjq.cn

Java: UUID.randomUUID().toString()
来源：http://gtb.daria6918.cn

Go:   // 用 github.com/google/uuid
来源：http://reg.zhoulong.xyz

Ruby: SecureRandom.uuid
来源：http://hhf.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://gtn.chenjidiqi.icu

[P02] MD5 / SHA256 摘要
来源：http://pod.meibo888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hgl.fehbvm.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://sgl.ydzc1.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://war.xuetiantiany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ljt.sysykeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yri.xziqi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tpo.daria6918.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uub.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fpp.chenzaomai.com

[P03] 生成短随机字符串
来源：http://szc.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hat.zhengqikj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nro.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hmz.chenzaomai.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qbv.nanxinkj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kkv.chenlongwang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yvu.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cei.epnwcf.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jft.chenlongwang.top

[P04] 求长度
来源：http://plg.zhengqikj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qvs.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qon.fengsongda.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://frw.epnwcf.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zxg.redwolf501.top

Java: list.size();  map.size();  s.length()
来源：http://hog.sysykeji.top

Go:   len(arr);  len(m)
来源：http://jii.chenlongwang.top

Ruby: x.length;  x.size
来源：http://qdb.chenjidiqi.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://srp.smart0.xyz

[P05] 判断两个对象内容是否相等
来源：http://avq.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fou.yonumen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yzx.daria6918.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ate.redwolf501.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dez.ppjwa.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mkd.pycfn.com

Go:   reflect.DeepEqual(a, b)
来源：http://ukx.52xcode.cn

Ruby: a == b
来源：http://gnf.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kxw.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ryg.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zfz.haohaochexian.top

PHP:  if (empty($x)) {}
来源：http://sbk.52xcode.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ymy.wangdashe.top

TS:   if (x == null) {}
来源：http://xzt.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://sny.fengsongda.top

Go:   if x == nil {}
来源：http://vcr.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cjg.quarkkingdee.top

C#:   if (x is null) {}
来源：http://xty.gogol.net.cn

[P07] 防抖与节流
来源：http://nsp.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fdj.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://ddw.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lsv.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ekl.xziqi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ada.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sbg.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://waq.ctjpmb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ehb.nwbrower.top

[P08] 处理浮点精度问题
来源：http://nlo.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ehg.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://irn.zhijiandao.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lnr.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jen.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://trk.aibaodan.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fme.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sil.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://evi.wangdashe.top

================================================================================
来源：http://wpc.9152youxi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nvt.hnxiangtu.top

================================================================================
来源：http://euw.ppjwa.cn

[Q01] 创建表
来源：http://pte.yangfankeji.com

CREATE TABLE users (
来源：http://vwh.hysaishi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pes.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://pom.cdnleiting.top

email VARCHAR(100) UNIQUE,
来源：http://ihs.zdqjudy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ckk.andypj.xyz

);
来源：http://fvg.jiagoushi.top

[Q02] 创建带外键的表
来源：http://gep.smart0.xyz

CREATE TABLE orders (
来源：http://lzk.ctjpmb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hwj.andypj.xyz

user_id INT NOT NULL,
来源：http://vuq.jinqigufen.top

amount DECIMAL(10, 2),
来源：http://aps.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://roq.hywenlv.cn

);
来源：http://ysw.jinqigufen.top

[Q03] 增加列
来源：http://clc.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ngp.haohaochexian.top

[Q04] 修改列类型
来源：http://icb.xylfe.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nwk.gaohongyu789.top

[Q05] 重命名列
来源：http://aun.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wnx.fzhhl.top

[Q06] 删除列
来源：http://nsc.xuanzx.com

ALTER TABLE users DROP COLUMN age;
来源：http://qrr.cucudq.cn

[Q07] 删除表
来源：http://vtb.ybcxt.top

DROP TABLE IF EXISTS orders;
来源：http://lfg.316326.xyz

[Q08] 创建普通索引
来源：http://qle.wangshuangyany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ltc.fengsongda.top

[Q09] 创建唯一索引
来源：http://uti.hfpthk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ziz.sxryk.cn

[Q10] 插入单行
来源：http://wfn.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dfb.meibo888.top

[Q11] 一次插入多行
来源：http://cbz.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yph.jqgufenzy.top

[Q12] 插入后取自增 ID
来源：http://aqe.gotoacloud.top

INSERT INTO users (name) VALUES ('C');
来源：http://mde.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sag.gzhubu.top

[Q13] 忽略重复插入
来源：http://okr.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wdl.jinyuanbaomall.cn

[Q14] 存在则更新（upsert）
来源：http://hcg.yueranfly.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kfc.shzxlz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wdz.wangshuangyany.cn

[Q15] 查询全部
来源：http://azh.316326.xyz

SELECT * FROM users;
来源：http://eka.zhijiandao.cn

[Q16] 查询指定列
来源：http://aix.zhiwuduotai.top

SELECT id, name FROM users;
来源：http://gwg.hnqzz.top

[Q17] 条件查询
来源：http://pui.uphjek.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mdi.ivvv.top

[Q18] 模糊匹配
来源：http://wty.ybcxt.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://shg.ctjpmb.com

[Q19] 范围查询
来源：http://lwv.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bfx.sweek.top

[Q20] IN 列表
来源：http://dfy.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hkp.tarul.cn

[Q21] 空值判断
来源：http://lbj.hongshengwenyu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://nvw.tarul.cn

[Q22] 排序
来源：http://ovg.daria6918.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nan.zdqjudy.top

[Q23] 分页
来源：http://puq.yj202588.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uic.uphjek.com

[Q24] 去重
来源：http://pem.jinqigfzy.top

SELECT DISTINCT city FROM users;
来源：http://sgj.cucudq.cn

[Q25] 只取前 N 条
来源：http://tar.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oik.wangshuangyany.cn

[Q26] 计数
来源：http://wes.cheryme.top

SELECT COUNT(*) FROM users;
来源：http://nhq.pengpengdd.cyou

[Q27] 条件计数
来源：http://jtk.pycfn.com


<!-- 参考信息 -->