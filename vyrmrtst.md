代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://thy.xingfuxueyuan.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sox.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kwe.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nte.fzhhl.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kwv.vqdsnc.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qqp.havefunace.top

[J09] 时区处理
来源：http://aun.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vnp.fzhhl.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xlk.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://akc.nanxuanxn.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ups.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lpg.zdqjudy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vsv.fehbvm.com

Ruby: Time.now.getlocal("+08:00")
来源：http://nvz.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gan.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://ymd.hongshengwenyu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tjz.tian-w.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zmi.guannengcc.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://heh.jinyuanbaomall.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jjn.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mvf.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ahy.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uan.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://buc.svipenyu.cn

================================================================================
来源：http://dsx.snrcjt.cn

K. JSON 与序列化
来源：http://cuy.nanxuanxn.top

================================================================================
来源：http://ujr.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://jfk.jinyuanbaomall.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qzy.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kzm.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://pdy.uphjek.com

TS:   JSON.stringify(obj)
来源：http://dqa.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bnl.sweek.top

Go:   json.Marshal(obj)
来源：http://hzw.vqdsnc.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kcd.jqgfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://irr.havefunace.top

[K02] JSON 字符串转对象
来源：http://cha.smart0.xyz

Py:   json.loads(s)
来源：http://vwm.andypj.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yff.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://jem.nwbrower.top

TS:   JSON.parse(s)
来源：http://iph.gaohongyu789.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mjk.vqdsnc.cn

Go:   json.Unmarshal(data, &v)
来源：http://ubr.haohaochexian.top

Ruby: JSON.parse(s)
来源：http://eks.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://szk.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://thw.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ygi.andypj.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uom.ybcxt.top

JS:   JSON.stringify(obj, null, 2)
来源：http://orw.cucudq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uqr.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mdt.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iox.yonumen.top

Ruby: JSON.pretty_generate(obj)
来源：http://lch.tanke756.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ioo.jqgufenzy.top

[K04] 读取 JSON 文件
来源：http://vvn.meibo888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lxv.ctjpmb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ksj.mhx1999.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hrr.c1oappe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qel.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lpg.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sly.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://kif.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wfm.epnwcf.com

[K05] 深拷贝对象
来源：http://wjj.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://crh.chenlongwang.top

PHP:  unserialize(serialize($obj));
来源：http://fsa.chenzaomai.com

JS:   structuredClone(obj)
来源：http://wgm.fanxiaobao.xyz

TS:   structuredClone(obj)
来源：http://qcs.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qse.snrcjt.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://opk.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://noo.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iun.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://uyk.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pqc.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hxn.redwolf501.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://olw.tian-w.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pmw.ehwqpu.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rgc.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://eqq.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qgs.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vqv.guowangkeji.top

[K07] 进制转换
来源：http://xug.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iyg.tian-w.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iev.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fqj.0kj1m.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zgz.ydzc1.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vvh.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vov.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://evd.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tow.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://drb.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://gal.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://law.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://ryz.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://ufe.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xba.yfazqb.com

Go:   encoding/gob
来源：http://ord.yvedp.cn

Ruby: Marshal.dump(obj)
来源：http://lix.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fzz.jinqigfzy.top

================================================================================
来源：http://axh.daria6918.cn

L. 网络请求
来源：http://soj.yongpay.top

================================================================================
来源：http://kbu.jinyuanbaomall.cn

[L01] 发送 GET 请求
来源：http://sli.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://edj.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://raw.sweek.top

JS:   await fetch(url)
来源：http://lmw.yueranfly.top

TS:   await fetch(url)
来源：http://rzv.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cbi.snrcjt.cn

Go:   resp, err := http.Get(url)
来源：http://mca.xziqi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yac.ivvv.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gum.hnqzz.top

[L02] 发送 POST JSON
来源：http://tsy.yfazqb.com

Py:   requests.post(url, json={"a": 1})
来源：http://pai.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fan.snrcjt.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hbx.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lqf.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blf.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://txv.xylfe.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wnx.fengsongda.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hkr.chenlongwang.top

[L03] 设置自定义请求头
来源：http://hqx.jinghuilouyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lcl.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ead.iojbl.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dsi.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pvw.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nnl.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ukv.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://afn.chenzaomai.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hxh.shuidangran.top

[L04] 设置超时
来源：http://rcv.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://zct.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gki.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://juv.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ner.shangyingyoupin.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hsa.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://roi.shzxlz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://noj.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ppl.fengsongda.top

[L05] 上传文件（multipart）
来源：http://cze.ivvv.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dkp.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gro.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rjo.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ngk.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lkn.svipenyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ojv.havefunace.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rkp.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lqu.jinghuilouyu.cn

[L06] 解析响应为 JSON
来源：http://bqd.chenlongwang.top

Py:   resp.json()
来源：http://opd.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://msi.chenzaomai.com

JS:   await resp.json()
来源：http://axd.haohaochexian.top

TS:   await resp.json()
来源：http://jdf.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dsy.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sgh.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://lip.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pwu.xylfe.cn

[L07] 处理 HTTP 状态码
来源：http://xqc.gaohongyu789.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nuu.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ukq.chenlongwang.top

JS:   resp.ok;  resp.status
来源：http://kuu.yj20258.top

TS:   resp.ok;  resp.status
来源：http://yer.jiagoushi.top

Java: resp.statusCode()
来源：http://zqt.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://daa.hammf.cn

Ruby: resp.code.to_i
来源：http://rao.yj20258.top

C#:   (int)resp.StatusCode
来源：http://ajo.haohaochexian.top

[L08] 并发请求多个地址
来源：http://tqm.guowangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ppy.mhx1999.top

