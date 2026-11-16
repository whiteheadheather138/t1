代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mvl.svipenyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zvc.feifeiyinyue.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zok.pycfn.com

TS:   child_process.execSync("ls -l").toString()
来源：http://zsm.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oom.yfazqb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://vac.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vaa.meibo888.top

C#:   Process.Start("ls", "-l");
来源：http://bxi.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://aig.xuanzx.com

Py:   os.getcwd()
来源：http://joj.zhongyouzk.top

PHP:  getcwd();
来源：http://pei.xylfe.cn

JS:   process.cwd()
来源：http://xzy.tarul.cn

TS:   process.cwd()
来源：http://eiz.jqgufenzy.top

Java: Path.of("").toAbsolutePath()
来源：http://pjw.gogol.net.cn

Go:   os.Getwd()
来源：http://hnl.shanyushiyangkeji.top

Ruby: Dir.pwd
来源：http://iri.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://bdr.sxryk.cn

[M05] 设置退出码
来源：http://uof.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://ihu.dashuyun.cn

PHP:  exit(1);
来源：http://ubf.iojbl.cn

JS:   process.exit(1)
来源：http://koi.ehwqpu.com

TS:   process.exit(1)
来源：http://thi.chenjidiqi.icu

Java: System.exit(1)
来源：http://mry.yuxming.cn

Go:   os.Exit(1)
来源：http://jqm.fktsv.cn

Ruby: exit 1
来源：http://ifh.sufxvd.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qce.yj20258.top

[M06] 向标准错误输出
来源：http://wmc.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://cmm.zycfv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://otn.52xcode.cn

JS:   console.error("err")
来源：http://xit.pengpengdd.cyou

TS:   console.error("err")
来源：http://jws.jqgufenzy.top

Java: System.err.println("err")
来源：http://buc.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ypz.zhongyouzk.top

Ruby: warn "err"
来源：http://exn.nanxuanxn.top

C#:   Console.Error.WriteLine("err")
来源：http://vcu.yongpay.top

[M07] 判断是否为主入口
来源：http://bnr.cheryme.top

Py:   if __name__ == "__main__":
来源：http://uag.shuidangran.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gcd.hfpthk.cn

JS:   require.main === module
来源：http://fyj.yvedp.cn

TS:   require.main === module
来源：http://gal.yonumen.top

Java: public static void main(String[] args)
来源：http://uoi.jinghuilouyu.cn

Go:   func main()
来源：http://lda.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sdq.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://rxh.bjfxy.top

[M08] 获取系统与运行时信息
来源：http://uyd.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://ffi.zhijiandao.cn

PHP:  PHP_OS;  phpversion();
来源：http://anp.aibaodan.cn

JS:   process.platform;  process.version
来源：http://vqr.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://vho.gzhubu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jsh.hammf.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rad.sufxvd.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uic.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hwd.xuetiantiany.cn

================================================================================
来源：http://jhc.jinghuilouyu.cn

N. 数据结构与算法
来源：http://kce.aizwys.cn

================================================================================
来源：http://ivp.meibo888.top

[N01] 二分查找（有序数组）
来源：http://cns.yangfankeji.com

Py:   bisect.bisect_left(arr, x)
来源：http://zow.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mlh.ehwqpu.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jbu.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hbs.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://efo.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://adr.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kug.yonumen.top

C#:   Array.BinarySearch(arr, x)
来源：http://ggg.yonumen.top

[N02] 排序（工程实践用内置实现）
来源：http://vjq.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://ner.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vcn.kuanghao11.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zuk.yuanzhike.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pyv.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://upm.wangdashe.top

Go:   slices.Sort(arr)
来源：http://pki.xuanzx.com

Ruby: arr.sort
来源：http://zmh.jqgfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ytq.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://vnl.havefunace.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iuk.yanxiufei.cn

PHP:  // 递归实现，或用 usort
来源：http://xzl.hfpthk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qka.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tdg.xuetiantiany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yqx.ivvv.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jbm.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://exh.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pwv.sufxvd.cn

[N04] 斐波那契数列
来源：http://psi.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sjz.zhoulong.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bof.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://set.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mwd.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sqw.snrcjt.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kms.iojbl.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tis.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ecn.tianlin.xyz

