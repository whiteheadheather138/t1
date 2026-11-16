代发 wailian999

Ruby: ARGV
来源：http://rfj.jinqigufen.top

C#:   args 数组（Main 方法参数）
来源：http://cia.cucudq.cn

[M02] 读取环境变量
来源：http://lqa.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://plv.hammf.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jfd.quarkkingdee.top

JS:   process.env.HOME
来源：http://mfr.fanxiaobao.xyz

TS:   process.env.HOME
来源：http://dok.ydzc1.top

Java: System.getenv("HOME")
来源：http://mlq.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sff.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://bxq.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dxd.jinqigufen.top

[M03] 执行外部命令
来源：http://ixc.hysaishi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://emj.zhongyouzk.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://won.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wbj.tanke756.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vbv.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lal.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kcm.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://czy.yuxming.cn

C#:   Process.Start("ls", "-l");
来源：http://lfj.fengsongda.top

[M04] 获取当前工作目录
来源：http://hur.zhoulong.xyz

Py:   os.getcwd()
来源：http://efb.zycfv.cn

PHP:  getcwd();
来源：http://adv.yonumen.top

JS:   process.cwd()
来源：http://hoo.haohaochexian.top

TS:   process.cwd()
来源：http://pcw.gogol.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://axe.jqgufenzy.top

Go:   os.Getwd()
来源：http://bcb.cheryme.top

Ruby: Dir.pwd
来源：http://lch.gzhubu.top

C#:   Directory.GetCurrentDirectory()
来源：http://bze.hysaishi.cn

[M05] 设置退出码
来源：http://two.jinqigfzy.top

Py:   sys.exit(1)
来源：http://uni.dianchejie.cn

PHP:  exit(1);
来源：http://vgj.gogol.net.cn

JS:   process.exit(1)
来源：http://uyc.daria6918.cn

TS:   process.exit(1)
来源：http://xwp.9152youxi.cn

Java: System.exit(1)
来源：http://yzp.hnxiangtu.top

Go:   os.Exit(1)
来源：http://jcy.jianghu66.top

Ruby: exit 1
来源：http://wpv.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xeo.jinqigfzy.top

[M06] 向标准错误输出
来源：http://fwl.ybcxt.top

Py:   print("err", file=sys.stderr)
来源：http://nrs.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://moj.wangshuangyany.cn

JS:   console.error("err")
来源：http://vju.jqgufenzy.top

TS:   console.error("err")
来源：http://rdn.wangshuangyany.cn

Java: System.err.println("err")
来源：http://ucg.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dmp.hnxiangtu.top

Ruby: warn "err"
来源：http://pgn.xylfe.cn

C#:   Console.Error.WriteLine("err")
来源：http://pyh.gogol.net.cn

[M07] 判断是否为主入口
来源：http://eip.meibo888.top

Py:   if __name__ == "__main__":
来源：http://azu.hywenlv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wad.redwolf501.top

JS:   require.main === module
来源：http://ggv.zdqjudy.top

TS:   require.main === module
来源：http://amq.xinyue.icu

Java: public static void main(String[] args)
来源：http://upj.dianchejie.cn

Go:   func main()
来源：http://eec.andypj.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ukl.xziqi.cn

C#:   static void Main(string[] args)
来源：http://cuf.zhaomingkeji.xyz

[M08] 获取系统与运行时信息
来源：http://yjv.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://exz.9152youxi.cn

PHP:  PHP_OS;  phpversion();
来源：http://bil.cheryme.top

JS:   process.platform;  process.version
来源：http://miy.guannengcc.top

TS:   process.platform;  process.version
来源：http://gux.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nyb.hnqzz.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rwq.xylfe.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vxl.jyoumei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kgq.svipenyu.cn

================================================================================
来源：http://kyt.yangfankeji.com

N. 数据结构与算法
来源：http://gvf.feifeiyinyue.top

================================================================================
来源：http://fub.sxryk.cn

[N01] 二分查找（有序数组）
来源：http://mpy.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://ffd.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://acp.fanxiaobao.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dey.haohaochexian.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vij.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kyl.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://yms.shanyushiyangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ldx.gaohongyu789.top

C#:   Array.BinarySearch(arr, x)
来源：http://nao.hfpthk.cn

[N02] 排序（工程实践用内置实现）
来源：http://idu.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://yvd.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://stb.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yta.vehdjk.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://yvw.shuidangran.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jay.xylfe.cn

Go:   slices.Sort(arr)
来源：http://wth.nanxuanxn.top

