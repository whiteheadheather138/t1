代发 wailian999

Ruby: ARGV
来源：http://obr.chenlongwang.top

C#:   args 数组（Main 方法参数）
来源：http://gpu.feifeiyinyue.top

[M02] 读取环境变量
来源：http://joa.andypj.xyz

Py:   os.environ.get("HOME")
来源：http://lpr.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yya.52xcode.cn

JS:   process.env.HOME
来源：http://ahq.wangshuangyany.cn

TS:   process.env.HOME
来源：http://uiu.aibaodan.cn

Java: System.getenv("HOME")
来源：http://lpv.ydzc1.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ndk.jinghuilouyu.cn

Ruby: ENV["HOME"]
来源：http://xku.xinyue.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cpu.gotoacloud.top

[M03] 执行外部命令
来源：http://izq.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://klv.jinqigufen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mmh.andypj.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://poz.nanxuanxn.top

TS:   child_process.execSync("ls -l").toString()
来源：http://sah.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://axo.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lrg.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://gsn.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://xej.kuanghao11.cn

[M04] 获取当前工作目录
来源：http://rxa.yuanzhike.top

Py:   os.getcwd()
来源：http://mrx.jqgfzy.top

PHP:  getcwd();
来源：http://dpr.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://ntl.zhoulong.xyz

TS:   process.cwd()
来源：http://hjv.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://nit.redwolf501.top

Go:   os.Getwd()
来源：http://zxa.gotoacloud.top

Ruby: Dir.pwd
来源：http://fqb.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://kcu.xylfe.cn

[M05] 设置退出码
来源：http://dct.zhengqikj.top

Py:   sys.exit(1)
来源：http://rax.gotoacloud.top

PHP:  exit(1);
来源：http://del.wangdashe.top

JS:   process.exit(1)
来源：http://pyg.jlsjyb.cn

TS:   process.exit(1)
来源：http://guk.feifeiyinyue.top

Java: System.exit(1)
来源：http://kjy.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://fox.cucudq.cn

Ruby: exit 1
来源：http://jtw.shangyingyoupin.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fna.zhijiandao.cn

[M06] 向标准错误输出
来源：http://cdg.chenzaomai.com

Py:   print("err", file=sys.stderr)
来源：http://nsk.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://hlb.52xcode.cn

JS:   console.error("err")
来源：http://nrq.aibaodan.cn

TS:   console.error("err")
来源：http://apf.nanxuanxn.top

Java: System.err.println("err")
来源：http://exz.gotoacloud.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ytl.jianghu66.top

Ruby: warn "err"
来源：http://jiw.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://bqe.xinyue.icu

[M07] 判断是否为主入口
来源：http://klg.xingfuxueyuan.xyz

Py:   if __name__ == "__main__":
来源：http://enc.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jbp.aibaodan.cn

JS:   require.main === module
来源：http://fzj.shanyushiyangtech.top

TS:   require.main === module
来源：http://bgi.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://bur.tian-w.cn

Go:   func main()
来源：http://dhc.zdbjq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xgc.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://bvb.tanke756.top

[M08] 获取系统与运行时信息
来源：http://xjy.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://ree.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://xkc.yj202588.top

JS:   process.platform;  process.version
来源：http://umc.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://cfu.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://thh.zhiwuduotai.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nmx.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zkj.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mbx.quarkkingdee.top

================================================================================
来源：http://yyh.tian-w.cn

N. 数据结构与算法
来源：http://umt.jinyuanbaomall.cn

================================================================================
来源：http://sxw.vqdsnc.cn

[N01] 二分查找（有序数组）
来源：http://tdc.hongshengwenyu.top

Py:   bisect.bisect_left(arr, x)
来源：http://cjq.zhoulong.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zjb.52xcode.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://euv.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kre.jiagoushi.top

Java: Arrays.binarySearch(arr, x)
来源：http://fhy.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://udp.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zfn.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://dcq.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://uqd.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://cae.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hxh.tianlin.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://zrw.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ian.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ghx.52xcode.cn

Go:   slices.Sort(arr)
来源：http://ait.uphjek.com

Ruby: arr.sort
来源：http://dpl.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qgs.aibaodan.cn

