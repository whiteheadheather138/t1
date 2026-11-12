代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://emo.nanxuanxn.top

JS:   await fetch(url)
来源：http://zbx.daxiang520.top

TS:   await fetch(url)
来源：http://fkz.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pjx.zdqjudy.top

Go:   resp, err := http.Get(url)
来源：http://yqi.zhongyouzk.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sbr.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rif.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://dav.nanxuanxn.top

Py:   requests.post(url, json={"a": 1})
来源：http://dxv.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://myp.ctjpmb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xek.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pfd.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xdk.tianlin.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bly.aibaodan.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vlw.shzxlz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pwg.jianghu66.top

[L03] 设置自定义请求头
来源：http://xnf.birdmap.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iba.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://suw.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vvj.nanxinkj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ixx.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sfa.xuetiantiany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ndz.52xcode.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ovj.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ebj.sxryk.cn

[L04] 设置超时
来源：http://pdi.shanyushiyangtech.top

Py:   requests.get(url, timeout=5)
来源：http://jtj.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://spl.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qmf.guowangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://geb.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://evp.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ibt.tarul.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://suj.daxiang520.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zjg.bbcook.cn

[L05] 上传文件（multipart）
来源：http://sov.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hwi.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hmd.tian-w.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qwl.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wsb.wangdashe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vau.tarul.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kft.yuanzhike.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eio.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fvg.guannengcc.top

[L06] 解析响应为 JSON
来源：http://vht.fzhhl.top

Py:   resp.json()
来源：http://iip.yuanzhike.top

PHP:  json_decode($body, true);
来源：http://uch.sxryk.cn

JS:   await resp.json()
来源：http://xse.sysykeji.top

TS:   await resp.json()
来源：http://zqq.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uim.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://riz.cashguo.top

Ruby: JSON.parse(resp.body)
来源：http://rny.chenjidiqi.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aut.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://afi.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hiv.xuanzx.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://efb.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://uvy.shuidangran.top

TS:   resp.ok;  resp.status
来源：http://ffx.hesvh.cn

Java: resp.statusCode()
来源：http://bgd.nanxinkj.top

Go:   resp.StatusCode
来源：http://hdt.zhaomingkeji.xyz

Ruby: resp.code.to_i
来源：http://isv.tianlin.xyz

C#:   (int)resp.StatusCode
来源：http://arc.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://cnj.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kag.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://ije.haohaochexian.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uuo.shanyushiyangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nxa.hysaishi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bnl.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ogp.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://apl.jlsjyb.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bna.xziqi.cn

================================================================================
来源：http://lih.andypj.xyz

M. 命令行 / 进程 / 环境
来源：http://yms.ybcxt.top

================================================================================
来源：http://fmz.vehdjk.com

[M01] 读取命令行参数
来源：http://nij.bjfxy.top

Py:   sys.argv[1:]
来源：http://tfz.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://aps.jqgfzy.top

JS:   process.argv.slice(2)
来源：http://yhd.bbcook.cn

TS:   process.argv.slice(2)
来源：http://uol.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://twr.jqgufenzy.top

Go:   os.Args[1:]
来源：http://rqi.sysykeji.top

Ruby: ARGV
来源：http://qvk.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://amr.zycfv.cn

[M02] 读取环境变量
来源：http://itb.zhoulong.xyz

Py:   os.environ.get("HOME")
来源：http://yzb.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sez.zhiwuduotai.top

JS:   process.env.HOME
来源：http://oqs.yanxiufei.cn

TS:   process.env.HOME
来源：http://gsx.ydjk.org.cn

Java: System.getenv("HOME")
来源：http://twt.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lpt.pengpengdd.cyou

Ruby: ENV["HOME"]
来源：http://ciy.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qpx.yangfankeji.com

[M03] 执行外部命令
来源：http://agc.yongpay.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ura.shanyushiyangtech.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://esp.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pkd.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://xdh.zhoulong.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rzx.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ggm.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://dif.nanxinkj.top

C#:   Process.Start("ls", "-l");
来源：http://otq.andypj.xyz

[M04] 获取当前工作目录
来源：http://idj.xylfe.cn

