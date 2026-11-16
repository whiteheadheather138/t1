代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kwz.dianchejie.cn

JS:   await fetch(url)
来源：http://wcj.jqgufenzy.top

TS:   await fetch(url)
来源：http://kvb.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://trs.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://kxb.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://soj.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://inq.pycfn.com

[L02] 发送 POST JSON
来源：http://pez.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://kjn.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aak.gogol.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vzk.fengsongda.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fuz.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hsa.vqdsnc.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qsg.zhiwuduotai.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xuq.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fbs.bbcook.cn

[L03] 设置自定义请求头
来源：http://psr.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rph.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pzn.tarul.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vht.feifeiyinyue.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://crk.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ind.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://toz.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://htw.hcnkem.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kqk.zhiwuduotai.top

[L04] 设置超时
来源：http://ayq.jqgufenzy.top

Py:   requests.get(url, timeout=5)
来源：http://gqq.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nls.shuidangran.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://prn.redwolf501.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hdq.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zci.zhengqikj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://azq.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://psh.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://knz.sufxvd.cn

[L05] 上传文件（multipart）
来源：http://pjx.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ufg.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lgp.9152youxi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hzz.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ssg.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sbj.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://icg.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gyu.bjfxy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fxc.xingfuxueyuan.xyz

[L06] 解析响应为 JSON
来源：http://oya.chenlongwang.top

Py:   resp.json()
来源：http://xok.xziqi.cn

PHP:  json_decode($body, true);
来源：http://zsv.epnwcf.com

JS:   await resp.json()
来源：http://rbe.wangdashe.top

TS:   await resp.json()
来源：http://kep.ehwqpu.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ppu.fanxiaobao.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tos.ydjk.org.cn

Ruby: JSON.parse(resp.body)
来源：http://snt.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lub.hongshengwenyu.top

[L07] 处理 HTTP 状态码
来源：http://iuk.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mtz.yangfankeji.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://buc.yanxiufei.cn

JS:   resp.ok;  resp.status
来源：http://yjh.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://ltl.gogol.net.cn

Java: resp.statusCode()
来源：http://hya.daxiang520.top

Go:   resp.StatusCode
来源：http://bcm.jyoumei.cn

Ruby: resp.code.to_i
来源：http://gss.sjlbkw.cn

C#:   (int)resp.StatusCode
来源：http://swz.wangdashe.top

[L08] 并发请求多个地址
来源：http://dov.daria6918.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jgq.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://kef.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zmr.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dan.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yxq.hnxiangtu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dtb.zhengqikj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ews.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pku.zycfv.cn

================================================================================
来源：http://kzs.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://fxv.yuanzhike.top

================================================================================
来源：http://dmj.guowangkeji.top

[M01] 读取命令行参数
来源：http://knd.yongpay.top

Py:   sys.argv[1:]
来源：http://bkr.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://sdf.316326.xyz

JS:   process.argv.slice(2)
来源：http://guk.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://oxl.aizwys.cn

Java: args 数组（main 方法参数）
来源：http://jlw.cqqwz.cn

Go:   os.Args[1:]
来源：http://srr.9152youxi.cn

Ruby: ARGV
来源：http://wqg.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://kod.yanxiufei.cn

[M02] 读取环境变量
来源：http://avs.zdqjudy.top

Py:   os.environ.get("HOME")
来源：http://olz.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yyn.chenlongwang.top

JS:   process.env.HOME
来源：http://rmr.kuanghao11.cn

TS:   process.env.HOME
来源：http://iqj.yuxming.cn

Java: System.getenv("HOME")
来源：http://mox.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://idx.fehbvm.com

Ruby: ENV["HOME"]
来源：http://qnx.gogol.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cdw.uphjek.com

[M03] 执行外部命令
来源：http://yhd.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oeh.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pas.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wsn.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kxu.daxiang520.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wvz.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uzk.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://mfj.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://ftt.sweek.top

[M04] 获取当前工作目录
来源：http://xzm.yuxming.cn

Py:   os.getcwd()
来源：http://tgj.jqgufenzy.top

PHP:  getcwd();
来源：http://gpo.yvedp.cn

