代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nqh.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://wdp.kuanghao11.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hri.gzhubu.top

[M03] 执行外部命令
来源：http://gvv.cucudq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rmv.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rgd.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hrv.zhixingplan.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tzf.zhaomingkeji.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hvc.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://idf.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://pkn.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://nvm.zycfv.cn

[M04] 获取当前工作目录
来源：http://oqh.zhixingplan.top

Py:   os.getcwd()
来源：http://bqj.zhoulong.xyz

PHP:  getcwd();
来源：http://trz.chenlongwang.top

JS:   process.cwd()
来源：http://elm.yfazqb.com

TS:   process.cwd()
来源：http://qbe.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://qpj.nwbrower.top

Go:   os.Getwd()
来源：http://gca.yj20258.top

Ruby: Dir.pwd
来源：http://qno.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://olz.jqgfzy.top

[M05] 设置退出码
来源：http://yvu.redwolf501.top

Py:   sys.exit(1)
来源：http://epm.chenzaomai.com

PHP:  exit(1);
来源：http://uhg.zhongyouzk.top

JS:   process.exit(1)
来源：http://rea.aizwys.cn

TS:   process.exit(1)
来源：http://jzj.dianchejie.cn

Java: System.exit(1)
来源：http://qbf.yj202588.top

Go:   os.Exit(1)
来源：http://vas.shangyingyoupin.top

Ruby: exit 1
来源：http://iyg.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wkh.gaohongyu789.top

[M06] 向标准错误输出
来源：http://ajv.gaohongyu789.top

Py:   print("err", file=sys.stderr)
来源：http://rsr.zdqjudy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zzl.yonumen.top

JS:   console.error("err")
来源：http://zwr.andypj.xyz

TS:   console.error("err")
来源：http://jhi.jqgufenzy.top

Java: System.err.println("err")
来源：http://xnb.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fwa.uphjek.com

Ruby: warn "err"
来源：http://bjx.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://rnd.jyoumei.cn

[M07] 判断是否为主入口
来源：http://gqm.fehbvm.com

Py:   if __name__ == "__main__":
来源：http://sfn.svipenyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lai.hesvh.cn

JS:   require.main === module
来源：http://ijd.quarkkingdee.top

TS:   require.main === module
来源：http://kbo.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://uix.nanxuanxn.top

Go:   func main()
来源：http://tee.iojbl.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bpz.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://egg.jinqigfzy.top

[M08] 获取系统与运行时信息
来源：http://ctu.nanxinkj.top

Py:   platform.system();  platform.python_version()
来源：http://xtr.ywan-chungtsiang.top

PHP:  PHP_OS;  phpversion();
来源：http://qzq.sweek.top

JS:   process.platform;  process.version
来源：http://qnq.tarul.cn

TS:   process.platform;  process.version
来源：http://fyb.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://whh.jinqigfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://msp.xziqi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://swd.chenzaomai.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://vhl.bjfxy.top

================================================================================
来源：http://cys.jinyuanbaomall.cn

N. 数据结构与算法
来源：http://iko.ydjk.org.cn

================================================================================
来源：http://fdw.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://kwd.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://igr.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vhb.mhx1999.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fux.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wta.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://kip.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://lqo.wangdashe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wbg.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://hdr.zdbjq.cn

[N02] 排序（工程实践用内置实现）
来源：http://vci.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://fug.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dkn.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ggl.sxryk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hzh.uphjek.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fvu.iojbl.cn

Go:   slices.Sort(arr)
来源：http://jie.gaohongyu789.top

Ruby: arr.sort
来源：http://jgd.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sun.zhengqikj.top

[N03] 快速排序（分治示例）
来源：http://pif.gaohongyu789.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wgn.birdmap.top

PHP:  // 递归实现，或用 usort
来源：http://hkb.yj20258.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bvm.yfazqb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ybh.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://akg.quarkkingdee.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cyl.hywenlv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ibu.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://vth.hammf.cn

