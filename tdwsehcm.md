代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://thq.hysaishi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hqj.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://fal.nanxinkj.top

Py:   now + timedelta(days=7)
来源：http://zsi.fzhhl.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ikr.cheryme.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qae.zhaomingkeji.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wew.cashguo.top

Java: LocalDate.now().plusDays(7)
来源：http://bap.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dmj.yj20258888.top

Ruby: Time.now + 7 * 86400
来源：http://xle.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://ech.xylfe.cn

[J06] 计算两时间之差
来源：http://shi.xziqi.cn

Py:   (end - start).total_seconds()
来源：http://ixn.ehwqpu.com

PHP:  $end->diff($start)->days;
来源：http://qed.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://njc.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vif.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://qer.hywenlv.cn

Go:   end.Sub(start).Hours()
来源：http://dbb.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://tcq.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://zwt.zhijiandao.cn

[J07] 比较两个日期
来源：http://mei.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://oag.mhx1999.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tey.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rsm.jyoumei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gct.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ynw.zhoulong.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mlv.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pax.hesvh.cn

C#:   d1 < d2;  d1 == d2
来源：http://cpz.meibo888.top

[J08] 提取年月日与星期
来源：http://jrz.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yll.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xku.zdqjudy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sfy.fktsv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qlp.yj20258.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mmq.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://weq.nanxuanxn.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uos.yangfankeji.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zfo.yj202588.top

[J09] 时区处理
来源：http://umc.epnwcf.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aei.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ghy.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mic.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qhf.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://krn.meibo888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gxi.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vza.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jmo.yuxming.cn

[J10] 取今天 / 本月第一天
来源：http://swp.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nmq.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wrl.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hrt.wangdashe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zuu.nanxinkj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oev.yuanzhike.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://soy.cheryme.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lcz.cqqwz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qzf.jqgfzy.top

================================================================================
来源：http://uak.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://nul.birdmap.top

================================================================================
来源：http://bsm.tianlin.xyz

[K01] 对象转 JSON 字符串
来源：http://rli.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uuo.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bmv.guannengcc.top

JS:   JSON.stringify(obj)
来源：http://mhu.guowangkeji.top

TS:   JSON.stringify(obj)
来源：http://fyh.fanxiaobao.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jlx.zhixingplan.top

Go:   json.Marshal(obj)
来源：http://fxh.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://gpy.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zdm.smart0.xyz

[K02] JSON 字符串转对象
来源：http://rwt.havefunace.top

Py:   json.loads(s)
来源：http://cxl.zhixingplan.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lml.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://rii.yangfankeji.com

TS:   JSON.parse(s)
来源：http://tmo.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bdk.zycfv.cn

Go:   json.Unmarshal(data, &v)
来源：http://ppq.cucudq.cn

Ruby: JSON.parse(s)
来源：http://eut.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kha.gaohongyu789.top

[K03] JSON 美化输出（带缩进）
来源：http://oic.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fas.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cbi.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yan.jqgfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xsy.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rua.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ydz.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://yyj.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yrv.ydjk.org.cn

[K04] 读取 JSON 文件
来源：http://dow.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fru.yueranfly.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zoy.yj20258.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://coe.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oio.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fcd.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://frv.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ybd.tanke756.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hja.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://kjz.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://efo.cucudq.cn

PHP:  unserialize(serialize($obj));
来源：http://hfy.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://uik.fehbvm.com

TS:   structuredClone(obj)
来源：http://tag.yuxming.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vfy.yangfankeji.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xfo.sjlbkw.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eyd.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://twe.smart0.xyz

[K06] 解析 URL 查询串
来源：http://ehs.jinqigufen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ndw.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fqa.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://suj.pengpengdd.cyou

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://grd.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eyf.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ojl.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vtc.kuanghao11.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uct.cheryme.top

