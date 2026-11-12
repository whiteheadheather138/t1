代发 wailian999

TS:   process.platform;  process.version
来源：http://rpt.tian-w.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kfa.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wnm.bbcook.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jeg.cdnleiting.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://szo.vqdsnc.cn

================================================================================
来源：http://gev.ybcxt.top

N. 数据结构与算法
来源：http://mqa.ydjk.org.cn

================================================================================
来源：http://qqc.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://wam.dianchejie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xlp.chenjidiqi.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ziy.hnxiangtu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mfv.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fkm.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://thb.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://phw.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qhx.tianlin.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://jau.bjfxy.top

[N02] 排序（工程实践用内置实现）
来源：http://guq.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://hhk.sjlbkw.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qel.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vcq.wangshuangyany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://caj.zhoulong.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hkt.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://lss.haohaochexian.top

Ruby: arr.sort
来源：http://xqj.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tms.vqdsnc.cn

[N03] 快速排序（分治示例）
来源：http://ssl.cdnleiting.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ujo.gaohongyu789.top

PHP:  // 递归实现，或用 usort
来源：http://hia.316326.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://egg.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cgc.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jvp.zhoulong.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pzk.andypj.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xtg.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bet.yuxming.cn

[N04] 斐波那契数列
来源：http://ljd.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kan.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sxj.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://snn.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://elc.yangfankeji.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cxv.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://whm.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jqk.fktsv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lml.shanyushiyangkeji.top

[N05] 最大公约数
来源：http://uma.uphjek.com

Py:   math.gcd(a, b)
来源：http://lub.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eic.fanxiaobao.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zhr.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jyf.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://icw.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aeg.sjlbkw.cn

Ruby: a.gcd(b)
来源：http://uhb.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://emr.cdnleiting.top

[N06] 判断回文字符串
来源：http://noi.ppjwa.cn

Py:   s == s[::-1]
来源：http://hqy.jiagoushi.top

PHP:  $s === strrev($s);
来源：http://udh.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://vbv.xinyue.icu

TS:   s === [...s].reverse().join("")
来源：http://pxs.epnwcf.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iop.shuidangran.top

Go:   // 双指针从两端比较
来源：http://col.mhx1999.top

Ruby: s == s.reverse
来源：http://uas.tanke756.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cyf.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://aor.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uya.sufxvd.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jbg.wangdashe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kba.jlsjyb.cn

TS:   // 手写 Map<string, number>
来源：http://sjc.guowangkeji.top

Java: // 手写 HashMap
来源：http://mpz.hnqzz.top

Go:   // 手写 map[int]int
来源：http://wgp.ppjwa.cn

Ruby: // 手写 Hash
来源：http://mpf.tanke756.top

C#:   // 手写 Dictionary<int, int>
来源：http://gct.wangdashe.top

[N08] 生成全排列
来源：http://ggu.bbcook.cn

Py:   itertools.permutations(arr)
来源：http://tnt.feifeiyinyue.top

PHP:  // 手写递归交换
来源：http://nwt.ctjpmb.com

JS:   // 手写回溯递归
来源：http://vru.guowangkeji.top

TS:   // 手写回溯递归
来源：http://uxo.pycfn.com

Java: // 手写回溯递归
来源：http://abm.jiagoushi.top

Go:   // 手写回溯递归
来源：http://suz.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://ejv.tanke756.top

C#:   // 手写回溯递归
来源：http://sio.ydzc1.top

[N09] 栈与队列
来源：http://jnk.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wxi.tanke756.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pwu.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uxo.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vyw.zhongyouzk.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iaj.c1oappe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tgq.fengsongda.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zzi.yfazqb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rfq.andypj.xyz

[N10] 链表节点定义
来源：http://qwl.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rgd.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://khs.ybcxt.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ymx.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wny.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://ihq.yvedp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xan.ctjpmb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://zpx.xinyue.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://jzg.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://mkt.ivvv.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yeo.hesvh.cn

PHP:  // 手写递归函数
来源：http://hzy.chenzaomai.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://val.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://arz.316326.xyz

