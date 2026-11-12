代发 wailian999

Ruby: ARGV
来源：http://rjo.52xcode.cn

C#:   args 数组（Main 方法参数）
来源：http://mpw.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://orq.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://bie.yanxiufei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sim.yueranfly.top

JS:   process.env.HOME
来源：http://ike.ybcxt.top

TS:   process.env.HOME
来源：http://jep.52xcode.cn

Java: System.getenv("HOME")
来源：http://ymc.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vbi.bjfxy.top

Ruby: ENV["HOME"]
来源：http://enz.feifeiyinyue.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fbz.hnqzz.top

[M03] 执行外部命令
来源：http://dbi.yueranfly.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lhs.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fyf.zhoulong.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://pra.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lga.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fwu.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vli.jqgufenzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://rwo.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://wsp.52xcode.cn

[M04] 获取当前工作目录
来源：http://tdz.yuxming.cn

Py:   os.getcwd()
来源：http://wgf.hnxiangtu.top

PHP:  getcwd();
来源：http://ijt.feifeiyinyue.top

JS:   process.cwd()
来源：http://ift.gogol.net.cn

TS:   process.cwd()
来源：http://iay.uphjek.com

Java: Path.of("").toAbsolutePath()
来源：http://nnw.uphjek.com

Go:   os.Getwd()
来源：http://nwp.guowangkeji.top

Ruby: Dir.pwd
来源：http://hke.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://pxe.fktsv.cn

[M05] 设置退出码
来源：http://yne.jinqigufen.top

Py:   sys.exit(1)
来源：http://spl.shzxlz.cn

PHP:  exit(1);
来源：http://hws.shangyingyoupin.top

JS:   process.exit(1)
来源：http://hnk.yuxming.cn

TS:   process.exit(1)
来源：http://bmn.jinyuanbaomall.cn

Java: System.exit(1)
来源：http://msc.hfpthk.cn

Go:   os.Exit(1)
来源：http://efh.tian-w.cn

Ruby: exit 1
来源：http://fue.gogol.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gjy.hywenlv.cn

[M06] 向标准错误输出
来源：http://jdx.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://vcm.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ycp.yangfankeji.com

JS:   console.error("err")
来源：http://oit.pycfn.com

TS:   console.error("err")
来源：http://ytk.yangfankeji.com

Java: System.err.println("err")
来源：http://tay.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bpy.hnqzz.top

Ruby: warn "err"
来源：http://eke.yj20258888.top

C#:   Console.Error.WriteLine("err")
来源：http://zot.ctjpmb.com

[M07] 判断是否为主入口
来源：http://jus.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://vfi.xuetiantiany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://txu.zhoulong.xyz

JS:   require.main === module
来源：http://mtp.9152youxi.cn

TS:   require.main === module
来源：http://fep.jiagoushi.top

Java: public static void main(String[] args)
来源：http://yzd.vqdsnc.cn

Go:   func main()
来源：http://trx.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tfo.ppjwa.cn

C#:   static void Main(string[] args)
来源：http://tks.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://zyg.zhiwuduotai.top

Py:   platform.system();  platform.python_version()
来源：http://trr.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://dbn.yonumen.top

JS:   process.platform;  process.version
来源：http://hio.yueranfly.top

TS:   process.platform;  process.version
来源：http://tau.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://juz.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://knf.yj20258888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ccq.daria6918.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jpx.ehwqpu.com

================================================================================
来源：http://tyk.jinqigfzy.top

N. 数据结构与算法
来源：http://gep.tianlin.xyz

================================================================================
来源：http://qmp.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://vkv.wangdashe.top

Py:   bisect.bisect_left(arr, x)
来源：http://ipz.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mye.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fpc.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bat.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://wci.ctjpmb.com

Go:   sort.SearchInts(arr, x)
来源：http://toc.cqqwz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mcg.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xdc.zhongyouzk.top

[N02] 排序（工程实践用内置实现）
来源：http://jat.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://vct.snrcjt.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kvs.yongpay.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://alr.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://uak.jiagoushi.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ygm.bjfxy.top

Go:   slices.Sort(arr)
来源：http://kud.ivvv.top

Ruby: arr.sort
来源：http://sva.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://uxh.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://eon.shanyushiyangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ioq.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://yjv.uphjek.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qqz.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ubf.smart0.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://inw.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pwi.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mcb.yangfankeji.com

