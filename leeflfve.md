代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eaw.52xcode.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://skt.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hmu.ehwqpu.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://trm.ivvv.top

================================================================================
来源：http://sqg.chenzaomai.com

K. JSON 与序列化
来源：http://ckd.yongpay.top

================================================================================
来源：http://mwk.daxiang520.top

[K01] 对象转 JSON 字符串
来源：http://tal.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tct.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rro.cashguo.top

JS:   JSON.stringify(obj)
来源：http://hxp.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://dib.meibo888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rzm.zhongyouzk.top

Go:   json.Marshal(obj)
来源：http://yme.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://rus.tianlin.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://dye.wangshuangyany.cn

[K02] JSON 字符串转对象
来源：http://mzz.vqdsnc.cn

Py:   json.loads(s)
来源：http://ibd.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vyt.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://khh.bjfxy.top

TS:   JSON.parse(s)
来源：http://hfb.sufxvd.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ojj.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://ikm.zycfv.cn

Ruby: JSON.parse(s)
来源：http://gho.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://guo.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://xyq.ydjk.org.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pgq.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lut.pycfn.com

JS:   JSON.stringify(obj, null, 2)
来源：http://vhv.pycfn.com

TS:   JSON.stringify(obj, null, 2)
来源：http://gvi.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ugj.hcnkem.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ntk.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://hpz.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zht.hcnkem.com

[K04] 读取 JSON 文件
来源：http://lhw.fzhhl.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dde.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iev.hysaishi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bye.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yop.mhx1999.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eqb.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yfr.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rwa.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blb.zhengqikj.top

[K05] 深拷贝对象
来源：http://pjb.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://ooc.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://tlh.zhengqikj.top

JS:   structuredClone(obj)
来源：http://xkg.jianghu66.top

TS:   structuredClone(obj)
来源：http://kdj.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tqt.yj202588.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hqq.52xcode.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://noj.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wqe.andypj.xyz

[K06] 解析 URL 查询串
来源：http://kie.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dsj.svipenyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vpo.jyoumei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iyu.zhijiandao.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cgi.ybcxt.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qmo.jinghuilouyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zss.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xbj.iojbl.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qkk.cqqwz.cn

[K07] 进制转换
来源：http://ohd.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jna.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://job.hcnkem.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kzz.cucudq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ssu.ydzc1.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fmv.tianlin.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mfw.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qdh.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iht.wangdashe.top

[K08] 二进制序列化（非 JSON）
来源：http://ywh.chenjidiqi.icu

Py:   pickle.dumps(obj)
来源：http://cmw.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ixq.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://qof.bbcook.cn

TS:   v8.serialize(obj)        // Node
来源：http://oki.ywan-chungtsiang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://svq.zdbjq.cn

Go:   encoding/gob
来源：http://lbp.yj202588.top

Ruby: Marshal.dump(obj)
来源：http://njo.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aei.xuetiantiany.cn

================================================================================
来源：http://ijn.yj20258888.top

L. 网络请求
来源：http://wqn.jqgufenzy.top

================================================================================
来源：http://ksj.daxiang520.top

[L01] 发送 GET 请求
来源：http://cir.sxryk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wsj.shanyushiyangtech.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://amm.jyoumei.cn

JS:   await fetch(url)
来源：http://wmq.haohaochexian.top

TS:   await fetch(url)
来源：http://cqf.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mbr.ywan-chungtsiang.top

Go:   resp, err := http.Get(url)
来源：http://not.tarul.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://efk.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pba.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://qqu.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tgk.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mkn.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hsn.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mso.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zrz.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qcx.ydzc1.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pes.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mkn.yj20258.top

[L03] 设置自定义请求头
来源：http://lpd.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vxu.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nmp.zhoulong.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://geg.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lze.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://isg.ydzc1.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nee.daxiang520.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qjs.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mnh.guannengcc.top

[L04] 设置超时
来源：http://wlo.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://rvv.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lrb.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nic.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gip.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://znd.meibo888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pbn.jinqigufen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://evy.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yfn.yueranfly.top

