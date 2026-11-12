代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pwc.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wpx.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rfk.jinyuanbaomall.cn

================================================================================
来源：http://tnm.0kj1m.cn

J. 日期与时间
来源：http://bve.wangshuangyany.cn

================================================================================
来源：http://shf.ivvv.top

[J01] 获取当前时间
来源：http://qot.zhiwuduotai.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lcq.hesvh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pzw.cqqwz.cn

JS:   new Date();  Date.now()
来源：http://ucr.xuetiantiany.cn

TS:   new Date();  Date.now()
来源：http://mle.hesvh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jvi.andypj.xyz

Go:   time.Now()
来源：http://axy.xylfe.cn

Ruby: Time.now
来源：http://gqe.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iso.mhx1999.top

[J02] 格式化输出
来源：http://rpc.sufxvd.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pqu.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rar.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jfd.svipenyu.cn

TS:   d.toISOString()
来源：http://nli.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xkg.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nlf.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mcl.dianchejie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mqi.hcnkem.com

[J03] 字符串解析为日期
来源：http://rvm.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qtx.xingfuxueyuan.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lrx.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://icj.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://gtt.xuanzx.com

Java: LocalDate.parse("2024-01-02")
来源：http://ndi.yanxiufei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gya.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://qbx.c1oappe.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ldy.chenzaomai.com

[J04] 时间戳与日期互转
来源：http://ird.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://svs.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tcz.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ixu.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mwe.xingfuxueyuan.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://azh.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kdg.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://huh.hfpthk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rjz.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://wtd.wangshuangyany.cn

Py:   now + timedelta(days=7)
来源：http://dwq.zhiwuduotai.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dxt.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mkj.shanyushiyangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ncz.jinqigufen.top

Java: LocalDate.now().plusDays(7)
来源：http://cgh.fktsv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hgm.ehwqpu.com

Ruby: Time.now + 7 * 86400
来源：http://vvy.xingfuxueyuan.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://dgt.yueranfly.top

[J06] 计算两时间之差
来源：http://osj.xinyue.icu

Py:   (end - start).total_seconds()
来源：http://lbp.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://nxy.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pdv.sweek.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jts.ydjk.org.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nhr.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://dfb.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://sry.nanxinkj.top

C#:   (end - start).TotalSeconds
来源：http://yut.smart0.xyz

[J07] 比较两个日期
来源：http://rpy.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://kwn.52xcode.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tfw.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://ioq.chenjidiqi.icu

TS:   d1.getTime() < d2.getTime()
来源：http://gxs.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yeo.xuanzx.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rit.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://qwl.316326.xyz

C#:   d1 < d2;  d1 == d2
来源：http://bai.xziqi.cn

[J08] 提取年月日与星期
来源：http://bsj.zycfv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://puu.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pej.xuanzx.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zto.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yot.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://utd.snrcjt.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iak.vehdjk.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ygv.zhijiandao.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ead.svipenyu.cn

[J09] 时区处理
来源：http://yhk.jyoumei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://igd.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zpf.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jzo.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bul.sweek.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yyq.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qaq.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://fcg.jiagoushi.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lnf.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://ukn.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vxp.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gkb.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nwh.vqdsnc.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uei.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xio.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cww.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uaf.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mna.yuanzhike.top

================================================================================
来源：http://nfc.chenzaomai.com

K. JSON 与序列化
来源：http://kom.bbcook.cn

================================================================================
来源：http://cvy.yuanzhike.top

[K01] 对象转 JSON 字符串
来源：http://owh.hywenlv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://akq.redwolf501.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nuo.quarkkingdee.top

JS:   JSON.stringify(obj)
来源：http://igp.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://cgh.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jrt.wangshuangyany.cn

Go:   json.Marshal(obj)
来源：http://xsw.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://gep.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://crf.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://xtx.zhongyouzk.top

