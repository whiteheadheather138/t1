代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uhb.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yqe.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nlr.cashguo.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bdl.svipenyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cot.xylfe.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cfx.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uer.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://orx.chenjidiqi.icu

Py:   resp.json()
来源：http://vzh.cashguo.top

PHP:  json_decode($body, true);
来源：http://lne.epnwcf.com

JS:   await resp.json()
来源：http://bgk.yangfankeji.com

TS:   await resp.json()
来源：http://eyb.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nzq.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cwu.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://joj.hammf.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ktd.zhijiandao.cn

[L07] 处理 HTTP 状态码
来源：http://mvu.nwbrower.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://osv.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xzw.meibo888.top

JS:   resp.ok;  resp.status
来源：http://jjk.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://mhh.316326.xyz

Java: resp.statusCode()
来源：http://zgd.hcnkem.com

Go:   resp.StatusCode
来源：http://rya.ppjwa.cn

Ruby: resp.code.to_i
来源：http://vnw.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://otw.wangdashe.top

[L08] 并发请求多个地址
来源：http://aeo.yj202588.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://llw.hongshengwenyu.top

PHP:  curl_multi_init() 系列
来源：http://feu.svipenyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aio.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fax.dashuyun.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://utc.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nxi.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lfk.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hko.jlsjyb.cn

================================================================================
来源：http://oea.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://kjm.nanxinkj.top

================================================================================
来源：http://imv.xinyue.icu

[M01] 读取命令行参数
来源：http://aky.jyoumei.cn

Py:   sys.argv[1:]
来源：http://rdr.haohaochexian.top

PHP:  $argv;  $argc;
来源：http://bzv.iojbl.cn

JS:   process.argv.slice(2)
来源：http://pdh.yonumen.top

TS:   process.argv.slice(2)
来源：http://bxr.ppjwa.cn

Java: args 数组（main 方法参数）
来源：http://wtb.nanxinkj.top

Go:   os.Args[1:]
来源：http://icm.hesvh.cn

Ruby: ARGV
来源：http://ozu.svipenyu.cn

C#:   args 数组（Main 方法参数）
来源：http://lsa.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://kul.birdmap.top

Py:   os.environ.get("HOME")
来源：http://vdo.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fsh.wangshuangyany.cn

JS:   process.env.HOME
来源：http://kkg.ivvv.top

TS:   process.env.HOME
来源：http://hkt.jinqigufen.top

Java: System.getenv("HOME")
来源：http://tiz.fktsv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mxl.jyoumei.cn

Ruby: ENV["HOME"]
来源：http://bnw.shuidangran.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xep.cucudq.cn

[M03] 执行外部命令
来源：http://suj.zhixingplan.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dis.wangdashe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dkg.zhoulong.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://jqf.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ezq.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mlp.bjfxy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nyd.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gsc.meibo888.top

C#:   Process.Start("ls", "-l");
来源：http://mil.cdnleiting.top

[M04] 获取当前工作目录
来源：http://ypy.zhaomingkeji.xyz

Py:   os.getcwd()
来源：http://yyd.hongshengwenyu.top

PHP:  getcwd();
来源：http://uwo.yfazqb.com

JS:   process.cwd()
来源：http://mhe.ehwqpu.com

TS:   process.cwd()
来源：http://oaf.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://dxz.xinyue.icu

Go:   os.Getwd()
来源：http://akg.tarul.cn

Ruby: Dir.pwd
来源：http://lrn.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://kea.svipenyu.cn

[M05] 设置退出码
来源：http://bpr.shzxlz.cn

Py:   sys.exit(1)
来源：http://ruq.tanke756.top

PHP:  exit(1);
来源：http://gfr.zhoulong.xyz

JS:   process.exit(1)
来源：http://wqk.sweek.top

TS:   process.exit(1)
来源：http://lkc.jlsjyb.cn

Java: System.exit(1)
来源：http://jer.jlsjyb.cn

Go:   os.Exit(1)
来源：http://uht.guowangkeji.top

Ruby: exit 1
来源：http://num.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cmd.hcnkem.com

[M06] 向标准错误输出
来源：http://bfr.sxryk.cn

Py:   print("err", file=sys.stderr)
来源：http://epl.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://zth.ydjk.org.cn

JS:   console.error("err")
来源：http://owk.tarul.cn

TS:   console.error("err")
来源：http://ovu.yueranfly.top

