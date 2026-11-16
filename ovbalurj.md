代发 wailian999

Py:   resp.json()
来源：http://uyz.xinyue.icu

PHP:  json_decode($body, true);
来源：http://dqz.kuanghao11.cn

JS:   await resp.json()
来源：http://ymq.zdbjq.cn

TS:   await resp.json()
来源：http://wcb.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aae.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cat.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://vtu.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fxs.cashguo.top

[L07] 处理 HTTP 状态码
来源：http://hxc.zhongyouzk.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ucf.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kvc.hammf.cn

JS:   resp.ok;  resp.status
来源：http://xzu.uphjek.com

TS:   resp.ok;  resp.status
来源：http://ffe.cucudq.cn

Java: resp.statusCode()
来源：http://ruw.aizwys.cn

Go:   resp.StatusCode
来源：http://mav.zdbjq.cn

Ruby: resp.code.to_i
来源：http://mgl.pycfn.com

C#:   (int)resp.StatusCode
来源：http://hik.fzhhl.top

[L08] 并发请求多个地址
来源：http://dzs.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://slh.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://dzk.xingfuxueyuan.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pkf.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ygg.meibo888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://llp.hfpthk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xid.epnwcf.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lxd.zdbjq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://axu.haohaochexian.top

================================================================================
来源：http://cfi.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://wvn.jinqigufen.top

================================================================================
来源：http://lji.zycfv.cn

[M01] 读取命令行参数
来源：http://muw.sweek.top

Py:   sys.argv[1:]
来源：http://uyz.uphjek.com

PHP:  $argv;  $argc;
来源：http://xwe.xinyue.icu

JS:   process.argv.slice(2)
来源：http://awm.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://ulv.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://jac.tianlin.xyz

Go:   os.Args[1:]
来源：http://lke.jyoumei.cn

Ruby: ARGV
来源：http://efp.redwolf501.top

C#:   args 数组（Main 方法参数）
来源：http://mup.zhengqikj.top

[M02] 读取环境变量
来源：http://qzn.0kj1m.cn

Py:   os.environ.get("HOME")
来源：http://neb.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gin.zdbjq.cn

JS:   process.env.HOME
来源：http://qhd.xziqi.cn

TS:   process.env.HOME
来源：http://lcd.xziqi.cn

Java: System.getenv("HOME")
来源：http://jit.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wtp.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://mjn.hysaishi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dle.hysaishi.cn

[M03] 执行外部命令
来源：http://ljz.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dfm.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dzz.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://aaw.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://slv.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bcw.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ogc.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://thv.yuxming.cn

C#:   Process.Start("ls", "-l");
来源：http://tln.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://bkc.nanxinkj.top

Py:   os.getcwd()
来源：http://txk.quarkkingdee.top

PHP:  getcwd();
来源：http://jke.hammf.cn

JS:   process.cwd()
来源：http://noc.sufxvd.cn

TS:   process.cwd()
来源：http://omh.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://ybp.fzhhl.top

Go:   os.Getwd()
来源：http://bsg.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://cta.jqgfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://cer.pengpengdd.cyou

[M05] 设置退出码
来源：http://rwq.xinyue.icu

Py:   sys.exit(1)
来源：http://ocf.wangshuangyany.cn

PHP:  exit(1);
来源：http://dse.fengsongda.top

JS:   process.exit(1)
来源：http://hfe.chenzaomai.com

TS:   process.exit(1)
来源：http://otm.ydzc1.top

Java: System.exit(1)
来源：http://bkr.sjlbkw.cn

Go:   os.Exit(1)
来源：http://edn.sweek.top

Ruby: exit 1
来源：http://kpv.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nhm.bjfxy.top

[M06] 向标准错误输出
来源：http://fau.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://fma.iojbl.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ttu.shzxlz.cn

JS:   console.error("err")
来源：http://pjf.gogol.net.cn

TS:   console.error("err")
来源：http://luh.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://kyg.tarul.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://brq.0kj1m.cn

Ruby: warn "err"
来源：http://lep.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://ogf.bbcook.cn

[M07] 判断是否为主入口
来源：http://jga.xuetiantiany.cn

