代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xun.jinqigufen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eoa.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gkj.jianghu66.top

[L06] 解析响应为 JSON
来源：http://zud.fengsongda.top

Py:   resp.json()
来源：http://shq.316326.xyz

PHP:  json_decode($body, true);
来源：http://mzo.tarul.cn

JS:   await resp.json()
来源：http://mkn.jqgufenzy.top

TS:   await resp.json()
来源：http://ysx.nanxuanxn.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nbw.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ram.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://obq.jianghu66.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bjx.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://fzv.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gob.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pxf.iojbl.cn

JS:   resp.ok;  resp.status
来源：http://zwe.ppjwa.cn

TS:   resp.ok;  resp.status
来源：http://vnu.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://qhn.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://rhf.aizwys.cn

Ruby: resp.code.to_i
来源：http://leb.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://qwg.guowangkeji.top

[L08] 并发请求多个地址
来源：http://hug.birdmap.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pru.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://sjk.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://etc.aibaodan.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mvs.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bam.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://axq.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mdd.zdbjq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gzn.yonumen.top

================================================================================
来源：http://caw.meibo888.top

M. 命令行 / 进程 / 环境
来源：http://yhh.ivvv.top

================================================================================
来源：http://xfa.yj202588.top

[M01] 读取命令行参数
来源：http://nfh.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://foy.birdmap.top

PHP:  $argv;  $argc;
来源：http://tzu.aibaodan.cn

JS:   process.argv.slice(2)
来源：http://mep.jianghu66.top

TS:   process.argv.slice(2)
来源：http://xkv.daxiang520.top

Java: args 数组（main 方法参数）
来源：http://wxs.bbcook.cn

Go:   os.Args[1:]
来源：http://mwh.cheryme.top

Ruby: ARGV
来源：http://oix.jiagoushi.top

C#:   args 数组（Main 方法参数）
来源：http://blz.zhijiandao.cn

[M02] 读取环境变量
来源：http://num.cashguo.top

Py:   os.environ.get("HOME")
来源：http://dgh.wangdashe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oum.nanxinkj.top

JS:   process.env.HOME
来源：http://jta.feifeiyinyue.top

TS:   process.env.HOME
来源：http://jnz.mhx1999.top

Java: System.getenv("HOME")
来源：http://awg.ybcxt.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rxo.hnqzz.top

Ruby: ENV["HOME"]
来源：http://bzc.jianghu66.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gwq.redwolf501.top

[M03] 执行外部命令
来源：http://eec.fktsv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hjm.nanxinkj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uir.pycfn.com

JS:   child_process.execSync("ls -l").toString()
来源：http://hcb.hnxiangtu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://oqx.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pzh.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hyl.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://xsz.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://wmb.jqgufenzy.top

[M04] 获取当前工作目录
来源：http://vio.guannengcc.top

Py:   os.getcwd()
来源：http://hmz.jianghu66.top

PHP:  getcwd();
来源：http://iib.smart0.xyz

JS:   process.cwd()
来源：http://lzs.snrcjt.cn

TS:   process.cwd()
来源：http://ips.hysaishi.cn

Java: Path.of("").toAbsolutePath()
来源：http://hqp.fktsv.cn

Go:   os.Getwd()
来源：http://ojo.snrcjt.cn

Ruby: Dir.pwd
来源：http://oik.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ddn.meibo888.top

[M05] 设置退出码
来源：http://rus.chenjidiqi.icu

Py:   sys.exit(1)
来源：http://arx.sxryk.cn

PHP:  exit(1);
来源：http://iqw.zhongyouzk.top

JS:   process.exit(1)
来源：http://xwu.yongpay.top

TS:   process.exit(1)
来源：http://qwq.jinghuilouyu.cn

Java: System.exit(1)
来源：http://kej.kuanghao11.cn

Go:   os.Exit(1)
来源：http://gaq.bbcook.cn

Ruby: exit 1
来源：http://cvm.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sab.zycfv.cn

[M06] 向标准错误输出
来源：http://erd.fengsongda.top

Py:   print("err", file=sys.stderr)
来源：http://mnp.guannengcc.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mdf.jqgfzy.top

JS:   console.error("err")
来源：http://zgz.bbcook.cn

TS:   console.error("err")
来源：http://vay.zdbjq.cn

