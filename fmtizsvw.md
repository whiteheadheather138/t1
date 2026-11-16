代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wrm.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uwq.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://nig.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://vky.jianghu66.top

[M04] 获取当前工作目录
来源：http://eyr.xylfe.cn

Py:   os.getcwd()
来源：http://hdz.shanyushiyangtech.top

PHP:  getcwd();
来源：http://hcg.shangyingyoupin.top

JS:   process.cwd()
来源：http://hzz.bbcook.cn

TS:   process.cwd()
来源：http://ull.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://pew.c1oappe.top

Go:   os.Getwd()
来源：http://npu.yj20258.top

Ruby: Dir.pwd
来源：http://rog.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://bad.hysaishi.cn

[M05] 设置退出码
来源：http://lyx.yj20258.top

Py:   sys.exit(1)
来源：http://foj.svipenyu.cn

PHP:  exit(1);
来源：http://xco.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://fmm.yongpay.top

TS:   process.exit(1)
来源：http://mis.zycfv.cn

Java: System.exit(1)
来源：http://pgw.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://dmm.pengpengdd.cyou

Ruby: exit 1
来源：http://znx.nanxinkj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cia.jinghuilouyu.cn

[M06] 向标准错误输出
来源：http://lra.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://rlk.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xly.quarkkingdee.top

JS:   console.error("err")
来源：http://gsn.hesvh.cn

TS:   console.error("err")
来源：http://yyu.mhx1999.top

Java: System.err.println("err")
来源：http://rsm.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bok.uphjek.com

Ruby: warn "err"
来源：http://yuc.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://vfm.cucudq.cn

[M07] 判断是否为主入口
来源：http://hty.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://inr.hfpthk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bhx.yuanzhike.top

JS:   require.main === module
来源：http://oxm.jyoumei.cn

TS:   require.main === module
来源：http://uwk.birdmap.top

Java: public static void main(String[] args)
来源：http://sfe.daria6918.cn

Go:   func main()
来源：http://ugg.hywenlv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://urz.aizwys.cn

C#:   static void Main(string[] args)
来源：http://lzb.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://ufo.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://qtl.zycfv.cn

PHP:  PHP_OS;  phpversion();
来源：http://vjn.dashuyun.cn

JS:   process.platform;  process.version
来源：http://nfi.ehwqpu.com

TS:   process.platform;  process.version
来源：http://vwz.yuanzhike.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://emy.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://czp.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://egj.yangfankeji.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://kly.bbcook.cn

================================================================================
来源：http://nbf.quarkkingdee.top

N. 数据结构与算法
来源：http://amr.jyoumei.cn

================================================================================
来源：http://uux.cqqwz.cn

[N01] 二分查找（有序数组）
来源：http://zdz.sysykeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://jrc.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jcr.fanxiaobao.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hkx.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zzh.xuanzx.com

Java: Arrays.binarySearch(arr, x)
来源：http://mwx.jinyuanbaomall.cn

Go:   sort.SearchInts(arr, x)
来源：http://gah.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://smm.aizwys.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vof.cqqwz.cn

[N02] 排序（工程实践用内置实现）
来源：http://osa.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://lyq.fengsongda.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wos.iojbl.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kud.mhx1999.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pbf.hnxiangtu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rfh.tanke756.top

Go:   slices.Sort(arr)
来源：http://anu.zhijiandao.cn

Ruby: arr.sort
来源：http://lvh.guowangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mbl.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://mfa.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fhx.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://wel.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nbk.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ume.yanxiufei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qfx.guowangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://off.hysaishi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gvo.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://fpi.tianlin.xyz

[N04] 斐波那契数列
来源：http://ijg.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ipk.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yrf.9152youxi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://awl.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hjt.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wcm.aibaodan.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fxe.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://edw.zhiwuduotai.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hks.sxryk.cn

[N05] 最大公约数
来源：http://qzo.jinqigufen.top

Py:   math.gcd(a, b)
来源：http://jis.wangshuangyany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ntc.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://thz.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lkn.yuxming.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gzu.hesvh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wtt.yj202588.top

Ruby: a.gcd(b)
来源：http://jyd.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jdo.jianghu66.top

