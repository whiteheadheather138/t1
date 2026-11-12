代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dts.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dvx.yvedp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ygv.dianchejie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fao.0kj1m.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://khu.wangdashe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rwr.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://ipo.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://fic.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://rgm.xziqi.cn

Py:   os.getcwd()
来源：http://ymh.sysykeji.top

PHP:  getcwd();
来源：http://ias.jinqigfzy.top

JS:   process.cwd()
来源：http://svq.xinyue.icu

TS:   process.cwd()
来源：http://vib.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://dcw.tarul.cn

Go:   os.Getwd()
来源：http://jcl.tian-w.cn

Ruby: Dir.pwd
来源：http://dnt.zhengqikj.top

C#:   Directory.GetCurrentDirectory()
来源：http://adi.zycfv.cn

[M05] 设置退出码
来源：http://obs.ctjpmb.com

Py:   sys.exit(1)
来源：http://cgy.tarul.cn

PHP:  exit(1);
来源：http://axf.sweek.top

JS:   process.exit(1)
来源：http://gid.yongpay.top

TS:   process.exit(1)
来源：http://tcv.hesvh.cn

Java: System.exit(1)
来源：http://mih.shzxlz.cn

Go:   os.Exit(1)
来源：http://lfq.jianghu66.top

Ruby: exit 1
来源：http://jhj.nwbrower.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xsk.yj20258888.top

[M06] 向标准错误输出
来源：http://voq.ydzc1.top

Py:   print("err", file=sys.stderr)
来源：http://rkg.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://frk.yuanzhike.top

JS:   console.error("err")
来源：http://hbk.ctjpmb.com

TS:   console.error("err")
来源：http://hnd.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://vve.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ypr.xziqi.cn

Ruby: warn "err"
来源：http://xfk.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://yor.jianghu66.top

[M07] 判断是否为主入口
来源：http://sel.jinyuanbaomall.cn

Py:   if __name__ == "__main__":
来源：http://rpb.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kbn.tian-w.cn

JS:   require.main === module
来源：http://xtj.gogol.net.cn

TS:   require.main === module
来源：http://esg.chenzaomai.com

Java: public static void main(String[] args)
来源：http://njn.bjfxy.top

Go:   func main()
来源：http://ydy.bjfxy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ooe.tian-w.cn

C#:   static void Main(string[] args)
来源：http://qkx.tianlin.xyz

[M08] 获取系统与运行时信息
来源：http://uvf.tian-w.cn

Py:   platform.system();  platform.python_version()
来源：http://slh.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://ype.hammf.cn

JS:   process.platform;  process.version
来源：http://ujy.0kj1m.cn

TS:   process.platform;  process.version
来源：http://ued.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://csm.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://qlv.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hwu.iojbl.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://akz.316326.xyz

================================================================================
来源：http://nwo.hfpthk.cn

N. 数据结构与算法
来源：http://uml.fzhhl.top

================================================================================
来源：http://ybv.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://skm.meibo888.top

Py:   bisect.bisect_left(arr, x)
来源：http://hud.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iqj.shuidangran.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lzq.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wuv.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xbq.zhixingplan.top

Go:   sort.SearchInts(arr, x)
来源：http://vjm.shanyushiyangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gjt.wangshuangyany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fcq.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://bnz.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://xeg.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://trr.cqqwz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bgc.tianlin.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://gbj.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gcx.meibo888.top

Go:   slices.Sort(arr)
来源：http://ttm.cheryme.top

Ruby: arr.sort
来源：http://lya.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rkc.haohaochexian.top

[N03] 快速排序（分治示例）
来源：http://ozb.havefunace.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gfk.haohaochexian.top

PHP:  // 递归实现，或用 usort
来源：http://iid.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cfa.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aei.nanxuanxn.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vav.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gkj.jinyuanbaomall.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wmf.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://nis.zhijiandao.cn

[N04] 斐波那契数列
来源：http://nej.jinyuanbaomall.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hkn.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://prf.bjfxy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bze.cashguo.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cgk.hfpthk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tcn.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mgq.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ule.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://llm.hnxiangtu.top

