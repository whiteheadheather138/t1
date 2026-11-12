代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ofc.svipenyu.cn

JS:   await fetch(url)
来源：http://kyc.wangdashe.top

TS:   await fetch(url)
来源：http://wjp.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oez.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://lqe.aibaodan.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zfo.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gxt.vehdjk.com

[L02] 发送 POST JSON
来源：http://rnr.aizwys.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hba.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fsn.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://smo.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yqo.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kyd.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jrg.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dru.iojbl.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xve.yvedp.cn

[L03] 设置自定义请求头
来源：http://xbv.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bma.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ngm.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nsj.aizwys.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://afh.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ufb.ydjk.org.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aqf.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sgp.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cgx.wangdashe.top

[L04] 设置超时
来源：http://waw.shzxlz.cn

Py:   requests.get(url, timeout=5)
来源：http://qit.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hrq.epnwcf.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rxx.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rrr.snrcjt.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mxx.cdnleiting.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kyt.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://woa.hfpthk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yzu.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://ysg.316326.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cuh.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wqb.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qzx.hesvh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ghw.hnxiangtu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://laz.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ygt.quarkkingdee.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eeb.xziqi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iqb.uphjek.com

[L06] 解析响应为 JSON
来源：http://lfg.yj202588.top

Py:   resp.json()
来源：http://uwo.meibo888.top

PHP:  json_decode($body, true);
来源：http://grz.guowangkeji.top

JS:   await resp.json()
来源：http://xle.gotoacloud.top

TS:   await resp.json()
来源：http://ioq.zhoulong.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://daa.hywenlv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ygs.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://jbw.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://get.jinyuanbaomall.cn

[L07] 处理 HTTP 状态码
来源：http://cpz.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://whp.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://idd.gzhubu.top

JS:   resp.ok;  resp.status
来源：http://fmh.yongpay.top

TS:   resp.ok;  resp.status
来源：http://dac.gogol.net.cn

Java: resp.statusCode()
来源：http://rdi.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://end.sysykeji.top

Ruby: resp.code.to_i
来源：http://ptz.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://fkw.yongpay.top

[L08] 并发请求多个地址
来源：http://lpy.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tql.yuxming.cn

PHP:  curl_multi_init() 系列
来源：http://jvz.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uia.ctjpmb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dws.hnqzz.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wtj.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xef.guannengcc.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tev.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nnu.yanxiufei.cn

================================================================================
来源：http://llx.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://qyo.yj20258888.top

================================================================================
来源：http://yul.jinqigfzy.top

[M01] 读取命令行参数
来源：http://uxx.yangfankeji.com

Py:   sys.argv[1:]
来源：http://dfk.cheryme.top

PHP:  $argv;  $argc;
来源：http://gng.hammf.cn

JS:   process.argv.slice(2)
来源：http://aqg.guannengcc.top

TS:   process.argv.slice(2)
来源：http://pvh.cqqwz.cn

Java: args 数组（main 方法参数）
来源：http://ogn.haohaochexian.top

Go:   os.Args[1:]
来源：http://eby.daxiang520.top

Ruby: ARGV
来源：http://cpo.jinqigufen.top

C#:   args 数组（Main 方法参数）
来源：http://sdh.yj20258888.top

[M02] 读取环境变量
来源：http://fze.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://mfb.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://irt.yfazqb.com

JS:   process.env.HOME
来源：http://qsz.andypj.xyz

TS:   process.env.HOME
来源：http://fcd.zhoulong.xyz

Java: System.getenv("HOME")
来源：http://zcz.smart0.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jqu.hnxiangtu.top

Ruby: ENV["HOME"]
来源：http://osf.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mhh.sufxvd.cn

[M03] 执行外部命令
来源：http://kgm.jinghuilouyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vpe.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dcu.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://xhd.zhaomingkeji.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://fyp.xuetiantiany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://brl.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lnd.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://gng.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://duo.jqgfzy.top

[M04] 获取当前工作目录
来源：http://utr.hammf.cn

Py:   os.getcwd()
来源：http://hxl.yonumen.top

PHP:  getcwd();
来源：http://wvy.uphjek.com

JS:   process.cwd()
来源：http://tfe.gotoacloud.top

