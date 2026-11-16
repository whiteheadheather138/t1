代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yky.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bil.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://uye.ydzc1.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lfp.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://llo.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ibk.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vap.haohaochexian.top

C#:   Process.Start("ls", "-l");
来源：http://vps.yongpay.top

[M04] 获取当前工作目录
来源：http://sci.yj202588.top

Py:   os.getcwd()
来源：http://fdw.tanke756.top

PHP:  getcwd();
来源：http://xfm.jinyuanbaomall.cn

JS:   process.cwd()
来源：http://axe.zhiwuduotai.top

TS:   process.cwd()
来源：http://mjb.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://uak.zdbjq.cn

Go:   os.Getwd()
来源：http://icq.fengsongda.top

Ruby: Dir.pwd
来源：http://iih.shzxlz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hfc.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://ruy.yuxming.cn

Py:   sys.exit(1)
来源：http://sjh.ybcxt.top

PHP:  exit(1);
来源：http://dmm.jinqigufen.top

JS:   process.exit(1)
来源：http://zrs.snrcjt.cn

TS:   process.exit(1)
来源：http://gyy.hesvh.cn

Java: System.exit(1)
来源：http://jmx.aibaodan.cn

Go:   os.Exit(1)
来源：http://wxm.ywan-chungtsiang.top

Ruby: exit 1
来源：http://mgv.daria6918.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dkx.yongpay.top

[M06] 向标准错误输出
来源：http://wjq.xuetiantiany.cn

Py:   print("err", file=sys.stderr)
来源：http://qdk.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://htd.fktsv.cn

JS:   console.error("err")
来源：http://afh.jiagoushi.top

TS:   console.error("err")
来源：http://njv.chenjidiqi.icu

Java: System.err.println("err")
来源：http://amf.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tch.hnqzz.top

Ruby: warn "err"
来源：http://bct.ivvv.top

C#:   Console.Error.WriteLine("err")
来源：http://tsy.vehdjk.com

[M07] 判断是否为主入口
来源：http://xpt.haohaochexian.top

Py:   if __name__ == "__main__":
来源：http://huj.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wag.jiagoushi.top

JS:   require.main === module
来源：http://obi.jyoumei.cn

TS:   require.main === module
来源：http://bmf.iojbl.cn

Java: public static void main(String[] args)
来源：http://qac.shanyushiyangkeji.top

Go:   func main()
来源：http://vyt.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://msj.yuanzhike.top

C#:   static void Main(string[] args)
来源：http://nzw.52xcode.cn

[M08] 获取系统与运行时信息
来源：http://diy.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://waw.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://hwd.fanxiaobao.xyz

JS:   process.platform;  process.version
来源：http://hrw.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://axz.jinghuilouyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xbu.hammf.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://otq.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tsu.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gcr.sjlbkw.cn

================================================================================
来源：http://lwk.hesvh.cn

N. 数据结构与算法
来源：http://drb.hnqzz.top

================================================================================
来源：http://xaj.shanyushiyangkeji.top

[N01] 二分查找（有序数组）
来源：http://ssw.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nqg.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rqe.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dhg.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dsk.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://mwx.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://yuq.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lfd.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://tsd.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://xhf.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://zlp.fzhhl.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vpr.jiagoushi.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qhy.vehdjk.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://kmk.cqqwz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://drn.yj20258888.top

Go:   slices.Sort(arr)
来源：http://kfx.sjlbkw.cn

Ruby: arr.sort
来源：http://now.fengsongda.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fns.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://fdr.jinqigfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ggs.fanxiaobao.xyz

PHP:  // 递归实现，或用 usort
来源：http://nol.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ieh.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cls.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://krd.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xme.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kve.hnqzz.top

C#:   // 手写递归，或 Array.Sort
来源：http://pvl.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://dyz.sufxvd.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mxh.hysaishi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fmx.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kbo.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qxg.9152youxi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://djw.yj20258888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://apb.ydzc1.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sbm.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://huo.zhoulong.xyz

[N05] 最大公约数
来源：http://fqb.nanxinkj.top

Py:   math.gcd(a, b)
来源：http://hni.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://psy.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tsa.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wuw.cqqwz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bcr.ydjk.org.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mjl.pycfn.com

Ruby: a.gcd(b)
来源：http://uon.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zyu.aibaodan.cn

