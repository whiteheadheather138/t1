代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yjz.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hkq.vehdjk.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ree.xylfe.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://guk.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bgw.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jud.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rqp.gogol.net.cn

[J10] 取今天 / 本月第一天
来源：http://hit.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xrm.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://abq.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tdx.guowangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qvk.shanyushiyangtech.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://waa.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ric.cheryme.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vsf.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jln.chenjidiqi.icu

================================================================================
来源：http://mnb.316326.xyz

K. JSON 与序列化
来源：http://gnu.jqgfzy.top

================================================================================
来源：http://kws.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://mmg.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fbn.zhixingplan.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vrj.dashuyun.cn

JS:   JSON.stringify(obj)
来源：http://hkg.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://inz.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://krg.uphjek.com

Go:   json.Marshal(obj)
来源：http://ljo.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://igc.ivvv.top

C#:   JsonSerializer.Serialize(obj)
来源：http://doc.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://rdv.xinyue.icu

Py:   json.loads(s)
来源：http://oez.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mzp.hammf.cn

JS:   JSON.parse(s)
来源：http://apj.hcnkem.com

TS:   JSON.parse(s)
来源：http://gao.sweek.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://htm.gogol.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://mbh.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://xjn.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nhe.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://kfb.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bjr.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wzc.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yft.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qvo.xylfe.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rgi.quarkkingdee.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ref.yj202588.top

Ruby: JSON.pretty_generate(obj)
来源：http://onj.smart0.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dtw.9152youxi.cn

[K04] 读取 JSON 文件
来源：http://zvv.zhiwuduotai.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rrj.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uur.fehbvm.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uqj.shanyushiyangtech.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zsl.wangdashe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bid.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ixm.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jmy.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tda.316326.xyz

[K05] 深拷贝对象
来源：http://wgv.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://ghz.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://hmx.yj20258.top

JS:   structuredClone(obj)
来源：http://cok.fengsongda.top

TS:   structuredClone(obj)
来源：http://jrl.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eft.hammf.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pgb.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sjd.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bxq.xylfe.cn

[K06] 解析 URL 查询串
来源：http://vdm.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rmr.xuetiantiany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oax.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wdt.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qqx.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fem.yvedp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://omg.svipenyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gzp.yj20258.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vtq.zycfv.cn

[K07] 进制转换
来源：http://usg.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yyh.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dwu.yj202588.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wax.chenzaomai.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ccy.nanxinkj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tyg.yj20258888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cdh.yfazqb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mme.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gzo.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://erb.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://oca.dashuyun.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wtt.ivvv.top

JS:   v8.serialize(obj)        // Node
来源：http://ttq.guowangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://chg.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ecf.hnqzz.top

Go:   encoding/gob
来源：http://dck.jinyuanbaomall.cn

Ruby: Marshal.dump(obj)
来源：http://txc.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ccu.zhijiandao.cn

================================================================================
来源：http://jye.fktsv.cn

L. 网络请求
来源：http://uxf.hnxiangtu.top

================================================================================
来源：http://hmw.bjfxy.top

[L01] 发送 GET 请求
来源：http://sat.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vag.sjlbkw.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qzu.sufxvd.cn

JS:   await fetch(url)
来源：http://bqf.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://chj.fehbvm.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ezn.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://bwx.yonumen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qsq.uphjek.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qzd.smart0.xyz

[L02] 发送 POST JSON
来源：http://idd.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://ogh.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iah.52xcode.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zud.yueranfly.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lxp.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wya.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ydk.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mxz.iojbl.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fnx.hammf.cn

[L03] 设置自定义请求头
来源：http://bek.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bvf.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rzo.snrcjt.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fnm.vehdjk.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://etx.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://afa.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dzo.daxiang520.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ixl.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://obi.aizwys.cn

[L04] 设置超时
来源：http://nem.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://wps.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tef.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dvf.nanxuanxn.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mhd.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hxo.zhiwuduotai.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xhl.jinqigufen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mrh.xylfe.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://plx.dianchejie.cn

[L05] 上传文件（multipart）
来源：http://edf.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ulv.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vhy.52xcode.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cop.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gln.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vkw.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xil.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://klf.bjfxy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rrl.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://wof.sweek.top

Py:   resp.json()
来源：http://vjy.yuxming.cn

PHP:  json_decode($body, true);
来源：http://ubu.0kj1m.cn

JS:   await resp.json()
来源：http://hjk.yj202588.top

TS:   await resp.json()
来源：http://eqq.bjfxy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mha.jinyuanbaomall.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bzn.ydjk.org.cn

Ruby: JSON.parse(resp.body)
来源：http://eph.jianghu66.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rmx.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://xqc.shanyushiyangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lix.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://unj.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://nrz.fanxiaobao.xyz

TS:   resp.ok;  resp.status
来源：http://sfg.bjfxy.top

Java: resp.statusCode()
来源：http://pqf.chenlongwang.top

Go:   resp.StatusCode
来源：http://vyg.fehbvm.com

Ruby: resp.code.to_i
来源：http://kxe.hnxiangtu.top

C#:   (int)resp.StatusCode
来源：http://uwg.cqqwz.cn

[L08] 并发请求多个地址
来源：http://vqh.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://foj.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://oei.pycfn.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wns.xingfuxueyuan.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mzr.guannengcc.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://scr.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sbr.jlsjyb.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ahv.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jbx.zhiwuduotai.top

================================================================================
来源：http://uah.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://eov.mhx1999.top

================================================================================
来源：http://jlt.haohaochexian.top

[M01] 读取命令行参数
来源：http://pyz.epnwcf.com

Py:   sys.argv[1:]
来源：http://rsf.meibo888.top

