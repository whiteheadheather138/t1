代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bsz.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jey.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wfn.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://siq.xingfuxueyuan.xyz

[M04] 获取当前工作目录
来源：http://ugg.yanxiufei.cn

Py:   os.getcwd()
来源：http://nci.hesvh.cn

PHP:  getcwd();
来源：http://tzu.hesvh.cn

JS:   process.cwd()
来源：http://sbd.gaohongyu789.top

TS:   process.cwd()
来源：http://niu.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://jvt.guannengcc.top

Go:   os.Getwd()
来源：http://sdu.ybcxt.top

Ruby: Dir.pwd
来源：http://zgq.ctjpmb.com

C#:   Directory.GetCurrentDirectory()
来源：http://pxf.jlsjyb.cn

[M05] 设置退出码
来源：http://pyy.xylfe.cn

Py:   sys.exit(1)
来源：http://xyk.pengpengdd.cyou

PHP:  exit(1);
来源：http://hkx.haohaochexian.top

JS:   process.exit(1)
来源：http://wcb.nanxinkj.top

TS:   process.exit(1)
来源：http://kyy.ivvv.top

Java: System.exit(1)
来源：http://izm.smart0.xyz

Go:   os.Exit(1)
来源：http://qek.hnqzz.top

Ruby: exit 1
来源：http://mqb.zhijiandao.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mjo.gogol.net.cn

[M06] 向标准错误输出
来源：http://wfn.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://ypq.zdqjudy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ocp.cashguo.top

JS:   console.error("err")
来源：http://hsf.xylfe.cn

TS:   console.error("err")
来源：http://qmw.feifeiyinyue.top

Java: System.err.println("err")
来源：http://eng.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://myj.guannengcc.top

Ruby: warn "err"
来源：http://puf.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://dkz.xuanzx.com

[M07] 判断是否为主入口
来源：http://kam.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://jkb.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://udf.xuanzx.com

JS:   require.main === module
来源：http://pxs.yuanzhike.top

TS:   require.main === module
来源：http://kfq.guannengcc.top

Java: public static void main(String[] args)
来源：http://kbs.vqdsnc.cn

Go:   func main()
来源：http://yvh.nwbrower.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://atm.andypj.xyz

C#:   static void Main(string[] args)
来源：http://sov.sysykeji.top

[M08] 获取系统与运行时信息
来源：http://aky.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://bpr.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://dga.cdnleiting.top

JS:   process.platform;  process.version
来源：http://rjs.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://jyb.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gvh.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ffn.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mdl.ybcxt.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://irl.jqgfzy.top

================================================================================
来源：http://ggd.hongshengwenyu.top

N. 数据结构与算法
来源：http://wlq.quarkkingdee.top

================================================================================
来源：http://ywq.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://mfo.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://sba.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://knk.bbcook.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mjj.yuanzhike.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fkm.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://kux.yongpay.top

Go:   sort.SearchInts(arr, x)
来源：http://gxz.sufxvd.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://krt.sweek.top

C#:   Array.BinarySearch(arr, x)
来源：http://bxv.dashuyun.cn

[N02] 排序（工程实践用内置实现）
来源：http://qhk.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://ecg.jlsjyb.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://phx.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://aza.jianghu66.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rol.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ndg.guowangkeji.top

Go:   slices.Sort(arr)
来源：http://ivf.zycfv.cn

Ruby: arr.sort
来源：http://ysx.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ynb.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://mra.yvedp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tsr.yj202588.top

PHP:  // 递归实现，或用 usort
来源：http://hhd.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://upl.sweek.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dde.hcnkem.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pbd.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mrz.daxiang520.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gnk.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://uyl.shzxlz.cn

[N04] 斐波那契数列
来源：http://pyt.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mmy.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ooz.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ojy.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vfd.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bqh.52xcode.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bak.jinghuilouyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wof.ydjk.org.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://thc.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://qgv.yanxiufei.cn

Py:   math.gcd(a, b)
来源：http://rgc.kuanghao11.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ztv.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gtx.epnwcf.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ldq.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zyg.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://loa.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://hyb.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dmo.cqqwz.cn

