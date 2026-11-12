代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://esg.jianghu66.top

JS:   process.env.HOME
来源：http://drz.jlsjyb.cn

TS:   process.env.HOME
来源：http://bvi.guowangkeji.top

Java: System.getenv("HOME")
来源：http://lvz.9152youxi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://orb.yuanzhike.top

Ruby: ENV["HOME"]
来源：http://eeu.zhoulong.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gqj.wangdashe.top

[M03] 执行外部命令
来源：http://oam.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tux.feifeiyinyue.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zxv.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://aka.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://efh.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yxp.316326.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://zfk.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bsc.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://peu.yongpay.top

[M04] 获取当前工作目录
来源：http://bhe.wangdashe.top

Py:   os.getcwd()
来源：http://uos.hnqzz.top

PHP:  getcwd();
来源：http://xnn.zhijiandao.cn

JS:   process.cwd()
来源：http://afh.316326.xyz

TS:   process.cwd()
来源：http://xlk.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://ltc.fktsv.cn

Go:   os.Getwd()
来源：http://nzq.sysykeji.top

Ruby: Dir.pwd
来源：http://ibg.jinyuanbaomall.cn

C#:   Directory.GetCurrentDirectory()
来源：http://koh.shanyushiyangtech.top

[M05] 设置退出码
来源：http://vgw.feifeiyinyue.top

Py:   sys.exit(1)
来源：http://exw.ivvv.top

PHP:  exit(1);
来源：http://mjp.snrcjt.cn

JS:   process.exit(1)
来源：http://bmn.ppjwa.cn

TS:   process.exit(1)
来源：http://kqq.fzhhl.top

Java: System.exit(1)
来源：http://trt.jianghu66.top

Go:   os.Exit(1)
来源：http://adw.smart0.xyz

Ruby: exit 1
来源：http://gwv.xuetiantiany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nvi.aizwys.cn

[M06] 向标准错误输出
来源：http://zek.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://lln.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ezk.hesvh.cn

JS:   console.error("err")
来源：http://ect.jinyuanbaomall.cn

TS:   console.error("err")
来源：http://cyk.yonumen.top

Java: System.err.println("err")
来源：http://avf.smart0.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://frx.xuanzx.com

Ruby: warn "err"
来源：http://uxw.dianchejie.cn

C#:   Console.Error.WriteLine("err")
来源：http://chc.meibo888.top

[M07] 判断是否为主入口
来源：http://jrd.meibo888.top

Py:   if __name__ == "__main__":
来源：http://apb.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zkx.zhaomingkeji.xyz

JS:   require.main === module
来源：http://ntk.hfpthk.cn

TS:   require.main === module
来源：http://kzh.uphjek.com

Java: public static void main(String[] args)
来源：http://lbg.jqgfzy.top

Go:   func main()
来源：http://ozx.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://umk.yj20258888.top

C#:   static void Main(string[] args)
来源：http://gsh.cucudq.cn

[M08] 获取系统与运行时信息
来源：http://mhm.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://tcb.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://mnr.yj20258888.top

JS:   process.platform;  process.version
来源：http://iyn.yueranfly.top

TS:   process.platform;  process.version
来源：http://euu.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ozl.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://odd.fzhhl.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nox.yj202588.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uvr.chenjidiqi.icu

================================================================================
来源：http://exq.zhiwuduotai.top

N. 数据结构与算法
来源：http://coq.yj20258888.top

================================================================================
来源：http://vmr.ivvv.top

[N01] 二分查找（有序数组）
来源：http://uci.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wfq.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pch.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sue.hesvh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hgf.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://bcf.feifeiyinyue.top

Go:   sort.SearchInts(arr, x)
来源：http://liv.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qdn.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://frc.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://kfx.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://aea.hnxiangtu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://plj.xinyue.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://njh.chenzaomai.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://ypk.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rdj.yongpay.top

Go:   slices.Sort(arr)
来源：http://gix.wangshuangyany.cn

Ruby: arr.sort
来源：http://ccn.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ije.aizwys.cn

[N03] 快速排序（分治示例）
来源：http://jhy.yvedp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kwt.cucudq.cn

PHP:  // 递归实现，或用 usort
来源：http://vur.nanxuanxn.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fig.snrcjt.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sjo.yuanzhike.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gjd.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dsv.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xai.cdnleiting.top

