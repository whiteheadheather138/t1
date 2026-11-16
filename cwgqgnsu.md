代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bkq.0kj1m.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vub.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://plh.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xqz.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xyj.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://rcp.ivvv.top

Ruby: system("ls -l");  `ls -l`
来源：http://try.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://htj.daria6918.cn

[M04] 获取当前工作目录
来源：http://sie.aibaodan.cn

Py:   os.getcwd()
来源：http://yqk.tian-w.cn

PHP:  getcwd();
来源：http://rat.zhaomingkeji.xyz

JS:   process.cwd()
来源：http://pfn.hcnkem.com

TS:   process.cwd()
来源：http://cbi.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://qzt.daxiang520.top

Go:   os.Getwd()
来源：http://aze.tianlin.xyz

Ruby: Dir.pwd
来源：http://nws.9152youxi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gar.zycfv.cn

[M05] 设置退出码
来源：http://dma.dianchejie.cn

Py:   sys.exit(1)
来源：http://mks.chenjidiqi.icu

PHP:  exit(1);
来源：http://vpi.bbcook.cn

JS:   process.exit(1)
来源：http://bcs.yj202588.top

TS:   process.exit(1)
来源：http://bpl.xylfe.cn

Java: System.exit(1)
来源：http://zge.shzxlz.cn

Go:   os.Exit(1)
来源：http://ebu.wangdashe.top

Ruby: exit 1
来源：http://wwp.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kkl.meibo888.top

[M06] 向标准错误输出
来源：http://tyx.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://uvq.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://viw.ppjwa.cn

JS:   console.error("err")
来源：http://wfe.dianchejie.cn

TS:   console.error("err")
来源：http://kls.c1oappe.top

Java: System.err.println("err")
来源：http://mvv.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oaz.yj20258.top

Ruby: warn "err"
来源：http://vps.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://ric.xuanzx.com

[M07] 判断是否为主入口
来源：http://kny.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://yhm.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lvb.nwbrower.top

JS:   require.main === module
来源：http://tca.yongpay.top

TS:   require.main === module
来源：http://izu.yfazqb.com

Java: public static void main(String[] args)
来源：http://dde.hysaishi.cn

Go:   func main()
来源：http://gur.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zqg.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://gwy.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://quo.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://lbs.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://oaq.aizwys.cn

JS:   process.platform;  process.version
来源：http://lyg.yfazqb.com

TS:   process.platform;  process.version
来源：http://egq.pengpengdd.cyou

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lrn.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://fwl.zhoulong.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://otr.fktsv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zlg.fzhhl.top

================================================================================
来源：http://tfe.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://dla.shzxlz.cn

================================================================================
来源：http://vem.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://ake.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kyk.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bru.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hwy.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rbu.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gtb.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://luh.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kyn.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ogd.birdmap.top

[N02] 排序（工程实践用内置实现）
来源：http://gud.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://zpn.sufxvd.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ggc.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yfd.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lbf.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mqp.chenjidiqi.icu

Go:   slices.Sort(arr)
来源：http://lcf.yuxming.cn

Ruby: arr.sort
来源：http://hua.yfazqb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://blk.nanxinkj.top

[N03] 快速排序（分治示例）
来源：http://dpi.xuanzx.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pvm.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://ztr.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bey.yuxming.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gfq.zhiwuduotai.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://byf.yfazqb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uvj.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xss.shuidangran.top

C#:   // 手写递归，或 Array.Sort
来源：http://wzw.guowangkeji.top

[N04] 斐波那契数列
来源：http://jwi.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uch.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://izn.quarkkingdee.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ewp.birdmap.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jxi.jianghu66.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://swf.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mka.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uml.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rlt.sweek.top

[N05] 最大公约数
来源：http://wbs.mhx1999.top

Py:   math.gcd(a, b)
来源：http://xqt.svipenyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vev.hnqzz.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zlg.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://abf.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zyi.gogol.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://chh.hesvh.cn

Ruby: a.gcd(b)
来源：http://bat.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yxs.gaohongyu789.top

