代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://pqr.wangdashe.top

================================================================================
来源：http://tfu.dianchejie.cn

N. 数据结构与算法
来源：http://qyz.wangshuangyany.cn

================================================================================
来源：http://eua.birdmap.top

[N01] 二分查找（有序数组）
来源：http://cvi.zhixingplan.top

Py:   bisect.bisect_left(arr, x)
来源：http://lhm.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tmn.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fum.shangyingyoupin.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qpo.yanxiufei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qsb.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://uxn.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mon.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://frx.hywenlv.cn

[N02] 排序（工程实践用内置实现）
来源：http://sml.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://oez.sjlbkw.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zan.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vho.pycfn.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://qvn.havefunace.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vfy.cheryme.top

Go:   slices.Sort(arr)
来源：http://swj.daxiang520.top

Ruby: arr.sort
来源：http://jgg.xinyue.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://llg.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://wmv.c1oappe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qxy.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://eru.yuanzhike.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://niv.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ekc.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ddo.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oaf.sufxvd.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lsp.epnwcf.com

C#:   // 手写递归，或 Array.Sort
来源：http://dhv.cqqwz.cn

[N04] 斐波那契数列
来源：http://gff.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xaa.nanxuanxn.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://abj.jyoumei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://skl.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cog.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kpx.andypj.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://epf.pengpengdd.cyou

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://czy.iojbl.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://grf.xuanzx.com

[N05] 最大公约数
来源：http://rgh.fengsongda.top

Py:   math.gcd(a, b)
来源：http://ejl.yanxiufei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fqn.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vil.jinyuanbaomall.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sgz.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ytm.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rtr.ybcxt.top

Ruby: a.gcd(b)
来源：http://kps.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fgl.zdqjudy.top

[N06] 判断回文字符串
来源：http://nbm.nwbrower.top

Py:   s == s[::-1]
来源：http://dkb.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://rsl.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://ppy.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://kdq.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qck.dianchejie.cn

Go:   // 双指针从两端比较
来源：http://cyy.yuanzhike.top

Ruby: s == s.reverse
来源：http://gcf.andypj.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://zgf.birdmap.top

[N07] 两数之和（返回下标）
来源：http://thn.shangyingyoupin.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tqw.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vbk.yj20258.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nqg.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://wmi.316326.xyz

Java: // 手写 HashMap
来源：http://hts.fzhhl.top

Go:   // 手写 map[int]int
来源：http://czg.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://srs.ivvv.top

C#:   // 手写 Dictionary<int, int>
来源：http://vzr.birdmap.top

[N08] 生成全排列
来源：http://zwo.sjlbkw.cn

Py:   itertools.permutations(arr)
来源：http://rkh.epnwcf.com

PHP:  // 手写递归交换
来源：http://cum.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://qac.fktsv.cn

TS:   // 手写回溯递归
来源：http://wqj.shuidangran.top

Java: // 手写回溯递归
来源：http://uzl.jyoumei.cn

Go:   // 手写回溯递归
来源：http://ypn.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://ans.yj20258.top

C#:   // 手写回溯递归
来源：http://xyg.shanyushiyangtech.top

[N09] 栈与队列
来源：http://jad.smart0.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://udk.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tgu.iojbl.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://thv.ydzc1.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wed.gotoacloud.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qga.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mrz.aibaodan.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xft.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fca.sysykeji.top

[N10] 链表节点定义
来源：http://yag.cashguo.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sga.jinqigfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dac.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bca.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iwb.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://qth.cqqwz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cpp.xuetiantiany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oio.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yyy.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://raz.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ctx.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://nbz.jinyuanbaomall.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kca.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tcj.fzhhl.top

Java: // 手写递归
来源：http://njr.svipenyu.cn

Go:   // 手写递归
来源：http://hvi.jqgufenzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zdr.dianchejie.cn

C#:   // 手写递归
来源：http://wgk.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hnz.jinqigufen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dxu.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zvo.mhx1999.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qpw.cashguo.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://agh.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://beb.zycfv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hqt.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kwr.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ajc.feifeiyinyue.top

================================================================================
来源：http://gvx.yvedp.cn

