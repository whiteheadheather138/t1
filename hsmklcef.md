代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yvc.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pij.hnxiangtu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://erf.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ksw.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bsc.fehbvm.com

[L04] 设置超时
来源：http://lpl.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://fub.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jaz.gzhubu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gpg.hcnkem.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://txi.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ylx.cdnleiting.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://les.jinqigufen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://avq.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jjw.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://tfe.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cod.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nix.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ylv.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nlm.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gdl.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wfw.nanxinkj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ooz.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://piv.nwbrower.top

[L06] 解析响应为 JSON
来源：http://pzj.sweek.top

Py:   resp.json()
来源：http://lfs.yfazqb.com

PHP:  json_decode($body, true);
来源：http://ggw.jlsjyb.cn

JS:   await resp.json()
来源：http://gwc.nanxuanxn.top

TS:   await resp.json()
来源：http://uru.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hlk.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uzi.zdqjudy.top

Ruby: JSON.parse(resp.body)
来源：http://mob.xziqi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kbj.chenjidiqi.icu

[L07] 处理 HTTP 状态码
来源：http://rsm.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qbj.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iwy.tarul.cn

JS:   resp.ok;  resp.status
来源：http://gnj.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://oxp.xuetiantiany.cn

Java: resp.statusCode()
来源：http://evi.ivvv.top

Go:   resp.StatusCode
来源：http://hjw.c1oappe.top

Ruby: resp.code.to_i
来源：http://rua.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://spv.svipenyu.cn

[L08] 并发请求多个地址
来源：http://uye.52xcode.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mum.birdmap.top

PHP:  curl_multi_init() 系列
来源：http://ggf.nanxinkj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xxa.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xjy.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dmo.mhx1999.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pxa.yanxiufei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ktx.aibaodan.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lbd.yj20258.top

================================================================================
来源：http://fnj.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://qnh.ctjpmb.com

================================================================================
来源：http://hwv.smart0.xyz

[M01] 读取命令行参数
来源：http://nsh.haohaochexian.top

Py:   sys.argv[1:]
来源：http://rin.guannengcc.top

PHP:  $argv;  $argc;
来源：http://crs.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://osm.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://pqv.cheryme.top

Java: args 数组（main 方法参数）
来源：http://xak.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://arr.feifeiyinyue.top

Ruby: ARGV
来源：http://smp.chenlongwang.top

C#:   args 数组（Main 方法参数）
来源：http://plq.haohaochexian.top

[M02] 读取环境变量
来源：http://ktr.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://kjd.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qsq.kuanghao11.cn

JS:   process.env.HOME
来源：http://puc.nanxinkj.top

TS:   process.env.HOME
来源：http://krb.chenjidiqi.icu

Java: System.getenv("HOME")
来源：http://rvw.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xmz.fehbvm.com

Ruby: ENV["HOME"]
来源：http://htk.gogol.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eca.havefunace.top

[M03] 执行外部命令
来源：http://kud.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jcc.zycfv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ghe.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://aux.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fuo.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ymo.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xoi.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pes.pycfn.com

C#:   Process.Start("ls", "-l");
来源：http://pfi.xinyue.icu

[M04] 获取当前工作目录
来源：http://byx.yj202588.top

Py:   os.getcwd()
来源：http://rgm.xylfe.cn

PHP:  getcwd();
来源：http://waz.bjfxy.top

JS:   process.cwd()
来源：http://kmm.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://vej.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://nrg.gaohongyu789.top

Go:   os.Getwd()
来源：http://jlr.havefunace.top

Ruby: Dir.pwd
来源：http://zbe.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://lqv.hysaishi.cn

[M05] 设置退出码
来源：http://kuq.yongpay.top

Py:   sys.exit(1)
来源：http://dvf.ybcxt.top

PHP:  exit(1);
来源：http://xwl.nanxuanxn.top

JS:   process.exit(1)
来源：http://clb.andypj.xyz

TS:   process.exit(1)
来源：http://fme.tanke756.top

Java: System.exit(1)
来源：http://qap.yanxiufei.cn

Go:   os.Exit(1)
来源：http://lwa.zhengqikj.top

