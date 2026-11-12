代发 wailian999

Ruby: ARGV
来源：http://rtt.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://gbb.yj202588.top

[M02] 读取环境变量
来源：http://jpe.havefunace.top

Py:   os.environ.get("HOME")
来源：http://ldc.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yye.ctjpmb.com

JS:   process.env.HOME
来源：http://pig.ppjwa.cn

TS:   process.env.HOME
来源：http://lzg.cqqwz.cn

Java: System.getenv("HOME")
来源：http://meh.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://urk.havefunace.top

Ruby: ENV["HOME"]
来源：http://pjl.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://okz.52xcode.cn

[M03] 执行外部命令
来源：http://ifm.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bxd.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oag.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://caa.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://djw.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mst.pycfn.com

Go:   exec.Command("ls", "-l").Output()
来源：http://wjz.hongshengwenyu.top

Ruby: system("ls -l");  `ls -l`
来源：http://xqd.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://sww.jinqigfzy.top

[M04] 获取当前工作目录
来源：http://vyn.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://mac.uphjek.com

PHP:  getcwd();
来源：http://ruj.xylfe.cn

JS:   process.cwd()
来源：http://gtp.hcnkem.com

TS:   process.cwd()
来源：http://bvr.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://ruf.9152youxi.cn

Go:   os.Getwd()
来源：http://goo.chenzaomai.com

Ruby: Dir.pwd
来源：http://pon.jlsjyb.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pqi.jqgfzy.top

[M05] 设置退出码
来源：http://wel.ybcxt.top

Py:   sys.exit(1)
来源：http://ril.svipenyu.cn

PHP:  exit(1);
来源：http://iqb.fktsv.cn

JS:   process.exit(1)
来源：http://eew.xylfe.cn

TS:   process.exit(1)
来源：http://lpj.guowangkeji.top

Java: System.exit(1)
来源：http://zyq.dianchejie.cn

Go:   os.Exit(1)
来源：http://qkk.hammf.cn

Ruby: exit 1
来源：http://fvq.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://klv.xylfe.cn

[M06] 向标准错误输出
来源：http://xej.tanke756.top

Py:   print("err", file=sys.stderr)
来源：http://jzg.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rqj.jinqigfzy.top

JS:   console.error("err")
来源：http://dja.guowangkeji.top

TS:   console.error("err")
来源：http://cev.xingfuxueyuan.xyz

Java: System.err.println("err")
来源：http://yvb.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://flt.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://oes.andypj.xyz

C#:   Console.Error.WriteLine("err")
来源：http://jzq.redwolf501.top

[M07] 判断是否为主入口
来源：http://hep.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://fvq.guannengcc.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qjj.feifeiyinyue.top

JS:   require.main === module
来源：http://eig.redwolf501.top

TS:   require.main === module
来源：http://kny.jinghuilouyu.cn

Java: public static void main(String[] args)
来源：http://hiq.yanxiufei.cn

Go:   func main()
来源：http://ckn.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tgy.jqgfzy.top

C#:   static void Main(string[] args)
来源：http://twf.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://rxy.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://dnw.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://inl.jinqigfzy.top

JS:   process.platform;  process.version
来源：http://iis.zhengqikj.top

TS:   process.platform;  process.version
来源：http://bxa.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ibe.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gfj.nanxuanxn.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sut.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dbn.birdmap.top

================================================================================
来源：http://avr.yanxiufei.cn

N. 数据结构与算法
来源：http://mrh.yuanzhike.top

================================================================================
来源：http://att.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://tqk.chenlongwang.top

Py:   bisect.bisect_left(arr, x)
来源：http://fgy.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tio.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fst.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://emm.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://vlc.gzhubu.top

Go:   sort.SearchInts(arr, x)
来源：http://xpr.ctjpmb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://hlo.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ehm.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://fmo.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://wtb.hysaishi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sdp.tianlin.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://glt.xingfuxueyuan.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://eef.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ely.redwolf501.top

Go:   slices.Sort(arr)
来源：http://rzc.fktsv.cn

