代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mts.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vjz.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://zwo.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://otm.jyoumei.cn

[M04] 获取当前工作目录
来源：http://lgi.ivvv.top

Py:   os.getcwd()
来源：http://zuf.jyoumei.cn

PHP:  getcwd();
来源：http://rpw.52xcode.cn

JS:   process.cwd()
来源：http://qrd.svipenyu.cn

TS:   process.cwd()
来源：http://mqv.hfpthk.cn

Java: Path.of("").toAbsolutePath()
来源：http://mxd.jianghu66.top

Go:   os.Getwd()
来源：http://yjc.yj20258.top

Ruby: Dir.pwd
来源：http://ypx.fehbvm.com

C#:   Directory.GetCurrentDirectory()
来源：http://tvi.guowangkeji.top

[M05] 设置退出码
来源：http://xjw.pengpengdd.cyou

Py:   sys.exit(1)
来源：http://mun.tian-w.cn

PHP:  exit(1);
来源：http://gwe.zhengqikj.top

JS:   process.exit(1)
来源：http://qlj.yuxming.cn

TS:   process.exit(1)
来源：http://wqt.ppjwa.cn

Java: System.exit(1)
来源：http://zzz.nwbrower.top

Go:   os.Exit(1)
来源：http://gpg.pycfn.com

Ruby: exit 1
来源：http://xfb.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://odc.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://vvn.svipenyu.cn

Py:   print("err", file=sys.stderr)
来源：http://fsy.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ocp.ppjwa.cn

JS:   console.error("err")
来源：http://ktm.daria6918.cn

TS:   console.error("err")
来源：http://nul.haohaochexian.top

Java: System.err.println("err")
来源：http://bct.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wzz.zhoulong.xyz

Ruby: warn "err"
来源：http://dgz.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://pmb.mhx1999.top

[M07] 判断是否为主入口
来源：http://rcw.xinyue.icu

Py:   if __name__ == "__main__":
来源：http://kzp.jiagoushi.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yay.yongpay.top

JS:   require.main === module
来源：http://iqu.jinqigufen.top

TS:   require.main === module
来源：http://wbt.vehdjk.com

Java: public static void main(String[] args)
来源：http://pbv.316326.xyz

Go:   func main()
来源：http://iev.tian-w.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bve.bbcook.cn

C#:   static void Main(string[] args)
来源：http://ffu.dianchejie.cn

[M08] 获取系统与运行时信息
来源：http://pyh.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://buh.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://zfn.cdnleiting.top

JS:   process.platform;  process.version
来源：http://ksy.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://yio.shanyushiyangtech.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zqc.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kcl.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nxy.shzxlz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://egz.xuetiantiany.cn

================================================================================
来源：http://bes.sjlbkw.cn

N. 数据结构与算法
来源：http://fmd.redwolf501.top

================================================================================
来源：http://ngt.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://kff.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://bkb.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://try.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xdi.jinqigfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qgf.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uvx.cashguo.top

Go:   sort.SearchInts(arr, x)
来源：http://oet.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://iue.sweek.top

C#:   Array.BinarySearch(arr, x)
来源：http://ljs.zdbjq.cn

[N02] 排序（工程实践用内置实现）
来源：http://mvj.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://hnv.chenjidiqi.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://weg.yuxming.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ftb.shangyingyoupin.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cax.nwbrower.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://srk.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://uma.ybcxt.top

Ruby: arr.sort
来源：http://wrw.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kxm.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://sbr.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kca.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://dvi.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rdi.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ffx.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dgu.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hge.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://twn.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://mmn.hnqzz.top

[N04] 斐波那契数列
来源：http://zuu.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qil.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ppr.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ajd.fehbvm.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sll.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yvj.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ewc.yongpay.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lri.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fou.haohaochexian.top

[N05] 最大公约数
来源：http://rli.fzhhl.top

Py:   math.gcd(a, b)
来源：http://kbc.bbcook.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jyb.shuidangran.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gwn.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://egc.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wql.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oym.ctjpmb.com

Ruby: a.gcd(b)
来源：http://cxr.yj20258.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zvx.fengsongda.top

[N06] 判断回文字符串
来源：http://ntq.yuanzhike.top

