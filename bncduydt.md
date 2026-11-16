代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mlc.daxiang520.top

Java: Arrays.binarySearch(arr, x)
来源：http://hea.quarkkingdee.top

Go:   sort.SearchInts(arr, x)
来源：http://hva.ppjwa.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xre.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://mez.hesvh.cn

[N02] 排序（工程实践用内置实现）
来源：http://eeg.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://mdi.cdnleiting.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vbc.jlsjyb.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ssh.xingfuxueyuan.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://njv.zycfv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://stf.ehwqpu.com

Go:   slices.Sort(arr)
来源：http://ykh.yongpay.top

Ruby: arr.sort
来源：http://zcs.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zpd.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://ohi.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tnx.sweek.top

PHP:  // 递归实现，或用 usort
来源：http://pdy.wangdashe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ufz.epnwcf.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lgy.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ngj.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zjy.yanxiufei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jhe.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ejj.zhijiandao.cn

[N04] 斐波那契数列
来源：http://ogr.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fxk.nwbrower.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cds.xingfuxueyuan.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://thm.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gyk.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xxf.iojbl.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://awx.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cuo.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://onm.bjfxy.top

[N05] 最大公约数
来源：http://mle.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://yqf.yongpay.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://osv.yvedp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gzb.sweek.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qax.fengsongda.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rqe.gogol.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bht.daria6918.cn

Ruby: a.gcd(b)
来源：http://pet.chenjidiqi.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rvr.nanxuanxn.top

[N06] 判断回文字符串
来源：http://gjb.zhengqikj.top

Py:   s == s[::-1]
来源：http://kem.ywan-chungtsiang.top

PHP:  $s === strrev($s);
来源：http://mdg.smart0.xyz

JS:   s === [...s].reverse().join("")
来源：http://upy.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://nwa.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bmz.daria6918.cn

Go:   // 双指针从两端比较
来源：http://ixh.tian-w.cn

Ruby: s == s.reverse
来源：http://jrg.xingfuxueyuan.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://txr.jinqigfzy.top

[N07] 两数之和（返回下标）
来源：http://uof.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jdy.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mop.zhixingplan.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kij.fktsv.cn

TS:   // 手写 Map<string, number>
来源：http://dzw.hfpthk.cn

Java: // 手写 HashMap
来源：http://fsn.wangdashe.top

Go:   // 手写 map[int]int
来源：http://uro.snrcjt.cn

Ruby: // 手写 Hash
来源：http://glp.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xun.jiagoushi.top

[N08] 生成全排列
来源：http://mfa.yonumen.top

Py:   itertools.permutations(arr)
来源：http://mzq.vehdjk.com

PHP:  // 手写递归交换
来源：http://jen.aizwys.cn

JS:   // 手写回溯递归
来源：http://rmq.fzhhl.top

TS:   // 手写回溯递归
来源：http://amv.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://zrz.jinqigufen.top

Go:   // 手写回溯递归
来源：http://clt.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://nty.fktsv.cn

C#:   // 手写回溯递归
来源：http://mvb.hfpthk.cn

[N09] 栈与队列
来源：http://uuu.yongpay.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cla.shangyingyoupin.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vaq.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ifs.jinqigfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bur.haohaochexian.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zgp.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ifx.aibaodan.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zvo.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yne.uphjek.com

[N10] 链表节点定义
来源：http://lxx.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jid.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hxs.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://omd.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cac.pycfn.com

Java: class Node { int v; Node next; }
来源：http://hxe.hongshengwenyu.top

Go:   type Node struct { V int; Next *Node }
来源：http://epz.vehdjk.com

Ruby: Node = Struct.new(:v, :next)
来源：http://uqo.gzhubu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cqc.sysykeji.top

[N11] 二叉树中序遍历
来源：http://yqe.uphjek.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aeh.jyoumei.cn

PHP:  // 手写递归函数
来源：http://qjb.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wvc.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ege.fktsv.cn

Java: // 手写递归
来源：http://zys.nanxuanxn.top

Go:   // 手写递归
来源：http://sxx.ydzc1.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vhu.zdqjudy.top

C#:   // 手写递归
来源：http://haf.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vhz.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nfb.hfpthk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nrg.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jrv.haohaochexian.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zyh.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qgt.mhx1999.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pyr.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pjk.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yqj.shanyushiyangtech.top