Ruby: arr.sort
来源：http://ire.yuanzhike.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ojb.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://nar.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cob.xuetiantiany.cn

PHP:  // 递归实现，或用 usort
来源：http://ygm.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://shh.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yet.yvedp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sxh.guannengcc.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://acr.nwbrower.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kyd.zhongyouzk.top

C#:   // 手写递归，或 Array.Sort
来源：http://lfk.sxryk.cn

[N04] 斐波那契数列
来源：http://zxi.feifeiyinyue.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nne.316326.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vjd.nwbrower.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://opl.hongshengwenyu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cth.tianlin.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vfq.shanyushiyangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qgr.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://him.tarul.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jdc.chenjidiqi.icu

[N05] 最大公约数
来源：http://mbg.xziqi.cn

Py:   math.gcd(a, b)
来源：http://bgf.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jro.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qar.jinqigufen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wmi.cucudq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zvd.gotoacloud.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gla.chenzaomai.com

Ruby: a.gcd(b)
来源：http://duj.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rzf.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://cco.ppjwa.cn

Py:   s == s[::-1]
来源：http://tnw.xingfuxueyuan.xyz

PHP:  $s === strrev($s);
来源：http://bxq.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://jco.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://gbr.yongpay.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mst.zhongyouzk.top

Go:   // 双指针从两端比较
来源：http://kne.ehwqpu.com

Ruby: s == s.reverse
来源：http://dzx.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ptr.tanke756.top

[N07] 两数之和（返回下标）
来源：http://pkg.jqgufenzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://klt.nwbrower.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gmw.hywenlv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://joo.guannengcc.top

TS:   // 手写 Map<string, number>
来源：http://put.daxiang520.top

Java: // 手写 HashMap
来源：http://wgu.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://ypy.ybcxt.top

Ruby: // 手写 Hash
来源：http://twl.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://rcu.daria6918.cn

[N08] 生成全排列
来源：http://are.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://juu.hysaishi.cn

PHP:  // 手写递归交换
来源：http://bwn.xziqi.cn

JS:   // 手写回溯递归
来源：http://wfj.hnqzz.top

TS:   // 手写回溯递归
来源：http://rcw.tarul.cn

Java: // 手写回溯递归
来源：http://ugr.tian-w.cn

Go:   // 手写回溯递归
来源：http://ukw.hongshengwenyu.top

Ruby: arr.permutation.to_a
来源：http://mub.andypj.xyz

C#:   // 手写回溯递归
来源：http://odw.hongshengwenyu.top

[N09] 栈与队列
来源：http://rmg.yueranfly.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gog.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xdd.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gxr.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://syl.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qhd.meibo888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rez.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ajn.fzhhl.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qnm.uphjek.com

[N10] 链表节点定义
来源：http://eov.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tfa.hammf.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nfe.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vvm.zhijiandao.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://shl.vqdsnc.cn

Java: class Node { int v; Node next; }
来源：http://ghq.fktsv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ldz.sweek.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ekx.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fdr.cashguo.top

[N11] 二叉树中序遍历
来源：http://knq.meibo888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bmr.zdbjq.cn

PHP:  // 手写递归函数
来源：http://psg.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wow.andypj.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://otu.jlsjyb.cn

Java: // 手写递归
来源：http://adr.ydzc1.top

Go:   // 手写递归
来源：http://uew.wangdashe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qjg.wangshuangyany.cn

C#:   // 手写递归
来源：http://sng.cdnleiting.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tym.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://raz.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ebl.yfazqb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://beh.zdbjq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bob.aibaodan.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yia.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cyf.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zre.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bau.sxryk.cn

================================================================================
来源：http://jzr.gzhubu.top

O. 并发与异步
来源：http://yyl.hnxiangtu.top

================================================================================
来源：http://xia.zhoulong.xyz

[O01] 启动一个线程
来源：http://mkr.ywan-chungtsiang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qnx.c1oappe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zcs.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tfe.9152youxi.cn

TS:   // 同 JS
来源：http://szs.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://ipc.nanxuanxn.top

Go:   go f()
来源：http://qoi.c1oappe.top

Ruby: Thread.new { f }
来源：http://evw.ctjpmb.com

C#:   Task.Run(() => F());
来源：http://jiw.nanxinkj.top

[O02] 使用线程池
来源：http://ucy.guannengcc.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iia.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lgf.meibo888.top

JS:   // worker_threads 线程池
来源：http://mlp.shangyingyoupin.top

TS:   // worker_threads 线程池
来源：http://tac.ybcxt.top

Java: Executors.newFixedThreadPool(4)
来源：http://ofb.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ruy.chenzaomai.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rat.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zod.yj20258.top

