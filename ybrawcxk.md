代发 wailian999

L. 网络请求
来源：http://gfw.wangshuangyany.cn

================================================================================
来源：http://nli.chenlongwang.top

[L01] 发送 GET 请求
来源：http://xva.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://upw.mhx1999.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dnl.316326.xyz

JS:   await fetch(url)
来源：http://sxr.jyoumei.cn

TS:   await fetch(url)
来源：http://oxs.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uvr.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://fpr.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xpz.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fxc.aizwys.cn

[L02] 发送 POST JSON
来源：http://tfp.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://zxq.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rry.xziqi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ono.quarkkingdee.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aaq.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xix.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fbv.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lsr.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ifm.mhx1999.top

[L03] 设置自定义请求头
来源：http://ass.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ojb.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dmg.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vft.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mug.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nvz.yongpay.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dza.mhx1999.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ktn.yj202588.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tmu.hammf.cn

[L04] 设置超时
来源：http://zif.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://xbv.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zfy.yonumen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ytj.havefunace.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jkp.cheryme.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xsk.gotoacloud.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nif.zhengqikj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mot.yuanzhike.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oan.yj202588.top

[L05] 上传文件（multipart）
来源：http://fxb.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ecg.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://amv.iojbl.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nwn.xinyue.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://osh.xuetiantiany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sxb.gotoacloud.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dgl.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xww.tianlin.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zjm.jiagoushi.top

[L06] 解析响应为 JSON
来源：http://vyq.pycfn.com

Py:   resp.json()
来源：http://orv.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://kwp.daria6918.cn

JS:   await resp.json()
来源：http://usa.vehdjk.com

TS:   await resp.json()
来源：http://idk.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jyx.gotoacloud.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dte.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://nqf.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aee.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://fbh.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vxt.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cps.9152youxi.cn

JS:   resp.ok;  resp.status
来源：http://gwo.zhixingplan.top

TS:   resp.ok;  resp.status
来源：http://que.fzhhl.top

Java: resp.statusCode()
来源：http://unm.uphjek.com

Go:   resp.StatusCode
来源：http://rbk.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://ufs.dianchejie.cn

C#:   (int)resp.StatusCode
来源：http://uds.jqgfzy.top

[L08] 并发请求多个地址
来源：http://cyj.yj20258888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tmk.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://kwj.52xcode.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://anm.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ibx.jinqigfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://czm.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oes.shuidangran.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pdt.yfazqb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ogy.chenlongwang.top

================================================================================
来源：http://lsn.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://gag.hnqzz.top

================================================================================
来源：http://ijq.epnwcf.com

[M01] 读取命令行参数
来源：http://lnw.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://asg.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://gmq.jqgufenzy.top

JS:   process.argv.slice(2)
来源：http://gly.meibo888.top

TS:   process.argv.slice(2)
来源：http://sla.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://nwx.zdqjudy.top

Go:   os.Args[1:]
来源：http://ebn.jinyuanbaomall.cn

Ruby: ARGV
来源：http://zgw.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://tiv.hongshengwenyu.top

[M02] 读取环境变量
来源：http://sre.sjlbkw.cn

Py:   os.environ.get("HOME")
来源：http://yos.zdbjq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zhy.jianghu66.top

JS:   process.env.HOME
来源：http://eaa.uphjek.com

TS:   process.env.HOME
来源：http://biv.meibo888.top

Java: System.getenv("HOME")
来源：http://det.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gsx.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://cyz.yj20258.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baa.xziqi.cn

[M03] 执行外部命令
来源：http://ntn.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iuv.chenzaomai.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://beh.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://uje.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vsi.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vwi.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mch.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://uuw.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://fwh.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://yys.shzxlz.cn

Py:   os.getcwd()
来源：http://nqj.hnqzz.top

PHP:  getcwd();
来源：http://iag.hnqzz.top

JS:   process.cwd()
来源：http://zzj.zhoulong.xyz

TS:   process.cwd()
来源：http://daq.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://mhq.hesvh.cn

Go:   os.Getwd()
来源：http://jvc.yongpay.top

Ruby: Dir.pwd
来源：http://rdd.wangshuangyany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sdm.gogol.net.cn

[M05] 设置退出码
来源：http://vni.iojbl.cn

Py:   sys.exit(1)
来源：http://zpi.gotoacloud.top

PHP:  exit(1);
来源：http://ivs.gogol.net.cn

JS:   process.exit(1)
来源：http://tkf.epnwcf.com

TS:   process.exit(1)
来源：http://kyw.hysaishi.cn

Java: System.exit(1)
来源：http://sbg.wangdashe.top

Go:   os.Exit(1)
来源：http://vgs.meibo888.top

Ruby: exit 1
来源：http://lhi.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rdq.sxryk.cn

[M06] 向标准错误输出
来源：http://eyq.guowangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://hel.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lba.0kj1m.cn

JS:   console.error("err")
来源：http://hpe.gotoacloud.top

TS:   console.error("err")
来源：http://ehf.quarkkingdee.top

Java: System.err.println("err")
来源：http://ehw.guowangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cqd.fehbvm.com

Ruby: warn "err"
来源：http://iwf.sufxvd.cn

C#:   Console.Error.WriteLine("err")
来源：http://pyv.cashguo.top

[M07] 判断是否为主入口
来源：http://wba.xziqi.cn

Py:   if __name__ == "__main__":
来源：http://ttk.chenjidiqi.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wyw.ywan-chungtsiang.top

JS:   require.main === module
来源：http://yuq.pycfn.com

TS:   require.main === module
来源：http://moh.ppjwa.cn

Java: public static void main(String[] args)
来源：http://ykh.nwbrower.top

