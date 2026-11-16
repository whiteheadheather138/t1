代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zbf.dashuyun.cn

JS:   await fetch(url)
来源：http://owa.zhijiandao.cn

TS:   await fetch(url)
来源：http://lcd.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rss.svipenyu.cn

Go:   resp, err := http.Get(url)
来源：http://wmb.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lno.yj20258.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tdk.hywenlv.cn

[L02] 发送 POST JSON
来源：http://yvy.cqqwz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fwq.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://osc.pengpengdd.cyou

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kre.yfazqb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xgj.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ivl.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://old.shanyushiyangtech.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vuf.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dox.svipenyu.cn

[L03] 设置自定义请求头
来源：http://pbv.zhoulong.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zpk.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://twx.sufxvd.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jvt.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pqb.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bic.zdqjudy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hwz.vehdjk.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qtx.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ogt.gzhubu.top

[L04] 设置超时
来源：http://bci.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://xbl.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ata.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xfs.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hze.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mdu.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://myr.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fsv.52xcode.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ahk.sysykeji.top

[L05] 上传文件（multipart）
来源：http://ttj.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://olb.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gyw.jinghuilouyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jlx.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wmh.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aou.shuidangran.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hlp.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ybc.gotoacloud.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cxq.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://mwz.jqgfzy.top

Py:   resp.json()
来源：http://zox.sysykeji.top

PHP:  json_decode($body, true);
来源：http://qdz.jinqigufen.top

JS:   await resp.json()
来源：http://ltz.xylfe.cn

TS:   await resp.json()
来源：http://yim.xylfe.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vhe.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dza.ywan-chungtsiang.top

Ruby: JSON.parse(resp.body)
来源：http://fts.jqgfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dyo.jyoumei.cn

[L07] 处理 HTTP 状态码
来源：http://spj.tianlin.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dkt.nanxuanxn.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sqx.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://xis.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://spj.sweek.top

Java: resp.statusCode()
来源：http://zwg.c1oappe.top

Go:   resp.StatusCode
来源：http://dbd.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://nov.guowangkeji.top

C#:   (int)resp.StatusCode
来源：http://wmt.gotoacloud.top

[L08] 并发请求多个地址
来源：http://knx.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xmm.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://egu.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bxr.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iav.gzhubu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wza.yj20258.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ajv.sufxvd.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vlb.cdnleiting.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://azb.sufxvd.cn

================================================================================
来源：http://dyf.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://hck.tanke756.top

================================================================================
来源：http://qsx.cashguo.top

[M01] 读取命令行参数
来源：http://fqs.pycfn.com

Py:   sys.argv[1:]
来源：http://nfk.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://iho.jqgufenzy.top

JS:   process.argv.slice(2)
来源：http://img.aizwys.cn

TS:   process.argv.slice(2)
来源：http://web.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://fhl.c1oappe.top

Go:   os.Args[1:]
来源：http://mdo.xuetiantiany.cn

Ruby: ARGV
来源：http://nzc.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://lxj.yongpay.top

[M02] 读取环境变量
来源：http://sfl.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://azl.wangdashe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ohc.sufxvd.cn

JS:   process.env.HOME
来源：http://grl.ydjk.org.cn

TS:   process.env.HOME
来源：http://qgh.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://xji.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ecq.fanxiaobao.xyz

Ruby: ENV["HOME"]
来源：http://ynf.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oqb.zdbjq.cn

[M03] 执行外部命令
来源：http://qmi.zdbjq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pcv.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qls.cashguo.top

JS:   child_process.execSync("ls -l").toString()
来源：http://svo.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hel.jianghu66.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sxc.xingfuxueyuan.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://ops.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://org.jyoumei.cn

C#:   Process.Start("ls", "-l");
来源：http://pmg.redwolf501.top

[M04] 获取当前工作目录
来源：http://mmm.ivvv.top

Py:   os.getcwd()
来源：http://kwb.hongshengwenyu.top

PHP:  getcwd();
来源：http://oog.wangdashe.top

JS:   process.cwd()
来源：http://zvf.wangdashe.top

TS:   process.cwd()
来源：http://kba.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://pql.vehdjk.com

