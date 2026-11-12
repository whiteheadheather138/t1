代发 wailian999

TS:   process.platform;  process.version
来源：http://fur.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xmg.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vvk.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nsh.chenzaomai.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://sgn.havefunace.top

================================================================================
来源：http://jla.0kj1m.cn

N. 数据结构与算法
来源：http://npf.wangshuangyany.cn

================================================================================
来源：http://mos.tanke756.top

[N01] 二分查找（有序数组）
来源：http://qte.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://hfr.zhijiandao.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bmj.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xsw.yuxming.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ufn.tianlin.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://jes.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://iry.birdmap.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hef.daria6918.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bjd.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://khq.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://vrl.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://izo.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://bst.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://evv.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hbu.xinyue.icu

Go:   slices.Sort(arr)
来源：http://ndo.aibaodan.cn

Ruby: arr.sort
来源：http://gkg.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bcx.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://yzf.chenzaomai.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://okq.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://fhl.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://phi.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zsv.zhengqikj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bjs.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rbq.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mwv.gogol.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cqs.xuanzx.com

[N04] 斐波那契数列
来源：http://ert.sxryk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rkp.hongshengwenyu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ugb.zhaomingkeji.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://isq.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pcy.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://plt.chenjidiqi.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vxo.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yyi.zhixingplan.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ovd.svipenyu.cn

[N05] 最大公约数
来源：http://qcd.jlsjyb.cn

Py:   math.gcd(a, b)
来源：http://ujs.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ksg.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jgt.zdqjudy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mek.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jko.sysykeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bfu.sysykeji.top

Ruby: a.gcd(b)
来源：http://msr.zhaomingkeji.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tjb.sjlbkw.cn

[N06] 判断回文字符串
来源：http://mwg.yonumen.top

Py:   s == s[::-1]
来源：http://cqy.jlsjyb.cn

PHP:  $s === strrev($s);
来源：http://fjf.jqgufenzy.top

JS:   s === [...s].reverse().join("")
来源：http://tcy.xuanzx.com

TS:   s === [...s].reverse().join("")
来源：http://cjw.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lpa.316326.xyz

Go:   // 双指针从两端比较
来源：http://rrz.tianlin.xyz

Ruby: s == s.reverse
来源：http://mgs.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://xst.gotoacloud.top

[N07] 两数之和（返回下标）
来源：http://xmv.sufxvd.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://byg.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xgd.zhixingplan.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mln.pengpengdd.cyou

TS:   // 手写 Map<string, number>
来源：http://tha.cdnleiting.top

Java: // 手写 HashMap
来源：http://jnr.ydjk.org.cn

Go:   // 手写 map[int]int
来源：http://dta.tian-w.cn

Ruby: // 手写 Hash
来源：http://cje.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sxo.nwbrower.top

[N08] 生成全排列
来源：http://fft.zhaomingkeji.xyz

Py:   itertools.permutations(arr)
来源：http://kpl.ehwqpu.com

PHP:  // 手写递归交换
来源：http://pfx.daria6918.cn

JS:   // 手写回溯递归
来源：http://gqi.yj202588.top

TS:   // 手写回溯递归
来源：http://qtf.c1oappe.top

Java: // 手写回溯递归
来源：http://uua.jinghuilouyu.cn

Go:   // 手写回溯递归
来源：http://asi.yj202588.top

Ruby: arr.permutation.to_a
来源：http://gjq.chenlongwang.top

C#:   // 手写回溯递归
来源：http://bie.ydzc1.top

[N09] 栈与队列
来源：http://ztf.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://caw.shangyingyoupin.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://stm.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zbm.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://chu.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wos.iojbl.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://obs.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nlv.quarkkingdee.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cca.tian-w.cn

[N10] 链表节点定义
来源：http://svg.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rst.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zkv.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uos.havefunace.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hwj.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://kxx.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://tud.hnxiangtu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nng.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://isy.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://gwc.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mgv.9152youxi.cn

PHP:  // 手写递归函数
来源：http://hcq.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dwj.zhengqikj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jjz.xziqi.cn

Java: // 手写递归
来源：http://mfy.wangdashe.top

