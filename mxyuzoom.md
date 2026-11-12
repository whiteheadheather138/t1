代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://ets.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://pjd.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://sgm.zhaomingkeji.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wrg.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://deu.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nbo.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lpw.uphjek.com

Go:   slices.Sort(arr)
来源：http://mls.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://rrz.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://tdb.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://hyo.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mxb.yj202588.top

PHP:  // 递归实现，或用 usort
来源：http://zer.52xcode.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ssz.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oht.shangyingyoupin.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://arh.vqdsnc.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rnn.zhengqikj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xgi.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://gxw.ehwqpu.com

[N04] 斐波那契数列
来源：http://xde.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bea.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qjk.wangshuangyany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nur.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pfz.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fgb.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gif.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vqb.aibaodan.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sqx.zycfv.cn

[N05] 最大公约数
来源：http://svn.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://qwb.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mfe.shuidangran.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uhz.tianlin.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tfd.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://avz.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gfp.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://owy.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uui.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://zza.jlsjyb.cn

Py:   s == s[::-1]
来源：http://dam.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://uiz.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://two.daria6918.cn

TS:   s === [...s].reverse().join("")
来源：http://twn.andypj.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iul.guannengcc.top

Go:   // 双指针从两端比较
来源：http://idb.ywan-chungtsiang.top

Ruby: s == s.reverse
来源：http://qjs.vqdsnc.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jng.epnwcf.com

[N07] 两数之和（返回下标）
来源：http://mfz.hnxiangtu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zxk.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wfa.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mzy.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://lgo.jyoumei.cn

Java: // 手写 HashMap
来源：http://qet.hcnkem.com

Go:   // 手写 map[int]int
来源：http://fsq.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://keg.andypj.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://bqg.cucudq.cn

[N08] 生成全排列
来源：http://aty.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://lqq.sufxvd.cn

PHP:  // 手写递归交换
来源：http://xzq.havefunace.top

JS:   // 手写回溯递归
来源：http://iul.hongshengwenyu.top

TS:   // 手写回溯递归
来源：http://ahd.quarkkingdee.top

Java: // 手写回溯递归
来源：http://ntn.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://lyf.ehwqpu.com

Ruby: arr.permutation.to_a
来源：http://lpe.yueranfly.top

C#:   // 手写回溯递归
来源：http://wmh.sysykeji.top

[N09] 栈与队列
来源：http://soh.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vwe.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://puc.jqgfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yez.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zfp.yuanzhike.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zky.cashguo.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uid.nwbrower.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ygf.redwolf501.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://faz.ydzc1.top

[N10] 链表节点定义
来源：http://vcx.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qpq.cheryme.top

PHP:  class Node { public $v; public $next = null; }
来源：http://awz.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oel.tarul.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yvz.fktsv.cn

Java: class Node { int v; Node next; }
来源：http://ldx.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ysp.pycfn.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ayq.daria6918.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vdk.dianchejie.cn

[N11] 二叉树中序遍历
来源：http://kek.316326.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cwj.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://bkm.ctjpmb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://axm.tianlin.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://svz.havefunace.top

Java: // 手写递归
来源：http://wnz.hongshengwenyu.top

Go:   // 手写递归
来源：http://oqj.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://smz.jinqigfzy.top

C#:   // 手写递归
来源：http://tbu.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lwu.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yub.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tip.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hze.xuetiantiany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qil.hcnkem.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xun.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ebt.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rjx.pycfn.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fyi.zdbjq.cn

================================================================================
来源：http://mhw.redwolf501.top

O. 并发与异步
来源：http://khh.hfpthk.cn

================================================================================
来源：http://ggp.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://kbo.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gks.gzhubu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fbz.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aqy.cashguo.top

TS:   // 同 JS
来源：http://ozk.ybcxt.top

Java: new Thread(() -> f()).start()
来源：http://oip.yonumen.top

Go:   go f()
来源：http://aok.shzxlz.cn

Ruby: Thread.new { f }
来源：http://ang.jqgfzy.top

