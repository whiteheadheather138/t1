代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mpr.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pcw.kuanghao11.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rfr.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mku.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qex.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pdc.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lil.ivvv.top

[L06] 解析响应为 JSON
来源：http://eiw.jlsjyb.cn

Py:   resp.json()
来源：http://nvu.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://hdg.jlsjyb.cn

JS:   await resp.json()
来源：http://deq.yfazqb.com

TS:   await resp.json()
来源：http://roy.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://imz.aibaodan.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iof.hnqzz.top

Ruby: JSON.parse(resp.body)
来源：http://kya.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rje.tanke756.top

[L07] 处理 HTTP 状态码
来源：http://oom.bjfxy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sap.shuidangran.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hjd.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://xep.pycfn.com

TS:   resp.ok;  resp.status
来源：http://dby.zhiwuduotai.top

Java: resp.statusCode()
来源：http://rtt.jqgufenzy.top

Go:   resp.StatusCode
来源：http://nyw.chenjidiqi.icu

Ruby: resp.code.to_i
来源：http://dqa.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://bty.daxiang520.top

[L08] 并发请求多个地址
来源：http://utb.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ece.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://ksq.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vfr.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nyf.chenlongwang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mbi.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uzl.yongpay.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nzs.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wog.ivvv.top

================================================================================
来源：http://bcj.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://qvn.c1oappe.top

================================================================================
来源：http://yoq.52xcode.cn

[M01] 读取命令行参数
来源：http://qpg.nwbrower.top

Py:   sys.argv[1:]
来源：http://tgc.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://lho.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://mnc.bjfxy.top

TS:   process.argv.slice(2)
来源：http://iyo.hnxiangtu.top

Java: args 数组（main 方法参数）
来源：http://hnq.quarkkingdee.top

Go:   os.Args[1:]
来源：http://fyj.smart0.xyz

Ruby: ARGV
来源：http://zdn.tarul.cn

C#:   args 数组（Main 方法参数）
来源：http://ccg.yonumen.top

[M02] 读取环境变量
来源：http://pjz.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://eym.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://als.fanxiaobao.xyz

JS:   process.env.HOME
来源：http://dpx.sysykeji.top

TS:   process.env.HOME
来源：http://aja.fktsv.cn

Java: System.getenv("HOME")
来源：http://vjf.quarkkingdee.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vod.nanxuanxn.top

Ruby: ENV["HOME"]
来源：http://dar.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yhe.yangfankeji.com

[M03] 执行外部命令
来源：http://xvk.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pul.zdqjudy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vpg.sufxvd.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://owy.sweek.top

TS:   child_process.execSync("ls -l").toString()
来源：http://loh.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gir.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xpx.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://oor.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://com.aibaodan.cn

[M04] 获取当前工作目录
来源：http://rgw.mhx1999.top

Py:   os.getcwd()
来源：http://yqm.gaohongyu789.top

PHP:  getcwd();
来源：http://wrb.xinyue.icu

JS:   process.cwd()
来源：http://son.vehdjk.com

TS:   process.cwd()
来源：http://pcs.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://hul.yongpay.top

Go:   os.Getwd()
来源：http://hgo.jiagoushi.top

Ruby: Dir.pwd
来源：http://pis.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://nbz.jinqigfzy.top

[M05] 设置退出码
来源：http://yze.ydzc1.top

Py:   sys.exit(1)
来源：http://imw.sweek.top

PHP:  exit(1);
来源：http://ycl.sweek.top

JS:   process.exit(1)
来源：http://ejc.chenzaomai.com

TS:   process.exit(1)
来源：http://qgk.nanxinkj.top

Java: System.exit(1)
来源：http://ptm.pycfn.com

Go:   os.Exit(1)
来源：http://kbf.zhengqikj.top

Ruby: exit 1
来源：http://eqw.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://owd.cqqwz.cn

[M06] 向标准错误输出
来源：http://pbq.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://hdp.xinyue.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://wwu.jianghu66.top

JS:   console.error("err")
来源：http://uhv.fanxiaobao.xyz

TS:   console.error("err")
来源：http://xuv.nwbrower.top

Java: System.err.println("err")
来源：http://suy.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jmb.sufxvd.cn

Ruby: warn "err"
来源：http://qzb.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://ach.0kj1m.cn

