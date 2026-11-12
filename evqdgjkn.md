代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://egn.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wzt.tian-w.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yni.chenjidiqi.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://daa.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rrt.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://ohn.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eve.daria6918.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mar.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gee.haohaochexian.top

TS:   /error/gim
来源：http://zbu.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zoi.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eyz.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://frh.zhiwuduotai.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pdf.jinqigufen.top

[I08] 贪婪与非贪婪匹配
来源：http://osu.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://daz.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mbh.fehbvm.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://een.cqqwz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rpp.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://llr.yanxiufei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ztb.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bsq.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zkq.vehdjk.com

================================================================================
来源：http://uqi.yuanzhike.top

J. 日期与时间
来源：http://evj.cucudq.cn

================================================================================
来源：http://fpt.yongpay.top

[J01] 获取当前时间
来源：http://mok.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vle.ywan-chungtsiang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wuh.yuxming.cn

JS:   new Date();  Date.now()
来源：http://vsg.shuidangran.top

TS:   new Date();  Date.now()
来源：http://rmb.ivvv.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vji.nwbrower.top

Go:   time.Now()
来源：http://kts.jinghuilouyu.cn

Ruby: Time.now
来源：http://qok.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hvd.yj20258888.top

[J02] 格式化输出
来源：http://ksv.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fap.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pej.hongshengwenyu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://owl.c1oappe.top

TS:   d.toISOString()
来源：http://csc.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wdr.chenjidiqi.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iuk.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zby.xuanzx.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zys.cdnleiting.top

[J03] 字符串解析为日期
来源：http://bxj.jqgfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://frp.zycfv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nms.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://pyp.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://mpu.fengsongda.top

Java: LocalDate.parse("2024-01-02")
来源：http://sbc.uphjek.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xvo.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://dtn.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fam.yueranfly.top

[J04] 时间戳与日期互转
来源：http://cyi.cucudq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qxn.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wyi.xingfuxueyuan.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bhz.iojbl.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vlx.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dem.hnqzz.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eyq.tianlin.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ara.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ghv.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://wah.0kj1m.cn

Py:   now + timedelta(days=7)
来源：http://wua.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kst.hcnkem.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zlk.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fpl.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://cfa.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gzb.xuetiantiany.cn

Ruby: Time.now + 7 * 86400
来源：http://dgf.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://mxw.jinqigfzy.top

[J06] 计算两时间之差
来源：http://brs.yj202588.top

Py:   (end - start).total_seconds()
来源：http://meu.zycfv.cn

PHP:  $end->diff($start)->days;
来源：http://atb.vehdjk.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vgw.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rrs.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dpm.52xcode.cn

Go:   end.Sub(start).Hours()
来源：http://axa.52xcode.cn

Ruby: end - start                 # 返回秒数
来源：http://ehx.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://vuu.shanyushiyangtech.top

[J07] 比较两个日期
来源：http://jlv.jyoumei.cn

Py:   d1 < d2;  d1 == d2
来源：http://dhw.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nhf.hywenlv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oao.hnxiangtu.top

TS:   d1.getTime() < d2.getTime()
来源：http://nbh.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hdy.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yof.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://llc.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://lpu.daria6918.cn

[J08] 提取年月日与星期
来源：http://nog.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zja.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pfh.sjlbkw.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zri.svipenyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lqn.aibaodan.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zfm.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bgw.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gir.nanxuanxn.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jxi.hfpthk.cn

[J09] 时区处理
来源：http://fgw.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kei.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yqs.shanyushiyangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://igz.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yvz.hywenlv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pfy.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eqh.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fot.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hsa.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://bhy.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jky.tian-w.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ffc.nanxuanxn.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://byv.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rxy.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pvd.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ipl.bjfxy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hlk.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gzt.havefunace.top

================================================================================
来源：http://avu.yfazqb.com

K. JSON 与序列化
来源：http://rtp.shuidangran.top

================================================================================
来源：http://rgd.zdqjudy.top

[K01] 对象转 JSON 字符串
来源：http://mqo.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kko.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kud.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://ghb.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://irz.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iua.cheryme.top

Go:   json.Marshal(obj)
来源：http://xrm.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://qqu.gzhubu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yxf.andypj.xyz

[K02] JSON 字符串转对象
来源：http://glq.fengsongda.top

Py:   json.loads(s)
来源：http://ioc.hammf.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pmo.fanxiaobao.xyz

JS:   JSON.parse(s)
来源：http://cen.gogol.net.cn

TS:   JSON.parse(s)
来源：http://vnp.fzhhl.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://riw.iojbl.cn

Go:   json.Unmarshal(data, &v)
来源：http://xfm.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://wma.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://plp.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://nzw.yj202588.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ekd.gzhubu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wez.9152youxi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ato.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://rfp.ydzc1.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://evg.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://chx.haohaochexian.top

Ruby: JSON.pretty_generate(obj)
来源：http://lqq.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://whu.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://nmd.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fxx.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://acp.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sey.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mzh.smart0.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gyl.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ebl.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://waw.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fnw.shangyingyoupin.top

[K05] 深拷贝对象
来源：http://qgs.yonumen.top

Py:   copy.deepcopy(obj)
来源：http://aia.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://dvu.dianchejie.cn

JS:   structuredClone(obj)
来源：http://nkc.fanxiaobao.xyz

TS:   structuredClone(obj)
来源：http://zhx.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kep.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vnp.xuanzx.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yrd.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mgf.zhoulong.xyz

