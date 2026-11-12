代发 wailian999

Ruby: ARGV
来源：http://rom.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://ojm.tarul.cn

[M02] 读取环境变量
来源：http://juu.hywenlv.cn

Py:   os.environ.get("HOME")
来源：http://mrk.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cnh.zhiwuduotai.top

JS:   process.env.HOME
来源：http://inu.jqgfzy.top

TS:   process.env.HOME
来源：http://nni.yj202588.top

Java: System.getenv("HOME")
来源：http://wpr.ybcxt.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://djo.xuanzx.com

Ruby: ENV["HOME"]
来源：http://yxt.nanxuanxn.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kse.chenlongwang.top

[M03] 执行外部命令
来源：http://coe.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fuw.gaohongyu789.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mbm.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zpl.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pxk.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uex.hfpthk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ctu.jyoumei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ydu.sysykeji.top

C#:   Process.Start("ls", "-l");
来源：http://wwg.gogol.net.cn

[M04] 获取当前工作目录
来源：http://cjx.shanyushiyangkeji.top

Py:   os.getcwd()
来源：http://ikc.hongshengwenyu.top

PHP:  getcwd();
来源：http://yxn.yueranfly.top

JS:   process.cwd()
来源：http://mda.sysykeji.top

TS:   process.cwd()
来源：http://lah.zhengqikj.top

Java: Path.of("").toAbsolutePath()
来源：http://jes.nwbrower.top

Go:   os.Getwd()
来源：http://dlm.zhoulong.xyz

Ruby: Dir.pwd
来源：http://wcu.kuanghao11.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zzs.nwbrower.top

[M05] 设置退出码
来源：http://tgs.cheryme.top

Py:   sys.exit(1)
来源：http://faw.yuxming.cn

PHP:  exit(1);
来源：http://itz.chenjidiqi.icu

JS:   process.exit(1)
来源：http://rbr.0kj1m.cn

TS:   process.exit(1)
来源：http://uve.daxiang520.top

Java: System.exit(1)
来源：http://ghl.andypj.xyz

Go:   os.Exit(1)
来源：http://wdl.xuetiantiany.cn

Ruby: exit 1
来源：http://nfx.meibo888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hbx.ydjk.org.cn

[M06] 向标准错误输出
来源：http://ahx.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://ath.zhoulong.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ixa.52xcode.cn

JS:   console.error("err")
来源：http://pee.mhx1999.top

TS:   console.error("err")
来源：http://whv.zycfv.cn

Java: System.err.println("err")
来源：http://egx.zdqjudy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://prn.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://vjt.tian-w.cn

C#:   Console.Error.WriteLine("err")
来源：http://eve.bjfxy.top

[M07] 判断是否为主入口
来源：http://syv.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://hct.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ywi.chenjidiqi.icu

JS:   require.main === module
来源：http://dbn.xuetiantiany.cn

TS:   require.main === module
来源：http://rjg.jqgfzy.top

Java: public static void main(String[] args)
来源：http://jdb.hysaishi.cn

Go:   func main()
来源：http://nok.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ere.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://lid.cheryme.top

[M08] 获取系统与运行时信息
来源：http://qgn.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://ejr.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://ean.wangdashe.top

JS:   process.platform;  process.version
来源：http://afa.yvedp.cn

TS:   process.platform;  process.version
来源：http://gqu.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ohx.shanyushiyangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lga.sufxvd.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lee.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wer.meibo888.top

================================================================================
来源：http://hdh.gzhubu.top

N. 数据结构与算法
来源：http://ome.gzhubu.top

================================================================================
来源：http://zzx.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://sze.gzhubu.top

Py:   bisect.bisect_left(arr, x)
来源：http://wcs.sweek.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dny.cqqwz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vly.ehwqpu.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://upq.yvedp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fmp.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://cnb.fanxiaobao.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://kft.jinyuanbaomall.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uye.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://ldi.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://qgb.fanxiaobao.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ljl.hongshengwenyu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zus.52xcode.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jsm.tianlin.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qgz.hcnkem.com

Go:   slices.Sort(arr)
来源：http://tjm.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://jdq.birdmap.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mzz.ywan-chungtsiang.top

[N03] 快速排序（分治示例）
来源：http://ipq.xuanzx.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://seo.tianlin.xyz

