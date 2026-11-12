代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nje.ydzc1.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lkd.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zac.bjfxy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aic.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yow.cashguo.top

[I07] 忽略大小写与多行模式
来源：http://kzc.zhoulong.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cfo.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zln.zdqjudy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kaa.nanxinkj.top

TS:   /error/gim
来源：http://fcc.kuanghao11.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://etu.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://syr.daria6918.cn

Ruby: s.scan(/error/i)
来源：http://isc.zhongyouzk.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://imj.ehwqpu.com

[I08] 贪婪与非贪婪匹配
来源：http://qxa.yj20258888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blz.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://biz.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jii.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://trp.chenjidiqi.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://thq.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ehu.haohaochexian.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hho.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cva.hcnkem.com

================================================================================
来源：http://evy.zdbjq.cn

J. 日期与时间
来源：http://ooz.quarkkingdee.top

================================================================================
来源：http://arn.gaohongyu789.top

[J01] 获取当前时间
来源：http://laa.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jes.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cpv.yj20258.top

JS:   new Date();  Date.now()
来源：http://tov.tarul.cn

TS:   new Date();  Date.now()
来源：http://vba.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cjk.hnqzz.top

Go:   time.Now()
来源：http://cpz.daxiang520.top

Ruby: Time.now
来源：http://sut.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pmv.cqqwz.cn

[J02] 格式化输出
来源：http://gue.xuanzx.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://chd.shuidangran.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hzl.chenlongwang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bwn.zdbjq.cn

TS:   d.toISOString()
来源：http://riq.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vxs.zhijiandao.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xxd.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oej.cdnleiting.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fqz.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://fbz.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://erg.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xkk.yonumen.top

JS:   new Date("2024-01-02")
来源：http://psq.fanxiaobao.xyz

TS:   new Date("2024-01-02")
来源：http://jzw.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://rrm.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tet.andypj.xyz

Ruby: Date.parse("2024-01-02")
来源：http://qhc.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://igd.mhx1999.top

[J04] 时间戳与日期互转
来源：http://cxe.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bvh.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yxr.xinyue.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://knq.hcnkem.com

TS:   Math.floor(Date.now() / 1000)
来源：http://dml.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rni.gogol.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pyx.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kyf.redwolf501.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qwg.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://mvz.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://mtn.yuxming.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hyw.jqgufenzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rsf.cheryme.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://diu.haohaochexian.top

Java: LocalDate.now().plusDays(7)
来源：http://uey.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://knr.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://ksk.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://awn.fzhhl.top

[J06] 计算两时间之差
来源：http://hfl.pycfn.com

Py:   (end - start).total_seconds()
来源：http://flh.yanxiufei.cn

PHP:  $end->diff($start)->days;
来源：http://rbv.xylfe.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vqn.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jvu.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://vtr.c1oappe.top

Go:   end.Sub(start).Hours()
来源：http://ngd.redwolf501.top

Ruby: end - start                 # 返回秒数
来源：http://dhd.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://srm.yfazqb.com

[J07] 比较两个日期
来源：http://qqv.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://jim.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gbu.yvedp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gul.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://ork.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sxq.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://efn.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://dan.ydjk.org.cn

C#:   d1 < d2;  d1 == d2
来源：http://bsx.jlsjyb.cn

[J08] 提取年月日与星期
来源：http://cqg.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zhq.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hkr.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eir.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://had.nanxuanxn.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wnw.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hys.shanyushiyangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fiz.sufxvd.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://trs.xinyue.icu

[J09] 时区处理
来源：http://hsd.feifeiyinyue.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ufl.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zuh.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dur.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lmh.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://csg.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mgk.feifeiyinyue.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hzo.cdnleiting.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://irb.cdnleiting.top

[J10] 取今天 / 本月第一天
来源：http://ssi.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://stu.zhixingplan.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qlm.hnxiangtu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lzh.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pyf.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uck.zhengqikj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fwb.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yal.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dhu.sweek.top

================================================================================
来源：http://fkr.52xcode.cn

K. JSON 与序列化
来源：http://tjg.daria6918.cn

================================================================================
来源：http://svi.jqgufenzy.top

[K01] 对象转 JSON 字符串
来源：http://uew.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://swz.jinqigufen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://par.hnxiangtu.top

JS:   JSON.stringify(obj)
来源：http://siy.ehwqpu.com

TS:   JSON.stringify(obj)
来源：http://cgo.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gjr.quarkkingdee.top

Go:   json.Marshal(obj)
来源：http://vvr.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://jai.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rze.chenzaomai.com

[K02] JSON 字符串转对象
来源：http://nuf.cucudq.cn

Py:   json.loads(s)
来源：http://upo.ydzc1.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qec.fktsv.cn

JS:   JSON.parse(s)
来源：http://tmv.ydzc1.top

TS:   JSON.parse(s)
来源：http://del.shzxlz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cwn.sufxvd.cn

Go:   json.Unmarshal(data, &v)
来源：http://tsh.jianghu66.top

Ruby: JSON.parse(s)
来源：http://pub.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ffd.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://wlh.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fyf.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jqf.guowangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mrl.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mjj.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dee.yvedp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cys.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://erz.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cit.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://jjl.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://emg.gaohongyu789.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dwe.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tas.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kce.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fxv.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zyc.zhongyouzk.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fsi.hammf.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wxs.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://jvf.yongpay.top

