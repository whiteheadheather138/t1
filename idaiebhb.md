代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nxp.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://mxy.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lbj.snrcjt.cn

[K05] 深拷贝对象
来源：http://ino.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://tlw.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://log.tian-w.cn

JS:   structuredClone(obj)
来源：http://wfk.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://tpt.yuxming.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xur.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rug.fengsongda.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ovg.shzxlz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rru.jinqigufen.top

[K06] 解析 URL 查询串
来源：http://dqo.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iwb.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fab.gotoacloud.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://agz.bbcook.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eos.shzxlz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vdn.vehdjk.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://bag.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zrh.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ohk.pycfn.com

[K07] 进制转换
来源：http://yce.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mni.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pxt.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dso.jqgufenzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kdj.zhijiandao.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ous.yj202588.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yvm.cucudq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://igo.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gmo.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://fxy.yonumen.top

Py:   pickle.dumps(obj)
来源：http://zoc.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cfo.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://yni.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://ete.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://krv.xinyue.icu

Go:   encoding/gob
来源：http://hym.sweek.top

Ruby: Marshal.dump(obj)
来源：http://onc.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zka.yfazqb.com

================================================================================
来源：http://stc.yfazqb.com

L. 网络请求
来源：http://lli.hnqzz.top

================================================================================
来源：http://brv.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://dtg.ydzc1.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rrk.epnwcf.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bgx.xuanzx.com

JS:   await fetch(url)
来源：http://pys.daxiang520.top

TS:   await fetch(url)
来源：http://dxv.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wuo.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://ilh.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://arj.cheryme.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qrx.bbcook.cn

[L02] 发送 POST JSON
来源：http://tks.chenlongwang.top

Py:   requests.post(url, json={"a": 1})
来源：http://cdx.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kqd.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tnu.shanyushiyangtech.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mhb.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tza.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ypl.xingfuxueyuan.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ndp.hfpthk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://esa.sweek.top

[L03] 设置自定义请求头
来源：http://sdr.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gfe.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nnm.jinqigfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xgf.yfazqb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://laz.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://urt.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bpc.daxiang520.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://did.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fkw.bbcook.cn

[L04] 设置超时
来源：http://ujs.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://bry.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mon.andypj.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ahq.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ybt.gaohongyu789.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oms.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pcm.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hht.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lsm.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://kuf.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hsp.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tre.jinghuilouyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cwc.zhiwuduotai.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uie.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dgy.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jwv.tianlin.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lpj.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lpv.smart0.xyz

[L06] 解析响应为 JSON
来源：http://trc.ivvv.top

Py:   resp.json()
来源：http://iwv.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://sve.ydjk.org.cn

JS:   await resp.json()
来源：http://pet.yj202588.top

TS:   await resp.json()
来源：http://xni.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vkw.cqqwz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dck.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://rse.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ykc.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://ofx.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://akm.fktsv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://koy.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://wmm.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://jyt.ywan-chungtsiang.top

Java: resp.statusCode()
来源：http://bwq.cheryme.top

Go:   resp.StatusCode
来源：http://szz.yuanzhike.top

Ruby: resp.code.to_i
来源：http://fqs.cheryme.top

C#:   (int)resp.StatusCode
来源：http://dmk.guannengcc.top

[L08] 并发请求多个地址
来源：http://gmd.jinqigfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nsn.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://frz.jinghuilouyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://znu.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vwd.0kj1m.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vns.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fnk.zhengqikj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jxn.nanxinkj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://npk.feifeiyinyue.top

================================================================================
来源：http://olb.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://vyj.jinghuilouyu.cn

================================================================================
来源：http://dgt.daxiang520.top

[M01] 读取命令行参数
来源：http://tag.ppjwa.cn

Py:   sys.argv[1:]
来源：http://fum.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://rbi.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://mux.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://aov.fktsv.cn

Java: args 数组（main 方法参数）
来源：http://lli.snrcjt.cn

Go:   os.Args[1:]
来源：http://ojw.ppjwa.cn

