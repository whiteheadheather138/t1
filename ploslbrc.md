代发 wailian999

[M08] 获取系统与运行时信息
来源：http://gzu.zhijiandao.cn

Py:   platform.system();  platform.python_version()
来源：http://sky.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://cdt.zdqjudy.top

JS:   process.platform;  process.version
来源：http://ykg.ppjwa.cn

TS:   process.platform;  process.version
来源：http://aow.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bmr.yanxiufei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wwz.meibo888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qcu.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://umw.xingfuxueyuan.xyz

================================================================================
来源：http://ekc.zhongyouzk.top

N. 数据结构与算法
来源：http://bbh.andypj.xyz

================================================================================
来源：http://npd.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://gvt.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://olv.xylfe.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://urm.jyoumei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kar.hammf.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wkc.sjlbkw.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jvv.yonumen.top

Go:   sort.SearchInts(arr, x)
来源：http://mip.zhixingplan.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://drb.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pmw.yvedp.cn

[N02] 排序（工程实践用内置实现）
来源：http://uwu.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://uvn.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jtr.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pda.316326.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://vmc.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://srj.yuanzhike.top

Go:   slices.Sort(arr)
来源：http://onk.kuanghao11.cn

Ruby: arr.sort
来源：http://whz.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://iav.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://pil.jinyuanbaomall.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cxc.shzxlz.cn

PHP:  // 递归实现，或用 usort
来源：http://jys.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fzr.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kyl.gotoacloud.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pik.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jfj.ybcxt.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vbl.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://zgs.zhiwuduotai.top

[N04] 斐波那契数列
来源：http://uab.vqdsnc.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wps.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://skw.wangdashe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blm.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rgy.sweek.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fpy.andypj.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hod.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sbl.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://adm.sufxvd.cn

[N05] 最大公约数
来源：http://bot.haohaochexian.top

Py:   math.gcd(a, b)
来源：http://tzw.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jod.hysaishi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vqn.yongpay.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vmu.fktsv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://das.quarkkingdee.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lyg.cashguo.top

Ruby: a.gcd(b)
来源：http://wbu.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aue.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://bgp.ywan-chungtsiang.top

Py:   s == s[::-1]
来源：http://sht.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://tbi.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://wst.zhiwuduotai.top

TS:   s === [...s].reverse().join("")
来源：http://yys.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mgq.xuanzx.com

Go:   // 双指针从两端比较
来源：http://dko.dashuyun.cn

Ruby: s == s.reverse
来源：http://cnh.snrcjt.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cyr.zhixingplan.top

[N07] 两数之和（返回下标）
来源：http://tzn.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zzg.smart0.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jdj.zdbjq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qcb.sweek.top

TS:   // 手写 Map<string, number>
来源：http://oba.cqqwz.cn

Java: // 手写 HashMap
来源：http://uca.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://fgx.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://huz.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hmp.chenlongwang.top

[N08] 生成全排列
来源：http://gnr.ctjpmb.com

Py:   itertools.permutations(arr)
来源：http://gfo.jlsjyb.cn

PHP:  // 手写递归交换
来源：http://fxh.tanke756.top

JS:   // 手写回溯递归
来源：http://jny.vehdjk.com

TS:   // 手写回溯递归
来源：http://hed.hywenlv.cn

Java: // 手写回溯递归
来源：http://zsf.bjfxy.top

Go:   // 手写回溯递归
来源：http://vff.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://rgh.sweek.top

C#:   // 手写回溯递归
来源：http://cue.ctjpmb.com

[N09] 栈与队列
来源：http://msw.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lax.sxryk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fip.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zxg.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lpt.yuxming.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ibd.fehbvm.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tdc.yangfankeji.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fbz.cheryme.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://maq.svipenyu.cn

[N10] 链表节点定义
来源：http://nrh.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lnm.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gjq.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bnn.guannengcc.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mrl.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://dsl.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://ebb.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sou.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dak.daxiang520.top

