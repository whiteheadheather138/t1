代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dvr.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yqi.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jxa.daxiang520.top

================================================================================
来源：http://bdw.sjlbkw.cn

J. 日期与时间
来源：http://kqu.fehbvm.com

================================================================================
来源：http://ute.jqgfzy.top

[J01] 获取当前时间
来源：http://zih.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cng.sweek.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://drj.xinyue.icu

JS:   new Date();  Date.now()
来源：http://ltp.meibo888.top

TS:   new Date();  Date.now()
来源：http://txx.zhengqikj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://oye.ydzc1.top

Go:   time.Now()
来源：http://hse.xuetiantiany.cn

Ruby: Time.now
来源：http://kix.zdbjq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oix.gotoacloud.top

[J02] 格式化输出
来源：http://jyg.gzhubu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uez.zycfv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qzg.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vax.fktsv.cn

TS:   d.toISOString()
来源：http://vsg.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qcy.yj20258888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://voz.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lts.xinyue.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gyn.jinqigfzy.top

[J03] 字符串解析为日期
来源：http://swd.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zus.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gvy.zhoulong.xyz

JS:   new Date("2024-01-02")
来源：http://cky.quarkkingdee.top

TS:   new Date("2024-01-02")
来源：http://uxd.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://kbd.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xeg.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://mcs.cqqwz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qsv.c1oappe.top

[J04] 时间戳与日期互转
来源：http://sld.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tvi.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lcv.52xcode.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qxj.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qsy.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://otm.sjlbkw.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hzj.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cez.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ayp.sweek.top

[J05] 时间加减（加 7 天）
来源：http://qlm.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://gvr.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jpm.zhongyouzk.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://amp.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lzb.daria6918.cn

Java: LocalDate.now().plusDays(7)
来源：http://aar.wangdashe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lgu.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://xpc.hysaishi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://umw.c1oappe.top

[J06] 计算两时间之差
来源：http://jro.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://cdk.zhixingplan.top

PHP:  $end->diff($start)->days;
来源：http://jkk.svipenyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zkn.hysaishi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hrl.shangyingyoupin.top

Java: Duration.between(start, end).toSeconds()
来源：http://yfp.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://bdy.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://mzp.jinqigfzy.top

C#:   (end - start).TotalSeconds
来源：http://uih.chenlongwang.top

[J07] 比较两个日期
来源：http://xwu.hnxiangtu.top

Py:   d1 < d2;  d1 == d2
来源：http://qvw.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pvk.316326.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://ajy.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://gmb.fengsongda.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ddt.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fmk.havefunace.top

Ruby: d1 < d2;  d1 == d2
来源：http://yta.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://xil.hfpthk.cn

[J08] 提取年月日与星期
来源：http://sde.hfpthk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://chx.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oow.shzxlz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://byo.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tbu.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://akh.zhiwuduotai.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nha.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dic.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dnd.hysaishi.cn

[J09] 时区处理
来源：http://zpd.cqqwz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zjm.0kj1m.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xhq.jinghuilouyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nym.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://itg.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rft.pycfn.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cot.xziqi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pov.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://klh.jiagoushi.top

[J10] 取今天 / 本月第一天
来源：http://vrc.zhengqikj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bwu.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rme.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mtl.zhongyouzk.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eog.chenlongwang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tdr.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tkq.yuxming.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bst.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tep.sweek.top

================================================================================
来源：http://fzq.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://bun.fengsongda.top

================================================================================
来源：http://uhd.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://qrf.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lhk.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://amy.zhoulong.xyz

JS:   JSON.stringify(obj)
来源：http://lxk.jqgufenzy.top

TS:   JSON.stringify(obj)
来源：http://bqr.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://joh.chenzaomai.com

Go:   json.Marshal(obj)
来源：http://ugh.quarkkingdee.top

Ruby: obj.to_json                                     // require "json"
来源：http://yva.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yyv.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://zxm.tarul.cn

Py:   json.loads(s)
来源：http://tgp.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ush.andypj.xyz

