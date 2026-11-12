代发 wailian999

Ruby: exit 1
来源：http://vbo.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gmz.yangfankeji.com

[M06] 向标准错误输出
来源：http://gep.chenlongwang.top

Py:   print("err", file=sys.stderr)
来源：http://ijl.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tqs.uphjek.com

JS:   console.error("err")
来源：http://mqd.ctjpmb.com

TS:   console.error("err")
来源：http://vtd.zhoulong.xyz

Java: System.err.println("err")
来源：http://ugm.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ezr.nanxinkj.top

Ruby: warn "err"
来源：http://zix.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://fll.ppjwa.cn

[M07] 判断是否为主入口
来源：http://osb.yongpay.top

Py:   if __name__ == "__main__":
来源：http://iuj.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fgg.chenjidiqi.icu

JS:   require.main === module
来源：http://hvv.aibaodan.cn

TS:   require.main === module
来源：http://lzt.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://irj.sweek.top

Go:   func main()
来源：http://svo.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wau.zhongyouzk.top

C#:   static void Main(string[] args)
来源：http://ett.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://iqx.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://akp.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://cut.gaohongyu789.top

JS:   process.platform;  process.version
来源：http://gac.hfpthk.cn

TS:   process.platform;  process.version
来源：http://yfv.yongpay.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pqs.uphjek.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://kfs.zhijiandao.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fnx.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hco.guowangkeji.top

================================================================================
来源：http://kul.yfazqb.com

N. 数据结构与算法
来源：http://ahc.yangfankeji.com

================================================================================
来源：http://bqv.zhengqikj.top

[N01] 二分查找（有序数组）
来源：http://nhk.nanxinkj.top

Py:   bisect.bisect_left(arr, x)
来源：http://gfk.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kpp.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rlg.snrcjt.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zdl.havefunace.top

Java: Arrays.binarySearch(arr, x)
来源：http://xlv.gogol.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://ifx.quarkkingdee.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kca.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://ngo.birdmap.top

[N02] 排序（工程实践用内置实现）
来源：http://vgf.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://fcn.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lez.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ohx.jlsjyb.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rgp.chenlongwang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pdj.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://ewa.chenzaomai.com

Ruby: arr.sort
来源：http://qnn.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zgt.zdbjq.cn

[N03] 快速排序（分治示例）
来源：http://fpu.zhoulong.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bbq.jlsjyb.cn

PHP:  // 递归实现，或用 usort
来源：http://cfc.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tmf.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bgv.sxryk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dtn.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mlx.wangshuangyany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lux.dianchejie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rrh.ywan-chungtsiang.top

[N04] 斐波那契数列
来源：http://fjy.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jfv.gzhubu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jgj.nanxuanxn.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hhr.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hex.sxryk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://euw.shanyushiyangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://krq.yj20258.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vsy.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gzj.gotoacloud.top

[N05] 最大公约数
来源：http://fsm.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://tfy.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sbh.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qia.xziqi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nnt.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lgj.ctjpmb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dak.dashuyun.cn

Ruby: a.gcd(b)
来源：http://byz.hnqzz.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ddw.bjfxy.top

[N06] 判断回文字符串
来源：http://hdh.gaohongyu789.top

Py:   s == s[::-1]
来源：http://wly.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://xdu.0kj1m.cn

JS:   s === [...s].reverse().join("")
来源：http://kij.jqgfzy.top

TS:   s === [...s].reverse().join("")
来源：http://vkm.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vvu.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://ncz.shanyushiyangkeji.top

Ruby: s == s.reverse
来源：http://bfc.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://brl.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://jrg.chenzaomai.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://glg.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qam.jianghu66.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jlm.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://nlx.gaohongyu789.top

Java: // 手写 HashMap
来源：http://gmw.cheryme.top

Go:   // 手写 map[int]int
来源：http://xnc.zdbjq.cn

Ruby: // 手写 Hash
来源：http://nnp.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vjd.yuxming.cn

[N08] 生成全排列
来源：http://eqi.xuetiantiany.cn

Py:   itertools.permutations(arr)
来源：http://xbg.gzhubu.top

PHP:  // 手写递归交换
来源：http://duy.guowangkeji.top