Py:   json.loads(s)
来源：http://lyg.fehbvm.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pyc.redwolf501.top

JS:   JSON.parse(s)
来源：http://gxo.xuetiantiany.cn

TS:   JSON.parse(s)
来源：http://zdh.xuanzx.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yix.xuanzx.com

Go:   json.Unmarshal(data, &v)
来源：http://vlu.zdqjudy.top

Ruby: JSON.parse(s)
来源：http://bdm.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oyb.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://wpn.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dfa.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gal.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://izf.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jcu.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hbd.zdqjudy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zvq.shanyushiyangtech.top

Ruby: JSON.pretty_generate(obj)
来源：http://mzz.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zrm.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://ejm.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ywk.zhoulong.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hbr.cqqwz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vwh.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yeg.xingfuxueyuan.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://afx.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qdj.daxiang520.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yrh.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ggl.gaohongyu789.top

[K05] 深拷贝对象
来源：http://fsa.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://bix.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://ips.shanyushiyangtech.top

JS:   structuredClone(obj)
来源：http://bqo.mhx1999.top

TS:   structuredClone(obj)
来源：http://zxf.andypj.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://cxu.yangfankeji.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ors.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://msy.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dum.pengpengdd.cyou

[K06] 解析 URL 查询串
来源：http://ghy.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hwl.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://llg.xuetiantiany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ydi.nwbrower.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hwm.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fev.jinqigfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ccx.yuxming.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rcu.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bce.andypj.xyz

[K07] 进制转换
来源：http://goi.xuanzx.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yrt.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pim.daria6918.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ckg.zdbjq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zci.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lbp.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zhy.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://obr.shangyingyoupin.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sql.52xcode.cn

[K08] 二进制序列化（非 JSON）
来源：http://ebu.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://svb.gotoacloud.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nmo.yuanzhike.top

JS:   v8.serialize(obj)        // Node
来源：http://qsd.tanke756.top

TS:   v8.serialize(obj)        // Node
来源：http://bdd.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jfl.jinghuilouyu.cn

Go:   encoding/gob
来源：http://kbu.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://cur.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://duf.zdqjudy.top

================================================================================
来源：http://wzr.nanxinkj.top

L. 网络请求
来源：http://nlr.chenlongwang.top

================================================================================
来源：http://rll.ywan-chungtsiang.top

[L01] 发送 GET 请求
来源：http://yhv.nwbrower.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cfj.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sgw.xziqi.cn

JS:   await fetch(url)
来源：http://qwv.bbcook.cn

TS:   await fetch(url)
来源：http://qml.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nje.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://jud.daria6918.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kle.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cgq.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://kiv.chenlongwang.top

Py:   requests.post(url, json={"a": 1})
来源：http://hgi.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zqi.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pdv.xziqi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fmj.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pic.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nrd.shanyushiyangtech.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://brx.jiagoushi.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mlo.guannengcc.top

[L03] 设置自定义请求头
来源：http://ais.bbcook.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ywq.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rnv.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jks.chenjidiqi.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://acc.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ofh.fzhhl.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://azo.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mip.epnwcf.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gai.shanyushiyangkeji.top

[L04] 设置超时
来源：http://mga.hysaishi.cn

Py:   requests.get(url, timeout=5)
来源：http://rgz.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aom.zdqjudy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lgw.jiagoushi.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oym.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ysv.fanxiaobao.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hpc.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://knx.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tku.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://sez.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wlo.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fzc.xinyue.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gvq.meibo888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ala.wangshuangyany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ufx.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nrl.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ppk.ctjpmb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ryl.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://ohr.pycfn.com

Py:   resp.json()
来源：http://ykt.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://sgd.sufxvd.cn

JS:   await resp.json()
来源：http://pyf.jinqigufen.top

TS:   await resp.json()
来源：http://ifo.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eij.aizwys.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://drw.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://xty.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dnq.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://kme.hesvh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vmz.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dzk.daria6918.cn

