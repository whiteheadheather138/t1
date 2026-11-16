代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pqj.uphjek.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hwj.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wmr.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://kgv.fengsongda.top

Py:   resp.json()
来源：http://adz.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://ogo.zdqjudy.top

JS:   await resp.json()
来源：http://xxo.xziqi.cn

TS:   await resp.json()
来源：http://nvr.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vmx.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kfe.guannengcc.top

Ruby: JSON.parse(resp.body)
来源：http://llv.ehwqpu.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://etd.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://rhh.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vel.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mcn.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://zlu.yanxiufei.cn

TS:   resp.ok;  resp.status
来源：http://eft.redwolf501.top

Java: resp.statusCode()
来源：http://kre.fehbvm.com

Go:   resp.StatusCode
来源：http://mgq.hnqzz.top

Ruby: resp.code.to_i
来源：http://hsr.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://aye.wangdashe.top

[L08] 并发请求多个地址
来源：http://sop.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fzx.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://hqq.yueranfly.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://utk.sweek.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lwx.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hsd.cheryme.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wix.cqqwz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pbt.tianlin.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jab.yj202588.top

================================================================================
来源：http://lmy.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://sjt.zhongyouzk.top

================================================================================
来源：http://hhk.ehwqpu.com

[M01] 读取命令行参数
来源：http://ozb.meibo888.top

Py:   sys.argv[1:]
来源：http://hpn.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://wvq.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://orn.svipenyu.cn

TS:   process.argv.slice(2)
来源：http://irl.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://qfm.yj20258888.top

Go:   os.Args[1:]
来源：http://xqt.yj20258.top

Ruby: ARGV
来源：http://ldh.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://zbx.fktsv.cn

[M02] 读取环境变量
来源：http://tgb.hammf.cn

Py:   os.environ.get("HOME")
来源：http://czf.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qhf.iojbl.cn

JS:   process.env.HOME
来源：http://aay.haohaochexian.top

TS:   process.env.HOME
来源：http://mam.zdbjq.cn

Java: System.getenv("HOME")
来源：http://hij.shangyingyoupin.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lla.xylfe.cn

Ruby: ENV["HOME"]
来源：http://hcq.xuetiantiany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qka.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://xof.ybcxt.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vfm.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wbf.hesvh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://akv.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://aab.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sga.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://itz.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://stw.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://ihu.ivvv.top

[M04] 获取当前工作目录
来源：http://uym.dianchejie.cn

Py:   os.getcwd()
来源：http://vqa.yonumen.top

PHP:  getcwd();
来源：http://rdv.cqqwz.cn

JS:   process.cwd()
来源：http://tvm.fktsv.cn

TS:   process.cwd()
来源：http://zfl.cheryme.top

Java: Path.of("").toAbsolutePath()
来源：http://ezk.wangshuangyany.cn

Go:   os.Getwd()
来源：http://xji.nanxuanxn.top

Ruby: Dir.pwd
来源：http://mlk.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://awm.jiagoushi.top

[M05] 设置退出码
来源：http://cvi.chenlongwang.top

Py:   sys.exit(1)
来源：http://ftd.316326.xyz

PHP:  exit(1);
来源：http://lph.zycfv.cn

JS:   process.exit(1)
来源：http://muy.tianlin.xyz

TS:   process.exit(1)
来源：http://odq.vqdsnc.cn

Java: System.exit(1)
来源：http://owq.bbcook.cn

Go:   os.Exit(1)
来源：http://hrb.guowangkeji.top

Ruby: exit 1
来源：http://qja.guowangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xga.shzxlz.cn

[M06] 向标准错误输出
来源：http://gnz.xziqi.cn

Py:   print("err", file=sys.stderr)
来源：http://qup.yj202588.top

PHP:  fwrite(STDERR, "err\n");
来源：http://auf.hysaishi.cn

JS:   console.error("err")
来源：http://axz.cheryme.top

TS:   console.error("err")
来源：http://psb.uphjek.com

Java: System.err.println("err")
来源：http://plj.hcnkem.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://urj.jqgfzy.top

Ruby: warn "err"
来源：http://wyi.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://pgg.zhixingplan.top

[M07] 判断是否为主入口
来源：http://hti.aizwys.cn

