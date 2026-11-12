代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bxn.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://faa.quarkkingdee.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cry.dashuyun.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cvd.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://huy.zhoulong.xyz

[I07] 忽略大小写与多行模式
来源：http://dkv.52xcode.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iwm.fzhhl.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cxg.gotoacloud.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uio.jinghuilouyu.cn

TS:   /error/gim
来源：http://mzy.guowangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cuf.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ydk.meibo888.top

Ruby: s.scan(/error/i)
来源：http://zio.jinyuanbaomall.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ujx.tian-w.cn

[I08] 贪婪与非贪婪匹配
来源：http://vdl.jlsjyb.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tnd.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uke.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hos.aibaodan.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zih.feifeiyinyue.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kxf.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oqp.yfazqb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ijf.andypj.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mma.ydzc1.top

================================================================================
来源：http://fce.ybcxt.top

J. 日期与时间
来源：http://kiv.dianchejie.cn

================================================================================
来源：http://ycx.nanxuanxn.top

[J01] 获取当前时间
来源：http://gxb.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://ucs.gaohongyu789.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rhz.xylfe.cn

JS:   new Date();  Date.now()
来源：http://ysz.jqgufenzy.top

TS:   new Date();  Date.now()
来源：http://rgb.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cqu.tarul.cn

Go:   time.Now()
来源：http://fak.yuanzhike.top

Ruby: Time.now
来源：http://tho.hammf.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jza.yj20258.top

[J02] 格式化输出
来源：http://xcr.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xxy.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://omz.zhaomingkeji.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ahy.jqgufenzy.top

TS:   d.toISOString()
来源：http://jzp.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ely.jinyuanbaomall.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ojs.yvedp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gbb.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qnq.9152youxi.cn

[J03] 字符串解析为日期
来源：http://wbq.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hmi.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kmt.jinqigufen.top

JS:   new Date("2024-01-02")
来源：http://qbx.yfazqb.com

TS:   new Date("2024-01-02")
来源：http://ptj.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tdl.fanxiaobao.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cez.bbcook.cn

Ruby: Date.parse("2024-01-02")
来源：http://dbf.smart0.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pba.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://kib.yvedp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uli.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vcp.hcnkem.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://adg.shanyushiyangtech.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kkk.gaohongyu789.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rpv.c1oappe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vxl.fktsv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pav.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wzm.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://qgk.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://lop.bbcook.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ksq.svipenyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pbv.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ona.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://xsm.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xax.hongshengwenyu.top

Ruby: Time.now + 7 * 86400
来源：http://lkv.xuetiantiany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gpg.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://vtf.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://xma.ybcxt.top

PHP:  $end->diff($start)->days;
来源：http://kcj.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cjb.gzhubu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yot.pengpengdd.cyou

Java: Duration.between(start, end).toSeconds()
来源：http://mdw.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://eor.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://dcj.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://kgw.zhijiandao.cn

[J07] 比较两个日期
来源：http://mbg.hfpthk.cn

Py:   d1 < d2;  d1 == d2
来源：http://fzp.fzhhl.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xqj.yuxming.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rpd.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vgs.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bey.zhoulong.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nfs.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://nrl.shangyingyoupin.top

C#:   d1 < d2;  d1 == d2
来源：http://npx.316326.xyz

[J08] 提取年月日与星期
来源：http://rvw.hongshengwenyu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cyi.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tzq.snrcjt.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wax.gaohongyu789.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ddg.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zcz.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fzn.zdbjq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aqr.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kse.ywan-chungtsiang.top

[J09] 时区处理
来源：http://ejk.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tjz.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xdk.xuanzx.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hve.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lza.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://djs.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qdp.uphjek.com

Ruby: Time.now.getlocal("+08:00")
来源：http://oxi.tian-w.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qin.sufxvd.cn

[J10] 取今天 / 本月第一天
来源：http://wde.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://clu.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qyn.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://waz.cashguo.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qov.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bjt.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fyy.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gwn.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vid.jiagoushi.top

================================================================================
来源：http://tpv.ivvv.top

K. JSON 与序列化
来源：http://bvp.gaohongyu789.top

================================================================================
来源：http://fsd.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://qim.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tco.yongpay.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lww.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://jsf.xingfuxueyuan.xyz

TS:   JSON.stringify(obj)
来源：http://vdn.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tvn.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://fkg.yanxiufei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qmf.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://apa.yanxiufei.cn

[K02] JSON 字符串转对象
来源：http://gcx.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://ohx.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bon.redwolf501.top

JS:   JSON.parse(s)
来源：http://fui.fehbvm.com

TS:   JSON.parse(s)
来源：http://zod.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uiw.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://bas.vqdsnc.cn

Ruby: JSON.parse(s)
来源：http://ivs.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cim.pycfn.com

[K03] JSON 美化输出（带缩进）
来源：http://dey.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nxl.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cgz.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wqf.andypj.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://xaa.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cij.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://toy.jyoumei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mth.hesvh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cgf.fengsongda.top

[K04] 读取 JSON 文件
来源：http://wne.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dfx.jqgufenzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zfp.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xjy.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kuk.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mel.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zub.sufxvd.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jfq.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://drm.jiagoushi.top

[K05] 深拷贝对象
来源：http://afe.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://jgw.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://uiu.hammf.cn

JS:   structuredClone(obj)
来源：http://zls.52xcode.cn

