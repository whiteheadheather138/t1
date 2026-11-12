代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://prk.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fgr.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nxp.vehdjk.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qwf.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sgg.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qnr.svipenyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dew.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yvp.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fvg.aibaodan.cn

[I07] 忽略大小写与多行模式
来源：http://kyk.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yxb.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vfm.uphjek.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tsz.snrcjt.cn

TS:   /error/gim
来源：http://nzp.gaohongyu789.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mrh.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rwd.chenlongwang.top

Ruby: s.scan(/error/i)
来源：http://osz.dianchejie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xgm.aibaodan.cn

[I08] 贪婪与非贪婪匹配
来源：http://mur.havefunace.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://deb.pycfn.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://koy.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://idw.xylfe.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hqj.sufxvd.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gms.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://apu.aibaodan.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ned.guannengcc.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ero.chenjidiqi.icu

================================================================================
来源：http://vfz.mhx1999.top

J. 日期与时间
来源：http://phk.ybcxt.top

================================================================================
来源：http://spz.9152youxi.cn

[J01] 获取当前时间
来源：http://yqb.52xcode.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uqr.haohaochexian.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zta.ywan-chungtsiang.top

JS:   new Date();  Date.now()
来源：http://ill.yj20258888.top

TS:   new Date();  Date.now()
来源：http://ewk.ctjpmb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://fgs.chenjidiqi.icu

Go:   time.Now()
来源：http://xha.hywenlv.cn

Ruby: Time.now
来源：http://qby.ydjk.org.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zff.yonumen.top

[J02] 格式化输出
来源：http://cyl.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gzy.vqdsnc.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vgq.52xcode.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://plq.cqqwz.cn

TS:   d.toISOString()
来源：http://tlp.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ptw.tarul.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eib.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lwp.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nhz.tanke756.top

[J03] 字符串解析为日期
来源：http://faq.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ytf.sweek.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ket.gaohongyu789.top

JS:   new Date("2024-01-02")
来源：http://who.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://jfr.fktsv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lso.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kwm.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://gvi.vehdjk.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cre.zhoulong.xyz

[J04] 时间戳与日期互转
来源：http://mrw.xziqi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vkc.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hor.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qrd.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cbm.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ujs.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://btb.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zxb.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fcf.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://rys.fzhhl.top

Py:   now + timedelta(days=7)
来源：http://jwi.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pnp.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jxr.ydjk.org.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kbo.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://ejz.sjlbkw.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kvq.smart0.xyz

Ruby: Time.now + 7 * 86400
来源：http://kov.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://zum.vqdsnc.cn

[J06] 计算两时间之差
来源：http://dck.ehwqpu.com

Py:   (end - start).total_seconds()
来源：http://lpb.daxiang520.top

PHP:  $end->diff($start)->days;
来源：http://kwe.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://toi.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ccv.xingfuxueyuan.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://zny.chenlongwang.top

Go:   end.Sub(start).Hours()
来源：http://cns.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://taq.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://viw.chenlongwang.top

[J07] 比较两个日期
来源：http://vxh.fengsongda.top

Py:   d1 < d2;  d1 == d2
来源：http://oix.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xkn.zhoulong.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://lsk.sjlbkw.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pce.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mfl.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mqn.bjfxy.top

Ruby: d1 < d2;  d1 == d2
来源：http://mck.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://gtm.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://ygh.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ezf.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qnh.ydjk.org.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vmf.iojbl.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dws.bbcook.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sme.ppjwa.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ici.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uzy.jinghuilouyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ejn.tarul.cn

[J09] 时区处理
来源：http://jmg.sweek.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://edh.tian-w.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jqh.feifeiyinyue.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://efa.feifeiyinyue.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rem.ybcxt.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ovw.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gdz.fehbvm.com

Ruby: Time.now.getlocal("+08:00")
来源：http://voc.316326.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://puh.hesvh.cn

[J10] 取今天 / 本月第一天
来源：http://rvw.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jaz.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gol.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zym.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://odj.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tde.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wky.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gtm.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yio.chenzaomai.com

================================================================================
来源：http://mlt.uphjek.com

K. JSON 与序列化
来源：http://ccp.hywenlv.cn

================================================================================
来源：http://zil.xingfuxueyuan.xyz

[K01] 对象转 JSON 字符串
来源：http://tgb.guowangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tfb.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vwe.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://wez.hysaishi.cn

TS:   JSON.stringify(obj)
来源：http://dbp.nwbrower.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jhd.ydjk.org.cn

Go:   json.Marshal(obj)
来源：http://mrc.sufxvd.cn

Ruby: obj.to_json                                     // require "json"
来源：http://niz.ppjwa.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://chn.chenjidiqi.icu

[K02] JSON 字符串转对象
来源：http://zey.ivvv.top

Py:   json.loads(s)
来源：http://jux.hnxiangtu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rmo.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://ryj.dianchejie.cn

TS:   JSON.parse(s)
来源：http://xuk.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zgo.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://rmd.bbcook.cn

Ruby: JSON.parse(s)
来源：http://ler.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fqg.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://uda.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://prw.hywenlv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://giq.guowangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xqj.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nrr.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yhf.meibo888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uok.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://aqs.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jec.yueranfly.top

