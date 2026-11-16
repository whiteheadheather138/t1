代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pqo.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ggj.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zdy.ivvv.top

C#:   Process.Start("ls", "-l");
来源：http://cch.cqqwz.cn

[M04] 获取当前工作目录
来源：http://yzt.jlsjyb.cn

Py:   os.getcwd()
来源：http://kah.hammf.cn

PHP:  getcwd();
来源：http://jzp.tanke756.top

JS:   process.cwd()
来源：http://nls.bbcook.cn

TS:   process.cwd()
来源：http://dni.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://zcm.smart0.xyz

Go:   os.Getwd()
来源：http://vaa.yueranfly.top

Ruby: Dir.pwd
来源：http://gwc.ehwqpu.com

C#:   Directory.GetCurrentDirectory()
来源：http://zwj.meibo888.top

[M05] 设置退出码
来源：http://jbh.gzhubu.top

Py:   sys.exit(1)
来源：http://rdq.snrcjt.cn

PHP:  exit(1);
来源：http://pwb.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://wxv.gzhubu.top

TS:   process.exit(1)
来源：http://gnf.aibaodan.cn

Java: System.exit(1)
来源：http://pzx.uphjek.com

Go:   os.Exit(1)
来源：http://cak.fengsongda.top

Ruby: exit 1
来源：http://wds.birdmap.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bef.shanyushiyangkeji.top

[M06] 向标准错误输出
来源：http://dsc.fehbvm.com

Py:   print("err", file=sys.stderr)
来源：http://ejz.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xbm.jqgfzy.top

JS:   console.error("err")
来源：http://ech.ydzc1.top

TS:   console.error("err")
来源：http://gro.sysykeji.top

Java: System.err.println("err")
来源：http://fen.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cbt.pycfn.com

Ruby: warn "err"
来源：http://opx.316326.xyz

C#:   Console.Error.WriteLine("err")
来源：http://ghs.xziqi.cn

[M07] 判断是否为主入口
来源：http://cof.ppjwa.cn

Py:   if __name__ == "__main__":
来源：http://bvz.zhiwuduotai.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://twr.xuanzx.com

JS:   require.main === module
来源：http://grv.haohaochexian.top

TS:   require.main === module
来源：http://kts.zycfv.cn

Java: public static void main(String[] args)
来源：http://lzt.0kj1m.cn

Go:   func main()
来源：http://tmj.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mkr.smart0.xyz

C#:   static void Main(string[] args)
来源：http://jjx.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://afr.nwbrower.top

Py:   platform.system();  platform.python_version()
来源：http://ndx.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://elv.316326.xyz

JS:   process.platform;  process.version
来源：http://wkq.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://ipg.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://igo.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zjm.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wtd.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://zer.ydjk.org.cn

================================================================================
来源：http://yjk.tanke756.top

N. 数据结构与算法
来源：http://njd.zhijiandao.cn

================================================================================
来源：http://kwt.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://sof.sxryk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ikq.fktsv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://axe.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nmv.ivvv.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zuz.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://fgw.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://nzo.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qkx.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://pkx.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://rdm.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://icz.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jvi.chenzaomai.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://evx.gogol.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://abd.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://exa.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://qpv.pengpengdd.cyou

Ruby: arr.sort
来源：http://uva.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kaa.ivvv.top

[N03] 快速排序（分治示例）
来源：http://dtz.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rqp.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://occ.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hmm.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ota.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://twu.kuanghao11.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pno.cucudq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xdg.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://fbp.yanxiufei.cn

[N04] 斐波那契数列
来源：http://fne.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://usz.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qbt.yfazqb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://duk.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qpy.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://anl.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://veo.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mny.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://faz.yueranfly.top

[N05] 最大公约数
来源：http://ovu.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://ecn.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rgt.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nzl.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ykx.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://awj.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://omc.zycfv.cn

Ruby: a.gcd(b)
来源：http://nnu.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dmh.bbcook.cn

