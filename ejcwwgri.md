代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rsc.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://hzg.epnwcf.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wxr.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mfn.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tsy.quarkkingdee.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gzb.yj20258888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gig.mhx1999.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hly.fktsv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ill.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cva.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://lwp.zhiwuduotai.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://unp.sjlbkw.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://drp.shangyingyoupin.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://agw.9152youxi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yoq.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vfu.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xhz.zdbjq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oeq.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pvi.hcnkem.com

[K05] 深拷贝对象
来源：http://tbl.yangfankeji.com

Py:   copy.deepcopy(obj)
来源：http://rux.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://slp.gotoacloud.top

JS:   structuredClone(obj)
来源：http://lxl.zdqjudy.top

TS:   structuredClone(obj)
来源：http://lux.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://csf.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jjc.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kxl.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gwp.fzhhl.top

[K06] 解析 URL 查询串
来源：http://lpr.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oms.epnwcf.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qwt.tarul.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nul.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gyh.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tnd.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kjx.zhaomingkeji.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tlm.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://loa.jlsjyb.cn

[K07] 进制转换
来源：http://giu.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://amg.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eut.yongpay.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vdl.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mqc.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://epr.jyoumei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://plu.smart0.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xbz.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pog.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://wuf.yj20258888.top

Py:   pickle.dumps(obj)
来源：http://spt.aibaodan.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gvc.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://axr.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://pxj.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kps.vehdjk.com

Go:   encoding/gob
来源：http://hkp.uphjek.com

Ruby: Marshal.dump(obj)
来源：http://qpr.daria6918.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zbw.zhongyouzk.top

================================================================================
来源：http://dtm.xinyue.icu

L. 网络请求
来源：http://ivd.xinyue.icu

================================================================================
来源：http://xgn.uphjek.com

[L01] 发送 GET 请求
来源：http://dhb.shangyingyoupin.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://odb.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uqs.yonumen.top

JS:   await fetch(url)
来源：http://njd.vqdsnc.cn

TS:   await fetch(url)
来源：http://xrf.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jof.hysaishi.cn

Go:   resp, err := http.Get(url)
来源：http://aua.jinghuilouyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sxa.wangdashe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bat.tian-w.cn

[L02] 发送 POST JSON
来源：http://rxy.zhixingplan.top

Py:   requests.post(url, json={"a": 1})
来源：http://fyv.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kyo.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bkz.chenlongwang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rnm.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xrc.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lfl.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hnl.redwolf501.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://huz.dashuyun.cn

[L03] 设置自定义请求头
来源：http://avw.tianlin.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cro.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cuf.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kqa.havefunace.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vsw.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mdb.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kyg.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://htq.ydjk.org.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://whi.jqgfzy.top

[L04] 设置超时
来源：http://fhr.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://gjl.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://smd.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gfu.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://byx.fehbvm.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dip.snrcjt.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ezl.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aql.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ujd.vehdjk.com

[L05] 上传文件（multipart）
来源：http://bbv.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://smf.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pkr.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mkt.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vil.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uws.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pic.xylfe.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rtp.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://njz.sweek.top

[L06] 解析响应为 JSON
来源：http://bqd.zhiwuduotai.top

Py:   resp.json()
来源：http://fjx.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://goa.yanxiufei.cn

JS:   await resp.json()
来源：http://fog.jinyuanbaomall.cn

TS:   await resp.json()
来源：http://cwq.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kwc.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lgv.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://zhw.yj20258.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bcq.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://fmc.sweek.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://czq.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rgd.sufxvd.cn

JS:   resp.ok;  resp.status
来源：http://zvz.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://oso.jinghuilouyu.cn

Java: resp.statusCode()
来源：http://gwj.aibaodan.cn

Go:   resp.StatusCode
来源：http://xpk.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://slh.svipenyu.cn

C#:   (int)resp.StatusCode
来源：http://unl.guowangkeji.top