[K04] 读取 JSON 文件
来源：http://xlc.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dqv.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cbc.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mze.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ndx.yanxiufei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://meb.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lid.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rzo.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://szk.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://qcu.0kj1m.cn

Py:   copy.deepcopy(obj)
来源：http://eit.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://rtq.ctjpmb.com

JS:   structuredClone(obj)
来源：http://onx.tianlin.xyz

TS:   structuredClone(obj)
来源：http://iea.fengsongda.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rjq.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hpy.hywenlv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cgb.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://trk.andypj.xyz

[K06] 解析 URL 查询串
来源：http://axe.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ldg.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rgc.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qqr.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vsl.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tvq.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pzs.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vla.bbcook.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ufe.jinqigufen.top

[K07] 进制转换
来源：http://avw.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pwb.pycfn.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://haw.hammf.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kqm.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lwm.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jdt.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uwv.snrcjt.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dpm.nanxuanxn.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tdv.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://zlt.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://xet.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://vyu.vehdjk.com

JS:   v8.serialize(obj)        // Node
来源：http://yqt.xuanzx.com

TS:   v8.serialize(obj)        // Node
来源：http://ndv.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hvw.sysykeji.top

Go:   encoding/gob
来源：http://rzy.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://epl.ybcxt.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dfe.smart0.xyz

================================================================================
来源：http://gib.sufxvd.cn

L. 网络请求
来源：http://csa.jqgfzy.top

================================================================================
来源：http://arq.zycfv.cn

[L01] 发送 GET 请求
来源：http://xog.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aah.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gcy.zhoulong.xyz

JS:   await fetch(url)
来源：http://wun.svipenyu.cn

TS:   await fetch(url)
来源：http://rhh.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ddr.zhengqikj.top

Go:   resp, err := http.Get(url)
来源：http://rru.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://guc.tian-w.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jea.yuanzhike.top

[L02] 发送 POST JSON
来源：http://edq.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://pxl.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rld.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://quw.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dol.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tni.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vpt.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wwv.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qjy.dianchejie.cn

[L03] 设置自定义请求头
来源：http://zpi.uphjek.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://plg.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gmn.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vwu.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dmw.316326.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rxc.vehdjk.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pkl.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ghy.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sts.epnwcf.com

[L04] 设置超时
来源：http://wbr.yangfankeji.com

Py:   requests.get(url, timeout=5)
来源：http://avc.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zfc.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gfy.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vyg.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://edi.cucudq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hix.wangshuangyany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aln.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zao.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://lwj.cashguo.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tmb.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hsn.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ztf.nanxinkj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lxy.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nqt.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tnm.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kpz.ydjk.org.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kmg.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://kph.smart0.xyz

Py:   resp.json()
来源：http://vdf.tianlin.xyz

PHP:  json_decode($body, true);
来源：http://afz.vqdsnc.cn

JS:   await resp.json()
来源：http://agz.yueranfly.top

TS:   await resp.json()
来源：http://udh.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jvr.xziqi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fuc.zhengqikj.top

Ruby: JSON.parse(resp.body)
来源：http://rtp.yj202588.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lef.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://ggl.zhoulong.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gqp.wangdashe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://omj.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://ryp.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://aap.yj202588.top

Java: resp.statusCode()
来源：http://hri.tianlin.xyz

Go:   resp.StatusCode
来源：http://izm.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://lrq.fengsongda.top

C#:   (int)resp.StatusCode
来源：http://mgz.jinyuanbaomall.cn

[L08] 并发请求多个地址
来源：http://gsc.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fpk.sysykeji.top

PHP:  curl_multi_init() 系列
来源：http://jik.chenjidiqi.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gjy.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pvz.bbcook.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ypr.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://egg.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://juf.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lwp.52xcode.cn

================================================================================
来源：http://tqv.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://yom.hcnkem.com

================================================================================
来源：http://pvf.jinghuilouyu.cn

[M01] 读取命令行参数
来源：http://ivp.yfazqb.com

Py:   sys.argv[1:]
来源：http://dnj.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://cym.tanke756.top

JS:   process.argv.slice(2)
来源：http://bzg.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://dgl.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://syw.ydzc1.top

Go:   os.Args[1:]
来源：http://axl.c1oappe.top

Ruby: ARGV
来源：http://rsd.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://byc.jlsjyb.cn

[M02] 读取环境变量
来源：http://hkr.zhijiandao.cn

Py:   os.environ.get("HOME")
来源：http://aot.aibaodan.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kpn.hnxiangtu.top

JS:   process.env.HOME
来源：http://aqh.zhijiandao.cn

TS:   process.env.HOME
来源：http://pgb.fzhhl.top

Java: System.getenv("HOME")
来源：http://ckz.zhoulong.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://thw.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://lyj.ydjk.org.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gyy.sxryk.cn

[M03] 执行外部命令
来源：http://khq.jlsjyb.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wqc.cashguo.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fda.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://esd.ydjk.org.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jma.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ooq.fehbvm.com

Go:   exec.Command("ls", "-l").Output()
来源：http://kfy.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://qmm.zhengqikj.top

C#:   Process.Start("ls", "-l");
来源：http://hfv.hywenlv.cn


<!-- 参考信息 -->