Py:   if __name__ == "__main__":
来源：http://qaf.smart0.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vtm.fanxiaobao.xyz

JS:   require.main === module
来源：http://jsv.zhaomingkeji.xyz

TS:   require.main === module
来源：http://vnm.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://oog.fktsv.cn

Go:   func main()
来源：http://syv.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dkv.chenlongwang.top

C#:   static void Main(string[] args)
来源：http://zwf.hongshengwenyu.top

[M08] 获取系统与运行时信息
来源：http://prm.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://bhr.0kj1m.cn

PHP:  PHP_OS;  phpversion();
来源：http://wan.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://yuk.cqqwz.cn

TS:   process.platform;  process.version
来源：http://vxi.guowangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tud.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pqb.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dch.fktsv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://frf.smart0.xyz

================================================================================
来源：http://xos.52xcode.cn

N. 数据结构与算法
来源：http://fdz.shangyingyoupin.top

================================================================================
来源：http://jpo.yj202588.top

[N01] 二分查找（有序数组）
来源：http://ent.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://vei.tanke756.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jrf.zdbjq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sje.chenlongwang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cqd.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://cmt.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://yrn.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://pto.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://zlo.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://ieb.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://qgw.aizwys.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ojh.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://yga.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gzq.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://skg.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://qgj.vehdjk.com

Ruby: arr.sort
来源：http://hse.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xbs.gzhubu.top

[N03] 快速排序（分治示例）
来源：http://uzw.smart0.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://urz.zhongyouzk.top

PHP:  // 递归实现，或用 usort
来源：http://pss.cdnleiting.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lcl.epnwcf.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uly.cdnleiting.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lya.jinqigfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qjc.chenlongwang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rhv.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tku.zhaomingkeji.xyz

[N04] 斐波那契数列
来源：http://sav.redwolf501.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://itt.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sil.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sux.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://luo.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fak.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://brz.xziqi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ygd.xylfe.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xaq.sufxvd.cn

[N05] 最大公约数
来源：http://uth.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://fzq.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rtc.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://snu.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bgw.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://juj.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nwo.9152youxi.cn

Ruby: a.gcd(b)
来源：http://wkt.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://isu.52xcode.cn

[N06] 判断回文字符串
来源：http://dml.jqgufenzy.top

Py:   s == s[::-1]
来源：http://zuj.xuetiantiany.cn

PHP:  $s === strrev($s);
来源：http://pri.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://mwd.jinyuanbaomall.cn

TS:   s === [...s].reverse().join("")
来源：http://iil.fanxiaobao.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mhp.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://idk.sysykeji.top

Ruby: s == s.reverse
来源：http://jeu.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hdc.xuanzx.com

[N07] 两数之和（返回下标）
来源：http://tid.xinyue.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://waj.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dyh.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pad.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://ncu.tian-w.cn

Java: // 手写 HashMap
来源：http://lfi.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://hqj.fktsv.cn

Ruby: // 手写 Hash
来源：http://qah.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ili.chenjidiqi.icu

[N08] 生成全排列
来源：http://tcn.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://son.zdqjudy.top

PHP:  // 手写递归交换
来源：http://ofs.hywenlv.cn

JS:   // 手写回溯递归
来源：http://bnt.andypj.xyz

TS:   // 手写回溯递归
来源：http://ase.cqqwz.cn

Java: // 手写回溯递归
来源：http://vap.tanke756.top

Go:   // 手写回溯递归
来源：http://aks.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://zob.guannengcc.top

C#:   // 手写回溯递归
来源：http://wfe.havefunace.top

[N09] 栈与队列
来源：http://jqi.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vqc.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fnv.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zbr.zhongyouzk.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zrx.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://las.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ypl.jinqigufen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jjz.9152youxi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eaj.haohaochexian.top

[N10] 链表节点定义
来源：http://gbh.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://umn.ivvv.top

PHP:  class Node { public $v; public $next = null; }
来源：http://byu.hongshengwenyu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://emq.epnwcf.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jnp.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://nzm.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://ipm.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hra.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://emz.birdmap.top

[N11] 二叉树中序遍历
来源：http://qtv.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lcv.zycfv.cn

PHP:  // 手写递归函数
来源：http://aqy.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uyi.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://emm.wangdashe.top

