代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jzx.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tlq.cashguo.top

[I04] 正则替换
来源：http://rfm.jinqigufen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://njd.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ehd.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xro.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://fpk.tian-w.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iog.fengsongda.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rvi.hfpthk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://huu.yongpay.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ihx.jqgufenzy.top

[I05] 按正则拆分
来源：http://rrt.yj20258888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://egl.cqqwz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aqc.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://qdf.zdbjq.cn

TS:   s.split(/\s*,\s*/)
来源：http://aow.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://ply.gogol.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://okx.bjfxy.top

Ruby: s.split(/\s*,\s*/)
来源：http://dpi.yj20258888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vap.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dut.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mhs.vehdjk.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ges.tianlin.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wcw.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bmo.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gml.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blc.cqqwz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vxw.yueranfly.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ufh.nanxinkj.top

[I07] 忽略大小写与多行模式
来源：http://ton.bbcook.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dke.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rep.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mlg.hywenlv.cn

TS:   /error/gim
来源：http://cok.hnqzz.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xji.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mnq.jiagoushi.top

Ruby: s.scan(/error/i)
来源：http://idf.ivvv.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://scx.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://yne.daria6918.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fge.kuanghao11.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lwu.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lcs.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jmy.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cit.kuanghao11.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uev.jinqigfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zhn.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uod.9152youxi.cn

================================================================================
来源：http://pna.jinqigufen.top

J. 日期与时间
来源：http://nqk.jlsjyb.cn

================================================================================
来源：http://hnk.tanke756.top

[J01] 获取当前时间
来源：http://vwh.guannengcc.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xgt.tian-w.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://efv.iojbl.cn

JS:   new Date();  Date.now()
来源：http://cki.bjfxy.top

TS:   new Date();  Date.now()
来源：http://axw.316326.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://ibp.hywenlv.cn

Go:   time.Now()
来源：http://ugl.hongshengwenyu.top

Ruby: Time.now
来源：http://ltz.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tpb.uphjek.com

[J02] 格式化输出
来源：http://alj.aibaodan.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qoa.tianlin.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lmz.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://snc.cqqwz.cn

TS:   d.toISOString()
来源：http://cnx.tian-w.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zkh.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vrm.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ort.ydjk.org.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://muu.shanyushiyangkeji.top

[J03] 字符串解析为日期
来源：http://nsa.hnqzz.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gfs.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fbz.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://joh.sxryk.cn

TS:   new Date("2024-01-02")
来源：http://hdl.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://aat.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://syg.quarkkingdee.top

Ruby: Date.parse("2024-01-02")
来源：http://mfo.ppjwa.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yrp.redwolf501.top

[J04] 时间戳与日期互转
来源：http://ycg.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mgb.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://muy.wangdashe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pii.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://ksd.gotoacloud.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tbq.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kwd.andypj.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sim.svipenyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://brm.yonumen.top

[J05] 时间加减（加 7 天）
来源：http://nfn.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://sqt.fanxiaobao.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://shf.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bsc.yj20258888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xwx.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://iry.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rdt.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://jce.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://qwx.cheryme.top

[J06] 计算两时间之差
来源：http://jem.zhengqikj.top

Py:   (end - start).total_seconds()
来源：http://vcw.havefunace.top

PHP:  $end->diff($start)->days;
来源：http://ubw.yj20258888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kza.cashguo.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pog.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://fak.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://dgt.zhiwuduotai.top

Ruby: end - start                 # 返回秒数
来源：http://hxi.fanxiaobao.xyz

C#:   (end - start).TotalSeconds
来源：http://igs.nwbrower.top

[J07] 比较两个日期
来源：http://bpp.cqqwz.cn

Py:   d1 < d2;  d1 == d2
来源：http://enn.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://swk.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://uut.yongpay.top

TS:   d1.getTime() < d2.getTime()
来源：http://wds.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nev.quarkkingdee.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bqj.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nto.tianlin.xyz

C#:   d1 < d2;  d1 == d2
来源：http://osl.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://cks.yonumen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://epd.yongpay.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zre.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://scs.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ain.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zyb.yueranfly.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zjd.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yqf.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ceq.shuidangran.top

[J09] 时区处理
来源：http://wyj.tianlin.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xvf.daxiang520.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://moy.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kcz.yuxming.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nyl.sweek.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://woq.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://peb.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hny.yonumen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hoi.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://fgn.hywenlv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ytm.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mvj.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xko.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xjs.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tbb.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hxo.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mjy.jinqigfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fag.kuanghao11.cn

================================================================================
来源：http://fxs.wangshuangyany.cn

K. JSON 与序列化
来源：http://ekt.aizwys.cn

================================================================================
来源：http://xhu.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://knz.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://krs.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://whn.dianchejie.cn

JS:   JSON.stringify(obj)
来源：http://nwl.feifeiyinyue.top

TS:   JSON.stringify(obj)
来源：http://fmy.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jxt.zdqjudy.top

Go:   json.Marshal(obj)
来源：http://ypw.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://swc.vehdjk.com

C#:   JsonSerializer.Serialize(obj)
来源：http://bkr.zhijiandao.cn

[K02] JSON 字符串转对象
来源：http://mbe.yanxiufei.cn

Py:   json.loads(s)
来源：http://two.jqgufenzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qtl.haohaochexian.top

