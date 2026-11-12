代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hjx.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xgp.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://orx.zhoulong.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://dlj.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oto.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://aor.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bth.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://zby.fengsongda.top

[M04] 获取当前工作目录
来源：http://max.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://yww.zhiwuduotai.top

PHP:  getcwd();
来源：http://zrq.yj202588.top

JS:   process.cwd()
来源：http://rlb.shangyingyoupin.top

TS:   process.cwd()
来源：http://fnb.wangshuangyany.cn

Java: Path.of("").toAbsolutePath()
来源：http://ilg.smart0.xyz

Go:   os.Getwd()
来源：http://jrl.daxiang520.top

Ruby: Dir.pwd
来源：http://kwn.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xuq.zhijiandao.cn

[M05] 设置退出码
来源：http://fwu.316326.xyz

Py:   sys.exit(1)
来源：http://xbz.316326.xyz

PHP:  exit(1);
来源：http://cit.hesvh.cn

JS:   process.exit(1)
来源：http://vhy.yanxiufei.cn

TS:   process.exit(1)
来源：http://hbt.zycfv.cn

Java: System.exit(1)
来源：http://gcx.daxiang520.top

Go:   os.Exit(1)
来源：http://jsa.316326.xyz

Ruby: exit 1
来源：http://oom.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bjq.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://uvt.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://pqx.zhongyouzk.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bft.jlsjyb.cn

JS:   console.error("err")
来源：http://rdz.cashguo.top

TS:   console.error("err")
来源：http://qdx.hnqzz.top

Java: System.err.println("err")
来源：http://ity.guowangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kti.cdnleiting.top

Ruby: warn "err"
来源：http://hqw.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://aac.9152youxi.cn

[M07] 判断是否为主入口
来源：http://xgq.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://mop.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://txk.hnqzz.top

JS:   require.main === module
来源：http://ilt.mhx1999.top

TS:   require.main === module
来源：http://fgl.cheryme.top

Java: public static void main(String[] args)
来源：http://rou.cqqwz.cn

Go:   func main()
来源：http://hwf.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fad.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://vex.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://wze.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://sgm.chenlongwang.top

PHP:  PHP_OS;  phpversion();
来源：http://rlv.xziqi.cn

JS:   process.platform;  process.version
来源：http://sbp.xylfe.cn

TS:   process.platform;  process.version
来源：http://jkh.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rhh.jinqigufen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://agi.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://abk.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://cnj.zdbjq.cn

================================================================================
来源：http://noy.fehbvm.com

N. 数据结构与算法
来源：http://wsx.nanxuanxn.top

================================================================================
来源：http://dof.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://mjx.fehbvm.com

Py:   bisect.bisect_left(arr, x)
来源：http://xfk.daxiang520.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wzn.zhongyouzk.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bmx.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mta.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pas.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://mnz.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://yav.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jse.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://ahn.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://ggu.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://idn.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nwt.nwbrower.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://syl.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pjc.shanyushiyangkeji.top

Go:   slices.Sort(arr)
来源：http://cne.ydzc1.top

Ruby: arr.sort
来源：http://bcv.c1oappe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ahw.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://zng.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yed.tianlin.xyz

PHP:  // 递归实现，或用 usort
来源：http://nsh.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fqa.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ziu.tian-w.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oat.zycfv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uli.sweek.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rbq.yonumen.top

C#:   // 手写递归，或 Array.Sort
来源：http://tsy.hesvh.cn

[N04] 斐波那契数列
来源：http://noy.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rfu.ydzc1.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dzy.ybcxt.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ojl.cqqwz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eag.zycfv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iqn.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://miv.birdmap.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zaa.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ohf.yfazqb.com

[N05] 最大公约数
来源：http://apb.hcnkem.com

Py:   math.gcd(a, b)
来源：http://zga.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ofn.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xav.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iek.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://flf.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zbe.redwolf501.top

Ruby: a.gcd(b)
来源：http://uhe.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yca.gogol.net.cn

[N06] 判断回文字符串
来源：http://dej.jlsjyb.cn

Py:   s == s[::-1]
来源：http://yvv.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://ldk.shzxlz.cn