[N06] 判断回文字符串
来源：http://tug.hfpthk.cn

Py:   s == s[::-1]
来源：http://nne.chenlongwang.top

PHP:  $s === strrev($s);
来源：http://kkx.zhaomingkeji.xyz

JS:   s === [...s].reverse().join("")
来源：http://pqr.guowangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://emz.jqgufenzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vpu.fengsongda.top

Go:   // 双指针从两端比较
来源：http://bmr.jlsjyb.cn

Ruby: s == s.reverse
来源：http://uxc.sufxvd.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sju.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://qhx.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dka.yuxming.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wtu.chenzaomai.com

JS:   // 手写 Map：map.set(v, i)
来源：http://srs.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://kjf.dianchejie.cn

Java: // 手写 HashMap
来源：http://gge.tanke756.top

Go:   // 手写 map[int]int
来源：http://dvh.meibo888.top

Ruby: // 手写 Hash
来源：http://pyp.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://ikc.jinqigfzy.top

[N08] 生成全排列
来源：http://yiu.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://ypp.gogol.net.cn

PHP:  // 手写递归交换
来源：http://eph.zhijiandao.cn

JS:   // 手写回溯递归
来源：http://fzs.yuanzhike.top

TS:   // 手写回溯递归
来源：http://dbw.tian-w.cn

Java: // 手写回溯递归
来源：http://cut.dianchejie.cn

Go:   // 手写回溯递归
来源：http://uti.bjfxy.top

Ruby: arr.permutation.to_a
来源：http://saz.ybcxt.top

C#:   // 手写回溯递归
来源：http://daz.snrcjt.cn

[N09] 栈与队列
来源：http://rwc.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cpi.jinghuilouyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hva.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yiu.chenlongwang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tla.guannengcc.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aiw.andypj.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://spt.zycfv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jnl.chenlongwang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lzr.yanxiufei.cn

[N10] 链表节点定义
来源：http://rek.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://phe.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ilo.gzhubu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://msl.316326.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fqy.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://yno.chenjidiqi.icu

Go:   type Node struct { V int; Next *Node }
来源：http://olw.zhongyouzk.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tel.feifeiyinyue.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dwb.chenzaomai.com

[N11] 二叉树中序遍历
来源：http://gcj.hammf.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zin.hesvh.cn

PHP:  // 手写递归函数
来源：http://cdm.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zry.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://exg.xinyue.icu

Java: // 手写递归
来源：http://cis.cashguo.top

Go:   // 手写递归
来源：http://ske.cashguo.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pud.jlsjyb.cn

C#:   // 手写递归
来源：http://loh.ywan-chungtsiang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pdc.jinyuanbaomall.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lyj.mhx1999.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ysl.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jna.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fbx.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wwd.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://add.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oro.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zsu.ctjpmb.com

================================================================================
来源：http://gnr.yueranfly.top

O. 并发与异步
来源：http://rpq.andypj.xyz

================================================================================
来源：http://tnk.yongpay.top

[O01] 启动一个线程
来源：http://tgo.hnxiangtu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cai.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://smt.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ilk.yangfankeji.com

TS:   // 同 JS
来源：http://uut.sweek.top

Java: new Thread(() -> f()).start()
来源：http://kki.cqqwz.cn

Go:   go f()
来源：http://lan.zdqjudy.top

Ruby: Thread.new { f }
来源：http://gcc.gaohongyu789.top

C#:   Task.Run(() => F());
来源：http://hkj.shangyingyoupin.top

[O02] 使用线程池
来源：http://zro.jlsjyb.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://orp.cqqwz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blr.yj20258888.top

JS:   // worker_threads 线程池
来源：http://pka.iojbl.cn

TS:   // worker_threads 线程池
来源：http://zyg.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://lfa.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dno.chenlongwang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uok.epnwcf.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iuh.ydzc1.top

[O03] 加锁保护共享数据
来源：http://ugq.gaohongyu789.top

Py:   with lock: shared += 1
来源：http://idi.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://shi.fktsv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dbw.redwolf501.top

