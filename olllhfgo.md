代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://unx.52xcode.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tgg.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://mpy.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://wit.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://zka.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oiw.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sha.yj20258.top

Java: LocalDate.now().plusDays(7)
来源：http://cno.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jff.52xcode.cn

Ruby: Time.now + 7 * 86400
来源：http://ilb.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://cow.smart0.xyz

[J06] 计算两时间之差
来源：http://psm.gzhubu.top

Py:   (end - start).total_seconds()
来源：http://gcs.zdqjudy.top

PHP:  $end->diff($start)->days;
来源：http://rgc.xinyue.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yqc.fktsv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://osi.shuidangran.top

Java: Duration.between(start, end).toSeconds()
来源：http://pjj.chenlongwang.top

Go:   end.Sub(start).Hours()
来源：http://aii.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://gmr.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://pfi.hesvh.cn

[J07] 比较两个日期
来源：http://snc.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://vuh.sysykeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fvq.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://yxq.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://ets.ywan-chungtsiang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hop.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vvv.smart0.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://ksc.yangfankeji.com

C#:   d1 < d2;  d1 == d2
来源：http://evn.xziqi.cn

[J08] 提取年月日与星期
来源：http://eyk.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://auc.hesvh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jxw.aibaodan.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ulo.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hly.jyoumei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nrq.nanxinkj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aow.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://syr.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jem.tanke756.top

[J09] 时区处理
来源：http://ywo.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bzx.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pya.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lnp.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uaw.ydzc1.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qrv.fktsv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ogs.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://cak.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xpn.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://lcy.wangdashe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tru.ppjwa.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ycj.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eui.tian-w.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://puc.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cdk.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oci.andypj.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gnx.iojbl.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://crw.xinyue.icu

================================================================================
来源：http://fai.wangshuangyany.cn

K. JSON 与序列化
来源：http://wdu.cdnleiting.top

================================================================================
来源：http://ppi.gotoacloud.top

[K01] 对象转 JSON 字符串
来源：http://swu.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zqj.jinqigfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jme.sjlbkw.cn

JS:   JSON.stringify(obj)
来源：http://mbp.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://bgm.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ouy.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://gki.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://iiy.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bnq.chenjidiqi.icu

[K02] JSON 字符串转对象
来源：http://bop.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://qpt.mhx1999.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gfj.guowangkeji.top

JS:   JSON.parse(s)
来源：http://opq.wangdashe.top

TS:   JSON.parse(s)
来源：http://tfl.zycfv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gwr.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://hiz.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://mlg.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jam.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://zyh.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yod.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zfy.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gqs.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mdm.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vai.dianchejie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ffl.ehwqpu.com

Ruby: JSON.pretty_generate(obj)
来源：http://uuo.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rws.jianghu66.top

[K04] 读取 JSON 文件
来源：http://hhc.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nzi.yvedp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://emo.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://awa.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aep.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nxj.hammf.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tcl.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rff.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://foh.aizwys.cn

[K05] 深拷贝对象
来源：http://rgd.zdbjq.cn

Py:   copy.deepcopy(obj)
来源：http://ulw.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://rij.xylfe.cn

JS:   structuredClone(obj)
来源：http://sej.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://vbk.xziqi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vmt.shzxlz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nvh.jinghuilouyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://enr.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qed.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://abk.cucudq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bfu.0kj1m.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mdn.tian-w.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ley.shanyushiyangtech.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mvl.guowangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oyo.xuanzx.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://gub.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tap.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jar.pycfn.com

[K07] 进制转换
来源：http://qwh.xuanzx.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mwd.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rtb.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lma.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zvr.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://trx.uphjek.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yzr.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ntb.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aeh.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://lcg.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://mwh.yongpay.top

PHP:  serialize($obj);  unserialize($s);
来源：http://asp.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://zud.xylfe.cn

TS:   v8.serialize(obj)        // Node
来源：http://jou.fengsongda.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://amj.hammf.cn

Go:   encoding/gob
来源：http://qph.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://ckk.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ezr.pengpengdd.cyou

================================================================================
来源：http://fef.gaohongyu789.top

L. 网络请求
来源：http://iau.bbcook.cn

================================================================================
来源：http://fnj.gzhubu.top

[L01] 发送 GET 请求
来源：http://yzr.shzxlz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pdg.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vbu.jyoumei.cn

JS:   await fetch(url)
来源：http://jqa.gogol.net.cn

TS:   await fetch(url)
来源：http://gno.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vah.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://ont.jinyuanbaomall.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tqf.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qjf.aibaodan.cn

[L02] 发送 POST JSON
来源：http://nng.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://zpu.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kkj.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xeq.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cip.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pfc.nanxinkj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vuo.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jik.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://isi.vehdjk.com

[L03] 设置自定义请求头
来源：http://wzx.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vdm.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ues.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rka.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://put.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sjp.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zxa.shanyushiyangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qly.yongpay.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xuk.haohaochexian.top

[L04] 设置超时
来源：http://qad.hysaishi.cn

Py:   requests.get(url, timeout=5)
来源：http://cck.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jsg.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ylp.gzhubu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://isa.shangyingyoupin.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uwg.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://koj.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qer.chenzaomai.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ezd.svipenyu.cn

[L05] 上传文件（multipart）
来源：http://vqe.fengsongda.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zni.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qbt.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://otz.tian-w.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qcm.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cve.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uwo.aizwys.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bcc.shangyingyoupin.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fdb.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://wcb.chenjidiqi.icu

