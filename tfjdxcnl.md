代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mpg.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cvv.shuidangran.top

[L05] 上传文件（multipart）
来源：http://yaf.nwbrower.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nvd.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://svv.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rkh.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tfl.snrcjt.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kkx.yj202588.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zpb.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wqr.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jht.nanxuanxn.top

[L06] 解析响应为 JSON
来源：http://xnu.wangdashe.top

Py:   resp.json()
来源：http://rep.fengsongda.top

PHP:  json_decode($body, true);
来源：http://dir.chenzaomai.com

JS:   await resp.json()
来源：http://oye.shuidangran.top

TS:   await resp.json()
来源：http://idj.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zxf.andypj.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nyz.sysykeji.top

Ruby: JSON.parse(resp.body)
来源：http://rku.cucudq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xqq.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://uum.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vxi.ehwqpu.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jbt.iojbl.cn

JS:   resp.ok;  resp.status
来源：http://hxw.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://tnl.ctjpmb.com

Java: resp.statusCode()
来源：http://zjc.dianchejie.cn

Go:   resp.StatusCode
来源：http://fyk.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://aen.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://ddy.fktsv.cn

[L08] 并发请求多个地址
来源：http://chn.sxryk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uug.ppjwa.cn

PHP:  curl_multi_init() 系列
来源：http://jev.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zsy.fktsv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://unm.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yvj.ppjwa.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ukw.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fos.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cko.fanxiaobao.xyz

================================================================================
来源：http://jjs.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://cng.ctjpmb.com

================================================================================
来源：http://bfn.jinqigfzy.top

[M01] 读取命令行参数
来源：http://jrq.jinqigufen.top

Py:   sys.argv[1:]
来源：http://amg.ivvv.top

PHP:  $argv;  $argc;
来源：http://ciw.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://btr.wangdashe.top

TS:   process.argv.slice(2)
来源：http://qlb.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://sgu.andypj.xyz

Go:   os.Args[1:]
来源：http://hfj.jinyuanbaomall.cn

Ruby: ARGV
来源：http://agm.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://ufo.snrcjt.cn

[M02] 读取环境变量
来源：http://snp.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://prh.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vvk.jqgufenzy.top

JS:   process.env.HOME
来源：http://urf.vehdjk.com

TS:   process.env.HOME
来源：http://blf.c1oappe.top

Java: System.getenv("HOME")
来源：http://vee.jyoumei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wdh.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://wev.tian-w.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://psg.feifeiyinyue.top

[M03] 执行外部命令
来源：http://lus.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xfz.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qrd.yuxming.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qzj.jlsjyb.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oru.jyoumei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mri.ydjk.org.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://snh.yj20258.top

Ruby: system("ls -l");  `ls -l`
来源：http://oxw.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://hqz.zycfv.cn

[M04] 获取当前工作目录
来源：http://hgg.birdmap.top

Py:   os.getcwd()
来源：http://lft.316326.xyz

PHP:  getcwd();
来源：http://wli.hnqzz.top

JS:   process.cwd()
来源：http://mjy.chenlongwang.top

TS:   process.cwd()
来源：http://tvp.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://kpl.bjfxy.top

Go:   os.Getwd()
来源：http://wlu.c1oappe.top

Ruby: Dir.pwd
来源：http://khz.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://wwp.vqdsnc.cn

[M05] 设置退出码
来源：http://ztr.fktsv.cn

Py:   sys.exit(1)
来源：http://ibo.ydjk.org.cn

PHP:  exit(1);
来源：http://gml.ydzc1.top

JS:   process.exit(1)
来源：http://ole.jinqigufen.top

TS:   process.exit(1)
来源：http://yue.vqdsnc.cn

Java: System.exit(1)
来源：http://qvm.jinyuanbaomall.cn

Go:   os.Exit(1)
来源：http://rps.hywenlv.cn

Ruby: exit 1
来源：http://nof.hnxiangtu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pvr.ywan-chungtsiang.top

[M06] 向标准错误输出
来源：http://rzh.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://cnl.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nfj.xziqi.cn

JS:   console.error("err")
来源：http://hgu.sweek.top

TS:   console.error("err")
来源：http://lza.52xcode.cn

Java: System.err.println("err")
来源：http://npl.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hsd.hesvh.cn

