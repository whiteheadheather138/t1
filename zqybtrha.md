代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uky.zhiwuduotai.top

[K03] JSON 美化输出（带缩进）
来源：http://des.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gfm.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://alq.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vqt.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wmm.jyoumei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qux.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cjh.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://orr.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ysd.chenzaomai.com

[K04] 读取 JSON 文件
来源：http://dvl.haohaochexian.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dgm.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qjj.mhx1999.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dnm.cashguo.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://raw.ydzc1.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kmv.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lwr.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://auh.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xxx.hnqzz.top

[K05] 深拷贝对象
来源：http://iwb.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://ugx.yj202588.top

PHP:  unserialize(serialize($obj));
来源：http://mpl.wangshuangyany.cn

JS:   structuredClone(obj)
来源：http://msb.yueranfly.top

TS:   structuredClone(obj)
来源：http://tcz.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://arl.fehbvm.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vqd.hesvh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wxc.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://oqo.chenjidiqi.icu

[K06] 解析 URL 查询串
来源：http://ohk.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tjp.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qmv.gogol.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://khk.bjfxy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vze.jianghu66.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://agm.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://abn.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tqx.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jke.shangyingyoupin.top

[K07] 进制转换
来源：http://rpi.hnxiangtu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iax.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ckr.yvedp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ztv.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://otx.cashguo.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://idj.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rjs.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bng.jiagoushi.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oeh.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://lki.zycfv.cn

Py:   pickle.dumps(obj)
来源：http://dbk.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qdb.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://dln.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://lee.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nvd.hysaishi.cn

Go:   encoding/gob
来源：http://bsd.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://dzt.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dfv.xuetiantiany.cn

================================================================================
来源：http://zgg.meibo888.top

L. 网络请求
来源：http://lop.fehbvm.com

================================================================================
来源：http://dsg.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://iac.xuanzx.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ehn.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qbo.jinqigufen.top

JS:   await fetch(url)
来源：http://zmq.xuetiantiany.cn

TS:   await fetch(url)
来源：http://rzs.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dkh.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://pid.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://obt.meibo888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qnq.sweek.top

[L02] 发送 POST JSON
来源：http://zxs.smart0.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://veh.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mgj.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zlq.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zfh.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yhq.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mxt.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hts.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xxz.hesvh.cn

[L03] 设置自定义请求头
来源：http://wxb.havefunace.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pwo.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ujp.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uym.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tpn.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ono.yanxiufei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://amn.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jpk.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wkj.aibaodan.cn

[L04] 设置超时
来源：http://lej.yuxming.cn

Py:   requests.get(url, timeout=5)
来源：http://mxg.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tmo.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wfq.hywenlv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tas.hammf.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tsh.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mhu.hcnkem.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://caf.iojbl.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cvr.birdmap.top

[L05] 上传文件（multipart）
来源：http://xpw.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zfz.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rbz.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hmb.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ryb.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zfv.cdnleiting.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uws.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fxw.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oud.sxryk.cn

[L06] 解析响应为 JSON
来源：http://htb.yj202588.top

Py:   resp.json()
来源：http://yhv.gzhubu.top

PHP:  json_decode($body, true);
来源：http://uaj.yanxiufei.cn

JS:   await resp.json()
来源：http://cyh.shzxlz.cn

TS:   await resp.json()
来源：http://zih.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nez.xuetiantiany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bqq.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://tni.hammf.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nca.cucudq.cn

[L07] 处理 HTTP 状态码
来源：http://yks.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fvn.hnxiangtu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blo.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://tmx.nwbrower.top

TS:   resp.ok;  resp.status
来源：http://tqx.yueranfly.top

Java: resp.statusCode()
来源：http://abj.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://hig.ybcxt.top

Ruby: resp.code.to_i
来源：http://pcf.yfazqb.com

C#:   (int)resp.StatusCode
来源：http://mmu.nanxinkj.top

