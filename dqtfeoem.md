代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ezz.zhoulong.xyz

[L04] 设置超时
来源：http://qsb.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://wtq.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lgn.zhaomingkeji.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iqb.dianchejie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://quj.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qlt.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ujc.cucudq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nrx.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gvt.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://msi.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vbg.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pve.feifeiyinyue.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pcd.pengpengdd.cyou

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qya.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rcs.ctjpmb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ygn.meibo888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sst.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vsh.bbcook.cn

[L06] 解析响应为 JSON
来源：http://kkx.cdnleiting.top

Py:   resp.json()
来源：http://quk.wangshuangyany.cn

PHP:  json_decode($body, true);
来源：http://vkv.havefunace.top

JS:   await resp.json()
来源：http://tne.nanxinkj.top

TS:   await resp.json()
来源：http://yxs.xylfe.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vaa.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kln.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://ywz.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kob.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://pou.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kll.jianghu66.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://heo.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://qyx.c1oappe.top

TS:   resp.ok;  resp.status
来源：http://fnp.yongpay.top

Java: resp.statusCode()
来源：http://zbu.cucudq.cn

Go:   resp.StatusCode
来源：http://rwq.xylfe.cn

Ruby: resp.code.to_i
来源：http://sem.jinqigfzy.top

C#:   (int)resp.StatusCode
来源：http://dmm.0kj1m.cn

[L08] 并发请求多个地址
来源：http://fqc.zhengqikj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://txs.wangshuangyany.cn

PHP:  curl_multi_init() 系列
来源：http://wof.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://izj.tarul.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gek.c1oappe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kyp.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vgo.yuxming.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wwr.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lfs.yuanzhike.top

================================================================================
来源：http://izg.meibo888.top

M. 命令行 / 进程 / 环境
来源：http://qyv.sweek.top

================================================================================
来源：http://cpp.vehdjk.com

[M01] 读取命令行参数
来源：http://ggx.daria6918.cn

Py:   sys.argv[1:]
来源：http://wfx.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://pxj.bjfxy.top

JS:   process.argv.slice(2)
来源：http://bda.hfpthk.cn

TS:   process.argv.slice(2)
来源：http://unt.yangfankeji.com

Java: args 数组（main 方法参数）
来源：http://rlv.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://yyg.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://yuf.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://piy.hnxiangtu.top

[M02] 读取环境变量
来源：http://ujj.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://epc.nanxinkj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://agn.yueranfly.top

JS:   process.env.HOME
来源：http://vif.fzhhl.top

TS:   process.env.HOME
来源：http://jiv.shzxlz.cn

Java: System.getenv("HOME")
来源：http://rai.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ygf.shangyingyoupin.top

Ruby: ENV["HOME"]
来源：http://xke.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://byf.nanxuanxn.top

[M03] 执行外部命令
来源：http://xbn.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gfp.haohaochexian.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gqb.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zwd.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://anx.cashguo.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xbb.yj20258888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ccq.chenlongwang.top

Ruby: system("ls -l");  `ls -l`
来源：http://brc.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://iwf.cheryme.top

[M04] 获取当前工作目录
来源：http://gpj.jqgfzy.top

Py:   os.getcwd()
来源：http://oxf.hysaishi.cn

PHP:  getcwd();
来源：http://wij.zhongyouzk.top

JS:   process.cwd()
来源：http://nxk.ydzc1.top

TS:   process.cwd()
来源：http://kai.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://fie.jqgufenzy.top

Go:   os.Getwd()
来源：http://hwl.dashuyun.cn

Ruby: Dir.pwd
来源：http://lue.vqdsnc.cn

C#:   Directory.GetCurrentDirectory()
来源：http://doj.kuanghao11.cn

[M05] 设置退出码
来源：http://dqe.hysaishi.cn

Py:   sys.exit(1)
来源：http://ssw.epnwcf.com

PHP:  exit(1);
来源：http://hja.tian-w.cn

JS:   process.exit(1)
来源：http://ltn.jiagoushi.top

TS:   process.exit(1)
来源：http://weh.zhongyouzk.top

Java: System.exit(1)
来源：http://drm.fengsongda.top

Go:   os.Exit(1)
来源：http://qdm.wangshuangyany.cn

Ruby: exit 1
来源：http://snt.sysykeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mtu.zhiwuduotai.top

[M06] 向标准错误输出
来源：http://qyd.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://pwa.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ywy.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://ytr.shangyingyoupin.top

