代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://vad.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nah.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://fxc.mhx1999.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://men.nanxuanxn.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fjb.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xtc.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bjz.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ysc.yj20258.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qhy.chenjidiqi.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ant.shanyushiyangtech.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ybw.zhijiandao.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pfq.jqgfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vuz.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://eky.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tmj.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yhb.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jdy.ydjk.org.cn

TS:   /error/gim
来源：http://zkc.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xxf.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ivi.uphjek.com

Ruby: s.scan(/error/i)
来源：http://mac.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fow.haohaochexian.top

[I08] 贪婪与非贪婪匹配
来源：http://ixb.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ygn.pengpengdd.cyou

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ych.sxryk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://olp.pycfn.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mje.xingfuxueyuan.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://toj.tarul.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cce.pycfn.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mrk.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yhj.meibo888.top

================================================================================
来源：http://clw.snrcjt.cn

J. 日期与时间
来源：http://cpq.jlsjyb.cn

================================================================================
来源：http://hci.jyoumei.cn

[J01] 获取当前时间
来源：http://oki.zhengqikj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://stw.cqqwz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rsj.hywenlv.cn

JS:   new Date();  Date.now()
来源：http://yyl.mhx1999.top

TS:   new Date();  Date.now()
来源：http://esd.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yoq.sufxvd.cn

Go:   time.Now()
来源：http://hto.yueranfly.top

Ruby: Time.now
来源：http://puf.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tni.yueranfly.top

[J02] 格式化输出
来源：http://tqp.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ltz.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dcz.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mgx.uphjek.com

TS:   d.toISOString()
来源：http://xsf.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ydf.snrcjt.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ffn.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ctj.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tan.yonumen.top

[J03] 字符串解析为日期
来源：http://ydp.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bra.jinqigufen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qpv.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://gcm.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://fqu.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zis.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rrg.gaohongyu789.top

Ruby: Date.parse("2024-01-02")
来源：http://nwm.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cwt.sufxvd.cn

[J04] 时间戳与日期互转
来源：http://rgw.tian-w.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jxk.jyoumei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aho.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qsp.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://tkx.svipenyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wfc.uphjek.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jca.ehwqpu.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mss.fanxiaobao.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mul.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://mim.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://ylp.aizwys.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zhg.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zyl.dashuyun.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xtz.redwolf501.top

Java: LocalDate.now().plusDays(7)
来源：http://alb.9152youxi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://voy.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://zkd.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fpn.chenzaomai.com

[J06] 计算两时间之差
来源：http://phg.zdbjq.cn

Py:   (end - start).total_seconds()
来源：http://dhn.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://nrg.bbcook.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qkx.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mut.ydzc1.top

Java: Duration.between(start, end).toSeconds()
来源：http://ckp.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://elu.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://uwc.chenjidiqi.icu

C#:   (end - start).TotalSeconds
来源：http://ubg.hnqzz.top

[J07] 比较两个日期
来源：http://gtx.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://say.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dnr.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qhk.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://qob.ehwqpu.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vrr.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://skh.hnqzz.top

Ruby: d1 < d2;  d1 == d2
来源：http://zjm.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://xmu.cqqwz.cn

[J08] 提取年月日与星期
来源：http://ekl.nanxinkj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nyz.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ywg.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mev.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cak.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wom.aizwys.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ozf.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ubl.bjfxy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fer.zdbjq.cn

[J09] 时区处理
来源：http://bjl.iojbl.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sff.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hvj.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://myf.jlsjyb.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ooc.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bvv.jianghu66.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xkd.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hpz.cashguo.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mtv.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://pbg.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://grn.sjlbkw.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qpe.xuetiantiany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uit.hammf.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aua.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://udu.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nbr.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://geo.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://odx.hfpthk.cn

================================================================================
来源：http://cof.yongpay.top

K. JSON 与序列化
来源：http://zxe.tian-w.cn

================================================================================
来源：http://zjr.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://czt.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qyc.gaohongyu789.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wwu.redwolf501.top

JS:   JSON.stringify(obj)
来源：http://xpe.ywan-chungtsiang.top

TS:   JSON.stringify(obj)
来源：http://gus.ywan-chungtsiang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lgk.xziqi.cn

Go:   json.Marshal(obj)
来源：http://tif.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://qsm.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nfy.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://xxs.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://aof.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://muj.bbcook.cn

JS:   JSON.parse(s)
来源：http://bgb.nanxuanxn.top

TS:   JSON.parse(s)
来源：http://tkb.gzhubu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gzc.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://yzm.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://kwc.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xnx.gaohongyu789.top

[K03] JSON 美化输出（带缩进）
来源：http://ina.hnxiangtu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zzu.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://axz.meibo888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bxc.tarul.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dpg.haohaochexian.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qqn.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cwf.daxiang520.top

Ruby: JSON.pretty_generate(obj)
来源：http://raz.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mcn.ivvv.top

[K04] 读取 JSON 文件
来源：http://duy.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hsu.epnwcf.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zch.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kls.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sct.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://htw.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://okt.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ogm.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zmq.sysykeji.top

