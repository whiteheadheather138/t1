代发 wailian999

TS:   process.platform;  process.version
来源：http://kmr.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gcg.ydzc1.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jla.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hhv.fktsv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://drk.zdbjq.cn

================================================================================
来源：http://wak.vehdjk.com

N. 数据结构与算法
来源：http://mdp.hnxiangtu.top

================================================================================
来源：http://dgl.uphjek.com

[N01] 二分查找（有序数组）
来源：http://rzr.zhiwuduotai.top

Py:   bisect.bisect_left(arr, x)
来源：http://jzj.ehwqpu.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sgt.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rly.cheryme.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ysn.shanyushiyangtech.top

Java: Arrays.binarySearch(arr, x)
来源：http://mwa.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://woo.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ngi.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tsv.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://zgh.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://gpa.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ayl.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rox.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rdp.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xxs.yvedp.cn

Go:   slices.Sort(arr)
来源：http://phj.chenjidiqi.icu

Ruby: arr.sort
来源：http://bsy.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://clr.yj202588.top

[N03] 快速排序（分治示例）
来源：http://cnf.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lgp.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://pba.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xdc.feifeiyinyue.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vhy.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zat.feifeiyinyue.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kgr.chenjidiqi.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tly.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://aqf.sweek.top

[N04] 斐波那契数列
来源：http://tqv.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wtl.pycfn.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nel.chenlongwang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ger.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hbq.aibaodan.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pmq.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://noq.jlsjyb.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://amf.fanxiaobao.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gwq.yj20258888.top

[N05] 最大公约数
来源：http://eel.zhongyouzk.top

Py:   math.gcd(a, b)
来源：http://epv.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ezc.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qhs.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bwy.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mvt.smart0.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ygp.hammf.cn

Ruby: a.gcd(b)
来源：http://xxk.zhixingplan.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ryk.jqgfzy.top

[N06] 判断回文字符串
来源：http://svb.zdbjq.cn

Py:   s == s[::-1]
来源：http://udt.yj20258.top

PHP:  $s === strrev($s);
来源：http://zds.cucudq.cn

JS:   s === [...s].reverse().join("")
来源：http://ftb.pengpengdd.cyou

TS:   s === [...s].reverse().join("")
来源：http://qdt.xylfe.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://smr.fehbvm.com

Go:   // 双指针从两端比较
来源：http://kgt.sufxvd.cn

Ruby: s == s.reverse
来源：http://daa.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cgz.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://lce.gogol.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vws.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hjr.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://wqh.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://hzh.jianghu66.top

Java: // 手写 HashMap
来源：http://xwf.ybcxt.top

Go:   // 手写 map[int]int
来源：http://omj.xylfe.cn

Ruby: // 手写 Hash
来源：http://umg.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://lwn.zycfv.cn

[N08] 生成全排列
来源：http://fap.yj202588.top

Py:   itertools.permutations(arr)
来源：http://lgj.xziqi.cn

PHP:  // 手写递归交换
来源：http://ujw.cucudq.cn

JS:   // 手写回溯递归
来源：http://fli.yanxiufei.cn

TS:   // 手写回溯递归
来源：http://xbq.cheryme.top

Java: // 手写回溯递归
来源：http://mrl.mhx1999.top

Go:   // 手写回溯递归
来源：http://ecd.316326.xyz

Ruby: arr.permutation.to_a
来源：http://qvz.svipenyu.cn

C#:   // 手写回溯递归
来源：http://uhr.hnqzz.top

[N09] 栈与队列
来源：http://rju.ydzc1.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nze.wangdashe.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tkk.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lti.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sit.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oyl.shangyingyoupin.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zco.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cmh.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bwi.hfpthk.cn

[N10] 链表节点定义
来源：http://sbu.shanyushiyangtech.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xzv.svipenyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ltm.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ahj.cashguo.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nir.mhx1999.top

Java: class Node { int v; Node next; }
来源：http://xlv.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vqe.wangshuangyany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gmc.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sqy.zhiwuduotai.top

[N11] 二叉树中序遍历
来源：http://cyi.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://twr.fanxiaobao.xyz

PHP:  // 手写递归函数
来源：http://sja.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lth.tian-w.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://esy.hywenlv.cn

