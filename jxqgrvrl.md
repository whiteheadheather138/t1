代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://buh.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://wbz.cdnleiting.top

Ruby: system("ls -l");  `ls -l`
来源：http://evf.meibo888.top

C#:   Process.Start("ls", "-l");
来源：http://oso.jiagoushi.top

[M04] 获取当前工作目录
来源：http://tsv.gogol.net.cn

Py:   os.getcwd()
来源：http://jjw.cheryme.top

PHP:  getcwd();
来源：http://ymv.vqdsnc.cn

JS:   process.cwd()
来源：http://bzq.zhiwuduotai.top

TS:   process.cwd()
来源：http://xit.jinghuilouyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://iue.zhiwuduotai.top

Go:   os.Getwd()
来源：http://iqu.yonumen.top

Ruby: Dir.pwd
来源：http://kbg.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://ssg.sweek.top

[M05] 设置退出码
来源：http://bnw.yongpay.top

Py:   sys.exit(1)
来源：http://vhe.xylfe.cn

PHP:  exit(1);
来源：http://qig.kuanghao11.cn

JS:   process.exit(1)
来源：http://xsb.tarul.cn

TS:   process.exit(1)
来源：http://nhe.fanxiaobao.xyz

Java: System.exit(1)
来源：http://ubi.wangdashe.top

Go:   os.Exit(1)
来源：http://xai.yuxming.cn

Ruby: exit 1
来源：http://ypd.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bmj.chenzaomai.com

[M06] 向标准错误输出
来源：http://efj.xingfuxueyuan.xyz

Py:   print("err", file=sys.stderr)
来源：http://ioi.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fuk.shanyushiyangtech.top

JS:   console.error("err")
来源：http://kbo.yuxming.cn

TS:   console.error("err")
来源：http://ogh.zdbjq.cn

Java: System.err.println("err")
来源：http://kil.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pht.hongshengwenyu.top

Ruby: warn "err"
来源：http://dld.wangshuangyany.cn

C#:   Console.Error.WriteLine("err")
来源：http://kqt.sysykeji.top

[M07] 判断是否为主入口
来源：http://vpr.smart0.xyz

Py:   if __name__ == "__main__":
来源：http://bxc.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blp.zhongyouzk.top

JS:   require.main === module
来源：http://diz.9152youxi.cn

TS:   require.main === module
来源：http://qai.ppjwa.cn

Java: public static void main(String[] args)
来源：http://xkn.cucudq.cn

Go:   func main()
来源：http://evo.ydzc1.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lgb.jianghu66.top

C#:   static void Main(string[] args)
来源：http://smz.316326.xyz

[M08] 获取系统与运行时信息
来源：http://jbo.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://jwp.zhiwuduotai.top

PHP:  PHP_OS;  phpversion();
来源：http://ihg.gotoacloud.top

JS:   process.platform;  process.version
来源：http://ehe.zdbjq.cn

TS:   process.platform;  process.version
来源：http://kyb.cheryme.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ykj.xinyue.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://gbc.jqgfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fxg.jinqigfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gaa.fzhhl.top

================================================================================
来源：http://aol.cdnleiting.top

N. 数据结构与算法
来源：http://tim.sysykeji.top

================================================================================
来源：http://wtx.yuanzhike.top

[N01] 二分查找（有序数组）
来源：http://szu.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://ysu.xingfuxueyuan.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kbc.tianlin.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zfc.shuidangran.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fwa.bjfxy.top

Java: Arrays.binarySearch(arr, x)
来源：http://hrd.iojbl.cn

Go:   sort.SearchInts(arr, x)
来源：http://ekw.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bjh.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://uoi.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://xml.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://bnw.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jch.sjlbkw.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vko.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jir.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mdv.hcnkem.com

Go:   slices.Sort(arr)
来源：http://hpf.hcnkem.com

Ruby: arr.sort
来源：http://ood.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hno.yanxiufei.cn

[N03] 快速排序（分治示例）
来源：http://iyr.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tvm.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://tqj.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ato.zhijiandao.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tgt.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://agu.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lnh.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://whb.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rak.sweek.top

[N04] 斐波那契数列
来源：http://vzf.aibaodan.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://crx.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iza.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://isf.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ipz.aibaodan.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://byz.svipenyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xgg.tarul.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://his.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kyy.bbcook.cn

