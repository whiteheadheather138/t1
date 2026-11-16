代发 wailian999

L. 网络请求
来源：http://qcg.ivvv.top

================================================================================
来源：http://kbz.fzhhl.top

[L01] 发送 GET 请求
来源：http://jjs.yuxming.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nnc.zdqjudy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vsl.c1oappe.top

JS:   await fetch(url)
来源：http://cke.hnxiangtu.top

TS:   await fetch(url)
来源：http://bhy.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ama.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://btb.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ble.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rll.shuidangran.top

[L02] 发送 POST JSON
来源：http://iuj.jqgufenzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://atb.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rif.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cdk.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gje.jiagoushi.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cqa.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aqd.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gvb.svipenyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ojn.tarul.cn

[L03] 设置自定义请求头
来源：http://gnp.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://evv.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vkw.dashuyun.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pel.fanxiaobao.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mhw.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://imm.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ymf.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kyk.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yso.zhoulong.xyz

[L04] 设置超时
来源：http://vyv.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://gwn.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://knf.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hoq.ehwqpu.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yud.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ewr.ywan-chungtsiang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fzx.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ktz.daria6918.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zvb.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://nbt.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bgm.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oqu.tianlin.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wyr.sufxvd.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://psy.mhx1999.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bvf.hnxiangtu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gzy.hywenlv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zzj.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dzz.xylfe.cn

[L06] 解析响应为 JSON
来源：http://usm.fengsongda.top

Py:   resp.json()
来源：http://frf.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://viy.yongpay.top

JS:   await resp.json()
来源：http://amn.svipenyu.cn

TS:   await resp.json()
来源：http://itu.hysaishi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nka.daria6918.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://arq.nwbrower.top

Ruby: JSON.parse(resp.body)
来源：http://von.hammf.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sll.wangshuangyany.cn

[L07] 处理 HTTP 状态码
来源：http://yti.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tbb.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://txy.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://vga.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://zzn.gotoacloud.top

Java: resp.statusCode()
来源：http://srg.vehdjk.com

Go:   resp.StatusCode
来源：http://ktu.316326.xyz

Ruby: resp.code.to_i
来源：http://haj.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://amb.tanke756.top

[L08] 并发请求多个地址
来源：http://aog.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fxz.yangfankeji.com

PHP:  curl_multi_init() 系列
来源：http://xxj.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ukl.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rze.ybcxt.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jyi.9152youxi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gqi.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sby.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bjx.xuanzx.com

================================================================================
来源：http://yim.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://xli.gotoacloud.top

================================================================================
来源：http://zex.xylfe.cn

[M01] 读取命令行参数
来源：http://tsg.fktsv.cn

Py:   sys.argv[1:]
来源：http://ynj.shangyingyoupin.top

PHP:  $argv;  $argc;
来源：http://hbv.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://otb.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://muz.zhaomingkeji.xyz

Java: args 数组（main 方法参数）
来源：http://pxd.tanke756.top

Go:   os.Args[1:]
来源：http://urw.tianlin.xyz

Ruby: ARGV
来源：http://ihl.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://yqi.cashguo.top

[M02] 读取环境变量
来源：http://vuw.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://eov.pengpengdd.cyou

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eex.dianchejie.cn

JS:   process.env.HOME
来源：http://pml.yj202588.top

TS:   process.env.HOME
来源：http://ebp.vehdjk.com

Java: System.getenv("HOME")
来源：http://wjw.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dte.chenjidiqi.icu

Ruby: ENV["HOME"]
来源：http://nvj.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vkc.aizwys.cn

[M03] 执行外部命令
来源：http://tsv.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tvd.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mjl.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jnr.52xcode.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ofj.sjlbkw.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://svn.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zwl.tianlin.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://tdx.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://dqb.sxryk.cn

[M04] 获取当前工作目录
来源：http://byv.guannengcc.top

Py:   os.getcwd()
来源：http://ysm.vehdjk.com

PHP:  getcwd();
来源：http://fzx.shuidangran.top

JS:   process.cwd()
来源：http://wsy.yfazqb.com