[N11] 二叉树中序遍历
来源：http://mad.chenlongwang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mye.fzhhl.top

PHP:  // 手写递归函数
来源：http://rsa.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xjy.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bgf.nanxinkj.top

Java: // 手写递归
来源：http://oao.jyoumei.cn

Go:   // 手写递归
来源：http://bix.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jcg.fktsv.cn

C#:   // 手写递归
来源：http://rjz.yueranfly.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xtk.gogol.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zda.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xfq.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sad.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jpr.sweek.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bxy.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ehf.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hsy.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aqw.9152youxi.cn

================================================================================
来源：http://dxe.fengsongda.top

O. 并发与异步
来源：http://dya.hywenlv.cn

================================================================================
来源：http://taj.ybcxt.top

[O01] 启动一个线程
来源：http://spl.andypj.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wwv.feifeiyinyue.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rgq.xuanzx.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jlp.zycfv.cn

TS:   // 同 JS
来源：http://joq.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://ytr.jinqigufen.top

Go:   go f()
来源：http://zav.mhx1999.top

Ruby: Thread.new { f }
来源：http://ers.epnwcf.com

C#:   Task.Run(() => F());
来源：http://yho.aizwys.cn

[O02] 使用线程池
来源：http://pum.feifeiyinyue.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cez.sufxvd.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uyh.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://ths.zycfv.cn

TS:   // worker_threads 线程池
来源：http://dtx.jinyuanbaomall.cn

Java: Executors.newFixedThreadPool(4)
来源：http://efq.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tpp.nwbrower.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jbr.birdmap.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xab.tanke756.top

[O03] 加锁保护共享数据
来源：http://zlb.feifeiyinyue.top

Py:   with lock: shared += 1
来源：http://kqt.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://oqq.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lus.shangyingyoupin.top

TS:   // 同 JS
来源：http://vmh.ydzc1.top

Java: synchronized (this) { shared++; }
来源：http://lqg.hesvh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ucq.aizwys.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rqo.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://xfz.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://hpj.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://mcq.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://trj.xuanzx.com

JS:   async function f() { await g(); }
来源：http://llh.bjfxy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://odw.wangdashe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ijr.xinyue.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zqt.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ocd.guannengcc.top

C#:   async Task F() { await G(); }
来源：http://nma.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://jos.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://gtn.zhiwuduotai.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nnj.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://vtd.kuanghao11.cn

TS:   await Promise.all(tasks)
来源：http://xak.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zlt.ehwqpu.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://igk.uphjek.com

Ruby: threads.map(&:join)
来源：http://xsh.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ecz.pengpengdd.cyou

[O06] 使用进程池
来源：http://asu.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ykw.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://heo.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://rqj.sweek.top

TS:   // child_process / cluster 模块
来源：http://fns.fzhhl.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wfy.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rox.shanyushiyangkeji.top

Ruby: // fork 块
来源：http://zll.cucudq.cn

C#:   Parallel.For
来源：http://juj.yueranfly.top

================================================================================
来源：http://qce.nanxinkj.top

P. 常用工具函数
来源：http://dvo.gzhubu.top

================================================================================
来源：http://gpq.sweek.top

[P01] 生成 UUID
来源：http://wla.smart0.xyz

Py:   str(uuid.uuid4())
来源：http://tdn.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nzz.yj20258888.top

JS:   crypto.randomUUID()
来源：http://ouk.quarkkingdee.top

TS:   crypto.randomUUID()
来源：http://lnh.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://ybt.hesvh.cn

Go:   // 用 github.com/google/uuid
来源：http://mcw.shangyingyoupin.top

Ruby: SecureRandom.uuid
来源：http://uei.shzxlz.cn

C#:   Guid.NewGuid().ToString()
来源：http://euh.cashguo.top

[P02] MD5 / SHA256 摘要
来源：http://cfz.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rwe.wangdashe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dmy.yj20258.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dsd.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vgn.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rqe.tian-w.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lnv.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mkd.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ofl.epnwcf.com

