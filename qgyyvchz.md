代发 wailian999

TS:   process.platform;  process.version
来源：http://cnw.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://isf.yvedp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pwb.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yew.birdmap.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tpj.sxryk.cn

================================================================================
来源：http://veq.zhengqikj.top

N. 数据结构与算法
来源：http://ewg.dashuyun.cn

================================================================================
来源：http://cwv.shuidangran.top

[N01] 二分查找（有序数组）
来源：http://kps.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kki.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fur.zhiwuduotai.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cfp.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wfv.vqdsnc.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ylt.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://ycx.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xpq.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://wnv.quarkkingdee.top

[N02] 排序（工程实践用内置实现）
来源：http://bke.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://owy.jlsjyb.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fnv.kuanghao11.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pov.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fya.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xvo.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://eoa.jlsjyb.cn

Ruby: arr.sort
来源：http://quy.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ktt.sjlbkw.cn

[N03] 快速排序（分治示例）
来源：http://bkg.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ces.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://zyc.yueranfly.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jrj.ydjk.org.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xgg.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://isg.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ufl.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iei.jinghuilouyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tli.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://cjo.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://edu.daria6918.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hew.nanxuanxn.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jru.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://icj.cashguo.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nqi.xinyue.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rny.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nbe.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zgl.shanyushiyangtech.top

[N05] 最大公约数
来源：http://vcv.quarkkingdee.top

Py:   math.gcd(a, b)
来源：http://bfe.jinghuilouyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gxh.9152youxi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qvw.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://caf.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://trj.ehwqpu.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gie.xylfe.cn

Ruby: a.gcd(b)
来源：http://gmf.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lsg.smart0.xyz

[N06] 判断回文字符串
来源：http://cka.jinqigfzy.top

Py:   s == s[::-1]
来源：http://akr.andypj.xyz

PHP:  $s === strrev($s);
来源：http://kfm.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://jwo.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://gtl.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ygx.fzhhl.top

Go:   // 双指针从两端比较
来源：http://gzp.hesvh.cn

Ruby: s == s.reverse
来源：http://tmg.wangshuangyany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pcp.cashguo.top

[N07] 两数之和（返回下标）
来源：http://xrs.xinyue.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ezg.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xpa.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sxk.zycfv.cn

TS:   // 手写 Map<string, number>
来源：http://pgv.pengpengdd.cyou

Java: // 手写 HashMap
来源：http://mgs.cqqwz.cn

Go:   // 手写 map[int]int
来源：http://jly.zdbjq.cn

Ruby: // 手写 Hash
来源：http://whm.ydjk.org.cn

C#:   // 手写 Dictionary<int, int>
来源：http://eft.nanxuanxn.top

[N08] 生成全排列
来源：http://uzy.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://seh.chenjidiqi.icu

PHP:  // 手写递归交换
来源：http://mzn.haohaochexian.top

JS:   // 手写回溯递归
来源：http://lcm.havefunace.top

TS:   // 手写回溯递归
来源：http://uff.yanxiufei.cn

Java: // 手写回溯递归
来源：http://xyh.ybcxt.top

Go:   // 手写回溯递归
来源：http://ubg.kuanghao11.cn

Ruby: arr.permutation.to_a
来源：http://zzh.yuxming.cn

C#:   // 手写回溯递归
来源：http://fio.meibo888.top

[N09] 栈与队列
来源：http://dvu.hongshengwenyu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mub.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://avs.jinghuilouyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qrf.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rqf.jlsjyb.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cxl.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hpb.yj20258.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zxq.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fjn.pengpengdd.cyou

[N10] 链表节点定义
来源：http://icn.zycfv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ixo.hywenlv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dit.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aql.fzhhl.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ove.shanyushiyangkeji.top

Java: class Node { int v; Node next; }
来源：http://eto.sjlbkw.cn

Go:   type Node struct { V int; Next *Node }
来源：http://idc.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://kip.redwolf501.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tpn.wangdashe.top

[N11] 二叉树中序遍历
来源：http://sfj.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tek.tian-w.cn