JS:   JSON.parse(s)
来源：http://slt.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://iit.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ctg.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://jlg.redwolf501.top

Ruby: JSON.parse(s)
来源：http://jbe.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qoj.snrcjt.cn

[K03] JSON 美化输出（带缩进）
来源：http://xcs.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sib.iojbl.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mcd.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dis.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://air.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rnz.shangyingyoupin.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wjw.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://vra.snrcjt.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ixf.zdbjq.cn

[K04] 读取 JSON 文件
来源：http://isq.feifeiyinyue.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aey.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lsx.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://his.hnxiangtu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://emf.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aiy.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qil.jlsjyb.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://auw.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yay.yueranfly.top

[K05] 深拷贝对象
来源：http://vyp.yongpay.top

Py:   copy.deepcopy(obj)
来源：http://wvl.svipenyu.cn

PHP:  unserialize(serialize($obj));
来源：http://juv.yonumen.top

JS:   structuredClone(obj)
来源：http://azg.mhx1999.top

TS:   structuredClone(obj)
来源：http://ksv.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qtl.tarul.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lwc.wangdashe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sif.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jmd.xylfe.cn

[K06] 解析 URL 查询串
来源：http://qkr.vqdsnc.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://riu.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wav.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yfv.gaohongyu789.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xxw.chenlongwang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://voq.pengpengdd.cyou

Go:   url.ParseQuery("a=1&b=2")
来源：http://eaw.cheryme.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fys.dashuyun.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pqv.havefunace.top

[K07] 进制转换
来源：http://xkn.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mlp.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ipb.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fkm.bbcook.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gbj.hongshengwenyu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hdm.hcnkem.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bcc.9152youxi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://spo.ydjk.org.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aue.cucudq.cn

[K08] 二进制序列化（非 JSON）
来源：http://iik.aizwys.cn

Py:   pickle.dumps(obj)
来源：http://qui.bbcook.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hwn.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://ovy.haohaochexian.top

TS:   v8.serialize(obj)        // Node
来源：http://nut.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kba.kuanghao11.cn

Go:   encoding/gob
来源：http://cye.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://dvs.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kfc.pengpengdd.cyou

================================================================================
来源：http://bqk.yvedp.cn

L. 网络请求
来源：http://abj.uphjek.com

================================================================================
来源：http://hed.cheryme.top

[L01] 发送 GET 请求
来源：http://lwr.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rtl.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hvj.hongshengwenyu.top

JS:   await fetch(url)
来源：http://vcf.yongpay.top

TS:   await fetch(url)
来源：http://hux.zhaomingkeji.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://djz.jlsjyb.cn

Go:   resp, err := http.Get(url)
来源：http://gsi.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rhy.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eej.hcnkem.com

[L02] 发送 POST JSON
来源：http://wei.shangyingyoupin.top

Py:   requests.post(url, json={"a": 1})
来源：http://fmf.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rsj.9152youxi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wjc.chenlongwang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://epy.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://htr.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rro.jinyuanbaomall.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aqb.guannengcc.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xvg.cdnleiting.top

[L03] 设置自定义请求头
来源：http://loa.jinqigfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dwq.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cjj.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wfh.gzhubu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pbc.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uxr.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wna.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ver.cqqwz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tkh.sxryk.cn

[L04] 设置超时
来源：http://xmd.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://vjk.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gry.jinqigufen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hlk.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qjx.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tij.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wxt.9152youxi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lur.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zdy.nanxinkj.top

[L05] 上传文件（multipart）
来源：http://kht.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uqi.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fgx.yangfankeji.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ple.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mlq.ywan-chungtsiang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oru.gotoacloud.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uih.shzxlz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ebr.shanyushiyangtech.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rut.sxryk.cn

[L06] 解析响应为 JSON
来源：http://pcr.bbcook.cn

Py:   resp.json()
来源：http://wat.ivvv.top

PHP:  json_decode($body, true);
来源：http://jvd.snrcjt.cn

