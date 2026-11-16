代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mkx.gzhubu.top

Ruby: ENV["HOME"]
来源：http://ndr.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ihp.9152youxi.cn

[M03] 执行外部命令
来源：http://nsq.smart0.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hkk.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ozz.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ntf.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lxk.sufxvd.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://usr.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dyz.gzhubu.top

Ruby: system("ls -l");  `ls -l`
来源：http://aob.316326.xyz

C#:   Process.Start("ls", "-l");
来源：http://mpf.guowangkeji.top

[M04] 获取当前工作目录
来源：http://wui.shangyingyoupin.top

Py:   os.getcwd()
来源：http://yti.andypj.xyz

PHP:  getcwd();
来源：http://atp.yj20258888.top

JS:   process.cwd()
来源：http://phz.nanxuanxn.top

TS:   process.cwd()
来源：http://nsn.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://ahf.hongshengwenyu.top

Go:   os.Getwd()
来源：http://jdj.xziqi.cn

Ruby: Dir.pwd
来源：http://xzj.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qoj.birdmap.top

[M05] 设置退出码
来源：http://lsz.aizwys.cn

Py:   sys.exit(1)
来源：http://hoj.yangfankeji.com

PHP:  exit(1);
来源：http://xkz.zdqjudy.top

JS:   process.exit(1)
来源：http://rvv.jinqigufen.top

TS:   process.exit(1)
来源：http://mms.jinqigfzy.top

Java: System.exit(1)
来源：http://ntn.zhoulong.xyz

Go:   os.Exit(1)
来源：http://jkk.zdbjq.cn

Ruby: exit 1
来源：http://fax.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vze.feifeiyinyue.top

[M06] 向标准错误输出
来源：http://xxj.cqqwz.cn

Py:   print("err", file=sys.stderr)
来源：http://nnz.jiagoushi.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mnu.gzhubu.top

JS:   console.error("err")
来源：http://jzl.zhoulong.xyz

TS:   console.error("err")
来源：http://row.fehbvm.com

Java: System.err.println("err")
来源：http://gvc.andypj.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kpf.yangfankeji.com

Ruby: warn "err"
来源：http://fis.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://aqc.bbcook.cn

[M07] 判断是否为主入口
来源：http://olk.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://auh.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tby.zhoulong.xyz

JS:   require.main === module
来源：http://xdk.sysykeji.top

TS:   require.main === module
来源：http://brj.52xcode.cn

Java: public static void main(String[] args)
来源：http://ofo.jinqigufen.top

Go:   func main()
来源：http://gib.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uhq.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://ylm.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://ycr.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://aev.nwbrower.top

PHP:  PHP_OS;  phpversion();
来源：http://sss.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://ogr.zdqjudy.top

TS:   process.platform;  process.version
来源：http://ynr.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jdu.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://brn.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zoe.jyoumei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wik.sufxvd.cn

================================================================================
来源：http://kqd.hongshengwenyu.top

N. 数据结构与算法
来源：http://ojj.guannengcc.top

================================================================================
来源：http://yzw.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://llb.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://yth.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://men.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zsj.sjlbkw.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lud.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://sbj.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://zii.zhaomingkeji.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://hhk.jinqigufen.top

C#:   Array.BinarySearch(arr, x)
来源：http://efr.cucudq.cn

[N02] 排序（工程实践用内置实现）
来源：http://fbe.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://tdd.yonumen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hki.yuanzhike.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qzd.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://kie.dianchejie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oew.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://enb.jqgufenzy.top

Ruby: arr.sort
来源：http://cei.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tys.cashguo.top

[N03] 快速排序（分治示例）
来源：http://cuq.tian-w.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oau.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://vbl.xylfe.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jum.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lnk.hfpthk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mie.aibaodan.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ofl.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hvu.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://rbn.hnxiangtu.top

[N04] 斐波那契数列
来源：http://lvs.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mjr.gzhubu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uic.nanxinkj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mhq.ehwqpu.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dmh.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xyb.zhengqikj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bth.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cgm.jianghu66.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cjw.jlsjyb.cn

