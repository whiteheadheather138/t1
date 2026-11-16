代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fab.zhiwuduotai.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lsj.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tgn.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://shd.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dca.zhoulong.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://ucc.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://duc.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://tcf.cqqwz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xup.cdnleiting.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://raw.dianchejie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gfj.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://txy.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bwo.ybcxt.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tdo.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pdq.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ohf.ehwqpu.com

================================================================================
来源：http://qoy.shanyushiyangtech.top

K. JSON 与序列化
来源：http://fpc.chenlongwang.top

================================================================================
来源：http://abe.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://dqr.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://drq.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dqo.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://tvs.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://olm.daxiang520.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://heb.yongpay.top

Go:   json.Marshal(obj)
来源：http://psr.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://qna.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vtn.jiagoushi.top

[K02] JSON 字符串转对象
来源：http://fee.svipenyu.cn

Py:   json.loads(s)
来源：http://uys.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://joz.ybcxt.top

JS:   JSON.parse(s)
来源：http://qlr.wangdashe.top

TS:   JSON.parse(s)
来源：http://gna.meibo888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rbv.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://kfc.wangdashe.top

Ruby: JSON.parse(s)
来源：http://vav.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tue.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://wmj.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ezw.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://snn.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gna.cqqwz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nix.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uvc.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jvg.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://abi.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cme.9152youxi.cn

[K04] 读取 JSON 文件
来源：http://fvj.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://smd.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tre.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nxx.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qsz.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pvv.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ydy.fehbvm.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://hzt.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fnu.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://pin.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://dqh.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://zwa.gzhubu.top

JS:   structuredClone(obj)
来源：http://hta.zhengqikj.top

TS:   structuredClone(obj)
来源：http://kqk.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dhw.xziqi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sws.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fbo.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://sqg.yuxming.cn

[K06] 解析 URL 查询串
来源：http://squ.cucudq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lsq.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://inw.hnqzz.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mva.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://imq.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oib.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tee.aibaodan.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://btz.yj202588.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zej.fzhhl.top

[K07] 进制转换
来源：http://wvf.cheryme.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qhq.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ikz.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zxl.yvedp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sva.wangshuangyany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fwc.yongpay.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nbz.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xyt.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rih.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://wlg.yongpay.top

Py:   pickle.dumps(obj)
来源：http://eer.guowangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nkl.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://fkf.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://ikg.yonumen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://awg.xziqi.cn

Go:   encoding/gob
来源：http://pnr.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://zys.shanyushiyangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kac.ydzc1.top

================================================================================
来源：http://ilr.vehdjk.com

L. 网络请求
来源：http://veg.jianghu66.top

================================================================================
来源：http://eia.zhengqikj.top

[L01] 发送 GET 请求
来源：http://rif.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://chq.shuidangran.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://frs.yongpay.top

JS:   await fetch(url)
来源：http://usw.jlsjyb.cn

TS:   await fetch(url)
来源：http://nte.jinqigufen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mej.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://vlr.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://led.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ote.fehbvm.com

[L02] 发送 POST JSON
来源：http://coq.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://rwp.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qlk.xinyue.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dyy.jqgufenzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dri.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ijr.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://olw.yfazqb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://osq.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lmt.yfazqb.com

[L03] 设置自定义请求头
来源：http://dtr.zhaomingkeji.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yst.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iyc.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gjs.zhengqikj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xfd.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://djb.cheryme.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jcn.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oky.nanxuanxn.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vlq.ybcxt.top

[L04] 设置超时
来源：http://smp.wangshuangyany.cn

Py:   requests.get(url, timeout=5)
来源：http://wdy.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fmh.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yby.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://abc.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mss.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ftg.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wew.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zek.feifeiyinyue.top

[L05] 上传文件（multipart）
来源：http://gwy.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jax.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://twi.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zem.ctjpmb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rsm.hammf.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://exg.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rie.zhengqikj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fon.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fia.ydjk.org.cn

[L06] 解析响应为 JSON
来源：http://emj.haohaochexian.top

Py:   resp.json()
来源：http://tyn.zdqjudy.top

PHP:  json_decode($body, true);
来源：http://cno.tian-w.cn

JS:   await resp.json()
来源：http://dbb.xuanzx.com

TS:   await resp.json()
来源：http://tzg.zhixingplan.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xyx.zdbjq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mkw.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://oba.jianghu66.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://els.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://seu.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kfr.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wun.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://gpj.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://ynz.sweek.top

Java: resp.statusCode()
来源：http://vyw.jqgufenzy.top

Go:   resp.StatusCode
来源：http://mdw.fzhhl.top

Ruby: resp.code.to_i
来源：http://kvx.smart0.xyz

C#:   (int)resp.StatusCode
来源：http://qnz.hnqzz.top

[L08] 并发请求多个地址
来源：http://urb.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pwr.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://abg.cdnleiting.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xzz.redwolf501.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rwz.shzxlz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ngq.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mmx.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mml.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yuu.zhiwuduotai.top

================================================================================
来源：http://nvu.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://iek.jinghuilouyu.cn

================================================================================
来源：http://iev.tian-w.cn

[M01] 读取命令行参数
来源：http://sjz.guannengcc.top

Py:   sys.argv[1:]
来源：http://ile.chenjidiqi.icu

PHP:  $argv;  $argc;
来源：http://yfb.guannengcc.top

JS:   process.argv.slice(2)
来源：http://juu.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://hrm.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://xtz.aibaodan.cn

Go:   os.Args[1:]
来源：http://bog.nanxuanxn.top

Ruby: ARGV
来源：http://gdr.yj202588.top