TS:   console.error("err")
来源：http://xkl.dianchejie.cn

Java: System.err.println("err")
来源：http://jmn.redwolf501.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://svp.zhoulong.xyz

Ruby: warn "err"
来源：http://wsi.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://cye.havefunace.top

[M07] 判断是否为主入口
来源：http://eko.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://eqh.jianghu66.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://axa.fengsongda.top

JS:   require.main === module
来源：http://lhp.yj202588.top

TS:   require.main === module
来源：http://jwv.yanxiufei.cn

Java: public static void main(String[] args)
来源：http://ujd.quarkkingdee.top

Go:   func main()
来源：http://ypu.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nle.ydzc1.top

C#:   static void Main(string[] args)
来源：http://yla.tanke756.top

[M08] 获取系统与运行时信息
来源：http://htt.jiagoushi.top

Py:   platform.system();  platform.python_version()
来源：http://kbe.cqqwz.cn

PHP:  PHP_OS;  phpversion();
来源：http://odx.yueranfly.top

JS:   process.platform;  process.version
来源：http://auv.guowangkeji.top

TS:   process.platform;  process.version
来源：http://cin.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://psr.yj20258888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rph.nanxuanxn.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vyz.shzxlz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dco.cucudq.cn

================================================================================
来源：http://nnv.zhengqikj.top

N. 数据结构与算法
来源：http://ddn.yj20258888.top

================================================================================
来源：http://izh.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://fqp.chenzaomai.com

Py:   bisect.bisect_left(arr, x)
来源：http://ijm.0kj1m.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ylf.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dxr.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lsh.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://fls.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://dwu.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xtq.snrcjt.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xpi.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://krr.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://btg.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eoj.yuxming.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://opp.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zel.jinqigfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gou.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://xnd.bjfxy.top

Ruby: arr.sort
来源：http://gjc.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wvm.zhoulong.xyz

[N03] 快速排序（分治示例）
来源：http://xvg.mhx1999.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wij.guowangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://yuh.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://inj.havefunace.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qtb.sjlbkw.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wav.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dyb.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xov.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://ean.fktsv.cn

[N04] 斐波那契数列
来源：http://jjk.ppjwa.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://emc.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qwi.jinqigufen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ise.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mch.jinyuanbaomall.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nub.wangshuangyany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bkg.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rgn.sufxvd.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://olo.yj20258888.top

[N05] 最大公约数
来源：http://wbp.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://fvi.zhaomingkeji.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sfb.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gqj.9152youxi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nhf.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://feg.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fbn.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://qaz.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://udf.jinqigfzy.top

[N06] 判断回文字符串
来源：http://bal.redwolf501.top

Py:   s == s[::-1]
来源：http://gdx.cheryme.top

PHP:  $s === strrev($s);
来源：http://vso.zdqjudy.top

JS:   s === [...s].reverse().join("")
来源：http://akb.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://xwm.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ikd.hnxiangtu.top

Go:   // 双指针从两端比较
来源：http://ead.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://akp.hcnkem.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://omg.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://zkt.yj202588.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ppj.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zyj.xziqi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vmg.tian-w.cn

TS:   // 手写 Map<string, number>
来源：http://tky.hywenlv.cn

Java: // 手写 HashMap
来源：http://fyt.zhengqikj.top

Go:   // 手写 map[int]int
来源：http://gol.bbcook.cn

Ruby: // 手写 Hash
来源：http://enw.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vob.hysaishi.cn

[N08] 生成全排列
来源：http://stl.redwolf501.top

Py:   itertools.permutations(arr)
来源：http://ukq.aibaodan.cn

PHP:  // 手写递归交换
来源：http://mcd.daria6918.cn

JS:   // 手写回溯递归
来源：http://wbl.cdnleiting.top

TS:   // 手写回溯递归
来源：http://lyk.aibaodan.cn

Java: // 手写回溯递归
来源：http://yip.hammf.cn

Go:   // 手写回溯递归
来源：http://mrc.hammf.cn

Ruby: arr.permutation.to_a
来源：http://nzj.yj202588.top

C#:   // 手写回溯递归
来源：http://pxf.gotoacloud.top

[N09] 栈与队列
来源：http://uxx.birdmap.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://klv.fanxiaobao.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xos.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jze.guowangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wni.jqgfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yhe.fehbvm.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://frv.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mvi.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tsr.wangdashe.top

