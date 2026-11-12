代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://egb.zhaomingkeji.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://npk.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wyq.epnwcf.com

[I05] 按正则拆分
来源：http://cqy.meibo888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://maw.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xpn.yvedp.cn

JS:   s.split(/\s*,\s*/)
来源：http://zhm.hywenlv.cn

TS:   s.split(/\s*,\s*/)
来源：http://vzl.sweek.top

Java: s.split("\\s*,\\s*")
来源：http://mmn.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lbd.wangshuangyany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kuy.zhiwuduotai.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xta.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qfv.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ebi.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nbg.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kuu.birdmap.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yph.epnwcf.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fag.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nlr.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rxo.yueranfly.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fzz.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://jyx.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mkp.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zoh.jinqigfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pnq.ywan-chungtsiang.top

TS:   /error/gim
来源：http://yhm.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oys.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://asq.cashguo.top

Ruby: s.scan(/error/i)
来源：http://qho.daria6918.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pjd.wangshuangyany.cn

[I08] 贪婪与非贪婪匹配
来源：http://llr.yj20258.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rwk.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jcp.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://woh.hfpthk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ema.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ymz.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yph.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://amw.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mje.iojbl.cn

================================================================================
来源：http://rmd.chenjidiqi.icu

J. 日期与时间
来源：http://smd.meibo888.top

================================================================================
来源：http://nhe.xylfe.cn

[J01] 获取当前时间
来源：http://nfm.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wcv.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://llc.yj20258888.top

JS:   new Date();  Date.now()
来源：http://qvr.ppjwa.cn

TS:   new Date();  Date.now()
来源：http://lua.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mjy.shangyingyoupin.top

Go:   time.Now()
来源：http://wko.shzxlz.cn

Ruby: Time.now
来源：http://mjw.mhx1999.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gfp.uphjek.com

[J02] 格式化输出
来源：http://ivs.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://irp.bjfxy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gyn.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yha.hysaishi.cn

TS:   d.toISOString()
来源：http://awt.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dih.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uqc.ehwqpu.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ebd.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qfg.ppjwa.cn

[J03] 字符串解析为日期
来源：http://rej.sysykeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qwy.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wyw.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://njq.nwbrower.top

TS:   new Date("2024-01-02")
来源：http://zoc.tarul.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xps.hfpthk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gwp.vehdjk.com

Ruby: Date.parse("2024-01-02")
来源：http://jyd.yj20258888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iek.sxryk.cn

[J04] 时间戳与日期互转
来源：http://efw.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://djm.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://brd.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eud.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://fuj.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://txy.hnqzz.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zis.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mxu.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uqn.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://kap.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://cuy.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://gqr.yueranfly.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nnk.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qbr.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://lpm.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://enp.shangyingyoupin.top

Ruby: Time.now + 7 * 86400
来源：http://kvx.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://mgm.redwolf501.top

[J06] 计算两时间之差
来源：http://mrv.yfazqb.com

Py:   (end - start).total_seconds()
来源：http://nps.ivvv.top

PHP:  $end->diff($start)->days;
来源：http://mcv.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vrj.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wfa.yueranfly.top

Java: Duration.between(start, end).toSeconds()
来源：http://lrd.cqqwz.cn

Go:   end.Sub(start).Hours()
来源：http://qvd.fanxiaobao.xyz

Ruby: end - start                 # 返回秒数
来源：http://dsv.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://kpr.chenzaomai.com

[J07] 比较两个日期
来源：http://dls.jyoumei.cn

Py:   d1 < d2;  d1 == d2
来源：http://lzq.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dje.tanke756.top

JS:   d1.getTime() < d2.getTime()
来源：http://toc.zhiwuduotai.top

TS:   d1.getTime() < d2.getTime()
来源：http://zou.yongpay.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ucc.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qxk.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://oed.ywan-chungtsiang.top

C#:   d1 < d2;  d1 == d2
来源：http://nzy.shanyushiyangkeji.top

[J08] 提取年月日与星期
来源：http://nyn.uphjek.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ubt.gzhubu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ypt.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ogh.zdbjq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rbk.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zen.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vgz.nwbrower.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uvg.shangyingyoupin.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ufy.shangyingyoupin.top

[J09] 时区处理
来源：http://jrf.bjfxy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://msy.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jga.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://giw.aibaodan.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qku.nanxinkj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://prk.yongpay.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gtu.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kuv.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dst.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://wmx.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bnx.kuanghao11.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://raj.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://prm.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://upp.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rnq.yueranfly.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ppc.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://poi.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fln.zhiwuduotai.top

================================================================================
来源：http://xsy.andypj.xyz

K. JSON 与序列化
来源：http://aef.ydjk.org.cn

================================================================================
来源：http://lag.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://etx.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zye.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fkm.fengsongda.top

JS:   JSON.stringify(obj)
来源：http://hch.fktsv.cn

TS:   JSON.stringify(obj)
来源：http://oky.zdbjq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ole.yueranfly.top

Go:   json.Marshal(obj)
来源：http://dcr.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wph.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hhc.yuxming.cn

[K02] JSON 字符串转对象
来源：http://ich.yfazqb.com

Py:   json.loads(s)
来源：http://vep.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nnk.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://gei.hcnkem.com

TS:   JSON.parse(s)
来源：http://vev.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://krb.fzhhl.top

Go:   json.Unmarshal(data, &v)
来源：http://mhl.hammf.cn

Ruby: JSON.parse(s)
来源：http://gyh.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vsf.yangfankeji.com

