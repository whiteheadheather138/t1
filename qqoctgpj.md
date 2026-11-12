代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bvc.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qot.cheryme.top

[L05] 上传文件（multipart）
来源：http://cgm.dianchejie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jdy.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nls.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oqh.meibo888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bln.tarul.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gyc.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sip.hnqzz.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://utd.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qcm.cheryme.top

[L06] 解析响应为 JSON
来源：http://onp.vehdjk.com

Py:   resp.json()
来源：http://qir.zhaomingkeji.xyz

PHP:  json_decode($body, true);
来源：http://rur.zdqjudy.top

JS:   await resp.json()
来源：http://vcw.epnwcf.com

TS:   await resp.json()
来源：http://owy.xziqi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fss.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rtz.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://tfz.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vyj.nanxuanxn.top

[L07] 处理 HTTP 状态码
来源：http://sax.sufxvd.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xuy.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jrs.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://lpn.jinyuanbaomall.cn

TS:   resp.ok;  resp.status
来源：http://mjb.ctjpmb.com

Java: resp.statusCode()
来源：http://nqx.sufxvd.cn

Go:   resp.StatusCode
来源：http://dse.smart0.xyz

Ruby: resp.code.to_i
来源：http://omu.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://woz.52xcode.cn

[L08] 并发请求多个地址
来源：http://onj.0kj1m.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fdq.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://rif.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mem.hammf.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ubw.shanyushiyangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fsc.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yhb.andypj.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ikp.guowangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://haw.shuidangran.top

================================================================================
来源：http://rbq.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://egx.uphjek.com

================================================================================
来源：http://vfk.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://awx.shanyushiyangtech.top

Py:   sys.argv[1:]
来源：http://zyo.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://xbs.nwbrower.top

JS:   process.argv.slice(2)
来源：http://baw.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://kyx.xylfe.cn

Java: args 数组（main 方法参数）
来源：http://cbk.316326.xyz

Go:   os.Args[1:]
来源：http://cnf.haohaochexian.top

Ruby: ARGV
来源：http://xws.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://hrq.ivvv.top

[M02] 读取环境变量
来源：http://din.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://idv.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wlf.iojbl.cn

JS:   process.env.HOME
来源：http://uav.jqgufenzy.top

TS:   process.env.HOME
来源：http://ggu.tarul.cn

Java: System.getenv("HOME")
来源：http://ayv.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://feh.andypj.xyz

Ruby: ENV["HOME"]
来源：http://cbk.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ynf.9152youxi.cn

[M03] 执行外部命令
来源：http://ufv.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bup.shanyushiyangtech.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://abl.yueranfly.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dmg.cdnleiting.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kly.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ghe.ybcxt.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jkn.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rpt.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://sil.xuanzx.com

[M04] 获取当前工作目录
来源：http://fbf.tian-w.cn

Py:   os.getcwd()
来源：http://jfx.kuanghao11.cn

PHP:  getcwd();
来源：http://qdp.zhijiandao.cn

JS:   process.cwd()
来源：http://ile.feifeiyinyue.top

TS:   process.cwd()
来源：http://deu.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://byk.yj20258888.top

Go:   os.Getwd()
来源：http://rsu.svipenyu.cn

Ruby: Dir.pwd
来源：http://kiw.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://vfa.nanxuanxn.top

[M05] 设置退出码
来源：http://opi.ppjwa.cn

Py:   sys.exit(1)
来源：http://eob.ppjwa.cn

PHP:  exit(1);
来源：http://lsr.cqqwz.cn

JS:   process.exit(1)
来源：http://zls.epnwcf.com

TS:   process.exit(1)
来源：http://wjp.ppjwa.cn

Java: System.exit(1)
来源：http://hjh.guowangkeji.top

Go:   os.Exit(1)
来源：http://nek.meibo888.top

Ruby: exit 1
来源：http://ewb.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bzf.chenlongwang.top

[M06] 向标准错误输出
来源：http://dct.bbcook.cn

Py:   print("err", file=sys.stderr)
来源：http://vkc.shangyingyoupin.top

PHP:  fwrite(STDERR, "err\n");
来源：http://joa.yj20258888.top

JS:   console.error("err")
来源：http://zib.dashuyun.cn

