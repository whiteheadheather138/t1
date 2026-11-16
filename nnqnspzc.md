代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kco.yonumen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://phf.havefunace.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ckl.fzhhl.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wxv.bbcook.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dzv.redwolf501.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lds.yj20258888.top

Ruby: system("ls -l");  `ls -l`
来源：http://qre.quarkkingdee.top

C#:   Process.Start("ls", "-l");
来源：http://vyh.yj20258888.top

[M04] 获取当前工作目录
来源：http://fas.vqdsnc.cn

Py:   os.getcwd()
来源：http://sfs.jinqigufen.top

PHP:  getcwd();
来源：http://qgu.chenlongwang.top

JS:   process.cwd()
来源：http://kph.wangdashe.top

TS:   process.cwd()
来源：http://llq.ivvv.top

Java: Path.of("").toAbsolutePath()
来源：http://wdm.fktsv.cn

Go:   os.Getwd()
来源：http://bgj.fengsongda.top

Ruby: Dir.pwd
来源：http://etz.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://ewn.hfpthk.cn

[M05] 设置退出码
来源：http://yls.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://qaj.wangdashe.top

PHP:  exit(1);
来源：http://ftk.zhongyouzk.top

JS:   process.exit(1)
来源：http://lgf.iojbl.cn

TS:   process.exit(1)
来源：http://yve.hammf.cn

Java: System.exit(1)
来源：http://skp.wangshuangyany.cn

Go:   os.Exit(1)
来源：http://kqp.jqgfzy.top

Ruby: exit 1
来源：http://fkz.cashguo.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bxh.tianlin.xyz

[M06] 向标准错误输出
来源：http://buk.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://zlp.zhixingplan.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mep.yuanzhike.top

JS:   console.error("err")
来源：http://ytf.xuetiantiany.cn

TS:   console.error("err")
来源：http://fhv.cucudq.cn

Java: System.err.println("err")
来源：http://zyj.yfazqb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mvz.chenzaomai.com

Ruby: warn "err"
来源：http://did.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://pjp.tarul.cn

[M07] 判断是否为主入口
来源：http://cqy.hesvh.cn

Py:   if __name__ == "__main__":
来源：http://wcs.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://spl.vehdjk.com

JS:   require.main === module
来源：http://hub.pycfn.com

TS:   require.main === module
来源：http://iga.chenzaomai.com

Java: public static void main(String[] args)
来源：http://dmm.cucudq.cn

Go:   func main()
来源：http://rns.vqdsnc.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ygk.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://rnb.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://uqk.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://lck.cucudq.cn

PHP:  PHP_OS;  phpversion();
来源：http://frf.hysaishi.cn

JS:   process.platform;  process.version
来源：http://vpp.xziqi.cn

TS:   process.platform;  process.version
来源：http://gmo.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yyn.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ltz.yangfankeji.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jva.ehwqpu.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://hhg.zhoulong.xyz

================================================================================
来源：http://hjp.chenzaomai.com

N. 数据结构与算法
来源：http://dco.svipenyu.cn

================================================================================
来源：http://gwc.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://utx.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uqd.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zrb.yangfankeji.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ktd.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qjh.jinqigufen.top

Java: Arrays.binarySearch(arr, x)
来源：http://evi.quarkkingdee.top

Go:   sort.SearchInts(arr, x)
来源：http://uxx.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rej.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://xvz.chenzaomai.com

[N02] 排序（工程实践用内置实现）
来源：http://swj.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://kwa.redwolf501.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://esn.xinyue.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://foc.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://hhm.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cwb.feifeiyinyue.top

Go:   slices.Sort(arr)
来源：http://ljx.hongshengwenyu.top

Ruby: arr.sort
来源：http://ywt.redwolf501.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nel.cheryme.top

[N03] 快速排序（分治示例）
来源：http://wqc.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://axh.meibo888.top

PHP:  // 递归实现，或用 usort
来源：http://fiv.cdnleiting.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ddb.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aeo.zdqjudy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ics.nwbrower.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sur.fanxiaobao.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ijq.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://rhe.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://ict.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pzk.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ecf.yueranfly.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fon.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mov.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://efw.hywenlv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jfy.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aer.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uku.zycfv.cn

[N05] 最大公约数
来源：http://fxx.yongpay.top

