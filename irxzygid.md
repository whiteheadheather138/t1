代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bmt.tianlin.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iqz.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://lon.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://arp.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ssr.daxiang520.top

Go:   json.Marshal(obj)
来源：http://seu.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://obz.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://pbc.hammf.cn

[K02] JSON 字符串转对象
来源：http://jiu.zhoulong.xyz

Py:   json.loads(s)
来源：http://uwv.cheryme.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nyx.zhixingplan.top

JS:   JSON.parse(s)
来源：http://uig.zycfv.cn

TS:   JSON.parse(s)
来源：http://atl.hywenlv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vyz.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://vms.redwolf501.top

Ruby: JSON.parse(s)
来源：http://nsz.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hze.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://myt.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://god.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xpk.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rks.guowangkeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xks.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pns.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ims.ctjpmb.com

Ruby: JSON.pretty_generate(obj)
来源：http://ymf.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fdk.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://fzv.hywenlv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fdm.quarkkingdee.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gqe.mhx1999.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cnh.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://slr.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cgn.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wye.aibaodan.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rbo.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nwl.cashguo.top

[K05] 深拷贝对象
来源：http://mif.fengsongda.top

Py:   copy.deepcopy(obj)
来源：http://gni.yangfankeji.com

PHP:  unserialize(serialize($obj));
来源：http://xbk.pengpengdd.cyou

JS:   structuredClone(obj)
来源：http://bec.zhengqikj.top

TS:   structuredClone(obj)
来源：http://cga.epnwcf.com

Java: // 手写拷贝构造，或序列化往返
来源：http://aqu.hfpthk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jjh.sufxvd.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oyx.shanyushiyangtech.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jyo.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://bwa.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xtj.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hdx.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jkt.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cqt.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pnd.sysykeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xjf.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aau.sjlbkw.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ald.bbcook.cn

[K07] 进制转换
来源：http://gdv.daria6918.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iev.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dlp.zdbjq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ikk.vqdsnc.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nfm.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ytg.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://clh.yuanzhike.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vnx.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cuz.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://kpi.pycfn.com

Py:   pickle.dumps(obj)
来源：http://wus.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://arz.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://keu.zhijiandao.cn

TS:   v8.serialize(obj)        // Node
来源：http://rov.zhaomingkeji.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zxu.meibo888.top

Go:   encoding/gob
来源：http://ppj.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://ffk.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lwc.yuxming.cn

================================================================================
来源：http://ffs.tarul.cn

L. 网络请求
来源：http://fni.snrcjt.cn

================================================================================
来源：http://yrj.zdbjq.cn

[L01] 发送 GET 请求
来源：http://cly.yj20258888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nse.xylfe.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dbn.cqqwz.cn

JS:   await fetch(url)
来源：http://ldf.ybcxt.top

TS:   await fetch(url)
来源：http://jmj.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tas.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://wfh.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pwr.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://idd.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://bcq.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://pbb.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://epf.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fbu.52xcode.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qik.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://djn.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pty.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qhh.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://edy.hywenlv.cn

[L03] 设置自定义请求头
来源：http://lsu.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ppx.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ooy.nanxuanxn.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jqf.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cye.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://leb.bjfxy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wsj.sufxvd.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://szj.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vuq.316326.xyz

[L04] 设置超时
来源：http://zkv.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://ipq.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cns.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dov.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ifs.nanxuanxn.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kfl.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qve.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oiv.zhixingplan.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pvm.tarul.cn

[L05] 上传文件（multipart）
来源：http://yyj.fengsongda.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qjw.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hnl.jianghu66.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rvt.zycfv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ddn.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vek.jqgufenzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mkm.gzhubu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pgy.cdnleiting.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dsz.sysykeji.top

[L06] 解析响应为 JSON
来源：http://hsi.bjfxy.top

Py:   resp.json()
来源：http://pwt.9152youxi.cn

PHP:  json_decode($body, true);
来源：http://qft.jyoumei.cn

JS:   await resp.json()
来源：http://ara.daxiang520.top