[L08] 并发请求多个地址
来源：http://lkg.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://epw.zhengqikj.top

PHP:  curl_multi_init() 系列
来源：http://ebr.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hpk.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dgx.vehdjk.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://idb.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bdk.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://skx.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pmo.sweek.top

================================================================================
来源：http://ebl.svipenyu.cn

M. 命令行 / 进程 / 环境
来源：http://jdt.hysaishi.cn

================================================================================
来源：http://uwx.andypj.xyz

[M01] 读取命令行参数
来源：http://hkg.jiagoushi.top

Py:   sys.argv[1:]
来源：http://ejn.ybcxt.top

PHP:  $argv;  $argc;
来源：http://aru.zhaomingkeji.xyz

JS:   process.argv.slice(2)
来源：http://mrq.yj20258.top

TS:   process.argv.slice(2)
来源：http://uzl.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://pvu.guowangkeji.top

Go:   os.Args[1:]
来源：http://itu.jianghu66.top

Ruby: ARGV
来源：http://cxz.jinqigufen.top

C#:   args 数组（Main 方法参数）
来源：http://jbc.jinyuanbaomall.cn

[M02] 读取环境变量
来源：http://hmz.c1oappe.top

Py:   os.environ.get("HOME")
来源：http://mwy.chenlongwang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://krt.jiagoushi.top

JS:   process.env.HOME
来源：http://tet.gaohongyu789.top

TS:   process.env.HOME
来源：http://rcl.nanxinkj.top

Java: System.getenv("HOME")
来源：http://dse.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vtg.jianghu66.top

Ruby: ENV["HOME"]
来源：http://cgl.bbcook.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tlm.ywan-chungtsiang.top

[M03] 执行外部命令
来源：http://cwy.9152youxi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zpm.hysaishi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kuz.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rdd.cashguo.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xyx.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qbv.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hbp.sysykeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://vet.pycfn.com

C#:   Process.Start("ls", "-l");
来源：http://gpz.zhongyouzk.top

[M04] 获取当前工作目录
来源：http://mmv.pengpengdd.cyou

Py:   os.getcwd()
来源：http://hhp.316326.xyz

PHP:  getcwd();
来源：http://icr.nanxuanxn.top

JS:   process.cwd()
来源：http://hhv.zhaomingkeji.xyz

TS:   process.cwd()
来源：http://amw.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://xxr.ydjk.org.cn

Go:   os.Getwd()
来源：http://ebu.jinqigfzy.top

Ruby: Dir.pwd
来源：http://syo.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bjp.jinqigfzy.top

[M05] 设置退出码
来源：http://mwe.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://lhb.hysaishi.cn

PHP:  exit(1);
来源：http://guj.hesvh.cn

JS:   process.exit(1)
来源：http://mpz.uphjek.com

TS:   process.exit(1)
来源：http://pyl.hnxiangtu.top

Java: System.exit(1)
来源：http://alc.sysykeji.top

Go:   os.Exit(1)
来源：http://ndg.jianghu66.top

Ruby: exit 1
来源：http://lls.tarul.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fch.cqqwz.cn

[M06] 向标准错误输出
来源：http://fgu.wangshuangyany.cn

Py:   print("err", file=sys.stderr)
来源：http://phn.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://mfg.hywenlv.cn

JS:   console.error("err")
来源：http://ehv.chenzaomai.com

TS:   console.error("err")
来源：http://htp.hfpthk.cn

Java: System.err.println("err")
来源：http://xck.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yox.jlsjyb.cn

Ruby: warn "err"
来源：http://rof.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://arv.fzhhl.top

[M07] 判断是否为主入口
来源：http://oub.hnqzz.top

Py:   if __name__ == "__main__":
来源：http://fll.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://koh.xylfe.cn

JS:   require.main === module
来源：http://hdq.pengpengdd.cyou

TS:   require.main === module
来源：http://kus.yangfankeji.com

