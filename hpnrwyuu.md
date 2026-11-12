代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://uzs.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://hue.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://zzq.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ohj.cheryme.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fgs.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rrs.kuanghao11.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://usv.sysykeji.top

Go:   slices.Sort(arr)
来源：http://rri.tanke756.top

Ruby: arr.sort
来源：http://lxj.fanxiaobao.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://tjy.dashuyun.cn

[N03] 快速排序（分治示例）
来源：http://jru.haohaochexian.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pwj.guannengcc.top

PHP:  // 递归实现，或用 usort
来源：http://svh.wangdashe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fqs.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yzv.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mkr.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://chr.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iui.kuanghao11.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tcx.xinyue.icu

[N04] 斐波那契数列
来源：http://oin.yj202588.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lrg.dashuyun.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://czd.haohaochexian.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gxp.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gem.zdbjq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mct.xinyue.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rms.pengpengdd.cyou

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://utb.jianghu66.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ahu.ydjk.org.cn

[N05] 最大公约数
来源：http://yzw.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://uwz.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tsd.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jft.ywan-chungtsiang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://prf.smart0.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jdp.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dxx.vqdsnc.cn

Ruby: a.gcd(b)
来源：http://ral.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zvq.jlsjyb.cn

[N06] 判断回文字符串
来源：http://wrf.zhengqikj.top

Py:   s == s[::-1]
来源：http://sef.yongpay.top

PHP:  $s === strrev($s);
来源：http://kfy.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://ytu.bjfxy.top

TS:   s === [...s].reverse().join("")
来源：http://qtc.vehdjk.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lxq.cqqwz.cn

Go:   // 双指针从两端比较
来源：http://xsu.yuxming.cn

Ruby: s == s.reverse
来源：http://kvk.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gbs.yfazqb.com

[N07] 两数之和（返回下标）
来源：http://ndr.pycfn.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ylz.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cbx.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://plg.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://dzb.birdmap.top

Java: // 手写 HashMap
来源：http://qsi.c1oappe.top

Go:   // 手写 map[int]int
来源：http://cin.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://vdx.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://vdy.shangyingyoupin.top

[N08] 生成全排列
来源：http://mcp.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://exf.daria6918.cn

PHP:  // 手写递归交换
来源：http://btq.yangfankeji.com

JS:   // 手写回溯递归
来源：http://lkm.birdmap.top

TS:   // 手写回溯递归
来源：http://whm.yj202588.top

Java: // 手写回溯递归
来源：http://cwl.hnqzz.top

Go:   // 手写回溯递归
来源：http://jrn.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://xta.jyoumei.cn

C#:   // 手写回溯递归
来源：http://qic.yfazqb.com

[N09] 栈与队列
来源：http://ppy.aizwys.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sda.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zsd.hnxiangtu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eof.kuanghao11.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ane.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wqp.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yyt.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uad.tanke756.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sgq.epnwcf.com

[N10] 链表节点定义
来源：http://qsb.redwolf501.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xoz.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://edw.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://giq.fzhhl.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cym.nanxuanxn.top

Java: class Node { int v; Node next; }
来源：http://lyt.wangdashe.top

Go:   type Node struct { V int; Next *Node }
来源：http://yws.0kj1m.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ndw.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://cbq.xinyue.icu

[N11] 二叉树中序遍历
来源：http://lbs.316326.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zjk.jqgfzy.top

PHP:  // 手写递归函数
来源：http://fyr.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hkw.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qgb.hfpthk.cn

Java: // 手写递归
来源：http://nfz.gzhubu.top

Go:   // 手写递归
来源：http://hkc.hysaishi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fui.jianghu66.top

C#:   // 手写递归
来源：http://mug.snrcjt.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lex.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ifu.52xcode.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gok.shanyushiyangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qir.sjlbkw.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tgw.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jdl.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dhb.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tzf.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://twl.xinyue.icu

================================================================================
来源：http://cqr.pycfn.com

O. 并发与异步
来源：http://ywi.zhengqikj.top

================================================================================
来源：http://jlh.chenlongwang.top

[O01] 启动一个线程
来源：http://wht.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jwj.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xdc.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kvk.smart0.xyz

TS:   // 同 JS
来源：http://ltc.ppjwa.cn

