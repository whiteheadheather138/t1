代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aas.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qws.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iql.kuanghao11.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fbh.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://srh.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gap.yuanzhike.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kso.jlsjyb.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://orz.fengsongda.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mou.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://ipz.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://izo.snrcjt.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cfo.gaohongyu789.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eax.haohaochexian.top

TS:   /error/gim
来源：http://mdr.yuanzhike.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nxs.zycfv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yen.zhongyouzk.top

Ruby: s.scan(/error/i)
来源：http://psa.epnwcf.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sli.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://zeo.yueranfly.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://usy.xylfe.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dmy.wangshuangyany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vur.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uwh.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uwl.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yty.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lqv.dianchejie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kuh.jyoumei.cn

================================================================================
来源：http://yji.jinyuanbaomall.cn

J. 日期与时间
来源：http://mbh.kuanghao11.cn

================================================================================
来源：http://dsk.hywenlv.cn

[J01] 获取当前时间
来源：http://ssb.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://shz.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qae.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://pek.guannengcc.top

TS:   new Date();  Date.now()
来源：http://jpb.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sry.xziqi.cn

Go:   time.Now()
来源：http://eaq.jlsjyb.cn

Ruby: Time.now
来源：http://hrt.xinyue.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yll.fktsv.cn

[J02] 格式化输出
来源：http://iap.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kbh.mhx1999.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dpa.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sxt.ivvv.top

TS:   d.toISOString()
来源：http://sad.cucudq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nhc.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kxv.ehwqpu.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hpp.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ecx.bjfxy.top

[J03] 字符串解析为日期
来源：http://zfh.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lwb.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yjo.zhaomingkeji.xyz

JS:   new Date("2024-01-02")
来源：http://ssp.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://rtx.zdbjq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dwv.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dmu.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://ogd.hfpthk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cwg.tian-w.cn

[J04] 时间戳与日期互转
来源：http://iph.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zwe.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eei.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hqb.yangfankeji.com

TS:   Math.floor(Date.now() / 1000)
来源：http://aup.zhaomingkeji.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xpw.guannengcc.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fjo.ppjwa.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://isb.daria6918.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ogm.ctjpmb.com

[J05] 时间加减（加 7 天）
来源：http://yor.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://jwh.9152youxi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cnn.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://elk.wangshuangyany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fcy.zhengqikj.top

Java: LocalDate.now().plusDays(7)
来源：http://lkr.pengpengdd.cyou

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tdj.gotoacloud.top

Ruby: Time.now + 7 * 86400
来源：http://txj.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://idn.hnqzz.top

[J06] 计算两时间之差
来源：http://tjr.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://tdl.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://aon.chenjidiqi.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rfc.epnwcf.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://esg.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://sni.jqgufenzy.top

Go:   end.Sub(start).Hours()
来源：http://zzu.shangyingyoupin.top

Ruby: end - start                 # 返回秒数
来源：http://zyx.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://wle.guannengcc.top

[J07] 比较两个日期
来源：http://mls.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://xqi.haohaochexian.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zlp.ydjk.org.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rgm.yongpay.top

TS:   d1.getTime() < d2.getTime()
来源：http://vtn.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pxb.ybcxt.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vko.zdbjq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tmo.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://qrv.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://msn.jqgfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ehn.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uik.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xeb.xziqi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://esx.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tmd.ppjwa.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://agn.uphjek.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rrc.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vlj.yfazqb.com

[J09] 时区处理
来源：http://veo.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dlz.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ivc.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mxh.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mlm.wangshuangyany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tot.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cvg.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uxg.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qcx.jyoumei.cn

[J10] 取今天 / 本月第一天
来源：http://xhi.kuanghao11.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gey.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eiq.shanyushiyangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dzx.yuanzhike.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ynz.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wil.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vhp.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nmv.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dcb.xuanzx.com

================================================================================
来源：http://lnj.chenzaomai.com

K. JSON 与序列化
来源：http://hyg.nanxuanxn.top

================================================================================
来源：http://nfi.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://kwm.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pru.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xue.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://gcd.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://nqn.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gqd.yj202588.top

Go:   json.Marshal(obj)
来源：http://ogo.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://fyx.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rsp.xingfuxueyuan.xyz

[K02] JSON 字符串转对象
来源：http://ovq.guannengcc.top

Py:   json.loads(s)
来源：http://tzf.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qfc.dashuyun.cn

JS:   JSON.parse(s)
来源：http://jye.yonumen.top

TS:   JSON.parse(s)
来源：http://mah.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mzm.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://tkf.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://pku.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oek.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://asy.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wov.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hbz.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nfl.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lga.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lsc.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gof.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://poe.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sro.bjfxy.top

[K04] 读取 JSON 文件
来源：http://ber.yj20258888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wnb.yongpay.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cwj.ivvv.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jtm.jlsjyb.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qyd.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jgi.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rpa.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qgf.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fpp.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://fbm.dianchejie.cn