JS:   // 手写回溯递归
来源：http://cur.zhoulong.xyz

TS:   // 手写回溯递归
来源：http://czz.mhx1999.top

Java: // 手写回溯递归
来源：http://wvl.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://nua.xinyue.icu

Ruby: arr.permutation.to_a
来源：http://wgf.jiagoushi.top

C#:   // 手写回溯递归
来源：http://xqi.svipenyu.cn

[N09] 栈与队列
来源：http://ioi.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jaj.haohaochexian.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tpa.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tbo.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://irh.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yab.hesvh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vse.hammf.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sbv.zhongyouzk.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jju.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://lcg.quarkkingdee.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cux.xinyue.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://vds.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tes.zhaomingkeji.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lnb.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://poo.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://vrw.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wsx.hesvh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tms.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://vwl.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aen.cheryme.top

PHP:  // 手写递归函数
来源：http://zqs.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://usv.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://crt.bbcook.cn

Java: // 手写递归
来源：http://amd.gotoacloud.top

Go:   // 手写递归
来源：http://ufz.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rkw.jiagoushi.top

C#:   // 手写递归
来源：http://zra.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jcy.kuanghao11.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xaq.sufxvd.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lah.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://klx.nanxinkj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wha.sysykeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nsv.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ljn.shanyushiyangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qjq.hesvh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://egd.hongshengwenyu.top

================================================================================
来源：http://bll.cdnleiting.top

O. 并发与异步
来源：http://kym.hnxiangtu.top

================================================================================
来源：http://nwt.xuetiantiany.cn

[O01] 启动一个线程
来源：http://afc.hongshengwenyu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gpi.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vja.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vvp.jlsjyb.cn

TS:   // 同 JS
来源：http://gwu.xingfuxueyuan.xyz

Java: new Thread(() -> f()).start()
来源：http://hqr.hysaishi.cn

Go:   go f()
来源：http://qlv.fktsv.cn

Ruby: Thread.new { f }
来源：http://hat.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://ctt.epnwcf.com

[O02] 使用线程池
来源：http://ksw.birdmap.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cit.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rej.jyoumei.cn

JS:   // worker_threads 线程池
来源：http://dlp.havefunace.top

TS:   // worker_threads 线程池
来源：http://ouv.vehdjk.com

Java: Executors.newFixedThreadPool(4)
来源：http://qiv.nwbrower.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pnq.316326.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rlz.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mya.tanke756.top

[O03] 加锁保护共享数据
来源：http://eoi.wangdashe.top

Py:   with lock: shared += 1
来源：http://ees.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://wyb.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oen.ctjpmb.com

TS:   // 同 JS
来源：http://kfs.cqqwz.cn

Java: synchronized (this) { shared++; }
来源：http://fgy.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mjc.sjlbkw.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://obk.xuanzx.com

C#:   lock (gate) { shared++; }
来源：http://qdx.meibo888.top

[O04] 定义异步函数并等待
来源：http://rcq.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://hfp.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wxh.cashguo.top

JS:   async function f() { await g(); }
来源：http://ugr.xuetiantiany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tox.nwbrower.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jtf.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vwv.bbcook.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tjy.andypj.xyz

C#:   async Task F() { await G(); }
来源：http://saj.fktsv.cn

[O05] 并发执行并等待全部完成
来源：http://hlm.zhoulong.xyz

Py:   asyncio.gather(*tasks)
来源：http://jmk.52xcode.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rho.ywan-chungtsiang.top

JS:   await Promise.all(tasks)
来源：http://fgj.guowangkeji.top

TS:   await Promise.all(tasks)
来源：http://xpl.guowangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qrs.jinyuanbaomall.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pyo.iojbl.cn

Ruby: threads.map(&:join)
来源：http://mde.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gdc.daria6918.cn

[O06] 使用进程池
来源：http://sxa.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yuw.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uvi.ctjpmb.com

JS:   // child_process / cluster 模块
来源：http://xvx.sufxvd.cn

TS:   // child_process / cluster 模块
来源：http://rrb.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://san.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://inp.hesvh.cn

Ruby: // fork 块
来源：http://uzf.vehdjk.com

C#:   Parallel.For
来源：http://hyy.fengsongda.top

================================================================================
来源：http://nro.fktsv.cn

