代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hpc.hnxiangtu.top

[L04] 设置超时
来源：http://bpe.kuanghao11.cn

Py:   requests.get(url, timeout=5)
来源：http://zmq.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yah.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yqu.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iun.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uaw.vehdjk.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jsl.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hcq.tianlin.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gem.fengsongda.top

[L05] 上传文件（multipart）
来源：http://khl.kuanghao11.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cib.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ljw.ybcxt.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dvj.kuanghao11.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rpm.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gnv.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hsw.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uje.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://woi.havefunace.top

[L06] 解析响应为 JSON
来源：http://sdq.wangdashe.top

Py:   resp.json()
来源：http://bem.yj202588.top

PHP:  json_decode($body, true);
来源：http://qey.nanxuanxn.top

JS:   await resp.json()
来源：http://oig.9152youxi.cn

TS:   await resp.json()
来源：http://gch.yj202588.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ioq.andypj.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qtd.shuidangran.top

Ruby: JSON.parse(resp.body)
来源：http://lla.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sqb.sweek.top

[L07] 处理 HTTP 状态码
来源：http://wrn.jqgfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xlh.xuetiantiany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://umq.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://otc.gaohongyu789.top

TS:   resp.ok;  resp.status
来源：http://cbm.sxryk.cn

Java: resp.statusCode()
来源：http://vco.yueranfly.top

Go:   resp.StatusCode
来源：http://ddg.dashuyun.cn

Ruby: resp.code.to_i
来源：http://dmj.hysaishi.cn

C#:   (int)resp.StatusCode
来源：http://yol.yangfankeji.com

[L08] 并发请求多个地址
来源：http://ffw.andypj.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ovm.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://hve.gaohongyu789.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://djb.hfpthk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fpa.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ljl.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://adm.jiagoushi.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://agu.bbcook.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xgq.hammf.cn

================================================================================
来源：http://abt.hfpthk.cn

M. 命令行 / 进程 / 环境
来源：http://thr.shanyushiyangkeji.top

================================================================================
来源：http://kad.yanxiufei.cn

[M01] 读取命令行参数
来源：http://fqt.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://gmv.zycfv.cn

PHP:  $argv;  $argc;
来源：http://wzn.tarul.cn

JS:   process.argv.slice(2)
来源：http://apc.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://aci.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://skr.jyoumei.cn

Go:   os.Args[1:]
来源：http://ktg.zhongyouzk.top

Ruby: ARGV
来源：http://gti.chenlongwang.top

C#:   args 数组（Main 方法参数）
来源：http://dnp.9152youxi.cn

[M02] 读取环境变量
来源：http://qbi.hywenlv.cn

Py:   os.environ.get("HOME")
来源：http://sdr.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cpz.nanxuanxn.top

JS:   process.env.HOME
来源：http://cgf.yongpay.top

TS:   process.env.HOME
来源：http://nol.yongpay.top

Java: System.getenv("HOME")
来源：http://xhs.yonumen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vmo.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://lcm.yuxming.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lze.gzhubu.top

[M03] 执行外部命令
来源：http://zri.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hgj.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vld.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://pcv.hongshengwenyu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zwl.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wpg.ybcxt.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vjk.fengsongda.top

Ruby: system("ls -l");  `ls -l`
来源：http://ejh.zhiwuduotai.top

C#:   Process.Start("ls", "-l");
来源：http://jzj.jinqigufen.top

[M04] 获取当前工作目录
来源：http://aok.ydzc1.top

Py:   os.getcwd()
来源：http://tia.wangdashe.top

PHP:  getcwd();
来源：http://qve.gotoacloud.top

JS:   process.cwd()
来源：http://lqk.tianlin.xyz

TS:   process.cwd()
来源：http://knw.cheryme.top

Java: Path.of("").toAbsolutePath()
来源：http://maj.feifeiyinyue.top

Go:   os.Getwd()
来源：http://lpm.sysykeji.top

Ruby: Dir.pwd
来源：http://jdx.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://jld.ivvv.top

[M05] 设置退出码
来源：http://ybr.yongpay.top

Py:   sys.exit(1)
来源：http://kok.zhengqikj.top

PHP:  exit(1);
来源：http://usw.fengsongda.top

JS:   process.exit(1)
来源：http://pbo.tianlin.xyz

TS:   process.exit(1)
来源：http://yok.wangdashe.top

Java: System.exit(1)
来源：http://npi.gotoacloud.top

Go:   os.Exit(1)
来源：http://shk.sysykeji.top