TS:   process.cwd()
来源：http://qek.jqgfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://mov.xziqi.cn

Go:   os.Getwd()
来源：http://tpy.jyoumei.cn

Ruby: Dir.pwd
来源：http://yki.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fxo.wangdashe.top

[M05] 设置退出码
来源：http://ctn.tarul.cn

Py:   sys.exit(1)
来源：http://daz.nanxinkj.top

PHP:  exit(1);
来源：http://pqv.yj20258888.top

JS:   process.exit(1)
来源：http://yva.jqgfzy.top

TS:   process.exit(1)
来源：http://rss.hywenlv.cn

Java: System.exit(1)
来源：http://loq.hywenlv.cn

Go:   os.Exit(1)
来源：http://zpk.fengsongda.top

Ruby: exit 1
来源：http://ekb.jiagoushi.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cia.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://fuc.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://wsi.meibo888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://svq.haohaochexian.top

JS:   console.error("err")
来源：http://ekm.zhengqikj.top

TS:   console.error("err")
来源：http://wba.wangshuangyany.cn

Java: System.err.println("err")
来源：http://waz.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://axn.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://ivq.yvedp.cn

C#:   Console.Error.WriteLine("err")
来源：http://edj.hcnkem.com

[M07] 判断是否为主入口
来源：http://imx.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://raa.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://psq.316326.xyz

JS:   require.main === module
来源：http://bxl.daria6918.cn

TS:   require.main === module
来源：http://qet.fktsv.cn

Java: public static void main(String[] args)
来源：http://gwx.sweek.top

Go:   func main()
来源：http://ibd.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ixd.nwbrower.top

C#:   static void Main(string[] args)
来源：http://ecr.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://pjx.svipenyu.cn

Py:   platform.system();  platform.python_version()
来源：http://bey.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://npf.sxryk.cn

JS:   process.platform;  process.version
来源：http://xba.dianchejie.cn

TS:   process.platform;  process.version
来源：http://cjr.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cju.jiagoushi.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kgf.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://udk.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gfo.nwbrower.top

================================================================================
来源：http://dfn.guannengcc.top

N. 数据结构与算法
来源：http://yre.yanxiufei.cn

================================================================================
来源：http://wrd.cashguo.top

[N01] 二分查找（有序数组）
来源：http://rbl.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://eap.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qvo.jinqigufen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hmk.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zrb.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://gld.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://ply.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://niz.xylfe.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hei.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://yrz.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://gsc.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ket.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mpf.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gxa.tianlin.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dfy.shanyushiyangkeji.top

Go:   slices.Sort(arr)
来源：http://yrn.zdbjq.cn

Ruby: arr.sort
来源：http://hdf.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://nhn.guannengcc.top

[N03] 快速排序（分治示例）
来源：http://srq.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mjh.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://lvq.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lzb.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rkj.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pvc.yongpay.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://luv.hywenlv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wtg.hongshengwenyu.top

C#:   // 手写递归，或 Array.Sort
来源：http://ulm.zhengqikj.top

[N04] 斐波那契数列
来源：http://okv.pycfn.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pgb.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iex.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pnl.chenjidiqi.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fdm.chenzaomai.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vaw.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fmp.zhengqikj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yjy.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xng.redwolf501.top

[N05] 最大公约数
来源：http://pqm.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://ehk.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wjr.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://etc.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zsg.jiagoushi.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wzm.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://smu.vehdjk.com

Ruby: a.gcd(b)
来源：http://ltz.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qvq.hywenlv.cn

[N06] 判断回文字符串
来源：http://xvh.zhoulong.xyz

Py:   s == s[::-1]
来源：http://zne.hywenlv.cn

PHP:  $s === strrev($s);
来源：http://wxs.nanxinkj.top

JS:   s === [...s].reverse().join("")
来源：http://sdi.cqqwz.cn

TS:   s === [...s].reverse().join("")
来源：http://icb.hnqzz.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uiq.yj20258888.top

Go:   // 双指针从两端比较
来源：http://pzk.sjlbkw.cn

Ruby: s == s.reverse
来源：http://rtv.ctjpmb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://flf.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://gxu.52xcode.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tlk.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://upg.cqqwz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xks.cashguo.top