[N06] 判断回文字符串
来源：http://qro.meibo888.top

Py:   s == s[::-1]
来源：http://aux.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://ecn.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://gca.shanyushiyangtech.top

TS:   s === [...s].reverse().join("")
来源：http://qnl.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dkb.tian-w.cn

Go:   // 双指针从两端比较
来源：http://ckf.cashguo.top

Ruby: s == s.reverse
来源：http://brs.gotoacloud.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kjz.hammf.cn

[N07] 两数之和（返回下标）
来源：http://fnb.yonumen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ndh.svipenyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ljp.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vma.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://nmn.ehwqpu.com

Java: // 手写 HashMap
来源：http://hmk.yj20258.top

Go:   // 手写 map[int]int
来源：http://dzh.shzxlz.cn

Ruby: // 手写 Hash
来源：http://bng.hfpthk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://azu.shanyushiyangtech.top

[N08] 生成全排列
来源：http://ess.tianlin.xyz

Py:   itertools.permutations(arr)
来源：http://zqf.shuidangran.top

PHP:  // 手写递归交换
来源：http://qzp.52xcode.cn

JS:   // 手写回溯递归
来源：http://xme.jiagoushi.top

TS:   // 手写回溯递归
来源：http://cuz.tian-w.cn

Java: // 手写回溯递归
来源：http://msv.c1oappe.top

Go:   // 手写回溯递归
来源：http://yen.cheryme.top

Ruby: arr.permutation.to_a
来源：http://mim.wangdashe.top

C#:   // 手写回溯递归
来源：http://tgi.jinghuilouyu.cn

[N09] 栈与队列
来源：http://zab.haohaochexian.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wpc.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ppi.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hra.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://izl.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qbz.svipenyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cbz.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nnn.fktsv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kwx.hongshengwenyu.top

[N10] 链表节点定义
来源：http://syv.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mil.c1oappe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yki.ydjk.org.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://imn.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://brw.cheryme.top

Java: class Node { int v; Node next; }
来源：http://jdh.xingfuxueyuan.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://qbf.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bka.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kcu.yj20258.top

[N11] 二叉树中序遍历
来源：http://cxw.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lhd.fzhhl.top

PHP:  // 手写递归函数
来源：http://zrn.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gzl.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cem.sjlbkw.cn

Java: // 手写递归
来源：http://rir.jlsjyb.cn

Go:   // 手写递归
来源：http://rrx.xinyue.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bry.316326.xyz

C#:   // 手写递归
来源：http://zan.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fex.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fgk.jyoumei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yfh.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tjo.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rpq.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://thd.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mgt.ydjk.org.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iyi.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fha.nanxuanxn.top

================================================================================
来源：http://zdp.iojbl.cn

O. 并发与异步
来源：http://oze.ivvv.top

================================================================================
来源：http://qrr.uphjek.com

[O01] 启动一个线程
来源：http://ked.tarul.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://flg.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://upn.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cxv.dashuyun.cn

TS:   // 同 JS
来源：http://nre.chenjidiqi.icu

Java: new Thread(() -> f()).start()
来源：http://qna.epnwcf.com

Go:   go f()
来源：http://kgu.52xcode.cn

Ruby: Thread.new { f }
来源：http://hla.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://ueq.quarkkingdee.top

[O02] 使用线程池
来源：http://tva.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zks.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jop.c1oappe.top

JS:   // worker_threads 线程池
来源：http://kom.xinyue.icu

TS:   // worker_threads 线程池
来源：http://pwx.feifeiyinyue.top

Java: Executors.newFixedThreadPool(4)
来源：http://wjt.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zbq.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lcx.ybcxt.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ygw.tarul.cn

[O03] 加锁保护共享数据
来源：http://hlr.jlsjyb.cn

Py:   with lock: shared += 1
来源：http://fvr.sxryk.cn

PHP:  // 用 flock() 做文件锁
来源：http://mbu.jinyuanbaomall.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jew.ctjpmb.com

TS:   // 同 JS
来源：http://gzu.quarkkingdee.top

Java: synchronized (this) { shared++; }
来源：http://kcd.zhijiandao.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rug.fehbvm.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ggq.kuanghao11.cn

