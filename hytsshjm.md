代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gum.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dij.nanxinkj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pyh.sufxvd.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tft.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dba.wangdashe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oix.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iqe.hcnkem.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pom.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jsa.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://xyv.0kj1m.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ryf.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rbx.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mgw.jinqigfzy.top

TS:   /error/gim
来源：http://lhr.tianlin.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vee.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fjg.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://guo.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://swk.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://lsd.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sjs.xziqi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fby.yuanzhike.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://njl.epnwcf.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://afq.yj202588.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hrj.nwbrower.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ucx.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nuf.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dsm.jinyuanbaomall.cn

================================================================================
来源：http://dqf.jiagoushi.top

J. 日期与时间
来源：http://svl.bbcook.cn

================================================================================
来源：http://jxa.hcnkem.com

[J01] 获取当前时间
来源：http://hyx.fktsv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kxx.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://miw.pycfn.com

JS:   new Date();  Date.now()
来源：http://qbr.zhoulong.xyz

TS:   new Date();  Date.now()
来源：http://cyf.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://hle.yj20258888.top

Go:   time.Now()
来源：http://suu.ydzc1.top

Ruby: Time.now
来源：http://upi.wangdashe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uwe.gotoacloud.top

[J02] 格式化输出
来源：http://xky.havefunace.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ebt.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tkg.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bxc.hcnkem.com

TS:   d.toISOString()
来源：http://mra.jinqigfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ebp.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tma.chenlongwang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sjd.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wls.0kj1m.cn

[J03] 字符串解析为日期
来源：http://mdx.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://chv.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://amz.tanke756.top

JS:   new Date("2024-01-02")
来源：http://snd.jiagoushi.top

TS:   new Date("2024-01-02")
来源：http://ftf.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://yry.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dms.cqqwz.cn

Ruby: Date.parse("2024-01-02")
来源：http://gne.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hwd.shangyingyoupin.top

[J04] 时间戳与日期互转
来源：http://vhg.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zbn.shanyushiyangtech.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://twk.hysaishi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vqh.sufxvd.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zzy.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wdx.yangfankeji.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kyz.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yaw.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kbq.cashguo.top

[J05] 时间加减（加 7 天）
来源：http://ymv.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://oga.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ggw.0kj1m.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://arv.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xtl.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://hva.ybcxt.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qqr.gzhubu.top

Ruby: Time.now + 7 * 86400
来源：http://rdf.fehbvm.com

C#:   DateTime.Now.AddDays(7)
来源：http://uvl.quarkkingdee.top

[J06] 计算两时间之差
来源：http://eis.nanxinkj.top

Py:   (end - start).total_seconds()
来源：http://cyl.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://zec.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yab.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eta.cqqwz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://stn.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://dwc.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://omz.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://uph.xuanzx.com

[J07] 比较两个日期
来源：http://xun.zhixingplan.top

Py:   d1 < d2;  d1 == d2
来源：http://brz.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ota.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://jky.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://zyl.svipenyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wzr.bbcook.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qbk.jinghuilouyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nxt.nwbrower.top

C#:   d1 < d2;  d1 == d2
来源：http://uqr.yueranfly.top

[J08] 提取年月日与星期
来源：http://wbl.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xem.yangfankeji.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jzt.hywenlv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://crz.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mju.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sdo.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zha.jlsjyb.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vte.0kj1m.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oxv.pycfn.com

[J09] 时区处理
来源：http://enc.daria6918.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nsf.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cvc.ydzc1.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vph.zhoulong.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rup.jlsjyb.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fio.chenlongwang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hlm.birdmap.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ccx.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dxy.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://apd.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ows.zhixingplan.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lnm.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vgk.vqdsnc.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iqt.haohaochexian.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xuc.haohaochexian.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://teo.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iwo.yvedp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://svl.fktsv.cn

================================================================================
来源：http://ldb.sxryk.cn

K. JSON 与序列化
来源：http://dni.yj20258.top

================================================================================
来源：http://sgf.zhiwuduotai.top

[K01] 对象转 JSON 字符串
来源：http://vxf.zhixingplan.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gaz.daxiang520.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wnp.zhengqikj.top

JS:   JSON.stringify(obj)
来源：http://ydr.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://uvc.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gxs.yongpay.top

Go:   json.Marshal(obj)
来源：http://zlb.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://zgl.hywenlv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rht.daria6918.cn

[K02] JSON 字符串转对象
来源：http://pmf.jqgufenzy.top

Py:   json.loads(s)
来源：http://qfy.gogol.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dpl.guowangkeji.top

JS:   JSON.parse(s)
来源：http://sph.guannengcc.top

TS:   JSON.parse(s)
来源：http://rzf.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xva.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://nbh.316326.xyz

Ruby: JSON.parse(s)
来源：http://wou.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iqt.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://tpz.shangyingyoupin.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xoj.cheryme.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pef.aizwys.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sod.dashuyun.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zcq.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://abf.birdmap.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ifi.hnqzz.top

Ruby: JSON.pretty_generate(obj)
来源：http://wst.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qqo.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://dlh.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dtd.cdnleiting.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://btx.yfazqb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yzc.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uow.jinqigufen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xzn.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://exi.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dvx.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tqt.zhoulong.xyz

