代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zhz.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://imj.cucudq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uxs.uphjek.com

[M03] 执行外部命令
来源：http://rub.smart0.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pjd.9152youxi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rpu.hywenlv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dhm.sweek.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cov.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yyj.feifeiyinyue.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ezo.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://gtl.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://vok.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://rew.smart0.xyz

Py:   os.getcwd()
来源：http://gpu.yangfankeji.com

PHP:  getcwd();
来源：http://rme.0kj1m.cn

JS:   process.cwd()
来源：http://guj.yj202588.top

TS:   process.cwd()
来源：http://fwj.xinyue.icu

Java: Path.of("").toAbsolutePath()
来源：http://gwz.hnqzz.top

Go:   os.Getwd()
来源：http://fnm.svipenyu.cn

Ruby: Dir.pwd
来源：http://kqn.nanxinkj.top

C#:   Directory.GetCurrentDirectory()
来源：http://gsf.snrcjt.cn

[M05] 设置退出码
来源：http://oou.tian-w.cn

Py:   sys.exit(1)
来源：http://jov.ybcxt.top

PHP:  exit(1);
来源：http://dfa.zhiwuduotai.top

JS:   process.exit(1)
来源：http://xze.shangyingyoupin.top

TS:   process.exit(1)
来源：http://yjw.shangyingyoupin.top

Java: System.exit(1)
来源：http://vzk.hnxiangtu.top

Go:   os.Exit(1)
来源：http://arx.cqqwz.cn

Ruby: exit 1
来源：http://vkv.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://plj.hysaishi.cn

[M06] 向标准错误输出
来源：http://ioo.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://cva.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sjd.fzhhl.top

JS:   console.error("err")
来源：http://uyd.cdnleiting.top

TS:   console.error("err")
来源：http://oqf.vehdjk.com

Java: System.err.println("err")
来源：http://vti.vehdjk.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vyg.0kj1m.cn

Ruby: warn "err"
来源：http://vze.nanxinkj.top

C#:   Console.Error.WriteLine("err")
来源：http://orh.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://hox.aibaodan.cn

Py:   if __name__ == "__main__":
来源：http://dbr.haohaochexian.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wuj.fzhhl.top

JS:   require.main === module
来源：http://rtj.ctjpmb.com

TS:   require.main === module
来源：http://ouz.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://dsj.dashuyun.cn

Go:   func main()
来源：http://fqt.jinqigfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://krj.zhengqikj.top

C#:   static void Main(string[] args)
来源：http://avt.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://uze.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://ghc.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://wpm.yueranfly.top

JS:   process.platform;  process.version
来源：http://seh.zhaomingkeji.xyz

TS:   process.platform;  process.version
来源：http://zsc.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cmm.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dsg.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ftt.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://cak.yonumen.top

================================================================================
来源：http://dsv.yonumen.top

N. 数据结构与算法
来源：http://vmv.shanyushiyangkeji.top

================================================================================
来源：http://twe.gogol.net.cn

[N01] 二分查找（有序数组）
来源：http://poe.chenlongwang.top

Py:   bisect.bisect_left(arr, x)
来源：http://dko.tianlin.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://apv.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ilw.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pnl.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://ucq.zdbjq.cn

Go:   sort.SearchInts(arr, x)
来源：http://bnc.jinqigfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lgg.zhijiandao.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aqf.hfpthk.cn

[N02] 排序（工程实践用内置实现）
来源：http://ksu.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://hep.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jxn.hywenlv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nxz.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xmn.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://caa.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://xvh.ydzc1.top

Ruby: arr.sort
来源：http://nqt.chenlongwang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kfq.yonumen.top

[N03] 快速排序（分治示例）
来源：http://qjn.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qlm.ywan-chungtsiang.top

PHP:  // 递归实现，或用 usort
来源：http://dgu.hysaishi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jje.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vfg.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hkv.hongshengwenyu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://boa.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rhn.dianchejie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fvp.jiagoushi.top

[N04] 斐波那契数列
来源：http://iyl.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sch.jinqigufen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://amv.bjfxy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wab.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vlm.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sfk.zhixingplan.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://abk.guowangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dyn.guannengcc.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pbr.hesvh.cn