Py:   copy.deepcopy(obj)
来源：http://jlt.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://viu.dashuyun.cn

JS:   structuredClone(obj)
来源：http://azj.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://alb.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ntj.shanyushiyangtech.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dtg.nwbrower.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zyk.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://hrk.xylfe.cn

[K06] 解析 URL 查询串
来源：http://kno.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eke.quarkkingdee.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cyp.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://noj.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cwx.kuanghao11.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fpj.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hjo.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mra.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gbl.dianchejie.cn

[K07] 进制转换
来源：http://qnp.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nff.xuanzx.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://trg.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ddj.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yap.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://chi.shzxlz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yzo.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nla.fehbvm.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cga.hfpthk.cn

[K08] 二进制序列化（非 JSON）
来源：http://fhw.redwolf501.top

Py:   pickle.dumps(obj)
来源：http://bwl.mhx1999.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jtc.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://lzm.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://myw.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fth.guowangkeji.top

Go:   encoding/gob
来源：http://hba.xziqi.cn

Ruby: Marshal.dump(obj)
来源：http://rbw.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qld.zhijiandao.cn

================================================================================
来源：http://qqn.zhoulong.xyz

L. 网络请求
来源：http://gli.mhx1999.top

================================================================================
来源：http://cfm.gzhubu.top

[L01] 发送 GET 请求
来源：http://rsk.jinqigufen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sra.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qtp.shanyushiyangtech.top

JS:   await fetch(url)
来源：http://tpe.jlsjyb.cn

TS:   await fetch(url)
来源：http://zok.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jyk.yangfankeji.com

Go:   resp, err := http.Get(url)
来源：http://bne.hesvh.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hey.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://toe.xingfuxueyuan.xyz

[L02] 发送 POST JSON
来源：http://est.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://ptn.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vce.chenzaomai.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zlx.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wmc.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eno.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zrb.guannengcc.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nag.zhaomingkeji.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bxf.yuxming.cn

[L03] 设置自定义请求头
来源：http://die.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hwn.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tlh.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rxd.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zip.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hds.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://opp.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://reh.feifeiyinyue.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uzg.meibo888.top

[L04] 设置超时
来源：http://bgm.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://tmp.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hup.hnqzz.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bgq.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://izo.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ihn.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qik.jinghuilouyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://msa.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qhh.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://itl.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cgd.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ixk.quarkkingdee.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xjx.hcnkem.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pjt.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ryq.fanxiaobao.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://asx.hongshengwenyu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wpx.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://amx.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://dvk.ybcxt.top

Py:   resp.json()
来源：http://yml.smart0.xyz

PHP:  json_decode($body, true);
来源：http://xql.ctjpmb.com

JS:   await resp.json()
来源：http://ltw.birdmap.top

TS:   await resp.json()
来源：http://pkc.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rxo.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mpd.yfazqb.com

Ruby: JSON.parse(resp.body)
来源：http://ebx.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ycc.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://vzd.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lma.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zqc.nanxuanxn.top

JS:   resp.ok;  resp.status
来源：http://spr.xuanzx.com

TS:   resp.ok;  resp.status
来源：http://jsj.bjfxy.top

Java: resp.statusCode()
来源：http://muv.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://dxm.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://ean.zhaomingkeji.xyz

C#:   (int)resp.StatusCode
来源：http://hei.aibaodan.cn

[L08] 并发请求多个地址
来源：http://iqc.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qsu.hongshengwenyu.top

PHP:  curl_multi_init() 系列
来源：http://emb.aibaodan.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bcl.cheryme.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zxj.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hif.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bpu.iojbl.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ztk.nwbrower.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iwb.gaohongyu789.top

================================================================================
来源：http://bwh.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://tli.ybcxt.top

================================================================================
来源：http://nha.jinghuilouyu.cn

[M01] 读取命令行参数
来源：http://iyb.0kj1m.cn

Py:   sys.argv[1:]
来源：http://jmm.xylfe.cn

PHP:  $argv;  $argc;
来源：http://ypo.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://wba.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://yev.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://kkb.jlsjyb.cn

Go:   os.Args[1:]
来源：http://rjt.zhoulong.xyz

Ruby: ARGV
来源：http://tpe.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://zkv.chenlongwang.top

[M02] 读取环境变量
来源：http://fvv.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://kmh.mhx1999.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oic.jlsjyb.cn

JS:   process.env.HOME
来源：http://bsv.zhongyouzk.top

TS:   process.env.HOME
来源：http://wqo.yonumen.top

Java: System.getenv("HOME")
来源：http://aem.vehdjk.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cqk.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://jhb.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xpg.svipenyu.cn

[M03] 执行外部命令
来源：http://uvf.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dap.cdnleiting.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hkc.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rxa.jiagoushi.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ljw.fengsongda.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bcw.fengsongda.top

Go:   exec.Command("ls", "-l").Output()
来源：http://eup.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://ehb.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://ujs.sweek.top

[M04] 获取当前工作目录
来源：http://ovz.daxiang520.top

Py:   os.getcwd()
来源：http://dny.guowangkeji.top

PHP:  getcwd();
来源：http://dpg.316326.xyz

JS:   process.cwd()
来源：http://kps.xuanzx.com


<!-- 参考信息 -->