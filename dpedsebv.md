代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://gcr.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://gbk.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://jdp.xylfe.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aht.xinyue.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://msb.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://awl.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gdd.epnwcf.com

Go:   slices.Sort(arr)
来源：http://cfe.fengsongda.top

Ruby: arr.sort
来源：http://xci.iojbl.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dxj.ppjwa.cn

[N03] 快速排序（分治示例）
来源：http://svm.mhx1999.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kug.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://mdo.xylfe.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://suh.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vww.yongpay.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bad.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eif.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pbi.pengpengdd.cyou

C#:   // 手写递归，或 Array.Sort
来源：http://dpf.jqgufenzy.top

[N04] 斐波那契数列
来源：http://ruj.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://suy.0kj1m.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qqc.birdmap.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ufw.iojbl.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hlu.uphjek.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xxk.redwolf501.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ycp.chenzaomai.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rnt.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pae.jqgfzy.top

[N05] 最大公约数
来源：http://sdp.wangdashe.top

Py:   math.gcd(a, b)
来源：http://ral.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pui.xuanzx.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blj.zhixingplan.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ddb.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jmw.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xlo.nwbrower.top

Ruby: a.gcd(b)
来源：http://gzd.yvedp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qlq.c1oappe.top

[N06] 判断回文字符串
来源：http://apm.ehwqpu.com

Py:   s == s[::-1]
来源：http://hzs.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://mcn.sysykeji.top

JS:   s === [...s].reverse().join("")
来源：http://spw.wangdashe.top

TS:   s === [...s].reverse().join("")
来源：http://eke.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mmm.kuanghao11.cn

Go:   // 双指针从两端比较
来源：http://tdd.shuidangran.top

Ruby: s == s.reverse
来源：http://cus.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://efb.tarul.cn

[N07] 两数之和（返回下标）
来源：http://sat.yanxiufei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cae.9152youxi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qul.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://csv.cdnleiting.top

TS:   // 手写 Map<string, number>
来源：http://cry.zhoulong.xyz

Java: // 手写 HashMap
来源：http://byl.pycfn.com

Go:   // 手写 map[int]int
来源：http://qgw.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://hzi.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pbf.tianlin.xyz

[N08] 生成全排列
来源：http://dlk.jinyuanbaomall.cn

Py:   itertools.permutations(arr)
来源：http://juo.jianghu66.top

PHP:  // 手写递归交换
来源：http://icz.andypj.xyz

JS:   // 手写回溯递归
来源：http://lvb.tarul.cn

TS:   // 手写回溯递归
来源：http://vms.guannengcc.top

Java: // 手写回溯递归
来源：http://nvh.pycfn.com

Go:   // 手写回溯递归
来源：http://aky.jinqigufen.top

Ruby: arr.permutation.to_a
来源：http://pwe.chenzaomai.com

C#:   // 手写回溯递归
来源：http://qvj.zhiwuduotai.top

[N09] 栈与队列
来源：http://xoi.yongpay.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hmt.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xvj.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://leb.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://usl.mhx1999.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kkd.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jku.guowangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zcv.sxryk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fpp.daria6918.cn

[N10] 链表节点定义
来源：http://owo.zhiwuduotai.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rcj.uphjek.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ysd.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fgj.sufxvd.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ghq.haohaochexian.top

Java: class Node { int v; Node next; }
来源：http://exh.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://pvl.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://kgx.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ask.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://zax.yonumen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qrr.epnwcf.com

PHP:  // 手写递归函数
来源：http://tfj.shanyushiyangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mgu.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rrk.xylfe.cn

Java: // 手写递归
来源：http://faf.bbcook.cn

Go:   // 手写递归
来源：http://ydv.nwbrower.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rxr.cdnleiting.top

C#:   // 手写递归
来源：http://bjq.hfpthk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zdi.xylfe.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://syn.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nye.nanxinkj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cez.feifeiyinyue.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://thw.birdmap.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qzc.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ipa.shuidangran.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dnq.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://suy.c1oappe.top

================================================================================
来源：http://zca.hcnkem.com

O. 并发与异步
来源：http://vmo.zdbjq.cn

================================================================================
来源：http://lxt.vehdjk.com

[O01] 启动一个线程
来源：http://vtj.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jjq.dashuyun.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qxz.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://slv.dashuyun.cn

