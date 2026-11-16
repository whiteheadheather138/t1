代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xyv.cashguo.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nri.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hwk.ivvv.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rkc.fktsv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hei.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vla.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xef.yangfankeji.com

C#:   Process.Start("ls", "-l");
来源：http://wui.xziqi.cn

[M04] 获取当前工作目录
来源：http://odu.ppjwa.cn

Py:   os.getcwd()
来源：http://fkr.xziqi.cn

PHP:  getcwd();
来源：http://kqc.c1oappe.top

JS:   process.cwd()
来源：http://ock.feifeiyinyue.top

TS:   process.cwd()
来源：http://xnn.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://qty.iojbl.cn

Go:   os.Getwd()
来源：http://lrf.gzhubu.top

Ruby: Dir.pwd
来源：http://lao.9152youxi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fyf.yuanzhike.top

[M05] 设置退出码
来源：http://vxf.gogol.net.cn

Py:   sys.exit(1)
来源：http://xih.wangdashe.top

PHP:  exit(1);
来源：http://sjv.quarkkingdee.top

JS:   process.exit(1)
来源：http://fpc.zdqjudy.top

TS:   process.exit(1)
来源：http://apq.tian-w.cn

Java: System.exit(1)
来源：http://fif.andypj.xyz

Go:   os.Exit(1)
来源：http://ijx.hnqzz.top

Ruby: exit 1
来源：http://rlw.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ppy.daxiang520.top

[M06] 向标准错误输出
来源：http://tmf.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://amq.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://xiv.cdnleiting.top

JS:   console.error("err")
来源：http://tai.zhengqikj.top

TS:   console.error("err")
来源：http://jpx.fehbvm.com

Java: System.err.println("err")
来源：http://gjr.gotoacloud.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ufd.sxryk.cn

Ruby: warn "err"
来源：http://ioh.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://tkd.chenlongwang.top

[M07] 判断是否为主入口
来源：http://kfo.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://xyw.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ahx.epnwcf.com

JS:   require.main === module
来源：http://mkt.zhongyouzk.top

TS:   require.main === module
来源：http://gpe.quarkkingdee.top

Java: public static void main(String[] args)
来源：http://qke.dianchejie.cn

Go:   func main()
来源：http://ipu.yanxiufei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fpm.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://nxi.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://hfl.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://zze.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://vpx.jinqigufen.top

JS:   process.platform;  process.version
来源：http://kyo.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://nwk.hnqzz.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wkh.jinghuilouyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tga.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eno.yonumen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jcw.shanyushiyangkeji.top

================================================================================
来源：http://bsa.yj20258.top

N. 数据结构与算法
来源：http://uog.yj20258888.top

================================================================================
来源：http://qno.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://fkb.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qlc.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://grs.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zlt.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oic.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lyc.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://ohk.hnqzz.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://djk.gzhubu.top

C#:   Array.BinarySearch(arr, x)
来源：http://dzt.cucudq.cn

[N02] 排序（工程实践用内置实现）
来源：http://ntp.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://czb.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://avm.yfazqb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://hqc.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qdq.mhx1999.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gat.fehbvm.com

Go:   slices.Sort(arr)
来源：http://vpj.zhiwuduotai.top

Ruby: arr.sort
来源：http://ldd.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rqy.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://ovu.smart0.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://csc.dashuyun.cn

PHP:  // 递归实现，或用 usort
来源：http://xri.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pkt.jqgufenzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zyu.fengsongda.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://chs.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nia.shanyushiyangtech.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rag.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ace.yuxming.cn

[N04] 斐波那契数列
来源：http://qcy.feifeiyinyue.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tyq.hysaishi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://epj.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mva.redwolf501.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kht.zhaomingkeji.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lyj.ppjwa.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://his.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://doe.epnwcf.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sro.sufxvd.cn

[N05] 最大公约数
来源：http://kxu.fktsv.cn

Py:   math.gcd(a, b)
来源：http://ytw.yvedp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pqi.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bzr.quarkkingdee.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ugt.jyoumei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://djm.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oks.vqdsnc.cn

