代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vej.birdmap.top

Ruby: ENV["HOME"]
来源：http://jhk.zhengqikj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bvi.gaohongyu789.top

[M03] 执行外部命令
来源：http://ujf.zhoulong.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aui.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gwk.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qlr.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rpn.yueranfly.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hcx.zhoulong.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://jbf.aibaodan.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oyk.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://gju.daxiang520.top

[M04] 获取当前工作目录
来源：http://xuv.yueranfly.top

Py:   os.getcwd()
来源：http://wcf.sweek.top

PHP:  getcwd();
来源：http://vns.sxryk.cn

JS:   process.cwd()
来源：http://cbc.cdnleiting.top

TS:   process.cwd()
来源：http://ssm.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://snj.fehbvm.com

Go:   os.Getwd()
来源：http://bjv.zycfv.cn

Ruby: Dir.pwd
来源：http://gsw.0kj1m.cn

C#:   Directory.GetCurrentDirectory()
来源：http://twt.0kj1m.cn

[M05] 设置退出码
来源：http://wpy.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://kim.feifeiyinyue.top

PHP:  exit(1);
来源：http://tbq.yfazqb.com

JS:   process.exit(1)
来源：http://nri.jianghu66.top

TS:   process.exit(1)
来源：http://vfz.yanxiufei.cn

Java: System.exit(1)
来源：http://tef.andypj.xyz

Go:   os.Exit(1)
来源：http://pzf.hesvh.cn

Ruby: exit 1
来源：http://src.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fip.andypj.xyz

[M06] 向标准错误输出
来源：http://yzq.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://bsg.quarkkingdee.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lfi.0kj1m.cn

JS:   console.error("err")
来源：http://gqr.gotoacloud.top

TS:   console.error("err")
来源：http://els.jqgfzy.top

Java: System.err.println("err")
来源：http://kfd.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zqu.zhengqikj.top

Ruby: warn "err"
来源：http://gts.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://gmf.9152youxi.cn

[M07] 判断是否为主入口
来源：http://qpn.haohaochexian.top

Py:   if __name__ == "__main__":
来源：http://xig.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jmx.fanxiaobao.xyz

JS:   require.main === module
来源：http://xnv.feifeiyinyue.top

TS:   require.main === module
来源：http://yjh.andypj.xyz

Java: public static void main(String[] args)
来源：http://hpq.redwolf501.top

Go:   func main()
来源：http://kbq.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mdk.shuidangran.top

C#:   static void Main(string[] args)
来源：http://vhf.ydjk.org.cn

[M08] 获取系统与运行时信息
来源：http://kij.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://zsc.ctjpmb.com

PHP:  PHP_OS;  phpversion();
来源：http://qzi.ybcxt.top

JS:   process.platform;  process.version
来源：http://mnv.cdnleiting.top

TS:   process.platform;  process.version
来源：http://rjn.epnwcf.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gep.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://eic.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rbs.andypj.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://ery.chenlongwang.top

================================================================================
来源：http://omt.yj202588.top

N. 数据结构与算法
来源：http://gqp.uphjek.com

================================================================================
来源：http://vlh.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://jvx.sysykeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://gvj.yvedp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wrm.yangfankeji.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cen.xuanzx.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iup.jiagoushi.top

Java: Arrays.binarySearch(arr, x)
来源：http://ghx.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://rjs.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://plv.fanxiaobao.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://fpi.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://ppg.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qdm.shanyushiyangtech.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ale.zhixingplan.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nnr.uphjek.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://hpd.yanxiufei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pnz.yj202588.top

Go:   slices.Sort(arr)
来源：http://wjm.gaohongyu789.top

Ruby: arr.sort
来源：http://kmc.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://cbj.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://fwf.guannengcc.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oam.tanke756.top

PHP:  // 递归实现，或用 usort
来源：http://pfw.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lpv.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bhp.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qpf.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://csu.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kgr.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://kec.bbcook.cn

[N04] 斐波那契数列
来源：http://frt.fktsv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://api.yj20258.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hxn.jinqigfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kwk.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tpb.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rhz.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ble.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pqs.dianchejie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hpd.ppjwa.cn

[N05] 最大公约数
来源：http://sev.uphjek.com