[K05] 深拷贝对象
来源：http://mfw.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://kue.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://uet.xziqi.cn

JS:   structuredClone(obj)
来源：http://dyu.xingfuxueyuan.xyz

TS:   structuredClone(obj)
来源：http://mhc.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://drm.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vvs.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kyu.chenzaomai.com

C#:   // 序列化往返，或自定义 Clone
来源：http://rju.meibo888.top

[K06] 解析 URL 查询串
来源：http://hnk.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bmf.feifeiyinyue.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://epw.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tbt.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://koz.uphjek.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vig.jinqigfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://umd.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pcb.svipenyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://akt.shzxlz.cn

[K07] 进制转换
来源：http://deb.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xob.xuanzx.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eze.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uck.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qyu.yuxming.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cpc.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uom.meibo888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://owd.sxryk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://asa.nanxinkj.top

[K08] 二进制序列化（非 JSON）
来源：http://xgd.jinqigufen.top

Py:   pickle.dumps(obj)
来源：http://gbh.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xfi.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://eba.jyoumei.cn

TS:   v8.serialize(obj)        // Node
来源：http://fyr.redwolf501.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sjf.dianchejie.cn

Go:   encoding/gob
来源：http://ulr.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://vhu.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rdw.yj20258888.top

================================================================================
来源：http://fkq.daria6918.cn

L. 网络请求
来源：http://rig.9152youxi.cn

================================================================================
来源：http://ecr.jyoumei.cn

[L01] 发送 GET 请求
来源：http://zcj.yongpay.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ham.sxryk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ucd.sxryk.cn

JS:   await fetch(url)
来源：http://kgb.xinyue.icu

TS:   await fetch(url)
来源：http://kgh.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rvs.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://vki.uphjek.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ntl.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lmw.sufxvd.cn

[L02] 发送 POST JSON
来源：http://lmk.jiagoushi.top

Py:   requests.post(url, json={"a": 1})
来源：http://eee.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gnu.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mrf.yuxming.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qnr.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rlf.jianghu66.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gmd.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jel.cqqwz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vgz.wangdashe.top

[L03] 设置自定义请求头
来源：http://jmq.yuanzhike.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wkm.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zhi.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ifl.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gmz.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ylu.yongpay.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kwp.andypj.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nyi.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cjv.nanxinkj.top

[L04] 设置超时
来源：http://ydm.havefunace.top

Py:   requests.get(url, timeout=5)
来源：http://fsu.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kep.chenlongwang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gjv.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tkb.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ulk.shanyushiyangtech.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sir.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://usy.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jhv.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://uix.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://utw.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bhm.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ixl.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ooi.sufxvd.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jti.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://swb.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sqt.gotoacloud.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sau.iojbl.cn

[L06] 解析响应为 JSON
来源：http://ewv.meibo888.top

Py:   resp.json()
来源：http://ctk.iojbl.cn

PHP:  json_decode($body, true);
来源：http://aid.zhixingplan.top

JS:   await resp.json()
来源：http://omm.zycfv.cn

TS:   await resp.json()
来源：http://mbs.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qbd.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vlx.chenjidiqi.icu

Ruby: JSON.parse(resp.body)
来源：http://coo.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zmr.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://nlk.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xdl.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mgh.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://rlu.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://hha.yfazqb.com

Java: resp.statusCode()
来源：http://etl.zdbjq.cn

Go:   resp.StatusCode
来源：http://eas.cucudq.cn

Ruby: resp.code.to_i
来源：http://fpw.guowangkeji.top

C#:   (int)resp.StatusCode
来源：http://xuo.chenlongwang.top

[L08] 并发请求多个地址
来源：http://gzc.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ddq.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://zlb.wangshuangyany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://chr.ctjpmb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://olv.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zal.hnqzz.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mgv.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://udd.zdbjq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dgl.vehdjk.com

================================================================================
来源：http://udw.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://htu.cqqwz.cn

================================================================================
来源：http://tmm.jyoumei.cn

[M01] 读取命令行参数
来源：http://you.0kj1m.cn

Py:   sys.argv[1:]
来源：http://ilk.gogol.net.cn

PHP:  $argv;  $argc;
来源：http://lrk.sweek.top

JS:   process.argv.slice(2)
来源：http://wyg.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://qdk.ctjpmb.com

Java: args 数组（main 方法参数）
来源：http://vre.gotoacloud.top

Go:   os.Args[1:]
来源：http://esj.tianlin.xyz

Ruby: ARGV
来源：http://gfj.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://yon.fktsv.cn

[M02] 读取环境变量
来源：http://xxw.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://bne.wangdashe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://epe.tianlin.xyz

JS:   process.env.HOME
来源：http://qio.zdqjudy.top

TS:   process.env.HOME
来源：http://vvi.jqgfzy.top

Java: System.getenv("HOME")
来源：http://oms.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://khv.svipenyu.cn

Ruby: ENV["HOME"]
来源：http://vry.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iow.mhx1999.top

[M03] 执行外部命令
来源：http://ecv.shangyingyoupin.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://muc.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oiw.mhx1999.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mzr.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oed.xuetiantiany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wan.xylfe.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vpi.havefunace.top

Ruby: system("ls -l");  `ls -l`
来源：http://yft.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://bwu.andypj.xyz


<!-- 参考信息 -->