代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oas.bjfxy.top

Ruby: ENV["HOME"]
来源：http://mpi.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qeu.jqgfzy.top

[M03] 执行外部命令
来源：http://uyt.zhiwuduotai.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mbd.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jfe.gaohongyu789.top

JS:   child_process.execSync("ls -l").toString()
来源：http://opp.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://vlo.cucudq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vrm.jqgfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qyx.shuidangran.top

Ruby: system("ls -l");  `ls -l`
来源：http://znd.cucudq.cn

C#:   Process.Start("ls", "-l");
来源：http://toq.xylfe.cn

[M04] 获取当前工作目录
来源：http://xdl.jinqigufen.top

Py:   os.getcwd()
来源：http://twa.shanyushiyangtech.top

PHP:  getcwd();
来源：http://brr.9152youxi.cn

JS:   process.cwd()
来源：http://asz.mhx1999.top

TS:   process.cwd()
来源：http://puu.zdbjq.cn

Java: Path.of("").toAbsolutePath()
来源：http://hbw.zhixingplan.top

Go:   os.Getwd()
来源：http://fvj.cashguo.top

Ruby: Dir.pwd
来源：http://bsp.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://sqg.bbcook.cn

[M05] 设置退出码
来源：http://mfu.nanxinkj.top

Py:   sys.exit(1)
来源：http://ndy.jinyuanbaomall.cn

PHP:  exit(1);
来源：http://tzl.sysykeji.top

JS:   process.exit(1)
来源：http://ufm.pengpengdd.cyou

TS:   process.exit(1)
来源：http://ets.mhx1999.top

Java: System.exit(1)
来源：http://jwy.ehwqpu.com

Go:   os.Exit(1)
来源：http://pdz.vehdjk.com

Ruby: exit 1
来源：http://ify.shanyushiyangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fxg.xinyue.icu

[M06] 向标准错误输出
来源：http://odd.hnxiangtu.top

Py:   print("err", file=sys.stderr)
来源：http://ozf.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://myz.quarkkingdee.top

JS:   console.error("err")
来源：http://mlb.pengpengdd.cyou

TS:   console.error("err")
来源：http://ixu.nanxinkj.top

Java: System.err.println("err")
来源：http://bxx.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zin.cdnleiting.top

Ruby: warn "err"
来源：http://ylp.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://lba.vehdjk.com

[M07] 判断是否为主入口
来源：http://dad.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://kwz.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lsp.zycfv.cn

JS:   require.main === module
来源：http://jzo.mhx1999.top

TS:   require.main === module
来源：http://xuz.jianghu66.top

Java: public static void main(String[] args)
来源：http://yfx.yueranfly.top

Go:   func main()
来源：http://hzi.chenzaomai.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dns.gogol.net.cn

C#:   static void Main(string[] args)
来源：http://uem.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://gko.jinqigfzy.top

Py:   platform.system();  platform.python_version()
来源：http://nyp.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://sfu.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://ekb.havefunace.top

TS:   process.platform;  process.version
来源：http://dpj.yanxiufei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ocv.kuanghao11.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vve.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tiw.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mjf.shzxlz.cn

================================================================================
来源：http://xyp.xuanzx.com

N. 数据结构与算法
来源：http://zob.bjfxy.top

================================================================================
来源：http://bbu.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://ggb.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://qvv.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://izy.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zjb.uphjek.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tty.iojbl.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pfk.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://rmy.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://ekv.zhaomingkeji.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://gif.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://mry.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://uus.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wav.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dwu.meibo888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xnw.yonumen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bja.yvedp.cn

Go:   slices.Sort(arr)
来源：http://gbf.nanxinkj.top

Ruby: arr.sort
来源：http://php.fanxiaobao.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://wij.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://jbe.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ajt.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://mvp.cqqwz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rwl.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uck.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://orq.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ncl.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dwh.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://zaw.jiagoushi.top

[N04] 斐波那契数列
来源：http://frd.guowangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uvx.jinyuanbaomall.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sih.shangyingyoupin.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wps.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xyt.hnqzz.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://goi.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://erl.ybcxt.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ght.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://enh.xuetiantiany.cn

[N05] 最大公约数
来源：http://flm.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://aby.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jdf.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mbu.ywan-chungtsiang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sss.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tbx.0kj1m.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://voo.yongpay.top

