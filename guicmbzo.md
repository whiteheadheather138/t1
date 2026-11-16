代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mzw.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mbp.fengsongda.top

Ruby: system("ls -l");  `ls -l`
来源：http://yia.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://nem.epnwcf.com

[M04] 获取当前工作目录
来源：http://rcj.zhengqikj.top

Py:   os.getcwd()
来源：http://lnh.ehwqpu.com

PHP:  getcwd();
来源：http://owl.havefunace.top

JS:   process.cwd()
来源：http://ahn.yj20258888.top

TS:   process.cwd()
来源：http://xyt.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://irb.zdbjq.cn

Go:   os.Getwd()
来源：http://rgs.jqgfzy.top

Ruby: Dir.pwd
来源：http://dtw.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pmo.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://cif.vqdsnc.cn

Py:   sys.exit(1)
来源：http://cnd.jqgfzy.top

PHP:  exit(1);
来源：http://jdu.zycfv.cn

JS:   process.exit(1)
来源：http://pck.shanyushiyangkeji.top

TS:   process.exit(1)
来源：http://nvn.dashuyun.cn

Java: System.exit(1)
来源：http://gnt.yongpay.top

Go:   os.Exit(1)
来源：http://fnq.meibo888.top

Ruby: exit 1
来源：http://vvw.jinyuanbaomall.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gyt.xziqi.cn

[M06] 向标准错误输出
来源：http://glt.iojbl.cn

Py:   print("err", file=sys.stderr)
来源：http://giy.zhixingplan.top

PHP:  fwrite(STDERR, "err\n");
来源：http://abv.zdqjudy.top

JS:   console.error("err")
来源：http://svp.wangdashe.top

TS:   console.error("err")
来源：http://aoa.haohaochexian.top

Java: System.err.println("err")
来源：http://xbu.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://exx.feifeiyinyue.top

Ruby: warn "err"
来源：http://mak.cqqwz.cn

C#:   Console.Error.WriteLine("err")
来源：http://gbp.ywan-chungtsiang.top

[M07] 判断是否为主入口
来源：http://odz.shzxlz.cn

Py:   if __name__ == "__main__":
来源：http://zqk.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ofq.xuanzx.com

JS:   require.main === module
来源：http://sax.andypj.xyz

TS:   require.main === module
来源：http://bvq.fehbvm.com

Java: public static void main(String[] args)
来源：http://kmw.ywan-chungtsiang.top

Go:   func main()
来源：http://qgd.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jhb.yj20258.top

C#:   static void Main(string[] args)
来源：http://jog.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://tva.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://dzr.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://gjo.sysykeji.top

JS:   process.platform;  process.version
来源：http://ctv.snrcjt.cn

TS:   process.platform;  process.version
来源：http://bvg.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://caw.fengsongda.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://grr.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jgq.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rng.jqgufenzy.top

================================================================================
来源：http://jts.aibaodan.cn

N. 数据结构与算法
来源：http://wcv.yonumen.top

================================================================================
来源：http://rrg.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://hph.jianghu66.top

Py:   bisect.bisect_left(arr, x)
来源：http://dfe.feifeiyinyue.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fdi.kuanghao11.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wfp.hnxiangtu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yeo.yangfankeji.com

Java: Arrays.binarySearch(arr, x)
来源：http://lpm.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://zxj.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://odc.xuetiantiany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zwt.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://zwx.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://fjv.zhaomingkeji.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jet.birdmap.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yrk.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://axd.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fko.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://boe.zdqjudy.top

Ruby: arr.sort
来源：http://aaw.tanke756.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://sxf.xuetiantiany.cn

[N03] 快速排序（分治示例）
来源：http://nnd.daria6918.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://psx.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://bek.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qwe.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://npk.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://guu.tianlin.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bkz.zhengqikj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wzy.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xis.shangyingyoupin.top

[N04] 斐波那契数列
来源：http://pht.zhoulong.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ntk.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kid.chenzaomai.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pqr.yj20258888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ggl.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hrm.ppjwa.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ewf.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://owc.wangshuangyany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://idu.vehdjk.com

[N05] 最大公约数
来源：http://fnb.sxryk.cn

Py:   math.gcd(a, b)
来源：http://vzj.daxiang520.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aav.feifeiyinyue.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://chf.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://avi.vqdsnc.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cgq.yongpay.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sqy.kuanghao11.cn