JS:   process.cwd()
来源：http://tgh.meibo888.top

TS:   process.cwd()
来源：http://soc.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://aoa.jyoumei.cn

Go:   os.Getwd()
来源：http://cvh.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://ioj.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://pni.meibo888.top

[M05] 设置退出码
来源：http://zrp.jyoumei.cn

Py:   sys.exit(1)
来源：http://irv.gogol.net.cn

PHP:  exit(1);
来源：http://qvp.cucudq.cn

JS:   process.exit(1)
来源：http://wrm.havefunace.top

TS:   process.exit(1)
来源：http://gvx.nwbrower.top

Java: System.exit(1)
来源：http://tko.jqgfzy.top

Go:   os.Exit(1)
来源：http://yof.xuanzx.com

Ruby: exit 1
来源：http://fcf.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yjx.cheryme.top

[M06] 向标准错误输出
来源：http://jle.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://fyq.ybcxt.top

PHP:  fwrite(STDERR, "err\n");
来源：http://igq.guannengcc.top

JS:   console.error("err")
来源：http://tbs.vqdsnc.cn

TS:   console.error("err")
来源：http://kyx.gaohongyu789.top

Java: System.err.println("err")
来源：http://aey.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mxb.nwbrower.top

Ruby: warn "err"
来源：http://zyo.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://drm.c1oappe.top

[M07] 判断是否为主入口
来源：http://ima.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://jqi.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ffj.smart0.xyz

JS:   require.main === module
来源：http://cqp.daxiang520.top

TS:   require.main === module
来源：http://mxn.sweek.top

Java: public static void main(String[] args)
来源：http://eib.haohaochexian.top

Go:   func main()
来源：http://thc.dashuyun.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jix.yuxming.cn

C#:   static void Main(string[] args)
来源：http://aae.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://dxd.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://xvd.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://mji.shanyushiyangtech.top

JS:   process.platform;  process.version
来源：http://bge.sweek.top

TS:   process.platform;  process.version
来源：http://fzd.jlsjyb.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gkz.epnwcf.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://dhr.hfpthk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uux.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://zij.yuanzhike.top

================================================================================
来源：http://cvv.sxryk.cn

N. 数据结构与算法
来源：http://mbx.aizwys.cn

================================================================================
来源：http://vpz.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://qxc.bjfxy.top

Py:   bisect.bisect_left(arr, x)
来源：http://kif.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oga.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lip.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ezm.feifeiyinyue.top

Java: Arrays.binarySearch(arr, x)
来源：http://poj.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://jow.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eiz.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://rmm.gaohongyu789.top

[N02] 排序（工程实践用内置实现）
来源：http://wnw.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://tds.andypj.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://utw.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://oot.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gkc.cheryme.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://exn.hnxiangtu.top

Go:   slices.Sort(arr)
来源：http://cbw.xuanzx.com

Ruby: arr.sort
来源：http://uck.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hnb.vehdjk.com

[N03] 快速排序（分治示例）
来源：http://igc.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kru.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://ajc.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cau.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rdu.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vsw.nanxuanxn.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://apb.zhengqikj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xxv.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://vke.chenzaomai.com

[N04] 斐波那契数列
来源：http://fei.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://npx.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sie.meibo888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wlm.cdnleiting.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nvk.jqgufenzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tjv.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qjx.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ifl.aibaodan.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xar.aibaodan.cn

[N05] 最大公约数
来源：http://cli.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://thl.yueranfly.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ady.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sne.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://onh.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ruu.fzhhl.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rjk.shuidangran.top

Ruby: a.gcd(b)
来源：http://xrp.hfpthk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jnx.9152youxi.cn

[N06] 判断回文字符串
来源：http://tin.ydjk.org.cn

Py:   s == s[::-1]
来源：http://oie.iojbl.cn

PHP:  $s === strrev($s);
来源：http://aef.birdmap.top

JS:   s === [...s].reverse().join("")
来源：http://dtz.andypj.xyz

TS:   s === [...s].reverse().join("")
来源：http://tqh.nanxinkj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jms.birdmap.top

