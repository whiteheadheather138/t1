代发 wailian999

[M04] 获取当前工作目录
来源：http://hye.xuetiantiany.cn

Py:   os.getcwd()
来源：http://mob.jqgfzy.top

PHP:  getcwd();
来源：http://blo.nanxinkj.top

JS:   process.cwd()
来源：http://pkg.daxiang520.top

TS:   process.cwd()
来源：http://hbf.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://muj.vqdsnc.cn

Go:   os.Getwd()
来源：http://asa.jlsjyb.cn

Ruby: Dir.pwd
来源：http://lol.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://mxz.birdmap.top

[M05] 设置退出码
来源：http://vzg.jiagoushi.top

Py:   sys.exit(1)
来源：http://iou.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://wom.hnxiangtu.top

JS:   process.exit(1)
来源：http://ujr.xylfe.cn

TS:   process.exit(1)
来源：http://ket.jinqigufen.top

Java: System.exit(1)
来源：http://psb.gzhubu.top

Go:   os.Exit(1)
来源：http://jlz.fktsv.cn

Ruby: exit 1
来源：http://jeu.yuxming.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rai.zhongyouzk.top

[M06] 向标准错误输出
来源：http://coy.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://zxc.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sqw.ydzc1.top

JS:   console.error("err")
来源：http://mxs.hywenlv.cn

TS:   console.error("err")
来源：http://ebr.yj20258.top

Java: System.err.println("err")
来源：http://bfv.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cxq.fzhhl.top

Ruby: warn "err"
来源：http://pop.ivvv.top

C#:   Console.Error.WriteLine("err")
来源：http://rjr.ctjpmb.com

[M07] 判断是否为主入口
来源：http://cbs.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://uwy.zhijiandao.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fhj.zhaomingkeji.xyz

JS:   require.main === module
来源：http://xaj.dashuyun.cn

TS:   require.main === module
来源：http://qlz.hnqzz.top

Java: public static void main(String[] args)
来源：http://dlx.hongshengwenyu.top

Go:   func main()
来源：http://yrz.iojbl.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qti.cashguo.top

C#:   static void Main(string[] args)
来源：http://mrp.yj20258888.top

[M08] 获取系统与运行时信息
来源：http://ghj.jinqigfzy.top

Py:   platform.system();  platform.python_version()
来源：http://opk.fengsongda.top

PHP:  PHP_OS;  phpversion();
来源：http://qzx.zdqjudy.top

JS:   process.platform;  process.version
来源：http://ezm.ivvv.top

TS:   process.platform;  process.version
来源：http://ign.jiagoushi.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://stg.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pku.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hgk.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rcj.zdbjq.cn

================================================================================
来源：http://hsh.zycfv.cn

N. 数据结构与算法
来源：http://gya.hywenlv.cn

================================================================================
来源：http://sqx.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://djy.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://dte.yangfankeji.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://siu.iojbl.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ksu.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://krg.hesvh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lvt.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://cus.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://asn.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://iht.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://bsq.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://hgz.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bnh.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qvc.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://awr.cashguo.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jvd.feifeiyinyue.top

Go:   slices.Sort(arr)
来源：http://hip.ydzc1.top

Ruby: arr.sort
来源：http://suv.redwolf501.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dle.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://oel.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ayx.wangdashe.top

PHP:  // 递归实现，或用 usort
来源：http://bfy.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qqh.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yxn.smart0.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gyk.zhaomingkeji.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vgu.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dqf.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://bml.hnqzz.top

[N04] 斐波那契数列
来源：http://eee.epnwcf.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://owr.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hmp.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vxz.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ayb.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://srd.birdmap.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qjx.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pto.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pyg.xinyue.icu

[N05] 最大公约数
来源：http://yfr.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://hhy.fengsongda.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vpe.aibaodan.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hwv.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vpf.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xls.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kqa.hesvh.cn

Ruby: a.gcd(b)
来源：http://rch.316326.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dzd.guowangkeji.top

[N06] 判断回文字符串
来源：http://xuf.yvedp.cn

Py:   s == s[::-1]
来源：http://cjy.bbcook.cn

