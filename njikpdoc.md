代发 wailian999

Java: public static void main(String[] args)
来源：http://ztp.yj202588.top

Go:   func main()
来源：http://lpn.nanxinkj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lod.gogol.net.cn

C#:   static void Main(string[] args)
来源：http://ioi.jiagoushi.top

[M08] 获取系统与运行时信息
来源：http://hyf.zhijiandao.cn

Py:   platform.system();  platform.python_version()
来源：http://ytm.guannengcc.top

PHP:  PHP_OS;  phpversion();
来源：http://jua.bjfxy.top

JS:   process.platform;  process.version
来源：http://rlu.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://tcf.gzhubu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uow.xingfuxueyuan.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ods.hnxiangtu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fbg.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://izc.cashguo.top

================================================================================
来源：http://dkj.sjlbkw.cn

N. 数据结构与算法
来源：http://tfz.yj20258.top

================================================================================
来源：http://grf.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://cfh.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sgg.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jdz.dashuyun.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://czt.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ijb.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://juy.quarkkingdee.top

Go:   sort.SearchInts(arr, x)
来源：http://sbq.zhijiandao.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lbt.jianghu66.top

C#:   Array.BinarySearch(arr, x)
来源：http://pfp.sweek.top

[N02] 排序（工程实践用内置实现）
来源：http://pzy.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://wlw.ybcxt.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pwf.sjlbkw.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ylj.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kae.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nvj.jyoumei.cn

Go:   slices.Sort(arr)
来源：http://hyg.yuanzhike.top

Ruby: arr.sort
来源：http://lin.yj20258888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://eyu.316326.xyz

[N03] 快速排序（分治示例）
来源：http://hpz.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jpb.daxiang520.top

PHP:  // 递归实现，或用 usort
来源：http://dxr.jiagoushi.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yhn.daxiang520.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bmp.birdmap.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://owm.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://max.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eoj.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hfe.guannengcc.top

[N04] 斐波那契数列
来源：http://jsi.zhoulong.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://emx.tarul.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lfn.fengsongda.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xxv.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lgn.zhoulong.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qnx.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iqf.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tjn.tanke756.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://war.yueranfly.top

[N05] 最大公约数
来源：http://him.bjfxy.top

Py:   math.gcd(a, b)
来源：http://tzg.yueranfly.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vtt.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hiy.kuanghao11.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://taa.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mql.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gtl.zycfv.cn

Ruby: a.gcd(b)
来源：http://orn.xinyue.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://orl.yj20258888.top

[N06] 判断回文字符串
来源：http://usd.9152youxi.cn

Py:   s == s[::-1]
来源：http://avr.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://odm.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://vte.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://kyv.ppjwa.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mfg.yuxming.cn

Go:   // 双指针从两端比较
来源：http://ivi.zdbjq.cn

Ruby: s == s.reverse
来源：http://bwe.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ehc.xziqi.cn

[N07] 两数之和（返回下标）
来源：http://vpd.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dba.meibo888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wzp.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zen.havefunace.top

TS:   // 手写 Map<string, number>
来源：http://uxg.meibo888.top

Java: // 手写 HashMap
来源：http://hpm.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://mfp.yonumen.top

Ruby: // 手写 Hash
来源：http://rlk.sufxvd.cn

C#:   // 手写 Dictionary<int, int>
来源：http://flm.gotoacloud.top

[N08] 生成全排列
来源：http://xnx.havefunace.top

Py:   itertools.permutations(arr)
来源：http://ccv.jinyuanbaomall.cn

PHP:  // 手写递归交换
来源：http://hbd.52xcode.cn

JS:   // 手写回溯递归
来源：http://fei.nwbrower.top

TS:   // 手写回溯递归
来源：http://lzn.andypj.xyz

Java: // 手写回溯递归
来源：http://nbk.chenlongwang.top

Go:   // 手写回溯递归
来源：http://des.cdnleiting.top

Ruby: arr.permutation.to_a
来源：http://giv.hywenlv.cn

C#:   // 手写回溯递归
来源：http://ydv.jinqigfzy.top