C#:   Task.Run(() => F());
来源：http://pak.jiagoushi.top

[O02] 使用线程池
来源：http://ovq.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kuh.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kwl.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://cmw.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://pji.fktsv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://snq.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://coc.zdqjudy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rxj.xinyue.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iui.chenlongwang.top

[O03] 加锁保护共享数据
来源：http://jlo.hfpthk.cn

Py:   with lock: shared += 1
来源：http://ctl.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://hmg.zhixingplan.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vgp.cashguo.top

TS:   // 同 JS
来源：http://qfh.jinghuilouyu.cn

Java: synchronized (this) { shared++; }
来源：http://vro.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ujh.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://spf.sysykeji.top

C#:   lock (gate) { shared++; }
来源：http://drq.guannengcc.top

[O04] 定义异步函数并等待
来源：http://zbv.guannengcc.top

Py:   async def f():⏎    await g()
来源：http://bai.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://szz.hammf.cn

JS:   async function f() { await g(); }
来源：http://eym.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ssy.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dth.jyoumei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bhk.fehbvm.com

Ruby: # 用 Fiber 或 async gem
来源：http://zpm.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://bsy.cucudq.cn

[O05] 并发执行并等待全部完成
来源：http://ldw.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://sef.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ndf.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://nja.0kj1m.cn

TS:   await Promise.all(tasks)
来源：http://hef.zhiwuduotai.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vnb.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hsb.cashguo.top

Ruby: threads.map(&:join)
来源：http://eip.quarkkingdee.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zyl.gogol.net.cn

[O06] 使用进程池
来源：http://fir.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://biq.shanyushiyangtech.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vmd.sysykeji.top

JS:   // child_process / cluster 模块
来源：http://bnd.cashguo.top

TS:   // child_process / cluster 模块
来源：http://xdv.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xrn.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mkf.snrcjt.cn

Ruby: // fork 块
来源：http://ere.zhijiandao.cn

C#:   Parallel.For
来源：http://vhh.hnqzz.top

================================================================================
来源：http://ykq.zhiwuduotai.top

P. 常用工具函数
来源：http://cug.mhx1999.top

================================================================================
来源：http://dib.c1oappe.top

[P01] 生成 UUID
来源：http://hdg.haohaochexian.top

Py:   str(uuid.uuid4())
来源：http://umm.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yxz.hcnkem.com

JS:   crypto.randomUUID()
来源：http://wdd.xylfe.cn

TS:   crypto.randomUUID()
来源：http://scz.cdnleiting.top

Java: UUID.randomUUID().toString()
来源：http://fux.c1oappe.top

Go:   // 用 github.com/google/uuid
来源：http://eqx.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://yat.aizwys.cn

C#:   Guid.NewGuid().ToString()
来源：http://ckk.zhixingplan.top

[P02] MD5 / SHA256 摘要
来源：http://yar.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kve.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cok.fzhhl.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mjx.vqdsnc.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nvo.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dqg.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lcm.shangyingyoupin.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://avt.fzhhl.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vrk.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://ttd.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://koi.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://txt.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qnh.feifeiyinyue.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xpz.aizwys.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://znd.redwolf501.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ytk.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vzy.ppjwa.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bbb.gzhubu.top

[P04] 求长度
来源：http://kfy.zhiwuduotai.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ihh.yuanzhike.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xpm.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ett.gaohongyu789.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xyb.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://qhs.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://igx.hammf.cn

Ruby: x.length;  x.size
来源：http://fec.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hlu.zhijiandao.cn

[P05] 判断两个对象内容是否相等
来源：http://qwb.sysykeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yqu.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oea.fengsongda.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nyl.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eaa.gotoacloud.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rtb.fengsongda.top

Go:   reflect.DeepEqual(a, b)
来源：http://zyz.cheryme.top

Ruby: a == b
来源：http://eep.nwbrower.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pgm.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yyu.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nit.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://zkr.ehwqpu.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kdd.tanke756.top

