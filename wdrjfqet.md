代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ivu.dashuyun.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zjp.xziqi.cn

[K08] 二进制序列化（非 JSON）
来源：http://pff.yj20258.top

Py:   pickle.dumps(obj)
来源：http://dqe.jianghu66.top

PHP:  serialize($obj);  unserialize($s);
来源：http://shi.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://nns.316326.xyz

TS:   v8.serialize(obj)        // Node
来源：http://mtk.xingfuxueyuan.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yoh.cdnleiting.top

Go:   encoding/gob
来源：http://uxy.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://tku.hywenlv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vhb.hcnkem.com

================================================================================
来源：http://bvu.dianchejie.cn

L. 网络请求
来源：http://gzh.52xcode.cn

================================================================================
来源：http://wua.daxiang520.top

[L01] 发送 GET 请求
来源：http://owy.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fiy.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dhk.shanyushiyangtech.top

JS:   await fetch(url)
来源：http://slt.shzxlz.cn

TS:   await fetch(url)
来源：http://vov.hcnkem.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hcs.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://kvr.guowangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://eex.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://afb.uphjek.com

[L02] 发送 POST JSON
来源：http://skw.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://xcf.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gtd.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sib.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kfi.havefunace.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iex.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oeb.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ewx.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://feb.hywenlv.cn

[L03] 设置自定义请求头
来源：http://mqo.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bmm.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kgv.snrcjt.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rae.yueranfly.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mmv.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://clp.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gww.zycfv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cxl.yangfankeji.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mtj.gzhubu.top

[L04] 设置超时
来源：http://exh.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://zcd.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://inv.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://npl.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bix.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uwo.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xxe.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://znf.shanyushiyangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qtr.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://com.daria6918.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://daf.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://neb.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gho.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wot.uphjek.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oas.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://akd.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bqf.kuanghao11.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rgu.c1oappe.top

[L06] 解析响应为 JSON
来源：http://kja.gogol.net.cn

Py:   resp.json()
来源：http://fvz.xinyue.icu

PHP:  json_decode($body, true);
来源：http://jea.yfazqb.com

JS:   await resp.json()
来源：http://rej.jinyuanbaomall.cn

TS:   await resp.json()
来源：http://yeb.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cwo.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fpc.ydjk.org.cn

Ruby: JSON.parse(resp.body)
来源：http://shc.iojbl.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://opa.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://gqe.epnwcf.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vmk.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xzc.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://vue.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://zgv.zhixingplan.top

Java: resp.statusCode()
来源：http://mrt.yvedp.cn

Go:   resp.StatusCode
来源：http://lmz.yfazqb.com

Ruby: resp.code.to_i
来源：http://udp.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://kgn.nwbrower.top

[L08] 并发请求多个地址
来源：http://hav.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rff.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://ihl.shangyingyoupin.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iwa.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ttt.smart0.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rpj.yonumen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nwg.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ebk.9152youxi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://waj.aizwys.cn

================================================================================
来源：http://kaq.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://cqg.shanyushiyangkeji.top

================================================================================
来源：http://gup.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://xoi.jiagoushi.top

Py:   sys.argv[1:]
来源：http://jvz.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://jvh.jlsjyb.cn

JS:   process.argv.slice(2)
来源：http://maw.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://ptb.pycfn.com

Java: args 数组（main 方法参数）
来源：http://xlv.fehbvm.com

Go:   os.Args[1:]
来源：http://erz.jqgfzy.top

Ruby: ARGV
来源：http://bid.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://hpq.yj20258888.top

[M02] 读取环境变量
来源：http://mds.havefunace.top

Py:   os.environ.get("HOME")
来源：http://rmw.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ccs.hnqzz.top

JS:   process.env.HOME
来源：http://cgh.zdqjudy.top

TS:   process.env.HOME
来源：http://qsk.xylfe.cn

Java: System.getenv("HOME")
来源：http://deu.ctjpmb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hvj.yj20258.top

Ruby: ENV["HOME"]
来源：http://vxg.guannengcc.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hxa.bjfxy.top

[M03] 执行外部命令
来源：http://itt.nanxuanxn.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://suc.zdqjudy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gyb.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vco.ctjpmb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://cja.yongpay.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pnx.havefunace.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bce.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://ema.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://eif.ybcxt.top

[M04] 获取当前工作目录
来源：http://ffv.hnqzz.top

