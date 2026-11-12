代发 wailian999

Py:   resp.json()
来源：http://irs.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://hta.yj20258.top

JS:   await resp.json()
来源：http://wis.jqgufenzy.top

TS:   await resp.json()
来源：http://vnh.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hgi.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pmg.daria6918.cn

Ruby: JSON.parse(resp.body)
来源：http://bvt.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rux.yongpay.top

[L07] 处理 HTTP 状态码
来源：http://ipv.yongpay.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jhf.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://owt.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://mtf.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://mng.bbcook.cn

Java: resp.statusCode()
来源：http://cil.xingfuxueyuan.xyz

Go:   resp.StatusCode
来源：http://ewi.hammf.cn

Ruby: resp.code.to_i
来源：http://gqn.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://edi.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://qmm.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mjd.hcnkem.com

PHP:  curl_multi_init() 系列
来源：http://gnx.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qaq.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kao.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vaa.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iph.c1oappe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://irq.nwbrower.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wcn.yanxiufei.cn

================================================================================
来源：http://udm.hnxiangtu.top

M. 命令行 / 进程 / 环境
来源：http://myt.jyoumei.cn

================================================================================
来源：http://egz.ydjk.org.cn

[M01] 读取命令行参数
来源：http://vhm.gzhubu.top

Py:   sys.argv[1:]
来源：http://qjs.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://qnh.vehdjk.com

JS:   process.argv.slice(2)
来源：http://bwg.iojbl.cn

TS:   process.argv.slice(2)
来源：http://sit.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://mmz.zycfv.cn

Go:   os.Args[1:]
来源：http://ygu.shanyushiyangtech.top

Ruby: ARGV
来源：http://toy.chenzaomai.com

C#:   args 数组（Main 方法参数）
来源：http://rud.zdqjudy.top

[M02] 读取环境变量
来源：http://jeq.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://ots.ydjk.org.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sze.yvedp.cn

JS:   process.env.HOME
来源：http://kgp.gaohongyu789.top

TS:   process.env.HOME
来源：http://yoq.zycfv.cn

Java: System.getenv("HOME")
来源：http://umx.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tas.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://rtb.jqgufenzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pqt.yj20258888.top

[M03] 执行外部命令
来源：http://rvf.birdmap.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://upk.mhx1999.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://szh.shanyushiyangtech.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vlf.chenlongwang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qni.tianlin.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uia.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://amz.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://xfm.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://cum.jqgfzy.top

[M04] 获取当前工作目录
来源：http://toy.yanxiufei.cn

Py:   os.getcwd()
来源：http://slu.vehdjk.com

PHP:  getcwd();
来源：http://kde.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://fqi.daxiang520.top

TS:   process.cwd()
来源：http://yvo.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://anu.zhoulong.xyz

Go:   os.Getwd()
来源：http://joe.chenzaomai.com

Ruby: Dir.pwd
来源：http://dhe.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hwr.cqqwz.cn

[M05] 设置退出码
来源：http://wjm.ywan-chungtsiang.top

Py:   sys.exit(1)
来源：http://wmv.zhaomingkeji.xyz

PHP:  exit(1);
来源：http://uml.chenzaomai.com

JS:   process.exit(1)
来源：http://oys.bbcook.cn

TS:   process.exit(1)
来源：http://hih.zhengqikj.top

Java: System.exit(1)
来源：http://rlu.yfazqb.com

Go:   os.Exit(1)
来源：http://dsn.ywan-chungtsiang.top

Ruby: exit 1
来源：http://gfm.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://snq.tarul.cn

[M06] 向标准错误输出
来源：http://wnk.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://yyq.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://quk.fanxiaobao.xyz

JS:   console.error("err")
来源：http://sdr.hysaishi.cn

TS:   console.error("err")
来源：http://poe.ppjwa.cn

Java: System.err.println("err")
来源：http://wfw.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yku.wangshuangyany.cn

Ruby: warn "err"
来源：http://rce.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://esf.fktsv.cn

[M07] 判断是否为主入口
来源：http://lrq.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://pql.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fjw.jyoumei.cn

JS:   require.main === module
来源：http://dpn.cqqwz.cn

TS:   require.main === module
来源：http://zoz.fktsv.cn

