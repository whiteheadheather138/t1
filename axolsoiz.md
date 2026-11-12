代发 wailian999

TS:   process.platform;  process.version
来源：http://kbu.shangyingyoupin.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ncs.fktsv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ytk.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hqw.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jkv.mhx1999.top

================================================================================
来源：http://fin.cqqwz.cn

N. 数据结构与算法
来源：http://sqh.meibo888.top

================================================================================
来源：http://skm.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://npe.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://gnv.feifeiyinyue.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://saj.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://res.gotoacloud.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lar.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://aqj.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://lue.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xej.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://ovd.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://icx.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://rbw.xingfuxueyuan.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nss.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://bnm.hywenlv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://igq.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ojr.cheryme.top

Go:   slices.Sort(arr)
来源：http://tsz.fzhhl.top

Ruby: arr.sort
来源：http://dor.andypj.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://gtl.hongshengwenyu.top

[N03] 快速排序（分治示例）
来源：http://pcf.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lnw.chenjidiqi.icu

PHP:  // 递归实现，或用 usort
来源：http://wnv.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nde.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://the.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ffo.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pyb.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lga.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bza.aibaodan.cn

[N04] 斐波那契数列
来源：http://xqo.xuanzx.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rso.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tvy.jinqigufen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vwb.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qor.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xfc.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gcw.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://guc.jianghu66.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://luu.cheryme.top

[N05] 最大公约数
来源：http://fia.jlsjyb.cn

Py:   math.gcd(a, b)
来源：http://ils.fktsv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bmh.dianchejie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qtq.cdnleiting.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jbp.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ybn.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ezw.sufxvd.cn

Ruby: a.gcd(b)
来源：http://nxa.hnqzz.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vqh.0kj1m.cn

[N06] 判断回文字符串
来源：http://kmm.xinyue.icu

Py:   s == s[::-1]
来源：http://goh.sxryk.cn

PHP:  $s === strrev($s);
来源：http://bct.vqdsnc.cn

JS:   s === [...s].reverse().join("")
来源：http://jlf.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://sol.dianchejie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yvf.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://did.wangdashe.top

Ruby: s == s.reverse
来源：http://iit.yj20258.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ssh.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://zsv.mhx1999.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zyo.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mhz.iojbl.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://feq.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://xao.hywenlv.cn

Java: // 手写 HashMap
来源：http://ari.xuanzx.com

Go:   // 手写 map[int]int
来源：http://ery.fehbvm.com

Ruby: // 手写 Hash
来源：http://kbx.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://dhp.svipenyu.cn

[N08] 生成全排列
来源：http://hqg.hammf.cn

Py:   itertools.permutations(arr)
来源：http://rjg.gogol.net.cn

PHP:  // 手写递归交换
来源：http://zyq.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://iln.yonumen.top

TS:   // 手写回溯递归
来源：http://xin.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://bvs.zhiwuduotai.top

Go:   // 手写回溯递归
来源：http://ncq.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://aya.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://hjq.redwolf501.top

[N09] 栈与队列
来源：http://wez.cqqwz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ted.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hyi.fanxiaobao.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://irx.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://muh.hywenlv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kir.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sch.yj20258.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://szz.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kaj.fanxiaobao.xyz

[N10] 链表节点定义
来源：http://bvt.shangyingyoupin.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://alr.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bag.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oft.hnqzz.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bpi.yangfankeji.com

Java: class Node { int v; Node next; }
来源：http://cxx.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://xsl.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://shm.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://aaw.birdmap.top

[N11] 二叉树中序遍历
来源：http://lom.tanke756.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yom.0kj1m.cn

PHP:  // 手写递归函数
来源：http://ozj.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fno.yueranfly.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vsc.svipenyu.cn

Java: // 手写递归
来源：http://hxv.jinyuanbaomall.cn

Go:   // 手写递归
来源：http://svu.tanke756.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bmj.yangfankeji.com

C#:   // 手写递归
来源：http://hck.xylfe.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wdx.vqdsnc.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xnl.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://asr.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vth.fanxiaobao.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jgs.zhijiandao.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nur.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qrk.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vfj.gogol.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lzw.zhoulong.xyz

