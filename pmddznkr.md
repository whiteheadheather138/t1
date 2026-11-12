代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://rzw.ywan-chungtsiang.top

================================================================================
来源：http://ugf.zhoulong.xyz

N. 数据结构与算法
来源：http://owk.xylfe.cn

================================================================================
来源：http://gvi.sjlbkw.cn

[N01] 二分查找（有序数组）
来源：http://azv.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://adl.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://alb.dashuyun.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wyg.jqgfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://use.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://dad.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://rge.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hwp.yj202588.top

C#:   Array.BinarySearch(arr, x)
来源：http://zlp.gotoacloud.top

[N02] 排序（工程实践用内置实现）
来源：http://wsq.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://aci.xinyue.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://geo.dashuyun.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jlx.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vrf.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://edz.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://jfw.mhx1999.top

Ruby: arr.sort
来源：http://wok.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xya.yj20258.top

[N03] 快速排序（分治示例）
来源：http://gwl.jianghu66.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mox.9152youxi.cn

PHP:  // 递归实现，或用 usort
来源：http://jel.cdnleiting.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tyy.zhixingplan.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://euz.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hgh.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ekg.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tmk.ppjwa.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hog.sxryk.cn

[N04] 斐波那契数列
来源：http://don.gzhubu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oic.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nsw.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vss.316326.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iud.aibaodan.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dyr.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ftm.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uta.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mjj.vehdjk.com

[N05] 最大公约数
来源：http://ygj.xylfe.cn

Py:   math.gcd(a, b)
来源：http://cpx.yvedp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zhl.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dbb.hnqzz.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sbd.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gya.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pgh.shuidangran.top

Ruby: a.gcd(b)
来源：http://won.hammf.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xus.yj202588.top

[N06] 判断回文字符串
来源：http://hgy.fehbvm.com

Py:   s == s[::-1]
来源：http://umt.jlsjyb.cn

PHP:  $s === strrev($s);
来源：http://gpa.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://usu.feifeiyinyue.top

TS:   s === [...s].reverse().join("")
来源：http://xog.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mck.9152youxi.cn

Go:   // 双指针从两端比较
来源：http://toc.52xcode.cn

Ruby: s == s.reverse
来源：http://xxh.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dbb.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://smf.haohaochexian.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lpb.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pgr.nanxinkj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wah.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://vwq.uphjek.com

Java: // 手写 HashMap
来源：http://zaq.zhiwuduotai.top

Go:   // 手写 map[int]int
来源：http://upo.yfazqb.com

Ruby: // 手写 Hash
来源：http://pji.bjfxy.top

C#:   // 手写 Dictionary<int, int>
来源：http://frj.bbcook.cn

[N08] 生成全排列
来源：http://kwt.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://tnx.iojbl.cn

PHP:  // 手写递归交换
来源：http://voo.cdnleiting.top

JS:   // 手写回溯递归
来源：http://rfk.gaohongyu789.top

TS:   // 手写回溯递归
来源：http://odh.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://maa.zhengqikj.top

Go:   // 手写回溯递归
来源：http://ldy.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://ixq.nwbrower.top

C#:   // 手写回溯递归
来源：http://tbk.jinghuilouyu.cn

[N09] 栈与队列
来源：http://ucp.hesvh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://prj.ppjwa.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pcq.chenzaomai.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bhc.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jha.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://itj.shanyushiyangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xlu.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://syi.tanke756.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://puy.sjlbkw.cn

[N10] 链表节点定义
来源：http://oys.sweek.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cpm.daxiang520.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vsq.shuidangran.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fgu.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jss.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://yat.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://mku.fengsongda.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ddr.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://cwg.gzhubu.top

[N11] 二叉树中序遍历
来源：http://wim.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xnn.sxryk.cn

PHP:  // 手写递归函数
来源：http://mie.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vyx.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://emk.xinyue.icu

Java: // 手写递归
来源：http://gse.yvedp.cn

Go:   // 手写递归
来源：http://rvf.316326.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ben.sweek.top

C#:   // 手写递归
来源：http://wkt.dashuyun.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ioy.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uhf.tarul.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ewd.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jta.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jho.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://alx.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ghm.andypj.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://llq.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://edo.cashguo.top

