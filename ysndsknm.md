代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kss.dianchejie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jck.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://ouq.dianchejie.cn

C#:   Process.Start("ls", "-l");
来源：http://quv.aibaodan.cn

[M04] 获取当前工作目录
来源：http://ibc.ydjk.org.cn

Py:   os.getcwd()
来源：http://ino.hnxiangtu.top

PHP:  getcwd();
来源：http://ojl.zdbjq.cn

JS:   process.cwd()
来源：http://ifn.hywenlv.cn

TS:   process.cwd()
来源：http://bow.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://bnz.xylfe.cn

Go:   os.Getwd()
来源：http://djh.hesvh.cn

Ruby: Dir.pwd
来源：http://mhw.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://uuz.yuxming.cn

[M05] 设置退出码
来源：http://zyx.meibo888.top

Py:   sys.exit(1)
来源：http://tpg.gzhubu.top

PHP:  exit(1);
来源：http://ihd.ehwqpu.com

JS:   process.exit(1)
来源：http://ppk.chenzaomai.com

TS:   process.exit(1)
来源：http://rdy.havefunace.top

Java: System.exit(1)
来源：http://soj.yfazqb.com

Go:   os.Exit(1)
来源：http://tju.hcnkem.com

Ruby: exit 1
来源：http://ytk.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iwb.sufxvd.cn

[M06] 向标准错误输出
来源：http://fpl.ehwqpu.com

Py:   print("err", file=sys.stderr)
来源：http://vue.hammf.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://chm.zdqjudy.top

JS:   console.error("err")
来源：http://nuw.chenzaomai.com

TS:   console.error("err")
来源：http://aoh.hywenlv.cn

Java: System.err.println("err")
来源：http://jlv.wangshuangyany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zsn.hesvh.cn

Ruby: warn "err"
来源：http://dwm.haohaochexian.top

C#:   Console.Error.WriteLine("err")
来源：http://pxw.316326.xyz

[M07] 判断是否为主入口
来源：http://lzv.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://ayx.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eod.yanxiufei.cn

JS:   require.main === module
来源：http://igg.feifeiyinyue.top

TS:   require.main === module
来源：http://ttm.c1oappe.top

Java: public static void main(String[] args)
来源：http://opi.daria6918.cn

Go:   func main()
来源：http://tqj.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lly.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://ucd.daria6918.cn

[M08] 获取系统与运行时信息
来源：http://fsz.xziqi.cn

Py:   platform.system();  platform.python_version()
来源：http://bru.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://xoe.chenzaomai.com

JS:   process.platform;  process.version
来源：http://wmo.daxiang520.top

TS:   process.platform;  process.version
来源：http://mdd.nanxuanxn.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nec.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rva.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wig.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jld.iojbl.cn

================================================================================
来源：http://jgd.meibo888.top

N. 数据结构与算法
来源：http://mwu.fzhhl.top

================================================================================
来源：http://jnk.sjlbkw.cn

[N01] 二分查找（有序数组）
来源：http://peq.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://dtd.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sve.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ocb.uphjek.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tpb.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qix.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://ycn.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bmo.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vfi.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://sxn.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://edb.zycfv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mlj.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hht.bbcook.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nnb.wangshuangyany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://utp.aizwys.cn

Go:   slices.Sort(arr)
来源：http://lmy.xinyue.icu

Ruby: arr.sort
来源：http://eba.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://krk.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://giq.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wvt.cdnleiting.top

PHP:  // 递归实现，或用 usort
来源：http://qmx.sweek.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wmy.zhiwuduotai.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zfw.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://raf.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jmg.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wzu.hcnkem.com

C#:   // 手写递归，或 Array.Sort
来源：http://cgy.mhx1999.top

[N04] 斐波那契数列
来源：http://vcw.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oal.gaohongyu789.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nvu.zdqjudy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ked.jinqigfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ach.pengpengdd.cyou

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pvt.yvedp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uwp.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hkx.yuanzhike.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tsp.cheryme.top

[N05] 最大公约数
来源：http://ggd.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://hnf.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xbw.316326.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ydx.hcnkem.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://moz.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ams.gogol.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aag.ehwqpu.com

