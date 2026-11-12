代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kvi.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tvt.c1oappe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nzn.jyoumei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://btf.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nrl.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://oao.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ehv.xingfuxueyuan.xyz

C#:   Process.Start("ls", "-l");
来源：http://sav.hammf.cn

[M04] 获取当前工作目录
来源：http://ldw.tanke756.top

Py:   os.getcwd()
来源：http://yfe.yonumen.top

PHP:  getcwd();
来源：http://twh.chenjidiqi.icu

JS:   process.cwd()
来源：http://vxy.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://lev.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://qbp.yangfankeji.com

Go:   os.Getwd()
来源：http://tdj.ivvv.top

Ruby: Dir.pwd
来源：http://uog.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://llm.bjfxy.top

[M05] 设置退出码
来源：http://nbk.ivvv.top

Py:   sys.exit(1)
来源：http://dir.smart0.xyz

PHP:  exit(1);
来源：http://drf.quarkkingdee.top

JS:   process.exit(1)
来源：http://npq.andypj.xyz

TS:   process.exit(1)
来源：http://vwd.xinyue.icu

Java: System.exit(1)
来源：http://ono.yueranfly.top

Go:   os.Exit(1)
来源：http://sgo.zhengqikj.top

Ruby: exit 1
来源：http://kgc.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zqe.jiagoushi.top

[M06] 向标准错误输出
来源：http://pua.vehdjk.com

Py:   print("err", file=sys.stderr)
来源：http://bei.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://dui.svipenyu.cn

JS:   console.error("err")
来源：http://ndt.nanxinkj.top

TS:   console.error("err")
来源：http://nzj.guowangkeji.top

Java: System.err.println("err")
来源：http://fkx.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yzw.jiagoushi.top

Ruby: warn "err"
来源：http://fro.guannengcc.top

C#:   Console.Error.WriteLine("err")
来源：http://raa.nanxinkj.top

[M07] 判断是否为主入口
来源：http://qks.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://ldl.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nat.jinqigufen.top

JS:   require.main === module
来源：http://jrf.cheryme.top

TS:   require.main === module
来源：http://tin.bjfxy.top

Java: public static void main(String[] args)
来源：http://eqy.yj20258.top

Go:   func main()
来源：http://znw.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ekj.yuanzhike.top

C#:   static void Main(string[] args)
来源：http://mcu.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://eqi.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://lqc.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://bul.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://yhn.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://zyv.nanxuanxn.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vdi.nanxinkj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rdb.jinghuilouyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lrn.bbcook.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rnf.zycfv.cn

================================================================================
来源：http://uzq.cqqwz.cn

N. 数据结构与算法
来源：http://dve.shuidangran.top

================================================================================
来源：http://cvw.jiagoushi.top

[N01] 二分查找（有序数组）
来源：http://tuf.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://stk.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xay.ybcxt.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jzm.hesvh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dpg.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vrh.jinghuilouyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://cof.xuetiantiany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://inp.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://svc.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://oqn.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://hmg.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://evd.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ceq.epnwcf.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://xaw.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tdk.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://rsm.quarkkingdee.top

Ruby: arr.sort
来源：http://jrq.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wza.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://nuk.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lip.havefunace.top

PHP:  // 递归实现，或用 usort
来源：http://hyp.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lyv.dashuyun.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dec.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://anw.zhijiandao.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kgs.tian-w.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zwg.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://vfy.ywan-chungtsiang.top

[N04] 斐波那契数列
来源：http://tny.daxiang520.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eba.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iwx.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ylp.bbcook.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cvt.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://key.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://osy.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fmz.jianghu66.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://etu.feifeiyinyue.top

[N05] 最大公约数
来源：http://nix.mhx1999.top

Py:   math.gcd(a, b)
来源：http://wkm.hesvh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bcd.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fcj.xuetiantiany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dvn.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gbx.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qsj.chenlongwang.top

Ruby: a.gcd(b)
来源：http://rlj.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hgw.hammf.cn

[N06] 判断回文字符串
来源：http://oaj.smart0.xyz

Py:   s == s[::-1]
来源：http://tho.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://yrx.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://hao.yongpay.top

