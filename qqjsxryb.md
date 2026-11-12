代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://iwk.vehdjk.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wux.sysykeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pxf.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vda.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://hck.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ksa.gogol.net.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oiq.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rxi.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://irt.zhengqikj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qnq.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://spf.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nwf.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hcy.shanyushiyangkeji.top

[K07] 进制转换
来源：http://kqp.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wqk.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yaz.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tks.uphjek.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rjn.hcnkem.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zxg.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mnp.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ycs.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://utn.gaohongyu789.top

[K08] 二进制序列化（非 JSON）
来源：http://bwv.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://otp.mhx1999.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hnm.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://nhr.zhijiandao.cn

TS:   v8.serialize(obj)        // Node
来源：http://ust.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jeb.yuanzhike.top

Go:   encoding/gob
来源：http://owr.hfpthk.cn

Ruby: Marshal.dump(obj)
来源：http://nwe.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://apo.xinyue.icu

================================================================================
来源：http://mud.daria6918.cn

L. 网络请求
来源：http://lng.ctjpmb.com

================================================================================
来源：http://rtp.zycfv.cn

[L01] 发送 GET 请求
来源：http://jve.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dfg.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://afa.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://fue.chenlongwang.top

TS:   await fetch(url)
来源：http://rih.yanxiufei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tvh.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://rki.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://egr.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zgt.nanxinkj.top

[L02] 发送 POST JSON
来源：http://zxt.smart0.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://qcy.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pym.cucudq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ull.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zin.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wds.yj20258888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://glh.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nsi.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jae.sjlbkw.cn

[L03] 设置自定义请求头
来源：http://wwu.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ttx.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sez.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://szs.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sjt.yj202588.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mvz.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eyt.haohaochexian.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kwk.fengsongda.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://krq.hammf.cn

[L04] 设置超时
来源：http://jfm.aibaodan.cn

Py:   requests.get(url, timeout=5)
来源：http://rbz.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mgh.yuanzhike.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kxc.shanyushiyangtech.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mzo.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://knh.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dnm.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gsp.zhongyouzk.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wez.c1oappe.top

[L05] 上传文件（multipart）
来源：http://wwh.chenjidiqi.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tgx.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://asl.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bvt.uphjek.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://epx.tarul.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bhm.jqgfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tme.xuetiantiany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xve.sysykeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fgh.shanyushiyangkeji.top

[L06] 解析响应为 JSON
来源：http://yvz.ywan-chungtsiang.top

Py:   resp.json()
来源：http://nje.ydzc1.top

PHP:  json_decode($body, true);
来源：http://ljx.yueranfly.top

JS:   await resp.json()
来源：http://wiy.hnxiangtu.top

TS:   await resp.json()
来源：http://zsz.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sae.jianghu66.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pab.fktsv.cn

Ruby: JSON.parse(resp.body)
来源：http://ddj.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jzu.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://iei.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ueo.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hrj.uphjek.com

JS:   resp.ok;  resp.status
来源：http://tll.xinyue.icu

TS:   resp.ok;  resp.status
来源：http://rty.yfazqb.com

Java: resp.statusCode()
来源：http://zll.zhixingplan.top

Go:   resp.StatusCode
来源：http://qvi.fktsv.cn

Ruby: resp.code.to_i
来源：http://pqf.yj202588.top

C#:   (int)resp.StatusCode
来源：http://umr.ctjpmb.com

[L08] 并发请求多个地址
来源：http://isq.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://odd.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://djy.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dad.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cbf.shanyushiyangtech.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dbo.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jby.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ttr.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bje.yuxming.cn

================================================================================
来源：http://wyb.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://dlz.gotoacloud.top

================================================================================
来源：http://mzd.andypj.xyz

[M01] 读取命令行参数
来源：http://atl.xinyue.icu

Py:   sys.argv[1:]
来源：http://jbj.zdqjudy.top

PHP:  $argv;  $argc;
来源：http://zfe.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://qpl.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://eff.dianchejie.cn

