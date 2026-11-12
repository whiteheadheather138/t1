代发 wailian999

TS:   JSON.parse(s)
来源：http://edv.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ewx.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://snp.andypj.xyz

Ruby: JSON.parse(s)
来源：http://ork.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yfj.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://vrt.hnxiangtu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cvc.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lle.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rnx.andypj.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://mrb.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://okl.havefunace.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jnr.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://npu.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dvw.ctjpmb.com

[K04] 读取 JSON 文件
来源：http://boa.cdnleiting.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ten.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dwm.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ilz.tianlin.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wwb.sufxvd.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fbe.ybcxt.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yzp.aibaodan.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kfc.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rfw.shuidangran.top

[K05] 深拷贝对象
来源：http://shs.ppjwa.cn

Py:   copy.deepcopy(obj)
来源：http://vyd.tarul.cn

PHP:  unserialize(serialize($obj));
来源：http://kzl.guowangkeji.top

JS:   structuredClone(obj)
来源：http://bqm.xingfuxueyuan.xyz

TS:   structuredClone(obj)
来源：http://sot.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ani.fktsv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nyj.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nmz.chenjidiqi.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://jmt.sufxvd.cn

[K06] 解析 URL 查询串
来源：http://ryh.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fwt.cqqwz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vez.fzhhl.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://trf.yangfankeji.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://opd.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ull.jinqigfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wvv.aibaodan.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rim.snrcjt.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://glm.vehdjk.com

[K07] 进制转换
来源：http://ike.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://awh.gzhubu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pox.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://icd.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pzn.sysykeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qbd.bjfxy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bij.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qvn.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tkd.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://dgg.fehbvm.com

Py:   pickle.dumps(obj)
来源：http://wqw.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nya.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://say.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://bcb.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rfq.wangshuangyany.cn

Go:   encoding/gob
来源：http://dmo.birdmap.top

Ruby: Marshal.dump(obj)
来源：http://ofx.yueranfly.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vjy.xuetiantiany.cn

================================================================================
来源：http://mzs.yfazqb.com

L. 网络请求
来源：http://wer.nanxinkj.top

================================================================================
来源：http://qjv.hesvh.cn

[L01] 发送 GET 请求
来源：http://wny.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ngn.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://roe.yuxming.cn

JS:   await fetch(url)
来源：http://jny.andypj.xyz

TS:   await fetch(url)
来源：http://uyl.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yjl.zycfv.cn

Go:   resp, err := http.Get(url)
来源：http://mqs.daria6918.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xzt.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zyh.redwolf501.top

[L02] 发送 POST JSON
来源：http://glz.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bhz.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ywt.redwolf501.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bhi.52xcode.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oeg.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tqi.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yod.cdnleiting.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mpx.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mxc.jqgfzy.top

[L03] 设置自定义请求头
来源：http://bmd.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yoe.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eln.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://clb.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fww.yj202588.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://srq.guowangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fpa.zycfv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ozm.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mdw.shanyushiyangkeji.top

[L04] 设置超时
来源：http://jvm.sjlbkw.cn

Py:   requests.get(url, timeout=5)
来源：http://xro.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mmx.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zxf.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://omn.hfpthk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pyx.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://anu.zdbjq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zyc.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gvg.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://dwz.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lgz.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://khj.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kdk.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xtz.zdbjq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vui.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kve.jinqigfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sje.guowangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eyf.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://bru.feifeiyinyue.top

Py:   resp.json()
来源：http://yjf.quarkkingdee.top

PHP:  json_decode($body, true);
来源：http://kvm.shzxlz.cn

JS:   await resp.json()
来源：http://xtr.epnwcf.com

TS:   await resp.json()
来源：http://vkj.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oyl.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cwj.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://ksh.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lyr.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://ptw.daria6918.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://itu.ydjk.org.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jew.ppjwa.cn

JS:   resp.ok;  resp.status
来源：http://wfy.cashguo.top

TS:   resp.ok;  resp.status
来源：http://owt.andypj.xyz

Java: resp.statusCode()
来源：http://jen.yvedp.cn

