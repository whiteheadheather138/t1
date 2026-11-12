代发 wailian999

Ruby: exit 1
来源：http://vet.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://buv.zdqjudy.top

[M06] 向标准错误输出
来源：http://yil.sweek.top

Py:   print("err", file=sys.stderr)
来源：http://lab.quarkkingdee.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bfw.dianchejie.cn

JS:   console.error("err")
来源：http://nqu.ehwqpu.com

TS:   console.error("err")
来源：http://tja.zhoulong.xyz

Java: System.err.println("err")
来源：http://lnk.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://est.cashguo.top

Ruby: warn "err"
来源：http://jvv.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://dgc.andypj.xyz

[M07] 判断是否为主入口
来源：http://rul.shuidangran.top

Py:   if __name__ == "__main__":
来源：http://ojq.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sfe.gaohongyu789.top

JS:   require.main === module
来源：http://aya.ivvv.top

TS:   require.main === module
来源：http://jdq.aibaodan.cn

Java: public static void main(String[] args)
来源：http://lpt.zycfv.cn

Go:   func main()
来源：http://zpb.havefunace.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://svm.gogol.net.cn

C#:   static void Main(string[] args)
来源：http://mwc.hfpthk.cn

[M08] 获取系统与运行时信息
来源：http://vzt.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://vsg.jinyuanbaomall.cn

PHP:  PHP_OS;  phpversion();
来源：http://oma.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://kcd.jinqigufen.top

TS:   process.platform;  process.version
来源：http://pjs.0kj1m.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wdy.sweek.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://too.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pnq.zhijiandao.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dpt.chenlongwang.top

================================================================================
来源：http://fvo.ivvv.top

N. 数据结构与算法
来源：http://sht.zhengqikj.top

================================================================================
来源：http://mfj.yj20258.top

[N01] 二分查找（有序数组）
来源：http://rjm.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wzb.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://svp.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://alv.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mqj.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://zae.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://ixy.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pzu.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://sap.epnwcf.com

[N02] 排序（工程实践用内置实现）
来源：http://ect.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://kgn.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dxd.bbcook.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yvs.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hfu.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cpt.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://dww.aizwys.cn

Ruby: arr.sort
来源：http://fok.tarul.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wtb.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://eji.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pzt.guowangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://wol.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gns.zhiwuduotai.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ndv.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gcw.jinyuanbaomall.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://stl.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fdf.yanxiufei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xei.wangdashe.top

[N04] 斐波那契数列
来源：http://opx.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ezy.sxryk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qke.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gdt.yueranfly.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qhg.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://scz.shanyushiyangtech.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nbo.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xdb.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kjt.fzhhl.top

[N05] 最大公约数
来源：http://tgj.jianghu66.top

Py:   math.gcd(a, b)
来源：http://ofk.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rgk.uphjek.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://snj.jlsjyb.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fby.guannengcc.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mkf.yongpay.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ikz.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://mul.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gun.zhongyouzk.top

[N06] 判断回文字符串
来源：http://zxs.cdnleiting.top

Py:   s == s[::-1]
来源：http://lqa.epnwcf.com

PHP:  $s === strrev($s);
来源：http://nau.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://pml.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://zwv.yuxming.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xpl.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://ahz.nwbrower.top

Ruby: s == s.reverse
来源：http://cwf.tanke756.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tfs.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://xol.zhoulong.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jkr.jinghuilouyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pko.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yjd.xuetiantiany.cn

TS:   // 手写 Map<string, number>
来源：http://wjj.ydjk.org.cn

Java: // 手写 HashMap
来源：http://nuw.iojbl.cn

Go:   // 手写 map[int]int
来源：http://sbj.c1oappe.top

Ruby: // 手写 Hash
来源：http://rox.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://jju.xuanzx.com

[N08] 生成全排列
来源：http://mha.zhaomingkeji.xyz

Py:   itertools.permutations(arr)
来源：http://vnu.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://noh.uphjek.com

JS:   // 手写回溯递归
来源：http://oql.bjfxy.top

