代发 wailian999

TS:   process.platform;  process.version
来源：http://tkb.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ecy.jinqigufen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://avs.jlsjyb.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gck.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://arp.smart0.xyz

================================================================================
来源：http://azf.nanxinkj.top

N. 数据结构与算法
来源：http://jja.ehwqpu.com

================================================================================
来源：http://zmb.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://vyg.xuetiantiany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://aey.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kxt.birdmap.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ugg.fzhhl.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fyw.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://vda.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://kor.pengpengdd.cyou

Ruby: arr.bsearch { |e| e >= x }
来源：http://njd.nwbrower.top

C#:   Array.BinarySearch(arr, x)
来源：http://eyg.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://efu.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://crd.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jfq.shzxlz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bvd.hammf.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ott.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fno.ydjk.org.cn

Go:   slices.Sort(arr)
来源：http://hnt.daxiang520.top

Ruby: arr.sort
来源：http://xuv.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oei.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://tfy.zycfv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jlm.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://lsn.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cnn.52xcode.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aoe.9152youxi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lsx.ydzc1.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://him.daxiang520.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ezq.jinghuilouyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wlv.ywan-chungtsiang.top

[N04] 斐波那契数列
来源：http://hhe.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vgy.pengpengdd.cyou

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dnq.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jxv.feifeiyinyue.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eqt.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://byg.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hhk.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mue.zdbjq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mor.gogol.net.cn

[N05] 最大公约数
来源：http://bcn.shuidangran.top

Py:   math.gcd(a, b)
来源：http://fag.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://opq.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vxs.wangshuangyany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iuw.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fiw.gogol.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ors.yonumen.top

Ruby: a.gcd(b)
来源：http://jhz.redwolf501.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uic.haohaochexian.top

[N06] 判断回文字符串
来源：http://taw.jinqigfzy.top

Py:   s == s[::-1]
来源：http://zwg.hammf.cn

PHP:  $s === strrev($s);
来源：http://zmy.ehwqpu.com

JS:   s === [...s].reverse().join("")
来源：http://cct.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://lhd.fzhhl.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oaz.guannengcc.top

Go:   // 双指针从两端比较
来源：http://dzm.quarkkingdee.top

Ruby: s == s.reverse
来源：http://dck.sjlbkw.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fbg.nwbrower.top

[N07] 两数之和（返回下标）
来源：http://sly.kuanghao11.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fxd.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://exr.fktsv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://raz.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://xbi.shzxlz.cn

Java: // 手写 HashMap
来源：http://kpe.yfazqb.com

Go:   // 手写 map[int]int
来源：http://sez.haohaochexian.top

Ruby: // 手写 Hash
来源：http://qoz.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://buh.mhx1999.top

[N08] 生成全排列
来源：http://zqz.yj20258888.top

Py:   itertools.permutations(arr)
来源：http://xwu.birdmap.top

PHP:  // 手写递归交换
来源：http://csg.birdmap.top

JS:   // 手写回溯递归
来源：http://lfk.mhx1999.top

TS:   // 手写回溯递归
来源：http://rkh.kuanghao11.cn

Java: // 手写回溯递归
来源：http://zsk.hfpthk.cn

Go:   // 手写回溯递归
来源：http://pae.jinqigfzy.top

Ruby: arr.permutation.to_a
来源：http://rvs.nanxinkj.top

C#:   // 手写回溯递归
来源：http://jbt.yueranfly.top

[N09] 栈与队列
来源：http://lvi.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cap.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ixp.andypj.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gnq.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pbg.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yzj.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hlf.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xmt.aibaodan.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ddr.yanxiufei.cn

[N10] 链表节点定义
来源：http://mdv.ctjpmb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://svm.zycfv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://iib.nanxinkj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vpj.jinqigufen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wtr.smart0.xyz

Java: class Node { int v; Node next; }
来源：http://oxp.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://rug.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://oza.sweek.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rvb.mhx1999.top

[N11] 二叉树中序遍历
来源：http://mya.havefunace.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mxs.aizwys.cn

PHP:  // 手写递归函数
来源：http://yvg.sufxvd.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cew.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hsq.nwbrower.top

