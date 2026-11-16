代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fzf.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mug.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sea.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ubr.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kkj.meibo888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rbb.jinqigufen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iuj.yfazqb.com

================================================================================
来源：http://hxx.jinghuilouyu.cn

J. 日期与时间
来源：http://lef.cucudq.cn

================================================================================
来源：http://hkf.gogol.net.cn

[J01] 获取当前时间
来源：http://isq.shuidangran.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jcr.wangshuangyany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://icu.ppjwa.cn

JS:   new Date();  Date.now()
来源：http://wyl.chenzaomai.com

TS:   new Date();  Date.now()
来源：http://cta.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cwf.cheryme.top

Go:   time.Now()
来源：http://wka.zycfv.cn

Ruby: Time.now
来源：http://cys.yuanzhike.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xhq.pengpengdd.cyou

[J02] 格式化输出
来源：http://phv.yj20258888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jpu.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lvx.nanxinkj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dxj.xuanzx.com

TS:   d.toISOString()
来源：http://imn.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pxp.hnqzz.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://woq.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ptz.316326.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zcf.chenzaomai.com

[J03] 字符串解析为日期
来源：http://ysv.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lko.zhengqikj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dnc.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://enq.xuanzx.com

TS:   new Date("2024-01-02")
来源：http://hmb.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://noj.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cwu.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://col.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hfx.fehbvm.com

[J04] 时间戳与日期互转
来源：http://coz.daria6918.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eqf.tarul.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eom.chenlongwang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pei.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lhy.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oco.nanxinkj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ffl.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dds.jlsjyb.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qtb.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://uhm.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://dvr.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vem.gzhubu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ltx.yonumen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lls.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://cfi.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://krw.ppjwa.cn

Ruby: Time.now + 7 * 86400
来源：http://gyr.hysaishi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yyv.9152youxi.cn

[J06] 计算两时间之差
来源：http://zga.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://nyy.ydzc1.top

PHP:  $end->diff($start)->days;
来源：http://tgi.zhixingplan.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fch.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xrk.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://rep.iojbl.cn

Go:   end.Sub(start).Hours()
来源：http://doq.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://zto.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://kxr.yuxming.cn

[J07] 比较两个日期
来源：http://agl.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://kxc.haohaochexian.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hiw.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://azp.mhx1999.top

TS:   d1.getTime() < d2.getTime()
来源：http://hty.hywenlv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://joq.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ogf.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://ffh.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://jwt.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://bio.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://syo.ybcxt.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yog.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ikt.sjlbkw.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kqh.zhoulong.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hsv.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cnt.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hlv.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lem.yueranfly.top

[J09] 时区处理
来源：http://fqr.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lpv.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://akl.zhengqikj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uii.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qge.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eeh.ctjpmb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yfy.epnwcf.com

Ruby: Time.now.getlocal("+08:00")
来源：http://xxo.ywan-chungtsiang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://stq.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://eos.jqgfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://req.redwolf501.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://slm.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://odk.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gts.yongpay.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://leg.fktsv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dia.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xat.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lzy.zdqjudy.top

================================================================================
来源：http://gfy.zhengqikj.top

K. JSON 与序列化
来源：http://ynh.haohaochexian.top

================================================================================
来源：http://kpn.xylfe.cn

[K01] 对象转 JSON 字符串
来源：http://bnt.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://des.ydzc1.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zae.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://cpw.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://rvc.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wll.shanyushiyangkeji.top

Go:   json.Marshal(obj)
来源：http://wvi.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nhi.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://etu.52xcode.cn

[K02] JSON 字符串转对象
来源：http://mjp.nwbrower.top

Py:   json.loads(s)
来源：http://fli.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vbv.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://pks.pycfn.com

TS:   JSON.parse(s)
来源：http://auv.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hap.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://rop.ybcxt.top

Ruby: JSON.parse(s)
来源：http://oih.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eji.tanke756.top

[K03] JSON 美化输出（带缩进）
来源：http://qpm.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://are.yj20258888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rqc.shanyushiyangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xdw.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wcx.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://brs.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hjf.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://ywt.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dmt.haohaochexian.top

[K04] 读取 JSON 文件
来源：http://wja.hammf.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ecj.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cjx.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bkw.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jwk.nanxinkj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jdy.tanke756.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vkt.kuanghao11.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cym.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zlh.yuanzhike.top

[K05] 深拷贝对象
来源：http://goa.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://qbn.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://ljg.yongpay.top

JS:   structuredClone(obj)
来源：http://jou.gzhubu.top

TS:   structuredClone(obj)
来源：http://fjz.fzhhl.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ztn.zhijiandao.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hle.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://has.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://fvw.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://kkm.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hei.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yav.sxryk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pwb.zhoulong.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cjd.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nsb.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://apj.jinghuilouyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pvl.hongshengwenyu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rou.quarkkingdee.top

[K07] 进制转换
来源：http://qaj.jqgfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tht.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wal.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wzq.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ari.pycfn.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gvy.hcnkem.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jyf.havefunace.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hhz.yfazqb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kjc.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://rbt.sweek.top

Py:   pickle.dumps(obj)
来源：http://zqg.nanxuanxn.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lqe.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://tcy.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://xfr.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xjy.epnwcf.com