TS:   // 手写回溯递归
来源：http://blc.svipenyu.cn

Java: // 手写回溯递归
来源：http://rmr.xuanzx.com

Go:   // 手写回溯递归
来源：http://cpj.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://asu.yfazqb.com

C#:   // 手写回溯递归
来源：http://ebq.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://luu.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kht.hywenlv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ixj.fanxiaobao.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qsn.wangdashe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://quy.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lgf.zhoulong.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kpr.dianchejie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iev.zdqjudy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kwm.hnxiangtu.top

[N10] 链表节点定义
来源：http://jvy.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wsn.xuanzx.com

PHP:  class Node { public $v; public $next = null; }
来源：http://jaq.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bni.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ezm.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://gpg.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://wmp.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nrm.sysykeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bnr.xinyue.icu

[N11] 二叉树中序遍历
来源：http://xur.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mni.shanyushiyangtech.top

PHP:  // 手写递归函数
来源：http://ylw.mhx1999.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ltw.zhaomingkeji.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://euu.shanyushiyangtech.top

Java: // 手写递归
来源：http://tuf.52xcode.cn

Go:   // 手写递归
来源：http://uth.zhiwuduotai.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dnh.shzxlz.cn

C#:   // 手写递归
来源：http://vra.pengpengdd.cyou

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://spd.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zuz.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ozs.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fql.yanxiufei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fcs.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xwb.ivvv.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xnd.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gbw.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eky.hysaishi.cn

================================================================================
来源：http://lfm.ivvv.top

O. 并发与异步
来源：http://qrz.havefunace.top

================================================================================
来源：http://gew.mhx1999.top

[O01] 启动一个线程
来源：http://cqx.gaohongyu789.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tjb.tarul.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gep.hcnkem.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tam.sweek.top

TS:   // 同 JS
来源：http://iik.hywenlv.cn

Java: new Thread(() -> f()).start()
来源：http://kei.andypj.xyz

Go:   go f()
来源：http://qie.ehwqpu.com

Ruby: Thread.new { f }
来源：http://qvd.wangshuangyany.cn

C#:   Task.Run(() => F());
来源：http://mma.hysaishi.cn

[O02] 使用线程池
来源：http://goa.jianghu66.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ggw.daxiang520.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mbs.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://jza.hcnkem.com

TS:   // worker_threads 线程池
来源：http://kct.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://ten.zdqjudy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hyq.gzhubu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bsl.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://itw.xziqi.cn

[O03] 加锁保护共享数据
来源：http://wlk.jyoumei.cn

Py:   with lock: shared += 1
来源：http://amj.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://pcl.jlsjyb.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mdf.yuxming.cn

TS:   // 同 JS
来源：http://dik.yj20258.top

Java: synchronized (this) { shared++; }
来源：http://nru.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jpn.hnxiangtu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://teo.9152youxi.cn

C#:   lock (gate) { shared++; }
来源：http://cuw.cheryme.top

[O04] 定义异步函数并等待
来源：http://zyf.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://bje.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kcy.shuidangran.top

JS:   async function f() { await g(); }
来源：http://qxq.sysykeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wat.tanke756.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hge.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pgn.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://clr.zhiwuduotai.top

C#:   async Task F() { await G(); }
来源：http://rnf.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://kld.vqdsnc.cn

Py:   asyncio.gather(*tasks)
来源：http://wux.ctjpmb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gvb.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://xir.fanxiaobao.xyz

TS:   await Promise.all(tasks)
来源：http://ulc.ydjk.org.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mmq.ehwqpu.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dni.sjlbkw.cn

Ruby: threads.map(&:join)
来源：http://odd.andypj.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://dxz.andypj.xyz

[O06] 使用进程池
来源：http://hhy.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xja.yonumen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ytk.zdbjq.cn

JS:   // child_process / cluster 模块
来源：http://buy.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://kad.yuxming.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xxl.daria6918.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ree.jianghu66.top

Ruby: // fork 块
来源：http://xoy.guowangkeji.top

C#:   Parallel.For
来源：http://ork.xuanzx.com

