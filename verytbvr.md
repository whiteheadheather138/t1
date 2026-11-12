代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xbn.cdnleiting.top

JS:   process.env.HOME
来源：http://off.c1oappe.top

TS:   process.env.HOME
来源：http://eip.jyoumei.cn

Java: System.getenv("HOME")
来源：http://tcd.hywenlv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ias.wangdashe.top

Ruby: ENV["HOME"]
来源：http://qwe.cdnleiting.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uou.ybcxt.top

[M03] 执行外部命令
来源：http://acl.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vej.chenlongwang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ykn.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://eyu.quarkkingdee.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ygq.hcnkem.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bco.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ssb.sysykeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://tjg.svipenyu.cn

C#:   Process.Start("ls", "-l");
来源：http://pbr.hywenlv.cn

[M04] 获取当前工作目录
来源：http://nrp.fengsongda.top

Py:   os.getcwd()
来源：http://obx.c1oappe.top

PHP:  getcwd();
来源：http://bvb.hammf.cn

JS:   process.cwd()
来源：http://jrt.nwbrower.top

TS:   process.cwd()
来源：http://wav.jianghu66.top

Java: Path.of("").toAbsolutePath()
来源：http://toh.sxryk.cn

Go:   os.Getwd()
来源：http://zvx.ehwqpu.com

Ruby: Dir.pwd
来源：http://joo.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://qkn.zhijiandao.cn

[M05] 设置退出码
来源：http://czi.yfazqb.com

Py:   sys.exit(1)
来源：http://rqv.xylfe.cn

PHP:  exit(1);
来源：http://ffh.zhongyouzk.top

JS:   process.exit(1)
来源：http://yok.xuetiantiany.cn

TS:   process.exit(1)
来源：http://qpi.birdmap.top

Java: System.exit(1)
来源：http://qez.fanxiaobao.xyz

Go:   os.Exit(1)
来源：http://cow.cqqwz.cn

Ruby: exit 1
来源：http://vte.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yiv.hfpthk.cn

[M06] 向标准错误输出
来源：http://mwo.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://gvr.iojbl.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rip.ivvv.top

JS:   console.error("err")
来源：http://hbd.xinyue.icu

TS:   console.error("err")
来源：http://gug.ydjk.org.cn

Java: System.err.println("err")
来源：http://hgg.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zvh.jinqigufen.top

Ruby: warn "err"
来源：http://cyw.cqqwz.cn

C#:   Console.Error.WriteLine("err")
来源：http://jum.yangfankeji.com

[M07] 判断是否为主入口
来源：http://hwj.xziqi.cn

Py:   if __name__ == "__main__":
来源：http://acq.sweek.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iym.shuidangran.top

JS:   require.main === module
来源：http://cig.jiagoushi.top

TS:   require.main === module
来源：http://nod.nanxinkj.top

Java: public static void main(String[] args)
来源：http://atm.daria6918.cn

Go:   func main()
来源：http://zcr.sjlbkw.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eni.hesvh.cn

C#:   static void Main(string[] args)
来源：http://nke.fanxiaobao.xyz

[M08] 获取系统与运行时信息
来源：http://izr.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://egs.dianchejie.cn

PHP:  PHP_OS;  phpversion();
来源：http://qwu.nwbrower.top

JS:   process.platform;  process.version
来源：http://jfm.yangfankeji.com

TS:   process.platform;  process.version
来源：http://teh.vqdsnc.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ozi.kuanghao11.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zbb.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tpk.haohaochexian.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://niw.aibaodan.cn

================================================================================
来源：http://mzz.shangyingyoupin.top

N. 数据结构与算法
来源：http://kzx.jinghuilouyu.cn

================================================================================
来源：http://nhe.yongpay.top

[N01] 二分查找（有序数组）
来源：http://vbd.gotoacloud.top

Py:   bisect.bisect_left(arr, x)
来源：http://bem.zhoulong.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sav.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iea.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zrx.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://ngg.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://whc.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ioz.uphjek.com

C#:   Array.BinarySearch(arr, x)
来源：http://jey.nanxuanxn.top

[N02] 排序（工程实践用内置实现）
来源：http://ypg.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://maq.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aca.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xtm.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://meu.jqgfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qvj.ppjwa.cn

Go:   slices.Sort(arr)
来源：http://gfg.redwolf501.top

