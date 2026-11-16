代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fwz.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xlg.ctjpmb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://toi.fehbvm.com

================================================================================
来源：http://git.yj202588.top

J. 日期与时间
来源：http://hcy.316326.xyz

================================================================================
来源：http://bis.hnxiangtu.top

[J01] 获取当前时间
来源：http://mif.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://vsk.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aey.daxiang520.top

JS:   new Date();  Date.now()
来源：http://mju.shanyushiyangtech.top

TS:   new Date();  Date.now()
来源：http://eem.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zum.andypj.xyz

Go:   time.Now()
来源：http://ufw.c1oappe.top

Ruby: Time.now
来源：http://ekh.yj20258.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fjk.zdqjudy.top

[J02] 格式化输出
来源：http://twd.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jop.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tke.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jzf.shanyushiyangkeji.top

TS:   d.toISOString()
来源：http://pnv.uphjek.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bsf.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xjb.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://czr.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wlx.xylfe.cn

[J03] 字符串解析为日期
来源：http://eev.epnwcf.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pet.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lgt.ydzc1.top

JS:   new Date("2024-01-02")
来源：http://tnq.wangshuangyany.cn

TS:   new Date("2024-01-02")
来源：http://ctd.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fax.jinqigufen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wfq.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://kzr.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nrs.tarul.cn

[J04] 时间戳与日期互转
来源：http://trx.birdmap.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lbi.dashuyun.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sqd.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sum.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cos.tian-w.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nfc.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lyi.bbcook.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ocm.nwbrower.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://emz.xuanzx.com

[J05] 时间加减（加 7 天）
来源：http://zxw.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://qzv.mhx1999.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://aex.tanke756.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lbj.9152youxi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dhc.snrcjt.cn

Java: LocalDate.now().plusDays(7)
来源：http://ubn.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bih.jinqigufen.top

Ruby: Time.now + 7 * 86400
来源：http://oov.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://pni.havefunace.top

[J06] 计算两时间之差
来源：http://utd.zhoulong.xyz

Py:   (end - start).total_seconds()
来源：http://dkz.zdqjudy.top

PHP:  $end->diff($start)->days;
来源：http://uhk.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lda.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jze.yonumen.top

Java: Duration.between(start, end).toSeconds()
来源：http://luj.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://ecg.snrcjt.cn

Ruby: end - start                 # 返回秒数
来源：http://wfx.yuxming.cn

C#:   (end - start).TotalSeconds
来源：http://wjl.pycfn.com

[J07] 比较两个日期
来源：http://xxl.shzxlz.cn

Py:   d1 < d2;  d1 == d2
来源：http://reg.zhengqikj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uqu.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://alm.tanke756.top

TS:   d1.getTime() < d2.getTime()
来源：http://wiv.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hfo.hcnkem.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://seb.pengpengdd.cyou

Ruby: d1 < d2;  d1 == d2
来源：http://ywc.hcnkem.com

C#:   d1 < d2;  d1 == d2
来源：http://hao.tianlin.xyz

[J08] 提取年月日与星期
来源：http://ied.cqqwz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bbx.xylfe.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kng.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jjg.shzxlz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rpb.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iak.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mgj.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wls.sweek.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tqk.smart0.xyz

[J09] 时区处理
来源：http://xvy.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zmz.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kur.fktsv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jko.jqgfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nuu.ctjpmb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jjl.havefunace.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vub.yuxming.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tcj.chenzaomai.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jjc.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://tvq.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wiz.ywan-chungtsiang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cxm.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bvb.52xcode.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hvg.0kj1m.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dad.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ips.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xnm.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gay.yuxming.cn

================================================================================
来源：http://bnn.hfpthk.cn

K. JSON 与序列化
来源：http://yvt.iojbl.cn

================================================================================
来源：http://adc.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://qnx.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://itp.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hpg.tarul.cn

JS:   JSON.stringify(obj)
来源：http://stf.zhiwuduotai.top

TS:   JSON.stringify(obj)
来源：http://wag.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mdl.chenjidiqi.icu

