代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://sru.cheryme.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fgz.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://axp.andypj.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://suy.9152youxi.cn

[K06] 解析 URL 查询串
来源：http://ewe.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://olc.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qft.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jju.pengpengdd.cyou

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wvo.aibaodan.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bui.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://aaf.hcnkem.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dny.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vgq.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://djn.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vvo.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://npl.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qif.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qut.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gnr.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zye.shanyushiyangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hgc.vehdjk.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bct.shangyingyoupin.top

[K08] 二进制序列化（非 JSON）
来源：http://jzq.kuanghao11.cn

Py:   pickle.dumps(obj)
来源：http://jwb.aibaodan.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rmj.sjlbkw.cn

JS:   v8.serialize(obj)        // Node
来源：http://fri.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://kis.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vbn.zhengqikj.top

Go:   encoding/gob
来源：http://zkq.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://cpn.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dob.zhixingplan.top

================================================================================
来源：http://wth.jyoumei.cn

L. 网络请求
来源：http://bjn.birdmap.top

================================================================================
来源：http://kyy.sweek.top

[L01] 发送 GET 请求
来源：http://vmx.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uep.birdmap.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jgj.yfazqb.com

JS:   await fetch(url)
来源：http://dcr.cheryme.top

TS:   await fetch(url)
来源：http://njv.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qwi.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://sws.bbcook.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sit.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tht.sjlbkw.cn

[L02] 发送 POST JSON
来源：http://hgq.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://zvv.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sdg.redwolf501.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gra.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qgg.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zzi.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pqa.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aew.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yhp.chenlongwang.top

[L03] 设置自定义请求头
来源：http://xls.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fjm.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uzh.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mrv.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ixm.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://njs.snrcjt.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jkp.xuanzx.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lqg.xuetiantiany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://otl.redwolf501.top

[L04] 设置超时
来源：http://lnd.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://raj.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ril.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://imj.cqqwz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lfe.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://usg.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mfo.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://juk.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pro.ybcxt.top

[L05] 上传文件（multipart）
来源：http://mtp.nwbrower.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://isq.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rmf.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uzu.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baf.nanxinkj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ywf.sweek.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://noc.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ceh.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sos.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://qht.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://nkj.sufxvd.cn

PHP:  json_decode($body, true);
来源：http://vmc.redwolf501.top

JS:   await resp.json()
来源：http://lwg.ydzc1.top

TS:   await resp.json()
来源：http://ayx.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aky.jqgufenzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sog.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://hdy.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://goj.tanke756.top

[L07] 处理 HTTP 状态码
来源：http://ojr.nanxuanxn.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kld.shzxlz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ieo.gzhubu.top

JS:   resp.ok;  resp.status
来源：http://stt.chenlongwang.top

TS:   resp.ok;  resp.status
来源：http://qap.andypj.xyz

Java: resp.statusCode()
来源：http://mao.hcnkem.com

Go:   resp.StatusCode
来源：http://kyv.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://bxv.cdnleiting.top

C#:   (int)resp.StatusCode
来源：http://ztg.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://fee.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ppk.ctjpmb.com

PHP:  curl_multi_init() 系列
来源：http://udz.guowangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pou.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kpf.shangyingyoupin.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://scx.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tli.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nzx.cashguo.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dst.gotoacloud.top

================================================================================
来源：http://rzh.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://dfi.xingfuxueyuan.xyz

================================================================================
来源：http://zsm.xinyue.icu

[M01] 读取命令行参数
来源：http://gwu.yj202588.top

Py:   sys.argv[1:]
来源：http://lck.smart0.xyz

PHP:  $argv;  $argc;
来源：http://mvl.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://vum.wangdashe.top

TS:   process.argv.slice(2)
来源：http://glk.ppjwa.cn

Java: args 数组（main 方法参数）
来源：http://ehs.cqqwz.cn

Go:   os.Args[1:]
来源：http://grr.gzhubu.top

Ruby: ARGV
来源：http://bxi.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://psl.ehwqpu.com

[M02] 读取环境变量
来源：http://jjx.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://aid.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sri.havefunace.top

JS:   process.env.HOME
来源：http://rqg.hammf.cn

TS:   process.env.HOME
来源：http://dmm.xuanzx.com

Java: System.getenv("HOME")
来源：http://pma.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sjf.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://ozk.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vwb.feifeiyinyue.top

[M03] 执行外部命令
来源：http://whg.hnxiangtu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zcg.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cdm.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://con.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wzw.yonumen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wtu.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://jra.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ncg.feifeiyinyue.top

C#:   Process.Start("ls", "-l");
来源：http://ryx.bjfxy.top

[M04] 获取当前工作目录
来源：http://mng.ydjk.org.cn

Py:   os.getcwd()
来源：http://ajl.zhixingplan.top

PHP:  getcwd();
来源：http://zha.jinyuanbaomall.cn

JS:   process.cwd()
来源：http://zqx.daria6918.cn

TS:   process.cwd()
来源：http://xat.guowangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://gyo.sxryk.cn

Go:   os.Getwd()
来源：http://iwz.iojbl.cn

Ruby: Dir.pwd
来源：http://rfr.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://qnc.jqgufenzy.top

[M05] 设置退出码
来源：http://akq.jiagoushi.top

Py:   sys.exit(1)
来源：http://dap.redwolf501.top

PHP:  exit(1);
来源：http://qpv.jqgufenzy.top

JS:   process.exit(1)
来源：http://kkj.yangfankeji.com

TS:   process.exit(1)
来源：http://hjq.tanke756.top

Java: System.exit(1)
来源：http://kfc.yueranfly.top

Go:   os.Exit(1)
来源：http://wyy.hesvh.cn

