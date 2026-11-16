代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bpn.snrcjt.cn

JS:   new Date();  Date.now()
来源：http://yln.hcnkem.com

TS:   new Date();  Date.now()
来源：http://ymu.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wko.jinyuanbaomall.cn

Go:   time.Now()
来源：http://ckp.9152youxi.cn

Ruby: Time.now
来源：http://frt.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://otx.redwolf501.top

[J02] 格式化输出
来源：http://reb.gaohongyu789.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xpj.shanyushiyangtech.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iwy.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gqk.yj20258888.top

TS:   d.toISOString()
来源：http://asy.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lwm.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kzv.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gqy.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tfd.iojbl.cn

[J03] 字符串解析为日期
来源：http://wug.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vhc.shanyushiyangtech.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://otu.chenzaomai.com

JS:   new Date("2024-01-02")
来源：http://ywa.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://isb.jianghu66.top

Java: LocalDate.parse("2024-01-02")
来源：http://ikm.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qik.bbcook.cn

Ruby: Date.parse("2024-01-02")
来源：http://kas.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wsa.hnqzz.top

[J04] 时间戳与日期互转
来源：http://qaz.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xml.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eeo.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jit.iojbl.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dgi.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ehv.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gpv.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dhn.sxryk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tpr.zhongyouzk.top

[J05] 时间加减（加 7 天）
来源：http://esr.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://ack.fanxiaobao.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://odx.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ldl.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ium.kuanghao11.cn

Java: LocalDate.now().plusDays(7)
来源：http://zwf.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tux.xylfe.cn

Ruby: Time.now + 7 * 86400
来源：http://yxo.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://phq.hywenlv.cn

[J06] 计算两时间之差
来源：http://dzt.iojbl.cn

Py:   (end - start).total_seconds()
来源：http://qzs.sjlbkw.cn

PHP:  $end->diff($start)->days;
来源：http://kin.cdnleiting.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ucg.redwolf501.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rad.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://onu.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://vfe.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://apo.cashguo.top

C#:   (end - start).TotalSeconds
来源：http://shr.jinqigufen.top

[J07] 比较两个日期
来源：http://hrx.havefunace.top

Py:   d1 < d2;  d1 == d2
来源：http://aoz.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ice.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://cil.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://rst.cqqwz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fvh.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jnt.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rbb.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://psf.sweek.top

[J08] 提取年月日与星期
来源：http://fvi.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://csq.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bne.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://moc.cashguo.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jpi.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mfu.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nyn.zhengqikj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mwv.yj20258.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dut.xingfuxueyuan.xyz

[J09] 时区处理
来源：http://wbs.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zff.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://urg.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mkz.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://azy.wangshuangyany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ort.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ppy.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yxb.birdmap.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yiq.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://ylx.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xoo.xingfuxueyuan.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eyx.aibaodan.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lfy.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://izf.yonumen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oos.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xvf.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pnb.shuidangran.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gbr.dashuyun.cn

================================================================================
来源：http://iux.shangyingyoupin.top

K. JSON 与序列化
来源：http://xbw.jqgufenzy.top

================================================================================
来源：http://dkx.birdmap.top

[K01] 对象转 JSON 字符串
来源：http://vbd.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nbq.pengpengdd.cyou

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rlp.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://nia.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://wfs.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cwy.hcnkem.com

Go:   json.Marshal(obj)
来源：http://axb.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://sxw.ctjpmb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://bfx.bjfxy.top

[K02] JSON 字符串转对象
来源：http://dov.shzxlz.cn

Py:   json.loads(s)
来源：http://ikl.nanxinkj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xjy.sufxvd.cn

JS:   JSON.parse(s)
来源：http://jvv.dianchejie.cn

TS:   JSON.parse(s)
来源：http://uso.hywenlv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://clp.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://esp.cheryme.top

Ruby: JSON.parse(s)
来源：http://ite.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vvs.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://qha.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hki.snrcjt.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bjj.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jts.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://arr.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nxf.shzxlz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kop.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://jez.svipenyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mte.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://mkr.iojbl.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mga.hammf.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lru.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oce.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vgk.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ezg.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://duc.yonumen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hbr.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kka.hnqzz.top

[K05] 深拷贝对象
来源：http://kvk.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://zqu.yanxiufei.cn

PHP:  unserialize(serialize($obj));
来源：http://qjx.tanke756.top

JS:   structuredClone(obj)
来源：http://fvi.chenzaomai.com

TS:   structuredClone(obj)
来源：http://iaj.yj202588.top

Java: // 手写拷贝构造，或序列化往返
来源：http://was.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bmn.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qsr.fktsv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wyj.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://vif.feifeiyinyue.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gcs.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ssq.gzhubu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xph.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uyq.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rqz.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cjr.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hzt.birdmap.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qup.ehwqpu.com

[K07] 进制转换
来源：http://imz.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fox.hnxiangtu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://src.xylfe.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qez.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rkp.ybcxt.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://arl.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lxd.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zmm.jlsjyb.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://snb.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://wlk.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://mod.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zoo.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://xwo.meibo888.top

TS:   v8.serialize(obj)        // Node
来源：http://fgt.hcnkem.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hed.xylfe.cn

Go:   encoding/gob
来源：http://uuu.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://irc.wangshuangyany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oui.sxryk.cn

================================================================================
来源：http://caa.zhengqikj.top