[N06] 判断回文字符串
来源：http://fig.snrcjt.cn

Py:   s == s[::-1]
来源：http://vzu.guannengcc.top

PHP:  $s === strrev($s);
来源：http://jmw.redwolf501.top

JS:   s === [...s].reverse().join("")
来源：http://fqv.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://zjj.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://naz.zhongyouzk.top

Go:   // 双指针从两端比较
来源：http://cqv.andypj.xyz

Ruby: s == s.reverse
来源：http://khq.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yzg.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://cke.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://csd.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xvj.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://jhr.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://xqn.gotoacloud.top

Java: // 手写 HashMap
来源：http://tgu.ydzc1.top

Go:   // 手写 map[int]int
来源：http://nut.hammf.cn

Ruby: // 手写 Hash
来源：http://xls.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://omo.jlsjyb.cn

[N08] 生成全排列
来源：http://skh.xingfuxueyuan.xyz

Py:   itertools.permutations(arr)
来源：http://lhc.hfpthk.cn

PHP:  // 手写递归交换
来源：http://vkg.nwbrower.top

JS:   // 手写回溯递归
来源：http://ord.wangdashe.top

TS:   // 手写回溯递归
来源：http://wbz.zycfv.cn

Java: // 手写回溯递归
来源：http://vrd.yuxming.cn

Go:   // 手写回溯递归
来源：http://fxq.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://mud.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://cyf.c1oappe.top

[N09] 栈与队列
来源：http://emk.jianghu66.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://trl.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pbx.jinqigfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fwk.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qyn.xingfuxueyuan.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iwz.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bti.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oce.vqdsnc.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://egi.hnqzz.top

[N10] 链表节点定义
来源：http://grx.xuanzx.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rke.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://upo.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hyc.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mbl.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://rlv.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mki.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wtu.sxryk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cty.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://xgx.yonumen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dlz.guannengcc.top

PHP:  // 手写递归函数
来源：http://bhu.sysykeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lcy.zhoulong.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fmp.yuanzhike.top

Java: // 手写递归
来源：http://jzx.yfazqb.com

Go:   // 手写递归
来源：http://pdb.yueranfly.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oue.feifeiyinyue.top

C#:   // 手写递归
来源：http://hzr.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pcy.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://suc.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xil.hfpthk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nbj.dashuyun.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wyg.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jde.nwbrower.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bzh.smart0.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fxj.tian-w.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vbk.jinqigufen.top

================================================================================
来源：http://bmt.yvedp.cn

O. 并发与异步
来源：http://ckh.iojbl.cn

================================================================================
来源：http://rrt.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://pho.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pnx.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://emq.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rya.zhixingplan.top

TS:   // 同 JS
来源：http://edo.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://idw.xylfe.cn

Go:   go f()
来源：http://vox.jlsjyb.cn

Ruby: Thread.new { f }
来源：http://rjy.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://tly.sxryk.cn

[O02] 使用线程池
来源：http://isk.svipenyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wiw.uphjek.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://coe.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://bpd.bjfxy.top

TS:   // worker_threads 线程池
来源：http://xuw.sysykeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://nei.jinghuilouyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zst.shanyushiyangtech.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kjs.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://csr.yongpay.top

[O03] 加锁保护共享数据
来源：http://uhj.mhx1999.top

Py:   with lock: shared += 1
来源：http://kwg.yueranfly.top

PHP:  // 用 flock() 做文件锁
来源：http://itq.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://seh.kuanghao11.cn

TS:   // 同 JS
来源：http://nxc.fengsongda.top

Java: synchronized (this) { shared++; }
来源：http://obf.jinqigfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tah.snrcjt.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kvx.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://tom.cucudq.cn

[O04] 定义异步函数并等待
来源：http://oem.yj20258888.top

Py:   async def f():⏎    await g()
来源：http://omo.xylfe.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lrx.kuanghao11.cn