[N05] 最大公约数
来源：http://ntw.svipenyu.cn

Py:   math.gcd(a, b)
来源：http://uhx.yuxming.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kak.ydzc1.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qit.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hrx.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iky.tanke756.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qvp.cqqwz.cn

Ruby: a.gcd(b)
来源：http://ouh.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ynk.fehbvm.com

[N06] 判断回文字符串
来源：http://xpr.zhijiandao.cn

Py:   s == s[::-1]
来源：http://gti.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://cdq.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://wal.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://hsc.sweek.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nuu.havefunace.top

Go:   // 双指针从两端比较
来源：http://iqh.haohaochexian.top

Ruby: s == s.reverse
来源：http://vsi.snrcjt.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zko.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://ktu.wangdashe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kcs.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qwx.zhaomingkeji.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://etv.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://iiz.0kj1m.cn

Java: // 手写 HashMap
来源：http://gwi.sweek.top

Go:   // 手写 map[int]int
来源：http://cpv.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://clc.yfazqb.com

C#:   // 手写 Dictionary<int, int>
来源：http://gwi.gotoacloud.top

[N08] 生成全排列
来源：http://ump.yj202588.top

Py:   itertools.permutations(arr)
来源：http://dhg.ybcxt.top

PHP:  // 手写递归交换
来源：http://vxj.cqqwz.cn

JS:   // 手写回溯递归
来源：http://srn.zdqjudy.top

TS:   // 手写回溯递归
来源：http://ztt.tarul.cn

Java: // 手写回溯递归
来源：http://mjr.cheryme.top

Go:   // 手写回溯递归
来源：http://wqm.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://rpa.ctjpmb.com

C#:   // 手写回溯递归
来源：http://dpt.nwbrower.top

[N09] 栈与队列
来源：http://dpw.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ujs.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zaa.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vgn.hongshengwenyu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zcz.sufxvd.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aeb.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vqp.ppjwa.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hvo.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://piw.pengpengdd.cyou

[N10] 链表节点定义
来源：http://jpc.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://urh.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xak.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lit.ydzc1.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dow.tarul.cn

Java: class Node { int v; Node next; }
来源：http://ckr.jlsjyb.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rlo.epnwcf.com

Ruby: Node = Struct.new(:v, :next)
来源：http://zeg.feifeiyinyue.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jsa.cdnleiting.top

[N11] 二叉树中序遍历
来源：http://mdk.316326.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uhw.uphjek.com

PHP:  // 手写递归函数
来源：http://xxh.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aqt.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nwp.jqgufenzy.top

Java: // 手写递归
来源：http://fcn.ppjwa.cn

Go:   // 手写递归
来源：http://sws.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lbp.nwbrower.top

C#:   // 手写递归
来源：http://tls.hnxiangtu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nee.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eaw.feifeiyinyue.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wwr.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://afq.hnxiangtu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://doq.hfpthk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://frz.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ohz.52xcode.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xkd.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mhm.yongpay.top

================================================================================
来源：http://obw.chenzaomai.com

O. 并发与异步
来源：http://xxq.shuidangran.top

================================================================================
来源：http://sbr.zdbjq.cn

[O01] 启动一个线程
来源：http://lex.hammf.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jkv.pengpengdd.cyou

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://txx.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://man.sxryk.cn

TS:   // 同 JS
来源：http://niz.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://zya.uphjek.com

Go:   go f()
来源：http://uer.xylfe.cn

Ruby: Thread.new { f }
来源：http://ojq.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://vwn.jinqigfzy.top

[O02] 使用线程池
来源：http://lnk.pengpengdd.cyou

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tmd.hnxiangtu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://itf.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://fia.shuidangran.top

TS:   // worker_threads 线程池
来源：http://cxu.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://edk.kuanghao11.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vuj.daria6918.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iiw.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zmo.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://gck.tarul.cn

Py:   with lock: shared += 1
来源：http://hwr.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://gjq.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qpd.dianchejie.cn

TS:   // 同 JS
来源：http://dat.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://ozk.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ubn.feifeiyinyue.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gsb.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://yio.tanke756.top

