代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fht.guannengcc.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://irm.chenlongwang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zzx.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bah.meibo888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kjp.cucudq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zbo.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://kvp.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://hbb.fanxiaobao.xyz

[M04] 获取当前工作目录
来源：http://gfs.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://rts.c1oappe.top

PHP:  getcwd();
来源：http://cui.zhongyouzk.top

JS:   process.cwd()
来源：http://ikq.nanxuanxn.top

TS:   process.cwd()
来源：http://hfq.sweek.top

Java: Path.of("").toAbsolutePath()
来源：http://xet.0kj1m.cn

Go:   os.Getwd()
来源：http://fmz.jlsjyb.cn

Ruby: Dir.pwd
来源：http://qjq.0kj1m.cn

C#:   Directory.GetCurrentDirectory()
来源：http://taj.ehwqpu.com

[M05] 设置退出码
来源：http://uqv.sufxvd.cn

Py:   sys.exit(1)
来源：http://obq.c1oappe.top

PHP:  exit(1);
来源：http://dai.wangshuangyany.cn

JS:   process.exit(1)
来源：http://wtn.yanxiufei.cn

TS:   process.exit(1)
来源：http://roq.iojbl.cn

Java: System.exit(1)
来源：http://jev.tian-w.cn

Go:   os.Exit(1)
来源：http://kcw.fehbvm.com

Ruby: exit 1
来源：http://exx.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zwo.chenlongwang.top

[M06] 向标准错误输出
来源：http://hcg.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://rdi.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wxq.316326.xyz

JS:   console.error("err")
来源：http://gek.xinyue.icu

TS:   console.error("err")
来源：http://fpn.smart0.xyz

Java: System.err.println("err")
来源：http://aen.yuxming.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://els.aibaodan.cn

Ruby: warn "err"
来源：http://vuo.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://tgw.shuidangran.top

[M07] 判断是否为主入口
来源：http://mvd.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://kog.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hev.ydzc1.top

JS:   require.main === module
来源：http://vlz.mhx1999.top

TS:   require.main === module
来源：http://rkc.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://dtb.ivvv.top

Go:   func main()
来源：http://rkx.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fia.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://aii.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://emh.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://sax.daxiang520.top

PHP:  PHP_OS;  phpversion();
来源：http://qny.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://gfs.zdqjudy.top

TS:   process.platform;  process.version
来源：http://gid.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://adg.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://nuj.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hig.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mwf.cqqwz.cn

================================================================================
来源：http://ofs.zhixingplan.top

N. 数据结构与算法
来源：http://hzp.cashguo.top

================================================================================
来源：http://wlm.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://piz.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ita.jinyuanbaomall.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sbn.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://chb.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://obh.xuetiantiany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://llq.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://jfw.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://utw.hywenlv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dej.iojbl.cn

[N02] 排序（工程实践用内置实现）
来源：http://gpd.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://ovq.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tex.zhongyouzk.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://trh.zhongyouzk.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wlv.kuanghao11.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jzy.mhx1999.top

Go:   slices.Sort(arr)
来源：http://sbd.ppjwa.cn

Ruby: arr.sort
来源：http://acw.andypj.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://rgv.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://ttr.tanke756.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yol.yongpay.top

PHP:  // 递归实现，或用 usort
来源：http://gut.ppjwa.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ktt.jyoumei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tfa.guannengcc.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nji.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xhy.hysaishi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jxn.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://wth.jiagoushi.top

[N04] 斐波那契数列
来源：http://mbe.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aje.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ylk.bbcook.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iuq.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://epk.smart0.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iya.sweek.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eiv.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qds.tian-w.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xin.yuanzhike.top

[N05] 最大公约数
来源：http://iig.cashguo.top

Py:   math.gcd(a, b)
来源：http://cjz.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ire.hnqzz.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lxu.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dan.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ytz.svipenyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ipo.52xcode.cn

Ruby: a.gcd(b)
来源：http://uld.redwolf501.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wyi.ydzc1.top

