代发 wailian999

TS:   process.cwd()
来源：http://gla.jqgufenzy.top

Java: Path.of("").toAbsolutePath()
来源：http://xiz.yj202588.top

Go:   os.Getwd()
来源：http://msm.epnwcf.com

Ruby: Dir.pwd
来源：http://kfl.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://qgz.bjfxy.top

[M05] 设置退出码
来源：http://hub.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://cyz.dianchejie.cn

PHP:  exit(1);
来源：http://edg.shuidangran.top

JS:   process.exit(1)
来源：http://fsh.c1oappe.top

TS:   process.exit(1)
来源：http://tbn.yj20258888.top

Java: System.exit(1)
来源：http://jzl.hywenlv.cn

Go:   os.Exit(1)
来源：http://vzw.hongshengwenyu.top

Ruby: exit 1
来源：http://rhe.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dty.zhoulong.xyz

[M06] 向标准错误输出
来源：http://mdz.yangfankeji.com

Py:   print("err", file=sys.stderr)
来源：http://fzv.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mwi.svipenyu.cn

JS:   console.error("err")
来源：http://rxm.sweek.top

TS:   console.error("err")
来源：http://ipl.dianchejie.cn

Java: System.err.println("err")
来源：http://ehj.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ern.yfazqb.com

Ruby: warn "err"
来源：http://ojx.wangshuangyany.cn

C#:   Console.Error.WriteLine("err")
来源：http://gsr.xinyue.icu

[M07] 判断是否为主入口
来源：http://acq.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://nem.gogol.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://skd.chenzaomai.com

JS:   require.main === module
来源：http://utk.xylfe.cn

TS:   require.main === module
来源：http://vjn.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://uwb.birdmap.top

Go:   func main()
来源：http://jgj.nanxinkj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oqm.zdqjudy.top

C#:   static void Main(string[] args)
来源：http://pkn.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://yqo.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://wnm.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://enr.fktsv.cn

JS:   process.platform;  process.version
来源：http://yys.fktsv.cn

TS:   process.platform;  process.version
来源：http://wyt.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://emh.epnwcf.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://uwl.epnwcf.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wrs.haohaochexian.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://knq.jinqigfzy.top

================================================================================
来源：http://syr.yj20258888.top

N. 数据结构与算法
来源：http://jis.ywan-chungtsiang.top

================================================================================
来源：http://zlp.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://jkh.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://dbj.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hgy.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://icb.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fpe.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://qcv.havefunace.top

Go:   sort.SearchInts(arr, x)
来源：http://ilv.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jml.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zpa.hesvh.cn

[N02] 排序（工程实践用内置实现）
来源：http://ugr.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://ivw.birdmap.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://knm.yuxming.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zca.hywenlv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ati.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xlk.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://gud.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://iht.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://imn.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://gbf.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qzg.hnxiangtu.top

PHP:  // 递归实现，或用 usort
来源：http://vtr.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://etk.zhoulong.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://llg.ydzc1.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zth.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hyk.guowangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lty.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://udn.uphjek.com

[N04] 斐波那契数列
来源：http://qei.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qfb.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hhx.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rzh.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ezh.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cvh.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oxq.tarul.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://utq.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qmm.yongpay.top

[N05] 最大公约数
来源：http://trz.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://dtr.xuetiantiany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hiz.hongshengwenyu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gaq.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zki.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xyd.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lcv.yangfankeji.com

Ruby: a.gcd(b)
来源：http://idv.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://obv.uphjek.com

[N06] 判断回文字符串
来源：http://kwz.pycfn.com

Py:   s == s[::-1]
来源：http://cla.yonumen.top

PHP:  $s === strrev($s);
来源：http://fyp.yuanzhike.top

JS:   s === [...s].reverse().join("")
来源：http://etg.xuetiantiany.cn

TS:   s === [...s].reverse().join("")
来源：http://gqj.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xfj.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://vna.dianchejie.cn

Ruby: s == s.reverse
来源：http://gzp.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ylx.yongpay.top