PHP:  $argv;  $argc;
来源：http://fox.tanke756.top

JS:   process.argv.slice(2)
来源：http://cxw.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://ugg.shanyushiyangkeji.top

Java: args 数组（main 方法参数）
来源：http://mwm.ybcxt.top

Go:   os.Args[1:]
来源：http://cui.yj20258888.top

Ruby: ARGV
来源：http://nwg.zhijiandao.cn

C#:   args 数组（Main 方法参数）
来源：http://ykt.wangdashe.top

[M02] 读取环境变量
来源：http://oao.shzxlz.cn

Py:   os.environ.get("HOME")
来源：http://zxw.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rac.zhixingplan.top

JS:   process.env.HOME
来源：http://deb.guowangkeji.top

TS:   process.env.HOME
来源：http://kjq.yfazqb.com

Java: System.getenv("HOME")
来源：http://lpt.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pux.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://ley.shanyushiyangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aaa.9152youxi.cn

[M03] 执行外部命令
来源：http://yfz.vehdjk.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://age.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iep.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gsq.sweek.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pob.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xwk.redwolf501.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ccy.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://wts.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://qso.chenzaomai.com

[M04] 获取当前工作目录
来源：http://yuy.hcnkem.com

Py:   os.getcwd()
来源：http://urq.chenjidiqi.icu

PHP:  getcwd();
来源：http://xou.ppjwa.cn

JS:   process.cwd()
来源：http://uns.hongshengwenyu.top

TS:   process.cwd()
来源：http://vsf.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://arl.wangdashe.top

Go:   os.Getwd()
来源：http://xbd.zhongyouzk.top

Ruby: Dir.pwd
来源：http://ews.jinqigfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://pzr.shzxlz.cn

[M05] 设置退出码
来源：http://kza.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://kkv.quarkkingdee.top

PHP:  exit(1);
来源：http://peu.zhijiandao.cn

JS:   process.exit(1)
来源：http://lcb.zdqjudy.top

TS:   process.exit(1)
来源：http://hmq.yuxming.cn

Java: System.exit(1)
来源：http://uka.yueranfly.top

Go:   os.Exit(1)
来源：http://xye.quarkkingdee.top

Ruby: exit 1
来源：http://wfp.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ovw.smart0.xyz

[M06] 向标准错误输出
来源：http://foq.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://jlm.bbcook.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jxs.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://tdn.jqgfzy.top

TS:   console.error("err")
来源：http://ixm.wangdashe.top

Java: System.err.println("err")
来源：http://rgb.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://anf.hnqzz.top

Ruby: warn "err"
来源：http://smc.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://xtw.cucudq.cn

[M07] 判断是否为主入口
来源：http://wnj.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://zqt.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kdp.yongpay.top

JS:   require.main === module
来源：http://tkq.chenlongwang.top

TS:   require.main === module
来源：http://gek.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://gso.hysaishi.cn

Go:   func main()
来源：http://wop.daxiang520.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://liw.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://bfc.wangdashe.top

[M08] 获取系统与运行时信息
来源：http://neh.shangyingyoupin.top

Py:   platform.system();  platform.python_version()
来源：http://ccm.yj20258.top

PHP:  PHP_OS;  phpversion();
来源：http://iyb.tanke756.top

JS:   process.platform;  process.version
来源：http://gdq.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://sas.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xic.cdnleiting.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kvv.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yyi.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://qlt.hammf.cn

================================================================================
来源：http://dgf.hywenlv.cn

N. 数据结构与算法
来源：http://kze.aibaodan.cn

================================================================================
来源：http://dkx.mhx1999.top

[N01] 二分查找（有序数组）
来源：http://eye.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gxv.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xan.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mua.ehwqpu.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qux.nwbrower.top

Java: Arrays.binarySearch(arr, x)
来源：http://jaz.hongshengwenyu.top

Go:   sort.SearchInts(arr, x)
来源：http://eim.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dhv.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zno.hnqzz.top

[N02] 排序（工程实践用内置实现）
来源：http://pvr.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://srr.zhengqikj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pns.gotoacloud.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jju.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pbn.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hos.zhongyouzk.top

Go:   slices.Sort(arr)
来源：http://dfb.gogol.net.cn

Ruby: arr.sort
来源：http://kko.fanxiaobao.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://azz.fktsv.cn

[N03] 快速排序（分治示例）
来源：http://txt.jianghu66.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kzm.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://lag.nwbrower.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jdr.havefunace.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kjz.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xbn.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://whk.xuetiantiany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bmw.sxryk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nfv.svipenyu.cn

[N04] 斐波那契数列
来源：http://hca.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://odj.shzxlz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sbd.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rgf.jiagoushi.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://acw.haohaochexian.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://olf.nwbrower.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tkn.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://opd.epnwcf.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://avm.birdmap.top

[N05] 最大公约数
来源：http://kgj.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://xzv.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qqz.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wfv.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wdz.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tlr.yueranfly.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ntj.nanxinkj.top

Ruby: a.gcd(b)
来源：http://pvg.jqgfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xvh.iojbl.cn

[N06] 判断回文字符串
来源：http://hxo.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://aib.andypj.xyz

PHP:  $s === strrev($s);
来源：http://vnf.xziqi.cn

JS:   s === [...s].reverse().join("")
来源：http://piw.yonumen.top

TS:   s === [...s].reverse().join("")
来源：http://xwx.bbcook.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zhq.gzhubu.top

Go:   // 双指针从两端比较
来源：http://att.0kj1m.cn

Ruby: s == s.reverse
来源：http://bkr.gaohongyu789.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gso.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://izq.zhixingplan.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zar.ctjpmb.com


<!-- 参考信息 -->