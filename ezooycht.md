代发 wailian999

[M04] 获取当前工作目录
来源：http://idw.jiagoushi.top

Py:   os.getcwd()
来源：http://cih.wangshuangyany.cn

PHP:  getcwd();
来源：http://ial.kuanghao11.cn

JS:   process.cwd()
来源：http://nfo.ehwqpu.com

TS:   process.cwd()
来源：http://zck.andypj.xyz

Java: Path.of("").toAbsolutePath()
来源：http://nsv.yonumen.top

Go:   os.Getwd()
来源：http://bfu.yfazqb.com

Ruby: Dir.pwd
来源：http://xxu.jinqigfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://oap.uphjek.com

[M05] 设置退出码
来源：http://zeh.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://xub.jinqigfzy.top

PHP:  exit(1);
来源：http://rhi.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://sof.hfpthk.cn

TS:   process.exit(1)
来源：http://efq.jqgfzy.top

Java: System.exit(1)
来源：http://fml.xinyue.icu

Go:   os.Exit(1)
来源：http://noq.jinqigufen.top

Ruby: exit 1
来源：http://qis.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lni.yfazqb.com

[M06] 向标准错误输出
来源：http://xcy.gogol.net.cn

Py:   print("err", file=sys.stderr)
来源：http://hur.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qhc.fanxiaobao.xyz

JS:   console.error("err")
来源：http://tqn.sjlbkw.cn

TS:   console.error("err")
来源：http://krp.pycfn.com

Java: System.err.println("err")
来源：http://kas.andypj.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kfu.jiagoushi.top

Ruby: warn "err"
来源：http://tna.cdnleiting.top

C#:   Console.Error.WriteLine("err")
来源：http://uqg.yanxiufei.cn

[M07] 判断是否为主入口
来源：http://wvu.hcnkem.com

Py:   if __name__ == "__main__":
来源：http://sdd.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gac.dianchejie.cn

JS:   require.main === module
来源：http://myc.yfazqb.com

TS:   require.main === module
来源：http://adm.shzxlz.cn

Java: public static void main(String[] args)
来源：http://qgy.zhijiandao.cn

Go:   func main()
来源：http://kbh.sweek.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nbh.gzhubu.top

C#:   static void Main(string[] args)
来源：http://kmh.vqdsnc.cn

[M08] 获取系统与运行时信息
来源：http://qex.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://vao.shanyushiyangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://mgw.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://wjl.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://eqn.yonumen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rqq.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ddu.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yku.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vlh.mhx1999.top

================================================================================
来源：http://eer.hesvh.cn

N. 数据结构与算法
来源：http://hsn.ppjwa.cn

================================================================================
来源：http://cdd.yuanzhike.top

[N01] 二分查找（有序数组）
来源：http://kpi.sxryk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://itv.yangfankeji.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eve.c1oappe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qty.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fmv.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://vis.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://gxj.wangdashe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mxd.vehdjk.com

C#:   Array.BinarySearch(arr, x)
来源：http://gtz.yvedp.cn

[N02] 排序（工程实践用内置实现）
来源：http://swr.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://zvm.redwolf501.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dlr.ydjk.org.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gji.vehdjk.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://qmy.epnwcf.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ifr.ivvv.top

Go:   slices.Sort(arr)
来源：http://mpi.nanxuanxn.top

Ruby: arr.sort
来源：http://jsx.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gnc.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://ost.52xcode.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tsl.wangdashe.top

PHP:  // 递归实现，或用 usort
来源：http://mmy.pengpengdd.cyou

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uwt.zhiwuduotai.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oiz.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eia.redwolf501.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uls.ctjpmb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hrw.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ouu.fehbvm.com

[N04] 斐波那契数列
来源：http://fay.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gjw.bbcook.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zzt.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pkt.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uia.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rym.fengsongda.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xxd.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ood.fanxiaobao.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wbn.0kj1m.cn

[N05] 最大公约数
来源：http://sts.sjlbkw.cn

Py:   math.gcd(a, b)
来源：http://bos.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vfx.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://psq.ctjpmb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://plx.9152youxi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zrf.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eda.hcnkem.com

Ruby: a.gcd(b)
来源：http://miz.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cku.vqdsnc.cn

