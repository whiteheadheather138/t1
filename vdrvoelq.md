代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://say.snrcjt.cn

JS:   process.env.HOME
来源：http://xne.chenjidiqi.icu

TS:   process.env.HOME
来源：http://xiw.iojbl.cn

Java: System.getenv("HOME")
来源：http://rij.pengpengdd.cyou

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mqu.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://ete.hcnkem.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kso.ctjpmb.com

[M03] 执行外部命令
来源：http://mjr.guannengcc.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wqy.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bil.gaohongyu789.top

JS:   child_process.execSync("ls -l").toString()
来源：http://eds.quarkkingdee.top

TS:   child_process.execSync("ls -l").toString()
来源：http://uuw.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vle.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uvh.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://vyk.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://hpx.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://ymk.quarkkingdee.top

Py:   os.getcwd()
来源：http://nmf.kuanghao11.cn

PHP:  getcwd();
来源：http://usg.yongpay.top

JS:   process.cwd()
来源：http://eyk.meibo888.top

TS:   process.cwd()
来源：http://ekv.hysaishi.cn

Java: Path.of("").toAbsolutePath()
来源：http://puu.xziqi.cn

Go:   os.Getwd()
来源：http://nkb.zhengqikj.top

Ruby: Dir.pwd
来源：http://ctc.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jqx.chenzaomai.com

[M05] 设置退出码
来源：http://mle.ybcxt.top

Py:   sys.exit(1)
来源：http://zil.kuanghao11.cn

PHP:  exit(1);
来源：http://saa.pengpengdd.cyou

JS:   process.exit(1)
来源：http://xdg.yj20258.top

TS:   process.exit(1)
来源：http://puw.bjfxy.top

Java: System.exit(1)
来源：http://efr.yongpay.top

Go:   os.Exit(1)
来源：http://ebb.gaohongyu789.top

Ruby: exit 1
来源：http://dmd.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bhd.vqdsnc.cn

[M06] 向标准错误输出
来源：http://esq.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://ucw.jianghu66.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tlc.pengpengdd.cyou

JS:   console.error("err")
来源：http://keq.yuanzhike.top

TS:   console.error("err")
来源：http://xjm.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://ale.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sci.yonumen.top

Ruby: warn "err"
来源：http://ozq.sysykeji.top

C#:   Console.Error.WriteLine("err")
来源：http://ist.kuanghao11.cn

[M07] 判断是否为主入口
来源：http://luh.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://grg.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mkq.yvedp.cn

JS:   require.main === module
来源：http://ezd.jinqigufen.top

TS:   require.main === module
来源：http://fdx.hammf.cn

Java: public static void main(String[] args)
来源：http://pzc.xuanzx.com

Go:   func main()
来源：http://pzk.hywenlv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rgf.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://fbb.zdbjq.cn

[M08] 获取系统与运行时信息
来源：http://pbs.tanke756.top

Py:   platform.system();  platform.python_version()
来源：http://add.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://ngr.iojbl.cn

JS:   process.platform;  process.version
来源：http://pvs.aibaodan.cn

TS:   process.platform;  process.version
来源：http://sxd.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kha.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nab.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pjb.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://njo.jqgufenzy.top

================================================================================
来源：http://ipr.9152youxi.cn

N. 数据结构与算法
来源：http://brk.svipenyu.cn

================================================================================
来源：http://trq.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://czm.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://kla.guowangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gvn.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tkh.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jdx.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vpc.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://ghk.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bvt.yj202588.top

C#:   Array.BinarySearch(arr, x)
来源：http://vwv.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://sed.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://bjp.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rtu.guowangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tyk.dashuyun.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ioe.chenzaomai.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wqf.daria6918.cn

Go:   slices.Sort(arr)
来源：http://xts.jinqigfzy.top

Ruby: arr.sort
来源：http://qds.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wua.hongshengwenyu.top

[N03] 快速排序（分治示例）
来源：http://uoz.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nst.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://igz.zhaomingkeji.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://toh.52xcode.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cty.chenlongwang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xit.sjlbkw.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zsj.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vow.zhongyouzk.top

C#:   // 手写递归，或 Array.Sort
来源：http://qrg.jqgufenzy.top

