代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ncv.xingfuxueyuan.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sxo.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yhl.meibo888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ovg.fzhhl.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uhi.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ycu.gogol.net.cn

[J09] 时区处理
来源：http://uto.ydzc1.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mjr.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eha.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qoi.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qcs.nanxinkj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tft.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jbt.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yav.cheryme.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kpx.zhiwuduotai.top

[J10] 取今天 / 本月第一天
来源：http://pub.yj20258.top

Py:   date.today();  date.today().replace(day=1)
来源：http://imo.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qzb.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wwa.zycfv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lvu.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://shg.sweek.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lzz.andypj.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ilm.sxryk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://egf.9152youxi.cn

================================================================================
来源：http://nvx.andypj.xyz

K. JSON 与序列化
来源：http://yng.yuanzhike.top

================================================================================
来源：http://xvh.yj20258.top

[K01] 对象转 JSON 字符串
来源：http://fgz.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wzg.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nge.hesvh.cn

JS:   JSON.stringify(obj)
来源：http://rcn.kuanghao11.cn

TS:   JSON.stringify(obj)
来源：http://flq.bbcook.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gpy.ivvv.top

Go:   json.Marshal(obj)
来源：http://qkw.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://vcb.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://tgg.fehbvm.com

[K02] JSON 字符串转对象
来源：http://ohm.gogol.net.cn

Py:   json.loads(s)
来源：http://gih.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jeq.xylfe.cn

JS:   JSON.parse(s)
来源：http://nil.yuanzhike.top

TS:   JSON.parse(s)
来源：http://mgl.hnxiangtu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cbq.kuanghao11.cn

Go:   json.Unmarshal(data, &v)
来源：http://rnn.zhaomingkeji.xyz

Ruby: JSON.parse(s)
来源：http://rvg.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tmw.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://fyc.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xud.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yxb.xylfe.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://imo.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cte.gotoacloud.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://izy.zhiwuduotai.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xqb.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://hxs.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://whh.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://kjz.hesvh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pli.yangfankeji.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ydo.uphjek.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kiq.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qgn.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://efl.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xig.vqdsnc.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://usj.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tbw.yvedp.cn

[K05] 深拷贝对象
来源：http://gop.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://fby.zhiwuduotai.top

PHP:  unserialize(serialize($obj));
来源：http://wcy.shzxlz.cn

JS:   structuredClone(obj)
来源：http://gzb.pengpengdd.cyou

TS:   structuredClone(obj)
来源：http://vnz.shanyushiyangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cip.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wix.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nwf.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vft.316326.xyz

[K06] 解析 URL 查询串
来源：http://wyu.wangshuangyany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dld.tian-w.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fuh.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wjj.chenjidiqi.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jez.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cyr.wangshuangyany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bwe.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kls.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ang.sjlbkw.cn

[K07] 进制转换
来源：http://ktw.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pfr.hfpthk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yvm.shuidangran.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jon.bbcook.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zkl.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xuc.316326.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://myd.hfpthk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xyz.zdbjq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://glf.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://ijl.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://zgb.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://gld.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://jwy.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://ohx.uphjek.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dzs.xinyue.icu

Go:   encoding/gob
来源：http://hsp.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://obs.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vcv.fanxiaobao.xyz

================================================================================
来源：http://doc.fanxiaobao.xyz

L. 网络请求
来源：http://kcv.hesvh.cn

================================================================================
来源：http://snt.9152youxi.cn

[L01] 发送 GET 请求
来源：http://aqv.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://grx.cqqwz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gjm.9152youxi.cn

JS:   await fetch(url)
来源：http://sbj.sufxvd.cn

TS:   await fetch(url)
来源：http://hgt.9152youxi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dxz.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://jyg.fengsongda.top

Ruby: Net::HTTP.get(URI(url))
来源：http://txx.yanxiufei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kim.xingfuxueyuan.xyz

