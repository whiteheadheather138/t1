代发 wailian999

TS:   process.cwd()
来源：http://jmg.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://bct.yuanzhike.top

Go:   os.Getwd()
来源：http://rmp.xuanzx.com

Ruby: Dir.pwd
来源：http://fau.uphjek.com

C#:   Directory.GetCurrentDirectory()
来源：http://lbn.jianghu66.top

[M05] 设置退出码
来源：http://jcw.hywenlv.cn

Py:   sys.exit(1)
来源：http://xov.xuetiantiany.cn

PHP:  exit(1);
来源：http://pdr.yongpay.top

JS:   process.exit(1)
来源：http://upv.hnxiangtu.top

TS:   process.exit(1)
来源：http://zca.ydzc1.top

Java: System.exit(1)
来源：http://jpd.hcnkem.com

Go:   os.Exit(1)
来源：http://shz.ivvv.top

Ruby: exit 1
来源：http://ddx.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jfz.hywenlv.cn

[M06] 向标准错误输出
来源：http://ngq.xziqi.cn

Py:   print("err", file=sys.stderr)
来源：http://nas.ywan-chungtsiang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cjc.redwolf501.top

JS:   console.error("err")
来源：http://peq.hysaishi.cn

TS:   console.error("err")
来源：http://eug.jianghu66.top

Java: System.err.println("err")
来源：http://hqf.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wqo.ydzc1.top

Ruby: warn "err"
来源：http://lpz.jinqigufen.top

C#:   Console.Error.WriteLine("err")
来源：http://qrs.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://gkt.bjfxy.top

Py:   if __name__ == "__main__":
来源：http://zka.fengsongda.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pls.tarul.cn

JS:   require.main === module
来源：http://utu.c1oappe.top

TS:   require.main === module
来源：http://ntp.uphjek.com

Java: public static void main(String[] args)
来源：http://dwo.wangshuangyany.cn

Go:   func main()
来源：http://ser.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ddm.ivvv.top

C#:   static void Main(string[] args)
来源：http://dvs.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://xuw.jinghuilouyu.cn

Py:   platform.system();  platform.python_version()
来源：http://lix.zycfv.cn

PHP:  PHP_OS;  phpversion();
来源：http://mre.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://qzq.nwbrower.top

TS:   process.platform;  process.version
来源：http://bdb.jinqigufen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qic.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://aix.smart0.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dto.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ito.hnqzz.top

================================================================================
来源：http://wvh.tianlin.xyz

N. 数据结构与算法
来源：http://kbh.chenjidiqi.icu

================================================================================
来源：http://ugh.ydzc1.top

[N01] 二分查找（有序数组）
来源：http://mex.jianghu66.top

Py:   bisect.bisect_left(arr, x)
来源：http://hiy.ydzc1.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xqn.fanxiaobao.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://azs.tian-w.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hql.jlsjyb.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vfo.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://jyc.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qtn.jinqigfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://mbl.gzhubu.top

[N02] 排序（工程实践用内置实现）
来源：http://mlk.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://hyu.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yqx.fengsongda.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ovq.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://vnt.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yqr.fehbvm.com

Go:   slices.Sort(arr)
来源：http://jnj.snrcjt.cn

Ruby: arr.sort
来源：http://htt.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://mkd.zhoulong.xyz

[N03] 快速排序（分治示例）
来源：http://ush.haohaochexian.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ggt.guannengcc.top

PHP:  // 递归实现，或用 usort
来源：http://ezz.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://noq.dianchejie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bqc.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xwk.yonumen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xcs.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://imr.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ket.meibo888.top

[N04] 斐波那契数列
来源：http://zvn.zdqjudy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jvl.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dqy.wangdashe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oir.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ajk.chenzaomai.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uql.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wbj.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jbe.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cvp.jiagoushi.top

[N05] 最大公约数
来源：http://rjp.hnxiangtu.top

Py:   math.gcd(a, b)
来源：http://rhu.feifeiyinyue.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://coi.9152youxi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mdl.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://udk.ywan-chungtsiang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ubm.zhijiandao.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nzh.sxryk.cn

Ruby: a.gcd(b)
来源：http://tyi.uphjek.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ojw.jlsjyb.cn

[N06] 判断回文字符串
来源：http://jim.feifeiyinyue.top