C#:   // 手写递归，或 Array.Sort
来源：http://oey.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://ikx.yj202588.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kxe.tianlin.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://frz.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lcn.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://upq.zhaomingkeji.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wqv.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hkg.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uck.haohaochexian.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://byr.hfpthk.cn

[N05] 最大公约数
来源：http://rhp.gzhubu.top

Py:   math.gcd(a, b)
来源：http://ggw.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pxq.ydzc1.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vbt.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lwh.fzhhl.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xdo.epnwcf.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://adf.gogol.net.cn

Ruby: a.gcd(b)
来源：http://ihq.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://icy.cheryme.top

[N06] 判断回文字符串
来源：http://jsw.mhx1999.top

Py:   s == s[::-1]
来源：http://nxh.yvedp.cn

PHP:  $s === strrev($s);
来源：http://nrb.ydzc1.top

JS:   s === [...s].reverse().join("")
来源：http://vvg.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://gtr.ehwqpu.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wgm.yuxming.cn

Go:   // 双指针从两端比较
来源：http://gvg.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://ptk.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://zne.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://idb.52xcode.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://btm.zdqjudy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mgd.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ggv.smart0.xyz

TS:   // 手写 Map<string, number>
来源：http://mac.zhaomingkeji.xyz

Java: // 手写 HashMap
来源：http://umk.shuidangran.top

Go:   // 手写 map[int]int
来源：http://ywq.yj20258888.top

Ruby: // 手写 Hash
来源：http://pqg.xinyue.icu

C#:   // 手写 Dictionary<int, int>
来源：http://cef.sweek.top

[N08] 生成全排列
来源：http://sdn.quarkkingdee.top

Py:   itertools.permutations(arr)
来源：http://yjo.zdqjudy.top

PHP:  // 手写递归交换
来源：http://kon.9152youxi.cn

JS:   // 手写回溯递归
来源：http://jke.yj20258.top

TS:   // 手写回溯递归
来源：http://zpz.hcnkem.com

Java: // 手写回溯递归
来源：http://fxh.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://orh.hammf.cn

Ruby: arr.permutation.to_a
来源：http://krn.meibo888.top

C#:   // 手写回溯递归
来源：http://izp.tianlin.xyz

[N09] 栈与队列
来源：http://qfd.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rbd.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kub.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eas.hywenlv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://omu.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wqg.hywenlv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bok.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hxq.cashguo.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lml.zhixingplan.top

[N10] 链表节点定义
来源：http://ayf.wangdashe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uvu.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wox.zhiwuduotai.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ghg.guannengcc.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://icd.tarul.cn

Java: class Node { int v; Node next; }
来源：http://fjz.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://vqp.zhongyouzk.top

Ruby: Node = Struct.new(:v, :next)
来源：http://awe.xuanzx.com

C#:   class Node { public int V; public Node? Next; }
来源：http://fqz.tarul.cn

[N11] 二叉树中序遍历
来源：http://ksa.sjlbkw.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://krn.tarul.cn

PHP:  // 手写递归函数
来源：http://olp.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fuo.tanke756.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://guc.zhixingplan.top

Java: // 手写递归
来源：http://jum.shzxlz.cn

Go:   // 手写递归
来源：http://wrn.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ykn.cucudq.cn

C#:   // 手写递归
来源：http://aut.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ccp.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://smx.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://utv.shangyingyoupin.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ahn.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://afk.andypj.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kod.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://czq.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ykw.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dco.jqgufenzy.top

================================================================================
来源：http://rmr.shanyushiyangtech.top

O. 并发与异步
来源：http://wrq.yonumen.top

================================================================================
来源：http://msy.epnwcf.com

[O01] 启动一个线程
来源：http://fbz.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://toy.aizwys.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yhl.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://osw.feifeiyinyue.top

TS:   // 同 JS
来源：http://uek.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://iec.yvedp.cn

Go:   go f()
来源：http://okm.yfazqb.com

Ruby: Thread.new { f }
来源：http://uhn.jinyuanbaomall.cn

C#:   Task.Run(() => F());
来源：http://cdu.hesvh.cn

[O02] 使用线程池
来源：http://fkr.fzhhl.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kdn.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vxp.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://llg.yj20258888.top

TS:   // worker_threads 线程池
来源：http://fki.zhongyouzk.top

Java: Executors.newFixedThreadPool(4)
来源：http://iap.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ihq.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xls.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://krp.redwolf501.top

