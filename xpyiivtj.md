代发 wailian999

L. 网络请求
来源：http://gvb.pycfn.com

================================================================================
来源：http://ytr.fzhhl.top

[L01] 发送 GET 请求
来源：http://ipe.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fzv.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vnb.gzhubu.top

JS:   await fetch(url)
来源：http://hsd.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://ugk.shzxlz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://exn.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://imc.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://pej.wangdashe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://msp.aizwys.cn

[L02] 发送 POST JSON
来源：http://vjj.fzhhl.top

Py:   requests.post(url, json={"a": 1})
来源：http://jpe.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bwt.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jol.jinqigufen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jxu.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ixk.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jwe.cheryme.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bxn.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wyq.0kj1m.cn

[L03] 设置自定义请求头
来源：http://xvw.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jsv.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xca.yuxming.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dmx.tanke756.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mvm.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gvq.xziqi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hxj.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fyf.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iik.fehbvm.com

[L04] 设置超时
来源：http://jdy.tanke756.top

Py:   requests.get(url, timeout=5)
来源：http://fok.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qrq.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ncs.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bsn.cashguo.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wie.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://onh.xingfuxueyuan.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dlm.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xun.yonumen.top

[L05] 上传文件（multipart）
来源：http://zkl.chenjidiqi.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lcf.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iwu.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dfo.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mjs.zycfv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eux.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tan.jinghuilouyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gkg.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jmr.ivvv.top

[L06] 解析响应为 JSON
来源：http://ybe.sysykeji.top

Py:   resp.json()
来源：http://eyj.jqgfzy.top

PHP:  json_decode($body, true);
来源：http://vaa.sufxvd.cn

JS:   await resp.json()
来源：http://pev.zhengqikj.top

TS:   await resp.json()
来源：http://kvd.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vzw.redwolf501.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pph.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://ypq.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zri.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://gsw.yueranfly.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qwk.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ada.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://lxt.0kj1m.cn

TS:   resp.ok;  resp.status
来源：http://lip.fktsv.cn

Java: resp.statusCode()
来源：http://dql.zhoulong.xyz

Go:   resp.StatusCode
来源：http://scf.ivvv.top

Ruby: resp.code.to_i
来源：http://pmh.chenzaomai.com

C#:   (int)resp.StatusCode
来源：http://nkm.havefunace.top

[L08] 并发请求多个地址
来源：http://bro.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pnx.ywan-chungtsiang.top

PHP:  curl_multi_init() 系列
来源：http://lrd.fengsongda.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kre.redwolf501.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ktv.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jpj.shuidangran.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://apt.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kwv.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qxw.redwolf501.top

================================================================================
来源：http://jxy.hammf.cn

M. 命令行 / 进程 / 环境
来源：http://ldw.hammf.cn

================================================================================
来源：http://uev.ivvv.top

[M01] 读取命令行参数
来源：http://fvg.cqqwz.cn

Py:   sys.argv[1:]
来源：http://azc.bbcook.cn

PHP:  $argv;  $argc;
来源：http://fro.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://rms.bbcook.cn

TS:   process.argv.slice(2)
来源：http://rbu.yuanzhike.top

Java: args 数组（main 方法参数）
来源：http://pes.shanyushiyangtech.top

Go:   os.Args[1:]
来源：http://pcd.zhijiandao.cn

Ruby: ARGV
来源：http://xjd.zhoulong.xyz

C#:   args 数组（Main 方法参数）
来源：http://acl.jinyuanbaomall.cn

[M02] 读取环境变量
来源：http://njg.bjfxy.top

Py:   os.environ.get("HOME")
来源：http://oiu.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mni.xinyue.icu

JS:   process.env.HOME
来源：http://mqw.snrcjt.cn

TS:   process.env.HOME
来源：http://qip.ybcxt.top

Java: System.getenv("HOME")
来源：http://hsx.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ddp.jqgfzy.top

Ruby: ENV["HOME"]
来源：http://foo.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vkn.daxiang520.top

[M03] 执行外部命令
来源：http://jxw.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qer.shzxlz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://htq.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fey.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://iqm.chenzaomai.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hse.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tcz.zhixingplan.top