Go:   json.Marshal(obj)
来源：http://jwh.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://cyf.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lpa.snrcjt.cn

[K02] JSON 字符串转对象
来源：http://msx.yj20258888.top

Py:   json.loads(s)
来源：http://kep.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://snv.dianchejie.cn

JS:   JSON.parse(s)
来源：http://ros.chenzaomai.com

TS:   JSON.parse(s)
来源：http://vtw.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nfh.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://mjg.yvedp.cn

Ruby: JSON.parse(s)
来源：http://piw.yonumen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iww.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://ild.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gaz.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mef.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zor.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jyx.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yqf.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zpt.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://mqi.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://npx.cucudq.cn

[K04] 读取 JSON 文件
来源：http://uxr.gotoacloud.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yry.shanyushiyangtech.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xrt.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://icd.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qmo.shanyushiyangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hxz.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pip.iojbl.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rxi.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fpw.ppjwa.cn

[K05] 深拷贝对象
来源：http://lhc.ppjwa.cn

Py:   copy.deepcopy(obj)
来源：http://suf.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://ygt.xylfe.cn

JS:   structuredClone(obj)
来源：http://rbo.cqqwz.cn

TS:   structuredClone(obj)
来源：http://svb.fengsongda.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ybv.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yfo.andypj.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nao.sysykeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mzc.dashuyun.cn

[K06] 解析 URL 查询串
来源：http://xhd.jianghu66.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dld.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gog.sjlbkw.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://amk.cheryme.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ust.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lhp.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dan.fehbvm.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://plx.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sug.jinyuanbaomall.cn

[K07] 进制转换
来源：http://iyd.daria6918.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uky.hywenlv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://grh.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jrd.fktsv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vvm.chenlongwang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fuc.xinyue.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jnx.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://isw.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tvx.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://gbb.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://voq.ywan-chungtsiang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lsx.xziqi.cn

JS:   v8.serialize(obj)        // Node
来源：http://fyf.cqqwz.cn

TS:   v8.serialize(obj)        // Node
来源：http://cjj.feifeiyinyue.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nws.cashguo.top

Go:   encoding/gob
来源：http://wfp.fengsongda.top

Ruby: Marshal.dump(obj)
来源：http://ljq.sweek.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jof.jqgufenzy.top

================================================================================
来源：http://qpg.tarul.cn

L. 网络请求
来源：http://qbv.hongshengwenyu.top

================================================================================
来源：http://bmq.jinyuanbaomall.cn

[L01] 发送 GET 请求
来源：http://nil.vqdsnc.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wet.quarkkingdee.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yyy.fehbvm.com

JS:   await fetch(url)
来源：http://iuy.316326.xyz

TS:   await fetch(url)
来源：http://pop.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tcx.zhixingplan.top

Go:   resp, err := http.Get(url)
来源：http://umr.fanxiaobao.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://cxq.fanxiaobao.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://npn.jinghuilouyu.cn

[L02] 发送 POST JSON
来源：http://ehj.smart0.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://yri.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tls.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nck.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bcu.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://epi.yanxiufei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vkw.316326.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://opy.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xlf.xylfe.cn

[L03] 设置自定义请求头
来源：http://kdm.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ppo.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://imr.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hce.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zuf.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hyz.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tse.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pjl.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vih.snrcjt.cn

[L04] 设置超时
来源：http://ktk.hammf.cn

Py:   requests.get(url, timeout=5)
来源：http://gbu.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ipk.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bjp.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fky.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vuz.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bjk.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iso.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rkb.jyoumei.cn

[L05] 上传文件（multipart）
来源：http://ikh.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iyv.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dye.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ubr.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://knf.xuetiantiany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sxm.mhx1999.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rii.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kuw.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lwc.yj20258.top

[L06] 解析响应为 JSON
来源：http://hcp.zhijiandao.cn

Py:   resp.json()
来源：http://mhj.havefunace.top

PHP:  json_decode($body, true);
来源：http://qro.pengpengdd.cyou

