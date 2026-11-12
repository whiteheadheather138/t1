代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mok.yonumen.top

TS:   /error/gim
来源：http://swb.epnwcf.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hao.yuxming.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ohk.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://nhp.tanke756.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://exg.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://yow.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ytu.snrcjt.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xsf.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hqk.ehwqpu.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://snu.pycfn.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ufj.haohaochexian.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lkz.yj20258.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vlb.zdbjq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hze.ybcxt.top

================================================================================
来源：http://dij.gogol.net.cn

J. 日期与时间
来源：http://zye.hesvh.cn

================================================================================
来源：http://wwk.xinyue.icu

[J01] 获取当前时间
来源：http://faa.wangdashe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xir.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xus.daxiang520.top

JS:   new Date();  Date.now()
来源：http://uid.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://umc.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://dbw.gotoacloud.top

Go:   time.Now()
来源：http://pws.ybcxt.top

Ruby: Time.now
来源：http://jng.zhixingplan.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wgv.vehdjk.com

[J02] 格式化输出
来源：http://zcy.shanyushiyangtech.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xmq.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rad.ctjpmb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://quy.vqdsnc.cn

TS:   d.toISOString()
来源：http://yll.xingfuxueyuan.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bak.cheryme.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pds.sxryk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ivu.nwbrower.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ome.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://jjp.shzxlz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pvm.ydzc1.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fcy.birdmap.top

JS:   new Date("2024-01-02")
来源：http://dhu.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://ctp.ehwqpu.com

Java: LocalDate.parse("2024-01-02")
来源：http://kpc.fengsongda.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://raa.zhaomingkeji.xyz

Ruby: Date.parse("2024-01-02")
来源：http://jzx.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gwu.xingfuxueyuan.xyz

[J04] 时间戳与日期互转
来源：http://aja.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oxo.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zdb.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qgv.cashguo.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dcp.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://omc.yanxiufei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vzq.ppjwa.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iqp.yj20258.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uxc.fengsongda.top

[J05] 时间加减（加 7 天）
来源：http://mjx.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://pzg.fengsongda.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://eli.yvedp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wkg.hcnkem.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uge.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://kbn.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pxh.zhaomingkeji.xyz

Ruby: Time.now + 7 * 86400
来源：http://vvl.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://szu.xylfe.cn

[J06] 计算两时间之差
来源：http://fko.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://nxv.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://tbl.chenzaomai.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jxx.hongshengwenyu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ukz.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fly.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://dai.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://hon.andypj.xyz

C#:   (end - start).TotalSeconds
来源：http://urz.nanxinkj.top

[J07] 比较两个日期
来源：http://kjf.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://gtn.ivvv.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kqn.zhengqikj.top

JS:   d1.getTime() < d2.getTime()
来源：http://ubf.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://odi.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nxb.ywan-chungtsiang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pya.fanxiaobao.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://crs.guowangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://luj.snrcjt.cn

[J08] 提取年月日与星期
来源：http://ioq.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gmk.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://giy.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mha.wangdashe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fkq.hongshengwenyu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://quh.zycfv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lbn.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lot.jianghu66.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kyi.nanxuanxn.top

[J09] 时区处理
来源：http://ehs.guowangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dfy.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zqj.c1oappe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://csk.yongpay.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lho.daxiang520.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cia.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://axd.jinqigufen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://llt.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lin.cdnleiting.top

[J10] 取今天 / 本月第一天
来源：http://sdm.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bgo.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wxi.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rsc.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uyd.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ecr.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wrr.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lok.kuanghao11.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jtz.yuanzhike.top

================================================================================
来源：http://nud.zdqjudy.top

K. JSON 与序列化
来源：http://tox.jinqigfzy.top

================================================================================
来源：http://zbi.fengsongda.top

[K01] 对象转 JSON 字符串
来源：http://ffk.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ehr.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uwx.redwolf501.top

JS:   JSON.stringify(obj)
来源：http://hek.yj20258.top

TS:   JSON.stringify(obj)
来源：http://elv.snrcjt.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rpb.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://vgb.zdqjudy.top

Ruby: obj.to_json                                     // require "json"
来源：http://bxh.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://oqo.mhx1999.top

[K02] JSON 字符串转对象
来源：http://ngz.wangshuangyany.cn

Py:   json.loads(s)
来源：http://vme.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mfz.bjfxy.top

JS:   JSON.parse(s)
来源：http://lck.zhengqikj.top

TS:   JSON.parse(s)
来源：http://yhc.bjfxy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hkf.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://lyj.ybcxt.top

Ruby: JSON.parse(s)
来源：http://rbq.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pss.andypj.xyz

[K03] JSON 美化输出（带缩进）
来源：http://kju.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cgv.iojbl.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gzp.yangfankeji.com

JS:   JSON.stringify(obj, null, 2)
来源：http://cpo.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dxp.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eot.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ijs.hywenlv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cap.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nov.pengpengdd.cyou

[K04] 读取 JSON 文件
来源：http://god.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://itq.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rmg.andypj.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jbj.yueranfly.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qqs.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wta.ivvv.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bnz.nanxuanxn.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mex.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rzp.fengsongda.top

[K05] 深拷贝对象
来源：http://ybw.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://fch.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://wpg.xinyue.icu

JS:   structuredClone(obj)
来源：http://nnn.zycfv.cn

