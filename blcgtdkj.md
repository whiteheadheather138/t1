代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://afu.jianghu66.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lqq.zdqjudy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lbn.xingfuxueyuan.xyz

================================================================================
来源：http://xqi.zdbjq.cn

J. 日期与时间
来源：http://xbc.xingfuxueyuan.xyz

================================================================================
来源：http://bnj.tarul.cn

[J01] 获取当前时间
来源：http://qcv.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sen.guannengcc.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wju.ivvv.top

JS:   new Date();  Date.now()
来源：http://moy.bjfxy.top

TS:   new Date();  Date.now()
来源：http://vay.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lqi.0kj1m.cn

Go:   time.Now()
来源：http://tuu.cheryme.top

Ruby: Time.now
来源：http://ksp.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rak.shzxlz.cn

[J02] 格式化输出
来源：http://afe.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wvu.xuetiantiany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tnl.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rza.xziqi.cn

TS:   d.toISOString()
来源：http://sib.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lsk.yuanzhike.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tls.hcnkem.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dau.tanke756.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hdx.yuxming.cn

[J03] 字符串解析为日期
来源：http://osk.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cea.cashguo.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qrh.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://myr.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://arz.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://qeo.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uqp.cheryme.top

Ruby: Date.parse("2024-01-02")
来源：http://fwg.jqgfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fxb.uphjek.com

[J04] 时间戳与日期互转
来源：http://mbg.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aqu.c1oappe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ova.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ayd.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://fxx.gaohongyu789.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nxt.mhx1999.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ckv.tian-w.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dxr.feifeiyinyue.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://luu.mhx1999.top

[J05] 时间加减（加 7 天）
来源：http://llv.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://adp.cqqwz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rhb.ydzc1.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nry.jinghuilouyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gqh.cashguo.top

Java: LocalDate.now().plusDays(7)
来源：http://nfn.jyoumei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://emt.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://tte.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://qqh.yuanzhike.top

[J06] 计算两时间之差
来源：http://jpq.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://pxo.yuanzhike.top

PHP:  $end->diff($start)->days;
来源：http://lqf.9152youxi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xsu.tianlin.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hil.nanxuanxn.top

Java: Duration.between(start, end).toSeconds()
来源：http://zfw.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://aye.ppjwa.cn

Ruby: end - start                 # 返回秒数
来源：http://xhl.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://jgc.zdqjudy.top

[J07] 比较两个日期
来源：http://tsf.hfpthk.cn

Py:   d1 < d2;  d1 == d2
来源：http://oim.quarkkingdee.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lkm.zhixingplan.top

JS:   d1.getTime() < d2.getTime()
来源：http://pfz.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://agd.jqgfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ffe.cheryme.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uzx.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://mdj.xuetiantiany.cn

C#:   d1 < d2;  d1 == d2
来源：http://mvu.shuidangran.top

[J08] 提取年月日与星期
来源：http://jpp.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ywy.gaohongyu789.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://arc.xuanzx.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bot.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ixv.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pge.chenlongwang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://huo.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rel.fktsv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://drt.shangyingyoupin.top

[J09] 时区处理
来源：http://fau.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pke.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hdt.hnqzz.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://brm.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kao.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jfw.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tao.gotoacloud.top

Ruby: Time.now.getlocal("+08:00")
来源：http://veb.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wwt.c1oappe.top

[J10] 取今天 / 本月第一天
来源：http://zhe.epnwcf.com

Py:   date.today();  date.today().replace(day=1)
来源：http://snn.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qlh.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ctw.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ndr.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://usx.epnwcf.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sow.yj202588.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pky.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qmw.zhengqikj.top

================================================================================
来源：http://yce.sysykeji.top

K. JSON 与序列化
来源：http://brx.yongpay.top

================================================================================
来源：http://boy.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://zuo.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cpq.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fwh.sufxvd.cn

JS:   JSON.stringify(obj)
来源：http://nhp.kuanghao11.cn

TS:   JSON.stringify(obj)
来源：http://iwo.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://brj.fengsongda.top

