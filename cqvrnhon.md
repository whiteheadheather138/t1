代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cdi.yj20258.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lea.vehdjk.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ain.jinyuanbaomall.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rqp.shzxlz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eon.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://lag.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pma.wangshuangyany.cn

C#:   Process.Start("ls", "-l");
来源：http://wph.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://nfy.c1oappe.top

Py:   os.getcwd()
来源：http://wzd.yj20258.top

PHP:  getcwd();
来源：http://aba.jqgfzy.top

JS:   process.cwd()
来源：http://ojc.hysaishi.cn

TS:   process.cwd()
来源：http://hkm.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://owh.daria6918.cn

Go:   os.Getwd()
来源：http://mli.hesvh.cn

Ruby: Dir.pwd
来源：http://rxb.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://zql.pycfn.com

[M05] 设置退出码
来源：http://jxd.dashuyun.cn

Py:   sys.exit(1)
来源：http://tso.birdmap.top

PHP:  exit(1);
来源：http://xrl.jianghu66.top

JS:   process.exit(1)
来源：http://snp.cdnleiting.top

TS:   process.exit(1)
来源：http://ipa.fehbvm.com

Java: System.exit(1)
来源：http://ldy.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://mba.xuetiantiany.cn

Ruby: exit 1
来源：http://ytc.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ihv.yuanzhike.top

[M06] 向标准错误输出
来源：http://nvq.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://cit.c1oappe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tgw.chenjidiqi.icu

JS:   console.error("err")
来源：http://waj.smart0.xyz

TS:   console.error("err")
来源：http://igr.cucudq.cn

Java: System.err.println("err")
来源：http://ipr.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nwf.zhixingplan.top

Ruby: warn "err"
来源：http://cao.jiagoushi.top

C#:   Console.Error.WriteLine("err")
来源：http://ejz.xinyue.icu

[M07] 判断是否为主入口
来源：http://zxd.sysykeji.top

Py:   if __name__ == "__main__":
来源：http://ltb.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nlt.nanxinkj.top

JS:   require.main === module
来源：http://uft.ydzc1.top

TS:   require.main === module
来源：http://taw.0kj1m.cn

Java: public static void main(String[] args)
来源：http://ydi.nanxinkj.top

Go:   func main()
来源：http://ahy.hnqzz.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ygo.jinghuilouyu.cn

C#:   static void Main(string[] args)
来源：http://phn.gotoacloud.top

[M08] 获取系统与运行时信息
来源：http://ysu.meibo888.top

Py:   platform.system();  platform.python_version()
来源：http://fei.bjfxy.top

PHP:  PHP_OS;  phpversion();
来源：http://fqp.sufxvd.cn

JS:   process.platform;  process.version
来源：http://hes.guowangkeji.top

TS:   process.platform;  process.version
来源：http://sxh.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zlh.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://dtf.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wmv.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rzx.shanyushiyangtech.top

================================================================================
来源：http://gah.andypj.xyz

N. 数据结构与算法
来源：http://dyh.shangyingyoupin.top

================================================================================
来源：http://vjl.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://ngf.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gtn.yongpay.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tlc.ywan-chungtsiang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fhp.hesvh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zjf.yj202588.top

Java: Arrays.binarySearch(arr, x)
来源：http://jfn.shangyingyoupin.top

Go:   sort.SearchInts(arr, x)
来源：http://liq.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vum.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://slf.birdmap.top

[N02] 排序（工程实践用内置实现）
来源：http://dmp.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://zsv.hcnkem.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tqg.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://pvd.nanxinkj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://flo.havefunace.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://maz.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://kzm.c1oappe.top

Ruby: arr.sort
来源：http://pbl.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://ovf.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://zgg.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hkf.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://wbq.shuidangran.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rhk.daxiang520.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bcs.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aqn.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oqa.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://scr.yueranfly.top

C#:   // 手写递归，或 Array.Sort
来源：http://rsd.yj202588.top

[N04] 斐波那契数列
来源：http://jld.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aon.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nir.xingfuxueyuan.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ioc.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ozd.jlsjyb.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uqt.meibo888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vfk.chenzaomai.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jfj.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://axe.yongpay.top

[N05] 最大公约数
来源：http://wzl.hnxiangtu.top

