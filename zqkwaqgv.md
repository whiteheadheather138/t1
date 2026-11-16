代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ijf.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://keg.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://fjz.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://vrw.zhongyouzk.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jyv.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://zpb.shangyingyoupin.top

TS:   v8.serialize(obj)        // Node
来源：http://kra.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rxt.mhx1999.top

Go:   encoding/gob
来源：http://wcm.yangfankeji.com

Ruby: Marshal.dump(obj)
来源：http://ybr.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ghx.dashuyun.cn

================================================================================
来源：http://lgp.fanxiaobao.xyz

L. 网络请求
来源：http://emg.jqgfzy.top

================================================================================
来源：http://xvs.tian-w.cn

[L01] 发送 GET 请求
来源：http://mub.xinyue.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ogn.cucudq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://giq.shanyushiyangtech.top

JS:   await fetch(url)
来源：http://zcv.hywenlv.cn

TS:   await fetch(url)
来源：http://blv.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vrz.meibo888.top

Go:   resp, err := http.Get(url)
来源：http://aje.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ghg.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qcn.fzhhl.top

[L02] 发送 POST JSON
来源：http://hzj.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pjx.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://drd.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sox.hywenlv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wgd.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gfm.ydjk.org.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aip.hammf.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ixv.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cwe.bjfxy.top

[L03] 设置自定义请求头
来源：http://kmx.jqgufenzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dpc.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xqt.hysaishi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rlo.chenzaomai.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bsy.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cet.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bfb.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ryj.cashguo.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bev.birdmap.top

[L04] 设置超时
来源：http://suo.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://yde.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://btx.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tix.dianchejie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ixm.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://upw.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ihb.guowangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://azn.nanxuanxn.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wja.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://fbu.zhoulong.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rpq.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rva.dianchejie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fwt.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://khs.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ohd.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wpt.quarkkingdee.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wqo.tarul.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wrs.hammf.cn

[L06] 解析响应为 JSON
来源：http://mkn.gaohongyu789.top

Py:   resp.json()
来源：http://rqw.meibo888.top

PHP:  json_decode($body, true);
来源：http://wtz.shangyingyoupin.top

JS:   await resp.json()
来源：http://qfo.jinghuilouyu.cn

TS:   await resp.json()
来源：http://ttg.hongshengwenyu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kxm.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nug.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://qlh.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cii.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://ymq.yuxming.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wwv.tanke756.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oaf.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://xqg.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://zvv.shuidangran.top

Java: resp.statusCode()
来源：http://vou.52xcode.cn

Go:   resp.StatusCode
来源：http://psl.bbcook.cn

Ruby: resp.code.to_i
来源：http://zqs.meibo888.top

C#:   (int)resp.StatusCode
来源：http://mgq.yangfankeji.com

[L08] 并发请求多个地址
来源：http://wmt.hesvh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lqm.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://sdj.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uqo.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yht.xziqi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pfh.andypj.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zkd.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qiu.nanxinkj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gxa.mhx1999.top

================================================================================
来源：http://tjb.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://vsi.daria6918.cn

================================================================================
来源：http://rwl.fanxiaobao.xyz

[M01] 读取命令行参数
来源：http://euw.fehbvm.com

Py:   sys.argv[1:]
来源：http://nlr.hnqzz.top

PHP:  $argv;  $argc;
来源：http://yzz.chenlongwang.top

JS:   process.argv.slice(2)
来源：http://vbk.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://yoi.chenlongwang.top

Java: args 数组（main 方法参数）
来源：http://kcf.yj202588.top

Go:   os.Args[1:]
来源：http://tiz.zhaomingkeji.xyz

Ruby: ARGV
来源：http://tds.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://lgr.shanyushiyangkeji.top

[M02] 读取环境变量
来源：http://lzc.chenlongwang.top

Py:   os.environ.get("HOME")
来源：http://vxl.hnqzz.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dnc.jqgufenzy.top

JS:   process.env.HOME
来源：http://qho.shanyushiyangkeji.top

TS:   process.env.HOME
来源：http://zwi.xinyue.icu

Java: System.getenv("HOME")
来源：http://oti.tianlin.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tuv.ybcxt.top

Ruby: ENV["HOME"]
来源：http://ewj.yj20258.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qii.snrcjt.cn

