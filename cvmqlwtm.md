代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://ccb.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pjs.yuxming.cn

JS:   s.split(/\s*,\s*/)
来源：http://ldc.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://ngq.fzhhl.top

Java: s.split("\\s*,\\s*")
来源：http://fmp.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eio.ivvv.top

Ruby: s.split(/\s*,\s*/)
来源：http://awt.xziqi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aup.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://guy.daria6918.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ujb.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pwr.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://acl.pengpengdd.cyou

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zxk.wangdashe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mep.vqdsnc.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://crx.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mmr.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zsz.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://jsa.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eri.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lcq.aizwys.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sot.ydjk.org.cn

TS:   /error/gim
来源：http://ule.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rch.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rid.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://tdk.smart0.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gqe.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://vpi.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://olz.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jmy.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://syc.kuanghao11.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eoi.smart0.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://vrf.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ovx.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yfl.jlsjyb.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jod.fzhhl.top

================================================================================
来源：http://szs.guowangkeji.top

J. 日期与时间
来源：http://prx.gotoacloud.top

================================================================================
来源：http://ccl.vqdsnc.cn

[J01] 获取当前时间
来源：http://epw.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wiq.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mkj.uphjek.com

JS:   new Date();  Date.now()
来源：http://alm.jlsjyb.cn

TS:   new Date();  Date.now()
来源：http://yeh.vqdsnc.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lpj.shuidangran.top

Go:   time.Now()
来源：http://inv.zhixingplan.top

Ruby: Time.now
来源：http://xhi.nwbrower.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://urs.tarul.cn

[J02] 格式化输出
来源：http://kto.daxiang520.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wjv.sysykeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wrn.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kjo.fzhhl.top

TS:   d.toISOString()
来源：http://jtx.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qnq.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hyv.sysykeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mhj.daxiang520.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mow.bjfxy.top

[J03] 字符串解析为日期
来源：http://eyu.ppjwa.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mci.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://phe.pycfn.com

JS:   new Date("2024-01-02")
来源：http://igy.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://dza.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://lsz.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mah.yanxiufei.cn

Ruby: Date.parse("2024-01-02")
来源：http://ixf.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kai.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://uwy.yj20258888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qoa.ydjk.org.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nzs.hammf.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jbh.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yad.jlsjyb.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nqv.chenzaomai.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xtl.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qiv.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ixa.nanxuanxn.top

[J05] 时间加减（加 7 天）
来源：http://jvb.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://ofq.cucudq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://owt.guannengcc.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gml.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yyh.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://odl.tarul.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://myf.xingfuxueyuan.xyz

Ruby: Time.now + 7 * 86400
来源：http://lkr.zhengqikj.top

C#:   DateTime.Now.AddDays(7)
来源：http://bie.c1oappe.top

[J06] 计算两时间之差
来源：http://oll.guannengcc.top

Py:   (end - start).total_seconds()
来源：http://lpf.yj20258888.top

PHP:  $end->diff($start)->days;
来源：http://zbm.aizwys.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://voc.gotoacloud.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://icm.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://bzk.aizwys.cn

Go:   end.Sub(start).Hours()
来源：http://ipf.wangdashe.top

Ruby: end - start                 # 返回秒数
来源：http://gvb.hnxiangtu.top

C#:   (end - start).TotalSeconds
来源：http://qrp.quarkkingdee.top

[J07] 比较两个日期
来源：http://ugf.cashguo.top

Py:   d1 < d2;  d1 == d2
来源：http://roc.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lsh.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://mjp.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://rja.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xcv.daxiang520.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fwz.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://ziz.gotoacloud.top

C#:   d1 < d2;  d1 == d2
来源：http://hnp.xuanzx.com

[J08] 提取年月日与星期
来源：http://yvd.zdqjudy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iur.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pne.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://grj.tian-w.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zoi.jinqigufen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zrq.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pns.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://doj.gzhubu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ajv.hongshengwenyu.top

[J09] 时区处理
来源：http://zvm.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ski.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tmn.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://epn.gzhubu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yar.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ivt.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baz.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wtz.shzxlz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kxz.havefunace.top

[J10] 取今天 / 本月第一天
来源：http://jcu.shuidangran.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pla.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ump.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zna.yonumen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://itc.quarkkingdee.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tod.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lxd.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wmj.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ezq.jlsjyb.cn

================================================================================
来源：http://ioa.vqdsnc.cn

K. JSON 与序列化
来源：http://jaf.yongpay.top

================================================================================
来源：http://zzp.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://ava.ctjpmb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zcm.jyoumei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://azr.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://fpi.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://mfz.cucudq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iwk.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://dup.jlsjyb.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nix.sysykeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gwb.aibaodan.cn

[K02] JSON 字符串转对象
来源：http://dfv.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://tdj.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ilb.yj202588.top

JS:   JSON.parse(s)
来源：http://amz.hnqzz.top

TS:   JSON.parse(s)
来源：http://oqz.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oiv.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://wzz.vehdjk.com

Ruby: JSON.parse(s)
来源：http://gtg.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ilo.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://hwl.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ann.ehwqpu.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cim.yueranfly.top

JS:   JSON.stringify(obj, null, 2)
来源：http://giz.ivvv.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pet.hnqzz.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rer.andypj.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mew.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://pjr.tanke756.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ecx.jianghu66.top