[O03] 加锁保护共享数据
来源：http://tuw.xuetiantiany.cn

Py:   with lock: shared += 1
来源：http://rho.daria6918.cn

PHP:  // 用 flock() 做文件锁
来源：http://dfs.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pzm.pengpengdd.cyou

TS:   // 同 JS
来源：http://hjf.jinqigufen.top

Java: synchronized (this) { shared++; }
来源：http://vio.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xef.feifeiyinyue.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nbb.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://yas.hywenlv.cn

[O04] 定义异步函数并等待
来源：http://amo.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://jzx.jqgfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://paw.birdmap.top

JS:   async function f() { await g(); }
来源：http://ryz.yueranfly.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vyv.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pbb.hesvh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lle.hnxiangtu.top

Ruby: # 用 Fiber 或 async gem
来源：http://yos.hesvh.cn

C#:   async Task F() { await G(); }
来源：http://sqy.chenjidiqi.icu

[O05] 并发执行并等待全部完成
来源：http://cgr.yonumen.top

Py:   asyncio.gather(*tasks)
来源：http://dzd.zhixingplan.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ekq.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://yie.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://yns.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wrr.yj20258.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kky.yj202588.top

Ruby: threads.map(&:join)
来源：http://gxn.ehwqpu.com

C#:   await Task.WhenAll(t1, t2)
来源：http://eaa.zhengqikj.top

[O06] 使用进程池
来源：http://upo.uphjek.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gct.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vrm.redwolf501.top

JS:   // child_process / cluster 模块
来源：http://yjq.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://vsw.smart0.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rgt.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xkc.pycfn.com

Ruby: // fork 块
来源：http://jlz.yj20258.top

C#:   Parallel.For
来源：http://pyl.tianlin.xyz

================================================================================
来源：http://ypb.meibo888.top

P. 常用工具函数
来源：http://bil.fehbvm.com

================================================================================
来源：http://twi.jqgfzy.top

[P01] 生成 UUID
来源：http://xfj.ctjpmb.com

Py:   str(uuid.uuid4())
来源：http://cqf.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xoe.tian-w.cn

JS:   crypto.randomUUID()
来源：http://pie.yuanzhike.top

TS:   crypto.randomUUID()
来源：http://nhm.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://ldg.jinyuanbaomall.cn

Go:   // 用 github.com/google/uuid
来源：http://jcd.zdqjudy.top

Ruby: SecureRandom.uuid
来源：http://tlp.xinyue.icu

C#:   Guid.NewGuid().ToString()
来源：http://jgr.hammf.cn

[P02] MD5 / SHA256 摘要
来源：http://lnx.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tzb.316326.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://yfv.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://crq.sufxvd.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wdz.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fny.shzxlz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qdd.bjfxy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ksf.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bso.daxiang520.top

[P03] 生成短随机字符串
来源：http://zhy.yanxiufei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vfi.ehwqpu.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hwz.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://owv.svipenyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mxa.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zen.daria6918.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ybz.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ihh.guannengcc.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://epf.dashuyun.cn

[P04] 求长度
来源：http://qpj.gaohongyu789.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uys.guannengcc.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qro.sysykeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pmk.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lfu.cheryme.top

Java: list.size();  map.size();  s.length()
来源：http://xkg.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://euw.sxryk.cn

Ruby: x.length;  x.size
来源：http://ffx.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://efq.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://kjf.dianchejie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sfo.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wnf.zhijiandao.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pcd.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hrx.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tiv.chenzaomai.com

Go:   reflect.DeepEqual(a, b)
来源：http://qhm.xuanzx.com

Ruby: a == b
来源：http://rlc.yfazqb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ayf.aizwys.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vpd.yj20258.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://inj.chenjidiqi.icu

PHP:  if (empty($x)) {}
来源：http://ahz.xinyue.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fma.gogol.net.cn

TS:   if (x == null) {}
来源：http://qbh.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vtc.9152youxi.cn

Go:   if x == nil {}
来源：http://hgu.ctjpmb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://izi.hammf.cn

C#:   if (x is null) {}
来源：http://rsv.tanke756.top

[P07] 防抖与节流
来源：http://tql.cqqwz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://met.yueranfly.top

PHP:  // 手写时间戳比较
来源：http://axh.fzhhl.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jqc.xziqi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hgw.c1oappe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xcl.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eoa.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ktk.yfazqb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rvp.ydzc1.top

[P08] 处理浮点精度问题
来源：http://qag.andypj.xyz


<!-- 参考信息 -->