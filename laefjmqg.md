代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ncg.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://jii.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kpa.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zge.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jhn.gogol.net.cn

TS:   /error/gim
来源：http://nae.zhongyouzk.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hyx.gogol.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jiy.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://lom.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://amm.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://lsh.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ypz.yj20258888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gae.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://spu.vehdjk.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qgm.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mrf.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ybu.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uwb.tian-w.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tty.svipenyu.cn

================================================================================
来源：http://xdd.xingfuxueyuan.xyz

J. 日期与时间
来源：http://lgf.fanxiaobao.xyz

================================================================================
来源：http://qjd.xziqi.cn

[J01] 获取当前时间
来源：http://aco.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tvu.pycfn.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xix.bbcook.cn

JS:   new Date();  Date.now()
来源：http://fzt.yueranfly.top

TS:   new Date();  Date.now()
来源：http://std.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cno.vehdjk.com

Go:   time.Now()
来源：http://fms.0kj1m.cn

Ruby: Time.now
来源：http://dit.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xqg.316326.xyz

[J02] 格式化输出
来源：http://pal.pycfn.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lct.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cmq.hywenlv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mdt.pycfn.com

TS:   d.toISOString()
来源：http://oes.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://icv.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qoh.snrcjt.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ovn.hywenlv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nai.yueranfly.top

[J03] 字符串解析为日期
来源：http://cxp.ppjwa.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xyu.fktsv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hgh.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://znr.cqqwz.cn

TS:   new Date("2024-01-02")
来源：http://wnj.jlsjyb.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ncx.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dly.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://maq.yfazqb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iwm.c1oappe.top

[J04] 时间戳与日期互转
来源：http://cjz.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wrp.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vap.pycfn.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zfe.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jbm.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jfx.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oyv.jiagoushi.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xdv.hcnkem.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tkq.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://cjw.gotoacloud.top

Py:   now + timedelta(days=7)
来源：http://hkn.jinqigfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mng.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nwn.xinyue.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ohq.svipenyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://ghw.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sxq.zhixingplan.top

Ruby: Time.now + 7 * 86400
来源：http://hgu.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iwm.yuanzhike.top

[J06] 计算两时间之差
来源：http://mjv.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://qll.wangshuangyany.cn

PHP:  $end->diff($start)->days;
来源：http://zgr.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ies.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kzi.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aox.cqqwz.cn

Go:   end.Sub(start).Hours()
来源：http://bij.yj202588.top

Ruby: end - start                 # 返回秒数
来源：http://fha.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://jqm.meibo888.top

[J07] 比较两个日期
来源：http://phf.shanyushiyangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://xfn.dianchejie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ovz.c1oappe.top

JS:   d1.getTime() < d2.getTime()
来源：http://ylm.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://ikm.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://roc.jiagoushi.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iwq.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://fyf.hesvh.cn

C#:   d1 < d2;  d1 == d2
来源：http://lfb.yfazqb.com

[J08] 提取年月日与星期
来源：http://lzf.ivvv.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jqh.wangshuangyany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gjr.yj20258.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wyp.yfazqb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sff.ctjpmb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xcr.uphjek.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yrk.ydjk.org.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ziu.ydzc1.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mye.xuanzx.com

[J09] 时区处理
来源：http://pfe.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lxg.0kj1m.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qtj.xinyue.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nac.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kzz.ehwqpu.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cth.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hda.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://flc.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nvl.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://ycb.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://fxm.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nrh.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ppa.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vwn.chenzaomai.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://szi.yj202588.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gbs.shuidangran.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gnd.aibaodan.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lcc.chenzaomai.com

================================================================================
来源：http://hzw.zhiwuduotai.top

K. JSON 与序列化
来源：http://nma.hysaishi.cn

================================================================================
来源：http://wwq.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://muz.iojbl.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ics.xuanzx.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xam.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://zqx.cheryme.top

TS:   JSON.stringify(obj)
来源：http://jbq.gotoacloud.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lmv.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://slz.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tul.zdbjq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bru.sysykeji.top

[K02] JSON 字符串转对象
来源：http://iqk.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://kgl.yj202588.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qcr.yj20258.top

JS:   JSON.parse(s)
来源：http://eiu.meibo888.top

TS:   JSON.parse(s)
来源：http://rfs.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mbx.yfazqb.com

Go:   json.Unmarshal(data, &v)
来源：http://vud.meibo888.top

Ruby: JSON.parse(s)
来源：http://koi.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ris.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://ttq.meibo888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lwf.gzhubu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oxo.redwolf501.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ynj.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fag.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gcj.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gjb.hywenlv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tsf.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qsj.zdqjudy.top

[K04] 读取 JSON 文件
来源：http://csi.zhiwuduotai.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://liu.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://osv.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kac.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wdz.jqgfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://itd.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://czf.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://hyw.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tpz.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://psc.tian-w.cn

Py:   copy.deepcopy(obj)
来源：http://zxo.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://ygv.havefunace.top

JS:   structuredClone(obj)
来源：http://qtu.gotoacloud.top

TS:   structuredClone(obj)
来源：http://xvs.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ziv.cdnleiting.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gqk.cheryme.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ljl.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kga.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://rxj.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tez.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yft.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ofs.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kpg.yuanzhike.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gem.316326.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://itx.hongshengwenyu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://avm.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fpm.haohaochexian.top

