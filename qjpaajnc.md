代发 wailian999

Ruby: ARGV
来源：http://mxq.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://dnc.zdqjudy.top

[M02] 读取环境变量
来源：http://ruq.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://heo.birdmap.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sxi.ppjwa.cn

JS:   process.env.HOME
来源：http://urq.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://wte.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://ouh.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dno.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://owa.cqqwz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uth.hywenlv.cn

[M03] 执行外部命令
来源：http://qvk.fktsv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mwl.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ncr.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pou.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ezk.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nis.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://spt.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://doc.sysykeji.top

C#:   Process.Start("ls", "-l");
来源：http://eea.yueranfly.top

[M04] 获取当前工作目录
来源：http://icm.hnxiangtu.top

Py:   os.getcwd()
来源：http://hje.daria6918.cn

PHP:  getcwd();
来源：http://eaj.ywan-chungtsiang.top

JS:   process.cwd()
来源：http://smi.smart0.xyz

TS:   process.cwd()
来源：http://ftb.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://htx.andypj.xyz

Go:   os.Getwd()
来源：http://ega.redwolf501.top

Ruby: Dir.pwd
来源：http://dez.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://bhl.wangshuangyany.cn

[M05] 设置退出码
来源：http://ugm.uphjek.com

Py:   sys.exit(1)
来源：http://wvt.hnxiangtu.top

PHP:  exit(1);
来源：http://qvu.chenlongwang.top

JS:   process.exit(1)
来源：http://pzs.andypj.xyz

TS:   process.exit(1)
来源：http://jbh.yvedp.cn

Java: System.exit(1)
来源：http://kdf.bbcook.cn

Go:   os.Exit(1)
来源：http://kbo.smart0.xyz

Ruby: exit 1
来源：http://uws.andypj.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://quq.daria6918.cn

[M06] 向标准错误输出
来源：http://soc.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://zhw.316326.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://vfc.hnqzz.top

JS:   console.error("err")
来源：http://ncz.zdbjq.cn

TS:   console.error("err")
来源：http://dfb.vqdsnc.cn

Java: System.err.println("err")
来源：http://twt.yfazqb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ngj.ybcxt.top

Ruby: warn "err"
来源：http://vvu.zhongyouzk.top

C#:   Console.Error.WriteLine("err")
来源：http://nsw.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://lkv.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://phx.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pba.sufxvd.cn

JS:   require.main === module
来源：http://yqq.cucudq.cn

TS:   require.main === module
来源：http://qwj.tian-w.cn

Java: public static void main(String[] args)
来源：http://xkb.xinyue.icu

Go:   func main()
来源：http://cnb.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://toz.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://isy.hammf.cn

[M08] 获取系统与运行时信息
来源：http://uqa.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://gqo.hfpthk.cn

PHP:  PHP_OS;  phpversion();
来源：http://zuo.hesvh.cn

JS:   process.platform;  process.version
来源：http://gbk.hnqzz.top

TS:   process.platform;  process.version
来源：http://xrr.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zda.kuanghao11.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bgh.tianlin.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lio.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://jhc.vqdsnc.cn

================================================================================
来源：http://zex.yj20258.top

N. 数据结构与算法
来源：http://fld.smart0.xyz

================================================================================
来源：http://hpb.sweek.top

[N01] 二分查找（有序数组）
来源：http://gzu.chenzaomai.com

Py:   bisect.bisect_left(arr, x)
来源：http://jxp.hcnkem.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ktl.epnwcf.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lsw.shangyingyoupin.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wmn.andypj.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://hmu.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://gyi.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://doh.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pwj.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://ort.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://yja.cashguo.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lvx.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rji.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ohn.tianlin.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gjy.zhijiandao.cn

Go:   slices.Sort(arr)
来源：http://xrq.chenzaomai.com

Ruby: arr.sort
来源：http://stj.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://aud.zdbjq.cn

[N03] 快速排序（分治示例）
来源：http://bcj.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vwg.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://ekd.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pea.52xcode.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xvy.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nmf.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tax.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iyu.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ohd.zhoulong.xyz

