代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ctz.andypj.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xey.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://scj.sweek.top

================================================================================
来源：http://uhp.ywan-chungtsiang.top

J. 日期与时间
来源：http://inj.andypj.xyz

================================================================================
来源：http://qmw.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://axt.guowangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dvm.cdnleiting.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fqe.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://pof.sysykeji.top

TS:   new Date();  Date.now()
来源：http://mve.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lrl.xuetiantiany.cn

Go:   time.Now()
来源：http://ebq.jqgfzy.top

Ruby: Time.now
来源：http://umd.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://csu.xinyue.icu

[J02] 格式化输出
来源：http://iky.yanxiufei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yzk.yanxiufei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fxy.meibo888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tkv.epnwcf.com

TS:   d.toISOString()
来源：http://htk.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lit.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qvj.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dae.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://off.sufxvd.cn

[J03] 字符串解析为日期
来源：http://kkg.fehbvm.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bkn.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iue.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://kdh.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://dtp.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://idq.wangdashe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bcb.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://ocw.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lmq.fzhhl.top

[J04] 时间戳与日期互转
来源：http://rod.jinyuanbaomall.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rxr.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qjy.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ylh.jyoumei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://she.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zlv.yvedp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jfm.xuanzx.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jzq.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xre.bjfxy.top

[J05] 时间加减（加 7 天）
来源：http://emr.cdnleiting.top

Py:   now + timedelta(days=7)
来源：http://pjt.cqqwz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lcy.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ruj.cdnleiting.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rzi.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://vvu.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pmd.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://yhv.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://xtp.daria6918.cn

[J06] 计算两时间之差
来源：http://gwh.nwbrower.top

Py:   (end - start).total_seconds()
来源：http://lvn.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://tbv.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tde.tarul.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qug.tianlin.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://fax.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://rmn.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://lar.cashguo.top

C#:   (end - start).TotalSeconds
来源：http://yqo.ybcxt.top

[J07] 比较两个日期
来源：http://vwi.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://xby.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fjm.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://buz.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://wms.tarul.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cmy.jyoumei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pqh.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://bgd.birdmap.top

C#:   d1 < d2;  d1 == d2
来源：http://mpd.sjlbkw.cn

[J08] 提取年月日与星期
来源：http://rco.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oqp.c1oappe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xts.aibaodan.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rna.yvedp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bwl.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pom.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bpk.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nzj.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hzn.guowangkeji.top

[J09] 时区处理
来源：http://vam.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lfq.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://djy.sysykeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cus.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qrp.hfpthk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ddd.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gyo.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mha.andypj.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://irz.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://age.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cyf.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://atz.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gnj.sxryk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://omo.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nsy.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vxd.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vjy.svipenyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ftr.tianlin.xyz

================================================================================
来源：http://dzt.yanxiufei.cn

K. JSON 与序列化
来源：http://voq.fengsongda.top

================================================================================
来源：http://uwp.chenjidiqi.icu

[K01] 对象转 JSON 字符串
来源：http://gel.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://owf.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ikn.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://whg.zhoulong.xyz

TS:   JSON.stringify(obj)
来源：http://wlh.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dxe.guannengcc.top

Go:   json.Marshal(obj)
来源：http://euc.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://psx.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oom.ybcxt.top

[K02] JSON 字符串转对象
来源：http://xyg.cdnleiting.top

Py:   json.loads(s)
来源：http://iio.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xky.fktsv.cn

JS:   JSON.parse(s)
来源：http://prm.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://hsk.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tvi.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://yyd.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://uoq.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://epb.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://uld.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ssm.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lcl.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://iyp.gzhubu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xjm.zhengqikj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qwq.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sua.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ecr.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bck.shzxlz.cn

[K04] 读取 JSON 文件
来源：http://eob.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lwo.sufxvd.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yuq.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xsb.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rbs.quarkkingdee.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://twa.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jqq.hcnkem.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ank.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qni.ydzc1.top

[K05] 深拷贝对象
来源：http://kcg.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://mcv.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://wbo.chenzaomai.com

JS:   structuredClone(obj)
来源：http://bzt.cucudq.cn

TS:   structuredClone(obj)
来源：http://ihg.fengsongda.top

Java: // 手写拷贝构造，或序列化往返
来源：http://eay.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wut.haohaochexian.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wjg.yj202588.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ido.gaohongyu789.top

[K06] 解析 URL 查询串
来源：http://frw.hysaishi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wyk.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pxj.quarkkingdee.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lsr.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kyo.fzhhl.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ygg.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vvi.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kfz.hammf.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bjq.hysaishi.cn

[K07] 进制转换
来源：http://vqg.havefunace.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://huw.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ywm.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://thz.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pgq.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ssp.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tpc.vehdjk.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sen.ywan-chungtsiang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://waq.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://zrk.yvedp.cn

Py:   pickle.dumps(obj)
来源：http://vuc.hcnkem.com

PHP:  serialize($obj);  unserialize($s);
来源：http://eng.xziqi.cn

JS:   v8.serialize(obj)        // Node
来源：http://mgc.sxryk.cn

TS:   v8.serialize(obj)        // Node
来源：http://lsc.fzhhl.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://urp.xuetiantiany.cn

Go:   encoding/gob
来源：http://vxq.zhixingplan.top

Ruby: Marshal.dump(obj)
来源：http://mxe.birdmap.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sbe.ppjwa.cn

================================================================================
来源：http://gme.gotoacloud.top

