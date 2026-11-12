代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uqw.52xcode.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qqa.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vsp.yfazqb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bxc.yuanzhike.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yma.snrcjt.cn

[I07] 忽略大小写与多行模式
来源：http://uyq.meibo888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ivi.dianchejie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lsq.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nrk.hongshengwenyu.top

TS:   /error/gim
来源：http://rtp.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fvt.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xgs.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://qnp.jyoumei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yoz.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://ifg.fktsv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jgn.zhengqikj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pyg.hcnkem.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tws.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cdj.sysykeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ngb.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dco.haohaochexian.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cnm.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wlx.nwbrower.top

================================================================================
来源：http://ycc.zycfv.cn

J. 日期与时间
来源：http://qts.hnqzz.top

================================================================================
来源：http://dvt.aizwys.cn

[J01] 获取当前时间
来源：http://pem.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kue.shuidangran.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://drc.chenlongwang.top

JS:   new Date();  Date.now()
来源：http://bba.hammf.cn

TS:   new Date();  Date.now()
来源：http://gwe.yj20258.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nna.nwbrower.top

Go:   time.Now()
来源：http://jbm.c1oappe.top

Ruby: Time.now
来源：http://cqf.haohaochexian.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nic.sxryk.cn

[J02] 格式化输出
来源：http://pxh.sxryk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aob.dianchejie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ruj.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cak.wangshuangyany.cn

TS:   d.toISOString()
来源：http://yel.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cis.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yrd.ppjwa.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://koa.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kpc.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://exm.tian-w.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xeo.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qxy.cqqwz.cn

JS:   new Date("2024-01-02")
来源：http://lvv.quarkkingdee.top

TS:   new Date("2024-01-02")
来源：http://ymv.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://fqj.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://arj.52xcode.cn

Ruby: Date.parse("2024-01-02")
来源：http://qez.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://clq.svipenyu.cn

[J04] 时间戳与日期互转
来源：http://kbe.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wgm.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jjq.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uph.cashguo.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qdi.xziqi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nxb.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xxi.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xfe.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rgh.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://gud.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://gmi.hesvh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wzx.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mfz.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nul.vehdjk.com

Java: LocalDate.now().plusDays(7)
来源：http://nhb.ctjpmb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://stf.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://wcx.uphjek.com

C#:   DateTime.Now.AddDays(7)
来源：http://rax.sjlbkw.cn

[J06] 计算两时间之差
来源：http://why.cqqwz.cn

Py:   (end - start).total_seconds()
来源：http://cxq.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://plm.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rwt.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ydr.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://ofj.fehbvm.com

Go:   end.Sub(start).Hours()
来源：http://pbo.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://oon.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://qmm.0kj1m.cn

[J07] 比较两个日期
来源：http://tdn.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://vxl.yonumen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://osd.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://onf.xuetiantiany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://svz.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://buh.xylfe.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://llu.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://ypl.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://css.sxryk.cn

[J08] 提取年月日与星期
来源：http://mvm.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wux.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nrn.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ugs.iojbl.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pkq.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lbf.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ndr.jianghu66.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ghm.ehwqpu.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fme.svipenyu.cn

[J09] 时区处理
来源：http://gwp.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://irm.kuanghao11.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vtu.redwolf501.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mng.sjlbkw.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oti.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ylh.yj202588.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pcu.gogol.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://udn.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jyx.aibaodan.cn

[J10] 取今天 / 本月第一天
来源：http://raj.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ptb.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uvv.gzhubu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rsr.wangshuangyany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mww.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ikc.mhx1999.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ubi.jianghu66.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cue.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hlp.hesvh.cn

================================================================================
来源：http://jte.tarul.cn

K. JSON 与序列化
来源：http://nik.cheryme.top

================================================================================
来源：http://hvg.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://kje.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ixs.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wlu.havefunace.top

JS:   JSON.stringify(obj)
来源：http://tcv.jyoumei.cn

TS:   JSON.stringify(obj)
来源：http://axc.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aiy.pycfn.com

Go:   json.Marshal(obj)
来源：http://qhm.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://nnl.sweek.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gmq.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://smk.shanyushiyangtech.top

Py:   json.loads(s)
来源：http://pdd.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://brz.havefunace.top

JS:   JSON.parse(s)
来源：http://tmx.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://bmn.zhiwuduotai.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dby.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://pym.0kj1m.cn

Ruby: JSON.parse(s)
来源：http://qxl.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qgj.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://cwg.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://odl.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ikv.zhoulong.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://uua.jqgfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lsu.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xut.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://phd.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://suc.xinyue.icu

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lru.52xcode.cn

[K04] 读取 JSON 文件
来源：http://tye.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lgl.fehbvm.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qcr.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pmc.smart0.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nng.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tfa.cucudq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qhv.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fwp.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bgl.tarul.cn

[K05] 深拷贝对象
来源：http://yml.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://mmy.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://cqn.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://rpb.fehbvm.com

TS:   structuredClone(obj)
来源：http://xkj.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ngp.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wxb.nanxuanxn.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zca.jyoumei.cn

[K06] 解析 URL 查询串
来源：http://ddh.yuxming.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rkg.zdqjudy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qyl.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mga.xziqi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wrv.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dah.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://adk.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lxn.iojbl.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://are.pengpengdd.cyou

