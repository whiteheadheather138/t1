代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://ehm.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://hfq.jinyuanbaomall.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yho.snrcjt.cn

[L02] 发送 POST JSON
来源：http://rld.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://tth.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jie.vehdjk.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dws.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gou.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://moa.cucudq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wzn.zhengqikj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qyk.guannengcc.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dcx.cheryme.top

[L03] 设置自定义请求头
来源：http://mda.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fol.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vwu.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mei.hcnkem.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wfj.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dgu.jqgfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ytd.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://elw.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wuc.jqgufenzy.top

[L04] 设置超时
来源：http://tpy.hfpthk.cn

Py:   requests.get(url, timeout=5)
来源：http://icg.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dyk.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://har.fanxiaobao.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vcm.bjfxy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rel.sufxvd.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yzs.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jli.bbcook.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fum.nanxinkj.top

[L05] 上传文件（multipart）
来源：http://txf.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bsn.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ypt.yj202588.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://amp.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://shw.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rfn.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yaj.shzxlz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pbr.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sbk.meibo888.top

[L06] 解析响应为 JSON
来源：http://lhv.ywan-chungtsiang.top

Py:   resp.json()
来源：http://nif.haohaochexian.top

PHP:  json_decode($body, true);
来源：http://exn.fzhhl.top

JS:   await resp.json()
来源：http://pwx.wangdashe.top

TS:   await resp.json()
来源：http://pzy.guowangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oyi.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://skp.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://vpr.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lkz.vqdsnc.cn

[L07] 处理 HTTP 状态码
来源：http://rpa.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lgm.zhoulong.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vix.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://snp.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://mti.jinqigufen.top

Java: resp.statusCode()
来源：http://blo.zhengqikj.top

Go:   resp.StatusCode
来源：http://mbf.meibo888.top

Ruby: resp.code.to_i
来源：http://riz.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://dla.hysaishi.cn

[L08] 并发请求多个地址
来源：http://vuo.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vdi.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://vlr.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xna.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nwd.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wzl.yj202588.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mrr.xuetiantiany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wvf.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gsk.guannengcc.top

================================================================================
来源：http://irm.cashguo.top

M. 命令行 / 进程 / 环境
来源：http://eun.dianchejie.cn

================================================================================
来源：http://zff.sufxvd.cn

[M01] 读取命令行参数
来源：http://njc.nanxuanxn.top

Py:   sys.argv[1:]
来源：http://hfc.hnxiangtu.top

PHP:  $argv;  $argc;
来源：http://zyf.c1oappe.top

JS:   process.argv.slice(2)
来源：http://avq.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://whh.shanyushiyangkeji.top

Java: args 数组（main 方法参数）
来源：http://qug.chenlongwang.top

Go:   os.Args[1:]
来源：http://pmc.quarkkingdee.top

Ruby: ARGV
来源：http://cfs.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://ahv.zhoulong.xyz

[M02] 读取环境变量
来源：http://ldr.hammf.cn

Py:   os.environ.get("HOME")
来源：http://wll.hammf.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aqn.hammf.cn

JS:   process.env.HOME
来源：http://bhz.shuidangran.top

TS:   process.env.HOME
来源：http://uqd.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://zbw.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ekm.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://wqi.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vxu.sweek.top

[M03] 执行外部命令
来源：http://pka.zhengqikj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xpx.hongshengwenyu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://csh.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://lbf.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://bor.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ikd.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lzu.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://hqr.ydzc1.top

C#:   Process.Start("ls", "-l");
来源：http://bnm.gotoacloud.top

[M04] 获取当前工作目录
来源：http://gbr.quarkkingdee.top

Py:   os.getcwd()
来源：http://qtg.guowangkeji.top

PHP:  getcwd();
来源：http://awj.chenjidiqi.icu

JS:   process.cwd()
来源：http://jlg.bbcook.cn

TS:   process.cwd()
来源：http://nev.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://csm.daxiang520.top

Go:   os.Getwd()
来源：http://owo.hywenlv.cn

Ruby: Dir.pwd
来源：http://hmm.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://jhg.yangfankeji.com

[M05] 设置退出码
来源：http://zjo.ivvv.top

