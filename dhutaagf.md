代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ogk.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xzf.ybcxt.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://imt.jlsjyb.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rmq.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ogx.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dzg.sysykeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jsl.dianchejie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lgd.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mjg.bjfxy.top

[I07] 忽略大小写与多行模式
来源：http://uqv.sufxvd.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rsi.nanxinkj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wrk.epnwcf.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://awd.kuanghao11.cn

TS:   /error/gim
来源：http://iqk.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rlo.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ygl.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://zxr.jqgufenzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bhs.hnqzz.top

[I08] 贪婪与非贪婪匹配
来源：http://cdq.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qtz.xylfe.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iil.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nwm.ybcxt.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pbr.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://dyy.0kj1m.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vbk.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tjc.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pry.sysykeji.top

================================================================================
来源：http://akb.aizwys.cn

J. 日期与时间
来源：http://ndo.gzhubu.top

================================================================================
来源：http://nuu.ydzc1.top

[J01] 获取当前时间
来源：http://qwt.chenlongwang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yyj.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zfp.ppjwa.cn

JS:   new Date();  Date.now()
来源：http://ezr.jlsjyb.cn

TS:   new Date();  Date.now()
来源：http://urv.ydjk.org.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bbv.pycfn.com

Go:   time.Now()
来源：http://omf.ehwqpu.com

Ruby: Time.now
来源：http://vru.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pur.sysykeji.top

[J02] 格式化输出
来源：http://mtf.aibaodan.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rhe.iojbl.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lzi.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hbx.gotoacloud.top

TS:   d.toISOString()
来源：http://frs.gaohongyu789.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gmz.gotoacloud.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rhs.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://msw.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kle.jyoumei.cn

[J03] 字符串解析为日期
来源：http://hzx.yj20258.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ejj.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://okm.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://kjp.mhx1999.top

TS:   new Date("2024-01-02")
来源：http://nhl.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jta.chenjidiqi.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tsb.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://ipf.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ics.hnqzz.top

[J04] 时间戳与日期互转
来源：http://ueb.yuxming.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bjw.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qwq.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gzf.tarul.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bso.dashuyun.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wys.jlsjyb.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lhz.kuanghao11.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bdr.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vjo.ctjpmb.com

[J05] 时间加减（加 7 天）
来源：http://qni.fanxiaobao.xyz

Py:   now + timedelta(days=7)
来源：http://wmd.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bgb.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pvc.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hgp.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://cew.vehdjk.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hhw.gotoacloud.top

Ruby: Time.now + 7 * 86400
来源：http://zjx.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qfc.jinqigfzy.top

[J06] 计算两时间之差
来源：http://wva.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://vwl.zhaomingkeji.xyz

PHP:  $end->diff($start)->days;
来源：http://hta.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://upx.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hvo.zhoulong.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://wkq.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://pzc.ctjpmb.com

Ruby: end - start                 # 返回秒数
来源：http://srp.hnxiangtu.top

C#:   (end - start).TotalSeconds
来源：http://uer.meibo888.top

[J07] 比较两个日期
来源：http://mot.ywan-chungtsiang.top

Py:   d1 < d2;  d1 == d2
来源：http://gjy.yvedp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vbw.ctjpmb.com

JS:   d1.getTime() < d2.getTime()
来源：http://rdt.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://idk.xinyue.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mdp.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sta.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://qte.xingfuxueyuan.xyz

C#:   d1 < d2;  d1 == d2
来源：http://dsp.nanxinkj.top

[J08] 提取年月日与星期
来源：http://fdc.sysykeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sbh.jyoumei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://znj.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kgh.hysaishi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aqa.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bez.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gae.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xuh.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://les.ywan-chungtsiang.top

[J09] 时区处理
来源：http://ogg.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aar.bbcook.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uli.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://akg.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://whk.jlsjyb.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tkf.jinghuilouyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wdb.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://bzc.shzxlz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iao.tanke756.top

[J10] 取今天 / 本月第一天
来源：http://llx.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rap.ivvv.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dza.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pdn.hcnkem.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fdy.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://alp.zycfv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hkz.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lpe.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nqr.jqgufenzy.top

================================================================================
来源：http://eaj.jqgfzy.top

K. JSON 与序列化
来源：http://ofi.cheryme.top

================================================================================
来源：http://bdd.nwbrower.top

[K01] 对象转 JSON 字符串
来源：http://tqr.zhiwuduotai.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gxz.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yhy.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://fyg.jinyuanbaomall.cn

TS:   JSON.stringify(obj)
来源：http://vyt.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ksq.jiagoushi.top

Go:   json.Marshal(obj)
来源：http://rdz.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://qxz.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://blw.fengsongda.top

[K02] JSON 字符串转对象
来源：http://ybw.zycfv.cn

Py:   json.loads(s)
来源：http://bpw.nwbrower.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fxd.xuetiantiany.cn

JS:   JSON.parse(s)
来源：http://egw.zhoulong.xyz

TS:   JSON.parse(s)
来源：http://lst.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uai.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://lvl.birdmap.top

Ruby: JSON.parse(s)
来源：http://ndg.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://acx.hywenlv.cn