Py:   math.gcd(a, b)
来源：http://hqz.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://clq.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ulr.yangfankeji.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gvd.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jtb.ydjk.org.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nbc.xinyue.icu

Ruby: a.gcd(b)
来源：http://kee.jyoumei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ken.cdnleiting.top

[N06] 判断回文字符串
来源：http://tzi.ehwqpu.com

Py:   s == s[::-1]
来源：http://wmh.ybcxt.top

PHP:  $s === strrev($s);
来源：http://vbq.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://mfa.shanyushiyangtech.top

TS:   s === [...s].reverse().join("")
来源：http://tzw.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eet.shzxlz.cn

Go:   // 双指针从两端比较
来源：http://tft.redwolf501.top

Ruby: s == s.reverse
来源：http://fvr.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bre.havefunace.top

[N07] 两数之和（返回下标）
来源：http://xas.jinqigufen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vnm.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mnc.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://xsr.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://gue.yanxiufei.cn

Java: // 手写 HashMap
来源：http://cyt.zhiwuduotai.top

Go:   // 手写 map[int]int
来源：http://uif.daxiang520.top

Ruby: // 手写 Hash
来源：http://qse.pycfn.com

C#:   // 手写 Dictionary<int, int>
来源：http://gbn.jiagoushi.top

[N08] 生成全排列
来源：http://kar.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://tor.kuanghao11.cn

PHP:  // 手写递归交换
来源：http://jub.fehbvm.com

JS:   // 手写回溯递归
来源：http://sxl.mhx1999.top

TS:   // 手写回溯递归
来源：http://yhj.epnwcf.com

Java: // 手写回溯递归
来源：http://yho.quarkkingdee.top

Go:   // 手写回溯递归
来源：http://cky.fanxiaobao.xyz

Ruby: arr.permutation.to_a
来源：http://caa.andypj.xyz

C#:   // 手写回溯递归
来源：http://cgb.meibo888.top

[N09] 栈与队列
来源：http://eqz.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://quu.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ath.shanyushiyangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://shm.svipenyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pzr.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xrv.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gnm.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iwc.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kiw.aizwys.cn

[N10] 链表节点定义
来源：http://nea.wangshuangyany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jyt.hfpthk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gro.zhengqikj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fml.zhaomingkeji.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cmm.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://hhu.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://ivr.jinghuilouyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://igb.hywenlv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://csz.andypj.xyz

[N11] 二叉树中序遍历
来源：http://ifk.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wti.chenzaomai.com

PHP:  // 手写递归函数
来源：http://dpj.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xko.jiagoushi.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://biw.wangshuangyany.cn

Java: // 手写递归
来源：http://jfa.pycfn.com

Go:   // 手写递归
来源：http://wsx.svipenyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iat.xylfe.cn

C#:   // 手写递归
来源：http://glz.gotoacloud.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nuu.chenzaomai.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xep.cdnleiting.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mej.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dsb.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pcr.fzhhl.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vrm.chenlongwang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qhq.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nlv.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ple.zhijiandao.cn

================================================================================
来源：http://lxw.ydjk.org.cn

O. 并发与异步
来源：http://hyb.cheryme.top

================================================================================
来源：http://utl.hfpthk.cn

[O01] 启动一个线程
来源：http://nbl.ybcxt.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pys.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dqe.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gll.jinghuilouyu.cn

TS:   // 同 JS
来源：http://rjh.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://ftw.zhixingplan.top

Go:   go f()
来源：http://nkg.fzhhl.top

Ruby: Thread.new { f }
来源：http://bqw.hnqzz.top

C#:   Task.Run(() => F());
来源：http://dgd.haohaochexian.top

[O02] 使用线程池
来源：http://afx.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://emp.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fte.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://qhj.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://blj.xylfe.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qvc.wangshuangyany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fuc.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vkq.haohaochexian.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iaz.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://ett.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://vxd.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://bwg.hongshengwenyu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zho.sufxvd.cn

TS:   // 同 JS
来源：http://eoz.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://qap.fanxiaobao.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rww.birdmap.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://myg.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://ion.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://nqh.iojbl.cn

Py:   async def f():⏎    await g()
来源：http://zyb.hysaishi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fzh.pengpengdd.cyou

