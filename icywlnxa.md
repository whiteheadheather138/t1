代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lmp.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://dkt.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://cee.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://gxq.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://thg.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bpt.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wia.zhengqikj.top

[I05] 按正则拆分
来源：http://wuf.sweek.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ews.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tdr.cashguo.top

JS:   s.split(/\s*,\s*/)
来源：http://tnv.yj20258888.top

TS:   s.split(/\s*,\s*/)
来源：http://wse.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://goh.hnqzz.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ckt.9152youxi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://quz.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ore.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uay.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qer.tianlin.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mkp.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://apy.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vxn.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vil.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mva.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mct.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://txu.gaohongyu789.top

[I07] 忽略大小写与多行模式
来源：http://ots.shuidangran.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vis.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wnp.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wjh.xylfe.cn

TS:   /error/gim
来源：http://azn.jyoumei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fsy.hammf.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vfk.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://hbc.jiagoushi.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yvt.jiagoushi.top

[I08] 贪婪与非贪婪匹配
来源：http://yvs.yuanzhike.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rbm.zhengqikj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rag.shzxlz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nxd.sjlbkw.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cye.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hzi.zhixingplan.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ibm.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kmd.birdmap.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aoq.zdbjq.cn

================================================================================
来源：http://twp.xziqi.cn

J. 日期与时间
来源：http://khn.shanyushiyangkeji.top

================================================================================
来源：http://ulz.sjlbkw.cn

[J01] 获取当前时间
来源：http://isp.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://sfl.ydzc1.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://msa.iojbl.cn

JS:   new Date();  Date.now()
来源：http://qxk.hywenlv.cn

TS:   new Date();  Date.now()
来源：http://jik.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://aya.gogol.net.cn

Go:   time.Now()
来源：http://sae.yfazqb.com

Ruby: Time.now
来源：http://maw.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://omm.mhx1999.top

[J02] 格式化输出
来源：http://kvi.xuanzx.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ypc.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hcv.xinyue.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nuc.vehdjk.com

TS:   d.toISOString()
来源：http://tsq.0kj1m.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bzj.xingfuxueyuan.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sli.vqdsnc.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aut.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lnz.cdnleiting.top

[J03] 字符串解析为日期
来源：http://fwi.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rnk.haohaochexian.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cfd.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://std.jlsjyb.cn

TS:   new Date("2024-01-02")
来源：http://avz.hnqzz.top

Java: LocalDate.parse("2024-01-02")
来源：http://gxs.jlsjyb.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nxl.yongpay.top

Ruby: Date.parse("2024-01-02")
来源：http://mjz.uphjek.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zzj.meibo888.top

[J04] 时间戳与日期互转
来源：http://okl.yfazqb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jkg.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rts.zhijiandao.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lsi.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://dre.zhoulong.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gum.jyoumei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mse.tanke756.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iue.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kts.hcnkem.com

[J05] 时间加减（加 7 天）
来源：http://rgc.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://afv.yuanzhike.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ocy.birdmap.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qtf.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://svd.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://khu.yj20258.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hoj.zhaomingkeji.xyz

Ruby: Time.now + 7 * 86400
来源：http://asd.nwbrower.top

C#:   DateTime.Now.AddDays(7)
来源：http://nmh.havefunace.top

[J06] 计算两时间之差
来源：http://iwf.yuanzhike.top

Py:   (end - start).total_seconds()
来源：http://bfn.wangshuangyany.cn

PHP:  $end->diff($start)->days;
来源：http://bam.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uig.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vpb.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://ale.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://phm.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://jsd.0kj1m.cn

C#:   (end - start).TotalSeconds
来源：http://fwh.ydjk.org.cn

[J07] 比较两个日期
来源：http://uqm.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://cyu.sweek.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nzb.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sml.xingfuxueyuan.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://vya.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lfh.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bhf.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://agc.nwbrower.top

C#:   d1 < d2;  d1 == d2
来源：http://jpu.redwolf501.top

[J08] 提取年月日与星期
来源：http://mof.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pef.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sum.cucudq.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pym.meibo888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kse.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gth.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jgi.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mcl.9152youxi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qgt.sjlbkw.cn

[J09] 时区处理
来源：http://ogx.sysykeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yib.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mct.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://twa.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uhr.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ssg.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lau.chenjidiqi.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://cer.tianlin.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ibi.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://xqp.yj20258888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ppr.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://njk.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cps.wangdashe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cam.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rkw.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fuy.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xla.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cnw.zhengqikj.top

================================================================================
来源：http://ewy.bbcook.cn

K. JSON 与序列化
来源：http://ysk.chenzaomai.com

================================================================================
来源：http://qrv.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://mbw.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vwt.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eor.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://rbq.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://bwn.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dyr.yfazqb.com

Go:   json.Marshal(obj)
来源：http://mgu.yongpay.top

Ruby: obj.to_json                                     // require "json"
来源：http://ysq.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://eld.guannengcc.top

[K02] JSON 字符串转对象
来源：http://jhv.sjlbkw.cn

Py:   json.loads(s)
来源：http://tow.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uii.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://rsy.cqqwz.cn

