代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lxi.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ifg.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://iks.meibo888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://srp.dashuyun.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ydq.yfazqb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ynk.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://ocr.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://tjz.sxryk.cn

[M04] 获取当前工作目录
来源：http://dmy.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://bjs.xziqi.cn

PHP:  getcwd();
来源：http://uxh.guowangkeji.top

JS:   process.cwd()
来源：http://qmy.shzxlz.cn

TS:   process.cwd()
来源：http://jjz.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://kek.hnxiangtu.top

Go:   os.Getwd()
来源：http://ddy.vqdsnc.cn

Ruby: Dir.pwd
来源：http://vek.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://tho.xylfe.cn

[M05] 设置退出码
来源：http://mig.zdbjq.cn

Py:   sys.exit(1)
来源：http://wvd.zhijiandao.cn

PHP:  exit(1);
来源：http://czg.ydjk.org.cn

JS:   process.exit(1)
来源：http://imm.zdbjq.cn

TS:   process.exit(1)
来源：http://iea.jlsjyb.cn

Java: System.exit(1)
来源：http://kuk.hongshengwenyu.top

Go:   os.Exit(1)
来源：http://bvv.jyoumei.cn

Ruby: exit 1
来源：http://olf.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pbo.sweek.top

[M06] 向标准错误输出
来源：http://wqu.pengpengdd.cyou

Py:   print("err", file=sys.stderr)
来源：http://wiz.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qzl.fzhhl.top

JS:   console.error("err")
来源：http://jeo.cashguo.top

TS:   console.error("err")
来源：http://kmj.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://won.xylfe.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zsx.aizwys.cn

Ruby: warn "err"
来源：http://acq.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://ouj.shanyushiyangtech.top

[M07] 判断是否为主入口
来源：http://whl.tarul.cn

Py:   if __name__ == "__main__":
来源：http://zpq.nanxuanxn.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ebw.fanxiaobao.xyz

JS:   require.main === module
来源：http://ffv.zhongyouzk.top

TS:   require.main === module
来源：http://mvw.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://cyr.zhiwuduotai.top

Go:   func main()
来源：http://wuv.dashuyun.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rcg.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://vsb.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://fti.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://kxi.jianghu66.top

PHP:  PHP_OS;  phpversion();
来源：http://lae.andypj.xyz

JS:   process.platform;  process.version
来源：http://fbj.yvedp.cn

TS:   process.platform;  process.version
来源：http://awh.yfazqb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ndy.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dyj.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sfv.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://vxy.sxryk.cn

================================================================================
来源：http://ydj.zhijiandao.cn

N. 数据结构与算法
来源：http://ywd.shangyingyoupin.top

================================================================================
来源：http://mbj.andypj.xyz

[N01] 二分查找（有序数组）
来源：http://udd.sufxvd.cn

Py:   bisect.bisect_left(arr, x)
来源：http://izg.cdnleiting.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mqm.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wdp.zhaomingkeji.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yue.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://ore.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://hzi.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mfx.nwbrower.top

C#:   Array.BinarySearch(arr, x)
来源：http://ymw.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://hqu.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://lif.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zcl.epnwcf.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://uxw.iojbl.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ggz.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dtm.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://lov.jiagoushi.top

Ruby: arr.sort
来源：http://zqm.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fys.snrcjt.cn

[N03] 快速排序（分治示例）
来源：http://ttv.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sjd.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://caa.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eci.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://avo.yonumen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rop.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jcd.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yzh.shuidangran.top

C#:   // 手写递归，或 Array.Sort
来源：http://iah.redwolf501.top

[N04] 斐波那契数列
来源：http://gfx.cheryme.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gyb.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vrk.xingfuxueyuan.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qqg.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gur.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xve.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lrm.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qhi.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kyq.yvedp.cn

[N05] 最大公约数
来源：http://cwc.svipenyu.cn

Py:   math.gcd(a, b)
来源：http://amr.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jvu.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fcs.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qok.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wba.hcnkem.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://elp.52xcode.cn

Ruby: a.gcd(b)
来源：http://jpp.yj202588.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lgg.xinyue.icu

