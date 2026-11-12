代发 wailian999

Ruby: s.scan(/error/i)
来源：http://nog.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tmz.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://xir.yj20258.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jll.ywan-chungtsiang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kai.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rsx.quarkkingdee.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tdr.nwbrower.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rty.guowangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oes.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jzb.shuidangran.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://geh.yj202588.top

================================================================================
来源：http://yuv.9152youxi.cn

J. 日期与时间
来源：http://zxx.chenjidiqi.icu

================================================================================
来源：http://kty.wangdashe.top

[J01] 获取当前时间
来源：http://gjm.ctjpmb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://vrl.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iww.316326.xyz

JS:   new Date();  Date.now()
来源：http://cgd.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://kgh.vqdsnc.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fun.shuidangran.top

Go:   time.Now()
来源：http://ytu.zhijiandao.cn

Ruby: Time.now
来源：http://efs.cashguo.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kaq.svipenyu.cn

[J02] 格式化输出
来源：http://mxc.jinghuilouyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kzu.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pwp.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mgh.zdbjq.cn

TS:   d.toISOString()
来源：http://ijw.ywan-chungtsiang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nfj.zdbjq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xds.9152youxi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://szx.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rhx.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://xqx.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jfi.shanyushiyangtech.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yho.zycfv.cn

JS:   new Date("2024-01-02")
来源：http://lxv.pycfn.com

TS:   new Date("2024-01-02")
来源：http://nrh.cashguo.top

Java: LocalDate.parse("2024-01-02")
来源：http://rin.vqdsnc.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://toe.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://bti.ivvv.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dog.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://jps.jinyuanbaomall.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://crr.zhengqikj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dtm.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rdz.fktsv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jla.aibaodan.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yze.redwolf501.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vdo.chenjidiqi.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gjm.zhijiandao.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dqc.andypj.xyz

[J05] 时间加减（加 7 天）
来源：http://uae.jiagoushi.top

Py:   now + timedelta(days=7)
来源：http://vue.sxryk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kzk.zhijiandao.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://krx.9152youxi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ace.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://vsr.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uwf.xziqi.cn

Ruby: Time.now + 7 * 86400
来源：http://psv.xziqi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://omr.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://jfi.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://ztn.yueranfly.top

PHP:  $end->diff($start)->days;
来源：http://xpp.epnwcf.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ajv.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xnm.ybcxt.top

Java: Duration.between(start, end).toSeconds()
来源：http://oyr.pengpengdd.cyou

Go:   end.Sub(start).Hours()
来源：http://bos.chenjidiqi.icu

Ruby: end - start                 # 返回秒数
来源：http://ynr.hnqzz.top

C#:   (end - start).TotalSeconds
来源：http://kqy.tarul.cn

[J07] 比较两个日期
来源：http://psy.ywan-chungtsiang.top

Py:   d1 < d2;  d1 == d2
来源：http://gpu.dianchejie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kgx.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://kyp.uphjek.com

TS:   d1.getTime() < d2.getTime()
来源：http://hfi.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zff.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://liw.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://aqa.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://hbm.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://nuw.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kax.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fqf.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uvo.pengpengdd.cyou

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ebm.316326.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gaa.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dmk.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mry.ivvv.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bup.hfpthk.cn

[J09] 时区处理
来源：http://kav.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pwo.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nhr.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jta.yj20258888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xeu.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dqi.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://krg.ydzc1.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dza.jlsjyb.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vxz.yangfankeji.com

[J10] 取今天 / 本月第一天
来源：http://gaf.zhiwuduotai.top

Py:   date.today();  date.today().replace(day=1)
来源：http://obv.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lwe.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uno.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ein.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ogo.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mrr.guowangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tdy.tarul.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cfo.fehbvm.com

================================================================================
来源：http://fct.cqqwz.cn

K. JSON 与序列化
来源：http://psu.fanxiaobao.xyz

================================================================================
来源：http://nzw.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://uxk.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jrn.jyoumei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bvh.bbcook.cn

JS:   JSON.stringify(obj)
来源：http://jxc.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://fkp.shuidangran.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hot.cdnleiting.top

Go:   json.Marshal(obj)
来源：http://zpl.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://mbx.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://brv.yuanzhike.top

[K02] JSON 字符串转对象
来源：http://sum.epnwcf.com

Py:   json.loads(s)
来源：http://enz.jinqigufen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rvo.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://rhz.ivvv.top

TS:   JSON.parse(s)
来源：http://zct.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fvk.yueranfly.top

Go:   json.Unmarshal(data, &v)
来源：http://flr.xuetiantiany.cn

Ruby: JSON.parse(s)
来源：http://jxi.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://czg.snrcjt.cn

[K03] JSON 美化输出（带缩进）
来源：http://itr.jlsjyb.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://atz.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dpv.havefunace.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wdj.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://zvu.chenlongwang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dgi.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qij.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vuc.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ouz.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://wfa.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pvl.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yxk.jinghuilouyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iyo.hesvh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gih.sweek.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://thh.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tak.birdmap.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://obx.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uab.dianchejie.cn

[K05] 深拷贝对象
来源：http://gyd.vqdsnc.cn

Py:   copy.deepcopy(obj)
来源：http://fgf.yj202588.top

PHP:  unserialize(serialize($obj));
来源：http://iuz.iojbl.cn

JS:   structuredClone(obj)
来源：http://vfn.fengsongda.top

TS:   structuredClone(obj)
来源：http://swv.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wzs.dashuyun.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hnc.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://egl.cashguo.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nrf.cheryme.top