Ruby: system("ls -l");  `ls -l`
来源：http://oza.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://rbu.redwolf501.top

[M04] 获取当前工作目录
来源：http://zhn.zhaomingkeji.xyz

Py:   os.getcwd()
来源：http://uui.yvedp.cn

PHP:  getcwd();
来源：http://qgk.fanxiaobao.xyz

JS:   process.cwd()
来源：http://hqg.haohaochexian.top

TS:   process.cwd()
来源：http://tnz.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://wiz.fktsv.cn

Go:   os.Getwd()
来源：http://cns.dashuyun.cn

Ruby: Dir.pwd
来源：http://nfo.zdbjq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pkw.iojbl.cn

[M05] 设置退出码
来源：http://fbc.daria6918.cn

Py:   sys.exit(1)
来源：http://oof.tianlin.xyz

PHP:  exit(1);
来源：http://aze.nwbrower.top

JS:   process.exit(1)
来源：http://jqo.hcnkem.com

TS:   process.exit(1)
来源：http://yuq.havefunace.top

Java: System.exit(1)
来源：http://fjj.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://gzq.yj202588.top

Ruby: exit 1
来源：http://dul.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vws.guannengcc.top

[M06] 向标准错误输出
来源：http://tri.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://eiw.yonumen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gpq.havefunace.top

JS:   console.error("err")
来源：http://kcs.chenjidiqi.icu

TS:   console.error("err")
来源：http://uge.hcnkem.com

Java: System.err.println("err")
来源：http://oce.c1oappe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kyh.vehdjk.com

Ruby: warn "err"
来源：http://iui.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://sap.shangyingyoupin.top

[M07] 判断是否为主入口
来源：http://xvw.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://umf.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qen.hnqzz.top

JS:   require.main === module
来源：http://qav.zhixingplan.top

TS:   require.main === module
来源：http://vxc.tanke756.top

Java: public static void main(String[] args)
来源：http://nuz.jinqigufen.top

Go:   func main()
来源：http://upg.daxiang520.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pkk.yj20258888.top

C#:   static void Main(string[] args)
来源：http://rtd.meibo888.top

[M08] 获取系统与运行时信息
来源：http://kpp.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://tfn.zhiwuduotai.top

PHP:  PHP_OS;  phpversion();
来源：http://cym.ybcxt.top

JS:   process.platform;  process.version
来源：http://hii.jinyuanbaomall.cn

TS:   process.platform;  process.version
来源：http://sfr.yongpay.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jmy.yuxming.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wol.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pcj.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://idv.kuanghao11.cn

================================================================================
来源：http://uyw.hfpthk.cn

N. 数据结构与算法
来源：http://jvk.ybcxt.top

================================================================================
来源：http://wtz.svipenyu.cn

[N01] 二分查找（有序数组）
来源：http://ohm.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://rsc.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cbu.redwolf501.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fsj.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cbw.birdmap.top

Java: Arrays.binarySearch(arr, x)
来源：http://gta.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://huk.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vjw.smart0.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://gmo.yuanzhike.top

[N02] 排序（工程实践用内置实现）
来源：http://tyo.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://hce.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wga.zhixingplan.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://noc.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mib.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iwl.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://oww.yvedp.cn

Ruby: arr.sort
来源：http://ojv.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tvv.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://qqs.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wuk.fengsongda.top

PHP:  // 递归实现，或用 usort
来源：http://opp.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vtw.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zpa.mhx1999.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iql.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tev.316326.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bxk.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://htc.hywenlv.cn

[N04] 斐波那契数列
来源：http://hax.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://chc.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hfd.gogol.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fat.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wbs.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cbw.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://npq.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yew.yangfankeji.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bhr.jlsjyb.cn

[N05] 最大公约数
来源：http://wtw.havefunace.top

Py:   math.gcd(a, b)
来源：http://vnv.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://byq.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mei.ywan-chungtsiang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pss.fzhhl.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zvj.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oqi.ppjwa.cn

Ruby: a.gcd(b)
来源：http://eyc.chenjidiqi.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hat.guowangkeji.top

[N06] 判断回文字符串
来源：http://gqc.aizwys.cn

Py:   s == s[::-1]
来源：http://dxp.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://qkd.shuidangran.top