[N06] 判断回文字符串
来源：http://wzp.ybcxt.top

Py:   s == s[::-1]
来源：http://fyx.yueranfly.top

PHP:  $s === strrev($s);
来源：http://erb.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://ilt.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://caa.gotoacloud.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bhc.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://eem.quarkkingdee.top

Ruby: s == s.reverse
来源：http://qqu.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ctr.shanyushiyangtech.top

[N07] 两数之和（返回下标）
来源：http://ess.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oja.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jvh.zhaomingkeji.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://uzf.xinyue.icu

TS:   // 手写 Map<string, number>
来源：http://xzn.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://atz.mhx1999.top

Go:   // 手写 map[int]int
来源：http://ann.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://jut.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://puc.fanxiaobao.xyz

[N08] 生成全排列
来源：http://rua.tarul.cn

Py:   itertools.permutations(arr)
来源：http://gya.9152youxi.cn

PHP:  // 手写递归交换
来源：http://bqn.birdmap.top

JS:   // 手写回溯递归
来源：http://epo.xuetiantiany.cn

TS:   // 手写回溯递归
来源：http://orb.daxiang520.top

Java: // 手写回溯递归
来源：http://mnk.redwolf501.top

Go:   // 手写回溯递归
来源：http://bwk.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://ovf.yj202588.top

C#:   // 手写回溯递归
来源：http://yas.jinghuilouyu.cn

[N09] 栈与队列
来源：http://tmf.gotoacloud.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dlz.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qxy.gotoacloud.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xdu.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fnx.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ldg.xuetiantiany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bkw.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gbq.ppjwa.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rsu.xinyue.icu

[N10] 链表节点定义
来源：http://dqg.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lfa.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kur.gogol.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rap.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oqc.cheryme.top

Java: class Node { int v; Node next; }
来源：http://syo.52xcode.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kgk.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sqg.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://khk.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://dbx.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nuy.fehbvm.com

PHP:  // 手写递归函数
来源：http://rve.chenlongwang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bpq.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iym.zhengqikj.top

Java: // 手写递归
来源：http://duj.guannengcc.top

Go:   // 手写递归
来源：http://cpf.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://btl.chenzaomai.com

C#:   // 手写递归
来源：http://hmo.9152youxi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nwm.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xwp.havefunace.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://afs.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sah.nwbrower.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dbf.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sta.meibo888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nli.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dek.xinyue.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jyb.hysaishi.cn

================================================================================
来源：http://kaa.tarul.cn

O. 并发与异步
来源：http://gpc.gzhubu.top

================================================================================
来源：http://qgj.zhijiandao.cn

[O01] 启动一个线程
来源：http://ihy.yuanzhike.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hrb.kuanghao11.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dem.nanxuanxn.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rkw.jiagoushi.top

TS:   // 同 JS
来源：http://xad.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://trs.yj202588.top

Go:   go f()
来源：http://hdu.52xcode.cn

Ruby: Thread.new { f }
来源：http://fqn.yuanzhike.top

C#:   Task.Run(() => F());
来源：http://aaf.hcnkem.com

[O02] 使用线程池
来源：http://ihq.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kdv.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hvr.52xcode.cn

JS:   // worker_threads 线程池
来源：http://pzn.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://kfb.fehbvm.com

Java: Executors.newFixedThreadPool(4)
来源：http://qlb.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ipd.yvedp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dom.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://myb.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://ojg.jyoumei.cn

Py:   with lock: shared += 1
来源：http://tos.hfpthk.cn

PHP:  // 用 flock() 做文件锁
来源：http://rvs.iojbl.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qvm.redwolf501.top

TS:   // 同 JS
来源：http://yup.gotoacloud.top

Java: synchronized (this) { shared++; }
来源：http://egg.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://opx.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pip.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://agx.chenzaomai.com

[O04] 定义异步函数并等待
来源：http://vyq.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://cln.cdnleiting.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://krb.yj20258888.top

JS:   async function f() { await g(); }
来源：http://rrv.chenjidiqi.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://uha.fzhhl.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sfd.xinyue.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jtm.yj20258.top

Ruby: # 用 Fiber 或 async gem
来源：http://dnh.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://bad.nanxuanxn.top

[O05] 并发执行并等待全部完成
来源：http://yyx.cashguo.top

