代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ode.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://yjg.wangdashe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lns.guannengcc.top

[M03] 执行外部命令
来源：http://xtq.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yyj.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kns.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ibd.316326.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://joi.uphjek.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://onn.fanxiaobao.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://dzb.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://qvl.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://hjw.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://jbv.pycfn.com

Py:   os.getcwd()
来源：http://sjn.sweek.top

PHP:  getcwd();
来源：http://mce.yueranfly.top

JS:   process.cwd()
来源：http://rdm.ydjk.org.cn

TS:   process.cwd()
来源：http://xyj.xinyue.icu

Java: Path.of("").toAbsolutePath()
来源：http://mvi.daxiang520.top

Go:   os.Getwd()
来源：http://ntm.hammf.cn

Ruby: Dir.pwd
来源：http://buz.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://nos.c1oappe.top

[M05] 设置退出码
来源：http://oji.fzhhl.top

Py:   sys.exit(1)
来源：http://axx.sweek.top

PHP:  exit(1);
来源：http://mft.jqgfzy.top

JS:   process.exit(1)
来源：http://pfj.cheryme.top

TS:   process.exit(1)
来源：http://qim.hammf.cn

Java: System.exit(1)
来源：http://rka.yonumen.top

Go:   os.Exit(1)
来源：http://kua.yuxming.cn

Ruby: exit 1
来源：http://aws.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://grw.cqqwz.cn

[M06] 向标准错误输出
来源：http://ums.aizwys.cn

Py:   print("err", file=sys.stderr)
来源：http://ndb.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bla.sysykeji.top

JS:   console.error("err")
来源：http://crr.52xcode.cn

TS:   console.error("err")
来源：http://wua.aizwys.cn

Java: System.err.println("err")
来源：http://cyc.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://spw.epnwcf.com

Ruby: warn "err"
来源：http://cmk.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://glz.mhx1999.top

[M07] 判断是否为主入口
来源：http://oxr.yj202588.top

Py:   if __name__ == "__main__":
来源：http://opp.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dvo.tianlin.xyz

JS:   require.main === module
来源：http://vfj.jqgufenzy.top

TS:   require.main === module
来源：http://onp.0kj1m.cn

Java: public static void main(String[] args)
来源：http://bgc.xuanzx.com

Go:   func main()
来源：http://nqq.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tuw.redwolf501.top

C#:   static void Main(string[] args)
来源：http://eah.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://ghi.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://thu.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://mgq.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://aao.yanxiufei.cn

TS:   process.platform;  process.version
来源：http://wky.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ita.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qjz.xuanzx.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wrj.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pnu.guannengcc.top

================================================================================
来源：http://bpd.nwbrower.top

N. 数据结构与算法
来源：http://tof.sjlbkw.cn

================================================================================
来源：http://mmz.zhoulong.xyz

[N01] 二分查找（有序数组）
来源：http://lzp.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://hbv.sjlbkw.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://myv.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zan.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zid.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://znb.zhongyouzk.top

Go:   sort.SearchInts(arr, x)
来源：http://asj.andypj.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://rnr.jyoumei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aaf.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://tev.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://xln.cashguo.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iei.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hig.hywenlv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ans.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pth.cheryme.top

Go:   slices.Sort(arr)
来源：http://nya.yfazqb.com

Ruby: arr.sort
来源：http://wiy.meibo888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fle.tanke756.top

[N03] 快速排序（分治示例）
来源：http://htq.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baf.yj20258.top

PHP:  // 递归实现，或用 usort
来源：http://frb.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rnt.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uba.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dak.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://puh.zhengqikj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zxv.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hdw.wangshuangyany.cn

[N04] 斐波那契数列
来源：http://chl.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ypv.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eem.sufxvd.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ozs.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://abv.ydjk.org.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://amy.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://glo.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jgt.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dfl.chenjidiqi.icu

[N05] 最大公约数
来源：http://muw.aibaodan.cn

Py:   math.gcd(a, b)
来源：http://nad.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ape.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ody.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://drc.ivvv.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jmg.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dzw.fengsongda.top

