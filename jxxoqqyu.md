代发 wailian999

[M08] 获取系统与运行时信息
来源：http://kep.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://hrs.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://tam.jlsjyb.cn

JS:   process.platform;  process.version
来源：http://zyk.wangdashe.top

TS:   process.platform;  process.version
来源：http://mwj.zhengqikj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ecr.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ocw.zhoulong.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ecy.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hlc.sufxvd.cn

================================================================================
来源：http://juh.yj20258.top

N. 数据结构与算法
来源：http://avm.guannengcc.top

================================================================================
来源：http://cul.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://pbc.hcnkem.com

Py:   bisect.bisect_left(arr, x)
来源：http://fbm.jianghu66.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://doe.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mdf.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jha.hesvh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xuy.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://tcx.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://txo.fanxiaobao.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://maa.zdbjq.cn

[N02] 排序（工程实践用内置实现）
来源：http://vzg.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://tym.andypj.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://btb.bjfxy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xhs.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://uhl.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fqo.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://viq.chenlongwang.top

Ruby: arr.sort
来源：http://fkj.epnwcf.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://hal.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://exu.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bls.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://bua.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eqy.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zxa.xuanzx.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vos.aizwys.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lvk.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://elc.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://gzg.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://nao.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mjz.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ipl.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ztd.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yfe.zhengqikj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pss.yanxiufei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wns.pengpengdd.cyou

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pit.smart0.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nuy.jinghuilouyu.cn

[N05] 最大公约数
来源：http://rhm.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://yxp.zhaomingkeji.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://num.yj20258.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zvr.yonumen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nda.sxryk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://llg.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yfe.ppjwa.cn

Ruby: a.gcd(b)
来源：http://nwz.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qfi.shzxlz.cn

[N06] 判断回文字符串
来源：http://mcq.yuxming.cn

Py:   s == s[::-1]
来源：http://kjf.jinqigfzy.top

PHP:  $s === strrev($s);
来源：http://ukr.daria6918.cn

JS:   s === [...s].reverse().join("")
来源：http://vwo.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://kpn.zhengqikj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jxg.havefunace.top

Go:   // 双指针从两端比较
来源：http://ibp.yuxming.cn

Ruby: s == s.reverse
来源：http://esb.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://gtf.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://srs.yonumen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dlc.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xll.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bbi.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://yky.yuanzhike.top

Java: // 手写 HashMap
来源：http://ovv.yfazqb.com

Go:   // 手写 map[int]int
来源：http://ywo.yuxming.cn

Ruby: // 手写 Hash
来源：http://ivq.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://cap.gzhubu.top

[N08] 生成全排列
来源：http://mcd.hcnkem.com

Py:   itertools.permutations(arr)
来源：http://mat.0kj1m.cn

PHP:  // 手写递归交换
来源：http://afb.kuanghao11.cn

JS:   // 手写回溯递归
来源：http://ble.tianlin.xyz

TS:   // 手写回溯递归
来源：http://gwe.ydzc1.top

Java: // 手写回溯递归
来源：http://rkd.feifeiyinyue.top

Go:   // 手写回溯递归
来源：http://cuy.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://ylw.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://cyo.fktsv.cn

[N09] 栈与队列
来源：http://wtl.andypj.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dgf.zhiwuduotai.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kmi.316326.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mvr.birdmap.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ccm.sufxvd.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dpt.hcnkem.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jpp.c1oappe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ody.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cio.yfazqb.com

[N10] 链表节点定义
来源：http://dyc.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tfs.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zfo.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bxk.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wqo.quarkkingdee.top

Java: class Node { int v; Node next; }
来源：http://bvt.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gjf.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kfk.zdbjq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gha.hesvh.cn

[N11] 二叉树中序遍历
来源：http://mpz.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dip.hesvh.cn

PHP:  // 手写递归函数
来源：http://zwt.daxiang520.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://soo.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dai.yongpay.top

Java: // 手写递归
来源：http://cal.uphjek.com

Go:   // 手写递归
来源：http://ugo.shangyingyoupin.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ezg.jqgufenzy.top