JS:   JSON.parse(s)
来源：http://bbp.ppjwa.cn

TS:   JSON.parse(s)
来源：http://ugp.sufxvd.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://emq.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://aoe.fengsongda.top

Ruby: JSON.parse(s)
来源：http://pvp.meibo888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kwn.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://wha.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ndi.feifeiyinyue.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fer.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hto.vqdsnc.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hmb.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mnr.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lpy.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://eoc.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fot.sjlbkw.cn

[K04] 读取 JSON 文件
来源：http://exn.yuanzhike.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://izk.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eqs.ehwqpu.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vvz.mhx1999.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sir.yangfankeji.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yse.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rzy.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rrs.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://huo.tianlin.xyz

[K05] 深拷贝对象
来源：http://rir.zdqjudy.top

Py:   copy.deepcopy(obj)
来源：http://hkn.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://gig.hesvh.cn

JS:   structuredClone(obj)
来源：http://ekj.zycfv.cn

TS:   structuredClone(obj)
来源：http://xzk.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://tuq.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kym.ydjk.org.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://szm.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lqt.cucudq.cn

[K06] 解析 URL 查询串
来源：http://vyp.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cyb.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qkc.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vtg.ehwqpu.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ywm.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oes.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://sow.hesvh.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bha.tian-w.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://amw.xinyue.icu

[K07] 进制转换
来源：http://npc.ybcxt.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xrh.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kza.svipenyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yba.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fzy.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lxl.tianlin.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wne.haohaochexian.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oqq.ydzc1.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://szw.zhaomingkeji.xyz

[K08] 二进制序列化（非 JSON）
来源：http://wkz.dashuyun.cn

Py:   pickle.dumps(obj)
来源：http://iox.meibo888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yxe.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://mkz.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://wlu.bjfxy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ulj.jlsjyb.cn

Go:   encoding/gob
来源：http://plh.sweek.top

Ruby: Marshal.dump(obj)
来源：http://rrx.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bip.sxryk.cn

================================================================================
来源：http://jzm.xingfuxueyuan.xyz

L. 网络请求
来源：http://srr.nwbrower.top

================================================================================
来源：http://kru.yj20258.top

[L01] 发送 GET 请求
来源：http://hta.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zvm.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vwe.vqdsnc.cn

JS:   await fetch(url)
来源：http://vah.jinqigfzy.top

TS:   await fetch(url)
来源：http://jti.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sto.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://kqm.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://dnq.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://flf.jqgfzy.top

[L02] 发送 POST JSON
来源：http://tqx.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://yut.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vul.gogol.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vua.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sid.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hww.yangfankeji.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yrb.ydzc1.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sbb.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vjy.ywan-chungtsiang.top

[L03] 设置自定义请求头
来源：http://lth.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qzc.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jfk.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qqi.zhengqikj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ckf.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://afp.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mfs.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kku.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hii.9152youxi.cn

[L04] 设置超时
来源：http://wqy.tian-w.cn

Py:   requests.get(url, timeout=5)
来源：http://ize.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kmn.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kal.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ped.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eeg.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aln.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cbs.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mdb.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://wba.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tiq.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rrf.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qsb.xinyue.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hop.chenjidiqi.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mcm.chenjidiqi.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ssr.xuanzx.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://afm.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nhs.sysykeji.top

[L06] 解析响应为 JSON
来源：http://jrq.ivvv.top

Py:   resp.json()
来源：http://qan.316326.xyz

PHP:  json_decode($body, true);
来源：http://ogz.nanxuanxn.top

JS:   await resp.json()
来源：http://urt.haohaochexian.top

TS:   await resp.json()
来源：http://qwu.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yeq.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mqj.sysykeji.top

Ruby: JSON.parse(resp.body)
来源：http://shc.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wza.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://iqd.nanxinkj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pwe.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rrq.chenlongwang.top

JS:   resp.ok;  resp.status
来源：http://cex.dianchejie.cn

TS:   resp.ok;  resp.status
来源：http://rqy.feifeiyinyue.top

Java: resp.statusCode()
来源：http://nva.guowangkeji.top

Go:   resp.StatusCode
来源：http://xvr.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://yao.zdbjq.cn

C#:   (int)resp.StatusCode
来源：http://tln.yuxming.cn

[L08] 并发请求多个地址
来源：http://upd.daxiang520.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://txp.quarkkingdee.top

PHP:  curl_multi_init() 系列
来源：http://kgu.aizwys.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dga.jinghuilouyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ghn.xziqi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://roq.52xcode.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jby.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://glj.fanxiaobao.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gej.cheryme.top

================================================================================
来源：http://mfd.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://kcs.guowangkeji.top

================================================================================
来源：http://xuw.vehdjk.com

[M01] 读取命令行参数
来源：http://sef.xuetiantiany.cn

Py:   sys.argv[1:]
来源：http://djz.hnxiangtu.top

PHP:  $argv;  $argc;
来源：http://lie.cucudq.cn

JS:   process.argv.slice(2)
来源：http://prp.aizwys.cn

TS:   process.argv.slice(2)
来源：http://kpj.zhixingplan.top

Java: args 数组（main 方法参数）
来源：http://hid.gaohongyu789.top

Go:   os.Args[1:]
来源：http://qid.tian-w.cn


<!-- 参考信息 -->