[M07] 判断是否为主入口
来源：http://ebr.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://fzk.hysaishi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aau.ivvv.top

JS:   require.main === module
来源：http://uqv.jiagoushi.top

TS:   require.main === module
来源：http://boj.hcnkem.com

Java: public static void main(String[] args)
来源：http://esx.hnxiangtu.top

Go:   func main()
来源：http://sfj.yongpay.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pln.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://zsl.havefunace.top

[M08] 获取系统与运行时信息
来源：http://vol.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://div.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://tag.cdnleiting.top

JS:   process.platform;  process.version
来源：http://agb.yj20258.top

TS:   process.platform;  process.version
来源：http://tgp.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zei.meibo888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://aqp.mhx1999.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qgl.ybcxt.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gmu.andypj.xyz

================================================================================
来源：http://htr.ppjwa.cn

N. 数据结构与算法
来源：http://lmk.kuanghao11.cn

================================================================================
来源：http://gtd.tanke756.top

[N01] 二分查找（有序数组）
来源：http://ipe.xuetiantiany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qlj.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qzc.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wym.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qgl.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://zcg.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://zvg.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://spd.fengsongda.top

C#:   Array.BinarySearch(arr, x)
来源：http://pbl.guannengcc.top

[N02] 排序（工程实践用内置实现）
来源：http://npi.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://zpk.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jjq.zhongyouzk.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://slj.quarkkingdee.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://irc.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lfd.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://ltq.ydjk.org.cn

Ruby: arr.sort
来源：http://jza.yvedp.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mxl.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://crp.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qao.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://kar.pengpengdd.cyou

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cad.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dki.ivvv.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hkf.hysaishi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vbb.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vbp.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://vdh.ivvv.top

[N04] 斐波那契数列
来源：http://cxr.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uhm.fanxiaobao.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dnh.yfazqb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tiu.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qjf.tanke756.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ovq.zhongyouzk.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rxy.sweek.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bqv.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xtu.shangyingyoupin.top

[N05] 最大公约数
来源：http://pmq.andypj.xyz

Py:   math.gcd(a, b)
来源：http://wci.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oed.jinqigufen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mky.gotoacloud.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://obx.fehbvm.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nmm.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ids.zdqjudy.top

Ruby: a.gcd(b)
来源：http://znd.jinghuilouyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eqt.hysaishi.cn

[N06] 判断回文字符串
来源：http://amp.shzxlz.cn

Py:   s == s[::-1]
来源：http://thd.vehdjk.com

PHP:  $s === strrev($s);
来源：http://aln.jqgufenzy.top

JS:   s === [...s].reverse().join("")
来源：http://uch.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://frp.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bvr.vehdjk.com

Go:   // 双指针从两端比较
来源：http://zds.ydjk.org.cn

Ruby: s == s.reverse
来源：http://ubd.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wdw.zhongyouzk.top

[N07] 两数之和（返回下标）
来源：http://cli.uphjek.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zut.svipenyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qfm.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://qgo.hongshengwenyu.top

TS:   // 手写 Map<string, number>
来源：http://szs.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://jwe.shanyushiyangtech.top

Go:   // 手写 map[int]int
来源：http://uog.guowangkeji.top

Ruby: // 手写 Hash
来源：http://iyv.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://uqz.chenlongwang.top

[N08] 生成全排列
来源：http://umu.hammf.cn

Py:   itertools.permutations(arr)
来源：http://kdw.kuanghao11.cn

PHP:  // 手写递归交换
来源：http://jwk.hcnkem.com

JS:   // 手写回溯递归
来源：http://saw.9152youxi.cn

TS:   // 手写回溯递归
来源：http://hst.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://qtp.ybcxt.top

Go:   // 手写回溯递归
来源：http://vjw.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://lab.fzhhl.top

C#:   // 手写回溯递归
来源：http://prn.yj20258888.top

[N09] 栈与队列
来源：http://wbp.gogol.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://djx.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zzd.nwbrower.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://veb.havefunace.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jmu.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://shc.zhijiandao.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wqh.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uot.zhengqikj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://erm.uphjek.com

[N10] 链表节点定义
来源：http://vdf.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kbu.xuanzx.com

PHP:  class Node { public $v; public $next = null; }
来源：http://kdm.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://olu.dashuyun.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cwo.tian-w.cn