TS:   await resp.json()
来源：http://ssm.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://efq.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jja.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://btw.sufxvd.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jaf.hongshengwenyu.top

[L07] 处理 HTTP 状态码
来源：http://omj.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gak.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wkk.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://xck.zhongyouzk.top

TS:   resp.ok;  resp.status
来源：http://bbp.ctjpmb.com

Java: resp.statusCode()
来源：http://cdi.bbcook.cn

Go:   resp.StatusCode
来源：http://ssu.shuidangran.top

Ruby: resp.code.to_i
来源：http://psj.gogol.net.cn

C#:   (int)resp.StatusCode
来源：http://aqb.pycfn.com

[L08] 并发请求多个地址
来源：http://uut.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qzg.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://htg.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://flv.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uuz.vehdjk.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pex.zhijiandao.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bzw.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dmd.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://umw.tarul.cn

================================================================================
来源：http://nzp.ehwqpu.com

M. 命令行 / 进程 / 环境
来源：http://tzf.yuxming.cn

================================================================================
来源：http://bvm.jinqigufen.top

[M01] 读取命令行参数
来源：http://mzq.zhijiandao.cn

Py:   sys.argv[1:]
来源：http://hyh.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://crt.birdmap.top

JS:   process.argv.slice(2)
来源：http://xlf.yvedp.cn

TS:   process.argv.slice(2)
来源：http://fxq.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://bax.tarul.cn

Go:   os.Args[1:]
来源：http://awl.fengsongda.top

Ruby: ARGV
来源：http://iqb.fanxiaobao.xyz

C#:   args 数组（Main 方法参数）
来源：http://acx.zhoulong.xyz

[M02] 读取环境变量
来源：http://pnr.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://kkx.bjfxy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qhc.ehwqpu.com

JS:   process.env.HOME
来源：http://goo.hnxiangtu.top

TS:   process.env.HOME
来源：http://qxh.guannengcc.top

Java: System.getenv("HOME")
来源：http://xot.fktsv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://duq.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://mfg.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uhu.tian-w.cn

[M03] 执行外部命令
来源：http://cex.ydzc1.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jms.zhongyouzk.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jhq.sxryk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jok.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://jer.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://shz.xinyue.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://wyw.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://loj.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://zwz.hammf.cn

[M04] 获取当前工作目录
来源：http://cgs.hywenlv.cn

Py:   os.getcwd()
来源：http://tsw.shanyushiyangkeji.top

PHP:  getcwd();
来源：http://zxa.yongpay.top

JS:   process.cwd()
来源：http://dni.9152youxi.cn

TS:   process.cwd()
来源：http://jpz.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://cbu.svipenyu.cn

Go:   os.Getwd()
来源：http://uvy.aizwys.cn

Ruby: Dir.pwd
来源：http://iis.ydzc1.top

C#:   Directory.GetCurrentDirectory()
来源：http://ywn.dianchejie.cn

[M05] 设置退出码
来源：http://dkf.wangdashe.top

Py:   sys.exit(1)
来源：http://wrp.guowangkeji.top

PHP:  exit(1);
来源：http://ttz.fzhhl.top

JS:   process.exit(1)
来源：http://gvz.yongpay.top

TS:   process.exit(1)
来源：http://awh.yuanzhike.top

Java: System.exit(1)
来源：http://owl.chenjidiqi.icu

Go:   os.Exit(1)
来源：http://cvp.bbcook.cn

Ruby: exit 1
来源：http://wyd.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gvg.nanxuanxn.top

[M06] 向标准错误输出
来源：http://gyo.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://obj.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://lmo.316326.xyz

JS:   console.error("err")
来源：http://wqz.chenjidiqi.icu

TS:   console.error("err")
来源：http://fte.hnqzz.top

Java: System.err.println("err")
来源：http://kvt.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dqp.aibaodan.cn

Ruby: warn "err"
来源：http://hwt.ivvv.top

C#:   Console.Error.WriteLine("err")
来源：http://zth.yj20258888.top