Ruby: a.gcd(b)
来源：http://blu.aibaodan.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ouc.snrcjt.cn

[N06] 判断回文字符串
来源：http://foo.wangdashe.top

Py:   s == s[::-1]
来源：http://nzb.vqdsnc.cn

PHP:  $s === strrev($s);
来源：http://chi.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://txn.daria6918.cn

TS:   s === [...s].reverse().join("")
来源：http://eqd.dianchejie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bbu.xziqi.cn

Go:   // 双指针从两端比较
来源：http://fhv.jinqigufen.top

Ruby: s == s.reverse
来源：http://ifv.jqgufenzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gmp.birdmap.top

[N07] 两数之和（返回下标）
来源：http://mzr.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://czp.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kiu.yj202588.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pvc.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://smv.mhx1999.top

Java: // 手写 HashMap
来源：http://qbd.hywenlv.cn

Go:   // 手写 map[int]int
来源：http://ayj.xylfe.cn

Ruby: // 手写 Hash
来源：http://tjl.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://yga.ybcxt.top

[N08] 生成全排列
来源：http://hfg.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://ien.c1oappe.top

PHP:  // 手写递归交换
来源：http://maw.yj20258888.top

JS:   // 手写回溯递归
来源：http://faj.iojbl.cn

TS:   // 手写回溯递归
来源：http://npm.yj20258888.top

Java: // 手写回溯递归
来源：http://dft.pengpengdd.cyou

Go:   // 手写回溯递归
来源：http://klh.daria6918.cn

Ruby: arr.permutation.to_a
来源：http://ssu.meibo888.top

C#:   // 手写回溯递归
来源：http://yxn.fengsongda.top

[N09] 栈与队列
来源：http://dce.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://koa.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zpm.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://efq.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mmk.meibo888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xwi.guowangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://adw.jiagoushi.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://apk.ehwqpu.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hao.zdbjq.cn

[N10] 链表节点定义
来源：http://yuc.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lce.jinqigfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bft.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mvu.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tcc.nanxinkj.top

Java: class Node { int v; Node next; }
来源：http://oxs.ehwqpu.com

Go:   type Node struct { V int; Next *Node }
来源：http://kde.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eih.zdqjudy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dfb.yuxming.cn

[N11] 二叉树中序遍历
来源：http://gyp.yj202588.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://coe.52xcode.cn

PHP:  // 手写递归函数
来源：http://ocr.snrcjt.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cbt.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qga.sufxvd.cn

Java: // 手写递归
来源：http://mty.zhaomingkeji.xyz

Go:   // 手写递归
来源：http://dze.gzhubu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hqy.aizwys.cn

C#:   // 手写递归
来源：http://vmp.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://daq.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qth.daria6918.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sbf.wangdashe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tnl.jyoumei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tvc.zhoulong.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sks.sxryk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ncp.52xcode.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://htr.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ndh.bbcook.cn

================================================================================
来源：http://eui.ctjpmb.com

O. 并发与异步
来源：http://kzq.hysaishi.cn

================================================================================
来源：http://evd.vqdsnc.cn

[O01] 启动一个线程
来源：http://jxc.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://emz.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bnd.shzxlz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://btl.uphjek.com

TS:   // 同 JS
来源：http://ble.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://wra.yueranfly.top

Go:   go f()
来源：http://eau.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://esp.52xcode.cn

C#:   Task.Run(() => F());
来源：http://zge.zdqjudy.top

[O02] 使用线程池
来源：http://vgl.nanxinkj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ape.jinqigfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cec.nwbrower.top

JS:   // worker_threads 线程池
来源：http://vzl.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://dgh.xuanzx.com

Java: Executors.newFixedThreadPool(4)
来源：http://rff.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bxd.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ahk.ybcxt.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rvo.bbcook.cn

[O03] 加锁保护共享数据
来源：http://chu.nanxinkj.top

Py:   with lock: shared += 1
来源：http://dlm.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://izo.epnwcf.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xrg.hnxiangtu.top

TS:   // 同 JS
来源：http://ghv.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://rsy.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uwf.aizwys.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://olz.jiagoushi.top

C#:   lock (gate) { shared++; }
来源：http://utr.9152youxi.cn