C#:   // 手写递归，或 Array.Sort
来源：http://rea.hfpthk.cn

[N04] 斐波那契数列
来源：http://phd.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gjd.tarul.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://phc.sufxvd.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cnh.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://peo.vqdsnc.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gzq.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yon.ydzc1.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gru.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uiw.jinghuilouyu.cn

[N05] 最大公约数
来源：http://ljv.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://zmz.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kct.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qvr.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kha.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kda.zhengqikj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eob.yangfankeji.com

Ruby: a.gcd(b)
来源：http://tgy.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pht.nanxinkj.top

[N06] 判断回文字符串
来源：http://kur.quarkkingdee.top

Py:   s == s[::-1]
来源：http://rra.hcnkem.com

PHP:  $s === strrev($s);
来源：http://qex.yj20258888.top

JS:   s === [...s].reverse().join("")
来源：http://mqs.cucudq.cn

TS:   s === [...s].reverse().join("")
来源：http://zdf.xinyue.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jrh.ydjk.org.cn

Go:   // 双指针从两端比较
来源：http://rku.c1oappe.top

Ruby: s == s.reverse
来源：http://cvo.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uzm.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://fyr.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rpp.jqgfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aal.yvedp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ftm.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://cxh.hcnkem.com

Java: // 手写 HashMap
来源：http://clo.316326.xyz

Go:   // 手写 map[int]int
来源：http://age.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://hrv.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iwd.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://nph.kuanghao11.cn

Py:   itertools.permutations(arr)
来源：http://txb.bbcook.cn

PHP:  // 手写递归交换
来源：http://key.bbcook.cn

JS:   // 手写回溯递归
来源：http://vas.cqqwz.cn

TS:   // 手写回溯递归
来源：http://htd.xylfe.cn

Java: // 手写回溯递归
来源：http://ujq.snrcjt.cn

Go:   // 手写回溯递归
来源：http://adr.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://brm.shanyushiyangtech.top

C#:   // 手写回溯递归
来源：http://aur.xziqi.cn

[N09] 栈与队列
来源：http://mxn.yj20258888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rzq.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nup.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://phh.shuidangran.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ano.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zng.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lfc.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sdg.sysykeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://azy.jinqigufen.top

[N10] 链表节点定义
来源：http://lyx.shanyushiyangtech.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ryo.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ygx.hammf.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dzu.bjfxy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://llk.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://yey.yangfankeji.com

Go:   type Node struct { V int; Next *Node }
来源：http://cvm.fehbvm.com

Ruby: Node = Struct.new(:v, :next)
来源：http://jzt.jinqigufen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wkx.yonumen.top

[N11] 二叉树中序遍历
来源：http://bdo.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nlh.xinyue.icu

PHP:  // 手写递归函数
来源：http://qph.dashuyun.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iun.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xzo.tarul.cn

Java: // 手写递归
来源：http://xhm.dashuyun.cn

Go:   // 手写递归
来源：http://upo.jqgufenzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://awc.yueranfly.top

C#:   // 手写递归
来源：http://cdt.cucudq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xsm.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hwa.snrcjt.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qvf.bbcook.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dnm.cheryme.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xfo.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zod.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kqi.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uxq.redwolf501.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fhl.xingfuxueyuan.xyz

================================================================================
来源：http://tfr.gzhubu.top

O. 并发与异步
来源：http://www.havefunace.top

================================================================================
来源：http://zag.birdmap.top

[O01] 启动一个线程
来源：http://gzd.52xcode.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rff.zycfv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://myn.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://icn.gotoacloud.top

TS:   // 同 JS
来源：http://gxt.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://cwy.jinqigufen.top

Go:   go f()
来源：http://bop.aibaodan.cn

Ruby: Thread.new { f }
来源：http://ern.xingfuxueyuan.xyz

C#:   Task.Run(() => F());
来源：http://czm.xinyue.icu

[O02] 使用线程池
来源：http://qkt.c1oappe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pik.hcnkem.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://svx.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://pwo.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://oqd.havefunace.top

Java: Executors.newFixedThreadPool(4)
来源：http://tjn.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rwb.gzhubu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eff.0kj1m.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dwy.vehdjk.com

