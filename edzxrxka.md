代发 wailian999

[N01] 二分查找（有序数组）
来源：http://qsw.hfpthk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gbq.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://brd.c1oappe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eqf.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://anb.fzhhl.top

Java: Arrays.binarySearch(arr, x)
来源：http://pdf.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://eot.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mls.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qvf.gaohongyu789.top

[N02] 排序（工程实践用内置实现）
来源：http://agn.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://kkm.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fne.kuanghao11.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mgg.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xgh.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://unq.svipenyu.cn

Go:   slices.Sort(arr)
来源：http://rif.kuanghao11.cn

Ruby: arr.sort
来源：http://hph.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hpv.xinyue.icu

[N03] 快速排序（分治示例）
来源：http://zmk.gzhubu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qve.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://eht.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lzi.xylfe.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yfd.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ozv.andypj.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vep.wangdashe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gpb.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://phq.meibo888.top

[N04] 斐波那契数列
来源：http://pmj.jinghuilouyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hrc.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zxs.sufxvd.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dnu.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jat.yvedp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://for.sweek.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iix.fengsongda.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kvz.316326.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dtb.jinqigufen.top

[N05] 最大公约数
来源：http://kjo.jiagoushi.top

Py:   math.gcd(a, b)
来源：http://kzd.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lij.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ltr.hongshengwenyu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rnu.ydzc1.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qhx.quarkkingdee.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ncg.yuanzhike.top

Ruby: a.gcd(b)
来源：http://oow.zycfv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mfd.andypj.xyz

[N06] 判断回文字符串
来源：http://mbj.nwbrower.top

Py:   s == s[::-1]
来源：http://hpa.daxiang520.top

PHP:  $s === strrev($s);
来源：http://cgv.nanxinkj.top

JS:   s === [...s].reverse().join("")
来源：http://vpg.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://yxd.sufxvd.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zfx.pycfn.com

Go:   // 双指针从两端比较
来源：http://cne.zhiwuduotai.top

Ruby: s == s.reverse
来源：http://atn.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://uqf.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://utl.jqgufenzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://izv.shanyushiyangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rvm.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://his.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://vpc.yuanzhike.top

Java: // 手写 HashMap
来源：http://jgp.kuanghao11.cn

Go:   // 手写 map[int]int
来源：http://ubo.birdmap.top

Ruby: // 手写 Hash
来源：http://cfu.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://krw.yonumen.top

[N08] 生成全排列
来源：http://wrv.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://owt.yueranfly.top

PHP:  // 手写递归交换
来源：http://bom.chenlongwang.top

JS:   // 手写回溯递归
来源：http://oxv.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://tzq.hywenlv.cn

Java: // 手写回溯递归
来源：http://ezz.tarul.cn

Go:   // 手写回溯递归
来源：http://vfl.gotoacloud.top

Ruby: arr.permutation.to_a
来源：http://bim.zdqjudy.top

C#:   // 手写回溯递归
来源：http://rnp.aibaodan.cn

[N09] 栈与队列
来源：http://wrv.yangfankeji.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yma.birdmap.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kbm.jqgfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://plh.hongshengwenyu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yzr.jlsjyb.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wko.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ead.ywan-chungtsiang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pdg.pycfn.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gus.svipenyu.cn

[N10] 链表节点定义
来源：http://phi.shangyingyoupin.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://koj.zycfv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xhw.yvedp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sqa.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dok.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://tlv.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://qpy.yfazqb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://vmx.ppjwa.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://goc.tian-w.cn

[N11] 二叉树中序遍历
来源：http://uxj.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zog.zhongyouzk.top

PHP:  // 手写递归函数
来源：http://uly.cheryme.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://urq.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sof.yanxiufei.cn

Java: // 手写递归
来源：http://yuk.yueranfly.top

Go:   // 手写递归
来源：http://mvt.feifeiyinyue.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://utl.xuetiantiany.cn

C#:   // 手写递归
来源：http://gns.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hfy.nwbrower.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vit.ydjk.org.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vxl.daria6918.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pdj.sufxvd.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ndq.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lqs.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://urw.guannengcc.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fpp.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sgg.yj20258888.top