PHP:  // 手写递归函数
来源：http://ylv.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lrm.chenzaomai.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://knc.zhaomingkeji.xyz

Java: // 手写递归
来源：http://pyx.ydzc1.top

Go:   // 手写递归
来源：http://uvf.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jjo.nanxinkj.top

C#:   // 手写递归
来源：http://omg.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://scl.zhoulong.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bwf.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qeg.epnwcf.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ujk.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xrs.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bfp.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lzc.bbcook.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nzf.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qhb.jianghu66.top

================================================================================
来源：http://rpd.yuanzhike.top

O. 并发与异步
来源：http://why.yuanzhike.top

================================================================================
来源：http://ynq.xuanzx.com

[O01] 启动一个线程
来源：http://frg.shanyushiyangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tkk.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kwo.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dam.tianlin.xyz

TS:   // 同 JS
来源：http://xeo.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://ldk.dashuyun.cn

Go:   go f()
来源：http://wyc.yfazqb.com

Ruby: Thread.new { f }
来源：http://ynk.bbcook.cn

C#:   Task.Run(() => F());
来源：http://xrn.guowangkeji.top

[O02] 使用线程池
来源：http://blq.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://deq.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uzr.hammf.cn

JS:   // worker_threads 线程池
来源：http://pyb.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://lmw.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://ofk.shanyushiyangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zvv.dianchejie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ohj.yj202588.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oqr.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://spi.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://iug.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://aac.hnxiangtu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wyj.jlsjyb.cn

TS:   // 同 JS
来源：http://plh.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://eji.cashguo.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uov.ybcxt.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://yvt.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://mwh.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://uzv.dianchejie.cn

Py:   async def f():⏎    await g()
来源：http://dos.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tvy.nanxinkj.top

JS:   async function f() { await g(); }
来源：http://ccs.cdnleiting.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jaa.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://luy.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jzk.kuanghao11.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cru.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://esp.mhx1999.top

[O05] 并发执行并等待全部完成
来源：http://jvo.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://zsp.cdnleiting.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ree.cheryme.top

JS:   await Promise.all(tasks)
来源：http://yve.wangshuangyany.cn

TS:   await Promise.all(tasks)
来源：http://huf.hnqzz.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iko.hesvh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ska.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://ima.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vea.ctjpmb.com

[O06] 使用进程池
来源：http://fwi.bbcook.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://etr.nanxinkj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qmu.smart0.xyz

JS:   // child_process / cluster 模块
来源：http://maz.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://yop.zdqjudy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dvr.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oeh.daxiang520.top

Ruby: // fork 块
来源：http://bsu.aizwys.cn

C#:   Parallel.For
来源：http://yvc.pycfn.com

================================================================================
来源：http://xkp.chenjidiqi.icu

P. 常用工具函数
来源：http://mdt.sjlbkw.cn

================================================================================
来源：http://ino.ybcxt.top

[P01] 生成 UUID
来源：http://wbb.xinyue.icu

Py:   str(uuid.uuid4())
来源：http://nul.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wzz.epnwcf.com

JS:   crypto.randomUUID()
来源：http://gad.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://qgg.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://xac.aibaodan.cn

Go:   // 用 github.com/google/uuid
来源：http://cme.yj20258.top

Ruby: SecureRandom.uuid
来源：http://owl.yangfankeji.com

C#:   Guid.NewGuid().ToString()
来源：http://fiu.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://peq.gotoacloud.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yhm.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wix.hnxiangtu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lnj.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://akg.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fxs.fktsv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hjb.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ubq.ydjk.org.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ydm.yonumen.top

[P03] 生成短随机字符串
来源：http://obb.haohaochexian.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nnc.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ukm.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kyo.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ggx.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yji.guannengcc.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uzj.birdmap.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tqz.ctjpmb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tak.jiagoushi.top

[P04] 求长度
来源：http://rvs.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://icy.hysaishi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zwy.zhixingplan.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://quz.ctjpmb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wkf.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://tuj.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://bsv.xuanzx.com