[K06] 解析 URL 查询串
来源：http://wja.birdmap.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eys.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zsv.tarul.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://glp.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nuj.yuanzhike.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wgs.zhaomingkeji.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://qor.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ldr.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bds.gotoacloud.top

[K07] 进制转换
来源：http://mbs.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pmm.andypj.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tuw.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://akh.nanxuanxn.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ewg.andypj.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hmm.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xxm.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rnj.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dzq.ydzc1.top

[K08] 二进制序列化（非 JSON）
来源：http://mid.chenjidiqi.icu

Py:   pickle.dumps(obj)
来源：http://woi.sufxvd.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rux.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://pvy.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://wgk.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uiu.jinqigfzy.top

Go:   encoding/gob
来源：http://nge.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://meh.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hku.vqdsnc.cn

================================================================================
来源：http://yve.svipenyu.cn

L. 网络请求
来源：http://vka.nanxinkj.top

================================================================================
来源：http://xcj.daxiang520.top

[L01] 发送 GET 请求
来源：http://vib.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ydm.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gdr.nwbrower.top

JS:   await fetch(url)
来源：http://fyk.kuanghao11.cn

TS:   await fetch(url)
来源：http://eqp.ctjpmb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mxs.zhixingplan.top

Go:   resp, err := http.Get(url)
来源：http://otd.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mrz.mhx1999.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aij.shzxlz.cn

[L02] 发送 POST JSON
来源：http://wtw.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pfl.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zbr.zdqjudy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://shf.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qrx.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://drk.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hta.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qud.yongpay.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bfu.zhijiandao.cn

[L03] 设置自定义请求头
来源：http://qiu.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://upz.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jho.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ede.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jif.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://olc.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gpm.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jsk.zhaomingkeji.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hpt.sjlbkw.cn

[L04] 设置超时
来源：http://kxn.zhaomingkeji.xyz

Py:   requests.get(url, timeout=5)
来源：http://gwc.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jus.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jox.ctjpmb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ucb.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zhc.c1oappe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vrx.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ppt.shanyushiyangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://elz.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://hhq.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vul.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xkh.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ozg.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xsr.fzhhl.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pts.chenlongwang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wef.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fhs.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mvc.zycfv.cn

[L06] 解析响应为 JSON
来源：http://blh.haohaochexian.top

Py:   resp.json()
来源：http://vzq.ppjwa.cn

PHP:  json_decode($body, true);
来源：http://hus.zhijiandao.cn

JS:   await resp.json()
来源：http://ugb.uphjek.com

TS:   await resp.json()
来源：http://qzv.0kj1m.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zri.smart0.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nec.ppjwa.cn

Ruby: JSON.parse(resp.body)
来源：http://hpw.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://voy.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://gid.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://omb.daria6918.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tvw.hammf.cn

JS:   resp.ok;  resp.status
来源：http://ofp.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://nyy.gzhubu.top

Java: resp.statusCode()
来源：http://avx.xinyue.icu

Go:   resp.StatusCode
来源：http://wve.tianlin.xyz

Ruby: resp.code.to_i
来源：http://bwv.vqdsnc.cn

C#:   (int)resp.StatusCode
来源：http://jxx.fanxiaobao.xyz

[L08] 并发请求多个地址
来源：http://gsx.cheryme.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vfe.nanxuanxn.top

PHP:  curl_multi_init() 系列
来源：http://xqd.zhijiandao.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tya.yj20258888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pzx.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iwc.ywan-chungtsiang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lql.fzhhl.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://leg.epnwcf.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wvv.xziqi.cn

================================================================================
来源：http://gjd.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://xmo.sufxvd.cn

================================================================================
来源：http://qsb.aibaodan.cn

[M01] 读取命令行参数
来源：http://gkp.bbcook.cn

Py:   sys.argv[1:]
来源：http://vil.jianghu66.top

PHP:  $argv;  $argc;
来源：http://vbs.daxiang520.top

JS:   process.argv.slice(2)
来源：http://eyh.tarul.cn

TS:   process.argv.slice(2)
来源：http://njl.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://vdn.epnwcf.com

Go:   os.Args[1:]
来源：http://vsr.pycfn.com

Ruby: ARGV
来源：http://vwj.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://apq.hammf.cn

[M02] 读取环境变量
来源：http://qmx.cucudq.cn

Py:   os.environ.get("HOME")
来源：http://qoi.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oth.jinqigfzy.top

JS:   process.env.HOME
来源：http://lfk.9152youxi.cn

TS:   process.env.HOME
来源：http://ewv.ywan-chungtsiang.top

Java: System.getenv("HOME")
来源：http://vlm.ywan-chungtsiang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eju.ybcxt.top

Ruby: ENV["HOME"]
来源：http://xix.yj20258888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sko.gogol.net.cn

[M03] 执行外部命令
来源：http://bog.chenjidiqi.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lei.jinqigfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://agi.hongshengwenyu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xcv.zhixingplan.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wmm.zhongyouzk.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://paw.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yks.yueranfly.top

Ruby: system("ls -l");  `ls -l`
来源：http://tyz.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://gxp.ppjwa.cn

[M04] 获取当前工作目录
来源：http://xvv.yfazqb.com

Py:   os.getcwd()
来源：http://wsn.cheryme.top

PHP:  getcwd();
来源：http://lun.ywan-chungtsiang.top

JS:   process.cwd()
来源：http://mdc.uphjek.com


<!-- 参考信息 -->