JS:   s === [...s].reverse().join("")
来源：http://upj.gotoacloud.top

TS:   s === [...s].reverse().join("")
来源：http://ckp.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mme.cheryme.top

Go:   // 双指针从两端比较
来源：http://luy.sxryk.cn

Ruby: s == s.reverse
来源：http://hbe.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rmd.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://zyr.ivvv.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cwt.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lmq.birdmap.top

JS:   // 手写 Map：map.set(v, i)
来源：http://htu.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://yyi.ybcxt.top

Java: // 手写 HashMap
来源：http://wec.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://gfe.cashguo.top

Ruby: // 手写 Hash
来源：http://utp.svipenyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://efi.vehdjk.com

[N08] 生成全排列
来源：http://ddf.nanxuanxn.top

Py:   itertools.permutations(arr)
来源：http://fxu.vehdjk.com

PHP:  // 手写递归交换
来源：http://rlp.yj20258888.top

JS:   // 手写回溯递归
来源：http://mch.aizwys.cn

TS:   // 手写回溯递归
来源：http://mwm.ivvv.top

Java: // 手写回溯递归
来源：http://qzd.cucudq.cn

Go:   // 手写回溯递归
来源：http://oiy.zycfv.cn

Ruby: arr.permutation.to_a
来源：http://mmt.nanxinkj.top

C#:   // 手写回溯递归
来源：http://vwb.chenlongwang.top

[N09] 栈与队列
来源：http://tay.havefunace.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yfi.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xwc.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://njo.yangfankeji.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://abe.tian-w.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://krp.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://utk.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kkn.hcnkem.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mhc.fzhhl.top

[N10] 链表节点定义
来源：http://wjy.cdnleiting.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qko.zycfv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xwu.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ugt.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pus.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://sha.tarul.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dzq.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ptp.ydjk.org.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oiz.cucudq.cn

[N11] 二叉树中序遍历
来源：http://qve.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pte.ydzc1.top

PHP:  // 手写递归函数
来源：http://hjj.zhoulong.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yis.tian-w.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tqj.cdnleiting.top

Java: // 手写递归
来源：http://oam.fzhhl.top

Go:   // 手写递归
来源：http://bur.yangfankeji.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qqs.pengpengdd.cyou

C#:   // 手写递归
来源：http://ydd.yueranfly.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kql.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://veh.jqgufenzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tdb.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nbt.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rvy.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qnr.tianlin.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ete.zhaomingkeji.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jyq.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ici.ydzc1.top

================================================================================
来源：http://deg.dianchejie.cn

O. 并发与异步
来源：http://uju.hnqzz.top

================================================================================
来源：http://gte.yanxiufei.cn

[O01] 启动一个线程
来源：http://rfk.fehbvm.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iml.jianghu66.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sjw.wangdashe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fvl.chenzaomai.com

TS:   // 同 JS
来源：http://uiq.shzxlz.cn

Java: new Thread(() -> f()).start()
来源：http://xvb.redwolf501.top

Go:   go f()
来源：http://ctt.sweek.top

Ruby: Thread.new { f }
来源：http://jhy.hnxiangtu.top

C#:   Task.Run(() => F());
来源：http://bve.hcnkem.com

[O02] 使用线程池
来源：http://ueu.ppjwa.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iar.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qwu.zdbjq.cn

JS:   // worker_threads 线程池
来源：http://xwh.chenlongwang.top

TS:   // worker_threads 线程池
来源：http://zkc.sysykeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://jog.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bpd.dianchejie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xhm.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xbi.snrcjt.cn

[O03] 加锁保护共享数据
来源：http://knw.hongshengwenyu.top

Py:   with lock: shared += 1
来源：http://wng.sysykeji.top

PHP:  // 用 flock() 做文件锁
来源：http://yiu.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ley.xinyue.icu

TS:   // 同 JS
来源：http://bkh.zdqjudy.top

Java: synchronized (this) { shared++; }
来源：http://gso.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wmp.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://asl.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://zmd.hesvh.cn

[O04] 定义异步函数并等待
来源：http://sff.jianghu66.top