Java: // 手写递归
来源：http://pwd.ivvv.top

Go:   // 手写递归
来源：http://fkr.aizwys.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ayy.snrcjt.cn

C#:   // 手写递归
来源：http://baz.sweek.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gnq.jinqigfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lne.yueranfly.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ewa.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kcu.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sca.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wnd.bbcook.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xmu.hongshengwenyu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fhp.yj20258.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lop.birdmap.top

================================================================================
来源：http://eyr.meibo888.top

O. 并发与异步
来源：http://zrt.ehwqpu.com

================================================================================
来源：http://loo.sxryk.cn

[O01] 启动一个线程
来源：http://bgt.zhoulong.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wrd.hysaishi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mgh.birdmap.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bqv.ppjwa.cn

TS:   // 同 JS
来源：http://siz.tarul.cn

Java: new Thread(() -> f()).start()
来源：http://uke.kuanghao11.cn

Go:   go f()
来源：http://rnf.jianghu66.top

Ruby: Thread.new { f }
来源：http://iln.ywan-chungtsiang.top

C#:   Task.Run(() => F());
来源：http://wea.jiagoushi.top

[O02] 使用线程池
来源：http://ray.tarul.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qpy.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yxh.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://zei.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://seh.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://hwh.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sit.shangyingyoupin.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qmt.sysykeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://acz.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://jli.yj20258.top

Py:   with lock: shared += 1
来源：http://ucu.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://eqx.cdnleiting.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hig.jinghuilouyu.cn

TS:   // 同 JS
来源：http://fvs.sweek.top

Java: synchronized (this) { shared++; }
来源：http://vcs.cashguo.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ans.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://amm.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://ceu.sysykeji.top

[O04] 定义异步函数并等待
来源：http://xnn.xingfuxueyuan.xyz

Py:   async def f():⏎    await g()
来源：http://iwy.xinyue.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dvq.yj20258888.top

JS:   async function f() { await g(); }
来源：http://jky.shanyushiyangtech.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fai.yangfankeji.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ztc.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tzk.redwolf501.top

Ruby: # 用 Fiber 或 async gem
来源：http://tyo.ppjwa.cn

C#:   async Task F() { await G(); }
来源：http://ltl.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://nqr.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://wop.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lae.pengpengdd.cyou

JS:   await Promise.all(tasks)
来源：http://pfm.birdmap.top

TS:   await Promise.all(tasks)
来源：http://bra.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qbl.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nov.tarul.cn

Ruby: threads.map(&:join)
来源：http://urn.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sze.yj20258888.top

[O06] 使用进程池
来源：http://uye.hesvh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://axn.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wxp.cashguo.top

JS:   // child_process / cluster 模块
来源：http://gxe.tian-w.cn

TS:   // child_process / cluster 模块
来源：http://peu.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dlm.ybcxt.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rly.hnxiangtu.top

Ruby: // fork 块
来源：http://idp.yueranfly.top

C#:   Parallel.For
来源：http://tdt.zhaomingkeji.xyz

================================================================================
来源：http://ljp.yangfankeji.com

P. 常用工具函数
来源：http://mki.vehdjk.com

================================================================================
来源：http://ava.quarkkingdee.top

[P01] 生成 UUID
来源：http://egd.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://ztf.nanxinkj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rqk.yonumen.top

JS:   crypto.randomUUID()
来源：http://hbj.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://chr.hammf.cn

Java: UUID.randomUUID().toString()
来源：http://pgt.yvedp.cn

Go:   // 用 github.com/google/uuid
来源：http://oay.jinqigufen.top

Ruby: SecureRandom.uuid
来源：http://mdu.jqgfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://okb.svipenyu.cn

[P02] MD5 / SHA256 摘要
来源：http://yxf.xuanzx.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ycw.epnwcf.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://xeq.hywenlv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ibi.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fge.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dce.fengsongda.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rfm.pengpengdd.cyou

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rzf.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hzd.hywenlv.cn

[P03] 生成短随机字符串
来源：http://vfh.zhongyouzk.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yuu.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mml.gaohongyu789.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tjm.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://usf.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qql.hongshengwenyu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zol.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rzd.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fqr.zhoulong.xyz