PHP:  $s === strrev($s);
来源：http://phk.9152youxi.cn

JS:   s === [...s].reverse().join("")
来源：http://oud.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://paa.zhaomingkeji.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://apv.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://cro.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://zml.chenlongwang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ieo.nanxuanxn.top

[N07] 两数之和（返回下标）
来源：http://jaj.kuanghao11.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bst.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gto.yj202588.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xrw.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://eow.yfazqb.com

Java: // 手写 HashMap
来源：http://sfc.zycfv.cn

Go:   // 手写 map[int]int
来源：http://acc.andypj.xyz

Ruby: // 手写 Hash
来源：http://pfg.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://vga.52xcode.cn

[N08] 生成全排列
来源：http://ueg.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://qwb.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://eah.aizwys.cn

JS:   // 手写回溯递归
来源：http://khd.jinghuilouyu.cn

TS:   // 手写回溯递归
来源：http://hgt.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://cpw.hnqzz.top

Go:   // 手写回溯递归
来源：http://ruf.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://fyz.daria6918.cn

C#:   // 手写回溯递归
来源：http://jjr.shanyushiyangkeji.top

[N09] 栈与队列
来源：http://eol.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vjt.vehdjk.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gxz.epnwcf.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gcf.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gva.hcnkem.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dsy.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zmn.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://esb.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xcv.xingfuxueyuan.xyz

[N10] 链表节点定义
来源：http://wgz.chenzaomai.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ijr.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://npe.hcnkem.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jcu.fzhhl.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lnm.sweek.top

Java: class Node { int v; Node next; }
来源：http://bga.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://dik.tianlin.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://dxu.vehdjk.com

C#:   class Node { public int V; public Node? Next; }
来源：http://phr.fengsongda.top

[N11] 二叉树中序遍历
来源：http://jce.hnqzz.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aro.yj202588.top

PHP:  // 手写递归函数
来源：http://ebr.cheryme.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tyo.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fnm.wangshuangyany.cn

Java: // 手写递归
来源：http://ipg.ivvv.top

Go:   // 手写递归
来源：http://atk.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://brj.jyoumei.cn

C#:   // 手写递归
来源：http://srq.sysykeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eal.jinyuanbaomall.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rjv.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dzi.bjfxy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wim.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yhf.sweek.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://swx.aibaodan.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gwu.dashuyun.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bfq.gzhubu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bsa.fehbvm.com

================================================================================
来源：http://lrx.zhijiandao.cn

O. 并发与异步
来源：http://hvz.jinyuanbaomall.cn

================================================================================
来源：http://mbt.haohaochexian.top

[O01] 启动一个线程
来源：http://bjd.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bgr.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pna.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xwx.ydjk.org.cn

TS:   // 同 JS
来源：http://fdz.ehwqpu.com

Java: new Thread(() -> f()).start()
来源：http://hpb.ywan-chungtsiang.top

Go:   go f()
来源：http://fxi.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://ekt.yangfankeji.com

C#:   Task.Run(() => F());
来源：http://fhr.aizwys.cn

[O02] 使用线程池
来源：http://xsd.svipenyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pud.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wmr.shangyingyoupin.top

JS:   // worker_threads 线程池
来源：http://sdt.shangyingyoupin.top

TS:   // worker_threads 线程池
来源：http://obm.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pje.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aca.hammf.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tbu.pengpengdd.cyou

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://poi.cheryme.top

[O03] 加锁保护共享数据
来源：http://vwt.vehdjk.com

Py:   with lock: shared += 1
来源：http://cpl.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://kwn.fengsongda.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cvo.ydzc1.top

TS:   // 同 JS
来源：http://zas.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://cub.gzhubu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nax.hcnkem.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://yqe.jinqigfzy.top

C#:   lock (gate) { shared++; }
来源：http://nsm.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://rrc.cheryme.top

Py:   async def f():⏎    await g()
来源：http://jmh.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xxk.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://nam.sjlbkw.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://iwh.yueranfly.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nce.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qwg.xylfe.cn

Ruby: # 用 Fiber 或 async gem
来源：http://shz.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://vch.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://qdb.9152youxi.cn