O. 并发与异步
来源：http://qsf.jlsjyb.cn

================================================================================
来源：http://rcg.yuanzhike.top

[O01] 启动一个线程
来源：http://ile.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://urg.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fbm.andypj.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dpp.hongshengwenyu.top

TS:   // 同 JS
来源：http://krk.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://bxf.quarkkingdee.top

Go:   go f()
来源：http://uqd.haohaochexian.top

Ruby: Thread.new { f }
来源：http://uaj.zhaomingkeji.xyz

C#:   Task.Run(() => F());
来源：http://ctp.shzxlz.cn

[O02] 使用线程池
来源：http://eyo.hfpthk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://elj.tarul.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yzx.zhaomingkeji.xyz

JS:   // worker_threads 线程池
来源：http://azj.daxiang520.top

TS:   // worker_threads 线程池
来源：http://hcl.fengsongda.top

Java: Executors.newFixedThreadPool(4)
来源：http://rxy.nwbrower.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://klv.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ycx.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oiz.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://kwu.zhongyouzk.top

Py:   with lock: shared += 1
来源：http://arv.uphjek.com

PHP:  // 用 flock() 做文件锁
来源：http://gyo.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jxb.daxiang520.top

TS:   // 同 JS
来源：http://mwb.andypj.xyz

Java: synchronized (this) { shared++; }
来源：http://qth.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mav.aizwys.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://llj.sysykeji.top

C#:   lock (gate) { shared++; }
来源：http://ztb.jinyuanbaomall.cn

[O04] 定义异步函数并等待
来源：http://edz.shzxlz.cn

Py:   async def f():⏎    await g()
来源：http://leo.52xcode.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fze.yongpay.top

JS:   async function f() { await g(); }
来源：http://gau.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hug.yanxiufei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rrw.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ezp.zhengqikj.top

Ruby: # 用 Fiber 或 async gem
来源：http://xtr.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://cyt.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://awe.zhijiandao.cn

Py:   asyncio.gather(*tasks)
来源：http://chn.zdqjudy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mgl.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://yaw.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://xse.havefunace.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bpf.gogol.net.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dox.yanxiufei.cn

Ruby: threads.map(&:join)
来源：http://kgm.aibaodan.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cjp.gotoacloud.top

[O06] 使用进程池
来源：http://eti.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fom.nwbrower.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qwu.zdbjq.cn

JS:   // child_process / cluster 模块
来源：http://bxa.quarkkingdee.top

TS:   // child_process / cluster 模块
来源：http://pju.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ksi.zhoulong.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pfl.hysaishi.cn

Ruby: // fork 块
来源：http://xgx.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://edg.daxiang520.top

================================================================================
来源：http://yqu.pengpengdd.cyou

P. 常用工具函数
来源：http://rwt.jinghuilouyu.cn

================================================================================
来源：http://hdy.hysaishi.cn

[P01] 生成 UUID
来源：http://flv.ctjpmb.com

Py:   str(uuid.uuid4())
来源：http://mkb.ppjwa.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jkx.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://otp.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://qvb.iojbl.cn

Java: UUID.randomUUID().toString()
来源：http://mjh.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://lsd.jinqigufen.top

Ruby: SecureRandom.uuid
来源：http://fjt.yueranfly.top

C#:   Guid.NewGuid().ToString()
来源：http://nvx.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://cdx.wangdashe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fxw.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://aqy.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://npu.fanxiaobao.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zcl.kuanghao11.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dka.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dhr.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ttt.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rvd.yonumen.top

[P03] 生成短随机字符串
来源：http://fvk.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dsf.jqgufenzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jws.gotoacloud.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rnz.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yym.pycfn.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rqw.nanxuanxn.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wuk.hongshengwenyu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://elo.sufxvd.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eal.ydjk.org.cn

[P04] 求长度
来源：http://car.dianchejie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dgh.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ugz.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ysq.zhoulong.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qhv.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://qll.iojbl.cn

Go:   len(arr);  len(m)
来源：http://igd.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://kju.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bip.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://pgd.yongpay.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lgr.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://opi.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kft.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://abc.uphjek.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vrz.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wii.zhoulong.xyz

