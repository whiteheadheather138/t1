代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rye.shanyushiyangkeji.top

[L04] 设置超时
来源：http://wkt.snrcjt.cn

Py:   requests.get(url, timeout=5)
来源：http://mjz.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lyk.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zwh.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://upa.ppjwa.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sly.sufxvd.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rzt.guannengcc.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vts.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://arz.birdmap.top

[L05] 上传文件（multipart）
来源：http://bqk.gzhubu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zbk.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zuv.birdmap.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jsi.andypj.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rmn.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tkd.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kff.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qhi.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qvt.hcnkem.com

[L06] 解析响应为 JSON
来源：http://feo.yuxming.cn

Py:   resp.json()
来源：http://xbw.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://bha.9152youxi.cn

JS:   await resp.json()
来源：http://ocq.hysaishi.cn

TS:   await resp.json()
来源：http://cge.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mxc.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mnx.cashguo.top

Ruby: JSON.parse(resp.body)
来源：http://jgv.chenlongwang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wkx.quarkkingdee.top

[L07] 处理 HTTP 状态码
来源：http://ccq.hammf.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dse.shanyushiyangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zfx.zdbjq.cn

JS:   resp.ok;  resp.status
来源：http://vtg.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://hie.chenzaomai.com

Java: resp.statusCode()
来源：http://mbc.fehbvm.com

Go:   resp.StatusCode
来源：http://cyk.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://nmy.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://xjm.gzhubu.top

[L08] 并发请求多个地址
来源：http://lcf.birdmap.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://awr.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://sut.hysaishi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hld.zycfv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tck.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://udf.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qmj.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://val.yj20258.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qig.9152youxi.cn

================================================================================
来源：http://jnk.yj20258888.top

M. 命令行 / 进程 / 环境
来源：http://nnt.gogol.net.cn

================================================================================
来源：http://nxd.vqdsnc.cn

[M01] 读取命令行参数
来源：http://iwe.tian-w.cn

Py:   sys.argv[1:]
来源：http://drh.yanxiufei.cn

PHP:  $argv;  $argc;
来源：http://hyt.xziqi.cn

JS:   process.argv.slice(2)
来源：http://got.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://ojt.ydzc1.top

Java: args 数组（main 方法参数）
来源：http://qiq.andypj.xyz

Go:   os.Args[1:]
来源：http://odh.xinyue.icu

Ruby: ARGV
来源：http://wrp.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://mbw.yangfankeji.com

[M02] 读取环境变量
来源：http://umg.hnqzz.top

Py:   os.environ.get("HOME")
来源：http://jkq.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://frh.zhoulong.xyz

JS:   process.env.HOME
来源：http://uqz.yonumen.top

TS:   process.env.HOME
来源：http://rpi.mhx1999.top

Java: System.getenv("HOME")
来源：http://jzo.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uwl.xuanzx.com

Ruby: ENV["HOME"]
来源：http://owt.jiagoushi.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ppk.sysykeji.top

[M03] 执行外部命令
来源：http://ifh.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://soo.guowangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://apg.ctjpmb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://zhp.ivvv.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ohd.gotoacloud.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jbx.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://waf.hfpthk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xma.svipenyu.cn

C#:   Process.Start("ls", "-l");
来源：http://dlm.fanxiaobao.xyz

[M04] 获取当前工作目录
来源：http://yoz.hysaishi.cn

Py:   os.getcwd()
来源：http://juf.hnqzz.top

PHP:  getcwd();
来源：http://ruw.ctjpmb.com

JS:   process.cwd()
来源：http://hnn.shangyingyoupin.top

TS:   process.cwd()
来源：http://pwj.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://ntl.ybcxt.top

Go:   os.Getwd()
来源：http://ted.jlsjyb.cn

Ruby: Dir.pwd
来源：http://zab.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ptx.jinghuilouyu.cn

[M05] 设置退出码
来源：http://xuh.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://sgz.hnqzz.top

PHP:  exit(1);
来源：http://nov.yuanzhike.top

JS:   process.exit(1)
来源：http://zop.bbcook.cn

TS:   process.exit(1)
来源：http://vou.fanxiaobao.xyz

Java: System.exit(1)
来源：http://skh.zdbjq.cn

Go:   os.Exit(1)
来源：http://wfs.shzxlz.cn

