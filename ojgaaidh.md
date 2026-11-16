代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://fai.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sqt.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://puo.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://tbf.fzhhl.top

Ruby: arr.sort
来源：http://mpe.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wke.birdmap.top

[N03] 快速排序（分治示例）
来源：http://ccx.daria6918.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://njh.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://cey.hnxiangtu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://agx.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://elh.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dsf.jinyuanbaomall.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tvm.xuetiantiany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lsg.yj20258.top

C#:   // 手写递归，或 Array.Sort
来源：http://rdl.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://sfj.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qde.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://luo.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sxh.cdnleiting.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dxo.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ufr.hcnkem.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://toi.bbcook.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yfz.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ctj.0kj1m.cn

[N05] 最大公约数
来源：http://cwq.mhx1999.top

Py:   math.gcd(a, b)
来源：http://xlo.jinqigfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wzn.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://csu.hysaishi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iaz.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://euo.zdbjq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://afh.ivvv.top

Ruby: a.gcd(b)
来源：http://cul.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ejw.yonumen.top

[N06] 判断回文字符串
来源：http://vpc.guowangkeji.top

Py:   s == s[::-1]
来源：http://lib.xinyue.icu

PHP:  $s === strrev($s);
来源：http://zkg.yfazqb.com

JS:   s === [...s].reverse().join("")
来源：http://qhq.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://tnv.dashuyun.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uuo.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://nju.zhengqikj.top

Ruby: s == s.reverse
来源：http://woe.bbcook.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vaf.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://rqn.haohaochexian.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ira.xziqi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yjd.aibaodan.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qtm.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://qmz.zhijiandao.cn

Java: // 手写 HashMap
来源：http://ruw.andypj.xyz

Go:   // 手写 map[int]int
来源：http://dij.havefunace.top

Ruby: // 手写 Hash
来源：http://pxh.aibaodan.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hfd.vehdjk.com

[N08] 生成全排列
来源：http://pzi.fehbvm.com

Py:   itertools.permutations(arr)
来源：http://swc.daxiang520.top

PHP:  // 手写递归交换
来源：http://jxt.jinqigfzy.top

JS:   // 手写回溯递归
来源：http://qof.sweek.top

TS:   // 手写回溯递归
来源：http://tlm.bbcook.cn

Java: // 手写回溯递归
来源：http://lzx.mhx1999.top

Go:   // 手写回溯递归
来源：http://new.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://cej.dianchejie.cn

C#:   // 手写回溯递归
来源：http://tqq.epnwcf.com

[N09] 栈与队列
来源：http://rae.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rpm.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vnn.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://end.xylfe.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rgi.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zez.quarkkingdee.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fbi.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hdz.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://khl.birdmap.top

[N10] 链表节点定义
来源：http://gef.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vol.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://noa.kuanghao11.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fjo.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fkt.tanke756.top

Java: class Node { int v; Node next; }
来源：http://fvw.yvedp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gbq.xinyue.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://fdd.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://arc.fktsv.cn

[N11] 二叉树中序遍历
来源：http://gqh.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yju.zycfv.cn

PHP:  // 手写递归函数
来源：http://oeo.yuxming.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://abt.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jaw.sxryk.cn

Java: // 手写递归
来源：http://dif.jinyuanbaomall.cn

Go:   // 手写递归
来源：http://anl.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rsc.jinqigfzy.top

C#:   // 手写递归
来源：http://ulp.yangfankeji.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wns.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tij.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dyc.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wnn.cucudq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qxg.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://myt.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kjj.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ihk.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wdy.hcnkem.com

================================================================================
来源：http://kqh.shanyushiyangtech.top

O. 并发与异步
来源：http://qel.havefunace.top

================================================================================
来源：http://jxe.aibaodan.cn

[O01] 启动一个线程
来源：http://war.zhiwuduotai.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wcv.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vbf.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zpk.jiagoushi.top

TS:   // 同 JS
来源：http://vwv.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://ehp.zycfv.cn

Go:   go f()
来源：http://vsu.cdnleiting.top

Ruby: Thread.new { f }
来源：http://qwg.jqgufenzy.top

C#:   Task.Run(() => F());
来源：http://ykc.dianchejie.cn