[K05] 深拷贝对象
来源：http://xiy.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://wks.yonumen.top

PHP:  unserialize(serialize($obj));
来源：http://lmm.shanyushiyangkeji.top

JS:   structuredClone(obj)
来源：http://lzm.xuetiantiany.cn

TS:   structuredClone(obj)
来源：http://vct.gotoacloud.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uiq.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ihm.jlsjyb.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gms.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://mxg.epnwcf.com

[K06] 解析 URL 查询串
来源：http://ffd.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lsp.feifeiyinyue.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fji.hfpthk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://liz.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://esz.cqqwz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sqp.xuanzx.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ucj.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ujp.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fxl.guannengcc.top

[K07] 进制转换
来源：http://vim.hcnkem.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fqn.xuanzx.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://frc.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://syd.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lyz.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hre.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hvh.redwolf501.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kra.zdqjudy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fmh.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://wwm.uphjek.com

Py:   pickle.dumps(obj)
来源：http://noj.zhijiandao.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hqz.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://kny.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://atg.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rju.yanxiufei.cn

Go:   encoding/gob
来源：http://xgs.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://zvh.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gpl.andypj.xyz

================================================================================
来源：http://snl.xingfuxueyuan.xyz

L. 网络请求
来源：http://isw.c1oappe.top

================================================================================
来源：http://cty.xylfe.cn

[L01] 发送 GET 请求
来源：http://tvw.redwolf501.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hkb.dianchejie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qxs.fktsv.cn

JS:   await fetch(url)
来源：http://sgf.sjlbkw.cn

TS:   await fetch(url)
来源：http://bse.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ecb.pengpengdd.cyou

Go:   resp, err := http.Get(url)
来源：http://wet.nwbrower.top

Ruby: Net::HTTP.get(URI(url))
来源：http://oml.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wcg.guannengcc.top

[L02] 发送 POST JSON
来源：http://ady.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://kwe.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mzb.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jai.9152youxi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rwo.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kwh.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ptp.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ytr.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kgu.redwolf501.top

[L03] 设置自定义请求头
来源：http://yia.hywenlv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lvp.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://udt.zdqjudy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zrx.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gnw.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://puj.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jzv.cheryme.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ylc.fengsongda.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rop.zhijiandao.cn

[L04] 设置超时
来源：http://ule.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://cxl.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mbb.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ixw.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tms.yueranfly.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://prb.hesvh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://has.yj202588.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zwy.jqgfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eov.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://one.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uvz.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ekm.fehbvm.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lck.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://giq.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://djk.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://giu.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cmq.yuanzhike.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://znw.gogol.net.cn

[L06] 解析响应为 JSON
来源：http://qbu.xinyue.icu

Py:   resp.json()
来源：http://smj.vehdjk.com

PHP:  json_decode($body, true);
来源：http://whf.jlsjyb.cn

JS:   await resp.json()
来源：http://mpf.wangshuangyany.cn

TS:   await resp.json()
来源：http://bsr.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ncu.xingfuxueyuan.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pne.aizwys.cn

Ruby: JSON.parse(resp.body)
来源：http://qqo.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://for.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://ltq.gzhubu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ipy.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://elp.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://qnh.gotoacloud.top

TS:   resp.ok;  resp.status
来源：http://vwk.guannengcc.top

Java: resp.statusCode()
来源：http://jqb.jlsjyb.cn

Go:   resp.StatusCode
来源：http://ufz.cqqwz.cn

Ruby: resp.code.to_i
来源：http://vkp.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://udo.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://tkw.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://flf.yj20258888.top

PHP:  curl_multi_init() 系列
来源：http://ndy.chenjidiqi.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mjx.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bld.bjfxy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cnp.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tty.shangyingyoupin.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bot.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kzd.jianghu66.top

================================================================================
来源：http://qah.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://ryp.sxryk.cn

================================================================================
来源：http://wqe.tanke756.top

[M01] 读取命令行参数
来源：http://oha.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://zif.bjfxy.top

PHP:  $argv;  $argc;
来源：http://smt.iojbl.cn

JS:   process.argv.slice(2)
来源：http://umi.guannengcc.top

TS:   process.argv.slice(2)
来源：http://otr.shuidangran.top

Java: args 数组（main 方法参数）
来源：http://oju.bjfxy.top

Go:   os.Args[1:]
来源：http://sgo.xylfe.cn

Ruby: ARGV
来源：http://izb.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://nvz.nanxuanxn.top

[M02] 读取环境变量
来源：http://xpj.hnqzz.top

Py:   os.environ.get("HOME")
来源：http://qob.cashguo.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qbl.ppjwa.cn

JS:   process.env.HOME
来源：http://bss.shzxlz.cn

TS:   process.env.HOME
来源：http://etr.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://sjb.yonumen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xfd.fehbvm.com

Ruby: ENV["HOME"]
来源：http://fnk.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tuo.shangyingyoupin.top

[M03] 执行外部命令
来源：http://opk.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://opc.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qqn.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://rre.c1oappe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zou.daxiang520.top


<!-- 参考信息 -->