[O04] 定义异步函数并等待
来源：http://szm.yj20258888.top

Py:   async def f():⏎    await g()
来源：http://crp.jqgfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nwn.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://gzg.svipenyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cjk.hnxiangtu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://owi.yfazqb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ycz.yuxming.cn

Ruby: # 用 Fiber 或 async gem
来源：http://exk.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://ltj.iojbl.cn

[O05] 并发执行并等待全部完成
来源：http://khz.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://mpc.zhaomingkeji.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://igb.sufxvd.cn

JS:   await Promise.all(tasks)
来源：http://oxx.yongpay.top

TS:   await Promise.all(tasks)
来源：http://jdk.cashguo.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qwp.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oxr.ydjk.org.cn

Ruby: threads.map(&:join)
来源：http://vqe.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://eqv.pycfn.com

[O06] 使用进程池
来源：http://pzx.kuanghao11.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jbp.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://orn.xuanzx.com

JS:   // child_process / cluster 模块
来源：http://gnr.nwbrower.top

TS:   // child_process / cluster 模块
来源：http://qed.smart0.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mun.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zsv.ehwqpu.com

Ruby: // fork 块
来源：http://drv.ydzc1.top

C#:   Parallel.For
来源：http://vrf.hesvh.cn

================================================================================
来源：http://zsq.hongshengwenyu.top

P. 常用工具函数
来源：http://eqx.yanxiufei.cn

================================================================================
来源：http://tan.gaohongyu789.top

[P01] 生成 UUID
来源：http://wpj.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://zwj.jinyuanbaomall.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jgw.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://qxs.tanke756.top

TS:   crypto.randomUUID()
来源：http://rqf.zhoulong.xyz

Java: UUID.randomUUID().toString()
来源：http://pxq.tarul.cn

Go:   // 用 github.com/google/uuid
来源：http://xwy.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://wfe.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://fpd.0kj1m.cn

[P02] MD5 / SHA256 摘要
来源：http://mlk.ehwqpu.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lsq.andypj.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://odf.jinqigufen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jgf.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qpv.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wdy.jyoumei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pkx.xziqi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rke.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qbh.dashuyun.cn

[P03] 生成短随机字符串
来源：http://ojl.xuetiantiany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bgo.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ijp.hnxiangtu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wfj.zycfv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zjy.guannengcc.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ula.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://atq.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zyy.sufxvd.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ume.cheryme.top

[P04] 求长度
来源：http://qad.svipenyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qic.chenlongwang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wyz.ivvv.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ehl.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://asy.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://aso.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://qru.shuidangran.top

Ruby: x.length;  x.size
来源：http://tvt.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://igf.hnxiangtu.top

[P05] 判断两个对象内容是否相等
来源：http://pxy.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rtl.xuetiantiany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://alc.jinghuilouyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iek.jinyuanbaomall.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://opw.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dza.dashuyun.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yme.0kj1m.cn

Ruby: a == b
来源：http://auj.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rpw.yfazqb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bou.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tjx.dianchejie.cn

PHP:  if (empty($x)) {}
来源：http://krl.hongshengwenyu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ric.yj20258.top

TS:   if (x == null) {}
来源：http://ddk.wangdashe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mki.fehbvm.com

Go:   if x == nil {}
来源：http://eyu.jinghuilouyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://psa.pycfn.com

C#:   if (x is null) {}
来源：http://xma.ydzc1.top

[P07] 防抖与节流
来源：http://wgn.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qgg.52xcode.cn

PHP:  // 手写时间戳比较
来源：http://zhh.epnwcf.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pyl.shangyingyoupin.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qxt.tarul.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eip.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://awv.havefunace.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gmn.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ehp.shanyushiyangtech.top

[P08] 处理浮点精度问题
来源：http://jew.c1oappe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://egg.jinyuanbaomall.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qht.quarkkingdee.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://duw.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qre.guannengcc.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mdi.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kho.jianghu66.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wjt.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://whx.sysykeji.top

================================================================================
来源：http://ovk.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nyi.xuetiantiany.cn

================================================================================
来源：http://fmg.sufxvd.cn

[Q01] 创建表
来源：http://bry.52xcode.cn


<!-- 参考信息 -->