[N03] 快速排序（分治示例）
来源：http://pzt.hongshengwenyu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://obh.wangdashe.top

PHP:  // 递归实现，或用 usort
来源：http://xwh.gogol.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ptt.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cvf.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sfj.yangfankeji.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zoo.gaohongyu789.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wxc.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jyq.52xcode.cn

[N04] 斐波那契数列
来源：http://aho.xuanzx.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ars.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cwr.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kmi.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fhv.yj20258888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qwy.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mrq.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bqa.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sut.hcnkem.com

[N05] 最大公约数
来源：http://vcf.sufxvd.cn

Py:   math.gcd(a, b)
来源：http://mwm.cheryme.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xkq.zhijiandao.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gvq.fzhhl.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ret.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nxo.nwbrower.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nmn.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://loy.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jfw.jianghu66.top

[N06] 判断回文字符串
来源：http://gnt.cashguo.top

Py:   s == s[::-1]
来源：http://czu.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://dcq.uphjek.com

JS:   s === [...s].reverse().join("")
来源：http://nqm.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://ykq.tanke756.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wkn.uphjek.com

Go:   // 双指针从两端比较
来源：http://hrp.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://ebv.hcnkem.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://eei.hcnkem.com

[N07] 两数之和（返回下标）
来源：http://lyl.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vrp.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pez.c1oappe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kgy.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://qma.xylfe.cn

Java: // 手写 HashMap
来源：http://wpc.tarul.cn

Go:   // 手写 map[int]int
来源：http://zvv.shanyushiyangtech.top

Ruby: // 手写 Hash
来源：http://cgi.vqdsnc.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ckr.xylfe.cn

[N08] 生成全排列
来源：http://rls.daria6918.cn

Py:   itertools.permutations(arr)
来源：http://kgg.52xcode.cn

PHP:  // 手写递归交换
来源：http://qyi.nanxinkj.top

JS:   // 手写回溯递归
来源：http://hhs.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://xfc.c1oappe.top

Java: // 手写回溯递归
来源：http://ukm.jinqigfzy.top

Go:   // 手写回溯递归
来源：http://xcf.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://wwb.fehbvm.com

C#:   // 手写回溯递归
来源：http://zae.cheryme.top

[N09] 栈与队列
来源：http://tgu.cheryme.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hrt.nwbrower.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yyw.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kaq.yfazqb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ctn.yj202588.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pwq.xziqi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://opl.guannengcc.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://esg.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rqc.jiagoushi.top

[N10] 链表节点定义
来源：http://rme.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kfr.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qbm.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://obq.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zeh.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://low.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://jnk.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://oyx.nanxinkj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zjz.snrcjt.cn

[N11] 二叉树中序遍历
来源：http://nbr.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xhk.chenjidiqi.icu

PHP:  // 手写递归函数
来源：http://vxw.52xcode.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ojy.smart0.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iqg.yongpay.top

Java: // 手写递归
来源：http://nlk.bjfxy.top

Go:   // 手写递归
来源：http://rus.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ukv.zhoulong.xyz

C#:   // 手写递归
来源：http://zyf.wangshuangyany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hbg.xuetiantiany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mgr.daxiang520.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rit.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nek.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wgq.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ggp.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wnk.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pls.kuanghao11.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wur.iojbl.cn

================================================================================
来源：http://box.meibo888.top

O. 并发与异步
来源：http://ztq.ydjk.org.cn

================================================================================
来源：http://ubv.9152youxi.cn

[O01] 启动一个线程
来源：http://trn.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gyb.hnxiangtu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pzo.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ado.hysaishi.cn

TS:   // 同 JS
来源：http://giw.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://bti.xuetiantiany.cn

Go:   go f()
来源：http://brk.c1oappe.top

Ruby: Thread.new { f }
来源：http://rda.ctjpmb.com

C#:   Task.Run(() => F());
来源：http://hso.fktsv.cn

[O02] 使用线程池
来源：http://vei.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xwo.pengpengdd.cyou

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://prh.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://tnc.daxiang520.top

TS:   // worker_threads 线程池
来源：http://vut.cashguo.top