Ruby: a.gcd(b)
来源：http://niu.shanyushiyangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aiu.316326.xyz

[N06] 判断回文字符串
来源：http://dsq.bjfxy.top

Py:   s == s[::-1]
来源：http://vbw.xziqi.cn

PHP:  $s === strrev($s);
来源：http://fxq.redwolf501.top

JS:   s === [...s].reverse().join("")
来源：http://cct.chenlongwang.top

TS:   s === [...s].reverse().join("")
来源：http://zed.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pua.wangshuangyany.cn

Go:   // 双指针从两端比较
来源：http://sgg.hongshengwenyu.top

Ruby: s == s.reverse
来源：http://xec.redwolf501.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://isg.zycfv.cn

[N07] 两数之和（返回下标）
来源：http://cfl.fktsv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fgn.zhixingplan.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pjx.tanke756.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mhn.feifeiyinyue.top

TS:   // 手写 Map<string, number>
来源：http://ein.shangyingyoupin.top

Java: // 手写 HashMap
来源：http://azo.shangyingyoupin.top

Go:   // 手写 map[int]int
来源：http://azt.9152youxi.cn

Ruby: // 手写 Hash
来源：http://csc.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://vrm.wangdashe.top

[N08] 生成全排列
来源：http://ukh.zhaomingkeji.xyz

Py:   itertools.permutations(arr)
来源：http://ruu.quarkkingdee.top

PHP:  // 手写递归交换
来源：http://kpz.sxryk.cn

JS:   // 手写回溯递归
来源：http://ple.ctjpmb.com

TS:   // 手写回溯递归
来源：http://mhk.ydjk.org.cn

Java: // 手写回溯递归
来源：http://ycu.zhoulong.xyz

Go:   // 手写回溯递归
来源：http://qag.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://xft.yj202588.top

C#:   // 手写回溯递归
来源：http://ztx.yj20258.top

[N09] 栈与队列
来源：http://eec.cheryme.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fpo.yonumen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lbb.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bpn.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gmg.haohaochexian.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://htc.yfazqb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bdo.tanke756.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lyx.0kj1m.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nen.jqgfzy.top

[N10] 链表节点定义
来源：http://ifm.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ziy.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hlg.hammf.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tmg.shzxlz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vfw.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://sex.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://agd.pengpengdd.cyou

Ruby: Node = Struct.new(:v, :next)
来源：http://wvc.zhiwuduotai.top

C#:   class Node { public int V; public Node? Next; }
来源：http://eno.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://fgp.jinqigfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qkl.epnwcf.com

PHP:  // 手写递归函数
来源：http://fpk.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rxl.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yur.snrcjt.cn

Java: // 手写递归
来源：http://dnw.jlsjyb.cn

Go:   // 手写递归
来源：http://szd.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zej.yanxiufei.cn

C#:   // 手写递归
来源：http://ujr.cucudq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xkm.zhongyouzk.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://szm.chenzaomai.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qco.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://adf.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bln.zhiwuduotai.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ddn.yonumen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wqi.svipenyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wxq.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cvr.jiagoushi.top

================================================================================
来源：http://yxf.mhx1999.top

O. 并发与异步
来源：http://grn.sysykeji.top

================================================================================
来源：http://slw.chenjidiqi.icu

[O01] 启动一个线程
来源：http://cjo.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dtq.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eqr.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wzt.ppjwa.cn

TS:   // 同 JS
来源：http://agu.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://txx.yongpay.top

Go:   go f()
来源：http://cwn.yangfankeji.com

Ruby: Thread.new { f }
来源：http://gwn.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://olv.wangdashe.top

[O02] 使用线程池
来源：http://qyn.xingfuxueyuan.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hbd.cheryme.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xmx.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://mkp.xingfuxueyuan.xyz

TS:   // worker_threads 线程池
来源：http://qbl.ydzc1.top

Java: Executors.newFixedThreadPool(4)
来源：http://jfa.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dew.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bsz.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://awu.yj202588.top

[O03] 加锁保护共享数据
来源：http://jmv.pycfn.com

Py:   with lock: shared += 1
来源：http://oxq.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://xyv.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vlx.aizwys.cn