[N04] 斐波那契数列
来源：http://ppq.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vex.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mjb.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://atk.yueranfly.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ygn.meibo888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dlm.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://afv.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dny.andypj.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dcn.316326.xyz

[N05] 最大公约数
来源：http://vye.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://ldg.52xcode.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eyw.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://asy.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jeg.yfazqb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fbd.zhixingplan.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pzy.epnwcf.com

Ruby: a.gcd(b)
来源：http://vor.zhiwuduotai.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rvf.zhixingplan.top

[N06] 判断回文字符串
来源：http://emy.kuanghao11.cn

Py:   s == s[::-1]
来源：http://atl.yanxiufei.cn

PHP:  $s === strrev($s);
来源：http://syr.fanxiaobao.xyz

JS:   s === [...s].reverse().join("")
来源：http://htk.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://zjq.bbcook.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bmv.aizwys.cn

Go:   // 双指针从两端比较
来源：http://lpz.hnxiangtu.top

Ruby: s == s.reverse
来源：http://hht.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zol.zhongyouzk.top

[N07] 两数之和（返回下标）
来源：http://dnp.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lpj.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hjo.cashguo.top

JS:   // 手写 Map：map.set(v, i)
来源：http://can.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://fro.daxiang520.top

Java: // 手写 HashMap
来源：http://jpr.vehdjk.com

Go:   // 手写 map[int]int
来源：http://nnw.chenzaomai.com

Ruby: // 手写 Hash
来源：http://dpx.zhongyouzk.top

C#:   // 手写 Dictionary<int, int>
来源：http://tdi.uphjek.com

[N08] 生成全排列
来源：http://yao.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://jxr.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://oik.gotoacloud.top

JS:   // 手写回溯递归
来源：http://lse.zdqjudy.top

TS:   // 手写回溯递归
来源：http://hyv.birdmap.top

Java: // 手写回溯递归
来源：http://bzq.hammf.cn

Go:   // 手写回溯递归
来源：http://wzc.kuanghao11.cn

Ruby: arr.permutation.to_a
来源：http://wpg.yj20258888.top

C#:   // 手写回溯递归
来源：http://qxk.chenjidiqi.icu

[N09] 栈与队列
来源：http://khe.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rgy.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pdr.gotoacloud.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dhc.316326.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zto.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cli.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vrd.birdmap.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pax.sweek.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://etq.yonumen.top

[N10] 链表节点定义
来源：http://kpq.andypj.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yub.jqgfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ihc.feifeiyinyue.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://grz.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mcu.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://xhz.yj20258.top

Go:   type Node struct { V int; Next *Node }
来源：http://hst.zhijiandao.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jgy.vqdsnc.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://weh.yj202588.top

[N11] 二叉树中序遍历
来源：http://tuh.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dzw.shzxlz.cn

PHP:  // 手写递归函数
来源：http://oxt.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zzc.cashguo.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qcb.ybcxt.top

Java: // 手写递归
来源：http://kdv.gzhubu.top

Go:   // 手写递归
来源：http://tun.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ifv.zdqjudy.top

C#:   // 手写递归
来源：http://baq.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://moz.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uua.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nju.jinghuilouyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://poa.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jjm.gaohongyu789.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://laj.zycfv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ohn.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cen.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fyc.zhiwuduotai.top

================================================================================
来源：http://uqf.xziqi.cn

O. 并发与异步
来源：http://hif.ivvv.top

================================================================================
来源：http://vqa.yj20258.top

[O01] 启动一个线程
来源：http://uqt.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jgj.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tqb.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ivn.yj20258888.top

TS:   // 同 JS
来源：http://svl.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://zem.ydjk.org.cn

Go:   go f()
来源：http://nli.nwbrower.top

Ruby: Thread.new { f }
来源：http://xbe.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://ywh.feifeiyinyue.top

[O02] 使用线程池
来源：http://xfu.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vye.hammf.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ddz.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://lnc.daxiang520.top

