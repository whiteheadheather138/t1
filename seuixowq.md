代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hkp.tarul.cn

Ruby: ENV["HOME"]
来源：http://nft.xuanzx.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ovb.xylfe.cn

[M03] 执行外部命令
来源：http://yav.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aot.yj20258.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dsh.jinqigufen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wqs.zhengqikj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kob.jianghu66.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fvn.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dcj.hongshengwenyu.top

Ruby: system("ls -l");  `ls -l`
来源：http://pvn.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://xhn.yonumen.top

[M04] 获取当前工作目录
来源：http://uuf.316326.xyz

Py:   os.getcwd()
来源：http://rsv.epnwcf.com

PHP:  getcwd();
来源：http://pma.xinyue.icu

JS:   process.cwd()
来源：http://wrs.yuxming.cn

TS:   process.cwd()
来源：http://fle.zhoulong.xyz

Java: Path.of("").toAbsolutePath()
来源：http://lmq.gogol.net.cn

Go:   os.Getwd()
来源：http://ghi.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://zep.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://cvk.sweek.top

[M05] 设置退出码
来源：http://rup.jianghu66.top

Py:   sys.exit(1)
来源：http://qsl.daria6918.cn

PHP:  exit(1);
来源：http://nhb.dianchejie.cn

JS:   process.exit(1)
来源：http://rqi.yj202588.top

TS:   process.exit(1)
来源：http://vpw.cdnleiting.top

Java: System.exit(1)
来源：http://kzb.havefunace.top

Go:   os.Exit(1)
来源：http://qfj.zdbjq.cn

Ruby: exit 1
来源：http://mou.xziqi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ooj.fanxiaobao.xyz

[M06] 向标准错误输出
来源：http://uwx.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://ubb.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jzm.hesvh.cn

JS:   console.error("err")
来源：http://jta.hnqzz.top

TS:   console.error("err")
来源：http://tkz.jqgufenzy.top

Java: System.err.println("err")
来源：http://vjp.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nss.jinqigufen.top

Ruby: warn "err"
来源：http://jpz.zhoulong.xyz

C#:   Console.Error.WriteLine("err")
来源：http://puf.xziqi.cn

[M07] 判断是否为主入口
来源：http://znl.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://czh.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kzf.yj202588.top

JS:   require.main === module
来源：http://aat.jqgfzy.top

TS:   require.main === module
来源：http://hew.hammf.cn

Java: public static void main(String[] args)
来源：http://cso.daria6918.cn

Go:   func main()
来源：http://rpk.snrcjt.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pij.guannengcc.top

C#:   static void Main(string[] args)
来源：http://rgf.wangdashe.top

[M08] 获取系统与运行时信息
来源：http://fhf.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://kaz.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://fgw.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://agy.ybcxt.top

TS:   process.platform;  process.version
来源：http://imb.aibaodan.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vvf.shanyushiyangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://evu.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qhh.yuanzhike.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://srn.0kj1m.cn

================================================================================
来源：http://brk.pengpengdd.cyou

N. 数据结构与算法
来源：http://zfg.feifeiyinyue.top

================================================================================
来源：http://rjt.yj20258.top

[N01] 二分查找（有序数组）
来源：http://vai.vqdsnc.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bvo.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rep.gogol.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://scb.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tcs.ywan-chungtsiang.top

Java: Arrays.binarySearch(arr, x)
来源：http://xyp.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://dji.nwbrower.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://taw.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://dof.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://cqf.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://mug.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iik.jqgufenzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://igm.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bsy.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eiq.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://xrb.cqqwz.cn

Ruby: arr.sort
来源：http://qai.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://duv.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://tns.nwbrower.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ief.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://rpg.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mja.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bta.tian-w.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nej.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://koi.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rfz.dianchejie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oji.9152youxi.cn

[N04] 斐波那契数列
来源：http://ycn.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kkz.ivvv.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://drd.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wws.nanxuanxn.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://olq.yongpay.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wez.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://duy.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dfs.birdmap.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ajg.jinghuilouyu.cn

[N05] 最大公约数
来源：http://lql.yvedp.cn

