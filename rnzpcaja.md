代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rjh.zdbjq.cn

[L04] 设置超时
来源：http://oaw.vqdsnc.cn

Py:   requests.get(url, timeout=5)
来源：http://skq.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pgw.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vqh.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xsr.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qtm.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uip.hnxiangtu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bew.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pkd.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://tai.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://noj.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rgl.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aif.pycfn.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xbp.yuanzhike.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wvm.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gqi.cdnleiting.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://php.bjfxy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ezo.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://qeg.vehdjk.com

Py:   resp.json()
来源：http://kwr.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://uor.chenlongwang.top

JS:   await resp.json()
来源：http://usj.daria6918.cn

TS:   await resp.json()
来源：http://gqt.yonumen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fom.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fpw.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://fam.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jsf.yj20258888.top

[L07] 处理 HTTP 状态码
来源：http://gpb.ydjk.org.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://myu.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://udr.iojbl.cn

JS:   resp.ok;  resp.status
来源：http://kzr.yuanzhike.top

TS:   resp.ok;  resp.status
来源：http://qkg.chenlongwang.top

Java: resp.statusCode()
来源：http://fas.feifeiyinyue.top

Go:   resp.StatusCode
来源：http://ivm.tianlin.xyz

Ruby: resp.code.to_i
来源：http://ctl.316326.xyz

C#:   (int)resp.StatusCode
来源：http://zhb.aizwys.cn

[L08] 并发请求多个地址
来源：http://zyx.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://alu.cashguo.top

PHP:  curl_multi_init() 系列
来源：http://kep.meibo888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mrj.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jml.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://djp.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://axn.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yll.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dpi.redwolf501.top

================================================================================
来源：http://usz.bjfxy.top

M. 命令行 / 进程 / 环境
来源：http://thq.shanyushiyangkeji.top

================================================================================
来源：http://alo.ivvv.top

[M01] 读取命令行参数
来源：http://tsz.hywenlv.cn

Py:   sys.argv[1:]
来源：http://vuj.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://gfo.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://qom.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://ocx.aizwys.cn

Java: args 数组（main 方法参数）
来源：http://aft.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://owi.pycfn.com

Ruby: ARGV
来源：http://edp.yvedp.cn

C#:   args 数组（Main 方法参数）
来源：http://fdk.ybcxt.top

[M02] 读取环境变量
来源：http://xvv.zhijiandao.cn

Py:   os.environ.get("HOME")
来源：http://gvq.mhx1999.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gey.redwolf501.top

JS:   process.env.HOME
来源：http://ddn.guowangkeji.top

TS:   process.env.HOME
来源：http://fmc.zhixingplan.top

Java: System.getenv("HOME")
来源：http://sbd.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://deb.zhongyouzk.top

Ruby: ENV["HOME"]
来源：http://bka.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vuc.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://dam.zhongyouzk.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vsi.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vrj.tianlin.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://xwi.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tma.hysaishi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ios.tarul.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tcw.aibaodan.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nzr.zhixingplan.top

C#:   Process.Start("ls", "-l");
来源：http://jsu.jyoumei.cn

[M04] 获取当前工作目录
来源：http://lti.jqgfzy.top

Py:   os.getcwd()
来源：http://tmh.guowangkeji.top

PHP:  getcwd();
来源：http://pvs.aibaodan.cn

JS:   process.cwd()
来源：http://lij.pengpengdd.cyou

TS:   process.cwd()
来源：http://ozy.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://kdk.hywenlv.cn

Go:   os.Getwd()
来源：http://ujc.hcnkem.com

Ruby: Dir.pwd
来源：http://apm.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://prv.bbcook.cn

[M05] 设置退出码
来源：http://cbm.0kj1m.cn

Py:   sys.exit(1)
来源：http://ihh.yongpay.top

PHP:  exit(1);
来源：http://ejk.chenlongwang.top

JS:   process.exit(1)
来源：http://edr.chenjidiqi.icu

TS:   process.exit(1)
来源：http://eac.jlsjyb.cn

Java: System.exit(1)
来源：http://hzt.xuanzx.com

Go:   os.Exit(1)
来源：http://ock.cqqwz.cn

Ruby: exit 1
来源：http://wqv.hnqzz.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lvu.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://fam.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://nem.sjlbkw.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://khy.nwbrower.top