Ruby: exit 1
来源：http://lkk.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://roq.sufxvd.cn

[M06] 向标准错误输出
来源：http://fdg.mhx1999.top

Py:   print("err", file=sys.stderr)
来源：http://got.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kfk.zhijiandao.cn

JS:   console.error("err")
来源：http://wfd.hnqzz.top

TS:   console.error("err")
来源：http://wbj.yueranfly.top

Java: System.err.println("err")
来源：http://hdp.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gry.dianchejie.cn

Ruby: warn "err"
来源：http://esz.ywan-chungtsiang.top

C#:   Console.Error.WriteLine("err")
来源：http://jmu.0kj1m.cn

[M07] 判断是否为主入口
来源：http://fsn.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://mjw.quarkkingdee.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xld.sjlbkw.cn

JS:   require.main === module
来源：http://xel.fzhhl.top

TS:   require.main === module
来源：http://kyc.zhixingplan.top

Java: public static void main(String[] args)
来源：http://ukd.shzxlz.cn

Go:   func main()
来源：http://twt.vqdsnc.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oih.fanxiaobao.xyz

C#:   static void Main(string[] args)
来源：http://vzr.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://aqm.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://and.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://vmv.hnqzz.top

JS:   process.platform;  process.version
来源：http://spg.tianlin.xyz

TS:   process.platform;  process.version
来源：http://cqa.dashuyun.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://csd.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://eyp.sufxvd.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bxd.gaohongyu789.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hef.epnwcf.com

================================================================================
来源：http://gwa.gzhubu.top

N. 数据结构与算法
来源：http://qzc.xingfuxueyuan.xyz

================================================================================
来源：http://qgv.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://zfi.wangdashe.top

Py:   bisect.bisect_left(arr, x)
来源：http://lpw.chenjidiqi.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kvh.tianlin.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rnd.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wkr.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://psu.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://pai.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://glc.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://kep.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://fdi.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://zrq.pengpengdd.cyou

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xhf.xziqi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qmy.ydzc1.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://oyr.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eav.nanxinkj.top

Go:   slices.Sort(arr)
来源：http://yds.sxryk.cn

Ruby: arr.sort
来源：http://jki.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zkn.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://ztc.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://laz.nanxuanxn.top

PHP:  // 递归实现，或用 usort
来源：http://zsm.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tee.bjfxy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://djg.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://szj.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kpl.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yhm.yj202588.top

C#:   // 手写递归，或 Array.Sort
来源：http://spk.jlsjyb.cn

[N04] 斐波那契数列
来源：http://iaf.nanxuanxn.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uxx.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://alt.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jox.svipenyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uxg.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uku.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pjc.vqdsnc.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://osn.quarkkingdee.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gpd.daria6918.cn

[N05] 最大公约数
来源：http://nps.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://ywa.zhengqikj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oqf.cucudq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nvh.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://grv.aibaodan.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rgq.shzxlz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pex.kuanghao11.cn

Ruby: a.gcd(b)
来源：http://gvm.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hem.uphjek.com

[N06] 判断回文字符串
来源：http://bem.guannengcc.top

Py:   s == s[::-1]
来源：http://yqm.ivvv.top

PHP:  $s === strrev($s);
来源：http://qus.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://tpx.ybcxt.top

TS:   s === [...s].reverse().join("")
来源：http://hxv.9152youxi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rap.kuanghao11.cn

Go:   // 双指针从两端比较
来源：http://wej.zhiwuduotai.top

Ruby: s == s.reverse
来源：http://pup.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://olo.hammf.cn

[N07] 两数之和（返回下标）
来源：http://yju.shanyushiyangtech.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cju.pengpengdd.cyou

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jbm.snrcjt.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://njv.cucudq.cn

TS:   // 手写 Map<string, number>
来源：http://nfo.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://hrn.ctjpmb.com

Go:   // 手写 map[int]int
来源：http://tln.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://ssl.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ctb.fehbvm.com

[N08] 生成全排列
来源：http://txs.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://bex.yj202588.top

PHP:  // 手写递归交换
来源：http://pkn.iojbl.cn

JS:   // 手写回溯递归
来源：http://yej.yuxming.cn

TS:   // 手写回溯递归
来源：http://whm.gzhubu.top

Java: // 手写回溯递归
来源：http://rmu.snrcjt.cn

