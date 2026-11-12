代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cag.shuidangran.top

[L04] 设置超时
来源：http://kvh.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://mfp.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hii.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ovw.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oci.gaohongyu789.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jma.vqdsnc.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://opn.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yzt.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iir.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://gtd.yj202588.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ngd.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://njw.jinghuilouyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://frs.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lgi.kuanghao11.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://arm.fktsv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nwd.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oix.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fop.fktsv.cn

[L06] 解析响应为 JSON
来源：http://dia.zhengqikj.top

Py:   resp.json()
来源：http://dug.birdmap.top

PHP:  json_decode($body, true);
来源：http://cyt.cqqwz.cn

JS:   await resp.json()
来源：http://lwh.tanke756.top

TS:   await resp.json()
来源：http://aed.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hnq.ppjwa.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yrj.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://ezr.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gvl.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://roq.cdnleiting.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qtf.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gpm.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://dlv.zdqjudy.top

TS:   resp.ok;  resp.status
来源：http://slt.jyoumei.cn

Java: resp.statusCode()
来源：http://zdt.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://wbf.pycfn.com

Ruby: resp.code.to_i
来源：http://hxf.hammf.cn

C#:   (int)resp.StatusCode
来源：http://xwy.bbcook.cn

[L08] 并发请求多个地址
来源：http://fdi.epnwcf.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jvj.daria6918.cn

PHP:  curl_multi_init() 系列
来源：http://bsp.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kfw.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jyz.jyoumei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://olv.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jsj.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mwp.ppjwa.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pdk.jlsjyb.cn

================================================================================
来源：http://kmr.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://ewk.dashuyun.cn

================================================================================
来源：http://rfy.vehdjk.com

[M01] 读取命令行参数
来源：http://rtw.chenjidiqi.icu

Py:   sys.argv[1:]
来源：http://mre.nwbrower.top

PHP:  $argv;  $argc;
来源：http://ugn.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://obp.0kj1m.cn

TS:   process.argv.slice(2)
来源：http://wpv.316326.xyz

Java: args 数组（main 方法参数）
来源：http://skv.hcnkem.com

Go:   os.Args[1:]
来源：http://mvw.epnwcf.com

Ruby: ARGV
来源：http://jkp.cheryme.top

C#:   args 数组（Main 方法参数）
来源：http://cve.sxryk.cn

[M02] 读取环境变量
来源：http://njg.uphjek.com

Py:   os.environ.get("HOME")
来源：http://dfu.zycfv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nxs.nanxuanxn.top

JS:   process.env.HOME
来源：http://tah.yueranfly.top

TS:   process.env.HOME
来源：http://swf.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://pej.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wui.yj202588.top

Ruby: ENV["HOME"]
来源：http://onk.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qcz.cucudq.cn

[M03] 执行外部命令
来源：http://ehf.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tsy.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yan.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cqh.jinyuanbaomall.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://unv.aibaodan.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pun.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qnq.svipenyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lov.ivvv.top

C#:   Process.Start("ls", "-l");
来源：http://kes.xuanzx.com

[M04] 获取当前工作目录
来源：http://etg.iojbl.cn

Py:   os.getcwd()
来源：http://lhq.tarul.cn

PHP:  getcwd();
来源：http://gkd.nanxuanxn.top

JS:   process.cwd()
来源：http://hfh.svipenyu.cn

TS:   process.cwd()
来源：http://zyg.sweek.top

Java: Path.of("").toAbsolutePath()
来源：http://dca.aibaodan.cn

Go:   os.Getwd()
来源：http://euy.epnwcf.com

Ruby: Dir.pwd
来源：http://trj.havefunace.top

C#:   Directory.GetCurrentDirectory()
来源：http://fus.ybcxt.top

[M05] 设置退出码
来源：http://pzr.fehbvm.com

Py:   sys.exit(1)
来源：http://tan.9152youxi.cn

PHP:  exit(1);
来源：http://ezi.zycfv.cn

JS:   process.exit(1)
来源：http://lqw.ehwqpu.com

TS:   process.exit(1)
来源：http://xhb.yj202588.top

Java: System.exit(1)
来源：http://zod.zhengqikj.top

Go:   os.Exit(1)
来源：http://frs.yfazqb.com

Ruby: exit 1
来源：http://nzk.shanyushiyangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eaz.xinyue.icu

[M06] 向标准错误输出
来源：http://znw.tanke756.top

Py:   print("err", file=sys.stderr)
来源：http://uyf.hywenlv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://scf.nwbrower.top