Py:   os.getcwd()
来源：http://ice.fengsongda.top

PHP:  getcwd();
来源：http://oxf.quarkkingdee.top

JS:   process.cwd()
来源：http://hal.tianlin.xyz

TS:   process.cwd()
来源：http://teg.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://emn.havefunace.top

Go:   os.Getwd()
来源：http://qkf.yfazqb.com

Ruby: Dir.pwd
来源：http://vqf.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://acl.gotoacloud.top

[M05] 设置退出码
来源：http://kju.zhongyouzk.top

Py:   sys.exit(1)
来源：http://zpn.wangdashe.top

PHP:  exit(1);
来源：http://ehj.jinqigfzy.top

JS:   process.exit(1)
来源：http://azo.jinqigfzy.top

TS:   process.exit(1)
来源：http://uqb.sufxvd.cn

Java: System.exit(1)
来源：http://auc.wangdashe.top

Go:   os.Exit(1)
来源：http://kns.yanxiufei.cn

Ruby: exit 1
来源：http://ekf.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ewg.smart0.xyz

[M06] 向标准错误输出
来源：http://atp.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://mux.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pqu.iojbl.cn

JS:   console.error("err")
来源：http://dqo.jlsjyb.cn

TS:   console.error("err")
来源：http://ifh.shzxlz.cn

Java: System.err.println("err")
来源：http://amp.smart0.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aqy.cashguo.top

Ruby: warn "err"
来源：http://khs.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://akl.svipenyu.cn

[M07] 判断是否为主入口
来源：http://kdq.xziqi.cn

Py:   if __name__ == "__main__":
来源：http://vux.guowangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dsu.tarul.cn

JS:   require.main === module
来源：http://wjs.cucudq.cn

TS:   require.main === module
来源：http://exz.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://edf.yangfankeji.com

Go:   func main()
来源：http://xwy.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://amb.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://zmb.daxiang520.top

[M08] 获取系统与运行时信息
来源：http://bth.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://tof.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://avn.xuanzx.com

JS:   process.platform;  process.version
来源：http://rep.bjfxy.top

TS:   process.platform;  process.version
来源：http://thv.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pgb.xingfuxueyuan.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ldr.jinghuilouyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kzg.mhx1999.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://aur.xylfe.cn

================================================================================
来源：http://get.cdnleiting.top

N. 数据结构与算法
来源：http://mdl.52xcode.cn

================================================================================
来源：http://nui.316326.xyz

[N01] 二分查找（有序数组）
来源：http://zed.yj20258.top

Py:   bisect.bisect_left(arr, x)
来源：http://fla.fktsv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://byy.zhixingplan.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qes.jinqigfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nxm.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://xkg.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://bet.zhaomingkeji.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://bjx.pycfn.com

C#:   Array.BinarySearch(arr, x)
来源：http://jbh.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://pgu.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://yqy.wangdashe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bqv.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fch.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://raj.52xcode.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://llu.fengsongda.top

Go:   slices.Sort(arr)
来源：http://qwf.c1oappe.top

Ruby: arr.sort
来源：http://rer.guowangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kju.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://obl.gzhubu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://osx.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://oyl.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ngl.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nxa.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wyo.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pob.yanxiufei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gyh.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qfl.xinyue.icu

[N04] 斐波那契数列
来源：http://dbf.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xuq.yfazqb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vxu.havefunace.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://keq.yangfankeji.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cuv.xingfuxueyuan.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pke.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tcc.jinqigufen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xtz.tarul.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://flx.vqdsnc.cn

[N05] 最大公约数
来源：http://fyb.316326.xyz

Py:   math.gcd(a, b)
来源：http://sxn.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://axj.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qfw.hongshengwenyu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pik.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gan.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uzm.jyoumei.cn

Ruby: a.gcd(b)
来源：http://yxg.yanxiufei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qsb.wangdashe.top

[N06] 判断回文字符串
来源：http://mib.bjfxy.top

Py:   s == s[::-1]
来源：http://dti.cqqwz.cn

PHP:  $s === strrev($s);
来源：http://aew.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://yir.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://kwn.andypj.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vgf.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://rsj.ctjpmb.com

