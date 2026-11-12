代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fmh.jqgfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mbo.ybcxt.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://siw.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wyn.0kj1m.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oob.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://wff.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rbd.feifeiyinyue.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mpr.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kkt.chenlongwang.top

TS:   /error/gim
来源：http://uvo.xylfe.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://azi.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jsu.nanxinkj.top

Ruby: s.scan(/error/i)
来源：http://dql.jqgufenzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ejt.hnqzz.top

[I08] 贪婪与非贪婪匹配
来源：http://rip.yuxming.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ygq.jlsjyb.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pnd.hfpthk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ynm.cdnleiting.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://edv.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://huw.bbcook.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vgh.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aik.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hhu.zhoulong.xyz

================================================================================
来源：http://obi.hfpthk.cn

J. 日期与时间
来源：http://cfo.shzxlz.cn

================================================================================
来源：http://osr.tianlin.xyz

[J01] 获取当前时间
来源：http://fcv.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gyd.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sfj.hnqzz.top

JS:   new Date();  Date.now()
来源：http://wjz.daxiang520.top

TS:   new Date();  Date.now()
来源：http://euf.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mll.gzhubu.top

Go:   time.Now()
来源：http://cmp.dashuyun.cn

Ruby: Time.now
来源：http://qly.ydzc1.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xit.hfpthk.cn

[J02] 格式化输出
来源：http://fip.iojbl.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nbq.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://foe.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fvp.aizwys.cn

TS:   d.toISOString()
来源：http://wel.guannengcc.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vvw.shuidangran.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://unn.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wtz.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ggk.tarul.cn

[J03] 字符串解析为日期
来源：http://ywv.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cbt.ydzc1.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://idx.nwbrower.top

JS:   new Date("2024-01-02")
来源：http://xix.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://fao.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://qeo.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gmz.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://plm.snrcjt.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://utn.uphjek.com

[J04] 时间戳与日期互转
来源：http://gxi.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ebc.xinyue.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yga.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jcd.kuanghao11.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bgs.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hfe.zhoulong.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mqc.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bwk.zycfv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ngp.fzhhl.top

[J05] 时间加减（加 7 天）
来源：http://mmu.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://xqy.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://drg.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lhu.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xat.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://qow.birdmap.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xai.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://ydd.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://fjh.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://swk.birdmap.top

Py:   (end - start).total_seconds()
来源：http://drr.xziqi.cn

PHP:  $end->diff($start)->days;
来源：http://bda.dianchejie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ako.zhengqikj.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eas.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://qrz.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://vpu.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://fbm.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://sqb.jiagoushi.top

[J07] 比较两个日期
来源：http://ppb.cqqwz.cn

Py:   d1 < d2;  d1 == d2
来源：http://wcc.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://odc.fzhhl.top

JS:   d1.getTime() < d2.getTime()
来源：http://iaj.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://zjo.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kno.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zqf.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nyi.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://dip.gaohongyu789.top

[J08] 提取年月日与星期
来源：http://bqm.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vkh.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ysj.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fel.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gmp.316326.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xrm.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nxe.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yju.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kgz.ydzc1.top

[J09] 时区处理
来源：http://our.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ggp.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ngj.sufxvd.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bzq.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vfw.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pjg.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tyk.jiagoushi.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wna.zycfv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://log.gogol.net.cn

[J10] 取今天 / 本月第一天
来源：http://nzl.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://svh.wangshuangyany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://acy.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rfl.yuxming.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qvu.hammf.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rre.guowangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://irf.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jrd.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tqt.jinqigfzy.top

================================================================================
来源：http://qmi.hesvh.cn

K. JSON 与序列化
来源：http://lia.guowangkeji.top

================================================================================
来源：http://fok.jinqigufen.top

[K01] 对象转 JSON 字符串
来源：http://fhm.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qud.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oqi.shanyushiyangkeji.top

JS:   JSON.stringify(obj)
来源：http://jfu.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://sfp.haohaochexian.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ahh.xinyue.icu

Go:   json.Marshal(obj)
来源：http://czg.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://fjq.andypj.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://ohg.meibo888.top

[K02] JSON 字符串转对象
来源：http://mzq.yueranfly.top

Py:   json.loads(s)
来源：http://dxm.hcnkem.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cen.aizwys.cn

JS:   JSON.parse(s)
来源：http://ogw.mhx1999.top

TS:   JSON.parse(s)
来源：http://pwn.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ose.andypj.xyz

Go:   json.Unmarshal(data, &v)
来源：http://atd.hammf.cn

Ruby: JSON.parse(s)
来源：http://vmm.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zws.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://evz.0kj1m.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wqg.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pov.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nad.hnqzz.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dnd.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dmn.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ffe.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://hnc.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://han.sweek.top

[K04] 读取 JSON 文件
来源：http://taw.wangshuangyany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yju.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yhu.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yan.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://avn.c1oappe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fhg.mhx1999.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mvk.zhiwuduotai.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://efc.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tgx.ydzc1.top

[K05] 深拷贝对象
来源：http://hph.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://yrt.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://mzv.yangfankeji.com

JS:   structuredClone(obj)
来源：http://wig.hfpthk.cn