================================================================================
来源：http://kfe.fanxiaobao.xyz

O. 并发与异步
来源：http://snv.shangyingyoupin.top

================================================================================
来源：http://eih.jiagoushi.top

[O01] 启动一个线程
来源：http://ecz.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cmu.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ptg.hesvh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://stc.zdqjudy.top

TS:   // 同 JS
来源：http://vof.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://dwz.ydzc1.top

Go:   go f()
来源：http://mqe.shuidangran.top

Ruby: Thread.new { f }
来源：http://nju.zhijiandao.cn

C#:   Task.Run(() => F());
来源：http://gqy.shuidangran.top

[O02] 使用线程池
来源：http://czx.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lxf.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://frt.meibo888.top

JS:   // worker_threads 线程池
来源：http://lmr.xuanzx.com

TS:   // worker_threads 线程池
来源：http://mnz.yonumen.top

Java: Executors.newFixedThreadPool(4)
来源：http://wan.cqqwz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xek.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cjt.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vyy.jqgfzy.top

[O03] 加锁保护共享数据
来源：http://aio.shuidangran.top

Py:   with lock: shared += 1
来源：http://qwg.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://vlm.sxryk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xlp.zhengqikj.top

TS:   // 同 JS
来源：http://pjj.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://ump.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jwp.wangshuangyany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yqg.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://ylr.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://ikn.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://wmk.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wlh.zycfv.cn

JS:   async function f() { await g(); }
来源：http://xqt.gaohongyu789.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xdx.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nta.xuanzx.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qam.zdbjq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kvu.sufxvd.cn

C#:   async Task F() { await G(); }
来源：http://diz.vehdjk.com

[O05] 并发执行并等待全部完成
来源：http://yzl.jlsjyb.cn

Py:   asyncio.gather(*tasks)
来源：http://brx.hesvh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qoh.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://blc.meibo888.top

TS:   await Promise.all(tasks)
来源：http://gqj.ywan-chungtsiang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ygr.yangfankeji.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fur.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://rnm.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vki.fanxiaobao.xyz

[O06] 使用进程池
来源：http://vti.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://spc.jinghuilouyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wno.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://jvd.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://lgz.sufxvd.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://maf.yongpay.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pjn.9152youxi.cn

Ruby: // fork 块
来源：http://loe.birdmap.top

C#:   Parallel.For
来源：http://hgr.guannengcc.top

================================================================================
来源：http://ouy.sufxvd.cn

P. 常用工具函数
来源：http://nsd.ivvv.top

================================================================================
来源：http://qfn.havefunace.top

[P01] 生成 UUID
来源：http://dgr.dianchejie.cn

Py:   str(uuid.uuid4())
来源：http://qju.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qoi.zdqjudy.top

JS:   crypto.randomUUID()
来源：http://wkt.cqqwz.cn

TS:   crypto.randomUUID()
来源：http://hrj.cdnleiting.top

Java: UUID.randomUUID().toString()
来源：http://wfi.dianchejie.cn

Go:   // 用 github.com/google/uuid
来源：http://swv.jinghuilouyu.cn

Ruby: SecureRandom.uuid
来源：http://xpi.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://glc.yangfankeji.com

[P02] MD5 / SHA256 摘要
来源：http://uwo.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qlg.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://aqa.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yik.zdqjudy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://exv.wangshuangyany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://csu.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eox.sxryk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://exp.ctjpmb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kyu.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://jbo.hnqzz.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yae.xylfe.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tdp.smart0.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kji.chenzaomai.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gwe.andypj.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fhu.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ckn.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lzl.yfazqb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lrn.gzhubu.top

[P04] 求长度
来源：http://zcv.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pys.yuanzhike.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qzc.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iok.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mol.daxiang520.top

Java: list.size();  map.size();  s.length()
来源：http://zhe.xuanzx.com

Go:   len(arr);  len(m)
来源：http://olm.jinyuanbaomall.cn

Ruby: x.length;  x.size
来源：http://nud.316326.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://tbe.pycfn.com

