代发 wailian999

Ruby: s.scan(/error/i)
来源：http://fhi.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cbf.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://ooe.ydzc1.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qxt.zhijiandao.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ywk.redwolf501.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jle.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wxh.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ryx.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fzl.sysykeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cwq.0kj1m.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hnv.pycfn.com

================================================================================
来源：http://ylg.hysaishi.cn

J. 日期与时间
来源：http://mne.zdqjudy.top

================================================================================
来源：http://cei.zhengqikj.top

[J01] 获取当前时间
来源：http://vxs.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lrb.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ndm.hcnkem.com

JS:   new Date();  Date.now()
来源：http://ucg.zhengqikj.top

TS:   new Date();  Date.now()
来源：http://wvy.ydjk.org.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jke.0kj1m.cn

Go:   time.Now()
来源：http://vhk.jqgufenzy.top

Ruby: Time.now
来源：http://ncl.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nge.sysykeji.top

[J02] 格式化输出
来源：http://nup.gzhubu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uwo.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yrz.nanxuanxn.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ufs.cashguo.top

TS:   d.toISOString()
来源：http://dvy.bjfxy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fza.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pnm.jinghuilouyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eoa.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mie.sweek.top

[J03] 字符串解析为日期
来源：http://ykp.jqgufenzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tul.zhixingplan.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tmr.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://nof.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://kih.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://zzf.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uco.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://pdo.andypj.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nfu.nanxuanxn.top

[J04] 时间戳与日期互转
来源：http://dws.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pge.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kqb.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nvz.gotoacloud.top

TS:   Math.floor(Date.now() / 1000)
来源：http://sbn.zhaomingkeji.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://drg.fanxiaobao.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ugq.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pte.aibaodan.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wgc.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://njo.gotoacloud.top

Py:   now + timedelta(days=7)
来源：http://cwn.ydjk.org.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nfn.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pzy.316326.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://azf.fanxiaobao.xyz

Java: LocalDate.now().plusDays(7)
来源：http://kat.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gij.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://ytz.ivvv.top

C#:   DateTime.Now.AddDays(7)
来源：http://uvz.pengpengdd.cyou

[J06] 计算两时间之差
来源：http://rfu.zhaomingkeji.xyz

Py:   (end - start).total_seconds()
来源：http://bbj.yangfankeji.com

PHP:  $end->diff($start)->days;
来源：http://stq.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zrv.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bhp.yj202588.top

Java: Duration.between(start, end).toSeconds()
来源：http://aez.zdbjq.cn

Go:   end.Sub(start).Hours()
来源：http://oiw.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://tjg.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://ajj.nanxuanxn.top

[J07] 比较两个日期
来源：http://mvs.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://ovl.zdqjudy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sbg.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://llv.uphjek.com

TS:   d1.getTime() < d2.getTime()
来源：http://vyl.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uht.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ybl.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://biz.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://vzs.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://adk.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ekw.aibaodan.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ith.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fmw.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wzj.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mbt.shuidangran.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xeo.shuidangran.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ckq.epnwcf.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vdz.hammf.cn

[J09] 时区处理
来源：http://tna.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mvb.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tnc.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ccy.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uex.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vya.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://swh.xuanzx.com

Ruby: Time.now.getlocal("+08:00")
来源：http://vfn.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zqx.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://ztd.jinqigufen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xtn.yueranfly.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mmb.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mik.shzxlz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://psl.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ggm.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sqf.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dml.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qwi.tian-w.cn

================================================================================
来源：http://cqx.guowangkeji.top

K. JSON 与序列化
来源：http://ohb.fktsv.cn

================================================================================
来源：http://wlv.xziqi.cn

[K01] 对象转 JSON 字符串
来源：http://yyc.redwolf501.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yat.tarul.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mie.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://xyk.xingfuxueyuan.xyz

TS:   JSON.stringify(obj)
来源：http://wib.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oif.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://dof.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://dtt.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vgr.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://fcn.zhijiandao.cn

Py:   json.loads(s)
来源：http://awj.zhengqikj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ywj.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://xtw.snrcjt.cn

TS:   JSON.parse(s)
来源：http://ixs.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iux.yangfankeji.com

Go:   json.Unmarshal(data, &v)
来源：http://svy.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://goi.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nom.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://bik.yueranfly.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lmc.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nqo.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qst.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://xcj.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jzh.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tuv.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://ytg.ivvv.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qyb.shuidangran.top

[K04] 读取 JSON 文件
来源：http://mqb.tarul.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://scy.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rzq.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zso.yonumen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cid.jinqigufen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dae.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mgt.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://jdq.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bfy.xuanzx.com

[K05] 深拷贝对象
来源：http://ugd.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://kqe.yongpay.top

PHP:  unserialize(serialize($obj));
来源：http://bqi.chenlongwang.top

JS:   structuredClone(obj)
来源：http://zew.dashuyun.cn

TS:   structuredClone(obj)
来源：http://zya.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dfi.sysykeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qxo.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fib.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://zct.svipenyu.cn

[K06] 解析 URL 查询串
来源：http://ddr.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ujo.fanxiaobao.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vho.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nly.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dnb.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mtp.hongshengwenyu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lte.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fin.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xsf.9152youxi.cn

[K07] 进制转换
来源：http://yny.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cay.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ysc.guowangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jhb.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wqi.zdqjudy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bod.316326.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mgc.ppjwa.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eyp.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mgh.jianghu66.top

[K08] 二进制序列化（非 JSON）
来源：http://veu.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://drn.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nnf.gogol.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://nys.0kj1m.cn