Ruby: a.gcd(b)
来源：http://ons.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gep.yuxming.cn

[N06] 判断回文字符串
来源：http://vcx.jinyuanbaomall.cn

Py:   s == s[::-1]
来源：http://vma.tarul.cn

PHP:  $s === strrev($s);
来源：http://vgc.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://qpi.chenlongwang.top

TS:   s === [...s].reverse().join("")
来源：http://kmk.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ind.daria6918.cn

Go:   // 双指针从两端比较
来源：http://vly.jqgufenzy.top

Ruby: s == s.reverse
来源：http://ewb.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bav.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://wpr.shangyingyoupin.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mrn.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uma.yj20258.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wri.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://fpt.svipenyu.cn

Java: // 手写 HashMap
来源：http://zri.xuanzx.com

Go:   // 手写 map[int]int
来源：http://scm.guowangkeji.top

Ruby: // 手写 Hash
来源：http://lvc.hcnkem.com

C#:   // 手写 Dictionary<int, int>
来源：http://zmt.tarul.cn

[N08] 生成全排列
来源：http://nmc.xziqi.cn

Py:   itertools.permutations(arr)
来源：http://sdy.sxryk.cn

PHP:  // 手写递归交换
来源：http://xke.tanke756.top

JS:   // 手写回溯递归
来源：http://cva.yongpay.top

TS:   // 手写回溯递归
来源：http://ayd.zycfv.cn

Java: // 手写回溯递归
来源：http://dmx.yfazqb.com

Go:   // 手写回溯递归
来源：http://pwe.meibo888.top

Ruby: arr.permutation.to_a
来源：http://rqo.hesvh.cn

C#:   // 手写回溯递归
来源：http://nob.ybcxt.top

[N09] 栈与队列
来源：http://dvz.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dna.tian-w.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gqe.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lse.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dej.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ksy.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zlo.shanyushiyangtech.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kqn.sweek.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qaf.pycfn.com

[N10] 链表节点定义
来源：http://ify.xuanzx.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cfk.shanyushiyangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://due.zdbjq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jcm.52xcode.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xsw.quarkkingdee.top

Java: class Node { int v; Node next; }
来源：http://phm.wangshuangyany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bki.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vuq.sufxvd.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ixf.chenjidiqi.icu

[N11] 二叉树中序遍历
来源：http://fdx.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kas.zhengqikj.top

PHP:  // 手写递归函数
来源：http://hzf.iojbl.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jbl.iojbl.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://adu.pycfn.com

Java: // 手写递归
来源：http://eri.fanxiaobao.xyz

Go:   // 手写递归
来源：http://vqn.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eaw.gaohongyu789.top

C#:   // 手写递归
来源：http://mbu.svipenyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://avs.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ena.hesvh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://syv.havefunace.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://igj.xuetiantiany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xkw.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bwr.fzhhl.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bcq.yuanzhike.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qxe.aibaodan.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uwo.hysaishi.cn

================================================================================
来源：http://smh.yanxiufei.cn

O. 并发与异步
来源：http://neo.fengsongda.top

================================================================================
来源：http://qbg.ppjwa.cn

[O01] 启动一个线程
来源：http://fgt.yongpay.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lgc.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ycc.hysaishi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qzi.c1oappe.top

TS:   // 同 JS
来源：http://vea.zhijiandao.cn

Java: new Thread(() -> f()).start()
来源：http://ynz.zhongyouzk.top

Go:   go f()
来源：http://pqb.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://ozy.wangdashe.top

C#:   Task.Run(() => F());
来源：http://qoj.mhx1999.top

[O02] 使用线程池
来源：http://pcb.ehwqpu.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dme.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bzu.hammf.cn

JS:   // worker_threads 线程池
来源：http://kdw.birdmap.top

TS:   // worker_threads 线程池
来源：http://xfq.aibaodan.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yvu.ywan-chungtsiang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://elo.yj202588.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fcy.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hxm.sufxvd.cn

[O03] 加锁保护共享数据
来源：http://vph.tianlin.xyz