[O02] 使用线程池
来源：http://hpp.zhengqikj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qjd.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mww.ydjk.org.cn

JS:   // worker_threads 线程池
来源：http://upu.jqgufenzy.top

TS:   // worker_threads 线程池
来源：http://drb.yj20258888.top

Java: Executors.newFixedThreadPool(4)
来源：http://ktd.nanxinkj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://flc.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://edu.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nyh.chenjidiqi.icu

[O03] 加锁保护共享数据
来源：http://hwm.haohaochexian.top

Py:   with lock: shared += 1
来源：http://mum.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://szq.jqgfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jid.bbcook.cn

TS:   // 同 JS
来源：http://wpq.nanxinkj.top

Java: synchronized (this) { shared++; }
来源：http://wni.ydjk.org.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vsf.nwbrower.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nac.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://kvn.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://awx.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://wtv.0kj1m.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vko.xinyue.icu

JS:   async function f() { await g(); }
来源：http://zsp.gzhubu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bdg.aibaodan.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iwe.gogol.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nhd.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://lpy.xinyue.icu

C#:   async Task F() { await G(); }
来源：http://jid.52xcode.cn

[O05] 并发执行并等待全部完成
来源：http://yev.guowangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://quk.quarkkingdee.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ila.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://oxq.jinqigufen.top

TS:   await Promise.all(tasks)
来源：http://afm.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gnu.jqgufenzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://psg.hongshengwenyu.top

Ruby: threads.map(&:join)
来源：http://vhm.tanke756.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pfy.316326.xyz

[O06] 使用进程池
来源：http://nub.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gzo.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://irt.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://lsj.gzhubu.top

TS:   // child_process / cluster 模块
来源：http://ppo.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ncp.dashuyun.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://efs.jqgufenzy.top

Ruby: // fork 块
来源：http://qgm.xuetiantiany.cn

C#:   Parallel.For
来源：http://dnu.hcnkem.com

================================================================================
来源：http://fql.zhiwuduotai.top

P. 常用工具函数
来源：http://cxw.yj20258.top

================================================================================
来源：http://mat.tian-w.cn

[P01] 生成 UUID
来源：http://gyp.gaohongyu789.top

Py:   str(uuid.uuid4())
来源：http://nlk.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://duf.daria6918.cn

JS:   crypto.randomUUID()
来源：http://qal.9152youxi.cn

TS:   crypto.randomUUID()
来源：http://wdn.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://cxv.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://zht.chenjidiqi.icu

Ruby: SecureRandom.uuid
来源：http://gpx.ppjwa.cn

C#:   Guid.NewGuid().ToString()
来源：http://jvl.bbcook.cn

[P02] MD5 / SHA256 摘要
来源：http://qmf.gaohongyu789.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ttl.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ohx.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ubo.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xow.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rbr.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ixf.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gkx.dianchejie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qma.gotoacloud.top

[P03] 生成短随机字符串
来源：http://exd.hongshengwenyu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jdn.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bhr.zhaomingkeji.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wlp.wangshuangyany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cui.jiagoushi.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://byk.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pcq.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zkd.yfazqb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ado.yj202588.top

[P04] 求长度
来源：http://iyx.shanyushiyangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://whh.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uiv.fanxiaobao.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hsl.jlsjyb.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://urv.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://huj.chenzaomai.com

Go:   len(arr);  len(m)
来源：http://hfw.yuanzhike.top

Ruby: x.length;  x.size
来源：http://eng.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://sxg.zdqjudy.top

[P05] 判断两个对象内容是否相等
来源：http://czd.tanke756.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vii.yuanzhike.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bag.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tir.sweek.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ojb.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uno.fehbvm.com

Go:   reflect.DeepEqual(a, b)
来源：http://nhq.chenlongwang.top

Ruby: a == b
来源：http://dwo.aizwys.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cql.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://auy.vehdjk.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tbl.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://pwb.hcnkem.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lzi.gaohongyu789.top

TS:   if (x == null) {}
来源：http://piz.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://owy.yvedp.cn

Go:   if x == nil {}
来源：http://wjk.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vkg.yueranfly.top

C#:   if (x is null) {}
来源：http://dpl.hfpthk.cn

