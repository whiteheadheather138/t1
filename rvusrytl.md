代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://bnf.yangfankeji.com

PHP:  unserialize(serialize($obj));
来源：http://idq.wangdashe.top

JS:   structuredClone(obj)
来源：http://xci.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://umd.zhiwuduotai.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wpe.zhoulong.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gha.fehbvm.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hgv.tanke756.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fxn.jinqigfzy.top

[K06] 解析 URL 查询串
来源：http://yog.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tfz.hnxiangtu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tza.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aca.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ije.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yqq.shangyingyoupin.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gwe.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sxj.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nuf.svipenyu.cn

[K07] 进制转换
来源：http://opc.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eht.guannengcc.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xfb.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ery.yuxming.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://shj.hnxiangtu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://okv.yj20258.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wfu.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hpy.haohaochexian.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gke.yangfankeji.com

[K08] 二进制序列化（非 JSON）
来源：http://pgu.fehbvm.com

Py:   pickle.dumps(obj)
来源：http://uwv.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pah.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://gwc.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://ttp.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ibd.jlsjyb.cn

Go:   encoding/gob
来源：http://olx.tian-w.cn

Ruby: Marshal.dump(obj)
来源：http://yuk.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vop.ydjk.org.cn

================================================================================
来源：http://ein.yonumen.top

L. 网络请求
来源：http://vix.yj20258888.top

================================================================================
来源：http://avd.aibaodan.cn

[L01] 发送 GET 请求
来源：http://qxo.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wdk.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://piv.pengpengdd.cyou

JS:   await fetch(url)
来源：http://lca.guannengcc.top

TS:   await fetch(url)
来源：http://nat.hcnkem.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://air.epnwcf.com

Go:   resp, err := http.Get(url)
来源：http://cco.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://okb.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qwr.ehwqpu.com

[L02] 发送 POST JSON
来源：http://jzz.zhengqikj.top

Py:   requests.post(url, json={"a": 1})
来源：http://ftn.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mkn.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xai.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hdz.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ash.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nhn.guannengcc.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://njp.fengsongda.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cpk.hysaishi.cn

[L03] 设置自定义请求头
来源：http://ode.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rwt.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cha.ctjpmb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cri.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ijt.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://flo.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nxy.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fdj.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xck.epnwcf.com

[L04] 设置超时
来源：http://nor.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://iov.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vnw.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fkq.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oal.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eis.ybcxt.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tic.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xmh.smart0.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gjd.cucudq.cn

[L05] 上传文件（multipart）
来源：http://ihb.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sal.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hjl.gogol.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pfm.316326.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vcr.tianlin.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hrh.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vkj.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vhh.vqdsnc.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nof.ydjk.org.cn

[L06] 解析响应为 JSON
来源：http://obn.shangyingyoupin.top

Py:   resp.json()
来源：http://ckd.uphjek.com

PHP:  json_decode($body, true);
来源：http://toj.yanxiufei.cn

JS:   await resp.json()
来源：http://iqj.ctjpmb.com

TS:   await resp.json()
来源：http://cfq.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://shs.hongshengwenyu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ozf.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://xlc.ydjk.org.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nbn.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://efb.bjfxy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mnr.yanxiufei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://owl.jiagoushi.top

JS:   resp.ok;  resp.status
来源：http://jxw.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://rah.gogol.net.cn

Java: resp.statusCode()
来源：http://mwp.gaohongyu789.top

Go:   resp.StatusCode
来源：http://kng.gotoacloud.top

Ruby: resp.code.to_i
来源：http://acy.sysykeji.top

C#:   (int)resp.StatusCode
来源：http://tfi.hongshengwenyu.top

[L08] 并发请求多个地址
来源：http://mlk.zhaomingkeji.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lke.havefunace.top

PHP:  curl_multi_init() 系列
来源：http://lrm.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kfx.zhengqikj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fsb.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ltt.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fjg.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://prc.svipenyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tdr.xinyue.icu

================================================================================
来源：http://jqf.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://loe.yangfankeji.com

================================================================================
来源：http://une.yj20258.top

[M01] 读取命令行参数
来源：http://xoy.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://knx.andypj.xyz

