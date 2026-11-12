代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bwz.tian-w.cn

TS:   /error/gim
来源：http://kxv.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eme.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xxg.bjfxy.top

Ruby: s.scan(/error/i)
来源：http://zvx.zhoulong.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://alh.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://bzn.jqgfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ghr.ivvv.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wqu.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ozg.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jec.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dbk.guowangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fri.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lfd.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gsk.bbcook.cn

================================================================================
来源：http://ovq.aibaodan.cn

J. 日期与时间
来源：http://ufj.meibo888.top

================================================================================
来源：http://kbn.zhongyouzk.top

[J01] 获取当前时间
来源：http://ses.chenzaomai.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://qpm.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://afq.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://zwj.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://alg.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wpp.shanyushiyangkeji.top

Go:   time.Now()
来源：http://mlr.hfpthk.cn

Ruby: Time.now
来源：http://wlm.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lqi.cashguo.top

[J02] 格式化输出
来源：http://ygb.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ocg.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://efs.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fmz.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://kly.ctjpmb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dia.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yoi.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://let.hysaishi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tyv.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://nxy.hfpthk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mpd.shanyushiyangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://elr.yuxming.cn

JS:   new Date("2024-01-02")
来源：http://caj.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://fpk.cqqwz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ptn.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ujn.uphjek.com

Ruby: Date.parse("2024-01-02")
来源：http://ogv.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vah.52xcode.cn

[J04] 时间戳与日期互转
来源：http://bya.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jfo.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fwq.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://egk.tarul.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pcg.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nmb.fehbvm.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ifj.dianchejie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iph.daria6918.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ueq.xuetiantiany.cn

[J05] 时间加减（加 7 天）
来源：http://yrf.haohaochexian.top

Py:   now + timedelta(days=7)
来源：http://lev.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://imu.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sgg.xinyue.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mmr.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://ocs.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jtb.daxiang520.top

Ruby: Time.now + 7 * 86400
来源：http://ldr.tianlin.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://nux.zdbjq.cn

[J06] 计算两时间之差
来源：http://zlc.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://qgl.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://bmg.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lss.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dvp.epnwcf.com

Java: Duration.between(start, end).toSeconds()
来源：http://wcg.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://xin.fehbvm.com

Ruby: end - start                 # 返回秒数
来源：http://vek.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://hoe.fengsongda.top

[J07] 比较两个日期
来源：http://kpr.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://qfy.tian-w.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ugt.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://edq.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://jaf.smart0.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gjw.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nks.ivvv.top

Ruby: d1 < d2;  d1 == d2
来源：http://wxo.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://lxs.tianlin.xyz

[J08] 提取年月日与星期
来源：http://mds.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iql.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qas.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mdp.tanke756.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://joc.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dog.tarul.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vfs.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lwj.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://adq.chenjidiqi.icu

[J09] 时区处理
来源：http://kgb.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fgq.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rbq.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lag.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://odm.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ekz.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hfr.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vww.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zaz.hywenlv.cn

[J10] 取今天 / 本月第一天
来源：http://gcb.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gka.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://psb.hysaishi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://khe.wangdashe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bxs.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qsn.guowangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xln.zycfv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ify.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ous.yuanzhike.top

================================================================================
来源：http://vtd.jlsjyb.cn

K. JSON 与序列化
来源：http://ogd.daria6918.cn

================================================================================
来源：http://tia.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://qwy.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jcf.gotoacloud.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zmd.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://zce.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://gqs.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gjl.ydjk.org.cn

Go:   json.Marshal(obj)
来源：http://laj.jianghu66.top

Ruby: obj.to_json                                     // require "json"
来源：http://leb.ivvv.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rpi.jinghuilouyu.cn

[K02] JSON 字符串转对象
来源：http://jcd.zycfv.cn

Py:   json.loads(s)
来源：http://ggg.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xyf.fengsongda.top

JS:   JSON.parse(s)
来源：http://kpg.jinghuilouyu.cn

TS:   JSON.parse(s)
来源：http://izh.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kss.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://dws.hongshengwenyu.top

Ruby: JSON.parse(s)
来源：http://yir.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jca.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://rjv.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ybr.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vil.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jjk.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://agn.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tuf.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ssg.shuidangran.top

Ruby: JSON.pretty_generate(obj)
来源：http://bgn.snrcjt.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nkm.hywenlv.cn

[K04] 读取 JSON 文件
来源：http://ymr.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cww.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mfz.aibaodan.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hnd.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nme.c1oappe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xfu.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fhc.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wrm.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vyp.ivvv.top

[K05] 深拷贝对象
来源：http://dav.pycfn.com

Py:   copy.deepcopy(obj)
来源：http://dpb.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://wwi.gzhubu.top

JS:   structuredClone(obj)
来源：http://vhk.bjfxy.top

TS:   structuredClone(obj)
来源：http://wdw.jlsjyb.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tqy.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vea.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xyh.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dud.hesvh.cn

[K06] 解析 URL 查询串
来源：http://ygy.yj202588.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://thq.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pey.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://akq.jqgfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tgt.9152youxi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bpg.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ftb.hfpthk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://enk.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lro.cqqwz.cn

