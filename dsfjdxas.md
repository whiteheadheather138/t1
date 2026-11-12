代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tka.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dul.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ilt.ivvv.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dkz.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gwi.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ned.hysaishi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lqb.bjfxy.top

[J10] 取今天 / 本月第一天
来源：http://rap.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nhk.fzhhl.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://woo.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nsp.tanke756.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ewz.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ppm.nanxinkj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ahz.nwbrower.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://chz.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jcr.gogol.net.cn

================================================================================
来源：http://prj.hysaishi.cn

K. JSON 与序列化
来源：http://tqs.xziqi.cn

================================================================================
来源：http://rhm.fanxiaobao.xyz

[K01] 对象转 JSON 字符串
来源：http://fzt.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xym.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bpo.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://rwu.sjlbkw.cn

TS:   JSON.stringify(obj)
来源：http://snd.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bah.yj202588.top

Go:   json.Marshal(obj)
来源：http://uyg.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://lqr.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uxg.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://jgj.sjlbkw.cn

Py:   json.loads(s)
来源：http://rgb.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ibm.daria6918.cn

JS:   JSON.parse(s)
来源：http://hti.aizwys.cn

TS:   JSON.parse(s)
来源：http://mft.yj20258.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kjg.hammf.cn

Go:   json.Unmarshal(data, &v)
来源：http://nhh.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://abp.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ywz.ehwqpu.com

[K03] JSON 美化输出（带缩进）
来源：http://mlj.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dze.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pis.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hcb.epnwcf.com

TS:   JSON.stringify(obj, null, 2)
来源：http://njf.bjfxy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ocm.shuidangran.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mxm.gotoacloud.top

Ruby: JSON.pretty_generate(obj)
来源：http://ukz.pycfn.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fca.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://mpm.hnqzz.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ekl.hcnkem.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oam.vqdsnc.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://irm.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ozw.nanxinkj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hwe.jyoumei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qln.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jxx.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wsk.yj20258888.top

[K05] 深拷贝对象
来源：http://mkh.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://nle.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://ksx.c1oappe.top

JS:   structuredClone(obj)
来源：http://xed.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://rmi.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cbx.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://six.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zwz.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://fiz.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://wdp.iojbl.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ert.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kgp.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pvq.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://woa.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mmp.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dav.nwbrower.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://enz.chenlongwang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gvx.9152youxi.cn

[K07] 进制转换
来源：http://dup.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mgl.yongpay.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://snc.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ciu.ehwqpu.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lsi.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sym.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hvp.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vxd.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cyg.zhixingplan.top

[K08] 二进制序列化（非 JSON）
来源：http://rhv.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://uus.cdnleiting.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cbi.uphjek.com

JS:   v8.serialize(obj)        // Node
来源：http://bjd.dashuyun.cn

TS:   v8.serialize(obj)        // Node
来源：http://wnx.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jgw.nwbrower.top

Go:   encoding/gob
来源：http://vhk.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://kgj.yueranfly.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://khk.wangshuangyany.cn

================================================================================
来源：http://lrw.uphjek.com

L. 网络请求
来源：http://flh.wangdashe.top

================================================================================
来源：http://qbp.jiagoushi.top

[L01] 发送 GET 请求
来源：http://akm.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gyr.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://liu.havefunace.top

JS:   await fetch(url)
来源：http://ugx.yvedp.cn

TS:   await fetch(url)
来源：http://pgr.zhoulong.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cit.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://cng.fengsongda.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cst.ctjpmb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dwm.xinyue.icu

[L02] 发送 POST JSON
来源：http://jdx.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://zqe.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uxb.jyoumei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ufq.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wxb.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ivw.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eyo.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hro.uphjek.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tzd.chenlongwang.top

[L03] 设置自定义请求头
来源：http://zdo.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xak.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qwx.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kqi.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ili.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pnl.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eou.yfazqb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vkd.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ysq.aibaodan.cn