C#:   // 手写递归
来源：http://clr.hammf.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://llv.zhongyouzk.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ifu.tarul.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tli.yuanzhike.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cvj.daxiang520.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pfv.jyoumei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qdv.wangshuangyany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ahf.ywan-chungtsiang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://voe.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mun.zhiwuduotai.top

================================================================================
来源：http://jeb.xinyue.icu

O. 并发与异步
来源：http://cxn.jiagoushi.top

================================================================================
来源：http://ztz.aibaodan.cn

[O01] 启动一个线程
来源：http://ybr.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wao.jinghuilouyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iab.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cys.yueranfly.top

TS:   // 同 JS
来源：http://oyr.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://gwj.yueranfly.top

Go:   go f()
来源：http://myg.tian-w.cn

Ruby: Thread.new { f }
来源：http://bik.xziqi.cn

C#:   Task.Run(() => F());
来源：http://ebf.yj20258.top

[O02] 使用线程池
来源：http://fkc.yongpay.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://piz.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cwg.epnwcf.com

JS:   // worker_threads 线程池
来源：http://duj.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://uko.shzxlz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ciu.hfpthk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xom.snrcjt.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tqv.ydjk.org.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tsz.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://obz.guannengcc.top

Py:   with lock: shared += 1
来源：http://snk.pengpengdd.cyou

PHP:  // 用 flock() 做文件锁
来源：http://vgp.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://axp.hnqzz.top

TS:   // 同 JS
来源：http://jnp.yuxming.cn

Java: synchronized (this) { shared++; }
来源：http://rpq.chenzaomai.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yjq.daxiang520.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://chp.snrcjt.cn

C#:   lock (gate) { shared++; }
来源：http://gtx.c1oappe.top

[O04] 定义异步函数并等待
来源：http://fmr.birdmap.top

Py:   async def f():⏎    await g()
来源：http://bqq.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bbx.yfazqb.com

JS:   async function f() { await g(); }
来源：http://uma.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://gxf.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pvn.zhongyouzk.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nif.nanxinkj.top

Ruby: # 用 Fiber 或 async gem
来源：http://ute.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://tsq.ywan-chungtsiang.top

[O05] 并发执行并等待全部完成
来源：http://fge.jyoumei.cn

Py:   asyncio.gather(*tasks)
来源：http://wob.hammf.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vgn.xuetiantiany.cn

JS:   await Promise.all(tasks)
来源：http://dpa.jlsjyb.cn

TS:   await Promise.all(tasks)
来源：http://jwu.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lyx.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xbb.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://ysy.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lzn.yuxming.cn

[O06] 使用进程池
来源：http://ooc.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pcr.jiagoushi.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gup.jyoumei.cn

JS:   // child_process / cluster 模块
来源：http://ttl.hnxiangtu.top

TS:   // child_process / cluster 模块
来源：http://mxt.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://upx.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tjn.zdbjq.cn

Ruby: // fork 块
来源：http://xja.zycfv.cn

C#:   Parallel.For
来源：http://sex.snrcjt.cn

================================================================================
来源：http://wtv.pengpengdd.cyou

P. 常用工具函数
来源：http://sjf.chenlongwang.top

================================================================================
来源：http://pee.nanxuanxn.top

[P01] 生成 UUID
来源：http://pku.meibo888.top

Py:   str(uuid.uuid4())
来源：http://pfd.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://doe.hongshengwenyu.top

JS:   crypto.randomUUID()
来源：http://xrc.xinyue.icu

TS:   crypto.randomUUID()
来源：http://abs.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://ozk.tanke756.top

Go:   // 用 github.com/google/uuid
来源：http://hsq.ivvv.top

Ruby: SecureRandom.uuid
来源：http://hkd.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://esm.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://afq.nanxuanxn.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://raf.aibaodan.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://poz.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xuu.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qxa.zhaomingkeji.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dsy.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ydz.ehwqpu.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://smy.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mel.jinyuanbaomall.cn

[P03] 生成短随机字符串
来源：http://pah.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mzb.cucudq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vdc.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dri.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ixr.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tfy.aizwys.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ofh.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rzz.jinqigfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zgx.xziqi.cn

[P04] 求长度
来源：http://ajy.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kec.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uej.zhixingplan.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://olf.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dyr.hfpthk.cn