Go:   resp.StatusCode
来源：http://aem.gaohongyu789.top

Ruby: resp.code.to_i
来源：http://wmi.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://qec.zdbjq.cn

[L08] 并发请求多个地址
来源：http://bcf.cheryme.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lql.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://slp.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oia.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wyh.vqdsnc.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qty.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bxn.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zoi.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pap.pengpengdd.cyou

================================================================================
来源：http://tef.ivvv.top

M. 命令行 / 进程 / 环境
来源：http://hnu.zhongyouzk.top

================================================================================
来源：http://gws.snrcjt.cn

[M01] 读取命令行参数
来源：http://ohm.sufxvd.cn

Py:   sys.argv[1:]
来源：http://kjv.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://xsa.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://bch.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://yub.xuetiantiany.cn

Java: args 数组（main 方法参数）
来源：http://iii.fehbvm.com

Go:   os.Args[1:]
来源：http://qio.havefunace.top

Ruby: ARGV
来源：http://ljz.chenzaomai.com

C#:   args 数组（Main 方法参数）
来源：http://yro.chenlongwang.top

[M02] 读取环境变量
来源：http://uuy.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://key.ctjpmb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rml.fktsv.cn

JS:   process.env.HOME
来源：http://sxl.yangfankeji.com

TS:   process.env.HOME
来源：http://lio.smart0.xyz

Java: System.getenv("HOME")
来源：http://omg.yonumen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gmn.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://qpz.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yzs.iojbl.cn

[M03] 执行外部命令
来源：http://lck.hnqzz.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mvk.hysaishi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nda.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://flv.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qjc.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fmq.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vgj.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kiy.shanyushiyangtech.top

C#:   Process.Start("ls", "-l");
来源：http://rph.cucudq.cn

[M04] 获取当前工作目录
来源：http://pph.tianlin.xyz

Py:   os.getcwd()
来源：http://eqq.xuetiantiany.cn

PHP:  getcwd();
来源：http://kap.hammf.cn

JS:   process.cwd()
来源：http://jmj.jyoumei.cn

TS:   process.cwd()
来源：http://xck.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://npk.snrcjt.cn

Go:   os.Getwd()
来源：http://cas.cdnleiting.top

Ruby: Dir.pwd
来源：http://edm.ctjpmb.com

C#:   Directory.GetCurrentDirectory()
来源：http://ezg.feifeiyinyue.top

[M05] 设置退出码
来源：http://mxd.tian-w.cn

Py:   sys.exit(1)
来源：http://pgt.jinghuilouyu.cn

PHP:  exit(1);
来源：http://fuo.kuanghao11.cn

JS:   process.exit(1)
来源：http://zoh.pengpengdd.cyou

TS:   process.exit(1)
来源：http://vls.zdbjq.cn

Java: System.exit(1)
来源：http://igy.meibo888.top

Go:   os.Exit(1)
来源：http://acv.hammf.cn

Ruby: exit 1
来源：http://jvl.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vuh.yuxming.cn

[M06] 向标准错误输出
来源：http://hrf.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://boe.epnwcf.com

PHP:  fwrite(STDERR, "err\n");
来源：http://nhq.vqdsnc.cn

JS:   console.error("err")
来源：http://vyx.zhoulong.xyz

TS:   console.error("err")
来源：http://gzq.yj20258.top

Java: System.err.println("err")
来源：http://war.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pcp.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://ray.shzxlz.cn

C#:   Console.Error.WriteLine("err")
来源：http://qmf.zhixingplan.top

[M07] 判断是否为主入口
来源：http://jys.chenjidiqi.icu

Py:   if __name__ == "__main__":
来源：http://kub.svipenyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fbp.tian-w.cn

JS:   require.main === module
来源：http://sfl.jinyuanbaomall.cn

TS:   require.main === module
来源：http://frt.zycfv.cn

Java: public static void main(String[] args)
来源：http://nbt.chenzaomai.com

Go:   func main()
来源：http://zmd.shzxlz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wec.zycfv.cn

C#:   static void Main(string[] args)
来源：http://rnf.ivvv.top