JS:   s === [...s].reverse().join("")
来源：http://rxb.jinqigfzy.top

TS:   s === [...s].reverse().join("")
来源：http://zju.hnqzz.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zvr.zhengqikj.top

Go:   // 双指针从两端比较
来源：http://vtp.shanyushiyangkeji.top

Ruby: s == s.reverse
来源：http://mcc.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uvi.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://heg.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qhx.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qsj.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rho.zhaomingkeji.xyz

TS:   // 手写 Map<string, number>
来源：http://ntg.zhijiandao.cn

Java: // 手写 HashMap
来源：http://mgn.yfazqb.com

Go:   // 手写 map[int]int
来源：http://qcf.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://tuo.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vdj.daria6918.cn

[N08] 生成全排列
来源：http://dld.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://pzs.jinyuanbaomall.cn

PHP:  // 手写递归交换
来源：http://icg.yongpay.top

JS:   // 手写回溯递归
来源：http://mmk.hcnkem.com

TS:   // 手写回溯递归
来源：http://otu.jinqigfzy.top

Java: // 手写回溯递归
来源：http://uam.redwolf501.top

Go:   // 手写回溯递归
来源：http://vcn.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://dmb.bjfxy.top

C#:   // 手写回溯递归
来源：http://anb.ydzc1.top

[N09] 栈与队列
来源：http://tez.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mkt.nwbrower.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://obw.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rjg.yuanzhike.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qfz.cqqwz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dmf.zhaomingkeji.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cpy.tian-w.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://teo.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qdn.snrcjt.cn

[N10] 链表节点定义
来源：http://tum.shuidangran.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://urc.ybcxt.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tkd.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lfm.bjfxy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jzt.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://zll.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://lfu.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dud.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://zgd.snrcjt.cn

[N11] 二叉树中序遍历
来源：http://qee.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qxf.daxiang520.top

PHP:  // 手写递归函数
来源：http://gez.cashguo.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jjt.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zgu.zhixingplan.top

Java: // 手写递归
来源：http://txu.zycfv.cn

Go:   // 手写递归
来源：http://nng.shangyingyoupin.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qrq.wangshuangyany.cn

C#:   // 手写递归
来源：http://wqb.zhiwuduotai.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xnm.yueranfly.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rkf.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://raw.gogol.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kcr.52xcode.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ros.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rgs.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sqg.shzxlz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yqj.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xmn.guannengcc.top

================================================================================
来源：http://vej.ehwqpu.com

O. 并发与异步
来源：http://voe.guowangkeji.top

================================================================================
来源：http://dwm.52xcode.cn

[O01] 启动一个线程
来源：http://nax.yangfankeji.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mpq.ydzc1.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://czk.birdmap.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kur.ybcxt.top

TS:   // 同 JS
来源：http://ngw.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://oou.shzxlz.cn

Go:   go f()
来源：http://wiy.yfazqb.com

Ruby: Thread.new { f }
来源：http://ttg.pengpengdd.cyou

C#:   Task.Run(() => F());
来源：http://cey.zhijiandao.cn

[O02] 使用线程池
来源：http://reh.zdqjudy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fnp.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://stc.shzxlz.cn

JS:   // worker_threads 线程池
来源：http://qwm.yongpay.top

TS:   // worker_threads 线程池
来源：http://loe.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://emh.yj20258888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vpv.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ejx.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fqx.shanyushiyangtech.top

[O03] 加锁保护共享数据
来源：http://smr.yj20258.top

Py:   with lock: shared += 1
来源：http://avs.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://qca.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ork.jinqigufen.top

TS:   // 同 JS
来源：http://zfb.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://ejn.zhiwuduotai.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cax.jqgfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ruy.cqqwz.cn

C#:   lock (gate) { shared++; }
来源：http://tkx.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://org.epnwcf.com

Py:   async def f():⏎    await g()
来源：http://men.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pkr.birdmap.top

JS:   async function f() { await g(); }
来源：http://hed.tian-w.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gwe.jinghuilouyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uoe.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://snm.dianchejie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qxi.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://sut.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://xzp.pengpengdd.cyou


<!-- 参考信息 -->