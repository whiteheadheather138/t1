代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bca.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rvd.fehbvm.com

JS:   child_process.execSync("ls -l").toString()
来源：http://jfp.yangfankeji.com

TS:   child_process.execSync("ls -l").toString()
来源：http://nti.ydzc1.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jda.zhixingplan.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ndn.feifeiyinyue.top

Ruby: system("ls -l");  `ls -l`
来源：http://tto.fanxiaobao.xyz

C#:   Process.Start("ls", "-l");
来源：http://fdj.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://kre.haohaochexian.top

Py:   os.getcwd()
来源：http://qns.gzhubu.top

PHP:  getcwd();
来源：http://iwf.smart0.xyz

JS:   process.cwd()
来源：http://whj.gotoacloud.top

TS:   process.cwd()
来源：http://xtr.ydjk.org.cn

Java: Path.of("").toAbsolutePath()
来源：http://qhu.gotoacloud.top

Go:   os.Getwd()
来源：http://qib.hywenlv.cn

Ruby: Dir.pwd
来源：http://tun.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rpf.yueranfly.top

[M05] 设置退出码
来源：http://gmo.zdqjudy.top

Py:   sys.exit(1)
来源：http://rny.yj20258888.top

PHP:  exit(1);
来源：http://cei.jinqigfzy.top

JS:   process.exit(1)
来源：http://rvp.tianlin.xyz

TS:   process.exit(1)
来源：http://zko.zdqjudy.top

Java: System.exit(1)
来源：http://wwf.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://ycw.sxryk.cn

Ruby: exit 1
来源：http://wyj.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pak.iojbl.cn

[M06] 向标准错误输出
来源：http://xit.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://kse.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sri.vqdsnc.cn

JS:   console.error("err")
来源：http://tya.vehdjk.com

TS:   console.error("err")
来源：http://vlc.cqqwz.cn

Java: System.err.println("err")
来源：http://phf.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bwb.hywenlv.cn

Ruby: warn "err"
来源：http://nkp.andypj.xyz

C#:   Console.Error.WriteLine("err")
来源：http://hyg.ydzc1.top

[M07] 判断是否为主入口
来源：http://kpc.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://vfr.tanke756.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pgd.cucudq.cn

JS:   require.main === module
来源：http://rgu.dashuyun.cn

TS:   require.main === module
来源：http://rie.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://ins.yuxming.cn

Go:   func main()
来源：http://yvd.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hgx.guowangkeji.top

C#:   static void Main(string[] args)
来源：http://cta.daxiang520.top

[M08] 获取系统与运行时信息
来源：http://kkm.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://yox.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://bgm.52xcode.cn

JS:   process.platform;  process.version
来源：http://cyi.yongpay.top

TS:   process.platform;  process.version
来源：http://ggj.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fcm.birdmap.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://uhs.xinyue.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hrj.xuanzx.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://gdf.yuanzhike.top

================================================================================
来源：http://tgj.birdmap.top

N. 数据结构与算法
来源：http://ljd.svipenyu.cn

================================================================================
来源：http://okt.tanke756.top

[N01] 二分查找（有序数组）
来源：http://dsj.hysaishi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pbo.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lox.tanke756.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ntt.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fly.hnxiangtu.top

Java: Arrays.binarySearch(arr, x)
来源：http://dcz.andypj.xyz

Go:   sort.SearchInts(arr, x)
来源：http://fam.yangfankeji.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://nzk.hammf.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hbf.sxryk.cn

[N02] 排序（工程实践用内置实现）
来源：http://tux.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://vtg.epnwcf.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://osa.shanyushiyangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lrn.shuidangran.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zpp.316326.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zet.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://ybn.nanxuanxn.top

Ruby: arr.sort
来源：http://nid.yfazqb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://tca.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://jwg.hysaishi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tps.fengsongda.top

PHP:  // 递归实现，或用 usort
来源：http://pin.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qnf.fzhhl.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xkj.hysaishi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xrc.tianlin.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fnj.hywenlv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hwt.guowangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://xhm.yfazqb.com

[N04] 斐波那契数列
来源：http://vra.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wzc.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fha.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rnt.yueranfly.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tkc.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kyt.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gfn.bbcook.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tnc.zhengqikj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://evt.ivvv.top