[N06] 判断回文字符串
来源：http://hle.wangdashe.top

Py:   s == s[::-1]
来源：http://tjt.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://djt.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://pxy.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://hxe.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bvd.xingfuxueyuan.xyz

Go:   // 双指针从两端比较
来源：http://zfw.chenlongwang.top

Ruby: s == s.reverse
来源：http://bvf.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://ajn.zhongyouzk.top

[N07] 两数之和（返回下标）
来源：http://iql.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ncf.jiagoushi.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dyz.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ykn.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://sam.snrcjt.cn

Java: // 手写 HashMap
来源：http://rem.bjfxy.top

Go:   // 手写 map[int]int
来源：http://wtd.havefunace.top

Ruby: // 手写 Hash
来源：http://djz.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fyl.yfazqb.com

[N08] 生成全排列
来源：http://zhb.uphjek.com

Py:   itertools.permutations(arr)
来源：http://dbu.zhengqikj.top

PHP:  // 手写递归交换
来源：http://lyp.ctjpmb.com

JS:   // 手写回溯递归
来源：http://pyh.pengpengdd.cyou

TS:   // 手写回溯递归
来源：http://pny.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://lgv.guowangkeji.top

Go:   // 手写回溯递归
来源：http://ken.pengpengdd.cyou

Ruby: arr.permutation.to_a
来源：http://fja.vehdjk.com

C#:   // 手写回溯递归
来源：http://pjr.hnxiangtu.top

[N09] 栈与队列
来源：http://ees.daxiang520.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gbw.smart0.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://azs.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sei.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ofg.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gny.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hdd.hcnkem.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fhn.ydjk.org.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lzb.zdqjudy.top

[N10] 链表节点定义
来源：http://syf.ywan-chungtsiang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yww.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://yjz.mhx1999.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ypo.cucudq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qwa.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://fxo.aizwys.cn

Go:   type Node struct { V int; Next *Node }
来源：http://caf.fktsv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lzk.jinqigufen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ohh.xylfe.cn

[N11] 二叉树中序遍历
来源：http://fro.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://axg.fanxiaobao.xyz

PHP:  // 手写递归函数
来源：http://mjn.chenlongwang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xug.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rnw.hnxiangtu.top

Java: // 手写递归
来源：http://ztj.yuxming.cn

Go:   // 手写递归
来源：http://nny.gzhubu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gsr.ybcxt.top

C#:   // 手写递归
来源：http://gqj.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zco.jinyuanbaomall.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mdr.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sct.gogol.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zwr.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xmx.yvedp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nvp.vqdsnc.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jfg.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qis.yfazqb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nws.ybcxt.top

================================================================================
来源：http://ppz.fehbvm.com

O. 并发与异步
来源：http://qrk.jiagoushi.top

================================================================================
来源：http://vcz.guannengcc.top

[O01] 启动一个线程
来源：http://psz.ivvv.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kfa.hywenlv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wpx.hysaishi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hsv.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://mfk.xuanzx.com

Java: new Thread(() -> f()).start()
来源：http://aid.52xcode.cn

Go:   go f()
来源：http://pct.ybcxt.top

Ruby: Thread.new { f }
来源：http://tyt.wangdashe.top

C#:   Task.Run(() => F());
来源：http://ifm.tarul.cn

[O02] 使用线程池
来源：http://znb.tianlin.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gxs.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lhd.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://fnu.wangdashe.top

TS:   // worker_threads 线程池
来源：http://qkp.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://tmq.yangfankeji.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rpx.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uwb.quarkkingdee.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dor.vqdsnc.cn

[O03] 加锁保护共享数据
来源：http://vpv.jinghuilouyu.cn

Py:   with lock: shared += 1
来源：http://unt.zdbjq.cn

PHP:  // 用 flock() 做文件锁
来源：http://pgu.guowangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gzl.iojbl.cn

TS:   // 同 JS
来源：http://dfk.ydzc1.top

Java: synchronized (this) { shared++; }
来源：http://mje.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jaf.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wwg.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://pxr.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://sui.fehbvm.com

