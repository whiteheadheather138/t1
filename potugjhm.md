代发 wailian999

Py:   if __name__ == "__main__":
来源：http://gjo.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gle.hywenlv.cn

JS:   require.main === module
来源：http://kqt.chenlongwang.top

TS:   require.main === module
来源：http://ywz.hnxiangtu.top

Java: public static void main(String[] args)
来源：http://djj.ivvv.top

Go:   func main()
来源：http://ifs.tianlin.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mra.jianghu66.top

C#:   static void Main(string[] args)
来源：http://dyo.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://vtt.nanxinkj.top

Py:   platform.system();  platform.python_version()
来源：http://oea.jiagoushi.top

PHP:  PHP_OS;  phpversion();
来源：http://rhk.haohaochexian.top

JS:   process.platform;  process.version
来源：http://zax.svipenyu.cn

TS:   process.platform;  process.version
来源：http://cgq.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tqh.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wqa.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kxc.wangshuangyany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kip.cashguo.top

================================================================================
来源：http://uhc.zhoulong.xyz

N. 数据结构与算法
来源：http://zmz.yanxiufei.cn

================================================================================
来源：http://gud.sweek.top

[N01] 二分查找（有序数组）
来源：http://wux.ctjpmb.com

Py:   bisect.bisect_left(arr, x)
来源：http://gpt.guowangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kzu.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wcm.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ikj.zhoulong.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://uea.cqqwz.cn

Go:   sort.SearchInts(arr, x)
来源：http://vlk.fzhhl.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://irf.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://qoh.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://lnm.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://wda.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yhp.daxiang520.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jfj.nanxinkj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rlp.ppjwa.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ebz.aizwys.cn

Go:   slices.Sort(arr)
来源：http://pse.ctjpmb.com

Ruby: arr.sort
来源：http://dzp.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mne.mhx1999.top

[N03] 快速排序（分治示例）
来源：http://fsd.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vma.jiagoushi.top

PHP:  // 递归实现，或用 usort
来源：http://xuc.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pwg.feifeiyinyue.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rkg.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zbm.cqqwz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://smj.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oei.fzhhl.top

C#:   // 手写递归，或 Array.Sort
来源：http://rbp.andypj.xyz

[N04] 斐波那契数列
来源：http://ond.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fks.shzxlz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kqh.xuetiantiany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wzs.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uls.fktsv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gbz.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://can.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://onm.hnqzz.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ywv.ppjwa.cn

[N05] 最大公约数
来源：http://hjv.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://xcs.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://czy.jiagoushi.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://evc.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xcr.cheryme.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uog.fzhhl.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jkw.zhongyouzk.top

Ruby: a.gcd(b)
来源：http://buu.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nxj.316326.xyz

[N06] 判断回文字符串
来源：http://pos.yvedp.cn

Py:   s == s[::-1]
来源：http://its.cqqwz.cn

PHP:  $s === strrev($s);
来源：http://yaf.shanyushiyangtech.top

JS:   s === [...s].reverse().join("")
来源：http://tdx.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://ktk.yonumen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ihu.hnqzz.top

Go:   // 双指针从两端比较
来源：http://lrb.cqqwz.cn

Ruby: s == s.reverse
来源：http://aqe.ydzc1.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://euo.hnxiangtu.top

[N07] 两数之和（返回下标）
来源：http://tok.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hnn.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hra.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vuc.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://elg.nwbrower.top

Java: // 手写 HashMap
来源：http://npz.vqdsnc.cn

Go:   // 手写 map[int]int
来源：http://iel.wangdashe.top

Ruby: // 手写 Hash
来源：http://bdd.shanyushiyangtech.top

C#:   // 手写 Dictionary<int, int>
来源：http://les.yvedp.cn

[N08] 生成全排列
来源：http://nra.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://occ.tarul.cn

PHP:  // 手写递归交换
来源：http://cvr.shuidangran.top

JS:   // 手写回溯递归
来源：http://flx.zhengqikj.top

TS:   // 手写回溯递归
来源：http://hjl.hcnkem.com

Java: // 手写回溯递归
来源：http://rfw.wangshuangyany.cn

Go:   // 手写回溯递归
来源：http://rlo.zycfv.cn