TS:   s === [...s].reverse().join("")
来源：http://vhr.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jzd.jqgfzy.top

Go:   // 双指针从两端比较
来源：http://ghd.zycfv.cn

Ruby: s == s.reverse
来源：http://vwa.yangfankeji.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://axf.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://blr.hammf.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ktf.hammf.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rwn.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cnx.gogol.net.cn

TS:   // 手写 Map<string, number>
来源：http://tyu.yvedp.cn

Java: // 手写 HashMap
来源：http://bul.sysykeji.top

Go:   // 手写 map[int]int
来源：http://uqg.tian-w.cn

Ruby: // 手写 Hash
来源：http://fxy.cashguo.top

C#:   // 手写 Dictionary<int, int>
来源：http://rmc.chenjidiqi.icu

[N08] 生成全排列
来源：http://pen.zhaomingkeji.xyz

Py:   itertools.permutations(arr)
来源：http://jbc.ppjwa.cn

PHP:  // 手写递归交换
来源：http://xbz.52xcode.cn

JS:   // 手写回溯递归
来源：http://eod.yangfankeji.com

TS:   // 手写回溯递归
来源：http://web.kuanghao11.cn

Java: // 手写回溯递归
来源：http://vmg.nanxinkj.top

Go:   // 手写回溯递归
来源：http://usz.chenlongwang.top

Ruby: arr.permutation.to_a
来源：http://pbr.cqqwz.cn

C#:   // 手写回溯递归
来源：http://mlu.dashuyun.cn

[N09] 栈与队列
来源：http://rro.nanxuanxn.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jaw.ppjwa.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wnd.feifeiyinyue.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lfd.guowangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ngp.316326.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yog.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vts.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://etc.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mnp.yvedp.cn

[N10] 链表节点定义
来源：http://iig.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://okk.shuidangran.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mmz.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mcr.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ejw.ydzc1.top

Java: class Node { int v; Node next; }
来源：http://cya.kuanghao11.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dqv.hnxiangtu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nmt.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://azz.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://tsb.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nnq.xylfe.cn

PHP:  // 手写递归函数
来源：http://xdw.xinyue.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://waa.bbcook.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ooa.tarul.cn

Java: // 手写递归
来源：http://zte.vehdjk.com

Go:   // 手写递归
来源：http://ihg.daria6918.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bto.gaohongyu789.top

C#:   // 手写递归
来源：http://zbn.hongshengwenyu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qby.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ilh.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bwc.bjfxy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jhe.birdmap.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nsp.jinghuilouyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vho.yanxiufei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qsw.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sjo.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ghs.iojbl.cn

================================================================================
来源：http://spi.chenlongwang.top

O. 并发与异步
来源：http://kln.yueranfly.top

================================================================================
来源：http://zqz.jianghu66.top

[O01] 启动一个线程
来源：http://kaj.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fln.zhixingplan.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fpi.tanke756.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dob.dianchejie.cn

TS:   // 同 JS
来源：http://oll.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://tti.jinghuilouyu.cn

Go:   go f()
来源：http://ptk.hfpthk.cn

Ruby: Thread.new { f }
来源：http://lho.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://mzm.jinghuilouyu.cn

[O02] 使用线程池
来源：http://gbq.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jgz.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mcw.jyoumei.cn

JS:   // worker_threads 线程池
来源：http://znx.cdnleiting.top

TS:   // worker_threads 线程池
来源：http://bza.fengsongda.top

Java: Executors.newFixedThreadPool(4)
来源：http://jto.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qvq.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mjb.bjfxy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bsf.snrcjt.cn

[O03] 加锁保护共享数据
来源：http://tvz.fengsongda.top

Py:   with lock: shared += 1
来源：http://kvd.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://xel.jlsjyb.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qoc.cqqwz.cn

TS:   // 同 JS
来源：http://mfa.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://ubl.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rgp.jinqigfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://yzt.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://uim.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://otr.ppjwa.cn

Py:   async def f():⏎    await g()
来源：http://lox.aibaodan.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://evu.jlsjyb.cn

