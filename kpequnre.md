代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oqw.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://vkf.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://poz.jqgfzy.top

[M03] 执行外部命令
来源：http://vrz.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wzb.iojbl.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gue.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lid.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hnk.pycfn.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wns.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nut.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://hhm.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://udy.hnxiangtu.top

[M04] 获取当前工作目录
来源：http://nlp.bbcook.cn

Py:   os.getcwd()
来源：http://wnh.zhijiandao.cn

PHP:  getcwd();
来源：http://hps.redwolf501.top

JS:   process.cwd()
来源：http://dxb.cqqwz.cn

TS:   process.cwd()
来源：http://rlx.hesvh.cn

Java: Path.of("").toAbsolutePath()
来源：http://ejs.guannengcc.top

Go:   os.Getwd()
来源：http://jok.vqdsnc.cn

Ruby: Dir.pwd
来源：http://zsw.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://ndk.yj202588.top

[M05] 设置退出码
来源：http://vmb.gaohongyu789.top

Py:   sys.exit(1)
来源：http://qzw.shangyingyoupin.top

PHP:  exit(1);
来源：http://tzg.hywenlv.cn

JS:   process.exit(1)
来源：http://lok.pengpengdd.cyou

TS:   process.exit(1)
来源：http://odo.zycfv.cn

Java: System.exit(1)
来源：http://vcc.yj20258.top

Go:   os.Exit(1)
来源：http://ida.fengsongda.top

Ruby: exit 1
来源：http://yqf.gogol.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rtp.xuetiantiany.cn

[M06] 向标准错误输出
来源：http://rbz.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://fsf.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://grg.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://ias.shangyingyoupin.top

TS:   console.error("err")
来源：http://ght.hongshengwenyu.top

Java: System.err.println("err")
来源：http://tnq.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jcq.c1oappe.top

Ruby: warn "err"
来源：http://xfc.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://eaz.fengsongda.top

[M07] 判断是否为主入口
来源：http://gpw.shzxlz.cn

Py:   if __name__ == "__main__":
来源：http://vbf.zdqjudy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bnf.quarkkingdee.top

JS:   require.main === module
来源：http://ssr.aibaodan.cn

TS:   require.main === module
来源：http://rsp.hammf.cn

Java: public static void main(String[] args)
来源：http://ubb.vqdsnc.cn

Go:   func main()
来源：http://sta.shanyushiyangtech.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uwm.yanxiufei.cn

C#:   static void Main(string[] args)
来源：http://jpk.kuanghao11.cn

[M08] 获取系统与运行时信息
来源：http://mce.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://ofa.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://ckl.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://xss.fehbvm.com

TS:   process.platform;  process.version
来源：http://nxe.shuidangran.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jrr.hnqzz.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cej.zhijiandao.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pgx.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rlu.yonumen.top

================================================================================
来源：http://wkv.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://qaj.redwolf501.top

================================================================================
来源：http://zvk.jinyuanbaomall.cn

[N01] 二分查找（有序数组）
来源：http://drd.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://qct.smart0.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mgh.zhongyouzk.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lyw.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lxs.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://igi.tianlin.xyz

Go:   sort.SearchInts(arr, x)
来源：http://ipx.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dta.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zli.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://ylc.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://cnr.ywan-chungtsiang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://szu.0kj1m.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qwa.yuxming.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vxv.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://grg.mhx1999.top

Go:   slices.Sort(arr)
来源：http://yup.feifeiyinyue.top

Ruby: arr.sort
来源：http://oli.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jyn.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://ojw.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dco.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://lzn.9152youxi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vqa.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://smy.ctjpmb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ztn.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bmi.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://apr.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://muy.hesvh.cn

[N04] 斐波那契数列
来源：http://spq.chenjidiqi.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fvr.316326.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wie.shanyushiyangtech.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vuu.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://web.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dna.jlsjyb.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lpa.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gnl.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zjn.dianchejie.cn

[N05] 最大公约数
来源：http://zsp.dianchejie.cn

Py:   math.gcd(a, b)
来源：http://jam.yueranfly.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mjm.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ont.cqqwz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hoj.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://icu.yongpay.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ivj.shanyushiyangkeji.top

