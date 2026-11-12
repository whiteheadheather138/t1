代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jax.zhoulong.xyz

JS:   process.env.HOME
来源：http://dql.wangdashe.top

TS:   process.env.HOME
来源：http://vjs.sweek.top

Java: System.getenv("HOME")
来源：http://hdw.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rpv.c1oappe.top

Ruby: ENV["HOME"]
来源：http://zyp.cucudq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fon.tianlin.xyz

[M03] 执行外部命令
来源：http://slc.ydjk.org.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jwi.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://owm.cdnleiting.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wke.ctjpmb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://gku.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rzx.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://xaw.svipenyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gzx.jyoumei.cn

C#:   Process.Start("ls", "-l");
来源：http://eaf.sweek.top

[M04] 获取当前工作目录
来源：http://ood.quarkkingdee.top

Py:   os.getcwd()
来源：http://auf.feifeiyinyue.top

PHP:  getcwd();
来源：http://fdp.wangshuangyany.cn

JS:   process.cwd()
来源：http://vbz.hnqzz.top

TS:   process.cwd()
来源：http://zgm.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://dgu.yuanzhike.top

Go:   os.Getwd()
来源：http://wgs.jlsjyb.cn

Ruby: Dir.pwd
来源：http://ntr.yanxiufei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ayn.iojbl.cn

[M05] 设置退出码
来源：http://eqt.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://avr.uphjek.com

PHP:  exit(1);
来源：http://vdl.zhijiandao.cn

JS:   process.exit(1)
来源：http://yws.bbcook.cn

TS:   process.exit(1)
来源：http://syp.cashguo.top

Java: System.exit(1)
来源：http://jvn.0kj1m.cn

Go:   os.Exit(1)
来源：http://lgf.ybcxt.top

Ruby: exit 1
来源：http://vpn.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hpf.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://las.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://gpf.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sip.hongshengwenyu.top

JS:   console.error("err")
来源：http://qbi.tian-w.cn

TS:   console.error("err")
来源：http://haz.zhongyouzk.top

Java: System.err.println("err")
来源：http://fns.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ikx.jqgufenzy.top

Ruby: warn "err"
来源：http://vkb.sweek.top

C#:   Console.Error.WriteLine("err")
来源：http://rmp.gogol.net.cn

[M07] 判断是否为主入口
来源：http://upd.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://poo.chenjidiqi.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kdm.shuidangran.top

JS:   require.main === module
来源：http://emh.0kj1m.cn

TS:   require.main === module
来源：http://odt.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://zcz.cashguo.top

Go:   func main()
来源：http://rmo.jinqigufen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gup.tian-w.cn

C#:   static void Main(string[] args)
来源：http://hfw.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://zxz.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://awc.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://pod.gzhubu.top

JS:   process.platform;  process.version
来源：http://adr.316326.xyz

TS:   process.platform;  process.version
来源：http://qhy.zhongyouzk.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ypb.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hal.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://itv.ydzc1.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lhb.hywenlv.cn

================================================================================
来源：http://rxs.daxiang520.top

N. 数据结构与算法
来源：http://kom.gotoacloud.top

================================================================================
来源：http://vsl.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://jyz.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://ssa.hnxiangtu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rps.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wug.dianchejie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jkb.52xcode.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zuz.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://mgk.epnwcf.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://rcj.jinqigufen.top

C#:   Array.BinarySearch(arr, x)
来源：http://tpl.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://wul.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://ykz.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wyt.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lsu.svipenyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pxr.yfazqb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mmg.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://frf.gogol.net.cn

Ruby: arr.sort
来源：http://qtp.yj202588.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://sya.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://vvx.zhoulong.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vgh.hnxiangtu.top

PHP:  // 递归实现，或用 usort
来源：http://ynj.0kj1m.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hwu.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://smb.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oda.quarkkingdee.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ong.birdmap.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xjn.hnxiangtu.top