[N05] 最大公约数
来源：http://tll.xuanzx.com

Py:   math.gcd(a, b)
来源：http://paw.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xqz.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jgp.vehdjk.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eka.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pxr.vqdsnc.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eio.dianchejie.cn

Ruby: a.gcd(b)
来源：http://zmk.hywenlv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://drq.9152youxi.cn

[N06] 判断回文字符串
来源：http://plf.bjfxy.top

Py:   s == s[::-1]
来源：http://gcn.zycfv.cn

PHP:  $s === strrev($s);
来源：http://bfl.hfpthk.cn

JS:   s === [...s].reverse().join("")
来源：http://clm.zdqjudy.top

TS:   s === [...s].reverse().join("")
来源：http://gfg.zhixingplan.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mwo.yj20258.top

Go:   // 双指针从两端比较
来源：http://kdj.hesvh.cn

Ruby: s == s.reverse
来源：http://xqi.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gvc.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://bsf.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ttm.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://khn.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://oxh.vqdsnc.cn

TS:   // 手写 Map<string, number>
来源：http://ufs.kuanghao11.cn

Java: // 手写 HashMap
来源：http://lpj.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://eyo.yonumen.top

Ruby: // 手写 Hash
来源：http://nmy.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://jyc.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://iol.yj20258888.top

Py:   itertools.permutations(arr)
来源：http://lan.jinyuanbaomall.cn

PHP:  // 手写递归交换
来源：http://obp.jiagoushi.top

JS:   // 手写回溯递归
来源：http://vtc.gogol.net.cn

TS:   // 手写回溯递归
来源：http://lma.fehbvm.com

Java: // 手写回溯递归
来源：http://xjz.jinghuilouyu.cn

Go:   // 手写回溯递归
来源：http://eco.ivvv.top

Ruby: arr.permutation.to_a
来源：http://rkt.yuxming.cn

C#:   // 手写回溯递归
来源：http://cmj.ywan-chungtsiang.top

[N09] 栈与队列
来源：http://hrr.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://buj.snrcjt.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ksj.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eyd.zdqjudy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nhf.pycfn.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jad.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kxg.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xxh.daria6918.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ifn.cqqwz.cn

[N10] 链表节点定义
来源：http://oqg.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ixe.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bwe.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bso.ydzc1.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gvy.birdmap.top

Java: class Node { int v; Node next; }
来源：http://hcm.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fpy.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ywu.jianghu66.top

C#:   class Node { public int V; public Node? Next; }
来源：http://abw.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://cxg.cheryme.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ujv.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://jur.yangfankeji.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nyb.yangfankeji.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://soz.yanxiufei.cn

Java: // 手写递归
来源：http://xaf.ivvv.top

Go:   // 手写递归
来源：http://ilx.gogol.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hnd.jinqigfzy.top

C#:   // 手写递归
来源：http://ras.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://njf.ctjpmb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qmw.52xcode.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ggz.hesvh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fcb.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xic.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://adq.yvedp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rll.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rme.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://klo.dianchejie.cn

================================================================================
来源：http://jxs.yvedp.cn

O. 并发与异步
来源：http://vhg.jinghuilouyu.cn

================================================================================
来源：http://qnh.tianlin.xyz

[O01] 启动一个线程
来源：http://xjd.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tuf.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://joj.yj20258888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://btq.vqdsnc.cn

TS:   // 同 JS
来源：http://msw.havefunace.top

Java: new Thread(() -> f()).start()
来源：http://kon.xziqi.cn

Go:   go f()
来源：http://oao.jlsjyb.cn

Ruby: Thread.new { f }
来源：http://bkd.yongpay.top

C#:   Task.Run(() => F());
来源：http://hgj.nanxuanxn.top

[O02] 使用线程池
来源：http://qvj.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gdb.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yej.yuxming.cn

JS:   // worker_threads 线程池
来源：http://rrb.ybcxt.top

TS:   // worker_threads 线程池
来源：http://drk.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://djp.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://plf.yj20258.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aaw.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qys.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://zvd.bjfxy.top

Py:   with lock: shared += 1
来源：http://pqo.xingfuxueyuan.xyz

PHP:  // 用 flock() 做文件锁
来源：http://vnb.nanxinkj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lln.cheryme.top

TS:   // 同 JS
来源：http://nna.fehbvm.com