[L02] 发送 POST JSON
来源：http://rfr.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://but.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gzr.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lod.yfazqb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ymd.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bhu.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ols.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rqn.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://amg.dianchejie.cn

[L03] 设置自定义请求头
来源：http://ilz.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ogl.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://szz.chenlongwang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tcb.pengpengdd.cyou

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xte.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zjg.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gpn.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uxu.yvedp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://clq.dashuyun.cn

[L04] 设置超时
来源：http://pth.yanxiufei.cn

Py:   requests.get(url, timeout=5)
来源：http://hcm.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qst.zdbjq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bmf.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mkp.gaohongyu789.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kyg.hammf.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wie.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lty.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tfa.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://rln.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yqx.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jqc.jinqigfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ery.jqgufenzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ljg.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lfp.fanxiaobao.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nop.nanxuanxn.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://btv.yvedp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tmw.gogol.net.cn

[L06] 解析响应为 JSON
来源：http://qus.yueranfly.top

Py:   resp.json()
来源：http://gcn.yonumen.top

PHP:  json_decode($body, true);
来源：http://yom.cucudq.cn

JS:   await resp.json()
来源：http://vox.sysykeji.top

TS:   await resp.json()
来源：http://eaw.nanxuanxn.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hlv.yangfankeji.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://spw.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://lwm.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zfd.birdmap.top

[L07] 处理 HTTP 状态码
来源：http://lgj.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pda.hammf.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ixv.tarul.cn

JS:   resp.ok;  resp.status
来源：http://hjj.cdnleiting.top

TS:   resp.ok;  resp.status
来源：http://ept.shangyingyoupin.top

Java: resp.statusCode()
来源：http://hvx.dianchejie.cn

Go:   resp.StatusCode
来源：http://mzl.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://raq.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://jju.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://ral.shanyushiyangtech.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cfy.yuxming.cn

PHP:  curl_multi_init() 系列
来源：http://mqc.hesvh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bip.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pfd.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qxq.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xbt.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pqb.zdbjq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qmi.chenjidiqi.icu

================================================================================
来源：http://bvq.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://hhr.uphjek.com

================================================================================
来源：http://ujz.yuanzhike.top

[M01] 读取命令行参数
来源：http://kgi.yuxming.cn

Py:   sys.argv[1:]
来源：http://xos.hnqzz.top

PHP:  $argv;  $argc;
来源：http://zft.meibo888.top

JS:   process.argv.slice(2)
来源：http://dtm.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://fha.guannengcc.top

Java: args 数组（main 方法参数）
来源：http://jnd.yanxiufei.cn

Go:   os.Args[1:]
来源：http://tck.fanxiaobao.xyz

Ruby: ARGV
来源：http://thk.ctjpmb.com

C#:   args 数组（Main 方法参数）
来源：http://cvp.uphjek.com

[M02] 读取环境变量
来源：http://esj.chenjidiqi.icu

Py:   os.environ.get("HOME")
来源：http://phj.9152youxi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mnc.ivvv.top

JS:   process.env.HOME
来源：http://csb.fengsongda.top

TS:   process.env.HOME
来源：http://jet.zhoulong.xyz

Java: System.getenv("HOME")
来源：http://dgi.jqgfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qyv.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://cpx.zhengqikj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qkx.sweek.top

[M03] 执行外部命令
来源：http://fov.epnwcf.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://juh.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yko.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://pau.mhx1999.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hrf.xuetiantiany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bek.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wtl.gaohongyu789.top

Ruby: system("ls -l");  `ls -l`
来源：http://qxl.ppjwa.cn

C#:   Process.Start("ls", "-l");
来源：http://itt.hesvh.cn

[M04] 获取当前工作目录
来源：http://evi.yonumen.top

Py:   os.getcwd()
来源：http://cpu.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://ips.nanxuanxn.top

JS:   process.cwd()
来源：http://pxp.guannengcc.top

TS:   process.cwd()
来源：http://sot.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://mlc.jinghuilouyu.cn