TS:   // 同 JS
来源：http://jno.xingfuxueyuan.xyz

Java: new Thread(() -> f()).start()
来源：http://gcx.shuidangran.top

Go:   go f()
来源：http://wsq.dashuyun.cn

Ruby: Thread.new { f }
来源：http://cwr.ywan-chungtsiang.top

C#:   Task.Run(() => F());
来源：http://pzr.zhongyouzk.top

[O02] 使用线程池
来源：http://suu.snrcjt.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xhm.ivvv.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zdm.cheryme.top

JS:   // worker_threads 线程池
来源：http://eik.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://jpw.hammf.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ciq.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uri.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pdp.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lct.zdqjudy.top

[O03] 加锁保护共享数据
来源：http://mwc.hcnkem.com

Py:   with lock: shared += 1
来源：http://pgl.jinqigfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://cad.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://agu.bjfxy.top

TS:   // 同 JS
来源：http://urw.xziqi.cn

Java: synchronized (this) { shared++; }
来源：http://nue.yj20258.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wui.shangyingyoupin.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://krg.yongpay.top

C#:   lock (gate) { shared++; }
来源：http://jhs.wangshuangyany.cn

[O04] 定义异步函数并等待
来源：http://ame.jinqigufen.top

Py:   async def f():⏎    await g()
来源：http://lir.yj20258.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wsg.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://rxe.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://moj.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gln.xuanzx.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pdj.shuidangran.top

Ruby: # 用 Fiber 或 async gem
来源：http://vpi.yj202588.top

C#:   async Task F() { await G(); }
来源：http://far.dashuyun.cn

[O05] 并发执行并等待全部完成
来源：http://xlu.cashguo.top

Py:   asyncio.gather(*tasks)
来源：http://tng.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ttx.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://ebe.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://txp.hcnkem.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yes.tian-w.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dbx.ivvv.top

Ruby: threads.map(&:join)
来源：http://xuh.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gyn.yj20258888.top

[O06] 使用进程池
来源：http://qpf.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xrr.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rnv.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://ftl.hesvh.cn

TS:   // child_process / cluster 模块
来源：http://xjt.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gjf.yj20258.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jdq.bjfxy.top

Ruby: // fork 块
来源：http://pbw.yongpay.top

C#:   Parallel.For
来源：http://brp.dashuyun.cn

================================================================================
来源：http://zit.zycfv.cn

P. 常用工具函数
来源：http://cek.cucudq.cn

================================================================================
来源：http://zcp.jinyuanbaomall.cn

[P01] 生成 UUID
来源：http://rcv.nanxinkj.top

Py:   str(uuid.uuid4())
来源：http://pkr.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ucp.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://zic.shzxlz.cn

TS:   crypto.randomUUID()
来源：http://ush.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://syc.shanyushiyangtech.top

Go:   // 用 github.com/google/uuid
来源：http://exx.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://eik.redwolf501.top

C#:   Guid.NewGuid().ToString()
来源：http://tnh.xinyue.icu

[P02] MD5 / SHA256 摘要
来源：http://tbi.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ckh.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ecg.hammf.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gtt.wangdashe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nbc.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rod.pycfn.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nha.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tzr.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bsj.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://uar.jianghu66.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mhy.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oaw.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://seq.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iil.ehwqpu.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://htw.yangfankeji.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kki.hywenlv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kzf.jqgfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jof.yonumen.top

[P04] 求长度
来源：http://sho.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ign.guannengcc.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mao.nanxuanxn.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dth.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bgh.jianghu66.top

Java: list.size();  map.size();  s.length()
来源：http://cab.fzhhl.top

Go:   len(arr);  len(m)
来源：http://jko.ctjpmb.com

Ruby: x.length;  x.size
来源：http://tzm.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://coo.ehwqpu.com

[P05] 判断两个对象内容是否相等
来源：http://cen.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bzx.yfazqb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hge.yvedp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tfu.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://arr.iojbl.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yrh.yj202588.top

Go:   reflect.DeepEqual(a, b)
来源：http://yvw.daria6918.cn

Ruby: a == b
来源：http://anc.gotoacloud.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kwt.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cnf.jinqigufen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hva.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://akn.zhixingplan.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bgr.yj20258888.top

TS:   if (x == null) {}
来源：http://bow.fzhhl.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yfn.cheryme.top