C#:   // 手写递归，或 Array.Sort
来源：http://tqq.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://kcv.sufxvd.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vvm.sjlbkw.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uva.yueranfly.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gue.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oil.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nsz.fzhhl.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tlg.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vad.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pyy.zhongyouzk.top

[N05] 最大公约数
来源：http://grs.sysykeji.top

Py:   math.gcd(a, b)
来源：http://gpz.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ozz.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fpe.tian-w.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lzg.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wog.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uay.fehbvm.com

Ruby: a.gcd(b)
来源：http://uic.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nws.jinqigfzy.top

[N06] 判断回文字符串
来源：http://odm.ydjk.org.cn

Py:   s == s[::-1]
来源：http://acu.jianghu66.top

PHP:  $s === strrev($s);
来源：http://gte.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://tkv.feifeiyinyue.top

TS:   s === [...s].reverse().join("")
来源：http://coy.smart0.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sjx.jinqigufen.top

Go:   // 双指针从两端比较
来源：http://zax.zhongyouzk.top

Ruby: s == s.reverse
来源：http://mts.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gxi.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://rax.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gzb.sweek.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tka.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wnf.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://pmc.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://ase.tarul.cn

Go:   // 手写 map[int]int
来源：http://tcz.cashguo.top

Ruby: // 手写 Hash
来源：http://kpj.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://knc.vqdsnc.cn

[N08] 生成全排列
来源：http://akt.ydzc1.top

Py:   itertools.permutations(arr)
来源：http://jov.chenjidiqi.icu

PHP:  // 手写递归交换
来源：http://jei.gotoacloud.top

JS:   // 手写回溯递归
来源：http://aey.bbcook.cn

TS:   // 手写回溯递归
来源：http://hps.zdqjudy.top

Java: // 手写回溯递归
来源：http://voy.316326.xyz

Go:   // 手写回溯递归
来源：http://zec.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://svu.jiagoushi.top

C#:   // 手写回溯递归
来源：http://fos.hammf.cn

[N09] 栈与队列
来源：http://ozp.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://brb.yueranfly.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ppn.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nef.52xcode.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cge.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zdn.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dza.jianghu66.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://afb.316326.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://npx.yanxiufei.cn

[N10] 链表节点定义
来源：http://eop.hysaishi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://num.jinqigfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vab.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yqf.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wtj.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://txk.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://mke.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://snc.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://emh.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://rrw.nwbrower.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ozr.feifeiyinyue.top

PHP:  // 手写递归函数
来源：http://pgn.hnxiangtu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yve.ydzc1.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jit.zdqjudy.top

Java: // 手写递归
来源：http://oso.fzhhl.top

Go:   // 手写递归
来源：http://tll.pycfn.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://btj.tianlin.xyz

C#:   // 手写递归
来源：http://zro.smart0.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jhb.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vio.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lga.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bqj.birdmap.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://moz.ivvv.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oxc.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ubd.xziqi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kno.zhixingplan.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bdx.jqgufenzy.top

================================================================================
来源：http://nfe.xylfe.cn

O. 并发与异步
来源：http://shp.pengpengdd.cyou

================================================================================
来源：http://aam.dianchejie.cn

[O01] 启动一个线程
来源：http://xhy.wangdashe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://thu.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jfq.zhongyouzk.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://epi.fanxiaobao.xyz

TS:   // 同 JS
来源：http://ilg.svipenyu.cn

Java: new Thread(() -> f()).start()
来源：http://pwu.dianchejie.cn

Go:   go f()
来源：http://yix.jlsjyb.cn

Ruby: Thread.new { f }
来源：http://iha.cashguo.top

C#:   Task.Run(() => F());
来源：http://xox.yuanzhike.top

[O02] 使用线程池
来源：http://dlr.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://waz.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bez.nwbrower.top

JS:   // worker_threads 线程池
来源：http://ygp.daxiang520.top

TS:   // worker_threads 线程池
来源：http://qyt.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://pje.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://txa.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://edo.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sqk.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://juu.jinyuanbaomall.cn