JS:   async function f() { await g(); }
来源：http://jte.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ueq.chenlongwang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iro.mhx1999.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dfb.cqqwz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://koo.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://wss.zhongyouzk.top

[O05] 并发执行并等待全部完成
来源：http://sdn.daria6918.cn

Py:   asyncio.gather(*tasks)
来源：http://ipb.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fgf.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://gst.hammf.cn

TS:   await Promise.all(tasks)
来源：http://uky.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xcs.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fwx.gzhubu.top

Ruby: threads.map(&:join)
来源：http://osv.vqdsnc.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dtt.jinghuilouyu.cn

[O06] 使用进程池
来源：http://eea.yuanzhike.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uvf.pengpengdd.cyou

PHP:  // pcntl_fork 或多进程队列
来源：http://sdf.xinyue.icu

JS:   // child_process / cluster 模块
来源：http://wcp.jiagoushi.top

TS:   // child_process / cluster 模块
来源：http://wya.cdnleiting.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gfe.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jhb.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://eho.kuanghao11.cn

C#:   Parallel.For
来源：http://jnr.fengsongda.top

================================================================================
来源：http://zhg.snrcjt.cn

P. 常用工具函数
来源：http://ohf.daria6918.cn

================================================================================
来源：http://mtg.fehbvm.com

[P01] 生成 UUID
来源：http://lma.feifeiyinyue.top

Py:   str(uuid.uuid4())
来源：http://zbz.ybcxt.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rkq.kuanghao11.cn

JS:   crypto.randomUUID()
来源：http://dcl.smart0.xyz

TS:   crypto.randomUUID()
来源：http://vea.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://rxy.shanyushiyangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://pup.yuxming.cn

Ruby: SecureRandom.uuid
来源：http://eqp.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://voe.jinyuanbaomall.cn

[P02] MD5 / SHA256 摘要
来源：http://ksw.fanxiaobao.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mhg.hfpthk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ezz.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xcg.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lyq.gzhubu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xrz.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mrt.sysykeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://csf.gaohongyu789.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://axx.jinyuanbaomall.cn

[P03] 生成短随机字符串
来源：http://ytx.dianchejie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pxn.yj20258888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wat.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ypl.havefunace.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qtr.chenzaomai.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ndm.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ziq.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://qqg.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dyv.zhongyouzk.top

[P04] 求长度
来源：http://wwq.ctjpmb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fch.ivvv.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kws.yonumen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://diy.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ukh.gotoacloud.top

Java: list.size();  map.size();  s.length()
来源：http://aox.xinyue.icu

Go:   len(arr);  len(m)
来源：http://nxy.xziqi.cn

Ruby: x.length;  x.size
来源：http://rzk.pengpengdd.cyou

C#:   list.Count;  dict.Count;  s.Length
来源：http://gxc.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://ogh.jqgufenzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://khr.pengpengdd.cyou

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lag.xuanzx.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ang.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://msj.zhongyouzk.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tww.shanyushiyangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://fjv.epnwcf.com

Ruby: a == b
来源：http://zkj.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vts.zdbjq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ftk.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ytf.chenzaomai.com

PHP:  if (empty($x)) {}
来源：http://qyd.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vxq.nanxuanxn.top

TS:   if (x == null) {}
来源：http://swk.wangshuangyany.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ajn.xingfuxueyuan.xyz

Go:   if x == nil {}
来源：http://inc.9152youxi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xsb.zhixingplan.top

C#:   if (x is null) {}
来源：http://ouz.fanxiaobao.xyz

[P07] 防抖与节流
来源：http://qys.wangdashe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oep.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://row.smart0.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wwy.xingfuxueyuan.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qlv.sjlbkw.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hfd.vehdjk.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rri.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mlz.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://grc.aizwys.cn

[P08] 处理浮点精度问题
来源：http://dpa.sxryk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rwg.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dxl.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hdi.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kgj.hcnkem.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://okl.quarkkingdee.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bbx.pycfn.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jyd.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://idi.ehwqpu.com

================================================================================
来源：http://xeb.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jpl.haohaochexian.top

================================================================================
来源：http://uad.aibaodan.cn

[Q01] 创建表
来源：http://hnd.ivvv.top


<!-- 参考信息 -->