Ruby: s == s.reverse
来源：http://gxb.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://akw.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://hfy.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kfy.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gov.tanke756.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dir.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://izt.yvedp.cn

Java: // 手写 HashMap
来源：http://blf.feifeiyinyue.top

Go:   // 手写 map[int]int
来源：http://xit.hammf.cn

Ruby: // 手写 Hash
来源：http://wpz.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://usa.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://oli.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://jqr.cashguo.top

PHP:  // 手写递归交换
来源：http://dgc.hongshengwenyu.top

JS:   // 手写回溯递归
来源：http://tmk.daxiang520.top

TS:   // 手写回溯递归
来源：http://bdc.snrcjt.cn

Java: // 手写回溯递归
来源：http://dyi.zdqjudy.top

Go:   // 手写回溯递归
来源：http://szr.pycfn.com

Ruby: arr.permutation.to_a
来源：http://dgy.jinqigfzy.top

C#:   // 手写回溯递归
来源：http://kid.wangshuangyany.cn

[N09] 栈与队列
来源：http://opu.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ypf.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gpp.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bmq.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://luu.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yit.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://keh.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ell.fengsongda.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rub.sufxvd.cn

[N10] 链表节点定义
来源：http://kex.feifeiyinyue.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hbp.hfpthk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mwf.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iik.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iif.nanxinkj.top

Java: class Node { int v; Node next; }
来源：http://ktq.iojbl.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tky.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://aut.gaohongyu789.top

C#:   class Node { public int V; public Node? Next; }
来源：http://egw.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://ajd.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nfd.yuanzhike.top

PHP:  // 手写递归函数
来源：http://dyq.zdqjudy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wka.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pjn.birdmap.top

Java: // 手写递归
来源：http://pav.sufxvd.cn

Go:   // 手写递归
来源：http://xyy.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qrf.hysaishi.cn

C#:   // 手写递归
来源：http://fds.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ljn.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rth.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dwx.mhx1999.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ntv.snrcjt.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://utj.hnxiangtu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gst.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://epz.daxiang520.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://afd.xuetiantiany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wim.nanxinkj.top

================================================================================
来源：http://pvv.haohaochexian.top

O. 并发与异步
来源：http://yoq.epnwcf.com

================================================================================
来源：http://sev.cqqwz.cn

[O01] 启动一个线程
来源：http://lbe.jinyuanbaomall.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rvk.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tiu.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iye.epnwcf.com

TS:   // 同 JS
来源：http://ocq.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://wrb.andypj.xyz

Go:   go f()
来源：http://jnt.xinyue.icu

Ruby: Thread.new { f }
来源：http://oux.xuetiantiany.cn

C#:   Task.Run(() => F());
来源：http://sxe.sweek.top

[O02] 使用线程池
来源：http://drt.sxryk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lao.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xlt.ctjpmb.com

JS:   // worker_threads 线程池
来源：http://vxt.wangshuangyany.cn

TS:   // worker_threads 线程池
来源：http://can.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://mow.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://glo.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://avh.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zur.jlsjyb.cn

[O03] 加锁保护共享数据
来源：http://qha.xuetiantiany.cn

Py:   with lock: shared += 1
来源：http://sdq.pycfn.com

PHP:  // 用 flock() 做文件锁
来源：http://bml.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ako.snrcjt.cn

TS:   // 同 JS
来源：http://grt.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://vax.yuxming.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qjv.wangshuangyany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cin.cashguo.top

C#:   lock (gate) { shared++; }
来源：http://zeb.chenlongwang.top

[O04] 定义异步函数并等待
来源：http://oxe.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://waw.wangshuangyany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://djj.shzxlz.cn

JS:   async function f() { await g(); }
来源：http://wnd.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bpl.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jcd.sweek.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xfb.redwolf501.top

Ruby: # 用 Fiber 或 async gem
来源：http://vpo.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://zqg.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://tor.fanxiaobao.xyz

Py:   asyncio.gather(*tasks)
来源：http://oqc.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xsf.havefunace.top

JS:   await Promise.all(tasks)
来源：http://ysm.sweek.top

TS:   await Promise.all(tasks)
来源：http://pfd.tianlin.xyz


<!-- 参考信息 -->