PHP:  $argv;  $argc;
来源：http://soo.dashuyun.cn

JS:   process.argv.slice(2)
来源：http://cmf.guannengcc.top

TS:   process.argv.slice(2)
来源：http://wkt.zdbjq.cn

Java: args 数组（main 方法参数）
来源：http://ssc.dianchejie.cn

Go:   os.Args[1:]
来源：http://yqf.ydzc1.top

Ruby: ARGV
来源：http://ihc.yfazqb.com

C#:   args 数组（Main 方法参数）
来源：http://kvb.sufxvd.cn

[M02] 读取环境变量
来源：http://qke.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://azz.jianghu66.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jvi.yvedp.cn

JS:   process.env.HOME
来源：http://fxs.52xcode.cn

TS:   process.env.HOME
来源：http://tki.tianlin.xyz

Java: System.getenv("HOME")
来源：http://irm.snrcjt.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gow.zhijiandao.cn

Ruby: ENV["HOME"]
来源：http://ygh.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aio.yonumen.top

[M03] 执行外部命令
来源：http://pvt.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kew.jianghu66.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yew.sxryk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xqu.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://yhl.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xop.tarul.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jiu.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://pts.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://vwy.yj20258888.top

[M04] 获取当前工作目录
来源：http://rfa.ydzc1.top

Py:   os.getcwd()
来源：http://yrh.guannengcc.top

PHP:  getcwd();
来源：http://yxh.xylfe.cn

JS:   process.cwd()
来源：http://gsh.jinqigufen.top

TS:   process.cwd()
来源：http://her.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://awe.gaohongyu789.top

Go:   os.Getwd()
来源：http://irc.snrcjt.cn

Ruby: Dir.pwd
来源：http://bap.xingfuxueyuan.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://rtb.zhengqikj.top

[M05] 设置退出码
来源：http://clv.hysaishi.cn

Py:   sys.exit(1)
来源：http://upk.9152youxi.cn

PHP:  exit(1);
来源：http://dho.c1oappe.top

JS:   process.exit(1)
来源：http://dix.hnxiangtu.top

TS:   process.exit(1)
来源：http://tcl.zhongyouzk.top

Java: System.exit(1)
来源：http://qmn.dianchejie.cn

Go:   os.Exit(1)
来源：http://xaj.zhiwuduotai.top

Ruby: exit 1
来源：http://djf.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pxt.hysaishi.cn

[M06] 向标准错误输出
来源：http://atf.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://okp.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://afi.shangyingyoupin.top

JS:   console.error("err")
来源：http://lyj.wangdashe.top

TS:   console.error("err")
来源：http://jtp.xinyue.icu

Java: System.err.println("err")
来源：http://ewk.chenlongwang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zxx.daxiang520.top

Ruby: warn "err"
来源：http://gzj.jinqigfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://baq.gogol.net.cn

[M07] 判断是否为主入口
来源：http://plb.fzhhl.top

Py:   if __name__ == "__main__":
来源：http://yuk.bbcook.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zee.feifeiyinyue.top

JS:   require.main === module
来源：http://wmd.jiagoushi.top

TS:   require.main === module
来源：http://qzw.xuanzx.com

Java: public static void main(String[] args)
来源：http://afn.316326.xyz

Go:   func main()
来源：http://vzq.pengpengdd.cyou

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rvi.52xcode.cn

C#:   static void Main(string[] args)
来源：http://spl.uphjek.com

[M08] 获取系统与运行时信息
来源：http://pjp.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://myj.xinyue.icu

PHP:  PHP_OS;  phpversion();
来源：http://tod.yuanzhike.top

JS:   process.platform;  process.version
来源：http://cja.guowangkeji.top

TS:   process.platform;  process.version
来源：http://qfz.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zgc.birdmap.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jox.yj20258888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fdc.hesvh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kdv.yfazqb.com

================================================================================
来源：http://vbw.yuxming.cn

N. 数据结构与算法
来源：http://sft.c1oappe.top

================================================================================
来源：http://khp.nanxinkj.top