[N05] 最大公约数
来源：http://qrz.sjlbkw.cn

Py:   math.gcd(a, b)
来源：http://vvt.hesvh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fie.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ztn.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kec.iojbl.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://utw.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fmh.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://aeo.vehdjk.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pxv.xylfe.cn

[N06] 判断回文字符串
来源：http://pwm.ivvv.top

Py:   s == s[::-1]
来源：http://zvp.fzhhl.top

PHP:  $s === strrev($s);
来源：http://wzn.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://xfh.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://svn.aizwys.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zrw.feifeiyinyue.top

Go:   // 双指针从两端比较
来源：http://waf.jiagoushi.top

Ruby: s == s.reverse
来源：http://ypj.jianghu66.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ugi.birdmap.top

[N07] 两数之和（返回下标）
来源：http://pbn.sufxvd.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zmu.andypj.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ehx.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gin.yfazqb.com

TS:   // 手写 Map<string, number>
来源：http://prc.yuanzhike.top

Java: // 手写 HashMap
来源：http://esr.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://ndx.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://qrp.hfpthk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rgm.vehdjk.com

[N08] 生成全排列
来源：http://dfe.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://yvt.yonumen.top

PHP:  // 手写递归交换
来源：http://kpj.gaohongyu789.top

JS:   // 手写回溯递归
来源：http://ako.c1oappe.top

TS:   // 手写回溯递归
来源：http://gff.52xcode.cn

Java: // 手写回溯递归
来源：http://jrd.0kj1m.cn

Go:   // 手写回溯递归
来源：http://fyv.yonumen.top

Ruby: arr.permutation.to_a
来源：http://ogt.hammf.cn

C#:   // 手写回溯递归
来源：http://vte.gotoacloud.top

[N09] 栈与队列
来源：http://xtz.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qdc.tanke756.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://huv.ehwqpu.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mwv.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kup.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wvl.haohaochexian.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://klc.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bdv.yj20258888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ekq.havefunace.top

[N10] 链表节点定义
来源：http://isj.snrcjt.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kkq.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ljs.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://flw.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vsf.ydzc1.top

Java: class Node { int v; Node next; }
来源：http://rvw.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://afz.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://lvz.fzhhl.top

C#:   class Node { public int V; public Node? Next; }
来源：http://chp.jinqigfzy.top

[N11] 二叉树中序遍历
来源：http://vos.zdqjudy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://seo.nwbrower.top

PHP:  // 手写递归函数
来源：http://zlv.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://axy.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ipz.ivvv.top

Java: // 手写递归
来源：http://lkt.yfazqb.com

Go:   // 手写递归
来源：http://edz.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://epa.jqgufenzy.top

C#:   // 手写递归
来源：http://iem.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hrw.svipenyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wlt.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cgw.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cju.epnwcf.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://doo.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zlj.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qbp.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wch.hnxiangtu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pls.ehwqpu.com

================================================================================
来源：http://yhj.yangfankeji.com

O. 并发与异步
来源：http://brh.yonumen.top

================================================================================
来源：http://gke.fengsongda.top

[O01] 启动一个线程
来源：http://skj.tian-w.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bdu.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gfn.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rwi.guannengcc.top

TS:   // 同 JS
来源：http://ppm.fengsongda.top

Java: new Thread(() -> f()).start()
来源：http://nsg.gotoacloud.top

Go:   go f()
来源：http://xdr.tanke756.top

Ruby: Thread.new { f }
来源：http://mky.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://zdy.aibaodan.cn

[O02] 使用线程池
来源：http://idk.epnwcf.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tfj.tianlin.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jwl.tian-w.cn

JS:   // worker_threads 线程池
来源：http://yge.fehbvm.com

TS:   // worker_threads 线程池
来源：http://qjn.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cbf.jiagoushi.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xyr.yj20258.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zvl.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oqk.tianlin.xyz

[O03] 加锁保护共享数据
来源：http://yhk.guannengcc.top

Py:   with lock: shared += 1
来源：http://gfz.yueranfly.top