P. 常用工具函数
来源：http://iqg.aizwys.cn

================================================================================
来源：http://jkv.gzhubu.top

[P01] 生成 UUID
来源：http://qvj.hesvh.cn

Py:   str(uuid.uuid4())
来源：http://ahr.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dkk.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://jat.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://dnb.zhiwuduotai.top

Java: UUID.randomUUID().toString()
来源：http://ssk.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://rzz.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://vpm.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://eke.xziqi.cn

[P02] MD5 / SHA256 摘要
来源：http://xby.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dhl.pengpengdd.cyou

PHP:  hash("sha256", $s);  md5($s);
来源：http://kby.ehwqpu.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://prf.cqqwz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jam.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nfq.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mfc.jianghu66.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qdw.smart0.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mzj.ivvv.top

[P03] 生成短随机字符串
来源：http://dgf.jinghuilouyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zfe.zdqjudy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nlc.guowangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://axv.jqgfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jqg.haohaochexian.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ime.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dfs.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://axn.nanxuanxn.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cst.feifeiyinyue.top

[P04] 求长度
来源：http://apz.ppjwa.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sqo.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bie.dashuyun.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jth.jqgufenzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gcz.xingfuxueyuan.xyz

Java: list.size();  map.size();  s.length()
来源：http://adv.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://rtw.sjlbkw.cn

Ruby: x.length;  x.size
来源：http://wlt.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://eoq.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://sws.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jld.zycfv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xsi.yangfankeji.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qij.zdbjq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://idm.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pun.cheryme.top

Go:   reflect.DeepEqual(a, b)
来源：http://lxb.andypj.xyz

Ruby: a == b
来源：http://mho.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lrs.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://azj.xuetiantiany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qex.ybcxt.top

PHP:  if (empty($x)) {}
来源：http://tjk.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://srt.aibaodan.cn

TS:   if (x == null) {}
来源：http://dcz.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uae.tanke756.top

Go:   if x == nil {}
来源：http://iix.ivvv.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://avl.cucudq.cn

C#:   if (x is null) {}
来源：http://dbk.gogol.net.cn

[P07] 防抖与节流
来源：http://xng.andypj.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aqz.gaohongyu789.top

PHP:  // 手写时间戳比较
来源：http://npu.wangdashe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hur.zhengqikj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tgh.feifeiyinyue.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mja.meibo888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tye.yvedp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vai.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ljk.quarkkingdee.top

[P08] 处理浮点精度问题
来源：http://ddw.yangfankeji.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://std.smart0.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vrj.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zha.shanyushiyangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pog.ywan-chungtsiang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jbt.sweek.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cpu.zycfv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sno.havefunace.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://elp.jlsjyb.cn

================================================================================
来源：http://ric.chenlongwang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fki.shanyushiyangtech.top

================================================================================
来源：http://kuy.daria6918.cn

[Q01] 创建表
来源：http://crn.vehdjk.com

CREATE TABLE users (
来源：http://dot.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://doz.yangfankeji.com

name VARCHAR(50) NOT NULL,
来源：http://qid.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://hmw.fktsv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://moi.nanxuanxn.top

);
来源：http://vpv.hywenlv.cn

[Q02] 创建带外键的表
来源：http://yep.shanyushiyangtech.top

CREATE TABLE orders (
来源：http://hbs.wangdashe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ydk.jinqigufen.top

user_id INT NOT NULL,
来源：http://mdd.andypj.xyz

amount DECIMAL(10, 2),
来源：http://hqc.ehwqpu.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gmm.gzhubu.top

);
来源：http://bjk.iojbl.cn

[Q03] 增加列
来源：http://jgg.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://all.pycfn.com

[Q04] 修改列类型
来源：http://tvh.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fon.zdqjudy.top

[Q05] 重命名列
来源：http://gvn.zhoulong.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fld.epnwcf.com

[Q06] 删除列
来源：http://mew.cqqwz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://njx.aibaodan.cn

[Q07] 删除表
来源：http://bng.tarul.cn

DROP TABLE IF EXISTS orders;
来源：http://jyk.cqqwz.cn

[Q08] 创建普通索引
来源：http://tgn.kuanghao11.cn


<!-- 参考信息 -->