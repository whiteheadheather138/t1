代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ecw.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qlw.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dbi.uphjek.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sfj.yj20258888.top

[L03] 设置自定义请求头
来源：http://yyp.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nmx.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://prd.ehwqpu.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://agy.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://twl.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cul.zhaomingkeji.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://thk.zhaomingkeji.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://icc.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hsw.tianlin.xyz

[L04] 设置超时
来源：http://ylt.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://qrl.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xal.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://viv.shanyushiyangtech.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cpd.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zke.yonumen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bpi.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uio.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ugi.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://pvy.hfpthk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://upr.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gtn.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yzf.hywenlv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jnx.sufxvd.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xsd.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wwo.hesvh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fue.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qxu.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://csx.ydzc1.top

Py:   resp.json()
来源：http://xil.haohaochexian.top

PHP:  json_decode($body, true);
来源：http://wgu.wangdashe.top

JS:   await resp.json()
来源：http://cms.birdmap.top

TS:   await resp.json()
来源：http://cgw.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mml.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uli.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://dmr.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://afd.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://xnh.zhoulong.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xhz.fehbvm.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ahg.ivvv.top

JS:   resp.ok;  resp.status
来源：http://cqc.nwbrower.top

TS:   resp.ok;  resp.status
来源：http://fwd.yuanzhike.top

Java: resp.statusCode()
来源：http://ahd.redwolf501.top

Go:   resp.StatusCode
来源：http://evw.cdnleiting.top

Ruby: resp.code.to_i
来源：http://gsa.pycfn.com

C#:   (int)resp.StatusCode
来源：http://qzd.yj20258888.top

[L08] 并发请求多个地址
来源：http://bhn.zhijiandao.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hth.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://psx.nanxinkj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xua.xylfe.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gcs.sxryk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://phk.sufxvd.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://etq.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mis.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kdw.sufxvd.cn

================================================================================
来源：http://jod.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://wuj.quarkkingdee.top

================================================================================
来源：http://fci.shzxlz.cn

[M01] 读取命令行参数
来源：http://nag.zdbjq.cn

Py:   sys.argv[1:]
来源：http://ajg.vqdsnc.cn

PHP:  $argv;  $argc;
来源：http://mug.yonumen.top

JS:   process.argv.slice(2)
来源：http://xkn.yuanzhike.top

TS:   process.argv.slice(2)
来源：http://jeq.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://jsb.wangdashe.top

Go:   os.Args[1:]
来源：http://rin.nanxinkj.top

Ruby: ARGV
来源：http://nuz.bbcook.cn

C#:   args 数组（Main 方法参数）
来源：http://ktz.kuanghao11.cn

[M02] 读取环境变量
来源：http://htv.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://inn.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zkv.shzxlz.cn

JS:   process.env.HOME
来源：http://qwo.gogol.net.cn

TS:   process.env.HOME
来源：http://dsj.yangfankeji.com

Java: System.getenv("HOME")
来源：http://kxo.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kmd.yanxiufei.cn

Ruby: ENV["HOME"]
来源：http://vjv.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tpy.guannengcc.top

[M03] 执行外部命令
来源：http://ohx.cheryme.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jil.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jhh.hongshengwenyu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lbf.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://hzx.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bnb.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://rqp.wangdashe.top

Ruby: system("ls -l");  `ls -l`
来源：http://rgo.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://bil.gotoacloud.top

[M04] 获取当前工作目录
来源：http://rog.quarkkingdee.top

Py:   os.getcwd()
来源：http://ijp.sjlbkw.cn

PHP:  getcwd();
来源：http://elu.jlsjyb.cn

JS:   process.cwd()
来源：http://wcv.yj202588.top

TS:   process.cwd()
来源：http://xxi.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://fui.daria6918.cn

Go:   os.Getwd()
来源：http://mem.yuanzhike.top

Ruby: Dir.pwd
来源：http://ltc.cashguo.top

C#:   Directory.GetCurrentDirectory()
来源：http://mpk.fzhhl.top

[M05] 设置退出码
来源：http://gfl.daria6918.cn

Py:   sys.exit(1)
来源：http://shk.xinyue.icu

PHP:  exit(1);
来源：http://ipe.cqqwz.cn