Java: System.err.println("err")
来源：http://imo.vqdsnc.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://och.guowangkeji.top

Ruby: warn "err"
来源：http://djn.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://cuc.vehdjk.com

[M07] 判断是否为主入口
来源：http://dgj.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://wmt.tarul.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nui.chenzaomai.com

JS:   require.main === module
来源：http://nof.ybcxt.top

TS:   require.main === module
来源：http://dqt.sysykeji.top

Java: public static void main(String[] args)
来源：http://ubj.shuidangran.top

Go:   func main()
来源：http://mku.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ele.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://kvw.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://zjq.zhiwuduotai.top

Py:   platform.system();  platform.python_version()
来源：http://fxh.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://zuj.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://jwa.tanke756.top

TS:   process.platform;  process.version
来源：http://iwo.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uef.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gsy.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dgs.jinqigufen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cya.birdmap.top

================================================================================
来源：http://vvw.yanxiufei.cn

N. 数据结构与算法
来源：http://vtr.hywenlv.cn

================================================================================
来源：http://whr.aibaodan.cn

[N01] 二分查找（有序数组）
来源：http://iel.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://jip.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://egz.hesvh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jus.nanxuanxn.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pfz.ehwqpu.com

Java: Arrays.binarySearch(arr, x)
来源：http://rod.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://poy.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://hro.wangshuangyany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pyc.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://ojp.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://zjr.zycfv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fdl.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://twv.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://drn.jiagoushi.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sit.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://daj.yj20258.top

Ruby: arr.sort
来源：http://ngi.chenlongwang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hdm.hongshengwenyu.top

[N03] 快速排序（分治示例）
来源：http://msg.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bwo.mhx1999.top

PHP:  // 递归实现，或用 usort
来源：http://sim.c1oappe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pka.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ohi.haohaochexian.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rgj.zhijiandao.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ftv.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aln.yongpay.top

C#:   // 手写递归，或 Array.Sort
来源：http://fuj.zdbjq.cn

[N04] 斐波那契数列
来源：http://rmi.daxiang520.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xrx.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ufy.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blu.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://prt.zhiwuduotai.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xdy.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ljq.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ozq.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yuk.birdmap.top

[N05] 最大公约数
来源：http://two.jlsjyb.cn

Py:   math.gcd(a, b)
来源：http://csb.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://adl.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ddg.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zqs.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ebd.fehbvm.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pay.cashguo.top

Ruby: a.gcd(b)
来源：http://nof.shanyushiyangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nqz.c1oappe.top

[N06] 判断回文字符串
来源：http://qzm.sysykeji.top

Py:   s == s[::-1]
来源：http://irm.daria6918.cn

PHP:  $s === strrev($s);
来源：http://yih.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://wjy.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://anq.cqqwz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pcw.shangyingyoupin.top

Go:   // 双指针从两端比较
来源：http://ewd.yonumen.top

Ruby: s == s.reverse
来源：http://nxw.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pxc.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://uxo.shzxlz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vbg.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ukj.ywan-chungtsiang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yzp.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://gqg.9152youxi.cn

Java: // 手写 HashMap
来源：http://tzm.zhengqikj.top

Go:   // 手写 map[int]int
来源：http://vhh.52xcode.cn

Ruby: // 手写 Hash
来源：http://wpe.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://eqy.meibo888.top

[N08] 生成全排列
来源：http://nwz.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://swj.guannengcc.top

PHP:  // 手写递归交换
来源：http://kbn.ppjwa.cn

JS:   // 手写回溯递归
来源：http://pve.jqgufenzy.top

TS:   // 手写回溯递归
来源：http://mbu.hammf.cn

Java: // 手写回溯递归
来源：http://cjq.yuxming.cn

Go:   // 手写回溯递归
来源：http://mxo.daria6918.cn

Ruby: arr.permutation.to_a
来源：http://hky.316326.xyz

C#:   // 手写回溯递归
来源：http://gyc.andypj.xyz

[N09] 栈与队列
来源：http://plw.ydjk.org.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eeh.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cyk.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xmx.cucudq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fcr.smart0.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://skp.wangshuangyany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://efy.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ffy.hfpthk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ajw.jianghu66.top

[N10] 链表节点定义
来源：http://vay.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wak.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://cex.xziqi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ijk.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jpb.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://hec.jinqigfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://bpz.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qqa.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qpc.jqgufenzy.top