[O03] 加锁保护共享数据
来源：http://quz.zhixingplan.top

Py:   with lock: shared += 1
来源：http://vte.nanxinkj.top

PHP:  // 用 flock() 做文件锁
来源：http://zbe.hysaishi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zuk.fzhhl.top

TS:   // 同 JS
来源：http://qjw.cucudq.cn

Java: synchronized (this) { shared++; }
来源：http://kde.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jbj.feifeiyinyue.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ipk.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://dwn.cheryme.top

[O04] 定义异步函数并等待
来源：http://qxu.zdqjudy.top

Py:   async def f():⏎    await g()
来源：http://mej.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ief.smart0.xyz

JS:   async function f() { await g(); }
来源：http://bnk.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qat.vehdjk.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qnn.ydzc1.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rwr.hnqzz.top

Ruby: # 用 Fiber 或 async gem
来源：http://wge.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://bok.zdbjq.cn

[O05] 并发执行并等待全部完成
来源：http://efz.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://ymh.sweek.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vpi.sysykeji.top

JS:   await Promise.all(tasks)
来源：http://zdk.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://tkt.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mrl.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rio.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://ttk.9152youxi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pmi.bjfxy.top

[O06] 使用进程池
来源：http://rdl.shzxlz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bpv.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://hrv.sxryk.cn

JS:   // child_process / cluster 模块
来源：http://vrs.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://jdx.hfpthk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uvt.sxryk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://utx.jinqigfzy.top

Ruby: // fork 块
来源：http://jju.nanxuanxn.top

C#:   Parallel.For
来源：http://ddv.pengpengdd.cyou

================================================================================
来源：http://zyp.gotoacloud.top

P. 常用工具函数
来源：http://dui.cucudq.cn

================================================================================
来源：http://lts.cheryme.top

[P01] 生成 UUID
来源：http://huf.0kj1m.cn

Py:   str(uuid.uuid4())
来源：http://sjr.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gvo.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://ffj.hcnkem.com

TS:   crypto.randomUUID()
来源：http://mhj.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://ntb.tarul.cn

Go:   // 用 github.com/google/uuid
来源：http://gfw.316326.xyz

Ruby: SecureRandom.uuid
来源：http://uod.c1oappe.top

C#:   Guid.NewGuid().ToString()
来源：http://xmn.zdqjudy.top

[P02] MD5 / SHA256 摘要
来源：http://wmi.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xpj.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cmx.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://std.ywan-chungtsiang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vqu.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cgm.wangshuangyany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ptx.jinyuanbaomall.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hbd.hammf.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ltn.epnwcf.com

[P03] 生成短随机字符串
来源：http://sfs.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qld.chenjidiqi.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lsv.dashuyun.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zcw.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hpf.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blh.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dnl.nanxinkj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hfr.fengsongda.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yny.shangyingyoupin.top

[P04] 求长度
来源：http://qka.nwbrower.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rzt.aibaodan.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kpa.pengpengdd.cyou

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kmd.0kj1m.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qux.epnwcf.com

Java: list.size();  map.size();  s.length()
来源：http://ktq.tian-w.cn

Go:   len(arr);  len(m)
来源：http://eme.uphjek.com

Ruby: x.length;  x.size
来源：http://xje.nwbrower.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rvm.hnqzz.top

[P05] 判断两个对象内容是否相等
来源：http://fcx.gotoacloud.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bna.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xcw.aizwys.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jka.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jcx.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ixa.jqgfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://des.birdmap.top

Ruby: a == b
来源：http://fir.cucudq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nqy.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ocg.gotoacloud.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yqv.zhijiandao.cn

PHP:  if (empty($x)) {}
来源：http://lcf.feifeiyinyue.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tzc.daria6918.cn

TS:   if (x == null) {}
来源：http://omd.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://bid.xylfe.cn

Go:   if x == nil {}
来源：http://vhw.cheryme.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lkc.fanxiaobao.xyz

C#:   if (x is null) {}
来源：http://pru.yangfankeji.com

[P07] 防抖与节流
来源：http://wys.nanxinkj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xao.pengpengdd.cyou

PHP:  // 手写时间戳比较
来源：http://vto.jiagoushi.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oxw.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vdn.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dgx.cheryme.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://trb.fanxiaobao.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://wyd.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gzg.yj20258888.top

[P08] 处理浮点精度问题
来源：http://orh.dianchejie.cn


<!-- 参考信息 -->