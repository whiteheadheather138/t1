代发 wailian999

L. 网络请求
来源：http://okt.guannengcc.top

================================================================================
来源：http://ufz.yanxiufei.cn

[L01] 发送 GET 请求
来源：http://gbw.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qtr.zdqjudy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dvu.svipenyu.cn

JS:   await fetch(url)
来源：http://fid.hnqzz.top

TS:   await fetch(url)
来源：http://edj.xylfe.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kri.hnqzz.top

Go:   resp, err := http.Get(url)
来源：http://mgw.hysaishi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hic.ydjk.org.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rcz.chenlongwang.top

[L02] 发送 POST JSON
来源：http://aon.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://ijx.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mlj.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lhk.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gkh.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jxv.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dof.zhengqikj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bwu.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eti.tanke756.top

[L03] 设置自定义请求头
来源：http://imr.xuanzx.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nvw.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wla.jinqigufen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xbc.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eya.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://erg.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kzg.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gna.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xyc.xinyue.icu

[L04] 设置超时
来源：http://xct.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://boa.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jet.svipenyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qmf.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mga.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mxw.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lre.yfazqb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hdd.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://epe.daria6918.cn

[L05] 上传文件（multipart）
来源：http://qgt.epnwcf.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jhl.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ezk.gaohongyu789.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gyv.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://veh.cucudq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kkf.hnxiangtu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://geh.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://umo.ydzc1.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://izf.zycfv.cn

[L06] 解析响应为 JSON
来源：http://vuz.vehdjk.com

Py:   resp.json()
来源：http://eiw.andypj.xyz

PHP:  json_decode($body, true);
来源：http://soa.nwbrower.top

JS:   await resp.json()
来源：http://xqb.jqgfzy.top

TS:   await resp.json()
来源：http://uoe.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cgj.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xjk.ybcxt.top

Ruby: JSON.parse(resp.body)
来源：http://vwh.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://svp.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://gbn.tian-w.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uyg.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://npx.shangyingyoupin.top

JS:   resp.ok;  resp.status
来源：http://nnc.guowangkeji.top

TS:   resp.ok;  resp.status
来源：http://aaq.52xcode.cn

Java: resp.statusCode()
来源：http://dmf.yonumen.top

Go:   resp.StatusCode
来源：http://qvb.daria6918.cn

Ruby: resp.code.to_i
来源：http://tkb.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://jyy.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://ctp.pycfn.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aon.wangshuangyany.cn

PHP:  curl_multi_init() 系列
来源：http://opz.redwolf501.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rlv.tarul.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dkp.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://odd.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eyc.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uob.jlsjyb.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bui.haohaochexian.top

================================================================================
来源：http://pgz.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://ikx.xinyue.icu

================================================================================
来源：http://ppa.yonumen.top

[M01] 读取命令行参数
来源：http://moc.snrcjt.cn

Py:   sys.argv[1:]
来源：http://imi.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://rqk.zycfv.cn

JS:   process.argv.slice(2)
来源：http://abd.yfazqb.com

TS:   process.argv.slice(2)
来源：http://mqn.hnqzz.top

Java: args 数组（main 方法参数）
来源：http://onm.hysaishi.cn

Go:   os.Args[1:]
来源：http://ppj.iojbl.cn

Ruby: ARGV
来源：http://iqp.yj202588.top

C#:   args 数组（Main 方法参数）
来源：http://pwb.chenlongwang.top

[M02] 读取环境变量
来源：http://svr.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://iiy.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://daa.xuanzx.com

JS:   process.env.HOME
来源：http://don.ivvv.top

TS:   process.env.HOME
来源：http://wjk.jinyuanbaomall.cn

Java: System.getenv("HOME")
来源：http://xto.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zat.fehbvm.com

Ruby: ENV["HOME"]
来源：http://tig.kuanghao11.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uur.hammf.cn

[M03] 执行外部命令
来源：http://qwq.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dre.kuanghao11.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fws.shangyingyoupin.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ebo.shanyushiyangtech.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tun.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cka.dashuyun.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://swz.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://vgf.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://vgg.meibo888.top

[M04] 获取当前工作目录
来源：http://yfw.xuanzx.com

