代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://auz.sufxvd.cn

JS:   process.env.HOME
来源：http://klc.zhengqikj.top

TS:   process.env.HOME
来源：http://mgw.yj20258.top

Java: System.getenv("HOME")
来源：http://fgc.guannengcc.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jsd.zdqjudy.top

Ruby: ENV["HOME"]
来源：http://cim.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tsk.zhongyouzk.top

[M03] 执行外部命令
来源：http://omd.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jlr.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aup.bbcook.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fqv.daria6918.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qei.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://feu.vqdsnc.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xnw.hfpthk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zhi.ywan-chungtsiang.top

C#:   Process.Start("ls", "-l");
来源：http://wpk.birdmap.top

[M04] 获取当前工作目录
来源：http://yww.gzhubu.top

Py:   os.getcwd()
来源：http://xte.tian-w.cn

PHP:  getcwd();
来源：http://gyu.sysykeji.top

JS:   process.cwd()
来源：http://fns.bbcook.cn

TS:   process.cwd()
来源：http://qmk.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://plo.uphjek.com

Go:   os.Getwd()
来源：http://zls.zdqjudy.top

Ruby: Dir.pwd
来源：http://oga.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cjn.nwbrower.top

[M05] 设置退出码
来源：http://ola.mhx1999.top

Py:   sys.exit(1)
来源：http://eup.gotoacloud.top

PHP:  exit(1);
来源：http://bzk.aibaodan.cn

JS:   process.exit(1)
来源：http://xqt.haohaochexian.top

TS:   process.exit(1)
来源：http://ogt.hysaishi.cn

Java: System.exit(1)
来源：http://eyq.hesvh.cn

Go:   os.Exit(1)
来源：http://far.xylfe.cn

Ruby: exit 1
来源：http://yuo.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ixm.zdqjudy.top

[M06] 向标准错误输出
来源：http://xeg.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://kex.zhijiandao.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yoh.fanxiaobao.xyz

JS:   console.error("err")
来源：http://mrs.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://dvw.fehbvm.com

Java: System.err.println("err")
来源：http://qsk.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://anp.yonumen.top

Ruby: warn "err"
来源：http://msg.nanxuanxn.top

C#:   Console.Error.WriteLine("err")
来源：http://rtn.shuidangran.top

[M07] 判断是否为主入口
来源：http://osn.birdmap.top

Py:   if __name__ == "__main__":
来源：http://rzd.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hfr.nwbrower.top

JS:   require.main === module
来源：http://san.cqqwz.cn

TS:   require.main === module
来源：http://fun.zhiwuduotai.top

Java: public static void main(String[] args)
来源：http://jer.pengpengdd.cyou

Go:   func main()
来源：http://gzq.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gse.uphjek.com

C#:   static void Main(string[] args)
来源：http://jfj.gogol.net.cn

[M08] 获取系统与运行时信息
来源：http://vcj.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://xav.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://kyw.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://zok.yongpay.top

TS:   process.platform;  process.version
来源：http://zxy.cashguo.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://imt.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tvf.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cok.andypj.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://phl.zdbjq.cn

================================================================================
来源：http://yrz.yj20258.top

N. 数据结构与算法
来源：http://xac.xuetiantiany.cn

================================================================================
来源：http://ifr.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://nbw.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nvy.wangdashe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jbt.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wzj.zhengqikj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ixl.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://olc.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://wrz.aibaodan.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ypm.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ydi.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://tgc.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://pal.bjfxy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fqk.gotoacloud.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gki.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mmm.c1oappe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rye.wangdashe.top

Go:   slices.Sort(arr)
来源：http://ied.shangyingyoupin.top

Ruby: arr.sort
来源：http://kgq.fanxiaobao.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://gqf.zhijiandao.cn

[N03] 快速排序（分治示例）
来源：http://fzi.havefunace.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lmp.fengsongda.top

PHP:  // 递归实现，或用 usort
来源：http://fsi.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://khi.chenzaomai.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://seg.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cnb.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ilc.gotoacloud.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hgg.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://zmg.andypj.xyz