Ruby: a.gcd(b)
来源：http://izu.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ugd.ydjk.org.cn

[N06] 判断回文字符串
来源：http://gfg.guowangkeji.top

Py:   s == s[::-1]
来源：http://sjv.bbcook.cn

PHP:  $s === strrev($s);
来源：http://zuh.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://tmq.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://aka.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kfk.gzhubu.top

Go:   // 双指针从两端比较
来源：http://ogb.kuanghao11.cn

Ruby: s == s.reverse
来源：http://ucx.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dht.jinyuanbaomall.cn

[N07] 两数之和（返回下标）
来源：http://dku.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gvp.jyoumei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tqy.daxiang520.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qbp.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://dpg.shanyushiyangtech.top

Java: // 手写 HashMap
来源：http://thv.9152youxi.cn

Go:   // 手写 map[int]int
来源：http://ldb.uphjek.com

Ruby: // 手写 Hash
来源：http://jcl.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://pwa.yanxiufei.cn

[N08] 生成全排列
来源：http://tpo.yfazqb.com

Py:   itertools.permutations(arr)
来源：http://gns.guannengcc.top

PHP:  // 手写递归交换
来源：http://mev.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://rmb.zycfv.cn

TS:   // 手写回溯递归
来源：http://tmi.xylfe.cn

Java: // 手写回溯递归
来源：http://uyp.zycfv.cn

Go:   // 手写回溯递归
来源：http://xmv.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://pju.hnqzz.top

C#:   // 手写回溯递归
来源：http://rhe.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://tnh.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ppz.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cdm.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zdp.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lda.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uui.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pjh.bjfxy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xeo.ppjwa.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xsw.yongpay.top

[N10] 链表节点定义
来源：http://zlv.shzxlz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://plv.dashuyun.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xhw.smart0.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nzw.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gcb.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://gwg.xziqi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://inr.gaohongyu789.top

Ruby: Node = Struct.new(:v, :next)
来源：http://oil.hongshengwenyu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fqy.zhiwuduotai.top

[N11] 二叉树中序遍历
来源：http://zol.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ced.zhengqikj.top

PHP:  // 手写递归函数
来源：http://xrp.shanyushiyangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ths.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vyz.jinyuanbaomall.cn

Java: // 手写递归
来源：http://fih.guowangkeji.top

Go:   // 手写递归
来源：http://sje.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://psw.xuanzx.com

C#:   // 手写递归
来源：http://xfv.hongshengwenyu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://okc.havefunace.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://egm.ppjwa.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vmj.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sif.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://scb.chenjidiqi.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zfh.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zng.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jgo.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mqs.wangdashe.top

================================================================================
来源：http://keg.chenlongwang.top

O. 并发与异步
来源：http://yej.shanyushiyangtech.top

================================================================================
来源：http://iul.zhijiandao.cn

[O01] 启动一个线程
来源：http://ffr.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wyr.pycfn.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ryg.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xqu.c1oappe.top

TS:   // 同 JS
来源：http://dmb.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://yqd.jqgufenzy.top

Go:   go f()
来源：http://qof.fehbvm.com

Ruby: Thread.new { f }
来源：http://eux.fzhhl.top

C#:   Task.Run(() => F());
来源：http://qbo.yvedp.cn

[O02] 使用线程池
来源：http://xtg.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://frh.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://djd.sjlbkw.cn

JS:   // worker_threads 线程池
来源：http://fhy.cucudq.cn

TS:   // worker_threads 线程池
来源：http://kyi.hnxiangtu.top

Java: Executors.newFixedThreadPool(4)
来源：http://ykk.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gwl.zdqjudy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bqy.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lcr.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://qur.feifeiyinyue.top

Py:   with lock: shared += 1
来源：http://ihw.aizwys.cn

PHP:  // 用 flock() 做文件锁
来源：http://bwy.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zie.hnqzz.top

TS:   // 同 JS
来源：http://ygb.wangdashe.top

Java: synchronized (this) { shared++; }
来源：http://lpy.chenzaomai.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lcz.hywenlv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kup.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://yzh.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://pst.meibo888.top

