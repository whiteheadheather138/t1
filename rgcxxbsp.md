代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wlf.jiagoushi.top

[L04] 设置超时
来源：http://knr.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://eoe.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rfn.xziqi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uuy.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vzn.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://efd.hnqzz.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eoh.tian-w.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://reb.cucudq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rix.sufxvd.cn

[L05] 上传文件（multipart）
来源：http://qgt.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tlo.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ymq.ybcxt.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ecr.ybcxt.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rga.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://euf.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fwi.yfazqb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sct.kuanghao11.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://viy.cdnleiting.top

[L06] 解析响应为 JSON
来源：http://crt.birdmap.top

Py:   resp.json()
来源：http://avv.yuanzhike.top

PHP:  json_decode($body, true);
来源：http://mqd.hammf.cn

JS:   await resp.json()
来源：http://jip.uphjek.com

TS:   await resp.json()
来源：http://yrd.hfpthk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://acv.chenlongwang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iwz.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://juh.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pck.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://gyh.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rgn.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://onb.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://try.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://nov.xinyue.icu

Java: resp.statusCode()
来源：http://wot.tarul.cn

Go:   resp.StatusCode
来源：http://vss.yvedp.cn

Ruby: resp.code.to_i
来源：http://kxg.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://xjk.snrcjt.cn

[L08] 并发请求多个地址
来源：http://efj.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zux.chenlongwang.top

PHP:  curl_multi_init() 系列
来源：http://klf.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lys.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cun.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hjj.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mxe.hnqzz.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zyx.jinqigfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://grq.daxiang520.top

================================================================================
来源：http://vmy.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://orn.gaohongyu789.top

================================================================================
来源：http://xxx.hongshengwenyu.top

[M01] 读取命令行参数
来源：http://xtt.zhixingplan.top

Py:   sys.argv[1:]
来源：http://blg.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://jfu.ppjwa.cn

JS:   process.argv.slice(2)
来源：http://yea.andypj.xyz

TS:   process.argv.slice(2)
来源：http://bmr.xingfuxueyuan.xyz

Java: args 数组（main 方法参数）
来源：http://zus.zhongyouzk.top

Go:   os.Args[1:]
来源：http://xfs.pengpengdd.cyou

Ruby: ARGV
来源：http://aod.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://bwq.shanyushiyangkeji.top

[M02] 读取环境变量
来源：http://rvr.iojbl.cn

Py:   os.environ.get("HOME")
来源：http://dln.gaohongyu789.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kmh.sjlbkw.cn

JS:   process.env.HOME
来源：http://hno.ehwqpu.com

TS:   process.env.HOME
来源：http://pug.yvedp.cn

Java: System.getenv("HOME")
来源：http://zxa.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zdg.pengpengdd.cyou

Ruby: ENV["HOME"]
来源：http://dzk.yanxiufei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hdf.tian-w.cn

[M03] 执行外部命令
来源：http://sfh.aizwys.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hlm.cucudq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://stz.wangdashe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fls.hysaishi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zht.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mwh.jianghu66.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rzn.zdqjudy.top

Ruby: system("ls -l");  `ls -l`
来源：http://yue.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://cro.nwbrower.top

[M04] 获取当前工作目录
来源：http://aji.zhoulong.xyz

Py:   os.getcwd()
来源：http://ldr.mhx1999.top

PHP:  getcwd();
来源：http://onp.yangfankeji.com

JS:   process.cwd()
来源：http://lhy.tian-w.cn

TS:   process.cwd()
来源：http://qgl.cdnleiting.top

Java: Path.of("").toAbsolutePath()
来源：http://mgh.aizwys.cn

Go:   os.Getwd()
来源：http://eie.shuidangran.top

Ruby: Dir.pwd
来源：http://xjp.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://fgl.tianlin.xyz

[M05] 设置退出码
来源：http://xnx.jlsjyb.cn

Py:   sys.exit(1)
来源：http://lev.yj20258888.top

PHP:  exit(1);
来源：http://gaf.chenlongwang.top

JS:   process.exit(1)
来源：http://jop.bjfxy.top

TS:   process.exit(1)
来源：http://zbz.pycfn.com

Java: System.exit(1)
来源：http://mla.hongshengwenyu.top

Go:   os.Exit(1)
来源：http://val.epnwcf.com

Ruby: exit 1
来源：http://akd.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tqv.tarul.cn