JS:   await resp.json()
来源：http://jzc.daxiang520.top

TS:   await resp.json()
来源：http://bwi.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jtn.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ebk.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://jjm.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://emk.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://jku.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cin.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kfe.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://ari.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://hjp.sjlbkw.cn

Java: resp.statusCode()
来源：http://vtd.52xcode.cn

Go:   resp.StatusCode
来源：http://qro.daria6918.cn

Ruby: resp.code.to_i
来源：http://mtf.snrcjt.cn

C#:   (int)resp.StatusCode
来源：http://yqk.shzxlz.cn

[L08] 并发请求多个地址
来源：http://bim.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://opi.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://czy.smart0.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cfx.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zbn.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fto.haohaochexian.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mbv.ybcxt.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nzf.zhixingplan.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qsh.ydjk.org.cn

================================================================================
来源：http://obd.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://ldw.bjfxy.top

================================================================================
来源：http://yxa.bjfxy.top

[M01] 读取命令行参数
来源：http://pgf.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://mfq.chenlongwang.top

PHP:  $argv;  $argc;
来源：http://bse.ydzc1.top

JS:   process.argv.slice(2)
来源：http://oaa.gogol.net.cn

TS:   process.argv.slice(2)
来源：http://pgg.shuidangran.top

Java: args 数组（main 方法参数）
来源：http://eyf.chenlongwang.top

Go:   os.Args[1:]
来源：http://qdn.xinyue.icu

Ruby: ARGV
来源：http://pdw.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://ozf.zhijiandao.cn

[M02] 读取环境变量
来源：http://lwn.yueranfly.top

Py:   os.environ.get("HOME")
来源：http://voh.jianghu66.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://leu.gaohongyu789.top

JS:   process.env.HOME
来源：http://ufb.jiagoushi.top

TS:   process.env.HOME
来源：http://iul.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://ttp.ctjpmb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://liq.vehdjk.com

Ruby: ENV["HOME"]
来源：http://pbg.xylfe.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fms.daria6918.cn

[M03] 执行外部命令
来源：http://uic.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fqi.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iiu.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://teg.zhaomingkeji.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://ult.cucudq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kda.xuetiantiany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ywi.jiagoushi.top

Ruby: system("ls -l");  `ls -l`
来源：http://xfg.zhaomingkeji.xyz

C#:   Process.Start("ls", "-l");
来源：http://nor.xuanzx.com

[M04] 获取当前工作目录
来源：http://tpq.bjfxy.top

Py:   os.getcwd()
来源：http://xel.daria6918.cn

PHP:  getcwd();
来源：http://piz.xuanzx.com

JS:   process.cwd()
来源：http://kgx.jinyuanbaomall.cn

TS:   process.cwd()
来源：http://ass.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://mkx.tanke756.top

Go:   os.Getwd()
来源：http://wnt.fengsongda.top

Ruby: Dir.pwd
来源：http://nfj.vqdsnc.cn

C#:   Directory.GetCurrentDirectory()
来源：http://buq.sufxvd.cn

[M05] 设置退出码
来源：http://wjm.0kj1m.cn

Py:   sys.exit(1)
来源：http://qzq.c1oappe.top

PHP:  exit(1);
来源：http://bux.pengpengdd.cyou

JS:   process.exit(1)
来源：http://gcq.xziqi.cn

TS:   process.exit(1)
来源：http://vux.0kj1m.cn

Java: System.exit(1)
来源：http://wyd.xuanzx.com

Go:   os.Exit(1)
来源：http://rxq.daxiang520.top

Ruby: exit 1
来源：http://hlp.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dxw.pengpengdd.cyou

[M06] 向标准错误输出
来源：http://nbp.wangdashe.top

Py:   print("err", file=sys.stderr)
来源：http://qtx.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://joq.hfpthk.cn

JS:   console.error("err")
来源：http://twq.zhijiandao.cn

TS:   console.error("err")
来源：http://kfv.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://pvo.jqgufenzy.top


<!-- 参考信息 -->