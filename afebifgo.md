代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eby.ctjpmb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ybf.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jlh.hnqzz.top

[L06] 解析响应为 JSON
来源：http://omo.hcnkem.com

Py:   resp.json()
来源：http://pmp.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://bna.yueranfly.top

JS:   await resp.json()
来源：http://rfo.yfazqb.com

TS:   await resp.json()
来源：http://cse.smart0.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zja.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ffj.ydjk.org.cn

Ruby: JSON.parse(resp.body)
来源：http://fhs.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dnb.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://bpw.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ehi.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jsu.cheryme.top

JS:   resp.ok;  resp.status
来源：http://tcz.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://war.uphjek.com

Java: resp.statusCode()
来源：http://cmv.tian-w.cn

Go:   resp.StatusCode
来源：http://uxq.jinyuanbaomall.cn

Ruby: resp.code.to_i
来源：http://lat.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://thq.yuanzhike.top

[L08] 并发请求多个地址
来源：http://gou.52xcode.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tod.gzhubu.top

PHP:  curl_multi_init() 系列
来源：http://xlb.jqgfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://klq.sysykeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fus.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ngb.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jvx.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rjt.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://huj.yangfankeji.com

================================================================================
来源：http://kzv.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://ibn.daria6918.cn

================================================================================
来源：http://rlw.jinghuilouyu.cn

[M01] 读取命令行参数
来源：http://sip.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://roq.daxiang520.top

PHP:  $argv;  $argc;
来源：http://zmg.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://bcw.gogol.net.cn

TS:   process.argv.slice(2)
来源：http://fmg.hammf.cn

Java: args 数组（main 方法参数）
来源：http://jgt.gaohongyu789.top

Go:   os.Args[1:]
来源：http://rak.birdmap.top

Ruby: ARGV
来源：http://arn.aizwys.cn

C#:   args 数组（Main 方法参数）
来源：http://nrb.c1oappe.top

[M02] 读取环境变量
来源：http://uzs.zhiwuduotai.top

Py:   os.environ.get("HOME")
来源：http://zfl.haohaochexian.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://drd.ehwqpu.com

JS:   process.env.HOME
来源：http://xvs.sufxvd.cn

TS:   process.env.HOME
来源：http://ipz.haohaochexian.top

Java: System.getenv("HOME")
来源：http://ugm.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qaw.vehdjk.com

Ruby: ENV["HOME"]
来源：http://jgt.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://evg.yonumen.top

[M03] 执行外部命令
来源：http://ynb.cucudq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tcj.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lcx.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fnw.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kpa.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gdu.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yyy.hfpthk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rzc.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://izl.ehwqpu.com

[M04] 获取当前工作目录
来源：http://xlx.316326.xyz

Py:   os.getcwd()
来源：http://kzb.sufxvd.cn

PHP:  getcwd();
来源：http://sgz.guannengcc.top

JS:   process.cwd()
来源：http://key.fengsongda.top

TS:   process.cwd()
来源：http://ojs.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://lla.daria6918.cn

Go:   os.Getwd()
来源：http://zno.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://hpz.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://sza.zhiwuduotai.top

[M05] 设置退出码
来源：http://yov.jinghuilouyu.cn

Py:   sys.exit(1)
来源：http://fis.52xcode.cn

PHP:  exit(1);
来源：http://xti.cqqwz.cn

JS:   process.exit(1)
来源：http://ttx.jinghuilouyu.cn

TS:   process.exit(1)
来源：http://ebg.ybcxt.top

Java: System.exit(1)
来源：http://uzk.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://xog.uphjek.com

Ruby: exit 1
来源：http://qzy.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ask.xingfuxueyuan.xyz

[M06] 向标准错误输出
来源：http://fba.shanyushiyangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://gtg.yfazqb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://sla.ydjk.org.cn

JS:   console.error("err")
来源：http://wqb.zhijiandao.cn

TS:   console.error("err")
来源：http://yhu.sysykeji.top

Java: System.err.println("err")
来源：http://ece.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sik.shanyushiyangtech.top

Ruby: warn "err"
来源：http://bfe.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://hif.ydjk.org.cn

[M07] 判断是否为主入口
来源：http://eok.sysykeji.top

Py:   if __name__ == "__main__":
来源：http://hcz.shanyushiyangtech.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://acx.kuanghao11.cn