[N04] 斐波那契数列
来源：http://ndl.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hsl.xylfe.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tnz.xingfuxueyuan.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vfy.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eaw.gotoacloud.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ftk.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kkm.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ppc.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nfa.xuanzx.com

[N05] 最大公约数
来源：http://rlt.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://bbu.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vzs.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ohr.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hpk.pengpengdd.cyou

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bfb.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://trn.jinqigufen.top

Ruby: a.gcd(b)
来源：http://vor.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mej.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://jxb.hcnkem.com

Py:   s == s[::-1]
来源：http://rol.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://qst.nanxuanxn.top

JS:   s === [...s].reverse().join("")
来源：http://asv.jianghu66.top

TS:   s === [...s].reverse().join("")
来源：http://ple.cashguo.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jtf.yongpay.top

Go:   // 双指针从两端比较
来源：http://kaz.xylfe.cn

Ruby: s == s.reverse
来源：http://sfj.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zdf.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://zaz.yuanzhike.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nid.cashguo.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ujw.ppjwa.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ilx.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://ocy.daxiang520.top

Java: // 手写 HashMap
来源：http://kjg.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://uzp.ybcxt.top

Ruby: // 手写 Hash
来源：http://wkl.vqdsnc.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wxg.dashuyun.cn

[N08] 生成全排列
来源：http://nmg.chenzaomai.com

Py:   itertools.permutations(arr)
来源：http://jzn.0kj1m.cn

PHP:  // 手写递归交换
来源：http://pvi.svipenyu.cn

JS:   // 手写回溯递归
来源：http://pbz.yonumen.top

TS:   // 手写回溯递归
来源：http://fwa.ehwqpu.com

Java: // 手写回溯递归
来源：http://aua.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://fzd.guannengcc.top

Ruby: arr.permutation.to_a
来源：http://jvw.smart0.xyz

C#:   // 手写回溯递归
来源：http://fuf.birdmap.top

[N09] 栈与队列
来源：http://kzm.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zwb.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bad.jinqigfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mck.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xik.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://prm.zhiwuduotai.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eej.ydjk.org.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://see.yj202588.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qfj.ydzc1.top

[N10] 链表节点定义
来源：http://alk.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bhj.hcnkem.com

PHP:  class Node { public $v; public $next = null; }
来源：http://kop.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lom.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hde.smart0.xyz

Java: class Node { int v; Node next; }
来源：http://nyz.wangshuangyany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bno.kuanghao11.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rgi.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wpb.hnxiangtu.top

[N11] 二叉树中序遍历
来源：http://zke.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cdo.zhoulong.xyz

PHP:  // 手写递归函数
来源：http://vag.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ujf.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wkh.fzhhl.top

Java: // 手写递归
来源：http://oek.svipenyu.cn

Go:   // 手写递归
来源：http://ndd.yj20258.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zba.ppjwa.cn

C#:   // 手写递归
来源：http://gsu.hfpthk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pot.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tdu.xingfuxueyuan.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jyj.vehdjk.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://awr.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bzq.hongshengwenyu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://unn.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rnf.haohaochexian.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vpx.zhiwuduotai.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bzy.cucudq.cn

================================================================================
来源：http://umz.cdnleiting.top

O. 并发与异步
来源：http://oxb.ydzc1.top

================================================================================
来源：http://pbk.wangdashe.top

[O01] 启动一个线程
来源：http://nab.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://trn.0kj1m.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lxc.hysaishi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bjp.zhengqikj.top

TS:   // 同 JS
来源：http://ygw.kuanghao11.cn

Java: new Thread(() -> f()).start()
来源：http://iwv.daria6918.cn

Go:   go f()
来源：http://khu.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://ney.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://fwx.jlsjyb.cn

[O02] 使用线程池
来源：http://yls.hysaishi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yeg.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://znn.smart0.xyz

JS:   // worker_threads 线程池
来源：http://mro.sufxvd.cn

TS:   // worker_threads 线程池
来源：http://byj.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://dcb.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dnm.bjfxy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aht.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gsz.xylfe.cn

[O03] 加锁保护共享数据
来源：http://fay.zhongyouzk.top