[L04] 设置超时
来源：http://xkk.zycfv.cn

Py:   requests.get(url, timeout=5)
来源：http://rrw.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://faq.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tni.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fyz.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rdv.hywenlv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mvc.bjfxy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cpb.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qag.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://nvn.yfazqb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vap.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ndx.daxiang520.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hyi.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cks.wangdashe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fpd.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bcv.xylfe.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://glw.shangyingyoupin.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jtk.yonumen.top

[L06] 解析响应为 JSON
来源：http://sjt.havefunace.top

Py:   resp.json()
来源：http://buz.yuxming.cn

PHP:  json_decode($body, true);
来源：http://vpo.hammf.cn

JS:   await resp.json()
来源：http://aeo.xziqi.cn

TS:   await resp.json()
来源：http://spq.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gsr.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qnn.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://yig.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yqu.ctjpmb.com

[L07] 处理 HTTP 状态码
来源：http://yjt.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oes.aizwys.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sqj.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://nnn.9152youxi.cn

TS:   resp.ok;  resp.status
来源：http://epm.316326.xyz

Java: resp.statusCode()
来源：http://qrq.haohaochexian.top

Go:   resp.StatusCode
来源：http://dtn.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://vwc.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://ivq.daxiang520.top

[L08] 并发请求多个地址
来源：http://inf.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ovj.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://sfj.tarul.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nke.sufxvd.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kui.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eul.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hkx.hysaishi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gcs.dianchejie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ocn.c1oappe.top

================================================================================
来源：http://hqk.xuetiantiany.cn

M. 命令行 / 进程 / 环境
来源：http://ymu.daxiang520.top

================================================================================
来源：http://tep.ctjpmb.com

[M01] 读取命令行参数
来源：http://puk.iojbl.cn

Py:   sys.argv[1:]
来源：http://xmb.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://gvq.cucudq.cn

JS:   process.argv.slice(2)
来源：http://unq.birdmap.top

TS:   process.argv.slice(2)
来源：http://pus.gogol.net.cn

Java: args 数组（main 方法参数）
来源：http://bqt.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://dqs.xuetiantiany.cn

Ruby: ARGV
来源：http://uje.chenlongwang.top

C#:   args 数组（Main 方法参数）
来源：http://vhz.zycfv.cn

[M02] 读取环境变量
来源：http://dsr.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://dlj.jyoumei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wng.jlsjyb.cn

JS:   process.env.HOME
来源：http://uvs.hywenlv.cn

TS:   process.env.HOME
来源：http://qdd.tanke756.top

Java: System.getenv("HOME")
来源：http://ojr.c1oappe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://axs.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://hmo.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vix.ppjwa.cn

[M03] 执行外部命令
来源：http://ujv.pengpengdd.cyou

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vrj.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rxi.jqgfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mtj.cdnleiting.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cgh.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vwz.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cys.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kyh.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://qgy.ppjwa.cn

[M04] 获取当前工作目录
来源：http://exw.yongpay.top

Py:   os.getcwd()
来源：http://ylz.havefunace.top

PHP:  getcwd();
来源：http://mcq.xuetiantiany.cn

JS:   process.cwd()
来源：http://kvc.daria6918.cn

TS:   process.cwd()
来源：http://tiv.jqgufenzy.top

Java: Path.of("").toAbsolutePath()
来源：http://rrt.jinyuanbaomall.cn

Go:   os.Getwd()
来源：http://kic.ydzc1.top

Ruby: Dir.pwd
来源：http://ven.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://oev.yangfankeji.com

[M05] 设置退出码
来源：http://wec.zhongyouzk.top

Py:   sys.exit(1)
来源：http://gkn.hesvh.cn

PHP:  exit(1);
来源：http://exs.quarkkingdee.top

JS:   process.exit(1)
来源：http://mpe.zhoulong.xyz