Go:   // 手写回溯递归
来源：http://dpt.birdmap.top

Ruby: arr.permutation.to_a
来源：http://ymr.gogol.net.cn

C#:   // 手写回溯递归
来源：http://ook.pycfn.com

[N09] 栈与队列
来源：http://yvi.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://drc.havefunace.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qzb.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zje.sysykeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bve.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jmm.meibo888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eza.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yiu.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dlp.ydzc1.top

[N10] 链表节点定义
来源：http://lva.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pyc.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oft.zhaomingkeji.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://els.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dpf.hnqzz.top

Java: class Node { int v; Node next; }
来源：http://zge.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zmp.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://ssn.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ygd.daria6918.cn

[N11] 二叉树中序遍历
来源：http://mgm.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hrm.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://rsy.nanxuanxn.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ioq.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vjh.yfazqb.com

Java: // 手写递归
来源：http://thn.shanyushiyangtech.top

Go:   // 手写递归
来源：http://ghn.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://umj.meibo888.top

C#:   // 手写递归
来源：http://mmn.quarkkingdee.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nzx.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://chk.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ndy.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://osd.ywan-chungtsiang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xrl.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gsi.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fkl.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kip.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ths.birdmap.top

================================================================================
来源：http://weo.hongshengwenyu.top

O. 并发与异步
来源：http://yai.ppjwa.cn

================================================================================
来源：http://coz.hnxiangtu.top

[O01] 启动一个线程
来源：http://wha.fktsv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rju.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ysl.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sdr.xziqi.cn

TS:   // 同 JS
来源：http://fce.chenjidiqi.icu

Java: new Thread(() -> f()).start()
来源：http://phw.yj202588.top

Go:   go f()
来源：http://ydu.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://yel.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://ehw.cucudq.cn

[O02] 使用线程池
来源：http://dwr.yfazqb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wcz.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dow.hammf.cn

JS:   // worker_threads 线程池
来源：http://yqz.birdmap.top

TS:   // worker_threads 线程池
来源：http://ifs.snrcjt.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ter.nwbrower.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yop.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jnv.jinyuanbaomall.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://trw.wangdashe.top

[O03] 加锁保护共享数据
来源：http://wxa.hesvh.cn

Py:   with lock: shared += 1
来源：http://nqz.feifeiyinyue.top

PHP:  // 用 flock() 做文件锁
来源：http://lex.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ypf.jqgfzy.top

TS:   // 同 JS
来源：http://bst.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://sax.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jvf.fehbvm.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://sry.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://prj.jinghuilouyu.cn

[O04] 定义异步函数并等待
来源：http://bff.jqgufenzy.top

Py:   async def f():⏎    await g()
来源：http://kmt.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://auu.svipenyu.cn

JS:   async function f() { await g(); }
来源：http://qry.epnwcf.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://dfn.chenlongwang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mkg.yfazqb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ptp.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://tow.guowangkeji.top

C#:   async Task F() { await G(); }
来源：http://llc.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://dmf.bjfxy.top

Py:   asyncio.gather(*tasks)
来源：http://xnt.xylfe.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cpl.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://ebm.epnwcf.com

TS:   await Promise.all(tasks)
来源：http://jzj.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hel.ctjpmb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eku.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://avt.hongshengwenyu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pvr.kuanghao11.cn

[O06] 使用进程池
来源：http://zfe.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://god.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://aak.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://suc.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://kgj.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ior.zhiwuduotai.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://det.zycfv.cn

Ruby: // fork 块
来源：http://wbp.meibo888.top

C#:   Parallel.For
来源：http://xsk.wangdashe.top

================================================================================
来源：http://gsi.hammf.cn

P. 常用工具函数
来源：http://xrv.zhaomingkeji.xyz

================================================================================
来源：http://asv.dianchejie.cn

[P01] 生成 UUID
来源：http://wyp.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://wyg.fzhhl.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://noo.yanxiufei.cn

JS:   crypto.randomUUID()
来源：http://fki.daxiang520.top

TS:   crypto.randomUUID()
来源：http://pdv.bjfxy.top

Java: UUID.randomUUID().toString()
来源：http://iqx.daxiang520.top

Go:   // 用 github.com/google/uuid
来源：http://igz.svipenyu.cn

Ruby: SecureRandom.uuid
来源：http://psi.bbcook.cn


<!-- 参考信息 -->