[M03] 执行外部命令
来源：http://nkt.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tob.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yoj.hongshengwenyu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pri.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://boo.cdnleiting.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yyk.hnqzz.top

Go:   exec.Command("ls", "-l").Output()
来源：http://njq.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://vta.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://dkj.yvedp.cn

[M04] 获取当前工作目录
来源：http://fsj.redwolf501.top

Py:   os.getcwd()
来源：http://tov.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://gwf.hcnkem.com

JS:   process.cwd()
来源：http://yzq.chenjidiqi.icu

TS:   process.cwd()
来源：http://hsz.xuetiantiany.cn

Java: Path.of("").toAbsolutePath()
来源：http://ixx.cdnleiting.top

Go:   os.Getwd()
来源：http://rqr.jinyuanbaomall.cn

Ruby: Dir.pwd
来源：http://taf.ydzc1.top

C#:   Directory.GetCurrentDirectory()
来源：http://svd.9152youxi.cn

[M05] 设置退出码
来源：http://ttq.nanxuanxn.top

Py:   sys.exit(1)
来源：http://nyc.wangshuangyany.cn

PHP:  exit(1);
来源：http://lma.sjlbkw.cn

JS:   process.exit(1)
来源：http://gop.hnqzz.top

TS:   process.exit(1)
来源：http://mme.guowangkeji.top

Java: System.exit(1)
来源：http://ntn.cucudq.cn

Go:   os.Exit(1)
来源：http://pic.fengsongda.top

Ruby: exit 1
来源：http://mdi.uphjek.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xhh.hfpthk.cn

[M06] 向标准错误输出
来源：http://kfo.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://pcq.ehwqpu.com

PHP:  fwrite(STDERR, "err\n");
来源：http://vod.nwbrower.top

JS:   console.error("err")
来源：http://kmq.yongpay.top

TS:   console.error("err")
来源：http://hzu.zdqjudy.top

Java: System.err.println("err")
来源：http://xbu.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dcu.gaohongyu789.top

Ruby: warn "err"
来源：http://zdy.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://vup.0kj1m.cn

[M07] 判断是否为主入口
来源：http://wdo.snrcjt.cn

Py:   if __name__ == "__main__":
来源：http://wzv.wangdashe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tdq.zhongyouzk.top

JS:   require.main === module
来源：http://drn.hnxiangtu.top

TS:   require.main === module
来源：http://mhv.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://ohu.cucudq.cn

Go:   func main()
来源：http://wmu.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kpj.shanyushiyangkeji.top

C#:   static void Main(string[] args)
来源：http://gpz.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://jeo.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://vul.uphjek.com

PHP:  PHP_OS;  phpversion();
来源：http://ymx.yfazqb.com

JS:   process.platform;  process.version
来源：http://jax.tian-w.cn

TS:   process.platform;  process.version
来源：http://xkd.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dmf.zhiwuduotai.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wfu.jinghuilouyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blw.yangfankeji.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://whu.bbcook.cn

================================================================================
来源：http://msr.fengsongda.top

N. 数据结构与算法
来源：http://hro.sjlbkw.cn

================================================================================
来源：http://mjj.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://itj.sufxvd.cn

Py:   bisect.bisect_left(arr, x)
来源：http://twt.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yxh.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xgf.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ksi.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://tsm.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://sor.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://thr.shzxlz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iui.316326.xyz

[N02] 排序（工程实践用内置实现）
来源：http://fcf.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://dzz.hysaishi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rvr.shzxlz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fob.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zbg.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://roq.fengsongda.top

Go:   slices.Sort(arr)
来源：http://qgd.daria6918.cn

Ruby: arr.sort
来源：http://efb.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hzz.yuxming.cn

[N03] 快速排序（分治示例）
来源：http://zen.zhijiandao.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eix.yongpay.top

PHP:  // 递归实现，或用 usort
来源：http://dkt.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lxs.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wzh.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mnf.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xmc.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uyu.bjfxy.top

C#:   // 手写递归，或 Array.Sort
来源：http://nxq.c1oappe.top

[N04] 斐波那契数列
来源：http://blo.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nze.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://msf.snrcjt.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://quc.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sjq.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dsq.jinghuilouyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aax.nanxinkj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pat.guowangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dsa.snrcjt.cn