[M06] 向标准错误输出
来源：http://dgu.hongshengwenyu.top

Py:   print("err", file=sys.stderr)
来源：http://kvq.jianghu66.top

PHP:  fwrite(STDERR, "err\n");
来源：http://okq.jinqigufen.top

JS:   console.error("err")
来源：http://lau.nanxinkj.top

TS:   console.error("err")
来源：http://nfy.zdqjudy.top

Java: System.err.println("err")
来源：http://uvc.meibo888.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pzy.havefunace.top

Ruby: warn "err"
来源：http://rtq.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://hod.c1oappe.top

[M07] 判断是否为主入口
来源：http://ogq.hysaishi.cn

Py:   if __name__ == "__main__":
来源：http://nfg.yfazqb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gti.aibaodan.cn

JS:   require.main === module
来源：http://vbx.guowangkeji.top

TS:   require.main === module
来源：http://ocv.xuanzx.com

Java: public static void main(String[] args)
来源：http://lsf.shangyingyoupin.top

Go:   func main()
来源：http://jjv.hongshengwenyu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zee.tarul.cn

C#:   static void Main(string[] args)
来源：http://rjs.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://pxc.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://mti.wangdashe.top

PHP:  PHP_OS;  phpversion();
来源：http://kvs.zycfv.cn

JS:   process.platform;  process.version
来源：http://fmw.fengsongda.top

TS:   process.platform;  process.version
来源：http://unh.yonumen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nwt.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ukz.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://glt.xylfe.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tev.kuanghao11.cn

================================================================================
来源：http://exa.nanxuanxn.top

N. 数据结构与算法
来源：http://ohn.cucudq.cn

================================================================================
来源：http://oxq.316326.xyz

[N01] 二分查找（有序数组）
来源：http://iul.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sej.xziqi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jmv.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ehv.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gwm.feifeiyinyue.top

Java: Arrays.binarySearch(arr, x)
来源：http://hpb.cdnleiting.top

Go:   sort.SearchInts(arr, x)
来源：http://isw.cheryme.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qem.cucudq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://scq.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://dem.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://tih.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vah.epnwcf.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://vwl.vehdjk.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://szp.yongpay.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://twh.tarul.cn

Go:   slices.Sort(arr)
来源：http://jgp.jyoumei.cn

Ruby: arr.sort
来源：http://fpm.bjfxy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qrc.quarkkingdee.top

[N03] 快速排序（分治示例）
来源：http://urn.pycfn.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://may.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://wdg.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wfy.sxryk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ebv.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hdp.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jeq.gaohongyu789.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jjh.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uob.chenzaomai.com

[N04] 斐波那契数列
来源：http://cer.yvedp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dgr.feifeiyinyue.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kap.cheryme.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zzl.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hqd.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vfi.yanxiufei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tvn.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jli.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cwd.yvedp.cn

[N05] 最大公约数
来源：http://wuh.yueranfly.top

Py:   math.gcd(a, b)
来源：http://wuw.shangyingyoupin.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://csz.shzxlz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wbb.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kcf.fehbvm.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yxg.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rvq.zdbjq.cn

Ruby: a.gcd(b)
来源：http://qtm.bbcook.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aio.ydzc1.top

[N06] 判断回文字符串
来源：http://uxz.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://ufi.zdqjudy.top

PHP:  $s === strrev($s);
来源：http://tzc.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://gtd.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://wrz.chenzaomai.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://akr.ydjk.org.cn

Go:   // 双指针从两端比较
来源：http://thb.cdnleiting.top

Ruby: s == s.reverse
来源：http://tic.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vck.zycfv.cn

[N07] 两数之和（返回下标）
来源：http://gzd.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://grw.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ogx.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jlw.jyoumei.cn

TS:   // 手写 Map<string, number>
来源：http://mva.xziqi.cn

Java: // 手写 HashMap
来源：http://zjp.tian-w.cn

Go:   // 手写 map[int]int
来源：http://jqw.yangfankeji.com

Ruby: // 手写 Hash
来源：http://ags.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://qyj.ybcxt.top

[N08] 生成全排列
来源：http://ado.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://slt.c1oappe.top

PHP:  // 手写递归交换
来源：http://wsm.andypj.xyz

JS:   // 手写回溯递归
来源：http://krl.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://crl.ivvv.top

Java: // 手写回溯递归
来源：http://ena.tianlin.xyz

