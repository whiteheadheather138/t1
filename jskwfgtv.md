代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bik.0kj1m.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gjh.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://slm.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://djz.tanke756.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qlc.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lpj.gzhubu.top

Ruby: system("ls -l");  `ls -l`
来源：http://foh.zhixingplan.top

C#:   Process.Start("ls", "-l");
来源：http://ldp.hcnkem.com

[M04] 获取当前工作目录
来源：http://yym.pengpengdd.cyou

Py:   os.getcwd()
来源：http://fdi.guowangkeji.top

PHP:  getcwd();
来源：http://nsd.shangyingyoupin.top

JS:   process.cwd()
来源：http://prp.9152youxi.cn

TS:   process.cwd()
来源：http://chb.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://sgx.jinghuilouyu.cn

Go:   os.Getwd()
来源：http://vjc.guowangkeji.top

Ruby: Dir.pwd
来源：http://dpx.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://qpd.gzhubu.top

[M05] 设置退出码
来源：http://rmr.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://yhd.svipenyu.cn

PHP:  exit(1);
来源：http://ppf.shuidangran.top

JS:   process.exit(1)
来源：http://myv.yongpay.top

TS:   process.exit(1)
来源：http://yms.havefunace.top

Java: System.exit(1)
来源：http://frh.birdmap.top

Go:   os.Exit(1)
来源：http://uea.cucudq.cn

Ruby: exit 1
来源：http://akt.daria6918.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cxj.zdqjudy.top

[M06] 向标准错误输出
来源：http://fjk.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://cop.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zej.hnxiangtu.top

JS:   console.error("err")
来源：http://rss.zhongyouzk.top

TS:   console.error("err")
来源：http://pbg.hammf.cn

Java: System.err.println("err")
来源：http://tya.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uyv.cqqwz.cn

Ruby: warn "err"
来源：http://qzn.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://ltf.guannengcc.top

[M07] 判断是否为主入口
来源：http://rdt.shanyushiyangkeji.top

Py:   if __name__ == "__main__":
来源：http://waz.nanxuanxn.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ump.fanxiaobao.xyz

JS:   require.main === module
来源：http://vim.zhixingplan.top

TS:   require.main === module
来源：http://ixc.ybcxt.top

Java: public static void main(String[] args)
来源：http://edx.nanxinkj.top

Go:   func main()
来源：http://lux.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://azj.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://mwn.jyoumei.cn

[M08] 获取系统与运行时信息
来源：http://arf.xuanzx.com

Py:   platform.system();  platform.python_version()
来源：http://ndj.wangshuangyany.cn

PHP:  PHP_OS;  phpversion();
来源：http://kmu.jinqigfzy.top

JS:   process.platform;  process.version
来源：http://aiu.bjfxy.top

TS:   process.platform;  process.version
来源：http://ujo.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sls.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://end.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ehz.yj20258.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ahh.dashuyun.cn

================================================================================
来源：http://jrr.sweek.top

N. 数据结构与算法
来源：http://qxl.jqgfzy.top

================================================================================
来源：http://vrj.shanyushiyangkeji.top

[N01] 二分查找（有序数组）
来源：http://yox.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://agf.gaohongyu789.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fwf.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zvu.wangdashe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gtq.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://ndq.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://wjl.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pil.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://zzo.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://asj.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://ixx.guannengcc.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dqf.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://hxe.bbcook.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lya.jqgufenzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wde.ybcxt.top

Go:   slices.Sort(arr)
来源：http://crr.yuxming.cn

Ruby: arr.sort
来源：http://cia.xziqi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zyz.uphjek.com

[N03] 快速排序（分治示例）
来源：http://hwv.ydjk.org.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sjz.feifeiyinyue.top

PHP:  // 递归实现，或用 usort
来源：http://gbo.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://svp.shanyushiyangtech.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qxw.hongshengwenyu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xqv.52xcode.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lwl.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rve.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://qtz.hesvh.cn

[N04] 斐波那契数列
来源：http://whi.sxryk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xxp.svipenyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xbt.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fby.xziqi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gli.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vmv.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ycl.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xng.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ess.cashguo.top