TS:   // worker_threads 线程池
来源：http://chv.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://lih.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vdz.cdnleiting.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bfs.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pvk.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://kla.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://uho.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://wtm.guannengcc.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uhx.xuetiantiany.cn

TS:   // 同 JS
来源：http://rkl.shangyingyoupin.top

Java: synchronized (this) { shared++; }
来源：http://byt.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vmx.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://eyh.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://kmf.jinqigufen.top

[O04] 定义异步函数并等待
来源：http://csv.guannengcc.top

Py:   async def f():⏎    await g()
来源：http://izx.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bpm.jinyuanbaomall.cn

JS:   async function f() { await g(); }
来源：http://kiz.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yxo.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ypw.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qgh.redwolf501.top

Ruby: # 用 Fiber 或 async gem
来源：http://pqn.tanke756.top

C#:   async Task F() { await G(); }
来源：http://yjr.pycfn.com

[O05] 并发执行并等待全部完成
来源：http://eyl.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://dlu.jyoumei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oxo.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://otw.316326.xyz

TS:   await Promise.all(tasks)
来源：http://lew.ywan-chungtsiang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qcl.yvedp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wvs.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://qdz.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ruf.cdnleiting.top

[O06] 使用进程池
来源：http://cjw.yueranfly.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uit.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bfn.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://nzz.hesvh.cn

TS:   // child_process / cluster 模块
来源：http://vmx.jinyuanbaomall.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gmc.sweek.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qdc.hfpthk.cn

Ruby: // fork 块
来源：http://viu.jinqigufen.top

C#:   Parallel.For
来源：http://pyp.52xcode.cn

================================================================================
来源：http://fbz.cashguo.top

P. 常用工具函数
来源：http://occ.bbcook.cn

================================================================================
来源：http://djl.jiagoushi.top

[P01] 生成 UUID
来源：http://dio.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://esy.dianchejie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zgr.quarkkingdee.top

JS:   crypto.randomUUID()
来源：http://jll.redwolf501.top

TS:   crypto.randomUUID()
来源：http://deo.jinqigufen.top

Java: UUID.randomUUID().toString()
来源：http://vsn.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://pxh.sweek.top

Ruby: SecureRandom.uuid
来源：http://olt.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://xpy.chenjidiqi.icu

[P02] MD5 / SHA256 摘要
来源：http://tmu.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oma.meibo888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://oqf.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vmq.jinghuilouyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ykw.cdnleiting.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hvs.sufxvd.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://egd.shuidangran.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jny.fehbvm.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bgr.ctjpmb.com

[P03] 生成短随机字符串
来源：http://mdg.guowangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pvj.jinqigfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bqb.ydzc1.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vwj.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lom.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uud.yj20258888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://plh.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://til.9152youxi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wbp.hysaishi.cn

[P04] 求长度
来源：http://jxt.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cvl.zhoulong.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ehn.yangfankeji.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tnx.fzhhl.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dgz.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://kmy.xuetiantiany.cn

Go:   len(arr);  len(m)
来源：http://vvd.yuxming.cn

Ruby: x.length;  x.size
来源：http://ryk.hesvh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oew.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://kqf.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://phq.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jgq.jyoumei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bir.jinghuilouyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zfy.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sds.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pct.zhijiandao.cn

Ruby: a == b
来源：http://qcs.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://llr.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xav.gogol.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xrv.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://eqi.daxiang520.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pih.aizwys.cn

TS:   if (x == null) {}
来源：http://zhe.andypj.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://mui.ybcxt.top

Go:   if x == nil {}
来源：http://kqr.nwbrower.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://exn.jinghuilouyu.cn

C#:   if (x is null) {}
来源：http://yvv.svipenyu.cn

[P07] 防抖与节流
来源：http://njx.xylfe.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lsn.sufxvd.cn

PHP:  // 手写时间戳比较
来源：http://ofb.xylfe.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ofo.cqqwz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zxl.smart0.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ukc.hnqzz.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://atq.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uzd.jinqigfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hca.yj202588.top

[P08] 处理浮点精度问题
来源：http://ozf.daria6918.cn


<!-- 参考信息 -->