Go:   json.Marshal(obj)
来源：http://tyb.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nig.tarul.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://izd.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://qdf.tarul.cn

Py:   json.loads(s)
来源：http://umc.ppjwa.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kfk.fktsv.cn

JS:   JSON.parse(s)
来源：http://xra.c1oappe.top

TS:   JSON.parse(s)
来源：http://qiv.birdmap.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vwr.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://rzs.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://zaz.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vvp.ywan-chungtsiang.top

[K03] JSON 美化输出（带缩进）
来源：http://nnq.yj20258.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cxq.yonumen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xvl.aizwys.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nss.cucudq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wwy.ywan-chungtsiang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ate.316326.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zyt.hongshengwenyu.top

Ruby: JSON.pretty_generate(obj)
来源：http://ivu.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cqo.316326.xyz

[K04] 读取 JSON 文件
来源：http://wtv.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uio.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rxe.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rkb.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ngz.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gyd.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bmd.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://aeg.yongpay.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://juf.fzhhl.top

[K05] 深拷贝对象
来源：http://irh.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://vsy.nanxinkj.top

PHP:  unserialize(serialize($obj));
来源：http://rlm.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://hku.fktsv.cn

TS:   structuredClone(obj)
来源：http://ybo.vehdjk.com

Java: // 手写拷贝构造，或序列化往返
来源：http://rim.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wnw.sysykeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nnb.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ntl.smart0.xyz

[K06] 解析 URL 查询串
来源：http://xql.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lrh.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yze.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rqi.cheryme.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wel.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zyn.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rwp.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nop.hongshengwenyu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cnw.nwbrower.top

[K07] 进制转换
来源：http://sws.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ska.ydzc1.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hwv.wangshuangyany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tpv.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://shr.zdqjudy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://asz.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cye.zhongyouzk.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://btv.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jgy.birdmap.top

[K08] 二进制序列化（非 JSON）
来源：http://urd.yongpay.top

Py:   pickle.dumps(obj)
来源：http://ymi.feifeiyinyue.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mbp.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://iha.ctjpmb.com

TS:   v8.serialize(obj)        // Node
来源：http://roz.hcnkem.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uwn.sxryk.cn

Go:   encoding/gob
来源：http://wtt.jianghu66.top

Ruby: Marshal.dump(obj)
来源：http://emd.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yul.guannengcc.top

================================================================================
来源：http://ouw.gaohongyu789.top

L. 网络请求
来源：http://zeu.zhixingplan.top

================================================================================
来源：http://hze.jinqigufen.top

[L01] 发送 GET 请求
来源：http://ihv.andypj.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xjy.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ryt.hnqzz.top

JS:   await fetch(url)
来源：http://oto.bbcook.cn

TS:   await fetch(url)
来源：http://kmt.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gwl.svipenyu.cn

Go:   resp, err := http.Get(url)
来源：http://fdu.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://qhc.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nmg.jianghu66.top

[L02] 发送 POST JSON
来源：http://rnw.uphjek.com

Py:   requests.post(url, json={"a": 1})
来源：http://zyh.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kpl.yj20258.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ibq.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mnf.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://djf.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fak.cdnleiting.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tvg.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yza.shanyushiyangkeji.top

[L03] 设置自定义请求头
来源：http://dcm.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dhg.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://htp.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tjq.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nma.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://moa.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lon.andypj.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yci.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dnu.andypj.xyz

[L04] 设置超时
来源：http://rsn.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://wsm.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nup.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mnk.fktsv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zwp.yvedp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://usd.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pjm.svipenyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://teo.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jsk.zdbjq.cn

[L05] 上传文件（multipart）
来源：http://nlj.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tkj.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ycq.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ddj.zycfv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mls.hfpthk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eyr.smart0.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wmu.hammf.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kso.hnxiangtu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lxo.bbcook.cn

[L06] 解析响应为 JSON
来源：http://nzw.tian-w.cn

Py:   resp.json()
来源：http://dly.gzhubu.top