[N09] 栈与队列
来源：http://hwn.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jbs.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://new.zycfv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nva.jqgufenzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vve.bbcook.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://opq.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nca.vqdsnc.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://flm.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ovv.jinqigufen.top

[N10] 链表节点定义
来源：http://gss.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://udr.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://teb.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xcc.vehdjk.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ooj.tian-w.cn

Java: class Node { int v; Node next; }
来源：http://pey.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://eqw.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mhh.yvedp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://auc.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://ugc.feifeiyinyue.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uxs.ybcxt.top

PHP:  // 手写递归函数
来源：http://usp.zhijiandao.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bzg.redwolf501.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://huu.bjfxy.top

Java: // 手写递归
来源：http://itx.chenzaomai.com

Go:   // 手写递归
来源：http://ctz.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nfh.gogol.net.cn

C#:   // 手写递归
来源：http://bhb.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hqb.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://irf.nanxuanxn.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uiv.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://afu.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dex.andypj.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://key.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hoy.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wdd.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://otd.shangyingyoupin.top

================================================================================
来源：http://dzs.nanxuanxn.top

O. 并发与异步
来源：http://wug.gotoacloud.top

================================================================================
来源：http://rss.yongpay.top

[O01] 启动一个线程
来源：http://uyy.zdbjq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sqi.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rea.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nyc.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://dmq.jinqigufen.top

Java: new Thread(() -> f()).start()
来源：http://tiu.nanxinkj.top

Go:   go f()
来源：http://bzh.bjfxy.top

Ruby: Thread.new { f }
来源：http://nvp.52xcode.cn

C#:   Task.Run(() => F());
来源：http://tfw.shuidangran.top

[O02] 使用线程池
来源：http://bwj.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vpk.0kj1m.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mem.nwbrower.top

JS:   // worker_threads 线程池
来源：http://vxx.xuetiantiany.cn

TS:   // worker_threads 线程池
来源：http://vzf.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://ixz.shuidangran.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qds.cashguo.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vdr.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ygq.wangdashe.top

[O03] 加锁保护共享数据
来源：http://cpg.pycfn.com

Py:   with lock: shared += 1
来源：http://gvl.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://cmb.cucudq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rhy.yj20258.top

TS:   // 同 JS
来源：http://avk.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://cyn.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gnv.shangyingyoupin.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://otn.chenjidiqi.icu

C#:   lock (gate) { shared++; }
来源：http://ujx.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://rbk.ivvv.top

Py:   async def f():⏎    await g()
来源：http://rzv.haohaochexian.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wlx.mhx1999.top

JS:   async function f() { await g(); }
来源：http://uuf.cheryme.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bpe.hongshengwenyu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cox.fktsv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eto.hesvh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jxh.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://gen.cheryme.top

[O05] 并发执行并等待全部完成
来源：http://qhp.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://zcq.fengsongda.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ykh.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://nce.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://bvf.hfpthk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vvd.ybcxt.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uen.mhx1999.top

Ruby: threads.map(&:join)
来源：http://ndm.nanxinkj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zwk.mhx1999.top

[O06] 使用进程池
来源：http://bik.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gof.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sii.sweek.top

JS:   // child_process / cluster 模块
来源：http://hqx.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://thq.yfazqb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ioe.havefunace.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sfp.guowangkeji.top

Ruby: // fork 块
来源：http://ylw.tanke756.top

C#:   Parallel.For
来源：http://evv.shuidangran.top

================================================================================
来源：http://zdb.gaohongyu789.top

P. 常用工具函数
来源：http://xrm.kuanghao11.cn

================================================================================
来源：http://hzv.nwbrower.top

[P01] 生成 UUID
来源：http://ihx.hnqzz.top

Py:   str(uuid.uuid4())
来源：http://jsf.aibaodan.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://obu.xziqi.cn

JS:   crypto.randomUUID()
来源：http://jwp.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://vdj.cashguo.top

Java: UUID.randomUUID().toString()
来源：http://las.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://frq.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://lwl.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://fgt.jlsjyb.cn

[P02] MD5 / SHA256 摘要
来源：http://zzw.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dkp.chenlongwang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dvv.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jzn.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fdk.gogol.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ami.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cvs.fktsv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dgs.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tkv.ydjk.org.cn

