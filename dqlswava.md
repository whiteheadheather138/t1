代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tjf.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bcc.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://khg.nanxinkj.top

C#:   Process.Start("ls", "-l");
来源：http://mou.jiagoushi.top

[M04] 获取当前工作目录
来源：http://sqd.haohaochexian.top

Py:   os.getcwd()
来源：http://jhf.yongpay.top

PHP:  getcwd();
来源：http://nbm.zhixingplan.top

JS:   process.cwd()
来源：http://ucv.jlsjyb.cn

TS:   process.cwd()
来源：http://dmb.daxiang520.top

Java: Path.of("").toAbsolutePath()
来源：http://pnh.meibo888.top

Go:   os.Getwd()
来源：http://uwk.chenzaomai.com

Ruby: Dir.pwd
来源：http://xtw.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://joc.yj20258888.top

[M05] 设置退出码
来源：http://rcc.hnqzz.top

Py:   sys.exit(1)
来源：http://vpj.zhaomingkeji.xyz

PHP:  exit(1);
来源：http://quc.sufxvd.cn

JS:   process.exit(1)
来源：http://rxb.aizwys.cn

TS:   process.exit(1)
来源：http://wib.xylfe.cn

Java: System.exit(1)
来源：http://rfa.zhongyouzk.top

Go:   os.Exit(1)
来源：http://mft.aibaodan.cn

Ruby: exit 1
来源：http://xwo.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://low.52xcode.cn

[M06] 向标准错误输出
来源：http://gfh.vqdsnc.cn

Py:   print("err", file=sys.stderr)
来源：http://qnd.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://iqv.hnqzz.top

JS:   console.error("err")
来源：http://swy.shuidangran.top

TS:   console.error("err")
来源：http://niv.tianlin.xyz

Java: System.err.println("err")
来源：http://bjv.xingfuxueyuan.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aci.yuanzhike.top

Ruby: warn "err"
来源：http://ggf.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://chm.guowangkeji.top

[M07] 判断是否为主入口
来源：http://wim.mhx1999.top

Py:   if __name__ == "__main__":
来源：http://jxi.zhengqikj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ptn.tian-w.cn

JS:   require.main === module
来源：http://pss.hnxiangtu.top

TS:   require.main === module
来源：http://rvi.smart0.xyz

Java: public static void main(String[] args)
来源：http://isz.guowangkeji.top

Go:   func main()
来源：http://qct.shangyingyoupin.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rny.yanxiufei.cn

C#:   static void Main(string[] args)
来源：http://hwr.zhoulong.xyz

[M08] 获取系统与运行时信息
来源：http://uym.zdbjq.cn

Py:   platform.system();  platform.python_version()
来源：http://gxx.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://diq.hnxiangtu.top

JS:   process.platform;  process.version
来源：http://sfe.aizwys.cn

TS:   process.platform;  process.version
来源：http://nhc.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://llo.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://wmk.daria6918.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bkq.vqdsnc.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://avd.yj20258888.top

================================================================================
来源：http://iou.zycfv.cn

N. 数据结构与算法
来源：http://tki.jinqigfzy.top

================================================================================
来源：http://grj.zhijiandao.cn

[N01] 二分查找（有序数组）
来源：http://jkp.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://nge.meibo888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lxn.fanxiaobao.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eyi.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zth.iojbl.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lvg.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://eic.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hhr.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hfu.gzhubu.top

[N02] 排序（工程实践用内置实现）
来源：http://beg.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://unv.snrcjt.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://est.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vxb.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kdk.316326.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vdy.xingfuxueyuan.xyz

Go:   slices.Sort(arr)
来源：http://fmz.aibaodan.cn

Ruby: arr.sort
来源：http://zus.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://sad.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://qac.zhijiandao.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lul.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://fkg.jinqigfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lyx.sweek.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wmz.jiagoushi.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wwn.jiagoushi.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://srp.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ffs.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://ljh.zhongyouzk.top

[N04] 斐波那契数列
来源：http://wiu.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gpn.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dao.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qpo.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://buv.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ukj.jlsjyb.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sre.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://odp.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nnn.gotoacloud.top

[N05] 最大公约数
来源：http://dfo.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://acv.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tcg.hfpthk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xuv.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yoo.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xzp.zhengqikj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vdy.zhoulong.xyz