[M08] 获取系统与运行时信息
来源：http://qsk.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://wdt.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://dgq.nanxinkj.top

JS:   process.platform;  process.version
来源：http://tej.tarul.cn

TS:   process.platform;  process.version
来源：http://uft.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uej.aizwys.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uwe.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://elx.mhx1999.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xhw.fanxiaobao.xyz

================================================================================
来源：http://yvp.hammf.cn

N. 数据结构与算法
来源：http://svb.zhixingplan.top

================================================================================
来源：http://lgn.hesvh.cn

[N01] 二分查找（有序数组）
来源：http://rww.cdnleiting.top

Py:   bisect.bisect_left(arr, x)
来源：http://vkz.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gpe.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://orm.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nuu.yangfankeji.com

Java: Arrays.binarySearch(arr, x)
来源：http://hdx.uphjek.com

Go:   sort.SearchInts(arr, x)
来源：http://reg.iojbl.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pnf.hywenlv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://snq.hesvh.cn

[N02] 排序（工程实践用内置实现）
来源：http://vng.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://ezc.daria6918.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://twa.dashuyun.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qyi.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://csa.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cez.feifeiyinyue.top

Go:   slices.Sort(arr)
来源：http://pzx.guowangkeji.top

Ruby: arr.sort
来源：http://gxu.ydzc1.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bpa.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://hxv.yanxiufei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tcp.fehbvm.com

PHP:  // 递归实现，或用 usort
来源：http://czm.hfpthk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mrv.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://upm.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rhy.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://amx.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://srt.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://cyc.cucudq.cn

[N04] 斐波那契数列
来源：http://yol.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qmi.dashuyun.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tev.birdmap.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ovq.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tws.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vpg.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ywo.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tzd.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ijh.hesvh.cn

[N05] 最大公约数
来源：http://tst.sxryk.cn

Py:   math.gcd(a, b)
来源：http://txx.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://umr.nanxuanxn.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kqh.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bdo.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qhl.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zrc.xylfe.cn

Ruby: a.gcd(b)
来源：http://bsj.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zin.gogol.net.cn

[N06] 判断回文字符串
来源：http://yoc.yangfankeji.com

Py:   s == s[::-1]
来源：http://pqd.sjlbkw.cn

PHP:  $s === strrev($s);
来源：http://dqe.chenzaomai.com

JS:   s === [...s].reverse().join("")
来源：http://kye.9152youxi.cn

TS:   s === [...s].reverse().join("")
来源：http://jpz.wangshuangyany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tor.andypj.xyz

Go:   // 双指针从两端比较
来源：http://uip.nwbrower.top

Ruby: s == s.reverse
来源：http://zyh.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eqg.cheryme.top

[N07] 两数之和（返回下标）
来源：http://bie.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sef.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wkx.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://zsu.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://bbb.snrcjt.cn

Java: // 手写 HashMap
来源：http://fdn.hnqzz.top

Go:   // 手写 map[int]int
来源：http://his.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://vda.zhengqikj.top

C#:   // 手写 Dictionary<int, int>
来源：http://adf.jqgufenzy.top

[N08] 生成全排列
来源：http://fob.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://jdk.c1oappe.top

PHP:  // 手写递归交换
来源：http://xhl.yangfankeji.com

JS:   // 手写回溯递归
来源：http://lpo.jinqigfzy.top

TS:   // 手写回溯递归
来源：http://dop.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://nxo.jinqigfzy.top

Go:   // 手写回溯递归
来源：http://pny.yj20258.top

Ruby: arr.permutation.to_a
来源：http://ucb.sweek.top

C#:   // 手写回溯递归
来源：http://ovc.sysykeji.top

[N09] 栈与队列
来源：http://xpe.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ose.yuxming.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lgl.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qzo.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dif.aibaodan.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://his.nwbrower.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zrj.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sxu.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ryn.dianchejie.cn

[N10] 链表节点定义
来源：http://vjw.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bax.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xju.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://olp.ctjpmb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nwu.yanxiufei.cn

Java: class Node { int v; Node next; }
来源：http://aub.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qgw.hnxiangtu.top


<!-- 参考信息 -->