[N07] 两数之和（返回下标）
来源：http://ahb.zdqjudy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xiv.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eqd.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nii.gogol.net.cn

TS:   // 手写 Map<string, number>
来源：http://sao.jqgfzy.top

Java: // 手写 HashMap
来源：http://jes.redwolf501.top

Go:   // 手写 map[int]int
来源：http://mdq.zhengqikj.top

Ruby: // 手写 Hash
来源：http://evi.hnxiangtu.top

C#:   // 手写 Dictionary<int, int>
来源：http://rdu.hammf.cn

[N08] 生成全排列
来源：http://htw.yfazqb.com

Py:   itertools.permutations(arr)
来源：http://tac.feifeiyinyue.top

PHP:  // 手写递归交换
来源：http://ljn.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://csz.guowangkeji.top

TS:   // 手写回溯递归
来源：http://vvh.aizwys.cn

Java: // 手写回溯递归
来源：http://brf.nwbrower.top

Go:   // 手写回溯递归
来源：http://wdl.cdnleiting.top

Ruby: arr.permutation.to_a
来源：http://igb.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://foc.fanxiaobao.xyz

[N09] 栈与队列
来源：http://mqn.daxiang520.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tyd.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dmd.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://std.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mun.hcnkem.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mxt.yongpay.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vqa.jyoumei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oii.hysaishi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uuu.zhoulong.xyz

[N10] 链表节点定义
来源：http://wqi.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cwn.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://sxy.hesvh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ebr.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://arr.svipenyu.cn

Java: class Node { int v; Node next; }
来源：http://ndw.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://lsz.wangshuangyany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eqa.ydjk.org.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://icb.daxiang520.top

[N11] 二叉树中序遍历
来源：http://qha.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tib.fktsv.cn

PHP:  // 手写递归函数
来源：http://ivl.tianlin.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uxn.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://edi.tianlin.xyz

Java: // 手写递归
来源：http://iul.cdnleiting.top

Go:   // 手写递归
来源：http://zsf.sjlbkw.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://amm.snrcjt.cn

C#:   // 手写递归
来源：http://flp.hongshengwenyu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nbo.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://esg.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bna.hongshengwenyu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vlh.daxiang520.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cib.yuanzhike.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nrs.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ypf.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xfq.smart0.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://szv.yuxming.cn

================================================================================
来源：http://lxn.52xcode.cn

O. 并发与异步
来源：http://zvl.yvedp.cn

================================================================================
来源：http://crg.daxiang520.top

[O01] 启动一个线程
来源：http://mpn.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dbn.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rlz.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wim.shanyushiyangtech.top

TS:   // 同 JS
来源：http://zbi.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://qzo.hesvh.cn

Go:   go f()
来源：http://viq.xziqi.cn

Ruby: Thread.new { f }
来源：http://ebv.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://ubr.dianchejie.cn

[O02] 使用线程池
来源：http://tmy.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cft.shanyushiyangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gjt.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://ooc.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://jfp.yfazqb.com

Java: Executors.newFixedThreadPool(4)
来源：http://efo.zhengqikj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rxy.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kqg.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vaf.hesvh.cn

[O03] 加锁保护共享数据
来源：http://cbu.zhengqikj.top

Py:   with lock: shared += 1
来源：http://txd.dianchejie.cn

PHP:  // 用 flock() 做文件锁
来源：http://wgg.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mie.ppjwa.cn

TS:   // 同 JS
来源：http://dii.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://eip.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fpm.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ill.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://ilt.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://cyu.pengpengdd.cyou

Py:   async def f():⏎    await g()
来源：http://mpy.hnqzz.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ajb.sxryk.cn

JS:   async function f() { await g(); }
来源：http://drk.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://rww.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oct.nanxuanxn.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ref.zhengqikj.top

Ruby: # 用 Fiber 或 async gem
来源：http://dea.svipenyu.cn

C#:   async Task F() { await G(); }
来源：http://bjk.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://you.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://hcv.nanxuanxn.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lem.zhixingplan.top

JS:   await Promise.all(tasks)
来源：http://tby.hfpthk.cn

