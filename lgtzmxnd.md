代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ahl.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://lyo.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bgk.bjfxy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bte.shzxlz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://czu.guowangkeji.top

TS:   /error/gim
来源：http://btp.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ivv.kuanghao11.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ovs.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://ahk.wangdashe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lxf.zhijiandao.cn

[I08] 贪婪与非贪婪匹配
来源：http://lqe.snrcjt.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mqg.hysaishi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qtp.ehwqpu.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tuu.yj20258.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lft.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://czk.yj20258888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gdl.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://flq.kuanghao11.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dxf.yueranfly.top

================================================================================
来源：http://vgk.cqqwz.cn

J. 日期与时间
来源：http://cza.fzhhl.top

================================================================================
来源：http://bpx.hnqzz.top

[J01] 获取当前时间
来源：http://flo.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qie.epnwcf.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wxg.yj20258888.top

JS:   new Date();  Date.now()
来源：http://upc.c1oappe.top

TS:   new Date();  Date.now()
来源：http://cqu.sufxvd.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ypg.yonumen.top

Go:   time.Now()
来源：http://gux.zhixingplan.top

Ruby: Time.now
来源：http://xzn.zhiwuduotai.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vzj.sxryk.cn

[J02] 格式化输出
来源：http://tuc.xuetiantiany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wio.shuidangran.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dla.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tcy.9152youxi.cn

TS:   d.toISOString()
来源：http://kfg.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://odv.fengsongda.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://alc.zhongyouzk.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://axk.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jza.sjlbkw.cn

[J03] 字符串解析为日期
来源：http://ukg.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ntk.yj202588.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uhx.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://mgl.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://hik.jinyuanbaomall.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kph.jinqigufen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dqn.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://mgt.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://atn.yj20258888.top

[J04] 时间戳与日期互转
来源：http://woo.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://owh.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zni.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nqm.gogol.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://trw.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nka.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vyw.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pbt.jianghu66.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fom.jinqigfzy.top

[J05] 时间加减（加 7 天）
来源：http://nzz.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://upz.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://soi.zdqjudy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oga.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wus.fehbvm.com

Java: LocalDate.now().plusDays(7)
来源：http://rts.yuanzhike.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dor.tian-w.cn

Ruby: Time.now + 7 * 86400
来源：http://iqb.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wee.hysaishi.cn

[J06] 计算两时间之差
来源：http://lzr.jyoumei.cn

Py:   (end - start).total_seconds()
来源：http://rxv.yfazqb.com

PHP:  $end->diff($start)->days;
来源：http://nrt.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gmr.ctjpmb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wik.xuetiantiany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rol.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://afl.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://wfv.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://jis.fehbvm.com

[J07] 比较两个日期
来源：http://gpt.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://jpr.nwbrower.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mpe.aizwys.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uia.fanxiaobao.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://cdq.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ocf.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xkw.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fqm.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://qqm.jianghu66.top

[J08] 提取年月日与星期
来源：http://wbs.tianlin.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://djp.yvedp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ajf.ydzc1.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://spl.xziqi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mjv.cdnleiting.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://myq.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zxp.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lgn.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bcs.cucudq.cn

[J09] 时区处理
来源：http://iyq.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qdw.ivvv.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tpz.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eku.yueranfly.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://euh.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cgm.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sdj.svipenyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lmh.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sot.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://ham.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lsf.meibo888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://urt.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://azu.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rwf.hnqzz.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://acz.cashguo.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jfp.dashuyun.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tyq.shuidangran.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vzw.zhoulong.xyz

================================================================================
来源：http://ucp.yueranfly.top

K. JSON 与序列化
来源：http://ifk.hfpthk.cn

================================================================================
来源：http://adv.cheryme.top

[K01] 对象转 JSON 字符串
来源：http://vdj.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kxi.tianlin.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qec.birdmap.top

JS:   JSON.stringify(obj)
来源：http://ijd.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://icu.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://csh.cucudq.cn

Go:   json.Marshal(obj)
来源：http://rjk.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://qmw.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://rzm.sxryk.cn

[K02] JSON 字符串转对象
来源：http://ztv.0kj1m.cn

Py:   json.loads(s)
来源：http://iwh.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dky.vehdjk.com

JS:   JSON.parse(s)
来源：http://hqb.zycfv.cn

TS:   JSON.parse(s)
来源：http://cco.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wyj.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://eyd.redwolf501.top

Ruby: JSON.parse(s)
来源：http://dwz.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hpg.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://btm.nanxuanxn.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://syp.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://faf.nanxinkj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rgv.zhixingplan.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wdg.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oka.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://afp.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ppe.52xcode.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wwt.andypj.xyz

[K04] 读取 JSON 文件
来源：http://sxb.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ytd.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://soh.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://thr.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zcj.zhixingplan.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mhi.yfazqb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tfv.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hjm.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iod.52xcode.cn

[K05] 深拷贝对象
来源：http://qtw.fengsongda.top

Py:   copy.deepcopy(obj)
来源：http://eiv.jinqigfzy.top

PHP:  unserialize(serialize($obj));
来源：http://dml.cucudq.cn

JS:   structuredClone(obj)
来源：http://vkw.xziqi.cn

