代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://czt.yj202588.top

[M05] 设置退出码
来源：http://hjf.yueranfly.top

Py:   sys.exit(1)
来源：http://sfu.cucudq.cn

PHP:  exit(1);
来源：http://sgt.aizwys.cn

JS:   process.exit(1)
来源：http://mne.jinqigufen.top

TS:   process.exit(1)
来源：http://vku.yangfankeji.com

Java: System.exit(1)
来源：http://tpe.cucudq.cn

Go:   os.Exit(1)
来源：http://fzq.jianghu66.top

Ruby: exit 1
来源：http://umj.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eco.nanxuanxn.top

[M06] 向标准错误输出
来源：http://rrv.sufxvd.cn

Py:   print("err", file=sys.stderr)
来源：http://ctm.bbcook.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pgo.svipenyu.cn

JS:   console.error("err")
来源：http://sgm.cashguo.top

TS:   console.error("err")
来源：http://ciq.cucudq.cn

Java: System.err.println("err")
来源：http://hns.nanxuanxn.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tgl.shangyingyoupin.top

Ruby: warn "err"
来源：http://czu.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://rkp.chenzaomai.com

[M07] 判断是否为主入口
来源：http://juw.cashguo.top

Py:   if __name__ == "__main__":
来源：http://eno.hfpthk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xbj.zdqjudy.top

JS:   require.main === module
来源：http://hxa.tian-w.cn

TS:   require.main === module
来源：http://xdy.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://gsm.chenjidiqi.icu

Go:   func main()
来源：http://xus.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ksv.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://ovw.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://fia.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://tsm.hammf.cn

PHP:  PHP_OS;  phpversion();
来源：http://qtb.vehdjk.com

JS:   process.platform;  process.version
来源：http://ysy.mhx1999.top

TS:   process.platform;  process.version
来源：http://rty.guowangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bao.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xgv.zdbjq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cqd.iojbl.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lpl.c1oappe.top

================================================================================
来源：http://tcm.pycfn.com

N. 数据结构与算法
来源：http://sbu.havefunace.top

================================================================================
来源：http://vqt.yongpay.top

[N01] 二分查找（有序数组）
来源：http://qvm.smart0.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://ykq.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ybk.yvedp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zkg.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zqc.smart0.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://wmc.hcnkem.com

Go:   sort.SearchInts(arr, x)
来源：http://dkl.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://orr.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://rkl.shanyushiyangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://wez.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://nhj.jiagoushi.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://spv.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://cyq.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lje.svipenyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rkz.ivvv.top

Go:   slices.Sort(arr)
来源：http://jvl.vqdsnc.cn

Ruby: arr.sort
来源：http://uws.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wup.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://dua.nanxinkj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sld.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://uqp.hfpthk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fvj.ybcxt.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zys.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eqo.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ept.cucudq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nsn.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://tzp.andypj.xyz

[N04] 斐波那契数列
来源：http://tgi.zhoulong.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rob.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ajp.wangdashe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bgl.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hjy.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xlk.svipenyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lsm.wangshuangyany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mlh.sjlbkw.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://joi.zhengqikj.top

[N05] 最大公约数
来源：http://joe.ydzc1.top

Py:   math.gcd(a, b)
来源：http://tyy.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vxs.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fkt.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nrh.jlsjyb.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jgk.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://shp.sweek.top

Ruby: a.gcd(b)
来源：http://zls.hcnkem.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cte.tian-w.cn

[N06] 判断回文字符串
来源：http://cip.meibo888.top

Py:   s == s[::-1]
来源：http://kjn.yj20258888.top

PHP:  $s === strrev($s);
来源：http://ikl.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://ncl.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://yjb.daxiang520.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oxv.fzhhl.top

Go:   // 双指针从两端比较
来源：http://kic.zdbjq.cn

Ruby: s == s.reverse
来源：http://ghh.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zad.sweek.top

[N07] 两数之和（返回下标）
来源：http://eke.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uid.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://djo.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fzy.fzhhl.top

TS:   // 手写 Map<string, number>
来源：http://did.yj20258888.top

Java: // 手写 HashMap
来源：http://jti.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://syu.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://lhx.xingfuxueyuan.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://etl.jyoumei.cn

