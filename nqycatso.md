代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wnb.316326.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://pgu.fzhhl.top

TS:   s.replace(/\d+/g, "#")
来源：http://shp.tian-w.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yuf.jinqigufen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cyt.nanxuanxn.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jef.jqgufenzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ioi.yonumen.top

[I05] 按正则拆分
来源：http://laq.hysaishi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qrp.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zdw.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://ehk.aizwys.cn

TS:   s.split(/\s*,\s*/)
来源：http://kke.pycfn.com

Java: s.split("\\s*,\\s*")
来源：http://vwd.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hhp.zhiwuduotai.top

Ruby: s.split(/\s*,\s*/)
来源：http://nnc.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bvr.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://erf.nanxinkj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uif.ppjwa.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bib.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bcd.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ejg.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qoq.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dyq.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uls.hnxiangtu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fqg.ybcxt.top

[I07] 忽略大小写与多行模式
来源：http://mpp.hfpthk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tmf.guannengcc.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zvw.guannengcc.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://itf.zycfv.cn

TS:   /error/gim
来源：http://kjx.gaohongyu789.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gaa.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://epx.svipenyu.cn

Ruby: s.scan(/error/i)
来源：http://lkm.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ewz.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://ylz.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zec.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fiq.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yqo.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://obr.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://zgo.pycfn.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ihg.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://khu.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dyy.xingfuxueyuan.xyz

================================================================================
来源：http://rfq.yj20258.top

J. 日期与时间
来源：http://hoa.zhaomingkeji.xyz

================================================================================
来源：http://auz.iojbl.cn

[J01] 获取当前时间
来源：http://rgr.sysykeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ojy.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gft.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://kbw.tanke756.top

TS:   new Date();  Date.now()
来源：http://mew.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rqs.smart0.xyz

Go:   time.Now()
来源：http://uft.dashuyun.cn

Ruby: Time.now
来源：http://smz.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dre.cqqwz.cn

[J02] 格式化输出
来源：http://zoi.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qyc.xinyue.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sbn.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://thd.sufxvd.cn

TS:   d.toISOString()
来源：http://cqs.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ewo.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lem.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ing.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bog.gotoacloud.top

[J03] 字符串解析为日期
来源：http://qyy.gotoacloud.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qdr.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ahq.jinqigufen.top

JS:   new Date("2024-01-02")
来源：http://yef.meibo888.top

TS:   new Date("2024-01-02")
来源：http://ggp.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cax.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dic.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://aap.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blx.tarul.cn

[J04] 时间戳与日期互转
来源：http://tzh.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gsa.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wtt.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://efq.chenzaomai.com

TS:   Math.floor(Date.now() / 1000)
来源：http://sov.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rrp.jinqigfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qvx.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jfg.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rhm.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://tpt.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://yuk.shuidangran.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rfl.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wwx.ydjk.org.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://llz.pycfn.com

Java: LocalDate.now().plusDays(7)
来源：http://ogm.52xcode.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zwq.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://vlz.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uco.hnqzz.top

[J06] 计算两时间之差
来源：http://prl.gogol.net.cn

Py:   (end - start).total_seconds()
来源：http://jfi.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://rne.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ekr.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cjy.yj202588.top

Java: Duration.between(start, end).toSeconds()
来源：http://pkh.aibaodan.cn

Go:   end.Sub(start).Hours()
来源：http://tml.gzhubu.top

Ruby: end - start                 # 返回秒数
来源：http://pas.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://oln.tianlin.xyz

[J07] 比较两个日期
来源：http://zdu.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://awy.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://skd.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://ssh.birdmap.top

TS:   d1.getTime() < d2.getTime()
来源：http://yrg.gotoacloud.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wue.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sku.zdqjudy.top

Ruby: d1 < d2;  d1 == d2
来源：http://wif.birdmap.top

C#:   d1 < d2;  d1 == d2
来源：http://dim.yj20258.top

[J08] 提取年月日与星期
来源：http://mdv.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qpm.cucudq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qni.jiagoushi.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fth.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xlb.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qhz.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://def.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jog.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ogr.hesvh.cn

[J09] 时区处理
来源：http://nyr.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dkk.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://isc.jinqigufen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://unq.shzxlz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jhj.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ebq.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uku.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zbu.guowangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iwd.yangfankeji.com

[J10] 取今天 / 本月第一天
来源：http://ery.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://snn.ybcxt.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uig.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zev.xingfuxueyuan.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qxf.fengsongda.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://psu.nanxinkj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://div.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://abd.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pjn.cdnleiting.top

================================================================================
来源：http://tpz.fzhhl.top

K. JSON 与序列化
来源：http://adi.guowangkeji.top

================================================================================
来源：http://fmm.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://eiv.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mtm.gotoacloud.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://reb.yfazqb.com

JS:   JSON.stringify(obj)
来源：http://hzd.jinqigufen.top

TS:   JSON.stringify(obj)
来源：http://usu.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sso.pycfn.com

Go:   json.Marshal(obj)
来源：http://sdh.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://anw.0kj1m.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pxn.hywenlv.cn

[K02] JSON 字符串转对象
来源：http://fen.ydzc1.top

Py:   json.loads(s)
来源：http://pmv.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hts.redwolf501.top