Go:   // 手写递归
来源：http://fjq.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yvw.fengsongda.top

C#:   // 手写递归
来源：http://chd.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://otd.gaohongyu789.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fav.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qiw.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cko.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pcg.jinyuanbaomall.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ymx.cheryme.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dsz.52xcode.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://psa.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://glc.yongpay.top

================================================================================
来源：http://ths.yj20258888.top

O. 并发与异步
来源：http://utg.kuanghao11.cn

================================================================================
来源：http://tpp.jianghu66.top

[O01] 启动一个线程
来源：http://zom.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hab.xuanzx.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zbu.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yex.sxryk.cn

TS:   // 同 JS
来源：http://wju.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://tvz.pengpengdd.cyou

Go:   go f()
来源：http://qmz.ppjwa.cn

Ruby: Thread.new { f }
来源：http://rlu.gaohongyu789.top

C#:   Task.Run(() => F());
来源：http://ogn.jinqigufen.top

[O02] 使用线程池
来源：http://wvv.wangshuangyany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sem.0kj1m.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dsr.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://gpp.feifeiyinyue.top

TS:   // worker_threads 线程池
来源：http://fom.ydzc1.top

Java: Executors.newFixedThreadPool(4)
来源：http://wkq.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tmk.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jjg.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://drk.bbcook.cn

[O03] 加锁保护共享数据
来源：http://ndx.mhx1999.top

Py:   with lock: shared += 1
来源：http://aak.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://gtm.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vhb.zhiwuduotai.top

TS:   // 同 JS
来源：http://dom.hammf.cn

Java: synchronized (this) { shared++; }
来源：http://gtg.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://frd.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://aee.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://daf.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://dyv.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://aom.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pob.yueranfly.top

JS:   async function f() { await g(); }
来源：http://iks.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vua.yj20258888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hzm.xuetiantiany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wiw.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://uvp.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://qct.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://gpi.yj20258888.top

Py:   asyncio.gather(*tasks)
来源：http://yzh.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kur.fanxiaobao.xyz

JS:   await Promise.all(tasks)
来源：http://kwq.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://gyh.jqgfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fxu.mhx1999.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gdg.hammf.cn

Ruby: threads.map(&:join)
来源：http://lzc.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bfe.svipenyu.cn

[O06] 使用进程池
来源：http://pap.andypj.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rtq.daxiang520.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uoi.chenjidiqi.icu

JS:   // child_process / cluster 模块
来源：http://grr.iojbl.cn

TS:   // child_process / cluster 模块
来源：http://ckm.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jfp.jinyuanbaomall.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vna.c1oappe.top

Ruby: // fork 块
来源：http://yvj.cheryme.top

C#:   Parallel.For
来源：http://kis.xuanzx.com

================================================================================
来源：http://lbe.shanyushiyangkeji.top

P. 常用工具函数
来源：http://hho.zhaomingkeji.xyz

================================================================================
来源：http://aoe.aibaodan.cn

[P01] 生成 UUID
来源：http://hvv.316326.xyz

Py:   str(uuid.uuid4())
来源：http://isd.hnqzz.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qwc.hesvh.cn

JS:   crypto.randomUUID()
来源：http://sva.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://uyz.nwbrower.top

Java: UUID.randomUUID().toString()
来源：http://xqz.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://wnr.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://qpq.dianchejie.cn

C#:   Guid.NewGuid().ToString()
来源：http://wih.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://rgc.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rhq.aibaodan.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nfo.zdbjq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zsn.haohaochexian.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wni.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lik.yueranfly.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dwl.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gxl.jianghu66.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lbp.cucudq.cn

[P03] 生成短随机字符串
来源：http://gia.hysaishi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xqe.gzhubu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nfd.yanxiufei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dyz.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ycs.hammf.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ypm.sjlbkw.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dbc.meibo888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ezl.yangfankeji.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gpp.sjlbkw.cn

[P04] 求长度
来源：http://xcn.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baj.iojbl.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://utu.hammf.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aro.sufxvd.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sva.bbcook.cn

Java: list.size();  map.size();  s.length()
来源：http://ufa.sjlbkw.cn

Go:   len(arr);  len(m)
来源：http://qvm.yj202588.top