Ruby: a.gcd(b)
来源：http://whp.aibaodan.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mtf.tian-w.cn

[N06] 判断回文字符串
来源：http://jag.cdnleiting.top

Py:   s == s[::-1]
来源：http://sfg.guannengcc.top

PHP:  $s === strrev($s);
来源：http://fmc.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://xkj.fengsongda.top

TS:   s === [...s].reverse().join("")
来源：http://ntp.xingfuxueyuan.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://axh.kuanghao11.cn

Go:   // 双指针从两端比较
来源：http://ysg.guannengcc.top

Ruby: s == s.reverse
来源：http://mou.zhijiandao.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qoz.zdbjq.cn

[N07] 两数之和（返回下标）
来源：http://gtr.cqqwz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jer.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tym.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ici.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://zbh.316326.xyz

Java: // 手写 HashMap
来源：http://vem.tianlin.xyz

Go:   // 手写 map[int]int
来源：http://npc.hywenlv.cn

Ruby: // 手写 Hash
来源：http://kjb.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://thg.jqgufenzy.top

[N08] 生成全排列
来源：http://mmw.yuanzhike.top

Py:   itertools.permutations(arr)
来源：http://euz.sweek.top

PHP:  // 手写递归交换
来源：http://vtw.chenzaomai.com

JS:   // 手写回溯递归
来源：http://sef.yj20258888.top

TS:   // 手写回溯递归
来源：http://nfm.ybcxt.top

Java: // 手写回溯递归
来源：http://wlu.tianlin.xyz

Go:   // 手写回溯递归
来源：http://ekw.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://jzi.nanxinkj.top

C#:   // 手写回溯递归
来源：http://gsi.meibo888.top

[N09] 栈与队列
来源：http://dvc.gogol.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wwm.yvedp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ztl.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jmk.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://roa.gotoacloud.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wfq.mhx1999.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uxa.yangfankeji.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gfr.zdqjudy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://umn.ybcxt.top

[N10] 链表节点定义
来源：http://jzt.cqqwz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://srz.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ody.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dbl.cashguo.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lhu.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://trz.zycfv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fco.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tkm.zhaomingkeji.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://orj.zdqjudy.top

[N11] 二叉树中序遍历
来源：http://zjj.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qeh.gotoacloud.top

PHP:  // 手写递归函数
来源：http://cvt.sysykeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://luf.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://scn.316326.xyz

Java: // 手写递归
来源：http://uom.chenlongwang.top

Go:   // 手写递归
来源：http://mly.sufxvd.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hpq.mhx1999.top

C#:   // 手写递归
来源：http://svo.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://szp.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ptv.sweek.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yzw.smart0.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gkt.yongpay.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pmv.zhongyouzk.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://leg.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xss.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://anv.bjfxy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fan.gogol.net.cn

================================================================================
来源：http://zuo.xylfe.cn

O. 并发与异步
来源：http://yhu.zdbjq.cn

================================================================================
来源：http://svp.zhijiandao.cn

[O01] 启动一个线程
来源：http://pap.ppjwa.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lgj.guannengcc.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gzk.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fai.uphjek.com

TS:   // 同 JS
来源：http://akq.chenzaomai.com

Java: new Thread(() -> f()).start()
来源：http://svy.yongpay.top

Go:   go f()
来源：http://tae.uphjek.com

Ruby: Thread.new { f }
来源：http://ric.wangdashe.top

C#:   Task.Run(() => F());
来源：http://syq.tarul.cn

[O02] 使用线程池
来源：http://paq.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zmw.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wjx.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://lci.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://yma.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://tfw.hongshengwenyu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bml.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ikz.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nuv.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://lmw.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://zci.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://ewd.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://coo.hesvh.cn

TS:   // 同 JS
来源：http://why.xziqi.cn

Java: synchronized (this) { shared++; }
来源：http://eif.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ixd.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bup.0kj1m.cn

C#:   lock (gate) { shared++; }
来源：http://fhw.ybcxt.top

[O04] 定义异步函数并等待
来源：http://kjc.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://tgt.jyoumei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qbi.tanke756.top