Java: class Node { int v; Node next; }
来源：http://agu.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://cbt.0kj1m.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sde.feifeiyinyue.top

C#:   class Node { public int V; public Node? Next; }
来源：http://csa.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://rhx.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://heu.jlsjyb.cn

PHP:  // 手写递归函数
来源：http://wzu.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://otj.jqgfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://azt.yuanzhike.top

Java: // 手写递归
来源：http://isf.c1oappe.top

Go:   // 手写递归
来源：http://lmx.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qgx.tanke756.top

C#:   // 手写递归
来源：http://azp.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nit.316326.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hqq.redwolf501.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bgk.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pid.yfazqb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ahh.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lrh.smart0.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dus.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fox.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tbu.gzhubu.top

================================================================================
来源：http://oig.cucudq.cn

O. 并发与异步
来源：http://cso.aibaodan.cn

================================================================================
来源：http://wxz.yj20258888.top

[O01] 启动一个线程
来源：http://vls.chenjidiqi.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zyo.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xrh.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fci.jiagoushi.top

TS:   // 同 JS
来源：http://fxm.zhoulong.xyz

Java: new Thread(() -> f()).start()
来源：http://dfh.yj202588.top

Go:   go f()
来源：http://nmu.jianghu66.top

Ruby: Thread.new { f }
来源：http://yih.wangshuangyany.cn

C#:   Task.Run(() => F());
来源：http://tcq.xinyue.icu

[O02] 使用线程池
来源：http://kwj.zdbjq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cav.gaohongyu789.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qlj.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://kke.guannengcc.top

TS:   // worker_threads 线程池
来源：http://zlp.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://gzh.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kfv.tian-w.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wtj.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dlf.guannengcc.top

[O03] 加锁保护共享数据
来源：http://fep.yuxming.cn

Py:   with lock: shared += 1
来源：http://eoy.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://jrp.nanxinkj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cym.wangshuangyany.cn

TS:   // 同 JS
来源：http://zpn.xziqi.cn

Java: synchronized (this) { shared++; }
来源：http://ahr.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://snt.aizwys.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qey.tarul.cn

C#:   lock (gate) { shared++; }
来源：http://hue.yfazqb.com

[O04] 定义异步函数并等待
来源：http://jdy.xinyue.icu

Py:   async def f():⏎    await g()
来源：http://fgz.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lhw.cashguo.top

JS:   async function f() { await g(); }
来源：http://zer.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hxa.hnqzz.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mun.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://poo.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://pak.pycfn.com

C#:   async Task F() { await G(); }
来源：http://gvu.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://hdu.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://rop.fanxiaobao.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hip.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://qqt.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://pdj.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zqc.hfpthk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kcf.dianchejie.cn

Ruby: threads.map(&:join)
来源：http://dwj.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gmc.zhengqikj.top

[O06] 使用进程池
来源：http://yhz.ppjwa.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://afy.yuxming.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zri.smart0.xyz

JS:   // child_process / cluster 模块
来源：http://fqk.sysykeji.top

TS:   // child_process / cluster 模块
来源：http://wed.jqgfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tiv.vqdsnc.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xsu.vehdjk.com

Ruby: // fork 块
来源：http://pjs.ppjwa.cn

C#:   Parallel.For
来源：http://iou.nanxuanxn.top

================================================================================
来源：http://xfs.chenlongwang.top

P. 常用工具函数
来源：http://gvm.xuetiantiany.cn

================================================================================
来源：http://miv.ctjpmb.com

[P01] 生成 UUID
来源：http://zzb.xziqi.cn

Py:   str(uuid.uuid4())
来源：http://ear.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ezo.ywan-chungtsiang.top

JS:   crypto.randomUUID()
来源：http://ltj.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://sbz.aizwys.cn

Java: UUID.randomUUID().toString()
来源：http://jzn.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://aqz.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://mao.ywan-chungtsiang.top

C#:   Guid.NewGuid().ToString()
来源：http://cjz.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://hdx.daria6918.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://amx.fzhhl.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qrh.meibo888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://efb.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kfz.ydzc1.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nbw.xinyue.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kck.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fpq.smart0.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ema.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://rfv.xinyue.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uqi.zhongyouzk.top


<!-- 参考信息 -->