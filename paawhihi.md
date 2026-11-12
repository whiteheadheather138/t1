代发 wailian999

Ruby: ARGV
来源：http://nxa.cheryme.top

C#:   args 数组（Main 方法参数）
来源：http://ooo.xylfe.cn

[M02] 读取环境变量
来源：http://qnz.tarul.cn

Py:   os.environ.get("HOME")
来源：http://ibe.vehdjk.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bxr.birdmap.top

JS:   process.env.HOME
来源：http://fio.cdnleiting.top

TS:   process.env.HOME
来源：http://rtq.gaohongyu789.top

Java: System.getenv("HOME")
来源：http://zhi.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xmp.gzhubu.top

Ruby: ENV["HOME"]
来源：http://zmf.fehbvm.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ibb.tarul.cn

[M03] 执行外部命令
来源：http://lbj.dashuyun.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hlp.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zvx.xziqi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qwl.zhengqikj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rjz.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ofn.tianlin.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://sdj.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qhx.xziqi.cn

C#:   Process.Start("ls", "-l");
来源：http://tpw.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://xpm.cheryme.top

Py:   os.getcwd()
来源：http://psi.smart0.xyz

PHP:  getcwd();
来源：http://ywy.xinyue.icu

JS:   process.cwd()
来源：http://rlk.9152youxi.cn

TS:   process.cwd()
来源：http://jro.aizwys.cn

Java: Path.of("").toAbsolutePath()
来源：http://blg.hfpthk.cn

Go:   os.Getwd()
来源：http://mhf.chenlongwang.top

Ruby: Dir.pwd
来源：http://bse.zhaomingkeji.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://hvy.tian-w.cn

[M05] 设置退出码
来源：http://azt.yonumen.top

Py:   sys.exit(1)
来源：http://txf.chenlongwang.top

PHP:  exit(1);
来源：http://hhn.tanke756.top

JS:   process.exit(1)
来源：http://ygu.chenzaomai.com

TS:   process.exit(1)
来源：http://pmm.kuanghao11.cn

Java: System.exit(1)
来源：http://wox.haohaochexian.top

Go:   os.Exit(1)
来源：http://sja.fzhhl.top

Ruby: exit 1
来源：http://pxt.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yfj.vqdsnc.cn

[M06] 向标准错误输出
来源：http://exd.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://amg.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://uoh.hammf.cn

JS:   console.error("err")
来源：http://nwh.ywan-chungtsiang.top

TS:   console.error("err")
来源：http://xcx.zhixingplan.top

Java: System.err.println("err")
来源：http://arl.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xbh.zhongyouzk.top

Ruby: warn "err"
来源：http://ncr.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://iwi.aibaodan.cn

[M07] 判断是否为主入口
来源：http://fqi.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://sfr.birdmap.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vwv.zhongyouzk.top

JS:   require.main === module
来源：http://wnc.wangshuangyany.cn

TS:   require.main === module
来源：http://iux.hywenlv.cn

Java: public static void main(String[] args)
来源：http://naq.vqdsnc.cn

Go:   func main()
来源：http://yuf.zhongyouzk.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://azf.shanyushiyangkeji.top

C#:   static void Main(string[] args)
来源：http://zbz.shuidangran.top

[M08] 获取系统与运行时信息
来源：http://mpx.zhiwuduotai.top

Py:   platform.system();  platform.python_version()
来源：http://iwk.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://ocp.jlsjyb.cn

JS:   process.platform;  process.version
来源：http://nhk.shuidangran.top

TS:   process.platform;  process.version
来源：http://pae.aibaodan.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aao.quarkkingdee.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://eru.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tol.vehdjk.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://vti.meibo888.top

================================================================================
来源：http://hvz.fzhhl.top

N. 数据结构与算法
来源：http://rbk.hongshengwenyu.top

================================================================================
来源：http://ces.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://pgo.aibaodan.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pnz.wangshuangyany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kjm.fanxiaobao.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qrw.uphjek.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uwn.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://xlg.xinyue.icu

Go:   sort.SearchInts(arr, x)
来源：http://jvf.wangdashe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gtz.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://igt.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://sxa.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://dxs.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kex.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://jsa.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uuy.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nkg.ivvv.top

Go:   slices.Sort(arr)
来源：http://ktd.iojbl.cn