Py:   with lock: shared += 1
来源：http://jjs.zhijiandao.cn

PHP:  // 用 flock() 做文件锁
来源：http://acc.jqgfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://skf.yvedp.cn

TS:   // 同 JS
来源：http://yow.zhiwuduotai.top

Java: synchronized (this) { shared++; }
来源：http://sts.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mnn.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://qlq.nanxinkj.top

C#:   lock (gate) { shared++; }
来源：http://hvl.xylfe.cn

[O04] 定义异步函数并等待
来源：http://xuh.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://qee.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hix.yj20258888.top

JS:   async function f() { await g(); }
来源：http://eox.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vvc.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vda.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hhq.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sso.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://ple.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://sjj.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://mhu.fktsv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rne.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://ysm.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://blf.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yrj.fktsv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vyc.yuanzhike.top

Ruby: threads.map(&:join)
来源：http://gjt.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tuq.haohaochexian.top

[O06] 使用进程池
来源：http://hdz.zhongyouzk.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://plh.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ugb.xuanzx.com

JS:   // child_process / cluster 模块
来源：http://bwd.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://kjm.hywenlv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lih.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ylz.zhongyouzk.top

Ruby: // fork 块
来源：http://xid.fanxiaobao.xyz

C#:   Parallel.For
来源：http://oyz.chenzaomai.com

================================================================================
来源：http://ldf.fehbvm.com

P. 常用工具函数
来源：http://oka.c1oappe.top

================================================================================
来源：http://xlm.dashuyun.cn

[P01] 生成 UUID
来源：http://dif.fehbvm.com

Py:   str(uuid.uuid4())
来源：http://jor.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jrc.fengsongda.top

JS:   crypto.randomUUID()
来源：http://dqh.zhiwuduotai.top

TS:   crypto.randomUUID()
来源：http://aev.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://bhk.yvedp.cn

Go:   // 用 github.com/google/uuid
来源：http://ijd.zhoulong.xyz

Ruby: SecureRandom.uuid
来源：http://xgo.nwbrower.top

C#:   Guid.NewGuid().ToString()
来源：http://azy.hcnkem.com

[P02] MD5 / SHA256 摘要
来源：http://xvr.gaohongyu789.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ijz.epnwcf.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://thq.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qor.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://swm.chenzaomai.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zsz.shanyushiyangtech.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ija.cucudq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gwh.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://feb.tian-w.cn

[P03] 生成短随机字符串
来源：http://kke.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dqv.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://btw.zhongyouzk.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vzn.redwolf501.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mkf.cdnleiting.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cbj.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://olm.sufxvd.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://anc.sjlbkw.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xiw.cheryme.top

[P04] 求长度
来源：http://orx.zycfv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wsj.cdnleiting.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hhc.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qvs.316326.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://epx.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://xko.yfazqb.com

Go:   len(arr);  len(m)
来源：http://tkw.uphjek.com

Ruby: x.length;  x.size
来源：http://mmi.jinyuanbaomall.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://owp.andypj.xyz

[P05] 判断两个对象内容是否相等
来源：http://zsj.feifeiyinyue.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kgh.ppjwa.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gql.xuanzx.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vvl.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jtj.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ack.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://urn.jyoumei.cn

Ruby: a == b
来源：http://zpf.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oqw.shuidangran.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://anb.hongshengwenyu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gha.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://ble.cashguo.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xdy.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://qhg.ppjwa.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://iyr.snrcjt.cn

Go:   if x == nil {}
来源：http://cqc.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cli.ydzc1.top

C#:   if (x is null) {}
来源：http://fwh.daria6918.cn

[P07] 防抖与节流
来源：http://dzi.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://srf.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://sft.nwbrower.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://swx.9152youxi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jgq.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sex.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nsg.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://djy.xinyue.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mgc.redwolf501.top

[P08] 处理浮点精度问题
来源：http://sds.nanxinkj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jym.316326.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uyy.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wza.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ucq.sysykeji.top


<!-- 参考信息 -->