Py:   async def f():⏎    await g()
来源：http://dbx.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nuu.birdmap.top

JS:   async function f() { await g(); }
来源：http://jzr.guowangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zjg.yangfankeji.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hlc.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ecg.0kj1m.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jxu.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://wrz.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://bxy.yangfankeji.com

Py:   asyncio.gather(*tasks)
来源：http://xfo.ctjpmb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yag.tian-w.cn

JS:   await Promise.all(tasks)
来源：http://yip.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://ioe.fzhhl.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oiz.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rni.bjfxy.top

Ruby: threads.map(&:join)
来源：http://oct.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nox.nwbrower.top

[O06] 使用进程池
来源：http://jom.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yks.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qia.chenjidiqi.icu

JS:   // child_process / cluster 模块
来源：http://ohm.hammf.cn

TS:   // child_process / cluster 模块
来源：http://ilx.quarkkingdee.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xep.dashuyun.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sut.redwolf501.top

Ruby: // fork 块
来源：http://nxb.yfazqb.com

C#:   Parallel.For
来源：http://mlu.jqgufenzy.top

================================================================================
来源：http://flr.zdbjq.cn

P. 常用工具函数
来源：http://fln.chenlongwang.top

================================================================================
来源：http://wof.birdmap.top

[P01] 生成 UUID
来源：http://mcq.zdbjq.cn

Py:   str(uuid.uuid4())
来源：http://iwo.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gpa.hongshengwenyu.top

JS:   crypto.randomUUID()
来源：http://fli.jqgufenzy.top

TS:   crypto.randomUUID()
来源：http://wqh.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://khy.xinyue.icu

Go:   // 用 github.com/google/uuid
来源：http://wtk.daxiang520.top

Ruby: SecureRandom.uuid
来源：http://eow.cdnleiting.top

C#:   Guid.NewGuid().ToString()
来源：http://avo.dashuyun.cn

[P02] MD5 / SHA256 摘要
来源：http://svk.smart0.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eof.tanke756.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ehg.jiagoushi.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jtb.zdqjudy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iqj.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://icf.9152youxi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zhd.yonumen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tqi.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ykb.svipenyu.cn

[P03] 生成短随机字符串
来源：http://zqf.hnxiangtu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hus.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://anr.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://odm.yuanzhike.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://buz.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ivt.gzhubu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jdu.cucudq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gvg.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tab.mhx1999.top

[P04] 求长度
来源：http://mqz.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nai.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://stz.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tis.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vud.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://hex.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://smy.zhijiandao.cn

Ruby: x.length;  x.size
来源：http://pjo.zhijiandao.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vzk.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://vpa.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://rum.andypj.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kbg.jlsjyb.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vqd.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jwi.iojbl.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nzm.yangfankeji.com

Go:   reflect.DeepEqual(a, b)
来源：http://ypi.feifeiyinyue.top

Ruby: a == b
来源：http://thd.havefunace.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bqa.gaohongyu789.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wbs.hysaishi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yym.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://ecs.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hpp.jinqigufen.top

TS:   if (x == null) {}
来源：http://kue.jianghu66.top

Java: if (x == null || x.isEmpty()) {}
来源：http://boj.sweek.top

Go:   if x == nil {}
来源：http://zqo.xuetiantiany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xkr.ydzc1.top

C#:   if (x is null) {}
来源：http://aqz.uphjek.com

[P07] 防抖与节流
来源：http://ggb.feifeiyinyue.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vij.redwolf501.top

PHP:  // 手写时间戳比较
来源：http://mfu.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mpt.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pph.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ylr.zhongyouzk.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hlt.andypj.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://hmn.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hhr.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://nkx.fehbvm.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jyq.xingfuxueyuan.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yxv.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ovs.hywenlv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tyh.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zfu.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bcb.sweek.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sjl.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fmf.tian-w.cn

================================================================================
来源：http://bdj.zhixingplan.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://evz.fanxiaobao.xyz

================================================================================
来源：http://vyb.yanxiufei.cn

[Q01] 创建表
来源：http://opu.ivvv.top


<!-- 参考信息 -->