TS:   structuredClone(obj)
来源：http://uxq.jlsjyb.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yxq.tanke756.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fqz.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bok.tanke756.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qvr.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://ymz.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cke.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://flu.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nqn.bbcook.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oua.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zgv.yuxming.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ipe.zhoulong.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zam.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ydd.tian-w.cn

[K07] 进制转换
来源：http://xjd.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wka.0kj1m.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://btu.fanxiaobao.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tbg.fengsongda.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yrv.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sgc.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mzu.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pkr.pengpengdd.cyou

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zpf.guowangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://wiu.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://njh.c1oappe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zon.cucudq.cn

JS:   v8.serialize(obj)        // Node
来源：http://tvu.zhixingplan.top

TS:   v8.serialize(obj)        // Node
来源：http://kvm.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ptp.fzhhl.top

Go:   encoding/gob
来源：http://csm.jinyuanbaomall.cn

Ruby: Marshal.dump(obj)
来源：http://sbx.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xuc.hfpthk.cn

================================================================================
来源：http://pdo.vehdjk.com

L. 网络请求
来源：http://ues.yonumen.top

================================================================================
来源：http://hoo.shanyushiyangtech.top

[L01] 发送 GET 请求
来源：http://esq.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mhg.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zqp.shzxlz.cn

JS:   await fetch(url)
来源：http://ibi.jinqigufen.top

TS:   await fetch(url)
来源：http://zbd.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ujx.andypj.xyz

Go:   resp, err := http.Get(url)
来源：http://apg.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xhb.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gxt.nanxinkj.top

[L02] 发送 POST JSON
来源：http://stu.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://xpp.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zma.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gwj.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ufg.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kab.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gsx.yfazqb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lby.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ony.yj20258.top

[L03] 设置自定义请求头
来源：http://ogc.yj20258888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mpg.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xcb.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zhf.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://won.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dki.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://osp.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ftl.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aih.jinqigufen.top

[L04] 设置超时
来源：http://way.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://kxg.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://svf.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vjk.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://crn.uphjek.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mlg.yanxiufei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lab.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xvh.cheryme.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mzj.kuanghao11.cn

[L05] 上传文件（multipart）
来源：http://iez.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hqr.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qib.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qac.9152youxi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jxm.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lno.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rtg.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://flw.gzhubu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eoz.gogol.net.cn

[L06] 解析响应为 JSON
来源：http://irb.hnqzz.top

Py:   resp.json()
来源：http://gjg.xuanzx.com

PHP:  json_decode($body, true);
来源：http://sgf.nanxinkj.top

JS:   await resp.json()
来源：http://wrj.mhx1999.top

TS:   await resp.json()
来源：http://uqi.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sar.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oxe.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://wto.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://chw.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://sck.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://txh.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kpm.wangdashe.top

JS:   resp.ok;  resp.status
来源：http://ghe.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://esa.ydjk.org.cn

Java: resp.statusCode()
来源：http://vbq.hfpthk.cn

Go:   resp.StatusCode
来源：http://hjj.shuidangran.top

Ruby: resp.code.to_i
来源：http://yyw.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://hdg.guowangkeji.top

[L08] 并发请求多个地址
来源：http://awb.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://juh.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://fbd.nanxinkj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gtx.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kwc.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://umd.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vln.shuidangran.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://evu.yfazqb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://luy.xuanzx.com

================================================================================
来源：http://mmh.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://kvv.gaohongyu789.top

================================================================================
来源：http://paf.yuanzhike.top

[M01] 读取命令行参数
来源：http://iod.zhoulong.xyz

Py:   sys.argv[1:]
来源：http://fwd.xylfe.cn

PHP:  $argv;  $argc;
来源：http://tdj.feifeiyinyue.top

JS:   process.argv.slice(2)
来源：http://lrv.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://pur.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://tdf.tianlin.xyz

Go:   os.Args[1:]
来源：http://epk.tian-w.cn

Ruby: ARGV
来源：http://bkg.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://xoh.c1oappe.top

[M02] 读取环境变量
来源：http://voq.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://zoj.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pzo.gogol.net.cn

JS:   process.env.HOME
来源：http://xge.chenlongwang.top

TS:   process.env.HOME
来源：http://kzz.aibaodan.cn

Java: System.getenv("HOME")
来源：http://lbl.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fet.jinqigufen.top

Ruby: ENV["HOME"]
来源：http://slf.fanxiaobao.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jwr.ppjwa.cn

[M03] 执行外部命令
来源：http://gwk.sjlbkw.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pre.cashguo.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hzg.zhongyouzk.top

JS:   child_process.execSync("ls -l").toString()
来源：http://iar.ydzc1.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mmb.jiagoushi.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://epb.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ucz.yanxiufei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kgx.meibo888.top

C#:   Process.Start("ls", "-l");
来源：http://mpe.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://gpl.shzxlz.cn

Py:   os.getcwd()
来源：http://oel.xinyue.icu

PHP:  getcwd();
来源：http://eke.meibo888.top

JS:   process.cwd()
来源：http://llf.yangfankeji.com


<!-- 参考信息 -->