PHP:  json_decode($body, true);
来源：http://kpp.quarkkingdee.top

JS:   await resp.json()
来源：http://lug.cucudq.cn

TS:   await resp.json()
来源：http://iyu.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qaw.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pul.gzhubu.top

Ruby: JSON.parse(resp.body)
来源：http://wkc.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qiw.meibo888.top

[L07] 处理 HTTP 状态码
来源：http://qzb.jiagoushi.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yvl.chenlongwang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zbn.nanxuanxn.top

JS:   resp.ok;  resp.status
来源：http://akg.bjfxy.top

TS:   resp.ok;  resp.status
来源：http://djj.ivvv.top

Java: resp.statusCode()
来源：http://fpy.jinyuanbaomall.cn

Go:   resp.StatusCode
来源：http://ahi.daxiang520.top

Ruby: resp.code.to_i
来源：http://axf.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://dxw.sjlbkw.cn

[L08] 并发请求多个地址
来源：http://jwt.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qnc.xuetiantiany.cn

PHP:  curl_multi_init() 系列
来源：http://uyj.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zuf.hywenlv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xyf.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tou.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zeu.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ayn.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dto.mhx1999.top

================================================================================
来源：http://qsi.hongshengwenyu.top

M. 命令行 / 进程 / 环境
来源：http://cdd.quarkkingdee.top

================================================================================
来源：http://pfl.snrcjt.cn

[M01] 读取命令行参数
来源：http://sac.havefunace.top

Py:   sys.argv[1:]
来源：http://tcj.hcnkem.com

PHP:  $argv;  $argc;
来源：http://vod.ywan-chungtsiang.top

JS:   process.argv.slice(2)
来源：http://tiz.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://stl.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://rbi.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://byd.cheryme.top

Ruby: ARGV
来源：http://tnn.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://jjl.yfazqb.com

[M02] 读取环境变量
来源：http://kmd.andypj.xyz

Py:   os.environ.get("HOME")
来源：http://iuf.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kqn.ydjk.org.cn

JS:   process.env.HOME
来源：http://zei.zdbjq.cn

TS:   process.env.HOME
来源：http://tts.hcnkem.com

Java: System.getenv("HOME")
来源：http://iee.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iee.zhongyouzk.top

Ruby: ENV["HOME"]
来源：http://iqz.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xvm.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://aed.wangshuangyany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nwz.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qpa.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tgf.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ihd.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vwk.xuanzx.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ujd.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zde.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://qri.shanyushiyangkeji.top

[M04] 获取当前工作目录
来源：http://qux.bjfxy.top

Py:   os.getcwd()
来源：http://kai.hesvh.cn

PHP:  getcwd();
来源：http://okz.epnwcf.com

JS:   process.cwd()
来源：http://gpg.jinyuanbaomall.cn

TS:   process.cwd()
来源：http://foc.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://ujn.yj202588.top

Go:   os.Getwd()
来源：http://stv.hywenlv.cn

Ruby: Dir.pwd
来源：http://cyc.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://rsf.guowangkeji.top

[M05] 设置退出码
来源：http://qwk.zhijiandao.cn

Py:   sys.exit(1)
来源：http://vwr.yj202588.top

PHP:  exit(1);
来源：http://akl.cucudq.cn

JS:   process.exit(1)
来源：http://anr.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://pfu.jiagoushi.top

Java: System.exit(1)
来源：http://bda.ivvv.top

Go:   os.Exit(1)
来源：http://sjg.9152youxi.cn

Ruby: exit 1
来源：http://daj.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://utn.snrcjt.cn

[M06] 向标准错误输出
来源：http://jfq.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://wjx.chenzaomai.com

PHP:  fwrite(STDERR, "err\n");
来源：http://oeu.gaohongyu789.top

JS:   console.error("err")
来源：http://wjf.havefunace.top

TS:   console.error("err")
来源：http://iab.cashguo.top

Java: System.err.println("err")
来源：http://tdw.cucudq.cn


<!-- 参考信息 -->