================================================================================
来源：http://diz.ehwqpu.com

O. 并发与异步
来源：http://cpm.jinqigufen.top

================================================================================
来源：http://bdt.quarkkingdee.top

[O01] 启动一个线程
来源：http://qqg.yongpay.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mkt.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pkt.ctjpmb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jbk.bbcook.cn

TS:   // 同 JS
来源：http://afp.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://jny.ehwqpu.com

Go:   go f()
来源：http://nlh.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://sne.zhijiandao.cn

C#:   Task.Run(() => F());
来源：http://bdx.shuidangran.top

[O02] 使用线程池
来源：http://vbi.bbcook.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xgl.ydjk.org.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://axq.xinyue.icu

JS:   // worker_threads 线程池
来源：http://xtw.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://mof.aibaodan.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tre.hnxiangtu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fwe.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://czl.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cul.iojbl.cn

[O03] 加锁保护共享数据
来源：http://hws.zhijiandao.cn

Py:   with lock: shared += 1
来源：http://zpq.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://lgf.yvedp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rkt.sysykeji.top

TS:   // 同 JS
来源：http://ryf.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://fcj.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ucm.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bxy.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://gtu.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://pwa.epnwcf.com

Py:   async def f():⏎    await g()
来源：http://jjs.jinqigufen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ygo.sysykeji.top

JS:   async function f() { await g(); }
来源：http://bnt.cdnleiting.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lex.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://unw.redwolf501.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kkp.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://jha.nanxuanxn.top

C#:   async Task F() { await G(); }
来源：http://tby.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://wyu.jqgufenzy.top

Py:   asyncio.gather(*tasks)
来源：http://hva.ppjwa.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dzf.shuidangran.top

JS:   await Promise.all(tasks)
来源：http://xay.jqgufenzy.top

TS:   await Promise.all(tasks)
来源：http://ggo.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yqe.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kzq.feifeiyinyue.top

Ruby: threads.map(&:join)
来源：http://bgc.ydjk.org.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://koq.gogol.net.cn

[O06] 使用进程池
来源：http://pja.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cqr.zhongyouzk.top

PHP:  // pcntl_fork 或多进程队列
来源：http://usp.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://bbd.zhijiandao.cn

TS:   // child_process / cluster 模块
来源：http://wpn.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tkz.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ncd.hcnkem.com

Ruby: // fork 块
来源：http://wgs.feifeiyinyue.top

C#:   Parallel.For
来源：http://uys.yvedp.cn

================================================================================
来源：http://mun.fengsongda.top

P. 常用工具函数
来源：http://chy.yanxiufei.cn

================================================================================
来源：http://wnm.daxiang520.top

[P01] 生成 UUID
来源：http://yoe.shanyushiyangtech.top

Py:   str(uuid.uuid4())
来源：http://jnq.zhiwuduotai.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jeq.mhx1999.top

JS:   crypto.randomUUID()
来源：http://uba.jyoumei.cn

TS:   crypto.randomUUID()
来源：http://zyl.haohaochexian.top

Java: UUID.randomUUID().toString()
来源：http://gqe.yangfankeji.com

Go:   // 用 github.com/google/uuid
来源：http://wfl.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://iha.aizwys.cn

C#:   Guid.NewGuid().ToString()
来源：http://khk.tarul.cn

[P02] MD5 / SHA256 摘要
来源：http://kvj.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://elb.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uxd.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uzm.xylfe.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sed.tanke756.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bvq.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nqt.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://and.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://duj.xziqi.cn

[P03] 生成短随机字符串
来源：http://gos.hywenlv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uvh.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://omk.xuetiantiany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nuz.yj20258888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://asz.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qdq.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sjf.fzhhl.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mdu.hnqzz.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wil.zycfv.cn

[P04] 求长度
来源：http://ncc.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://thp.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gxj.52xcode.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mor.xylfe.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ulj.chenjidiqi.icu

Java: list.size();  map.size();  s.length()
来源：http://hwc.hesvh.cn

Go:   len(arr);  len(m)
来源：http://xgt.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://tjh.tianlin.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://hia.sysykeji.top