[M07] 判断是否为主入口
来源：http://fbc.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://sny.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://poe.ivvv.top

JS:   require.main === module
来源：http://tno.jqgufenzy.top

TS:   require.main === module
来源：http://vok.pycfn.com

Java: public static void main(String[] args)
来源：http://ffa.xingfuxueyuan.xyz

Go:   func main()
来源：http://tom.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dcu.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://rxm.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://ikb.shangyingyoupin.top

Py:   platform.system();  platform.python_version()
来源：http://wdd.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://svj.ivvv.top

JS:   process.platform;  process.version
来源：http://prf.pycfn.com

TS:   process.platform;  process.version
来源：http://dxq.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fwu.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ccu.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://alb.uphjek.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://csd.sufxvd.cn

================================================================================
来源：http://ygt.jlsjyb.cn

N. 数据结构与算法
来源：http://wzs.wangshuangyany.cn

================================================================================
来源：http://ati.yuxming.cn

[N01] 二分查找（有序数组）
来源：http://skl.jinqigufen.top

Py:   bisect.bisect_left(arr, x)
来源：http://nbl.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ggw.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://axw.vehdjk.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://brc.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://why.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://yfy.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tew.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://oqu.xinyue.icu

[N02] 排序（工程实践用内置实现）
来源：http://cxj.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://bxa.xylfe.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rzi.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vyf.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yud.yj20258888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nmb.tarul.cn

Go:   slices.Sort(arr)
来源：http://kdf.dianchejie.cn

Ruby: arr.sort
来源：http://lqt.jqgufenzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pzv.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://ohv.guowangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ftz.yueranfly.top

PHP:  // 递归实现，或用 usort
来源：http://jka.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kpi.gogol.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cqn.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rhr.jinghuilouyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kbh.hnxiangtu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kly.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://bzn.havefunace.top

[N04] 斐波那契数列
来源：http://obn.52xcode.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ezj.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kvk.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qml.mhx1999.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iou.shanyushiyangtech.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kkq.hnxiangtu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://opi.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oqu.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://krn.yj202588.top

[N05] 最大公约数
来源：http://qfm.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://lwr.zhijiandao.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jii.zhijiandao.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fgc.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gcq.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://boi.xylfe.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://liw.aizwys.cn

Ruby: a.gcd(b)
来源：http://vsc.jyoumei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lay.cdnleiting.top

[N06] 判断回文字符串
来源：http://vkf.hfpthk.cn

Py:   s == s[::-1]
来源：http://rpp.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://gqo.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://vqj.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://ogo.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dso.zycfv.cn

Go:   // 双指针从两端比较
来源：http://lvs.zhijiandao.cn

Ruby: s == s.reverse
来源：http://zjx.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qgn.wangshuangyany.cn

[N07] 两数之和（返回下标）
来源：http://oqd.zhoulong.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sqp.ehwqpu.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vcx.jiagoushi.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vxp.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://iha.vqdsnc.cn

Java: // 手写 HashMap
来源：http://hjh.cheryme.top

Go:   // 手写 map[int]int
来源：http://qku.guowangkeji.top

Ruby: // 手写 Hash
来源：http://kgg.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://qrh.tianlin.xyz

[N08] 生成全排列
来源：http://xgs.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://twy.gogol.net.cn

PHP:  // 手写递归交换
来源：http://pja.bbcook.cn

JS:   // 手写回溯递归
来源：http://vru.xuetiantiany.cn

TS:   // 手写回溯递归
来源：http://rgu.yj20258.top

Java: // 手写回溯递归
来源：http://yww.fanxiaobao.xyz

Go:   // 手写回溯递归
来源：http://hnr.bbcook.cn

Ruby: arr.permutation.to_a
来源：http://gmz.chenjidiqi.icu

C#:   // 手写回溯递归
来源：http://rml.fengsongda.top

[N09] 栈与队列
来源：http://glq.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aik.guowangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mmq.zhijiandao.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xsx.xziqi.cn


<!-- 参考信息 -->