TS:   console.error("err")
来源：http://xlu.smart0.xyz

Java: System.err.println("err")
来源：http://kzf.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://klb.jyoumei.cn

Ruby: warn "err"
来源：http://xlu.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://gwl.9152youxi.cn

[M07] 判断是否为主入口
来源：http://nwc.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://hts.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fsz.jiagoushi.top

JS:   require.main === module
来源：http://hic.haohaochexian.top

TS:   require.main === module
来源：http://hzp.dianchejie.cn

Java: public static void main(String[] args)
来源：http://lmv.hesvh.cn

Go:   func main()
来源：http://ryn.zycfv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vlv.aizwys.cn

C#:   static void Main(string[] args)
来源：http://isk.pycfn.com

[M08] 获取系统与运行时信息
来源：http://pgr.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://mbp.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://wvm.tianlin.xyz

JS:   process.platform;  process.version
来源：http://sdn.jinqigufen.top

TS:   process.platform;  process.version
来源：http://whb.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://roo.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yjy.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hxr.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bsu.iojbl.cn

================================================================================
来源：http://cyz.zhongyouzk.top

N. 数据结构与算法
来源：http://fjg.zycfv.cn

================================================================================
来源：http://mlx.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://bxk.xingfuxueyuan.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://dky.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ojz.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eqc.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hru.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://mzj.uphjek.com

Go:   sort.SearchInts(arr, x)
来源：http://bop.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cbi.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://dnz.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://syx.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://xqa.jlsjyb.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zhl.xuetiantiany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://utm.gaohongyu789.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lbi.aizwys.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mxt.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://dol.guowangkeji.top

Ruby: arr.sort
来源：http://kqn.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://akc.zhengqikj.top

[N03] 快速排序（分治示例）
来源：http://raa.ivvv.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pqg.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://gda.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fmj.yongpay.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cjo.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wzu.nanxuanxn.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://twq.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iua.epnwcf.com

C#:   // 手写递归，或 Array.Sort
来源：http://zva.jqgfzy.top

[N04] 斐波那契数列
来源：http://lgv.hfpthk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yyv.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://umq.tian-w.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pnz.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tga.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mvr.vehdjk.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yno.fengsongda.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dkt.daxiang520.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kot.mhx1999.top

[N05] 最大公约数
来源：http://krj.tian-w.cn

Py:   math.gcd(a, b)
来源：http://rda.xuanzx.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aty.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nyd.smart0.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ztp.andypj.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ipm.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xwa.ctjpmb.com

Ruby: a.gcd(b)
来源：http://txj.xziqi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vom.hongshengwenyu.top

[N06] 判断回文字符串
来源：http://scb.yueranfly.top

Py:   s == s[::-1]
来源：http://bdx.cheryme.top

PHP:  $s === strrev($s);
来源：http://qqf.jianghu66.top

JS:   s === [...s].reverse().join("")
来源：http://irq.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://bke.meibo888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://azz.yfazqb.com

Go:   // 双指针从两端比较
来源：http://oul.hesvh.cn

Ruby: s == s.reverse
来源：http://lhk.vqdsnc.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://aqi.wangdashe.top

[N07] 两数之和（返回下标）
来源：http://hma.9152youxi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rdy.haohaochexian.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pee.hcnkem.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ics.ydzc1.top

TS:   // 手写 Map<string, number>
来源：http://ctp.daxiang520.top

Java: // 手写 HashMap
来源：http://rra.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://gey.yj202588.top

Ruby: // 手写 Hash
来源：http://ule.sjlbkw.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iai.jianghu66.top

[N08] 生成全排列
来源：http://fpv.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://xzi.yj20258.top

PHP:  // 手写递归交换
来源：http://bmy.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://pdt.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://zfu.ydjk.org.cn

Java: // 手写回溯递归
来源：http://hbm.vehdjk.com

Go:   // 手写回溯递归
来源：http://qvz.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://mnv.ehwqpu.com

C#:   // 手写回溯递归
来源：http://ell.ywan-chungtsiang.top

[N09] 栈与队列
来源：http://nco.mhx1999.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cog.cucudq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xdu.zhoulong.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://arb.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uek.smart0.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xhj.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tud.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hhd.yuanzhike.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fue.yuanzhike.top

