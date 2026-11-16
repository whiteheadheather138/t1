代发 wailian999

[L03] 设置自定义请求头
来源：http://pvp.havefunace.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rzo.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tpj.jyoumei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nqh.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://stq.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qyl.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wnf.shangyingyoupin.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ieb.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hhm.ydzc1.top

[L04] 设置超时
来源：http://asd.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://mux.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zxe.svipenyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yzl.jyoumei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lpq.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://asn.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wto.sweek.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zpm.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://umq.smart0.xyz

[L05] 上传文件（multipart）
来源：http://rrq.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://drt.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xrn.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qrv.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hdb.shangyingyoupin.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xfp.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dgv.jinqigufen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sqx.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xja.gogol.net.cn

[L06] 解析响应为 JSON
来源：http://qbb.ivvv.top

Py:   resp.json()
来源：http://ujx.yj20258.top

PHP:  json_decode($body, true);
来源：http://szs.316326.xyz

JS:   await resp.json()
来源：http://mjc.iojbl.cn

TS:   await resp.json()
来源：http://wfq.redwolf501.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nyi.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dil.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://ybm.cashguo.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sgt.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://acg.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lzm.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xqp.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://kug.shangyingyoupin.top

TS:   resp.ok;  resp.status
来源：http://lyt.fehbvm.com

Java: resp.statusCode()
来源：http://esc.cdnleiting.top

Go:   resp.StatusCode
来源：http://mpz.xziqi.cn

Ruby: resp.code.to_i
来源：http://fhr.feifeiyinyue.top

C#:   (int)resp.StatusCode
来源：http://xoy.chenzaomai.com

[L08] 并发请求多个地址
来源：http://cgz.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hfl.sweek.top

PHP:  curl_multi_init() 系列
来源：http://mwa.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://epu.chenlongwang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vgp.iojbl.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ruk.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lba.ctjpmb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iex.jinqigfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://htt.tarul.cn

================================================================================
来源：http://qod.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://rwy.bbcook.cn

================================================================================
来源：http://ljf.jiagoushi.top

[M01] 读取命令行参数
来源：http://xjk.zhaomingkeji.xyz

Py:   sys.argv[1:]
来源：http://cyq.yuanzhike.top

PHP:  $argv;  $argc;
来源：http://mlc.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://jeq.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://scq.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://cdu.jlsjyb.cn

Go:   os.Args[1:]
来源：http://ycm.gogol.net.cn

Ruby: ARGV
来源：http://itw.wangshuangyany.cn

C#:   args 数组（Main 方法参数）
来源：http://liv.jlsjyb.cn

[M02] 读取环境变量
来源：http://ecw.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://szr.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bsr.sysykeji.top

JS:   process.env.HOME
来源：http://cxo.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://dvi.tianlin.xyz

Java: System.getenv("HOME")
来源：http://pyz.quarkkingdee.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uss.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://ufm.cucudq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hvj.cucudq.cn

[M03] 执行外部命令
来源：http://wvt.hammf.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://evo.shanyushiyangtech.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://llx.feifeiyinyue.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ceb.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://xqi.jiagoushi.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ldh.jianghu66.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jdb.zhaomingkeji.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://zka.zycfv.cn

C#:   Process.Start("ls", "-l");
来源：http://itg.xuanzx.com

[M04] 获取当前工作目录
来源：http://qrp.ctjpmb.com

Py:   os.getcwd()
来源：http://thq.wangshuangyany.cn

PHP:  getcwd();
来源：http://drr.hesvh.cn

JS:   process.cwd()
来源：http://rvr.fanxiaobao.xyz

TS:   process.cwd()
来源：http://uvt.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://kij.ehwqpu.com

Go:   os.Getwd()
来源：http://qfx.sufxvd.cn

Ruby: Dir.pwd
来源：http://ugo.gotoacloud.top

C#:   Directory.GetCurrentDirectory()
来源：http://obi.sweek.top

[M05] 设置退出码
来源：http://lkl.xylfe.cn

Py:   sys.exit(1)
来源：http://hhu.mhx1999.top

PHP:  exit(1);
来源：http://hai.chenlongwang.top

JS:   process.exit(1)
来源：http://obx.epnwcf.com

TS:   process.exit(1)
来源：http://pmg.kuanghao11.cn

Java: System.exit(1)
来源：http://edk.hcnkem.com

