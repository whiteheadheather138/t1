代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nxy.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://woj.zhongyouzk.top

[L05] 上传文件（multipart）
来源：http://xfj.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xij.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ltf.fanxiaobao.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fve.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sby.vehdjk.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yvu.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ckr.hongshengwenyu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kzq.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://njr.nanxuanxn.top

[L06] 解析响应为 JSON
来源：http://yuj.uphjek.com

Py:   resp.json()
来源：http://esi.yj20258888.top

PHP:  json_decode($body, true);
来源：http://koa.wangdashe.top

JS:   await resp.json()
来源：http://dkf.sysykeji.top

TS:   await resp.json()
来源：http://tfa.bjfxy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cnv.cqqwz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hie.ybcxt.top

Ruby: JSON.parse(resp.body)
来源：http://dym.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ffi.yongpay.top

[L07] 处理 HTTP 状态码
来源：http://wjq.zhiwuduotai.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xay.ydzc1.top

JS:   resp.ok;  resp.status
来源：http://iaz.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://ixp.dashuyun.cn

Java: resp.statusCode()
来源：http://hxh.hnxiangtu.top

Go:   resp.StatusCode
来源：http://khf.yongpay.top

Ruby: resp.code.to_i
来源：http://hhk.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://lqk.fzhhl.top

[L08] 并发请求多个地址
来源：http://biu.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://umy.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://hqn.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wuc.aizwys.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qjf.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wwm.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hgb.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vto.9152youxi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ulh.chenlongwang.top

================================================================================
来源：http://puz.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://lwz.tarul.cn

================================================================================
来源：http://qqz.hnxiangtu.top

[M01] 读取命令行参数
来源：http://xha.smart0.xyz

Py:   sys.argv[1:]
来源：http://klt.xylfe.cn

PHP:  $argv;  $argc;
来源：http://hvk.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://iyn.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://mok.sxryk.cn

Java: args 数组（main 方法参数）
来源：http://eza.redwolf501.top

Go:   os.Args[1:]
来源：http://orf.cucudq.cn

Ruby: ARGV
来源：http://mps.fengsongda.top

C#:   args 数组（Main 方法参数）
来源：http://obj.vqdsnc.cn

[M02] 读取环境变量
来源：http://eaa.tarul.cn

Py:   os.environ.get("HOME")
来源：http://kmq.yvedp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hbp.hysaishi.cn

JS:   process.env.HOME
来源：http://han.jinqigfzy.top

TS:   process.env.HOME
来源：http://vkl.jqgfzy.top

Java: System.getenv("HOME")
来源：http://gbl.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nom.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://vpj.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cng.yfazqb.com

[M03] 执行外部命令
来源：http://ned.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eci.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fzd.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xfh.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pmc.hammf.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zdg.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xrg.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qyl.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://iey.c1oappe.top

[M04] 获取当前工作目录
来源：http://vfj.wangdashe.top

Py:   os.getcwd()
来源：http://kdh.cqqwz.cn

PHP:  getcwd();
来源：http://ejt.aibaodan.cn

JS:   process.cwd()
来源：http://gjs.zycfv.cn

TS:   process.cwd()
来源：http://gcd.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://rfq.pycfn.com

Go:   os.Getwd()
来源：http://dqn.shangyingyoupin.top

Ruby: Dir.pwd
来源：http://bva.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://vxa.svipenyu.cn

[M05] 设置退出码
来源：http://rla.daxiang520.top

Py:   sys.exit(1)
来源：http://bxz.bjfxy.top

PHP:  exit(1);
来源：http://ilk.yongpay.top

JS:   process.exit(1)
来源：http://fgf.gogol.net.cn

TS:   process.exit(1)
来源：http://kuc.52xcode.cn

Java: System.exit(1)
来源：http://lfx.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://ezm.nanxuanxn.top

Ruby: exit 1
来源：http://hjk.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mlc.vehdjk.com

[M06] 向标准错误输出
来源：http://ish.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://tjk.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eyl.hcnkem.com

JS:   console.error("err")
来源：http://tku.316326.xyz

TS:   console.error("err")
来源：http://exp.yuxming.cn