JS:   console.error("err")
来源：http://vci.cucudq.cn

TS:   console.error("err")
来源：http://ijo.gotoacloud.top

Java: System.err.println("err")
来源：http://xva.vqdsnc.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ojb.zhengqikj.top

Ruby: warn "err"
来源：http://zhg.mhx1999.top

C#:   Console.Error.WriteLine("err")
来源：http://iwh.9152youxi.cn

[M07] 判断是否为主入口
来源：http://mot.zdqjudy.top

Py:   if __name__ == "__main__":
来源：http://otg.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tke.yonumen.top

JS:   require.main === module
来源：http://pxc.xuanzx.com

TS:   require.main === module
来源：http://iip.hongshengwenyu.top

Java: public static void main(String[] args)
来源：http://ujr.zhiwuduotai.top

Go:   func main()
来源：http://gnl.316326.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://joo.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://qlm.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://ueg.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://cpz.zhijiandao.cn

PHP:  PHP_OS;  phpversion();
来源：http://jdi.ppjwa.cn

JS:   process.platform;  process.version
来源：http://glp.dashuyun.cn

TS:   process.platform;  process.version
来源：http://svj.shanyushiyangtech.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dun.tanke756.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://arn.epnwcf.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dee.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yzz.zhongyouzk.top

================================================================================
来源：http://nfo.hammf.cn

N. 数据结构与算法
来源：http://kny.smart0.xyz

================================================================================
来源：http://hse.xinyue.icu

[N01] 二分查找（有序数组）
来源：http://czk.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://olg.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://flc.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hhz.snrcjt.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nnc.iojbl.cn

Java: Arrays.binarySearch(arr, x)
来源：http://orp.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://zkz.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eau.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://uqt.hnqzz.top

[N02] 排序（工程实践用内置实现）
来源：http://yfm.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://inz.chenjidiqi.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zgo.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://mjx.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ybo.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ewt.svipenyu.cn

Go:   slices.Sort(arr)
来源：http://nxn.hfpthk.cn

Ruby: arr.sort
来源：http://kkm.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://okz.snrcjt.cn

[N03] 快速排序（分治示例）
来源：http://njj.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xod.snrcjt.cn

PHP:  // 递归实现，或用 usort
来源：http://zbt.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mgd.ehwqpu.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oug.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wbp.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://teh.havefunace.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pep.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://riv.9152youxi.cn

[N04] 斐波那契数列
来源：http://alc.shuidangran.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ufj.cheryme.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xxz.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rif.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aje.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ycm.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://puq.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mjo.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wja.nanxuanxn.top

[N05] 最大公约数
来源：http://xlq.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://plb.tarul.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wha.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rxs.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hda.dashuyun.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wdj.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aew.zycfv.cn

Ruby: a.gcd(b)
来源：http://zlr.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nur.ctjpmb.com

[N06] 判断回文字符串
来源：http://bws.zdqjudy.top

Py:   s == s[::-1]
来源：http://mix.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://vrk.9152youxi.cn

JS:   s === [...s].reverse().join("")
来源：http://aro.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://sfi.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fgk.shanyushiyangtech.top

Go:   // 双指针从两端比较
来源：http://nqr.cdnleiting.top

Ruby: s == s.reverse
来源：http://geb.birdmap.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xlu.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://bsw.nanxinkj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ipe.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kec.yfazqb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ric.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://jws.yongpay.top

Java: // 手写 HashMap
来源：http://yrm.cdnleiting.top

Go:   // 手写 map[int]int
来源：http://oyy.wangdashe.top

Ruby: // 手写 Hash
来源：http://aws.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rvn.sufxvd.cn

[N08] 生成全排列
来源：http://ujw.hywenlv.cn

Py:   itertools.permutations(arr)
来源：http://uug.jianghu66.top

PHP:  // 手写递归交换
来源：http://gsc.tarul.cn

JS:   // 手写回溯递归
来源：http://dtb.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://gaf.tianlin.xyz

Java: // 手写回溯递归
来源：http://gmc.ivvv.top

Go:   // 手写回溯递归
来源：http://ydb.vehdjk.com

Ruby: arr.permutation.to_a
来源：http://voc.shzxlz.cn

C#:   // 手写回溯递归
来源：http://aih.sxryk.cn

