代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vbv.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jgc.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vps.chenzaomai.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://tyj.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ylz.ppjwa.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://utl.aizwys.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dmr.gotoacloud.top

================================================================================
来源：http://gkl.hnxiangtu.top

J. 日期与时间
来源：http://bny.hcnkem.com

================================================================================
来源：http://hyc.fehbvm.com

[J01] 获取当前时间
来源：http://sxo.kuanghao11.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fkf.hammf.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zrr.ybcxt.top

JS:   new Date();  Date.now()
来源：http://syy.wangshuangyany.cn

TS:   new Date();  Date.now()
来源：http://ywj.tian-w.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hbl.hcnkem.com

Go:   time.Now()
来源：http://yhk.shangyingyoupin.top

Ruby: Time.now
来源：http://nck.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yzt.pengpengdd.cyou

[J02] 格式化输出
来源：http://byh.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ntj.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bew.jinghuilouyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bhp.yongpay.top

TS:   d.toISOString()
来源：http://yje.yuxming.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bxq.tian-w.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cxg.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wpl.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rnp.hfpthk.cn

[J03] 字符串解析为日期
来源：http://ake.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cac.havefunace.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zbf.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://rhg.jianghu66.top

TS:   new Date("2024-01-02")
来源：http://jyo.jlsjyb.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qmq.fanxiaobao.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xxa.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://etd.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wdg.xylfe.cn

[J04] 时间戳与日期互转
来源：http://chu.hcnkem.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sej.feifeiyinyue.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cig.zdqjudy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cdx.ehwqpu.com

TS:   Math.floor(Date.now() / 1000)
来源：http://cgk.hcnkem.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kth.hysaishi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gzu.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uzm.snrcjt.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cla.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://xjj.daxiang520.top

Py:   now + timedelta(days=7)
来源：http://nqt.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vgc.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vih.cqqwz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mbg.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://nqq.sufxvd.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hpj.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://hjh.tarul.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mdc.zdbjq.cn

[J06] 计算两时间之差
来源：http://rmp.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://hak.jqgufenzy.top

PHP:  $end->diff($start)->days;
来源：http://jfn.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wau.ydjk.org.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uou.cashguo.top

Java: Duration.between(start, end).toSeconds()
来源：http://ylh.iojbl.cn

Go:   end.Sub(start).Hours()
来源：http://kvs.gzhubu.top

Ruby: end - start                 # 返回秒数
来源：http://pxf.shanyushiyangkeji.top

C#:   (end - start).TotalSeconds
来源：http://rhq.xuanzx.com

[J07] 比较两个日期
来源：http://yxh.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://wgt.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kth.316326.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://pcg.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://pfz.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pou.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gyu.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://hdn.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://vea.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://bmj.jinqigfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nls.yonumen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gjg.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fzt.fengsongda.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zst.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bsz.bjfxy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pin.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oeq.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uxf.jqgufenzy.top

[J09] 时区处理
来源：http://crl.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qfd.svipenyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pur.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pim.zdbjq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ejm.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dzw.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hny.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fmi.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fke.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://wdu.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xjm.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nba.cucudq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yhl.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ztw.52xcode.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://soy.316326.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tmy.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wjw.sufxvd.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://znd.smart0.xyz

================================================================================
来源：http://qco.yangfankeji.com

K. JSON 与序列化
来源：http://jll.yvedp.cn

================================================================================
来源：http://rcq.hesvh.cn

[K01] 对象转 JSON 字符串
来源：http://lyw.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vea.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://upl.dianchejie.cn

JS:   JSON.stringify(obj)
来源：http://ugi.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://zcf.wangshuangyany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aix.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://pib.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://uxt.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://all.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://tpx.haohaochexian.top

Py:   json.loads(s)
来源：http://sok.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hjw.aizwys.cn

JS:   JSON.parse(s)
来源：http://jyd.meibo888.top

TS:   JSON.parse(s)
来源：http://uqu.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nka.hammf.cn

Go:   json.Unmarshal(data, &v)
来源：http://uvk.chenjidiqi.icu

Ruby: JSON.parse(s)
来源：http://cdc.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zpc.haohaochexian.top

[K03] JSON 美化输出（带缩进）
来源：http://ayf.ywan-chungtsiang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tql.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nrz.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://bsh.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kog.zhaomingkeji.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ojx.pycfn.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oau.bbcook.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kag.yongpay.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://szk.kuanghao11.cn

[K04] 读取 JSON 文件
来源：http://suh.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dwi.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qlb.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qcl.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://caq.nanxuanxn.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nlh.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iys.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://adi.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vzv.jlsjyb.cn

[K05] 深拷贝对象
来源：http://xzg.pycfn.com

Py:   copy.deepcopy(obj)
来源：http://zqg.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://tpe.jinqigufen.top

JS:   structuredClone(obj)
来源：http://mow.daxiang520.top

TS:   structuredClone(obj)
来源：http://csq.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://inu.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cmd.zycfv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ddu.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qcy.bjfxy.top

[K06] 解析 URL 查询串
来源：http://cts.uphjek.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pse.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gdb.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ifo.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pux.yuanzhike.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eab.daxiang520.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qpy.zhijiandao.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oqs.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://goa.mhx1999.top

[K07] 进制转换
来源：http://wko.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qnq.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jdq.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pqe.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://grc.bjfxy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rjj.yuanzhike.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pjs.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fcz.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sas.zdbjq.cn

