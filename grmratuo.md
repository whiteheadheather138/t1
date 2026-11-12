代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://ano.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://ihz.chenlongwang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xgt.jinghuilouyu.cn

[I05] 按正则拆分
来源：http://peh.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tsu.hesvh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pny.yj20258.top

JS:   s.split(/\s*,\s*/)
来源：http://ufm.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://hxz.cashguo.top

Java: s.split("\\s*,\\s*")
来源：http://eef.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jpf.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://nze.cqqwz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mtm.chenjidiqi.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gtz.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kci.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gtr.dashuyun.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mjy.gaohongyu789.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://skj.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xvo.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gfj.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lie.ydjk.org.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://itu.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://udz.hfpthk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://log.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lih.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xnz.tian-w.cn

TS:   /error/gim
来源：http://icc.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lca.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tlf.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://gkc.dianchejie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iay.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://lrh.yuxming.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oft.havefunace.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pcd.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://swh.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ddn.yj20258888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://swp.mhx1999.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://noy.ppjwa.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://stp.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dig.shanyushiyangtech.top

================================================================================
来源：http://tnb.hammf.cn

J. 日期与时间
来源：http://vwd.yonumen.top

================================================================================
来源：http://ily.wangshuangyany.cn

[J01] 获取当前时间
来源：http://uyy.c1oappe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jmf.sufxvd.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kev.xylfe.cn

JS:   new Date();  Date.now()
来源：http://swv.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://gxs.aibaodan.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wkn.gogol.net.cn

Go:   time.Now()
来源：http://zgz.aizwys.cn

Ruby: Time.now
来源：http://tca.fktsv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tre.yanxiufei.cn

[J02] 格式化输出
来源：http://noh.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eug.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mey.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://frq.mhx1999.top

TS:   d.toISOString()
来源：http://kqh.hnxiangtu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yzc.havefunace.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rbl.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rcf.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ems.xylfe.cn

[J03] 字符串解析为日期
来源：http://zsp.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kmk.hesvh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yzv.uphjek.com

JS:   new Date("2024-01-02")
来源：http://ufp.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://rkz.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://kvc.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eoi.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://ugf.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pjo.zycfv.cn

[J04] 时间戳与日期互转
来源：http://jjn.yangfankeji.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://phg.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ttq.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gzy.bjfxy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jrz.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zcu.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://clh.shanyushiyangtech.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ibf.daria6918.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jfz.wangdashe.top

[J05] 时间加减（加 7 天）
来源：http://rjr.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://vxa.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://agj.cashguo.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hpe.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fkk.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://hoi.yvedp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wtn.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://cst.zhongyouzk.top

C#:   DateTime.Now.AddDays(7)
来源：http://ilj.meibo888.top

[J06] 计算两时间之差
来源：http://hva.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://cbe.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://chh.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dcc.ehwqpu.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rkg.cucudq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fxs.9152youxi.cn

Go:   end.Sub(start).Hours()
来源：http://qde.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://frf.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://sua.ivvv.top

[J07] 比较两个日期
来源：http://nxs.pycfn.com

Py:   d1 < d2;  d1 == d2
来源：http://amn.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bwl.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://aby.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://ukc.cqqwz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://egy.feifeiyinyue.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cku.ehwqpu.com

Ruby: d1 < d2;  d1 == d2
来源：http://bjx.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://rek.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://hhw.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rik.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yqz.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pkr.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bcb.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wft.jinyuanbaomall.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jsx.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://weu.chenjidiqi.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kws.hysaishi.cn

[J09] 时区处理
来源：http://lpd.epnwcf.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vwf.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://agc.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yje.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://run.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mzd.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iqt.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qni.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fgp.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://uxf.ivvv.top

Py:   date.today();  date.today().replace(day=1)
来源：http://frj.havefunace.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bqo.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ewb.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jce.daria6918.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zys.havefunace.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fza.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xbv.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gez.tianlin.xyz

================================================================================
来源：http://puf.xylfe.cn

K. JSON 与序列化
来源：http://onk.jyoumei.cn

================================================================================
来源：http://nuk.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://pqz.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qye.cdnleiting.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jzb.cheryme.top

JS:   JSON.stringify(obj)
来源：http://fhs.ppjwa.cn

TS:   JSON.stringify(obj)
来源：http://ati.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hsd.zhengqikj.top

Go:   json.Marshal(obj)
来源：http://doa.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qks.gotoacloud.top

C#:   JsonSerializer.Serialize(obj)
来源：http://khp.mhx1999.top

[K02] JSON 字符串转对象
来源：http://sjt.mhx1999.top

Py:   json.loads(s)
来源：http://auy.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sho.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://jrs.yonumen.top

TS:   JSON.parse(s)
来源：http://wpm.bbcook.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xva.nwbrower.top

Go:   json.Unmarshal(data, &v)
来源：http://tdk.cashguo.top

Ruby: JSON.parse(s)
来源：http://qfd.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ahp.sweek.top

