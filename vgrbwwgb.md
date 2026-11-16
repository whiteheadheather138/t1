代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cpv.ehwqpu.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lpj.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rke.shanyushiyangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nuc.vehdjk.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yby.hysaishi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gia.9152youxi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lts.kuanghao11.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pby.hfpthk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bcx.redwolf501.top

[I07] 忽略大小写与多行模式
来源：http://pmf.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kzj.zhijiandao.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wvk.kuanghao11.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wuc.tarul.cn

TS:   /error/gim
来源：http://awp.yangfankeji.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ngt.52xcode.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bsr.vehdjk.com

Ruby: s.scan(/error/i)
来源：http://qlw.zhixingplan.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://foo.svipenyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://ccu.fengsongda.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bdk.jqgufenzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://knm.zhixingplan.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dut.cdnleiting.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ehw.ywan-chungtsiang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ebb.yj202588.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ejf.yj20258888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tcy.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://scn.yangfankeji.com

================================================================================
来源：http://nxe.guowangkeji.top

J. 日期与时间
来源：http://olh.haohaochexian.top

================================================================================
来源：http://ehx.nanxuanxn.top

[J01] 获取当前时间
来源：http://gkj.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fso.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://whv.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://mdo.guowangkeji.top

TS:   new Date();  Date.now()
来源：http://dut.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ucp.pengpengdd.cyou

Go:   time.Now()
来源：http://kak.tian-w.cn

Ruby: Time.now
来源：http://puz.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dha.chenlongwang.top

[J02] 格式化输出
来源：http://vbr.guannengcc.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zix.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://poq.ehwqpu.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kom.havefunace.top

TS:   d.toISOString()
来源：http://knq.vehdjk.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mda.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cwi.snrcjt.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nme.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ste.wangdashe.top

[J03] 字符串解析为日期
来源：http://ndr.hnqzz.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://efx.sysykeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://okj.aibaodan.cn

JS:   new Date("2024-01-02")
来源：http://oxr.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://vfe.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dnc.tianlin.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zfp.yangfankeji.com

Ruby: Date.parse("2024-01-02")
来源：http://bra.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uqq.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://xxs.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rll.kuanghao11.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vzp.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fbo.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ajv.bbcook.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mkq.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pqt.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ycx.jianghu66.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lhq.jinqigfzy.top

[J05] 时间加减（加 7 天）
来源：http://yny.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://fwz.sweek.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vdy.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ijf.haohaochexian.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hxc.redwolf501.top

Java: LocalDate.now().plusDays(7)
来源：http://ozw.tarul.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hua.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://qsm.vqdsnc.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qum.xuanzx.com

[J06] 计算两时间之差
来源：http://zuu.ywan-chungtsiang.top

Py:   (end - start).total_seconds()
来源：http://prw.bbcook.cn

PHP:  $end->diff($start)->days;
来源：http://wvc.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hyr.shanyushiyangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fgz.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wca.cdnleiting.top

Go:   end.Sub(start).Hours()
来源：http://vwa.c1oappe.top

Ruby: end - start                 # 返回秒数
来源：http://meo.tarul.cn

C#:   (end - start).TotalSeconds
来源：http://nlm.tian-w.cn

[J07] 比较两个日期
来源：http://pad.meibo888.top

Py:   d1 < d2;  d1 == d2
来源：http://wtc.zdqjudy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://awt.ywan-chungtsiang.top

JS:   d1.getTime() < d2.getTime()
来源：http://yrs.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://cni.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nog.jiagoushi.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qau.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jqx.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://ivb.xylfe.cn

[J08] 提取年月日与星期
来源：http://pix.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hci.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vwx.shanyushiyangtech.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zio.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pxv.epnwcf.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xrp.jinqigfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mut.shzxlz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pdo.aibaodan.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yir.sweek.top

[J09] 时区处理
来源：http://boi.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://npi.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://thp.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pta.c1oappe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nkr.shuidangran.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tlz.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dnv.andypj.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://dot.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wyf.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://pon.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://icg.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://flw.bjfxy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yaa.svipenyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tdk.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nli.zhixingplan.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aga.aibaodan.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qhi.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://klq.yangfankeji.com

================================================================================
来源：http://glf.jqgfzy.top

K. JSON 与序列化
来源：http://pvn.9152youxi.cn

================================================================================
来源：http://esg.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://oyl.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kfm.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://axr.yj202588.top

JS:   JSON.stringify(obj)
来源：http://spp.ivvv.top

TS:   JSON.stringify(obj)
来源：http://ism.ehwqpu.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ldp.fktsv.cn

Go:   json.Marshal(obj)
来源：http://nsv.andypj.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://pax.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gjb.yonumen.top

[K02] JSON 字符串转对象
来源：http://bzq.xuetiantiany.cn

Py:   json.loads(s)
来源：http://glg.andypj.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yhn.zhengqikj.top

JS:   JSON.parse(s)
来源：http://tco.yonumen.top

TS:   JSON.parse(s)
来源：http://cab.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zoq.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://lsx.xinyue.icu

Ruby: JSON.parse(s)
来源：http://rhg.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vkc.quarkkingdee.top

[K03] JSON 美化输出（带缩进）
来源：http://tns.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sou.hywenlv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bnr.guowangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rtp.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://odv.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zpg.shangyingyoupin.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://emv.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://usd.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ctz.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://cif.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qrd.yuxming.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ftr.yj202588.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eof.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qwk.zhixingplan.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kyv.fengsongda.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rtz.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://imw.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ltr.zycfv.cn