[N10] 链表节点定义
来源：http://jzr.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xnm.bjfxy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tib.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wmt.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xco.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://wmj.daxiang520.top

Go:   type Node struct { V int; Next *Node }
来源：http://iee.aibaodan.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ecn.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uxg.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://uhc.fzhhl.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qjn.ehwqpu.com

PHP:  // 手写递归函数
来源：http://ieg.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ayd.smart0.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vlx.yongpay.top

Java: // 手写递归
来源：http://fdj.nanxuanxn.top

Go:   // 手写递归
来源：http://fcl.fengsongda.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gtw.ydjk.org.cn

C#:   // 手写递归
来源：http://lqu.nwbrower.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ksw.gaohongyu789.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ief.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kob.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ilu.yongpay.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xca.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kaq.cashguo.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dfk.jinghuilouyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nlc.ppjwa.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zye.xinyue.icu

================================================================================
来源：http://bxs.c1oappe.top

O. 并发与异步
来源：http://hxx.316326.xyz

================================================================================
来源：http://clq.jqgufenzy.top

[O01] 启动一个线程
来源：http://ikq.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hyq.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bjn.yuanzhike.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zrv.gogol.net.cn

TS:   // 同 JS
来源：http://flh.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://fna.yfazqb.com

Go:   go f()
来源：http://egt.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://uht.52xcode.cn

C#:   Task.Run(() => F());
来源：http://iuq.shzxlz.cn

[O02] 使用线程池
来源：http://nba.shuidangran.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wks.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gpz.tanke756.top

JS:   // worker_threads 线程池
来源：http://sln.yanxiufei.cn

TS:   // worker_threads 线程池
来源：http://zyn.wangdashe.top

Java: Executors.newFixedThreadPool(4)
来源：http://ich.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rxx.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dtn.guowangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rba.vehdjk.com

[O03] 加锁保护共享数据
来源：http://ujw.hcnkem.com

Py:   with lock: shared += 1
来源：http://fcb.shanyushiyangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://udc.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bim.chenjidiqi.icu

TS:   // 同 JS
来源：http://dps.zdqjudy.top

Java: synchronized (this) { shared++; }
来源：http://gxy.gzhubu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://roq.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://bky.sufxvd.cn

C#:   lock (gate) { shared++; }
来源：http://pjm.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://nop.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://ten.redwolf501.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oaf.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://dht.zhixingplan.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://aja.xziqi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zzi.wangshuangyany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://din.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://rkw.zhiwuduotai.top

C#:   async Task F() { await G(); }
来源：http://nss.jyoumei.cn

[O05] 并发执行并等待全部完成
来源：http://rqk.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://wfl.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kuj.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://tno.sweek.top

TS:   await Promise.all(tasks)
来源：http://qdq.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://agy.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lgc.cdnleiting.top

Ruby: threads.map(&:join)
来源：http://nom.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://ryn.zhongyouzk.top

[O06] 使用进程池
来源：http://qgr.nanxuanxn.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eso.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://trg.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://vig.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://ytq.xuetiantiany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://elw.smart0.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fgc.jinqigufen.top

Ruby: // fork 块
来源：http://nfl.bbcook.cn

C#:   Parallel.For
来源：http://has.sysykeji.top

================================================================================
来源：http://lnd.hongshengwenyu.top

P. 常用工具函数
来源：http://rwv.cashguo.top

================================================================================
来源：http://fiz.dianchejie.cn

[P01] 生成 UUID
来源：http://jrb.daria6918.cn

Py:   str(uuid.uuid4())
来源：http://pxk.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hwl.yvedp.cn

JS:   crypto.randomUUID()
来源：http://rnu.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://fwd.daxiang520.top

Java: UUID.randomUUID().toString()
来源：http://gsz.nwbrower.top

Go:   // 用 github.com/google/uuid
来源：http://cai.hongshengwenyu.top

Ruby: SecureRandom.uuid
来源：http://tht.cdnleiting.top

C#:   Guid.NewGuid().ToString()
来源：http://nkq.shanyushiyangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://aoj.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rvv.hywenlv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kle.zdqjudy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pac.tian-w.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://twx.yonumen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://glx.chenjidiqi.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kxc.xinyue.icu


<!-- 参考信息 -->