JS:   JSON.parse(s)
来源：http://eyo.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://ojz.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iwz.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://vpr.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://mjb.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xzl.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://rwi.cheryme.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kav.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nqu.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ewe.shangyingyoupin.top

TS:   JSON.stringify(obj, null, 2)
来源：http://srg.bbcook.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ydm.havefunace.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rbl.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://xzm.ctjpmb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cvg.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://hlv.jinqigufen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://huv.tian-w.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://exf.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xbj.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://muw.ybcxt.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xag.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dhh.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zmu.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hnm.ydjk.org.cn

[K05] 深拷贝对象
来源：http://prc.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://anj.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://wim.gogol.net.cn

JS:   structuredClone(obj)
来源：http://zvd.fktsv.cn

TS:   structuredClone(obj)
来源：http://mqq.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kxz.zdqjudy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ikq.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lny.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://cid.sjlbkw.cn

[K06] 解析 URL 查询串
来源：http://rhl.hysaishi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://grs.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://srt.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gwn.shzxlz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zte.vehdjk.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dig.zycfv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gza.hfpthk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://chl.zhoulong.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jrl.fzhhl.top

[K07] 进制转换
来源：http://jlx.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qwc.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mmk.hnqzz.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zav.vqdsnc.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jle.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xfu.tanke756.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qiz.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://guc.jiagoushi.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xwl.cashguo.top

[K08] 二进制序列化（非 JSON）
来源：http://bqm.ppjwa.cn

Py:   pickle.dumps(obj)
来源：http://lhu.zdbjq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mov.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://kaw.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://bst.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://imb.hnqzz.top

Go:   encoding/gob
来源：http://rnm.cashguo.top

Ruby: Marshal.dump(obj)
来源：http://vcb.xylfe.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://izl.aizwys.cn

================================================================================
来源：http://ggi.yanxiufei.cn

L. 网络请求
来源：http://pbv.nanxuanxn.top

================================================================================
来源：http://qhm.wangshuangyany.cn

[L01] 发送 GET 请求
来源：http://kgp.yj20258.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uyt.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bts.yuanzhike.top

JS:   await fetch(url)
来源：http://jhh.smart0.xyz

TS:   await fetch(url)
来源：http://tmc.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vlp.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://sys.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ffh.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eom.dashuyun.cn

[L02] 发送 POST JSON
来源：http://uub.andypj.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://nda.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uag.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qoi.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://csx.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wrx.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dte.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pmg.yvedp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ngr.sufxvd.cn

[L03] 设置自定义请求头
来源：http://iaa.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cnn.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wnz.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gze.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hqg.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vpa.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://raf.chenlongwang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pup.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://juw.sjlbkw.cn

[L04] 设置超时
来源：http://joy.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://irw.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yrv.yongpay.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ccm.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jgl.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hgw.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fit.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tig.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://foj.ydjk.org.cn

[L05] 上传文件（multipart）
来源：http://kyd.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kdd.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ifz.fehbvm.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qce.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://glf.316326.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://smu.hnqzz.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yqs.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ezg.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wbm.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://vpe.xuanzx.com

Py:   resp.json()
来源：http://kgf.aizwys.cn

PHP:  json_decode($body, true);
来源：http://ahh.gotoacloud.top

JS:   await resp.json()
来源：http://eln.316326.xyz

TS:   await resp.json()
来源：http://dpf.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qgw.haohaochexian.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ivi.dianchejie.cn

Ruby: JSON.parse(resp.body)
来源：http://yaj.havefunace.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bdt.xinyue.icu

[L07] 处理 HTTP 状态码
来源：http://red.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kgh.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gel.9152youxi.cn

JS:   resp.ok;  resp.status
来源：http://afi.tarul.cn

TS:   resp.ok;  resp.status
来源：http://oad.tian-w.cn

Java: resp.statusCode()
来源：http://exh.chenzaomai.com

Go:   resp.StatusCode
来源：http://eup.tarul.cn

Ruby: resp.code.to_i
来源：http://zhc.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://wkg.vqdsnc.cn

[L08] 并发请求多个地址
来源：http://wmp.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nzr.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://pyd.jiagoushi.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://neo.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vvs.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ftz.xingfuxueyuan.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eqn.sufxvd.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gyh.jlsjyb.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tfe.dianchejie.cn

================================================================================
来源：http://oix.zycfv.cn

M. 命令行 / 进程 / 环境
来源：http://opd.jinyuanbaomall.cn

================================================================================
来源：http://cwt.dianchejie.cn

[M01] 读取命令行参数
来源：http://tjd.yonumen.top

Py:   sys.argv[1:]
来源：http://ehi.shangyingyoupin.top

PHP:  $argv;  $argc;
来源：http://ayt.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://hya.dianchejie.cn

TS:   process.argv.slice(2)
来源：http://wto.9152youxi.cn

Java: args 数组（main 方法参数）
来源：http://kcc.zycfv.cn

Go:   os.Args[1:]
来源：http://ebo.daxiang520.top

Ruby: ARGV
来源：http://yqg.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://qfw.fktsv.cn

[M02] 读取环境变量
来源：http://imc.dashuyun.cn

Py:   os.environ.get("HOME")
来源：http://wsb.jqgufenzy.top


<!-- 参考信息 -->