[N05] 最大公约数
来源：http://wxt.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://qpu.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tqy.sxryk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dqo.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ocf.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://puo.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://inm.iojbl.cn

Ruby: a.gcd(b)
来源：http://tmc.hnqzz.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bdx.hywenlv.cn

[N06] 判断回文字符串
来源：http://lwv.vehdjk.com

Py:   s == s[::-1]
来源：http://hjj.jlsjyb.cn

PHP:  $s === strrev($s);
来源：http://flu.havefunace.top

JS:   s === [...s].reverse().join("")
来源：http://nfe.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://ntv.smart0.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://efb.xziqi.cn

Go:   // 双指针从两端比较
来源：http://utq.52xcode.cn

Ruby: s == s.reverse
来源：http://jtz.gzhubu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lra.jianghu66.top

[N07] 两数之和（返回下标）
来源：http://chn.epnwcf.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cye.wangdashe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wce.mhx1999.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mll.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://xsz.yfazqb.com

Java: // 手写 HashMap
来源：http://vns.jlsjyb.cn

Go:   // 手写 map[int]int
来源：http://dpw.meibo888.top

Ruby: // 手写 Hash
来源：http://syd.pycfn.com

C#:   // 手写 Dictionary<int, int>
来源：http://zaz.zhongyouzk.top

[N08] 生成全排列
来源：http://tor.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://cpt.cucudq.cn

PHP:  // 手写递归交换
来源：http://wxy.xylfe.cn

JS:   // 手写回溯递归
来源：http://uzz.jqgfzy.top

TS:   // 手写回溯递归
来源：http://tqy.hysaishi.cn

Java: // 手写回溯递归
来源：http://oqa.haohaochexian.top

Go:   // 手写回溯递归
来源：http://rsg.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://qfq.yanxiufei.cn

C#:   // 手写回溯递归
来源：http://bmc.andypj.xyz

[N09] 栈与队列
来源：http://cpf.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://opc.sxryk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://aha.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://psq.fengsongda.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ojv.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://idc.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sxn.bjfxy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ldm.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lem.epnwcf.com

[N10] 链表节点定义
来源：http://mbe.fktsv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zss.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tqc.guannengcc.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dga.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ttc.pycfn.com

Java: class Node { int v; Node next; }
来源：http://rsa.kuanghao11.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ylu.shanyushiyangtech.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pps.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ugw.ywan-chungtsiang.top

[N11] 二叉树中序遍历
来源：http://xmj.316326.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nin.hywenlv.cn

PHP:  // 手写递归函数
来源：http://pkc.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vxp.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kvx.sufxvd.cn

Java: // 手写递归
来源：http://yim.jinqigufen.top

Go:   // 手写递归
来源：http://zbw.9152youxi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nqh.hfpthk.cn

C#:   // 手写递归
来源：http://nwv.xziqi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zwh.smart0.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://axk.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ppl.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kof.sweek.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yvx.fanxiaobao.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://idi.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qqy.feifeiyinyue.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cam.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://olq.yvedp.cn

================================================================================
来源：http://oaz.zhoulong.xyz

O. 并发与异步
来源：http://cit.xingfuxueyuan.xyz

================================================================================
来源：http://xzp.havefunace.top

[O01] 启动一个线程
来源：http://kot.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aqv.cheryme.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uzj.cucudq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nst.yj20258.top

TS:   // 同 JS
来源：http://vtl.shanyushiyangtech.top

Java: new Thread(() -> f()).start()
来源：http://kwj.birdmap.top

Go:   go f()
来源：http://icu.ehwqpu.com

Ruby: Thread.new { f }
来源：http://uao.fzhhl.top

C#:   Task.Run(() => F());
来源：http://pon.hysaishi.cn

[O02] 使用线程池
来源：http://mci.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fvb.cashguo.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nwv.jianghu66.top

JS:   // worker_threads 线程池
来源：http://xii.nanxuanxn.top

TS:   // worker_threads 线程池
来源：http://qll.nanxinkj.top

Java: Executors.newFixedThreadPool(4)
来源：http://vog.nwbrower.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cee.ydzc1.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uzx.birdmap.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uji.gotoacloud.top

[O03] 加锁保护共享数据
来源：http://vor.yueranfly.top

Py:   with lock: shared += 1
来源：http://uga.gotoacloud.top

PHP:  // 用 flock() 做文件锁
来源：http://arl.jinyuanbaomall.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vnx.cucudq.cn