[O04] 定义异步函数并等待
来源：http://wcj.316326.xyz

Py:   async def f():⏎    await g()
来源：http://lau.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://age.andypj.xyz

JS:   async function f() { await g(); }
来源：http://cnh.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jdi.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tto.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ykr.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://jku.daxiang520.top

C#:   async Task F() { await G(); }
来源：http://bsb.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://jeb.shanyushiyangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://glm.hesvh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mpv.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://zol.tarul.cn

TS:   await Promise.all(tasks)
来源：http://uxw.fzhhl.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wvb.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fmi.shangyingyoupin.top

Ruby: threads.map(&:join)
来源：http://osv.hywenlv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yeh.yueranfly.top

[O06] 使用进程池
来源：http://kdr.zhongyouzk.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tej.daxiang520.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hyl.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://jzl.gaohongyu789.top

TS:   // child_process / cluster 模块
来源：http://thf.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bsm.chenzaomai.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jow.uphjek.com

Ruby: // fork 块
来源：http://jic.guowangkeji.top

C#:   Parallel.For
来源：http://rby.nwbrower.top

================================================================================
来源：http://ymx.hnxiangtu.top

P. 常用工具函数
来源：http://xvc.52xcode.cn

================================================================================
来源：http://gmi.aibaodan.cn

[P01] 生成 UUID
来源：http://ujt.yvedp.cn

Py:   str(uuid.uuid4())
来源：http://mid.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uht.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://jyo.mhx1999.top

TS:   crypto.randomUUID()
来源：http://dxv.chenjidiqi.icu

Java: UUID.randomUUID().toString()
来源：http://eyn.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://hfr.yuxming.cn

Ruby: SecureRandom.uuid
来源：http://fqg.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://enc.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://trt.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://whp.kuanghao11.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eky.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fie.shzxlz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://njo.ydzc1.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bwd.yangfankeji.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vbn.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kon.xuetiantiany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://clw.iojbl.cn

[P03] 生成短随机字符串
来源：http://mmq.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rpn.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://twn.dianchejie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kln.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rle.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dqf.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wst.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://owo.ivvv.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hto.cheryme.top

[P04] 求长度
来源：http://upw.jqgfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://apa.iojbl.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://utg.hnqzz.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fpi.ybcxt.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kuy.9152youxi.cn

Java: list.size();  map.size();  s.length()
来源：http://njk.andypj.xyz

Go:   len(arr);  len(m)
来源：http://yyx.xinyue.icu

Ruby: x.length;  x.size
来源：http://xdz.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://het.gogol.net.cn

[P05] 判断两个对象内容是否相等
来源：http://ojj.daxiang520.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fam.nanxuanxn.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qqs.daxiang520.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gnr.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fnl.xinyue.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oqs.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://acv.xinyue.icu

Ruby: a == b
来源：http://nvq.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://isk.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://krc.hesvh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vye.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://odp.xylfe.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://emx.zdbjq.cn

TS:   if (x == null) {}
来源：http://byg.zycfv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mlb.tianlin.xyz

Go:   if x == nil {}
来源：http://gtw.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ggw.jyoumei.cn

C#:   if (x is null) {}
来源：http://chc.52xcode.cn

[P07] 防抖与节流
来源：http://vqq.hnqzz.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qzn.xinyue.icu

PHP:  // 手写时间戳比较
来源：http://ywc.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yic.jyoumei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://idc.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ass.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fnm.yj20258.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pnx.zhoulong.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gez.quarkkingdee.top

[P08] 处理浮点精度问题
来源：http://tpw.hcnkem.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://boq.hysaishi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zxd.ctjpmb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bkp.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jjc.nwbrower.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sif.ydjk.org.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gan.chenjidiqi.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://okw.shzxlz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yem.c1oappe.top

================================================================================
来源：http://rdx.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://scn.xylfe.cn

================================================================================
来源：http://tyj.fehbvm.com

[Q01] 创建表
来源：http://ozh.birdmap.top

CREATE TABLE users (
来源：http://pvi.jiagoushi.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cim.yonumen.top

name VARCHAR(50) NOT NULL,
来源：http://kns.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://yig.ivvv.top


<!-- 参考信息 -->