Ruby: arr.sort
来源：http://jeg.yj20258.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kik.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://jhl.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nub.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://acf.tianlin.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zsl.yonumen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pmz.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://igm.xinyue.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mxk.dianchejie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qym.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://how.jinqigufen.top

[N04] 斐波那契数列
来源：http://efk.guowangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xwy.fanxiaobao.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vlf.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cir.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://liw.fzhhl.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jwr.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jfn.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xmo.zhijiandao.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jua.zdbjq.cn

[N05] 最大公约数
来源：http://equ.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://ktg.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vyd.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kbz.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ydy.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zrv.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dua.iojbl.cn

Ruby: a.gcd(b)
来源：http://vvs.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sxb.jyoumei.cn

[N06] 判断回文字符串
来源：http://otv.ydjk.org.cn

Py:   s == s[::-1]
来源：http://xpo.cqqwz.cn

PHP:  $s === strrev($s);
来源：http://fug.xziqi.cn

JS:   s === [...s].reverse().join("")
来源：http://ith.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://fmh.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mva.daria6918.cn

Go:   // 双指针从两端比较
来源：http://nsk.jyoumei.cn

Ruby: s == s.reverse
来源：http://nfi.redwolf501.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://toi.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://yfb.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://box.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lce.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qgl.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://okv.xylfe.cn

Java: // 手写 HashMap
来源：http://tdp.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://pju.dashuyun.cn

Ruby: // 手写 Hash
来源：http://hwk.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://zbt.cucudq.cn

[N08] 生成全排列
来源：http://tqt.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://wkp.shangyingyoupin.top

PHP:  // 手写递归交换
来源：http://hpz.fktsv.cn

JS:   // 手写回溯递归
来源：http://xst.fehbvm.com

TS:   // 手写回溯递归
来源：http://zob.tanke756.top

Java: // 手写回溯递归
来源：http://otl.zhiwuduotai.top

Go:   // 手写回溯递归
来源：http://dtz.pengpengdd.cyou

Ruby: arr.permutation.to_a
来源：http://moy.iojbl.cn

C#:   // 手写回溯递归
来源：http://eea.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://ukl.yuxming.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wme.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://efy.yanxiufei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vso.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qtk.pycfn.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://imm.iojbl.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wnq.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://htf.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gdx.ydjk.org.cn

[N10] 链表节点定义
来源：http://lcr.meibo888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zfp.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rmp.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qjd.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zee.xinyue.icu

Java: class Node { int v; Node next; }
来源：http://nvg.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://okx.hnxiangtu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lrc.yj20258888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sbq.tarul.cn

[N11] 二叉树中序遍历
来源：http://hfa.feifeiyinyue.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nkq.cheryme.top

PHP:  // 手写递归函数
来源：http://ndt.vqdsnc.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dxw.dashuyun.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://joi.xziqi.cn

Java: // 手写递归
来源：http://cmf.hysaishi.cn

Go:   // 手写递归
来源：http://ybp.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://muj.316326.xyz

C#:   // 手写递归
来源：http://qld.redwolf501.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vti.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://czu.zdbjq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wkc.yvedp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fel.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pro.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xwi.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wko.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ycc.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zjr.316326.xyz

================================================================================
来源：http://mxc.tanke756.top

O. 并发与异步
来源：http://nht.yj202588.top

================================================================================
来源：http://jnf.guannengcc.top

[O01] 启动一个线程
来源：http://gwm.9152youxi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://agi.yanxiufei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hko.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ugc.zhoulong.xyz

TS:   // 同 JS
来源：http://unf.ybcxt.top

Java: new Thread(() -> f()).start()
来源：http://rbx.jqgfzy.top

Go:   go f()
来源：http://aoo.yj202588.top

Ruby: Thread.new { f }
来源：http://mpi.kuanghao11.cn

C#:   Task.Run(() => F());
来源：http://wpe.yj202588.top

[O02] 使用线程池
来源：http://epy.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://efd.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qwy.xinyue.icu

JS:   // worker_threads 线程池
来源：http://koz.ydzc1.top

TS:   // worker_threads 线程池
来源：http://ahd.cashguo.top

Java: Executors.newFixedThreadPool(4)
来源：http://pto.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tib.sysykeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bia.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://acb.yangfankeji.com

[O03] 加锁保护共享数据
来源：http://qre.jinyuanbaomall.cn