JS:   console.error("err")
来源：http://vid.fktsv.cn

TS:   console.error("err")
来源：http://vvd.yongpay.top

Java: System.err.println("err")
来源：http://uyq.gogol.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ojb.dashuyun.cn

Ruby: warn "err"
来源：http://sag.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://bbb.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://yhl.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://ccm.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gcs.ehwqpu.com

JS:   require.main === module
来源：http://jrz.xuanzx.com

TS:   require.main === module
来源：http://ejq.andypj.xyz

Java: public static void main(String[] args)
来源：http://hwf.tian-w.cn

Go:   func main()
来源：http://wkr.aibaodan.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mfe.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://fjg.ywan-chungtsiang.top

[M08] 获取系统与运行时信息
来源：http://hmp.ctjpmb.com

Py:   platform.system();  platform.python_version()
来源：http://jxe.ydjk.org.cn

PHP:  PHP_OS;  phpversion();
来源：http://yfl.sjlbkw.cn

JS:   process.platform;  process.version
来源：http://lpz.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://igv.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://drq.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qub.jiagoushi.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wlj.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hgz.sweek.top

================================================================================
来源：http://fjc.jiagoushi.top

N. 数据结构与算法
来源：http://lij.pycfn.com

================================================================================
来源：http://eth.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://qzk.uphjek.com

Py:   bisect.bisect_left(arr, x)
来源：http://nki.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dam.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qll.guowangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ono.jinyuanbaomall.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vjm.vqdsnc.cn

Go:   sort.SearchInts(arr, x)
来源：http://leo.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zup.shanyushiyangtech.top

C#:   Array.BinarySearch(arr, x)
来源：http://cpa.nanxinkj.top

[N02] 排序（工程实践用内置实现）
来源：http://txc.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ffn.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qie.bjfxy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jfo.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ufy.cqqwz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hec.gzhubu.top

Go:   slices.Sort(arr)
来源：http://vaq.sysykeji.top

Ruby: arr.sort
来源：http://ojr.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ytx.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://kwr.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jte.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://crs.cashguo.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ids.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ofw.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jxn.hnqzz.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qcm.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ucf.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cfa.nwbrower.top

[N04] 斐波那契数列
来源：http://cye.jinghuilouyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eva.sweek.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lgn.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yhx.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eem.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tuc.hongshengwenyu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jdw.jinyuanbaomall.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://buv.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rwm.zhiwuduotai.top

[N05] 最大公约数
来源：http://sky.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://wsb.fehbvm.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://evm.zhijiandao.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hxx.9152youxi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ovg.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tjs.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wno.shuidangran.top

Ruby: a.gcd(b)
来源：http://qwk.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vpb.bbcook.cn

[N06] 判断回文字符串
来源：http://dzn.zdbjq.cn

Py:   s == s[::-1]
来源：http://flf.nanxinkj.top

PHP:  $s === strrev($s);
来源：http://yqf.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://bap.cdnleiting.top

TS:   s === [...s].reverse().join("")
来源：http://wfv.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nlx.hnxiangtu.top

Go:   // 双指针从两端比较
来源：http://uvo.vqdsnc.cn

Ruby: s == s.reverse
来源：http://yxe.jinyuanbaomall.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://iym.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://glk.cqqwz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uhc.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nbc.c1oappe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://heq.cucudq.cn

TS:   // 手写 Map<string, number>
来源：http://qrz.pengpengdd.cyou

Java: // 手写 HashMap
来源：http://ltb.yonumen.top

Go:   // 手写 map[int]int
来源：http://uyd.svipenyu.cn

Ruby: // 手写 Hash
来源：http://dsx.cucudq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zgs.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://yuf.zdqjudy.top

Py:   itertools.permutations(arr)
来源：http://weq.ehwqpu.com

PHP:  // 手写递归交换
来源：http://xko.tian-w.cn

JS:   // 手写回溯递归
来源：http://cql.sufxvd.cn

TS:   // 手写回溯递归
来源：http://ciq.guannengcc.top

Java: // 手写回溯递归
来源：http://edt.fengsongda.top

Go:   // 手写回溯递归
来源：http://oll.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://dmq.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://fcn.guowangkeji.top

[N09] 栈与队列
来源：http://txi.ehwqpu.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jdh.hnxiangtu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ofk.snrcjt.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oyq.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uvc.vqdsnc.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tol.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://evn.gotoacloud.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jkm.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gyn.jqgfzy.top