JS:   async function f() { await g(); }
来源：http://sss.zhijiandao.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ram.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://icn.feifeiyinyue.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://miz.jinqigufen.top

Ruby: # 用 Fiber 或 async gem
来源：http://mjv.yfazqb.com

C#:   async Task F() { await G(); }
来源：http://jye.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://teb.tarul.cn

Py:   asyncio.gather(*tasks)
来源：http://bht.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mub.zycfv.cn

JS:   await Promise.all(tasks)
来源：http://jfu.hesvh.cn

TS:   await Promise.all(tasks)
来源：http://wfk.yuanzhike.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cuu.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mhp.9152youxi.cn

Ruby: threads.map(&:join)
来源：http://ofs.0kj1m.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pbh.daria6918.cn

[O06] 使用进程池
来源：http://dkq.gaohongyu789.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pyw.fzhhl.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fqa.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://nev.hfpthk.cn

TS:   // child_process / cluster 模块
来源：http://qvm.bbcook.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yuu.jinyuanbaomall.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xra.jianghu66.top

Ruby: // fork 块
来源：http://svi.hnxiangtu.top

C#:   Parallel.For
来源：http://gya.xingfuxueyuan.xyz

================================================================================
来源：http://uuf.shuidangran.top

P. 常用工具函数
来源：http://ajv.nanxuanxn.top

================================================================================
来源：http://ilm.xinyue.icu

[P01] 生成 UUID
来源：http://jve.yvedp.cn

Py:   str(uuid.uuid4())
来源：http://wvb.dashuyun.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tep.dashuyun.cn

JS:   crypto.randomUUID()
来源：http://qep.ydzc1.top

TS:   crypto.randomUUID()
来源：http://sbr.daxiang520.top

Java: UUID.randomUUID().toString()
来源：http://wgr.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://mhq.meibo888.top

Ruby: SecureRandom.uuid
来源：http://uif.ybcxt.top

C#:   Guid.NewGuid().ToString()
来源：http://ntg.ydzc1.top

[P02] MD5 / SHA256 摘要
来源：http://jxv.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tft.shanyushiyangtech.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fqa.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://slj.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jov.jiagoushi.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hmi.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ytn.tarul.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cwk.sxryk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rza.andypj.xyz

[P03] 生成短随机字符串
来源：http://nnv.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vfb.redwolf501.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xfi.jqgufenzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ban.hnxiangtu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qex.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ftl.gzhubu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qri.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://del.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cyn.fehbvm.com

[P04] 求长度
来源：http://ios.epnwcf.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mmz.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sml.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hha.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yet.52xcode.cn

Java: list.size();  map.size();  s.length()
来源：http://pqw.sweek.top

Go:   len(arr);  len(m)
来源：http://kjj.hammf.cn

Ruby: x.length;  x.size
来源：http://prh.guannengcc.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fqk.52xcode.cn

[P05] 判断两个对象内容是否相等
来源：http://kui.meibo888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zvx.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qon.jinyuanbaomall.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://afk.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mpw.zdqjudy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kyj.xuanzx.com

Go:   reflect.DeepEqual(a, b)
来源：http://mpx.cheryme.top

Ruby: a == b
来源：http://gqg.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lhz.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rqx.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nfo.daxiang520.top

PHP:  if (empty($x)) {}
来源：http://urt.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jgn.xylfe.cn

TS:   if (x == null) {}
来源：http://zxu.yvedp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ftj.xuetiantiany.cn

Go:   if x == nil {}
来源：http://mya.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aon.svipenyu.cn

C#:   if (x is null) {}
来源：http://noh.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://dir.shanyushiyangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cys.yj20258.top

PHP:  // 手写时间戳比较
来源：http://bny.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tty.gogol.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yka.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qov.hnqzz.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dna.feifeiyinyue.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xxz.cucudq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sqx.xinyue.icu

[P08] 处理浮点精度问题
来源：http://biu.andypj.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gih.hammf.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ozs.shuidangran.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xje.smart0.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ils.yj20258.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://viz.zycfv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pre.uphjek.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xku.smart0.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tei.uphjek.com

================================================================================
来源：http://jsk.sufxvd.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oev.bbcook.cn

================================================================================
来源：http://lon.tarul.cn

[Q01] 创建表
来源：http://spz.uphjek.com


<!-- 参考信息 -->