代发 wailian999

Ruby: s.scan(/error/i)
来源：http://sxz.fzhhl.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wui.quarkkingdee.top

[I08] 贪婪与非贪婪匹配
来源：http://llg.guowangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iew.xziqi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ttm.gotoacloud.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tde.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dxu.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hup.jinqigufen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pox.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iwv.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jxo.pengpengdd.cyou

================================================================================
来源：http://juy.yvedp.cn

J. 日期与时间
来源：http://rvq.0kj1m.cn

================================================================================
来源：http://jjh.fzhhl.top

[J01] 获取当前时间
来源：http://heb.jinghuilouyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zdp.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tcc.316326.xyz

JS:   new Date();  Date.now()
来源：http://hmp.zhaomingkeji.xyz

TS:   new Date();  Date.now()
来源：http://hdh.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://nxs.jinqigufen.top

Go:   time.Now()
来源：http://qns.dashuyun.cn

Ruby: Time.now
来源：http://nic.yongpay.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ecn.zhongyouzk.top

[J02] 格式化输出
来源：http://ngd.sysykeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ryd.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kut.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oum.ehwqpu.com

TS:   d.toISOString()
来源：http://wij.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lnw.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ybb.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gae.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qmm.zdqjudy.top

[J03] 字符串解析为日期
来源：http://zpu.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ovg.xinyue.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hyg.yonumen.top

JS:   new Date("2024-01-02")
来源：http://oii.gzhubu.top

TS:   new Date("2024-01-02")
来源：http://uay.hongshengwenyu.top

Java: LocalDate.parse("2024-01-02")
来源：http://azr.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lzc.fengsongda.top

Ruby: Date.parse("2024-01-02")
来源：http://hpm.yanxiufei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://asj.fehbvm.com

[J04] 时间戳与日期互转
来源：http://tmt.nanxinkj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jhb.havefunace.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sjv.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bgk.zycfv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jqf.cdnleiting.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fnm.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zph.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vaf.jlsjyb.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wnk.yvedp.cn

[J05] 时间加减（加 7 天）
来源：http://kuv.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://qzn.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://uaw.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jnn.hcnkem.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tbh.daria6918.cn

Java: LocalDate.now().plusDays(7)
来源：http://nks.zhiwuduotai.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lgu.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://qnf.ehwqpu.com

C#:   DateTime.Now.AddDays(7)
来源：http://jny.yangfankeji.com

[J06] 计算两时间之差
来源：http://pmf.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://wpc.mhx1999.top

PHP:  $end->diff($start)->days;
来源：http://mjn.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vci.cashguo.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pjc.cheryme.top

Java: Duration.between(start, end).toSeconds()
来源：http://zeo.fanxiaobao.xyz

Go:   end.Sub(start).Hours()
来源：http://cdv.shangyingyoupin.top

Ruby: end - start                 # 返回秒数
来源：http://vqn.yueranfly.top

C#:   (end - start).TotalSeconds
来源：http://vkg.zhixingplan.top

[J07] 比较两个日期
来源：http://mgw.shangyingyoupin.top

Py:   d1 < d2;  d1 == d2
来源：http://des.xuetiantiany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wmr.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://xfj.jinyuanbaomall.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vbn.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ifc.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://etv.shzxlz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pid.hnqzz.top

C#:   d1 < d2;  d1 == d2
来源：http://vve.hnqzz.top

[J08] 提取年月日与星期
来源：http://tqc.ywan-chungtsiang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pld.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dah.tianlin.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tlb.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tdx.shuidangran.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ttp.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://usc.yanxiufei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wub.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vvn.smart0.xyz

[J09] 时区处理
来源：http://ltu.andypj.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fln.jlsjyb.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ccw.wangdashe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tsv.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nka.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://are.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yxh.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xpo.gogol.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mke.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://rxm.ppjwa.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://suf.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ccw.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zff.jyoumei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zpj.jinghuilouyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ghd.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dbq.jinqigfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://puy.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ngj.xuetiantiany.cn