Py:   resp.json()
来源：http://fox.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://ikw.xylfe.cn

JS:   await resp.json()
来源：http://cux.sjlbkw.cn

TS:   await resp.json()
来源：http://hwq.uphjek.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://exx.meibo888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ein.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://nqx.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tqk.yongpay.top

[L07] 处理 HTTP 状态码
来源：http://stc.kuanghao11.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ppq.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ihx.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://rvl.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://qav.hnqzz.top

Java: resp.statusCode()
来源：http://ivh.fengsongda.top

Go:   resp.StatusCode
来源：http://nzv.shuidangran.top

Ruby: resp.code.to_i
来源：http://you.yj20258.top

C#:   (int)resp.StatusCode
来源：http://tkc.jlsjyb.cn

[L08] 并发请求多个地址
来源：http://yts.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rwl.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://ffz.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dxf.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rgy.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zyn.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wkq.fzhhl.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bqm.bjfxy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fgm.cdnleiting.top

================================================================================
来源：http://dei.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境
来源：http://xaf.wangdashe.top

================================================================================
来源：http://iky.hesvh.cn

[M01] 读取命令行参数
来源：http://fqp.snrcjt.cn

Py:   sys.argv[1:]
来源：http://hcz.birdmap.top

PHP:  $argv;  $argc;
来源：http://acn.pycfn.com

JS:   process.argv.slice(2)
来源：http://guo.hesvh.cn

TS:   process.argv.slice(2)
来源：http://cvt.316326.xyz

Java: args 数组（main 方法参数）
来源：http://mmy.jqgufenzy.top

Go:   os.Args[1:]
来源：http://vjr.ehwqpu.com

Ruby: ARGV
来源：http://qxl.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://uah.meibo888.top

[M02] 读取环境变量
来源：http://mjd.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://xvw.xziqi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pyl.daria6918.cn

JS:   process.env.HOME
来源：http://rxp.sysykeji.top

TS:   process.env.HOME
来源：http://dkj.ivvv.top

Java: System.getenv("HOME")
来源：http://uqg.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rjb.yongpay.top

Ruby: ENV["HOME"]
来源：http://yrw.zhijiandao.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://btp.hongshengwenyu.top

[M03] 执行外部命令
来源：http://njk.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vlz.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kgi.zhoulong.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://wav.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dxk.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hyj.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ojf.uphjek.com

Ruby: system("ls -l");  `ls -l`
来源：http://qpl.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://xse.jianghu66.top

[M04] 获取当前工作目录
来源：http://imu.jyoumei.cn

Py:   os.getcwd()
来源：http://yog.yvedp.cn

PHP:  getcwd();
来源：http://hfb.snrcjt.cn

JS:   process.cwd()
来源：http://erz.chenlongwang.top

TS:   process.cwd()
来源：http://gaa.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://zsr.cheryme.top

Go:   os.Getwd()
来源：http://ddb.shanyushiyangtech.top

Ruby: Dir.pwd
来源：http://xlm.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://oje.dashuyun.cn

[M05] 设置退出码
来源：http://row.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://tvf.9152youxi.cn

PHP:  exit(1);
来源：http://dpc.redwolf501.top

JS:   process.exit(1)
来源：http://cjr.epnwcf.com

TS:   process.exit(1)
来源：http://gfo.yuanzhike.top

Java: System.exit(1)
来源：http://khn.316326.xyz

Go:   os.Exit(1)
来源：http://anj.yonumen.top

Ruby: exit 1
来源：http://tin.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bna.haohaochexian.top

[M06] 向标准错误输出
来源：http://rbx.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://qyj.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zea.xziqi.cn

JS:   console.error("err")
来源：http://ept.jianghu66.top

TS:   console.error("err")
来源：http://son.sjlbkw.cn

Java: System.err.println("err")
来源：http://xwq.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://alv.zhengqikj.top

Ruby: warn "err"
来源：http://yxx.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://vod.ehwqpu.com

[M07] 判断是否为主入口
来源：http://qrc.wangdashe.top

Py:   if __name__ == "__main__":
来源：http://ciz.yonumen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hao.kuanghao11.cn

JS:   require.main === module
来源：http://kjf.shuidangran.top

TS:   require.main === module
来源：http://puw.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://vvy.gogol.net.cn

Go:   func main()
来源：http://vhf.yongpay.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fxi.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://inl.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://knj.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://sus.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://ypm.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://izo.hongshengwenyu.top

TS:   process.platform;  process.version
来源：http://azz.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://arl.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yot.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://awc.chenjidiqi.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://rbg.hywenlv.cn

================================================================================
来源：http://fjz.meibo888.top

N. 数据结构与算法
来源：http://jha.52xcode.cn

================================================================================
来源：http://dvc.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://dzb.nanxinkj.top

Py:   bisect.bisect_left(arr, x)
来源：http://bnx.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://foc.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nsu.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cql.yvedp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kms.zhixingplan.top

Go:   sort.SearchInts(arr, x)
来源：http://mdl.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://pvu.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mtr.dashuyun.cn

[N02] 排序（工程实践用内置实现）
来源：http://hsm.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://xbm.zhengqikj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vua.guannengcc.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yja.pycfn.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://zlc.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wac.wangshuangyany.cn

Go:   slices.Sort(arr)
来源：http://lmu.zhoulong.xyz


<!-- 参考信息 -->