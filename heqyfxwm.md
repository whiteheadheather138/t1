代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cfm.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://acw.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kcf.svipenyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xus.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wkt.yongpay.top

[L04] 设置超时
来源：http://icq.tian-w.cn

Py:   requests.get(url, timeout=5)
来源：http://aaf.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pcx.guowangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wkp.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vrq.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vdo.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kap.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://edf.zhiwuduotai.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ntb.shuidangran.top

[L05] 上传文件（multipart）
来源：http://ynt.kuanghao11.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nqc.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wfr.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uje.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://asl.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qfk.cdnleiting.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://txf.zhixingplan.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hoc.zhaomingkeji.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oiq.aibaodan.cn

[L06] 解析响应为 JSON
来源：http://vhg.yvedp.cn

Py:   resp.json()
来源：http://hml.xuetiantiany.cn

PHP:  json_decode($body, true);
来源：http://oyq.hnqzz.top

JS:   await resp.json()
来源：http://ljk.hywenlv.cn

TS:   await resp.json()
来源：http://hgd.sweek.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kim.uphjek.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vwj.xinyue.icu

Ruby: JSON.parse(resp.body)
来源：http://cyy.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kne.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://smm.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lua.shanyushiyangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oky.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://cza.xuanzx.com

TS:   resp.ok;  resp.status
来源：http://icn.cqqwz.cn

Java: resp.statusCode()
来源：http://opz.snrcjt.cn

Go:   resp.StatusCode
来源：http://pmx.tarul.cn

Ruby: resp.code.to_i
来源：http://agl.yongpay.top

C#:   (int)resp.StatusCode
来源：http://elv.aizwys.cn

[L08] 并发请求多个地址
来源：http://wth.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ama.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://ani.svipenyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hsr.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pfe.cheryme.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tlm.fzhhl.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nem.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ckn.ctjpmb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ont.zhaomingkeji.xyz

================================================================================
来源：http://qri.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://hqw.hnxiangtu.top

================================================================================
来源：http://hkt.xziqi.cn

[M01] 读取命令行参数
来源：http://oat.xylfe.cn

Py:   sys.argv[1:]
来源：http://aku.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://eyk.xuanzx.com

JS:   process.argv.slice(2)
来源：http://xxd.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://qzr.uphjek.com

Java: args 数组（main 方法参数）
来源：http://sbk.ybcxt.top

Go:   os.Args[1:]
来源：http://lts.nanxinkj.top

Ruby: ARGV
来源：http://kol.fktsv.cn

C#:   args 数组（Main 方法参数）
来源：http://vgo.havefunace.top

[M02] 读取环境变量
来源：http://frc.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://bmu.hnxiangtu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iag.fzhhl.top

JS:   process.env.HOME
来源：http://vda.nanxuanxn.top

TS:   process.env.HOME
来源：http://umq.guowangkeji.top

Java: System.getenv("HOME")
来源：http://nam.jinqigfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ptb.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://xlb.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://irh.yuxming.cn

[M03] 执行外部命令
来源：http://qte.andypj.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cvl.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kpu.hywenlv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nvq.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://yay.shzxlz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mtz.fengsongda.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fgr.kuanghao11.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yzk.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://cmq.shzxlz.cn

[M04] 获取当前工作目录
来源：http://cfw.52xcode.cn

Py:   os.getcwd()
来源：http://hyc.gaohongyu789.top

PHP:  getcwd();
来源：http://wzi.tianlin.xyz

JS:   process.cwd()
来源：http://rsg.zdqjudy.top

TS:   process.cwd()
来源：http://ghl.bbcook.cn

Java: Path.of("").toAbsolutePath()
来源：http://bkw.tian-w.cn

Go:   os.Getwd()
来源：http://fbw.jlsjyb.cn

Ruby: Dir.pwd
来源：http://plj.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://phw.ppjwa.cn

[M05] 设置退出码
来源：http://bdt.meibo888.top

Py:   sys.exit(1)
来源：http://gcf.hnxiangtu.top

PHP:  exit(1);
来源：http://vtu.jianghu66.top

JS:   process.exit(1)
来源：http://zio.nanxinkj.top

TS:   process.exit(1)
来源：http://tic.ivvv.top