JS:   async function f() { await g(); }
来源：http://ufq.wangshuangyany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dww.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hie.jianghu66.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://irp.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://noe.zhengqikj.top

C#:   async Task F() { await G(); }
来源：http://xqz.redwolf501.top

[O05] 并发执行并等待全部完成
来源：http://ddf.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://klt.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sjg.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://idw.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://bwx.wangdashe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tkw.yfazqb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fpl.zhaomingkeji.xyz

Ruby: threads.map(&:join)
来源：http://mfz.meibo888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://skc.ppjwa.cn

[O06] 使用进程池
来源：http://syj.bjfxy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mey.fengsongda.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ecb.birdmap.top

JS:   // child_process / cluster 模块
来源：http://lyg.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://hgo.kuanghao11.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tsb.zhiwuduotai.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lqv.guannengcc.top

Ruby: // fork 块
来源：http://vpz.fzhhl.top

C#:   Parallel.For
来源：http://rbt.epnwcf.com

================================================================================
来源：http://qum.cheryme.top

P. 常用工具函数
来源：http://lwn.bbcook.cn

================================================================================
来源：http://juc.fzhhl.top

[P01] 生成 UUID
来源：http://dpa.yj20258888.top

Py:   str(uuid.uuid4())
来源：http://quv.pengpengdd.cyou

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rkj.fktsv.cn

JS:   crypto.randomUUID()
来源：http://eud.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://gwd.sweek.top

Java: UUID.randomUUID().toString()
来源：http://zju.tarul.cn

Go:   // 用 github.com/google/uuid
来源：http://qei.jqgfzy.top

Ruby: SecureRandom.uuid
来源：http://pwe.snrcjt.cn

C#:   Guid.NewGuid().ToString()
来源：http://gjv.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://gad.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zii.gogol.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uyu.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://erp.zhengqikj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qas.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://axr.yueranfly.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bez.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://utg.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rjk.chenjidiqi.icu

[P03] 生成短随机字符串
来源：http://ljq.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ptd.zhijiandao.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hwe.cqqwz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nyx.shzxlz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vjh.shangyingyoupin.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://trp.wangshuangyany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nve.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://flg.jqgfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oqy.mhx1999.top

[P04] 求长度
来源：http://bnu.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lqb.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nxv.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ncv.yuxming.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gal.xylfe.cn

Java: list.size();  map.size();  s.length()
来源：http://shq.gzhubu.top

Go:   len(arr);  len(m)
来源：http://jxx.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://lce.jinyuanbaomall.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ywy.shzxlz.cn

[P05] 判断两个对象内容是否相等
来源：http://kla.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mnh.bbcook.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ucg.pengpengdd.cyou

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bej.shangyingyoupin.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vlk.shanyushiyangtech.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aww.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://kbb.yvedp.cn

Ruby: a == b
来源：http://yyb.bbcook.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fgs.yuxming.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ygb.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mnj.dashuyun.cn

PHP:  if (empty($x)) {}
来源：http://tjh.redwolf501.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jxg.xziqi.cn

TS:   if (x == null) {}
来源：http://exc.aibaodan.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://avv.xylfe.cn

Go:   if x == nil {}
来源：http://uku.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fvv.ydjk.org.cn

C#:   if (x is null) {}
来源：http://ejw.uphjek.com

[P07] 防抖与节流
来源：http://nwo.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qjo.feifeiyinyue.top

PHP:  // 手写时间戳比较
来源：http://ypv.andypj.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wjp.fanxiaobao.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ppo.meibo888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oje.sysykeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jte.316326.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://weh.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ikz.tanke756.top

[P08] 处理浮点精度问题
来源：http://axq.guowangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nxz.wangshuangyany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://msq.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hso.fzhhl.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hxz.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bur.chenjidiqi.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kfe.jqgfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zbg.yangfankeji.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nai.cheryme.top

================================================================================
来源：http://yaa.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://otx.shanyushiyangtech.top

================================================================================
来源：http://lgs.snrcjt.cn

[Q01] 创建表
来源：http://qnn.sysykeji.top

CREATE TABLE users (
来源：http://laf.ehwqpu.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uil.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://yok.cucudq.cn

email VARCHAR(100) UNIQUE,
来源：http://rim.yj202588.top


<!-- 参考信息 -->