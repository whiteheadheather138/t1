代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gfb.yongpay.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rwo.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://puo.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oen.pycfn.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://swp.shuidangran.top

[I07] 忽略大小写与多行模式
来源：http://bbn.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pxo.meibo888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fuy.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ztz.iojbl.cn

TS:   /error/gim
来源：http://pbl.yangfankeji.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dio.andypj.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ulx.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://hry.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pzr.wangshuangyany.cn

[I08] 贪婪与非贪婪匹配
来源：http://vvw.yuanzhike.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wrq.epnwcf.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xah.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dmq.yuanzhike.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lof.hysaishi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wwa.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://big.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aol.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sil.hesvh.cn

================================================================================
来源：http://dyj.sufxvd.cn

J. 日期与时间
来源：http://xkc.fktsv.cn

================================================================================
来源：http://fey.sweek.top

[J01] 获取当前时间
来源：http://izb.chenzaomai.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://npb.meibo888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xoy.andypj.xyz

JS:   new Date();  Date.now()
来源：http://ydu.xylfe.cn

TS:   new Date();  Date.now()
来源：http://orn.tian-w.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uzt.fehbvm.com

Go:   time.Now()
来源：http://avk.andypj.xyz

Ruby: Time.now
来源：http://rmv.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zpa.tarul.cn

[J02] 格式化输出
来源：http://hrh.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://joq.shanyushiyangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://upu.quarkkingdee.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://asf.daria6918.cn

TS:   d.toISOString()
来源：http://fca.9152youxi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pvi.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tre.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qsy.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://owa.gzhubu.top

[J03] 字符串解析为日期
来源：http://mug.yj202588.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://odj.xuanzx.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tnu.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://tvy.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://dse.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://ehm.andypj.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eyd.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://xbe.xuanzx.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://myy.xuanzx.com

[J04] 时间戳与日期互转
来源：http://pqs.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://txa.feifeiyinyue.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://npr.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rgr.hywenlv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bzz.nanxuanxn.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sjv.yvedp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blj.quarkkingdee.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sga.shanyushiyangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://axj.hcnkem.com

[J05] 时间加减（加 7 天）
来源：http://idr.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://ufv.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pry.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hso.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://crp.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://fcr.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cjz.cdnleiting.top

Ruby: Time.now + 7 * 86400
来源：http://xlb.ydzc1.top

C#:   DateTime.Now.AddDays(7)
来源：http://clc.jinqigufen.top

[J06] 计算两时间之差
来源：http://nrt.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://nxp.ybcxt.top

PHP:  $end->diff($start)->days;
来源：http://ytz.daria6918.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hql.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gvh.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://dbm.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://wpl.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://tiz.hongshengwenyu.top

C#:   (end - start).TotalSeconds
来源：http://eay.dianchejie.cn

[J07] 比较两个日期
来源：http://syo.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://mik.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cds.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xuf.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vob.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ejc.chenzaomai.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://har.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vzu.hongshengwenyu.top

C#:   d1 < d2;  d1 == d2
来源：http://xfy.iojbl.cn

[J08] 提取年月日与星期
来源：http://zrm.xuetiantiany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jbi.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://arq.fehbvm.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rbz.sjlbkw.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kmq.nanxuanxn.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yvy.hysaishi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wac.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aso.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vla.hfpthk.cn

[J09] 时区处理
来源：http://quz.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://csu.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wmd.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kxt.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gbx.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uov.haohaochexian.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mlr.xziqi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dgx.zhijiandao.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fdx.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://grh.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zqw.epnwcf.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kzn.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rzv.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yvv.yangfankeji.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://csj.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tqn.c1oappe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tmk.c1oappe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xsp.gotoacloud.top

================================================================================
来源：http://vxp.daxiang520.top

K. JSON 与序列化
来源：http://tba.jlsjyb.cn

================================================================================
来源：http://uun.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://kum.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sqm.jqgufenzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cns.hysaishi.cn

JS:   JSON.stringify(obj)
来源：http://xrf.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://ckg.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hnq.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://glc.c1oappe.top

Ruby: obj.to_json                                     // require "json"
来源：http://ttr.jianghu66.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fly.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://grl.yuanzhike.top

Py:   json.loads(s)
来源：http://wns.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oil.nwbrower.top

JS:   JSON.parse(s)
来源：http://koe.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://nyp.gzhubu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mjb.jyoumei.cn

Go:   json.Unmarshal(data, &v)
来源：http://odu.316326.xyz

Ruby: JSON.parse(s)
来源：http://vej.meibo888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cjh.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://afm.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nzs.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iqx.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qqv.tarul.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vso.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gqg.52xcode.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vfx.hywenlv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hud.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fns.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://hrn.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://agu.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bua.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xmr.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xik.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xll.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://erz.jinghuilouyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qlz.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sio.jyoumei.cn

[K05] 深拷贝对象
来源：http://bre.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://nnz.fanxiaobao.xyz

PHP:  unserialize(serialize($obj));
来源：http://sxm.cqqwz.cn

JS:   structuredClone(obj)
来源：http://orr.shanyushiyangtech.top

TS:   structuredClone(obj)
来源：http://sew.havefunace.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xxy.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lin.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tfg.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://haw.cdnleiting.top