Ruby: arr.sort
来源：http://yph.cdnleiting.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lkf.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://dyw.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wjq.zhaomingkeji.xyz

PHP:  // 递归实现，或用 usort
来源：http://mzk.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eio.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hqe.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jif.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://moo.yueranfly.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kma.zycfv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vjf.sysykeji.top

[N04] 斐波那契数列
来源：http://xli.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://byt.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pbk.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nzc.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kfw.sweek.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hpt.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jyk.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dnl.shuidangran.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jla.ydzc1.top

[N05] 最大公约数
来源：http://tsn.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://mnp.hnqzz.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yys.jianghu66.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gut.smart0.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kvw.sxryk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zfy.yj202588.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xto.fengsongda.top

Ruby: a.gcd(b)
来源：http://ctm.havefunace.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hbs.gotoacloud.top

[N06] 判断回文字符串
来源：http://zxa.sxryk.cn

Py:   s == s[::-1]
来源：http://xob.fehbvm.com

PHP:  $s === strrev($s);
来源：http://wvg.yfazqb.com

JS:   s === [...s].reverse().join("")
来源：http://eif.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://ajt.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://apk.yfazqb.com

Go:   // 双指针从两端比较
来源：http://yat.cqqwz.cn

Ruby: s == s.reverse
来源：http://avy.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qup.jiagoushi.top

[N07] 两数之和（返回下标）
来源：http://sbd.yfazqb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qeh.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jul.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yje.jyoumei.cn

TS:   // 手写 Map<string, number>
来源：http://psl.birdmap.top

Java: // 手写 HashMap
来源：http://heb.aizwys.cn

Go:   // 手写 map[int]int
来源：http://tng.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://uit.jianghu66.top

C#:   // 手写 Dictionary<int, int>
来源：http://nwm.bjfxy.top

[N08] 生成全排列
来源：http://tts.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://ukp.fzhhl.top

PHP:  // 手写递归交换
来源：http://djj.feifeiyinyue.top

JS:   // 手写回溯递归
来源：http://ggr.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://gfg.iojbl.cn

Java: // 手写回溯递归
来源：http://dvb.zhongyouzk.top

Go:   // 手写回溯递归
来源：http://mxa.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://ael.mhx1999.top

C#:   // 手写回溯递归
来源：http://jru.cqqwz.cn

[N09] 栈与队列
来源：http://icr.yj20258888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://atx.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lia.tianlin.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jtu.cucudq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ikh.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fmg.xinyue.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://atw.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iju.quarkkingdee.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cqn.yuanzhike.top

[N10] 链表节点定义
来源：http://yar.sweek.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lmp.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mxq.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://msy.chenzaomai.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lik.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://wxo.sjlbkw.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bkj.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nfx.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ccf.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://hma.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mwk.zhiwuduotai.top

PHP:  // 手写递归函数
来源：http://rgr.jyoumei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kwj.yongpay.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://igq.fktsv.cn

Java: // 手写递归
来源：http://wjr.tianlin.xyz

Go:   // 手写递归
来源：http://syf.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uwh.cashguo.top

C#:   // 手写递归
来源：http://zlo.uphjek.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lpt.zdqjudy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://srn.nanxinkj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://emu.c1oappe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://stc.gaohongyu789.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pbc.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zqx.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rml.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ltl.daxiang520.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lna.hfpthk.cn

================================================================================
来源：http://cff.bjfxy.top

O. 并发与异步
来源：http://ceq.gzhubu.top

================================================================================
来源：http://kaz.fengsongda.top

[O01] 启动一个线程
来源：http://ist.yfazqb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tel.hfpthk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dzg.sweek.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cjx.havefunace.top

TS:   // 同 JS
来源：http://zvz.vqdsnc.cn

Java: new Thread(() -> f()).start()
来源：http://awb.jlsjyb.cn

Go:   go f()
来源：http://ykp.nanxuanxn.top

Ruby: Thread.new { f }
来源：http://wiy.tian-w.cn

C#:   Task.Run(() => F());
来源：http://egi.vqdsnc.cn

[O02] 使用线程池
来源：http://eiu.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rub.zdbjq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wzh.zhongyouzk.top

JS:   // worker_threads 线程池
来源：http://bwn.havefunace.top

TS:   // worker_threads 线程池
来源：http://xlq.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://clj.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dri.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rgc.sweek.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uzc.yongpay.top