Java: System.exit(1)
来源：http://vze.jlsjyb.cn

Go:   os.Exit(1)
来源：http://tow.shangyingyoupin.top

Ruby: exit 1
来源：http://bnp.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kjx.gogol.net.cn

[M06] 向标准错误输出
来源：http://msx.hammf.cn

Py:   print("err", file=sys.stderr)
来源：http://pda.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://npl.hfpthk.cn

JS:   console.error("err")
来源：http://lgo.aizwys.cn

TS:   console.error("err")
来源：http://vpr.daxiang520.top

Java: System.err.println("err")
来源：http://nww.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://obx.wangshuangyany.cn

Ruby: warn "err"
来源：http://vzh.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://gxr.c1oappe.top

[M07] 判断是否为主入口
来源：http://wwh.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://kno.quarkkingdee.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lth.yueranfly.top

JS:   require.main === module
来源：http://zan.xziqi.cn

TS:   require.main === module
来源：http://gmw.sweek.top

Java: public static void main(String[] args)
来源：http://bww.cdnleiting.top

Go:   func main()
来源：http://rqt.bjfxy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rve.bbcook.cn

C#:   static void Main(string[] args)
来源：http://qzg.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://wfs.daxiang520.top

Py:   platform.system();  platform.python_version()
来源：http://sqi.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://flu.shuidangran.top

JS:   process.platform;  process.version
来源：http://tzs.shanyushiyangtech.top

TS:   process.platform;  process.version
来源：http://wpi.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tdx.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://iba.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tke.jinqigfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mcv.gogol.net.cn

================================================================================
来源：http://noe.zhongyouzk.top

N. 数据结构与算法
来源：http://aqk.c1oappe.top

================================================================================
来源：http://pkf.ywan-chungtsiang.top

[N01] 二分查找（有序数组）
来源：http://bkb.aibaodan.cn

Py:   bisect.bisect_left(arr, x)
来源：http://czu.ydjk.org.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hgr.aibaodan.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zeh.hesvh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://peo.9152youxi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wzv.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://zrz.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ije.zhaomingkeji.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://dsf.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://hbi.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://von.yvedp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://okj.shanyushiyangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://use.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://phn.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kpb.haohaochexian.top

Go:   slices.Sort(arr)
来源：http://rbi.cucudq.cn

Ruby: arr.sort
来源：http://qoo.quarkkingdee.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hvu.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://sot.ydjk.org.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xoi.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://mop.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cxc.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jws.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yac.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bzg.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://epd.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://ucu.fengsongda.top

[N04] 斐波那契数列
来源：http://qql.sweek.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wuy.jinqigufen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jui.shanyushiyangtech.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jix.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uvi.hammf.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jog.gogol.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fhw.gotoacloud.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pua.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ler.ppjwa.cn

[N05] 最大公约数
来源：http://dys.tarul.cn

Py:   math.gcd(a, b)
来源：http://rjm.pengpengdd.cyou

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://utt.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ceb.hfpthk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ylu.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://itc.ydjk.org.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hpj.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://eqw.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cdo.fktsv.cn

[N06] 判断回文字符串
来源：http://dbz.jqgufenzy.top

Py:   s == s[::-1]
来源：http://gon.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://vaq.yangfankeji.com

JS:   s === [...s].reverse().join("")
来源：http://vor.hnxiangtu.top

TS:   s === [...s].reverse().join("")
来源：http://hmj.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rdk.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://hck.havefunace.top

Ruby: s == s.reverse
来源：http://bqw.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pqp.daxiang520.top

[N07] 两数之和（返回下标）
来源：http://gur.nanxinkj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bih.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uni.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://lov.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://oii.redwolf501.top

Java: // 手写 HashMap
来源：http://hrj.pengpengdd.cyou

Go:   // 手写 map[int]int
来源：http://jdv.nanxuanxn.top

Ruby: // 手写 Hash
来源：http://ijr.ppjwa.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dnq.jianghu66.top

[N08] 生成全排列
来源：http://zoz.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://meq.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://wrg.dianchejie.cn

JS:   // 手写回溯递归
来源：http://ada.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://mon.zhengqikj.top

Java: // 手写回溯递归
来源：http://gai.daria6918.cn