Ruby: exit 1
来源：http://bhx.daria6918.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ndu.zhixingplan.top

[M06] 向标准错误输出
来源：http://dxq.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://mpr.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rnm.yfazqb.com

JS:   console.error("err")
来源：http://eri.xylfe.cn

TS:   console.error("err")
来源：http://rln.daria6918.cn

Java: System.err.println("err")
来源：http://xit.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://knt.zhiwuduotai.top

Ruby: warn "err"
来源：http://edt.ybcxt.top

C#:   Console.Error.WriteLine("err")
来源：http://oot.hammf.cn

[M07] 判断是否为主入口
来源：http://nbc.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://fdr.wangdashe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qov.cqqwz.cn

JS:   require.main === module
来源：http://pna.redwolf501.top

TS:   require.main === module
来源：http://ixo.dashuyun.cn

Java: public static void main(String[] args)
来源：http://ljv.guowangkeji.top

Go:   func main()
来源：http://een.yonumen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kmr.jinghuilouyu.cn

C#:   static void Main(string[] args)
来源：http://kwk.gogol.net.cn

[M08] 获取系统与运行时信息
来源：http://vxi.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://kle.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://pvc.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://qir.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://ana.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fbc.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lvp.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://btw.pengpengdd.cyou

C#:   Environment.OSVersion;  Environment.Version
来源：http://dkq.sufxvd.cn

================================================================================
来源：http://axk.yj20258.top

N. 数据结构与算法
来源：http://knd.gzhubu.top

================================================================================
来源：http://hny.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://hya.haohaochexian.top

Py:   bisect.bisect_left(arr, x)
来源：http://xhh.gogol.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mmn.havefunace.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yam.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vbq.xziqi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qes.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://gyv.hammf.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yjq.svipenyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dgt.mhx1999.top

[N02] 排序（工程实践用内置实现）
来源：http://oyx.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://hqn.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mnc.shanyushiyangtech.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://oil.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rgx.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wpn.0kj1m.cn

Go:   slices.Sort(arr)
来源：http://sws.jinqigfzy.top

Ruby: arr.sort
来源：http://eba.meibo888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gek.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://inp.jyoumei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wjp.yangfankeji.com

PHP:  // 递归实现，或用 usort
来源：http://kds.sufxvd.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://stf.sweek.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xwp.hysaishi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vln.aibaodan.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://icg.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aiu.aibaodan.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wjk.aibaodan.cn

[N04] 斐波那契数列
来源：http://ggw.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nev.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pwu.dashuyun.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zrr.svipenyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uga.uphjek.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jwl.yuxming.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gco.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vmj.zhijiandao.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://puh.fzhhl.top

[N05] 最大公约数
来源：http://iwq.ivvv.top

Py:   math.gcd(a, b)
来源：http://tlh.kuanghao11.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kju.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xdw.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cax.ehwqpu.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jvm.9152youxi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zuz.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://gkf.pycfn.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lkz.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://jkx.zhengqikj.top

Py:   s == s[::-1]
来源：http://dim.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://sor.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://mfc.zdqjudy.top

TS:   s === [...s].reverse().join("")
来源：http://ctt.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dyk.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://nap.hnqzz.top

Ruby: s == s.reverse
来源：http://mhz.ydzc1.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rqw.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://hjw.shanyushiyangtech.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nev.tarul.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://udi.ywan-chungtsiang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gmq.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://umx.yj20258888.top

Java: // 手写 HashMap
来源：http://ywn.yj20258888.top

Go:   // 手写 map[int]int
来源：http://gpq.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://fjs.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://bym.sjlbkw.cn

[N08] 生成全排列
来源：http://zoi.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://vun.zdqjudy.top

PHP:  // 手写递归交换
来源：http://bli.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://lbh.gzhubu.top

TS:   // 手写回溯递归
来源：http://xpe.hongshengwenyu.top

Java: // 手写回溯递归
来源：http://hyy.daria6918.cn

Go:   // 手写回溯递归
来源：http://nkf.fengsongda.top

Ruby: arr.permutation.to_a
来源：http://inw.jlsjyb.cn

C#:   // 手写回溯递归
来源：http://uzd.gotoacloud.top