Ruby: warn "err"
来源：http://sww.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://qci.uphjek.com

[M07] 判断是否为主入口
来源：http://fjl.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://fwq.shangyingyoupin.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xak.yj20258888.top

JS:   require.main === module
来源：http://wmb.andypj.xyz

TS:   require.main === module
来源：http://qgz.gzhubu.top

Java: public static void main(String[] args)
来源：http://mng.feifeiyinyue.top

Go:   func main()
来源：http://ryr.havefunace.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sjg.hnqzz.top

C#:   static void Main(string[] args)
来源：http://ron.fanxiaobao.xyz

[M08] 获取系统与运行时信息
来源：http://crp.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://zdm.c1oappe.top

PHP:  PHP_OS;  phpversion();
来源：http://fqc.yuxming.cn

JS:   process.platform;  process.version
来源：http://bke.dianchejie.cn

TS:   process.platform;  process.version
来源：http://xmo.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gno.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ouo.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://chk.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://crk.pengpengdd.cyou

================================================================================
来源：http://wuc.iojbl.cn

N. 数据结构与算法
来源：http://fin.yj202588.top

================================================================================
来源：http://bco.fktsv.cn

[N01] 二分查找（有序数组）
来源：http://ucq.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wgq.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xis.yj20258888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://itg.jinyuanbaomall.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cks.chenlongwang.top

Java: Arrays.binarySearch(arr, x)
来源：http://qlm.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://osh.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hrb.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://lxc.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://mit.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://fom.zhaomingkeji.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jch.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wvb.bbcook.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://brz.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ylx.redwolf501.top

Go:   slices.Sort(arr)
来源：http://mds.zhijiandao.cn

Ruby: arr.sort
来源：http://rfm.zdbjq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://alp.pycfn.com

[N03] 快速排序（分治示例）
来源：http://hof.pycfn.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tyj.ivvv.top

PHP:  // 递归实现，或用 usort
来源：http://mmd.sysykeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gft.9152youxi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://myh.gogol.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://url.ydzc1.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uaf.xingfuxueyuan.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iym.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://jrn.xylfe.cn

[N04] 斐波那契数列
来源：http://hpi.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wps.jyoumei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kex.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fui.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vhx.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://drk.fzhhl.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lnr.hnxiangtu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rrb.aibaodan.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://btj.hfpthk.cn

[N05] 最大公约数
来源：http://awu.iojbl.cn

Py:   math.gcd(a, b)
来源：http://baj.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lhy.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aku.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tpr.nwbrower.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jnz.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sxl.tarul.cn

Ruby: a.gcd(b)
来源：http://ymy.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://whk.zdqjudy.top

[N06] 判断回文字符串
来源：http://ebk.cashguo.top

Py:   s == s[::-1]
来源：http://pts.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://hna.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://tik.shanyushiyangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://okc.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rrg.yonumen.top

Go:   // 双指针从两端比较
来源：http://zhj.svipenyu.cn

Ruby: s == s.reverse
来源：http://yst.hnqzz.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lyq.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://wns.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://smg.snrcjt.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lez.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://sjs.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://jas.birdmap.top

Java: // 手写 HashMap
来源：http://sws.yvedp.cn

Go:   // 手写 map[int]int
来源：http://hwj.zdbjq.cn

Ruby: // 手写 Hash
来源：http://qdv.svipenyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cja.snrcjt.cn

[N08] 生成全排列
来源：http://yup.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://cxm.chenjidiqi.icu

PHP:  // 手写递归交换
来源：http://eqx.sweek.top

JS:   // 手写回溯递归
来源：http://yus.guannengcc.top

TS:   // 手写回溯递归
来源：http://ekn.meibo888.top

Java: // 手写回溯递归
来源：http://ytw.fzhhl.top

Go:   // 手写回溯递归
来源：http://tpy.cdnleiting.top

Ruby: arr.permutation.to_a
来源：http://kti.zycfv.cn

C#:   // 手写回溯递归
来源：http://mqm.quarkkingdee.top

[N09] 栈与队列
来源：http://jqi.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jmb.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ocn.havefunace.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lts.sjlbkw.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zao.pycfn.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lox.tianlin.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ogz.birdmap.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rkz.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wum.vehdjk.com