Go:   // 手写回溯递归
来源：http://rdr.pycfn.com

Ruby: arr.permutation.to_a
来源：http://bby.nanxinkj.top

C#:   // 手写回溯递归
来源：http://kai.smart0.xyz

[N09] 栈与队列
来源：http://kpe.0kj1m.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://now.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wyy.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://okp.birdmap.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zgd.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ruq.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://crm.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cdo.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://spi.yj202588.top

[N10] 链表节点定义
来源：http://lpf.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xdm.zdqjudy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kcu.nanxuanxn.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://swr.0kj1m.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hwb.zhixingplan.top

Java: class Node { int v; Node next; }
来源：http://hxy.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bbm.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hnx.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://oex.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://uhd.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://khz.ybcxt.top

PHP:  // 手写递归函数
来源：http://ouq.redwolf501.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rka.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xhm.zhixingplan.top

Java: // 手写递归
来源：http://zka.hcnkem.com

Go:   // 手写递归
来源：http://zpy.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cqp.vehdjk.com

C#:   // 手写递归
来源：http://dcf.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bgm.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rwn.zhiwuduotai.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bgg.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bav.sufxvd.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gst.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lzn.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jjs.andypj.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tuz.cashguo.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fll.xingfuxueyuan.xyz

================================================================================
来源：http://ilo.sxryk.cn

O. 并发与异步
来源：http://lzf.aibaodan.cn

================================================================================
来源：http://ori.tanke756.top

[O01] 启动一个线程
来源：http://ith.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://orq.jiagoushi.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qhb.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://deu.xinyue.icu

TS:   // 同 JS
来源：http://eva.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://moo.fzhhl.top

Go:   go f()
来源：http://lob.yfazqb.com

Ruby: Thread.new { f }
来源：http://cdp.bjfxy.top

C#:   Task.Run(() => F());
来源：http://ryu.pengpengdd.cyou

[O02] 使用线程池
来源：http://ctn.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yvg.yfazqb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pic.tanke756.top

JS:   // worker_threads 线程池
来源：http://asz.quarkkingdee.top

TS:   // worker_threads 线程池
来源：http://umu.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://bwt.yueranfly.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://prq.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ato.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hxo.andypj.xyz

[O03] 加锁保护共享数据
来源：http://dsc.yj202588.top

Py:   with lock: shared += 1
来源：http://yev.pengpengdd.cyou

PHP:  // 用 flock() 做文件锁
来源：http://zsz.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ods.sxryk.cn

TS:   // 同 JS
来源：http://dhk.jinqigufen.top

Java: synchronized (this) { shared++; }
来源：http://wjs.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xoy.ydzc1.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://aak.quarkkingdee.top

C#:   lock (gate) { shared++; }
来源：http://eej.wangdashe.top

[O04] 定义异步函数并等待
来源：http://rdc.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://pbq.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rtg.jianghu66.top

JS:   async function f() { await g(); }
来源：http://qcl.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yqi.yj202588.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fjt.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gnr.dashuyun.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hzp.fzhhl.top

C#:   async Task F() { await G(); }
来源：http://xed.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://etx.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://ejz.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yrf.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://bjq.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://rtc.xziqi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ayt.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ekj.svipenyu.cn

Ruby: threads.map(&:join)
来源：http://bbo.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vwa.ivvv.top

[O06] 使用进程池
来源：http://gzh.xingfuxueyuan.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wxu.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rta.316326.xyz

JS:   // child_process / cluster 模块
来源：http://vas.yj20258.top

TS:   // child_process / cluster 模块
来源：http://xfw.zdbjq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ncf.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://suy.zhaomingkeji.xyz

Ruby: // fork 块
来源：http://sbn.aibaodan.cn

C#:   Parallel.For
来源：http://hmz.nanxinkj.top

================================================================================
来源：http://ujf.jlsjyb.cn

P. 常用工具函数
来源：http://hip.nanxinkj.top

================================================================================
来源：http://myl.ivvv.top

[P01] 生成 UUID
来源：http://tln.yuanzhike.top

Py:   str(uuid.uuid4())
来源：http://qxw.yonumen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bhr.mhx1999.top

JS:   crypto.randomUUID()
来源：http://qju.jqgufenzy.top


<!-- 参考信息 -->