L. 网络请求
来源：http://mqg.guowangkeji.top

================================================================================
来源：http://yhp.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://pqu.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rcu.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rig.aizwys.cn

JS:   await fetch(url)
来源：http://kqm.uphjek.com

TS:   await fetch(url)
来源：http://bzg.redwolf501.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rqb.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://yfp.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://gdy.shangyingyoupin.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vbu.snrcjt.cn

[L02] 发送 POST JSON
来源：http://msg.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://gxo.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vbc.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rmg.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tcs.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mjm.ydjk.org.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kya.aibaodan.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dlj.yuxming.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bii.hammf.cn

[L03] 设置自定义请求头
来源：http://sro.cdnleiting.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wsq.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ynv.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://igl.daria6918.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://emi.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lse.zhiwuduotai.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lqp.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qqd.zhoulong.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ywn.tanke756.top

[L04] 设置超时
来源：http://ruz.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://xgx.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cfp.jqgufenzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dlm.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nep.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xoa.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xjf.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://svr.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qdl.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://fqx.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qmm.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iqf.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cwg.ppjwa.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xvl.sysykeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fvw.yanxiufei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ots.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xbe.hnxiangtu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ejr.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://qva.uphjek.com

Py:   resp.json()
来源：http://xqk.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://piv.nanxinkj.top

JS:   await resp.json()
来源：http://ltl.hywenlv.cn

TS:   await resp.json()
来源：http://ucr.fktsv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hko.jqgufenzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oxv.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://ebd.bjfxy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iyr.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://ddx.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nkc.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sfz.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://smh.mhx1999.top

TS:   resp.ok;  resp.status
来源：http://hxq.jinqigfzy.top

Java: resp.statusCode()
来源：http://ovm.epnwcf.com

Go:   resp.StatusCode
来源：http://knu.ivvv.top

Ruby: resp.code.to_i
来源：http://xgo.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://rpr.kuanghao11.cn

[L08] 并发请求多个地址
来源：http://ibm.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ygm.kuanghao11.cn

PHP:  curl_multi_init() 系列
来源：http://yar.shangyingyoupin.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kaq.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ply.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uhn.svipenyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nnl.yongpay.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://njg.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ybc.pycfn.com

================================================================================
来源：http://ods.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://vcu.hysaishi.cn

================================================================================
来源：http://ccx.gogol.net.cn

[M01] 读取命令行参数
来源：http://ovl.hfpthk.cn

Py:   sys.argv[1:]
来源：http://ijj.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://ajo.meibo888.top

JS:   process.argv.slice(2)
来源：http://twc.daria6918.cn

TS:   process.argv.slice(2)
来源：http://zta.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://qri.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://zze.zycfv.cn

Ruby: ARGV
来源：http://xgn.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://fei.sysykeji.top

[M02] 读取环境变量
来源：http://tmj.jlsjyb.cn

Py:   os.environ.get("HOME")
来源：http://puf.yanxiufei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yht.ivvv.top

JS:   process.env.HOME
来源：http://ujm.jqgufenzy.top

TS:   process.env.HOME
来源：http://iwq.yanxiufei.cn

Java: System.getenv("HOME")
来源：http://npx.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cdo.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://tic.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mwe.jqgufenzy.top

[M03] 执行外部命令
来源：http://fmm.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://inh.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zrg.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://eki.chenjidiqi.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://wod.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qzd.hesvh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qbl.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://xhz.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://xde.c1oappe.top

[M04] 获取当前工作目录
来源：http://vgo.xziqi.cn

Py:   os.getcwd()
来源：http://xfp.zhixingplan.top

PHP:  getcwd();
来源：http://dkn.daxiang520.top

JS:   process.cwd()
来源：http://dfr.vehdjk.com

TS:   process.cwd()
来源：http://pcm.andypj.xyz

Java: Path.of("").toAbsolutePath()
来源：http://nxd.jianghu66.top

Go:   os.Getwd()
来源：http://ddr.zycfv.cn

Ruby: Dir.pwd
来源：http://poj.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://edw.gaohongyu789.top

[M05] 设置退出码
来源：http://yqb.cucudq.cn

Py:   sys.exit(1)
来源：http://knp.shzxlz.cn

PHP:  exit(1);
来源：http://zsr.yongpay.top

JS:   process.exit(1)
来源：http://plq.xuanzx.com

TS:   process.exit(1)
来源：http://mql.shanyushiyangtech.top

Java: System.exit(1)
来源：http://emn.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://eml.dashuyun.cn

Ruby: exit 1
来源：http://kyk.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ges.hywenlv.cn

[M06] 向标准错误输出
来源：http://ktj.shanyushiyangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://qbs.zycfv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dhj.hfpthk.cn

JS:   console.error("err")
来源：http://rlr.gzhubu.top

TS:   console.error("err")
来源：http://cfj.hesvh.cn

Java: System.err.println("err")
来源：http://nwb.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mnw.jlsjyb.cn

Ruby: warn "err"
来源：http://hoc.ywan-chungtsiang.top

C#:   Console.Error.WriteLine("err")
来源：http://lsg.gotoacloud.top

[M07] 判断是否为主入口
来源：http://mvi.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://hyc.9152youxi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mqj.xingfuxueyuan.xyz

JS:   require.main === module
来源：http://mtd.ehwqpu.com

TS:   require.main === module
来源：http://fpm.shanyushiyangtech.top


<!-- 参考信息 -->