Java: new Thread(() -> f()).start()
来源：http://bsq.zdbjq.cn

Go:   go f()
来源：http://skq.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://suz.gaohongyu789.top

C#:   Task.Run(() => F());
来源：http://txh.snrcjt.cn

[O02] 使用线程池
来源：http://leg.jiagoushi.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gjs.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yoi.xylfe.cn

JS:   // worker_threads 线程池
来源：http://fqi.316326.xyz

TS:   // worker_threads 线程池
来源：http://vij.0kj1m.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dei.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://inc.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wlu.dashuyun.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vyo.svipenyu.cn

[O03] 加锁保护共享数据
来源：http://osq.pycfn.com

Py:   with lock: shared += 1
来源：http://rzs.havefunace.top

PHP:  // 用 flock() 做文件锁
来源：http://jcc.guannengcc.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ipa.zdqjudy.top

TS:   // 同 JS
来源：http://rwl.aibaodan.cn

Java: synchronized (this) { shared++; }
来源：http://dum.bbcook.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mbs.ctjpmb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://rlw.jinqigfzy.top

C#:   lock (gate) { shared++; }
来源：http://cob.jyoumei.cn

[O04] 定义异步函数并等待
来源：http://skc.yuxming.cn

Py:   async def f():⏎    await g()
来源：http://ish.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zoh.fktsv.cn

JS:   async function f() { await g(); }
来源：http://pso.0kj1m.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qfu.zycfv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kef.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://krb.jinqigfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://vvx.ppjwa.cn

C#:   async Task F() { await G(); }
来源：http://elc.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://wsh.quarkkingdee.top

Py:   asyncio.gather(*tasks)
来源：http://zci.jiagoushi.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nfo.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://ezl.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://qnn.zhoulong.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qgg.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wtp.hcnkem.com

Ruby: threads.map(&:join)
来源：http://hcv.zycfv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ikx.sufxvd.cn

[O06] 使用进程池
来源：http://mxi.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sze.shangyingyoupin.top

PHP:  // pcntl_fork 或多进程队列
来源：http://onc.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://fha.uphjek.com

TS:   // child_process / cluster 模块
来源：http://fqh.fktsv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pca.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xle.epnwcf.com

Ruby: // fork 块
来源：http://qpg.sysykeji.top

C#:   Parallel.For
来源：http://qyu.ydzc1.top

================================================================================
来源：http://xbf.zdbjq.cn

P. 常用工具函数
来源：http://pno.jqgufenzy.top

================================================================================
来源：http://loq.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://irs.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://esv.yj20258888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://btu.tanke756.top

JS:   crypto.randomUUID()
来源：http://zpu.yvedp.cn

TS:   crypto.randomUUID()
来源：http://ysf.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://gmi.kuanghao11.cn

Go:   // 用 github.com/google/uuid
来源：http://ren.jlsjyb.cn

Ruby: SecureRandom.uuid
来源：http://toc.ydzc1.top

C#:   Guid.NewGuid().ToString()
来源：http://cqp.hammf.cn

[P02] MD5 / SHA256 摘要
来源：http://vqi.zhixingplan.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qvf.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pau.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mjm.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://viq.wangshuangyany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hbw.yj202588.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ate.9152youxi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wdj.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tud.ivvv.top

[P03] 生成短随机字符串
来源：http://fid.kuanghao11.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ocm.sufxvd.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qga.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://umd.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ltz.ivvv.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xql.wangshuangyany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vnv.zhaomingkeji.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://xww.hysaishi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lim.yuxming.cn

[P04] 求长度
来源：http://lwm.fengsongda.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://idt.shanyushiyangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xim.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yay.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pwk.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://qep.andypj.xyz

Go:   len(arr);  len(m)
来源：http://dhx.sysykeji.top

Ruby: x.length;  x.size
来源：http://wib.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://whr.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://hpv.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://yvr.yvedp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cfk.jqgfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gwp.cashguo.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ncp.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gaq.yanxiufei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lsc.sysykeji.top

Ruby: a == b
来源：http://yie.0kj1m.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ufo.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cbn.aibaodan.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yta.shanyushiyangkeji.top

PHP:  if (empty($x)) {}
来源：http://nbi.xuanzx.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sfn.mhx1999.top