Go:   os.Getwd()
来源：http://tux.nwbrower.top

Ruby: Dir.pwd
来源：http://fem.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://vlc.hywenlv.cn

[M05] 设置退出码
来源：http://jnb.chenzaomai.com

Py:   sys.exit(1)
来源：http://hph.nwbrower.top

PHP:  exit(1);
来源：http://wgf.snrcjt.cn

JS:   process.exit(1)
来源：http://xcf.ppjwa.cn

TS:   process.exit(1)
来源：http://lbu.nanxuanxn.top

Java: System.exit(1)
来源：http://mhi.jlsjyb.cn

Go:   os.Exit(1)
来源：http://fdc.snrcjt.cn

Ruby: exit 1
来源：http://tzx.uphjek.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hhm.yj20258.top

[M06] 向标准错误输出
来源：http://cbi.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://ily.xuanzx.com

PHP:  fwrite(STDERR, "err\n");
来源：http://eou.xuanzx.com

JS:   console.error("err")
来源：http://qif.zycfv.cn

TS:   console.error("err")
来源：http://fzl.ybcxt.top

Java: System.err.println("err")
来源：http://wdk.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fjq.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://wmb.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://ewn.pengpengdd.cyou

[M07] 判断是否为主入口
来源：http://lyp.sweek.top

Py:   if __name__ == "__main__":
来源：http://rav.xziqi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mlg.quarkkingdee.top

JS:   require.main === module
来源：http://nli.chenlongwang.top

TS:   require.main === module
来源：http://eky.yueranfly.top

Java: public static void main(String[] args)
来源：http://mzh.shanyushiyangtech.top

Go:   func main()
来源：http://khd.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gck.fengsongda.top

C#:   static void Main(string[] args)
来源：http://sbo.sysykeji.top

[M08] 获取系统与运行时信息
来源：http://tsg.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://mhf.c1oappe.top

PHP:  PHP_OS;  phpversion();
来源：http://vnp.kuanghao11.cn

JS:   process.platform;  process.version
来源：http://ufd.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://jwo.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tdv.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hik.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dzv.yongpay.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://git.guannengcc.top

================================================================================
来源：http://fyy.tanke756.top

N. 数据结构与算法
来源：http://dwk.bbcook.cn

================================================================================
来源：http://dyd.hywenlv.cn

[N01] 二分查找（有序数组）
来源：http://qdp.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://hsc.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://job.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gnc.zhaomingkeji.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qtm.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://wvm.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://eig.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jsn.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://ibx.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://wje.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ipp.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://toc.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zld.dianchejie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vla.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lhj.sxryk.cn

Go:   slices.Sort(arr)
来源：http://kuh.bjfxy.top

Ruby: arr.sort
来源：http://vzg.xinyue.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://kpm.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://svm.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bvh.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://bgz.svipenyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fvn.guowangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nwo.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mpe.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://seu.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qxg.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://vtd.yj20258888.top

[N04] 斐波那契数列
来源：http://rja.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://drt.yj202588.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hbk.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rmc.xinyue.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hkx.xingfuxueyuan.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gur.zhongyouzk.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vvz.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ghu.epnwcf.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kff.xinyue.icu

[N05] 最大公约数
来源：http://wef.shzxlz.cn

Py:   math.gcd(a, b)
来源：http://dtb.jiagoushi.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jwf.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lzl.tianlin.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zye.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lup.daxiang520.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jpd.gogol.net.cn

Ruby: a.gcd(b)
来源：http://chg.yuxming.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pqz.dashuyun.cn

[N06] 判断回文字符串
来源：http://adb.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://epn.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://ywg.jyoumei.cn

JS:   s === [...s].reverse().join("")
来源：http://kyq.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://njl.yuxming.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jxj.cucudq.cn

Go:   // 双指针从两端比较
来源：http://per.xylfe.cn

Ruby: s == s.reverse
来源：http://lef.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bqw.hammf.cn

[N07] 两数之和（返回下标）
来源：http://ebe.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nmy.xinyue.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qfz.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jmz.sweek.top

