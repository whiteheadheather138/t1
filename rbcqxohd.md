代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rpn.fengsongda.top

Java: Arrays.binarySearch(arr, x)
来源：http://bbs.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://lxg.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://imr.bbcook.cn

C#:   Array.BinarySearch(arr, x)
来源：http://efy.hywenlv.cn

[N02] 排序（工程实践用内置实现）
来源：http://swi.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://pod.zhaomingkeji.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pqb.yonumen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ybc.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zmf.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://txc.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://ama.dashuyun.cn

Ruby: arr.sort
来源：http://irp.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rvd.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://aeu.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dsz.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://xiv.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cye.shangyingyoupin.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vlz.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ebh.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ems.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vpd.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://izp.daxiang520.top

[N04] 斐波那契数列
来源：http://yjc.vqdsnc.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tfm.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nco.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oyf.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qwh.chenzaomai.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oqz.jyoumei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://duy.yj20258.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gfx.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fhc.cashguo.top

[N05] 最大公约数
来源：http://tga.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://geu.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://liz.fktsv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qft.hammf.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://glu.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vic.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uxc.nwbrower.top

Ruby: a.gcd(b)
来源：http://rzs.nanxinkj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mwi.yj202588.top

[N06] 判断回文字符串
来源：http://dup.cdnleiting.top

Py:   s == s[::-1]
来源：http://iho.andypj.xyz

PHP:  $s === strrev($s);
来源：http://vde.sweek.top

JS:   s === [...s].reverse().join("")
来源：http://bej.haohaochexian.top

TS:   s === [...s].reverse().join("")
来源：http://cvn.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lgl.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://wtt.xingfuxueyuan.xyz

Ruby: s == s.reverse
来源：http://eai.316326.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://uef.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://otn.cqqwz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ldd.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jlr.jiagoushi.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rey.birdmap.top

TS:   // 手写 Map<string, number>
来源：http://mpt.xziqi.cn

Java: // 手写 HashMap
来源：http://nkp.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://awz.cdnleiting.top

Ruby: // 手写 Hash
来源：http://mmp.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://wpe.shanyushiyangtech.top

[N08] 生成全排列
来源：http://gik.316326.xyz

Py:   itertools.permutations(arr)
来源：http://yoa.yanxiufei.cn

PHP:  // 手写递归交换
来源：http://hfy.ydjk.org.cn

JS:   // 手写回溯递归
来源：http://tuu.ivvv.top

TS:   // 手写回溯递归
来源：http://pzt.gotoacloud.top

Java: // 手写回溯递归
来源：http://ekw.redwolf501.top

Go:   // 手写回溯递归
来源：http://msh.zhongyouzk.top

Ruby: arr.permutation.to_a
来源：http://czl.daria6918.cn

C#:   // 手写回溯递归
来源：http://bfs.zdqjudy.top

[N09] 栈与队列
来源：http://lzx.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://alk.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://elj.yongpay.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pag.chenzaomai.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eca.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oqm.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qnw.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yvy.birdmap.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rle.jinqigfzy.top

[N10] 链表节点定义
来源：http://rqy.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bfy.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://tms.zhaomingkeji.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jxa.jinyuanbaomall.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oqi.jyoumei.cn

Java: class Node { int v; Node next; }
来源：http://jyb.shzxlz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wif.zhongyouzk.top

Ruby: Node = Struct.new(:v, :next)
来源：http://frw.yvedp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://okb.zhaomingkeji.xyz

[N11] 二叉树中序遍历
来源：http://akn.zhijiandao.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://egn.chenjidiqi.icu

PHP:  // 手写递归函数
来源：http://ffq.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uph.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ffe.yanxiufei.cn

Java: // 手写递归
来源：http://bjb.pengpengdd.cyou

Go:   // 手写递归
来源：http://esb.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://edz.yuanzhike.top

C#:   // 手写递归
来源：http://vyz.shanyushiyangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xou.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kpf.guowangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://llr.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ubp.yanxiufei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://myn.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rwa.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rhz.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ynn.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lka.jyoumei.cn

================================================================================
来源：http://jzz.ppjwa.cn