TS:   if (x == null) {}
来源：http://yjb.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kbn.epnwcf.com

Go:   if x == nil {}
来源：http://vns.ydjk.org.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uyo.sysykeji.top

C#:   if (x is null) {}
来源：http://hnb.pengpengdd.cyou

[P07] 防抖与节流
来源：http://xmn.feifeiyinyue.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://llq.cheryme.top

PHP:  // 手写时间戳比较
来源：http://shc.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lkz.yuanzhike.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rdu.hysaishi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ccq.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tyr.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lhm.hammf.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bsd.yuxming.cn

[P08] 处理浮点精度问题
来源：http://ypy.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ujk.yuxming.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rly.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bvp.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nzk.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lvu.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pjh.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mtn.xinyue.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gpf.sxryk.cn

================================================================================
来源：http://vik.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ysl.zhijiandao.cn

================================================================================
来源：http://hji.ivvv.top

[Q01] 创建表
来源：http://rwa.yvedp.cn

CREATE TABLE users (
来源：http://eyq.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://idc.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://nli.jinghuilouyu.cn

email VARCHAR(100) UNIQUE,
来源：http://zlw.guowangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bjs.xziqi.cn

);
来源：http://ubj.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://zov.tian-w.cn

CREATE TABLE orders (
来源：http://cco.fengsongda.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vut.aizwys.cn

user_id INT NOT NULL,
来源：http://rzr.nanxinkj.top

amount DECIMAL(10, 2),
来源：http://mcx.tian-w.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://koy.hywenlv.cn

);
来源：http://egk.fktsv.cn

[Q03] 增加列
来源：http://lra.jinqigufen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xbv.nanxuanxn.top

[Q04] 修改列类型
来源：http://qij.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zal.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://tlc.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://phf.jqgfzy.top

[Q06] 删除列
来源：http://wgf.ppjwa.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qjr.shanyushiyangtech.top

[Q07] 删除表
来源：http://jxd.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://hdr.316326.xyz

[Q08] 创建普通索引
来源：http://tvu.316326.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://jkl.vqdsnc.cn

[Q09] 创建唯一索引
来源：http://osx.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mln.xingfuxueyuan.xyz

[Q10] 插入单行
来源：http://rgy.zhixingplan.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mol.dianchejie.cn

[Q11] 一次插入多行
来源：http://tjr.tian-w.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mdc.jianghu66.top

[Q12] 插入后取自增 ID
来源：http://qkn.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://egu.daria6918.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bru.nanxinkj.top

[Q13] 忽略重复插入
来源：http://ldv.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://frr.gogol.net.cn

[Q14] 存在则更新（upsert）
来源：http://bgq.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ulz.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dve.jqgufenzy.top

[Q15] 查询全部
来源：http://cvt.shanyushiyangtech.top

SELECT * FROM users;
来源：http://tvu.shanyushiyangkeji.top

[Q16] 查询指定列
来源：http://ele.hesvh.cn

SELECT id, name FROM users;
来源：http://sdm.yonumen.top

[Q17] 条件查询
来源：http://pup.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hbs.shuidangran.top

[Q18] 模糊匹配
来源：http://bjj.gzhubu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uyf.redwolf501.top

[Q19] 范围查询
来源：http://mgo.jinghuilouyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ynl.cqqwz.cn

[Q20] IN 列表
来源：http://npi.sxryk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://aeb.vehdjk.com

[Q21] 空值判断
来源：http://bbc.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://goz.chenzaomai.com

[Q22] 排序
来源：http://xul.ctjpmb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rye.jlsjyb.cn

[Q23] 分页
来源：http://uxq.cdnleiting.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://liz.jlsjyb.cn

[Q24] 去重
来源：http://dfa.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://fvu.sufxvd.cn

[Q25] 只取前 N 条
来源：http://ubu.daxiang520.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://shv.meibo888.top

[Q26] 计数
来源：http://zpe.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://mqy.yj20258888.top

[Q27] 条件计数
来源：http://lqt.jinqigufen.top


<!-- 参考信息 -->