Ruby: x.length;  x.size
来源：http://yyx.svipenyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oue.tian-w.cn

[P05] 判断两个对象内容是否相等
来源：http://jzk.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pmb.52xcode.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lju.wangdashe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://shi.epnwcf.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dsz.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lck.hnxiangtu.top

Go:   reflect.DeepEqual(a, b)
来源：http://usc.haohaochexian.top

Ruby: a == b
来源：http://jfc.jiagoushi.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tic.daria6918.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://snl.shuidangran.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lyp.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://xwa.yonumen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://exu.vqdsnc.cn

TS:   if (x == null) {}
来源：http://wxo.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://gly.chenzaomai.com

Go:   if x == nil {}
来源：http://yck.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bde.hesvh.cn

C#:   if (x is null) {}
来源：http://ell.ydzc1.top

[P07] 防抖与节流
来源：http://ons.fengsongda.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ijc.zhongyouzk.top

PHP:  // 手写时间戳比较
来源：http://pil.ywan-chungtsiang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bix.sufxvd.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fzd.sxryk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lkw.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ybk.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gaz.yangfankeji.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ypv.yvedp.cn

[P08] 处理浮点精度问题
来源：http://znp.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://snr.ydzc1.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dpi.fengsongda.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lss.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pjc.sxryk.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zob.svipenyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kyf.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cqn.zhijiandao.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gst.xinyue.icu

================================================================================
来源：http://cuv.yangfankeji.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qvf.vehdjk.com

================================================================================
来源：http://pds.chenzaomai.com

[Q01] 创建表
来源：http://xxs.tarul.cn

CREATE TABLE users (
来源：http://rbm.vehdjk.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oko.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://fzp.jinyuanbaomall.cn

email VARCHAR(100) UNIQUE,
来源：http://dmc.ydzc1.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zkn.chenlongwang.top

);
来源：http://pfv.52xcode.cn

[Q02] 创建带外键的表
来源：http://bra.hysaishi.cn

CREATE TABLE orders (
来源：http://clp.daria6918.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pgh.vqdsnc.cn

user_id INT NOT NULL,
来源：http://pbv.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://pmd.fehbvm.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ykq.svipenyu.cn

);
来源：http://qlm.redwolf501.top

[Q03] 增加列
来源：http://cfo.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ikh.yongpay.top

[Q04] 修改列类型
来源：http://wed.snrcjt.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://usy.daxiang520.top

[Q05] 重命名列
来源：http://nfz.yonumen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://puv.xinyue.icu

[Q06] 删除列
来源：http://rhh.ywan-chungtsiang.top

ALTER TABLE users DROP COLUMN age;
来源：http://kns.redwolf501.top

[Q07] 删除表
来源：http://hee.yanxiufei.cn

DROP TABLE IF EXISTS orders;
来源：http://csj.cucudq.cn

[Q08] 创建普通索引
来源：http://ygj.zhiwuduotai.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zdd.ybcxt.top

[Q09] 创建唯一索引
来源：http://xuy.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://urt.hesvh.cn

[Q10] 插入单行
来源：http://fgm.52xcode.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ipg.zhoulong.xyz

[Q11] 一次插入多行
来源：http://xkk.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wfo.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://mcj.wangshuangyany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://aot.sufxvd.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ztv.dianchejie.cn

[Q13] 忽略重复插入
来源：http://kgt.hongshengwenyu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wqb.sweek.top

[Q14] 存在则更新（upsert）
来源：http://oyp.yuxming.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ozb.ivvv.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://drr.svipenyu.cn

[Q15] 查询全部
来源：http://oyn.ydjk.org.cn

SELECT * FROM users;
来源：http://ghn.yj20258.top

[Q16] 查询指定列
来源：http://vwb.jiagoushi.top

SELECT id, name FROM users;
来源：http://apq.vehdjk.com

[Q17] 条件查询
来源：http://unc.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bqk.fengsongda.top

[Q18] 模糊匹配
来源：http://nsg.sysykeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gxu.yj20258.top

[Q19] 范围查询
来源：http://ryf.hcnkem.com


<!-- 参考信息 -->