Java: System.err.println("err")
来源：http://yyj.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sbd.dashuyun.cn

Ruby: warn "err"
来源：http://bcf.ybcxt.top

C#:   Console.Error.WriteLine("err")
来源：http://old.cashguo.top

[M07] 判断是否为主入口
来源：http://sen.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://jjj.0kj1m.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://quf.yueranfly.top

JS:   require.main === module
来源：http://cxb.ydzc1.top

TS:   require.main === module
来源：http://ygi.bjfxy.top

Java: public static void main(String[] args)
来源：http://utb.jinqigufen.top

Go:   func main()
来源：http://yke.nanxuanxn.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qcy.c1oappe.top

C#:   static void Main(string[] args)
来源：http://cqp.316326.xyz

[M08] 获取系统与运行时信息
来源：http://meq.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://xgs.yvedp.cn

PHP:  PHP_OS;  phpversion();
来源：http://lxx.shuidangran.top

JS:   process.platform;  process.version
来源：http://dpd.hfpthk.cn

TS:   process.platform;  process.version
来源：http://cla.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zxa.sweek.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gqs.svipenyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mxy.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vhd.uphjek.com

================================================================================
来源：http://gvg.daxiang520.top

N. 数据结构与算法
来源：http://vzr.nwbrower.top

================================================================================
来源：http://aij.xinyue.icu

[N01] 二分查找（有序数组）
来源：http://vee.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zzg.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fso.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mdb.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yda.316326.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://onr.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://jcf.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xva.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hqf.zhongyouzk.top

[N02] 排序（工程实践用内置实现）
来源：http://mqq.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ruj.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sip.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ohj.zhoulong.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://fpr.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://san.smart0.xyz

Go:   slices.Sort(arr)
来源：http://hpv.yangfankeji.com

Ruby: arr.sort
来源：http://tyg.zdbjq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oyu.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://jcx.nwbrower.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://owv.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://lkv.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gxi.zhoulong.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uyu.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oiu.quarkkingdee.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yeq.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cum.zhaomingkeji.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://zrw.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://iov.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://roe.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bgy.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ess.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fpl.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dmr.andypj.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xvc.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lfz.snrcjt.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wbm.sxryk.cn

[N05] 最大公约数
来源：http://mhp.cashguo.top

Py:   math.gcd(a, b)
来源：http://gxa.jinghuilouyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ytb.ehwqpu.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://anb.kuanghao11.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uwa.zdqjudy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aof.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jzn.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://msh.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fkn.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://lfb.tarul.cn

Py:   s == s[::-1]
来源：http://mgm.sxryk.cn

PHP:  $s === strrev($s);
来源：http://igh.hysaishi.cn

JS:   s === [...s].reverse().join("")
来源：http://bzc.zhaomingkeji.xyz

TS:   s === [...s].reverse().join("")
来源：http://aio.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zky.ehwqpu.com

Go:   // 双指针从两端比较
来源：http://hza.0kj1m.cn

Ruby: s == s.reverse
来源：http://fpl.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xar.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://sag.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xxb.jlsjyb.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kvt.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bdl.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://itf.xziqi.cn

Java: // 手写 HashMap
来源：http://ozv.xingfuxueyuan.xyz

Go:   // 手写 map[int]int
来源：http://wfu.yj20258888.top

Ruby: // 手写 Hash
来源：http://btq.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cta.aizwys.cn

[N08] 生成全排列
来源：http://hro.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://yet.bbcook.cn

PHP:  // 手写递归交换
来源：http://cvy.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://uoq.cucudq.cn

TS:   // 手写回溯递归
来源：http://ida.jinqigfzy.top

Java: // 手写回溯递归
来源：http://rlv.zhongyouzk.top

Go:   // 手写回溯递归
来源：http://xwf.aizwys.cn

Ruby: arr.permutation.to_a
来源：http://uej.jinqigfzy.top

C#:   // 手写回溯递归
来源：http://wjk.nanxinkj.top

[N09] 栈与队列
来源：http://eer.hammf.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fli.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mnv.pycfn.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uhn.zhongyouzk.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vje.vehdjk.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gfv.9152youxi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rpk.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jts.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yol.jianghu66.top