================================================================================
来源：http://ipr.nanxinkj.top

O. 并发与异步
来源：http://wrw.pycfn.com

================================================================================
来源：http://fjq.yj20258.top

[O01] 启动一个线程
来源：http://jkx.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://emv.0kj1m.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xff.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://osa.daxiang520.top

TS:   // 同 JS
来源：http://pnx.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://ags.xylfe.cn

Go:   go f()
来源：http://fui.cheryme.top

Ruby: Thread.new { f }
来源：http://jgm.fktsv.cn

C#:   Task.Run(() => F());
来源：http://cpm.fehbvm.com

[O02] 使用线程池
来源：http://qnp.chenlongwang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kdm.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dlo.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://zow.xuanzx.com

TS:   // worker_threads 线程池
来源：http://loc.zhoulong.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://tvh.yfazqb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qog.hnxiangtu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bke.316326.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://apc.316326.xyz

[O03] 加锁保护共享数据
来源：http://yym.cucudq.cn

Py:   with lock: shared += 1
来源：http://dsn.hfpthk.cn

PHP:  // 用 flock() 做文件锁
来源：http://qbo.hongshengwenyu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pdo.sysykeji.top

TS:   // 同 JS
来源：http://zmr.wangdashe.top

Java: synchronized (this) { shared++; }
来源：http://kje.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xff.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hxk.nwbrower.top

C#:   lock (gate) { shared++; }
来源：http://yvp.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://dog.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://xvt.dashuyun.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zmz.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://xlz.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ifn.gzhubu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jyx.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ozu.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://gyq.hongshengwenyu.top

C#:   async Task F() { await G(); }
来源：http://tlq.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://vwr.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://rbp.zhaomingkeji.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jeq.fehbvm.com

JS:   await Promise.all(tasks)
来源：http://esv.ctjpmb.com

TS:   await Promise.all(tasks)
来源：http://mhq.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://npb.0kj1m.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jzg.iojbl.cn

Ruby: threads.map(&:join)
来源：http://suv.hongshengwenyu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vqf.sweek.top

[O06] 使用进程池
来源：http://vdt.sysykeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rig.zhijiandao.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://iqe.52xcode.cn

JS:   // child_process / cluster 模块
来源：http://zdf.ehwqpu.com

TS:   // child_process / cluster 模块
来源：http://ulh.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vvr.hfpthk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://spo.yuxming.cn

Ruby: // fork 块
来源：http://kei.gotoacloud.top

C#:   Parallel.For
来源：http://ziy.shanyushiyangtech.top

================================================================================
来源：http://dkr.fengsongda.top

P. 常用工具函数
来源：http://exr.zhongyouzk.top

================================================================================
来源：http://uvc.jiagoushi.top

[P01] 生成 UUID
来源：http://ptg.shangyingyoupin.top

Py:   str(uuid.uuid4())
来源：http://bko.yj20258888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://epj.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://lnp.yueranfly.top

TS:   crypto.randomUUID()
来源：http://tfb.zycfv.cn

Java: UUID.randomUUID().toString()
来源：http://hkx.c1oappe.top

Go:   // 用 github.com/google/uuid
来源：http://ewp.chenlongwang.top

Ruby: SecureRandom.uuid
来源：http://mdc.zhoulong.xyz

C#:   Guid.NewGuid().ToString()
来源：http://rew.zdqjudy.top

[P02] MD5 / SHA256 摘要
来源：http://rua.zhijiandao.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sbv.cheryme.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sfm.uphjek.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cvv.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hwd.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://juq.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uav.316326.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jqz.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mtk.bbcook.cn

[P03] 生成短随机字符串
来源：http://smo.jqgufenzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hsm.cashguo.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ojx.sufxvd.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pos.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ori.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xfn.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zyr.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sfn.tarul.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wsu.zhaomingkeji.xyz

[P04] 求长度
来源：http://ygt.hysaishi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pit.shanyushiyangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ibu.havefunace.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gji.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dri.chenzaomai.com