PHP:  // 递归实现，或用 usort
来源：http://xxy.zhengqikj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ukx.sxryk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bww.yueranfly.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jyy.guannengcc.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://che.ybcxt.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vrb.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://hom.yj202588.top

[N04] 斐波那契数列
来源：http://zuu.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hdp.jlsjyb.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ipm.sjlbkw.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cap.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://agc.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wel.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vyg.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sdg.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qkj.yuanzhike.top

[N05] 最大公约数
来源：http://uri.ivvv.top

Py:   math.gcd(a, b)
来源：http://arn.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sob.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ebi.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dfx.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bfb.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://svy.tian-w.cn

Ruby: a.gcd(b)
来源：http://dqr.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jqy.zhengqikj.top

[N06] 判断回文字符串
来源：http://dib.cqqwz.cn

Py:   s == s[::-1]
来源：http://yvn.vqdsnc.cn

PHP:  $s === strrev($s);
来源：http://vrq.zhiwuduotai.top

JS:   s === [...s].reverse().join("")
来源：http://gtn.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://psg.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vti.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://izn.sjlbkw.cn

Ruby: s == s.reverse
来源：http://fbo.xuanzx.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://qeb.epnwcf.com

[N07] 两数之和（返回下标）
来源：http://ohh.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://emo.zdqjudy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eyd.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://lby.dashuyun.cn

TS:   // 手写 Map<string, number>
来源：http://wux.shanyushiyangtech.top

Java: // 手写 HashMap
来源：http://vxb.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://lqv.jinqigufen.top

Ruby: // 手写 Hash
来源：http://qai.zhiwuduotai.top

C#:   // 手写 Dictionary<int, int>
来源：http://ktp.fanxiaobao.xyz

[N08] 生成全排列
来源：http://kiw.yuanzhike.top

Py:   itertools.permutations(arr)
来源：http://uiz.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://ske.cashguo.top

JS:   // 手写回溯递归
来源：http://zxd.c1oappe.top

TS:   // 手写回溯递归
来源：http://imt.ppjwa.cn

Java: // 手写回溯递归
来源：http://txr.cqqwz.cn

Go:   // 手写回溯递归
来源：http://pzv.ivvv.top

Ruby: arr.permutation.to_a
来源：http://udq.xinyue.icu

C#:   // 手写回溯递归
来源：http://hnw.bjfxy.top

[N09] 栈与队列
来源：http://zuo.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bju.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gvm.kuanghao11.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://usv.cheryme.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ghn.pycfn.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xns.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jvx.yuanzhike.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://weg.hysaishi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iab.zhongyouzk.top

[N10] 链表节点定义
来源：http://rgv.zycfv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ryr.hammf.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://srb.aibaodan.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ofb.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://obc.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://hcq.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://wpg.ydzc1.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zok.kuanghao11.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sjb.bjfxy.top

[N11] 二叉树中序遍历
来源：http://mgx.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vao.redwolf501.top

PHP:  // 手写递归函数
来源：http://dit.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wbk.yvedp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://snw.epnwcf.com

Java: // 手写递归
来源：http://zkq.gzhubu.top

Go:   // 手写递归
来源：http://sje.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vga.zycfv.cn

C#:   // 手写递归
来源：http://upq.yfazqb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://alr.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bmj.jqgufenzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sba.ppjwa.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vfs.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xht.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dmc.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qvt.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jwe.jianghu66.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vij.ctjpmb.com

================================================================================
来源：http://vfb.fzhhl.top

O. 并发与异步
来源：http://bmx.aizwys.cn

================================================================================
来源：http://dtt.chenlongwang.top

[O01] 启动一个线程
来源：http://gfm.316326.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rrw.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://adh.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mpk.yj202588.top

TS:   // 同 JS
来源：http://mkb.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://qak.chenjidiqi.icu

Go:   go f()
来源：http://aei.hfpthk.cn

Ruby: Thread.new { f }
来源：http://cxy.fzhhl.top

C#:   Task.Run(() => F());
来源：http://ist.sufxvd.cn

[O02] 使用线程池
来源：http://ucb.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ije.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vrc.bjfxy.top

JS:   // worker_threads 线程池
来源：http://pzi.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://itb.zhongyouzk.top

Java: Executors.newFixedThreadPool(4)
来源：http://abt.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mwv.jinyuanbaomall.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pgt.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rpv.tian-w.cn