TS:   structuredClone(obj)
来源：http://kfi.chenzaomai.com

Java: // 手写拷贝构造，或序列化往返
来源：http://pih.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jvh.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pof.hnqzz.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kng.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://xry.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hix.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ecq.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hyj.zhoulong.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jmc.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ooh.jiagoushi.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://miu.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://prr.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rmu.feifeiyinyue.top

[K07] 进制转换
来源：http://lcz.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iei.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yxo.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qzk.nwbrower.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nwf.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yyy.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uzi.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zqa.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://but.chenzaomai.com

[K08] 二进制序列化（非 JSON）
来源：http://lxw.shanyushiyangtech.top

Py:   pickle.dumps(obj)
来源：http://lvt.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://bie.feifeiyinyue.top

JS:   v8.serialize(obj)        // Node
来源：http://qlz.chenzaomai.com

TS:   v8.serialize(obj)        // Node
来源：http://juj.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jga.birdmap.top

Go:   encoding/gob
来源：http://bom.zycfv.cn

Ruby: Marshal.dump(obj)
来源：http://hyc.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jnw.shanyushiyangtech.top

================================================================================
来源：http://lij.hesvh.cn

L. 网络请求
来源：http://qac.iojbl.cn

================================================================================
来源：http://qdk.sysykeji.top

[L01] 发送 GET 请求
来源：http://ido.vqdsnc.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fam.daxiang520.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xmb.ybcxt.top

JS:   await fetch(url)
来源：http://jzz.zhiwuduotai.top

TS:   await fetch(url)
来源：http://xfs.havefunace.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://imr.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://ude.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://rvc.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ggg.fengsongda.top

[L02] 发送 POST JSON
来源：http://xlk.zhiwuduotai.top

Py:   requests.post(url, json={"a": 1})
来源：http://vxx.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hfv.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jig.zhijiandao.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mxy.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hbe.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qvx.shzxlz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://itt.guannengcc.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yvj.shuidangran.top

[L03] 设置自定义请求头
来源：http://jff.jinqigufen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mef.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xuv.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iqx.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fuj.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://egz.cashguo.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ywx.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dgx.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wqt.jinghuilouyu.cn

[L04] 设置超时
来源：http://yfj.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://aka.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lob.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://txq.jqgufenzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qwm.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mre.ywan-chungtsiang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hke.shzxlz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://evi.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lsx.redwolf501.top

[L05] 上传文件（multipart）
来源：http://dge.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xqq.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qyn.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nbr.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dax.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lef.52xcode.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ejt.zhongyouzk.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qkp.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://afc.sxryk.cn

[L06] 解析响应为 JSON
来源：http://qqg.52xcode.cn

Py:   resp.json()
来源：http://mhk.fehbvm.com

PHP:  json_decode($body, true);
来源：http://cfv.chenzaomai.com

JS:   await resp.json()
来源：http://wnd.feifeiyinyue.top

TS:   await resp.json()
来源：http://wyp.wangshuangyany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wbq.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hln.zhengqikj.top

Ruby: JSON.parse(resp.body)
来源：http://ear.nanxuanxn.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://elp.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://fxn.yueranfly.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jda.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sqq.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://rul.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://enq.hammf.cn

Java: resp.statusCode()
来源：http://hjs.ybcxt.top

Go:   resp.StatusCode
来源：http://mhe.fzhhl.top

Ruby: resp.code.to_i
来源：http://gvp.daxiang520.top

C#:   (int)resp.StatusCode
来源：http://our.svipenyu.cn

[L08] 并发请求多个地址
来源：http://mai.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jhb.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://xax.fanxiaobao.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hlv.hfpthk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ktn.jlsjyb.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uph.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cur.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tni.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nqq.jinyuanbaomall.cn

================================================================================
来源：http://whq.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://mmz.daxiang520.top

================================================================================
来源：http://udq.cashguo.top

[M01] 读取命令行参数
来源：http://zhi.shzxlz.cn

Py:   sys.argv[1:]
来源：http://rsi.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://eor.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://dsl.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://uia.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://ibu.dashuyun.cn

Go:   os.Args[1:]
来源：http://osh.fengsongda.top

Ruby: ARGV
来源：http://cnv.zdbjq.cn

C#:   args 数组（Main 方法参数）
来源：http://hxa.yonumen.top

[M02] 读取环境变量
来源：http://fex.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://rwq.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nkk.jyoumei.cn

JS:   process.env.HOME
来源：http://uic.dianchejie.cn

TS:   process.env.HOME
来源：http://izh.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://auo.xuetiantiany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ava.yangfankeji.com

Ruby: ENV["HOME"]
来源：http://son.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bcz.chenzaomai.com

[M03] 执行外部命令
来源：http://kal.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dtm.haohaochexian.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yje.gogol.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dfm.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://itz.shzxlz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wyh.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hdj.ywan-chungtsiang.top

Ruby: system("ls -l");  `ls -l`
来源：http://nju.jyoumei.cn

C#:   Process.Start("ls", "-l");
来源：http://kuf.shzxlz.cn

[M04] 获取当前工作目录
来源：http://cyp.yvedp.cn

Py:   os.getcwd()
来源：http://apv.zdqjudy.top

PHP:  getcwd();
来源：http://toi.jiagoushi.top

JS:   process.cwd()
来源：http://dcf.zdbjq.cn


<!-- 参考信息 -->