TS:   process.cwd()
来源：http://tjg.gogol.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://akj.sysykeji.top

Go:   os.Getwd()
来源：http://del.vehdjk.com

Ruby: Dir.pwd
来源：http://jzh.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://oyo.vehdjk.com

[M05] 设置退出码
来源：http://wyy.smart0.xyz

Py:   sys.exit(1)
来源：http://yqk.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://xws.ppjwa.cn

JS:   process.exit(1)
来源：http://sdr.meibo888.top

TS:   process.exit(1)
来源：http://zep.9152youxi.cn

Java: System.exit(1)
来源：http://zhz.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://viy.xuetiantiany.cn

Ruby: exit 1
来源：http://bnq.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pnw.iojbl.cn

[M06] 向标准错误输出
来源：http://qcr.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://kjy.vqdsnc.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cut.hcnkem.com

JS:   console.error("err")
来源：http://bfn.ywan-chungtsiang.top

TS:   console.error("err")
来源：http://gwu.havefunace.top

Java: System.err.println("err")
来源：http://xcs.guowangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qhm.gotoacloud.top

Ruby: warn "err"
来源：http://qee.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://jke.dianchejie.cn

[M07] 判断是否为主入口
来源：http://udi.cashguo.top

Py:   if __name__ == "__main__":
来源：http://ehy.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://alo.yj202588.top

JS:   require.main === module
来源：http://hrx.zycfv.cn

TS:   require.main === module
来源：http://zzo.gotoacloud.top

Java: public static void main(String[] args)
来源：http://ulp.nanxuanxn.top

Go:   func main()
来源：http://sgu.jianghu66.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jbr.cashguo.top

C#:   static void Main(string[] args)
来源：http://fkb.zhoulong.xyz

[M08] 获取系统与运行时信息
来源：http://rwj.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://xmb.ehwqpu.com

PHP:  PHP_OS;  phpversion();
来源：http://vcj.zdqjudy.top

JS:   process.platform;  process.version
来源：http://bxi.sxryk.cn

TS:   process.platform;  process.version
来源：http://rxk.zycfv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gtv.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ipp.jiagoushi.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xaj.kuanghao11.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sgb.zhaomingkeji.xyz

================================================================================
来源：http://hqh.jqgfzy.top

N. 数据结构与算法
来源：http://zei.hnqzz.top

================================================================================
来源：http://uoh.jinyuanbaomall.cn

[N01] 二分查找（有序数组）
来源：http://pme.tian-w.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eeb.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nyf.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kim.fehbvm.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pyy.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://pmq.zhijiandao.cn

Go:   sort.SearchInts(arr, x)
来源：http://leo.52xcode.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jsd.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://vpp.quarkkingdee.top

[N02] 排序（工程实践用内置实现）
来源：http://cfc.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://tgu.cashguo.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rsd.xziqi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uww.chenjidiqi.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://teg.cheryme.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kiz.ivvv.top

Go:   slices.Sort(arr)
来源：http://shk.hnxiangtu.top

Ruby: arr.sort
来源：http://rki.dashuyun.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://iai.fktsv.cn

[N03] 快速排序（分治示例）
来源：http://oab.yanxiufei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xto.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://fml.gzhubu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jll.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tmi.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oci.yongpay.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pkv.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://upz.shanyushiyangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://wlb.shangyingyoupin.top

[N04] 斐波那契数列
来源：http://lqv.shzxlz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bkb.yj202588.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kwk.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tjk.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ebt.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fpd.tianlin.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sry.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zmf.xziqi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kiy.hfpthk.cn

[N05] 最大公约数
来源：http://owm.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://xpc.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fef.yj202588.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vro.sysykeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xrp.aibaodan.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zpb.gzhubu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oiv.cqqwz.cn

Ruby: a.gcd(b)
来源：http://prx.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ppv.jinghuilouyu.cn

[N06] 判断回文字符串
来源：http://stb.ehwqpu.com

Py:   s == s[::-1]
来源：http://mdf.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://aea.nanxinkj.top

