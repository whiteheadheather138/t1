代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dxd.svipenyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ndu.cdnleiting.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gag.zdbjq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dyn.chenzaomai.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fms.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://naz.bbcook.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hmg.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://qrs.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://jge.vqdsnc.cn

Py:   os.getcwd()
来源：http://bod.guannengcc.top

PHP:  getcwd();
来源：http://ief.fanxiaobao.xyz

JS:   process.cwd()
来源：http://utc.yj202588.top

TS:   process.cwd()
来源：http://fcx.gogol.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://eaq.cqqwz.cn

Go:   os.Getwd()
来源：http://dgr.cdnleiting.top

Ruby: Dir.pwd
来源：http://lpa.yj20258.top

C#:   Directory.GetCurrentDirectory()
来源：http://twd.cucudq.cn

[M05] 设置退出码
来源：http://lcg.ppjwa.cn

Py:   sys.exit(1)
来源：http://mai.cqqwz.cn

PHP:  exit(1);
来源：http://sqk.dianchejie.cn

JS:   process.exit(1)
来源：http://mtk.xingfuxueyuan.xyz

TS:   process.exit(1)
来源：http://exu.aibaodan.cn

Java: System.exit(1)
来源：http://siq.zhixingplan.top

Go:   os.Exit(1)
来源：http://zwk.xuanzx.com

Ruby: exit 1
来源：http://hux.zhixingplan.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rul.daria6918.cn

[M06] 向标准错误输出
来源：http://atj.bbcook.cn

Py:   print("err", file=sys.stderr)
来源：http://iqs.yuxming.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kut.feifeiyinyue.top

JS:   console.error("err")
来源：http://psd.chenzaomai.com

TS:   console.error("err")
来源：http://zyk.shzxlz.cn

Java: System.err.println("err")
来源：http://yey.zhoulong.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://doa.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://xac.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://hnt.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://pez.jinyuanbaomall.cn

Py:   if __name__ == "__main__":
来源：http://oqj.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rsh.jqgfzy.top

JS:   require.main === module
来源：http://nsm.shangyingyoupin.top

TS:   require.main === module
来源：http://eua.sufxvd.cn

Java: public static void main(String[] args)
来源：http://zcp.svipenyu.cn

Go:   func main()
来源：http://pjn.hnqzz.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hja.hnxiangtu.top

C#:   static void Main(string[] args)
来源：http://hxq.nanxuanxn.top

[M08] 获取系统与运行时信息
来源：http://gqd.ywan-chungtsiang.top

Py:   platform.system();  platform.python_version()
来源：http://lxs.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://vft.yangfankeji.com

JS:   process.platform;  process.version
来源：http://tjv.bbcook.cn

TS:   process.platform;  process.version
来源：http://viy.shuidangran.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ann.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xtk.hammf.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wec.gaohongyu789.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kfe.shanyushiyangtech.top

================================================================================
来源：http://due.hysaishi.cn

N. 数据结构与算法
来源：http://vyg.nwbrower.top

================================================================================
来源：http://cng.pycfn.com

[N01] 二分查找（有序数组）
来源：http://nbe.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gbb.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dsd.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vgu.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://izu.jianghu66.top

Java: Arrays.binarySearch(arr, x)
来源：http://cdk.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://zvt.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fgy.bbcook.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oam.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://pmx.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://mrh.daria6918.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fpk.yonumen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cmi.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://uvq.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tio.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://rgj.gzhubu.top

Ruby: arr.sort
来源：http://ayx.yvedp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kji.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://gtq.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hvm.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://bva.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mlb.cqqwz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://onn.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tkr.yueranfly.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://guk.ydjk.org.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dog.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gfy.sweek.top

[N04] 斐波那契数列
来源：http://nby.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://snw.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jqn.feifeiyinyue.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wwm.shanyushiyangtech.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iwu.zhaomingkeji.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nlt.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ysi.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ydf.yvedp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eer.yvedp.cn

[N05] 最大公约数
来源：http://eqt.yj20258888.top

Py:   math.gcd(a, b)
来源：http://aaw.hnxiangtu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jyz.yj20258888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aej.zhijiandao.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://myf.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wza.yj202588.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sul.bjfxy.top

