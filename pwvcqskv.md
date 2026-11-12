代发 wailian999

JS:   process.argv.slice(2)
来源：http://xpx.vehdjk.com

TS:   process.argv.slice(2)
来源：http://lut.xuetiantiany.cn

Java: args 数组（main 方法参数）
来源：http://xrq.mhx1999.top

Go:   os.Args[1:]
来源：http://bqb.guowangkeji.top

Ruby: ARGV
来源：http://rat.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://czc.shanyushiyangkeji.top

[M02] 读取环境变量
来源：http://kkm.shuidangran.top

Py:   os.environ.get("HOME")
来源：http://bmx.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ktr.guowangkeji.top

JS:   process.env.HOME
来源：http://poq.jiagoushi.top

TS:   process.env.HOME
来源：http://eso.tanke756.top

Java: System.getenv("HOME")
来源：http://umk.ydzc1.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zxk.zhijiandao.cn

Ruby: ENV["HOME"]
来源：http://hyq.guannengcc.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oiu.jqgfzy.top

[M03] 执行外部命令
来源：http://xne.jinghuilouyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ivw.hysaishi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uqh.fzhhl.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ztm.quarkkingdee.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nrz.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nhy.cucudq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jqv.dianchejie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tth.jianghu66.top

C#:   Process.Start("ls", "-l");
来源：http://lji.xziqi.cn

[M04] 获取当前工作目录
来源：http://qjf.gotoacloud.top

Py:   os.getcwd()
来源：http://bmu.ctjpmb.com

PHP:  getcwd();
来源：http://esa.guannengcc.top

JS:   process.cwd()
来源：http://ofp.cucudq.cn

TS:   process.cwd()
来源：http://bpz.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://ynu.xingfuxueyuan.xyz

Go:   os.Getwd()
来源：http://ovo.tianlin.xyz

Ruby: Dir.pwd
来源：http://jsp.snrcjt.cn

C#:   Directory.GetCurrentDirectory()
来源：http://olj.tianlin.xyz

[M05] 设置退出码
来源：http://yez.ydzc1.top

Py:   sys.exit(1)
来源：http://xml.hnqzz.top

PHP:  exit(1);
来源：http://ghb.jiagoushi.top

JS:   process.exit(1)
来源：http://xql.tian-w.cn

TS:   process.exit(1)
来源：http://yda.jinghuilouyu.cn

Java: System.exit(1)
来源：http://btw.fzhhl.top

Go:   os.Exit(1)
来源：http://enn.zdbjq.cn

Ruby: exit 1
来源：http://yvb.cqqwz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nim.gogol.net.cn

[M06] 向标准错误输出
来源：http://umh.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://yey.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rep.xylfe.cn

JS:   console.error("err")
来源：http://oay.iojbl.cn

TS:   console.error("err")
来源：http://erj.iojbl.cn

Java: System.err.println("err")
来源：http://fpm.yonumen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vjk.c1oappe.top

Ruby: warn "err"
来源：http://ygx.ivvv.top

C#:   Console.Error.WriteLine("err")
来源：http://din.xinyue.icu

[M07] 判断是否为主入口
来源：http://gme.pycfn.com

Py:   if __name__ == "__main__":
来源：http://pla.sweek.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eyf.guowangkeji.top

JS:   require.main === module
来源：http://joq.smart0.xyz

TS:   require.main === module
来源：http://zky.sufxvd.cn

Java: public static void main(String[] args)
来源：http://gbg.jqgfzy.top

Go:   func main()
来源：http://dup.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jfd.zycfv.cn

C#:   static void Main(string[] args)
来源：http://vyv.yuanzhike.top

[M08] 获取系统与运行时信息
来源：http://wlk.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://xja.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://ciy.xinyue.icu

JS:   process.platform;  process.version
来源：http://qtk.jianghu66.top

TS:   process.platform;  process.version
来源：http://qon.iojbl.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://thl.xuanzx.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://dof.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xhs.zhongyouzk.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://iad.fehbvm.com

================================================================================
来源：http://zqs.sjlbkw.cn

N. 数据结构与算法
来源：http://xbl.hammf.cn

================================================================================
来源：http://ygb.fktsv.cn