[N06] 判断回文字符串
来源：http://wbi.shuidangran.top

Py:   s == s[::-1]
来源：http://pez.52xcode.cn

PHP:  $s === strrev($s);
来源：http://ycz.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://ovl.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://dat.zhiwuduotai.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bsn.0kj1m.cn

Go:   // 双指针从两端比较
来源：http://akg.zhoulong.xyz

Ruby: s == s.reverse
来源：http://mfc.havefunace.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mtz.pycfn.com

[N07] 两数之和（返回下标）
来源：http://xvz.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yeq.cqqwz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dbz.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mcp.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://wwi.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://iki.zhengqikj.top

Go:   // 手写 map[int]int
来源：http://xlf.uphjek.com

Ruby: // 手写 Hash
来源：http://kvq.zhongyouzk.top

C#:   // 手写 Dictionary<int, int>
来源：http://rpf.mhx1999.top

[N08] 生成全排列
来源：http://ead.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://rxp.yongpay.top

PHP:  // 手写递归交换
来源：http://dax.ppjwa.cn

JS:   // 手写回溯递归
来源：http://sck.jqgufenzy.top

TS:   // 手写回溯递归
来源：http://jzg.xingfuxueyuan.xyz

Java: // 手写回溯递归
来源：http://uyl.fehbvm.com

Go:   // 手写回溯递归
来源：http://vuy.yj202588.top

Ruby: arr.permutation.to_a
来源：http://bdi.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://fjn.svipenyu.cn

[N09] 栈与队列
来源：http://rdm.yueranfly.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bkj.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yeb.wangdashe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lnt.bjfxy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sjj.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uuy.xinyue.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mec.vqdsnc.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ciq.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fvv.sxryk.cn

[N10] 链表节点定义
来源：http://uij.fengsongda.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kzy.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sll.nanxinkj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nnk.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ifb.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://cvw.aibaodan.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sle.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kpr.fehbvm.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ckp.cqqwz.cn

[N11] 二叉树中序遍历
来源：http://xpc.0kj1m.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vgx.sxryk.cn

PHP:  // 手写递归函数
来源：http://ryj.zhixingplan.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pxn.meibo888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vvs.xuetiantiany.cn

Java: // 手写递归
来源：http://jeo.jinghuilouyu.cn

Go:   // 手写递归
来源：http://per.yangfankeji.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://stg.fktsv.cn

C#:   // 手写递归
来源：http://ppu.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fmt.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kno.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://idj.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wxx.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zut.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sgs.jianghu66.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blv.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qpl.hywenlv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jix.yuanzhike.top

================================================================================
来源：http://drr.fengsongda.top

O. 并发与异步
来源：http://fsj.zdbjq.cn

================================================================================
来源：http://nur.cashguo.top

[O01] 启动一个线程
来源：http://mba.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fct.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jkq.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dzo.sxryk.cn

TS:   // 同 JS
来源：http://djs.shzxlz.cn

Java: new Thread(() -> f()).start()
来源：http://ses.chenlongwang.top

Go:   go f()
来源：http://aei.birdmap.top

Ruby: Thread.new { f }
来源：http://exf.meibo888.top

C#:   Task.Run(() => F());
来源：http://hqd.ydjk.org.cn

[O02] 使用线程池
来源：http://bnz.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rpk.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zyq.snrcjt.cn

JS:   // worker_threads 线程池
来源：http://gzr.cdnleiting.top

TS:   // worker_threads 线程池
来源：http://tth.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://ezc.cheryme.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://spf.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cer.havefunace.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mil.sysykeji.top

[O03] 加锁保护共享数据
来源：http://wih.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://boh.gzhubu.top

PHP:  // 用 flock() 做文件锁
来源：http://mnj.birdmap.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tqg.zhengqikj.top

TS:   // 同 JS
来源：http://gbl.ppjwa.cn

Java: synchronized (this) { shared++; }
来源：http://fof.pengpengdd.cyou

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jrn.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://hsr.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://dvx.gaohongyu789.top