Py:   copy.deepcopy(obj)
来源：http://cjx.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://bse.bbcook.cn

JS:   structuredClone(obj)
来源：http://lym.hcnkem.com

TS:   structuredClone(obj)
来源：http://dlm.feifeiyinyue.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mty.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oro.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yng.zhongyouzk.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kqt.bjfxy.top

[K06] 解析 URL 查询串
来源：http://kvy.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ejp.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://szv.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dld.chenjidiqi.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mgk.jinqigfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yom.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kqd.gotoacloud.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rju.yuanzhike.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gkj.gaohongyu789.top

[K07] 进制转换
来源：http://and.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://syl.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lig.zycfv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cvu.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kde.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hwi.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://glw.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cna.uphjek.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://upj.hesvh.cn

[K08] 二进制序列化（非 JSON）
来源：http://ejz.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://jfs.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uzc.yangfankeji.com

JS:   v8.serialize(obj)        // Node
来源：http://otk.birdmap.top

TS:   v8.serialize(obj)        // Node
来源：http://vos.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lvz.shanyushiyangkeji.top

Go:   encoding/gob
来源：http://hyi.tianlin.xyz

Ruby: Marshal.dump(obj)
来源：http://gwk.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://top.zhijiandao.cn

================================================================================
来源：http://fqm.jqgfzy.top

L. 网络请求
来源：http://dmw.hcnkem.com

================================================================================
来源：http://xjr.zhoulong.xyz

[L01] 发送 GET 请求
来源：http://jyv.sysykeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oyo.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zjb.ctjpmb.com

JS:   await fetch(url)
来源：http://kdm.dashuyun.cn

TS:   await fetch(url)
来源：http://eze.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gwe.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://vxp.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jlj.pengpengdd.cyou

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dro.xingfuxueyuan.xyz

[L02] 发送 POST JSON
来源：http://cpw.iojbl.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ies.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uxy.zdbjq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zgw.yueranfly.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kke.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mhc.bjfxy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xyl.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yml.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uyn.tianlin.xyz

[L03] 设置自定义请求头
来源：http://uta.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gzz.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vzt.jlsjyb.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://okv.gzhubu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cmu.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iwp.jlsjyb.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://usa.fanxiaobao.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://beu.xylfe.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bbi.bjfxy.top

[L04] 设置超时
来源：http://tsf.yuxming.cn

Py:   requests.get(url, timeout=5)
来源：http://jwj.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ahk.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bit.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uhd.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xkx.zhixingplan.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nvw.xuanzx.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://spt.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vkn.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://uvt.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xhg.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://osz.ybcxt.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wgp.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://psl.ctjpmb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://okn.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fcw.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nin.ydjk.org.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kjl.yvedp.cn

[L06] 解析响应为 JSON
来源：http://vgs.zhiwuduotai.top

Py:   resp.json()
来源：http://wbu.daxiang520.top

PHP:  json_decode($body, true);
来源：http://qfm.shzxlz.cn

JS:   await resp.json()
来源：http://srf.zycfv.cn

TS:   await resp.json()
来源：http://vxj.zhengqikj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wwl.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jnl.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://xdz.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uaa.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://dqo.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lsa.ywan-chungtsiang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lzo.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://fuq.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://her.jyoumei.cn

Java: resp.statusCode()
来源：http://sgz.jinqigufen.top

Go:   resp.StatusCode
来源：http://ncj.yonumen.top

Ruby: resp.code.to_i
来源：http://muw.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://fpu.xinyue.icu

[L08] 并发请求多个地址
来源：http://cde.tianlin.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xxg.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://lkx.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kda.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mbu.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jvm.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gdm.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jrc.zhoulong.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uzj.zdqjudy.top

================================================================================
来源：http://rfr.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://sju.jinghuilouyu.cn

================================================================================
来源：http://tei.sjlbkw.cn

[M01] 读取命令行参数
来源：http://bpm.fktsv.cn

Py:   sys.argv[1:]
来源：http://ztm.fehbvm.com

PHP:  $argv;  $argc;
来源：http://zud.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://bmg.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://gnv.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://lgu.ehwqpu.com

Go:   os.Args[1:]
来源：http://mbe.ydjk.org.cn

Ruby: ARGV
来源：http://ibh.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://rww.tianlin.xyz

[M02] 读取环境变量
来源：http://cjp.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://upa.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hbh.jianghu66.top

JS:   process.env.HOME
来源：http://fjr.ybcxt.top

TS:   process.env.HOME
来源：http://jfb.ybcxt.top

Java: System.getenv("HOME")
来源：http://bmo.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wup.meibo888.top

Ruby: ENV["HOME"]
来源：http://rgd.iojbl.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bpc.zhaomingkeji.xyz

[M03] 执行外部命令
来源：http://zqw.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xsu.svipenyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lmu.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://enb.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://unu.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xqq.guowangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://war.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://aos.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://hwu.daria6918.cn


<!-- 参考信息 -->