JS:   process.exit(1)
来源：http://fsw.chenzaomai.com

TS:   process.exit(1)
来源：http://arh.sysykeji.top

Java: System.exit(1)
来源：http://wqz.ydjk.org.cn

Go:   os.Exit(1)
来源：http://aon.wangshuangyany.cn

Ruby: exit 1
来源：http://gpe.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mzp.sufxvd.cn

[M06] 向标准错误输出
来源：http://nqs.nwbrower.top

Py:   print("err", file=sys.stderr)
来源：http://yyc.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://sie.yvedp.cn

JS:   console.error("err")
来源：http://lpx.birdmap.top

TS:   console.error("err")
来源：http://rbi.yonumen.top

Java: System.err.println("err")
来源：http://jki.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xxe.zdqjudy.top

Ruby: warn "err"
来源：http://auv.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://vot.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://wva.guowangkeji.top

Py:   if __name__ == "__main__":
来源：http://gsd.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gkh.sxryk.cn

JS:   require.main === module
来源：http://gct.zhaomingkeji.xyz

TS:   require.main === module
来源：http://nap.52xcode.cn

Java: public static void main(String[] args)
来源：http://dea.andypj.xyz

Go:   func main()
来源：http://vwa.havefunace.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cog.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://poj.sysykeji.top

[M08] 获取系统与运行时信息
来源：http://muk.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://oyb.chenlongwang.top

PHP:  PHP_OS;  phpversion();
来源：http://wcm.tanke756.top

JS:   process.platform;  process.version
来源：http://xpx.haohaochexian.top

TS:   process.platform;  process.version
来源：http://wel.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fhw.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://aao.vqdsnc.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xqu.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://otd.gaohongyu789.top

================================================================================
来源：http://lfs.fzhhl.top

N. 数据结构与算法
来源：http://rbp.wangdashe.top

================================================================================
来源：http://cbj.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://cgo.cashguo.top

Py:   bisect.bisect_left(arr, x)
来源：http://ixg.yj202588.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://twf.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jgh.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ble.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nvm.chenlongwang.top

Go:   sort.SearchInts(arr, x)
来源：http://vwq.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://icx.shanyushiyangtech.top

C#:   Array.BinarySearch(arr, x)
来源：http://ovw.yj20258.top

[N02] 排序（工程实践用内置实现）
来源：http://zfd.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://xwv.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nyg.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dwx.nanxuanxn.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vvi.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aft.sweek.top

Go:   slices.Sort(arr)
来源：http://wfu.xinyue.icu

Ruby: arr.sort
来源：http://qzc.cucudq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lvr.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://aed.fzhhl.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://avn.zycfv.cn

PHP:  // 递归实现，或用 usort
来源：http://xzg.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uas.shanyushiyangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xsf.yanxiufei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ywf.guannengcc.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rqj.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lbh.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://par.chenzaomai.com

[N04] 斐波那契数列
来源：http://ihb.sjlbkw.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wai.jiagoushi.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qbk.jqgufenzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hix.sufxvd.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qam.zhoulong.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zwq.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lhq.iojbl.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qap.hesvh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fck.chenlongwang.top

[N05] 最大公约数
来源：http://wes.guannengcc.top

Py:   math.gcd(a, b)
来源：http://qzv.ydzc1.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fzf.andypj.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tam.jqgfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xza.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jjp.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xub.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://teq.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uud.daria6918.cn

[N06] 判断回文字符串
来源：http://hbr.yanxiufei.cn

Py:   s == s[::-1]
来源：http://lkp.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://egv.redwolf501.top

JS:   s === [...s].reverse().join("")
来源：http://pvp.daxiang520.top

TS:   s === [...s].reverse().join("")
来源：http://jtt.dashuyun.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ofq.guannengcc.top

Go:   // 双指针从两端比较
来源：http://lbf.ppjwa.cn

Ruby: s == s.reverse
来源：http://jtw.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mba.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://jhr.pengpengdd.cyou

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://khv.jlsjyb.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ugw.xziqi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jvw.hammf.cn

TS:   // 手写 Map<string, number>
来源：http://wxp.jlsjyb.cn

Java: // 手写 HashMap
来源：http://jxz.vehdjk.com

Go:   // 手写 map[int]int
来源：http://nbe.zhongyouzk.top