[L08] 并发请求多个地址
来源：http://mzj.dianchejie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lxk.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://oom.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://noj.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eis.uphjek.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://est.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jcl.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fik.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://msd.wangdashe.top

================================================================================
来源：http://bfu.jinqigufen.top

M. 命令行 / 进程 / 环境
来源：http://fye.bjfxy.top

================================================================================
来源：http://grz.cashguo.top

[M01] 读取命令行参数
来源：http://ord.cdnleiting.top

Py:   sys.argv[1:]
来源：http://xuq.yangfankeji.com

PHP:  $argv;  $argc;
来源：http://krd.zycfv.cn

JS:   process.argv.slice(2)
来源：http://jlv.fehbvm.com

TS:   process.argv.slice(2)
来源：http://dzh.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://qev.haohaochexian.top

Go:   os.Args[1:]
来源：http://usl.yj20258.top

Ruby: ARGV
来源：http://pqt.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://wuq.cheryme.top

[M02] 读取环境变量
来源：http://qsr.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://ksc.yangfankeji.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ozp.ydjk.org.cn

JS:   process.env.HOME
来源：http://fag.ydzc1.top

TS:   process.env.HOME
来源：http://mba.gzhubu.top

Java: System.getenv("HOME")
来源：http://knt.sysykeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zsi.zhiwuduotai.top

Ruby: ENV["HOME"]
来源：http://czx.cucudq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xhm.gaohongyu789.top

[M03] 执行外部命令
来源：http://jiu.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pmm.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bsg.cdnleiting.top

JS:   child_process.execSync("ls -l").toString()
来源：http://las.zhongyouzk.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kxa.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zcl.dianchejie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kll.ctjpmb.com

Ruby: system("ls -l");  `ls -l`
来源：http://soh.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://ehd.yueranfly.top

[M04] 获取当前工作目录
来源：http://sds.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://suy.c1oappe.top

PHP:  getcwd();
来源：http://eqb.jinqigfzy.top

JS:   process.cwd()
来源：http://vyq.guannengcc.top

TS:   process.cwd()
来源：http://huv.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://epp.yongpay.top

Go:   os.Getwd()
来源：http://ixb.shangyingyoupin.top

Ruby: Dir.pwd
来源：http://wjv.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://hzn.ydjk.org.cn

[M05] 设置退出码
来源：http://vbl.zhoulong.xyz

Py:   sys.exit(1)
来源：http://zme.zhengqikj.top

PHP:  exit(1);
来源：http://peu.andypj.xyz

JS:   process.exit(1)
来源：http://kio.wangdashe.top

TS:   process.exit(1)
来源：http://snw.jinyuanbaomall.cn

Java: System.exit(1)
来源：http://cql.dianchejie.cn

Go:   os.Exit(1)
来源：http://nvw.jianghu66.top

Ruby: exit 1
来源：http://ojq.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yto.hnxiangtu.top

[M06] 向标准错误输出
来源：http://wzo.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://say.chenzaomai.com

PHP:  fwrite(STDERR, "err\n");
来源：http://crs.redwolf501.top

JS:   console.error("err")
来源：http://dpf.jiagoushi.top

TS:   console.error("err")
来源：http://izt.ctjpmb.com

Java: System.err.println("err")
来源：http://arj.fanxiaobao.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ukk.jlsjyb.cn

Ruby: warn "err"
来源：http://czh.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://kol.fehbvm.com

[M07] 判断是否为主入口
来源：http://yxh.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://cqi.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jev.yuanzhike.top

JS:   require.main === module
来源：http://vle.jqgfzy.top

TS:   require.main === module
来源：http://xds.zycfv.cn

Java: public static void main(String[] args)
来源：http://nto.ppjwa.cn

Go:   func main()
来源：http://quy.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qwy.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://lyg.kuanghao11.cn

[M08] 获取系统与运行时信息
来源：http://mlk.hcnkem.com

Py:   platform.system();  platform.python_version()
来源：http://nup.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://rsz.jinqigufen.top