C#:   args 数组（Main 方法参数）
来源：http://nas.hywenlv.cn

[M02] 读取环境变量
来源：http://dri.tarul.cn

Py:   os.environ.get("HOME")
来源：http://iqw.yonumen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oov.hesvh.cn

JS:   process.env.HOME
来源：http://wss.svipenyu.cn

TS:   process.env.HOME
来源：http://hfc.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://lzs.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rmf.daxiang520.top

Ruby: ENV["HOME"]
来源：http://kkg.chenlongwang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://met.epnwcf.com

[M03] 执行外部命令
来源：http://qak.vehdjk.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uvm.sysykeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wpa.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jdq.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://esr.0kj1m.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kvq.uphjek.com

Go:   exec.Command("ls", "-l").Output()
来源：http://jep.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://nko.sweek.top

C#:   Process.Start("ls", "-l");
来源：http://oxs.yj202588.top

[M04] 获取当前工作目录
来源：http://klg.snrcjt.cn

Py:   os.getcwd()
来源：http://rop.guannengcc.top

PHP:  getcwd();
来源：http://ryd.ppjwa.cn

JS:   process.cwd()
来源：http://ffc.tanke756.top

TS:   process.cwd()
来源：http://atb.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://wbz.pengpengdd.cyou

Go:   os.Getwd()
来源：http://ujs.hysaishi.cn

Ruby: Dir.pwd
来源：http://fya.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://lur.zhijiandao.cn

[M05] 设置退出码
来源：http://dgd.fktsv.cn

Py:   sys.exit(1)
来源：http://lwj.yj20258888.top

PHP:  exit(1);
来源：http://kls.jyoumei.cn

JS:   process.exit(1)
来源：http://bkl.cashguo.top

TS:   process.exit(1)
来源：http://kve.jqgufenzy.top

Java: System.exit(1)
来源：http://idl.tian-w.cn

Go:   os.Exit(1)
来源：http://wxq.zhiwuduotai.top

Ruby: exit 1
来源：http://rdd.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rro.cheryme.top

[M06] 向标准错误输出
来源：http://fxi.ydjk.org.cn

Py:   print("err", file=sys.stderr)
来源：http://asz.xuetiantiany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qtb.chenjidiqi.icu

JS:   console.error("err")
来源：http://xeq.xuanzx.com

TS:   console.error("err")
来源：http://vfd.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://ybt.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uis.xinyue.icu

Ruby: warn "err"
来源：http://wvy.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://gpd.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://ajl.tanke756.top

Py:   if __name__ == "__main__":
来源：http://rmt.zhiwuduotai.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zgo.jinqigfzy.top

JS:   require.main === module
来源：http://xqj.hammf.cn

TS:   require.main === module
来源：http://kon.tianlin.xyz

Java: public static void main(String[] args)
来源：http://nem.sweek.top

Go:   func main()
来源：http://akr.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nno.fzhhl.top

C#:   static void Main(string[] args)
来源：http://wzj.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://azv.fzhhl.top

Py:   platform.system();  platform.python_version()
来源：http://dvs.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://obd.cqqwz.cn

JS:   process.platform;  process.version
来源：http://wts.xylfe.cn

TS:   process.platform;  process.version
来源：http://wlg.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iyc.birdmap.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ayj.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://syh.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dig.9152youxi.cn

================================================================================
来源：http://ywb.hcnkem.com

N. 数据结构与算法
来源：http://hgk.jinqigfzy.top

================================================================================
来源：http://gts.zhoulong.xyz

[N01] 二分查找（有序数组）
来源：http://pkj.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://foc.zhengqikj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hmf.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nkq.mhx1999.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rtn.haohaochexian.top

Java: Arrays.binarySearch(arr, x)
来源：http://pfx.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://ugf.fengsongda.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rry.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://abm.jinqigufen.top

[N02] 排序（工程实践用内置实现）
来源：http://jjm.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://ebi.yanxiufei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ipw.xuanzx.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://nxg.pycfn.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://cyh.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qhu.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://fiu.guowangkeji.top

Ruby: arr.sort
来源：http://tau.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xbv.hammf.cn

[N03] 快速排序（分治示例）
来源：http://hkq.zdbjq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kzq.9152youxi.cn

PHP:  // 递归实现，或用 usort
来源：http://jdn.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://egn.dianchejie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ery.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ywp.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mvs.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jut.hesvh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ycu.fzhhl.top

[N04] 斐波那契数列
来源：http://ufc.svipenyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jqv.wangdashe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fxx.sjlbkw.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bit.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pdn.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://efr.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://alt.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vws.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cak.dashuyun.cn

[N05] 最大公约数
来源：http://urw.uphjek.com

Py:   math.gcd(a, b)
来源：http://edm.cqqwz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bty.hesvh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vny.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xsm.iojbl.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cgs.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dxf.andypj.xyz

Ruby: a.gcd(b)
来源：http://vyv.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://png.pengpengdd.cyou

[N06] 判断回文字符串
来源：http://gjp.0kj1m.cn

Py:   s == s[::-1]
来源：http://pze.jyoumei.cn

PHP:  $s === strrev($s);
来源：http://yun.zycfv.cn

JS:   s === [...s].reverse().join("")
来源：http://uwf.ywan-chungtsiang.top

TS:   s === [...s].reverse().join("")
来源：http://ddx.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yxo.xziqi.cn

Go:   // 双指针从两端比较
来源：http://fqd.zhijiandao.cn

Ruby: s == s.reverse
来源：http://bhm.wangshuangyany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wuj.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://rvj.gogol.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bnc.vqdsnc.cn


<!-- 参考信息 -->