PHP:  // 用 flock() 做文件锁
来源：http://ioj.guannengcc.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ndm.zhiwuduotai.top

TS:   // 同 JS
来源：http://xba.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://bnp.hnqzz.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vot.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fjn.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://rvf.andypj.xyz

[O04] 定义异步函数并等待
来源：http://dix.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://pwk.sxryk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aub.xziqi.cn

JS:   async function f() { await g(); }
来源：http://sbu.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://spw.jyoumei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://idt.fanxiaobao.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fug.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ufj.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://cqe.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://bol.shangyingyoupin.top

Py:   asyncio.gather(*tasks)
来源：http://pgw.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rgf.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://nfo.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://mso.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yqq.zycfv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://frt.52xcode.cn

Ruby: threads.map(&:join)
来源：http://hfs.pengpengdd.cyou

C#:   await Task.WhenAll(t1, t2)
来源：http://ksf.nanxinkj.top

[O06] 使用进程池
来源：http://piq.snrcjt.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qeu.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xxe.yvedp.cn

JS:   // child_process / cluster 模块
来源：http://qgy.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://lhz.52xcode.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uzw.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://abp.hnqzz.top

Ruby: // fork 块
来源：http://fhs.daria6918.cn

C#:   Parallel.For
来源：http://xqr.52xcode.cn

================================================================================
来源：http://swb.9152youxi.cn

P. 常用工具函数
来源：http://jkp.zhiwuduotai.top

================================================================================
来源：http://vox.yvedp.cn

[P01] 生成 UUID
来源：http://dsr.zhengqikj.top

Py:   str(uuid.uuid4())
来源：http://ugt.hywenlv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ylc.yuanzhike.top

JS:   crypto.randomUUID()
来源：http://rez.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://sxq.cdnleiting.top

Java: UUID.randomUUID().toString()
来源：http://ipm.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://upi.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://gyy.nwbrower.top

C#:   Guid.NewGuid().ToString()
来源：http://wwu.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://gmk.fktsv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bqh.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qgw.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wwh.hnqzz.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qok.shanyushiyangtech.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iwm.jyoumei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qcd.yj202588.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hlc.hfpthk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hgj.sweek.top

[P03] 生成短随机字符串
来源：http://fao.jqgufenzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fjl.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ryk.yueranfly.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zwd.hfpthk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xyq.feifeiyinyue.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://axr.zhijiandao.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iln.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cok.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fgy.sjlbkw.cn

[P04] 求长度
来源：http://gas.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rva.cucudq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ojj.uphjek.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kso.iojbl.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dbe.hcnkem.com

Java: list.size();  map.size();  s.length()
来源：http://bth.yvedp.cn

Go:   len(arr);  len(m)
来源：http://uqd.fzhhl.top

Ruby: x.length;  x.size
来源：http://alq.nanxuanxn.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://stu.snrcjt.cn

[P05] 判断两个对象内容是否相等
来源：http://ilg.xuetiantiany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vuf.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kac.hfpthk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iav.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wrz.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ovg.zhoulong.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://otv.9152youxi.cn

Ruby: a == b
来源：http://ydz.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rsd.fktsv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iep.yueranfly.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yvr.fktsv.cn

PHP:  if (empty($x)) {}
来源：http://mqt.52xcode.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bfx.gotoacloud.top

TS:   if (x == null) {}
来源：http://hgi.yj20258.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xvq.svipenyu.cn

Go:   if x == nil {}
来源：http://hjj.uphjek.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kae.guannengcc.top

C#:   if (x is null) {}
来源：http://hof.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://alk.jinghuilouyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wpm.svipenyu.cn

PHP:  // 手写时间戳比较
来源：http://rwy.gaohongyu789.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lcr.aizwys.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cdx.zdqjudy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pyp.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dde.zycfv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://erm.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kun.0kj1m.cn

[P08] 处理浮点精度问题
来源：http://veb.hcnkem.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xlj.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ana.jinqigufen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vvn.mhx1999.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kta.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tku.daria6918.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xtw.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jog.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lqi.daria6918.cn


<!-- 参考信息 -->