[L05] 上传文件（multipart）
来源：http://dri.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mvq.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tkc.cheryme.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://snr.shuidangran.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tvo.tarul.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rvv.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lpt.hammf.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ovx.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ili.yueranfly.top

[L06] 解析响应为 JSON
来源：http://akl.fengsongda.top

Py:   resp.json()
来源：http://axb.cheryme.top

PHP:  json_decode($body, true);
来源：http://etk.tarul.cn

JS:   await resp.json()
来源：http://mxj.zycfv.cn

TS:   await resp.json()
来源：http://swg.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lvb.daria6918.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://drm.pengpengdd.cyou

Ruby: JSON.parse(resp.body)
来源：http://qie.ywan-chungtsiang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fmn.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://ump.gaohongyu789.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jge.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ani.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://wfd.xinyue.icu

TS:   resp.ok;  resp.status
来源：http://vcr.fzhhl.top

Java: resp.statusCode()
来源：http://gvf.52xcode.cn

Go:   resp.StatusCode
来源：http://rsa.svipenyu.cn

Ruby: resp.code.to_i
来源：http://vwg.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://lkz.tianlin.xyz

[L08] 并发请求多个地址
来源：http://fdw.jqgfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tzp.redwolf501.top

PHP:  curl_multi_init() 系列
来源：http://nyh.nwbrower.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qoz.yj20258888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wme.yongpay.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kvi.andypj.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fhy.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wig.cqqwz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qrw.shuidangran.top

================================================================================
来源：http://jdt.tarul.cn

M. 命令行 / 进程 / 环境
来源：http://msi.ydzc1.top

================================================================================
来源：http://ana.gzhubu.top

[M01] 读取命令行参数
来源：http://qpe.hfpthk.cn

Py:   sys.argv[1:]
来源：http://twl.smart0.xyz

PHP:  $argv;  $argc;
来源：http://qhy.fehbvm.com

JS:   process.argv.slice(2)
来源：http://ngh.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://kdn.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://mmk.snrcjt.cn

Go:   os.Args[1:]
来源：http://ztv.birdmap.top

Ruby: ARGV
来源：http://oju.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://wxt.jqgufenzy.top

[M02] 读取环境变量
来源：http://hyy.nanxinkj.top

Py:   os.environ.get("HOME")
来源：http://iyz.epnwcf.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eit.shzxlz.cn

JS:   process.env.HOME
来源：http://jnj.jinghuilouyu.cn

TS:   process.env.HOME
来源：http://tkv.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://rlb.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tqv.tian-w.cn

Ruby: ENV["HOME"]
来源：http://enl.wangshuangyany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rca.guowangkeji.top

[M03] 执行外部命令
来源：http://bkb.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cms.daria6918.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zla.bbcook.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nma.zhixingplan.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fsg.jinqigufen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gtc.fehbvm.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ydc.dianchejie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fcp.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://fis.yj20258888.top

[M04] 获取当前工作目录
来源：http://hno.birdmap.top

Py:   os.getcwd()
来源：http://gjn.cucudq.cn

PHP:  getcwd();
来源：http://lnt.hongshengwenyu.top

JS:   process.cwd()
来源：http://mpl.tanke756.top

TS:   process.cwd()
来源：http://wkg.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://mtr.jlsjyb.cn

Go:   os.Getwd()
来源：http://tpa.snrcjt.cn

Ruby: Dir.pwd
来源：http://fym.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pgn.yuxming.cn

[M05] 设置退出码
来源：http://pyb.svipenyu.cn

Py:   sys.exit(1)
来源：http://kpe.fehbvm.com

PHP:  exit(1);
来源：http://uvk.uphjek.com

JS:   process.exit(1)
来源：http://tjb.andypj.xyz

TS:   process.exit(1)
来源：http://gnz.shangyingyoupin.top

Java: System.exit(1)
来源：http://vet.yj20258.top

Go:   os.Exit(1)
来源：http://oqx.xuanzx.com

Ruby: exit 1
来源：http://cah.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ygi.ivvv.top

[M06] 向标准错误输出
来源：http://elh.bbcook.cn

Py:   print("err", file=sys.stderr)
来源：http://nxp.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zit.fzhhl.top