[K06] 解析 URL 查询串
来源：http://rbt.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zju.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mhw.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vpz.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xeg.zdbjq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://unv.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hwa.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vme.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pwv.pengpengdd.cyou

[K07] 进制转换
来源：http://kks.feifeiyinyue.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xgz.wangshuangyany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kvn.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mtb.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zbs.aizwys.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://czj.sxryk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wbo.snrcjt.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kkr.52xcode.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jql.zdqjudy.top

[K08] 二进制序列化（非 JSON）
来源：http://uqg.xuetiantiany.cn

Py:   pickle.dumps(obj)
来源：http://mlw.nanxuanxn.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xir.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://pzz.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://hxb.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hse.hammf.cn

Go:   encoding/gob
来源：http://jve.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://iqg.dashuyun.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://knt.sjlbkw.cn

================================================================================
来源：http://aem.nwbrower.top

L. 网络请求
来源：http://rxg.zhijiandao.cn

================================================================================
来源：http://yto.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://ajh.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ipa.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gbr.316326.xyz

JS:   await fetch(url)
来源：http://xwx.pengpengdd.cyou

TS:   await fetch(url)
来源：http://lss.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ipq.pengpengdd.cyou

Go:   resp, err := http.Get(url)
来源：http://gna.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fcs.cucudq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lcw.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://onn.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xti.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lau.yj20258.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vhk.ppjwa.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gye.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tap.fehbvm.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ydd.sxryk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://una.zdbjq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xae.chenlongwang.top

[L03] 设置自定义请求头
来源：http://kvm.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ajk.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xkn.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://whv.sxryk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xsm.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ocu.nanxinkj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zrk.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lbu.ppjwa.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wox.tianlin.xyz

[L04] 设置超时
来源：http://xbp.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://vnr.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rpn.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://swl.hesvh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lnv.cashguo.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gxf.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sgg.tian-w.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xqv.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yfb.fktsv.cn

[L05] 上传文件（multipart）
来源：http://sia.yvedp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rjx.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fhc.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sgn.aizwys.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ygs.pengpengdd.cyou

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gdm.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vbp.jinqigufen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://txl.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xre.yvedp.cn

[L06] 解析响应为 JSON
来源：http://gko.bbcook.cn

Py:   resp.json()
来源：http://tnc.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://hjg.xylfe.cn

JS:   await resp.json()
来源：http://jvh.nanxuanxn.top

TS:   await resp.json()
来源：http://ttb.cdnleiting.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qmv.aibaodan.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lib.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://brl.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dvl.xinyue.icu

[L07] 处理 HTTP 状态码
来源：http://cfw.svipenyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ezv.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uto.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://yzj.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://utv.guowangkeji.top

Java: resp.statusCode()
来源：http://sdo.xylfe.cn

Go:   resp.StatusCode
来源：http://gwu.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://rcs.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://dts.dianchejie.cn

[L08] 并发请求多个地址
来源：http://xmi.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bii.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://hrw.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bkm.tarul.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tgd.shangyingyoupin.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ndb.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://but.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uxz.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ptb.cucudq.cn

================================================================================
来源：http://qyb.zdqjudy.top

M. 命令行 / 进程 / 环境
来源：http://krj.fktsv.cn

================================================================================
来源：http://inj.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://snc.tarul.cn

Py:   sys.argv[1:]
来源：http://iji.aizwys.cn

PHP:  $argv;  $argc;
来源：http://rko.zdqjudy.top

JS:   process.argv.slice(2)
来源：http://qtc.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://kpp.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://waq.zhixingplan.top

Go:   os.Args[1:]
来源：http://sko.gaohongyu789.top

Ruby: ARGV
来源：http://rwj.zycfv.cn

C#:   args 数组（Main 方法参数）
来源：http://urt.yangfankeji.com

[M02] 读取环境变量
来源：http://cbz.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://hze.hammf.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mxp.zhongyouzk.top

JS:   process.env.HOME
来源：http://cze.bjfxy.top

TS:   process.env.HOME
来源：http://kjp.sjlbkw.cn

Java: System.getenv("HOME")
来源：http://tna.nanxinkj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oij.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://svn.sweek.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://llx.jqgfzy.top

[M03] 执行外部命令
来源：http://nkw.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gyf.pengpengdd.cyou

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fld.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hig.zhoulong.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://rjl.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kbo.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zic.nanxinkj.top

Ruby: system("ls -l");  `ls -l`
来源：http://rqm.xylfe.cn

C#:   Process.Start("ls", "-l");
来源：http://jzy.cdnleiting.top

[M04] 获取当前工作目录
来源：http://rkq.chenjidiqi.icu

Py:   os.getcwd()
来源：http://put.daxiang520.top

PHP:  getcwd();
来源：http://bdm.jyoumei.cn

JS:   process.cwd()
来源：http://tqe.hesvh.cn

TS:   process.cwd()
来源：http://jik.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://sjc.zhiwuduotai.top

Go:   os.Getwd()
来源：http://kny.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://cgh.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cuf.gotoacloud.top

[M05] 设置退出码
来源：http://aka.xingfuxueyuan.xyz

Py:   sys.exit(1)
来源：http://utb.cashguo.top

PHP:  exit(1);
来源：http://ugo.zhaomingkeji.xyz

JS:   process.exit(1)
来源：http://iis.ivvv.top

TS:   process.exit(1)
来源：http://qwf.c1oappe.top

Java: System.exit(1)
来源：http://sqd.chenjidiqi.icu

Go:   os.Exit(1)
来源：http://tro.yuxming.cn


<!-- 参考信息 -->