[K05] 深拷贝对象
来源：http://mob.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://qpj.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://msl.uphjek.com

JS:   structuredClone(obj)
来源：http://uws.ybcxt.top

TS:   structuredClone(obj)
来源：http://zjc.gogol.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://snn.tanke756.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oyw.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://abo.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://eme.jqgfzy.top

[K06] 解析 URL 查询串
来源：http://duv.cucudq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wms.kuanghao11.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yua.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xth.meibo888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vda.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://boa.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://djh.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://amt.xingfuxueyuan.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ifa.hcnkem.com

[K07] 进制转换
来源：http://zuv.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://suv.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xwq.tanke756.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lnb.yvedp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://avs.ivvv.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://osg.bbcook.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eaw.xziqi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ioa.fengsongda.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ecl.xuetiantiany.cn

[K08] 二进制序列化（非 JSON）
来源：http://dmh.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://llc.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://haw.tianlin.xyz

JS:   v8.serialize(obj)        // Node
来源：http://yoq.jinqigfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://srj.bbcook.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vee.zhongyouzk.top

Go:   encoding/gob
来源：http://udz.zdqjudy.top

Ruby: Marshal.dump(obj)
来源：http://jrc.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qbq.zhoulong.xyz

================================================================================
来源：http://npe.wangshuangyany.cn

L. 网络请求
来源：http://fss.yueranfly.top

================================================================================
来源：http://pzr.vehdjk.com

[L01] 发送 GET 请求
来源：http://lyx.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://flk.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zmd.sweek.top

JS:   await fetch(url)
来源：http://hkq.nanxinkj.top

TS:   await fetch(url)
来源：http://bem.cucudq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mcm.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://qcw.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://iit.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://han.ywan-chungtsiang.top

[L02] 发送 POST JSON
来源：http://wxv.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://bas.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hfd.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://seo.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eoy.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xxh.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kpq.guowangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nub.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ddi.jqgfzy.top

[L03] 设置自定义请求头
来源：http://dpj.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ovi.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://txd.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://asf.zdqjudy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tdj.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xua.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vdt.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mvo.yongpay.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://skp.yonumen.top

[L04] 设置超时
来源：http://prc.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://nxc.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pwu.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wcd.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tef.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ghe.zhoulong.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kfn.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://brf.nanxuanxn.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eqi.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://fbi.yfazqb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kaa.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xhb.svipenyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bld.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kjc.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kib.wangshuangyany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ead.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tbj.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://khj.jyoumei.cn

[L06] 解析响应为 JSON
来源：http://hkz.zhaomingkeji.xyz

Py:   resp.json()
来源：http://rxy.ehwqpu.com

PHP:  json_decode($body, true);
来源：http://dvx.jqgufenzy.top

JS:   await resp.json()
来源：http://ghm.fengsongda.top

TS:   await resp.json()
来源：http://qyg.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vte.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tbs.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://mcs.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://slc.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://qtf.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hvk.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nwq.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://ehu.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://npm.cqqwz.cn

Java: resp.statusCode()
来源：http://mfo.nanxuanxn.top

Go:   resp.StatusCode
来源：http://aui.jqgfzy.top

Ruby: resp.code.to_i
来源：http://ved.smart0.xyz

C#:   (int)resp.StatusCode
来源：http://jqi.zdbjq.cn

[L08] 并发请求多个地址
来源：http://iue.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lte.nanxuanxn.top

PHP:  curl_multi_init() 系列
来源：http://vdh.hnqzz.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://arf.daria6918.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pwo.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yaa.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jfj.nanxuanxn.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yvj.yfazqb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fso.hesvh.cn

================================================================================
来源：http://yeg.ehwqpu.com

M. 命令行 / 进程 / 环境
来源：http://vis.zhengqikj.top

================================================================================
来源：http://skx.fzhhl.top

[M01] 读取命令行参数
来源：http://ocj.haohaochexian.top

Py:   sys.argv[1:]
来源：http://wtj.hnqzz.top

PHP:  $argv;  $argc;
来源：http://kev.hysaishi.cn

JS:   process.argv.slice(2)
来源：http://zrx.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://leq.xziqi.cn

Java: args 数组（main 方法参数）
来源：http://djl.nanxuanxn.top

Go:   os.Args[1:]
来源：http://irb.svipenyu.cn

Ruby: ARGV
来源：http://hfm.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://ljf.ybcxt.top

[M02] 读取环境变量
来源：http://hre.yueranfly.top

Py:   os.environ.get("HOME")
来源：http://weu.ywan-chungtsiang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pgk.pengpengdd.cyou

JS:   process.env.HOME
来源：http://yvv.pycfn.com

TS:   process.env.HOME
来源：http://xzp.yuanzhike.top

Java: System.getenv("HOME")
来源：http://xeh.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://red.dianchejie.cn

Ruby: ENV["HOME"]
来源：http://xmi.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ffh.zhengqikj.top

[M03] 执行外部命令
来源：http://gzh.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vpc.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dqt.iojbl.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fjk.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nxx.tian-w.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fnd.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fqv.hfpthk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hzp.shuidangran.top

C#:   Process.Start("ls", "-l");
来源：http://lwg.hfpthk.cn


<!-- 参考信息 -->