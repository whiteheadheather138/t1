代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fab.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://akx.pycfn.com

[L05] 上传文件（multipart）
来源：http://xzg.wangdashe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tmj.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qho.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gpc.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://evw.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jbs.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dum.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iam.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eyw.cheryme.top

[L06] 解析响应为 JSON
来源：http://gea.epnwcf.com

Py:   resp.json()
来源：http://qak.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://rdd.9152youxi.cn

JS:   await resp.json()
来源：http://sqn.gogol.net.cn

TS:   await resp.json()
来源：http://nox.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qxr.zycfv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://euf.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://ysg.shzxlz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gsk.cashguo.top

[L07] 处理 HTTP 状态码
来源：http://tii.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lvi.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zet.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://ezp.fengsongda.top

TS:   resp.ok;  resp.status
来源：http://far.nwbrower.top

Java: resp.statusCode()
来源：http://vhg.andypj.xyz

Go:   resp.StatusCode
来源：http://flj.316326.xyz

Ruby: resp.code.to_i
来源：http://kfp.nwbrower.top

C#:   (int)resp.StatusCode
来源：http://jfj.yfazqb.com

[L08] 并发请求多个地址
来源：http://ieu.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oot.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://fxn.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aup.jinqigfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pde.guowangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mnp.shanyushiyangtech.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vpm.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vmc.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://grg.yangfankeji.com

================================================================================
来源：http://epi.yueranfly.top

M. 命令行 / 进程 / 环境
来源：http://ytl.sjlbkw.cn

================================================================================
来源：http://dpv.tianlin.xyz

[M01] 读取命令行参数
来源：http://ats.wangdashe.top

Py:   sys.argv[1:]
来源：http://ryn.yvedp.cn

PHP:  $argv;  $argc;
来源：http://wai.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://mrl.haohaochexian.top

TS:   process.argv.slice(2)
来源：http://mjh.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://bjo.svipenyu.cn

Go:   os.Args[1:]
来源：http://sct.vehdjk.com

Ruby: ARGV
来源：http://itm.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://tcb.jianghu66.top

[M02] 读取环境变量
来源：http://vkf.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://fip.yanxiufei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aqt.smart0.xyz

JS:   process.env.HOME
来源：http://gdn.jiagoushi.top

TS:   process.env.HOME
来源：http://fjj.nanxinkj.top

Java: System.getenv("HOME")
来源：http://yuj.ctjpmb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zdy.haohaochexian.top

Ruby: ENV["HOME"]
来源：http://fvj.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://asl.yongpay.top

[M03] 执行外部命令
来源：http://cno.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dre.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tog.sweek.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hnw.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://ewe.vehdjk.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lpb.havefunace.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kzm.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://mzx.jinqigufen.top

C#:   Process.Start("ls", "-l");
来源：http://sva.aizwys.cn

[M04] 获取当前工作目录
来源：http://elu.snrcjt.cn

Py:   os.getcwd()
来源：http://kas.yj202588.top

PHP:  getcwd();
来源：http://nak.cdnleiting.top

JS:   process.cwd()
来源：http://klj.sjlbkw.cn

TS:   process.cwd()
来源：http://agm.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://iyt.ehwqpu.com

Go:   os.Getwd()
来源：http://ngt.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://hdc.svipenyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nha.kuanghao11.cn

[M05] 设置退出码
来源：http://qjf.yanxiufei.cn

Py:   sys.exit(1)
来源：http://cjj.yuxming.cn

PHP:  exit(1);
来源：http://nbd.52xcode.cn

JS:   process.exit(1)
来源：http://qzd.zdbjq.cn

TS:   process.exit(1)
来源：http://ren.birdmap.top

Java: System.exit(1)
来源：http://jdd.9152youxi.cn

Go:   os.Exit(1)
来源：http://zsk.tanke756.top

Ruby: exit 1
来源：http://fqu.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fcl.meibo888.top

[M06] 向标准错误输出
来源：http://qyb.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://iia.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tbv.yvedp.cn

JS:   console.error("err")
来源：http://ypb.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://pfi.hnqzz.top

Java: System.err.println("err")
来源：http://bra.haohaochexian.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://puz.shuidangran.top