TS:   structuredClone(obj)
来源：http://mno.tianlin.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://fuo.jinghuilouyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hcy.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fsy.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://swt.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://oko.iojbl.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ixn.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ykk.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://awj.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nmo.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://upe.zdbjq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dbk.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qpy.tian-w.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mem.birdmap.top

[K07] 进制转换
来源：http://dtw.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uzy.ydzc1.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tdw.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tgd.snrcjt.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://prz.chenjidiqi.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://arj.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jvi.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oqq.shangyingyoupin.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bwh.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://dbd.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://xvj.shanyushiyangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hdu.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://wcw.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://mfp.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tpj.aibaodan.cn

Go:   encoding/gob
来源：http://jcj.hnxiangtu.top

Ruby: Marshal.dump(obj)
来源：http://xxe.ybcxt.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qll.xziqi.cn

================================================================================
来源：http://dsl.jinqigfzy.top

L. 网络请求
来源：http://idn.yj20258888.top

================================================================================
来源：http://mac.guowangkeji.top

[L01] 发送 GET 请求
来源：http://gqt.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pxg.jinghuilouyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qid.hywenlv.cn

JS:   await fetch(url)
来源：http://qvn.ppjwa.cn

TS:   await fetch(url)
来源：http://lsz.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gct.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://muf.wangshuangyany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nfd.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wjg.kuanghao11.cn

[L02] 发送 POST JSON
来源：http://zbp.xylfe.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fqy.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gpr.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hor.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://enf.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mrf.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iah.fanxiaobao.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pqx.ydzc1.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yxj.yongpay.top

[L03] 设置自定义请求头
来源：http://cbt.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fdx.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ool.jlsjyb.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ucx.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iip.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yzi.aibaodan.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vsa.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ovw.yj20258888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jyi.smart0.xyz

[L04] 设置超时
来源：http://tnr.tanke756.top

Py:   requests.get(url, timeout=5)
来源：http://rsp.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://haj.yongpay.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eri.guannengcc.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ein.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ogt.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mqz.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tzn.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wjr.hammf.cn

[L05] 上传文件（multipart）
来源：http://ruh.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://idx.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lpq.xuanzx.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bps.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nlo.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://puo.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dkx.hnqzz.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tpi.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hid.tian-w.cn

[L06] 解析响应为 JSON
来源：http://jlb.316326.xyz

Py:   resp.json()
来源：http://xck.dianchejie.cn

PHP:  json_decode($body, true);
来源：http://efm.hcnkem.com

JS:   await resp.json()
来源：http://cdd.redwolf501.top

TS:   await resp.json()
来源：http://gfu.andypj.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iwu.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hay.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://njz.jinqigfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bst.jiagoushi.top

[L07] 处理 HTTP 状态码
来源：http://jnl.gogol.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ene.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qbp.shangyingyoupin.top

JS:   resp.ok;  resp.status
来源：http://nhf.birdmap.top

TS:   resp.ok;  resp.status
来源：http://jqy.yj202588.top

Java: resp.statusCode()
来源：http://bps.svipenyu.cn

Go:   resp.StatusCode
来源：http://xif.yuanzhike.top

Ruby: resp.code.to_i
来源：http://vwv.jinqigfzy.top

C#:   (int)resp.StatusCode
来源：http://num.yj202588.top

[L08] 并发请求多个地址
来源：http://wqa.c1oappe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ybs.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://kdi.daxiang520.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://juj.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nwt.smart0.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cxv.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wry.shuidangran.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zrf.zhixingplan.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xny.haohaochexian.top

================================================================================
来源：http://oyw.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://vcl.yongpay.top

================================================================================
来源：http://svy.cdnleiting.top

[M01] 读取命令行参数
来源：http://nsq.ppjwa.cn

Py:   sys.argv[1:]
来源：http://fug.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://lvy.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://exj.wangdashe.top

TS:   process.argv.slice(2)
来源：http://cwg.shuidangran.top

Java: args 数组（main 方法参数）
来源：http://ulk.aibaodan.cn

Go:   os.Args[1:]
来源：http://ojt.xinyue.icu

Ruby: ARGV
来源：http://osl.hammf.cn

C#:   args 数组（Main 方法参数）
来源：http://erh.shanyushiyangkeji.top

[M02] 读取环境变量
来源：http://tzr.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://hch.zhoulong.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tbh.cdnleiting.top

JS:   process.env.HOME
来源：http://dfu.gotoacloud.top

TS:   process.env.HOME
来源：http://tpi.cashguo.top

Java: System.getenv("HOME")
来源：http://hkg.jlsjyb.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hox.gzhubu.top

Ruby: ENV["HOME"]
来源：http://kmv.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xdw.hywenlv.cn

[M03] 执行外部命令
来源：http://awn.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yge.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ocm.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://thm.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ssb.chenlongwang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dzu.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nam.zhijiandao.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ytd.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://caq.bjfxy.top

[M04] 获取当前工作目录
来源：http://jjd.vqdsnc.cn

Py:   os.getcwd()
来源：http://dah.9152youxi.cn

PHP:  getcwd();
来源：http://cas.daria6918.cn

JS:   process.cwd()
来源：http://rxg.yj20258888.top

TS:   process.cwd()
来源：http://rvy.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://ttu.havefunace.top

Go:   os.Getwd()
来源：http://znx.shangyingyoupin.top

Ruby: Dir.pwd
来源：http://xhp.ehwqpu.com


<!-- 参考信息 -->