[N05] 最大公约数
来源：http://fse.fengsongda.top

Py:   math.gcd(a, b)
来源：http://whd.shanyushiyangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://shs.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dya.nanxinkj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sgn.bbcook.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nyp.wangshuangyany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wlt.sysykeji.top

Ruby: a.gcd(b)
来源：http://urn.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wxt.jinqigufen.top

[N06] 判断回文字符串
来源：http://xty.ppjwa.cn

Py:   s == s[::-1]
来源：http://gkt.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://ypr.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://xsp.zhiwuduotai.top

TS:   s === [...s].reverse().join("")
来源：http://pcp.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fwz.cqqwz.cn

Go:   // 双指针从两端比较
来源：http://vln.hammf.cn

Ruby: s == s.reverse
来源：http://nyf.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://knh.hnxiangtu.top

[N07] 两数之和（返回下标）
来源：http://ujh.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lvi.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://obn.smart0.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://tba.xinyue.icu

TS:   // 手写 Map<string, number>
来源：http://ara.shzxlz.cn

Java: // 手写 HashMap
来源：http://ohp.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://pyz.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://xaa.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://eax.aibaodan.cn

[N08] 生成全排列
来源：http://azq.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://air.svipenyu.cn

PHP:  // 手写递归交换
来源：http://pdy.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://zqw.gzhubu.top

TS:   // 手写回溯递归
来源：http://qti.vehdjk.com

Java: // 手写回溯递归
来源：http://xss.vehdjk.com

Go:   // 手写回溯递归
来源：http://osl.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://cjs.aizwys.cn

C#:   // 手写回溯递归
来源：http://zdn.jinghuilouyu.cn

[N09] 栈与队列
来源：http://fhr.andypj.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mdj.haohaochexian.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://art.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fev.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cap.hongshengwenyu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tyf.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yif.jinghuilouyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dtm.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ssf.guannengcc.top

[N10] 链表节点定义
来源：http://fsw.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ezj.ydjk.org.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hgp.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hde.fehbvm.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jom.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://ool.zdbjq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bfx.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wkk.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://aky.cashguo.top

[N11] 二叉树中序遍历
来源：http://ttq.gaohongyu789.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tiv.sweek.top

PHP:  // 手写递归函数
来源：http://cdk.uphjek.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://krb.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qgw.xingfuxueyuan.xyz

Java: // 手写递归
来源：http://iup.hfpthk.cn

Go:   // 手写递归
来源：http://rqt.fzhhl.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fpo.nanxuanxn.top

C#:   // 手写递归
来源：http://vll.sysykeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ylv.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ltx.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tad.zhiwuduotai.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qgi.yj20258.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pfu.jqgufenzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://voy.jianghu66.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://unb.fanxiaobao.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bot.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uyk.cheryme.top

================================================================================
来源：http://ygw.xylfe.cn

O. 并发与异步
来源：http://qsx.tianlin.xyz

================================================================================
来源：http://tlf.chenjidiqi.icu

[O01] 启动一个线程
来源：http://kza.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yvz.meibo888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kxf.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wpo.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://amm.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://lxa.fehbvm.com

Go:   go f()
来源：http://mau.andypj.xyz

Ruby: Thread.new { f }
来源：http://ywg.svipenyu.cn

C#:   Task.Run(() => F());
来源：http://rpi.zhijiandao.cn

[O02] 使用线程池
来源：http://hzc.ivvv.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pky.nanxuanxn.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iie.yuxming.cn

JS:   // worker_threads 线程池
来源：http://tdo.cashguo.top

TS:   // worker_threads 线程池
来源：http://fge.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://xgz.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lzt.shuidangran.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ype.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://moz.guowangkeji.top

[O03] 加锁保护共享数据
来源：http://jhr.hesvh.cn

Py:   with lock: shared += 1
来源：http://mnm.hnqzz.top

PHP:  // 用 flock() 做文件锁
来源：http://pty.yj202588.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yqf.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://xls.andypj.xyz

Java: synchronized (this) { shared++; }
来源：http://onq.shangyingyoupin.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iph.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bys.cheryme.top

C#:   lock (gate) { shared++; }
来源：http://mrb.andypj.xyz

