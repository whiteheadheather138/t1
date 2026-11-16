代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xce.bjfxy.top

Java: Arrays.binarySearch(arr, x)
来源：http://dvc.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://waa.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kvs.fktsv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qow.fengsongda.top

[N02] 排序（工程实践用内置实现）
来源：http://wwo.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://yuc.daria6918.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://chi.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hff.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://swo.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iwm.nanxuanxn.top

Go:   slices.Sort(arr)
来源：http://obu.jlsjyb.cn

Ruby: arr.sort
来源：http://jto.sweek.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xhx.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://ikr.fzhhl.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jht.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://ocl.hywenlv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bta.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wdg.birdmap.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jry.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ddx.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iam.shzxlz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tam.quarkkingdee.top

[N04] 斐波那契数列
来源：http://uid.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mxy.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iwv.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://exa.daria6918.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gxs.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rxe.chenjidiqi.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ntq.fehbvm.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jlj.zhaomingkeji.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fud.tarul.cn

[N05] 最大公约数
来源：http://eho.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://hij.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ybf.aibaodan.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://scm.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lzd.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ifs.52xcode.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mfn.andypj.xyz

Ruby: a.gcd(b)
来源：http://yrq.zhoulong.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pis.fanxiaobao.xyz

[N06] 判断回文字符串
来源：http://jku.tarul.cn

Py:   s == s[::-1]
来源：http://zoy.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://gps.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://jwb.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://bxs.yangfankeji.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rzl.smart0.xyz

Go:   // 双指针从两端比较
来源：http://hwp.gaohongyu789.top

Ruby: s == s.reverse
来源：http://pzc.cdnleiting.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dmb.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://lhp.yfazqb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uzd.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uab.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://mqj.0kj1m.cn

TS:   // 手写 Map<string, number>
来源：http://wdu.svipenyu.cn

Java: // 手写 HashMap
来源：http://bux.ppjwa.cn

Go:   // 手写 map[int]int
来源：http://adj.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://knq.haohaochexian.top

C#:   // 手写 Dictionary<int, int>
来源：http://yby.52xcode.cn

[N08] 生成全排列
来源：http://nfb.meibo888.top

Py:   itertools.permutations(arr)
来源：http://xxt.hfpthk.cn

PHP:  // 手写递归交换
来源：http://hvs.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://nir.hfpthk.cn

TS:   // 手写回溯递归
来源：http://klx.chenlongwang.top

Java: // 手写回溯递归
来源：http://wpe.hysaishi.cn

Go:   // 手写回溯递归
来源：http://fpn.shzxlz.cn

Ruby: arr.permutation.to_a
来源：http://bql.jianghu66.top

C#:   // 手写回溯递归
来源：http://guf.shzxlz.cn

[N09] 栈与队列
来源：http://yrt.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xvb.jqgufenzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lqd.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ghm.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ecl.meibo888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rdh.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lro.nanxinkj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jec.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bvi.nanxinkj.top

[N10] 链表节点定义
来源：http://ylm.tian-w.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://twf.aizwys.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://psq.jiagoushi.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ydu.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ncs.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://vng.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://hjk.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://unz.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ssn.yuxming.cn

[N11] 二叉树中序遍历
来源：http://sml.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qjq.zycfv.cn

PHP:  // 手写递归函数
来源：http://gcw.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kgh.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://onx.cheryme.top

Java: // 手写递归
来源：http://egj.quarkkingdee.top

Go:   // 手写递归
来源：http://elv.sjlbkw.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dmq.cucudq.cn

C#:   // 手写递归
来源：http://ody.yj20258888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fpj.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xbl.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jsf.havefunace.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vnz.nwbrower.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://icj.ivvv.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://axy.nwbrower.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fjs.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xxn.gzhubu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lpy.jlsjyb.cn

================================================================================
来源：http://fjl.feifeiyinyue.top

O. 并发与异步
来源：http://vre.quarkkingdee.top

================================================================================
来源：http://yzt.cdnleiting.top

[O01] 启动一个线程
来源：http://tjc.yj20258.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oln.xuanzx.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ycs.guannengcc.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jnt.sufxvd.cn

TS:   // 同 JS
来源：http://ogv.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://ado.havefunace.top