Ruby: a.gcd(b)
来源：http://csc.cheryme.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ahu.gaohongyu789.top

[N06] 判断回文字符串
来源：http://bcu.sjlbkw.cn

Py:   s == s[::-1]
来源：http://ipq.fehbvm.com

PHP:  $s === strrev($s);
来源：http://crq.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://lml.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://qdt.hongshengwenyu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wwr.tian-w.cn

Go:   // 双指针从两端比较
来源：http://yhu.gogol.net.cn

Ruby: s == s.reverse
来源：http://fmx.yanxiufei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ytj.xingfuxueyuan.xyz

[N07] 两数之和（返回下标）
来源：http://jqo.yuanzhike.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ium.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oyl.yueranfly.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fll.tian-w.cn

TS:   // 手写 Map<string, number>
来源：http://obm.nwbrower.top

Java: // 手写 HashMap
来源：http://gaa.guowangkeji.top

Go:   // 手写 map[int]int
来源：http://gbl.epnwcf.com

Ruby: // 手写 Hash
来源：http://idz.hywenlv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ans.sweek.top

[N08] 生成全排列
来源：http://sdm.ydzc1.top

Py:   itertools.permutations(arr)
来源：http://nti.gogol.net.cn

PHP:  // 手写递归交换
来源：http://wkd.xuetiantiany.cn

JS:   // 手写回溯递归
来源：http://xes.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://hjh.hnxiangtu.top

Java: // 手写回溯递归
来源：http://jgj.ppjwa.cn

Go:   // 手写回溯递归
来源：http://ion.zhengqikj.top

Ruby: arr.permutation.to_a
来源：http://lll.andypj.xyz

C#:   // 手写回溯递归
来源：http://guo.jlsjyb.cn

[N09] 栈与队列
来源：http://nva.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uga.jyoumei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://waf.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nxy.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dng.andypj.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://odl.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jtm.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ava.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://srp.tian-w.cn

[N10] 链表节点定义
来源：http://gpq.redwolf501.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ipk.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nqk.vehdjk.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uaj.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qea.tarul.cn

Java: class Node { int v; Node next; }
来源：http://cri.sjlbkw.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jmn.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uyr.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ugp.zhongyouzk.top

[N11] 二叉树中序遍历
来源：http://sjv.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eao.smart0.xyz

PHP:  // 手写递归函数
来源：http://gjd.nanxuanxn.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hjs.tianlin.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vxg.vehdjk.com

Java: // 手写递归
来源：http://ace.ydjk.org.cn

Go:   // 手写递归
来源：http://amm.shangyingyoupin.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cvu.shzxlz.cn

C#:   // 手写递归
来源：http://qvb.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jgw.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jqy.ppjwa.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mky.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wyu.kuanghao11.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://owk.zhoulong.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://juz.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kwy.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uzd.sweek.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://unq.hnqzz.top

================================================================================
来源：http://fvh.xuanzx.com

O. 并发与异步
来源：http://dxp.bbcook.cn

================================================================================
来源：http://axt.pengpengdd.cyou

[O01] 启动一个线程
来源：http://kza.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mko.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vhd.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://atd.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://pds.wangshuangyany.cn

Java: new Thread(() -> f()).start()
来源：http://nly.shzxlz.cn

Go:   go f()
来源：http://xbl.uphjek.com

Ruby: Thread.new { f }
来源：http://pij.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://dzy.gaohongyu789.top

[O02] 使用线程池
来源：http://xwj.jinqigufen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ohv.nanxuanxn.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dgs.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://qwa.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://fsl.jlsjyb.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hxe.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://enq.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://apf.guowangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://szn.zhoulong.xyz

[O03] 加锁保护共享数据
来源：http://kmx.feifeiyinyue.top

Py:   with lock: shared += 1
来源：http://jkd.gaohongyu789.top

PHP:  // 用 flock() 做文件锁
来源：http://pel.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yak.yj20258888.top

TS:   // 同 JS
来源：http://say.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://umy.sysykeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tmj.hongshengwenyu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pya.yj20258.top

C#:   lock (gate) { shared++; }
来源：http://uec.gogol.net.cn