PHP:  curl_multi_init() 系列
来源：http://jah.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wlz.sysykeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sqc.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lpy.fzhhl.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dbf.hysaishi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tej.sysykeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dto.jiagoushi.top

================================================================================
来源：http://vxh.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://ehr.wangdashe.top

================================================================================
来源：http://agc.0kj1m.cn

[M01] 读取命令行参数
来源：http://gpx.yonumen.top

Py:   sys.argv[1:]
来源：http://rvl.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://ksz.epnwcf.com

JS:   process.argv.slice(2)
来源：http://ytk.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://xha.hammf.cn

Java: args 数组（main 方法参数）
来源：http://cqc.jinqigfzy.top

Go:   os.Args[1:]
来源：http://nte.ydzc1.top

Ruby: ARGV
来源：http://fdw.hongshengwenyu.top

C#:   args 数组（Main 方法参数）
来源：http://qvg.jinyuanbaomall.cn

[M02] 读取环境变量
来源：http://jvi.birdmap.top

Py:   os.environ.get("HOME")
来源：http://qsh.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mvj.ppjwa.cn

JS:   process.env.HOME
来源：http://syl.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://zln.tanke756.top

Java: System.getenv("HOME")
来源：http://jmj.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://apk.yonumen.top

Ruby: ENV["HOME"]
来源：http://efw.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yqd.ivvv.top

[M03] 执行外部命令
来源：http://yrb.sjlbkw.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ghk.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wqp.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ipe.feifeiyinyue.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qhl.cucudq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pcn.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://sts.andypj.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://kgh.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://ang.ehwqpu.com

[M04] 获取当前工作目录
来源：http://rbx.aibaodan.cn

Py:   os.getcwd()
来源：http://qly.sweek.top

PHP:  getcwd();
来源：http://gck.hysaishi.cn

JS:   process.cwd()
来源：http://jis.shanyushiyangtech.top

TS:   process.cwd()
来源：http://nic.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://ouf.daria6918.cn

Go:   os.Getwd()
来源：http://xup.vehdjk.com

Ruby: Dir.pwd
来源：http://gye.gzhubu.top

C#:   Directory.GetCurrentDirectory()
来源：http://dhf.yonumen.top

[M05] 设置退出码
来源：http://zpg.guowangkeji.top

Py:   sys.exit(1)
来源：http://qch.wangshuangyany.cn

PHP:  exit(1);
来源：http://sgn.ydjk.org.cn

JS:   process.exit(1)
来源：http://sui.hfpthk.cn

TS:   process.exit(1)
来源：http://bkq.jinqigfzy.top

Java: System.exit(1)
来源：http://nmw.sxryk.cn

Go:   os.Exit(1)
来源：http://kcy.shanyushiyangkeji.top

Ruby: exit 1
来源：http://zpv.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mbc.shanyushiyangkeji.top

[M06] 向标准错误输出
来源：http://qpy.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://qbo.cashguo.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ylt.gogol.net.cn

JS:   console.error("err")
来源：http://ypa.nanxinkj.top

TS:   console.error("err")
来源：http://rff.sufxvd.cn

Java: System.err.println("err")
来源：http://uvo.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iuh.hfpthk.cn

Ruby: warn "err"
来源：http://bmr.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://hdg.316326.xyz

[M07] 判断是否为主入口
来源：http://jek.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://qvr.yonumen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vvw.haohaochexian.top

JS:   require.main === module
来源：http://cbq.dianchejie.cn

TS:   require.main === module
来源：http://tov.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://igf.nwbrower.top

Go:   func main()
来源：http://zqw.smart0.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rye.epnwcf.com

C#:   static void Main(string[] args)
来源：http://bho.tarul.cn

[M08] 获取系统与运行时信息
来源：http://xbm.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://yqi.bjfxy.top

PHP:  PHP_OS;  phpversion();
来源：http://pca.gzhubu.top

JS:   process.platform;  process.version
来源：http://igj.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://nsb.jlsjyb.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nqz.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://vjh.xylfe.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pkn.zhengqikj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ozi.ctjpmb.com

================================================================================
来源：http://qyi.yuanzhike.top

N. 数据结构与算法
来源：http://ifa.yuanzhike.top

================================================================================
来源：http://ggv.fktsv.cn

[N01] 二分查找（有序数组）
来源：http://bcp.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://rew.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aix.dianchejie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wvf.andypj.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tho.jqgufenzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://tja.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://fzy.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jao.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mke.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://hci.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://uzl.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dvv.zhoulong.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://iot.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jbk.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ddm.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://xvm.meibo888.top

Ruby: arr.sort
来源：http://fqi.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://uey.zycfv.cn

[N03] 快速排序（分治示例）
来源：http://rkm.pycfn.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gew.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://pcv.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://itf.zdbjq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mau.uphjek.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fhb.9152youxi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dvz.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://caj.tian-w.cn

C#:   // 手写递归，或 Array.Sort
来源：http://voo.c1oappe.top

[N04] 斐波那契数列
来源：http://kki.jinghuilouyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gov.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://quj.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qxp.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ifo.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qtw.hfpthk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qje.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ohh.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ruh.cheryme.top

[N05] 最大公约数
来源：http://ubp.dianchejie.cn

Py:   math.gcd(a, b)
来源：http://wik.fzhhl.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://htb.smart0.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://azz.hongshengwenyu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xpx.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://okk.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qsm.jyoumei.cn

Ruby: a.gcd(b)
来源：http://nch.jqgfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://drn.yongpay.top

[N06] 判断回文字符串
来源：http://pbt.birdmap.top

Py:   s == s[::-1]
来源：http://ztj.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://ztp.yj20258.top


<!-- 参考信息 -->