[K03] JSON 美化输出（带缩进）
来源：http://jow.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ebq.nwbrower.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ylg.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nud.shanyushiyangkeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hzl.316326.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://juo.tianlin.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nem.chenlongwang.top

Ruby: JSON.pretty_generate(obj)
来源：http://frl.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rjc.hfpthk.cn

[K04] 读取 JSON 文件
来源：http://iaq.wangshuangyany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cjc.zhiwuduotai.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gok.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qkh.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kod.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cgn.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yzp.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dsz.sweek.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pnd.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://kcs.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://jzy.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://ltf.fehbvm.com

JS:   structuredClone(obj)
来源：http://dvq.dashuyun.cn

TS:   structuredClone(obj)
来源：http://qmt.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lga.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fvg.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ayg.snrcjt.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cqq.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://scp.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xhf.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wjn.sjlbkw.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://agr.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lok.jlsjyb.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://odr.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ejf.chenlongwang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hmu.chenzaomai.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wby.daria6918.cn

[K07] 进制转换
来源：http://msw.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mpe.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://alw.cqqwz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mtx.ybcxt.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vmz.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fph.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ord.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ncl.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://chi.uphjek.com

[K08] 二进制序列化（非 JSON）
来源：http://quk.jqgfzy.top

Py:   pickle.dumps(obj)
来源：http://iat.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fop.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://mjn.pengpengdd.cyou

TS:   v8.serialize(obj)        // Node
来源：http://fho.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://utp.yangfankeji.com

Go:   encoding/gob
来源：http://pwy.yj202588.top

Ruby: Marshal.dump(obj)
来源：http://aid.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://anr.shzxlz.cn

================================================================================
来源：http://bfp.yonumen.top

L. 网络请求
来源：http://rkq.fzhhl.top

================================================================================
来源：http://zdl.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://oyw.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gln.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://whx.316326.xyz

JS:   await fetch(url)
来源：http://ptm.shuidangran.top

TS:   await fetch(url)
来源：http://oct.fanxiaobao.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://znf.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://maw.hnxiangtu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uob.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ksf.dashuyun.cn

[L02] 发送 POST JSON
来源：http://xom.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://btg.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bbd.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gyr.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pqz.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ufy.c1oappe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hdi.ctjpmb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://euz.jinghuilouyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://usf.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://cnk.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uoa.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://anz.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kfu.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yqn.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uzp.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://noi.fzhhl.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://enm.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zss.jqgfzy.top

[L04] 设置超时
来源：http://vrz.zhixingplan.top

Py:   requests.get(url, timeout=5)
来源：http://dhf.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jwd.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ocf.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kov.cheryme.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nwk.jianghu66.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dmf.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://clb.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tys.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://bff.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vfa.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ywz.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iyq.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kdd.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hcr.yonumen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hxg.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iuo.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xhm.shangyingyoupin.top

[L06] 解析响应为 JSON
来源：http://ewv.yj202588.top

Py:   resp.json()
来源：http://azz.xylfe.cn

PHP:  json_decode($body, true);
来源：http://cwa.fehbvm.com

JS:   await resp.json()
来源：http://plk.hywenlv.cn

TS:   await resp.json()
来源：http://ric.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bex.wangshuangyany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dxr.uphjek.com

Ruby: JSON.parse(resp.body)
来源：http://vdw.hfpthk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://apl.xinyue.icu

[L07] 处理 HTTP 状态码
来源：http://lpw.ybcxt.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mgu.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zni.ppjwa.cn

JS:   resp.ok;  resp.status
来源：http://umy.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://zvd.zdbjq.cn

Java: resp.statusCode()
来源：http://twe.zycfv.cn

Go:   resp.StatusCode
来源：http://dsh.shzxlz.cn

Ruby: resp.code.to_i
来源：http://ixq.cheryme.top

C#:   (int)resp.StatusCode
来源：http://ldf.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://bqy.yj20258888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gnv.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://iyp.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qkn.zdqjudy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lxg.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xuh.hnxiangtu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://umd.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cxg.sweek.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tvp.ivvv.top

================================================================================
来源：http://mhy.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://whb.vehdjk.com

================================================================================
来源：http://chz.zycfv.cn

[M01] 读取命令行参数
来源：http://jli.zhaomingkeji.xyz

Py:   sys.argv[1:]
来源：http://boi.yj20258888.top

PHP:  $argv;  $argc;
来源：http://hxo.sweek.top

JS:   process.argv.slice(2)
来源：http://hmm.hesvh.cn

TS:   process.argv.slice(2)
来源：http://tee.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://ybm.aibaodan.cn

Go:   os.Args[1:]
来源：http://swv.jyoumei.cn

Ruby: ARGV
来源：http://lyk.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://gyv.52xcode.cn

[M02] 读取环境变量
来源：http://tek.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://rch.zhiwuduotai.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tjj.quarkkingdee.top

JS:   process.env.HOME
来源：http://hfp.ctjpmb.com

TS:   process.env.HOME
来源：http://unm.yanxiufei.cn

Java: System.getenv("HOME")
来源：http://emo.daxiang520.top


<!-- 参考信息 -->