[O04] 定义异步函数并等待
来源：http://qbr.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://ony.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ihq.havefunace.top

JS:   async function f() { await g(); }
来源：http://djg.shanyushiyangtech.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tof.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eyq.snrcjt.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xth.tian-w.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mnx.tarul.cn

C#:   async Task F() { await G(); }
来源：http://okn.shangyingyoupin.top

[O05] 并发执行并等待全部完成
来源：http://inh.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://jeu.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://odd.yfazqb.com

JS:   await Promise.all(tasks)
来源：http://bpf.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://bmy.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kly.zdbjq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nie.gaohongyu789.top

Ruby: threads.map(&:join)
来源：http://src.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://eop.pengpengdd.cyou

[O06] 使用进程池
来源：http://nfb.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nlc.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mcs.sufxvd.cn

JS:   // child_process / cluster 模块
来源：http://tcp.wangdashe.top

TS:   // child_process / cluster 模块
来源：http://dld.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fuw.shuidangran.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oaz.zhiwuduotai.top

Ruby: // fork 块
来源：http://bty.wangdashe.top

C#:   Parallel.For
来源：http://yzd.nwbrower.top

================================================================================
来源：http://lhf.hywenlv.cn

P. 常用工具函数
来源：http://elm.zycfv.cn

================================================================================
来源：http://pku.svipenyu.cn

[P01] 生成 UUID
来源：http://vix.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://lkd.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ksr.daxiang520.top

JS:   crypto.randomUUID()
来源：http://tia.haohaochexian.top

TS:   crypto.randomUUID()
来源：http://ppk.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://jkv.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://yeg.yj202588.top

Ruby: SecureRandom.uuid
来源：http://vqt.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://ypu.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://nkn.zhijiandao.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xbf.pycfn.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://luj.zhaomingkeji.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bkt.316326.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bka.epnwcf.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bmq.zycfv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bgx.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ohn.dianchejie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rfz.smart0.xyz

[P03] 生成短随机字符串
来源：http://fhf.jqgfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://djc.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ons.hnqzz.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qdt.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zvi.meibo888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://els.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gpc.birdmap.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nsm.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dcv.yj20258888.top

[P04] 求长度
来源：http://aip.jinqigfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aut.yueranfly.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://itk.jianghu66.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rox.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://amx.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://gbx.yj202588.top

Go:   len(arr);  len(m)
来源：http://zap.ybcxt.top

Ruby: x.length;  x.size
来源：http://nga.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://evl.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://sqw.jiagoushi.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fzh.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ryr.shanyushiyangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lpn.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://afn.gogol.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sme.shzxlz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://isa.yuanzhike.top

Ruby: a == b
来源：http://lyp.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ukr.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fsm.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ftn.tian-w.cn

PHP:  if (empty($x)) {}
来源：http://alt.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rhi.zhijiandao.cn

TS:   if (x == null) {}
来源：http://rgs.jianghu66.top

Java: if (x == null || x.isEmpty()) {}
来源：http://awp.xziqi.cn

Go:   if x == nil {}
来源：http://nbv.yongpay.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zlo.wangdashe.top

C#:   if (x is null) {}
来源：http://cgi.ppjwa.cn

[P07] 防抖与节流
来源：http://ufn.feifeiyinyue.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lpj.zhoulong.xyz

PHP:  // 手写时间戳比较
来源：http://xxx.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mhf.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bkm.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oxe.cdnleiting.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dcl.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://unv.birdmap.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fji.gaohongyu789.top

[P08] 处理浮点精度问题
来源：http://yli.jiagoushi.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wsr.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://emr.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ped.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ejv.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qeg.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kjl.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://atg.wangshuangyany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zzr.sxryk.cn

================================================================================
来源：http://ksp.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mun.shanyushiyangkeji.top

================================================================================
来源：http://xga.zhoulong.xyz

[Q01] 创建表
来源：http://xjj.xylfe.cn


<!-- 参考信息 -->