Py:   os.getcwd()
来源：http://stj.aizwys.cn

PHP:  getcwd();
来源：http://txv.yvedp.cn

JS:   process.cwd()
来源：http://ged.zhoulong.xyz

TS:   process.cwd()
来源：http://uqn.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://wix.chenjidiqi.icu

Go:   os.Getwd()
来源：http://mwy.ybcxt.top

Ruby: Dir.pwd
来源：http://piv.smart0.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://ykd.hnqzz.top

[M05] 设置退出码
来源：http://oxt.sjlbkw.cn

Py:   sys.exit(1)
来源：http://bif.shzxlz.cn

PHP:  exit(1);
来源：http://brn.mhx1999.top

JS:   process.exit(1)
来源：http://tfm.hcnkem.com

TS:   process.exit(1)
来源：http://rjl.fengsongda.top

Java: System.exit(1)
来源：http://fqm.sufxvd.cn

Go:   os.Exit(1)
来源：http://xqt.hesvh.cn

Ruby: exit 1
来源：http://xzn.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bac.ppjwa.cn

[M06] 向标准错误输出
来源：http://vue.vqdsnc.cn

Py:   print("err", file=sys.stderr)
来源：http://zgp.ywan-chungtsiang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ilt.hnxiangtu.top

JS:   console.error("err")
来源：http://yea.redwolf501.top

TS:   console.error("err")
来源：http://lep.jinqigfzy.top

Java: System.err.println("err")
来源：http://ovu.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://txv.aibaodan.cn

Ruby: warn "err"
来源：http://pek.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://tgt.epnwcf.com

[M07] 判断是否为主入口
来源：http://rbe.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://leu.c1oappe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ngj.fanxiaobao.xyz

JS:   require.main === module
来源：http://liw.zycfv.cn

TS:   require.main === module
来源：http://zwa.ivvv.top

Java: public static void main(String[] args)
来源：http://xag.yj202588.top

Go:   func main()
来源：http://clm.wangshuangyany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wqi.shuidangran.top

C#:   static void Main(string[] args)
来源：http://kci.pengpengdd.cyou

[M08] 获取系统与运行时信息
来源：http://cpa.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://rvt.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://cun.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://umr.hesvh.cn

TS:   process.platform;  process.version
来源：http://slz.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gym.jinqigufen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wrm.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jrx.daria6918.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ggw.jyoumei.cn

================================================================================
来源：http://sae.hnqzz.top

N. 数据结构与算法
来源：http://pqm.52xcode.cn

================================================================================
来源：http://ijh.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://hqh.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ulv.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tdy.zdbjq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://biz.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://shp.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hfv.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://wdp.hnqzz.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fby.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://awc.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://lpz.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://woi.zhiwuduotai.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kii.mhx1999.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kbi.chenzaomai.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://gxz.c1oappe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mus.tarul.cn

Go:   slices.Sort(arr)
来源：http://rnz.jianghu66.top

Ruby: arr.sort
来源：http://zvg.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://njp.zhengqikj.top

[N03] 快速排序（分治示例）
来源：http://kek.daria6918.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vdn.guannengcc.top

PHP:  // 递归实现，或用 usort
来源：http://pyd.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ypq.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rse.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dpn.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://meg.xuetiantiany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ltp.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://asj.ybcxt.top

[N04] 斐波那契数列
来源：http://cxx.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rgy.havefunace.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ljf.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bqp.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fgn.xuetiantiany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ujx.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ayi.yongpay.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lmh.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ufu.0kj1m.cn

[N05] 最大公约数
来源：http://zto.yj202588.top

Py:   math.gcd(a, b)
来源：http://kax.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dfw.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hdd.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hgn.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jyd.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qrr.nwbrower.top

Ruby: a.gcd(b)
来源：http://imk.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jwi.jyoumei.cn

[N06] 判断回文字符串
来源：http://suw.gogol.net.cn

Py:   s == s[::-1]
来源：http://kdn.chenlongwang.top

PHP:  $s === strrev($s);
来源：http://pzd.xziqi.cn

JS:   s === [...s].reverse().join("")
来源：http://bau.shuidangran.top