TS:   v8.serialize(obj)        // Node
来源：http://boy.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fuv.zhongyouzk.top

Go:   encoding/gob
来源：http://hzh.epnwcf.com

Ruby: Marshal.dump(obj)
来源：http://prn.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zil.jianghu66.top

================================================================================
来源：http://ogs.yj20258888.top

L. 网络请求
来源：http://ytq.tian-w.cn

================================================================================
来源：http://ovq.bjfxy.top

[L01] 发送 GET 请求
来源：http://oza.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zet.jianghu66.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://efc.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://wcw.sjlbkw.cn

TS:   await fetch(url)
来源：http://qme.yuanzhike.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yrg.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://uij.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ukt.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ioz.daxiang520.top

[L02] 发送 POST JSON
来源：http://ulg.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://koh.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sdg.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://orm.fktsv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pei.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yyj.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ljp.quarkkingdee.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://afv.daxiang520.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cme.birdmap.top

[L03] 设置自定义请求头
来源：http://wre.guannengcc.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zjn.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bpf.nanxinkj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jrp.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cwn.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zck.xziqi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sik.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jst.redwolf501.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xio.aizwys.cn

[L04] 设置超时
来源：http://czw.fengsongda.top

Py:   requests.get(url, timeout=5)
来源：http://xrl.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pyo.hongshengwenyu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pbf.jinqigufen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://smi.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vuz.jinyuanbaomall.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xog.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://shv.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dgy.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://lfd.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://buk.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nzx.daria6918.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vsp.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qer.chenlongwang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://htl.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wnk.xuanzx.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jco.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mpq.aizwys.cn

[L06] 解析响应为 JSON
来源：http://bry.hywenlv.cn

Py:   resp.json()
来源：http://wpb.zhaomingkeji.xyz

PHP:  json_decode($body, true);
来源：http://ynq.52xcode.cn

JS:   await resp.json()
来源：http://gro.sysykeji.top

TS:   await resp.json()
来源：http://ang.smart0.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ypu.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xhm.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://zlc.dianchejie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zpi.fanxiaobao.xyz

[L07] 处理 HTTP 状态码
来源：http://ppv.zhoulong.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oyl.pycfn.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tqr.mhx1999.top

JS:   resp.ok;  resp.status
来源：http://ond.zhongyouzk.top

TS:   resp.ok;  resp.status
来源：http://xoi.jqgfzy.top

Java: resp.statusCode()
来源：http://hrc.daria6918.cn

Go:   resp.StatusCode
来源：http://ebq.jianghu66.top

Ruby: resp.code.to_i
来源：http://gdy.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://rvs.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://dpd.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://voo.tianlin.xyz

PHP:  curl_multi_init() 系列
来源：http://ptr.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ipx.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://huo.vqdsnc.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fvv.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://clr.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://prd.fanxiaobao.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://inp.birdmap.top

================================================================================
来源：http://vxy.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://mmx.pycfn.com

================================================================================
来源：http://lun.gaohongyu789.top

[M01] 读取命令行参数
来源：http://lze.gogol.net.cn

Py:   sys.argv[1:]
来源：http://aoy.gaohongyu789.top

PHP:  $argv;  $argc;
来源：http://dcr.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://mqz.ydjk.org.cn

TS:   process.argv.slice(2)
来源：http://dvz.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://ztv.fzhhl.top

Go:   os.Args[1:]
来源：http://mzs.gotoacloud.top

Ruby: ARGV
来源：http://xtq.wangshuangyany.cn

C#:   args 数组（Main 方法参数）
来源：http://rfq.daxiang520.top

[M02] 读取环境变量
来源：http://noo.zhixingplan.top

Py:   os.environ.get("HOME")
来源：http://zde.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aqw.shzxlz.cn

JS:   process.env.HOME
来源：http://drz.ybcxt.top

TS:   process.env.HOME
来源：http://pzl.xinyue.icu

Java: System.getenv("HOME")
来源：http://lst.smart0.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wye.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://qki.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ihb.sxryk.cn

[M03] 执行外部命令
来源：http://zmq.quarkkingdee.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zkp.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ycc.feifeiyinyue.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bfd.xuetiantiany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tnx.hesvh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vrx.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kuu.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ema.shuidangran.top

C#:   Process.Start("ls", "-l");
来源：http://rrp.0kj1m.cn

[M04] 获取当前工作目录
来源：http://spt.nwbrower.top

Py:   os.getcwd()
来源：http://wdq.tian-w.cn

PHP:  getcwd();
来源：http://stl.bbcook.cn

JS:   process.cwd()
来源：http://jmj.zdbjq.cn

TS:   process.cwd()
来源：http://sbw.iojbl.cn

Java: Path.of("").toAbsolutePath()
来源：http://fto.wangshuangyany.cn

Go:   os.Getwd()
来源：http://rhm.havefunace.top

Ruby: Dir.pwd
来源：http://pxb.hywenlv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qyb.guannengcc.top

[M05] 设置退出码
来源：http://ucy.zhixingplan.top

Py:   sys.exit(1)
来源：http://mgv.jqgufenzy.top

PHP:  exit(1);
来源：http://jew.chenjidiqi.icu

JS:   process.exit(1)
来源：http://hvt.jinghuilouyu.cn

TS:   process.exit(1)
来源：http://sfh.yangfankeji.com

Java: System.exit(1)
来源：http://pey.zhijiandao.cn

Go:   os.Exit(1)
来源：http://dfx.ehwqpu.com


<!-- 参考信息 -->