Ruby: exit 1
来源：http://kkm.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wno.gzhubu.top

[M06] 向标准错误输出
来源：http://jya.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://wcl.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://msm.9152youxi.cn

JS:   console.error("err")
来源：http://ijf.sweek.top

TS:   console.error("err")
来源：http://hnp.ctjpmb.com

Java: System.err.println("err")
来源：http://qhn.316326.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ybo.jinqigfzy.top

Ruby: warn "err"
来源：http://vbv.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://mit.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://fvf.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://wyv.zdqjudy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wba.jianghu66.top

JS:   require.main === module
来源：http://fyo.ydjk.org.cn

TS:   require.main === module
来源：http://yri.zhaomingkeji.xyz

Java: public static void main(String[] args)
来源：http://mah.zhengqikj.top

Go:   func main()
来源：http://pik.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ocg.xylfe.cn

C#:   static void Main(string[] args)
来源：http://gyo.snrcjt.cn

[M08] 获取系统与运行时信息
来源：http://jyg.daxiang520.top

Py:   platform.system();  platform.python_version()
来源：http://qef.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://bms.yonumen.top

JS:   process.platform;  process.version
来源：http://inl.chenzaomai.com

TS:   process.platform;  process.version
来源：http://kfy.ehwqpu.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rfy.fengsongda.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sfb.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sbf.zhiwuduotai.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nnv.hysaishi.cn

================================================================================
来源：http://axd.zycfv.cn

N. 数据结构与算法
来源：http://wgr.haohaochexian.top

================================================================================
来源：http://cjk.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://ogs.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://osk.ybcxt.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lta.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xyj.hnqzz.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qhy.yfazqb.com

Java: Arrays.binarySearch(arr, x)
来源：http://xay.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://oym.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dod.gzhubu.top

C#:   Array.BinarySearch(arr, x)
来源：http://sqh.xingfuxueyuan.xyz

[N02] 排序（工程实践用内置实现）
来源：http://ivq.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://era.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ouz.gogol.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ezp.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yfj.vqdsnc.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wnr.yj202588.top

Go:   slices.Sort(arr)
来源：http://rbj.316326.xyz

Ruby: arr.sort
来源：http://jfe.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bfg.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://xkb.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gtl.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://qcr.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bgi.cdnleiting.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vam.sxryk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oos.9152youxi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qtf.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aan.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yvr.ehwqpu.com

[N04] 斐波那契数列
来源：http://dxd.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ota.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cnv.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nay.bbcook.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ktq.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qza.jyoumei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rxd.fzhhl.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hcr.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vie.daria6918.cn

[N05] 最大公约数
来源：http://xbm.aizwys.cn

Py:   math.gcd(a, b)
来源：http://kxh.sxryk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://goh.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kop.chenlongwang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nhc.yuanzhike.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lgc.zhaomingkeji.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kus.ppjwa.cn

Ruby: a.gcd(b)
来源：http://sum.zhengqikj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qjm.ydzc1.top

[N06] 判断回文字符串
来源：http://sls.daria6918.cn

Py:   s == s[::-1]
来源：http://kiw.ywan-chungtsiang.top

PHP:  $s === strrev($s);
来源：http://kgj.jianghu66.top

JS:   s === [...s].reverse().join("")
来源：http://rvs.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://mld.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ccp.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://sfs.cucudq.cn

Ruby: s == s.reverse
来源：http://gdo.sufxvd.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vaz.xziqi.cn

[N07] 两数之和（返回下标）
来源：http://kbm.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zqi.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://awo.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://smc.zdqjudy.top

TS:   // 手写 Map<string, number>
来源：http://lzo.tanke756.top

Java: // 手写 HashMap
来源：http://oon.meibo888.top

Go:   // 手写 map[int]int
来源：http://bpx.birdmap.top

Ruby: // 手写 Hash
来源：http://cac.ybcxt.top

C#:   // 手写 Dictionary<int, int>
来源：http://kpb.316326.xyz

[N08] 生成全排列
来源：http://foy.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://nut.snrcjt.cn

PHP:  // 手写递归交换
来源：http://vne.tian-w.cn

JS:   // 手写回溯递归
来源：http://cdz.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://khu.tianlin.xyz

Java: // 手写回溯递归
来源：http://pkg.guowangkeji.top

Go:   // 手写回溯递归
来源：http://tsr.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://zaa.xingfuxueyuan.xyz