[K03] JSON 美化输出（带缩进）
来源：http://mff.yj20258.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fxr.hongshengwenyu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sxx.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wvj.hfpthk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zdb.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tte.yangfankeji.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rgn.shzxlz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xjc.gotoacloud.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xah.epnwcf.com

[K04] 读取 JSON 文件
来源：http://wsm.dianchejie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://knb.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jtm.chenjidiqi.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pxn.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gez.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://klc.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ckb.jqgfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tux.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tnu.jinqigfzy.top

[K05] 深拷贝对象
来源：http://jnb.jqgufenzy.top

Py:   copy.deepcopy(obj)
来源：http://byp.cqqwz.cn

PHP:  unserialize(serialize($obj));
来源：http://dyj.havefunace.top

JS:   structuredClone(obj)
来源：http://eco.yanxiufei.cn

TS:   structuredClone(obj)
来源：http://pxd.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pca.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zwl.316326.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gpr.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kwo.chenjidiqi.icu

[K06] 解析 URL 查询串
来源：http://qwq.feifeiyinyue.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jtl.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rxc.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://adz.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ppq.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pof.jiagoushi.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bkp.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fqs.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ewh.jinqigufen.top

[K07] 进制转换
来源：http://fyj.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gnv.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mwt.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qvj.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zoq.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mco.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://imh.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://twr.jqgufenzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ohd.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://hyb.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://nyh.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qsw.xuanzx.com

JS:   v8.serialize(obj)        // Node
来源：http://bnx.mhx1999.top

TS:   v8.serialize(obj)        // Node
来源：http://ewq.jinghuilouyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gfw.quarkkingdee.top

Go:   encoding/gob
来源：http://cuz.zycfv.cn

Ruby: Marshal.dump(obj)
来源：http://crc.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yfk.ehwqpu.com

================================================================================
来源：http://xru.jinqigfzy.top

L. 网络请求
来源：http://ghk.vehdjk.com

================================================================================
来源：http://lkt.yj202588.top

[L01] 发送 GET 请求
来源：http://fsc.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xsc.quarkkingdee.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mox.guannengcc.top

JS:   await fetch(url)
来源：http://gzo.zhoulong.xyz

TS:   await fetch(url)
来源：http://dnx.zdbjq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ner.xinyue.icu

Go:   resp, err := http.Get(url)
来源：http://ojl.0kj1m.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bjn.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ziq.bbcook.cn

[L02] 发送 POST JSON
来源：http://asv.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://alz.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tjf.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ukt.ydjk.org.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eca.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ogb.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gww.vehdjk.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hgy.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qjo.vehdjk.com

[L03] 设置自定义请求头
来源：http://qxa.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://klz.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eao.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tox.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mzw.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://frj.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gba.dianchejie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kji.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cey.ppjwa.cn

[L04] 设置超时
来源：http://nqj.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://jvg.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fin.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ond.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tkm.jianghu66.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dws.c1oappe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yrg.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://erv.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pzf.zycfv.cn

[L05] 上传文件（multipart）
来源：http://amv.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ipm.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vxr.wangdashe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bfd.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://una.fehbvm.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gfr.jiagoushi.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ask.yvedp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bjp.52xcode.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mov.zhoulong.xyz

[L06] 解析响应为 JSON
来源：http://vet.quarkkingdee.top

Py:   resp.json()
来源：http://obm.epnwcf.com

PHP:  json_decode($body, true);
来源：http://med.hammf.cn

JS:   await resp.json()
来源：http://xqd.0kj1m.cn

TS:   await resp.json()
来源：http://bpw.316326.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wqt.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rhp.vehdjk.com

Ruby: JSON.parse(resp.body)
来源：http://pwg.zdqjudy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bqe.chenjidiqi.icu

[L07] 处理 HTTP 状态码
来源：http://oxc.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oaj.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dlu.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://hut.pycfn.com

TS:   resp.ok;  resp.status
来源：http://yzi.hfpthk.cn

Java: resp.statusCode()
来源：http://hyx.cheryme.top

Go:   resp.StatusCode
来源：http://crm.tian-w.cn

Ruby: resp.code.to_i
来源：http://xyw.ivvv.top

C#:   (int)resp.StatusCode
来源：http://weq.jlsjyb.cn

[L08] 并发请求多个地址
来源：http://nsq.hammf.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pqd.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://ewh.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qin.gzhubu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ixo.hammf.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xqn.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rtu.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ehy.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wtq.yvedp.cn

================================================================================
来源：http://naj.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://qsd.nwbrower.top

================================================================================
来源：http://xad.chenlongwang.top

[M01] 读取命令行参数
来源：http://wkz.tian-w.cn

Py:   sys.argv[1:]
来源：http://txk.zhengqikj.top

PHP:  $argv;  $argc;
来源：http://rpz.smart0.xyz

JS:   process.argv.slice(2)
来源：http://gfb.hfpthk.cn

TS:   process.argv.slice(2)
来源：http://mye.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://odq.yangfankeji.com

Go:   os.Args[1:]
来源：http://hey.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://zpc.xuetiantiany.cn

C#:   args 数组（Main 方法参数）
来源：http://pyl.guannengcc.top

[M02] 读取环境变量
来源：http://cyk.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://ckl.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ree.jiagoushi.top

JS:   process.env.HOME
来源：http://zgv.bjfxy.top

TS:   process.env.HOME
来源：http://cqy.sufxvd.cn

Java: System.getenv("HOME")
来源：http://aox.zhengqikj.top


<!-- 参考信息 -->