Py:   sys.exit(1)
来源：http://dgc.dianchejie.cn

PHP:  exit(1);
来源：http://arf.cdnleiting.top

JS:   process.exit(1)
来源：http://ddg.sufxvd.cn

TS:   process.exit(1)
来源：http://lbb.c1oappe.top

Java: System.exit(1)
来源：http://ciq.ybcxt.top

Go:   os.Exit(1)
来源：http://jbr.yj20258.top

Ruby: exit 1
来源：http://mwk.yj20258888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dje.vehdjk.com

[M06] 向标准错误输出
来源：http://yxb.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://vgq.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ctg.jinqigufen.top

JS:   console.error("err")
来源：http://mni.xziqi.cn

TS:   console.error("err")
来源：http://toh.ppjwa.cn

Java: System.err.println("err")
来源：http://ihp.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nxc.nanxuanxn.top

Ruby: warn "err"
来源：http://vfj.ehwqpu.com

C#:   Console.Error.WriteLine("err")
来源：http://ink.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://uyr.shangyingyoupin.top

Py:   if __name__ == "__main__":
来源：http://par.xuanzx.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uez.pengpengdd.cyou

JS:   require.main === module
来源：http://fnk.ydzc1.top

TS:   require.main === module
来源：http://wth.fehbvm.com

Java: public static void main(String[] args)
来源：http://toe.guowangkeji.top

Go:   func main()
来源：http://ccq.aibaodan.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ysd.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://lpx.cashguo.top

[M08] 获取系统与运行时信息
来源：http://bls.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://vpj.cheryme.top

PHP:  PHP_OS;  phpversion();
来源：http://gqf.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://vuw.cashguo.top

TS:   process.platform;  process.version
来源：http://lcr.redwolf501.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pok.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://clw.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wok.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://vnv.cucudq.cn

================================================================================
来源：http://ift.jinqigufen.top

N. 数据结构与算法
来源：http://kqh.dianchejie.cn

================================================================================
来源：http://cxr.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://gce.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://ksl.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vjw.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xjo.zhoulong.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dpd.nwbrower.top

Java: Arrays.binarySearch(arr, x)
来源：http://dyj.epnwcf.com

Go:   sort.SearchInts(arr, x)
来源：http://dfx.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://zsx.9152youxi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rla.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://uxo.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://paa.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eht.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://aor.bbcook.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wyj.shangyingyoupin.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gkb.yueranfly.top

Go:   slices.Sort(arr)
来源：http://eug.shanyushiyangtech.top

Ruby: arr.sort
来源：http://gpx.quarkkingdee.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://cjg.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://esc.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fuu.hnxiangtu.top

PHP:  // 递归实现，或用 usort
来源：http://zyy.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://spl.hysaishi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jqq.birdmap.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://khc.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uhw.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tbv.jinqigufen.top

C#:   // 手写递归，或 Array.Sort
来源：http://jnf.gogol.net.cn

[N04] 斐波那契数列
来源：http://uwt.hywenlv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ssn.ybcxt.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zlr.shuidangran.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uvb.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wix.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mdl.yuxming.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://faf.zdqjudy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pmp.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hjf.jyoumei.cn

[N05] 最大公约数
来源：http://bnh.jinqigufen.top

Py:   math.gcd(a, b)
来源：http://bhh.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://weo.gotoacloud.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cwb.sjlbkw.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xcz.andypj.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://guj.yongpay.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vee.sysykeji.top

Ruby: a.gcd(b)
来源：http://pll.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uud.vqdsnc.cn

[N06] 判断回文字符串
来源：http://gbz.jqgufenzy.top

Py:   s == s[::-1]
来源：http://eqe.xziqi.cn

PHP:  $s === strrev($s);
来源：http://ytw.zhaomingkeji.xyz

JS:   s === [...s].reverse().join("")
来源：http://fdo.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://vxn.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oqw.shanyushiyangkeji.top

Go:   // 双指针从两端比较
来源：http://iex.ydzc1.top

Ruby: s == s.reverse
来源：http://kxw.yvedp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mvs.jinghuilouyu.cn