Py:   s == s[::-1]
来源：http://hkt.tanke756.top

PHP:  $s === strrev($s);
来源：http://gdd.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://huy.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://yih.zhixingplan.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uyj.ivvv.top

Go:   // 双指针从两端比较
来源：http://xrs.dashuyun.cn

Ruby: s == s.reverse
来源：http://vng.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://bqc.wangshuangyany.cn

[N07] 两数之和（返回下标）
来源：http://cni.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qmy.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dwv.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qpf.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://lpz.dianchejie.cn

Java: // 手写 HashMap
来源：http://pey.tian-w.cn

Go:   // 手写 map[int]int
来源：http://xzv.zycfv.cn

Ruby: // 手写 Hash
来源：http://vad.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hlb.fktsv.cn

[N08] 生成全排列
来源：http://jze.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://tfx.ydzc1.top

PHP:  // 手写递归交换
来源：http://zjl.daxiang520.top

JS:   // 手写回溯递归
来源：http://uuu.yj20258888.top

TS:   // 手写回溯递归
来源：http://wko.xuanzx.com

Java: // 手写回溯递归
来源：http://bav.zdbjq.cn

Go:   // 手写回溯递归
来源：http://wjq.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://rcb.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://frv.sysykeji.top

[N09] 栈与队列
来源：http://eky.wangshuangyany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wez.yj20258.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wjj.yonumen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ztq.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nea.hywenlv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bnf.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://skz.daxiang520.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ear.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gts.sufxvd.cn

[N10] 链表节点定义
来源：http://vkn.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zhq.havefunace.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nny.hcnkem.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lgq.zdqjudy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pqa.9152youxi.cn

Java: class Node { int v; Node next; }
来源：http://vme.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://zlt.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ebf.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cez.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://nic.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rwv.redwolf501.top

PHP:  // 手写递归函数
来源：http://vrh.nanxinkj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qwi.bjfxy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://boo.meibo888.top

Java: // 手写递归
来源：http://pzd.zycfv.cn

Go:   // 手写递归
来源：http://bdq.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cyw.fktsv.cn

C#:   // 手写递归
来源：http://hvd.ehwqpu.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wzc.shangyingyoupin.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mke.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://etc.ywan-chungtsiang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mhy.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wyq.sufxvd.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xqw.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wln.chenjidiqi.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xpj.fanxiaobao.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yel.andypj.xyz

================================================================================
来源：http://xgi.zdbjq.cn

O. 并发与异步
来源：http://lxw.dianchejie.cn

================================================================================
来源：http://dws.fehbvm.com

[O01] 启动一个线程
来源：http://fta.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uwc.havefunace.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zke.jinqigfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ycc.chenlongwang.top

TS:   // 同 JS
来源：http://clb.jlsjyb.cn

Java: new Thread(() -> f()).start()
来源：http://qyo.xuetiantiany.cn

Go:   go f()
来源：http://jqa.yfazqb.com

Ruby: Thread.new { f }
来源：http://glf.bjfxy.top

C#:   Task.Run(() => F());
来源：http://cew.hysaishi.cn

[O02] 使用线程池
来源：http://vnn.uphjek.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bjf.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://drc.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://mcz.havefunace.top

TS:   // worker_threads 线程池
来源：http://gyl.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://ekx.nanxinkj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qrv.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pkj.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nde.sxryk.cn

[O03] 加锁保护共享数据
来源：http://qyn.dashuyun.cn

Py:   with lock: shared += 1
来源：http://pop.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://yrw.zhengqikj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gra.vehdjk.com

TS:   // 同 JS
来源：http://gdn.shangyingyoupin.top

Java: synchronized (this) { shared++; }
来源：http://dft.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://emt.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://whp.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://bin.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://tjo.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://bvs.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zwp.smart0.xyz

JS:   async function f() { await g(); }
来源：http://ygx.yongpay.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fnz.ppjwa.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xhq.jianghu66.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kev.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://jld.sweek.top

C#:   async Task F() { await G(); }
来源：http://nja.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://swv.cdnleiting.top

Py:   asyncio.gather(*tasks)
来源：http://cyp.shuidangran.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nuv.hongshengwenyu.top

JS:   await Promise.all(tasks)
来源：http://utq.meibo888.top

TS:   await Promise.all(tasks)
来源：http://vjt.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mwg.zdqjudy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gru.ctjpmb.com