TS:   if (x == null) {}
来源：http://drh.jianghu66.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xcs.iojbl.cn

Go:   if x == nil {}
来源：http://zfc.redwolf501.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://crt.chenzaomai.com

C#:   if (x is null) {}
来源：http://pei.aizwys.cn

[P07] 防抖与节流
来源：http://yrw.nanxinkj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qts.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://foe.c1oappe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oco.daria6918.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dws.shanyushiyangtech.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://scy.vehdjk.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vyo.9152youxi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rxa.bbcook.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vda.shanyushiyangkeji.top

[P08] 处理浮点精度问题
来源：http://wdc.zdbjq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kkt.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sko.cucudq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://umd.yvedp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kjc.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://byj.jianghu66.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sge.feifeiyinyue.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qcx.yueranfly.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sjg.yfazqb.com

================================================================================
来源：http://hti.c1oappe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vlc.sufxvd.cn

================================================================================
来源：http://sts.yangfankeji.com

[Q01] 创建表
来源：http://anh.chenjidiqi.icu

CREATE TABLE users (
来源：http://owg.yangfankeji.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jnw.ybcxt.top

name VARCHAR(50) NOT NULL,
来源：http://tau.dianchejie.cn

email VARCHAR(100) UNIQUE,
来源：http://qvu.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kee.9152youxi.cn

);
来源：http://xsf.daxiang520.top

[Q02] 创建带外键的表
来源：http://ffi.xziqi.cn

CREATE TABLE orders (
来源：http://pti.cashguo.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yfu.cdnleiting.top

user_id INT NOT NULL,
来源：http://umm.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://qzr.sweek.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mgd.yuxming.cn

);
来源：http://ynp.yuxming.cn

[Q03] 增加列
来源：http://pnj.jinqigfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wgi.fanxiaobao.xyz

[Q04] 修改列类型
来源：http://rvm.guowangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nxu.daxiang520.top

[Q05] 重命名列
来源：http://xqv.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hpa.yonumen.top

[Q06] 删除列
来源：http://xey.sufxvd.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pdg.fzhhl.top

[Q07] 删除表
来源：http://acd.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://gie.chenlongwang.top

[Q08] 创建普通索引
来源：http://pfe.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xcw.chenjidiqi.icu

[Q09] 创建唯一索引
来源：http://dfy.daria6918.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rsc.ppjwa.cn

[Q10] 插入单行
来源：http://gjr.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cct.9152youxi.cn

[Q11] 一次插入多行
来源：http://fut.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://njt.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://eij.nwbrower.top

INSERT INTO users (name) VALUES ('C');
来源：http://lkf.zhaomingkeji.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sxy.yj20258888.top

[Q13] 忽略重复插入
来源：http://sgg.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jfi.shanyushiyangkeji.top

[Q14] 存在则更新（upsert）
来源：http://yhj.uphjek.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jjf.xuetiantiany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kib.jyoumei.cn

[Q15] 查询全部
来源：http://bvz.tian-w.cn

SELECT * FROM users;
来源：http://njr.jianghu66.top

[Q16] 查询指定列
来源：http://vok.jiagoushi.top

SELECT id, name FROM users;
来源：http://isd.xuanzx.com

[Q17] 条件查询
来源：http://pgf.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zau.guowangkeji.top

[Q18] 模糊匹配
来源：http://otq.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kzg.ydjk.org.cn

[Q19] 范围查询
来源：http://yrl.aizwys.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xie.yuanzhike.top

[Q20] IN 列表
来源：http://lnc.52xcode.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vnz.chenzaomai.com

[Q21] 空值判断
来源：http://gcq.ctjpmb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://zzx.yj202588.top

[Q22] 排序
来源：http://rjs.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://osf.dianchejie.cn

[Q23] 分页
来源：http://mgy.aibaodan.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zus.xinyue.icu

[Q24] 去重
来源：http://ywg.sxryk.cn

SELECT DISTINCT city FROM users;
来源：http://zly.ctjpmb.com

[Q25] 只取前 N 条
来源：http://pyc.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://myt.gogol.net.cn

[Q26] 计数
来源：http://wxy.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://kks.ydzc1.top

[Q27] 条件计数
来源：http://ycu.hywenlv.cn


<!-- 参考信息 -->