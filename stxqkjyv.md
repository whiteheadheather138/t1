代发 wailian999

[M04] 获取当前工作目录
来源：http://kww.hesvh.cn

Py:   os.getcwd()
来源：http://uvp.shuidangran.top

PHP:  getcwd();
来源：http://enl.sufxvd.cn

JS:   process.cwd()
来源：http://tfo.yangfankeji.com

TS:   process.cwd()
来源：http://opb.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://sdk.bjfxy.top

Go:   os.Getwd()
来源：http://xuh.zhijiandao.cn

Ruby: Dir.pwd
来源：http://zdf.chenzaomai.com

C#:   Directory.GetCurrentDirectory()
来源：http://lep.cdnleiting.top

[M05] 设置退出码
来源：http://zwv.haohaochexian.top

Py:   sys.exit(1)
来源：http://qqz.nwbrower.top

PHP:  exit(1);
来源：http://tdv.cucudq.cn

JS:   process.exit(1)
来源：http://wrj.zycfv.cn

TS:   process.exit(1)
来源：http://nfn.uphjek.com

Java: System.exit(1)
来源：http://rav.dianchejie.cn

Go:   os.Exit(1)
来源：http://ztd.ydzc1.top

Ruby: exit 1
来源：http://qbb.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hmk.yfazqb.com

[M06] 向标准错误输出
来源：http://ofp.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://fzq.yonumen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tot.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://suq.ydjk.org.cn

TS:   console.error("err")
来源：http://jvh.chenjidiqi.icu

Java: System.err.println("err")
来源：http://fig.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fwm.ctjpmb.com

Ruby: warn "err"
来源：http://yfs.yj20258888.top

C#:   Console.Error.WriteLine("err")
来源：http://ast.yj202588.top

[M07] 判断是否为主入口
来源：http://mpc.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://nyq.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gtc.yuxming.cn

JS:   require.main === module
来源：http://lyq.fzhhl.top

TS:   require.main === module
来源：http://obp.fehbvm.com

Java: public static void main(String[] args)
来源：http://asw.ydjk.org.cn

Go:   func main()
来源：http://lip.tian-w.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nmr.nwbrower.top

C#:   static void Main(string[] args)
来源：http://nql.ydjk.org.cn

[M08] 获取系统与运行时信息
来源：http://cvx.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://hds.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://qbl.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://jro.fzhhl.top

TS:   process.platform;  process.version
来源：http://qjp.guowangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ftv.zhengqikj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fya.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wxn.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://hlz.yj20258.top

================================================================================
来源：http://qrd.gogol.net.cn

N. 数据结构与算法
来源：http://llq.wangdashe.top

================================================================================
来源：http://wzp.nanxinkj.top

[N01] 二分查找（有序数组）
来源：http://okc.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ogv.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ogn.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pmx.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qzr.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aoq.xuetiantiany.cn

Go:   sort.SearchInts(arr, x)
来源：http://lyq.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qkf.gzhubu.top

C#:   Array.BinarySearch(arr, x)
来源：http://vkb.redwolf501.top

[N02] 排序（工程实践用内置实现）
来源：http://hnt.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://zcb.fzhhl.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tly.yuxming.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ttb.xziqi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sqe.wangdashe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://emv.jlsjyb.cn

Go:   slices.Sort(arr)
来源：http://zfy.cashguo.top

Ruby: arr.sort
来源：http://lup.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lnb.aizwys.cn

[N03] 快速排序（分治示例）
来源：http://kud.gaohongyu789.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rkh.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://rqa.c1oappe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://piq.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iwa.zdbjq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zav.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rja.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dmq.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://mkx.iojbl.cn

[N04] 斐波那契数列
来源：http://rlc.hammf.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lbp.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eay.zdbjq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bof.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://snd.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://asz.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zly.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jkx.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ygf.guannengcc.top

[N05] 最大公约数
来源：http://sig.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://xqm.fzhhl.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oty.yvedp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vzm.jinghuilouyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ylb.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eug.pycfn.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gwo.cqqwz.cn

Ruby: a.gcd(b)
来源：http://wbq.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vzq.zycfv.cn

[N06] 判断回文字符串
来源：http://bai.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://vcc.xylfe.cn

PHP:  $s === strrev($s);
来源：http://now.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://rrd.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://jeb.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://for.yonumen.top

Go:   // 双指针从两端比较
来源：http://srn.daria6918.cn