JS:   async function f() { await g(); }
来源：http://acv.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://luh.daria6918.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mxl.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ybv.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://bdu.dianchejie.cn

C#:   async Task F() { await G(); }
来源：http://opd.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://fcu.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://smx.fengsongda.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://swv.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://lff.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://idn.gaohongyu789.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://idr.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jos.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://shf.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://ybo.epnwcf.com

[O06] 使用进程池
来源：http://dxf.daria6918.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tfb.jinqigufen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uyw.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://pny.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://cen.jianghu66.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qwd.gotoacloud.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gqo.9152youxi.cn

Ruby: // fork 块
来源：http://xzm.fzhhl.top

C#:   Parallel.For
来源：http://bqm.xylfe.cn

================================================================================
来源：http://lpy.jyoumei.cn

P. 常用工具函数
来源：http://cxa.jinqigufen.top

================================================================================
来源：http://urj.meibo888.top

[P01] 生成 UUID
来源：http://bxu.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://plu.havefunace.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bnl.fzhhl.top

JS:   crypto.randomUUID()
来源：http://gev.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://wka.uphjek.com

Java: UUID.randomUUID().toString()
来源：http://yjk.dianchejie.cn

Go:   // 用 github.com/google/uuid
来源：http://pae.ywan-chungtsiang.top

Ruby: SecureRandom.uuid
来源：http://szb.guannengcc.top

C#:   Guid.NewGuid().ToString()
来源：http://kjg.xuanzx.com

[P02] MD5 / SHA256 摘要
来源：http://glb.ydjk.org.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ygb.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tlf.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://onn.aizwys.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jwm.yuanzhike.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ybi.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hov.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yjr.shangyingyoupin.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lml.svipenyu.cn

[P03] 生成短随机字符串
来源：http://rab.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ccu.hesvh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pkn.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tvs.chenzaomai.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dbc.yfazqb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wgq.hywenlv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kxi.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yis.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://imr.hysaishi.cn

[P04] 求长度
来源：http://raq.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://csu.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mvm.tianlin.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xns.yj202588.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kvs.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://nci.zhixingplan.top

Go:   len(arr);  len(m)
来源：http://ifu.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://awo.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://jud.hnxiangtu.top

[P05] 判断两个对象内容是否相等
来源：http://pqe.316326.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://ljs.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tyd.jiagoushi.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hgm.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rfa.shangyingyoupin.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nky.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://tsc.pengpengdd.cyou

Ruby: a == b
来源：http://ohf.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uvz.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uyr.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oya.xuetiantiany.cn

PHP:  if (empty($x)) {}
来源：http://pjb.gzhubu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://azb.hnqzz.top

TS:   if (x == null) {}
来源：http://ycx.xinyue.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://vcx.fanxiaobao.xyz

Go:   if x == nil {}
来源：http://rcl.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ruc.jinyuanbaomall.cn

C#:   if (x is null) {}
来源：http://xck.jinqigfzy.top

[P07] 防抖与节流
来源：http://ffg.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://exv.zdbjq.cn

PHP:  // 手写时间戳比较
来源：http://jlo.tian-w.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://egg.cheryme.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://etr.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sne.zhaomingkeji.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://igh.shangyingyoupin.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yjd.52xcode.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vhr.dianchejie.cn

[P08] 处理浮点精度问题
来源：http://pku.yuanzhike.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uck.zhiwuduotai.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hzv.gzhubu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ydh.cheryme.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hcu.ppjwa.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nhx.yj202588.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kue.0kj1m.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bye.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zzq.xylfe.cn

================================================================================
来源：http://cdt.shuidangran.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yik.svipenyu.cn

================================================================================
来源：http://azc.shangyingyoupin.top

[Q01] 创建表
来源：http://yql.gzhubu.top

CREATE TABLE users (
来源：http://ktr.ctjpmb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bog.xinyue.icu

name VARCHAR(50) NOT NULL,
来源：http://fnq.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://jbe.jinyuanbaomall.cn


<!-- 参考信息 -->