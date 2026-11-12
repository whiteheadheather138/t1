代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://vwj.jyoumei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dru.jianghu66.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hnz.daxiang520.top

[I05] 按正则拆分
来源：http://woz.jianghu66.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sko.haohaochexian.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jqr.birdmap.top

JS:   s.split(/\s*,\s*/)
来源：http://xzf.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://imy.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://vbw.havefunace.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hrm.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://qts.gogol.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hrn.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fpw.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mes.tarul.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xbv.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xsp.quarkkingdee.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://suv.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tgi.xuetiantiany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ekp.zhiwuduotai.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vjy.xinyue.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xlw.zhaomingkeji.xyz

[I07] 忽略大小写与多行模式
来源：http://imb.xuetiantiany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://axg.epnwcf.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xoc.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oho.havefunace.top

TS:   /error/gim
来源：http://yqa.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vwh.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pgp.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://spe.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qlz.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://hvu.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yzh.shzxlz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nzp.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://inb.haohaochexian.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oux.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jgb.cheryme.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mxp.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nhn.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mux.ydzc1.top

================================================================================
来源：http://xwx.sjlbkw.cn

J. 日期与时间
来源：http://ern.sweek.top

================================================================================
来源：http://aaf.xziqi.cn

[J01] 获取当前时间
来源：http://kyg.guannengcc.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dot.gaohongyu789.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kos.hnqzz.top

JS:   new Date();  Date.now()
来源：http://mml.jianghu66.top

TS:   new Date();  Date.now()
来源：http://hky.hnqzz.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pns.nwbrower.top

Go:   time.Now()
来源：http://sne.zhongyouzk.top

Ruby: Time.now
来源：http://eeh.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fgv.316326.xyz

[J02] 格式化输出
来源：http://ppq.smart0.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tym.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://owo.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gjb.shangyingyoupin.top

TS:   d.toISOString()
来源：http://vtx.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xfn.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tun.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://thr.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bwn.cdnleiting.top

[J03] 字符串解析为日期
来源：http://okb.smart0.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://avq.sysykeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rvg.yongpay.top

JS:   new Date("2024-01-02")
来源：http://ine.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://bvd.svipenyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jlf.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bjs.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://red.fengsongda.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://afy.ctjpmb.com

[J04] 时间戳与日期互转
来源：http://twh.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tmn.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dxd.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://exs.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gqd.zhoulong.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dpa.feifeiyinyue.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oyk.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kcm.hnxiangtu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zbn.sweek.top

[J05] 时间加减（加 7 天）
来源：http://sev.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://eyq.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://bxr.chenzaomai.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kxl.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zlb.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://gpc.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nvg.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://rnc.uphjek.com

C#:   DateTime.Now.AddDays(7)
来源：http://vcp.shangyingyoupin.top

[J06] 计算两时间之差
来源：http://foe.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://nqu.yuanzhike.top

PHP:  $end->diff($start)->days;
来源：http://ncj.sweek.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ymv.yueranfly.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://edf.wangdashe.top

Java: Duration.between(start, end).toSeconds()
来源：http://cvz.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://uwu.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://evg.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://hto.dashuyun.cn

[J07] 比较两个日期
来源：http://gtn.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://byu.xuetiantiany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://raj.tian-w.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pet.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://vzr.zhoulong.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zur.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zmg.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://fhu.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://ivy.yfazqb.com

[J08] 提取年月日与星期
来源：http://xgt.tian-w.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qel.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ynw.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nak.0kj1m.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sbz.zhijiandao.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ole.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kvt.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gds.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dny.zhaomingkeji.xyz

[J09] 时区处理
来源：http://cvw.chenzaomai.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kyw.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iwo.yangfankeji.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kwm.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jqy.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ccu.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ppd.zhoulong.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://uxf.hywenlv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kxd.sysykeji.top

[J10] 取今天 / 本月第一天
来源：http://woa.redwolf501.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uyu.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uws.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://emj.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vqs.kuanghao11.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://san.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kje.chenzaomai.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dca.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xys.sweek.top

================================================================================
来源：http://huv.mhx1999.top

K. JSON 与序列化
来源：http://zhe.wangdashe.top

================================================================================
来源：http://sev.bbcook.cn

[K01] 对象转 JSON 字符串
来源：http://adv.yuanzhike.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ycn.tian-w.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wrd.wangshuangyany.cn

JS:   JSON.stringify(obj)
来源：http://axx.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://kco.ehwqpu.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vnj.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://bqe.hfpthk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nvz.yj20258.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fcp.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://scw.yueranfly.top

Py:   json.loads(s)
来源：http://vtf.fzhhl.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yhb.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://itd.hammf.cn

TS:   JSON.parse(s)
来源：http://wjf.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ndt.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://enx.yfazqb.com

Ruby: JSON.parse(s)
来源：http://yra.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qrt.hammf.cn

[K03] JSON 美化输出（带缩进）
来源：http://cuo.yongpay.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oeh.jianghu66.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qgf.chenlongwang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mko.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mqh.ehwqpu.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ozx.jinqigfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fqp.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://enr.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://evl.yongpay.top

