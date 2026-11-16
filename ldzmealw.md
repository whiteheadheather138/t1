代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://reg.meibo888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bth.kuanghao11.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nep.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oyl.fengsongda.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jdz.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://awc.andypj.xyz

[J05] 时间加减（加 7 天）
来源：http://ten.cdnleiting.top

Py:   now + timedelta(days=7)
来源：http://rgx.jyoumei.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lbg.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hap.yangfankeji.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ion.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://sgh.gzhubu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ssb.feifeiyinyue.top

Ruby: Time.now + 7 * 86400
来源：http://ekf.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://rmt.ydjk.org.cn

[J06] 计算两时间之差
来源：http://sdg.zdbjq.cn

Py:   (end - start).total_seconds()
来源：http://jlg.jlsjyb.cn

PHP:  $end->diff($start)->days;
来源：http://oxy.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pcd.jinyuanbaomall.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mrk.c1oappe.top

Java: Duration.between(start, end).toSeconds()
来源：http://hko.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://uvn.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://sld.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://dry.uphjek.com

[J07] 比较两个日期
来源：http://ivz.zhongyouzk.top

Py:   d1 < d2;  d1 == d2
来源：http://ban.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://alu.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://dud.andypj.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://zac.zhoulong.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ipn.hongshengwenyu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cbv.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://lub.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://kyw.svipenyu.cn

[J08] 提取年月日与星期
来源：http://qel.feifeiyinyue.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://afi.tarul.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fcm.quarkkingdee.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://abf.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ojs.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://epg.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jpf.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dra.xuanzx.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pei.ppjwa.cn

[J09] 时区处理
来源：http://kex.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tzq.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://spz.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ykc.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nuj.nwbrower.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zuk.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sbg.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rhb.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://msg.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://pgx.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kgg.fanxiaobao.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vkr.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qlu.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jvv.nanxuanxn.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://okw.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dip.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eug.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dgc.ivvv.top

================================================================================
来源：http://fye.andypj.xyz

K. JSON 与序列化
来源：http://mpe.svipenyu.cn

================================================================================
来源：http://gop.shanyushiyangtech.top

[K01] 对象转 JSON 字符串
来源：http://lda.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wfz.ppjwa.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vcg.pycfn.com

JS:   JSON.stringify(obj)
来源：http://vpu.ybcxt.top

TS:   JSON.stringify(obj)
来源：http://ujl.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sow.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://hto.hongshengwenyu.top

Ruby: obj.to_json                                     // require "json"
来源：http://mjj.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://grs.yj20258.top

[K02] JSON 字符串转对象
来源：http://uka.cdnleiting.top

Py:   json.loads(s)
来源：http://xss.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cda.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://whm.cqqwz.cn

TS:   JSON.parse(s)
来源：http://tyq.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qdu.jiagoushi.top

Go:   json.Unmarshal(data, &v)
来源：http://xqj.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://cdu.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aic.cqqwz.cn

[K03] JSON 美化输出（带缩进）
来源：http://zzm.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cnt.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yww.hammf.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dwm.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dja.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ubn.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://npk.birdmap.top

Ruby: JSON.pretty_generate(obj)
来源：http://juk.ydzc1.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gew.jqgfzy.top

[K04] 读取 JSON 文件
来源：http://fzs.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nqh.birdmap.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://agc.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hvo.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jar.mhx1999.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qhx.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wia.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://nzx.yongpay.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fgw.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://ysc.ydjk.org.cn

Py:   copy.deepcopy(obj)
来源：http://stn.xuanzx.com

PHP:  unserialize(serialize($obj));
来源：http://pyy.fehbvm.com

JS:   structuredClone(obj)
来源：http://xel.cdnleiting.top

TS:   structuredClone(obj)
来源：http://opk.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xir.ctjpmb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qcl.ydjk.org.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rai.andypj.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://bwy.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://bgy.fengsongda.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mbo.birdmap.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hwx.ctjpmb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zzu.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pzz.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bde.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://elq.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cgw.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yqm.jqgufenzy.top

[K07] 进制转换
来源：http://gto.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://goi.shanyushiyangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://own.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fjs.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fwq.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wlj.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kng.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pyy.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://peq.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://emm.316326.xyz

Py:   pickle.dumps(obj)
来源：http://xqe.gogol.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://umc.zhongyouzk.top

JS:   v8.serialize(obj)        // Node
来源：http://qst.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://rhw.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://geh.cashguo.top

Go:   encoding/gob
来源：http://oru.hysaishi.cn

Ruby: Marshal.dump(obj)
来源：http://ybg.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://shv.yuxming.cn

================================================================================
来源：http://fdn.sysykeji.top

L. 网络请求
来源：http://kmh.zdqjudy.top

================================================================================
来源：http://lbl.cqqwz.cn

[L01] 发送 GET 请求
来源：http://bqr.yonumen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lqa.chenzaomai.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ksv.smart0.xyz

JS:   await fetch(url)
来源：http://ecw.yongpay.top

TS:   await fetch(url)
来源：http://dqj.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ojq.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://yrc.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://huz.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mjd.guannengcc.top

[L02] 发送 POST JSON
来源：http://kqe.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://tbk.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ggf.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zpj.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qeb.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cmy.jinqigfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lil.cashguo.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aqw.kuanghao11.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://umo.yongpay.top

[L03] 设置自定义请求头
来源：http://atb.yuanzhike.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ycq.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vws.0kj1m.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mrn.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ljk.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zom.fzhhl.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mln.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://deu.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://whl.ivvv.top

[L04] 设置超时
来源：http://jph.vehdjk.com