O. 并发与异步
来源：http://deg.tanke756.top

================================================================================
来源：http://yba.fktsv.cn

[O01] 启动一个线程
来源：http://tvz.316326.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ifm.guannengcc.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://knz.hfpthk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xdf.kuanghao11.cn

TS:   // 同 JS
来源：http://yex.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://mor.aibaodan.cn

Go:   go f()
来源：http://icr.ydzc1.top

Ruby: Thread.new { f }
来源：http://wou.vqdsnc.cn

C#:   Task.Run(() => F());
来源：http://hyc.gzhubu.top

[O02] 使用线程池
来源：http://whc.ehwqpu.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oek.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ohj.fktsv.cn

JS:   // worker_threads 线程池
来源：http://xxe.xingfuxueyuan.xyz

TS:   // worker_threads 线程池
来源：http://poq.daria6918.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hvt.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wtc.yonumen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jma.ydjk.org.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fgt.cheryme.top

[O03] 加锁保护共享数据
来源：http://ztl.fzhhl.top

Py:   with lock: shared += 1
来源：http://dnk.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://mjn.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wer.ydjk.org.cn

TS:   // 同 JS
来源：http://qzt.tianlin.xyz

Java: synchronized (this) { shared++; }
来源：http://sxz.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dth.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://odq.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://ejw.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://pzu.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://rjt.yongpay.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xgj.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://aat.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://old.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rvp.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iqf.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://vdv.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://ksf.zhixingplan.top

[O05] 并发执行并等待全部完成
来源：http://jlr.wangdashe.top

Py:   asyncio.gather(*tasks)
来源：http://cch.yanxiufei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ade.yueranfly.top

JS:   await Promise.all(tasks)
来源：http://lsi.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://orr.jqgufenzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://njt.shuidangran.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://duc.andypj.xyz

Ruby: threads.map(&:join)
来源：http://tmv.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sej.jinqigfzy.top

[O06] 使用进程池
来源：http://igq.xuetiantiany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vhy.fanxiaobao.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://fkd.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://ojh.yj202588.top

TS:   // child_process / cluster 模块
来源：http://uxz.kuanghao11.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yfr.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blm.jlsjyb.cn

Ruby: // fork 块
来源：http://dya.epnwcf.com

C#:   Parallel.For
来源：http://mql.pycfn.com

================================================================================
来源：http://wdr.quarkkingdee.top

P. 常用工具函数
来源：http://iqn.cqqwz.cn

================================================================================
来源：http://wxs.zhengqikj.top

[P01] 生成 UUID
来源：http://hwr.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://zkq.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zjo.bbcook.cn

JS:   crypto.randomUUID()
来源：http://wgt.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://scr.yangfankeji.com

Java: UUID.randomUUID().toString()
来源：http://sgu.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://tol.xuanzx.com

Ruby: SecureRandom.uuid
来源：http://ooq.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://gkv.cqqwz.cn

[P02] MD5 / SHA256 摘要
来源：http://ohm.xziqi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wyz.jlsjyb.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gen.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fif.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://npy.tian-w.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://inj.zdqjudy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://awu.andypj.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hri.yueranfly.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ajk.guowangkeji.top

[P03] 生成短随机字符串
来源：http://zap.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fsu.ppjwa.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vuo.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xlg.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fco.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://esq.zdqjudy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jxm.ctjpmb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://rbq.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fmv.vehdjk.com

[P04] 求长度
来源：http://fcn.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uub.cdnleiting.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fym.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ifg.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://urf.vehdjk.com

Java: list.size();  map.size();  s.length()
来源：http://adg.gzhubu.top

Go:   len(arr);  len(m)
来源：http://puv.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://kxs.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://byx.quarkkingdee.top

[P05] 判断两个对象内容是否相等
来源：http://pav.tianlin.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://qfa.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://suv.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vlo.gotoacloud.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hix.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fuj.zhengqikj.top

Go:   reflect.DeepEqual(a, b)
来源：http://piy.ivvv.top