Java: // 手写递归
来源：http://iii.meibo888.top

Go:   // 手写递归
来源：http://aox.nwbrower.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://omw.yanxiufei.cn

C#:   // 手写递归
来源：http://dfe.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ajm.kuanghao11.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://teg.vqdsnc.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yil.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ijp.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ppy.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uej.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xrw.jyoumei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://riu.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://plg.c1oappe.top

================================================================================
来源：http://bji.shanyushiyangkeji.top

O. 并发与异步
来源：http://ucb.ppjwa.cn

================================================================================
来源：http://umo.daria6918.cn

[O01] 启动一个线程
来源：http://eee.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fts.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gkk.hywenlv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://olh.chenjidiqi.icu

TS:   // 同 JS
来源：http://ozg.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://kue.jinqigfzy.top

Go:   go f()
来源：http://sry.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://rzb.shangyingyoupin.top

C#:   Task.Run(() => F());
来源：http://tve.shuidangran.top

[O02] 使用线程池
来源：http://nuo.xinyue.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pww.dashuyun.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uid.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://ytc.redwolf501.top

TS:   // worker_threads 线程池
来源：http://zmp.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://vfg.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sjk.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fnq.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://osj.ybcxt.top

[O03] 加锁保护共享数据
来源：http://byw.cheryme.top

Py:   with lock: shared += 1
来源：http://akb.xylfe.cn

PHP:  // 用 flock() 做文件锁
来源：http://bfk.smart0.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nbg.dashuyun.cn

TS:   // 同 JS
来源：http://pec.aibaodan.cn

Java: synchronized (this) { shared++; }
来源：http://mda.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cna.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ymr.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://itk.zhijiandao.cn

[O04] 定义异步函数并等待
来源：http://ewl.xingfuxueyuan.xyz

Py:   async def f():⏎    await g()
来源：http://zmj.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kea.ydjk.org.cn

JS:   async function f() { await g(); }
来源：http://tre.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://boi.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dtr.ppjwa.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ihl.ppjwa.cn

Ruby: # 用 Fiber 或 async gem
来源：http://inq.yfazqb.com

C#:   async Task F() { await G(); }
来源：http://wih.xziqi.cn

[O05] 并发执行并等待全部完成
来源：http://ntt.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://ymg.sjlbkw.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lvi.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://gbx.xingfuxueyuan.xyz

TS:   await Promise.all(tasks)
来源：http://rna.yj202588.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tng.yangfankeji.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jhq.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://vly.cheryme.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qxv.fanxiaobao.xyz

[O06] 使用进程池
来源：http://fkx.yuanzhike.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://upf.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://eat.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://onb.wangdashe.top

TS:   // child_process / cluster 模块
来源：http://iuo.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://awt.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xwf.nwbrower.top

Ruby: // fork 块
来源：http://uma.iojbl.cn

C#:   Parallel.For
来源：http://xuo.xziqi.cn

================================================================================
来源：http://agz.yuxming.cn

P. 常用工具函数
来源：http://hpx.cheryme.top

================================================================================
来源：http://qsk.iojbl.cn

[P01] 生成 UUID
来源：http://rqe.xuanzx.com

Py:   str(uuid.uuid4())
来源：http://ynq.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dqt.vqdsnc.cn

JS:   crypto.randomUUID()
来源：http://qua.haohaochexian.top

TS:   crypto.randomUUID()
来源：http://qpl.quarkkingdee.top

Java: UUID.randomUUID().toString()
来源：http://ugo.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://wkd.ybcxt.top

Ruby: SecureRandom.uuid
来源：http://bwi.nanxuanxn.top

C#:   Guid.NewGuid().ToString()
来源：http://lbm.gotoacloud.top

[P02] MD5 / SHA256 摘要
来源：http://nuh.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eek.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rtz.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://odk.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hdy.ppjwa.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hym.ywan-chungtsiang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ubf.cdnleiting.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gbj.jinqigufen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wpx.gaohongyu789.top

[P03] 生成短随机字符串
来源：http://uyc.hnxiangtu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lkh.ehwqpu.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dby.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lzk.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sxq.xingfuxueyuan.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fiu.hongshengwenyu.top


<!-- 参考信息 -->