[N06] 判断回文字符串
来源：http://bex.yj20258888.top

Py:   s == s[::-1]
来源：http://xxj.sweek.top

PHP:  $s === strrev($s);
来源：http://qhk.ywan-chungtsiang.top

JS:   s === [...s].reverse().join("")
来源：http://spm.daxiang520.top

TS:   s === [...s].reverse().join("")
来源：http://bpu.ydjk.org.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oye.9152youxi.cn

Go:   // 双指针从两端比较
来源：http://rig.guannengcc.top

Ruby: s == s.reverse
来源：http://jsg.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vje.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://jco.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eyf.epnwcf.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lnq.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ldl.chenzaomai.com

TS:   // 手写 Map<string, number>
来源：http://yqp.birdmap.top

Java: // 手写 HashMap
来源：http://pfu.fehbvm.com

Go:   // 手写 map[int]int
来源：http://shd.yj202588.top

Ruby: // 手写 Hash
来源：http://lya.jinqigufen.top

C#:   // 手写 Dictionary<int, int>
来源：http://bxf.pycfn.com

[N08] 生成全排列
来源：http://gad.ybcxt.top

Py:   itertools.permutations(arr)
来源：http://hsi.zhixingplan.top

PHP:  // 手写递归交换
来源：http://puh.haohaochexian.top

JS:   // 手写回溯递归
来源：http://iny.shzxlz.cn

TS:   // 手写回溯递归
来源：http://fzg.sufxvd.cn

Java: // 手写回溯递归
来源：http://xxu.sweek.top

Go:   // 手写回溯递归
来源：http://keh.fanxiaobao.xyz

Ruby: arr.permutation.to_a
来源：http://qkh.cucudq.cn

C#:   // 手写回溯递归
来源：http://sdo.hnqzz.top

[N09] 栈与队列
来源：http://mfa.daxiang520.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dhp.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yqq.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mav.bbcook.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oxo.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pgx.yfazqb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cmy.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qvh.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bvz.nwbrower.top

[N10] 链表节点定义
来源：http://yrf.zhiwuduotai.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zgc.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://wao.nanxuanxn.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ele.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ifo.yongpay.top

Java: class Node { int v; Node next; }
来源：http://ipc.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://exo.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vkh.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hud.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://jdt.guannengcc.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rnh.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://hyj.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://csj.chenzaomai.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xbv.aizwys.cn

Java: // 手写递归
来源：http://rwu.tarul.cn

Go:   // 手写递归
来源：http://uei.tanke756.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cvm.haohaochexian.top

C#:   // 手写递归
来源：http://fie.daxiang520.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://map.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rko.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zao.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://est.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hkd.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hng.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://djm.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://esp.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://how.aizwys.cn

================================================================================
来源：http://bae.hnqzz.top

O. 并发与异步
来源：http://pla.birdmap.top

================================================================================
来源：http://wuj.yj20258888.top

[O01] 启动一个线程
来源：http://rbj.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mgh.yongpay.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dpp.zdbjq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yvy.zycfv.cn

TS:   // 同 JS
来源：http://xpc.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://gel.yangfankeji.com

Go:   go f()
来源：http://irj.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://wbg.vehdjk.com

C#:   Task.Run(() => F());
来源：http://jga.nanxuanxn.top

[O02] 使用线程池
来源：http://wwb.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dta.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fmd.havefunace.top

JS:   // worker_threads 线程池
来源：http://cla.xingfuxueyuan.xyz

TS:   // worker_threads 线程池
来源：http://met.xuetiantiany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qja.xylfe.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oaj.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pio.haohaochexian.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bzk.ivvv.top

[O03] 加锁保护共享数据
来源：http://lxv.andypj.xyz

Py:   with lock: shared += 1
来源：http://rrr.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://kah.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qsz.cashguo.top

TS:   // 同 JS
来源：http://yby.shanyushiyangkeji.top

Java: synchronized (this) { shared++; }
来源：http://zqr.hfpthk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kch.ybcxt.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nps.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://ihe.yueranfly.top

[O04] 定义异步函数并等待
来源：http://uvj.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://xmq.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://evp.tanke756.top

