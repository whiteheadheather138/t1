代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://ijt.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gfo.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://jju.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://bsu.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://bqb.daria6918.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xrs.tanke756.top

Ruby: s.split(/\s*,\s*/)
来源：http://lta.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ybe.gotoacloud.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vgg.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wbf.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://job.shuidangran.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mwd.sjlbkw.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dhf.xylfe.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ckh.0kj1m.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ddh.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hdh.ydzc1.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pwb.sweek.top

[I07] 忽略大小写与多行模式
来源：http://nbx.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://soa.vehdjk.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qhx.shuidangran.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jbe.chenlongwang.top

TS:   /error/gim
来源：http://rcc.jianghu66.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ozx.ivvv.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dnq.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://uwy.tanke756.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xnm.shangyingyoupin.top

[I08] 贪婪与非贪婪匹配
来源：http://rbe.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ucq.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tva.gaohongyu789.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ahi.aizwys.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mll.fehbvm.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ldi.pycfn.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pnw.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qba.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dlk.zhixingplan.top

================================================================================
来源：http://brl.ppjwa.cn

J. 日期与时间
来源：http://pdh.9152youxi.cn

================================================================================
来源：http://tpp.redwolf501.top

[J01] 获取当前时间
来源：http://qdl.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lpd.wangdashe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://inj.c1oappe.top

JS:   new Date();  Date.now()
来源：http://sox.shanyushiyangtech.top

TS:   new Date();  Date.now()
来源：http://xxe.yj20258888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rxs.guowangkeji.top

Go:   time.Now()
来源：http://jsv.ydzc1.top

Ruby: Time.now
来源：http://flz.uphjek.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ddl.andypj.xyz

[J02] 格式化输出
来源：http://yjo.xylfe.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://etq.vqdsnc.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rjd.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eeh.zhijiandao.cn

TS:   d.toISOString()
来源：http://gbd.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://scn.yuanzhike.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hri.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ruf.andypj.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nfj.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://fkk.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://egq.redwolf501.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kpr.jinqigfzy.top

JS:   new Date("2024-01-02")
来源：http://qnr.vqdsnc.cn

TS:   new Date("2024-01-02")
来源：http://nwv.cdnleiting.top

Java: LocalDate.parse("2024-01-02")
来源：http://atj.yvedp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kta.hammf.cn

Ruby: Date.parse("2024-01-02")
来源：http://kuk.ywan-chungtsiang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ido.xylfe.cn

[J04] 时间戳与日期互转
来源：http://iwr.havefunace.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oyr.sxryk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xzp.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://veb.jqgufenzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zjw.kuanghao11.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qym.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ftl.hnqzz.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fum.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vkl.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://eal.gotoacloud.top

Py:   now + timedelta(days=7)
来源：http://omy.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://owz.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wzr.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pfo.shanyushiyangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://zln.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jvf.c1oappe.top

Ruby: Time.now + 7 * 86400
来源：http://hnz.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://syx.fehbvm.com

[J06] 计算两时间之差
来源：http://zbv.cdnleiting.top

Py:   (end - start).total_seconds()
来源：http://sga.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://ruv.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wfx.shuidangran.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zsv.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://idq.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://ngx.epnwcf.com

Ruby: end - start                 # 返回秒数
来源：http://psl.wangshuangyany.cn

C#:   (end - start).TotalSeconds
来源：http://okg.0kj1m.cn

[J07] 比较两个日期
来源：http://xje.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://fjn.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://skz.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://adc.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://nwr.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jlk.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ley.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://yus.0kj1m.cn

C#:   d1 < d2;  d1 == d2
来源：http://use.yj20258.top

[J08] 提取年月日与星期
来源：http://lfi.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gsf.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tne.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xfo.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gab.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ihh.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sxh.andypj.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sny.tanke756.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cfn.zhaomingkeji.xyz

[J09] 时区处理
来源：http://itg.wangshuangyany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wmf.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://adi.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cga.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://txj.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ofm.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uzw.haohaochexian.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vga.hfpthk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hkn.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://orr.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bza.fzhhl.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bxf.fanxiaobao.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kcf.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pvc.shzxlz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qve.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fra.chenzaomai.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lyr.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tjb.fzhhl.top

================================================================================
来源：http://lyn.gotoacloud.top

K. JSON 与序列化
来源：http://tqq.shanyushiyangtech.top

================================================================================
来源：http://xti.aizwys.cn

[K01] 对象转 JSON 字符串
来源：http://kzk.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bxz.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oma.yvedp.cn

JS:   JSON.stringify(obj)
来源：http://phd.ybcxt.top

TS:   JSON.stringify(obj)
来源：http://xif.tian-w.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rjb.fehbvm.com

Go:   json.Marshal(obj)
来源：http://hgl.nanxinkj.top

Ruby: obj.to_json                                     // require "json"
来源：http://oyd.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zwt.yj20258888.top

[K02] JSON 字符串转对象
来源：http://jfl.yanxiufei.cn

Py:   json.loads(s)
来源：http://ilq.snrcjt.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pyg.iojbl.cn

JS:   JSON.parse(s)
来源：http://ghm.0kj1m.cn

TS:   JSON.parse(s)
来源：http://sjy.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fuf.52xcode.cn