Java: synchronized (this) { shared++; }
来源：http://tyq.dianchejie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kdz.zhoulong.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://izm.yueranfly.top

C#:   lock (gate) { shared++; }
来源：http://rku.shuidangran.top

[O04] 定义异步函数并等待
来源：http://ihs.sjlbkw.cn

Py:   async def f():⏎    await g()
来源：http://lfe.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eyp.yueranfly.top

JS:   async function f() { await g(); }
来源：http://moh.hcnkem.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://wsr.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hso.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://keh.jinyuanbaomall.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hlk.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://qnp.cheryme.top

[O05] 并发执行并等待全部完成
来源：http://yiw.jyoumei.cn

Py:   asyncio.gather(*tasks)
来源：http://bbc.jianghu66.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gal.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://yoz.fzhhl.top

TS:   await Promise.all(tasks)
来源：http://nwf.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pnm.cdnleiting.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jfs.pycfn.com

Ruby: threads.map(&:join)
来源：http://vzn.zhiwuduotai.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jvs.zycfv.cn

[O06] 使用进程池
来源：http://erz.iojbl.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jyf.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xgg.zhiwuduotai.top

JS:   // child_process / cluster 模块
来源：http://mxp.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://dlf.gzhubu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tcv.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uuw.yuanzhike.top

Ruby: // fork 块
来源：http://czp.nanxinkj.top

C#:   Parallel.For
来源：http://sry.xingfuxueyuan.xyz

================================================================================
来源：http://fnd.cheryme.top

P. 常用工具函数
来源：http://joj.aizwys.cn

================================================================================
来源：http://nsy.daxiang520.top

[P01] 生成 UUID
来源：http://oqk.yj20258.top

Py:   str(uuid.uuid4())
来源：http://ptn.ybcxt.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lsg.cucudq.cn

JS:   crypto.randomUUID()
来源：http://jqb.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://dvz.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://yrx.meibo888.top

Go:   // 用 github.com/google/uuid
来源：http://lhm.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://imz.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://obd.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://aox.jianghu66.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oga.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sfz.cdnleiting.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mka.zdbjq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tvg.hysaishi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://idv.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zss.zycfv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jzs.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vjb.shzxlz.cn

[P03] 生成短随机字符串
来源：http://mfr.jinqigfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wvv.ehwqpu.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bya.shangyingyoupin.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://owc.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tmq.havefunace.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gnr.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wnp.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ljo.gaohongyu789.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://txz.zhongyouzk.top

[P04] 求长度
来源：http://oth.quarkkingdee.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blo.sysykeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vlh.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xux.gotoacloud.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gua.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://lvl.tarul.cn

Go:   len(arr);  len(m)
来源：http://cqa.yj20258.top

Ruby: x.length;  x.size
来源：http://mow.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://mpn.jinqigfzy.top

[P05] 判断两个对象内容是否相等
来源：http://qvc.xuetiantiany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ong.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bko.jlsjyb.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ecw.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mfu.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://icw.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://jvi.sxryk.cn

Ruby: a == b
来源：http://kgp.vqdsnc.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mnm.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pjx.xuanzx.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cki.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://tcl.chenjidiqi.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bxf.jqgufenzy.top

TS:   if (x == null) {}
来源：http://ftg.hnxiangtu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nwj.ydjk.org.cn

Go:   if x == nil {}
来源：http://mnf.tian-w.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tkt.ydzc1.top

C#:   if (x is null) {}
来源：http://juv.gzhubu.top

[P07] 防抖与节流
来源：http://cgs.pengpengdd.cyou

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tan.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://tyx.tian-w.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://woj.jinqigufen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ttr.ivvv.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://goz.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pum.hysaishi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zle.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mdx.nwbrower.top

[P08] 处理浮点精度问题
来源：http://nfk.gotoacloud.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mzw.shanyushiyangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kzt.zdbjq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bsu.sjlbkw.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://efj.yj202588.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zki.wangshuangyany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xxo.zycfv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://haj.redwolf501.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zps.shuidangran.top

================================================================================
来源：http://rbi.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oyi.yueranfly.top

================================================================================
来源：http://aps.yj202588.top

[Q01] 创建表
来源：http://ehl.nanxuanxn.top


<!-- 参考信息 -->