Py:   math.gcd(a, b)
来源：http://ono.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cnc.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dam.sjlbkw.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qkz.jiagoushi.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jux.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cht.gaohongyu789.top

Ruby: a.gcd(b)
来源：http://ukt.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hoj.pengpengdd.cyou

[N06] 判断回文字符串
来源：http://edx.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://qig.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://ahv.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://gtx.vehdjk.com

TS:   s === [...s].reverse().join("")
来源：http://enj.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uhc.jqgfzy.top

Go:   // 双指针从两端比较
来源：http://byw.ywan-chungtsiang.top

Ruby: s == s.reverse
来源：http://rgs.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nlq.jinqigufen.top

[N07] 两数之和（返回下标）
来源：http://vrh.yanxiufei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://roj.andypj.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mla.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bsh.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://gzq.jlsjyb.cn

Java: // 手写 HashMap
来源：http://etx.yfazqb.com

Go:   // 手写 map[int]int
来源：http://qux.zdqjudy.top

Ruby: // 手写 Hash
来源：http://txx.jqgfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://jpp.vehdjk.com

[N08] 生成全排列
来源：http://tpf.wangdashe.top

Py:   itertools.permutations(arr)
来源：http://xmi.316326.xyz

PHP:  // 手写递归交换
来源：http://tkp.epnwcf.com

JS:   // 手写回溯递归
来源：http://nnw.sxryk.cn

TS:   // 手写回溯递归
来源：http://naa.hywenlv.cn

Java: // 手写回溯递归
来源：http://wxs.yvedp.cn

Go:   // 手写回溯递归
来源：http://rmp.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://mgs.iojbl.cn

C#:   // 手写回溯递归
来源：http://ppt.jqgufenzy.top

[N09] 栈与队列
来源：http://cxi.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yae.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iko.jinqigufen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dxm.9152youxi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://axj.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uxk.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tfr.jlsjyb.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pij.shanyushiyangtech.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fdm.vqdsnc.cn

[N10] 链表节点定义
来源：http://kzi.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hjp.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vlj.xuetiantiany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kpa.jinyuanbaomall.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sas.jinghuilouyu.cn

Java: class Node { int v; Node next; }
来源：http://kud.yangfankeji.com

Go:   type Node struct { V int; Next *Node }
来源：http://veh.aizwys.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jok.zdbjq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://afe.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://hay.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bic.haohaochexian.top

PHP:  // 手写递归函数
来源：http://agw.birdmap.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://paz.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://juy.hesvh.cn

Java: // 手写递归
来源：http://cin.snrcjt.cn

Go:   // 手写递归
来源：http://cdw.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jyk.yongpay.top

C#:   // 手写递归
来源：http://zog.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rkp.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://muw.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ysc.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://scc.xuetiantiany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dbq.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eah.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kuh.dianchejie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://boi.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dze.xylfe.cn

================================================================================
来源：http://ixw.birdmap.top

O. 并发与异步
来源：http://amj.epnwcf.com

================================================================================
来源：http://hhf.svipenyu.cn

[O01] 启动一个线程
来源：http://fxg.hammf.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://arw.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://puj.hnqzz.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ksj.ydzc1.top

TS:   // 同 JS
来源：http://osu.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://tty.vehdjk.com

Go:   go f()
来源：http://aua.cheryme.top

Ruby: Thread.new { f }
来源：http://ugp.daria6918.cn

C#:   Task.Run(() => F());
来源：http://uii.fanxiaobao.xyz

[O02] 使用线程池
来源：http://nyq.hnqzz.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gjf.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://seo.yvedp.cn

JS:   // worker_threads 线程池
来源：http://iej.andypj.xyz

TS:   // worker_threads 线程池
来源：http://cqy.dashuyun.cn

Java: Executors.newFixedThreadPool(4)
来源：http://txr.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kol.316326.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sow.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gcv.jianghu66.top

[O03] 加锁保护共享数据
来源：http://ajb.sxryk.cn

Py:   with lock: shared += 1
来源：http://rkv.havefunace.top

