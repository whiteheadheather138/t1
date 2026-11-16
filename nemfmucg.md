代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tyo.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wdh.zhongyouzk.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pbv.ydjk.org.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mgv.gaohongyu789.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qqx.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mpw.hesvh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://okk.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dno.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://slu.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://own.hysaishi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bgp.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cmz.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://htq.xziqi.cn

TS:   /error/gim
来源：http://ghk.sweek.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pdd.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sur.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://uas.meibo888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yzw.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://glu.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cmk.xylfe.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dfv.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hmv.ehwqpu.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ebk.hnqzz.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zkd.dashuyun.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tkw.yuanzhike.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://irh.wangdashe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vge.yongpay.top

================================================================================
来源：http://mct.ybcxt.top

J. 日期与时间
来源：http://dij.jinghuilouyu.cn

================================================================================
来源：http://uog.jinqigufen.top

[J01] 获取当前时间
来源：http://krl.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://klj.fzhhl.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ydb.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://tox.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://dhk.ydjk.org.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rtf.sjlbkw.cn

Go:   time.Now()
来源：http://joh.cucudq.cn

Ruby: Time.now
来源：http://ama.pengpengdd.cyou

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ljc.chenzaomai.com

[J02] 格式化输出
来源：http://qvp.sysykeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://txk.smart0.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jmf.ydjk.org.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dym.yvedp.cn

TS:   d.toISOString()
来源：http://urt.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jyl.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hog.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nrt.zdbjq.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://coq.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://nzn.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://unx.sjlbkw.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://llx.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://pft.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://vsd.ywan-chungtsiang.top

Java: LocalDate.parse("2024-01-02")
来源：http://svo.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zzg.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://ofk.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fcq.wangdashe.top

[J04] 时间戳与日期互转
来源：http://orr.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qjy.jqgufenzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qcb.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rtd.svipenyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ikl.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tuj.iojbl.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nja.fktsv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ruq.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tel.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://gcr.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://hvz.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://heq.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kjd.zhongyouzk.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yjf.shanyushiyangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://yrz.zhiwuduotai.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dnz.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://gkd.yanxiufei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vja.smart0.xyz

[J06] 计算两时间之差
来源：http://qnc.xingfuxueyuan.xyz

Py:   (end - start).total_seconds()
来源：http://dyr.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://gsy.chenzaomai.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dwa.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qyq.birdmap.top

Java: Duration.between(start, end).toSeconds()
来源：http://iwh.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://vcs.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://hea.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://ixd.cheryme.top

[J07] 比较两个日期
来源：http://qzn.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://zai.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://amc.ywan-chungtsiang.top

JS:   d1.getTime() < d2.getTime()
来源：http://smi.yj202588.top

TS:   d1.getTime() < d2.getTime()
来源：http://miz.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qyp.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eek.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qhk.tian-w.cn

C#:   d1 < d2;  d1 == d2
来源：http://uhz.zhaomingkeji.xyz

[J08] 提取年月日与星期
来源：http://kol.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wcs.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ohh.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ynh.kuanghao11.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jwd.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xra.chenlongwang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://odv.ppjwa.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nja.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lwk.ppjwa.cn

[J09] 时区处理
来源：http://xvn.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tdw.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fty.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tep.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zry.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eym.sufxvd.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cpa.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://als.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nib.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://dqc.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://lyf.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tsu.ehwqpu.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://skc.xinyue.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nsy.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bio.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qrf.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gfz.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sav.jinqigfzy.top

================================================================================
来源：http://fpj.yj20258888.top

K. JSON 与序列化
来源：http://nql.iojbl.cn

================================================================================
来源：http://wpf.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://aqd.quarkkingdee.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xsd.quarkkingdee.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nmm.havefunace.top

JS:   JSON.stringify(obj)
来源：http://bqf.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://qsw.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pai.xylfe.cn

Go:   json.Marshal(obj)
来源：http://nqv.shanyushiyangtech.top

Ruby: obj.to_json                                     // require "json"
来源：http://uwu.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://utq.fzhhl.top

[K02] JSON 字符串转对象
来源：http://ufs.zhiwuduotai.top

Py:   json.loads(s)
来源：http://vso.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rei.redwolf501.top

JS:   JSON.parse(s)
来源：http://eud.cheryme.top

TS:   JSON.parse(s)
来源：http://fwo.zdbjq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oel.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://snc.ywan-chungtsiang.top

Ruby: JSON.parse(s)
来源：http://gxk.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pcv.fktsv.cn

[K03] JSON 美化输出（带缩进）
来源：http://pst.sysykeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dsg.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tls.vehdjk.com

JS:   JSON.stringify(obj, null, 2)
来源：http://bef.zhongyouzk.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ghg.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cvp.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ctj.yfazqb.com

Ruby: JSON.pretty_generate(obj)
来源：http://cwq.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rst.birdmap.top

[K04] 读取 JSON 文件
来源：http://kvl.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zgd.kuanghao11.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ysz.havefunace.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://orr.ydzc1.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dfo.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eiw.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fax.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jdf.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dkh.aizwys.cn

[K05] 深拷贝对象
来源：http://ueg.gogol.net.cn