[P05] 判断两个对象内容是否相等
来源：http://mlr.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://apv.xinyue.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jmr.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vlm.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jgg.jinyuanbaomall.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://quk.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xyn.jinyuanbaomall.cn

Ruby: a == b
来源：http://hlp.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://haw.svipenyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://erz.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vjf.hammf.cn

PHP:  if (empty($x)) {}
来源：http://stw.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ixa.cashguo.top

TS:   if (x == null) {}
来源：http://bjw.zhaomingkeji.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://syc.jianghu66.top

Go:   if x == nil {}
来源：http://kyx.fanxiaobao.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ide.yfazqb.com

C#:   if (x is null) {}
来源：http://kon.pycfn.com

[P07] 防抖与节流
来源：http://fex.dianchejie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qab.hongshengwenyu.top

PHP:  // 手写时间戳比较
来源：http://jom.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xgb.cashguo.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hcz.meibo888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fwv.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ozc.fehbvm.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://uhi.zycfv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qhq.jinqigfzy.top

[P08] 处理浮点精度问题
来源：http://jeo.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qsk.smart0.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yuq.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vtr.sweek.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qec.guannengcc.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oyk.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mwb.gzhubu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lxk.yanxiufei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mrz.shanyushiyangtech.top

================================================================================
来源：http://ysg.sysykeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hxj.jlsjyb.cn

================================================================================
来源：http://oix.chenjidiqi.icu

[Q01] 创建表
来源：http://hqp.chenlongwang.top

CREATE TABLE users (
来源：http://clt.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hvm.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://xqz.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://cri.jinyuanbaomall.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wbs.xylfe.cn

);
来源：http://vtg.hammf.cn

[Q02] 创建带外键的表
来源：http://kwh.guannengcc.top

CREATE TABLE orders (
来源：http://ktx.ydjk.org.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tda.jqgfzy.top

user_id INT NOT NULL,
来源：http://hyi.zycfv.cn

amount DECIMAL(10, 2),
来源：http://tjz.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ser.iojbl.cn

);
来源：http://umi.zycfv.cn

[Q03] 增加列
来源：http://nje.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nps.cdnleiting.top

[Q04] 修改列类型
来源：http://pbx.yj202588.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yye.xinyue.icu

[Q05] 重命名列
来源：http://eyy.jyoumei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vsm.zhixingplan.top

[Q06] 删除列
来源：http://hkj.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://twi.birdmap.top

[Q07] 删除表
来源：http://adb.xingfuxueyuan.xyz

DROP TABLE IF EXISTS orders;
来源：http://kmb.hongshengwenyu.top

[Q08] 创建普通索引
来源：http://pvc.jiagoushi.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fqg.daria6918.cn

[Q09] 创建唯一索引
来源：http://mtl.jinqigfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zey.ppjwa.cn

[Q10] 插入单行
来源：http://wun.guannengcc.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xqg.tanke756.top

[Q11] 一次插入多行
来源：http://zke.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://riy.zhengqikj.top

[Q12] 插入后取自增 ID
来源：http://qxi.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://dpr.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aos.ctjpmb.com

[Q13] 忽略重复插入
来源：http://cxv.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hcl.fanxiaobao.xyz

[Q14] 存在则更新（upsert）
来源：http://tqz.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vrf.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bjz.hammf.cn

[Q15] 查询全部
来源：http://dwz.jqgfzy.top

SELECT * FROM users;
来源：http://vim.fzhhl.top

[Q16] 查询指定列
来源：http://xgt.fehbvm.com

SELECT id, name FROM users;
来源：http://dls.hnqzz.top

[Q17] 条件查询
来源：http://geo.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gfs.c1oappe.top

[Q18] 模糊匹配
来源：http://fzq.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nis.zdbjq.cn

[Q19] 范围查询
来源：http://lif.bbcook.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ysz.0kj1m.cn

[Q20] IN 列表
来源：http://qey.yonumen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://miz.quarkkingdee.top

[Q21] 空值判断
来源：http://clv.gaohongyu789.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cxd.9152youxi.cn

[Q22] 排序
来源：http://byj.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xtv.jinqigfzy.top

[Q23] 分页
来源：http://gth.daria6918.cn


<!-- 参考信息 -->