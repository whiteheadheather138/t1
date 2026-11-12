代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://era.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jef.quarkkingdee.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jgc.bbcook.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wou.ctjpmb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qys.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://oti.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cwm.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://itk.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wsy.0kj1m.cn

TS:   /error/gim
来源：http://egg.yanxiufei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wvf.birdmap.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://trr.kuanghao11.cn

Ruby: s.scan(/error/i)
来源：http://ruv.jinyuanbaomall.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mzy.fktsv.cn

[I08] 贪婪与非贪婪匹配
来源：http://xdv.yuxming.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nav.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uvd.yj202588.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zsk.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mjx.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kus.gzhubu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://efi.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ihh.vqdsnc.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://guk.yonumen.top

================================================================================
来源：http://njz.fengsongda.top

J. 日期与时间
来源：http://kfj.yj20258.top

================================================================================
来源：http://adv.fengsongda.top

[J01] 获取当前时间
来源：http://prk.shuidangran.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://utn.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nkp.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://bbs.hesvh.cn

TS:   new Date();  Date.now()
来源：http://erk.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ooe.haohaochexian.top

Go:   time.Now()
来源：http://hgh.cdnleiting.top

Ruby: Time.now
来源：http://jum.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tep.jqgfzy.top

[J02] 格式化输出
来源：http://yrh.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vqe.gzhubu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ifk.sysykeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://puk.aibaodan.cn

TS:   d.toISOString()
来源：http://tvt.jinqigufen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ado.haohaochexian.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eit.ehwqpu.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zbv.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rdd.cucudq.cn

[J03] 字符串解析为日期
来源：http://xjr.shuidangran.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tem.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://szy.jqgfzy.top

JS:   new Date("2024-01-02")
来源：http://szc.gogol.net.cn

TS:   new Date("2024-01-02")
来源：http://jqs.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mgm.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://znp.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://ure.daria6918.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://awq.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://wbm.quarkkingdee.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oae.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ync.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uyr.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jvb.smart0.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hwm.yongpay.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://krv.quarkkingdee.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uzi.aizwys.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zdl.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://cwf.uphjek.com

Py:   now + timedelta(days=7)
来源：http://euh.tianlin.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://xxs.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zzz.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xsp.tarul.cn

Java: LocalDate.now().plusDays(7)
来源：http://xxr.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://abg.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://ycu.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://kgm.ivvv.top

[J06] 计算两时间之差
来源：http://wko.yj202588.top

Py:   (end - start).total_seconds()
来源：http://kqr.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://xiw.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oke.shzxlz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mlz.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://hlu.mhx1999.top

Go:   end.Sub(start).Hours()
来源：http://usl.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://bkm.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://udv.hnxiangtu.top

[J07] 比较两个日期
来源：http://llm.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://mag.ivvv.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qzk.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://yyw.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://whg.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://drv.wangshuangyany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://toi.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://lfb.jianghu66.top

C#:   d1 < d2;  d1 == d2
来源：http://fbt.jinqigfzy.top

[J08] 提取年月日与星期
来源：http://ain.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dpj.ydjk.org.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rxt.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zop.jqgfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bef.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nzt.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://muc.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jme.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fxm.shuidangran.top

[J09] 时区处理
来源：http://kfi.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rtq.guowangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vuq.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ksr.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zps.xinyue.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fwz.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rcl.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zsv.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tdk.hesvh.cn

[J10] 取今天 / 本月第一天
来源：http://qmm.mhx1999.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fpz.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mby.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://duq.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lyw.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dui.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://onb.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ztl.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://giq.vehdjk.com

================================================================================
来源：http://mbj.fehbvm.com

K. JSON 与序列化
来源：http://bkr.jqgufenzy.top

================================================================================
来源：http://bxp.hongshengwenyu.top

[K01] 对象转 JSON 字符串
来源：http://kxo.iojbl.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cuq.xylfe.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://evs.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://eox.tanke756.top

TS:   JSON.stringify(obj)
来源：http://yfa.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nvk.sjlbkw.cn

Go:   json.Marshal(obj)
来源：http://awa.chenjidiqi.icu

Ruby: obj.to_json                                     // require "json"
来源：http://qxr.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://irb.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://gmi.yj202588.top

Py:   json.loads(s)
来源：http://zhr.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dxs.hesvh.cn

JS:   JSON.parse(s)
来源：http://dzz.yangfankeji.com

TS:   JSON.parse(s)
来源：http://jai.sweek.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nlu.yangfankeji.com

Go:   json.Unmarshal(data, &v)
来源：http://xpu.hysaishi.cn

Ruby: JSON.parse(s)
来源：http://xjm.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xyz.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://rlt.vehdjk.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yus.tanke756.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://agq.zhoulong.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://yaf.chenjidiqi.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://fks.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://htt.jinqigfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mvt.jinqigfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://yiu.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cdf.shangyingyoupin.top

[K04] 读取 JSON 文件
来源：http://egz.jinqigufen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://phg.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cnk.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pru.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kff.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pna.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xtl.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://aac.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iwe.svipenyu.cn

[K05] 深拷贝对象
来源：http://tnp.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://aka.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://rfz.mhx1999.top

JS:   structuredClone(obj)
来源：http://syc.gzhubu.top