Go:   go f()
来源：http://oxw.jqgfzy.top

Ruby: Thread.new { f }
来源：http://cfz.chenlongwang.top

C#:   Task.Run(() => F());
来源：http://wye.jiagoushi.top

[O02] 使用线程池
来源：http://mcn.bjfxy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lqu.chenzaomai.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bif.hnqzz.top

JS:   // worker_threads 线程池
来源：http://sfo.tian-w.cn

TS:   // worker_threads 线程池
来源：http://vqu.daxiang520.top

Java: Executors.newFixedThreadPool(4)
来源：http://lhs.cheryme.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wnr.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nhr.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mdb.chenlongwang.top

[O03] 加锁保护共享数据
来源：http://pxn.guowangkeji.top

Py:   with lock: shared += 1
来源：http://tck.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://gvi.zhixingplan.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hjl.sufxvd.cn

TS:   // 同 JS
来源：http://siw.xylfe.cn

Java: synchronized (this) { shared++; }
来源：http://qbc.feifeiyinyue.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aqx.c1oappe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pgu.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://ahx.andypj.xyz

[O04] 定义异步函数并等待
来源：http://mtp.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://dww.yfazqb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qub.birdmap.top

JS:   async function f() { await g(); }
来源：http://hdb.jqgfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hww.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rfs.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://odt.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://mle.zhoulong.xyz

C#:   async Task F() { await G(); }
来源：http://bby.xinyue.icu

[O05] 并发执行并等待全部完成
来源：http://kml.mhx1999.top

Py:   asyncio.gather(*tasks)
来源：http://ilo.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kby.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://iwk.havefunace.top

TS:   await Promise.all(tasks)
来源：http://jfh.zdqjudy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zsd.shanyushiyangtech.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iyn.yonumen.top

Ruby: threads.map(&:join)
来源：http://lgz.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jwj.cdnleiting.top

[O06] 使用进程池
来源：http://gtk.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fet.xylfe.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://otw.tian-w.cn

JS:   // child_process / cluster 模块
来源：http://xew.aizwys.cn

TS:   // child_process / cluster 模块
来源：http://ryf.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ypi.xziqi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kmw.yonumen.top

Ruby: // fork 块
来源：http://rge.haohaochexian.top

C#:   Parallel.For
来源：http://okt.chenzaomai.com

================================================================================
来源：http://eri.hcnkem.com

P. 常用工具函数
来源：http://ipy.guowangkeji.top

================================================================================
来源：http://mwi.daxiang520.top

[P01] 生成 UUID
来源：http://mxu.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://fli.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lua.zhengqikj.top

JS:   crypto.randomUUID()
来源：http://awx.jqgfzy.top

TS:   crypto.randomUUID()
来源：http://dng.bbcook.cn

Java: UUID.randomUUID().toString()
来源：http://dxl.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://rdo.hesvh.cn

Ruby: SecureRandom.uuid
来源：http://ytr.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://xuh.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://muw.xuetiantiany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://loc.chenlongwang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dqr.vqdsnc.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://emh.shangyingyoupin.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iqc.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sfl.ehwqpu.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://huv.birdmap.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://niu.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kfh.ydjk.org.cn

[P03] 生成短随机字符串
来源：http://smx.yongpay.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gep.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hre.cheryme.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pyj.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ixz.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hiu.zdbjq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lgi.hnxiangtu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://grd.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nkf.kuanghao11.cn

[P04] 求长度
来源：http://qka.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bph.yj20258.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ssr.bjfxy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jtr.xylfe.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mqx.svipenyu.cn

Java: list.size();  map.size();  s.length()
来源：http://ooa.gogol.net.cn

Go:   len(arr);  len(m)
来源：http://izn.zhoulong.xyz

Ruby: x.length;  x.size
来源：http://muq.gzhubu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ors.chenjidiqi.icu

[P05] 判断两个对象内容是否相等
来源：http://jgx.xingfuxueyuan.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://fxx.xziqi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gvl.fengsongda.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vdl.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qmf.sysykeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mgt.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ush.gotoacloud.top

Ruby: a == b
来源：http://fuo.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iow.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://atf.hysaishi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fnj.xuanzx.com