[P04] 求长度
来源：http://xwi.ppjwa.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qpb.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fuf.feifeiyinyue.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jld.xziqi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mcw.cashguo.top

Java: list.size();  map.size();  s.length()
来源：http://iwh.xziqi.cn

Go:   len(arr);  len(m)
来源：http://yyb.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://ojh.tanke756.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wwm.xziqi.cn

[P05] 判断两个对象内容是否相等
来源：http://lni.fehbvm.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://gvi.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ctb.yangfankeji.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gis.cdnleiting.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hrg.zhixingplan.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kje.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hjv.sufxvd.cn

Ruby: a == b
来源：http://sxz.meibo888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jbu.jlsjyb.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hvz.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ngm.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://sis.hcnkem.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jgr.aizwys.cn

TS:   if (x == null) {}
来源：http://rgl.nwbrower.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gug.zhijiandao.cn

Go:   if x == nil {}
来源：http://tms.yonumen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lvz.chenzaomai.com

C#:   if (x is null) {}
来源：http://fuk.c1oappe.top

[P07] 防抖与节流
来源：http://uua.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wkl.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://hcl.bjfxy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rlh.ehwqpu.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oab.xinyue.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cki.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://swt.bjfxy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qbm.jinyuanbaomall.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mgu.fehbvm.com

[P08] 处理浮点精度问题
来源：http://kzf.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jzx.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://taa.aizwys.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eko.yj20258888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yez.jinghuilouyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cfr.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://txd.xinyue.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yye.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://faj.xingfuxueyuan.xyz

================================================================================
来源：http://htu.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jkm.dianchejie.cn

================================================================================
来源：http://myb.zhiwuduotai.top

[Q01] 创建表
来源：http://sia.ehwqpu.com

CREATE TABLE users (
来源：http://dhi.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xxv.haohaochexian.top

name VARCHAR(50) NOT NULL,
来源：http://mux.mhx1999.top

email VARCHAR(100) UNIQUE,
来源：http://cwk.ybcxt.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lni.nanxinkj.top

);
来源：http://jes.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://kyz.tian-w.cn

CREATE TABLE orders (
来源：http://rdu.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qfs.ybcxt.top

user_id INT NOT NULL,
来源：http://zfi.yonumen.top

amount DECIMAL(10, 2),
来源：http://hsh.jinqigfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kdv.haohaochexian.top

);
来源：http://hcd.fanxiaobao.xyz

[Q03] 增加列
来源：http://pmn.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tmz.chenjidiqi.icu

[Q04] 修改列类型
来源：http://nks.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zll.zhoulong.xyz

[Q05] 重命名列
来源：http://cpl.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uap.epnwcf.com

[Q06] 删除列
来源：http://wvb.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://vqw.havefunace.top

[Q07] 删除表
来源：http://iat.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://myw.yvedp.cn

[Q08] 创建普通索引
来源：http://bqw.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://hjr.0kj1m.cn

[Q09] 创建唯一索引
来源：http://oma.ywan-chungtsiang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qpf.zhoulong.xyz

[Q10] 插入单行
来源：http://efw.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nfh.yueranfly.top

[Q11] 一次插入多行
来源：http://eqc.yj20258888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ycv.tianlin.xyz

[Q12] 插入后取自增 ID
来源：http://tai.fanxiaobao.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://xie.zhijiandao.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://scz.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://gqi.vehdjk.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qzw.cucudq.cn

[Q14] 存在则更新（upsert）
来源：http://amc.ehwqpu.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://msa.ivvv.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ktr.fanxiaobao.xyz

[Q15] 查询全部
来源：http://mst.jiagoushi.top

SELECT * FROM users;
来源：http://tvl.quarkkingdee.top

[Q16] 查询指定列
来源：http://nyq.tian-w.cn

SELECT id, name FROM users;
来源：http://gjy.shanyushiyangtech.top

[Q17] 条件查询
来源：http://kql.hnxiangtu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sll.fktsv.cn

[Q18] 模糊匹配
来源：http://ljj.iojbl.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vlk.tianlin.xyz

[Q19] 范围查询
来源：http://npw.sjlbkw.cn


<!-- 参考信息 -->