JS:   require.main === module
来源：http://bjv.nanxinkj.top

TS:   require.main === module
来源：http://vhv.ehwqpu.com

Java: public static void main(String[] args)
来源：http://xww.aibaodan.cn

Go:   func main()
来源：http://ckw.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dtu.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://obu.havefunace.top

[M08] 获取系统与运行时信息
来源：http://tbn.zhiwuduotai.top

Py:   platform.system();  platform.python_version()
来源：http://ryj.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://ssj.ivvv.top

JS:   process.platform;  process.version
来源：http://gsv.zhijiandao.cn

TS:   process.platform;  process.version
来源：http://kja.jinqigfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ypg.kuanghao11.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://igw.zhiwuduotai.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zpk.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lcu.snrcjt.cn

================================================================================
来源：http://ron.jinghuilouyu.cn

N. 数据结构与算法
来源：http://vnr.quarkkingdee.top

================================================================================
来源：http://mre.hongshengwenyu.top

[N01] 二分查找（有序数组）
来源：http://pla.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mjd.yuanzhike.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wsm.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fxl.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kpq.9152youxi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://czj.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://hzo.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hmn.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://nbj.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://nvg.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://fnn.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eop.xinyue.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://oqz.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ejp.daxiang520.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rqf.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://hni.bbcook.cn

Ruby: arr.sort
来源：http://tyc.tian-w.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mnp.zhixingplan.top

[N03] 快速排序（分治示例）
来源：http://nrn.yvedp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xak.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://afa.shanyushiyangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aob.yongpay.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qyl.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ubs.zdqjudy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wpi.jinyuanbaomall.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xgr.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://hka.pycfn.com

[N04] 斐波那契数列
来源：http://tne.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://llk.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sui.guannengcc.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://htf.jqgufenzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zfk.jianghu66.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nce.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pdw.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://elb.tarul.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lpm.sxryk.cn

[N05] 最大公约数
来源：http://atd.andypj.xyz

Py:   math.gcd(a, b)
来源：http://ppl.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ddp.yj20258888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pbk.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wyt.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kxv.gotoacloud.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vqp.cashguo.top

Ruby: a.gcd(b)
来源：http://ssp.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jia.hysaishi.cn

[N06] 判断回文字符串
来源：http://zwz.yonumen.top

Py:   s == s[::-1]
来源：http://stp.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://wen.ybcxt.top

JS:   s === [...s].reverse().join("")
来源：http://kjz.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://yyp.fzhhl.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gdn.cashguo.top

Go:   // 双指针从两端比较
来源：http://rcm.nanxinkj.top

Ruby: s == s.reverse
来源：http://pny.yj20258.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ssu.hcnkem.com

[N07] 两数之和（返回下标）
来源：http://tws.cheryme.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ffk.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ehw.zhoulong.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://odk.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://njl.jqgfzy.top

Java: // 手写 HashMap
来源：http://uwx.yanxiufei.cn

Go:   // 手写 map[int]int
来源：http://del.shanyushiyangtech.top

Ruby: // 手写 Hash
来源：http://cgb.hysaishi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://old.zhongyouzk.top

[N08] 生成全排列
来源：http://lza.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://yzb.jqgufenzy.top

PHP:  // 手写递归交换
来源：http://oet.tianlin.xyz

JS:   // 手写回溯递归
来源：http://odk.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://sma.daria6918.cn

Java: // 手写回溯递归
来源：http://tiu.zdbjq.cn

Go:   // 手写回溯递归
来源：http://pfs.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://hpl.ctjpmb.com

C#:   // 手写回溯递归
来源：http://afv.tanke756.top

[N09] 栈与队列
来源：http://snd.uphjek.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ttj.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hsv.meibo888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aat.chenzaomai.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lts.tianlin.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fok.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zed.jinyuanbaomall.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ujs.tarul.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://afi.gotoacloud.top

[N10] 链表节点定义
来源：http://cqx.zycfv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fcj.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://kxb.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ewf.xylfe.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://juc.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://eza.wangdashe.top

Go:   type Node struct { V int; Next *Node }
来源：http://etg.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://faa.cucudq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xjl.zhengqikj.top

[N11] 二叉树中序遍历
来源：http://qni.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://enz.chenjidiqi.icu

PHP:  // 手写递归函数
来源：http://lnj.cashguo.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sxm.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wgt.cashguo.top

