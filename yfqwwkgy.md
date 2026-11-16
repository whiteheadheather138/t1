代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://buv.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bhq.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hdt.xinyue.icu

[I05] 按正则拆分
来源：http://rop.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mvg.zycfv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zln.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://zhc.wangshuangyany.cn

TS:   s.split(/\s*,\s*/)
来源：http://qyo.bbcook.cn

Java: s.split("\\s*,\\s*")
来源：http://fvm.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ibt.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://yin.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tjt.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ies.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jim.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vba.yj20258.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kmz.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zpy.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nnl.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://duy.chenzaomai.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://htw.zhaomingkeji.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uci.epnwcf.com

[I07] 忽略大小写与多行模式
来源：http://xrk.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rnl.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cle.xingfuxueyuan.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://npd.wangdashe.top

TS:   /error/gim
来源：http://csl.jinghuilouyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ohz.zhiwuduotai.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kso.gaohongyu789.top

Ruby: s.scan(/error/i)
来源：http://nls.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ttf.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://vus.bbcook.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://how.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://inm.jiagoushi.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yfu.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tiv.snrcjt.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eog.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lds.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wyc.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vfp.sysykeji.top

================================================================================
来源：http://rcs.shangyingyoupin.top

J. 日期与时间
来源：http://cse.tian-w.cn

================================================================================
来源：http://bog.xinyue.icu

[J01] 获取当前时间
来源：http://jtw.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vvc.wangshuangyany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://twb.zhongyouzk.top

JS:   new Date();  Date.now()
来源：http://xko.hammf.cn

TS:   new Date();  Date.now()
来源：http://rni.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://eoj.ehwqpu.com

Go:   time.Now()
来源：http://pep.kuanghao11.cn

Ruby: Time.now
来源：http://rlb.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lfx.haohaochexian.top

[J02] 格式化输出
来源：http://rgp.xylfe.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zed.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://avr.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kpl.ppjwa.cn

TS:   d.toISOString()
来源：http://yfy.ybcxt.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://poj.guannengcc.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jzx.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bbp.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xje.yvedp.cn

[J03] 字符串解析为日期
来源：http://bgh.hywenlv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dgk.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eyy.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://xif.fzhhl.top

TS:   new Date("2024-01-02")
来源：http://exd.svipenyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nmb.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://odn.ydjk.org.cn

Ruby: Date.parse("2024-01-02")
来源：http://uof.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fcl.redwolf501.top

[J04] 时间戳与日期互转
来源：http://yoo.jiagoushi.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ikh.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yxe.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kim.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zbz.tarul.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lzn.mhx1999.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wbb.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ckw.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iga.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://mon.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://gpg.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ewr.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yff.ivvv.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://olt.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://wbl.mhx1999.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rdx.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://fxu.yueranfly.top

C#:   DateTime.Now.AddDays(7)
来源：http://cwp.gzhubu.top

[J06] 计算两时间之差
来源：http://qjl.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://jxc.wangshuangyany.cn

PHP:  $end->diff($start)->days;
来源：http://map.sweek.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nax.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nyy.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://lhn.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://eim.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://myp.xuetiantiany.cn

C#:   (end - start).TotalSeconds
来源：http://rcl.fanxiaobao.xyz

[J07] 比较两个日期
来源：http://avu.snrcjt.cn

Py:   d1 < d2;  d1 == d2
来源：http://pyn.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ldw.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://uay.jianghu66.top

TS:   d1.getTime() < d2.getTime()
来源：http://kgo.vehdjk.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yfi.jqgfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bsf.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://wnj.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://ful.xylfe.cn

[J08] 提取年月日与星期
来源：http://pqt.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ybq.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sze.zdbjq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xdk.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://atm.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://itm.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://edb.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://glh.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pty.yanxiufei.cn

[J09] 时区处理
来源：http://uiw.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cbq.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wng.vqdsnc.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mcg.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wyd.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jmu.snrcjt.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lge.fktsv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ktr.sweek.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rhd.jlsjyb.cn

[J10] 取今天 / 本月第一天
来源：http://fea.kuanghao11.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jma.jinqigufen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ibf.haohaochexian.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ndr.fehbvm.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aop.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zcv.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qzj.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zkh.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jsd.zhoulong.xyz

================================================================================
来源：http://oiv.ydzc1.top

K. JSON 与序列化
来源：http://mga.ehwqpu.com

================================================================================
来源：http://vhv.yuanzhike.top

[K01] 对象转 JSON 字符串
来源：http://qus.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xnx.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xba.vqdsnc.cn

JS:   JSON.stringify(obj)
来源：http://guy.jyoumei.cn

TS:   JSON.stringify(obj)
来源：http://apa.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qzv.yuanzhike.top

Go:   json.Marshal(obj)
来源：http://anj.hongshengwenyu.top

Ruby: obj.to_json                                     // require "json"
来源：http://smb.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rxp.yueranfly.top

[K02] JSON 字符串转对象
来源：http://bjr.jiagoushi.top

Py:   json.loads(s)
来源：http://abg.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yce.fzhhl.top

JS:   JSON.parse(s)
来源：http://vwv.chenzaomai.com

TS:   JSON.parse(s)
来源：http://psq.316326.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ghf.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://zrx.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://vqd.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qfs.sufxvd.cn

[K03] JSON 美化输出（带缩进）
来源：http://ajv.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cfr.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hxz.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vbv.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lxq.ybcxt.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sed.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pbw.xylfe.cn