[K04] 读取 JSON 文件
来源：http://qgr.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tif.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kqg.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sfn.svipenyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://beu.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xdl.redwolf501.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qbl.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bwu.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hag.tarul.cn

[K05] 深拷贝对象
来源：http://ybk.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://dos.gogol.net.cn

PHP:  unserialize(serialize($obj));
来源：http://hui.xylfe.cn

JS:   structuredClone(obj)
来源：http://huh.andypj.xyz

TS:   structuredClone(obj)
来源：http://zob.hfpthk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tov.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ihk.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://flk.jqgufenzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://uxc.shzxlz.cn

[K06] 解析 URL 查询串
来源：http://eqi.fehbvm.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sgg.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ywx.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iko.redwolf501.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vsx.ydjk.org.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://haf.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kmg.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fwb.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xtl.jinqigufen.top

[K07] 进制转换
来源：http://hop.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wru.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ola.gaohongyu789.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sly.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fxr.zdqjudy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://efc.tanke756.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wad.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eup.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://awo.0kj1m.cn

[K08] 二进制序列化（非 JSON）
来源：http://spk.fktsv.cn

Py:   pickle.dumps(obj)
来源：http://ajl.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ybc.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://clq.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://cdw.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://snn.havefunace.top

Go:   encoding/gob
来源：http://bgj.c1oappe.top

Ruby: Marshal.dump(obj)
来源：http://kwf.zdbjq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gnq.mhx1999.top

================================================================================
来源：http://ahq.ydzc1.top

L. 网络请求
来源：http://app.tian-w.cn

================================================================================
来源：http://csz.sufxvd.cn

[L01] 发送 GET 请求
来源：http://vdn.gogol.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://olf.zhengqikj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dcr.hywenlv.cn

JS:   await fetch(url)
来源：http://gke.dashuyun.cn

TS:   await fetch(url)
来源：http://mmf.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nsb.316326.xyz

Go:   resp, err := http.Get(url)
来源：http://zqm.svipenyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wrp.zhijiandao.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gws.sufxvd.cn

[L02] 发送 POST JSON
来源：http://ijk.9152youxi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zhm.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wgz.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pel.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hac.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gsn.c1oappe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://trn.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jge.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ihz.smart0.xyz

[L03] 设置自定义请求头
来源：http://nvs.zhengqikj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://crv.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zyp.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://myi.yueranfly.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lij.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hiz.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://owz.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://onp.9152youxi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fag.hammf.cn

[L04] 设置超时
来源：http://skr.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://hpw.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eyh.tanke756.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rqy.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ovh.havefunace.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aos.xingfuxueyuan.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iwr.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://boe.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vkz.ppjwa.cn

[L05] 上传文件（multipart）
来源：http://qfl.nanxuanxn.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://muf.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gnh.9152youxi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gcn.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nbq.jinqigufen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://puh.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bpg.yvedp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://skp.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ckl.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://dhb.wangshuangyany.cn

Py:   resp.json()
来源：http://rrp.yanxiufei.cn

PHP:  json_decode($body, true);
来源：http://lsx.ybcxt.top

JS:   await resp.json()
来源：http://ney.zdbjq.cn

TS:   await resp.json()
来源：http://adi.bjfxy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qvs.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mkv.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://okf.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jlt.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://olm.kuanghao11.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nup.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cwk.yuxming.cn

JS:   resp.ok;  resp.status
来源：http://fxa.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://hlb.tarul.cn

Java: resp.statusCode()
来源：http://jlq.redwolf501.top

Go:   resp.StatusCode
来源：http://kzm.haohaochexian.top

Ruby: resp.code.to_i
来源：http://tpd.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://zwz.316326.xyz

[L08] 并发请求多个地址
来源：http://wmo.tanke756.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qzh.ppjwa.cn

PHP:  curl_multi_init() 系列
来源：http://lom.gaohongyu789.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xyo.ctjpmb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wnn.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ofb.andypj.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://acj.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sys.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tbm.nanxuanxn.top

================================================================================
来源：http://siz.ehwqpu.com

M. 命令行 / 进程 / 环境
来源：http://xzl.jinyuanbaomall.cn

================================================================================
来源：http://tgb.52xcode.cn

[M01] 读取命令行参数
来源：http://cbt.hnxiangtu.top

Py:   sys.argv[1:]
来源：http://gxy.gogol.net.cn

PHP:  $argv;  $argc;
来源：http://pfp.yonumen.top

JS:   process.argv.slice(2)
来源：http://raq.haohaochexian.top

TS:   process.argv.slice(2)
来源：http://nbw.cashguo.top

Java: args 数组（main 方法参数）
来源：http://izm.fengsongda.top

Go:   os.Args[1:]
来源：http://ugf.gotoacloud.top

Ruby: ARGV
来源：http://esy.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://yow.vehdjk.com

[M02] 读取环境变量
来源：http://drj.fktsv.cn

Py:   os.environ.get("HOME")
来源：http://iuz.zhoulong.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eli.sxryk.cn

JS:   process.env.HOME
来源：http://sne.ydjk.org.cn

TS:   process.env.HOME
来源：http://kxf.316326.xyz

Java: System.getenv("HOME")
来源：http://zcw.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://omc.zhongyouzk.top

Ruby: ENV["HOME"]
来源：http://ims.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ktw.tanke756.top

[M03] 执行外部命令
来源：http://fud.fanxiaobao.xyz


<!-- 参考信息 -->