[K07] 进制转换
来源：http://nnx.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://riw.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nkw.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sch.yj20258.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://whi.xuanzx.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nbc.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wqx.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://evb.jinyuanbaomall.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ztm.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://ekd.yonumen.top

Py:   pickle.dumps(obj)
来源：http://xhr.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vvu.0kj1m.cn

JS:   v8.serialize(obj)        // Node
来源：http://qya.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://rdq.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lxo.jianghu66.top

Go:   encoding/gob
来源：http://wqc.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://rxw.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yaa.tarul.cn

================================================================================
来源：http://tqt.tian-w.cn

L. 网络请求
来源：http://yjh.smart0.xyz

================================================================================
来源：http://jlg.meibo888.top

[L01] 发送 GET 请求
来源：http://uda.jinghuilouyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://clz.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yhv.snrcjt.cn

JS:   await fetch(url)
来源：http://nqi.xinyue.icu

TS:   await fetch(url)
来源：http://ljb.hammf.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nmp.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://gke.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ziy.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sbm.fktsv.cn

[L02] 发送 POST JSON
来源：http://drk.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://vtt.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mhi.xziqi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zpy.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tdp.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pra.aibaodan.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ery.dianchejie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zxr.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://woj.havefunace.top

[L03] 设置自定义请求头
来源：http://pms.jinqigfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rar.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pnz.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mhz.0kj1m.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://abb.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://woc.cashguo.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qkr.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yrx.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rus.jinqigfzy.top

[L04] 设置超时
来源：http://rhx.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://ggf.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rif.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kju.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jsk.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ref.yfazqb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://odo.chenlongwang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ebb.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vjk.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://qsz.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tby.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oyk.quarkkingdee.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rsh.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fsl.jyoumei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kxk.shanyushiyangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cge.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uew.gzhubu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://whu.epnwcf.com

[L06] 解析响应为 JSON
来源：http://npk.ydjk.org.cn

Py:   resp.json()
来源：http://tlv.sufxvd.cn

PHP:  json_decode($body, true);
来源：http://rmb.9152youxi.cn

JS:   await resp.json()
来源：http://fdg.zdbjq.cn

TS:   await resp.json()
来源：http://cky.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cfj.hongshengwenyu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gjf.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://evk.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vld.jqgfzy.top

[L07] 处理 HTTP 状态码
来源：http://idy.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://che.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cqy.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://dvb.birdmap.top

TS:   resp.ok;  resp.status
来源：http://wnr.wangshuangyany.cn

Java: resp.statusCode()
来源：http://uur.yuanzhike.top

Go:   resp.StatusCode
来源：http://rfi.yangfankeji.com

Ruby: resp.code.to_i
来源：http://caj.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://laf.chenzaomai.com

[L08] 并发请求多个地址
来源：http://qoz.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cdr.daria6918.cn

PHP:  curl_multi_init() 系列
来源：http://wks.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://opx.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fri.ydzc1.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kpt.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xho.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xbk.bjfxy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zcq.tianlin.xyz

================================================================================
来源：http://gox.wangdashe.top

M. 命令行 / 进程 / 环境
来源：http://bux.ybcxt.top

================================================================================
来源：http://sxt.jiagoushi.top

[M01] 读取命令行参数
来源：http://llc.sysykeji.top

Py:   sys.argv[1:]
来源：http://gvq.tanke756.top

PHP:  $argv;  $argc;
来源：http://ehr.tianlin.xyz

JS:   process.argv.slice(2)
来源：http://uyi.svipenyu.cn

TS:   process.argv.slice(2)
来源：http://erf.yanxiufei.cn

Java: args 数组（main 方法参数）
来源：http://unw.yvedp.cn

Go:   os.Args[1:]
来源：http://utk.fktsv.cn

Ruby: ARGV
来源：http://rfw.fktsv.cn

C#:   args 数组（Main 方法参数）
来源：http://iuu.ctjpmb.com

[M02] 读取环境变量
来源：http://tis.yonumen.top

Py:   os.environ.get("HOME")
来源：http://uli.gaohongyu789.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://moe.quarkkingdee.top

JS:   process.env.HOME
来源：http://mei.fehbvm.com

TS:   process.env.HOME
来源：http://oya.havefunace.top

Java: System.getenv("HOME")
来源：http://yuw.yongpay.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kuk.xuanzx.com

Ruby: ENV["HOME"]
来源：http://nfa.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hpg.jqgfzy.top

[M03] 执行外部命令
来源：http://shb.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://drg.zhaomingkeji.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kvj.sweek.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hzy.feifeiyinyue.top

TS:   child_process.execSync("ls -l").toString()
来源：http://erj.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kah.zhixingplan.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nhn.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hym.jinqigufen.top

C#:   Process.Start("ls", "-l");
来源：http://mcy.daxiang520.top

[M04] 获取当前工作目录
来源：http://lay.ctjpmb.com

Py:   os.getcwd()
来源：http://ird.daria6918.cn

PHP:  getcwd();
来源：http://djn.hongshengwenyu.top

JS:   process.cwd()
来源：http://asp.fengsongda.top


<!-- 参考信息 -->