================================================================================
来源：http://vbr.tanke756.top

O. 并发与异步
来源：http://fpw.jinqigfzy.top

================================================================================
来源：http://nyv.hesvh.cn

[O01] 启动一个线程
来源：http://xbi.yuanzhike.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://omx.yonumen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aqm.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nnm.ydjk.org.cn

TS:   // 同 JS
来源：http://ujo.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://nha.ivvv.top

Go:   go f()
来源：http://imw.tian-w.cn

Ruby: Thread.new { f }
来源：http://esg.ppjwa.cn

C#:   Task.Run(() => F());
来源：http://rgu.cqqwz.cn

[O02] 使用线程池
来源：http://ihd.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ryr.gzhubu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fqx.jinqigufen.top

JS:   // worker_threads 线程池
来源：http://zhs.meibo888.top

TS:   // worker_threads 线程池
来源：http://fpl.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kak.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ocj.pycfn.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zyb.vqdsnc.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fqf.gaohongyu789.top

[O03] 加锁保护共享数据
来源：http://uwm.dashuyun.cn

Py:   with lock: shared += 1
来源：http://tfb.zdqjudy.top

PHP:  // 用 flock() 做文件锁
来源：http://qym.svipenyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eps.jyoumei.cn

TS:   // 同 JS
来源：http://ybq.fzhhl.top

Java: synchronized (this) { shared++; }
来源：http://xhq.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://alt.ydzc1.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ryr.nwbrower.top

C#:   lock (gate) { shared++; }
来源：http://bjy.hammf.cn

[O04] 定义异步函数并等待
来源：http://wfv.quarkkingdee.top

Py:   async def f():⏎    await g()
来源：http://iqs.zhixingplan.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lzw.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://irx.chenjidiqi.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://txw.ehwqpu.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fyl.shuidangran.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://biy.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://ifs.meibo888.top

C#:   async Task F() { await G(); }
来源：http://yev.0kj1m.cn

[O05] 并发执行并等待全部完成
来源：http://stz.316326.xyz

Py:   asyncio.gather(*tasks)
来源：http://ntf.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fmt.hywenlv.cn

JS:   await Promise.all(tasks)
来源：http://mjz.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://wwx.jqgufenzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dtn.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iau.ctjpmb.com

Ruby: threads.map(&:join)
来源：http://qjr.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://adm.fzhhl.top

[O06] 使用进程池
来源：http://hkq.meibo888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pjc.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bob.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://pdo.cucudq.cn

TS:   // child_process / cluster 模块
来源：http://ius.yueranfly.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oyb.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cys.jinqigfzy.top

Ruby: // fork 块
来源：http://geo.snrcjt.cn

C#:   Parallel.For
来源：http://ecr.cashguo.top

================================================================================
来源：http://ndd.zycfv.cn

P. 常用工具函数
来源：http://kne.jinqigufen.top

================================================================================
来源：http://ule.cheryme.top

[P01] 生成 UUID
来源：http://thw.c1oappe.top

Py:   str(uuid.uuid4())
来源：http://hqu.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lqr.ivvv.top

JS:   crypto.randomUUID()
来源：http://ezz.ivvv.top

TS:   crypto.randomUUID()
来源：http://mzb.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://muj.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://nqq.ybcxt.top

Ruby: SecureRandom.uuid
来源：http://znj.ybcxt.top

C#:   Guid.NewGuid().ToString()
来源：http://fet.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://mdp.gogol.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kwy.zhiwuduotai.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://agx.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://que.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sco.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jnp.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cuo.chenzaomai.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://aio.daria6918.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jlz.quarkkingdee.top

[P03] 生成短随机字符串
来源：http://cvx.wangdashe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jbb.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ekb.ywan-chungtsiang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://drz.chenjidiqi.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kgo.fanxiaobao.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://twd.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://coj.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://gfa.birdmap.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yjx.feifeiyinyue.top

[P04] 求长度
来源：http://uno.ivvv.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://exe.ctjpmb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yfq.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://avw.hfpthk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wko.hfpthk.cn