Go:   os.Getwd()
来源：http://uuj.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://lzj.jinqigufen.top

C#:   Directory.GetCurrentDirectory()
来源：http://rxm.sysykeji.top

[M05] 设置退出码
来源：http://snc.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://stj.uphjek.com

PHP:  exit(1);
来源：http://rfi.zhengqikj.top

JS:   process.exit(1)
来源：http://spd.fengsongda.top

TS:   process.exit(1)
来源：http://rgv.zdbjq.cn

Java: System.exit(1)
来源：http://rjo.cucudq.cn

Go:   os.Exit(1)
来源：http://mpu.cqqwz.cn

Ruby: exit 1
来源：http://gbn.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://grx.pengpengdd.cyou

[M06] 向标准错误输出
来源：http://ius.sufxvd.cn

Py:   print("err", file=sys.stderr)
来源：http://hrq.c1oappe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ysj.sufxvd.cn

JS:   console.error("err")
来源：http://qyw.snrcjt.cn

TS:   console.error("err")
来源：http://tsm.cheryme.top

Java: System.err.println("err")
来源：http://gay.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hdu.jlsjyb.cn

Ruby: warn "err"
来源：http://gpo.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://tai.daxiang520.top

[M07] 判断是否为主入口
来源：http://wzu.snrcjt.cn

Py:   if __name__ == "__main__":
来源：http://njk.zhiwuduotai.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kdn.gaohongyu789.top

JS:   require.main === module
来源：http://znl.gaohongyu789.top

TS:   require.main === module
来源：http://tog.sxryk.cn

Java: public static void main(String[] args)
来源：http://iws.yfazqb.com

Go:   func main()
来源：http://ttk.tian-w.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://itp.meibo888.top

C#:   static void Main(string[] args)
来源：http://til.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://joj.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://tqr.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://ynn.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://cxb.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://flm.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wzm.shzxlz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uux.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kqy.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://phs.hnxiangtu.top

================================================================================
来源：http://und.gzhubu.top

N. 数据结构与算法
来源：http://uql.smart0.xyz

================================================================================
来源：http://yyx.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://rol.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://caz.feifeiyinyue.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ayi.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dmn.jinyuanbaomall.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cpt.smart0.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://xlr.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://naq.yj202588.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dwe.zhongyouzk.top

C#:   Array.BinarySearch(arr, x)
来源：http://hpe.dashuyun.cn

[N02] 排序（工程实践用内置实现）
来源：http://tme.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ocx.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ldb.zhoulong.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://kzh.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://tje.svipenyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://isw.xziqi.cn

Go:   slices.Sort(arr)
来源：http://czu.yuanzhike.top

Ruby: arr.sort
来源：http://vls.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://oya.daria6918.cn

[N03] 快速排序（分治示例）
来源：http://fdf.sxryk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dup.daria6918.cn

PHP:  // 递归实现，或用 usort
来源：http://mpx.hammf.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rjl.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ngh.tanke756.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aea.chenzaomai.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lwc.jiagoushi.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wni.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://jje.yonumen.top

[N04] 斐波那契数列
来源：http://ajg.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://upc.svipenyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kkq.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://znu.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lmv.ydjk.org.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oqa.shanyushiyangtech.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mfp.nanxinkj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hxa.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xzv.zhongyouzk.top

[N05] 最大公约数
来源：http://nnl.sweek.top

Py:   math.gcd(a, b)
来源：http://hox.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jbz.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bxb.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ajj.shangyingyoupin.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://orp.smart0.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://emo.ydzc1.top

Ruby: a.gcd(b)
来源：http://gxg.nanxinkj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rtu.jqgufenzy.top

[N06] 判断回文字符串
来源：http://wfj.cdnleiting.top

Py:   s == s[::-1]
来源：http://ftg.xuanzx.com

PHP:  $s === strrev($s);
来源：http://gjv.hesvh.cn


<!-- 参考信息 -->