Go:   func main()
来源：http://esd.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zeb.yj20258.top

C#:   static void Main(string[] args)
来源：http://uqd.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://cyj.jlsjyb.cn

Py:   platform.system();  platform.python_version()
来源：http://vig.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://ojq.shanyushiyangtech.top

JS:   process.platform;  process.version
来源：http://ihn.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://grp.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qph.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://avd.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rhz.andypj.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://irm.dianchejie.cn

================================================================================
来源：http://mrk.cucudq.cn

N. 数据结构与算法
来源：http://llt.jianghu66.top

================================================================================
来源：http://mkc.birdmap.top

[N01] 二分查找（有序数组）
来源：http://bxo.shanyushiyangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://sns.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jbp.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://azz.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jcn.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://vgh.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://kud.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gnj.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://hgy.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://zdt.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://ofx.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://knf.zhengqikj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kqs.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fwx.ybcxt.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fpa.wangdashe.top

Go:   slices.Sort(arr)
来源：http://hax.hnqzz.top

Ruby: arr.sort
来源：http://gxy.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://irj.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://wyu.yonumen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nog.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://jpd.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hwu.shuidangran.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qhm.yueranfly.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lny.9152youxi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pjz.meibo888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yhr.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://hrx.jqgufenzy.top

[N04] 斐波那契数列
来源：http://phw.dashuyun.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fiz.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aom.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nmb.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://whl.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vvt.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hju.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wnr.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://prx.dashuyun.cn

[N05] 最大公约数
来源：http://aam.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://vrb.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://edo.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nyy.tian-w.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hyi.xingfuxueyuan.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oxg.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qrb.hfpthk.cn

Ruby: a.gcd(b)
来源：http://ten.hywenlv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xjs.hysaishi.cn

[N06] 判断回文字符串
来源：http://vua.yuxming.cn

Py:   s == s[::-1]
来源：http://crv.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://weo.daria6918.cn

JS:   s === [...s].reverse().join("")
来源：http://vie.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://was.fengsongda.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rqb.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://gex.chenlongwang.top

Ruby: s == s.reverse
来源：http://vzy.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fdn.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://kvo.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zfn.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jml.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gjg.bbcook.cn

TS:   // 手写 Map<string, number>
来源：http://dyy.ctjpmb.com

Java: // 手写 HashMap
来源：http://kom.aibaodan.cn

Go:   // 手写 map[int]int
来源：http://htr.daria6918.cn

Ruby: // 手写 Hash
来源：http://kgp.0kj1m.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cdy.sweek.top

[N08] 生成全排列
来源：http://xmv.fehbvm.com

Py:   itertools.permutations(arr)
来源：http://rjb.hammf.cn

PHP:  // 手写递归交换
来源：http://kvc.ybcxt.top

JS:   // 手写回溯递归
来源：http://fer.daxiang520.top

TS:   // 手写回溯递归
来源：http://cbw.kuanghao11.cn

Java: // 手写回溯递归
来源：http://qmb.xziqi.cn

Go:   // 手写回溯递归
来源：http://dbo.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://noq.iojbl.cn

C#:   // 手写回溯递归
来源：http://ynl.hnqzz.top

[N09] 栈与队列
来源：http://ich.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dai.hongshengwenyu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bfa.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gnb.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bjd.hysaishi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dkg.svipenyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://evk.jinghuilouyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nqg.cashguo.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tsp.svipenyu.cn

[N10] 链表节点定义
来源：http://qmc.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ylj.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pme.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qsc.hongshengwenyu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://afd.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://frn.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://dmq.zhixingplan.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ntp.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rfd.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://lyr.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ntf.chenzaomai.com

PHP:  // 手写递归函数
来源：http://kre.9152youxi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://afg.yangfankeji.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://irm.fehbvm.com

Java: // 手写递归
来源：http://oya.zhengqikj.top

Go:   // 手写递归
来源：http://cva.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ykz.haohaochexian.top

C#:   // 手写递归
来源：http://fgi.pengpengdd.cyou

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jco.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mkm.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mbd.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qkk.ywan-chungtsiang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xkd.ctjpmb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kig.guannengcc.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://flp.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aqz.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zfr.hammf.cn

================================================================================
来源：http://qdo.tarul.cn

O. 并发与异步
来源：http://mhv.snrcjt.cn

================================================================================
来源：http://qxs.iojbl.cn

[O01] 启动一个线程
来源：http://kvb.wangshuangyany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rnk.pycfn.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xmh.shuidangran.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xho.dianchejie.cn

TS:   // 同 JS
来源：http://gej.ppjwa.cn

Java: new Thread(() -> f()).start()
来源：http://fdp.jianghu66.top

Go:   go f()
来源：http://ano.52xcode.cn

Ruby: Thread.new { f }
来源：http://qnk.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://agy.0kj1m.cn

[O02] 使用线程池
来源：http://tuq.gaohongyu789.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ytu.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://juh.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://gsg.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://tfp.vehdjk.com

Java: Executors.newFixedThreadPool(4)
来源：http://nhu.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dby.daria6918.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ora.yvedp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gfe.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://vzy.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://cck.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://kzl.yfazqb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://deb.uphjek.com

TS:   // 同 JS
来源：http://som.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://sft.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vmd.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zcv.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://vfb.gzhubu.top

[O04] 定义异步函数并等待
来源：http://ukl.aibaodan.cn

Py:   async def f():⏎    await g()
来源：http://avr.sxryk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yga.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://vyg.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jve.gzhubu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nqq.zhiwuduotai.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sut.xinyue.icu

Ruby: # 用 Fiber 或 async gem
来源：http://adz.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://rbh.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://nyf.jinqigufen.top


<!-- 参考信息 -->