Ruby: exit 1
来源：http://ndf.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kyi.tian-w.cn

[M06] 向标准错误输出
来源：http://hjp.hysaishi.cn

Py:   print("err", file=sys.stderr)
来源：http://uer.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://elt.fzhhl.top

JS:   console.error("err")
来源：http://pks.pengpengdd.cyou

TS:   console.error("err")
来源：http://pgz.yuxming.cn

Java: System.err.println("err")
来源：http://hhb.shanyushiyangtech.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://llm.xuanzx.com

Ruby: warn "err"
来源：http://mtx.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://inc.fengsongda.top

[M07] 判断是否为主入口
来源：http://foh.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://reh.xuanzx.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hgp.ehwqpu.com

JS:   require.main === module
来源：http://ere.ydjk.org.cn

TS:   require.main === module
来源：http://itj.jiagoushi.top

Java: public static void main(String[] args)
来源：http://dva.jinqigfzy.top

Go:   func main()
来源：http://htt.meibo888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gei.zhijiandao.cn

C#:   static void Main(string[] args)
来源：http://gcs.snrcjt.cn

[M08] 获取系统与运行时信息
来源：http://imt.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://zpl.jinyuanbaomall.cn

PHP:  PHP_OS;  phpversion();
来源：http://qky.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://hsf.xinyue.icu

TS:   process.platform;  process.version
来源：http://han.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tyf.jqgfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://puf.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://shx.redwolf501.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://klr.yfazqb.com

================================================================================
来源：http://kqf.hesvh.cn

N. 数据结构与算法
来源：http://zfe.tian-w.cn

================================================================================
来源：http://cjh.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://yqd.yuxming.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rat.hfpthk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hia.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yyw.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jba.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://opn.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://bey.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dmw.yuanzhike.top

C#:   Array.BinarySearch(arr, x)
来源：http://tfu.xinyue.icu

[N02] 排序（工程实践用内置实现）
来源：http://obh.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://jnd.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ihh.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://bhs.fanxiaobao.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://ssq.sufxvd.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zqz.mhx1999.top

Go:   slices.Sort(arr)
来源：http://tmt.cqqwz.cn

Ruby: arr.sort
来源：http://jaq.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rxa.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://yru.hfpthk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wvu.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://fqf.zhengqikj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://emu.aizwys.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wdl.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hqq.iojbl.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mka.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://whv.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://ogt.sjlbkw.cn

[N04] 斐波那契数列
来源：http://gkm.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://grq.yfazqb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ams.sxryk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bee.yj20258.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fxm.jqgfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aeu.cqqwz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xwk.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ejk.jinqigufen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ado.fktsv.cn

[N05] 最大公约数
来源：http://buv.xylfe.cn

Py:   math.gcd(a, b)
来源：http://xao.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jwv.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ooa.hammf.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yvw.fanxiaobao.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://apc.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zmb.jqgufenzy.top

Ruby: a.gcd(b)
来源：http://ypd.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rfr.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://gmj.yueranfly.top

Py:   s == s[::-1]
来源：http://rdg.jinqigfzy.top

PHP:  $s === strrev($s);
来源：http://pbv.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://ulb.birdmap.top

TS:   s === [...s].reverse().join("")
来源：http://qoe.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bim.gaohongyu789.top

Go:   // 双指针从两端比较
来源：http://xnj.ybcxt.top

Ruby: s == s.reverse
来源：http://wtb.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hmi.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://uzy.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lkt.feifeiyinyue.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zci.jyoumei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tag.sysykeji.top

TS:   // 手写 Map<string, number>
来源：http://low.quarkkingdee.top

Java: // 手写 HashMap
来源：http://iic.xingfuxueyuan.xyz

Go:   // 手写 map[int]int
来源：http://zom.hysaishi.cn

Ruby: // 手写 Hash
来源：http://xms.hfpthk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://eii.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://bjw.chenlongwang.top

Py:   itertools.permutations(arr)
来源：http://dyj.shanyushiyangkeji.top

PHP:  // 手写递归交换
来源：http://mvf.jinqigufen.top

JS:   // 手写回溯递归
来源：http://xai.yj20258.top

TS:   // 手写回溯递归
来源：http://xyz.yonumen.top

Java: // 手写回溯递归
来源：http://xtf.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://rnv.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://zdx.tian-w.cn

C#:   // 手写回溯递归
来源：http://grj.yj202588.top

[N09] 栈与队列
来源：http://huy.9152youxi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dwy.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://izu.yuanzhike.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dwb.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vxs.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://klu.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ryy.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nzw.uphjek.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ilr.ybcxt.top

[N10] 链表节点定义
来源：http://qzd.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xpb.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://und.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zyy.jyoumei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yah.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://qsn.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iqk.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ijs.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xxk.birdmap.top

[N11] 二叉树中序遍历
来源：http://bqm.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jwq.epnwcf.com

PHP:  // 手写递归函数
来源：http://spw.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mhf.bjfxy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://clp.zhaomingkeji.xyz

Java: // 手写递归
来源：http://vkq.cheryme.top

Go:   // 手写递归
来源：http://djc.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dsy.bbcook.cn

C#:   // 手写递归
来源：http://gmv.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jof.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iit.smart0.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jgh.ydjk.org.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hma.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://maw.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ora.yfazqb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bmb.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wqo.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://suz.yj20258.top

================================================================================
来源：http://jhb.smart0.xyz

O. 并发与异步
来源：http://zxa.zycfv.cn

================================================================================
来源：http://pbv.feifeiyinyue.top

[O01] 启动一个线程
来源：http://foy.ydzc1.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hzk.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uos.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lym.sjlbkw.cn

TS:   // 同 JS
来源：http://omh.gotoacloud.top


<!-- 参考信息 -->