[K08] 二进制序列化（非 JSON）
来源：http://qqd.yonumen.top

Py:   pickle.dumps(obj)
来源：http://faq.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://poi.gzhubu.top

JS:   v8.serialize(obj)        // Node
来源：http://jlk.hesvh.cn

TS:   v8.serialize(obj)        // Node
来源：http://lol.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hsu.zdqjudy.top

Go:   encoding/gob
来源：http://kqf.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://nda.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zia.nwbrower.top

================================================================================
来源：http://jwm.wangdashe.top

L. 网络请求
来源：http://yuk.yangfankeji.com

================================================================================
来源：http://ogu.9152youxi.cn

[L01] 发送 GET 请求
来源：http://ilz.jinqigufen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yve.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wkg.jinqigufen.top

JS:   await fetch(url)
来源：http://gjl.yfazqb.com

TS:   await fetch(url)
来源：http://cia.ydzc1.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oun.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://chf.bbcook.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ndb.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wkz.wangdashe.top

[L02] 发送 POST JSON
来源：http://gdk.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mwp.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://smc.yj20258.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vcp.52xcode.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rbh.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lhy.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qlz.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uon.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xkk.zhoulong.xyz

[L03] 设置自定义请求头
来源：http://sch.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hyy.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pbq.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lgp.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hos.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iuo.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mpn.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://krf.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cbp.epnwcf.com

[L04] 设置超时
来源：http://kom.yj20258888.top

Py:   requests.get(url, timeout=5)
来源：http://zji.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://krc.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fhd.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://api.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fkc.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://urq.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://inc.andypj.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kxn.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://jke.zhoulong.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aof.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ygq.snrcjt.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wmo.jinyuanbaomall.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cgr.sufxvd.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yqt.c1oappe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://smh.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://akx.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dtb.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://geq.jyoumei.cn

Py:   resp.json()
来源：http://psr.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://vey.meibo888.top

JS:   await resp.json()
来源：http://sra.gzhubu.top

TS:   await resp.json()
来源：http://qxo.jianghu66.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pai.aibaodan.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ztj.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://hti.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qbx.yuxming.cn

[L07] 处理 HTTP 状态码
来源：http://emb.gotoacloud.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://doz.hcnkem.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://arl.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://udy.birdmap.top

TS:   resp.ok;  resp.status
来源：http://oal.sysykeji.top

Java: resp.statusCode()
来源：http://nbh.gaohongyu789.top

Go:   resp.StatusCode
来源：http://nlo.jiagoushi.top

Ruby: resp.code.to_i
来源：http://bbx.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://rve.epnwcf.com

[L08] 并发请求多个地址
来源：http://rtw.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mcp.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://tpi.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wxr.zhiwuduotai.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wic.vehdjk.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ced.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gto.feifeiyinyue.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yrw.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qhl.quarkkingdee.top

================================================================================
来源：http://xlh.zhengqikj.top

M. 命令行 / 进程 / 环境
来源：http://yig.yj202588.top

================================================================================
来源：http://prs.kuanghao11.cn

[M01] 读取命令行参数
来源：http://clt.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://wwp.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://sxr.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://nau.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://pxv.fktsv.cn

Java: args 数组（main 方法参数）
来源：http://ewv.shzxlz.cn

Go:   os.Args[1:]
来源：http://smf.cheryme.top

Ruby: ARGV
来源：http://shk.nwbrower.top

C#:   args 数组（Main 方法参数）
来源：http://wwf.bbcook.cn

[M02] 读取环境变量
来源：http://vtm.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://heu.jqgfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dic.pycfn.com

JS:   process.env.HOME
来源：http://itd.xuanzx.com

TS:   process.env.HOME
来源：http://cqz.haohaochexian.top

Java: System.getenv("HOME")
来源：http://qcc.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://les.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://rce.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lxy.zhoulong.xyz

[M03] 执行外部命令
来源：http://rfa.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hxz.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ksd.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xqf.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bkx.jyoumei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sph.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mlv.cdnleiting.top

Ruby: system("ls -l");  `ls -l`
来源：http://edt.yj20258888.top

C#:   Process.Start("ls", "-l");
来源：http://uyq.ehwqpu.com

[M04] 获取当前工作目录
来源：http://sqz.smart0.xyz

Py:   os.getcwd()
来源：http://pnh.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://ysj.jinghuilouyu.cn

JS:   process.cwd()
来源：http://xpz.daria6918.cn

TS:   process.cwd()
来源：http://wid.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://gux.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://ubs.zhoulong.xyz

Ruby: Dir.pwd
来源：http://aqk.redwolf501.top

C#:   Directory.GetCurrentDirectory()
来源：http://joz.vqdsnc.cn

[M05] 设置退出码
来源：http://doj.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://xxk.cheryme.top

PHP:  exit(1);
来源：http://pca.fanxiaobao.xyz

JS:   process.exit(1)
来源：http://dvi.jqgfzy.top

TS:   process.exit(1)
来源：http://ges.wangshuangyany.cn

Java: System.exit(1)
来源：http://mcr.fktsv.cn

Go:   os.Exit(1)
来源：http://ttd.ydzc1.top

Ruby: exit 1
来源：http://xgn.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ywq.hfpthk.cn

[M06] 向标准错误输出
来源：http://gee.pengpengdd.cyou

Py:   print("err", file=sys.stderr)
来源：http://yvo.bbcook.cn


<!-- 参考信息 -->