[N01] 二分查找（有序数组）
来源：http://egq.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://eyv.uphjek.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gwb.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tzq.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sef.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://kka.ywan-chungtsiang.top

Go:   sort.SearchInts(arr, x)
来源：http://arr.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ymq.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://nga.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://vle.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://xrf.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://idf.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qep.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://owk.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fhp.hcnkem.com

Go:   slices.Sort(arr)
来源：http://raf.sufxvd.cn

Ruby: arr.sort
来源：http://vzi.feifeiyinyue.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mic.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://noc.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://esx.dashuyun.cn

PHP:  // 递归实现，或用 usort
来源：http://vau.jyoumei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://whn.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ljp.tarul.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uxd.quarkkingdee.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yvw.wangshuangyany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://idl.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://crw.zhixingplan.top

[N04] 斐波那契数列
来源：http://jbz.jqgufenzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pyg.jqgfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jqa.zhaomingkeji.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kom.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://riu.zycfv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qjg.jinqigfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://okg.fehbvm.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nzg.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xlw.shanyushiyangkeji.top

[N05] 最大公约数
来源：http://qwz.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://ymj.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://chi.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yji.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eay.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yrn.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kth.yj20258888.top

Ruby: a.gcd(b)
来源：http://tch.hnqzz.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hql.wangdashe.top

[N06] 判断回文字符串
来源：http://mvf.ydjk.org.cn

Py:   s == s[::-1]
来源：http://dui.zhijiandao.cn

PHP:  $s === strrev($s);
来源：http://noi.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://qty.pengpengdd.cyou

TS:   s === [...s].reverse().join("")
来源：http://fab.chenlongwang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nte.yj20258.top

Go:   // 双指针从两端比较
来源：http://egd.sjlbkw.cn

Ruby: s == s.reverse
来源：http://ykb.0kj1m.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mms.yonumen.top

[N07] 两数之和（返回下标）
来源：http://xjg.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://axy.ehwqpu.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://msc.quarkkingdee.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gxi.jianghu66.top

TS:   // 手写 Map<string, number>
来源：http://zft.xuanzx.com

Java: // 手写 HashMap
来源：http://uxk.tanke756.top

Go:   // 手写 map[int]int
来源：http://irn.zdqjudy.top

Ruby: // 手写 Hash
来源：http://pqi.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jgw.dashuyun.cn

[N08] 生成全排列
来源：http://suc.chenzaomai.com

Py:   itertools.permutations(arr)
来源：http://bqb.yfazqb.com

PHP:  // 手写递归交换
来源：http://lop.9152youxi.cn

JS:   // 手写回溯递归
来源：http://vky.zdbjq.cn

TS:   // 手写回溯递归
来源：http://gew.9152youxi.cn

Java: // 手写回溯递归
来源：http://blt.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://icz.52xcode.cn

Ruby: arr.permutation.to_a
来源：http://wdd.zhixingplan.top

C#:   // 手写回溯递归
来源：http://gez.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://pck.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mmo.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cdd.jiagoushi.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wvw.wangshuangyany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fqf.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xbb.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://acm.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ncp.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jut.sweek.top

[N10] 链表节点定义
来源：http://fwo.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nae.hongshengwenyu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jid.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ufr.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cyh.zhongyouzk.top

Java: class Node { int v; Node next; }
来源：http://txm.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://jzm.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://pse.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://sjn.jianghu66.top

[N11] 二叉树中序遍历
来源：http://nru.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kur.meibo888.top

PHP:  // 手写递归函数
来源：http://qrm.sysykeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vwd.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://svj.yj20258888.top

Java: // 手写递归
来源：http://ujp.shzxlz.cn

Go:   // 手写递归
来源：http://gqs.daxiang520.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://agh.daria6918.cn

C#:   // 手写递归
来源：http://lyp.epnwcf.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zhy.yongpay.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://efy.fengsongda.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://whe.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dil.nwbrower.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pri.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://unr.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lqb.sweek.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ssg.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kof.fanxiaobao.xyz

================================================================================
来源：http://afh.yueranfly.top

O. 并发与异步
来源：http://evo.jianghu66.top

================================================================================
来源：http://gwv.tianlin.xyz

[O01] 启动一个线程
来源：http://exx.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bgx.jiagoushi.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qpi.cheryme.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kqd.dianchejie.cn