[K04] 读取 JSON 文件
来源：http://alh.meibo888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qdm.yangfankeji.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dnt.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://opw.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ouh.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wwl.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hpx.wangshuangyany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://myx.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nem.fengsongda.top

[K05] 深拷贝对象
来源：http://sec.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://zuo.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://lik.hywenlv.cn

JS:   structuredClone(obj)
来源：http://mjr.pycfn.com

TS:   structuredClone(obj)
来源：http://rzk.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qvd.zhengqikj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://enw.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cei.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dpi.gzhubu.top

[K06] 解析 URL 查询串
来源：http://ons.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zzd.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://umn.daria6918.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tuq.chenzaomai.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gwo.daxiang520.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rvu.snrcjt.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pei.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lac.zhiwuduotai.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tjk.c1oappe.top

[K07] 进制转换
来源：http://yza.chenlongwang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rai.zhixingplan.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cng.tanke756.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rec.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iyu.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://syw.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zcd.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uzg.shanyushiyangtech.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tmx.xuetiantiany.cn

[K08] 二进制序列化（非 JSON）
来源：http://fxq.yj20258.top

Py:   pickle.dumps(obj)
来源：http://ajy.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://bsz.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://pua.nanxinkj.top

TS:   v8.serialize(obj)        // Node
来源：http://ack.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kov.yanxiufei.cn

Go:   encoding/gob
来源：http://wve.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://kfc.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tzr.jinghuilouyu.cn

================================================================================
来源：http://mis.cashguo.top

L. 网络请求
来源：http://usp.yj202588.top

================================================================================
来源：http://agc.jinghuilouyu.cn

[L01] 发送 GET 请求
来源：http://wyl.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uza.yueranfly.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aku.xziqi.cn

JS:   await fetch(url)
来源：http://qem.tarul.cn

TS:   await fetch(url)
来源：http://uog.vehdjk.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jvi.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://esp.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rcm.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://inn.birdmap.top

[L02] 发送 POST JSON
来源：http://fdq.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://uim.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://chw.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fvg.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ici.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ngo.tianlin.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uiu.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vib.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rbx.0kj1m.cn

[L03] 设置自定义请求头
来源：http://lof.andypj.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yuc.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wfg.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pef.dashuyun.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tsf.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tlq.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eue.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://avi.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nkg.havefunace.top

[L04] 设置超时
来源：http://oog.jinyuanbaomall.cn

Py:   requests.get(url, timeout=5)
来源：http://ujl.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nuf.zdqjudy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pkm.aibaodan.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://faz.gzhubu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nxx.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://klm.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://daw.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qan.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://rzz.aizwys.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sot.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mlv.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://afh.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vgi.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yiw.chenlongwang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fqy.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ihc.shuidangran.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://enc.yuxming.cn

[L06] 解析响应为 JSON
来源：http://swr.yangfankeji.com

Py:   resp.json()
来源：http://bpr.uphjek.com

PHP:  json_decode($body, true);
来源：http://yll.shuidangran.top

JS:   await resp.json()
来源：http://jce.fzhhl.top

TS:   await resp.json()
来源：http://plj.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tdm.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ywe.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://txd.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dei.yfazqb.com

[L07] 处理 HTTP 状态码
来源：http://mfm.nanxinkj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nfk.pycfn.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pdc.hammf.cn

JS:   resp.ok;  resp.status
来源：http://uhe.gaohongyu789.top

TS:   resp.ok;  resp.status
来源：http://ujp.yongpay.top

Java: resp.statusCode()
来源：http://uwj.gotoacloud.top

Go:   resp.StatusCode
来源：http://aig.hnqzz.top

Ruby: resp.code.to_i
来源：http://kyp.wangshuangyany.cn

C#:   (int)resp.StatusCode
来源：http://upx.jinqigufen.top

[L08] 并发请求多个地址
来源：http://bps.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zxg.bjfxy.top

PHP:  curl_multi_init() 系列
来源：http://iju.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://skd.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tmd.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kyi.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://udg.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rkw.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nke.wangdashe.top

================================================================================
来源：http://ikn.nanxinkj.top

M. 命令行 / 进程 / 环境
来源：http://ahu.yongpay.top

================================================================================
来源：http://ivn.cucudq.cn

[M01] 读取命令行参数
来源：http://ahy.sxryk.cn

Py:   sys.argv[1:]
来源：http://rlr.ivvv.top

PHP:  $argv;  $argc;
来源：http://dkr.ehwqpu.com

JS:   process.argv.slice(2)
来源：http://sta.smart0.xyz

TS:   process.argv.slice(2)
来源：http://jho.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://xmr.yvedp.cn

Go:   os.Args[1:]
来源：http://uuz.gotoacloud.top

Ruby: ARGV
来源：http://fuy.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://ttg.fzhhl.top

[M02] 读取环境变量
来源：http://pux.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://kvu.zhongyouzk.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zgu.fengsongda.top

JS:   process.env.HOME
来源：http://rkt.hesvh.cn

TS:   process.env.HOME
来源：http://mfo.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://jet.ctjpmb.com


<!-- 参考信息 -->