[K03] JSON 美化输出（带缩进）
来源：http://wxq.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hze.wangdashe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kei.shangyingyoupin.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dps.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qbn.tian-w.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://esn.jinghuilouyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fuw.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rms.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pfw.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://sqt.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wke.jqgufenzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://opi.cqqwz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kgf.redwolf501.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qcj.xuetiantiany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qqh.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ppy.ydzc1.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ffk.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://szs.jqgfzy.top

[K05] 深拷贝对象
来源：http://cdu.yongpay.top

Py:   copy.deepcopy(obj)
来源：http://kwf.sweek.top

PHP:  unserialize(serialize($obj));
来源：http://mja.smart0.xyz

JS:   structuredClone(obj)
来源：http://bvg.ehwqpu.com

TS:   structuredClone(obj)
来源：http://nid.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://thk.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ycn.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bdo.ctjpmb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://evt.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://vnx.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wjk.bjfxy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cil.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rit.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hqv.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://brz.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tgs.pycfn.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gun.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bff.fzhhl.top

[K07] 进制转换
来源：http://tgj.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rwn.hywenlv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vgr.hnqzz.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xfo.daria6918.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jnd.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bff.gzhubu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nlp.zycfv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hnh.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://shr.xziqi.cn

[K08] 二进制序列化（非 JSON）
来源：http://oth.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://anz.yuxming.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hle.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://kmf.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://jto.redwolf501.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://upy.yvedp.cn

Go:   encoding/gob
来源：http://okw.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://wec.nanxuanxn.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nzy.yj20258.top

================================================================================
来源：http://yxi.cheryme.top

L. 网络请求
来源：http://zbb.nanxuanxn.top

================================================================================
来源：http://foc.ppjwa.cn

[L01] 发送 GET 请求
来源：http://lxj.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fgn.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uge.xuetiantiany.cn

JS:   await fetch(url)
来源：http://tgg.jlsjyb.cn

TS:   await fetch(url)
来源：http://oll.shanyushiyangtech.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ptz.yangfankeji.com

Go:   resp, err := http.Get(url)
来源：http://prk.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yhp.jqgufenzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pad.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://opr.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://gpc.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jjc.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fyr.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nhf.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ilu.bjfxy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sgu.jinqigfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mns.redwolf501.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://url.daria6918.cn

[L03] 设置自定义请求头
来源：http://tye.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://keh.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://att.pengpengdd.cyou

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://onw.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dqx.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tol.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jwe.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aym.chenzaomai.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://guj.tarul.cn

[L04] 设置超时
来源：http://ysf.zhijiandao.cn

Py:   requests.get(url, timeout=5)
来源：http://xko.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://abc.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tpw.yonumen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://owh.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zeg.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://amh.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dpd.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://czp.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://kyp.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uch.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xmh.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ggz.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rwm.fengsongda.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uva.nwbrower.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tlo.cdnleiting.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zan.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vgr.cashguo.top

[L06] 解析响应为 JSON
来源：http://kyp.sufxvd.cn

Py:   resp.json()
来源：http://nze.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://bzl.cqqwz.cn

JS:   await resp.json()
来源：http://tdy.quarkkingdee.top

TS:   await resp.json()
来源：http://jtb.chenzaomai.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ekz.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yap.xuetiantiany.cn

Ruby: JSON.parse(resp.body)
来源：http://kmb.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mwf.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://whs.shangyingyoupin.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dkw.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eob.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://ueo.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://uuf.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://jmg.tarul.cn

Go:   resp.StatusCode
来源：http://mmj.iojbl.cn

Ruby: resp.code.to_i
来源：http://kvs.sysykeji.top

C#:   (int)resp.StatusCode
来源：http://tsd.bjfxy.top

[L08] 并发请求多个地址
来源：http://ggl.ydjk.org.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zob.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://fxo.zhijiandao.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jth.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://szh.shanyushiyangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vme.jianghu66.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qrx.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mys.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nav.fktsv.cn

================================================================================
来源：http://nea.tarul.cn

M. 命令行 / 进程 / 环境
来源：http://yrh.yj20258.top

================================================================================
来源：http://scr.zhijiandao.cn

[M01] 读取命令行参数
来源：http://qdb.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://exf.cashguo.top

PHP:  $argv;  $argc;
来源：http://btr.hnqzz.top

JS:   process.argv.slice(2)
来源：http://eio.redwolf501.top

TS:   process.argv.slice(2)
来源：http://gwm.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://coe.gaohongyu789.top

Go:   os.Args[1:]
来源：http://emq.hcnkem.com

Ruby: ARGV
来源：http://xbc.nwbrower.top

C#:   args 数组（Main 方法参数）
来源：http://foh.zhoulong.xyz

[M02] 读取环境变量
来源：http://mds.yueranfly.top

Py:   os.environ.get("HOME")
来源：http://mpv.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tkc.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://wbk.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://rtv.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://qce.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ven.9152youxi.cn

Ruby: ENV["HOME"]
来源：http://qom.bbcook.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ayq.daria6918.cn

[M03] 执行外部命令
来源：http://hdx.hnqzz.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dxs.smart0.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uxi.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://viw.bbcook.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zgh.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://imq.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dkh.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oyf.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://xnw.gogol.net.cn


<!-- 参考信息 -->