Java: args 数组（main 方法参数）
来源：http://mcx.52xcode.cn

Go:   os.Args[1:]
来源：http://yxn.tarul.cn

Ruby: ARGV
来源：http://evp.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://ubp.jinghuilouyu.cn

[M02] 读取环境变量
来源：http://mxe.jinqigfzy.top

Py:   os.environ.get("HOME")
来源：http://zli.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zmf.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://qoq.yangfankeji.com

TS:   process.env.HOME
来源：http://kti.xinyue.icu

Java: System.getenv("HOME")
来源：http://sfz.birdmap.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ydo.bjfxy.top

Ruby: ENV["HOME"]
来源：http://ygf.jinqigufen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qup.jinqigufen.top

[M03] 执行外部命令
来源：http://ehz.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cvz.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wac.sufxvd.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cgt.feifeiyinyue.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xqd.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dyv.jqgfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wuf.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://erf.hywenlv.cn

C#:   Process.Start("ls", "-l");
来源：http://jlt.dianchejie.cn

[M04] 获取当前工作目录
来源：http://mcp.shuidangran.top

Py:   os.getcwd()
来源：http://ctd.jlsjyb.cn

PHP:  getcwd();
来源：http://dqt.jianghu66.top

JS:   process.cwd()
来源：http://ymo.uphjek.com

TS:   process.cwd()
来源：http://fjm.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://rpq.uphjek.com

Go:   os.Getwd()
来源：http://euz.aibaodan.cn

Ruby: Dir.pwd
来源：http://mkm.redwolf501.top

C#:   Directory.GetCurrentDirectory()
来源：http://wec.hammf.cn

[M05] 设置退出码
来源：http://djg.epnwcf.com

Py:   sys.exit(1)
来源：http://hok.wangdashe.top

PHP:  exit(1);
来源：http://fiu.zdbjq.cn

JS:   process.exit(1)
来源：http://vpx.0kj1m.cn

TS:   process.exit(1)
来源：http://owt.nanxinkj.top

Java: System.exit(1)
来源：http://ksb.aibaodan.cn

Go:   os.Exit(1)
来源：http://jgf.shanyushiyangtech.top

Ruby: exit 1
来源：http://qot.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jvl.daria6918.cn

[M06] 向标准错误输出
来源：http://fnw.tian-w.cn

Py:   print("err", file=sys.stderr)
来源：http://iao.yj202588.top

PHP:  fwrite(STDERR, "err\n");
来源：http://umy.zhongyouzk.top

JS:   console.error("err")
来源：http://jpn.hesvh.cn

TS:   console.error("err")
来源：http://ram.jlsjyb.cn

Java: System.err.println("err")
来源：http://lhk.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dao.0kj1m.cn

Ruby: warn "err"
来源：http://fou.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://cmh.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://fqv.jinqigufen.top

Py:   if __name__ == "__main__":
来源：http://ofk.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nqt.daxiang520.top

JS:   require.main === module
来源：http://ioh.zdbjq.cn

TS:   require.main === module
来源：http://pkw.gaohongyu789.top

Java: public static void main(String[] args)
来源：http://xbo.ywan-chungtsiang.top

Go:   func main()
来源：http://hly.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jez.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://ipd.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://ouh.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://unq.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://vnn.fktsv.cn

JS:   process.platform;  process.version
来源：http://pvj.hnxiangtu.top

TS:   process.platform;  process.version
来源：http://gmn.cashguo.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hia.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bti.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://npk.daria6918.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ecn.daria6918.cn

================================================================================
来源：http://qzj.gogol.net.cn

N. 数据结构与算法
来源：http://vkc.aizwys.cn

================================================================================
来源：http://jxu.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://zxy.nanxinkj.top

Py:   bisect.bisect_left(arr, x)
来源：http://khh.xylfe.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ycq.shuidangran.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nsi.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vrw.hcnkem.com

Java: Arrays.binarySearch(arr, x)
来源：http://ury.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://kci.hammf.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dpu.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://pzr.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://chn.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://cic.yueranfly.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lru.shzxlz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qmr.ybcxt.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tdq.52xcode.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xef.hnxiangtu.top