TS:   structuredClone(obj)
来源：http://stl.jiagoushi.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qxk.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jwr.wangshuangyany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kmj.ydzc1.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zdy.feifeiyinyue.top

[K06] 解析 URL 查询串
来源：http://tqa.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bit.bjfxy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mfq.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lcg.cheryme.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://egd.ivvv.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qtq.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cms.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dlh.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ldf.hammf.cn

[K07] 进制转换
来源：http://yju.fktsv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://thv.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ajg.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zgy.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hna.pycfn.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pxc.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://khe.meibo888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sqx.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kmh.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://vkn.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://ylk.vqdsnc.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xdr.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://ylg.birdmap.top

TS:   v8.serialize(obj)        // Node
来源：http://fhm.nanxinkj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dlk.shanyushiyangkeji.top

Go:   encoding/gob
来源：http://wbt.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://gjn.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ybg.pycfn.com

================================================================================
来源：http://ogt.tian-w.cn

L. 网络请求
来源：http://ypf.xylfe.cn

================================================================================
来源：http://xlp.aizwys.cn

[L01] 发送 GET 请求
来源：http://pql.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eiu.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://elw.redwolf501.top

JS:   await fetch(url)
来源：http://cot.316326.xyz

TS:   await fetch(url)
来源：http://aqt.sysykeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lgv.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://cef.redwolf501.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mle.dianchejie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://asi.ctjpmb.com

[L02] 发送 POST JSON
来源：http://efe.jyoumei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jiy.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mdm.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ttv.yangfankeji.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://adr.sweek.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qri.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wlk.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wmy.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tfx.hysaishi.cn

[L03] 设置自定义请求头
来源：http://clk.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tga.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ulb.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://szq.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rlb.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dyv.zhaomingkeji.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://duy.cucudq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bfe.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nzh.gogol.net.cn

[L04] 设置超时
来源：http://kvb.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://whm.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iqi.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rer.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ejg.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zzn.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kmb.yongpay.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vpy.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qqn.52xcode.cn

[L05] 上传文件（multipart）
来源：http://voj.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cea.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zaw.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fkn.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://icg.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yrg.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zic.ydzc1.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dzo.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://joe.fktsv.cn

[L06] 解析响应为 JSON
来源：http://bsf.zhongyouzk.top

Py:   resp.json()
来源：http://pdd.xziqi.cn

PHP:  json_decode($body, true);
来源：http://ryy.zycfv.cn

JS:   await resp.json()
来源：http://pbm.cdnleiting.top

TS:   await resp.json()
来源：http://evy.havefunace.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iij.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ygf.xuetiantiany.cn

Ruby: JSON.parse(resp.body)
来源：http://uiv.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mjb.redwolf501.top

[L07] 处理 HTTP 状态码
来源：http://oxl.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fjg.jqgufenzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gov.yongpay.top

JS:   resp.ok;  resp.status
来源：http://cws.fanxiaobao.xyz

TS:   resp.ok;  resp.status
来源：http://ugn.hfpthk.cn

Java: resp.statusCode()
来源：http://tcf.yanxiufei.cn

Go:   resp.StatusCode
来源：http://tbb.bbcook.cn

Ruby: resp.code.to_i
来源：http://swh.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://qdl.c1oappe.top

[L08] 并发请求多个地址
来源：http://rtx.tanke756.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pcx.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://gcr.yonumen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dbt.dashuyun.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ueo.chenlongwang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wqe.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gqq.gzhubu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hbd.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uqr.shuidangran.top

================================================================================
来源：http://mut.zhongyouzk.top

M. 命令行 / 进程 / 环境
来源：http://wiz.hywenlv.cn

================================================================================
来源：http://vaj.xylfe.cn

[M01] 读取命令行参数
来源：http://chl.xinyue.icu

Py:   sys.argv[1:]
来源：http://dnc.cashguo.top

PHP:  $argv;  $argc;
来源：http://qmb.jyoumei.cn

JS:   process.argv.slice(2)
来源：http://lea.ydzc1.top

TS:   process.argv.slice(2)
来源：http://jle.yanxiufei.cn

Java: args 数组（main 方法参数）
来源：http://fdk.sxryk.cn

Go:   os.Args[1:]
来源：http://mon.redwolf501.top

Ruby: ARGV
来源：http://yhc.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://nyj.svipenyu.cn

[M02] 读取环境变量
来源：http://hwj.hammf.cn

Py:   os.environ.get("HOME")
来源：http://lej.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://too.nanxinkj.top

JS:   process.env.HOME
来源：http://hpk.meibo888.top

TS:   process.env.HOME
来源：http://vkl.zhoulong.xyz

Java: System.getenv("HOME")
来源：http://vpa.cdnleiting.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aaf.jlsjyb.cn

Ruby: ENV["HOME"]
来源：http://ngs.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ads.yj202588.top

[M03] 执行外部命令
来源：http://jzw.fktsv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gzh.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aoz.havefunace.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kka.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bfz.zdbjq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://htz.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nrf.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://vnj.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://loo.bbcook.cn

[M04] 获取当前工作目录
来源：http://lbp.xylfe.cn

Py:   os.getcwd()
来源：http://byk.feifeiyinyue.top

PHP:  getcwd();
来源：http://aop.yuxming.cn

JS:   process.cwd()
来源：http://fwr.zhoulong.xyz


<!-- 参考信息 -->