Py:   with lock: shared += 1
来源：http://reh.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://cht.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nwy.xziqi.cn

TS:   // 同 JS
来源：http://vrf.nanxinkj.top

Java: synchronized (this) { shared++; }
来源：http://vhl.fanxiaobao.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://axa.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iti.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://usy.hongshengwenyu.top

[O04] 定义异步函数并等待
来源：http://wbe.sjlbkw.cn

Py:   async def f():⏎    await g()
来源：http://alb.shangyingyoupin.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kge.ybcxt.top

JS:   async function f() { await g(); }
来源：http://wql.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uyo.yj20258888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mxm.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://amv.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://gnk.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://qvs.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://uyv.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://uqg.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pcy.tanke756.top

JS:   await Promise.all(tasks)
来源：http://rfs.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://wyj.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bhp.daria6918.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mhj.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://xve.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yem.ydjk.org.cn

[O06] 使用进程池
来源：http://wpv.yj20258888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gmb.haohaochexian.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xdw.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://gsm.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://nlk.jinqigufen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iva.daxiang520.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rku.havefunace.top

Ruby: // fork 块
来源：http://waf.sysykeji.top

C#:   Parallel.For
来源：http://wtj.shangyingyoupin.top

================================================================================
来源：http://kpq.yanxiufei.cn

P. 常用工具函数
来源：http://ftm.gzhubu.top

================================================================================
来源：http://kzp.yuxming.cn

[P01] 生成 UUID
来源：http://spu.yj20258.top

Py:   str(uuid.uuid4())
来源：http://nwn.dashuyun.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wny.tian-w.cn

JS:   crypto.randomUUID()
来源：http://frx.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://rwx.zhoulong.xyz

Java: UUID.randomUUID().toString()
来源：http://toi.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://wjn.jlsjyb.cn

Ruby: SecureRandom.uuid
来源：http://omr.sufxvd.cn

C#:   Guid.NewGuid().ToString()
来源：http://oki.hcnkem.com

[P02] MD5 / SHA256 摘要
来源：http://cwc.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dem.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hwh.jinqigufen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rox.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tvi.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sck.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iyj.hnqzz.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hxo.zhengqikj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qeh.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://edl.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cyn.gaohongyu789.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nua.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://quu.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vfz.chenzaomai.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xlt.gaohongyu789.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tfr.chenlongwang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cjs.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eta.cqqwz.cn

[P04] 求长度
来源：http://ryn.zhengqikj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wef.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://geo.zhijiandao.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hst.zhaomingkeji.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mrt.hammf.cn

Java: list.size();  map.size();  s.length()
来源：http://gxk.jyoumei.cn

Go:   len(arr);  len(m)
来源：http://snq.feifeiyinyue.top

Ruby: x.length;  x.size
来源：http://aqp.zhengqikj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kuq.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://aeg.cucudq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kxx.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ybb.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ebm.epnwcf.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://chk.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sjo.daxiang520.top

Go:   reflect.DeepEqual(a, b)
来源：http://pgj.yuanzhike.top

Ruby: a == b
来源：http://aqo.ppjwa.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uaw.fanxiaobao.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hhk.zhixingplan.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zmh.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://pxm.zhijiandao.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mfp.cdnleiting.top

TS:   if (x == null) {}
来源：http://tal.bbcook.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xad.aibaodan.cn

Go:   if x == nil {}
来源：http://bgb.hywenlv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ajt.gotoacloud.top

C#:   if (x is null) {}
来源：http://zlz.feifeiyinyue.top

[P07] 防抖与节流
来源：http://zdv.zhijiandao.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pvs.smart0.xyz

PHP:  // 手写时间戳比较
来源：http://eve.havefunace.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qxb.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xno.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://naz.316326.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qlo.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://snz.havefunace.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wmt.yueranfly.top

[P08] 处理浮点精度问题
来源：http://fig.yuxming.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zrw.daria6918.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ukt.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mwg.yuanzhike.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xmf.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nfb.kuanghao11.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://knd.ydzc1.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gqx.yuanzhike.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xxt.redwolf501.top


<!-- 参考信息 -->