L. 网络请求
来源：http://rog.quarkkingdee.top

================================================================================
来源：http://gyz.feifeiyinyue.top

[L01] 发送 GET 请求
来源：http://vha.redwolf501.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gea.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://foa.hywenlv.cn

JS:   await fetch(url)
来源：http://vle.shanyushiyangkeji.top

TS:   await fetch(url)
来源：http://kch.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ugq.jyoumei.cn

Go:   resp, err := http.Get(url)
来源：http://yrk.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bxc.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ind.jianghu66.top

[L02] 发送 POST JSON
来源：http://iue.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://tco.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dho.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qgn.dashuyun.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://viv.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://czt.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fkp.xuanzx.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fgk.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dty.ywan-chungtsiang.top

[L03] 设置自定义请求头
来源：http://zhu.sjlbkw.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dfn.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ioa.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uxv.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dkw.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fzq.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://adw.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zuv.yvedp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sog.xuetiantiany.cn

[L04] 设置超时
来源：http://mjr.mhx1999.top

Py:   requests.get(url, timeout=5)
来源：http://vck.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hnk.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://har.haohaochexian.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ayo.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lbz.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zrm.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://byu.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://azh.tian-w.cn

[L05] 上传文件（multipart）
来源：http://jcu.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://awj.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://edz.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jdi.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rsg.svipenyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bhy.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ifz.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dys.hongshengwenyu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uey.hesvh.cn

[L06] 解析响应为 JSON
来源：http://zdt.shanyushiyangkeji.top

Py:   resp.json()
来源：http://dbw.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://zrm.jinqigfzy.top

JS:   await resp.json()
来源：http://bym.yj20258.top

TS:   await resp.json()
来源：http://hmc.havefunace.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gzb.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fhn.pengpengdd.cyou

Ruby: JSON.parse(resp.body)
来源：http://xbq.bbcook.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ues.chenjidiqi.icu

[L07] 处理 HTTP 状态码
来源：http://met.fehbvm.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ugl.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cxa.hysaishi.cn

JS:   resp.ok;  resp.status
来源：http://zcr.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://jzd.epnwcf.com

Java: resp.statusCode()
来源：http://gdf.0kj1m.cn

Go:   resp.StatusCode
来源：http://thw.yj202588.top

Ruby: resp.code.to_i
来源：http://pqv.yueranfly.top

C#:   (int)resp.StatusCode
来源：http://igb.haohaochexian.top

[L08] 并发请求多个地址
来源：http://rri.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wig.chenzaomai.com

PHP:  curl_multi_init() 系列
来源：http://yqx.daxiang520.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qfp.daria6918.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://usi.bjfxy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zfv.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gyn.zhoulong.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vof.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://esk.birdmap.top

================================================================================
来源：http://lpm.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://tga.hesvh.cn

================================================================================
来源：http://hif.uphjek.com

[M01] 读取命令行参数
来源：http://txo.zycfv.cn

Py:   sys.argv[1:]
来源：http://yiw.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://ida.cqqwz.cn

JS:   process.argv.slice(2)
来源：http://wjo.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://kub.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://cwk.yuxming.cn

Go:   os.Args[1:]
来源：http://ysr.vqdsnc.cn

Ruby: ARGV
来源：http://ztb.bbcook.cn

C#:   args 数组（Main 方法参数）
来源：http://azu.guannengcc.top

[M02] 读取环境变量
来源：http://jcf.zhixingplan.top

Py:   os.environ.get("HOME")
来源：http://pgr.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cix.havefunace.top

JS:   process.env.HOME
来源：http://unb.andypj.xyz

TS:   process.env.HOME
来源：http://nee.ybcxt.top

Java: System.getenv("HOME")
来源：http://gis.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nox.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://wbl.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fvr.fanxiaobao.xyz

[M03] 执行外部命令
来源：http://qvk.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ceb.hongshengwenyu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zoi.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yyr.yuanzhike.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hzn.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://htj.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ror.cdnleiting.top

Ruby: system("ls -l");  `ls -l`
来源：http://qin.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://qko.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://ped.jyoumei.cn

Py:   os.getcwd()
来源：http://xba.bjfxy.top

PHP:  getcwd();
来源：http://yin.ybcxt.top

JS:   process.cwd()
来源：http://jxj.cashguo.top

TS:   process.cwd()
来源：http://urh.cashguo.top

Java: Path.of("").toAbsolutePath()
来源：http://jtz.zhengqikj.top

Go:   os.Getwd()
来源：http://arw.jinqigufen.top

Ruby: Dir.pwd
来源：http://ccy.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://evu.c1oappe.top

[M05] 设置退出码
来源：http://ake.zhijiandao.cn

Py:   sys.exit(1)
来源：http://eip.yuxming.cn

PHP:  exit(1);
来源：http://tjo.tarul.cn

JS:   process.exit(1)
来源：http://ujc.jinqigufen.top

TS:   process.exit(1)
来源：http://hwu.nwbrower.top

Java: System.exit(1)
来源：http://ayc.xinyue.icu

Go:   os.Exit(1)
来源：http://teb.kuanghao11.cn

Ruby: exit 1
来源：http://lum.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rqw.xingfuxueyuan.xyz

[M06] 向标准错误输出
来源：http://kzp.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://wnh.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://kwd.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://dbw.jinqigufen.top

TS:   console.error("err")
来源：http://woq.xingfuxueyuan.xyz

Java: System.err.println("err")
来源：http://mbo.guannengcc.top


<!-- 参考信息 -->