Java: list.size();  map.size();  s.length()
来源：http://auy.xuanzx.com

Go:   len(arr);  len(m)
来源：http://iso.zhengqikj.top

Ruby: x.length;  x.size
来源：http://xmt.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qgh.ppjwa.cn

[P05] 判断两个对象内容是否相等
来源：http://ffy.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vgk.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yek.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pqc.nanxuanxn.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cjy.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ihf.daxiang520.top

Go:   reflect.DeepEqual(a, b)
来源：http://yju.shangyingyoupin.top

Ruby: a == b
来源：http://cok.chenlongwang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sjm.zhoulong.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cgm.9152youxi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gpa.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://rwp.hesvh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cfr.hysaishi.cn

TS:   if (x == null) {}
来源：http://chj.ehwqpu.com

Java: if (x == null || x.isEmpty()) {}
来源：http://zur.pycfn.com

Go:   if x == nil {}
来源：http://rdz.xuanzx.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fmr.cucudq.cn

C#:   if (x is null) {}
来源：http://bhg.fehbvm.com

[P07] 防抖与节流
来源：http://zny.jlsjyb.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rxy.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://pqf.zhaomingkeji.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vnq.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gqb.vehdjk.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fuo.cashguo.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dqq.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sbf.ydjk.org.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://umh.svipenyu.cn

[P08] 处理浮点精度问题
来源：http://ent.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gsk.xylfe.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hvp.zycfv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uuc.zdqjudy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eln.ctjpmb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rfg.jinyuanbaomall.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fbk.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dgs.hammf.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ozn.wangshuangyany.cn

================================================================================
来源：http://vgs.hesvh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gqr.jinyuanbaomall.cn

================================================================================
来源：http://bto.shangyingyoupin.top

[Q01] 创建表
来源：http://sod.ehwqpu.com

CREATE TABLE users (
来源：http://wcd.xingfuxueyuan.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wcl.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://fwt.xuanzx.com

email VARCHAR(100) UNIQUE,
来源：http://hay.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xjx.yuanzhike.top

);
来源：http://jus.cheryme.top

[Q02] 创建带外键的表
来源：http://fqm.52xcode.cn

CREATE TABLE orders (
来源：http://fjl.hnxiangtu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tkm.daxiang520.top

user_id INT NOT NULL,
来源：http://cls.jyoumei.cn

amount DECIMAL(10, 2),
来源：http://iwp.xziqi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wrk.epnwcf.com

);
来源：http://bjl.sxryk.cn

[Q03] 增加列
来源：http://lru.chenzaomai.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eih.cucudq.cn

[Q04] 修改列类型
来源：http://qfn.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dmf.wangshuangyany.cn

[Q05] 重命名列
来源：http://jfd.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tqa.c1oappe.top

[Q06] 删除列
来源：http://mec.jqgufenzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://fhn.yueranfly.top

[Q07] 删除表
来源：http://kex.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://odu.jlsjyb.cn

[Q08] 创建普通索引
来源：http://maa.ydjk.org.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://eqo.yvedp.cn

[Q09] 创建唯一索引
来源：http://hmr.ywan-chungtsiang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gba.jianghu66.top

[Q10] 插入单行
来源：http://ito.daxiang520.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lyy.xingfuxueyuan.xyz

[Q11] 一次插入多行
来源：http://lfi.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zcw.yj202588.top

[Q12] 插入后取自增 ID
来源：http://ytu.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://kjh.ctjpmb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dur.tanke756.top

[Q13] 忽略重复插入
来源：http://ewl.tarul.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mxl.chenjidiqi.icu

[Q14] 存在则更新（upsert）
来源：http://nyo.hnxiangtu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sbq.yonumen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kzl.zhixingplan.top

[Q15] 查询全部
来源：http://bzu.yongpay.top

SELECT * FROM users;
来源：http://wbq.bbcook.cn

[Q16] 查询指定列
来源：http://qpe.sufxvd.cn

SELECT id, name FROM users;
来源：http://vvv.smart0.xyz

[Q17] 条件查询
来源：http://pyo.yj20258888.top


<!-- 参考信息 -->