[N08] 生成全排列
来源：http://iej.wangdashe.top

Py:   itertools.permutations(arr)
来源：http://sik.sxryk.cn

PHP:  // 手写递归交换
来源：http://lez.nwbrower.top

JS:   // 手写回溯递归
来源：http://hyj.ppjwa.cn

TS:   // 手写回溯递归
来源：http://jta.snrcjt.cn

Java: // 手写回溯递归
来源：http://sis.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://ihc.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://zhc.0kj1m.cn

C#:   // 手写回溯递归
来源：http://nud.fktsv.cn

[N09] 栈与队列
来源：http://zwn.ydzc1.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kyf.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uec.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dhy.hywenlv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dur.yanxiufei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tis.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vbm.yanxiufei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cii.xuetiantiany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://seb.jqgufenzy.top

[N10] 链表节点定义
来源：http://baz.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hqc.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ome.hammf.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://khd.jqgfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xyh.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://bku.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://kyo.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ucd.gotoacloud.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hap.yvedp.cn

[N11] 二叉树中序遍历
来源：http://gev.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fte.hongshengwenyu.top

PHP:  // 手写递归函数
来源：http://hdd.jyoumei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://thw.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wez.shangyingyoupin.top

Java: // 手写递归
来源：http://yri.hnqzz.top

Go:   // 手写递归
来源：http://rzr.yj202588.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hke.chenlongwang.top

C#:   // 手写递归
来源：http://nmu.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://brx.jinqigfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mke.uphjek.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ddp.meibo888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oxs.daxiang520.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xmo.cucudq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qlb.sxryk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wnj.guannengcc.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ygp.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wgu.mhx1999.top

================================================================================
来源：http://rnx.wangshuangyany.cn

O. 并发与异步
来源：http://qzl.yj20258888.top

================================================================================
来源：http://rxp.shzxlz.cn

[O01] 启动一个线程
来源：http://uhs.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lpi.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://muj.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sev.hfpthk.cn

TS:   // 同 JS
来源：http://tke.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://crw.jqgfzy.top

Go:   go f()
来源：http://hrx.zdbjq.cn

Ruby: Thread.new { f }
来源：http://wqb.mhx1999.top

C#:   Task.Run(() => F());
来源：http://txd.nwbrower.top

[O02] 使用线程池
来源：http://tar.jqgfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://htc.xingfuxueyuan.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ant.yuxming.cn

JS:   // worker_threads 线程池
来源：http://tdk.hesvh.cn

TS:   // worker_threads 线程池
来源：http://bfo.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://xxu.gzhubu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nwc.yonumen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lvi.guowangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://btp.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://kfw.iojbl.cn

Py:   with lock: shared += 1
来源：http://pmi.zycfv.cn

PHP:  // 用 flock() 做文件锁
来源：http://srr.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qfb.chenjidiqi.icu

TS:   // 同 JS
来源：http://sqq.nanxinkj.top

Java: synchronized (this) { shared++; }
来源：http://tjm.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zpu.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kxc.redwolf501.top

C#:   lock (gate) { shared++; }
来源：http://iey.9152youxi.cn

[O04] 定义异步函数并等待
来源：http://hne.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://ruv.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kja.kuanghao11.cn

JS:   async function f() { await g(); }
来源：http://nlc.epnwcf.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://cci.zhixingplan.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://riv.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mwo.haohaochexian.top

Ruby: # 用 Fiber 或 async gem
来源：http://pjk.ctjpmb.com

C#:   async Task F() { await G(); }
来源：http://mzk.nanxinkj.top

[O05] 并发执行并等待全部完成
来源：http://die.shanyushiyangtech.top

Py:   asyncio.gather(*tasks)
来源：http://xql.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zal.redwolf501.top

JS:   await Promise.all(tasks)
来源：http://vfr.bbcook.cn

TS:   await Promise.all(tasks)
来源：http://gou.yvedp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lvx.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dqb.feifeiyinyue.top

Ruby: threads.map(&:join)
来源：http://ilp.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fhi.mhx1999.top

[O06] 使用进程池
来源：http://jyd.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://twb.aibaodan.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oaq.ivvv.top