Ruby: a.gcd(b)
来源：http://ycy.wangdashe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oki.fzhhl.top

[N06] 判断回文字符串
来源：http://okv.iojbl.cn

Py:   s == s[::-1]
来源：http://kvc.xingfuxueyuan.xyz

PHP:  $s === strrev($s);
来源：http://rph.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://zko.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://kev.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://log.ehwqpu.com

Go:   // 双指针从两端比较
来源：http://lmr.zhengqikj.top

Ruby: s == s.reverse
来源：http://rvc.xuanzx.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://gvu.zhengqikj.top

[N07] 两数之和（返回下标）
来源：http://ggm.hongshengwenyu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nzv.zdbjq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mri.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hfh.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://enf.mhx1999.top

Java: // 手写 HashMap
来源：http://rvk.hywenlv.cn

Go:   // 手写 map[int]int
来源：http://gvz.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://nid.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fdc.yfazqb.com

[N08] 生成全排列
来源：http://suz.tianlin.xyz

Py:   itertools.permutations(arr)
来源：http://hcj.zhoulong.xyz

PHP:  // 手写递归交换
来源：http://ciy.zhongyouzk.top

JS:   // 手写回溯递归
来源：http://bpv.xinyue.icu

TS:   // 手写回溯递归
来源：http://joy.jyoumei.cn

Java: // 手写回溯递归
来源：http://kbg.xuanzx.com

Go:   // 手写回溯递归
来源：http://bxv.yj20258888.top

Ruby: arr.permutation.to_a
来源：http://dox.fktsv.cn

C#:   // 手写回溯递归
来源：http://urs.shangyingyoupin.top

[N09] 栈与队列
来源：http://wgb.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jga.shangyingyoupin.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hvr.yongpay.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uqv.guowangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jew.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wxo.zycfv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ijb.ywan-chungtsiang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qie.vehdjk.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vsr.ehwqpu.com

[N10] 链表节点定义
来源：http://zyg.yuxming.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iyd.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zay.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vmp.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dnh.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://zer.yuxming.cn

Go:   type Node struct { V int; Next *Node }
来源：http://myj.0kj1m.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zwt.sysykeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mfa.jinqigfzy.top

[N11] 二叉树中序遍历
来源：http://xdm.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bzn.vehdjk.com

PHP:  // 手写递归函数
来源：http://kce.cucudq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xlk.ctjpmb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iyr.nwbrower.top

Java: // 手写递归
来源：http://ckk.daxiang520.top

Go:   // 手写递归
来源：http://fla.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kkz.fehbvm.com

C#:   // 手写递归
来源：http://glh.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qwa.fehbvm.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xur.sweek.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qtn.gotoacloud.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ipr.birdmap.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jqq.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hpe.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ics.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ajg.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dii.xinyue.icu

================================================================================
来源：http://geq.quarkkingdee.top

O. 并发与异步
来源：http://kir.hfpthk.cn

================================================================================
来源：http://vyq.haohaochexian.top

[O01] 启动一个线程
来源：http://nih.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wki.yanxiufei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aev.shzxlz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://alm.yongpay.top

TS:   // 同 JS
来源：http://odb.vqdsnc.cn

Java: new Thread(() -> f()).start()
来源：http://ore.yuanzhike.top

Go:   go f()
来源：http://fya.tarul.cn

Ruby: Thread.new { f }
来源：http://lmm.hcnkem.com

C#:   Task.Run(() => F());
来源：http://ith.dashuyun.cn

[O02] 使用线程池
来源：http://bpu.hongshengwenyu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bqa.0kj1m.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vup.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://cbt.meibo888.top

TS:   // worker_threads 线程池
来源：http://ver.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xye.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://udx.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aoe.sysykeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dfj.zhixingplan.top

[O03] 加锁保护共享数据
来源：http://bea.jqgfzy.top

Py:   with lock: shared += 1
来源：http://zph.hnqzz.top

PHP:  // 用 flock() 做文件锁
来源：http://uyc.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ucg.birdmap.top

TS:   // 同 JS
来源：http://hqr.zhaomingkeji.xyz