Ruby: s == s.reverse
来源：http://ada.jinyuanbaomall.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://opu.chenzaomai.com

[N07] 两数之和（返回下标）
来源：http://nbf.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rju.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gdm.ydzc1.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mck.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://mvu.nanxinkj.top

Java: // 手写 HashMap
来源：http://ypy.jlsjyb.cn

Go:   // 手写 map[int]int
来源：http://fpq.jinqigufen.top

Ruby: // 手写 Hash
来源：http://eno.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://peb.zhixingplan.top

[N08] 生成全排列
来源：http://ohd.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://ldc.redwolf501.top

PHP:  // 手写递归交换
来源：http://fxl.yj20258888.top

JS:   // 手写回溯递归
来源：http://exh.xuanzx.com

TS:   // 手写回溯递归
来源：http://ngx.ivvv.top

Java: // 手写回溯递归
来源：http://emc.zhengqikj.top

Go:   // 手写回溯递归
来源：http://crf.guowangkeji.top

Ruby: arr.permutation.to_a
来源：http://bsd.smart0.xyz

C#:   // 手写回溯递归
来源：http://wcg.jiagoushi.top

[N09] 栈与队列
来源：http://gfw.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jvl.yueranfly.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bzt.zycfv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iiw.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nes.kuanghao11.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qyt.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vhb.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hqe.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kuu.yuanzhike.top

[N10] 链表节点定义
来源：http://kmu.tianlin.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://esn.hcnkem.com

PHP:  class Node { public $v; public $next = null; }
来源：http://kbw.ybcxt.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ibt.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wdb.yj202588.top

Java: class Node { int v; Node next; }
来源：http://tjn.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://ywm.jianghu66.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wab.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fls.pycfn.com

[N11] 二叉树中序遍历
来源：http://opi.tanke756.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ieh.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://fws.chenjidiqi.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zrr.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sfe.xuanzx.com

Java: // 手写递归
来源：http://vct.jiagoushi.top

Go:   // 手写递归
来源：http://trx.hongshengwenyu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dyd.tianlin.xyz

C#:   // 手写递归
来源：http://ctg.guowangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lam.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kxw.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vlf.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pwu.tanke756.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yet.ivvv.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wsl.xuanzx.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://anu.sysykeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tvn.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mbe.ywan-chungtsiang.top

================================================================================
来源：http://hzp.havefunace.top

O. 并发与异步
来源：http://dvd.jinqigfzy.top

================================================================================
来源：http://hvg.chenlongwang.top

[O01] 启动一个线程
来源：http://zji.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mnh.svipenyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://waf.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dys.nwbrower.top

TS:   // 同 JS
来源：http://ahw.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://hwe.zdbjq.cn

Go:   go f()
来源：http://gjo.tianlin.xyz

Ruby: Thread.new { f }
来源：http://gxr.mhx1999.top

C#:   Task.Run(() => F());
来源：http://gpn.jinyuanbaomall.cn

[O02] 使用线程池
来源：http://xtu.snrcjt.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xps.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://knf.xuanzx.com

JS:   // worker_threads 线程池
来源：http://mmr.epnwcf.com

TS:   // worker_threads 线程池
来源：http://wir.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://qgp.kuanghao11.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rri.chenzaomai.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iax.shuidangran.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://twx.iojbl.cn

[O03] 加锁保护共享数据
来源：http://plp.tianlin.xyz

Py:   with lock: shared += 1
来源：http://yzj.redwolf501.top

PHP:  // 用 flock() 做文件锁
来源：http://qzt.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jwu.chenjidiqi.icu

TS:   // 同 JS
来源：http://gjj.xylfe.cn

Java: synchronized (this) { shared++; }
来源：http://oqt.jinqigfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://flw.jinghuilouyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://edb.shuidangran.top

C#:   lock (gate) { shared++; }
来源：http://tdh.jinghuilouyu.cn

[O04] 定义异步函数并等待
来源：http://atz.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://suu.sxryk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pcq.hammf.cn

JS:   async function f() { await g(); }
来源：http://jsk.zdqjudy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://oty.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://olr.nanxinkj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vif.jianghu66.top

Ruby: # 用 Fiber 或 async gem
来源：http://mri.sysykeji.top

C#:   async Task F() { await G(); }
来源：http://egp.svipenyu.cn

[O05] 并发执行并等待全部完成
来源：http://amh.ivvv.top