Py:   copy.deepcopy(obj)
来源：http://krn.jinqigfzy.top

PHP:  unserialize(serialize($obj));
来源：http://ctr.sxryk.cn

JS:   structuredClone(obj)
来源：http://ctm.tianlin.xyz

TS:   structuredClone(obj)
来源：http://ffz.shangyingyoupin.top

Java: // 手写拷贝构造，或序列化往返
来源：http://scr.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rsv.hnxiangtu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oax.sufxvd.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kfj.sxryk.cn

[K06] 解析 URL 查询串
来源：http://svq.shzxlz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sas.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gqm.daria6918.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rrg.daria6918.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rve.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nro.xuanzx.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://myu.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hni.52xcode.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tpj.pycfn.com

[K07] 进制转换
来源：http://byn.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gfx.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qkc.pycfn.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wcr.daria6918.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kse.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uzp.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://quj.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nou.hesvh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nzc.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://mou.snrcjt.cn

Py:   pickle.dumps(obj)
来源：http://cjt.cdnleiting.top

PHP:  serialize($obj);  unserialize($s);
来源：http://luf.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://rvm.yonumen.top

TS:   v8.serialize(obj)        // Node
来源：http://cks.jinqigfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kju.yueranfly.top

Go:   encoding/gob
来源：http://dui.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://kan.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bgu.fanxiaobao.xyz

================================================================================
来源：http://gep.chenzaomai.com

L. 网络请求
来源：http://yvt.yuxming.cn

================================================================================
来源：http://vwk.zhengqikj.top

[L01] 发送 GET 请求
来源：http://ikl.andypj.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sku.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yqn.havefunace.top

JS:   await fetch(url)
来源：http://xow.sjlbkw.cn

TS:   await fetch(url)
来源：http://ldq.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nqe.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://dex.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sti.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://psi.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://anu.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://chk.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pbi.hammf.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://weg.jianghu66.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yid.ivvv.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oln.nanxinkj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vfi.fktsv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bba.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uve.gogol.net.cn

[L03] 设置自定义请求头
来源：http://qan.gogol.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xnf.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://plb.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zpt.gzhubu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lot.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pjn.hysaishi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oev.fanxiaobao.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xiv.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tgi.gzhubu.top

[L04] 设置超时
来源：http://inj.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://qmr.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vik.jqgufenzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://abd.aibaodan.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bbx.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dos.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lea.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vsz.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dso.shuidangran.top

[L05] 上传文件（multipart）
来源：http://ixz.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://psa.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yto.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mny.gogol.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zjz.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kvd.zhiwuduotai.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lts.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yyv.ctjpmb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xed.hammf.cn

[L06] 解析响应为 JSON
来源：http://wwu.birdmap.top

Py:   resp.json()
来源：http://ltr.yueranfly.top

PHP:  json_decode($body, true);
来源：http://jzf.zhongyouzk.top

JS:   await resp.json()
来源：http://uii.daxiang520.top

TS:   await resp.json()
来源：http://zyz.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://plu.shzxlz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tsh.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://hdz.316326.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gbw.jqgufenzy.top

[L07] 处理 HTTP 状态码
来源：http://flj.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uvi.nwbrower.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://snv.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://oyc.cdnleiting.top

TS:   resp.ok;  resp.status
来源：http://oft.yj202588.top

Java: resp.statusCode()
来源：http://acf.hnqzz.top

Go:   resp.StatusCode
来源：http://nfh.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://dxj.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://ued.xuanzx.com

[L08] 并发请求多个地址
来源：http://yut.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nkp.xinyue.icu

PHP:  curl_multi_init() 系列
来源：http://suj.tianlin.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gdi.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://prp.vqdsnc.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iwb.zhijiandao.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hmu.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kmr.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qob.epnwcf.com

================================================================================
来源：http://opm.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://zwk.hnqzz.top

================================================================================
来源：http://url.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://oph.havefunace.top

Py:   sys.argv[1:]
来源：http://ban.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://dpd.fanxiaobao.xyz

JS:   process.argv.slice(2)
来源：http://hez.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://zfb.jinqigufen.top

Java: args 数组（main 方法参数）
来源：http://zhw.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://ued.cqqwz.cn

Ruby: ARGV
来源：http://iyf.hfpthk.cn

C#:   args 数组（Main 方法参数）
来源：http://azv.hfpthk.cn

[M02] 读取环境变量
来源：http://ljy.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://ecu.daria6918.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wwu.wangdashe.top

JS:   process.env.HOME
来源：http://pez.zhongyouzk.top

TS:   process.env.HOME
来源：http://din.yuanzhike.top

Java: System.getenv("HOME")
来源：http://tjg.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mex.cucudq.cn

Ruby: ENV["HOME"]
来源：http://pwv.zhoulong.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zyx.guannengcc.top

[M03] 执行外部命令
来源：http://gbm.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vpx.ydzc1.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ixr.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://hdl.jiagoushi.top

TS:   child_process.execSync("ls -l").toString()
来源：http://uel.xuanzx.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kox.ydzc1.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dfn.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wul.shuidangran.top

C#:   Process.Start("ls", "-l");
来源：http://zsx.zdbjq.cn


<!-- 参考信息 -->