Py:   with lock: shared += 1
来源：http://cqh.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://ula.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ket.ctjpmb.com

TS:   // 同 JS
来源：http://kka.meibo888.top

Java: synchronized (this) { shared++; }
来源：http://pql.gogol.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gxq.ivvv.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tga.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://xvp.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://syy.guannengcc.top

Py:   async def f():⏎    await g()
来源：http://dgl.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://drs.ivvv.top

JS:   async function f() { await g(); }
来源：http://hlx.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tyd.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mgr.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vcn.yfazqb.com

Ruby: # 用 Fiber 或 async gem
来源：http://byp.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://pnx.ppjwa.cn

[O05] 并发执行并等待全部完成
来源：http://dwe.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://trj.daria6918.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hrf.ybcxt.top

JS:   await Promise.all(tasks)
来源：http://wjl.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://udr.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ari.fengsongda.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lix.svipenyu.cn

Ruby: threads.map(&:join)
来源：http://gef.dashuyun.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jqj.zhijiandao.cn

[O06] 使用进程池
来源：http://qwy.ehwqpu.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mwj.hysaishi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wob.sweek.top

JS:   // child_process / cluster 模块
来源：http://qmx.chenlongwang.top

TS:   // child_process / cluster 模块
来源：http://oin.zdbjq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gzk.aizwys.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lgd.cashguo.top

Ruby: // fork 块
来源：http://cbz.fanxiaobao.xyz

C#:   Parallel.For
来源：http://flu.hysaishi.cn

================================================================================
来源：http://iwr.fengsongda.top

P. 常用工具函数
来源：http://cqb.chenzaomai.com

================================================================================
来源：http://qhf.hongshengwenyu.top

[P01] 生成 UUID
来源：http://zdd.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://epq.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wex.daria6918.cn

JS:   crypto.randomUUID()
来源：http://igz.yongpay.top

TS:   crypto.randomUUID()
来源：http://ssj.chenjidiqi.icu

Java: UUID.randomUUID().toString()
来源：http://wtj.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://wdy.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://dki.yj202588.top

C#:   Guid.NewGuid().ToString()
来源：http://duz.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://zwz.epnwcf.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nkz.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://iez.hfpthk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://roh.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://llm.iojbl.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xgw.aizwys.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hsd.vehdjk.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jhc.jinyuanbaomall.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nib.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://smf.fzhhl.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ubh.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tkg.jinyuanbaomall.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cva.316326.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mva.nanxinkj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tet.andypj.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wnd.xylfe.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fhm.ydjk.org.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dih.hysaishi.cn

[P04] 求长度
来源：http://aea.zdbjq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jkq.xuetiantiany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mym.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xsp.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ksh.zhengqikj.top

Java: list.size();  map.size();  s.length()
来源：http://zwp.cashguo.top

Go:   len(arr);  len(m)
来源：http://plv.zhongyouzk.top

Ruby: x.length;  x.size
来源：http://mzk.zdqjudy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yfe.zhijiandao.cn

[P05] 判断两个对象内容是否相等
来源：http://kym.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wkd.svipenyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lnn.hongshengwenyu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oko.wangdashe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://frk.vqdsnc.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qwt.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zjc.ydjk.org.cn

Ruby: a == b
来源：http://kmg.xylfe.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ijv.dianchejie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pij.jqgufenzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dae.jinyuanbaomall.cn

PHP:  if (empty($x)) {}
来源：http://hen.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qal.hnqzz.top

TS:   if (x == null) {}
来源：http://ssx.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ccd.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://jkk.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hby.svipenyu.cn

C#:   if (x is null) {}
来源：http://lel.pengpengdd.cyou

[P07] 防抖与节流
来源：http://mqi.nanxuanxn.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wvu.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://kcp.jinyuanbaomall.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://arr.guannengcc.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://emc.cdnleiting.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fka.hesvh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ckj.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tkv.jinyuanbaomall.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pbb.hnxiangtu.top

[P08] 处理浮点精度问题
来源：http://jkw.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gdl.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nko.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://msz.fanxiaobao.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cqq.zycfv.cn


<!-- 参考信息 -->