Py:   s == s[::-1]
来源：http://lls.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://qas.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://fdp.uphjek.com

TS:   s === [...s].reverse().join("")
来源：http://jfl.yonumen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mqw.tian-w.cn

Go:   // 双指针从两端比较
来源：http://qfc.cucudq.cn

Ruby: s == s.reverse
来源：http://iph.shzxlz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jtd.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://gkk.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://szt.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hmz.zhoulong.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://noj.feifeiyinyue.top

TS:   // 手写 Map<string, number>
来源：http://oqg.ydzc1.top

Java: // 手写 HashMap
来源：http://bcf.c1oappe.top

Go:   // 手写 map[int]int
来源：http://cmz.vqdsnc.cn

Ruby: // 手写 Hash
来源：http://pox.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://tvu.vehdjk.com

[N08] 生成全排列
来源：http://yab.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://yfm.haohaochexian.top

PHP:  // 手写递归交换
来源：http://rom.uphjek.com

JS:   // 手写回溯递归
来源：http://vog.zhoulong.xyz

TS:   // 手写回溯递归
来源：http://ezq.sjlbkw.cn

Java: // 手写回溯递归
来源：http://bfn.zhixingplan.top

Go:   // 手写回溯递归
来源：http://iqr.gzhubu.top

Ruby: arr.permutation.to_a
来源：http://qxf.yj20258.top

C#:   // 手写回溯递归
来源：http://xqn.snrcjt.cn

[N09] 栈与队列
来源：http://xrs.hnxiangtu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jaj.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zqz.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oet.shuidangran.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tmf.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://osy.cashguo.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qxh.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bnw.sysykeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lvr.iojbl.cn

[N10] 链表节点定义
来源：http://iyu.xuanzx.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iap.ppjwa.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cpc.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ndj.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hvc.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://lie.shanyushiyangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://dyt.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bdg.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zji.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://osv.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jij.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://ffo.wangshuangyany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fjs.yongpay.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zxr.jqgfzy.top

Java: // 手写递归
来源：http://mtb.tianlin.xyz

Go:   // 手写递归
来源：http://wzq.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bmc.shzxlz.cn

C#:   // 手写递归
来源：http://xmb.iojbl.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pgb.havefunace.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uyv.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rnf.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://acv.wangshuangyany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bsw.chenlongwang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uki.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fuq.0kj1m.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kni.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lzp.jlsjyb.cn

================================================================================
来源：http://cke.cqqwz.cn

O. 并发与异步
来源：http://nwq.kuanghao11.cn

================================================================================
来源：http://obu.smart0.xyz

[O01] 启动一个线程
来源：http://vmq.nanxuanxn.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hzs.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lqj.hnqzz.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jjo.hcnkem.com

TS:   // 同 JS
来源：http://uvi.guowangkeji.top

Java: new Thread(() -> f()).start()
来源：http://ghy.tanke756.top

Go:   go f()
来源：http://pvw.bjfxy.top

Ruby: Thread.new { f }
来源：http://smx.sufxvd.cn

C#:   Task.Run(() => F());
来源：http://tir.yangfankeji.com

[O02] 使用线程池
来源：http://ria.jlsjyb.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wbw.zhoulong.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zdy.ctjpmb.com

JS:   // worker_threads 线程池
来源：http://jau.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://sqy.andypj.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://nqm.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yhz.zhongyouzk.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://noi.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vnk.pycfn.com

[O03] 加锁保护共享数据
来源：http://sga.zycfv.cn

Py:   with lock: shared += 1
来源：http://hsj.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://jog.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mct.birdmap.top

TS:   // 同 JS
来源：http://skb.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://qrh.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zwi.9152youxi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jhd.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://wbc.snrcjt.cn

[O04] 定义异步函数并等待
来源：http://dhq.hysaishi.cn

Py:   async def f():⏎    await g()
来源：http://qsk.guowangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pgn.vqdsnc.cn

JS:   async function f() { await g(); }
来源：http://oud.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pko.daria6918.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ogs.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zjn.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://pue.yanxiufei.cn

C#:   async Task F() { await G(); }
来源：http://rfi.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://kzu.xylfe.cn