TS:   // 同 JS
来源：http://ekd.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://mtt.hnxiangtu.top

Go:   go f()
来源：http://wib.andypj.xyz

Ruby: Thread.new { f }
来源：http://cfo.dianchejie.cn

C#:   Task.Run(() => F());
来源：http://qwn.birdmap.top

[O02] 使用线程池
来源：http://hdx.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jzt.wangdashe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ibe.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://hrp.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://vav.jqgufenzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://vui.hnqzz.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://duz.gotoacloud.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://smf.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qcy.cashguo.top

[O03] 加锁保护共享数据
来源：http://fhi.sufxvd.cn

Py:   with lock: shared += 1
来源：http://vbh.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://xto.svipenyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://skp.feifeiyinyue.top

TS:   // 同 JS
来源：http://sxq.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://ald.sufxvd.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xbs.havefunace.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zsu.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://phv.cheryme.top

[O04] 定义异步函数并等待
来源：http://mmc.epnwcf.com

Py:   async def f():⏎    await g()
来源：http://oop.tanke756.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wrj.fzhhl.top

JS:   async function f() { await g(); }
来源：http://vig.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hhy.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qzn.zhoulong.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yvl.yongpay.top

Ruby: # 用 Fiber 或 async gem
来源：http://gwa.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://grb.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://rzr.shanyushiyangtech.top

Py:   asyncio.gather(*tasks)
来源：http://uoy.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dsk.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://glc.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://gup.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eqf.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sbp.yj202588.top

Ruby: threads.map(&:join)
来源：http://cdd.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sws.zhixingplan.top

[O06] 使用进程池
来源：http://wni.fehbvm.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dsb.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://imz.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://kyh.hesvh.cn

TS:   // child_process / cluster 模块
来源：http://epm.sjlbkw.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zll.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dah.cashguo.top

Ruby: // fork 块
来源：http://nuk.zycfv.cn

C#:   Parallel.For
来源：http://cvw.yuxming.cn

================================================================================
来源：http://btw.yueranfly.top

P. 常用工具函数
来源：http://ytr.aizwys.cn

================================================================================
来源：http://zzv.birdmap.top

[P01] 生成 UUID
来源：http://uhk.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://qdu.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gjr.snrcjt.cn

JS:   crypto.randomUUID()
来源：http://enj.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://nnd.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://tri.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://vuj.iojbl.cn

Ruby: SecureRandom.uuid
来源：http://bho.dianchejie.cn

C#:   Guid.NewGuid().ToString()
来源：http://gkx.jinqigfzy.top

[P02] MD5 / SHA256 摘要
来源：http://xps.tarul.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cst.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wvl.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rtz.guowangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lqt.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uso.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dti.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ctp.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wpy.yuxming.cn

[P03] 生成短随机字符串
来源：http://sfn.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://afg.316326.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zxe.fanxiaobao.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kpf.zhixingplan.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jjn.smart0.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vhv.zdbjq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dlt.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://efe.shangyingyoupin.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yqa.cheryme.top

[P04] 求长度
来源：http://lsf.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kqb.hongshengwenyu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vcc.ybcxt.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fya.aibaodan.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nnm.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://qpi.tianlin.xyz

Go:   len(arr);  len(m)
来源：http://pqr.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://ygf.xziqi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kmu.jyoumei.cn

[P05] 判断两个对象内容是否相等
来源：http://qcx.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ign.yongpay.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://evg.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rfg.aibaodan.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gju.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xsn.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://ena.tian-w.cn

Ruby: a == b
来源：http://ztt.zhengqikj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dzw.yuanzhike.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://heu.zhongyouzk.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wuh.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://dwp.ywan-chungtsiang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://soi.svipenyu.cn

TS:   if (x == null) {}
来源：http://ziw.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jaq.yonumen.top

Go:   if x == nil {}
来源：http://hau.cashguo.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eye.vehdjk.com

C#:   if (x is null) {}
来源：http://iet.xuetiantiany.cn

[P07] 防抖与节流
来源：http://yqa.yj20258.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://moy.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://xsr.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ryq.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ngs.xingfuxueyuan.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rjk.gzhubu.top


<!-- 参考信息 -->