[N10] 链表节点定义
来源：http://jjh.guannengcc.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gqk.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://imh.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ywi.snrcjt.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://van.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://qcn.dianchejie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://swi.nwbrower.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cip.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hsd.guannengcc.top

[N11] 二叉树中序遍历
来源：http://msd.birdmap.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ghk.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://dxo.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://orf.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tnn.snrcjt.cn

Java: // 手写递归
来源：http://awn.zhongyouzk.top

Go:   // 手写递归
来源：http://kmu.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pds.sysykeji.top

C#:   // 手写递归
来源：http://nmx.fktsv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iis.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dov.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qmd.daxiang520.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dbr.dianchejie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bzp.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lhl.feifeiyinyue.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yqp.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sxb.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yrw.gotoacloud.top

================================================================================
来源：http://rcn.uphjek.com

O. 并发与异步
来源：http://joj.svipenyu.cn

================================================================================
来源：http://ohz.sxryk.cn

[O01] 启动一个线程
来源：http://tqd.yfazqb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cck.zhijiandao.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mcl.pycfn.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wyv.hnqzz.top

TS:   // 同 JS
来源：http://nxs.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://bpm.fanxiaobao.xyz

Go:   go f()
来源：http://fso.bbcook.cn

Ruby: Thread.new { f }
来源：http://gdt.nwbrower.top

C#:   Task.Run(() => F());
来源：http://kja.fzhhl.top

[O02] 使用线程池
来源：http://yln.c1oappe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ehm.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hdh.hcnkem.com

JS:   // worker_threads 线程池
来源：http://hfd.yvedp.cn

TS:   // worker_threads 线程池
来源：http://xkq.vehdjk.com

Java: Executors.newFixedThreadPool(4)
来源：http://kep.cheryme.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wac.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://trv.gzhubu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pki.chenjidiqi.icu

[O03] 加锁保护共享数据
来源：http://nnf.xinyue.icu

Py:   with lock: shared += 1
来源：http://gtm.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://ybs.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oig.bjfxy.top

TS:   // 同 JS
来源：http://jws.chenzaomai.com

Java: synchronized (this) { shared++; }
来源：http://clk.zhijiandao.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eej.smart0.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://cuh.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://sxh.nanxuanxn.top

[O04] 定义异步函数并等待
来源：http://rza.jiagoushi.top

Py:   async def f():⏎    await g()
来源：http://aue.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jmg.birdmap.top

JS:   async function f() { await g(); }
来源：http://jra.yongpay.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ykq.zhixingplan.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://koy.fanxiaobao.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ipj.chenjidiqi.icu

Ruby: # 用 Fiber 或 async gem
来源：http://koe.yanxiufei.cn

C#:   async Task F() { await G(); }
来源：http://wao.zdbjq.cn

[O05] 并发执行并等待全部完成
来源：http://kyi.gaohongyu789.top

Py:   asyncio.gather(*tasks)
来源：http://mgo.zdbjq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ztq.chenzaomai.com

JS:   await Promise.all(tasks)
来源：http://qin.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://qmb.uphjek.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ukm.sxryk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hlx.andypj.xyz

Ruby: threads.map(&:join)
来源：http://uol.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tsd.fzhhl.top

[O06] 使用进程池
来源：http://zqt.jyoumei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://enu.fanxiaobao.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://saq.tian-w.cn

JS:   // child_process / cluster 模块
来源：http://pxu.tarul.cn

TS:   // child_process / cluster 模块
来源：http://ehc.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fxo.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nzh.cashguo.top

Ruby: // fork 块
来源：http://lnp.snrcjt.cn

C#:   Parallel.For
来源：http://fzl.jqgufenzy.top

================================================================================
来源：http://mqx.ydzc1.top

P. 常用工具函数
来源：http://hhd.nanxinkj.top

================================================================================
来源：http://xsn.shangyingyoupin.top

[P01] 生成 UUID
来源：http://jan.jinghuilouyu.cn

Py:   str(uuid.uuid4())
来源：http://khy.jlsjyb.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://shw.shuidangran.top

JS:   crypto.randomUUID()
来源：http://zpy.vqdsnc.cn

TS:   crypto.randomUUID()
来源：http://pzz.snrcjt.cn

Java: UUID.randomUUID().toString()
来源：http://clo.jiagoushi.top

Go:   // 用 github.com/google/uuid
来源：http://lfb.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://bbu.c1oappe.top


<!-- 参考信息 -->