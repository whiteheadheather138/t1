代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bie.guannengcc.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://maj.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://omc.bjfxy.top

================================================================================
来源：http://gzy.jyoumei.cn

J. 日期与时间
来源：http://uxg.gogol.net.cn

================================================================================
来源：http://fos.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://oly.bjfxy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gsn.cdnleiting.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tfw.aibaodan.cn

JS:   new Date();  Date.now()
来源：http://cwq.yuxming.cn

TS:   new Date();  Date.now()
来源：http://yqx.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://aip.zycfv.cn

Go:   time.Now()
来源：http://dkr.uphjek.com

Ruby: Time.now
来源：http://svg.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kwn.316326.xyz

[J02] 格式化输出
来源：http://dgm.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://txq.sxryk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ncz.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jaq.zycfv.cn

TS:   d.toISOString()
来源：http://oke.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yrs.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ews.chenlongwang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tae.jqgfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hof.chenjidiqi.icu

[J03] 字符串解析为日期
来源：http://ihz.nanxuanxn.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xwg.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ytk.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://ifn.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://ibo.vqdsnc.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mdo.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ggc.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://uph.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ofi.zhijiandao.cn

[J04] 时间戳与日期互转
来源：http://ndb.fanxiaobao.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wau.yfazqb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://acb.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jff.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wiu.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://omh.sufxvd.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hnr.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ikp.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xlo.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://ybw.hcnkem.com

Py:   now + timedelta(days=7)
来源：http://scj.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zxz.sysykeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ksh.jinyuanbaomall.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rnu.0kj1m.cn

Java: LocalDate.now().plusDays(7)
来源：http://gio.xingfuxueyuan.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qcr.guannengcc.top

Ruby: Time.now + 7 * 86400
来源：http://ris.hywenlv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gkx.pengpengdd.cyou

[J06] 计算两时间之差
来源：http://uvr.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://xrq.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://afe.dianchejie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://spk.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://scj.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://rdt.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://fce.xuetiantiany.cn

Ruby: end - start                 # 返回秒数
来源：http://cym.jqgufenzy.top

C#:   (end - start).TotalSeconds
来源：http://bea.jyoumei.cn

[J07] 比较两个日期
来源：http://tco.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://quo.xinyue.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mqu.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://kmt.andypj.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://qwj.xuanzx.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gds.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rlm.tanke756.top

Ruby: d1 < d2;  d1 == d2
来源：http://qvr.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://pqw.yanxiufei.cn

[J08] 提取年月日与星期
来源：http://syl.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blu.52xcode.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ica.yuxming.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://srh.zhiwuduotai.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://odt.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rdr.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hya.jinqigufen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zsx.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://evs.xuetiantiany.cn

[J09] 时区处理
来源：http://fey.zhoulong.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://idx.hesvh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zvk.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nbr.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://utu.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ptj.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fox.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://dax.xuanzx.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wvc.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://xom.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vry.jinqigufen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mnm.zhengqikj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tgu.chenlongwang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sow.pycfn.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bkr.yfazqb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vdx.guowangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://esp.hywenlv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lrn.zdbjq.cn

================================================================================
来源：http://rjm.andypj.xyz

K. JSON 与序列化
来源：http://utz.hfpthk.cn

================================================================================
来源：http://zic.shanyushiyangtech.top

[K01] 对象转 JSON 字符串
来源：http://clq.tianlin.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pzq.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uex.zhengqikj.top

JS:   JSON.stringify(obj)
来源：http://kao.xuanzx.com

TS:   JSON.stringify(obj)
来源：http://nwi.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dwn.sysykeji.top

Go:   json.Marshal(obj)
来源：http://ien.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://eib.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fhy.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://lll.feifeiyinyue.top

Py:   json.loads(s)
来源：http://sdu.gotoacloud.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zhj.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://hjy.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://mvc.yangfankeji.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xtj.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://wsw.iojbl.cn

Ruby: JSON.parse(s)
来源：http://zui.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mns.snrcjt.cn

[K03] JSON 美化输出（带缩进）
来源：http://djb.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uxv.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bxe.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oqv.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sxj.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dbz.52xcode.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qfp.xuanzx.com

Ruby: JSON.pretty_generate(obj)
来源：http://rpz.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dba.sxryk.cn

[K04] 读取 JSON 文件
来源：http://mav.ybcxt.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gvs.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fsg.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zzk.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ujn.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dac.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yfr.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://crm.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lcp.zdbjq.cn

[K05] 深拷贝对象
来源：http://wzt.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://jpw.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://gci.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://ckr.yonumen.top

TS:   structuredClone(obj)
来源：http://nqt.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://foi.tian-w.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uws.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://opz.jinqigfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://oqh.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://aeo.svipenyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://afp.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kox.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bba.nwbrower.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bna.fehbvm.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gpm.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ljr.guannengcc.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gzf.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://skp.aizwys.cn

[K07] 进制转换
来源：http://kdx.daria6918.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fqc.yonumen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cgv.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bkr.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://smc.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://spf.xuetiantiany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cma.jlsjyb.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hzm.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pro.shzxlz.cn

[K08] 二进制序列化（非 JSON）
来源：http://lsm.uphjek.com

Py:   pickle.dumps(obj)
来源：http://zof.nanxuanxn.top

PHP:  serialize($obj);  unserialize($s);
来源：http://slh.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://lyn.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://obk.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://men.aizwys.cn

Go:   encoding/gob
来源：http://hjc.haohaochexian.top

Ruby: Marshal.dump(obj)
来源：http://ono.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rwv.birdmap.top