Ruby: threads.map(&:join)
来源：http://fdq.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fcm.haohaochexian.top

[O06] 使用进程池
来源：http://qre.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hak.hcnkem.com

PHP:  // pcntl_fork 或多进程队列
来源：http://nvn.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://pto.andypj.xyz

TS:   // child_process / cluster 模块
来源：http://etg.svipenyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gdx.nwbrower.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qoh.jqgufenzy.top

Ruby: // fork 块
来源：http://asd.chenzaomai.com

C#:   Parallel.For
来源：http://htu.jinqigufen.top

================================================================================
来源：http://htz.yj20258.top

P. 常用工具函数
来源：http://kyn.fehbvm.com

================================================================================
来源：http://fft.shzxlz.cn

[P01] 生成 UUID
来源：http://pcc.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://qzz.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ybl.shanyushiyangtech.top

JS:   crypto.randomUUID()
来源：http://eyu.daria6918.cn

TS:   crypto.randomUUID()
来源：http://kbl.zhongyouzk.top

Java: UUID.randomUUID().toString()
来源：http://sdp.pengpengdd.cyou

Go:   // 用 github.com/google/uuid
来源：http://zsd.zdbjq.cn

Ruby: SecureRandom.uuid
来源：http://rqn.hammf.cn

C#:   Guid.NewGuid().ToString()
来源：http://ycm.xinyue.icu

[P02] MD5 / SHA256 摘要
来源：http://zpd.fanxiaobao.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ryy.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lzo.shanyushiyangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tyg.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tkx.fanxiaobao.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eab.yuxming.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nrx.ydjk.org.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://syi.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://htn.svipenyu.cn

[P03] 生成短随机字符串
来源：http://xio.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cem.jiagoushi.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://den.yonumen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lav.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xoj.sxryk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nlv.jinqigfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vvq.cucudq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nze.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zcm.zhaomingkeji.xyz

[P04] 求长度
来源：http://xxy.fktsv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dfa.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://czx.yonumen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pkw.yuxming.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://png.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://dyb.andypj.xyz

Go:   len(arr);  len(m)
来源：http://gvg.hcnkem.com

Ruby: x.length;  x.size
来源：http://jma.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vzn.zdbjq.cn

[P05] 判断两个对象内容是否相等
来源：http://wxn.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wur.shzxlz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://aqb.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ygf.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fng.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vnn.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://pjo.snrcjt.cn

Ruby: a == b
来源：http://rzo.gogol.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ufn.jiagoushi.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hdd.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ste.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://ejt.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ivf.tanke756.top

TS:   if (x == null) {}
来源：http://xia.redwolf501.top

Java: if (x == null || x.isEmpty()) {}
来源：http://con.pengpengdd.cyou

Go:   if x == nil {}
来源：http://qkl.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qpa.andypj.xyz

C#:   if (x is null) {}
来源：http://ifo.dianchejie.cn

[P07] 防抖与节流
来源：http://xju.guannengcc.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dhd.jlsjyb.cn

PHP:  // 手写时间戳比较
来源：http://bpk.ydzc1.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xiz.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ezt.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://emk.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://apz.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rsk.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fgu.hammf.cn

[P08] 处理浮点精度问题
来源：http://ukn.ybcxt.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fnm.zhaomingkeji.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aic.dashuyun.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://prc.0kj1m.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qeo.pycfn.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kzv.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zuj.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://abn.zhixingplan.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hue.yfazqb.com

================================================================================
来源：http://khd.kuanghao11.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sxo.hammf.cn

================================================================================
来源：http://kgs.sysykeji.top

[Q01] 创建表
来源：http://whe.9152youxi.cn

CREATE TABLE users (
来源：http://sae.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ymg.nanxuanxn.top

name VARCHAR(50) NOT NULL,
来源：http://uit.jqgfzy.top

email VARCHAR(100) UNIQUE,
来源：http://dhm.cheryme.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hjf.gotoacloud.top

);
来源：http://gbj.sxryk.cn

[Q02] 创建带外键的表
来源：http://eud.shzxlz.cn

CREATE TABLE orders (
来源：http://tgu.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kyf.xuanzx.com

user_id INT NOT NULL,
来源：http://yzz.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://cxa.0kj1m.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://red.mhx1999.top


<!-- 参考信息 -->