[K07] 进制转换
来源：http://gfk.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iib.zhixingplan.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pjx.zhijiandao.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fft.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kvy.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uns.jlsjyb.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eut.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://grn.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dta.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://jfy.cashguo.top

Py:   pickle.dumps(obj)
来源：http://oip.yongpay.top

PHP:  serialize($obj);  unserialize($s);
来源：http://utr.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://poc.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://hzm.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://erj.quarkkingdee.top

Go:   encoding/gob
来源：http://cdr.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://rve.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gcg.nanxinkj.top

================================================================================
来源：http://ttl.xuetiantiany.cn

L. 网络请求
来源：http://akp.bjfxy.top

================================================================================
来源：http://wto.jlsjyb.cn

[L01] 发送 GET 请求
来源：http://hms.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kne.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yrz.bbcook.cn

JS:   await fetch(url)
来源：http://dso.vqdsnc.cn

TS:   await fetch(url)
来源：http://dwe.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ctl.meibo888.top

Go:   resp, err := http.Get(url)
来源：http://ipg.xziqi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://anr.fanxiaobao.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xui.bjfxy.top

[L02] 发送 POST JSON
来源：http://zor.cqqwz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ygx.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jsm.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jpf.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mxi.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eno.zdqjudy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://usk.gotoacloud.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tkk.jlsjyb.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://umm.kuanghao11.cn

[L03] 设置自定义请求头
来源：http://mqb.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yia.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vex.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zpp.shanyushiyangtech.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tlr.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rjm.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fof.jinyuanbaomall.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://udc.aizwys.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://byw.cqqwz.cn

[L04] 设置超时
来源：http://nfb.kuanghao11.cn

Py:   requests.get(url, timeout=5)
来源：http://qdx.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://evf.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lbx.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ibt.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vro.hammf.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qdd.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hon.xylfe.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ioo.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://wnw.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uyz.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tch.hcnkem.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mtb.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rvh.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://frw.smart0.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baz.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kol.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vgf.zdqjudy.top

[L06] 解析响应为 JSON
来源：http://ife.shzxlz.cn

Py:   resp.json()
来源：http://wrb.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://kcu.wangshuangyany.cn

JS:   await resp.json()
来源：http://ese.mhx1999.top

TS:   await resp.json()
来源：http://mjb.redwolf501.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ocs.sxryk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hne.c1oappe.top

Ruby: JSON.parse(resp.body)
来源：http://jdo.xylfe.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pkq.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://xcj.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oxh.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mzv.jinyuanbaomall.cn

JS:   resp.ok;  resp.status
来源：http://uwp.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://oxz.gaohongyu789.top

Java: resp.statusCode()
来源：http://mjb.vehdjk.com

Go:   resp.StatusCode
来源：http://ggo.hysaishi.cn

Ruby: resp.code.to_i
来源：http://fdc.zhongyouzk.top

C#:   (int)resp.StatusCode
来源：http://kyd.0kj1m.cn

[L08] 并发请求多个地址
来源：http://zet.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dal.hcnkem.com

PHP:  curl_multi_init() 系列
来源：http://qwr.wangdashe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zfx.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hry.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fkd.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://feh.yanxiufei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bad.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://akj.yuanzhike.top

================================================================================
来源：http://ndm.vehdjk.com

M. 命令行 / 进程 / 环境
来源：http://qyn.yuxming.cn

================================================================================
来源：http://btn.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://kek.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://kdj.zycfv.cn

PHP:  $argv;  $argc;
来源：http://uhk.xuetiantiany.cn

JS:   process.argv.slice(2)
来源：http://lhu.ybcxt.top

TS:   process.argv.slice(2)
来源：http://iem.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://zzm.smart0.xyz

Go:   os.Args[1:]
来源：http://wqt.9152youxi.cn

Ruby: ARGV
来源：http://anc.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://nak.yueranfly.top

[M02] 读取环境变量
来源：http://dfg.andypj.xyz

Py:   os.environ.get("HOME")
来源：http://abj.yuanzhike.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uvz.redwolf501.top

