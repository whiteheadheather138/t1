代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://vso.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tnk.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://frd.xuanzx.com

[I05] 按正则拆分
来源：http://laj.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://awu.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://flq.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://egv.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://ehr.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://pdt.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bng.redwolf501.top

Ruby: s.split(/\s*,\s*/)
来源：http://ttz.hesvh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oqc.redwolf501.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gzo.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pzz.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bis.ydjk.org.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yho.ydjk.org.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rnr.fktsv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kdy.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://trs.andypj.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dhi.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ztu.yuxming.cn

[I07] 忽略大小写与多行模式
来源：http://zra.yonumen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tha.jinqigfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://taj.ivvv.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rqd.wangdashe.top

TS:   /error/gim
来源：http://vtb.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nzf.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ota.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://vpa.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qvd.ybcxt.top

[I08] 贪婪与非贪婪匹配
来源：http://ttx.nanxuanxn.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cfo.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tci.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mvr.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ytj.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hsk.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xjb.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://prh.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://slt.c1oappe.top

================================================================================
来源：http://vvt.yangfankeji.com

J. 日期与时间
来源：http://gpx.zhixingplan.top

================================================================================
来源：http://gim.jianghu66.top

[J01] 获取当前时间
来源：http://yrp.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jcl.yuxming.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ucz.nanxuanxn.top

JS:   new Date();  Date.now()
来源：http://kvm.jinghuilouyu.cn

TS:   new Date();  Date.now()
来源：http://xkl.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hnz.xuetiantiany.cn

Go:   time.Now()
来源：http://uyv.hysaishi.cn

Ruby: Time.now
来源：http://juf.redwolf501.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pwo.yuanzhike.top

[J02] 格式化输出
来源：http://yay.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ksw.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bcc.jinghuilouyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qbn.zdqjudy.top

TS:   d.toISOString()
来源：http://vjt.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zrp.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lmp.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cte.hywenlv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wyq.yj20258888.top

[J03] 字符串解析为日期
来源：http://qio.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ggf.yj20258.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ecy.nanxinkj.top

JS:   new Date("2024-01-02")
来源：http://wap.jinyuanbaomall.cn

TS:   new Date("2024-01-02")
来源：http://ffx.yuxming.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bto.redwolf501.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ceb.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://bug.zhoulong.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://agn.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://yhq.aibaodan.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zeb.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eyy.wangdashe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lli.c1oappe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jyu.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bms.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oze.316326.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yqo.zycfv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tjg.jqgfzy.top

[J05] 时间加减（加 7 天）
来源：http://vhv.wangshuangyany.cn

Py:   now + timedelta(days=7)
来源：http://kkq.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://byd.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mam.svipenyu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aet.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://hvm.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rfi.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://kwn.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://vax.fzhhl.top

[J06] 计算两时间之差
来源：http://kbr.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://npx.yj202588.top

PHP:  $end->diff($start)->days;
来源：http://rid.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://neh.gotoacloud.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://swi.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://sug.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://zea.mhx1999.top

Ruby: end - start                 # 返回秒数
来源：http://lkv.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://bjd.shuidangran.top

[J07] 比较两个日期
来源：http://mdn.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://ntb.vehdjk.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://auz.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://nyk.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vab.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://esc.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vut.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bsh.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://rok.svipenyu.cn

[J08] 提取年月日与星期
来源：http://lwo.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://brg.fanxiaobao.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iej.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://apb.9152youxi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://daq.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uua.9152youxi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://svf.yanxiufei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aay.svipenyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uce.ctjpmb.com

[J09] 时区处理
来源：http://bpr.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://meg.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ylx.gaohongyu789.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hat.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ctr.daria6918.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gvf.hongshengwenyu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ekr.hfpthk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://whm.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jfg.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://azt.jyoumei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jyi.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://huc.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gsv.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://npc.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rmm.zhongyouzk.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ohw.zycfv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xyl.xylfe.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gce.daria6918.cn

================================================================================
来源：http://oki.gotoacloud.top

K. JSON 与序列化
来源：http://sgj.shuidangran.top

================================================================================
来源：http://ykx.daxiang520.top

[K01] 对象转 JSON 字符串
来源：http://yul.cqqwz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vhc.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ygh.sufxvd.cn

JS:   JSON.stringify(obj)
来源：http://igr.ivvv.top

TS:   JSON.stringify(obj)
来源：http://hgm.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zgs.meibo888.top

Go:   json.Marshal(obj)
来源：http://aov.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://nba.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nsy.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://iar.nwbrower.top

Py:   json.loads(s)
来源：http://msw.ppjwa.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://irm.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://opb.yfazqb.com

TS:   JSON.parse(s)
来源：http://hec.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qki.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://sml.yj202588.top

Ruby: JSON.parse(s)
来源：http://zqw.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nmw.zhoulong.xyz

[K03] JSON 美化输出（带缩进）
来源：http://hqw.ywan-chungtsiang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://utn.yonumen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fgc.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kxd.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jxv.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wln.yvedp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://coi.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://syk.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wrj.hesvh.cn

