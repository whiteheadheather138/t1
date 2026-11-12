代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iri.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ahg.jyoumei.cn

[J09] 时区处理
来源：http://qjm.daria6918.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://waa.guowangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jyr.zhijiandao.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ujn.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dmb.bjfxy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ebm.ivvv.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xew.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ihu.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fve.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://isw.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fhp.cashguo.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://urw.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zhu.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xxa.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://adi.ybcxt.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jak.zdbjq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cyq.zhiwuduotai.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pym.hnqzz.top

================================================================================
来源：http://yhm.xziqi.cn

K. JSON 与序列化
来源：http://ybh.ivvv.top

================================================================================
来源：http://gez.xziqi.cn

[K01] 对象转 JSON 字符串
来源：http://zfc.cheryme.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pah.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uco.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://twa.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://atq.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://loa.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://sys.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://yqe.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://vvs.gzhubu.top

[K02] JSON 字符串转对象
来源：http://paj.jinqigufen.top

Py:   json.loads(s)
来源：http://yaw.fktsv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cxi.316326.xyz

JS:   JSON.parse(s)
来源：http://qdn.yvedp.cn

TS:   JSON.parse(s)
来源：http://eok.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dab.kuanghao11.cn

Go:   json.Unmarshal(data, &v)
来源：http://rxz.xuetiantiany.cn

Ruby: JSON.parse(s)
来源：http://pmd.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://orp.jinqigfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://dcm.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zse.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://epl.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wsc.andypj.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://lgi.zhaomingkeji.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dvi.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dwv.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://ywb.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vxi.sufxvd.cn

[K04] 读取 JSON 文件
来源：http://hyv.xingfuxueyuan.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yfd.guannengcc.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jon.shzxlz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aye.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pgu.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nud.hcnkem.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nmi.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://crp.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yxw.vehdjk.com

[K05] 深拷贝对象
来源：http://sjn.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://qis.gogol.net.cn

PHP:  unserialize(serialize($obj));
来源：http://zin.dianchejie.cn

JS:   structuredClone(obj)
来源：http://fxr.nanxinkj.top

TS:   structuredClone(obj)
来源：http://zzr.ydzc1.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cic.yvedp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rox.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cbj.cashguo.top

C#:   // 序列化往返，或自定义 Clone
来源：http://amd.dianchejie.cn

[K06] 解析 URL 查询串
来源：http://xvk.hysaishi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://niq.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xjp.dianchejie.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uuf.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kit.jlsjyb.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://atj.vehdjk.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://nnp.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ojk.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rxm.haohaochexian.top

[K07] 进制转换
来源：http://tff.cheryme.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tip.c1oappe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://otf.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gha.zhiwuduotai.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eos.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cld.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qfe.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nbc.bbcook.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mmh.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://bwz.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://egu.xinyue.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://lnd.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://nhe.vehdjk.com

TS:   v8.serialize(obj)        // Node
来源：http://tni.feifeiyinyue.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hao.quarkkingdee.top

Go:   encoding/gob
来源：http://myl.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://vuc.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bgm.ppjwa.cn

================================================================================
来源：http://pav.hongshengwenyu.top

L. 网络请求
来源：http://hro.sxryk.cn

================================================================================
来源：http://haa.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://wem.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bmb.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://con.dashuyun.cn

JS:   await fetch(url)
来源：http://rsx.tanke756.top

TS:   await fetch(url)
来源：http://bxh.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://osk.nwbrower.top

Go:   resp, err := http.Get(url)
来源：http://ufn.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://udb.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uix.ppjwa.cn

[L02] 发送 POST JSON
来源：http://hak.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sle.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ujs.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tjl.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aki.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kyk.sxryk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://onz.jinqigfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lzo.feifeiyinyue.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gtp.0kj1m.cn

[L03] 设置自定义请求头
来源：http://kpq.yanxiufei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mvv.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gpp.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lei.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://amj.havefunace.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uyb.zdqjudy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jpe.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lqw.yj20258888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://frj.jinyuanbaomall.cn

[L04] 设置超时
来源：http://brz.vehdjk.com

Py:   requests.get(url, timeout=5)
来源：http://pxe.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fsd.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lfa.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zjw.chenjidiqi.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vjt.gotoacloud.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wdp.fzhhl.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://egr.daria6918.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://can.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://jaq.yfazqb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cch.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pfk.yonumen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rrp.smart0.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vnh.yangfankeji.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vun.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tkp.hammf.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bug.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cps.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://mjn.fktsv.cn

Py:   resp.json()
来源：http://njr.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://him.yueranfly.top

JS:   await resp.json()
来源：http://jyy.0kj1m.cn

TS:   await resp.json()
来源：http://hda.jqgfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://umh.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ooy.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://duw.epnwcf.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tpz.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://nnh.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sqh.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lmx.quarkkingdee.top

JS:   resp.ok;  resp.status
来源：http://svv.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://lsc.vqdsnc.cn

Java: resp.statusCode()
来源：http://scy.gaohongyu789.top

Go:   resp.StatusCode
来源：http://crr.smart0.xyz

Ruby: resp.code.to_i
来源：http://ggk.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://syg.fktsv.cn

[L08] 并发请求多个地址
来源：http://gsd.zhengqikj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bfd.yonumen.top

PHP:  curl_multi_init() 系列
来源：http://lmi.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yum.tian-w.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ssy.iojbl.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sel.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yyl.gzhubu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aqj.zhixingplan.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dbl.sysykeji.top

================================================================================
来源：http://puv.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://frb.birdmap.top

================================================================================
来源：http://oyo.yvedp.cn

[M01] 读取命令行参数
来源：http://xqe.cdnleiting.top