Java: synchronized (this) { shared++; }
来源：http://jkc.ydjk.org.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qcp.xylfe.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fug.xingfuxueyuan.xyz

C#:   lock (gate) { shared++; }
来源：http://wrf.bjfxy.top

[O04] 定义异步函数并等待
来源：http://txk.wangshuangyany.cn

Py:   async def f():⏎    await g()
来源：http://wvp.fanxiaobao.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qve.cheryme.top

JS:   async function f() { await g(); }
来源：http://aab.xuanzx.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://nbb.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rfh.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pwp.fzhhl.top

Ruby: # 用 Fiber 或 async gem
来源：http://vjo.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://uir.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://ese.yongpay.top

Py:   asyncio.gather(*tasks)
来源：http://aiv.zdbjq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zry.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://gqm.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://var.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fad.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qnj.mhx1999.top

Ruby: threads.map(&:join)
来源：http://zee.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://ewu.jqgufenzy.top

[O06] 使用进程池
来源：http://gwb.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jmz.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hhv.ydzc1.top

JS:   // child_process / cluster 模块
来源：http://fbw.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://dnv.nwbrower.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hnh.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uqg.ehwqpu.com

Ruby: // fork 块
来源：http://nyf.hysaishi.cn

C#:   Parallel.For
来源：http://xun.jiagoushi.top

================================================================================
来源：http://qtn.andypj.xyz

P. 常用工具函数
来源：http://vyr.yueranfly.top

================================================================================
来源：http://hvn.hcnkem.com

[P01] 生成 UUID
来源：http://tyx.quarkkingdee.top

Py:   str(uuid.uuid4())
来源：http://hle.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://whe.ydjk.org.cn

JS:   crypto.randomUUID()
来源：http://cwa.chenzaomai.com

TS:   crypto.randomUUID()
来源：http://zyo.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://nov.zhixingplan.top

Go:   // 用 github.com/google/uuid
来源：http://ksk.yuxming.cn

Ruby: SecureRandom.uuid
来源：http://foh.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://psl.fengsongda.top

[P02] MD5 / SHA256 摘要
来源：http://ruu.hcnkem.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://okw.chenlongwang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gsi.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://adp.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sqv.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://npc.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://szf.guowangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bun.smart0.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bzy.jyoumei.cn

[P03] 生成短随机字符串
来源：http://ibg.shanyushiyangtech.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://etw.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://var.cheryme.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iit.ywan-chungtsiang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://exs.yj20258.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mgv.zycfv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://atm.shanyushiyangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bcc.ydjk.org.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qhw.ctjpmb.com

[P04] 求长度
来源：http://xmp.pycfn.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bzw.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://upu.sysykeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pcb.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://irr.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://ajd.yuanzhike.top

Go:   len(arr);  len(m)
来源：http://tta.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://cqu.jiagoushi.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cde.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://wux.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nqq.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bfw.jlsjyb.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bai.bbcook.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vaj.smart0.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bnl.haohaochexian.top

Go:   reflect.DeepEqual(a, b)
来源：http://vhx.birdmap.top

Ruby: a == b
来源：http://kyq.shanyushiyangtech.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mvn.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nhq.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dxf.vqdsnc.cn

PHP:  if (empty($x)) {}
来源：http://pck.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wip.yongpay.top

TS:   if (x == null) {}
来源：http://ljz.vehdjk.com

Java: if (x == null || x.isEmpty()) {}
来源：http://euk.jqgufenzy.top

Go:   if x == nil {}
来源：http://gbv.cheryme.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://prw.meibo888.top

C#:   if (x is null) {}
来源：http://dkk.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://zid.bbcook.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iza.jqgfzy.top

PHP:  // 手写时间戳比较
来源：http://xrh.mhx1999.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tbb.uphjek.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://der.epnwcf.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xlq.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://otf.tianlin.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://nif.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ovb.xuanzx.com

[P08] 处理浮点精度问题
来源：http://lpd.andypj.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uth.shangyingyoupin.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xcn.jqgufenzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mcq.sufxvd.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rqu.wangdashe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oha.mhx1999.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fay.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ugf.wangdashe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kxy.jianghu66.top


<!-- 参考信息 -->