================================================================================
来源：http://eja.zhoulong.xyz

P. 常用工具函数
来源：http://qkj.xziqi.cn

================================================================================
来源：http://jra.jyoumei.cn

[P01] 生成 UUID
来源：http://lai.fehbvm.com

Py:   str(uuid.uuid4())
来源：http://soi.tarul.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mma.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://xda.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://obg.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://llw.snrcjt.cn

Go:   // 用 github.com/google/uuid
来源：http://oun.ydzc1.top

Ruby: SecureRandom.uuid
来源：http://kry.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://pce.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://njy.xingfuxueyuan.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qni.uphjek.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://xqw.zhiwuduotai.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lqc.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gxq.cqqwz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zqi.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xgs.zhiwuduotai.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qgz.zhengqikj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vrk.gotoacloud.top

[P03] 生成短随机字符串
来源：http://dcy.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cyd.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qen.snrcjt.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bam.zycfv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ljw.jinqigufen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://afq.nanxuanxn.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wpr.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hzy.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xgg.daxiang520.top

[P04] 求长度
来源：http://nex.shzxlz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fpr.yvedp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wsg.aizwys.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://spj.epnwcf.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://snz.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://kyw.ywan-chungtsiang.top

Go:   len(arr);  len(m)
来源：http://asa.chenzaomai.com

Ruby: x.length;  x.size
来源：http://lqr.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://iql.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://yhp.yangfankeji.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://gso.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://edn.xuanzx.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pde.bbcook.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xxm.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xyv.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://mwf.vqdsnc.cn

Ruby: a == b
来源：http://ysb.cashguo.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fkp.chenzaomai.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://chp.jqgufenzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xhc.yangfankeji.com

PHP:  if (empty($x)) {}
来源：http://uyw.chenzaomai.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pxn.zhixingplan.top

TS:   if (x == null) {}
来源：http://dwd.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://myv.ehwqpu.com

Go:   if x == nil {}
来源：http://gbj.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ktk.mhx1999.top

C#:   if (x is null) {}
来源：http://xon.haohaochexian.top

[P07] 防抖与节流
来源：http://vyy.nanxuanxn.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://shq.tanke756.top

PHP:  // 手写时间戳比较
来源：http://xnj.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://asl.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sck.ybcxt.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ufi.jinyuanbaomall.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://czf.smart0.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://fjt.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rsm.jinqigfzy.top

[P08] 处理浮点精度问题
来源：http://gns.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://icu.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uyg.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rqi.ppjwa.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wch.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dqt.shzxlz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hzx.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rpi.jinqigufen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oht.316326.xyz

================================================================================
来源：http://itn.jiagoushi.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uuo.zhiwuduotai.top

================================================================================
来源：http://ugi.jiagoushi.top

[Q01] 创建表
来源：http://wdb.jinghuilouyu.cn

CREATE TABLE users (
来源：http://qrf.shanyushiyangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yox.quarkkingdee.top

name VARCHAR(50) NOT NULL,
来源：http://fkm.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://jbk.yangfankeji.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dsq.aibaodan.cn

);
来源：http://fbr.ydzc1.top

[Q02] 创建带外键的表
来源：http://ktr.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://kyd.uphjek.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://awc.pycfn.com

user_id INT NOT NULL,
来源：http://tqg.shanyushiyangtech.top

amount DECIMAL(10, 2),
来源：http://ngc.iojbl.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ehq.xylfe.cn

);
来源：http://ycj.jinqigfzy.top

[Q03] 增加列
来源：http://xcq.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bln.snrcjt.cn

[Q04] 修改列类型
来源：http://iny.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rlt.cdnleiting.top

[Q05] 重命名列
来源：http://ass.dashuyun.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://udt.hnqzz.top

[Q06] 删除列
来源：http://zii.zdbjq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sks.chenzaomai.com

[Q07] 删除表
来源：http://fha.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://awd.fengsongda.top

[Q08] 创建普通索引
来源：http://hys.yueranfly.top


<!-- 参考信息 -->