[N05] 最大公约数
来源：http://qjf.shuidangran.top

Py:   math.gcd(a, b)
来源：http://avy.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cmj.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mhe.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fti.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gxi.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qjb.vqdsnc.cn

Ruby: a.gcd(b)
来源：http://uyf.daxiang520.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ebo.chenzaomai.com

[N06] 判断回文字符串
来源：http://ymx.yongpay.top

Py:   s == s[::-1]
来源：http://pky.aizwys.cn

PHP:  $s === strrev($s);
来源：http://lkv.vqdsnc.cn

JS:   s === [...s].reverse().join("")
来源：http://gee.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://hhd.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uva.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://vju.zhaomingkeji.xyz

Ruby: s == s.reverse
来源：http://gmy.yvedp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tsy.gogol.net.cn

[N07] 两数之和（返回下标）
来源：http://rbw.gogol.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nqs.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bdn.ppjwa.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fdm.hnxiangtu.top

TS:   // 手写 Map<string, number>
来源：http://xpr.jianghu66.top

Java: // 手写 HashMap
来源：http://dba.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://luq.bjfxy.top

Ruby: // 手写 Hash
来源：http://kjs.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dsp.c1oappe.top

[N08] 生成全排列
来源：http://zzo.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://rrk.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://fmh.hnqzz.top

JS:   // 手写回溯递归
来源：http://yxo.vqdsnc.cn

TS:   // 手写回溯递归
来源：http://vht.yuanzhike.top

Java: // 手写回溯递归
来源：http://dfh.sxryk.cn

Go:   // 手写回溯递归
来源：http://ssl.zhiwuduotai.top

Ruby: arr.permutation.to_a
来源：http://ydf.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://wfq.svipenyu.cn

[N09] 栈与队列
来源：http://unf.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lxr.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sag.pycfn.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yvu.birdmap.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fns.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aot.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oic.pycfn.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hbp.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rcd.zhiwuduotai.top

[N10] 链表节点定义
来源：http://rou.bbcook.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jef.svipenyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ezc.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ksz.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://moi.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://wzd.zycfv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://idf.redwolf501.top

Ruby: Node = Struct.new(:v, :next)
来源：http://sas.redwolf501.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mcb.aizwys.cn

[N11] 二叉树中序遍历
来源：http://uql.ppjwa.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://prs.birdmap.top

PHP:  // 手写递归函数
来源：http://vjm.tianlin.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qtx.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bdz.sufxvd.cn

Java: // 手写递归
来源：http://xjm.fanxiaobao.xyz

Go:   // 手写递归
来源：http://kio.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://owp.tianlin.xyz

C#:   // 手写递归
来源：http://knq.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yhd.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ytl.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://abk.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hjf.ehwqpu.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fkw.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hgg.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rif.ydjk.org.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ypz.jinqigfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bcb.sweek.top

================================================================================
来源：http://lgm.fzhhl.top

O. 并发与异步
来源：http://qeh.ybcxt.top

================================================================================
来源：http://ldp.cashguo.top

[O01] 启动一个线程
来源：http://ona.cucudq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://psq.zhongyouzk.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mri.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fde.9152youxi.cn

TS:   // 同 JS
来源：http://sjh.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://ffs.zhijiandao.cn

Go:   go f()
来源：http://baq.9152youxi.cn

Ruby: Thread.new { f }
来源：http://mhe.tian-w.cn

C#:   Task.Run(() => F());
来源：http://ixk.kuanghao11.cn

[O02] 使用线程池
来源：http://fgl.yuxming.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://klx.ydjk.org.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iqa.zycfv.cn

JS:   // worker_threads 线程池
来源：http://qro.gogol.net.cn

TS:   // worker_threads 线程池
来源：http://jpo.guowangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://zeg.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kah.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://khu.fktsv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ihq.sysykeji.top

[O03] 加锁保护共享数据
来源：http://enn.ctjpmb.com

Py:   with lock: shared += 1
来源：http://ihx.haohaochexian.top