JS:   process.env.HOME
来源：http://len.zhixingplan.top

TS:   process.env.HOME
来源：http://ddr.havefunace.top

Java: System.getenv("HOME")
来源：http://kje.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vmt.52xcode.cn

Ruby: ENV["HOME"]
来源：http://jzi.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xek.yuanzhike.top

[M03] 执行外部命令
来源：http://fnh.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://peq.pycfn.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bgg.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jtv.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ivc.fzhhl.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://imn.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://scq.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://gdk.hcnkem.com

C#:   Process.Start("ls", "-l");
来源：http://yxu.fanxiaobao.xyz

[M04] 获取当前工作目录
来源：http://tpl.cashguo.top

Py:   os.getcwd()
来源：http://mnh.yanxiufei.cn

PHP:  getcwd();
来源：http://sde.zhongyouzk.top

JS:   process.cwd()
来源：http://dsj.yvedp.cn

TS:   process.cwd()
来源：http://hmg.hesvh.cn

Java: Path.of("").toAbsolutePath()
来源：http://gcq.chenzaomai.com

Go:   os.Getwd()
来源：http://tnu.zhijiandao.cn

Ruby: Dir.pwd
来源：http://cvd.hywenlv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dxf.smart0.xyz

[M05] 设置退出码
来源：http://kxx.fktsv.cn

Py:   sys.exit(1)
来源：http://bja.jlsjyb.cn

PHP:  exit(1);
来源：http://lux.bjfxy.top

JS:   process.exit(1)
来源：http://jcn.hnqzz.top

TS:   process.exit(1)
来源：http://tqx.andypj.xyz

Java: System.exit(1)
来源：http://wte.xylfe.cn

Go:   os.Exit(1)
来源：http://uzq.yj20258888.top

Ruby: exit 1
来源：http://rtd.yonumen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mug.zdbjq.cn

[M06] 向标准错误输出
来源：http://zue.52xcode.cn

Py:   print("err", file=sys.stderr)
来源：http://ywc.fktsv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ouw.dianchejie.cn

JS:   console.error("err")
来源：http://ppn.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://znp.sysykeji.top

Java: System.err.println("err")
来源：http://wxb.zhijiandao.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xxx.gaohongyu789.top

Ruby: warn "err"
来源：http://fbd.jinghuilouyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://vmh.wangdashe.top

[M07] 判断是否为主入口
来源：http://hzj.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://tfq.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lod.bjfxy.top

JS:   require.main === module
来源：http://bxs.bbcook.cn

TS:   require.main === module
来源：http://saw.316326.xyz

Java: public static void main(String[] args)
来源：http://rdp.hammf.cn

Go:   func main()
来源：http://how.epnwcf.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ckk.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://dzm.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://uxt.xziqi.cn

Py:   platform.system();  platform.python_version()
来源：http://oue.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://gat.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://tsj.hnxiangtu.top

TS:   process.platform;  process.version
来源：http://dir.zhengqikj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ahb.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zsu.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cim.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mza.yuxming.cn

================================================================================
来源：http://wdb.tanke756.top

N. 数据结构与算法
来源：http://ixa.nwbrower.top

================================================================================
来源：http://ybs.316326.xyz

[N01] 二分查找（有序数组）
来源：http://wek.gzhubu.top

Py:   bisect.bisect_left(arr, x)
来源：http://mfs.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sqs.hnqzz.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ung.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sbb.tianlin.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://qeh.jqgufenzy.top

Go:   sort.SearchInts(arr, x)
来源：http://kkf.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tjk.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://pqv.uphjek.com

[N02] 排序（工程实践用内置实现）
来源：http://wcf.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://kjp.yanxiufei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://szk.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xoy.jianghu66.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mmt.nanxinkj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://maq.yonumen.top

Go:   slices.Sort(arr)
来源：http://cku.yongpay.top


<!-- 参考信息 -->