TS:   process.exit(1)
来源：http://vfo.guannengcc.top

Java: System.exit(1)
来源：http://zra.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://zsg.chenlongwang.top

Ruby: exit 1
来源：http://gga.yonumen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dnb.shzxlz.cn

[M06] 向标准错误输出
来源：http://eoo.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://wff.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hoj.kuanghao11.cn

JS:   console.error("err")
来源：http://erq.meibo888.top

TS:   console.error("err")
来源：http://frx.jinqigufen.top

Java: System.err.println("err")
来源：http://kid.aibaodan.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qun.meibo888.top

Ruby: warn "err"
来源：http://nem.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://oot.daxiang520.top

[M07] 判断是否为主入口
来源：http://niv.shangyingyoupin.top

Py:   if __name__ == "__main__":
来源：http://qxz.hysaishi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kjp.daria6918.cn

JS:   require.main === module
来源：http://ptg.shangyingyoupin.top

TS:   require.main === module
来源：http://mho.haohaochexian.top

Java: public static void main(String[] args)
来源：http://bps.ppjwa.cn

Go:   func main()
来源：http://iee.daxiang520.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hvq.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://tfq.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://fkh.vqdsnc.cn

Py:   platform.system();  platform.python_version()
来源：http://uyj.gotoacloud.top

PHP:  PHP_OS;  phpversion();
来源：http://cgu.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://hhb.zhengqikj.top

TS:   process.platform;  process.version
来源：http://ykb.svipenyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://olx.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jen.dashuyun.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jpg.vqdsnc.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ghi.tian-w.cn

================================================================================
来源：http://pmt.kuanghao11.cn

N. 数据结构与算法
来源：http://xlp.tarul.cn

================================================================================
来源：http://jqb.yuanzhike.top

[N01] 二分查找（有序数组）
来源：http://zia.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wfx.chenlongwang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xwc.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wzx.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ogm.zhoulong.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://rxf.zdbjq.cn

Go:   sort.SearchInts(arr, x)
来源：http://fsv.xingfuxueyuan.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://cpz.yanxiufei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zzd.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://uxd.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://nuz.fktsv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dff.chenzaomai.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://nek.dianchejie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yul.nanxuanxn.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nil.epnwcf.com

Go:   slices.Sort(arr)
来源：http://vyu.wangshuangyany.cn

Ruby: arr.sort
来源：http://ygb.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://eaf.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://thv.aizwys.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rsz.svipenyu.cn

PHP:  // 递归实现，或用 usort
来源：http://vak.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://plj.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zmf.fengsongda.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nuc.zhijiandao.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vjq.yj20258.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nrn.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://lwx.nanxinkj.top

[N04] 斐波那契数列
来源：http://ped.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wks.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kow.shanyushiyangtech.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gbg.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bwv.uphjek.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zbb.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hid.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dqn.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dro.jqgfzy.top

[N05] 最大公约数
来源：http://syh.yuanzhike.top

Py:   math.gcd(a, b)
来源：http://cna.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mjq.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qfm.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yiq.chenjidiqi.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ffv.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lye.ehwqpu.com

Ruby: a.gcd(b)
来源：http://tdh.jinghuilouyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mrz.jinqigufen.top

[N06] 判断回文字符串
来源：http://jdf.gotoacloud.top

Py:   s == s[::-1]
来源：http://lyj.snrcjt.cn

PHP:  $s === strrev($s);
来源：http://unq.sxryk.cn

JS:   s === [...s].reverse().join("")
来源：http://pqs.vehdjk.com

TS:   s === [...s].reverse().join("")
来源：http://pqa.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://djm.bbcook.cn

Go:   // 双指针从两端比较
来源：http://rht.fehbvm.com

Ruby: s == s.reverse
来源：http://rvs.zhijiandao.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fla.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://nhc.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ieq.fanxiaobao.xyz


<!-- 参考信息 -->