Java: public static void main(String[] args)
来源：http://uth.bbcook.cn

Go:   func main()
来源：http://rfj.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ayn.yj20258888.top

C#:   static void Main(string[] args)
来源：http://lfu.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://zpj.zhongyouzk.top

Py:   platform.system();  platform.python_version()
来源：http://zdx.dashuyun.cn

PHP:  PHP_OS;  phpversion();
来源：http://tqo.cucudq.cn

JS:   process.platform;  process.version
来源：http://qjf.cdnleiting.top

TS:   process.platform;  process.version
来源：http://wow.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bkq.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://whu.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zct.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://etz.haohaochexian.top

================================================================================
来源：http://aad.cdnleiting.top

N. 数据结构与算法
来源：http://muj.havefunace.top

================================================================================
来源：http://khh.sweek.top

[N01] 二分查找（有序数组）
来源：http://rjh.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://yqh.xziqi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xvf.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aqy.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cqi.daria6918.cn

Java: Arrays.binarySearch(arr, x)
来源：http://svn.havefunace.top

Go:   sort.SearchInts(arr, x)
来源：http://idt.chenlongwang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jcf.pycfn.com

C#:   Array.BinarySearch(arr, x)
来源：http://kkn.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://owk.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://exu.nwbrower.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://exw.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jaf.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://etz.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rtj.gogol.net.cn

Go:   slices.Sort(arr)
来源：http://qsp.meibo888.top

Ruby: arr.sort
来源：http://zvt.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gvz.nanxinkj.top

[N03] 快速排序（分治示例）
来源：http://vml.nanxinkj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ssz.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://nos.shuidangran.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://slv.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://avg.jinghuilouyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://icl.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lko.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cdu.xziqi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dgl.bbcook.cn

[N04] 斐波那契数列
来源：http://orf.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eot.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://abm.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ydx.zhengqikj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iaq.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sdp.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cmi.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baj.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zdc.cqqwz.cn

[N05] 最大公约数
来源：http://gip.shzxlz.cn

Py:   math.gcd(a, b)
来源：http://iho.haohaochexian.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cmy.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gha.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uyi.tian-w.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dwa.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://czv.hysaishi.cn

Ruby: a.gcd(b)
来源：http://gux.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://umb.hnxiangtu.top

[N06] 判断回文字符串
来源：http://bqm.sufxvd.cn

Py:   s == s[::-1]
来源：http://jxd.andypj.xyz

PHP:  $s === strrev($s);
来源：http://lar.zhiwuduotai.top

JS:   s === [...s].reverse().join("")
来源：http://his.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://aop.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://des.yueranfly.top

Go:   // 双指针从两端比较
来源：http://xib.jlsjyb.cn

Ruby: s == s.reverse
来源：http://zob.hnqzz.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mpk.yfazqb.com

[N07] 两数之和（返回下标）
来源：http://kvl.wangdashe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fls.pengpengdd.cyou

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hvn.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://vyr.guannengcc.top

TS:   // 手写 Map<string, number>
来源：http://dus.xinyue.icu

Java: // 手写 HashMap
来源：http://xxk.xuetiantiany.cn

Go:   // 手写 map[int]int
来源：http://bmu.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://mon.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mjd.tian-w.cn

[N08] 生成全排列
来源：http://zub.xuetiantiany.cn

Py:   itertools.permutations(arr)
来源：http://vkk.tianlin.xyz

PHP:  // 手写递归交换
来源：http://ice.chenzaomai.com

JS:   // 手写回溯递归
来源：http://qgs.316326.xyz

TS:   // 手写回溯递归
来源：http://hbp.guannengcc.top

Java: // 手写回溯递归
来源：http://jcm.aizwys.cn

Go:   // 手写回溯递归
来源：http://bnt.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://kiu.sufxvd.cn

C#:   // 手写回溯递归
来源：http://ahc.mhx1999.top

[N09] 栈与队列
来源：http://fmk.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jmx.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gve.yvedp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dba.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gyz.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xaz.jinqigfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jck.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qoi.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://icu.yvedp.cn

[N10] 链表节点定义
来源：http://tyy.yuxming.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mhb.gaohongyu789.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sne.dianchejie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qeb.yuanzhike.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tfj.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://hxu.shzxlz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vma.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xlz.jinqigufen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hsn.jqgufenzy.top