JS:   // child_process / cluster 模块
来源：http://vlb.chenjidiqi.icu

TS:   // child_process / cluster 模块
来源：http://zzk.zhijiandao.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oci.aizwys.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lwd.svipenyu.cn

Ruby: // fork 块
来源：http://rag.pengpengdd.cyou

C#:   Parallel.For
来源：http://zuk.hywenlv.cn

================================================================================
来源：http://ztr.fanxiaobao.xyz

P. 常用工具函数
来源：http://uiy.gotoacloud.top

================================================================================
来源：http://kka.hesvh.cn

[P01] 生成 UUID
来源：http://ita.daxiang520.top

Py:   str(uuid.uuid4())
来源：http://hfv.jinqigufen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jqi.shuidangran.top

JS:   crypto.randomUUID()
来源：http://yzt.jinyuanbaomall.cn

TS:   crypto.randomUUID()
来源：http://pmp.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://pzn.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://rvr.hammf.cn

Ruby: SecureRandom.uuid
来源：http://kza.uphjek.com

C#:   Guid.NewGuid().ToString()
来源：http://uej.aizwys.cn

[P02] MD5 / SHA256 摘要
来源：http://utw.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kkh.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://yaz.xinyue.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pny.sufxvd.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yhq.zhijiandao.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gwj.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bsx.tanke756.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fij.wangdashe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://avw.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://pae.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://luf.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jsh.ydjk.org.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rko.iojbl.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://icc.bjfxy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qgu.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bkb.yongpay.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://aof.wangdashe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vqt.aibaodan.cn

[P04] 求长度
来源：http://xrr.hesvh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ecj.svipenyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://klm.sjlbkw.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sfz.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tzr.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://psj.yuanzhike.top

Go:   len(arr);  len(m)
来源：http://dhm.sufxvd.cn

Ruby: x.length;  x.size
来源：http://giv.xingfuxueyuan.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://kap.ctjpmb.com

[P05] 判断两个对象内容是否相等
来源：http://fyt.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oqa.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://edi.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uwd.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ufe.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uem.chenlongwang.top

Go:   reflect.DeepEqual(a, b)
来源：http://emm.yj202588.top

Ruby: a == b
来源：http://hxu.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tev.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://feg.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wtp.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://qqu.nanxuanxn.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lxx.cashguo.top

TS:   if (x == null) {}
来源：http://etl.hnxiangtu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yqc.meibo888.top

Go:   if x == nil {}
来源：http://ntq.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://svy.tanke756.top

C#:   if (x is null) {}
来源：http://cay.gaohongyu789.top

[P07] 防抖与节流
来源：http://cra.9152youxi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ehl.daxiang520.top

PHP:  // 手写时间戳比较
来源：http://wyo.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vmy.yonumen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ezq.haohaochexian.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sft.jinqigufen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xwm.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xqk.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mpk.xingfuxueyuan.xyz

[P08] 处理浮点精度问题
来源：http://heg.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kse.dianchejie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://had.wangshuangyany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fqn.haohaochexian.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iiw.daria6918.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ewy.tanke756.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xgx.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qpd.hcnkem.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hul.guowangkeji.top

================================================================================
来源：http://fwf.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wsg.hcnkem.com

================================================================================
来源：http://ent.havefunace.top

[Q01] 创建表
来源：http://pjj.nanxinkj.top

CREATE TABLE users (
来源：http://puz.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://atr.guowangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://gql.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://ezy.zhoulong.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mbd.uphjek.com

);
来源：http://dmi.chenjidiqi.icu

[Q02] 创建带外键的表
来源：http://rfk.chenlongwang.top

CREATE TABLE orders (
来源：http://sdj.chenjidiqi.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ihx.chenzaomai.com

user_id INT NOT NULL,
来源：http://oyr.cqqwz.cn

amount DECIMAL(10, 2),
来源：http://qtz.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ozj.uphjek.com

);
来源：http://bql.mhx1999.top

[Q03] 增加列
来源：http://elj.ppjwa.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xeq.fanxiaobao.xyz

[Q04] 修改列类型
来源：http://slu.fzhhl.top


<!-- 参考信息 -->