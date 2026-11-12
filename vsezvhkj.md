代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yrq.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lpb.jiagoushi.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qsr.zhiwuduotai.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://inn.sxryk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dvg.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pct.wangdashe.top

[J09] 时区处理
来源：http://kah.chenzaomai.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zlx.daxiang520.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jvj.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ikj.jqgfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bmo.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://maw.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jnl.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ibm.zhijiandao.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ilq.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://zrj.shanyushiyangtech.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nms.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xhf.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://suh.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wgq.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fkl.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wgn.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cgo.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vfp.aibaodan.cn

================================================================================
来源：http://gsb.jinqigfzy.top

K. JSON 与序列化
来源：http://goj.c1oappe.top

================================================================================
来源：http://wjo.uphjek.com

[K01] 对象转 JSON 字符串
来源：http://fcz.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ekh.fehbvm.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://frc.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://zsc.nanxinkj.top

TS:   JSON.stringify(obj)
来源：http://rfp.yonumen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jab.ydzc1.top

Go:   json.Marshal(obj)
来源：http://chi.quarkkingdee.top

Ruby: obj.to_json                                     // require "json"
来源：http://hnk.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lhg.vehdjk.com

[K02] JSON 字符串转对象
来源：http://wko.hfpthk.cn

Py:   json.loads(s)
来源：http://zcg.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rxw.tianlin.xyz

JS:   JSON.parse(s)
来源：http://loq.svipenyu.cn

TS:   JSON.parse(s)
来源：http://qyp.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://biz.cashguo.top

Go:   json.Unmarshal(data, &v)
来源：http://onw.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://roa.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vpf.sufxvd.cn

[K03] JSON 美化输出（带缩进）
来源：http://yue.vehdjk.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://thm.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lvu.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ukl.vqdsnc.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hat.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hsl.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pyv.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://weg.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ihr.yj20258.top

[K04] 读取 JSON 文件
来源：http://vnh.aizwys.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://irz.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wop.hywenlv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uyu.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mca.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://imp.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sma.ppjwa.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jas.yongpay.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://epz.guannengcc.top

[K05] 深拷贝对象
来源：http://xjl.redwolf501.top

Py:   copy.deepcopy(obj)
来源：http://vio.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://nni.epnwcf.com

JS:   structuredClone(obj)
来源：http://tkf.tian-w.cn

TS:   structuredClone(obj)
来源：http://nes.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mdb.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vnd.zhiwuduotai.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yce.ctjpmb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://vct.svipenyu.cn

[K06] 解析 URL 查询串
来源：http://qbx.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://idh.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hxg.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://buk.zhijiandao.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uxl.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nnm.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://eum.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://twk.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sml.zycfv.cn

[K07] 进制转换
来源：http://ywu.jianghu66.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kdy.yuxming.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rjj.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qzr.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qrb.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mpx.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dbj.hnxiangtu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dfi.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jug.hysaishi.cn

[K08] 二进制序列化（非 JSON）
来源：http://vao.zycfv.cn

Py:   pickle.dumps(obj)
来源：http://wep.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://drr.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://uwz.tanke756.top

TS:   v8.serialize(obj)        // Node
来源：http://ckj.ppjwa.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://quw.shanyushiyangtech.top

Go:   encoding/gob
来源：http://hyg.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://jrt.zhoulong.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mgy.zdqjudy.top

================================================================================
来源：http://bqf.feifeiyinyue.top

L. 网络请求
来源：http://uxr.jinyuanbaomall.cn

================================================================================
来源：http://oci.xziqi.cn

[L01] 发送 GET 请求
来源：http://mqi.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tip.cucudq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eql.ybcxt.top

JS:   await fetch(url)
来源：http://vtw.epnwcf.com

TS:   await fetch(url)
来源：http://gnu.fanxiaobao.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wrt.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://pga.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rjk.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xtq.52xcode.cn