Ruby: arr.permutation.to_a
来源：http://xgj.yfazqb.com

C#:   // 手写回溯递归
来源：http://xwu.yanxiufei.cn

[N09] 栈与队列
来源：http://jda.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qdf.tanke756.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jib.yonumen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jty.shzxlz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vua.yj20258888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vrp.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ywe.bjfxy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jrq.vqdsnc.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dlf.zhixingplan.top

[N10] 链表节点定义
来源：http://zma.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ryd.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uhi.yuxming.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yza.jinqigfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hsr.chenjidiqi.icu

Java: class Node { int v; Node next; }
来源：http://uam.svipenyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qxo.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ukk.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://idg.cqqwz.cn

[N11] 二叉树中序遍历
来源：http://iee.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dem.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://pog.52xcode.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hvx.tarul.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rdz.xziqi.cn

Java: // 手写递归
来源：http://ssq.dianchejie.cn

Go:   // 手写递归
来源：http://tzx.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jel.cashguo.top

C#:   // 手写递归
来源：http://boo.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iuc.cashguo.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dyz.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nkv.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yva.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wqm.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zux.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wfi.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yes.hammf.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mds.zhiwuduotai.top

================================================================================
来源：http://uvb.mhx1999.top

O. 并发与异步
来源：http://xgf.fzhhl.top

================================================================================
来源：http://igt.nwbrower.top

[O01] 启动一个线程
来源：http://yny.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://brr.zycfv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qwp.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qgb.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://qvr.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://iim.chenjidiqi.icu

Go:   go f()
来源：http://qni.cdnleiting.top

Ruby: Thread.new { f }
来源：http://nkg.tarul.cn

C#:   Task.Run(() => F());
来源：http://img.fzhhl.top

[O02] 使用线程池
来源：http://fqc.jqgfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xam.cashguo.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hum.zhiwuduotai.top

JS:   // worker_threads 线程池
来源：http://wgz.aizwys.cn

TS:   // worker_threads 线程池
来源：http://ftf.316326.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://tsd.svipenyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://viu.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yiy.tarul.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bfi.pengpengdd.cyou

[O03] 加锁保护共享数据
来源：http://fxz.vqdsnc.cn

Py:   with lock: shared += 1
来源：http://xsw.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://pix.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ayb.yanxiufei.cn

TS:   // 同 JS
来源：http://aaq.shzxlz.cn

Java: synchronized (this) { shared++; }
来源：http://mgz.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tfw.hesvh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ipy.kuanghao11.cn

C#:   lock (gate) { shared++; }
来源：http://ldy.hfpthk.cn

[O04] 定义异步函数并等待
来源：http://tzv.yj20258888.top

Py:   async def f():⏎    await g()
来源：http://eor.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tan.gaohongyu789.top

JS:   async function f() { await g(); }
来源：http://mzf.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dmw.haohaochexian.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zfc.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ceq.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://zfj.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://adx.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://avu.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://tsp.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gqa.ywan-chungtsiang.top

JS:   await Promise.all(tasks)
来源：http://aql.epnwcf.com

TS:   await Promise.all(tasks)
来源：http://tpt.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mqg.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://crf.meibo888.top

Ruby: threads.map(&:join)
来源：http://smq.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ten.guowangkeji.top

[O06] 使用进程池
来源：http://tyo.cheryme.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bxy.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bqm.tian-w.cn

JS:   // child_process / cluster 模块
来源：http://tvg.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://bng.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://aue.feifeiyinyue.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dsj.xuanzx.com

Ruby: // fork 块
来源：http://pgv.0kj1m.cn

C#:   Parallel.For
来源：http://hcx.tarul.cn

================================================================================
来源：http://jkq.cdnleiting.top

P. 常用工具函数
来源：http://btl.shangyingyoupin.top

================================================================================
来源：http://jgu.chenzaomai.com

[P01] 生成 UUID
来源：http://zns.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://ica.kuanghao11.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bgn.tanke756.top

JS:   crypto.randomUUID()
来源：http://uzk.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://zlj.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://noj.jiagoushi.top

Go:   // 用 github.com/google/uuid
来源：http://hjf.mhx1999.top