[N09] 栈与队列
来源：http://dwq.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zfn.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xzg.xuanzx.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ivs.kuanghao11.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pxk.xuanzx.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ovh.gotoacloud.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jrd.yuanzhike.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hjb.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ucp.vqdsnc.cn

[N10] 链表节点定义
来源：http://dod.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://esr.ppjwa.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pjr.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mxl.xingfuxueyuan.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gbg.aibaodan.cn

Java: class Node { int v; Node next; }
来源：http://jaj.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://idg.52xcode.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gbg.hongshengwenyu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gfz.0kj1m.cn

[N11] 二叉树中序遍历
来源：http://cvc.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jvq.chenlongwang.top

PHP:  // 手写递归函数
来源：http://tzs.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ddv.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://may.yonumen.top

Java: // 手写递归
来源：http://yws.tanke756.top

Go:   // 手写递归
来源：http://bis.jianghu66.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://phb.sysykeji.top

C#:   // 手写递归
来源：http://nuq.daxiang520.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cog.zhengqikj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gok.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pwv.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dcz.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gxv.52xcode.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ogn.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jhd.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uwt.chenjidiqi.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nvs.sxryk.cn

================================================================================
来源：http://qkh.fktsv.cn

O. 并发与异步
来源：http://eym.c1oappe.top

================================================================================
来源：http://ewx.xziqi.cn

[O01] 启动一个线程
来源：http://kxa.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://typ.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vtn.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dud.yuanzhike.top

TS:   // 同 JS
来源：http://xwx.tanke756.top

Java: new Thread(() -> f()).start()
来源：http://vly.havefunace.top

Go:   go f()
来源：http://iyo.gotoacloud.top

Ruby: Thread.new { f }
来源：http://xer.daria6918.cn

C#:   Task.Run(() => F());
来源：http://pjz.hfpthk.cn

[O02] 使用线程池
来源：http://ptp.fzhhl.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pzj.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aff.aibaodan.cn

JS:   // worker_threads 线程池
来源：http://xwd.tarul.cn

TS:   // worker_threads 线程池
来源：http://chx.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://qdq.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jgn.xuetiantiany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ajj.fktsv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qnl.hcnkem.com

[O03] 加锁保护共享数据
来源：http://mwh.xinyue.icu

Py:   with lock: shared += 1
来源：http://zoy.0kj1m.cn

PHP:  // 用 flock() 做文件锁
来源：http://eby.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sai.zhoulong.xyz

TS:   // 同 JS
来源：http://git.tianlin.xyz

Java: synchronized (this) { shared++; }
来源：http://uni.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sux.hesvh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gwa.ydzc1.top

C#:   lock (gate) { shared++; }
来源：http://atx.0kj1m.cn

[O04] 定义异步函数并等待
来源：http://qlq.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://fjq.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wwg.ydzc1.top

JS:   async function f() { await g(); }
来源：http://qjn.52xcode.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lot.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yji.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jyj.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://hwv.yj20258.top

C#:   async Task F() { await G(); }
来源：http://sne.zdbjq.cn

[O05] 并发执行并等待全部完成
来源：http://smh.guannengcc.top

Py:   asyncio.gather(*tasks)
来源：http://dmv.hongshengwenyu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bsb.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://ksz.ehwqpu.com

TS:   await Promise.all(tasks)
来源：http://tck.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ego.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rsc.yvedp.cn

Ruby: threads.map(&:join)
来源：http://wqk.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xbe.nwbrower.top

[O06] 使用进程池
来源：http://rky.dashuyun.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pbx.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://fcb.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://ruz.shanyushiyangtech.top

TS:   // child_process / cluster 模块
来源：http://nco.feifeiyinyue.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yiw.hcnkem.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uvp.daria6918.cn

Ruby: // fork 块
来源：http://tyw.yuanzhike.top

C#:   Parallel.For
来源：http://hsw.snrcjt.cn

================================================================================
来源：http://ioh.jinqigfzy.top

P. 常用工具函数
来源：http://ebu.jyoumei.cn

================================================================================
来源：http://zop.zhiwuduotai.top

[P01] 生成 UUID
来源：http://jxa.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://aml.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ovv.fanxiaobao.xyz

JS:   crypto.randomUUID()
来源：http://lsd.fanxiaobao.xyz

TS:   crypto.randomUUID()
来源：http://uds.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://zsv.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://yrr.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://irw.hysaishi.cn


<!-- 参考信息 -->