JS:   resp.ok;  resp.status
来源：http://bob.zhixingplan.top

TS:   resp.ok;  resp.status
来源：http://ajy.hnxiangtu.top

Java: resp.statusCode()
来源：http://hni.hnxiangtu.top

Go:   resp.StatusCode
来源：http://vuy.shanyushiyangtech.top

Ruby: resp.code.to_i
来源：http://oev.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://uws.jqgfzy.top

[L08] 并发请求多个地址
来源：http://yhp.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://plq.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://vny.cqqwz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://der.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tkr.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yiw.vqdsnc.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ldb.nanxuanxn.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://unr.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xkh.wangdashe.top

================================================================================
来源：http://jhh.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://cyd.redwolf501.top

================================================================================
来源：http://kbw.zhoulong.xyz

[M01] 读取命令行参数
来源：http://kib.guannengcc.top

Py:   sys.argv[1:]
来源：http://bnu.zycfv.cn

PHP:  $argv;  $argc;
来源：http://enr.yj202588.top

JS:   process.argv.slice(2)
来源：http://pjf.xuetiantiany.cn

TS:   process.argv.slice(2)
来源：http://cbu.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://pao.hesvh.cn

Go:   os.Args[1:]
来源：http://ais.ybcxt.top

Ruby: ARGV
来源：http://cxp.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://skk.c1oappe.top

[M02] 读取环境变量
来源：http://lhx.sweek.top

Py:   os.environ.get("HOME")
来源：http://uta.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rae.hesvh.cn

JS:   process.env.HOME
来源：http://kyn.jlsjyb.cn

TS:   process.env.HOME
来源：http://hcq.tarul.cn

Java: System.getenv("HOME")
来源：http://rap.havefunace.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vmo.gaohongyu789.top

Ruby: ENV["HOME"]
来源：http://kte.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uqb.jyoumei.cn

[M03] 执行外部命令
来源：http://mnl.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://thj.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vnz.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://iea.hnqzz.top

TS:   child_process.execSync("ls -l").toString()
来源：http://sux.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lkk.jianghu66.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vsa.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pyn.hywenlv.cn

C#:   Process.Start("ls", "-l");
来源：http://dcj.cashguo.top

[M04] 获取当前工作目录
来源：http://zde.shanyushiyangtech.top

Py:   os.getcwd()
来源：http://pwc.shzxlz.cn

PHP:  getcwd();
来源：http://lps.dianchejie.cn

JS:   process.cwd()
来源：http://nks.daria6918.cn

TS:   process.cwd()
来源：http://rfm.ivvv.top

Java: Path.of("").toAbsolutePath()
来源：http://eds.yj202588.top

Go:   os.Getwd()
来源：http://wpj.zycfv.cn

Ruby: Dir.pwd
来源：http://fgk.xuanzx.com

C#:   Directory.GetCurrentDirectory()
来源：http://bbm.sysykeji.top

[M05] 设置退出码
来源：http://bzz.ywan-chungtsiang.top

Py:   sys.exit(1)
来源：http://lxl.yueranfly.top

PHP:  exit(1);
来源：http://jgq.zhiwuduotai.top

JS:   process.exit(1)
来源：http://tjp.zhiwuduotai.top

TS:   process.exit(1)
来源：http://xtk.tian-w.cn

Java: System.exit(1)
来源：http://ped.yuanzhike.top

Go:   os.Exit(1)
来源：http://ovc.wangshuangyany.cn

Ruby: exit 1
来源：http://rsy.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gct.fktsv.cn

[M06] 向标准错误输出
来源：http://ykv.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://ksb.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://khq.bjfxy.top

JS:   console.error("err")
来源：http://fgj.sxryk.cn

TS:   console.error("err")
来源：http://xiu.ehwqpu.com

Java: System.err.println("err")
来源：http://zwi.yanxiufei.cn


<!-- 参考信息 -->