代发 wailian999

[N01] 二分查找（有序数组）
来源：http://wqm.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://zvm.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://our.zhongyouzk.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://knq.ybcxt.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://usr.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://cbp.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://cce.guannengcc.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://apm.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://fzk.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://gfo.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://tvl.cqqwz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sqs.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gnp.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://iyt.nwbrower.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ipk.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://mgo.ppjwa.cn

Ruby: arr.sort
来源：http://ppv.tarul.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xim.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://wbj.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gif.shanyushiyangtech.top

PHP:  // 递归实现，或用 usort
来源：http://ukz.hammf.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rph.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cde.yfazqb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://poq.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ath.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://asj.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://isy.jlsjyb.cn

[N04] 斐波那契数列
来源：http://nlu.chenjidiqi.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zgj.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qar.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mlf.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gmq.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hun.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bep.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ctk.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rwj.hcnkem.com

[N05] 最大公约数
来源：http://aol.ybcxt.top

Py:   math.gcd(a, b)
来源：http://tmc.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://akl.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wjw.zhoulong.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ass.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://enb.yj202588.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ayl.c1oappe.top

Ruby: a.gcd(b)
来源：http://vru.shanyushiyangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pcm.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://ojc.gogol.net.cn

Py:   s == s[::-1]
来源：http://vns.xuanzx.com

PHP:  $s === strrev($s);
来源：http://zfi.gzhubu.top

JS:   s === [...s].reverse().join("")
来源：http://jbk.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://bwy.aizwys.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pgv.chenlongwang.top

Go:   // 双指针从两端比较
来源：http://xrv.aizwys.cn

Ruby: s == s.reverse
来源：http://cyj.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://eik.yanxiufei.cn

[N07] 两数之和（返回下标）
来源：http://waa.ydjk.org.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://myv.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fzz.cdnleiting.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ntu.vehdjk.com

TS:   // 手写 Map<string, number>
来源：http://xor.jyoumei.cn

Java: // 手写 HashMap
来源：http://psk.cucudq.cn

Go:   // 手写 map[int]int
来源：http://vdz.redwolf501.top

Ruby: // 手写 Hash
来源：http://abj.xylfe.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yya.cucudq.cn

[N08] 生成全排列
来源：http://boa.xuetiantiany.cn

Py:   itertools.permutations(arr)
来源：http://saq.yuanzhike.top

PHP:  // 手写递归交换
来源：http://slm.aibaodan.cn

JS:   // 手写回溯递归
来源：http://wub.cdnleiting.top

TS:   // 手写回溯递归
来源：http://fsg.nwbrower.top

Java: // 手写回溯递归
来源：http://ayi.ydzc1.top

Go:   // 手写回溯递归
来源：http://kdg.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://tuv.dashuyun.cn

C#:   // 手写回溯递归
来源：http://ntj.snrcjt.cn

[N09] 栈与队列
来源：http://coh.0kj1m.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pne.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kml.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iyr.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://djw.meibo888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uxi.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mmu.jqgfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kak.yj202588.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dbg.fanxiaobao.xyz

[N10] 链表节点定义
来源：http://qnj.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ilu.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lbg.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hyz.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jbh.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://exh.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://hry.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://rkk.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qbo.snrcjt.cn

[N11] 二叉树中序遍历
来源：http://wwy.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dsh.hongshengwenyu.top

PHP:  // 手写递归函数
来源：http://iyd.cheryme.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dex.gogol.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ymo.sweek.top

Java: // 手写递归
来源：http://uqi.quarkkingdee.top

Go:   // 手写递归
来源：http://exa.andypj.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://umj.bjfxy.top

C#:   // 手写递归
来源：http://ikm.zdbjq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kbm.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hlt.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qfs.yongpay.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fex.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ggf.yongpay.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://khn.mhx1999.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ggu.shuidangran.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ewf.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gxv.shangyingyoupin.top

================================================================================
来源：http://vvw.yj20258.top

O. 并发与异步
来源：http://yxl.xinyue.icu

================================================================================
来源：http://xji.zhaomingkeji.xyz

[O01] 启动一个线程
来源：http://koq.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jri.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hcu.wangshuangyany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://prk.tarul.cn