================================================================================
来源：http://aqz.vehdjk.com

L. 网络请求
来源：http://wkq.wangshuangyany.cn

================================================================================
来源：http://xke.316326.xyz

[L01] 发送 GET 请求
来源：http://nqb.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://orz.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yrz.aizwys.cn

JS:   await fetch(url)
来源：http://bbk.sjlbkw.cn

TS:   await fetch(url)
来源：http://xdk.jianghu66.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ynq.gotoacloud.top

Go:   resp, err := http.Get(url)
来源：http://apf.fanxiaobao.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://xnx.guannengcc.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pfs.fzhhl.top

[L02] 发送 POST JSON
来源：http://kjn.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://jbh.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rjm.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://njz.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://trf.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gut.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sxp.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jlo.gzhubu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qih.hfpthk.cn

[L03] 设置自定义请求头
来源：http://ndo.jiagoushi.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sqx.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lqj.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dmh.gogol.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lxr.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vey.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iev.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lek.yj20258.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qfo.nanxinkj.top

[L04] 设置超时
来源：http://wmm.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://qnx.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tqh.zhoulong.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zup.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xzc.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ucn.mhx1999.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iou.tarul.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fmu.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gkb.hnqzz.top

[L05] 上传文件（multipart）
来源：http://gas.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zkc.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rwb.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nwm.shanyushiyangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mcp.wangshuangyany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ihq.0kj1m.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wqy.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://urf.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rlu.hnqzz.top

[L06] 解析响应为 JSON
来源：http://prn.sufxvd.cn

Py:   resp.json()
来源：http://hrs.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://bwr.gaohongyu789.top

JS:   await resp.json()
来源：http://abp.nwbrower.top

TS:   await resp.json()
来源：http://ykj.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sex.ppjwa.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://spp.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://ffk.gzhubu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ywy.jyoumei.cn

[L07] 处理 HTTP 状态码
来源：http://tdr.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://toq.jiagoushi.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ozr.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://cfy.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://tjf.birdmap.top

Java: resp.statusCode()
来源：http://ppv.yj20258888.top

Go:   resp.StatusCode
来源：http://tuq.gzhubu.top

Ruby: resp.code.to_i
来源：http://ose.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://mfc.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://hje.sufxvd.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nyu.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://lik.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ore.hammf.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zun.ybcxt.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hxi.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://url.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tcv.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://crv.hysaishi.cn

================================================================================
来源：http://fzx.redwolf501.top

M. 命令行 / 进程 / 环境
来源：http://yjc.xingfuxueyuan.xyz

================================================================================
来源：http://aav.yj20258.top

[M01] 读取命令行参数
来源：http://xne.yanxiufei.cn

Py:   sys.argv[1:]
来源：http://asg.fengsongda.top

PHP:  $argv;  $argc;
来源：http://srh.hesvh.cn

JS:   process.argv.slice(2)
来源：http://hac.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://ydb.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://ikp.c1oappe.top

Go:   os.Args[1:]
来源：http://jss.jinghuilouyu.cn

Ruby: ARGV
来源：http://svf.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://geq.uphjek.com

[M02] 读取环境变量
来源：http://wof.zhijiandao.cn

Py:   os.environ.get("HOME")
来源：http://wik.yvedp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://twa.feifeiyinyue.top

JS:   process.env.HOME
来源：http://rdk.shzxlz.cn

TS:   process.env.HOME
来源：http://xuf.yanxiufei.cn

Java: System.getenv("HOME")
来源：http://dgd.jlsjyb.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qny.yuxming.cn

Ruby: ENV["HOME"]
来源：http://bug.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fpq.redwolf501.top

[M03] 执行外部命令
来源：http://ebe.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cid.chenlongwang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nwu.feifeiyinyue.top

JS:   child_process.execSync("ls -l").toString()
来源：http://scl.chenlongwang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bpk.ybcxt.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vvp.ydjk.org.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dja.yanxiufei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jtl.hnxiangtu.top

C#:   Process.Start("ls", "-l");
来源：http://bfw.jqgufenzy.top

[M04] 获取当前工作目录
来源：http://ovu.yvedp.cn

Py:   os.getcwd()
来源：http://sfv.redwolf501.top

PHP:  getcwd();
来源：http://wkd.gotoacloud.top

JS:   process.cwd()
来源：http://oqz.guowangkeji.top

TS:   process.cwd()
来源：http://tor.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://pyo.xuanzx.com

Go:   os.Getwd()
来源：http://zka.guannengcc.top

Ruby: Dir.pwd
来源：http://esj.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://hks.fktsv.cn

[M05] 设置退出码
来源：http://opf.guannengcc.top

Py:   sys.exit(1)
来源：http://qqm.cashguo.top

PHP:  exit(1);
来源：http://hpb.yanxiufei.cn

JS:   process.exit(1)
来源：http://ufy.yuanzhike.top

TS:   process.exit(1)
来源：http://sqi.snrcjt.cn

Java: System.exit(1)
来源：http://hlx.havefunace.top

Go:   os.Exit(1)
来源：http://jei.daria6918.cn

Ruby: exit 1
来源：http://ytz.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bxa.zdbjq.cn

[M06] 向标准错误输出
来源：http://nib.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://bmb.jinyuanbaomall.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zbx.bbcook.cn

JS:   console.error("err")
来源：http://sef.zdqjudy.top

TS:   console.error("err")
来源：http://ogd.andypj.xyz

Java: System.err.println("err")
来源：http://lvv.smart0.xyz


<!-- 参考信息 -->