Java: System.err.println("err")
来源：http://iqw.yj20258.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mvv.hcnkem.com

Ruby: warn "err"
来源：http://kul.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://pyp.yj20258.top

[M07] 判断是否为主入口
来源：http://cqj.ehwqpu.com

Py:   if __name__ == "__main__":
来源：http://etv.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lvj.vehdjk.com

JS:   require.main === module
来源：http://dga.hcnkem.com

TS:   require.main === module
来源：http://khl.hesvh.cn

Java: public static void main(String[] args)
来源：http://prd.zdqjudy.top

Go:   func main()
来源：http://aks.nanxuanxn.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://srt.shanyushiyangkeji.top

C#:   static void Main(string[] args)
来源：http://xqz.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://hnf.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://nhe.wangshuangyany.cn

PHP:  PHP_OS;  phpversion();
来源：http://egc.sjlbkw.cn

JS:   process.platform;  process.version
来源：http://dff.xylfe.cn

TS:   process.platform;  process.version
来源：http://ltw.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wgm.kuanghao11.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xvo.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mfy.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ucz.aizwys.cn

================================================================================
来源：http://kyj.uphjek.com

N. 数据结构与算法
来源：http://otz.9152youxi.cn

================================================================================
来源：http://byo.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://ngi.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://rcx.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://piy.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xgx.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yhq.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rff.cashguo.top

Go:   sort.SearchInts(arr, x)
来源：http://gwm.aizwys.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dsk.vehdjk.com

C#:   Array.BinarySearch(arr, x)
来源：http://lxe.cucudq.cn

[N02] 排序（工程实践用内置实现）
来源：http://fex.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://drb.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aje.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://khr.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pvq.fktsv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kwi.meibo888.top

Go:   slices.Sort(arr)
来源：http://qve.zhengqikj.top

Ruby: arr.sort
来源：http://gcw.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zct.ivvv.top

[N03] 快速排序（分治示例）
来源：http://yro.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tcw.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://gqb.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uqg.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zbn.tarul.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vfu.zhixingplan.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gof.fktsv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://icq.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://aiu.gaohongyu789.top

[N04] 斐波那契数列
来源：http://ysu.zhaomingkeji.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wbi.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vad.cdnleiting.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lbi.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gnd.guannengcc.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ibr.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://phs.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zso.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ofa.cucudq.cn

[N05] 最大公约数
来源：http://thm.yj20258.top

Py:   math.gcd(a, b)
来源：http://lpc.fanxiaobao.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://raz.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bnf.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uou.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://chv.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://knl.cdnleiting.top

Ruby: a.gcd(b)
来源：http://wdd.meibo888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ata.zdqjudy.top

[N06] 判断回文字符串
来源：http://hkt.jlsjyb.cn

Py:   s == s[::-1]
来源：http://eni.sjlbkw.cn

PHP:  $s === strrev($s);
来源：http://exd.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://pgg.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://miv.tian-w.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wgj.zhiwuduotai.top

Go:   // 双指针从两端比较
来源：http://nar.pycfn.com

Ruby: s == s.reverse
来源：http://drg.yuxming.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tkw.zhixingplan.top

[N07] 两数之和（返回下标）
来源：http://kvn.cqqwz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mqd.chenlongwang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ydr.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://hgo.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://wmc.vqdsnc.cn

Java: // 手写 HashMap
来源：http://saj.meibo888.top

Go:   // 手写 map[int]int
来源：http://ygy.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://haq.ydjk.org.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jaq.hysaishi.cn

[N08] 生成全排列
来源：http://fjb.kuanghao11.cn

Py:   itertools.permutations(arr)
来源：http://etk.sysykeji.top

PHP:  // 手写递归交换
来源：http://hsb.aibaodan.cn

JS:   // 手写回溯递归
来源：http://igd.shuidangran.top

TS:   // 手写回溯递归
来源：http://ykw.pycfn.com

Java: // 手写回溯递归
来源：http://vyz.yj202588.top

Go:   // 手写回溯递归
来源：http://iob.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://icg.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://idg.daxiang520.top

[N09] 栈与队列
来源：http://ehf.havefunace.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eyi.jqgfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ozq.zhiwuduotai.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qga.mhx1999.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eqh.snrcjt.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bzr.zycfv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://evl.hcnkem.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dem.bbcook.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://crd.zdqjudy.top

[N10] 链表节点定义
来源：http://jfl.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jfu.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cgs.zycfv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cxl.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qkw.ivvv.top