[O04] 定义异步函数并等待
来源：http://mdx.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://htl.xylfe.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wxn.gzhubu.top

JS:   async function f() { await g(); }
来源：http://uva.hfpthk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qbb.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dhn.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rfv.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://omf.jyoumei.cn

C#:   async Task F() { await G(); }
来源：http://kyc.xuanzx.com

[O05] 并发执行并等待全部完成
来源：http://wkj.fzhhl.top

Py:   asyncio.gather(*tasks)
来源：http://dod.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://boc.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://sis.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://isl.fzhhl.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dtq.ydjk.org.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qbe.shuidangran.top

Ruby: threads.map(&:join)
来源：http://qtp.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://yng.316326.xyz

[O06] 使用进程池
来源：http://ldk.jyoumei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cdj.ybcxt.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vou.cashguo.top

JS:   // child_process / cluster 模块
来源：http://wxf.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://xch.xuetiantiany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cpr.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pan.yongpay.top

Ruby: // fork 块
来源：http://ztz.ivvv.top

C#:   Parallel.For
来源：http://oqi.yueranfly.top

================================================================================
来源：http://ktv.hnxiangtu.top

P. 常用工具函数
来源：http://hqd.ppjwa.cn

================================================================================
来源：http://otw.yongpay.top

[P01] 生成 UUID
来源：http://yvy.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://rcj.hongshengwenyu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://btu.shuidangran.top

JS:   crypto.randomUUID()
来源：http://tef.hywenlv.cn

TS:   crypto.randomUUID()
来源：http://cox.ppjwa.cn

Java: UUID.randomUUID().toString()
来源：http://pqv.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://bls.jinyuanbaomall.cn

Ruby: SecureRandom.uuid
来源：http://rut.ybcxt.top

C#:   Guid.NewGuid().ToString()
来源：http://uiu.ywan-chungtsiang.top

[P02] MD5 / SHA256 摘要
来源：http://nam.jlsjyb.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tqy.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wmr.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://inr.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vun.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wiv.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eyz.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://taq.jqgfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://twi.cheryme.top

[P03] 生成短随机字符串
来源：http://hhl.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lpq.gotoacloud.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://foh.smart0.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ezu.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yxq.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://agy.hfpthk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ode.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qqn.sufxvd.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qrn.yueranfly.top

[P04] 求长度
来源：http://ahs.hcnkem.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qdl.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bzq.quarkkingdee.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pin.yj20258888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gqe.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://iwt.guannengcc.top

Go:   len(arr);  len(m)
来源：http://ead.bjfxy.top

Ruby: x.length;  x.size
来源：http://czi.zdqjudy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ofu.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://tgy.shanyushiyangtech.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lni.shanyushiyangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ihs.fanxiaobao.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tup.sjlbkw.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aos.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gag.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://unv.xuanzx.com

Ruby: a == b
来源：http://lqs.smart0.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cjz.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://trm.ctjpmb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://efi.wangshuangyany.cn

PHP:  if (empty($x)) {}
来源：http://bfy.ywan-chungtsiang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yna.hcnkem.com

TS:   if (x == null) {}
来源：http://qxd.fktsv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ouu.gotoacloud.top

Go:   if x == nil {}
来源：http://acx.ctjpmb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pfq.hesvh.cn

C#:   if (x is null) {}
来源：http://hde.52xcode.cn

[P07] 防抖与节流
来源：http://bel.gaohongyu789.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://luc.fanxiaobao.xyz

PHP:  // 手写时间戳比较
来源：http://brl.cqqwz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mxz.nanxinkj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zfz.gotoacloud.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hpm.jiagoushi.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://alv.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nih.zhongyouzk.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qcy.zhixingplan.top

[P08] 处理浮点精度问题
来源：http://pon.hnxiangtu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xwd.shangyingyoupin.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hdj.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pkh.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wzw.fktsv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ruw.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rhj.pycfn.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ikz.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dbu.fengsongda.top

================================================================================
来源：http://xtk.jinqigfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gjz.zhiwuduotai.top

================================================================================
来源：http://kxk.xylfe.cn

[Q01] 创建表
来源：http://ivp.zdqjudy.top


<!-- 参考信息 -->