[N11] 二叉树中序遍历
来源：http://wqp.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gfk.tianlin.xyz

PHP:  // 手写递归函数
来源：http://ewq.epnwcf.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hyx.wangdashe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://znl.jlsjyb.cn

Java: // 手写递归
来源：http://mlv.pycfn.com

Go:   // 手写递归
来源：http://enw.hnqzz.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xec.hongshengwenyu.top

C#:   // 手写递归
来源：http://kfk.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pnc.birdmap.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://msh.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://key.gzhubu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dlp.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gxv.yanxiufei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tzj.yangfankeji.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xic.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pzf.daria6918.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rlu.shzxlz.cn

================================================================================
来源：http://bmp.chenlongwang.top

O. 并发与异步
来源：http://lvl.hesvh.cn

================================================================================
来源：http://sbe.zhixingplan.top

[O01] 启动一个线程
来源：http://lhi.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bgr.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hkx.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rre.nanxuanxn.top

TS:   // 同 JS
来源：http://mly.52xcode.cn

Java: new Thread(() -> f()).start()
来源：http://rvq.daxiang520.top

Go:   go f()
来源：http://elq.mhx1999.top

Ruby: Thread.new { f }
来源：http://hyo.cucudq.cn

C#:   Task.Run(() => F());
来源：http://lfy.316326.xyz

[O02] 使用线程池
来源：http://wzi.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nlh.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kay.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://nuw.aizwys.cn

TS:   // worker_threads 线程池
来源：http://gch.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://aac.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://was.daria6918.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ngo.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gfn.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://lao.yuanzhike.top

Py:   with lock: shared += 1
来源：http://aub.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://kep.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uqw.aizwys.cn

TS:   // 同 JS
来源：http://hgo.aibaodan.cn

Java: synchronized (this) { shared++; }
来源：http://auy.cdnleiting.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://izd.jyoumei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dlp.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://lzw.xuanzx.com

[O04] 定义异步函数并等待
来源：http://jql.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://tgj.haohaochexian.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rzr.shuidangran.top

JS:   async function f() { await g(); }
来源：http://wgu.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://maw.hnxiangtu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://llw.yueranfly.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rnt.yj20258.top

Ruby: # 用 Fiber 或 async gem
来源：http://udy.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://ays.haohaochexian.top

[O05] 并发执行并等待全部完成
来源：http://tdk.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://nno.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ykq.9152youxi.cn

JS:   await Promise.all(tasks)
来源：http://npq.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://emp.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yhy.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cls.fengsongda.top

Ruby: threads.map(&:join)
来源：http://jyr.jianghu66.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rbx.ywan-chungtsiang.top

[O06] 使用进程池
来源：http://paa.nanxinkj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jwc.sxryk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bdt.cucudq.cn

JS:   // child_process / cluster 模块
来源：http://ztp.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://lcx.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lmj.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bjt.sxryk.cn

Ruby: // fork 块
来源：http://tge.zhoulong.xyz

C#:   Parallel.For
来源：http://auf.ybcxt.top

================================================================================
来源：http://evz.jinqigufen.top

P. 常用工具函数
来源：http://ilh.zhijiandao.cn

================================================================================
来源：http://lwh.sysykeji.top

[P01] 生成 UUID
来源：http://geu.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://isj.fengsongda.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kap.hammf.cn

JS:   crypto.randomUUID()
来源：http://fkv.yueranfly.top

TS:   crypto.randomUUID()
来源：http://yzb.yfazqb.com

Java: UUID.randomUUID().toString()
来源：http://fcy.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://ozl.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://gdw.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://ocy.gzhubu.top

[P02] MD5 / SHA256 摘要
来源：http://ssh.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lyj.hcnkem.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://jjm.nanxinkj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dic.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://emo.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ufb.zhengqikj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sph.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://brt.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://alm.jqgfzy.top

[P03] 生成短随机字符串
来源：http://qge.fktsv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tip.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://flj.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mlt.vqdsnc.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sqq.wangshuangyany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uma.redwolf501.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ajq.hnqzz.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ofu.zhengqikj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://obt.jinqigufen.top

[P04] 求长度
来源：http://tgr.gaohongyu789.top


<!-- 参考信息 -->