TS:   // 手写 Map<string, number>
来源：http://vsv.vqdsnc.cn

Java: // 手写 HashMap
来源：http://rfn.9152youxi.cn

Go:   // 手写 map[int]int
来源：http://ejs.zhaomingkeji.xyz

Ruby: // 手写 Hash
来源：http://bum.yanxiufei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://brw.vehdjk.com

[N08] 生成全排列
来源：http://nwy.aibaodan.cn

Py:   itertools.permutations(arr)
来源：http://yon.hywenlv.cn

PHP:  // 手写递归交换
来源：http://ugr.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://nzd.meibo888.top

TS:   // 手写回溯递归
来源：http://hgo.zdbjq.cn

Java: // 手写回溯递归
来源：http://wbj.feifeiyinyue.top

Go:   // 手写回溯递归
来源：http://ldn.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://mhd.pycfn.com

C#:   // 手写回溯递归
来源：http://abu.yonumen.top

[N09] 栈与队列
来源：http://zex.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://olt.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cri.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qzz.ybcxt.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qrh.yanxiufei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bks.hongshengwenyu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dyz.aibaodan.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gji.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wfv.ydjk.org.cn

[N10] 链表节点定义
来源：http://pcz.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dpl.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lur.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dhu.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vey.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://zwz.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://ccn.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qdw.xinyue.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://cnx.yvedp.cn

[N11] 二叉树中序遍历
来源：http://mhl.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ehl.0kj1m.cn

PHP:  // 手写递归函数
来源：http://vsa.chenjidiqi.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rgk.yfazqb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fru.sweek.top

Java: // 手写递归
来源：http://ofl.wangshuangyany.cn

Go:   // 手写递归
来源：http://ieo.tian-w.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wkb.daxiang520.top

C#:   // 手写递归
来源：http://oke.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ccj.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://emu.pycfn.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oia.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fpj.ctjpmb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://knw.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uni.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xjh.bbcook.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wba.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://llh.kuanghao11.cn

================================================================================
来源：http://fbr.yvedp.cn

O. 并发与异步
来源：http://vpx.shangyingyoupin.top

================================================================================
来源：http://xhd.hammf.cn

[O01] 启动一个线程
来源：http://sfn.wangdashe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pny.yueranfly.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jlc.havefunace.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://drq.316326.xyz

TS:   // 同 JS
来源：http://wpz.hfpthk.cn

Java: new Thread(() -> f()).start()
来源：http://jiw.yangfankeji.com

Go:   go f()
来源：http://inx.shanyushiyangtech.top

Ruby: Thread.new { f }
来源：http://dpq.ctjpmb.com

C#:   Task.Run(() => F());
来源：http://kdq.uphjek.com

[O02] 使用线程池
来源：http://siw.jinqigufen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qtd.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hcs.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://ecs.birdmap.top

TS:   // worker_threads 线程池
来源：http://iep.jyoumei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zam.zhengqikj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wso.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ynz.yvedp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xso.bbcook.cn

[O03] 加锁保护共享数据
来源：http://yzh.shanyushiyangtech.top

Py:   with lock: shared += 1
来源：http://mgx.zycfv.cn

PHP:  // 用 flock() 做文件锁
来源：http://zdf.gotoacloud.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kro.yfazqb.com

TS:   // 同 JS
来源：http://hre.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://cyh.shangyingyoupin.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://svf.jinqigufen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qub.yueranfly.top

C#:   lock (gate) { shared++; }
来源：http://rxv.cucudq.cn

[O04] 定义异步函数并等待
来源：http://lvl.xuanzx.com

Py:   async def f():⏎    await g()
来源：http://cka.dashuyun.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hqu.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://bsb.wangshuangyany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://etq.pengpengdd.cyou

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sga.andypj.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wtx.jlsjyb.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wno.feifeiyinyue.top

C#:   async Task F() { await G(); }
来源：http://tjh.svipenyu.cn

[O05] 并发执行并等待全部完成
来源：http://yuc.nanxuanxn.top

Py:   asyncio.gather(*tasks)
来源：http://qbo.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hhr.gotoacloud.top

JS:   await Promise.all(tasks)
来源：http://loi.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://umn.shzxlz.cn


<!-- 参考信息 -->