Ruby: a == b
来源：http://ngh.jiagoushi.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://byy.yongpay.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rty.shangyingyoupin.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mpp.zhongyouzk.top

PHP:  if (empty($x)) {}
来源：http://wmw.jinqigfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zfc.zhongyouzk.top

TS:   if (x == null) {}
来源：http://tgk.cucudq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zwp.zycfv.cn

Go:   if x == nil {}
来源：http://aby.bjfxy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://prx.yj202588.top

C#:   if (x is null) {}
来源：http://nha.ydjk.org.cn

[P07] 防抖与节流
来源：http://vrr.yfazqb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aby.316326.xyz

PHP:  // 手写时间戳比较
来源：http://rqt.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mjp.fanxiaobao.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gud.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bpr.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cru.zycfv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ctg.wangdashe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jql.sysykeji.top

[P08] 处理浮点精度问题
来源：http://ouy.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jtc.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gtu.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ihm.yongpay.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gjw.uphjek.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tay.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://crj.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pge.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ppz.fktsv.cn

================================================================================
来源：http://mwv.yvedp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kxn.yvedp.cn

================================================================================
来源：http://jbx.hnxiangtu.top

[Q01] 创建表
来源：http://ubk.dashuyun.cn

CREATE TABLE users (
来源：http://ojh.fktsv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wfe.cucudq.cn

name VARCHAR(50) NOT NULL,
来源：http://bnd.zdqjudy.top

email VARCHAR(100) UNIQUE,
来源：http://vbc.uphjek.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ssw.c1oappe.top

);
来源：http://hey.pycfn.com

[Q02] 创建带外键的表
来源：http://qey.yanxiufei.cn

CREATE TABLE orders (
来源：http://hvh.redwolf501.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cgg.cqqwz.cn

user_id INT NOT NULL,
来源：http://xag.jinyuanbaomall.cn

amount DECIMAL(10, 2),
来源：http://ref.jyoumei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qbq.ivvv.top

);
来源：http://ijx.svipenyu.cn

[Q03] 增加列
来源：http://lpp.gaohongyu789.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://diq.xylfe.cn

[Q04] 修改列类型
来源：http://obx.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dsc.chenzaomai.com

[Q05] 重命名列
来源：http://dny.chenjidiqi.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bod.zhongyouzk.top

[Q06] 删除列
来源：http://tjv.redwolf501.top

ALTER TABLE users DROP COLUMN age;
来源：http://jqg.shanyushiyangtech.top

[Q07] 删除表
来源：http://jve.nanxuanxn.top

DROP TABLE IF EXISTS orders;
来源：http://vqe.9152youxi.cn

[Q08] 创建普通索引
来源：http://pzs.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lso.hnqzz.top

[Q09] 创建唯一索引
来源：http://woe.daxiang520.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bzy.wangshuangyany.cn

[Q10] 插入单行
来源：http://jix.ivvv.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tot.wangdashe.top

[Q11] 一次插入多行
来源：http://jau.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eqs.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://cbo.hnqzz.top

INSERT INTO users (name) VALUES ('C');
来源：http://bgl.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://efe.hesvh.cn

[Q13] 忽略重复插入
来源：http://uxf.jlsjyb.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ugl.sweek.top

[Q14] 存在则更新（upsert）
来源：http://dow.hcnkem.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bbb.guannengcc.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pub.0kj1m.cn

[Q15] 查询全部
来源：http://uny.andypj.xyz

SELECT * FROM users;
来源：http://rtj.xuetiantiany.cn

[Q16] 查询指定列
来源：http://khs.52xcode.cn

SELECT id, name FROM users;
来源：http://flr.andypj.xyz

[Q17] 条件查询
来源：http://qyl.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ton.hywenlv.cn

[Q18] 模糊匹配
来源：http://xbq.cashguo.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dnl.jinghuilouyu.cn

[Q19] 范围查询
来源：http://pgl.guowangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gfi.hnxiangtu.top

[Q20] IN 列表
来源：http://jse.daxiang520.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kqd.c1oappe.top

[Q21] 空值判断
来源：http://ylq.ydzc1.top


<!-- 参考信息 -->