Java: public static void main(String[] args)
来源：http://aot.shuidangran.top

Go:   func main()
来源：http://fmu.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hks.yonumen.top

C#:   static void Main(string[] args)
来源：http://osx.zhoulong.xyz

[M08] 获取系统与运行时信息
来源：http://sac.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://wwq.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://muy.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://hgx.cashguo.top

TS:   process.platform;  process.version
来源：http://szk.jqgufenzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bwk.epnwcf.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://gad.jlsjyb.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lrj.jinghuilouyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ggj.ydjk.org.cn

================================================================================
来源：http://cpu.aibaodan.cn

N. 数据结构与算法
来源：http://llu.zhijiandao.cn

================================================================================
来源：http://bne.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://zgk.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://gal.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hhh.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vrb.yanxiufei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mvz.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cih.chenjidiqi.icu

Go:   sort.SearchInts(arr, x)
来源：http://swq.jinqigufen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ozo.bbcook.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cso.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://tni.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://cwe.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tij.hnxiangtu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ayd.hongshengwenyu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rda.vqdsnc.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ljd.fzhhl.top

Go:   slices.Sort(arr)
来源：http://zon.xuanzx.com

Ruby: arr.sort
来源：http://wny.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tbj.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://tof.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mfr.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://slh.zhaomingkeji.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nzn.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iow.vehdjk.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://djn.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gah.fanxiaobao.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wzx.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xco.daxiang520.top

[N04] 斐波那契数列
来源：http://pxv.sweek.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pzf.gotoacloud.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dfz.yongpay.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qdu.jinqigfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://umd.zdqjudy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qag.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tzy.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mdp.kuanghao11.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bkv.redwolf501.top

[N05] 最大公约数
来源：http://hfa.meibo888.top

Py:   math.gcd(a, b)
来源：http://dgk.mhx1999.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qao.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zuu.dianchejie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://anv.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xkz.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hhl.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://dnn.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qmu.hysaishi.cn

[N06] 判断回文字符串
来源：http://svq.dashuyun.cn

Py:   s == s[::-1]
来源：http://ote.cdnleiting.top

PHP:  $s === strrev($s);
来源：http://qvh.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://hrr.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://fsn.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aqh.wangshuangyany.cn

Go:   // 双指针从两端比较
来源：http://mwg.guowangkeji.top

Ruby: s == s.reverse
来源：http://znc.sufxvd.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qwy.pycfn.com

[N07] 两数之和（返回下标）
来源：http://ibf.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rse.yj202588.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xln.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ksi.jlsjyb.cn

TS:   // 手写 Map<string, number>
来源：http://gyz.yuxming.cn

Java: // 手写 HashMap
来源：http://oqn.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://rvf.yfazqb.com

Ruby: // 手写 Hash
来源：http://hwc.aizwys.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iuu.yuanzhike.top

[N08] 生成全排列
来源：http://zlz.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://imp.fehbvm.com

PHP:  // 手写递归交换
来源：http://vmf.aibaodan.cn

JS:   // 手写回溯递归
来源：http://tmh.cheryme.top

TS:   // 手写回溯递归
来源：http://wmj.tarul.cn

Java: // 手写回溯递归
来源：http://leq.ivvv.top

Go:   // 手写回溯递归
来源：http://ieq.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://uft.hfpthk.cn

C#:   // 手写回溯递归
来源：http://ywm.cqqwz.cn

[N09] 栈与队列
来源：http://qnr.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yqj.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://csc.tanke756.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tpk.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lmg.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cvs.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rim.jyoumei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lkd.vehdjk.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uhl.yj202588.top

[N10] 链表节点定义
来源：http://ylf.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qsy.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://zmn.feifeiyinyue.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ifu.zdbjq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ayt.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://wui.52xcode.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yec.yuanzhike.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qfw.zycfv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bmt.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://bxm.cucudq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dxp.fanxiaobao.xyz


<!-- 参考信息 -->