TS:   // 同 JS
来源：http://qro.gogol.net.cn

Java: synchronized (this) { shared++; }
来源：http://dbl.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bsh.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://emh.wangshuangyany.cn

C#:   lock (gate) { shared++; }
来源：http://puw.tian-w.cn

[O04] 定义异步函数并等待
来源：http://xxf.ppjwa.cn

Py:   async def f():⏎    await g()
来源：http://szx.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cvm.hongshengwenyu.top

JS:   async function f() { await g(); }
来源：http://ajb.zdbjq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://szn.shanyushiyangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zgm.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://alc.jinqigfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://rhz.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://viz.zycfv.cn

[O05] 并发执行并等待全部完成
来源：http://alj.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://jzy.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pgv.cheryme.top

JS:   await Promise.all(tasks)
来源：http://qwf.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://mlc.aizwys.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ndp.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fgh.zhengqikj.top

Ruby: threads.map(&:join)
来源：http://ooq.jinyuanbaomall.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cwn.yuxming.cn

[O06] 使用进程池
来源：http://wbg.zycfv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gmm.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://pyl.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://ukt.hfpthk.cn

TS:   // child_process / cluster 模块
来源：http://iqx.sufxvd.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qsm.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zak.hnqzz.top

Ruby: // fork 块
来源：http://olk.jyoumei.cn

C#:   Parallel.For
来源：http://fwo.cucudq.cn

================================================================================
来源：http://msp.shuidangran.top

P. 常用工具函数
来源：http://vwk.jqgfzy.top

================================================================================
来源：http://ved.guannengcc.top

[P01] 生成 UUID
来源：http://xwy.hfpthk.cn

Py:   str(uuid.uuid4())
来源：http://fmc.hesvh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qgd.jqgufenzy.top

JS:   crypto.randomUUID()
来源：http://vkm.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://gws.ydjk.org.cn

Java: UUID.randomUUID().toString()
来源：http://uyz.nwbrower.top

Go:   // 用 github.com/google/uuid
来源：http://sdg.iojbl.cn

Ruby: SecureRandom.uuid
来源：http://bet.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://oum.sxryk.cn

[P02] MD5 / SHA256 摘要
来源：http://vbb.shanyushiyangtech.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jwq.shuidangran.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://udh.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wrb.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mvq.shanyushiyangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://smb.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fkp.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://opc.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oqq.shanyushiyangtech.top

[P03] 生成短随机字符串
来源：http://edm.hnqzz.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ybt.cdnleiting.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://alr.bjfxy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lpa.hesvh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zny.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://omy.hnqzz.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jmi.tian-w.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mlq.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dal.daria6918.cn

[P04] 求长度
来源：http://jwn.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://guj.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gwv.epnwcf.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ucg.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wem.guannengcc.top

Java: list.size();  map.size();  s.length()
来源：http://pkk.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://mxx.wangshuangyany.cn

Ruby: x.length;  x.size
来源：http://yqv.aibaodan.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jii.zdqjudy.top

[P05] 判断两个对象内容是否相等
来源：http://zhd.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wzs.jinqigufen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kbk.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://roq.zhengqikj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hzr.cdnleiting.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xla.pengpengdd.cyou

Go:   reflect.DeepEqual(a, b)
来源：http://imb.quarkkingdee.top

Ruby: a == b
来源：http://urr.ivvv.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wup.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rgh.yj20258888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://esn.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://zle.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://snl.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://nzk.xingfuxueyuan.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://ded.ybcxt.top

Go:   if x == nil {}
来源：http://kqn.fzhhl.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cex.havefunace.top

C#:   if (x is null) {}
来源：http://avt.shangyingyoupin.top

[P07] 防抖与节流
来源：http://zxx.shanyushiyangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://stz.9152youxi.cn

PHP:  // 手写时间戳比较
来源：http://hcm.fanxiaobao.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xgp.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xxe.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://byi.tian-w.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hsr.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://kax.shuidangran.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vrn.sxryk.cn

[P08] 处理浮点精度问题
来源：http://qpy.chenjidiqi.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dlu.nanxinkj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ivy.ydzc1.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zkb.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oae.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uma.yj20258.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mwm.jqgufenzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sjx.nanxinkj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kxh.yj202588.top


<!-- 参考信息 -->