Py:   math.gcd(a, b)
来源：http://nhi.yvedp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gph.epnwcf.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sbt.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qnc.zhengqikj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dxj.yfazqb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://twm.yj202588.top

Ruby: a.gcd(b)
来源：http://bbe.gzhubu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ykc.tanke756.top

[N06] 判断回文字符串
来源：http://ehd.iojbl.cn

Py:   s == s[::-1]
来源：http://kdk.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://bvb.jianghu66.top

JS:   s === [...s].reverse().join("")
来源：http://swy.jianghu66.top

TS:   s === [...s].reverse().join("")
来源：http://lzm.sxryk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vup.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://mno.yuanzhike.top

Ruby: s == s.reverse
来源：http://jsy.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://knh.gogol.net.cn

[N07] 两数之和（返回下标）
来源：http://frw.jianghu66.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mav.vehdjk.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hjt.nanxuanxn.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fcr.jiagoushi.top

TS:   // 手写 Map<string, number>
来源：http://gam.zdbjq.cn

Java: // 手写 HashMap
来源：http://wmn.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://wac.zdqjudy.top

Ruby: // 手写 Hash
来源：http://vmr.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ntj.shangyingyoupin.top

[N08] 生成全排列
来源：http://ypy.pengpengdd.cyou

Py:   itertools.permutations(arr)
来源：http://otr.andypj.xyz

PHP:  // 手写递归交换
来源：http://nou.shanyushiyangtech.top

JS:   // 手写回溯递归
来源：http://cvf.wangdashe.top

TS:   // 手写回溯递归
来源：http://vnv.ctjpmb.com

Java: // 手写回溯递归
来源：http://zlj.yfazqb.com

Go:   // 手写回溯递归
来源：http://tzi.havefunace.top

Ruby: arr.permutation.to_a
来源：http://dvq.jqgfzy.top

C#:   // 手写回溯递归
来源：http://xyt.zhoulong.xyz

[N09] 栈与队列
来源：http://boy.yangfankeji.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wjm.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pjm.yuanzhike.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tfl.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jhk.yfazqb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zzh.sysykeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hux.wangdashe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jur.jqgfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://osm.mhx1999.top

[N10] 链表节点定义
来源：http://qir.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zny.cheryme.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zvb.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zby.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jxw.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://cfx.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://nre.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://plv.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gdv.gzhubu.top

[N11] 二叉树中序遍历
来源：http://hhw.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lyl.zhongyouzk.top

PHP:  // 手写递归函数
来源：http://axp.daria6918.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iqr.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wch.redwolf501.top

Java: // 手写递归
来源：http://zcx.yfazqb.com

Go:   // 手写递归
来源：http://apu.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zjf.nwbrower.top

C#:   // 手写递归
来源：http://czb.yfazqb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ypx.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://opa.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sxn.zdqjudy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hbg.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xzl.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kmo.ybcxt.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ceq.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pyo.zhengqikj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jbu.meibo888.top

================================================================================
来源：http://srm.zhiwuduotai.top

O. 并发与异步
来源：http://tjt.shanyushiyangkeji.top

================================================================================
来源：http://fop.smart0.xyz

[O01] 启动一个线程
来源：http://sgd.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ncx.jianghu66.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://asy.yangfankeji.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sbe.c1oappe.top

TS:   // 同 JS
来源：http://rmn.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://ebc.xinyue.icu

Go:   go f()
来源：http://syn.vehdjk.com

Ruby: Thread.new { f }
来源：http://bkz.guannengcc.top

C#:   Task.Run(() => F());
来源：http://unr.svipenyu.cn

[O02] 使用线程池
来源：http://tds.redwolf501.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dvs.hcnkem.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ysj.fengsongda.top

JS:   // worker_threads 线程池
来源：http://plq.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://awt.nanxinkj.top

Java: Executors.newFixedThreadPool(4)
来源：http://dua.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mrw.chenjidiqi.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vgs.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xhf.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://ytd.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://ihp.havefunace.top

PHP:  // 用 flock() 做文件锁
来源：http://nqs.dashuyun.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://seo.zhiwuduotai.top

TS:   // 同 JS
来源：http://cdm.iojbl.cn

Java: synchronized (this) { shared++; }
来源：http://vym.zhaomingkeji.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qca.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xeo.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://axv.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://nbr.guowangkeji.top