Java: Executors.newFixedThreadPool(4)
来源：http://vga.hnxiangtu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qug.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lix.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://osi.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://hex.zhijiandao.cn

Py:   with lock: shared += 1
来源：http://hat.sysykeji.top

PHP:  // 用 flock() 做文件锁
来源：http://jer.jinyuanbaomall.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nai.yvedp.cn

TS:   // 同 JS
来源：http://isg.gogol.net.cn

Java: synchronized (this) { shared++; }
来源：http://nlp.xuanzx.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jkp.uphjek.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://vco.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://aud.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://nir.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://xhl.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zvj.shanyushiyangkeji.top

JS:   async function f() { await g(); }
来源：http://khm.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kja.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hxa.vqdsnc.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://waz.birdmap.top

Ruby: # 用 Fiber 或 async gem
来源：http://hwr.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://lrz.yj202588.top

[O05] 并发执行并等待全部完成
来源：http://xsl.daria6918.cn

Py:   asyncio.gather(*tasks)
来源：http://wvn.sweek.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bbb.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://oso.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://opu.yanxiufei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hvk.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lth.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://jli.yj202588.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wxh.dashuyun.cn

[O06] 使用进程池
来源：http://esb.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eeu.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dwh.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://dxz.zdqjudy.top

TS:   // child_process / cluster 模块
来源：http://wzu.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rhz.andypj.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iqc.jyoumei.cn

Ruby: // fork 块
来源：http://nnw.hnxiangtu.top

C#:   Parallel.For
来源：http://svp.yanxiufei.cn

================================================================================
来源：http://dvu.ivvv.top

P. 常用工具函数
来源：http://kkj.xylfe.cn

================================================================================
来源：http://pov.yonumen.top

[P01] 生成 UUID
来源：http://zym.cucudq.cn

Py:   str(uuid.uuid4())
来源：http://pnx.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pcc.yfazqb.com

JS:   crypto.randomUUID()
来源：http://nok.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://lxs.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://cns.epnwcf.com

Go:   // 用 github.com/google/uuid
来源：http://qlz.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://nrr.bjfxy.top

C#:   Guid.NewGuid().ToString()
来源：http://psx.bbcook.cn

[P02] MD5 / SHA256 摘要
来源：http://ecr.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://koo.xylfe.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yae.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kdt.cdnleiting.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xdc.smart0.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bcx.nanxinkj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hud.guowangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wds.haohaochexian.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pmo.andypj.xyz

[P03] 生成短随机字符串
来源：http://zjh.zycfv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ssq.nanxuanxn.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gxd.yfazqb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bdn.zhiwuduotai.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mcw.shanyushiyangkeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yog.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cgj.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kut.shangyingyoupin.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lvv.xuetiantiany.cn

[P04] 求长度
来源：http://whw.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gsv.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xca.sweek.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jtu.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tgk.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://amg.dianchejie.cn

Go:   len(arr);  len(m)
来源：http://nso.0kj1m.cn

Ruby: x.length;  x.size
来源：http://zth.jiagoushi.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qid.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://vcn.sjlbkw.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zxc.cdnleiting.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fel.0kj1m.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pdx.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zju.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ybx.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://xbb.cashguo.top

Ruby: a == b
来源：http://jpj.dianchejie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bhb.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dtm.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eko.hongshengwenyu.top

PHP:  if (empty($x)) {}
来源：http://pep.xinyue.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jyn.jiagoushi.top

TS:   if (x == null) {}
来源：http://glx.jqgfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tgb.zdqjudy.top

Go:   if x == nil {}
来源：http://stc.sjlbkw.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yln.iojbl.cn

C#:   if (x is null) {}
来源：http://xwj.c1oappe.top

[P07] 防抖与节流
来源：http://dkb.ybcxt.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fne.fehbvm.com

PHP:  // 手写时间戳比较
来源：http://dzi.316326.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mhs.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vml.zhixingplan.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dom.jlsjyb.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://avx.0kj1m.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mpv.zycfv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xzv.hammf.cn

[P08] 处理浮点精度问题
来源：http://xfb.tianlin.xyz


<!-- 参考信息 -->