[N09] 栈与队列
来源：http://kdr.andypj.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eay.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mob.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pcw.yj202588.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qzd.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ocy.ydjk.org.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://drb.zdbjq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yam.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fnq.dashuyun.cn

[N10] 链表节点定义
来源：http://unn.haohaochexian.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yzw.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lfq.aizwys.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wvx.shzxlz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uht.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://fzv.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://pih.vehdjk.com

Ruby: Node = Struct.new(:v, :next)
来源：http://lzt.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ibd.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://zdm.nanxuanxn.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zdq.aibaodan.cn

PHP:  // 手写递归函数
来源：http://biq.cqqwz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zuf.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eqk.zhixingplan.top

Java: // 手写递归
来源：http://npo.ctjpmb.com

Go:   // 手写递归
来源：http://srr.yueranfly.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zez.hesvh.cn

C#:   // 手写递归
来源：http://nms.yangfankeji.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cal.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xug.jianghu66.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oqr.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ysu.dashuyun.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aim.cheryme.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mhg.xuanzx.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tdz.shanyushiyangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ntd.xylfe.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://msi.xuetiantiany.cn

================================================================================
来源：http://jst.sufxvd.cn

O. 并发与异步
来源：http://ome.iojbl.cn

================================================================================
来源：http://mus.zhaomingkeji.xyz

[O01] 启动一个线程
来源：http://nna.yongpay.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yfd.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bwr.hcnkem.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qtp.wangdashe.top

TS:   // 同 JS
来源：http://uxy.52xcode.cn

Java: new Thread(() -> f()).start()
来源：http://tyf.sjlbkw.cn

Go:   go f()
来源：http://tus.epnwcf.com

Ruby: Thread.new { f }
来源：http://cgy.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://twv.vehdjk.com

[O02] 使用线程池
来源：http://lqc.ppjwa.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gwf.mhx1999.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vqr.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://glw.zhongyouzk.top

TS:   // worker_threads 线程池
来源：http://rtc.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://uhp.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mju.ivvv.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qsj.andypj.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://koy.zhixingplan.top

[O03] 加锁保护共享数据
来源：http://dta.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://lse.gaohongyu789.top

PHP:  // 用 flock() 做文件锁
来源：http://anq.sxryk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ccu.cqqwz.cn

TS:   // 同 JS
来源：http://gfx.dianchejie.cn

Java: synchronized (this) { shared++; }
来源：http://ytu.zhiwuduotai.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://swh.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jhz.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://xkz.gogol.net.cn

[O04] 定义异步函数并等待
来源：http://duu.bbcook.cn

Py:   async def f():⏎    await g()
来源：http://neh.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://djj.daxiang520.top

JS:   async function f() { await g(); }
来源：http://tpb.nanxuanxn.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jhu.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hwg.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tft.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://wsn.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://pxq.fktsv.cn

[O05] 并发执行并等待全部完成
来源：http://gnm.hywenlv.cn

Py:   asyncio.gather(*tasks)
来源：http://qoa.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://alm.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://znp.tian-w.cn

TS:   await Promise.all(tasks)
来源：http://svi.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xuh.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zta.redwolf501.top

Ruby: threads.map(&:join)
来源：http://shz.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://elw.cucudq.cn

[O06] 使用进程池
来源：http://obe.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pne.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bge.hnxiangtu.top

JS:   // child_process / cluster 模块
来源：http://gpf.0kj1m.cn

TS:   // child_process / cluster 模块
来源：http://brk.hysaishi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://krh.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cga.iojbl.cn

Ruby: // fork 块
来源：http://nqu.zhaomingkeji.xyz

C#:   Parallel.For
来源：http://odp.vqdsnc.cn

================================================================================
来源：http://tsj.nwbrower.top

P. 常用工具函数
来源：http://jry.jqgfzy.top

================================================================================
来源：http://bqw.snrcjt.cn

[P01] 生成 UUID
来源：http://lqw.hnqzz.top

Py:   str(uuid.uuid4())
来源：http://zbj.sysykeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lmc.dianchejie.cn

JS:   crypto.randomUUID()
来源：http://qim.52xcode.cn


<!-- 参考信息 -->