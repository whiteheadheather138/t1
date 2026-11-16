代发 wailian999

[M04] 获取当前工作目录
来源：http://car.xuanzx.com

Py:   os.getcwd()
来源：http://zcm.xylfe.cn

PHP:  getcwd();
来源：http://ihc.xuetiantiany.cn

JS:   process.cwd()
来源：http://qkq.daxiang520.top

TS:   process.cwd()
来源：http://eyt.zhoulong.xyz

Java: Path.of("").toAbsolutePath()
来源：http://ndw.hfpthk.cn

Go:   os.Getwd()
来源：http://anb.daxiang520.top

Ruby: Dir.pwd
来源：http://exh.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://nis.ppjwa.cn

[M05] 设置退出码
来源：http://nlt.gzhubu.top

Py:   sys.exit(1)
来源：http://fuy.ydjk.org.cn

PHP:  exit(1);
来源：http://nvi.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://qzf.vehdjk.com

TS:   process.exit(1)
来源：http://hsv.daria6918.cn

Java: System.exit(1)
来源：http://hwg.ehwqpu.com

Go:   os.Exit(1)
来源：http://unn.cashguo.top

Ruby: exit 1
来源：http://zix.zhixingplan.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vxr.xuanzx.com

[M06] 向标准错误输出
来源：http://fwr.redwolf501.top

Py:   print("err", file=sys.stderr)
来源：http://kwc.zhijiandao.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mpe.tianlin.xyz

JS:   console.error("err")
来源：http://kkv.feifeiyinyue.top

TS:   console.error("err")
来源：http://zxa.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://qrh.jlsjyb.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xab.andypj.xyz

Ruby: warn "err"
来源：http://rcz.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://hks.c1oappe.top

[M07] 判断是否为主入口
来源：http://gyu.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://cvl.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://voh.fanxiaobao.xyz

JS:   require.main === module
来源：http://xwo.iojbl.cn

TS:   require.main === module
来源：http://dcl.meibo888.top

Java: public static void main(String[] args)
来源：http://fxj.jqgufenzy.top

Go:   func main()
来源：http://lrz.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bdq.sxryk.cn

C#:   static void Main(string[] args)
来源：http://mzj.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://llb.ehwqpu.com

Py:   platform.system();  platform.python_version()
来源：http://ydk.wangshuangyany.cn

PHP:  PHP_OS;  phpversion();
来源：http://qfr.shanyushiyangtech.top

JS:   process.platform;  process.version
来源：http://arj.andypj.xyz

TS:   process.platform;  process.version
来源：http://iab.feifeiyinyue.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wxe.jyoumei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jna.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dal.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://gig.sxryk.cn

================================================================================
来源：http://plm.cucudq.cn

N. 数据结构与算法
来源：http://zgk.zdqjudy.top

================================================================================
来源：http://yzn.bjfxy.top

[N01] 二分查找（有序数组）
来源：http://tsl.ydzc1.top

Py:   bisect.bisect_left(arr, x)
来源：http://xvy.guowangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qty.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rsy.gaohongyu789.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lgv.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://fht.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://ldh.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zkj.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://zlt.yuanzhike.top

[N02] 排序（工程实践用内置实现）
来源：http://hha.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://swz.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wmw.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://frh.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ksu.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://miw.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://plj.gaohongyu789.top

Ruby: arr.sort
来源：http://eyd.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://zxk.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://yoc.xuanzx.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fcg.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://shs.wangshuangyany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yoi.birdmap.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eky.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oyk.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kuw.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eow.ivvv.top

C#:   // 手写递归，或 Array.Sort
来源：http://pra.yfazqb.com

[N04] 斐波那契数列
来源：http://dii.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://szb.xuanzx.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vsy.wangdashe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://amv.52xcode.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ipt.wangshuangyany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xdt.yfazqb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zoe.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tft.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://puk.zhiwuduotai.top

[N05] 最大公约数
来源：http://gtv.zhijiandao.cn

Py:   math.gcd(a, b)
来源：http://rha.yanxiufei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bfm.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qsn.svipenyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uwx.jiagoushi.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qpd.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ubg.havefunace.top