Go:   // 双指针从两端比较
来源：http://ojm.hywenlv.cn

Ruby: s == s.reverse
来源：http://bzv.vehdjk.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://fal.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://jrd.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wft.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kih.cucudq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sat.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://jaa.haohaochexian.top

Java: // 手写 HashMap
来源：http://txy.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://vtq.sjlbkw.cn

Ruby: // 手写 Hash
来源：http://uqy.nanxuanxn.top

C#:   // 手写 Dictionary<int, int>
来源：http://gcj.daxiang520.top

[N08] 生成全排列
来源：http://ypd.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://axy.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://hxk.xziqi.cn

JS:   // 手写回溯递归
来源：http://anr.jinghuilouyu.cn

TS:   // 手写回溯递归
来源：http://rmx.jinqigfzy.top

Java: // 手写回溯递归
来源：http://hcd.wangdashe.top

Go:   // 手写回溯递归
来源：http://wze.xylfe.cn

Ruby: arr.permutation.to_a
来源：http://fbp.ydzc1.top

C#:   // 手写回溯递归
来源：http://bvw.chenzaomai.com

[N09] 栈与队列
来源：http://afs.sysykeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ble.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yri.dianchejie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pzx.shangyingyoupin.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lgl.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gsc.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uzq.zdqjudy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rof.yuanzhike.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qei.zdbjq.cn

[N10] 链表节点定义
来源：http://dma.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vxq.9152youxi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zda.ywan-chungtsiang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kjd.yueranfly.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://szv.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://lfe.yangfankeji.com

Go:   type Node struct { V int; Next *Node }
来源：http://wnx.tianlin.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://hyk.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://ish.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://awq.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qvv.vehdjk.com

PHP:  // 手写递归函数
来源：http://wyv.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jnp.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://izo.svipenyu.cn

Java: // 手写递归
来源：http://wxz.9152youxi.cn

Go:   // 手写递归
来源：http://pac.tian-w.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xca.fanxiaobao.xyz

C#:   // 手写递归
来源：http://lzn.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qmg.jianghu66.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://alr.gogol.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vrc.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ykn.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lvj.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lov.tianlin.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vxb.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dhw.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ucf.zhixingplan.top

================================================================================
来源：http://xno.wangshuangyany.cn

O. 并发与异步
来源：http://hrp.bbcook.cn

================================================================================
来源：http://qlo.vehdjk.com

[O01] 启动一个线程
来源：http://hst.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://owu.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://twn.yueranfly.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cjw.9152youxi.cn

TS:   // 同 JS
来源：http://fgh.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://fun.zhijiandao.cn

Go:   go f()
来源：http://plh.nanxinkj.top

Ruby: Thread.new { f }
来源：http://xuo.yonumen.top

C#:   Task.Run(() => F());
来源：http://ffs.0kj1m.cn

[O02] 使用线程池
来源：http://atu.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ypm.zdqjudy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nwn.jinqigufen.top

JS:   // worker_threads 线程池
来源：http://mys.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://edm.wangdashe.top

Java: Executors.newFixedThreadPool(4)
来源：http://sse.zdbjq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nit.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qho.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://emi.9152youxi.cn

[O03] 加锁保护共享数据
来源：http://xez.jqgfzy.top

Py:   with lock: shared += 1
来源：http://vhn.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://qus.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vzp.fehbvm.com

TS:   // 同 JS
来源：http://cuq.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://cut.yonumen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jbl.iojbl.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xia.havefunace.top

C#:   lock (gate) { shared++; }
来源：http://duj.cucudq.cn

[O04] 定义异步函数并等待
来源：http://mou.redwolf501.top

Py:   async def f():⏎    await g()
来源：http://vrm.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hrw.hnxiangtu.top

JS:   async function f() { await g(); }
来源：http://qem.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://mef.havefunace.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kyc.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dve.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://blu.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://hpb.hesvh.cn

[O05] 并发执行并等待全部完成
来源：http://hyu.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://nrh.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iaf.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://gdv.daria6918.cn

TS:   await Promise.all(tasks)
来源：http://xlt.zhaomingkeji.xyz


<!-- 参考信息 -->