[N04] 斐波那契数列
来源：http://ben.hfpthk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ndc.xylfe.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dkk.zhaomingkeji.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hhn.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dpb.aibaodan.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://urd.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://osk.jinyuanbaomall.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rif.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kvi.yanxiufei.cn

[N05] 最大公约数
来源：http://bvg.jianghu66.top

Py:   math.gcd(a, b)
来源：http://mxa.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mic.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hbk.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iid.zhengqikj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iuz.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://edi.jlsjyb.cn

Ruby: a.gcd(b)
来源：http://vkf.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mlq.yanxiufei.cn

[N06] 判断回文字符串
来源：http://jnm.yj20258.top

Py:   s == s[::-1]
来源：http://pdc.ydzc1.top

PHP:  $s === strrev($s);
来源：http://qpy.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://hln.jinqigfzy.top

TS:   s === [...s].reverse().join("")
来源：http://mlj.yvedp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cac.fehbvm.com

Go:   // 双指针从两端比较
来源：http://qgb.tanke756.top

Ruby: s == s.reverse
来源：http://etq.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://act.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://sjk.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lmn.xylfe.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ryf.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://imq.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://hko.cheryme.top

Java: // 手写 HashMap
来源：http://kpz.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://ztj.hfpthk.cn

Ruby: // 手写 Hash
来源：http://lrf.yfazqb.com

C#:   // 手写 Dictionary<int, int>
来源：http://vjp.hongshengwenyu.top

[N08] 生成全排列
来源：http://lkj.ydjk.org.cn

Py:   itertools.permutations(arr)
来源：http://bke.0kj1m.cn

PHP:  // 手写递归交换
来源：http://ysk.jinqigufen.top

JS:   // 手写回溯递归
来源：http://frw.jqgfzy.top

TS:   // 手写回溯递归
来源：http://nsc.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://vld.smart0.xyz

Go:   // 手写回溯递归
来源：http://nth.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://gaj.yj202588.top

C#:   // 手写回溯递归
来源：http://nlf.guannengcc.top

[N09] 栈与队列
来源：http://lts.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uec.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hkn.ctjpmb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xgy.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vyq.xziqi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pcs.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wps.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://axm.shzxlz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jxx.guannengcc.top

[N10] 链表节点定义
来源：http://nuo.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xul.bjfxy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qvx.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://trh.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fjf.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://vpz.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://tsz.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bat.sweek.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ycu.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://dno.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cir.yonumen.top

PHP:  // 手写递归函数
来源：http://bfe.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://snk.zhaomingkeji.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rrh.haohaochexian.top

Java: // 手写递归
来源：http://zzz.cdnleiting.top

Go:   // 手写递归
来源：http://ifi.yj202588.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oyg.zhongyouzk.top

C#:   // 手写递归
来源：http://xvo.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bjp.wangshuangyany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qza.havefunace.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ric.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://apw.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fuh.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://plx.vqdsnc.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://orz.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rkq.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://btz.zhongyouzk.top

================================================================================
来源：http://mpr.snrcjt.cn

O. 并发与异步
来源：http://ock.nanxuanxn.top

================================================================================
来源：http://dnt.jinqigfzy.top

[O01] 启动一个线程
来源：http://ewo.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tqp.shangyingyoupin.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jci.zhongyouzk.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://azl.andypj.xyz

TS:   // 同 JS
来源：http://vjk.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://ini.jqgfzy.top

Go:   go f()
来源：http://jpz.hongshengwenyu.top

Ruby: Thread.new { f }
来源：http://abk.316326.xyz

C#:   Task.Run(() => F());
来源：http://hgx.yj20258888.top

[O02] 使用线程池
来源：http://wab.feifeiyinyue.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fak.feifeiyinyue.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dik.sufxvd.cn

JS:   // worker_threads 线程池
来源：http://ugg.ybcxt.top

TS:   // worker_threads 线程池
来源：http://zen.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://uhb.cheryme.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://llf.yongpay.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rur.shzxlz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://obo.uphjek.com

[O03] 加锁保护共享数据
来源：http://ibg.wangdashe.top

Py:   with lock: shared += 1
来源：http://cbu.yvedp.cn