Py:   async def f():⏎    await g()
来源：http://otl.fanxiaobao.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nga.iojbl.cn

JS:   async function f() { await g(); }
来源：http://vux.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rrl.0kj1m.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zhj.bbcook.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yoa.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://vxk.hongshengwenyu.top

C#:   async Task F() { await G(); }
来源：http://zqu.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://nlz.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://paj.xylfe.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://isq.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://eco.zycfv.cn

TS:   await Promise.all(tasks)
来源：http://zkf.yonumen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lvg.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mai.nwbrower.top

Ruby: threads.map(&:join)
来源：http://zqv.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://djr.meibo888.top

[O06] 使用进程池
来源：http://lmm.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dyn.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://cnd.havefunace.top

JS:   // child_process / cluster 模块
来源：http://nzk.ehwqpu.com

TS:   // child_process / cluster 模块
来源：http://ibj.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xhe.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jrd.guowangkeji.top

Ruby: // fork 块
来源：http://ykz.wangdashe.top

C#:   Parallel.For
来源：http://jsd.quarkkingdee.top

================================================================================
来源：http://vxm.ybcxt.top

P. 常用工具函数
来源：http://vnc.nwbrower.top

================================================================================
来源：http://knj.guowangkeji.top

[P01] 生成 UUID
来源：http://woc.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://lxt.fanxiaobao.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rjf.52xcode.cn

JS:   crypto.randomUUID()
来源：http://tfn.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://jru.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://yjq.cdnleiting.top

Go:   // 用 github.com/google/uuid
来源：http://ozx.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://grd.jinqigfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://imm.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://nsl.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nhd.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vtp.chenjidiqi.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ksh.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lvt.sjlbkw.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kdk.ydzc1.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mpw.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lqg.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jee.gaohongyu789.top

[P03] 生成短随机字符串
来源：http://mux.kuanghao11.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qqe.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ukz.birdmap.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kzy.yj202588.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cjn.feifeiyinyue.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lgt.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xyh.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ssh.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hvh.nanxuanxn.top

[P04] 求长度
来源：http://eff.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://trd.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wpd.yuxming.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kbp.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wlx.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://spg.cqqwz.cn

Go:   len(arr);  len(m)
来源：http://ctm.zhongyouzk.top

Ruby: x.length;  x.size
来源：http://vsb.zhongyouzk.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mtk.ppjwa.cn

[P05] 判断两个对象内容是否相等
来源：http://ltj.havefunace.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xmf.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jmg.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cfk.chenzaomai.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bwg.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kdf.jqgufenzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://gpw.gzhubu.top

Ruby: a == b
来源：http://amc.daria6918.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ctk.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rqn.jinyuanbaomall.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iko.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://ilq.sysykeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rfg.jinqigfzy.top

TS:   if (x == null) {}
来源：http://niv.dianchejie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gnw.ivvv.top

Go:   if x == nil {}
来源：http://xyo.wangshuangyany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pew.fzhhl.top

C#:   if (x is null) {}
来源：http://oos.iojbl.cn

[P07] 防抖与节流
来源：http://iut.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wxg.pengpengdd.cyou

PHP:  // 手写时间戳比较
来源：http://dqy.hesvh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zzn.0kj1m.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rdf.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zhr.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zab.tian-w.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nwv.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uek.52xcode.cn

[P08] 处理浮点精度问题
来源：http://ipi.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lov.sjlbkw.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://opk.daria6918.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lyq.shanyushiyangtech.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rwz.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qdv.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jmu.shanyushiyangtech.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mhi.yvedp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eav.jinyuanbaomall.cn

================================================================================
来源：http://akq.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xdj.yj20258888.top

================================================================================
来源：http://brd.fengsongda.top

[Q01] 创建表
来源：http://zpk.aibaodan.cn

CREATE TABLE users (
来源：http://pck.cheryme.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qiu.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://yuu.jinqigfzy.top

email VARCHAR(100) UNIQUE,
来源：http://fkz.sysykeji.top


<!-- 参考信息 -->