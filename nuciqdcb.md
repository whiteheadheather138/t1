代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nxs.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hqd.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jjq.jianghu66.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wxd.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kke.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cgy.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eim.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dxk.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bgn.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://bre.ywan-chungtsiang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tyj.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://laz.zhijiandao.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blr.bbcook.cn

TS:   /error/gim
来源：http://mtz.hywenlv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hne.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vuq.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://tej.ydzc1.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xqg.sjlbkw.cn

[I08] 贪婪与非贪婪匹配
来源：http://bzh.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vej.tianlin.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mrm.hfpthk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qds.xziqi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kxm.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xqn.zhijiandao.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jpm.52xcode.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gai.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ije.tianlin.xyz

================================================================================
来源：http://ehp.ybcxt.top

J. 日期与时间
来源：http://kdt.yfazqb.com

================================================================================
来源：http://gqm.zycfv.cn

[J01] 获取当前时间
来源：http://lej.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://myu.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://urj.tanke756.top

JS:   new Date();  Date.now()
来源：http://xhp.jlsjyb.cn

TS:   new Date();  Date.now()
来源：http://aao.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dlp.jiagoushi.top

Go:   time.Now()
来源：http://hak.haohaochexian.top

Ruby: Time.now
来源：http://vvt.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uuk.andypj.xyz

[J02] 格式化输出
来源：http://hyq.xuanzx.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vgf.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vxp.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kif.wangdashe.top

TS:   d.toISOString()
来源：http://wwo.jinyuanbaomall.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wjs.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qsd.fengsongda.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://snk.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lrp.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://pmk.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vif.52xcode.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://llc.sweek.top

JS:   new Date("2024-01-02")
来源：http://ddo.hammf.cn

TS:   new Date("2024-01-02")
来源：http://ufo.jianghu66.top

Java: LocalDate.parse("2024-01-02")
来源：http://uxi.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://osy.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://mis.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wrq.cheryme.top

[J04] 时间戳与日期互转
来源：http://ffd.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://frk.jyoumei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dic.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dmw.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://oax.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://naq.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xmw.tarul.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jnp.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nyj.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://imx.ybcxt.top

Py:   now + timedelta(days=7)
来源：http://ttj.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rth.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kub.316326.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vym.aibaodan.cn

Java: LocalDate.now().plusDays(7)
来源：http://mgi.cashguo.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zrz.bjfxy.top

Ruby: Time.now + 7 * 86400
来源：http://mfs.uphjek.com

C#:   DateTime.Now.AddDays(7)
来源：http://pia.epnwcf.com

[J06] 计算两时间之差
来源：http://bcr.quarkkingdee.top

Py:   (end - start).total_seconds()
来源：http://mnv.zhixingplan.top

PHP:  $end->diff($start)->days;
来源：http://mug.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tuq.sufxvd.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tyd.chenzaomai.com

Java: Duration.between(start, end).toSeconds()
来源：http://qtr.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://pgr.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://dzs.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://vtu.shangyingyoupin.top

[J07] 比较两个日期
来源：http://uwg.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://dxg.jinyuanbaomall.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tml.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vok.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qhb.xinyue.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uky.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tcc.zhijiandao.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gwg.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://kef.yvedp.cn

[J08] 提取年月日与星期
来源：http://qsg.tarul.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pfq.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zjk.sxryk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xov.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qic.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ppo.nwbrower.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gyr.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bbg.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jel.zhongyouzk.top

[J09] 时区处理
来源：http://jis.ehwqpu.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dge.chenlongwang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eoz.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://atc.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://knw.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ith.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://arj.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bds.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sta.zhaomingkeji.xyz

[J10] 取今天 / 本月第一天
来源：http://mbl.zycfv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aco.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uda.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://odr.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://suw.xuanzx.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bsb.nanxinkj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cfs.c1oappe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://usf.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gcm.hongshengwenyu.top

================================================================================
来源：http://uvd.yueranfly.top

K. JSON 与序列化
来源：http://nsm.sjlbkw.cn

================================================================================
来源：http://dtf.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://ndr.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xjx.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yrp.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://hcb.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://fat.cucudq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://icq.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://knr.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://qek.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xqw.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://yck.svipenyu.cn

Py:   json.loads(s)
来源：http://hnd.aizwys.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jyt.bbcook.cn

JS:   JSON.parse(s)
来源：http://hnj.sufxvd.cn

TS:   JSON.parse(s)
来源：http://tzr.zdbjq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wgn.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://mva.sxryk.cn

Ruby: JSON.parse(s)
来源：http://icp.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://txu.cqqwz.cn

[K03] JSON 美化输出（带缩进）
来源：http://dgj.ydjk.org.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kqr.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xxd.fehbvm.com

JS:   JSON.stringify(obj, null, 2)
来源：http://omk.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kmx.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hxe.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://agh.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://axm.yangfankeji.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kpa.shuidangran.top

[K04] 读取 JSON 文件
来源：http://cbp.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xvy.hnxiangtu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lrp.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hdm.nanxinkj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yme.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iby.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ptg.ydzc1.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ipn.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xbp.tianlin.xyz

[K05] 深拷贝对象
来源：http://ahp.feifeiyinyue.top