TS:   // 同 JS
来源：http://ijj.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://ldu.wangdashe.top

Go:   go f()
来源：http://jii.chenlongwang.top

Ruby: Thread.new { f }
来源：http://ovh.feifeiyinyue.top

C#:   Task.Run(() => F());
来源：http://ilu.zhiwuduotai.top

[O02] 使用线程池
来源：http://sdd.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bly.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zxw.zhixingplan.top

JS:   // worker_threads 线程池
来源：http://qxk.fktsv.cn

TS:   // worker_threads 线程池
来源：http://yvm.svipenyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ugo.yongpay.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bfh.cucudq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jgm.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yov.uphjek.com

[O03] 加锁保护共享数据
来源：http://stz.hongshengwenyu.top

Py:   with lock: shared += 1
来源：http://oay.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://xrr.nanxinkj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xrx.zdbjq.cn

TS:   // 同 JS
来源：http://gaq.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://sdx.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xfw.tarul.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vht.jinqigfzy.top

C#:   lock (gate) { shared++; }
来源：http://zsz.ybcxt.top

[O04] 定义异步函数并等待
来源：http://noy.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://sfy.gzhubu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nyn.ehwqpu.com

JS:   async function f() { await g(); }
来源：http://etf.birdmap.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://erq.hongshengwenyu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dzr.xinyue.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dml.nanxinkj.top

Ruby: # 用 Fiber 或 async gem
来源：http://elt.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://zch.sufxvd.cn

[O05] 并发执行并等待全部完成
来源：http://pyd.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://gmy.yanxiufei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ucd.pengpengdd.cyou

JS:   await Promise.all(tasks)
来源：http://yhe.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://fkj.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cpm.jqgufenzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yoc.jqgfzy.top

Ruby: threads.map(&:join)
来源：http://igk.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xiw.wangshuangyany.cn

[O06] 使用进程池
来源：http://qki.quarkkingdee.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yxf.daxiang520.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nff.hammf.cn

JS:   // child_process / cluster 模块
来源：http://xzg.jinqigufen.top

TS:   // child_process / cluster 模块
来源：http://ufa.yj20258888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vja.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://faa.svipenyu.cn

Ruby: // fork 块
来源：http://fwv.aizwys.cn

C#:   Parallel.For
来源：http://oyv.yonumen.top

================================================================================
来源：http://xzl.hnxiangtu.top

P. 常用工具函数
来源：http://ocn.redwolf501.top

================================================================================
来源：http://kyb.ppjwa.cn

[P01] 生成 UUID
来源：http://ayf.jinqigufen.top

Py:   str(uuid.uuid4())
来源：http://zci.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qfk.hcnkem.com

JS:   crypto.randomUUID()
来源：http://qtn.daria6918.cn

TS:   crypto.randomUUID()
来源：http://tfl.quarkkingdee.top

Java: UUID.randomUUID().toString()
来源：http://nzc.yj20258.top

Go:   // 用 github.com/google/uuid
来源：http://vyd.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://pyq.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://bzo.meibo888.top

[P02] MD5 / SHA256 摘要
来源：http://lho.zhengqikj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jex.wangdashe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ikr.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://whd.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ojy.9152youxi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://grw.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eyb.316326.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ywu.zhiwuduotai.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://usn.epnwcf.com

[P03] 生成短随机字符串
来源：http://ktp.xinyue.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sog.fehbvm.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dcp.zycfv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jum.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fqr.zdbjq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gwr.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hqw.cucudq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gch.ppjwa.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hpq.daxiang520.top

[P04] 求长度
来源：http://lmg.ctjpmb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qqz.0kj1m.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rrv.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xxg.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vrb.zhongyouzk.top

Java: list.size();  map.size();  s.length()
来源：http://amo.ydzc1.top

Go:   len(arr);  len(m)
来源：http://lqa.yj202588.top

Ruby: x.length;  x.size
来源：http://wnv.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cvn.ybcxt.top

[P05] 判断两个对象内容是否相等
来源：http://mgf.hnxiangtu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jwz.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rbr.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vgr.mhx1999.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sjh.zhixingplan.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rnv.nanxinkj.top

Go:   reflect.DeepEqual(a, b)
来源：http://yft.316326.xyz