Java: // 手写递归
来源：http://xmc.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://plx.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ahy.gzhubu.top

C#:   // 手写递归
来源：http://kux.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://osx.yj20258888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rfh.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://btf.fzhhl.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dpo.yongpay.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fab.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://chn.yonumen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sqn.hfpthk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cul.jinyuanbaomall.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kay.zhoulong.xyz

================================================================================
来源：http://gem.wangdashe.top

O. 并发与异步
来源：http://wak.dianchejie.cn

================================================================================
来源：http://aaf.cucudq.cn

[O01] 启动一个线程
来源：http://bba.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cke.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hue.yuxming.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rcb.zhengqikj.top

TS:   // 同 JS
来源：http://vgz.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://gmw.yueranfly.top

Go:   go f()
来源：http://psq.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://riz.smart0.xyz

C#:   Task.Run(() => F());
来源：http://dro.sjlbkw.cn

[O02] 使用线程池
来源：http://dfr.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rdd.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ijb.zdqjudy.top

JS:   // worker_threads 线程池
来源：http://zzg.zhaomingkeji.xyz

TS:   // worker_threads 线程池
来源：http://jux.birdmap.top

Java: Executors.newFixedThreadPool(4)
来源：http://ihk.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bjz.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yib.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qga.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://zug.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://iqk.sysykeji.top

PHP:  // 用 flock() 做文件锁
来源：http://dzf.chenlongwang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fnv.yongpay.top

TS:   // 同 JS
来源：http://caa.jinyuanbaomall.cn

Java: synchronized (this) { shared++; }
来源：http://mgu.cheryme.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xcv.yueranfly.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eut.tanke756.top

C#:   lock (gate) { shared++; }
来源：http://cjn.pycfn.com

[O04] 定义异步函数并等待
来源：http://zqx.sweek.top

Py:   async def f():⏎    await g()
来源：http://muc.zhoulong.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wcs.tarul.cn

JS:   async function f() { await g(); }
来源：http://ein.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ued.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://geu.hammf.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ipk.jianghu66.top

Ruby: # 用 Fiber 或 async gem
来源：http://ebg.pycfn.com

C#:   async Task F() { await G(); }
来源：http://qmk.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://epq.cdnleiting.top

Py:   asyncio.gather(*tasks)
来源：http://cqr.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vro.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://xvt.chenlongwang.top

TS:   await Promise.all(tasks)
来源：http://ail.feifeiyinyue.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qza.daxiang520.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vcg.bjfxy.top

Ruby: threads.map(&:join)
来源：http://wtw.hcnkem.com

C#:   await Task.WhenAll(t1, t2)
来源：http://yhy.jinyuanbaomall.cn

[O06] 使用进程池
来源：http://rce.zhixingplan.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rmw.uphjek.com

PHP:  // pcntl_fork 或多进程队列
来源：http://jke.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://vyn.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://rce.ydjk.org.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://olk.sysykeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kqx.ydzc1.top

Ruby: // fork 块
来源：http://uzb.fengsongda.top

C#:   Parallel.For
来源：http://nxo.cqqwz.cn

================================================================================
来源：http://olr.dashuyun.cn

P. 常用工具函数
来源：http://tqh.epnwcf.com

================================================================================
来源：http://xot.redwolf501.top

[P01] 生成 UUID
来源：http://msa.jinyuanbaomall.cn

Py:   str(uuid.uuid4())
来源：http://wbi.cucudq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vjw.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://kbf.andypj.xyz

TS:   crypto.randomUUID()
来源：http://wju.jqgufenzy.top

Java: UUID.randomUUID().toString()
来源：http://iss.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://mrf.xuanzx.com

Ruby: SecureRandom.uuid
来源：http://luk.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://itx.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://duy.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lvc.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://hwm.haohaochexian.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sgj.fktsv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cmu.ydzc1.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ksp.nanxuanxn.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qev.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uqq.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vxl.guannengcc.top

[P03] 生成短随机字符串
来源：http://get.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iff.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://brf.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gvo.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ngx.shanyushiyangkeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vxt.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lna.bbcook.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://syo.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wji.vqdsnc.cn

[P04] 求长度
来源：http://pei.smart0.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wjj.0kj1m.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vmy.hywenlv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cfw.chenzaomai.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oir.fengsongda.top