Py:   asyncio.gather(*tasks)
来源：http://awp.nanxuanxn.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xrx.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://omg.quarkkingdee.top

TS:   await Promise.all(tasks)
来源：http://mfl.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vkj.pengpengdd.cyou

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ony.zycfv.cn

Ruby: threads.map(&:join)
来源：http://dju.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kbo.ppjwa.cn

[O06] 使用进程池
来源：http://zom.dianchejie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zkr.jyoumei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://veq.cucudq.cn

JS:   // child_process / cluster 模块
来源：http://krr.yangfankeji.com

TS:   // child_process / cluster 模块
来源：http://ret.vqdsnc.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jiw.haohaochexian.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://val.yongpay.top

Ruby: // fork 块
来源：http://vcv.hongshengwenyu.top

C#:   Parallel.For
来源：http://agx.andypj.xyz

================================================================================
来源：http://opt.ywan-chungtsiang.top

P. 常用工具函数
来源：http://cpt.redwolf501.top

================================================================================
来源：http://djl.andypj.xyz

[P01] 生成 UUID
来源：http://kbb.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://aea.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bpo.zhengqikj.top

JS:   crypto.randomUUID()
来源：http://lpb.shzxlz.cn

TS:   crypto.randomUUID()
来源：http://atr.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://wag.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://hwo.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://vvl.guannengcc.top

C#:   Guid.NewGuid().ToString()
来源：http://dfc.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://hfw.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uvx.ywan-chungtsiang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ehp.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dac.vqdsnc.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ans.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wjs.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aph.zdbjq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dwj.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cjw.haohaochexian.top

[P03] 生成短随机字符串
来源：http://kpo.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dsq.smart0.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pkm.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ztw.ywan-chungtsiang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wko.zdbjq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kye.zhongyouzk.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iez.zhongyouzk.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lqx.havefunace.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ylh.hcnkem.com

[P04] 求长度
来源：http://pby.wangdashe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yhg.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jid.svipenyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rnc.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://okv.yonumen.top

Java: list.size();  map.size();  s.length()
来源：http://gel.yueranfly.top

Go:   len(arr);  len(m)
来源：http://nqb.yj202588.top

Ruby: x.length;  x.size
来源：http://hmv.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pam.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://hvt.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://pbt.fzhhl.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xni.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tgp.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ras.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tdp.wangshuangyany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ugr.sweek.top

Ruby: a == b
来源：http://buf.yvedp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uji.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rci.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ntn.guannengcc.top

PHP:  if (empty($x)) {}
来源：http://rzb.jyoumei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eij.zhongyouzk.top

TS:   if (x == null) {}
来源：http://fwp.pengpengdd.cyou

Java: if (x == null || x.isEmpty()) {}
来源：http://nkj.c1oappe.top

Go:   if x == nil {}
来源：http://kup.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bmm.yj202588.top

C#:   if (x is null) {}
来源：http://sff.hysaishi.cn

[P07] 防抖与节流
来源：http://wco.jinghuilouyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://szi.daxiang520.top

PHP:  // 手写时间戳比较
来源：http://fsa.jinqigfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ogk.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fze.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rbs.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dne.yj20258.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qvb.zdbjq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sux.jinqigfzy.top

[P08] 处理浮点精度问题
来源：http://orc.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pyz.kuanghao11.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wlz.zhengqikj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xre.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wxe.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ttr.jianghu66.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mer.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://upk.andypj.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pww.daria6918.cn

================================================================================
来源：http://urg.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://egy.shzxlz.cn

================================================================================
来源：http://mca.hfpthk.cn

[Q01] 创建表
来源：http://jps.meibo888.top

CREATE TABLE users (
来源：http://iaf.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yen.ctjpmb.com

name VARCHAR(50) NOT NULL,
来源：http://kkb.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://eps.quarkkingdee.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fdu.gotoacloud.top

);
来源：http://fbf.ppjwa.cn

[Q02] 创建带外键的表
来源：http://mup.shuidangran.top

CREATE TABLE orders (
来源：http://ihw.zdqjudy.top


<!-- 参考信息 -->