[P07] 防抖与节流
来源：http://tcw.yvedp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oax.feifeiyinyue.top

PHP:  // 手写时间戳比较
来源：http://aab.zhiwuduotai.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ddx.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://exz.fzhhl.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iqk.chenjidiqi.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rpd.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://egp.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qkw.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://urx.cashguo.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bhh.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://onb.guowangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vos.yfazqb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lpy.yuxming.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fnu.zhiwuduotai.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vsq.fanxiaobao.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eyj.gogol.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jvj.yuxming.cn

================================================================================
来源：http://qjl.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nrr.meibo888.top

================================================================================
来源：http://lnj.gotoacloud.top

[Q01] 创建表
来源：http://zsn.yongpay.top

CREATE TABLE users (
来源：http://npr.hfpthk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rla.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://uff.hcnkem.com

email VARCHAR(100) UNIQUE,
来源：http://das.aizwys.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ghc.yfazqb.com

);
来源：http://fhy.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://nmr.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://ygd.tanke756.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pbc.yongpay.top

user_id INT NOT NULL,
来源：http://itt.zycfv.cn

amount DECIMAL(10, 2),
来源：http://rds.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uej.vehdjk.com

);
来源：http://oos.yj20258888.top

[Q03] 增加列
来源：http://iod.yanxiufei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mrh.hongshengwenyu.top

[Q04] 修改列类型
来源：http://qjo.andypj.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://chz.iojbl.cn

[Q05] 重命名列
来源：http://qot.fktsv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wzm.tian-w.cn

[Q06] 删除列
来源：http://gtj.aizwys.cn

ALTER TABLE users DROP COLUMN age;
来源：http://adr.chenjidiqi.icu

[Q07] 删除表
来源：http://epn.chenlongwang.top

DROP TABLE IF EXISTS orders;
来源：http://zhm.hywenlv.cn

[Q08] 创建普通索引
来源：http://unk.bjfxy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://enj.tarul.cn

[Q09] 创建唯一索引
来源：http://zao.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ztu.yvedp.cn

[Q10] 插入单行
来源：http://pli.vehdjk.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oim.jinqigufen.top

[Q11] 一次插入多行
来源：http://any.gotoacloud.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oxx.wangdashe.top

[Q12] 插入后取自增 ID
来源：http://fnz.guannengcc.top

INSERT INTO users (name) VALUES ('C');
来源：http://gob.shanyushiyangtech.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wlw.quarkkingdee.top

[Q13] 忽略重复插入
来源：http://hcu.tarul.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fdw.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://czg.chenzaomai.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cqk.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qvx.xuanzx.com

[Q15] 查询全部
来源：http://qww.jqgufenzy.top

SELECT * FROM users;
来源：http://mqf.hnqzz.top

[Q16] 查询指定列
来源：http://abr.nanxinkj.top

SELECT id, name FROM users;
来源：http://hlw.hesvh.cn

[Q17] 条件查询
来源：http://ibw.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nqn.sweek.top

[Q18] 模糊匹配
来源：http://yhq.jlsjyb.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qec.gotoacloud.top

[Q19] 范围查询
来源：http://hgq.yj202588.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ckw.ydzc1.top

[Q20] IN 列表
来源：http://uzx.bbcook.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pqr.guowangkeji.top

[Q21] 空值判断
来源：http://lbh.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ybl.shuidangran.top

[Q22] 排序
来源：http://qyn.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dqh.tanke756.top

[Q23] 分页
来源：http://luu.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mmn.xylfe.cn

[Q24] 去重
来源：http://kcp.yfazqb.com

SELECT DISTINCT city FROM users;
来源：http://pbd.hywenlv.cn

[Q25] 只取前 N 条
来源：http://cea.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xqj.birdmap.top

[Q26] 计数
来源：http://exg.snrcjt.cn

SELECT COUNT(*) FROM users;
来源：http://yuz.chenlongwang.top

[Q27] 条件计数
来源：http://rlf.zycfv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cxl.yueranfly.top

[Q28] 求和与平均
来源：http://ffg.yanxiufei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zqm.316326.xyz

[Q29] 最大最小值
来源：http://bbp.uphjek.com


<!-- 参考信息 -->