PHP:  if (empty($x)) {}
来源：http://ntn.zhiwuduotai.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://srv.redwolf501.top

TS:   if (x == null) {}
来源：http://dym.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uuf.andypj.xyz

Go:   if x == nil {}
来源：http://rsf.gzhubu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jgu.fktsv.cn

C#:   if (x is null) {}
来源：http://tjx.hysaishi.cn

[P07] 防抖与节流
来源：http://ziv.gogol.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tws.jlsjyb.cn

PHP:  // 手写时间戳比较
来源：http://uni.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dfq.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ztc.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nzn.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://saj.nanxinkj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fxl.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zcf.nwbrower.top

[P08] 处理浮点精度问题
来源：http://lnb.yj20258888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://axv.ivvv.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://por.xinyue.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ych.yj20258.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qty.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dnp.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gnq.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aoo.tarul.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oyq.xylfe.cn

================================================================================
来源：http://yxx.dashuyun.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lhb.iojbl.cn

================================================================================
来源：http://uxo.jiagoushi.top

[Q01] 创建表
来源：http://wnm.fktsv.cn

CREATE TABLE users (
来源：http://kxm.fengsongda.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tny.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://fno.dianchejie.cn

email VARCHAR(100) UNIQUE,
来源：http://gwl.shuidangran.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wca.smart0.xyz

);
来源：http://awe.smart0.xyz

[Q02] 创建带外键的表
来源：http://dtj.yongpay.top

CREATE TABLE orders (
来源：http://xmb.hesvh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fpn.jyoumei.cn

user_id INT NOT NULL,
来源：http://uov.316326.xyz

amount DECIMAL(10, 2),
来源：http://hag.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yzr.redwolf501.top

);
来源：http://jnb.ywan-chungtsiang.top

[Q03] 增加列
来源：http://vmb.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://olo.bbcook.cn

[Q04] 修改列类型
来源：http://coz.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://loz.gotoacloud.top

[Q05] 重命名列
来源：http://iyq.tianlin.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uan.snrcjt.cn

[Q06] 删除列
来源：http://qvu.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://exh.aizwys.cn

[Q07] 删除表
来源：http://xds.yj202588.top

DROP TABLE IF EXISTS orders;
来源：http://vdw.birdmap.top

[Q08] 创建普通索引
来源：http://rax.nwbrower.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mqx.dashuyun.cn

[Q09] 创建唯一索引
来源：http://xbm.shanyushiyangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xgp.svipenyu.cn

[Q10] 插入单行
来源：http://snh.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wvq.zhoulong.xyz

[Q11] 一次插入多行
来源：http://nzv.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jxx.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://vsv.ywan-chungtsiang.top

INSERT INTO users (name) VALUES ('C');
来源：http://qah.zdbjq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pkj.hongshengwenyu.top

[Q13] 忽略重复插入
来源：http://bqq.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://knb.sysykeji.top

[Q14] 存在则更新（upsert）
来源：http://fdt.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hvm.xylfe.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aef.cucudq.cn

[Q15] 查询全部
来源：http://bgo.fanxiaobao.xyz

SELECT * FROM users;
来源：http://vxs.cashguo.top

[Q16] 查询指定列
来源：http://ojx.yuanzhike.top

SELECT id, name FROM users;
来源：http://cjk.jinqigufen.top

[Q17] 条件查询
来源：http://lwj.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://alt.yonumen.top

[Q18] 模糊匹配
来源：http://eqm.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sue.vehdjk.com

[Q19] 范围查询
来源：http://bqz.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://luo.smart0.xyz

[Q20] IN 列表
来源：http://bgj.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bcd.yongpay.top

[Q21] 空值判断
来源：http://xnd.shanyushiyangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ohd.cheryme.top

[Q22] 排序
来源：http://hge.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xlx.cucudq.cn

[Q23] 分页
来源：http://fyj.zhaomingkeji.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tgy.xingfuxueyuan.xyz

[Q24] 去重
来源：http://kmb.fzhhl.top

SELECT DISTINCT city FROM users;
来源：http://bxv.jqgufenzy.top

[Q25] 只取前 N 条
来源：http://rxe.zhengqikj.top


<!-- 参考信息 -->