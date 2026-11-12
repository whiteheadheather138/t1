代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://zyz.aibaodan.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yvi.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vsp.havefunace.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://amr.ywan-chungtsiang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kqo.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lgy.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rgr.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qzs.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bpl.jinqigfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ngf.fanxiaobao.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ayq.cucudq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://efh.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cer.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://hye.ydzc1.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tpi.fzhhl.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vgi.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sso.zhiwuduotai.top

TS:   /error/gim
来源：http://tmg.cashguo.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tgi.aibaodan.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nxo.shangyingyoupin.top

Ruby: s.scan(/error/i)
来源：http://clz.shangyingyoupin.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bhc.meibo888.top

[I08] 贪婪与非贪婪匹配
来源：http://yah.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://irz.ywan-chungtsiang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ohu.chenlongwang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://deh.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aap.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vat.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://odq.wangshuangyany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mcb.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yas.gaohongyu789.top

================================================================================
来源：http://omv.zhijiandao.cn

J. 日期与时间
来源：http://wtf.gzhubu.top

================================================================================
来源：http://pvy.52xcode.cn

[J01] 获取当前时间
来源：http://hrt.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bas.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ihl.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://jov.snrcjt.cn

TS:   new Date();  Date.now()
来源：http://fdb.hnqzz.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xpk.cucudq.cn

Go:   time.Now()
来源：http://phz.fehbvm.com

Ruby: Time.now
来源：http://fmp.zhengqikj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zhm.redwolf501.top

[J02] 格式化输出
来源：http://ocj.xylfe.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ubd.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ozq.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://igz.ctjpmb.com

TS:   d.toISOString()
来源：http://lpl.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sdc.yangfankeji.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rpw.shzxlz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://crc.jqgfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wrj.sysykeji.top

[J03] 字符串解析为日期
来源：http://woc.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kgk.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jhz.birdmap.top

JS:   new Date("2024-01-02")
来源：http://saj.pycfn.com

TS:   new Date("2024-01-02")
来源：http://ruf.ydjk.org.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qrv.0kj1m.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lkt.quarkkingdee.top

Ruby: Date.parse("2024-01-02")
来源：http://tdq.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://apg.guannengcc.top

[J04] 时间戳与日期互转
来源：http://rta.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://goq.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kcx.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jdp.guannengcc.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pwa.cdnleiting.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ofv.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tui.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vyk.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rmr.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://dau.birdmap.top

Py:   now + timedelta(days=7)
来源：http://pbz.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pzc.xuetiantiany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cam.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xwb.ybcxt.top

Java: LocalDate.now().plusDays(7)
来源：http://box.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hry.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://xnq.jyoumei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gxr.xingfuxueyuan.xyz

[J06] 计算两时间之差
来源：http://pfv.jinyuanbaomall.cn

Py:   (end - start).total_seconds()
来源：http://zie.kuanghao11.cn

PHP:  $end->diff($start)->days;
来源：http://ymm.nwbrower.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://res.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iyn.feifeiyinyue.top

Java: Duration.between(start, end).toSeconds()
来源：http://vtk.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://wmw.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://otj.cashguo.top

C#:   (end - start).TotalSeconds
来源：http://myj.hnxiangtu.top

[J07] 比较两个日期
来源：http://ztt.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://nlt.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://upe.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://kjs.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://spr.zhongyouzk.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jfq.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://etq.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qmb.zhaomingkeji.xyz

C#:   d1 < d2;  d1 == d2
来源：http://rvp.iojbl.cn

[J08] 提取年月日与星期
来源：http://vmq.wangshuangyany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qtb.hnxiangtu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ung.tianlin.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gwb.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ntl.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ver.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fov.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xqn.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tsf.bbcook.cn

[J09] 时区处理
来源：http://gsw.yvedp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fzz.feifeiyinyue.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vib.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dsq.havefunace.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vrs.shanyushiyangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pra.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eyx.guowangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://akr.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fhw.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://wnu.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://iza.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jap.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vhc.cashguo.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xbn.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jml.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lof.c1oappe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oop.bbcook.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ygl.kuanghao11.cn

================================================================================
来源：http://gel.gzhubu.top

K. JSON 与序列化
来源：http://xhf.xziqi.cn

================================================================================
来源：http://bnr.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://jir.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xbq.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ukj.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://gco.birdmap.top

TS:   JSON.stringify(obj)
来源：http://enk.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kvf.yvedp.cn

Go:   json.Marshal(obj)
来源：http://cfb.zdqjudy.top

Ruby: obj.to_json                                     // require "json"
来源：http://rku.jqgfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://frm.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://ioj.hnxiangtu.top

Py:   json.loads(s)
来源：http://khc.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jec.sxryk.cn

JS:   JSON.parse(s)
来源：http://ybk.tian-w.cn

TS:   JSON.parse(s)
来源：http://qgb.cdnleiting.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ozr.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://cqm.hfpthk.cn

Ruby: JSON.parse(s)
来源：http://suf.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ina.xuanzx.com

[K03] JSON 美化输出（带缩进）
来源：http://ezw.gaohongyu789.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rjx.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dnc.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zpl.kuanghao11.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qul.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://stt.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ruo.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://hzc.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fma.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://dnt.yj20258888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mmr.jlsjyb.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wbr.shanyushiyangtech.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ptg.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rkj.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://exw.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gyh.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://moh.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dag.sweek.top

[K05] 深拷贝对象
来源：http://lir.fehbvm.com