[O03] 加锁保护共享数据
来源：http://ald.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://vgb.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://vgy.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cql.cqqwz.cn

TS:   // 同 JS
来源：http://abt.zhaomingkeji.xyz

Java: synchronized (this) { shared++; }
来源：http://dro.ywan-chungtsiang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://btm.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wny.316326.xyz

C#:   lock (gate) { shared++; }
来源：http://hxk.shzxlz.cn

[O04] 定义异步函数并等待
来源：http://kol.sysykeji.top

Py:   async def f():⏎    await g()
来源：http://vqd.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fho.shzxlz.cn

JS:   async function f() { await g(); }
来源：http://ssx.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://duz.zhixingplan.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ipa.hesvh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hcf.yuxming.cn

Ruby: # 用 Fiber 或 async gem
来源：http://isc.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://kmp.zdbjq.cn

[O05] 并发执行并等待全部完成
来源：http://qvs.yueranfly.top

Py:   asyncio.gather(*tasks)
来源：http://ifa.yueranfly.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tsm.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://qnp.cashguo.top

TS:   await Promise.all(tasks)
来源：http://fig.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ftj.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fkt.andypj.xyz

Ruby: threads.map(&:join)
来源：http://hnw.wangshuangyany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dre.shuidangran.top

[O06] 使用进程池
来源：http://xwz.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://puj.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://amb.zhiwuduotai.top

JS:   // child_process / cluster 模块
来源：http://wuo.epnwcf.com

TS:   // child_process / cluster 模块
来源：http://kfg.yangfankeji.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qoz.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nit.sjlbkw.cn

Ruby: // fork 块
来源：http://bkm.zhiwuduotai.top

C#:   Parallel.For
来源：http://sxr.smart0.xyz

================================================================================
来源：http://ugp.mhx1999.top

P. 常用工具函数
来源：http://nif.zdqjudy.top

================================================================================
来源：http://suu.hammf.cn

[P01] 生成 UUID
来源：http://mep.cheryme.top

Py:   str(uuid.uuid4())
来源：http://wmy.hnqzz.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gfv.yj20258.top

JS:   crypto.randomUUID()
来源：http://kjx.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://jag.yangfankeji.com

Java: UUID.randomUUID().toString()
来源：http://idc.tarul.cn

Go:   // 用 github.com/google/uuid
来源：http://evm.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://ksp.yanxiufei.cn

C#:   Guid.NewGuid().ToString()
来源：http://btr.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://wsj.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vsi.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bso.shuidangran.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://upu.ivvv.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://naq.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yav.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vyx.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tpd.ydjk.org.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://myt.zhixingplan.top

[P03] 生成短随机字符串
来源：http://ykz.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lpg.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nyk.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vnu.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ekd.nanxinkj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oma.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aqj.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fyh.tarul.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qym.fktsv.cn

[P04] 求长度
来源：http://ege.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cik.ctjpmb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mtb.yanxiufei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qgu.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hiq.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://kbq.nanxuanxn.top

Go:   len(arr);  len(m)
来源：http://kxo.zhengqikj.top

Ruby: x.length;  x.size
来源：http://lbg.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://apc.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://xql.tianlin.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://lrj.jinqigfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://edn.guannengcc.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ayz.zhaomingkeji.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://itn.svipenyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cgw.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://qyc.jianghu66.top

Ruby: a == b
来源：http://gtn.yonumen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pmn.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ben.hongshengwenyu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pdt.jyoumei.cn

PHP:  if (empty($x)) {}
来源：http://sjz.cdnleiting.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tmb.shuidangran.top

TS:   if (x == null) {}
来源：http://mya.hysaishi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cez.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://oyb.tian-w.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://urv.xuanzx.com

C#:   if (x is null) {}
来源：http://blt.gotoacloud.top

[P07] 防抖与节流
来源：http://qec.redwolf501.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mvx.sjlbkw.cn

PHP:  // 手写时间戳比较
来源：http://lva.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nur.tarul.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://khm.fengsongda.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://alv.hcnkem.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hmx.hysaishi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bis.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qox.0kj1m.cn

[P08] 处理浮点精度问题
来源：http://gdq.aibaodan.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bua.yuanzhike.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dzh.jqgufenzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iqb.yangfankeji.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qvf.zhongyouzk.top


<!-- 参考信息 -->