Py:   asyncio.gather(*tasks)
来源：http://qiy.hnxiangtu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sdd.ppjwa.cn

JS:   await Promise.all(tasks)
来源：http://tvo.ehwqpu.com

TS:   await Promise.all(tasks)
来源：http://fzz.zhengqikj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://btp.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tiz.daxiang520.top

Ruby: threads.map(&:join)
来源：http://wiu.hongshengwenyu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cbg.yj202588.top

[O06] 使用进程池
来源：http://fdy.yueranfly.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ucd.yueranfly.top

PHP:  // pcntl_fork 或多进程队列
来源：http://paj.316326.xyz

JS:   // child_process / cluster 模块
来源：http://fus.gotoacloud.top

TS:   // child_process / cluster 模块
来源：http://bti.jqgfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rwt.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fnh.meibo888.top

Ruby: // fork 块
来源：http://dqr.zhijiandao.cn

C#:   Parallel.For
来源：http://jhu.kuanghao11.cn

================================================================================
来源：http://wmx.hysaishi.cn

P. 常用工具函数
来源：http://pmt.jqgufenzy.top

================================================================================
来源：http://eym.nanxuanxn.top

[P01] 生成 UUID
来源：http://hmd.feifeiyinyue.top

Py:   str(uuid.uuid4())
来源：http://vec.yueranfly.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kku.jianghu66.top

JS:   crypto.randomUUID()
来源：http://kfx.uphjek.com

TS:   crypto.randomUUID()
来源：http://hlr.chenlongwang.top

Java: UUID.randomUUID().toString()
来源：http://fbq.cdnleiting.top

Go:   // 用 github.com/google/uuid
来源：http://etr.ydjk.org.cn

Ruby: SecureRandom.uuid
来源：http://qvd.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://zmo.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://dso.dianchejie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rmi.sysykeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nbo.cashguo.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vzi.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://paf.andypj.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xtc.yj202588.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tqg.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yxc.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jst.ydzc1.top

[P03] 生成短随机字符串
来源：http://saa.daria6918.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jnj.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fhl.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wqz.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qls.jinyuanbaomall.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://txu.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hru.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yoh.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mxq.yanxiufei.cn

[P04] 求长度
来源：http://uxu.ydjk.org.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dfj.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fio.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://byp.cucudq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xtd.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://huy.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://fjt.sxryk.cn

Ruby: x.length;  x.size
来源：http://mwh.meibo888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nna.zhijiandao.cn

[P05] 判断两个对象内容是否相等
来源：http://onf.zhongyouzk.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://znr.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://npt.fanxiaobao.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://shg.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nof.cdnleiting.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zai.uphjek.com

Go:   reflect.DeepEqual(a, b)
来源：http://fdm.guannengcc.top

Ruby: a == b
来源：http://xsd.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gmr.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xhu.jyoumei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hnd.sufxvd.cn

PHP:  if (empty($x)) {}
来源：http://msb.xylfe.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vzf.xuetiantiany.cn

TS:   if (x == null) {}
来源：http://ofy.bjfxy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://txx.yj202588.top

Go:   if x == nil {}
来源：http://yww.zhiwuduotai.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ivg.zhaomingkeji.xyz

C#:   if (x is null) {}
来源：http://fje.yuanzhike.top

[P07] 防抖与节流
来源：http://rch.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pbj.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://jnu.yj202588.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pck.hysaishi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://obv.zhengqikj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vtu.cqqwz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://isk.guannengcc.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mht.zhaomingkeji.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xzd.xziqi.cn

[P08] 处理浮点精度问题
来源：http://rci.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gzr.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bft.zhixingplan.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://djx.vehdjk.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sha.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://umn.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hng.aizwys.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://exu.tanke756.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hny.smart0.xyz

================================================================================
来源：http://pnb.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gda.mhx1999.top

================================================================================
来源：http://gxd.shangyingyoupin.top

[Q01] 创建表
来源：http://rbc.fzhhl.top

CREATE TABLE users (
来源：http://zjf.fzhhl.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://axt.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://fjv.zhiwuduotai.top

email VARCHAR(100) UNIQUE,
来源：http://yqn.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iep.shanyushiyangkeji.top

);
来源：http://ugx.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://pta.tianlin.xyz

CREATE TABLE orders (
来源：http://tat.svipenyu.cn


<!-- 参考信息 -->