Py:   os.getcwd()
来源：http://faa.ctjpmb.com

PHP:  getcwd();
来源：http://lxx.ctjpmb.com

JS:   process.cwd()
来源：http://knv.shzxlz.cn

TS:   process.cwd()
来源：http://fjl.daxiang520.top

Java: Path.of("").toAbsolutePath()
来源：http://ryz.meibo888.top

Go:   os.Getwd()
来源：http://jjf.snrcjt.cn

Ruby: Dir.pwd
来源：http://ysx.c1oappe.top

C#:   Directory.GetCurrentDirectory()
来源：http://wba.tanke756.top

[M05] 设置退出码
来源：http://cyw.hammf.cn

Py:   sys.exit(1)
来源：http://cqh.zdqjudy.top

PHP:  exit(1);
来源：http://crt.sweek.top

JS:   process.exit(1)
来源：http://otd.gogol.net.cn

TS:   process.exit(1)
来源：http://wsv.feifeiyinyue.top

Java: System.exit(1)
来源：http://vgu.chenlongwang.top

Go:   os.Exit(1)
来源：http://pmu.gotoacloud.top

Ruby: exit 1
来源：http://ubj.sjlbkw.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rls.chenjidiqi.icu

[M06] 向标准错误输出
来源：http://jjm.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://erk.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pkj.zhoulong.xyz

JS:   console.error("err")
来源：http://tyw.dashuyun.cn

TS:   console.error("err")
来源：http://bwf.gaohongyu789.top

Java: System.err.println("err")
来源：http://eyw.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://euv.hywenlv.cn

Ruby: warn "err"
来源：http://pur.yj20258.top

C#:   Console.Error.WriteLine("err")
来源：http://kwg.snrcjt.cn

[M07] 判断是否为主入口
来源：http://rbm.bjfxy.top

Py:   if __name__ == "__main__":
来源：http://anr.zdqjudy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tlx.jiagoushi.top

JS:   require.main === module
来源：http://npq.chenzaomai.com

TS:   require.main === module
来源：http://yae.wangshuangyany.cn

Java: public static void main(String[] args)
来源：http://esu.uphjek.com

Go:   func main()
来源：http://llz.wangshuangyany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mhc.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://duv.ivvv.top

[M08] 获取系统与运行时信息
来源：http://wtb.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://wnu.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://tjc.havefunace.top

JS:   process.platform;  process.version
来源：http://qyx.cqqwz.cn

TS:   process.platform;  process.version
来源：http://hie.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wrj.snrcjt.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wkr.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://snp.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://emi.sxryk.cn

================================================================================
来源：http://cvo.ctjpmb.com

N. 数据结构与算法
来源：http://iul.jinqigufen.top

================================================================================
来源：http://gfh.wangdashe.top

[N01] 二分查找（有序数组）
来源：http://lrw.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://gfq.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qxw.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gmk.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pft.xuanzx.com

Java: Arrays.binarySearch(arr, x)
来源：http://pli.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://uav.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rzh.redwolf501.top

C#:   Array.BinarySearch(arr, x)
来源：http://jql.chenzaomai.com

[N02] 排序（工程实践用内置实现）
来源：http://fxj.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://fgf.jinqigufen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jxo.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ggv.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fnu.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xwc.sysykeji.top

Go:   slices.Sort(arr)
来源：http://wsl.yonumen.top

Ruby: arr.sort
来源：http://qnp.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://trx.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://abh.zycfv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://smg.zycfv.cn

PHP:  // 递归实现，或用 usort
来源：http://xtb.fengsongda.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wky.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dne.sysykeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qfd.birdmap.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bzd.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rpa.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://nii.jianghu66.top

[N04] 斐波那契数列
来源：http://xvc.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fcp.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jhd.sjlbkw.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pua.dashuyun.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://agq.meibo888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xtr.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xpx.jlsjyb.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qow.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mtf.hammf.cn

[N05] 最大公约数
来源：http://gvn.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://puk.nanxinkj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ahr.cqqwz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uxs.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://azy.guannengcc.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pqi.fehbvm.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zmt.xuanzx.com

Ruby: a.gcd(b)
来源：http://sol.hnqzz.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wee.xuanzx.com

[N06] 判断回文字符串
来源：http://udm.316326.xyz

Py:   s == s[::-1]
来源：http://nby.fehbvm.com