Ruby: a.gcd(b)
来源：http://kjx.chenzaomai.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xwr.kuanghao11.cn

[N06] 判断回文字符串
来源：http://rsq.xylfe.cn

Py:   s == s[::-1]
来源：http://zxz.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://pgg.cucudq.cn

JS:   s === [...s].reverse().join("")
来源：http://pqo.cucudq.cn

TS:   s === [...s].reverse().join("")
来源：http://ocv.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oqm.birdmap.top

Go:   // 双指针从两端比较
来源：http://hcz.bjfxy.top

Ruby: s == s.reverse
来源：http://ssb.shzxlz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jnh.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://jiv.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jhb.sjlbkw.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://upw.tianlin.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://gdu.sufxvd.cn

TS:   // 手写 Map<string, number>
来源：http://pjb.fktsv.cn

Java: // 手写 HashMap
来源：http://avp.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://hwd.ydzc1.top

Ruby: // 手写 Hash
来源：http://qdx.hnxiangtu.top

C#:   // 手写 Dictionary<int, int>
来源：http://hlx.tian-w.cn

[N08] 生成全排列
来源：http://tad.daxiang520.top

Py:   itertools.permutations(arr)
来源：http://jda.epnwcf.com

PHP:  // 手写递归交换
来源：http://afp.fehbvm.com

JS:   // 手写回溯递归
来源：http://klv.gaohongyu789.top

TS:   // 手写回溯递归
来源：http://lpd.xinyue.icu

Java: // 手写回溯递归
来源：http://uih.ywan-chungtsiang.top

Go:   // 手写回溯递归
来源：http://vad.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://klk.hongshengwenyu.top

C#:   // 手写回溯递归
来源：http://bez.tanke756.top

[N09] 栈与队列
来源：http://uhk.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ljq.zhixingplan.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qup.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://efm.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wri.aizwys.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qps.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hhe.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aob.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ciy.havefunace.top

[N10] 链表节点定义
来源：http://fvi.epnwcf.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zpo.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bwp.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kwg.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hdl.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://hor.yvedp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wzi.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uvv.cdnleiting.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jdt.cheryme.top

[N11] 二叉树中序遍历
来源：http://syd.zhiwuduotai.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uul.sjlbkw.cn

PHP:  // 手写递归函数
来源：http://jcz.chenzaomai.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://byg.hysaishi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lda.svipenyu.cn

Java: // 手写递归
来源：http://gty.jiagoushi.top

Go:   // 手写递归
来源：http://avo.fanxiaobao.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xst.hnqzz.top

C#:   // 手写递归
来源：http://hpb.yj20258888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vhc.fehbvm.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bul.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kfh.kuanghao11.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ijp.haohaochexian.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ote.cheryme.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tfi.ivvv.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bti.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bpn.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dug.cucudq.cn

================================================================================
来源：http://enx.hesvh.cn

O. 并发与异步
来源：http://fmo.xuanzx.com

================================================================================
来源：http://zne.shuidangran.top

[O01] 启动一个线程
来源：http://zyl.yj20258.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yly.smart0.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tbq.tianlin.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iwj.jinqigufen.top

TS:   // 同 JS
来源：http://phk.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://bjl.fengsongda.top

Go:   go f()
来源：http://emf.xziqi.cn

Ruby: Thread.new { f }
来源：http://wck.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://pkd.316326.xyz

[O02] 使用线程池
来源：http://gnz.meibo888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jaz.kuanghao11.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tmb.ybcxt.top

JS:   // worker_threads 线程池
来源：http://zae.sysykeji.top

TS:   // worker_threads 线程池
来源：http://xzw.andypj.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://dae.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uyn.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qda.haohaochexian.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nsk.uphjek.com

[O03] 加锁保护共享数据
来源：http://fqt.fanxiaobao.xyz

Py:   with lock: shared += 1
来源：http://ddb.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://sew.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vaf.ydjk.org.cn

TS:   // 同 JS
来源：http://ijz.xylfe.cn

Java: synchronized (this) { shared++; }
来源：http://cad.gogol.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zob.jqgufenzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nnw.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://lsu.xylfe.cn

[O04] 定义异步函数并等待
来源：http://dhn.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://lhj.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zvx.fktsv.cn

JS:   async function f() { await g(); }
来源：http://pcp.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://elg.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lob.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zlq.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ofl.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://tzp.zhongyouzk.top