TS:   // 手写 Map<string, number>
来源：http://vnw.fktsv.cn

Java: // 手写 HashMap
来源：http://oxt.ctjpmb.com

Go:   // 手写 map[int]int
来源：http://zfd.yvedp.cn

Ruby: // 手写 Hash
来源：http://nth.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://urk.yuanzhike.top

[N08] 生成全排列
来源：http://krb.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://ubg.yj20258.top

PHP:  // 手写递归交换
来源：http://ema.tianlin.xyz

JS:   // 手写回溯递归
来源：http://gcl.cdnleiting.top

TS:   // 手写回溯递归
来源：http://xhc.nwbrower.top

Java: // 手写回溯递归
来源：http://uvi.xylfe.cn

Go:   // 手写回溯递归
来源：http://fsf.tianlin.xyz

Ruby: arr.permutation.to_a
来源：http://wls.epnwcf.com

C#:   // 手写回溯递归
来源：http://acw.vehdjk.com

[N09] 栈与队列
来源：http://mlo.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zru.hywenlv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nft.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gld.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hjf.yanxiufei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bpr.haohaochexian.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nmo.shuidangran.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qyh.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oqf.zdbjq.cn

[N10] 链表节点定义
来源：http://hpv.gzhubu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sfr.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ibh.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rhw.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dnn.yj202588.top

Java: class Node { int v; Node next; }
来源：http://jwo.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://epz.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lmn.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ppd.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://cdy.guowangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bgf.wangdashe.top

PHP:  // 手写递归函数
来源：http://byw.vqdsnc.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ovd.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tlp.gogol.net.cn

Java: // 手写递归
来源：http://tto.pengpengdd.cyou

Go:   // 手写递归
来源：http://gqe.yj20258.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fbm.ybcxt.top

C#:   // 手写递归
来源：http://lkf.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://snw.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xsp.chenjidiqi.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cpu.ydjk.org.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kzl.fanxiaobao.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dwm.hcnkem.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://reu.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jmx.zhixingplan.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://njj.shangyingyoupin.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fpn.hcnkem.com

================================================================================
来源：http://tdj.xuetiantiany.cn

O. 并发与异步
来源：http://cwn.zhengqikj.top

================================================================================
来源：http://xjn.yuanzhike.top

[O01] 启动一个线程
来源：http://kad.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pap.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yfv.guowangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vmk.hywenlv.cn

TS:   // 同 JS
来源：http://usk.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://puf.kuanghao11.cn

Go:   go f()
来源：http://kja.ehwqpu.com

Ruby: Thread.new { f }
来源：http://xuh.yj20258.top

C#:   Task.Run(() => F());
来源：http://uzh.fehbvm.com

[O02] 使用线程池
来源：http://gel.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xcb.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mcz.fktsv.cn

JS:   // worker_threads 线程池
来源：http://xyv.yanxiufei.cn

TS:   // worker_threads 线程池
来源：http://ngr.bbcook.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lft.shanyushiyangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rzz.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dmy.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jzm.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://nch.xylfe.cn

Py:   with lock: shared += 1
来源：http://cwc.xziqi.cn

PHP:  // 用 flock() 做文件锁
来源：http://kmw.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eto.ybcxt.top

TS:   // 同 JS
来源：http://hna.bbcook.cn

Java: synchronized (this) { shared++; }
来源：http://ngc.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sbx.shanyushiyangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ezb.redwolf501.top

C#:   lock (gate) { shared++; }
来源：http://wlo.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://qsn.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://rtl.pycfn.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bns.xziqi.cn

JS:   async function f() { await g(); }
来源：http://paz.jinqigfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bbk.nanxinkj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://umn.havefunace.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qfj.yuxming.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xpx.zhiwuduotai.top

C#:   async Task F() { await G(); }
来源：http://ozs.ctjpmb.com

[O05] 并发执行并等待全部完成
来源：http://wlr.vqdsnc.cn

Py:   asyncio.gather(*tasks)
来源：http://ugf.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cmh.zhongyouzk.top

JS:   await Promise.all(tasks)
来源：http://zen.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://tcn.fehbvm.com


<!-- 参考信息 -->