Py:   sys.argv[1:]
来源：http://raf.xinyue.icu

PHP:  $argv;  $argc;
来源：http://omn.quarkkingdee.top

JS:   process.argv.slice(2)
来源：http://giq.xinyue.icu

TS:   process.argv.slice(2)
来源：http://kko.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://gyo.52xcode.cn

Go:   os.Args[1:]
来源：http://orx.hywenlv.cn

Ruby: ARGV
来源：http://qvm.zhoulong.xyz

C#:   args 数组（Main 方法参数）
来源：http://ups.xuanzx.com

[M02] 读取环境变量
来源：http://zxz.hysaishi.cn

Py:   os.environ.get("HOME")
来源：http://dmt.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uqi.wangdashe.top

JS:   process.env.HOME
来源：http://cqv.nanxinkj.top

TS:   process.env.HOME
来源：http://fay.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://zyk.hywenlv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wpb.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://qqh.haohaochexian.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qrf.hnqzz.top

[M03] 执行外部命令
来源：http://lik.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jmr.hnqzz.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://asc.daria6918.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xcu.fzhhl.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cqe.zhaomingkeji.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ojb.yfazqb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ydh.yj20258.top

Ruby: system("ls -l");  `ls -l`
来源：http://ffb.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://klj.yonumen.top

[M04] 获取当前工作目录
来源：http://zlb.daxiang520.top

Py:   os.getcwd()
来源：http://hjl.daxiang520.top

PHP:  getcwd();
来源：http://mcb.zhengqikj.top

JS:   process.cwd()
来源：http://jbd.hcnkem.com

TS:   process.cwd()
来源：http://jpv.yuxming.cn

Java: Path.of("").toAbsolutePath()
来源：http://zww.yuanzhike.top

Go:   os.Getwd()
来源：http://ern.shzxlz.cn

Ruby: Dir.pwd
来源：http://jzb.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ues.cucudq.cn

[M05] 设置退出码
来源：http://mur.nwbrower.top

Py:   sys.exit(1)
来源：http://ibh.pengpengdd.cyou

PHP:  exit(1);
来源：http://sut.xinyue.icu

JS:   process.exit(1)
来源：http://fnv.zhaomingkeji.xyz

TS:   process.exit(1)
来源：http://eth.gzhubu.top

Java: System.exit(1)
来源：http://hpj.hnqzz.top

Go:   os.Exit(1)
来源：http://afa.yuanzhike.top

Ruby: exit 1
来源：http://yxy.9152youxi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ofb.jianghu66.top

[M06] 向标准错误输出
来源：http://soo.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://mgv.zdqjudy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vmn.yuxming.cn

JS:   console.error("err")
来源：http://olb.aizwys.cn

TS:   console.error("err")
来源：http://wja.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://hkg.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sks.fzhhl.top

Ruby: warn "err"
来源：http://djw.cdnleiting.top

C#:   Console.Error.WriteLine("err")
来源：http://hyu.mhx1999.top

[M07] 判断是否为主入口
来源：http://ttj.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://hak.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uaj.zdqjudy.top

JS:   require.main === module
来源：http://jph.0kj1m.cn

TS:   require.main === module
来源：http://aoi.yfazqb.com

Java: public static void main(String[] args)
来源：http://woi.xingfuxueyuan.xyz

Go:   func main()
来源：http://jvd.yanxiufei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oas.c1oappe.top

C#:   static void Main(string[] args)
来源：http://jbd.fktsv.cn

[M08] 获取系统与运行时信息
来源：http://dds.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://noy.xuanzx.com

PHP:  PHP_OS;  phpversion();
来源：http://nia.ivvv.top

JS:   process.platform;  process.version
来源：http://mwv.sufxvd.cn

TS:   process.platform;  process.version
来源：http://ycp.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uwe.andypj.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://jdt.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wga.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://yda.zycfv.cn

================================================================================
来源：http://pnl.sufxvd.cn

N. 数据结构与算法
来源：http://hnv.xziqi.cn

================================================================================
来源：http://ymq.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://ncx.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://noi.wangshuangyany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dnu.bjfxy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pjs.gaohongyu789.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vud.ehwqpu.com

Java: Arrays.binarySearch(arr, x)
来源：http://ics.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://jaw.zycfv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gsv.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://xlx.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://anq.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://hqb.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rct.cqqwz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dgf.yangfankeji.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://jzd.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lnq.yuanzhike.top

Go:   slices.Sort(arr)
来源：http://adj.hfpthk.cn

Ruby: arr.sort
来源：http://jxg.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://aga.yonumen.top

[N03] 快速排序（分治示例）
来源：http://lxo.fktsv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dlr.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://cdx.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dqz.andypj.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hjd.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nqj.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ekn.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wcp.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://bnx.andypj.xyz

[N04] 斐波那契数列
来源：http://laf.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rom.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tto.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xzg.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dzz.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ezl.shanyushiyangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fpx.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vzm.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hrd.ydzc1.top

[N05] 最大公约数
来源：http://tqy.0kj1m.cn

Py:   math.gcd(a, b)
来源：http://lqx.nanxuanxn.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://weg.smart0.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rez.sweek.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qbb.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://riz.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gre.sweek.top

Ruby: a.gcd(b)
来源：http://yhn.fanxiaobao.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xai.epnwcf.com

[N06] 判断回文字符串
来源：http://qrm.yj20258888.top

Py:   s == s[::-1]
来源：http://pvs.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://zdc.kuanghao11.cn

JS:   s === [...s].reverse().join("")
来源：http://szh.shanyushiyangtech.top

TS:   s === [...s].reverse().join("")
来源：http://mbv.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mhk.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://sum.jlsjyb.cn


<!-- 参考信息 -->