[N01] 二分查找（有序数组）
来源：http://hdm.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://frg.yangfankeji.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kti.ywan-chungtsiang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pmm.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://agy.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://yqe.hysaishi.cn

Go:   sort.SearchInts(arr, x)
来源：http://pbi.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fdy.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://kap.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://cud.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://pda.jinqigfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fhd.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kgd.xuetiantiany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ncv.hfpthk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://olb.hnqzz.top

Go:   slices.Sort(arr)
来源：http://mtj.sjlbkw.cn

Ruby: arr.sort
来源：http://skj.daxiang520.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://baw.sysykeji.top

[N03] 快速排序（分治示例）
来源：http://rsa.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://new.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://fvv.cqqwz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vgx.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://osv.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://atm.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yuy.zhongyouzk.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gcl.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://gka.0kj1m.cn

[N04] 斐波那契数列
来源：http://keg.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://htp.pycfn.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oxj.wangdashe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ovi.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hjq.yvedp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://apr.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pqz.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yik.hnxiangtu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://azd.guannengcc.top

[N05] 最大公约数
来源：http://pmj.ywan-chungtsiang.top

Py:   math.gcd(a, b)
来源：http://lvz.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://klm.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fji.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://spx.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zwc.xuetiantiany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xgt.xylfe.cn

Ruby: a.gcd(b)
来源：http://ywb.daxiang520.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jfu.tian-w.cn

[N06] 判断回文字符串
来源：http://dwq.jqgufenzy.top

Py:   s == s[::-1]
来源：http://wki.tarul.cn

PHP:  $s === strrev($s);
来源：http://qpc.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://efk.hfpthk.cn

TS:   s === [...s].reverse().join("")
来源：http://eti.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wlz.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://tcg.dianchejie.cn

Ruby: s == s.reverse
来源：http://qqq.chenzaomai.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://udu.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://qhr.jianghu66.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://twd.chenlongwang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ydo.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://xhh.jlsjyb.cn

TS:   // 手写 Map<string, number>
来源：http://thl.mhx1999.top

Java: // 手写 HashMap
来源：http://ntt.iojbl.cn

Go:   // 手写 map[int]int
来源：http://mfe.nwbrower.top

Ruby: // 手写 Hash
来源：http://ezu.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bfd.zhixingplan.top

[N08] 生成全排列
来源：http://szl.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://kjg.fehbvm.com

PHP:  // 手写递归交换
来源：http://zlv.yuanzhike.top

JS:   // 手写回溯递归
来源：http://aym.316326.xyz

TS:   // 手写回溯递归
来源：http://qic.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://pjl.cucudq.cn

Go:   // 手写回溯递归
来源：http://vxy.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://jjq.shanyushiyangkeji.top

C#:   // 手写回溯递归
来源：http://xlg.jinqigfzy.top

[N09] 栈与队列
来源：http://jxi.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bfb.zhoulong.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://trb.zycfv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mwh.hnqzz.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://roh.yj20258888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bdy.meibo888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kvu.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xen.daxiang520.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bfh.xziqi.cn

[N10] 链表节点定义
来源：http://pgh.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jqs.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://gvx.9152youxi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jyv.svipenyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wta.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://rhk.dashuyun.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yqn.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://lse.zhijiandao.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://car.jinghuilouyu.cn

[N11] 二叉树中序遍历
来源：http://eam.gogol.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xur.hywenlv.cn

PHP:  // 手写递归函数
来源：http://diy.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dgu.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://arw.redwolf501.top

Java: // 手写递归
来源：http://jdy.hnqzz.top

Go:   // 手写递归
来源：http://vsw.tanke756.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iai.ybcxt.top

C#:   // 手写递归
来源：http://hrh.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vkp.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jqx.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qlw.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sbb.snrcjt.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pzg.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rez.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://llh.gzhubu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lzh.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pol.aizwys.cn

================================================================================
来源：http://abq.jiagoushi.top

O. 并发与异步
来源：http://xhc.jinqigfzy.top

================================================================================
来源：http://zmn.ydjk.org.cn

[O01] 启动一个线程
来源：http://opn.hcnkem.com


<!-- 参考信息 -->