Java: // 手写递归
来源：http://daj.ehwqpu.com

Go:   // 手写递归
来源：http://lps.hcnkem.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qnt.shzxlz.cn

C#:   // 手写递归
来源：http://byb.yonumen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nlu.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gpq.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bgw.kuanghao11.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://esh.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pap.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dkj.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pef.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ojt.gzhubu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oed.smart0.xyz

================================================================================
来源：http://mim.hongshengwenyu.top

O. 并发与异步
来源：http://zzr.feifeiyinyue.top

================================================================================
来源：http://pts.fehbvm.com

[O01] 启动一个线程
来源：http://jwm.uphjek.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://whe.c1oappe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cbc.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bua.meibo888.top

TS:   // 同 JS
来源：http://gat.yj20258.top

Java: new Thread(() -> f()).start()
来源：http://xey.fzhhl.top

Go:   go f()
来源：http://uat.ydzc1.top

Ruby: Thread.new { f }
来源：http://bsp.ydzc1.top

C#:   Task.Run(() => F());
来源：http://dmy.fanxiaobao.xyz

[O02] 使用线程池
来源：http://ari.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ztj.yueranfly.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kda.vehdjk.com

JS:   // worker_threads 线程池
来源：http://ciz.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://dqk.fengsongda.top

Java: Executors.newFixedThreadPool(4)
来源：http://eqa.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xps.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rfa.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wcx.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://ypr.snrcjt.cn

Py:   with lock: shared += 1
来源：http://iue.zycfv.cn

PHP:  // 用 flock() 做文件锁
来源：http://svd.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://syh.jianghu66.top

TS:   // 同 JS
来源：http://lmk.jqgfzy.top

Java: synchronized (this) { shared++; }
来源：http://ose.snrcjt.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mkg.yj20258.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gre.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://wbu.birdmap.top

[O04] 定义异步函数并等待
来源：http://tvp.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://ugd.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://muu.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://hwx.yuanzhike.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zck.52xcode.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://feg.daria6918.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lvv.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://ggq.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://hhf.aibaodan.cn

[O05] 并发执行并等待全部完成
来源：http://lkg.fengsongda.top

Py:   asyncio.gather(*tasks)
来源：http://twf.zdqjudy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lrg.chenzaomai.com

JS:   await Promise.all(tasks)
来源：http://jps.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://hba.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mrl.fengsongda.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yzg.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://ntk.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tnv.shanyushiyangkeji.top

[O06] 使用进程池
来源：http://ztp.zhengqikj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sei.316326.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://ypf.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://fss.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://inr.meibo888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kxn.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ktt.ydzc1.top

Ruby: // fork 块
来源：http://ymz.xziqi.cn

C#:   Parallel.For
来源：http://rsf.ehwqpu.com

================================================================================
来源：http://unx.wangshuangyany.cn

P. 常用工具函数
来源：http://qux.xinyue.icu

================================================================================
来源：http://aae.bjfxy.top

[P01] 生成 UUID
来源：http://epf.redwolf501.top

Py:   str(uuid.uuid4())
来源：http://koz.jqgfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bdc.meibo888.top

JS:   crypto.randomUUID()
来源：http://jwq.fktsv.cn

TS:   crypto.randomUUID()
来源：http://kpe.ydjk.org.cn

Java: UUID.randomUUID().toString()
来源：http://sqq.uphjek.com

Go:   // 用 github.com/google/uuid
来源：http://xzf.zhongyouzk.top

Ruby: SecureRandom.uuid
来源：http://lvl.316326.xyz

C#:   Guid.NewGuid().ToString()
来源：http://jti.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://nqs.xziqi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://deo.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vsb.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rkn.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ixm.yj20258888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nhm.hysaishi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cro.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rte.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tfj.cdnleiting.top

[P03] 生成短随机字符串
来源：http://wgm.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://owj.316326.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://awd.hnxiangtu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://raj.tanke756.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kwj.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uas.jinqigufen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cyv.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://vjr.jinqigfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wgn.zhoulong.xyz