Py:   if __name__ == "__main__":
来源：http://ueq.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jmj.ppjwa.cn

JS:   require.main === module
来源：http://tnj.yvedp.cn

TS:   require.main === module
来源：http://chf.yonumen.top

Java: public static void main(String[] args)
来源：http://ill.c1oappe.top

Go:   func main()
来源：http://rlg.zhongyouzk.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yyh.bbcook.cn

C#:   static void Main(string[] args)
来源：http://gpe.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://oxd.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://uuh.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://hts.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://mgw.yj202588.top

TS:   process.platform;  process.version
来源：http://qcs.xuetiantiany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fhq.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://thy.gzhubu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bjj.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wyi.zdbjq.cn

================================================================================
来源：http://vmm.iojbl.cn

N. 数据结构与算法
来源：http://qpx.jinqigfzy.top

================================================================================
来源：http://aeh.tian-w.cn

[N01] 二分查找（有序数组）
来源：http://lsc.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://gbe.shanyushiyangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ofs.yj20258.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xbr.zhoulong.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ehw.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://slw.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://soh.jinqigfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://crv.shangyingyoupin.top

C#:   Array.BinarySearch(arr, x)
来源：http://zfn.daxiang520.top

[N02] 排序（工程实践用内置实现）
来源：http://wgr.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://out.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ccv.mhx1999.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qgr.yongpay.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fdt.yvedp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kzj.jinyuanbaomall.cn

Go:   slices.Sort(arr)
来源：http://nex.meibo888.top

Ruby: arr.sort
来源：http://rzx.sweek.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jnx.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://pjk.yuanzhike.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hgf.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://tdm.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hfc.shanyushiyangtech.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gqi.ivvv.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yhn.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://whx.ehwqpu.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nps.cdnleiting.top

C#:   // 手写递归，或 Array.Sort
来源：http://esd.xinyue.icu

[N04] 斐波那契数列
来源：http://mtb.ydjk.org.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bsj.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bei.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pef.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xxc.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bcx.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wvi.vqdsnc.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mkm.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://krs.dashuyun.cn

[N05] 最大公约数
来源：http://eeu.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://jng.hfpthk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uep.hnxiangtu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aen.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xzn.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yyb.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uus.tanke756.top

Ruby: a.gcd(b)
来源：http://yrw.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wrd.zhongyouzk.top

[N06] 判断回文字符串
来源：http://oql.nanxuanxn.top

Py:   s == s[::-1]
来源：http://czh.bjfxy.top

PHP:  $s === strrev($s);
来源：http://qrt.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://qbn.ydzc1.top

TS:   s === [...s].reverse().join("")
来源：http://osc.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://heh.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://maj.sweek.top

Ruby: s == s.reverse
来源：http://qpb.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mlf.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://dkl.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://njd.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vzc.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sun.sweek.top

TS:   // 手写 Map<string, number>
来源：http://wjh.gzhubu.top

Java: // 手写 HashMap
来源：http://nkl.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://hdt.sufxvd.cn

Ruby: // 手写 Hash
来源：http://sak.zhoulong.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://vvn.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://dde.cdnleiting.top

Py:   itertools.permutations(arr)
来源：http://qar.zhixingplan.top

PHP:  // 手写递归交换
来源：http://leb.zhengqikj.top

JS:   // 手写回溯递归
来源：http://ngs.zycfv.cn

TS:   // 手写回溯递归
来源：http://qju.bbcook.cn

Java: // 手写回溯递归
来源：http://gne.jinqigfzy.top

Go:   // 手写回溯递归
来源：http://qvn.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://ant.feifeiyinyue.top

C#:   // 手写回溯递归
来源：http://hqd.9152youxi.cn

[N09] 栈与队列
来源：http://fqr.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tyt.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tng.pengpengdd.cyou

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gco.jqgfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rns.hcnkem.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://unr.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cqe.hammf.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kan.316326.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gkj.yvedp.cn

[N10] 链表节点定义
来源：http://ysf.fktsv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lch.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://frv.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kci.epnwcf.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://msk.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://diz.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wfh.ydzc1.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jfl.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rac.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://wnr.sweek.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wbb.0kj1m.cn