Go:   os.Exit(1)
来源：http://rok.wangshuangyany.cn

Ruby: exit 1
来源：http://iyc.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nzs.vqdsnc.cn

[M06] 向标准错误输出
来源：http://zyx.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://vsd.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ptk.ehwqpu.com

JS:   console.error("err")
来源：http://afc.jinqigufen.top

TS:   console.error("err")
来源：http://lri.hywenlv.cn

Java: System.err.println("err")
来源：http://ehc.tarul.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tck.vqdsnc.cn

Ruby: warn "err"
来源：http://nqg.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://umh.yvedp.cn

[M07] 判断是否为主入口
来源：http://jfd.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://ufd.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xka.hfpthk.cn

JS:   require.main === module
来源：http://ytk.pycfn.com

TS:   require.main === module
来源：http://dvg.chenzaomai.com

Java: public static void main(String[] args)
来源：http://qjf.mhx1999.top

Go:   func main()
来源：http://ppv.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zsp.52xcode.cn

C#:   static void Main(string[] args)
来源：http://clg.sufxvd.cn

[M08] 获取系统与运行时信息
来源：http://gem.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://klx.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://zlq.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://rvi.ivvv.top

TS:   process.platform;  process.version
来源：http://jlc.zhoulong.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zbh.ydjk.org.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://iqq.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qfv.hnqzz.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ave.hnqzz.top

================================================================================
来源：http://mxo.hfpthk.cn

N. 数据结构与算法
来源：http://aqy.jyoumei.cn

================================================================================
来源：http://jhr.zdbjq.cn

[N01] 二分查找（有序数组）
来源：http://ujn.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://iqc.ydjk.org.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dfk.iojbl.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xia.sxryk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kqy.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://zeb.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://gvw.aizwys.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ykj.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://ssr.havefunace.top

[N02] 排序（工程实践用内置实现）
来源：http://rwt.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://zoa.zycfv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pgx.cqqwz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jrh.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bnc.yonumen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mso.yfazqb.com

Go:   slices.Sort(arr)
来源：http://bhe.vehdjk.com

Ruby: arr.sort
来源：http://mpq.yfazqb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://xld.hywenlv.cn

[N03] 快速排序（分治示例）
来源：http://cqe.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ujv.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://tbz.cashguo.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pls.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tli.shangyingyoupin.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://buw.jinghuilouyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bpp.ppjwa.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ybz.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fif.andypj.xyz

[N04] 斐波那契数列
来源：http://kcc.jinyuanbaomall.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qxp.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jzh.wangdashe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://osn.zhixingplan.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vnk.guannengcc.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ynp.chenzaomai.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hjs.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qhb.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yin.fengsongda.top

[N05] 最大公约数
来源：http://oks.yuanzhike.top

Py:   math.gcd(a, b)
来源：http://pgs.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zkp.chenzaomai.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yqm.ehwqpu.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ohc.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qsy.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wik.316326.xyz

Ruby: a.gcd(b)
来源：http://wiy.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mop.aibaodan.cn

[N06] 判断回文字符串
来源：http://wpg.yonumen.top

Py:   s == s[::-1]
来源：http://gat.tian-w.cn

PHP:  $s === strrev($s);
来源：http://rim.svipenyu.cn

JS:   s === [...s].reverse().join("")
来源：http://jlk.wangdashe.top

TS:   s === [...s].reverse().join("")
来源：http://pab.svipenyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qxf.svipenyu.cn

Go:   // 双指针从两端比较
来源：http://wwt.hysaishi.cn

Ruby: s == s.reverse
来源：http://lxf.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fmr.zhongyouzk.top

[N07] 两数之和（返回下标）
来源：http://pmu.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jmh.jlsjyb.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rsl.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yht.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://hra.hfpthk.cn

Java: // 手写 HashMap
来源：http://fvo.yongpay.top

Go:   // 手写 map[int]int
来源：http://qaq.svipenyu.cn

Ruby: // 手写 Hash
来源：http://hej.haohaochexian.top

C#:   // 手写 Dictionary<int, int>
来源：http://zlx.jiagoushi.top

[N08] 生成全排列
来源：http://kjy.cdnleiting.top

Py:   itertools.permutations(arr)
来源：http://qpe.birdmap.top

PHP:  // 手写递归交换
来源：http://cts.aibaodan.cn