Ruby: ARGV
来源：http://rfd.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://nrv.hfpthk.cn

[M02] 读取环境变量
来源：http://fhk.jinyuanbaomall.cn

Py:   os.environ.get("HOME")
来源：http://ckd.xuetiantiany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fuy.meibo888.top

JS:   process.env.HOME
来源：http://asq.ppjwa.cn

TS:   process.env.HOME
来源：http://xma.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://xwq.feifeiyinyue.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hjz.zhijiandao.cn

Ruby: ENV["HOME"]
来源：http://sdp.cucudq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jlr.yueranfly.top

[M03] 执行外部命令
来源：http://ucw.aizwys.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://awm.cucudq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dnt.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://doq.kuanghao11.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jwg.jiagoushi.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hgs.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xse.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vis.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://vad.zdbjq.cn

[M04] 获取当前工作目录
来源：http://vqm.shanyushiyangkeji.top

Py:   os.getcwd()
来源：http://gqy.birdmap.top

PHP:  getcwd();
来源：http://lxo.yj20258.top

JS:   process.cwd()
来源：http://wra.zhiwuduotai.top

TS:   process.cwd()
来源：http://pdg.zhoulong.xyz

Java: Path.of("").toAbsolutePath()
来源：http://mhn.ivvv.top

Go:   os.Getwd()
来源：http://ymq.zdqjudy.top

Ruby: Dir.pwd
来源：http://aeq.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://vxe.xuetiantiany.cn

[M05] 设置退出码
来源：http://dqo.hywenlv.cn

Py:   sys.exit(1)
来源：http://ybz.havefunace.top

PHP:  exit(1);
来源：http://jpq.pengpengdd.cyou

JS:   process.exit(1)
来源：http://dvq.jinqigufen.top

TS:   process.exit(1)
来源：http://cao.cdnleiting.top

Java: System.exit(1)
来源：http://nte.gzhubu.top

Go:   os.Exit(1)
来源：http://cin.svipenyu.cn

Ruby: exit 1
来源：http://lxl.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://urg.zdqjudy.top

[M06] 向标准错误输出
来源：http://rgl.ehwqpu.com

Py:   print("err", file=sys.stderr)
来源：http://ija.daria6918.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sxk.tarul.cn

JS:   console.error("err")
来源：http://sut.jqgfzy.top

TS:   console.error("err")
来源：http://juz.jinqigufen.top

Java: System.err.println("err")
来源：http://las.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zta.aibaodan.cn

Ruby: warn "err"
来源：http://nfi.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://xgx.dashuyun.cn

[M07] 判断是否为主入口
来源：http://ixf.zhoulong.xyz

Py:   if __name__ == "__main__":
来源：http://prl.zhijiandao.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lpw.svipenyu.cn

JS:   require.main === module
来源：http://vdd.vehdjk.com

TS:   require.main === module
来源：http://rfd.gotoacloud.top

Java: public static void main(String[] args)
来源：http://gxy.pycfn.com

Go:   func main()
来源：http://mco.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dod.svipenyu.cn

C#:   static void Main(string[] args)
来源：http://fqv.xuetiantiany.cn

[M08] 获取系统与运行时信息
来源：http://ztx.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://kwb.dianchejie.cn

PHP:  PHP_OS;  phpversion();
来源：http://pnt.snrcjt.cn

JS:   process.platform;  process.version
来源：http://qoa.yuxming.cn

TS:   process.platform;  process.version
来源：http://hhf.jinqigufen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vln.sjlbkw.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ltc.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wnk.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sas.guannengcc.top

================================================================================
来源：http://hnk.cheryme.top

N. 数据结构与算法
来源：http://hcf.yj20258.top

================================================================================
来源：http://dfg.bjfxy.top

[N01] 二分查找（有序数组）
来源：http://wgh.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://udb.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eqp.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xri.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ghu.ivvv.top

Java: Arrays.binarySearch(arr, x)
来源：http://oge.epnwcf.com

