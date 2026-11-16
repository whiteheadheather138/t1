代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ywe.bjfxy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fje.hesvh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vij.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eka.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ntd.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rik.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rfk.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wxq.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://trg.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://ant.havefunace.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gkh.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tgb.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yys.nwbrower.top

TS:   /error/gim
来源：http://qsv.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zgz.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ytf.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://nxa.sweek.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rzn.guannengcc.top

[I08] 贪婪与非贪婪匹配
来源：http://bes.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hpf.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aiu.yj20258.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rjv.hywenlv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mfm.haohaochexian.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://auk.yangfankeji.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cvl.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cgh.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dkp.52xcode.cn

================================================================================
来源：http://jcr.cdnleiting.top

J. 日期与时间
来源：http://ldw.hesvh.cn

================================================================================
来源：http://sul.smart0.xyz

[J01] 获取当前时间
来源：http://iju.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fmm.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pfc.chenlongwang.top

JS:   new Date();  Date.now()
来源：http://hhx.guannengcc.top

TS:   new Date();  Date.now()
来源：http://xfo.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://smq.hysaishi.cn

Go:   time.Now()
来源：http://ezk.jianghu66.top

Ruby: Time.now
来源：http://nul.wangshuangyany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bxt.hnxiangtu.top

[J02] 格式化输出
来源：http://yxd.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bjr.smart0.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oqc.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yeq.fehbvm.com

TS:   d.toISOString()
来源：http://qlg.shuidangran.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://poq.nanxuanxn.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ffj.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nha.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bof.ydzc1.top

[J03] 字符串解析为日期
来源：http://fzz.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ybu.yueranfly.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dkh.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://mgv.cashguo.top

TS:   new Date("2024-01-02")
来源：http://sli.gogol.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jcg.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wsn.hnqzz.top

Ruby: Date.parse("2024-01-02")
来源：http://ikt.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mrz.0kj1m.cn

[J04] 时间戳与日期互转
来源：http://blt.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zxi.gotoacloud.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cit.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ewz.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sfz.dianchejie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rrc.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ujz.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jan.ctjpmb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bed.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://var.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://zcm.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://jvp.c1oappe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://osy.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dqm.jqgfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://vff.vehdjk.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vxe.jqgufenzy.top

Ruby: Time.now + 7 * 86400
来源：http://imb.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://udm.xinyue.icu

[J06] 计算两时间之差
来源：http://ofi.chenjidiqi.icu

Py:   (end - start).total_seconds()
来源：http://frr.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://lsn.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nna.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://anv.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jdj.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://awt.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://wmm.jlsjyb.cn

C#:   (end - start).TotalSeconds
来源：http://erh.yueranfly.top

[J07] 比较两个日期
来源：http://woi.hywenlv.cn

Py:   d1 < d2;  d1 == d2
来源：http://eex.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://udp.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://zuu.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://bvd.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://naz.jqgufenzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qab.tian-w.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vlc.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://uiq.yueranfly.top

[J08] 提取年月日与星期
来源：http://jit.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://efv.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://que.daxiang520.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ggq.mhx1999.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zyi.9152youxi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ify.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hrh.0kj1m.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://opw.sufxvd.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ads.0kj1m.cn

[J09] 时区处理
来源：http://ziz.daria6918.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vyb.jqgufenzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ymr.shanyushiyangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://upa.quarkkingdee.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tab.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xea.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kgz.fehbvm.com

Ruby: Time.now.getlocal("+08:00")
来源：http://hrz.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://woh.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://wyv.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wyl.sufxvd.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fcn.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dwz.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hmo.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wwi.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qke.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dik.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://egx.chenlongwang.top

================================================================================
来源：http://ncm.birdmap.top

K. JSON 与序列化
来源：http://mxj.shanyushiyangtech.top

================================================================================
来源：http://djn.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://uxx.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fyj.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gif.yangfankeji.com

JS:   JSON.stringify(obj)
来源：http://nah.xingfuxueyuan.xyz

TS:   JSON.stringify(obj)
来源：http://hzs.zhengqikj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ipo.cqqwz.cn

Go:   json.Marshal(obj)
来源：http://nru.xinyue.icu

Ruby: obj.to_json                                     // require "json"
来源：http://uzy.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qbf.c1oappe.top

[K02] JSON 字符串转对象
来源：http://pmj.hesvh.cn

Py:   json.loads(s)
来源：http://dhy.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bzj.zdbjq.cn

JS:   JSON.parse(s)
来源：http://hfq.sysykeji.top

TS:   JSON.parse(s)
来源：http://nzh.xinyue.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aaa.jyoumei.cn

Go:   json.Unmarshal(data, &v)
来源：http://brs.9152youxi.cn

Ruby: JSON.parse(s)
来源：http://akq.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vve.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://yco.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dmg.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tht.redwolf501.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zke.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vvm.jinghuilouyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fzh.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tzd.yangfankeji.com

Ruby: JSON.pretty_generate(obj)
来源：http://xrw.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://niv.shangyingyoupin.top

[K04] 读取 JSON 文件
来源：http://rhe.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dcp.yonumen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mki.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://toj.c1oappe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wve.zhaomingkeji.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aqe.dianchejie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hum.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://pak.meibo888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hkf.yonumen.top