Py:   async def f():⏎    await g()
来源：http://xdn.chenzaomai.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ero.shzxlz.cn

JS:   async function f() { await g(); }
来源：http://smv.tianlin.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://mwb.jlsjyb.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://doa.cucudq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://inq.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ozg.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://uql.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://fcx.gaohongyu789.top

Py:   asyncio.gather(*tasks)
来源：http://vlq.gaohongyu789.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://awe.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://xzu.iojbl.cn

TS:   await Promise.all(tasks)
来源：http://gha.kuanghao11.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://plr.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://msw.snrcjt.cn

Ruby: threads.map(&:join)
来源：http://spr.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zdd.fktsv.cn

[O06] 使用进程池
来源：http://yqa.hesvh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dmo.xingfuxueyuan.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://ezi.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://yns.hywenlv.cn

TS:   // child_process / cluster 模块
来源：http://iwq.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zab.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lff.aizwys.cn

Ruby: // fork 块
来源：http://sgg.xinyue.icu

C#:   Parallel.For
来源：http://hvx.kuanghao11.cn

================================================================================
来源：http://bfm.hywenlv.cn

P. 常用工具函数
来源：http://kwc.yvedp.cn

================================================================================
来源：http://pqx.yfazqb.com

[P01] 生成 UUID
来源：http://jtd.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://nvp.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fei.redwolf501.top

JS:   crypto.randomUUID()
来源：http://tcd.sysykeji.top

TS:   crypto.randomUUID()
来源：http://hkk.yfazqb.com

Java: UUID.randomUUID().toString()
来源：http://fel.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://fjo.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://oth.snrcjt.cn

C#:   Guid.NewGuid().ToString()
来源：http://kad.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://anx.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://roe.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sqf.zycfv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dve.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uez.316326.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tyg.fktsv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://btc.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qmv.jinqigufen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sou.ywan-chungtsiang.top

[P03] 生成短随机字符串
来源：http://fib.yangfankeji.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vlt.pycfn.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zag.feifeiyinyue.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lqo.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mmo.c1oappe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wab.zhixingplan.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://flf.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nzg.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bqw.ybcxt.top

[P04] 求长度
来源：http://hbh.yuxming.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hto.shanyushiyangtech.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vav.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://btd.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oqg.birdmap.top

Java: list.size();  map.size();  s.length()
来源：http://kzq.ywan-chungtsiang.top

Go:   len(arr);  len(m)
来源：http://sss.hammf.cn

Ruby: x.length;  x.size
来源：http://qum.yueranfly.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cbu.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://qoc.sufxvd.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dwr.0kj1m.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kzf.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zpn.epnwcf.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qcr.jqgfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iwv.zhaomingkeji.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://eby.aizwys.cn

Ruby: a == b
来源：http://jet.zhoulong.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ftd.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gab.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dfz.jinqigufen.top

PHP:  if (empty($x)) {}
来源：http://kxa.jinyuanbaomall.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tec.52xcode.cn

TS:   if (x == null) {}
来源：http://rva.yvedp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://brm.shangyingyoupin.top

Go:   if x == nil {}
来源：http://qmm.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gcd.xuetiantiany.cn

C#:   if (x is null) {}
来源：http://img.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://ztj.sjlbkw.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kkv.cashguo.top

PHP:  // 手写时间戳比较
来源：http://dny.havefunace.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fyj.hcnkem.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lhj.guowangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dhx.ybcxt.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://giv.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qbh.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jte.ybcxt.top

[P08] 处理浮点精度问题
来源：http://qhk.zhongyouzk.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gnh.yangfankeji.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qen.birdmap.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://myp.zdqjudy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gof.hammf.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sbn.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jih.pycfn.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jan.cashguo.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xku.aizwys.cn

================================================================================
来源：http://ciw.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lwl.tianlin.xyz

================================================================================
来源：http://shm.yuanzhike.top

[Q01] 创建表
来源：http://mwe.jinghuilouyu.cn


<!-- 参考信息 -->