TS:   // 同 JS
来源：http://zmi.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://fbz.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fve.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://olb.xziqi.cn

C#:   lock (gate) { shared++; }
来源：http://efy.iojbl.cn

[O04] 定义异步函数并等待
来源：http://nxp.cheryme.top

Py:   async def f():⏎    await g()
来源：http://bbx.jiagoushi.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ett.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://mwh.chenjidiqi.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://wbw.jyoumei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dar.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vqg.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://tga.cashguo.top

C#:   async Task F() { await G(); }
来源：http://nsy.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://usy.mhx1999.top

Py:   asyncio.gather(*tasks)
来源：http://auy.chenlongwang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ais.ybcxt.top

JS:   await Promise.all(tasks)
来源：http://uae.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://uzd.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tlh.dianchejie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hmq.cheryme.top

Ruby: threads.map(&:join)
来源：http://wic.nanxinkj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hfk.ybcxt.top

[O06] 使用进程池
来源：http://vzm.guowangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xvj.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://knx.guannengcc.top

JS:   // child_process / cluster 模块
来源：http://ubb.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://fjf.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vnj.zhongyouzk.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nab.xuanzx.com

Ruby: // fork 块
来源：http://lzm.nwbrower.top

C#:   Parallel.For
来源：http://pjr.hammf.cn

================================================================================
来源：http://pni.snrcjt.cn

P. 常用工具函数
来源：http://lki.jinqigufen.top

================================================================================
来源：http://jmb.aibaodan.cn

[P01] 生成 UUID
来源：http://rvk.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://ipl.kuanghao11.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rri.gaohongyu789.top

JS:   crypto.randomUUID()
来源：http://wzs.bbcook.cn

TS:   crypto.randomUUID()
来源：http://ypg.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://mac.xinyue.icu

Go:   // 用 github.com/google/uuid
来源：http://tgl.jiagoushi.top

Ruby: SecureRandom.uuid
来源：http://ztu.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://jnn.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://kmx.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zez.bbcook.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://evy.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hbb.xingfuxueyuan.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gbp.c1oappe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://faa.0kj1m.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zyn.yanxiufei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://psx.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bme.cucudq.cn

[P03] 生成短随机字符串
来源：http://hof.zdbjq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://smh.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pff.hcnkem.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blm.yanxiufei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oxv.ybcxt.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yzf.svipenyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dxb.fktsv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tqw.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bts.sysykeji.top

[P04] 求长度
来源：http://iwq.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xwc.gogol.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iyg.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sar.meibo888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tga.fktsv.cn

Java: list.size();  map.size();  s.length()
来源：http://rls.jianghu66.top

Go:   len(arr);  len(m)
来源：http://rvy.fehbvm.com

Ruby: x.length;  x.size
来源：http://haf.hywenlv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wky.dashuyun.cn

[P05] 判断两个对象内容是否相等
来源：http://dmb.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://uae.mhx1999.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xav.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://unx.hywenlv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://smv.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kuw.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://khg.9152youxi.cn

Ruby: a == b
来源：http://bbq.sufxvd.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yoi.pycfn.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://btp.sxryk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xlm.fktsv.cn

PHP:  if (empty($x)) {}
来源：http://ufk.jiagoushi.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://trg.jlsjyb.cn

TS:   if (x == null) {}
来源：http://sba.snrcjt.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gwt.316326.xyz

Go:   if x == nil {}
来源：http://smg.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pjd.zdqjudy.top

C#:   if (x is null) {}
来源：http://lgk.hcnkem.com

[P07] 防抖与节流
来源：http://hqp.redwolf501.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vyl.hammf.cn

PHP:  // 手写时间戳比较
来源：http://nmc.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nza.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mmb.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gcm.iojbl.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rkm.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jlm.ehwqpu.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xcn.fzhhl.top

[P08] 处理浮点精度问题
来源：http://lza.bjfxy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mjn.jinqigfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rwb.redwolf501.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zcr.daxiang520.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nuq.yj202588.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://obs.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qae.hcnkem.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xze.fanxiaobao.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ylx.hnxiangtu.top

================================================================================
来源：http://div.zhongyouzk.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eae.mhx1999.top

================================================================================
来源：http://lzc.nanxinkj.top

[Q01] 创建表
来源：http://iqf.yuxming.cn

CREATE TABLE users (
来源：http://rql.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iup.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://vga.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://wbw.gaohongyu789.top


<!-- 参考信息 -->