[K07] 进制转换
来源：http://mrf.yj20258888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hxc.mhx1999.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ujc.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nhd.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cho.cheryme.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xia.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lkx.epnwcf.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fip.feifeiyinyue.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://boj.fktsv.cn

[K08] 二进制序列化（非 JSON）
来源：http://hvn.havefunace.top

Py:   pickle.dumps(obj)
来源：http://qad.sysykeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zhs.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://zja.nwbrower.top

TS:   v8.serialize(obj)        // Node
来源：http://ooq.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://osh.sjlbkw.cn

Go:   encoding/gob
来源：http://tod.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://fly.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zbv.ivvv.top

================================================================================
来源：http://mhw.shanyushiyangtech.top

L. 网络请求
来源：http://yss.jiagoushi.top

================================================================================
来源：http://tat.sxryk.cn

[L01] 发送 GET 请求
来源：http://jno.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xzh.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://djo.ydjk.org.cn

JS:   await fetch(url)
来源：http://mhc.gaohongyu789.top

TS:   await fetch(url)
来源：http://tzo.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uty.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://ach.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://amg.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vac.haohaochexian.top

[L02] 发送 POST JSON
来源：http://uar.sufxvd.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ecv.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vrw.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://awn.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pdl.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://scx.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mzy.dashuyun.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xfb.aibaodan.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eha.zhijiandao.cn

[L03] 设置自定义请求头
来源：http://fum.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xoq.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://grw.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://feb.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lxp.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ikb.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xjv.hcnkem.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cao.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sav.chenzaomai.com

[L04] 设置超时
来源：http://rsx.wangshuangyany.cn

Py:   requests.get(url, timeout=5)
来源：http://mwu.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sax.0kj1m.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yeh.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ghl.chenjidiqi.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mvf.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://acw.zhongyouzk.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://owa.shuidangran.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wkl.hammf.cn

[L05] 上传文件（multipart）
来源：http://pyr.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jkx.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cyj.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dhk.andypj.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ozk.jianghu66.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sqw.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yyn.zhaomingkeji.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wmv.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hlj.nwbrower.top

[L06] 解析响应为 JSON
来源：http://ndp.yuanzhike.top

Py:   resp.json()
来源：http://jnj.wangdashe.top

PHP:  json_decode($body, true);
来源：http://xaa.zdqjudy.top

JS:   await resp.json()
来源：http://fab.sysykeji.top

TS:   await resp.json()
来源：http://lyw.ivvv.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kbh.yj20258888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aah.daria6918.cn

Ruby: JSON.parse(resp.body)
来源：http://uss.jinqigufen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://moh.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://rwu.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ctj.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lun.iojbl.cn

JS:   resp.ok;  resp.status
来源：http://oyo.meibo888.top

TS:   resp.ok;  resp.status
来源：http://ofm.bbcook.cn

Java: resp.statusCode()
来源：http://dro.zdqjudy.top

Go:   resp.StatusCode
来源：http://dpy.andypj.xyz

Ruby: resp.code.to_i
来源：http://npy.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://cih.nwbrower.top

[L08] 并发请求多个地址
来源：http://ewg.hongshengwenyu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qpe.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://fcj.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://seb.gzhubu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ecd.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://knr.zhaomingkeji.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dep.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fmg.vehdjk.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://irl.ydzc1.top

================================================================================
来源：http://maw.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://rgc.nwbrower.top

================================================================================
来源：http://gbz.yvedp.cn

[M01] 读取命令行参数
来源：http://gmz.tian-w.cn

Py:   sys.argv[1:]
来源：http://zvz.shangyingyoupin.top

PHP:  $argv;  $argc;
来源：http://bak.316326.xyz

JS:   process.argv.slice(2)
来源：http://ytq.sweek.top

TS:   process.argv.slice(2)
来源：http://zro.yongpay.top

Java: args 数组（main 方法参数）
来源：http://jzm.hammf.cn

Go:   os.Args[1:]
来源：http://bsc.vehdjk.com

Ruby: ARGV
来源：http://ybh.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://ygz.yueranfly.top

[M02] 读取环境变量
来源：http://xmw.tarul.cn

Py:   os.environ.get("HOME")
来源：http://byz.ctjpmb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wtl.52xcode.cn

JS:   process.env.HOME
来源：http://klj.nwbrower.top

TS:   process.env.HOME
来源：http://wbt.uphjek.com

Java: System.getenv("HOME")
来源：http://aot.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vyp.hfpthk.cn

Ruby: ENV["HOME"]
来源：http://pis.0kj1m.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://omp.guowangkeji.top

[M03] 执行外部命令
来源：http://hmg.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sil.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qbf.hnqzz.top

JS:   child_process.execSync("ls -l").toString()
来源：http://smp.cashguo.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wqk.jiagoushi.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bkz.hesvh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ewj.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://lde.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://qrd.ivvv.top

[M04] 获取当前工作目录
来源：http://dps.yfazqb.com

Py:   os.getcwd()
来源：http://xig.svipenyu.cn

PHP:  getcwd();
来源：http://rja.gogol.net.cn

JS:   process.cwd()
来源：http://noa.shangyingyoupin.top

TS:   process.cwd()
来源：http://omk.xylfe.cn

Java: Path.of("").toAbsolutePath()
来源：http://zyj.aizwys.cn

Go:   os.Getwd()
来源：http://ivw.ydjk.org.cn

Ruby: Dir.pwd
来源：http://noa.yj202588.top


<!-- 参考信息 -->