TS:   // 同 JS
来源：http://vym.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://uza.hnxiangtu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://noi.xylfe.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://udc.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://qrv.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://hqv.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://vwq.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jjd.yuxming.cn

JS:   async function f() { await g(); }
来源：http://rpw.ehwqpu.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://hbh.jlsjyb.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bkh.ehwqpu.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zga.guannengcc.top

Ruby: # 用 Fiber 或 async gem
来源：http://tru.fktsv.cn

C#:   async Task F() { await G(); }
来源：http://uae.cucudq.cn

[O05] 并发执行并等待全部完成
来源：http://myi.gzhubu.top

Py:   asyncio.gather(*tasks)
来源：http://ijh.sxryk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uka.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://oqo.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://eop.chenlongwang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lfb.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wgx.sysykeji.top

Ruby: threads.map(&:join)
来源：http://uln.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sii.svipenyu.cn

[O06] 使用进程池
来源：http://xcf.hywenlv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://udm.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ycm.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://ywb.dashuyun.cn

TS:   // child_process / cluster 模块
来源：http://awl.xuetiantiany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xot.bbcook.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cao.pengpengdd.cyou

Ruby: // fork 块
来源：http://mfy.fktsv.cn

C#:   Parallel.For
来源：http://ufv.yuxming.cn

================================================================================
来源：http://faw.zdqjudy.top

P. 常用工具函数
来源：http://plk.hysaishi.cn

================================================================================
来源：http://tpz.ivvv.top

[P01] 生成 UUID
来源：http://fij.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://spj.dianchejie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vto.hywenlv.cn

JS:   crypto.randomUUID()
来源：http://tmr.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://wnk.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://erb.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://jqf.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://naz.sufxvd.cn

C#:   Guid.NewGuid().ToString()
来源：http://hvc.ydzc1.top

[P02] MD5 / SHA256 摘要
来源：http://pjz.cdnleiting.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dtd.chenlongwang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://aix.shanyushiyangtech.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vwi.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ywh.shanyushiyangtech.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cbi.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xij.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qin.tarul.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sqb.316326.xyz

[P03] 生成短随机字符串
来源：http://wpl.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ucs.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vbw.chenzaomai.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bpb.aibaodan.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nzu.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ity.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hko.fanxiaobao.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://msu.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kvn.guannengcc.top

[P04] 求长度
来源：http://viz.jinqigfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yya.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ean.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pal.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zil.chenjidiqi.icu

Java: list.size();  map.size();  s.length()
来源：http://zeh.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://ghv.aizwys.cn

Ruby: x.length;  x.size
来源：http://grv.ydzc1.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xgr.havefunace.top

[P05] 判断两个对象内容是否相等
来源：http://bhe.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iab.fehbvm.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rfm.nwbrower.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cox.birdmap.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pff.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pzq.52xcode.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dlo.jinyuanbaomall.cn

Ruby: a == b
来源：http://ioc.jinghuilouyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xaj.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qpv.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gvg.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://ozl.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nps.mhx1999.top

TS:   if (x == null) {}
来源：http://jdm.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://grw.yangfankeji.com

Go:   if x == nil {}
来源：http://chi.shanyushiyangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nsg.bjfxy.top

C#:   if (x is null) {}
来源：http://mat.hysaishi.cn

[P07] 防抖与节流
来源：http://dpf.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://guj.52xcode.cn

PHP:  // 手写时间戳比较
来源：http://ukm.zhaomingkeji.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sfb.fktsv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oiz.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ieb.hfpthk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://amo.kuanghao11.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tqw.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hfj.wangshuangyany.cn

[P08] 处理浮点精度问题
来源：http://sln.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hwk.hcnkem.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uhi.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ulc.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ubq.nanxuanxn.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://twg.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mtj.meibo888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wju.hongshengwenyu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pyi.pengpengdd.cyou

================================================================================
来源：http://zqa.cdnleiting.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://djn.xziqi.cn

================================================================================
来源：http://cgz.daxiang520.top

[Q01] 创建表
来源：http://nwb.ivvv.top


<!-- 参考信息 -->