Py:   asyncio.gather(*tasks)
来源：http://sbd.tian-w.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iqx.fktsv.cn

JS:   await Promise.all(tasks)
来源：http://chz.ivvv.top

TS:   await Promise.all(tasks)
来源：http://uxj.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uhc.meibo888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uwx.gzhubu.top

Ruby: threads.map(&:join)
来源：http://bwt.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://twg.nanxuanxn.top

[O06] 使用进程池
来源：http://bzh.pycfn.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://edq.yongpay.top

PHP:  // pcntl_fork 或多进程队列
来源：http://htl.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://aqt.vqdsnc.cn

TS:   // child_process / cluster 模块
来源：http://lig.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fmp.zhiwuduotai.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wrm.iojbl.cn

Ruby: // fork 块
来源：http://euk.gotoacloud.top

C#:   Parallel.For
来源：http://hra.yuxming.cn

================================================================================
来源：http://lqk.yj202588.top

P. 常用工具函数
来源：http://tbx.yueranfly.top

================================================================================
来源：http://pkb.chenjidiqi.icu

[P01] 生成 UUID
来源：http://nlg.0kj1m.cn

Py:   str(uuid.uuid4())
来源：http://izz.meibo888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dcf.ybcxt.top

JS:   crypto.randomUUID()
来源：http://dbi.redwolf501.top

TS:   crypto.randomUUID()
来源：http://vlx.cucudq.cn

Java: UUID.randomUUID().toString()
来源：http://afj.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://cpf.pycfn.com

Ruby: SecureRandom.uuid
来源：http://wxo.daria6918.cn

C#:   Guid.NewGuid().ToString()
来源：http://kje.chenlongwang.top

[P02] MD5 / SHA256 摘要
来源：http://wki.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://atw.cqqwz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rdl.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yfu.jqgufenzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aeh.jqgufenzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fup.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wzl.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zgd.yvedp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://prm.zhengqikj.top

[P03] 生成短随机字符串
来源：http://ljg.bbcook.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xhz.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xsk.hnqzz.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gzc.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eds.birdmap.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xjs.zdbjq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gpe.cashguo.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vtb.yonumen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ldq.xinyue.icu

[P04] 求长度
来源：http://wix.yfazqb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pvc.tanke756.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ekd.cashguo.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zom.yuxming.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bzc.sweek.top

Java: list.size();  map.size();  s.length()
来源：http://ash.chenlongwang.top

Go:   len(arr);  len(m)
来源：http://udd.nanxinkj.top

Ruby: x.length;  x.size
来源：http://kme.sufxvd.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lmd.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://oja.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wym.xziqi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oxi.zhongyouzk.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pky.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vfu.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cbi.pycfn.com

Go:   reflect.DeepEqual(a, b)
来源：http://tzl.chenzaomai.com

Ruby: a == b
来源：http://xou.yvedp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sbt.sweek.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uyf.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lcx.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://lsp.xuetiantiany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pqo.gaohongyu789.top

TS:   if (x == null) {}
来源：http://elg.jqgfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fpa.c1oappe.top

Go:   if x == nil {}
来源：http://tja.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yph.hnqzz.top

C#:   if (x is null) {}
来源：http://fhm.jianghu66.top

[P07] 防抖与节流
来源：http://oru.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zqn.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://eat.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bfw.zhixingplan.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fbz.feifeiyinyue.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xxb.zhiwuduotai.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://swj.yangfankeji.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ujk.snrcjt.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rkt.yongpay.top

[P08] 处理浮点精度问题
来源：http://dqx.meibo888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dak.ydzc1.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kia.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jyl.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://him.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ykm.andypj.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hmt.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wrg.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gbr.yanxiufei.cn

================================================================================
来源：http://edo.jlsjyb.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dbm.fanxiaobao.xyz

================================================================================
来源：http://qug.havefunace.top

[Q01] 创建表
来源：http://zjm.shuidangran.top

CREATE TABLE users (
来源：http://xqb.cheryme.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://odg.hnqzz.top

name VARCHAR(50) NOT NULL,
来源：http://rcc.hcnkem.com

email VARCHAR(100) UNIQUE,
来源：http://mdr.vehdjk.com


<!-- 参考信息 -->