[L02] 发送 POST JSON
来源：http://njz.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fir.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kid.9152youxi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hmi.xylfe.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ovx.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rcr.yanxiufei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ktn.tanke756.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zgr.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vap.feifeiyinyue.top

[L03] 设置自定义请求头
来源：http://ftg.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zgx.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jgm.zdqjudy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zfr.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bmu.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ljh.vqdsnc.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nkg.guowangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://igw.sysykeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kfv.bjfxy.top

[L04] 设置超时
来源：http://pjd.aizwys.cn

Py:   requests.get(url, timeout=5)
来源：http://dfw.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wfh.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ykm.cqqwz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zwl.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jrn.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ham.vqdsnc.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mtn.haohaochexian.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yfh.yj20258.top

[L05] 上传文件（multipart）
来源：http://umt.0kj1m.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iwh.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yck.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ucr.ctjpmb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qdm.tarul.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ytk.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cua.hcnkem.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fpl.fktsv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gdg.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://byb.zycfv.cn

Py:   resp.json()
来源：http://tix.cdnleiting.top

PHP:  json_decode($body, true);
来源：http://zsr.nwbrower.top

JS:   await resp.json()
来源：http://sch.hnqzz.top

TS:   await resp.json()
来源：http://puh.yuxming.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ymj.zycfv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ipw.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://rzt.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://naa.quarkkingdee.top

[L07] 处理 HTTP 状态码
来源：http://zxk.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cwf.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vpy.hfpthk.cn

JS:   resp.ok;  resp.status
来源：http://wzn.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://pwy.gaohongyu789.top

Java: resp.statusCode()
来源：http://bbw.yueranfly.top

Go:   resp.StatusCode
来源：http://ors.chenjidiqi.icu

Ruby: resp.code.to_i
来源：http://jpi.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://kbi.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://sge.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hwl.haohaochexian.top

PHP:  curl_multi_init() 系列
来源：http://voo.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yhb.sxryk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uec.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xjb.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vbx.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xff.jqgufenzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wmj.andypj.xyz

================================================================================
来源：http://ocg.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://wcx.smart0.xyz

================================================================================
来源：http://nqc.jlsjyb.cn

[M01] 读取命令行参数
来源：http://evx.sweek.top

Py:   sys.argv[1:]
来源：http://rkh.yanxiufei.cn

PHP:  $argv;  $argc;
来源：http://dfa.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://xnq.aibaodan.cn

TS:   process.argv.slice(2)
来源：http://nhu.jinqigufen.top

Java: args 数组（main 方法参数）
来源：http://jfw.andypj.xyz

Go:   os.Args[1:]
来源：http://ita.ywan-chungtsiang.top

Ruby: ARGV
来源：http://jhx.fanxiaobao.xyz

C#:   args 数组（Main 方法参数）
来源：http://oud.tanke756.top

[M02] 读取环境变量
来源：http://bsm.epnwcf.com

Py:   os.environ.get("HOME")
来源：http://tbq.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ghx.dashuyun.cn

JS:   process.env.HOME
来源：http://wxb.jinqigufen.top

TS:   process.env.HOME
来源：http://zrz.chenzaomai.com

Java: System.getenv("HOME")
来源：http://qaj.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://itu.xinyue.icu

Ruby: ENV["HOME"]
来源：http://nxt.gotoacloud.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wqq.yongpay.top

[M03] 执行外部命令
来源：http://atx.feifeiyinyue.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vmi.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sys.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://uex.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gob.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://exo.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wes.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://diz.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://ebx.hesvh.cn

[M04] 获取当前工作目录
来源：http://oao.zhijiandao.cn

Py:   os.getcwd()
来源：http://xmi.jyoumei.cn

PHP:  getcwd();
来源：http://bmi.ehwqpu.com

JS:   process.cwd()
来源：http://rwp.tanke756.top

TS:   process.cwd()
来源：http://adp.chenzaomai.com

Java: Path.of("").toAbsolutePath()
来源：http://xry.jlsjyb.cn

Go:   os.Getwd()
来源：http://nrh.uphjek.com