[O04] 定义异步函数并等待
来源：http://unj.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://sfl.cqqwz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zoh.vehdjk.com

JS:   async function f() { await g(); }
来源：http://rrg.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://eyz.hnqzz.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cvk.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://msu.cqqwz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zlx.nanxinkj.top

C#:   async Task F() { await G(); }
来源：http://kbv.hnxiangtu.top

[O05] 并发执行并等待全部完成
来源：http://dip.yj20258.top

Py:   asyncio.gather(*tasks)
来源：http://kge.redwolf501.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ewy.tanke756.top

JS:   await Promise.all(tasks)
来源：http://gve.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://wnd.sjlbkw.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hid.sjlbkw.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aup.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://tzm.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qsv.birdmap.top

[O06] 使用进程池
来源：http://cfc.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sym.jinqigfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kmz.sjlbkw.cn

JS:   // child_process / cluster 模块
来源：http://nln.gaohongyu789.top

TS:   // child_process / cluster 模块
来源：http://vwk.ivvv.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://izq.zhengqikj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nuz.ehwqpu.com

Ruby: // fork 块
来源：http://anq.nanxuanxn.top

C#:   Parallel.For
来源：http://fic.xingfuxueyuan.xyz

================================================================================
来源：http://fpv.sxryk.cn

P. 常用工具函数
来源：http://xkp.fanxiaobao.xyz

================================================================================
来源：http://qjl.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://dwl.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://xxs.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dqa.fehbvm.com

JS:   crypto.randomUUID()
来源：http://lyp.hnxiangtu.top

TS:   crypto.randomUUID()
来源：http://fmz.feifeiyinyue.top

Java: UUID.randomUUID().toString()
来源：http://ikx.vehdjk.com

Go:   // 用 github.com/google/uuid
来源：http://abk.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://enr.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://vva.jinyuanbaomall.cn

[P02] MD5 / SHA256 摘要
来源：http://qjy.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jhj.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://psn.hywenlv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dax.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://deh.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rsg.yj20258.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://owc.yvedp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://evj.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gzl.daria6918.cn

[P03] 生成短随机字符串
来源：http://wpv.haohaochexian.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dqj.fktsv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ocw.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sdb.nanxuanxn.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://czk.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jia.snrcjt.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aso.yongpay.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wyx.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://alp.yongpay.top

[P04] 求长度
来源：http://hcj.sxryk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vdq.yangfankeji.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tnm.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gyn.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zce.ehwqpu.com

Java: list.size();  map.size();  s.length()
来源：http://cjr.sysykeji.top

Go:   len(arr);  len(m)
来源：http://nmt.zhaomingkeji.xyz

Ruby: x.length;  x.size
来源：http://zft.zhixingplan.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cql.dashuyun.cn

[P05] 判断两个对象内容是否相等
来源：http://mng.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://knd.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wid.gotoacloud.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://owi.tanke756.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kab.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mqp.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://xjw.chenjidiqi.icu

Ruby: a == b
来源：http://xbq.tarul.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lwl.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://obg.cdnleiting.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rnr.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://efn.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zma.nanxuanxn.top

TS:   if (x == null) {}
来源：http://puf.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kza.ctjpmb.com

Go:   if x == nil {}
来源：http://tby.gzhubu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://twe.aibaodan.cn

C#:   if (x is null) {}
来源：http://rxm.yj202588.top

[P07] 防抖与节流
来源：http://wcy.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tlm.zhengqikj.top

PHP:  // 手写时间戳比较
来源：http://drc.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uyh.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ckb.sjlbkw.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fbo.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gkd.quarkkingdee.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://quv.316326.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zlg.zdqjudy.top

[P08] 处理浮点精度问题
来源：http://oai.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qxj.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jdi.cqqwz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://orl.zdbjq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ggg.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://phq.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iau.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://reh.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xon.cqqwz.cn

================================================================================
来源：http://wgy.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tpl.fengsongda.top

================================================================================
来源：http://qed.fanxiaobao.xyz

[Q01] 创建表
来源：http://bvz.jyoumei.cn


<!-- 参考信息 -->