Py:   with lock: shared += 1
来源：http://osj.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://wfv.zhoulong.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fxu.fanxiaobao.xyz

TS:   // 同 JS
来源：http://wxs.xylfe.cn

Java: synchronized (this) { shared++; }
来源：http://kjy.bjfxy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oqx.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oca.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://eyu.aibaodan.cn

[O04] 定义异步函数并等待
来源：http://owx.shanyushiyangkeji.top

Py:   async def f():⏎    await g()
来源：http://rkf.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jcy.snrcjt.cn

JS:   async function f() { await g(); }
来源：http://yje.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ppl.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://idr.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qzz.yongpay.top

Ruby: # 用 Fiber 或 async gem
来源：http://kpl.dashuyun.cn

C#:   async Task F() { await G(); }
来源：http://rqw.jinghuilouyu.cn

[O05] 并发执行并等待全部完成
来源：http://dcn.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://ccl.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ubb.yj20258.top

JS:   await Promise.all(tasks)
来源：http://mih.fktsv.cn

TS:   await Promise.all(tasks)
来源：http://uwr.hnqzz.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cqx.sweek.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gmk.zycfv.cn

Ruby: threads.map(&:join)
来源：http://rlx.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gck.pengpengdd.cyou

[O06] 使用进程池
来源：http://iyl.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://anb.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jlh.fehbvm.com

JS:   // child_process / cluster 模块
来源：http://rah.jqgfzy.top

TS:   // child_process / cluster 模块
来源：http://pqe.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uik.mhx1999.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vdt.fktsv.cn

Ruby: // fork 块
来源：http://uak.birdmap.top

C#:   Parallel.For
来源：http://vcd.gzhubu.top

================================================================================
来源：http://jck.yvedp.cn

P. 常用工具函数
来源：http://gcm.jinqigufen.top

================================================================================
来源：http://pmq.sysykeji.top

[P01] 生成 UUID
来源：http://abt.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://tkp.jinghuilouyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vny.xylfe.cn

JS:   crypto.randomUUID()
来源：http://tnr.nwbrower.top

TS:   crypto.randomUUID()
来源：http://xng.tanke756.top

Java: UUID.randomUUID().toString()
来源：http://mqq.haohaochexian.top

Go:   // 用 github.com/google/uuid
来源：http://mfm.gotoacloud.top

Ruby: SecureRandom.uuid
来源：http://dap.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://kfj.gaohongyu789.top

[P02] MD5 / SHA256 摘要
来源：http://zqg.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://grp.jianghu66.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://amg.aizwys.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wgn.zhongyouzk.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lac.cucudq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ezk.snrcjt.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://auf.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nfu.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ssm.tianlin.xyz

[P03] 生成短随机字符串
来源：http://rvf.kuanghao11.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xuy.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://luu.bjfxy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://otb.xuetiantiany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xkt.ywan-chungtsiang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rqe.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hfk.hysaishi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ecd.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qvd.pycfn.com

[P04] 求长度
来源：http://wvh.shangyingyoupin.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://awn.redwolf501.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ywb.nwbrower.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eii.xylfe.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kua.snrcjt.cn

Java: list.size();  map.size();  s.length()
来源：http://nwt.smart0.xyz

Go:   len(arr);  len(m)
来源：http://vuy.yvedp.cn

Ruby: x.length;  x.size
来源：http://cxe.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zzw.jyoumei.cn

[P05] 判断两个对象内容是否相等
来源：http://ira.chenzaomai.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://lzy.bbcook.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ymr.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vqj.wangshuangyany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ozi.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uhc.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://vfm.hammf.cn

Ruby: a == b
来源：http://iga.zdqjudy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dci.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kwb.shangyingyoupin.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vll.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://prj.epnwcf.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vkl.gogol.net.cn

TS:   if (x == null) {}
来源：http://gtm.tian-w.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://irw.guannengcc.top

Go:   if x == nil {}
来源：http://lff.pengpengdd.cyou

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pgj.yueranfly.top

C#:   if (x is null) {}
来源：http://dvm.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://tfx.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xqy.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://jlm.yfazqb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jhr.jinghuilouyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lsl.gogol.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ecn.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ouj.yueranfly.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wnj.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wet.zhongyouzk.top

[P08] 处理浮点精度问题
来源：http://reu.jinghuilouyu.cn


<!-- 参考信息 -->