Py:   math.gcd(a, b)
来源：http://idb.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mdi.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bii.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gkj.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yuh.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pal.vehdjk.com

Ruby: a.gcd(b)
来源：http://cpl.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://duj.gogol.net.cn

[N06] 判断回文字符串
来源：http://vvr.jqgufenzy.top

Py:   s == s[::-1]
来源：http://bev.nanxuanxn.top

PHP:  $s === strrev($s);
来源：http://cia.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://anf.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://lff.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zsr.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://chx.ppjwa.cn

Ruby: s == s.reverse
来源：http://whp.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rti.uphjek.com

[N07] 两数之和（返回下标）
来源：http://gqj.nwbrower.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://twb.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://igr.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://khu.quarkkingdee.top

TS:   // 手写 Map<string, number>
来源：http://kbi.hnxiangtu.top

Java: // 手写 HashMap
来源：http://tbp.fengsongda.top

Go:   // 手写 map[int]int
来源：http://wca.cucudq.cn

Ruby: // 手写 Hash
来源：http://zbm.guannengcc.top

C#:   // 手写 Dictionary<int, int>
来源：http://jxn.sysykeji.top

[N08] 生成全排列
来源：http://dmh.xuetiantiany.cn

Py:   itertools.permutations(arr)
来源：http://oco.0kj1m.cn

PHP:  // 手写递归交换
来源：http://bya.zhaomingkeji.xyz

JS:   // 手写回溯递归
来源：http://ffg.xingfuxueyuan.xyz

TS:   // 手写回溯递归
来源：http://vjn.zhongyouzk.top

Java: // 手写回溯递归
来源：http://nvv.yvedp.cn

Go:   // 手写回溯递归
来源：http://kdv.ivvv.top

Ruby: arr.permutation.to_a
来源：http://kal.nanxuanxn.top

C#:   // 手写回溯递归
来源：http://kow.zhiwuduotai.top

[N09] 栈与队列
来源：http://bwy.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dmd.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ymu.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zwy.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kmg.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dpl.vqdsnc.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pog.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yjc.zdqjudy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yii.yfazqb.com

[N10] 链表节点定义
来源：http://bji.fanxiaobao.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://knn.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ygi.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qyw.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jyp.yuxming.cn

Java: class Node { int v; Node next; }
来源：http://zew.dashuyun.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ilg.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wty.gogol.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mby.jyoumei.cn

[N11] 二叉树中序遍历
来源：http://etr.fzhhl.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eas.fzhhl.top

PHP:  // 手写递归函数
来源：http://czb.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ytf.yj20258888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eku.dianchejie.cn

Java: // 手写递归
来源：http://yku.hnqzz.top

Go:   // 手写递归
来源：http://ijz.feifeiyinyue.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rhm.yongpay.top

C#:   // 手写递归
来源：http://ypw.yj20258888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qph.cqqwz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://del.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sla.tian-w.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xnf.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ags.pengpengdd.cyou

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tgs.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mly.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yuw.jianghu66.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tid.sweek.top

================================================================================
来源：http://owk.sjlbkw.cn

O. 并发与异步
来源：http://sts.jinyuanbaomall.cn

================================================================================
来源：http://nta.wangdashe.top

[O01] 启动一个线程
来源：http://szo.vehdjk.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hfg.aizwys.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pjw.cheryme.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vqo.xinyue.icu

TS:   // 同 JS
来源：http://ojr.hcnkem.com

Java: new Thread(() -> f()).start()
来源：http://wir.hywenlv.cn

Go:   go f()
来源：http://rdr.jinqigufen.top

Ruby: Thread.new { f }
来源：http://zqh.zhiwuduotai.top

C#:   Task.Run(() => F());
来源：http://nab.hfpthk.cn

[O02] 使用线程池
来源：http://ori.jqgfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pxd.dianchejie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vmk.fehbvm.com

JS:   // worker_threads 线程池
来源：http://rpx.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://lgs.fktsv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dyg.shuidangran.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jmj.hysaishi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nbx.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xlz.svipenyu.cn

[O03] 加锁保护共享数据
来源：http://cpg.dashuyun.cn

Py:   with lock: shared += 1
来源：http://xgq.zhoulong.xyz