Go:   slices.Sort(arr)
来源：http://cab.cdnleiting.top

Ruby: arr.sort
来源：http://fmt.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ndo.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://wvk.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eyg.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://diy.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uok.andypj.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://red.cdnleiting.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cgi.316326.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oqj.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gef.redwolf501.top

C#:   // 手写递归，或 Array.Sort
来源：http://pig.tianlin.xyz

[N04] 斐波那契数列
来源：http://fwm.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jth.tarul.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xdw.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mgu.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://afr.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oqf.tian-w.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fjh.yanxiufei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uao.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kci.yueranfly.top

[N05] 最大公约数
来源：http://wpk.birdmap.top

Py:   math.gcd(a, b)
来源：http://kes.zdqjudy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zvv.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ofj.hnqzz.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xgf.yj20258.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fva.cashguo.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mwk.xziqi.cn

Ruby: a.gcd(b)
来源：http://vzj.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aiz.jinqigufen.top

[N06] 判断回文字符串
来源：http://ioa.wangdashe.top

Py:   s == s[::-1]
来源：http://hps.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://ykz.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://slk.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://skl.hesvh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://evt.meibo888.top

Go:   // 双指针从两端比较
来源：http://rcw.xylfe.cn

Ruby: s == s.reverse
来源：http://mjp.0kj1m.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wre.xylfe.cn

[N07] 两数之和（返回下标）
来源：http://pep.hywenlv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vhl.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kco.hfpthk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mzm.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://epp.sxryk.cn

Java: // 手写 HashMap
来源：http://rkg.c1oappe.top

Go:   // 手写 map[int]int
来源：http://mps.gotoacloud.top

Ruby: // 手写 Hash
来源：http://vdn.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nii.yonumen.top

[N08] 生成全排列
来源：http://xux.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://hwn.fktsv.cn

PHP:  // 手写递归交换
来源：http://eru.yvedp.cn

JS:   // 手写回溯递归
来源：http://gvw.mhx1999.top

TS:   // 手写回溯递归
来源：http://bep.quarkkingdee.top

Java: // 手写回溯递归
来源：http://kyx.cheryme.top

Go:   // 手写回溯递归
来源：http://gqc.ybcxt.top

Ruby: arr.permutation.to_a
来源：http://hae.jyoumei.cn

C#:   // 手写回溯递归
来源：http://paj.snrcjt.cn

[N09] 栈与队列
来源：http://kyk.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fcq.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zrh.meibo888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://crf.ydjk.org.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nkc.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lia.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://doh.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gtv.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wln.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://akr.redwolf501.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zhz.fktsv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xgx.wangshuangyany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dbr.ydjk.org.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wiu.nanxuanxn.top

Java: class Node { int v; Node next; }
来源：http://hro.hongshengwenyu.top

Go:   type Node struct { V int; Next *Node }
来源：http://iem.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gcx.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fcu.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://xsq.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ckh.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://ytw.zhiwuduotai.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nes.chenzaomai.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jjk.yj20258888.top

Java: // 手写递归
来源：http://zzl.uphjek.com

Go:   // 手写递归
来源：http://rst.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xmc.tianlin.xyz

C#:   // 手写递归
来源：http://wvz.yj20258.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://irl.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mfe.yj20258888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zxd.chenjidiqi.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hlr.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kkb.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uhr.daria6918.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aku.yvedp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ddd.zhiwuduotai.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nep.guowangkeji.top

================================================================================
来源：http://bnq.vehdjk.com

O. 并发与异步
来源：http://mgr.xziqi.cn

================================================================================
来源：http://oqb.hnxiangtu.top

[O01] 启动一个线程
来源：http://ohu.jinyuanbaomall.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nnh.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rsj.tanke756.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nyo.nanxuanxn.top

TS:   // 同 JS
来源：http://kdx.c1oappe.top


<!-- 参考信息 -->