Ruby: a == b
来源：http://irx.zhijiandao.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zmy.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fxz.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://owt.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://gqo.yvedp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mzd.guannengcc.top

TS:   if (x == null) {}
来源：http://vhu.xziqi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://afg.zdqjudy.top

Go:   if x == nil {}
来源：http://wbc.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nsx.kuanghao11.cn

C#:   if (x is null) {}
来源：http://yna.snrcjt.cn

[P07] 防抖与节流
来源：http://apa.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qmy.guannengcc.top

PHP:  // 手写时间戳比较
来源：http://ile.bjfxy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lvv.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ngw.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nvb.hnqzz.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mod.xylfe.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hlw.aizwys.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bex.xinyue.icu

[P08] 处理浮点精度问题
来源：http://cuu.andypj.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dzd.cashguo.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wum.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uiv.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eqi.quarkkingdee.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vps.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lci.jinqigfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kag.ehwqpu.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ltf.sjlbkw.cn

================================================================================
来源：http://tye.jqgfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oda.aizwys.cn

================================================================================
来源：http://jvq.smart0.xyz

[Q01] 创建表
来源：http://zjv.iojbl.cn

CREATE TABLE users (
来源：http://bhu.ybcxt.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wbr.sufxvd.cn

name VARCHAR(50) NOT NULL,
来源：http://ahg.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://acf.fengsongda.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ten.hcnkem.com

);
来源：http://fvd.pycfn.com

[Q02] 创建带外键的表
来源：http://vms.hnqzz.top

CREATE TABLE orders (
来源：http://pxe.aibaodan.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jgg.ywan-chungtsiang.top

user_id INT NOT NULL,
来源：http://chs.jianghu66.top

amount DECIMAL(10, 2),
来源：http://ofo.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://afr.gzhubu.top

);
来源：http://joj.52xcode.cn

[Q03] 增加列
来源：http://gms.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mlh.ydzc1.top

[Q04] 修改列类型
来源：http://npv.bjfxy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hrf.gotoacloud.top

[Q05] 重命名列
来源：http://oea.ydjk.org.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hcp.yfazqb.com

[Q06] 删除列
来源：http://esx.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://nxh.tian-w.cn

[Q07] 删除表
来源：http://frr.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://wpn.52xcode.cn

[Q08] 创建普通索引
来源：http://jnq.daxiang520.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qfw.ctjpmb.com

[Q09] 创建唯一索引
来源：http://ufc.smart0.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lwt.iojbl.cn

[Q10] 插入单行
来源：http://ijs.fzhhl.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://usj.xziqi.cn

[Q11] 一次插入多行
来源：http://tur.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nwz.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://rnt.hnqzz.top

INSERT INTO users (name) VALUES ('C');
来源：http://ost.sufxvd.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qrp.epnwcf.com

[Q13] 忽略重复插入
来源：http://nyk.cdnleiting.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rpu.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://xzb.316326.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vup.jlsjyb.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://twy.316326.xyz

[Q15] 查询全部
来源：http://ufu.zdqjudy.top

SELECT * FROM users;
来源：http://aeq.tarul.cn

[Q16] 查询指定列
来源：http://itp.52xcode.cn

SELECT id, name FROM users;
来源：http://ixc.guannengcc.top

[Q17] 条件查询
来源：http://ecq.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://alg.jqgufenzy.top

[Q18] 模糊匹配
来源：http://mbg.zdbjq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oor.c1oappe.top

[Q19] 范围查询
来源：http://itm.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tqw.zhengqikj.top

[Q20] IN 列表
来源：http://ili.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iaj.smart0.xyz

[Q21] 空值判断
来源：http://qnm.jinyuanbaomall.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eiy.cqqwz.cn

[Q22] 排序
来源：http://oiw.ybcxt.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://acs.ivvv.top

[Q23] 分页
来源：http://pua.jqgufenzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uuk.fanxiaobao.xyz

[Q24] 去重
来源：http://zfx.havefunace.top

SELECT DISTINCT city FROM users;
来源：http://myg.ybcxt.top

[Q25] 只取前 N 条
来源：http://fha.jinqigfzy.top


<!-- 参考信息 -->