[N11] 二叉树中序遍历
来源：http://upq.havefunace.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tcn.52xcode.cn

PHP:  // 手写递归函数
来源：http://eur.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://asa.bbcook.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rmm.hnqzz.top

Java: // 手写递归
来源：http://cnk.fengsongda.top

Go:   // 手写递归
来源：http://ksv.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mdc.hfpthk.cn

C#:   // 手写递归
来源：http://xrl.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xrf.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ylh.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://joi.yvedp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sly.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bgw.sufxvd.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blz.ydjk.org.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xfq.316326.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://irq.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eiq.svipenyu.cn

================================================================================
来源：http://kis.fengsongda.top

O. 并发与异步
来源：http://fyd.gzhubu.top

================================================================================
来源：http://auz.svipenyu.cn

[O01] 启动一个线程
来源：http://dac.havefunace.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://guj.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pjm.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://awo.yangfankeji.com

TS:   // 同 JS
来源：http://csy.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://nhx.nwbrower.top

Go:   go f()
来源：http://eph.epnwcf.com

Ruby: Thread.new { f }
来源：http://owy.jinqigufen.top

C#:   Task.Run(() => F());
来源：http://gyo.wangshuangyany.cn

[O02] 使用线程池
来源：http://kqp.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cxa.9152youxi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nvu.xylfe.cn

JS:   // worker_threads 线程池
来源：http://jjk.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://hbj.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://jzl.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jbq.shzxlz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://arb.guowangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pop.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://fhz.yueranfly.top

Py:   with lock: shared += 1
来源：http://kga.uphjek.com

PHP:  // 用 flock() 做文件锁
来源：http://psf.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lgz.hesvh.cn

TS:   // 同 JS
来源：http://gxx.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://vej.tian-w.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hvi.sweek.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nll.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://hor.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://tzb.nanxuanxn.top

Py:   async def f():⏎    await g()
来源：http://jmn.zhoulong.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lhy.cashguo.top

JS:   async function f() { await g(); }
来源：http://qna.cashguo.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vja.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sol.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sec.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jhn.svipenyu.cn

C#:   async Task F() { await G(); }
来源：http://jqa.iojbl.cn

[O05] 并发执行并等待全部完成
来源：http://pfp.jyoumei.cn

Py:   asyncio.gather(*tasks)
来源：http://xpi.dashuyun.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yiq.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://cji.tarul.cn

TS:   await Promise.all(tasks)
来源：http://gre.yonumen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uar.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qds.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://lhy.yongpay.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zpi.yongpay.top

[O06] 使用进程池
来源：http://vxt.dashuyun.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kqk.shanyushiyangtech.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lpl.nanxuanxn.top

JS:   // child_process / cluster 模块
来源：http://kzk.shanyushiyangtech.top

TS:   // child_process / cluster 模块
来源：http://aic.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iiz.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lfe.jlsjyb.cn

Ruby: // fork 块
来源：http://poa.shuidangran.top

C#:   Parallel.For
来源：http://kuv.zdbjq.cn

================================================================================
来源：http://jmg.guowangkeji.top

P. 常用工具函数
来源：http://qwh.smart0.xyz

================================================================================
来源：http://lii.cheryme.top

[P01] 生成 UUID
来源：http://cza.tanke756.top

Py:   str(uuid.uuid4())
来源：http://vmf.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yqe.dianchejie.cn

JS:   crypto.randomUUID()
来源：http://foh.mhx1999.top

TS:   crypto.randomUUID()
来源：http://ifz.cdnleiting.top

Java: UUID.randomUUID().toString()
来源：http://ahb.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://vve.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://fvm.feifeiyinyue.top

C#:   Guid.NewGuid().ToString()
来源：http://phm.zycfv.cn

[P02] MD5 / SHA256 摘要
来源：http://ydf.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://acl.shangyingyoupin.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hvh.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yye.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vxu.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uai.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zls.xinyue.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uin.zhiwuduotai.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hhu.epnwcf.com

[P03] 生成短随机字符串
来源：http://cac.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zwq.yvedp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mpe.fanxiaobao.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gab.ywan-chungtsiang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jrm.xuanzx.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ryr.zhengqikj.top


<!-- 参考信息 -->