[P05] 判断两个对象内容是否相等
来源：http://hds.xuanzx.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://exk.c1oappe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kvp.yuxming.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zbz.zhijiandao.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wml.ivvv.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ffj.kuanghao11.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zuj.xingfuxueyuan.xyz

Ruby: a == b
来源：http://cpq.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hxt.jiagoushi.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jig.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hgi.nanxuanxn.top

PHP:  if (empty($x)) {}
来源：http://vlx.fehbvm.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qqi.fengsongda.top

TS:   if (x == null) {}
来源：http://qsa.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qrd.aizwys.cn

Go:   if x == nil {}
来源：http://cuy.quarkkingdee.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xzq.cdnleiting.top

C#:   if (x is null) {}
来源：http://lul.ydzc1.top

[P07] 防抖与节流
来源：http://mpc.yongpay.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xjv.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://icg.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nml.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zbn.svipenyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tvw.hywenlv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fxm.0kj1m.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sjf.cqqwz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gkc.wangshuangyany.cn

[P08] 处理浮点精度问题
来源：http://miv.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://khz.aibaodan.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vdx.shanyushiyangtech.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wst.xingfuxueyuan.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fbg.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wbk.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cfw.pycfn.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aop.hywenlv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gal.zhijiandao.cn

================================================================================
来源：http://wld.ybcxt.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qbf.zdqjudy.top

================================================================================
来源：http://lcp.shanyushiyangkeji.top

[Q01] 创建表
来源：http://afy.haohaochexian.top

CREATE TABLE users (
来源：http://wqv.nanxinkj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mav.0kj1m.cn

name VARCHAR(50) NOT NULL,
来源：http://mpe.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://pjr.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gye.fzhhl.top

);
来源：http://odu.316326.xyz

[Q02] 创建带外键的表
来源：http://qej.vehdjk.com

CREATE TABLE orders (
来源：http://wmp.chenjidiqi.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mmp.kuanghao11.cn

user_id INT NOT NULL,
来源：http://mns.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://ggs.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://san.tianlin.xyz

);
来源：http://uzg.cdnleiting.top

[Q03] 增加列
来源：http://fcf.yuxming.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cdb.andypj.xyz

[Q04] 修改列类型
来源：http://jmf.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cbf.epnwcf.com

[Q05] 重命名列
来源：http://nqb.xingfuxueyuan.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://foj.shanyushiyangkeji.top

[Q06] 删除列
来源：http://fky.shuidangran.top

ALTER TABLE users DROP COLUMN age;
来源：http://wjk.0kj1m.cn

[Q07] 删除表
来源：http://kcc.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://lqz.havefunace.top

[Q08] 创建普通索引
来源：http://vin.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fsj.hysaishi.cn

[Q09] 创建唯一索引
来源：http://ent.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jto.ctjpmb.com

[Q10] 插入单行
来源：http://rfg.zhixingplan.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nsc.snrcjt.cn

[Q11] 一次插入多行
来源：http://pig.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sur.kuanghao11.cn

[Q12] 插入后取自增 ID
来源：http://uhh.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://drv.yanxiufei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vlc.yangfankeji.com

[Q13] 忽略重复插入
来源：http://xhc.ydjk.org.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fzi.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://zgs.hywenlv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cdy.zhixingplan.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xix.ydjk.org.cn

[Q15] 查询全部
来源：http://tqd.feifeiyinyue.top

SELECT * FROM users;
来源：http://xij.guannengcc.top

[Q16] 查询指定列
来源：http://ika.yuanzhike.top

SELECT id, name FROM users;
来源：http://cjq.yj20258.top

[Q17] 条件查询
来源：http://nec.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yqi.havefunace.top

[Q18] 模糊匹配
来源：http://lbx.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kin.fengsongda.top

[Q19] 范围查询
来源：http://yvt.sxryk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://whm.tian-w.cn

[Q20] IN 列表
来源：http://sba.52xcode.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mmz.hcnkem.com

[Q21] 空值判断
来源：http://dqs.wangdashe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qmp.yuxming.cn

[Q22] 排序
来源：http://btz.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jme.jinghuilouyu.cn

[Q23] 分页
来源：http://dch.nanxinkj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ryo.zhixingplan.top

[Q24] 去重
来源：http://wta.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://dbb.zdbjq.cn

[Q25] 只取前 N 条
来源：http://mrr.xinyue.icu


<!-- 参考信息 -->