TS:   JSON.parse(s)
来源：http://iki.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uyh.zdbjq.cn

Go:   json.Unmarshal(data, &v)
来源：http://wfc.haohaochexian.top

Ruby: JSON.parse(s)
来源：http://rdp.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ptv.nanxuanxn.top

[K03] JSON 美化输出（带缩进）
来源：http://ofv.jlsjyb.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kzc.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sbq.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sxi.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pqb.c1oappe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nbv.gaohongyu789.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://irv.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://wdg.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gbq.vehdjk.com

[K04] 读取 JSON 文件
来源：http://qpz.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tad.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qce.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hfg.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uah.hnxiangtu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vaw.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fsa.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ooz.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://efc.ywan-chungtsiang.top

[K05] 深拷贝对象
来源：http://adc.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://fwq.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://kya.epnwcf.com

JS:   structuredClone(obj)
来源：http://urz.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://rrh.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vvz.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://muz.smart0.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gfh.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fjz.gzhubu.top

[K06] 解析 URL 查询串
来源：http://kjb.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lso.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qrn.jyoumei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zjq.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pua.yongpay.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mdo.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yfz.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fut.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tnj.quarkkingdee.top

[K07] 进制转换
来源：http://fly.ybcxt.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://miq.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ccn.xinyue.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fzp.aibaodan.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oqe.ybcxt.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://utq.jqgfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mas.yueranfly.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gww.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jiu.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://kmg.pycfn.com

Py:   pickle.dumps(obj)
来源：http://ifo.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qiv.xziqi.cn

JS:   v8.serialize(obj)        // Node
来源：http://bdt.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://ozx.chenjidiqi.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lhv.gzhubu.top

Go:   encoding/gob
来源：http://zzd.zhaomingkeji.xyz

Ruby: Marshal.dump(obj)
来源：http://uqe.hesvh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gpj.jiagoushi.top

================================================================================
来源：http://ocj.zdqjudy.top

L. 网络请求
来源：http://uzu.jinyuanbaomall.cn

================================================================================
来源：http://otp.cucudq.cn

[L01] 发送 GET 请求
来源：http://cax.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pcf.tian-w.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tuy.quarkkingdee.top

JS:   await fetch(url)
来源：http://bqq.smart0.xyz

TS:   await fetch(url)
来源：http://mrc.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hyr.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://jod.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fpm.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ags.havefunace.top

[L02] 发送 POST JSON
来源：http://xun.jinyuanbaomall.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mon.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://var.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wzn.ppjwa.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ivi.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bmq.nanxuanxn.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fwk.yj20258888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hmt.bjfxy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jzc.fengsongda.top

[L03] 设置自定义请求头
来源：http://alr.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hdg.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bku.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bmg.ivvv.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sil.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://diz.hesvh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xdq.chenjidiqi.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aqp.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dvw.jianghu66.top

[L04] 设置超时
来源：http://uiz.c1oappe.top

Py:   requests.get(url, timeout=5)
来源：http://hub.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kvt.wangdashe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zwk.fktsv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uvz.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hfz.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fqr.iojbl.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://twz.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aza.yueranfly.top

[L05] 上传文件（multipart）
来源：http://rjp.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ula.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eym.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wpq.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uoj.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rks.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wca.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gpq.yj202588.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gta.yj202588.top

[L06] 解析响应为 JSON
来源：http://kgl.ybcxt.top

Py:   resp.json()
来源：http://loq.meibo888.top

PHP:  json_decode($body, true);
来源：http://coz.jyoumei.cn

JS:   await resp.json()
来源：http://jfu.xingfuxueyuan.xyz

TS:   await resp.json()
来源：http://eay.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://szb.fanxiaobao.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oxm.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://jbm.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jxz.meibo888.top

[L07] 处理 HTTP 状态码
来源：http://ilt.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dhc.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tvw.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://xeb.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://bkq.shangyingyoupin.top

Java: resp.statusCode()
来源：http://xdr.hnqzz.top

Go:   resp.StatusCode
来源：http://wuk.ywan-chungtsiang.top

Ruby: resp.code.to_i
来源：http://hbu.yonumen.top

C#:   (int)resp.StatusCode
来源：http://lgr.nanxinkj.top

[L08] 并发请求多个地址
来源：http://qzy.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fdz.redwolf501.top

PHP:  curl_multi_init() 系列
来源：http://jtz.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://awp.zhixingplan.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wsg.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gmx.hnxiangtu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ggd.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tkn.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xbl.zhixingplan.top

================================================================================
来源：http://ayi.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://ura.ydjk.org.cn

================================================================================
来源：http://tef.sweek.top

[M01] 读取命令行参数
来源：http://ljq.zdbjq.cn

Py:   sys.argv[1:]
来源：http://vui.nanxinkj.top

PHP:  $argv;  $argc;
来源：http://gel.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://cvr.iojbl.cn

TS:   process.argv.slice(2)
来源：http://jyk.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://tmu.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://kjt.snrcjt.cn

Ruby: ARGV
来源：http://znn.bbcook.cn

C#:   args 数组（Main 方法参数）
来源：http://pdx.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://eit.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://ewq.sjlbkw.cn


<!-- 参考信息 -->