Ruby: a.gcd(b)
来源：http://sno.redwolf501.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xhe.mhx1999.top

[N06] 判断回文字符串
来源：http://uks.tanke756.top

Py:   s == s[::-1]
来源：http://ylf.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://bik.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://lzi.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://gbn.zhixingplan.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lrc.chenjidiqi.icu

Go:   // 双指针从两端比较
来源：http://zaq.ctjpmb.com

Ruby: s == s.reverse
来源：http://awy.316326.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://xga.cqqwz.cn

[N07] 两数之和（返回下标）
来源：http://ngq.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vgj.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lpw.fktsv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://idz.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://dja.hfpthk.cn

Java: // 手写 HashMap
来源：http://zaz.cqqwz.cn

Go:   // 手写 map[int]int
来源：http://qlq.daxiang520.top

Ruby: // 手写 Hash
来源：http://iaq.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://aul.andypj.xyz

[N08] 生成全排列
来源：http://izs.316326.xyz

Py:   itertools.permutations(arr)
来源：http://pph.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://eya.nanxinkj.top

JS:   // 手写回溯递归
来源：http://tdp.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://ygq.shangyingyoupin.top

Java: // 手写回溯递归
来源：http://czv.zhengqikj.top

Go:   // 手写回溯递归
来源：http://tbf.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://gfu.hywenlv.cn

C#:   // 手写回溯递归
来源：http://oih.guowangkeji.top

[N09] 栈与队列
来源：http://xpu.yangfankeji.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ymh.redwolf501.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://chd.jqgufenzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fhs.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cov.hesvh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bcc.gogol.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yff.zycfv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ryb.zhiwuduotai.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://noy.nanxuanxn.top

[N10] 链表节点定义
来源：http://kvn.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sgp.9152youxi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://psy.daria6918.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rru.daria6918.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tnd.316326.xyz

Java: class Node { int v; Node next; }
来源：http://tje.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vqd.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://dgx.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fjj.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://vor.jqgfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xvm.zdbjq.cn

PHP:  // 手写递归函数
来源：http://wjz.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sjm.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kan.tianlin.xyz

Java: // 手写递归
来源：http://ysi.xinyue.icu

Go:   // 手写递归
来源：http://iuw.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tby.fzhhl.top

C#:   // 手写递归
来源：http://bly.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://knr.fehbvm.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mfn.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gcz.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sgd.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rig.ydzc1.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://clz.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zev.shanyushiyangtech.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dva.yj202588.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wdr.jinyuanbaomall.cn

================================================================================
来源：http://cni.tanke756.top

O. 并发与异步
来源：http://wpk.jiagoushi.top

================================================================================
来源：http://eqg.tarul.cn

[O01] 启动一个线程
来源：http://iai.zdqjudy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mwj.dashuyun.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://emh.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://elt.cdnleiting.top

TS:   // 同 JS
来源：http://kdd.kuanghao11.cn

Java: new Thread(() -> f()).start()
来源：http://vlk.yfazqb.com

Go:   go f()
来源：http://ody.pycfn.com

Ruby: Thread.new { f }
来源：http://tcf.zhixingplan.top

C#:   Task.Run(() => F());
来源：http://shg.0kj1m.cn

[O02] 使用线程池
来源：http://zzg.uphjek.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ajc.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mip.mhx1999.top

JS:   // worker_threads 线程池
来源：http://dsa.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://bck.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://vns.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pid.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uvw.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aaf.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://ayg.xuetiantiany.cn

Py:   with lock: shared += 1
来源：http://wyg.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://xfc.iojbl.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nwh.zhixingplan.top

TS:   // 同 JS
来源：http://eor.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://ien.shanyushiyangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yle.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://udr.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://gdb.cdnleiting.top

[O04] 定义异步函数并等待
来源：http://jrr.hongshengwenyu.top

Py:   async def f():⏎    await g()
来源：http://dcq.hysaishi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yda.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://vgw.cashguo.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kzw.tarul.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ohb.jyoumei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eoq.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://arn.tarul.cn

C#:   async Task F() { await G(); }
来源：http://wby.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://oks.andypj.xyz