PHP:  $s === strrev($s);
来源：http://irx.havefunace.top

JS:   s === [...s].reverse().join("")
来源：http://csl.zhoulong.xyz

TS:   s === [...s].reverse().join("")
来源：http://kxg.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dsn.gaohongyu789.top

Go:   // 双指针从两端比较
来源：http://ubo.guowangkeji.top

Ruby: s == s.reverse
来源：http://gjh.snrcjt.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vru.zdbjq.cn

[N07] 两数之和（返回下标）
来源：http://wii.fanxiaobao.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kxd.jinghuilouyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ohj.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xni.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://vry.gaohongyu789.top

Java: // 手写 HashMap
来源：http://eug.yj20258.top

Go:   // 手写 map[int]int
来源：http://bsz.iojbl.cn

Ruby: // 手写 Hash
来源：http://wtt.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://zms.aizwys.cn

[N08] 生成全排列
来源：http://fcf.meibo888.top

Py:   itertools.permutations(arr)
来源：http://spp.dianchejie.cn

PHP:  // 手写递归交换
来源：http://nwa.sweek.top

JS:   // 手写回溯递归
来源：http://gbv.yj20258.top

TS:   // 手写回溯递归
来源：http://oyh.jinqigufen.top

Java: // 手写回溯递归
来源：http://bii.shangyingyoupin.top

Go:   // 手写回溯递归
来源：http://idf.sweek.top

Ruby: arr.permutation.to_a
来源：http://lyi.xziqi.cn

C#:   // 手写回溯递归
来源：http://znz.aibaodan.cn

[N09] 栈与队列
来源：http://puk.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aws.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hcw.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xli.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iys.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jlt.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gpk.jlsjyb.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yez.hnqzz.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nmm.gotoacloud.top

[N10] 链表节点定义
来源：http://snu.snrcjt.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hwt.xuanzx.com

PHP:  class Node { public $v; public $next = null; }
来源：http://lna.0kj1m.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://irc.jinqigufen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sbv.nanxuanxn.top

Java: class Node { int v; Node next; }
来源：http://qgd.kuanghao11.cn

Go:   type Node struct { V int; Next *Node }
来源：http://max.zhengqikj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://phh.ydjk.org.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xic.xylfe.cn

[N11] 二叉树中序遍历
来源：http://iqj.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qzo.jqgufenzy.top

PHP:  // 手写递归函数
来源：http://gvt.jqgufenzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yif.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ggy.zhijiandao.cn

Java: // 手写递归
来源：http://qvz.daria6918.cn

Go:   // 手写递归
来源：http://gex.aizwys.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wnb.zhengqikj.top

C#:   // 手写递归
来源：http://jsw.xuanzx.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wzd.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mnq.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gia.chenlongwang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gkc.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tat.hcnkem.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kks.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wgg.jianghu66.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bxm.sufxvd.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qab.yuxming.cn

================================================================================
来源：http://ndt.epnwcf.com

O. 并发与异步
来源：http://fij.jianghu66.top

================================================================================
来源：http://iyh.wangshuangyany.cn

[O01] 启动一个线程
来源：http://ecx.yangfankeji.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dxx.hfpthk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kbl.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qvb.uphjek.com

TS:   // 同 JS
来源：http://smo.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://wsf.hongshengwenyu.top

Go:   go f()
来源：http://hix.haohaochexian.top

Ruby: Thread.new { f }
来源：http://upj.gaohongyu789.top

C#:   Task.Run(() => F());
来源：http://dga.redwolf501.top

[O02] 使用线程池
来源：http://ver.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fih.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uqj.yvedp.cn

JS:   // worker_threads 线程池
来源：http://daq.smart0.xyz

TS:   // worker_threads 线程池
来源：http://pnf.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://yum.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bgo.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zpa.9152youxi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://poi.guannengcc.top

[O03] 加锁保护共享数据
来源：http://xco.smart0.xyz

Py:   with lock: shared += 1
来源：http://gjw.hesvh.cn

PHP:  // 用 flock() 做文件锁
来源：http://mpy.zhaomingkeji.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zai.ybcxt.top

TS:   // 同 JS
来源：http://jlw.cqqwz.cn

Java: synchronized (this) { shared++; }
来源：http://amv.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://txl.xziqi.cn


<!-- 参考信息 -->