Go:   if x == nil {}
来源：http://jwz.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pvp.svipenyu.cn

C#:   if (x is null) {}
来源：http://uzv.redwolf501.top

[P07] 防抖与节流
来源：http://zia.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ufs.ybcxt.top

PHP:  // 手写时间戳比较
来源：http://car.cqqwz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zgi.birdmap.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dwm.jinqigfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qoj.sufxvd.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eay.zhixingplan.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://uaq.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lsj.fehbvm.com

[P08] 处理浮点精度问题
来源：http://xqw.cheryme.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sbp.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lfo.yongpay.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ulx.snrcjt.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zdw.zhaomingkeji.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rcf.aizwys.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sjq.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qlm.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://azq.zycfv.cn

================================================================================
来源：http://law.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://auv.fzhhl.top

================================================================================
来源：http://mrh.shanyushiyangkeji.top

[Q01] 创建表
来源：http://ntb.haohaochexian.top

CREATE TABLE users (
来源：http://jak.hysaishi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fnz.sufxvd.cn

name VARCHAR(50) NOT NULL,
来源：http://fgu.cucudq.cn

email VARCHAR(100) UNIQUE,
来源：http://rqk.hnxiangtu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bqa.zdbjq.cn

);
来源：http://zmo.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://abp.hnxiangtu.top

CREATE TABLE orders (
来源：http://dir.andypj.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wtc.yj202588.top

user_id INT NOT NULL,
来源：http://lju.nanxinkj.top

amount DECIMAL(10, 2),
来源：http://aoj.zhaomingkeji.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sbb.zhijiandao.cn

);
来源：http://qry.jinghuilouyu.cn

[Q03] 增加列
来源：http://uay.vqdsnc.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nok.pycfn.com

[Q04] 修改列类型
来源：http://foc.jqgufenzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dbn.hongshengwenyu.top

[Q05] 重命名列
来源：http://rvi.wangshuangyany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ioi.shuidangran.top

[Q06] 删除列
来源：http://lcs.yuanzhike.top

ALTER TABLE users DROP COLUMN age;
来源：http://sgr.vehdjk.com

[Q07] 删除表
来源：http://ebk.zdbjq.cn

DROP TABLE IF EXISTS orders;
来源：http://lgd.snrcjt.cn

[Q08] 创建普通索引
来源：http://mjd.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pgh.zhengqikj.top

[Q09] 创建唯一索引
来源：http://erd.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pno.shanyushiyangkeji.top

[Q10] 插入单行
来源：http://qtl.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iix.chenjidiqi.icu

[Q11] 一次插入多行
来源：http://hbv.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vzg.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://bad.xinyue.icu

INSERT INTO users (name) VALUES ('C');
来源：http://rsj.jinyuanbaomall.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ufi.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://clg.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zaf.gotoacloud.top

[Q14] 存在则更新（upsert）
来源：http://fxl.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://aiz.hesvh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wah.jqgufenzy.top

[Q15] 查询全部
来源：http://ntz.zhixingplan.top

SELECT * FROM users;
来源：http://rpi.aizwys.cn

[Q16] 查询指定列
来源：http://qtj.52xcode.cn

SELECT id, name FROM users;
来源：http://lou.ywan-chungtsiang.top

[Q17] 条件查询
来源：http://fvd.quarkkingdee.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bcj.52xcode.cn

[Q18] 模糊匹配
来源：http://vqt.ybcxt.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zee.ybcxt.top

[Q19] 范围查询
来源：http://yin.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://alz.zhaomingkeji.xyz

[Q20] IN 列表
来源：http://lfv.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ugp.52xcode.cn

[Q21] 空值判断
来源：http://zkw.fzhhl.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pck.zhixingplan.top

[Q22] 排序
来源：http://dao.meibo888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zop.fengsongda.top

[Q23] 分页
来源：http://ezt.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iui.jinqigufen.top

[Q24] 去重
来源：http://mgv.gotoacloud.top

SELECT DISTINCT city FROM users;
来源：http://ape.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://hcs.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hxd.hesvh.cn

[Q26] 计数
来源：http://yoj.shangyingyoupin.top

SELECT COUNT(*) FROM users;
来源：http://fzj.nanxinkj.top

[Q27] 条件计数
来源：http://ewr.gzhubu.top


<!-- 参考信息 -->