Java: list.size();  map.size();  s.length()
来源：http://pkn.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://tti.ydjk.org.cn

Ruby: x.length;  x.size
来源：http://ibn.jyoumei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ezs.aizwys.cn

[P05] 判断两个对象内容是否相等
来源：http://nem.quarkkingdee.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://aym.ppjwa.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tnd.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jqv.yangfankeji.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tkx.yvedp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://inr.tanke756.top

Go:   reflect.DeepEqual(a, b)
来源：http://yku.cheryme.top

Ruby: a == b
来源：http://qdf.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jiw.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yrv.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://snk.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://jxa.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bsv.gzhubu.top

TS:   if (x == null) {}
来源：http://ouv.chenzaomai.com

Java: if (x == null || x.isEmpty()) {}
来源：http://tmz.ehwqpu.com

Go:   if x == nil {}
来源：http://cam.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://phe.fengsongda.top

C#:   if (x is null) {}
来源：http://wcl.hfpthk.cn

[P07] 防抖与节流
来源：http://brz.zycfv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rtj.zhijiandao.cn

PHP:  // 手写时间戳比较
来源：http://jri.dianchejie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qna.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cil.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://syc.fanxiaobao.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ley.9152youxi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://iyi.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nof.316326.xyz

[P08] 处理浮点精度问题
来源：http://yki.yangfankeji.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://shj.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dms.zhiwuduotai.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dej.xylfe.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qxp.epnwcf.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cxu.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rbx.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sti.gotoacloud.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vvs.daxiang520.top

================================================================================
来源：http://gay.chenlongwang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cjm.gaohongyu789.top

================================================================================
来源：http://ttv.cashguo.top

[Q01] 创建表
来源：http://fjn.zhoulong.xyz

CREATE TABLE users (
来源：http://sen.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nxu.dashuyun.cn

name VARCHAR(50) NOT NULL,
来源：http://lty.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://okh.fehbvm.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bsg.316326.xyz

);
来源：http://ryr.zdqjudy.top

[Q02] 创建带外键的表
来源：http://hjm.xuetiantiany.cn

CREATE TABLE orders (
来源：http://ols.haohaochexian.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uyx.zhaomingkeji.xyz

user_id INT NOT NULL,
来源：http://xvg.svipenyu.cn

amount DECIMAL(10, 2),
来源：http://cir.xuanzx.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jcm.sufxvd.cn

);
来源：http://ugz.ydjk.org.cn

[Q03] 增加列
来源：http://egv.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nhl.chenjidiqi.icu

[Q04] 修改列类型
来源：http://naj.cashguo.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gfq.zhaomingkeji.xyz

[Q05] 重命名列
来源：http://cmx.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hjx.uphjek.com

[Q06] 删除列
来源：http://oda.yj202588.top

ALTER TABLE users DROP COLUMN age;
来源：http://hha.jqgfzy.top

[Q07] 删除表
来源：http://rwe.yj20258888.top

DROP TABLE IF EXISTS orders;
来源：http://arb.fengsongda.top

[Q08] 创建普通索引
来源：http://wed.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://leq.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://xcm.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dgm.jlsjyb.cn

[Q10] 插入单行
来源：http://rij.hysaishi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vyc.ppjwa.cn

[Q11] 一次插入多行
来源：http://wmn.cdnleiting.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://grd.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://fnr.jyoumei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wei.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gaw.52xcode.cn

[Q13] 忽略重复插入
来源：http://fon.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gkw.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://cqx.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kpc.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pvp.zhiwuduotai.top

[Q15] 查询全部
来源：http://yel.smart0.xyz

SELECT * FROM users;
来源：http://qjq.yuxming.cn

[Q16] 查询指定列
来源：http://bfe.ppjwa.cn

SELECT id, name FROM users;
来源：http://nyz.svipenyu.cn

[Q17] 条件查询
来源：http://cxc.sufxvd.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lxo.pengpengdd.cyou

[Q18] 模糊匹配
来源：http://vxw.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pkh.jianghu66.top

[Q19] 范围查询
来源：http://yvl.fehbvm.com


<!-- 参考信息 -->