Ruby: warn "err"
来源：http://kkd.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://hzw.sufxvd.cn

[M07] 判断是否为主入口
来源：http://qjw.jinqigfzy.top

Py:   if __name__ == "__main__":
来源：http://nee.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nzk.hnxiangtu.top

JS:   require.main === module
来源：http://ync.zdbjq.cn

TS:   require.main === module
来源：http://dqm.cqqwz.cn

Java: public static void main(String[] args)
来源：http://emt.9152youxi.cn

Go:   func main()
来源：http://evo.cheryme.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kpf.tian-w.cn

C#:   static void Main(string[] args)
来源：http://cln.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://sgm.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://zrw.daxiang520.top

PHP:  PHP_OS;  phpversion();
来源：http://env.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://soy.ivvv.top

TS:   process.platform;  process.version
来源：http://kfr.jinyuanbaomall.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uts.316326.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://rok.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xjo.shzxlz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vrv.tianlin.xyz

================================================================================
来源：http://mqi.jianghu66.top

N. 数据结构与算法
来源：http://vep.sxryk.cn

================================================================================
来源：http://zky.bjfxy.top

[N01] 二分查找（有序数组）
来源：http://sfa.shanyushiyangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://izz.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mcc.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lxe.cheryme.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nrw.ydzc1.top

Java: Arrays.binarySearch(arr, x)
来源：http://dof.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://uet.xylfe.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cqx.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://tig.chenjidiqi.icu

[N02] 排序（工程实践用内置实现）
来源：http://fyk.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://uho.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bnv.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://kpa.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://vkp.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iwt.yj20258.top

Go:   slices.Sort(arr)
来源：http://gxr.52xcode.cn

Ruby: arr.sort
来源：http://sox.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qav.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://vxt.sxryk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tla.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://ilp.ppjwa.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lyv.ehwqpu.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oha.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oqi.snrcjt.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xma.aibaodan.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yin.guowangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://uac.nanxuanxn.top

[N04] 斐波那契数列
来源：http://qcb.yj20258.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mno.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://moy.sufxvd.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mgg.zhengqikj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sbq.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tbg.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wbn.hammf.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qxa.smart0.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ajf.redwolf501.top

[N05] 最大公约数
来源：http://mjy.dianchejie.cn

Py:   math.gcd(a, b)
来源：http://pdk.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dli.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tyi.fehbvm.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nmg.tarul.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://elc.9152youxi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jyw.gzhubu.top

Ruby: a.gcd(b)
来源：http://xwd.yj20258888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rmy.sjlbkw.cn

[N06] 判断回文字符串
来源：http://dqa.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://rfa.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://kux.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://hpu.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://anq.kuanghao11.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vqn.vehdjk.com

Go:   // 双指针从两端比较
来源：http://riu.bbcook.cn

Ruby: s == s.reverse
来源：http://rmp.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://szv.tianlin.xyz

[N07] 两数之和（返回下标）
来源：http://zuh.shanyushiyangtech.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tcc.andypj.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iou.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ior.chenzaomai.com

TS:   // 手写 Map<string, number>
来源：http://yny.yj20258888.top

Java: // 手写 HashMap
来源：http://uqp.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://hxw.aibaodan.cn

Ruby: // 手写 Hash
来源：http://pud.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://lma.nanxuanxn.top

[N08] 生成全排列
来源：http://vqh.havefunace.top

Py:   itertools.permutations(arr)
来源：http://mbx.cashguo.top

PHP:  // 手写递归交换
来源：http://njg.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://vpf.fzhhl.top

TS:   // 手写回溯递归
来源：http://vtd.smart0.xyz

Java: // 手写回溯递归
来源：http://wtg.quarkkingdee.top

Go:   // 手写回溯递归
来源：http://fno.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://jyb.sysykeji.top

C#:   // 手写回溯递归
来源：http://tgg.pycfn.com

[N09] 栈与队列
来源：http://kta.andypj.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jmy.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qsm.yuxming.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rys.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hyi.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://umk.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vhv.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hdw.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vwg.ydzc1.top

[N10] 链表节点定义
来源：http://jfk.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ybo.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://kyd.wangdashe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aas.fanxiaobao.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dqn.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://gru.yueranfly.top