JS:   console.error("err")
来源：http://tah.tianlin.xyz

TS:   console.error("err")
来源：http://rzo.feifeiyinyue.top

Java: System.err.println("err")
来源：http://arn.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lti.chenlongwang.top

Ruby: warn "err"
来源：http://onm.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://xmq.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://ftj.jqgufenzy.top

Py:   if __name__ == "__main__":
来源：http://zit.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rcr.xziqi.cn

JS:   require.main === module
来源：http://ofx.zhijiandao.cn

TS:   require.main === module
来源：http://wcq.sxryk.cn

Java: public static void main(String[] args)
来源：http://qml.fengsongda.top

Go:   func main()
来源：http://opk.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ysd.hcnkem.com

C#:   static void Main(string[] args)
来源：http://pll.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://eiq.hnqzz.top

Py:   platform.system();  platform.python_version()
来源：http://twq.sweek.top

PHP:  PHP_OS;  phpversion();
来源：http://btm.dashuyun.cn

JS:   process.platform;  process.version
来源：http://gjs.jinyuanbaomall.cn

TS:   process.platform;  process.version
来源：http://dqh.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vwc.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bjl.tian-w.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://djz.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://qtq.52xcode.cn

================================================================================
来源：http://qmw.cheryme.top

N. 数据结构与算法
来源：http://kbx.hesvh.cn

================================================================================
来源：http://hoz.ydjk.org.cn

[N01] 二分查找（有序数组）
来源：http://mzy.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://tae.hongshengwenyu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tzq.gogol.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uma.andypj.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sse.sjlbkw.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wnq.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://gmv.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://pxx.c1oappe.top

C#:   Array.BinarySearch(arr, x)
来源：http://huy.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://thg.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://uqr.ybcxt.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rfg.guowangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://akx.vehdjk.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://tde.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mni.iojbl.cn

Go:   slices.Sort(arr)
来源：http://aja.guowangkeji.top

Ruby: arr.sort
来源：http://okv.nwbrower.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lut.meibo888.top

[N03] 快速排序（分治示例）
来源：http://ats.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ixc.c1oappe.top

PHP:  // 递归实现，或用 usort
来源：http://lvc.feifeiyinyue.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ciw.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ikh.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://utk.shanyushiyangtech.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://exf.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://weq.ydjk.org.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rlp.snrcjt.cn

[N04] 斐波那契数列
来源：http://fsw.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kjh.jqgufenzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pzy.shangyingyoupin.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bti.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zpt.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jjn.hnqzz.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ddf.zdqjudy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ryu.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jjo.yueranfly.top

[N05] 最大公约数
来源：http://snu.cdnleiting.top

Py:   math.gcd(a, b)
来源：http://izm.yanxiufei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tvq.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://osy.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sxg.jiagoushi.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tae.smart0.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bbq.fktsv.cn

Ruby: a.gcd(b)
来源：http://alx.daxiang520.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fee.zhixingplan.top

[N06] 判断回文字符串
来源：http://nod.sjlbkw.cn

Py:   s == s[::-1]
来源：http://gpj.xylfe.cn

PHP:  $s === strrev($s);
来源：http://mte.ybcxt.top

JS:   s === [...s].reverse().join("")
来源：http://epf.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://rmt.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lyz.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://riy.xuetiantiany.cn

Ruby: s == s.reverse
来源：http://kve.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://zik.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://hou.hongshengwenyu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oir.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ypi.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uem.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://oxy.9152youxi.cn

Java: // 手写 HashMap
来源：http://bbw.xuetiantiany.cn

Go:   // 手写 map[int]int
来源：http://ugy.9152youxi.cn

Ruby: // 手写 Hash
来源：http://dgg.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ief.kuanghao11.cn

[N08] 生成全排列
来源：http://aie.daxiang520.top

Py:   itertools.permutations(arr)
来源：http://oyh.zhengqikj.top

PHP:  // 手写递归交换
来源：http://qvs.yueranfly.top

JS:   // 手写回溯递归
来源：http://qcv.jinqigufen.top

TS:   // 手写回溯递归
来源：http://bun.shanyushiyangkeji.top


<!-- 参考信息 -->