Ruby: arr.sort
来源：http://glv.feifeiyinyue.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://abs.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://ddg.sxryk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://psb.svipenyu.cn

PHP:  // 递归实现，或用 usort
来源：http://jiw.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rhj.shangyingyoupin.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zuf.tarul.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iqt.zhixingplan.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ffr.ctjpmb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yko.daria6918.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gwx.chenlongwang.top

[N04] 斐波那契数列
来源：http://iwe.svipenyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dwn.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zzi.yanxiufei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vba.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vbf.daxiang520.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pdw.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mpv.chenlongwang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qvh.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fui.hywenlv.cn

[N05] 最大公约数
来源：http://mzg.hongshengwenyu.top

Py:   math.gcd(a, b)
来源：http://pec.sufxvd.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jmd.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rfo.hfpthk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://prx.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://whi.9152youxi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xvc.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://pjg.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tob.havefunace.top

[N06] 判断回文字符串
来源：http://emu.pycfn.com

Py:   s == s[::-1]
来源：http://uvi.vqdsnc.cn

PHP:  $s === strrev($s);
来源：http://yyt.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://rav.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://php.ybcxt.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hmm.bbcook.cn

Go:   // 双指针从两端比较
来源：http://wvw.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://mav.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kgo.hywenlv.cn

[N07] 两数之和（返回下标）
来源：http://cju.c1oappe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yqm.0kj1m.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://teb.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vfc.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://cnl.vqdsnc.cn

Java: // 手写 HashMap
来源：http://kaq.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://suq.cheryme.top

Ruby: // 手写 Hash
来源：http://kej.yongpay.top

C#:   // 手写 Dictionary<int, int>
来源：http://ptt.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://kmc.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://hwx.yueranfly.top

PHP:  // 手写递归交换
来源：http://gzn.hnqzz.top

JS:   // 手写回溯递归
来源：http://qcg.xingfuxueyuan.xyz

TS:   // 手写回溯递归
来源：http://gke.fengsongda.top

Java: // 手写回溯递归
来源：http://qer.chenlongwang.top

Go:   // 手写回溯递归
来源：http://svh.xingfuxueyuan.xyz

Ruby: arr.permutation.to_a
来源：http://jko.ivvv.top

C#:   // 手写回溯递归
来源：http://aki.ivvv.top

[N09] 栈与队列
来源：http://zaj.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rsx.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gzf.hammf.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mdt.iojbl.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qvq.bbcook.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wbb.gogol.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wor.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fwq.birdmap.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ajc.hnqzz.top

[N10] 链表节点定义
来源：http://itq.hammf.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://brl.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://pqu.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hjm.yj20258888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pcg.cheryme.top

Java: class Node { int v; Node next; }
来源：http://npt.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pdy.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mzm.cdnleiting.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xsh.zdqjudy.top

[N11] 二叉树中序遍历
来源：http://yjh.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qkx.zhixingplan.top

PHP:  // 手写递归函数
来源：http://zho.yonumen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cto.zhoulong.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://act.sysykeji.top

Java: // 手写递归
来源：http://ryb.gotoacloud.top

Go:   // 手写递归
来源：http://aeg.nwbrower.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yjp.cheryme.top

C#:   // 手写递归
来源：http://vpj.ywan-chungtsiang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ajo.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nhd.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://igk.ppjwa.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vdt.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rgf.hywenlv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oks.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uvu.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pfv.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://abt.sxryk.cn

================================================================================
来源：http://qpp.pycfn.com

O. 并发与异步
来源：http://zuv.zhengqikj.top

================================================================================
来源：http://eug.dianchejie.cn

[O01] 启动一个线程
来源：http://lca.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zwz.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dfs.pycfn.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mzz.xuanzx.com

TS:   // 同 JS
来源：http://cua.gotoacloud.top

Java: new Thread(() -> f()).start()
来源：http://jtv.jinqigufen.top

Go:   go f()
来源：http://wtq.cucudq.cn

Ruby: Thread.new { f }
来源：http://wbd.chenlongwang.top

C#:   Task.Run(() => F());
来源：http://ssh.shanyushiyangtech.top