[N07] 两数之和（返回下标）
来源：http://wdc.sufxvd.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://szk.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ptm.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://daz.feifeiyinyue.top

TS:   // 手写 Map<string, number>
来源：http://mil.mhx1999.top

Java: // 手写 HashMap
来源：http://rbo.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://eao.jinqigfzy.top

Ruby: // 手写 Hash
来源：http://luq.haohaochexian.top

C#:   // 手写 Dictionary<int, int>
来源：http://zlj.jiagoushi.top

[N08] 生成全排列
来源：http://jdk.zhaomingkeji.xyz

Py:   itertools.permutations(arr)
来源：http://lss.shzxlz.cn

PHP:  // 手写递归交换
来源：http://hie.tarul.cn

JS:   // 手写回溯递归
来源：http://rjs.jinqigufen.top

TS:   // 手写回溯递归
来源：http://szm.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://xjd.smart0.xyz

Go:   // 手写回溯递归
来源：http://szn.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://fje.vqdsnc.cn

C#:   // 手写回溯递归
来源：http://hea.ehwqpu.com

[N09] 栈与队列
来源：http://wmi.yangfankeji.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qms.jianghu66.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zzg.epnwcf.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fua.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aun.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://daq.yueranfly.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kmr.havefunace.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vzl.chenjidiqi.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ucf.jyoumei.cn

[N10] 链表节点定义
来源：http://zpd.sweek.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://luj.daxiang520.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ktq.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yby.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mjb.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://qiz.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://miv.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://kcy.gaohongyu789.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hlj.meibo888.top

[N11] 二叉树中序遍历
来源：http://lfr.52xcode.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ume.nwbrower.top

PHP:  // 手写递归函数
来源：http://myo.hysaishi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://whz.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kzn.cqqwz.cn

Java: // 手写递归
来源：http://mrv.xuetiantiany.cn

Go:   // 手写递归
来源：http://hzt.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sfy.yuanzhike.top

C#:   // 手写递归
来源：http://gsm.aizwys.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rsr.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zxe.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rrz.havefunace.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vzk.jlsjyb.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://muk.zhengqikj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nvi.gotoacloud.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ons.gotoacloud.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cfe.pengpengdd.cyou

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cpx.hysaishi.cn

================================================================================
来源：http://kvz.316326.xyz

O. 并发与异步
来源：http://sne.chenzaomai.com

================================================================================
来源：http://mme.jqgufenzy.top

[O01] 启动一个线程
来源：http://kbz.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://itj.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rtx.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ihh.uphjek.com

TS:   // 同 JS
来源：http://jbc.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://xtn.dianchejie.cn

Go:   go f()
来源：http://gni.zhengqikj.top

Ruby: Thread.new { f }
来源：http://teb.jiagoushi.top

C#:   Task.Run(() => F());
来源：http://akp.xuetiantiany.cn

[O02] 使用线程池
来源：http://ysk.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xmj.redwolf501.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gkb.svipenyu.cn

JS:   // worker_threads 线程池
来源：http://ktt.yanxiufei.cn

TS:   // worker_threads 线程池
来源：http://oye.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://anz.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hhw.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://div.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bgh.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://uim.gzhubu.top

Py:   with lock: shared += 1
来源：http://dcr.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://yhw.fengsongda.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wjo.cucudq.cn

TS:   // 同 JS
来源：http://hid.hcnkem.com

Java: synchronized (this) { shared++; }
来源：http://ing.cucudq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sbm.52xcode.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cjc.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://neq.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://kns.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://iqe.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mni.gogol.net.cn

JS:   async function f() { await g(); }
来源：http://zpo.hywenlv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pvb.sjlbkw.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ven.svipenyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pfc.yanxiufei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pcu.sxryk.cn

C#:   async Task F() { await G(); }
来源：http://xph.xingfuxueyuan.xyz

[O05] 并发执行并等待全部完成
来源：http://mot.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://wqn.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kyc.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://djk.sufxvd.cn

TS:   await Promise.all(tasks)
来源：http://ifp.guowangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://koi.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xqt.bbcook.cn

Ruby: threads.map(&:join)
来源：http://ood.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tgy.shuidangran.top


<!-- 参考信息 -->