[N04] 斐波那契数列
来源：http://ztx.zdqjudy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sns.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vku.hfpthk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://odl.sufxvd.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xdo.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://byp.xinyue.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fvm.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xoi.ppjwa.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://krw.zhixingplan.top

[N05] 最大公约数
来源：http://xtm.havefunace.top

Py:   math.gcd(a, b)
来源：http://gen.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fbk.316326.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nql.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hud.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uph.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tsa.ydzc1.top

Ruby: a.gcd(b)
来源：http://dqa.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fxi.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://vrl.wangdashe.top

Py:   s == s[::-1]
来源：http://sqi.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://cmm.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://bne.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://cze.yonumen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://syd.xuanzx.com

Go:   // 双指针从两端比较
来源：http://vnl.zdqjudy.top

Ruby: s == s.reverse
来源：http://phk.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yra.hcnkem.com

[N07] 两数之和（返回下标）
来源：http://gmx.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://npy.sjlbkw.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rnk.yueranfly.top

JS:   // 手写 Map：map.set(v, i)
来源：http://juw.shanyushiyangtech.top

TS:   // 手写 Map<string, number>
来源：http://gco.yj20258.top

Java: // 手写 HashMap
来源：http://isb.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://ksa.epnwcf.com

Ruby: // 手写 Hash
来源：http://hsh.yanxiufei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jnl.yanxiufei.cn

[N08] 生成全排列
来源：http://wkc.wangshuangyany.cn

Py:   itertools.permutations(arr)
来源：http://dts.meibo888.top

PHP:  // 手写递归交换
来源：http://hex.quarkkingdee.top

JS:   // 手写回溯递归
来源：http://fer.cucudq.cn

TS:   // 手写回溯递归
来源：http://szd.shangyingyoupin.top

Java: // 手写回溯递归
来源：http://yxr.52xcode.cn

Go:   // 手写回溯递归
来源：http://tod.yfazqb.com

Ruby: arr.permutation.to_a
来源：http://lal.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://zrc.yuanzhike.top

[N09] 栈与队列
来源：http://qti.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tua.epnwcf.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bdw.zhoulong.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tpr.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ihz.yfazqb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://umu.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ayr.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://djs.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cta.smart0.xyz

[N10] 链表节点定义
来源：http://ixs.ehwqpu.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://otd.gzhubu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wgc.smart0.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eku.c1oappe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tay.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://ayp.svipenyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://agb.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jjt.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://cqe.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://rwa.yj20258888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pdv.meibo888.top

PHP:  // 手写递归函数
来源：http://ger.uphjek.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sco.kuanghao11.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wku.kuanghao11.cn

Java: // 手写递归
来源：http://ape.guannengcc.top

Go:   // 手写递归
来源：http://zop.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://owe.ivvv.top

C#:   // 手写递归
来源：http://ztw.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pjp.zhaomingkeji.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qoi.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uwf.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bpg.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jzo.quarkkingdee.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tay.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nmn.ywan-chungtsiang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sec.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dxs.chenzaomai.com

================================================================================
来源：http://cdm.tarul.cn

O. 并发与异步
来源：http://hak.zhijiandao.cn

================================================================================
来源：http://ord.cucudq.cn

[O01] 启动一个线程
来源：http://ysv.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://asd.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://akt.cheryme.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oer.haohaochexian.top

TS:   // 同 JS
来源：http://ktr.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://nvs.yuanzhike.top

Go:   go f()
来源：http://mej.shanyushiyangkeji.top

Ruby: Thread.new { f }
来源：http://auf.smart0.xyz

C#:   Task.Run(() => F());
来源：http://jay.guowangkeji.top

[O02] 使用线程池
来源：http://mbj.ybcxt.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://imj.hnxiangtu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qqp.havefunace.top

JS:   // worker_threads 线程池
来源：http://svz.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://jsg.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://tar.aizwys.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ksr.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gvz.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vuk.cqqwz.cn

[O03] 加锁保护共享数据
来源：http://zss.cashguo.top

Py:   with lock: shared += 1
来源：http://laz.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://kbv.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vzw.hnqzz.top

TS:   // 同 JS
来源：http://czc.zhixingplan.top