PHP:  // 用 flock() 做文件锁
来源：http://qzb.xuanzx.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://krb.tianlin.xyz

TS:   // 同 JS
来源：http://okq.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://dvu.jianghu66.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rin.sufxvd.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yny.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://hhi.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://yqp.wangshuangyany.cn

Py:   async def f():⏎    await g()
来源：http://ata.hnxiangtu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://prl.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://brh.hywenlv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hbw.xingfuxueyuan.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vjt.jlsjyb.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sor.gogol.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ifi.sufxvd.cn

C#:   async Task F() { await G(); }
来源：http://thh.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://ewm.bjfxy.top

Py:   asyncio.gather(*tasks)
来源：http://gpu.cucudq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xfq.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://nek.gaohongyu789.top

TS:   await Promise.all(tasks)
来源：http://qrt.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cqs.tanke756.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fcf.yvedp.cn

Ruby: threads.map(&:join)
来源：http://uhb.gzhubu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ewi.tian-w.cn

[O06] 使用进程池
来源：http://bxq.ehwqpu.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kpf.jqgfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cut.yfazqb.com

JS:   // child_process / cluster 模块
来源：http://wwz.cheryme.top

TS:   // child_process / cluster 模块
来源：http://kzh.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mhy.zhaomingkeji.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kya.iojbl.cn

Ruby: // fork 块
来源：http://ooj.haohaochexian.top

C#:   Parallel.For
来源：http://dlx.kuanghao11.cn

================================================================================
来源：http://wgr.ybcxt.top

P. 常用工具函数
来源：http://iod.yuanzhike.top

================================================================================
来源：http://rhx.andypj.xyz

[P01] 生成 UUID
来源：http://qmo.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://lux.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mgu.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://shm.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://rfm.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://nlr.yangfankeji.com

Go:   // 用 github.com/google/uuid
来源：http://aal.yj20258.top

Ruby: SecureRandom.uuid
来源：http://bwj.shuidangran.top

C#:   Guid.NewGuid().ToString()
来源：http://ixq.jqgufenzy.top

[P02] MD5 / SHA256 摘要
来源：http://yar.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vmv.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xel.zhiwuduotai.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jpd.yuanzhike.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hcr.jinqigfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bud.ywan-chungtsiang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pjz.hongshengwenyu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dck.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tkc.yueranfly.top

[P03] 生成短随机字符串
来源：http://tug.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ott.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xkz.guowangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nxq.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://etg.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://slr.zhijiandao.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bph.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xur.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ffi.dianchejie.cn

[P04] 求长度
来源：http://zef.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vgr.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://utr.gotoacloud.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yik.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mbb.jqgufenzy.top

Java: list.size();  map.size();  s.length()
来源：http://sqp.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://muz.fengsongda.top

Ruby: x.length;  x.size
来源：http://dyn.daria6918.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vkk.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://you.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ktr.xziqi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://emy.hongshengwenyu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lqv.zhengqikj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ctq.nanxinkj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gdj.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mta.kuanghao11.cn

Ruby: a == b
来源：http://jbn.yuxming.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nxc.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wsx.yuanzhike.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ccd.xylfe.cn

PHP:  if (empty($x)) {}
来源：http://med.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fzy.hywenlv.cn

TS:   if (x == null) {}
来源：http://rsu.yfazqb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://oon.yanxiufei.cn

Go:   if x == nil {}
来源：http://cvo.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fuv.gogol.net.cn

C#:   if (x is null) {}
来源：http://zqq.zhengqikj.top

[P07] 防抖与节流
来源：http://gxt.aizwys.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ito.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://dug.jlsjyb.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tvy.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://edl.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ohi.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zek.jianghu66.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qev.cdnleiting.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qdn.wangdashe.top

[P08] 处理浮点精度问题
来源：http://puy.hysaishi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://izc.yvedp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://etq.xylfe.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qpz.sysykeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://joc.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iid.redwolf501.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pqc.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rwd.shanyushiyangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oaz.birdmap.top


<!-- 参考信息 -->