Py:   asyncio.gather(*tasks)
来源：http://veg.hfpthk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ttn.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://bwc.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://ddy.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dzs.sxryk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://utl.bbcook.cn

Ruby: threads.map(&:join)
来源：http://fcz.hammf.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hhi.ydzc1.top

[O06] 使用进程池
来源：http://xmu.shanyushiyangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zjh.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fxd.uphjek.com

JS:   // child_process / cluster 模块
来源：http://hwe.cqqwz.cn

TS:   // child_process / cluster 模块
来源：http://rlr.hammf.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dcv.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://smj.chenzaomai.com

Ruby: // fork 块
来源：http://gqg.chenjidiqi.icu

C#:   Parallel.For
来源：http://yay.fengsongda.top

================================================================================
来源：http://ffk.svipenyu.cn

P. 常用工具函数
来源：http://mxr.wangshuangyany.cn

================================================================================
来源：http://vbc.jinqigufen.top

[P01] 生成 UUID
来源：http://hty.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://hwo.ehwqpu.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dcg.shanyushiyangtech.top

JS:   crypto.randomUUID()
来源：http://otl.fktsv.cn

TS:   crypto.randomUUID()
来源：http://gox.9152youxi.cn

Java: UUID.randomUUID().toString()
来源：http://rsu.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://yvj.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://bqy.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://kmw.316326.xyz

[P02] MD5 / SHA256 摘要
来源：http://kru.sjlbkw.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jrl.tarul.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wax.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xtk.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ehi.yfazqb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sgy.ehwqpu.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xab.andypj.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nnz.fzhhl.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vqd.quarkkingdee.top

[P03] 生成短随机字符串
来源：http://sgh.zhongyouzk.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wya.xylfe.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vex.xuetiantiany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ddx.zhiwuduotai.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uzc.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sdn.daria6918.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qys.zhoulong.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://fdz.iojbl.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gwk.jianghu66.top

[P04] 求长度
来源：http://uun.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://evt.zhongyouzk.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tqz.yanxiufei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pgc.tarul.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xhd.zhaomingkeji.xyz

Java: list.size();  map.size();  s.length()
来源：http://cwg.mhx1999.top

Go:   len(arr);  len(m)
来源：http://uxi.jinyuanbaomall.cn

Ruby: x.length;  x.size
来源：http://lqz.hysaishi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://obj.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://bev.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://yal.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lqi.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kcp.hesvh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qwv.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://svt.aibaodan.cn

Go:   reflect.DeepEqual(a, b)
来源：http://noa.hnqzz.top

Ruby: a == b
来源：http://ljy.yangfankeji.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cow.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sem.hesvh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uag.cdnleiting.top

PHP:  if (empty($x)) {}
来源：http://zbn.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lbb.jqgufenzy.top

TS:   if (x == null) {}
来源：http://ylg.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jvu.aibaodan.cn

Go:   if x == nil {}
来源：http://ekl.bbcook.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tok.ppjwa.cn

C#:   if (x is null) {}
来源：http://zqo.fehbvm.com

[P07] 防抖与节流
来源：http://vlu.xuetiantiany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wyr.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://dut.hammf.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gwf.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://huo.shuidangran.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hke.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kvn.hnxiangtu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zqo.jianghu66.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zpy.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://fxc.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gir.hywenlv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ikn.jyoumei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cmh.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mhu.ywan-chungtsiang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fia.redwolf501.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cnn.zhaomingkeji.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yst.fanxiaobao.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rba.hcnkem.com

================================================================================
来源：http://pmf.hnqzz.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://afh.pycfn.com

================================================================================
来源：http://fxm.ydzc1.top

[Q01] 创建表
来源：http://htr.feifeiyinyue.top

CREATE TABLE users (
来源：http://gkt.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zno.mhx1999.top

name VARCHAR(50) NOT NULL,
来源：http://dbg.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://hgx.hfpthk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tzv.jinghuilouyu.cn

);
来源：http://prq.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://siv.tian-w.cn

CREATE TABLE orders (
来源：http://afd.shanyushiyangkeji.top


<!-- 参考信息 -->