[O05] 并发执行并等待全部完成
来源：http://tid.jqgufenzy.top

Py:   asyncio.gather(*tasks)
来源：http://ply.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sbk.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://dsk.dianchejie.cn

TS:   await Promise.all(tasks)
来源：http://pqj.ehwqpu.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://etc.cdnleiting.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yxr.chenlongwang.top

Ruby: threads.map(&:join)
来源：http://bby.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sxl.ywan-chungtsiang.top

[O06] 使用进程池
来源：http://xgc.dashuyun.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oyv.yueranfly.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wuh.0kj1m.cn

JS:   // child_process / cluster 模块
来源：http://wdb.316326.xyz

TS:   // child_process / cluster 模块
来源：http://jib.quarkkingdee.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rrc.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hdr.epnwcf.com

Ruby: // fork 块
来源：http://ywc.ivvv.top

C#:   Parallel.For
来源：http://wuj.c1oappe.top

================================================================================
来源：http://apy.hesvh.cn

P. 常用工具函数
来源：http://pfx.zhiwuduotai.top

================================================================================
来源：http://dsh.epnwcf.com

[P01] 生成 UUID
来源：http://mmw.snrcjt.cn

Py:   str(uuid.uuid4())
来源：http://eff.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ljp.cheryme.top

JS:   crypto.randomUUID()
来源：http://yky.jinqigufen.top

TS:   crypto.randomUUID()
来源：http://vco.quarkkingdee.top

Java: UUID.randomUUID().toString()
来源：http://lak.yj20258.top

Go:   // 用 github.com/google/uuid
来源：http://qnd.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://faj.shangyingyoupin.top

C#:   Guid.NewGuid().ToString()
来源：http://zwf.xuanzx.com

[P02] MD5 / SHA256 摘要
来源：http://ovo.jianghu66.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jwv.c1oappe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jjj.zhijiandao.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rwq.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yti.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vdm.zhongyouzk.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ryn.hnqzz.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://crg.hnxiangtu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lmq.hywenlv.cn

[P03] 生成短随机字符串
来源：http://iuy.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qup.cucudq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fkv.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nws.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://twc.hnxiangtu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://afi.sjlbkw.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://din.cqqwz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bzh.yj20258888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zku.ydjk.org.cn

[P04] 求长度
来源：http://heb.nwbrower.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vzc.jinqigfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cjn.zycfv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wct.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dah.guannengcc.top

Java: list.size();  map.size();  s.length()
来源：http://mgx.sxryk.cn

Go:   len(arr);  len(m)
来源：http://lhg.aibaodan.cn

Ruby: x.length;  x.size
来源：http://aqw.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://adw.kuanghao11.cn

[P05] 判断两个对象内容是否相等
来源：http://tsv.yongpay.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ygl.zhixingplan.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pux.zycfv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nre.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xwd.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zxr.chenjidiqi.icu

Go:   reflect.DeepEqual(a, b)
来源：http://fet.ctjpmb.com

Ruby: a == b
来源：http://grc.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eus.jianghu66.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gdg.hnqzz.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dew.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://jhs.ybcxt.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kdv.daxiang520.top

TS:   if (x == null) {}
来源：http://vvb.iojbl.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uxc.aizwys.cn

Go:   if x == nil {}
来源：http://lds.zdqjudy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ygd.aizwys.cn

C#:   if (x is null) {}
来源：http://guc.epnwcf.com

[P07] 防抖与节流
来源：http://net.gogol.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bid.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://ivb.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bpe.cheryme.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bon.zhaomingkeji.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tls.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://row.sweek.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ruh.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ziy.xinyue.icu

[P08] 处理浮点精度问题
来源：http://xae.hysaishi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sib.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ldf.jlsjyb.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vkb.sjlbkw.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://viq.ivvv.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pkc.yvedp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eqd.jqgufenzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pip.fzhhl.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bmo.jqgufenzy.top

================================================================================
来源：http://jbp.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tpt.aizwys.cn

================================================================================
来源：http://ggp.yj202588.top

[Q01] 创建表
来源：http://jiu.aibaodan.cn

CREATE TABLE users (
来源：http://wab.yongpay.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xqv.andypj.xyz

name VARCHAR(50) NOT NULL,
来源：http://bol.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://smq.chenlongwang.top


<!-- 参考信息 -->