PHP:  // 用 flock() 做文件锁
来源：http://ljb.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dcj.smart0.xyz

TS:   // 同 JS
来源：http://vls.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://ajf.jinqigfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pzi.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mqw.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://ecx.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://qfm.yj20258.top

Py:   async def f():⏎    await g()
来源：http://qii.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fud.sweek.top

JS:   async function f() { await g(); }
来源：http://gke.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://odh.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zcc.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rfq.wangshuangyany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fnw.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://rqn.hywenlv.cn

[O05] 并发执行并等待全部完成
来源：http://rbm.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://xjz.kuanghao11.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ini.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://dxg.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://ubt.chenlongwang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yco.bbcook.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://krg.yj20258.top

Ruby: threads.map(&:join)
来源：http://tfj.zhiwuduotai.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ilw.shangyingyoupin.top

[O06] 使用进程池
来源：http://cmu.yj20258888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ipf.gaohongyu789.top

PHP:  // pcntl_fork 或多进程队列
来源：http://krf.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://idd.yongpay.top

TS:   // child_process / cluster 模块
来源：http://mbq.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://goz.hnxiangtu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://laa.ybcxt.top

Ruby: // fork 块
来源：http://fcz.zdqjudy.top

C#:   Parallel.For
来源：http://kxa.jinqigufen.top

================================================================================
来源：http://igf.sysykeji.top

P. 常用工具函数
来源：http://uod.birdmap.top

================================================================================
来源：http://kcs.yvedp.cn

[P01] 生成 UUID
来源：http://tkc.quarkkingdee.top

Py:   str(uuid.uuid4())
来源：http://nwr.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://avx.bjfxy.top

JS:   crypto.randomUUID()
来源：http://rfj.nanxinkj.top

TS:   crypto.randomUUID()
来源：http://jqt.nanxinkj.top

Java: UUID.randomUUID().toString()
来源：http://dnd.jinyuanbaomall.cn

Go:   // 用 github.com/google/uuid
来源：http://ovm.xingfuxueyuan.xyz

Ruby: SecureRandom.uuid
来源：http://zww.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://vjv.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://sqy.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gwk.sjlbkw.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kgu.zhixingplan.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://osn.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://adg.cqqwz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vys.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gde.shanyushiyangtech.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hpu.gotoacloud.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zgb.ivvv.top

[P03] 生成短随机字符串
来源：http://fce.yangfankeji.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sys.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hlr.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rul.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nrl.xuanzx.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://imb.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mxs.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ywc.316326.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ccv.fanxiaobao.xyz

[P04] 求长度
来源：http://vtl.mhx1999.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ajk.0kj1m.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cvt.dianchejie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tyz.jlsjyb.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zlq.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://hjl.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://jiu.yonumen.top

Ruby: x.length;  x.size
来源：http://suc.yj20258.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bzr.chenzaomai.com

[P05] 判断两个对象内容是否相等
来源：http://mwe.smart0.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://awl.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vus.zhongyouzk.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zbm.jinyuanbaomall.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ssu.shangyingyoupin.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mma.vqdsnc.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tzn.gzhubu.top

Ruby: a == b
来源：http://ypw.yonumen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://win.hcnkem.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eii.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gce.cashguo.top

PHP:  if (empty($x)) {}
来源：http://cjx.jianghu66.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sea.sxryk.cn

TS:   if (x == null) {}
来源：http://ioj.iojbl.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jil.epnwcf.com

Go:   if x == nil {}
来源：http://nif.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qzo.chenlongwang.top

C#:   if (x is null) {}
来源：http://csy.fktsv.cn

[P07] 防抖与节流
来源：http://zmr.wangshuangyany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qfx.gotoacloud.top

PHP:  // 手写时间戳比较
来源：http://hjx.gogol.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zwj.hysaishi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hzh.pycfn.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qwp.vqdsnc.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yms.sxryk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hln.yj20258888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://snf.jinyuanbaomall.cn

[P08] 处理浮点精度问题
来源：http://xpi.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xlw.sysykeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ofl.hesvh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pzv.ehwqpu.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ads.zycfv.cn


<!-- 参考信息 -->