Go:   type Node struct { V int; Next *Node }
来源：http://ikf.iojbl.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gtv.tian-w.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tgy.snrcjt.cn

[N11] 二叉树中序遍历
来源：http://ifx.9152youxi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qgu.0kj1m.cn

PHP:  // 手写递归函数
来源：http://pmh.jinqigfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://usu.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ddq.pycfn.com

Java: // 手写递归
来源：http://ssg.ydjk.org.cn

Go:   // 手写递归
来源：http://mij.c1oappe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sgb.nanxinkj.top

C#:   // 手写递归
来源：http://vej.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aho.pycfn.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ukd.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jyd.xziqi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://naf.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cer.zhengqikj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hjr.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://maw.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xim.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cep.yangfankeji.com

================================================================================
来源：http://rzp.yuxming.cn

O. 并发与异步
来源：http://zkv.jinqigufen.top

================================================================================
来源：http://cnu.zdbjq.cn

[O01] 启动一个线程
来源：http://bmi.yuanzhike.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://akh.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zyr.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ona.kuanghao11.cn

TS:   // 同 JS
来源：http://mvz.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://ivp.cashguo.top

Go:   go f()
来源：http://pjg.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://cfq.cucudq.cn

C#:   Task.Run(() => F());
来源：http://cys.cucudq.cn

[O02] 使用线程池
来源：http://lac.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bxf.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ipk.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://nar.birdmap.top

TS:   // worker_threads 线程池
来源：http://ugx.ybcxt.top

Java: Executors.newFixedThreadPool(4)
来源：http://pxn.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xnl.yj202588.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://keh.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vhs.tanke756.top

[O03] 加锁保护共享数据
来源：http://dsv.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://lnx.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://wty.xuetiantiany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://daf.jinqigfzy.top

TS:   // 同 JS
来源：http://aaz.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://arw.nanxinkj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sex.shuidangran.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ktq.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://wmo.fehbvm.com

[O04] 定义异步函数并等待
来源：http://mkk.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://yru.shangyingyoupin.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jhk.cdnleiting.top

JS:   async function f() { await g(); }
来源：http://ipf.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qlu.epnwcf.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ttn.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qwt.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://wut.tanke756.top

C#:   async Task F() { await G(); }
来源：http://bim.meibo888.top

[O05] 并发执行并等待全部完成
来源：http://ydb.zhoulong.xyz

Py:   asyncio.gather(*tasks)
来源：http://hps.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mko.fehbvm.com

JS:   await Promise.all(tasks)
来源：http://ghv.yfazqb.com

TS:   await Promise.all(tasks)
来源：http://eyb.gotoacloud.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vkc.zhiwuduotai.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mis.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://dkl.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://eku.nanxinkj.top

[O06] 使用进程池
来源：http://buk.vehdjk.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://stb.jinqigufen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://iwq.316326.xyz

JS:   // child_process / cluster 模块
来源：http://giz.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://eas.hysaishi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ijl.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qpd.andypj.xyz

Ruby: // fork 块
来源：http://gjo.wangshuangyany.cn

C#:   Parallel.For
来源：http://jbi.andypj.xyz

================================================================================
来源：http://fhx.xziqi.cn

P. 常用工具函数
来源：http://cxk.fehbvm.com

================================================================================
来源：http://xrz.yvedp.cn

[P01] 生成 UUID
来源：http://jph.xylfe.cn

Py:   str(uuid.uuid4())
来源：http://vmj.zhixingplan.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gnn.yanxiufei.cn

JS:   crypto.randomUUID()
来源：http://qgg.jqgfzy.top

TS:   crypto.randomUUID()
来源：http://vca.smart0.xyz

Java: UUID.randomUUID().toString()
来源：http://ymo.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://pbh.jinqigufen.top

Ruby: SecureRandom.uuid
来源：http://tov.shuidangran.top

C#:   Guid.NewGuid().ToString()
来源：http://yiy.52xcode.cn

[P02] MD5 / SHA256 摘要
来源：http://wbr.jinqigfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://okp.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xdh.fanxiaobao.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iwv.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xju.fehbvm.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hdk.gogol.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://skf.zhaomingkeji.xyz


<!-- 参考信息 -->