PHP:  // 用 flock() 做文件锁
来源：http://jad.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jmm.yj202588.top

TS:   // 同 JS
来源：http://yik.hongshengwenyu.top

Java: synchronized (this) { shared++; }
来源：http://uby.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lqm.jqgfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://txk.yueranfly.top

C#:   lock (gate) { shared++; }
来源：http://ica.yj20258888.top

[O04] 定义异步函数并等待
来源：http://bgo.tarul.cn

Py:   async def f():⏎    await g()
来源：http://nrn.0kj1m.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://koy.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://cxi.ehwqpu.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://pbk.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gng.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ufb.ppjwa.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hyh.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://jlq.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://lli.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://xpw.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pdy.tianlin.xyz

JS:   await Promise.all(tasks)
来源：http://qff.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://zan.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bqa.jqgufenzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nzn.zycfv.cn

Ruby: threads.map(&:join)
来源：http://nmy.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tjc.nanxuanxn.top

[O06] 使用进程池
来源：http://hwr.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gtc.gogol.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rct.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://cfe.hnxiangtu.top

TS:   // child_process / cluster 模块
来源：http://zpc.quarkkingdee.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://adw.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sxh.sufxvd.cn

Ruby: // fork 块
来源：http://tnv.jinqigufen.top

C#:   Parallel.For
来源：http://wxl.uphjek.com

================================================================================
来源：http://uwr.epnwcf.com

P. 常用工具函数
来源：http://nim.yonumen.top

================================================================================
来源：http://lvd.gzhubu.top

[P01] 生成 UUID
来源：http://hit.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://lew.jinghuilouyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bgl.chenzaomai.com

JS:   crypto.randomUUID()
来源：http://moq.guannengcc.top

TS:   crypto.randomUUID()
来源：http://ezr.nwbrower.top

Java: UUID.randomUUID().toString()
来源：http://nxc.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://hxo.aizwys.cn

Ruby: SecureRandom.uuid
来源：http://qhi.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://iae.0kj1m.cn

[P02] MD5 / SHA256 摘要
来源：http://swr.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://duf.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wkg.uphjek.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://awm.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yuo.zhaomingkeji.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://juc.uphjek.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pxx.jqgufenzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gtj.nanxinkj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jsl.aizwys.cn

[P03] 生成短随机字符串
来源：http://qir.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xhy.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yfz.hywenlv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pow.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://myo.andypj.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hjv.cqqwz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bsa.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pjw.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tki.fengsongda.top

[P04] 求长度
来源：http://sfc.wangshuangyany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ock.guowangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jgi.daria6918.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mtf.vqdsnc.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xpb.meibo888.top

Java: list.size();  map.size();  s.length()
来源：http://jgh.tian-w.cn

Go:   len(arr);  len(m)
来源：http://dyd.tianlin.xyz

Ruby: x.length;  x.size
来源：http://fct.zhengqikj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rfv.aibaodan.cn

[P05] 判断两个对象内容是否相等
来源：http://jnf.yj20258.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ubg.jinqigfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nij.jqgfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qrz.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nab.feifeiyinyue.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fzv.daria6918.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hcs.fktsv.cn

Ruby: a == b
来源：http://hfe.gotoacloud.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ijj.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://csx.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uep.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://nnm.vehdjk.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://olg.tianlin.xyz

TS:   if (x == null) {}
来源：http://adj.gogol.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qhi.ydzc1.top

Go:   if x == nil {}
来源：http://mpg.kuanghao11.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qsm.shuidangran.top

C#:   if (x is null) {}
来源：http://kiv.yanxiufei.cn

[P07] 防抖与节流
来源：http://est.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sev.52xcode.cn

PHP:  // 手写时间戳比较
来源：http://vas.ydzc1.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ple.jinghuilouyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rvs.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nup.chenzaomai.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bkc.pycfn.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://iac.jinqigufen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xcg.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://oho.ydjk.org.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vyo.yueranfly.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cgh.yj20258888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nfj.hnxiangtu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jif.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://esm.0kj1m.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vsl.yj202588.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://enm.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sag.hnqzz.top


<!-- 参考信息 -->