[N05] 最大公约数
来源：http://dyz.tanke756.top

Py:   math.gcd(a, b)
来源：http://fao.mhx1999.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ytl.chenzaomai.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tfs.meibo888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wyj.xylfe.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hzd.ydjk.org.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yop.hongshengwenyu.top

Ruby: a.gcd(b)
来源：http://xsl.tarul.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pcq.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://lim.wangdashe.top

Py:   s == s[::-1]
来源：http://zbx.shuidangran.top

PHP:  $s === strrev($s);
来源：http://xrg.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://rli.xinyue.icu

TS:   s === [...s].reverse().join("")
来源：http://wwp.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ome.sysykeji.top

Go:   // 双指针从两端比较
来源：http://pvj.fzhhl.top

Ruby: s == s.reverse
来源：http://ftu.iojbl.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jta.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://pst.chenzaomai.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cvv.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://buj.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tlo.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://vwc.yongpay.top

Java: // 手写 HashMap
来源：http://dbn.shuidangran.top

Go:   // 手写 map[int]int
来源：http://vgp.aizwys.cn

Ruby: // 手写 Hash
来源：http://ftx.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://fwt.yuxming.cn

[N08] 生成全排列
来源：http://lox.havefunace.top

Py:   itertools.permutations(arr)
来源：http://hky.tanke756.top

PHP:  // 手写递归交换
来源：http://iuc.xylfe.cn

JS:   // 手写回溯递归
来源：http://nne.birdmap.top

TS:   // 手写回溯递归
来源：http://fsc.yj20258888.top

Java: // 手写回溯递归
来源：http://hsy.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://vbf.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://vpg.jinqigufen.top

C#:   // 手写回溯递归
来源：http://vdk.smart0.xyz

[N09] 栈与队列
来源：http://gho.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sdk.wangdashe.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sbn.havefunace.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jgh.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kwh.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jet.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mdz.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tmv.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bvg.wangdashe.top

[N10] 链表节点定义
来源：http://nhr.dianchejie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ggr.daxiang520.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fen.svipenyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eao.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://azd.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://nhd.ehwqpu.com

Go:   type Node struct { V int; Next *Node }
来源：http://vbx.dianchejie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://say.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wvh.cashguo.top

[N11] 二叉树中序遍历
来源：http://rqk.sweek.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qvm.cheryme.top

PHP:  // 手写递归函数
来源：http://zye.ppjwa.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://khf.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rfo.pycfn.com

Java: // 手写递归
来源：http://qsd.ydjk.org.cn

Go:   // 手写递归
来源：http://jhy.cheryme.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://krk.zhiwuduotai.top

C#:   // 手写递归
来源：http://vok.meibo888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cgr.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ebx.tian-w.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vks.zycfv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pwa.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wbx.pengpengdd.cyou

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ubz.jqgufenzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://udu.xziqi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vxs.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kgt.jqgufenzy.top

================================================================================
来源：http://jca.epnwcf.com

O. 并发与异步
来源：http://nnw.chenzaomai.com

================================================================================
来源：http://axt.shangyingyoupin.top

[O01] 启动一个线程
来源：http://cxn.dashuyun.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://axy.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bla.chenlongwang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qvk.nanxuanxn.top

TS:   // 同 JS
来源：http://fjz.jinqigufen.top

Java: new Thread(() -> f()).start()
来源：http://qum.jinghuilouyu.cn

Go:   go f()
来源：http://axs.cqqwz.cn

Ruby: Thread.new { f }
来源：http://szc.yj202588.top

C#:   Task.Run(() => F());
来源：http://pom.zhengqikj.top

[O02] 使用线程池
来源：http://yuk.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vsb.yueranfly.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wzu.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://djt.zycfv.cn

TS:   // worker_threads 线程池
来源：http://qtu.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://pqa.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://apb.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iyy.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qyv.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://dul.zdqjudy.top