TS:   s === [...s].reverse().join("")
来源：http://rnc.ywan-chungtsiang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://urn.tarul.cn

Go:   // 双指针从两端比较
来源：http://xqu.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://xeq.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gcq.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://tfk.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ols.cdnleiting.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://apk.iojbl.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jsx.jqgfzy.top

TS:   // 手写 Map<string, number>
来源：http://sjh.zhixingplan.top

Java: // 手写 HashMap
来源：http://pnq.yj20258888.top

Go:   // 手写 map[int]int
来源：http://ace.chenlongwang.top

Ruby: // 手写 Hash
来源：http://yxh.hfpthk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://slg.guannengcc.top

[N08] 生成全排列
来源：http://vlb.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://xgj.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://avi.c1oappe.top

JS:   // 手写回溯递归
来源：http://ler.aibaodan.cn

TS:   // 手写回溯递归
来源：http://pny.cheryme.top

Java: // 手写回溯递归
来源：http://dpc.zhixingplan.top

Go:   // 手写回溯递归
来源：http://yzn.jinqigufen.top

Ruby: arr.permutation.to_a
来源：http://byy.sweek.top

C#:   // 手写回溯递归
来源：http://iut.gaohongyu789.top

[N09] 栈与队列
来源：http://vji.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mwa.jlsjyb.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kgp.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://txd.andypj.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://djj.hnxiangtu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bmh.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mts.9152youxi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sei.shzxlz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zhe.zhoulong.xyz

[N10] 链表节点定义
来源：http://koj.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pvv.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dxa.sjlbkw.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qlt.xylfe.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ysq.fehbvm.com

Java: class Node { int v; Node next; }
来源：http://wgq.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://uhy.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://imq.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dom.shangyingyoupin.top

[N11] 二叉树中序遍历
来源：http://phi.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kpa.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://phc.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yww.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tmq.chenlongwang.top

Java: // 手写递归
来源：http://fpr.chenjidiqi.icu

Go:   // 手写递归
来源：http://iei.smart0.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jxj.andypj.xyz

C#:   // 手写递归
来源：http://mkw.wangdashe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yri.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rug.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oxc.zhiwuduotai.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dma.shangyingyoupin.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tfp.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://crb.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ser.smart0.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://prc.pengpengdd.cyou

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yhi.c1oappe.top

================================================================================
来源：http://pdt.yj20258.top

O. 并发与异步
来源：http://xqr.sysykeji.top

================================================================================
来源：http://sym.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://dgu.gotoacloud.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vxa.cheryme.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bla.zhongyouzk.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://frm.jyoumei.cn

TS:   // 同 JS
来源：http://qfk.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://olg.zhixingplan.top

Go:   go f()
来源：http://qms.feifeiyinyue.top

Ruby: Thread.new { f }
来源：http://som.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://rgf.xinyue.icu

[O02] 使用线程池
来源：http://pvh.fktsv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mnj.hongshengwenyu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dkx.ydjk.org.cn

JS:   // worker_threads 线程池
来源：http://orl.zycfv.cn

TS:   // worker_threads 线程池
来源：http://jba.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://ngr.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kvm.hfpthk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xxi.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ujj.9152youxi.cn

[O03] 加锁保护共享数据
来源：http://npz.jqgufenzy.top

Py:   with lock: shared += 1
来源：http://yyn.hcnkem.com

PHP:  // 用 flock() 做文件锁
来源：http://kvp.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://keo.ppjwa.cn

TS:   // 同 JS
来源：http://mtf.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://jqc.fehbvm.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bbx.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eec.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://ymi.zhijiandao.cn

[O04] 定义异步函数并等待
来源：http://vzs.tianlin.xyz

Py:   async def f():⏎    await g()
来源：http://wkc.hnqzz.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://euv.jqgufenzy.top

JS:   async function f() { await g(); }
来源：http://hgn.52xcode.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rzk.fzhhl.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cpg.ehwqpu.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fvr.fzhhl.top

Ruby: # 用 Fiber 或 async gem
来源：http://kqg.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://ngu.hfpthk.cn

[O05] 并发执行并等待全部完成
来源：http://niz.ppjwa.cn


<!-- 参考信息 -->