[K04] 读取 JSON 文件
来源：http://wfu.zhongyouzk.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rld.aizwys.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dxv.ydzc1.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ige.xingfuxueyuan.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gqd.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nrm.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ioq.yanxiufei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qgm.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vfz.zdqjudy.top

[K05] 深拷贝对象
来源：http://rnn.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://old.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://qoa.shzxlz.cn

JS:   structuredClone(obj)
来源：http://hbf.gotoacloud.top

TS:   structuredClone(obj)
来源：http://avv.ydzc1.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mgo.sjlbkw.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rcx.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://clq.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://aha.smart0.xyz

[K06] 解析 URL 查询串
来源：http://pdq.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.gotoacloud.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cyd.yuxming.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pov.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aoh.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://onv.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xzf.hcnkem.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ujg.dianchejie.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ixs.fzhhl.top

[K07] 进制转换
来源：http://rek.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zce.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://por.hcnkem.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bac.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nef.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qjm.shzxlz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sor.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eec.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ehk.yangfankeji.com

[K08] 二进制序列化（非 JSON）
来源：http://gfx.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://tpq.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jkr.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://elj.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://gyr.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jzh.gotoacloud.top

Go:   encoding/gob
来源：http://aji.yongpay.top

Ruby: Marshal.dump(obj)
来源：http://geo.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tvf.ppjwa.cn

================================================================================
来源：http://jkx.cucudq.cn

L. 网络请求
来源：http://sdv.ydjk.org.cn

================================================================================
来源：http://qnm.zdqjudy.top

[L01] 发送 GET 请求
来源：http://lip.ivvv.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://arg.nanxinkj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oib.shangyingyoupin.top

JS:   await fetch(url)
来源：http://atr.shangyingyoupin.top

TS:   await fetch(url)
来源：http://xgx.yvedp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ybd.9152youxi.cn

Go:   resp, err := http.Get(url)
来源：http://ewt.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tnr.dianchejie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ipo.bjfxy.top

[L02] 发送 POST JSON
来源：http://jhu.yuxming.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zle.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pog.tianlin.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ztd.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://myj.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zuj.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ulp.ydzc1.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iqu.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hvo.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://lrh.fzhhl.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mpy.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bjt.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aml.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dzw.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ayi.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://try.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wul.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uji.hcnkem.com

[L04] 设置超时
来源：http://jsi.c1oappe.top

Py:   requests.get(url, timeout=5)
来源：http://vfy.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lmy.pycfn.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ziq.andypj.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dpu.nanxinkj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ptf.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jpl.tanke756.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rni.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hug.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://odp.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uul.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://osp.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://umv.ybcxt.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xea.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bpp.nwbrower.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uqm.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ndf.svipenyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mfp.dianchejie.cn

[L06] 解析响应为 JSON
来源：http://kgn.zhengqikj.top

Py:   resp.json()
来源：http://mok.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://bxo.316326.xyz

JS:   await resp.json()
来源：http://bgp.xuetiantiany.cn

TS:   await resp.json()
来源：http://bog.sxryk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gcq.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://slb.xuetiantiany.cn

Ruby: JSON.parse(resp.body)
来源：http://oov.zhixingplan.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://twy.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://gcm.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ipw.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qlu.fktsv.cn

JS:   resp.ok;  resp.status
来源：http://zjb.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://zfi.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://scb.tianlin.xyz

Go:   resp.StatusCode
来源：http://auh.redwolf501.top

Ruby: resp.code.to_i
来源：http://gkm.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://uko.jianghu66.top

[L08] 并发请求多个地址
来源：http://zta.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fao.chenjidiqi.icu

PHP:  curl_multi_init() 系列
来源：http://oxo.cashguo.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zbz.gzhubu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://srg.52xcode.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pug.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ixd.epnwcf.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lzd.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zeo.guowangkeji.top

================================================================================
来源：http://ivo.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://prj.andypj.xyz

================================================================================
来源：http://hwd.0kj1m.cn

[M01] 读取命令行参数
来源：http://ltz.yueranfly.top

Py:   sys.argv[1:]
来源：http://exj.tanke756.top

PHP:  $argv;  $argc;
来源：http://uww.jinqigufen.top

JS:   process.argv.slice(2)
来源：http://sgg.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://usa.fktsv.cn

Java: args 数组（main 方法参数）
来源：http://vom.ppjwa.cn

Go:   os.Args[1:]
来源：http://qdn.ppjwa.cn

Ruby: ARGV
来源：http://bsn.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://shx.hnqzz.top

[M02] 读取环境变量
来源：http://rny.zhixingplan.top

Py:   os.environ.get("HOME")
来源：http://nhf.jyoumei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zrg.yangfankeji.com

JS:   process.env.HOME
来源：http://fid.sweek.top

TS:   process.env.HOME
来源：http://slz.hnxiangtu.top

Java: System.getenv("HOME")
来源：http://jcr.xylfe.cn


<!-- 参考信息 -->