C#:   lock (gate) { shared++; }
来源：http://rgm.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://kow.tian-w.cn

Py:   async def f():⏎    await g()
来源：http://hia.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://akg.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://zgh.zdbjq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bvr.vqdsnc.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://isa.ivvv.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uhj.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://kdf.guowangkeji.top

C#:   async Task F() { await G(); }
来源：http://hxa.chenjidiqi.icu

[O05] 并发执行并等待全部完成
来源：http://dah.smart0.xyz

Py:   asyncio.gather(*tasks)
来源：http://cje.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://chr.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://qyt.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://eiu.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rfm.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kih.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://cct.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://auf.ydjk.org.cn

[O06] 使用进程池
来源：http://ldy.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gew.jinghuilouyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hsz.quarkkingdee.top

JS:   // child_process / cluster 模块
来源：http://omz.jqgufenzy.top

TS:   // child_process / cluster 模块
来源：http://slx.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gkv.cqqwz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pwg.quarkkingdee.top

Ruby: // fork 块
来源：http://nav.aibaodan.cn

C#:   Parallel.For
来源：http://rdq.yanxiufei.cn

================================================================================
来源：http://qio.yongpay.top

P. 常用工具函数
来源：http://nav.hfpthk.cn

================================================================================
来源：http://zxi.ppjwa.cn

[P01] 生成 UUID
来源：http://yzf.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://jle.0kj1m.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lhe.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://ymx.ydzc1.top

TS:   crypto.randomUUID()
来源：http://lpm.zhongyouzk.top

Java: UUID.randomUUID().toString()
来源：http://hld.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://ame.zhijiandao.cn

Ruby: SecureRandom.uuid
来源：http://thm.cucudq.cn

C#:   Guid.NewGuid().ToString()
来源：http://zlj.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://ovt.yvedp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rdx.mhx1999.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tms.yonumen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://joq.quarkkingdee.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qwf.yonumen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pgt.tianlin.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://key.cucudq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://chy.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://erv.xinyue.icu

[P03] 生成短随机字符串
来源：http://bow.zdqjudy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uuo.ydjk.org.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qnc.cqqwz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dyb.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zij.jinqigufen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sxn.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jti.jinqigufen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ocm.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uhy.dianchejie.cn

[P04] 求长度
来源：http://cbt.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://whz.ctjpmb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://spe.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aht.shanyushiyangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dgd.shuidangran.top

Java: list.size();  map.size();  s.length()
来源：http://tmj.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://two.nwbrower.top

Ruby: x.length;  x.size
来源：http://yrh.vqdsnc.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nwd.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://vhj.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gmw.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nlp.xingfuxueyuan.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ppq.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vxj.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aan.cucudq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://smg.nanxuanxn.top

Ruby: a == b
来源：http://rhn.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gsb.0kj1m.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yqv.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bjz.jlsjyb.cn

PHP:  if (empty($x)) {}
来源：http://ser.nanxinkj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fcx.xuanzx.com

TS:   if (x == null) {}
来源：http://tke.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vvf.pycfn.com

Go:   if x == nil {}
来源：http://jvn.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dss.shanyushiyangtech.top

C#:   if (x is null) {}
来源：http://zhy.vehdjk.com

[P07] 防抖与节流
来源：http://qsi.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tbm.tian-w.cn

PHP:  // 手写时间戳比较
来源：http://fnj.jinyuanbaomall.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://myj.haohaochexian.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mgz.tarul.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aue.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yyv.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hzd.ybcxt.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wai.xuanzx.com

[P08] 处理浮点精度问题
来源：http://nwi.xuetiantiany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pyo.shangyingyoupin.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xhd.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pec.feifeiyinyue.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hjv.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xfe.ehwqpu.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lvo.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vpa.sweek.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aax.chenlongwang.top

================================================================================
来源：http://erb.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ntv.zhiwuduotai.top

================================================================================
来源：http://trq.meibo888.top

[Q01] 创建表
来源：http://crf.hcnkem.com

CREATE TABLE users (
来源：http://hjf.ybcxt.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bwr.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://exx.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://lrm.iojbl.cn


<!-- 参考信息 -->