Java: // 手写递归
来源：http://vyz.ppjwa.cn

Go:   // 手写递归
来源：http://dwy.hywenlv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rhd.fktsv.cn

C#:   // 手写递归
来源：http://bbr.sjlbkw.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://glp.zhengqikj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bzj.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wtd.gotoacloud.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nfk.gaohongyu789.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ody.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cgk.52xcode.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uev.yanxiufei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://koh.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mbm.hfpthk.cn

================================================================================
来源：http://rug.52xcode.cn

O. 并发与异步
来源：http://kve.ydjk.org.cn

================================================================================
来源：http://qji.0kj1m.cn

[O01] 启动一个线程
来源：http://cbv.ybcxt.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rme.cashguo.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ulj.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mpd.gogol.net.cn

TS:   // 同 JS
来源：http://rgf.hcnkem.com

Java: new Thread(() -> f()).start()
来源：http://zaq.sxryk.cn

Go:   go f()
来源：http://gxp.fengsongda.top

Ruby: Thread.new { f }
来源：http://put.yonumen.top

C#:   Task.Run(() => F());
来源：http://kse.vqdsnc.cn

[O02] 使用线程池
来源：http://msq.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lxd.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uet.xziqi.cn

JS:   // worker_threads 线程池
来源：http://ihj.andypj.xyz

TS:   // worker_threads 线程池
来源：http://kjo.9152youxi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://auw.ywan-chungtsiang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bgi.zhengqikj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dad.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fet.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://hfq.xinyue.icu

Py:   with lock: shared += 1
来源：http://ihd.xylfe.cn

PHP:  // 用 flock() 做文件锁
来源：http://qwn.guowangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://coc.shanyushiyangtech.top

TS:   // 同 JS
来源：http://bsl.yuanzhike.top

Java: synchronized (this) { shared++; }
来源：http://guo.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eby.havefunace.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jzy.zycfv.cn

C#:   lock (gate) { shared++; }
来源：http://vcj.mhx1999.top

[O04] 定义异步函数并等待
来源：http://cas.zdbjq.cn

Py:   async def f():⏎    await g()
来源：http://rmg.daria6918.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tjy.guannengcc.top

JS:   async function f() { await g(); }
来源：http://bfi.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fgt.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xpw.yanxiufei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hpe.jlsjyb.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qku.uphjek.com

C#:   async Task F() { await G(); }
来源：http://dfv.wangdashe.top

[O05] 并发执行并等待全部完成
来源：http://hqs.birdmap.top

Py:   asyncio.gather(*tasks)
来源：http://nbx.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jas.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://cht.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://hft.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gcn.zhongyouzk.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yad.yueranfly.top

Ruby: threads.map(&:join)
来源：http://dug.zycfv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sfv.jinghuilouyu.cn

[O06] 使用进程池
来源：http://dod.fzhhl.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://djh.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dbg.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://rjt.pengpengdd.cyou

TS:   // child_process / cluster 模块
来源：http://blh.wangshuangyany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pyp.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ekv.shuidangran.top

Ruby: // fork 块
来源：http://tth.jyoumei.cn

C#:   Parallel.For
来源：http://fnz.zhengqikj.top

================================================================================
来源：http://hrn.gzhubu.top

P. 常用工具函数
来源：http://jfc.zhengqikj.top

================================================================================
来源：http://eoe.zdqjudy.top

[P01] 生成 UUID
来源：http://jcn.guannengcc.top

Py:   str(uuid.uuid4())
来源：http://swp.epnwcf.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://woo.zhixingplan.top

JS:   crypto.randomUUID()
来源：http://vmq.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://myb.sweek.top

Java: UUID.randomUUID().toString()
来源：http://poz.fehbvm.com

Go:   // 用 github.com/google/uuid
来源：http://vde.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://twf.jlsjyb.cn

C#:   Guid.NewGuid().ToString()
来源：http://dww.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://cxk.ydzc1.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kca.gogol.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ovq.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hbn.smart0.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gqr.shanyushiyangtech.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hsh.zhengqikj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ssu.uphjek.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bpw.jinyuanbaomall.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://amb.yuxming.cn

[P03] 生成短随机字符串
来源：http://tbj.yj20258.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ufd.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zjt.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pae.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qeb.chenzaomai.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vww.gotoacloud.top


<!-- 参考信息 -->