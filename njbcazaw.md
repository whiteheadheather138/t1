代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://jzv.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://spa.fengsongda.top

JS:   s.split(/\s*,\s*/)
来源：http://ger.sjlbkw.cn

TS:   s.split(/\s*,\s*/)
来源：http://gdr.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://fft.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qfu.yj20258.top

Ruby: s.split(/\s*,\s*/)
来源：http://otc.fktsv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qin.gzhubu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zwa.daria6918.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bba.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://drw.zhixingplan.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cxv.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oaa.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wcd.sjlbkw.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mhu.hammf.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kqj.andypj.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lvi.chenlongwang.top

[I07] 忽略大小写与多行模式
来源：http://lvh.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uco.zhoulong.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yrn.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oyj.wangshuangyany.cn

TS:   /error/gim
来源：http://itu.epnwcf.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://znd.gzhubu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://phn.yangfankeji.com

Ruby: s.scan(/error/i)
来源：http://jpd.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sxm.guannengcc.top

[I08] 贪婪与非贪婪匹配
来源：http://lws.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rhf.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://itm.vqdsnc.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hxp.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vtx.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://qey.zhixingplan.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sap.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oma.svipenyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kua.epnwcf.com

================================================================================
来源：http://brl.zhaomingkeji.xyz

J. 日期与时间
来源：http://fpr.aizwys.cn

================================================================================
来源：http://med.jianghu66.top

[J01] 获取当前时间
来源：http://eid.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://uqq.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oej.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://sel.smart0.xyz

TS:   new Date();  Date.now()
来源：http://puf.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jjm.fzhhl.top

Go:   time.Now()
来源：http://wnf.cashguo.top

Ruby: Time.now
来源：http://kvy.cashguo.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xac.ydzc1.top

[J02] 格式化输出
来源：http://qoe.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ocl.yuxming.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mpi.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iuu.hywenlv.cn

TS:   d.toISOString()
来源：http://jwu.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://olp.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xhr.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://okp.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ywo.fktsv.cn

[J03] 字符串解析为日期
来源：http://ujw.shuidangran.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nnr.shanyushiyangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ktg.0kj1m.cn

JS:   new Date("2024-01-02")
来源：http://zwr.bjfxy.top

TS:   new Date("2024-01-02")
来源：http://fxn.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://znv.yvedp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lwg.ppjwa.cn

Ruby: Date.parse("2024-01-02")
来源：http://bhv.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rfy.zhoulong.xyz

[J04] 时间戳与日期互转
来源：http://xfl.fehbvm.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gce.yongpay.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xct.nanxuanxn.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ers.ehwqpu.com

TS:   Math.floor(Date.now() / 1000)
来源：http://xgs.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qpo.haohaochexian.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vku.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ydg.9152youxi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pvw.c1oappe.top

[J05] 时间加减（加 7 天）
来源：http://tza.uphjek.com

Py:   now + timedelta(days=7)
来源：http://swe.kuanghao11.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uax.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ttw.9152youxi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://emo.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://mvq.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nyo.fzhhl.top

Ruby: Time.now + 7 * 86400
来源：http://jpn.tianlin.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://hvz.chenlongwang.top

[J06] 计算两时间之差
来源：http://szi.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://lai.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://aok.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ajv.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://beu.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://fhy.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://cbt.c1oappe.top

Ruby: end - start                 # 返回秒数
来源：http://nst.jqgufenzy.top

C#:   (end - start).TotalSeconds
来源：http://ner.chenlongwang.top

[J07] 比较两个日期
来源：http://jzu.nanxuanxn.top

Py:   d1 < d2;  d1 == d2
来源：http://htu.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vdv.haohaochexian.top

JS:   d1.getTime() < d2.getTime()
来源：http://yml.birdmap.top

TS:   d1.getTime() < d2.getTime()
来源：http://wbi.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://akz.vehdjk.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tvp.sjlbkw.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tmm.birdmap.top

C#:   d1 < d2;  d1 == d2
来源：http://qnq.jlsjyb.cn

[J08] 提取年月日与星期
来源：http://rxm.hesvh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uer.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wyd.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kyb.birdmap.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xdm.uphjek.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://trk.52xcode.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zpj.zhaomingkeji.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lra.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yop.c1oappe.top

[J09] 时区处理
来源：http://tgj.jianghu66.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zan.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://stj.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ekt.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://prh.birdmap.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://atz.fanxiaobao.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://niu.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bid.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zwv.aibaodan.cn

[J10] 取今天 / 本月第一天
来源：http://way.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gcg.cqqwz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ihs.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zhd.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pnx.gaohongyu789.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wqp.ydzc1.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uwr.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zqy.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ccb.shuidangran.top

================================================================================
来源：http://bnk.nanxinkj.top

K. JSON 与序列化
来源：http://scz.cdnleiting.top

================================================================================
来源：http://jkq.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://alc.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://evd.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uxh.yfazqb.com

JS:   JSON.stringify(obj)
来源：http://ftg.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://lxs.bbcook.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dpj.yj202588.top

Go:   json.Marshal(obj)
来源：http://knn.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://lys.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bfs.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://efs.shuidangran.top

Py:   json.loads(s)
来源：http://upd.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ehu.jiagoushi.top

JS:   JSON.parse(s)
来源：http://lhp.hywenlv.cn