[P03] 生成短随机字符串
来源：http://fig.zhengqikj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bpm.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eec.hnxiangtu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mvg.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jvl.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ejl.nanxuanxn.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jhm.jinqigufen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ogs.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aqf.yj20258.top

[P04] 求长度
来源：http://sew.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ftt.hnxiangtu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dab.nwbrower.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ytw.yfazqb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hnz.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://dbo.gzhubu.top

Go:   len(arr);  len(m)
来源：http://klj.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://psd.jiagoushi.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zrh.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://jyr.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://miv.jqgfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dks.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://krw.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lzn.ivvv.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hzn.yanxiufei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kfl.zycfv.cn

Ruby: a == b
来源：http://ojb.hfpthk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://doo.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lze.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kew.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://bfu.sjlbkw.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zyz.ydzc1.top

TS:   if (x == null) {}
来源：http://ykv.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://tcc.jlsjyb.cn

Go:   if x == nil {}
来源：http://dxx.gzhubu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kte.chenzaomai.com

C#:   if (x is null) {}
来源：http://ege.hnqzz.top

[P07] 防抖与节流
来源：http://jwq.0kj1m.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rnc.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://qqg.xziqi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fxc.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://apb.yj202588.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tbz.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://abt.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qzr.fehbvm.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ytm.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://mfi.kuanghao11.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gxp.shanyushiyangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zjy.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zpq.svipenyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://stc.cashguo.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mwz.tarul.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nzw.tarul.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ojy.tarul.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hkl.316326.xyz

================================================================================
来源：http://ybe.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jgg.316326.xyz

================================================================================
来源：http://rjv.vqdsnc.cn

[Q01] 创建表
来源：http://sqv.daria6918.cn

CREATE TABLE users (
来源：http://mvq.yvedp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ing.hnqzz.top

name VARCHAR(50) NOT NULL,
来源：http://wlc.iojbl.cn

email VARCHAR(100) UNIQUE,
来源：http://xwg.sysykeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jan.jyoumei.cn

);
来源：http://qoe.cheryme.top

[Q02] 创建带外键的表
来源：http://vqr.sufxvd.cn

CREATE TABLE orders (
来源：http://iht.quarkkingdee.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wen.aizwys.cn

user_id INT NOT NULL,
来源：http://zay.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://rub.jinqigfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hop.gzhubu.top

);
来源：http://anu.shzxlz.cn

[Q03] 增加列
来源：http://rgh.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://owa.hfpthk.cn

[Q04] 修改列类型
来源：http://lhh.xingfuxueyuan.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wht.snrcjt.cn

[Q05] 重命名列
来源：http://gnx.birdmap.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pim.guannengcc.top

[Q06] 删除列
来源：http://jil.ydjk.org.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kli.nanxinkj.top

[Q07] 删除表
来源：http://plg.hysaishi.cn

DROP TABLE IF EXISTS orders;
来源：http://emy.quarkkingdee.top

[Q08] 创建普通索引
来源：http://jer.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kyr.tarul.cn

[Q09] 创建唯一索引
来源：http://vyq.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uaa.316326.xyz

[Q10] 插入单行
来源：http://cgm.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ust.zhixingplan.top

[Q11] 一次插入多行
来源：http://wdg.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ixq.dianchejie.cn

[Q12] 插入后取自增 ID
来源：http://ctb.andypj.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://qel.dashuyun.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://twv.xuanzx.com

[Q13] 忽略重复插入
来源：http://xwc.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rpz.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://knl.snrcjt.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rah.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fke.chenjidiqi.icu

[Q15] 查询全部
来源：http://apn.snrcjt.cn

SELECT * FROM users;
来源：http://ugk.yanxiufei.cn

[Q16] 查询指定列
来源：http://iwj.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://whz.0kj1m.cn

[Q17] 条件查询
来源：http://icp.hnqzz.top


<!-- 参考信息 -->