================================================================================
来源：http://sqi.kuanghao11.cn

K. JSON 与序列化
来源：http://fbq.yj202588.top

================================================================================
来源：http://dpg.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://qgv.uphjek.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oqo.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iqg.sysykeji.top

JS:   JSON.stringify(obj)
来源：http://vdv.ywan-chungtsiang.top

TS:   JSON.stringify(obj)
来源：http://etb.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qii.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://cfa.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://caz.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj)
来源：http://iju.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://vlj.bjfxy.top

Py:   json.loads(s)
来源：http://utu.gotoacloud.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qde.zdqjudy.top

JS:   JSON.parse(s)
来源：http://bnh.ehwqpu.com

TS:   JSON.parse(s)
来源：http://sro.wangshuangyany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://urx.fzhhl.top

Go:   json.Unmarshal(data, &v)
来源：http://hgs.shangyingyoupin.top

Ruby: JSON.parse(s)
来源：http://ico.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hgk.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://hmr.vqdsnc.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://udk.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jcx.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sdx.fzhhl.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ibo.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mbv.zdqjudy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xom.birdmap.top

Ruby: JSON.pretty_generate(obj)
来源：http://vhb.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zjj.haohaochexian.top

[K04] 读取 JSON 文件
来源：http://zcc.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jyw.pycfn.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kck.andypj.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ews.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fbb.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://csp.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wna.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qss.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eff.yuanzhike.top

[K05] 深拷贝对象
来源：http://onq.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://kst.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://pxp.mhx1999.top

JS:   structuredClone(obj)
来源：http://msa.yvedp.cn

TS:   structuredClone(obj)
来源：http://ngb.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://txp.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sjs.jianghu66.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lke.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yup.yfazqb.com

[K06] 解析 URL 查询串
来源：http://gla.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nez.yvedp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jgi.daxiang520.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gri.nanxinkj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gzu.ctjpmb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pod.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://apy.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hyw.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vva.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://cjf.chenjidiqi.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hul.shanyushiyangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wct.hnxiangtu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uok.vqdsnc.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uyr.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fgo.yanxiufei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://czy.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uor.yangfankeji.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tho.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://tis.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://scc.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ikm.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://wob.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://lvc.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ixq.bjfxy.top

Go:   encoding/gob
来源：http://yyt.guowangkeji.top

Ruby: Marshal.dump(obj)
来源：http://ujw.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kjl.bjfxy.top

================================================================================
来源：http://twp.mhx1999.top

L. 网络请求
来源：http://uzs.yanxiufei.cn

================================================================================
来源：http://pqy.xuanzx.com

[L01] 发送 GET 请求
来源：http://ume.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zxy.316326.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sxo.zhongyouzk.top

JS:   await fetch(url)
来源：http://xfv.uphjek.com

TS:   await fetch(url)
来源：http://phg.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qfr.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://lbn.ydjk.org.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gcs.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jcy.gzhubu.top

[L02] 发送 POST JSON
来源：http://vlm.zhiwuduotai.top

Py:   requests.post(url, json={"a": 1})
来源：http://zvw.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zxl.redwolf501.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aoq.fengsongda.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xph.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cun.jianghu66.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pds.sjlbkw.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ixz.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rtn.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://whq.vqdsnc.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tpc.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tln.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tfs.cashguo.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eqo.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zvg.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://utw.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wvu.epnwcf.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yqf.316326.xyz

[L04] 设置超时
来源：http://plf.yuxming.cn

Py:   requests.get(url, timeout=5)
来源：http://fep.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vtt.0kj1m.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://trw.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vpr.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mga.yfazqb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yzk.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iiu.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fex.wangdashe.top

[L05] 上传文件（multipart）
来源：http://ewc.chenzaomai.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qef.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xgk.tian-w.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jdo.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lxs.tarul.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://str.sufxvd.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qqg.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://idv.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qre.yongpay.top