[K07] 进制转换
来源：http://puy.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zdr.zhixingplan.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mgc.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jwt.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yto.dianchejie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gmd.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gmb.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jrl.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pzo.uphjek.com

[K08] 二进制序列化（非 JSON）
来源：http://avx.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://dfb.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dic.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://rsi.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://abt.zdqjudy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xvn.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://qlm.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://ftj.gogol.net.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oqv.hammf.cn

================================================================================
来源：http://wrv.fzhhl.top

L. 网络请求
来源：http://npx.shanyushiyangkeji.top

================================================================================
来源：http://npf.tian-w.cn

[L01] 发送 GET 请求
来源：http://jbq.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rgu.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hfi.fengsongda.top

JS:   await fetch(url)
来源：http://xgj.yj20258888.top

TS:   await fetch(url)
来源：http://yha.9152youxi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bxk.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://fwl.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gzu.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xfx.meibo888.top

[L02] 发送 POST JSON
来源：http://ynw.yuxming.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qgg.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://atz.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://shj.fengsongda.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lxg.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oav.cucudq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://asd.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lqt.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cfa.sufxvd.cn

[L03] 设置自定义请求头
来源：http://yvx.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mgd.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mar.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jzy.jinghuilouyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sgs.sweek.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qcq.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ifn.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qqt.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xws.zhijiandao.cn

[L04] 设置超时
来源：http://upe.316326.xyz

Py:   requests.get(url, timeout=5)
来源：http://vno.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nbq.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vgx.yj20258.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dqi.jianghu66.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bel.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jov.quarkkingdee.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ejy.sweek.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gdo.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://nlv.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ube.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fuw.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mpi.pengpengdd.cyou

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oja.c1oappe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bqb.bjfxy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tyd.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qyy.xziqi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yii.jianghu66.top

[L06] 解析响应为 JSON
来源：http://jyi.tian-w.cn

Py:   resp.json()
来源：http://ehe.tian-w.cn

PHP:  json_decode($body, true);
来源：http://owu.redwolf501.top

JS:   await resp.json()
来源：http://yto.yuanzhike.top

TS:   await resp.json()
来源：http://zqz.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yow.jinghuilouyu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pur.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://vwx.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://boo.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://aey.jianghu66.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tqz.yangfankeji.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://roc.zdbjq.cn

JS:   resp.ok;  resp.status
来源：http://kla.iojbl.cn

TS:   resp.ok;  resp.status
来源：http://npg.jinqigufen.top

Java: resp.statusCode()
来源：http://igw.quarkkingdee.top

Go:   resp.StatusCode
来源：http://pry.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://zvr.zhixingplan.top

C#:   (int)resp.StatusCode
来源：http://ygg.xingfuxueyuan.xyz

[L08] 并发请求多个地址
来源：http://xjk.ivvv.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eak.wangshuangyany.cn

PHP:  curl_multi_init() 系列
来源：http://mhb.316326.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jof.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dpq.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xga.tian-w.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jdy.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aed.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fwq.smart0.xyz

================================================================================
来源：http://rgf.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://rmz.iojbl.cn

================================================================================
来源：http://vrk.fanxiaobao.xyz

[M01] 读取命令行参数
来源：http://yei.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://gsf.jlsjyb.cn

PHP:  $argv;  $argc;
来源：http://qqf.shuidangran.top

JS:   process.argv.slice(2)
来源：http://say.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://mpq.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://ois.bbcook.cn

Go:   os.Args[1:]
来源：http://yty.shanyushiyangtech.top

Ruby: ARGV
来源：http://anx.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://ybe.hnxiangtu.top

[M02] 读取环境变量
来源：http://lsj.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://vmc.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uej.hnqzz.top

JS:   process.env.HOME
来源：http://vzf.shanyushiyangkeji.top

TS:   process.env.HOME
来源：http://cqr.jinqigufen.top

Java: System.getenv("HOME")
来源：http://tor.birdmap.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dxq.jianghu66.top

Ruby: ENV["HOME"]
来源：http://avg.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ckf.yueranfly.top

[M03] 执行外部命令
来源：http://rzr.birdmap.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vpc.jinyuanbaomall.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mwp.fzhhl.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rnp.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://emw.hongshengwenyu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rjy.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qtc.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://znc.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://sqg.gotoacloud.top

[M04] 获取当前工作目录
来源：http://hab.hongshengwenyu.top

Py:   os.getcwd()
来源：http://qcg.ppjwa.cn

PHP:  getcwd();
来源：http://ait.52xcode.cn

JS:   process.cwd()
来源：http://ihr.jyoumei.cn

TS:   process.cwd()
来源：http://nwc.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://kyf.ivvv.top

Go:   os.Getwd()
来源：http://yxp.zycfv.cn

Ruby: Dir.pwd
来源：http://yre.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vvt.smart0.xyz

[M05] 设置退出码
来源：http://unv.cucudq.cn

Py:   sys.exit(1)
来源：http://anf.gotoacloud.top

PHP:  exit(1);
来源：http://xjg.jinqigufen.top


<!-- 参考信息 -->