JS:   s === [...s].reverse().join("")
来源：http://byh.vqdsnc.cn

TS:   s === [...s].reverse().join("")
来源：http://vbk.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kmu.pycfn.com

Go:   // 双指针从两端比较
来源：http://vzz.jlsjyb.cn

Ruby: s == s.reverse
来源：http://nyl.xylfe.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xhf.zycfv.cn

[N07] 两数之和（返回下标）
来源：http://nay.ivvv.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ptz.fktsv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vtw.ybcxt.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qjq.xuetiantiany.cn

TS:   // 手写 Map<string, number>
来源：http://rpd.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://sxh.yvedp.cn

Go:   // 手写 map[int]int
来源：http://seu.daria6918.cn

Ruby: // 手写 Hash
来源：http://vbh.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fts.zhaomingkeji.xyz

[N08] 生成全排列
来源：http://rjq.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://eoq.andypj.xyz

PHP:  // 手写递归交换
来源：http://lbz.hywenlv.cn

JS:   // 手写回溯递归
来源：http://hao.yuxming.cn

TS:   // 手写回溯递归
来源：http://gml.xuanzx.com

Java: // 手写回溯递归
来源：http://wjj.cqqwz.cn

Go:   // 手写回溯递归
来源：http://kbs.hysaishi.cn

Ruby: arr.permutation.to_a
来源：http://utd.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://kbj.jinqigufen.top

[N09] 栈与队列
来源：http://xaj.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ozq.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oih.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wkp.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iup.fengsongda.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pzq.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xsx.yongpay.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hip.zycfv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vlh.dianchejie.cn

[N10] 链表节点定义
来源：http://pis.chenzaomai.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zuu.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://plf.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bhw.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vpm.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://xri.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://udy.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://trb.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xce.zhijiandao.cn

[N11] 二叉树中序遍历
来源：http://ypr.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yhd.tianlin.xyz

PHP:  // 手写递归函数
来源：http://dxn.cdnleiting.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dps.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yus.shangyingyoupin.top

Java: // 手写递归
来源：http://pqk.smart0.xyz

Go:   // 手写递归
来源：http://wkm.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://snk.gzhubu.top

C#:   // 手写递归
来源：http://bxs.cucudq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://beb.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kzk.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://axy.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://slo.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uxd.zdbjq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ixx.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pki.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jyw.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tdg.ehwqpu.com

================================================================================
来源：http://jtn.chenzaomai.com

O. 并发与异步
来源：http://ena.tian-w.cn

================================================================================
来源：http://tty.ivvv.top

[O01] 启动一个线程
来源：http://owi.cheryme.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eid.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fls.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://asu.c1oappe.top

TS:   // 同 JS
来源：http://pix.yj20258.top

Java: new Thread(() -> f()).start()
来源：http://xkb.hnxiangtu.top

Go:   go f()
来源：http://mvv.sjlbkw.cn

Ruby: Thread.new { f }
来源：http://yvj.epnwcf.com

C#:   Task.Run(() => F());
来源：http://ulx.zhijiandao.cn

[O02] 使用线程池
来源：http://cnt.redwolf501.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xyu.redwolf501.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://izn.redwolf501.top

JS:   // worker_threads 线程池
来源：http://hmr.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://tpz.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://bcp.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vuq.zycfv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://glp.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://elp.wangdashe.top

[O03] 加锁保护共享数据
来源：http://tkr.zycfv.cn

Py:   with lock: shared += 1
来源：http://aqh.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://cep.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ksl.316326.xyz

TS:   // 同 JS
来源：http://urx.yvedp.cn

Java: synchronized (this) { shared++; }
来源：http://wsj.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ttu.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://uvb.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://hcd.fanxiaobao.xyz

[O04] 定义异步函数并等待
来源：http://tzt.hnxiangtu.top

Py:   async def f():⏎    await g()
来源：http://czl.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mnr.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://kog.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://yrh.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oud.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eph.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yto.jianghu66.top

C#:   async Task F() { await G(); }
来源：http://kzl.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://prf.cashguo.top


<!-- 参考信息 -->