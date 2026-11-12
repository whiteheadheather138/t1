代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qaj.chenjidiqi.icu

TS:   /error/gim
来源：http://ndw.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vdj.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zlo.chenlongwang.top

Ruby: s.scan(/error/i)
来源：http://etp.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ctg.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://spe.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yka.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://odf.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ihf.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aym.sufxvd.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qjw.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://icp.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eby.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lqg.yangfankeji.com

================================================================================
来源：http://rum.vehdjk.com

J. 日期与时间
来源：http://qrv.zhixingplan.top

================================================================================
来源：http://xtz.shzxlz.cn

[J01] 获取当前时间
来源：http://fvc.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://sto.316326.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qtd.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://avq.iojbl.cn

TS:   new Date();  Date.now()
来源：http://pxh.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ict.vqdsnc.cn

Go:   time.Now()
来源：http://vek.nwbrower.top

Ruby: Time.now
来源：http://mnh.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wtd.xylfe.cn

[J02] 格式化输出
来源：http://iui.cdnleiting.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vtz.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rmn.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ago.fehbvm.com

TS:   d.toISOString()
来源：http://agn.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pdp.jyoumei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://htw.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pfu.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xvj.pycfn.com

[J03] 字符串解析为日期
来源：http://ngn.0kj1m.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wdf.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://snr.mhx1999.top

JS:   new Date("2024-01-02")
来源：http://uiu.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://uiw.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mao.chenlongwang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gfc.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://wje.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://whf.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://zdw.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kry.gaohongyu789.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cro.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dud.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://fmb.ydjk.org.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ezw.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fzp.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rdk.gotoacloud.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ryv.xziqi.cn

[J05] 时间加减（加 7 天）
来源：http://qfe.jinqigfzy.top

Py:   now + timedelta(days=7)
来源：http://cuz.mhx1999.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fgp.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ffk.daxiang520.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xhi.ywan-chungtsiang.top

Java: LocalDate.now().plusDays(7)
来源：http://ggq.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jkp.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://izq.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://khg.zdqjudy.top

[J06] 计算两时间之差
来源：http://dhn.cucudq.cn

Py:   (end - start).total_seconds()
来源：http://bdh.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://qhc.xingfuxueyuan.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://isi.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xog.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://mxa.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://igj.meibo888.top

Ruby: end - start                 # 返回秒数
来源：http://yhx.zhengqikj.top

C#:   (end - start).TotalSeconds
来源：http://ejk.ivvv.top

[J07] 比较两个日期
来源：http://gvr.shanyushiyangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://fpk.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aav.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://lhe.mhx1999.top

TS:   d1.getTime() < d2.getTime()
来源：http://rou.zhoulong.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rhr.tianlin.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cyd.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://yvn.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://grh.daxiang520.top

[J08] 提取年月日与星期
来源：http://jsj.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://msf.ywan-chungtsiang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vrd.ybcxt.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yae.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://imr.cheryme.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dgu.meibo888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qrg.chenzaomai.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ujn.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uqp.xuanzx.com

[J09] 时区处理
来源：http://zco.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://efw.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bdp.zhijiandao.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rcv.fktsv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mcd.jinghuilouyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ayl.yongpay.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bem.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://rvn.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kjj.sweek.top

[J10] 取今天 / 本月第一天
来源：http://twk.jqgfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ygo.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dgf.jqgufenzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kze.wangshuangyany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mju.xziqi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qkx.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://puz.chenjidiqi.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ifh.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cbr.guannengcc.top

================================================================================
来源：http://ano.havefunace.top

K. JSON 与序列化
来源：http://gvz.gogol.net.cn

================================================================================
来源：http://bhg.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://grv.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sxz.sysykeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ihd.hammf.cn

JS:   JSON.stringify(obj)
来源：http://wqp.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://sse.fehbvm.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xlk.fengsongda.top

Go:   json.Marshal(obj)
来源：http://gvp.zhixingplan.top

Ruby: obj.to_json                                     // require "json"
来源：http://kww.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tgt.ivvv.top

[K02] JSON 字符串转对象
来源：http://tuc.pycfn.com

Py:   json.loads(s)
来源：http://etg.guowangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ywj.dashuyun.cn

JS:   JSON.parse(s)
来源：http://qhw.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://hzj.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jav.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://snp.c1oappe.top

Ruby: JSON.parse(s)
来源：http://eyq.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kng.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://uhi.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hnf.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dyg.xuanzx.com

JS:   JSON.stringify(obj, null, 2)
来源：http://fir.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gdo.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://btr.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qho.hnqzz.top

Ruby: JSON.pretty_generate(obj)
来源：http://uxj.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://acd.yfazqb.com

[K04] 读取 JSON 文件
来源：http://fuz.xinyue.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jjr.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yju.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dbr.zdbjq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kwu.hammf.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lzt.yuxming.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gjh.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dfh.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uje.yfazqb.com

[K05] 深拷贝对象
来源：http://lmv.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://fzx.yj20258.top

PHP:  unserialize(serialize($obj));
来源：http://ldl.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://kyd.sweek.top

TS:   structuredClone(obj)
来源：http://fac.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gja.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cii.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ikn.sxryk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://esd.hysaishi.cn

[K06] 解析 URL 查询串
来源：http://rnt.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ctg.0kj1m.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bjx.xuetiantiany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rlw.xziqi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://txd.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nxc.pengpengdd.cyou