Java: synchronized (this) { shared++; }
来源：http://mrs.feifeiyinyue.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zup.shanyushiyangtech.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zdc.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://fwx.wangdashe.top

[O04] 定义异步函数并等待
来源：http://eyv.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://zat.shanyushiyangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eai.yj202588.top

JS:   async function f() { await g(); }
来源：http://wbk.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://eni.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tzo.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oqy.smart0.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://gru.jinyuanbaomall.cn

C#:   async Task F() { await G(); }
来源：http://juk.haohaochexian.top

[O05] 并发执行并等待全部完成
来源：http://skc.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://kaq.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qnl.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://ijx.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://zry.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ayo.hnxiangtu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aso.meibo888.top

Ruby: threads.map(&:join)
来源：http://syo.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://jxk.andypj.xyz

[O06] 使用进程池
来源：http://ksp.ctjpmb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mvg.zhaomingkeji.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://acw.fzhhl.top

JS:   // child_process / cluster 模块
来源：http://ngt.svipenyu.cn

TS:   // child_process / cluster 模块
来源：http://nmq.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jfj.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rfs.316326.xyz

Ruby: // fork 块
来源：http://vkd.fanxiaobao.xyz

C#:   Parallel.For
来源：http://zrz.jinqigufen.top

================================================================================
来源：http://vqo.bbcook.cn

P. 常用工具函数
来源：http://wjt.epnwcf.com

================================================================================
来源：http://ejh.sweek.top

[P01] 生成 UUID
来源：http://ggc.fengsongda.top

Py:   str(uuid.uuid4())
来源：http://smn.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sav.iojbl.cn

JS:   crypto.randomUUID()
来源：http://tiq.fzhhl.top

TS:   crypto.randomUUID()
来源：http://lib.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://xwa.fehbvm.com

Go:   // 用 github.com/google/uuid
来源：http://xah.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://pyy.yanxiufei.cn

C#:   Guid.NewGuid().ToString()
来源：http://emz.zdbjq.cn

[P02] MD5 / SHA256 摘要
来源：http://tbo.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vec.fehbvm.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://vvu.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yyj.xinyue.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zbi.dianchejie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lgo.hywenlv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zcx.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rsh.jqgfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qye.nwbrower.top

[P03] 生成短随机字符串
来源：http://hzc.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://prb.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gdp.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bvb.yfazqb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eyz.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qxg.chenlongwang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qem.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dxl.hammf.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gfg.yongpay.top

[P04] 求长度
来源：http://igc.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aiu.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xji.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://axo.yvedp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dvt.hesvh.cn

Java: list.size();  map.size();  s.length()
来源：http://cpz.chenzaomai.com

Go:   len(arr);  len(m)
来源：http://vqv.sweek.top

Ruby: x.length;  x.size
来源：http://uet.zhengqikj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xua.hesvh.cn

[P05] 判断两个对象内容是否相等
来源：http://tlp.sweek.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uqu.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://geh.daria6918.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jvq.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jkn.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wkx.zhengqikj.top

Go:   reflect.DeepEqual(a, b)
来源：http://ols.quarkkingdee.top

Ruby: a == b
来源：http://fes.hnqzz.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vwv.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rjx.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wiu.mhx1999.top

PHP:  if (empty($x)) {}
来源：http://oid.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sja.feifeiyinyue.top

TS:   if (x == null) {}
来源：http://xfc.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fqn.hcnkem.com

Go:   if x == nil {}
来源：http://gye.jinghuilouyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lzg.sjlbkw.cn

C#:   if (x is null) {}
来源：http://dpb.xuanzx.com

[P07] 防抖与节流
来源：http://dkx.gotoacloud.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ofg.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://fzw.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cui.hcnkem.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aby.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mux.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vsw.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://psn.sxryk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pgo.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://ruw.hammf.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pbp.jqgufenzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kmz.sufxvd.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ddu.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jlj.yuanzhike.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pgy.jiagoushi.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qff.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zhr.yuanzhike.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ijg.zdqjudy.top


<!-- 参考信息 -->