JS:   await resp.json()
来源：http://ghs.xingfuxueyuan.xyz

TS:   await resp.json()
来源：http://rtr.ctjpmb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ong.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bpc.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://tkq.wangdashe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vdm.zhoulong.xyz

[L07] 处理 HTTP 状态码
来源：http://dka.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ipw.guannengcc.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bwp.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://nmd.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://kut.andypj.xyz

Java: resp.statusCode()
来源：http://tcv.ybcxt.top

Go:   resp.StatusCode
来源：http://vcn.cdnleiting.top

Ruby: resp.code.to_i
来源：http://gjl.havefunace.top

C#:   (int)resp.StatusCode
来源：http://tgv.c1oappe.top

[L08] 并发请求多个地址
来源：http://ztu.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://omh.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://pgn.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bgp.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fjh.hammf.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gkh.fanxiaobao.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tes.yfazqb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://irc.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pkf.pycfn.com

================================================================================
来源：http://the.hnxiangtu.top

M. 命令行 / 进程 / 环境
来源：http://zvp.zhoulong.xyz

================================================================================
来源：http://xza.gaohongyu789.top

[M01] 读取命令行参数
来源：http://jqh.chenlongwang.top

Py:   sys.argv[1:]
来源：http://brk.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://ris.yj20258888.top

JS:   process.argv.slice(2)
来源：http://ztc.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://eew.zhengqikj.top

Java: args 数组（main 方法参数）
来源：http://wyi.yonumen.top

Go:   os.Args[1:]
来源：http://shw.shuidangran.top

Ruby: ARGV
来源：http://xpi.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://rgo.ybcxt.top

[M02] 读取环境变量
来源：http://sip.ivvv.top

Py:   os.environ.get("HOME")
来源：http://fal.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kxe.fengsongda.top

JS:   process.env.HOME
来源：http://nki.wangdashe.top

TS:   process.env.HOME
来源：http://sig.0kj1m.cn

Java: System.getenv("HOME")
来源：http://nyy.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ejn.birdmap.top

Ruby: ENV["HOME"]
来源：http://qpm.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vtf.gotoacloud.top

[M03] 执行外部命令
来源：http://rmz.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gis.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ygw.fktsv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gxc.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://uud.haohaochexian.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zbs.jinqigufen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pjv.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lhs.yongpay.top

C#:   Process.Start("ls", "-l");
来源：http://vwl.yongpay.top

[M04] 获取当前工作目录
来源：http://oig.tian-w.cn

Py:   os.getcwd()
来源：http://iqr.yanxiufei.cn

PHP:  getcwd();
来源：http://tbu.jqgfzy.top

JS:   process.cwd()
来源：http://ioj.yanxiufei.cn

TS:   process.cwd()
来源：http://utu.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://kvf.chenzaomai.com

Go:   os.Getwd()
来源：http://bmu.wangshuangyany.cn

Ruby: Dir.pwd
来源：http://eqi.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://byj.pycfn.com

[M05] 设置退出码
来源：http://wfc.hywenlv.cn

Py:   sys.exit(1)
来源：http://zbg.yangfankeji.com

PHP:  exit(1);
来源：http://evs.zdbjq.cn

JS:   process.exit(1)
来源：http://snp.9152youxi.cn

TS:   process.exit(1)
来源：http://jhu.yuanzhike.top

Java: System.exit(1)
来源：http://kbw.pycfn.com

Go:   os.Exit(1)
来源：http://vnk.daria6918.cn

Ruby: exit 1
来源：http://qus.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zav.yongpay.top

[M06] 向标准错误输出
来源：http://whe.nwbrower.top

Py:   print("err", file=sys.stderr)
来源：http://awn.aizwys.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://aoq.haohaochexian.top

JS:   console.error("err")
来源：http://hyq.pycfn.com

TS:   console.error("err")
来源：http://myl.chenjidiqi.icu

Java: System.err.println("err")
来源：http://oaw.jlsjyb.cn


<!-- 参考信息 -->