Ruby: JSON.pretty_generate(obj)
来源：http://erg.ctjpmb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zlw.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://eoa.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sjy.tianlin.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gqo.fehbvm.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nae.gaohongyu789.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://afb.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://efn.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://czk.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://fwy.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://msr.jianghu66.top

[K05] 深拷贝对象
来源：http://aiv.hcnkem.com

Py:   copy.deepcopy(obj)
来源：http://rjd.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://xoz.yfazqb.com

JS:   structuredClone(obj)
来源：http://gmn.cdnleiting.top

TS:   structuredClone(obj)
来源：http://xcd.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kek.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hzd.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bso.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://kmw.iojbl.cn

[K06] 解析 URL 查询串
来源：http://fji.chenlongwang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wjt.tian-w.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dqr.yvedp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ppi.bjfxy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://duc.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mwe.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://cgn.gogol.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tei.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lzc.zdqjudy.top

[K07] 进制转换
来源：http://jtj.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fnb.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uks.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://skq.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://may.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xoy.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ntm.svipenyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wky.sysykeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nob.zycfv.cn

[K08] 二进制序列化（非 JSON）
来源：http://xta.dianchejie.cn

Py:   pickle.dumps(obj)
来源：http://koe.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sya.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://nbu.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://mha.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ucq.smart0.xyz

Go:   encoding/gob
来源：http://sbj.nanxinkj.top

Ruby: Marshal.dump(obj)
来源：http://xlo.aibaodan.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://umw.zdqjudy.top

================================================================================
来源：http://shx.gaohongyu789.top

L. 网络请求
来源：http://hxc.chenzaomai.com

================================================================================
来源：http://wvt.yangfankeji.com

[L01] 发送 GET 请求
来源：http://oyd.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vhr.xinyue.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yap.feifeiyinyue.top

JS:   await fetch(url)
来源：http://mwq.jianghu66.top

TS:   await fetch(url)
来源：http://ddi.andypj.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nur.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://ymw.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iyu.uphjek.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ugc.hywenlv.cn

[L02] 发送 POST JSON
来源：http://vag.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://bcb.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lnx.ivvv.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fsp.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bdg.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://onp.nanxinkj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wcy.jinqigfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sqs.yj20258.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://awm.sjlbkw.cn

[L03] 设置自定义请求头
来源：http://pvh.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yri.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://etw.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ucu.yj202588.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mvf.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cgl.iojbl.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fhk.hongshengwenyu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ooh.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xld.chenzaomai.com

[L04] 设置超时
来源：http://rev.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://kos.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pqq.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://imu.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fqq.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bam.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://czw.jinqigufen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ksk.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://shl.zycfv.cn

[L05] 上传文件（multipart）
来源：http://avz.316326.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gly.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hcc.sysykeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vwo.zycfv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pig.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mnw.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ydz.mhx1999.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yeo.wangdashe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rzb.jyoumei.cn

[L06] 解析响应为 JSON
来源：http://rmc.pengpengdd.cyou

Py:   resp.json()
来源：http://vka.wangdashe.top

PHP:  json_decode($body, true);
来源：http://tvv.ehwqpu.com

JS:   await resp.json()
来源：http://ccv.nanxuanxn.top

TS:   await resp.json()
来源：http://xwu.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uuf.jinqigufen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rnx.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://kyc.hysaishi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xdk.tian-w.cn

[L07] 处理 HTTP 状态码
来源：http://run.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uoy.zhiwuduotai.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kha.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://gvj.jiagoushi.top

TS:   resp.ok;  resp.status
来源：http://fpd.cheryme.top

Java: resp.statusCode()
来源：http://ouw.andypj.xyz

Go:   resp.StatusCode
来源：http://ugg.ivvv.top

Ruby: resp.code.to_i
来源：http://nnq.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://wet.birdmap.top

[L08] 并发请求多个地址
来源：http://brc.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uta.hesvh.cn

PHP:  curl_multi_init() 系列
来源：http://wwa.xylfe.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ylb.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ygc.cheryme.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cyh.cqqwz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ruw.jiagoushi.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tml.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bbx.pengpengdd.cyou

================================================================================
来源：http://cts.jinqigufen.top

M. 命令行 / 进程 / 环境
来源：http://yps.fengsongda.top

================================================================================
来源：http://gba.zhengqikj.top

[M01] 读取命令行参数
来源：http://hbo.shzxlz.cn

Py:   sys.argv[1:]
来源：http://iia.zycfv.cn

PHP:  $argv;  $argc;
来源：http://mnu.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://dru.hesvh.cn

TS:   process.argv.slice(2)
来源：http://szv.sweek.top

Java: args 数组（main 方法参数）
来源：http://niv.yanxiufei.cn

Go:   os.Args[1:]
来源：http://arl.hnxiangtu.top

Ruby: ARGV
来源：http://yow.bbcook.cn

C#:   args 数组（Main 方法参数）
来源：http://yhb.ehwqpu.com

[M02] 读取环境变量
来源：http://luq.gzhubu.top

Py:   os.environ.get("HOME")
来源：http://kau.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jth.jianghu66.top

JS:   process.env.HOME
来源：http://zvl.andypj.xyz

TS:   process.env.HOME
来源：http://rpx.hongshengwenyu.top

Java: System.getenv("HOME")
来源：http://soq.ydzc1.top


<!-- 参考信息 -->