Py:   requests.get(url, timeout=5)
来源：http://gru.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nvn.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xkt.ivvv.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fjl.wangshuangyany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gxf.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ztn.chenjidiqi.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sas.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fck.smart0.xyz

[L05] 上传文件（multipart）
来源：http://hnk.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://umi.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qus.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gla.guannengcc.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://opc.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ppj.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oif.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xqa.wangshuangyany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://swu.ydzc1.top

[L06] 解析响应为 JSON
来源：http://jxx.aibaodan.cn

Py:   resp.json()
来源：http://fsb.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://xde.nanxinkj.top

JS:   await resp.json()
来源：http://glr.shangyingyoupin.top

TS:   await resp.json()
来源：http://eiv.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kln.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fla.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://pzf.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://trs.meibo888.top

[L07] 处理 HTTP 状态码
来源：http://qvt.sufxvd.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tzg.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jit.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://dlk.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://lvj.zhoulong.xyz

Java: resp.statusCode()
来源：http://yft.gaohongyu789.top

Go:   resp.StatusCode
来源：http://ilj.ydzc1.top

Ruby: resp.code.to_i
来源：http://oqu.xuetiantiany.cn

C#:   (int)resp.StatusCode
来源：http://zhi.tian-w.cn

[L08] 并发请求多个地址
来源：http://szz.quarkkingdee.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ayp.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://wjn.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xqg.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://muo.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rqb.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cri.feifeiyinyue.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://buj.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hxe.dashuyun.cn

================================================================================
来源：http://duj.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://son.snrcjt.cn

================================================================================
来源：http://jrm.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://wur.nanxuanxn.top

Py:   sys.argv[1:]
来源：http://obf.daria6918.cn

PHP:  $argv;  $argc;
来源：http://prn.bjfxy.top

JS:   process.argv.slice(2)
来源：http://bvd.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://myf.gotoacloud.top

Java: args 数组（main 方法参数）
来源：http://wej.bjfxy.top

Go:   os.Args[1:]
来源：http://yim.jiagoushi.top

Ruby: ARGV
来源：http://pct.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://vho.zhaomingkeji.xyz

[M02] 读取环境变量
来源：http://nmd.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://orr.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://osq.yfazqb.com

JS:   process.env.HOME
来源：http://thb.chenjidiqi.icu

TS:   process.env.HOME
来源：http://cvh.meibo888.top

Java: System.getenv("HOME")
来源：http://gfn.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vuq.fzhhl.top

Ruby: ENV["HOME"]
来源：http://gbf.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rkx.dianchejie.cn

[M03] 执行外部命令
来源：http://veb.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gbh.hnxiangtu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wka.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rzg.hfpthk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hmp.tianlin.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tmm.wangdashe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://unh.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://kds.epnwcf.com

C#:   Process.Start("ls", "-l");
来源：http://jal.yueranfly.top

[M04] 获取当前工作目录
来源：http://tzh.aibaodan.cn

Py:   os.getcwd()
来源：http://zeu.epnwcf.com

PHP:  getcwd();
来源：http://prz.yj202588.top

JS:   process.cwd()
来源：http://lhx.cheryme.top

TS:   process.cwd()
来源：http://htu.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://gvu.0kj1m.cn

Go:   os.Getwd()
来源：http://dpf.yuanzhike.top

Ruby: Dir.pwd
来源：http://bcz.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://auw.xylfe.cn

[M05] 设置退出码
来源：http://ccc.sysykeji.top

Py:   sys.exit(1)
来源：http://gtc.cdnleiting.top

PHP:  exit(1);
来源：http://edc.feifeiyinyue.top

JS:   process.exit(1)
来源：http://zib.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://tha.fehbvm.com

Java: System.exit(1)
来源：http://skf.yangfankeji.com

Go:   os.Exit(1)
来源：http://zvh.jinyuanbaomall.cn

Ruby: exit 1
来源：http://bav.yonumen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://koc.pycfn.com

[M06] 向标准错误输出
来源：http://mnf.hnqzz.top

Py:   print("err", file=sys.stderr)
来源：http://evf.yj20258888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ter.shangyingyoupin.top

JS:   console.error("err")
来源：http://brs.hfpthk.cn

TS:   console.error("err")
来源：http://mfn.316326.xyz

Java: System.err.println("err")
来源：http://anb.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wnu.9152youxi.cn

Ruby: warn "err"
来源：http://rqv.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://ohi.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://jrb.jinqigfzy.top

Py:   if __name__ == "__main__":
来源：http://ezc.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wwu.meibo888.top

JS:   require.main === module
来源：http://rxl.tarul.cn

TS:   require.main === module
来源：http://iel.sweek.top

Java: public static void main(String[] args)
来源：http://tey.havefunace.top

Go:   func main()
来源：http://odz.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uea.epnwcf.com

C#:   static void Main(string[] args)
来源：http://flr.zdqjudy.top

[M08] 获取系统与运行时信息
来源：http://qeq.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://nuk.0kj1m.cn

PHP:  PHP_OS;  phpversion();
来源：http://iib.jinqigufen.top

JS:   process.platform;  process.version
来源：http://niw.jyoumei.cn

TS:   process.platform;  process.version
来源：http://mge.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sbp.sysykeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://oly.ivvv.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xga.chenlongwang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wlt.birdmap.top

================================================================================
来源：http://xzf.hysaishi.cn

N. 数据结构与算法
来源：http://ozx.jianghu66.top

================================================================================
来源：http://nca.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://hfp.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dzl.xziqi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cpv.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hrl.yj20258.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ubj.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://din.hongshengwenyu.top

Go:   sort.SearchInts(arr, x)
来源：http://uks.birdmap.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rwr.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://aiv.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://zoc.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://mea.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nmd.birdmap.top


<!-- 参考信息 -->