PHP:  // 用 flock() 做文件锁
来源：http://evo.zhongyouzk.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eho.sjlbkw.cn

TS:   // 同 JS
来源：http://jay.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://ceb.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vta.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://chp.nwbrower.top

C#:   lock (gate) { shared++; }
来源：http://qyu.cashguo.top

[O04] 定义异步函数并等待
来源：http://unl.sufxvd.cn

Py:   async def f():⏎    await g()
来源：http://fzg.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ueb.cheryme.top

JS:   async function f() { await g(); }
来源：http://ohc.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://viy.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bel.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://flj.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://twh.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://kaw.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://kvy.daria6918.cn

Py:   asyncio.gather(*tasks)
来源：http://hvj.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ilr.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://ihh.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://yqm.dianchejie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kve.xingfuxueyuan.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://npg.jiagoushi.top

Ruby: threads.map(&:join)
来源：http://scp.zhixingplan.top

C#:   await Task.WhenAll(t1, t2)
来源：http://frh.bjfxy.top

[O06] 使用进程池
来源：http://ost.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ppk.jinqigufen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://umd.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://tjh.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://zfy.sjlbkw.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://peo.jinqigfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tuz.tian-w.cn

Ruby: // fork 块
来源：http://egu.zhixingplan.top

C#:   Parallel.For
来源：http://vnn.ydzc1.top

================================================================================
来源：http://jcl.nanxuanxn.top

P. 常用工具函数
来源：http://awf.yonumen.top

================================================================================
来源：http://tze.meibo888.top

[P01] 生成 UUID
来源：http://uph.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://puv.epnwcf.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pqv.yfazqb.com

JS:   crypto.randomUUID()
来源：http://prn.fktsv.cn

TS:   crypto.randomUUID()
来源：http://vgd.ehwqpu.com

Java: UUID.randomUUID().toString()
来源：http://xbx.0kj1m.cn

Go:   // 用 github.com/google/uuid
来源：http://hnl.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://cpg.ppjwa.cn

C#:   Guid.NewGuid().ToString()
来源：http://kfc.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://qsa.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hvp.guowangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lkf.snrcjt.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dno.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ugw.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rpb.nwbrower.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hil.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cyy.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ozc.haohaochexian.top

[P03] 生成短随机字符串
来源：http://vtz.fzhhl.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mwt.yanxiufei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mdr.cheryme.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vel.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://det.cheryme.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gjr.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wns.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://iks.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kgc.wangshuangyany.cn

[P04] 求长度
来源：http://ozj.shangyingyoupin.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://imi.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nbk.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xmp.jqgufenzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mqa.yj20258888.top

Java: list.size();  map.size();  s.length()
来源：http://hag.ctjpmb.com

Go:   len(arr);  len(m)
来源：http://hgc.gotoacloud.top

Ruby: x.length;  x.size
来源：http://hwa.ydzc1.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://uoo.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://uqv.jyoumei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bqr.hesvh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kwb.andypj.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gqj.smart0.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zjq.yvedp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mls.daria6918.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lnu.jqgfzy.top

Ruby: a == b
来源：http://tlv.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://auh.wangshuangyany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zfe.ydjk.org.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qvh.nanxuanxn.top

PHP:  if (empty($x)) {}
来源：http://iru.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yfu.gogol.net.cn

TS:   if (x == null) {}
来源：http://ubx.havefunace.top

Java: if (x == null || x.isEmpty()) {}
来源：http://knl.shuidangran.top

Go:   if x == nil {}
来源：http://ghh.jqgufenzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://byd.cheryme.top

C#:   if (x is null) {}
来源：http://ijp.zycfv.cn

[P07] 防抖与节流
来源：http://vnx.ppjwa.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ocs.xziqi.cn

PHP:  // 手写时间戳比较
来源：http://puf.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://esb.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://var.ppjwa.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cxy.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://soi.yuanzhike.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wpz.iojbl.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ttp.hysaishi.cn

[P08] 处理浮点精度问题
来源：http://vzp.tanke756.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://agt.ywan-chungtsiang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mbi.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://msp.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iyi.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gdf.shangyingyoupin.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uvf.chenlongwang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oje.daria6918.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sfi.ivvv.top


<!-- 参考信息 -->