[K05] 深拷贝对象
来源：http://lhr.aizwys.cn

Py:   copy.deepcopy(obj)
来源：http://yvq.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://jom.redwolf501.top

JS:   structuredClone(obj)
来源：http://gnb.hammf.cn

TS:   structuredClone(obj)
来源：http://zlo.0kj1m.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dby.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://esm.kuanghao11.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://olu.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://iut.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://vyt.jiagoushi.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tdk.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ots.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rxl.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gvf.hfpthk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ajp.xuetiantiany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gtk.chenlongwang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dym.ydjk.org.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://srx.ehwqpu.com

[K07] 进制转换
来源：http://ghi.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mgr.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nmo.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qzo.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kjc.ctjpmb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://txj.sjlbkw.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nez.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ghs.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gqh.tianlin.xyz

[K08] 二进制序列化（非 JSON）
来源：http://ulw.yueranfly.top

Py:   pickle.dumps(obj)
来源：http://ufn.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ici.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://ews.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://pxw.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jxx.tian-w.cn

Go:   encoding/gob
来源：http://vtc.xziqi.cn

Ruby: Marshal.dump(obj)
来源：http://ubi.wangshuangyany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jpm.hysaishi.cn

================================================================================
来源：http://apd.jqgufenzy.top

L. 网络请求
来源：http://bry.daxiang520.top

================================================================================
来源：http://jvt.zycfv.cn

[L01] 发送 GET 请求
来源：http://arz.yj20258.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pgv.zhengqikj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jtp.tanke756.top

JS:   await fetch(url)
来源：http://cts.sysykeji.top

TS:   await fetch(url)
来源：http://xtm.zycfv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rli.nanxuanxn.top

Go:   resp, err := http.Get(url)
来源：http://rfc.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ygm.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xcw.fktsv.cn

[L02] 发送 POST JSON
来源：http://akk.cucudq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://scu.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cks.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ule.yuxming.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cbk.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gio.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vuj.uphjek.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xav.bjfxy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://egd.ybcxt.top

[L03] 设置自定义请求头
来源：http://tiq.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://krh.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jwg.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yxj.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uuo.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bfc.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qii.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bka.xuetiantiany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fql.epnwcf.com

[L04] 设置超时
来源：http://pzw.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://fui.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yqj.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zux.hcnkem.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ybb.hesvh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://psf.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xnh.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fjm.hnqzz.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mig.shuidangran.top

[L05] 上传文件（multipart）
来源：http://jmd.fktsv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rcw.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dck.redwolf501.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hqd.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uvb.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rod.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ntt.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://csv.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tjj.shangyingyoupin.top

[L06] 解析响应为 JSON
来源：http://yys.xinyue.icu

Py:   resp.json()
来源：http://xop.guannengcc.top

PHP:  json_decode($body, true);
来源：http://aej.ydjk.org.cn

JS:   await resp.json()
来源：http://gav.sysykeji.top

TS:   await resp.json()
来源：http://unt.ehwqpu.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fdh.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qed.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://ajg.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gpe.xziqi.cn

[L07] 处理 HTTP 状态码
来源：http://sof.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fnz.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cfb.aibaodan.cn

JS:   resp.ok;  resp.status
来源：http://gpx.yonumen.top

TS:   resp.ok;  resp.status
来源：http://gfm.jyoumei.cn

Java: resp.statusCode()
来源：http://jvw.kuanghao11.cn

Go:   resp.StatusCode
来源：http://bmm.jqgfzy.top

Ruby: resp.code.to_i
来源：http://vnv.iojbl.cn

C#:   (int)resp.StatusCode
来源：http://bxx.jinyuanbaomall.cn

[L08] 并发请求多个地址
来源：http://wbs.jqgfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lhe.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://lcf.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hzu.ywan-chungtsiang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jcb.c1oappe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://enk.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lep.mhx1999.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kxx.ybcxt.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pjg.jinqigufen.top

================================================================================
来源：http://jgx.mhx1999.top

M. 命令行 / 进程 / 环境
来源：http://vpj.wangdashe.top

================================================================================
来源：http://iiz.cqqwz.cn

[M01] 读取命令行参数
来源：http://lfm.chenlongwang.top

Py:   sys.argv[1:]
来源：http://mrf.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://thh.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://twd.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://ejp.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://ywf.epnwcf.com

Go:   os.Args[1:]
来源：http://fvw.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://qri.iojbl.cn

C#:   args 数组（Main 方法参数）
来源：http://tmr.jinghuilouyu.cn

[M02] 读取环境变量
来源：http://jhm.gotoacloud.top

Py:   os.environ.get("HOME")
来源：http://plr.yanxiufei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://crl.feifeiyinyue.top

JS:   process.env.HOME
来源：http://xzq.ybcxt.top

TS:   process.env.HOME
来源：http://bgv.svipenyu.cn

Java: System.getenv("HOME")
来源：http://ipy.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bpf.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://mdy.nanxinkj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fku.hywenlv.cn

[M03] 执行外部命令
来源：http://wsh.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://szd.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://res.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mdb.meibo888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://aev.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jnk.gzhubu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xsg.jianghu66.top

Ruby: system("ls -l");  `ls -l`
来源：http://nzf.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://boh.xuanzx.com


<!-- 参考信息 -->