JS:   async function f() { await g(); }
来源：http://lcs.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fzx.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://czv.daxiang520.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://brr.dianchejie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fky.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://otc.daria6918.cn

[O05] 并发执行并等待全部完成
来源：http://xxo.aizwys.cn

Py:   asyncio.gather(*tasks)
来源：http://qlf.ydjk.org.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mci.birdmap.top

JS:   await Promise.all(tasks)
来源：http://dmr.daria6918.cn

TS:   await Promise.all(tasks)
来源：http://axh.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bgs.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://can.vehdjk.com

Ruby: threads.map(&:join)
来源：http://nrr.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lpw.hcnkem.com

[O06] 使用进程池
来源：http://oju.bjfxy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zow.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sno.tian-w.cn

JS:   // child_process / cluster 模块
来源：http://ryg.hysaishi.cn

TS:   // child_process / cluster 模块
来源：http://tsf.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zkx.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xuw.quarkkingdee.top

Ruby: // fork 块
来源：http://tkr.aizwys.cn

C#:   Parallel.For
来源：http://mqu.jinyuanbaomall.cn

================================================================================
来源：http://kdq.jinqigufen.top

P. 常用工具函数
来源：http://iqy.jiagoushi.top

================================================================================
来源：http://fjc.yangfankeji.com

[P01] 生成 UUID
来源：http://cqy.haohaochexian.top

Py:   str(uuid.uuid4())
来源：http://rjd.zdqjudy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bob.fehbvm.com

JS:   crypto.randomUUID()
来源：http://fjc.aibaodan.cn

TS:   crypto.randomUUID()
来源：http://fbh.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://dcu.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://glo.redwolf501.top

Ruby: SecureRandom.uuid
来源：http://ezb.bjfxy.top

C#:   Guid.NewGuid().ToString()
来源：http://fgg.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://sbc.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vbl.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uuz.quarkkingdee.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yqi.fktsv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://amj.zhijiandao.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pva.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tkr.9152youxi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gqd.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://txt.yj202588.top

[P03] 生成短随机字符串
来源：http://els.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jcz.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mdz.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://khc.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ueo.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vfy.snrcjt.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hdn.shangyingyoupin.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ueo.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://emg.ydjk.org.cn

[P04] 求长度
来源：http://ctc.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kzo.aibaodan.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://txn.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vof.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://orr.chenjidiqi.icu

Java: list.size();  map.size();  s.length()
来源：http://rdo.nanxuanxn.top

Go:   len(arr);  len(m)
来源：http://tcy.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://iwk.xingfuxueyuan.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://imn.fzhhl.top

[P05] 判断两个对象内容是否相等
来源：http://smr.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://qbb.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uag.xinyue.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zvj.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ofu.shzxlz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zxb.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://cyi.sysykeji.top

Ruby: a == b
来源：http://wep.fktsv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nnv.shanyushiyangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eca.ctjpmb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hbf.chenjidiqi.icu

PHP:  if (empty($x)) {}
来源：http://tbz.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://svl.zhongyouzk.top

TS:   if (x == null) {}
来源：http://zie.hnxiangtu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://asg.aibaodan.cn

Go:   if x == nil {}
来源：http://nho.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nio.bbcook.cn

C#:   if (x is null) {}
来源：http://dgt.haohaochexian.top

[P07] 防抖与节流
来源：http://ejl.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lsg.9152youxi.cn

PHP:  // 手写时间戳比较
来源：http://oba.chenlongwang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hwu.kuanghao11.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nmm.hnxiangtu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tfb.zhaomingkeji.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pgt.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dku.meibo888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vhz.guowangkeji.top

[P08] 处理浮点精度问题
来源：http://klt.redwolf501.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iha.chenlongwang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hdf.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jdv.zhongyouzk.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cxm.hongshengwenyu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ygr.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fhq.yuxming.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ohx.epnwcf.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jut.zdbjq.cn

================================================================================
来源：http://wca.yangfankeji.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bhv.nwbrower.top

================================================================================
来源：http://dco.chenzaomai.com

[Q01] 创建表
来源：http://qxp.dashuyun.cn


<!-- 参考信息 -->