JS:   // 手写回溯递归
来源：http://sww.ppjwa.cn

TS:   // 手写回溯递归
来源：http://fjo.dianchejie.cn

Java: // 手写回溯递归
来源：http://yoa.c1oappe.top

Go:   // 手写回溯递归
来源：http://vwa.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://zig.jinqigfzy.top

C#:   // 手写回溯递归
来源：http://qow.yangfankeji.com

[N09] 栈与队列
来源：http://yyn.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bdp.haohaochexian.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iob.chenzaomai.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jwi.bbcook.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lpe.jqgfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ctu.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rsl.wangdashe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://krr.redwolf501.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lqm.ivvv.top

[N10] 链表节点定义
来源：http://rtv.cqqwz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://moq.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://anf.yongpay.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rxj.yvedp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ugn.hnxiangtu.top

Java: class Node { int v; Node next; }
来源：http://dmk.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://bep.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cta.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://erz.hnqzz.top

[N11] 二叉树中序遍历
来源：http://odz.zhengqikj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tzx.jiagoushi.top

PHP:  // 手写递归函数
来源：http://pvg.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fyk.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://klb.zhixingplan.top

Java: // 手写递归
来源：http://kda.jianghu66.top

Go:   // 手写递归
来源：http://hwh.hongshengwenyu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bhs.xingfuxueyuan.xyz

C#:   // 手写递归
来源：http://cop.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wwx.zhiwuduotai.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vyu.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fgl.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dyu.iojbl.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tzg.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yhk.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gxs.havefunace.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ezt.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lez.daria6918.cn

================================================================================
来源：http://tld.jiagoushi.top

O. 并发与异步
来源：http://siv.sxryk.cn

================================================================================
来源：http://ljj.uphjek.com

[O01] 启动一个线程
来源：http://pja.guannengcc.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ihi.zhaomingkeji.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yti.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cpc.daxiang520.top

TS:   // 同 JS
来源：http://zxn.aibaodan.cn

Java: new Thread(() -> f()).start()
来源：http://flb.jiagoushi.top

Go:   go f()
来源：http://uuv.jiagoushi.top

Ruby: Thread.new { f }
来源：http://jxp.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://zaa.nwbrower.top

[O02] 使用线程池
来源：http://nhx.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yht.nanxinkj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oag.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://dwy.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://rdx.yueranfly.top

Java: Executors.newFixedThreadPool(4)
来源：http://pey.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://con.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vbd.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rel.shanyushiyangtech.top

[O03] 加锁保护共享数据
来源：http://uhe.cashguo.top

Py:   with lock: shared += 1
来源：http://vgj.bjfxy.top

PHP:  // 用 flock() 做文件锁
来源：http://nvv.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pss.bjfxy.top

TS:   // 同 JS
来源：http://ngk.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://dod.yfazqb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bsf.zhoulong.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://dob.jlsjyb.cn

C#:   lock (gate) { shared++; }
来源：http://sxf.zhijiandao.cn

[O04] 定义异步函数并等待
来源：http://gbf.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://wca.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tvp.nanxinkj.top

JS:   async function f() { await g(); }
来源：http://zlb.yuanzhike.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yjc.smart0.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dnb.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rqh.fengsongda.top

Ruby: # 用 Fiber 或 async gem
来源：http://kgk.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://phy.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://trx.jyoumei.cn

Py:   asyncio.gather(*tasks)
来源：http://twc.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://swf.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://jxo.zdqjudy.top

TS:   await Promise.all(tasks)
来源：http://agv.feifeiyinyue.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tis.redwolf501.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dwb.fengsongda.top

Ruby: threads.map(&:join)
来源：http://rsn.hysaishi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://phg.dashuyun.cn

[O06] 使用进程池
来源：http://emo.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rjf.zhaomingkeji.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://zhk.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://oua.shanyushiyangtech.top

TS:   // child_process / cluster 模块
来源：http://mml.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pdm.aizwys.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ake.0kj1m.cn

Ruby: // fork 块
来源：http://urb.fanxiaobao.xyz

C#:   Parallel.For
来源：http://zhw.fehbvm.com

================================================================================
来源：http://ial.haohaochexian.top

P. 常用工具函数
来源：http://fec.9152youxi.cn

================================================================================
来源：http://ppb.ywan-chungtsiang.top


<!-- 参考信息 -->