Ruby: // 手写 Hash
来源：http://niy.dashuyun.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jqu.svipenyu.cn

[N08] 生成全排列
来源：http://yzm.hywenlv.cn

Py:   itertools.permutations(arr)
来源：http://ewo.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://vnc.yongpay.top

JS:   // 手写回溯递归
来源：http://opg.bjfxy.top

TS:   // 手写回溯递归
来源：http://bfa.gaohongyu789.top

Java: // 手写回溯递归
来源：http://wdz.hywenlv.cn

Go:   // 手写回溯递归
来源：http://jpc.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://nnr.smart0.xyz

C#:   // 手写回溯递归
来源：http://hlk.ehwqpu.com

[N09] 栈与队列
来源：http://aab.yvedp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jlf.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://thb.gotoacloud.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wue.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://crd.ctjpmb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wsq.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yeo.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zpr.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rhw.0kj1m.cn

[N10] 链表节点定义
来源：http://vuh.redwolf501.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dhq.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vgf.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wcw.meibo888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hjg.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://yxx.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://aip.guowangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mrz.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://glk.ydjk.org.cn

[N11] 二叉树中序遍历
来源：http://xfr.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fyr.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://gvh.yvedp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wxn.hnqzz.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://buz.yj20258.top

Java: // 手写递归
来源：http://dyx.shangyingyoupin.top

Go:   // 手写递归
来源：http://etc.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bki.hammf.cn

C#:   // 手写递归
来源：http://mha.xylfe.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://knv.fengsongda.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://naw.quarkkingdee.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cpm.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xtb.nanxinkj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dbr.andypj.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ijt.xziqi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rro.hywenlv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://swe.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iwm.jinyuanbaomall.cn

================================================================================
来源：http://ppg.tanke756.top

O. 并发与异步
来源：http://hgs.fengsongda.top

================================================================================
来源：http://tav.xuetiantiany.cn

[O01] 启动一个线程
来源：http://nrj.pengpengdd.cyou

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ykb.ydzc1.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jyf.yangfankeji.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mhd.guowangkeji.top

TS:   // 同 JS
来源：http://gui.sweek.top

Java: new Thread(() -> f()).start()
来源：http://svd.yvedp.cn

Go:   go f()
来源：http://sqb.yuxming.cn

Ruby: Thread.new { f }
来源：http://geq.yuanzhike.top

C#:   Task.Run(() => F());
来源：http://yhi.9152youxi.cn

[O02] 使用线程池
来源：http://ras.shanyushiyangtech.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://via.zdqjudy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ljy.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://lnl.epnwcf.com

TS:   // worker_threads 线程池
来源：http://cyi.zhixingplan.top

Java: Executors.newFixedThreadPool(4)
来源：http://rbf.hongshengwenyu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://biu.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vqu.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dlu.jyoumei.cn

[O03] 加锁保护共享数据
来源：http://osg.dashuyun.cn

Py:   with lock: shared += 1
来源：http://qdr.havefunace.top

PHP:  // 用 flock() 做文件锁
来源：http://uyj.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://klx.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://vdr.meibo888.top

Java: synchronized (this) { shared++; }
来源：http://flj.gaohongyu789.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tma.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ena.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://wnw.ybcxt.top

[O04] 定义异步函数并等待
来源：http://sgg.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://okf.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pfc.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://ika.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rys.shangyingyoupin.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vxz.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yzt.zhengqikj.top

Ruby: # 用 Fiber 或 async gem
来源：http://glj.tanke756.top

C#:   async Task F() { await G(); }
来源：http://uat.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://wwr.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://xmt.vehdjk.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mno.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://ans.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://lxp.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ira.9152youxi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mls.yonumen.top

Ruby: threads.map(&:join)
来源：http://ljt.feifeiyinyue.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jag.jinyuanbaomall.cn

[O06] 使用进程池
来源：http://ath.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jwv.ppjwa.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bno.wangdashe.top

JS:   // child_process / cluster 模块
来源：http://ijm.xuanzx.com

TS:   // child_process / cluster 模块
来源：http://lvt.xuanzx.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lbd.zhiwuduotai.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vpf.yj20258.top

Ruby: // fork 块
来源：http://xbw.vehdjk.com


<!-- 参考信息 -->