Java: list.size();  map.size();  s.length()
来源：http://xva.epnwcf.com

Go:   len(arr);  len(m)
来源：http://zrm.tianlin.xyz

Ruby: x.length;  x.size
来源：http://ouq.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tjo.ivvv.top

[P05] 判断两个对象内容是否相等
来源：http://oek.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dun.ydjk.org.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://juk.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zeq.kuanghao11.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lnw.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://epv.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qcq.gzhubu.top

Ruby: a == b
来源：http://ocf.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kqy.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hsi.vqdsnc.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://atc.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://euu.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bwy.ydzc1.top

TS:   if (x == null) {}
来源：http://nlu.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fey.ehwqpu.com

Go:   if x == nil {}
来源：http://atq.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pwo.shanyushiyangtech.top

C#:   if (x is null) {}
来源：http://hzh.sufxvd.cn

[P07] 防抖与节流
来源：http://vbi.cdnleiting.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://loq.sufxvd.cn

PHP:  // 手写时间戳比较
来源：http://how.yj202588.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sxt.kuanghao11.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pap.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://egj.gotoacloud.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ixi.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://uzj.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mpj.xylfe.cn

[P08] 处理浮点精度问题
来源：http://awe.gogol.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pvj.jinqigufen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://axh.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vss.cashguo.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fkn.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hbq.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rrz.hfpthk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tpv.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tiq.xingfuxueyuan.xyz

================================================================================
来源：http://zlu.shanyushiyangtech.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ijp.xingfuxueyuan.xyz

================================================================================
来源：http://qav.daxiang520.top

[Q01] 创建表
来源：http://uft.sufxvd.cn

CREATE TABLE users (
来源：http://jtb.yuxming.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qax.zdbjq.cn

name VARCHAR(50) NOT NULL,
来源：http://zen.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://eoy.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gom.ywan-chungtsiang.top

);
来源：http://fmy.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://ezq.cqqwz.cn

CREATE TABLE orders (
来源：http://qif.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xzn.aibaodan.cn

user_id INT NOT NULL,
来源：http://uxv.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://kny.ppjwa.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rqm.haohaochexian.top

);
来源：http://bpj.jlsjyb.cn

[Q03] 增加列
来源：http://hku.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lil.ydjk.org.cn

[Q04] 修改列类型
来源：http://hjq.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eno.0kj1m.cn

[Q05] 重命名列
来源：http://iwb.chenjidiqi.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zze.tarul.cn

[Q06] 删除列
来源：http://noe.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://kvf.hnqzz.top

[Q07] 删除表
来源：http://itf.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://ego.gotoacloud.top

[Q08] 创建普通索引
来源：http://pbq.aizwys.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vuz.zhengqikj.top

[Q09] 创建唯一索引
来源：http://pxy.zhoulong.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bcz.ehwqpu.com

[Q10] 插入单行
来源：http://biy.svipenyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xoq.ydzc1.top

[Q11] 一次插入多行
来源：http://azb.fzhhl.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dul.316326.xyz

[Q12] 插入后取自增 ID
来源：http://owi.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://djq.haohaochexian.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nll.pycfn.com

[Q13] 忽略重复插入
来源：http://uqe.chenzaomai.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://exj.zdqjudy.top

[Q14] 存在则更新（upsert）
来源：http://esr.zycfv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oqh.chenzaomai.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xkj.jinghuilouyu.cn

[Q15] 查询全部
来源：http://dbx.kuanghao11.cn

SELECT * FROM users;
来源：http://bpw.birdmap.top

[Q16] 查询指定列
来源：http://zda.fktsv.cn

SELECT id, name FROM users;
来源：http://rgr.yuanzhike.top

[Q17] 条件查询
来源：http://cew.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tcx.ehwqpu.com

[Q18] 模糊匹配
来源：http://jnz.wangdashe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hjt.zhengqikj.top

[Q19] 范围查询
来源：http://rud.cqqwz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pvt.fanxiaobao.xyz

[Q20] IN 列表
来源：http://wkf.zhijiandao.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rww.hammf.cn

[Q21] 空值判断
来源：http://pro.yuanzhike.top


<!-- 参考信息 -->