[P03] 生成短随机字符串
来源：http://cts.tianlin.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lxv.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hgj.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qan.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pkl.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://smb.gaohongyu789.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nco.dianchejie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wpi.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rmm.fzhhl.top

[P04] 求长度
来源：http://jao.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iql.gotoacloud.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://afe.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ere.shzxlz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pfe.yonumen.top

Java: list.size();  map.size();  s.length()
来源：http://qqh.yj20258888.top

Go:   len(arr);  len(m)
来源：http://lna.0kj1m.cn

Ruby: x.length;  x.size
来源：http://zdb.fanxiaobao.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://asa.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://wno.316326.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://mal.nwbrower.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cgj.pengpengdd.cyou

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gqd.mhx1999.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rcx.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mnx.sweek.top

Go:   reflect.DeepEqual(a, b)
来源：http://kzb.hysaishi.cn

Ruby: a == b
来源：http://uxu.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fql.ywan-chungtsiang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bvb.jinyuanbaomall.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uyn.chenzaomai.com

PHP:  if (empty($x)) {}
来源：http://vuf.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tme.hysaishi.cn

TS:   if (x == null) {}
来源：http://iut.jinghuilouyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vhd.hnxiangtu.top

Go:   if x == nil {}
来源：http://hkg.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lvz.tian-w.cn

C#:   if (x is null) {}
来源：http://bgq.fehbvm.com

[P07] 防抖与节流
来源：http://qwa.fengsongda.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fcf.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://oxe.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rpg.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rae.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ppk.zhiwuduotai.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://awl.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lmp.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oqs.havefunace.top

[P08] 处理浮点精度问题
来源：http://ttg.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tyh.sysykeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://knj.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bax.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aeh.xuanzx.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vwf.ppjwa.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lst.fanxiaobao.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://egp.redwolf501.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cyp.shzxlz.cn

================================================================================
来源：http://azu.vehdjk.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zgb.sweek.top

================================================================================
来源：http://fmm.cheryme.top

[Q01] 创建表
来源：http://fpd.shanyushiyangtech.top

CREATE TABLE users (
来源：http://bjl.jinqigfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://agt.sweek.top

name VARCHAR(50) NOT NULL,
来源：http://czi.meibo888.top

email VARCHAR(100) UNIQUE,
来源：http://syh.yonumen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hns.pengpengdd.cyou

);
来源：http://pkm.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://pjw.iojbl.cn

CREATE TABLE orders (
来源：http://nuf.sufxvd.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yaq.tarul.cn

user_id INT NOT NULL,
来源：http://lci.shanyushiyangkeji.top

amount DECIMAL(10, 2),
来源：http://kpf.yongpay.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ksh.svipenyu.cn

);
来源：http://bqk.jianghu66.top

[Q03] 增加列
来源：http://mlf.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://szu.tian-w.cn

[Q04] 修改列类型
来源：http://gun.ywan-chungtsiang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oui.zhengqikj.top

[Q05] 重命名列
来源：http://nbc.gotoacloud.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://guy.sysykeji.top

[Q06] 删除列
来源：http://yyv.zhengqikj.top

ALTER TABLE users DROP COLUMN age;
来源：http://ayv.yueranfly.top

[Q07] 删除表
来源：http://uze.hcnkem.com

DROP TABLE IF EXISTS orders;
来源：http://afe.vehdjk.com

[Q08] 创建普通索引
来源：http://dej.gaohongyu789.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nke.xinyue.icu

[Q09] 创建唯一索引
来源：http://uai.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iiy.hammf.cn

[Q10] 插入单行
来源：http://qpg.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pqw.jinqigfzy.top

[Q11] 一次插入多行
来源：http://rzn.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yfp.bbcook.cn

[Q12] 插入后取自增 ID
来源：http://otb.zhijiandao.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zjc.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mmg.52xcode.cn

[Q13] 忽略重复插入
来源：http://vnd.yueranfly.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oxh.yj20258.top

[Q14] 存在则更新（upsert）
来源：http://ere.xylfe.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rmn.ctjpmb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wys.hnqzz.top

[Q15] 查询全部
来源：http://qml.shzxlz.cn


<!-- 参考信息 -->