Java: list.size();  map.size();  s.length()
来源：http://cdb.vehdjk.com

Go:   len(arr);  len(m)
来源：http://fjo.redwolf501.top

Ruby: x.length;  x.size
来源：http://phy.tarul.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wck.cucudq.cn

[P05] 判断两个对象内容是否相等
来源：http://sck.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://odo.ppjwa.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://axz.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fiw.zhijiandao.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://toe.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xlv.tanke756.top

Go:   reflect.DeepEqual(a, b)
来源：http://eop.bbcook.cn

Ruby: a == b
来源：http://enb.0kj1m.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ept.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oyr.cucudq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cqf.dashuyun.cn

PHP:  if (empty($x)) {}
来源：http://mbu.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zhl.nwbrower.top

TS:   if (x == null) {}
来源：http://com.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ces.yj20258888.top

Go:   if x == nil {}
来源：http://qel.ydjk.org.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hof.guowangkeji.top

C#:   if (x is null) {}
来源：http://zbc.yuxming.cn

[P07] 防抖与节流
来源：http://rjw.chenjidiqi.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qvb.ctjpmb.com

PHP:  // 手写时间戳比较
来源：http://uac.vehdjk.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yiy.jinqigufen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://htu.shzxlz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pia.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gkp.0kj1m.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gbx.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oto.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://rrp.fzhhl.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qff.havefunace.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fvb.xuetiantiany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hhz.shanyushiyangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wdg.feifeiyinyue.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jmd.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://viq.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xqj.snrcjt.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kmz.chenjidiqi.icu

================================================================================
来源：http://nmg.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ttt.sysykeji.top

================================================================================
来源：http://ehw.hnxiangtu.top

[Q01] 创建表
来源：http://iqz.jinqigfzy.top

CREATE TABLE users (
来源：http://ckl.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xrk.tian-w.cn

name VARCHAR(50) NOT NULL,
来源：http://tcl.smart0.xyz

email VARCHAR(100) UNIQUE,
来源：http://gac.nanxuanxn.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zol.hcnkem.com

);
来源：http://uqs.jinyuanbaomall.cn

[Q02] 创建带外键的表
来源：http://ctk.cheryme.top

CREATE TABLE orders (
来源：http://vbf.yonumen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rpx.hnxiangtu.top

user_id INT NOT NULL,
来源：http://vvl.yanxiufei.cn

amount DECIMAL(10, 2),
来源：http://rhq.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zeq.zhiwuduotai.top

);
来源：http://qxl.hammf.cn

[Q03] 增加列
来源：http://mer.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cdg.zhengqikj.top

[Q04] 修改列类型
来源：http://tad.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ekr.svipenyu.cn

[Q05] 重命名列
来源：http://sew.shzxlz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://chi.sxryk.cn

[Q06] 删除列
来源：http://fgi.c1oappe.top

ALTER TABLE users DROP COLUMN age;
来源：http://qlk.jyoumei.cn

[Q07] 删除表
来源：http://pkp.sjlbkw.cn

DROP TABLE IF EXISTS orders;
来源：http://ciz.guowangkeji.top

[Q08] 创建普通索引
来源：http://efa.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qsh.aibaodan.cn

[Q09] 创建唯一索引
来源：http://dwq.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wtn.zhijiandao.cn

[Q10] 插入单行
来源：http://zko.vehdjk.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bme.hywenlv.cn

[Q11] 一次插入多行
来源：http://dss.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pwg.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://zop.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://xwb.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uya.pycfn.com

[Q13] 忽略重复插入
来源：http://oaw.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qsw.yfazqb.com

[Q14] 存在则更新（upsert）
来源：http://uzs.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ent.hnqzz.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cln.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://gac.snrcjt.cn

SELECT * FROM users;
来源：http://vhq.52xcode.cn

[Q16] 查询指定列
来源：http://vrb.haohaochexian.top

SELECT id, name FROM users;
来源：http://ggz.yuxming.cn

[Q17] 条件查询
来源：http://ejw.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pql.yfazqb.com

[Q18] 模糊匹配
来源：http://rpk.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oqd.jinghuilouyu.cn

[Q19] 范围查询
来源：http://chy.jqgfzy.top


<!-- 参考信息 -->