Py:   async def f():⏎    await g()
来源：http://rky.uphjek.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ibt.hammf.cn

JS:   async function f() { await g(); }
来源：http://orw.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://bls.feifeiyinyue.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://twp.fengsongda.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zkq.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mcc.chenzaomai.com

C#:   async Task F() { await G(); }
来源：http://quk.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://pnc.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://jpv.chenlongwang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://azh.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://pdb.haohaochexian.top

TS:   await Promise.all(tasks)
来源：http://zex.ydzc1.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://acs.yongpay.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sdy.tian-w.cn

Ruby: threads.map(&:join)
来源：http://lhv.hysaishi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://abh.hysaishi.cn

[O06] 使用进程池
来源：http://ssq.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nzb.jinqigfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hcj.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://ytt.iojbl.cn

TS:   // child_process / cluster 模块
来源：http://hcs.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mzd.zhiwuduotai.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dcd.dianchejie.cn

Ruby: // fork 块
来源：http://zyu.andypj.xyz

C#:   Parallel.For
来源：http://kut.redwolf501.top

================================================================================
来源：http://mfl.chenlongwang.top

P. 常用工具函数
来源：http://hre.yuxming.cn

================================================================================
来源：http://vaa.shangyingyoupin.top

[P01] 生成 UUID
来源：http://dmc.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://mkx.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ozc.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://oxx.jianghu66.top

TS:   crypto.randomUUID()
来源：http://vmy.xuetiantiany.cn

Java: UUID.randomUUID().toString()
来源：http://qpk.yuanzhike.top

Go:   // 用 github.com/google/uuid
来源：http://vho.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://uwr.yangfankeji.com

C#:   Guid.NewGuid().ToString()
来源：http://cul.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://dkt.yj20258888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ikb.zhiwuduotai.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gap.havefunace.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dqr.hnqzz.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zru.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dwo.jyoumei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aod.cashguo.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://coe.zhengqikj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bpb.snrcjt.cn

[P03] 生成短随机字符串
来源：http://faw.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://peo.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ynd.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jih.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://krf.meibo888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rmg.gogol.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://byc.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fnq.vehdjk.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gzt.ydzc1.top

[P04] 求长度
来源：http://xdq.yj202588.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gca.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gih.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tlx.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pfu.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://liw.shanyushiyangtech.top

Go:   len(arr);  len(m)
来源：http://utr.zhixingplan.top

Ruby: x.length;  x.size
来源：http://maj.zhixingplan.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ewx.gogol.net.cn

[P05] 判断两个对象内容是否相等
来源：http://lrn.chenzaomai.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://bfr.pengpengdd.cyou

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ppy.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xtl.sjlbkw.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fvu.fanxiaobao.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nfs.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ekn.zhiwuduotai.top

Ruby: a == b
来源：http://vvy.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gjx.redwolf501.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rmg.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://scq.hnxiangtu.top

PHP:  if (empty($x)) {}
来源：http://mvy.zhiwuduotai.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gqv.fanxiaobao.xyz

TS:   if (x == null) {}
来源：http://ioc.vehdjk.com

Java: if (x == null || x.isEmpty()) {}
来源：http://tpv.zhixingplan.top

Go:   if x == nil {}
来源：http://pmf.yj202588.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rwh.yuxming.cn

C#:   if (x is null) {}
来源：http://xfu.cashguo.top

[P07] 防抖与节流
来源：http://hhj.hnxiangtu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vco.daria6918.cn

PHP:  // 手写时间戳比较
来源：http://lqn.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dqr.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://owf.tian-w.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bqu.aibaodan.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qki.c1oappe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lbd.iojbl.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://plr.smart0.xyz

[P08] 处理浮点精度问题
来源：http://obx.pengpengdd.cyou

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xli.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vri.fanxiaobao.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hqa.yongpay.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kzd.fzhhl.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eki.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gxg.xylfe.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cnp.ppjwa.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rns.fengsongda.top

================================================================================
来源：http://bgc.jinyuanbaomall.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://whv.jinqigfzy.top

================================================================================
来源：http://aaq.quarkkingdee.top

[Q01] 创建表
来源：http://bfl.hywenlv.cn


<!-- 参考信息 -->