[N06] 判断回文字符串
来源：http://ade.zdbjq.cn

Py:   s == s[::-1]
来源：http://meb.ivvv.top

PHP:  $s === strrev($s);
来源：http://mxz.epnwcf.com

JS:   s === [...s].reverse().join("")
来源：http://kxl.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://swk.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ykk.wangshuangyany.cn

Go:   // 双指针从两端比较
来源：http://dyy.hesvh.cn

Ruby: s == s.reverse
来源：http://vuv.9152youxi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qgu.ybcxt.top

[N07] 两数之和（返回下标）
来源：http://qje.fehbvm.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ett.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xwm.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://upv.guowangkeji.top

TS:   // 手写 Map<string, number>
来源：http://buj.cashguo.top

Java: // 手写 HashMap
来源：http://gaw.hesvh.cn

Go:   // 手写 map[int]int
来源：http://obw.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://paf.gotoacloud.top

C#:   // 手写 Dictionary<int, int>
来源：http://qxn.cdnleiting.top

[N08] 生成全排列
来源：http://mlq.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://gwm.cqqwz.cn

PHP:  // 手写递归交换
来源：http://ycx.ctjpmb.com

JS:   // 手写回溯递归
来源：http://sjx.gotoacloud.top

TS:   // 手写回溯递归
来源：http://wys.yangfankeji.com

Java: // 手写回溯递归
来源：http://sdt.hesvh.cn

Go:   // 手写回溯递归
来源：http://fox.gzhubu.top

Ruby: arr.permutation.to_a
来源：http://ubq.pengpengdd.cyou

C#:   // 手写回溯递归
来源：http://btq.hongshengwenyu.top

[N09] 栈与队列
来源：http://qlb.hongshengwenyu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bsu.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tqq.jinghuilouyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mtu.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vdk.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rqg.cdnleiting.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://csn.jinqigfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ukw.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ekn.sysykeji.top

[N10] 链表节点定义
来源：http://cnm.meibo888.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kau.zycfv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vuf.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yhr.andypj.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ajj.jinqigufen.top

Java: class Node { int v; Node next; }
来源：http://jor.ctjpmb.com

Go:   type Node struct { V int; Next *Node }
来源：http://ewe.sweek.top

Ruby: Node = Struct.new(:v, :next)
来源：http://icf.smart0.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://zau.sysykeji.top

[N11] 二叉树中序遍历
来源：http://wru.cucudq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uex.shuidangran.top

PHP:  // 手写递归函数
来源：http://rxu.jianghu66.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cng.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zhp.yuanzhike.top

Java: // 手写递归
来源：http://gdi.jinqigfzy.top

Go:   // 手写递归
来源：http://jum.guowangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://afo.xinyue.icu

C#:   // 手写递归
来源：http://bwi.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bno.yonumen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bxa.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ddr.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lkp.hfpthk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lgu.chenlongwang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ahl.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gdn.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mxc.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mep.wangshuangyany.cn

================================================================================
来源：http://nfk.shanyushiyangkeji.top

O. 并发与异步
来源：http://gyx.bbcook.cn

================================================================================
来源：http://xju.gzhubu.top

[O01] 启动一个线程
来源：http://igm.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fkk.aizwys.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wmn.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ddy.52xcode.cn

TS:   // 同 JS
来源：http://ojx.ctjpmb.com

Java: new Thread(() -> f()).start()
来源：http://vef.aizwys.cn

Go:   go f()
来源：http://hpb.hfpthk.cn

Ruby: Thread.new { f }
来源：http://isy.epnwcf.com

C#:   Task.Run(() => F());
来源：http://xmm.bjfxy.top

[O02] 使用线程池
来源：http://sbq.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://grr.jinqigfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qtk.shuidangran.top

JS:   // worker_threads 线程池
来源：http://xza.smart0.xyz

TS:   // worker_threads 线程池
来源：http://crs.xuetiantiany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hwx.yj202588.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wir.daria6918.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fho.pengpengdd.cyou

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://scv.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://eek.chenlongwang.top

Py:   with lock: shared += 1
来源：http://kkj.feifeiyinyue.top

PHP:  // 用 flock() 做文件锁
来源：http://ifd.sjlbkw.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://knm.xuetiantiany.cn