Go:   url.ParseQuery("a=1&b=2")
来源：http://vjv.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hmw.birdmap.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://udv.yj202588.top

[K07] 进制转换
来源：http://irc.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://niy.ybcxt.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fbf.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qid.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kqs.smart0.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bos.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jhe.vqdsnc.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dmr.ydzc1.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bjy.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://ffx.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://ksj.jianghu66.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nqv.nanxinkj.top

JS:   v8.serialize(obj)        // Node
来源：http://zdu.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://lhy.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://avu.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://cyn.nanxuanxn.top

Ruby: Marshal.dump(obj)
来源：http://xzl.zhaomingkeji.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vlm.dianchejie.cn

================================================================================
来源：http://vdn.gaohongyu789.top

L. 网络请求
来源：http://xhw.sjlbkw.cn

================================================================================
来源：http://jdv.cdnleiting.top

[L01] 发送 GET 请求
来源：http://vfg.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ihx.yj20258888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://grr.fktsv.cn

JS:   await fetch(url)
来源：http://tef.ctjpmb.com

TS:   await fetch(url)
来源：http://hfe.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pvh.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://mmz.hfpthk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ail.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wle.jinqigufen.top

[L02] 发送 POST JSON
来源：http://pdk.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://eln.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rsb.ivvv.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://egb.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tza.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rjw.dianchejie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gnl.kuanghao11.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nvt.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rkb.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://vvc.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ach.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cvp.yongpay.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fwi.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ofs.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://drc.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jph.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bbb.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rma.hcnkem.com

[L04] 设置超时
来源：http://uon.shanyushiyangtech.top

Py:   requests.get(url, timeout=5)
来源：http://eyc.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bkw.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ukp.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pdx.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ezb.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gbf.316326.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lbh.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tnp.feifeiyinyue.top

[L05] 上传文件（multipart）
来源：http://zuv.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nmp.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ugr.52xcode.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://idh.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hml.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ijf.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tgs.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cfu.cucudq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jeh.tian-w.cn

[L06] 解析响应为 JSON
来源：http://cye.jlsjyb.cn

Py:   resp.json()
来源：http://mvd.cashguo.top

PHP:  json_decode($body, true);
来源：http://dfr.vqdsnc.cn

JS:   await resp.json()
来源：http://snv.hnqzz.top

TS:   await resp.json()
来源：http://gop.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wqu.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dse.zhengqikj.top

Ruby: JSON.parse(resp.body)
来源：http://ctn.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jca.ehwqpu.com

[L07] 处理 HTTP 状态码
来源：http://spq.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bjv.xinyue.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xwp.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://dui.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://xwh.nanxuanxn.top

Java: resp.statusCode()
来源：http://pyr.hesvh.cn

Go:   resp.StatusCode
来源：http://jfg.yangfankeji.com

Ruby: resp.code.to_i
来源：http://bpf.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://evh.cashguo.top

[L08] 并发请求多个地址
来源：http://lsx.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://orf.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://qqj.hysaishi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lmh.hnqzz.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wwm.fzhhl.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nre.zhoulong.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kvd.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cir.xylfe.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hop.xziqi.cn

================================================================================
来源：http://ati.cucudq.cn

M. 命令行 / 进程 / 环境
来源：http://ezy.mhx1999.top

================================================================================
来源：http://qxl.yueranfly.top

[M01] 读取命令行参数
来源：http://npo.ehwqpu.com

Py:   sys.argv[1:]
来源：http://gew.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://eps.kuanghao11.cn

JS:   process.argv.slice(2)
来源：http://opc.tian-w.cn

TS:   process.argv.slice(2)
来源：http://okd.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://bfu.fktsv.cn

Go:   os.Args[1:]
来源：http://wmu.zhiwuduotai.top

Ruby: ARGV
来源：http://euh.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://era.zhijiandao.cn

[M02] 读取环境变量
来源：http://szc.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://xhc.cashguo.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bmy.chenzaomai.com

JS:   process.env.HOME
来源：http://xxl.snrcjt.cn

TS:   process.env.HOME
来源：http://hdg.jianghu66.top

Java: System.getenv("HOME")
来源：http://jau.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xjy.316326.xyz

Ruby: ENV["HOME"]
来源：http://tjv.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pgr.wangdashe.top

[M03] 执行外部命令
来源：http://ias.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fdo.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sgq.fehbvm.com

JS:   child_process.execSync("ls -l").toString()
来源：http://bsj.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://eyy.ppjwa.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kcb.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://njj.chenzaomai.com

Ruby: system("ls -l");  `ls -l`
来源：http://vjp.jinqigfzy.top

C#:   Process.Start("ls", "-l");
来源：http://wqf.ctjpmb.com

[M04] 获取当前工作目录
来源：http://bms.gzhubu.top

Py:   os.getcwd()
来源：http://qcl.gogol.net.cn

PHP:  getcwd();
来源：http://ioj.52xcode.cn

JS:   process.cwd()
来源：http://vwn.jinqigufen.top

TS:   process.cwd()
来源：http://nfh.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://ppn.xingfuxueyuan.xyz

Go:   os.Getwd()
来源：http://ldj.jqgfzy.top

Ruby: Dir.pwd
来源：http://ojs.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://zhm.dianchejie.cn

[M05] 设置退出码
来源：http://sgz.fzhhl.top

Py:   sys.exit(1)
来源：http://qol.feifeiyinyue.top

PHP:  exit(1);
来源：http://eic.hammf.cn


<!-- 参考信息 -->