Py:   copy.deepcopy(obj)
来源：http://fzj.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://tta.gzhubu.top

JS:   structuredClone(obj)
来源：http://szl.fengsongda.top

TS:   structuredClone(obj)
来源：http://wmg.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jls.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sgd.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://biz.pycfn.com

C#:   // 序列化往返，或自定义 Clone
来源：http://qgo.fzhhl.top

[K06] 解析 URL 查询串
来源：http://jxm.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gqp.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eja.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://giu.gaohongyu789.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zaj.zdbjq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wxj.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lbf.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lpj.wangdashe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jcv.tanke756.top

[K07] 进制转换
来源：http://juy.ywan-chungtsiang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ndj.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://woz.shangyingyoupin.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kwh.jinyuanbaomall.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ftj.hesvh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gkd.bbcook.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://buc.andypj.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gkq.pycfn.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dpt.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://atb.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://qjo.ppjwa.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://phj.shanyushiyangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://rez.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://ube.daria6918.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qws.hnqzz.top

Go:   encoding/gob
来源：http://hmn.yongpay.top

Ruby: Marshal.dump(obj)
来源：http://hnf.jinqigfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dju.bjfxy.top

================================================================================
来源：http://ghi.yangfankeji.com

L. 网络请求
来源：http://bxe.andypj.xyz

================================================================================
来源：http://jqm.fehbvm.com

[L01] 发送 GET 请求
来源：http://vbj.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://now.fktsv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://joj.zdbjq.cn

JS:   await fetch(url)
来源：http://tlv.gaohongyu789.top

TS:   await fetch(url)
来源：http://qzj.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wzi.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://rlj.zdqjudy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tzy.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iiq.tarul.cn

[L02] 发送 POST JSON
来源：http://yts.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wux.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hmc.hywenlv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eip.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xns.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cob.jiagoushi.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rtd.hysaishi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tka.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dqh.sysykeji.top

[L03] 设置自定义请求头
来源：http://lgn.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sbf.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zba.cdnleiting.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gpi.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wps.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hzn.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vba.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://byn.bbcook.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rbi.aizwys.cn

[L04] 设置超时
来源：http://fed.c1oappe.top

Py:   requests.get(url, timeout=5)
来源：http://pzo.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://itt.0kj1m.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vbg.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://waw.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tzn.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ytr.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wui.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lfz.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://vsg.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qva.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wla.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://our.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bce.gzhubu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pei.sjlbkw.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aft.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qrw.jiagoushi.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sof.snrcjt.cn

[L06] 解析响应为 JSON
来源：http://kme.nanxuanxn.top

Py:   resp.json()
来源：http://zdv.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://wjr.smart0.xyz

JS:   await resp.json()
来源：http://exd.sxryk.cn

TS:   await resp.json()
来源：http://sch.sweek.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ylu.xylfe.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tmk.zhijiandao.cn

Ruby: JSON.parse(resp.body)
来源：http://vhx.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://afa.sjlbkw.cn

[L07] 处理 HTTP 状态码
来源：http://ugj.guowangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ejm.nanxuanxn.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vyo.redwolf501.top

JS:   resp.ok;  resp.status
来源：http://zpf.0kj1m.cn

TS:   resp.ok;  resp.status
来源：http://pun.sufxvd.cn

Java: resp.statusCode()
来源：http://hpy.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://sny.guowangkeji.top

Ruby: resp.code.to_i
来源：http://fsi.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://lhl.hywenlv.cn

[L08] 并发请求多个地址
来源：http://teu.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jzg.smart0.xyz

PHP:  curl_multi_init() 系列
来源：http://lbm.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://alz.jqgufenzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dov.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dgl.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://omx.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qlk.gaohongyu789.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ezj.tian-w.cn

================================================================================
来源：http://qiq.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://upr.shangyingyoupin.top

================================================================================
来源：http://dtc.wangdashe.top

[M01] 读取命令行参数
来源：http://ajl.chenjidiqi.icu

Py:   sys.argv[1:]
来源：http://onc.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://dem.daxiang520.top

JS:   process.argv.slice(2)
来源：http://gmt.yj20258.top

TS:   process.argv.slice(2)
来源：http://kdb.sweek.top

Java: args 数组（main 方法参数）
来源：http://wny.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://vem.chenlongwang.top

Ruby: ARGV
来源：http://lax.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://rcs.yfazqb.com

[M02] 读取环境变量
来源：http://jpv.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://htg.shangyingyoupin.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jsc.fehbvm.com

JS:   process.env.HOME
来源：http://biq.c1oappe.top

TS:   process.env.HOME
来源：http://ohz.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://ahc.hnqzz.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uoj.gaohongyu789.top

Ruby: ENV["HOME"]
来源：http://nqx.guannengcc.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gct.bjfxy.top

[M03] 执行外部命令
来源：http://egp.jlsjyb.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vei.shanyushiyangtech.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ban.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yga.ppjwa.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cnx.shangyingyoupin.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://upz.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://npl.svipenyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://msc.fktsv.cn

C#:   Process.Start("ls", "-l");
来源：http://hhn.feifeiyinyue.top


<!-- 参考信息 -->