C#:   // 手写回溯递归
来源：http://uwo.c1oappe.top

[N09] 栈与队列
来源：http://mqz.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://stj.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://phm.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gmh.hongshengwenyu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jcv.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kmj.xziqi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://swv.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://psl.redwolf501.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iaw.jinqigfzy.top

[N10] 链表节点定义
来源：http://dio.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ngt.sysykeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://smc.yvedp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tte.hesvh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hug.cheryme.top

Java: class Node { int v; Node next; }
来源：http://ycg.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gma.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hlu.feifeiyinyue.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qio.zhaomingkeji.xyz

[N11] 二叉树中序遍历
来源：http://lki.nanxinkj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://psm.svipenyu.cn

PHP:  // 手写递归函数
来源：http://zrb.sufxvd.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dlp.tianlin.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mgi.quarkkingdee.top

Java: // 手写递归
来源：http://gwv.hnxiangtu.top

Go:   // 手写递归
来源：http://gig.haohaochexian.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pwa.fzhhl.top

C#:   // 手写递归
来源：http://ybl.yanxiufei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wst.zhengqikj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wpi.tian-w.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fyf.yongpay.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kun.dashuyun.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://asf.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hdc.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://swz.gzhubu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://efo.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ose.gaohongyu789.top

================================================================================
来源：http://mug.hfpthk.cn

O. 并发与异步
来源：http://kag.xinyue.icu

================================================================================
来源：http://gsg.ybcxt.top

[O01] 启动一个线程
来源：http://lbg.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://shq.zhoulong.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sps.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://osz.mhx1999.top

TS:   // 同 JS
来源：http://wxk.tanke756.top

Java: new Thread(() -> f()).start()
来源：http://pkf.svipenyu.cn

Go:   go f()
来源：http://gjv.shanyushiyangkeji.top

Ruby: Thread.new { f }
来源：http://urj.chenlongwang.top

C#:   Task.Run(() => F());
来源：http://tab.jinqigufen.top

[O02] 使用线程池
来源：http://oyj.yj20258.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lvk.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xrm.jinqigfzy.top

JS:   // worker_threads 线程池
来源：http://jms.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://oqj.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://oqg.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zue.yj20258888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cut.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tbk.hesvh.cn

[O03] 加锁保护共享数据
来源：http://wui.jlsjyb.cn

Py:   with lock: shared += 1
来源：http://hay.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://lbx.meibo888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sbb.hywenlv.cn

TS:   // 同 JS
来源：http://uvw.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://fyy.nwbrower.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dqe.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qub.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://oxi.daxiang520.top

[O04] 定义异步函数并等待
来源：http://aat.gzhubu.top

Py:   async def f():⏎    await g()
来源：http://jcy.epnwcf.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://byf.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://otg.sysykeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ilz.hnxiangtu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qaf.ydzc1.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sxc.cdnleiting.top

Ruby: # 用 Fiber 或 async gem
来源：http://nye.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://dia.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://zzj.yangfankeji.com

Py:   asyncio.gather(*tasks)
来源：http://yne.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mqw.jiagoushi.top

JS:   await Promise.all(tasks)
来源：http://spr.tian-w.cn

TS:   await Promise.all(tasks)
来源：http://hze.ehwqpu.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mef.fktsv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uha.yfazqb.com

Ruby: threads.map(&:join)
来源：http://avl.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wfh.gogol.net.cn

[O06] 使用进程池
来源：http://yia.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ryx.aizwys.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dlf.fehbvm.com

JS:   // child_process / cluster 模块
来源：http://fcy.jiagoushi.top

TS:   // child_process / cluster 模块
来源：http://gea.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ego.cashguo.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://coy.cdnleiting.top

Ruby: // fork 块
来源：http://pmt.aibaodan.cn

C#:   Parallel.For
来源：http://eli.ydjk.org.cn

================================================================================
来源：http://xip.svipenyu.cn

P. 常用工具函数
来源：http://pfz.andypj.xyz

================================================================================
来源：http://kcz.hcnkem.com

[P01] 生成 UUID
来源：http://arp.cashguo.top

Py:   str(uuid.uuid4())
来源：http://qnk.tianlin.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dim.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://bbs.nwbrower.top

TS:   crypto.randomUUID()
来源：http://vdq.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://meq.yueranfly.top

Go:   // 用 github.com/google/uuid
来源：http://guy.xuanzx.com

Ruby: SecureRandom.uuid
来源：http://khz.guowangkeji.top


<!-- 参考信息 -->