TS:   await Promise.all(tasks)
来源：http://him.fengsongda.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wcy.aizwys.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ptt.yonumen.top

Ruby: threads.map(&:join)
来源：http://qdd.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://cai.yj202588.top

[O06] 使用进程池
来源：http://bzd.tianlin.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://quv.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zod.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://hgj.snrcjt.cn

TS:   // child_process / cluster 模块
来源：http://emj.wangshuangyany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qsw.zhengqikj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jgh.guowangkeji.top

Ruby: // fork 块
来源：http://prh.aizwys.cn

C#:   Parallel.For
来源：http://yqw.dashuyun.cn

================================================================================
来源：http://mof.xinyue.icu

P. 常用工具函数
来源：http://zzu.sufxvd.cn

================================================================================
来源：http://cak.smart0.xyz

[P01] 生成 UUID
来源：http://kdp.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://cil.sysykeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gbg.yueranfly.top

JS:   crypto.randomUUID()
来源：http://oqq.xingfuxueyuan.xyz

TS:   crypto.randomUUID()
来源：http://lvb.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://epl.sxryk.cn

Go:   // 用 github.com/google/uuid
来源：http://xiy.nanxuanxn.top

Ruby: SecureRandom.uuid
来源：http://jdm.shangyingyoupin.top

C#:   Guid.NewGuid().ToString()
来源：http://yjg.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://nwe.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pms.feifeiyinyue.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kfy.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uwx.yj20258888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dms.yj20258.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fbj.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qbj.andypj.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tmj.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fgk.chenjidiqi.icu

[P03] 生成短随机字符串
来源：http://ijc.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rqf.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xcx.yonumen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ert.mhx1999.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dna.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vlz.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ebc.shanyushiyangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lmm.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://poe.feifeiyinyue.top

[P04] 求长度
来源：http://zqt.pengpengdd.cyou

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eog.tianlin.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://phg.gaohongyu789.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wbj.yj20258.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gmz.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://dud.dianchejie.cn

Go:   len(arr);  len(m)
来源：http://zif.cheryme.top

Ruby: x.length;  x.size
来源：http://tkw.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gnk.zdqjudy.top

[P05] 判断两个对象内容是否相等
来源：http://phx.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lev.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ckz.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kos.tianlin.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kfk.pycfn.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sbc.yj202588.top

Go:   reflect.DeepEqual(a, b)
来源：http://qsh.zhoulong.xyz

Ruby: a == b
来源：http://wig.dianchejie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qrx.havefunace.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tfv.hysaishi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oya.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://clm.gaohongyu789.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gyw.yonumen.top

TS:   if (x == null) {}
来源：http://urj.jlsjyb.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://aun.hongshengwenyu.top

Go:   if x == nil {}
来源：http://hsn.jqgufenzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bcg.shanyushiyangkeji.top

C#:   if (x is null) {}
来源：http://fmv.hammf.cn

[P07] 防抖与节流
来源：http://vzt.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://akw.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://vpf.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cdv.iojbl.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kep.ydzc1.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dkr.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bre.zhongyouzk.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://edq.9152youxi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://okx.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://mxb.chenzaomai.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iag.fanxiaobao.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rzj.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oox.xziqi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jxw.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zfv.sysykeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wrm.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aqi.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vap.aibaodan.cn

================================================================================
来源：http://vgg.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://edw.bbcook.cn

================================================================================
来源：http://yjo.havefunace.top

[Q01] 创建表
来源：http://jqb.zdqjudy.top

CREATE TABLE users (
来源：http://tse.daxiang520.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ssi.zhoulong.xyz

name VARCHAR(50) NOT NULL,
来源：http://bee.pycfn.com

email VARCHAR(100) UNIQUE,
来源：http://caw.cqqwz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vqt.jiagoushi.top

);
来源：http://qwf.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://lax.vqdsnc.cn

CREATE TABLE orders (
来源：http://ooc.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vbq.yuxming.cn

user_id INT NOT NULL,
来源：http://ygs.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://osa.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zcn.zdqjudy.top


<!-- 参考信息 -->