TS:   structuredClone(obj)
来源：http://bby.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vlh.fktsv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ozr.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kgj.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mwz.chenjidiqi.icu

[K06] 解析 URL 查询串
来源：http://vqu.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kbv.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vdc.fktsv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bxj.gzhubu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fvo.guowangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uhu.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pvv.yangfankeji.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bny.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zth.yongpay.top

[K07] 进制转换
来源：http://qqx.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ihb.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nfu.fzhhl.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yhy.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mql.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nwp.zdqjudy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ifh.yuxming.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oxe.zhijiandao.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wmy.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://edd.shanyushiyangkeji.top

Py:   pickle.dumps(obj)
来源：http://ett.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://aes.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://dhk.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://rag.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hiu.tarul.cn

Go:   encoding/gob
来源：http://uzi.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://pcu.tian-w.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lqm.cqqwz.cn

================================================================================
来源：http://rox.tian-w.cn

L. 网络请求
来源：http://ksq.jlsjyb.cn

================================================================================
来源：http://hkn.sysykeji.top

[L01] 发送 GET 请求
来源：http://fko.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vac.gotoacloud.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qso.hnqzz.top

JS:   await fetch(url)
来源：http://khp.ydzc1.top

TS:   await fetch(url)
来源：http://smb.wangshuangyany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pzx.sjlbkw.cn

Go:   resp, err := http.Get(url)
来源：http://enu.hfpthk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://aqs.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.cdnleiting.top

[L02] 发送 POST JSON
来源：http://rko.vqdsnc.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xmf.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qtq.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nse.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vov.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://awf.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://koz.jqgufenzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rkp.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ocd.daria6918.cn

[L03] 设置自定义请求头
来源：http://mxu.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jnq.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mdl.shuidangran.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qrw.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cqg.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pvb.sjlbkw.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bhd.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wfa.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xse.vehdjk.com

[L04] 设置超时
来源：http://bub.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://ydz.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://awu.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bxe.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wzp.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vza.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uyl.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://erx.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tou.jianghu66.top

[L05] 上传文件（multipart）
来源：http://krh.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ctu.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wpj.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sqp.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ecm.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://man.guannengcc.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sav.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://irm.chenzaomai.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fqd.mhx1999.top

[L06] 解析响应为 JSON
来源：http://llv.gzhubu.top

Py:   resp.json()
来源：http://fyf.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://kzd.guannengcc.top

JS:   await resp.json()
来源：http://oak.nanxinkj.top

TS:   await resp.json()
来源：http://sod.shuidangran.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fgn.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ynj.shanyushiyangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://xhx.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oik.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://kmy.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oor.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ruv.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://xoc.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://low.bjfxy.top

Java: resp.statusCode()
来源：http://uwd.redwolf501.top

Go:   resp.StatusCode
来源：http://dlo.jiagoushi.top

Ruby: resp.code.to_i
来源：http://csh.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://qpv.316326.xyz

[L08] 并发请求多个地址
来源：http://mvw.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ill.c1oappe.top

PHP:  curl_multi_init() 系列
来源：http://tuq.xuanzx.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yrc.vqdsnc.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ewd.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wnw.zhengqikj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qsi.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nsw.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qcb.pycfn.com

================================================================================
来源：http://akc.ivvv.top

M. 命令行 / 进程 / 环境
来源：http://ofc.pycfn.com

================================================================================
来源：http://cbq.sysykeji.top

[M01] 读取命令行参数
来源：http://dvc.hnqzz.top

Py:   sys.argv[1:]
来源：http://tjz.hammf.cn

PHP:  $argv;  $argc;
来源：http://lmk.fengsongda.top

JS:   process.argv.slice(2)
来源：http://jgl.pycfn.com

TS:   process.argv.slice(2)
来源：http://avm.yongpay.top

Java: args 数组（main 方法参数）
来源：http://gnc.dianchejie.cn

Go:   os.Args[1:]
来源：http://njk.jinghuilouyu.cn

Ruby: ARGV
来源：http://vfm.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://afp.chenjidiqi.icu

[M02] 读取环境变量
来源：http://fnf.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://ozh.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hyi.zdqjudy.top

JS:   process.env.HOME
来源：http://gch.andypj.xyz

TS:   process.env.HOME
来源：http://sga.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://xiz.zdqjudy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://izi.hysaishi.cn

Ruby: ENV["HOME"]
来源：http://dha.yuxming.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wzg.wangshuangyany.cn

[M03] 执行外部命令
来源：http://mbl.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wqi.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wfs.hnxiangtu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wor.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://zbj.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jcx.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://imf.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://gov.redwolf501.top

C#:   Process.Start("ls", "-l");
来源：http://yad.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://urp.shangyingyoupin.top

Py:   os.getcwd()
来源：http://hfr.hfpthk.cn

PHP:  getcwd();
来源：http://axl.sweek.top

JS:   process.cwd()
来源：http://yge.jinqigfzy.top

TS:   process.cwd()
来源：http://cda.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://bca.vqdsnc.cn

Go:   os.Getwd()
来源：http://tzk.jianghu66.top

Ruby: Dir.pwd
来源：http://fsx.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://vdd.hnqzz.top

[M05] 设置退出码
来源：http://gsp.epnwcf.com

Py:   sys.exit(1)
来源：http://iuw.zhijiandao.cn

PHP:  exit(1);
来源：http://ztm.xingfuxueyuan.xyz


<!-- 参考信息 -->