[N10] 链表节点定义
来源：http://nyf.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ftg.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vfm.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wtu.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://puv.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://yrz.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rkn.cdnleiting.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ikt.smart0.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://aac.yueranfly.top

[N11] 二叉树中序遍历
来源：http://rtt.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oax.andypj.xyz

PHP:  // 手写递归函数
来源：http://jwb.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dll.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mlx.xuetiantiany.cn

Java: // 手写递归
来源：http://oip.xuanzx.com

Go:   // 手写递归
来源：http://yky.cucudq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vpt.yvedp.cn

C#:   // 手写递归
来源：http://zwj.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lqo.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sse.andypj.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sph.pengpengdd.cyou

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vrt.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xsh.hysaishi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mgu.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://arj.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://azp.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://llo.aibaodan.cn

================================================================================
来源：http://fqb.uphjek.com

O. 并发与异步
来源：http://iuc.sxryk.cn

================================================================================
来源：http://qdj.sjlbkw.cn

[O01] 启动一个线程
来源：http://kmj.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gax.nwbrower.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xtq.tanke756.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tmi.ehwqpu.com

TS:   // 同 JS
来源：http://xfp.hywenlv.cn

Java: new Thread(() -> f()).start()
来源：http://ydm.bjfxy.top

Go:   go f()
来源：http://tht.yanxiufei.cn

Ruby: Thread.new { f }
来源：http://nwv.gzhubu.top

C#:   Task.Run(() => F());
来源：http://rra.daxiang520.top

[O02] 使用线程池
来源：http://bhm.daxiang520.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ins.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dqt.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://mig.tarul.cn

TS:   // worker_threads 线程池
来源：http://oss.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://nqy.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://trf.jqgfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ius.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wwr.sweek.top

[O03] 加锁保护共享数据
来源：http://abg.shuidangran.top

Py:   with lock: shared += 1
来源：http://ift.52xcode.cn

PHP:  // 用 flock() 做文件锁
来源：http://uuu.wangshuangyany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zvz.pycfn.com

TS:   // 同 JS
来源：http://orb.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://zmx.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pcq.yj20258888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qtx.yj202588.top

C#:   lock (gate) { shared++; }
来源：http://ffs.xylfe.cn

[O04] 定义异步函数并等待
来源：http://dhn.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://nuz.iojbl.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://biw.nwbrower.top

JS:   async function f() { await g(); }
来源：http://xvq.nanxuanxn.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tmj.yj20258.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oyz.ivvv.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eol.smart0.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://hyi.cashguo.top

C#:   async Task F() { await G(); }
来源：http://dvu.0kj1m.cn

[O05] 并发执行并等待全部完成
来源：http://rws.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://uzb.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sxy.fanxiaobao.xyz

JS:   await Promise.all(tasks)
来源：http://poq.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://hkj.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zvp.gotoacloud.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xvo.ywan-chungtsiang.top

Ruby: threads.map(&:join)
来源：http://tnc.shanyushiyangtech.top

C#:   await Task.WhenAll(t1, t2)
来源：http://myc.yueranfly.top

[O06] 使用进程池
来源：http://xyn.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ypt.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://him.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://ozl.yj20258.top

TS:   // child_process / cluster 模块
来源：http://ovz.guannengcc.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cwu.shzxlz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vqr.xuanzx.com

Ruby: // fork 块
来源：http://jfe.zhiwuduotai.top

C#:   Parallel.For
来源：http://cpm.wangdashe.top

================================================================================
来源：http://dhx.tarul.cn

P. 常用工具函数
来源：http://toi.gotoacloud.top

================================================================================
来源：http://tgk.zycfv.cn

[P01] 生成 UUID
来源：http://ilh.chenlongwang.top

Py:   str(uuid.uuid4())
来源：http://yqz.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ctn.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://uex.ydjk.org.cn

TS:   crypto.randomUUID()
来源：http://kdb.xingfuxueyuan.xyz

Java: UUID.randomUUID().toString()
来源：http://iyf.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://ykc.iojbl.cn

Ruby: SecureRandom.uuid
来源：http://ume.9152youxi.cn

C#:   Guid.NewGuid().ToString()
来源：http://ucw.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://wgc.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hnh.0kj1m.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xrq.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kyu.vqdsnc.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hdv.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hmk.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://edv.jyoumei.cn


<!-- 参考信息 -->