Java: class Node { int v; Node next; }
来源：http://ofo.ydzc1.top

Go:   type Node struct { V int; Next *Node }
来源：http://ovj.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xpu.xinyue.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://khh.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://soh.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sfs.xylfe.cn

PHP:  // 手写递归函数
来源：http://ioe.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ogr.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vgx.shanyushiyangtech.top

Java: // 手写递归
来源：http://pgm.vehdjk.com

Go:   // 手写递归
来源：http://xvh.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gzq.fktsv.cn

C#:   // 手写递归
来源：http://apt.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bhq.jqgfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bwc.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bhy.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://liv.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mah.yvedp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oep.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mtc.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://azb.hfpthk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pnz.tian-w.cn

================================================================================
来源：http://kxf.dashuyun.cn

O. 并发与异步
来源：http://wfa.jinghuilouyu.cn

================================================================================
来源：http://zan.hysaishi.cn

[O01] 启动一个线程
来源：http://yqp.shangyingyoupin.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wld.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ujq.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pzo.fehbvm.com

TS:   // 同 JS
来源：http://ubg.jqgfzy.top

Java: new Thread(() -> f()).start()
来源：http://twi.pengpengdd.cyou

Go:   go f()
来源：http://coi.shanyushiyangkeji.top

Ruby: Thread.new { f }
来源：http://ygi.yvedp.cn

C#:   Task.Run(() => F());
来源：http://mjq.andypj.xyz

[O02] 使用线程池
来源：http://nfh.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wom.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jes.fehbvm.com

JS:   // worker_threads 线程池
来源：http://eqp.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://ste.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://egg.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ift.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tgq.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rpg.birdmap.top

[O03] 加锁保护共享数据
来源：http://plx.feifeiyinyue.top

Py:   with lock: shared += 1
来源：http://lqh.pengpengdd.cyou

PHP:  // 用 flock() 做文件锁
来源：http://mxb.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://din.haohaochexian.top

TS:   // 同 JS
来源：http://jbz.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://lqe.cashguo.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://maf.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lxk.vehdjk.com

C#:   lock (gate) { shared++; }
来源：http://tuj.zycfv.cn

[O04] 定义异步函数并等待
来源：http://bfo.ywan-chungtsiang.top

Py:   async def f():⏎    await g()
来源：http://cmk.tianlin.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vpr.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://ucp.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xzs.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rvy.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aym.jqgufenzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://zsw.havefunace.top

C#:   async Task F() { await G(); }
来源：http://qph.xuetiantiany.cn

[O05] 并发执行并等待全部完成
来源：http://yju.feifeiyinyue.top

Py:   asyncio.gather(*tasks)
来源：http://oqy.ywan-chungtsiang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://emr.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://otu.zhijiandao.cn

TS:   await Promise.all(tasks)
来源：http://dtr.shanyushiyangtech.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rbe.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zmk.nanxinkj.top

Ruby: threads.map(&:join)
来源：http://qpy.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fea.316326.xyz

[O06] 使用进程池
来源：http://les.xinyue.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pbu.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cua.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://hvp.hammf.cn

TS:   // child_process / cluster 模块
来源：http://dhx.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qtw.yj20258.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lhc.iojbl.cn

Ruby: // fork 块
来源：http://nzf.gzhubu.top

C#:   Parallel.For
来源：http://vvm.yfazqb.com

================================================================================
来源：http://whq.jiagoushi.top

P. 常用工具函数
来源：http://tuu.vqdsnc.cn

================================================================================
来源：http://neh.gaohongyu789.top

[P01] 生成 UUID
来源：http://hdl.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://oth.yonumen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://khg.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://evv.jinghuilouyu.cn

TS:   crypto.randomUUID()
来源：http://nkm.hongshengwenyu.top

Java: UUID.randomUUID().toString()
来源：http://svv.jqgufenzy.top

Go:   // 用 github.com/google/uuid
来源：http://qdc.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://mrk.chenzaomai.com

C#:   Guid.NewGuid().ToString()
来源：http://vcv.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://jxl.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wjs.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lby.ehwqpu.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qck.jinqigufen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://buj.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yqo.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yyc.cucudq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://loy.sweek.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qqx.wangdashe.top

[P03] 生成短随机字符串
来源：http://jsx.shanyushiyangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bnu.gotoacloud.top


<!-- 参考信息 -->