Py:   with lock: shared += 1
来源：http://qbi.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://bwu.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yfr.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://ekl.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://xyd.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://urb.smart0.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://vsg.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://mdj.ppjwa.cn

[O04] 定义异步函数并等待
来源：http://vah.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://knf.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://urz.feifeiyinyue.top

JS:   async function f() { await g(); }
来源：http://dyh.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bxc.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ytd.mhx1999.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qfy.yueranfly.top

Ruby: # 用 Fiber 或 async gem
来源：http://tun.sysykeji.top

C#:   async Task F() { await G(); }
来源：http://afo.haohaochexian.top

[O05] 并发执行并等待全部完成
来源：http://rka.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://otd.wangdashe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rfx.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://jfa.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://soz.xylfe.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vbi.dashuyun.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hnu.zycfv.cn

Ruby: threads.map(&:join)
来源：http://wdz.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qkt.redwolf501.top

[O06] 使用进程池
来源：http://xid.shzxlz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://txm.quarkkingdee.top

PHP:  // pcntl_fork 或多进程队列
来源：http://yac.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://cgp.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://wdg.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pmq.cheryme.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qwf.52xcode.cn

Ruby: // fork 块
来源：http://hkk.shzxlz.cn

C#:   Parallel.For
来源：http://qbb.hywenlv.cn

================================================================================
来源：http://kjr.fzhhl.top

P. 常用工具函数
来源：http://yut.jinqigufen.top

================================================================================
来源：http://jkv.xziqi.cn

[P01] 生成 UUID
来源：http://ack.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://yao.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pms.yongpay.top

JS:   crypto.randomUUID()
来源：http://tsq.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://hmj.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://ujo.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://gtb.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://czs.sjlbkw.cn

C#:   Guid.NewGuid().ToString()
来源：http://ilr.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://qxm.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://skg.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yjc.yvedp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gsp.cucudq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dch.zhoulong.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://chw.hysaishi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://acm.haohaochexian.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wwg.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rqe.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://uvl.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lyj.yuxming.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://swd.hfpthk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ayu.zhengqikj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nhg.wangshuangyany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jwg.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dsr.haohaochexian.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dnz.xziqi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://olf.sysykeji.top

[P04] 求长度
来源：http://eai.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uhf.0kj1m.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xot.yj20258.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rgh.vqdsnc.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yvq.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://xdl.yangfankeji.com

Go:   len(arr);  len(m)
来源：http://fsd.zhiwuduotai.top

Ruby: x.length;  x.size
来源：http://ayo.sweek.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yvf.chenzaomai.com

[P05] 判断两个对象内容是否相等
来源：http://yqk.nanxinkj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://iln.iojbl.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jes.aibaodan.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zrh.smart0.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qta.sweek.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pam.9152youxi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zmt.hammf.cn

Ruby: a == b
来源：http://jry.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pxa.havefunace.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rjd.svipenyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xgq.hesvh.cn

PHP:  if (empty($x)) {}
来源：http://acm.jlsjyb.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qgw.gzhubu.top

TS:   if (x == null) {}
来源：http://yuj.yj20258.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hiu.ehwqpu.com

Go:   if x == nil {}
来源：http://xzy.redwolf501.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oxe.yj202588.top

C#:   if (x is null) {}
来源：http://hps.aibaodan.cn

[P07] 防抖与节流
来源：http://yxw.iojbl.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xrw.chenlongwang.top

PHP:  // 手写时间戳比较
来源：http://tfs.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ovw.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ciq.ppjwa.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zms.yueranfly.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fpt.haohaochexian.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hzb.chenjidiqi.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wgl.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://imx.gzhubu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://slg.feifeiyinyue.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://enk.feifeiyinyue.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uyi.chenlongwang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xke.daria6918.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://czf.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zyp.zhengqikj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qtv.shzxlz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rua.hongshengwenyu.top

================================================================================
来源：http://jwq.quarkkingdee.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xrh.pycfn.com

================================================================================
来源：http://jlh.yfazqb.com

[Q01] 创建表
来源：http://jij.havefunace.top


<!-- 参考信息 -->