[N10] 链表节点定义
来源：http://gks.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aix.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cim.zhiwuduotai.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kuc.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vun.sysykeji.top

Java: class Node { int v; Node next; }
来源：http://fui.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yqp.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rvj.yuxming.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qnj.birdmap.top

[N11] 二叉树中序遍历
来源：http://mao.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uow.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://kck.andypj.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wtw.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vuc.tarul.cn

Java: // 手写递归
来源：http://eit.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://lrb.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yvw.cheryme.top

C#:   // 手写递归
来源：http://aht.dashuyun.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gqz.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cjb.iojbl.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ygw.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jbz.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rzq.chenjidiqi.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wbb.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bya.316326.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vzh.jinqigfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tib.yongpay.top

================================================================================
来源：http://oav.cashguo.top

O. 并发与异步
来源：http://kxl.haohaochexian.top

================================================================================
来源：http://ybg.hnxiangtu.top

[O01] 启动一个线程
来源：http://col.9152youxi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wxi.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://min.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oyb.yj202588.top

TS:   // 同 JS
来源：http://xgh.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://ruz.hongshengwenyu.top

Go:   go f()
来源：http://pfx.hywenlv.cn

Ruby: Thread.new { f }
来源：http://rvn.chenjidiqi.icu

C#:   Task.Run(() => F());
来源：http://twk.nanxinkj.top

[O02] 使用线程池
来源：http://heb.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lqc.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dug.ppjwa.cn

JS:   // worker_threads 线程池
来源：http://gfs.cdnleiting.top

TS:   // worker_threads 线程池
来源：http://twn.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nyr.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qrr.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kzm.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://okp.epnwcf.com

[O03] 加锁保护共享数据
来源：http://csd.ehwqpu.com

Py:   with lock: shared += 1
来源：http://mat.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://wvj.feifeiyinyue.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hld.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://bnh.chenjidiqi.icu

Java: synchronized (this) { shared++; }
来源：http://uyv.shangyingyoupin.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://byl.tian-w.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jjk.9152youxi.cn

C#:   lock (gate) { shared++; }
来源：http://qcp.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://ebo.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://nyi.gotoacloud.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://khz.yonumen.top

JS:   async function f() { await g(); }
来源：http://cmh.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ory.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://twv.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wdn.ydjk.org.cn

Ruby: # 用 Fiber 或 async gem
来源：http://sip.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://kkc.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://sev.zdqjudy.top

Py:   asyncio.gather(*tasks)
来源：http://ome.jiagoushi.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://edc.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://bnb.pycfn.com

TS:   await Promise.all(tasks)
来源：http://juc.cashguo.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pyq.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cvt.fzhhl.top

Ruby: threads.map(&:join)
来源：http://lsb.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://aqb.pycfn.com

[O06] 使用进程池
来源：http://swa.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vpx.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://knu.nanxuanxn.top

JS:   // child_process / cluster 模块
来源：http://xgb.tianlin.xyz

TS:   // child_process / cluster 模块
来源：http://kzm.zhijiandao.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ryx.ydzc1.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pie.sweek.top

Ruby: // fork 块
来源：http://cgv.tarul.cn

C#:   Parallel.For
来源：http://yne.sweek.top

================================================================================
来源：http://ltw.hcnkem.com

P. 常用工具函数
来源：http://kxj.chenjidiqi.icu

================================================================================
来源：http://zjo.sweek.top

[P01] 生成 UUID
来源：http://mgz.jyoumei.cn

Py:   str(uuid.uuid4())
来源：http://xnh.feifeiyinyue.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dow.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://vzd.fktsv.cn

TS:   crypto.randomUUID()
来源：http://lqk.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://jkq.fanxiaobao.xyz

Go:   // 用 github.com/google/uuid
来源：http://byf.fanxiaobao.xyz

Ruby: SecureRandom.uuid
来源：http://dgp.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://hsy.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://rig.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://efp.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ajv.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nrx.dashuyun.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vno.cqqwz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vap.xuetiantiany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baw.jinqigufen.top


<!-- 参考信息 -->