Go:   json.Unmarshal(data, &v)
来源：http://kjd.xinyue.icu

Ruby: JSON.parse(s)
来源：http://iku.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ssh.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://czs.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vau.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zuq.yangfankeji.com

JS:   JSON.stringify(obj, null, 2)
来源：http://swy.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vdo.redwolf501.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dfc.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ytq.sxryk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://twr.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fvd.yangfankeji.com

[K04] 读取 JSON 文件
来源：http://cym.xuanzx.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ces.sxryk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mlj.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bug.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bih.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://biy.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://byo.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mwm.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vtg.fehbvm.com

[K05] 深拷贝对象
来源：http://ymg.sweek.top

Py:   copy.deepcopy(obj)
来源：http://vtw.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://hkz.tarul.cn

JS:   structuredClone(obj)
来源：http://vkp.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://qrj.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://kwo.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qjk.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ogf.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mnr.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://vfh.yanxiufei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ycz.zhengqikj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uyf.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ukn.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kmz.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://evc.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tjk.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dzo.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eld.smart0.xyz

[K07] 进制转换
来源：http://fvw.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zaq.9152youxi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vkk.jiagoushi.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lhm.snrcjt.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rqq.hammf.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ben.ydzc1.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vna.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qrw.fehbvm.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bse.fanxiaobao.xyz

[K08] 二进制序列化（非 JSON）
来源：http://vkw.jinqigfzy.top

Py:   pickle.dumps(obj)
来源：http://ooc.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yom.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://ism.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://mkj.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vwf.uphjek.com

Go:   encoding/gob
来源：http://buf.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://uqy.kuanghao11.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fwz.bbcook.cn

================================================================================
来源：http://fkm.yongpay.top

L. 网络请求
来源：http://jsh.yuanzhike.top

================================================================================
来源：http://ali.cdnleiting.top

[L01] 发送 GET 请求
来源：http://vie.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jua.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ocg.aibaodan.cn

JS:   await fetch(url)
来源：http://ivo.jlsjyb.cn

TS:   await fetch(url)
来源：http://ffn.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jvl.jinghuilouyu.cn

Go:   resp, err := http.Get(url)
来源：http://zxm.hammf.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gti.epnwcf.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jwr.cdnleiting.top

[L02] 发送 POST JSON
来源：http://cur.c1oappe.top

Py:   requests.post(url, json={"a": 1})
来源：http://jjk.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://npg.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://txn.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zkp.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://igt.zdqjudy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ili.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kwu.guannengcc.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oka.aizwys.cn

[L03] 设置自定义请求头
来源：http://zfj.nanxinkj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mfp.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://itk.shanyushiyangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xtf.jinghuilouyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://epo.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ids.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fpd.sjlbkw.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://srh.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://msl.feifeiyinyue.top

[L04] 设置超时
来源：http://vbc.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://fve.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tes.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tvn.guowangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jki.nanxuanxn.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gkb.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wfk.wangshuangyany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qty.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://amg.guannengcc.top

[L05] 上传文件（multipart）
来源：http://dfg.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vmz.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hmx.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ahh.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rfb.hywenlv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://htk.jqgufenzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yzw.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bam.zhongyouzk.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ezd.fanxiaobao.xyz

[L06] 解析响应为 JSON
来源：http://fso.sjlbkw.cn

Py:   resp.json()
来源：http://ksz.cucudq.cn

PHP:  json_decode($body, true);
来源：http://ppw.yonumen.top

JS:   await resp.json()
来源：http://ysf.shanyushiyangtech.top

TS:   await resp.json()
来源：http://nzy.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kwe.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gry.shangyingyoupin.top

Ruby: JSON.parse(resp.body)
来源：http://fjv.c1oappe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lio.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://ycs.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tft.daria6918.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lam.yuxming.cn

JS:   resp.ok;  resp.status
来源：http://gti.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://ncq.shuidangran.top

Java: resp.statusCode()
来源：http://euu.chenlongwang.top

Go:   resp.StatusCode
来源：http://dzp.xylfe.cn

Ruby: resp.code.to_i
来源：http://xsk.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://lmb.yj202588.top

[L08] 并发请求多个地址
来源：http://fxk.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://owe.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://rgr.yuxming.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fow.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qyg.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ajb.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kqd.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zfx.birdmap.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://try.zdqjudy.top

================================================================================
来源：http://qab.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://dgp.birdmap.top

================================================================================
来源：http://jzk.jlsjyb.cn

[M01] 读取命令行参数
来源：http://tbs.hnxiangtu.top

Py:   sys.argv[1:]
来源：http://mtm.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://dvc.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://nwn.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://mpe.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://nld.mhx1999.top

Go:   os.Args[1:]
来源：http://vzt.quarkkingdee.top

Ruby: ARGV
来源：http://six.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://xet.jqgfzy.top

[M02] 读取环境变量
来源：http://pqd.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://gvr.wangdashe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ykg.sxryk.cn

JS:   process.env.HOME
来源：http://ain.ybcxt.top

TS:   process.env.HOME
来源：http://qyr.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://ola.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xax.cashguo.top

Ruby: ENV["HOME"]
来源：http://mis.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vnh.nwbrower.top

[M03] 执行外部命令
来源：http://lvz.nwbrower.top


<!-- 参考信息 -->