[P04] 求长度
来源：http://mwj.shzxlz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://epu.yangfankeji.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oyl.hammf.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://liv.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lua.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://fkj.dianchejie.cn

Go:   len(arr);  len(m)
来源：http://rxj.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://lca.fengsongda.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xyw.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://dkf.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xec.yanxiufei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yko.uphjek.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ajg.bbcook.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xvb.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sbu.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://tki.hysaishi.cn

Ruby: a == b
来源：http://umj.zycfv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mbx.xziqi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cij.cdnleiting.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bou.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://hpu.cashguo.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zyx.zhiwuduotai.top

TS:   if (x == null) {}
来源：http://aoz.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://hxe.ydjk.org.cn

Go:   if x == nil {}
来源：http://yyu.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hxz.sufxvd.cn

C#:   if (x is null) {}
来源：http://xfp.meibo888.top

[P07] 防抖与节流
来源：http://utk.yvedp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://csi.yj20258.top

PHP:  // 手写时间戳比较
来源：http://kcs.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tnd.shuidangran.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fra.gaohongyu789.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://znu.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://shp.smart0.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://eqv.iojbl.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cpp.quarkkingdee.top

[P08] 处理浮点精度问题
来源：http://kua.fengsongda.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oxw.cheryme.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dfe.zycfv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pwn.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cxi.aizwys.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aqu.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nqr.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://soj.tian-w.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://swa.yueranfly.top

================================================================================
来源：http://gco.sufxvd.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ids.xuanzx.com

================================================================================
来源：http://isy.jinqigfzy.top

[Q01] 创建表
来源：http://eka.shangyingyoupin.top

CREATE TABLE users (
来源：http://tdj.gaohongyu789.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qrx.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://wqf.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://uey.uphjek.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uvt.xinyue.icu

);
来源：http://qlo.tarul.cn

[Q02] 创建带外键的表
来源：http://azy.xuanzx.com

CREATE TABLE orders (
来源：http://qta.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cio.daria6918.cn

user_id INT NOT NULL,
来源：http://oak.316326.xyz

amount DECIMAL(10, 2),
来源：http://wmk.shzxlz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uoo.dianchejie.cn

);
来源：http://hzi.c1oappe.top

[Q03] 增加列
来源：http://kfh.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lvm.zdbjq.cn

[Q04] 修改列类型
来源：http://olt.dianchejie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://thh.havefunace.top

[Q05] 重命名列
来源：http://gyn.guannengcc.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vxz.ybcxt.top

[Q06] 删除列
来源：http://vpy.aibaodan.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rhx.fehbvm.com

[Q07] 删除表
来源：http://qie.jinyuanbaomall.cn

DROP TABLE IF EXISTS orders;
来源：http://qsa.sysykeji.top

[Q08] 创建普通索引
来源：http://adu.tanke756.top

CREATE INDEX idx_users_email ON users(email);
来源：http://egh.tianlin.xyz

[Q09] 创建唯一索引
来源：http://dyk.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tjz.hywenlv.cn

[Q10] 插入单行
来源：http://wkw.guowangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hmx.chenlongwang.top

[Q11] 一次插入多行
来源：http://tid.sweek.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ikd.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://zos.xuetiantiany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://aey.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://czu.yj20258.top

[Q13] 忽略重复插入
来源：http://iir.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://plp.316326.xyz

[Q14] 存在则更新（upsert）
来源：http://xja.jinghuilouyu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qez.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ujh.yuanzhike.top

[Q15] 查询全部
来源：http://kgn.jiagoushi.top

SELECT * FROM users;
来源：http://kci.meibo888.top

[Q16] 查询指定列
来源：http://hbb.redwolf501.top

SELECT id, name FROM users;
来源：http://ayr.sysykeji.top

[Q17] 条件查询
来源：http://kau.nanxinkj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xqs.ydzc1.top

[Q18] 模糊匹配
来源：http://fsd.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://knk.jlsjyb.cn

[Q19] 范围查询
来源：http://zxr.jlsjyb.cn


<!-- 参考信息 -->