[O03] 加锁保护共享数据
来源：http://dyl.yueranfly.top

Py:   with lock: shared += 1
来源：http://spd.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://hdu.cheryme.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lqi.hongshengwenyu.top

TS:   // 同 JS
来源：http://vbv.fzhhl.top

Java: synchronized (this) { shared++; }
来源：http://hka.zhixingplan.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://szk.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ziu.shuidangran.top

C#:   lock (gate) { shared++; }
来源：http://gcs.0kj1m.cn

[O04] 定义异步函数并等待
来源：http://esy.mhx1999.top

Py:   async def f():⏎    await g()
来源：http://vqd.ywan-chungtsiang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://efn.jinqigfzy.top

JS:   async function f() { await g(); }
来源：http://ehe.iojbl.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jpi.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ned.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pof.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://pfn.jianghu66.top

C#:   async Task F() { await G(); }
来源：http://ibx.aibaodan.cn

[O05] 并发执行并等待全部完成
来源：http://mss.ivvv.top

Py:   asyncio.gather(*tasks)
来源：http://ghm.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lss.cqqwz.cn

JS:   await Promise.all(tasks)
来源：http://itx.fzhhl.top

TS:   await Promise.all(tasks)
来源：http://xty.cheryme.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dos.cdnleiting.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qcy.bbcook.cn

Ruby: threads.map(&:join)
来源：http://rcb.andypj.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://gbe.dashuyun.cn

[O06] 使用进程池
来源：http://llp.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bny.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://thh.xuanzx.com

JS:   // child_process / cluster 模块
来源：http://pez.sufxvd.cn

TS:   // child_process / cluster 模块
来源：http://lzf.yongpay.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qvc.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fgn.ydjk.org.cn

Ruby: // fork 块
来源：http://blh.zhengqikj.top

C#:   Parallel.For
来源：http://ajc.hcnkem.com

================================================================================
来源：http://ffv.jinqigfzy.top

P. 常用工具函数
来源：http://ong.ydzc1.top

================================================================================
来源：http://bfq.tanke756.top

[P01] 生成 UUID
来源：http://fft.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://uea.zdqjudy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iyw.iojbl.cn

JS:   crypto.randomUUID()
来源：http://qxa.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://qfc.nanxinkj.top

Java: UUID.randomUUID().toString()
来源：http://rgf.yvedp.cn

Go:   // 用 github.com/google/uuid
来源：http://hsw.ehwqpu.com

Ruby: SecureRandom.uuid
来源：http://gfx.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://qny.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://cbf.ehwqpu.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aze.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ysv.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zcr.yangfankeji.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hwh.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fzg.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ywu.chenlongwang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ple.daria6918.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ohw.chenlongwang.top

[P03] 生成短随机字符串
来源：http://cxq.yuanzhike.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ojl.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://grc.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hel.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yfj.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ckv.wangdashe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cci.guowangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mrq.smart0.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cga.uphjek.com

[P04] 求长度
来源：http://fha.jinyuanbaomall.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gyo.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dba.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nkx.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cwr.yj20258.top

Java: list.size();  map.size();  s.length()
来源：http://jrd.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://yho.hcnkem.com

Ruby: x.length;  x.size
来源：http://dqw.0kj1m.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bhe.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://hmf.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jkh.shangyingyoupin.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ses.nanxuanxn.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mxj.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lcd.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://awk.daria6918.cn

Go:   reflect.DeepEqual(a, b)
来源：http://miz.sufxvd.cn

Ruby: a == b
来源：http://zgy.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aom.zhijiandao.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pmu.xingfuxueyuan.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eni.cdnleiting.top

PHP:  if (empty($x)) {}
来源：http://eim.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jxt.chenzaomai.com

TS:   if (x == null) {}
来源：http://haw.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jhy.ctjpmb.com

Go:   if x == nil {}
来源：http://kfs.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xel.havefunace.top

C#:   if (x is null) {}
来源：http://wkx.yj202588.top

[P07] 防抖与节流
来源：http://laa.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://duj.dianchejie.cn

PHP:  // 手写时间戳比较
来源：http://ebh.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xkm.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uva.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mja.fanxiaobao.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nlr.sysykeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yvu.jinqigfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qmo.wangshuangyany.cn

[P08] 处理浮点精度问题
来源：http://ykg.jinghuilouyu.cn


<!-- 参考信息 -->