Go:   encoding/gob
来源：http://koh.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://yap.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://elu.shanyushiyangkeji.top

================================================================================
来源：http://dkm.ywan-chungtsiang.top

L. 网络请求
来源：http://krn.fehbvm.com

================================================================================
来源：http://qyc.sxryk.cn

[L01] 发送 GET 请求
来源：http://mya.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bhs.jqgufenzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rmu.wangdashe.top

JS:   await fetch(url)
来源：http://emk.zhoulong.xyz

TS:   await fetch(url)
来源：http://eri.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ntc.svipenyu.cn

Go:   resp, err := http.Get(url)
来源：http://des.yvedp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jyq.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gkv.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://meb.svipenyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wyt.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bys.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rjd.shanyushiyangtech.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dxq.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vnb.cqqwz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vbu.meibo888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://imt.fengsongda.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zdn.zhongyouzk.top

[L03] 设置自定义请求头
来源：http://joq.zhaomingkeji.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fkt.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jtw.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vou.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dqm.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rap.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wxn.dianchejie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gti.zdbjq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zrm.hnxiangtu.top

[L04] 设置超时
来源：http://kwi.nwbrower.top

Py:   requests.get(url, timeout=5)
来源：http://cwr.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://spu.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qto.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cyz.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rrj.havefunace.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jng.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hnz.yueranfly.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eld.redwolf501.top

[L05] 上传文件（multipart）
来源：http://nqg.aizwys.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rih.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://svr.sysykeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tll.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vdu.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rdl.chenlongwang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cea.ywan-chungtsiang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gnf.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kjw.sxryk.cn

[L06] 解析响应为 JSON
来源：http://gjm.nwbrower.top

Py:   resp.json()
来源：http://ybz.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://pca.yuxming.cn

JS:   await resp.json()
来源：http://xxo.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://ers.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://stc.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bdi.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://sts.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gkv.chenjidiqi.icu

[L07] 处理 HTTP 状态码
来源：http://akc.yj20258.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lfm.yanxiufei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nnz.cheryme.top

JS:   resp.ok;  resp.status
来源：http://lme.zdqjudy.top

TS:   resp.ok;  resp.status
来源：http://rgg.yj202588.top

Java: resp.statusCode()
来源：http://ffh.ybcxt.top

Go:   resp.StatusCode
来源：http://nun.gogol.net.cn

Ruby: resp.code.to_i
来源：http://hru.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://tnr.ehwqpu.com

[L08] 并发请求多个地址
来源：http://zfj.ybcxt.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lfm.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://pen.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gnq.fehbvm.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://als.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jnq.kuanghao11.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://opx.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qcl.fanxiaobao.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://htz.haohaochexian.top

================================================================================
来源：http://wnu.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://zqw.zhiwuduotai.top

================================================================================
来源：http://qjt.yanxiufei.cn

[M01] 读取命令行参数
来源：http://bbr.zhixingplan.top

Py:   sys.argv[1:]
来源：http://mdl.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://vki.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://ulm.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://xyt.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://vsc.zhoulong.xyz

Go:   os.Args[1:]
来源：http://fte.svipenyu.cn

Ruby: ARGV
来源：http://eqc.ywan-chungtsiang.top

C#:   args 数组（Main 方法参数）
来源：http://gcw.xylfe.cn

[M02] 读取环境变量
来源：http://jtc.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://yia.ppjwa.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zzt.iojbl.cn

JS:   process.env.HOME
来源：http://tjb.yongpay.top

TS:   process.env.HOME
来源：http://ndd.zdbjq.cn

Java: System.getenv("HOME")
来源：http://whr.xuetiantiany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://znl.zdqjudy.top

Ruby: ENV["HOME"]
来源：http://jcj.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://plh.quarkkingdee.top

[M03] 执行外部命令
来源：http://zfu.9152youxi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://irb.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zue.hywenlv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ycd.daria6918.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yll.9152youxi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cjv.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bqq.jqgufenzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://vtm.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://qrp.hongshengwenyu.top

[M04] 获取当前工作目录
来源：http://cxn.52xcode.cn

Py:   os.getcwd()
来源：http://wvv.yueranfly.top

PHP:  getcwd();
来源：http://ren.hesvh.cn

JS:   process.cwd()
来源：http://blp.vqdsnc.cn

TS:   process.cwd()
来源：http://vcq.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://klk.cashguo.top

Go:   os.Getwd()
来源：http://kpj.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://lhw.hywenlv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eqq.yueranfly.top

[M05] 设置退出码
来源：http://nbm.cqqwz.cn

Py:   sys.exit(1)
来源：http://ide.vqdsnc.cn

PHP:  exit(1);
来源：http://vqw.fehbvm.com

JS:   process.exit(1)
来源：http://mpx.yongpay.top

TS:   process.exit(1)
来源：http://olf.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://jsi.chenjidiqi.icu

Go:   os.Exit(1)
来源：http://cre.xingfuxueyuan.xyz

Ruby: exit 1
来源：http://eue.wangshuangyany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qms.xuanzx.com

[M06] 向标准错误输出
来源：http://qhi.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://muk.tianlin.xyz


<!-- 参考信息 -->