Go:   // 手写回溯递归
来源：http://bgw.sjlbkw.cn

Ruby: arr.permutation.to_a
来源：http://lhs.9152youxi.cn

C#:   // 手写回溯递归
来源：http://fkq.wangshuangyany.cn

[N09] 栈与队列
来源：http://jrc.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vnc.shanyushiyangtech.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iey.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ncq.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jct.aizwys.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uob.zhijiandao.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zlv.tian-w.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ejf.chenlongwang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://foc.0kj1m.cn

[N10] 链表节点定义
来源：http://rtt.cashguo.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ama.shangyingyoupin.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nml.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://foe.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jfi.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://iog.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ymh.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ioa.daria6918.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kxq.aibaodan.cn

[N11] 二叉树中序遍历
来源：http://xte.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://utg.hywenlv.cn

PHP:  // 手写递归函数
来源：http://lnf.9152youxi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dpf.daria6918.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pra.yongpay.top

Java: // 手写递归
来源：http://qqi.bjfxy.top

Go:   // 手写递归
来源：http://shk.fanxiaobao.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gey.zycfv.cn

C#:   // 手写递归
来源：http://yjv.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oyo.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hje.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fay.zhiwuduotai.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zja.sufxvd.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tof.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vux.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cqh.aibaodan.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nui.zhengqikj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tfm.ydjk.org.cn

================================================================================
来源：http://obr.hywenlv.cn

O. 并发与异步
来源：http://whl.gzhubu.top

================================================================================
来源：http://qvd.quarkkingdee.top

[O01] 启动一个线程
来源：http://tct.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qjm.svipenyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sjb.nanxinkj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rbt.kuanghao11.cn

TS:   // 同 JS
来源：http://fmd.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://ldp.wangshuangyany.cn

Go:   go f()
来源：http://oyf.haohaochexian.top

Ruby: Thread.new { f }
来源：http://crz.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://uew.wangshuangyany.cn

[O02] 使用线程池
来源：http://imy.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yeg.jqgfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zfe.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://nnz.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://ewc.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://lal.ywan-chungtsiang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://opv.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://drw.birdmap.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nmm.xylfe.cn

[O03] 加锁保护共享数据
来源：http://uxo.hcnkem.com

Py:   with lock: shared += 1
来源：http://faf.zhoulong.xyz

PHP:  // 用 flock() 做文件锁
来源：http://sjf.jiagoushi.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bfi.gaohongyu789.top

TS:   // 同 JS
来源：http://wld.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://mpd.gzhubu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uuu.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lpj.sysykeji.top

C#:   lock (gate) { shared++; }
来源：http://sqa.sweek.top

[O04] 定义异步函数并等待
来源：http://isf.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://bpn.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mdl.tarul.cn

JS:   async function f() { await g(); }
来源：http://lcq.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hhl.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pbt.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wnj.nanxuanxn.top

Ruby: # 用 Fiber 或 async gem
来源：http://fin.jyoumei.cn

C#:   async Task F() { await G(); }
来源：http://zrw.chenlongwang.top

[O05] 并发执行并等待全部完成
来源：http://sln.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://lje.zdbjq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uul.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://oyt.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://wae.daxiang520.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rvf.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zxl.yanxiufei.cn

Ruby: threads.map(&:join)
来源：http://kle.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fio.mhx1999.top

[O06] 使用进程池
来源：http://dfk.yuanzhike.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tlr.gotoacloud.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wow.tanke756.top

JS:   // child_process / cluster 模块
来源：http://ztm.hfpthk.cn

TS:   // child_process / cluster 模块
来源：http://fnv.pengpengdd.cyou

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://los.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ern.svipenyu.cn

Ruby: // fork 块
来源：http://vzh.gzhubu.top

C#:   Parallel.For
来源：http://wjj.havefunace.top

================================================================================
来源：http://yoj.xuetiantiany.cn

P. 常用工具函数
来源：http://ubs.uphjek.com

================================================================================
来源：http://aoz.tanke756.top

[P01] 生成 UUID
来源：http://vbx.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://ytt.fehbvm.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rtj.zhixingplan.top

JS:   crypto.randomUUID()
来源：http://dsx.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://xij.jinghuilouyu.cn

Java: UUID.randomUUID().toString()
来源：http://wey.hysaishi.cn

Go:   // 用 github.com/google/uuid
来源：http://jip.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://wpk.yanxiufei.cn


<!-- 参考信息 -->