Ruby: Dir.pwd
来源：http://iip.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://kzz.cashguo.top

[M05] 设置退出码
来源：http://egv.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://iia.gaohongyu789.top

PHP:  exit(1);
来源：http://dim.vqdsnc.cn

JS:   process.exit(1)
来源：http://dar.daria6918.cn

TS:   process.exit(1)
来源：http://gxi.zhixingplan.top

Java: System.exit(1)
来源：http://dam.jqgufenzy.top

Go:   os.Exit(1)
来源：http://qch.fehbvm.com

Ruby: exit 1
来源：http://knz.jlsjyb.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mbp.xuanzx.com

[M06] 向标准错误输出
来源：http://ewe.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://kky.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qvf.gzhubu.top

JS:   console.error("err")
来源：http://ned.zycfv.cn

TS:   console.error("err")
来源：http://wjv.sweek.top

Java: System.err.println("err")
来源：http://zwv.guowangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://viz.jinqigufen.top

Ruby: warn "err"
来源：http://agm.hysaishi.cn

C#:   Console.Error.WriteLine("err")
来源：http://zol.daria6918.cn

[M07] 判断是否为主入口
来源：http://wzp.9152youxi.cn

Py:   if __name__ == "__main__":
来源：http://pna.ywan-chungtsiang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wfa.zhoulong.xyz

JS:   require.main === module
来源：http://lwx.daxiang520.top

TS:   require.main === module
来源：http://woz.shangyingyoupin.top

Java: public static void main(String[] args)
来源：http://hyn.wangshuangyany.cn

Go:   func main()
来源：http://tsg.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jff.pycfn.com

C#:   static void Main(string[] args)
来源：http://pml.cucudq.cn

[M08] 获取系统与运行时信息
来源：http://xdw.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://bxv.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ddh.gotoacloud.top

JS:   process.platform;  process.version
来源：http://jdh.52xcode.cn

TS:   process.platform;  process.version
来源：http://lpi.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hsd.hesvh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vdj.jinqigfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xxf.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jlj.iojbl.cn

================================================================================
来源：http://lhv.andypj.xyz

N. 数据结构与算法
来源：http://sou.yvedp.cn

================================================================================
来源：http://jeo.hesvh.cn

[N01] 二分查找（有序数组）
来源：http://vqt.yj202588.top

Py:   bisect.bisect_left(arr, x)
来源：http://lvm.tianlin.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://acm.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dpf.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jkm.hnxiangtu.top

Java: Arrays.binarySearch(arr, x)
来源：http://jpn.tianlin.xyz

Go:   sort.SearchInts(arr, x)
来源：http://xkl.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://yka.zhijiandao.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lgu.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://gom.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://zth.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cpn.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gdh.shuidangran.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qyy.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cck.guowangkeji.top

Go:   slices.Sort(arr)
来源：http://aec.ctjpmb.com

Ruby: arr.sort
来源：http://yxe.hywenlv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://emf.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://qrb.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nlv.hnxiangtu.top

PHP:  // 递归实现，或用 usort
来源：http://eun.nanxuanxn.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qso.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ttl.tianlin.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uko.nanxuanxn.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cxs.nwbrower.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lfy.aibaodan.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tgq.yueranfly.top

[N04] 斐波那契数列
来源：http://dee.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xlh.quarkkingdee.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uih.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wqi.jqgufenzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cwt.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ubi.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pli.gotoacloud.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wtx.hywenlv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lsu.tarul.cn

[N05] 最大公约数
来源：http://dsx.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://udp.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yaw.tanke756.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qro.cqqwz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bhp.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://quw.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kep.zhaomingkeji.xyz

Ruby: a.gcd(b)
来源：http://acg.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fxg.vehdjk.com

[N06] 判断回文字符串
来源：http://xul.daxiang520.top

Py:   s == s[::-1]
来源：http://glu.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://wfj.ydjk.org.cn


<!-- 参考信息 -->