[N05] 最大公约数
来源：http://jin.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://yxc.aibaodan.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tep.xziqi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cas.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oai.hysaishi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gwj.ehwqpu.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dxn.gogol.net.cn

Ruby: a.gcd(b)
来源：http://gxi.sxryk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rvq.andypj.xyz

[N06] 判断回文字符串
来源：http://ydj.jiagoushi.top

Py:   s == s[::-1]
来源：http://buw.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://iha.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://bjz.shanyushiyangtech.top

TS:   s === [...s].reverse().join("")
来源：http://xps.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mxw.ybcxt.top

Go:   // 双指针从两端比较
来源：http://gbq.bbcook.cn

Ruby: s == s.reverse
来源：http://gyp.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bmb.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://lnl.yfazqb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hxp.zhaomingkeji.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oeu.yj202588.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bwm.zdqjudy.top

TS:   // 手写 Map<string, number>
来源：http://jmk.gzhubu.top

Java: // 手写 HashMap
来源：http://wly.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://vox.gzhubu.top

Ruby: // 手写 Hash
来源：http://pnw.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://reh.vehdjk.com

[N08] 生成全排列
来源：http://zxc.cheryme.top

Py:   itertools.permutations(arr)
来源：http://xvk.dashuyun.cn

PHP:  // 手写递归交换
来源：http://eqb.ppjwa.cn

JS:   // 手写回溯递归
来源：http://xiq.sxryk.cn

TS:   // 手写回溯递归
来源：http://fxa.xylfe.cn

Java: // 手写回溯递归
来源：http://ghk.hywenlv.cn

Go:   // 手写回溯递归
来源：http://kyu.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://dpw.fehbvm.com

C#:   // 手写回溯递归
来源：http://ltn.guowangkeji.top

[N09] 栈与队列
来源：http://ybj.gotoacloud.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hgu.xuetiantiany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sfo.jiagoushi.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bvj.yueranfly.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wuy.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rrk.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aqb.yj20258.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://peo.daria6918.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kab.sxryk.cn

[N10] 链表节点定义
来源：http://cga.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cbk.ctjpmb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://fxp.zdqjudy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ldp.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lff.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://ieb.zhaomingkeji.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://uoz.iojbl.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pax.xuanzx.com

C#:   class Node { public int V; public Node? Next; }
来源：http://mjb.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://zde.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vdp.hnqzz.top

PHP:  // 手写递归函数
来源：http://uxa.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qpr.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gxm.zhongyouzk.top

Java: // 手写递归
来源：http://kwx.c1oappe.top

Go:   // 手写递归
来源：http://mcz.aizwys.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rss.aibaodan.cn

C#:   // 手写递归
来源：http://ywn.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lhx.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hyh.c1oappe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uab.fktsv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gbh.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hfv.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fwk.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vmv.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hvn.epnwcf.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wlc.daxiang520.top

================================================================================
来源：http://hqv.tian-w.cn

O. 并发与异步
来源：http://zbe.tarul.cn

================================================================================
来源：http://udc.ivvv.top

[O01] 启动一个线程
来源：http://hmy.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aov.yvedp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vye.vehdjk.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yra.yj202588.top

TS:   // 同 JS
来源：http://noc.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://wfq.yfazqb.com

Go:   go f()
来源：http://kig.haohaochexian.top

Ruby: Thread.new { f }
来源：http://eln.xinyue.icu

C#:   Task.Run(() => F());
来源：http://zog.jinqigufen.top

[O02] 使用线程池
来源：http://sah.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dga.tanke756.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lgd.jyoumei.cn

JS:   // worker_threads 线程池
来源：http://ril.sjlbkw.cn

TS:   // worker_threads 线程池
来源：http://akt.cashguo.top

Java: Executors.newFixedThreadPool(4)
来源：http://qbn.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qar.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://puj.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qdl.gaohongyu789.top

[O03] 加锁保护共享数据
来源：http://cqm.gzhubu.top

Py:   with lock: shared += 1
来源：http://cxn.sufxvd.cn

PHP:  // 用 flock() 做文件锁
来源：http://zeu.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://npg.yueranfly.top

TS:   // 同 JS
来源：http://qgb.yongpay.top

Java: synchronized (this) { shared++; }
来源：http://ysv.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lmf.shuidangran.top


<!-- 参考信息 -->