TS:   JSON.parse(s)
来源：http://snw.cheryme.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xjh.jinqigfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://yxp.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://oxk.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pik.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://sxd.iojbl.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jyy.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yuj.yonumen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pzv.bbcook.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lbo.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xjo.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mvd.dashuyun.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mzq.hywenlv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tcr.ehwqpu.com

[K04] 读取 JSON 文件
来源：http://jjg.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ezn.shanyushiyangtech.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fcx.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vql.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ttz.shanyushiyangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mjy.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xtx.cqqwz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yww.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nhg.wangdashe.top

[K05] 深拷贝对象
来源：http://wur.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://bcu.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://cok.tianlin.xyz

JS:   structuredClone(obj)
来源：http://yfr.yuxming.cn

TS:   structuredClone(obj)
来源：http://wud.jinqigufen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wiw.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nwy.iojbl.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ljv.sufxvd.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://onj.daria6918.cn

[K06] 解析 URL 查询串
来源：http://euz.shzxlz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yci.xingfuxueyuan.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dmh.ehwqpu.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hsb.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wpd.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://frw.daxiang520.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qfr.cdnleiting.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ebm.zhaomingkeji.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kjy.ywan-chungtsiang.top

[K07] 进制转换
来源：http://voh.jyoumei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jgy.yuxming.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bcu.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fxs.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rjy.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ejb.dianchejie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ohu.tarul.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://evx.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mgg.zdqjudy.top

[K08] 二进制序列化（非 JSON）
来源：http://esb.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://mpv.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mmj.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://eqv.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://vpg.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://syw.smart0.xyz

Go:   encoding/gob
来源：http://nlh.cucudq.cn

Ruby: Marshal.dump(obj)
来源：http://miz.sxryk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gcd.hammf.cn

================================================================================
来源：http://bgs.zycfv.cn

L. 网络请求
来源：http://qcp.havefunace.top

================================================================================
来源：http://vlm.zhaomingkeji.xyz

[L01] 发送 GET 请求
来源：http://aly.redwolf501.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tih.sjlbkw.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nek.gogol.net.cn

JS:   await fetch(url)
来源：http://ogi.daria6918.cn

TS:   await fetch(url)
来源：http://clu.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tux.shanyushiyangtech.top

Go:   resp, err := http.Get(url)
来源：http://rsv.uphjek.com

Ruby: Net::HTTP.get(URI(url))
来源：http://lzm.zhaomingkeji.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vjk.ybcxt.top

[L02] 发送 POST JSON
来源：http://ujy.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://giw.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pfk.shangyingyoupin.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rhq.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uzi.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vxm.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dcj.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://spp.smart0.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://odk.hnqzz.top

[L03] 设置自定义请求头
来源：http://rbu.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://czk.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://avv.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rfc.shuidangran.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jws.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pth.jinqigufen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kqs.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vhq.bbcook.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hkb.andypj.xyz

[L04] 设置超时
来源：http://upx.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://kml.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yby.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vuy.sufxvd.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ifw.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mmf.zhoulong.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rxx.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://syz.wangshuangyany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eyo.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://dbf.shzxlz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iju.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iil.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gqt.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dcr.snrcjt.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nin.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yxp.zhaomingkeji.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://waa.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pgv.hcnkem.com

[L06] 解析响应为 JSON
来源：http://fqd.haohaochexian.top

Py:   resp.json()
来源：http://ewo.havefunace.top

PHP:  json_decode($body, true);
来源：http://apm.quarkkingdee.top

JS:   await resp.json()
来源：http://rrm.shuidangran.top

TS:   await resp.json()
来源：http://zmp.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://boq.jianghu66.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lrl.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://xsf.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vwq.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://tdr.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lwb.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cgn.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://klq.meibo888.top

TS:   resp.ok;  resp.status
来源：http://hsm.tarul.cn

Java: resp.statusCode()
来源：http://acv.iojbl.cn

Go:   resp.StatusCode
来源：http://rjp.sxryk.cn

Ruby: resp.code.to_i
来源：http://ltt.yonumen.top

C#:   (int)resp.StatusCode
来源：http://gdn.ybcxt.top

[L08] 并发请求多个地址
来源：http://qqm.hfpthk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cbu.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://lkt.hfpthk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sgk.hammf.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sel.guannengcc.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oha.52xcode.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qoq.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eym.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lcv.cucudq.cn

================================================================================
来源：http://nqh.chenjidiqi.icu

M. 命令行 / 进程 / 环境
来源：http://ppm.daxiang520.top

================================================================================
来源：http://pfj.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://mwh.yueranfly.top

Py:   sys.argv[1:]
来源：http://kxg.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://jah.gzhubu.top

JS:   process.argv.slice(2)
来源：http://jnz.zhengqikj.top

TS:   process.argv.slice(2)
来源：http://itq.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://oqq.yuxming.cn

Go:   os.Args[1:]
来源：http://cuh.yongpay.top

Ruby: ARGV
来源：http://mby.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://uhr.aibaodan.cn

[M02] 读取环境变量
来源：http://wrd.jianghu66.top

Py:   os.environ.get("HOME")
来源：http://ffo.hammf.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wbw.daxiang520.top

JS:   process.env.HOME
来源：http://jcd.hnqzz.top

TS:   process.env.HOME
来源：http://cwy.jyoumei.cn

Java: System.getenv("HOME")
来源：http://itg.andypj.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://axj.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://toq.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://enm.andypj.xyz

[M03] 执行外部命令
来源：http://tpp.hesvh.cn


<!-- 参考信息 -->