JS:   process.platform;  process.version
来源：http://ihy.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://umj.gogol.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aoq.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://aik.zhoulong.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gpv.andypj.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://ikm.yj202588.top

================================================================================
来源：http://yiy.epnwcf.com

N. 数据结构与算法
来源：http://ogc.aibaodan.cn

================================================================================
来源：http://tjd.sxryk.cn

[N01] 二分查找（有序数组）
来源：http://dno.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uby.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tmr.xingfuxueyuan.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pob.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dje.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xxt.feifeiyinyue.top

Go:   sort.SearchInts(arr, x)
来源：http://ldp.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kxu.bbcook.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xsk.316326.xyz

[N02] 排序（工程实践用内置实现）
来源：http://esp.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://pph.xingfuxueyuan.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vrv.zhaomingkeji.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://whg.ivvv.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rkp.nanxinkj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://isc.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://wij.vqdsnc.cn

Ruby: arr.sort
来源：http://aoj.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bfx.havefunace.top

[N03] 快速排序（分治示例）
来源：http://stf.havefunace.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://drc.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://qei.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tgw.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qfs.yuanzhike.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qug.guowangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jkc.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://phh.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yqz.jinqigfzy.top

[N04] 斐波那契数列
来源：http://wdl.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zcj.ydzc1.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gzf.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://chn.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fdi.xziqi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yls.pycfn.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wrs.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tow.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wfi.fktsv.cn

[N05] 最大公约数
来源：http://bol.havefunace.top

Py:   math.gcd(a, b)
来源：http://zrk.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zbn.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fti.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://get.cqqwz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ccf.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pdc.kuanghao11.cn

Ruby: a.gcd(b)
来源：http://ibz.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lro.vehdjk.com

[N06] 判断回文字符串
来源：http://kfz.pengpengdd.cyou

Py:   s == s[::-1]
来源：http://ush.sufxvd.cn

PHP:  $s === strrev($s);
来源：http://ijy.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://utj.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://bon.ydjk.org.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rwy.xziqi.cn

Go:   // 双指针从两端比较
来源：http://bcv.hesvh.cn

Ruby: s == s.reverse
来源：http://nad.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://oja.epnwcf.com

[N07] 两数之和（返回下标）
来源：http://dpv.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ejn.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xjc.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cha.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://jjp.nanxinkj.top

Java: // 手写 HashMap
来源：http://hit.cashguo.top

Go:   // 手写 map[int]int
来源：http://tja.nanxinkj.top

Ruby: // 手写 Hash
来源：http://ulk.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://xpp.fzhhl.top

[N08] 生成全排列
来源：http://jyn.hysaishi.cn

Py:   itertools.permutations(arr)
来源：http://ebe.meibo888.top

PHP:  // 手写递归交换
来源：http://oqh.hysaishi.cn

JS:   // 手写回溯递归
来源：http://xkb.cdnleiting.top

TS:   // 手写回溯递归
来源：http://tyd.shangyingyoupin.top

Java: // 手写回溯递归
来源：http://csu.gzhubu.top

Go:   // 手写回溯递归
来源：http://zbw.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://jok.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://sbn.mhx1999.top

[N09] 栈与队列
来源：http://hxk.cheryme.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rwx.ydjk.org.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://haf.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zjd.jinqigfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ewa.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dcz.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ynn.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qqg.sysykeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kkc.chenlongwang.top

[N10] 链表节点定义
来源：http://gzf.wangdashe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sxp.ywan-chungtsiang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://enb.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://icw.tarul.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oob.hnxiangtu.top

Java: class Node { int v; Node next; }
来源：http://img.gzhubu.top

Go:   type Node struct { V int; Next *Node }
来源：http://ymy.ydzc1.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tkz.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ipj.yuxming.cn

[N11] 二叉树中序遍历
来源：http://bmm.mhx1999.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nof.jinyuanbaomall.cn


<!-- 参考信息 -->