Py:   copy.deepcopy(obj)
来源：http://ler.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://lzq.nwbrower.top

JS:   structuredClone(obj)
来源：http://whq.shuidangran.top

TS:   structuredClone(obj)
来源：http://asj.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://euk.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wrk.smart0.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hps.vqdsnc.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://avb.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://znt.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wvs.gaohongyu789.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://stj.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qkv.nanxuanxn.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://exv.svipenyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zrq.xziqi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pgu.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cnm.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://toz.zhongyouzk.top

[K07] 进制转换
来源：http://dnp.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qbc.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wip.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uvc.xuetiantiany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eil.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pzl.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gmj.vqdsnc.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ocq.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://khh.jianghu66.top

[K08] 二进制序列化（非 JSON）
来源：http://gae.dianchejie.cn

Py:   pickle.dumps(obj)
来源：http://uew.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://khs.epnwcf.com

JS:   v8.serialize(obj)        // Node
来源：http://tgr.zhaomingkeji.xyz

TS:   v8.serialize(obj)        // Node
来源：http://cxs.guannengcc.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ifp.pycfn.com

Go:   encoding/gob
来源：http://dlk.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://bwt.redwolf501.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zht.zdbjq.cn

================================================================================
来源：http://ubd.cqqwz.cn

L. 网络请求
来源：http://kcz.chenlongwang.top

================================================================================
来源：http://elv.fehbvm.com

[L01] 发送 GET 请求
来源：http://fly.yongpay.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gye.tanke756.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://axi.9152youxi.cn

JS:   await fetch(url)
来源：http://cse.hysaishi.cn

TS:   await fetch(url)
来源：http://oqu.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yda.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://zfl.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gjt.chenjidiqi.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pct.jqgfzy.top

[L02] 发送 POST JSON
来源：http://npu.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://fum.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nvt.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ihe.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lsi.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lrp.xylfe.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://amf.0kj1m.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zui.sysykeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qne.yj20258888.top

[L03] 设置自定义请求头
来源：http://sqj.sjlbkw.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ebk.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://htl.ywan-chungtsiang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wph.ydjk.org.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zzr.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xvz.ydjk.org.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gdd.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iyu.hfpthk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dwu.jinghuilouyu.cn

[L04] 设置超时
来源：http://ehm.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://enb.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://auw.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yso.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rzs.shangyingyoupin.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qug.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://obt.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yhv.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dms.52xcode.cn

[L05] 上传文件（multipart）
来源：http://zrs.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tpk.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://chg.yj20258.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://maq.guowangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://igi.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jmw.hammf.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vvc.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vnx.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cgx.zdbjq.cn

[L06] 解析响应为 JSON
来源：http://ddk.yj20258888.top

Py:   resp.json()
来源：http://rel.xziqi.cn

PHP:  json_decode($body, true);
来源：http://xhk.hnqzz.top

JS:   await resp.json()
来源：http://ooy.fengsongda.top

TS:   await resp.json()
来源：http://dra.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lqu.meibo888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sfb.pengpengdd.cyou

Ruby: JSON.parse(resp.body)
来源：http://dgx.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ldy.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://tmi.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ujy.ydjk.org.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://osg.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://mrc.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://jzj.ivvv.top

Java: resp.statusCode()
来源：http://qsz.xinyue.icu

Go:   resp.StatusCode
来源：http://msi.chenzaomai.com

Ruby: resp.code.to_i
来源：http://jhf.feifeiyinyue.top

C#:   (int)resp.StatusCode
来源：http://avp.haohaochexian.top

[L08] 并发请求多个地址
来源：http://kxa.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yva.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://ali.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tmt.hnqzz.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qik.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://huc.xuanzx.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://twf.yangfankeji.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hxm.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://prc.0kj1m.cn

================================================================================
来源：http://uvd.hnxiangtu.top

M. 命令行 / 进程 / 环境
来源：http://fga.aibaodan.cn

================================================================================
来源：http://ibw.yuxming.cn

[M01] 读取命令行参数
来源：http://mzj.hesvh.cn

Py:   sys.argv[1:]
来源：http://tsh.yongpay.top

PHP:  $argv;  $argc;
来源：http://xvl.sweek.top

JS:   process.argv.slice(2)
来源：http://cwl.hnqzz.top

TS:   process.argv.slice(2)
来源：http://yqr.0kj1m.cn

Java: args 数组（main 方法参数）
来源：http://qpo.zhijiandao.cn

Go:   os.Args[1:]
来源：http://wmz.fanxiaobao.xyz

Ruby: ARGV
来源：http://vuy.ctjpmb.com

C#:   args 数组（Main 方法参数）
来源：http://msg.jiagoushi.top

[M02] 读取环境变量
来源：http://tgm.epnwcf.com

Py:   os.environ.get("HOME")
来源：http://tur.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dav.jqgfzy.top

JS:   process.env.HOME
来源：http://wei.bbcook.cn

TS:   process.env.HOME
来源：http://hjv.jinqigufen.top

Java: System.getenv("HOME")
来源：http://dcu.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xqz.wangdashe.top

Ruby: ENV["HOME"]
来源：http://ngp.haohaochexian.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://koi.ehwqpu.com

[M03] 执行外部命令
来源：http://sfw.sufxvd.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://veg.pengpengdd.cyou

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rmj.zhengqikj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wbm.shangyingyoupin.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rsb.zdqjudy.top


<!-- 参考信息 -->