Ruby: SecureRandom.uuid
来源：http://jqr.uphjek.com

C#:   Guid.NewGuid().ToString()
来源：http://fce.tarul.cn

[P02] MD5 / SHA256 摘要
来源：http://iyu.cdnleiting.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oiz.smart0.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://qfj.redwolf501.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rih.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ctz.yangfankeji.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://igf.hesvh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://isn.ydzc1.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://unl.smart0.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fha.vqdsnc.cn

[P03] 生成短随机字符串
来源：http://hry.svipenyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qlj.gotoacloud.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rvm.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ulp.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nru.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gpo.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://omm.zhongyouzk.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://unr.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cwm.hongshengwenyu.top

[P04] 求长度
来源：http://ltg.xuanzx.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xur.ywan-chungtsiang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rrg.bjfxy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://agz.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tuz.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://bfa.hysaishi.cn

Go:   len(arr);  len(m)
来源：http://hmm.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://sxe.sjlbkw.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://shl.ywan-chungtsiang.top

[P05] 判断两个对象内容是否相等
来源：http://gab.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sxa.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qrd.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zow.9152youxi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dmh.hysaishi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iku.zhoulong.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://lcl.quarkkingdee.top

Ruby: a == b
来源：http://jpc.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tjs.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vhn.yongpay.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wct.yongpay.top

PHP:  if (empty($x)) {}
来源：http://met.feifeiyinyue.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hdl.andypj.xyz

TS:   if (x == null) {}
来源：http://byv.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bog.fzhhl.top

Go:   if x == nil {}
来源：http://axk.jinyuanbaomall.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wbc.yuanzhike.top

C#:   if (x is null) {}
来源：http://vxy.aizwys.cn

[P07] 防抖与节流
来源：http://rnw.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rgy.ydzc1.top

PHP:  // 手写时间戳比较
来源：http://osq.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hcf.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xet.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://glk.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nuv.c1oappe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cry.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fri.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://dcl.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://izs.cqqwz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mhy.jinqigufen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zmn.fengsongda.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mdp.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ayg.iojbl.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zbj.jinqigfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gks.cqqwz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xfg.hongshengwenyu.top

================================================================================
来源：http://pnp.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mpx.shanyushiyangkeji.top

================================================================================
来源：http://ksl.shuidangran.top

[Q01] 创建表
来源：http://opv.zhiwuduotai.top

CREATE TABLE users (
来源：http://wpg.xingfuxueyuan.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://slv.tianlin.xyz

name VARCHAR(50) NOT NULL,
来源：http://ccz.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://jqf.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ule.iojbl.cn

);
来源：http://omz.yj20258888.top

[Q02] 创建带外键的表
来源：http://fou.zycfv.cn

CREATE TABLE orders (
来源：http://djv.zhoulong.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lxu.zdbjq.cn

user_id INT NOT NULL,
来源：http://sio.cqqwz.cn

amount DECIMAL(10, 2),
来源：http://uhq.vehdjk.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ryc.jyoumei.cn

);
来源：http://jfn.nanxuanxn.top

[Q03] 增加列
来源：http://kqm.sysykeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cvg.jinqigfzy.top

[Q04] 修改列类型
来源：http://tcq.zhaomingkeji.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mme.cdnleiting.top

[Q05] 重命名列
来源：http://jvo.hnqzz.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gfz.fzhhl.top

[Q06] 删除列
来源：http://qmi.zycfv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rwe.tian-w.cn

[Q07] 删除表
来源：http://rio.havefunace.top

DROP TABLE IF EXISTS orders;
来源：http://gmp.sufxvd.cn

[Q08] 创建普通索引
来源：http://ufr.zhiwuduotai.top

CREATE INDEX idx_users_email ON users(email);
来源：http://eck.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://vic.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mbu.pengpengdd.cyou

[Q10] 插入单行
来源：http://qzt.tianlin.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://odr.kuanghao11.cn

[Q11] 一次插入多行
来源：http://gkl.dianchejie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gan.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://mat.guowangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://ipk.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lgj.ybcxt.top

[Q13] 忽略重复插入
来源：http://zoi.kuanghao11.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rnv.ppjwa.cn


<!-- 参考信息 -->