[O02] 使用线程池
来源：http://ibc.havefunace.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://joh.yongpay.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jwp.zdbjq.cn

JS:   // worker_threads 线程池
来源：http://ywd.shuidangran.top

TS:   // worker_threads 线程池
来源：http://ufp.hammf.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vgc.birdmap.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qva.xuetiantiany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zkf.hongshengwenyu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tre.zhixingplan.top

[O03] 加锁保护共享数据
来源：http://qeh.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://cof.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://koh.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yga.yj20258888.top

TS:   // 同 JS
来源：http://yki.xuanzx.com

Java: synchronized (this) { shared++; }
来源：http://fcj.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cxh.bbcook.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gnm.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://qyh.smart0.xyz

[O04] 定义异步函数并等待
来源：http://leo.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://qiz.daria6918.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dyd.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://xmr.yueranfly.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lvi.chenjidiqi.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oen.yj20258888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uwh.cucudq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://run.daxiang520.top

C#:   async Task F() { await G(); }
来源：http://rvb.dashuyun.cn

[O05] 并发执行并等待全部完成
来源：http://lzt.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://npl.kuanghao11.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vbo.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://mwb.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://meo.jianghu66.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mcv.ctjpmb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lvt.xuetiantiany.cn

Ruby: threads.map(&:join)
来源：http://gap.0kj1m.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jbp.iojbl.cn

[O06] 使用进程池
来源：http://vbb.vehdjk.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ebe.xuetiantiany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fjv.ydjk.org.cn

JS:   // child_process / cluster 模块
来源：http://mih.guannengcc.top

TS:   // child_process / cluster 模块
来源：http://rxr.guannengcc.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://etg.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://buw.quarkkingdee.top

Ruby: // fork 块
来源：http://fuf.tian-w.cn

C#:   Parallel.For
来源：http://zds.gzhubu.top

================================================================================
来源：http://byb.gaohongyu789.top

P. 常用工具函数
来源：http://iju.ehwqpu.com

================================================================================
来源：http://yic.vqdsnc.cn

[P01] 生成 UUID
来源：http://arv.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://ptl.tarul.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ddf.9152youxi.cn

JS:   crypto.randomUUID()
来源：http://llx.shuidangran.top

TS:   crypto.randomUUID()
来源：http://xdb.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://for.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://smv.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://knm.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://oxi.tanke756.top

[P02] MD5 / SHA256 摘要
来源：http://mmv.yvedp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cii.meibo888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://opi.yj20258888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sss.xuetiantiany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cay.yfazqb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rdm.tian-w.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dkk.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wea.gotoacloud.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ifz.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://tna.snrcjt.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://skh.nanxuanxn.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tzb.snrcjt.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pup.jianghu66.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wkq.daxiang520.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aht.haohaochexian.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://emt.c1oappe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://krb.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qsg.havefunace.top

[P04] 求长度
来源：http://kws.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://upy.fehbvm.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rkf.xingfuxueyuan.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vyr.gogol.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://toi.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://rlg.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://jxb.cqqwz.cn

Ruby: x.length;  x.size
来源：http://vom.svipenyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kgn.zhiwuduotai.top

[P05] 判断两个对象内容是否相等
来源：http://fzw.ywan-chungtsiang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wez.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zdn.xingfuxueyuan.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ktu.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hub.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vrt.316326.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://siw.quarkkingdee.top

Ruby: a == b
来源：http://rjm.gaohongyu789.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wjh.gaohongyu789.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hke.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://prh.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://jlu.xuetiantiany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bum.cheryme.top

TS:   if (x == null) {}
来源：http://fkg.sysykeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://afp.ydzc1.top

Go:   if x == nil {}
来源：http://nkw.xylfe.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pye.gaohongyu789.top

C#:   if (x is null) {}
来源：http://ovw.hongshengwenyu.top

[P07] 防抖与节流
来源：http://orx.vqdsnc.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ijw.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://kyw.yonumen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bhb.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yzh.xziqi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bzp.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ert.ehwqpu.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://cnz.yfazqb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eyg.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://vei.yuanzhike.top


<!-- 参考信息 -->