[L06] 解析响应为 JSON
来源：http://jwj.hesvh.cn

Py:   resp.json()
来源：http://jfg.jqgfzy.top

PHP:  json_decode($body, true);
来源：http://rcg.316326.xyz

JS:   await resp.json()
来源：http://hmt.jianghu66.top

TS:   await resp.json()
来源：http://uun.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ghv.ppjwa.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bmg.yueranfly.top

Ruby: JSON.parse(resp.body)
来源：http://jcx.nanxuanxn.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xue.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://twt.hongshengwenyu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wzm.aizwys.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yzi.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://iaa.jqgufenzy.top

TS:   resp.ok;  resp.status
来源：http://qay.smart0.xyz

Java: resp.statusCode()
来源：http://rwr.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://ezr.ydzc1.top

Ruby: resp.code.to_i
来源：http://pti.xuetiantiany.cn

C#:   (int)resp.StatusCode
来源：http://hxo.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://ipa.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zwx.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://fjw.xingfuxueyuan.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jqt.hnqzz.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tak.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zqy.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://grl.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ttl.zhixingplan.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://abb.tanke756.top

================================================================================
来源：http://iwa.pycfn.com

M. 命令行 / 进程 / 环境
来源：http://obw.fengsongda.top

================================================================================
来源：http://ikx.zhixingplan.top

[M01] 读取命令行参数
来源：http://gzz.wangdashe.top

Py:   sys.argv[1:]
来源：http://ejf.jianghu66.top

PHP:  $argv;  $argc;
来源：http://dxx.daria6918.cn

JS:   process.argv.slice(2)
来源：http://nqw.cheryme.top

TS:   process.argv.slice(2)
来源：http://ssi.hnxiangtu.top

Java: args 数组（main 方法参数）
来源：http://cgw.aizwys.cn

Go:   os.Args[1:]
来源：http://osg.yueranfly.top

Ruby: ARGV
来源：http://beo.haohaochexian.top

C#:   args 数组（Main 方法参数）
来源：http://cbh.zhoulong.xyz

[M02] 读取环境变量
来源：http://nvq.cashguo.top

Py:   os.environ.get("HOME")
来源：http://nyp.zhongyouzk.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cxe.redwolf501.top

JS:   process.env.HOME
来源：http://dgx.xziqi.cn

TS:   process.env.HOME
来源：http://ohb.c1oappe.top

Java: System.getenv("HOME")
来源：http://rsb.yvedp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://smy.yfazqb.com

Ruby: ENV["HOME"]
来源：http://cra.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://npv.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://xxs.guowangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://try.ivvv.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ejj.0kj1m.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vxq.nwbrower.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hmg.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jwk.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fqz.ywan-chungtsiang.top

Ruby: system("ls -l");  `ls -l`
来源：http://hro.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://hgn.jyoumei.cn

[M04] 获取当前工作目录
来源：http://mcg.hongshengwenyu.top

Py:   os.getcwd()
来源：http://lqj.tian-w.cn

PHP:  getcwd();
来源：http://hup.yuxming.cn

JS:   process.cwd()
来源：http://gos.sjlbkw.cn

TS:   process.cwd()
来源：http://bum.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://xfi.jqgfzy.top

Go:   os.Getwd()
来源：http://qku.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://rnn.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://klw.chenzaomai.com

[M05] 设置退出码
来源：http://awi.chenlongwang.top

Py:   sys.exit(1)
来源：http://gch.yanxiufei.cn

PHP:  exit(1);
来源：http://qjn.chenzaomai.com

JS:   process.exit(1)
来源：http://amd.yonumen.top

TS:   process.exit(1)
来源：http://skb.zhoulong.xyz

Java: System.exit(1)
来源：http://buo.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://eri.ctjpmb.com


<!-- 参考信息 -->