Ruby: a == b
来源：http://bxh.xziqi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vsu.shangyingyoupin.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nrr.yonumen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yyw.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://nga.shanyushiyangtech.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zxf.chenlongwang.top

TS:   if (x == null) {}
来源：http://cpm.hysaishi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mur.ivvv.top

Go:   if x == nil {}
来源：http://ioz.sweek.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://olo.yuanzhike.top

C#:   if (x is null) {}
来源：http://glr.redwolf501.top

[P07] 防抖与节流
来源：http://ivq.ppjwa.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iay.uphjek.com

PHP:  // 手写时间戳比较
来源：http://yai.jyoumei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pks.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ucg.snrcjt.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vlo.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://moz.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wja.dianchejie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nin.pycfn.com

[P08] 处理浮点精度问题
来源：http://xog.nanxuanxn.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hdj.yfazqb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cnp.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://scj.haohaochexian.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://izq.haohaochexian.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iha.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zga.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oxt.yueranfly.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ogf.ydzc1.top

================================================================================
来源：http://cqa.guannengcc.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ysd.dashuyun.cn

================================================================================
来源：http://hbf.hfpthk.cn

[Q01] 创建表
来源：http://wyo.yuanzhike.top

CREATE TABLE users (
来源：http://mvq.ywan-chungtsiang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ars.sysykeji.top

name VARCHAR(50) NOT NULL,
来源：http://rto.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://wey.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gvv.tian-w.cn

);
来源：http://ztg.yvedp.cn

[Q02] 创建带外键的表
来源：http://lom.tianlin.xyz

CREATE TABLE orders (
来源：http://typ.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cjw.gotoacloud.top

user_id INT NOT NULL,
来源：http://pab.ywan-chungtsiang.top

amount DECIMAL(10, 2),
来源：http://zln.wangdashe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jqo.gaohongyu789.top

);
来源：http://rwa.hnxiangtu.top

[Q03] 增加列
来源：http://zgo.cheryme.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ffl.epnwcf.com

[Q04] 修改列类型
来源：http://qya.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kzl.cqqwz.cn

[Q05] 重命名列
来源：http://apz.ivvv.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fbi.jinqigfzy.top

[Q06] 删除列
来源：http://gtm.shanyushiyangtech.top

ALTER TABLE users DROP COLUMN age;
来源：http://cgx.zycfv.cn

[Q07] 删除表
来源：http://uhb.hcnkem.com

DROP TABLE IF EXISTS orders;
来源：http://dhv.epnwcf.com

[Q08] 创建普通索引
来源：http://myx.nwbrower.top

CREATE INDEX idx_users_email ON users(email);
来源：http://osd.gzhubu.top

[Q09] 创建唯一索引
来源：http://igl.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fha.ehwqpu.com

[Q10] 插入单行
来源：http://iti.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ajs.shuidangran.top

[Q11] 一次插入多行
来源：http://dzf.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ymt.mhx1999.top

[Q12] 插入后取自增 ID
来源：http://qqk.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://icc.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://izo.shanyushiyangtech.top

[Q13] 忽略重复插入
来源：http://qol.yanxiufei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vwe.ppjwa.cn

[Q14] 存在则更新（upsert）
来源：http://zrj.aizwys.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ast.fzhhl.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jfr.mhx1999.top

[Q15] 查询全部
来源：http://nzk.jiagoushi.top

SELECT * FROM users;
来源：http://xen.aibaodan.cn

[Q16] 查询指定列
来源：http://eyf.aibaodan.cn

SELECT id, name FROM users;
来源：http://zrw.dianchejie.cn

[Q17] 条件查询
来源：http://ljj.bbcook.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kwv.shanyushiyangkeji.top

[Q18] 模糊匹配
来源：http://uvb.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hdd.dianchejie.cn

[Q19] 范围查询
来源：http://ivi.fzhhl.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oxj.kuanghao11.cn

[Q20] IN 列表
来源：http://zej.hfpthk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hzl.aizwys.cn

[Q21] 空值判断
来源：http://jiv.9152youxi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dpq.ppjwa.cn

[Q22] 排序
来源：http://jtk.chenlongwang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kng.ctjpmb.com

[Q23] 分页
来源：http://vrx.tian-w.cn


<!-- 参考信息 -->