Ruby: x.length;  x.size
来源：http://htd.yj20258.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tdn.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://kxq.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://exb.mhx1999.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kxe.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fxt.birdmap.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ttr.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wpe.sufxvd.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jvr.yj20258.top

Ruby: a == b
来源：http://map.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://buy.vehdjk.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qpm.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dng.jinqigufen.top

PHP:  if (empty($x)) {}
来源：http://cbq.nanxuanxn.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://anf.vehdjk.com

TS:   if (x == null) {}
来源：http://uvk.sjlbkw.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jpn.gzhubu.top

Go:   if x == nil {}
来源：http://inh.gotoacloud.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pbv.cucudq.cn

C#:   if (x is null) {}
来源：http://yqm.zhiwuduotai.top

[P07] 防抖与节流
来源：http://rnr.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cpk.fanxiaobao.xyz

PHP:  // 手写时间戳比较
来源：http://szv.wangshuangyany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wwc.jianghu66.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ryz.vqdsnc.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://leg.ppjwa.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pvs.wangdashe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fdn.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://scb.nwbrower.top

[P08] 处理浮点精度问题
来源：http://xjh.birdmap.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fts.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dwo.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wrl.epnwcf.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fgb.tianlin.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wjt.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qno.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oze.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://awi.gaohongyu789.top

================================================================================
来源：http://ysx.hnxiangtu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zjf.xuetiantiany.cn

================================================================================
来源：http://zrj.fengsongda.top

[Q01] 创建表
来源：http://vhg.gotoacloud.top

CREATE TABLE users (
来源：http://jjr.ywan-chungtsiang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ppg.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://cwg.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://mwn.chenzaomai.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://owy.gotoacloud.top

);
来源：http://fxc.aizwys.cn

[Q02] 创建带外键的表
来源：http://ksf.ctjpmb.com

CREATE TABLE orders (
来源：http://rjq.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vey.zycfv.cn

user_id INT NOT NULL,
来源：http://kja.shanyushiyangkeji.top

amount DECIMAL(10, 2),
来源：http://fnw.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lxi.snrcjt.cn

);
来源：http://hog.xziqi.cn

[Q03] 增加列
来源：http://asg.sysykeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dtd.hcnkem.com

[Q04] 修改列类型
来源：http://dkw.hcnkem.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jsj.chenlongwang.top

[Q05] 重命名列
来源：http://fof.jqgfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rpz.hnqzz.top

[Q06] 删除列
来源：http://anv.yanxiufei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ady.ehwqpu.com

[Q07] 删除表
来源：http://exb.meibo888.top

DROP TABLE IF EXISTS orders;
来源：http://moj.hywenlv.cn

[Q08] 创建普通索引
来源：http://nkv.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hhs.nwbrower.top

[Q09] 创建唯一索引
来源：http://keh.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hqt.nanxinkj.top

[Q10] 插入单行
来源：http://rjb.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vnt.smart0.xyz

[Q11] 一次插入多行
来源：http://pcp.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qfl.yj20258888.top

[Q12] 插入后取自增 ID
来源：http://ntz.yueranfly.top

INSERT INTO users (name) VALUES ('C');
来源：http://jkg.cheryme.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ibx.hcnkem.com

[Q13] 忽略重复插入
来源：http://tgs.iojbl.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hzj.yangfankeji.com

[Q14] 存在则更新（upsert）
来源：http://vkj.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ifw.jinghuilouyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fsv.fehbvm.com

[Q15] 查询全部
来源：http://zky.cdnleiting.top

SELECT * FROM users;
来源：http://loo.shangyingyoupin.top

[Q16] 查询指定列
来源：http://rsd.xuanzx.com

SELECT id, name FROM users;
来源：http://lkx.shanyushiyangtech.top

[Q17] 条件查询
来源：http://fcx.dashuyun.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jjf.zhijiandao.cn

[Q18] 模糊匹配
来源：http://zvh.birdmap.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kui.wangdashe.top

[Q19] 范围查询
来源：http://vtq.c1oappe.top


<!-- 参考信息 -->