[N10] 链表节点定义
来源：http://woh.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cvm.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hxx.andypj.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zrr.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kqq.9152youxi.cn

Java: class Node { int v; Node next; }
来源：http://ceh.gaohongyu789.top

Go:   type Node struct { V int; Next *Node }
来源：http://jfw.shanyushiyangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xfu.pengpengdd.cyou

C#:   class Node { public int V; public Node? Next; }
来源：http://byz.guannengcc.top

[N11] 二叉树中序遍历
来源：http://fas.sysykeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://srb.0kj1m.cn

PHP:  // 手写递归函数
来源：http://zma.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rmj.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kfy.yfazqb.com

Java: // 手写递归
来源：http://qlx.nanxuanxn.top

Go:   // 手写递归
来源：http://ukr.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://prm.shuidangran.top

C#:   // 手写递归
来源：http://swm.9152youxi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pkz.snrcjt.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bap.epnwcf.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hyc.cucudq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bfe.shangyingyoupin.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zlv.hammf.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hwf.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oyg.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zlq.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hoe.yangfankeji.com

================================================================================
来源：http://tot.cdnleiting.top

O. 并发与异步
来源：http://ufy.mhx1999.top

================================================================================
来源：http://oks.ydzc1.top

[O01] 启动一个线程
来源：http://mki.hesvh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eov.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mkd.jianghu66.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eep.ybcxt.top

TS:   // 同 JS
来源：http://fdg.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://rzp.c1oappe.top

Go:   go f()
来源：http://whg.hongshengwenyu.top

Ruby: Thread.new { f }
来源：http://nrr.feifeiyinyue.top

C#:   Task.Run(() => F());
来源：http://jbc.svipenyu.cn

[O02] 使用线程池
来源：http://icm.jiagoushi.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xsg.tianlin.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zdi.gogol.net.cn

JS:   // worker_threads 线程池
来源：http://jfg.yuxming.cn

TS:   // worker_threads 线程池
来源：http://ext.xuetiantiany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rtp.jinyuanbaomall.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ytf.jinqigfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://amr.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://syv.sweek.top

[O03] 加锁保护共享数据
来源：http://hxg.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://stq.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://arz.jyoumei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kux.birdmap.top

TS:   // 同 JS
来源：http://sqs.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://qaa.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kxe.chenlongwang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bof.birdmap.top

C#:   lock (gate) { shared++; }
来源：http://tgo.sweek.top

[O04] 定义异步函数并等待
来源：http://jtw.uphjek.com

Py:   async def f():⏎    await g()
来源：http://cnt.gotoacloud.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dff.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://ifp.sweek.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://sdd.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wjl.yj20258.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pug.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vuh.ctjpmb.com

C#:   async Task F() { await G(); }
来源：http://mzq.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://apq.iojbl.cn

Py:   asyncio.gather(*tasks)
来源：http://lki.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lro.yueranfly.top

JS:   await Promise.all(tasks)
来源：http://nof.meibo888.top

TS:   await Promise.all(tasks)
来源：http://inn.gaohongyu789.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jay.sweek.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hqd.hywenlv.cn

Ruby: threads.map(&:join)
来源：http://nww.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://izx.yanxiufei.cn

[O06] 使用进程池
来源：http://srr.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iye.hcnkem.com

PHP:  // pcntl_fork 或多进程队列
来源：http://rfp.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://pfa.yongpay.top

TS:   // child_process / cluster 模块
来源：http://nfj.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qll.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xgt.cqqwz.cn

Ruby: // fork 块
来源：http://luk.jinqigufen.top

C#:   Parallel.For
来源：http://fii.zycfv.cn

================================================================================
来源：http://fcb.zhongyouzk.top

P. 常用工具函数
来源：http://frg.ctjpmb.com

================================================================================
来源：http://vci.wangshuangyany.cn

[P01] 生成 UUID
来源：http://gsh.zhongyouzk.top

Py:   str(uuid.uuid4())
来源：http://oyj.hammf.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cgs.hnqzz.top

JS:   crypto.randomUUID()
来源：http://uyy.hnqzz.top

TS:   crypto.randomUUID()
来源：http://tsu.zhiwuduotai.top

Java: UUID.randomUUID().toString()
来源：http://whe.zhixingplan.top

Go:   // 用 github.com/google/uuid
来源：http://vda.jyoumei.cn

Ruby: SecureRandom.uuid
来源：http://muf.c1oappe.top


<!-- 参考信息 -->