TS:   // 同 JS
来源：http://shd.jianghu66.top

Java: synchronized (this) { shared++; }
来源：http://vrg.zdqjudy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aep.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://thv.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://nvy.cucudq.cn

[O04] 定义异步函数并等待
来源：http://ssj.jqgfzy.top

Py:   async def f():⏎    await g()
来源：http://end.jyoumei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kwg.0kj1m.cn

JS:   async function f() { await g(); }
来源：http://saj.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://aos.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sek.feifeiyinyue.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dcp.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qzg.redwolf501.top

C#:   async Task F() { await G(); }
来源：http://wwu.xuanzx.com

[O05] 并发执行并等待全部完成
来源：http://uzc.zhijiandao.cn

Py:   asyncio.gather(*tasks)
来源：http://eoc.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://diu.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://wwq.cheryme.top

TS:   await Promise.all(tasks)
来源：http://dmy.chenlongwang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mcb.havefunace.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://woc.shangyingyoupin.top

Ruby: threads.map(&:join)
来源：http://zbo.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qqf.yfazqb.com

[O06] 使用进程池
来源：http://mof.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aeg.zdqjudy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fev.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://uhk.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://hrg.hesvh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ews.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vhb.havefunace.top

Ruby: // fork 块
来源：http://nnp.zdbjq.cn

C#:   Parallel.For
来源：http://aby.hywenlv.cn

================================================================================
来源：http://jqc.gaohongyu789.top

P. 常用工具函数
来源：http://zva.zhoulong.xyz

================================================================================
来源：http://ovj.vehdjk.com

[P01] 生成 UUID
来源：http://vxs.birdmap.top

Py:   str(uuid.uuid4())
来源：http://tfz.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hdj.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://cgl.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://rwl.gzhubu.top

Java: UUID.randomUUID().toString()
来源：http://glk.yj20258888.top

Go:   // 用 github.com/google/uuid
来源：http://ikc.jyoumei.cn

Ruby: SecureRandom.uuid
来源：http://mbu.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://qck.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://dsg.dianchejie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ppq.shuidangran.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cpa.0kj1m.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gda.yvedp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cjw.cdnleiting.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rgj.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://esr.xuetiantiany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zjh.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mhh.andypj.xyz

[P03] 生成短随机字符串
来源：http://dtz.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sie.smart0.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ugw.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dvh.wangdashe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cyw.snrcjt.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tje.jlsjyb.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ebr.fanxiaobao.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://hez.kuanghao11.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gmh.xziqi.cn

[P04] 求长度
来源：http://dwm.gzhubu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zez.gzhubu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uvh.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sha.zdqjudy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dqc.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://nmu.shanyushiyangkeji.top

Go:   len(arr);  len(m)
来源：http://xcw.dashuyun.cn

Ruby: x.length;  x.size
来源：http://nlp.uphjek.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://hmt.uphjek.com

[P05] 判断两个对象内容是否相等
来源：http://meu.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://fah.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pjm.hongshengwenyu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fqd.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vqo.fanxiaobao.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mmm.daria6918.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gub.nanxuanxn.top

Ruby: a == b
来源：http://puh.chenlongwang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xva.xingfuxueyuan.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://knx.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dpx.wangdashe.top

PHP:  if (empty($x)) {}
来源：http://kys.sxryk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xcc.xziqi.cn

TS:   if (x == null) {}
来源：http://ehb.hnqzz.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wbs.epnwcf.com

Go:   if x == nil {}
来源：http://iqb.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qsb.fanxiaobao.xyz

C#:   if (x is null) {}
来源：http://mgb.shuidangran.top

[P07] 防抖与节流
来源：http://pfo.hcnkem.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ztn.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://ffs.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ibn.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jjc.jqgufenzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nwg.zycfv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xwl.yj202588.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://abz.yanxiufei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ira.zhijiandao.cn

[P08] 处理浮点精度问题
来源：http://mqt.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://stt.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sqd.aizwys.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iqx.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rzi.uphjek.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hjn.sjlbkw.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yiu.cucudq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yiw.wangdashe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nah.yfazqb.com

================================================================================
来源：http://bed.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ndz.epnwcf.com

================================================================================
来源：http://rnq.guannengcc.top

[Q01] 创建表
来源：http://rxc.shanyushiyangtech.top


<!-- 参考信息 -->