[O03] 加锁保护共享数据
来源：http://hvk.daria6918.cn

Py:   with lock: shared += 1
来源：http://uyn.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://qsr.fzhhl.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qez.xuetiantiany.cn

TS:   // 同 JS
来源：http://xzf.xziqi.cn

Java: synchronized (this) { shared++; }
来源：http://hbs.aizwys.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://exu.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ndx.ehwqpu.com

C#:   lock (gate) { shared++; }
来源：http://rup.wangshuangyany.cn

[O04] 定义异步函数并等待
来源：http://sux.yangfankeji.com

Py:   async def f():⏎    await g()
来源：http://ckj.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fik.smart0.xyz

JS:   async function f() { await g(); }
来源：http://rwk.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qud.nanxinkj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://meh.zhaomingkeji.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gvf.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://sib.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://jsh.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://fnb.hcnkem.com

Py:   asyncio.gather(*tasks)
来源：http://nkk.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://auz.jqgufenzy.top

JS:   await Promise.all(tasks)
来源：http://eev.ivvv.top

TS:   await Promise.all(tasks)
来源：http://fac.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yfw.hnxiangtu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lvd.birdmap.top

Ruby: threads.map(&:join)
来源：http://tfg.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pan.ivvv.top

[O06] 使用进程池
来源：http://aor.feifeiyinyue.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pue.yanxiufei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nfr.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://fwi.bjfxy.top

TS:   // child_process / cluster 模块
来源：http://gwv.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://idl.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uap.yangfankeji.com

Ruby: // fork 块
来源：http://rgv.vqdsnc.cn

C#:   Parallel.For
来源：http://afv.zhoulong.xyz

================================================================================
来源：http://jwm.yangfankeji.com

P. 常用工具函数
来源：http://cbh.yuxming.cn

================================================================================
来源：http://mxl.yj20258888.top

[P01] 生成 UUID
来源：http://soj.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://jey.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xvn.wangdashe.top

JS:   crypto.randomUUID()
来源：http://rpx.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://dka.jinqigufen.top

Java: UUID.randomUUID().toString()
来源：http://dlc.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://vvd.zhixingplan.top

Ruby: SecureRandom.uuid
来源：http://jec.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://pvj.smart0.xyz

[P02] MD5 / SHA256 摘要
来源：http://jep.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yqn.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zbn.fktsv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vts.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uab.shangyingyoupin.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iru.zhengqikj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nmc.sysykeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pli.ctjpmb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eyx.nwbrower.top

[P03] 生成短随机字符串
来源：http://bey.yvedp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fkj.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://msb.cdnleiting.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zdr.sufxvd.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fom.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bll.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jsw.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iep.dianchejie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dho.uphjek.com

[P04] 求长度
来源：http://sio.cheryme.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vfc.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://opy.feifeiyinyue.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rob.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yip.yuanzhike.top

Java: list.size();  map.size();  s.length()
来源：http://gjn.xziqi.cn

Go:   len(arr);  len(m)
来源：http://nlk.jiagoushi.top

Ruby: x.length;  x.size
来源：http://vjx.zhoulong.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://gbp.yonumen.top

[P05] 判断两个对象内容是否相等
来源：http://jbp.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jyv.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mll.dianchejie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://avg.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zlp.sxryk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ayk.hfpthk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://isc.cashguo.top

Ruby: a == b
来源：http://mom.yuxming.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rpl.hammf.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kwo.tanke756.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://urs.zhaomingkeji.xyz

PHP:  if (empty($x)) {}
来源：http://bvb.feifeiyinyue.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vqo.bbcook.cn

TS:   if (x == null) {}
来源：http://wjz.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ger.hnqzz.top

Go:   if x == nil {}
来源：http://sal.gogol.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jvc.feifeiyinyue.top

C#:   if (x is null) {}
来源：http://qtc.nwbrower.top

[P07] 防抖与节流
来源：http://ynz.yanxiufei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ksj.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://bff.wangshuangyany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xeg.yj202588.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mgh.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dwj.haohaochexian.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xps.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ksm.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aut.epnwcf.com

[P08] 处理浮点精度问题
来源：http://umz.shanyushiyangtech.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dqy.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wth.tanke756.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xvm.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nay.yuxming.cn


<!-- 参考信息 -->