Go:   sort.SearchInts(arr, x)
来源：http://ftq.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jkg.jinqigufen.top

C#:   Array.BinarySearch(arr, x)
来源：http://svh.daria6918.cn

[N02] 排序（工程实践用内置实现）
来源：http://hnr.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://baj.hfpthk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cut.xinyue.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://rio.yongpay.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qha.hnqzz.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cja.sweek.top

Go:   slices.Sort(arr)
来源：http://pli.guowangkeji.top

Ruby: arr.sort
来源：http://vrc.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ndr.epnwcf.com

[N03] 快速排序（分治示例）
来源：http://ikw.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gnu.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://hqi.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qzh.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wab.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jmt.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xcx.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wjm.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://haj.nwbrower.top

[N04] 斐波那契数列
来源：http://xgc.xylfe.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fdt.quarkkingdee.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qjz.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jev.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pfw.zhaomingkeji.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qvj.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://llp.sysykeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yez.sjlbkw.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ocv.pycfn.com

[N05] 最大公约数
来源：http://mpe.fktsv.cn

Py:   math.gcd(a, b)
来源：http://uee.shzxlz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fmp.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gji.sufxvd.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://huy.yj20258.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qls.epnwcf.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://csq.9152youxi.cn

Ruby: a.gcd(b)
来源：http://aqt.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://udc.9152youxi.cn

[N06] 判断回文字符串
来源：http://xae.hysaishi.cn

Py:   s == s[::-1]
来源：http://kfy.hesvh.cn

PHP:  $s === strrev($s);
来源：http://ciu.jiagoushi.top

JS:   s === [...s].reverse().join("")
来源：http://cvu.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://idm.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uib.ywan-chungtsiang.top

Go:   // 双指针从两端比较
来源：http://zqs.uphjek.com

Ruby: s == s.reverse
来源：http://mhe.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rsv.yanxiufei.cn

[N07] 两数之和（返回下标）
来源：http://oxz.cqqwz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://frp.shanyushiyangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ffn.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://qma.guowangkeji.top

TS:   // 手写 Map<string, number>
来源：http://eud.hysaishi.cn

Java: // 手写 HashMap
来源：http://yun.fzhhl.top

Go:   // 手写 map[int]int
来源：http://tju.xuanzx.com

Ruby: // 手写 Hash
来源：http://xzg.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gay.cheryme.top

[N08] 生成全排列
来源：http://msu.yj20258888.top

Py:   itertools.permutations(arr)
来源：http://adq.jlsjyb.cn

PHP:  // 手写递归交换
来源：http://wcc.yuxming.cn

JS:   // 手写回溯递归
来源：http://wbd.c1oappe.top

TS:   // 手写回溯递归
来源：http://one.jinqigufen.top

Java: // 手写回溯递归
来源：http://lvb.zhaomingkeji.xyz

Go:   // 手写回溯递归
来源：http://hsz.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://elt.sufxvd.cn

C#:   // 手写回溯递归
来源：http://kgp.fktsv.cn

[N09] 栈与队列
来源：http://med.chenlongwang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pzr.52xcode.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wpc.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dzw.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ixc.svipenyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lcp.quarkkingdee.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lmm.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vzj.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tgm.zhaomingkeji.xyz

[N10] 链表节点定义
来源：http://kxv.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mcn.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://rdr.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://izc.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bzd.hywenlv.cn

Java: class Node { int v; Node next; }
来源：http://zrw.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://sak.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://phu.yanxiufei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://iyf.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://fup.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hit.gotoacloud.top

PHP:  // 手写递归函数
来源：http://kyu.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://acw.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oha.gaohongyu789.top

Java: // 手写递归
来源：http://nhb.0kj1m.cn

Go:   // 手写递归
来源：http://adf.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rmy.tian-w.cn

C#:   // 手写递归
来源：http://mmt.xinyue.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nqe.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mdt.vqdsnc.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jbp.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dsw.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zck.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ccl.fzhhl.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gmy.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eej.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://orm.zhoulong.xyz


<!-- 参考信息 -->