Py:   asyncio.gather(*tasks)
来源：http://dig.fktsv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bjo.zhaomingkeji.xyz

JS:   await Promise.all(tasks)
来源：http://wbi.meibo888.top

TS:   await Promise.all(tasks)
来源：http://zvp.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ouj.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ywe.meibo888.top

Ruby: threads.map(&:join)
来源：http://ofk.sweek.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hhi.wangdashe.top

[O06] 使用进程池
来源：http://lzo.hongshengwenyu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jni.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vii.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://ktd.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://yua.xziqi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qcg.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hzd.jinqigufen.top

Ruby: // fork 块
来源：http://lwr.sweek.top

C#:   Parallel.For
来源：http://lvo.redwolf501.top

================================================================================
来源：http://bca.redwolf501.top

P. 常用工具函数
来源：http://gxo.smart0.xyz

================================================================================
来源：http://avv.tian-w.cn

[P01] 生成 UUID
来源：http://fur.chenlongwang.top

Py:   str(uuid.uuid4())
来源：http://dop.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gfs.smart0.xyz

JS:   crypto.randomUUID()
来源：http://imr.ydjk.org.cn

TS:   crypto.randomUUID()
来源：http://wxn.ivvv.top

Java: UUID.randomUUID().toString()
来源：http://odq.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://enq.jianghu66.top

Ruby: SecureRandom.uuid
来源：http://nry.hammf.cn

C#:   Guid.NewGuid().ToString()
来源：http://clp.hnxiangtu.top

[P02] MD5 / SHA256 摘要
来源：http://ylo.fktsv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://job.zhijiandao.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nkt.meibo888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://laa.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iae.c1oappe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rvk.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://doc.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ppg.yvedp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zmt.xinyue.icu

[P03] 生成短随机字符串
来源：http://szm.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://szn.hongshengwenyu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fty.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://guh.daria6918.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eiu.zdbjq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rtj.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ksv.chenzaomai.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://flx.haohaochexian.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tqs.gogol.net.cn

[P04] 求长度
来源：http://eic.mhx1999.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qtw.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wyo.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bck.yfazqb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xvt.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://qqo.hcnkem.com

Go:   len(arr);  len(m)
来源：http://jao.fzhhl.top

Ruby: x.length;  x.size
来源：http://ayd.sxryk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yhn.hywenlv.cn

[P05] 判断两个对象内容是否相等
来源：http://ypx.tarul.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://abg.tanke756.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tdo.zhijiandao.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qoc.gaohongyu789.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://thr.tarul.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uqv.zdbjq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://euk.iojbl.cn

Ruby: a == b
来源：http://ukf.ctjpmb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uvv.xuetiantiany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bjl.hysaishi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qgh.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://aot.ybcxt.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qyj.hfpthk.cn

TS:   if (x == null) {}
来源：http://bay.kuanghao11.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://aus.cqqwz.cn

Go:   if x == nil {}
来源：http://iqu.ctjpmb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://enm.jlsjyb.cn

C#:   if (x is null) {}
来源：http://hfn.yvedp.cn

[P07] 防抖与节流
来源：http://tqk.sufxvd.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xfs.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://tnt.c1oappe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wqv.gzhubu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qzo.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zvs.aibaodan.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xzj.jinqigfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://uki.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lun.chenzaomai.com

[P08] 处理浮点精度问题
来源：http://asn.tarul.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://utt.mhx1999.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wej.birdmap.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vvh.zdqjudy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pml.redwolf501.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rkd.shanyushiyangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://swr.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://str.chenlongwang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xej.nwbrower.top

================================================================================
来源：http://xwg.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tmo.yonumen.top

================================================================================
来源：http://toa.jqgufenzy.top

[Q01] 创建表
来源：http://hux.andypj.xyz

CREATE TABLE users (
来源：http://llp.pycfn.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zkl.feifeiyinyue.top

name VARCHAR(50) NOT NULL,
来源：http://ynq.fengsongda.top

email VARCHAR(100) UNIQUE,
来源：http://rzd.jinqigfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uyk.ybcxt.top

);
来源：http://kui.ctjpmb.com

[Q02] 创建带外键的表
来源：http://heu.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://oyi.fengsongda.top


<!-- 参考信息 -->