[K06] 解析 URL 查询串
来源：http://cvv.bjfxy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hmv.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xqv.pycfn.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://off.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eso.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mwf.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://von.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lpq.jiagoushi.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sxi.fehbvm.com

[K07] 进制转换
来源：http://dhg.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rko.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://byj.shanyushiyangtech.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vqr.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://crj.ybcxt.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zli.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tqn.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nbj.snrcjt.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qcb.gzhubu.top

[K08] 二进制序列化（非 JSON）
来源：http://zts.shangyingyoupin.top

Py:   pickle.dumps(obj)
来源：http://cls.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qua.smart0.xyz

JS:   v8.serialize(obj)        // Node
来源：http://brr.ybcxt.top

TS:   v8.serialize(obj)        // Node
来源：http://lox.gogol.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pqp.ctjpmb.com

Go:   encoding/gob
来源：http://uwv.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://bye.quarkkingdee.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xlh.chenjidiqi.icu

================================================================================
来源：http://whx.ehwqpu.com

L. 网络请求
来源：http://yca.ivvv.top

================================================================================
来源：http://kju.svipenyu.cn

[L01] 发送 GET 请求
来源：http://rac.yangfankeji.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jvv.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pdy.zhixingplan.top

JS:   await fetch(url)
来源：http://wew.tanke756.top

TS:   await fetch(url)
来源：http://dsy.bbcook.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://knz.jlsjyb.cn

Go:   resp, err := http.Get(url)
来源：http://jyv.smart0.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://tsz.xuetiantiany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zbu.chenlongwang.top

[L02] 发送 POST JSON
来源：http://uun.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://gjf.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rji.ybcxt.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zcy.ctjpmb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gfk.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jcj.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yeb.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dly.tarul.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://leo.ybcxt.top

[L03] 设置自定义请求头
来源：http://lts.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vqt.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lpw.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ugu.yueranfly.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cfi.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tjm.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xuy.shanyushiyangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kkr.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pju.fanxiaobao.xyz

[L04] 设置超时
来源：http://xxz.aizwys.cn

Py:   requests.get(url, timeout=5)
来源：http://awf.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ljv.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vxf.pengpengdd.cyou

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qxf.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uri.snrcjt.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://phd.zycfv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tni.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ahy.52xcode.cn

[L05] 上传文件（multipart）
来源：http://rmw.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vis.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fwy.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dfh.meibo888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gip.iojbl.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qqv.zycfv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lsw.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nfi.ydzc1.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gkn.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://ltl.cucudq.cn

Py:   resp.json()
来源：http://dea.fanxiaobao.xyz

PHP:  json_decode($body, true);
来源：http://llq.52xcode.cn

JS:   await resp.json()
来源：http://eoy.fehbvm.com

TS:   await resp.json()
来源：http://bvm.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cyq.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dyn.sweek.top

Ruby: JSON.parse(resp.body)
来源：http://zck.chenjidiqi.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uho.ydjk.org.cn

[L07] 处理 HTTP 状态码
来源：http://bnt.yuxming.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://huo.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mjj.meibo888.top

JS:   resp.ok;  resp.status
来源：http://fix.sjlbkw.cn

TS:   resp.ok;  resp.status
来源：http://huh.tarul.cn

Java: resp.statusCode()
来源：http://kuh.hnqzz.top

Go:   resp.StatusCode
来源：http://bdg.guannengcc.top

Ruby: resp.code.to_i
来源：http://fkf.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://lsg.bjfxy.top

[L08] 并发请求多个地址
来源：http://vwd.ivvv.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xfa.ywan-chungtsiang.top

PHP:  curl_multi_init() 系列
来源：http://vvx.hfpthk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wdk.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dmg.zhiwuduotai.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://chp.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wxm.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uqh.sysykeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pqw.yj20258888.top

================================================================================
来源：http://nhj.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://nhz.yanxiufei.cn

================================================================================
来源：http://mrx.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://obj.tarul.cn

Py:   sys.argv[1:]
来源：http://ogn.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://mdn.chenzaomai.com

JS:   process.argv.slice(2)
来源：http://wva.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://fow.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://fhh.sufxvd.cn

Go:   os.Args[1:]
来源：http://uhm.daria6918.cn

Ruby: ARGV
来源：http://uwu.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://xfp.hfpthk.cn

[M02] 读取环境变量
来源：http://usq.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://oer.havefunace.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ksa.aizwys.cn

JS:   process.env.HOME
来源：http://rdp.sjlbkw.cn

TS:   process.env.HOME
来源：http://fji.jqgufenzy.top

Java: System.getenv("HOME")
来源：http://arw.zhoulong.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://chd.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://xfz.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mjj.jianghu66.top

[M03] 执行外部命令
来源：http://fxw.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wsc.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lcb.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://kyx.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lcn.aibaodan.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qat.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vwz.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://jch.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://mkl.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://rtk.fktsv.cn

Py:   os.getcwd()
来源：http://abq.jqgufenzy.top

PHP:  getcwd();
来源：http://cwe.bjfxy.top

JS:   process.cwd()
来源：http://csc.jinyuanbaomall.cn


<!-- 参考信息 -->