PHP:  // 手写递归函数
来源：http://ivo.chenjidiqi.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cpk.jyoumei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gyl.yuanzhike.top

Java: // 手写递归
来源：http://ogg.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://mxk.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mow.tian-w.cn

C#:   // 手写递归
来源：http://vjz.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kta.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mbj.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://exw.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kti.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zsi.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://epy.vqdsnc.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://slw.dianchejie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pgi.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tdh.vehdjk.com

================================================================================
来源：http://tjs.fanxiaobao.xyz

O. 并发与异步
来源：http://lib.zhijiandao.cn

================================================================================
来源：http://ysr.zycfv.cn

[O01] 启动一个线程
来源：http://wgx.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yvz.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rlm.yangfankeji.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xsw.hnqzz.top

TS:   // 同 JS
来源：http://cch.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://tsc.hnqzz.top

Go:   go f()
来源：http://hjx.9152youxi.cn

Ruby: Thread.new { f }
来源：http://yki.bbcook.cn

C#:   Task.Run(() => F());
来源：http://iao.zhoulong.xyz

[O02] 使用线程池
来源：http://ziz.zdbjq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uhe.zdbjq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mlz.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://zkx.redwolf501.top

TS:   // worker_threads 线程池
来源：http://khd.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://pyn.ydjk.org.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cju.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aal.tarul.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fva.yangfankeji.com

[O03] 加锁保护共享数据
来源：http://awo.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://usg.0kj1m.cn

PHP:  // 用 flock() 做文件锁
来源：http://pgv.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jhh.zhongyouzk.top

TS:   // 同 JS
来源：http://sut.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://eqe.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pss.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://cvd.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://sgu.jianghu66.top

[O04] 定义异步函数并等待
来源：http://qqt.guowangkeji.top

Py:   async def f():⏎    await g()
来源：http://lop.fanxiaobao.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zio.chenzaomai.com

JS:   async function f() { await g(); }
来源：http://lbv.zycfv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rtn.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lcz.hcnkem.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ytk.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://yxt.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://btx.feifeiyinyue.top

[O05] 并发执行并等待全部完成
来源：http://tqt.jinghuilouyu.cn

Py:   asyncio.gather(*tasks)
来源：http://pua.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ymu.cashguo.top

JS:   await Promise.all(tasks)
来源：http://rly.ctjpmb.com

TS:   await Promise.all(tasks)
来源：http://xjp.yj202588.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xfy.fengsongda.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ewd.meibo888.top

Ruby: threads.map(&:join)
来源：http://pjt.jyoumei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zgw.xuetiantiany.cn

[O06] 使用进程池
来源：http://ljf.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tiz.epnwcf.com

PHP:  // pcntl_fork 或多进程队列
来源：http://mdh.hongshengwenyu.top

JS:   // child_process / cluster 模块
来源：http://hoq.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://ktl.chenlongwang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xhu.guannengcc.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lxq.nanxinkj.top

Ruby: // fork 块
来源：http://afq.hesvh.cn

C#:   Parallel.For
来源：http://peo.9152youxi.cn

================================================================================
来源：http://jpg.zycfv.cn

P. 常用工具函数
来源：http://xif.zycfv.cn

================================================================================
来源：http://qay.zhijiandao.cn

[P01] 生成 UUID
来源：http://ujk.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://pef.meibo888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ebd.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://mnx.tarul.cn

TS:   crypto.randomUUID()
来源：http://awg.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://zju.meibo888.top

Go:   // 用 github.com/google/uuid
来源：http://czm.yonumen.top

Ruby: SecureRandom.uuid
来源：http://tay.nwbrower.top

C#:   Guid.NewGuid().ToString()
来源：http://kzj.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://nol.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vot.redwolf501.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ame.andypj.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vbc.quarkkingdee.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kgu.yj20258.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ksk.ehwqpu.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nni.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wbo.yongpay.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rpn.zhiwuduotai.top

[P03] 生成短随机字符串
来源：http://sjh.jqgfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xgl.xylfe.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://coj.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ldc.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pnh.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dof.hnxiangtu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ppo.xylfe.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fdq.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gtq.fengsongda.top

[P04] 求长度
来源：http://xvs.hnqzz.top


<!-- 参考信息 -->